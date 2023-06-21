# Comparing `tmp/turbx-0.3.0.tar.gz` & `tmp/turbx-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbx-0.3.0.tar", last modified: Mon Jun  5 13:53:04 2023, max compression
+gzip compressed data, was "turbx-0.3.1.tar", last modified: Wed Jun 21 10:36:54 2023, max compression
```

## Comparing `turbx-0.3.0.tar` & `turbx-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-05 13:53:04.442429 turbx-0.3.0/
--rwxrwxr-x   0 jason     (1000) jason     (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.3.0/LICENSE
--rw-rw-r--   0 jason     (1000) jason     (1000)     2353 2023-06-05 13:53:04.442429 turbx-0.3.0/PKG-INFO
--rwxrwxr-x   0 jason     (1000) jason     (1000)     1072 2023-04-15 18:45:25.000000 turbx-0.3.0/README.md
--rw-rw-r--   0 jason     (1000) jason     (1000)       38 2023-06-05 13:53:04.442429 turbx-0.3.0/setup.cfg
--rwxrwxr-x   0 jason     (1000) jason     (1000)     2295 2023-06-05 13:43:40.000000 turbx-0.3.0/setup.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-05 13:53:04.438429 turbx-0.3.0/turbx/
--rwxrwxr-x   0 jason     (1000) jason     (1000)     3260 2023-06-05 13:43:21.000000 turbx-0.3.0/turbx/__init__.py
--rwxrwxr-x   0 jason     (1000) jason     (1000)  1170945 2023-06-05 13:37:28.000000 turbx-0.3.0/turbx/turbx.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-05 13:53:04.442429 turbx-0.3.0/turbx.egg-info/
--rw-rw-r--   0 jason     (1000) jason     (1000)     2353 2023-06-05 13:53:04.000000 turbx-0.3.0/turbx.egg-info/PKG-INFO
--rw-rw-r--   0 jason     (1000) jason     (1000)      203 2023-06-05 13:53:04.000000 turbx-0.3.0/turbx.egg-info/SOURCES.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-06-05 13:53:04.000000 turbx-0.3.0/turbx.egg-info/dependency_links.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)      143 2023-06-05 13:53:04.000000 turbx-0.3.0/turbx.egg-info/requires.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        6 2023-06-05 13:53:04.000000 turbx-0.3.0/turbx.egg-info/top_level.txt
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-21 10:36:54.309107 turbx-0.3.1/
+-rwxrwxr-x   0 jason     (1000) jason     (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.3.1/LICENSE
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2353 2023-06-21 10:36:54.309107 turbx-0.3.1/PKG-INFO
+-rwxrwxr-x   0 jason     (1000) jason     (1000)     1072 2023-04-15 18:45:25.000000 turbx-0.3.1/README.md
+-rw-rw-r--   0 jason     (1000) jason     (1000)       38 2023-06-21 10:36:54.309107 turbx-0.3.1/setup.cfg
+-rwxrwxr-x   0 jason     (1000) jason     (1000)     2295 2023-06-21 10:32:03.000000 turbx-0.3.1/setup.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-21 10:36:54.305107 turbx-0.3.1/turbx/
+-rwxrwxr-x   0 jason     (1000) jason     (1000)     3260 2023-06-21 10:29:06.000000 turbx-0.3.1/turbx/__init__.py
+-rwxrwxr-x   0 jason     (1000) jason     (1000)  1228402 2023-06-21 10:28:35.000000 turbx-0.3.1/turbx/turbx.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-21 10:36:54.309107 turbx-0.3.1/turbx.egg-info/
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2353 2023-06-21 10:36:54.000000 turbx-0.3.1/turbx.egg-info/PKG-INFO
+-rw-rw-r--   0 jason     (1000) jason     (1000)      203 2023-06-21 10:36:54.000000 turbx-0.3.1/turbx.egg-info/SOURCES.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-06-21 10:36:54.000000 turbx-0.3.1/turbx.egg-info/dependency_links.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)      143 2023-06-21 10:36:54.000000 turbx-0.3.1/turbx.egg-info/requires.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)        6 2023-06-21 10:36:54.000000 turbx-0.3.1/turbx.egg-info/top_level.txt
```

### Comparing `turbx-0.3.0/LICENSE` & `turbx-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `turbx-0.3.0/PKG-INFO` & `turbx-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.3.0
+Version: 0.3.1
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
```

### Comparing `turbx-0.3.0/README.md` & `turbx-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `turbx-0.3.0/setup.py` & `turbx-0.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='turbx',
-    version='0.3.0',
+    version='0.3.1',
     description='Extensible toolkit for analyzing turbulent flow datasets',
     
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     url='https://github.com/iagappel/turbx',
     author='Jason A',
```

### Comparing `turbx-0.3.0/turbx/__init__.py` & `turbx-0.3.1/turbx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 turbx
 
 Extensible toolkit for analyzing turbulent flow datasets
 '''
 
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 __author__ = 'Jason A'
 
 from .turbx import cgd
 from .turbx import rgd
 from .turbx import eas4
 from .turbx import ztmd
 from .turbx import lpd
```

### Comparing `turbx-0.3.0/turbx/turbx.py` & `turbx-0.3.1/turbx/turbx.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,19 +71,14 @@
     Curvilinear Grid Data (CGD)
     ---------------------------
     - super()'ed h5py.File class
     '''
     
     def __init__(self, *args, **kwargs):
         
-        ## passthrough arg to get_header() to automatically read the full 3D grid on every MPI rank
-        ## upon opening. This is in general a bad idea for CGD, which has a 3D grid. If every rank reads the
-        ## full grid, RAM can very quickly fill up.
-        read_grid = kwargs.pop('read_grid', False) 
-        
         self.fname, self.open_mode = args
         
         self.fname_path = os.path.dirname(self.fname)
         self.fname_base = os.path.basename(self.fname)
         self.fname_root, self.fname_ext = os.path.splitext(self.fname_base)
         
         ## default to libver='latest' if none provided
@@ -106,29 +101,50 @@
             self.n_ranks = self.comm.Get_size()
             self.rank    = self.comm.Get_rank()
         else:
             self.comm    = None
             self.n_ranks = 1
             self.rank    = 0
         
+        ## cgd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
+        stripe_count   = kwargs.pop('stripe_count'   , 32    )
+        stripe_size_mb = kwargs.pop('stripe_size_mb' , 8     )
+        perms          = kwargs.pop('stripe_size_mb' , '640' )
+        
+        ## passthrough arg to get_header() to automatically read the full 3D grid on every MPI rank
+        ## upon opening. This is in general a bad idea for CGD, which has a 3D grid. If every rank reads the
+        ## full grid, RAM can very quickly fill up.
+        read_grid = kwargs.pop('read_grid', False)
+        
+        if not isinstance(stripe_count, int):
+            raise ValueError
+        if not isinstance(stripe_size_mb, int):
+            raise ValueError
+        if not isinstance(perms, str):
+            raise ValueError
+        if not len(perms)==3:
+            raise ValueError
+        if not re.fullmatch(r'\d{3}',perms):
+            raise ValueError
+        
         ## if not using MPI, remove 'driver' and 'comm' from kwargs
         if ( not self.usingmpi ) and ('driver' in kwargs):
             kwargs.pop('driver')
         if ( not self.usingmpi ) and ('comm' in kwargs):
             kwargs.pop('comm')
         
         ## | mpiexec --mca io romio321 -n $NP python3 ...
         ## | mpiexec --mca io ompio -n $NP python3 ...
-        ## | ompi_info --> print ompi settings ('MCA io' gives io implementation options)
+        ## | ompi_info --> print ompi settings (grep 'MCA io' for I/O opts)
         ## | export ROMIO_FSTYPE_FORCE="lustre:" --> force Lustre driver over UFS when using romio --> causes crash
         ## | export ROMIO_FSTYPE_FORCE="ufs:"
         ## | export ROMIO_PRINT_HINTS=1 --> show available hints
-        
+        ##
         ## https://doku.lrz.de/best-practices-hints-and-optimizations-for-io-10747318.html
-        
+        ##
         ## OMPIO
         ## export OMPI_MCA_sharedfp=^lockedfile,individual
         ## mpiexec --mca io ompio -n $NP python3 script.py
         
         ## set ROMIO hints, passed through 'mpi_info' dict
         if self.usingmpi:
             if ('info' in kwargs):
@@ -138,44 +154,47 @@
                 ##
                 mpi_info.Set('romio_ds_write' , 'disable'   )
                 mpi_info.Set('romio_ds_read'  , 'disable'   )
                 mpi_info.Set('romio_cb_read'  , 'automatic' )
                 mpi_info.Set('romio_cb_write' , 'automatic' )
                 #mpi_info.Set('romio_cb_read'  , 'enable' )
                 #mpi_info.Set('romio_cb_write' , 'enable' )
-                #mpi_info.Set('cb_buffer_size' , str(int(round(16*1024**2))) ) ## 16 [MB]
-                mpi_info.Set('cb_buffer_size' , str(int(round(32*1024**2))) ) ## 32 [MB]
+                mpi_info.Set('cb_buffer_size' , str(int(round(16*1024**2))) ) ## 16 [MB]
                 ##
-                #mpi_info.Set('romio_no_indep_rw' , 'true' ) ## Deferred open + only collective I/O 
+                #mpi_info.Set('romio_no_indep_rw' , 'true' ) ## deferred open + only collective I/O 
                 #mpi_info.Set('cb_nodes' , str(int(round(1*self.n_ranks))) )
                 ##
                 kwargs['info'] = mpi_info
                 self.mpi_info = mpi_info
         
         ## | rdcc_nbytes:
         ## | ------------
         ## | Integer setting the total size of the raw data chunk cache for this dataset in bytes.
         ## | In most cases increasing this number will improve performance, as long as you have 
         ## | enough free memory. The default size is 1 MB
         
         ## --> gets passed to H5Pset_chunk_cache
         if ('rdcc_nbytes' not in kwargs):
-            kwargs['rdcc_nbytes'] = int(32*1024**2) ## 32 [MB]
-            #kwargs['rdcc_nbytes'] = int(16*1024**2) ## 16 [MB]
+            kwargs['rdcc_nbytes'] = int(16*1024**2) ## 16 [MB]
         
         ## | rdcc_nslots:
         ## | ------------
         ## | Integer defining the number of chunk slots in the raw data chunk cache for this dataset.
         
         ## if ('rdcc_nslots' not in kwargs):
         ##     kwargs['rdcc_nslots'] = 521
         
-        ## cgd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
-        verbose = kwargs.pop('verbose',False)
-        force   = kwargs.pop('force',False)
+        ## rgd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
+        verbose = kwargs.pop( 'verbose' , False )
+        force   = kwargs.pop( 'force'   , False )
+        
+        if not isinstance(verbose, bool):
+            raise ValueError
+        if not isinstance(force, bool):
+            raise ValueError
         
         # === initialize file on FS
         
         ## if file open mode is 'w', the file exists, and force is False
         ## --> raise error
         if (self.open_mode == 'w') and (force is False) and os.path.isfile(self.fname):
             if (self.rank==0):
@@ -191,28 +210,32 @@
                                   or use force=True arg:
                                   
                                   >>> with cgd(<<fname>>,'w',force=True) as f:
                                   >>>     ...
                                   '''
                 print(textwrap.indent(textwrap.dedent(openModeInfoStr), 2*' ').strip('\n'))
                 print(72*'-'+'\n')
+                sys.stdout.flush()
             
             if (self.comm is not None):
                 self.comm.Barrier()
             raise FileExistsError()
         
-        ## if file open mode is 'w', the file exists, and force is True
-        ## --> delete, touch, chmod, stripe
-        if (self.open_mode == 'w') and (force is True) and os.path.isfile(self.fname):
+        ## if file open mode is 'w'
+        ## --> <delete>, touch, chmod, stripe
+        if (self.open_mode == 'w'):
             if (self.rank==0):
-                os.remove(self.fname)
-                Path(self.fname).touch()
-                os.chmod(self.fname, int('640', base=8))
-                if shutil.which('lfs') is not None:
-                    return_code = subprocess.call(f'lfs migrate --stripe-count 16 --stripe-size 16M {self.fname} > /dev/null 2>&1', shell=True)
+                if os.path.isfile(self.fname): ## if the file exists, delete it
+                    os.remove(self.fname)
+                    time.sleep(0.1)
+                Path(self.fname).touch() ## touch a new file
+                os.chmod(self.fname, int(perms, base=8)) ## change permissions
+                if shutil.which('lfs') is not None: ## set stripe if on Lustre
+                    cmd_str_lfs_migrate = f'lfs migrate --stripe-count {stripe_count:d} --stripe-size {stripe_size_mb:d}M {self.fname} > /dev/null 2>&1'
+                    return_code = subprocess.call(cmd_str_lfs_migrate, shell=True)
                     if (return_code != 0):
                         raise ValueError('lfs migrate failed')
                 else:
                     #print('striping with lfs not permitted on this filesystem')
                     pass
         
         if (self.comm is not None):
@@ -7764,32 +7787,45 @@
             self.n_ranks = self.comm.Get_size()
             self.rank    = self.comm.Get_rank()
         else:
             self.comm    = None
             self.n_ranks = 1
             self.rank    = 0
         
-        stripe_count   = kwargs.pop('stripe_count'   , 32 )
-        stripe_size_mb = kwargs.pop('stripe_size_mb' , 8  )
+        ## rgd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
+        stripe_count   = kwargs.pop('stripe_count'   , 32    )
+        stripe_size_mb = kwargs.pop('stripe_size_mb' , 8     )
+        perms          = kwargs.pop('stripe_size_mb' , '640' )
+        
+        if not isinstance(stripe_count, int):
+            raise ValueError
+        if not isinstance(stripe_size_mb, int):
+            raise ValueError
+        if not isinstance(perms, str):
+            raise ValueError
+        if not len(perms)==3:
+            raise ValueError
+        if not re.fullmatch(r'\d{3}',perms):
+            raise ValueError
         
         ## if not using MPI, remove 'driver' and 'comm' from kwargs
         if ( not self.usingmpi ) and ('driver' in kwargs):
             kwargs.pop('driver')
         if ( not self.usingmpi ) and ('comm' in kwargs):
             kwargs.pop('comm')
         
         ## | mpiexec --mca io romio321 -n $NP python3 ...
         ## | mpiexec --mca io ompio -n $NP python3 ...
-        ## | ompi_info --> print ompi settings ('MCA io' gives io implementation options)
+        ## | ompi_info --> print ompi settings (grep 'MCA io' for I/O opts)
         ## | export ROMIO_FSTYPE_FORCE="lustre:" --> force Lustre driver over UFS when using romio --> causes crash
         ## | export ROMIO_FSTYPE_FORCE="ufs:"
         ## | export ROMIO_PRINT_HINTS=1 --> show available hints
-        
+        ##
         ## https://doku.lrz.de/best-practices-hints-and-optimizations-for-io-10747318.html
-        
+        ##
         ## OMPIO
         ## export OMPI_MCA_sharedfp=^lockedfile,individual
         ## mpiexec --mca io ompio -n $NP python3 script.py
         
         ## set ROMIO hints, passed through 'mpi_info' dict
         if self.usingmpi:
             if ('info' in kwargs):
@@ -7800,43 +7836,46 @@
                 mpi_info.Set('romio_ds_write' , 'disable'   )
                 mpi_info.Set('romio_ds_read'  , 'disable'   )
                 mpi_info.Set('romio_cb_read'  , 'automatic' )
                 mpi_info.Set('romio_cb_write' , 'automatic' )
                 #mpi_info.Set('romio_cb_read'  , 'enable' )
                 #mpi_info.Set('romio_cb_write' , 'enable' )
                 mpi_info.Set('cb_buffer_size' , str(int(round(16*1024**2))) ) ## 16 [MB]
-                #mpi_info.Set('cb_buffer_size' , str(int(round(32*1024**2))) ) ## 32 [MB]
                 ##
-                #mpi_info.Set('romio_no_indep_rw' , 'true' ) ## Deferred open + only collective I/O 
+                #mpi_info.Set('romio_no_indep_rw' , 'true' ) ## deferred open + only collective I/O 
                 #mpi_info.Set('cb_nodes' , str(int(round(1*self.n_ranks))) )
                 ##
                 kwargs['info'] = mpi_info
                 self.mpi_info = mpi_info
         
         ## | rdcc_nbytes:
         ## | ------------
         ## | Integer setting the total size of the raw data chunk cache for this dataset in bytes.
         ## | In most cases increasing this number will improve performance, as long as you have 
         ## | enough free memory. The default size is 1 MB
         
         ## --> gets passed to H5Pset_chunk_cache
         if ('rdcc_nbytes' not in kwargs):
-            #kwargs['rdcc_nbytes'] = int(32*1024**2) ## 32 [MB]
             kwargs['rdcc_nbytes'] = int(16*1024**2) ## 16 [MB]
         
         ## | rdcc_nslots:
         ## | ------------
         ## | Integer defining the number of chunk slots in the raw data chunk cache for this dataset.
         
         ## if ('rdcc_nslots' not in kwargs):
         ##     kwargs['rdcc_nslots'] = 521
         
         ## rgd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
-        verbose = kwargs.pop('verbose',False)
-        force   = kwargs.pop('force',False)
+        verbose = kwargs.pop( 'verbose' , False )
+        force   = kwargs.pop( 'force'   , False )
+        
+        if not isinstance(verbose, bool):
+            raise ValueError
+        if not isinstance(force, bool):
+            raise ValueError
         
         # === initialize file on FS
         
         ## if file open mode is 'w', the file exists, and force is False
         ## --> raise error
         if (self.open_mode == 'w') and (force is False) and os.path.isfile(self.fname):
             if (self.rank==0):
@@ -7852,27 +7891,30 @@
                                   or use force=True arg:
                                   
                                   >>> with rgd(<<fname>>,'w',force=True) as f:
                                   >>>     ...
                                   '''
                 print(textwrap.indent(textwrap.dedent(openModeInfoStr), 2*' ').strip('\n'))
                 print(72*'-'+'\n')
