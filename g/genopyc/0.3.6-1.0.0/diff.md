# Comparing `tmp/genopyc-0.3.6-py3-none-any.whl.zip` & `tmp/genopyc-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 18390 bytes, number of entries: 7
--rwxrwxrwx  2.0 unx      881 b- defN 23-Jun-06 08:23 genopyc/__init__.py
--rwxrwxrwx  2.0 unx    24058 b- defN 23-May-31 11:38 genopyc/genopyc.py
--rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-06 08:24 genopyc-0.3.6.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      463 b- defN 23-Jun-06 08:24 genopyc-0.3.6.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-06 08:24 genopyc-0.3.6.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-06 08:24 genopyc-0.3.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      540 b- defN 23-Jun-06 08:24 genopyc-0.3.6.dist-info/RECORD
-7 files, 60565 bytes uncompressed, 17436 bytes compressed:  71.2%
+Zip file size: 20537 bytes, number of entries: 7
+-rwxrwxrwx  2.0 unx      917 b- defN 23-Jun-21 11:24 genopyc/__init__.py
+-rwxrwxrwx  2.0 unx    32925 b- defN 23-Jun-21 11:22 genopyc/genopyc.py
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-21 11:24 genopyc-1.0.0.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-21 11:24 genopyc-1.0.0.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-21 11:24 genopyc-1.0.0.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-21 11:24 genopyc-1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      540 b- defN 23-Jun-21 11:24 genopyc-1.0.0.dist-info/RECORD
+7 files, 69601 bytes uncompressed, 19583 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: genopyc/__init__.py
 Comment: 
 
 Filename: genopyc/genopyc.py
 Comment: 
 
-Filename: genopyc-0.3.6.dist-info/LICENSE.txt
+Filename: genopyc-1.0.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-0.3.6.dist-info/METADATA
+Filename: genopyc-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-0.3.6.dist-info/WHEEL
+Filename: genopyc-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-0.3.6.dist-info/top_level.txt
+Filename: genopyc-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-0.3.6.dist-info/RECORD
+Filename: genopyc-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genopyc/__init__.py

```diff
@@ -13,8 +13,9 @@
 from genopyc.genopyc import get_eqtl_variant
 from genopyc.genopyc import get_variant_info
 from genopyc.genopyc import get_variant_info_many
 from genopyc.genopyc import get_eqtl_df
 from genopyc.genopyc import GetLDMatrix
 from genopyc.genopyc import PairwiseLD
 from genopyc.genopyc import ConvertVariantsForOT
-from genopyc.genopyc import OT_L2G
+from genopyc.genopyc import OT_L2G
+from genopyc.genopyc import FuEnViz
```

## genopyc/genopyc.py

