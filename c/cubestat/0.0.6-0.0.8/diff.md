# Comparing `tmp/cubestat-0.0.6.tar.gz` & `tmp/cubestat-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubestat-0.0.6.tar", last modified: Mon Jun 19 01:25:08 2023, max compression
+gzip compressed data, was "cubestat-0.0.8.tar", last modified: Wed Jun 21 01:52:58 2023, max compression
```

## Comparing `cubestat-0.0.6.tar` & `cubestat-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:25:08.401373 cubestat-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-19 01:24:58.000000 cubestat-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-19 01:25:08.397374 cubestat-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-19 01:24:58.000000 cubestat-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:25:08.397374 cubestat-0.0.6/cubestat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 01:24:58.000000 cubestat-0.0.6/cubestat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15236 2023-06-19 01:24:58.000000 cubestat-0.0.6/cubestat/cubestat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:25:08.397374 cubestat-0.0.6/cubestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 01:25:08.401373 cubestat-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 01:24:58.000000 cubestat-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:52:58.134715 cubestat-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-21 01:52:47.000000 cubestat-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 01:52:58.134715 cubestat-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-21 01:52:47.000000 cubestat-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:52:58.134715 cubestat-0.0.8/cubestat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 01:52:47.000000 cubestat-0.0.8/cubestat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16390 2023-06-21 01:52:47.000000 cubestat-0.0.8/cubestat/cubestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:52:58.134715 cubestat-0.0.8/cubestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:52:58.134715 cubestat-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-21 01:52:47.000000 cubestat-0.0.8/setup.py
```

### Comparing `cubestat-0.0.6/LICENSE` & `cubestat-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cubestat-0.0.6/README.md` & `cubestat-0.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,49 +16,55 @@
 Despite many monitoring tools available for monitoring typical system counters as well as GPU/Accelerators, horizon charts have a unique information density properties which makes it possible to show a history of N measurements for M metrics on a single screen for significantly large N and M. Thus, this tool was created.
 
 ## Installation and Usage:
 
 ```
 pip3 install cubestat
 
-usage: cubestat [-h] [--refresh_ms REFRESH_MS] [--buffer_size BUFFER_SIZE]
-                [--cpu {all,by_cluster,by_core}] [--color {red,green,blue,mixed}]
-                [--percentages {hidden,last}] [--disk] [--network]
+usage: cubestat [-h] [--refresh_ms REFRESH_MS] [--buffer_size BUFFER_SIZE] [--cpu {all,by_cluster,by_core}] [--color {red,green,blue,mixed}] [--percentages {hidden,last}] [--disk] [--network] [--no-disk] [--no-network]
 
 options:
   -h, --help            show this help message and exit
   --refresh_ms REFRESH_MS, -i REFRESH_MS
                         Update frequency, milliseconds
   --buffer_size BUFFER_SIZE
-                        How many datapoints to store. Having it larger than screen width is a good
-                        idea as terminal window can be resized
+                        How many datapoints to store. Having it larger than screen width is a good idea as terminal window can be resized
   --cpu {all,by_cluster,by_core}
-                        CPU mode - showing all cores, only cumulative by cluster or both. Can be
-                        toggled by pressing c.
+                        CPU mode - showing all cores, only cumulative by cluster or both. Can be toggled by pressing c.
   --color {red,green,blue,mixed}
   --percentages {hidden,last}
                         Show/hide numeric utilization percentage. Can be toggled by pressing p.
-  --disk                show disk read/write. Can be toggled by pressing d.
-  --network             show network io. Can be toggled by pressing n.
+  --disk                Show disk read/write. Can be toggled by pressing d.
+  --network             Show network io. Can be toggled by pressing n.
+  --no-disk             Hide disk read/write. Can be toggled by pressing d.
+  --no-network          Hide network io. Can be toggled by pressing n.
 ```
 
