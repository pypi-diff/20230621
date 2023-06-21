# Comparing `tmp/EASYPLOT_TOOLBOX-2023.4.tar.gz` & `tmp/EASYPLOT_TOOLBOX-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EASYPLOT_TOOLBOX-2023.4.tar", last modified: Fri Apr 14 12:06:10 2023, max compression
+gzip compressed data, was "EASYPLOT_TOOLBOX-2023.5.tar", last modified: Wed Jun 21 18:11:43 2023, max compression
```

## Comparing `EASYPLOT_TOOLBOX-2023.4.tar` & `EASYPLOT_TOOLBOX-2023.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 mateus    (1000) mateus    (1000)        0 2023-04-14 12:06:10.755847 EASYPLOT_TOOLBOX-2023.4/
-drwxrwxr-x   0 mateus    (1000) mateus    (1000)        0 2023-04-14 12:06:10.751847 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX/
--rw-rw-r--   0 mateus    (1000) mateus    (1000)    13335 2023-04-13 15:49:20.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX/EASYPLOT.py
--rw-rw-r--   0 mateus    (1000) mateus    (1000)       23 2023-04-13 15:05:35.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX/__init__.py
-drwxrwxr-x   0 mateus    (1000) mateus    (1000)        0 2023-04-14 12:06:10.755847 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/
--rw-rw-r--   0 mateus    (1000) mateus    (1000)      426 2023-04-14 12:06:10.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/PKG-INFO
--rw-rw-r--   0 mateus    (1000) mateus    (1000)      265 2023-04-14 12:06:10.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/SOURCES.txt
--rw-rw-r--   0 mateus    (1000) mateus    (1000)        1 2023-04-14 12:06:10.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/dependency_links.txt
--rw-rw-r--   0 mateus    (1000) mateus    (1000)       19 2023-04-14 12:06:10.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/requires.txt
--rw-rw-r--   0 mateus    (1000) mateus    (1000)       17 2023-04-14 12:06:10.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/top_level.txt
--rw-rw-r--   0 mateus    (1000) mateus    (1000)      426 2023-04-14 12:06:10.755847 EASYPLOT_TOOLBOX-2023.4/PKG-INFO
--rw-rw-r--   0 mateus    (1000) mateus    (1000)       38 2023-04-14 12:06:10.755847 EASYPLOT_TOOLBOX-2023.4/setup.cfg
--rw-rw-r--   0 mateus    (1000) mateus    (1000)      913 2023-04-14 12:05:08.000000 EASYPLOT_TOOLBOX-2023.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:11:43.966195 EASYPLOT_TOOLBOX-2023.5/
+drwxrwxrwx   0        0        0        0 2023-06-21 18:11:43.936115 EASYPLOT_TOOLBOX-2023.5/EASYPLOT_TOOLBOX/
+-rw-rw-rw-   0        0        0    11401 2023-06-21 17:56:56.000000 EASYPLOT_TOOLBOX-2023.5/EASYPLOT_TOOLBOX/EASYPLOT.py
+-rw-rw-rw-   0        0        0       23 2023-02-18 15:01:30.000000 EASYPLOT_TOOLBOX-2023.5/EASYPLOT_TOOLBOX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:11:43.964197 EASYPLOT_TOOLBOX-2023.5/EASYPLOT_TOOLBOX.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-06-21 18:11:43.000000 EASYPLOT_TOOLBOX-2023.5/EASYPLOT_TOOLBOX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-06-21 18:11:43.000000 EASYPLOT_TOOLBOX-2023.5/EASYPLOT_TOOLBOX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 18:11:43.000000 EASYPLOT_TOOLBOX-2023.5/EASYPLOT_TOOLBOX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-21 18:11:43.000000 EASYPLOT_TOOLBOX-2023.5/EASYPLOT_TOOLBOX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-21 18:11:43.000000 EASYPLOT_TOOLBOX-2023.5/EASYPLOT_TOOLBOX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      434 2023-06-21 18:11:43.966195 EASYPLOT_TOOLBOX-2023.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11558 2022-09-07 16:11:09.000000 EASYPLOT_TOOLBOX-2023.5/license.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 18:11:43.967196 EASYPLOT_TOOLBOX-2023.5/setup.cfg
+-rw-rw-rw-   0        0        0      965 2023-06-21 18:10:24.000000 EASYPLOT_TOOLBOX-2023.5/setup.py
```

### Comparing `EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX/EASYPLOT.py` & `EASYPLOT_TOOLBOX-2023.5/EASYPLOT_TOOLBOX/EASYPLOT.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,352 +1,310 @@
-import matplotlib.pyplot as plt
-import seaborn as sns
-import numpy as np
-
-def CONVERT_SI_TO_INCHES(WIDTH, HEIGHT):
-    """ 
-    This function convert figure dimensions from meters to inches.
-    
-    Input:
-    WIDTH    |  Figure width in SI units       |         |  Float
-    HEIGHT   |  Figure height in SI units      |         |  Float
-    
-    Output:
-    WIDTH    |  Figure width in INCHES units   |         |  Float
-    HEIGHT   |  Figure height in INCHES units  |         |  Float
-    """
-    
-    # Converting dimensions
-    WIDTH /= 0.0254
-    HEIGHT /= 0.0254
-    
-    return WIDTH, HEIGHT
-
-def SAVE_GRAPHIC(NAME, EXT, DPI):
-    """ 
-    This function saves graphics according to the selected extension.
-
-    Input: 
-    NAME  | Path + name figure               |         |  String
-          |   NAME = 'svg'                   |         |  
-          |   NAME = 'png'                   |         |
-          |   NAME = 'eps'                   |         | 
-          |   NAME = 'pdf'                   |         |
-    EXT   | File extension                   |         |  String
-    DPI   | The resolution in dots per inch  |         |  Integer
-    
-    Output:
-    N/A
-    """
-    
-    plt.savefig(NAME + '.' + EXT, dpi = DPI, bbox_inches = 'tight', transparent = True)
-
-def HISTOGRAM_CHART(DATASET, PLOT_SETUP):
-    """
-    See documentation in: https://wmpjrufg.github.io/EASYPLOT_TOOLBOX/
-    """
-    
-    # Setup
-    NAME = PLOT_SETUP['NAME']
-    W = PLOT_SETUP['WIDTH']
-    H = PLOT_SETUP['HEIGHT']
-    X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
-    X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
-    Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']
-    Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
-    AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
-    LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
-    LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
-    CHART_COLOR = PLOT_SETUP['CHART COLOR']
-    BINS = int(PLOT_SETUP['BINS'])
-    KDE = PLOT_SETUP['KDE']
-    DPI = PLOT_SETUP['DPI']
-    EXT = PLOT_SETUP['EXTENSION']
-    
-    # Dataset and others information
-    AUX = DATASET['DATASET']
-    COLUMN = DATASET['COLUMN']
-    DATA = AUX[COLUMN]
-    
-    # Plot
-    [W, H] = CONVERT_SI_TO_INCHES(W, H)
-    sns.set(style = 'ticks')
-    FIG, (AX_BOX, AX_HIST) = plt.subplots(2, figsize = (W, H), sharex = True, gridspec_kw = {'height_ratios': (.15, .85)})
-    sns.boxplot(x=DATA, ax = AX_BOX, color = CHART_COLOR)
-    sns.histplot(DATA, ax = AX_HIST, kde = KDE, color = CHART_COLOR, bins = BINS)
-    AX_BOX.set(yticks = [])
-    AX_BOX.set(xlabel='')
-    font = {'fontname': 'DejaVu Sans',
-            'color':  LABELS_COLOR,
-            'weight': 'normal',
-            'size': LABELS_SIZE}
-    AX_HIST.set_xlabel(X_AXIS_LABEL, fontdict = font)
-    AX_HIST.set_ylabel(Y_AXIS_LABEL, fontdict = font)
-    AX_HIST.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
-    AX_HIST.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
-    plt.grid()
-    sns.despine(ax = AX_HIST)
-    sns.despine(ax = AX_BOX, left = True)
-    
-    # Save figure
-    SAVE_GRAPHIC(NAME, EXT, DPI)
-
-def LINE_CHART(DATASET, PLOT_SETUP):
-	"""
-    OF or FIT - Line chart
-
-    Input:  
-    DATASET     | META Optimization toolbox results                        | Py dictionary
-	            |  Dictionary tags                                         |
-				|    'X'     = Values NEOF or Iterations                   | Py  array[M_ITER + 1 x 1]
-	            |    'Y'  = Line value by iterations                       | Py  array[N_ITER + 1 x 1][M_ITER + 1 x 1]
-	            |    'LEGEND'  = Name of lines for the legend              | Py  array[N_ITER + 1 x 1]
-	            |    'COLORS'  = Color of the lines                        | Py  array[N_ITER + 1 x 1]
-    PLOT_SETUP  | Contains specifications of each model of chart           | Py Dictionary
-                |  Dictionary tags                                         |
-                |    'NAME'          == Filename output file               | String 
-                |    'WIDTH'         == Width figure                       | Float
-                |    'HEIGHT         == Height figure                      | Float
-                |    'EXTENSION'     == Extension output file              | String 
-                |    'DPI'           == Dots Per Inch - Image quality      | Integer   
-				|    'MARKER'        == Line marker                        | String
-				|    'MARKER SIZE'   == Marker size                        | Float
-				|    'LINE WIDTH'    == Line width                         | Float
-				|    'LINE STYLE'    == Line style                         | String
-                |    'Y AXIS LABEL'  == Y axis label name                  | String
-                |    'X AXIS LABEL'  == X axis label name                  | String
-				|    'LABELS COLOR'  == Labels color                       | String
-				|    'LABELS SIZE'   == Labels size                        | Float
-                |    'X AXIS SIZE'   == X axis size                        | Float
-                |    'Y AXIS SIZE'   == Y axis size                        | Float
-                |    'AXISES COLOR'  == Axis color                         | String
-                |    'GRID'          == Grid in chart                      | Boolean  
-				|    'Y LOG'         == Y axis logscale                    | Boolean 
-				|    'X LOG'         == X axis logscale                    | Boolean 
-				|    LOC LEGEND      == Legend location                    | String
-				|    SIZE LEGEND     == Legend size                        | Float
-    
-    Output:
-    The image is saved in the current directory 
-	"""
-	NAME = PLOT_SETUP['NAME']
-	W = PLOT_SETUP['WIDTH']
-	H = PLOT_SETUP['HEIGHT']
-	EXT = PLOT_SETUP['EXTENSION']
-	DPI = PLOT_SETUP['DPI']
-	MARKER = PLOT_SETUP['MARKER']
-	MARKER_SIZE = PLOT_SETUP['MARKER SIZE']
-	LINE_WIDTH = PLOT_SETUP['LINE WIDTH']
-	LINE_STYLE = PLOT_SETUP['LINE STYLE']
-	Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']
-	X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
-	LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
-	LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
-	X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
-	Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
-	AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
-	GRID = PLOT_SETUP['ON GRID?']
-	YLOGSCALE = PLOT_SETUP['Y LOG']
-	XLOGSCALE = PLOT_SETUP['X LOG']
-	LOC = PLOT_SETUP['LOC LEGEND']
-	SIZE_LEGEND = PLOT_SETUP['SIZE LEGEND']
-    
-	X = DATASET['X']
-	# The variable is a array with the data to be distributed in the graph.
-	DATA_Y = DATASET['Y']
-	# A list containing the name assigned to each line of the graph in the legend
-	LEGENDA = DATASET['LEGEND']
-	COLORS = DATASET['COLORS']
-	
-    # Convert units of size figure
-	W, H = CONVERT_SI_TO_INCHES(W, H)
-	
-	# Plot
-	FIG, AX= plt.subplots(1, 1, figsize = (W, H), sharex = True)
-	
-    # Go through each row of the array, where each row represents a line on the graph.
-	for k in range(len( DATA_Y)):
-		AX.plot(X, DATA_Y[k], marker = MARKER,color =COLORS[k], linestyle = LINE_STYLE, linewidth = LINE_WIDTH, markersize = MARKER_SIZE, label=LEGENDA[k])
-	if YLOGSCALE:
-		AX.semilogy()
-	if XLOGSCALE:
-		AX.semilogx()
-	font = {'fontname': 'Arial',
-			'color':  LABELS_COLOR,
-			'weight': 'normal',
-			'size': LABELS_SIZE}
-	AX.set_ylabel(Y_AXIS_LABEL, fontdict = font)
-	AX.set_xlabel(X_AXIS_LABEL, fontdict = font)   
-	AX.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
-	AX.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
-	if GRID == True:
-		AX.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
-	plt.legend(loc = LOC, prop = {'size': SIZE_LEGEND})
-	SAVE_GRAPHIC(NAME, EXT, DPI)
-
-def SCATTER_PLOT(DATASET, PLOT_SETUP):    
-
-    NAME = PLOT_SETUP['NAME']
-    W = PLOT_SETUP['WIDTH']
-    H = PLOT_SETUP['HEIGHT']
-    EXT = PLOT_SETUP['EXTENSION']
-    DPI = PLOT_SETUP['DPI']
-    MARKER = PLOT_SETUP['MARKER']
-    MARKER_SIZE = PLOT_SETUP['MARKER SIZE']
-    Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']
-    X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
-    LABELS_SIZE = PLOT_SETUP['LABELS SIZE']   
-    LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
-    X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
-    Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
-    AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
-    GRID = PLOT_SETUP['ON GRID?']
-    YLOGSCALE = PLOT_SETUP['Y LOG']
-    XLOGSCALE = PLOT_SETUP['X LOG']
-    LOC = PLOT_SETUP['LOC LEGEND']
-    SIZE_LEGEND = PLOT_SETUP['SIZE LEGEND']
-    SMOOTH_LINE = PLOT_SETUP['SMOOTH LINE']
-
-    X = DATASET['X']
-    
-    #The variable is an array with the data to be distributed in the graph.
-    DATA_Y = DATASET['Y']
-    
-    # A list containing the name assigned to each line of the graph in the legend.
-    LEGENDA = DATASET['LEGEND']
-    
-    #List with colors that must be used
-    COLORS = DATASET['COLORS']
-    
-    # Convert units of size figure
-    W, H = CONVERT_SI_TO_INCHES(W, H)
-    FIG, AX = plt.subplots(1, 1, figsize = (W, H), sharex = True)
-    
-    
-    # Go through each row of the array, where each row represents a line on the graph
-    for k in range(len( DATA_Y)):
-        plt.scatter(X, DATA_Y[k],marker = MARKER,c =COLORS[k] ,linewidths=MARKER_SIZE,label=LEGENDA[k])
-        
-    plt.title(NAME)
-    
-    # Trend line
-    if SMOOTH_LINE:
-        p = np.polyfit(X, DATA_Y, 1)
-        plt.plot(X, np.polyval(p, X), color='b')
-    
-    if YLOGSCALE:
-        AX.semilogy()
-    if XLOGSCALE:
-        AX.semilogx()
-    plt.xlabel(X_AXIS_LABEL, fontsize=X_AXIS_SIZE,color = LABELS_COLOR)
-    plt.ylabel(Y_AXIS_LABEL, fontsize=Y_AXIS_SIZE,color = LABELS_COLOR)
-    plt.tick_params(axis = 'x', labelsize = LABELS_SIZE, colors = AXISES_COLOR, labelrotation = 90, direction = 'out',which = 'both', length = 10)
-    plt.tick_params(axis = 'y', labelsize = LABELS_SIZE, colors = AXISES_COLOR)
-    if GRID == True:
-        AX.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
-    plt.legend(loc = LOC, prop = {'size': SIZE_LEGEND})
-    SAVE_GRAPHIC(NAME, EXT, DPI)
-    plt.show()
-
-def HEATMAP(DATASET,PLOT_SETUP):
-    NAME = PLOT_SETUP['NAME']
-    W = PLOT_SETUP['WIDTH']
-    H = PLOT_SETUP['HEIGHT']
-    EXT = PLOT_SETUP['EXTENSION']
-    DPI = PLOT_SETUP['DPI']
-    SQUARE = PLOT_SETUP['SQUARE']
-    ESCADA = PLOT_SETUP['MASK']
-    GRID = PLOT_SETUP['ON GRID?']
-    LINE_WIDTHS = PLOT_SETUP['LINE WIDTHS']
-    CMAP =  PLOT_SETUP['CMAP']
-    LINE_COLOR = PLOT_SETUP['LINE COLOR']
-    ANNOT =  PLOT_SETUP['ANNOT']
-    ANNOT_SIZE_FONT = PLOT_SETUP['ANNOT SIZE FONT']
-    ANNOT_FONT_WEIGHT = PLOT_SETUP['ANNOT FONT WEIGHT']
-
-    W, H = CONVERT_SI_TO_INCHES(W, H)
-
-
-    IRIS = DATASET['DATA']
-
-    # Create a correlation array
-    CORR = IRIS.corr()
-
-    #Check if the graph will be in the form of a ladder
-    if ESCADA:
-        #Remove the repeated values and those equal to 1
-        mask = np.tril(CORR)
-    else:
-        mask = None
-    
-    # Creating the ladder-shaped correlation plot
-    ax = sns.heatmap(CORR,center=0,linewidths= LINE_WIDTHS,xticklabels= True,
-                linecolor = LINE_COLOR ,annot=ANNOT, vmin=-1,vmax=1,
-                annot_kws={'fontsize':ANNOT_SIZE_FONT,'fontweight':ANNOT_FONT_WEIGHT},cmap=CMAP, square=SQUARE,mask = mask)
-    
-    #Invert the values of the y-axis and the graph becomes in the ladder-shaped form
-    plt.gca().invert_yaxis() 
-    
-    if GRID == True:
-        ax.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
-    
-    ax.tick_params(axis='y', rotation=0)
-    
-    SAVE_GRAPHIC(NAME, EXT, DPI)
-    
-    plt.show()
-
-def BAR_GRAPH(DATASET, PLOT_SETUP):
-    # Group the data by resistance class and calculate the average of EMA for each group
-    
-    # Plot a bar chart
-    NAME = PLOT_SETUP['NAME']
-    W = PLOT_SETUP['WIDTH']
-    H = PLOT_SETUP['HEIGHT']
-    EXT = PLOT_SETUP['EXTENSION']
-    DPI = PLOT_SETUP['DPI']
-    FONT = PLOT_SETUP['FONT']
-    Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']
-    X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
-    LABELS_SIZE = PLOT_SETUP['LABELS SIZE']   
-    LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
-    X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
-    Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
-    AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
-    GRID = PLOT_SETUP['ON GRID?']
-    YLOGSCALE = PLOT_SETUP['Y LOG']
-    XLOGSCALE = PLOT_SETUP['X LOG']
-    BAR_WIDTH = PLOT_SETUP['BAR WIDTH']
-    OPACITY = PLOT_SETUP['OPACITY']
-    
-    X = DATASET['X']
-    Y = DATASET['Y']
-    COLORS = DATASET['COLORS']
-   
-    [W, H] = CONVERT_SI_TO_INCHES(W, H)
-    fig, ax = plt.subplots(1, 1, figsize = (W, H))
-    error_config = {'ecolor': '0.3'}
-
-    for k in range(len(Y)):
-        ax.bar(X[k], Y[k], BAR_WIDTH, color=COLORS[k], error_kw=error_config,alpha = OPACITY)
-    
-    FONT = {
-            'fontname': FONT,
-            'color':  LABELS_COLOR,
-            'weight': 'normal',
-            'size': LABELS_SIZE
-        }
-    
-    ax.set_ylabel(Y_AXIS_LABEL, fontdict = FONT)
-    ax.set_xlabel(X_AXIS_LABEL, fontdict = FONT)
-    ax.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
-    ax.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
-    if YLOGSCALE:
-        ax.semilogy()
-    if XLOGSCALE:
-        ax.semilogx()
-    if GRID == True:
-        ax.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
-    
-    plt.tight_layout()
-    SAVE_GRAPHIC(NAME, EXT, DPI)
-    plt.show()
+import matplotlib.pyplot as plt
+import seaborn as sns
+
+def CONVERT_SI_TO_INCHES(WIDTH, HEIGHT):
+    """ 
+    This function convert figure dimensions from meters to inches.
+    
+    Input:
+    WIDTH    |  Figure width in SI units       |         |  Float
+    HEIGHT   |  Figure height in SI units      |         |  Float
+    
+    Output:
+    WIDTH    |  Figure width in INCHES units   |         |  Float
+    HEIGHT   |  Figure height in INCHES units  |         |  Float
+    """
+    
+    # Converting dimensions
+    WIDTH /= 0.0254
+    HEIGHT /= 0.0254
+    
+    return WIDTH, HEIGHT
+
+def SAVE_GRAPHIC(NAME, EXT, DPI):
+    """ 
+    This function saves graphics according to the selected extension.
+
+    Input: 
+    NAME  | Path + name figure               |         |  String
+          |   NAME = 'svg'                   |         |  
+          |   NAME = 'png'                   |         |
+          |   NAME = 'eps'                   |         | 
+          |   NAME = 'pdf'                   |         |
+    EXT   | File extension                   |         |  String
+    DPI   | The resolution in dots per inch  |         |  Integer
+    
+    Output:
+    N/A
+    """
+    
+    plt.savefig(NAME + '.' + EXT, dpi = DPI, bbox_inches = 'tight', transparent = True)
+
+def BARRA_GRAF(DATASET, PLOT_SETUP):
+    # Agrupar os dados por classe de resistência e calcular a média do EMA para cada grupo
+    
+    #mean_ema = grouped.apply(lambda x: np.mean(np.abs(x['fck_obs (MPa)'] - x['fck_pred (MPa)'])))
+    # Plotar o gráfico de barras
+    NAME = PLOT_SETUP['NAME']#
+    W = PLOT_SETUP['WIDTH']#
+    H = PLOT_SETUP['HEIGHT']#
+    EXT = PLOT_SETUP['EXTENSION']#
+    DPI = PLOT_SETUP['DPI']#
+    FONT = PLOT_SETUP['FONT']#
+    Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']#
+    X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']#
+    LABELS_SIZE = PLOT_SETUP['LABELS SIZE']  #   
+    LABELS_COLOR = PLOT_SETUP['LABELS COLOR']#
+    X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']#
+    Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']#
+    AXISES_COLOR = PLOT_SETUP['AXISES COLOR']#
+    GRID = PLOT_SETUP['ON GRID?']#
+    YLOGSCALE = PLOT_SETUP['Y LOG']#
+    XLOGSCALE = PLOT_SETUP['X LOG']#
+    BAR_WIDTH = PLOT_SETUP['BAR WIDTH']#
+    OPACITY = PLOT_SETUP['OPACITY']#
+    
+    X = DATASET['X']
+    Y = DATASET['Y']
+    COLORS = DATASET['COLORS']
+   
+    [W, H] = CONVERT_SI_TO_INCHES(W, H)
+    fig, ax = plt.subplots(1, 1, figsize = (W, H))
+    error_config = {'ecolor': '0.3'}
+    
+    for k in range(len(Y)):
+        ax.bar(X[k], Y[k], BAR_WIDTH, color=COLORS[k], error_kw=error_config,alpha = OPACITY)
+    FONT = {
+            'fontname': FONT,
+            'color':  LABELS_COLOR,
+            'weight': 'normal',
+            'size': LABELS_SIZE
+            }
+    ax.set_ylabel(Y_AXIS_LABEL, fontdict = FONT)
+    ax.set_xlabel(X_AXIS_LABEL, fontdict = FONT)
+    ax.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
+    ax.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
+    if YLOGSCALE:
+        ax.semilogy()
+    if XLOGSCALE:
+        ax.semilogx()
+    if GRID == True:
+        ax.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
+    plt.tight_layout()
+    #save figure
+    SAVE_GRAPHIC(NAME, EXT, DPI)
+
+def HISTOGRAM_CHART(DATASET, PLOT_SETUP):
+    """
+    See documentation in:https://wmpjrufg.github.io/EASYPLOT_TOOLBOX/002-HISTOGRAM.html
+    """
+    
+    # Setup
+    NAME = PLOT_SETUP['NAME']
+    W = PLOT_SETUP['WIDTH']
+    H = PLOT_SETUP['HEIGHT']
+    X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
+    X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
+    Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']
+    Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
+    AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
+    LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
+    LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
+    CHART_COLOR = PLOT_SETUP['CHART COLOR']
+    BINS = int(PLOT_SETUP['BINS'])
+    # KDE = PLOT_SETUP['KDE']
+    DPI = PLOT_SETUP['DPI']
+    EXT = PLOT_SETUP['EXTENSION']
+    
+    # Dataset and others information
+    DATA = DATASET['DATASET']
+    COLUMN = DATASET['COLUMN']
+ 
+    # Plot
+    [W, H] = CONVERT_SI_TO_INCHES(W, H)
+    sns.set(style = 'ticks')
+    FIG, (AX_BOX, AX_HIST) = plt.subplots(2, figsize = (W, H), sharex = True, gridspec_kw = {'height_ratios': (.15, .85)})
+    sns.boxplot(data = DATA, x = COLUMN, ax = AX_BOX, color = CHART_COLOR)
+    sns.histplot(data = DATA, x = COLUMN, ax = AX_HIST, color = CHART_COLOR, bins = BINS)
+    AX_BOX.set(yticks = [])
+    AX_BOX.set(xlabel = '')
+    FONT = {'fontname': 'DejaVu Sans',
+            'color':  LABELS_COLOR,
+            'weight': 'normal',
+            'size': LABELS_SIZE}
+    AX_HIST.set_xlabel(xlabel = X_AXIS_LABEL, fontdict = FONT)
+    AX_HIST.set_ylabel(ylabel = Y_AXIS_LABEL, fontdict = FONT)
+    AX_HIST.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
+    AX_HIST.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
+    plt.grid()
+    sns.despine(ax = AX_HIST)
+    sns.despine(ax = AX_BOX, left = True)
+    
+    # Save figure
+    SAVE_GRAPHIC(NAME, EXT, DPI)
+
+def LINE_CHART(DATASET, PLOT_SETUP):
+    """
+    See documentation in:https://wmpjrufg.github.io/EASYPLOT_TOOLBOX/002-LINE.html
+    """
+    
+    # Setup
+    NAME = PLOT_SETUP['NAME']
+    W = PLOT_SETUP['WIDTH']
+    H = PLOT_SETUP['HEIGHT']
+    EXT = PLOT_SETUP['EXTENSION']
+    DPI = PLOT_SETUP['DPI']
+    MARKER = PLOT_SETUP['MARKER']
+    MARKER_SIZE = PLOT_SETUP['MARKER SIZE']
+    LINE_WIDTH = PLOT_SETUP['LINE WIDTH']
+    LINE_STYLE = PLOT_SETUP['LINE STYLE']
+    Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']
+    X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
+    LABELS_SIZE = PLOT_SETUP['LABELS SIZE']     
+    LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
+    X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
+    Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
+    AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
+    COLORS = PLOT_SETUP['CHART COLOR']
+    GRID = PLOT_SETUP['ON GRID?']
+    YLOGSCALE = PLOT_SETUP['Y LOG']
+    XLOGSCALE = PLOT_SETUP['X LOG']
+    LOC = PLOT_SETUP['LOC LEGEND']
+    SIZE_LEGEND = PLOT_SETUP['SIZE LEGEND']
+    
+    # Dataset and others information
+    X = DATASET['X']
+    DATA_Y = DATASET['Y']
+    LEGEND = DATASET['LEGEND']
+    
+    # Plot
+    W, H = CONVERT_SI_TO_INCHES(W, H)
+    FIG, AX = plt.subplots(1, 1, figsize = (W, H), sharex = True)
+    for K, Y in enumerate(DATA_Y):
+        AX.plot(X, Y, marker = MARKER,  linestyle = LINE_STYLE[K], linewidth = LINE_WIDTH, markersize = MARKER_SIZE, label = LEGEND[K], color = COLORS[K])
+    if YLOGSCALE:
+        AX.semilogy()
+    if XLOGSCALE:
+        AX.semilogx()
+    font = {'fontname': 'DejaVu Sans',
+            'color':  LABELS_COLOR,
+            'weight': 'normal',
+            'size': LABELS_SIZE}
+    AX.set_ylabel(Y_AXIS_LABEL, fontdict = font)
+    AX.set_xlabel(X_AXIS_LABEL, fontdict = font)   
+    AX.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
+    AX.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
+    if GRID == True:
+        AX.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
+    plt.legend(loc = LOC, prop = {'size': SIZE_LEGEND})
+    
+    # Save figure
+    SAVE_GRAPHIC(NAME, EXT, DPI)
+
+def RADAR_CHART(DATASET, PLOT_SETUP):
+    
+    # Setup
+    NAME = PLOT_SETUP['NAME']
+    W = PLOT_SETUP['WIDTH']
+    H = PLOT_SETUP['HEIGHT']
+    X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
+    AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
+    LEGEND_SIZE = PLOT_SETUP['LEGEND SIZE']
+    LINE_WIDTH = PLOT_SETUP['LINE WIDTH']
+    GRID = PLOT_SETUP['ON GRID?']
+    DPI = PLOT_SETUP['DPI']
+    EXT = PLOT_SETUP['EXTENSION']
+    
+    #Dataset
+    CATEGORIAS = DATASET['CATEGORIAS']
+    VALORES = DATASET['VALORES']
+    CORES = DATASET['CORES']
+    LEGENDAS = DATASET['LEGENDA']
+
+    # Calcular os ângulos para cada categoria
+    num_categorias = len(CATEGORIAS)
+    angulos = np.linspace(0, 2 * np.pi, num_categorias, endpoint=False).tolist()
+
+
+    W, H = CONVERT_SI_TO_INCHES(W, H)
+    fig, AX = plt.subplots(1, 1, figsize=(W, H),subplot_kw={'projection': 'polar'})
+
+    legendas = []
+    for valor, cor, legenda in zip(VALORES, CORES, LEGENDAS):
+        # Plotar as linhas do gráfico de radar
+        linha, = AX.plot(angulos, valor, color=cor, linewidth=LINE_WIDTH, label=legenda)
+        # Preencher as áreas entre as linhas
+        AX.fill(angulos, valor, cor, alpha=0.25)
+        # Criar as legendas
+        legendas.append(Line2D([0], [0], color=cor, linewidth=LINE_WIDTH, label=legenda)) 
+    
+    # Configurar os rótulos das categorias
+    AX.set_xticks(angulos)
+    AX.set_xticklabels(CATEGORIAS,position=(-0.2, -0.05, 0.3))
+    AX.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR, labelrotation = 0, direction = 'out', which = 'both', length = 10)
+
+    # Configurar os limites dos eixos
+    AX.set_ylim(0, max(max(valores1), max(valores2)))
+
+    # Adicionar as legendas ao gráfico
+    legenda = AX.legend(handles=legendas, loc='upper right', bbox_to_anchor=(1.3, 1),fontsize=LEGEND_SIZE)
+
+    # Adicionar título
+    plt.title(NAME)
+
+    # Ajustar o layout para evitar sobreposição
+    plt.tight_layout()
+    
+    if GRID == True:
+        AX.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
+        
+    SAVE_GRAPHIC(NAME, EXT, DPI)
+
+def SCATTER_PLOT(DATASET, PLOT_SETUP):    
+    """
+    See documentation in:https://wmpjrufg.github.io/EASYPLOT_TOOLBOX/003-SCATTER.html
+    """
+
+    # Setup
+    NAME = PLOT_SETUP['NAME']
+    W = PLOT_SETUP['WIDTH']
+    H = PLOT_SETUP['HEIGHT']
+    MARKER_SIZE = PLOT_SETUP['MARKER SIZE']
+    CMAP = PLOT_SETUP['CMAP COLOR']
+    Y_AXIS_LABEL = PLOT_SETUP['Y AXIS LABEL']
+    Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
+    X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
+    X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
+    LABELS_SIZE = PLOT_SETUP['LABELS SIZE']  
+    LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
+    AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
+    GRID = PLOT_SETUP['ON GRID?']
+    YLOGSCALE = PLOT_SETUP['Y LOG']
+    XLOGSCALE = PLOT_SETUP['X LOG']
+    DPI = PLOT_SETUP['DPI']
+    EXT = PLOT_SETUP['EXTENSION']
+
+    # Data
+    X = DATASET['X']
+    Y = DATASET['Y']
+    Z = DATASET['Z']
+    
+    # Plot
+    W, H = CONVERT_SI_TO_INCHES(W, H)
+    FIG, AX = plt.subplots(1, 1, figsize = (W, H), sharex = True)
+    im = AX.scatter(X, Y, c = Z, marker = 'o', s = MARKER_SIZE , cmap = CMAP)
+    colorbar = plt.colorbar(im)
+    if YLOGSCALE:
+        AX.semilogy()
+    if XLOGSCALE:
+        AX.semilogx()
+    font = {'fontname': 'DejaVu Sans',
+            'color':  LABELS_COLOR,
+            'weight': 'normal',
+            'size': LABELS_SIZE}
+    AX.set_ylabel(Y_AXIS_LABEL, fontdict = font)
+    AX.set_xlabel(X_AXIS_LABEL, fontdict = font)   
+    AX.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR, labelrotation = 0, direction = 'out', which = 'both', length = 10)
+    AX.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
+    if GRID == True:
+        AX.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
+    SAVE_GRAPHIC(NAME, EXT, DPI)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EASYPLOT_TOOLBOX-2023.4/setup.py` & `EASYPLOT_TOOLBOX-2023.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from setuptools import setup
-
-setup(
-    	name = 'EASYPLOT_TOOLBOX',
-    	version = '2023.4',
-		url = 'https://wmpjrufg.github.io/EASYPLOT_TOOLBOX/',
-    	description= 'Ferramenta para plotagem rápida de gráficos',
-        keywords = ["Plot", "Data Science", "Optimezation"],
-		license = 'Apache License 2.0',
-        readme = 'readme.md',
-		authors = ['Wanderlei Malaquias Pereira Junior', 'Sergio Francisco da Silva', 'Nilson Jorge Leão Junior', 'Mateus Pereira da Silva'],
-		author_email = 'wanderlei_junior@ufcat.edu.br',
-    	maintainers = 'Wanderlei Malaquias Pereira Junior',
-		packages = ['EASYPLOT_TOOLBOX'],
-    	install_requires = ["matplotlib", "seaborn"],
-		classifiers=[
-    		'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
-			'Topic :: Software Development :: Build Tools',
-  		]
-    )
-
+from setuptools import setup
+
+setup(
+    	name = 'EASYPLOT_TOOLBOX',
+    	version = '2023.5',
+		url = 'https://wmpjrufg.github.io/EASYPLOT_TOOLBOX/',
+    	description= 'Ferramenta para plotagem rápida de gráficos',
+        keywords = ["Plot", "Data Science", "Optimezation"],
+		license = 'Apache License 2.0',
+        readme = 'readme.md',
+		authors = ['Wanderlei Malaquias Pereira Junior', 'Sergio Francisco da Silva', 'Nilson Jorge Leão Junior', 'Mateus Pereira da Silva'],
+		author_email = 'wanderlei_junior@ufcat.edu.br',
+    	maintainers = ['Wanderlei Malaquias Pereira Junior', 'Mateus Pereira da Silva'],
+		packages = ['EASYPLOT_TOOLBOX'],
+    	install_requires = ["matplotlib", "seaborn"],
+		classifiers = [
+    		'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+			'Topic :: Software Development :: Build Tools',
+  		]
+    )
+
```

