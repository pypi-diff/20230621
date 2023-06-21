# Comparing `tmp/simplegeomap-0.0.32.tar.gz` & `tmp/simplegeomap-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simplegeomap-0.0.32.tar", last modified: Mon Jun 19 20:20:20 2023, max compression
+gzip compressed data, was "dist/simplegeomap-0.0.33.tar", last modified: Wed Jun 21 11:08:01 2023, max compression
```

## Comparing `simplegeomap-0.0.32.tar` & `simplegeomap-0.0.33.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-19 20:20:20.000000 simplegeomap-0.0.32/
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-19 20:20:20.000000 simplegeomap-0.0.32/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.32/README.md
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-19 20:20:20.000000 simplegeomap-0.0.32/simplegeomap.egg-info/
--rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-06-19 20:20:20.000000 simplegeomap-0.0.32/simplegeomap.egg-info/dependency_links.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-19 20:20:20.000000 simplegeomap-0.0.32/simplegeomap.egg-info/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-06-19 20:20:20.000000 simplegeomap-0.0.32/simplegeomap.egg-info/top_level.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)       45 2023-06-19 20:20:20.000000 simplegeomap-0.0.32/simplegeomap.egg-info/requires.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-06-19 20:20:20.000000 simplegeomap-0.0.32/simplegeomap.egg-info/SOURCES.txt
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-19 20:20:20.000000 simplegeomap-0.0.32/simplegeomap/
--rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.32/simplegeomap/__init__.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     6689 2023-06-19 19:41:34.000000 simplegeomap-0.0.32/simplegeomap/simplegeomap.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     7585 2023-06-19 19:42:56.000000 simplegeomap-0.0.32/simplegeomap/util.py
--rw-rw-r--   0 burak     (1000) burak     (1000)      618 2023-06-19 10:24:43.000000 simplegeomap-0.0.32/setup.py
--rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-06-19 20:20:20.000000 simplegeomap-0.0.32/setup.cfg
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-21 11:08:01.000000 simplegeomap-0.0.33/
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-21 11:08:01.000000 simplegeomap-0.0.33/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.33/README.md
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-21 11:08:01.000000 simplegeomap-0.0.33/simplegeomap.egg-info/
+-rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-06-21 11:08:00.000000 simplegeomap-0.0.33/simplegeomap.egg-info/dependency_links.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-21 11:08:00.000000 simplegeomap-0.0.33/simplegeomap.egg-info/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-06-21 11:08:00.000000 simplegeomap-0.0.33/simplegeomap.egg-info/top_level.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)       45 2023-06-21 11:08:00.000000 simplegeomap-0.0.33/simplegeomap.egg-info/requires.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-06-21 11:08:00.000000 simplegeomap-0.0.33/simplegeomap.egg-info/SOURCES.txt
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-21 11:08:01.000000 simplegeomap-0.0.33/simplegeomap/
+-rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.33/simplegeomap/__init__.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     7137 2023-06-21 11:03:52.000000 simplegeomap-0.0.33/simplegeomap/simplegeomap.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     7598 2023-06-21 10:06:04.000000 simplegeomap-0.0.33/simplegeomap/util.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)      618 2023-06-21 08:57:01.000000 simplegeomap-0.0.33/setup.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-06-21 11:08:01.000000 simplegeomap-0.0.33/setup.cfg
```

### Comparing `simplegeomap-0.0.32/PKG-INFO` & `simplegeomap-0.0.33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.32
+Version: 0.0.33
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.32/README.md` & `simplegeomap-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.32/simplegeomap.egg-info/PKG-INFO` & `simplegeomap-0.0.33/simplegeomap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.32
+Version: 0.0.33
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.32/simplegeomap/simplegeomap.py` & `simplegeomap-0.0.33/simplegeomap/simplegeomap.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,46 +86,60 @@
             if len(x[0]) > len_thres:
                 arr = np.array(x[0])
                 if fill:
                    ax.fill(arr[:,0],arr[:,1],incolor,alpha=0.5)
                 else:
                    ax.plot(arr[:,0],arr[:,1],incolor)
                 
