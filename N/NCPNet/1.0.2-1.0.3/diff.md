# Comparing `tmp/NCPNet-1.0.2.tar.gz` & `tmp/NCPNet-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NCPNet-1.0.2.tar", last modified: Tue Jun 20 07:59:31 2023, max compression
+gzip compressed data, was "NCPNet-1.0.3.tar", last modified: Wed Jun 21 12:48:13 2023, max compression
```

## Comparing `NCPNet-1.0.2.tar` & `NCPNet-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-20 07:59:31.125763 NCPNet-1.0.2/
--rw-rw-r--   0 wgj       (1024) wgj       (1025)     1073 2023-06-13 10:35:09.000000 NCPNet-1.0.2/LICENSE
-drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-20 07:59:31.125763 NCPNet-1.0.2/NCPNet/
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)      119 2023-06-13 06:11:03.000000 NCPNet-1.0.2/NCPNet/__init__.py
-drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-20 07:59:31.125763 NCPNet-1.0.2/NCPNet/approaches/
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     4859 2023-06-13 03:06:30.000000 NCPNet-1.0.2/NCPNet/approaches/Decoder.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     5326 2023-06-13 02:30:59.000000 NCPNet-1.0.2/NCPNet/approaches/Encoder.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     2720 2023-06-13 05:48:20.000000 NCPNet-1.0.2/NCPNet/approaches/PairEncoder.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)      216 2023-06-13 05:48:00.000000 NCPNet-1.0.2/NCPNet/approaches/__init__.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     2843 2023-06-13 05:50:16.000000 NCPNet-1.0.2/NCPNet/approaches/method.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)    26879 2023-06-13 09:10:39.000000 NCPNet-1.0.2/NCPNet/brain_data.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     4988 2023-06-13 03:06:48.000000 NCPNet-1.0.2/NCPNet/task.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)    22572 2023-06-13 03:07:04.000000 NCPNet-1.0.2/NCPNet/trainer.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     1942 2023-06-08 13:29:28.000000 NCPNet-1.0.2/NCPNet/utils.py
-drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-20 07:59:31.125763 NCPNet-1.0.2/NCPNet.egg-info/
--rw-rw-r--   0 wgj       (1024) wgj       (1025)     2168 2023-06-20 07:59:31.000000 NCPNet-1.0.2/NCPNet.egg-info/PKG-INFO
--rw-rw-r--   0 wgj       (1024) wgj       (1025)      413 2023-06-20 07:59:31.000000 NCPNet-1.0.2/NCPNet.egg-info/SOURCES.txt
--rw-rw-r--   0 wgj       (1024) wgj       (1025)        1 2023-06-20 07:59:31.000000 NCPNet-1.0.2/NCPNet.egg-info/dependency_links.txt
--rw-rw-r--   0 wgj       (1024) wgj       (1025)      176 2023-06-20 07:59:31.000000 NCPNet-1.0.2/NCPNet.egg-info/requires.txt
--rw-rw-r--   0 wgj       (1024) wgj       (1025)        7 2023-06-20 07:59:31.000000 NCPNet-1.0.2/NCPNet.egg-info/top_level.txt
--rw-rw-r--   0 wgj       (1024) wgj       (1025)     2168 2023-06-20 07:59:31.125763 NCPNet-1.0.2/PKG-INFO
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     1670 2023-06-16 05:53:41.000000 NCPNet-1.0.2/README.md
--rw-rw-r--   0 wgj       (1024) wgj       (1025)       38 2023-06-20 07:59:31.125763 NCPNet-1.0.2/setup.cfg
--rw-rw-r--   0 wgj       (1024) wgj       (1025)     1113 2023-06-20 07:59:29.000000 NCPNet-1.0.2/setup.py
+drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-21 12:48:13.278123 NCPNet-1.0.3/
+-rw-rw-r--   0 wgj       (1024) wgj       (1025)     1073 2023-06-13 10:35:09.000000 NCPNet-1.0.3/LICENSE
+drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-21 12:48:13.278123 NCPNet-1.0.3/NCPNet/
+-rwxrwxr-x   0 wgj       (1024) wgj       (1025)      160 2023-06-21 12:23:37.000000 NCPNet-1.0.3/NCPNet/__init__.py
+-rw-rw-r--   0 wgj       (1024) wgj       (1025)       83 2023-06-21 12:27:02.000000 NCPNet-1.0.3/NCPNet/__main__.py
+drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-21 12:48:13.278123 NCPNet-1.0.3/NCPNet/approaches/
+-rwxrwxr-x   0 wgj       (1024) wgj       (1025)     4859 2023-06-13 03:06:30.000000 NCPNet-1.0.3/NCPNet/approaches/Decoder.py
+-rwxrwxr-x   0 wgj       (1024) wgj       (1025)     5326 2023-06-13 02:30:59.000000 NCPNet-1.0.3/NCPNet/approaches/Encoder.py
+-rwxrwxr-x   0 wgj       (1024) wgj       (1025)     2921 2023-06-21 12:09:19.000000 NCPNet-1.0.3/NCPNet/approaches/PairEncoder.py
+-rwxrwxr-x   0 wgj       (1024) wgj       (1025)      217 2023-06-21 11:53:03.000000 NCPNet-1.0.3/NCPNet/approaches/__init__.py
+-rwxrwxr-x   0 wgj       (1024) wgj       (1025)     6961 2023-06-21 11:58:54.000000 NCPNet-1.0.3/NCPNet/approaches/method.py
+-rwxrwxr-x   0 wgj       (1024) wgj       (1025)    27693 2023-06-21 12:26:48.000000 NCPNet-1.0.3/NCPNet/brain_data.py
+-rw-rw-r--   0 wgj       (1024) wgj       (1025)     2086 2023-06-21 12:33:41.000000 NCPNet-1.0.3/NCPNet/predict.py
+-rwxrwxr-x   0 wgj       (1024) wgj       (1025)     4988 2023-06-13 03:06:48.000000 NCPNet-1.0.3/NCPNet/task.py
+-rwxrwxr-x   0 wgj       (1024) wgj       (1025)    22453 2023-06-21 02:52:51.000000 NCPNet-1.0.3/NCPNet/trainer.py
+-rwxrwxr-x   0 wgj       (1024) wgj       (1025)     2107 2023-06-20 10:43:06.000000 NCPNet-1.0.3/NCPNet/utils.py
+drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-21 12:48:13.278123 NCPNet-1.0.3/NCPNet.egg-info/
+-rw-rw-r--   0 wgj       (1024) wgj       (1025)     3295 2023-06-21 12:48:13.000000 NCPNet-1.0.3/NCPNet.egg-info/PKG-INFO
+-rw-rw-r--   0 wgj       (1024) wgj       (1025)      450 2023-06-21 12:48:13.000000 NCPNet-1.0.3/NCPNet.egg-info/SOURCES.txt
+-rw-rw-r--   0 wgj       (1024) wgj       (1025)        1 2023-06-21 12:48:13.000000 NCPNet-1.0.3/NCPNet.egg-info/dependency_links.txt
+-rw-rw-r--   0 wgj       (1024) wgj       (1025)      180 2023-06-21 12:48:13.000000 NCPNet-1.0.3/NCPNet.egg-info/requires.txt
+-rw-rw-r--   0 wgj       (1024) wgj       (1025)        7 2023-06-21 12:48:13.000000 NCPNet-1.0.3/NCPNet.egg-info/top_level.txt
+-rw-rw-r--   0 wgj       (1024) wgj       (1025)     3295 2023-06-21 12:48:13.278123 NCPNet-1.0.3/PKG-INFO
+-rwxrwxr-x   0 wgj       (1024) wgj       (1025)     2797 2023-06-21 12:47:26.000000 NCPNet-1.0.3/README.md
+-rw-rw-r--   0 wgj       (1024) wgj       (1025)       38 2023-06-21 12:48:13.278123 NCPNet-1.0.3/setup.cfg
+-rw-rw-r--   0 wgj       (1024) wgj       (1025)     1128 2023-06-21 12:46:00.000000 NCPNet-1.0.3/setup.py
```

### Comparing `NCPNet-1.0.2/LICENSE` & `NCPNet-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NCPNet-1.0.2/NCPNet/approaches/Decoder.py` & `NCPNet-1.0.3/NCPNet/approaches/Decoder.py`

 * *Files identical despite different names*

### Comparing `NCPNet-1.0.2/NCPNet/approaches/Encoder.py` & `NCPNet-1.0.3/NCPNet/approaches/Encoder.py`

 * *Files identical despite different names*

### Comparing `NCPNet-1.0.2/NCPNet/approaches/PairEncoder.py` & `NCPNet-1.0.3/NCPNet/approaches/PairEncoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,20 +51,23 @@
         self.act_f1=nn.LeakyReLU(0.05)
         self.dp1=torch.nn.Dropout(inplace=True)
         
         self.conv2=torch.nn.Conv1d(int(config['out_channels']*0.5),config['out_channels']-int(config['out_channels']*0.5),kernel_size=1,bias=False)
         self.act_f2=nn.LeakyReLU(0.05)
         self.dp2=torch.nn.Dropout(inplace=True)
     def forward(self,z,neighbor=None):
