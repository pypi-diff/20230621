# Comparing `tmp/cysecuretools-4.2.0.tar.gz` & `tmp/cysecuretools-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cysecuretools-4.2.0.tar", last modified: Thu May 18 10:54:49 2023, max compression
+gzip compressed data, was "cysecuretools-5.0.0.tar", last modified: Wed Jun 21 10:27:08 2023, max compression
```

## Comparing `cysecuretools-4.2.0.tar` & `cysecuretools-5.0.0.tar`

### file list

```diff
@@ -1,406 +1,443 @@
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.510923 cysecuretools-4.2.0/
--rw-r--r--   0 ihos       (501) staff       (20)     2674 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/CHANGELOG.md
--rw-r--r--   0 ihos       (501) staff       (20)      582 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/LICENSE
--rw-r--r--   0 ihos       (501) staff       (20)      970 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/MANIFEST.in
--rw-r--r--   0 ihos       (501) staff       (20)    10995 2023-05-18 10:54:49.510355 cysecuretools-4.2.0/PKG-INFO
--rw-r--r--   0 ihos       (501) staff       (20)     7575 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/README.md
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.976153 cysecuretools-4.2.0/cysecuretools/
--rw-r--r--   0 ihos       (501) staff       (20)      631 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)      714 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/__main__.py
--rw-r--r--   0 ihos       (501) staff       (20)    11340 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/cli.py
--rw-r--r--   0 ihos       (501) staff       (20)     6113 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/cli_creator.py
--rw-r--r--   0 ihos       (501) staff       (20)    32939 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/cli_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)    27673 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/cli_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.149679 cysecuretools-4.2.0/cysecuretools/core/
--rw-r--r--   0 ihos       (501) staff       (20)     1098 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)      784 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/bitops.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.157485 cysecuretools-4.2.0/cysecuretools/core/certificates/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/certificates/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     9951 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/certificates/x509.py
--rw-r--r--   0 ihos       (501) staff       (20)     5168 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/connect_helper.py
--rw-r--r--   0 ihos       (501) staff       (20)     2230 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/cy_bootloader_map_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)     1259 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/dependecy_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1191 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/deprecated.py
--rw-r--r--   0 ihos       (501) staff       (20)      945 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/entrance_exam_base.py
--rw-r--r--   0 ihos       (501) staff       (20)     1450 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/enums.py
--rw-r--r--   0 ihos       (501) staff       (20)      736 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/exceptions.py
--rw-r--r--   0 ihos       (501) staff       (20)     1469 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/json_helper.py
--rw-r--r--   0 ihos       (501) staff       (20)     1674 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/jsonpath.py
--rw-r--r--   0 ihos       (501) staff       (20)     2144 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/key_data.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.176950 cysecuretools-4.2.0/cysecuretools/core/key_handlers/
--rw-r--r--   0 ihos       (501) staff       (20)       67 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/key_handlers/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2539 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/key_handlers/ec_handler.py
--rw-r--r--   0 ihos       (501) staff       (20)     3889 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/key_handlers/rsa_handler.py
--rw-r--r--   0 ihos       (501) staff       (20)     2280 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/key_helper.py
--rw-r--r--   0 ihos       (501) staff       (20)     2434 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/logging_configurator.py
--rw-r--r--   0 ihos       (501) staff       (20)     2401 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/logging_formatter.py
--rw-r--r--   0 ihos       (501) staff       (20)      701 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/memory_area.py
--rw-r--r--   0 ihos       (501) staff       (20)     2253 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/memory_map_base.py
--rw-r--r--   0 ihos       (501) staff       (20)     3161 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/mtb_tools_discovery.py
--rw-r--r--   0 ihos       (501) staff       (20)     2209 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/ocd_settings.py
--rw-r--r--   0 ihos       (501) staff       (20)      840 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/policy_filter_base.py
--rw-r--r--   0 ihos       (501) staff       (20)      954 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/policy_validator_base.py
--rw-r--r--   0 ihos       (501) staff       (20)      783 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/progress_bar.py
--rw-r--r--   0 ihos       (501) staff       (20)     6765 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/project.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.190496 cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/
--rw-r--r--   0 ihos       (501) staff       (20)      134 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)      716 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/application.py
--rw-r--r--   0 ihos       (501) staff       (20)      894 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/flow.py
--rw-r--r--   0 ihos       (501) staff       (20)     3267 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/register_map_base.py
--rw-r--r--   0 ihos       (501) staff       (20)     1216 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/signtool_base.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.216458 cysecuretools-4.2.0/cysecuretools/core/strategy_context/
--rw-r--r--   0 ihos       (501) staff       (20)      107 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/strategy_context/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2062 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/strategy_context/cert_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)     2812 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/strategy_context/encrypted_programming_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)     1997 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/strategy_context/prov_packet_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)     2890 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/strategy_context/provisioning_strategy_ctx.py
--rw-r--r--   0 ihos       (501) staff       (20)      716 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/strops.py
--rw-r--r--   0 ihos       (501) staff       (20)     4306 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/target_builder.py
--rw-r--r--   0 ihos       (501) staff       (20)    11714 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/core/target_director.py
--rw-r--r--   0 ihos       (501) staff       (20)      847 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/core/voltage_tool.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.221202 cysecuretools-4.2.0/cysecuretools/data/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/data/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1579 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/data/cy_bootloader_map.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.228789 cysecuretools-4.2.0/cysecuretools/data/mxs40sv2/
--rw-r--r--   0 ihos       (501) staff       (20)     4698 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.237971 cysecuretools-4.2.0/cysecuretools/data/mxs40v1/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/data/mxs40v1/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)    13578 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/data/mxs40v1/mxs40v1_sfb_status_codes.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.284675 cysecuretools-4.2.0/cysecuretools/execute/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3086 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/bootloader_provider_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.302133 cysecuretools-4.2.0/cysecuretools/execute/debug_cert/
--rw-r--r--   0 ihos       (501) staff       (20)       97 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/debug_cert/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2924 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/debug_cert/debug_cert_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     4365 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/debug_cert/debug_cert_parser_mxs40sv2.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.335268 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2459 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_cipher.py
--rw-r--r--   0 ihos       (501) staff       (20)     4024 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_header.py
--rw-r--r--   0 ihos       (501) staff       (20)     5550 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_header_strategy.py
--rw-r--r--   0 ihos       (501) staff       (20)     2857 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/ecc_kdf.py
--rw-r--r--   0 ihos       (501) staff       (20)     3204 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/encrypted_programming.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.348715 cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     8164 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/exam_cyb06xx7.py
--rw-r--r--   0 ihos       (501) staff       (20)     8849 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/exam_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)     5062 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_cert.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.392051 cysecuretools-4.2.0/cysecuretools/execute/image_signing/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3152 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/encrypt_mxv40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     7260 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/image.py
--rw-r--r--   0 ihos       (501) staff       (20)     1450 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/image_config_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)     3782 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/rsa_converter.py
--rw-r--r--   0 ihos       (501) staff       (20)    18698 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/signtool_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)    17625 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/signtool_mxv40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     1231 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/image_signing/xip_encryptor.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.426820 cysecuretools-4.2.0/cysecuretools/execute/imgtool/
--rw-r--r--   0 ihos       (501) staff       (20)      650 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1613 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/boot_record.py
--rw-r--r--   0 ihos       (501) staff       (20)     1208 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/custom_encryptor.py
--rw-r--r--   0 ihos       (501) staff       (20)    25962 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/image.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.482580 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/
--rw-r--r--   0 ihos       (501) staff       (20)     3737 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5388 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ecdsa.py
--rw-r--r--   0 ihos       (501) staff       (20)     2970 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ecdsa_test.py
--rw-r--r--   0 ihos       (501) staff       (20)     3090 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ed25519.py
--rw-r--r--   0 ihos       (501) staff       (20)     3026 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ed25519_test.py
--rw-r--r--   0 ihos       (501) staff       (20)     1822 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/general.py
--rw-r--r--   0 ihos       (501) staff       (20)     5422 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/rsa.py
--rw-r--r--   0 ihos       (501) staff       (20)     3810 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/rsa_test.py
--rw-r--r--   0 ihos       (501) staff       (20)     3169 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/x25519.py
--rwxr-xr-x   0 ihos       (501) staff       (20)    18214 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/main.py
--rw-r--r--   0 ihos       (501) staff       (20)     1773 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/imgtool/version.py
--rw-r--r--   0 ihos       (501) staff       (20)     2587 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/jwt.py
--rw-r--r--   0 ihos       (501) staff       (20)     3924 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/key_reader.py
--rw-r--r--   0 ihos       (501) staff       (20)     1956 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/key_reader_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.498247 cysecuretools-4.2.0/cysecuretools/execute/key_source/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/key_source/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5174 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/key_source/key_source_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)      825 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/key_source/key_source_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)     8251 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/keygen.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.555964 cysecuretools-4.2.0/cysecuretools/execute/programmer/
--rw-r--r--   0 ihos       (501) staff       (20)      658 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     8209 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/base.py
--rw-r--r--   0 ihos       (501) staff       (20)    12720 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/openocd_server.py
--rw-r--r--   0 ihos       (501) staff       (20)      938 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/openocd_target_map.json
--rw-r--r--   0 ihos       (501) staff       (20)    22128 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/openocd_wrapper.py
--rw-r--r--   0 ihos       (501) staff       (20)     1009 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/programmer.py
--rw-r--r--   0 ihos       (501) staff       (20)     1427 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/pyocd_target_map.json
--rw-r--r--   0 ihos       (501) staff       (20)    16156 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/programmer/pyocd_wrapper.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.572987 cysecuretools-4.2.0/cysecuretools/execute/project_init/
--rw-r--r--   0 ihos       (501) staff       (20)      122 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/project_init/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     7365 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/project_init/project_init_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     7933 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/project_init/project_init_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.606679 cysecuretools-4.2.0/cysecuretools/execute/provisioning/
--rw-r--r--   0 ihos       (501) staff       (20)      200 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.627815 cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/
--rw-r--r--   0 ihos       (501) staff       (20)      181 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5753 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/application_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     3484 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/flow_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     8975 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/load_ram_app.py
--rw-r--r--   0 ihos       (501) staff       (20)     7139 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/provision_device_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)    21411 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning/provision_device_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.645562 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/
--rw-r--r--   0 ihos       (501) staff       (20)      107 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.707965 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/
--rw-r--r--   0 ihos       (501) staff       (20)      564 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5407 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_crypto.py
--rw-r--r--   0 ihos       (501) staff       (20)     1581 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_customer.py
--rw-r--r--   0 ihos       (501) staff       (20)     3514 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_dev.py
--rw-r--r--   0 ihos       (501) staff       (20)     1731 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_entity.py
--rw-r--r--   0 ihos       (501) staff       (20)     3428 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_hsm.py
--rw-r--r--   0 ihos       (501) staff       (20)     3153 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_oem.py
--rw-r--r--   0 ihos       (501) staff       (20)     3672 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_pem.py
--rw-r--r--   0 ihos       (501) staff       (20)     1049 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_types.py
--rw-r--r--   0 ihos       (501) staff       (20)     6784 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     8310 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.732637 cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/
--rw-r--r--   0 ihos       (501) staff       (20)     1218 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3893 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     2856 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)    22517 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/sys_call.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.749827 cysecuretools-4.2.0/cysecuretools/execute/version_provider/
--rw-r--r--   0 ihos       (501) staff       (20)      124 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/version_provider/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     5951 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/version_provider/version_provider_mxs40sv2.py
--rw-r--r--   0 ihos       (501) staff       (20)     8684 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/execute/version_provider/version_provider_mxs40v1.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.762015 cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     3139 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/lvd_voltage_picker.py
--rw-r--r--   0 ihos       (501) staff       (20)     1251 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/voltage_tool_mxs40v1.py
--rw-r--r--   0 ihos       (501) staff       (20)    40522 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/main.py
--rw-r--r--   0 ihos       (501) staff       (20)      718 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/pkg_globals.py
--rw-r--r--   0 ihos       (501) staff       (20)       79 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/settings.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.767948 cysecuretools-4.2.0/cysecuretools/targets/
--rw-r--r--   0 ihos       (501) staff       (20)     5662 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.768920 cysecuretools-4.2.0/cysecuretools/targets/common/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.824049 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/
--rw-r--r--   0 ihos       (501) staff       (20)      160 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1336 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset.py
--rw-r--r--   0 ihos       (501) staff       (20)     1376 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset_builder.py
--rw-r--r--   0 ihos       (501) staff       (20)     3073 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset_enums.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.864425 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/
--rw-r--r--   0 ihos       (501) staff       (20)     1201 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1964 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1304 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1919 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     3387 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/nv_counter_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1508 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1198 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py
--rw-r--r--   0 ihos       (501) staff       (20)     1151 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/enums.py
--rw-r--r--   0 ihos       (501) staff       (20)     3537 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/flow_parser.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.884601 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/
--rw-r--r--   0 ihos       (501) staff       (20)    24916 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)     2049 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)     7972 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)    29537 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_secure.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)     3282 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/nv_counter_calc.py
--rw-r--r--   0 ihos       (501) staff       (20)    12510 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/policy_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)     4182 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/policy_validator.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.918414 cysecuretools-4.2.0/cysecuretools/targets/common/p64/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)      839 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/enums.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.927355 cysecuretools-4.2.0/cysecuretools/targets/common/p64/json/
--rw-r--r--   0 ihos       (501) staff       (20)     4452 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/json/policy_template.json
--rw-r--r--   0 ihos       (501) staff       (20)    15796 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/json/schema.json_schema
--rw-r--r--   0 ihos       (501) staff       (20)     5756 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_filter.py
--rw-r--r--   0 ihos       (501) staff       (20)    15561 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_parser.py
--rw-r--r--   0 ihos       (501) staff       (20)    46232 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_validator.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.935210 cysecuretools-4.2.0/cysecuretools/targets/common/p64/prebuilt/
--rw-r--r--   0 ihos       (501) staff       (20)      511 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/prebuilt/hsm_state.json
--rw-r--r--   0 ihos       (501) staff       (20)      511 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/prebuilt/oem_state.json
--rw-r--r--   0 ihos       (501) staff       (20)     1381 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/p64/silicon_data_parser.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.938401 cysecuretools-4.2.0/cysecuretools/targets/common/prebuilt/
--rw-r--r--   0 ihos       (501) staff       (20)      173 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/common/prebuilt/bootloader_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.951127 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/
--rw-r--r--   0 ihos       (501) staff       (20)       75 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.954395 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.967235 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1599 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     2401 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/register_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:48.985546 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1051 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/cy_auth_512k_b0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.004017 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     5312 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     5314 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4_smif.json
--rw-r--r--   0 ihos       (501) staff       (20)     4927 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     4927 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4_smif.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.881461 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.013319 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/
--rw-r--r--   0 ihos       (501) staff       (20)   134553 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      536 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.022255 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/
--rw-r--r--   0 ihos       (501) staff       (20)   148119 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      540 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)     4562 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.029820 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.033059 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.047056 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     2001 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     2401 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/register_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.061004 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1031 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.099640 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     5095 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     5095 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json
--rw-r--r--   0 ihos       (501) staff       (20)     5740 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5739 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     4883 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4.json
--rw-r--r--   0 ihos       (501) staff       (20)     4883 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json
--rw-r--r--   0 ihos       (501) staff       (20)     5531 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5529 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_swap.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.886198 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.112820 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/
--rw-r--r--   0 ihos       (501) staff       (20)   138714 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      543 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.123089 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/
--rw-r--r--   0 ihos       (501) staff       (20)   150520 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      542 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)     4465 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.135164 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/
--rw-r--r--   0 ihos       (501) staff       (20)       75 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.137169 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.148477 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1692 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     2402 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/register_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.160752 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1051 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.181908 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6068 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5784 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5621 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5573 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_swap.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.890798 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.191202 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   138738 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      592 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.201285 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   155454 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      588 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)     4468 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.213719 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/
--rw-r--r--   0 ihos       (501) staff       (20)       75 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.216895 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      191 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/keys/cy_pub_key.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.232996 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/
--rw-r--r--   0 ihos       (501) staff       (20)      371 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/control_dap_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)     1031 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt
--rw-r--r--   0 ihos       (501) staff       (20)      151 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/ec_key_tmpl.json
--rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/entrance_exam.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.252777 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6068 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5784 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5621 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_smif_swap.json
--rw-r--r--   0 ihos       (501) staff       (20)     5573 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_swap.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.894629 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.262236 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   138738 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      592 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.272609 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/
--rw-r--r--   0 ihos       (501) staff       (20)   155454 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
--rw-r--r--   0 ihos       (501) staff       (20)      588 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
--rw-r--r--   0 ihos       (501) staff       (20)     4468 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.293330 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/
--rw-r--r--   0 ihos       (501) staff       (20)       74 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.326872 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     8407 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/asset_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     1020 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/load_app_data.py
--rw-r--r--   0 ihos       (501) staff       (20)      179 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/oem_assets.json
--rw-r--r--   0 ihos       (501) staff       (20)      858 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/prov_flows.json
--rw-r--r--   0 ihos       (501) staff       (20)       94 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/reprovisioning_assets.json
--rw-r--r--   0 ihos       (501) staff       (20)     9210 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/reverse_asset_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.334383 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      460 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/keys/pub_hci_0.pem
--rw-r--r--   0 ihos       (501) staff       (20)      460 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/keys/pub_hci_1.pem
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.345423 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/
--rw-r--r--   0 ihos       (501) staff       (20)        0 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/__init__.py
--rw-r--r--   0 ihos       (501) staff       (20)     1052 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/memory_map.py
--rw-r--r--   0 ihos       (501) staff       (20)     1715 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/register_map.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.353465 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.898919 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.368260 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/
--rw-r--r--   0 ihos       (501) staff       (20)      235 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/config.json
--rw-r--r--   0 ihos       (501) staff       (20)     7780 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      375 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.381095 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/
--rw-r--r--   0 ihos       (501) staff       (20)      241 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/config.json
--rw-r--r--   0 ihos       (501) staff       (20)    28868 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      264 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.392899 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/
--rw-r--r--   0 ihos       (501) staff       (20)      269 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/config.json
--rw-r--r--   0 ihos       (501) staff       (20)    28676 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      289 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/info.txt
--rw-r--r--   0 ihos       (501) staff       (20)      624 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/debug_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)      168 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/rsa_key_tmpl.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.413759 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6135 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_hci_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     6344 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)      374 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_reprovisioning_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     2099 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_reprovisioning_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     8568 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     2841 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy_generator.py
--rw-r--r--   0 ihos       (501) staff       (20)     4481 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829/target_builder.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.426161 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/
--rw-r--r--   0 ihos       (501) staff       (20)       79 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/__init__.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.435227 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/flows/
--rw-r--r--   0 ihos       (501) staff       (20)      179 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/flows/oem_assets.json
--rw-r--r--   0 ihos       (501) staff       (20)      858 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/flows/prov_flows.json
--rw-r--r--   0 ihos       (501) staff       (20)       94 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/flows/reprovisioning_assets.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.439997 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/keys/
--rw-r--r--   0 ihos       (501) staff       (20)      460 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/keys/pub_hci_0.pem
--rw-r--r--   0 ihos       (501) staff       (20)      460 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/keys/pub_hci_1.pem
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.446155 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.902629 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.456379 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/
--rw-r--r--   0 ihos       (501) staff       (20)      235 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/config.json
--rwxr-xr-x   0 ihos       (501) staff       (20)     7812 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      375 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.466198 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/
--rw-r--r--   0 ihos       (501) staff       (20)      241 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/config.json
--rwxr-xr-x   0 ihos       (501) staff       (20)    28836 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      264 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/info.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.476534 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/
--rw-r--r--   0 ihos       (501) staff       (20)      269 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/config.json
--rwxr-xr-x   0 ihos       (501) staff       (20)    28612 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
--rwxr-xr-x   0 ihos       (501) staff       (20)      289 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/info.txt
--rw-r--r--   0 ihos       (501) staff       (20)      624 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/debug_cert.json
--rw-r--r--   0 ihos       (501) staff       (20)      168 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/rsa_key_tmpl.json
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.494492 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/
--rw-r--r--   0 ihos       (501) staff       (20)     6135 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_hci_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     6344 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)      374 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_reprovisioning_no_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     1812 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_reprovisioning_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     8281 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_secure.json
--rw-r--r--   0 ihos       (501) staff       (20)     1185 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/target_builder.py
--rw-r--r--   0 ihos       (501) staff       (20)      613 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/cysecuretools/version.py
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:47.982369 cysecuretools-4.2.0/cysecuretools.egg-info/
--rw-r--r--   0 ihos       (501) staff       (20)    10995 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/PKG-INFO
--rw-r--r--   0 ihos       (501) staff       (20)    17340 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/SOURCES.txt
--rw-r--r--   0 ihos       (501) staff       (20)        1 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/dependency_links.txt
--rw-r--r--   0 ihos       (501) staff       (20)       63 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/entry_points.txt
--rw-r--r--   0 ihos       (501) staff       (20)      156 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/requires.txt
--rw-r--r--   0 ihos       (501) staff       (20)       14 2023-05-18 10:54:47.000000 cysecuretools-4.2.0/cysecuretools.egg-info/top_level.txt
-drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-05-18 10:54:49.509165 cysecuretools-4.2.0/docs/
--rw-r--r--   0 ihos       (501) staff       (20)    40778 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/docs/README_CYW20829.md
--rw-r--r--   0 ihos       (501) staff       (20)    40021 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/docs/README_PSOC64.md
--rw-r--r--   0 ihos       (501) staff       (20)      141 2023-05-18 10:27:19.000000 cysecuretools-4.2.0/pyproject.toml
--rw-r--r--   0 ihos       (501) staff       (20)       38 2023-05-18 10:54:49.511077 cysecuretools-4.2.0/setup.cfg
--rw-r--r--   0 ihos       (501) staff       (20)     2441 2023-05-18 10:29:21.000000 cysecuretools-4.2.0/setup.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.429350 cysecuretools-5.0.0/
+-rw-r--r--   0 ihos       (501) staff       (20)     2871 2023-06-21 08:45:39.000000 cysecuretools-5.0.0/CHANGELOG.md
+-rw-r--r--   0 ihos       (501) staff       (20)      676 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/LICENSE
+-rw-r--r--   0 ihos       (501) staff       (20)      669 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/MANIFEST.in
+-rw-r--r--   0 ihos       (501) staff       (20)    10331 2023-06-21 10:27:08.429109 cysecuretools-5.0.0/PKG-INFO
+-rw-r--r--   0 ihos       (501) staff       (20)     6674 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/README.md
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.755707 cysecuretools-5.0.0/cysecuretools.egg-info/
+-rw-r--r--   0 ihos       (501) staff       (20)    10331 2023-06-21 10:27:07.000000 cysecuretools-5.0.0/cysecuretools.egg-info/PKG-INFO
+-rw-r--r--   0 ihos       (501) staff       (20)    16400 2023-06-21 10:27:07.000000 cysecuretools-5.0.0/cysecuretools.egg-info/SOURCES.txt
+-rw-r--r--   0 ihos       (501) staff       (20)        1 2023-06-21 10:27:07.000000 cysecuretools-5.0.0/cysecuretools.egg-info/dependency_links.txt
+-rw-r--r--   0 ihos       (501) staff       (20)       63 2023-06-21 10:27:07.000000 cysecuretools-5.0.0/cysecuretools.egg-info/entry_points.txt
+-rw-r--r--   0 ihos       (501) staff       (20)      164 2023-06-21 10:27:07.000000 cysecuretools-5.0.0/cysecuretools.egg-info/requires.txt
+-rw-r--r--   0 ihos       (501) staff       (20)       14 2023-06-21 10:27:07.000000 cysecuretools-5.0.0/cysecuretools.egg-info/top_level.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.767825 cysecuretools-5.0.0/docs/
+-rw-r--r--   0 ihos       (501) staff       (20)    40726 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/docs/README_CYW20829.md
+-rw-r--r--   0 ihos       (501) staff       (20)    39599 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/docs/README_PSOC64.md
+-rw-r--r--   0 ihos       (501) staff       (20)    14181 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/docs/README_XMC7XXX.md
+-rw-r--r--   0 ihos       (501) staff       (20)      141 2023-06-21 08:41:33.000000 cysecuretools-5.0.0/pyproject.toml
+-rw-r--r--   0 ihos       (501) staff       (20)       38 2023-06-21 10:27:08.429395 cysecuretools-5.0.0/setup.cfg
+-rw-r--r--   0 ihos       (501) staff       (20)     2561 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/setup.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.815980 cysecuretools-5.0.0/src/
+-rw-r--r--   0 ihos       (501) staff       (20)      762 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/__about__.py
+-rw-r--r--   0 ihos       (501) staff       (20)      737 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)      700 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/__main__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    21227 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/api_common.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7177 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/api_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)    18433 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/api_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3950 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/api_traveo_t2g.py
+-rw-r--r--   0 ihos       (501) staff       (20)    22497 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/cli.py
+-rw-r--r--   0 ihos       (501) staff       (20)     6605 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/cli_creator.py
+-rw-r--r--   0 ihos       (501) staff       (20)    32964 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/cli_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)    27492 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/cli_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     6043 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/cli_traveo_t2g.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.899645 cysecuretools-5.0.0/src/core/
+-rw-r--r--   0 ihos       (501) staff       (20)     1217 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1037 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/bitops.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5075 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/connect_helper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1715 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/crc.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2230 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/cy_bootloader_map_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1259 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/dependecy_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1191 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/deprecated.py
+-rw-r--r--   0 ihos       (501) staff       (20)      945 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/entrance_exam_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1635 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/enums.py
+-rw-r--r--   0 ihos       (501) staff       (20)      736 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/exceptions.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1469 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/json_helper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1674 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/jsonpath.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2144 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/key_data.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.911105 cysecuretools-5.0.0/src/core/key_handlers/
+-rw-r--r--   0 ihos       (501) staff       (20)     3852 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/key_handlers/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4417 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/key_handlers/ec_handler.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3919 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/key_handlers/pem_key.py
+-rw-r--r--   0 ihos       (501) staff       (20)    15654 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/key_handlers/rsa_handler.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2422 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/key_helper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2472 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/logging_configurator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2453 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/logging_formatter.py
+-rw-r--r--   0 ihos       (501) staff       (20)      701 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/memory_area.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2253 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/memory_map_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3161 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/mtb_tools_discovery.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2562 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/ocd_settings.py
+-rw-r--r--   0 ihos       (501) staff       (20)      840 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/policy_filter_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)      911 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/policy_parser_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1034 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/policy_validator_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)      858 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/progress_bar.py
+-rw-r--r--   0 ihos       (501) staff       (20)    11374 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/project_base.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.917505 cysecuretools-5.0.0/src/core/provisioning_flows/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/provisioning_flows/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3655 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/provisioning_flows/app_loading_flow.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7642 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/provisioning_flows/application.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1002 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/ram_app_loader_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3267 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/register_map_base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4707 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/signtool_base.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.933970 cysecuretools-5.0.0/src/core/strategy_context/
+-rw-r--r--   0 ihos       (501) staff       (20)      498 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/strategy_context/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2769 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/strategy_context/cert_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2735 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/strategy_context/encrypted_programming_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2534 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/strategy_context/prov_packet_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2890 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/strategy_context/provisioning_strategy_ctx.py
+-rw-r--r--   0 ihos       (501) staff       (20)      716 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/strops.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4629 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/target_builder.py
+-rw-r--r--   0 ihos       (501) staff       (20)    12476 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/target_director.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5078 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/version_provider.py
+-rw-r--r--   0 ihos       (501) staff       (20)      847 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/core/voltage_tool.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.936803 cysecuretools-5.0.0/src/data/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/data/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1579 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/data/cy_bootloader_map.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.939301 cysecuretools-5.0.0/src/data/mxs22/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/data/mxs22/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4858 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/data/mxs22/mxs22_ram_app_status_codes.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.941985 cysecuretools-5.0.0/src/data/mxs40sv2/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/data/mxs40sv2/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4698 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.945194 cysecuretools-5.0.0/src/data/mxs40v1/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/data/mxs40v1/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    13578 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/data/mxs40v1/mxs40v1_sfb_status_codes.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.953333 cysecuretools-5.0.0/src/execute/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.959171 cysecuretools-5.0.0/src/execute/dfuht_commands/
+-rw-r--r--   0 ihos       (501) staff       (20)      734 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/dfuht_commands/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7004 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/dfuht_commands/dfuht_packet.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3488 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/dfuht_commands/dfuht_packet_creator.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.967407 cysecuretools-5.0.0/src/execute/image_signing/
+-rw-r--r--   0 ihos       (501) staff       (20)      709 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/image_signing/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    12155 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/image_signing/image.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1578 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/image_signing/image_config_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)    13339 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/image_signing/sign_tool.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.982138 cysecuretools-5.0.0/src/execute/imgtool/
+-rw-r--r--   0 ihos       (501) staff       (20)      650 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1613 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/boot_record.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1208 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/custom_encryptor.py
+-rw-r--r--   0 ihos       (501) staff       (20)    26031 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/image.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.000753 cysecuretools-5.0.0/src/execute/imgtool/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)     3847 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/keys/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5388 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/keys/ecdsa.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2970 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/keys/ecdsa_test.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3090 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/keys/ed25519.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3026 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/keys/ed25519_test.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1822 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/keys/general.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5428 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/keys/rsa.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3810 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/keys/rsa_test.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3169 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/keys/x25519.py
+-rwxr-xr-x   0 ihos       (501) staff       (20)    18219 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/main.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1773 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/imgtool/version.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4279 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/jwt.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3676 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/key_reader.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.007100 cysecuretools-5.0.0/src/execute/keygens/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/keygens/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1753 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/keygens/aes_keygen.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4044 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/keygens/ec_keygen.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4678 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/keygens/rsa_keygen.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.024790 cysecuretools-5.0.0/src/execute/programmer/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/programmer/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     6799 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/programmer/base.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8264 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/programmer/dfuht_runner.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8790 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/programmer/dfuht_wrapper.py
+-rw-r--r--   0 ihos       (501) staff       (20)    13257 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/programmer/openocd_server.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1731 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/programmer/openocd_target_map.json
+-rw-r--r--   0 ihos       (501) staff       (20)    22526 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/programmer/openocd_wrapper.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1273 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/programmer/programmer.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.028675 cysecuretools-5.0.0/src/execute/project_init/
+-rw-r--r--   0 ihos       (501) staff       (20)      729 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/project_init/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8549 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/project_init/project_init.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1089 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/execute/silicon_data_reader.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3187 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/main.py
+-rw-r--r--   0 ihos       (501) staff       (20)      734 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/pkg_globals.py
+-rw-r--r--   0 ihos       (501) staff       (20)      502 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/settings.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.030759 cysecuretools-5.0.0/src/targets/
+-rw-r--r--   0 ihos       (501) staff       (20)     4025 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.038749 cysecuretools-5.0.0/src/targets/common/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1561 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/dependencies_validation.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3527 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/flow_parser.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.068133 cysecuretools-5.0.0/src/targets/common/mxs40sv2/
+-rw-r--r--   0 ihos       (501) staff       (20)     1329 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1336 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/asset.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1285 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/asset_builder.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3073 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/asset_enums.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.073694 cysecuretools-5.0.0/src/targets/common/mxs40sv2/debug_cert/
+-rw-r--r--   0 ihos       (501) staff       (20)      742 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/debug_cert/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3141 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4365 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_parser_mxs40sv2.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.087105 cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1929 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1295 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2098 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3387 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/nv_counter_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1500 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1189 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1828 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependency_validator_mxs40v2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1151 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/enums.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.096462 cysecuretools-5.0.0/src/targets/common/mxs40sv2/image_signing/
+-rw-r--r--   0 ihos       (501) staff       (20)      732 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/image_signing/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3243 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/image_signing/encrypt_mxv40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)    17996 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/image_signing/signtool_mxv40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1325 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/image_signing/xip_encryptor_mxs40sv2.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.102675 cysecuretools-5.0.0/src/targets/common/mxs40sv2/json/
+-rw-r--r--   0 ihos       (501) staff       (20)    24916 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     2049 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     7972 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)    29537 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/json/cyw20829_secure.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     4920 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/key_source_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3282 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/nv_counter_calc.py
+-rw-r--r--   0 ihos       (501) staff       (20)    12563 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/policy_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1713 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/policy_validator_mxs40v2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2018 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/project_init_mxs40sv2.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.108579 cysecuretools-5.0.0/src/targets/common/mxs40sv2/provisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      802 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/provisioning/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     6955 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/provisioning/provision_device_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     9446 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/provisioning/ram_app_loader_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     7028 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/provisioning_packet_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3981 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/silicon_data_reader_mxs40sv2.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2917 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40sv2/version_provider_mxs40sv2.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.143878 cysecuretools-5.0.0/src/targets/common/mxs40v1/
+-rw-r--r--   0 ihos       (501) staff       (20)     1510 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3172 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/bootloader_provider_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.156105 cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/
+-rw-r--r--   0 ihos       (501) staff       (20)      735 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2561 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_cipher.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3830 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_header.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5396 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_header_strategy.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2957 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/ecc_kdf.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3227 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/encrypted_programming.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.163668 cysecuretools-5.0.0/src/targets/common/mxs40v1/entrance_exam/
+-rw-r--r--   0 ihos       (501) staff       (20)      778 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/entrance_exam/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8150 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/entrance_exam/exam_cyb06xx7.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8821 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/entrance_exam/exam_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)      839 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/enums.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5110 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/image_cert.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.166945 cysecuretools-5.0.0/src/targets/common/mxs40v1/json/
+-rw-r--r--   0 ihos       (501) staff       (20)     4452 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/json/policy_template.json
+-rw-r--r--   0 ihos       (501) staff       (20)    15796 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/json/schema.json_schema
+-rw-r--r--   0 ihos       (501) staff       (20)     1977 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/key_reader_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)      825 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/key_source_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5747 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/policy_filter.py
+-rw-r--r--   0 ihos       (501) staff       (20)    15539 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/policy_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)    46181 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/policy_validator.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.170028 cysecuretools-5.0.0/src/targets/common/mxs40v1/prebuilt/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/prebuilt/cy_pub_key.json
+-rw-r--r--   0 ihos       (501) staff       (20)      511 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/prebuilt/hsm_state.json
+-rw-r--r--   0 ihos       (501) staff       (20)      511 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/prebuilt/oem_state.json
+-rw-r--r--   0 ihos       (501) staff       (20)     8014 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/project_init_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.177143 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      742 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    20588 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning/provision_device_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)    22504 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning/sys_call.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.180916 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/
+-rw-r--r--   0 ihos       (501) staff       (20)      751 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.196584 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     5408 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_crypto.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1491 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_customer.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3380 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_dev.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1822 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_entity.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3295 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_hsm.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3019 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_oem.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1049 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_types.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8651 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/provisioning_packet_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)    17211 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/signtool_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1441 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/silicon_data_parser.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2841 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/silicon_data_reader_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     8744 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/version_provider_mxs40v1.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.202075 cysecuretools-5.0.0/src/targets/common/mxs40v1/voltage_tool/
+-rw-r--r--   0 ihos       (501) staff       (20)      737 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/voltage_tool/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     3215 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/voltage_tool/lvd_voltage_picker.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1327 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/voltage_tool/voltage_tool_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)    10084 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/mxs40v1/x509_mxs40v1.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4453 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/policy_validator.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.203228 cysecuretools-5.0.0/src/targets/common/prebuilt/
+-rw-r--r--   0 ihos       (501) staff       (20)      173 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/prebuilt/bootloader_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.208292 cysecuretools-5.0.0/src/targets/common/traveo_t2g/
+-rw-r--r--   0 ihos       (501) staff       (20)      725 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/traveo_t2g/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)    12799 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/common/traveo_t2g/signtool_xmc7xxx.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.214323 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/
+-rw-r--r--   0 ihos       (501) staff       (20)     1242 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.215135 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.219545 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1681 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2385 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/maps/register_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.224539 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1051 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/packets/cy_auth_512k_b0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.230978 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     5498 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5500 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4_smif.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5111 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/policy/policy_single_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5111 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/policy/policy_single_CM0_CM4_smif.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.717046 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.235736 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/
+-rw-r--r--   0 ihos       (501) staff       (20)   134553 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      536 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.239651 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/
+-rw-r--r--   0 ihos       (501) staff       (20)   148119 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      540 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)     3936 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx5_a1/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.243907 cysecuretools-5.0.0/src/targets/cyb06xx7/
+-rw-r--r--   0 ihos       (501) staff       (20)     1548 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.244617 cysecuretools-5.0.0/src/targets/cyb06xx7/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.249206 cysecuretools-5.0.0/src/targets/cyb06xx7/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1991 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2391 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/maps/register_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.254075 cysecuretools-5.0.0/src/targets/cyb06xx7/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1031 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.267894 cysecuretools-5.0.0/src/targets/cyb06xx7/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     5115 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5115 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5740 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5739 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4903 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4903 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5531 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5529 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_swap.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.718186 cysecuretools-5.0.0/src/targets/cyb06xx7/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.272749 cysecuretools-5.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/
+-rw-r--r--   0 ihos       (501) staff       (20)   138714 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      543 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.277691 cysecuretools-5.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/
+-rw-r--r--   0 ihos       (501) staff       (20)   150520 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      542 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)     3799 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xx7/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.282153 cysecuretools-5.0.0/src/targets/cyb06xxa/
+-rw-r--r--   0 ihos       (501) staff       (20)     1147 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.282888 cysecuretools-5.0.0/src/targets/cyb06xxa/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.287351 cysecuretools-5.0.0/src/targets/cyb06xxa/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1682 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2392 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/maps/register_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.292127 cysecuretools-5.0.0/src/targets/cyb06xxa/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1051 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.298693 cysecuretools-5.0.0/src/targets/cyb06xxa/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6084 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5800 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5637 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5589 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/policy/policy_single_CM0_CM4_swap.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.730357 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.303856 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/
+-rw-r--r--   0 ihos       (501) staff       (20)   158689 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      543 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.307758 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   138738 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      592 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.311690 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/
+-rw-r--r--   0 ihos       (501) staff       (20)   172504 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      544 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.315818 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   155454 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      588 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)     3802 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyb06xxa/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.320885 cysecuretools-5.0.0/src/targets/cys06xxa/
+-rw-r--r--   0 ihos       (501) staff       (20)     1151 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.322108 cysecuretools-5.0.0/src/targets/cys06xxa/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      191 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/keys/cy_pub_key.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.326660 cysecuretools-5.0.0/src/targets/cys06xxa/packets/
+-rw-r--r--   0 ihos       (501) staff       (20)      371 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/packets/control_dap_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1031 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      151 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/packets/ec_key_tmpl.json
+-rw-r--r--   0 ihos       (501) staff       (20)     4490 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/packets/entrance_exam.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.333370 cysecuretools-5.0.0/src/targets/cys06xxa/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6084 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5800 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/policy/policy_multi_CM0_CM4_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5637 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/policy/policy_single_CM0_CM4_smif_swap.json
+-rw-r--r--   0 ihos       (501) staff       (20)     5589 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/policy/policy_single_CM0_CM4_swap.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.743614 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.337408 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/
+-rw-r--r--   0 ihos       (501) staff       (20)   158689 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      543 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.341779 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   138738 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      592 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.345307 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/
+-rw-r--r--   0 ihos       (501) staff       (20)   172504 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      544 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.350999 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/
+-rw-r--r--   0 ihos       (501) staff       (20)   155454 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex
+-rw-r--r--   0 ihos       (501) staff       (20)      588 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt
+-rw-r--r--   0 ihos       (501) staff       (20)      804 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cys06xxa/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.358223 cysecuretools-5.0.0/src/targets/cyw20829/
+-rw-r--r--   0 ihos       (501) staff       (20)     1196 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.362024 cysecuretools-5.0.0/src/targets/cyw20829/flows/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/flows/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)      179 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/flows/oem_assets.json
+-rw-r--r--   0 ihos       (501) staff       (20)      858 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/flows/prov_flows.json
+-rw-r--r--   0 ihos       (501) staff       (20)       94 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/flows/reprovisioning_assets.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.364276 cysecuretools-5.0.0/src/targets/cyw20829/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/keys/pub_hci_0.pem
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/keys/pub_hci_1.pem
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.373661 cysecuretools-5.0.0/src/targets/cyw20829/maps/
+-rw-r--r--   0 ihos       (501) staff       (20)        0 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/maps/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     9431 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/maps/asset_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1052 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/maps/memory_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     1705 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/maps/register_map.py
+-rw-r--r--   0 ihos       (501) staff       (20)     9308 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/maps/reverse_asset_map.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.376380 cysecuretools-5.0.0/src/targets/cyw20829/packets/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.744971 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.381304 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/prov_oem/
+-rw-r--r--   0 ihos       (501) staff       (20)      235 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/prov_oem/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)     7780 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      375 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/prov_oem/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.385344 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/reprovisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      241 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/reprovisioning/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)    28868 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      264 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/reprovisioning/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.389692 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/to_rma/
+-rw-r--r--   0 ihos       (501) staff       (20)      269 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/to_rma/config.json
+-rw-r--r--   0 ihos       (501) staff       (20)    28676 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      289 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/to_rma/info.txt
+-rw-r--r--   0 ihos       (501) staff       (20)      624 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/packets/debug_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)      168 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/packets/rsa_key_tmpl.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.398213 cysecuretools-5.0.0/src/targets/cyw20829/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6135 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/policy/policy_hci_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     6344 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/policy/policy_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)      374 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/policy/policy_reprovisioning_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     2099 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/policy/policy_reprovisioning_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     8568 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/policy/policy_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     2953 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/policy_generator.py
+-rw-r--r--   0 ihos       (501) staff       (20)     4038 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.402630 cysecuretools-5.0.0/src/targets/cyw20829_a0/
+-rw-r--r--   0 ihos       (501) staff       (20)      984 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/__init__.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.406032 cysecuretools-5.0.0/src/targets/cyw20829_a0/flows/
+-rw-r--r--   0 ihos       (501) staff       (20)      179 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/flows/oem_assets.json
+-rw-r--r--   0 ihos       (501) staff       (20)      858 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/flows/prov_flows.json
+-rw-r--r--   0 ihos       (501) staff       (20)       94 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/flows/reprovisioning_assets.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.407415 cysecuretools-5.0.0/src/targets/cyw20829_a0/keys/
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/keys/pub_hci_0.pem
+-rw-r--r--   0 ihos       (501) staff       (20)      460 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/keys/pub_hci_1.pem
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.409442 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:07.746310 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.412367 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/prov_oem/
+-rw-r--r--   0 ihos       (501) staff       (20)      235 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/prov_oem/config.json
+-rwxr-xr-x   0 ihos       (501) staff       (20)     7812 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      375 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/prov_oem/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.415527 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/
+-rw-r--r--   0 ihos       (501) staff       (20)      241 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/config.json
+-rwxr-xr-x   0 ihos       (501) staff       (20)    28836 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      264 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/info.txt
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.418857 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/to_rma/
+-rw-r--r--   0 ihos       (501) staff       (20)      269 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/to_rma/config.json
+-rwxr-xr-x   0 ihos       (501) staff       (20)    28612 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin
+-rwxr-xr-x   0 ihos       (501) staff       (20)      289 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/to_rma/info.txt
+-rw-r--r--   0 ihos       (501) staff       (20)      624 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/debug_cert.json
+-rw-r--r--   0 ihos       (501) staff       (20)      168 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/rsa_key_tmpl.json
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.424857 cysecuretools-5.0.0/src/targets/cyw20829_a0/policy/
+-rw-r--r--   0 ihos       (501) staff       (20)     6135 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/policy/policy_hci_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     6344 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/policy/policy_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)      374 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/policy/policy_reprovisioning_no_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1812 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/policy/policy_reprovisioning_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     8281 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/policy/policy_secure.json
+-rw-r--r--   0 ihos       (501) staff       (20)     1286 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/cyw20829_a0/target_builder.py
+drwxr-xr-x   0 ihos       (501) staff       (20)        0 2023-06-21 10:27:08.428754 cysecuretools-5.0.0/src/targets/xmc7xxx/
+-rw-r--r--   0 ihos       (501) staff       (20)     1124 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/xmc7xxx/__init__.py
+-rw-r--r--   0 ihos       (501) staff       (20)     2544 2023-06-21 08:44:23.000000 cysecuretools-5.0.0/src/targets/xmc7xxx/target_builder.py
```

### Comparing `cysecuretools-4.2.0/CHANGELOG.md` & `cysecuretools-5.0.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
+## 5.0.0
+### Changed
+- Removed pyOCD support. OpenOCD is used as a default On-Chip debugger for all platforms
+- High-level API module refactoring
+
+### Added
+- Support for XMC7100, XMC7200 devices
+
 ## 4.2.0
 ### Added
 - Support for CYW20829 B0 silicon revision
 - Multi-image NV counter for CYW20829
 - Transition PSoC 64 devices to RMA LCS
 - Open PSoC 64 devices in RMA LCS for debugging
 - OpenOCD autodiscovery in ModusToolbox directory
```

### Comparing `cysecuretools-4.2.0/LICENSE` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/provisioning/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-Copyright (c) 2019-2023 Cypress Semiconductor Corporation
+"""
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
-limitations under the License.
+limitations under the License.
+"""
+from .provision_device_mxs40sv2 import ProvisioningMXS40Sv2
+from .ram_app_loader_mxs40sv2 import RamAppLoaderMXS40Sv2
```

### Comparing `cysecuretools-4.2.0/PKG-INFO` & `cysecuretools-5.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cysecuretools
-Version: 4.2.0
-Summary: Cypress secure tools for Python
-Home-page: https://github.com/cypresssemiconductorco/cysecuretools
-Author: Cypress Semiconductor
+Version: 5.0.0
+Summary: Python tools for provisioning Cypress/Infineon MCUs
+Home-page: https://github.com/Infineon/cysecuretools
+Author: Cypress Semiconductor Corporation (an Infineon company)
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,34 +17,34 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This package contains security tools for creating keys, creating certificates, signing user applications, and provisioning Cypress MCUs.
 
 # Table of Contents
-- [HW/SW compatibility](#hwsw-compatibility)
 - [Prerequisites](#prerequisites)
 - [Documentation](#documentation)
 - [Installing package](#installing-package)
 - [Supported devices](#supported-devices)
 - [Interface and Usage](#interface-and-usage)
     - [PSoC 64](#psoc-64)
     - [CYW20829](#cyw20829)
+    - [XMC7100/7200](#xmc71007200)
 - [Logging](#logging)
 - [Installing libusb driver](#installing-libusb-driver)
 - [Known issues](#known-issues)
 - [License and Contributions](#license-and-contributions)
 
 # HW/SW compatibility
 ## PSoC 64
 <table>
   <thead>
     <tr>
       <td>Target/Kit</td>
-      <td>Silicon Revision</td>
+      <td>Silicon Revision<sup>1</sup></td>
       <td>Silicon ID, Silicon Rev., Family ID</td>
       <td>CySecureTools Version</td>
       <td>Secure FlashBoot Version</td>
       <td>CyBootloader Version</td>
     </tr>
   </thead>
   <tbody>
@@ -69,26 +69,26 @@
       <td>
         cyb06xxa<br>
         cy8ckit&#8209;064b0s2&#8209;4343w
       </td>
       <td>A1</td>
       <td>0xE470, 0x12, 0x102</td>
       <td>4.2.0</td>
-      <td>4.0.2.1842</td>
+      <td>4.0.3.2319</td>
       <td>2.0.2.8102</td>
     </tr>
     <tr>
       <td>
         cys06xxa<br>
         cy8ckit&#8209;064s0s2&#8209;4343w
       </td>
       <td>A1</td>
-      <td>0xE4A0, 0x12, 0x102</td>
+      <td>0xE4A0, 0x12, 0x02</td>
       <td>4.2.0</td>
-      <td>4.0.2.1842</td>
+      <td>4.0.3.2319</td>
       <td>2.0.2.8102</td>
     </tr>
     <tr>
       <td colspan="6" style="text-align: center;">1M</td>
     </tr>
     <tr>
       <td>
@@ -143,71 +143,57 @@
 
 <sup>1</sup> Specify `--rev` option for older revision of the silicon (e.g. `$ cysecuretools -t cyw20829 --rev a0 <COMMAND>`). Using the latest revision does not require specifying the option.
 
 # Prerequisites
 * General
   * Python 3.6 or later
 * For PSoC 64 devices
-  * In case of use PyOCD:
-    * [Installed the libusb driver](#installing-libusb-driver)
-    * Ensure the KitProg3 programming mode is **DAPLink**
-  * In case of use OpenOCD:
-    * [Installed Cypress OpenOCD](https://github.com/cypresssemiconductorco/openocd/releases)
-    * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk**
+  * [Installed Cypress OpenOCD](https://github.com/cypresssemiconductorco/openocd/releases)
+  * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk**
   * Ensure the power selection jumper is set to provide 2.5 V to the power supply pin related to eFuse power. This voltage level is required to blow eFuses
 * For CYW20829 devices
   * [Installed Cypress OpenOCD](https://github.com/cypresssemiconductorco/openocd/releases)
   * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk**
   * Ensure the power selection jumper is set to provide 2.5 V to the power supply pin related to eFuse power. This voltage level is required to blow eFuses
 
+
 # Documentation
 * [PSoC64 Secure MCU Secure Boot SDK User Guide](https://www.cypress.com/documentation/software-and-drivers/psoc-64-secure-mcu-secure-boot-sdk-user-guide)
-* [Changelog](CHANGELOG.md)
+* [Changelog](https://github.com/Infineon/cysecuretools/blob/master/CHANGELOG.md)
 
 # Installing Package
 Invoke `pip install` from the command line:
 ```bash
 $ pip install cysecuretools
 ```
+To update the already installed package:
+```bash
+$ pip install --upgrade --force-reinstall cysecuretools
+```
 
 
 # Supported devices
 Use `device-list` command for output of the supported devices list.
 ```bash
 $ cysecuretools device-list
 ```
 
 
 # Interface and Usage
 ## PSoC 64
-See [README_PSOC64.md](docs/README_PSOC64.md)
+See [README_PSOC64.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_PSOC64.md)
 ## CYW20829
-See [README_CYW20829.md](docs/README_CYW20829.md)
+See [README_CYW20829.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_CYW20829.md)
+## XMC7100/7200
+See [README_XMC7XXX.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_XMC7XXX.md)
 
 
 # Logging
 Every time the tool is invoked, a new log file is created in the _logs_ directory of the project. By default, the console output has INFO logging severity. The log file contains the DEBUG logging severity.
 
-When using _pyOCD_ as a debugger, the log files contain messages sent by both tools - _CySecureTools_ and _pyOCD_. When using _OpenOCD_, the log files contain messages from the package only. For the _OpenOCD_ messages, the additional files are created (e.g. _openocd_1.log_).
-
-
-# Installing libusb driver
-
-**Windows**
-  - Download and unzip libusb-1.0.25.7z from https://github.com/libusb/libusb/releases/tag/v1.0.25.
-  - Run the following command to determine if a Python shell is executing in 32-bit or 64-bit mode on the OS: `python -c "import struct; print(struct.calcsize('P') * 8)"`
-  - Copy *libusb-1.0.dll* file into the Python root folder (in same folder with *python.exe*). Use the 64-bit version of DLL for the 64-bit Python (MinGW64 directory) and the 32-bit version of DLL for the 32-bit Python (MinGW32 directory).
-  - Ensure the Python path is located at the beginning of the Path environment variable.
-
-**Mac OS**
-  - Use [homebrew](https://brew.sh/) to install the driver from the terminal: `homebrew install libusb`.
-
-**Linux**
-  - Bundled with the system, no need for additional installation.
-
 
 # Known issues
 - Using the policy from version 4.0.0 in projects created by version 4.1.0 causes the CY_FB_INVALID_IMG_JWT_SIGNATURE error during re-provisioning on PSoC64-2M devices:
 ```
   ...
   ERROR : SFB status: CY_FB_INVALID_IMG_JWT_SIGNATURE: Invalid image certificate signature. Check the log for details
 ```
@@ -246,14 +232,22 @@
 The software is provided under the Apache-2.0 license. Contributions to this project are accepted under the same license.
 This project contains code from other projects. The original license text is included in those source files.
 
 
 # Changelog
 All notable changes to this project will be documented in this file.
 
+## 5.0.0
+### Changed
+- Removed pyOCD support. OpenOCD is used as a default On-Chip debugger for all platforms
+- High-level API module refactoring
+
+### Added
+- Support for XMC7100, XMC7200 devices
+
 ## 4.2.0
 ### Added
 - Support for CYW20829 B0 silicon revision
 - Multi-image NV counter for CYW20829
 - Transition PSoC 64 devices to RMA LCS
 - Open PSoC 64 devices in RMA LCS for debugging
 - OpenOCD autodiscovery in ModusToolbox directory
```

#### html2text {}

```diff
@@ -1,99 +1,88 @@
-Metadata-Version: 2.1 Name: cysecuretools Version: 4.2.0 Summary: Cypress
-secure tools for Python Home-page: https://github.com/cypresssemiconductorco/
-cysecuretools Author: Cypress Semiconductor License: Apache 2.0 Platform:
-UNKNOWN Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Embedded Systems Requires-Python:
->=3.6 Description-Content-Type: text/markdown License-File: LICENSE This
-package contains security tools for creating keys, creating certificates,
-signing user applications, and provisioning Cypress MCUs. # Table of Contents -
-[HW/SW compatibility](#hwsw-compatibility) - [Prerequisites](#prerequisites) -
-[Documentation](#documentation) - [Installing package](#installing-package) -
-[Supported devices](#supported-devices) - [Interface and Usage](#interface-and-
-usage) - [PSoC 64](#psoc-64) - [CYW20829](#cyw20829) - [Logging](#logging) -
+Metadata-Version: 2.1 Name: cysecuretools Version: 5.0.0 Summary: Python tools
+for provisioning Cypress/Infineon MCUs Home-page: https://github.com/Infineon/
+cysecuretools Author: Cypress Semiconductor Corporation (an Infineon company)
+License: Apache 2.0 Platform: UNKNOWN Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
+:: OS Independent Classifier: Topic :: Software Development :: Embedded Systems
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE This package contains security tools for creating keys, creating
+certificates, signing user applications, and provisioning Cypress MCUs. # Table
+of Contents - [Prerequisites](#prerequisites) - [Documentation](#documentation)
+- [Installing package](#installing-package) - [Supported devices](#supported-
+devices) - [Interface and Usage](#interface-and-usage) - [PSoC 64](#psoc-64) -
+[CYW20829](#cyw20829) - [XMC7100/7200](#xmc71007200) - [Logging](#logging) -
 [Installing libusb driver](#installing-libusb-driver) - [Known issues](#known-
 issues) - [License and Contributions](#license-and-contributions) # HW/SW
 compatibility ## PSoC 64
-                                   Silicon
-                                   ID,                   Secure
-Target/Kit                Silicon  Silicon CySecureTools FlashBoot  CyBootloader
-                          Revision Rev.,   Version       Version    Version
-                                   Family
-                                   ID
+                                    Silicon
+                                    ID,                   Secure
+Target/Kit                Silicon   Silicon CySecureTools FlashBoot  CyBootloader
+                          Revision1 Rev.,   Version       Version    Version
+                                    Family
+                                    ID
 512K
-cyb06xx5                           0xE70D,
-cy8cproto‑064b0s3       A1       0x12,   4.2.0         4.0.2.1842 2.0.1.6441
-                                   0x105
+cyb06xx5                            0xE70D,
+cy8cproto‑064b0s3       A1        0x12,   4.2.0         4.0.2.1842 2.0.1.6441
+                                    0x105
 2M
-cyb06xxa                           0xE470,
-cy8ckit‑064b0s2‑4343w A1       0x12,   4.2.0         4.0.2.1842 2.0.2.8102
-                                   0x102
-cys06xxa                           0xE4A0,
-cy8ckit‑064s0s2‑4343w A1       0x12,   4.2.0         4.0.2.1842 2.0.2.8102
-                                   0x102
+cyb06xxa                            0xE470,
+cy8ckit‑064b0s2‑4343w A1        0x12,   4.2.0         4.0.3.2319 2.0.2.8102
+                                    0x102
+cys06xxa                            0xE4A0,
+cy8ckit‑064s0s2‑4343w A1        0x12,   4.2.0         4.0.3.2319 2.0.2.8102
+                                    0x02
 1M
-                                   0xE262,
-cyb06xx7                           0x24,
-cy8cproto‑064s1‑sb    B3       0x100   4.2.0         4.0.2.1842 2.0.0.4041
-cy8cproto‑064b0s1‑ble          0xE261,
-cy8cproto‑064b0s1‑ssa          0x24,
-                                   0x100
+                                    0xE262,
+cyb06xx7                            0x24,
+cy8cproto‑064s1‑sb    B3        0x100   4.2.0         4.0.2.1842 2.0.0.4041
+cy8cproto‑064b0s1‑ble           0xE261,
+cy8cproto‑064b0s1‑ssa           0x24,
+                                    0x100
 ## CYW20829
            Silicon   Silicon ID,   CySecureTools                 RAM
 Target/Kit Revision1 Silicon Rev., Version       BootROM Version Applications
                      Family ID                                   Version
 cyw20829   A0        0xEB40, 0x11, 4.2.0         1.0.0.7120      1.0.0.2857
                      0x110
 cyw20829   B0        0xEB43, 0x21, 4.2.0         1.2.0.8274      1.2.0.3073
                      0x110
 1 Specify `--rev` option for older revision of the silicon (e.g. `$
 cysecuretools -t cyw20829 --rev a0 `). Using the latest revision does not
 require specifying the option. # Prerequisites * General * Python 3.6 or later
-* For PSoC 64 devices * In case of use PyOCD: * [Installed the libusb driver]
-(#installing-libusb-driver) * Ensure the KitProg3 programming mode is
-**DAPLink** * In case of use OpenOCD: * [Installed Cypress OpenOCD](https://
-github.com/cypresssemiconductorco/openocd/releases) * Ensure the KitProg3
-programming mode is **CMSIS-DAP Bulk** * Ensure the power selection jumper is
-set to provide 2.5 V to the power supply pin related to eFuse power. This
-voltage level is required to blow eFuses * For CYW20829 devices * [Installed
-Cypress OpenOCD](https://github.com/cypresssemiconductorco/openocd/releases) *
-Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk** * Ensure the power
-selection jumper is set to provide 2.5 V to the power supply pin related to
-eFuse power. This voltage level is required to blow eFuses # Documentation *
-[PSoC64 Secure MCU Secure Boot SDK User Guide](https://www.cypress.com/
-documentation/software-and-drivers/psoc-64-secure-mcu-secure-boot-sdk-user-
-guide) * [Changelog](CHANGELOG.md) # Installing Package Invoke `pip install`
-from the command line: ```bash $ pip install cysecuretools ``` # Supported
-devices Use `device-list` command for output of the supported devices list.
-```bash $ cysecuretools device-list ``` # Interface and Usage ## PSoC 64 See
-[README_PSOC64.md](docs/README_PSOC64.md) ## CYW20829 See [README_CYW20829.md]
-(docs/README_CYW20829.md) # Logging Every time the tool is invoked, a new log
-file is created in the _logs_ directory of the project. By default, the console
-output has INFO logging severity. The log file contains the DEBUG logging
-severity. When using _pyOCD_ as a debugger, the log files contain messages sent
-by both tools - _CySecureTools_ and _pyOCD_. When using _OpenOCD_, the log
-files contain messages from the package only. For the _OpenOCD_ messages, the
-additional files are created (e.g. _openocd_1.log_). # Installing libusb driver
-**Windows** - Download and unzip libusb-1.0.25.7z from https://github.com/
-libusb/libusb/releases/tag/v1.0.25. - Run the following command to determine if
-a Python shell is executing in 32-bit or 64-bit mode on the OS: `python -
-c "import struct; print(struct.calcsize('P') * 8)"` - Copy *libusb-1.0.dll*
-file into the Python root folder (in same folder with *python.exe*). Use the
-64-bit version of DLL for the 64-bit Python (MinGW64 directory) and the 32-bit
-version of DLL for the 32-bit Python (MinGW32 directory). - Ensure the Python
-path is located at the beginning of the Path environment variable. **Mac OS** -
-Use [homebrew](https://brew.sh/) to install the driver from the terminal:
-`homebrew install libusb`. **Linux** - Bundled with the system, no need for
-additional installation. # Known issues - Using the policy from version 4.0.0
-in projects created by version 4.1.0 causes the CY_FB_INVALID_IMG_JWT_SIGNATURE
-error during re-provisioning on PSoC64-2M devices: ``` ... ERROR : SFB status:
+* For PSoC 64 devices * [Installed Cypress OpenOCD](https://github.com/
+cypresssemiconductorco/openocd/releases) * Ensure the KitProg3 programming mode
+is **CMSIS-DAP Bulk** * Ensure the power selection jumper is set to provide 2.5
+V to the power supply pin related to eFuse power. This voltage level is
+required to blow eFuses * For CYW20829 devices * [Installed Cypress OpenOCD]
+(https://github.com/cypresssemiconductorco/openocd/releases) * Ensure the
+KitProg3 programming mode is **CMSIS-DAP Bulk** * Ensure the power selection
+jumper is set to provide 2.5 V to the power supply pin related to eFuse power.
+This voltage level is required to blow eFuses # Documentation * [PSoC64 Secure
+MCU Secure Boot SDK User Guide](https://www.cypress.com/documentation/software-
+and-drivers/psoc-64-secure-mcu-secure-boot-sdk-user-guide) * [Changelog](https:
+//github.com/Infineon/cysecuretools/blob/master/CHANGELOG.md) # Installing
+Package Invoke `pip install` from the command line: ```bash $ pip install
+cysecuretools ``` To update the already installed package: ```bash $ pip
+install --upgrade --force-reinstall cysecuretools ``` # Supported devices Use
+`device-list` command for output of the supported devices list. ```bash $
+cysecuretools device-list ``` # Interface and Usage ## PSoC 64 See
+[README_PSOC64.md](https://github.com/Infineon/cysecuretools/blob/master/docs/
+README_PSOC64.md) ## CYW20829 See [README_CYW20829.md](https://github.com/
+Infineon/cysecuretools/blob/master/docs/README_CYW20829.md) ## XMC7100/7200 See
+[README_XMC7XXX.md](https://github.com/Infineon/cysecuretools/blob/master/docs/
+README_XMC7XXX.md) # Logging Every time the tool is invoked, a new log file is
+created in the _logs_ directory of the project. By default, the console output
+has INFO logging severity. The log file contains the DEBUG logging severity. #
+Known issues - Using the policy from version 4.0.0 in projects created by
+version 4.1.0 causes the CY_FB_INVALID_IMG_JWT_SIGNATURE error during re-
+provisioning on PSoC64-2M devices: ``` ... ERROR : SFB status:
 CY_FB_INVALID_IMG_JWT_SIGNATURE: Invalid image certificate signature. Check the
 log for details ``` _Workaround_: 1. Open the policy file. 2. Navigate to
 section 1 of the `boot_upgrade/firmware`. 3. Set `boot_auth` and
 `bootloader_keys` as follows: ``` "boot_auth": [ 3 ], "bootloader_keys": [
 { "kid": 3, "key": "../keys/cy_pub_key.json" } ] ``` - During the installation
 of the package via _pip_ on Mac OS Big Sur, the following exception is raised:
 ``` ... distutils.errors.DistutilsError: Setup script exited with error:
@@ -106,37 +95,39 @@
 EasyInstall maintainers to find out if a fix or workaround is available. ```
 _Solution:_ Upgrade the `pip` package running the following command from the
 terminal: `python3 -m pip install --upgrade pip`. # License and Contributions
 The software is provided under the Apache-2.0 license. Contributions to this
 project are accepted under the same license. This project contains code from
 other projects. The original license text is included in those source files. #
 Changelog All notable changes to this project will be documented in this file.
-## 4.2.0 ### Added - Support for CYW20829 B0 silicon revision - Multi-image NV
-counter for CYW20829 - Transition PSoC 64 devices to RMA LCS - Open PSoC 64
-devices in RMA LCS for debugging - OpenOCD autodiscovery in ModusToolbox
-directory - Add SW/HW compatibility table to the readme ### Changed - Target
-`cyw20829` is used for the latest silicon revision. For the previous silicon
-revision (A0) add _--rev_ option in the command line (`-t cyw20829 --rev a0`)
-## 4.1.0 ### Added - OpenOCD support for PSoC 64 devices - Creating update
-package in the unsigned image (_extend-image_ command) ### Changed - Fixed
-installation failure using pip 22.1 - CyBootloader 2.0.2.8102 for PSoC 64 2M: -
-Improved performance of SWAP algorithm - Image certificate signed with the
-Infineon key (id=3) - Use Infineon key (id=3) for bootloader in the policy
-files ## 4.0.0 ### Added - Support of CYW20829 devices - Support Python 3.10 -
-Signing images with HSM ### Changed - Separated PSoC 64 and CYW20829 devices
-CLI - Updated PSoC 64 CyBootloader for 512k and 2M: - added
-"reset_after_failure" feature - decreased boot time - Protect PSA API from NSPE
-in PSoC 64 2M-S0 policy - Prevent signing of already signed images - Change
-MCUboot image header padding to erase value - Use CyBootloader from the project
-directory if the project exists - Updated dependencies packages to the latest
-versions - Use pyocd 0.32.3 ## 3.1.1 ### Changed - Fixed installation failure
-on macOS Big Sur and Apple M1 chip - Fixed installation failure in Python 3.9
-## 3.1.0 ### Added - SCRATCH with Status Partition swap mode - Small image
-slots support in the external memory ## 3.0.0 ### Added - Image SWAP using
-Status Partition ### Changed - CyBootloader 2.0 - Secure Flash Boot 4.0.2
+## 5.0.0 ### Changed - Removed pyOCD support. OpenOCD is used as a default On-
+Chip debugger for all platforms - High-level API module refactoring ### Added -
+Support for XMC7100, XMC7200 devices ## 4.2.0 ### Added - Support for CYW20829
+B0 silicon revision - Multi-image NV counter for CYW20829 - Transition PSoC 64
+devices to RMA LCS - Open PSoC 64 devices in RMA LCS for debugging - OpenOCD
+autodiscovery in ModusToolbox directory - Add SW/HW compatibility table to the
+readme ### Changed - Target `cyw20829` is used for the latest silicon revision.
+For the previous silicon revision (A0) add _--rev_ option in the command line
+(`-t cyw20829 --rev a0`) ## 4.1.0 ### Added - OpenOCD support for PSoC 64
+devices - Creating update package in the unsigned image (_extend-image_
+command) ### Changed - Fixed installation failure using pip 22.1 - CyBootloader
+2.0.2.8102 for PSoC 64 2M: - Improved performance of SWAP algorithm - Image
+certificate signed with the Infineon key (id=3) - Use Infineon key (id=3) for
+bootloader in the policy files ## 4.0.0 ### Added - Support of CYW20829 devices
+- Support Python 3.10 - Signing images with HSM ### Changed - Separated PSoC 64
+and CYW20829 devices CLI - Updated PSoC 64 CyBootloader for 512k and 2M: -
+added "reset_after_failure" feature - decreased boot time - Protect PSA API
+from NSPE in PSoC 64 2M-S0 policy - Prevent signing of already signed images -
+Change MCUboot image header padding to erase value - Use CyBootloader from the
+project directory if the project exists - Updated dependencies packages to the
+latest versions - Use pyocd 0.32.3 ## 3.1.1 ### Changed - Fixed installation
+failure on macOS Big Sur and Apple M1 chip - Fixed installation failure in
+Python 3.9 ## 3.1.0 ### Added - SCRATCH with Status Partition swap mode - Small
+image slots support in the external memory ## 3.0.0 ### Added - Image SWAP
+using Status Partition ### Changed - CyBootloader 2.0 - Secure Flash Boot 4.0.2
 support ## 2.1.0 ### Added - Support PSoC64 1M - New command to read device die
 ID - Optionally add boot record to the signed image - New policy validators
 (address overlaps between images and bootloader, slots address alignment with
 the SMPU address limits, DAP closure, monotonic counter) - Log the device
 response JWT during the provisioning process ### Changed - Fixed issue with
 using group private key - Use pyocd 0.27.3 ## 2.0.0 ### Added - Support PSoC64
 2M, PSoC64 512K - Command line interface - Encrypted programming - Single-image
```

### Comparing `cysecuretools-4.2.0/cysecuretools/__init__.py` & `cysecuretools-5.0.0/src/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 """
-Copyright (c) 2019 Cypress Semiconductor Corporation
+Copyright (c) 2020 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.main import CySecureTools
+from .cli_creator import CliCreator
+
+
+def main():
+    CliCreator.create()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `cysecuretools-4.2.0/cysecuretools/__main__.py` & `cysecuretools-5.0.0/src/targets/cys06xxa/target_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.cli_creator import CliCreator
+from ..cyb06xxa import CYB06xxA_Builder
 
 
-def main():
-    CliCreator.create()
-
-
-if __name__ == '__main__':
-    main()
-
+class CYS06xxA_Builder(CYB06xxA_Builder):
+    """ CYS06xxA target builder """
```

### Comparing `cysecuretools-4.2.0/cysecuretools/cli_creator.py` & `cysecuretools-5.0.0/src/cli_creator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,47 +12,59 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import sys
+from importlib import import_module
+
 import click
 
-from cysecuretools.targets import target_data
-from cysecuretools import cli as base_cli
+from .core import package_name
+from .targets import target_data
+from . import cli as base_cli
 
 
 class CliCreator:
+    """Implements dynamic CLI layer creation and CLI validation"""
+
     @staticmethod
     def create():
+        """Dynamic CLI creation"""
         is_help = '--help' in sys.argv[1:]
 
         target = CliCreator.option_from_args(['-t', '--target'])
 
-        common_commands = CliCreator._command_list(base_cli.main)
-        if not any(a in common_commands for a in sys.argv[1:]):
-            if target is None and is_help:
-                CliCreator._print_help_instructions()
-                sys.stderr.write("Error: Missing option '-t' / '--target'.\n")
-                sys.exit(2)
-
-        CliCreator.validate_target_presence(target)
-
         platform = CliCreator._get_platform(target)
         if platform == 'mxs40sv2':
             if not is_help:
                 CliCreator.validate_policy_presence(target)
-            from cysecuretools import cli_mxs40sv2
-            cli_mxs40sv2.main()  # pylint: disable=no-value-for-parameter
+            module_name = 'cli_mxs40sv2'
         elif platform == 'psoc64':
-            from cysecuretools import cli_mxs40v1
-            cli_mxs40v1.main()  # pylint: disable=no-value-for-parameter
+            module_name = 'cli_mxs40v1'
+        elif platform == 'mxs22':
+            if not is_help:
+                CliCreator.validate_policy_presence(target)
+            module_name = 'cli_mxs22'
+        elif platform == 'traveo_t2g':
+            module_name = 'cli_traveo_t2g'
         else:
+            module_name = None if target else 'cli'
+
+        try:
+            module = import_module(f'.{module_name}', package=package_name())
+        except ModuleNotFoundError:
             CliCreator.unknown_target_error(target)
+            sys.exit(2)
+        else:
+            module.main(standalone_mode=not is_help)
+            common_commands = CliCreator._command_list(base_cli.main)
+            if not any(a in common_commands for a in sys.argv[1:]) and is_help:
+                CliCreator._print_help_instructions()
 
     @staticmethod
     def validate_target_presence(target):
         """ Validates 'target' option presence. Exits the process
         on error.
 
         Specifying target is necessary for all commands except the
@@ -73,15 +86,15 @@
         For the mxs40sv2 platform, specifying policy is necessary for
         all commands except the common commands (those which do not
         require specifying target) and 'init' command
         """
         platform = CliCreator._get_platform(target)
         if platform == 'mxs40sv2':
             common_cmds = CliCreator._command_list(base_cli.main)
-            from cysecuretools import cli_mxs40sv2
+            from . import cli_mxs40sv2
             mxs40v2_cmds = CliCreator._command_list(cli_mxs40sv2.main)
             mxs40v2_cmds = [c for c in mxs40v2_cmds if c not in common_cmds]
             mxs40v2_cmds.remove('init')
             mxs40v2_cmds.remove('extend-image')
             mxs40v2_cmds.remove('device-info')
             mxs40v2_cmds.remove('read-die-id')
             mxs40v2_cmds.remove('load-and-run-app')
@@ -140,18 +153,21 @@
                 platform = None
         return platform
 
     @staticmethod
     def _command_list(obj):
         if isinstance(obj, click.Group):
             return [name for name, value in obj.commands.items()]
+        return None
 
     @staticmethod
     def _print_help_instructions():
         app_name = os.path.basename(sys.argv[0])
+        print()
         print('Command line interfaces are different for different targets.\n')
         print('To see a list of commands supported for a specific target:')
         print(f'{app_name} -t <TARGET> --help\n')
         print('To see a list of options for a specific command:')
         print(f'{app_name} -t <TARGET> <COMMAND> --help\n')
         print('To see a list of available targets:')
         print(f'{app_name} device-list\n')
+        print('For detailed usage description refer to readme.md')
```

### Comparing `cysecuretools-4.2.0/cysecuretools/cli_mxs40sv2.py` & `cysecuretools-5.0.0/src/cli_mxs40sv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -15,18 +16,19 @@
 """
 import os
 import sys
 import json
 import logging
 import binascii
 import click
-from cysecuretools.core.connect_helper import ConnectHelper
-from cysecuretools.core.enums import KeyAlgorithm
-from cysecuretools.cli import main, process_handler
-from cysecuretools.execute.imgtool.main import get_dependencies
+
+from .core.connect_helper import ConnectHelper
+from .core.enums import KeyAlgorithm
+from .cli import main, process_handler
+from .execute.imgtool.main import get_dependencies
 
 logger = logging.getLogger(__name__)
 
 
 @main.command('create-key', help='Creates private and public key pair')
 @click.option('-k', '--key-id', type=click.Choice(['0', '1']),
               help='OEM key ID')
@@ -173,15 +175,15 @@
         def print_error():
             if error:
                 sys.stderr.write(f'Error: {error}\n')
                 sys.exit(2)
 
         error = None
         from .targets.common.mxs40sv2.enums import PolicyType
-        policy_type = ctx.obj['TOOL'].policy_parser.get_policy_type()
+        policy_type = ctx.obj['TOOL'].policy_parser.policy_type()
 
         if PolicyType.REPROVISIONING_SECURE == policy_type:
             if all(v is None for v in [key_id, key_path, signature,
                                        non_signed]):
                 error = "One of the following options must be " \
                         "specified: '--key-id', '--key-path', " \
                         "'--signature', '--non-signed'."
@@ -245,15 +247,15 @@
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         validate_testapps_args(testapps, testapps_si)
         if existing_packet:
             result = True
         else:
-            policy_type = ctx.obj['TOOL'].policy_parser.get_policy_type()
+            policy_type = ctx.obj['TOOL'].policy_parser.policy_type()
             if 'reprovisioning' in policy_type:
                 logger.error('Reprovisioning policy type specified for '
                              'the provisioning operation')
                 return False
             result = ctx.obj['TOOL'].create_provisioning_packet(
                 testapps=test_pkg_type(testapps, testapps_si))
         if result:
@@ -300,15 +302,15 @@
             result = ctx.obj['TOOL'].re_provision_device(
                 probe_id, testapps=test_pkg_type(testapps, testapps_si))
         return result
 
     def validate_args():
         error = None
         from .targets.common.mxs40sv2.enums import PolicyType
-        policy_type = ctx.obj['TOOL'].policy_parser.get_policy_type()
+        policy_type = ctx.obj['TOOL'].policy_parser.policy_type()
 
         if existing_packet:
             if any(v for v in [key_id, key_path, signature]):
                 error = "The options '--key-id', '--key-path', " \
                         "'--signature' are not applicable when " \
                         "the existing packet is used."
         elif PolicyType.REPROVISIONING_SECURE == policy_type:
@@ -324,15 +326,15 @@
             sys.stderr.write(f'Error: {error}\n')
             sys.exit(2)
 
         validate_testapps_args(testapps, testapps_si)
 
     def validate_policy_type():
         from .targets.common.mxs40sv2.enums import PolicyType
-        policy_type = ctx.obj['TOOL'].policy_parser.get_policy_type()
+        policy_type = ctx.obj['TOOL'].policy_parser.policy_type()
         if policy_type not in [PolicyType.REPROVISIONING_SECURE,
                                PolicyType.REPROVISIONING_NO_SECURE]:
             sys.stderr.write('Error: Provisioning policy type specified for '
                              'the reprovisioning operation\n')
             sys.exit(2)
 
     return process
@@ -486,15 +488,15 @@
             sys.exit(2)
         elif key_id and key_path:
             sys.stderr.write("The '--key-id' and '--key-path' options are "
                              "mutually exclusive.\n")
             sys.exit(2)
 
         from .targets.common.mxs40sv2.enums import PolicyType
-        policy_type = ctx.obj['TOOL'].policy_parser.get_policy_type()
+        policy_type = ctx.obj['TOOL'].policy_parser.policy_type()
         if policy_type == PolicyType.REPROVISIONING_SECURE:
             validate_update_key(update_key_id, update_key_path)
 
     return process
 
 
 @main.command('extend-image', help='Extends firmware image with the TLVs',
@@ -568,15 +570,15 @@
     def validate_args():
         if image_format == 'bootrom_next_app' and not pubkey:
             sys.stderr.write("Error: Missing option '--pubkey'.\n")
             sys.exit(2)
 
         from .targets.common.mxs40sv2.enums import PolicyType
         if ctx.obj['TOOL'].policy_parser.json:
-            policy_type = ctx.obj['TOOL'].policy_parser.get_policy_type()
+            policy_type = ctx.obj['TOOL'].policy_parser.policy_type()
             if policy_type == PolicyType.REPROVISIONING_SECURE:
                 validate_update_key(update_key_id, update_key_path)
 
     return process
 
 
 @main.command('init', help='Initializes new project')
@@ -698,15 +700,15 @@
                     json.dump(data, f, indent=4)
             return True
         return False
 
     return process
 
 
-@main.command('convert-to-rma', help='Converts device to RMA lifecycle stage')
+@main.command('convert-to-rma', help='Transition device to RMA lifecycle stage')
 @click.option('-c', '--cert', type=click.Path(),
               help='Path to debug certificate')
 @click.option('--probe-id', default=None, help='Probe serial number')
 @click.option('--testapps', is_flag=True, hidden=True)
 @click.option('--testapps-si', is_flag=True, hidden=True)
 @click.pass_context
 def cmd_convert_to_rma(ctx, cert, probe_id, testapps, testapps_si):
```

### Comparing `cysecuretools-4.2.0/cysecuretools/cli_mxs40v1.py` & `cysecuretools-5.0.0/src/cli_mxs40v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020-2022 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,22 +12,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import sys
 import json
-import click
 import logging
-from intelhex import HexRecordError
 from json.decoder import JSONDecodeError
+
+import click
+from intelhex import HexRecordError
 from cryptography.hazmat.primitives import serialization
-from cysecuretools.execute.image_cert import ImageCertificate
-from cysecuretools.core.enums import KeyAlgorithm
-from cysecuretools.cli import main as main, process_handler
+
+from .targets.common.mxs40v1.image_cert import ImageCertificate
+from .core.enums import KeyAlgorithm
+from .cli import main as main, process_handler
 
 logger = logging.getLogger(__name__)
 name = 'cli_mxs40v1'
 
 
 @main.command('create-keys', help='Creates keys specified in policy file')
 @click.option('--overwrite/--no-overwrite', 'overwrite', is_flag=True,
@@ -35,17 +38,16 @@
                    'if they already exist')
 @click.option('-o', '--out', type=click.Path(), default=None, required=False,
               help='Output directory for generated keys. By default keys '
                    'location is as specified in the policy file')
 @click.option('--kid', type=click.INT, default=None, required=False,
               help='The ID of the key to create. If not specified, all the '
                    'keys found in the policy will be generated')
-@click.option('-a', '--algorithm', default=None,
-              type=click.Choice(
-                  [KeyAlgorithm.EC, KeyAlgorithm.RSA], case_sensitive=False),
+@click.option('-a', '--algorithm', default=None, hidden=True,
+              type=click.Choice([KeyAlgorithm.EC], case_sensitive=False),
               help='Key algorithm')
 @click.option('--template', type=click.Path(),
               help='A JSON file containing public numbers')
 @click.pass_context
 def cmd_create_keys(ctx, overwrite, out, kid, algorithm, template):
     @process_handler()
     def process():
@@ -431,34 +433,32 @@
               short_help='Creates encrypted image for encrypted programming')
 @click.option('-i', '--image', type=click.File('r'), required=True,
               help='The image to encrypt')
 @click.option('-h', '--host-key-id', type=click.INT, required=True,
               help='Host private key ID (4 - HSM, 5 - OEM)')
 @click.option('-d', '--device-key-id', type=click.INT, required=True,
               help='Device public key ID (1 - device, 12 - group)')
-@click.option('-a', '--algorithm', 'algorithm', default='ECC',
-              help='Asymmetric algorithm for key derivation function')
 @click.option('--key-length', type=click.INT, default=16,
               help='Derived key length')
 @click.option('-o', '--encrypted-image', required=True, type=click.File('w+'),
               help='Output file of encrypted image for encrypted programming')
 @click.option('--padding-value', default=0, type=click.INT,
               help='Value for image padding')
 @click.option('--probe-id', default=None,
               help='Probe serial number. '
                    'Used to read device public key from device.')
 @click.pass_context
-def cmd_encrypt_image(ctx, image, host_key_id, device_key_id, algorithm,
+def cmd_encrypt_image(ctx, image, host_key_id, device_key_id,
                       key_length, encrypted_image, padding_value, probe_id):
     @process_handler()
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         return ctx.obj['TOOL'].encrypt_image(
-            image.name, host_key_id, device_key_id, algorithm, key_length,
+            image.name, host_key_id, device_key_id, key_length,
             encrypted_image.name, padding_value, probe_id)
 
     return process
 
 
 @main.command('encrypted-programming', help='Programs encrypted image')
 # w+ is for -i option necessary if encryption and programming are run together
@@ -490,16 +490,15 @@
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         address, _ = ctx.obj['TOOL'].flash_map(image_id, image_type)
         if address:
             print(hex(address) if display_hex else address)
             return True
-        else:
-            return False
+        return False
 
     return process
 
 
 @main.command('slot-size', short_help='Gets slot size from given policy')
 @click.option('-i', '--image-id', type=click.INT, required=True,
               help='Image ID')
@@ -513,16 +512,15 @@
     def process():
         if 'TOOL' not in ctx.obj:
             return False
         _, size = ctx.obj['TOOL'].flash_map(image_id, image_type)
         if size:
             print(hex(size) if display_hex else size)
             return True
-        else:
-            return False
+        return False
 
     return process
 
 
 @main.command('read-public-key', help='Reads public key from device')
 @click.option('-k', '--key-id', type=click.INT, required=True,
               help='Key ID to read (1 - DEVICE, 4 - HSM, 5 - OEM, 12 - GROUP')
@@ -544,16 +542,15 @@
             if type(key) is dict:
                 logger.info(json.dumps(key, indent=4))
             elif type(key) is bytes:
                 logger.info(key.decode("utf-8"))
             else:
                 logger.info(key)
             return True
-        else:
-            return False
+        return False
 
     return process
 
 
 @main.command('read-die-id', help='Reads die ID from device')
 @click.option('-o', '--out-file', default=None,
               help='Filename where to save die ID')
@@ -568,16 +565,15 @@
         data = ctx.obj['TOOL'].read_die_id(probe_id)
         if data:
             logger.info('die_id = %s', json.dumps(data, indent=4))
             if out_file:
                 with open(out_file, 'w', encoding='utf-8') as f:
                     json.dump(data, f, indent=4)
             return True
-        else:
-            return False
+        return False
 
     return process
 
 
 @main.command('sign-cert', help='Signs JSON certificate with the private key')
 @click.option('-j', '--json-file', '--template', 'template', type=click.Path(),
               required=True, help='Certificate template')
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/bitops.py` & `cysecuretools-5.0.0/src/core/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright (c) 2020 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,12 +11,11 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
-def get_bits(value, start, end):
-    """ Gets the specified number of bits from the value """
-    count = end - start + 1
-    mask = ((1 << count) - 1) << start
-    return (value & mask) >> start
+class ValidationError(Exception):
+    def __init__(self, message=None, errors=None):
+        super().__init__(message)
+        self.errors = errors
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/certificates/x509.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/x509_mxs40v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,33 +14,34 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import json
 import logging
 import datetime
+
 from cryptography import x509
 from cryptography.x509.oid import NameOID
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
-from cysecuretools.execute.key_reader import load_key
-from cysecuretools.core.strategy_context.cert_strategy_ctx \
-    import CertificateStrategy
-from cysecuretools.core.target_director import Target
-from cysecuretools.execute.provisioning_packet.lib.cyprov_pem import PemKey
-from cysecuretools.targets.common.p64.silicon_data_parser import SiliconDataParser
-from cysecuretools.targets.common.p64.enums import KeyId
-from cysecuretools.execute.provisioning.provision_device_mxs40v1 import read_silicon_data
-from ..connect_helper import ConnectHelper
+
+from .enums import KeyId
+from .silicon_data_parser import SiliconDataParser
+from ....core.key_handlers.pem_key import PemKey
+from ....core.connect_helper import ConnectHelper
+from ....core.strategy_context.cert_strategy_ctx import CertificateStrategy
+from ....execute.key_reader import load_key
+from .provisioning.provision_device_mxs40v1 import read_silicon_data
 
 logger = logging.getLogger(__name__)
 
 
-class X509CertificateStrategy(CertificateStrategy):
+class X509CertificateStrategyMXS40v1(CertificateStrategy):
+
     def create_certificate(self, filename, encoding, overwrite=None, **kwargs):
         """
         Creates certificate in X.509 format.
         """
         filename = os.path.abspath(filename)
 
         if 'subject_name' in kwargs:
@@ -155,21 +157,15 @@
                 self._save_to_file(certificate, encoding, filename)
         elif overwrite:
             self._save_to_file(certificate, encoding, filename)
         else:
             logger.info('Skip saving certificate to file')
         return certificate
 
-    @staticmethod
-    def _save_to_file(certificate, encoding, filename):
-        with open(filename, 'wb') as f:
-            f.write(certificate.public_bytes(encoding))
-        logger.info('Certificate created: %s', filename)
-
-    def default_certificate_data(self, tool, target: Target, probe_id=None):
+    def default_certificate_data(self, tool, target, probe_id=None):
         """
         Gets a dictionary with the default values.
         Default certificate requires device to be connected to read
         device public key and die ID, which are used as a certificate
         fields
         :param tool: Programming tool to connect to device
         :param target: Target object
@@ -218,14 +214,20 @@
             'public_key': dev_pub_key,
             'private_key': hsm_priv_key,
             'serial_number': serial,
         }
         logger.debug(json.dumps(data))
         return data
 
+    def verify_certificate(self, cert_path, root_cert_path, key_path):
+        raise NotImplementedError('N/A for mxs40v1 platform')
+
+    def create_csr(self, output, key_path, **kwargs):
+        raise NotImplementedError
+
     @staticmethod
     def load_pem(key_path):
         """
         Reads PEM file.
         :param key_path: Path to certificate.
         :return: File content as a string.
         """
@@ -249,7 +251,13 @@
         """
         pem = PemKey()
         if type(jwk) is dict:
             jwk = json.dumps(jwk)
         pem.load_str(jwk)
         pem_str = pem.to_str(private_key=private_key)
         return pem_str
+
+    @staticmethod
+    def _save_to_file(certificate, encoding, filename):
+        with open(filename, 'wb') as f:
+            f.write(certificate.public_bytes(encoding))
+        logger.info('Certificate created: %s', filename)
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/connect_helper.py` & `cysecuretools-5.0.0/src/core/connect_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     """ Helper class for connection creation process """
 
     connected = False
     do_not_disconnect = False
 
     @staticmethod
     def connect(tool: ProgrammerBase, target: Target,
-                probe_id=None, ap='sysap', acquire=True, blocking=True,
-                ignore_errors=False, power=None, voltage=None) -> bool:
+                probe_id=None, ap='sysap', acquire=True, ignore_errors=False,
+                power=None, voltage=None) -> bool:
         """ Checks for target/OCD compatibility and creates a connection """
 
         if tool.name not in target.ocds:
             logger.error("Target '%s' is not supported by the selected "
                          "on-chip debugger '%s'", target.name, tool.name)
             ConnectHelper._print_ocd_info(tool, target)
             ConnectHelper._print_example()
@@ -58,16 +58,15 @@
                 raise ValueError('Invalid on-chip debugger path')
 
         if not ConnectHelper.connected:
             if tool.require_path and tool.tool_path:
                 logger.info("On-Chip debugger path is '%s'", tool.tool_path)
             ConnectHelper.connected = tool.connect(
                 target.name, probe_id=probe_id, ap=ap, acquire=acquire,
-                blocking=blocking, power=power, voltage=voltage,
-                ignore_errors=ignore_errors)
+                power=power, voltage=voltage, ignore_errors=ignore_errors)
 
         if not ConnectHelper.connected:
             if tool.name == 'openocd' and not ignore_errors:
                 logger.error('OpenOCD server has not started')
         return ConnectHelper.connected
 
     @staticmethod
@@ -78,15 +77,15 @@
         logger.warning('ATTENTION! To avoid device destruction, make sure the '
                        'external power is not connected. Continue? (y/n): ')
         confirm = input()
         if confirm.lower() == 'y':
             if voltage is None:
                 voltage = 2500
                 logger.warning('Voltage is not specified. Default voltage '
-                               f'level will be used ({voltage} mV).')
+                               'level will be used (%d mV).', voltage)
             if ConnectHelper.connect(tool, target, power='on', voltage=voltage):
                 logger.info('Power on command sent')
                 return True
         else:
             return True
         return False
 
@@ -118,12 +117,11 @@
         print(f'The currently selected on-chip debugger: {tool.name}.')
         print(f"The supported on-chip debugger(s) for the '{target.name}' "
               f'target: {",".join(target.ocds)}.')
 
     @staticmethod
     def _print_example():
         app_name = os.path.basename(sys.argv[0])
-        print("Use the 'set-ocd' command to set the active debugger.")
-        print('Examples:')
-        print(f'{app_name} set-ocd --name pyocd')
+        print("Use the 'set-ocd' command to configure the On-Chip debugger.")
+        print('Example:')
         print(f'{app_name} set-ocd --name openocd --path /Users/username/'
               f'tools/openocd')
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/cy_bootloader_map_parser.py` & `cysecuretools-5.0.0/src/core/cy_bootloader_map_parser.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/dependecy_validator.py` & `cysecuretools-5.0.0/src/core/dependecy_validator.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/deprecated.py` & `cysecuretools-5.0.0/src/core/deprecated.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/entrance_exam_base.py` & `cysecuretools-5.0.0/src/core/entrance_exam_base.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/enums.py` & `cysecuretools-5.0.0/src/core/enums.py`

 * *Files 19% similar despite different names*

```diff
@@ -50,17 +50,24 @@
     user, encryption, device_public, group_public = range(4)
 
 
 class KeyAlgorithm:
     """
     Supported key algorithms.
     """
-    EC = 'EC'
-    RSA = 'RSA'
-    AES = 'AES'
+    ECDSA_P256 = 'ECDSA-P256'
+    ECDSA_P384 = 'ECDSA-P384'
+    RSA2048 = 'RSA2048'
+    RSA3072 = 'RSA3072'
+    RSA4096 = 'RSA4096'
+    AES128 = 'AES128'
+    AES256 = 'AES256'
+    EC = ECDSA_P256
+    RSA = RSA2048
+    AES = AES128
 
 
 class ImageType(Enum):
     """
     Available image types.
     """
     BOOT = 'BOOT'
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/exceptions.py` & `cysecuretools-5.0.0/src/core/strops.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright (c) 2021 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,11 +11,10 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
-class ValidationError(Exception):
-    def __init__(self, message=None, errors=None):
-        super().__init__(message)
-        self.errors = errors
+def split_by_n(seq, n):
+    """ Splits string every N-th character """
+    return [seq[i:i + n] for i in range(0, len(seq), n)]
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/json_helper.py` & `cysecuretools-5.0.0/src/core/json_helper.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/jsonpath.py` & `cysecuretools-5.0.0/src/core/jsonpath.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/key_data.py` & `cysecuretools-5.0.0/src/core/key_data.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/key_handlers/rsa_handler.py` & `cysecuretools-5.0.0/src/core/key_handlers/ec_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,107 +1,131 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright (c) 2022 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-import os
-import base64
 import hashlib
-from pathlib import Path
-from collections import namedtuple
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import serialization
-from cryptography.hazmat.primitives.serialization import (
-    load_der_public_key, load_der_private_key)
-from cryptography.hazmat.primitives.hashes import SHA256
-from cryptography.hazmat.primitives.asymmetric import padding
-from cryptography.hazmat.primitives.asymmetric import utils
-from cryptography.hazmat.primitives.asymmetric import rsa
 
+from jose.utils import long_to_base64
+from cryptography.hazmat.primitives.asymmetric.utils import decode_dss_signature
+from cryptography.hazmat.primitives.asymmetric import ec
+from cryptography.hazmat.primitives import serialization, hashes
 
-class RSAHandler:
+from .pem_key import PemKey
+from . import load_private_key, load_public_key
 
-    @staticmethod
-    def read_key(key_path):
-        """ Reads key data without header and footer """
-        with open(key_path, 'r', encoding='utf-8') as f:
-            content = f.read()
-            b64data = '\n'.join(content.splitlines()[1:-1])
-        return b64data
 
-    @staticmethod
-    def decode(key_path):
-        """ Decodes Base64 key into binary """
-        b64data = RSAHandler.read_key(key_path)
-        decoded = base64.b64decode(b64data)
-        return decoded
+class ECHandler:
+    """Handles EC signature and parse key data operations"""
 
     @staticmethod
-    def is_private_key(key_path):
-        """ Gets a value indicating whether the key is a private key """
-        data = RSAHandler.decode(key_path)
-        try:
-            load_der_private_key(data, None, default_backend())
-            is_private = True
-        except ValueError:
-            load_der_public_key(data, default_backend())
-            is_private = False
-
-        return is_private
-
-    @staticmethod
-    def public_numbers(key_path):
-        """ Gets modulus, exponent, length of the RSA key """
-        data = RSAHandler.decode(key_path)
-        try:
-            key = load_der_private_key(data, None, default_backend())
-            pn = key.private_numbers().public_numbers
-        except ValueError:
-            key = load_der_public_key(data, default_backend())
-            pn = key.public_numbers()
-
-        PublicNumbers = namedtuple('PublicNumbers', 'modulus exponent length')
-
-        return PublicNumbers(pn.n, pn.e, key.key_size)
-
-    @staticmethod
-    def sign(key_path, message):
-        """ Signs a message using a key loaded from key_path """
-        data = RSAHandler.decode(key_path)
-        privkey = load_der_private_key(data, None, default_backend())
-        digest = hashlib.sha256(message).digest()
-        sig = privkey.sign(
-                digest,
-                padding.PSS(
-                    mgf=padding.MGF1(SHA256()),
-                    salt_length=padding.PSS.MAX_LENGTH),
-                utils.Prehashed(SHA256()))
-        return sig
-
-    @staticmethod
-    def populate_public_key(exponent, modulus):
-        """ Generates an RSA public key from the modulus and exponent """
-        exponent = int(exponent, 16)
-        modulus = int(modulus, 16)
-        pubkey = rsa.RSAPublicNumbers(exponent, modulus).public_key(
-            default_backend())
+    def populate_public_key(pub):
+        """ Generates an EC public key from the public numbers """
+        pubkey = ec.EllipticCurvePublicKey.from_encoded_point(
+            ec.SECP256R1(), pub)
         return pubkey
 
     @staticmethod
-    def save_public_key(pubkey, filename):
-        """ Saves RSA public key to a PEM file """
-        pem = pubkey.public_bytes(
-            encoding=serialization.Encoding.PEM,
-            format=serialization.PublicFormat.SubjectPublicKeyInfo)
-        Path(os.path.dirname(filename)).mkdir(parents=True, exist_ok=True)
-        with open(filename, 'wb') as f:
-            f.write(pem)
+    def public_jwk(pubkey, kid=None):
+        """ Gets EC public key is JSON format """
+        alg, crv = ECHandler._jwk_alg(pubkey)
+        key_json = {
+            'alg': alg,
+            'kty': 'EC',
+            'crv': crv,
+            'use': 'sig',
+            'x': long_to_base64(pubkey.public_numbers().x).decode('utf-8'),
+            'y': long_to_base64(pubkey.public_numbers().y).decode('utf-8')
+        }
+        if kid:
+            key_json['kid'] = str(kid)
+        return key_json
+
+    @staticmethod
+    def private_jwk(privkey, kid=None):
+        """ Gets EC private key is JSON format """
+        alg, crv = ECHandler._jwk_alg(privkey)
+        pubkey = privkey.public_key()
+        key_json = {
+            'alg': alg,
+            'kty': 'EC',
+            'crv': crv,
+            'use': 'sig',
+            'x': long_to_base64(pubkey.public_numbers().x).decode('utf-8'),
+            'y': long_to_base64(pubkey.public_numbers().y).decode('utf-8'),
+            'd': long_to_base64(
+                privkey.private_numbers().private_value).decode('utf-8'),
+        }
+        if kid:
+            key_json['kid'] = str(kid)
+        return key_json
+
+    @staticmethod
+    def _jwk_alg(privkey):
+        if isinstance(privkey.curve, ec.SECP256R1):
+            alg = 'ES256'
+            crv = 'P-256'
+        elif isinstance(privkey.curve, ec.SECP384R1):
+            alg = 'ES384'
+            crv = 'P-384'
+        return alg, crv
+
+    @staticmethod
+    def key_hash(pubkey):
+        """Encoding public key and return as byte sequence"""
+        pub = pubkey.public_bytes(
+            serialization.Encoding.DER,
+            serialization.PublicFormat.SubjectPublicKeyInfo)
+        sha = hashlib.sha256()
+        sha.update(pub)
+        key_hash = sha.digest()
+        return key_hash
+
+    @staticmethod
+    def is_private_key(key):
+        """ Gets a value indicating whether the key is a private key """
+        if isinstance(key, str):
+            try:
+                p_key = load_private_key(key)
+            except ValueError:
+                p_key = load_public_key(key)
+        else:
+            p_key = key
+
+        if not isinstance(p_key, (ec.EllipticCurvePrivateKey,
+                                  ec.EllipticCurvePublicKey)):
+            raise ValueError("Using EC with unsupported key")
+
+        return isinstance(p_key, ec.EllipticCurvePrivateKey)
+
+    @staticmethod
+    def sign(key_path, token):
+        """ Signs a token using a key loaded from key_path """
+        private_key = load_private_key(key_path)
+        sig = private_key.sign(
+            token,
+            ec.ECDSA(hashes.SHA256())
+        )
+        return ECHandler.asn1_to_rs(sig)
+
+    @staticmethod
+    def jwk_to_pem(jwk_file, private_key=True):
+        """Converts JWK file content to PEM format string"""
+        pem = PemKey(jwk_file)
+        pem_str = pem.to_str(private_key=private_key)
+        return pem_str
+
+    @staticmethod
+    def asn1_to_rs(signature):
+        """Converts ECDSA signature in ASN.1 format to R and S values"""
+        r, s = decode_dss_signature(signature)
+        return r.to_bytes(32, byteorder='big'), s.to_bytes(32, byteorder='big')
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/key_helper.py` & `cysecuretools-5.0.0/src/core/key_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,32 +12,40 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import hashlib
 import logging
-from cysecuretools.execute.image_signing.rsa_converter import RSAConverter
-from cysecuretools.core.key_handlers import RSAHandler
+
+from .key_handlers.rsa_handler import RSAHandler
+from .key_handlers.pem_key import PemKey
 
 logger = logging.getLogger(__name__)
 
 TRUNCATED_SHA256_SIZE = 16
 PUB_KEY_SIZE = 516
 AES_KEY_SIZE = 16
 
 
+def jwk_to_pem(jwk_file, private_key=True):
+    """Converts JWK file content to PEM format string"""
+    pem = PemKey(jwk_file)
+    pem_str = pem.to_str(private_key=private_key)
+    return pem_str
+
+
 def get_key_bytearray(key_path):
     """Gets key bytes"""
     if key_path and os.path.isfile(key_path):
         if verify_key_format(key_path, 'binary'):
             with open(key_path, 'rb') as key:
                 key_bytes = key.read()
         elif verify_key_format(key_path, 'rsa'):
-            key_str = RSAConverter.convert_to_mbedtls(key_path)
+            key_str = RSAHandler.convert_to_mbedtls(key_path)
             key_bytes = bytearray.fromhex(key_str)
         else:
             raise ValueError(f'Invalid key format ({key_path})')
         return key_bytes
 
     zero_bytes = bytes(b'\x00' * PUB_KEY_SIZE)
     return zero_bytes
@@ -61,11 +69,10 @@
     """Verifies whether key format matches the specified"""
     if key_type == 'rsa':
         try:
             RSAHandler.public_numbers(key_path)
         except ValueError:
             return False
         return True
-    elif key_type == 'binary':
+    if key_type == 'binary':
         return os.path.getsize(key_path) == AES_KEY_SIZE
-    else:
-        raise ValueError(f'Invalid key type ({key_type})')
+    raise ValueError(f'Invalid key type ({key_type})')
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/logging_configurator.py` & `cysecuretools-5.0.0/src/core/logging_configurator.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import logging
 from datetime import datetime
-from cysecuretools.core.project import ProjectInitializer
-from cysecuretools.core.logging_formatter import CustomFormatter
+
+from .project_base import ProjectInitializerBase
+from .logging_formatter import CustomFormatter
 
 logger = logging.getLogger(__name__)
 
 
 class LoggingConfigurator:
     """
     The class that allows configuring the way how the data is logged
@@ -51,24 +52,25 @@
                 handler.setLevel(level)
 
     @staticmethod
     def add_file_logging():
         """
         Adds file logger
         """
+        prefix = LoggingConfigurator.LOG_FORMATTER.package_name
         log_filename = datetime.now().strftime(os.path.join(
             LoggingConfigurator.get_log_dir(),
-            'cysecuretools_%Y-%m-%d_%H-%M-%S.log'))
+            f'{prefix}_%Y-%m-%d_%H-%M-%S.log'))
         os.makedirs(os.path.dirname(log_filename), exist_ok=True)
         file_handler = logging.FileHandler(log_filename, mode='w+')
         file_handler.setLevel(logging.DEBUG)
         file_handler.setFormatter(LoggingConfigurator.LOG_FORMATTER)
         logger.root.addHandler(file_handler)
 
     @staticmethod
     def get_log_dir():
-        if ProjectInitializer.is_project():
+        if ProjectInitializerBase.is_project():
             cwd = os.path.join(os.getcwd(), 'logs')
         else:
             cwd = os.path.abspath(
                 os.path.join(os.path.dirname(__file__), '..', 'logs'))
         return cwd
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/logging_formatter.py` & `cysecuretools-5.0.0/src/core/logging_formatter.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,45 +11,46 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import logging
 
+from ..__about__ import __pkg_name__, __pkg_short_name__
+
 
 class CustomFormatter(logging.Formatter):
     error_fmt = '%(asctime)s : ##_package_## : ERROR : %(message)s'
     debug_fmt = '%(asctime)s : ##_package_## : DEBUG : %(name)s, line %(lineno)d: %(message)s'
     warning_fmt = '%(asctime)s : ##_package_## : WARN  : %(message)s'
     info_fmt = '%(asctime)s : ##_package_## : INFO  : %(message)s'
 
     def __init__(self):
         super().__init__(fmt="%(levelno)d: %(msg)s", datefmt=None, style='%')
         self.style = self._style = CustomPercentStyle()
         self.original_format = self.style.fmt
+        self.package_name = __pkg_name__.lower()
 
     def format(self, record):
         if record.levelno == logging.DEBUG:
             self.style.fmt = CustomFormatter.debug_fmt
 
         elif record.levelno == logging.INFO:
             self.style.fmt = CustomFormatter.info_fmt
 
         elif record.levelno == logging.WARNING:
             self.style.fmt = CustomFormatter.warning_fmt
 
         elif record.levelno == logging.ERROR:
             self.style.fmt = CustomFormatter.error_fmt
 
-        if record.name.startswith('pyocd'):
-            package = 'P'
-        elif 'openocd' in record.name:
+        if 'openocd' in record.name:
             package = 'O'
-        elif record.name.startswith('cysecuretools'):
-            package = 'C'
+        elif record.name.startswith(self.package_name):
+            package = __pkg_short_name__
             if record.levelno == logging.ERROR:
                 self.style.fmt += '. Check the log for details'
         else:
             package = ' '
 
         self.style.fmt = self.style.fmt.replace('##_package_##', package)
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/memory_area.py` & `cysecuretools-5.0.0/src/core/memory_area.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/memory_map_base.py` & `cysecuretools-5.0.0/src/core/memory_map_base.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/mtb_tools_discovery.py` & `cysecuretools-5.0.0/src/core/mtb_tools_discovery.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/policy_filter_base.py` & `cysecuretools-5.0.0/src/core/policy_filter_base.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/policy_validator_base.py` & `cysecuretools-5.0.0/src/core/policy_validator_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from abc import ABC, abstractmethod
 
+from .enums import ValidationStatus
+
 
 class PolicyValidatorBase(ABC):
     """
     Base class for the classes that implement policy validator.
     Each device-specific policy validator must implement its methods.
     """
 
     skip_validation = False
 
     @abstractmethod
-    def validate(self, skip=None, skip_prompts=False):
+    def validate(
+            self, skip=None, skip_prompts=False, **kwargs) -> ValidationStatus:
         """ Validates policy file """
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/progress_bar.py` & `cysecuretools-5.0.0/src/execute/imgtool/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-"""
-Copyright (c) 2020-2021 Cypress Semiconductor Corporation
+# Copyright 2017-2020 Linaro Limited
+#
+# SPDX-License-Identifier: Apache-2.0
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-import logging
-
-logger = logging.getLogger(__name__)
-
-
-def update_progress(progress):
-    logging.info('\r[ %s%s ] %d%%', '#' * progress, ' ' * int(100 - progress),
-                 progress)
+imgtool_version = "1.7.0"
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/application.py` & `cysecuretools-5.0.0/src/pkg_globals.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright (c) 2019-2021 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from abc import ABC, abstractmethod
+import os
 
-
-class Application(ABC):
-
-    @abstractmethod
-    def __init__(self, app_name):
-        pass
+TOOLS_PATH = os.path.abspath(os.path.dirname(os.path.realpath(__file__)))
+SETTINGS_FILE = os.path.join(TOOLS_PATH, 'settings.json')
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/provisioning_flows/flow.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright (c) 2020-2021 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from abc import ABC, abstractmethod
+from enum import IntEnum
 
 
-class Flow(ABC):
-    """
-    Abstract class necessary for implementation by targets, which
-    use RAM application provisioning approach
-    """
-
-    @abstractmethod
-    def run(self, tool, **kwargs):
-        """ Implements device provisioning with RAM applications """
+class ProtectionState(IntEnum):
+    """ Device protection states """
+    unknown = 0
+    virgin = 1
+    normal = 2
+    secure = 3
+    dead = 4
+
+
+class KeyId(IntEnum):
+    HSM = 4
+    OEM = 5
+    DEVICE = 1
+    GROUP = 12
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/register_map_base.py` & `cysecuretools-5.0.0/src/core/register_map_base.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/core/signtool_base.py` & `cysecuretools-5.0.0/src/core/policy_parser_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2022 Cypress Semiconductor Corporation
+Copyright 2022 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,28 +12,14 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from abc import ABC, abstractmethod
 
-from intelhex import hex2bin, bin2hex
 
-
-class SignTool(ABC):
-    """Base class for the classes that implement
-    image signing behaviour
-    """
+class PolicyParserBase(ABC):
+    """Base class for the classes that implement policy parser"""
 
     @abstractmethod
-    def sign_image(self, image_path, **kwargs):
-        """Signs firmware image"""
-
-    @staticmethod
-    def bin2hex(fin, fout, offset=0):
-        """Converts bin to hex"""
-        return bin2hex(fin, fout, offset) == 0
-
-    @staticmethod
-    def hex2bin(fin, fout, start=None, end=None, size=None, pad=None):
-        """Converts hex to bin"""
-        return hex2bin(fin, fout, start=start, end=end, size=size, pad=pad) == 0
+    def policy_type(self):
+        """Gets a value of policy type property"""
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/strategy_context/cert_strategy_ctx.py` & `cysecuretools-5.0.0/src/core/strategy_context/provisioning_strategy_ctx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright (c) 2020-2023 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,54 +12,86 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from abc import ABC, abstractmethod
 
 
-class CertificateStrategy(ABC):
+class ProvisioningStrategy(ABC):
     """
-    The Strategy interface declares operations common to all supported versions
-    of some algorithm.
+    The Strategy interface declares operations common to all supported
+    versions of some algorithm.
     """
     @abstractmethod
-    def create_certificate(self, filename, encoding, overwrite, **kwargs):
+    def provision(self, tool, target, bootloader, **kwargs):
         pass
 
     @abstractmethod
-    def default_certificate_data(self, tool, target, probe_id):
+    def re_provision(self, tool, target, bootloader, **kwargs):
         pass
 
+    @abstractmethod
+    def erase_flash(self, tool, target):
+        pass
+
+    @abstractmethod
+    def transit_to_rma(self, tool, target, cert, **kwargs):
+        pass
 
-class CertificateContext:
+    @abstractmethod
+    def open_rma(self, tool, target, cert):
+        pass
+
+
+class ProvisioningContext:
     """
     The Context defines the interface of interest to clients.
     """
-    def __init__(self, strategy: CertificateStrategy):
+    def __init__(self, strategy: ProvisioningStrategy):
         self._strategy = strategy
 
     @property
-    def strategy(self) -> CertificateStrategy:
+    def strategy(self) -> ProvisioningStrategy:
         """
-        The Context maintains a reference to one of the Strategy objects.
+        The Context maintains a reference to one of the Strategy
+        objects.
         """
         return self._strategy
 
     @strategy.setter
-    def strategy(self, strategy: CertificateStrategy):
+    def strategy(self, strategy: ProvisioningStrategy):
         """
         Allows replacing a Strategy object at runtime.
         """
         self._strategy = strategy
 
-    def create_certificate(self, filename, encoding, overwrite, **kwargs):
+    def provision(self, tool, target, bootloader=None, **kwargs):
+        """
+        Delegates work to the Strategy object.
+        """
+        return self._strategy.provision(tool, target, bootloader=bootloader,
+                                        **kwargs)
+
+    def re_provision(self, tool, target, bootloader=None, **kwargs):
+        """
+        Delegates work to the Strategy object.
+        """
+        return self._strategy.re_provision(tool, target, bootloader=bootloader,
+                                           **kwargs)
+
+    def erase_flash(self, tool, target):
+        """
+        Delegates work to the Strategy object.
+        """
+        self._strategy.erase_flash(tool, target)
+
+    def transit_to_rma(self, tool, target, cert, **kwargs):
         """
         Delegates work to the Strategy object.
         """
-        return self._strategy.create_certificate(filename, encoding, overwrite,
-                                                 **kwargs)
+        return self._strategy.transit_to_rma(tool, target, cert, **kwargs)
 
-    def default_certificate_data(self, tool, target, probe_id):
+    def open_rma(self, tool, target, cert):
         """
         Delegates work to the Strategy object.
         """
-        return self._strategy.default_certificate_data(tool, target, probe_id)
+        return self._strategy.open_rma(tool, target, cert)
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/strategy_context/encrypted_programming_strategy_ctx.py` & `cysecuretools-5.0.0/src/core/strategy_context/encrypted_programming_strategy_ctx.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 class EncryptedProgrammingStrategy(ABC):
     """
     The Strategy interface declares operations common to all
     supported versions of some algorithm.
     """
     @abstractmethod
-    def create_header(self, host_key, dev_pub_key, key_to_encrypt, algorithm,
-                      key_length):
+    def create_header(self, host_key, dev_pub_key, key_to_encrypt, key_length):
         pass
 
     @abstractmethod
     def create_encrypted_image(self, hex_file, aes_key_file, aes_header,
                                host_key_id, dev_key_id, out_file_encrypt,
                                padding_value):
         pass
@@ -54,21 +53,20 @@
     @strategy.setter
     def strategy(self, strategy: EncryptedProgrammingStrategy):
         """
         Allows replacing a Strategy object at runtime.
         """
         self._strategy = strategy
 
-    def create_header(self, host_key, dev_pub_key, key_to_encrypt, algorithm,
-                      key_length):
+    def create_header(self, host_key, dev_pub_key, key_to_encrypt, key_length):
         """
         Delegates work to the Strategy object.
         """
         return self._strategy.create_header(
-            self, host_key, dev_pub_key, key_to_encrypt, algorithm, key_length)
+            self, host_key, dev_pub_key, key_to_encrypt, key_length)
 
     def create_encrypted_image(self, hex_file, aes_key_file, aes_header,
                                host_key_id, dev_key_id, out_file_encrypt,
                                padding_value):
         """
         Delegates work to the Strategy object.
         """
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/strategy_context/prov_packet_strategy_ctx.py` & `cysecuretools-5.0.0/src/core/strategy_context/prov_packet_strategy_ctx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2022 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,52 +14,60 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from abc import ABC, abstractmethod
 
 
 class ProvisioningPacketStrategy(ABC):
+    """The Strategy interface declares operations common to all
+    supported versions of some algorithm
     """
-    The Strategy interface declares operations common to all supported versions
-    of some algorithm.
-    """
+
     @abstractmethod
     def create(self, target, **kwargs):
-        """ Creates provisioning packet """
+        """Creates provisioning packet"""
+
+    @abstractmethod
+    def verify(self, target, **kwargs):
+        """Verifies packet signature"""
+
+    @abstractmethod
+    def create_package(self, target, **kwargs):
+        """Creates provisioning package"""
 
     @abstractmethod
     def reverse_conversion(self, target, packets, output):
-        """ Converts provisioning packet back to policy """
+        """Converts provisioning packet back to policy"""
 
 
 class ProvisioningPacketCtx:
-    """
-    The Context defines the interface of interest to clients.
-    """
+    """The Context defines the interface of interest to clients"""
     def __init__(self, strategy: ProvisioningPacketStrategy):
         self._strategy = strategy
 
     @property
     def strategy(self) -> ProvisioningPacketStrategy:
-        """
-        The Context maintains a reference to one of the Strategy objects.
+        """The Context maintains a reference to one of the Strategy
+        objects
         """
         return self._strategy
 
     @strategy.setter
     def strategy(self, strategy: ProvisioningPacketStrategy):
-        """
-        Allows replacing a Strategy object at runtime.
-        """
+        """Allows replacing a Strategy object at runtime"""
         self._strategy = strategy
 
     def create(self, target, **kwargs):
-        """
-        Delegates work to the Strategy object.
-        """
+        """Delegates work to the Strategy object"""
         return self._strategy.create(target, **kwargs)
 
+    def verify(self, target, **kwargs):
+        """Delegates work to the Strategy object"""
+        return self._strategy.verify(target, **kwargs)
+
+    def create_package(self, target, **kwargs):
+        """Delegates work to the Strategy object"""
+        self._strategy.create_package(target, **kwargs)
+
     def reverse_conversion(self, target, packets, output):
-        """
-        Delegates work to the Strategy object.
-        """
+        """Delegates work to the Strategy object"""
         return self._strategy.reverse_conversion(target, packets, output)
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/strops.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
-
-def split_by_n(seq, n):
-    """ Splits string every N-th character """
-    return [seq[i:i + n] for i in range(0, len(seq), n)]
+from .aes_header_strategy import AesHeaderStrategy
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/target_builder.py` & `cysecuretools-5.0.0/src/core/target_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,11 +151,24 @@
     def get_test_packages(self):
         """
         Gets a dictionary with Python packages containing content for
         testing purpose
         """
 
     @abstractmethod
+    def get_certificate_strategy(self):
+        """
+        Gets an object containing implementation of certificate x509
+        generator
+        """
+
+    @abstractmethod
+    def get_app_loader(self):
+        """
+        Gets an object containing implementation of RAM application loading
+        """
+
+    @abstractmethod
     def get_silicon_id(self):
         """
         Gets the target silicon ID
         """
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/target_director.py` & `cysecuretools-5.0.0/src/core/target_director.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2022 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,15 +14,16 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import inspect
 from abc import ABCMeta
 from collections import namedtuple
-from cysecuretools.core.target_builder import TargetBuilder
+
+from .target_builder import TargetBuilder
 
 
 class TargetDirector:
     """
     The Director is only responsible for executing the building steps
     in a particular sequence. It is helpful when producing products
     according to a specific order or configuration.
@@ -129,26 +131,32 @@
         # Policy generator
         target.policy_generator = self._builder.get_policy_generator(
             policy_parser)
 
         # Python package name containing content for testing purpose
         target.test_packages = self._builder.get_test_packages()
 
+        # Certificate strategy
+        target.certificate_strategy = self._builder.get_certificate_strategy()
+
+        # Application loader
+        target.app_loader = self._builder.get_app_loader()
+
         # Target silicon ID
         target.silicon_id = self._builder.get_silicon_id()
 
         self._instantiate_types(target)
 
         return target
 
     @staticmethod
     def _instantiate_types(target):
         """
         Instantiates properties of a class type.
-        Some target parts use use the target as an input parameter
+        Some target parts use the target as an input parameter
         and must be instantiated when the target contains all parts
         """
         TypeObject = namedtuple('TypeObject', ['type', 'name'])
         for t in [TypeObject(getattr(target, m), m) for m in dir(target) if
                   not m.startswith('_')]:
             if isinstance(t.type, ABCMeta) or isinstance(t.type, type):
                 setattr(target, t.name, t.type(target))
@@ -180,14 +188,16 @@
         self._sign_tool = None
         self._key_source = None
         self._bootloader_provider = None
         self._version_provider = None
         self._debug_certificate = None
         self._policy_generator = None
         self._test_packages = None
+        self._certificate_strategy = None
+        self._app_loader = None
         self._silicon_id = None
 
     @property
     def name(self):
         return self._name
 
     @name.setter
@@ -407,13 +417,29 @@
         return self._test_packages
 
     @test_packages.setter
     def test_packages(self, packages):
         self._test_packages = packages
 
     @property
+    def certificate_strategy(self):
+        return self._certificate_strategy
+
+    @certificate_strategy.setter
+    def certificate_strategy(self, certificate_strategy):
+        self._certificate_strategy = certificate_strategy
+
+    @property
+    def app_loader(self):
+        return self._app_loader
+
+    @app_loader.setter
+    def app_loader(self, app_loader):
+        self._app_loader = app_loader
+
+    @property
     def silicon_id(self):
         return self._silicon_id
 
     @silicon_id.setter
     def silicon_id(self, silicon_id):
         self._silicon_id = silicon_id
```

### Comparing `cysecuretools-4.2.0/cysecuretools/core/voltage_tool.py` & `cysecuretools-5.0.0/src/core/voltage_tool.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/data/cy_bootloader_map.json` & `cysecuretools-5.0.0/src/data/cy_bootloader_map.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py` & `cysecuretools-5.0.0/src/data/mxs40sv2/mxs40sv2_ram_app_status_codes.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/data/mxs40v1/mxs40v1_sfb_status_codes.py` & `cysecuretools-5.0.0/src/data/mxs40v1/mxs40v1_sfb_status_codes.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/bootloader_provider_mxs40v1.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/bootloader_provider_mxs40v1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,25 +12,26 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import logging
-from cysecuretools.core.project import ProjectInitializer
-from cysecuretools.core.cy_bootloader_map_parser import CyBootloaderMapParser
+
+from ....core.project_base import ProjectInitializerBase
+from ....core.cy_bootloader_map_parser import CyBootloaderMapParser
 
 logger = logging.getLogger(__name__)
 
 
 class BootloaderProviderMXS40v1:
     def __init__(self, target):
         self.target = target
         self.policy_parser = target.policy_parser
-        self.cb_dir = ProjectInitializer.prebuilt_dir_name
+        self.cb_dir = ProjectInitializerBase.prebuilt_dirname
 
     def hex_path(self, from_project=None):
         """
         Gets CyBootloader hex-file path.
         :return: File path.
         """
         build_mode = self.policy_parser.get_cybootloader_mode()
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/debug_cert/debug_cert_mxs40sv2.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_mxs40sv2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.execute.image_signing.rsa_converter import RSAConverter
-from cysecuretools.core.key_handlers.rsa_handler import RSAHandler
-from cysecuretools.execute.debug_cert.debug_cert_parser_mxs40sv2 import (
-    DebugCertificateParserMXS40Sv2)
+import logging
+
+from .debug_cert_parser_mxs40sv2 import DebugCertificateParserMXS40Sv2
+from .....core.key_handlers.rsa_handler import RSAHandler
+
+logger = logging.getLogger(__name__)
 
 
 class DebugCertificateMXS40Sv2:
+    """Create: debug, transit to RMA certificates"""
 
-    def create(self, template, key, output, sign):
+    def create(self, template, key, output, sign, **_):
         """
         Creates debug or RMA certificate binary from the
         certificate in JSON format
         :param template:
             Path to the certificate template in JSON format
         :param key:
             This key will be used to add public key to the certificate.
@@ -50,18 +54,19 @@
         json_cert = self.add_pub_key(json_cert, key)
         payload = b''.join([json_cert[field] for field in cert_fields])
         if sign:
             cert = self.sign_cert(payload, key)
         else:
             cert = payload
         self.save_cert(output, cert)
+        logger.info('Debug certificate created (%s)', output)
 
     @staticmethod
     def add_pub_key(json_cert, priv_key):
-        key = RSAConverter.convert_to_mbedtls(priv_key)
+        key = RSAHandler.convert_to_mbedtls(priv_key)
         json_cert['public_key'] = bytearray.fromhex(key)
         return json_cert
 
     @staticmethod
     def sign_cert(payload, priv_key):
         signature = RSAHandler.sign(priv_key, payload)
         cert = payload + signature
@@ -71,13 +76,14 @@
     def add_signature(self, cert_file, signature_file, output):
         with open(cert_file, 'rb') as f:
             payload = f.read()
         with open(signature_file, 'rb') as f:
             signature = f.read()
         signed_cert = payload + signature
         self.save_cert(output, signed_cert)
+        logger.info('Debug certificate has been signed (%s)', output)
         return signed_cert
 
     @staticmethod
     def save_cert(path, cert):
         with open(path, 'wb') as f:
             f.write(cert)
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/debug_cert/debug_cert_parser_mxs40sv2.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/debug_cert/debug_cert_parser_mxs40sv2.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_cipher.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_cipher.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -28,15 +29,15 @@
     @staticmethod
     def get_bytes(data):
         if type(data) is str:
             return str.encode(data, 'utf-8')
         elif type(data) is bytes:
             return data
         else:
-            raise Exception('Unknown input data type.')
+            raise ValueError('Unknown input data type.')
 
 
 class AESCipherCBC(AESCipher):
     def __init__(self, key, iv):
         super().__init__(key, iv)
         self.cipher = Cipher(algorithms.AES(self.key), modes.CBC(self.iv), backend=self.backend)
 
@@ -50,23 +51,23 @@
         unpadder = padding.PKCS7(self.block_size).unpadder()
         return unpadder.update(decryptor.update(enc) + decryptor.finalize()) + unpadder.finalize()
 
 
 def read_key_from_file(key):
     content = key.splitlines()
     if len(content) < 2:
-        raise Exception('Not enough AES input data: in the file should be two lines: key, iv.')
+        raise ValueError('Not enough AES input data: in the file should be two lines: key, iv.')
 
     key = bytes.fromhex(content[0])
     iv = bytes.fromhex(content[1])
 
     if 8 * len(key) not in [128, 192, 256]:
-        raise Exception('Invalid AES Key length: should be 128, 192 or 256 bits.')
+        raise ValueError('Invalid AES Key length: should be 128, 192 or 256 bits.')
     check_iv_length(iv)
 
     return key, iv
 
 
 def check_iv_length(iv):
     if 8 * len(iv) != 128:
-        raise Exception('Invalid AES IV length: should be 128 bits.')
+        raise ValueError('Invalid AES IV length: should be 128 bits.')
     return True
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_header.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_header.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020-2021 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,46 +12,40 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import copy
 import logging
-from cysecuretools.execute.encrypted_programming.aes_cipher import (
-    AESCipherCBC, read_key_from_file)
-from cysecuretools.execute.encrypted_programming.ecc_kdf import EcdhKdf
+
+from .aes_cipher import AESCipherCBC, read_key_from_file
+from .ecc_kdf import EcdhKdf
 
 logger = logging.getLogger(__name__)
 
 AES_HEADER_AES_KEYDATA_SIZE = 64
 
 
 class AesHeader:
     @staticmethod
-    def create(host_key, dev_pub_key, key_to_encrypt, algorithm='ECC',
-               key_length=16,
+    def create(host_key, dev_pub_key, key_to_encrypt, key_length=16,
                salt=b'0000000000000000',
                info=b'0000000000000000'):
         """
         Generates encrypted header file.
-        :param algorithm: Asymmetric algorithm for KDF.
         :param host_key: Host key pair file.
         :param dev_pub_key: Device public key.
         :param key_length: Derived key (AES) length.
         :param salt: Salt for KDF.
         :param info: Info data for KDF
         :param key_to_encrypt: AES key filename (key and iv are
                used for image encryption), should be AES encrypted,
                using derived key.
         """
-        if algorithm in ['ECC']:
-            kdf_object = EcdhKdf(host_key, dev_pub_key, key_length, salt, info)
-        else:
-            raise ValueError('Algorithm not supported.')
-
+        kdf_object = EcdhKdf(host_key, dev_pub_key, key_length, salt, info)
         aes_header = AesHeader._get_header_info(kdf_object, key_to_encrypt)
         aes_header_hex = aes_header.hex()
         logger.debug('aes_header=%s', aes_header_hex)
 
         return aes_header_hex
 
     @staticmethod
@@ -60,17 +55,17 @@
 
         key_to_enc, iv_to_enc = read_key_from_file(key_to_encrypt_file)
         key_encrypted = aes.encrypt(key_to_enc + iv_to_enc)
         key_encrypted += bytearray([ord('0')] * (
                 AES_HEADER_AES_KEYDATA_SIZE - (len(key_encrypted))))
 
         if kdf_object.salt is None or kdf_object.info is None:
-            raise Exception('Salt and info should be presented...')
+            raise ValueError('Salt and info should be presented...')
         if len(kdf_object.salt) != 16 or len(kdf_object.info) != 16:
-            raise Exception('Salt and info fields length should be 16 bytes')
+            raise ValueError('Salt and info fields length should be 16 bytes')
 
         aes_key_iv_padding = AesHeader._split_list_to_bytes(key_encrypted, 16)
         aes_key_iv_padding.append(copy.copy(list(kdf_object.salt)))
         aes_key_iv_padding.append(copy.copy(list(kdf_object.info)))
 
         for i in range(len(aes_key_iv_padding)):
             aes_key_iv_padding[i] = aes_key_iv_padding[i]
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/aes_header_strategy.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/aes_header_strategy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,22 +12,22 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import logging
+
 from intelhex import IntelHex
-import cysecuretools.execute.encrypted_programming.encrypted_programming \
-    as encrypted_programming
-from cysecuretools.execute.encrypted_programming.aes_header import AesHeader
-from cysecuretools.execute.encrypted_programming.aes_cipher import (
-    AESCipherCBC, read_key_from_file)
-from cysecuretools.core.strategy_context.encrypted_programming_strategy_ctx \
-    import EncryptedProgrammingStrategy
+
+from . import encrypted_programming
+from .aes_header import AesHeader
+from .aes_cipher import AESCipherCBC, read_key_from_file
+from .....core.strategy_context import EncryptedProgrammingStrategy
+
 
 logger = logging.getLogger(__name__)
 
 FLASH_ROW_SIZE = 512
 MAIN_FLASH_START_ADDR = 0x10000000
 
 
@@ -42,18 +43,17 @@
         for i in range(0, len(in_list), n):
             yield in_list[i:i + n]
 
     @staticmethod
     def hex_str_wo_header(data):
         return "%02X" % data
 
-    def create_header(self, host_key, dev_pub_key, key_to_encrypt, algorithm,
-                      key_length):
+    def create_header(self, host_key, dev_pub_key, key_to_encrypt, key_length):
         return AesHeader.create(host_key, dev_pub_key, key_to_encrypt,
-                                algorithm, key_length)
+                                key_length)
 
     def create_encrypted_image(self, hex_file, aes_key_file, aes_header,
                                host_key_id, dev_key_id, out_file_encrypt,
                                padding_value=0):
         """
         Creates encrypted image for encrypted programming
         Format:
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/ecc_kdf.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/ecc_kdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
+
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.kdf.hkdf import HKDF
 from cryptography.hazmat.primitives import serialization
 
 
@@ -55,15 +57,15 @@
     @staticmethod
     def get_bytes(data):
         if type(data) is str:
             return str.encode(data, 'utf-8')
         elif type(data) is bytes:
             return data
         else:
-            raise Exception('Unknown input data type.')
+            raise ValueError('Unknown input data type.')
         
     @staticmethod
     def read_key_bytes(key_file):
         with open(key_file, 'rb') as key_file:
             return key_file.read()
 
     def derive_key(self):
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/encrypted_programming/encrypted_programming.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/encrypted_programming/encrypted_programming.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,17 +13,17 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import logging
 from enum import IntEnum
-from cysecuretools.core import progress_bar
-from cysecuretools.execute.sys_call import encrypted_programming
-from cysecuretools.execute.programmer.base import ResetType
+
+from ..provisioning.sys_call import encrypted_programming
+from .....core import progress_bar
 
 ENCRYPTED_DATA_LEN = 0x210
 
 logger = logging.getLogger(__name__)
 
 
 class EPMode(IntEnum):
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/exam_cyb06xx7.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/entrance_exam/exam_cyb06xx7.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,19 +12,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import hashlib
 import logging
-from cysecuretools.core.target_director import Target
-from cysecuretools.core.enums import EntranceExamStatus
-from cysecuretools.execute.provisioning_packet.lib import Crypto
-from cysecuretools.execute.entrance_exam.exam_mxs40v1 import \
-    EntranceExamMXS40v1
+
+from . import EntranceExamMXS40v1
+from .....core.target_director import Target
+from .....core.enums import EntranceExamStatus
+from .....execute import jwt
 
 logger = logging.getLogger(__name__)
 
 
 class EntranceExamCyb06xx7(EntranceExamMXS40v1):
     def __init__(self, target: Target, **kwargs):
         super(EntranceExamCyb06xx7, self).__init__(target, **kwargs)
@@ -44,16 +45,16 @@
                 return EntranceExamStatus.FAIL
 
     def verify_asset_hash(self, tool):
         """
         Verifies SecureFlashBoot asset hash
         """
         logger.info('Verify SecureFlashBoot asset hash:')
-        jwt_text = Crypto.read_jwt(self.entrance_exam_jwt)
-        json_data = Crypto.readable_jwt(jwt_text)
+        jwt_text = jwt.read_jwt(self.entrance_exam_jwt)
+        json_data = jwt.readable_jwt(jwt_text)
         payload = json_data['payload']['ahb_reads8']
 
         segments = self._get_sfb_toc1_segments(tool)
         sfb_hash = self._calculate_sfb_asset_hash(tool, segments)
 
         exam_pass = self._compare_asset_hash(sfb_hash, payload)
         return exam_pass
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/entrance_exam/exam_mxs40v1.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/entrance_exam/exam_mxs40v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,29 +13,30 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import logging
 
-from cysecuretools.core.connect_helper import ConnectHelper
-from cysecuretools.core.enums import EntranceExamStatus, RegionHashStatus
-from cysecuretools.core.strategy_context.provisioning_strategy_ctx import ProvisioningContext
-from cysecuretools.execute.sys_call import region_hash, read_lifecycle
-from cysecuretools.execute.programmer.base import AP
-from cysecuretools.execute.provisioning_packet.lib import Crypto
-from cysecuretools.core.target_director import Target
-from cysecuretools.core.entrance_exam_base import EntranceExam
-from cysecuretools.targets.common.p64.enums import ProtectionState
+from ..enums import ProtectionState
+from ..provisioning.sys_call import region_hash, read_lifecycle
+from .....__about__ import __pkg_name__
+from .....core.enums import EntranceExamStatus, RegionHashStatus
+from .....core.target_director import Target
+from .....core.connect_helper import ConnectHelper
+from .....core.entrance_exam_base import EntranceExam
+from .....core.strategy_context import ProvisioningContext
+from .....execute import jwt
+from .....execute.programmer.base import AP
 
 logger = logging.getLogger(__name__)
 
 ENTRANCE_EXAM_JWT = 'entrance_exam.jwt'
 SFB_VER_ERROR = 'Engineering Sample version of PSoC64 detected, the current ' \
-                'version of CySecureTools is incompatible. Please contact ' \
+                f'version of {__pkg_name__} is incompatible. Please contact ' \
                 'Cypress to receive production versions of PSoC64 Silicon\n'
 
 
 class EntranceExamMXS40v1(EntranceExam):
     def __init__(self, target: Target, **kwargs):
         super().__init__(target, **kwargs)
         self.reg_map = target.register_map
@@ -46,15 +48,15 @@
         return os.path.abspath(os.path.join(packet_dir, ENTRANCE_EXAM_JWT))
 
     def execute(self, tool, **kwargs):
         """
         Checks device life-cycle, FlashBoot firmware, Flash state and
         a bunch of registers.
         """
-        jwt_text = Crypto.read_jwt(self.entrance_exam_jwt)
+        jwt_text = jwt.read_jwt(self.entrance_exam_jwt)
 
         logger.info('*****************************************')
         logger.info('             ENTRANCE EXAM               ')
         logger.info('*****************************************')
 
         complete = self.target.silicon_data_reader.read_complete_status(tool)
         exam_pass = not complete
@@ -85,23 +87,23 @@
                 exam_pass = True
             tool.set_ap(AP.SYS)
 
         # Verify entrance exam JWT signature
         if exam_pass:
             logger.info('Verify entrance exam JWT signature:')
             cy_pub_key = self.target.key_reader.get_cypress_public_key()
-            exam_pass = Crypto.validate_jwt(jwt_text, cy_pub_key)
+            exam_pass = jwt.validate_jwt(jwt_text, cy_pub_key)
             if exam_pass:
                 logger.info('Signature verified')
             else:
                 logger.error('Invalid signature')
 
         # Verify ahb_reads32
         if exam_pass:
-            json_data = Crypto.readable_jwt(jwt_text)
+            json_data = jwt.readable_jwt(jwt_text)
             payload = json_data['payload']
             tool.reset()
             exam_pass = self.verify_ahb_reads(tool, payload['ahb_reads'], 32)
 
         # Verify ahb_reads8
         if exam_pass:
             exam_pass &= self.verify_ahb_reads(tool, payload['ahb_reads8'], 8)
@@ -145,16 +147,16 @@
         try:
             protection_state = ProtectionState(lifecycle).name
         except ValueError:
             protection_state = f'{ProtectionState.unknown.name} ({lifecycle})'
         logger.info('Chip protection state: %s', protection_state.capitalize())
 
     def read_sfb_version(self, tool):
-        jwt_text = Crypto.read_jwt(self.entrance_exam_jwt)
-        json_data = Crypto.readable_jwt(jwt_text)
+        jwt_text = jwt.read_jwt(self.entrance_exam_jwt)
+        json_data = jwt.readable_jwt(jwt_text)
         payload = json_data['payload']
         major_version = None
         minor_version = None
         for item in payload['ahb_reads']:
             if item['description'].startswith('SFB_VER_HI'):
                 address = int(item['address'], 0)
                 mask = int(item['mask'], 0)
@@ -198,15 +200,15 @@
             value = int(item['value'], 0)
 
             if bits == 8:
                 read_value = tool.read8(address) & mask
             elif bits == 32:
                 read_value = tool.read32(address) & mask
             else:
-                ValueError('Invalid number of bits.')
+                raise ValueError('Invalid number of bits.')
 
             expected_value = value & mask
             logger.info('Address: %s', item["address"])
             logger.info('Expected value:     0x%x', expected_value)
             logger.info('Received value:     0x%x', read_value)
             if read_value == expected_value:
                 logger.info('PASS\n')
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/image_cert.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/image_cert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2018-2021 Cypress Semiconductor Corporation
+Copyright 2018-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,20 +13,22 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import hashlib
 from datetime import datetime
+
 from click import BadParameter
 from intelhex import IntelHex
-from cysecuretools.core.json_helper import dump_json
-import cysecuretools.execute.jwt as jwt
-import cysecuretools.execute.sys_call as sys_call
-from cysecuretools.execute.key_reader import load_key
+
+from .provisioning import sys_call
+from ....execute import jwt
+from ....execute.key_reader import load_key
+from ....core.json_helper import dump_json
 
 
 class ImageCertificate:
     def __init__(self, image, key, output, version, image_id, exp_date_str):
         self.image = image
         self.key = key
         self.output = output
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/image_signing/encrypt_mxv40sv2.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/image_signing/encrypt_mxv40sv2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,17 +12,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import struct
-from cryptography.hazmat.primitives.ciphers import (
-    Cipher, algorithms, modes
-)
+
+from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
 NONCE_SIZE = 12
 
 
 class EncryptorMXS40Sv2:
     def __init__(self, key):
         if isinstance(key, bytes):
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/image_signing/image_config_parser.py` & `cysecuretools-5.0.0/src/execute/image_signing/image_config_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright (c) 2022 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core.json_helper import read_json
+from ...core.json_helper import read_json
 
 
 class ImageConfigParser:
+    """Class for parsing image config JSON,
+    used to add TLVs to RAM app images
+    """
 
     @staticmethod
     def get_image_tlvs(config_file):
         """
         Gets tag-value pairs that will be added to the protected TLV area
         :param config_file: Path to the image config file
         """
         config = read_json(config_file)
-        tlv_list = dict()
+        tlv_list = {}
         for tlv in config['tlv']:
             tlv_value = '0x'
             if isinstance(tlv['value'], list):
                 for v in tlv['value']:
                     int_value = int(v['value'], 0)
-                    byte_value = int_value.to_bytes(v['length'], byteorder='little')
+                    byte_value = int_value.to_bytes(v['length'],
+                                                    byteorder='little')
                     hex_value = byte_value.hex()
                     tlv_value += hex_value
             else:
                 tlv_value = tlv['value']
 
             tlv_list[tlv['tag']] = tlv_value
         return tlv_list
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/image_signing/signtool_mxs40v1.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/signtool_mxs40v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2022 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -14,33 +15,30 @@
 limitations under the License.
 """
 import os
 import sys
 import logging
 import tempfile
 import binascii
-import importlib
 import pathlib
 from shutil import copy2
-from inspect import getmembers
 
-import click
 from intelhex import IntelHex
 
-from cysecuretools.core.enums import ImageType
-from cysecuretools.core.signtool_base import SignTool
-from cysecuretools.execute.key_reader import is_private_key
-from cysecuretools.execute.image_signing.image import Image, TLV
-import cysecuretools.execute.imgtool.main as imgtool
-from cysecuretools.execute.imgtool.image import TLV_VALUES
+from ....execute.image_signing.image import Image, TLV
+from ....execute import key_reader
+from ....execute.imgtool.image import TLV_VALUES
+from ....core.enums import ImageType
+from ....core.signtool_base import SignToolBase
+
 
 logger = logging.getLogger(__name__)
 
 
-class SignToolMXS40v1(SignTool):
+class SignToolMXS40v1(SignToolBase):
     """
     Implements image signing functionality for the MXS40v1 platform.
     The class can be used to sign binary and Intel hex images. However,
     it always operates with the binary. If the Intel hex image was
     specified, it is converted to the binary before the signing.
     The self.tmp_bin is a path to the binary to be signed.
     For the Intel hex format, a temporary binary file is created.
@@ -72,84 +70,83 @@
         self.slot = None
         self.enckey = None
         self.output = None
         self.tlv = []
         self.protected_tlv = []
         self.mem_map = target.memory_map
 
-    def add_metadata(self, image_path, **kwargs):
+    def add_metadata(self, image, **kwargs):
         """Adds MCUboot metadata to the image. Optionally
         encrypts the image
         """
-        self._initialize(image_path, kwargs)
-
+        self._initialize(image, kwargs)
         self._validate_output_extension('bin')
 
-        result = self._process_image(
-            'sign', image_path, kwargs.get('erased_val'),
-            pubkey=kwargs.get('pubkey'))
+        result = self._process_image('sign', image, kwargs.get('erased_val'),
+                                     pubkey=kwargs.get('pubkey'))
 
         decrypted = None
         if self.enckey and self.image_type == 'UPGRADE':
             decrypted = self._get_decrypted(kwargs)
-            self._replace_image_body(result[0], self.tmp_bin, output=decrypted)
+            self.replace_image_body(result[0], self.tmp_bin, self.header_size,
+                                    self.erased_val, output=decrypted)
             logger.info(
                 "Saved decrypted image to '%s'", os.path.abspath(decrypted))
             logger.info(
                 'Image signature is calculated based on decrypted data. Ensure '
                 'the decrypted image is used for signing with HSM')
 
         self._cleanup()
         return tuple([result[0], decrypted]) if len(result) > 0 else None
 
     @staticmethod
-    def extract_payload(image_path, output):
+    def extract_payload(image, output):
         """Extracts a part to be signed from MCUboot image"""
-        image = Image(image_path)
-        if not image.has_metadata:
+        img = Image(image)
+        if not img.has_metadata:
             raise ValueError('The image does not have metadata')
         with open(output, 'wb') as f:
-            f.write(image.payload)
+            f.write(img.payload)
         logger.info("Saved image payload to '%s'", os.path.abspath(output))
 
     @staticmethod
-    def add_signature(image_path, signature, output):
+    def add_signature(image, signature, alg=None, output=None):
         """Adds ECDSA256 signature into MCUboot image"""
-        image = Image(image_path)
+        img = Image(image)
         with open(signature, 'rb') as f:
             sig_bytes = f.read()
 
-        image.remove_tlv(TLV_VALUES['ECDSA256'])
-        image.add_tlv(TLV(TLV_VALUES['ECDSA256'], sig_bytes))
+        img.remove_tlv(TLV_VALUES['ECDSA256'])
+        img.add_tlv(TLV(TLV_VALUES['ECDSA256'], sig_bytes))
 
-        if image.is_upgrade():
+        if img.is_upgrade():
             ecdsa_sig_max_len = 72
-            pad_value = image.header[-1]
+            pad_value = img.header.header_bytes()[-1]
             pad_length = ecdsa_sig_max_len - len(sig_bytes)
             pad = pad_value.to_bytes(1, byteorder='big') * pad_length
-            image.trailer = pad + image.trailer
+            img.trailer = pad + img.trailer
 
-        data = image.data
+        data = img.data
         with open(output, 'wb') as f:
             f.write(data)
         logger.info("Saved image to '%s'", os.path.abspath(output))
 
-    def sign_image(self, image_path, **kwargs):
+    def sign_image(self, image, **kwargs):
         """Signs bin or hex image with the key specified
         in the policy. Optionally encrypts the image
         """
-        img = Image(image_path)
+        img = Image(image)
         if img.is_signed:
             raise ValueError(
                 'Signature not added. The image has been already signed')
 
-        self._initialize(image_path, kwargs)
+        self._initialize(image, kwargs)
 
         result = self._process_image(
-            'sign', image_path, kwargs.get('erased_val'))
+            'sign', image, kwargs.get('erased_val'))
 
         self._cleanup()
         return tuple(result) if len(result) > 0 else None
 
     def backup_image(self, image):
         """Creates an image binary backup. All manipulations are going to be
         done with it. The original image stays unchanged"""
@@ -197,15 +194,17 @@
             self._load_image(image_backup)
 
             if current_image_type == ImageType.BOOT.name:
                 processed_bin = method(current_image_type, self.output.boot,
                                        image['address'], **kwargs)
 
                 if self.enckey is not None:
-                    self._replace_image_body(processed_bin, self.tmp_bin)
+                    self.replace_image_body(
+                        processed_bin, self.tmp_bin, self.header_size,
+                        self.erased_val, output=processed_bin)
                     if self.output.boot.endswith('.hex'):
                         self.bin2hex(
                             processed_bin, self.output.boot, image['address'])
                 result.append(self.output.boot)
             elif current_image_type == ImageType.UPGRADE.name:
                 if not self.slot.get('upgrade', False):
                     continue
@@ -290,52 +289,17 @@
 
         if output.endswith('.hex'):
             self.bin2hex(tmp_output, output, image_address)
             self.tmp_files.append(tmp_output)
 
         logger.info(
             'Image for slot %s %s successfully (%s)', image_type,
-            'signed' if is_private_key(key) else 'processed', output)
+            'signed' if key_reader.is_private_key(key) else 'processed', output)
         return tmp_output
 
-    def _replace_image_body(self, orig, repl, output=None):
-        """
-        Replaces original image with the replacement image
-        :param orig: Original binary image
-        :param repl: Binary image to replace with
-        :param output: Output file
-        """
-        if output is None:
-            output = orig
-
-        with open(orig, 'rb') as of:
-            original = of.read()
-        with open(repl, 'rb') as rf:
-            replacement = rf.read()
-
-        modified = bytearray(original)
-        body_start = self.header_size
-        body_end = self.header_size + len(replacement)
-
-        j = 0
-        for i in range(body_start, body_end):
-            modified[i] = replacement[j]
-            j += 1
-
-        # This adds padding if the image is not aligned to 16 Bytes
-        pad_len = body_end % 16
-        pad_value = int(self.erased_val, 0)
-        if pad_len > 0:
-            pad_len = 16 - pad_len
-            for i in range(body_end, body_end + pad_len):
-                modified[i] = pad_value
-
-        with open(output, 'wb') as of:
-            of.write(modified)
-
     def _cleanup(self):
         """ Removes temporary files created during image signing """
         for file in self.tmp_files:
             if file is not None:
                 try:
                     os.remove(file)
                 except OSError:
@@ -483,20 +447,7 @@
             raise ValueError(f'Invalid value {upgrade_mode}')
 
     def _validate_output_extension(self, expected_ext):
         for out in [self.output.boot, self.output.upgrade]:
             if out is not None and not out.endswith(f'.{expected_ext}'):
                 raise ValueError(
                     f"Invalid output file type '{out}'. Use (.{expected_ext})")
-
-    @staticmethod
-    def _call_imgtool_sign(args):
-
-        def _call_click_command(cmd: click.Command, *args, **kwargs):
-            result = cmd.callback(*args, **kwargs)
-            return result
-
-        module = importlib.import_module('cysecuretools.execute.imgtool.main')
-        for _, obj in getmembers(module):
-            if isinstance(obj, click.Command) and obj.name == 'sign':
-                _call_click_command(obj, **args)
-                break
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/image_signing/signtool_mxv40sv2.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/image_signing/signtool_mxv40sv2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021-2022 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,37 +13,35 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import logging
 import binascii
-import click
-import importlib
 from shutil import copy2
 from pathlib import Path
-from inspect import getmembers
 
-import cysecuretools.execute.imgtool.main as imgtool
-from cysecuretools.execute.imgtool.keys import ecdsa
-from cysecuretools.core.signtool_base import SignTool
-from cysecuretools.core.key_handlers import RSAHandler
-from .image_config_parser import ImageConfigParser
-from .rsa_converter import RSAConverter
 from .encrypt_mxv40sv2 import EncryptorMXS40Sv2
-from .xip_encryptor import XipEncryptor
-from cysecuretools.targets.common.mxs40sv2.enums import PolicyType
-from cysecuretools.execute.image_signing.image import Image
-from ...targets.common.mxs40sv2.nv_counter_calc import NvCounterCalculator
-
+from .xip_encryptor_mxs40sv2 import XipEncryptor
+from ..enums import PolicyType
+from ..nv_counter_calc import NvCounterCalculator
+from .....execute.image_signing.image import Image
+from .....execute.image_signing.image_config_parser import ImageConfigParser
+from .....execute.imgtool.keys import ecdsa
+from .....execute.imgtool import main as imgtool
+from .....core.signtool_base import SignToolBase
+from .....core.key_handlers.rsa_handler import RSAHandler
+from .....core.key_handlers.ec_handler import ECHandler
 
 logger = logging.getLogger(__name__)
 
 
-class SignToolMXS40Sv2(SignTool):
+class SignToolMXS40Sv2(SignToolBase):
+    """Image signing and manipulations with its data"""
+
     IMAGE_ALIGNMENT = 8
     WARN_SLOT_SIZE = 0x400000
     IMAGE_VERSION = '0.1'
 
     def __init__(self, target):
         self.target = target
         self.mem_map = self.target.memory_map
@@ -82,15 +81,15 @@
 
         tlvs = self._get_config_tlvs(kwargs.get('image_config'))
         for t, v in tlvs.items():
             protected_tlv.append((t, v))
 
         nv_counter = None
         if self.policy_parser.json:
-            policy_type = self.policy_parser.get_policy_type()
+            policy_type = self.policy_parser.policy_type()
             if policy_type == PolicyType.REPROVISIONING_SECURE:
                 nv_counter, update_packet = self._get_update_packet_data(
                    update_key_id, update_key_path, image_id)
                 protected_tlv.append(update_packet)
             else:
                 if update_key_id is not None or update_key_path:
                     logger.warning(
@@ -113,45 +112,45 @@
             logger.info('Image processed successfully (%s)', output)
         except Exception as e:
             logger.error('Failed to add data to the image')
             logger.error('imgtool finished execution with errors')
             raise e
         return output
 
-    def sign_image(self, image_path, **kwargs):
+    def sign_image(self, image, **kwargs):
         """
         Signs image with the key specified in the policy file.
         Creates copy of unsigned hex file.
-        :param image_path: The file to sign.
+        :param image: The file to sign.
         :return: Path to the signed file
         """
-        img = Image(image_path)
+        img = Image(image)
         if img.is_signed:
             raise ValueError(
                 'Signature not added. The image has been already signed')
 
         key_path = self._get_key_path(kwargs)
         erased_val = self._get_erased_val(kwargs)
         image_format = self._get_image_format(kwargs)
         header_size = self._get_header_size(image_format, kwargs)
         slot_size = self._get_slot_size(kwargs)
         app_addr = self._get_app_addr(kwargs)
         hex_addr = self._get_hex_addr(kwargs)
-        output = self._get_output(image_path, 'unsigned', kwargs)
+        output = self._get_output(image, 'unsigned', kwargs)
         enckey = self._get_enckey(kwargs)
         pad = self._get_pad(kwargs)
         confirm = self._get_confirm(image_format, kwargs)
         overwrite_only = self._get_overwrite_only(image_format, kwargs)
         min_erase_size = self._get_min_erase_size(kwargs)
         align = self._get_align(kwargs)
         dependencies = self._get_dependencies(kwargs)
         image_version = self._get_image_version(kwargs)
         image_id = self._get_image_id(kwargs)
 
-        if not RSAHandler.is_private_key(key_path):
+        if not self._is_private_key(key_path):
             raise ValueError(f'Signing image with public key \'{key_path}\'')
 
         self._time_warning(pad, slot_size)
 
         tlvs = self._get_config_tlvs(kwargs.get('image_config'))
 
         if 'mcuboot_user_app' == image_format and enckey:
@@ -174,15 +173,15 @@
             'slot_size': slot_size,
             'pad': pad,
             'confirm': confirm,
             'max_sectors': 512,
             'overwrite_only': overwrite_only,
             'endian': 'little',
             'encrypt': enckey if 'mcuboot_user_app' == image_format else None,
-            'infile': image_path,
+            'infile': image,
             'outfile': output,
             'dependencies': dependencies,
             'load_addr': None,
             'hex_addr': hex_addr,
             'erased_val': erased_val,
             'save_enctlv': False,
             'security_counter': None,
@@ -195,18 +194,18 @@
             'encryptor': encryptor,
         }
 
         for t, v in tlvs.items():
             args['custom_tlv'].append((t, v))
 
         if image_format in ['bootrom_next_app', 'bootrom_ram_app']:
-            pubkey_data = RSAConverter.convert_to_mbedtls(key_path)
+            pubkey_data = RSAHandler.convert_to_mbedtls(key_path)
             args['custom_tlv'].append(('0xf0', f'0x{pubkey_data}'))
 
-        policy_type = self.policy_parser.get_policy_type()
+        policy_type = self.policy_parser.policy_type()
         if policy_type == PolicyType.REPROVISIONING_SECURE:
             nv_counter, update_packet = self._get_update_packet_data(
                 kwargs.get('update_key_id'), kwargs.get('update_key_path'),
                 image_id)
             args['security_counter'] = nv_counter
             args['custom_tlv'].append(update_packet)
 
@@ -240,14 +239,28 @@
             else:
                 logger.info(
                     'Image signed and encrypted successfully (%s)', output)
         else:
             logger.info('Image signed successfully (%s)', output)
         return output
 
+    def add_metadata(self, image, **kwargs):
+        """N/A for MXS40Sv2 platform"""
+        raise NotImplementedError
+
+    @staticmethod
+    def extract_payload(image, output, **kwargs):
+        """N/A for MXS40Sv2 platform"""
+        raise NotImplementedError
+
+    @staticmethod
+    def add_signature(image, signature, alg, output=None):
+        """N/A for MXS40Sv2 platform"""
+        raise NotImplementedError
+
     def _get_update_packet_data(self, update_key_id, update_key_path, image_id):
         if update_key_id is None and update_key_path is None:
             raise KeyError('Either update data packet key ID or key path '
                            'must be specified')
         if update_key_path is None:
             update_key_path = self.key_source.get_key(update_key_id, 'private')
 
@@ -258,33 +271,31 @@
 
         reprov_data = binascii.hexlify(self._reprovisioning_packet(
             key_id=update_key_id, key_path=update_key_path,
             image_id=image_id)).decode()
         return nv_counter, ('0x51', f'0x{reprov_data}')
 
     def _reprovisioning_packet(self, **kwargs):
-        from ..provisioning_packet.provisioning_packet_mxs40sv2 import (
-            ProvisioningPacketMXS40Sv2)
-        packet = ProvisioningPacketMXS40Sv2(self.policy_parser)
-        return packet.reprovisioning_data(self.target.key_source, **kwargs)
+        return self.target.provisioning_packet_strategy.reprovisioning_data(
+            self.target.key_source, **kwargs)
 
     def _time_warning(self, pad, slot_size):
         if pad:
             if slot_size > self.mem_map.MAX_SLOT_SIZE:
                 logger.warning('The slot size is %s bytes. The padding '
                                'operation may take a long time', slot_size)
             elif slot_size > self.WARN_SLOT_SIZE:
                 logger.warning('The slot size is %s bytes. The padding '
                                'operation may take a while', slot_size)
 
     @staticmethod
     def _get_pubkey(kwargs):
         pubkey = kwargs.get('pubkey')
         if pubkey is not None:
-            pubkey_data = RSAConverter.convert_to_mbedtls(pubkey)
+            pubkey_data = RSAHandler.convert_to_mbedtls(pubkey)
         else:
             pubkey_data = None
         return pubkey_data
 
     def _get_enckey(self, kwargs):
         if kwargs.get('encrypt', False):
             enckey = kwargs.get('enckey')
@@ -358,16 +369,15 @@
     def _get_pad(kwargs):
         return kwargs.get('pad', False)
 
     @staticmethod
     def _get_confirm(image_format, kwargs):
         if image_format == 'mcuboot_user_app':
             return kwargs.get('confirm', False)
-        else:
-            return False
+        return False
 
     @staticmethod
     def _get_image_id(kwargs):
         image_id = kwargs.get('image_id')
         return 0 if image_id is None else image_id
 
     @staticmethod
@@ -410,36 +420,41 @@
     def _copy_input_image(image_path, suffix):
         unsigned = '{0}_{2}{1}'.format(*os.path.splitext(image_path) + (
             suffix,))
         copy2(image_path, unsigned)
 
     @staticmethod
     def _get_config_tlvs(image_config):
-        tlvs = dict()
+        tlvs = {}
         if image_config is not None:
             if os.path.isfile(image_config):
                 tlvs = ImageConfigParser.get_image_tlvs(image_config)
             else:
                 raise FileNotFoundError(
                     f'Image configuration file \'{image_config}\' not found')
         return tlvs
 
     @staticmethod
+    def _is_private_key(key_path):
+        """Gets a value indicating whether a key
+        is a private key of RSA or EC type"""
+        k = SignToolMXS40Sv2.load_key(key_path)
+
+        try:
+            is_private = RSAHandler.is_private_key(k)
+        except ValueError:
+            try:
+                is_private = ECHandler.is_private_key(k)
+            except ValueError as e:
+                raise ValueError(
+                    f"Invalid or unsupported key '{key_path}'") from e
+
+        return is_private
+
+    @staticmethod
     def _cleanup(file):
         """Removes file"""
         if file is not None:
             try:
                 os.remove(file)
             except OSError:
                 pass
-
-    @staticmethod
-    def _call_imgtool_sign(args):
-
-        def _call_click_command(cmd: click.Command, *args, **kwargs):
-            result = cmd.callback(*args, **kwargs)
-            return result
-
-        module = importlib.import_module('cysecuretools.execute.imgtool.main')
-        for _, obj in getmembers(module):
-            if isinstance(obj, click.Command) and obj.name == 'sign':
-                _call_click_command(obj, **args)
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/image_signing/xip_encryptor.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/image_signing/xip_encryptor_mxs40sv2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from ..imgtool.custom_encryptor import CustomEncryptor
-from ..image_signing.encrypt_mxv40sv2 import EncryptorMXS40Sv2
+from .encrypt_mxv40sv2 import EncryptorMXS40Sv2
+from .....execute.imgtool.custom_encryptor import CustomEncryptor
 
 
 class XipEncryptor(CustomEncryptor):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.header_size = kwargs.get('header_size')
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/boot_record.py` & `cysecuretools-5.0.0/src/execute/imgtool/boot_record.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/custom_encryptor.py` & `cysecuretools-5.0.0/src/execute/imgtool/custom_encryptor.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/image.py` & `cysecuretools-5.0.0/src/execute/imgtool/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         'PUBKEY': 0x02,
         'SHA256': 0x10,
         'RSA2048': 0x20,
         'ECDSA224': 0x21,
         'ECDSA256': 0x22,
         'RSA3072': 0x23,
         'ED25519': 0x24,
+        'RSA4096': 0x25,
         'ENCRSA2048': 0x30,
         'ENCKW128': 0x31,
         'ENCEC256': 0x32,
         'ENCX25519': 0x33,
         'DEPENDENCY': 0x40,
         'SEC_CNT': 0x50,
         'BOOT_RECORD': 0x60,
@@ -197,14 +198,28 @@
                     self.slot_size,
                     self.max_sectors,
                     self.overwrite_only,
                     self.endian,
                     self.__class__.__name__,
                     len(self.payload))
 
+    @staticmethod
+    def header_format(endian):
+        return (endian +
+                # type ImageHdr struct {
+                'I' +     # Magic    uint32
+                'I' +     # LoadAddr uint32
+                'H' +     # HdrSz    uint16
+                'H' +     # PTLVSz   uint16
+                'I' +     # ImgSz    uint32
+                'I' +     # Flags    uint32
+                'BBHI' +  # Vers     ImageVersion
+                'I'       # Pad1     uint32
+                )  # }
+
     def load(self, path):
         """Load an image from a given file"""
         ext = os.path.splitext(path)[1][1:].lower()
         try:
             if ext == INTEL_HEX_EXT:
                 ih = IntelHex(path)
                 self.payload = ih.tobinarray()
@@ -518,26 +533,15 @@
             if self.load_addr != 0:
                 # Indicates that this image should be loaded into RAM
                 # instead of run directly from flash.
                 flags |= IMAGE_F['RAM_LOAD']
             if self.rom_fixed:
                 flags |= IMAGE_F['ROM_FIXED']
 
-            e = STRUCT_ENDIAN_DICT[self.endian]
-            fmt = (e +
-                   # type ImageHdr struct {
-                   'I' +     # Magic    uint32
-                   'I' +     # LoadAddr uint32
-                   'H' +     # HdrSz    uint16
-                   'H' +     # PTLVSz   uint16
-                   'I' +     # ImgSz    uint32
-                   'I' +     # Flags    uint32
-                   'BBHI' +  # Vers     ImageVersion
-                   'I'       # Pad1     uint32
-                   )  # }
+            fmt = self.header_format(STRUCT_ENDIAN_DICT[self.endian])
             assert struct.calcsize(fmt) == IMAGE_HEADER_SIZE
             header = struct.pack(fmt,
                     IMAGE_MAGIC,
                     self.rom_fixed or self.load_addr,
                     self.header_size,
                     protected_tlv_size,  # TLV Info header + Protected TLVs
                     len(self.payload) - self.header_size,  # ImageSz
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/__init__.py` & `cysecuretools-5.0.0/src/execute/imgtool/keys/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Cryptographic key management for imgtool.
 """
-
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric.rsa import (
     RSAPrivateKey, RSAPublicKey)
 from cryptography.hazmat.primitives.asymmetric.ec import (
     EllipticCurvePrivateKey, EllipticCurvePublicKey)
 from cryptography.hazmat.primitives.asymmetric.ed25519 import (
@@ -37,36 +36,39 @@
 
 class PasswordRequired(Exception):
     """Raised to indicate that the key is password protected, but a
     password was not specified."""
     pass
 
 
-def load(path, passwd=None):
+def load(key, passwd=None):
     """Try loading a key from the given path.  Returns None if the password wasn't specified."""
-    with open(path, 'rb') as f:
-        raw_pem = f.read()
-    try:
-        pk = serialization.load_pem_private_key(
-                raw_pem,
-                password=passwd,
-                backend=default_backend())
-    # Unfortunately, the crypto library raises unhelpful exceptions,
-    # so we have to look at the text.
-    except TypeError as e:
-        msg = str(e)
-        if "private key is encrypted" in msg:
-            return None
-        raise e
-    except ValueError:
-        # This seems to happen if the key is a public key, let's try
-        # loading it as a public key.
-        pk = serialization.load_pem_public_key(
-                raw_pem,
-                backend=default_backend())
+
+    if isinstance(key, str):
+        with open(key, 'rb') as f:
+            raw_pem = f.read()
+        try:
+            pk = serialization.load_pem_private_key(
+                    raw_pem,
+                    password=passwd,
+                    backend=default_backend())
+        # Unfortunately, the crypto library raises unhelpful exceptions,
+        # so we have to look at the text.
+        except TypeError as e:
+            msg = str(e)
+            if "private key is encrypted" in msg:
+                return None
+            raise e
+        except ValueError:
+            # This seems to happen if the key is a public key, let's try
+            # loading it as a public key.
+            pk = serialization.load_pem_public_key(
+                raw_pem, backend=default_backend())
+    else:
+        pk = key
 
     if isinstance(pk, RSAPrivateKey):
         if pk.key_size not in RSA_KEY_SIZES:
             raise Exception("Unsupported RSA key size: " + pk.key_size)
         return RSA(pk)
     elif isinstance(pk, RSAPublicKey):
         if pk.key_size not in RSA_KEY_SIZES:
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ecdsa.py` & `cysecuretools-5.0.0/src/execute/imgtool/keys/ecdsa.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ecdsa_test.py` & `cysecuretools-5.0.0/src/execute/imgtool/keys/ecdsa_test.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ed25519.py` & `cysecuretools-5.0.0/src/execute/imgtool/keys/ed25519.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/ed25519_test.py` & `cysecuretools-5.0.0/src/execute/imgtool/keys/ed25519_test.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/general.py` & `cysecuretools-5.0.0/src/execute/imgtool/keys/general.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/rsa.py` & `cysecuretools-5.0.0/src/execute/imgtool/keys/rsa.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from cryptography.hazmat.primitives.asymmetric.padding import PSS, MGF1
 from cryptography.hazmat.primitives.hashes import SHA256
 
 from .general import KeyClass
 
 
 # Sizes that bootutil will recognize
-RSA_KEY_SIZES = [2048, 3072]
+RSA_KEY_SIZES = [2048, 3072, 4096]
 
 
 class RSAUsageError(Exception):
     pass
 
 
 class RSAPublic(KeyClass):
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/rsa_test.py` & `cysecuretools-5.0.0/src/execute/imgtool/keys/rsa_test.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/keys/x25519.py` & `cysecuretools-5.0.0/src/execute/imgtool/keys/x25519.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/main.py` & `cysecuretools-5.0.0/src/execute/imgtool/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,15 @@
                custom_tlvs, use_random_iv=use_random_iv, encryptor=encryptor)
     img.save(outfile, hex_addr)
 
 
 def parse_tlvs(custom_tlv, allow_predefined=False):
     custom_tlvs = {}
     for tlv in custom_tlv:
-        tag = int(tlv[0], 0)
+        tag = int(str(tlv[0]), 0)
         if tag in custom_tlvs:
             raise click.UsageError('Custom TLV %s already exists.' % hex(tag))
         if not allow_predefined and tag in image.TLV_VALUES.values():
             raise click.UsageError(
                 'Custom TLV %s conflicts with predefined TLV.' % hex(tag))
 
         value = tlv[1]
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/imgtool/version.py` & `cysecuretools-5.0.0/src/execute/imgtool/version.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/key_reader.py` & `cysecuretools-5.0.0/src/execute/key_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,35 +12,23 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import json
 import logging
+
 from jose import jwk, exceptions
 from jose.constants import ALGORITHMS
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 
-import cysecuretools.execute.keygen as keygen
-from cysecuretools.execute.provisioning_packet.lib.cyprov_pem import PemKey
-
 logger = logging.getLogger(__name__)
 
 
-def jwk_to_pem(json_key, private_key=False):
-    pem = PemKey(json_key)
-    pem_key = pem.to_str(private_key)
-    return pem_key
-
-
-def get_aes_key(key_size, fmt):
-    return keygen.generate_aes_key(key_size=key_size, fmt=fmt).private
-
-
 def load_key(key):
     """
     Load JWK for certificate signing.
     :param key: File that contains the key.
     :return: Tuple - private key, public key
     """
     priv_key = None
@@ -92,21 +81,21 @@
         for item in key_json:
             if 'pub_key' in item:
                 pub_key = key_json[item]
                 break
 
         # Input file does not contain JWK
         if not priv_key:
-            ValueError(f'Private key not found in {key}')
+            raise ValueError(f'Private key not found in {key}')
         if not pub_key:
             if priv_key:
                 pub_key = priv_key
                 del pub_key["d"]
             else:
-                ValueError(f'Public key not found in {key}')
+                raise ValueError(f'Public key not found in {key}')
 
     return priv_key, pub_key
 
 
 def is_private_key(path):
     with open(path, 'rb') as f:
         raw_pem = f.read()
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/key_reader_mxs40v1.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/key_reader_mxs40v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,17 +12,18 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import json
 import logging
-from cysecuretools.execute.key_reader import jwk_to_pem
-from cysecuretools.execute.provisioning_packet.lib.cyprov_crypto import Crypto
-from cysecuretools.execute.sys_call import get_prov_details
+
+from .provisioning.sys_call import get_prov_details
+from ....core.key_helper import jwk_to_pem
+from ....execute import jwt
 
 logger = logging.getLogger(__name__)
 
 
 class KeyReaderMXS40V1:
     def __init__(self, target):
         self.target = target
@@ -45,10 +47,10 @@
             return None
 
     def get_cypress_public_key(self):
         """
         Gets Cypress public key from cy_auth JWT packet.
         :return: Cypress public key (JWK).
         """
-        jwt_text = Crypto.read_jwt(self.policy_parser.get_cy_auth())
-        json_data = Crypto.readable_jwt(jwt_text)
+        jwt_text = jwt.read_jwt(self.policy_parser.get_cy_auth())
+        json_data = jwt.readable_jwt(jwt_text)
         return json_data["payload"]['cy_pub_key']
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/key_source/key_source_mxs40sv2.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/key_source_mxs40sv2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
-Copyright (c) 2020 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
-from cysecuretools.core import KeyData
-from cysecuretools.core.enums import KeyType, KeyAlgorithm
+
+from ....core.enums import KeyPair, KeyAlgorithm
 
 
 class KeySourceMXS40Sv2:
 
     def __init__(self, policy_parser):
         self.policy_parser = policy_parser
 
@@ -41,29 +42,25 @@
             if key_path:
                 aes_key_path = key_path
             else:
                 aes_key_path = self.get_aes_key()
             if aes_key_path is None:
                 raise KeyError('The encryption key is not specified')
 
-            keys.append(KeyData(key_type=KeyType.user,
-                                pem_key=os.path.abspath(aes_key_path)))
+            keys.append(KeyPair(os.path.abspath(aes_key_path), None))
         else:
             if key_id is None and not key_path:
                 raise KeyError('Either key ID or key path must be specified')
             if key_path:
                 if isinstance(key_path, str):
-                    keys.append(KeyData(key_type=KeyType.user,
-                                        pem_key_pub=os.path.abspath(key_path)))
+                    keys.append(KeyPair(None, os.path.abspath(key_path)))
                 elif isinstance(key_path, (tuple, list)):
                     for pair in key_path:
-                        keys.append(KeyData(
-                            key_type=KeyType.user,
-                            pem_key=os.path.abspath(pair[0]),
-                            pem_key_pub=os.path.abspath(pair[1])))
+                        keys.append(KeyPair(os.path.abspath(pair[0]),
+                                            os.path.abspath(pair[1])))
                 else:
                     raise TypeError("Expected types are 'str' or 'tuple'")
             else:
                 if key_id == 0:
                     pub_key = self.policy_parser.get_pub_key_0_path()
                     priv_key = self.policy_parser.get_priv_key_0_path()
                 elif key_id == 1:
@@ -75,17 +72,16 @@
                 if pub_key is None:
                     raise KeyError(f'OEM public key {key_id} not specified '
                                    f'({self.policy_parser.policy_file})')
                 if priv_key is None:
                     raise KeyError(f'OEM private key {key_id} not specified '
                                    f'({self.policy_parser.policy_file})')
 
-                keys.append(KeyData(key_type=KeyType.user, key_id=key_id,
-                                    pem_key=os.path.abspath(priv_key),
-                                    pem_key_pub=os.path.abspath(pub_key)))
+                keys.append(KeyPair(os.path.abspath(priv_key),
+                                    os.path.abspath(pub_key)))
 
         return keys
 
     def get_key(self, key_id, key_type):
         """
         Gets a key based on specified ID and type
         :param key_id: The ID of the key in the policy.
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/key_source/key_source_mxs40v1.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/key_source_mxs40v1.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/programmer/__init__.py` & `cysecuretools-5.0.0/src/targets/common/traveo_t2g/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
-Copyright (c) 2019 Cypress Semiconductor Corporation
+Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from . import base
-from . import programmer
-from . import pyocd_wrapper
+from .signtool_xmc7xxx import SignToolXMC7xxx
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/programmer/openocd_server.py` & `cysecuretools-5.0.0/src/execute/programmer/openocd_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,21 +18,18 @@
 import logging
 import enum
 import platform
 import time
 import atexit
 import subprocess
 from pathlib import Path
+from collections import namedtuple
 
-from cysecuretools.core.logging_configurator import LoggingConfigurator
-from cysecuretools.core.ocd_settings import OcdSettings
-
-
-OPENOCD_DEFAULT_PATH = os.path.join(os.path.dirname(__file__), os.pardir,
-                                    os.pardir, os.pardir, 'openocd')
+from ...core.logging_configurator import LoggingConfigurator
+from ...core.ocd_settings import OcdSettings
 
 logger = logging.getLogger(__name__)
 
 
 class OcdTransport(enum.Enum):
     """ Enum with supported transport protocols in OpenOCD """
     SWD = 'swd'
@@ -42,19 +39,23 @@
 class OcdProbeInterface(enum.Enum):
     """ Enum with supported debug probes in OpenOCD """
     KITPROG3 = 'kitprog3'
     CMSIS_DAP = 'cmsis-dap'
 
 
 class OcdAcquire(enum.IntEnum):
-    """ Enum with possible Aquire options in OpenOCD """
+    """ Enum with possible Acquire options in OpenOCD """
     ENABLE = 1
     DISABLE = 0
 
 
+OcdCustomConfig = namedtuple(
+    'OcdCustomConfig', 'variables interface before_init after_init')
+
+
 class OcdConfig:
     """
         This is a class which contains configuration settings for OpenOCD.
 
         See OpenOCD documentation for details:
         http://openocd.org/doc/pdf/openocd.pdf
     """
@@ -136,28 +137,31 @@
         if interface:
             raise NotImplementedError
 
         super().__init__()
         self.inited = True
         self.server_proc = None  # TCL RPC server process
         self.openocd_cmd = ''    # command for OpenOCD configuration
-        self.before_init, self.after_init = self._get_ocd_config(target)
+
+        self.custom_config = self._ocd_custom_config(target)
         self.power = power
         self.voltage = voltage
         self.ignore_errors = ignore_errors
+        if self.custom_config['interface']:
+            self.probe_interface = self.custom_config['interface']
 
         os_name = platform.system()  # current OS type
         # Set OpenOCD execution filename
-        if os_name in self._supported_os_short_names.keys():
+        if os_name in self._supported_os_short_names:
             self._os_short_name = self._supported_os_short_names[os_name]
         else:
             self.inited = False
             raise ValueError(f'Unsupported OS platform: {os_name}')
 
-        # Set OpenOCD executabe filename
+        # Set OpenOCD executable filename
         if self._os_short_name == 'win':
             self.openocd_exec_file = 'openocd.exe'
         else:
             self.openocd_exec_file = 'openocd'
 
         # Get OpenOCD directory path
         if tool_path is None:
@@ -175,24 +179,33 @@
         # Update Flash restriction size to be able to program Secure Bootloader
         self.flash_restriction_size = target.memory_map.FLASH_SIZE
 
         # Only SWD interface supported by now
         self.transport_select = OcdTransport.SWD.value
 
     @staticmethod
-    def _get_ocd_config(target):
+    def _ocd_custom_config(target):
+        try:
+            variables = target.ocd_config['openocd']['variables']
+        except KeyError:
+            variables = ''
+        try:
+            interface = target.ocd_config['openocd']['interface']
+        except KeyError:
+            interface = ''
         try:
             before_init = target.ocd_config['openocd']['before_init']
         except KeyError:
             before_init = ''
         try:
             after_init = target.ocd_config['openocd']['after_init']
         except KeyError:
             after_init = ''
-        return before_init, after_init
+        return {'variables': variables, 'interface': interface,
+                'before_init': before_init, 'after_init': after_init}
 
     def _prepare_command(self, ap='sysap', acquire=None):
         """
         This command configure the local OpenOCD server.
         :return: None
         """
         openocd_exec_file = os.path.abspath(os.path.join(
@@ -221,32 +234,34 @@
 
         openocd_config_cmd = []
         if self.flash_restriction_size is not None:
             openocd_config_cmd += [f'set FLASH_RESTRICTION_SIZE {self.flash_restriction_size}']
 
         if self.power:
             volt = '' if self.power == 'off' else self.voltage
-            self.before_init += f'kitprog3 power_config {self.power} {volt}'
+            self.custom_config[
+                'before_init'] += f'kitprog3 power_config {self.power} {volt}'
 
         openocd_config_cmd += [
             f'debug_level {self.debug_level}',
             f'set ENABLE_ACQUIRE {enable_acquire}',
             f'set ENABLE_POWER_SUPPLY {self.enable_power_supply}',
             'set ACQUIRE_TIMEOUT 5000',
+            self.custom_config['variables'],
             ap_config,
             'gdb_memory_map enable',
             'gdb_flash_program enable',
             f'source [find interface/{self.probe_interface}.cfg]',
             f'{set_probe_id_command}',
             f'transport select {self.transport_select}',
             f'source [find target/{self.target_device_name}.cfg]',
             f'adapter speed {self.adapter_speed_khz}',
-            self.before_init,
+            self.custom_config['before_init'],
             'init',
-            self.after_init
+            self.custom_config['after_init']
         ]
 
         # Remove empty elements from list
         openocd_config_cmd = list(filter(None, openocd_config_cmd))
         # Insert a command '-c' before each element in list
         openocd_config_cmd = \
             [cmd for elem in openocd_config_cmd for cmd in ('-c', elem)]
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/programmer/openocd_wrapper.py` & `cysecuretools-5.0.0/src/execute/programmer/openocd_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 import os
 import re
 import sys
 import json
 import socket
 import signal
 import logging
-from cysecuretools.execute.programmer.base import ProgrammerBase, ResetType, AP
-from cysecuretools.core.target_director import TargetDirector
-from cysecuretools.execute.programmer.openocd_server import OpenocdServer
+
+from .openocd_server import OpenocdServer
+from .base import ProgrammerBase, ResetType, AP
+from ...core.target_director import TargetDirector
 
 TARGET_MAP = os.path.join(os.path.dirname(__file__), 'openocd_target_map.json')
 logger = logging.getLogger(__name__)
 
 
 class Openocd(ProgrammerBase):
-    """
-    OpenOCD wrapper for client side
-    """
+    """OpenOCD wrapper for client side"""
 
     _CMD_SUCCESS = 0
     _CMD_FAIL = -1
 
-    def __init__(self, name, path=None):
-        super(Openocd, self).__init__(name, path)
+    def __init__(self, name, settings):
+        path = settings.ocd_path if settings else None
+        super().__init__(name, path=path)
         self.sock = None
         self.target = None
         self.ocd_server = None
         self.verbose = False
         self.tcp_host_address = '127.0.0.1'
         self.tcp_host_port = 6666
         self.sock_buffer_size = 4096
@@ -59,43 +59,34 @@
             'Error',
             'error writing',
             'invalid command name',
         ]
         self.current_ap = AP.SYS  # currently selected by user access port
         self.connect_ap = AP.SYS  # access port selected before init
         self.mcu = None
-
-    @property
-    def wait_for_target(self):
-        """
-        N/A for OpenOCD
-        """
-
-    @wait_for_target.setter
-    def wait_for_target(self, value):
-        """
-        N/A for OpenOCD
-        """
+        self.cm0_name = None
+        self.cm4_name = None
+        self.cm33_name = None
+        self.cm55_name = None
+        self.sysap_name = None
 
     def connect(self, target_name=None, interface=None, probe_id=None,
-                ap='sysap', acquire=None, blocking=None, power=None,
-                voltage=None, ignore_errors=False):
+                ap='sysap', acquire=None, power=None, voltage=None,
+                ignore_errors=False):
         """
         Connects to target using default debug interface.
         @param target_name: The target name.
         @param interface: Debug interface.
         @param probe_id: Probe serial number.
         @param ap: The access port to be used for flash operations
         @param acquire: Indicates whether to acquire device on connect
-        @param blocking: Specifies whether to wait for a probe to be
-               connected if there are no available probes.
         @param power: Indicates whether to on/off the KitProg3 power
         @param voltage: The KitProg3 voltage level
         @param ignore_errors: Ignore errors and continue execution
-        @return: True if connected successfully, otherwise False.
+        @return: True if connected successfully, otherwise False
         """
         if interface:
             raise NotImplementedError
 
         if target_name:
             ocd_target_name = ''
             # Search for device in target map
@@ -103,23 +94,28 @@
                 file_content = f.read()
                 json_data = json.loads(file_content)
             for json_target in json_data:
                 if target_name.lower().strip() == json_target.lower().strip():
                     # Get target info
                     director = TargetDirector()
                     try:
-                        from cysecuretools.targets import target_data
+                        from ...targets import target_data
                         director.builder = target_data(target_name)['class']()
                     except KeyError as e:
                         raise ValueError(
                             f'Unknown target "{target_name}"') from e
                     self.target = director.get_target(None, target_name, None)
                     # Get target name which is relevant to OpenOCD
                     ocd_target_name = json_data[json_target]['target']
-                    self.mcu = json_data[json_target]['mcu']
+                    self.mcu = json_data[json_target].get('mcu')
+                    self.cm0_name = json_data[json_target].get('cm0')
+                    self.cm4_name = json_data[json_target].get('cm4')
+                    self.cm33_name = json_data[json_target].get('cm33')
+                    self.cm55_name = json_data[json_target].get('cm55')
+                    self.sysap_name = json_data[json_target].get('sysap')
                     break
         else:
             raise ValueError("Parameter 'target_name' is None")
 
         if ap == 'cm4':
             self.connect_ap = AP.CM4
         elif ap == 'cm0':
@@ -158,261 +154,243 @@
                 raise ValueError('Debug session has already initialized')
         else:
             return False
 
         return True
 
     def disconnect(self):
-        """
-        Closes active connection.
-        """
+        """Closes active connection"""
         self.halt()  # halted core before disconnecting from it
         if self.sock is None:
             raise ValueError('Debug session is not initialized')
         self.sock.close()
         self.sock = None
         self.ocd_server.stop()
 
     def set_frequency(self, value_khz):
-        """
-        Sets probe frequency.
-        @param value_khz: Frequency in kHz.
+        """Sets probe frequency
+        @param value_khz: Frequency in kHz
         """
         if self.sock is None:
             raise ValueError('Debug probe is not initialized')
         self._send('adapter_khz {0}'.format(value_khz))
 
     def halt(self):
-        """
-        Halts the target.
-        """
+        """Halts the core"""
         if self.sock is None:
             raise ValueError('Debug session is not initialized')
         logger.debug('halt')
         self._send('halt')
 
     def resume(self):
-        """
-        Resumes the execution
-        """
+        """Resumes the execution"""
         if self.sock is None:
             raise ValueError('Target is not initialized')
         logger.debug('resume')
         self._send('resume')
 
     def reset(self, reset_type=ResetType.SW):
-        """
-        Resets the target.
-        @param reset_type: The reset type.
+        """Resets the target
+        @param reset_type: The reset type
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         logger.debug('reset')
+        if reset_type == ResetType.SW:
+            self._send('reset_config srst_only')
+        elif reset_type == ResetType.HW:
+            self._send('reset_config trst_only')
+        elif reset_type == ResetType.HW_SW:
+            self._send('reset_config trst_and_srst')
         self._send('reset run')
 
     def reset_and_halt(self, reset_type=ResetType.SW):
-        """
-        Resets the target and halts the CPU immediately after reset.
-        @param reset_type: The reset type.
+        """Resets the target and halts the CPU immediately after reset
+        @param reset_type: The reset type
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         logger.debug('reset_and_halt')
         self._send('reset init')
 
     def read8(self, address):
-        """
-        Reads 8-bit value from specified memory location.
-        @param address: The memory address to read.
-        @return: The read value.
+        """Reads 8-bit value from specified memory location
+        @param address: The memory address to read
+        @return: The read value
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         cmd_rsp = self._send('mdb 0x{0:x}'.format(address))
         value = self._parse_and_convert_read(cmd_rsp)
         logger.debug('read8 (0x%x): 0x%x', address, value)
         return value
 
     def read16(self, address):
-        """
-        Reads 16-bit value from specified memory location.
-        @param address: The memory address to read.
-        @return: The read value.
+        """Reads 16-bit value from specified memory location.
+        @param address: The memory address to read
+        @return: The read value
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         if (address & 0x01) == 0:
             cmd_rsp = self._send('mdh 0x{0:x}'.format(address))
             value = self._parse_and_convert_read(cmd_rsp)
             logger.debug('read16 (0x%x): 0x%x', address, value)
             return value
-        else:
-            raise ValueError('Address not aligned')
+        raise ValueError('Address not aligned')
 
     def read32(self, address):
-        """
-        Reads 32-bit value from specified memory location.
-        @param address: The memory address to read.
-        @return: The read value.
+        """Reads 32-bit value from specified memory location
+        @param address: The memory address to read
+        @return: The read value
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         if (address & 0x03) == 0:
             cmd_rsp = self._send('mdw 0x{0:x}'.format(address))
             value = self._parse_and_convert_read(cmd_rsp)
             logger.debug('read32 (0x%x): 0x%x', address, value)
             return value
-        else:
-            raise ValueError('Address not aligned')
+        raise ValueError('Address not aligned')
 
     def write8(self, address, value):
-        """
-        Writes 8-bit value by specified memory location.
-        @param address: The memory address to write.
-        @param value: The 8-bit value to write.
+        """Writes 8-bit value by specified memory location
+        @param address: The memory address to write
+        @param value: The 8-bit value to write
         """
         if self.sock is None:
             raise ValueError('Target is not initialized.')
         logger.debug('write8 (0x%x): 0x%x', address, value)
         data = self._send('mwb 0x{0:x} 0x{1:x}'.format(address, value))
         return data
 
     def write16(self, address, value):
-        """
-        Writes 16-bit value by specified memory location.
-        @param address: The memory address to write.
-        @param value: The 16-bit value to write.
+        """Writes 16-bit value by specified memory location
+        @param address: The memory address to write
+        @param value: The 16-bit value to write
         """
         if self.sock is None:
             raise ValueError('Target is not initialized')
         logger.debug('write16 (0x%x): 0x%x', address, value)
         data = self._send('mwh 0x{0:x} 0x{1:x}'.format(address, value))
         return data
 
     def write32(self, address, value):
-        """
-        Writes 32-bit value by specified memory location.
-        @param address: The memory address to write.
-        @param value: The 32-bit value to write.
+        """Writes 32-bit value by specified memory location
+        @param address: The memory address to write
+        @param value: The 32-bit value to write
         """
         self._send('targets')
         if self.sock is None:
             raise ValueError('Target is not initialized')
         logger.debug('write32 (0x%x): 0x%x', address, value)
         data = self._send('mww 0x{0:x} 0x{1:x}'.format(address, value))
         return data
 
     def read_reg(self, reg_name):
-        """
-        Gets value of a core register.
-        @param reg_name: Core register name.
-        @return: The register value.
+        """Gets value of a core register
+        @param reg_name: Core register name
+        @return: The register value
         """
         reg = reg_name.lower()
         value = self._send('reg {0}'.format(reg))
         logger.debug('read_reg (%s): 0x%x', reg, value)
         return value
 
     def write_reg(self, reg_name, value):
-        """
-        Sets value of a core register.
-        @param reg_name: Core register name.
-        @param value: The value to set.
-        @return: The register value.
+        """Sets value of a core register
+        @param reg_name: Core register name
+        @param value: The value to set
+        @return: The register value
         """
         reg = reg_name.lower()
         logger.debug('write_reg (%s): 0x%x', reg, value)
         self._send('reg {0} {1:#x}'.format(reg, value))
 
     def erase(self, address, size):
-        """
-        Erases entire device flash or specified sectors.
-        @param address: The memory location.
-        @param size: The memory size.
+        """Erases entire device flash or specified sectors
+        @param address: The memory location
+        @param size: The memory size
         """
         if self.sock is None:
             raise ValueError('Debug session is not initialized')
         self.halt()
         logger.debug('erase 0x%x-0x%x', address, address + size)
         self._send('flash erase_address {0} {1}'.format(address, size))
 
-    def program(self, filename, file_format=None, address=None):
-        """
-        Programs a file into flash.
-        @param filename: Path to a file.
-        @param file_format: N/A for OpenOCD.
+    def program(self, filename, file_format=None, address=None, **kwargs):
+        """Programs a file into flash
+        @param filename: Path to a file
+        @param file_format: N/A for OpenOCD
         @param address: Base address used for the address where to
-               flash a binary.
-        @return: True if programmed successfully, otherwise False.
+               flash a binary
+        @return: True if programmed successfully, otherwise False
         """
         if self.sock is None:
             raise ValueError('Debug session is not initialized')
         # Remove Windows-style path separator
         filename = filename.replace(os.sep, '/')
         self.halt()
         if address:
             logger.debug("Programming '%s' to %s", filename, address)
             self._send(f'flash write_image erase "{filename}" {address}')
         else:
             logger.debug("Programming '%s'", filename)
             self._send(f'flash write_image erase "{filename}"')
 
-    def program_ram(self, filename, file_format=None, address=None):
-        """
-        Programs a file into flash.
-        @param filename: Path to a file.
-        @param file_format: N/A for OpenOCD.
+    def program_ram(self, filename, _file_format=None, address=None):
+        """Programs a file into flash
+        @param filename: Path to a file
+        @param _file_format: N/A for OpenOCD
         @param address: Base address used for the address where to
-               flash a binary.
-        @return: True if programmed successfully, otherwise False.
+               flash a binary
+        @return: True if programmed successfully, otherwise False
         """
         if self.sock is None:
             raise ValueError('Debug session is not initialized')
         # Remove Windows-style path separator
         filename = filename.replace(os.sep, '/')
         self.halt()
         if address:
             logger.debug("Programming '%s' to %s", filename, address)
             self._send(f'load_image "{filename}" {address}')
         else:
             logger.debug("Programming '%s'", filename)
             self._send(f'load_image "{filename}"')
 
     def _parse_read(self, cmd_response):
-        """
-        Parse OpenOCD output from read memory commands
+        """Parse OpenOCD output from read memory commands
         @param cmd_response: String with response from server to the
                read command
         @return: The register as integer value
         """
         for err_msg in self._error_msg_patterns:
             if err_msg in cmd_response:
                 logger.error("Unable to get data from the memory")
                 return self._CMD_FAIL
         cmd_result = cmd_response.split(':')
         value = cmd_result[1].strip()
         return value
 
     def _parse_and_convert_read(self, cmd_response):
-        """
-        Parse OpenOCD output from read memory commands
+        """Parse OpenOCD output from read memory commands
         @param cmd_response: String with response from server to the
                read command
         @return: The register as integer value
         """
         value = self._parse_read(cmd_response)
         value = int(value, 16)
         return value
 
     def _send(self, cmd):
-        """
-        Send a command to TCL RPC.
-        Note: This command also check command status and if it is not SUCCESS raise ValueError exception
-        @param cmd: String with command for OpenOCD server.
-        @return: String with response on sent command to the server.
+        """Send a command to TCL RPC
+        Note: This command also check command status and if it is not
+        SUCCESS raise ValueError exception
+        @param cmd: String with command for OpenOCD server
+        @return: String with response on sent command to the server
         """
         if self.sock is None:
             raise ValueError('Debug session is not initialized')
             # Stop OpenOCD server if termination signal was received
 
         if self.verbose:
             logger.info('send -> %s', cmd)
@@ -434,27 +412,25 @@
                                                                   os.linesep))
         cmd_message = cmd_message.rstrip()
         if cmd_message:
             logger.debug(cmd_message)
         return cmd_message
 
     def _send_cmd(self, cmd):
-        """
-        Send a command string to TCL RPC.
-        @param cmd: String with command for OpenOCD server.
-        @return: String with response on sent command.
+        """Send a command string to TCL RPC
+        @param cmd: String with command for OpenOCD server
+        @return: String with response on sent command
         """
         data = (cmd + self._command_token).encode("utf-8")
         self.sock.send(data)
         return self._receive()
 
     def _receive(self):
-        """
-        Read from the stream until the token (\x1a) was received.
-        @return: String with response on sent command to the server.
+        """Read from the stream until the token (\x1a) was received
+        @return: String with response on sent command to the server
         """
         data = bytes()
         while True:
             chunk = self.sock.recv(self.sock_buffer_size)
             data += chunk
             if bytes(self._command_token, encoding="utf-8") in chunk:
                 break
@@ -472,54 +448,44 @@
             logger.info('The termination signal from the system was received')
         if self.sock is not None:
             self.sock.close()
         self.ocd_server.stop()
         sys.exit(0)
 
     def get_ap(self):
-        """
-        Gets access port.
-        @return: Selected AP.
+        """Gets access port
+        @return: Selected AP
         """
         logger.debug('AP: %s', self.current_ap)
         return self.current_ap
 
-    def set_ap(self, ap):
-        """
-        Sets access port.
-        @param ap: The AP name.
+    def set_ap(self, ap: AP):
+        """Sets access port
+        @param ap: Access port
         """
         if ap == AP.CM0:
-            logger.debug('Use cm0 AP')
-            self._send(f'targets {self.mcu}.cm0')
+            self._send(f'targets {self.mcu}.{self.cm0_name}')
         elif ap == AP.CM4:
-            logger.debug('Use cm4 AP')
-            self._send(f'targets {self.mcu}.cm4')
+            self._send(f'targets {self.mcu}.{self.cm4_name}')
         elif ap == AP.CMx:
             if self.connect_ap == AP.CM0:
-                logger.debug('Use cm0 AP')
-                self._send(f'targets {self.mcu}.cm0')
+                self._send(f'targets {self.mcu}.{self.cm0_name}')
             elif self.connect_ap == AP.CM4:
-                logger.debug('Use cm4 AP')
-                self._send(f'targets {self.mcu}.cm4')
+                self._send(f'targets {self.mcu}.{self.cm4_name}')
             elif self.connect_ap == AP.CM33:
-                logger.debug('Use system CM33 AP')
-                self._send(f'targets {self.mcu}.cm33ap')
+                self._send(f'targets {self.mcu}.{self.cm33_name}')
         elif ap == AP.CM33:
-            logger.debug('Use system CM33 AP')
-            self._send(f'targets {self.mcu}.cm33ap')
+            self._send(f'targets {self.mcu}.{self.cm33_name}')
         elif ap == AP.SYS:
-            logger.debug('Use system AP')
-            self._send(f'targets {self.mcu}.sysap')
+            self._send(f'targets {self.mcu}.{self.sysap_name}')
         self._send('targets')
         self.current_ap = ap
 
     def read(self, address, length):
-        """
-        Reads a block of unaligned bytes in memory
+        """Reads a block of unaligned bytes in memory
         @param address: The memory address where start reading
         @param length: Number of bytes to read
         @return: An array of byte values
         """
         def read_memory(addr, size):
             cmd = 'read_memory 0x{0:x} 8 {1}'.format(addr, size)
             logger.debug(cmd)
@@ -542,16 +508,15 @@
                 read_address += read_size
         else:
             data = read_memory(address, length)
 
         return data
 
     def write(self, address, data):
-        """
-        Write a block of unaligned bytes in memory
+        """Write a block of unaligned bytes in memory
         @param address: The memory address where start writing
         @param data: An array of byte values
         """
         if self.sock is None:
             raise ValueError('Target is not initialized.')
 
         if isinstance(data, list) and all(isinstance(i, int) for i in data):
@@ -562,37 +527,28 @@
         else:
             raise ValueError('Either int array or bytes is supported')
 
         cmd = 'write_memory 0x{0:x} 8 {{{1}}}'.format(address, value)
         logger.debug(cmd)
         self._send(cmd)
 
-    @staticmethod
-    def get_probe_list():
-        """
-        Not implemented in OpenOCD.
-        """
+    def get_probe_list(self):
+        """Not implemented in OpenOCD"""
         raise NotImplementedError
 
-    def set_skip_reset_and_halt(self, value):
-        """
-        N/A for OpenOCD
-        """
-
     def examine_ap(self):
-        """
-        Examines CMx (depending on selected ap for connection) AP
+        """Examines CMx (depending on selected ap for connection) AP
         without reset
         """
         if self.connect_ap == AP.CM0:
-            ap = 'cm0'
+            ap = self.cm0_name
         elif self.connect_ap == AP.CM4:
-            ap = 'cm4'
+            ap = self.cm4_name
         elif self.connect_ap == AP.SYS:
-            ap = 'sysap'
+            ap = self.sysap_name
 
         self._send(f'{self.mcu}.{ap} arp_examine')
 
     def get_voltage(self):
         """Reads target voltage
         @return Voltage value in Volts
         """
@@ -608,7 +564,24 @@
                 logger.debug('VTarget = %s', voltage)
             else:
                 voltage = None
                 logger.warning('VTarget is unknown')
         else:
             raise NotImplementedError
         return voltage
+
+    def dump_image(self, filename, addr, size):
+        """Dumps memory region to the file
+        @param filename: Filename where to save the dump
+        @param addr: Region address
+        @param size: Region size
+        @return: True if programmed successfully, otherwise False
+        """
+        if self.sock is None:
+            raise ValueError('Debug session is not initialized')
+        # Remove Windows-style path separator
+        filename = filename.replace(os.sep, '/')
+        logger.debug("Load data to file '%s'", filename)
+        self._send(f'dump_image {filename} {addr} {size}')
+
+    def verify(self, filename, address, **kwargs):
+        """N/A to OpenOCD"""
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/programmer/programmer.py` & `cysecuretools-5.0.0/src/execute/programmer/programmer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 """
-Copyright (c) 2019 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.execute.programmer.pyocd_wrapper import Pyocd
-from cysecuretools.execute.programmer.openocd_wrapper import Openocd
+from .base import ProgrammerBase
+from .openocd_wrapper import Openocd
+from .dfuht_wrapper import Dfuht
+from ...core import OcdSettings
 
 tools = {
-    'pyocd': Pyocd,
-    'openocd': Openocd
+    'openocd': Openocd,
+    'serial': Dfuht
 }
 
 
 class ProgrammingTool:
+    """Implements a factory method for creating OCD wrapper objects
+    without specifying their concrete classes
+    """
+
     @staticmethod
-    def create(name, path=None):
+    def create(name, settings: OcdSettings = None) -> ProgrammerBase:
         """ Creates an instance of the on-chip debugger wrapper """
         tool_type = tools[name]
-        tool = tool_type(name, path)
+        tool = tool_type(name, settings)
         return tool
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/project_init/project_init_mxs40sv2.py` & `cysecuretools-5.0.0/src/execute/project_init/project_init.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,187 +13,223 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import logging
 import importlib
-from pathlib import Path
-from cysecuretools.core.project import ProjectInitializer
-from cysecuretools.targets.common.mxs40sv2.flow_parser import FlowParser
 
-logger = logging.getLogger(__name__)
+from ...core.project_base import ProjectInitializerBase
+from ...targets.common.flow_parser import FlowParser
 
-project_files = {
-    'packets': {
-        'templates': [
-            'debug_cert.json',
-            'rsa_key_tmpl.json',
-        ]
-    }
-}
+logger = logging.getLogger(__name__)
 
 
-class ProjectInitializerMXS40Sv2(ProjectInitializer):
+class ProjectInitializer(ProjectInitializerBase):
     """
-    A class that implements project creation logic for
-    MXS40Sv2 platform
+    A class that implements project creation logic
     """
 
     def __init__(self, target):
         super().__init__(target)
-        self.packets_src = os.path.join(self.target_dir, self.packets_dir_name)
-        self.apps_src = os.path.join(self.target_dir, self.packets_dir_name)
-        self.keys_src = os.path.join(self.target_dir, self.keys_dir_name)
+        self.test_pkg_type = None
+        self.apps_paths = {}
+
+        self.packets_src = os.path.join(self.target_dir, self.packets_dirname)
+        self.packets_dst = os.path.join(self.cwd, os.path.basename(
+            os.path.normpath(self.packets_src)))
+        self.apps_src = os.path.join(self.target_dir, self.packets_dirname)
+        self.keys_src = os.path.join(self.target_dir, self.keys_dirname)
+
         self.flow_parser = FlowParser(self.target)
+        self.test_packages = target.test_packages
+
+    @property
+    def policy_dir(self):
+        """
+        Returns path to policy directory
+        """
         if self.policy_parser.policy_dir is None:
             if self.is_project():
-                self.policy_dir = os.path.join(self.cwd, self.policy_dir_name)
+                policy_dir = os.path.join(self.cwd, self.policy_dirname)
             else:
-                self.policy_dir = os.path.join(target.target_dir, self.policy_dir_name)
+                policy_dir = os.path.join(self.target.target_dir,
+                                          self.policy_dirname)
         else:
-            self.policy_dir = self.policy_parser.policy_dir
-        self.test_packages = target.test_packages
-        self.test_pkg_type = None
+            policy_dir = self.policy_parser.policy_dir
+        return policy_dir
 
     @property
     def packets_dir(self):
         """ Gets a path to the packets directory in the project """
         return os.path.abspath(os.path.join(
-            self.policy_dir, '..', self.packets_dir_name))
+            self.policy_dir, '..', self.packets_dirname))
 
     @property
     def apps_dir(self):
         """ Gets a path to the apps directory in the project """
-        return os.path.join(self.packets_dir, self.apps_dir_name)
+        return os.path.join(self.packets_dir, self.apps_dirname)
 
     @property
     def pkg_apps_dir(self):
         """ Gets a path to the apps directory in the package """
         return os.path.join(
-            self.target_dir, self.packets_dir_name, self.apps_dir_name)
+            self.target_dir, self.packets_dirname, self.apps_dirname)
 
     @property
     def test_policies_dir(self):
         """ A path to a directory containing test policies """
         if self.test_pkg_type is not None:
             package_data = self.test_packages.get(self.test_pkg_type)
             package_name = package_data['package']
             try:
                 module = importlib.import_module(package_name)
                 if module.__file__ is None:
                     raise ImportError(f"No module named '{package_name}'")
             except ImportError as e:
                 raise ImportError(
                     f'Test applications not found. {e.msg}') from e
-            return module.TEST_POLICY_DIR
+            if os.path.exists(module.TEST_POLICY_DIR):
+                return module.TEST_POLICY_DIR
         return None
 
-    def init(self, cwd=None, overwrite=None, **kwargs):
-        """
-        Initializes new project
-        :param cwd: Current working directory
-        :param overwrite: Indicates whether to overwrite project files
-               if already exist. If the value is None, an interactive prompt
-               will ask whether to overwrite existing files
+    def init(self, cwd, overwrite):
+        """Initializes new project"""
+        raise NotImplementedError
+
+    def create_project(self, overwrite=None):
+        """
+        Creates new project
+        :param overwrite: indicates whether the existing project files have
+                to be overwritten. If the value is None, an interactive prompt
+                will ask whether to overwrite existing files
         """
-        if cwd:
-            self.cwd = cwd
-
-        self.test_pkg_type = kwargs.get('testapps')
-        self.flow_parser.test_pkg_type = self.test_pkg_type
-        apps_paths = self.flow_parser.get_apps_paths()
-
-        packets_dst = os.path.join(self.cwd, os.path.basename(
-            os.path.normpath(self.packets_src)))
-
         if overwrite is None:
-            exist = []
-
-            # Check apps existence
-            for d, f in apps_paths.items():
-                files = self._filenames_from_dir(os.path.dirname(f))
-                app_dst = os.path.join(packets_dst, self.apps_dir_name, d)
-                exist.extend(self.get_existent(app_dst, files))
-
-            # Check templates
-            exist.extend(self.get_existent(
-                packets_dst, project_files['packets']['templates']))
-
-            # Check policies existence
-            policy_dst = os.path.join(self.cwd, self.policy_dir_name)
-            files = self.get_policy_src_files(self.policy_src)
-            exist.extend(self.get_existent(policy_dst, files))
-
-            # Check keys existence
-            keys_dst = os.path.join(self.cwd, self.keys_dir_name)
-            files = self._filenames_from_dir(self.keys_src, 'pem')
-            exist.extend(self.get_existent(keys_dst, files))
-
-            # Create a project
-            if exist:
-                print('%s' % '\n'.join(exist))
-                answer = input(f'{len(exist)} files exist and will be '
-                               f'overwritten. Continue? (y/n): ')
+            if self.existing_files:
+                print('%s' % '\n'.join(self.existing_files))
+                answer = input(f'{len(self.existing_files)} files exist '
+                               f'and will be overwritten. Continue? (y/n): ')
                 if answer.strip() == 'y':
-                    self.create_project(packets_dst)
+                    self.copy_project_files()
                 else:
                     logger.info('Skip project creation')
             else:
-                self.create_project(packets_dst)
+                self.copy_project_files()
         elif overwrite is True:
-            self.create_project(packets_dst)
+            self.copy_project_files()
         else:
             logger.info('Skip project creation')
 
-    def create_project(self, packets_dst):
+    @property
+    def existing_files(self):
+        """ Gets existing files in project directory """
+        return self.existing_apps + self.existing_misc_files \
+            + self.existing_policies + self.existing_keys
+
+    @property
+    def existing_apps(self):
+        """ Gets existing RAM applications in project directory """
+        apps = []
+        app_paths = self.flow_parser.get_apps_paths()
+        for d, f in app_paths.items():
+            files = self._filenames_from_dir(os.path.dirname(f))
+            app_dst = os.path.join(self.packets_dst, self.apps_dirname, d)
+            apps.extend(self.get_existent(app_dst, files))
+        return apps
+
+    @property
+    def existing_keys(self):
+        """ Gets existing keys in project directory """
+        keys_dst = os.path.join(self.cwd, self.keys_dirname)
+        files = self._filenames_from_dir(self.keys_src, 'pem')
+        return self.get_existent(keys_dst, files)
+
+    @property
+    def existing_policies(self):
+        """ Gets existing policies in project directory """
+        policy_dst = os.path.join(self.cwd, self.policy_dirname)
+        files = self.get_policy_src_files(self.policy_src)
+        return self.get_existent(policy_dst, files)
+
+    @property
+    def existing_misc_files(self):
+        """ Gets existing miscellaneous files in project directory """
+        existing = []
+        for file_dir, files in self.misc_files.items():
+            src = os.path.join(self.target_dir, file_dir)
+            dst = os.path.join(self.cwd, os.path.basename(
+                os.path.normpath(src)))
+            existing.extend(self.get_existent(dst, files))
+        return existing
+
+    def copy_project_files(self):
         """
-        Creates project in cwd
-        :param packets_dst: Packets destination directory
+        Copies all files from the package directory to the project directory
         """
         self.copy_apps()
-        Path(os.path.join(self.cwd, 'keys')).mkdir(parents=True, exist_ok=True)
-        self.copy_files(self.packets_src, packets_dst,
-                        project_files['packets']['templates'])
         self.copy_policies()
-        if self.test_pkg_type is not None:
-            self.copy_policies(src=self.test_policies_dir)
         self.copy_keys()
+        self.copy_misc_files()
         self.create_config_file()
 
-    def copy_policies(self, src=None):
+    def copy_policies(self):
         """
         Copies policy files from the package directory to the
         project directory
         """
-        src = self.policy_src if src is None else src
-        dst = os.path.join(self.cwd, self.policy_dir_name)
-        files = self.get_policy_src_files(src)
-        self.copy_files(src, dst, files)
+        if self.test_pkg_type:
+            src = (self.policy_src, self.test_policies_dir)
+        else:
+            src = (self.policy_src, )
+        dst = os.path.join(self.cwd, self.policy_dirname)
+        for policy_src in src:
+            if not policy_src:
+                continue
+            files = self.get_policy_src_files(policy_src)
+            self.copy_files(policy_src, dst, files)
 
     def copy_keys(self):
         """
         Copies key files from the package directory to the
         project directory
         """
         src = self.keys_src
-        dst = os.path.join(self.cwd, self.keys_dir_name)
+        dst = os.path.join(self.cwd, self.keys_dirname)
         files = self._filenames_from_dir(self.keys_src, ext='pem')
         self.copy_files(src, dst, files)
 
     def copy_apps(self):
         """
         Copies ram applications data from the package directory to the
         project directory
         """
         apps_paths = self.flow_parser.get_apps_paths()
         apps_dir_dst = os.path.join(
-            self.cwd, self.packets_dir_name, self.apps_dir_name)
+            self.cwd, self.packets_dirname, self.apps_dirname)
         for app_name, file_name in apps_paths.items():
             dst = os.path.join(apps_dir_dst, app_name)
             src = os.path.dirname(file_name)
             files = self._filenames_from_dir(src)
             self.copy_files(src, dst, files)
 
+    def copy_misc_files(self):
+        """
+        Copies miscellaneous files from the package directory to the
+        project directory
+        """
+        for file_dir, files in self.misc_files.items():
+            src = os.path.join(self.target_dir, file_dir)
+            dst = os.path.join(self.cwd, os.path.basename(
+                os.path.normpath(src)))
+            self.copy_files(src, dst, files)
+
     def create_config_file(self):
         """ Creates project configuration file """
         self.create_config(self.target.default_policy)
+
+    @property
+    def misc_files(self):
+        """
+        Gets miscellaneous project files
+        Must follow target project folder structure
+        """
+        return {}
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/project_init/project_init_mxs40v1.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/project_init_mxs40v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020-2022 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,16 +14,17 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import posixpath
 import json
 import logging
-from cysecuretools.core import jsonpath
-from cysecuretools.core.project import ProjectInitializer
+
+from ....core import jsonpath
+from ....core.project_base import ProjectInitializerBase
 
 logger = logging.getLogger(__name__)
 
 
 # The sufficient list of files to initialize the
 # project. The policy directory is copied entirely
 project_files = {
@@ -39,28 +41,28 @@
         'cy_pub_key.json',
         'hsm_state.json',
         'oem_state.json'
     }
 }
 
 
-class ProjectInitializerMXS40V1(ProjectInitializer):
+class ProjectInitializerMXS40V1(ProjectInitializerBase):
     """Project creation implementation for the MXS40v1 platform"""
 
     def __init__(self, target):
         super().__init__(target)
-        self.common_prebuilt_dir_name = '../common/p64/prebuilt'
+        self.common_prebuilt_dir_name = '../common/mxs40v1/prebuilt'
         self.default_policy_file_name = os.path.basename(os.path.normpath(
             target.policy))
         self.common_keys_src = os.path.abspath(os.path.join(
             self.target_dir, self.common_prebuilt_dir_name))
         self.target_keys_src = os.path.abspath(os.path.join(
-            self.target_dir, self.keys_dir_name))
+            self.target_dir, self.keys_dirname))
         self.prebuilt_src = os.path.join(
-            self.target_dir, self.prebuilt_dir_name)
+            self.target_dir, self.prebuilt_dirname)
 
     @property
     def _packets_src(self):
         packets_dir_name = os.path.basename(os.path.normpath(
             self.policy_parser.get_provisioning_packet_dir()))
         return os.path.join(self.target_dir, packets_dir_name)
 
@@ -72,31 +74,31 @@
                if already exist. If the value is None, an interactive prompt
                will ask whether to overwrite existing files
         """
         if cwd:
             self.cwd = cwd
         exist = []
 
-        keys_dst = os.path.join(self.cwd, self.keys_dir_name)
+        keys_dst = os.path.join(self.cwd, self.keys_dirname)
         packets_dst = os.path.join(self.cwd, os.path.basename(
             os.path.normpath(self._packets_src)))
 
         if overwrite is None:
             # Check packets existence
             exist.extend(self.get_existent(
                 packets_dst, project_files['packets']))
 
             # Check policies existence
-            policy_dst = os.path.join(self.cwd, self.policy_dir_name)
+            policy_dst = os.path.join(self.cwd, self.policy_dirname)
             files = self.get_policy_src_files(self.policy_src)
             exist.extend(self.get_existent(policy_dst, files))
 
             # Check prebuilt existence
             src_files = self.get_prebuilt_files(self.prebuilt_src)
-            prebuilt_dst = os.path.join(self.cwd, self.prebuilt_dir_name)
+            prebuilt_dst = os.path.join(self.cwd, self.prebuilt_dirname)
             dst_files = self.get_prebuilt_files(prebuilt_dst)
             try:
                 for item in dst_files:
                     if item in src_files:
                         exist.extend([os.path.join(prebuilt_dst, item)])
             except FileNotFoundError:
                 pass
@@ -152,25 +154,25 @@
 
     def copy_policies(self):
         """
         Copies policy files from the package directory to the
         project directory
         """
         src = self.policy_src
-        dst = os.path.join(self.cwd, self.policy_dir_name)
+        dst = os.path.join(self.cwd, self.policy_dirname)
         files = self.get_policy_src_files(self.policy_src)
         self.copy_files(src, dst, files)
 
     def copy_prebuilt(self):
         """
         Copies prebuilt files from the package directory to the
         project directory
         """
         src = self.prebuilt_src
-        dst = os.path.join(self.cwd, self.prebuilt_dir_name)
+        dst = os.path.join(self.cwd, self.prebuilt_dirname)
         files = self.get_prebuilt_files(src)
         self.copy_files(src, dst, files)
 
     def create_config_file(self):
         """Creates a project configuration file"""
         rel_path = os.path.relpath(self.target.default_policy, self.target_dir)
         self.create_config(os.path.relpath(rel_path))
@@ -178,15 +180,15 @@
     def update_policies(self):
         """
         Updates paths pointing to the package to the paths
         pointing to the project in policy destination files.
         """
         policy_files = self.get_policy_src_files(self.policy_src)
         for policy in policy_files:
-            policy_path = os.path.join(self.cwd, self.policy_dir_name, policy)
+            policy_path = os.path.join(self.cwd, self.policy_dirname, policy)
             with open(policy_path, encoding='utf-8') as f:
                 json_str = f.read()
                 policy = json.loads(json_str)
 
             self._update_bootloader_keys_section(policy)
             self._update_pre_build_section(policy)
 
@@ -195,16 +197,16 @@
 
     def _update_pre_build_section(self, policy):
         update_nodes = ['oem_public_key', 'oem_private_key', 'hsm_public_key',
                         'hsm_private_key']
         for k, v in policy['pre_build'].items():
             if k in update_nodes:
                 filename = os.path.basename(os.path.normpath(v))
-                new_path = posixpath.join('../', self.keys_dir_name, filename)
+                new_path = posixpath.join('../', self.keys_dirname, filename)
                 policy['pre_build'][k] = new_path
 
     def _update_bootloader_keys_section(self, policy):
         path = 'boot_upgrade.firmware.0.bootloader_keys.0.key'
         old_value = jsonpath.get_node_value(policy, path)
         filename = os.path.basename(os.path.normpath(old_value))
-        new_value = posixpath.join('../', self.keys_dir_name, filename)
+        new_value = posixpath.join('../', self.keys_dirname, filename)
         jsonpath.set_node_value(policy, path, new_value)
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/application_mxs40sv2.py` & `cysecuretools-5.0.0/src/core/provisioning_flows/application.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,47 +12,51 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import json
-from cysecuretools.core.provisioning_flows import Application
 
 
-class ApplicationMXS40Sv2(Application):
+class Application:
     """
-    Implements RAM application data for MXS40Sv2 silicons
+    Implements RAM application data for silicons
     """
 
-    APP_DIR = os.path.abspath(os.path.join(os.path.dirname(
-        __file__), '..', '..', '..', 'targets', 'cyw20829', 'packets', 'apps'))
-
-    def __init__(self, app, app_dir=APP_DIR):
+    def __init__(self, app, app_dir=None):
         """
         Creates instance of the application
-        :param app: Either application name or application
+        @param app: Either application name or application
             configuration file. If the application name is specified,
             the application config will be found in the apps directory,
             otherwise the specified file will be used
+        @param app_dir: Application directory. Not needed if a config
+            file is specified
         """
-        super().__init__(app)
         if os.path.isfile(app):
             self.config = app
         else:
+            if app_dir is None:
+                raise ValueError('Application directory not specified')
             self.config = os.path.join(app_dir, app, 'config.json')
+        self.app_dir = os.path.abspath(os.path.dirname(self.config))
         self.config_data = self._get_json(self.config)
 
         self._name = app
         self._image_path = self._get_image_path()
         self._image_address = self._get_image_address()
         self._in_params_path = self._get_in_params_path()
         self._in_params_address = self._get_in_params_address()
         self._in_params_optional = self._get_in_params_optional()
+        self._out_results_path = self._get_out_results_path()
+        self._out_results_offset = self._get_out_results_offset()
         self._allowed_lcs = self._get_allowed_lcs()
+        self._dfu_commands_path = self._get_dfu_commands_path()
+        self._dlm_path = self._get_dlm_path()
 
     @property
     def name(self):
         """ Application name """
         return self._name
 
     @property
@@ -82,14 +87,34 @@
     @property
     def allowed_lcs(self):
         """
         A list of device lifecycles allowed to program the application
         """
         return self._allowed_lcs
 
+    @property
+    def dfu_commands_path(self):
+        """ A path to the file containing DFU commands """
+        return self._dfu_commands_path
+
+    @property
+    def out_results_path(self):
+        """ A path to the file to save output results """
+        return self._out_results_path
+
+    @property
+    def out_results_offset(self):
+        """ Address offset for app out results """
+        return self._out_results_offset
+
+    @property
+    def dlm_path(self):
+        """ A path to the DLM package """
+        return self._dlm_path
+
     def _get_image_data(self):
         image_data = self.config_data.get('image')
         if image_data is None:
             raise KeyError(f"'image' field not found in '{self.config}'")
         return image_data
 
     def _get_image_path(self):
@@ -105,22 +130,15 @@
         except ValueError as e:
             raise ValueError(f'{e} ({self.config})') from e
         return image_path
 
     def _get_image_address(self):
         image_data = self._get_image_data()
         image_address = image_data.get('address')
-        if image_address is None:
-            raise KeyError(f"Image 'address' not found in '{self.config}'")
-
-        try:
-            image_address = int(image_address, 0)
-        except ValueError as e:
-            raise ValueError(f'{e} ({self.config})') from e
-        return image_address
+        return int(str(image_address), 0) if image_address else None
 
     def _get_in_params_path(self):
         in_params = self.config_data.get('in_params')
         if in_params is None:
             in_params_path = None
         else:
             in_params_path = in_params.get('path')
@@ -133,31 +151,62 @@
                         os.path.dirname(self.config), in_params_path))
             except ValueError as e:
                 raise ValueError(f'{e} ({self.config})') from e
         return in_params_path
 
     def _get_in_params_address(self):
         in_params = self.config_data.get('in_params')
-        if in_params is None:
-            in_params_address = None
-        else:
-            in_params_address = in_params.get('address')
-            if in_params_address is None:
-                raise KeyError(
-                    f"Input parameters 'address' not found in '{self.config}'")
-            in_params_address = int(in_params_address, 0)
-        return in_params_address
+        if in_params:
+            in_params_addr = in_params.get('address')
+            if in_params_addr:
+                return int(str(in_params_addr), 0)
+        return None
 
     def _get_in_params_optional(self):
         in_params = self.config_data.get('in_params')
         return in_params.get('optional', False) if in_params else False
 
+    def _get_out_results_path(self):
+        out_results = self.config_data.get('out_results')
+        out_results_path = out_results.get('path') if out_results else None
+        if out_results_path:
+            if not os.path.isabs(out_results_path):
+                out_results_path = os.path.abspath(os.path.join(
+                    os.path.dirname(self.config), out_results_path))
+        return out_results_path
+
+    def _get_out_results_offset(self):
+        out_results = self.config_data.get('out_results')
+        if out_results:
+            out_offset = out_results.get('offset')
+            return int(str(out_offset), 0) if out_offset else 0
+        return None
+
+    def _get_dlm_path(self):
+        out_results = self.config_data.get('dlm')
+        out_results_path = out_results.get('path') if out_results else None
+        if out_results_path:
+            if not os.path.isabs(out_results_path):
+                out_results_path = os.path.abspath(os.path.join(
+                    os.path.dirname(self.config), out_results_path))
+        return out_results_path
+
     def _get_allowed_lcs(self):
         return self.config_data.get('allowed_lcs')
 
+    def _get_dfu_commands_path(self):
+
+        dfu_cmd_path = self.config_data.get('dfu_commands')
+        if dfu_cmd_path:
+            dfu_cmd_path = dfu_cmd_path.get('path')
+            if not os.path.isabs(dfu_cmd_path):
+                dfu_cmd_path = os.path.abspath(
+                    os.path.join(self.app_dir, dfu_cmd_path))
+        return dfu_cmd_path
+
     @staticmethod
     def _get_json(filename):
         """
         Opens JSON file with the provisioning flows description as
         a dictionary
         """
         with open(filename, encoding='utf-8') as f:
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning/flows/flow_mxs40sv2.py` & `cysecuretools-5.0.0/src/core/provisioning_flows/app_loading_flow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,73 +13,75 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import json
 import logging
-from cysecuretools.core.provisioning_flows import Flow
-from cysecuretools.core.enums import ProvisioningStatus
-from cysecuretools.execute.provisioning.flows.application_mxs40sv2 import (
-    ApplicationMXS40Sv2)
-from cysecuretools.execute.provisioning.load_ram_app import RamAppLoader
-from cysecuretools.targets.common.mxs40sv2.flow_parser import FlowParser
+
+from ..enums import ProvisioningStatus
+from ...core.provisioning_flows.application import Application
+from ...targets.common.flow_parser import FlowParser
 
 logger = logging.getLogger(__name__)
 
 
-class FlowMXS40Sv2(Flow):
-    """ Implements provisioning flow for MXS40Sv2 platform """
+class AppLoadingFlow:
+    """ Implements provisioning flow """
 
-    def __init__(self, target, mode, app_dir, **kwargs):
+    def __init__(self, target, flow_name, app_dir, **kwargs):
         self.target = target
         config = kwargs.get('config', None)
         test_pkg_type = kwargs.get('test_pkg_type')
         self.app_list = []
 
         if config is not None:
-            self.app_list = [ApplicationMXS40Sv2(config)]
+            self.app_list = [Application(config)]
         else:
             flow_parser = FlowParser(target, test_pkg_type=test_pkg_type)
             try:
-                for app in flow_parser.apps_by_flow(mode):
-                    self.app_list.append(ApplicationMXS40Sv2(app, app_dir))
+                for app in flow_parser.apps_by_flow(flow_name):
+                    self.app_list.append(Application(app, app_dir=app_dir))
             except KeyError as e:
                 msg = f'Field {e} not found ({flow_parser.provisioning_flows})'
                 raise KeyError(msg) from e
 
-    def run(self, tool, **kwargs):
+    def run(self, tool):
         """ Starts loading RAM applications """
         status = ProvisioningStatus.OK
 
         if not self.app_list:
             logger.warning('Application list is empty')
 
         self._check_files_exist()
 
         for app in self.app_list:
-            app_loader = RamAppLoader(
-                tool, self.target, kwargs.get('load_app_data'), app)
-            status = app_loader.load()
-
+            self.target.app_loader.__init__(tool, self.target, app)
+            status = self.target.app_loader.load()
             if status == ProvisioningStatus.OK:
                 if app == self.app_list[-1]:
-                    app_loader.reset()
-                self.target.version_provider.log_lifecycle_stage(tool)
+                    self.target.app_loader.reset()
+                try:
+                    self.target.version_provider.log_lifecycle_stage(tool)
+                except RuntimeError:
+                    logging.error('Unable to read current LCS value')
+                    return ProvisioningStatus.FAIL
             elif status == ProvisioningStatus.FAIL:
                 break
-
         return status
 
     def _check_files_exist(self):
         """ Checks whether all the files necessary for provisioning exist """
         for app in self.app_list:
-            if not os.path.isfile(app.image_path):
-                raise FileNotFoundError(f'Application file '
-                                        f'not found ({app.image_path})')
+            file_path = app.dlm_path or app.image_path
+            if not file_path:
+                raise ValueError(f"Application not specified in '{app.config}'")
+            if file_path and not os.path.isfile(file_path):
+                raise FileNotFoundError(
+                    f"Cannot find '{os.path.abspath(file_path)}'")
             if not app.in_params_optional and app.in_params_path is not None:
                 if not os.path.isfile(app.in_params_path):
                     raise FileNotFoundError(
                         f'Application input parameters file not found '
                         f'({app.in_params_path})')
 
     @staticmethod
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning/load_ram_app.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/provisioning/ram_app_loader_mxs40sv2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,96 +1,110 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-import logging
 import os
 import time
+import logging
 
-import cysecuretools.data.mxs40sv2.mxs40sv2_ram_app_status_codes as app_status
-from cysecuretools.core.enums import ProvisioningStatus
-from cysecuretools.execute.programmer.base import AP
-from cysecuretools.targets.common.mxs40sv2.enums import LifecycleStage
+from ..enums import LifecycleStage
+from .....execute.programmer.base import AP
+from .....core.ram_app_loader_base import RamAppLoader
+from .....core.enums import ProvisioningStatus
+from .....data.mxs40sv2 import mxs40sv2_ram_app_status_codes as app_status
 
 logger = logging.getLogger(__name__)
 
 
-class RamAppLoader:
+class RamAppLoaderMXS40Sv2(RamAppLoader):
     """ A class that implements loading RAM application routine """
+    WAIT_FOR_APP_TIMEOUT = 200
+    WAIT_APP_END_TIMEOUT = 200
+    CYAPP_STATE_FINISHED = 2
+    INPUT_PARAM_MIN_SIZE = 8
+
+    RES_SOFT_CTL_RESET_RQST = 0x00000001
+    TST_DBG_CTL_WAIT_APP_RQST = 0x00000001
+    TST_DBG_CTL_WFA_Msk = 0x80000000
+
+    TST_DBG_STS_APP_WFA_SET = 0x0D500080
+    TST_DBG_STS_APP_LAUNCHED = 0x0D500081
+    TST_DBG_STS_APP_NOT_LAUNCHED = 0x0D500082
+    TST_DBG_STS_APP_RUNNING = 0xF2A00010
 
-    def __init__(self, tool, target, load_app_data, app):
+    def __init__(self, tool=None, target=None, app=None):
         self.tool = tool
         self.target = target
-        self.reg_map = target.register_map
-        self.load_data = load_app_data
         self.app = app
 
     def load(self):
         """ Loads application and its input parameters into RAM """
         self.tool.set_ap(AP.SYS)
         time.sleep(0.2)
         self.tool.reset()
 
-        ctrl_reg = self.tool.read32(self.reg_map.TST_DEBUG_CTL)
-        if (ctrl_reg & self.load_data.TST_DBG_CTL_WFA_Msk) == 0:
-            self.tool.write32(self.reg_map.TST_DEBUG_CTL,
-                              self.load_data.TST_DBG_CTL_WAIT_APP_RQST)
+        ctrl_reg = self.tool.read32(self.target.register_map.TST_DEBUG_CTL)
+        if (ctrl_reg & self.TST_DBG_CTL_WFA_Msk) == 0:
+            self.tool.write32(self.target.register_map.TST_DEBUG_CTL,
+                              self.TST_DBG_CTL_WAIT_APP_RQST)
             self.reset()
             logger.debug('Waiting until BootROM stopped '
                          'and read for application upload...')
 
-        for func in [self.check_bootrom_readiness,
-                     self.load_application,
-                     self.load_input_parameters]:
+        for func in [self.__check_bootrom_readiness,
+                     self.__load_application,
+                     self.__load_input_parameters]:
             status = func()
             if status != ProvisioningStatus.OK:
                 return status
 
         logger.debug('Clear DEBUG_IMAGE bit in SRSS_TST_DEBUG_CTL register '
                      'to start application')
-        self.tool.write32(self.reg_map.TST_DEBUG_CTL, 0)
+        self.tool.write32(self.target.register_map.TST_DEBUG_CTL, 0)
         self.tool.resume()
 
-        return self.app_completion_status()
+        return self.__app_completion_status()
 
-    def check_bootrom_readiness(self):
+    def __check_bootrom_readiness(self):
         """ Checks whether BootROM is ready for application programming """
         status = ProvisioningStatus.OK
         counter = 0
-        while (self.tool.read32(self.reg_map.TST_DEBUG_CTL) &
-               self.load_data.TST_DBG_CTL_WFA_Msk) == 0:
+        while (self.tool.read32(self.target.register_map.TST_DEBUG_CTL) &
+               self.TST_DBG_CTL_WFA_Msk) == 0:
             counter += 1
-            if counter > self.load_data.WAIT_FOR_APP_TIMEOUT:
+            if counter > self.WAIT_FOR_APP_TIMEOUT:
                 raise TimeoutError('BootROM did not set flag '
                                    'waiting for application')
             time.sleep(0.1)
-        debug_sts = self.tool.read32(self.reg_map.TST_DEBUG_STATUS)
-        if debug_sts != self.load_data.TST_DBG_STS_APP_WFA_SET:
+        debug_sts = self.tool.read32(self.target.register_map.TST_DEBUG_STATUS)
+        if debug_sts != self.TST_DBG_STS_APP_WFA_SET:
+            logger.error('TST_DEBUG_STATUS: 0x%x',
+                         self.target.register_map.TST_DEBUG_STATUS)
             logger.error(
-                'TST_DEBUG_STATUS: 0x%x', self.reg_map.TST_DEBUG_STATUS)
-            logger.error('TST_DEBUG_CTL: 0x%x', self.reg_map.TST_DEBUG_CTL)
+                'TST_DEBUG_CTL: 0x%x', self.target.register_map.TST_DEBUG_CTL)
             logger.error('BootROM did not set expected TST_DEBUG_STATUS')
             status = ProvisioningStatus.FAIL
         else:
             logger.debug('Ready for application programming')
 
         return status
 
-    def load_application(self):
+    def __load_application(self):
         """ Programs application into RAM """
         lcs = self.target.silicon_data_reader.read_lifecycle_stage(self.tool)
         lcs = LifecycleStage(lcs).name.upper()
         if lcs in self.app.allowed_lcs:
             logger.info(
                 "Programming '%s' application at address 0x%x (%s)",
                 self.app.name, self.app.image_address, self.app.image_path)
@@ -100,71 +114,73 @@
             status = ProvisioningStatus.OK
         else:
             logger.warning("Skip programming '%s' application. The device "
                            "lifecycle stage is %s", self.app.name, lcs)
             status = ProvisioningStatus.SKIPPED
         return status
 
-    def load_input_parameters(self):
+    def __load_input_parameters(self):
         """ Programs application input parameters """
         status = ProvisioningStatus.OK
         if self.app.in_params_path and os.path.isfile(self.app.in_params_path):
             file_size = os.path.getsize(self.app.in_params_path)
-            if file_size > self.load_data.INPUT_PARAM_MIN_SIZE:
+            if file_size > self.INPUT_PARAM_MIN_SIZE:
                 logger.info(
                     "Programming '%s' application input parameters at address "
                     "0x%x (%s)", self.app.name, self.app.in_params_address,
                     self.app.in_params_path)
                 self.tool.program_ram(self.app.in_params_path,
-                                  address=self.app.in_params_address)
+                                      address=self.app.in_params_address)
                 logger.info('Programming complete')
             else:
                 raise ValueError(f'Input parameters size must be larger then '
-                                 f'{self.load_data.INPUT_PARAM_MIN_SIZE} '
+                                 f'{self.INPUT_PARAM_MIN_SIZE} '
                                  f'bytes ({self.app.in_params_path}')
         else:
             logger.debug('No input parameters provided, skipped')
 
         return status
 
-    def app_completion_status(self):
+    def __app_completion_status(self):
         """ Checks application programming status """
         status = ProvisioningStatus.OK
         # Wait until debugger is connected and TST_DEBUG_STATUS is changed
         timeout = 0
-        tmp_status = self.load_data.TST_DBG_STS_APP_WFA_SET
-        while tmp_status == self.load_data.TST_DBG_STS_APP_WFA_SET:
+        tmp_status = self.TST_DBG_STS_APP_WFA_SET
+        while tmp_status == self.TST_DBG_STS_APP_WFA_SET:
             timeout += 1
-            if timeout > self.load_data.WAIT_APP_END_TIMEOUT:
+            if timeout > self.WAIT_APP_END_TIMEOUT:
                 raise TimeoutError('Application did not return status')
             time.sleep(0.1)
             try:
-                tmp_status = self.tool.read32(self.reg_map.TST_DEBUG_STATUS)
+                tmp_status = self.tool.read32(
+                    self.target.register_map.TST_DEBUG_STATUS)
             except RuntimeError:
-                tmp_status = self.load_data.TST_DBG_STS_APP_WFA_SET
+                tmp_status = self.TST_DBG_STS_APP_WFA_SET
 
         # Wait for application completion
-        while tmp_status in [self.load_data.TST_DBG_STS_APP_LAUNCHED,
-                             self.load_data.TST_DBG_STS_APP_RUNNING]:
+        while tmp_status in [self.TST_DBG_STS_APP_LAUNCHED,
+                             self.TST_DBG_STS_APP_RUNNING]:
             timeout += 1
-            if timeout > self.load_data.WAIT_APP_END_TIMEOUT:
-                if tmp_status == self.load_data.TST_DBG_STS_APP_WFA_SET:
+            if timeout > self.WAIT_APP_END_TIMEOUT:
+                if tmp_status == self.TST_DBG_STS_APP_WFA_SET:
                     logger.error('BootROM pass control to application timeout '
                                  '(status: 0x%x)', tmp_status)
-                elif tmp_status == self.load_data.TST_DBG_STS_APP_RUNNING:
+                elif tmp_status == self.TST_DBG_STS_APP_RUNNING:
                     logger.error('Application return status timeout '
                                  '(status: 0x%x)', tmp_status)
                 else:
                     logger.error('Unexpected error - status 0x%x', tmp_status)
                 raise TimeoutError('Application did not return status')
             time.sleep(0.1)
-            tmp_status = self.tool.read32(self.reg_map.TST_DEBUG_STATUS)
+            tmp_status = self.tool.read32(
+                self.target.register_map.TST_DEBUG_STATUS)
 
         # Application completion status
-        if tmp_status == self.load_data.TST_DBG_STS_APP_NOT_LAUNCHED:
+        if tmp_status == self.TST_DBG_STS_APP_NOT_LAUNCHED:
             logger.error('BootROM did not launch application due to '
                          'verification failure (status: 0x%x)', tmp_status)
             status = ProvisioningStatus.FAIL
         else:
             if tmp_status == app_status.get_code_by_name('CYAPP_SUCCESS'):
                 logger.info('Application execution successfully completed')
             else:
@@ -173,16 +189,16 @@
 
         return status
 
     def reset(self):
         """ Reset device using RES_SOFT_CTL register """
         logger.debug('Reset device')
         try:
-            self.tool.write32(self.reg_map.RES_SOFT_CTL,
-                              self.load_data.RES_SOFT_CTL_RESET_RQST)
+            self.tool.write32(self.target.register_map.RES_SOFT_CTL,
+                              self.RES_SOFT_CTL_RESET_RQST)
         except RuntimeError:
             pass  # the mww command fails so catch this fail and continue
         time.sleep(0.1)
 
     @staticmethod
     def print_ram_app_status(status_code, severity='error'):
         """
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning/provision_device_mxs40sv2.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/provisioning/provision_device_mxs40sv2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,35 +14,30 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import logging
 from shutil import copyfile
 
-from cysecuretools.core.target_director import Target
-from cysecuretools.core.enums import ProvisioningStatus
-from cysecuretools.core.strategy_context.provisioning_strategy_ctx import (
-    ProvisioningStrategy)
-from cysecuretools.execute.provisioning.flows import FlowMXS40Sv2
-from ..provisioning.flows.application_mxs40sv2 import ApplicationMXS40Sv2
-from ...targets.common.mxs40sv2.flow_parser import FlowParser
-from ...targets.common.mxs40sv2.enums import LifecycleStage
+from ..enums import LifecycleStage
+from ...flow_parser import FlowParser
+from .....core.provisioning_flows.application import Application
+from .....core.provisioning_flows.app_loading_flow import AppLoadingFlow
+from .....core.target_director import Target
+from .....core.enums import ProvisioningStatus
+from .....core.strategy_context import ProvisioningStrategy
 
 
 logger = logging.getLogger(__name__)
 
 
 class ProvisioningMXS40Sv2(ProvisioningStrategy):
     """
     A high-level class for provisioning targets on MXS40Sv2 platform
     """
-
-    def __init__(self, **kwargs):
-        self.load_app_data = kwargs.get('load_app_data')
-
     def provision(self, tool, target: Target, bootloader=None,
                   **kwargs) -> ProvisioningStatus:
         """
         Starts provisioning process using the specified flow
         :param tool: Programming/debugging tool used for communication
         :param target: The target object
         :param bootloader: N/A for MXS40Sv2 platform
@@ -50,15 +46,15 @@
         :return:
             The provisioning status
         """
         mode = None
         config = kwargs.get('config')
 
         if config is None:
-            mode = target.policy_parser.get_policy_type()
+            mode = target.policy_parser.policy_type()
 
         if mode is not None and 'reprovisioning' in mode:
             raise ValueError('Reprovisioning policy type specified for the '
                              'provisioning operation')
 
         status = self._provision(
             tool, target, mode, config, kwargs.get('testapps'))
@@ -81,15 +77,15 @@
         :param target: The target object
         :param bootloader: N/A for MXS40Sv2 platform
         :raises:
             ValueError - when invalid policy type is used
         :return:
             The reprovisioning status
         """
-        mode = target.policy_parser.get_policy_type()
+        mode = target.policy_parser.policy_type()
         if 'reprovisioning' not in mode:
             raise ValueError('Provisioning policy type specified for the '
                              'reprovisioning operation')
 
         status = self._provision(
             tool, target, mode, None, kwargs.get('testapps'))
 
@@ -103,36 +99,35 @@
 
         return status
 
     def erase_flash(self, tool, target):
         """ N/A. The target does not have flash """
 
     def transit_to_rma(self, tool, target, cert, **kwargs):
-        """ Converts a part to the RMA LCS """
+        """ Transits a part to the RMA LCS """
         test_pkg_type = kwargs.get('testapps')
 
         flow_parser = FlowParser(target, test_pkg_type=test_pkg_type)
         apps = flow_parser.apps_by_flow('rma')
         if not apps:
             raise ValueError('RAM applications list is empty')
 
         lcs_value = target.silicon_data_reader.read_lifecycle_stage(tool)
         if lcs_value == LifecycleStage.SECURE:
             if cert is None:
                 logger.error('Certificate must be specified for transition '
                              'from SECURE to RMA LCS')
                 return ProvisioningStatus.FAIL
-            else:
-                if not self._copy_rma_cert(cert, apps, flow_parser.apps_dir):
-                    return ProvisioningStatus.FAIL
+            if not self._copy_rma_cert(cert, apps, flow_parser.apps_dir):
+                return ProvisioningStatus.FAIL
         else:
             if cert is not None:
                 logger.warning(
-                    f'The certificate will be ignored. Transition from the '
-                    f'current LCS to RMA LCS does not require a certificate')
+                    'The certificate will be ignored. Transition from the '
+                    'current LCS to RMA LCS does not require a certificate')
 
         status = self._provision(
             tool, target, 'rma', apps_dir=flow_parser.apps_dir,
             test_pkg_type=test_pkg_type)
 
         self._remove_rma_inparams(apps, flow_parser.apps_dir)
 
@@ -141,38 +136,38 @@
             logger.info('       TRANSITION TO RMA PASSED          ')
             logger.info('*****************************************\n')
         elif status == ProvisioningStatus.SKIPPED:
             logger.error('The device cannot be converted to RMA due to '
                          'invalid lifecycle stage')
         return status
 
-    def open_rma(self, tool, target, cert, **kwargs):
+    def open_rma(self, tool, target, cert):
         """Not implemented for MXS40Sv2 platform"""
         raise NotImplementedError
 
     @staticmethod
     def _copy_rma_cert(cert, apps, apps_dir):
         for app_name in apps:
-            app = ApplicationMXS40Sv2(app_name, apps_dir)
+            app = Application(app_name, app_dir=apps_dir)
             cert = os.path.abspath(cert)
             if os.path.isfile(cert):
                 logger.debug("Copy '%s' into '%s'", cert, app.in_params_path)
                 copyfile(cert, app.in_params_path)
             else:
                 logger.error("File '%s' not found", cert)
                 return False
         return True
 
     @staticmethod
     def _remove_rma_inparams(apps, apps_dir):
         for app_name in apps:
-            app = ApplicationMXS40Sv2(app_name, apps_dir)
+            app = Application(app_name, app_dir=apps_dir)
             if os.path.isfile(app.in_params_path):
                 logger.debug("Remove file '%s'", app.in_params_path)
                 os.remove(app.in_params_path)
 
     def _provision(self, tool, target, mode, config=None, test_pkg_type=None,
                    apps_dir=None):
         app_dir = apps_dir if apps_dir else target.project_initializer.apps_dir
-        flow = FlowMXS40Sv2(
+        flow = AppLoadingFlow(
             target, mode, app_dir, config=config, test_pkg_type=test_pkg_type)
-        return flow.run(tool, load_app_data=self.load_app_data)
+        return flow.run(tool)
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning/provision_device_mxs40v1.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning/provision_device_mxs40v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2018-2023 Cypress Semiconductor Corporation
+Copyright 2018-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,35 +14,30 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import json
 import logging
 from time import sleep
-import cysecuretools.execute.provisioning_packet.provisioning_packet_mxs40v1 as prov_packet
-from cysecuretools.core.connect_helper import ConnectHelper
-from cysecuretools.core.target_director import Target
-from cysecuretools.core.enums import (EntranceExamStatus, ProvisioningStatus)
-from cysecuretools.execute.provisioning_packet.lib.cyprov_pem import PemKey
-from cysecuretools.execute.sys_call import (
-    provision_keys_and_policies, read_lifecycle, dap_control, get_prov_details,
-    transition_to_rma, open_rma, FB_POLICY_JWT)
-from cysecuretools.execute.programmer.base import AP
-from cysecuretools.execute.programmer.pyocd_wrapper import ResetType
-from cysecuretools.core.strategy_context.provisioning_strategy_ctx import \
-    ProvisioningStrategy
-from cysecuretools.core.strategy_context.encrypted_programming_strategy_ctx \
-    import EncryptedProgrammingContext
-from cysecuretools.execute.encrypted_programming.aes_header_strategy import \
-    AesHeaderStrategy
-from cysecuretools.data.mxs40v1.mxs40v1_sfb_status_codes import \
-    sfb_status_codes
-from cysecuretools.targets.common.p64.policy_parser import PolicyParser
-from cysecuretools.targets.common.p64.enums import ProtectionState, KeyId
-from cysecuretools.execute.provisioning_packet.lib import Crypto
+
+from . import sys_call
+from ..enums import ProtectionState, KeyId
+from ..encrypted_programming import AesHeaderStrategy
+from ..provisioning_packet import provisioning_packet_mxs40v1 as prov_packet
+from .....execute import jwt
+from .....core.key_handlers.pem_key import PemKey
+from .....core.connect_helper import ConnectHelper
+from .....core.target_director import Target
+from .....core.enums import EntranceExamStatus, ProvisioningStatus
+from .....core.strategy_context import ProvisioningStrategy
+from .....core.strategy_context import EncryptedProgrammingContext
+from .....execute.programmer.base import AP, ResetType
+
+from .....data.mxs40v1.mxs40v1_sfb_status_codes import sfb_status_codes
+
 
 logger = logging.getLogger(__name__)
 
 
 class ProvisioningMXS40v1(ProvisioningStrategy):
 
     def provision(self, tool, target: Target, bootloader,
@@ -52,23 +48,16 @@
         :param tool: Programming/debugging tool used for communication
         :param target: The target object.
         :param bootloader: Path to Cypress Bootloader program file.
         :param kwargs: Dictionary with the following fields:
                - probe_id: Probe ID to use
         :return: Provisioning status.
         """
-        if 'skip_prompts' in kwargs:
-            skip_prompts = kwargs['skip_prompts']
-        else:
-            skip_prompts = None
-
-        if 'probe_id' in kwargs:
-            probe_id = kwargs['probe_id']
-        else:
-            probe_id = None
+        skip_prompts = kwargs.get('skip_prompts')
+        probe_id = kwargs.get('probe_id')
 
         prov_packets = self._get_provisioning_packet(target)
         status = _provision_identity(
             tool, target, prov_packets['prov_identity'], skip_prompts)
 
         if status == ProvisioningStatus.OK:
             status = _provision_complete(tool, target,
@@ -91,84 +80,74 @@
         :param target: The target object.
         :param bootloader: Path to Cypress Bootloader program file.
         :param kwargs: Dictionary with the following fields:
                - erase_boot: Indicates whether to erase BOOT slot
                - control_dap_cert: Certificate for AP control
         :return: Provisioning status.
         """
-        if 'erase_boot' in kwargs:
-            erase_boot = kwargs['erase_boot']
-        else:
-            erase_boot = False
-
-        if 'control_dap_cert' in kwargs:
-            control_dap_cert = kwargs['control_dap_cert']
-        else:
-            control_dap_cert = None
-
-        if 'probe_id' in kwargs:
-            probe_id = kwargs['probe_id']
-        else:
-            probe_id = None
+        erase_boot = kwargs.get('erase_boot', False)
+        control_dap_cert = kwargs.get('control_dap_cert')
+        probe_id = kwargs.get('probe_id')
 
         prov_packets = self._get_re_provisioning_packet(target)
         status = _provision_complete(
             tool, target, prov_packets['prov_cmd'], bootloader, True,
             erase_boot=erase_boot, control_dap_cert=control_dap_cert,
             probe_id=probe_id)
 
         if status == ProvisioningStatus.OK:
             logger.info('*****************************************')
-            logger.info('       RE-PROVISIONING PASSED               ')
+            logger.info('       RE-PROVISIONING PASSED            ')
             logger.info('*****************************************\n')
 
         return status
 
     def erase_flash(self, tool, target):
         """
         Erases allowed (w/o bootloader, data only) flash area
         :param tool: Programming/debugging tool used for communication
         :param target: The target object
         """
         erase_flash(tool, target)
 
-    def transit_to_rma(self, tool, target, cert, *_):
+    def transit_to_rma(self, tool, target, cert, **_):
         """Transits a part to the RMA LCS
         @param tool: Programming/debugging tool used for communication
         @param target: The target object
         @param cert: JWT packet signed by the key mentioned in the debug/RMA
                      section of the policy, with authentication object
                      including valid DIE_ID range
         """
         if cert is None:
             raise ValueError('Certificate not specified')
         logger.info("Apply certificate '%s'", cert)
         with open(cert, encoding='utf-8') as f:
             cert_data = f.read()
-        if transition_to_rma(tool, target.memory_map, target.register_map,
-                             cert_data):
+        if sys_call.transition_to_rma(
+                tool, target.memory_map, target.register_map, cert_data):
             tool.reset()
             logger.info('*****************************************')
             logger.info('      TRANSITION TO RMA LCS PASSED       ')
             logger.info('*****************************************\n')
             return ProvisioningStatus.OK
         return ProvisioningStatus.FAIL
 
-    def open_rma(self, tool, target, cert, **kwargs):
+    def open_rma(self, tool, target, cert):
         """Enables full access to device in RMA lifecycle stage
         @param tool: Programming/debugging tool used for communication
         @param target: The target object
         @param cert: JWT packet signed by the key mentioned in the debug/RMA
                      section of the policy, with authentication object
                      including valid DIE_ID range
         """
         logger.info("Apply certificate '%s'", cert)
         with open(cert, encoding='utf-8') as f:
             cert_data = f.read()
-        if open_rma(tool, target.memory_map, target.register_map, cert_data):
+        if sys_call.open_rma(tool, target.memory_map, target.register_map,
+                             cert_data):
             logger.info('*****************************************')
             logger.info('          FULL ACCESS ENABLED            ')
             logger.info('        DO NOT RESET THE DEVICE          ')
             logger.info('*****************************************\n')
             return ProvisioningStatus.OK
         return ProvisioningStatus.FAIL
 
@@ -203,16 +182,17 @@
     """
     Reads silicon data from device
     :param tool: Programming/debugging tool used for communication
     :param target: The target object.
     :return: Device response
     """
     logger.debug('Read silicon data')
-    tool.reset(ResetType.HW)
-    _, response = provision_keys_and_policies(tool, None, target.register_map)
+    tool.reset(ResetType.SW)
+    _, response = sys_call.provision_keys_and_policies(tool, None,
+                                                       target.register_map)
     return response
 
 
 def erase_flash(tool, target):
     logger.info('Erase main flash:')
     addr = target.memory_map.FLASH_ADDRESS
     size = target.memory_map.FLASH_SIZE
@@ -300,15 +280,15 @@
         tool.set_ap(ap)
         if first_only:
             break
 
 
 def _provision_identity(tool, target: Target,
                         prov_identity_jwt, skip_prompts) -> ProvisioningStatus:
-    lifecycle = read_lifecycle(tool, target.register_map)
+    lifecycle = sys_call.read_lifecycle(tool, target.register_map)
     tool.examine_ap()
 
     if lifecycle == ProtectionState.secure:
         status = target.entrance_exam.execute(tool)
         if status == EntranceExamStatus.FLASH_NOT_EMPTY:
             if skip_prompts:
                 logger.error('Cannot start provisioning. '
@@ -324,15 +304,15 @@
             return ProvisioningStatus.FAIL
     else:
         erase_flash(tool, target)
 
     tool.reset_and_halt()
     sleep(0.2)
 
-    is_exam_pass, response = provision_keys_and_policies(
+    is_exam_pass, response = sys_call.provision_keys_and_policies(
         tool, prov_identity_jwt, target.register_map)
     _save_device_response(target, response)
 
     if not is_exam_pass:
         logger.error('Unexpected ProvisionKeysAndPolicies syscall response')
         return ProvisioningStatus.FAIL
     else:
@@ -342,15 +322,15 @@
 def _provision_complete(tool, target: Target, prov_cmd_jwt, bootloader,
                         re_provision, erase_boot=False, control_dap_cert=None,
                         probe_id=None, ap='cm0') -> ProvisioningStatus:
     reg_map = target.register_map
     flash_ops_allowed = True
 
     if re_provision:
-        is_cm0_open = read_cm0_permissions(tool, reg_map)
+        is_cm0_open = read_cm0_permissions(tool, target)
         if is_cm0_open:
             ConnectHelper.disconnect(tool)
             ConnectHelper.connect(tool, target, probe_id=probe_id, ap=ap)
             tool.examine_ap()
         flash_ops_allowed = is_cm0_open
 
     if flash_ops_allowed:
@@ -375,21 +355,21 @@
             logger.info('SFB status: %s: %s', status['status'], status['desc'])
         except KeyError:
             logger.debug('Unexpected SFB status 0x%x', received)
 
     # Open cm0 AP with a certificate
     if control_dap_cert:
         logger.info('Opening cm0 AP')
-        is_cm0_open = dap_control(tool, reg_map, 0, 1, False, control_dap_cert)
+        is_cm0_open = sys_call.dap_control(
+            tool, reg_map, 0, 1, False, control_dap_cert)
         logger.info('cm0 AP %s', 'open' if is_cm0_open else 'closed')
         if is_cm0_open:
             ConnectHelper.disconnect(tool)
             ConnectHelper.connect(tool, target, probe_id=probe_id, ap='cm0',
                                   acquire=False)
-            tool.set_skip_reset_and_halt(True)
             tool.examine_ap()
         flash_ops_allowed = is_cm0_open
 
     if erase_boot:
         if flash_ops_allowed:
             erase_slots(tool, target, 'BOOT')
         else:
@@ -458,26 +438,23 @@
             logger.info("Programming bootloader '%s':", bootloader)
             tool.halt()
             tool.program(bootloader)
             logger.info('Programming bootloader complete')
             tool.resume()
             tool.set_ap(current_ap)
 
-    if control_dap_cert:
-        tool.set_skip_reset_and_halt(False)
-
-    tool.reset(ResetType.HW)
+    tool.reset(ResetType.SW)
     sleep(3)
 
     _save_device_public_key(tool, target)
 
     # Run provisioning syscall
     logger.info('Run provisioning syscall:')
-    is_exam_pass, response = provision_keys_and_policies(tool, prov_cmd_jwt,
-                                                         target.register_map)
+    is_exam_pass, response = sys_call.provision_keys_and_policies(
+        tool, prov_cmd_jwt, target.register_map)
     tool.reset()
 
     if not is_exam_pass:
         return ProvisioningStatus.FAIL
 
     _save_device_response(target, response)
 
@@ -492,20 +469,21 @@
 
     if not is_exam_pass:
         logger.error('FlashBoot firmware status is not as expected')
 
     return ProvisioningStatus.OK if is_exam_pass else ProvisioningStatus.FAIL
 
 
-def read_cm0_permissions(tool, reg_map):
+def read_cm0_permissions(tool, target):
     logger.info('Checking cm0 AP permissions')
-    passed, data = get_prov_details(tool, reg_map, FB_POLICY_JWT)
+    passed, data = sys_call.get_prov_details(tool, target.register_map,
+                                             sys_call.FB_POLICY_JWT)
     if passed and len(data) > 0:
-        policy = Crypto.readable_jwt(data)
-        silicon_policy_parser = PolicyParser(policy['payload'])
+        policy = jwt.readable_jwt(data)
+        silicon_policy_parser = target.policy_parser.__class__(policy['payload'])
         is_cm0_open = silicon_policy_parser.is_cmx_ap_enabled(True)
         logger.info('cm0 AP %s', 'open' if is_cm0_open else 'closed')
     else:
         logger.error('Failed to read policy from device while getting AP '
                      'permission')
         logger.warning('Flash operations will be skipped')
         is_cm0_open = False
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_crypto.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_crypto.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import json
 import logging
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives.asymmetric import ec
+from datetime import datetime
+
 from jose import jws, jwt
 from jose.constants import ALGORITHMS
 from jose.utils import long_to_base64
-from datetime import datetime
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives.asymmetric import ec
 
 logger = logging.getLogger(__name__)
 
 
 class Crypto:
     @staticmethod
     def create_jwk():
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_dev.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_dev.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
-from cysecuretools.execute.provisioning_packet.lib.cyprov_types import Types
-from cysecuretools.execute.provisioning_packet.lib.cyprov_entity import Entity
-from cysecuretools.execute.provisioning_packet.lib.cyprov_crypto import Crypto
+
+from .cyprov_types import Types
+from .cyprov_entity import Entity
+from .cyprov_crypto import Crypto
 
 
 class DeviceEntity(Entity):
     STAGE_VIRGIN = "VIRGIN"
     STAGE_NORMAL = "NORMAL"
     STAGE_SECURE = "SECURE"
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_entity.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_entity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,15 +12,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import json
 import os
-from cysecuretools.execute.key_reader import load_key
+
+from ......execute.key_reader import load_key
 
 
 # Cypress Entity
 class Entity:
     def __init__(self, state_name, audit_name):
         self.state = {}
         self.state_name = state_name
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_hsm.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_hsm.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import logging
 import base64
-from cysecuretools.execute.provisioning_packet.lib.cyprov_types import Types
-from cysecuretools.execute.provisioning_packet.lib.cyprov_entity import Entity
-from cysecuretools.execute.provisioning_packet.lib.cyprov_crypto import Crypto
+
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 
+from .cyprov_types import Types
+from .cyprov_entity import Entity
+from .cyprov_crypto import Crypto
+
 logger = logging.getLogger(__name__)
 
 
 class HsmEntity(Entity):
     def __init__(self, state_name='', audit_name='',
                  hsm_priv_key=None, hsm_pub_key=None):
         Entity.__init__(self, state_name, audit_name)
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_oem.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_oem.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.execute.provisioning_packet.lib.cyprov_types import Types
-from cysecuretools.execute.provisioning_packet.lib.cyprov_entity import Entity
-from cysecuretools.execute.provisioning_packet.lib.cyprov_crypto import Crypto
 from datetime import datetime
 
+from .cyprov_types import Types
+from .cyprov_entity import Entity
+from .cyprov_crypto import Crypto
+
 
 class OemEntity(Entity):
     def __init__(self, state_name='', audit_name='',
                  oem_priv_key=None, oem_pub_key=None):
         Entity.__init__(self, state_name, audit_name)
         if oem_priv_key and oem_pub_key:
             self.create_entity(oem_priv_key=oem_priv_key,
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_pem.py` & `cysecuretools-5.0.0/src/core/key_handlers/pem_key.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2019 Cypress Semiconductor Corporation
+Copyright (c) 2019-2022 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,91 +11,94 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import json
 import logging
-from jose.backends import ECKey
+
+import jose
+from jose.backends import ECKey, RSAKey
 from jose.constants import ALGORITHMS
 
 logger = logging.getLogger(__name__)
 
 
-def pretty_search(dict_or_list, key_to_search, search_for_first_only=False):
-    """
-    Give it a dict or a list of dicts and a dict key (to get values of),
-    it will search through it and all containing dicts and arrays
-    for all values of dict key you gave, and will return you set of them
-    unless you wont specify search_for_first_only=True
-
-    :param dict_or_list:
-    :param key_to_search:
-    :param search_for_first_only:
-    :return:
-    """
-    search_result = set()
-    if isinstance(dict_or_list, dict):
-        for key in dict_or_list:
-            key_value = dict_or_list[key]
-            if key == key_to_search:
-                if search_for_first_only:
-                    return key_value
-                else:
-                    search_result.add(key_value)
-            if isinstance(key_value, dict) or isinstance(key_value, list) or isinstance(key_value, set):
-                _search_result = pretty_search(key_value, key_to_search, search_for_first_only)
-                if _search_result and search_for_first_only:
-                    return _search_result
-                elif _search_result:
-                    for result in _search_result:
-                        search_result.add(result)
-    elif isinstance(dict_or_list, list) or isinstance(dict_or_list, set):
-        for element in dict_or_list:
-            if isinstance(element, list) or isinstance(element, set) or isinstance(element, dict):
-                _search_result = pretty_search(element, key_to_search, search_result)
-                if _search_result and search_for_first_only:
-                    return _search_result
-                elif _search_result:
-                    for result in _search_result:
-                        search_result.add(result)
-    return search_result if search_result else None
-
-
 class PemKey:
+    """A class representing a key in a PEM format"""
+
     def __init__(self, jwk_file=None, item=None):
         if jwk_file is not None:
             if isinstance(jwk_file, dict):
                 self.jwk = jwk_file
             else:
                 with open(jwk_file, encoding='utf-8') as f:
                     jwk_str = f.read()
                     self.jwk = json.loads(jwk_str)
 
         if item is not None:
-            self.jwk = pretty_search(
-                self.jwk,
-                item,
-                search_for_first_only=True
-            )
+            self.jwk = self._pretty_search(self.jwk, item,
+                                           search_first_only=True)
 
     def save(self, file=None, private_key=False):
+        """Saves a key to a file"""
         pem_str = self.to_str(private_key)
         if file is not None:
             with open(file, 'wb') as f:
                 f.write(pem_str)
         else:
             logger.info(pem_str)
 
     def to_str(self, private_key=False):
-        key = ECKey(self.jwk, ALGORITHMS.ES256)
+        """Converts EC or RSA key to string"""
+        try:
+            key = ECKey(self.jwk, ALGORITHMS.ES256)
+        except jose.exceptions.JWKError:
+            key = RSAKey(self.jwk, ALGORITHMS.RS256)
         if private_key:
             pem_str = key.to_pem().strip()
         else:
             pem_str = key.public_key().to_pem().strip()
         return pem_str
 
     def load(self, jwk):
+        """Loads JWK"""
         self.jwk = jwk
 
     def load_str(self, jwk_str):
+        """Loads JWK string"""
         self.jwk = json.loads(jwk_str)
+
+    @staticmethod
+    def _pretty_search(dict_or_list, key_to_search, search_first_only=False):
+        """Give it a dict or a list of dicts and a dict key (to get values of),
+        it will search through it and all containing dicts and arrays
+        for all values of dict key you gave, and will return you set of them
+        unless you want to specify search_first_only=True
+        """
+        search_result = set()
+        if isinstance(dict_or_list, dict):
+            for key in dict_or_list:
+                key_value = dict_or_list[key]
+                if key == key_to_search:
+                    if search_first_only:
+                        return key_value
+                    search_result.add(key_value)
+                if isinstance(key_value, (dict, list, set)):
+                    _search_result = PemKey._pretty_search(
+                        key_value, key_to_search, search_first_only)
+                    if _search_result and search_first_only:
+                        return _search_result
+                    if _search_result:
+                        for result in _search_result:
+                            search_result.add(result)
+        elif isinstance(dict_or_list, (list, set)):
+            for element in dict_or_list:
+                if isinstance(element, (list, set, dict)):
+                    _search_result = PemKey._pretty_search(
+                        element, key_to_search, search_result)
+                    if _search_result and search_first_only:
+                        return _search_result
+                    if _search_result:
+                        for result in _search_result:
+                            search_result.add(result)
+        return search_result if search_result else None
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/lib/cyprov_types.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/lib/cyprov_types.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40sv2.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/provisioning_packet_mxs40sv2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,41 +14,40 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import errno
 import logging
 
-from cysecuretools.core.json_helper import read_json, dump_json
-from cysecuretools.core.key_handlers import RSAHandler
-from cysecuretools.core.strategy_context.prov_packet_strategy_ctx import (
-    ProvisioningPacketStrategy)
-from cysecuretools.targets.common.mxs40sv2.asset_builder import AssetBuilder
-from cysecuretools.targets.common.mxs40sv2.enums import PolicyType
-from cysecuretools.targets.common.mxs40sv2.flow_parser import FlowParser
+from .asset_builder import AssetBuilder
+from .enums import PolicyType
+from ..flow_parser import FlowParser
+from ....core.json_helper import read_json, dump_json
+from ....core.key_handlers.rsa_handler import RSAHandler
+from ....core.strategy_context import ProvisioningPacketStrategy
 
 logger = logging.getLogger(__name__)
 
 
 class ProvisioningPacketMXS40Sv2(ProvisioningPacketStrategy):
     """ Provisioning packet generator for MXS40Sv2 targets """
 
     ASSETS_DIR = os.path.abspath(os.path.join(
-        os.path.dirname(__file__),
-        '..', '..', 'targets', 'cyw20829', 'flows'))
+        os.path.dirname(__file__), '..', '..', 'cyw20829', 'flows'))
 
-    def __init__(self, policy_parser):
+    def __init__(self, policy_parser, asset_map):
         self.policy_parser = policy_parser
+        self.asset_map = asset_map
 
     def create(self, target, **kwargs):
         """
         Creates RAM applications input parameters binary packets
         :return: True if packet created successfully, otherwise False.
         """
-        policy_type = self.policy_parser.get_policy_type()
+        policy_type = self.policy_parser.policy_type()
         apps_dir = target.project_initializer.apps_dir
         flow_parser = FlowParser(target, kwargs.get('testapps'))
         apps_data = flow_parser.apps_by_flow(policy_type)
 
         for app, config_path in apps_data.items():
 
             if not os.path.isfile(config_path):
@@ -79,30 +79,39 @@
                 with open(in_params_path, 'wb') as f:
                     f.write(input_data)
 
                 logger.info("Provisioning packet for '%s' application "
                             "successfully created (%s)", app, in_params_path)
         return True
 
+    def verify(self, target, **kwargs):
+        """N/A for the MXS40Sv2 platform"""
+        raise NotImplementedError
+
+    def create_package(self, target, **kwargs):
+        """N/A for MXS40Sv2 platform"""
+        raise NotImplementedError
+
     def reverse_conversion(self, target, packets, output):
         """ Does conversion of provisioning packet to policy """
-        policy_type = self.policy_parser.get_policy_type()
+        policy_type = self.policy_parser.policy_type()
         if PolicyType.REPROVISIONING_SECURE == policy_type:
             assets = self._reprovisioning_assets()
         else:
             assets = self._provisioning_assets()
         data = target.policy_generator.populate(packets, assets)
         dump_json(data, output)
         logger.info("Created policy in '%s'", os.path.abspath(output))
         return True
 
     def provisioning_data(self):
         """ Gets provisioning packet data """
         assets_list = self._provisioning_assets()
-        asset_builder = AssetBuilder(self.policy_parser, assets_list)
+        asset_builder = AssetBuilder(
+            self.policy_parser, assets_list, self.asset_map)
         input_data = asset_builder.get_assets()
         return input_data
 
     def reprovisioning_data(self, key_source, **kwargs):
         """ Gets reprovisioning packet data """
         key_id = kwargs.get('key_id')
         key_path = kwargs.get('key_path')
@@ -133,15 +142,15 @@
         if not signature:
             if not os.path.isfile(pubkey):
                 raise FileNotFoundError(
                     errno.ENOENT, os.strerror(errno.ENOENT), pubkey)
 
             assets_list = self._reprovisioning_assets()
             asset_builder = AssetBuilder(
-                self.policy_parser, assets_list, pubkey=pubkey,
+                self.policy_parser, assets_list, self.asset_map, pubkey=pubkey,
                 image_id=kwargs.get('image_id'))
             input_data = asset_builder.get_assets()
         else:
             if not in_params_path:
                 raise ValueError('Input parameters file not specified')
             with open(in_params_path, 'rb') as f:
                 input_data = f.read()
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/provisioning_packet/provisioning_packet_mxs40v1.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning_packet/provisioning_packet_mxs40v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2022 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,21 +13,22 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import json
 import logging
-from .lib import HsmEntity
-from .lib import OemEntity
-from .lib import DeviceEntity
-from .lib import Crypto
-from cysecuretools.core.enums import ImageType
-from cysecuretools.core.strategy_context.prov_packet_strategy_ctx import (
-    ProvisioningPacketStrategy)
+
+from .lib.cyprov_hsm import HsmEntity
+from .lib.cyprov_oem import OemEntity
+from .lib.cyprov_dev import DeviceEntity
+from .lib.cyprov_crypto import Crypto
+from .....core.enums import ImageType
+from .....core.strategy_context import ProvisioningPacketStrategy
+
 
 # Default output values and paths
 PROV_IDENTITY_JWT = 'prov_identity.jwt'
 PROV_REQ_JWT = 'prov_req.jwt'
 ROT_AUTH_JWT = 'rot_auth.jwt'
 PROV_CMD_JWT = 'prov_cmd.jwt'
 PROV_PRIV_KEY_JWT = 'prov_priv_key.jwt'
@@ -37,14 +39,15 @@
 CUSTOMER_KEY_N = 5
 PROD_NAME = 'my_thing'
 DEV_NAME = "my_device"
 logger = logging.getLogger(__name__)
 
 
 class ProvisioningPacketMXS40v1(ProvisioningPacketStrategy):
+    """Provisioning packet generator for MXS40v1 platform"""
 
     def __init__(self, policy_parser):
         self.policy_parser = policy_parser
 
     def create(self, target, **kwargs):
         """
         Generates provisioning JWT packet.
@@ -171,41 +174,47 @@
         Crypto.dump_jwt(prov_cmd, prov_jwt_path)
 
         logger.info('#' * 70)
         logger.info('Provisioning packet is created')
         logger.info('#' * 70)
         return True
 
+    def verify(self, target, **kwargs):
+        """N/A for the MXS40v1 platform"""
+        raise NotImplementedError
+
+    def create_package(self, target, **kwargs):
+        """N/A for MXS40v1 platform"""
+        raise NotImplementedError
+
     def reverse_conversion(self, target, packets, output):
         raise NotImplementedError
 
     def _abs_path(self, path):
         """
         Converts policy related path to the absolute.
         """
         if os.path.isabs(path):
             return path
-        else:
-            rel_path = os.path.join(self.policy_parser.policy_dir, path)
-            return os.path.abspath(rel_path)
+        rel_path = os.path.join(self.policy_parser.policy_dir, path)
+        return os.path.abspath(rel_path)
 
     def _get_custom_keys(self):
         json_key_paths = []
         for image_type in [ImageType.BOOT,
                            ImageType.UPGRADE,
                            ImageType.BOOTLOADER]:
             keys = self.policy_parser.get_keys(image_type=image_type)
             for key in keys:
                 json_key_path = key.json_key
                 if not os.path.isfile(json_key_path):
                     logger.error("Cannot find the key '%s'", json_key_path)
                     return None
-                else:
-                    if json_key_path not in json_key_paths:
-                        json_key_paths.append(json_key_path)
+                if json_key_path not in json_key_paths:
+                    json_key_paths.append(json_key_path)
         return json_key_paths
 
     @staticmethod
     def _get_image_certificate(target):
         """ Gets bootloader image certificate """
         image_cert = target.bootloader_provider.jwt_path()
         if not os.path.isfile(image_cert):
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/__init__.py` & `cysecuretools-5.0.0/src/execute/silicon_data_reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """
-Copyright 2022 Cypress Semiconductor Corporation (an Infineon company)
+Copyright 2022-2023 Cypress Semiconductor Corporation (an Infineon company)
 or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .silicon_data_reader_mxs40v1 import SiliconDataReaderMXS40v1
-from .silicon_data_reader_mxs40sv2 import SiliconDataReaderMXS40Sv2
 
 
 def si_rev_name(revision_id):
     """Gets silicon revision name based on revision ID (e.g. 0x12 = A1)"""
     letters = 'ABCDEF'
     numbers = '012345678'
     hexadecimal = f'{revision_id:02x}'
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40sv2.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/silicon_data_reader_mxs40sv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,15 +13,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import logging
 from collections import namedtuple
 
-from cysecuretools.core.bitops import get_bits
+from ....core.bitops import get_bits
 
 logger = logging.getLogger(__name__)
 
 
 class SiliconDataReaderMXS40Sv2:
     """ Implements reading data from the devices on MXS40Sv2 platform """
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/silicon_data_reader/silicon_data_reader_mxs40v1.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/silicon_data_reader_mxs40v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,52 +11,53 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import logging
 from collections import namedtuple
-from .. provisioning_packet.lib import Crypto
-from .. provisioning.provision_device_mxs40v1 import read_silicon_data
-from ... targets.common.p64.silicon_data_parser import SiliconDataParser
+
+from .provisioning import provision_device_mxs40v1
+from .silicon_data_parser import SiliconDataParser
+from ....execute import jwt
 
 logger = logging.getLogger(__name__)
 
 
 class SiliconDataReaderMXS40v1:
     def __init__(self, target):
         self.target = target
 
     def read_die_id(self, tool):
-        data = read_silicon_data(tool, self.target)
+        data = provision_device_mxs40v1.read_silicon_data(tool, self.target)
         if data is None:
             logger.error('Failed to read silicon data')
             return None
         parser = SiliconDataParser(data)
         try:
             die_id = parser.get_die_id()
         except KeyError:
             logger.error('Invalid response. \'die_id\' field not found')
         return die_id
 
     def read_complete_status(self, tool):
-        data = read_silicon_data(tool, self.target)
+        data = provision_device_mxs40v1.read_silicon_data(tool, self.target)
         if data is None:
             logger.error('Failed to read silicon data')
             return None
         parser = SiliconDataParser(data)
         try:
             complete = parser.get_complete_status()
         except KeyError:
             logger.error('Invalid response. \'complete\' field not found')
         return complete
 
     def read_device_info(self, tool):
-        jwt_text = Crypto.read_jwt(self.target.entrance_exam.entrance_exam_jwt)
-        json_data = Crypto.readable_jwt(jwt_text)
+        jwt_text = jwt.read_jwt(self.target.entrance_exam.entrance_exam_jwt)
+        json_data = jwt.readable_jwt(jwt_text)
         payload = json_data['payload']
         silicon_id = None
         silicon_rev = None
         family_id = None
         for item in payload['ahb_reads']:
             if item['description'].startswith('SI_ID'):
                 address = int(item['address'], 0)
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/sys_call.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/provisioning/sys_call.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import logging
 from time import sleep
 
-from cysecuretools.core.enums import RegionHashStatus
-import cysecuretools.data.mxs40v1.mxs40v1_sfb_status_codes as sfb_status
+from .....core.enums import RegionHashStatus
+from .....data.mxs40v1 import mxs40v1_sfb_status_codes as sfb_status
 
 # SysCall operation codes
 READ_SILICON_ID_OPCODE = 0x00
 READ_SILICON_ID_COMM = 0x01
 REGION_HASH_OPCODE = 0x31
 PROVISIONING_OPCODE = 0x33
 ENCRYPTED_PROGRAMMING_OPCODE = 0x34
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/version_provider/version_provider_mxs40v1.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/version_provider_mxs40v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2020-2023 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -16,43 +17,39 @@
 import os
 import logging
 from os import path
 
 import json
 from packaging import version
 
-from cysecuretools import __path__ as site_packages
-from cysecuretools.version import __version__
-from cysecuretools.core.project import ProjectInitializer
-from cysecuretools.execute.image_cert import ImageCertificate
-from cysecuretools.execute.silicon_data_reader import si_rev_name
-from cysecuretools.execute.bootloader_provider_mxs40v1 import (
-    BootloaderProviderMXS40v1)
+from . import __path__ as site_packages
+from .image_cert import ImageCertificate
+from ....__about__ import __version__, __pkg_name__
+from ....core.project_base import ProjectInitializerBase
+from ....execute.silicon_data_reader import si_rev_name
+from ....core.version_provider import VersionProvider
 
 logger = logging.getLogger(__name__)
 
 
-class VersionProviderMXS40v1:
+class VersionProviderMXS40v1(VersionProvider):
     """
     Helper class that encapsulates the routine for getting a version
     of different parts of the package
     """
 
     CST_2_1_0_SFB_VER = '4.0.1.1267'
 
-    def __init__(self, target):
-        self.target = target
-
     def package_bootloader_version(self):
         """
         Gets a bootloader version bundled with the package
         :return: Version of the cybootloader bundled with the package
         """
-        bootloader = BootloaderProviderMXS40v1(self.target)
-        jwt_path = bootloader.jwt_path(build_mode='release', from_project=False)
+        jwt_path = self.target.bootloader_provider.jwt_path(
+            build_mode='release', from_project=False)
 
         ver = 'unknown'
         if not os.path.isfile(jwt_path):
             logger.error('File %s not found', jwt_path)
         else:
             try:
                 ver = ImageCertificate.get_version(jwt_path)
@@ -63,18 +60,18 @@
 
     def project_bootloader_version(self):
         """
         Gets a bootloader version in the project dir
         :return: Version of the cybootloader from the project if it was
                  initialized, otherwise None
         """
-        bootloader = BootloaderProviderMXS40v1(self.target)
-        jwt_path = bootloader.jwt_path(build_mode='release', from_project=True)
+        jwt_path = self.target.bootloader_provider.jwt_path(
+            build_mode='release', from_project=True)
 
-        if ProjectInitializer.is_project():
+        if ProjectInitializerBase.is_project():
             ver = 'unknown'
             if not os.path.isfile(jwt_path):
                 logger.error('File %s not found', jwt_path)
             else:
                 try:
                     ver = ImageCertificate.get_version(jwt_path)
                     logger.debug('Project bootloader version: %s', ver)
@@ -109,25 +106,25 @@
         """
         bootloader_ver = self.device_bootloader_version(tool)
         sfb_ver = self.device_sfb_version(tool)
         print('\tDevice:')
         print(f'\t\tCyBootloader: {bootloader_ver}')
         print(f'\t\tSecure Flash Boot: {sfb_ver}')
 
-    def print_version(self):
+    def print_version(self,  **_):
         """
         Prints the package version and CyBootloader version bundled with
         the package for the specified targets. Find installation source
         and build version information in verbose mode [-v] [--verbose]
         """
         package_ver = self.package_bootloader_version()
-        print(f'\nCySecureTools: {__version__}')
+        print(f'\n{__pkg_name__}: {__version__}')
         print('\tPackage:')
         print(f'\t\tCyBootloader: {package_ver}')
-        if ProjectInitializer.is_project():
+        if ProjectInitializerBase.is_project():
             project_ver = self.project_bootloader_version()
             print('\tProject:')
             print(f'\t\tCyBootloader: {project_ver}')
 
         direct_url = os.path.join(
             f'{site_packages[0]}-{__version__}.dist-info', 'direct_url.json')
         logger.debug(
@@ -162,20 +159,24 @@
         logger.info('Device CyBootloader version: %s', dev_bootloader_ver)
 
         pkg_bootloader_ver = self.package_bootloader_version()
         logger.info('Package CyBootloader version: %s', pkg_bootloader_ver)
 
         self.target.entrance_exam.log_protection_state(tool)
 
-    def check_compatibility(self, tool, check_si_rev=True):
+    def check_compatibility(self, tool, **kwargs):
         """Checks HW compatibility
         @param tool: OCD tool used for communication
         @param check_si_rev: Indicates whether to check silicon revision
         @return True if compatible, otherwise False
         """
+        if 'check_si_rev' in kwargs:
+            check_si_rev = kwargs.get('check_si_rev')
+        else:
+            check_si_rev = True
         result = self._verify_fw_version(tool)
         dev_info = self.target.silicon_data_reader.read_device_info(tool)
         result &= self._verify_silicon_family(dev_info.family_id)
         if result and check_si_rev:
             result &= self._verify_silicon_revision(dev_info.silicon_rev)
         return result
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/lvd_voltage_picker.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/voltage_tool/lvd_voltage_picker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,16 +12,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import logging
 from time import sleep
-from cysecuretools.execute.programmer.base import AP
-from cysecuretools.core.target_director import Target
+
+from .....execute.programmer.base import AP
+from .....core.target_director import Target
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_EFUSE_VOLTAGE = 2.5
 
 
 class LvdVoltagePicker:
```

### Comparing `cysecuretools-4.2.0/cysecuretools/execute/voltage_tool/voltage_tool_mxs40v1.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/voltage_tool/voltage_tool_mxs40v1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import logging
-from cysecuretools.core.target_director import Target
-from cysecuretools.core.voltage_tool import VoltageTool
+
 from .lvd_voltage_picker import LvdVoltagePicker
+from .....core.target_director import Target
+from .....core.voltage_tool import VoltageTool
 
 logger = logging.getLogger(__name__)
 
 
 class VoltageToolMXS40v1(VoltageTool, LvdVoltagePicker):
     """ Implementation of reading voltage for MXS40v1 platform """
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/asset.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset_builder.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/asset_builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.targets.common.mxs40sv2.asset import Asset
-from cysecuretools.targets.cyw20829.flows.asset_map import asset_map
+from .asset import Asset
 
 
 class AssetBuilder:
-    def __init__(self, policy_parser, assets_list, **kwargs):
+    def __init__(self, policy_parser, assets_list, asset_map, **kwargs):
         self.assets_dict = {}
-        self.all_assets = asset_map(policy_parser, **kwargs)
+        self.all_assets = asset_map.get(policy_parser, **kwargs)
         for item in assets_list:
             self.assets_dict[item] = self.all_assets[item]
 
     def get_assets(self):
         """
         Creates a list of assets and sort it by order
         :return: Return a byte-array value representing a value of single Asset
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/asset_enums.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/asset_enums.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
 from enum import Enum, IntEnum
 
+
 ApPermission = Enum(
     value='Permissions',
     names=[
         ('Enable', 0),
         ('Disable', 1),
         ('Permanently Disable', 2),
         ('None', 0),
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/access_restrictions_validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core.dependecy_validator import DependencyValidator
-from cysecuretools.targets.common.mxs40sv2 import asset_enums as enums
+from ...mxs40sv2 import asset_enums as enums
+from .....core.dependecy_validator import DependencyValidator
 
 
 class AccessRestrictionsValidator(DependencyValidator):
     def validate(self):
 
         def verify():
             if mpc_ppc_permission == enums.MpcPpcPermission['Disable']:
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/encryption_key_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core.dependecy_validator import DependencyValidator
+from .....core.dependecy_validator import DependencyValidator
 
 
 class EncryptionAndProgramOemKey1Validator(DependencyValidator):
     def validate(self):
         _pp = self.policy_parser
 
         encryption = _pp.get_encryption()
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/hci_mode_validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2022 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.targets.common.mxs40sv2 import asset_enums as enums
-from cysecuretools.core.dependecy_validator import DependencyValidator
 from ..enums import PolicyType
+from ...mxs40sv2 import asset_enums as enums
+from .....core.dependecy_validator import DependencyValidator
 
 
 class HciModeValidator(DependencyValidator):
+    """Dependencies validator for HCI mode settings"""
+
     def validate(self):
+        """Validates dependencies between policy properties"""
         _pp = self.policy_parser
 
-        policy_type = _pp.get_policy_type()
+        policy_type = _pp.policy_type()
 
         if policy_type == PolicyType.HCI_SECURE:
             dead_cm33 = _pp.get_dead_cm33_permission()
             cm33 = _pp.get_cm33_permission()
             smif = _pp.get_smif_configuration()
             lifecycle = _pp.get_target_lcs()
 
@@ -37,11 +41,11 @@
             if cm33 == enums.ApPermission['Enable']:
                 self.add_msg('For the HCI mode CM33 AP must be "Disabled"')
 
             if smif != enums.SMIFConfiguation['HCI mode']:
                 self.add_msg('For the HCI mode smif configuration '
                              'must be "HCI mode"')
 
-            if lifecycle != enums.LifecycleStage['SECURE'] and \
-                    lifecycle != enums.LifecycleStage['NORMAL']:
+            if lifecycle not in (enums.LifecycleStage['SECURE'],
+                                 enums.LifecycleStage['NORMAL']):
                 self.add_msg('For the HCI mode target_lcs must be "SECURE"'
                              ' or "NORMAL"')
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/nv_counter_validator.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/nv_counter_validator.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/pre_build_keys_exist_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
-from cysecuretools.core.dependecy_validator import DependencyValidator
+
+from .....core.dependecy_validator import DependencyValidator
 
 
 class PreBuildKeysExistValidator(DependencyValidator):
     def validate(self):
         _pp = self.policy_parser
 
         pub_key_0 = _pp.get_program_oem_key_0_hash()
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/dependencies_validator/revoke_oem_encryption_validator.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core.dependecy_validator import DependencyValidator
+from .....core.dependecy_validator import DependencyValidator
 
 
 class RevocationAndEncryptionValidator(DependencyValidator):
     def validate(self):
         _pp = self.policy_parser
 
         encryption = _pp.get_encryption()
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/enums.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/enums.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/flow_parser.py` & `cysecuretools-5.0.0/src/targets/common/flow_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import importlib
-from cysecuretools.core.json_helper import read_json
+
+from ...core.json_helper import read_json
 
 
 class FlowParser:
     """ Implements searching data in the provisioning flow map """
 
     def __init__(self, target, test_pkg_type=None):
         self.test_packages = target.test_packages
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/json/cyw20829_no_secure.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_no_secure.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/json/cyw20829_reprovisioning_secure.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/json/cyw20829_secure.json_schema` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/json/cyw20829_secure.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/nv_counter_calc.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/nv_counter_calc.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/mxs40sv2/policy_parser.py` & `cysecuretools-5.0.0/src/targets/common/mxs40sv2/policy_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import json
 from pathlib import Path
+
 from . import asset_enums as enums
+from ....core import PolicyParserBase
 
 
-class PolicyParser:
+class PolicyParser(PolicyParserBase):
     """
     Provides functionality for searching data in the package policy.
     """
     def __init__(self, policy_file):
         """
         Creates instance of policy parser.
         :param policy_file: Path to policy file.
@@ -49,15 +51,15 @@
             try:
                 data = json.loads(file_content)
             except json.decoder.JSONDecodeError as e:
                 msg = f"Failed to parse policy '{filename}': {e.args[0]}"
                 raise json.decoder.JSONDecodeError(msg, e.doc, e.pos)
         return data
 
-    def get_policy_type(self):
+    def policy_type(self):
         try:
             return self.json['policy']['type']
         except KeyError as e:
             raise KeyError(
                 f'Policy type not specified ({self.policy_file})') from e
 
     def get_pub_key_0_path(self):
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/p64/enums.py` & `cysecuretools-5.0.0/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,14 @@
-"""
-Copyright (c) 2020-2021 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-"""
-from enum import IntEnum
-
-
-class ProtectionState(IntEnum):
-    """ Device protection states """
-    unknown = 0
-    virgin = 1
-    normal = 2
-    secure = 3
-    dead = 4
-
-
-class KeyId(IntEnum):
-    HSM = 4
-    OEM = 5
-    DEVICE = 1
-    GROUP = 12
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/p64/json/policy_template.json` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/json/policy_template.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/p64/json/schema.json_schema` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/json/schema.json_schema`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_filter.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/policy_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 limitations under the License.
 """
 import os
 import errno
 import json
 import copy
 import logging
-from cysecuretools.core import PolicyFilterBase
+
+from ....core import PolicyFilterBase
 
 logger = logging.getLogger(__name__)
 
 
 class PolicyFilter(PolicyFilterBase):
     def __init__(
             self, policy_parser, policy_template='json/policy_template.json'):
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_parser.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/policy_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import json
 from pathlib import Path
-from cysecuretools.core import MemoryArea, KeyData
-from cysecuretools.core.enums import KeyType, ImageType
-from cysecuretools.execute.key_reader import load_key, jwk_to_pem
-from cysecuretools.targets.common.p64.enums import KeyId
+
+from .enums import KeyId
+from ....core import MemoryArea, KeyData
+from ....core.enums import KeyType, ImageType
+from ....execute import key_reader
+from ....core import key_helper
 
 
 class PolicyParser:
-    """
-    Provides functionality for searching data in cysecuretools policy.
-    """
+    """Provides functionality for searching data in a policy files"""
+
     def __init__(self, policy):
         """
         Creates instance of policy parser.
         :param policy: Either path to policy file or policy dictionary
         """
         self.json = None
         self.policy_dir = None
@@ -378,26 +379,26 @@
             use_key = False
         return use_key
 
     def private_key(self, key_path):
         if not os.path.isabs(key_path):
             key_path = os.path.abspath(os.path.join(self.policy_dir, key_path))
         try:
-            private_jwk, _ = load_key(key_path)
-            private_pem = jwk_to_pem(private_jwk, private_key=True)
+            private_jwk, _ = key_reader.load_key(key_path)
+            private_pem = key_helper.jwk_to_pem(private_jwk, private_key=True)
         except (FileNotFoundError, AttributeError):
             private_jwk, private_pem = None, None
         return private_jwk, private_pem
 
     def public_key(self, key_path):
         if not os.path.isabs(key_path):
             key_path = os.path.abspath(os.path.join(self.policy_dir, key_path))
         try:
-            _, public_jwk = load_key(key_path)
-            public_pem = jwk_to_pem(public_jwk)
+            _, public_jwk = key_reader.load_key(key_path)
+            public_pem = key_helper.jwk_to_pem(public_jwk)
         except FileNotFoundError:
             public_jwk, public_pem = None, None
         return public_jwk, public_pem
 
     def abs_policy_path(self, path):
         """ Converts policy relative path to the absolute """
         if not os.path.isabs(path):
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/p64/policy_validator.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/policy_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 """
 import jsonschema
 import logging
 import json
 import os.path
 from math import ceil
 from collections import namedtuple
-from cysecuretools.targets.common.p64.policy_parser import ImageType
-from cysecuretools.core import PolicyValidatorBase
-from cysecuretools.core.enums import ValidationStatus
-from cysecuretools.execute.key_reader import load_key
+
+from .policy_parser import ImageType
+from ....core import PolicyValidatorBase
+from ....core.enums import ValidationStatus
+from ....execute.key_reader import load_key
 
 MODULE_PATH = os.path.dirname(os.path.realpath(__file__))
 POLICY_SCHEMA = os.path.join(MODULE_PATH, 'json', 'schema.json_schema')
 
 logger = logging.getLogger(__name__)
 
 
@@ -44,15 +45,15 @@
         self.parser = policy_parser
         self.memory_map = memory_map
         self.policy_dir = self.parser.policy_dir
         self.stage = None
         self.is_smif = None
         self.is_multi_image = None
 
-    def validate(self, skip=None, skip_prompts=False):
+    def validate(self, skip=None, skip_prompts=False, **kwargs):
         """
         Validation of policy.json.
         :param skip: Validators to skip (e.g. pre_build, dap_disabling)
         :param skip_prompts: Indicates whether to skip interactive prompts
         :return Validation status
         """
         status = ValidationStatus.OK
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/common/p64/silicon_data_parser.py` & `cysecuretools-5.0.0/src/targets/common/mxs40v1/silicon_data_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """
-Copyright (c) 2019 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.execute.provisioning_packet.lib import Crypto
+from ....execute.jwt import readable_jwt
 
 
 class SiliconDataParser:
     @property
     def jwt(self):
         return self._jwt
 
     @jwt.setter
     def jwt(self, jwt):
         self._jwt = jwt
 
     @property
     def data(self):
         if self._data is None:
-            self._data = Crypto.readable_jwt(self.jwt)
+            self._data = readable_jwt(self.jwt)
         return self._data
 
     def __init__(self, jwt=None):
         self._jwt = jwt
-        self._data = Crypto.readable_jwt(jwt) if jwt is not None else None
+        self._data = readable_jwt(jwt) if jwt is not None else None
 
     def get_die_id(self):
         return self.data['payload']['die_id']
 
     def get_serial(self):
         die_id = self.get_die_id()
         concat = ''.join(str(x) for x in die_id.values())
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/memory_map.py` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/maps/memory_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core import MemoryMapBaseP64
+from ....core import MemoryMapBaseP64
 
 
-class MemoryMap_cyb06xx5(MemoryMapBaseP64):
+class MemoryMapCYB06xx5(MemoryMapBaseP64):
     @property
     def FLASH_ADDRESS(self):
         return 0x10000000
 
     @property
     def FLASH_SIZE(self):
         return 0x00070000
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/maps/register_map.py` & `cysecuretools-5.0.0/src/targets/cyb06xxa/maps/register_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core import RegisterMapBaseP64
+from ....core import RegisterMapBaseP64
 
 
-class RegisterMap_cyb06xx5(RegisterMapBaseP64):
+class RegisterMap_cyb06xxa(RegisterMapBaseP64):
 
     #
     #  Entrance exam registers and constants
     #
 
     @property
     def ENTRANCE_EXAM_FW_STATUS_REG(self):
-        return 0x0803e000
+        return 0x080fe000
 
     @property
     def ENTRANCE_EXAM_FW_STATUS_VAL(self):
         return 0xF0000000
 
     @property
     def ENTRANCE_EXAM_FW_STATUS_RE_VAL(self):
@@ -36,27 +36,27 @@
 
     @property
     def ENTRANCE_EXAM_FW_STATUS_MASK(self):
         return 0xF0800000
 
     @property
     def ENTRANCE_EXAM_SRAM_ADDR(self):
-        return 0x0802c000
+        return 0x080ec000
 
     @property
     def ENTRANCE_EXAM_SRAM_SIZE(self):
         return 0x00004000
 
     @property
     def ENTRANCE_EXAM_REGION_HASH_ADDR(self):
         return 0x10000000
 
     @property
     def ENTRANCE_EXAM_REGION_HASH_SIZE(self):
-        return 0x00070000
+        return 0x001e0000
 
     @property
     def ENTRANCE_EXAM_REGION_HASH_MODE(self):
         return 255
 
     @property
     def ENTRANCE_EXAM_REGION_HASH_EXPECTED_VAL(self):
@@ -101,7 +101,8 @@
     @property
     def CYREG_IPC2_STRUCT_LOCK_STATUS(self):
         return 0x4022005C
 
     @property
     def CYREG_EFUSE_SECURE_HASH(self):
         return 0x402c0814
+
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/cy_auth_512k_b0_sample.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/packets/cy_auth_512k_b0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/packets/entrance_exam.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4.json` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9814453125%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'bootloader_keys': {0: {'key': "*

 * *                   "'../../common/mxs40v1/prebuilt/oem_state.json'}}}}}",*

 * * "'pre_build'": "{'oem_public_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'oem_private_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'hsm_public_key': '../../common/mxs40v1/prebuilt/hsm_state.json', "*

 * *                "'hsm_private_key': '../../common/mxs40v1/prebuilt/hsm_state.json'}"}*

```diff
@@ -4,15 +4,15 @@
             {
                 "acq_win": 100,
                 "boot_auth": [
                     5
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/p64/prebuilt/oem_state.json",
+                        "key": "../../common/mxs40v1/prebuilt/oem_state.json",
                         "kid": 5
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
@@ -161,18 +161,18 @@
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
         "cy_auth": "../packets/cy_auth_512k_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_multi_CM0_CM4_smif.json` & `cysecuretools-5.0.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9724874614197532%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'boot_auth': [3], 'bootloader_keys': {0: {'kid': 3, 'key': "*

 * *                   "'../keys/cy_pub_key.json'}}, 'wdt_enable': True, 'resources': {0: {'address': "*

 * *                   "270336000}, 1: {'address': 135135232}, 2: {'address': 135184384}, insert: [(3, "*

 * *                   "OrderedDict([('type', 'STATUS_PARTITION'), ('address', 270303232), ('size', "*

 * *                   "32768)])), (4, OrderedDict([('type', 'SCRATCH'), ('address', 405274624), "*

 * *                    […]*

```diff
@@ -1,46 +1,58 @@
 {
     "boot_upgrade": {
         "firmware": [
             {
                 "acq_win": 100,
                 "boot_auth": [
-                    5
+                    3
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/p64/prebuilt/oem_state.json",
-                        "kid": 5
+                        "key": "../keys/cy_pub_key.json",
+                        "kid": 3
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
                 "protect_flags": 1,
                 "reset_after_failure": 0,
                 "resources": [
                     {
-                        "address": 268828672,
+                        "address": 270336000,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
                     {
-                        "address": 134348800,
+                        "address": 135135232,
                         "size": 65536,
                         "type": "SRAM_SPM_PRIV"
                     },
                     {
-                        "address": 134397952,
+                        "address": 135184384,
                         "size": 16384,
                         "type": "SRAM_DAP"
+                    },
+                    {
+                        "address": 270303232,
+                        "size": 32768,
+                        "type": "STATUS_PARTITION"
+                    },
+                    {
+                        "address": 405274624,
+                        "size": 524288,
+                        "type": "SCRATCH"
                     }
                 ],
                 "upgrade": false,
-                "wdt_enable": false
+                "upgrade_mode": "swap",
+                "wdt_enable": true,
+                "wdt_timeout": 4000
             },
             {
                 "acq_win": 100,
                 "boot_auth": [
                     8
                 ],
                 "boot_keys": [
@@ -54,28 +66,31 @@
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
                 "monotonic": 0,
                 "multi_image": 1,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 131072,
+                        "size": 933888,
                         "type": "BOOT"
                     },
                     {
-                        "address": 402653184,
-                        "size": 131072,
+                        "address": 402768384,
+                        "size": 933888,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
+                "set_img_ok": true,
                 "smif_id": 1,
+                "smif_sector_size": 262144,
                 "upgrade": true,
                 "version": "0.1",
-                "wdt_enable": false
+                "wdt_enable": false,
+                "wdt_timeout": 4000
             },
             {
                 "boot_auth": [
                     8
                 ],
                 "boot_keys": [
                     {
@@ -87,34 +102,35 @@
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
                 "multi_image": 2,
                 "resources": [
                     {
-                        "address": 268566528,
-                        "size": 262144,
+                        "address": 269369344,
+                        "size": 933888,
                         "type": "BOOT"
                     },
                     {
-                        "address": 402915328,
-                        "size": 262144,
+                        "address": 404079104,
+                        "size": 933888,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 1,
+                "smif_sector_size": 262144,
                 "upgrade": true,
                 "version": "0.1"
             }
         ],
         "reprogram": [
             {
                 "size": 65536,
-                "start": 268828672
+                "start": 270336000
             }
         ],
         "reprovision": {
             "boot_loader": true,
             "keys_and_policies": true
         },
         "title": "upgrade_policy"
@@ -158,21 +174,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_512k_b0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_2m_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4.json` & `cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9738610789609053%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'bootloader_keys': {0: {'key': "*

 * *                   "'../../common/mxs40v1/prebuilt/oem_state.json'}}, 'resources': {0: {'address': "*

 * *                   "269287424}}, delete: ['reset_after_failure']}, 1: {'resources': {0: {'size': "*

 * *                   "425984}, 1: {'address': 268861440, 'size': 425984}}}, 2: {'resources': {0: "*

 * *                   "{'size': 360448}}}}, 'reprogram': {0: {'start': 269287424}}}",*

 * * "'pre_build'": "{'oem_public_key': '../../common/mxs40v1/pre […]*

```diff
@@ -4,27 +4,26 @@
             {
                 "acq_win": 100,
                 "boot_auth": [
                     5
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/p64/prebuilt/oem_state.json",
+                        "key": "../../common/mxs40v1/prebuilt/oem_state.json",
                         "kid": 5
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
                 "protect_flags": 1,
-                "reset_after_failure": 0,
                 "resources": [
                     {
-                        "address": 268828672,
+                        "address": 269287424,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
                     {
                         "address": 134348800,
                         "size": 65536,
                         "type": "SRAM_SPM_PRIV"
@@ -54,20 +53,20 @@
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
                 "launch": 16,
                 "monotonic": 0,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 196608,
+                        "size": 425984,
                         "type": "BOOT"
                     },
                     {
-                        "address": 268632064,
-                        "size": 196608,
+                        "address": 268861440,
+                        "size": 425984,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 0,
                 "upgrade": true,
                 "version": "0.1",
@@ -87,28 +86,28 @@
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
                 "resources": [
                     {
                         "address": 268500992,
-                        "size": 131072,
+                        "size": 360448,
                         "type": "BOOT"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 0,
                 "upgrade": false,
                 "version": "0.1"
             }
         ],
         "reprogram": [
             {
                 "size": 65536,
-                "start": 268828672
+                "start": 269287424
             }
         ],
         "reprovision": {
             "boot_loader": true,
             "keys_and_policies": true
         },
         "title": "upgrade_policy"
@@ -152,21 +151,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_512k_b0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_1m_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/policy/policy_single_CM0_CM4_smif.json` & `cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9728387951586738%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'bootloader_keys': {0: {'key': "*

 * *                   "'../../common/mxs40v1/prebuilt/oem_state.json'}}, 'resources': {0: {'address': "*

 * *                   "269287424}}, delete: ['reset_after_failure']}, 1: {'resources': {0: {'size': "*

 * *                   "262144}, 1: {'size': 262144}}, 'multi_image': 1, delete: ['launch']}, 2: "*

 * *                   "{'smif_id': 1, 'upgrade': True, 'resources': {0: {'address': 268697600, "*

 * *                   "'size': 589824}, insert: [(1, Or […]*

```diff
@@ -4,27 +4,26 @@
             {
                 "acq_win": 100,
                 "boot_auth": [
                     5
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/p64/prebuilt/oem_state.json",
+                        "key": "../../common/mxs40v1/prebuilt/oem_state.json",
                         "kid": 5
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
                 "protect_flags": 1,
-                "reset_after_failure": 0,
                 "resources": [
                     {
-                        "address": 268828672,
+                        "address": 269287424,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
                     {
                         "address": 134348800,
                         "size": 65536,
                         "type": "SRAM_SPM_PRIV"
@@ -49,25 +48,25 @@
                         "kid": 8
                     }
                 ],
                 "encrypt": false,
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
-                "launch": 16,
                 "monotonic": 0,
+                "multi_image": 1,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 393216,
+                        "size": 262144,
                         "type": "BOOT"
                     },
                     {
                         "address": 402653184,
-                        "size": 393216,
+                        "size": 262144,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 1,
                 "upgrade": true,
                 "version": "0.1",
@@ -84,31 +83,37 @@
                     }
                 ],
                 "encrypt": false,
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
+                "multi_image": 2,
                 "resources": [
                     {
-                        "address": 268500992,
-                        "size": 327680,
+                        "address": 268697600,
+                        "size": 589824,
                         "type": "BOOT"
+                    },
+                    {
+                        "address": 402915328,
+                        "size": 589824,
+                        "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
-                "smif_id": 0,
-                "upgrade": false,
+                "smif_id": 1,
+                "upgrade": true,
                 "version": "0.1"
             }
         ],
         "reprogram": [
             {
                 "size": 65536,
-                "start": 268828672
+                "start": 269287424
             }
         ],
         "reprovision": {
             "boot_loader": true,
             "keys_and_policies": true
         },
         "title": "upgrade_policy"
@@ -152,21 +157,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_512k_b0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_1m_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx5/target_builder.py` & `cysecuretools-5.0.0/src/targets/cyb06xxa/target_builder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,69 +12,58 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 
-from cysecuretools.core import TargetBuilder
-from cysecuretools.core.enums import KeyAlgorithm
-from cysecuretools.targets.cyb06xx5.maps.memory_map import MemoryMap_cyb06xx5
-from cysecuretools.targets.cyb06xx5.maps.register_map import \
-    RegisterMap_cyb06xx5
-from cysecuretools.targets.common.p64.policy_filter import PolicyFilter
-from cysecuretools.targets.common.p64.policy_parser import PolicyParser
-from cysecuretools.targets.common.p64.policy_validator import PolicyValidator
-from cysecuretools.execute.provisioning import ProvisioningMXS40v1
-from cysecuretools.execute.provisioning_packet import ProvisioningPacketMXS40v1
-from cysecuretools.execute.entrance_exam.exam_mxs40v1 import \
-    EntranceExamMXS40v1
-from cysecuretools.execute.project_init.project_init_mxs40v1 import \
-    ProjectInitializerMXS40V1
-from cysecuretools.execute.voltage_tool.voltage_tool_mxs40v1 import VoltageToolMXS40v1
-from cysecuretools.execute.key_reader_mxs40v1 import KeyReaderMXS40V1
-from cysecuretools.execute.silicon_data_reader import SiliconDataReaderMXS40v1
-from cysecuretools.execute.image_signing.signtool_mxs40v1 import \
-    SignToolMXS40v1
-from cysecuretools.execute.key_source.key_source_mxs40v1 import (
-    KeySourceMXS40v1)
+from .maps.memory_map import MemoryMap_cyb06xxa
+from .maps.register_map import RegisterMap_cyb06xxa
+from ..common.mxs40v1 import (
+    PolicyFilter, PolicyParser, PolicyValidator, X509CertificateStrategyMXS40v1,
+    ProvisioningPacketMXS40v1, EntranceExamMXS40v1, SignToolMXS40v1,
+    KeySourceMXS40v1, ProjectInitializerMXS40V1, ProvisioningMXS40v1,
+    SiliconDataReaderMXS40v1, VersionProviderMXS40v1, VoltageToolMXS40v1,
+    BootloaderProviderMXS40v1, KeyReaderMXS40V1
+)
+from ...core import TargetBuilder
+from ...core.enums import KeyAlgorithm
 
 
-class CYB06xx5_Builder(TargetBuilder):
-    """ CYB06xx5 target builder """
+class CYB06xxA_Builder(TargetBuilder):
+    """ CYB06xxA target builder """
 
     def get_default_policy(self):
         return os.path.join(
-            self.target_dir, 'policy', 'policy_single_CM0_CM4.json')
+            self.target_dir, 'policy', 'policy_single_CM0_CM4_swap.json')
 
     def get_ocds(self):
-        return ['pyocd', 'openocd']
+        return ['openocd']
 
     def get_ocd_config(self):
         return {
             'openocd': {
                 'before_init': '',
                 'after_init': 'targets'
             }
         }
 
     def get_memory_map(self):
-        memory_map = MemoryMap_cyb06xx5()
+        memory_map = MemoryMap_cyb06xxa()
         return memory_map
 
     def get_register_map(self):
-        register_map = RegisterMap_cyb06xx5()
+        register_map = RegisterMap_cyb06xxa()
         return register_map
 
     def get_policy_parser(self, policy):
         policy_parser = PolicyParser(policy)
         return policy_parser
 
     def get_policy_validator(self, policy_parser, memory_map):
-
         policy_validator = PolicyValidator(policy_parser, memory_map)
         return policy_validator
 
     def get_policy_filter(self, policy_parser):
         policy_filter = PolicyFilter(policy_parser)
         return policy_filter
 
@@ -104,35 +94,33 @@
     def get_sign_tool(self):
         return SignToolMXS40v1
 
     def get_key_source(self, **kwargs):
         return KeySourceMXS40v1(kwargs['policy_parser'])
 
     def get_bootloader_provider(self):
-        from cysecuretools.execute.bootloader_provider_mxs40v1 import \
-            BootloaderProviderMXS40v1
         return BootloaderProviderMXS40v1
 
     def get_version_provider(self):
-        from cysecuretools.execute.version_provider.version_provider_mxs40v1 \
-            import VersionProviderMXS40v1
         return VersionProviderMXS40v1
 
     def get_debug_certificate(self):
         """ N/A for MXS40v1 platform """
         return None
 
     def get_policy_generator(self, policy_parser):
         """ N/A for MXS40v1 platform """
         return None
 
     def get_test_packages(self):
         """ N/A for MXS40v1 platform """
         return None
 
+    def get_certificate_strategy(self):
+        return X509CertificateStrategyMXS40v1()
+
+    def get_app_loader(self):
+        """ N/A for MXS40v1 platform """
+
     def get_silicon_id(self):
         """Gets the target silicon ID"""
-        return {
-            'id': [0xE701, 0xE70D],
-            'rev': [0x12],
-            'family': 0x105
-        }
+        return None
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/memory_map.py` & `cysecuretools-5.0.0/src/targets/cyb06xx7/maps/memory_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core import MemoryMapBaseP64
+from ....core import MemoryMapBaseP64
 
 
 class MemoryMap_cyb06xx7(MemoryMapBaseP64):
     @property
     def FLASH_ADDRESS(self):
         return 0x10000000
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/maps/register_map.py` & `cysecuretools-5.0.0/src/targets/cyb06xx7/maps/register_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core import RegisterMapBaseP64
+from ....core import RegisterMapBaseP64
 
 
 class RegisterMap_cyb06xx7(RegisterMapBaseP64):
 
     #
     #  Entrance exam registers and constants
     #
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xx7/packets/cy_auth_1m_b0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/packets/entrance_exam.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xx7/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json` & `cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9814420244107745%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'bootloader_keys': {0: {'key': "*

 * *                   "'../../common/mxs40v1/prebuilt/oem_state.json'}}}}}",*

 * * "'pre_build'": "{'oem_public_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'oem_private_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'hsm_public_key': '../../common/mxs40v1/prebuilt/hsm_state.json', "*

 * *                "'hsm_private_key': '../../common/mxs40v1/prebuilt/hsm_state.json'}"}*

```diff
@@ -4,15 +4,15 @@
             {
                 "acq_win": 100,
                 "boot_auth": [
                     5
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/p64/prebuilt/oem_state.json",
+                        "key": "../../common/mxs40v1/prebuilt/oem_state.json",
                         "kid": 5
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
@@ -160,18 +160,18 @@
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
         "cy_auth": "../packets/cy_auth_1m_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif.json` & `cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9803666927690365%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'bootloader_keys': {0: {'key': "*

 * *                   "'../../common/mxs40v1/prebuilt/oem_state.json'}}}, 1: {'resources': {0: "*

 * *                   "{'size': 851968}, 1: {'size': 851968}}, 'launch': 16, delete: "*

 * *                   "['multi_image']}, 2: {'smif_id': 0, 'upgrade': False, 'resources': {0: "*

 * *                   "{'address': 268500992, 'size': 786432}, delete: [1]}, delete: "*

 * *                   "['multi_image']}}}",*

 * * "'pre_build'": "{'oem_public_key': '../../co […]*

```diff
@@ -4,15 +4,15 @@
             {
                 "acq_win": 100,
                 "boot_auth": [
                     5
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/p64/prebuilt/oem_state.json",
+                        "key": "../../common/mxs40v1/prebuilt/oem_state.json",
                         "kid": 5
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
@@ -48,25 +48,25 @@
                         "kid": 8
                     }
                 ],
                 "encrypt": false,
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
+                "launch": 16,
                 "monotonic": 0,
-                "multi_image": 1,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 262144,
+                        "size": 851968,
                         "type": "BOOT"
                     },
                     {
                         "address": 402653184,
-                        "size": 262144,
+                        "size": 851968,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 1,
                 "upgrade": true,
                 "version": "0.1",
@@ -83,30 +83,24 @@
                     }
                 ],
                 "encrypt": false,
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
-                "multi_image": 2,
                 "resources": [
                     {
-                        "address": 268697600,
-                        "size": 589824,
+                        "address": 268500992,
+                        "size": 786432,
                         "type": "BOOT"
-                    },
-                    {
-                        "address": 402915328,
-                        "size": 589824,
-                        "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
-                "smif_id": 1,
-                "upgrade": true,
+                "smif_id": 0,
+                "upgrade": false,
                 "version": "0.1"
             }
         ],
         "reprogram": [
             {
                 "size": 65536,
                 "start": 269287424
@@ -160,18 +154,18 @@
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
         "cy_auth": "../packets/cy_auth_1m_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif_swap.json` & `cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_smif_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_multi_CM0_CM4_swap.json` & `cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_multi_CM0_CM4_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif.json` & `cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_swap.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9801666762680856%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'bootloader_keys': {0: {'key': "*

 * *                   "'../../common/prebuilt/oem_state.json'}}, 'wdt_enable': True, 'resources': "*

 * *                   "{insert: [(3, OrderedDict([('type', 'STATUS_PARTITION'), ('address', "*

 * *                   "269271040), ('size', 16384)])), (4, OrderedDict([('type', 'SCRATCH'), "*

 * *                   "('address', 269221888), ('size', 49152)]))]}, 'wdt_timeout': 4000, "*

 * *                   "'upgrade_mode': 'swap'}, 1: {'smif_id': 0, 'resource […]*

```diff
@@ -4,15 +4,15 @@
             {
                 "acq_win": 100,
                 "boot_auth": [
                     5
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/p64/prebuilt/oem_state.json",
+                        "key": "../../common/prebuilt/oem_state.json",
                         "kid": 5
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
@@ -28,18 +28,30 @@
                         "size": 65536,
                         "type": "SRAM_SPM_PRIV"
                     },
                     {
                         "address": 134397952,
                         "size": 16384,
                         "type": "SRAM_DAP"
+                    },
+                    {
+                        "address": 269271040,
+                        "size": 16384,
+                        "type": "STATUS_PARTITION"
+                    },
+                    {
+                        "address": 269221888,
+                        "size": 49152,
+                        "type": "SCRATCH"
                     }
                 ],
                 "upgrade": false,
-                "wdt_enable": false
+                "upgrade_mode": "swap",
+                "wdt_enable": true,
+                "wdt_timeout": 4000
             },
             {
                 "acq_win": 100,
                 "boot_auth": [
                     8
                 ],
                 "boot_keys": [
@@ -53,28 +65,30 @@
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
                 "launch": 16,
                 "monotonic": 0,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 851968,
+                        "size": 393216,
                         "type": "BOOT"
                     },
                     {
-                        "address": 402653184,
-                        "size": 851968,
+                        "address": 268828672,
+                        "size": 393216,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
-                "smif_id": 1,
+                "set_img_ok": true,
+                "smif_id": 0,
                 "upgrade": true,
                 "version": "0.1",
-                "wdt_enable": false
+                "wdt_enable": false,
+                "wdt_timeout": 4000
             },
             {
                 "boot_auth": [
                     8
                 ],
                 "boot_keys": [
                     {
@@ -86,15 +100,15 @@
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
                 "resources": [
                     {
                         "address": 268500992,
-                        "size": 786432,
+                        "size": 327680,
                         "type": "BOOT"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 0,
                 "upgrade": false,
                 "version": "0.1"
@@ -154,18 +168,18 @@
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
         "cy_auth": "../packets/cy_auth_1m_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif_swap.json` & `cysecuretools-5.0.0/src/targets/cyb06xx7/policy/policy_single_CM0_CM4_smif_swap.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/policy/policy_single_CM0_CM4_swap.json` & `cysecuretools-5.0.0/src/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9734471450617285%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'boot_auth': [3], 'bootloader_keys': {0: {'kid': 3, 'key': "*

 * *                   "'../keys/cy_pub_key.json'}}, 'resources': {0: {'address': 270336000}, 1: "*

 * *                   "{'address': 135135232}, 2: {'address': 135184384}, 3: {'address': 270303232, "*

 * *                   "'size': 32768}, 4: {'address': 405012480, 'size': 786432}}, "*

 * *                   "'reset_after_failure': 0}, 1: {'smif_id': 1, 'resources': {0: {'size': "*

 * *                   "1867776}, 1: {'address': […]*

```diff
@@ -1,50 +1,51 @@
 {
     "boot_upgrade": {
         "firmware": [
             {
                 "acq_win": 100,
                 "boot_auth": [
-                    5
+                    3
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../../common/prebuilt/oem_state.json",
-                        "kid": 5
+                        "key": "../keys/cy_pub_key.json",
+                        "kid": 3
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
                 "protect_flags": 1,
+                "reset_after_failure": 0,
                 "resources": [
                     {
-                        "address": 269287424,
+                        "address": 270336000,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
                     {
-                        "address": 134348800,
+                        "address": 135135232,
                         "size": 65536,
                         "type": "SRAM_SPM_PRIV"
                     },
                     {
-                        "address": 134397952,
+                        "address": 135184384,
                         "size": 16384,
                         "type": "SRAM_DAP"
                     },
                     {
-                        "address": 269271040,
-                        "size": 16384,
+                        "address": 270303232,
+                        "size": 32768,
                         "type": "STATUS_PARTITION"
                     },
                     {
-                        "address": 269221888,
-                        "size": 49152,
+                        "address": 405012480,
+                        "size": 786432,
                         "type": "SCRATCH"
                     }
                 ],
                 "upgrade": false,
                 "upgrade_mode": "swap",
                 "wdt_enable": true,
                 "wdt_timeout": 4000
@@ -65,26 +66,27 @@
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
                 "launch": 16,
                 "monotonic": 0,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 393216,
+                        "size": 1867776,
                         "type": "BOOT"
                     },
                     {
-                        "address": 268828672,
-                        "size": 393216,
+                        "address": 402883584,
+                        "size": 1867776,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "set_img_ok": true,
-                "smif_id": 0,
+                "smif_id": 1,
+                "smif_sector_size": 262144,
                 "upgrade": true,
                 "version": "0.1",
                 "wdt_enable": false,
                 "wdt_timeout": 4000
             },
             {
                 "boot_auth": [
@@ -100,28 +102,28 @@
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
                 "resources": [
                     {
                         "address": 268500992,
-                        "size": 327680,
+                        "size": 1802240,
                         "type": "BOOT"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 0,
                 "upgrade": false,
                 "version": "0.1"
             }
         ],
         "reprogram": [
             {
                 "size": 65536,
-                "start": 269287424
+                "start": 270336000
             }
         ],
         "reprovision": {
             "boot_loader": true,
             "keys_and_policies": true
         },
         "title": "upgrade_policy"
@@ -165,21 +167,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_1m_b0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_2m_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex` & `cysecuretools-5.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_Release/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex` & `cysecuretools-5.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xx7/prebuilt/CyBootloader_WithLogs/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/memory_map.py` & `cysecuretools-5.0.0/src/targets/cyb06xxa/maps/memory_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core import MemoryMapBaseP64
+from ....core import MemoryMapBaseP64
 
 
 class MemoryMap_cyb06xxa(MemoryMapBaseP64):
     @property
     def FLASH_ADDRESS(self):
         return 0x10000000
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/maps/register_map.py` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/maps/register_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
-Copyright (c) 2019-2020 Cypress Semiconductor Corporation
+Copyright (c) 2022 Cypress Semiconductor Corporation
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core import RegisterMapBaseP64
+from ....core import RegisterMapBaseP64
 
 
-class RegisterMap_cyb06xxa(RegisterMapBaseP64):
+class RegisterMapCYB06xx5(RegisterMapBaseP64):
 
     #
     #  Entrance exam registers and constants
     #
 
     @property
     def ENTRANCE_EXAM_FW_STATUS_REG(self):
-        return 0x080fe000
+        return 0x0803e000
 
     @property
     def ENTRANCE_EXAM_FW_STATUS_VAL(self):
         return 0xF0000000
 
     @property
     def ENTRANCE_EXAM_FW_STATUS_RE_VAL(self):
@@ -36,27 +36,27 @@
 
     @property
     def ENTRANCE_EXAM_FW_STATUS_MASK(self):
         return 0xF0800000
 
     @property
     def ENTRANCE_EXAM_SRAM_ADDR(self):
-        return 0x080ec000
+        return 0x0802c000
 
     @property
     def ENTRANCE_EXAM_SRAM_SIZE(self):
         return 0x00004000
 
     @property
     def ENTRANCE_EXAM_REGION_HASH_ADDR(self):
         return 0x10000000
 
     @property
     def ENTRANCE_EXAM_REGION_HASH_SIZE(self):
-        return 0x001e0000
+        return 0x00070000
 
     @property
     def ENTRANCE_EXAM_REGION_HASH_MODE(self):
         return 255
 
     @property
     def ENTRANCE_EXAM_REGION_HASH_EXPECTED_VAL(self):
@@ -101,8 +101,7 @@
     @property
     def CYREG_IPC2_STRUCT_LOCK_STATUS(self):
         return 0x4022005C
 
     @property
     def CYREG_EFUSE_SECURE_HASH(self):
         return 0x402c0814
-
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xxa/packets/cy_auth_2m_b0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/packets/entrance_exam.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xxa/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_smif_swap.json` & `cysecuretools-5.0.0/src/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9767278439153438%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'protect_flags': 3}}}",*

 * * "'pre_build'": "{'oem_public_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'oem_private_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'hsm_public_key': '../../common/mxs40v1/prebuilt/hsm_state.json', "*

 * *                "'hsm_private_key': '../../common/mxs40v1/prebuilt/hsm_state.json', 'cy_auth': "*

 * *                "'../packets/cy_auth_2m_s0_sample.jwt'}"}*

```diff
@@ -12,15 +12,15 @@
                         "kid": 3
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
-                "protect_flags": 1,
+                "protect_flags": 3,
                 "reset_after_failure": 0,
                 "resources": [
                     {
                         "address": 270336000,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
@@ -174,21 +174,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_2m_b0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_2m_s0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json` & `cysecuretools-5.0.0/src/targets/cyb06xxa/policy/policy_multi_CM0_CM4_swap.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9814814814814815%*

 * *Differences: {"'pre_build'": "{'oem_public_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'oem_private_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'hsm_public_key': '../../common/mxs40v1/prebuilt/hsm_state.json', "*

 * *                "'hsm_private_key': '../../common/mxs40v1/prebuilt/hsm_state.json'}"}*

```diff
@@ -175,18 +175,18 @@
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
         "cy_auth": "../packets/cy_auth_2m_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_smif_swap.json` & `cysecuretools-5.0.0/src/targets/cys06xxa/policy/policy_single_CM0_CM4_swap.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9763737323633158%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'protect_flags': 3, 'resources': {3: {'address': 270319616, "*

 * *                   "'size': 16384}, 4: {'address': 270270464, 'size': 49152}}}, 1: {'smif_id': 0, "*

 * *                   "'resources': {0: {'size': 917504}, 1: {'address': 269352960, 'size': 917504}}, "*

 * *                   "delete: ['smif_sector_size']}, 2: {'resources': {0: {'size': 851968}}}}}",*

 * * "'pre_build'": "{'oem_public_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'oem_private_ […]*

```diff
@@ -12,15 +12,15 @@
                         "kid": 3
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
-                "protect_flags": 1,
+                "protect_flags": 3,
                 "reset_after_failure": 0,
                 "resources": [
                     {
                         "address": 270336000,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
@@ -31,21 +31,21 @@
                     },
                     {
                         "address": 135184384,
                         "size": 16384,
                         "type": "SRAM_DAP"
                     },
                     {
-                        "address": 270303232,
-                        "size": 32768,
+                        "address": 270319616,
+                        "size": 16384,
                         "type": "STATUS_PARTITION"
                     },
                     {
-                        "address": 405012480,
-                        "size": 786432,
+                        "address": 270270464,
+                        "size": 49152,
                         "type": "SCRATCH"
                     }
                 ],
                 "upgrade": false,
                 "upgrade_mode": "swap",
                 "wdt_enable": true,
                 "wdt_timeout": 4000
@@ -66,27 +66,26 @@
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
                 "launch": 16,
                 "monotonic": 0,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 1867776,
+                        "size": 917504,
                         "type": "BOOT"
                     },
                     {
-                        "address": 402883584,
-                        "size": 1867776,
+                        "address": 269352960,
+                        "size": 917504,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "set_img_ok": true,
-                "smif_id": 1,
-                "smif_sector_size": 262144,
+                "smif_id": 0,
                 "upgrade": true,
                 "version": "0.1",
                 "wdt_enable": false,
                 "wdt_timeout": 4000
             },
             {
                 "boot_auth": [
@@ -102,15 +101,15 @@
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
                 "resources": [
                     {
                         "address": 268500992,
-                        "size": 1802240,
+                        "size": 851968,
                         "type": "BOOT"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 0,
                 "upgrade": false,
                 "version": "0.1"
@@ -167,21 +166,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_2m_b0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_2m_s0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/policy/policy_single_CM0_CM4_swap.json` & `cysecuretools-5.0.0/src/targets/cyb06xxa/policy/policy_single_CM0_CM4_swap.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9814814814814815%*

 * *Differences: {"'pre_build'": "{'oem_public_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'oem_private_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'hsm_public_key': '../../common/mxs40v1/prebuilt/hsm_state.json', "*

 * *                "'hsm_private_key': '../../common/mxs40v1/prebuilt/hsm_state.json'}"}*

```diff
@@ -169,18 +169,18 @@
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
         "cy_auth": "../packets/cy_auth_2m_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex` & `cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex` & `cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-5.0.0/src/targets/cyb06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyb06xxa/target_builder.py` & `cysecuretools-5.0.0/src/targets/cyw20829/target_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,132 +1,132 @@
 """
-Copyright (c) 2019-2021 Cypress Semiconductor Corporation
+Copyright 2020-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-import os
-from cysecuretools.core import TargetBuilder
-from cysecuretools.core.enums import KeyAlgorithm
-from cysecuretools.targets.cyb06xxa.maps.memory_map import MemoryMap_cyb06xxa
-from cysecuretools.targets.cyb06xxa.maps.register_map import \
-    RegisterMap_cyb06xxa
-from cysecuretools.targets.common.p64.policy_filter import PolicyFilter
-from cysecuretools.targets.common.p64.policy_parser import PolicyParser
-from cysecuretools.targets.common.p64.policy_validator import PolicyValidator
-from cysecuretools.execute.provisioning import ProvisioningMXS40v1
-from cysecuretools.execute.provisioning_packet import ProvisioningPacketMXS40v1
-from cysecuretools.execute.entrance_exam.exam_mxs40v1 import \
-    EntranceExamMXS40v1
-from cysecuretools.execute.project_init.project_init_mxs40v1 import \
-    ProjectInitializerMXS40V1
-from cysecuretools.execute.voltage_tool.voltage_tool_mxs40v1 import VoltageToolMXS40v1
-from cysecuretools.execute.key_reader_mxs40v1 import KeyReaderMXS40V1
-from cysecuretools.execute.silicon_data_reader import SiliconDataReaderMXS40v1
-from cysecuretools.execute.image_signing.signtool_mxs40v1 import \
-    SignToolMXS40v1
-from cysecuretools.execute.key_source.key_source_mxs40v1 import (
-    KeySourceMXS40v1)
+from .policy_generator import PolicyGenerator
+from .maps.asset_map import AssetMapCYW20829
+from .maps.memory_map import MemoryMapCYW20829
+from .maps.register_map import RegisterMap_cyw20829
+from ..common.mxs40sv2 import (
+    DependencyValidatorMXS40v2, PolicyValidatorMXS40v2, PolicyParser,
+    DebugCertificateMXS40Sv2, ProvisioningPacketMXS40Sv2, SignToolMXS40Sv2,
+    KeySourceMXS40Sv2, ProjectInitializerMXS40Sv2, ProvisioningMXS40Sv2,
+    RamAppLoaderMXS40Sv2, VersionProviderMXS40Sv2, SiliconDataReaderMXS40Sv2
+)
+from ...core import TargetBuilder
+from ...core.enums import KeyAlgorithm
 
 
-class CYB06xxA_Builder(TargetBuilder):
-    """ CYB06xxA target builder """
+class CYW20829Builder(TargetBuilder):
+    """ CYW20829 target builder """
 
     def get_default_policy(self):
-        return os.path.join(
-            self.target_dir, 'policy', 'policy_single_CM0_CM4_swap.json')
+        return None
 
     def get_ocds(self):
-        return ['pyocd', 'openocd']
+        return ['openocd']
 
     def get_ocd_config(self):
         return {
             'openocd': {
-                'before_init': '',
-                'after_init': 'targets'
+                'before_init': 'cyw20829.cm33 configure -defer-examine',
+                'after_init': 'targets cyw20829.sysap'
             }
         }
 
     def get_memory_map(self):
-        memory_map = MemoryMap_cyb06xxa()
+        memory_map = MemoryMapCYW20829()
         return memory_map
 
     def get_register_map(self):
-        register_map = RegisterMap_cyb06xxa()
+        register_map = RegisterMap_cyw20829()
         return register_map
 
     def get_policy_parser(self, policy):
         policy_parser = PolicyParser(policy)
         return policy_parser
 
     def get_policy_validator(self, policy_parser, memory_map):
-        policy_validator = PolicyValidator(policy_parser, memory_map)
+        dependency_validator = DependencyValidatorMXS40v2(policy_parser)
+        policy_validator = PolicyValidatorMXS40v2(policy_parser, dependency_validator)
         return policy_validator
 
     def get_policy_filter(self, policy_parser):
-        policy_filter = PolicyFilter(policy_parser)
-        return policy_filter
+        pass
 
     def get_provisioning_strategy(self):
-        return ProvisioningMXS40v1()
+        return ProvisioningMXS40Sv2()
 
     def get_provisioning_packet_strategy(self, policy_parser):
-        return ProvisioningPacketMXS40v1(policy_parser)
+        return ProvisioningPacketMXS40Sv2(policy_parser, AssetMapCYW20829())
 
     def get_entrance_exam(self):
-        return EntranceExamMXS40v1
+        return None
 
     def get_voltage_tool(self):
-        return VoltageToolMXS40v1
+        return None
 
     def get_key_reader(self):
-        return KeyReaderMXS40V1
+        return None
 
     def get_project_initializer(self):
-        return ProjectInitializerMXS40V1
+        return ProjectInitializerMXS40Sv2
 
     def get_silicon_data_reader(self):
-        return SiliconDataReaderMXS40v1
+        return SiliconDataReaderMXS40Sv2
 
     def get_key_algorithms(self):
-        return [KeyAlgorithm.EC]
+        return [KeyAlgorithm.RSA, KeyAlgorithm.AES]
 
     def get_sign_tool(self):
-        return SignToolMXS40v1
+        return SignToolMXS40Sv2
 
     def get_key_source(self, **kwargs):
-        return KeySourceMXS40v1(kwargs['policy_parser'])
+        return KeySourceMXS40Sv2(kwargs['policy_parser'])
 
     def get_bootloader_provider(self):
-        from cysecuretools.execute.bootloader_provider_mxs40v1 import (
-            BootloaderProviderMXS40v1)
-        return BootloaderProviderMXS40v1
+        return None
 
     def get_version_provider(self):
-        from cysecuretools.execute.version_provider.version_provider_mxs40v1 \
-            import VersionProviderMXS40v1
-        return VersionProviderMXS40v1
+        return VersionProviderMXS40Sv2
 
     def get_debug_certificate(self):
-        """ N/A for MXS40v1 platform """
-        return None
+        return DebugCertificateMXS40Sv2()
 
     def get_policy_generator(self, policy_parser):
-        """ N/A for MXS40v1 platform """
-        return None
+        return PolicyGenerator(policy_parser)
 
     def get_test_packages(self):
-        """ N/A for MXS40v1 platform """
+        return {
+            'testapps': {
+                'package': 'testapps_cyw20829_b0', 'flow_name': 'testapps'
+            },
+            'testapps_si': {
+                'package': 'testapps_cyw20829_b0', 'flow_name': 'testapps_si'
+            }
+        }
+
+    def get_certificate_strategy(self):
         return None
 
+    def get_app_loader(self):
+        return RamAppLoaderMXS40Sv2()
+
     def get_silicon_id(self):
         """Gets the target silicon ID"""
-        return None
+        return {
+            'id': [0xEB43],
+            'rev': [0x21],
+            'family': 0x110
+        }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt` & `cysecuretools-5.0.0/src/targets/cys06xxa/packets/cy_auth_2m_s0_sample.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/packets/entrance_exam.jwt` & `cysecuretools-5.0.0/src/targets/cys06xxa/packets/entrance_exam.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_smif_swap.json` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/policy/policy_multi_CM0_CM4_smif.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9723634534832453%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'boot_auth': [5], 'bootloader_keys': {0: {'kid': 5, 'key': "*

 * *                   "'../../common/mxs40v1/prebuilt/oem_state.json'}}, 'wdt_enable': False, "*

 * *                   "'protect_flags': 1, 'resources': {0: {'address': 268828672}, 1: {'address': "*

 * *                   "134348800}, 2: {'address': 134397952}, delete: [4, 3]}, delete: "*

 * *                   "['wdt_timeout', 'upgrade_mode']}, 1: {'resources': {0: {'size': 131072}, 1: "*

 * *                   "{'address': 402653 […]*

```diff
@@ -1,58 +1,46 @@
 {
     "boot_upgrade": {
         "firmware": [
             {
                 "acq_win": 100,
                 "boot_auth": [
-                    3
+                    5
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../keys/cy_pub_key.json",
-                        "kid": 3
+                        "key": "../../common/mxs40v1/prebuilt/oem_state.json",
+                        "kid": 5
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
-                "protect_flags": 3,
+                "protect_flags": 1,
                 "reset_after_failure": 0,
                 "resources": [
                     {
-                        "address": 270336000,
+                        "address": 268828672,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
                     {
-                        "address": 135135232,
+                        "address": 134348800,
                         "size": 65536,
                         "type": "SRAM_SPM_PRIV"
                     },
                     {
-                        "address": 135184384,
+                        "address": 134397952,
                         "size": 16384,
                         "type": "SRAM_DAP"
-                    },
-                    {
-                        "address": 270303232,
-                        "size": 32768,
-                        "type": "STATUS_PARTITION"
-                    },
-                    {
-                        "address": 405274624,
-                        "size": 524288,
-                        "type": "SCRATCH"
                     }
                 ],
                 "upgrade": false,
-                "upgrade_mode": "swap",
-                "wdt_enable": true,
-                "wdt_timeout": 4000
+                "wdt_enable": false
             },
             {
                 "acq_win": 100,
                 "boot_auth": [
                     8
                 ],
                 "boot_keys": [
@@ -66,31 +54,28 @@
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
                 "monotonic": 0,
                 "multi_image": 1,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 933888,
+                        "size": 131072,
                         "type": "BOOT"
                     },
                     {
-                        "address": 402768384,
-                        "size": 933888,
+                        "address": 402653184,
+                        "size": 131072,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
-                "set_img_ok": true,
                 "smif_id": 1,
-                "smif_sector_size": 262144,
                 "upgrade": true,
                 "version": "0.1",
-                "wdt_enable": false,
-                "wdt_timeout": 4000
+                "wdt_enable": false
             },
             {
                 "boot_auth": [
                     8
                 ],
                 "boot_keys": [
                     {
@@ -102,35 +87,34 @@
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
                 "multi_image": 2,
                 "resources": [
                     {
-                        "address": 269369344,
-                        "size": 933888,
+                        "address": 268566528,
+                        "size": 262144,
                         "type": "BOOT"
                     },
                     {
-                        "address": 404079104,
-                        "size": 933888,
+                        "address": 402915328,
+                        "size": 262144,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 1,
-                "smif_sector_size": 262144,
                 "upgrade": true,
                 "version": "0.1"
             }
         ],
         "reprogram": [
             {
                 "size": 65536,
-                "start": 270336000
+                "start": 268828672
             }
         ],
         "reprovision": {
             "boot_loader": true,
             "keys_and_policies": true
         },
         "title": "upgrade_policy"
@@ -174,21 +158,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_2m_s0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_512k_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_multi_CM0_CM4_swap.json` & `cysecuretools-5.0.0/src/targets/cys06xxa/policy/policy_multi_CM0_CM4_swap.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9814814814814815%*

 * *Differences: {"'pre_build'": "{'oem_public_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'oem_private_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'hsm_public_key': '../../common/mxs40v1/prebuilt/hsm_state.json', "*

 * *                "'hsm_private_key': '../../common/mxs40v1/prebuilt/hsm_state.json'}"}*

```diff
@@ -175,18 +175,18 @@
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
         "cy_auth": "../packets/cy_auth_2m_s0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_smif_swap.json` & `cysecuretools-5.0.0/src/targets/cys06xxa/policy/policy_single_CM0_CM4_smif_swap.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9814814814814815%*

 * *Differences: {"'pre_build'": "{'oem_public_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'oem_private_key': '../../common/mxs40v1/prebuilt/oem_state.json', "*

 * *                "'hsm_public_key': '../../common/mxs40v1/prebuilt/hsm_state.json', "*

 * *                "'hsm_private_key': '../../common/mxs40v1/prebuilt/hsm_state.json'}"}*

```diff
@@ -170,18 +170,18 @@
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
         "cy_auth": "../packets/cy_auth_2m_s0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/policy/policy_single_CM0_CM4_swap.json` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/policy/policy_single_CM0_CM4_smif.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9726953570780165%*

 * *Differences: {"'boot_upgrade'": "{'firmware': {0: {'boot_auth': [5], 'bootloader_keys': {0: {'kid': 5, 'key': "*

 * *                   "'../../common/mxs40v1/prebuilt/oem_state.json'}}, 'wdt_enable': False, "*

 * *                   "'protect_flags': 1, 'resources': {0: {'address': 268828672}, 1: {'address': "*

 * *                   "134348800}, 2: {'address': 134397952}, delete: [4, 3]}, delete: "*

 * *                   "['upgrade_mode', 'wdt_timeout']}, 1: {'smif_id': 1, 'resources': {0: {'size': "*

 * *                   "393216}, 1: {'ad […]*

```diff
@@ -1,58 +1,46 @@
 {
     "boot_upgrade": {
         "firmware": [
             {
                 "acq_win": 100,
                 "boot_auth": [
-                    3
+                    5
                 ],
                 "bootloader_keys": [
                     {
-                        "key": "../keys/cy_pub_key.json",
-                        "kid": 3
+                        "key": "../../common/mxs40v1/prebuilt/oem_state.json",
+                        "kid": 5
                     }
                 ],
                 "clock_flags": 578,
                 "id": 0,
                 "launch": 1,
                 "monotonic": 0,
-                "protect_flags": 3,
+                "protect_flags": 1,
                 "reset_after_failure": 0,
                 "resources": [
                     {
-                        "address": 270336000,
+                        "address": 268828672,
                         "size": 65536,
                         "type": "FLASH_PC1_SPM"
                     },
                     {
-                        "address": 135135232,
+                        "address": 134348800,
                         "size": 65536,
                         "type": "SRAM_SPM_PRIV"
                     },
                     {
-                        "address": 135184384,
+                        "address": 134397952,
                         "size": 16384,
                         "type": "SRAM_DAP"
-                    },
-                    {
-                        "address": 270319616,
-                        "size": 16384,
-                        "type": "STATUS_PARTITION"
-                    },
-                    {
-                        "address": 270270464,
-                        "size": 49152,
-                        "type": "SCRATCH"
                     }
                 ],
                 "upgrade": false,
-                "upgrade_mode": "swap",
-                "wdt_enable": true,
-                "wdt_timeout": 4000
+                "wdt_enable": false
             },
             {
                 "acq_win": 100,
                 "boot_auth": [
                     8
                 ],
                 "boot_keys": [
@@ -66,30 +54,28 @@
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 1,
                 "launch": 16,
                 "monotonic": 0,
                 "resources": [
                     {
                         "address": 268435456,
-                        "size": 917504,
+                        "size": 393216,
                         "type": "BOOT"
                     },
                     {
-                        "address": 269352960,
-                        "size": 917504,
+                        "address": 402653184,
+                        "size": 393216,
                         "type": "UPGRADE"
                     }
                 ],
                 "rollback_counter": 0,
-                "set_img_ok": true,
-                "smif_id": 0,
+                "smif_id": 1,
                 "upgrade": true,
                 "version": "0.1",
-                "wdt_enable": false,
-                "wdt_timeout": 4000
+                "wdt_enable": false
             },
             {
                 "boot_auth": [
                     8
                 ],
                 "boot_keys": [
                     {
@@ -101,28 +87,28 @@
                 "encrypt_key_id": 1,
                 "encrypt_peer": "../keys/dev_pub_key.pem",
                 "id": 16,
                 "monotonic": 8,
                 "resources": [
                     {
                         "address": 268500992,
-                        "size": 851968,
+                        "size": 327680,
                         "type": "BOOT"
                     }
                 ],
                 "rollback_counter": 0,
                 "smif_id": 0,
                 "upgrade": false,
                 "version": "0.1"
             }
         ],
         "reprogram": [
             {
                 "size": 65536,
-                "start": 270336000
+                "start": 268828672
             }
         ],
         "reprovision": {
             "boot_loader": true,
             "keys_and_policies": true
         },
         "title": "upgrade_policy"
@@ -166,21 +152,21 @@
         }
     },
     "policy": {
         "platform": "psoc64",
         "version": 1.0
     },
     "pre_build": {
-        "cy_auth": "../packets/cy_auth_2m_s0_sample.jwt",
+        "cy_auth": "../packets/cy_auth_512k_b0_sample.jwt",
         "device_private_key": "../keys/dev_priv_key.json",
         "group_private_key": "../keys/grp_priv_key.json",
-        "hsm_private_key": "../../common/p64/prebuilt/hsm_state.json",
-        "hsm_public_key": "../../common/p64/prebuilt/hsm_state.json",
-        "oem_private_key": "../../common/p64/prebuilt/oem_state.json",
-        "oem_public_key": "../../common/p64/prebuilt/oem_state.json",
+        "hsm_private_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "hsm_public_key": "../../common/mxs40v1/prebuilt/hsm_state.json",
+        "oem_private_key": "../../common/mxs40v1/prebuilt/oem_state.json",
+        "oem_public_key": "../../common/mxs40v1/prebuilt/oem_state.json",
         "provision_device_private_key": false,
         "provision_group_private_key": false
     },
     "provisioning": {
         "chain_of_trust": [],
         "packet_dir": "../packets"
     }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex` & `cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_Release_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex` & `cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.hex`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt` & `cysecuretools-5.0.0/src/targets/cys06xxa/prebuilt/CyBootloader_WithLogs_swap/CypressBootloader_CM0p.jwt`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cys06xxa/target_builder.py` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/target_builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,62 @@
 """
-Copyright (c) 2020-2021 Cypress Semiconductor Corporation
+Copyright 2019-2022 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
-from cysecuretools.core import TargetBuilder
-from cysecuretools.core.enums import KeyAlgorithm
-from cysecuretools.targets.cyb06xxa.maps.memory_map import MemoryMap_cyb06xxa
-from cysecuretools.targets.cyb06xxa.maps.register_map import \
-    RegisterMap_cyb06xxa
-from cysecuretools.targets.common.p64.policy_filter import PolicyFilter
-from cysecuretools.targets.common.p64.policy_parser import PolicyParser
-from cysecuretools.targets.common.p64.policy_validator import PolicyValidator
-from cysecuretools.execute.provisioning import ProvisioningMXS40v1
-from cysecuretools.execute.provisioning_packet import ProvisioningPacketMXS40v1
-from cysecuretools.execute.entrance_exam.exam_mxs40v1 import \
-    EntranceExamMXS40v1
-from cysecuretools.execute.project_init.project_init_mxs40v1 import \
-    ProjectInitializerMXS40V1
-from cysecuretools.execute.voltage_tool.voltage_tool_mxs40v1 import VoltageToolMXS40v1
-from cysecuretools.execute.key_reader_mxs40v1 import KeyReaderMXS40V1
-from cysecuretools.execute.silicon_data_reader import SiliconDataReaderMXS40v1
-from cysecuretools.execute.image_signing.signtool_mxs40v1 import \
-    SignToolMXS40v1
-from cysecuretools.execute.key_source.key_source_mxs40v1 import (
-    KeySourceMXS40v1)
 
+from ..cyb06xx5_a1.maps.memory_map import MemoryMapCYB06xx5
+from ..cyb06xx5_a1.maps.register_map import RegisterMapCYB06xx5
+from ..common.mxs40v1 import (
+    PolicyFilter, PolicyParser, PolicyValidator, X509CertificateStrategyMXS40v1,
+    ProvisioningPacketMXS40v1, EntranceExamMXS40v1, SignToolMXS40v1,
+    KeySourceMXS40v1, ProjectInitializerMXS40V1, ProvisioningMXS40v1,
+    SiliconDataReaderMXS40v1, VersionProviderMXS40v1, VoltageToolMXS40v1,
+    BootloaderProviderMXS40v1, KeyReaderMXS40V1
+)
+from ...core import TargetBuilder
+from ...core.enums import KeyAlgorithm
 
-class CYS06xxA_Builder(TargetBuilder):
-    """ CYS06xxA target builder """
+
+class CYB06xx5A1Builder(TargetBuilder):
+    """ CYB06xx5 A1 target builder """
 
     def get_default_policy(self):
-        return os.path.join(
-            self.target_dir, 'policy', 'policy_single_CM0_CM4_swap.json')
+        return os.path.join(self.target_dir, 'policy',
+                            'policy_single_CM0_CM4.json')
 
     def get_ocds(self):
-        return ['pyocd', 'openocd']
+        return ['openocd']
 
     def get_ocd_config(self):
         return {
             'openocd': {
                 'before_init': '',
                 'after_init': 'targets'
             }
         }
 
     def get_memory_map(self):
-        memory_map = MemoryMap_cyb06xxa()
+        memory_map = MemoryMapCYB06xx5()
         return memory_map
 
     def get_register_map(self):
-        register_map = RegisterMap_cyb06xxa()
+        register_map = RegisterMapCYB06xx5()
         return register_map
 
     def get_policy_parser(self, policy):
         policy_parser = PolicyParser(policy)
         return policy_parser
 
     def get_policy_validator(self, policy_parser, memory_map):
@@ -102,31 +94,37 @@
     def get_sign_tool(self):
         return SignToolMXS40v1
 
     def get_key_source(self, **kwargs):
         return KeySourceMXS40v1(kwargs['policy_parser'])
 
     def get_bootloader_provider(self):
-        from cysecuretools.execute.bootloader_provider_mxs40v1 import (
-            BootloaderProviderMXS40v1)
         return BootloaderProviderMXS40v1
 
     def get_version_provider(self):
-        from cysecuretools.execute.version_provider.version_provider_mxs40v1 \
-            import VersionProviderMXS40v1
         return VersionProviderMXS40v1
 
     def get_debug_certificate(self):
         """ N/A for MXS40v1 platform """
         return None
 
     def get_policy_generator(self, policy_parser):
         """ N/A for MXS40v1 platform """
         return None
 
     def get_test_packages(self):
         """ N/A for MXS40v1 platform """
         return None
 
+    def get_certificate_strategy(self):
+        return X509CertificateStrategyMXS40v1()
+
+    def get_app_loader(self):
+        """ N/A for MXS40v1 platform """
+
     def get_silicon_id(self):
         """Gets the target silicon ID"""
-        return None
+        return {
+            'id': [0xE701, 0xE70D],
+            'rev': [0x12],
+            'family': 0x105
+        }
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/asset_map.py` & `cysecuretools-5.0.0/src/targets/cyw20829/maps/asset_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,259 +1,263 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core.key_helper import get_key_bytearray
-from cysecuretools.core.key_helper import calc_key_hash
 from ...common.mxs40sv2.nv_counter_calc import NvCounterCalculator
+from ....core.key_helper import get_key_bytearray, calc_key_hash
 
 
-def asset_map(p, **kwargs):
-    """
-    RAM applications asset map
-    @params p: Policy parser
-    @return: Initialized asset map
+class AssetMapCYW20829:
+    """Asset map for CYW20829"""
 
-    Map fields description:
-    size  - asset size in bytes
-    shift - represents asset bits number that store a parameter. It says about
-            the number of bits the value should be shifted to the left
-    mask  - the number of bits used to store the asset item
-    value - integer value of the bits.
-    """
-    assets = {
-        "target_lcs": {
-            "size": 4,
-            "data": [
-                {
-                    "name": "TARGET_LCS",
-                    "shift": 0,
-                    "value": p.get_target_lcs().value
-                },
-            ],
-        },
-        "control_word": {
-            "size": 4,
-            "data": [
-                {
-                    "name": "CONTROL_WORD",
-                    "shift": 0,
-                    "value": p.get_control_word()
-                },
-            ],
-        },
-        "access_restrict": {
-            "size": 4,
-            "data": [
-                {
-                    "name": "S_NS_AP_CTL_CM33",
-                    "shift": 0,
-                    "mask": 0x03,
-                    "value": p.get_cm33_permission().value
-                },
-                {
-                    "name": "S_NS_AP_CTL_SYS",
-                    "shift": 2,
-                    "mask": 0x03,
-                    "value": p.get_sys_permission().value
-                },
-                {
-                    "name": "S_NS_AP_CTL_DBG",
-                    "shift": 4,
-                    "mask": 0x03,
-                    "value": p.get_cm33_dbg().value
-                },
-                {
-                    "name": "S_NS_AP_CTL_NID",
-                    "shift": 6,
-                    "mask": 0x03,
-                    "value": p.get_cm33_nid().value
-                },
-                {
-                    "name": "S_NS_SYS_AP_MPC_PPC_ENABLE",
-                    "shift": 8,
-                    "mask": 0x01,
-                    "value": p.get_mpc_ppc_permission().value
-                },
-                {
-                    "name": "S_NS_SRAM",
-                    "shift": 9,
-                    "mask": 0x07,
-                    "value": p.get_sram_region().value
-                },
-                {
-                    "name": "S_NS_MMIO",
-                    "shift": 12,
-                    "mask": 0x03,
-                    "value": p.get_mmio_region().value
-                },
-                {
-                    "name": "DEAD_AP_CTL_CM33",
-                    "shift": 14,
-                    "mask": 0x03,
-                    "value": p.get_dead_cm33_permission().value
-                },
-                {
-                    "name": "DEAD_AP_CTL_SYS",
-                    "shift": 16,
-                    "mask": 0x03,
-                    "value": p.get_dead_sys_permission().value
-                },
-                {
-                    "name": "DEAD_AP_CTL_DBG",
-                    "shift": 18,
-                    "mask": 0x03,
-                    "value": p.get_dead_cm33_dbg().value
-                },
-                {
-                    "name": "DEAD_AP_CTL_NID",
-                    "shift": 20,
-                    "mask": 0x03,
-                    "value": p.get_dead_cm33_nid().value
-                },
-                {
-                    "name": "DEAD_SYS_AP_MPC_PPC_ENABLE",
-                    "shift": 22,
-                    "mask": 0x01,
-                    "value": p.get_dead_mpc_ppc_permission().value
-                },
-                {
-                    "name": "DEAD_SRAM",
-                    "shift": 23,
-                    "mask": 0x07,
-                    "value": p.get_dead_sram_region().value
-                },
-                {
-                    "name": "DEAD_MMIO",
-                    "shift": 26,
-                    "mask": 0x03,
-                    "value": p.get_dead_mmio_region().value
-                },
-            ],
-        },
-        "wounding": {
-            "size": 4,
-            "data": [
-                {
-                    "name": "LISTEN_WINDOW",
-                    "shift": 4,
-                    "mask": 0x03,
-                    "value": p.get_listen_window().value
-                },
-            ]
-        },
-        "oem_config": {
-            "size": 4,
-            "data": [
-                {
-                    "name": "CHIP_SELECT",
-                    "shift": 0,
-                    "mask": 0x01,
-                    "value": p.get_chip_select().value
-                },
-                {
-                    "name": "DATA_WIDTH",
-                    "shift": 1,
-                    "mask": 0x03,
-                    "value": p.get_data_width().value
-                },
-                {
-                    "name": "DATA_SELECT",
-                    "shift": 3,
-                    "mask": 0x03,
-                    "value": p.get_data_select().value
-                },
-                {
-                    "name": "ADDRESSING_MODE",
-                    "shift": 5,
-                    "mask": 0x01,
-                    "value": p.get_addressing_mode().value
-                },
-                {
-                    "name": "SMIF_CRYPTO_ENABLED",
-                    "shift": 6,
-                    "mask": 0x01,
-                    "value": int(p.get_encryption())
-                },
-                {
-                    "name": "SMIF_CONFIGURATION",
-                    "shift": 8,
-                    "mask": 0x0F,
-                    "value": p.get_smif_configuration().value
-                },
-            ],
-        },
-        "nv_counter": {
-            "size": 4,
-            "data": [
-                {
-                    "name": "ANTI_ROLLBACK",
-                    "shift": 0,
-                    "value": NvCounterCalculator.calculate(
-                        p.get_nv_counter(), p.get_bits_per_cnt(),
-                        kwargs.get('image_id'))
-                },
-            ],
-        },
-        "oem_key_0_hash": {
-            "size": 16,
-            "data": [
-                {
-                    "name": "KEY_MANAGEMENT_0",
-                    "shift": 0,
-                    "value": calc_key_hash(p.get_pub_key_0_path()
-                                           if p.get_program_oem_key_0_hash()
-                                           else None)
-                },
-            ],
-        },
-        "oem_key_1_hash": {
-            "size": 16,
-            "data": [
-                {
-                    "name": "KEY_MANAGEMENT_1",
-                    "shift": 0,
-                    "value": (calc_key_hash(p.get_pub_key_1_path())
-                              if p.get_program_oem_key_1_hash()
-                              else get_key_bytearray(p.get_encrypt_key_path())
-                              if p.get_encryption()
-                              else calc_key_hash(None))
-                },
-            ],
-        },
-        "pubkey": {
-            "size": 516,
-            "data": [
-                {
-                    "name": "PUBLIC_KEY",
-                    "shift": 0,
-                    "value": get_key_bytearray(kwargs.get('pubkey'))
-                },
-            ],
-        },
-    }
+    @staticmethod
+    def get(p, **kwargs):
+        """
+        RAM applications asset map
+        @params p: Policy parser
+        @return: Initialized asset map
 
-    return assets
+        Map fields description:
+        size  - asset size in bytes
+        shift - represents asset bits number that store a parameter. It says about
+                the number of bits the value should be shifted to the left
+        mask  - the number of bits used to store the asset item
+        value - integer value of the bits.
+        """
+        assets = {
+            "target_lcs": {
+                "size": 4,
+                "data": [
+                    {
+                        "name": "TARGET_LCS",
+                        "shift": 0,
+                        "value": p.get_target_lcs().value
+                    },
+                ],
+            },
+            "control_word": {
+                "size": 4,
+                "data": [
+                    {
+                        "name": "CONTROL_WORD",
+                        "shift": 0,
+                        "value": p.get_control_word()
+                    },
+                ],
+            },
+            "access_restrict": {
+                "size": 4,
+                "data": [
+                    {
+                        "name": "S_NS_AP_CTL_CM33",
+                        "shift": 0,
+                        "mask": 0x03,
+                        "value": p.get_cm33_permission().value
+                    },
+                    {
+                        "name": "S_NS_AP_CTL_SYS",
+                        "shift": 2,
+                        "mask": 0x03,
+                        "value": p.get_sys_permission().value
+                    },
+                    {
+                        "name": "S_NS_AP_CTL_DBG",
+                        "shift": 4,
+                        "mask": 0x03,
+                        "value": p.get_cm33_dbg().value
+                    },
+                    {
+                        "name": "S_NS_AP_CTL_NID",
+                        "shift": 6,
+                        "mask": 0x03,
+                        "value": p.get_cm33_nid().value
+                    },
+                    {
+                        "name": "S_NS_SYS_AP_MPC_PPC_ENABLE",
+                        "shift": 8,
+                        "mask": 0x01,
+                        "value": p.get_mpc_ppc_permission().value
+                    },
+                    {
+                        "name": "S_NS_SRAM",
+                        "shift": 9,
+                        "mask": 0x07,
+                        "value": p.get_sram_region().value
+                    },
+                    {
+                        "name": "S_NS_MMIO",
+                        "shift": 12,
+                        "mask": 0x03,
+                        "value": p.get_mmio_region().value
+                    },
+                    {
+                        "name": "DEAD_AP_CTL_CM33",
+                        "shift": 14,
+                        "mask": 0x03,
+                        "value": p.get_dead_cm33_permission().value
+                    },
+                    {
+                        "name": "DEAD_AP_CTL_SYS",
+                        "shift": 16,
+                        "mask": 0x03,
+                        "value": p.get_dead_sys_permission().value
+                    },
+                    {
+                        "name": "DEAD_AP_CTL_DBG",
+                        "shift": 18,
+                        "mask": 0x03,
+                        "value": p.get_dead_cm33_dbg().value
+                    },
+                    {
+                        "name": "DEAD_AP_CTL_NID",
+                        "shift": 20,
+                        "mask": 0x03,
+                        "value": p.get_dead_cm33_nid().value
+                    },
+                    {
+                        "name": "DEAD_SYS_AP_MPC_PPC_ENABLE",
+                        "shift": 22,
+                        "mask": 0x01,
+                        "value": p.get_dead_mpc_ppc_permission().value
+                    },
+                    {
+                        "name": "DEAD_SRAM",
+                        "shift": 23,
+                        "mask": 0x07,
+                        "value": p.get_dead_sram_region().value
+                    },
+                    {
+                        "name": "DEAD_MMIO",
+                        "shift": 26,
+                        "mask": 0x03,
+                        "value": p.get_dead_mmio_region().value
+                    },
+                ],
+            },
+            "wounding": {
+                "size": 4,
+                "data": [
+                    {
+                        "name": "LISTEN_WINDOW",
+                        "shift": 4,
+                        "mask": 0x03,
+                        "value": p.get_listen_window().value
+                    },
+                ]
+            },
+            "oem_config": {
+                "size": 4,
+                "data": [
+                    {
+                        "name": "CHIP_SELECT",
+                        "shift": 0,
+                        "mask": 0x01,
+                        "value": p.get_chip_select().value
+                    },
+                    {
+                        "name": "DATA_WIDTH",
+                        "shift": 1,
+                        "mask": 0x03,
+                        "value": p.get_data_width().value
+                    },
+                    {
+                        "name": "DATA_SELECT",
+                        "shift": 3,
+                        "mask": 0x03,
+                        "value": p.get_data_select().value
+                    },
+                    {
+                        "name": "ADDRESSING_MODE",
+                        "shift": 5,
+                        "mask": 0x01,
+                        "value": p.get_addressing_mode().value
+                    },
+                    {
+                        "name": "SMIF_CRYPTO_ENABLED",
+                        "shift": 6,
+                        "mask": 0x01,
+                        "value": int(p.get_encryption())
+                    },
+                    {
+                        "name": "SMIF_CONFIGURATION",
+                        "shift": 8,
+                        "mask": 0x0F,
+                        "value": p.get_smif_configuration().value
+                    },
+                ],
+            },
+            "nv_counter": {
+                "size": 4,
+                "data": [
+                    {
+                        "name": "ANTI_ROLLBACK",
+                        "shift": 0,
+                        "value": NvCounterCalculator.calculate(
+                            p.get_nv_counter(), p.get_bits_per_cnt(),
+                            kwargs.get('image_id'))
+                    },
+                ],
+            },
+            "oem_key_0_hash": {
+                "size": 16,
+                "data": [
+                    {
+                        "name": "KEY_MANAGEMENT_0",
+                        "shift": 0,
+                        "value": calc_key_hash(p.get_pub_key_0_path()
+                                               if p.get_program_oem_key_0_hash()
+                                               else None)
+                    },
+                ],
+            },
+            "oem_key_1_hash": {
+                "size": 16,
+                "data": [
+                    {
+                        "name": "KEY_MANAGEMENT_1",
+                        "shift": 0,
+                        "value": (calc_key_hash(p.get_pub_key_1_path())
+                                  if p.get_program_oem_key_1_hash()
+                                  else get_key_bytearray(p.get_encrypt_key_path())
+                                  if p.get_encryption()
+                                  else calc_key_hash(None))
+                    },
+                ],
+            },
+            "pubkey": {
+                "size": 516,
+                "data": [
+                    {
+                        "name": "PUBLIC_KEY",
+                        "shift": 0,
+                        "value": get_key_bytearray(kwargs.get('pubkey'))
+                    },
+                ],
+            },
+        }
+
+        return assets
 
 
 def asset_item_data(p, asset_name, asset_item_name):
     """ Gets a tuple with the asset item size and mask """
     shift = None
     mask = None
-    assets = asset_map(p)
+    assets = AssetMapCYW20829.get(p)
     for item in assets[asset_name]['data']:
         if item['name'] == asset_item_name:
             shift = item['shift']
             mask = item['mask']
             break
     return shift, mask
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/prov_flows.json` & `cysecuretools-5.0.0/src/targets/cyw20829/flows/prov_flows.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/flows/reverse_asset_map.py` & `cysecuretools-5.0.0/src/targets/cyw20829/maps/reverse_asset_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,16 +12,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import binascii
 
-from ...common.mxs40sv2 import asset_enums as enums
 from .asset_map import asset_item_data
+from ...common.mxs40sv2 import asset_enums as enums
 
 
 class ReverseAssetMap:
 
     def __init__(self, policy_parser):
         self.policy_parser = policy_parser
         self.encryption_enabled = None
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/memory_map.py` & `cysecuretools-5.0.0/src/targets/cyw20829/maps/memory_map.py`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/maps/register_map.py` & `cysecuretools-5.0.0/src/targets/cyw20829/maps/register_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from cysecuretools.core import RegisterMapBaseCYW20829
+from ....core import RegisterMapBaseCYW20829
 
 
 class RegisterMap_cyw20829(RegisterMapBaseCYW20829):
 
     @property
     def BOOTROM_VERSION(self):
         return 0x20000004
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin` & `cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin` & `cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin` & `cysecuretools-5.0.0/src/targets/cyw20829/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/packets/debug_cert.json` & `cysecuretools-5.0.0/src/targets/cyw20829/packets/debug_cert.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_hci_secure.json` & `cysecuretools-5.0.0/src/targets/cyw20829/policy/policy_hci_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_no_secure.json` & `cysecuretools-5.0.0/src/targets/cyw20829/policy/policy_no_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_reprovisioning_secure.json` & `cysecuretools-5.0.0/src/targets/cyw20829/policy/policy_reprovisioning_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy/policy_secure.json` & `cysecuretools-5.0.0/src/targets/cyw20829/policy/policy_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829/policy_generator.py` & `cysecuretools-5.0.0/src/targets/cyw20829/policy_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Copyright (c) 2021 Cypress Semiconductor Corporation
+Copyright 2021-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,18 +12,18 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import struct
 
-from ... core.json_helper import replace
-from ... core.jsonpath import set_node_value
-from .flows.asset_map import asset_map
-from .flows.reverse_asset_map import ReverseAssetMap
+from .maps.asset_map import AssetMapCYW20829
+from .maps.reverse_asset_map import ReverseAssetMap
+from ...core.json_helper import replace
+from ...core.jsonpath import set_node_value
 
 
 class PolicyGenerator:
     def __init__(self, policy_parser):
         self.policy_parser = policy_parser
 
     def populate(self, packets, assets):
@@ -59,15 +60,15 @@
             data[asset] = unpacked[i]
         return data
 
     def _struct_format(self, asset_list):
         """ Gets format string based on asset map items size """
         fmt = '<'
         assets_size = 0
-        assets = asset_map(self.policy_parser)
+        assets = AssetMapCYW20829.get(self.policy_parser)
         for asset in asset_list:
             size = assets[asset]['size']
             if size == 4:
                 fmt += 'I'
                 assets_size += size
             elif size > 4:
                 fmt += f'{size}s'
```

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/flows/prov_flows.json` & `cysecuretools-5.0.0/src/targets/cyw20829_a0/flows/prov_flows.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin` & `cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/prov_oem/cyapp_prov_oem_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin` & `cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/reprovisioning/cyapp_reprovisioning_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin` & `cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/apps/to_rma/cyapp_to_rma_signed_icv0.bin`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/packets/debug_cert.json` & `cysecuretools-5.0.0/src/targets/cyw20829_a0/packets/debug_cert.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_hci_secure.json` & `cysecuretools-5.0.0/src/targets/cyw20829_a0/policy/policy_hci_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_no_secure.json` & `cysecuretools-5.0.0/src/targets/cyw20829_a0/policy/policy_no_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_reprovisioning_secure.json` & `cysecuretools-5.0.0/src/targets/cyw20829_a0/policy/policy_reprovisioning_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/policy/policy_secure.json` & `cysecuretools-5.0.0/src/targets/cyw20829_a0/policy/policy_secure.json`

 * *Files identical despite different names*

### Comparing `cysecuretools-4.2.0/cysecuretools/targets/cyw20829_a0/target_builder.py` & `cysecuretools-5.0.0/src/targets/cyb06xx5_a1/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
-Copyright (c) 2020-2023 Cypress Semiconductor Corporation
+Copyright 2019-2023 Cypress Semiconductor Corporation (an Infineon company)
+or an affiliate of Cypress Semiconductor Corporation. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .. import CYW20829Builder
+from .target_builder import CYB06xx5A1Builder
 
-
-class CYW20829A0Builder(CYW20829Builder):
-    """ CYW20829 A0 target builder """
-
-    def get_test_packages(self):
-        return {
-            'testapps': {
-                'package': 'testapps_cyw20829_a0', 'flow_name': 'testapps'
-            },
-            'testapps_si': {
-                'package': 'testapps_cyw20829_a0', 'flow_name': 'testapps_si'
-            }
+target_map = {
+    'cy8cproto-064b0s3': {
+        'a1': {
+            'class': CYB06xx5A1Builder,
+            'family': 'PSoC64 Kit targets',
+            'display_name': 'PSoC64 512K',
+            'type': 'kit',
+            'platform': 'psoc64'
         }
-
-    def get_silicon_id(self):
-        """Gets the target silicon ID"""
-        return {
-            'id': [0xEB40],
-            'rev': [0x11],
-            'family': 0x110
+    },
+    'cyb06xx5': {
+        'a1': {
+            'class': CYB06xx5A1Builder,
+            'family': 'PSoC64 Secure Boot Family',
+            'display_name': 'PSoC64 512K',
+            'type': 'family',
+            'platform': 'psoc64'
         }
+    }
+}
```

### Comparing `cysecuretools-4.2.0/cysecuretools.egg-info/PKG-INFO` & `cysecuretools-5.0.0/cysecuretools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cysecuretools
-Version: 4.2.0
-Summary: Cypress secure tools for Python
-Home-page: https://github.com/cypresssemiconductorco/cysecuretools
-Author: Cypress Semiconductor
+Version: 5.0.0
+Summary: Python tools for provisioning Cypress/Infineon MCUs
+Home-page: https://github.com/Infineon/cysecuretools
+Author: Cypress Semiconductor Corporation (an Infineon company)
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,34 +17,34 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This package contains security tools for creating keys, creating certificates, signing user applications, and provisioning Cypress MCUs.
 
 # Table of Contents
-- [HW/SW compatibility](#hwsw-compatibility)
 - [Prerequisites](#prerequisites)
 - [Documentation](#documentation)
 - [Installing package](#installing-package)
 - [Supported devices](#supported-devices)
 - [Interface and Usage](#interface-and-usage)
     - [PSoC 64](#psoc-64)
     - [CYW20829](#cyw20829)
+    - [XMC7100/7200](#xmc71007200)
 - [Logging](#logging)
 - [Installing libusb driver](#installing-libusb-driver)
 - [Known issues](#known-issues)
 - [License and Contributions](#license-and-contributions)
 
 # HW/SW compatibility
 ## PSoC 64
 <table>
   <thead>
     <tr>
       <td>Target/Kit</td>
-      <td>Silicon Revision</td>
+      <td>Silicon Revision<sup>1</sup></td>
       <td>Silicon ID, Silicon Rev., Family ID</td>
       <td>CySecureTools Version</td>
       <td>Secure FlashBoot Version</td>
       <td>CyBootloader Version</td>
     </tr>
   </thead>
   <tbody>
@@ -69,26 +69,26 @@
       <td>
         cyb06xxa<br>
         cy8ckit&#8209;064b0s2&#8209;4343w
       </td>
       <td>A1</td>
       <td>0xE470, 0x12, 0x102</td>
       <td>4.2.0</td>
-      <td>4.0.2.1842</td>
+      <td>4.0.3.2319</td>
       <td>2.0.2.8102</td>
     </tr>
     <tr>
       <td>
         cys06xxa<br>
         cy8ckit&#8209;064s0s2&#8209;4343w
       </td>
       <td>A1</td>
-      <td>0xE4A0, 0x12, 0x102</td>
+      <td>0xE4A0, 0x12, 0x02</td>
       <td>4.2.0</td>
-      <td>4.0.2.1842</td>
+      <td>4.0.3.2319</td>
       <td>2.0.2.8102</td>
     </tr>
     <tr>
       <td colspan="6" style="text-align: center;">1M</td>
     </tr>
     <tr>
       <td>
@@ -143,71 +143,57 @@
 
 <sup>1</sup> Specify `--rev` option for older revision of the silicon (e.g. `$ cysecuretools -t cyw20829 --rev a0 <COMMAND>`). Using the latest revision does not require specifying the option.
 
 # Prerequisites
 * General
   * Python 3.6 or later
 * For PSoC 64 devices
-  * In case of use PyOCD:
-    * [Installed the libusb driver](#installing-libusb-driver)
-    * Ensure the KitProg3 programming mode is **DAPLink**
-  * In case of use OpenOCD:
-    * [Installed Cypress OpenOCD](https://github.com/cypresssemiconductorco/openocd/releases)
-    * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk**
+  * [Installed Cypress OpenOCD](https://github.com/cypresssemiconductorco/openocd/releases)
+  * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk**
   * Ensure the power selection jumper is set to provide 2.5 V to the power supply pin related to eFuse power. This voltage level is required to blow eFuses
 * For CYW20829 devices
   * [Installed Cypress OpenOCD](https://github.com/cypresssemiconductorco/openocd/releases)
   * Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk**
   * Ensure the power selection jumper is set to provide 2.5 V to the power supply pin related to eFuse power. This voltage level is required to blow eFuses
 
+
 # Documentation
 * [PSoC64 Secure MCU Secure Boot SDK User Guide](https://www.cypress.com/documentation/software-and-drivers/psoc-64-secure-mcu-secure-boot-sdk-user-guide)
-* [Changelog](CHANGELOG.md)
+* [Changelog](https://github.com/Infineon/cysecuretools/blob/master/CHANGELOG.md)
 
 # Installing Package
 Invoke `pip install` from the command line:
 ```bash
 $ pip install cysecuretools
 ```
+To update the already installed package:
+```bash
+$ pip install --upgrade --force-reinstall cysecuretools
+```
 
 
 # Supported devices
 Use `device-list` command for output of the supported devices list.
 ```bash
 $ cysecuretools device-list
 ```
 
 
 # Interface and Usage
 ## PSoC 64
-See [README_PSOC64.md](docs/README_PSOC64.md)
+See [README_PSOC64.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_PSOC64.md)
 ## CYW20829
-See [README_CYW20829.md](docs/README_CYW20829.md)
+See [README_CYW20829.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_CYW20829.md)
+## XMC7100/7200
+See [README_XMC7XXX.md](https://github.com/Infineon/cysecuretools/blob/master/docs/README_XMC7XXX.md)
 
 
 # Logging
 Every time the tool is invoked, a new log file is created in the _logs_ directory of the project. By default, the console output has INFO logging severity. The log file contains the DEBUG logging severity.
 
-When using _pyOCD_ as a debugger, the log files contain messages sent by both tools - _CySecureTools_ and _pyOCD_. When using _OpenOCD_, the log files contain messages from the package only. For the _OpenOCD_ messages, the additional files are created (e.g. _openocd_1.log_).
-
-
-# Installing libusb driver
-
-**Windows**
-  - Download and unzip libusb-1.0.25.7z from https://github.com/libusb/libusb/releases/tag/v1.0.25.
-  - Run the following command to determine if a Python shell is executing in 32-bit or 64-bit mode on the OS: `python -c "import struct; print(struct.calcsize('P') * 8)"`
-  - Copy *libusb-1.0.dll* file into the Python root folder (in same folder with *python.exe*). Use the 64-bit version of DLL for the 64-bit Python (MinGW64 directory) and the 32-bit version of DLL for the 32-bit Python (MinGW32 directory).
-  - Ensure the Python path is located at the beginning of the Path environment variable.
-
-**Mac OS**
-  - Use [homebrew](https://brew.sh/) to install the driver from the terminal: `homebrew install libusb`.
-
-**Linux**
-  - Bundled with the system, no need for additional installation.
-
 
 # Known issues
 - Using the policy from version 4.0.0 in projects created by version 4.1.0 causes the CY_FB_INVALID_IMG_JWT_SIGNATURE error during re-provisioning on PSoC64-2M devices:
 ```
   ...
   ERROR : SFB status: CY_FB_INVALID_IMG_JWT_SIGNATURE: Invalid image certificate signature. Check the log for details
 ```
@@ -246,14 +232,22 @@
 The software is provided under the Apache-2.0 license. Contributions to this project are accepted under the same license.
 This project contains code from other projects. The original license text is included in those source files.
 
 
 # Changelog
 All notable changes to this project will be documented in this file.
 
+## 5.0.0
+### Changed
+- Removed pyOCD support. OpenOCD is used as a default On-Chip debugger for all platforms
+- High-level API module refactoring
+
+### Added
+- Support for XMC7100, XMC7200 devices
+
 ## 4.2.0
 ### Added
 - Support for CYW20829 B0 silicon revision
 - Multi-image NV counter for CYW20829
 - Transition PSoC 64 devices to RMA LCS
 - Open PSoC 64 devices in RMA LCS for debugging
 - OpenOCD autodiscovery in ModusToolbox directory
```

#### html2text {}

```diff
@@ -1,99 +1,88 @@
-Metadata-Version: 2.1 Name: cysecuretools Version: 4.2.0 Summary: Cypress
-secure tools for Python Home-page: https://github.com/cypresssemiconductorco/
-cysecuretools Author: Cypress Semiconductor License: Apache 2.0 Platform:
-UNKNOWN Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Embedded Systems Requires-Python:
->=3.6 Description-Content-Type: text/markdown License-File: LICENSE This
-package contains security tools for creating keys, creating certificates,
-signing user applications, and provisioning Cypress MCUs. # Table of Contents -
-[HW/SW compatibility](#hwsw-compatibility) - [Prerequisites](#prerequisites) -
-[Documentation](#documentation) - [Installing package](#installing-package) -
-[Supported devices](#supported-devices) - [Interface and Usage](#interface-and-
-usage) - [PSoC 64](#psoc-64) - [CYW20829](#cyw20829) - [Logging](#logging) -
+Metadata-Version: 2.1 Name: cysecuretools Version: 5.0.0 Summary: Python tools
+for provisioning Cypress/Infineon MCUs Home-page: https://github.com/Infineon/
+cysecuretools Author: Cypress Semiconductor Corporation (an Infineon company)
+License: Apache 2.0 Platform: UNKNOWN Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Operating System
+:: OS Independent Classifier: Topic :: Software Development :: Embedded Systems
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE This package contains security tools for creating keys, creating
+certificates, signing user applications, and provisioning Cypress MCUs. # Table
+of Contents - [Prerequisites](#prerequisites) - [Documentation](#documentation)
+- [Installing package](#installing-package) - [Supported devices](#supported-
+devices) - [Interface and Usage](#interface-and-usage) - [PSoC 64](#psoc-64) -
+[CYW20829](#cyw20829) - [XMC7100/7200](#xmc71007200) - [Logging](#logging) -
 [Installing libusb driver](#installing-libusb-driver) - [Known issues](#known-
 issues) - [License and Contributions](#license-and-contributions) # HW/SW
 compatibility ## PSoC 64
-                                   Silicon
-                                   ID,                   Secure
-Target/Kit                Silicon  Silicon CySecureTools FlashBoot  CyBootloader
-                          Revision Rev.,   Version       Version    Version
-                                   Family
-                                   ID
+                                    Silicon
+                                    ID,                   Secure
+Target/Kit                Silicon   Silicon CySecureTools FlashBoot  CyBootloader
+                          Revision1 Rev.,   Version       Version    Version
+                                    Family
+                                    ID
 512K
-cyb06xx5                           0xE70D,
-cy8cproto‑064b0s3       A1       0x12,   4.2.0         4.0.2.1842 2.0.1.6441
-                                   0x105
+cyb06xx5                            0xE70D,
+cy8cproto‑064b0s3       A1        0x12,   4.2.0         4.0.2.1842 2.0.1.6441
+                                    0x105
 2M
-cyb06xxa                           0xE470,
-cy8ckit‑064b0s2‑4343w A1       0x12,   4.2.0         4.0.2.1842 2.0.2.8102
-                                   0x102
-cys06xxa                           0xE4A0,
-cy8ckit‑064s0s2‑4343w A1       0x12,   4.2.0         4.0.2.1842 2.0.2.8102
-                                   0x102
+cyb06xxa                            0xE470,
+cy8ckit‑064b0s2‑4343w A1        0x12,   4.2.0         4.0.3.2319 2.0.2.8102
+                                    0x102
+cys06xxa                            0xE4A0,
+cy8ckit‑064s0s2‑4343w A1        0x12,   4.2.0         4.0.3.2319 2.0.2.8102
+                                    0x02
 1M
-                                   0xE262,
-cyb06xx7                           0x24,
-cy8cproto‑064s1‑sb    B3       0x100   4.2.0         4.0.2.1842 2.0.0.4041
-cy8cproto‑064b0s1‑ble          0xE261,
-cy8cproto‑064b0s1‑ssa          0x24,
-                                   0x100
+                                    0xE262,
+cyb06xx7                            0x24,
+cy8cproto‑064s1‑sb    B3        0x100   4.2.0         4.0.2.1842 2.0.0.4041
+cy8cproto‑064b0s1‑ble           0xE261,
+cy8cproto‑064b0s1‑ssa           0x24,
+                                    0x100
 ## CYW20829
            Silicon   Silicon ID,   CySecureTools                 RAM
 Target/Kit Revision1 Silicon Rev., Version       BootROM Version Applications
                      Family ID                                   Version
 cyw20829   A0        0xEB40, 0x11, 4.2.0         1.0.0.7120      1.0.0.2857
                      0x110
 cyw20829   B0        0xEB43, 0x21, 4.2.0         1.2.0.8274      1.2.0.3073
                      0x110
 1 Specify `--rev` option for older revision of the silicon (e.g. `$
 cysecuretools -t cyw20829 --rev a0 `). Using the latest revision does not
 require specifying the option. # Prerequisites * General * Python 3.6 or later
-* For PSoC 64 devices * In case of use PyOCD: * [Installed the libusb driver]
-(#installing-libusb-driver) * Ensure the KitProg3 programming mode is
-**DAPLink** * In case of use OpenOCD: * [Installed Cypress OpenOCD](https://
-github.com/cypresssemiconductorco/openocd/releases) * Ensure the KitProg3
-programming mode is **CMSIS-DAP Bulk** * Ensure the power selection jumper is
-set to provide 2.5 V to the power supply pin related to eFuse power. This
-voltage level is required to blow eFuses * For CYW20829 devices * [Installed
-Cypress OpenOCD](https://github.com/cypresssemiconductorco/openocd/releases) *
-Ensure the KitProg3 programming mode is **CMSIS-DAP Bulk** * Ensure the power
-selection jumper is set to provide 2.5 V to the power supply pin related to
-eFuse power. This voltage level is required to blow eFuses # Documentation *
-[PSoC64 Secure MCU Secure Boot SDK User Guide](https://www.cypress.com/
-documentation/software-and-drivers/psoc-64-secure-mcu-secure-boot-sdk-user-
-guide) * [Changelog](CHANGELOG.md) # Installing Package Invoke `pip install`
-from the command line: ```bash $ pip install cysecuretools ``` # Supported
-devices Use `device-list` command for output of the supported devices list.
-```bash $ cysecuretools device-list ``` # Interface and Usage ## PSoC 64 See
-[README_PSOC64.md](docs/README_PSOC64.md) ## CYW20829 See [README_CYW20829.md]
-(docs/README_CYW20829.md) # Logging Every time the tool is invoked, a new log
-file is created in the _logs_ directory of the project. By default, the console
-output has INFO logging severity. The log file contains the DEBUG logging
-severity. When using _pyOCD_ as a debugger, the log files contain messages sent
-by both tools - _CySecureTools_ and _pyOCD_. When using _OpenOCD_, the log
-files contain messages from the package only. For the _OpenOCD_ messages, the
-additional files are created (e.g. _openocd_1.log_). # Installing libusb driver
-**Windows** - Download and unzip libusb-1.0.25.7z from https://github.com/
-libusb/libusb/releases/tag/v1.0.25. - Run the following command to determine if
-a Python shell is executing in 32-bit or 64-bit mode on the OS: `python -
-c "import struct; print(struct.calcsize('P') * 8)"` - Copy *libusb-1.0.dll*
-file into the Python root folder (in same folder with *python.exe*). Use the
-64-bit version of DLL for the 64-bit Python (MinGW64 directory) and the 32-bit
-version of DLL for the 32-bit Python (MinGW32 directory). - Ensure the Python
-path is located at the beginning of the Path environment variable. **Mac OS** -
-Use [homebrew](https://brew.sh/) to install the driver from the terminal:
-`homebrew install libusb`. **Linux** - Bundled with the system, no need for
-additional installation. # Known issues - Using the policy from version 4.0.0
-in projects created by version 4.1.0 causes the CY_FB_INVALID_IMG_JWT_SIGNATURE
-error during re-provisioning on PSoC64-2M devices: ``` ... ERROR : SFB status:
+* For PSoC 64 devices * [Installed Cypress OpenOCD](https://github.com/
+cypresssemiconductorco/openocd/releases) * Ensure the KitProg3 programming mode
+is **CMSIS-DAP Bulk** * Ensure the power selection jumper is set to provide 2.5
+V to the power supply pin related to eFuse power. This voltage level is
+required to blow eFuses * For CYW20829 devices * [Installed Cypress OpenOCD]
+(https://github.com/cypresssemiconductorco/openocd/releases) * Ensure the
+KitProg3 programming mode is **CMSIS-DAP Bulk** * Ensure the power selection
+jumper is set to provide 2.5 V to the power supply pin related to eFuse power.
+This voltage level is required to blow eFuses # Documentation * [PSoC64 Secure
+MCU Secure Boot SDK User Guide](https://www.cypress.com/documentation/software-
+and-drivers/psoc-64-secure-mcu-secure-boot-sdk-user-guide) * [Changelog](https:
+//github.com/Infineon/cysecuretools/blob/master/CHANGELOG.md) # Installing
+Package Invoke `pip install` from the command line: ```bash $ pip install
+cysecuretools ``` To update the already installed package: ```bash $ pip
+install --upgrade --force-reinstall cysecuretools ``` # Supported devices Use
+`device-list` command for output of the supported devices list. ```bash $
+cysecuretools device-list ``` # Interface and Usage ## PSoC 64 See
+[README_PSOC64.md](https://github.com/Infineon/cysecuretools/blob/master/docs/
+README_PSOC64.md) ## CYW20829 See [README_CYW20829.md](https://github.com/
+Infineon/cysecuretools/blob/master/docs/README_CYW20829.md) ## XMC7100/7200 See
+[README_XMC7XXX.md](https://github.com/Infineon/cysecuretools/blob/master/docs/
+README_XMC7XXX.md) # Logging Every time the tool is invoked, a new log file is
+created in the _logs_ directory of the project. By default, the console output
+has INFO logging severity. The log file contains the DEBUG logging severity. #
+Known issues - Using the policy from version 4.0.0 in projects created by
+version 4.1.0 causes the CY_FB_INVALID_IMG_JWT_SIGNATURE error during re-
+provisioning on PSoC64-2M devices: ``` ... ERROR : SFB status:
 CY_FB_INVALID_IMG_JWT_SIGNATURE: Invalid image certificate signature. Check the
 log for details ``` _Workaround_: 1. Open the policy file. 2. Navigate to
 section 1 of the `boot_upgrade/firmware`. 3. Set `boot_auth` and
 `bootloader_keys` as follows: ``` "boot_auth": [ 3 ], "bootloader_keys": [
 { "kid": 3, "key": "../keys/cy_pub_key.json" } ] ``` - During the installation
 of the package via _pip_ on Mac OS Big Sur, the following exception is raised:
 ``` ... distutils.errors.DistutilsError: Setup script exited with error:
@@ -106,37 +95,39 @@
 EasyInstall maintainers to find out if a fix or workaround is available. ```
 _Solution:_ Upgrade the `pip` package running the following command from the
 terminal: `python3 -m pip install --upgrade pip`. # License and Contributions
 The software is provided under the Apache-2.0 license. Contributions to this
 project are accepted under the same license. This project contains code from
 other projects. The original license text is included in those source files. #
 Changelog All notable changes to this project will be documented in this file.
-## 4.2.0 ### Added - Support for CYW20829 B0 silicon revision - Multi-image NV
-counter for CYW20829 - Transition PSoC 64 devices to RMA LCS - Open PSoC 64
-devices in RMA LCS for debugging - OpenOCD autodiscovery in ModusToolbox
-directory - Add SW/HW compatibility table to the readme ### Changed - Target
-`cyw20829` is used for the latest silicon revision. For the previous silicon
-revision (A0) add _--rev_ option in the command line (`-t cyw20829 --rev a0`)
-## 4.1.0 ### Added - OpenOCD support for PSoC 64 devices - Creating update
-package in the unsigned image (_extend-image_ command) ### Changed - Fixed
-installation failure using pip 22.1 - CyBootloader 2.0.2.8102 for PSoC 64 2M: -
-Improved performance of SWAP algorithm - Image certificate signed with the
-Infineon key (id=3) - Use Infineon key (id=3) for bootloader in the policy
-files ## 4.0.0 ### Added - Support of CYW20829 devices - Support Python 3.10 -
-Signing images with HSM ### Changed - Separated PSoC 64 and CYW20829 devices
-CLI - Updated PSoC 64 CyBootloader for 512k and 2M: - added
-"reset_after_failure" feature - decreased boot time - Protect PSA API from NSPE
-in PSoC 64 2M-S0 policy - Prevent signing of already signed images - Change
-MCUboot image header padding to erase value - Use CyBootloader from the project
-directory if the project exists - Updated dependencies packages to the latest
-versions - Use pyocd 0.32.3 ## 3.1.1 ### Changed - Fixed installation failure
-on macOS Big Sur and Apple M1 chip - Fixed installation failure in Python 3.9
-## 3.1.0 ### Added - SCRATCH with Status Partition swap mode - Small image
-slots support in the external memory ## 3.0.0 ### Added - Image SWAP using
-Status Partition ### Changed - CyBootloader 2.0 - Secure Flash Boot 4.0.2
+## 5.0.0 ### Changed - Removed pyOCD support. OpenOCD is used as a default On-
+Chip debugger for all platforms - High-level API module refactoring ### Added -
+Support for XMC7100, XMC7200 devices ## 4.2.0 ### Added - Support for CYW20829
+B0 silicon revision - Multi-image NV counter for CYW20829 - Transition PSoC 64
+devices to RMA LCS - Open PSoC 64 devices in RMA LCS for debugging - OpenOCD
+autodiscovery in ModusToolbox directory - Add SW/HW compatibility table to the
+readme ### Changed - Target `cyw20829` is used for the latest silicon revision.
+For the previous silicon revision (A0) add _--rev_ option in the command line
+(`-t cyw20829 --rev a0`) ## 4.1.0 ### Added - OpenOCD support for PSoC 64
+devices - Creating update package in the unsigned image (_extend-image_
+command) ### Changed - Fixed installation failure using pip 22.1 - CyBootloader
+2.0.2.8102 for PSoC 64 2M: - Improved performance of SWAP algorithm - Image
+certificate signed with the Infineon key (id=3) - Use Infineon key (id=3) for
+bootloader in the policy files ## 4.0.0 ### Added - Support of CYW20829 devices
+- Support Python 3.10 - Signing images with HSM ### Changed - Separated PSoC 64
+and CYW20829 devices CLI - Updated PSoC 64 CyBootloader for 512k and 2M: -
+added "reset_after_failure" feature - decreased boot time - Protect PSA API
+from NSPE in PSoC 64 2M-S0 policy - Prevent signing of already signed images -
+Change MCUboot image header padding to erase value - Use CyBootloader from the
+project directory if the project exists - Updated dependencies packages to the
+latest versions - Use pyocd 0.32.3 ## 3.1.1 ### Changed - Fixed installation
+failure on macOS Big Sur and Apple M1 chip - Fixed installation failure in
+Python 3.9 ## 3.1.0 ### Added - SCRATCH with Status Partition swap mode - Small
+image slots support in the external memory ## 3.0.0 ### Added - Image SWAP
+using Status Partition ### Changed - CyBootloader 2.0 - Secure Flash Boot 4.0.2
 support ## 2.1.0 ### Added - Support PSoC64 1M - New command to read device die
 ID - Optionally add boot record to the signed image - New policy validators
 (address overlaps between images and bootloader, slots address alignment with
 the SMPU address limits, DAP closure, monotonic counter) - Log the device
 response JWT during the provisioning process ### Changed - Fixed issue with
 using group private key - Use pyocd 0.27.3 ## 2.0.0 ### Added - Support PSoC64
 2M, PSoC64 512K - Command line interface - Encrypted programming - Single-image
```

### Comparing `cysecuretools-4.2.0/docs/README_CYW20829.md` & `cysecuretools-5.0.0/docs/README_CYW20829.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,26 +36,25 @@
 * [Provisioning a device](#provision-a-device) - Provisioning is the act of configuring a device with an authorized set of keys, policies, and optionally certificates.
 * [Sign a user application](#sign-an-image) - Signs a user application with a private key locally or with a Hardware Security Module.
 * [Encrypt a user application](#encrypt-the-user-application) - Signs and encrypts a user application.
 * [Create a debug certificate](#create-debug-certificate) - The debug certificate is used by BootROM to enable CM33-AP and/or Sys-AP when it is temporarily disabled.
 
 
 # Quick start
-## 1. Set On-Chip debugger
+## 1. Set a path to the On-Chip debugger
 ```bash
 $ cysecuretools set-ocd --name openocd --path <PATH_TO_OPENOCD_ROOT_DIRECTORY>
 ```
 Make sure you provide the path to the root directory of OpenOCD (NOT _bin_ directory).
 Specifying the path is not mandatory if you have ModusToolbox™ installed on your machine. OpenOCD from the ModusToolbox™ directory is used by default.
 
 _Example:_
 ```bash
 $ cysecuretools set-ocd --name openocd --path /Users/username/tools/openocd
 ```
-_NOTE_: pyOCD is not currently supported for the CYW20829 device.
 
 ## 2. Define a target
 Run the following command and find the name of your target in the list of supported targets.
 ```bash
 $ cysecuretools device-list
 ```
 This target name will be used as a `-t` option value with each command.
```

### Comparing `cysecuretools-4.2.0/docs/README_PSOC64.md` & `cysecuretools-5.0.0/docs/README_PSOC64.md`

 * *Files 1% similar despite different names*

```diff
@@ -50,49 +50,37 @@
 * [Sign a user application](#sign-image) - To run a user application on a secure device, the application must be signed with the key provisioned to the device earlier.
 * [Create a certificate](#create-a-certificate) - Create a certificate in the X.509 format: with the device public key inside and signed with the private key. The certificate can be used when connecting to a cloud service.
 * [Create image certificate](#create-image-certificate) - Based on an image, create a JWT that certifies the image's validity.
 * [Output CyBootloader and Secure Flash Boot version](#output-cybootloader-and-secure-flash-boot-version) - Outputs CyBootloader and Secure Flash Boot version.
 
 
 # Quick start
-## 1. Set On-Chip debugger
+## 1. Set a path to the On-Chip debugger
 ```bash
-$ cysecuretools set-ocd --name <NAME> --path <PATH>
+$ cysecuretools set-ocd --name openocd --path <PATH_TO_OPENOCD_ROOT_DIRECTORY>
 ```
-To use PyOCD only name may be specified:
-
-_Example_:
-```bash
-$ cysecuretools set-ocd --name pyocd
-```
-To use OpenOCD specify both name and path to OpenOCD:
+Make sure you provide the path to the root directory of OpenOCD (NOT _bin_ directory).
+Specifying the path is not mandatory if you have ModusToolbox™ installed on your machine. OpenOCD from the ModusToolbox™ directory is used by default.
 
-_Example_:
+_Example:_
 ```bash
-$ cysecuretools set-ocd --name openocd --path <PATH>
+$ cysecuretools set-ocd --name openocd --path /Users/username/tools/openocd
 ```
 
-Make sure you provide the path to the root directory of OpenOCD (NOT _bin_ directory).
-Specifying the path is not mandatory if you have ModusToolbox™ installed on your machine. OpenOCD from the ModusToolbox™ directory is used by default.
-
 ## 2. Define a target
 Run the following command and find the name of your target in the list of supported targets.
 ```bash
 $ cysecuretools device-list
 ```
 This target name will be used as a `-t` option value with each command.
-If the device revision is not the latest one, use `--rev` option to specify a revision ([HW/SW compatibility](../README.md#hwsw-compatibility)).
 
 _Example_:
 ```bash
 $ cysecuretools -t CY8CKIT-064B0S2-4343W -p <POLICY> <COMMAND> [OPTIONS]
 ```
-```bash
-$ cysecuretools -t cyb06xx5 --rev a1 -p <POLICY> <COMMAND> [OPTIONS]
-```
 
 ## 3. Create a new project
 This copies the list of files required to start using the tool to the current working directory.
 ```bash
 $ cysecuretools -t <TARGET> init
 ```
 
@@ -406,15 +394,14 @@
 ### Command: `encrypt-image`
 ### Parameters
 | Name                  | Optional/Required  | Description   |
 | --------------------- |:------------------:| ------------- |
 | -i, --image           | required           | The image to encrypt. |
 | -h, --host-key-id     | required           | Host private key ID (4 - HSM, 5 - OEM). |
 | -d, --device-key-id   | required           | Device public key ID (1 - device, 12 - group). |
-| -a, --algorithm       | optional           | Asymmetric algorithm for key derivation function.   |
 | --key-length          | optional           | Derived key length. |
 | -o, --encrypted-image | required           | Output file of encrypted image for encrypted programming. |
 | --padding-value       | optional           | Value for image padding. |
 | --probe-id            | optional           | Probe serial number. Used to read device public key from device. |
 ### Usage example
 ```bash
 $ cysecuretools -t CY8CKIT-064B0S2-4343W -p policy/policy_single_CM0_CM4_swap.json encrypt-image -i BlinkyApp.hex -h 4 -d 1 -o encrypted_image.txt
@@ -671,17 +658,17 @@
 $ cysecuretools -t CY8CKIT-064B0S2-4343W extract-payload --image BlinkyApp_meta.bin --output BlinkyApp_payload.bin
 ```
 __IMPORTANT:__ in case of using image encryption, make sure to specify the decrypted payload to HSM. Image signature is calculated based on decrypted data.
 ```bash
 $ cysecuretools -t CY8CKIT-064B0S2-4343W extract-payload --image BlinkyApp_decrypted.bin --output BlinkyApp_payload.bin
 ```
 ### Step 6
-Use the tools provided by your HSM vendor to sign the extended image with the HSM. Save the signature returned by the HSM to a file. The format of the MCUboot signature is ASN.1 (binary decoded).
+Use the tools provided by your HSM vendor to sign the payload with the HSM. Save the signature returned by the HSM to a file. The format of the MCUboot signature is ASN.1 (binary decoded).
 ### Step 7
-Run the _add-signature_ command and provide the signature file created by the HSM. As an input image use the extended image created in the step #4.
+Run the _add-signature_ command and provide the signature file created by the HSM. As an input image use the image with metadata created in the step #4.
 ```bash
 $ cysecuretools -t CY8CKIT-064B0S2-4343W add-signature --image BlinkyApp_meta.bin --output BlinkyApp_signed.bin --signature ec_signature_asn.bin
 ```
 
 
 ## Closing All Access Ports
 Often it is necessary to close all access ports during provisioning. After closing the access ports, there will be no way to program application.
```

### Comparing `cysecuretools-4.2.0/setup.py` & `cysecuretools-5.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,46 +10,51 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from setuptools import setup, find_packages
+from setuptools import setup
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 with open('CHANGELOG.md', 'r', encoding='utf-8') as f:
     changelog = f.read()
 
-version = {}
-with open('cysecuretools/version.py', 'r', encoding='utf-8') as f:
-    exec(f.read(), version)  # pylint: disable=exec-used
+about = {}
+with open('src/__about__.py', 'r', encoding='utf-8') as f:
+    exec(f.read(), about)  # pylint: disable=exec-used
+
+version = about['__version__']
+package_name = about['__pkg_name__'].lower()
 
 setup(
-    name='cysecuretools',
-    version=version['__version__'],
+    name=package_name,
+    version=version,
+    packages=[package_name],
+    package_dir={package_name: 'src'},
     install_requires=[
         'setuptools==59.6.0',
         'cryptography==36.0.1',
         'click==8.0.4',
         'intelhex==2.3.0',
         'python-jose==3.3.0',
         'jsonschema>=4.0.0,<=4.4.0',
-        'pyocd==0.32.3',
         'cbor==1.0.0',
-        'packaging==21.3'
+        'packaging==21.3',
+        'lief>=0.12.3,<=0.13.1'
         ],
-    description='Cypress secure tools for Python',
+    description='Python tools for provisioning Cypress/Infineon MCUs',
     long_description=readme + '\n\n' + changelog,
     long_description_content_type='text/markdown',
-    author='Cypress Semiconductor',
-    url='https://github.com/cypresssemiconductorco/cysecuretools',
+    author='Cypress Semiconductor Corporation (an Infineon company)',
+    url='https://github.com/Infineon/cysecuretools',
     license='Apache 2.0',
     python_requires='>=3.6',
     include_package_data=True,  # include files from MANIFEST.in
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
@@ -57,17 +62,16 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Embedded Systems',
     ],
     entry_points={
         'console_scripts': [
-            'cysecuretools = cysecuretools.__main__:main',
+            f'cysecuretools = {package_name}.__main__:main',
         ],
     },
-    packages=find_packages(),
     options={
         'bdist_wheel': {
             'python_tag': 'py3',
         }
     }
 )
```