```diff
@@ -1,11 +1,23 @@
 import requests
 import pandas as pd
-from tqdm import tqdm
+import biomapy as bp
+import networkx as nx
 import numpy as np
+import pandas as pd
+import requests
+from gprofiler import GProfiler
+import igraph as ig 
+import warnings
+warnings.filterwarnings('ignore')
+import dash
+import dash_core_components as dcc
+import dash_html_components as html
+from dash.dependencies import Input,Output
+import dash_cytoscape as cyto
 
 
 def get_associations(efotrait,verbose=False):
     """Retrieve snps associated to an EFO trait"""
     df=pd.DataFrame(columns=['variantid','p-value','risk_allele','RAF','beta','CI','mapped_gene'])
     http= 'https://www.ebi.ac.uk/gwas/rest/api/efoTraits/%s/associations' %(efotrait)
     if verbose:
@@ -628,12 +640,197 @@
     if output=='all':
         return results
     elif output=='GenScor':
         return {key:[value for value in values if value[1]>score] for (key,values) in results.items()}
     else:
         return list(set(sum([[value[0] for value in values if value[1]>score] for (key,values) in results.items()],[])))
     
+
+
+
+#Function enrichment
+def FuEnViz(ListOfGenes):
+    def ParseInteractome():
+        location = os.path.dirname(os.path.realpath(__file__))
+        Interactome=pd.read_csv(os.path.join(location, 'data', 'hippie_interactome.sif'),header=None, sep=' ',usecols=[0,2])
+        Interactome.columns=['source','target']
+        # if ((args.sep=='space') & (args.id=='symbol')):
+        Interactome.source=bp.gene_mapping_many(Interactome.source.astype(int).tolist(),'entrez','symbol')
+        Interactome.target=bp.gene_mapping_many(Interactome.target.astype(int).tolist(),'entrez','symbol')
+        Interactome.dropna(inplace=True)
+        return Interactome
+
+
+
+    def EnrichmentAnalisys(ListOfGenes):
+        ## PERFORM ENRICHMENT ANALISYS##
+        gp = GProfiler(return_dataframe=True)
+        Enrichment=gp.profile(organism='hsapiens',
+                    query=ListOfGenes,
+                    significance_threshold_method='bonferroni',
+                    no_iea=True,
+                    no_evidences=False)
+        return Enrichment
+
+    def BuildGraph(SubGraph,EnrichmentDataframe):
+        ## implement the possibility to make different layouts and to add attributes to the edges and to the nodes
+        EnrichmentDataframe.dropna(subset = 'p_value',inplace = True)
+        ig_subgraph=ig.Graph.from_networkx(SubGraph)
+        pos_= dict(zip([v['_nx_name'] for v in ig_subgraph.vs],[coord for coord in ig_subgraph.layout_auto()]))
+        app=dash.Dash(__name__)
+        cyto_node_data=list(
+                            zip(
+                                    pos_.keys(),
+                                    [coord[0] for coord in pos_.values()],
+                                    [coord[1] for coord in pos_.values()]
+                                    
+                                    
+                                )
+                        )
+        nodes = [
+        {
+            'data': {'id': str(_id), 'label':str(_id)},
+            'position': {'x': 120*x, 'y': 120*y}
+        }
+        for _id, x, y, in cyto_node_data
+        ]
+
+
+
+        edges = [
+            {'data': {'source': source, 'target': target}}
+            for source, target in SubGraph.edges()
+            ]
+
+        elements = nodes + edges
+
+
+
+
+        default_stylesheet = [
+            {
+                'selector': 'node',
+                'style': {
+                    'background-color': '#F5CEC5',
+                    'border-color':'black',
+                    'border-width':'1',
+                    'label': 'data(label)',
+                    'width':'60',
+                    'height':'60'
+                }
+            },
+            {
+                'selector': 'edge',
+                'style': {
+                    'line-color': 'red',
+                    'width':'1'
+                }
+            }
+        ]
+
+        app.layout=html.Div([
+                            html.Header(html.H1(['Function enrichment analysis topology visualization'],
+                            style={'textAlign':'center','paddingBottom':'50px','border':'0px solid','border-bottom':'1px solid black'})),
+
+                            html.Main([html.Div([html.Label('P-value Slider'),
+                                                dcc.Slider(id='pvalue_slider',
+                                                        min=round(-np.log10(EnrichmentDataframe['p_value'].max())),
+                                                        max=round(-np.log10(EnrichmentDataframe['p_value'].min())),
+                                                        value=round(-np.log10(EnrichmentDataframe['p_value'].max())),
+                                                        marks=dict(list(zip(set(sorted([round(el) for el in -np.log10(EnrichmentDataframe.p_value.tolist())])),
+                                                        [{} for value in set([round(el) for el in -np.log10(EnrichmentDataframe.p_value.tolist())])]))),
+                                                            step=None),
+                                                    
+                                                    html.Div(id='updatemode-output-container', style={'marginTop': 20}),
+                                                    
+                                                    html.Br(style={'lineHeight':'4'}),
+                                                    html.Label('Sources'),
+                                                    dcc.RadioItems(id='sources',
+                                                                    labelStyle={'display': 'flex'}
+                                                                    ),
+                                                    html.Br(style={'lineHeight':'4'}), 
+                                                    html.Label('Function'),
+                                                    dcc.Dropdown(id='function_dropdown'),
+                                                    html.P(id='cytoscape-mouseoverNodeData-output')
+                                                    
+
+
+                                                    
+                                                    
+                                                ],
+                                                style={'width':'20%','display':'inline-block','float':'left','paddingTop':'20px','paddingLeft':'50px'}
+                                            ),
+                                    
+                                    
+                                    
+                                    html.Div([cyto.Cytoscape(id='cytoscape_network',
+                                                            layout={'name': 'preset'},
+                                                            style={'width': '100%', 'height': '800px'},
+                                                            stylesheet=default_stylesheet,
+                                                            elements=elements,
+                                                            autoRefreshLayout=True
+                                                            )
+                                                
+                                                ],
+                                    style={'width':'75%','float':'right','position':'relative','top':'20px'}
+                                            
+                                            )])
+                            
+                            ])
+
+
+
+
+
+        @app.callback(Output('updatemode-output-container', 'children'),
+                    Input('pvalue_slider', 'value'))
+        def display_value(value):
+            return '-log10(P_Value): %s' %value  
+
+        @app.callback(
+            Output('sources', 'options'),
+            Input('pvalue_slider', 'value'))
+        def set_sources(selected_pvalue):
+            return [{'label': i, 'value': i} for i in set(EnrichmentDataframe[-np.log10(EnrichmentDataframe.p_value)>=selected_pvalue].source.tolist())]
+
+
+        @app.callback(Output('function_dropdown', 'options'),
+                    Input('pvalue_slider', 'value'),
+                    Input('sources', 'value'))
+        def set_functions(p_value,source):
+            return [{'label': i, 'value': i} for i in set(EnrichmentDataframe[(-np.log10(EnrichmentDataframe.p_value)>=p_value)&(EnrichmentDataframe.source==source)].name.tolist())]
+
+
+        @app.callback(Output('cytoscape_network', 'stylesheet'),
+                    Input('sources', 'value'),
+                    Input('function_dropdown', 'value'))
+
+
+
+        def update_network(fsource,ffunction):
+            """Filter the functions in the dataset"""
+            try:
+                filt_enrich=EnrichmentDataframe[(EnrichmentDataframe.name==ffunction)&(EnrichmentDataframe.source==fsource)].intersections.values[0]
+
+                new_stylesheet=[{
+                                    'selector':"[id='%s']"%ele ,
+                                    'style': {
+                                        'background-color': 'black',
+                                        'line-color': 'black'
+                                    }
+                                    } for ele in filt_enrich]
             
-            
-    
+                return default_stylesheet+new_stylesheet
+            except:
+                return default_stylesheet
+        
 
+        
+        
+        app.run_server()
+    
+    EdgeFile=ParseInteractome()
 
+    HippieNet = nx.from_pandas_edgelist(EdgeFile)
+    SubG = HippieNet.subgraph(ListOfGenes)
+    Enrichment = EnrichmentAnalisys(ListOfGenes)
+    BuildGraph(SubG,Enrichment)
```

## Comparing `genopyc-0.3.6.dist-info/LICENSE.txt` & `genopyc-1.0.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

