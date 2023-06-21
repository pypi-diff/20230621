# Comparing `tmp/qoyllur_quipu-1.0.1.tar.gz` & `tmp/qoyllur_quipu-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoyllur_quipu-1.0.1.tar", last modified: Sat Nov 27 13:06:23 2021, max compression
+gzip compressed data, was "qoyllur_quipu-1.0.2.tar", last modified: Wed Jun 21 04:24:57 2023, max compression
```

## Comparing `qoyllur_quipu-1.0.1.tar` & `qoyllur_quipu-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kayleigh  (1000) kayleigh  (1000)        0 2021-11-27 13:06:23.675070 qoyllur_quipu-1.0.1/
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)      164 2021-09-26 17:39:33.000000 qoyllur_quipu-1.0.1/MANIFEST.in
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)     5387 2021-11-27 13:06:23.675070 qoyllur_quipu-1.0.1/PKG-INFO
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)     4183 2021-11-27 13:05:22.000000 qoyllur_quipu-1.0.1/README.md
-drwxrwxr-x   0 kayleigh  (1000) kayleigh  (1000)        0 2021-11-27 13:06:23.675070 qoyllur_quipu-1.0.1/q2/
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)      991 2021-09-26 21:04:35.000000 qoyllur_quipu-1.0.1/q2/__init__.py
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)    22312 2020-11-30 00:21:28.000000 qoyllur_quipu-1.0.1/q2/abundances.py
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)     7331 2021-09-27 21:01:19.000000 qoyllur_quipu-1.0.1/q2/config.py
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)     5833 2019-08-24 15:04:17.000000 qoyllur_quipu-1.0.1/q2/errors.py
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)    33910 2021-11-27 12:55:21.000000 qoyllur_quipu-1.0.1/q2/isopars.py
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)     7479 2019-08-24 15:04:17.000000 qoyllur_quipu-1.0.1/q2/modatm.py
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)    11898 2021-09-26 21:20:26.000000 qoyllur_quipu-1.0.1/q2/moog.py
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)    24526 2021-02-19 19:58:18.000000 qoyllur_quipu-1.0.1/q2/specpars.py
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)     7492 2021-09-22 00:39:57.000000 qoyllur_quipu-1.0.1/q2/star.py
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)     4100 2019-08-24 15:04:17.000000 qoyllur_quipu-1.0.1/q2/tools.py
-drwxrwxr-x   0 kayleigh  (1000) kayleigh  (1000)        0 2021-11-27 13:06:23.675070 qoyllur_quipu-1.0.1/qoyllur_quipu.egg-info/
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)     5387 2021-11-27 13:06:23.000000 qoyllur_quipu-1.0.1/qoyllur_quipu.egg-info/PKG-INFO
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)      348 2021-11-27 13:06:23.000000 qoyllur_quipu-1.0.1/qoyllur_quipu.egg-info/SOURCES.txt
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)        1 2021-11-27 13:06:23.000000 qoyllur_quipu-1.0.1/qoyllur_quipu.egg-info/dependency_links.txt
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)       23 2021-11-27 13:06:23.000000 qoyllur_quipu-1.0.1/qoyllur_quipu.egg-info/requires.txt
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)        3 2021-11-27 13:06:23.000000 qoyllur_quipu-1.0.1/qoyllur_quipu.egg-info/top_level.txt
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)       38 2021-11-27 13:06:23.675070 qoyllur_quipu-1.0.1/setup.cfg
--rw-rw-r--   0 kayleigh  (1000) kayleigh  (1000)      774 2021-11-27 13:06:05.000000 qoyllur_quipu-1.0.1/setup.py
+drwxr-xr-x   0 ramstojh   (501) staff       (20)        0 2023-06-21 04:24:57.597010 qoyllur_quipu-1.0.2/
+-rw-------   0 ramstojh   (501) staff       (20)      164 2021-09-26 17:39:33.000000 qoyllur_quipu-1.0.2/MANIFEST.in
+-rw-r--r--   0 ramstojh   (501) staff       (20)     4572 2023-06-21 04:24:57.597463 qoyllur_quipu-1.0.2/PKG-INFO
+-rw-------   0 ramstojh   (501) staff       (20)     4183 2021-11-27 13:05:22.000000 qoyllur_quipu-1.0.2/README.md
+drwxr-xr-x   0 ramstojh   (501) staff       (20)        0 2023-06-21 04:24:57.524899 qoyllur_quipu-1.0.2/q2/
+-rw-------   0 ramstojh   (501) staff       (20)      991 2021-09-26 21:04:35.000000 qoyllur_quipu-1.0.2/q2/__init__.py
+-rw-------   0 ramstojh   (501) staff       (20)    22312 2020-11-30 00:21:28.000000 qoyllur_quipu-1.0.2/q2/abundances.py
+-rw-------   0 ramstojh   (501) staff       (20)     7331 2021-09-27 21:01:19.000000 qoyllur_quipu-1.0.2/q2/config.py
+-rw-------   0 ramstojh   (501) staff       (20)     5833 2019-08-24 15:04:17.000000 qoyllur_quipu-1.0.2/q2/errors.py
+-rw-------   0 ramstojh   (501) staff       (20)    33910 2021-11-27 12:55:21.000000 qoyllur_quipu-1.0.2/q2/isopars.py
+-rw-------   0 ramstojh   (501) staff       (20)     7479 2019-08-24 15:04:17.000000 qoyllur_quipu-1.0.2/q2/modatm.py
+-rw-------   0 ramstojh   (501) staff       (20)    11898 2021-09-26 21:20:26.000000 qoyllur_quipu-1.0.2/q2/moog.py
+-rw-------   0 ramstojh   (501) staff       (20)    24526 2023-06-20 23:34:00.000000 qoyllur_quipu-1.0.2/q2/specpars.py
+-rw-------   0 ramstojh   (501) staff       (20)     7492 2021-09-22 00:39:57.000000 qoyllur_quipu-1.0.2/q2/star.py
+-rw-------   0 ramstojh   (501) staff       (20)     4100 2019-08-24 15:04:17.000000 qoyllur_quipu-1.0.2/q2/tools.py
+drwxr-xr-x   0 ramstojh   (501) staff       (20)        0 2023-06-21 04:24:57.595372 qoyllur_quipu-1.0.2/qoyllur_quipu.egg-info/
+-rw-------   0 ramstojh   (501) staff       (20)     4572 2023-06-21 04:24:57.000000 qoyllur_quipu-1.0.2/qoyllur_quipu.egg-info/PKG-INFO
+-rw-------   0 ramstojh   (501) staff       (20)      358 2023-06-21 04:24:57.000000 qoyllur_quipu-1.0.2/qoyllur_quipu.egg-info/SOURCES.txt
+-rw-------   0 ramstojh   (501) staff       (20)        1 2023-06-21 04:24:57.000000 qoyllur_quipu-1.0.2/qoyllur_quipu.egg-info/dependency_links.txt
+-rw-------   0 ramstojh   (501) staff       (20)       23 2023-06-21 04:24:57.000000 qoyllur_quipu-1.0.2/qoyllur_quipu.egg-info/requires.txt
+-rw-------   0 ramstojh   (501) staff       (20)        3 2023-06-21 04:24:57.000000 qoyllur_quipu-1.0.2/qoyllur_quipu.egg-info/top_level.txt
+-rw-------   0 ramstojh   (501) staff       (20)       38 2023-06-21 04:24:57.600229 qoyllur_quipu-1.0.2/setup.cfg
+-rw-------   0 ramstojh   (501) staff       (20)      774 2023-06-21 04:16:04.000000 qoyllur_quipu-1.0.2/setup.py
```

### Comparing `qoyllur_quipu-1.0.1/PKG-INFO` & `qoyllur_quipu-1.0.2/qoyllur_quipu.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,111 @@
 Metadata-Version: 2.1