-def create_grid(clat,clon,dist,N):
-    p1 = LatLon(clat,clon)
-    EARTH_RAD = 6371
-    upright = p1.destination (dist, bearing=45, radius=EARTH_RAD)
-    lowleft = p1.destination (dist, bearing=225, radius=EARTH_RAD)
-    latmin = np.min([lowleft.lat, upright.lat])
-    latmax = np.max([lowleft.lat, upright.lat])
-    lonmin = np.min([lowleft.lon, upright.lon])
-    lonmax = np.max([lowleft.lon, upright.lon])
-    x = np.linspace(lonmin,lonmax,N)
-    y = np.linspace(latmin,latmax,N)
-    xx,yy =  np.meshgrid(x,y)
-    latints = np.unique(y.astype(int))
-    print (latints)
-    lonints = np.unique(x.astype(int))
-    return xx,yy,latints,lonints
-
-def plot_elevation(clat,clon,zoom,levels=None,ax=None):
+def plot_elevation(clat,clon,zoom,levels=None,lleft=None,uright=None,ax=None):
     if not ax: fig, ax = plt.subplots()    
     tkeys = np.array(list(gltiles.keys()))
     CENTER_DIST = 2000 * zoom
     print ('dist',CENTER_DIST)
-    newx,newy,latints,lonints = create_grid(clat,clon,CENTER_DIST,20)
+
+    if not lleft:
+        p1 = LatLon(clat,clon)
+        EARTH_RAD = 6371
+        upright = p1.destination (CENTER_DIST, bearing=45, radius=EARTH_RAD)
+        lowleft = p1.destination (CENTER_DIST, bearing=225, radius=EARTH_RAD)
+        latmin = np.min([lowleft.lat, upright.lat])
+        latmax = np.max([lowleft.lat, upright.lat])
+        lonmin = np.min([lowleft.lon, upright.lon])
+        lonmax = np.max([lowleft.lon, upright.lon])
+    else:
+        latmin = np.min([lleft[0],uright[0]])
+        latmax = np.max([lleft[0],uright[0]])
+        lonmin = np.min([lleft[1],uright[1]])
+        lonmax = np.max([lleft[1],uright[1]])
+
+    N = 15
+    x = np.linspace(lonmin,lonmax,N)
+    y = np.linspace(latmin,latmax,N)
+    newx,newy =  np.meshgrid(x,y)
+    latints = np.unique(y.astype(int))
+    lonints = np.unique(x.astype(int))
+    
     skip = len(latints)
     tile = tkeys[find_tile(clat,clon)]    
-    q = get_quad(tuple(latints),tuple(lonints),tile,skip=skip)
+    q = get_quad(tuple(latints),tuple(lonints),tile)
     interp = np.vectorize(q.interpolate,otypes=[np.float64])
     newz = interp(newx,newy)
     newz[newz<0] = 0
     #newz = conv2d(padding(newz),initialize_kernel((3,3),1))    
     CS=plt.contour(newx,newy,newz,cmap=plt.cm.binary,levels=levels)
     plt.clabel(CS, fontsize=10, inline=1)
+
+def elev_at(clat,clon):    
+    clats = [int(clat)-1, int(clat), int(clat)+1]
+    clons = [int(clon)-1, int(clon), int(clon)+1]
+    tkeys = np.array(list(gltiles.keys()))
+    tile = tkeys[find_tile(clat,clon)]    
+    q = get_quad(tuple(clats),tuple(clons),tile)
+    res = q.interpolate(clon,clat)
+    return res
     
 def plot_line(regarr,ax,color='black',linestyle='solid'):
     ax.plot(regarr[:,1],regarr[:,0],color=color,linestyle=linestyle)
        
 def plot_region(regarr,ax,color='lightgray',alpha=0.5):
     ax.fill(regarr[:,1],regarr[:,0],color=color,alpha=alpha)
```

### Comparing `simplegeomap-0.0.32/simplegeomap/util.py` & `simplegeomap-0.0.33/simplegeomap/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                 per = np.round(perimeterOf(latlons, radius=6371),2)
                 mid = meanOf(latlons)
                 res.append([mid.lat,mid.lon,per,type,geo])
 
     df = pd.DataFrame(res)
     df.columns = ['lat','lon','perimeter','type','polygon']
     df.to_csv('/tmp/lake_river.csv',index=None)
