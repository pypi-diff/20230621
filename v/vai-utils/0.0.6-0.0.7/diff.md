# Comparing `tmp/vai_utils-0.0.6.tar.gz` & `tmp/vai_utils-0.0.7.tar.gz`

## Comparing `vai_utils-0.0.6.tar` & `vai_utils-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 vai_utils-0.0.6/requirements.txt
--rw-r--r--   0        0        0    47189 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/0.07147342294341652.png
--rw-r--r--   0        0        0    33753 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/0.10837279097800767.png
--rw-r--r--   0        0        0    18545 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/0.5082194061656471.png
--rw-r--r--   0        0        0    42225 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/0.5284006170869843.png
--rw-r--r--   0        0        0    40716 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/0.6682099640762634.png
--rw-r--r--   0        0        0    43577 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/0.6929515496940593.png
--rw-r--r--   0        0        0    42433 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/0.701794926485459.png
--rw-r--r--   0        0        0    40716 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/0.9143838183319077.png
--rw-r--r--   0        0        0    47189 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/0.9859292536666209.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/__init__.py
--rw-r--r--   0        0        0    23562 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/plot.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 vai_utils-0.0.6/src/vai_utils/vai.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 vai_utils-0.0.6/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 vai_utils-0.0.6/LICENSE
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 vai_utils-0.0.6/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 vai_utils-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 vai_utils-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vai_utils-0.0.7/requirements.txt
+-rw-r--r--   0        0        0    13897 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.06565430985926124.png
+-rw-r--r--   0        0        0    47189 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.07147342294341652.png
+-rw-r--r--   0        0        0    33753 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.10837279097800767.png
+-rw-r--r--   0        0        0    15973 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.14226826635823298.png
+-rw-r--r--   0        0        0    14047 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.2966477897710217.png
+-rw-r--r--   0        0        0    18545 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.5082194061656471.png
+-rw-r--r--   0        0        0    42225 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.5284006170869843.png
+-rw-r--r--   0        0        0    40716 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.6682099640762634.png
+-rw-r--r--   0        0        0    43577 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.6929515496940593.png
+-rw-r--r--   0        0        0    42433 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.701794926485459.png
+-rw-r--r--   0        0        0    40716 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.9143838183319077.png
+-rw-r--r--   0        0        0    47189 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/0.9859292536666209.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/__init__.py
+-rw-r--r--   0        0        0    32765 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/plot.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 vai_utils-0.0.7/src/vai_utils/vai.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 vai_utils-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 vai_utils-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 vai_utils-0.0.7/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 vai_utils-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 vai_utils-0.0.7/PKG-INFO
```

### Comparing `vai_utils-0.0.6/src/vai_utils/0.07147342294341652.png` & `vai_utils-0.0.7/src/vai_utils/0.07147342294341652.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/src/vai_utils/0.10837279097800767.png` & `vai_utils-0.0.7/src/vai_utils/0.10837279097800767.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/src/vai_utils/0.5082194061656471.png` & `vai_utils-0.0.7/src/vai_utils/0.5082194061656471.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/src/vai_utils/0.5284006170869843.png` & `vai_utils-0.0.7/src/vai_utils/0.5284006170869843.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/src/vai_utils/0.6682099640762634.png` & `vai_utils-0.0.7/src/vai_utils/0.6682099640762634.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/src/vai_utils/0.6929515496940593.png` & `vai_utils-0.0.7/src/vai_utils/0.6929515496940593.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/src/vai_utils/0.701794926485459.png` & `vai_utils-0.0.7/src/vai_utils/0.701794926485459.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/src/vai_utils/0.9143838183319077.png` & `vai_utils-0.0.7/src/vai_utils/0.9143838183319077.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/src/vai_utils/0.9859292536666209.png` & `vai_utils-0.0.7/src/vai_utils/0.9859292536666209.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/src/vai_utils/plot.py` & `vai_utils-0.0.7/src/vai_utils/plot.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from matplotlib.colors import ListedColormap
 from PIL import Image
 import random
 import seaborn as sns
 import numpy as np
 from scipy.interpolate import interp1d
 import matplotlib.ticker as ticker
+import squarify
 
 colors =["#1D2026","#393939","#666666","#BDBDBD","#E0E0E0","#F2F2F2","#FD93B1","#FC2964","#FEC9D8","#FD5F8B","#0095FF","#E6F5FF","#5C33F6","#8566F8",]
 
 def bar_chart( categories, series, **optional_params):
     fig, ax = plt.subplots()
     bar_labels =[]
     if('bar_labels' in optional_params):
