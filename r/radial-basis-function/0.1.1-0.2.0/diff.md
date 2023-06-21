# Comparing `tmp/radial_basis_function-0.1.1.tar.gz` & `tmp/radial_basis_function-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radial_basis_function-0.1.1.tar", max compression
+gzip compressed data, was "radial_basis_function-0.2.0.tar", max compression
```

## Comparing `radial_basis_function-0.1.1.tar` & `radial_basis_function-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      605 2023-06-13 09:16:03.814602 radial_basis_function-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      142 2023-06-13 09:16:08.875203 radial_basis_function-0.1.1/radial_basis_function/__init__.py
--rw-r--r--   0        0        0     1652 2023-06-13 05:31:49.224159 radial_basis_function-0.1.1/radial_basis_function/pseudo_inversa.py
--rw-r--r--   0        0        0     5368 2023-06-13 09:02:03.281223 radial_basis_function-0.1.1/radial_basis_function/rbf.py
--rw-r--r--   0        0        0       46 2023-06-13 06:44:22.333854 radial_basis_function-0.1.1/README.md
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 radial_basis_function-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-06-21 04:30:39.171530 radial_basis_function-0.2.0/LICENSE
+-rw-r--r--   0        0        0      940 2023-06-21 04:49:28.209051 radial_basis_function-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-06-21 04:49:16.483812 radial_basis_function-0.2.0/radial_basis_function/__init__.py
+-rw-r--r--   0        0        0     1952 2023-06-21 04:14:33.497639 radial_basis_function-0.2.0/radial_basis_function/pseudo_inversa.py
+-rw-r--r--   0        0        0     6396 2023-06-21 04:16:11.508336 radial_basis_function-0.2.0/radial_basis_function/rbf.py
+-rw-r--r--   0        0        0     2781 2023-06-21 05:26:54.329205 radial_basis_function-0.2.0/README.md
+-rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 radial_basis_function-0.2.0/PKG-INFO
```

### Comparing `radial_basis_function-0.1.1/pyproject.toml` & `radial_basis_function-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 [tool.poetry]
 name = "radial-basis-function"
-version = "0.1.1"
+version = "0.2.0"
 description = "Radial Basis Function e Multiplicação de Matriz Pseudo-Inversa, para modelos de Regressão e Multi-Classificatórios."
 authors = ["Victor Venites <contato@victorvenites.com>"]
+maintainers = ["Victor Venites <contato@victorvenites.com>"]
+license = "MIT"
 readme = "README.md"
 packages = [{include = "radial_basis_function"}]