-Running on Apple devices will require sudo access, as `powermetrics` has such limitation. Running on Linux machines doesn't have this limitation.
+Interactive commands:
+* q - quit
+* p - show/hide percentage for last data point
+* c - change cpu display mode (individual cores, aggregated by cluster or both)
+* d - show/hide disk reads/writes
+* n - show/hide network utilization
+* UP/DOWN - scroll the lines in case there are more cores.
+
+Running on Apple devices will require sudo access, as `powermetrics` has this limitation. Running on Linux doesn't require it.
 
 Multi-gpu example - training [nano GPT](https://github.com/karpathy/nanoGPT) on 4 nVidia GPU instance:
 ![multigpu](static/multigpu.png)
 
 ## Dependencies
 * Python 3.?+
 * psutil 5.9.5
 * pynvml for nVidia cards monitoring
 
 ## TODO
 * GPU aggregation
 * CPU by socket/NUMA/SMT
-* better IO scale (joint scale for all IO?)
-* status line
+* status line (why though?)
 * better colors (especially for dark background)
 * multi-column layout for large instances (e.g. with 100+ cores)
 * try on Windows and BSD
 * Google TPU load?
 * AMD GPU load?
 * Filter by process?
+* joint scale for IO
```

### Comparing `cubestat-0.0.6/cubestat/cubestat.py` & `cubestat-0.0.8/cubestat/cubestat.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 parser.add_argument('--no-network', action="store_false", dest="network", help="Hide network io. Can be toggled by pressing n.")
 
 args = parser.parse_args()
 
 def snapshot_base():
     return {
         'cpu': {},
-        'accelerators': {},
         'ram': {'RAM used %': psutil.virtual_memory().percent},
+        'accelerators': {},
         'disk': {},
         'network': {},
     }
 
 # psutil + nvsmi for nVidia GPU
 class LinuxReader:
     def __init__(self, interval_ms):
@@ -100,17 +100,17 @@
         for i, v in enumerate(cpu_load):
             title = f'CPU {i} util %'
             res['cpu'][title] = v
             total_load += v
         res['cpu'][cluster_title] = total_load / len(cpu_load)
 
         if self.has_nvidia:
-            for i, v in enumerate(self.nvsmi.DeviceQuery('utilization.gpu')['gpu']):
-                title = f'GPU {i} util %'
-                res['accelerators'][title] = v['utilization']['gpu_util']
+            for i, v in enumerate(self.nvsmi.DeviceQuery('utilization.gpu,memory.total,memory.used')['gpu']):
+                res['accelerators'][f'GPU {i} util %'] = v['utilization']['gpu_util']
+                res['accelerators'][f'GPU {i} memory used %'] = 100.0 * v['fb_memory_usage']['used'] / v['fb_memory_usage']['total']
 
         if self.first:
             self.disk_read_last = disk_read_kb
             self.disk_written_last = disk_written_kb
             self.network_read_last = nw_read_kb
             self.network_written_last = nw_written_kb
             self.first = False
@@ -146,18 +146,18 @@
                 total_cluster += 1.0
             res['cpu'][cluster_title] = 100.0 - 100.0 * idle_cluster / total_cluster
 
         res['accelerators']['GPU util %'] = 100.0 - 100.0 * snapshot['gpu']['idle_ratio']
         ane_scaling = 8.0 * self.interval_ms
         res['accelerators']['ANE util %'] = 100.0 * snapshot['processor']['ane_energy'] / ane_scaling
 
-        res['disk']['disk read KB/s'] = snapshot['disk']['rbytes_per_s'] / (2 ** 10)
-        res['disk']['disk write KB/s'] = snapshot['disk']['wbytes_per_s'] / (2 ** 10)
-        res['network']['network i KB/s'] = snapshot['network']['ibyte_rate'] / (2 ** 10)
-        res['network']['network o KB/s'] = snapshot['network']['obyte_rate'] / (2 ** 10)
+        res['disk']['disk read'] = snapshot['disk']['rbytes_per_s']
+        res['disk']['disk write'] = snapshot['disk']['wbytes_per_s']
+        res['network']['network rx'] = snapshot['network']['ibyte_rate']
+        res['network']['network tx'] = snapshot['network']['obyte_rate']
         return res.items(), cpu_clusters
 
 # settings
 
 class Horizon:
     def __init__(self, stdscr, reader):
         stdscr.nodelay(False)
@@ -166,39 +166,40 @@
         curses.start_color()
         curses.use_default_colors()
 
         self.spacing_width = 1
         self.filling = '.'
         self.colorschemes = {
             Color.green: [-1, 150, 107, 22],
-            Color.red: [-1, 224, 138, 52],
-            Color.blue: [-1, 189, 103, 17],
+            Color.red: [-1, 224, 181, 138],
+            Color.blue: [-1, 189, 146, 103],
         }
 
         self.cells = self.prepare_cells()
         self.stdscr = stdscr
 
         # all of the fields below are mutable and can be accessed from 2 threads
         self.lock = Lock()
         self.data = {k: collections.defaultdict(lambda: collections.deque(maxlen=args.buffer_size)) for k in ['cpu', 'accelerators', 'ram', 'disk', 'network']}
         self.colormap = {
             'cpu': Color.green if args.color == Color.mixed else args.color,
-            'accelerators': Color.red if args.color == Color.mixed else args.color,
             'ram': Color.green if args.color == Color.mixed else args.color,
+            'accelerators': Color.red if args.color == Color.mixed else args.color,
             'disk': Color.blue if args.color == Color.mixed else args.color,
             'network': Color.blue if args.color == Color.mixed else args.color,
         }
         self.snapshots_observed = 0
         self.snapshots_rendered = 0
         self.percentage_mode = args.percentages
         self.cpumode = args.cpu
         self.show_disk = args.disk
         self.show_network = args.network
         self.settings_changed = False
         self.reader = reader
+        self.vertical_shift = 0
 
 
     def prepare_cells(self):
         chrs = [' ', '▁', '▂', '▃', '▄', '▅', '▆', '▇', '█']
         cells = {}
         colorpair = 1
         for name, colors in self.colorschemes.items():
@@ -243,23 +244,27 @@
                 return
         self.stdscr.erase()
         self.rows, self.cols = self.stdscr.getmaxyx()
         spacing = ' ' * self.spacing_width
 
         with self.lock:
             i = 0
+            skip = self.vertical_shift
             for group_name, group in self.data.items():
                 if group_name == 'disk' and not self.show_disk:
                     continue
                 if group_name == 'network' and not self.show_network:
                     continue
 
                 cells = self.cells[self.colormap[group_name]]
                 range = len(cells)
                 for title, series in group.items():
+                    if skip > 0:
+                        skip -= 1
+                        continue
                     indent = ''
 
                     if group_name == 'cpu':
                         if self.cpumode == CPUMode.by_cluster and title not in self.cpu_clusters:
                             continue
                         if self.cpumode == CPUMode.by_core and title in self.cpu_clusters:
                             continue
@@ -273,15 +278,20 @@
                     data_slice = list(itertools.islice(series, index, None))
 
                     B = 100.0
                     strvalue = f'last:{data_slice[-1]:3.0f}%{spacing}╗' if self.percentage_mode == Percentages.last else f'{spacing}╗'
                     if group_name == 'disk' or group_name == 'network':
                         B = max(data_slice)
                         B = float(1 if B == 0 else 2 ** (int((B - 1)).bit_length()))
-                        strvalue =  f'last:{data_slice[-1]:3.0f}|{int(B)}Kb/s{spacing}╗' if self.percentage_mode == Percentages.last else f'{spacing}╗'
+                        if B > 1024 * 1024: # Mb/s
+                            strvalue =  f'last:{data_slice[-1] / (1024 * 1024) :3.0f}|{int(B / (1024 * 1024))}Mb/s{spacing}╗' if self.percentage_mode == Percentages.last else f'{spacing}╗'
+                        elif B > 1024: # Kb/s
+                            strvalue =  f'last:{data_slice[-1] / 1024:3.0f}|{int(B / 1024)}Kb/s{spacing}╗' if self.percentage_mode == Percentages.last else f'{spacing}╗'
+                        else:
+                            strvalue =  f'last:{data_slice[-1]:3.0f}|{int(B)}bytes/s{spacing}╗' if self.percentage_mode == Percentages.last else f'{spacing}╗'
 
                     title_filling = self.filling * (self.cols - len(strvalue) - len(titlestr))
                     self.write_string(i * 2, len(titlestr), title_filling)
                     self.write_string(i * 2, self.cols - len(strvalue), strvalue)
 
                     border = f'{spacing}╝'
                     self.write_string(i * 2 + 1, self.cols - len(border), border)
@@ -303,14 +313,15 @@
                     i += 1
 
                 self.snapshots_rendered += 1
                 
         self.stdscr.refresh()
 
     def render_loop(self):
+        self.stdscr.keypad(True)
         while True:
             self.render()
             key = self.stdscr.getch()
             if key == ord('q') or key == ord('Q'):
                 exit(0)
             if key == ord('p'):
                 with self.lock:
@@ -324,14 +335,24 @@
                 with self.lock:
                     self.show_disk = not self.show_disk
                     self.settings_changed = True
             if key == ord('n'):
                 with self.lock:
                     self.show_network = not self.show_network
                     self.settings_changed = True
+            if key == curses.KEY_UP:
+                with self.lock:
+                    if self.vertical_shift > 0:
+                        self.vertical_shift -= 1
+                        self.settings_changed = True
+            if key == curses.KEY_DOWN:
+                with self.lock:
+                    self.vertical_shift += 1
+                    self.settings_changed = True
+
 
     def reader_loop_linux(self):
         begin_ts = time.time()
         n = 0
         d = args.refresh_ms / 1000.0
         while True:
             snapshot, cpu_clusters = self.reader.read()
```

### Comparing `cubestat-0.0.6/setup.py` & `cubestat-0.0.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cubestat',
-    version='0.0.6',
+    version='0.0.8',
     author='Oleksandr Kuvshynov',
     author_email='okuvshynov@gmail.com',
-    description='Horizon chart in terminal for CPU/GPU/ANE monitoring',
-    long_description='Horizon chart in terminal. Supports CPU/GPU/ANE monitoring for Apple M1/M2, nVidia GPUs',
+    description='Horizon chart in terminal for system monitoring',
+    long_description='Horizon chart in terminal. Supports CPU/GPU/ANE/RAM/IO monitoring for Apple M1/M2, nVidia GPUs',
     packages=find_packages(),
     install_requires=[
         'psutil>=5.9.5',
         'pynvml; platform_system=="Linux"'
     ],
     url='https://github.com/okuvshynov/cubestat',
     entry_points={
```