-Name: qoyllur_quipu
-Version: 1.0.1
+Name: qoyllur-quipu
+Version: 1.0.2
 Summary: q2 Python Package
 Home-page: https://github.com/astroChasqui/q2
 Author: Ivan Ramirez
 Author-email: iramirez@tacomacc.edu
 License: BSD 2-Clause 'Simplified' License
-Description: # q2 Python package
-        
-        <a href="http://www.as.utexas.edu/~chris/moog.html">
-            <img src="https://img.shields.io/badge/powered%20by-MOOG-orange"/>
-        </a>
-        <a href="https://matplotlib.org/3.1.1/index.html">
-            <img src="https://img.shields.io/badge/powered%20by-matplotlib-orange"/>
-        </a>
-        <a href="https://docs.python.org/3/library/os.html">
-            <img src="https://img.shields.io/badge/powered%20by-os-orange"/>
-        </a>
-        <a href="https://numpy.org/">
-            <img src="https://img.shields.io/badge/powered%20by-numpy-orange"/>
-        </a>
-        <a href="https://scipy.org/">
-            <img src="https://img.shields.io/badge/powered%20by-scipy-orange"/>
-        </a>
-        <a href="https://bokeh.org/">
-            <img src="https://img.shields.io/badge/powered%20by-bokeh-orange"/>
-        <br/>
-        <a href="https://ui.adsabs.harvard.edu/abs/2014A&A...572A..48R">
-            <img src="https://img.shields.io/badge/read-paper-blue"/>
-        
-        The `q2` code allows you to use the 2019 <a href="http://www.as.utexas.edu/~chris/moog.html">MOOG</a> version (in its SILENT mode) to calculate elemental abundances of stars and/or determine their atmospheric parameters using the standard techniques of iron line excitation/ionization equilibrium. It also allows you to calculate other fundamental stellar parameters such as mass and age using isochrones. A tutorial is available <a href="https://github.com/astroChasqui/q2_tutorial">here</a>.
-        
-        Installation
-        ------------
-        The new version of `q2` can only be installed via pip. Simply try:
-        
-        ```bash
-        pip install qoyllur-quipu
-        ```
-        
-        If you have installed the old version of `q2`, you must delete it from your HOME directory and also remove its PATH from bashrc (.bash_profile for Mac OS). Once you have installed `q2`, open a Jupyter Notebook Environment (or iPython) and import `q2`.
-        
-        ```python
-        import q2
-        ```
-        
-        By importing `q2`, the latest version of <a href="http://www.as.utexas.edu/~chris/moog.html">MOOG</a> (2019) will begin to install. The only thing you need to do is declare the kind of machine you are using, i.g., 'rh64' for 64-bit linux (Linux Mint, Ubuntu, etc), 'rh' for 32-bit linux system and 'maclap' for Mac Os. That's all folks. This process is done only once. Note that the `q2` package requires Python 3.7 or later. 
-            
-        Future releases will be upgraded via:
-        
-        ```bash
-        pip install qoyllur-quipu --upgrade
-        ```
-        
-        Quickstart
-        ----------
-        Find spectroscopic parameters of a sample of stars using the Sun as the reference star (strict line-by-line differential analysis):
-        
-        ```python
-        import q2
-        data = q2.Data('stars.csv', 'lines.csv')
-        sp = q2.specpars.SolvePars(grid='marcs')
-        q2.specpars.solve_all(data, sp, 'solution.csv', 'Sun')
-        ```
-        
-        Measure elemental abundances of a sample of stars with respect to the solar abundances (line-by-line):
-        
-        ```python
-        species_ids = ['CI', 'OI', 'BaII']
-        q2.abundances.get_all(data, species_ids, 'abundances.csv', 'Sun')
-        ```
-        
-        Author
-        ------
-        - Ivan Ramirez (iramirez@tacomacc.edu)
-        
-        Maintainers
-        -----------
-        - <a href="https://github.com/ramstojh">Jhon Yana Galarza</a> 
-        - <a href="https://github.com/kaykeigh">Kayleigh Meneghini</a>
-        
-        Preferred citation
-        ------------------
-        
-        If you make use of this code, please cite <a href="https://doi.org/10.1051/0004-6361/201424244">Ramirez et al. 2014, A&A, 572, A48</a>. The BibTeX entry for the paper is:
-        ```bibtex
-        @ARTICLE{Ramirez2014,
-               author = {{Ram{\'\i}rez}, I. and {Mel{\'e}ndez}, J. and {Bean}, J. and {Asplund}, M. and {Bedell}, M. and {Monroe}, T. and {Casagrande}, L. and {Schirbel}, L. and {Dreizler}, S. and {Teske}, J. and {Tucci Maia}, M. and {Alves-Brito}, A. and {Baumann}, P.},
-                title = "{The Solar Twin Planet Search. I. Fundamental parameters of the stellar sample}",
-              journal = {\aap},
-             keywords = {stars: abundances, stars: fundamental parameters, planetary systems, Astrophysics - Solar and Stellar Astrophysics},
-                 year = 2014,
-                month = dec,
-               volume = {572},
-                  eid = {A48},
-                pages = {A48},
-                  doi = {10.1051/0004-6361/201424244},
-        archivePrefix = {arXiv},
-               eprint = {1408.4130},
-         primaryClass = {astro-ph.SR},
-               adsurl = {https://ui.adsabs.harvard.edu/abs/2014A&A...572A..48R},
-              adsnote = {Provided by the SAO/NASA Astrophysics Data System}
-        }
-        ```
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+
+# q2 Python package
+
+<a href="http://www.as.utexas.edu/~chris/moog.html">
+    <img src="https://img.shields.io/badge/powered%20by-MOOG-orange"/>
+</a>
+<a href="https://matplotlib.org/3.1.1/index.html">
+    <img src="https://img.shields.io/badge/powered%20by-matplotlib-orange"/>
+</a>
+<a href="https://docs.python.org/3/library/os.html">
+    <img src="https://img.shields.io/badge/powered%20by-os-orange"/>
+</a>
+<a href="https://numpy.org/">
+    <img src="https://img.shields.io/badge/powered%20by-numpy-orange"/>
+</a>
+<a href="https://scipy.org/">
+    <img src="https://img.shields.io/badge/powered%20by-scipy-orange"/>
+</a>
+<a href="https://bokeh.org/">
+    <img src="https://img.shields.io/badge/powered%20by-bokeh-orange"/>
+<br/>
+<a href="https://ui.adsabs.harvard.edu/abs/2014A&A...572A..48R">
+    <img src="https://img.shields.io/badge/read-paper-blue"/>
+
+The `q2` code allows you to use the 2019 <a href="http://www.as.utexas.edu/~chris/moog.html">MOOG</a> version (in its SILENT mode) to calculate elemental abundances of stars and/or determine their atmospheric parameters using the standard techniques of iron line excitation/ionization equilibrium. It also allows you to calculate other fundamental stellar parameters such as mass and age using isochrones. A tutorial is available <a href="https://github.com/astroChasqui/q2_tutorial">here</a>.
+
+Installation
+------------
+The new version of `q2` can only be installed via pip. Simply try:
+
+```bash
+pip install qoyllur-quipu
+```
+
+If you have installed the old version of `q2`, you must delete it from your HOME directory and also remove its PATH from bashrc (.bash_profile for Mac OS). Once you have installed `q2`, open a Jupyter Notebook Environment (or iPython) and import `q2`.
+
+```python
+import q2
+```
+
+By importing `q2`, the latest version of <a href="http://www.as.utexas.edu/~chris/moog.html">MOOG</a> (2019) will begin to install. The only thing you need to do is declare the kind of machine you are using, i.g., 'rh64' for 64-bit linux (Linux Mint, Ubuntu, etc), 'rh' for 32-bit linux system and 'maclap' for Mac Os. That's all folks. This process is done only once. Note that the `q2` package requires Python 3.7 or later. 
+    
+Future releases will be upgraded via:
+
+```bash
+pip install qoyllur-quipu --upgrade
+```
+
+Quickstart
+----------
+Find spectroscopic parameters of a sample of stars using the Sun as the reference star (strict line-by-line differential analysis):
+
+```python
+import q2
+data = q2.Data('stars.csv', 'lines.csv')
+sp = q2.specpars.SolvePars(grid='marcs')
+q2.specpars.solve_all(data, sp, 'solution.csv', 'Sun')
+```
+
+Measure elemental abundances of a sample of stars with respect to the solar abundances (line-by-line):
+
+```python
+species_ids = ['CI', 'OI', 'BaII']
+q2.abundances.get_all(data, species_ids, 'abundances.csv', 'Sun')
+```
+
+Author
+------
+- Ivan Ramirez (iramirez@tacomacc.edu)
+
+Maintainers
+-----------
+- <a href="https://github.com/ramstojh">Jhon Yana Galarza</a> 
+- <a href="https://github.com/kaykeigh">Kayleigh Meneghini</a>
+
+Preferred citation
+------------------
+
+If you make use of this code, please cite <a href="https://doi.org/10.1051/0004-6361/201424244">Ramirez et al. 2014, A&A, 572, A48</a>. The BibTeX entry for the paper is:
+```bibtex
+@ARTICLE{Ramirez2014,
+       author = {{Ram{\'\i}rez}, I. and {Mel{\'e}ndez}, J. and {Bean}, J. and {Asplund}, M. and {Bedell}, M. and {Monroe}, T. and {Casagrande}, L. and {Schirbel}, L. and {Dreizler}, S. and {Teske}, J. and {Tucci Maia}, M. and {Alves-Brito}, A. and {Baumann}, P.},
+        title = "{The Solar Twin Planet Search. I. Fundamental parameters of the stellar sample}",
+      journal = {\aap},
+     keywords = {stars: abundances, stars: fundamental parameters, planetary systems, Astrophysics - Solar and Stellar Astrophysics},
+         year = 2014,
+        month = dec,
+       volume = {572},
+          eid = {A48},
+        pages = {A48},
+          doi = {10.1051/0004-6361/201424244},
+archivePrefix = {arXiv},
+       eprint = {1408.4130},
+ primaryClass = {astro-ph.SR},
+       adsurl = {https://ui.adsabs.harvard.edu/abs/2014A&A...572A..48R},
+      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+}
+```
+
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 2.1 Name: qoyllur_quipu Version: 1.0.1 Summary: q2 Python
+Metadata-Version: 2.1 Name: qoyllur-quipu Version: 1.0.2 Summary: q2 Python
 Package Home-page: https://github.com/astroChasqui/q2 Author: Ivan Ramirez
 Author-email: iramirez@tacomacc.edu License: BSD 2-Clause 'Simplified' License