+                sys.stdout.flush()
             
             if (self.comm is not None):
                 self.comm.Barrier()
             raise FileExistsError()
         
-        ## if file open mode is 'w', the file exists, and force is True
-        ## --> delete, touch, chmod, stripe
-        if (self.open_mode == 'w') and (force is True) and os.path.isfile(self.fname):
+        ## if file open mode is 'w'
+        ## --> <delete>, touch, chmod, stripe
+        if (self.open_mode == 'w'):
             if (self.rank==0):
-                os.remove(self.fname)
-                Path(self.fname).touch()
-                os.chmod(self.fname, int('640', base=8))
-                if shutil.which('lfs') is not None:
+                if os.path.isfile(self.fname): ## if the file exists, delete it
+                    os.remove(self.fname)
+                    time.sleep(0.1)
+                Path(self.fname).touch() ## touch a new file
+                os.chmod(self.fname, int(perms, base=8)) ## change permissions
+                if shutil.which('lfs') is not None: ## set stripe if on Lustre
                     cmd_str_lfs_migrate = f'lfs migrate --stripe-count {stripe_count:d} --stripe-size {stripe_size_mb:d}M {self.fname} > /dev/null 2>&1'
                     return_code = subprocess.call(cmd_str_lfs_migrate, shell=True)
                     if (return_code != 0):
                         raise ValueError('lfs migrate failed')
                 else:
                     #print('striping with lfs not permitted on this filesystem')
                     pass
@@ -8568,15 +8610,15 @@
             raise ValueError('prec not set correctly')
         
         ## HDF5 chunk parameters (t,z,y,x)
         if (chunk_constraint is None):
             chunk_constraint = (1,None,None,None) ## single [t] convention
             #chunk_constraint = (None,-1,1,-1) ## single [y] convention
         if (chunk_base is None):
-            chunk_base = 4
+            chunk_base = 2
         
         ## check for an often made mistake
         ts_min = kwargs.get('ts_min',None)
         ts_max = kwargs.get('ts_max',None)
         if (ts_min is not None):
             raise AssertionError('ts_min is not an option --> did you mean ti_min or tt_min?')
         if (ts_max is not None):
@@ -8994,15 +9036,15 @@
             raise FileExistsError('%s already exists. delete it or use \'force=True\' kwarg'%fn_rgd_tgt)
         
         ## HDF5 chunk parameters
         if (chunk_constraint is None):
             chunk_constraint = (1,None,None,None) ## single [t] convention
             #chunk_constraint = (None,-1,1,-1) ## single [y] convention
         if (chunk_base is None):
-            chunk_base = 4
+            chunk_base = 2
         
         # ===
         
         with rgd(fn_rgd_src, 'r', comm=MPI.COMM_WORLD, driver='mpio', libver='latest') as hf_src:
             with rgd(fn_rgd_tgt, 'w', comm=MPI.COMM_WORLD, driver='mpio', libver='latest', force=force) as hf_tgt:
                 
                 ## copy over header info (source --> target)
@@ -9664,15 +9706,15 @@
         t_start_func = timeit.default_timer()
         
         rx = kwargs.get('rx',1)
         ry = kwargs.get('ry',1)
         rz = kwargs.get('rz',1)
         rt = kwargs.get('rt',1)
         
-        chunk_kb         = kwargs.get('chunk_kb',4*1024) ## h5 chunk size: default 4 [MB]
+        chunk_kb         = kwargs.get('chunk_kb',8*1024) ## h5 chunk size: default 8 [MB]
         chunk_constraint = kwargs.get('chunk_constraint',None) ## the 'constraint' parameter for sizing h5 chunks
         chunk_base       = kwargs.get('chunk_base',None)
         
         self.nx = nx = kwargs.get('nx',128)
         self.ny = ny = kwargs.get('ny',128)
         self.nz = nz = kwargs.get('nz',128)
         self.nt = nt = kwargs.get('nt',128)
