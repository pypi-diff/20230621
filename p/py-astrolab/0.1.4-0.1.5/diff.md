# Comparing `tmp/py_astrolab-0.1.4.tar.gz` & `tmp/py_astrolab-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.1.4.tar", max compression
+gzip compressed data, was "py_astrolab-0.1.5.tar", max compression
```

## Comparing `py_astrolab-0.1.4.tar` & `py_astrolab-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.1.4/README.md
--rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.1.4/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    14779 2023-06-17 10:10:20.260982 py_astrolab-0.1.4/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.1.4/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    70111 2023-06-17 10:10:20.247410 py_astrolab-0.1.4/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.1.4/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.1.4/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.1.4/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-05-29 18:14:56.449179 py_astrolab-0.1.4/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    25286 2023-06-17 10:10:20.258711 py_astrolab-0.1.4/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.1.4/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.1.4/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2356 2023-06-17 10:10:20.255187 py_astrolab-0.1.4/py_astrolab/report.py
--rwxr-xr-x   0        0        0     5061 2023-05-31 21:03:53.211311 py_astrolab-0.1.4/py_astrolab/types.py
--rwxr-xr-x   0        0        0     5952 2023-06-17 10:10:20.255187 py_astrolab-0.1.4/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      689 2023-06-17 11:22:53.914368 py_astrolab-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.1.5/README.md
+-rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.1.5/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    16850 2023-06-21 20:38:42.474113 py_astrolab-0.1.5/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.1.5/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    70111 2023-06-17 10:10:20.247410 py_astrolab-0.1.5/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.1.5/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.1.5/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.1.5/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-05-29 18:14:56.449179 py_astrolab-0.1.5/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    26385 2023-06-21 20:10:47.767169 py_astrolab-0.1.5/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.1.5/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.1.5/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2356 2023-06-17 10:10:20.255187 py_astrolab-0.1.5/py_astrolab/report.py
+-rwxr-xr-x   0        0        0     5061 2023-05-31 21:03:53.211311 py_astrolab-0.1.5/py_astrolab/types.py
+-rwxr-xr-x   0        0        0     5952 2023-06-17 10:10:20.255187 py_astrolab-0.1.5/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      689 2023-06-21 20:48:27.158466 py_astrolab-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.1.5/PKG-INFO
```

### Comparing `py_astrolab-0.1.4/py_astrolab/__init__.py` & `py_astrolab-0.1.5/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.4/py_astrolab/aspects.py` & `py_astrolab-0.1.5/py_astrolab/aspects.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,14 +204,33 @@
                              "p1": self.p_id_decoder(point_list[first]['name']),
                              "p2": self.p_id_decoder(point_list[second]['name'],)
                              }
                     self.all_aspects_list.append(d_asp)
 
         return self.all_aspects_list
 
+    def is_fake_aspect(self, aspect: dict) -> bool:
+        is_fake_aspect = False
+        user = json.loads(self.user.json())
+        p1_name = aspect['p1_name'].lower().replace(' ', '_')
+        p2_name = aspect['p2_name'].lower().replace(' ', '_')
+        if user[p1_name]['element'] == user[p2_name]['element'] and aspect['aspect'] == 'square':
+            is_fake_aspect = True
+        if aspect['aspect'] in {'trine', 'conjunction'}:
+            if user[p1_name]['element'] != user[p2_name]['element']:
+                if aspect['orbit'] > 3:
+                    is_fake_aspect = True
+        elif aspect['aspect'] == 'opposition':
+            p1_sign = user[p1_name]['sign']
+            p2_sign = user[p2_name]['sign']
+            p1_sign_opposite = self.user.signs_dict[p1_sign]['opposite']
+            if not p1_sign_opposite.startswith(p2_sign):
+                is_fake_aspect = True
+        return is_fake_aspect
+
     def get_relevant_aspects(self):
         """ 
         Filters the aspects list with the desired points, in this case
         the most important are hardcoded.
         Set the list with set_points and creating a list with the names
         or the numbers of the houses.
         """
@@ -240,14 +259,17 @@
             if name_p1 in axes_list:
                 if abs(a['orbit']) >= self.axes_orbit_settings:
                     aspects_list_subtract.append(a)
 
             elif name_p2 in axes_list:
                 if abs(a['orbit']) >= self.axes_orbit_settings:
                     aspects_list_subtract.append(a)
+            
+            if self.is_fake_aspect(a):
+                aspects_list_subtract.append(a)
 
         self.aspects = [
             item for item in aspects_filtered if item not in aspects_list_subtract]
 
         return self.aspects
 
 
