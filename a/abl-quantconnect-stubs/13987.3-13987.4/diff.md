# Comparing `tmp/abl-quantconnect-stubs-13987.3.tar.gz` & `tmp/abl-quantconnect-stubs-13987.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abl-quantconnect-stubs-13987.3.tar", last modified: Wed Jun 21 03:43:40 2023, max compression
+gzip compressed data, was "abl-quantconnect-stubs-13987.4.tar", last modified: Wed Jun 21 04:49:55 2023, max compression
```

## Comparing `abl-quantconnect-stubs-13987.3.tar` & `abl-quantconnect-stubs-13987.4.tar`

### file list

```diff
@@ -1,645 +1,648 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.322899 abl-quantconnect-stubs-13987.3/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.594463 abl-quantconnect-stubs-13987.3/AlgorithmImports/
--rw-rw-rw-   0        0        0     3521 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/AlgorithmImports/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.597990 abl-quantconnect-stubs-13987.3/Calculators/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.600398 abl-quantconnect-stubs-13987.3/Calculators/DataType/
--rw-rw-rw-   0        0        0     1248 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/Calculators/DataType/__init__.py
--rw-rw-rw-   0        0        0     3354 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/Calculators/DataType/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.603908 abl-quantconnect-stubs-13987.3/Calculators/Estimators/
--rw-rw-rw-   0        0        0     1254 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/Calculators/Estimators/__init__.py
--rw-rw-rw-   0        0        0     1137 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/Calculators/Estimators/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.605920 abl-quantconnect-stubs-13987.3/Calculators/IO/
--rw-rw-rw-   0        0        0     1230 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/Calculators/IO/__init__.py
--rw-rw-rw-   0        0        0     2277 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/Calculators/IO/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.609168 abl-quantconnect-stubs-13987.3/Calculators/Margins/
--rw-rw-rw-   0        0        0     1245 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/Calculators/Margins/__init__.py
--rw-rw-rw-   0        0        0     5466 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/Calculators/Margins/__init__.pyi
--rw-rw-rw-   0        0        0     1221 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/Calculators/__init__.py
--rw-rw-rw-   0        0        0      229 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/Calculators/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.611168 abl-quantconnect-stubs-13987.3/FtxApi/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.614166 abl-quantconnect-stubs-13987.3/FtxApi/Rest/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.616681 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Enums/
--rw-rw-rw-   0        0        0     1234 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Enums/__init__.py
--rw-rw-rw-   0        0        0      551 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Enums/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.619115 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.622122 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/LeveragedTokens/
--rw-rw-rw-   0        0        0     1285 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/LeveragedTokens/__init__.py
--rw-rw-rw-   0        0        0     6913 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/LeveragedTokens/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.624525 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/Markets/
--rw-rw-rw-   0        0        0     1261 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/Markets/__init__.py
--rw-rw-rw-   0        0        0     3638 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/Markets/__init__.pyi
--rw-rw-rw-   0        0        0     1237 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/__init__.py
--rw-rw-rw-   0        0        0    33778 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/__init__.pyi
--rw-rw-rw-   0        0        0     1216 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/Rest/__init__.py
--rw-rw-rw-   0        0        0    10001 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/Rest/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.627043 abl-quantconnect-stubs-13987.3/FtxApi/WebSocket/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.630047 abl-quantconnect-stubs-13987.3/FtxApi/WebSocket/Models/
--rw-rw-rw-   0        0        0     1252 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/WebSocket/Models/__init__.py
--rw-rw-rw-   0        0        0     9468 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/WebSocket/Models/__init__.pyi
--rw-rw-rw-   0        0        0     1231 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/WebSocket/__init__.py
--rw-rw-rw-   0        0        0     5168 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/WebSocket/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.632038 abl-quantconnect-stubs-13987.3/FtxApi/WsEngine/
--rw-rw-rw-   0        0        0     1228 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/WsEngine/__init__.py
--rw-rw-rw-   0        0        0     2151 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/FtxApi/WsEngine/__init__.pyi
--rw-rw-rw-   0        0        0     1201 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/FtxApi/__init__.py
--rw-rw-rw-   0        0        0      772 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/FtxApi/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.635159 abl-quantconnect-stubs-13987.3/Internal/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.636676 abl-quantconnect-stubs-13987.3/Internal/Runtime/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.639048 abl-quantconnect-stubs-13987.3/Internal/Runtime/InteropServices/
--rw-rw-rw-   0        0        0     1281 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/Internal/Runtime/InteropServices/__init__.py
--rw-rw-rw-   0        0        0     1883 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/Internal/Runtime/InteropServices/__init__.pyi
--rw-rw-rw-   0        0        0     1233 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/Internal/Runtime/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.640422 abl-quantconnect-stubs-13987.3/Internal/Win32/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.641903 abl-quantconnect-stubs-13987.3/Internal/Win32/SafeHandles/
--rw-rw-rw-   0        0        0     1263 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/Internal/Win32/SafeHandles/__init__.py
--rw-rw-rw-   0        0        0     1227 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/Internal/Win32/__init__.py
--rw-rw-rw-   0        0        0     1209 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/Internal/__init__.py
--rw-rw-rw-   0        0        0      942 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/Internal/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.643052 abl-quantconnect-stubs-13987.3/MS/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.644062 abl-quantconnect-stubs-13987.3/MS/Internal/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.645759 abl-quantconnect-stubs-13987.3/MS/Internal/Xml/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.646767 abl-quantconnect-stubs-13987.3/MS/Internal/Xml/Linq/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.647768 abl-quantconnect-stubs-13987.3/MS/Internal/Xml/Linq/ComponentModel/
--rw-rw-rw-   0        0        0     1284 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/MS/Internal/Xml/Linq/ComponentModel/__init__.py
--rw-rw-rw-   0        0        0     1239 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/MS/Internal/Xml/Linq/__init__.py
--rw-rw-rw-   0        0        0     1224 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/MS/Internal/Xml/__init__.py
--rw-rw-rw-   0        0        0     1212 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/MS/Internal/__init__.py
--rw-rw-rw-   0        0        0     1185 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/MS/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.649777 abl-quantconnect-stubs-13987.3/Microsoft/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.650776 abl-quantconnect-stubs-13987.3/Microsoft/Win32/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.652776 abl-quantconnect-stubs-13987.3/Microsoft/Win32/SafeHandles/
--rw-rw-rw-   0        0        0     1267 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/Microsoft/Win32/SafeHandles/__init__.py
--rw-rw-rw-   0        0        0     3966 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/Microsoft/Win32/SafeHandles/__init__.pyi
--rw-rw-rw-   0        0        0     1231 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/Microsoft/Win32/__init__.py
--rw-rw-rw-   0        0        0     1213 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/Microsoft/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.654775 abl-quantconnect-stubs-13987.3/MomCrypto/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.657293 abl-quantconnect-stubs-13987.3/MomCrypto/Api/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.660301 abl-quantconnect-stubs-13987.3/MomCrypto/Api/Algorithm/
--rw-rw-rw-   0        0        0     1255 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/MomCrypto/Api/Algorithm/__init__.py
--rw-rw-rw-   0        0        0      812 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/MomCrypto/Api/Algorithm/__init__.pyi
--rw-rw-rw-   0        0        0     1225 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/MomCrypto/Api/__init__.py
--rw-rw-rw-   0        0        0   137897 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/MomCrypto/Api/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.663300 abl-quantconnect-stubs-13987.3/MomCrypto/DataApi/
--rw-rw-rw-   0        0        0     1237 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/MomCrypto/DataApi/__init__.py
--rw-rw-rw-   0        0        0     4524 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/MomCrypto/DataApi/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.665809 abl-quantconnect-stubs-13987.3/MomCrypto/Frontend/
--rw-rw-rw-   0        0        0     1240 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/MomCrypto/Frontend/__init__.py
--rw-rw-rw-   0        0        0     6025 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/MomCrypto/Frontend/__init__.pyi
--rw-rw-rw-   0        0        0     1213 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/MomCrypto/__init__.py
--rw-rw-rw-   0        0        0     1316 2023-06-21 03:43:40.321898 abl-quantconnect-stubs-13987.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.667827 abl-quantconnect-stubs-13987.3/QuantConnect/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.694923 abl-quantconnect-stubs-13987.3/QuantConnect/ABL/
--rw-rw-rw-   0        0        0     1237 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/ABL/__init__.py
--rw-rw-rw-   0        0        0    19882 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/ABL/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.698200 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.707585 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.709587 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.712005 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/DataType/
--rw-rw-rw-   0        0        0     1342 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/DataType/__init__.py
--rw-rw-rw-   0        0        0    10103 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/DataType/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.714587 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/PricingModels/
--rw-rw-rw-   0        0        0     1357 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/PricingModels/__init__.py
--rw-rw-rw-   0        0        0     2989 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/PricingModels/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.716654 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/Strategies/
--rw-rw-rw-   0        0        0     1348 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/Strategies/__init__.py
--rw-rw-rw-   0        0        0    35222 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/Strategies/__init__.pyi
--rw-rw-rw-   0        0        0     1315 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/__init__.py
--rw-rw-rw-   0        0        0     1276 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/__init__.py
--rw-rw-rw-   0        0        0   171777 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.718655 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.721656 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/AlgoTrade/
--rw-rw-rw-   0        0        0     1324 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/AlgoTrade/__init__.py
--rw-rw-rw-   0        0        0     2324 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/AlgoTrade/__init__.pyi
--rw-rw-rw-   0        0        0     1294 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.723655 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/tools/
--rw-rw-rw-   0        0        0     1312 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/tools/__init__.py
--rw-rw-rw-   0        0        0    11607 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/tools/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.727171 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.729291 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.732291 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.734786 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/Functions/
--rw-rw-rw-   0        0        0     1363 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/Functions/__init__.py
--rw-rw-rw-   0        0        0      679 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/Functions/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.737802 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/Providers/
--rw-rw-rw-   0        0        0     1363 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/Providers/__init__.py
--rw-rw-rw-   0        0        0     2071 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/Providers/__init__.pyi
--rw-rw-rw-   0        0        0     1333 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/__init__.py
--rw-rw-rw-   0        0        0    19575 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.741230 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Serialization/
--rw-rw-rw-   0        0        0     1348 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Serialization/__init__.py
--rw-rw-rw-   0        0        0     7906 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Serialization/__init__.pyi
--rw-rw-rw-   0        0        0     1306 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/__init__.py
--rw-rw-rw-   0        0        0    60354 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.743238 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Execution/
--rw-rw-rw-   0        0        0     1315 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Execution/__init__.py
--rw-rw-rw-   0        0        0    14111 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Execution/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.745747 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Portfolio/
--rw-rw-rw-   0        0        0     1315 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Portfolio/__init__.py
--rw-rw-rw-   0        0        0    87601 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Portfolio/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.748756 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Risk/
--rw-rw-rw-   0        0        0     1300 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Risk/__init__.py
--rw-rw-rw-   0        0        0    13855 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Risk/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.751778 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Selection/
--rw-rw-rw-   0        0        0     1315 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Selection/__init__.py
--rw-rw-rw-   0        0        0    50885 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Selection/__init__.pyi
--rw-rw-rw-   0        0        0     1285 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/__init__.py
--rw-rw-rw-   0        0        0     7060 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.754756 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Selection/
--rw-rw-rw-   0        0        0     1285 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Selection/__init__.py
--rw-rw-rw-   0        0        0     3855 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Selection/__init__.pyi
--rw-rw-rw-   0        0        0     1255 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/__init__.py
--rw-rw-rw-   0        0        0   364115 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.701387 abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.702550 abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/Python/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.705066 abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/Python/Wrappers/
--rw-rw-rw-   0        0        0     1324 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/Python/Wrappers/__init__.py
--rw-rw-rw-   0        0        0    27733 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/Python/Wrappers/__init__.pyi
--rw-rw-rw-   0        0        0     1297 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/Python/__init__.py
--rw-rw-rw-   0        0        0     1276 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/__init__.py
--rw-rw-rw-   0        0        0     5122 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.757768 abl-quantconnect-stubs-13987.3/QuantConnect/Api/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.760781 abl-quantconnect-stubs-13987.3/QuantConnect/Api/Serialization/
--rw-rw-rw-   0        0        0     1279 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Api/Serialization/__init__.py
--rw-rw-rw-   0        0        0     1818 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Api/Serialization/__init__.pyi
--rw-rw-rw-   0        0        0     1237 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Api/__init__.py
--rw-rw-rw-   0        0        0    89791 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Api/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.762808 abl-quantconnect-stubs-13987.3/QuantConnect/Benchmarks/
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Benchmarks/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Benchmarks/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.765934 abl-quantconnect-stubs-13987.3/QuantConnect/Brokerages/
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Brokerages/__init__.py
--rw-rw-rw-   0        0        0    80077 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Brokerages/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.768613 abl-quantconnect-stubs-13987.3/QuantConnect/Configuration/
--rw-rw-rw-   0        0        0     1267 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Configuration/__init__.py
--rw-rw-rw-   0        0        0     9823 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Configuration/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.771745 abl-quantconnect-stubs-13987.3/QuantConnect/Data/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.778057 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Auxiliary/
--rw-rw-rw-   0        0        0     1270 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Auxiliary/__init__.py
--rw-rw-rw-   0        0        0    56159 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Auxiliary/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.781489 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Consolidators/
--rw-rw-rw-   0        0        0     1282 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Consolidators/__init__.py
--rw-rw-rw-   0        0        0    60856 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Consolidators/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.784486 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.788016 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/AlphaStreams/
--rw-rw-rw-   0        0        0     1300 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/AlphaStreams/__init__.py
--rw-rw-rw-   0        0        0    10350 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/AlphaStreams/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.792013 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/IconicTypes/
--rw-rw-rw-   0        0        0     1297 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/IconicTypes/__init__.py
--rw-rw-rw-   0        0        0    11899 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/IconicTypes/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.795013 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/Intrinio/
--rw-rw-rw-   0        0        0     1288 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/Intrinio/__init__.py
--rw-rw-rw-   0        0        0    14156 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/Intrinio/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.797530 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/Tiingo/
--rw-rw-rw-   0        0        0     1282 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/Tiingo/__init__.py
--rw-rw-rw-   0        0        0     9264 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/Tiingo/__init__.pyi
--rw-rw-rw-   0        0        0     1261 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/__init__.py
--rw-rw-rw-   0        0        0     2853 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.800538 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Fundamental/
--rw-rw-rw-   0        0        0     1276 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Fundamental/__init__.py
--rw-rw-rw-   0        0        0  2258687 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Fundamental/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.811581 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Market/
--rw-rw-rw-   0        0        0     1261 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Market/__init__.py
--rw-rw-rw-   0        0        0   147856 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Market/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.814610 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Shortable/
--rw-rw-rw-   0        0        0     1270 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Shortable/__init__.py
--rw-rw-rw-   0        0        0     3280 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/Shortable/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.818137 abl-quantconnect-stubs-13987.3/QuantConnect/Data/UniverseSelection/
--rw-rw-rw-   0        0        0     1294 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/UniverseSelection/__init__.py
--rw-rw-rw-   0        0        0    97037 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/UniverseSelection/__init__.pyi
--rw-rw-rw-   0        0        0     1240 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/__init__.py
--rw-rw-rw-   0        0        0   105848 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Data/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.774199 abl-quantconnect-stubs-13987.3/QuantConnect/DataSource/
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/DataSource/__init__.py
--rw-rw-rw-   0        0        0      194 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/DataSource/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.820729 abl-quantconnect-stubs-13987.3/QuantConnect/Exceptions/
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Exceptions/__init__.py
--rw-rw-rw-   0        0        0    13451 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Exceptions/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.823737 abl-quantconnect-stubs-13987.3/QuantConnect/Indicators/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.826788 abl-quantconnect-stubs-13987.3/QuantConnect/Indicators/CandlestickPatterns/
--rw-rw-rw-   0        0        0     1318 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Indicators/CandlestickPatterns/__init__.py
--rw-rw-rw-   0        0        0    89280 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Indicators/CandlestickPatterns/__init__.pyi
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Indicators/__init__.py
--rw-rw-rw-   0        0        0   271769 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Indicators/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.829788 abl-quantconnect-stubs-13987.3/QuantConnect/Interfaces/
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Interfaces/__init__.py
--rw-rw-rw-   0        0        0   107861 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Interfaces/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.831788 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.835819 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.838839 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Alpha/
--rw-rw-rw-   0        0        0     1279 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Alpha/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Alpha/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.841839 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Alphas/
--rw-rw-rw-   0        0        0     1282 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Alphas/__init__.py
--rw-rw-rw-   0        0        0    14828 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Alphas/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.845838 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.849681 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Enumerators/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.852906 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Enumerators/Factories/
--rw-rw-rw-   0        0        0     1357 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Enumerators/Factories/__init__.py
--rw-rw-rw-   0        0        0    15757 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Enumerators/Factories/__init__.pyi
--rw-rw-rw-   0        0        0     1327 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Enumerators/__init__.py
--rw-rw-rw-   0        0        0    65002 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Enumerators/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.856425 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Queues/
--rw-rw-rw-   0        0        0     1312 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Queues/__init__.py
--rw-rw-rw-   0        0        0     3819 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Queues/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.859439 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Transport/
--rw-rw-rw-   0        0        0     1321 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Transport/__init__.py
--rw-rw-rw-   0        0        0     6804 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Transport/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.863435 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/WorkScheduling/
--rw-rw-rw-   0        0        0     1336 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/WorkScheduling/__init__.py
--rw-rw-rw-   0        0        0     3029 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/WorkScheduling/__init__.pyi
--rw-rw-rw-   0        0        0     1291 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/__init__.py
--rw-rw-rw-   0        0        0   121452 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.867093 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/HistoricalData/
--rw-rw-rw-   0        0        0     1306 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/HistoricalData/__init__.py
--rw-rw-rw-   0        0        0     7640 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/HistoricalData/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.870289 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/RealTime/
--rw-rw-rw-   0        0        0     1288 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/RealTime/__init__.py
--rw-rw-rw-   0        0        0    15114 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/RealTime/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.873382 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Results/
--rw-rw-rw-   0        0        0     1285 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Results/__init__.py
--rw-rw-rw-   0        0        0    52400 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Results/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.876907 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Server/
--rw-rw-rw-   0        0        0     1282 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Server/__init__.py
--rw-rw-rw-   0        0        0     4431 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Server/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.880246 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Setup/
--rw-rw-rw-   0        0        0     1279 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Setup/__init__.py
--rw-rw-rw-   0        0        0    18217 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Setup/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.884247 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Storage/
--rw-rw-rw-   0        0        0     1285 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Storage/__init__.py
--rw-rw-rw-   0        0        0     7556 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Storage/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.887770 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/TransactionHandlers/
--rw-rw-rw-   0        0        0     1321 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/TransactionHandlers/__init__.py
--rw-rw-rw-   0        0        0    16387 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/TransactionHandlers/__init__.pyi
--rw-rw-rw-   0        0        0     1261 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/__init__.py
--rw-rw-rw-   0        0        0    16909 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/__init__.pyi
--rw-rw-rw-   0        0        0     1240 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Lean/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.890767 abl-quantconnect-stubs-13987.3/QuantConnect/Logging/
--rw-rw-rw-   0        0        0     1249 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Logging/__init__.py
--rw-rw-rw-   0        0        0    14948 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Logging/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.894769 abl-quantconnect-stubs-13987.3/QuantConnect/Messaging/
--rw-rw-rw-   0        0        0     1255 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Messaging/__init__.py
--rw-rw-rw-   0        0        0     9814 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Messaging/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.898304 abl-quantconnect-stubs-13987.3/QuantConnect/Notifications/
--rw-rw-rw-   0        0        0     1267 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Notifications/__init__.py
--rw-rw-rw-   0        0        0    17007 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Notifications/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.901558 abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.905076 abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/Objectives/
--rw-rw-rw-   0        0        0     1288 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/Objectives/__init__.py
--rw-rw-rw-   0        0        0     6258 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/Objectives/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.908194 abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/Parameters/
--rw-rw-rw-   0        0        0     1288 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/Parameters/__init__.py
--rw-rw-rw-   0        0        0     5743 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/Parameters/__init__.pyi
--rw-rw-rw-   0        0        0     1255 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/__init__.py
--rw-rw-rw-   0        0        0      403 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.912276 abl-quantconnect-stubs-13987.3/QuantConnect/OptionQuote/
--rw-rw-rw-   0        0        0     1261 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/OptionQuote/__init__.py
--rw-rw-rw-   0        0        0     8033 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/OptionQuote/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.915597 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.918788 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Fees/
--rw-rw-rw-   0        0        0     1261 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Fees/__init__.py
--rw-rw-rw-   0        0        0    28821 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Fees/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.922276 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Fills/
--rw-rw-rw-   0        0        0     1264 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Fills/__init__.py
--rw-rw-rw-   0        0        0    17584 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Fills/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.925737 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/OptionExercise/
--rw-rw-rw-   0        0        0     1291 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/OptionExercise/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/OptionExercise/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.929746 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Serialization/
--rw-rw-rw-   0        0        0     1288 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Serialization/__init__.py
--rw-rw-rw-   0        0        0    17543 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Serialization/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.932746 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Slippage/
--rw-rw-rw-   0        0        0     1273 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Slippage/__init__.py
--rw-rw-rw-   0        0        0     2514 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Slippage/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.937264 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/TimeInForces/
--rw-rw-rw-   0        0        0     1285 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/TimeInForces/__init__.py
--rw-rw-rw-   0        0        0     3861 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/TimeInForces/__init__.pyi
--rw-rw-rw-   0        0        0     1246 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/__init__.py
--rw-rw-rw-   0        0        0    97990 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Orders/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.940275 abl-quantconnect-stubs-13987.3/QuantConnect/Packets/
--rw-rw-rw-   0        0        0     1249 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Packets/__init__.py
--rw-rw-rw-   0        0        0    67443 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Packets/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.944413 abl-quantconnect-stubs-13987.3/QuantConnect/Parameters/
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Parameters/__init__.py
--rw-rw-rw-   0        0        0     7438 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Parameters/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.947943 abl-quantconnect-stubs-13987.3/QuantConnect/Python/
--rw-rw-rw-   0        0        0     1246 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Python/__init__.py
--rw-rw-rw-   0        0        0    41145 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Python/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.952943 abl-quantconnect-stubs-13987.3/QuantConnect/Queues/
--rw-rw-rw-   0        0        0     1246 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Queues/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Queues/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.956453 abl-quantconnect-stubs-13987.3/QuantConnect/Report/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.960464 abl-quantconnect-stubs-13987.3/QuantConnect/Report/ReportElements/
--rw-rw-rw-   0        0        0     1291 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Report/ReportElements/__init__.py
--rw-rw-rw-   0        0        0     1847 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Report/ReportElements/__init__.pyi
--rw-rw-rw-   0        0        0     1246 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Report/__init__.py
--rw-rw-rw-   0        0        0    29787 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Report/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.963465 abl-quantconnect-stubs-13987.3/QuantConnect/Scheduling/
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Scheduling/__init__.py
--rw-rw-rw-   0        0        0    45704 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Scheduling/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.965973 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.970099 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Cfd/
--rw-rw-rw-   0        0        0     1270 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Cfd/__init__.py
--rw-rw-rw-   0        0        0     4734 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Cfd/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.973705 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Crypto/
--rw-rw-rw-   0        0        0     1279 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Crypto/__init__.py
--rw-rw-rw-   0        0        0     4788 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Crypto/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.978241 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/CurrencyConversion/
--rw-rw-rw-   0        0        0     1315 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/CurrencyConversion/__init__.py
--rw-rw-rw-   0        0        0     3680 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/CurrencyConversion/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.982260 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Equity/
--rw-rw-rw-   0        0        0     1279 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Equity/__init__.py
--rw-rw-rw-   0        0        0     5988 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Equity/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.985637 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Forex/
--rw-rw-rw-   0        0        0     1276 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Forex/__init__.py
--rw-rw-rw-   0        0        0     5649 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Forex/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.988654 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Future/
--rw-rw-rw-   0        0        0     1279 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Future/__init__.py
--rw-rw-rw-   0        0        0    31841 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Future/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.993807 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/FutureOption/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.996942 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/FutureOption/Api/
--rw-rw-rw-   0        0        0     1309 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/FutureOption/Api/__init__.py
--rw-rw-rw-   0        0        0     8802 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/FutureOption/Api/__init__.pyi
--rw-rw-rw-   0        0        0     1297 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/FutureOption/__init__.py
--rw-rw-rw-   0        0        0     5003 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/FutureOption/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.999935 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Index/
--rw-rw-rw-   0        0        0     1276 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Index/__init__.py
--rw-rw-rw-   0        0        0     4494 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Index/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.002936 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/IndexOption/
--rw-rw-rw-   0        0        0     1294 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/IndexOption/__init__.py
--rw-rw-rw-   0        0        0     3777 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/IndexOption/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.006026 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Interfaces/
--rw-rw-rw-   0        0        0     1291 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Interfaces/__init__.py
--rw-rw-rw-   0        0        0     3677 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Interfaces/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.008963 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Option/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.012205 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Option/StrategyMatcher/
--rw-rw-rw-   0        0        0     1327 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Option/StrategyMatcher/__init__.py
--rw-rw-rw-   0        0        0    62863 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Option/StrategyMatcher/__init__.pyi
--rw-rw-rw-   0        0        0     1279 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Option/__init__.py
--rw-rw-rw-   0        0        0    76753 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Option/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.015633 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Positions/
--rw-rw-rw-   0        0        0     1288 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Positions/__init__.py
--rw-rw-rw-   0        0        0    77338 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Positions/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.017973 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Volatility/
--rw-rw-rw-   0        0        0     1291 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Volatility/__init__.py
--rw-rw-rw-   0        0        0     3175 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Volatility/__init__.pyi
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/__init__.py
--rw-rw-rw-   0        0        0   309418 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Securities/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.022110 abl-quantconnect-stubs-13987.3/QuantConnect/Statistics/
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Statistics/__init__.py
--rw-rw-rw-   0        0        0    49509 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Statistics/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.025617 abl-quantconnect-stubs-13987.3/QuantConnect/Storage/
--rw-rw-rw-   0        0        0     1249 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Storage/__init__.py
--rw-rw-rw-   0        0        0     8697 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Storage/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.028628 abl-quantconnect-stubs-13987.3/QuantConnect/Util/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.032626 abl-quantconnect-stubs-13987.3/QuantConnect/Util/RateLimit/
--rw-rw-rw-   0        0        0     1270 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Util/RateLimit/__init__.py
--rw-rw-rw-   0        0        0     9089 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Util/RateLimit/__init__.pyi
--rw-rw-rw-   0        0        0     1240 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Util/__init__.py
--rw-rw-rw-   0        0        0   115046 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnect/Util/__init__.pyi
--rw-rw-rw-   0        0        0     1232 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/__init__.py
--rw-rw-rw-   0        0        0   279434 2023-06-21 03:43:30.000000 abl-quantconnect-stubs-13987.3/QuantConnect/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.670827 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.673826 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Model/
--rw-rw-rw-   0        0        0     1299 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Model/__init__.py
--rw-rw-rw-   0        0        0     8541 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Model/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.675826 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Parser/
--rw-rw-rw-   0        0        0     1302 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Parser/__init__.py
--rw-rw-rw-   0        0        0     7556 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Parser/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.680266 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Renderer/
--rw-rw-rw-   0        0        0     1308 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Renderer/__init__.py
--rw-rw-rw-   0        0        0     4542 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Renderer/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.683265 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.685774 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/Model/
--rw-rw-rw-   0        0        0     1317 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/Model/__init__.py
--rw-rw-rw-   0        0        0     2422 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/Model/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.689792 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/Utility/
--rw-rw-rw-   0        0        0     1323 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/Utility/__init__.py
--rw-rw-rw-   0        0        0      566 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/Utility/__init__.pyi
--rw-rw-rw-   0        0        0     1299 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:39.692021 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Utility/
--rw-rw-rw-   0        0        0     1305 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Utility/__init__.py
--rw-rw-rw-   0        0        0     1122 2023-06-21 03:43:32.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Utility/__init__.pyi
--rw-rw-rw-   0        0        0     1281 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/__init__.py
--rw-rw-rw-   0        0        0      310 2023-06-21 03:43:31.000000 abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.035626 abl-quantconnect-stubs-13987.3/System/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.039989 abl-quantconnect-stubs-13987.3/System/Buffers/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.042989 abl-quantconnect-stubs-13987.3/System/Buffers/Binary/
--rw-rw-rw-   0        0        0     1246 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Buffers/Binary/__init__.py
--rw-rw-rw-   0        0        0    24270 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Buffers/Binary/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.044988 abl-quantconnect-stubs-13987.3/System/Buffers/Text/
--rw-rw-rw-   0        0        0     1240 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Buffers/Text/__init__.py
--rw-rw-rw-   0        0        0    25180 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Buffers/Text/__init__.pyi
--rw-rw-rw-   0        0        0     1225 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Buffers/__init__.py
--rw-rw-rw-   0        0        0    10797 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Buffers/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.046496 abl-quantconnect-stubs-13987.3/System/CodeDom/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.049515 abl-quantconnect-stubs-13987.3/System/CodeDom/Compiler/
--rw-rw-rw-   0        0        0     1252 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/CodeDom/Compiler/__init__.py
--rw-rw-rw-   0        0        0     9830 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/CodeDom/Compiler/__init__.pyi
--rw-rw-rw-   0        0        0     1225 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/CodeDom/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.052513 abl-quantconnect-stubs-13987.3/System/Collections/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.056022 abl-quantconnect-stubs-13987.3/System/Collections/Concurrent/
--rw-rw-rw-   0        0        0     1270 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/Concurrent/__init__.py
--rw-rw-rw-   0        0        0    84433 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/Concurrent/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.059046 abl-quantconnect-stubs-13987.3/System/Collections/Generic/
--rw-rw-rw-   0        0        0     1261 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/Generic/__init__.py
--rw-rw-rw-   0        0        0   124954 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/Generic/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.062285 abl-quantconnect-stubs-13987.3/System/Collections/Immutable/
--rw-rw-rw-   0        0        0     1267 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/Immutable/__init__.py
--rw-rw-rw-   0        0        0   385223 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/Immutable/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.066011 abl-quantconnect-stubs-13987.3/System/Collections/ObjectModel/
--rw-rw-rw-   0        0        0     1273 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/ObjectModel/__init__.py
--rw-rw-rw-   0        0        0    30145 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/ObjectModel/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.069031 abl-quantconnect-stubs-13987.3/System/Collections/Specialized/
--rw-rw-rw-   0        0        0     1273 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/Specialized/__init__.py
--rw-rw-rw-   0        0        0     9141 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/Specialized/__init__.pyi
--rw-rw-rw-   0        0        0     1237 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/__init__.py
--rw-rw-rw-   0        0        0    21378 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Collections/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.072035 abl-quantconnect-stubs-13987.3/System/ComponentModel/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.075032 abl-quantconnect-stubs-13987.3/System/ComponentModel/DataAnnotations/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.078151 abl-quantconnect-stubs-13987.3/System/ComponentModel/DataAnnotations/Schema/
--rw-rw-rw-   0        0        0     1315 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/ComponentModel/DataAnnotations/Schema/__init__.py
--rw-rw-rw-   0        0        0     5432 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/ComponentModel/DataAnnotations/Schema/__init__.pyi
--rw-rw-rw-   0        0        0     1294 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/ComponentModel/DataAnnotations/__init__.py
--rw-rw-rw-   0        0        0    66033 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/ComponentModel/DataAnnotations/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.081154 abl-quantconnect-stubs-13987.3/System/ComponentModel/Design/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.084326 abl-quantconnect-stubs-13987.3/System/ComponentModel/Design/Serialization/
--rw-rw-rw-   0        0        0     1309 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/ComponentModel/Design/Serialization/__init__.py
--rw-rw-rw-   0        0        0    41818 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/ComponentModel/Design/Serialization/__init__.pyi
--rw-rw-rw-   0        0        0     1267 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/ComponentModel/Design/__init__.py
--rw-rw-rw-   0        0        0    90031 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/ComponentModel/Design/__init__.pyi
--rw-rw-rw-   0        0        0     1246 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/ComponentModel/__init__.py
--rw-rw-rw-   0        0        0   259337 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/ComponentModel/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.085833 abl-quantconnect-stubs-13987.3/System/Configuration/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.087924 abl-quantconnect-stubs-13987.3/System/Configuration/Assemblies/
--rw-rw-rw-   0        0        0     1276 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Configuration/Assemblies/__init__.py
--rw-rw-rw-   0        0        0      484 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Configuration/Assemblies/__init__.pyi
--rw-rw-rw-   0        0        0     1243 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Configuration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.091924 abl-quantconnect-stubs-13987.3/System/Diagnostics/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.093923 abl-quantconnect-stubs-13987.3/System/Diagnostics/CodeAnalysis/
--rw-rw-rw-   0        0        0     1276 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Diagnostics/CodeAnalysis/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Diagnostics/CodeAnalysis/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.097443 abl-quantconnect-stubs-13987.3/System/Diagnostics/Contracts/
--rw-rw-rw-   0        0        0     1267 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Diagnostics/Contracts/__init__.py
--rw-rw-rw-   0        0        0    15321 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Diagnostics/Contracts/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.101802 abl-quantconnect-stubs-13987.3/System/Diagnostics/SymbolStore/
--rw-rw-rw-   0        0        0     1273 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Diagnostics/SymbolStore/__init__.py
--rw-rw-rw-   0        0        0      397 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Diagnostics/SymbolStore/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.104245 abl-quantconnect-stubs-13987.3/System/Diagnostics/Tracing/
--rw-rw-rw-   0        0        0     1261 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Diagnostics/Tracing/__init__.py
--rw-rw-rw-   0        0        0    86639 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Diagnostics/Tracing/__init__.pyi
--rw-rw-rw-   0        0        0     1237 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Diagnostics/__init__.py
--rw-rw-rw-   0        0        0    31082 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Diagnostics/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.107791 abl-quantconnect-stubs-13987.3/System/Drawing/
--rw-rw-rw-   0        0        0     1225 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Drawing/__init__.py
--rw-rw-rw-   0        0        0    43297 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Drawing/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.110799 abl-quantconnect-stubs-13987.3/System/Globalization/
--rw-rw-rw-   0        0        0     1243 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Globalization/__init__.py
--rw-rw-rw-   0        0        0   137594 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Globalization/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.113552 abl-quantconnect-stubs-13987.3/System/IO/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.116804 abl-quantconnect-stubs-13987.3/System/IO/Enumeration/
--rw-rw-rw-   0        0        0     1246 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/IO/Enumeration/__init__.py
--rw-rw-rw-   0        0        0    11155 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/IO/Enumeration/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.118041 abl-quantconnect-stubs-13987.3/System/IO/Strategies/
--rw-rw-rw-   0        0        0     1243 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/IO/Strategies/__init__.py
--rw-rw-rw-   0        0        0     1210 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/IO/__init__.py
--rw-rw-rw-   0        0        0   142074 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/IO/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.121122 abl-quantconnect-stubs-13987.3/System/Linq/
--rw-rw-rw-   0        0        0     1216 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Linq/__init__.py
--rw-rw-rw-   0        0        0   111478 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Linq/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.124121 abl-quantconnect-stubs-13987.3/System/Net/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.127316 abl-quantconnect-stubs-13987.3/System/Net/Cache/
--rw-rw-rw-   0        0        0     1231 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Net/Cache/__init__.py
--rw-rw-rw-   0        0        0      811 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Net/Cache/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.130328 abl-quantconnect-stubs-13987.3/System/Net/NetworkInformation/
--rw-rw-rw-   0        0        0     1270 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Net/NetworkInformation/__init__.py
--rw-rw-rw-   0        0        0     1173 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Net/NetworkInformation/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.133740 abl-quantconnect-stubs-13987.3/System/Net/Security/
--rw-rw-rw-   0        0        0     1240 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Net/Security/__init__.py
--rw-rw-rw-   0        0        0      529 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Net/Security/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.136256 abl-quantconnect-stubs-13987.3/System/Net/Sockets/
--rw-rw-rw-   0        0        0     1237 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Net/Sockets/__init__.py
--rw-rw-rw-   0        0        0     3548 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Net/Sockets/__init__.pyi
--rw-rw-rw-   0        0        0     1213 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Net/__init__.py
--rw-rw-rw-   0        0        0    24710 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Net/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.139272 abl-quantconnect-stubs-13987.3/System/Numerics/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.141273 abl-quantconnect-stubs-13987.3/System/Numerics/Hashing/
--rw-rw-rw-   0        0        0     1252 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Numerics/Hashing/__init__.py
--rw-rw-rw-   0        0        0     1228 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Numerics/__init__.py
--rw-rw-rw-   0        0        0   251256 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Numerics/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.144274 abl-quantconnect-stubs-13987.3/System/Reflection/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.147109 abl-quantconnect-stubs-13987.3/System/Reflection/Emit/
--rw-rw-rw-   0        0        0     1249 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Reflection/Emit/__init__.py
--rw-rw-rw-   0        0        0    25180 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Reflection/Emit/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.150119 abl-quantconnect-stubs-13987.3/System/Reflection/Metadata/
--rw-rw-rw-   0        0        0     1261 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Reflection/Metadata/__init__.py
--rw-rw-rw-   0        0        0      672 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Reflection/Metadata/__init__.pyi
--rw-rw-rw-   0        0        0     1234 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Reflection/__init__.py
--rw-rw-rw-   0        0        0    97444 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Reflection/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.152664 abl-quantconnect-stubs-13987.3/System/Resources/
--rw-rw-rw-   0        0        0     1231 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Resources/__init__.py
--rw-rw-rw-   0        0        0     9590 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Resources/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.156182 abl-quantconnect-stubs-13987.3/System/Runtime/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.158404 abl-quantconnect-stubs-13987.3/System/Runtime/CompilerServices/
--rw-rw-rw-   0        0        0     1276 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/CompilerServices/__init__.py
--rw-rw-rw-   0        0        0    91271 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/CompilerServices/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.161405 abl-quantconnect-stubs-13987.3/System/Runtime/ConstrainedExecution/
--rw-rw-rw-   0        0        0     1288 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/ConstrainedExecution/__init__.py
--rw-rw-rw-   0        0        0     1511 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/ConstrainedExecution/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.164440 abl-quantconnect-stubs-13987.3/System/Runtime/ExceptionServices/
--rw-rw-rw-   0        0        0     1279 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/ExceptionServices/__init__.py
--rw-rw-rw-   0        0        0     1843 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/ExceptionServices/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.168064 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.171566 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/ComTypes/
--rw-rw-rw-   0        0        0     1300 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/ComTypes/__init__.py
--rw-rw-rw-   0        0        0    45970 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/ComTypes/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.174568 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/Marshalling/
--rw-rw-rw-   0        0        0     1309 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/Marshalling/__init__.py
--rw-rw-rw-   0        0        0    18435 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/Marshalling/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.180096 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/ObjectiveC/
--rw-rw-rw-   0        0        0     1306 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/ObjectiveC/__init__.py
--rw-rw-rw-   0        0        0     7264 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/ObjectiveC/__init__.pyi
--rw-rw-rw-   0        0        0     1273 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/__init__.py
--rw-rw-rw-   0        0        0   129933 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.184282 abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.193205 abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/Arm/
--rw-rw-rw-   0        0        0     1270 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/Arm/__init__.py
--rw-rw-rw-   0        0        0   911602 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/Arm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.198915 abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/X86/
--rw-rw-rw-   0        0        0     1270 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/X86/__init__.py
--rw-rw-rw-   0        0        0   863037 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/X86/__init__.pyi
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/__init__.py
--rw-rw-rw-   0        0        0   327049 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.202932 abl-quantconnect-stubs-13987.3/System/Runtime/Loader/
--rw-rw-rw-   0        0        0     1246 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Loader/__init__.py
--rw-rw-rw-   0        0        0     7228 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Loader/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.206083 abl-quantconnect-stubs-13987.3/System/Runtime/Remoting/
--rw-rw-rw-   0        0        0     1252 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Remoting/__init__.py
--rw-rw-rw-   0        0        0      311 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Remoting/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.208204 abl-quantconnect-stubs-13987.3/System/Runtime/Serialization/
--rw-rw-rw-   0        0        0     1267 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Serialization/__init__.py
--rw-rw-rw-   0        0        0    11408 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Serialization/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.211213 abl-quantconnect-stubs-13987.3/System/Runtime/Versioning/
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Versioning/__init__.py
--rw-rw-rw-   0        0        0     4083 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/Versioning/__init__.pyi
--rw-rw-rw-   0        0        0     1225 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/__init__.py
--rw-rw-rw-   0        0        0     3893 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Runtime/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.214213 abl-quantconnect-stubs-13987.3/System/Security/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.217112 abl-quantconnect-stubs-13987.3/System/Security/Authentication/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.221123 abl-quantconnect-stubs-13987.3/System/Security/Authentication/ExtendedProtection/
--rw-rw-rw-   0        0        0     1330 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/Authentication/ExtendedProtection/__init__.py
--rw-rw-rw-   0        0        0     1318 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/Authentication/ExtendedProtection/__init__.pyi
--rw-rw-rw-   0        0        0     1273 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/Authentication/__init__.py
--rw-rw-rw-   0        0        0     1076 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/Authentication/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.224219 abl-quantconnect-stubs-13987.3/System/Security/Cryptography/
--rw-rw-rw-   0        0        0     1267 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/Cryptography/__init__.py
--rw-rw-rw-   0        0        0      859 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/Cryptography/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.227734 abl-quantconnect-stubs-13987.3/System/Security/Permissions/
--rw-rw-rw-   0        0        0     1264 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/Permissions/__init__.py
--rw-rw-rw-   0        0        0     5209 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/Permissions/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.230735 abl-quantconnect-stubs-13987.3/System/Security/Principal/
--rw-rw-rw-   0        0        0     1258 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/Principal/__init__.py
--rw-rw-rw-   0        0        0     1131 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/Principal/__init__.pyi
--rw-rw-rw-   0        0        0     1228 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/__init__.py
--rw-rw-rw-   0        0        0    14504 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Security/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.233734 abl-quantconnect-stubs-13987.3/System/Text/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.237252 abl-quantconnect-stubs-13987.3/System/Text/RegularExpressions/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.239476 abl-quantconnect-stubs-13987.3/System/Text/RegularExpressions/Symbolic/
--rw-rw-rw-   0        0        0     1300 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Text/RegularExpressions/Symbolic/__init__.py
--rw-rw-rw-   0        0        0     1273 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Text/RegularExpressions/__init__.py
--rw-rw-rw-   0        0        0    64801 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Text/RegularExpressions/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.241509 abl-quantconnect-stubs-13987.3/System/Text/Unicode/
--rw-rw-rw-   0        0        0     1240 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Text/Unicode/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Text/__init__.py
--rw-rw-rw-   0        0        0    77244 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Text/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.244516 abl-quantconnect-stubs-13987.3/System/Threading/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.247032 abl-quantconnect-stubs-13987.3/System/Threading/Tasks/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.250141 abl-quantconnect-stubs-13987.3/System/Threading/Tasks/Sources/
--rw-rw-rw-   0        0        0     1273 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Threading/Tasks/Sources/__init__.py
--rw-rw-rw-   0        0        0     6944 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Threading/Tasks/Sources/__init__.pyi
--rw-rw-rw-   0        0        0     1249 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Threading/Tasks/__init__.py
--rw-rw-rw-   0        0        0   233718 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Threading/Tasks/__init__.pyi
--rw-rw-rw-   0        0        0     1231 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Threading/__init__.py
--rw-rw-rw-   0        0        0   120535 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Threading/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.254151 abl-quantconnect-stubs-13987.3/System/Timers/
--rw-rw-rw-   0        0        0     1222 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Timers/__init__.py
--rw-rw-rw-   0        0        0     5957 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Timers/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.255593 abl-quantconnect-stubs-13987.3/System/Windows/
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.258602 abl-quantconnect-stubs-13987.3/System/Windows/Input/
--rw-rw-rw-   0        0        0     1243 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Windows/Input/__init__.py
--rw-rw-rw-   0        0        0     2418 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Windows/Input/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.261602 abl-quantconnect-stubs-13987.3/System/Windows/Markup/
--rw-rw-rw-   0        0        0     1246 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Windows/Markup/__init__.py
--rw-rw-rw-   0        0        0     1390 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Windows/Markup/__init__.pyi
--rw-rw-rw-   0        0        0     1225 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/Windows/__init__.py
--rw-rw-rw-   0        0        0     1201 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/__init__.py
--rw-rw-rw-   0        0        0   901366 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/System/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.317899 abl-quantconnect-stubs-13987.3/abl_quantconnect_stubs.egg-info/
--rw-rw-rw-   0        0        0     1316 2023-06-21 03:43:36.000000 abl-quantconnect-stubs-13987.3/abl_quantconnect_stubs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17293 2023-06-21 03:43:39.000000 abl-quantconnect-stubs-13987.3/abl_quantconnect_stubs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 03:43:36.000000 abl-quantconnect-stubs-13987.3/abl_quantconnect_stubs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-21 03:43:36.000000 abl-quantconnect-stubs-13987.3/abl_quantconnect_stubs.egg-info/requires.txt
--rw-rw-rw-   0        0        0      119 2023-06-21 03:43:36.000000 abl-quantconnect-stubs-13987.3/abl_quantconnect_stubs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 03:43:40.318899 abl-quantconnect-stubs-13987.3/clr/
--rw-rw-rw-   0        0        0      446 2023-06-21 03:43:33.000000 abl-quantconnect-stubs-13987.3/clr/__init__.pyi
--rw-rw-rw-   0        0        0       42 2023-06-21 03:43:40.322899 abl-quantconnect-stubs-13987.3/setup.cfg
--rw-rw-rw-   0        0        0    23019 2023-06-21 03:43:34.000000 abl-quantconnect-stubs-13987.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.466831 abl-quantconnect-stubs-13987.4/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.692411 abl-quantconnect-stubs-13987.4/AlgorithmImports/
+-rw-rw-rw-   0        0        0     3521 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/AlgorithmImports/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.695526 abl-quantconnect-stubs-13987.4/Calculators/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.697839 abl-quantconnect-stubs-13987.4/Calculators/DataType/
+-rw-rw-rw-   0        0        0     1248 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/Calculators/DataType/__init__.py
+-rw-rw-rw-   0        0        0     3354 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/Calculators/DataType/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.700600 abl-quantconnect-stubs-13987.4/Calculators/Estimators/
+-rw-rw-rw-   0        0        0     1254 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/Calculators/Estimators/__init__.py
+-rw-rw-rw-   0        0        0     1137 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/Calculators/Estimators/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.702610 abl-quantconnect-stubs-13987.4/Calculators/IO/
+-rw-rw-rw-   0        0        0     1230 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/Calculators/IO/__init__.py
+-rw-rw-rw-   0        0        0     2277 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/Calculators/IO/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.705609 abl-quantconnect-stubs-13987.4/Calculators/Margins/
+-rw-rw-rw-   0        0        0     1245 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/Calculators/Margins/__init__.py
+-rw-rw-rw-   0        0        0     5466 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/Calculators/Margins/__init__.pyi
+-rw-rw-rw-   0        0        0     1221 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/Calculators/__init__.py
+-rw-rw-rw-   0        0        0      229 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/Calculators/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.708609 abl-quantconnect-stubs-13987.4/FtxApi/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.710610 abl-quantconnect-stubs-13987.4/FtxApi/Rest/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.713095 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Enums/
+-rw-rw-rw-   0        0        0     1234 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Enums/__init__.py
+-rw-rw-rw-   0        0        0      551 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Enums/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.716401 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.719528 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/LeveragedTokens/
+-rw-rw-rw-   0        0        0     1285 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/LeveragedTokens/__init__.py
+-rw-rw-rw-   0        0        0     6913 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/LeveragedTokens/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.722537 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/Markets/
+-rw-rw-rw-   0        0        0     1261 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/Markets/__init__.py
+-rw-rw-rw-   0        0        0     3638 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/Markets/__init__.pyi
+-rw-rw-rw-   0        0        0     1237 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/__init__.py
+-rw-rw-rw-   0        0        0    33778 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/__init__.pyi
+-rw-rw-rw-   0        0        0     1216 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/Rest/__init__.py
+-rw-rw-rw-   0        0        0    10001 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/Rest/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.724975 abl-quantconnect-stubs-13987.4/FtxApi/WebSocket/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.727476 abl-quantconnect-stubs-13987.4/FtxApi/WebSocket/Models/
+-rw-rw-rw-   0        0        0     1252 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/WebSocket/Models/__init__.py
+-rw-rw-rw-   0        0        0     9468 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/WebSocket/Models/__init__.pyi
+-rw-rw-rw-   0        0        0     1231 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/WebSocket/__init__.py
+-rw-rw-rw-   0        0        0     5168 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/WebSocket/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.729790 abl-quantconnect-stubs-13987.4/FtxApi/WsEngine/
+-rw-rw-rw-   0        0        0     1228 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/WsEngine/__init__.py
+-rw-rw-rw-   0        0        0     2151 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/FtxApi/WsEngine/__init__.pyi
+-rw-rw-rw-   0        0        0     1201 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/FtxApi/__init__.py
+-rw-rw-rw-   0        0        0      772 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/FtxApi/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.732380 abl-quantconnect-stubs-13987.4/Internal/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.733584 abl-quantconnect-stubs-13987.4/Internal/Runtime/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.736545 abl-quantconnect-stubs-13987.4/Internal/Runtime/InteropServices/
+-rw-rw-rw-   0        0        0     1281 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/Internal/Runtime/InteropServices/__init__.py
+-rw-rw-rw-   0        0        0     1883 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/Internal/Runtime/InteropServices/__init__.pyi
+-rw-rw-rw-   0        0        0     1233 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/Internal/Runtime/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.737739 abl-quantconnect-stubs-13987.4/Internal/Win32/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.739752 abl-quantconnect-stubs-13987.4/Internal/Win32/SafeHandles/
+-rw-rw-rw-   0        0        0     1263 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/Internal/Win32/SafeHandles/__init__.py
+-rw-rw-rw-   0        0        0     1227 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/Internal/Win32/__init__.py
+-rw-rw-rw-   0        0        0     1209 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/Internal/__init__.py
+-rw-rw-rw-   0        0        0      942 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/Internal/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.741748 abl-quantconnect-stubs-13987.4/MS/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.742748 abl-quantconnect-stubs-13987.4/MS/Internal/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.743748 abl-quantconnect-stubs-13987.4/MS/Internal/Xml/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.745747 abl-quantconnect-stubs-13987.4/MS/Internal/Xml/Linq/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.747096 abl-quantconnect-stubs-13987.4/MS/Internal/Xml/Linq/ComponentModel/
+-rw-rw-rw-   0        0        0     1284 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/MS/Internal/Xml/Linq/ComponentModel/__init__.py
+-rw-rw-rw-   0        0        0     1239 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/MS/Internal/Xml/Linq/__init__.py
+-rw-rw-rw-   0        0        0     1224 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/MS/Internal/Xml/__init__.py
+-rw-rw-rw-   0        0        0     1212 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/MS/Internal/__init__.py
+-rw-rw-rw-   0        0        0     1185 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/MS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.748107 abl-quantconnect-stubs-13987.4/Microsoft/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.749578 abl-quantconnect-stubs-13987.4/Microsoft/Win32/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.752788 abl-quantconnect-stubs-13987.4/Microsoft/Win32/SafeHandles/
+-rw-rw-rw-   0        0        0     1267 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/Microsoft/Win32/SafeHandles/__init__.py
+-rw-rw-rw-   0        0        0     3966 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/Microsoft/Win32/SafeHandles/__init__.pyi
+-rw-rw-rw-   0        0        0     1231 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/Microsoft/Win32/__init__.py
+-rw-rw-rw-   0        0        0     1213 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/Microsoft/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.753966 abl-quantconnect-stubs-13987.4/MomCrypto/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.757113 abl-quantconnect-stubs-13987.4/MomCrypto/Api/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.760113 abl-quantconnect-stubs-13987.4/MomCrypto/Api/Algorithm/
+-rw-rw-rw-   0        0        0     1255 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/MomCrypto/Api/Algorithm/__init__.py
+-rw-rw-rw-   0        0        0      812 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/MomCrypto/Api/Algorithm/__init__.pyi
+-rw-rw-rw-   0        0        0     1225 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/MomCrypto/Api/__init__.py
+-rw-rw-rw-   0        0        0   137897 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/MomCrypto/Api/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.763140 abl-quantconnect-stubs-13987.4/MomCrypto/DataApi/
+-rw-rw-rw-   0        0        0     1237 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/MomCrypto/DataApi/__init__.py
+-rw-rw-rw-   0        0        0     4524 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/MomCrypto/DataApi/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.766481 abl-quantconnect-stubs-13987.4/MomCrypto/Frontend/
+-rw-rw-rw-   0        0        0     1240 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/MomCrypto/Frontend/__init__.py
+-rw-rw-rw-   0        0        0     6025 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/MomCrypto/Frontend/__init__.pyi
+-rw-rw-rw-   0        0        0     1213 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/MomCrypto/__init__.py
+-rw-rw-rw-   0        0        0     1316 2023-06-21 04:49:55.465832 abl-quantconnect-stubs-13987.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.769853 abl-quantconnect-stubs-13987.4/QuantConnect/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.808351 abl-quantconnect-stubs-13987.4/QuantConnect/ABL/
+-rw-rw-rw-   0        0        0     1237 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/ABL/__init__.py
+-rw-rw-rw-   0        0        0    19882 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/ABL/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.822395 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.852911 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.854912 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.858024 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/DataType/
+-rw-rw-rw-   0        0        0     1342 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/DataType/__init__.py
+-rw-rw-rw-   0        0        0    10103 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/DataType/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.865528 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/PricingModels/
+-rw-rw-rw-   0        0        0     1357 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/PricingModels/__init__.py
+-rw-rw-rw-   0        0        0     2989 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/PricingModels/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.868528 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/Strategies/
+-rw-rw-rw-   0        0        0     1348 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/Strategies/__init__.py
+-rw-rw-rw-   0        0        0    35222 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/Strategies/__init__.pyi
+-rw-rw-rw-   0        0        0     1315 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/__init__.py
+-rw-rw-rw-   0        0        0     1276 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/__init__.py
+-rw-rw-rw-   0        0        0   171777 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.870680 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.872680 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/AlgoTrade/
+-rw-rw-rw-   0        0        0     1324 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/AlgoTrade/__init__.py
+-rw-rw-rw-   0        0        0     2324 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/AlgoTrade/__init__.pyi
+-rw-rw-rw-   0        0        0     1294 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.875679 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/tools/
+-rw-rw-rw-   0        0        0     1312 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/tools/__init__.py
+-rw-rw-rw-   0        0        0    11607 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/tools/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.878917 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.881949 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.884945 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.894864 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/Functions/
+-rw-rw-rw-   0        0        0     1363 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/Functions/__init__.py
+-rw-rw-rw-   0        0        0      679 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/Functions/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.897862 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/Providers/
+-rw-rw-rw-   0        0        0     1363 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/Providers/__init__.py
+-rw-rw-rw-   0        0        0     2071 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/Providers/__init__.pyi
+-rw-rw-rw-   0        0        0     1333 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/__init__.py
+-rw-rw-rw-   0        0        0    19575 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.899881 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Serialization/
+-rw-rw-rw-   0        0        0     1348 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Serialization/__init__.py
+-rw-rw-rw-   0        0        0     7906 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Serialization/__init__.pyi
+-rw-rw-rw-   0        0        0     1306 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/__init__.py
+-rw-rw-rw-   0        0        0    60354 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.902290 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Execution/
+-rw-rw-rw-   0        0        0     1315 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Execution/__init__.py
+-rw-rw-rw-   0        0        0    14111 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Execution/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.905712 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Portfolio/
+-rw-rw-rw-   0        0        0     1315 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Portfolio/__init__.py
+-rw-rw-rw-   0        0        0    87601 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Portfolio/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.909068 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Risk/
+-rw-rw-rw-   0        0        0     1300 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Risk/__init__.py
+-rw-rw-rw-   0        0        0    13855 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Risk/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.912079 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Selection/
+-rw-rw-rw-   0        0        0     1315 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Selection/__init__.py
+-rw-rw-rw-   0        0        0    50885 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Selection/__init__.pyi
+-rw-rw-rw-   0        0        0     1285 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/__init__.py
+-rw-rw-rw-   0        0        0     7060 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.915079 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Selection/
+-rw-rw-rw-   0        0        0     1285 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Selection/__init__.py
+-rw-rw-rw-   0        0        0     3855 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Selection/__init__.pyi
+-rw-rw-rw-   0        0        0     1255 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/__init__.py
+-rw-rw-rw-   0        0        0   364115 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.844465 abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.846902 abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/Python/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.849913 abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/Python/Wrappers/
+-rw-rw-rw-   0        0        0     1324 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/Python/Wrappers/__init__.py
+-rw-rw-rw-   0        0        0    27733 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/Python/Wrappers/__init__.pyi
+-rw-rw-rw-   0        0        0     1297 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/Python/__init__.py
+-rw-rw-rw-   0        0        0     1276 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/__init__.py
+-rw-rw-rw-   0        0        0     5122 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.922594 abl-quantconnect-stubs-13987.4/QuantConnect/Api/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.935591 abl-quantconnect-stubs-13987.4/QuantConnect/Api/Serialization/
+-rw-rw-rw-   0        0        0     1279 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Api/Serialization/__init__.py
+-rw-rw-rw-   0        0        0     1818 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Api/Serialization/__init__.pyi
+-rw-rw-rw-   0        0        0     1237 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Api/__init__.py
+-rw-rw-rw-   0        0        0    89791 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Api/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.937586 abl-quantconnect-stubs-13987.4/QuantConnect/Benchmarks/
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Benchmarks/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Benchmarks/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.940897 abl-quantconnect-stubs-13987.4/QuantConnect/Brokerages/
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Brokerages/__init__.py
+-rw-rw-rw-   0        0        0    80077 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Brokerages/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.943245 abl-quantconnect-stubs-13987.4/QuantConnect/Configuration/
+-rw-rw-rw-   0        0        0     1267 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Configuration/__init__.py
+-rw-rw-rw-   0        0        0     9823 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Configuration/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.945465 abl-quantconnect-stubs-13987.4/QuantConnect/Data/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.950670 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Auxiliary/
+-rw-rw-rw-   0        0        0     1270 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Auxiliary/__init__.py
+-rw-rw-rw-   0        0        0    56159 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Auxiliary/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.953912 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Consolidators/
+-rw-rw-rw-   0        0        0     1282 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Consolidators/__init__.py
+-rw-rw-rw-   0        0        0    60856 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Consolidators/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.956940 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.959078 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/AlphaStreams/
+-rw-rw-rw-   0        0        0     1300 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/AlphaStreams/__init__.py
+-rw-rw-rw-   0        0        0    10350 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/AlphaStreams/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.962080 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/IconicTypes/
+-rw-rw-rw-   0        0        0     1297 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/IconicTypes/__init__.py
+-rw-rw-rw-   0        0        0    11899 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/IconicTypes/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.964228 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/Intrinio/
+-rw-rw-rw-   0        0        0     1288 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/Intrinio/__init__.py
+-rw-rw-rw-   0        0        0    14156 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/Intrinio/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.967316 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/Tiingo/
+-rw-rw-rw-   0        0        0     1282 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/Tiingo/__init__.py
+-rw-rw-rw-   0        0        0     9264 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/Tiingo/__init__.pyi
+-rw-rw-rw-   0        0        0     1261 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/__init__.py
+-rw-rw-rw-   0        0        0     2853 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.970572 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Fundamental/
+-rw-rw-rw-   0        0        0     1276 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Fundamental/__init__.py
+-rw-rw-rw-   0        0        0  2258687 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Fundamental/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.977571 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Market/
+-rw-rw-rw-   0        0        0     1261 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Market/__init__.py
+-rw-rw-rw-   0        0        0   147856 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Market/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.980571 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Shortable/
+-rw-rw-rw-   0        0        0     1270 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Shortable/__init__.py
+-rw-rw-rw-   0        0        0     3280 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/Shortable/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.982817 abl-quantconnect-stubs-13987.4/QuantConnect/Data/UniverseSelection/
+-rw-rw-rw-   0        0        0     1294 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/UniverseSelection/__init__.py
+-rw-rw-rw-   0        0        0    97037 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/UniverseSelection/__init__.pyi
+-rw-rw-rw-   0        0        0     1240 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/__init__.py
+-rw-rw-rw-   0        0        0   105848 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Data/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.948643 abl-quantconnect-stubs-13987.4/QuantConnect/DataSource/
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/DataSource/__init__.py
+-rw-rw-rw-   0        0        0      194 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/DataSource/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.984827 abl-quantconnect-stubs-13987.4/QuantConnect/Exceptions/
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Exceptions/__init__.py
+-rw-rw-rw-   0        0        0    13451 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Exceptions/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.988136 abl-quantconnect-stubs-13987.4/QuantConnect/Indicators/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.992147 abl-quantconnect-stubs-13987.4/QuantConnect/Indicators/CandlestickPatterns/
+-rw-rw-rw-   0        0        0     1318 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Indicators/CandlestickPatterns/__init__.py
+-rw-rw-rw-   0        0        0    89280 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Indicators/CandlestickPatterns/__init__.pyi
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Indicators/__init__.py
+-rw-rw-rw-   0        0        0   271769 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Indicators/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.995147 abl-quantconnect-stubs-13987.4/QuantConnect/Interfaces/
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Interfaces/__init__.py
+-rw-rw-rw-   0        0        0   107861 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Interfaces/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.997150 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.999147 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.002455 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Alpha/
+-rw-rw-rw-   0        0        0     1279 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Alpha/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Alpha/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.005455 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Alphas/
+-rw-rw-rw-   0        0        0     1282 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Alphas/__init__.py
+-rw-rw-rw-   0        0        0    14828 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Alphas/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.008541 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.011520 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Enumerators/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.014531 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Enumerators/Factories/
+-rw-rw-rw-   0        0        0     1357 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Enumerators/Factories/__init__.py
+-rw-rw-rw-   0        0        0    15757 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Enumerators/Factories/__init__.pyi
+-rw-rw-rw-   0        0        0     1327 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Enumerators/__init__.py
+-rw-rw-rw-   0        0        0    65002 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Enumerators/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.017964 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Queues/
+-rw-rw-rw-   0        0        0     1312 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Queues/__init__.py
+-rw-rw-rw-   0        0        0     3819 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Queues/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.019963 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Transport/
+-rw-rw-rw-   0        0        0     1321 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Transport/__init__.py
+-rw-rw-rw-   0        0        0     6804 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Transport/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.021963 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/WorkScheduling/
+-rw-rw-rw-   0        0        0     1336 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/WorkScheduling/__init__.py
+-rw-rw-rw-   0        0        0     3029 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/WorkScheduling/__init__.pyi
+-rw-rw-rw-   0        0        0     1291 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/__init__.py
+-rw-rw-rw-   0        0        0   121452 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.024964 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/HistoricalData/
+-rw-rw-rw-   0        0        0     1306 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/HistoricalData/__init__.py
+-rw-rw-rw-   0        0        0     7640 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/HistoricalData/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.027825 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/RealTime/
+-rw-rw-rw-   0        0        0     1288 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/RealTime/__init__.py
+-rw-rw-rw-   0        0        0    15114 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/RealTime/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.029835 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Results/
+-rw-rw-rw-   0        0        0     1285 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Results/__init__.py
+-rw-rw-rw-   0        0        0    52400 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Results/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.032834 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Server/
+-rw-rw-rw-   0        0        0     1282 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Server/__init__.py
+-rw-rw-rw-   0        0        0     4431 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Server/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.035486 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Setup/
+-rw-rw-rw-   0        0        0     1279 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Setup/__init__.py
+-rw-rw-rw-   0        0        0    18217 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Setup/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.038445 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Storage/
+-rw-rw-rw-   0        0        0     1285 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Storage/__init__.py
+-rw-rw-rw-   0        0        0     7556 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Storage/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.041455 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/TransactionHandlers/
+-rw-rw-rw-   0        0        0     1321 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/TransactionHandlers/__init__.py
+-rw-rw-rw-   0        0        0    16387 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/TransactionHandlers/__init__.pyi
+-rw-rw-rw-   0        0        0     1261 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/__init__.py
+-rw-rw-rw-   0        0        0    16909 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/__init__.pyi
+-rw-rw-rw-   0        0        0     1240 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Lean/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.043929 abl-quantconnect-stubs-13987.4/QuantConnect/Logging/
+-rw-rw-rw-   0        0        0     1249 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Logging/__init__.py
+-rw-rw-rw-   0        0        0    14948 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Logging/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.046084 abl-quantconnect-stubs-13987.4/QuantConnect/Messaging/
+-rw-rw-rw-   0        0        0     1255 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Messaging/__init__.py
+-rw-rw-rw-   0        0        0     9814 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Messaging/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.048628 abl-quantconnect-stubs-13987.4/QuantConnect/Notifications/
+-rw-rw-rw-   0        0        0     1267 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Notifications/__init__.py
+-rw-rw-rw-   0        0        0    17007 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Notifications/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.051639 abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.054320 abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/Objectives/
+-rw-rw-rw-   0        0        0     1288 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/Objectives/__init__.py
+-rw-rw-rw-   0        0        0     6258 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/Objectives/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.057625 abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/Parameters/
+-rw-rw-rw-   0        0        0     1288 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/Parameters/__init__.py
+-rw-rw-rw-   0        0        0     5743 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/Parameters/__init__.pyi
+-rw-rw-rw-   0        0        0     1255 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.059625 abl-quantconnect-stubs-13987.4/QuantConnect/OptionQuote/
+-rw-rw-rw-   0        0        0     1261 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/OptionQuote/__init__.py
+-rw-rw-rw-   0        0        0     8033 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/OptionQuote/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.063624 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.065724 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Fees/
+-rw-rw-rw-   0        0        0     1261 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Fees/__init__.py
+-rw-rw-rw-   0        0        0    28821 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Fees/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.068162 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Fills/
+-rw-rw-rw-   0        0        0     1264 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Fills/__init__.py
+-rw-rw-rw-   0        0        0    17584 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Fills/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.070516 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/OptionExercise/
+-rw-rw-rw-   0        0        0     1291 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/OptionExercise/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/OptionExercise/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.072875 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Serialization/
+-rw-rw-rw-   0        0        0     1288 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Serialization/__init__.py
+-rw-rw-rw-   0        0        0    17543 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Serialization/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.075335 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Slippage/
+-rw-rw-rw-   0        0        0     1273 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Slippage/__init__.py
+-rw-rw-rw-   0        0        0     2514 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Slippage/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.077875 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/TimeInForces/
+-rw-rw-rw-   0        0        0     1285 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/TimeInForces/__init__.py
+-rw-rw-rw-   0        0        0     3861 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/TimeInForces/__init__.pyi
+-rw-rw-rw-   0        0        0     1246 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/__init__.py
+-rw-rw-rw-   0        0        0    97990 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Orders/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.080261 abl-quantconnect-stubs-13987.4/QuantConnect/Packets/
+-rw-rw-rw-   0        0        0     1249 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Packets/__init__.py
+-rw-rw-rw-   0        0        0    67443 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Packets/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.082255 abl-quantconnect-stubs-13987.4/QuantConnect/Parameters/
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Parameters/__init__.py
+-rw-rw-rw-   0        0        0     7438 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Parameters/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.085256 abl-quantconnect-stubs-13987.4/QuantConnect/Python/
+-rw-rw-rw-   0        0        0     1246 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Python/__init__.py
+-rw-rw-rw-   0        0        0    41145 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Python/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.086257 abl-quantconnect-stubs-13987.4/QuantConnect/Queues/
+-rw-rw-rw-   0        0        0     1246 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Queues/__init__.py
+-rw-rw-rw-   0        0        0     1127 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Queues/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.089490 abl-quantconnect-stubs-13987.4/QuantConnect/Report/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.091996 abl-quantconnect-stubs-13987.4/QuantConnect/Report/ReportElements/
+-rw-rw-rw-   0        0        0     1291 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Report/ReportElements/__init__.py
+-rw-rw-rw-   0        0        0     1847 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Report/ReportElements/__init__.pyi
+-rw-rw-rw-   0        0        0     1246 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Report/__init__.py
+-rw-rw-rw-   0        0        0    29787 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Report/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.098835 abl-quantconnect-stubs-13987.4/QuantConnect/Research/
+-rw-rw-rw-   0        0        0     1252 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Research/__init__.py
+-rw-rw-rw-   0        0        0    17193 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Research/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.104594 abl-quantconnect-stubs-13987.4/QuantConnect/Scheduling/
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Scheduling/__init__.py
+-rw-rw-rw-   0        0        0    45704 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Scheduling/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.107454 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.111455 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Cfd/
+-rw-rw-rw-   0        0        0     1270 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Cfd/__init__.py
+-rw-rw-rw-   0        0        0     4734 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Cfd/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.118107 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Crypto/
+-rw-rw-rw-   0        0        0     1279 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Crypto/__init__.py
+-rw-rw-rw-   0        0        0     4788 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Crypto/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.121582 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/CurrencyConversion/
+-rw-rw-rw-   0        0        0     1315 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/CurrencyConversion/__init__.py
+-rw-rw-rw-   0        0        0     3680 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/CurrencyConversion/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.124287 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Equity/
+-rw-rw-rw-   0        0        0     1279 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Equity/__init__.py
+-rw-rw-rw-   0        0        0     5988 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Equity/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.126296 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Forex/
+-rw-rw-rw-   0        0        0     1276 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Forex/__init__.py
+-rw-rw-rw-   0        0        0     5649 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Forex/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.129296 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Future/
+-rw-rw-rw-   0        0        0     1279 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Future/__init__.py
+-rw-rw-rw-   0        0        0    31841 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Future/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.131297 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/FutureOption/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.133296 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/FutureOption/Api/
+-rw-rw-rw-   0        0        0     1309 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/FutureOption/Api/__init__.py
+-rw-rw-rw-   0        0        0     8802 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/FutureOption/Api/__init__.pyi
+-rw-rw-rw-   0        0        0     1297 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/FutureOption/__init__.py
+-rw-rw-rw-   0        0        0     5003 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/FutureOption/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.135295 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Index/
+-rw-rw-rw-   0        0        0     1276 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Index/__init__.py
+-rw-rw-rw-   0        0        0     4494 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Index/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.141610 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/IndexOption/
+-rw-rw-rw-   0        0        0     1294 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/IndexOption/__init__.py
+-rw-rw-rw-   0        0        0     3777 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/IndexOption/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.146489 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Interfaces/
+-rw-rw-rw-   0        0        0     1291 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3677 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Interfaces/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.149498 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Option/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.152858 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Option/StrategyMatcher/
+-rw-rw-rw-   0        0        0     1327 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Option/StrategyMatcher/__init__.py
+-rw-rw-rw-   0        0        0    62863 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Option/StrategyMatcher/__init__.pyi
+-rw-rw-rw-   0        0        0     1279 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Option/__init__.py
+-rw-rw-rw-   0        0        0    76753 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Option/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.163935 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Positions/
+-rw-rw-rw-   0        0        0     1288 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Positions/__init__.py
+-rw-rw-rw-   0        0        0    77338 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Positions/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.169933 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Volatility/
+-rw-rw-rw-   0        0        0     1291 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Volatility/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Volatility/__init__.pyi
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/__init__.py
+-rw-rw-rw-   0        0        0   309418 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Securities/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.175934 abl-quantconnect-stubs-13987.4/QuantConnect/Statistics/
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Statistics/__init__.py
+-rw-rw-rw-   0        0        0    49509 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Statistics/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.180966 abl-quantconnect-stubs-13987.4/QuantConnect/Storage/
+-rw-rw-rw-   0        0        0     1249 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Storage/__init__.py
+-rw-rw-rw-   0        0        0     8697 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Storage/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.183472 abl-quantconnect-stubs-13987.4/QuantConnect/Util/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.185987 abl-quantconnect-stubs-13987.4/QuantConnect/Util/RateLimit/
+-rw-rw-rw-   0        0        0     1270 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Util/RateLimit/__init__.py
+-rw-rw-rw-   0        0        0     9089 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Util/RateLimit/__init__.pyi
+-rw-rw-rw-   0        0        0     1240 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Util/__init__.py
+-rw-rw-rw-   0        0        0   115046 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/Util/__init__.pyi
+-rw-rw-rw-   0        0        0     1232 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/__init__.py
+-rw-rw-rw-   0        0        0   279434 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnect/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.774005 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.777013 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Model/
+-rw-rw-rw-   0        0        0     1299 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Model/__init__.py
+-rw-rw-rw-   0        0        0     8541 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Model/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.779234 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Parser/
+-rw-rw-rw-   0        0        0     1302 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Parser/__init__.py
+-rw-rw-rw-   0        0        0     7556 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Parser/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.783762 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Renderer/
+-rw-rw-rw-   0        0        0     1308 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Renderer/__init__.py
+-rw-rw-rw-   0        0        0     4542 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Renderer/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.785760 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.788760 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/Model/
+-rw-rw-rw-   0        0        0     1317 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/Model/__init__.py
+-rw-rw-rw-   0        0        0     2422 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/Model/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.792189 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/Utility/
+-rw-rw-rw-   0        0        0     1323 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/Utility/__init__.py
+-rw-rw-rw-   0        0        0      566 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/Utility/__init__.pyi
+-rw-rw-rw-   0        0        0     1299 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:54.795180 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Utility/
+-rw-rw-rw-   0        0        0     1305 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Utility/__init__.py
+-rw-rw-rw-   0        0        0     1122 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Utility/__init__.pyi
+-rw-rw-rw-   0        0        0     1281 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/__init__.py
+-rw-rw-rw-   0        0        0      310 2023-06-21 04:49:46.000000 abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.188262 abl-quantconnect-stubs-13987.4/System/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.192481 abl-quantconnect-stubs-13987.4/System/Buffers/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.194725 abl-quantconnect-stubs-13987.4/System/Buffers/Binary/
+-rw-rw-rw-   0        0        0     1246 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Buffers/Binary/__init__.py
+-rw-rw-rw-   0        0        0    24270 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Buffers/Binary/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.195915 abl-quantconnect-stubs-13987.4/System/Buffers/Text/
+-rw-rw-rw-   0        0        0     1240 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Buffers/Text/__init__.py
+-rw-rw-rw-   0        0        0    25180 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Buffers/Text/__init__.pyi
+-rw-rw-rw-   0        0        0     1225 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/System/Buffers/__init__.py
+-rw-rw-rw-   0        0        0    10797 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/System/Buffers/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.198362 abl-quantconnect-stubs-13987.4/System/CodeDom/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.200659 abl-quantconnect-stubs-13987.4/System/CodeDom/Compiler/
+-rw-rw-rw-   0        0        0     1252 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/CodeDom/Compiler/__init__.py
+-rw-rw-rw-   0        0        0     9830 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/CodeDom/Compiler/__init__.pyi
+-rw-rw-rw-   0        0        0     1225 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/CodeDom/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.204669 abl-quantconnect-stubs-13987.4/System/Collections/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.208670 abl-quantconnect-stubs-13987.4/System/Collections/Concurrent/
+-rw-rw-rw-   0        0        0     1270 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/Concurrent/__init__.py
+-rw-rw-rw-   0        0        0    84433 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/Concurrent/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.215673 abl-quantconnect-stubs-13987.4/System/Collections/Generic/
+-rw-rw-rw-   0        0        0     1261 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/Generic/__init__.py
+-rw-rw-rw-   0        0        0   124954 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/Generic/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.219669 abl-quantconnect-stubs-13987.4/System/Collections/Immutable/
+-rw-rw-rw-   0        0        0     1267 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/Immutable/__init__.py
+-rw-rw-rw-   0        0        0   385223 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/Immutable/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.223975 abl-quantconnect-stubs-13987.4/System/Collections/ObjectModel/
+-rw-rw-rw-   0        0        0     1273 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/ObjectModel/__init__.py
+-rw-rw-rw-   0        0        0    30145 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/ObjectModel/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.228452 abl-quantconnect-stubs-13987.4/System/Collections/Specialized/
+-rw-rw-rw-   0        0        0     1273 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/Specialized/__init__.py
+-rw-rw-rw-   0        0        0     9141 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/Specialized/__init__.pyi
+-rw-rw-rw-   0        0        0     1237 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/__init__.py
+-rw-rw-rw-   0        0        0    21378 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Collections/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.230670 abl-quantconnect-stubs-13987.4/System/ComponentModel/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.233879 abl-quantconnect-stubs-13987.4/System/ComponentModel/DataAnnotations/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.238351 abl-quantconnect-stubs-13987.4/System/ComponentModel/DataAnnotations/Schema/
+-rw-rw-rw-   0        0        0     1315 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/ComponentModel/DataAnnotations/Schema/__init__.py
+-rw-rw-rw-   0        0        0     5432 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/ComponentModel/DataAnnotations/Schema/__init__.pyi
+-rw-rw-rw-   0        0        0     1294 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/ComponentModel/DataAnnotations/__init__.py
+-rw-rw-rw-   0        0        0    66033 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/ComponentModel/DataAnnotations/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.241351 abl-quantconnect-stubs-13987.4/System/ComponentModel/Design/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.244350 abl-quantconnect-stubs-13987.4/System/ComponentModel/Design/Serialization/
+-rw-rw-rw-   0        0        0     1309 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/ComponentModel/Design/Serialization/__init__.py
+-rw-rw-rw-   0        0        0    41818 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/ComponentModel/Design/Serialization/__init__.pyi
+-rw-rw-rw-   0        0        0     1267 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/ComponentModel/Design/__init__.py
+-rw-rw-rw-   0        0        0    90031 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/ComponentModel/Design/__init__.pyi
+-rw-rw-rw-   0        0        0     1246 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/ComponentModel/__init__.py
+-rw-rw-rw-   0        0        0   259337 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/ComponentModel/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.245350 abl-quantconnect-stubs-13987.4/System/Configuration/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.249351 abl-quantconnect-stubs-13987.4/System/Configuration/Assemblies/
+-rw-rw-rw-   0        0        0     1276 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Configuration/Assemblies/__init__.py
+-rw-rw-rw-   0        0        0      484 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Configuration/Assemblies/__init__.pyi
+-rw-rw-rw-   0        0        0     1243 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Configuration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.252863 abl-quantconnect-stubs-13987.4/System/Diagnostics/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.254861 abl-quantconnect-stubs-13987.4/System/Diagnostics/CodeAnalysis/
+-rw-rw-rw-   0        0        0     1276 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Diagnostics/CodeAnalysis/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Diagnostics/CodeAnalysis/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.257861 abl-quantconnect-stubs-13987.4/System/Diagnostics/Contracts/
+-rw-rw-rw-   0        0        0     1267 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Diagnostics/Contracts/__init__.py
+-rw-rw-rw-   0        0        0    15321 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Diagnostics/Contracts/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.259954 abl-quantconnect-stubs-13987.4/System/Diagnostics/SymbolStore/
+-rw-rw-rw-   0        0        0     1273 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Diagnostics/SymbolStore/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Diagnostics/SymbolStore/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.261963 abl-quantconnect-stubs-13987.4/System/Diagnostics/Tracing/
+-rw-rw-rw-   0        0        0     1261 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Diagnostics/Tracing/__init__.py
+-rw-rw-rw-   0        0        0    86639 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Diagnostics/Tracing/__init__.pyi
+-rw-rw-rw-   0        0        0     1237 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Diagnostics/__init__.py
+-rw-rw-rw-   0        0        0    31082 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Diagnostics/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.264629 abl-quantconnect-stubs-13987.4/System/Drawing/
+-rw-rw-rw-   0        0        0     1225 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Drawing/__init__.py
+-rw-rw-rw-   0        0        0    43297 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Drawing/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.268118 abl-quantconnect-stubs-13987.4/System/Globalization/
+-rw-rw-rw-   0        0        0     1243 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Globalization/__init__.py
+-rw-rw-rw-   0        0        0   137594 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Globalization/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.272119 abl-quantconnect-stubs-13987.4/System/IO/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.275117 abl-quantconnect-stubs-13987.4/System/IO/Enumeration/
+-rw-rw-rw-   0        0        0     1246 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/IO/Enumeration/__init__.py
+-rw-rw-rw-   0        0        0    11155 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/IO/Enumeration/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.276142 abl-quantconnect-stubs-13987.4/System/IO/Strategies/
+-rw-rw-rw-   0        0        0     1243 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/IO/Strategies/__init__.py
+-rw-rw-rw-   0        0        0     1210 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/IO/__init__.py
+-rw-rw-rw-   0        0        0   142074 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/IO/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.278714 abl-quantconnect-stubs-13987.4/System/Linq/
+-rw-rw-rw-   0        0        0     1216 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Linq/__init__.py
+-rw-rw-rw-   0        0        0   111478 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Linq/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.283863 abl-quantconnect-stubs-13987.4/System/Net/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.286868 abl-quantconnect-stubs-13987.4/System/Net/Cache/
+-rw-rw-rw-   0        0        0     1231 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Net/Cache/__init__.py
+-rw-rw-rw-   0        0        0      811 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Net/Cache/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.290271 abl-quantconnect-stubs-13987.4/System/Net/NetworkInformation/
+-rw-rw-rw-   0        0        0     1270 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Net/NetworkInformation/__init__.py
+-rw-rw-rw-   0        0        0     1173 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Net/NetworkInformation/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.292984 abl-quantconnect-stubs-13987.4/System/Net/Security/
+-rw-rw-rw-   0        0        0     1240 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Net/Security/__init__.py
+-rw-rw-rw-   0        0        0      529 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Net/Security/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.294402 abl-quantconnect-stubs-13987.4/System/Net/Sockets/
+-rw-rw-rw-   0        0        0     1237 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Net/Sockets/__init__.py
+-rw-rw-rw-   0        0        0     3548 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Net/Sockets/__init__.pyi
+-rw-rw-rw-   0        0        0     1213 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Net/__init__.py
+-rw-rw-rw-   0        0        0    24710 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Net/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.298129 abl-quantconnect-stubs-13987.4/System/Numerics/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.300127 abl-quantconnect-stubs-13987.4/System/Numerics/Hashing/
+-rw-rw-rw-   0        0        0     1252 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Numerics/Hashing/__init__.py
+-rw-rw-rw-   0        0        0     1228 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Numerics/__init__.py
+-rw-rw-rw-   0        0        0   251256 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Numerics/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.302128 abl-quantconnect-stubs-13987.4/System/Reflection/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.305126 abl-quantconnect-stubs-13987.4/System/Reflection/Emit/
+-rw-rw-rw-   0        0        0     1249 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Reflection/Emit/__init__.py
+-rw-rw-rw-   0        0        0    25180 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Reflection/Emit/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.307541 abl-quantconnect-stubs-13987.4/System/Reflection/Metadata/
+-rw-rw-rw-   0        0        0     1261 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Reflection/Metadata/__init__.py
+-rw-rw-rw-   0        0        0      672 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Reflection/Metadata/__init__.pyi
+-rw-rw-rw-   0        0        0     1234 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Reflection/__init__.py
+-rw-rw-rw-   0        0        0    97444 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Reflection/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.309551 abl-quantconnect-stubs-13987.4/System/Resources/
+-rw-rw-rw-   0        0        0     1231 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Resources/__init__.py
+-rw-rw-rw-   0        0        0     9590 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Resources/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.312551 abl-quantconnect-stubs-13987.4/System/Runtime/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.315779 abl-quantconnect-stubs-13987.4/System/Runtime/CompilerServices/
+-rw-rw-rw-   0        0        0     1276 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/CompilerServices/__init__.py
+-rw-rw-rw-   0        0        0    91271 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/CompilerServices/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.321406 abl-quantconnect-stubs-13987.4/System/Runtime/ConstrainedExecution/
+-rw-rw-rw-   0        0        0     1288 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/ConstrainedExecution/__init__.py
+-rw-rw-rw-   0        0        0     1511 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/ConstrainedExecution/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.325857 abl-quantconnect-stubs-13987.4/System/Runtime/ExceptionServices/
+-rw-rw-rw-   0        0        0     1279 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/ExceptionServices/__init__.py
+-rw-rw-rw-   0        0        0     1843 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/ExceptionServices/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.328700 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.331813 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/ComTypes/
+-rw-rw-rw-   0        0        0     1300 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/ComTypes/__init__.py
+-rw-rw-rw-   0        0        0    45970 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/ComTypes/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.333851 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/Marshalling/
+-rw-rw-rw-   0        0        0     1309 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/Marshalling/__init__.py
+-rw-rw-rw-   0        0        0    18435 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/Marshalling/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.336125 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/ObjectiveC/
+-rw-rw-rw-   0        0        0     1306 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/ObjectiveC/__init__.py
+-rw-rw-rw-   0        0        0     7264 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/ObjectiveC/__init__.pyi
+-rw-rw-rw-   0        0        0     1273 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/__init__.py
+-rw-rw-rw-   0        0        0   129933 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.339603 abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.342888 abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/Arm/
+-rw-rw-rw-   0        0        0     1270 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/Arm/__init__.py
+-rw-rw-rw-   0        0        0   911602 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/Arm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.346899 abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/X86/
+-rw-rw-rw-   0        0        0     1270 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/X86/__init__.py
+-rw-rw-rw-   0        0        0   863037 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/X86/__init__.pyi
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/__init__.py
+-rw-rw-rw-   0        0        0   327049 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.351899 abl-quantconnect-stubs-13987.4/System/Runtime/Loader/
+-rw-rw-rw-   0        0        0     1246 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Loader/__init__.py
+-rw-rw-rw-   0        0        0     7228 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Loader/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.354906 abl-quantconnect-stubs-13987.4/System/Runtime/Remoting/
+-rw-rw-rw-   0        0        0     1252 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Remoting/__init__.py
+-rw-rw-rw-   0        0        0      311 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Remoting/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.357923 abl-quantconnect-stubs-13987.4/System/Runtime/Serialization/
+-rw-rw-rw-   0        0        0     1267 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Serialization/__init__.py
+-rw-rw-rw-   0        0        0    11408 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Serialization/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.360401 abl-quantconnect-stubs-13987.4/System/Runtime/Versioning/
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Versioning/__init__.py
+-rw-rw-rw-   0        0        0     4083 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/Versioning/__init__.pyi
+-rw-rw-rw-   0        0        0     1225 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/__init__.py
+-rw-rw-rw-   0        0        0     3893 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Runtime/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.363659 abl-quantconnect-stubs-13987.4/System/Security/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.365938 abl-quantconnect-stubs-13987.4/System/Security/Authentication/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.369077 abl-quantconnect-stubs-13987.4/System/Security/Authentication/ExtendedProtection/
+-rw-rw-rw-   0        0        0     1330 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/Authentication/ExtendedProtection/__init__.py
+-rw-rw-rw-   0        0        0     1318 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/Authentication/ExtendedProtection/__init__.pyi
+-rw-rw-rw-   0        0        0     1273 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/Authentication/__init__.py
+-rw-rw-rw-   0        0        0     1076 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/Authentication/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.370077 abl-quantconnect-stubs-13987.4/System/Security/Cryptography/
+-rw-rw-rw-   0        0        0     1267 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/Cryptography/__init__.py
+-rw-rw-rw-   0        0        0      859 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/Cryptography/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.373579 abl-quantconnect-stubs-13987.4/System/Security/Permissions/
+-rw-rw-rw-   0        0        0     1264 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/Permissions/__init__.py
+-rw-rw-rw-   0        0        0     5209 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/Permissions/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.375746 abl-quantconnect-stubs-13987.4/System/Security/Principal/
+-rw-rw-rw-   0        0        0     1258 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/Principal/__init__.py
+-rw-rw-rw-   0        0        0     1131 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/Principal/__init__.pyi
+-rw-rw-rw-   0        0        0     1228 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/__init__.py
+-rw-rw-rw-   0        0        0    14504 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Security/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.377881 abl-quantconnect-stubs-13987.4/System/Text/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.379883 abl-quantconnect-stubs-13987.4/System/Text/RegularExpressions/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.381883 abl-quantconnect-stubs-13987.4/System/Text/RegularExpressions/Symbolic/
+-rw-rw-rw-   0        0        0     1300 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Text/RegularExpressions/Symbolic/__init__.py
+-rw-rw-rw-   0        0        0     1273 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Text/RegularExpressions/__init__.py
+-rw-rw-rw-   0        0        0    64801 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Text/RegularExpressions/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.383036 abl-quantconnect-stubs-13987.4/System/Text/Unicode/
+-rw-rw-rw-   0        0        0     1240 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Text/Unicode/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Text/__init__.py
+-rw-rw-rw-   0        0        0    77244 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Text/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.385470 abl-quantconnect-stubs-13987.4/System/Threading/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.390479 abl-quantconnect-stubs-13987.4/System/Threading/Tasks/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.395516 abl-quantconnect-stubs-13987.4/System/Threading/Tasks/Sources/
+-rw-rw-rw-   0        0        0     1273 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Threading/Tasks/Sources/__init__.py
+-rw-rw-rw-   0        0        0     6944 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Threading/Tasks/Sources/__init__.pyi
+-rw-rw-rw-   0        0        0     1249 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Threading/Tasks/__init__.py
+-rw-rw-rw-   0        0        0   233718 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Threading/Tasks/__init__.pyi
+-rw-rw-rw-   0        0        0     1231 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Threading/__init__.py
+-rw-rw-rw-   0        0        0   120535 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Threading/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.399526 abl-quantconnect-stubs-13987.4/System/Timers/
+-rw-rw-rw-   0        0        0     1222 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Timers/__init__.py
+-rw-rw-rw-   0        0        0     5957 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Timers/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.400525 abl-quantconnect-stubs-13987.4/System/Windows/
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.404526 abl-quantconnect-stubs-13987.4/System/Windows/Input/
+-rw-rw-rw-   0        0        0     1243 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Windows/Input/__init__.py
+-rw-rw-rw-   0        0        0     2418 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Windows/Input/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.407841 abl-quantconnect-stubs-13987.4/System/Windows/Markup/
+-rw-rw-rw-   0        0        0     1246 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Windows/Markup/__init__.py
+-rw-rw-rw-   0        0        0     1390 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Windows/Markup/__init__.pyi
+-rw-rw-rw-   0        0        0     1225 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/System/Windows/__init__.py
+-rw-rw-rw-   0        0        0     1201 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/System/__init__.py
+-rw-rw-rw-   0        0        0   901366 2023-06-21 04:49:48.000000 abl-quantconnect-stubs-13987.4/System/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.462846 abl-quantconnect-stubs-13987.4/abl_quantconnect_stubs.egg-info/
+-rw-rw-rw-   0        0        0     1316 2023-06-21 04:49:51.000000 abl-quantconnect-stubs-13987.4/abl_quantconnect_stubs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17362 2023-06-21 04:49:54.000000 abl-quantconnect-stubs-13987.4/abl_quantconnect_stubs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 04:49:51.000000 abl-quantconnect-stubs-13987.4/abl_quantconnect_stubs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-21 04:49:51.000000 abl-quantconnect-stubs-13987.4/abl_quantconnect_stubs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      119 2023-06-21 04:49:51.000000 abl-quantconnect-stubs-13987.4/abl_quantconnect_stubs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 04:49:55.464836 abl-quantconnect-stubs-13987.4/clr/
+-rw-rw-rw-   0        0        0      446 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/clr/__init__.pyi
+-rw-rw-rw-   0        0        0       42 2023-06-21 04:49:55.467832 abl-quantconnect-stubs-13987.4/setup.cfg
+-rw-rw-rw-   0        0        0    23104 2023-06-21 04:49:49.000000 abl-quantconnect-stubs-13987.4/setup.py
```

### Comparing `abl-quantconnect-stubs-13987.3/AlgorithmImports/__init__.pyi` & `abl-quantconnect-stubs-13987.4/AlgorithmImports/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Calculators/DataType/__init__.py` & `abl-quantconnect-stubs-13987.4/Calculators/DataType/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Calculators/DataType/__init__.pyi` & `abl-quantconnect-stubs-13987.4/Calculators/DataType/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Calculators/Estimators/__init__.py` & `abl-quantconnect-stubs-13987.4/Calculators/Estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Calculators/Estimators/__init__.pyi` & `abl-quantconnect-stubs-13987.4/Calculators/Estimators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Calculators/IO/__init__.py` & `abl-quantconnect-stubs-13987.4/Calculators/IO/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Calculators/IO/__init__.pyi` & `abl-quantconnect-stubs-13987.4/Calculators/IO/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Calculators/Margins/__init__.py` & `abl-quantconnect-stubs-13987.4/Calculators/Margins/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Calculators/Margins/__init__.pyi` & `abl-quantconnect-stubs-13987.4/Calculators/Margins/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Calculators/__init__.py` & `abl-quantconnect-stubs-13987.4/Calculators/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/Rest/Enums/__init__.py` & `abl-quantconnect-stubs-13987.4/FtxApi/Rest/Enums/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/Rest/Enums/__init__.pyi` & `abl-quantconnect-stubs-13987.4/FtxApi/Rest/Enums/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/LeveragedTokens/__init__.py` & `abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/LeveragedTokens/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/LeveragedTokens/__init__.pyi` & `abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/LeveragedTokens/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/Markets/__init__.py` & `abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/Markets/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/Markets/__init__.pyi` & `abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/Markets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/__init__.py` & `abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/Rest/Models/__init__.pyi` & `abl-quantconnect-stubs-13987.4/FtxApi/Rest/Models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/Rest/__init__.py` & `abl-quantconnect-stubs-13987.4/FtxApi/Rest/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/Rest/__init__.pyi` & `abl-quantconnect-stubs-13987.4/FtxApi/Rest/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/WebSocket/Models/__init__.py` & `abl-quantconnect-stubs-13987.4/FtxApi/WebSocket/Models/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/WebSocket/Models/__init__.pyi` & `abl-quantconnect-stubs-13987.4/FtxApi/WebSocket/Models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/WebSocket/__init__.py` & `abl-quantconnect-stubs-13987.4/FtxApi/WebSocket/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/WebSocket/__init__.pyi` & `abl-quantconnect-stubs-13987.4/FtxApi/WebSocket/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/WsEngine/__init__.py` & `abl-quantconnect-stubs-13987.4/FtxApi/WsEngine/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/WsEngine/__init__.pyi` & `abl-quantconnect-stubs-13987.4/FtxApi/WsEngine/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/__init__.py` & `abl-quantconnect-stubs-13987.4/FtxApi/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/FtxApi/__init__.pyi` & `abl-quantconnect-stubs-13987.4/FtxApi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Internal/Runtime/InteropServices/__init__.py` & `abl-quantconnect-stubs-13987.4/Internal/Runtime/InteropServices/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Internal/Runtime/InteropServices/__init__.pyi` & `abl-quantconnect-stubs-13987.4/Internal/Runtime/InteropServices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Internal/Runtime/__init__.py` & `abl-quantconnect-stubs-13987.4/Internal/Runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Internal/Win32/SafeHandles/__init__.py` & `abl-quantconnect-stubs-13987.4/Internal/Win32/SafeHandles/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Internal/Win32/__init__.py` & `abl-quantconnect-stubs-13987.4/Internal/Win32/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Internal/__init__.py` & `abl-quantconnect-stubs-13987.4/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Internal/__init__.pyi` & `abl-quantconnect-stubs-13987.4/Internal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MS/Internal/Xml/Linq/ComponentModel/__init__.py` & `abl-quantconnect-stubs-13987.4/MS/Internal/Xml/Linq/ComponentModel/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MS/Internal/Xml/Linq/__init__.py` & `abl-quantconnect-stubs-13987.4/MS/Internal/Xml/Linq/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MS/Internal/Xml/__init__.py` & `abl-quantconnect-stubs-13987.4/MS/Internal/Xml/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MS/Internal/__init__.py` & `abl-quantconnect-stubs-13987.4/MS/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MS/__init__.py` & `abl-quantconnect-stubs-13987.4/MS/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Microsoft/Win32/SafeHandles/__init__.py` & `abl-quantconnect-stubs-13987.4/Microsoft/Win32/SafeHandles/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Microsoft/Win32/SafeHandles/__init__.pyi` & `abl-quantconnect-stubs-13987.4/Microsoft/Win32/SafeHandles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Microsoft/Win32/__init__.py` & `abl-quantconnect-stubs-13987.4/Microsoft/Win32/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/Microsoft/__init__.py` & `abl-quantconnect-stubs-13987.4/Microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MomCrypto/Api/Algorithm/__init__.py` & `abl-quantconnect-stubs-13987.4/MomCrypto/Api/Algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MomCrypto/Api/Algorithm/__init__.pyi` & `abl-quantconnect-stubs-13987.4/MomCrypto/Api/Algorithm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MomCrypto/Api/__init__.py` & `abl-quantconnect-stubs-13987.4/MomCrypto/Api/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MomCrypto/Api/__init__.pyi` & `abl-quantconnect-stubs-13987.4/MomCrypto/Api/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MomCrypto/DataApi/__init__.py` & `abl-quantconnect-stubs-13987.4/MomCrypto/DataApi/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MomCrypto/DataApi/__init__.pyi` & `abl-quantconnect-stubs-13987.4/MomCrypto/DataApi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MomCrypto/Frontend/__init__.py` & `abl-quantconnect-stubs-13987.4/MomCrypto/Frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MomCrypto/Frontend/__init__.pyi` & `abl-quantconnect-stubs-13987.4/MomCrypto/Frontend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/MomCrypto/__init__.py` & `abl-quantconnect-stubs-13987.4/MomCrypto/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/PKG-INFO` & `abl-quantconnect-stubs-13987.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abl-quantconnect-stubs
-Version: 13987.3
+Version: 13987.4
 Summary: Type stubs for QuantConnect's Lean
 Home-page: https://github.com/QuantConnect/quantconnect-stubs-generator
 Author: QuantConnect
 Author-email: support@quantconnect.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/ABL/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/ABL/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/ABL/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/ABL/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/DataType/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/DataType/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/DataType/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/DataType/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/PricingModels/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/PricingModels/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/PricingModels/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/PricingModels/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/Strategies/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/Strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/Strategies/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/Strategies/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/LiveStrategy/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/LiveStrategy/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/AlgoTrade/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/AlgoTrade/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/AlgoTrade/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/AlgoTrade/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/tools/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/CSharp/qlnet/tools/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/CSharp/qlnet/tools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/Functions/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/Functions/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/Functions/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/Functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/Providers/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/Providers/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/Providers/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/Providers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Analysis/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Analysis/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Serialization/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/Serialization/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/Serialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Alphas/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Alphas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Execution/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Execution/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Execution/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Execution/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Portfolio/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Portfolio/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Portfolio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Risk/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Risk/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Risk/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Risk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Selection/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Selection/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/Selection/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/Selection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Framework/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Framework/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Selection/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Selection/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/Selection/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/Selection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Algorithm/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Algorithm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/Python/Wrappers/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/Python/Wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/Python/Wrappers/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/Python/Wrappers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/Python/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/Python/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/AlgorithmFactory/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/AlgorithmFactory/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Api/Serialization/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Api/Serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Api/Serialization/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Api/Serialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Api/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Api/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Api/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Api/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Benchmarks/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Benchmarks/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Benchmarks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Brokerages/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Brokerages/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Brokerages/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Brokerages/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Configuration/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Configuration/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Configuration/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Auxiliary/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Auxiliary/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Auxiliary/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Auxiliary/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Consolidators/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Consolidators/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Consolidators/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Consolidators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/AlphaStreams/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/AlphaStreams/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/AlphaStreams/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/AlphaStreams/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/IconicTypes/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/IconicTypes/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/IconicTypes/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/IconicTypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/Intrinio/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/Intrinio/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/Intrinio/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/Intrinio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/Tiingo/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/Tiingo/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/Tiingo/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/Tiingo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Custom/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Custom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Fundamental/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Fundamental/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Fundamental/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Fundamental/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Market/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Market/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Market/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Market/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Shortable/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Shortable/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/Shortable/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/Shortable/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/UniverseSelection/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/UniverseSelection/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/UniverseSelection/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/UniverseSelection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Data/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/DataSource/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/DataSource/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Exceptions/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Exceptions/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Exceptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Indicators/CandlestickPatterns/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Indicators/CandlestickPatterns/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Indicators/CandlestickPatterns/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Indicators/CandlestickPatterns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Indicators/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Indicators/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Indicators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Interfaces/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Interfaces/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Interfaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Alpha/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Alpha/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Alpha/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Alphas/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Alphas/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Alphas/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Alphas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Enumerators/Factories/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Enumerators/Factories/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Enumerators/Factories/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Enumerators/Factories/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Enumerators/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Enumerators/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Enumerators/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Enumerators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Queues/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Queues/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Queues/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Queues/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Transport/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Transport/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/Transport/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/Transport/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/WorkScheduling/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/WorkScheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/WorkScheduling/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/WorkScheduling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/DataFeeds/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/DataFeeds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/HistoricalData/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/HistoricalData/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/HistoricalData/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/HistoricalData/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/RealTime/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/RealTime/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/RealTime/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/RealTime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Results/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Results/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Results/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Results/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Server/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Server/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Server/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Server/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Setup/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Setup/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Setup/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Setup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Storage/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Storage/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/Storage/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/Storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/TransactionHandlers/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/TransactionHandlers/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/TransactionHandlers/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/TransactionHandlers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/Engine/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/Engine/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Lean/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Lean/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Logging/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Logging/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Logging/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Logging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Messaging/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Messaging/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Messaging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Notifications/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Notifications/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Notifications/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/Objectives/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/Objectives/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/Objectives/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/Objectives/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/Parameters/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/Parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/Parameters/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/Parameters/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Optimizer/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/OptionQuote/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/OptionQuote/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/OptionQuote/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/OptionQuote/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Fees/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Fees/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Fees/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Fees/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Fills/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Fills/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Fills/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Fills/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/OptionExercise/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/OptionExercise/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/OptionExercise/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/OptionExercise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Serialization/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Serialization/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Serialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Slippage/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Slippage/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/Slippage/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/Slippage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/TimeInForces/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/TimeInForces/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/TimeInForces/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/TimeInForces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Orders/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Orders/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Packets/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Packets/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Packets/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Packets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Parameters/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Parameters/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Parameters/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Python/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Python/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Python/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Python/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Queues/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Queues/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Queues/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Queues/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Report/ReportElements/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Report/ReportElements/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Report/ReportElements/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Report/ReportElements/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Report/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Report/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Report/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Report/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Scheduling/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Scheduling/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Scheduling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Cfd/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Cfd/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Cfd/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Cfd/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Crypto/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Crypto/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Crypto/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/CurrencyConversion/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/CurrencyConversion/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/CurrencyConversion/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/CurrencyConversion/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Equity/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Equity/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Equity/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Equity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Forex/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Forex/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Forex/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Forex/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Future/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Future/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Future/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Future/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/FutureOption/Api/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/FutureOption/Api/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/FutureOption/Api/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/FutureOption/Api/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/FutureOption/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/FutureOption/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/FutureOption/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/FutureOption/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Index/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Index/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Index/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Index/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/IndexOption/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/IndexOption/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/IndexOption/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/IndexOption/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Interfaces/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Interfaces/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Interfaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Option/StrategyMatcher/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Option/StrategyMatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Option/StrategyMatcher/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Option/StrategyMatcher/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Option/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Option/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Option/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Option/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Positions/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Positions/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Positions/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Positions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Volatility/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Volatility/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/Volatility/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/Volatility/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Securities/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Securities/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Statistics/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Statistics/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Statistics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Storage/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Storage/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Storage/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Util/RateLimit/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Util/RateLimit/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Util/RateLimit/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Util/RateLimit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Util/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/Util/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/Util/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/Util/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnect/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnect/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Model/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Model/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Model/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Parser/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Parser/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Parser/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Parser/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Renderer/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Renderer/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Renderer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/Model/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/Model/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/Model/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/Model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/Utility/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/Utility/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/Utility/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/Utility/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Tests/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Tests/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Utility/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Utility/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/Utility/__init__.pyi` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/Utility/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/QuantConnectStubsGenerator/__init__.py` & `abl-quantconnect-stubs-13987.4/QuantConnectStubsGenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Buffers/Binary/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Buffers/Binary/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Buffers/Binary/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Buffers/Binary/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Buffers/Text/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Buffers/Text/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Buffers/Text/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Buffers/Text/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Buffers/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Buffers/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Buffers/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Buffers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/CodeDom/Compiler/__init__.py` & `abl-quantconnect-stubs-13987.4/System/CodeDom/Compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/CodeDom/Compiler/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/CodeDom/Compiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/CodeDom/__init__.py` & `abl-quantconnect-stubs-13987.4/System/CodeDom/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/Concurrent/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Collections/Concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/Concurrent/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Collections/Concurrent/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/Generic/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Collections/Generic/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/Generic/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Collections/Generic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/Immutable/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Collections/Immutable/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/Immutable/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Collections/Immutable/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/ObjectModel/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Collections/ObjectModel/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/ObjectModel/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Collections/ObjectModel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/Specialized/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Collections/Specialized/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/Specialized/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Collections/Specialized/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Collections/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Collections/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Collections/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/ComponentModel/DataAnnotations/Schema/__init__.py` & `abl-quantconnect-stubs-13987.4/System/ComponentModel/DataAnnotations/Schema/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/ComponentModel/DataAnnotations/Schema/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/ComponentModel/DataAnnotations/Schema/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/ComponentModel/DataAnnotations/__init__.py` & `abl-quantconnect-stubs-13987.4/System/ComponentModel/DataAnnotations/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/ComponentModel/DataAnnotations/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/ComponentModel/DataAnnotations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/ComponentModel/Design/Serialization/__init__.py` & `abl-quantconnect-stubs-13987.4/System/ComponentModel/Design/Serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/ComponentModel/Design/Serialization/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/ComponentModel/Design/Serialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/ComponentModel/Design/__init__.py` & `abl-quantconnect-stubs-13987.4/System/ComponentModel/Design/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/ComponentModel/Design/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/ComponentModel/Design/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/ComponentModel/__init__.py` & `abl-quantconnect-stubs-13987.4/System/ComponentModel/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/ComponentModel/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/ComponentModel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Configuration/Assemblies/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Configuration/Assemblies/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Configuration/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Diagnostics/CodeAnalysis/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Diagnostics/CodeAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Diagnostics/CodeAnalysis/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Diagnostics/CodeAnalysis/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Diagnostics/Contracts/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Diagnostics/Contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Diagnostics/Contracts/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Diagnostics/Contracts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Diagnostics/SymbolStore/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Diagnostics/SymbolStore/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Diagnostics/Tracing/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Diagnostics/Tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Diagnostics/Tracing/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Diagnostics/Tracing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Diagnostics/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Diagnostics/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Diagnostics/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Diagnostics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Drawing/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Drawing/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Drawing/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Drawing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Globalization/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Globalization/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Globalization/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Globalization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/IO/Enumeration/__init__.py` & `abl-quantconnect-stubs-13987.4/System/IO/Enumeration/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/IO/Enumeration/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/IO/Enumeration/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/IO/Strategies/__init__.py` & `abl-quantconnect-stubs-13987.4/System/IO/Strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/IO/__init__.py` & `abl-quantconnect-stubs-13987.4/System/IO/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/IO/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/IO/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Linq/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Linq/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Linq/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Linq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Net/Cache/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Net/Cache/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Net/Cache/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Net/Cache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Net/NetworkInformation/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Net/NetworkInformation/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Net/NetworkInformation/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Net/NetworkInformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Net/Security/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Net/Security/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Net/Security/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Net/Security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Net/Sockets/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Net/Sockets/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Net/Sockets/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Net/Sockets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Net/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Net/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Net/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Net/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Numerics/Hashing/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Numerics/Hashing/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Numerics/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Numerics/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Numerics/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Numerics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Reflection/Emit/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Reflection/Emit/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Reflection/Emit/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Reflection/Emit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Reflection/Metadata/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Reflection/Metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Reflection/Metadata/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Reflection/Metadata/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Reflection/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Reflection/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Reflection/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Reflection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Resources/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Resources/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Resources/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Resources/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/CompilerServices/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/CompilerServices/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/CompilerServices/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/CompilerServices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/ConstrainedExecution/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/ConstrainedExecution/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/ConstrainedExecution/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/ConstrainedExecution/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/ExceptionServices/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/ExceptionServices/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/ExceptionServices/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/ExceptionServices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/ComTypes/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/ComTypes/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/ComTypes/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/ComTypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/Marshalling/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/Marshalling/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/Marshalling/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/Marshalling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/ObjectiveC/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/ObjectiveC/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/ObjectiveC/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/ObjectiveC/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/InteropServices/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/InteropServices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/Arm/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/Arm/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/Arm/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/Arm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/X86/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/X86/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/X86/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/X86/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Intrinsics/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/Intrinsics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Loader/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/Loader/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Loader/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/Loader/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Remoting/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/Remoting/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Serialization/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/Serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Serialization/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/Serialization/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Versioning/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/Versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/Versioning/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/Versioning/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Runtime/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/Authentication/ExtendedProtection/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Security/Authentication/ExtendedProtection/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/Authentication/ExtendedProtection/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Security/Authentication/ExtendedProtection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/Authentication/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Security/Authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/Authentication/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Security/Authentication/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/Cryptography/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Security/Cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/Cryptography/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Security/Cryptography/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/Permissions/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Security/Permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/Permissions/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Security/Permissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/Principal/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Security/Principal/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/Principal/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Security/Principal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Security/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Security/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Text/RegularExpressions/Symbolic/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Text/RegularExpressions/Symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Text/RegularExpressions/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Text/RegularExpressions/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Text/RegularExpressions/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Text/RegularExpressions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Text/Unicode/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Text/Unicode/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Text/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Text/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Text/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Text/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Threading/Tasks/Sources/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Threading/Tasks/Sources/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Threading/Tasks/Sources/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Threading/Tasks/Sources/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Threading/Tasks/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Threading/Tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Threading/Tasks/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Threading/Tasks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Threading/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Threading/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Threading/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Threading/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Timers/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Timers/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Timers/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Timers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Windows/Input/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Windows/Input/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Windows/Input/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Windows/Input/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Windows/Markup/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Windows/Markup/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Windows/Markup/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/Windows/Markup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/Windows/__init__.py` & `abl-quantconnect-stubs-13987.4/System/Windows/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/__init__.py` & `abl-quantconnect-stubs-13987.4/System/__init__.py`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/System/__init__.pyi` & `abl-quantconnect-stubs-13987.4/System/__init__.pyi`

 * *Files identical despite different names*

### Comparing `abl-quantconnect-stubs-13987.3/abl_quantconnect_stubs.egg-info/PKG-INFO` & `abl-quantconnect-stubs-13987.4/abl_quantconnect_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abl-quantconnect-stubs
-Version: 13987.3
+Version: 13987.4
 Summary: Type stubs for QuantConnect's Lean
 Home-page: https://github.com/QuantConnect/quantconnect-stubs-generator
 Author: QuantConnect
 Author-email: support@quantconnect.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `abl-quantconnect-stubs-13987.3/abl_quantconnect_stubs.egg-info/SOURCES.txt` & `abl-quantconnect-stubs-13987.4/abl_quantconnect_stubs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,16 @@
 QuantConnect/Python/__init__.pyi
 QuantConnect/Queues/__init__.py
 QuantConnect/Queues/__init__.pyi
 QuantConnect/Report/__init__.py
 QuantConnect/Report/__init__.pyi
 QuantConnect/Report/ReportElements/__init__.py
 QuantConnect/Report/ReportElements/__init__.pyi
+QuantConnect/Research/__init__.py
+QuantConnect/Research/__init__.pyi
 QuantConnect/Scheduling/__init__.py
 QuantConnect/Scheduling/__init__.pyi
 QuantConnect/Securities/__init__.py
 QuantConnect/Securities/__init__.pyi
 QuantConnect/Securities/Cfd/__init__.py
 QuantConnect/Securities/Cfd/__init__.pyi
 QuantConnect/Securities/Crypto/__init__.py
```