@@ -186,35 +187,15 @@
     name = random.random()
     plt.savefig(str(name) + '.png')
     im = Image.open(str(name) + '.png') 
     print("Image saved: ", str(name) + '.png')
     im.show()        
   
 
-# def waterfall_graph(categories,values ,   **optional_params):
-#     fig, ax = plt.subplots()
-#     cumulative_values = [sum(values[:i+1]) for i in range(len(values))]
-#     color = colors[0]
-#     if ('color' in optional_params):
-#         color =(optional_params['color'])
-#     plt.bar(categories, values, color=color, align='center', width=0.5)
-#     plt.plot(categories, cumulative_values, marker='o', color=color, linestyle='--')
-#     if ('xlabel' in optional_params):
-#         ax.set_xlabel(optional_params['xlabel'])
-#     if ('ylabel' in optional_params):
-#         ax.set_ylabel(optional_params['ylabel'])
-#     if ('title' in optional_params):
-#         ax.set_title(optional_params['title'])
-#     if ('legend' in optional_params):
-#         ax.legend(title=optional_params['legend'])
-#     name = random.random()
-#     plt.savefig(str(name) + '.png')
-#     im = Image.open(str(name) + '.png') 
-#     print("Image saved: ", str(name) + '.png')
-#     im.show()        
+  
 
   
 def dot_graph(categories, data,**optional_params):
     fig, ax = plt.subplots() 
     color = colors[0]
     data = data
     data = list(map(lambda a, i: {'index': i, 'value': a}, data, range(len(data))))
@@ -248,94 +229,94 @@
     if 'title' in optional_params:
         ax.set_title(optional_params['title'])
     cumulative_sum = [sum(values[:i+1]) for i in range(len(values))]
     bars = ax.bar(categories, values, align='center', alpha=0.5)  
     ax.set_xlabel('Categories') 
     ax.set_ylabel('Value') 
     ax.set_title('Waterfall Chart')  
-    ax.grid(True)
+
     ax.axhline(0, color='black', linewidth=0.8) 
     ax.set_xticklabels(categories, rotation=45) 
+    ax.grid(axis='y', linestyle='--', alpha=1) 
     for bar, value in zip(bars, values):
         if value < 0:
             bar.set_color('red')
         else:
-            bar.set_color(random.choice(colors))  # Random color selection
+            bar.set_color('#0095FF') 
 
     name = str(random.random())
     plt.savefig(name + '.png')
     im = Image.open(name + '.png') 
     print("Image saved:", name + '.png')
     im.show()  
 
 
 # categories = ['W1', 'W3', 'W5', 'W7', 'W9', 'W10']
 # values = [10, 5, 4, -4, -5, -10]
 # title = 'Secondary text'
-# colors = ["#1D2026", "#393939", "#666666"]
 # waterfall_graph(categories, values, title=title)
 
 
-def baseline_graph(baseline, x_labels,colors, *series_data):
+def baseline_graph(baseline, x_labels, series_colors, *series_data):
     fig, ax = plt.subplots()
-    
+
     for i, series in enumerate(series_data):
         percentage_change_series = [(value - baseline[j]) / baseline[j] * 100 for j, value in enumerate(series)]
-        ax.plot(x_labels, percentage_change_series, label=f'Product {i+1}', marker='o', color=random.choice(colors))
-
+        color = series_colors[i % len(series_colors)]  
+        ax.plot(x_labels, percentage_change_series, label=f'Product {i+1}', marker='o', color=color)
+    
+    ax.axhline(y=0, color='black', linestyle='dotted')
+    ax.grid(True)
     ax.set_title('Chg. from Baseline')
-    ax.legend()
+    ax.legend(bbox_to_anchor=(1, 0.9))
+    
     name = str(random.random())
-    plt.savefig(name + '.png')
+    plt.savefig(name + '.png', bbox_inches='tight')
     im = Image.open(name + '.png')
     print("Image saved:", name + '.png')
     im.show()
 
 # baseline = [10, 12, 14, 16, 18]
 # series1 = [11, 15, 12, 13, 20]
 # series2 = [9, 11, 13, 15, 17]
 # series3 = [13, 14, 10, 12, 11]
 # x_labels = ['W1', 'W3', 'W5', 'W7', 'W9']
-# colors = ["#FC2964","#0095FF","#5C33F6"]
-# baseline_graph(baseline, x_labels,colors, series1, series2, series3)
+# colors = ["#FC2964", "#0095FF", "#5C33F6"]
+# baseline_graph(baseline, x_labels, colors, series1, series2, series3)
 
 
 def scatter_plot_graph(marker_shapes, x_values, series_data, colors):
     np.random.seed(19680801)
