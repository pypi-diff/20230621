# Comparing `tmp/segment-geospatial-0.8.2.tar.gz` & `tmp/segment-geospatial-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.8.2.tar", last modified: Wed Jun 14 13:41:10 2023, max compression
+gzip compressed data, was "segment-geospatial-0.8.3.tar", last modified: Wed Jun 21 03:39:32 2023, max compression
```

## Comparing `segment-geospatial-0.8.2.tar` & `segment-geospatial-0.8.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:41:10.766271 segment-geospatial-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-14 13:41:01.000000 segment-geospatial-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-14 13:41:01.000000 segment-geospatial-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-14 13:41:10.766271 segment-geospatial-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-14 13:41:01.000000 segment-geospatial-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-14 13:41:01.000000 segment-geospatial-0.8.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:41:10.766271 segment-geospatial-0.8.2/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-14 13:41:01.000000 segment-geospatial-0.8.2/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86998 2023-06-14 13:41:01.000000 segment-geospatial-0.8.2/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    29816 2023-06-14 13:41:01.000000 segment-geospatial-0.8.2/samgeo/samgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)    16816 2023-06-14 13:41:01.000000 segment-geospatial-0.8.2/samgeo/text_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:41:10.766271 segment-geospatial-0.8.2/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-14 13:41:10.000000 segment-geospatial-0.8.2/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-14 13:41:10.000000 segment-geospatial-0.8.2/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-14 13:41:10.000000 segment-geospatial-0.8.2/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:41:10.000000 segment-geospatial-0.8.2/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-14 13:41:10.000000 segment-geospatial-0.8.2/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 13:41:10.000000 segment-geospatial-0.8.2/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-14 13:41:10.766271 segment-geospatial-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-14 13:41:01.000000 segment-geospatial-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:39:32.241140 segment-geospatial-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-21 03:39:32.241140 segment-geospatial-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:39:32.241140 segment-geospatial-0.8.3/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92509 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29816 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/samgeo/samgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/samgeo/text_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:39:32.241140 segment-geospatial-0.8.3/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-21 03:39:32.241140 segment-geospatial-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/setup.py
```

### Comparing `segment-geospatial-0.8.2/LICENSE` & `segment-geospatial-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.8.2/PKG-INFO` & `segment-geospatial-0.8.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.8.2
+Version: 0.8.3
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -58,15 +58,17 @@
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
 -   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
 -   [Segmenting imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
+-   [Batch segmentation with text prompts](https://samgeo.gishub.org/examples/text_prompts_batch)
 -   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/arcgis)
+-   [Segmenting swimming pools with text prompts](https://samgeo.gishub.org/examples/swimming_pools)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
 
@@ -105,14 +107,14 @@
 
 ## Computing Resources
 
 The Segment Anything Model is computationally intensive, and a powerful GPU is recommended to process large datasets. It is recommended to have a GPU with at least 8 GB of GPU memory. You can utilize the free GPU resources provided by Google Colab. Alternatively, you can apply for [AWS Cloud Credit for Research](https://aws.amazon.com/government-education/research-and-technical-computing/cloud-credit-for-research), which offers cloud credits to support academic research. If you are in the Greater China region, apply for the AWS Cloud Credit [here](https://aws.amazon.com/cn/events/educate_cloud/research-credits).
 
 ## Acknowledgements
 
-This package was made possible by the following open source projects. Credit goes to the developers of these projects.
+This project is supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
 -   [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO)
 -   [lang-segment-anything](https://github.com/luca-medeiros/lang-segment-anything)
```

### Comparing `segment-geospatial-0.8.2/README.md` & `segment-geospatial-0.8.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
 -   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
 -   [Segmenting imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
+-   [Batch segmentation with text prompts](https://samgeo.gishub.org/examples/text_prompts_batch)
 -   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/arcgis)
+-   [Segmenting swimming pools with text prompts](https://samgeo.gishub.org/examples/swimming_pools)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
 
@@ -83,14 +85,14 @@
 
 ## Computing Resources
 
 The Segment Anything Model is computationally intensive, and a powerful GPU is recommended to process large datasets. It is recommended to have a GPU with at least 8 GB of GPU memory. You can utilize the free GPU resources provided by Google Colab. Alternatively, you can apply for [AWS Cloud Credit for Research](https://aws.amazon.com/government-education/research-and-technical-computing/cloud-credit-for-research), which offers cloud credits to support academic research. If you are in the Greater China region, apply for the AWS Cloud Credit [here](https://aws.amazon.com/cn/events/educate_cloud/research-credits).
 
 ## Acknowledgements
 
-This package was made possible by the following open source projects. Credit goes to the developers of these projects.
+This project is supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
 -   [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO)
 -   [lang-segment-anything](https://github.com/luca-medeiros/lang-segment-anything)
```

### Comparing `segment-geospatial-0.8.2/samgeo/common.py` & `segment-geospatial-0.8.3/samgeo/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -508,18 +508,16 @@
         return r.content
 
     def draw_tile(
         source, lat0, lon0, lat1, lon1, zoom, filename, quiet=False, **kwargs
     ):
         x0, y0 = deg2num(lat0, lon0, zoom)
         x1, y1 = deg2num(lat1, lon1, zoom)
-        if x0 > x1:
-            x0, x1 = x1, x0
-        if y0 > y1:
-            y0, y1 = y1, y0
+        x0, x1 = sorted([x0, x1])
+        y0, y1 = sorted([y0, y1])
         corners = tuple(
             itertools.product(
                 range(math.floor(x0), math.ceil(x1)),
                 range(math.floor(y0), math.ceil(y1)),
             )
         )
         totalnum = len(corners)
@@ -898,24 +896,24 @@
     h, w = sample_h, sample_w
     blocks = []
     height = h + 2 * bound
     width = w + 2 * bound
 
     for y in range(-bound, raster_h, h):
         for x in range(-bound, raster_w, w):
-            rigth_x_bound = max(bound, x + width - raster_w)
+            right_x_bound = max(bound, x + width - raster_w)
             bottom_y_bound = max(bound, y + height - raster_h)
 
             blocks.append(
                 {
                     "x": x,
                     "y": y,
                     "height": height,
                     "width": width,
-                    "bounds": [[bound, bottom_y_bound], [bound, rigth_x_bound]],
+                    "bounds": [[bound, bottom_y_bound], [bound, right_x_bound]],
                 }
             )
     return blocks
 
 
 def read_block(src, x, y, height, width, nodata=0, **kwargs):
     return src.read(
@@ -1384,15 +1382,15 @@
     )
     if title is not None:
         plt.title(title)
     plt.axis(axis)
     plt.show()
 
 
-def show_box(image, box, ax):
+def show_box(box, ax):
     ax = plt.gca()
     x0, y0 = box[0], box[1]
     w, h = box[2] - box[0], box[3] - box[1]
     ax.add_patch(
         plt.Rectangle((x0, y0), w, h, edgecolor="green", facecolor=(0, 0, 0, 0), lw=2)
     )
 
@@ -2185,15 +2183,15 @@
         raise ValueError("Input image must be a URL or a NumPy array.")
 
     # Create an empty list to store the mouse click coordinates
     left_clicks = []
     right_clicks = []
 
     # Create a mouse callback function
-    def get_mouse_coordinates(event, x, y, flags, param):
+    def get_mouse_coordinates(event, x, y):
         if event == cv2.EVENT_LBUTTONDOWN:
             # Append the coordinates to the mouse_clicks list
             left_clicks.append((x, y))
 
             # Draw a green circle at the mouse click coordinates
             cv2.circle(image, (x, y), radius, fg_color, -1)
 
@@ -2255,15 +2253,24 @@
             if output:
                 print(output.decode("utf-8").strip())
 
         # Wait for process to complete
         process.wait()
 
 
-def text_sam_gui(sam, basemap="SATELLITE", out_dir=None, **kwargs):
+def text_sam_gui(
+    sam,
+    basemap="SATELLITE",
+    out_dir=None,
+    box_threshold=0.25,
+    text_threshold=0.25,
+    cmap="viridis",
+    opacity=0.5,
+    **kwargs,
+):
     """Display the SAM Map GUI.
 
     Args:
         sam (SamGeo):
         basemap (str, optional): The basemap to use. Defaults to "SATELLITE".
         out_dir (str, optional): The output directory. Defaults to None.
 
@@ -2321,47 +2328,47 @@
         layout=widgets.Layout(width=widget_width, padding=padding),
     )
 
     box_slider = widgets.FloatSlider(
         description="Box threshold:",
         min=0,
         max=1,
-        value=0.25,
+        value=box_threshold,
         step=0.01,
         readout=True,
         continuous_update=True,
         layout=widgets.Layout(width=widget_width, padding=padding),
         style=style,
     )
 
     text_slider = widgets.FloatSlider(
         description="Text threshold:",
         min=0,
         max=1,
         step=0.01,
-        value=0.25,
+        value=text_threshold,
         readout=True,
         continuous_update=True,
         layout=widgets.Layout(width=widget_width, padding=padding),
         style=style,
     )
 
     cmap_dropdown = widgets.Dropdown(
         description="Palette:",
         options=cm.list_colormaps(),
-        value="viridis",
+        value=cmap,
         style=style,
         layout=widgets.Layout(width=widget_width, padding=padding),
     )
 
     opacity_slider = widgets.FloatSlider(
         description="Opacity:",
         min=0,
         max=1,
-        value=0.5,
+        value=opacity,
         readout=True,
         continuous_update=True,
         layout=widgets.Layout(width=widget_width, padding=padding),
         style=style,
     )
 
     def opacity_changed(change):
@@ -2575,16 +2582,16 @@
 
     def reset_button_click(change):
         if change["new"]:
             segment_button.value = False
             save_button.value = False
             reset_button.value = False
             opacity_slider.value = 0.5
-            box_slider.value = 0.5
-            text_slider.value = 0.5
+            box_slider.value = 0.25
+            text_slider.value = 0.25
             cmap_dropdown.value = "viridis"
             text_prompt.value = ""
             output.clear_output()
             try:
                 if hasattr(m, "layer_name") and m.find_layer(m.layer_name) is not None:
                     m.remove_layer(m.find_layer(m.layer_name))
                 m.clear_drawings()
@@ -2625,7 +2632,164 @@
 
     if crs is not None:
         result.to_crs(crs, inplace=True)
     if output is not None:
         result.to_file(output, **kwargs)
     else:
         return result
+
+
+def split_raster(filename, out_dir, tile_size=256, overlap=0):
+    """Split a raster into tiles.
+
+    Args:
+        filename (str): The path or http URL to the raster file.
+        out_dir (str): The path to the output directory.
+        tile_size (int | tuple, optional): The size of the tiles. Can be an integer or a tuple of (width, height). Defaults to 256.
+        overlap (int, optional): The number of pixels to overlap between tiles. Defaults to 0.
+
+    Raises:
+        ImportError: Raised if GDAL is not installed.
+    """
+
+    try:
+        from osgeo import gdal
+    except ImportError:
+        raise ImportError(
+            "GDAL is required to use this function. Install it with `conda install gdal -c conda-forge`"
+        )
+
+    if isinstance(filename, str):
+        if filename.startswith("http"):
+            output = filename.split("/")[-1]
+            download_file(filename, output)
+            filename = output
+
+    # Open the input GeoTIFF file
+    ds = gdal.Open(filename)
+
+    if not os.path.exists(out_dir):
+        os.makedirs(out_dir)
+
+    if isinstance(tile_size, int):
+        tile_width = tile_size
+        tile_height = tile_size
+    elif isinstance(tile_size, tuple):
+        tile_width = tile_size[0]
+        tile_height = tile_size[1]
+
+    # Get the size of the input raster
+    width = ds.RasterXSize
+    height = ds.RasterYSize
+
+    # Calculate the number of tiles needed in both directions, taking into account the overlap
+    num_tiles_x = (width - overlap) // (tile_width - overlap) + int(
+        (width - overlap) % (tile_width - overlap) > 0
+    )
+    num_tiles_y = (height - overlap) // (tile_height - overlap) + int(
+        (height - overlap) % (tile_height - overlap) > 0
+    )
+
+    # Get the georeferencing information of the input raster
+    geotransform = ds.GetGeoTransform()
+
+    # Loop over all the tiles
+    for i in range(num_tiles_x):
+        for j in range(num_tiles_y):
+            # Calculate the pixel coordinates of the tile, taking into account the overlap and clamping to the edge of the raster
+            x_min = i * (tile_width - overlap)
+            y_min = j * (tile_height - overlap)
+            x_max = min(x_min + tile_width, width)
+            y_max = min(y_min + tile_height, height)
+
+            # Adjust the size of the last tile in each row and column to include any remaining pixels
+            if i == num_tiles_x - 1:
+                x_min = max(x_max - tile_width, 0)
+            if j == num_tiles_y - 1:
+                y_min = max(y_max - tile_height, 0)
+
+            # Calculate the size of the tile, taking into account the overlap
+            tile_width = x_max - x_min
+            tile_height = y_max - y_min
+
+            # Set the output file name
+            output_file = f"{out_dir}/tile_{i}_{j}.tif"
+
+            # Create a new dataset for the tile
+            driver = gdal.GetDriverByName("GTiff")
+            tile_ds = driver.Create(
+                output_file,
+                tile_width,
+                tile_height,
+                ds.RasterCount,
+                ds.GetRasterBand(1).DataType,
+            )
+
+            # Calculate the georeferencing information for the output tile
+            tile_geotransform = (
+                geotransform[0] + x_min * geotransform[1],
+                geotransform[1],
+                0,
+                geotransform[3] + y_min * geotransform[5],
+                0,
+                geotransform[5],
+            )
+
+            # Set the geotransform and projection of the tile
+            tile_ds.SetGeoTransform(tile_geotransform)
+            tile_ds.SetProjection(ds.GetProjection())
+
+            # Read the data from the input raster band(s) and write it to the tile band(s)
+            for k in range(ds.RasterCount):
+                band = ds.GetRasterBand(k + 1)
+                tile_band = tile_ds.GetRasterBand(k + 1)
+                tile_data = band.ReadAsArray(x_min, y_min, tile_width, tile_height)
+                tile_band.WriteArray(tile_data)
+
+            # Close the tile dataset
+            tile_ds = None
+
+    # Close the input dataset
+    ds = None
+
+
+def merge_rasters(
+    input_dir,
+    output,
+    input_pattern="*.tif",
+    output_format="GTiff",
+    output_nodata=None,
+    output_options=["COMPRESS=DEFLATE"],
+):
+    """Merge a directory of rasters into a single raster.
+
+    Args:
+        input_dir (str): The path to the input directory.
+        output (str): The path to the output raster.
+        input_pattern (str, optional): The pattern to match the input files. Defaults to "*.tif".
+        output_format (str, optional): The output format. Defaults to "GTiff".
+        output_nodata (float, optional): The output nodata value. Defaults to None.
+        output_options (list, optional): A list of output options. Defaults to ["COMPRESS=DEFLATE"].
+
+    Raises:
+        ImportError: Raised if GDAL is not installed.
+    """
+
+    import glob
+
+    try:
+        from osgeo import gdal
+    except ImportError:
+        raise ImportError(
+            "GDAL is required to use this function. Install it with `conda install gdal -c conda-forge`"
+        )
+    # Get a list of all the input files
+    input_files = glob.glob(os.path.join(input_dir, input_pattern))
+
+    # Merge the input files into a single output file
+    gdal.Warp(
+        output,
+        input_files,
+        format=output_format,
+        dstNodata=output_nodata,
+        options=output_options,
+    )
```

### Comparing `segment-geospatial-0.8.2/samgeo/samgeo.py` & `segment-geospatial-0.8.3/samgeo/samgeo.py`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.8.2/samgeo/text_sam.py` & `segment-geospatial-0.8.3/samgeo/text_sam.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,19 +61,25 @@
         ckpt_config_filename (str): Name of the config file for the model in the repository.
         device (str): Device to load the model onto. Default is 'cpu'.
 
     Returns:
         torch.nn.Module: The loaded model.
     """
 
-    cache_config_file = hf_hub_download(repo_id=repo_id, filename=ckpt_config_filename, force_filename=ckpt_config_filename)
+    cache_config_file = hf_hub_download(
+        repo_id=repo_id,
+        filename=ckpt_config_filename,
+        force_filename=ckpt_config_filename,
+    )
     args = SLConfig.fromfile(cache_config_file)
     model = build_model(args)
     model.to(device)
-    cache_file = hf_hub_download(repo_id=repo_id, filename=filename, force_filename=filename)
+    cache_file = hf_hub_download(
+        repo_id=repo_id, filename=filename, force_filename=filename
+    )
     checkpoint = torch.load(cache_file, map_location="cpu")
     model.load_state_dict(clean_state_dict(checkpoint["model"]), strict=False)
     model.eval()
     return model
 
 
 def transform_image(image: Image) -> torch.Tensor:
@@ -311,14 +317,78 @@
         self.phrases = phrases
         self.logits = logits
         self.prediction = mask_overlay
 
         if return_results:
             return masks, boxes, phrases, logits
 
+    def predict_batch(
+        self,
+        images,
+        out_dir,
+        text_prompt,
+        box_threshold,
+        text_threshold,
+        mask_multiplier=255,
+        dtype=np.uint8,
+        save_args={},
+        merge=True,
+        verbose=True,
+        **kwargs,
+    ):
+        """
+        Run both GroundingDINO and SAM model prediction for a batch of images.
+
+        Parameters:
+            images (list): List of input PIL Images.
+            out_dir (str): Output directory for the prediction.
+            text_prompt (str): Text prompt for the model.
+            box_threshold (float): Box threshold for the prediction.
+            text_threshold (float): Text threshold for the prediction.
+            mask_multiplier (int, optional): Mask multiplier for the prediction. Defaults to 255.
+            dtype (np.dtype, optional): Data type for the prediction. Defaults to np.uint8.
+            save_args (dict, optional): Save arguments for the prediction. Defaults to {}.
+            merge (bool, optional): Whether to merge the predictions into a single GeoTIFF file. Defaults to True.
+        """
+
+        import glob
+
+        if not os.path.exists(out_dir):
+            os.makedirs(out_dir)
+
+        if isinstance(images, str):
+            images = list(glob.glob(os.path.join(images, "*.tif")))
+            images.sort()
+
+        if not isinstance(images, list):
+            raise ValueError("images must be a list or a directory to GeoTIFF files.")
+
+        for i, image in enumerate(images):
+            basename = os.path.splitext(os.path.basename(image))[0]
+            if verbose:
+                print(f"Processing image {str(i+1).zfill(len(str(len(images))))} of {len(images)}: {image}...")
+            output = os.path.join(out_dir, f"{basename}_mask.tif")
+            self.predict(
+                image,
+                text_prompt,
+                box_threshold,
+                text_threshold,
+                output=output,
+                mask_multiplier=mask_multiplier,
+                dtype=dtype,
+                save_args=save_args,
+                **kwargs,
+            )
+
+        if merge:
+            output = os.path.join(out_dir, "merged.tif")
+            merge_rasters(out_dir, output)
+            if verbose:
+                print(f"Saved the merged prediction to {output}.")
+
     def show_anns(
         self,
         figsize=(12, 10),
         axis="off",
         cmap="viridis",
         alpha=0.4,
         add_boxes=True,
```

### Comparing `segment-geospatial-0.8.2/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.8.3/segment_geospatial.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.8.2
+Version: 0.8.3
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -58,15 +58,17 @@
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
 -   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
 -   [Segmenting imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
+-   [Batch segmentation with text prompts](https://samgeo.gishub.org/examples/text_prompts_batch)
 -   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/arcgis)
+-   [Segmenting swimming pools with text prompts](https://samgeo.gishub.org/examples/swimming_pools)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
 
@@ -105,14 +107,14 @@
 
 ## Computing Resources
 
 The Segment Anything Model is computationally intensive, and a powerful GPU is recommended to process large datasets. It is recommended to have a GPU with at least 8 GB of GPU memory. You can utilize the free GPU resources provided by Google Colab. Alternatively, you can apply for [AWS Cloud Credit for Research](https://aws.amazon.com/government-education/research-and-technical-computing/cloud-credit-for-research), which offers cloud credits to support academic research. If you are in the Greater China region, apply for the AWS Cloud Credit [here](https://aws.amazon.com/cn/events/educate_cloud/research-credits).
 
 ## Acknowledgements
 
-This package was made possible by the following open source projects. Credit goes to the developers of these projects.
+This project is supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
 -   [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO)
 -   [lang-segment-anything](https://github.com/luca-medeiros/lang-segment-anything)
```

### Comparing `segment-geospatial-0.8.2/setup.py` & `segment-geospatial-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords="samgeo",
     name="segment-geospatial",
     packages=find_packages(include=["samgeo", "samgeo.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/opengeos/segment-geospatial",
-    version='0.8.2',
+    version='0.8.3',
     zip_safe=False,
 )
```

