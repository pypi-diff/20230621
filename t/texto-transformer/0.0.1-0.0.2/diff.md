# Comparing `tmp/texto_transformer-0.0.1.tar.gz` & `tmp/texto_transformer-0.0.2.tar.gz`

## Comparing `texto_transformer-0.0.1.tar` & `texto_transformer-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/requirements.txt
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/target/pylist.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/__init__.py
--rw-r--r--   0        0        0    40424 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/textotransformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/mensurador/__init__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/mensurador/medidas.py
--rw-r--r--   0        0        0    36781 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/mensurador/mensurador.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/mensurador/mensuradorenum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/modelo/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/modelo/modeloarguments.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/modelo/modeloenum.py
--rw-r--r--   0        0        0    32796 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/modelo/transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/pln/__init__.py
--rw-r--r--   0        0        0    15106 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/pln/pln.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/__init__.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/utilambiente.py
--rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/utilarquivo.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/utilconstantes.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/utiltempo.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/textotransformer/util/utiltexto.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/LICENSE
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 texto_transformer-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/__init__.py
+-rw-r--r--   0        0        0    52677 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/textotransformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/mensurador/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/mensurador/medidas.py
+-rw-r--r--   0        0        0    37639 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/mensurador/mensurador.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/mensurador/mensuradorenum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/modelo/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/modelo/modeloarguments.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/modelo/modeloenum.py
+-rw-r--r--   0        0        0    29287 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/modelo/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/pln/__init__.py
+-rw-r--r--   0        0        0    15485 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/pln/pln.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/__init__.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/utilambiente.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/utilarquivo.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/utilconstantes.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/utiltempo.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/textotransformer/util/utiltexto.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/README.md
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 texto_transformer-0.0.2/PKG-INFO
```

### Comparing `texto_transformer-0.0.1/textotransformer/textotransformer.py` & `texto_transformer-0.0.2/textotransformer/textotransformer.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,30 +11,31 @@
 from tqdm import trange
 
 # Biblioteca próprias
 from textotransformer.pln.pln import PLN
 from textotransformer.mensurador.mensurador import Mensurador
 from textotransformer.modelo.transformer import Transformer
 from textotransformer.modelo.modeloarguments import ModeloArgumentos
-from textotransformer.modelo.modeloenum import LISTATIPOCAMADA_NOME, EstrategiasPooling, listaTipoCamadas
+from textotransformer.modelo.modeloenum import LISTATIPOCAMADA_NOME
 from textotransformer.modelo.modeloenum import EstrategiasPooling
-from textotransformer.mensurador.mensuradorenum import PalavrasRelevantes 
+from textotransformer.modelo.modeloenum import listaTipoCamadas
+from textotransformer.mensurador.mensuradorenum import PalavrasRelevantes
 from textotransformer.util.utiltexto import encontrarIndiceSubLista
 
 logger = logging.getLogger(__name__)
 
 # Definição dos parâmetros do Modelo para os cálculos das Medidas
 modelo_argumentos = ModeloArgumentos(
         max_seq_len=512,
         pretrained_model_name_or_path="neuralmind/bert-base-portuguese-cased", # Nome do modelo de linguagem pré-treinado Transformer
         modelo_spacy="pt_core_news_lg", # Nome do modelo de linguagem da ferramenta de PLN
         do_lower_case=False,            # default True
         output_attentions=False,        # default False
         output_hidden_states=True,      # default False  /Retornar os embeddings das camadas ocultas  
-        camadas_embeddings = 2,         # 0-Primeira/1-Penúltima/2-Ùltima/3-Soma 4 últimas/4-Concat 4 últiamas/5-Todas
+        camadas_embeddings=2,           # 0-Primeira/1-Penúltima/2-Ùltima/3-Soma 4 últimas/4-Concat 4 últiamas/5-Todas
         estrategia_pooling=0,           # 0 - MEAN estratégia média / 1 - MAX  estratégia maior
         palavra_relevante=0             # 0 - Considera todas as palavras das sentenças / 1 - Desconsidera as stopwords / 2 - Considera somente as palavras substantivas
         )
 
 class TextoTransformer:
     
     ''' 
@@ -45,35 +46,35 @@
     `pretrained_model_name_or_path` - Se for um caminho de arquivo no disco, carrega o modelo a partir desse caminho. Se não for um caminho, ele primeiro faz o download do repositório de modelos do Huggingface com esse nome. Valor default: 'neuralmind/bert-base-portuguese-cased'.                  
     `modelo_spacy` - Nome do modelo a ser instalado e carregado pela ferramenta de pln spaCy. Valor default 'pt_core_news_lg'.                       
     `camadas_embeddings` - Especifica de qual camada ou camadas será recuperado os embeddings do transformer. Valor defaul '2'. Valores possíveis: 0-Primeira/1-Penúltima/2-Ùltima/3-Soma 4 últimas/4-Concat 4 últiamas/5-Todas.       
     `device` - Dispositivo (como 'cuda' / 'cpu') que deve ser usado para computação. Se none, verifica se uma GPU pode ser usada.
     ''' 
     
     # Construtor da classe
-    def __init__(self, pretrained_model_name_or_path="neuralmind/bert-base-portuguese-cased", 
-                       modelo_spacy="pt_core_news_lg",
+    def __init__(self, pretrained_model_name_or_path: str ="neuralmind/bert-base-portuguese-cased", 
+                       modelo_spacy: str ="pt_core_news_lg",
                        camadas_embeddings: int = 2,
-                       device=None):
+                       device = None):
                        
         # Parâmetro recebido para o modelo de linguagem
         modelo_argumentos.pretrained_model_name_or_path = pretrained_model_name_or_path
                
         # Parâmetro recebido para o modelo da ferramenta de pln
         modelo_argumentos.modelo_spacy = modelo_spacy
                 
         # Carrega o modelo de linguagem da classe transformador
         self.transformer = Transformer(modelo_args=modelo_argumentos)
     
-        # Recupera o modelo.
+        # Recupera o modelo de linguagem.
         self.model = self.transformer.get_auto_model()
     
         # Recupera o tokenizador.     
         self.tokenizer = self.transformer.get_tokenizer()
         
-        # Especifica de qual camada utilizar os embeddings        
+        # Especifica de qual camada utilizar os embeddings                
         logger.info("Utilizando embeddings do modelo da {} camada(s).".format(listaTipoCamadas[modelo_argumentos.camadas_embeddings][LISTATIPOCAMADA_NOME]))
                     
         # Especifica camadas para recuperar os embeddings
         modelo_argumentos.camadas_embeddings = camadas_embeddings
       
         # Carrega o spaCy
         self.pln = PLN(modelo_args=modelo_argumentos)
@@ -83,166 +84,209 @@
                                      transformer=self.transformer, 
                                      pln=self.pln)        
     
         # Verifica se é possível usar GPU
         if device is None:
             if torch.cuda.is_available():    
                 device = "cuda"
-                logging.info("Existem {} GPU(s) disponíveis.".format(torch.cuda.device_count()))
-                logging.info("Iremos usar a GPU: {}.".format(torch.cuda.get_device_name(0)))
+                logger.info("Existem {} GPU(s) disponíveis.".format(torch.cuda.device_count()))
+                logger.info("Iremos usar a GPU: {}.".format(torch.cuda.get_device_name(0)))
 
             else:                
                 device = "cpu"
-                logging.info("Sem GPU disponível, usando CPU.")
+                logger.info("Sem GPU disponível, usando CPU.")
             
-         # Diz ao PyTorch para usar o dispositvo (GPU ou CPU)
-        self._target_device = torch.device(device)
+            # Diz ao PyTorch para usar o dispositvo (GPU ou CPU)
+            self._target_device = torch.device(device)
+        else:
+            # Usa o device informado
+            self._target_device = torch.device(device)
 
+        # Mensagem de carregamento da classe
         logger.info("Classe TextoTransformer carregada: {}.".format(modelo_argumentos))
     
+    # ============================   
+    def __repr__(self):
+        '''
+        Retorna uma string com descrição do objeto
+        '''
+        return "Classe ({}) com modelo Transformer: {} e NLP: {} ".format(self.__class__.__name__, 
+                                                                          self.get_transformer().auto_model.__class__.__name__,
+                                                                          self.get_pln().model_pln.__class__.__name__)
+    
     # ============================
-    def _defineEstrategiaPooling(self, estrategiaPooling):
+    def _defineEstrategiaPooling(self, estrategia_pooling: Union[int, EstrategiasPooling] = EstrategiasPooling.MEAN):
         ''' 
         Define a estratégia de pooling para os parâmetros do modelo.
 
         Parâmetros:
-        `estrategiaPooling` - Um número de 0 a 1 com a estratégia de pooling das camadas do modelo contextualizado. Valor defaul '0'. Valores possíveis: 0 - MEAN estratégia média / 1 - MAX  estratégia maior.
+        `estrategia_pooling` - Um número de 0 a 1 com a estratégia de pooling das camadas do modelo contextualizado. Valor defaul '0'. Valores possíveis: 0 - MEAN estratégia média / 1 - MAX  estratégia maior.
         ''' 
         
-        if estrategiaPooling == EstrategiasPooling.MEAN.name:
+        # Verifica o tipo de dado do parâmetro 'estrategia_pooling'
+        if isinstance(estrategia_pooling, int):
+          if estrategia_pooling == 0:
+            estrategia_pooling = EstrategiasPooling.MEAN
+          else:
+            if estrategia_pooling == 1:
+              estrategia_pooling = EstrategiasPooling.MAX
+            else:
+              estrategia_pooling = None
+              logger.info("Não foi especificado um valor inteiro para a estratégia de pooling.") 
+        
+        # Atribui para os parâmetros do modelo
+        if estrategia_pooling == EstrategiasPooling.MEAN:
             modelo_argumentos.estrategia_pooling = EstrategiasPooling.MEAN.value
         else:
-            if estrategiaPooling == EstrategiasPooling.MAX.name:
+            if estrategia_pooling == EstrategiasPooling.MAX:
                 modelo_argumentos.estrategia_pooling = EstrategiasPooling.MAX.value            
             else:
                 logger.info("Não foi especificado uma estratégia de pooling válida.") 
     
     # ============================
-    def _definePalavraRelevante(self, palavraRelevante=0):
+    def _definePalavraRelevante(self, palavra_relevante: Union[int, PalavrasRelevantes] = PalavrasRelevantes.ALL):
         ''' 
         Define a estratégia de palavra relavante para os parâmetros do modelo.
         
         Parâmetros:        
-        `palavraRelevante` - Um número de 0 a 2 que indica a estratégia de relevância das palavras do texto. Valor defaul '0'. Valores possíveis: 0 - Considera todas as palavras das sentenças / 1 - Desconsidera as stopwords / 2 - Considera somente as palavras substantivas.
+        `palavra_relevante` - Um número de 0 a 2 que indica a estratégia de relevância das palavras do texto. Valor defaul '0'. Valores possíveis: 0 - Considera todas as palavras das sentenças / 1 - Desconsidera as stopwords / 2 - Considera somente as palavras substantivas.
         ''' 
         
-        if palavraRelevante == PalavrasRelevantes.CLEAN.name:
-            modelo_argumentos.palavra_relevante = PalavrasRelevantes.CLEAN.value
-            
+        # Verifica o tipo de dado do parâmetro 'palavra_relevante'
+        if isinstance(palavra_relevante, int):
+          if palavra_relevante == 0:
+            palavra_relevante = PalavrasRelevantes.ALL
+          else:
+            if palavra_relevante == 1:
+              palavra_relevante = PalavrasRelevantes.CLEAN
+            else:
+                if palavra_relevante == 2:
+                    palavra_relevante = PalavrasRelevantes.NOUN
+                else:
+                    palavra_relevante = None
+                    logger.info("Não foi especificado um valor inteiro para a estratégia de relevância de palavra.") 
+        
+        # Atribui para os parâmetros do modelo
+        if palavra_relevante == PalavrasRelevantes.ALL:
+            modelo_argumentos.palavra_relevante = PalavrasRelevantes.ALL.value            
         else:
-            if palavraRelevante == PalavrasRelevantes.NOUN.name:
-                modelo_argumentos.palavra_relevante = PalavrasRelevantes.NOUN.value
-                
+            if palavra_relevante == PalavrasRelevantes.CLEAN:
+                modelo_argumentos.palavra_relevante = PalavrasRelevantes.CLEAN.value                
             else:
-                if palavraRelevante == PalavrasRelevantes.ALL.name:
-                    modelo_argumentos.palavra_relevante = PalavrasRelevantes.ALL.value                    
+                if palavra_relevante == PalavrasRelevantes.NOUN:
+                    modelo_argumentos.palavra_relevante = PalavrasRelevantes.NOUN.value                    
                 else:
                     logger.info("Não foi especificado uma estratégia de relevância de palavras do texto válida.") 
 
     # ============================
-    def getMedidasTexto(self, texto, estrategiaPooling='MEAN', palavraRelevante='ALL'):
+    def getMedidasTexto(self, texto: str, 
+                        estrategia_pooling: EstrategiasPooling = EstrategiasPooling.MEAN, 
+                        palavra_relevante: PalavrasRelevantes = PalavrasRelevantes.ALL):
         ''' 
         Retorna as medidas de (in)coerência Ccos, Ceuc, Cman do texto.
         
         Parâmetros:
         `texto` - Um texto a ser medido.           
-        `estrategiaPooling` - Estratégia de pooling das camadas do BERT.
-        `palavraRelevante` - Estratégia de relevância das palavras do texto.            
+        `estrategia_pooling` - Estratégia de pooling das camadas do BERT.
+        `palavra_relevante` - Estratégia de relevância das palavras do texto.            
         
-        Retorno:
-        `Ccos` - Medida de coerência Ccos do do texto.            
-        `Ceuc` - Medida de incoerência Ceuc do do texto.            
-        `Cman` - Medida de incoerência Cman do do texto.            
+        Retorno um dicionário com:
+        `cos` - Medida de cos do do texto.
+        `euc` - Medida de euc do do texto.
+        `man` - Medida de man do do texto.
         ''' 
 
-        self._defineEstrategiaPooling(estrategiaPooling)
-        self._definePalavraRelevante(palavraRelevante)
+        self._defineEstrategiaPooling(estrategia_pooling)
+        self._definePalavraRelevante(palavra_relevante)
         
-        self.Ccos, self.Ceuc, self.Cman = self.mensurador.getMedidasComparacaoTexto(texto, 
-                                                                                    camada=modelo_argumentos.camadas_embeddings, 
-                                                                                    tipoTexto='o')
+        saida = self.mensurador.getMedidasComparacaoTexto(texto, 
+                                                          camada=modelo_argumentos.camadas_embeddings, 
+                                                          tipo_texto='o')
           
-        return self.Ccos, self.Ceuc, self.Cman
+        return saida
     
     # ============================
-    def getMedidasTextoCosseno(self, 
-                               texto, 
-                               estrategiaPooling='MEAN', 
-                               palavraRelevante='ALL'):
+    def getMedidasTextoCosseno(self, texto: str, 
+                               estrategia_pooling: EstrategiasPooling = EstrategiasPooling.MEAN, 
+                               palavra_relevante: PalavrasRelevantes = PalavrasRelevantes.ALL):
         ''' 
-        Retorna a medida de coerência do texto utilizando a medida de similaridade de cosseno.
+        Retorna a medida do texto utilizando a medida de similaridade de cosseno.
         
         Parâmetros:
         `texto` - Um texto a ser medido a coerência.           
-        `estrategiaPooling` - Estratégia de pooling das camadas do BERT. 
-        `palavraRelevante` - Estratégia de relevância das palavras do texto.            
+        `estrategia_pooling` - Estratégia de pooling das camadas do BERT. 
+        `palavra_relevante` - Estratégia de relevância das palavras do texto.            
         
         Retorno:
-        `Ccos` - Medida de coerência Ccos do do texto.            
+        `cos` - Medida de cos do do texto.            
         '''         
         
-        self._defineEstrategiaPooling(estrategiaPooling)
-        self._definePalavraRelevante(palavraRelevante)
+        self._defineEstrategiaPooling(estrategia_pooling)
+        self._definePalavraRelevante(palavra_relevante)
         
-        self.Ccos, self.Ceuc, self.Cman = self.mensurador.getMedidasComparacaoTexto(texto, 
-                                                                    camada=modelo_argumentos.camadas_embeddings, 
-                                                                    tipoTexto='o')
+        saida = self.mensurador.getMedidasComparacaoTexto(texto, 
+                                                          camada=modelo_argumentos.camadas_embeddings, 
+                                                          tipo_texto='o')
           
-        return self.Ccos
+        return saida['cos']
     
     # ============================
-    def getMedidasTextoEuclediana(self, texto, estrategiaPooling='MEAN', palavraRelevante='ALL'):
+    def getMedidasTextoEuclediana(self, texto: str, 
+                                  estrategia_pooling: EstrategiasPooling = EstrategiasPooling.MEAN, 
+                                  palavra_relevante: PalavrasRelevantes = PalavrasRelevantes.ALL):
         ''' 
-        Retorna a medida de incoerência do texto utilizando a medida de distância de Euclidiana.
+        Retorna a medida do texto utilizando a medida de distância de Euclidiana.
                  
         Parâmetros:
-        `texto` - Um texto a ser medido a coerência.           
-        `estrategiaPooling` - Estratégia de pooling das camadas do BERT.
-        `palavraRelevante` - Estratégia de relevância das palavras do texto.            
+        `texto` - Um texto a ser mensurado.           
+        `estrategia_pooling` - Estratégia de pooling das camadas do BERT.
+        `palavra_relevante` - Estratégia de relevância das palavras do texto.            
         
         Retorno:
-        `Ceuc` - Medida de incoerência Ceuc do do texto.            
+        `ceu` - Medida euc do texto.            
         ''' 
         
-        self._defineEstrategiaPooling(estrategiaPooling)
-        self._definePalavraRelevante(palavraRelevante)
+        self._defineEstrategiaPooling(estrategia_pooling)
+        self._definePalavraRelevante(palavra_relevante)
 