-    sizes = np.random.rand(len(x_values[0])) * 100 + 100
+    sizes = np.random.rand(len(x_values[0])) * 50 + 50
 
     fig, ax = plt.subplots()
 
     for i, marker in enumerate(marker_shapes):
         x = x_values[i]
         y = series_data[i]
-        color = colors[i % len(colors)]  # Cycle through the available colors
+        color = colors[i % len(colors)]
         ax.scatter(x, y, s=sizes, alpha=0.5, marker=marker, color=color, label="Group {}".format(i+1))
-
     ax.set_title('Scatter Plot')
     ax.set_xlabel("Title")
     ax.set_ylabel("Title")
-    ax.legend()
-
-    name = random.random()
-    plt.savefig(str(name) + '.png')
-    im = Image.open(str(name) + '.png')
-    print("Image saved: ", str(name) + '.png')
+    ax.legend(bbox_to_anchor=(1, 0.9))
+    name = str(random.random())
+    plt.savefig(name + '.png', bbox_inches='tight')
+    im = Image.open(name + '.png')
+    print("Image saved:", name + '.png')
     im.show()
 
 # marker_shapes = ['s', 'o', 'D']
 # x_values = [np.arange(0.15, 50.0, 2.0), np.arange(0.15, 50.0, 2.0), np.arange(0.15, 50.0, 2.0)]
 # series_data = [
 #     x_values[0] ** 1.3 + np.random.rand(*x_values[0].shape) * 30.0,
 #     x_values[1] ** 1.5 + np.random.rand(*x_values[1].shape) * 40.0,
 #     x_values[2] ** 1.2 + np.random.rand(*x_values[2].shape) * 20.0
 # ]
-
-# colors = ["#FC2964","#0095FF","#5C33F6"]
-
+# colors = ["#FC2964", "#0095FF", "#5C33F6"]
 # scatter_plot_graph(marker_shapes, x_values, series_data, colors)
 
 
 def stacked_bar(categories, below, above,**optional_params):
     species = categories
     weight_counts = {
         "Below": np.array(below),
@@ -343,40 +324,38 @@
     }
     width = 0.5
 
     fig, ax = plt.subplots()
     bottom = np.zeros(len(categories))
 
     index= 0
-    color=["#0095FF","#1D2026"]
-
+    color=["#FC2964","#0095FF"]
     if ('color' in optional_params):
         color= (optional_params['color'])
-    
-    print('BOTTOM: ',bottom)
-
     for boolean, weight_count in weight_counts.items():
         p = ax.bar(species, weight_count, width, color = color[index], label=boolean, bottom=bottom)
         index = index+1
         bottom += weight_count
 
     if ('xlabel' in optional_params):
         ax.set_xlabel(optional_params['xlabel'])
     if ('ylabel' in optional_params):
         ax.set_ylabel(optional_params['ylabel'])
     if ('title' in optional_params):
         ax.set_title(optional_params['title'])
     if ('legend' in optional_params):
-        ax.legend(loc='upper left',title=optional_params['legend'],bbox_to_anchor= (0.0, 1.010), ncol = 2)
+        ax.legend(loc='lower center',title=optional_params['legend'],bbox_to_anchor= (0.50, -0.25), ncol = 2)
         
+    fig.tight_layout()
     name = random.random()
     plt.savefig(str(name) + '.png')
     im = Image.open(str(name) + '.png') 
     print("Image saved: ", str(name) + '.png')
     im.show() 
+    # plt.show()
 
 # categories = ('2010','2012','2014','2016','2018','2020')
 # below=[30,35,40,45,50,55]
 # above=[70,70,45,50,55,60]
 # title = 'Stacked bar chart'
 # ylabel='Title'
 # legend='legends'
@@ -439,28 +418,33 @@
 # x_axis_data = [2007, 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2017, 2019, 2021, 2023]
 # colors = ["#1D2026", "#393939", "#666666", "#BDBDBD", "#E0E0E0", "#F2F2F2", "#FD93B1",
 #           "#FC2964", "#FEC9D8", "#FD5F8B", "#0095FF", "#E6F5FF", "#5C33F6", "#8566F8"]
 # heatmap2_graph(y_axis_data, x_axis_data, colors,title,dataFrom,dataTo)
 
 def boxPlot_graph(data, titles, colors,xAxisTitle,yAxisTitle):
     fig, ax = plt.subplots()