@@ -270,14 +292,34 @@
             self.second_user.__get_all()
 
         self.first_init_point_list = self.first_user.planets_list + \
             self.first_user.houses_list + self.first_user.axis_list
         self.second_init_point_list = self.second_user.planets_list + \
             self.second_user.houses_list + self.second_user.axis_list
 
+    def is_fake_aspect(self, aspect: dict) -> bool:
+        is_fake_aspect = False
+        user_1 = json.loads(self.first_user.json())
+        user_2 = json.loads(self.second_user.json())
+        p1_name = aspect['p1_name'].lower().replace(' ', '_')
+        p2_name = aspect['p2_name'].lower().replace(' ', '_')
+        if user_1[p1_name]['element'] == user_2[p2_name]['element'] and aspect['aspect'] == 'square':
+            is_fake_aspect = True
+        if aspect['aspect'] in {'trine', 'conjunction'}:
+            if user_1[p1_name]['element'] != user_2[p2_name]['element']:
+                if aspect['orbit'] > 3:
+                    is_fake_aspect = True
+        elif aspect['aspect'] == 'opposition':
+            p1_sign = user_1[p1_name]['sign']
+            p2_sign = user_2[p2_name]['sign']
+            p1_sign_opposite = self.first_user.signs_dict[p1_sign]['opposite']
+            if not p1_sign_opposite.startswith(p2_sign):
+                is_fake_aspect = True
+        return is_fake_aspect
+
     def get_all_aspects(self):
         """
         Return all the aspects of the points in the natal chart in a dictionary,
         first all the individual aspects of each planet, second the aspects
         whitout repetitions.
         """
```

### Comparing `py_astrolab-0.1.4/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.1.5/py_astrolab/charts/charts_svg.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.4/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.1.5/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.4/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.1.5/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.4/py_astrolab/fetch_geonames.py` & `py_astrolab-0.1.5/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.4/py_astrolab/kr.config.json` & `py_astrolab-0.1.5/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.4/py_astrolab/main.py` & `py_astrolab-0.1.5/py_astrolab/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,29 @@
 
     # Generated internally
     julian_day: Union[int, float]
     utc: datetime
 
     now = datetime.now()
 
+    signs_dict = {
+        'Ari': {'extended_name': 'Aries', 'governor': 'Mars', 'opposite': 'Libra'},
+        'Tau': {'extended_name': 'Taurus', 'governor': 'Venus', 'opposite': 'Scorpio'},
+        'Gem': {'extended_name': 'Gemini', 'governor': 'Mercury', 'opposite': 'Sagittarius'},
+        'Can': {'extended_name': 'Cancer', 'governor': 'Moon', 'opposite': 'Capricorn'},
+        'Leo': {'extended_name': 'Leo', 'governor': 'Sun', 'opposite': 'Aquarius'},
+        'Vir': {'extended_name': 'Virgo', 'governor': 'Mercury', 'opposite': 'Pisces'},
+        'Lib': {'extended_name': 'Libra', 'governor': 'Venus', 'opposite': 'Aries'},
+        'Sco': {'extended_name': 'Scorpio', 'governor': 'Mars', 'opposite': 'Taurus'},
+        'Sag': {'extended_name': 'Sagittarius', 'governor': 'Jupiter', 'opposite': 'Gemini'},
+        'Cap': {'extended_name': 'Capricorn', 'governor': 'Saturn', 'opposite': 'Cancer'},
+        'Aqu': {'extended_name': 'Aquarius', 'governor': 'Saturn', 'opposite': 'Leo'},
+        'Pis': {'extended_name': 'Pisces', 'governor': 'Jupiter', 'opposite': 'Virgo'}
+    }
+
     def __init__(
         self,
         name="Now",
         year: int = now.year,
         month: int = now.month,
         day: int = now.day,
         hour: int = now.hour,
```

### Comparing `py_astrolab-0.1.4/py_astrolab/print_all_data.py` & `py_astrolab-0.1.5/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.4/py_astrolab/relationship_score.py` & `py_astrolab-0.1.5/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.4/py_astrolab/report.py` & `py_astrolab-0.1.5/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.4/py_astrolab/types.py` & `py_astrolab-0.1.5/py_astrolab/types.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.4/py_astrolab/utilities.py` & `py_astrolab-0.1.5/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.4/pyproject.toml` & `py_astrolab-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.1.4"
+version = "0.1.5"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.1.4/PKG-INFO` & `py_astrolab-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