-        self.Ccos, self.Ceuc, self.Cman = self.mensurador.getMedidasComparacaoTexto(texto,
-                                                                    camada=modelo_argumentos.camadas_embeddings, 
-                                                                    tipoTexto='o')
+        saida = self.mensurador.getMedidasComparacaoTexto(texto,
+                                                          camada=modelo_argumentos.camadas_embeddings, 
+                                                          tipo_texto='o')
           
-        return self.Ceuc        
+        return saida['euc']      
        
     # ============================
-    def getMedidasTextoManhattan(self, texto, estrategiaPooling='MEAN', palavraRelevante='ALL'):
+    def getMedidasTextoManhattan(self, texto: str, 
+                                 estrategia_pooling: EstrategiasPooling = EstrategiasPooling.MEAN, 
+                                 palavra_relevante: PalavrasRelevantes = PalavrasRelevantes.ALL):
         ''' 
-        Retorna a medida de incoerência do texto utilizando a medida de distância de Manhattan.
+        Retorna a medida do texto utilizando a medida de distância de Manhattan.
                  
         Parâmetros:
-        `texto` - Um texto a ser medido a coerência.           
-        `estrategiaPooling` - Estratégia de pooling das camadas do BERT.
-        `palavraRelevante` - Estratégia de relevância das palavras do texto.            
+        `texto` - Um texto a ser mensurado.           
+        `estrategia_pooling` - Estratégia de pooling das camadas do BERT.
+        `palavra_relevante` - Estratégia de relevância das palavras do texto.            
         
         Retorno:
-        `Cman` - Medida de incoerência Cman do do texto.            
+        `man` - Medida  Cman do do texto.            
         ''' 
         
-        self._defineEstrategiaPooling(estrategiaPooling)
-        self._definePalavraRelevante(palavraRelevante)
+        self._defineEstrategiaPooling(estrategia_pooling)
+        self._definePalavraRelevante(palavra_relevante)
         
-        self.Ccos, self.Ceuc, self.Cman = self.mensurador.getMedidasComparacaoTexto(texto, 
-                                                                    camada=modelo_argumentos.camadas_embeddings, 
-                                                                    tipoTexto='o')
+        saida = self.mensurador.getMedidasComparacaoTexto(texto, 
+                                                          camada=modelo_argumentos.camadas_embeddings, 
+                                                          tipo_texto='o')
           
-        return self.Cman                
+        return saida['man']
     
     # ============================
-    def tokenize(self, texto):
+    def tokenize(self, texto: Union[str, List[str]]):
         '''
-        D Tokeniza um texto para submeter ao modelo de linguagem. 
+        Tokeniza um texto para submeter ao modelo de linguagem. 
         Retorna um dicionário listas de mesmo tamanho para garantir o processamento em lote.
         Use a quantidade de tokens para saber até onde deve ser recuperado em uma lista de saída.
         Ou use attention_mask diferente de 1 para saber que posições devem ser utilizadas na lista.
 
         Facilita acesso a classe Transformer.    
 
         :param texto: Texto a ser tokenizado para o modelo de linguagem.
@@ -252,190 +296,310 @@
             input_ids uma lista com os ids dos tokens de entrada mapeados em seus índices do vocabuário.
             token_type_ids uma lista com os tipos dos tokens.
             attention_mask uma lista com os as máscaras de atenção indicando com '1' os tokens  pertencentes à sentença.
         '''
         return self.get_transformer().tokenize(texto)
     
     # ============================
-    def getCodificacao(self, texto: Union[str, List[str]],
+    def getCodificacaoCompleta(self, texto: Union[str, List[str]],
                     tamanho_lote: int = 32, 
                     mostra_barra_progresso: bool = False,                     
-                    tipo_saida: str = 'texto_embedding',
-                    convert_to_numpy: bool = True,
-                    convert_to_tensor: bool = False,
-                    device: str = None,
-                    normalize_embeddings: bool = False):
+                    convert_to_numpy: bool = False,         
+                    device: str = None):
 
         '''
-        Calcula os embeddings de um texto utilizando o modelo de linguagem.
+        Retorna um dicionário com as informações completas da codificação do texto utilizando o modelo de linguagem.
     
         Parâmetros:
          `texto` - Um texto a ser recuperado os embeddings do modelo de linguagem
          `tamanho_lote` - o tamanho do lote usado para o computação
          `mostra_barra_progresso` - Mostra uma barra de progresso ao codificar o texto.
-         `tipo_saida` -  Especifica o tipo dos embeddings de saída. Pode ser definido como texto_embedding, sentenca_embedding, word_embedding, token_embeddings para obter embeddings de token do texto. Defina como none, para obter todos os valores de saída
-         `convert_to_numpy` - Se verdadeiro, a saída é uma lista de vetores numpy. Caso contrário, é uma lista de tensores pytorch.
-         `convert_to_tensor` - Se verdadeiro, você obtém um grande tensor como retorno. Substitui qualquer configuração de convert_to_numpy
+         `convert_to_numpy` - Se verdadeiro, a saída é uma lista de vetores numpy. Caso contrário, é uma lista de tensores pytorch.        
          `device` - Qual torch.device usar para o computação.
-         `normalize_embeddings` - Se definido como verdadeiro, os vetores retornados terão comprimento 1. Nesse caso, o produto escalar mais rápido (util.dot_score) em vez da similaridade de cosseno pode ser usado.
-        
     
-        :return::
-            Por padrão, uma lista de tensores é retornada. Se convert_to_tensor, um tensor empilhado é retornado. Se convert_to_numpy, uma matriz numpy é retornada.
+        Retorno um dicionário com:            
+            token_embeddings uma lista com os embeddings da última camada
+            input_ids uma lista com os textos indexados.            
+            attention_mask uma lista com os as máscaras de atenção
+            token_type_ids uma lista com os tipos dos tokens.            
+            tokens_texto_mcl uma lista com os textos tokenizados com os tokens especiais.
+            texto_original uma lista com os textos originais.
+            all_layer_embeddings uma lista com os embeddings de todas as camadas.
         '''
+        #Coloca o modelo e modo avaliação
+        self.model.eval()
+
+        entrada_eh_string = False
+        if isinstance(texto, str) or not hasattr(texto, '__len__'): 
+            #Colocar uma texto individual em uma lista com comprimento 1
+            texto = [texto]
+            entrada_eh_string = True
+
+        # Se não foi especificado um dispositivo, use-o defaul
+        if device is None:
+            device = self._target_device
+
+        # Adiciona um dispositivo ao modelo
+        self.model.to(device)
+
+        # Dicionário com a saída
+        saida = {}
+        saida.update({'token_embeddings': [],                        
+                      'input_ids': [],
+                      'attention_mask': [],
+                      'token_type_ids': [],        
+                      'tokens_texto_mcl': [],
+                      'texto_original': [],
+                      'all_layer_embeddings': []
+                      }
+                     )
+
+        # Percorre os lotes
+        for start_index in trange(0, 
+                                  len(texto), 
+                                  tamanho_lote, 
+                                  desc="Lotes", 
+                                  disable=not mostra_barra_progresso):
+            
+            # Recupera um lote
+            lote_textos = texto[start_index:start_index+tamanho_lote]
+
+            # Tokeniza o lote usando o modelo
+            lote_textos_tokenizados = self.get_transformer().tokenize(lote_textos)
+
+            # Adiciona ao device gpu ou cpu
+            lote_textos_tokenizados = self.get_transformer().batch_to_device(lote_textos_tokenizados, device)
+            
+            # Recupera os embeddings do modelo
+            with torch.no_grad():
 
-        if convert_to_tensor:
-            convert_to_numpy = False
+                # Recupera a saída da rede
+                output_rede = self.get_transformer().getSaidaRede(lote_textos_tokenizados)
 
-        if tipo_saida != 'texto_embedding':
-            convert_to_tensor = False
-            convert_to_numpy = False
+                # Lista para os embeddings do texto
+                embeddings = []
+
+                # Percorre todas as saídas(textos) do lote
+                #for token_embeddings, attention_mask in zip(output_rede['token_embeddings'], output_rede['attention_mask']):                    
+                for token_embeddings, input_ids, attention_mask,token_type_ids, tokens_texto_mcl,texto_original,all_layer_embeddings in zip(output_rede['token_embeddings'], 
+                                              output_rede['input_ids'],
+                                              output_rede['attention_mask'],
+                                              output_rede['token_type_ids'],
+                                              output_rede['tokens_texto_mcl'],
+                                              output_rede['texto_original'],
+                                              output_rede['all_layer_embeddings']):
+
+                    ultimo_mask_id = len(attention_mask)-1
+                    
+                    # Localiza o último token de "attention_mask" igual a 1
+                    while ultimo_mask_id > 0 and attention_mask[ultimo_mask_id].item() == 0:                        
+                      ultimo_mask_id -= 1                        
+                    
+                    # Recupera os embeddings do primeiro(0) até o último token que "attention_mask" seja 1                        
+
+                    # Concatena a lista dos embeddings do texto a lista já existente
+                    saida['token_embeddings'].append(token_embeddings[0:ultimo_mask_id+1])
+                    saida['input_ids'].append(input_ids[0:ultimo_mask_id+1])
+                    saida['attention_mask'].append(attention_mask[0:ultimo_mask_id+1])                    
+                    saida['token_type_ids'].append(token_type_ids[0:ultimo_mask_id+1])
+                    saida['tokens_texto_mcl'].append(tokens_texto_mcl[0:ultimo_mask_id+1])
+                    saida['texto_original'].append(texto_original)
+                    saida['all_layer_embeddings'].append(all_layer_embeddings[0:ultimo_mask_id+1])
+        
+        if convert_to_numpy:
+          saida['token_embeddings'] = np.array([emb.numpy() for emb in saida['token_embeddings']],dtype=object)
+
+        # Se é uma string remove a lista de lista
+        if entrada_eh_string:
+            saida['token_embeddings'] = saida['token_embeddings'][0]
+            saida['input_ids'] = saida['input_ids'][0]
+            saida['attention_mask'] = saida['attention_mask'][0]
+            saida['token_type_ids'] = saida['token_type_ids'][0]
+            saida['tokens_texto_mcl'] = saida['tokens_texto_mcl'][0]
+            saida['texto_original'] = saida['texto_original'][0]
+            saida['all_layer_embeddings'] = saida['all_layer_embeddings'][0]
+
+        return saida
+
+    # ============================
+    def getCodificacao(self, texto: Union[str, List[str]],
+                       tamanho_lote: int = 32,
+                       mostra_barra_progresso: bool = False,
+                       convert_to_numpy: bool = False,
+                       device: str = None):
+
+        '''
+        Retorna os embeddings da codificação de um texto utilizando o modelo de linguagem.
+    
+        Parâmetros:
+         `texto` - Um texto a ser recuperado os embeddings do modelo de linguagem
+         `tamanho_lote` - o tamanho do lote usado para o computação
+         `mostra_barra_progresso` - Mostra uma barra de progresso ao codificar o texto.
+         `convert_to_numpy` - Se verdadeiro, a saída é uma lista de vetores numpy. Caso contrário, é uma lista de tensores pytorch.        
+         `device` - Qual torch.device usar para o computação.
+    
+        Retorno:
+         Uma lista de tensores é com os embeddings do texto. Se convert_to_numpy, uma matriz numpy é retornada.
+        '''
+        #Coloca o modelo e modo avaliação
+        self.model.eval()
 
         entrada_eh_string = False
         if isinstance(texto, str) or not hasattr(texto, '__len__'): 
             #Colocar uma texto individual em uma lista com comprimento 1
             texto = [texto]
             entrada_eh_string = True
 
+        # Se não foi especificado um dispositivo, use-o defaul
         if device is None:
             device = self._target_device
 
-        self.to(device)
+        # Adiciona um dispositivo ao modelo
+        self.model.to(device)
 
         # Lista com embeddings de saída
         all_embeddings = []
+
         # Ordena o texto pelo comprimento decrescente
-        length_sorted_idx = np.argsort([-self._text_length(sen) for sen in texto])
+        indice_tamanho_ordenado = np.argsort([-self._tamanho_texto(sen) for sen in texto])        
         # Ordena o texto pelo comprimento decrescente
-        textos_ordenados = [texto[idx] for idx in length_sorted_idx]
-
+        textos_ordenados = [texto[idx] for idx in indice_tamanho_ordenado]
+        
+        # Percorre os lotes
         for start_index in trange(0, 
                                   len(texto), 
                                   tamanho_lote, 
                                   desc="Lotes", 
                                   disable=not mostra_barra_progresso):
             # Recupera um lote
             lote_textos = textos_ordenados[start_index:start_index+tamanho_lote]
 
             # Tokeniza o lote
-            features = self.get_transformer().tokenize(lote_textos)
-            features = self.get_transformer().batch_to_device(features, device)
-
+            lote_textos_tokenizados = self.get_transformer().tokenize(lote_textos)
+            # Adiciona ao device gpu ou cpu
+            lote_textos_tokenizados = self.get_transformer().batch_to_device(lote_textos_tokenizados, device)
+            
             # Recupera os embeddings do modelo
             with torch.no_grad():
-                out_features = self.get_transformer().forward(features)
-
-                # Retorno embeddings de tokens
-                if tipo_saida == 'token_embeddings':
-                    embeddings = []
-                    for token_emb, attention in zip(out_features[tipo_saida], out_features['attention_mask']):
-                        last_mask_id = len(attention)-1
-                        while last_mask_id > 0 and attention[last_mask_id].item() == 0:
-                            last_mask_id -= 1
-
-                        embeddings.append(token_emb[0:last_mask_id+1])
-                else:
-                    # Retorna toda a saída
-                    if tipo_saida is None: 
-                        embeddings = []
-                        for sent_idx in range(len(out_features['sentence_embedding'])):
-                            row =  {name: out_features[name][sent_idx] for name in out_features}
-                            embeddings.append(row)
-                    else:   
-                        #Retorna Texto embeddings
-                        embeddings = out_features[tipo_saida]
-                        embeddings = embeddings.detach()
-                        if normalize_embeddings:
-                            embeddings = torch.nn.functional.normalize(embeddings, p=2, dim=1)
 
-                        if convert_to_numpy:
-                            embeddings = embeddings.cpu()
+                # Recupera a saída da rede
+                output_rede = self.get_transformer().getSaidaRede(lote_textos_tokenizados)
 
+                embeddings = []
+                # Percorre todas as saídas(textos) do lote
+                for token_emb, attention in zip(output_rede['token_embeddings'], output_rede['attention_mask']):                    
+                    ultimo_mask_id = len(attention)-1
+                    
+                    # Localiza o último token de "attention_mask" igual a 1
+                    while ultimo_mask_id > 0 and attention[ultimo_mask_id].item() == 0:                        
+                      ultimo_mask_id -= 1                        
+                    
+                    # Adiciona os embeddings do primeiro(0) até o último token que "attention_mask" seja 1                        
+                    embeddings.append(token_emb[0:ultimo_mask_id+1])
+                                   
+                # Concatena a nova lista a lista já existente
                 all_embeddings.extend(embeddings)
+        
+        # Reorganiza a lista
+        all_embeddings = [all_embeddings[idx] for idx in np.argsort(indice_tamanho_ordenado)]
 
-        all_embeddings = [all_embeddings[idx] for idx in np.argsort(length_sorted_idx)]
-
-        if convert_to_tensor:
-            all_embeddings = torch.stack(all_embeddings)
-        else:
-            if convert_to_numpy:
-                all_embeddings = np.asarray([emb.numpy() for emb in all_embeddings])
+        if convert_to_numpy:
+          all_embeddings = np.array([emb.numpy() for emb in all_embeddings],dtype=object)
 
+        # Se é uma string remove a lista de lista
         if entrada_eh_string:
-            all_embeddings = all_embeddings[0]
+          all_embeddings = all_embeddings[0]
 
         return all_embeddings
 
     # ============================
-    def getEmbeddings(self, texto):
+    def getSaidaRede(self, texto: Union[str, dict]):
         '''
         De um texto preparado(tokenizado) ou não, retorna token_embeddings, input_ids, attention_mask, token_type_ids, 
         tokens_texto, texto_original  e all_layer_embeddings em um dicionário.
         
-        Facilita acesso ao método "getEmbeddings" da classe Transformer.
+        Facilita acesso ao método "getSaidaRede" da classe Transformer.
     
         Parâmetros:
         `texto` - Um texto a ser recuperado os embeddings do modelo de linguagem
     
         Retorna um dicionário com:            
             token_embeddings uma lista com os embeddings da última camada
             input_ids uma lista com os textos indexados.            
             attention_mask uma lista com os as máscaras de atenção
             token_type_ids uma lista com os tipos dos tokens.            
             tokens_texto uma lista com os textos tokenizados com os tokens especiais.
             texto_original uma lista com os textos originais.
             all_layer_embeddings uma lista com os embeddings de todas as camadas.
         '''
-        return self.get_transformer().getEmbeddings(texto)
+        return self.get_transformer().getSaidaRede(texto)
 
-    # ============================
-    def getEmbeddingsTextosMEAN(self, texto):
+   # ============================
+    def getEmbeddingTexto(self, texto: Union[str, List[str]], 
+                          estrategia_pooling: Union[int, EstrategiasPooling] = EstrategiasPooling.MEAN):
         '''
-        De um texto preparado(tokenizado) ou não, retorna os embeddings dos textos consolidados dos tokens do texto utilizando estratégia pooling MEAN.
+        Recebe um texto (string ou uma lista de strings) e retorna os embeddings consolidados dos tokens do texto utilizando estratégia pooling especificada(MEAN, MAX).
             
         Parâmetros:
-        `texto` - Um texto a ser recuperado os embeddings dos textos consolidados dos tokens com a estratégia MEAN utilizando o modelo de linguagem.
+        `texto` - Um texto é uma string ou uma lista de strings.
+        `estrategia_pooling` - Valor default MEAN. Uma estratégia de pooling,(EstrategiasPooling.MEAN, EstrategiasPooling.MAX). Pode ser utilizado os valores inteiros 0 para MEAN e 1 para MAX.
     
-        Retorna uma lista com os embeddings dos textos consolidados dos tokens com a estratégia MEAN.
+        Retorno: 
+        Os embeddings consolidados do texto se o parâmetro texto é uma string, caso contrário uma lista com os embeddings consolidados se o parâmetro é lista de string.
         '''
 