-    box_plot = ax.boxplot(data, patch_artist=True)
-    for patch, color in zip(box_plot['boxes'], colors):
-        patch.set_facecolor(color)
-        patch.set_linewidth(1)  # Set the linewidth for solid color style
-    ax.set_xticklabels(titles)
+    ranges = [np.max(dataset) - np.min(dataset) for dataset in data]
+    sorted_data = sorted(zip(data, ranges, titles, colors), key=lambda x: x[1], reverse=True)
+    sorted_values, sorted_ranges, sorted_titles, sorted_colors = zip(*sorted_data)
+    box_plot = ax.boxplot(sorted_values, patch_artist=True)
+
+    for patch, color in zip(box_plot['boxes'], sorted_colors):
+        patch.set(facecolor=color, linewidth=1)
+
+    ax.set_xticklabels(sorted_titles)
     ax.legend().remove()
     ax.set_ylabel(yAxisTitle, fontsize=12)
     ax.set_xlabel(xAxisTitle, fontsize=12)
     plt.title('Box Plot')
     name = random.random()
     plt.savefig(str(name) + '.png')
     im = Image.open(str(name) + '.png') 
     print("Image saved: ", str(name) + '.png')
     im.show()
+    # plt.show()
 
 # data = [[25, 26, 27, 28, 29],
 #         [20, 21, 22, 23, 24],
 #         [10, 12, 14, 16, 18],
 #         [10, 15, 20, 25, 30],
 #         [20, 23, 26, 29, 32],
 #         [22, 26, 29, 33, 36]]
@@ -470,28 +454,33 @@
 # titles = ['Group 1', 'Group 2', 'Group 3', 'Group 4', 'Group 5', 'Group 6']
 # xAxisTitle='Title'
 # yAxisTitle='Title'
 # boxPlot_graph(data, titles, colors,xAxisTitle,yAxisTitle)
 
 def boxPlot2_graph(data, titles, colors, xAxisTitle, yAxisTitle):
     fig, ax = plt.subplots()
-    box_plot = ax.boxplot(data, patch_artist=True)
-    for patch, color in zip(box_plot['boxes'], colors):
-        patch.set(facecolor=color, alpha=0.5, edgecolor=color)
-        patch.set_linewidth(1)  
-    ax.set_xticklabels(titles)
+    ranges = [np.max(dataset) - np.min(dataset) for dataset in data]
+    sorted_data = sorted(zip(data, ranges, titles, colors), key=lambda x: x[1], reverse=True)
+    sorted_values, sorted_ranges, sorted_titles, sorted_colors = zip(*sorted_data)
+    box_plot = ax.boxplot(sorted_values, patch_artist=True)
+
+    for patch, color in zip(box_plot['boxes'], sorted_colors):
+        patch.set(facecolor=color, alpha=0.5, edgecolor=color, linewidth=1)
+
+    ax.set_xticklabels(sorted_titles)
     ax.legend().remove()
     ax.set_ylabel(yAxisTitle, fontsize=12)
     ax.set_xlabel(xAxisTitle, fontsize=12)
     plt.title('Box Plot')
     name = random.random()
     plt.savefig(str(name) + '.png')
     im = Image.open(str(name) + '.png') 
     print("Image saved: ", str(name) + '.png')
     im.show()
+    # plt.show()
 
 # data = [[25, 26, 27, 28, 29],
 #         [20, 21, 22, 23, 24],
 #         [10, 12, 14, 16, 18],
 #         [10, 15, 20, 25, 30],
 #         [20, 23, 26, 29, 32],
 #         [22, 26, 29, 33, 36]]
@@ -499,115 +488,362 @@
 # colors = ["#FEC9D8","#FD5F8B","#0095FF","#1D2026","#5C33F6","#8566F8"]
 # titles = ['Group 1', 'Group 2', 'Group 3', 'Group 4', 'Group 5', 'Group 6']
 # xAxisTitle = 'Title'
 # yAxisTitle = 'Title'
 # boxPlot2_graph(data, titles, colors, xAxisTitle, yAxisTitle)
 
 
-
-def boxPlot3_graph(data, colors,title, xAxisTitle, yAxisTitle):
-    fig, ax = plt.subplots()
+def boxPlot3_graph(data, colors, title, xAxisTitle, yAxisTitle):
+    fig, ax = plt.subplots(figsize=(10, 6))  # Adjust the figure size as needed
     box_plots = ax.boxplot(data, patch_artist=True, vert=True, widths=0.5)
     for patch, color in zip(box_plots['boxes'], colors[:len(data)]):
         patch.set_facecolor(color)
         patch.set_edgecolor('black')
+    
     legend_handles = [plt.Rectangle((0, 0), 1, 1, color=color) for color in colors[:len(data)]]
     legend_labels = [f'{i+1}' for i in range(len(data))]