+homepage = "https://github.com/VictorVenites/Radial-Basis-Function"
+documentation = "https://github.com/VictorVenites/Radial-Basis-Function"
+keywords = ["rbf", "Radial Basis Function", "Pseudo-Inverse Matrix", "Matriz Pseudo-Inversa", "Victor Venites"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.2"
 numpy = "^1.24.3"
```

### Comparing `radial_basis_function-0.1.1/radial_basis_function/pseudo_inversa.py` & `radial_basis_function-0.2.0/radial_basis_function/pseudo_inversa.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,49 +2,57 @@
 Classe e métodos para implementar a Regressão por multiplicação de Matriz Pseudo-Inversa.
 
 Original Author: Victor Venites
 """
 
 import numpy as np
 import pandas as pd
+import time
 
 class PseudoInversa:
     """Multiplicacao de Matriz Pseudo-Inversa
     Original Author: Victor Venites
     """
     def __init__(self, bias = 1):
         self.weights = None
         self.bias = bias
         self.feature_names_in_ = None
         self.n_feature_in_ = None
+        self.n_linhas_in_ = None
+        self.time = None
 
     def fit(self, X, y):
         try:
             self.feature_names_in_ = X.columns
             self.n_feature_in_ = X.shape[1]
+            self.n_linhas_in_ = X.shape[0]
         except:
             self.n_feature_in_ = len(X[0])
+            self.n_linhas_in_ = len(X)
         Matriz_X = pd.DataFrame(X)
         if self.bias != 0:
             Matriz_X["Bias_Vies_Intercept"] = self.bias
+        tempo_Inicial = time.time()
         # Base_T * Base
         Matriz_Quadrada = np.dot(Matriz_X.T, Matriz_X)
         # Matriz Inversa
         try:
             Matriz_Inversa = np.linalg.inv(Matriz_Quadrada)
         except np.linalg.LinAlgError as err:
             if 'Singular matrix' in str(err):
                 Matriz_Regulada = Matriz_Quadrada + np.identity(len(Matriz_Quadrada))
                 Matriz_Inversa = np.linalg.inv(Matriz_Regulada)
         # Inversa * Base_Dados_T
         Matriz_Pseudo_Inversa = pd.DataFrame(np.dot(Matriz_Inversa, Matriz_X.T))
         # Isola o peso final
         self.weights = np.dot(Matriz_Pseudo_Inversa, y)
+        self.time = time.time() - tempo_Inicial
 
     def predict(self, X):
         Matriz_X = pd.DataFrame(X)
         if self.bias != 0:
             Matriz_X["Bias_Vies_Intercept"] = self.bias
         return np.dot(Matriz_X, self.weights)
 
     def score(self, x, y):
+        # TODO: adicionar métricas do próprio Sklearn
         pass
```

### Comparing `radial_basis_function-0.1.1/radial_basis_function/rbf.py` & `radial_basis_function-0.2.0/radial_basis_function/rbf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Classe e métodos para implementar a Regressão por Radial Basis Function
 
 Original Author: Victor Venites
 """
 
+# Dependencias internas á Biblioteca
+from .pseudo_inversa import PseudoInversa
+# Dependencias Externas
 import numpy as np
 import pandas as pd
-from .pseudo_inversa import PseudoInversa
+import time
 
 
 class RadialBasisFunction:
     """Radial Basis Function
     Original Author: Victor Venites
     """
     def __init__(self, funcao = 'Gaussiana',
@@ -20,21 +23,28 @@
         self.Polos_iniciais_fixos = Polos_iniciais_fixos
         self.C = Polos_Otimizados
         self.sigma = None
         self.pesos = None
         self.R = None
         self.feature_names_in_ = None
         self.n_feature_in_ = None
+        self.n_linhas_in_ = None
+        self.time = None
         
     # # # Funções Base
     def FuncoesBase(self, t, n_PoloAtual, N_TotalPolos, X, C):
-        Gama = 1 / (2 * self.sigma ** 2)
+        # TODO: revisar as funções, para se aproximarem do original de inspiração
+        Gama = 1 / (2 * self.sigma ** 2) # Por Convensão
         Radial = np.linalg.norm(X - C)
+        #Radial = (np.linalg.norm(X - C)) ** 2 # 
         if self.funcao == "Gaussiana":
             calculo = np.exp(-Gama * (Radial ** 2))
+            #calculo = np.exp(- Gama * Radial)
+        #elif funcao == "Multiquadratica":
+        #    calculo = np.sqrt(Radial + (1 / Gama) ** 2)
         elif self.funcao == "Sigmoide":
             calculo = np.tanh(-Gama * (Radial ** 2))
         elif self.funcao == "Senoidal":
             calculo = np.sin(-Gama * (Radial ** 2))
         elif self.funcao == "Logistica":
             calculo = 1 / (1 + np.exp(Gama * (Radial**2)))
         elif self.funcao == "ReLu":
@@ -64,25 +74,31 @@
             num_de_polos = 2
         elif num_de_variaveis > 2:
             num_de_polos = num_de_variaveis
         if self.Qtd_Polos > 1:
             num_de_polos = self.Qtd_Polos
         if self.Qtd_Polos > num_de_licoes:
             num_de_polos = num_de_licoes - 2
-        if self.Qtd_Polos > num_de_variaveis * 10:
-            num_de_polos = int(round(self.Qtd_Polos / 2 + 2))
+        if self.Qtd_Polos > num_de_variaveis * 8:
+            # TODO: Avaliar uma bordagem melhor para evitar Overfitting
+            num_de_polos = int(round((self.Qtd_Polos + num_de_variaveis * 8) / 9 + 2))
+        if num_de_polos > num_de_licoes:
+            #num_de_polos = num_de_licoes - 2
+            num_de_polos = num_de_licoes
 
-        # Gerando os Polos(Ex: Centróides do K-means)
+        # Gerando os Polos Aleatórios
+        # TODO: Centróides do K-means, ou gerados por Algoritmo Genéticos)
         C = np.zeros((num_de_polos, num_de_variaveis), dtype = float)
         C = np.random.rand(num_de_polos, num_de_variaveis)
         # Limite por Coluna (apenas entre as escalas de cada coluna)
         Limite = np.array(variaveis.max() - variaveis.min())
         C = pd.DataFrame(C) * Limite + np.array(variaveis.min())
         C = np.array(C)
         
+        # TODO: Criar Função específica para geração dos Polos
         #if self.C is not None:
 
         dist_entre_os_polos = np.zeros((num_de_polos, num_de_polos))
         for i in range(0, num_de_polos, 1):
             for j in range(0, num_de_polos, 1):
                 dist_entre_os_polos[i, j] = np.linalg.norm(C[i] - C[j])
         if self.Polos_iniciais_fixos:
@@ -110,20 +126,24 @@
         self.R = pd.DataFrame(R)
         self.C = C
 
     def fit(self, X, Matriz_Y):
         try:
             self.feature_names_in_ = X.columns
             self.n_feature_in_ = X.shape[1]
+            self.n_linhas_in_ = X.shape[0]
         except:
             self.n_feature_in_ = len(X[0])
+            self.n_linhas_in_ = len(X)
+        tempo_Inicial = time.time()
         self.Radial(X)
         Matriz_Pseudo_Inversa = PseudoInversa()
         Matriz_Pseudo_Inversa.fit(np.array(self.R), Matriz_Y)
         self.pesos = Matriz_Pseudo_Inversa.weights
+        self.time = time.time() - tempo_Inicial
 
     def predict(self, X):
         #A = np.dot(variaveis_X, W) # Valores finais da predição
         variaveis_X = np.array(X)
         Predicao_Y = np.zeros(len(variaveis_X))
         W = [i for i in self.pesos]
         C = self.C
@@ -134,9 +154,10 @@
             for j in range(0, len(W) - 1, 1):
                 # Somatorio + Pesos * Funcoes_Ativa
                 Predicao_Y[i] = Predicao_Y[i] + W[j] * self.FuncoesBase(i, (i+1), len(C), variaveis_X[i], C[j])
 
         return Predicao_Y
 
     def score(self, x, y):
+        # TODO: adicionar métricas do próprio Sklearn
         pass
```