-        x=self.lookupneigh(z,neighbor)
-        x=x.permute((0,2,1)).contiguous()
-        x=self.conv1(x)
-        x=self.act_f1(x)
-        x1=self.dp1(x)
-        x2=self.conv2(x1)
-        x2=self.act_f2(x2)
-        x2=self.dp2(x2)
-        x=torch.cat([x1,x2],dim=1)
-        x=F.adaptive_max_pool1d(x,1).squeeze()
-    
-        #x=x.mean(dim=2)
-        return x
+        if len(neighbor.squeeze())==0:
+            return torch.zeros(size=(len(neighbor),self.model_config['out_channels']))
+        else:
+            x=self.lookupneigh(z,neighbor)
+            x=x.permute((0,2,1)).contiguous()
+            x=self.conv1(x)
+            x=self.act_f1(x)
+            x1=self.dp1(x)
+            x2=self.conv2(x1)
+            x2=self.act_f2(x2)
+            x2=self.dp2(x2)
+            x=torch.cat([x1,x2],dim=1)
+            x=F.adaptive_max_pool1d(x,1)
+            x=x.squeeze(-1)
+            #x=x.mean(dim=2)
+            return x
```

### Comparing `NCPNet-1.0.2/NCPNet/brain_data.py` & `NCPNet-1.0.3/NCPNet/brain_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import torch_geometric
 from torch_geometric.data import InMemoryDataset, download_url
 from torch_geometric.io import read_planetoid_data
 from torch_geometric.data import Data
 from torch_geometric.utils import negative_sampling
 import networkx as nx
 import random