-    ax.legend(legend_handles, legend_labels, loc='upper right')
+    
+    legend = ax.legend(legend_handles, legend_labels, loc='upper right', bbox_to_anchor=(1.1, 1))
+    legend.set_title("Legend")
+    
+    for line, handle in zip(legend.get_lines(), legend.get_patches()):
+        line.set_linestyle('-')
+        line.set_linewidth(1.0)
+        line.set_color('black')
+        handle.set_visible(False)
+    
     ax.set_title(title)
     ax.set_xlabel(xAxisTitle)
     ax.set_ylabel(yAxisTitle)
-    name = random.random()
-    plt.savefig(str(name) + '.png')
-    im = Image.open(str(name) + '.png') 
-    print("Image saved: ", str(name) + '.png')
+    
+    name = str(random.random())
+    plt.savefig(name + '.png', bbox_inches='tight')  # Use bbox_inches='tight' to include the legend
+    im = Image.open(name + '.png')
+    print("Image saved:", name + '.png')
     im.show()
 
-
-# title="Box Plot"
-# xAxisTitle="Legend"
-# yAxisTitle="Title"
-# title="Box Plot"
+# title = "Box Plot"
+# xAxisTitle = "Legend"
+# yAxisTitle = "Title"
 # colors = ["#1D2026", "#393939", "#666666", "#BDBDBD", "#E0E0E0", "#F2F2F2",
 #           "#FD93B1", "#FC2964", "#FEC9D8"]
-# data = [[25, 26, 27, 28, 29],
-#         [20, 25, 29, 33, 35],
-#         [20, 21, 22, 23, 24],
-#         [10, 12, 14, 16, 18],
-#         [10, 15, 20, 25, 30],
-#         [20, 23, 26, 29, 32],
-#         [22, 26, 29, 33, 36],
-#         [22, 26, 29, 33, 36],
-#         [20, 21, 22, 23, 24],
-#         [20, 23, 26, 29, 32],
-#         [22, 26, 29, 33, 36]]
-# boxPlot3_graph(data, colors,title, xAxisTitle, yAxisTitle)
+# data=[[10, 15, 20, 25, 30],
+#       [20, 25, 29, 33, 35],
+#       [22, 26, 29, 33, 36],
+#       [22, 26, 29, 33, 36],
+#       [22, 26, 29, 33, 36],
+#       [20, 23, 26, 29, 32],
+#       [20, 23, 26, 29, 32],
+#       [10, 12, 14, 16, 18],
+#       [20, 21, 22, 23, 24],
+#       [20, 21, 22, 23, 24],
+#       [25, 26, 27, 28, 29],
+#       [20, 21, 22, 23, 24]
+#       ]
+        
+# boxPlot3_graph(data, colors, title, xAxisTitle, yAxisTitle)
 
 
 
 def next_item_predictions(categories, values, **optional_params):
     fig, ax = plt.subplots()
     categories = [c for c, v in zip(categories, values) if v is not None]
     values = [v for v in values if v is not None]
     if 'title' in optional_params:
         ax.set_title(optional_params['title'])
-    cumulative_sum = [sum(values[:i + 1]) for i in range(len(values))]
-    
-    colors = [ "#FC2964", "#5C33F6"]
     
     bars = ax.barh(categories, values, align='center', alpha=0.5)
     ax.set_xlabel('Value')
     ax.set_ylabel('Categories')
-    ax.set_title('Next Item Predications')
-    ax.grid(True)
+    ax.set_title('Next Item Predictions')
+    ax.spines['top'].set_visible(False)  
+    ax.spines['right'].set_visible(False)  
+    ax.grid(axis='x', linestyle='--', alpha=1) 
     ax.axvline(0, color='black', linewidth=0.8)
     ax.set_yticklabels(categories)
     
     for bar, value in zip(bars, values):
         if value < 0:
             bar.set_color('red')
         else:
-            bar.set_color('blue')
+            bar.set_color('#0095FF')
     
     name = str(random.random())
     plt.savefig(name + '.png')
     im = Image.open(name + '.png')
     print("Image saved:", name + '.png')
     im.show()
 
 
 # categories = ['Burger', 'Pizza', 'sandwitch', 'pasta', 'momos', 'garlic']
-# values = [10, 5, 4, -4, -5, -10]
+# values = [ -10, -5, -4,4, 5, 10]
 # title = 'Secondary text'
 
 # next_item_predictions(categories, values, title=title)
 
 
 
+
 def table_count(xAxisvalue, predicatedLine, actualLine):
     x = np.arange(len(xAxisvalue))
     x_smooth = np.linspace(0, len(xAxisvalue) - 1, 100)
     f_actual = interp1d(x, actualLine, kind='cubic')
     f_predicted = interp1d(x, predicatedLine, kind='cubic')
     actualLine_smooth = f_actual(x_smooth)
     predicatedLine_smooth = f_predicted(x_smooth)
