# Comparing `tmp/kadaster_kikinzage_client-0.1.6.tar.gz` & `tmp/kadaster_kikinzage_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kadaster_kikinzage_client-0.1.6.tar", max compression
+gzip compressed data, was "kadaster_kikinzage_client-0.2.0.tar", max compression
```

## Comparing `kadaster_kikinzage_client-0.1.6.tar` & `kadaster_kikinzage_client-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1071 2023-06-20 12:16:47.768472 kadaster_kikinzage_client-0.1.6/LICENSE
--rw-r--r--   0        0        0     4027 2023-06-20 12:16:47.768472 kadaster_kikinzage_client-0.1.6/README.md
--rw-r--r--   0        0        0     2113 2023-06-20 12:17:02.372542 kadaster_kikinzage_client-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       45 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/__init__.py
--rw-r--r--   0        0        0     2274 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/__main__.py
--rw-r--r--   0        0        0      302 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/__init__.py
--rw-r--r--   0        0        0    13244 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/asyncio.py
--rw-r--r--   0        0        0    16611 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/base.py
--rw-r--r--   0        0        0    12666 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/default.py
--rw-r--r--   0        0        0      610 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/errors.py
--rw-r--r--   0        0        0      188 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/client/utils.py
--rw-r--r--   0        0        0      401 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/__init__.py
--rw-r--r--   0        0        0     2927 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/adres.py
--rw-r--r--   0        0        0    11899 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/collectie.py
--rw-r--r--   0        0        0     5786 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/eigendomsinformatie.py
--rw-r--r--   0        0        0     1445 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/enum.py
--rw-r--r--   0        0        0     8739 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/generated.py
--rw-r--r--   0        0        0      613 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/misc.py
--rw-r--r--   0        0        0     3452 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/persoon.py
--rw-r--r--   0        0        0     4030 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/product.py
--rw-r--r--   0        0        0     2361 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/stukken.py
--rw-r--r--   0        0        0     1195 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/models/zekerheid.py
--rw-r--r--   0        0        0        0 2023-06-20 12:16:47.772472 kadaster_kikinzage_client-0.1.6/src/kikinzage/py.typed
--rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4027 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/README.md
+-rw-r--r--   0        0        0     2113 2023-06-21 12:26:27.652500 kadaster_kikinzage_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/__init__.py
+-rw-r--r--   0        0        0     2274 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/__main__.py
+-rw-r--r--   0        0        0      302 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/__init__.py
+-rw-r--r--   0        0        0    19206 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/asyncio.py
+-rw-r--r--   0        0        0    22661 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/base.py
+-rw-r--r--   0        0        0    18556 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/default.py
+-rw-r--r--   0        0        0      610 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/errors.py
+-rw-r--r--   0        0        0      188 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/client/utils.py
+-rw-r--r--   0        0        0      401 2023-06-21 12:26:13.604369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/__init__.py
+-rw-r--r--   0        0        0     2927 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/adres.py
+-rw-r--r--   0        0        0    11899 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/collectie.py
+-rw-r--r--   0        0        0     5786 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/eigendomsinformatie.py
+-rw-r--r--   0        0        0     1445 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/enum.py
+-rw-r--r--   0        0        0     8739 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/generated.py
+-rw-r--r--   0        0        0      613 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/misc.py
+-rw-r--r--   0        0        0     3452 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/persoon.py
+-rw-r--r--   0        0        0     4030 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/product.py
+-rw-r--r--   0        0        0     2361 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/stukken.py
+-rw-r--r--   0        0        0     1195 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/models/zekerheid.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:26:13.608369 kadaster_kikinzage_client-0.2.0/src/kikinzage/py.typed
+-rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.2.0/PKG-INFO
```

### Comparing `kadaster_kikinzage_client-0.1.6/LICENSE` & `kadaster_kikinzage_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/README.md` & `kadaster_kikinzage_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/pyproject.toml` & `kadaster_kikinzage_client-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kadaster-kikinzage-client"
-version = "0.1.6"
+version = "0.2.0"
 description = " Kadaster - KIK Inzage API Python client"
 authors = ["Jelmer Draaijer <info@jelmert.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 repository = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 documentation = "https://kadaster-kik-inzage-api-python-client.readthedocs.io"
```

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/__main__.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/__main__.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/client/asyncio.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/client/asyncio.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from types import TracebackType
 from typing import Any
 from typing import Optional
 from typing import Type
 from typing import Union
 
 import httpx
@@ -322,7 +323,155 @@
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
         return await self.send(request, models.ObjectlijstPersoon)
+
+    async def brondocument(
+        self,
+        soort_register: str,
+        register_code: str,
+        deel: str,
+        nummer: str,
+        *,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.Brondocument:
+        request = self.request_brondocument(
+            soort_register=soort_register,
+            register_code=register_code,
+            deel=deel,
+            nummer=nummer,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return await self.send(request, models.Brondocument)
+
+    async def kadastralekaart_kadastraalobjectidentificatie(
+        self,
+        kadastraalobjectidentificatie: str,
+        formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.KadastraleKaart:
+        request = self.request_kadastralekaart_kadastraalobjectidentificatie(
+            kadastraalobjectidentificatie=kadastraalobjectidentificatie,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return await self.send(request, models.KadastraleKaart)
+
+    async def kadastralekaart_kadastraleaanduiding(
+        self,
+        kadastralegemeente: str,
+        sectie: str,
+        perceelnummer: int,
+        appartementsrecht_volgnummer: Optional[int] = None,
+        formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.KadastraleKaart:
+        request = self.request_kadastralekaart_kadastraleaanduiding(
+            kadastralegemeente=kadastralegemeente,
+            sectie=sectie,
+            perceelnummer=perceelnummer,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
+            appartementsrecht_volgnummer=appartementsrecht_volgnummer,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return await self.send(request, models.KadastraleKaart)
+
+    async def kadastralekaart_postcode(
+        self,
+        postcode: str,
+        huisnummer: int,
+        huisletter: Optional[str] = None,
+        huisnummertoevoeging: Optional[str] = None,
+        *,
+        formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.KadastraleKaart:
+        request = self.request_kadastralekaart_postcode(
+            postcode=postcode,
+            huisnummer=huisnummer,
+            huisletter=huisletter,
+            huisnummertoevoeging=huisnummertoevoeging,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return await self.send(request, models.KadastraleKaart)
+
+    async def datuminformatie(
+        self,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        *,
+        gebruikeridentificatie: Optional[str] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.Datuminformatie:
+        request = self.request_datuminformatie(
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return await self.send(request, models.Datuminformatie)
+
+    async def kadastraalpersoonidentificatie_persoonsgegevens(
+        self,
+        geslachtsnaam: str,
+        voornamen: str,
+        geboortedatum: datetime.date,
+        voorvoegselsgeslachtsnaam: Optional[str] = None,
+        *,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.KadastraalPersoonIdentificatie:
+        request = self.request_kadastraalpersoonidentificatie_persoonsgegevens(
+            geslachtsnaam=geslachtsnaam,
+            voornamen=voornamen,
+            geboortedatum=geboortedatum,
+            voorvoegselsgeslachtsnaam=voorvoegselsgeslachtsnaam,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return await self.send(request, models.KadastraalPersoonIdentificatie)
```

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/client/base.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/client/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from abc import ABC
 from json import JSONDecodeError
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Type
 from typing import Union
@@ -61,22 +62,26 @@
         self.client = self.create_client(**httpx_kwargs)
 
     def create_client(self, **httpx_kwargs: Any) -> BaseClient:
         raise NotImplementedError
 
     def _create_params(
         self,
-        formaat: Union[Formaat, UseClientDefault],
+        *,
         klantreferentie: Union[str, UseClientDefault],
+        formaat: Optional[Union[Formaat, UseClientDefault]] = None,
         **optionals: Any,
     ) -> Dict[str, Any]:
-        params: Dict[str, Any] = {
-            "formaat": self._get_formaat(formaat),
-            "klantreferentie": self._get_klantreferentie(klantreferentie),
-        }
+        params: Dict[str, Any] = {}
+
+        if formaat:
+            params["formaat"] = self._get_formaat(formaat)
+
+        params["klantreferentie"] = self._get_klantreferentie(klantreferentie)
+
         params.update(remove_optional_params(**optionals))
 
         return params
 
     def process_response(
         self,
         response: httpx.Response,
@@ -141,16 +146,16 @@
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
     ) -> Request:
         params = self._create_params(
-            formaat,
-            klantreferentie,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
             appartementsrechtVolgnummer=appartementsrecht_volgnummer,
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
@@ -171,16 +176,16 @@
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
     ) -> Request:
         """GET /eigendomsinformatie/kadastraalobjectidentificatie/{kadastraalobjectidentificatie}"""
         params = self._create_params(
-            formaat,
-            klantreferentie,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
         request = self.client.build_request(
@@ -203,16 +208,16 @@
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
     ) -> Request:
         """GET /eigendomsinformatie/postcode/{postcode}/{huisnummer}"""
         params = self._create_params(
-            formaat,
-            klantreferentie,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
             huisletter=huisletter,
             huisnummertoevoeging=huisnummertoevoeging,
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
@@ -235,16 +240,16 @@
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
     ) -> Request:
         params = self._create_params(
-            formaat,
-            klantreferentie,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
             huisletter=huisletter,
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
@@ -262,16 +267,16 @@
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
     ) -> Request:
         params = self._create_params(
-            formaat,
-            klantreferentie,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
         return self.client.build_request(
@@ -291,16 +296,16 @@
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
     ) -> Request:
         params = self._create_params(
-            formaat,
-            klantreferentie,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
             appartementsrechtVolgnummer=appartementsrecht_volgnummer,
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
@@ -321,16 +326,16 @@
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
     ) -> Request:
         params = self._create_params(
-            formaat,
-            klantreferentie,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
             huisletter=huisletter,
             huisnummertoevoeging=huisnummertoevoeging,
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
@@ -349,16 +354,16 @@
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
     ) -> Request:
         params = self._create_params(
-            formaat,
-            klantreferentie,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
         return self.client.build_request(
@@ -374,25 +379,21 @@
         formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
     ) -> Request:
-        params: Dict[str, Any] = {
-            "formaat": self._get_formaat(formaat),
-            "klantreferentie": self._get_klantreferentie(klantreferentie),
-        }
-        params.update(
-            remove_optional_params(
-                gebruikeridentificatie=gebruikeridentificatie,
-                hyperlinkopproduct=hyperlinkopproduct,
-                inkoopnummer=inkoopnummer,
-                referentienummer=referentienummer,
-            )
+        params = self._create_params(
+            formaat=formaat,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
         )
 
         return self.client.build_request(
             method="GET",
             url=f"eigenaarsinformatie/burgerservicenummer/{burgerservicenummer}",
             params=params,
         )
@@ -405,16 +406,16 @@
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
     ) -> Request:
         params = self._create_params(
-            formaat,
-            klantreferentie,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
         return self.client.build_request(
@@ -430,25 +431,187 @@
         formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
         inkoopnummer: Optional[str] = None,
         referentienummer: Optional[str] = None,
     ) -> Request:
-        params: Dict[str, Any] = {
-            "formaat": self._get_formaat(formaat),
-            "klantreferentie": self._get_klantreferentie(klantreferentie),
-        }
-        params.update(
-            remove_optional_params(
-                gebruikeridentificatie=gebruikeridentificatie,
-                hyperlinkopproduct=hyperlinkopproduct,
-                inkoopnummer=inkoopnummer,
-                referentienummer=referentienummer,
-            )
+        params = self._create_params(
+            formaat=formaat,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
         )
 
         return self.client.build_request(
             method="GET",
             url=f"objectlijstpersoon/burgerservicenummer/{burgerservicenummer}",
             params=params,
         )
+
+    def request_brondocument(
+        self,
+        soort_register: str,
+        register_code: str,
+        deel: str,
+        nummer: str,
+        *,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> Request:
+        params = self._create_params(
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return self.client.build_request(
+            method="GET",
+            url=f"brondocument/deelennummer/{soort_register}/{register_code}/{deel}/{nummer}",
+            params=params,
+        )
+
+    def request_kadastralekaart_kadastraalobjectidentificatie(
+        self,
+        kadastraalobjectidentificatie: str,
+        *,
+        formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> Request:
+        params = self._create_params(
+            formaat=formaat,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        request = self.client.build_request(
+            method="GET",
+            url=f"kadastralekaart/kadastraalobjectidentificatie/{kadastraalobjectidentificatie}",
+            params=params,
+        )
+
+        return request
+
+    def request_kadastralekaart_kadastraleaanduiding(
+        self,
+        kadastralegemeente: str,
+        sectie: str,
+        perceelnummer: int,
+        appartementsrecht_volgnummer: Optional[int] = None,
+        *,
+        formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> Request:
+        params = self._create_params(
+            formaat=formaat,
+            klantreferentie=klantreferentie,
+            appartementsrechtVolgnummer=appartementsrecht_volgnummer,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        request = self.client.build_request(
+            method="GET",
+            url=f"/kadastralekaart/kadastraleaanduiding/{kadastralegemeente}/{sectie}/{perceelnummer}",
+            params=params,
+        )
+
+        return request
+
+    def request_kadastralekaart_postcode(
+        self,
+        postcode: str,
+        huisnummer: int,
+        huisletter: Optional[str] = None,
+        huisnummertoevoeging: Optional[str] = None,
+        *,
+        formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> Request:
+        params = self._create_params(
+            formaat=formaat,
+            klantreferentie=klantreferentie,
+            huisletter=huisletter,
+            huisnummertoevoeging=huisnummertoevoeging,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        request = self.client.build_request(
+            method="GET",
+            url=f"kadastralekaart/postcode/{postcode}/{huisnummer}",
+            params=params,
+        )
+        return request
+
+    def request_datuminformatie(
+        self,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        *,
+        gebruikeridentificatie: Optional[str] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> Request:
+        params = self._create_params(
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return self.client.build_request(
+            method="GET",
+            url="datuminformatie",
+            params=params,
+        )
+
+    def request_kadastraalpersoonidentificatie_persoonsgegevens(
+        self,
+        geslachtsnaam: str,
+        voornamen: str,
+        geboortedatum: datetime.date,
+        voorvoegselsgeslachtsnaam: Optional[str] = None,
+        *,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> Request:
+        params = self._create_params(
+            voorvoegselsgeslachtsnaam=voorvoegselsgeslachtsnaam,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return self.client.build_request(
+            method="GET",
+            url=f"kadastraalpersoonidentificatie/persoonsgegevens/{geslachtsnaam}/{voornamen}/{geboortedatum.isoformat()}",
+            params=params,
+        )
```

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/client/default.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/client/default.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from typing import Any
 from typing import Optional
 from typing import Type
 from typing import Union
 
 import httpx
 from httpx._client import USE_CLIENT_DEFAULT
@@ -309,7 +310,155 @@
             gebruikeridentificatie=gebruikeridentificatie,
             hyperlinkopproduct=hyperlinkopproduct,
             inkoopnummer=inkoopnummer,
             referentienummer=referentienummer,
         )
 
         return self.send(request, models.ObjectlijstPersoon)
+
+    def brondocument(
+        self,
+        soort_register: str,
+        register_code: str,
+        deel: str,
+        nummer: str,
+        *,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.Brondocument:
+        request = self.request_brondocument(
+            soort_register=soort_register,
+            register_code=register_code,
+            deel=deel,
+            nummer=nummer,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return self.send(request, models.Brondocument)
+
+    def kadastralekaart_kadastraalobjectidentificatie(
+        self,
+        kadastraalobjectidentificatie: str,
+        formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.KadastraleKaart:
+        request = self.request_kadastralekaart_kadastraalobjectidentificatie(
+            kadastraalobjectidentificatie=kadastraalobjectidentificatie,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return self.send(request, models.KadastraleKaart)
+
+    def kadastralekaart_kadastraleaanduiding(
+        self,
+        kadastralegemeente: str,
+        sectie: str,
+        perceelnummer: int,
+        appartementsrecht_volgnummer: Optional[int] = None,
+        formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.KadastraleKaart:
+        request = self.request_kadastralekaart_kadastraleaanduiding(
+            kadastralegemeente=kadastralegemeente,
+            sectie=sectie,
+            perceelnummer=perceelnummer,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
+            appartementsrecht_volgnummer=appartementsrecht_volgnummer,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return self.send(request, models.KadastraleKaart)
+
+    def kadastralekaart_postcode(
+        self,
+        postcode: str,
+        huisnummer: int,
+        huisletter: Optional[str] = None,
+        huisnummertoevoeging: Optional[str] = None,
+        *,
+        formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        hyperlinkopproduct: Optional[bool] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.KadastraleKaart:
+        request = self.request_kadastralekaart_postcode(
+            postcode=postcode,
+            huisnummer=huisnummer,
+            huisletter=huisletter,
+            huisnummertoevoeging=huisnummertoevoeging,
+            formaat=formaat,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            hyperlinkopproduct=hyperlinkopproduct,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return self.send(request, models.KadastraleKaart)
+
+    def datuminformatie(
+        self,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        *,
+        gebruikeridentificatie: Optional[str] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.Datuminformatie:
+        request = self.request_datuminformatie(
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return self.send(request, models.Datuminformatie)
+
+    def kadastraalpersoonidentificatie_persoonsgegevens(
+        self,
+        geslachtsnaam: str,
+        voornamen: str,
+        geboortedatum: datetime.date,
+        voorvoegselsgeslachtsnaam: Optional[str] = None,
+        *,
+        klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
+        gebruikeridentificatie: Optional[str] = None,
+        inkoopnummer: Optional[str] = None,
+        referentienummer: Optional[str] = None,
+    ) -> models.KadastraalPersoonIdentificatie:
+        request = self.request_kadastraalpersoonidentificatie_persoonsgegevens(
+            geslachtsnaam=geslachtsnaam,
+            voornamen=voornamen,
+            geboortedatum=geboortedatum,
+            voorvoegselsgeslachtsnaam=voorvoegselsgeslachtsnaam,
+            klantreferentie=klantreferentie,
+            gebruikeridentificatie=gebruikeridentificatie,
+            inkoopnummer=inkoopnummer,
+            referentienummer=referentienummer,
+        )
+
+        return self.send(request, models.KadastraalPersoonIdentificatie)
```

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/client/errors.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/client/errors.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/adres.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/adres.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/collectie.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/collectie.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/eigendomsinformatie.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/eigendomsinformatie.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/enum.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/enum.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/generated.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/generated.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/misc.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/misc.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/persoon.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/persoon.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/product.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/product.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/stukken.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/stukken.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/src/kikinzage/models/zekerheid.py` & `kadaster_kikinzage_client-0.2.0/src/kikinzage/models/zekerheid.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.6/PKG-INFO` & `kadaster_kikinzage_client-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kadaster-kikinzage-client
-Version: 0.1.6
+Version: 0.2.0
 Summary:  Kadaster - KIK Inzage API Python client
 Home-page: https://github.com/foarsitter/kadaster-kik-inzage-api-python-client
 License: MIT
 Author: Jelmer Draaijer
 Author-email: info@jelmert.nl
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
```