+from NCPNet.utils import edge_index2Graph
 
 class HemiBrain(InMemoryDataset):
     r"""
     Args:
         root (string): Root directory where the dataset should be saved.
         transform (callable, optional): A function/transform that takes in an
             :obj:`torch_geometric.data.Data` object and returns a transformed
@@ -303,17 +304,19 @@
                     if j !=n:
                         for kj in self.nxg[j]:
                             if kj not in self.nxg[n] and kj!=n:
                                 self.nxg[n].add(kj)
         self.cached_nxg_neighbors=None
         self.step=0
         self.max_pad_num=None
+    
     def get_neighboor(self,edge_index,mode='inter',max_num=30):
         edge_index_list=edge_index.cpu().T.tolist()
         res=[]
+        
      
         if mode=='inter':
   
             for edges in edge_index_list:
                 u,v=tuple(edges)
                 u_set,v_set=self.nxg[u],self.nxg[v]
 
@@ -624,15 +627,32 @@
 
     def __repr__(self) -> str:
         return 'Celegans19-%s'%self.name
 class Celegans19_herm(Celegans19):
     def __init__(self,*args,**kwargs):
         kwargs['mode']='herm'
         super(self,Celegans19_herm).__init__(*args,**kwargs)
+class DIYbrain_networks(InMemoryDataset):
+    def __init__(self, root: str,split='node', transform: Optional[Callable] = None,
+                 pre_transform: Optional[Callable] = None,process=False,restore_split=None,device=None):
 
+        super().__init__(root, transform, pre_transform)
+        if device is None:
+            self.device='cpu'
+        else:
+            self.device=device
+        if process:
+            self._process()
+        if restore_split is None:
+            self.data, self.slices = torch.load(self.processed_paths[0],map_location=self.device)
+        elif isinstance(restore_split,str):
+            self.data= torch.load(restore_split,map_location=self.device)
+        self.data, self.slices = self.collate([self.data])
+    
+    
 class NxGraph(InMemoryDataset):
     url=None
     def __init__(self, root: Optional[str] = None, nxg='barbell',transform: Optional[Callable] = None, pre_transform: Optional[Callable] = None, pre_filter: Optional[Callable] = None,**kwargs):
         
         
         self.kwargs=kwargs
         if isinstance(nxg,str):
```

### Comparing `NCPNet-1.0.2/NCPNet/task.py` & `NCPNet-1.0.3/NCPNet/task.py`

 * *Files identical despite different names*

### Comparing `NCPNet-1.0.2/NCPNet/trainer.py` & `NCPNet-1.0.3/NCPNet/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,14 @@
         reconstruct_error=torch.abs(pred_graph-ground_truth).sum()
         print(reconstruct_error)
 
 
 class LinkPred_trainer(Base_Trainer):
 
     def update(self,batch):
-        torch.save(self.model,'/data/users/wgj/project/NDGNN_Neurips22_Realeased/runs/tsne_savemodel-%d.pt'%self.iter)
         self.model.train()
         self.optimizer.zero_grad()
         if len(batch)==6:
             x, edge_index, edge_attr, edge_label_index, edge_label,neighbor=batch
             out=self.model(x=x,edge_index=edge_index,edge_label_index=edge_label_index,neighbor=neighbor)
         elif len(batch)==5:
             x,edge_index, edge_attr, edge_label_index, edge_label=batch
```

### Comparing `NCPNet-1.0.2/NCPNet/utils.py` & `NCPNet-1.0.3/NCPNet/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 def load_config(path):
     if os.path.isfile(path):
         with open(path,'r') as fin:
             config=yaml.safe_load(fin)
         return config
     else:
         raise FileNotFoundError('Not found config file..')
+def find_directory(root_dir, target_file):
+    for root, dirs, files in os.walk(root_dir):
+        if target_file in files:
+            return root
+    return None
+
 def dict_sequential(obj):
     if isinstance(obj,dict):
         back={}
 
         for k,v in obj.items():
             back[k]=dict_sequential(v)
     elif isinstance(obj,np.ndarray) or isinstance(obj,torch.Tensor):
```

### Comparing `NCPNet-1.0.2/NCPNet.egg-info/PKG-INFO` & `NCPNet-1.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,38 @@
-Metadata-Version: 2.1
-Name: NCPNet
-Version: 1.0.2
-Summary: Learning synapse-level brain circuit networks. Include training, inferring, evaluation, and visualization.
-Home-page: https://github.com/mxz12119/NCPNet
-Author: Guojia Wan
-Author-email: guojiawan@whu.edu.cn
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # NCPNet
 ![PyPI](https://img.shields.io/pypi/v/NCPNet)![Packagist License](https://img.shields.io/packagist/l/mxz12119/NCPNet)
 
 
 ## 1. Brief Introduction
 Neuronal Circuit Prediction Network (NCPNet), a simple and effective model for inferring neuron-level connections in a brain circuit network.
-## 2. Environment and Dependencies
+## 2. Installation
+### Requirements
+* Linux
+* CUDA environment >=10.2
+* NVIDIA CUDA Compiler Driver NVCC version>=10.2. This is used for compiling the dependencies of torch_geometric: torch-cluster,torch-sparse,torch-scatter.
+* torch==1.8.0
+
+### Step 1
+1. Ensure that [nvcc](https://docs.nvidia.com/cuda/cuda-compiler-driver-nvcc/index.html) is accessible from terminal and version >=10.2
+
+```nvcc --version```
+
+If NVCC is not not included in your device,  it can be installed through the CUDA Toolkit. NVCC is a part of the [CUDA Toolkit](https://developer.nvidia.com/cuda-downloads?target_os=Linux).
+
+2. Ensure that CUDA is usable and version >=10.2
+```
+nvidia-smi |grep Version
+>>>CUDA Version: >=10.2
+```
+### Step 2
+Use pip to install NCPNet
+```
+pip install NCPNet
+```
+Note that it takes a long time to build torch-cluster,torch-sparse,and torch-scatter by pip. Don`t worry, just wait for a while.
 ### Our main dependencies:
 ```
 torch==1.8.0
 torch_geometric==2.0.1
 torch-cluster==1.5.9
 torch-sparse==0.6.12
 torch-scatter==2.0.8
@@ -30,15 +40,15 @@
 neuprint-python==0.4.25
 ```
 If you would like to reproduce our experiments and plots, please also install jupyter.
 ```
 pip install jupyter
 ```
 
-### Code structure:
+## Code structure:
 ```
 Source Code
 ├── data
 |   ├──Hemibrain
 |   └──C.Elegans
 ├── example
 ├── runs
@@ -48,33 +58,43 @@
 |   ├── brain_data.py
 |   ├── task.py
 |   ├── trainer.py
 |   └── utils.py
 └── requirements.txt
 ```
 ## Examples
-NCPNet uses configuration files (yaml) to control training and test.
+### 1. Easy train a model on *Drosophila* HemiBrain
+NCPNet uses a configuration file (yaml) to control training and test.
 
 Run 
 ```
-python src/main_run.py -c src/configs/fly_linkpred.yaml
+python main_run.py -c configs/linkpred.yaml
 ```
+linkpred.yaml include the hyperparameters of NCPNet.
+### 2. Predict  neuronal connection
+ Once you train a model, such as 'model.ncpnet', then use the following command to predict the probility between two neurons:
+ ```
+ python -m NCPNet -pred 1721996278 1722670151 -m model.ncpnet
+ ```
+ Response:
+ ```
+ Inferring the connection probability of (1721996278->1722670151)
+The score of (1721996278->1722670151): 0.874
+ ```
 ## Reproducibility of Our Paper
-Please try to use jupyter to reproduce our experiments in ./Plot_figure/
+Please try to use jupyter to reproduce our experiments in ./examples/
 
 ## Access Data
 ### Raw Data
 The *Drosophila* connectome is available at <https://www.janelia.org/project-team/flyem/hemibrain>.
 
 
 The *C.elegans* connectome is available at <https://wormwiring.org/>
 ### Preprocessed Data
 The data will be released after the review process.
-<!-- The *Drosophila* connectome can be downloaded at <https://drive.google.com/file/d/1FQVZkzAgaDXSO9Dl7ken6oAohIlzKqWD/view?usp=sharing>
 
-The *C.elegans* connectome is included in './data/'. -->
```

### Comparing `NCPNet-1.0.2/setup.py` & `NCPNet-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(
     name='NCPNet',
-    version='1.0.2',
+    version='1.0.3',
     author='Guojia Wan',
     author_email='guojiawan@whu.edu.cn',
     description='Learning synapse-level brain circuit networks. Include training, inferring, evaluation, and visualization.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mxz12119/NCPNet',
     packages=find_packages(),
@@ -21,15 +21,16 @@
         'navis==1.3.1',
         'neuprint-python==0.4.25',
         'networkx',
         'tqdm',
         'tensorboardx',
         'pandas',
         'numpy',
-        'scikit-learn'
+        'scikit-learn',
+        'zmq'
     ],
     python_requires='>=3.7',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
```