-    fig, ax = plt.subplots(figsize=(16, 9))  # Set maximum size
-    
+    fig, ax = plt.subplots(figsize=(16, 9)) 
+    ax.grid(True, linestyle='--', alpha=1)
     ax.plot(x_smooth, actualLine_smooth, color="#FC2964", label='Actual')
     ax.plot(x_smooth, predicatedLine_smooth, color="#5C33F6", label='Predicted')
     ax.set_xlabel('Time')
     ax.set_ylabel('Value')
     ax.set_title('Table Count')
-    ax.legend()
-    ax.xaxis.set_major_locator(ticker.IndexLocator(base=1, offset=0))
+    ax.legend(bbox_to_anchor=(1.02, 1))
+    ax.xaxis.set_major_locator(plt.IndexLocator(base=1, offset=0))
     ax.set_xticklabels(xAxisvalue)
-    
     name = str(random.random())
-    plt.savefig(name + '.png', dpi=300)  # Set higher dpi for better image quality
+    plt.savefig(name + '.png', dpi=300) 
     im = Image.open(name + '.png')
     print("Image saved:", name + '.png')
     im.show()
 
 # xAxisvalue = ['8:00 PM', '9:00 PM', '10:00 PM', '12:00 PM', '1:00 AM', '3:00 AM', '3:00 AM', '4:00 AM', '5:00 AM','3:00 AM', '3:00 AM', '4:00 AM', '5:00 AM']
-# predicatedLine = [30,30, 33, 28,34,29, 33, 28,34,29,28,33,32]
-# actualLine = [30,30,29, 33,32,29,29, 33,32,29,30,31,37]
+# predicatedLine = [30, 30, 33, 28, 34, 29, 33, 28, 34, 29, 28, 33, 32]
+# actualLine = [30, 30, 29, 33, 32, 29, 29, 33, 32, 29, 30, 31, 37]
 # table_count(xAxisvalue, predicatedLine, actualLine)