-        return self.getCodificacaoTextos(texto)['texto_embeddings_MEAN']
-    
-    # ============================
-    def getEmbeddingsTextosMAX(self, texto):
-        '''
-        De um texto preparado(tokenizado) ou não, retorna os embeddings dos textos consolidados dos tokens do texto utilizando estratégia pooling MAX.
-            
-        Parâmetros:
-        `texto` - Um texto a ser recuperado os embeddings dos textos consolidados dos tokens com a estratégia MAX utilizando o modelo de linguagem.
-    
-        Retorna uma lista com os embeddings dos textos consolidados dos tokens com a estratégia MAX.
-        '''
+        # Verifica o tipo da estratégia de pooling
+        if isinstance(estrategia_pooling, int):
+          if estrategia_pooling == 0:
+            estrategia_pooling = EstrategiasPooling.MEAN
+          else:
+            if estrategia_pooling == 1:
+              estrategia_pooling = EstrategiasPooling.MAX
+            else:
+              estrategia_pooling = None
+              logger.info("Não foi especificado um valor inteiro para a estratégia de pooling.") 
 
-        return self.getCodificacaoTextos(texto)['texto_embeddings_MAx']    
+        # Retorna os embeddings de acordo com a estratégia
+        if estrategia_pooling == EstrategiasPooling.MEAN:
+            return self.getCodificacaoTexto(texto)['texto_embeddings_MEAN']
+        else:
+            if estrategia_pooling == EstrategiasPooling.MAX:
+                return self.getCodificacaoTexto(texto)['texto_embeddings_MAX']
+            else:              
+                logger.info("Não foi especificado uma estratégia de pooling válida.") 
+                return None  
 
     # ============================
-    def getCodificacaoTextos(self, texto):
+    def getCodificacaoTexto(self, texto: Union[str, List[str]],
+                             tamanho_lote: int = 32, 
+                             mostra_barra_progresso: bool = False,                     
+                             convert_to_numpy: bool = False,         
+                             device: str = None):
         '''        
         De um texto preparado(tokenizado) ou não, retorna a codificação dos textos consolidados dos tokens do textos utilizando estratégia pooling MEAN e MAX.
     
         Parâmetros:
         `texto` - Um texto a ser recuperado os embeddings dos textos consolidados dos tokens com a estratégia MEAN e MAX utilizando o modelo de linguagem
     
-        Retorna uma lista com os embeddings consolidados dos textos utilizando embeddings da última camada do transformer.
+        Retorno:
+        Uma lista com os embeddings consolidados dos textos utilizando embeddings da última camada do transformer.
         '''
 
         # Se o texto é uma string, coloca em uma lista de comprimento 1
         entrada_eh_string = False
         if isinstance(texto, str) or not hasattr(texto, '__len__'):             
             texto = [texto]
             entrada_eh_string = True
 
         # Recupera os embeddings do texto
