# Comparing `tmp/sui_brownie-1.0.5-py3-none-any.whl.zip` & `tmp/sui_brownie-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 27906 bytes, number of entries: 16
+Zip file size: 28009 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       10 b- defN 22-Dec-02 09:41 sui_brownie/MANIFEST.in
 -rw-r--r--  2.0 unx      878 b- defN 23-Apr-01 13:03 sui_brownie/README.md
 -rw-r--r--  2.0 unx       38 b- defN 23-Apr-11 02:45 sui_brownie/__init__.py
 -rw-r--r--  2.0 unx     2514 b- defN 23-Apr-01 12:52 sui_brownie/account.py
 -rw-r--r--  2.0 unx    12144 b- defN 23-Apr-21 09:58 sui_brownie/bcs.py
 -rw-r--r--  2.0 unx     4326 b- defN 23-Apr-01 12:53 sui_brownie/ed25519.py
 -rw-r--r--  2.0 unx    10047 b- defN 22-Dec-02 09:41 sui_brownie/parallelism.py
--rw-r--r--  2.0 unx    94808 b- defN 23-Jun-07 02:58 sui_brownie/sui_brownie.py
+-rw-r--r--  2.0 unx    95593 b- defN 23-Jun-21 01:54 sui_brownie/sui_brownie.py
 -rw-r--r--  2.0 unx    32439 b- defN 23-Apr-19 08:03 sui_brownie/sui_client.py
 -rw-r--r--  2.0 unx      140 b- defN 22-Dec-02 09:41 sui_brownie/sui_config.template.yaml
 -rw-r--r--  2.0 unx       19 b- defN 22-Dec-02 09:41 sui_brownie/sui_keystore.template.keystore
 -rw-r--r--  2.0 unx      866 b- defN 23-Apr-11 02:45 sui_brownie/utils.py
--rw-r--r--  2.0 unx     1002 b- defN 23-Jun-07 02:58 sui_brownie-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 02:58 sui_brownie-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-07 02:58 sui_brownie-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1297 b- defN 23-Jun-07 02:58 sui_brownie-1.0.5.dist-info/RECORD
-16 files, 160632 bytes uncompressed, 25772 bytes compressed:  84.0%
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-21 01:57 sui_brownie-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 01:57 sui_brownie-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-21 01:57 sui_brownie-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1296 b- defN 23-Jun-21 01:57 sui_brownie-1.0.6.dist-info/RECORD
+16 files, 161396 bytes uncompressed, 25875 bytes compressed:  84.0%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sui_brownie/sui_keystore.template.keystore
 Comment: 
 
 Filename: sui_brownie/utils.py
 Comment: 
 
-Filename: sui_brownie-1.0.5.dist-info/METADATA
+Filename: sui_brownie-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: sui_brownie-1.0.5.dist-info/WHEEL
+Filename: sui_brownie-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: sui_brownie-1.0.5.dist-info/top_level.txt
+Filename: sui_brownie-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: sui_brownie-1.0.5.dist-info/RECORD
+Filename: sui_brownie-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sui_brownie/sui_brownie.py

```diff
@@ -863,14 +863,26 @@
                 assert isinstance(call_arg, Argument), f"Not support:{call_arg}"
                 actual_params_index = call_arg.value.v0
                 if call_arg.key == "Input" and not has_actual_params[actual_params_index]:
                     batch_call_args_index[len(batch_call_args)] = actual_params_index
                     batch_call_args.append(actual_params[actual_params_index])
                     batch_parameters.append(abi["parameters"][i])
                     has_actual_params[actual_params_index] = True
+                if "Struct" in abi["parameters"][i] and abi["parameters"][i]["Struct"]["address"] == "0x2" and \
+                        abi["parameters"][i]["Struct"]["module"] == "coin" \
+                        and abi["parameters"][i]["Struct"]["name"] == "Coin" and \
+                        abi["parameters"][i]["Struct"]["typeArguments"][0]["Struct"]['module'] == "sui":
+                    batch_commands.append(
+                        Command("SplitCoins", SplitCoins(
+                            Argument("GasCoin", NONE()),
+                            [call_arg]
+                        ))
+                    )
+                    call_args[i] = Argument("NestedResult", NestedResult(U16(len(batch_commands) - 1), U16(0)))
+                    batch_parameters[-1] = "U64"
             # generate commands
             type_arguments = [
                 cls.generate_type_arg(v) for v in type_args
             ]
             commands = [
                 Command("MoveCall", ProgrammableMoveCall(
                     ObjectID(package_id),
```

