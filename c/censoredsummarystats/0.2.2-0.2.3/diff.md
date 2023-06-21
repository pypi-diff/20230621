# Comparing `tmp/censoredsummarystats-0.2.2.tar.gz` & `tmp/censoredsummarystats-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredsummarystats-0.2.2.tar", max compression
+gzip compressed data, was "censoredsummarystats-0.2.3.tar", max compression
```

## Comparing `censoredsummarystats-0.2.2.tar` & `censoredsummarystats-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       58 2023-06-21 09:23:06.539217 censoredsummarystats-0.2.2/censoredsummarystats/__init__.py
--rw-r--r--   0        0        0    56473 2023-06-21 09:44:54.719729 censoredsummarystats-0.2.2/censoredsummarystats/statistics.py
--rw-r--r--   0        0        0     2291 2023-06-21 07:54:57.800594 censoredsummarystats-0.2.2/censoredsummarystats/utils.py
--rw-r--r--   0        0        0    11558 2023-06-21 07:54:57.796594 censoredsummarystats-0.2.2/LICENSE
--rw-r--r--   0        0        0      558 2023-06-21 09:44:54.724729 censoredsummarystats-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     8308 2023-06-21 07:54:57.797594 censoredsummarystats-0.2.2/README.md
--rw-r--r--   0        0        0     8939 1970-01-01 00:00:00.000000 censoredsummarystats-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-06-21 09:23:06.539217 censoredsummarystats-0.2.3/censoredsummarystats/__init__.py
+-rw-r--r--   0        0        0    56475 2023-06-21 10:32:36.151410 censoredsummarystats-0.2.3/censoredsummarystats/statistics.py
+-rw-r--r--   0        0        0     2291 2023-06-21 07:54:57.800594 censoredsummarystats-0.2.3/censoredsummarystats/utils.py
+-rw-r--r--   0        0        0    11558 2023-06-21 07:54:57.796594 censoredsummarystats-0.2.3/LICENSE
+-rw-r--r--   0        0        0      558 2023-06-21 10:34:21.395260 censoredsummarystats-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     8308 2023-06-21 07:54:57.797594 censoredsummarystats-0.2.3/README.md
+-rw-r--r--   0        0        0     8939 1970-01-01 00:00:00.000000 censoredsummarystats-0.2.3/PKG-INFO
```

### Comparing `censoredsummarystats-0.2.2/censoredsummarystats/statistics.py` & `censoredsummarystats-0.2.3/censoredsummarystats/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -3438,93 +3438,93 @@
 0000d6d0: 3e20 302c 2063 6466 2e72 6573 756c 745f  > 0, cdf.result_
 0000d6e0: 636f 6c5d 203d 2028 0d0a 2020 2020 2020  col] = (..      
 0000d6f0: 2020 2020 2020 6466 5b63 6466 2e72 6573        df[cdf.res
 0000d700: 756c 745f 636f 6c5d 202b 0d0a 2020 2020  ult_col] +..    
 0000d710: 2020 2020 2020 2020 2720 2827 202b 2064          ' (' + d
 0000d720: 665b 6364 662e 6967 6e6f 7265 645f 636f  f[cdf.ignored_co
 0000d730: 6c5d 2e61 7374 7970 6528 7374 7229 202b  l].astype(str) +
-0000d740: 2027 2076 616c 7565 7320 6967 6e6f 7265   ' values ignore
-0000d750: 6429 270d 0a20 2020 2020 2020 2020 2020  d)'..           
-0000d760: 2029 0d0a 2020 2020 2020 2020 0d0a 2020   )..        ..  
-0000d770: 2020 2020 2020 2320 4372 6561 7465 2061        # Create a
-0000d780: 2063 6f6c 756d 6e20 7468 6174 2069 6e64   column that ind
-0000d790: 6963 6174 6573 2074 6865 2067 656e 6572  icates the gener
-0000d7a0: 6174 6564 2073 7461 7469 7374 6963 200d  ated statistic .
-0000d7b0: 0a20 2020 2020 2020 2064 665b 6364 662e  .        df[cdf.
-0000d7c0: 7374 6174 5f63 6f6c 5d20 3d20 2750 6572  stat_col] = 'Per
-0000d7d0: 6365 6e74 2045 7863 6565 6461 6e63 6527  cent Exceedance'
-0000d7e0: 0d0a 2020 2020 2020 2020 6466 5b63 6466  ..        df[cdf
-0000d7f0: 2e74 6872 6573 686f 6c64 5f63 6f6c 5d20  .threshold_col] 
-0000d800: 3d20 6627 7b74 6872 6573 686f 6c64 7d27  = f'{threshold}'
-0000d810: 0d0a 2020 2020 2020 2020 6966 2074 6872  ..        if thr
-0000d820: 6573 686f 6c64 5f69 735f 6578 6365 6564  eshold_is_exceed
-0000d830: 616e 6365 3a0d 0a20 2020 2020 2020 2020  ance:..         
-0000d840: 2020 2064 665b 6364 662e 7468 7265 7368     df[cdf.thresh
-0000d850: 6f6c 645f 636f 6c5d 203d 2027 3c27 202b  old_col] = '<' +
-0000d860: 2064 665b 6364 662e 7468 7265 7368 6f6c   df[cdf.threshol
-0000d870: 645f 636f 6c5d 0d0a 2020 2020 2020 2020  d_col]..        
-0000d880: 0d0a 2020 2020 2020 2020 2320 5265 7365  ..        # Rese
-0000d890: 7420 696e 6465 780d 0a20 2020 2020 2020  t index..       
-0000d8a0: 2064 6620 3d20 6466 2e72 6573 6574 5f69   df = df.reset_i
-0000d8b0: 6e64 6578 2829 0d0a 2020 2020 2020 2020  ndex()..        
-0000d8c0: 0d0a 2020 2020 2020 2020 2320 5265 6f72  ..        # Reor
-0000d8d0: 6465 7220 636f 6c75 6d6e 730d 0a20 2020  der columns..   
-0000d8e0: 2020 2020 206f 7574 7075 745f 636f 6c73       output_cols
-0000d8f0: 203d 205b 6364 662e 7374 6174 5f63 6f6c   = [cdf.stat_col
-0000d900: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000d910: 2020 2020 2020 2020 2020 6364 662e 7468            cdf.th
-0000d920: 7265 7368 6f6c 645f 636f 6c2c 0d0a 2020  reshold_col,..  
+0000d740: 2027 2076 616c 7565 2873 2920 6967 6e6f   ' value(s) igno
+0000d750: 7265 6429 270d 0a20 2020 2020 2020 2020  red)'..         
+0000d760: 2020 2029 0d0a 2020 2020 2020 2020 0d0a     )..        ..
+0000d770: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+0000d780: 2061 2063 6f6c 756d 6e20 7468 6174 2069   a column that i
+0000d790: 6e64 6963 6174 6573 2074 6865 2067 656e  ndicates the gen
+0000d7a0: 6572 6174 6564 2073 7461 7469 7374 6963  erated statistic
+0000d7b0: 200d 0a20 2020 2020 2020 2064 665b 6364   ..        df[cd
+0000d7c0: 662e 7374 6174 5f63 6f6c 5d20 3d20 2750  f.stat_col] = 'P
+0000d7d0: 6572 6365 6e74 2045 7863 6565 6461 6e63  ercent Exceedanc
+0000d7e0: 6527 0d0a 2020 2020 2020 2020 6466 5b63  e'..        df[c
+0000d7f0: 6466 2e74 6872 6573 686f 6c64 5f63 6f6c  df.threshold_col
+0000d800: 5d20 3d20 6627 7b74 6872 6573 686f 6c64  ] = f'{threshold
+0000d810: 7d27 0d0a 2020 2020 2020 2020 6966 2074  }'..        if t
+0000d820: 6872 6573 686f 6c64 5f69 735f 6578 6365  hreshold_is_exce
+0000d830: 6564 616e 6365 3a0d 0a20 2020 2020 2020  edance:..       
+0000d840: 2020 2020 2064 665b 6364 662e 7468 7265       df[cdf.thre
+0000d850: 7368 6f6c 645f 636f 6c5d 203d 2027 3c27  shold_col] = '<'
+0000d860: 202b 2064 665b 6364 662e 7468 7265 7368   + df[cdf.thresh
+0000d870: 6f6c 645f 636f 6c5d 0d0a 2020 2020 2020  old_col]..      
+0000d880: 2020 0d0a 2020 2020 2020 2020 2320 5265    ..        # Re
+0000d890: 7365 7420 696e 6465 780d 0a20 2020 2020  set index..     
+0000d8a0: 2020 2064 6620 3d20 6466 2e72 6573 6574     df = df.reset
+0000d8b0: 5f69 6e64 6578 2829 0d0a 2020 2020 2020  _index()..      
+0000d8c0: 2020 0d0a 2020 2020 2020 2020 2320 5265    ..        # Re
+0000d8d0: 6f72 6465 7220 636f 6c75 6d6e 730d 0a20  order columns.. 
+0000d8e0: 2020 2020 2020 206f 7574 7075 745f 636f         output_co
+0000d8f0: 6c73 203d 205b 6364 662e 7374 6174 5f63  ls = [cdf.stat_c
+0000d900: 6f6c 2c0d 0a20 2020 2020 2020 2020 2020  ol,..           
+0000d910: 2020 2020 2020 2020 2020 2020 6364 662e              cdf.
+0000d920: 7468 7265 7368 6f6c 645f 636f 6c2c 0d0a  threshold_col,..
 0000d930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d940: 2020 2020 2063 6466 2e72 6573 756c 745f       cdf.result_
-0000d950: 636f 6c2c 0d0a 2020 2020 2020 2020 2020  col,..          
-0000d960: 2020 2020 2020 2020 2020 2020 2063 6466               cdf
-0000d970: 2e6e 756d 6572 6963 5f63 6f6c 2c0d 0a20  .numeric_col,.. 
-0000d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d990: 2020 2020 2020 6364 662e 6578 6365 6564        cdf.exceed
-0000d9a0: 616e 6365 735f 636f 6c2c 0d0a 2020 2020  ances_col,..    
+0000d940: 2020 2020 2020 2063 6466 2e72 6573 756c         cdf.resul
+0000d950: 745f 636f 6c2c 0d0a 2020 2020 2020 2020  t_col,..        
+0000d960: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000d970: 6466 2e6e 756d 6572 6963 5f63 6f6c 2c0d  df.numeric_col,.
+0000d980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d990: 2020 2020 2020 2020 6364 662e 6578 6365          cdf.exce
+0000d9a0: 6564 616e 6365 735f 636f 6c2c 0d0a 2020  edances_col,..  
 0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9c0: 2020 2063 6466 2e6e 6f6e 5f65 7863 6565     cdf.non_excee
-0000d9d0: 6461 6e63 6573 5f63 6f6c 2c0d 0a20 2020  dances_col,..   
+0000d9c0: 2020 2020 2063 6466 2e6e 6f6e 5f65 7863       cdf.non_exc
+0000d9d0: 6565 6461 6e63 6573 5f63 6f6c 2c0d 0a20  eedances_col,.. 
 0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9f0: 2020 2020 6364 662e 6967 6e6f 7265 645f      cdf.ignored_
-0000da00: 636f 6c5d 0d0a 2020 2020 2020 2020 0d0a  col]..        ..
-0000da10: 2020 2020 2020 2020 6966 2067 726f 7570          if group
-0000da20: 6279 5f63 6f6c 7320 3d3d 204e 6f6e 653a  by_cols == None:
-0000da30: 0d0a 2020 2020 2020 2020 2020 2020 6364  ..            cd
-0000da40: 662e 6461 7461 203d 2064 665b 6f75 7470  f.data = df[outp
-0000da50: 7574 5f63 6f6c 735d 0d0a 2020 2020 2020  ut_cols]..      
-0000da60: 2020 656c 6966 2028 616c 6c28 6973 696e    elif (all(isin
-0000da70: 7374 616e 6365 286e 616d 652c 2073 7472  stance(name, str
-0000da80: 2920 666f 7220 6e61 6d65 2069 6e20 6772  ) for name in gr
-0000da90: 6f75 7062 795f 636f 6c73 2929 3a0d 0a20  oupby_cols)):.. 
-0000daa0: 2020 2020 2020 2020 2020 2063 6466 2e64             cdf.d
-0000dab0: 6174 6120 3d20 6466 5b67 726f 7570 6279  ata = df[groupby
-0000dac0: 5f63 6f6c 7320 2b20 6f75 7470 7574 5f63  _cols + output_c
-0000dad0: 6f6c 735d 0d0a 2020 2020 2020 2020 656c  ols]..        el
-0000dae0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000daf0: 2063 6466 2e64 6174 6120 3d20 6466 5b67   cdf.data = df[g
-0000db00: 726f 7570 6279 5f63 6f6c 735b 2d31 5d20  roupby_cols[-1] 
-0000db10: 2b20 6f75 7470 7574 5f63 6f6c 735d 0d0a  + output_cols]..
-0000db20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000db30: 2020 2320 4d65 7267 6520 636f 756e 7420    # Merge count 
-0000db40: 696e 666f 0d0a 2020 2020 2020 2020 6966  info..        if
-0000db50: 2063 6f75 6e74 5f63 6f6c 7320 213d 204e   count_cols != N
-0000db60: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-0000db70: 2020 6364 662e 6461 7461 203d 2073 656c    cdf.data = sel
-0000db80: 662e 6d65 7267 655f 636f 756e 7473 2863  f.merge_counts(c
-0000db90: 6466 2e64 6174 612c 0d0a 2020 2020 2020  df.data,..      
+0000d9f0: 2020 2020 2020 6364 662e 6967 6e6f 7265        cdf.ignore
+0000da00: 645f 636f 6c5d 0d0a 2020 2020 2020 2020  d_col]..        
+0000da10: 0d0a 2020 2020 2020 2020 6966 2067 726f  ..        if gro
+0000da20: 7570 6279 5f63 6f6c 7320 3d3d 204e 6f6e  upby_cols == Non
+0000da30: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000da40: 6364 662e 6461 7461 203d 2064 665b 6f75  cdf.data = df[ou
+0000da50: 7470 7574 5f63 6f6c 735d 0d0a 2020 2020  tput_cols]..    
+0000da60: 2020 2020 656c 6966 2028 616c 6c28 6973      elif (all(is
+0000da70: 696e 7374 616e 6365 286e 616d 652c 2073  instance(name, s
+0000da80: 7472 2920 666f 7220 6e61 6d65 2069 6e20  tr) for name in 
+0000da90: 6772 6f75 7062 795f 636f 6c73 2929 3a0d  groupby_cols)):.
+0000daa0: 0a20 2020 2020 2020 2020 2020 2063 6466  .            cdf
+0000dab0: 2e64 6174 6120 3d20 6466 5b67 726f 7570  .data = df[group
+0000dac0: 6279 5f63 6f6c 7320 2b20 6f75 7470 7574  by_cols + output
+0000dad0: 5f63 6f6c 735d 0d0a 2020 2020 2020 2020  _cols]..        
+0000dae0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0000daf0: 2020 2063 6466 2e64 6174 6120 3d20 6466     cdf.data = df
+0000db00: 5b67 726f 7570 6279 5f63 6f6c 735b 2d31  [groupby_cols[-1
+0000db10: 5d20 2b20 6f75 7470 7574 5f63 6f6c 735d  ] + output_cols]
+0000db20: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0000db30: 2020 2020 2320 4d65 7267 6520 636f 756e      # Merge coun
+0000db40: 7420 696e 666f 0d0a 2020 2020 2020 2020  t info..        
+0000db50: 6966 2063 6f75 6e74 5f63 6f6c 7320 213d  if count_cols !=
+0000db60: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0000db70: 2020 2020 6364 662e 6461 7461 203d 2073      cdf.data = s
+0000db80: 656c 662e 6d65 7267 655f 636f 756e 7473  elf.merge_counts
+0000db90: 2863 6466 2e64 6174 612c 0d0a 2020 2020  (cdf.data,..    
 0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbc0: 2020 2063 6f75 6e74 5f63 6f6c 732c 0d0a     count_cols,..
-0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbc0: 2020 2020 2063 6f75 6e74 5f63 6f6c 732c       count_cols,
+0000dbd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbf0: 2020 2020 2020 2020 2067 726f 7570 6279           groupby
-0000dc00: 5f63 6f6c 7329 0d0a 2020 2020 2020 2020  _cols)..        
-0000dc10: 0d0a 2020 2020 2020 2020 2320 5265 706c  ..        # Repl
-0000dc20: 6163 6520 6f72 2072 6574 7572 6e20 7265  ace or return re
-0000dc30: 7375 6c74 0d0a 2020 2020 2020 2020 6966  sult..        if
-0000dc40: 2069 6e70 6c61 6365 3a0d 0a20 2020 2020   inplace:..     
-0000dc50: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-0000dc60: 203d 2063 6466 2e64 6174 610d 0a20 2020   = cdf.data..   
-0000dc70: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-0000dc80: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-0000dc90: 6466 2e64 6174 610d 0a                   df.data..
+0000dbf0: 2020 2020 2020 2020 2020 2067 726f 7570             group
+0000dc00: 6279 5f63 6f6c 7329 0d0a 2020 2020 2020  by_cols)..      
+0000dc10: 2020 0d0a 2020 2020 2020 2020 2320 5265    ..        # Re
+0000dc20: 706c 6163 6520 6f72 2072 6574 7572 6e20  place or return 
+0000dc30: 7265 7375 6c74 0d0a 2020 2020 2020 2020  result..        
+0000dc40: 6966 2069 6e70 6c61 6365 3a0d 0a20 2020  if inplace:..   
+0000dc50: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
+0000dc60: 7461 203d 2063 6466 2e64 6174 610d 0a20  ta = cdf.data.. 
+0000dc70: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000dc80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000dc90: 2063 6466 2e64 6174 610d 0a               cdf.data..
```

### Comparing `censoredsummarystats-0.2.2/censoredsummarystats/utils.py` & `censoredsummarystats-0.2.3/censoredsummarystats/utils.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.2/LICENSE` & `censoredsummarystats-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.2/pyproject.toml` & `censoredsummarystats-0.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censoredsummarystats"
-version = "0.2.2"
+version = "0.2.3"
 description = "A python package for calculating summary stats on censored data (data that contains < and > symbols)."
 authors = ["Kurt van Ness <vanness.kurt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kurtvanness/CensoredSummaryStats"
 license = "Apache-2.0"
 packages = [{include = "censoredsummarystats"}]
```

### Comparing `censoredsummarystats-0.2.2/README.md` & `censoredsummarystats-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.2/PKG-INFO` & `censoredsummarystats-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censoredsummarystats
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python package for calculating summary stats on censored data (data that contains < and > symbols).
 Home-page: https://github.com/kurtvanness/CensoredSummaryStats
 License: Apache-2.0
 Author: Kurt van Ness
 Author-email: vanness.kurt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