+
+
+
+def dot_plot(categories,data,**optional_params):
+    fig, ax = plt.subplots()
+    ax.set_aspect('equal')
+    ax.scatter(np.arange(len(categories)), data, s=100, c='#8566F8', alpha=0.7)
+    ax.set_xticks(np.arange(len(categories)))
+    ax.set_xticklabels(categories)
+    # ax.set_ylabel('Values')
+    ax.set_title('Dots Horizontal Scale')
+    name = random.random()
+    plt.savefig(str(name) + '.png')
+    im = Image.open(str(name) + '.png') 
+    print("Image saved: ", str(name) + '.png')
+    im.show()  
+
+
+# categories = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16]
+# values = ['Option 1','Option 2','Option 3','Option 4','Option 5','Option 6','Option 7','Option 8','Option 9','Option 10','Option 11','Option 12','Option 13','Option 14','Option 15','Option 16']
+# dot_plot(categories,values)
+
+def dot_plot_grouped(categories, data, **optional_params):
+    fig, ax = plt.subplots()
+    ax.set_aspect('equal')
+
+    colors = ["#FD93B1", "#FC2964", "#8566F8", "#5C33F6", "#E0E0E0", "#F2F2F2","#FD93B1", "#FC2964", "#FEC9D8"]
+
+    grouped_categories = [categories[i:i+4] for i in range(0, len(categories), 4)]
+    group_count = len(grouped_categories)
+    # group_positions = np.arange(group_count) * 1
+    
+    index=0
+    for i, group_cats in enumerate(grouped_categories):
+        ax.scatter(group_cats, data[i*4:(i+1)*4], s=100, c=colors[index], alpha=0.7)
+        index=index+1
+
+    ax.set_xticks(np.arange(len(categories)))
+    ax.set_xticklabels(categories)
+    ax.set_yticks(np.arange(len(categories)))
+    y_labels = ax.set_yticklabels(data)
+
+    for i, label in enumerate(y_labels):
+        if i < 4:
+            label.set_color("#FD93B1")
+        elif i < 8:
+            label.set_color("#FC2964")
+        elif i < 12:
+            label.set_color("#8566F8")
+        else:
+            label.set_color("#5C33F6")
+
+    # ax.set_ylabel('Group')
+    # ax.set_xlabel('Categories')
+    ax.set_title('Grouped Dots Horizontal Scale')
+    ax.legend(np.arange(group_count)+1,title='legend',loc='lower center', bbox_to_anchor=(0.5, -0.3), ncol = 4)
+
+    name = random.random()
+    plt.savefig(str(name) + '.png')
+    im = Image.open(str(name) + '.png')
+    print("Image saved: ", str(name) + '.png')
+    im.show()
+    plt.close()
+    # plt.show()
+
+# categories = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16]
+# values = ['Option 1', 'Option 2', 'Option 3', 'Option 4', 'Option 5', 'Option 6', 'Option 7', 'Option 8',
+#           'Option 9', 'Option 10', 'Option 11', 'Option 12', 'Option 13', 'Option 14', 'Option 15', 'Option 16']
+
+# dot_plot_grouped(categories, values)
+
+
+def scatter_plot_with_dotted_line(data,**optional_params):
+    fig, ax = plt.subplots() 
+    shapes = ["o", "v", "^", ".", ",", "<", ">", "1", "2", "3", "4", "8", "s", "p"]
+    color = ["#8566F8","#8566F8","#666666","#BDBDBD","#FD93B1","#FEC9D8","#393939"]
+
+    index=0
+    for y in data:
+        res = random.sample(range(1, len(y)+1), len(y))
+        ax.scatter(res, y,color=color[index],marker=shapes[index])
+        index=index+1
+
+    if ('xlabel' in optional_params):
+        ax.set_xlabel(optional_params['xlabel'])
+    if ('ylabel' in optional_params):
+        ax.set_ylabel(optional_params['ylabel'])
+    if ('title' in optional_params):
+        ax.set_title(optional_params['title'])
+    if ('handles' in optional_params):
+        ax.legend(handles=optional_params['handles'],ncol = 1 ,loc='upper left', bbox_to_anchor= (0.0, 1.010))
+        
+    ax.axhline(y = (len(data)*len(data[0]))/2, color = '#FC2964', linestyle = ':')
+    name = random.random()
+    plt.savefig(str(name) + '.png')
+    im = Image.open(str(name) + '.png') 
+    print("Image saved: ", str(name) + '.png')
+    im.show()
+    # plt.show()
+
+# data=[[2,4,6,8,10,3,6,9,12,15,5,8,11,13,17,7,14,17,16,19,21,23,18,19,31,25,27,24,26,30,32,41,33,25,35,41,]]
+# title = 'Scatter plot'
+# xlabel='Title'
+# ylabel='Title'
+# handles=['Group 1']
+# scatter_plot_with_dotted_line(data,handles=handles,title=title,xlabel=xlabel,ylabel=ylabel)
+
+def scatter_plot_with_line(data,**optional_params):
+    fig, ax = plt.subplots() 
+    shapes = ["o", "v", "^", ".", ",", "<", ">", "1", "2", "3", "4", "8", "s", "p"]
+    color = ["#8566F8","#8566F8","#666666","#BDBDBD","#FD93B1","#FEC9D8","#393939"]
+    # x =  categories
+    index=0
+    for y in data:
+        res = random.sample(range(1, len(y)+1), len(y))
+        print('RES:',res)
+        ax.scatter(res, y,color=color[index],marker=shapes[index])
+        index=index+1
+
+    if ('xlabel' in optional_params):
+        ax.set_xlabel(optional_params['xlabel'])
+    if ('ylabel' in optional_params):
+        ax.set_ylabel(optional_params['ylabel'])
+    if ('title' in optional_params):
+        ax.set_title(optional_params['title'])
+    if ('handles' in optional_params):
+        ax.legend(handles=optional_params('handles'),ncol = 1 ,loc='upper left', bbox_to_anchor= (0.0, 1.010))
+    x1=np.array([1,(len(data)*len(data[0]))-1])
+    y1=np.array([1,(len(data)*len(data[0]))-1])
+    ax.plot(x1,y1,label='line',color = '#FC2964')
+
+    name = random.random()
+    plt.savefig(str(name) + '.png')
+    im = Image.open(str(name) + '.png') 
+    print("Image saved: ", str(name) + '.png')
+    im.show()
+    # plt.show()
+
+# data=[[2,4,6,8,10,3,6,9,12,15,5,8,11,13,17,7,14,17,16,19,21,23,18,19,31,25,27,24,26,30,32,41,33,25,35,41,]]
+# title = 'Scatter plot'
+# xlabel='Title'
+# ylabel='Title'
+# handles=['Group 1']
+# scatter_plot_with_line(data,handles=handles,title=title,xlabel=xlabel,ylabel=ylabel)
+
+def treeMap(data,colors,title):
+    labels = [item for sublist in data for item in sublist]
+    sizes = [1] * len(labels)
+    fig = plt.figure(figsize=(8, 6))
+    ax = fig.add_subplot(111)
+    plt.title(title)
+    squarify.plot(sizes=sizes, label=labels, color=colors, alpha=0.7, ax=ax)
+    plt.axis('off')
+    name = random.random()
+    plt.savefig(str(name) + '.png')
+    im = Image.open(str(name) + '.png') 
+    print("Image saved: ", str(name) + '.png')
+    im.show()
+
+# data = [["property", "property", "property"],
+#         ["property", "property", "property"],
+#         ["property", "property"],
+#         ["property"]]
+# colors = ['#5C33F6', '#FEC9D8', '#BDBDBD']
+# title="Tree Map"
+# treeMap(data,colors,title)
+
+def forest_plot_graph(yAxisdata, xAxisdata, effect_sizes, color,confidence_intervals):
+    plt.figure(figsize=(6, 4))
+    for i in range(len(yAxisdata)):
+        if i < len(confidence_intervals):
+            plt.plot([confidence_intervals[i][0], confidence_intervals[i][1]], [i, i], color=color)
+            center = (confidence_intervals[i][0] + confidence_intervals[i][1]) / 2
+            plt.scatter(center, i, color=color, zorder=10)
+    x_vals = np.full(len(effect_sizes), np.nan)  # Create an array of NaN values
+    y_vals = np.arange(len(effect_sizes))
+    plt.scatter(effect_sizes, y_vals[:len(effect_sizes)], color=color, zorder=10)
+    plt.yticks(range(len(yAxisdata)), yAxisdata)
+    plt.xticks(xAxisdata)
+    plt.xlim(min(xAxisdata), max(xAxisdata))
+    plt.title('Forest Plot')
+    plt.xlabel('Title')
+    plt.ylabel('Title')
+    name = random.random()
+    plt.savefig(str(name) + '.png')
+    im = Image.open(str(name) + '.png') 
+    print("Image saved: ", str(name) + '.png')
+    im.show()
+
+# yAxisdata = [10, 20, 30, 40, 50, 60, 70]
+# xAxisdata = [10, 20, 30, 40, 50, 60, 70, 80]
+# effect_sizes = [13, 20, 30, 40, 50]
+# confidence_intervals = [(10, 20), (20, 30), (30, 40), (40, 50), (50, 60)]
+# color="#5C33F6"
+# forest_plot_graph(yAxisdata, xAxisdata, effect_sizes,color, confidence_intervals)
+
+
+# def box_plot(data,**optional_params):
+#     fig, ax = plt.subplots() 
+#     colors = ['#8566F8','#E6F5FF']
+#     length_of_data = len(data)
+
+#     boxplot = ax.boxplot(data, vert=True, patch_artist=True)
+#     ax.grid(color=colors[1])
+#     boxplot['whiskers'][0].set(color=colors[0])
+#     boxplot['whiskers'][1].set(color=colors[0])
+#     boxplot['caps'][0].set(color=colors[0])
+#     boxplot['caps'][1].set(color=colors[0])
+#     ax.set_xticklabels(np.arange(length_of_data))
+
+#     for box in boxplot['boxes']:
+#         box.set_facecolor(colors[0])
+#         box.set_edgecolor(colors[0])
+
+#     # for whisker in boxplot['whiskers']:
+#     #     whisker.set_linestyle('') 
+
+#     if('y_label' in optional_params):
+#         ax.set_ylabel(optional_params['y_label'])
+#     if('x_label' in optional_params):
+#         ax.set_xlabel(optional_params['x_label'])
+#     if('title' in optional_params):
+#         ax.set_title(optional_params['title'])
+    
+#     name = random.random()
+#     plt.savefig(str(name) + '.png')
+#     im = Image.open(str(name) + '.png') 
+#     print("Image saved: ", str(name) + '.png')
+#     im.show()
+#     plt.show()
+
+# data=[[25, 30],[20, 27],[22, 27],[25, 28],[19, 28],[25, 40],[30, 40],[38, 50],[40, 47],[40, 50],[38, 55]]
+# title = 'Box plots'
+# x_label='Title'
+# y_label='Title'
+
+# box_plot(data,title=title,x_label=x_label,y_label=y_label)
```

### Comparing `vai_utils-0.0.6/src/vai_utils/vai.py` & `vai_utils-0.0.7/src/vai_utils/vai.py`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/.gitignore` & `vai_utils-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/LICENSE` & `vai_utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/README.md` & `vai_utils-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.6/pyproject.toml` & `vai_utils-0.0.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vai_utils"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="VirtuousAI", email="info@virtuousai.com" },
 ]
 dynamic = ["dependencies"]
 description = "VAI utils"
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `vai_utils-0.0.6/PKG-INFO` & `vai_utils-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vai_utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: VAI utils
 Author-email: VirtuousAI <info@virtuousai.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