## Comparing `sui_brownie-1.0.5.dist-info/METADATA` & `sui_brownie-1.0.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sui-brownie
-Version: 1.0.5
+Version: 1.0.6
 Summary: Sui Package Tool
 Home-page: https://github.com/OmniBTC/DolaProtocol/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
@@ -24,9 +23,7 @@
 Requires-Dist: retrying
 Requires-Dist: mnemonic
 Requires-Dist: httpx
 Requires-Dist: python-dotenv
 Requires-Dist: pynacl
 
 This is an sui python tool to quickly implement sui calls
-
-
```

## Comparing `sui_brownie-1.0.5.dist-info/RECORD` & `sui_brownie-1.0.6.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 sui_brownie/MANIFEST.in,sha256=BzExY9sw9x0Pqk6SYHuMRRvYS-cm75AxBOBjsYGFfU4,10
 sui_brownie/README.md,sha256=-7DxT6cGHbWLr_VufOEwIzl4Vtojp5dZc_r89lwnK3o,878
 sui_brownie/__init__.py,sha256=ROrbn7qi0haZjB8FG5JqXpD5mQ6qQPDNOwe0-rPnKeM,38
 sui_brownie/account.py,sha256=suZRI__kDNhyuoCZ9_q4mIV673lJDz0jgj0HyEj_hsQ,2514
 sui_brownie/bcs.py,sha256=8LwJihqmjLGwtzq87XKAQhE7ZgxiRDUsUYRbK6yRy7s,12144
 sui_brownie/ed25519.py,sha256=8hLHtC21og60B3MzXi4JmdQoOCbUutExyQIJhypJ9dg,4326
 sui_brownie/parallelism.py,sha256=Thh7TUrRU1fn47lNTF30RrcL5lBPBeMT2DX9A_swXDg,10047
-sui_brownie/sui_brownie.py,sha256=IzdkmRLqCtcvPbnTy_V0QlE_c667iouBtQlqOAOMy-A,94808
+sui_brownie/sui_brownie.py,sha256=XrVjzYkPMmImDGwyXIOB3ERPd1UErnUNxVi0fEfNPw8,95593
 sui_brownie/sui_client.py,sha256=Epyu5pXAI6jl_L-lzBg4gnNLYQVjdQTZ8kR4YrJfnqk,32439
 sui_brownie/sui_config.template.yaml,sha256=Qa6n48nf4qeLDhZnpVNjZJIYDm8jYFs7dVLCyLjxMTs,140
 sui_brownie/sui_keystore.template.keystore,sha256=dIQsJL_H6FdnGlET9u5NYXSmjTc1-8dk8wZWKrzcLOM,19
 sui_brownie/utils.py,sha256=bttovGstKoozRoMvzYFOFs_z73aled7UFbNBDPxX9Uo,866
-sui_brownie-1.0.5.dist-info/METADATA,sha256=TVk2AymYjM6k9uUSJ-vgwRTNpkz_LtV5KNBkPYNCnj8,1002
-sui_brownie-1.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sui_brownie-1.0.5.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
-sui_brownie-1.0.5.dist-info/RECORD,,
+sui_brownie-1.0.6.dist-info/METADATA,sha256=OlFg0Zq4XoyHmnB3TNsJsclS0pR17B-5Ej6PHHr401A,982
+sui_brownie-1.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sui_brownie-1.0.6.dist-info/top_level.txt,sha256=Rh3-9xCv23H03EevKs1qJcZsUKCgFfOoxlhaDld3TdE,12
+sui_brownie-1.0.6.dist-info/RECORD,,
```