-Description: # q2 Python package [https://img.shields.io/badge/powered%20by-
-MOOG-orange] [https://img.shields.io/badge/powered%20by-matplotlib-orange]
-[https://img.shields.io/badge/powered%20by-os-orange] [https://img.shields.io/
-badge/powered%20by-numpy-orange] [https://img.shields.io/badge/powered%20by-
-scipy-orange] [https://img.shields.io/badge/powered%20by-bokeh-orange]_
+Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
+OS Independent Requires-Python: >=3.5 Description-Content-Type: text/markdown #
+q2 Python package [https://img.shields.io/badge/powered%20by-MOOG-orange]
+[https://img.shields.io/badge/powered%20by-matplotlib-orange] [https://
+img.shields.io/badge/powered%20by-os-orange] [https://img.shields.io/badge/
+powered%20by-numpy-orange] [https://img.shields.io/badge/powered%20by-scipy-
+orange] [https://img.shields.io/badge/powered%20by-bokeh-orange]_
 [https://img.shields.io/badge/read-paper-blue]_The_`q2`_code_allows_you_to_use
 the_2019_MOOG_version_(in_its_SILENT_mode)_to_calculate_elemental_abundances_of
 stars_and/or_determine_their_atmospheric_parameters_using_the_standard
 techniques_of_iron_line_excitation/ionization_equilibrium._It_also_allows_you
 to_calculate_other_fundamental_stellar_parameters_such_as_mass_and_age_using
 isochrones._A_tutorial_is_available_here._Installation_------------_The_new
 version_of_`q2`_can_only_be_installed_via_pip._Simply_try:_```bash_pip_install
@@ -40,10 +42,8 @@
 {Baumann},_P.},_title_=_"{The_Solar_Twin_Planet_Search._I._Fundamental
 parameters_of_the_stellar_sample}",_journal_=_{\aap},_keywords_=_{stars:
 abundances,_stars:_fundamental_parameters,_planetary_systems,_Astrophysics_-
 Solar_and_Stellar_Astrophysics},_year_=_2014,_month_=_dec,_volume_=_{572},_eid
 =_{A48},_pages_=_{A48},_doi_=_{10.1051/0004-6361/201424244},_archivePrefix_=_
 {arXiv},_eprint_=_{1408.4130},_primaryClass_=_{astro-ph.SR},_adsurl_=_{https://
 ui.adsabs.harvard.edu/abs/2014A&A...572A..48R},_adsnote_=_{Provided_by_the_SAO/
-NASA_Astrophysics_Data_System}_}_```_Platform:_UNKNOWN_Classifier:_Programming
-Language_::_Python_::_3_Classifier:_Operating_System_::_OS_Independent
-Requires-Python:_>=3.5_Description-Content-Type:_text/markdown_
+NASA_Astrophysics_Data_System}_}_```_
```

### Comparing `qoyllur_quipu-1.0.1/README.md` & `qoyllur_quipu-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qoyllur_quipu-1.0.1/q2/__init__.py` & `qoyllur_quipu-1.0.2/q2/__init__.py`

 * *Files identical despite different names*

### Comparing `qoyllur_quipu-1.0.1/q2/abundances.py` & `qoyllur_quipu-1.0.2/q2/abundances.py`

 * *Files identical despite different names*

### Comparing `qoyllur_quipu-1.0.1/q2/config.py` & `qoyllur_quipu-1.0.2/q2/config.py`

 * *Files identical despite different names*

### Comparing `qoyllur_quipu-1.0.1/q2/errors.py` & `qoyllur_quipu-1.0.2/q2/errors.py`

 * *Files identical despite different names*

### Comparing `qoyllur_quipu-1.0.1/q2/isopars.py` & `qoyllur_quipu-1.0.2/q2/isopars.py`

 * *Files identical despite different names*

### Comparing `qoyllur_quipu-1.0.1/q2/modatm.py` & `qoyllur_quipu-1.0.2/q2/modatm.py`

 * *Files identical despite different names*

### Comparing `qoyllur_quipu-1.0.1/q2/moog.py` & `qoyllur_quipu-1.0.2/q2/moog.py`

 * *Files identical despite different names*

### Comparing `qoyllur_quipu-1.0.1/q2/specpars.py` & `qoyllur_quipu-1.0.2/q2/specpars.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import logging
 import matplotlib.pyplot as plt
 from . import moog, errors
 from .tools import linfit
 from .star import Star
 import datetime
-from scipy import ma
+from numpy import ma
 from collections import OrderedDict
 from bokeh.plotting import *
 from bokeh.models import HoverTool
 
 logger = logging.getLogger(__name__)
```

### Comparing `qoyllur_quipu-1.0.1/q2/star.py` & `qoyllur_quipu-1.0.2/q2/star.py`

 * *Files identical despite different names*

### Comparing `qoyllur_quipu-1.0.1/q2/tools.py` & `qoyllur_quipu-1.0.2/q2/tools.py`

 * *Files identical despite different names*

### Comparing `qoyllur_quipu-1.0.1/qoyllur_quipu.egg-info/PKG-INFO` & `qoyllur_quipu-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,112 +1,111 @@
 Metadata-Version: 2.1
-Name: qoyllur-quipu
-Version: 1.0.1
+Name: qoyllur_quipu
+Version: 1.0.2
 Summary: q2 Python Package
 Home-page: https://github.com/astroChasqui/q2
 Author: Ivan Ramirez
 Author-email: iramirez@tacomacc.edu
 License: BSD 2-Clause 'Simplified' License
-Description: # q2 Python package
-        
-        <a href="http://www.as.utexas.edu/~chris/moog.html">
-            <img src="https://img.shields.io/badge/powered%20by-MOOG-orange"/>
-        </a>
-        <a href="https://matplotlib.org/3.1.1/index.html">
-            <img src="https://img.shields.io/badge/powered%20by-matplotlib-orange"/>
-        </a>
-        <a href="https://docs.python.org/3/library/os.html">
-            <img src="https://img.shields.io/badge/powered%20by-os-orange"/>
-        </a>
-        <a href="https://numpy.org/">
-            <img src="https://img.shields.io/badge/powered%20by-numpy-orange"/>
-        </a>
-        <a href="https://scipy.org/">
-            <img src="https://img.shields.io/badge/powered%20by-scipy-orange"/>
-        </a>
-        <a href="https://bokeh.org/">
-            <img src="https://img.shields.io/badge/powered%20by-bokeh-orange"/>
-        <br/>
-        <a href="https://ui.adsabs.harvard.edu/abs/2014A&A...572A..48R">
-            <img src="https://img.shields.io/badge/read-paper-blue"/>
-        
-        The `q2` code allows you to use the 2019 <a href="http://www.as.utexas.edu/~chris/moog.html">MOOG</a> version (in its SILENT mode) to calculate elemental abundances of stars and/or determine their atmospheric parameters using the standard techniques of iron line excitation/ionization equilibrium. It also allows you to calculate other fundamental stellar parameters such as mass and age using isochrones. A tutorial is available <a href="https://github.com/astroChasqui/q2_tutorial">here</a>.
-        
-        Installation
-        ------------
-        The new version of `q2` can only be installed via pip. Simply try:
-        
-        ```bash
-        pip install qoyllur-quipu
-        ```
-        
-        If you have installed the old version of `q2`, you must delete it from your HOME directory and also remove its PATH from bashrc (.bash_profile for Mac OS). Once you have installed `q2`, open a Jupyter Notebook Environment (or iPython) and import `q2`.
-        
-        ```python
-        import q2
-        ```
-        
-        By importing `q2`, the latest version of <a href="http://www.as.utexas.edu/~chris/moog.html">MOOG</a> (2019) will begin to install. The only thing you need to do is declare the kind of machine you are using, i.g., 'rh64' for 64-bit linux (Linux Mint, Ubuntu, etc), 'rh' for 32-bit linux system and 'maclap' for Mac Os. That's all folks. This process is done only once. Note that the `q2` package requires Python 3.7 or later. 
-            
-        Future releases will be upgraded via:
-        
-        ```bash
-        pip install qoyllur-quipu --upgrade
-        ```
-        
-        Quickstart
-        ----------
-        Find spectroscopic parameters of a sample of stars using the Sun as the reference star (strict line-by-line differential analysis):
-        
-        ```python
-        import q2
-        data = q2.Data('stars.csv', 'lines.csv')
-        sp = q2.specpars.SolvePars(grid='marcs')
-        q2.specpars.solve_all(data, sp, 'solution.csv', 'Sun')
-        ```
-        
-        Measure elemental abundances of a sample of stars with respect to the solar abundances (line-by-line):
-        
-        ```python
-        species_ids = ['CI', 'OI', 'BaII']
-        q2.abundances.get_all(data, species_ids, 'abundances.csv', 'Sun')
-        ```
-        
-        Author
-        ------
-        - Ivan Ramirez (iramirez@tacomacc.edu)
-        
-        Maintainers
-        -----------
-        - <a href="https://github.com/ramstojh">Jhon Yana Galarza</a> 
-        - <a href="https://github.com/kaykeigh">Kayleigh Meneghini</a>
-        
-        Preferred citation
-        ------------------
-        
-        If you make use of this code, please cite <a href="https://doi.org/10.1051/0004-6361/201424244">Ramirez et al. 2014, A&A, 572, A48</a>. The BibTeX entry for the paper is:
-        ```bibtex
-        @ARTICLE{Ramirez2014,
-               author = {{Ram{\'\i}rez}, I. and {Mel{\'e}ndez}, J. and {Bean}, J. and {Asplund}, M. and {Bedell}, M. and {Monroe}, T. and {Casagrande}, L. and {Schirbel}, L. and {Dreizler}, S. and {Teske}, J. and {Tucci Maia}, M. and {Alves-Brito}, A. and {Baumann}, P.},
-                title = "{The Solar Twin Planet Search. I. Fundamental parameters of the stellar sample}",
-              journal = {\aap},
-             keywords = {stars: abundances, stars: fundamental parameters, planetary systems, Astrophysics - Solar and Stellar Astrophysics},
-                 year = 2014,
-                month = dec,
-               volume = {572},
-                  eid = {A48},
-                pages = {A48},
-                  doi = {10.1051/0004-6361/201424244},
-        archivePrefix = {arXiv},
-               eprint = {1408.4130},
-         primaryClass = {astro-ph.SR},
-               adsurl = {https://ui.adsabs.harvard.edu/abs/2014A&A...572A..48R},
-              adsnote = {Provided by the SAO/NASA Astrophysics Data System}
-        }
-        ```
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+
+# q2 Python package
+
+<a href="http://www.as.utexas.edu/~chris/moog.html">
+    <img src="https://img.shields.io/badge/powered%20by-MOOG-orange"/>
+</a>
+<a href="https://matplotlib.org/3.1.1/index.html">
+    <img src="https://img.shields.io/badge/powered%20by-matplotlib-orange"/>
+</a>
+<a href="https://docs.python.org/3/library/os.html">
+    <img src="https://img.shields.io/badge/powered%20by-os-orange"/>
+</a>
+<a href="https://numpy.org/">
+    <img src="https://img.shields.io/badge/powered%20by-numpy-orange"/>
+</a>
+<a href="https://scipy.org/">
+    <img src="https://img.shields.io/badge/powered%20by-scipy-orange"/>
+</a>
+<a href="https://bokeh.org/">
+    <img src="https://img.shields.io/badge/powered%20by-bokeh-orange"/>
+<br/>
+<a href="https://ui.adsabs.harvard.edu/abs/2014A&A...572A..48R">
+    <img src="https://img.shields.io/badge/read-paper-blue"/>
+
+The `q2` code allows you to use the 2019 <a href="http://www.as.utexas.edu/~chris/moog.html">MOOG</a> version (in its SILENT mode) to calculate elemental abundances of stars and/or determine their atmospheric parameters using the standard techniques of iron line excitation/ionization equilibrium. It also allows you to calculate other fundamental stellar parameters such as mass and age using isochrones. A tutorial is available <a href="https://github.com/astroChasqui/q2_tutorial">here</a>.
+
+Installation
+------------
+The new version of `q2` can only be installed via pip. Simply try:
+
+```bash
+pip install qoyllur-quipu
+```
+
+If you have installed the old version of `q2`, you must delete it from your HOME directory and also remove its PATH from bashrc (.bash_profile for Mac OS). Once you have installed `q2`, open a Jupyter Notebook Environment (or iPython) and import `q2`.
+
+```python
+import q2
+```
+
+By importing `q2`, the latest version of <a href="http://www.as.utexas.edu/~chris/moog.html">MOOG</a> (2019) will begin to install. The only thing you need to do is declare the kind of machine you are using, i.g., 'rh64' for 64-bit linux (Linux Mint, Ubuntu, etc), 'rh' for 32-bit linux system and 'maclap' for Mac Os. That's all folks. This process is done only once. Note that the `q2` package requires Python 3.7 or later. 
+    
+Future releases will be upgraded via:
+
+```bash
+pip install qoyllur-quipu --upgrade
+```
+
+Quickstart
+----------
+Find spectroscopic parameters of a sample of stars using the Sun as the reference star (strict line-by-line differential analysis):
+
+```python
+import q2
+data = q2.Data('stars.csv', 'lines.csv')
+sp = q2.specpars.SolvePars(grid='marcs')
+q2.specpars.solve_all(data, sp, 'solution.csv', 'Sun')
+```
+
+Measure elemental abundances of a sample of stars with respect to the solar abundances (line-by-line):
+
+```python
+species_ids = ['CI', 'OI', 'BaII']
+q2.abundances.get_all(data, species_ids, 'abundances.csv', 'Sun')
+```
+
+Author
+------
+- Ivan Ramirez (iramirez@tacomacc.edu)
+
+Maintainers
+-----------
+- <a href="https://github.com/ramstojh">Jhon Yana Galarza</a> 
+- <a href="https://github.com/kaykeigh">Kayleigh Meneghini</a>
+
+Preferred citation
+------------------
+
+If you make use of this code, please cite <a href="https://doi.org/10.1051/0004-6361/201424244">Ramirez et al. 2014, A&A, 572, A48</a>. The BibTeX entry for the paper is:
+```bibtex
+@ARTICLE{Ramirez2014,
+       author = {{Ram{\'\i}rez}, I. and {Mel{\'e}ndez}, J. and {Bean}, J. and {Asplund}, M. and {Bedell}, M. and {Monroe}, T. and {Casagrande}, L. and {Schirbel}, L. and {Dreizler}, S. and {Teske}, J. and {Tucci Maia}, M. and {Alves-Brito}, A. and {Baumann}, P.},
+        title = "{The Solar Twin Planet Search. I. Fundamental parameters of the stellar sample}",
+      journal = {\aap},
+     keywords = {stars: abundances, stars: fundamental parameters, planetary systems, Astrophysics - Solar and Stellar Astrophysics},
+         year = 2014,
+        month = dec,
+       volume = {572},
+          eid = {A48},
+        pages = {A48},
+          doi = {10.1051/0004-6361/201424244},
+archivePrefix = {arXiv},
+       eprint = {1408.4130},
+ primaryClass = {astro-ph.SR},
+       adsurl = {https://ui.adsabs.harvard.edu/abs/2014A&A...572A..48R},
+      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+}
+```
+
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 2.1 Name: qoyllur-quipu Version: 1.0.1 Summary: q2 Python
+Metadata-Version: 2.1 Name: qoyllur_quipu Version: 1.0.2 Summary: q2 Python
 Package Home-page: https://github.com/astroChasqui/q2 Author: Ivan Ramirez
 Author-email: iramirez@tacomacc.edu License: BSD 2-Clause 'Simplified' License
-Description: # q2 Python package [https://img.shields.io/badge/powered%20by-
-MOOG-orange] [https://img.shields.io/badge/powered%20by-matplotlib-orange]
-[https://img.shields.io/badge/powered%20by-os-orange] [https://img.shields.io/
-badge/powered%20by-numpy-orange] [https://img.shields.io/badge/powered%20by-
-scipy-orange] [https://img.shields.io/badge/powered%20by-bokeh-orange]_
+Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
+OS Independent Requires-Python: >=3.5 Description-Content-Type: text/markdown #
+q2 Python package [https://img.shields.io/badge/powered%20by-MOOG-orange]
+[https://img.shields.io/badge/powered%20by-matplotlib-orange] [https://
+img.shields.io/badge/powered%20by-os-orange] [https://img.shields.io/badge/
+powered%20by-numpy-orange] [https://img.shields.io/badge/powered%20by-scipy-
+orange] [https://img.shields.io/badge/powered%20by-bokeh-orange]_
 [https://img.shields.io/badge/read-paper-blue]_The_`q2`_code_allows_you_to_use
 the_2019_MOOG_version_(in_its_SILENT_mode)_to_calculate_elemental_abundances_of
 stars_and/or_determine_their_atmospheric_parameters_using_the_standard
 techniques_of_iron_line_excitation/ionization_equilibrium._It_also_allows_you
 to_calculate_other_fundamental_stellar_parameters_such_as_mass_and_age_using
 isochrones._A_tutorial_is_available_here._Installation_------------_The_new
 version_of_`q2`_can_only_be_installed_via_pip._Simply_try:_```bash_pip_install
@@ -40,10 +42,8 @@
 {Baumann},_P.},_title_=_"{The_Solar_Twin_Planet_Search._I._Fundamental
 parameters_of_the_stellar_sample}",_journal_=_{\aap},_keywords_=_{stars:
 abundances,_stars:_fundamental_parameters,_planetary_systems,_Astrophysics_-
 Solar_and_Stellar_Astrophysics},_year_=_2014,_month_=_dec,_volume_=_{572},_eid
 =_{A48},_pages_=_{A48},_doi_=_{10.1051/0004-6361/201424244},_archivePrefix_=_
 {arXiv},_eprint_=_{1408.4130},_primaryClass_=_{astro-ph.SR},_adsurl_=_{https://
 ui.adsabs.harvard.edu/abs/2014A&A...572A..48R},_adsnote_=_{Provided_by_the_SAO/
-NASA_Astrophysics_Data_System}_}_```_Platform:_UNKNOWN_Classifier:_Programming
-Language_::_Python_::_3_Classifier:_Operating_System_::_OS_Independent
-Requires-Python:_>=3.5_Description-Content-Type:_text/markdown_
+NASA_Astrophysics_Data_System}_}_```_
```

### Comparing `qoyllur_quipu-1.0.1/setup.py` & `qoyllur_quipu-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
   
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 setup(
     name="qoyllur_quipu",
     version=__version__,
     description="q2 Python Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ivan Ramirez",
```

