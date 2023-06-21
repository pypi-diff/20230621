# Comparing `tmp/arcane-date-0.1.2.tar.gz` & `tmp/arcane_date-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcane-date-0.1.2.tar", max compression
+gzip compressed data, was "arcane_date-0.1.3.tar", max compression
```

## Comparing `arcane-date-0.1.2.tar` & `arcane_date-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0       56 2022-08-08 11:44:19.323128 arcane-date-0.1.2/README.md
--rw-r--r--   0        0        0     2211 2022-08-08 11:44:19.323128 arcane-date-0.1.2/arcane/date.py
--rw-r--r--   0        0        0      395 2022-08-08 11:44:19.323128 arcane-date-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      575 2022-08-08 11:44:40.343641 arcane-date-0.1.2/setup.py
--rw-r--r--   0        0        0      566 2022-08-08 11:44:40.343928 arcane-date-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       56 2023-06-21 10:16:41.990475 arcane_date-0.1.3/README.md
+-rw-r--r--   0        0        0     2219 2023-06-21 10:16:41.990475 arcane_date-0.1.3/arcane/date.py
+-rw-r--r--   0        0        0      395 2023-06-21 10:16:41.990475 arcane_date-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 arcane_date-0.1.3/PKG-INFO
```

### Comparing `arcane-date-0.1.2/arcane/date.py` & `arcane_date-0.1.3/arcane/date.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,13 +45,13 @@
         end_date (datetime): The ending date of the range
         period_length (int, optional): The size of each each period. Defaults to 30.
 
     Yields:
         Iterator[tuple[datetime, datetime]]: An iterator of tuples of the form (period_start, period_end)
     """
     nb_days = (end_date - start_date).days
-    nb_of_period = math.ceil(nb_days / period_length)
+    nb_of_period = max(math.ceil(nb_days / period_length), 1)
     for i in range(nb_of_period):
         period_end = start_date + timedelta(days=(i + 1) * period_length - 1)
         if period_end > end_date:
             period_end = end_date
         yield start_date + timedelta(days=i * period_length), period_end
```

### Comparing `arcane-date-0.1.2/PKG-INFO` & `arcane_date-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: arcane-date
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to work with dates
 Author: Arcane
 Author-email: product@arcane.run
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Arcane date
 
 This package helps us to work with dates
```

