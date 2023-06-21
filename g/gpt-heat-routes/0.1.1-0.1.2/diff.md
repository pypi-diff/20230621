# Comparing `tmp/gpt_heat_routes-0.1.1.tar.gz` & `tmp/gpt_heat_routes-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_heat_routes-0.1.1.tar", last modified: Sun Jun 18 13:39:10 2023, max compression
+gzip compressed data, was "gpt_heat_routes-0.1.2.tar", last modified: Wed Jun 21 13:08:28 2023, max compression
```

## Comparing `gpt_heat_routes-0.1.1.tar` & `gpt_heat_routes-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-18 13:39:10.320149 gpt_heat_routes-0.1.1/
--rw-r--r--   0 christostrydom   (501) staff       (20)      243 2023-06-18 13:39:10.319889 gpt_heat_routes-0.1.1/PKG-INFO
--rw-r--r--   0 christostrydom   (501) staff       (20)     2264 2023-06-18 12:33:36.000000 gpt_heat_routes-0.1.1/README.md
-drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-18 13:39:10.316353 gpt_heat_routes-0.1.1/gpt_heat_routes/
--rw-r--r--   0 christostrydom   (501) staff       (20)       32 2023-06-18 12:41:18.000000 gpt_heat_routes-0.1.1/gpt_heat_routes/__init__.py
--rw-r--r--   0 christostrydom   (501) staff       (20)     9885 2023-06-17 09:41:19.000000 gpt_heat_routes-0.1.1/gpt_heat_routes/gpt_heat_routes.py
-drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-18 13:39:10.319485 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/
--rw-r--r--   0 christostrydom   (501) staff       (20)      243 2023-06-18 13:39:10.000000 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/PKG-INFO
--rw-r--r--   0 christostrydom   (501) staff       (20)      275 2023-06-18 13:39:10.000000 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/SOURCES.txt
--rw-r--r--   0 christostrydom   (501) staff       (20)        1 2023-06-18 13:39:10.000000 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/dependency_links.txt
--rw-r--r--   0 christostrydom   (501) staff       (20)       53 2023-06-18 13:39:10.000000 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/requires.txt
--rw-r--r--   0 christostrydom   (501) staff       (20)       16 2023-06-18 13:39:10.000000 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/top_level.txt
--rw-r--r--   0 christostrydom   (501) staff       (20)       38 2023-06-18 13:39:10.320218 gpt_heat_routes-0.1.1/setup.cfg
--rw-r--r--   0 christostrydom   (501) staff       (20)      500 2023-06-18 13:38:15.000000 gpt_heat_routes-0.1.1/setup.py
+drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-21 13:08:28.898262 gpt_heat_routes-0.1.2/
+-rw-r--r--   0 christostrydom   (501) staff       (20)      181 2023-06-21 13:08:28.897939 gpt_heat_routes-0.1.2/PKG-INFO
+-rw-r--r--   0 christostrydom   (501) staff       (20)     2264 2023-06-18 13:46:05.000000 gpt_heat_routes-0.1.2/README.md
+drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-21 13:08:28.894590 gpt_heat_routes-0.1.2/gpt_heat_routes/
+-rw-r--r--   0 christostrydom   (501) staff       (20)       31 2023-06-18 13:46:05.000000 gpt_heat_routes-0.1.2/gpt_heat_routes/__init__.py
+-rw-r--r--   0 christostrydom   (501) staff       (20)     9489 2023-06-21 12:57:19.000000 gpt_heat_routes-0.1.2/gpt_heat_routes/gpt_heat_routes.py
+drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-21 13:08:28.897400 gpt_heat_routes-0.1.2/gpt_heat_routes.egg-info/
+-rw-r--r--   0 christostrydom   (501) staff       (20)      181 2023-06-21 13:08:28.000000 gpt_heat_routes-0.1.2/gpt_heat_routes.egg-info/PKG-INFO
+-rw-r--r--   0 christostrydom   (501) staff       (20)      275 2023-06-21 13:08:28.000000 gpt_heat_routes-0.1.2/gpt_heat_routes.egg-info/SOURCES.txt
+-rw-r--r--   0 christostrydom   (501) staff       (20)        1 2023-06-21 13:08:28.000000 gpt_heat_routes-0.1.2/gpt_heat_routes.egg-info/dependency_links.txt
+-rw-r--r--   0 christostrydom   (501) staff       (20)       53 2023-06-21 13:08:28.000000 gpt_heat_routes-0.1.2/gpt_heat_routes.egg-info/requires.txt
+-rw-r--r--   0 christostrydom   (501) staff       (20)       16 2023-06-21 13:08:28.000000 gpt_heat_routes-0.1.2/gpt_heat_routes.egg-info/top_level.txt
+-rw-r--r--   0 christostrydom   (501) staff       (20)       38 2023-06-21 13:08:28.898329 gpt_heat_routes-0.1.2/setup.cfg
+-rw-r--r--   0 christostrydom   (501) staff       (20)      503 2023-06-21 13:08:16.000000 gpt_heat_routes-0.1.2/setup.py
```

### Comparing `gpt_heat_routes-0.1.1/README.md` & `gpt_heat_routes-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gpt_heat_routes-0.1.1/gpt_heat_routes/gpt_heat_routes.py` & `gpt_heat_routes-0.1.2/gpt_heat_routes/gpt_heat_routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,37 +191,22 @@
     GE.set_index(["u", "v", "key"], inplace=True)
     GE = GE[~GE[popup_vals].isna()]
     return GE
 
 
 def get_colormap_legend(df, color_col, count_col):
     """Get a branca colormap based on the colors in the given dataframe."""
-    df = df[[color_col, count_col]].drop_duplicates().sort_values(count_col)
-
-    unique_colors = list(df[color_col].unique())
 
-    if len(unique_colors) < 2:
-        # Handle the case with less than 2 unique colors
-        # You can assign a default colormap or handle it differently
-        print("Not enough unique colors. Please provide at least 2 colors.")
-        return None
+    # Create a dictionary mapping each unique value in 'count_col' to a color in 'color_col'
+    color_dict = dict(zip(df[count_col], df[color_col]))
 
-    cmapl = (
-        bcm.LinearColormap(
-            unique_colors,
-            vmin=df[count_col].min(),
-            vmax=df[count_col].max(),
-            index=list(df[count_col]),
-        )
-        .scale(vmin=df[count_col].min(), vmax=df[count_col].max())
-        .to_step(10)
-    )
-    cmapl.caption = "Number of PVs"
-    return cmapl
+    # Create a discrete colormap using the color_dict
+    cmap = bcm.StepColormap(colors=color_dict.values(), index=color_dict.keys(), caption="Number of PVs")
 
+    return cmap
 
 def get_colormap_legend_depr(df, color_col, count_col):
     df = df[[color_col, count_col]].drop_duplicates().sort_values(count_col)
     cmapl = (
         bcm.LinearColormap(
             list(df[color_col]),
             vmin=df[count_col].min(),
```