-        texto_embeddings = self.getEmbeddings(texto)
+        texto_embeddings = self.getCodificacaoCompleta(texto,
+                                                       tamanho_lote,
+                                                       mostra_barra_progresso,
+                                                       convert_to_numpy,
+                                                       device)
 
         # Acumula a saída do método
         saida = {}
         saida.update({'texto_original' : [],            # Lista com os textos originais
                       'tokens_texto_mcl' : [],          # Lista com os tokens dos textos originais
                       'texto_embeddings_MEAN': [],      # Lista de lista média dos embeddings dos tokens que da sentença.
                       'texto_embeddings_MAX': [],       # Lista de lista máximo dos embeddings dos tokens que da sentença.
@@ -470,82 +634,102 @@
                 saida['tokens_texto_mcl'].append(tokens_texto_mcl)
                 saida['texto_embeddings_MEAN'].append(embedding_documento_media)
                 saida['texto_embeddings_MAX'].append(embedding_documento_maximo)
 
         return saida
     
     # ============================
-    def getEmbeddingsSentencasMEAN(self, texto):    
+    def getEmbeddingSentenca(self, texto: Union[str, List[str]], 
+                             estrategia_pooling: Union[int, EstrategiasPooling] = EstrategiasPooling.MEAN):
         '''
-        De um texto preparado(tokenizado) ou não, retorna os embeddings das sentenças consolidados dos tokens do texto utilizando estratégia pooling MEAN.
+        Recebe um texto (string ou uma lista de strings) e retorna os embeddings consolidados dos tokens das sentenças do texto utilizando estratégia pooling especificada(MEAN, MAX).          
+        O texto ou a lista de textos é sentenciado utilizando a ferramenta de PLN. 
+        Os embeddings dos tokens gerados pelo modelo de linguagem serão consolidados em sentenças geradas pela sentenciação da ferramenta de pln.
             
         Parâmetros:
-        `texto` - Um texto a ser recuperado os embeddings das sentenças consolidados dos tokens com a estratégia MEAN utilizando o modelo de linguagem.
+        `texto` - Um texto é uma string ou uma lista de strings.
+        `estrategia_pooling` - Valor default MEAN. Uma estratégia de pooling,(EstrategiasPooling.MEAN, EstrategiasPooling.MAX). Pode ser utilizado os valores inteiros 0 para MEAN e 1 para MAX.
     
-        Retorna uma lista com os embeddings das sentenças consolidados dos tokens com a estratégia MEAN.
+        Retorno: 
+        Uma lista com os embeddings consolidados das sentenças se o parâmetro texto é uma string, caso contrário uma lista com a lista dos embeddings consolidados das sentenças se o parâmetro é lista de string.
         '''
 
-        return self.getCodificacaoSentencas(texto)['sentenca_embeddings_MEAN']
-
-    # ============================
-    def getEmbeddingsSentencasMAX(self, texto):    
-        '''
-        De um texto preparado(tokenizado) ou não, retorna os embeddings das sentenças consolidados dos tokens do texto utilizando estratégia pooling MAX.
-            
-        Parâmetros:
-        `texto` - Um texto a ser recuperado os embeddings das sentenças consolidados dos tokens com a estratégia MAX utilizando o modelo de linguagem.
-    
-        Retorna uma lista com os embeddings das sentenças consolidados dos tokens com a estratégia MAX.
-        '''
+        # Verifica o tipo da estratégia de pooling
+        if isinstance(estrategia_pooling, int):
+          if estrategia_pooling == 0:
+            estrategia_pooling = EstrategiasPooling.MEAN
+          else:
+            if estrategia_pooling == 1:
+              estrategia_pooling = EstrategiasPooling.MAX
+            else:
+              estrategia_pooling = None
+              logger.info("Não foi especificado um valor inteiro para a estratégia de pooling.") 
 
-        return self.getCodificacaoSentencas(texto)['sentenca_embeddings_MAX']
+        # Retorna os embeddings de acordo com a estratégia
+        if estrategia_pooling == EstrategiasPooling.MEAN:
+            return self.getCodificacaoSentenca(texto)['sentenca_embeddings_MEAN']
+        else:
+            if estrategia_pooling == EstrategiasPooling.MAX:
+                return self.getCodificacaoSentenca(texto)['sentenca_embeddings_MAX']
+            else:              
+                logger.info("Não foi especificado uma estratégia de pooling válida.") 
+                return None
 
-    # ============================
-    def getCodificacaoSentencas(self, texto):    
+    # ============================    
+    def getCodificacaoSentenca(self, texto: Union[str, List[str]],
+                               tamanho_lote: int = 32, 
+                               mostra_barra_progresso: bool = False,                     
+                               convert_to_numpy: bool = False,         
+                               device: str = None):      
         '''        
         De um texto preparado(tokenizado) ou não, retorna a codificação das sentenças consolidados dos tokens do textos utilizando estratégia pooling MEAN e MAX.
     
         Parâmetros:
         `texto` - Um texto a ser recuperado os embeddings das sentenças consolidados dos tokens com a estratégia MEAN e MAX utilizando o modelo de linguagem
     
-        Retorna uma lista com os embeddings consolidados das sentenças utilizando embeddings da última camada do transformer.
+        Retorno:
+        Uma lista com os embeddings consolidados das sentenças utilizando embeddings da última camada do transformer.
         '''
 
         # Se o texto é uma string, coloca em uma lista de comprimento 1
         entrada_eh_string = False
         if isinstance(texto, str) or not hasattr(texto, '__len__'):             
             texto = [texto]
             entrada_eh_string = True
-
+        
         # Recupera os embeddings do texto
-        texto_embeddings = self.getEmbeddings(texto)
+        texto_embeddings = self.getCodificacaoCompleta(texto,
+                                               tamanho_lote,
+                                               mostra_barra_progresso,
+                                               convert_to_numpy,
+                                               device)
 
         # Acumula a saída do método
         saida = {}
         saida.update({'texto_original' : [],            # Lista com os textos originais
                       'tokens_texto_mcl' : [],          # Lista com os tokens dos textos originais
                       'sentencas_texto' : [],           # Lista com as sentenças do texto
                       'sentenca_embeddings_MEAN': [],      # Lista de lista média dos embeddings dos tokens que da sentença.
                       'sentenca_embeddings_MAX': [],       # Lista de lista máximo dos embeddings dos tokens que da sentença.
-                      #'all_layer_embeddings': []
                      }
         )
 
         # Percorre os textos da lista.
         for i, texto in enumerate(texto_embeddings['texto_original']):       
 
             # Recupera os embeddings do texto  
             embeddings_texto = texto_embeddings['token_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]            
-           
+
             # Recupera a lista de tokens do tokenizado pelo MCL sem CLS e SEP
             tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]            
-            
+                        
             # Recupera as sentenças do texto
             lista_sentencas_texto = self.get_pln().getListaSentencasTexto(texto_embeddings['texto_original'][i])
-                 
+
+            # Lista de embeddings das sentenças do texto    
             lista_embeddings_tokens_sentencas_texto_media = []
             lista_embeddings_tokens_sentencas_texto_maximo = []
             
             # Percorre as sentenças do texto
             for j, sentenca in enumerate(lista_sentencas_texto):
 
                 # Tokeniza a sentença
@@ -567,66 +751,74 @@
 
                 # Calcula a média dos embeddings dos tokens das sentenças do texto
                 embedding_sentenca_maximo, linha = torch.max(embedding_sentenca, dim=0)
 
                 # Guarda os tokens e os embeddings das sentenças do texto da média e do máximo
                 lista_embeddings_tokens_sentencas_texto_media.append(embedding_sentenca_media)
                 lista_embeddings_tokens_sentencas_texto_maximo.append(embedding_sentenca_maximo)
-
             
-            #Acumula a saída do método 
-            #Se é uma string uma lista com comprimento 1
-            if entrada_eh_string:
-                saida['texto_original'] = texto_embeddings['texto_original'][i]
-                saida['tokens_texto_mcl'] =  tokens_texto_mcl
-                saida['sentencas_texto'] = lista_sentencas_texto
-                saida['sentenca_embeddings_MEAN'] = lista_embeddings_tokens_sentencas_texto_media
-                saida['sentenca_embeddings_MAX'] = lista_embeddings_tokens_sentencas_texto_maximo
-            else:
-                saida['texto_original'].append(texto_embeddings['texto_original'][i])
-                saida['tokens_texto_mcl'].append(tokens_texto_mcl)
-                saida['sentencas_texto'].append(lista_sentencas_texto)
-                saida['sentenca_embeddings_MEAN'].append(lista_embeddings_tokens_sentencas_texto_media)
-                saida['sentenca_embeddings_MAX'].append(lista_embeddings_tokens_sentencas_texto_maximo)
+            #Acumula a saída do método             
+            saida['texto_original'].append(texto_embeddings['texto_original'][i])
+            saida['tokens_texto_mcl'].append(tokens_texto_mcl)
+            saida['sentencas_texto'].append(lista_sentencas_texto)
+            saida['sentenca_embeddings_MEAN'].append(lista_embeddings_tokens_sentencas_texto_media)
+            saida['sentenca_embeddings_MAX'].append(lista_embeddings_tokens_sentencas_texto_maximo)
+
+        #Se é uma string uma lista com comprimento 1
+        if entrada_eh_string:
+          saida['texto_original'] = saida['texto_original'][0]
+          saida['tokens_texto_mcl'] =  saida['tokens_texto_mcl'][0]
+          saida['sentencas_texto'] = saida['sentencas_texto'][0]
+          saida['sentenca_embeddings_MEAN'] = saida['sentenca_embeddings_MEAN'][0]
+          saida['sentenca_embeddings_MAX'] = saida['sentenca_embeddings_MAX'][0]
 
         return saida
    
     # ============================
-    def getEmbeddingsPalavrasMEAN(self, 
-                                  texto):
+    def getEmbeddingPalavra(self, texto: Union[str, List[str]], 
+                             estrategia_pooling: Union[int, EstrategiasPooling] = EstrategiasPooling.MEAN):
         '''
-        De um texto preparado(tokenizado) ou não, retorna os embeddings das palavras consolidados dos tokens do texto utilizando estratégia pooling MEAN.
+        Recebe um texto (string ou uma lista de strings) e retorna os embeddings consolidados dos tokens das palavras do texto utilizando estratégia pooling especificada(MEAN, MAX).          
+        O texto ou a lista de textos será tokenizado utilizando a ferramenta de PLN. 
+        Os embeddings dos tokens gerados pelo modelo de linguagem serão consolidados em palavras geradas pela tokenização da ferramenta de pln.
             
         Parâmetros:
-        `texto` - Um texto a ser recuperado os embeddings das palavras consolidados dos tokens com a estratégia MEAN utilizando o modelo de linguagem.
+        `texto` - Um texto é uma string ou uma lista de strings.
+        `estrategia_pooling` - Valor default MEAN. Uma estratégia de pooling,(EstrategiasPooling.MEAN, EstrategiasPooling.MAX). Pode ser utilizado os valores inteiros 0 para MEAN e 1 para MAX.
     
-        Retorna uma lista com os embeddings das palavras consolidados dos tokens com a estratégia MEAN.
+        Retorno: Uma lista com os embeddings consolidados das palavras se o parâmetro texto é uma string, caso contrário uma lista com a lista dos embeddings consolidados das palavras se o parâmetro é lista de string.
         '''
-        saida = self.getCodificacaoPalavras(texto)['embeddings_MEAN']
-        
-        return saida
 
-    # ============================
-    def getEmbeddingsPalavrasMAX(self, 
-                                  texto):
-        '''
-        De um texto preparado(tokenizado) ou não, retorna os embeddings das palavras consolidados dos tokens do texto utilizando estratégia pooling MAX.
-            
-        Parâmetros:
-        `texto` - Um texto a ser recuperado os embeddings das palavras consolidados dos tokens com a estratégia MAX utilizando o modelo de linguagem.
-    
-        Retorna uma lista com os embeddings das palavras consolidados dos tokens com a estratégia MAX.
-        '''
-        saida = self.getCodificacaoPalavras(texto)['embeddings_MAX']
-        
-        return saida
+        # Verifica o tipo da estratégia de pooling
+        if isinstance(estrategia_pooling, int):
+          if estrategia_pooling == 0:
+            estrategia_pooling = EstrategiasPooling.MEAN
+          else:
+            if estrategia_pooling == 1:
+              estrategia_pooling = EstrategiasPooling.MAX
+            else:
+              estrategia_pooling = None
+              logger.info("Não foi especificado um valor inteiro para a estratégia de pooling.") 
+
+        # Retorna os embeddings de acordo com a estratégia
+        if estrategia_pooling == EstrategiasPooling.MEAN:
+            return self.getCodificacaoPalavra(texto)['embeddings_MEAN']
+        else:
+            if estrategia_pooling == EstrategiasPooling.MAX:
+                return self.getCodificacaoPalavra(texto)['embeddings_MAX']
+            else:              
+                logger.info("Não foi especificado uma estratégia de pooling válida.") 
+                return None
             
     # ============================
-    def getCodificacaoPalavras(self, 
-                               texto):
+    def getCodificacaoPalavra(self, texto: Union[str, List[str]],
+                              tamanho_lote: int = 32, 
+                              mostra_barra_progresso: bool = False,
+                              convert_to_numpy: bool = False,
+                              device: str = None):      
         
         '''
         De um texto preparado(tokenizado) ou não, retorna os embeddings das palavras do texto. 
         Retorna um dicionário 5 listas, os tokens(palavras), as postagging, tokens OOV, e os embeddings dos tokens igualando a quantidade de tokens do spaCy com a tokenização do MCL de acordo com a estratégia. 
         Utiliza duas estratégias para realizar o pooling de tokens que forma uma palavra.
             - Estratégia MEAN para calcular a média dos embeddings dos tokens que formam uma palavra.
             - Estratégia MAX para calcular o valor máximo dos embeddings dos tokens que formam uma palavra.
@@ -646,85 +838,97 @@
         
         # Se o texto é uma string, coloca em uma lista de comprimento 1
         entrada_eh_string = False
         if isinstance(texto, str) or not hasattr(texto, '__len__'):             
             texto = [texto]
             entrada_eh_string = True
 
-        # Tokeniza o texto
-        texto_embeddings = self.get_transformer().getEmbeddings(texto)
-
+        # Recupera os embeddings do texto
+        texto_embeddings = self.getCodificacaoCompleta(texto,
+                                               tamanho_lote,
+                                               mostra_barra_progresso,
+                                               convert_to_numpy,
+                                               device)
+        
         # Acumula a saída do método
         saida = {}
         saida.update({'texto_original' : [],
                       'tokens_texto': [], 
                       'tokens_texto_mcl' : [],
                       'tokens_oov_texto_mcl': [],                      
                       'tokens_texto_pln' : [],
                       'pos_texto_pln': [],
                       'embeddings_MEAN': [],        
                       'embeddings_MAX': []
                      }
         )
 
         # Percorre os textos da lista.
-        for i, sentenca in enumerate(texto_embeddings['tokens_texto_mcl']):
+        for i, texto in enumerate(texto_embeddings['texto_original']):
+            
             # Recupera o texto tokenizado pela ferramenta de pln do texto original
             lista_tokens_texto_pln = self.get_pln().getTokensTexto(texto_embeddings['texto_original'][i])
+            
             # Recupera os embeddings do texto  
             embeddings_texto = texto_embeddings['token_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]            
+            
             # Recupera a lista de tokens do tokenizado pelo MCL sem CLS e SEP
-            tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]            
+            tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]        
+            
             # Concatena os tokens gerandos pela ferramenta de pln
             tokens_texto_concatenado = " ".join(lista_tokens_texto_pln)
+
             # Recupera os embeddings e tokens de palavra            
-            lista_tokens_texto, lista_pos_texto_pln, lista_tokens_oov_texto_mcl, lista_embeddings_MEAN, lista_embeddings_MAX = self.get_transformer().getTokensEmbeddingsPOSTexto(
-                                                    embeddings_texto,
-                                                    tokens_texto_mcl,
-                                                    tokens_texto_concatenado,
-                                                    self.get_pln())
+            saidaEmbeddingPalavra = self.get_transformer().getTokensEmbeddingsPOSTexto(embeddings_texto,
+                                                                                       tokens_texto_mcl,
+                                                                                       tokens_texto_concatenado,
+                                                                                       self.get_pln())
 
             #Acumula a saída do método 
-            #Se é uma string uma lista com comprimento 1
-            if entrada_eh_string:
-                saida['texto_original'] = texto_embeddings['texto_original'][i]
-                saida['tokens_texto'] = lista_tokens_texto
-                saida['tokens_texto_mcl'] = tokens_texto_mcl
-                saida['tokens_oov_texto_mcl'] = lista_tokens_oov_texto_mcl
-                saida['tokens_texto_pln'] = lista_tokens_texto_pln
-                saida['pos_texto_pln'] = lista_pos_texto_pln
-                saida['embeddings_MEAN'] = lista_embeddings_MEAN
-                saida['embeddings_MAX'] = lista_embeddings_MAX
-            else:
-                saida['texto_original'].append(texto_embeddings['texto_original'][i])
-                saida['tokens_texto'].append(lista_tokens_texto)
-                saida['tokens_texto_mcl'].append(tokens_texto_mcl)
-                saida['tokens_oov_texto_mcl'].append(lista_tokens_oov_texto_mcl)            
-                saida['tokens_texto_pln'].append(lista_tokens_texto_pln)
-                saida['pos_texto_pln'].append(lista_pos_texto_pln)            
-                saida['embeddings_MEAN'].append(lista_embeddings_MEAN)
-                saida['embeddings_MAX'].append(lista_embeddings_MAX)
+            saida['texto_original'].append(texto_embeddings['texto_original'][i])
+            saida['tokens_texto'].append(saidaEmbeddingPalavra['tokens_texto'])
+            saida['tokens_texto_mcl'].append(tokens_texto_mcl)
+            saida['tokens_oov_texto_mcl'].append(saidaEmbeddingPalavra['tokens_oov_texto_mcl'])            
+            saida['tokens_texto_pln'].append(lista_tokens_texto_pln)
+            saida['pos_texto_pln'].append(saidaEmbeddingPalavra['pos_texto_pln'])            
+            saida['embeddings_MEAN'].append(saidaEmbeddingPalavra['embeddings_MEAN'])
+            saida['embeddings_MAX'].append(saidaEmbeddingPalavra['embeddings_MAX'])
+        
+        #Se é uma string uma lista com comprimento 1
+        if entrada_eh_string:
+            saida['texto_original'] = saida['texto_original'][0]
+            saida['tokens_texto'] = saida['tokens_texto'][0]
+            saida['tokens_texto_mcl'] = saida['tokens_texto_mcl'][0]
+            saida['tokens_oov_texto_mcl'] = saida['tokens_oov_texto_mcl'][0]
+            saida['tokens_texto_pln'] = saida['tokens_texto_pln'][0]
+            saida['pos_texto_pln'] = saida['pos_texto_pln'][0]
+            saida['embeddings_MEAN'] = saida['embeddings_MEAN'][0]
+            saida['embeddings_MAX'] = saida['embeddings_MAX'][0]
 
         return saida
     
-    def getEmbeddingsTokens(self, texto):
+    # ============================
+    def getEmbeddingToken(self, texto: Union[str, List[str]]):
         '''
-        De um texto preparado(tokenizado) ou não, retorna os embeddings dos tokens do texto.
-            
+        Recebe um texto (string ou uma lista de strings) e retorna os embeddings dos tokens gerados pelo tokenizador modelo de linguagem.                  
+                    
         Parâmetros:
-        `texto` - Um texto a ser recuperado os embeddings das palavras do modelo de linguagem.
+        `texto` - Um texto é uma string ou uma lista de strings.
     
-        Retorna uma lista com os embeddings dos tokens.
+        Retorno: Uma lista com os embeddings dos tokens se o parâmetro texto é uma string, caso contrário uma lista com a lista dos embeddings dos tokens se o parâmetro é lista de string.
         '''
-        saida = self.getCodificaoTokens(texto)['token_embeddings']
-        
-        return saida
 
-    # ============================
-    def getCodificaoTokens(self, texto):
+        return self.getCodificacaoToken(texto)['token_embeddings']
+
+    # ============================    
+    def getCodificacaoToken(self, texto: Union[str, List[str]],
+                            tamanho_lote: int = 32, 
+                            mostra_barra_progresso: bool = False,                     
+                            convert_to_numpy: bool = False,         
+                            device: str = None):
         '''        
         De um texto preparado(tokenizado) ou não, retorna os embeddings dos tokens do texto utilizando estratégia pooling MEAN.
     
         Parâmetros:
         `texto` - Um texto a ser recuperado os embeddings do modelo de linguagem
     
         Retorna uma lista com os embeddings da última camada.
@@ -733,52 +937,79 @@
         # Se o texto é uma string, coloca em uma lista de comprimento 1
         entrada_eh_string = False
         if isinstance(texto, str) or not hasattr(texto, '__len__'):             
             texto = [texto]
             entrada_eh_string = True
 
         # Recupera os embeddings do texto
-        texto_embeddings = self.getEmbeddings(texto)
-
+        #texto_embeddings = self.getEmbeddings(texto)
+          
+        texto_embeddings = self.getCodificacaoCompleta(texto,
+                                               tamanho_lote,
+                                               mostra_barra_progresso,
+                                               convert_to_numpy,
+                                               device)
+        
         # Acumula a saída do método
         saida = {}
         saida.update({'texto_original' : [],
                       'tokens_texto_mcl' : [],                      
-                      'pos_texto_pln': [],
                       'token_embeddings': [],        
-                      'all_layer_embeddings': []
+                      #'all_layer_embeddings': []
                      }
         )
 
         # Percorre os textos da lista.
-        for i, sentenca in enumerate(texto_embeddings['tokens_texto_mcl']):            
+        for i, texto in enumerate(texto_embeddings['texto_original']):            
             # Recupera os embeddings do texto  
             lista_token_embeddings = texto_embeddings['token_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]
 
             # Recupera os embeddings do texto  
-            lista_all_layer_embeddings = texto_embeddings['all_layer_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]
+            #lista_all_layer_embeddings = texto_embeddings['all_layer_embeddings'][i][0:len(texto_embeddings['tokens_texto_mcl'][i])]
             
             # Recupera a lista de tokens do tokenizado pelo MCL sem CLS e SEP
             tokens_texto_mcl = texto_embeddings['tokens_texto_mcl'][i][1:-1]
 
             #Acumula a saída do método 
             #Se é uma string uma lista com comprimento 1
             if entrada_eh_string:
                 saida['texto_original'] = texto_embeddings['texto_original'][i]
                 saida['tokens_texto_mcl'] = tokens_texto_mcl
                 saida['token_embeddings'] = lista_token_embeddings
-                saida['all_layer_embeddings'] = lista_all_layer_embeddings
             else:
                 saida['texto_original'].append(texto_embeddings['texto_original'][i])
                 saida['tokens_texto_mcl'].append(tokens_texto_mcl)
                 saida['token_embeddings'].append(lista_token_embeddings)
-                saida['all_layer_embeddings'].append(lista_all_layer_embeddings)
 
         return saida
 
+    # ============================    
+    def _tamanho_texto(self, texto: Union[List[int], List[List[int]]]):
+        '''                
+        Função de ajuda para obter o comprimento do texto de entrada. O texto pode ser 
+        uma lista de ints (o que significa um único texto como entrada) ou uma tupla de 
+        lista de ints (representando várias entradas de texto para o modelo).
+
+        Parâmetros:
+        `texto` - Um texto a ser recuperado o tamanho.
+
+        Retorno:
+          Um inteiro com tamanho do texto.
+        '''
+        if isinstance(texto, dict):              # caso seja um dic de listas
+            return len(next(iter(texto.values())))
+        else:
+            if not hasattr(texto, '__len__'):      # Objeto não tem o len()
+                return 1
+            else:
+                if len(texto) == 0 or isinstance(texto[0], int):  #String vazia ou lista de ints
+                    return len(texto)
+                else:
+                    return sum([len(t) for t in texto])      ##Soma do comprimento de strings individuais
+    
     # ============================
     def get_model(self):
         return self.model
 
     # ============================
     def get_tokenizer(self):
         return self.tokenizer
@@ -789,26 +1020,8 @@
 
     # ============================    
     def get_mensurador(self):
         return self.mensurador        
         
     # ============================        
     def get_pln(self):
-        return self.pln          
-
-
-  # ============================
-    def getEmbeddingsTexto(self, texto):
-        '''
-        De um texto preparado(tokenizado) ou não, retorna token_embeddings, input_ids, attention_mask, token_type_ids, 
-        tokens_texto, texto_original  e all_layer_embeddings em um dicionário.
-        
-        Facilita acesso a classe Transformer.
-    
-        Parâmetros:
-        `texto` - Um texto a ser recuperado os embeddings do modelo de linguagem
-    
-        Retorna:
-            token_embeddings uma lista com os embeddings da última camada.
-           
-        '''
-        return self.get_transformer().getEmbeddings(texto)['token_embeddings']
+        return self.pln
```

### Comparing `texto_transformer-0.0.1/textotransformer/mensurador/medidas.py` & `texto_transformer-0.0.2/textotransformer/mensurador/medidas.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.1/textotransformer/mensurador/mensurador.py` & `texto_transformer-0.0.2/textotransformer/mensurador/mensurador.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Import das bibliotecas.
 
 # Biblioteca de logging
-import logging 
+import logging
 
 # Biblioteca de aprendizado de máquina
 import torch 
 
 # Bibliotecas próprias
+from textotransformer.modelo.transformer import Transformer
+from textotransformer.modelo.modeloarguments import ModeloArgumentos 
+from textotransformer.pln.pln import PLN
 from textotransformer.mensurador.medidas import distanciaEuclidiana, distanciaManhattan, similaridadeCoseno
 from textotransformer.mensurador.mensuradorenum import PalavrasRelevantes
 from textotransformer.modelo.modeloenum import LISTATIPOCAMADA_NOME, EmbeddingsCamadas, EstrategiasPooling 
 from textotransformer.util.utilconstantes import OUTPUTS, OUTPUTS_HIDDEN_STATES
 from textotransformer.util.utiltexto import encontrarIndiceSubLista  
 
 logger = logging.getLogger(__name__)
@@ -23,97 +26,109 @@
     Parâmetros:
     `modelo_args` - Parâmetros do modelo de linguagem.
     `transformer` - Modelo de linguagem carregado.
     `pln` - Processador de linguagem natural.
     ''' 
 
     # Construtor da classe
-    def __init__(self, modelo_args, transformer, pln):
+    def __init__(self, modelo_args: ModeloArgumentos,
+                 transformer: Transformer, 
+                 pln: PLN):
     
         # Parâmetros do modelo
         self.model_args = modelo_args
     
         # Recupera o objeto do transformer.
         self.transformer = transformer
     
         # Recupera o modelo.
-        self.model = transformer.get_auto_model()
+        self.auto_model = transformer.get_auto_model()
     
         # Recupera o tokenizador.     
         self.tokenizer = transformer.get_tokenizer()
         
         # Recupera a classe PLN
         self.pln = pln
         
         logger.info("Classe Mensurador carregada: {}.".format(modelo_args))
-      
+
+    # ============================   
+    def __repr__(self):
+        '''
+        Retorna uma string com descrição do objeto
+        '''
+        return "Classe ({}) com modelo Transformer: {}, tokenizador: {} e NLP: {} ".format(self.__class__.__name__, 
+                                                                          self.auto_model.__class__.__name__,
+                                                                          self.tokenizer.__class__.__name__,
+                                                                          self.pln.__class__.__name__)
+
     # ============================
     def getEmbeddingsTodasCamadas(self, texto):    
         '''   
         Retorna os embeddings de todas as camadas de um texto.
         
         Parâmetros:
         `texto` - Um texto a ser recuperado os embeddings do BERT.
         
         Retorno:
-        `textoTokenizado` - Texto tokenizado.
+        `texto_tokenizado` - Texto tokenizado.
         `input_ids` - Input ids do texto.
         `attention_mask` - Máscara de atenção do texto
         `token_type_ids` - Token types ids do texto.
         `outputs` - Embeddings do texto.
         '''
 
         # Texto tokenizado
-        textoTokenizado =  self.transformer.getTextoTokenizado(texto)
+        texto_tokenizado =  self.transformer.getTextoTokenizado(texto)
 
-        #print('O texto (', texto, ') tem tamanho = ', len(textoTokenizado), ' = ', textoTokenizado)
+        #print('O texto (', texto, ') tem tamanho = ', len(texto_tokenizado), ' = ', texto_tokenizado)
 
         # Recupera a quantidade tokens do texto tokenizado.
-        qtdeTokens = len(textoTokenizado)
+        qtdeTokens = len(texto_tokenizado)
 
         #tokeniza o texto e retorna os tensores.
-        dicCodificado = self.tokenizer.encode_plus(
+        dic_codificado = self.tokenizer.encode_plus(
                                                 texto, # Texto a ser codificado.
                                                 add_special_tokens=True, # Adiciona os tokens especiais '[CLS]' e '[SEP]'
                                                 max_length=qtdeTokens, # Define o tamanho máximo para preencheer ou truncar.
                                                 truncation=True, # Trunca o texto por max_length
                                                 padding='max_length', # Preenche o texto até max_length
                                                 return_attention_mask=True, # Constrói a máscara de atenção.
                                                 return_tensors='pt' # Retorna os dados como tensores pytorch.
                                                 )
         
         # Ids dos tokens de entrada mapeados em seus índices do vocabuário.
-        input_ids = dicCodificado['input_ids']
+        input_ids = dic_codificado['input_ids']
 
         # Máscara de atenção de cada um dos tokens como pertencentes à sentença '1'.
-        attention_mask = dicCodificado['attention_mask']
+        attention_mask = dic_codificado['attention_mask']
 
         # Recupera os tensores dos segmentos.
-        token_type_ids = dicCodificado['token_type_ids']
+        token_type_ids = dic_codificado['token_type_ids']
 
         # Roda o texto através do BERT, e coleta todos os estados ocultos produzidos.
         # das 12 camadas. 
         with torch.no_grad():
 
             # Passe para a frente, calcule as previsões outputs.     
-            outputs = self.model(input_ids=input_ids, 
+            outputs = self.auto_model(input_ids=input_ids, 
                                  attention_mask=attention_mask)
 
             # A avaliação do modelo retorna um número de diferentes objetos com base em
             # como é configurado na chamada do método `from_pretrained` anterior. Nesse caso,
             # porque definimos `output_hidden_states = True`, o terceiro item será o
             # estados ocultos(hidden_states) de todas as camadas. Veja a documentação para mais detalhes:
             # https://huggingface.co/transformers/model_doc/bert.html#bertmodel
 
             # Retorno de model quando ´output_hidden_states=True´ é setado:    
             # outputs[0] = last_hidden_state, outputs[1] = pooler_output, outputs[2] = hidden_states
             # hidden_states é uma lista python, e cada elemento um tensor pytorch no formado <lote> x <qtde_tokens> x <768 ou 1024>.
             
             # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
-        return textoTokenizado, input_ids, attention_mask, token_type_ids, outputs
+        return texto_tokenizado, input_ids, attention_mask, token_type_ids, outputs
 
     # ============================
     # Cria um buffer com os embeddings de sentenças para economizar memória no processamento.
     buffer_embeddings = {}
     
     def getEmbeddingsTodasCamadasBuffer(self, S):
         '''
@@ -121,183 +136,183 @@
         '''
         
         # Se está no dicionário retorna o embedding
         if S in self.buffer_embeddings:
             return self.buffer_embeddings.get(S)
         else:
             # Gera o embedding
-            totalCamada = self.getEmbeddingsTodasCamadas(S)
-            self.buffer_embeddings.update({S: totalCamada})
-            return totalCamada
+            total_camada = self.getEmbeddingsTodasCamadas(S)
+            self.buffer_embeddings.update({S: total_camada})
+            return total_camada
 
     # ============================
     def limpaBufferEmbedding(self):
         '''
         Esvazia o buffer de embeddings das sentenças.
         '''
         
         self.buffer_embeddings.clear(self)
 
     # ============================
-    def getEmbeddingPrimeiraCamada(self, sentencaEmbedding):
+    def getEmbeddingPrimeiraCamada(self, sentenca_embedding):
         '''
         Retorna os embeddings da primeira camada.
         '''
         
-        # Cada elemento do vetor sentencaEmbeddinging é formado por:  
+        # Cada elemento do vetor sentenca_embedding é formado por:  
         # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
         # hidden_states é uma lista python, e cada elemento um tensor pytorch no formado <lote> x <qtde_tokens> x <768 ou 1024>.
         #[4]outpus e [2]hidden_states 
         #[OUTPUTS]outpus e [OUTPUTS_HIDDEN_STATES]hidden_states      
       
         # Retorna todas a primeira(-1) camada
         # Entrada: List das camadas(13 ou 25) (<1(lote)> x <qtde_tokens> x <768 ou 1024>)  
-        resultado = sentencaEmbedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][0]
+        resultado = sentenca_embedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][0]
         # Retorno: (<1(lote)> x <qtde_tokens> x <768 ou 1024>)  
         #print('resultado=',resultado.size())
 
         return resultado
 
     # ============================
-    def getEmbeddingPenultimaCamada(self, sentencaEmbedding):
+    def getEmbeddingPenultimaCamada(self, sentenca_embedding):
         '''
         Retorna os embeddings da penúltima camada.
         '''
         
         # Cada elemento do vetor sentencaEmbedding é formado por:  
         # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
         # hidden_states é uma lista python, e cada elemento um tensor pytorch no formado <lote> x <qtde_tokens> x <768 ou 1024>.
         #[4]outpus e [2]hidden_states 
         #[OUTPUTS]outpus e [OUTPUTS_HIDDEN_STATES]hidden_states      
       
         # Retorna todas a penúltima(-2) camada
         # Entrada: List das camadas(13 ou 25) (<1(lote)> x <qtde_tokens> x <768 ou 1024>)  
-        resultado = sentencaEmbedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][-2]
+        resultado = sentenca_embedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][-2]
         # Retorno: (<1(lote)> x <qtde_tokens> <768 ou 1024>)  
         #print('resultado=',resultado.size())
 
         return resultado
 
     # ============================
-    def getEmbeddingUltimaCamada(self, sentencaEmbedding):
+    def getEmbeddingUltimaCamada(self, sentenca_embedding):
         '''
         Retorna os embeddings da última camada.
         '''
         
         # Cada elemento do vetor sentencaEmbedding é formado por:  
         # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
         # hidden_states é uma lista python, e cada elemento um tensor pytorch no formado <lote> x <qtde_tokens> x <768 ou 1024>.
         #[4]outpus e [2]hidden_states 
         #[OUTPUTS]outpus e [OUTPUTS_HIDDEN_STATES]hidden_states      
       
         # Retorna todas a última(-1) camada
         # Entrada: List das camadas(13 ou 25) (<1(lote)> x <qtde_tokens> x <768 ou 1024>)  
-        resultado = sentencaEmbedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][-1]
+        resultado = sentenca_embedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][-1]
         # Retorno: (<1(lote)> x <qtde_tokens> <768 ou 1024>)  
         #print('resultado=',resultado.size())
       
         return resultado    
 
     # ============================
-    def getEmbeddingSoma4UltimasCamadas(self, sentencaEmbedding):
+    def getEmbeddingSoma4UltimasCamadas(self, sentenca_embedding):
         '''
         Retorna os embeddings da soma das 4 últimas camadas.
         '''
         
         # Cada elemento do vetor sentencaEmbedding é formado por:  
         # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
         # hidden_states é uma lista python, e cada elemento um tensor pytorch no formado <lote> x <qtde_tokens> x <768 ou 1024>.
         #[4]outpus e [2]hidden_states 
         #[OUTPUTS]outpus e [OUTPUTS_HIDDEN_STATES]hidden_states      
       
         # Retorna todas as 4 últimas camadas
         # Entrada: List das camadas(13 ou 25) (<1(lote)> x <qtde_tokens> <768 ou 1024>)  
-        embeddingCamadas = sentencaEmbedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][-4:]
+        embedding_camadas = sentenca_embedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][-4:]
         # Retorno: List das camadas(4) (<1(lote)> x <qtde_tokens> x <768 ou 1024>)  
 
         # Usa o método `stack` para criar uma nova dimensão no tensor 
         # com a concateção dos tensores dos embeddings.        
         # Entrada: List das camadas(4) (<1(lote)> x <qtde_tokens> <768 ou 1024>)  
-        resultadoStack = torch.stack(embeddingCamadas, dim=0)
+        resultado_stack = torch.stack(embedding_camadas, dim=0)
         # Retorno: <4> x <1(lote)> x <qtde_tokens> x <768 ou 1024>
-        #print('resultadoStack=',resultadoStack.size())
+        #print('resultado_stack=',resultado_stack.size())
       
         # Realiza a soma dos embeddings de todos os tokens para as camadas
         # Entrada: <4> x <1(lote)> x <qtde_tokens> x <768 ou 1024>
-        resultado = torch.sum(resultadoStack, dim=0)
+        resultado = torch.sum(resultado_stack, dim=0)
         # Saida: <1(lote)> x <qtde_tokens> x <768 ou 1024>
         #print('resultado=',resultado.size())
 
         return resultado
 
     # ============================
-    def getEmbeddingConcat4UltimasCamadas(self, sentencaEmbedding):
+    def getEmbeddingConcat4UltimasCamadas(self, sentenca_embedding):
         '''
         Retorna os embeddings da concatenação das 4 últimas camadas.
         '''
         
         # Cada elemento do vetor sentencaEmbedding é formado por:  
         # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
         # hidden_states é uma lista python, e cada elemento um tensor pytorch no formado <lote> x <qtde_tokens> x <768 ou 1024>.
         #[4]outpus e [2]hidden_states 
         #[OUTPUTS]outpus e [OUTPUTS_HIDDEN_STATES]hidden_states      
         
         # Cria uma lista com os tensores a serem concatenados
         # Entrada: List das camadas(13 ou 25) (<1(lote)> x <qtde_tokens> x <768 ou 1024>)  
         # Lista com os tensores a serem concatenados
-        listaConcat = []
+        lista_concatenada = []
         # Percorre os 4 últimos
         for i in [-1, -2, -3, -4]:
             # Concatena da lista
-            listaConcat.append(sentencaEmbedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][i])
+            lista_concatenada.append(sentenca_embedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][i])
         # Retorno: Entrada: List das camadas(4) (<1(lote)> x <qtde_tokens> <768 ou 1024>)  
-        #print('listaConcat=',len(listaConcat))
+        #print('lista_concatenada=',len(lista_concatenada))
 
         # Realiza a concatenação dos embeddings de todos as camadas
         # Retorno: Entrada: List das camadas(4) (<1(lote)> x <qtde_tokens> <768 ou 1024>)  
-        resultado = torch.cat(listaConcat, dim=-1)
+        resultado = torch.cat(lista_concatenada, dim=-1)
         # Retorno: Entrada: (<1(lote)> x <qtde_tokens> <3072 ou 4096>)  
         # print('resultado=',resultado.size())
       
         return resultado   
 
     # ============================
-    def getEmbeddingSomaTodasAsCamada(self, sentencaEmbedding):
+    def getEmbeddingSomaTodasAsCamada(self, sentenca_embedding):
         '''
         Retorna os embeddings da soma de todas as camadas.
         '''
         
         # Cada elemento do vetor sentencaEmbedding é formado por:  
         # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
         # hidden_states é uma lista python, e cada elemento um tensor pytorch no formado <lote> x <qtde_tokens> x <768 ou 1024>.
         #[4]outpus e [2]hidden_states 
         #[OUTPUTS]outpus e [OUTPUTS_HIDDEN_STATES]hidden_states      
       
         # Retorna todas as camadas descontando a primeira(0)
         # Entrada: List das camadas(13 ou 25) (<1(lote)> x <qtde_tokens> x <768 ou 1024>)  
-        embeddingCamadas = sentencaEmbedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][1:]
+        embedding_camadas = sentenca_embedding[OUTPUTS][OUTPUTS_HIDDEN_STATES][1:]
         # Retorno: List das camadas(12 ou 24) (<1(lote)> x <qtde_tokens> <768 ou 1024>)  
 
         # Usa o método `stack` para criar uma nova dimensão no tensor 
         # com a concateção dos tensores dos embeddings.        
         # Entrada: List das camadas(12 ou 24) (<1(lote)> x <qtde_tokens> x <768 ou 1024>)  
-        resultadoStack = torch.stack(embeddingCamadas, dim=0)
+        resultado_stack = torch.stack(embedding_camadas, dim=0)
         # Retorno: <12 ou 24> x <1(lote)> x <qtde_tokens> x <768 ou 1024>
-        #print('resultadoStack=',resultadoStack.size())
+        #print('resultado_stack=',resultado_stack.size())
       
         # Realiza a soma dos embeddings de todos os tokens para as camadas
         # Entrada: <12 ou 24> x <1(lote)> x <qtde_tokens> x <768 ou 1024>
-        resultado = torch.sum(resultadoStack, dim=0)
+        resultado = torch.sum(resultado_stack, dim=0)
         # Saida: <1(lote)> x <qtde_tokens> x <768 ou 1024>
         # print('resultado=',resultado.size())
       
         return resultado
 
     # ============================
-    def getResultadoEmbeddings(self, sentencaEmbedding, camada):
+    def getResultadoEmbeddings(self, sentenca_embedding, camada):
         '''
         Retorna o resultado da operação sobre os embeddings das camadas de acordo com tipo de camada especificada.
         
         Parâmetros:
         `sentencaEmbedding` - Embeddings da stentença.
         `camada` - Camada dos embeddings.
         '''
@@ -305,396 +320,402 @@
         # Cada elemento do vetor sentencaEmbedding é formado por:  
         # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
         # hidden_states é uma lista python, e cada elemento um tensor pytorch no formado <lote> x <qtde_tokens> x <768 ou 1024>.
         #[4]outpus e [2]hidden_states 
         #[OUTPUTS]outpus e [OUTPUTS_HIDDEN_STATES]hidden_states      
         # Entrada: List das camadas(13 ou 25) (<1(lote)> x <qtde_tokens> x <768 ou 1024>) 
 
-        resultadoEmbeddingCamadas = None
+        resultado_embedding_camadas = None
       
         if camada == EmbeddingsCamadas.PRIMEIRA_CAMADA.value[0]:
-            resultadoEmbeddingCamadas = self.getEmbeddingPrimeiraCamada(sentencaEmbedding)
+            resultado_embedding_camadas = self.getEmbeddingPrimeiraCamada(sentenca_embedding)
             #print('resultadoEmbeddingCamadas1=',resultadoEmbeddingCamadas.size())
         else:
             if camada == EmbeddingsCamadas.PENULTIMA_CAMADA.value[0]:
-                resultadoEmbeddingCamadas = self.getEmbeddingPenultimaCamada(sentencaEmbedding)
+                resultado_embedding_camadas = self.getEmbeddingPenultimaCamada(sentenca_embedding)
                 #print('resultadoEmbeddingCamadas1=',resultadoEmbeddingCamadas.size())
             else:                
                 if camada == EmbeddingsCamadas.ULTIMA_CAMADA.value[0]:
-                    resultadoEmbeddingCamadas = self.getEmbeddingUltimaCamada(sentencaEmbedding)
+                    resultado_embedding_camadas = self.getEmbeddingUltimaCamada(sentenca_embedding)
                     #print('resultadoEmbeddingCamadas2=',resultadoEmbeddingCamadas.size())
                 else:
                     if camada == EmbeddingsCamadas.SOMA_4_ULTIMAS_CAMADAS.value[0]:
-                        resultadoEmbeddingCamadas = self.getEmbeddingSoma4UltimasCamadas(sentencaEmbedding)
+                        resultado_embedding_camadas = self.getEmbeddingSoma4UltimasCamadas(sentenca_embedding)
                         #print('resultadoEmbeddingCamadas3=',resultadoEmbeddingCamadas.size())
                     else:                        
                         if camada == EmbeddingsCamadas.CONCAT_4_ULTIMAS_CAMADAS.value[0]:
-                            resultadoEmbeddingCamadas = self.getEmbeddingConcat4UltimasCamadas(sentencaEmbedding)
+                            resultado_embedding_camadas = self.getEmbeddingConcat4UltimasCamadas(sentenca_embedding)
                             #print('resultadoEmbeddingCamadas4=',resultadoEmbeddingCamadas.size())
                         else:
                             if camada == EmbeddingsCamadas.TODAS_AS_CAMADAS.value[0]:                            
-                                resultadoEmbeddingCamadas = self.getEmbeddingSomaTodasAsCamada(sentencaEmbedding)
+                                resultado_embedding_camadas = self.getEmbeddingSomaTodasAsCamada(sentenca_embedding)
                                 #print('resultadoEmbeddingCamadas5=',resultadoEmbeddingCamadas.size())
                                 # Retorno: <1> x <qtde_tokens> x <768 ou 1024>
                             else:
                                 logger.info("Nenhuma seleção da camada dos embeddings foi especificada.")
           
         # Verifica se a primeira dimensão é igual 1 para remover a dimensão de lote 'batches'
         # Entrada: <1> x <qtde_tokens> x <768 ou 1024>
-        if resultadoEmbeddingCamadas.shape[0] == 1:
+        if resultado_embedding_camadas.shape[0] == 1:
             # Remove a dimensão 0 caso seja de tamanho 1.
             # Usa o método 'squeeze' para remover a primeira dimensão(0) pois possui tamanho 1
             # Entrada: <1> x <qtde_tokens> x <768 ou 1024>
-            resultadoEmbeddingCamadas = torch.squeeze(resultadoEmbeddingCamadas, dim=0)     
+            resultado_embedding_camadas = torch.squeeze(resultado_embedding_camadas, dim=0)     
         #print('resultadoEmbeddingCamadas2=', resultadoEmbeddingCamadas.size())    
         # Retorno: <qtde_tokens> x <768 ou 1024>
       
         # Retorna o resultados dos embeddings dos tokens da sentença  
-        return resultadoEmbeddingCamadas
+        return resultado_embedding_camadas
 
     # ============================
-    def getMedidasSentencasEmbeddingMEAN(self, embeddingSi, embeddingSj):
+    def getMedidasSentencasEmbeddingMEAN(self, embedding_si, embedding_sj):
         '''
         Retorna as medidas de duas sentenças Si e Sj utilizando a estratégia MEAN.
         
         Parâmetros:
-        `embeddingSi` - Embeddings da primeira sentença.
-        `embeddingSj` - Embeddings da segunda sentença.
+        `embedding_si` - Embeddings da primeira sentença.
+        `embedding_sj` - Embeddings da segunda sentença.
         
         Retorno:
         `Scos` - Similaridade do cosseno - usando a média dos embeddings Si e Sj das camadas especificadas.
         `Seuc` - Distância euclidiana - usando a média dos embeddings Si e Sj das camadas especificadas.
         `Sman` - Distância de manhattan - usando a média dos embeddings Si e Sj das camadas especificadas.
         '''
 
-        #print('embeddingSi=', embeddingSi.shape) 
-        #print('embeddingSj=', embeddingSj.shape)
+        #print('embedding_si=', embedding_si.shape) 
+        #print('embedding_sj=', embedding_sj.shape)
       
         # As operações de subtração(sub), mul(multiplicação/produto), soma(sum), cosseno(similaridade), euclediana(diferença) e manhattan(diferença)
         # Necessitam que os embeddings tenha a mesmo número de dimensões.
       
         # Calcula a média dos embeddings para os tokens de Si, removendo a primeira dimensão.
         # Entrada: <qtde_tokens> x <768 ou 1024>  
-        mediaEmbeddingSi = torch.mean(embeddingSi, dim=0)    
+        media_embedding_si = torch.mean(embedding_si, dim=0)    
         # Retorno: <768 ou 1024>
         #print('mediaCamadasSi=', mediaCamadasSi.shape)
       
         # Calcula a média dos embeddings para os tokens de Sj, removendo a primeira dimensão.
         # Entrada: <qtde_tokens> x <768 ou 1024>  
-        mediaEmbeddingSj = torch.mean(embeddingSj, dim=0)    
+        media_embedding_sj = torch.mean(embedding_sj, dim=0)    
         # Retorno: <768 ou 1024>
         #print('mediaCamadasSj=', mediaCamadasSj.shape)
         
         # Similaridade do cosseno entre os embeddings Si e Sj
         # Entrada: (<768 ou 1024>) x (<768 ou 1024>)
-        Scos = similaridadeCoseno(mediaEmbeddingSi, mediaEmbeddingSj)
+        Scos = similaridadeCoseno(media_embedding_si, media_embedding_sj)
         # Retorno: Número real
 
         # Distância euclidiana entre os embeddings Si e Sj
         # Entrada: (<768 ou 1024>) x (<768 ou 1024>)
-        Seuc = distanciaEuclidiana(mediaEmbeddingSi, mediaEmbeddingSj)
+        Seuc = distanciaEuclidiana(media_embedding_si, media_embedding_sj)
         # Retorno: Número real
 
         # Distância de manhattan entre os embeddings Si e Sj
         # Entrada: (<768 ou 1024>) x (<768 ou 1024>)
-        Sman = distanciaManhattan(mediaEmbeddingSi, mediaEmbeddingSj)
+        Sman = distanciaManhattan(media_embedding_si, media_embedding_sj)
         # Retorno: Número real
 
         # Retorno das medidas das sentenças  
-        return mediaEmbeddingSi, mediaEmbeddingSj, Scos, Seuc, Sman
+        return media_embedding_si, media_embedding_sj, Scos, Seuc, Sman
 
     # ============================
-    def getMedidasSentencasEmbeddingMAX(self, embeddingSi, embeddingSj):
+    def getMedidasSentencasEmbeddingMAX(self, embedding_si, embedding_sj):
         '''
         Retorna as medidas de duas sentenças Si e Sj utilizando a estratégia MAX.
         
         Parâmetros:
-        `embeddingSi` - Embeddings da primeira sentença.
-        `embeddingSj` - Embeddings da segunda sentença.
+        `embedding_si` - Embeddings da primeira sentença.
+        `embedding_sj` - Embeddings da segunda sentença.
            
         Retorno:
         `Scos` - Similaridade do cosseno - usando o maior dos embeddings Si e Sj das camadas especificadas.
         `Seuc` - Distância euclidiana - usando o maior dos embeddings Si e Sj das camadas especificadas.
         `Sman` - Distância de manhattan - usando o maior dos embeddings Si e Sj das camadas especificadas.
         '''
 
-        #print('embeddingSi=', embeddingSi.shape) 
-        #print('embeddingSj=', embeddingSj.shape)
+        #print('embedding_si=', embedding_si.shape) 
+        #print('embedding_sj=', embedding_sj.shape)
 
         # As operações de subtração(sub), mul(multiplicação/produto), soma(sum), cosseno(similaridade), euclediana(diferença) e manhattan(diferença)
         # Necessitam que os embeddings tenha a mesmo número de dimensões.
 
         # Encontra os maiores embeddings os tokens de Si, removendo a primeira dimensão.
         # Entrada: <qtde_tokens> x <768 ou 1024>  
-        maiorEmbeddingSi, linha = torch.max(embeddingSi, dim=0)    
+        maior_embedding_si, linha = torch.max(embedding_si, dim=0)    
         # Retorno: <768 ou 1024>
-        #print('maiorEmbeddingSi=', maiorEmbeddingSi.shape)
+        #print('maior_embedding_si=', maior_embedding_si.shape)
 
         # Encontra os maiores embeddings os tokens de Sj, removendo a primeira dimensão.
         # Entrada: <qtde_tokens> x <768 ou 1024>  
-        maiorEmbeddingSj, linha = torch.max(embeddingSj, dim=0)    
+        maior_embedding_sj, linha = torch.max(embedding_sj, dim=0)    
         # Retorno: <768 ou 1024>
-        #print('maiorEmbeddingSj=', maiorEmbeddingSj.shape)
+        #print('maior_embedding_sj=', maior_embedding_sj.shape)
 
         # Similaridade do cosseno entre os embeddings Si e Sj
         # Entrada: (<768 ou 1024>) x (<768 ou 1024>)
-        Scos = similaridadeCoseno(maiorEmbeddingSi, maiorEmbeddingSj)
+        Scos = similaridadeCoseno(maior_embedding_si, maior_embedding_sj)
         # Retorno: Número real
 
         # Distância euclidiana entre os embeddings Si e Sj
         # Entrada: (<768 ou 1024>) x (<768 ou 1024>)
-        Seuc = distanciaEuclidiana(maiorEmbeddingSi, maiorEmbeddingSj)
+        Seuc = distanciaEuclidiana(maior_embedding_si, maior_embedding_sj)
         # Retorno: Número real
 
         # Distância de manhattan entre os embeddings Si e Sj
         # Entrada: (<768 ou 1024>) x (<768 ou 1024>)
-        Sman = distanciaManhattan(maiorEmbeddingSi, maiorEmbeddingSj)
+        Sman = distanciaManhattan(maior_embedding_si, maior_embedding_sj)
         # Retorno: Número real
 
         # Retorno das medidas das sentenças
-        return maiorEmbeddingSi, maiorEmbeddingSj, Scos, Seuc, Sman
+        return maior_embedding_si, maior_embedding_sj, Scos, Seuc, Sman
 
     # ============================
-    def getMedidasSentencasEmbedding(self, embeddingSi, embeddingSj):
+    def getMedidasSentencasEmbedding(self, embedding_si, embedding_sj):
         '''
         Realiza o cálculo da medida do texto de acordo com a estratégia de pooling(MAX ou MEAN).
         
         Parâmetros:
-        `embeddingSi` - Embeddings da primeira sentença.
-        `embeddingSj` - Embeddings da segunda sentença.
+        `embedding_si` - Embeddings da primeira sentença.
+        `embedding_sj` - Embeddings da segunda sentença.
         `estrategia_pooling` - Estratégia de pooling a ser utilizada.       
         '''
 
         if self.model_args.estrategia_pooling == EstrategiasPooling.MEAN.value:
-            return self.getMedidasSentencasEmbeddingMEAN(embeddingSi, embeddingSj)
+            return self.getMedidasSentencasEmbeddingMEAN(embedding_si, embedding_sj)
         else:
             if self.model_args.estrategia_pooling == EstrategiasPooling.MAX.value:
-                return self.getMedidasSentencasEmbeddingMAX(embeddingSi, embeddingSj)
+                return self.getMedidasSentencasEmbeddingMAX(embedding_si, embedding_sj)
             else:
                 logger.info("Nenhuma seleção da estratégia de pooling foi especificada.")
+                return None
 
     # ============================
     def getEmbeddingSentencaEmbeddingTextoALL(self, 
-                                              embeddingTexto, 
+                                              embedding_texto, 
                                               texto, 
                                               sentenca):
         '''
         Retorna os embeddings de uma sentença com todas as palavras(ALL) a partir dos embeddings do texto.
         
         '''
             
         # Tokeniza o texto
-        textoTokenizado =  self.transformer.getTextoTokenizado(texto)
-        #print(textoTokenizado)
+        texto_tokenizado =  self.transformer.getTextoTokenizado(texto)
+        #print(texto_tokenizado)
 
         # Tokeniza a sentença
-        sentencaTokenizada =  self.transformer.getTextoTokenizado(sentenca)
+        sentenca_tokenizada =  self.transformer.getTextoTokenizado(sentenca)
         #print(sentencaTokenizada)
         # Remove os tokens de início e fim da sentença
-        sentencaTokenizada.remove('[CLS]')
-        sentencaTokenizada.remove('[SEP]')    
-        #print(len(sentencaTokenizada))
+        sentenca_tokenizada.remove('[CLS]')
+        sentenca_tokenizada.remove('[SEP]')    
+        #print(len(sentenca_tokenizada))
 
         # Localiza os índices dos tokens da sentença no texto
-        inicio, fim = encontrarIndiceSubLista(textoTokenizado, sentencaTokenizada)
+        inicio, fim = encontrarIndiceSubLista(texto_tokenizado, sentenca_tokenizada)
         #print(inicio,fim) 
 
         # Recupera os embeddings dos tokens da sentença a partir dos embeddings do texto
-        embeddingSentenca = embeddingTexto[inicio:fim + 1]
-        #print('embeddingSentenca=', embeddingSentenca.shape)
+        embedding_sentenca = embedding_texto[inicio:fim + 1]
+        #print('embedding_sentenca=', embedding_sentenca.shape)
 
         # Retorna o embedding da sentença no texto
-        return embeddingSentenca
+        return embedding_sentenca
 
     # ============================
     def getEmbeddingSentencaEmbeddingTextoCLEAN(self, 
-                                                embeddingTexto, 
+                                                embedding_texto, 
                                                 texto, 
                                                 sentenca):
         '''
         Retorna os embeddings de uma sentença sem stopwords(CLEAN) a partir dos embeddings do texto.
         '''
           
         # Tokeniza o texto
-        textoTokenizado =  self.transformer.getTextoTokenizado(texto)  
+        texto_tokenizado =  self.transformer.getTextoTokenizado(texto)  
         #print(textoTokenizado)
 
         # Remove as stopword da sentença
-        sentencaSemStopWord = self.pln.removeStopWord(sentenca)
+        sentenca_sem_stopword = self.pln.removeStopWord(sentenca)
 
         # Tokeniza a sentença sem stopword
-        sentencaTokenizadaSemStopWord =  self.transformer.getTextoTokenizado(sentencaSemStopWord)
-        #print(sentencaTokenizadaSemStopWord)
+        sentenca_tokenizada_sem_stopword =  self.transformer.getTextoTokenizado(sentenca_sem_stopword)
+        #print(sentenca_tokenizada_sem_stopword)
 
         # Remove os tokens de início e fim da sentença
-        sentencaTokenizadaSemStopWord.remove('[CLS]')
-        sentencaTokenizadaSemStopWord.remove('[SEP]')    
-        #print(len(sentencaTokenizadaSemStopWord))
+        sentenca_tokenizada_sem_stopword.remove('[CLS]')
+        sentenca_tokenizada_sem_stopword.remove('[SEP]')    
+        #print(len(sentenca_tokenizada_sem_stopword))
 
         # Tokeniza a sentença
-        sentencaTokenizada =  self.transformer.getTextoTokenizado(sentenca)
+        sentenca_tokenizada =  self.transformer.getTextoTokenizado(sentenca)
 
         # Remove os tokens de início e fim da sentença
-        sentencaTokenizada.remove('[CLS]')
-        sentencaTokenizada.remove('[SEP]')  
-        #print(sentencaTokenizada)
-        #print(len(sentencaTokenizada))
+        sentenca_tokenizada.remove('[CLS]')
+        sentenca_tokenizada.remove('[SEP]')  
+        #print(sentenca_tokenizada)
+        #print(len(sentenca_tokenizada))
 
         # Localiza os índices dos tokens da sentença no texto
-        inicio, fim = encontrarIndiceSubLista(textoTokenizado, sentencaTokenizada)
+        inicio, fim = encontrarIndiceSubLista(texto_tokenizado, sentenca_tokenizada)
         #print('Sentença inicia em:', inicio, 'até', fim) 
 
         # Recupera os embeddings dos tokens da sentença a partir dos embeddings do texto
-        embeddingSentenca = embeddingTexto[inicio:fim + 1]
-        #print('embeddingSentenca=', embeddingSentenca.shape)
+        embedding_sentenca = embedding_texto[inicio:fim + 1]
+        #print('embedding_sentenca=', embedding_sentenca.shape)
 
         # Lista com os tensores selecionados
-        listaTokensSelecionados = []
+        lista_tokens_selecionados = []
         # Localizar os embeddings dos tokens da sentença tokenizada sem stop word na sentença 
         # Procura somente no intervalo da sentença
-        for i, tokenSentenca in enumerate(sentencaTokenizada):
-            for tokenSentencaSemStopWord in sentencaTokenizadaSemStopWord: 
+        for i, token_sentenca in enumerate(sentenca_tokenizada):
+            for token_sentenca_sem_stopword in sentenca_tokenizada_sem_stopword: 
                 # Se o token da sentença é igual ao token da sentença sem stopword    
-                if tokenSentenca == tokenSentencaSemStopWord:
-                    listaTokensSelecionados.append(embeddingSentenca[i:i + 1])
+                if token_sentenca == token_sentenca_sem_stopword:
+                    lista_tokens_selecionados.append(embedding_sentenca[i:i + 1])
 
-        embeddingSentencaSemStopWord = None
+        embedding_sentenca_sem_stopword = None
 
-        if len(listaTokensSelecionados) != 0:
+        if len(lista_tokens_selecionados) != 0:
             # Concatena os vetores da lista pela dimensão 0
-            embeddingSentencaSemStopWord = torch.cat(listaTokensSelecionados, dim=0)
-            #print("embeddingSentencaSemStopWord:",embeddingSentencaSemStopWord.shape)
+            embedding_sentenca_sem_stopword = torch.cat(lista_tokens_selecionados, dim=0)
+            #print("embedding_sentenca_sem_stopword:",embedding_sentenca_sem_stopword.shape)
 
         # Retorna o embedding da sentença no texto
-        return embeddingSentencaSemStopWord
+        return embedding_sentenca_sem_stopword
 
     # ============================
     def getEmbeddingSentencaEmbeddingTextoNOUN(self, 
-                                               embeddingTexto, 
+                                               embedding_texto, 
                                                texto, 
                                                sentenca):
         '''
         Retorna os embeddings de uma sentença somente com as palavras relevantes(NOUN) de um tipo a partir dos embeddings do texto.
         '''
 
         # Tokeniza o texto
-        textoTokenizado =  self.transformer.getTextoTokenizado(texto)  
+        texto_tokenizado =  self.transformer.getTextoTokenizado(texto)  
         #print(textoTokenizado)
 
         # Retorna as palavras relevantes da sentença do tipo especificado
-        sentencaSomenteRelevante = self.pln.retornaPalavraRelevante(sentenca, self.model_args.palavra_relevante)
+        sentenca_somente_relevante = self.pln.retornaPalavraRelevante(sentenca, self.model_args.palavra_relevante)
 
         # Tokeniza a sentença 
-        sentencaTokenizadaSomenteRelevante =  self.transformer.getTextoTokenizado(sentencaSomenteRelevante)
+        sentenca_tokenizada_somente_relevante =  self.transformer.getTextoTokenizado(sentenca_somente_relevante)
 
         # Remove os tokens de início e fim da sentença
-        sentencaTokenizadaSomenteRelevante.remove('[CLS]')
-        sentencaTokenizadaSomenteRelevante.remove('[SEP]')  
-        #print(sentencaTokenizadaSomenteRelevante)
-        #print(len(sentencaTokenizadaSomenteRelevante))
+        sentenca_tokenizada_somente_relevante.remove('[CLS]')
+        sentenca_tokenizada_somente_relevante.remove('[SEP]')  
+        #print(sentenca_tokenizada_somente_relevante)
+        #print(len(sentenca_tokenizada_somente_relevante))
 
         # Tokeniza a sentença
-        sentencaTokenizada =  self.transformer.getTextoTokenizado(sentenca)
+        sentenca_tokenizada =  self.transformer.getTextoTokenizado(sentenca)
 
         # Remove os tokens de início e fim da sentença
-        sentencaTokenizada.remove('[CLS]')
-        sentencaTokenizada.remove('[SEP]')  
-        #print(sentencaTokenizada)
-        #print(len(sentencaTokenizada))
+        sentenca_tokenizada.remove('[CLS]')
+        sentenca_tokenizada.remove('[SEP]')  
+        #print(sentenca_tokenizada)
+        #print(len(sentenca_tokenizada))
 
         # Localiza os índices dos tokens da sentença no texto
-        inicio, fim = encontrarIndiceSubLista(textoTokenizado, sentencaTokenizada)
+        inicio, fim = encontrarIndiceSubLista(texto_tokenizado, sentenca_tokenizada)
         #print('Sentença inicia em:', inicio, 'até', fim) 
 
         # Recupera os embeddings dos tokens da sentença a partir dos embeddings do texto
-        embeddingSentenca = embeddingTexto[inicio:fim + 1]
-        #print('embeddingSentenca=', embeddingSentenca.shape)
+        embedding_sentenca = embedding_texto[inicio:fim + 1]
+        #print('embedding_sentenca=', embedding_sentenca.shape)
 
         # Lista com os tensores selecionados
         listaTokensSelecionados = []
         # Localizar os embeddings dos tokens da sentença tokenizada sem stop word na sentença 
         # Procura somente no intervalo da sentença
-        for i, tokenSentenca in enumerate(sentencaTokenizada):
-            for tokenSentencaSomenteRelevante in sentencaTokenizadaSomenteRelevante: 
-                if tokenSentenca == tokenSentencaSomenteRelevante:        
-                    listaTokensSelecionados.append(embeddingSentenca[i:i + 1])
+        for i, token_sentenca in enumerate(sentenca_tokenizada):
+            for token_sentenca_somente_relevante in sentenca_tokenizada_somente_relevante: 
+                if token_sentenca == token_sentenca_somente_relevante:        
+                    listaTokensSelecionados.append(embedding_sentenca[i:i + 1])
 
-        embeddingSentencaComSubstantivo = None
+        embedding_sentenca_com_substantivo = None
 
         if len(listaTokensSelecionados) != 0:
             # Concatena os vetores da lista pela dimensão 0  
-            embeddingSentencaComSubstantivo = torch.cat(listaTokensSelecionados, dim=0)
-            #print("embeddingSentencaComSubstantivo:",embeddingSentencaComSubstantivo.shape)
+            embedding_sentenca_com_substantivo = torch.cat(listaTokensSelecionados, dim=0)
+            #print("embedding_sentenca_com_substantivo:",embedding_sentenca_com_substantivo.shape)
 
         # Retorna o embedding da sentença do texto
-        return embeddingSentencaComSubstantivo
+        return embedding_sentenca_com_substantivo
 
     # ============================
     def getEmbeddingSentencaEmbeddingTexto(self, 
-                                           embeddingTexto, 
+                                           embedding_texto, 
                                            texto, 
                                            sentenca):
         '''
         Retorna os embeddings de uma sentença considerando a relevância das palavras (ALL, CLEAN ou NOUN) a partir dos embeddings do texto.    
         '''
 
         if self.model_args.palavra_relevante == PalavrasRelevantes.ALL.value:
-            return self.getEmbeddingSentencaEmbeddingTextoALL(embeddingTexto, texto, sentenca)
+            return self.getEmbeddingSentencaEmbeddingTextoALL(embedding_texto, texto, sentenca)
         else:
             if self.model_args.palavra_relevante == PalavrasRelevantes.CLEAN.value:                
-                return self.getEmbeddingSentencaEmbeddingTextoCLEAN(embeddingTexto, texto, sentenca)
+                return self.getEmbeddingSentencaEmbeddingTextoCLEAN(embedding_texto, texto, sentenca)
             else:
                 if self.model_args.palavra_relevante == PalavrasRelevantes.NOUN.value:
-                    return self.getEmbeddingSentencaEmbeddingTextoNOUN(embeddingTexto, texto, sentenca)
+                    return self.getEmbeddingSentencaEmbeddingTextoNOUN(embedding_texto, texto, sentenca)
                 else:
                     logger.info("Nenhuma estratégia de relevância de palavras foi especificada.") 
 
     # ============================
     def getMedidasComparacaoTexto(self, 
                                   texto, 
                                   camada, 
-                                  tipoTexto='p'):
+                                  tipo_texto='p'):
         '''
-        Retorna as medidas de coerência do texto.
+        Retorna as medidas do texto.
         Considera somente sentenças com pelo menos uma palavra.
         Estratégia de pooling padrão é MEAN(0).
         Palavra relavante padrão é ALL(0).
+        
+        Retorno um dicionário com:
+        `cos` - Medida de cos do do texto.
+        `euc` - Medida de euc do do texto.
+        `man` - Medida de man do do texto.
         '''
 
         # Quantidade de sentenças no texto
         n = len(texto)
         
         # Divisor da quantidade de textos
         divisor = n - 1
 
         # Texto é uma lista com as sentenças
         #print('camada=',camada)
         #print('Texto=', texto)
 
         # Junta a lista de sentenças em um texto(string)
-        stringTexto = ' '.join(texto)
+        string_texto = ' '.join(texto)
 
         # Envia o texto ao MCL e recupera os embeddings de todas as camadas
         # Se for o texto original pega do buffer para evitar a repetição
-        if tipoTexto == 'o':
+        if tipo_texto == 'o':
             # Retorna os embeddings de todas as camadas do texto
             # O embedding possui os seguintes valores        
             # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
-            totalCamadasTexto = self.getEmbeddingsTodasCamadasBuffer(stringTexto)      
+            total_camadas_texto = self.getEmbeddingsTodasCamadasBuffer(string_texto)      
             # Retorno: List das camadas(13 ou 25) (<1(lote)> x <qtde_tokens> <768 ou 1024>) 
         else:
             # Retorna os embeddings de todas as camadas do texto
             # O embedding possui os seguintes valores        
             # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
-            totalCamadasTexto = self.getEmbeddingsTodasCamadas(stringTexto)      
+            total_camadas_texto = self.getEmbeddingsTodasCamadas(string_texto)      
             # Retorno: List das camadas(13 ou 25) (<1(lote)> x <qtde_tokens> <768 ou 1024>) 
 
         # Recupera os embeddings dos tokens das camadas especificadas de acordo com a estratégia especificada para camada  
-        embeddingTexto = self.getResultadoEmbeddings(totalCamadasTexto, camada=camada)
-        #print('embeddingTexto=', embeddingTexto.shape)
+        embedding_texto = self.getResultadoEmbeddings(total_camadas_texto, camada=camada)
+        #print('embedding_texto=', embedding_texto.shape)
 
         # Acumuladores das medidas entre as sentenças  
         somaScos = 0
         somaSeuc = 0
         somaSman = 0
 
         # Seleciona os pares de sentença a serem avaliados
@@ -705,63 +726,55 @@
         while posSj <= (n-1):  
 
             # Seleciona as sentenças do texto  
             Si = texto[posSi]
             Sj = texto[posSj]
 
             # Recupera os embedding das sentenças Si e Sj do embedding do texto      
-            embeddingSi = self.getEmbeddingSentencaEmbeddingTexto(embeddingTexto, stringTexto, Si)
-            embeddingSj = self.getEmbeddingSentencaEmbeddingTexto(embeddingTexto, stringTexto, Sj)
+            embedding_si = self.getEmbeddingSentencaEmbeddingTexto(embedding_texto, string_texto, Si)
+            embedding_sj = self.getEmbeddingSentencaEmbeddingTexto(embedding_texto, string_texto, Sj)
 
             # Verifica se os embeddings sentenças estão preenchidos
-            if embeddingSi != None and embeddingSj != None:
+            if embedding_si != None and embedding_sj != None:
 
                 # Recupera as medidas entre Si e Sj     
-                ajustadoEmbeddingSi, ajustadoEmbeddingSj, Scos, Seuc, Sman = self.getMedidasSentencasEmbedding(embeddingSi, embeddingSj)
+                ajustado_embedding_si, ajustado_embedding_sj, Scos, Seuc, Sman = self.getMedidasSentencasEmbedding(embedding_si, embedding_sj)
 
                 # Acumula as medidas
                 somaScos = somaScos + Scos
                 somaSeuc = somaSeuc + Seuc
                 somaSman = somaSman + Sman
 
                     # avança para o próximo par de sentenças
                 posSi = posSj
                 posSj = posSj + 1
             else:
                 # Reduz um da quantidade de sentenças pois uma delas está vazia
                 divisor = divisor - 1
                 # Se embeddingSi igual a None avanca pos1 e pos2
-                if embeddingSi == None:
+                if embedding_si == None:
                     # Avança a posição da sentença posSi para a posSj
                     posSi = posSj
                     # Avança para a próxima sentença de posSj
                     posSj = posSj + 1        
                 else:          
                     # Se embeddingSj = None avança somente posJ para a próxima sentença
-                    if embeddingSj == None:
+                    if embedding_sj == None:
                         posSj = posSj + 1
 
         # Calcula a medida 
         Ccos = 0
         Ceuc = 0
         Cman = 0
 
         if divisor != 0:
             Ccos = float(somaScos) / float(divisor)
             Ceuc = float(somaSeuc) / float(divisor)
             Cman = float(somaSman) / float(divisor)
 
-        return Ccos, Ceuc, Cman
-   
-    # ============================
-    def comparaMedidasCamadasSentencas(self, Si, Sj, camada):
-        '''
-        Facilita a exibição dos valores de comparação de duas orações.
-        '''
-      
-        # Recupera os embeddings da sentença Si e sentença Sj e suas medidas
-        embeddingSi, embeddingSj, Scos, Seuc, Sman = self.getMedidasCamadasSentencas(Si, Sj, camada)
+        # Retorna as medidas em um dicionário
+        saida = {}
+        saida.update({'cos' : Ccos,
+                      'euc' : Ceuc,
+                      'man' : Cman})
 
-        logger.info('  ->Mostra comparação da ' + camada[LISTATIPOCAMADA_NOME] + ' camada(s)')    
-        logger.info('   Cosseno(SixSj)     = %.8f' % Scos)
-        logger.info('   Euclidiana(SixSj)  = %.8f' % Seuc)
-        logger.info('   Manhattan(SixSj)   = %.8f' % Sman)
+        return saida
```

### Comparing `texto_transformer-0.0.1/textotransformer/modelo/modeloarguments.py` & `texto_transformer-0.0.2/textotransformer/modelo/modeloarguments.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.1/textotransformer/modelo/modeloenum.py` & `texto_transformer-0.0.2/textotransformer/modelo/modeloenum.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.1/textotransformer/modelo/transformer.py` & `texto_transformer-0.0.2/textotransformer/modelo/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,91 +7,93 @@
 import torch 
 from torch import Tensor, device
 # Biblioteca do transformer
 from transformers import AutoModel, AutoTokenizer, AutoConfig, T5Config, MT5Config
 # Biblioteca de manipulação json
 import json
 # Biblioteca de tipos
-from typing import List, Dict, Optional, Union, Tuple
+from typing import List, Dict, Optional, Union
 # Biblioteca de manipulação sistema
 import os
 
 # Bibliotecas próprias
 from textotransformer.modelo.modeloarguments import ModeloArgumentos
 from textotransformer.modelo.modeloenum import listaTipoCamadas
 
 logger = logging.getLogger(__name__)
 
 class Transformer(nn.Module):
     '''
-    Huggingface AutoModel para gerar embeddings de token, palavra, sentença ou texto.
+    Classe que encapsula a classe AutoModel da Huggingface para gerar embeddings de token, palavra, sentença ou texto.
     Carrega a classe correta, por exemplo BERT / RoBERTa etc.
 
      :param modelo_args: Argumentos passados para o modelo Huggingface Transformers          
      :param cache_dir: Cache dir para Huggingface Transformers para armazenar/carregar modelos
      :param tokenizer_args: Argumentos (chave, pares de valor) passados para o modelo Huggingface Tokenizer
      :param tokenizer_name_or_path: Nome ou caminho do tokenizer. Quando None, model_name_or_path é usado
     
     '''
     def __init__(self, 
-                modelo_args : ModeloArgumentos,
-                max_seq_length: Optional[int] = None,                
+                modelo_args : ModeloArgumentos,                
                 cache_dir: Optional[str] = None,
                 tokenizer_args: Dict = {}, 
                 tokenizer_name_or_path : str = None):
         
         # Inicializa o construtor da superclasse
         super(Transformer, self).__init__()
         
         # Define os argumentos do modelo
         self.modelo_args = modelo_args
 
         # Recupera o nome do modelo dos argumentos
         model_name_or_path = modelo_args.pretrained_model_name_or_path;
-        # Recupera o tamanho máximo de um texto
-        max_seq_length = modelo_args.max_seq_len
-        
-        # Parâmetros do modelo
-        self.config_keys = ['max_seq_length', 'do_lower_case']
-        self.do_lower_case = modelo_args.do_lower_case
-
+      
         # Recupera parâmetros do transformador dos argumentos
         model_args = {"output_attentions": modelo_args.output_attentions, 
                       "output_hidden_states": modelo_args.output_hidden_states}
     
         # Configuração do modelo        
-        config = AutoConfig.from_pretrained(model_name_or_path, 
+        self.config = AutoConfig.from_pretrained(model_name_or_path, 
                                             **model_args, 
                                             cache_dir=cache_dir)
         
         # Carrega o modelo
         self._load_model(model_name_or_path, 
-                         config, 
+                         self.config, 
                          cache_dir)
 
         # Carrega o tokenizador
         self.tokenizer = AutoTokenizer.from_pretrained(tokenizer_name_or_path if tokenizer_name_or_path is not None else  model_name_or_path, cache_dir=cache_dir, **tokenizer_args)
 
         #Se max_seq_length não foi especificado, tenta inferir do modelo
-        if max_seq_length is None:
+        if self.modelo_args.max_seq_len is None:
             if hasattr(self.auto_model, "config") and hasattr(self.auto_model.config, "max_position_embeddings") and hasattr(self.tokenizer, "model_max_length"):
-                max_seq_length = min(self.auto_model.config.max_position_embeddings,
+                self.modelo_args.max_seq_len = min(self.auto_model.config.max_position_embeddings,
                                      self.tokenizer.model_max_length)
 
-        # Define o máximo de tokens
-        self.max_seq_length = max_seq_length
-
         # Define a classe do tokenizador
         if tokenizer_name_or_path is not None:
             self.auto_model.config.tokenizer_class = self.tokenizer.__class__.__name__
             
         logger.info("Classe Transformer carregada: {}.".format(modelo_args))            
 
     # ============================   
-    def _load_model(self, model_name_or_path, config, cache_dir):
+    def __repr__(self):
+        '''
+        Retorna uma string com descrição do objeto
+        '''
+        return "Classe ({}) com AutoConfig: {}, modelo Transformer: {} e tokenizador: {}.".format(self.__class__.__name__, 
+                                                                                                             self.config.__class__.__name__,
+                                                                                                             self.auto_model.__class__.__name__,
+                                                                                                             self.tokenizer.__class__.__name__)
+
+    # ============================   
+    def _load_model(self, 
+                    model_name_or_path: str, 
+                    config, cache_dir):
         '''
         Carrega o modelo transformer
         '''
         # Carregamento T5
         if isinstance(config, T5Config):
             self._load_t5_model(model_name_or_path, 
                                 config, 
@@ -106,44 +108,41 @@
             else:
                 # Carrega modelos genéricos
                 self.auto_model = AutoModel.from_pretrained(model_name_or_path, 
                                                             config=config, 
                                                             cache_dir=cache_dir)
 
     # ============================   
-    def _load_t5_model(self, model_name_or_path, config, cache_dir):
+    def _load_t5_model(self, model_name_or_path: str, 
+                       config, 
+                       cache_dir):
         '''
         Carrega codificador do modelo¨T5
         '''
         from transformers import T5EncoderModel
         T5EncoderModel._keys_to_ignore_on_load_unexpected = ["decoder.*"]
         self.auto_model = T5EncoderModel.from_pretrained(model_name_or_path, 
                                                          config=config, 
                                                          cache_dir=cache_dir)
 
     # ============================   
-    def _load_mt5_model(self, model_name_or_path, config, cache_dir):
+    def _load_mt5_model(self, model_name_or_path: str, 
+                        config, 
+                        cache_dir):
         '''
         Carrega codificador do modelo MT5
         '''
         from transformers import MT5EncoderModel
         MT5EncoderModel._keys_to_ignore_on_load_unexpected = ["decoder.*"]
         self.auto_model = MT5EncoderModel.from_pretrained(model_name_or_path, 
                                                           config=config, 
                                                           cache_dir=cache_dir)
-    
-    # ============================   
-    def __repr__(self):
-        '''
-        Retorna uma string com descrição do objeto
-        '''
-        return "Transformer({}) com modelo Transformer: {} ".format(self.get_config_dict(), 
-                                                                    self.auto_model.__class__.__name__)
+   
     # ============================      
-    def getTextoTokenizado(self, texto: str):
+    def getTextoTokenizado(self, texto : str):
         '''
         Retorna um texto tokenizado e concatenado com tokens especiais '[CLS]' no início e o token '[SEP]' no fim para ser submetido ao modelo de linguagem.
         
         Parâmetros:
         `texto` - Um texto a ser tokenizado.
         
         Retorno:
@@ -154,23 +153,24 @@
         textoMarcado = '[CLS] ' + texto + ' [SEP]'
 
         # Tokeniza o texto
         textoTokenizado = self.tokenizer.tokenize(textoMarcado)
 
         return textoTokenizado
 
-    # ============================       
-    def tokenize(self, texto):
+    # ============================    
+
+    def tokenize(self, texto: Union[str, List[str]]):
         '''        
         Tokeniza um texto para submeter ao modelo de linguagem. 
         Retorna um dicionário listas de mesmo tamanho para garantir o processamento em lote.
         Use a quantidade de tokens para saber até onde deve ser recuperado em uma lista de saída.
         Ou use attention_mask diferente de 1 para saber que posições devem ser utilizadas na lista.
 
-        :param texto: Texto a ser tokenizado para o modelo de linguagem.
+        :param texto: Texto é uma string ou uma lista de strings a serem tokenizados para o modelo de linguagem.
          
         Retorna um dicionário com:
             tokens_texto_mcl uma lista com os textos tokenizados com os tokens especiais.
             input_ids uma lista com os ids dos tokens de entrada mapeados em seus índices do vocabuário.
             token_type_ids uma lista com os tipos dos tokens.
             attention_mask uma lista com os as máscaras de atenção indicando com '1' os tokens  pertencentes à sentença.
         '''
@@ -188,43 +188,43 @@
                 # Se for uma lista de listas de strings, não faz nada
                 to_tokenize = texto
                 
         # Remove os espaços em branco antes e depois de cada texto usando strip
         to_tokenize = [[str(s).strip() for s in col] for col in to_tokenize]
 
         # Se for para colocar para minúsculo usa Lowercase nos textos
-        if self.do_lower_case:
+        if self.modelo_args.do_lower_case:
            to_tokenize = [[s.lower() for s in col] for col in to_tokenize]
 
         # Tokeniza o texto
         # Faz o mesmo que o método encode_plus com uma string e o mesmo que batch_encode_plus com uma lista de strings
         saida.update(self.tokenizer(*to_tokenize,  # Texto a ser codificado.
                                      add_special_tokens=True, # Adiciona os tokens especiais '[CLS]' e '[SEP]'
                                      padding=True, # Preenche o texto até max_length
                                      truncation='longest_first',  # Trunca o texto no maior texto
                                      return_tensors="pt",  # Retorna os dados como tensores pytorch.
-                                     max_length=self.max_seq_length # Define o tamanho máximo para preencheer ou truncar.
+                                     max_length=self.modelo_args.max_seq_len # Define o tamanho máximo para preencheer ou truncar.
                                     ) 
                     )
                         
-        # Gera o texto tokenizado        
-        saida['tokens_texto_mcl'] = [[self.getTextoTokenizado(s) for s in col] for col in to_tokenize][0]
+        # Gera o texto tokenizado convertendo os ids para os respectivos tokens           
+        saida['tokens_texto_mcl'] = [[self.tokenizer.convert_ids_to_tokens(s.item()) for s in col] for col in saida['input_ids']]
 
         # Guarda o texto original        
-        saida['texto_original'] = [[s for s in col] for col in to_tokenize][0]
+        saida['texto_original'] = [[s for s in col] for col in to_tokenize][0]     
         
         # Verifica se existe algum texto maior que o limite de tokenização
         for tokens in saida['tokens_texto_mcl']:
             if len(tokens) >= 512:
                 logger.info("Utilizando embeddings do modelo de: {}.".format(listaTipoCamadas[self.modelo_args.camadas_embeddings]))   
-                        
+  
         return saida
-    
+        
     # ============================           
-    def forward(self, texto):
+    def getSaidaRede(self, texto: Union[str, dict]):
         '''
         De um texto preparado(tokenizado) ou não, retorna os embeddings dos tokens do texto. 
         O retorno é um dicionário com token_embeddings, input_ids, attention_mask, token_type_ids, 
         tokens_texto_mcl, texto_original  e all_layer_embeddings.
         
         Retorna os embeddings de todas as camadas de um texto.
     
@@ -261,91 +261,14 @@
         # como é configurado na chamada do método `from_pretrained` anterior. Nesse caso,
         # porque definimos `output_hidden_states = True`, o terceiro item será o
         # estados ocultos(hidden_states) de todas as camadas. Veja a documentação para mais detalhes:
         # https://huggingface.co/transformers/model_doc/bert.html#bertmodel
 
         # Retorno de model quando ´output_hidden_states=True´ é setado:    
         # outputs[0] = last_hidden_state, outputs[1] = pooler_output, outputs[2] = hidden_states
-        # hidden_states é uma lista python, e cada elemento um tensor pytorch no formado <lote> x <qtde_tokens> x <768 ou 1024>.        
-        # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
-        
-        last_hidden_state = outputs[0]
-
-        # Adiciona os embeddings da última camada e os dados do texto preparado na saída
-        saida = {}
-        saida.update({'token_embeddings': last_hidden_state,  # Embeddings da última camada
-                      'input_ids': texto['input_ids'],
-                      'attention_mask': texto['attention_mask'],
-                      'token_type_ids': texto['token_type_ids'],        
-                      'tokens_texto_mcl': texto['tokens_texto_mcl'],
-                      'texto_original': texto['texto_original']
-                      }
-                     )
-
-        # output_hidden_states == True existem embeddings nas camadas ocultas
-        if self.auto_model.config.output_hidden_states:
-            # 2 é o índice da saída com todos os embeddings em outputs
-            all_layer_idx = 2
-            if len(outputs) < 3: #Alguns modelos apenas geram last_hidden_states e all_hidden_states
-                all_layer_idx = 1
-
-            hidden_states = outputs[all_layer_idx]
-            # Adiciona os embeddings de todas as camadas na saída
-            saida.update({'all_layer_embeddings': hidden_states})
-
-        return saida
-
-    # ============================           
-    def getEmbeddings(self, texto):
-        '''
-        De um texto preparado(tokenizado) ou não, retorna os embeddings dos tokens do texto. 
-        O retorno é um dicionário com token_embeddings, input_ids, attention_mask, token_type_ids, 
-        tokens_texto_mcl, texto_original  e all_layer_embeddings.
-        
-        Retorna os embeddings de todas as camadas de um texto.
-    
-        Parâmetros:
-        `texto` - Um texto a ser recuperado os embeddings do modelo de linguagem
-    
-        Retorna um dicionário com:            
-            token_embeddings uma lista com os embeddings da última camada
-            input_ids uma lista com os textos indexados.            
-            attention_mask uma lista com os as máscaras de atenção
-            token_type_ids uma lista com os tipos dos tokens.            
-            tokens_texto_mcl uma lista com os textos tokenizados com os tokens especiais.
-            texto_original uma lista com os textos originais.
-            all_layer_embeddings uma lista com os embeddings de todas as camadas.
-        '''
-
-        # Se o texto não estiver tokenizado, tokeniza
-        if not isinstance(texto, dict):
-            texto = self.tokenize(texto)
-    
-        # Recupera o texto preparado pelo tokenizador para envio ao modelo
-        dic_texto_tokenizado = {'input_ids': texto['input_ids'],                                 
-                                'attention_mask': texto['attention_mask']}
-        
-        # Se token_type_ids estiver no texto preparado copia para dicionário
-        if 'token_type_ids' in texto:
-            dic_texto_tokenizado['token_type_ids'] = texto['token_type_ids']
-
-        # Roda o texto através do modelo, e coleta todos os estados ocultos produzidos.
-        with torch.no_grad():
-
-            outputs = self.auto_model(**dic_texto_tokenizado, 
-                                      return_dict=False)
-        
-        # A avaliação do modelo retorna um número de diferentes objetos com base em
-        # como é configurado na chamada do método `from_pretrained` anterior. Nesse caso,
-        # porque definimos `output_hidden_states = True`, o terceiro item será o
-        # estados ocultos(hidden_states) de todas as camadas. Veja a documentação para mais detalhes:
-        # https://huggingface.co/transformers/model_doc/bert.html#bertmodel
-
-        # Retorno de model quando ´output_hidden_states=True´ é setado:    
-        # outputs[0] = last_hidden_state, outputs[1] = pooler_output, outputs[2] = hidden_states
         # hidden_states é uma lista python, e cada elemento um tensor pytorch no formado <lote> x <qtde_tokens> x <768 ou 1024>.
         
         # 0-texto_tokenizado, 1-input_ids, 2-attention_mask, 3-token_type_ids, 4-outputs(0=last_hidden_state,1=pooler_output,2=hidden_states)
         
         last_hidden_state = outputs[0]
 
         # Adiciona os embeddings da última camada e os dados do texto preparado na saída
@@ -377,28 +300,28 @@
     # Gera os tokens, POS e embeddings de cada texto.
     
     # Dicionário de tokens de exceções e seus deslocamentos para considerar mais tokens do BERT em relação ao spaCy
     # A tokenização do BERT gera mais tokens que a tokenização das palavras do spaCy
     _dic_excecao_maior = {"":-1,
                          }
                              
-    def _getExcecaoDicMaior(self, token):   
+    def _getExcecaoDicMaior(self, token: str):   
     
         valor = self._dic_excecao_maior.get(token)
         if valor != None:
             return valor
         else:
             return -1                             
     
     # Dicionário de tokens de exceções e seus deslocamentos para considerar menos tokens do BERT em relação ao spaCy
     # A tokenização do BERT gera menos tokens que a tokenização das palavras do spaCy
     _dic_excecao_menor = {"1°":1,
                           }
     
-    def _getExcecaoDicMenor(self, token):   
+    def _getExcecaoDicMenor(self, token: str):   
         
         valor = self._dic_excecao_menor.get(token)
         if valor != None:
             return valor
         else:
             return -1
 
@@ -413,25 +336,25 @@
         Utiliza duas estratégias para realizar o pooling de tokens que forma uma palavra.
             - Estratégia MEAN para calcular a média dos embeddings dos tokens que formam uma palavra.
             - Estratégia MAX para calcular o valor máximo dos embeddings dos tokens que formam uma palavra.
             
         Parâmetros:
         `texto` - Um texto a ser recuperado os embeddings das palavras do modelo de linguagem
     
-        Retorna 5 lista:            
+        Retorna um dicionário com 5 lista:            
             lista_tokens  uma lista com os tokens do texto gerados pelo método.
             texto_pos_pln uma lista com as postagging dos tokens gerados pela ferramenta de pln.
             lista_tokens_OOV_mcl uma lista com os tokens OOV do mcl.
             lista_embeddings_MEAN uma lista com os embeddings com a estratégia MEAN.
             lista_embeddings_MAX uma lista com os embeddings com a estratégia MAX.
         '''
        
         #Guarda os tokens e embeddings de retorno
         lista_tokens = []
-        lista_tokens_OOV_mcl = []
+        lista_tokens_oov_mcl = []
         lista_embeddings_MEAN = []
         lista_embeddings_MAX = []
         
         # Gera a tokenização e POS-Tagging da sentença    
         lista_tokens_texto_pln, lista_pos_texto_pln = pln.getListaTokensPOSTexto(tokens_texto_concatenado)
 
         # print("\tokens_texto_concatenado    :",tokens_texto_concatenado)    
@@ -474,15 +397,15 @@
             #print("Exceção pos:", pos)
                 
             if pos != -1 or pos2 != -1:      
                 if pos != -1:
                     #print("Adiciona 1 Exceção palavra == wi or palavra = [UNK]:",wi)
                     lista_tokens.append(wi)
                     # Marca como fora do vocabulário do MCL
-                    lista_tokens_OOV_mcl.append(1)
+                    lista_tokens_oov_mcl.append(1)
                     # Verifica se tem mais de um token
                     if pos != 1:
                         indice_token = pos_wj + pos
                         #print("Calcula a média de :", pos_wj , "até", indice_token)
                         embeddings_tokens_palavra = embeddings_texto[pos_wj:indice_token]
                         #print("embeddings_tokens_palavra:",embeddings_tokens_palavra.shape)
                         # calcular a média dos embeddings dos tokens do MCL da palavra
@@ -506,15 +429,15 @@
                     #print("wi[",pos_wi,"]=", texto_token[pos_wi])
                     #print("wj[",pos_wj,"]=", texto_tokenizada_MCL[pos_wj])
                 else:
                     if pos2 != -1:
                         #print("Adiciona 1 Exceção palavra == wi or palavra = [UNK]:",wi)
                         lista_tokens.append(wi+wi1)
                         # Marca como fora do vocabulário do MCL
-                        lista_tokens_OOV_mcl.append(1)
+                        lista_tokens_oov_mcl.append(1)
                         # Verifica se tem mais de um token
                         if pos2 == 1: 
                             # Adiciona o embedding do token a lista de embeddings
                             lista_embeddings_MEAN.append(embeddings_texto[pos_wj])
                             lista_embeddings_MAX.append(embeddings_texto[pos_wj])
               
                         # Avança para a próxima palavra e token do MCL
@@ -526,15 +449,15 @@
             else:  
                 # Tokens iguais adiciona a lista, o token não possui subtoken
                 if (wi == wj or wj=="[UNK]"):
                     # Adiciona o token a lista de tokens
                     #print("Adiciona 2 wi==wj or wj==[UNK]:", wi )
                     lista_tokens.append(wi)    
                     # Marca como dentro do vocabulário do MCL
-                    lista_tokens_OOV_mcl.append(0)
+                    lista_tokens_oov_mcl.append(0)
                     # Adiciona o embedding do token a lista de embeddings
                     lista_embeddings_MEAN.append(embeddings_texto[pos_wj])
                     lista_embeddings_MAX.append(embeddings_texto[pos_wj])
                     #print("embedding1[pos_wj]:", embedding_texto[pos_wj].shape)
                     # Avança para a próxima palavra e token do MCL
                     pos_wi = pos_wi + 1
                     pos_wj = pos_wj + 1   
@@ -558,15 +481,15 @@
 
                     #print("\nMontei palavra:",palavra_POS)
                     if (palavra_POS == wi or palavra_POS == "[UNK]"):
                         # Adiciona o token a lista
                         #print("Adiciona 3 palavra == wi or palavra_POS = [UNK]:",wi)
                         lista_tokens.append(wi)
                         # Marca como fora do vocabulário do MCL
-                        lista_tokens_OOV_mcl.append(1)
+                        lista_tokens_oov_mcl.append(1)
                         # Calcula a média dos tokens da palavra
                         #print("Calcula o máximo :", pos_wj , "até", indice_token)
                         embeddings_tokens_palavra = embeddings_texto[pos_wj:indice_token]
                         #print("embeddings_tokens_palavra2:",embeddings_tokens_palavra)
                         #print("embeddings_tokens_palavra2:",embeddings_tokens_palavra.shape)
                   
                         # calcular a média dos embeddings dos tokens do MCL da palavra
@@ -600,30 +523,32 @@
             logger.info("lista_embeddings_MAX       :{}.".format(lista_embeddings_MAX))
             logger.info("len(lista_embeddings_MAX)  :{}.".format(len(lista_embeddings_MAX)))
        
         del embeddings_texto
         del tokens_texto_mcl
         del lista_tokens_texto_pln
 
-        return lista_tokens, lista_pos_texto_pln, lista_tokens_OOV_mcl, lista_embeddings_MEAN, lista_embeddings_MAX
+        # Retorna as medidas em um dicionário
+        saida = {}
+        saida.update({'tokens_texto' : lista_tokens,
+                      'pos_texto_pln' : lista_pos_texto_pln,
+                      'tokens_oov_texto_mcl' : lista_tokens_oov_mcl,
+                      'embeddings_MEAN' : lista_embeddings_MEAN,
+                      'embeddings_MAX' : lista_embeddings_MAX})
+
+        #return lista_tokens, lista_pos_texto_pln, lista_tokens_OOV_mcl, lista_embeddings_MEAN, lista_embeddings_MAX
+        return saida
 
     # ============================   
-    def get_dimensao_embedding(self) -> int:
+    def getDimensaoEmbedding(self) -> int:
         '''
         Retorna a dimensão do embedding
         '''
         return self.auto_model.config.hidden_size        
         
-    # ============================           
-    def get_config_dict(self):
-        '''
-        Retorna as configurações com dicionário
-        '''
-        return {key: self.__dict__[key] for key in self.config_keys}
-
     # ============================   
     def save(self, output_path: str):
         '''
         Salva o modelo.
         '''
         self.auto_model.save_pretrained(output_path)
         self.tokenizer.save_pretrained(output_path)
```

### Comparing `texto_transformer-0.0.1/textotransformer/pln/pln.py` & `texto_transformer-0.0.2/textotransformer/pln/pln.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,30 @@
 
     # Construtor da classe
     def __init__(self, modelo_args):
     
         # Parâmetros do modelo
         self.modelo_args = modelo_args
         
-        #Instala o spaCy
+        #Instala a ferramenta pln spaCy
         InstaladorModelo(modelo_args=modelo_args)
         
         #Carrega o modelo do spacy
         self.carrega()
             
         logger.info("Classe PLN carregada: {}.".format(modelo_args))    
             
+    # ============================   
+    def __repr__(self):
+        '''
+        Retorna uma string com descrição do objeto
+        '''
+        return "Classe ({}) com modelo: {}".format(self.__class__.__name__,
+                                                   self.model_pln.__class__.__name__)            
+    
     # ============================    
     def carrega(self):
         '''
         Realiza o carregamento da ferramenta de PLN.
      
         '''
        
@@ -135,21 +143,21 @@
         `textoComRelevantesConcatenado` - Texto somente com as palavras relevantes.
         '''
       
         # Realiza o parsing no texto usando spacy
         doc = self.model_pln(texto)
 
         # Retorna a lista das palavras relevantes de um tipo
-        textoComRelevantes = [token.text for token in doc if token.pos_ == tipo_palavra_relevante]
+        texto_com_palavras_relevantes = [token.text for token in doc if token.pos_ == tipo_palavra_relevante]
 
         # Concatena o texto com as palavras relevantes
-        textoComRelevantesConcatenado = ' '.join(textoComRelevantes)
+        texto_com_palavras_relevantes_concatenado = ' '.join(texto_com_palavras_relevantes)
 
         # Retorna o texto
-        return textoComRelevantesConcatenado       
+        return texto_com_palavras_relevantes_concatenado       
        
     # ============================
     def getListaSentencasTexto(self, texto):
         '''
         Retorna uma lista com as sentenças de um texto. Utiliza o spacy para dividir o texto em sentenças.
         
         Parâmetros:
```

### Comparing `texto_transformer-0.0.1/textotransformer/util/utilarquivo.py` & `texto_transformer-0.0.2/textotransformer/util/utilarquivo.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         # Cria o diretório
         os.makedirs(DIRETORIO_MODELO_LINGUAGEM)
         logger.info("Diretório modelo de linguagem criado: {}".format(DIRETORIO_MODELO_LINGUAGEM))
     
     return DIRETORIO_MODELO_LINGUAGEM
 
 # ============================  
-def downloadArquivo(url_arquivo, nome_arquivo_destino):
+def downloadArquivo(url_arquivo: str, nome_arquivo_destino: str):
     '''    
     Realiza o download de um arquivo de uma url em salva em nome_arquivo_destino.
     
     Parâmetros:
     `url_arquivo` - URL do arquivo a ser feito download.      
     `nome_arquivo_destino` - Nome do arquivo a ser salvo.      
     '''
@@ -75,15 +75,15 @@
     # Renomeia o arquivo temporário para o arquivo definitivo
     os.rename(nome_arquivo_temporario, nome_arquivo_destino)
     
     # Fecha a barra de progresso.
     progresso_bar.close()
 
 # ============================      
-def carregar(nome_arquivo):
+def carregar(nome_arquivo: str):
     '''
     Carrega um arquivo texto e retorna as linhas como um único parágrafo(texto).
     
     Parâmetros:
     `nome_arquivo` - Nome do arquivo a ser carregado.           
     '''
         
@@ -102,15 +102,15 @@
     # Fecha o arquivo
     arquivo.close()
     
     # Remove os espaços em branco antes e depois do parágrafo
     return paragrafo.strip()
 
 # ============================  
-def carregarLista(nome_arquivo):
+def carregarLista(nome_arquivo: str):
     '''
     Carrega um arquivo texto e retorna as linhas como uma lista de sentenças(texto).
     
     Parâmetros:
     `nome_arquivo` - Nome do arquivo a ser carregado.           
     '''
 
@@ -127,19 +127,19 @@
             
     # Fecha o arquivo
     arquivo.close()
     
     return sentencas    
 
 # ============================      
-def salvar(nome_arquivo, texto):                       
+def salvar(nome_arquivo: str, texto: str):                       
     '''
     Salva um texto em um arquivo.
      
     Parâmetros:
     `nome_arquivo` - Nome do arquivo a ser salvo.     
     `texto` - Texto a ser salvo.     
      '''
 
     arquivo = open(nome_arquivo, 'w')
     arquivo.write(str(texto))
-    arquivo.close()     
+    arquivo.close()
```

### Comparing `texto_transformer-0.0.1/textotransformer/util/utilconstantes.py` & `texto_transformer-0.0.2/textotransformer/util/utilconstantes.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.1/textotransformer/util/utiltempo.py` & `texto_transformer-0.0.2/textotransformer/util/utiltempo.py`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.1/textotransformer/util/utiltexto.py` & `texto_transformer-0.0.2/textotransformer/util/utiltexto.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 import logging  
 # Biblioteca de expressão regular
 import re 
 # Biblioteca de codificação de caracteres
 import unicodedata 
 from collections import Counter
 from functools import reduce
+# Biblioteca de tipos
+from typing import List
 
 logger = logging.getLogger(__name__)
 
 # ============================  
-def convertTextoUtf8(texto):   
+def convertTextoUtf8(texto: str):   
     '''    
     Converte um texto para utf-8.
     
     Parâmetros:
    `texto` - Texto a ser convertido para utf-8.
 
     Retorno:
@@ -25,16 +27,17 @@
     
     try:
         texto = texto.encode('utf-8')
     except (TypeError, NameError): 
         pass
 
     return texto
+
 # ============================  
-def removeAcentos(texto):   
+def removeAcentos(texto: str):   
     '''    
     Remove acentos de um texto.
     
     Parâmetros:
    `texto` - Texto a ser removido os acentos.
 
     Retorno:
@@ -45,15 +48,15 @@
     texto = unicodedata.normalize('NFD', texto)
     texto = texto.encode('ascii', 'ignore')
     texto = texto.decode("utf-8")
     
     return str(texto)
 
 # ============================  
-def limpaTexto(texto):    
+def limpaTexto(texto: str):    
     '''    
     Remove acentos e espaços e outros caracteres de um texto.
     
     Parâmetros:
    `texto` - Texto a ser limpo.
     '''
     # Converte para minúsculo
@@ -62,28 +65,28 @@
     texto = re.sub('[ ]+', '_', texto)
     # Remove caracteres especiais
     texto = re.sub('[^.0-9a-zA-Z_-]', '', texto)
     
     return texto
     
 # ============================  
-def remove_tags(texto):
+def remove_tags(texto: str):
     '''
     Remove tags de um texto.
      
     Parâmetros:
     `texto` - Texto com tags a serem removidas.      
     '''
      
     textoLimpo = re.compile('<.*?>')
      
     return re.sub(textoLimpo, '', texto)
 
 # ============================
-def encontrarIndiceSubLista(lista, sublista):
+def encontrarIndiceSubLista(lista: List, sublista: List):
     '''
     Localiza os índices de início e fim de uma sublista em uma lista.
     
     Parâmetros:
     `lista` - Uma lista.
     `sublista` - Uma sublista a ser localizada na lista.
     '''
@@ -102,15 +105,15 @@
             indiceInicio = i - n + 1
             indiceFim = indiceInicio + len(sublista)-1
             return indiceInicio, indiceFim
         
     return -1, -1
     
 # ============================
-def getTextoLista(listaSentencas):
+def getTextoLista(listaSentencas: List):
     '''
     Recebe uma lista de sentenças e faz a concatenação em uma string.
     
     Parâmetros:
     `listaTexto` - Uma lista contendo diversas sentenças.           
     '''
 
@@ -121,28 +124,28 @@
 
 # ============================   
 def atualizaValor(a,b):
     a.update(b)
     return a
 
 # ============================   
-def getSomaDic(lista):
+def getSomaDic(lista: List):
     '''
     Soma os valores de dicionários com as mesmas chaves.
     
     Parâmetros:
     `lista` - Uma lista contendo dicionários.           
     '''
     
     # Soma os dicionários da lista
     novodic = reduce(atualizaValor, (Counter(dict(x)) for x in lista))
  
     return novodic
 
-def limpeza(texto):
+def limpeza(texto: str):
     '''
     Realiza limpeza dos dados.
         
     Parâmetros:
     `texto` - Um texto a ser limpo.      
 
     Retorno:
```

### Comparing `texto_transformer-0.0.1/LICENSE` & `texto_transformer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `texto_transformer-0.0.1/pyproject.toml` & `texto_transformer-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "texto-transformer"
-version = "0.0.1"
-description = "Texto Transformer: Framework multilingual para processamento de textos utilizando modelos de linguagem baseados baseados em Transformer"
+version = "0.0.2"
+description = "Texto Transformer: Framework para processamento de textos utilizando modelos de linguagem baseados baseados em Transformer"
 readme = "README.md"
 requires-python = ">=3.6.0"
 license = { file = "LICENSE" }
 
 authors = [
     { name = "Osmar de Oliveira Braz Junior", email = "osmar.braz@udesc.br" }
 ]
```