@@ -9806,15 +9848,15 @@
         if verbose: print('total time : rgd.populate_white_noise() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
     # === averaging
     
-    def get_mean(self, **kwargs):
+    def __get_mean_legacy(self, **kwargs):
         '''
         get mean in [t] --> leaves [x,y,z,1]
         --> save to new RGD file
         '''
         
         if (self.rank==0):
             verbose = True
@@ -9843,15 +9885,15 @@
         chunk_base       = kwargs.get('chunk_base',None)
         
         ## HDF5 chunk parameters (t,z,y,x)
         if (chunk_constraint is None):
             chunk_constraint = (1,None,None,None) ## single [t] convention
             #chunk_constraint = (None,-1,1,-1) ## single [y] convention
         if (chunk_base is None):
-            chunk_base = 4
+            chunk_base = 2
         
         if (rx*ry*rz != self.n_ranks):
             raise AssertionError('rx*ry*rz != self.n_ranks')
         if (rx>self.nx):
             raise AssertionError('rx>self.nx')
         if (ry>self.ny):
             raise AssertionError('ry>self.ny')
@@ -10174,14 +10216,462 @@
         if verbose: even_print('read total avg', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_read,t_read,(data_gb_read/t_read)))
         if verbose: even_print('write total avg', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_write,t_write,(data_gb_write/t_write)))
         if verbose: print(72*'-')
         if verbose: print('total time : rgd.get_mean() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         return
     
+    def get_mean(self, **kwargs):
+        '''
+        get mean in [t] --> leaves [x,y,z,1]
+        --> save to new RGD file
+        -----
+        - this version uses accumulator buffers and does *(1/n) at end to calculate mean
+        - this allows for low RAM usage, as the time dim can be sub-chunked (ct=N)
+        '''
+        
+        if (self.rank==0):
+            verbose = True
+        else:
+            verbose = False
+        
+        if verbose: print('\n'+'rgd.get_mean()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
+        
+        rx = kwargs.get('rx',1)
+        ry = kwargs.get('ry',1)
+        rz = kwargs.get('rz',1)
+        rt = kwargs.get('rt',1)
+        
+        fn_rgd_mean  = kwargs.get('fn_rgd_mean',None)
+        #sfm         = kwargs.get('scalars',None) ## scalars to take (for mean)
+        ti_min       = kwargs.get('ti_min',None)
+        favre        = kwargs.get('favre',True)
+        reynolds     = kwargs.get('reynolds',True)
+        
+        ct           = kwargs.get('ct',1)
+        
+        force        = kwargs.get('force',False)
+        
+        chunk_kb         = kwargs.get('chunk_kb',4*1024) ## h5 chunk size: default 4 [MB]
+        chunk_constraint = kwargs.get('chunk_constraint',None) ## the 'constraint' parameter for sizing h5 chunks
+        chunk_base       = kwargs.get('chunk_base',None)
+        
+        ## HDF5 chunk parameters (t,z,y,x)
+        if (chunk_constraint is None):
+            chunk_constraint = (1,None,None,None)
+        if (chunk_base is None):
+            chunk_base = 2
+        
+        if (rt!=1):
+            raise AssertionError('rt!=1')
+        if (rx*ry*rz != self.n_ranks):
+            raise AssertionError('rx*ry*rz != self.n_ranks')
+        if (rx>self.nx):
+            raise AssertionError('rx>self.nx')
+        if (ry>self.ny):
+            raise AssertionError('ry>self.ny')
+        if (rz>self.nz):
+            raise AssertionError('rz>self.nz')
+        if (ti_min is not None):
+            if not isinstance(ti_min, int):
+                raise TypeError('ti_min must be type int')
+        
+        if self.usingmpi:
+            comm4d = self.comm.Create_cart(dims=[rx,ry,rz], periods=[False,False,False], reorder=False)
+            t4d = comm4d.Get_coords(self.rank)
+            
+            rxl_ = np.array_split(np.arange(self.nx,dtype=np.int64),min(rx,self.nx))
+            ryl_ = np.array_split(np.arange(self.ny,dtype=np.int64),min(ry,self.ny))
+            rzl_ = np.array_split(np.arange(self.nz,dtype=np.int64),min(rz,self.nz))
+            #rtl_ = np.array_split(np.arange(self.nt,dtype=np.int64),min(rt,self.nt))
+            
+            rxl = [[b[0],b[-1]+1] for b in rxl_ ]
+            ryl = [[b[0],b[-1]+1] for b in ryl_ ]
+            rzl = [[b[0],b[-1]+1] for b in rzl_ ]
+            #rtl = [[b[0],b[-1]+1] for b in rtl_ ]
+            
+            rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
+            ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
+            rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
+            #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
+        else:
+            nxr = self.nx
+            nyr = self.ny
+            nzr = self.nz
+            #ntr = self.nt
+        
+        # === mean file name (for writing)
+        if (fn_rgd_mean is None):
+            fname_path = os.path.dirname(self.fname)
+            fname_base = os.path.basename(self.fname)
+            fname_root, fname_ext = os.path.splitext(fname_base)
+            fname_mean_h5_base = fname_root+'_mean.h5'
+            #fn_rgd_mean = os.path.join(fname_path, fname_mean_h5_base)
+            fn_rgd_mean = str(PurePosixPath(fname_path, fname_mean_h5_base))
+            #fn_rgd_mean = Path(fname_path, fname_mean_h5_base)
+        
+        if verbose: even_print('fn_rgd'       , self.fname   )
+        if verbose: even_print('fn_rgd_mean'  , fn_rgd_mean  )
+        #if verbose: even_print('fn_rgd_prime' , fn_rgd_prime )
+        if verbose: even_print('do Favre avg' , str(favre)   )
+        if verbose: even_print('do Reynolds avg' , str(reynolds)   )
+        if verbose: print(72*'-')
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: print(72*'-')
+        if verbose: even_print('rx','%i'%rx)
+        if verbose: even_print('ry','%i'%ry)
+        if verbose: even_print('rz','%i'%rz)
+        if verbose: even_print('ct','%i'%ct)
+        if verbose: print(72*'-')
+        
+        ## get times to take for avg
+        if (ti_min is not None):
+            ti_for_avg = np.copy( self.ti[ti_min:] )
+        else:
+            ti_for_avg = np.copy( self.ti )
+        
+        nt_avg       = ti_for_avg.shape[0]
+        t_avg_start  = self.t[ti_for_avg[0]]
+        t_avg_end    = self.t[ti_for_avg[-1]]
+        duration_avg = t_avg_end - t_avg_start
+        
+        #if not isinstance(ct, (int,np.int32,np.int64)):
+        if not isinstance(ct, int):
+            raise ValueError
+        if (ct<1):
+            raise ValueError
+        
+        ## [t] sub chunk range
+        ctl_ = np.array_split( ti_for_avg, min(ct,nt_avg) )
+        ctl = [[b[0],b[-1]+1] for b in ctl_ ]
+        
+        ## check that no sub ranges are <=1
+        for a_ in [ ctl_[1]-ctl_[0] for ctl_ in ctl ]:
+            if (a_ <= 1):
+                raise ValueError
+        
+        ## assert constant Δt, later attach dt as attribute to mean file
+        dt0 = np.diff(self.t)[0]
+        if not np.all(np.isclose(np.diff(self.t), dt0, rtol=1e-7)):
+            raise ValueError
+        
+        if verbose: even_print('n timesteps avg','%i/%i'%(nt_avg,self.nt))
+        if verbose: even_print('t index avg start','%i'%(ti_for_avg[0],))
+        if verbose: even_print('t index avg end','%i'%(ti_for_avg[-1],))
+        if verbose: even_print('t avg start','%0.2f [-]'%(t_avg_start,))
+        if verbose: even_print('t avg end','%0.2f [-]'%(t_avg_end,))
+        if verbose: even_print('duration avg','%0.2f [-]'%(duration_avg,))
+        if verbose: even_print('Δt','%0.2f [-]'%(dt0,))
+        #if verbose: print(72*'-')
+        
+        ## performance
+        t_read = 0.
+        t_write = 0.
+        data_gb_read = 0.
+        data_gb_write = 0.
+        
+        ##data_gb      = 4*self.nx*self.ny*self.nz*self.nt / 1024**3
+        #data_gb      = 4*self.nx*self.ny*self.nz*nt_avg / 1024**3
+        #data_gb_mean = 4*self.nx*self.ny*self.nz*1      / 1024**3
+        
+        scalars_re = ['u','v','w','p','T','rho']
+        scalars_fv = ['u','v','w','p','T','rho']
+        
+        ## do a loop through to get names
+        scalars_mean_names  = []
+        scalars_mean_dtypes = []
+        for scalar in self.scalars:
+            dtype = self.scalars_dtypes_dict[scalar]
+            if reynolds:
+                if True: ## always
+                    sc_name = scalar
+                    scalars_mean_names.append(sc_name)
+                    scalars_mean_dtypes.append(dtype)
+            if favre:
+                if (scalar in scalars_fv):
+                    sc_name = f'r_{scalar}'
+                    scalars_mean_names.append(sc_name)
+                    scalars_mean_dtypes.append(dtype)
+        
+        #with rgd(fn_rgd_mean, 'w', force=force, driver='mpio', comm=MPI.COMM_WORLD) as hf_mean:
+        with rgd(fn_rgd_mean, 'w', force=force, driver=self.driver, comm=self.comm) as hf_mean:
+            
+            ## initialize the mean file from the opened unsteady rgd file
+            hf_mean.init_from_rgd(self.fname)
+            
+            ## set some top-level attributes
+            hf_mean.attrs['duration_avg'] = duration_avg ## duration of mean
+            #hf_mean.attrs['duration_avg'] = self.duration
+            hf_mean.attrs['dt'] = dt0
+            #hf_mean.attrs['fclass'] = 'rgd'
+            hf_mean.attrs['fsubtype'] = 'mean'
+            
+            if verbose: print(72*'-')
+            
+            # === initialize mean datasets
+            for scalar in self.scalars:
+                
+                dtype = self.scalars_dtypes_dict[scalar]
+                float_bytes = self.scalars_dtypes_dict[scalar].itemsize
+                
+                data_gb_mean = float_bytes*self.nx*self.ny*self.nz*1 / 1024**3
+                
+                shape  = (1,self.nz,self.ny,self.nx)
+                chunks = h5_chunk_sizer(nxi=shape, constraint=chunk_constraint, size_kb=chunk_kb, base=chunk_base, itemsize=float_bytes)
+                
+                if reynolds:
+                    
+                    ## do the Re mean of all scalars in file, regardless whether explicitly in scalars_re or not
+                    #if scalar in scalars_re:
+                    if True:
+                        
+                        if ('data/%s'%scalar in hf_mean):
+                            del hf_mean['data/%s'%scalar]
+                        if verbose:
+                            even_print( f'initializing data/{scalar}' , f'{data_gb_mean:0.3f} [GB]' )
+                        dset = hf_mean.create_dataset(f'data/{scalar}',
+                                                      shape=shape,
+                                                      dtype=dtype,
+                                                      chunks=chunks,
+                                                      )
+                        hf_mean.scalars.append('data/%s'%scalar)
+                        
+                        chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
+                        if verbose:
+                            even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
+                            even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
+                
+                if favre:
+                    
+                    if (scalar in scalars_fv):
+                        if ('data/%s_fv'%scalar in hf_mean):
+                            del hf_mean['data/%s_fv'%scalar]
+                        if verbose:
+                            even_print( f'initializing data/{scalar}_fv' , f'{data_gb_mean:0.3f} [GB]' )
+                        dset = hf_mean.create_dataset(f'data/{scalar}_fv',
+                                                      shape=shape,
+                                                      dtype=dtype,
+                                                      chunks=chunks,
+                                                      )
+                        hf_mean.scalars.append('data/%s_fv'%scalar)
+                        
+                        chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
+                        if verbose:
+                            even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
+                            even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
+            
+            if self.usingmpi: self.comm.Barrier()
+            if verbose: print(72*'-')
+            
+            ## accumulator array for local rank --> initialize
+            data_sum = np.zeros(shape=(nxr,nyr,nzr,1), dtype={'names':scalars_mean_names, 'formats':[np.float64 for _ in scalars_mean_names]})
+            
+            # === main loop
+            
+            if verbose:
+                progress_bar = tqdm(total=ct, ncols=100, desc='mean', leave=False, file=sys.stdout)
+            
+            ct_counter=0
+            for ctl_ in ctl:
+                ct_counter += 1
+                ct1, ct2 = ctl_
+                ntc = ct2 - ct1
+                
+                if verbose:
+                    mesg = f'[t] sub chunk {ct_counter:d}/{ct:d}'
+                    tqdm.write( mesg )
+                    tqdm.write( '-'*len(mesg) )
+                
+                # === read rho
+                if favre:
+                    
+                    dset = self['data/rho']
+                    
+                    dtype = self.scalars_dtypes_dict['rho']
+                    if (dtype!=dset.dtype):
+                        raise ValueError
+                    float_bytes = self.scalars_dtypes_dict[scalar].itemsize
+                    
+                    if self.usingmpi: self.comm.Barrier()
+                    t_start = timeit.default_timer()
+                    
+                    if self.usingmpi: 
+                        with dset.collective:
+                            ##rho = dset[:,rz1:rz2,ry1:ry2,rx1:rx2].T
+                            #rho = dset[ti_min:,rz1:rz2,ry1:ry2,rx1:rx2].T
+                            rho = dset[ct1:ct2,rz1:rz2,ry1:ry2,rx1:rx2].T
+                    else:
+                        #rho = dset[()].T
+                        #rho = dset[ti_min:,:,:,:].T
+                        rho = dset[ct1:ct2,:,:,:].T
+                    
+                    if self.usingmpi: self.comm.Barrier()
+                    t_delta = timeit.default_timer() - t_start
+                    
+                    #data_gb = float_bytes*self.nx*self.ny*self.nz*nt_avg / 1024**3
+                    data_gb = float_bytes*self.nx*self.ny*self.nz*ntc / 1024**3
+                    
+                    if verbose:
+                        txt = even_print('read: rho', '%0.2f [GB]  %0.2f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)), s=True)
+                        tqdm.write(txt)
+                    
+                    t_read       += t_delta
+                    data_gb_read += data_gb
+                
+                # === read data, sum
+                for scalar in self.scalars:
+                    
+                    dset = self[f'data/{scalar}']
+                    dtype = self.scalars_dtypes_dict[scalar]
+                    if (dtype!=dset.dtype):
+                        raise ValueError
+                    float_bytes = dtype.itemsize
+                    
+                    # === collective read
+                    if self.usingmpi: self.comm.Barrier()
+                    t_start = timeit.default_timer()
+                    
+                    if self.usingmpi:
+                        with dset.collective:
+                            ##data = dset[:,rz1:rz2,ry1:ry2,rx1:rx2].T
+                            #data = dset[ti_min:,rz1:rz2,ry1:ry2,rx1:rx2].T
+                            data = dset[ct1:ct2,rz1:rz2,ry1:ry2,rx1:rx2].T
+                    else:
+                        ##data = dset[()].T
+                        #data = dset[ti_min:,:,:,:].T
+                        data = dset[ct1:ct2,:,:,:].T
+                    
+                    if self.usingmpi: self.comm.Barrier()
+                    t_delta = timeit.default_timer() - t_start
+                    
+                    #data_gb = float_bytes*self.nx*self.ny*self.nz*nt_avg / 1024**3
+                    data_gb = float_bytes*self.nx*self.ny*self.nz*ntc / 1024**3
+                    
+                    if (self.rank==0):
+                        txt = even_print('read: %s'%scalar, '%0.2f [GB]  %0.2f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)), s=True)
+                        tqdm.write(txt)
+                    
+                    t_read       += t_delta
+                    data_gb_read += data_gb
+                    
+                    # === do sum, add to accumulator
+                    if reynolds:
+                        sc_name = scalar
+                        data_sum[sc_name] += np.sum(data, axis=-1, dtype=np.float64, keepdims=True)
+                    if favre:
+                        ##if (scalar in scalars_fv):
+                        sc_name = f'r_{scalar}'
+                        data_sum[sc_name] += np.sum(data*rho, axis=-1, dtype=np.float64, keepdims=True)
+                    
+                    if self.usingmpi: self.comm.Barrier()
+                
+                mem_avail_gb = psutil.virtual_memory().available/1024**3
+                mem_free_gb  = psutil.virtual_memory().free/1024**3
+                if verbose:
+                    tqdm.write(even_print('mem free', '%0.1f [GB]'%mem_free_gb, s=True))
+                
+                if verbose: progress_bar.update()
+                if verbose: tqdm.write(72*'-')
+            if verbose: progress_bar.close()
+            
+            # === multiply accumulators by (1/n)
+            for scalar in self.scalars:
+                if reynolds:
+                    sc_name = scalar
+                    data_sum[sc_name] *= (1/nt_avg)
+                if favre:
+                    sc_name = f'r_{scalar}'
+                    data_sum[sc_name] *= (1/nt_avg)
+            
+            # ======================================== #
+            # === 'data_sum' now contains averages === #
+            # ======================================== #
+            
+            ## Favre avg : φ_tilde = avg[ρ·φ]/avg[ρ]
+            rho_mean = np.copy(data_sum['rho'])
+            
+            # === write
+            for scalar in self.scalars:
+                
+                if reynolds:
+                    
+                    dset = hf_mean[f'data/{scalar}']
+                    dtype = dset.dtype
+                    float_bytes = dtype.itemsize
+                    
+                    if self.usingmpi: self.comm.Barrier()
+                    t_start = timeit.default_timer()
+                    if self.usingmpi:
+                        with dset.collective:
+                            dset[:,rz1:rz2,ry1:ry2,rx1:rx2] = data_sum[scalar].T
+                    else:
+                        dset[:,:,:,:] = data_sum[scalar].T
+                    if self.usingmpi: self.comm.Barrier()
+                    t_delta = timeit.default_timer() - t_start
+                    
+                    data_gb_mean = float_bytes*self.nx*self.ny*self.nz*1 / 1024**3
+                    
+                    if verbose:
+                        txt = even_print(f'write: {scalar}', '%0.2f [GB]  %0.2f [s]  %0.3f [GB/s]'%(data_gb_mean,t_delta,(data_gb_mean/t_delta)), s=True)
+                        tqdm.write(txt)
+                    
+                    t_write       += t_delta
+                    data_gb_write += data_gb_mean
+                
+                if favre:
+                    
+                    dset = hf_mean[f'data/{scalar}_fv']
+                    dtype = dset.dtype
+                    float_bytes = dtype.itemsize
+                    
+                    data_ = np.copy( data_sum[f'r_{scalar}'] / rho_mean )
+                    
+                    if self.usingmpi: self.comm.Barrier()
+                    t_start = timeit.default_timer()
+                    if self.usingmpi:
+                        with dset.collective:
+                            dset[:,rz1:rz2,ry1:ry2,rx1:rx2] = data_.T
+                    else:
+                        dset[:,:,:,:] = data_.T
+                    if self.usingmpi: self.comm.Barrier()
+                    t_delta = timeit.default_timer() - t_start
+                    
+                    data_gb_mean = float_bytes*self.nx*self.ny*self.nz*1 / 1024**3
+                    
+                    if verbose:
+                        txt = even_print(f'write: {scalar}_fv', '%0.2f [GB]  %0.2f [s]  %0.3f [GB/s]'%(data_gb_mean,t_delta,(data_gb_mean/t_delta)), s=True)
+                        tqdm.write(txt)
+                    
+                    t_write       += t_delta
+                    data_gb_write += data_gb_mean
+            
+            # === replace dims/t array --> take last time of series
+            t = np.array([self.t[-1]],dtype=np.float64)
+            if ('dims/t' in hf_mean):
+                del hf_mean['dims/t']
+            hf_mean.create_dataset('dims/t', data=t)
+            
+            if hasattr(hf_mean, 'duration_avg'):
+                if verbose: even_print('duration avg', '%0.2f [-]'%hf_mean.duration_avg)
+        
+        if verbose: print(72*'-')
+        if verbose: even_print('time read',format_time_string(t_read))
+        if verbose: even_print('time write',format_time_string(t_write))
+        if verbose: even_print(fn_rgd_mean, '%0.2f [GB]'%(os.path.getsize(fn_rgd_mean)/1024**3))
+        if verbose: even_print('read total avg', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_read,t_read,(data_gb_read/t_read)))
+        if verbose: even_print('write total avg', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_write,t_write,(data_gb_write/t_write)))
+        if verbose: print(72*'-')
+        if verbose: print('total time : rgd.get_mean() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        return
+    
     def add_mean_dimensional_data_xpln(self, **kwargs):
         '''
         get dimensionalized mean data for [x] plane
         --> save to existing RGD file with fsubtype=mean
         - assumes volume which is thin in [x] direction
         - an RGD which is the output of rgd.get_mean() should be opened here
         - not parallel
@@ -10520,14 +11010,50 @@
         
         if verbose: print(72*'-')
         if verbose: print('total time : rgd.add_mean_dimensional_data_xpln() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
+    def add_mean_dimensional_data_ypln(self, **kwargs):
+        '''
+        get dimensionalized mean data for [y] plane
+        --> save to existing RGD file with fsubtype=mean
+        - assumes volume which is thin in [y] direction
+        - an RGD which is the output of rgd.get_mean() should be opened here
+        - not parallel
+        '''
+        
+        pass
+        raise NotImplementedError
+        
+        if verbose: print(72*'-')
+        if verbose: print('total time : rgd.add_mean_dimensional_data_ypln() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
+        return
+    
+    def add_mean_dimensional_data_zpln(self, **kwargs):
+        '''
+        get dimensionalized mean data for [z] plane
+        --> save to existing RGD file with fsubtype=mean
+        - assumes volume which is thin in [z] direction
+        - an RGD which is the output of rgd.get_mean() should be opened here
+        - not parallel
+        '''
+        
+        pass
+        raise NotImplementedError
+        
+        if verbose: print(72*'-')
+        if verbose: print('total time : rgd.add_mean_dimensional_data_zpln() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
+        return
+    
     # === unsteady
     
     def get_prime(self, **kwargs):
         '''
         get mean-removed (prime) variables in [t]
         -----
         XI  : Reynolds primes : mean(XI)=0
@@ -10566,15 +11092,15 @@
         ti_min = kwargs.get('ti_min',None)
         
         ## HDF5 chunk parameters (t,z,y,x)
         if (chunk_constraint is None):
             chunk_constraint = (1,None,None,None) ## single [t] convention
             #chunk_constraint = (None,-1,1,-1) ## single [y] convention
         if (chunk_base is None):
-            chunk_base = 4
+            chunk_base = 2
         
         ## if writing Favre primes, copy over ρ --> mean(ρ·XII)=0 / mean(XII)≠0 !!
         if favre:
             copy_rho = True
         else:
             copy_rho = False
         
@@ -13137,27 +13663,29 @@
             even_print('mem available', '%0.1f [GB] / %0.1f[%%]'%(mem_avail_gb,(100*mem_avail_gb/mem_total_gb)))
             even_print('mem free',      '%0.1f [GB] / %0.1f[%%]'%(mem_free_gb,(100*mem_free_gb/mem_total_gb)))
         
         ## for spanwise mean, no overlapping windows are applied, so win_len = [z] vec length
         win_len = nz
         
         ## the window function
-        window_type = 'tukey'
+        #window_type = 'tukey'
+        window_type = None
         if (window_type=='tukey'):
             window = sp.signal.windows.tukey(win_len, alpha=0.1)
         elif (window_type is None):
             window = np.ones(win_len, dtype=np.float64)
         if verbose:
             even_print('window type', '\'%s\''%str(window_type))
         
         ## sum of sqrt of window: needed for power normalization
         sum_sqrt_win = np.sum(np.sqrt(window))
         
         if verbose:
-            even_print('sum(sqrt(window)) / win_len', '%0.5f'%(sum_sqrt_win/win_len))
+            even_print('sum(sqrt(window))'          , '%0.5f'%(sum_sqrt_win,))
+            even_print('sum(sqrt(window)) / win_len', '%0.5f'%(sum_sqrt_win/win_len,))
         
         if verbose:
             print(72*'-')
         
         # === main loop
         
         ## main loop --> turbulent spectrum in [Δz] at every [x,y,t]
@@ -13264,15 +13792,15 @@
                         #A_uj = sp.fft.fft(uj)[fp] / n
                         ui   *= window
                         uj   *= window
                         #ui  -= np.mean(ui) ## de-trend
                         #uj  -= np.mean(uj)
                         A_ui    = sp.fft.fft(ui)[kzp] / sum_sqrt_win
                         A_uj    = sp.fft.fft(uj)[kzp] / sum_sqrt_win
-                        Euu_ijk = 2 * np.real(A_ui*np.conj(A_uj)) / dkz
+                        Euu_ijk = 2. * np.real(A_ui*np.conj(A_uj)) / dkz
                         
                         ## divide off mean mass density
                         if density_scaling:
                             Euu_ijk /= rho_avg**2
                         
                         ## normalize such that ∫PSD=(co)variance
                         if normalize_psd_by_cov:
@@ -13338,15 +13866,382 @@
         return
     
     def calc_turb_spectrum_2d_span_time(self, **kwargs):
         '''
         calculate 2D FFT in [z,t] at every [x,y], avg in [x]
         - designed for analyzing unsteady, thin planes in [x]
         '''
-        pass
+        
+        if (self.rank==0):
+            verbose = True
+        else:
+            verbose = False
+        
+        if verbose: print('\n'+'rgd.calc_turb_spectrum_2d_span_time()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
+        
+        if (self.fsubtype!='prime'):
+            raise ValueError
+        
+        rx = kwargs.get('rx',1)
+        ry = kwargs.get('ry',1)
+        rz = kwargs.get('rz',1)
+        rt = kwargs.get('rt',1)
+        
+        overlap_fac_nom = kwargs.get('overlap_fac_nom',0.50)
+        n_win           = kwargs.get('n_win',10)
+        fn_dat_fft      = kwargs.get('fn_dat_fft',None)
+        
+        ## only distribute data in [y]
+        if (rx!=1):
+            raise AssertionError('rx!=1')
+        if (rz!=1):
+            raise AssertionError('rz!=1')
+        if (rt!=1):
+            raise AssertionError('rt!=1')
+        
+        ## check the choice of ranks per dimension
+        if (rx*ry*rz*rt != self.n_ranks):
+            raise AssertionError('rx*ry*rz*rt != self.n_ranks')
+        if (rx>self.nx):
+            raise AssertionError('rx>self.nx')
+        if (ry>self.ny):
+            raise AssertionError('ry>self.ny')
+        if (rz>self.nz):
+            raise AssertionError('rz>self.nz')
+        if (rt>self.nt):
+            raise AssertionError('rt>self.nt')
+        
+        # === distribute 4D data over ranks --> here only in [y]
+        
+        #comm4d = self.comm.Create_cart(dims=[rx,ry,ry,rt], periods=[False,False,False,False], reorder=False)
+        #t4d = comm4d.Get_coords(self.rank)
+        
+        #rxl_ = np.array_split(np.arange(self.nx,dtype=np.int64),min(rx,self.nx))
+        ryl_ = np.array_split(np.arange(self.ny,dtype=np.int64),min(ry,self.ny))
+        #rzl_ = np.array_split(np.arange(self.nz,dtype=np.int64),min(rz,self.nz))
+        #rtl_ = np.array_split(np.arange(self.nt,dtype=np.int64),min(rt,self.nt))
+        
+        #rxl = [[b[0],b[-1]+1] for b in rxl_ ]
+        ryl = [[b[0],b[-1]+1] for b in ryl_ ]
+        #rzl = [[b[0],b[-1]+1] for b in rzl_ ]
+        #rtl = [[b[0],b[-1]+1] for b in rtl_ ]
+        
+        #rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
+        #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
+        #rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
+        #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
+        
+        ry1,ry2 = ryl[self.rank]; nyr = ry2 - ry1
+        
+        # === fft file name (for writing) : dat
+        if (fn_dat_fft is None):
+            fname_path = os.path.dirname(self.fname)
+            fname_base = os.path.basename(self.fname)
+            fname_root, fname_ext = os.path.splitext(fname_base)
+            fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
+            fname_fft_dat_base = fname_root+'_turb_spec_2d_zt.dat'
+            fn_dat_fft = str(PurePosixPath(fname_path, fname_fft_dat_base))
+        
+        if verbose: even_print('fn_rgd_prime' , self.fname )
+        if verbose: even_print('fn_dat_fft'   , fn_dat_fft )
+        if verbose: print(72*'-')
+        
+        # ===
+        
+        if verbose: even_print('nx' , '%i'%self.nx)
+        if verbose: even_print('ny' , '%i'%self.ny)
+        if verbose: even_print('nz' , '%i'%self.nz)
+        if verbose: even_print('nt' , '%i'%self.nt)
+        if verbose: print(72*'-')
+        
+        if self.usingmpi: self.comm.Barrier()
+        
+        ## the data dictionary to be pickled later
+        data = {}
+        
+        if ('data_dim' not in self):
+            raise ValueError('group data_dim not present')
+        
+        ## put all data from 'data_dim' into the dictionary data which will be pickled at the end
+        for dsn in self['data_dim'].keys():
+            d_ = np.copy( self[f'data_dim/{dsn}'][()] )
+            if (d_.ndim == 0):
+                d_ = float(d_)
+            data[dsn] = d_
+        
+        ## 1D
+        rho_avg = np.copy( self['data_dim/rho'][()] )
+        u_avg   = np.copy( self['data_dim/u'][()]   )
+        #v_avg   = np.copy( self['data_dim/v'][()]   )
+        #w_avg   = np.copy( self['data_dim/w'][()]   )
+        #T_avg   = np.copy( self['data_dim/T'][()]   )
+        #p_avg   = np.copy( self['data_dim/p'][()]   )
+        
+        ## 0D
+        u_tau    = float( self['data_dim/u_tau'][()]    )
+        nu_wall  = float( self['data_dim/nu_wall'][()]  )
+        rho_wall = float( self['data_dim/rho_wall'][()] )
+        T_wall   = float( self['data_dim/T_wall'][()]   )
+        d99      = float( self['data_dim/d99'][()]      )
+        u_99     = float( self['data_dim/u_99'][()]     )
+        Re_tau   = float( self['data_dim/Re_tau'][()]   )
+        Re_theta = float( self['data_dim/Re_theta'][()] )
+        sc_u_in  = float( self['data_dim/sc_u_in'][()]  )
+        sc_l_in  = float( self['data_dim/sc_l_in'][()]  )
+        sc_t_in  = float( self['data_dim/sc_t_in'][()]  )
+        sc_u_out = float( self['data_dim/sc_u_out'][()] )
+        sc_l_out = float( self['data_dim/sc_l_out'][()] )
+        sc_t_out = float( self['data_dim/sc_t_out'][()] )
+        
+        ## 0D scalars
+        lchar   = self.lchar   ; data['lchar']   = lchar
+        U_inf   = self.U_inf   ; data['U_inf']   = U_inf
+        rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
+        T_inf   = self.T_inf   ; data['T_inf']   = T_inf
+        
+        #data['M_inf'] = self.M_inf
+        data['Ma'] = self.Ma
+        data['Pr'] = self.Pr
+        
+        ## read in 1D coordinate arrays, then re-dimensionalize [m]
+        x = np.copy( self['dims/x'][()] * self.lchar )
+        y = np.copy( self['dims/y'][()] * self.lchar )
+        z = np.copy( self['dims/z'][()] * self.lchar )
+        t = np.copy( self['dims/t'][()] * self.tchar )
+        
+        ## dimensional [s]
+        dt = self.dt * self.tchar
+        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-14, atol=1e-14)
+        
+        t_meas = self.duration * self.tchar
+        np.testing.assert_allclose(t_meas, t.max()-t.min(), rtol=1e-14, atol=1e-14)
+        
+        t_eddy = t_meas / ( d99 / u_tau )
+        
+        ## check if constant Δz (calculate Δz+ later)
+        dz0 = np.diff(z)[0]
+        if not np.all(np.isclose(np.diff(z), dz0, rtol=1e-7)):
+            raise NotImplementedError
+        np.testing.assert_allclose(dz0, z[1]-z[0], rtol=1e-14, atol=1e-14)
+        
+        zrange = z.max() - z.min()
+        np.testing.assert_allclose(zrange, z[-1]-z[0], rtol=1e-14, atol=1e-14)
+        
+        nx = self.nx ; data['nx'] = nx
+        ny = self.ny ; data['ny'] = ny
+        nz = self.nz ; data['nz'] = nz
+        nt = self.nt ; data['nt'] = nt
+        
+        ## add data to dict that gets output
+        data['x'] = x
+        data['y'] = y
+        data['z'] = z
+        data['t'] = t
+        data['t_meas'] = t_meas
+        data['dt'] = dt
+        data['dz0'] = dz0
+        data['zrange'] = zrange
+        
+        if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
+        if verbose: even_print('Δt','%0.3e [s]'%(dt,))
+        if verbose: even_print('duration/tchar','%0.1f'%(self.duration,))
+        if verbose: even_print('duration','%0.3e [s]'%(self.duration*self.tchar,))
+        if verbose: print(72*'-')
+        
+        ## report
+        if verbose:
+            even_print('dt'     , '%0.5e [s]' % dt      )
+            even_print('t_meas' , '%0.5e [s]' % t_meas  )
+            even_print('dz0'    , '%0.5e [m]' % dz0     )
+            even_print('zrange' , '%0.5e [m]' % zrange  )
+            print(72*'-')
+        
+        ## report
+        if verbose:
+            even_print('Re_τ'    , '%0.1f'        % Re_tau    )
+            even_print('Re_θ'    , '%0.1f'        % Re_theta  )
+            even_print('δ99'     , '%0.5e [m]'    % d99       )
+            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in )
+            even_print('U_inf'  , '%0.3f [m/s]'   % self.U_inf )
+            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau     )
+            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall   )
+            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall  )
+            ##
+            even_print( 'Δz+'        , '%0.3f'%(dz0/sc_l_in) )
+            even_print( 'zrange/δ99' , '%0.3f'%(zrange/d99)  )
+            even_print( 'Δt+'        , '%0.3f'%(dt/sc_t_in)  )
+            print(72*'-')
+        
+        ## report
+        if verbose:
+            even_print('t_meas/(δ99/u_τ) = t_eddy' , '%0.2f'%t_eddy)
+            even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99/u_99)))
+            even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99/u_99)))
+            print(72*'-')
+        
+        # ===
+        
+        ## establish fft (time) windowing
+        win_len, overlap = get_overlapping_window_size(nt, n_win, overlap_fac_nom)
+        overlap_fac = overlap / win_len
+        tw, n_win, n_pad = get_overlapping_windows(t, win_len, overlap)
+        
+        data['win_len']     = win_len
+        data['overlap_fac'] = overlap_fac
+        data['overlap']     = overlap
+        data['n_win']       = n_win
+        
+        t_meas_per_win = (win_len-1)*dt
+        t_eddy_per_win = t_meas_per_win / (d99/u_tau)
+        
+        data['t_eddy_per_win'] = t_eddy_per_win
+        
+        if verbose:
+            even_print('overlap_fac (nominal)' , '%0.5f'%overlap_fac_nom    )
+            even_print('n_win'                 , '%i'%n_win                 )
+            even_print('win_len'               , '%i'%win_len               )
+            even_print('overlap'               , '%i'%overlap               )
+            even_print('overlap_fac'           , '%0.5f'%overlap_fac        )
+            even_print('n_pad'                 , '%i'%n_pad                 )
+            even_print('t_win/(δ99/u_τ)'       , '%0.3f [-]'%t_eddy_per_win )
+            print(72*'-')
+        
+        ## get frequency vector --> here for short time FFT, i.e. for [t] signal broken into overlapping segments
+        freq_full = sp.fft.fftfreq(n=win_len, d=dt)
+        fp        = np.where(freq_full>0)
+        freq      = np.copy(freq_full[fp])
+        df        = freq[1]-freq[0]
+        nf        = freq.size
+        
+        data['freq'] = freq
+        data['df']   = df
+        data['nf']   = nf
+        data['fp']   = fp ## tmp
+        data['freq_full'] = freq_full ## tmp
+        
+        # λx = u/f
+        # kx = 2·π·f/u
+        # ---
+        # λx/δ99
+        # λx+ = λx/(ν/u_tau)
+        # kx·δ99
+        # kx+ = (2·π·f/u)·(ν/u_tau)
+        
+        ## get wavenumber vector/array [x]
+        
+        na = np.newaxis
+        
+        ## prevent zeros since later we divide by wall u to get kx
+        u_avg[0] = u_avg[1]*1e-6
+        
+        ## kx = 2·π·f/u --> shape=(ny,nf)
+        kx = np.copy( 2*np.pi*freq[na,:]/u_avg[:,na] )
+        kx_full = np.copy( 2*np.pi*freq_full[na,:]/u_avg[:,na] ) ## tmp
+        
+        ## λx = u/f --> shape=(ny,nf)
+        lx = np.copy( u_avg[:,na]/freq[na,:] )
+        lx_full = np.copy( u_avg[:,na]/freq_full[na,:] ) ## tmp
+        
+        data['kx']  = kx
+        data['kx_full'] = kx_full ## tmp
+        data['lx'] = lx
+        data['lx_full'] = lx_full ## tmp
+        
+        ## get wavenumber vector [z]
+        kz_full = sp.fft.fftfreq(n=nz, d=dz0) * ( 2 * np.pi )
+        kzp     = np.where(kz_full>0)
+        kz      = np.copy(kz_full[kzp])
+        dkz     = kz[1]-kz[0]
+        nkz     = kz.size
+        
+        data['kz']  = kz
+        data['dkz'] = dkz
+        data['nkz'] = nkz
+        data['kzp'] = kzp ## tmp
+        data['kz_full'] = kz_full ## tmp
+        
+        ## λz = (2·π)/kz
+        lz = np.copy( 2 * np.pi / kz )
+        lz_full = np.copy( 2 * np.pi / kz_full ) ## tmp
+        data['lz'] = lz
+        data['lz_full'] = lz_full ## tmp
+        
+        if verbose:
+            even_print('freq min','%0.1f [Hz]'%freq.min())
+            even_print('freq max','%0.1f [Hz]'%freq.max())
+            even_print('df','%0.1f [Hz]'%df)
+            even_print('nf','%i'%nf)
+            
+            period_eddy = (1/freq) / (d99/u_tau)
+            period_plus = (1/freq) / sc_t_in
+            even_print('min : period+ = (1/f)/(ν_wall/u_τ²)'   , '%0.5f [-]'%period_plus.min())
+            even_print('max : period+ = (1/f)/(ν_wall/u_τ²)'   , '%0.5f [-]'%period_plus.max())
+            even_print('min : period_eddy = (1/f)/(d99/u_tau)' , '%0.5e [-]'%period_eddy.min())
+            even_print('max : period_eddy = (1/f)/(d99/u_tau)' , '%0.5f [-]'%period_eddy.max())
+            
+            print(72*'-')
+        
+        if verbose:
+            even_print('kz min','%0.1f [1/m]'%kz.min())
+            even_print('kz max','%0.1f [1/m]'%kz.max())
+            even_print('dkz','%0.1f [1/m]'%dkz)
+            even_print('nkz','%i'%nkz)
+            
+            kz_inner = np.copy( kz * sc_l_in  )
+            kz_outer = np.copy( kz * sc_l_out )
+            
+            even_print('min : (kz·δ_ν) ' , '%0.5e [-]'%kz_inner.min())
+            even_print('max : (kz·δ_ν) ' , '%0.5f [-]'%kz_inner.max())
+            even_print('min : (kz·δ99) ' , '%0.5f [-]'%kz_outer.min())
+            even_print('max : (kz·δ99) ' , '%0.5e [-]'%kz_outer.max())
+            
+            print(72*'-')
+        
+        kzp2d,fp2d = np.meshgrid(kzp,fp, indexing='ij')
+        
+        if self.usingmpi: self.comm.Barrier()
+        
+        # ===
+        
+        if True: ## just a test currently --> not finished!!!
+            
+            yp_tgt = 100.
+            yp = np.copy( y / sc_l_in )
+            yi = np.abs(yp-yp_tgt).argmin()
+            
+            dd = np.copy( self.U_inf * self['data/uI'][:win_len,:,yi,0].T )
+            #print(dd.shape)
+            
+            A_ui = sp.fft.fftn(dd) # [kzp2d, fp2d]
+            A_uj = sp.fft.fftn(dd) # [kzp2d, fp2d]
+            data['A_ui'] = A_ui
+            data['A_uj'] = A_uj
+            
+            #Euu_ijk = np.copy(  2 * np.real(A_ui*np.conj(A_uj)) / ( df * dkz ) )
+            #data['Euu'] = Euu_ijk
+        
+        # === save results
+        if (self.rank==0):
+            
+            #data['Euu']      = Euu_avg
+            #data['uIuI_avg'] = uIuI_avg
+            
+            with open(fn_dat_fft,'wb') as f:
+                pickle.dump(data, f, protocol=4)
+            print('--w-> %s : %0.2f [MB]'%(fn_dat_fft,os.path.getsize(fn_dat_fft)/1024**2))
+        
+        # ===
+        
+        if self.usingmpi: self.comm.Barrier()
+        
+        if verbose: print(72*'-')
+        if verbose: print('total time : rgd.calc_turb_spectrum_2d_span_time() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
         return
     
     def calc_ccor_time(self, **kwargs):
         '''
         calculate cross-correlation in [t] and avg in [x,z] --> leave [y,Δt]
         - designed for analyzing unsteady, thin planes in [x]
         '''
@@ -14422,15 +15317,15 @@
         #rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
         #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
         #rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
         #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
         
         rt1,rt2 = rtl[self.rank]; ntr = rt2 - rt1
         
-        # === [t] sub chunk range --> ctl = list of ranges in rt1:rt2
+        ## [t] sub chunk range --> ctl = list of ranges in rt1:rt2
         ctl_ = np.array_split( np.arange(rt1,rt2) , min(ct,ntr) )
         ctl = [[b[0],b[-1]+1] for b in ctl_ ]
         
         ## check that no sub ranges are <=1
         for a_ in [ ctl_[1]-ctl_[0] for ctl_ in ctl ]:
             if (a_ <= 1):
                 raise ValueError
@@ -14763,15 +15658,14 @@
                 unsteady_transport_sum    = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
                 unsteady_diffusion_sum    = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
                 unsteady_p_diffusion_sum  = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
                 unsteady_p_dilatation_sum = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
                 
                 # === main loop (iterate through sub-ranges within rank-distributed [t] range)
                 
-                ## main loop --> cross-correlation in [Δz] at every [x,y,t]
                 if verbose:
                     progress_bar = tqdm(total=ct, ncols=100, desc='turb budget', leave=False, file=sys.stdout)
                 
                 ct_counter=0
                 for ctl_ in ctl:
                     ct_counter += 1
                     ct1, ct2 = ctl_
@@ -17212,39 +18106,100 @@
             self.n_ranks = self.comm.Get_size()
             self.rank    = self.comm.Get_rank()
         else:
             self.comm    = None
             self.n_ranks = 1
             self.rank    = 0
         
-        ## determine MPI info / hints
+        ## ztmd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
+        stripe_count   = kwargs.pop('stripe_count'   , 16    )
+        stripe_size_mb = kwargs.pop('stripe_size_mb' , 8     )
+        perms          = kwargs.pop('stripe_size_mb' , '640' )
+        
+        if not isinstance(stripe_count, int):
+            raise ValueError
+        if not isinstance(stripe_size_mb, int):
+            raise ValueError
+        if not isinstance(perms, str):
+            raise ValueError
+        if not len(perms)==3:
+            raise ValueError
+        if not re.fullmatch(r'\d{3}',perms):
+            raise ValueError
+        
+        ## if not using MPI, remove 'driver' and 'comm' from kwargs
+        if ( not self.usingmpi ) and ('driver' in kwargs):
+            kwargs.pop('driver')
+        if ( not self.usingmpi ) and ('comm' in kwargs):
+            kwargs.pop('comm')
+        
+        ## | mpiexec --mca io romio321 -n $NP python3 ...
+        ## | mpiexec --mca io ompio -n $NP python3 ...
+        ## | ompi_info --> print ompi settings (grep 'MCA io' for I/O opts)
+        ## | export ROMIO_FSTYPE_FORCE="lustre:" --> force Lustre driver over UFS when using romio --> causes crash
+        ## | export ROMIO_FSTYPE_FORCE="ufs:"
+        ## | export ROMIO_PRINT_HINTS=1 --> show available hints
+        ##
+        ## https://doku.lrz.de/best-practices-hints-and-optimizations-for-io-10747318.html
+        ##
+        ## OMPIO
+        ## export OMPI_MCA_sharedfp=^lockedfile,individual
+        ## mpiexec --mca io ompio -n $NP python3 script.py
+        
+        ## set ROMIO hints, passed through 'mpi_info' dict
         if self.usingmpi:
             if ('info' in kwargs):
                 self.mpi_info = kwargs['info']
             else:
                 mpi_info = MPI.Info.Create()
                 ##
                 mpi_info.Set('romio_ds_write' , 'disable'   )
                 mpi_info.Set('romio_ds_read'  , 'disable'   )
                 mpi_info.Set('romio_cb_read'  , 'automatic' )
                 mpi_info.Set('romio_cb_write' , 'automatic' )
                 #mpi_info.Set('romio_cb_read'  , 'enable' )
                 #mpi_info.Set('romio_cb_write' , 'enable' )
-                mpi_info.Set('cb_buffer_size' , str(int(round(8*1024**2))) ) ## 8 [MB]
+                mpi_info.Set('cb_buffer_size' , str(int(round(16*1024**2))) ) ## 16 [MB]
+                ##
+                #mpi_info.Set('romio_no_indep_rw' , 'true' ) ## deferred open + only collective I/O 
+                #mpi_info.Set('cb_nodes' , str(int(round(1*self.n_ranks))) )
                 ##
                 kwargs['info'] = mpi_info
                 self.mpi_info = mpi_info
         
+        ## | rdcc_nbytes:
+        ## | ------------
+        ## | Integer setting the total size of the raw data chunk cache for this dataset in bytes.
+        ## | In most cases increasing this number will improve performance, as long as you have 
+        ## | enough free memory. The default size is 1 MB
+        
+        ## --> gets passed to H5Pset_chunk_cache
         if ('rdcc_nbytes' not in kwargs):
             kwargs['rdcc_nbytes'] = int(16*1024**2) ## 16 [MB]
         
+        ## | rdcc_nslots:
+        ## | ------------
+        ## | Integer defining the number of chunk slots in the raw data chunk cache for this dataset.
+        
+        ## if ('rdcc_nslots' not in kwargs):
+        ##     kwargs['rdcc_nslots'] = 521
+        
         ## ztmd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
-        verbose = kwargs.pop('verbose',False)
-        force   = kwargs.pop('force',False)
+        verbose = kwargs.pop( 'verbose' , False )
+        force   = kwargs.pop( 'force'   , False )
         
+        if not isinstance(verbose, bool):
+            raise ValueError
+        if not isinstance(force, bool):
+            raise ValueError
+        
+        # === initialize file on FS
+        
+        ## if file open mode is 'w', the file exists, and force is False
+        ## --> raise error
         if (self.open_mode == 'w') and (force is False) and os.path.isfile(self.fname):
             if (self.rank==0):
                 print('\n'+72*'-')
                 print(self.fname+' already exists! opening with \'w\' would overwrite.\n')
                 openModeInfoStr = '''
                                   r       --> Read only, file must exist
                                   r+      --> Read/write, file must exist
@@ -17255,43 +18210,38 @@
                                   or use force=True arg:
                                   
                                   >>> with ztmd(<<fname>>,'w',force=True) as f:
                                   >>>     ...
                                   '''
                 print(textwrap.indent(textwrap.dedent(openModeInfoStr), 2*' ').strip('\n'))
                 print(72*'-'+'\n')
+                sys.stdout.flush()
             
             if (self.comm is not None):
                 self.comm.Barrier()
             raise FileExistsError()
         
-        ## remove file, touch, stripe
-        elif (self.open_mode == 'w') and (force is True) and os.path.isfile(self.fname):
-            if (self.rank==0):
-                os.remove(self.fname)
-                Path(self.fname).touch()
-                if shutil.which('lfs') is not None:
-                    return_code = subprocess.call('lfs migrate --stripe-count 16 --stripe-size 8M %s > /dev/null 2>&1'%self.fname, shell=True)
-                else:
-                    #print('striping with lfs not permitted on this filesystem')
-                    pass
-        
-        ## touch, stripe
-        elif (self.open_mode == 'w') and not os.path.isfile(self.fname):
+        ## if file open mode is 'w'
+        ## --> <delete>, touch, chmod, stripe
+        if (self.open_mode == 'w'):
             if (self.rank==0):
-                Path(self.fname).touch()
-                if shutil.which('lfs') is not None:
-                    return_code = subprocess.call('lfs migrate --stripe-count 16 --stripe-size 8M %s > /dev/null 2>&1'%self.fname, shell=True)
+                if os.path.isfile(self.fname): ## if the file exists, delete it
+                    os.remove(self.fname)
+                    time.sleep(0.1)
+                Path(self.fname).touch() ## touch a new file
+                os.chmod(self.fname, int(perms, base=8)) ## change permissions
+                if shutil.which('lfs') is not None: ## set stripe if on Lustre
+                    cmd_str_lfs_migrate = f'lfs migrate --stripe-count {stripe_count:d} --stripe-size {stripe_size_mb:d}M {self.fname} > /dev/null 2>&1'
+                    return_code = subprocess.call(cmd_str_lfs_migrate, shell=True)
+                    if (return_code != 0):
+                        raise ValueError('lfs migrate failed')
                 else:
                     #print('striping with lfs not permitted on this filesystem')
                     pass
         
-        else:
-            pass
-        
         if (self.comm is not None):
             self.comm.Barrier()
         
         self.mod_avail_tqdm = ('tqdm' in sys.modules)
         
         ## call actual h5py.File.__init__()
         super(ztmd, self).__init__(*args, **kwargs)
@@ -17511,14 +18461,23 @@
                 self.yy = np.copy( self.y   )
             else:
                 raise ValueError
         
         if ('dz' in self.attrs.keys()):
             self.dz = self.attrs['dz']
         
+        if ('dims/stang' in self):
+            self.stang = np.copy( self['dims/stang'][()] )
+        if ('dims/snorm' in self):
+            self.snorm = np.copy( self['dims/snorm'][()] )
+        if ('dims/crv_R' in self):
+            self.crv_R = np.copy( self['dims/crv_R'][()] )
+        if ('dims/R_min' in self):
+            self.R_min = self['dims/R_min'][()]
+        
         if verbose: print(72*'-')
         if verbose and hasattr(self,'duration_avg'): even_print('duration_avg', '%0.5f'%self.duration_avg)
         if verbose: even_print('nx', '%i'%self.nx)
         if verbose: even_print('ny', '%i'%self.ny)
         #if verbose: print(72*'-')
         
         # ===
@@ -18042,14 +19001,34 @@
                 r_rII_rII   = data_mean["r r''r''"]   * rho_inf * rho_inf**2
                 r_muII_muII = data_mean["r mu''mu''"] * rho_inf * mu_inf**2
                 ##
                 self.create_dataset('data/r_TII_TII',   data=r_TII_TII.T,   chunks=None)
                 self.create_dataset('data/r_pII_pII',   data=r_pII_pII.T,   chunks=None)
                 self.create_dataset('data/r_rII_rII',   data=r_rII_rII.T,   chunks=None)
                 self.create_dataset('data/r_muII_muII', data=r_muII_muII.T, chunks=None)
+                
+                # === RMS
+                
+                if True:
+                    
+                    r_uII_uII_rms = np.sqrt(       data_mean["r u''u''"]  * rho_inf * U_inf**2 )
+                    r_vII_vII_rms = np.sqrt(       data_mean["r v''v''"]  * rho_inf * U_inf**2 )
+                    r_wII_wII_rms = np.sqrt(       data_mean["r w''_w''"] * rho_inf * U_inf**2 )
+                    r_uII_vII_rms = np.sqrt(np.abs(data_mean["r u''v''"]) * rho_inf * U_inf**2 ) * np.sign(data_mean["r u''v''"]) 
+                    r_uII_wII_rms = np.sqrt(np.abs(data_mean["r u''w''"]) * rho_inf * U_inf**2 ) * np.sign(data_mean["r u''w''"])
+                    r_vII_wII_rms = np.sqrt(np.abs(data_mean["r w''v''"]) * rho_inf * U_inf**2 ) * np.sign(data_mean["r w''v''"])
+                    ## ... rho*u''T''
+                    
+                    self.create_dataset( 'data/r_uII_uII_rms' , data=r_uII_uII_rms.T , chunks=None )
+                    self.create_dataset( 'data/r_vII_vII_rms' , data=r_vII_vII_rms.T , chunks=None )
+                    self.create_dataset( 'data/r_wII_wII_rms' , data=r_wII_wII_rms.T , chunks=None )
+                    self.create_dataset( 'data/r_uII_vII_rms' , data=r_uII_vII_rms.T , chunks=None )
+                    self.create_dataset( 'data/r_uII_wII_rms' , data=r_uII_wII_rms.T , chunks=None )
+                    self.create_dataset( 'data/r_vII_wII_rms' , data=r_vII_wII_rms.T , chunks=None )
+                    ## ... rho*u''T''
         
         if fn_turb_budget.exists():
             #print('--r-> %s'%fn_turb_budget.relative_to(Path()) )
             even_print('eas4 turb budget',str(fn_turb_budget.relative_to(Path())))
             with eas4(str(fn_turb_budget),'r',verbose=False) as f1:
                 
                 data_mean = f1.get_mean() ## numpy structured array
@@ -18183,15 +19162,17 @@
     # ===
     
     def calc_gradients(self, acc=6, edge_stencil='full', **kwargs):
         '''
         calculate spatial gradients of averaged quantities
         '''
         
-        verbose = kwargs.get('verbose',True)
+        verbose  = kwargs.get('verbose',True)
+        do_favre = kwargs.get('favre',True)
+        
         if verbose: print('\n'+'ztmd.calc_gradients()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
         
         if verbose: even_print('acc','%i'%(acc,))
         if verbose: even_print('edge_stencil','%s'%(edge_stencil,))
         
         ## check
@@ -18242,14 +19223,16 @@
             
             ## the 'computational' grid (unit Cartesian)
             #x_comp = np.arange(nx, dtype=np.float64)
             #y_comp = np.arange(ny, dtype=np.float64)
             x_comp = 1.
             y_comp = 1.
         
+        print(72*'-')
+        
         # === get gradients of [u,v,p,T,ρ]
         
         if ('data/u' in self):
             
             u = np.copy( self['data/u'][()].T )
             
             if self.rectilinear:
@@ -18428,14 +19411,68 @@
             dset = self.create_dataset('data/ddx_unorm', data=ddx_unorm.T, chunks=None)
             if verbose: even_print('ddx[unorm]','%s'%str(ddx_unorm.shape))
             
             if ('data/ddy_unorm' in self): del self['data/ddy_unorm']
             dset = self.create_dataset('data/ddy_unorm', data=ddy_unorm.T, chunks=None)
             if verbose: even_print('ddy[unorm]','%s'%str(ddy_unorm.shape))
         
+        # === Favre
+        
+        if do_favre:
+            
+            print(72*'-')
+            
+            if ('data/u_Fv' in self):
+                
+                u_Fv = np.copy( self['data/u_Fv'][()].T )
+                
+                if self.rectilinear:
+                    ddx_u_Fv = gradient(u_Fv, self.x, axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+                    ddy_u_Fv = gradient(u_Fv, self.y, axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+                elif self.curvilinear:
+                    ddx_u_Fv_comp = gradient(u_Fv, x_comp, axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+                    ddy_u_Fv_comp = gradient(u_Fv, y_comp, axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+                    ddx_u_Fv      = ddx_u_Fv_comp*ddx_q1 + ddy_u_Fv_comp*ddx_q2
+                    ddy_u_Fv      = ddx_u_Fv_comp*ddy_q1 + ddy_u_Fv_comp*ddy_q2
+                else:
+                    raise ValueError
+                
+                if ('data/ddx_u_Fv' in self): del self['data/ddx_u_Fv']
+                self.create_dataset('data/ddx_u_Fv', data=ddx_u_Fv.T, chunks=None)
+                
+                if ('data/ddy_u_Fv' in self): del self['data/ddy_u_Fv']
+                self.create_dataset('data/ddy_u_Fv', data=ddy_u_Fv.T, chunks=None)
+                
+                if verbose: even_print('ddx[u_Fv]','%s'%str(ddx_u_Fv.shape))
+                if verbose: even_print('ddy[u_Fv]','%s'%str(ddy_u_Fv.shape))
+            
+            if ('data/v_Fv' in self):
+                
+                v_Fv = np.copy( self['data/v_Fv'][()].T )
+                
+                if self.rectilinear:
+                    ddx_v_Fv = gradient(v_Fv, self.x, axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+                    ddy_v_Fv = gradient(v_Fv, self.y, axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+                elif self.curvilinear:
+                    ddx_v_Fv_comp = gradient(v_Fv, x_comp, axis=0, acc=acc, edge_stencil=edge_stencil, d=1)
+                    ddy_v_Fv_comp = gradient(v_Fv, y_comp, axis=1, acc=acc, edge_stencil=edge_stencil, d=1)
+                    ddx_v_Fv      = ddx_v_Fv_comp*ddx_q1 + ddy_v_Fv_comp*ddx_q2
+                    ddy_v_Fv      = ddx_v_Fv_comp*ddy_q1 + ddy_v_Fv_comp*ddy_q2
+                else:
+                    raise ValueError
+                
+                if ('data/ddx_v_Fv' in self): del self['data/ddx_v_Fv']
+                self.create_dataset('data/ddx_v_Fv', data=ddx_v_Fv.T, chunks=None)
+                
+                if ('data/ddy_v_Fv' in self): del self['data/ddy_v_Fv']
+                self.create_dataset('data/ddy_v_Fv', data=ddy_v_Fv.T, chunks=None)
+                
+                if verbose: even_print('ddx[v_Fv]','%s'%str(ddx_v_Fv.shape))
+                if verbose: even_print('ddy[v_Fv]','%s'%str(ddy_v_Fv.shape))
+        
         self.get_header(verbose=False)
         if verbose: print(72*'-')
         if verbose: print('total time : ztmd.calc_gradients() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
@@ -18888,57 +19925,98 @@
         if not ('csys/vtang' in self):
             raise ValueError('csys/vtang not in hdf5')
         if not ('csys/vnorm' in self):
             raise ValueError('csys/vnorm not in hdf5')
         if not (self.open_mode=='a') or (self.open_mode=='w'):
             raise ValueError('not able to write to hdf5 file')
         
-        ## read 2D velocities
-        u  = np.copy( self['data/u'][()].T )
-        v  = np.copy( self['data/v'][()].T )
-        uv = np.stack((u,v), axis=-1)
-        
-        umag1 = np.copy( np.sqrt( u**2 + v**2 ) )
-        
         ## read unit vectors (wall tangent, wall norm) from HDF5
         vtang = np.copy( self['csys/vtang'][()] )
         vnorm = np.copy( self['csys/vnorm'][()] )
         
-        ## inner product of velocity vector and basis vector (csys transform)
-        utang = np.einsum('xyi,xyi->xy', vtang, uv)
-        unorm = np.einsum('xyi,xyi->xy', vnorm, uv)
-        
-        umag2 = np.copy( np.sqrt( utang**2 + unorm**2 ) )
-        
-        if (umag1.dtype==np.dtype(np.float32)):
-            np.testing.assert_allclose(umag1, umag2, rtol=1e-6) ## single precision
-        elif (umag2.dtype==np.dtype(np.float64)):
-            np.testing.assert_allclose(umag1, umag2, rtol=1e-12) ## double precision
-        else:
-            raise ValueError
-        
-        # if self.get('data/u').attrs['dimensional']:
-        #     raise AssertionError('u is dimensional')
-        # if self.get('data/v').attrs['dimensional']:
-        #     raise AssertionError('v is dimensional')
+        # === Reynolds
         
-        if ('data/utang' in self): del self['data/utang']
-        dset = self.create_dataset('data/utang', data=utang.T, chunks=None)
-        #dset.attrs['dimensional'] = False
-        if verbose: even_print('utang','%s'%str(utang.shape))
+        if ('data/u' in self) and ('data/v' in self):
+            
+            ## read 2D velocities
+            u  = np.copy( self['data/u'][()].T )
+            v  = np.copy( self['data/v'][()].T )
+            uv = np.stack((u,v), axis=-1)
+            
+            umag1 = np.copy( np.sqrt( u**2 + v**2 ) )
+            
+            ## inner product of velocity vector and basis vector (csys transform)
+            utang = np.einsum('xyi,xyi->xy', vtang, uv)
+            unorm = np.einsum('xyi,xyi->xy', vnorm, uv)
+            
+            umag2 = np.copy( np.sqrt( utang**2 + unorm**2 ) )
+            
+            if (umag1.dtype==np.dtype(np.float32)):
+                np.testing.assert_allclose(umag1, umag2, rtol=1e-6) ## single precision
+            elif (umag2.dtype==np.dtype(np.float64)):
+                np.testing.assert_allclose(umag1, umag2, rtol=1e-12) ## double precision
+            else:
+                raise ValueError
+            
+            # if self.get('data/u').attrs['dimensional']:
+            #     raise AssertionError('u is dimensional')
+            # if self.get('data/v').attrs['dimensional']:
+            #     raise AssertionError('v is dimensional')
+            
+            if ('data/utang' in self): del self['data/utang']
+            dset = self.create_dataset('data/utang', data=utang.T, chunks=None)
+            #dset.attrs['dimensional'] = False
+            if verbose: even_print('utang','%s'%str(utang.shape))
+            
+            if ('data/unorm' in self): del self['data/unorm']
+            dset = self.create_dataset('data/unorm', data=unorm.T, chunks=None)
+            #dset.attrs['dimensional'] = False
+            if verbose: even_print('unorm','%s'%str(unorm.shape))
+            
+            ## assert that in rectilinear case that u==utang & v==unorm
+            if self.rectilinear:
+                np.testing.assert_allclose(u, utang, rtol=1e-14, atol=1e-14)
+                np.testing.assert_allclose(v, unorm, rtol=1e-14, atol=1e-14)
         
-        if ('data/unorm' in self): del self['data/unorm']
-        dset = self.create_dataset('data/unorm', data=unorm.T, chunks=None)
-        #dset.attrs['dimensional'] = False
-        if verbose: even_print('unorm','%s'%str(unorm.shape))
+        # === Favre
         
-        ## check
-        if self.rectilinear:
-            np.testing.assert_allclose(u, utang, rtol=1e-14, atol=1e-14)
-            np.testing.assert_allclose(v, unorm, rtol=1e-14, atol=1e-14)
+        if ('data/u_Fv' in self) and ('data/v_Fv' in self):
+            
+            ## read 2D velocities
+            u_Fv     = np.copy( self['data/u_Fv'][()].T )
+            v_Fv     = np.copy( self['data/v_Fv'][()].T )
+            uv_Fv    = np.stack((u_Fv,v_Fv), axis=-1)
+            umag1_Fv = np.copy( np.sqrt( u_Fv**2 + v_Fv**2 ) )
+            
+            ## inner product of velocity vector and basis vector (csys transform)
+            utang_Fv = np.einsum('xyi,xyi->xy', vtang, uv_Fv)
+            unorm_Fv = np.einsum('xyi,xyi->xy', vnorm, uv_Fv)
+            
+            umag2_Fv = np.copy( np.sqrt( utang_Fv**2 + unorm_Fv**2 ) )
+            
+            if (umag1_Fv.dtype==np.dtype(np.float32)):
+                np.testing.assert_allclose(umag1_Fv, umag2_Fv, rtol=1e-6) ## single precision
+            elif (umag2_Fv.dtype==np.dtype(np.float64)):
+                np.testing.assert_allclose(umag1_Fv, umag2_Fv, rtol=1e-12) ## double precision
+            else:
+                raise ValueError
+            
+            if ('data/utang_Fv' in self): del self['data/utang_Fv']
+            dset = self.create_dataset('data/utang_Fv', data=utang_Fv.T, chunks=None)
+            if verbose: even_print('utang_Fv','%s'%str(utang_Fv.shape))
+            
+            if ('data/unorm_Fv' in self): del self['data/unorm_Fv']
+            dset = self.create_dataset('data/unorm_Fv', data=unorm_Fv.T, chunks=None)
+            #dset.attrs['dimensional'] = False
+            if verbose: even_print('unorm_Fv','%s'%str(unorm_Fv.shape))
+            
+            ## assert that in rectilinear case that u==utang & v==unorm
+            if self.rectilinear:
+                np.testing.assert_allclose(u_Fv, utang_Fv, rtol=1e-14, atol=1e-14)
+                np.testing.assert_allclose(v_Fv, unorm_Fv, rtol=1e-14, atol=1e-14)
         
         self.get_header(verbose=False)
         if verbose: print(72*'-')
         if verbose: print('total time : ztmd.calc_vel_tangnorm() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
@@ -18963,349 +20041,237 @@
         if not ('csys/vtang' in self):
             raise ValueError('csys/vtang not in hdf5')
         if not ('csys/vnorm' in self):
             raise ValueError('csys/vnorm not in hdf5')
         if not (self.open_mode=='a') or (self.open_mode=='w'):
             raise ValueError('not able to write to hdf5 file')
         
-        uI_uI = np.copy( self['data/uI_uI'][()].T )
-        vI_vI = np.copy( self['data/vI_vI'][()].T )
-        uI_vI = np.copy( self['data/uI_vI'][()].T )
-        vI_uI = np.copy( uI_vI )
-        
-        ## construct 2D tensor --> (nx,ny,2,2)
-        uIuI_ij = np.stack( (np.stack( [uI_uI, uI_vI], axis=-1 ),
-                             np.stack( [vI_uI, vI_vI], axis=-1 )), axis=-1 )
-        
-        #uIuI_ij = np.transpose(uIuI_ij, (0,1,3,2))
-        
-        uI_uI_rms = np.copy( self['data/uI_uI_rms'][()].T )
-        vI_vI_rms = np.copy( self['data/vI_vI_rms'][()].T )
-        uI_vI_rms = np.copy( self['data/uI_vI_rms'][()].T )
-        vI_uI_rms = np.copy( uI_vI_rms )
-        
-        ## construct 2D tensor --> (nx,ny,2,2)
-        uIuI_rms_ij = np.stack( (np.stack( [uI_uI_rms, uI_vI_rms], axis=-1 ),
-                                 np.stack( [vI_uI_rms, vI_vI_rms], axis=-1 )), axis=-1 )
-        
-        #uIuI_rms_ij = np.transpose(uIuI_rms_ij, (0,1,3,2))
-        
-        ## check
-        np.testing.assert_allclose(uI_uI, uI_uI_rms**2, rtol=1e-6, atol=1e-6)
-        np.testing.assert_allclose(vI_vI, vI_vI_rms**2, rtol=1e-6, atol=1e-6)
-        
         ## read unit vectors (wall tangent, wall norm) from HDF5
         vtang = np.copy( self['csys/vtang'][()] )
         vnorm = np.copy( self['csys/vnorm'][()] )
         trafo = np.stack((vtang,vnorm),axis=-1)
         
         ## transpose [2,2] matrix at every [x,y]
         trafoT = np.transpose(trafo,(0,1,3,2))
         
-        ## these three ops are the same
-        #uIuI_ij_tn_A = np.einsum('xyij,xyjk,xykl->xyil', trafoT, uIuI_ij, trafo)
-        #uIuI_ij_tn_B = np.einsum('xyji,xyjk,xykl->xyil', trafo,  uIuI_ij, trafo)
-        #uIuI_ij_tn_C = np.matmul(np.matmul(trafoT, uIuI_ij), trafo)
-        #np.testing.assert_allclose(uIuI_ij_tn_A, uIuI_ij_tn_B, atol=1e-14, rtol=1e-14)
-        #np.testing.assert_allclose(uIuI_ij_tn_B, uIuI_ij_tn_C, atol=1e-14, rtol=1e-14)
-        
-        uIuI_ij_tn     = np.einsum('xyji,xyjk,xykl->xyil', trafo, uIuI_ij,     trafo)
-        uIuI_rms_ij_tn = np.einsum('xyji,xyjk,xykl->xyil', trafo, uIuI_rms_ij, trafo)
-        
-        utI_utI = np.copy(uIuI_ij_tn[:,:,0,0])
-        unI_unI = np.copy(uIuI_ij_tn[:,:,1,1])
-        utI_unI = np.copy(uIuI_ij_tn[:,:,0,1])
-        unI_utI = np.copy(uIuI_ij_tn[:,:,1,0])
-        
-        np.testing.assert_allclose( utI_unI, unI_utI, rtol=1e-14, atol=1e-14 )
-        
-        utI_utI_rms = np.copy(uIuI_rms_ij_tn[:,:,0,0])
-        unI_unI_rms = np.copy(uIuI_rms_ij_tn[:,:,1,1])
-        utI_unI_rms = np.copy(uIuI_rms_ij_tn[:,:,0,1])
-        unI_utI_rms = np.copy(uIuI_rms_ij_tn[:,:,1,0])
-        
-        np.testing.assert_allclose( utI_unI_rms, unI_utI_rms, rtol=1e-14, atol=1e-14 )
-        
-        ## FAILS!
-        #np.testing.assert_allclose( utI_utI, utI_utI_rms**2, rtol=1e-6, atol=1e-6 )
-        #np.testing.assert_allclose( unI_unI, unI_unI_rms**2, rtol=1e-6, atol=1e-6 )
-        
-        ## only write full covariances, not RMSes
-        
-        if ('data/utI_utI' in self): del self['data/utI_utI']
-        dset = self.create_dataset('data/utI_utI', data=utI_utI.T, chunks=None)
-        if verbose: even_print('utI_utI','%s'%str(utI_utI.shape))
-        
-        if ('data/unI_unI' in self): del self['data/unI_unI']
-        dset = self.create_dataset('data/unI_unI', data=unI_unI.T, chunks=None)
-        if verbose: even_print('unI_unI','%s'%str(unI_unI.shape))
-        
-        if ('data/utI_unI' in self): del self['data/utI_unI']
-        dset = self.create_dataset('data/utI_unI', data=utI_unI.T, chunks=None)
-        if verbose: even_print('utI_unI','%s'%str(utI_unI.shape))
-        
-        ## check
-        if self.rectilinear:
-            np.testing.assert_allclose(utI_utI, uI_uI, rtol=1e-14, atol=1e-14)
-            np.testing.assert_allclose(unI_unI, vI_vI, rtol=1e-14, atol=1e-14)
-            np.testing.assert_allclose(utI_unI, uI_vI, rtol=1e-14, atol=1e-14)
-        
-        self.get_header(verbose=False)
-        if verbose: print(72*'-')
-        if verbose: print('total time : ztmd.calc_vel_tangnorm_mean_removed() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
-        if verbose: print(72*'-')
+        # === Reynolds
         
-        return
-    
-    # ===
-    
-    def get_wall_norm_mesh(self, **kwargs):
-        '''
-        get a new 'grid' which is extruded in the normal direction from the wall
-        - this grid is good for post-processing in the wall-normal direction ONLY
-        - orthogonal to the wall-normal direction may have jumps or be folded
-        '''
-        
-        verbose = kwargs.get('verbose',True)
-        
-        ## the wall-normal unit tangent and normal vectors
-        if ('csys/vtang' in self) and ('csys/vnorm' in self):
-            vtang = np.copy( self['csys/vtang'][()] )
-            vnorm = np.copy( self['csys/vnorm'][()] )
-            #wall_trafo_mat = np.stack((vtang,vnorm), axis=-1)
-        else:
-            raise AssertionError('no vnorm/vtang unit projection vector!')
-        
-        if ('data/wall_distance' in self):
-            wall_dist = np.copy( self['data/wall_distance'][()].T )
-        else:
-            raise AssertionError('dset not present: data/wall_distance')
-        
-        xy2d_n1D          = np.zeros((self.nx,self.ny,2) , dtype=np.float64)
-        wall_distance_n1D = np.zeros((self.nx,self.ny)   , dtype=np.float64)
-        
-        for i in range(self.nx):
+        if ('data/uI_uI' in self) and ('data/uI_vI' in self) and ('data/vI_vI' in self):
             
-            p0_ = np.array([self.x[i,0],self.y[i,0]], dtype=np.float64) ## wall point coordinate
+            uI_uI = np.copy( self['data/uI_uI'][()].T )
+            vI_vI = np.copy( self['data/vI_vI'][()].T )
+            uI_vI = np.copy( self['data/uI_vI'][()].T )
+            vI_uI = np.copy( uI_vI )
             
-            vnorm_ = np.copy( vnorm[i,0,:] ) ## unit normal vec @ wall at this x
-            #vtang_ = np.copy( vtang[i,0,:] ) ## unit tangent vec @ wall at this x
+            ## construct 2D tensor --> (nx,ny,2,2)
+            uIuI_ij = np.stack( (np.stack( [uI_uI, uI_vI], axis=-1 ),
+                                 np.stack( [vI_uI, vI_vI], axis=-1 )), axis=-1 )
             
-            #x_  = np.copy( self.x[i,:] )
-            #y_  = np.copy( self.y[i,:] )
-            #dx_ = np.diff(x_,n=1)
-            #dy_ = np.diff(y_,n=1)
-            #ds_ = np.sqrt(dx_**2+dy_**2)
-            #s_  = np.cumsum(np.concatenate(([0.,],ds_))) ## path length normal to wall @ this x
+            #uIuI_ij = np.transpose(uIuI_ij, (0,1,3,2))
             
-            s_ = np.copy( wall_dist[i,:] )
+            uI_uI_rms = np.copy( self['data/uI_uI_rms'][()].T )
+            vI_vI_rms = np.copy( self['data/vI_vI_rms'][()].T )
+            uI_vI_rms = np.copy( self['data/uI_vI_rms'][()].T )
+            vI_uI_rms = np.copy( uI_vI_rms )
             
-            wall_distance_n1D[i,:] = s_
+            ## construct 2D tensor --> (nx,ny,2,2)
+            uIuI_rms_ij = np.stack( (np.stack( [uI_uI_rms, uI_vI_rms], axis=-1 ),
+                                     np.stack( [vI_uI_rms, vI_vI_rms], axis=-1 )), axis=-1 )
             
-            xy = p0_ + np.einsum( 'i,j->ij', s_, vnorm_ )
+            #uIuI_rms_ij = np.transpose(uIuI_rms_ij, (0,1,3,2))
             
-            xy2d_n1D[i,:,:] = xy
-        
-        if ('dims_2Dw/x' in self): del self['dims_2Dw/x']
-        self.create_dataset('dims_2Dw/x', data=np.squeeze(xy2d_n1D[:,:,0]).T, chunks=None)
-        
-        if ('dims_2Dw/y' in self): del self['dims_2Dw/y']
-        self.create_dataset('dims_2Dw/y', data=np.squeeze(xy2d_n1D[:,:,1]).T, chunks=None)
-        
-        if ('data_2Dw/wall_distance' in self): del self['data_2Dw/wall_distance']
-        self.create_dataset('data_2Dw/wall_distance', data=wall_distance_n1D.T, chunks=None)
-        
-        self.attrs['requires_wall_norm_interp'] = True
-        self.get_header(verbose=False)
+            ## check
+            np.testing.assert_allclose(uI_uI, uI_uI_rms**2, rtol=1e-6, atol=1e-6)
+            np.testing.assert_allclose(vI_vI, vI_vI_rms**2, rtol=1e-6, atol=1e-6)
+            
+            ## these three ops are the same
+            #uIuI_ij_tn_A = np.einsum('xyij,xyjk,xykl->xyil', trafoT, uIuI_ij, trafo)
+            #uIuI_ij_tn_B = np.einsum('xyji,xyjk,xykl->xyil', trafo,  uIuI_ij, trafo)
+            #uIuI_ij_tn_C = np.matmul(np.matmul(trafoT, uIuI_ij), trafo)
+            #np.testing.assert_allclose(uIuI_ij_tn_A, uIuI_ij_tn_B, atol=1e-14, rtol=1e-14)
+            #np.testing.assert_allclose(uIuI_ij_tn_B, uIuI_ij_tn_C, atol=1e-14, rtol=1e-14)
+            
+            uIuI_ij_tn     = np.einsum('xyji,xyjk,xykl->xyil', trafo, uIuI_ij,     trafo)
+            uIuI_rms_ij_tn = np.einsum('xyji,xyjk,xykl->xyil', trafo, uIuI_rms_ij, trafo)
+            
+            utI_utI = np.copy(uIuI_ij_tn[:,:,0,0])
+            unI_unI = np.copy(uIuI_ij_tn[:,:,1,1])
+            utI_unI = np.copy(uIuI_ij_tn[:,:,0,1])
+            unI_utI = np.copy(uIuI_ij_tn[:,:,1,0])
+            
+            np.testing.assert_allclose( utI_unI, unI_utI, rtol=1e-14, atol=1e-14 )
+            
+            utI_utI_rms = np.copy(uIuI_rms_ij_tn[:,:,0,0])
+            unI_unI_rms = np.copy(uIuI_rms_ij_tn[:,:,1,1])
+            utI_unI_rms = np.copy(uIuI_rms_ij_tn[:,:,0,1])
+            unI_utI_rms = np.copy(uIuI_rms_ij_tn[:,:,1,0])
+            
+            np.testing.assert_allclose( utI_unI_rms, unI_utI_rms, rtol=1e-14, atol=1e-14 )
+            
+            ## fails
+            #np.testing.assert_allclose( utI_utI, utI_utI_rms**2, rtol=1e-6, atol=1e-6 )
+            #np.testing.assert_allclose( unI_unI, unI_unI_rms**2, rtol=1e-6, atol=1e-6 )
+            
+            ## only write full covariances, not RMSes
+            
+            if ('data/utI_utI' in self): del self['data/utI_utI']
+            dset = self.create_dataset('data/utI_utI', data=utI_utI.T, chunks=None)
+            if verbose: even_print('utI_utI','%s'%str(utI_utI.shape))
+            
+            if ('data/unI_unI' in self): del self['data/unI_unI']
+            dset = self.create_dataset('data/unI_unI', data=unI_unI.T, chunks=None)
+            if verbose: even_print('unI_unI','%s'%str(unI_unI.shape))
+            
+            if ('data/utI_unI' in self): del self['data/utI_unI']
+            dset = self.create_dataset('data/utI_unI', data=utI_unI.T, chunks=None)
+            if verbose: even_print('utI_unI','%s'%str(utI_unI.shape))
+            
+            ## check
+            if self.rectilinear:
+                np.testing.assert_allclose(utI_utI, uI_uI, rtol=1e-14, atol=1e-14)
+                np.testing.assert_allclose(unI_unI, vI_vI, rtol=1e-14, atol=1e-14)
+                np.testing.assert_allclose(utI_unI, uI_vI, rtol=1e-14, atol=1e-14)
         
-        # ===
+        # === Favre
         
-        if False: ## debug plot
+        if ('data/r_uII_uII' in self) and ('data/r_uII_vII' in self) and ('data/r_vII_vII' in self):
             
-            lwg = 0.12 ## line width grid
+            r_uII_uII = np.copy( self['data/r_uII_uII'][()].T )
+            r_vII_vII = np.copy( self['data/r_vII_vII'][()].T )
+            r_uII_vII = np.copy( self['data/r_uII_vII'][()].T )
+            r_vII_uII = np.copy( r_uII_vII )
             
-            xy2d1 = np.copy( np.stack((self.x,self.y), axis=-1) / self.lchar )
-            xy2d2 = np.copy( xy2d_n1D / self.lchar )
+            ## construct 2D tensor --> (nx,ny,2,2)
+            r_uIIuII_ij = np.stack( (np.stack( [r_uII_uII, r_uII_vII], axis=-1 ),
+                                     np.stack( [r_vII_uII, r_vII_vII], axis=-1 )), axis=-1 )
             
-            plt.close('all')
-            mpl.style.use('dark_background')
-            fig1 = plt.figure(figsize=(8,8/2), dpi=230)
-            ax1 = fig1.gca()
-            ax1.set_aspect('equal')
-            ax1.tick_params(axis='x', which='both', direction='out')
-            ax1.tick_params(axis='y', which='both', direction='out')
-            ##
-            # grid_ln_y = mpl.collections.LineCollection(xy2d1,                       linewidth=lwg, edgecolors='red', zorder=19)
-            # grid_ln_x = mpl.collections.LineCollection(np.transpose(xy2d1,(1,0,2)), linewidth=lwg, edgecolors='red', zorder=19)
-            # ax1.add_collection(grid_ln_y)
-            # ax1.add_collection(grid_ln_x)
-            ##
-            grid_ln_y = mpl.collections.LineCollection(xy2d2,                       linewidth=lwg, edgecolors=ax1.xaxis.label.get_color(), zorder=19)
-            grid_ln_x = mpl.collections.LineCollection(np.transpose(xy2d2,(1,0,2)), linewidth=lwg, edgecolors=ax1.xaxis.label.get_color(), zorder=19)
-            ax1.add_collection(grid_ln_y)
-            ax1.add_collection(grid_ln_x)
-            ##
-            ax1.set_xlabel('$x/\ell_{char}$')
-            ax1.set_ylabel('$y/\ell_{char}$')
-            ##
-            ax1.set_xlim(xy2d1[:,:,0].min()-3,xy2d1[:,:,0].max()+3)
-            ax1.set_ylim(xy2d1[:,:,1].min()-3,xy2d1[:,:,1].max()+3)
-            ##
-            #ax1.set_xlim(self.plot_xlim[0],self.plot_xlim[1])
-            #ax1.set_ylim(self.plot_ylim[0],self.plot_ylim[1])
-            ##
-            ax1.xaxis.set_major_locator(mpl.ticker.MultipleLocator(20))
-            ax1.xaxis.set_minor_locator(mpl.ticker.MultipleLocator(5))
-            ax1.yaxis.set_major_locator(mpl.ticker.MultipleLocator(20))
-            ax1.yaxis.set_minor_locator(mpl.ticker.MultipleLocator(5))
-            ##
-            fig1.tight_layout(pad=0.25)
-            fig1.tight_layout(pad=0.25)
-            ##
-            #dpi_out = 2*2160/plt.gcf().get_size_inches()[1]
-            #turbx.fig_trim_x(fig1, [ax1], offset_px=10, dpi=dpi_out)
-            #fig1.savefig('grid.png', dpi=dpi_out)
-            plt.show()
-            pass
+            r_uII_uII_rms = np.copy( self['data/r_uII_uII_rms'][()].T )
+            r_vII_vII_rms = np.copy( self['data/r_vII_vII_rms'][()].T )
+            r_uII_vII_rms = np.copy( self['data/r_uII_vII_rms'][()].T )
+            r_vII_uII_rms = np.copy( r_uII_vII_rms )
+            
+            ## construct 2D tensor --> (nx,ny,2,2)
+            r_uIIuII_rms_ij = np.stack( (np.stack( [r_uII_uII_rms, r_uII_vII_rms], axis=-1 ),
+                                         np.stack( [r_vII_uII_rms, r_vII_vII_rms], axis=-1 )), axis=-1 )
+            
+            ## check
+            np.testing.assert_allclose(r_uII_uII, r_uII_uII_rms**2, rtol=1e-6, atol=1e-6)
+            np.testing.assert_allclose(r_vII_vII, r_vII_vII_rms**2, rtol=1e-6, atol=1e-6)
+            
+            r_uIIuII_ij_tn     = np.einsum('xyji,xyjk,xykl->xyil', trafo, r_uIIuII_ij,     trafo)
+            r_uIIuII_rms_ij_tn = np.einsum('xyji,xyjk,xykl->xyil', trafo, r_uIIuII_rms_ij, trafo)
+            
+            r_utII_utII = np.copy(r_uIIuII_ij_tn[:,:,0,0])
+            r_unII_unII = np.copy(r_uIIuII_ij_tn[:,:,1,1])
+            r_utII_unII = np.copy(r_uIIuII_ij_tn[:,:,0,1])
+            r_unII_utII = np.copy(r_uIIuII_ij_tn[:,:,1,0])
+            
+            np.testing.assert_allclose( r_utII_unII, r_unII_utII, rtol=1e-14, atol=1e-14 )
+            
+            r_utII_utII_rms = np.copy(uIuI_rms_ij_tn[:,:,0,0])
+            r_unII_unII_rms = np.copy(uIuI_rms_ij_tn[:,:,1,1])
+            r_utII_unII_rms = np.copy(uIuI_rms_ij_tn[:,:,0,1])
+            r_unII_utII_rms = np.copy(uIuI_rms_ij_tn[:,:,1,0])
+            
+            np.testing.assert_allclose( r_utII_unII_rms, r_unII_utII_rms, rtol=1e-14, atol=1e-14 )
+            
+            ## fails!
+            #np.testing.assert_allclose( r_utII_utII, r_utII_utII_rms**2, rtol=1e-6, atol=1e-6 )
+            #np.testing.assert_allclose( r_unII_unII, r_unII_unII_rms**2, rtol=1e-6, atol=1e-6 )
+            
+            ## only write full covariances, not RMSes
+            
+            if ('data/r_utII_utII' in self): del self['data/r_utII_utII']
+            dset = self.create_dataset('data/r_utII_utII', data=r_utII_utII.T, chunks=None)
+            if verbose: even_print('r_utII_utII','%s'%str(r_utII_utII.shape))
+            
+            if ('data/r_unII_unII' in self): del self['data/r_unII_unII']
+            dset = self.create_dataset('data/r_unII_unII', data=r_unII_unII.T, chunks=None)
+            if verbose: even_print('r_unII_unII','%s'%str(r_unII_unII.shape))
+            
+            if ('data/r_utII_unII' in self): del self['data/r_utII_unII']
+            dset = self.create_dataset('data/r_utII_unII', data=r_utII_unII.T, chunks=None)
+            if verbose: even_print('r_utII_unII','%s'%str(r_utII_unII.shape))
+            
+            ## check
+            if self.rectilinear:
+                np.testing.assert_allclose(r_utII_utII, r_uII_uII, rtol=1e-14, atol=1e-14)
+                np.testing.assert_allclose(r_unII_unII, r_vII_vII, rtol=1e-14, atol=1e-14)
+                np.testing.assert_allclose(r_utII_unII, r_uII_vII, rtol=1e-14, atol=1e-14)
+        
+        self.get_header(verbose=False)
+        if verbose: print(72*'-')
+        if verbose: print('total time : ztmd.calc_vel_tangnorm_mean_removed() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
         
         return
     
-    def interp_to_wall_norm_mesh(self, **kwargs):
+    # === post-processing: mass, momentum, energy balance
+    
+    def calc_mass_balance_terms(self, **kwargs):
         '''
-        interpolate fields from original grid to 'wall-normal' grid
+        calculate terms of time-averaged mass conservation equation
         '''
         
         verbose = kwargs.get('verbose',True)
-        scalars = kwargs.get('scalars',None)
-        
-        if verbose: print('\n'+'turbx.ztmd.interp_to_wall_norm_mesh()'+'\n'+72*'-')
+        if verbose: print('\n'+'ztmd.calc_mass_balance_terms()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
         
-        ## read: wall normal grid x
-        if ('dims_2Dw/x' in self):
-            x_wn = np.copy( self['dims_2Dw/x'][()].T )
-        else:
-            raise AssertionError('dset not present: dims_2Dw/x')
-        
-        ## read: wall normal grid y
-        if ('dims_2Dw/y' in self):
-            y_wn = np.copy( self['dims_2Dw/y'][()].T )
-        else:
-            raise AssertionError('dset not present: dims_2Dw/y')
-        
-        # === get list of scalars to interpolate
-        
-        scalars_2d_names = list(self['data'].keys())
-        if verbose: even_print('n scalars found in data/','%i'%(len(scalars_2d_names),))
-        
-        if (scalars is None): ## take all scalars present in file
-            
-            ## dont interpolate ddx[] or ddy[] gradients or 'wall_distance'
-            scalars_2d_names = [ s for s in scalars_2d_names if ('ddx_' not in s)    ]
-            scalars_2d_names = [ s for s in scalars_2d_names if ('ddy_' not in s)    ]
-            scalars_2d_names = [ s for s in scalars_2d_names if (s!='wall_distance') ]
-        
-        else: ## explicit scalar list was passed
-            
-            if not isinstance(scalars, list):
-                raise ValueError("'scalars' should be type list")
-            if not isinstance(scalars[0], str):
-                raise ValueError("'scalars' should contain strings")
-            
-            scalars_2d_names = list(self['data'].keys())
-            
-            ## take only scalars which actually exist
-            scalars_2d_names = [ s for s in scalars if (s in scalars_2d_names) ]
-        
-        # === interpolate
-        
-        if verbose: even_print('n scalars to be interpolated','%i'%(len(scalars_2d_names),))
-        
-        if True: ## interpolate
-            
-            x2d_A = self.x
-            y2d_A = self.y
-            x2d_B = x_wn
-            y2d_B = y_wn
-            
-            if verbose: progress_bar = tqdm(total=len(scalars_2d_names), ncols=100, desc='interpolate 2D', leave=False, file=sys.stdout)
-            for scalar_name in scalars_2d_names:
-                
-                ## copy data into memory
-                scalar_data = np.copy( self['data/%s'%scalar_name][()].T  )
-                
-                ## do interpolation
-                if verbose: tqdm.write(even_print('start interpolate',scalar_name,s=True))
-                t_start = timeit.default_timer()
-                scalar_data_wn = interp_2d_structured(x2d_A, y2d_A, x2d_B, y2d_B, scalar_data)
-                if verbose: tqdm.write(even_print('done interpolating','%s'%format_time_string((timeit.default_timer() - t_start)),s=True))
-                
-                ## write to HDF5
-                if ('data_2Dw/%s'%scalar_name in self):
-                    del self['data_2Dw/%s'%scalar_name]
-                self.create_dataset('data_2Dw/%s'%scalar_name, data=scalar_data_wn.T, chunks=None)
-                
-                ## clear from memory
-                scalar_data    = None ; del scalar_data
-                scalar_data_wn = None ; del scalar_data_wn
-                
-                progress_bar.update()
-            progress_bar.close()
+        pass
+        pass
+        raise NotImplementedError
         
-        self.attrs['requires_wall_norm_interp'] = True
         self.get_header(verbose=False)
-        
-        if verbose: print('\n'+72*'-')
-        if verbose: print('total time : turbx.interp_to_wall_norm_mesh() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        if verbose: print('total time : ztmd.calc_mass_balance_terms() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
-    def add_grid_quality_metrics_2d(self, **kwargs):
+    def calc_momentum_balance_x_terms(self, **kwargs):
         '''
-        attach grid quality measures to ZTMD
+        calculate terms of time-averaged momentum [x] conservation equation
         '''
-        x = np.copy( self['dims/x'][()].T )
-        y = np.copy( self['dims/y'][()].T )
         
-        grid_quality_dict = get_grid_quality_metrics_2d(x,y,verbose=True)
-        
-        if ('data_cells/skew' in self): del self['data_cells/skew']
-        dset = self.create_dataset('data_cells/skew', data=grid_quality_dict['skew'].T, chunks=None)
+        verbose = kwargs.get('verbose',True)
+        if verbose: print('\n'+'ztmd.calc_momentum_balance_x_terms()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
         
-        if ('data/ds1avg' in self): del self['data/ds1avg']
-        dset = self.create_dataset('data/ds1avg', data=grid_quality_dict['ds1avg'].T, chunks=None)
+        pass
+        pass
+        raise NotImplementedError
         
-        if ('data/ds2avg' in self): del self['data/ds2avg']
-        dset = self.create_dataset('data/ds2avg', data=grid_quality_dict['ds2avg'].T, chunks=None)
+        self.get_header(verbose=False)
+        if verbose: print(72*'-')
+        if verbose: print('total time : ztmd.calc_momentum_balance_x_terms() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
         
         return
     
-    def add_cyl_coords(self, **kwargs):
+    def calc_momentum_balance_y_terms(self, **kwargs):
         '''
-        attach [θ,r] coords, calculated from [x,y]
+        calculate terms of time-averaged momentum [y] conservation equation
         '''
-        cx = kwargs.get('cx',0.)
-        cy = kwargs.get('cy',0.)
         
-        x = np.copy( self['dims/x'][()].T )
-        y = np.copy( self['dims/y'][()].T )
-        
-        xy2d = np.stack((x,y), axis=-1)
+        verbose = kwargs.get('verbose',True)
+        if verbose: print('\n'+'ztmd.calc_momentum_balance_y_terms()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
         
-        trz = rect_to_cyl(xy2d, cx=cx, cy=cy)
+        pass
+        pass
+        raise NotImplementedError
         
-        if ('dims/theta' in self): del self['dims/theta']
-        dset = self.create_dataset('dims/theta', data=trz[:,:,0].T, chunks=None)
-        if ('dims/r' in self): del self['dims/r']
-        dset = self.create_dataset('dims/r', data=trz[:,:,1].T, chunks=None)
+        self.get_header(verbose=False)
+        if verbose: print(72*'-')
+        if verbose: print('total time : ztmd.calc_momentum_balance_y_terms() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
         
         return
     
-    # === post-processing
+    # === post-processing: 1D profiles
     
     def calc_bl_edge(self, **kwargs):
         '''
         determine the boundary layer edge location
         psvel : pseudo-velocity, i.e. [-ω_z] cumulatively integrated in wall-normal direction
         y_edge : the wall-normal coordinate corresponding to the peak of the (interpolated) pseudo-velocity
         j_edge : the nearest index to y_edge
@@ -19457,14 +20423,39 @@
             ## get [y] of first intersection
             jtop = ny-1
             for j in range(ny):
                 if ( ddy_psvel_[j] < epsilon):
                     jtop = j
                     break
             
+            # if (i==5001):
+            #     plt.close('all')
+            #     fig1 = plt.figure(figsize=(3,3), dpi=300)
+            #     ax1 = plt.gca()
+            #     ax1.plot(  psvel_, y/self.lchar, lw=0.5 )
+            #     #ax1.axhline(y=y_max[i]/self.lchar, linestyle='dashed', c='lightgray', zorder=1, lw=0.3)
+            #     fig1.tight_layout(pad=0.25)
+            #     fig1.tight_layout(pad=0.25)
+            #     plt.show()
+            
+            # print(f'i={i:d}, s={stang[i]/self.lchar:0.5f}')
+            
+            # print(ddy_psvel_.min())
+            
+            # if (i==3739):
+            #     plt.close('all')
+            #     fig1 = plt.figure(figsize=(3,3), dpi=300)
+            #     ax1 = plt.gca()
+            #     #ax1.plot(  ddy_psvel_[jtop-2:jtop+1], y_[jtop-2:jtop+1]/self.lchar, lw=0.5, marker='o' )
+            #     ax1.plot(  ddy_psvel_, y_/self.lchar, lw=0.5 )
+            #     ax1.axvline(x=epsilon, linestyle='dashed', c='lightgray', zorder=1, lw=0.3)
+            #     fig1.tight_layout(pad=0.25)
+            #     fig1.tight_layout(pad=0.25)
+            #     plt.show()
+            
             intrp_func = sp.interpolate.interp1d(y_/self.lchar, ddy_psvel_, kind='linear', bounds_error=True)
             
             def __f_opt1(y_test, intrp_func, epsilon):
                 ddy_psvel_test = intrp_func(y_test/self.lchar)
                 root = np.abs( ddy_psvel_test - epsilon )
                 return root
             
@@ -20308,14 +21299,259 @@
         self.get_header(verbose=False)
         if verbose: print(72*'-')
         if verbose: print('total time : ztmd.calc_bl_integral_quantities() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
+    # === legacy: functions for curved TBL cases where axis=1 mesh is not identical over axis=0
+    
+    def get_wall_norm_mesh(self, **kwargs):
+        '''
+        get a new 'grid' which is extruded in the normal direction from the wall
+        - this grid is good for post-processing in the wall-normal direction ONLY
+        - orthogonal to the wall-normal direction may have jumps or be folded
+        '''
+        
+        verbose = kwargs.get('verbose',True)
+        
+        ## the wall-normal unit tangent and normal vectors
+        if ('csys/vtang' in self) and ('csys/vnorm' in self):
+            vtang = np.copy( self['csys/vtang'][()] )
+            vnorm = np.copy( self['csys/vnorm'][()] )
+            #wall_trafo_mat = np.stack((vtang,vnorm), axis=-1)
+        else:
+            raise AssertionError('no vnorm/vtang unit projection vector!')
+        
+        if ('data/wall_distance' in self):
+            wall_dist = np.copy( self['data/wall_distance'][()].T )
+        else:
+            raise AssertionError('dset not present: data/wall_distance')
+        
+        xy2d_n1D          = np.zeros((self.nx,self.ny,2) , dtype=np.float64)
+        wall_distance_n1D = np.zeros((self.nx,self.ny)   , dtype=np.float64)
+        
+        for i in range(self.nx):
+            
+            p0_ = np.array([self.x[i,0],self.y[i,0]], dtype=np.float64) ## wall point coordinate
+            
+            vnorm_ = np.copy( vnorm[i,0,:] ) ## unit normal vec @ wall at this x
+            #vtang_ = np.copy( vtang[i,0,:] ) ## unit tangent vec @ wall at this x
+            
+            #x_  = np.copy( self.x[i,:] )
+            #y_  = np.copy( self.y[i,:] )
+            #dx_ = np.diff(x_,n=1)
+            #dy_ = np.diff(y_,n=1)
+            #ds_ = np.sqrt(dx_**2+dy_**2)
+            #s_  = np.cumsum(np.concatenate(([0.,],ds_))) ## path length normal to wall @ this x
+            
+            s_ = np.copy( wall_dist[i,:] )
+            
+            wall_distance_n1D[i,:] = s_
+            
+            xy = p0_ + np.einsum( 'i,j->ij', s_, vnorm_ )
+            
+            xy2d_n1D[i,:,:] = xy
+        
+        if ('dims_2Dw/x' in self): del self['dims_2Dw/x']
+        self.create_dataset('dims_2Dw/x', data=np.squeeze(xy2d_n1D[:,:,0]).T, chunks=None)
+        
+        if ('dims_2Dw/y' in self): del self['dims_2Dw/y']
+        self.create_dataset('dims_2Dw/y', data=np.squeeze(xy2d_n1D[:,:,1]).T, chunks=None)
+        
+        if ('data_2Dw/wall_distance' in self): del self['data_2Dw/wall_distance']
+        self.create_dataset('data_2Dw/wall_distance', data=wall_distance_n1D.T, chunks=None)
+        
+        self.attrs['requires_wall_norm_interp'] = True
+        self.get_header(verbose=False)
+        
+        # ===
+        
+        if False: ## debug plot
+            
+            lwg = 0.12 ## line width grid
+            
+            xy2d1 = np.copy( np.stack((self.x,self.y), axis=-1) / self.lchar )
+            xy2d2 = np.copy( xy2d_n1D / self.lchar )
+            
+            plt.close('all')
+            mpl.style.use('dark_background')
+            fig1 = plt.figure(figsize=(8,8/2), dpi=230)
+            ax1 = fig1.gca()
+            ax1.set_aspect('equal')
+            ax1.tick_params(axis='x', which='both', direction='out')
+            ax1.tick_params(axis='y', which='both', direction='out')
+            ##
+            # grid_ln_y = mpl.collections.LineCollection(xy2d1,                       linewidth=lwg, edgecolors='red', zorder=19)
+            # grid_ln_x = mpl.collections.LineCollection(np.transpose(xy2d1,(1,0,2)), linewidth=lwg, edgecolors='red', zorder=19)
+            # ax1.add_collection(grid_ln_y)
+            # ax1.add_collection(grid_ln_x)
+            ##
+            grid_ln_y = mpl.collections.LineCollection(xy2d2,                       linewidth=lwg, edgecolors=ax1.xaxis.label.get_color(), zorder=19)
+            grid_ln_x = mpl.collections.LineCollection(np.transpose(xy2d2,(1,0,2)), linewidth=lwg, edgecolors=ax1.xaxis.label.get_color(), zorder=19)
+            ax1.add_collection(grid_ln_y)
+            ax1.add_collection(grid_ln_x)
+            ##
+            ax1.set_xlabel('$x/\ell_{char}$')
+            ax1.set_ylabel('$y/\ell_{char}$')
+            ##
+            ax1.set_xlim(xy2d1[:,:,0].min()-3,xy2d1[:,:,0].max()+3)
+            ax1.set_ylim(xy2d1[:,:,1].min()-3,xy2d1[:,:,1].max()+3)
+            ##
+            #ax1.set_xlim(self.plot_xlim[0],self.plot_xlim[1])
+            #ax1.set_ylim(self.plot_ylim[0],self.plot_ylim[1])
+            ##
+            ax1.xaxis.set_major_locator(mpl.ticker.MultipleLocator(20))
+            ax1.xaxis.set_minor_locator(mpl.ticker.MultipleLocator(5))
+            ax1.yaxis.set_major_locator(mpl.ticker.MultipleLocator(20))
+            ax1.yaxis.set_minor_locator(mpl.ticker.MultipleLocator(5))
+            ##
+            fig1.tight_layout(pad=0.25)
+            fig1.tight_layout(pad=0.25)
+            ##
+            #dpi_out = 2*2160/plt.gcf().get_size_inches()[1]
+            #turbx.fig_trim_x(fig1, [ax1], offset_px=10, dpi=dpi_out)
+            #fig1.savefig('grid.png', dpi=dpi_out)
+            plt.show()
+            pass
+        
+        return
+    
+    def interp_to_wall_norm_mesh(self, **kwargs):
+        '''
+        interpolate fields from original grid to 'wall-normal' grid
+        '''
+        
+        verbose = kwargs.get('verbose',True)
+        scalars = kwargs.get('scalars',None)
+        
+        if verbose: print('\n'+'turbx.ztmd.interp_to_wall_norm_mesh()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
+        
+        ## read: wall normal grid x
+        if ('dims_2Dw/x' in self):
+            x_wn = np.copy( self['dims_2Dw/x'][()].T )
+        else:
+            raise AssertionError('dset not present: dims_2Dw/x')
+        
+        ## read: wall normal grid y
+        if ('dims_2Dw/y' in self):
+            y_wn = np.copy( self['dims_2Dw/y'][()].T )
+        else:
+            raise AssertionError('dset not present: dims_2Dw/y')
+        
+        # === get list of scalars to interpolate
+        
+        scalars_2d_names = list(self['data'].keys())
+        if verbose: even_print('n scalars found in data/','%i'%(len(scalars_2d_names),))
+        
+        if (scalars is None): ## take all scalars present in file
+            
+            ## dont interpolate ddx[] or ddy[] gradients or 'wall_distance'
+            scalars_2d_names = [ s for s in scalars_2d_names if ('ddx_' not in s)    ]
+            scalars_2d_names = [ s for s in scalars_2d_names if ('ddy_' not in s)    ]
+            scalars_2d_names = [ s for s in scalars_2d_names if (s!='wall_distance') ]
+        
+        else: ## explicit scalar list was passed
+            
+            if not isinstance(scalars, list):
+                raise ValueError("'scalars' should be type list")
+            if not isinstance(scalars[0], str):
+                raise ValueError("'scalars' should contain strings")
+            
+            scalars_2d_names = list(self['data'].keys())
+            
+            ## take only scalars which actually exist
+            scalars_2d_names = [ s for s in scalars if (s in scalars_2d_names) ]
+        
+        # === interpolate
+        
+        if verbose: even_print('n scalars to be interpolated','%i'%(len(scalars_2d_names),))
+        
+        if True: ## interpolate
+            
+            x2d_A = self.x
+            y2d_A = self.y
+            x2d_B = x_wn
+            y2d_B = y_wn
+            
+            if verbose: progress_bar = tqdm(total=len(scalars_2d_names), ncols=100, desc='interpolate 2D', leave=False, file=sys.stdout)
+            for scalar_name in scalars_2d_names:
+                
+                ## copy data into memory
+                scalar_data = np.copy( self['data/%s'%scalar_name][()].T  )
+                
+                ## do interpolation
+                if verbose: tqdm.write(even_print('start interpolate',scalar_name,s=True))
+                t_start = timeit.default_timer()
+                scalar_data_wn = interp_2d_structured(x2d_A, y2d_A, x2d_B, y2d_B, scalar_data)
+                if verbose: tqdm.write(even_print('done interpolating','%s'%format_time_string((timeit.default_timer() - t_start)),s=True))
+                
+                ## write to HDF5
+                if ('data_2Dw/%s'%scalar_name in self):
+                    del self['data_2Dw/%s'%scalar_name]
+                self.create_dataset('data_2Dw/%s'%scalar_name, data=scalar_data_wn.T, chunks=None)
+                
+                ## clear from memory
+                scalar_data    = None ; del scalar_data
+                scalar_data_wn = None ; del scalar_data_wn
+                
+                progress_bar.update()
+            progress_bar.close()
+        
+        self.attrs['requires_wall_norm_interp'] = True
+        self.get_header(verbose=False)
+        
+        if verbose: print('\n'+72*'-')
+        if verbose: print('total time : turbx.interp_to_wall_norm_mesh() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
+        return
+    
+    def add_grid_quality_metrics_2d(self, **kwargs):
+        '''
+        attach grid quality measures to ZTMD
+        '''
+        x = np.copy( self['dims/x'][()].T )
+        y = np.copy( self['dims/y'][()].T )
+        
+        grid_quality_dict = get_grid_quality_metrics_2d(x,y,verbose=True)
+        
+        if ('data_cells/skew' in self): del self['data_cells/skew']
+        dset = self.create_dataset('data_cells/skew', data=grid_quality_dict['skew'].T, chunks=None)
+        
+        if ('data/ds1avg' in self): del self['data/ds1avg']
+        dset = self.create_dataset('data/ds1avg', data=grid_quality_dict['ds1avg'].T, chunks=None)
+        
+        if ('data/ds2avg' in self): del self['data/ds2avg']
+        dset = self.create_dataset('data/ds2avg', data=grid_quality_dict['ds2avg'].T, chunks=None)
+        
+        return
+    
+    def add_cyl_coords(self, **kwargs):
+        '''
+        attach [θ,r] coords, calculated from [x,y]
+        '''
+        cx = kwargs.get('cx',0.)
+        cy = kwargs.get('cy',0.)
+        
+        x = np.copy( self['dims/x'][()].T )
+        y = np.copy( self['dims/y'][()].T )
+        
+        xy2d = np.stack((x,y), axis=-1)
+        
+        trz = rect_to_cyl(xy2d, cx=cx, cy=cy)
+        
+        if ('dims/theta' in self): del self['dims/theta']
+        dset = self.create_dataset('dims/theta', data=trz[:,:,0].T, chunks=None)
+        if ('dims/r' in self): del self['dims/r']
+        dset = self.create_dataset('dims/r', data=trz[:,:,1].T, chunks=None)
+        
+        return
+    
     # === Paraview
     
     def make_xdmf(self, **kwargs):
         '''
         generate an XDMF/XMF2 from ZTMD for processing with Paraview
         -----
         --> https://www.xdmf.org/index.php/XDMF_Model_and_Format
@@ -21392,20 +22628,49 @@
             self.n_ranks = self.comm.Get_size()
             self.rank    = self.comm.Get_rank()
         else:
             self.comm    = None
             self.n_ranks = 1
             self.rank    = 0
         
+        ## spd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
+        stripe_count   = kwargs.pop('stripe_count'   , 32    )
+        stripe_size_mb = kwargs.pop('stripe_size_mb' , 8     )
+        perms          = kwargs.pop('stripe_size_mb' , '640' )
+        
+        if not isinstance(stripe_count, int):
+            raise ValueError
+        if not isinstance(stripe_size_mb, int):
+            raise ValueError
+        if not isinstance(perms, str):
+            raise ValueError
+        if not len(perms)==3:
+            raise ValueError
+        if not re.fullmatch(r'\d{3}',perms):
+            raise ValueError
+        
         ## if not using MPI, remove 'driver' and 'comm' from kwargs
         if ( not self.usingmpi ) and ('driver' in kwargs):
             kwargs.pop('driver')
         if ( not self.usingmpi ) and ('comm' in kwargs):
             kwargs.pop('comm')
         
+        ## | mpiexec --mca io romio321 -n $NP python3 ...
+        ## | mpiexec --mca io ompio -n $NP python3 ...
+        ## | ompi_info --> print ompi settings (grep 'MCA io' for I/O opts)
+        ## | export ROMIO_FSTYPE_FORCE="lustre:" --> force Lustre driver over UFS when using romio --> causes crash
+        ## | export ROMIO_FSTYPE_FORCE="ufs:"
+        ## | export ROMIO_PRINT_HINTS=1 --> show available hints
+        ##
+        ## https://doku.lrz.de/best-practices-hints-and-optimizations-for-io-10747318.html
+        ##
+        ## OMPIO
+        ## export OMPI_MCA_sharedfp=^lockedfile,individual
+        ## mpiexec --mca io ompio -n $NP python3 script.py
+        
         ## set ROMIO hints, passed through 'mpi_info' dict
         if self.usingmpi:
             if ('info' in kwargs):
                 self.mpi_info = kwargs['info']
             else:
                 mpi_info = MPI.Info.Create()
                 ##
@@ -21413,23 +22678,45 @@
                 mpi_info.Set('romio_ds_read'  , 'disable'   )
                 mpi_info.Set('romio_cb_read'  , 'automatic' )
                 mpi_info.Set('romio_cb_write' , 'automatic' )
                 #mpi_info.Set('romio_cb_read'  , 'enable' )
                 #mpi_info.Set('romio_cb_write' , 'enable' )
                 mpi_info.Set('cb_buffer_size' , str(int(round(16*1024**2))) ) ## 16 [MB]
                 ##
+                #mpi_info.Set('romio_no_indep_rw' , 'true' ) ## deferred open + only collective I/O 
+                #mpi_info.Set('cb_nodes' , str(int(round(1*self.n_ranks))) )
+                ##
                 kwargs['info'] = mpi_info
                 self.mpi_info = mpi_info
         
+        ## | rdcc_nbytes:
+        ## | ------------
+        ## | Integer setting the total size of the raw data chunk cache for this dataset in bytes.
+        ## | In most cases increasing this number will improve performance, as long as you have 
+        ## | enough free memory. The default size is 1 MB
+        
+        ## --> gets passed to H5Pset_chunk_cache
         if ('rdcc_nbytes' not in kwargs):
             kwargs['rdcc_nbytes'] = int(16*1024**2) ## 16 [MB]
         
+        ## | rdcc_nslots:
+        ## | ------------
+        ## | Integer defining the number of chunk slots in the raw data chunk cache for this dataset.
+        
+        ## if ('rdcc_nslots' not in kwargs):
+        ##     kwargs['rdcc_nslots'] = 521
+        
         ## spd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
-        verbose = kwargs.pop('verbose',False)
-        force   = kwargs.pop('force',False)
+        verbose = kwargs.pop( 'verbose' , False )
+        force   = kwargs.pop( 'force'   , False )
+        
+        if not isinstance(verbose, bool):
+            raise ValueError
+        if not isinstance(force, bool):
+            raise ValueError
         
         # === initialize file on FS
         
         ## if file open mode is 'w', the file exists, and force is False
         ## --> raise error
         if (self.open_mode == 'w') and (force is False) and os.path.isfile(self.fname):
             if (self.rank==0):
@@ -21445,28 +22732,32 @@
                                   or use force=True arg:
                                   
                                   >>> with spd(<<fname>>,'w',force=True) as f:
                                   >>>     ...
                                   '''
                 print(textwrap.indent(textwrap.dedent(openModeInfoStr), 2*' ').strip('\n'))
                 print(72*'-'+'\n')
+                sys.stdout.flush()
             
             if (self.comm is not None):
                 self.comm.Barrier()
             raise FileExistsError()
         
-        ## if file open mode is 'w', the file exists, and force is True
-        ## --> delete, touch, chmod, stripe
-        if (self.open_mode == 'w') and (force is True) and os.path.isfile(self.fname):
+        ## if file open mode is 'w'
+        ## --> <delete>, touch, chmod, stripe
+        if (self.open_mode == 'w'):
             if (self.rank==0):
-                os.remove(self.fname)
-                Path(self.fname).touch()
-                os.chmod(self.fname, int('640', base=8))
-                if shutil.which('lfs') is not None:
-                    return_code = subprocess.call(f'lfs migrate --stripe-count 16 --stripe-size 16M {self.fname} > /dev/null 2>&1', shell=True)
+                if os.path.isfile(self.fname): ## if the file exists, delete it
+                    os.remove(self.fname)
+                    time.sleep(0.1)
+                Path(self.fname).touch() ## touch a new file
+                os.chmod(self.fname, int(perms, base=8)) ## change permissions
+                if shutil.which('lfs') is not None: ## set stripe if on Lustre
+                    cmd_str_lfs_migrate = f'lfs migrate --stripe-count {stripe_count:d} --stripe-size {stripe_size_mb:d}M {self.fname} > /dev/null 2>&1'
+                    return_code = subprocess.call(cmd_str_lfs_migrate, shell=True)
                     if (return_code != 0):
                         raise ValueError('lfs migrate failed')
                 else:
                     #print('striping with lfs not permitted on this filesystem')
                     pass
         
         if (self.comm is not None):
```

### Comparing `turbx-0.3.0/turbx.egg-info/PKG-INFO` & `turbx-0.3.1/turbx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.3.0
+Version: 0.3.1
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
```