-
+    
 def initialize_kernel(size , sigma): 
     w, h = size                                                  
     x = np.linspace(-1,1,w)                         
     y = np.linspace(-1,1, h)                         
     x_cor, y_cor  = np.meshgrid(x, y) 
     kernel = 1/(2*np.pi*np.power(sigma,2) )*\
              np.exp((- (x_cor ** 2 + y_cor ** 2) )/ 
@@ -115,16 +115,18 @@
     return np.einsum('ij,ijkl->kl', ftr, sub_image)
     
 def cdist(p1,p2):    
     distances = np.linalg.norm(p1 - p2, axis=1)
     return distances
 
 class QuadTreeInterpolator:
-    def __init__(self, x, y, z):
-        self.tree = quads.QuadTree((np.mean(x), np.mean(y)), np.std(x)*10, np.std(y)*10)
+    def __init__(self):
+        self.tree = quads.QuadTree((0,0), 500, 500)
+
+    def append(self, x, y, z):        
         for xx,yy,zz in zip(x,y,z):
             self.tree.insert((xx,yy),data=zz)
 
     def interp_cell(self, x, y, points):
         a = np.array([x,y]).reshape(-1,2)
         b = np.array(points)[:,:2]
         ds = cdist(a,b)
@@ -140,53 +142,55 @@
         return self.interp_cell(x, y, points)
 
 def find_tile(lat,lon):
     res = [lat >= x[0] and lon < x[1] and lon >= x[2] and lon < x[3] for x in gltiles.values()]
     return res.index(True)
 
 @cached(cache=FIFOCache(maxsize=4))
-def get_quad(clats,clons,tile,skip,data_dir=None):
+def get_quad(clats,clons,tile,data_dir=None):
 
     if not data_dir: data_dir = os.path.dirname(__file__)
     print ('data_dir',data_dir)
     npz_file = data_dir + "/" + tile + ".npz"
     if os.path.exists(npz_file) == False:
         s = "Required data file for tile %s not found, place the required npz file under %s, see https://github.com/burakbayramli/simplegeomap/blob/main/elevation.md for details" % (tile,data_dir)
         raise ValueError(s)
     zm = np.load(npz_file)
     zm = zm['arr_0']
     clats = list(clats)
     clons = list(clons)
     print ('clat clons',clats,clons)
+    skip = np.min([len(clats),len(clons)])
     lat_min, lat_max, lon_min, lon_max, elev_min, elev_max, cols, rows = gltiles[tile]    
     lon = lon_min + 1/120*np.arange(cols)
     lat = lat_max - 1/120*np.arange(rows)
-    d = [[x,y,zm[i,j]] for i,y in enumerate(lat) for j,x in enumerate(lon) if i%skip == 0 and j%skip==0 and int(y) in clats and int(x) in clons]
+    d = [[x,y,zm[i,j]] for i,y in enumerate(lat) for j,x in enumerate(lon) if j%skip==0 and int(y) in clats and int(x) in clons]
     d = np.array(d)
     print ('d',d.shape)
-    q = QuadTreeInterpolator(d[:,0],d[:,1],d[:,2])
+    q = QuadTreeInterpolator()
+    q.append(d[:,0],d[:,1],d[:,2])
     return q
-        
+
 def test1():
     x = np.array(list(range(4,10)))
     y = np.array(list(range(10,16)))
     z = np.array(list(range(20,26)))
     q = QuadTreeInterpolator(x,y,z)
     for x in q.tree.nearest_neighbors((15,20), count=4):
         print (x)    
 
 def test2():
-    q = get_quad(tuple([40]),tuple([30]),'g10g',skip=1,data_dir=".")
+    q = get_quad(tuple([40]),tuple([30]),'g10g',data_dir=".")
     res = q.interpolate(30.5,40.5)
     print (res)
     res = q.interpolate(30.1,40.1)
     print (res)    
 
 def test3():
-    q = get_quad(tuple([-29]),tuple([151]),'l10g',skip=1,data_dir=".")
+    q = get_quad(tuple([-29]),tuple([151]),'l10g',data_dir=".")
     print (q.interpolate(151.20361804339458,-29.35574897873761))
                    
 if __name__ == "__main__": 
     
     #preprocess_GSHHS()
     #preprocess_GLOBE()
     test1()
```

### Comparing `simplegeomap-0.0.32/setup.py` & `simplegeomap-0.0.33/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 readme=open("README.md").read()
 
 setuptools.setup(
     name='simplegeomap',    
-    version='0.0.32',
+    version='0.0.33',
     description="Simple offline map plot utility, for country borders, elevation, water",
     long_description=readme,
     long_description_content_type="text/markdown",    
     install_requires=['pandas','pygeodesy','matplotlib','numpy','pyshp','zarr'],
     include_package_data=True,
     url="https://github.com/burakbayramli/simplegeomap",
     author="Burak Bayramli",
```