### Comparing `abl-quantconnect-stubs-13987.3/setup.py` & `abl-quantconnect-stubs-13987.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ```
 
 This line imports [all common QuantConnect members](https://github.com/QuantConnect/Lean/blob/master/Common/AlgorithmImports.py) and provides autocomplete for them.
 """.strip()
 
 setup(
     name="abl-quantconnect-stubs",
-    version="13987.3",
+    version="13987.4",
     description="Type stubs for QuantConnect's Lean",
     author="QuantConnect",
     author_email="support@quantconnect.com",
     url="https://github.com/QuantConnect/quantconnect-stubs-generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
@@ -147,14 +147,15 @@
         "QuantConnect.Orders.TimeInForces",
         "QuantConnect.Packets",
         "QuantConnect.Parameters",
         "QuantConnect.Python",
         "QuantConnect.Queues",
         "QuantConnect.Report",
         "QuantConnect.Report.ReportElements",
+        "QuantConnect.Research",
         "QuantConnect.Scheduling",
         "QuantConnect.Securities",
         "QuantConnect.Securities.Cfd",
         "QuantConnect.Securities.Crypto",
         "QuantConnect.Securities.CurrencyConversion",
         "QuantConnect.Securities.Equity",
         "QuantConnect.Securities.Forex",
@@ -369,14 +370,15 @@
         "QuantConnect.Orders.TimeInForces": ["*.py", "*.pyi"],
         "QuantConnect.Packets": ["*.py", "*.pyi"],
         "QuantConnect.Parameters": ["*.py", "*.pyi"],
         "QuantConnect.Python": ["*.py", "*.pyi"],
         "QuantConnect.Queues": ["*.py", "*.pyi"],
         "QuantConnect.Report": ["*.py", "*.pyi"],
         "QuantConnect.Report.ReportElements": ["*.py", "*.pyi"],
+        "QuantConnect.Research": ["*.py", "*.pyi"],
         "QuantConnect.Scheduling": ["*.py", "*.pyi"],
         "QuantConnect.Securities": ["*.py", "*.pyi"],
         "QuantConnect.Securities.Cfd": ["*.py", "*.pyi"],
         "QuantConnect.Securities.Crypto": ["*.py", "*.pyi"],
         "QuantConnect.Securities.CurrencyConversion": ["*.py", "*.pyi"],
         "QuantConnect.Securities.Equity": ["*.py", "*.pyi"],
         "QuantConnect.Securities.Forex": ["*.py", "*.pyi"],
```

