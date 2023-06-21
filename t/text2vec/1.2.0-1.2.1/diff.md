# Comparing `tmp/text2vec-1.2.0.tar.gz` & `tmp/text2vec-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2vec-1.2.0.tar", last modified: Fri Jun 16 14:37:05 2023, max compression
+gzip compressed data, was "text2vec-1.2.1.tar", last modified: Wed Jun 21 03:03:37 2023, max compression
```

## Comparing `text2vec-1.2.0.tar` & `text2vec-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-16 14:37:05.368094 text2vec-1.2.0/
--rw-r--r--   0 xuming     (501) staff       (20)    45156 2023-06-16 14:37:05.367656 text2vec-1.2.0/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    38244 2023-06-16 09:11:18.000000 text2vec-1.2.0/README.md
--rw-r--r--   0 xuming     (501) staff       (20)       38 2023-06-16 14:37:05.368214 text2vec-1.2.0/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1606 2023-06-14 08:11:02.000000 text2vec-1.2.0/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-16 14:37:05.354938 text2vec-1.2.0/text2vec/
--rw-r--r--   0 xuming     (501) staff       (20)     1221 2023-06-14 14:22:28.000000 text2vec-1.2.0/text2vec/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3715 2023-06-14 14:12:57.000000 text2vec-1.2.0/text2vec/bertmatching_dataset.py
--rw-r--r--   0 xuming     (501) staff       (20)    18322 2023-06-15 02:51:06.000000 text2vec-1.2.0/text2vec/bertmatching_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     1803 2023-06-14 08:11:02.000000 text2vec-1.2.0/text2vec/bm25.py
--rw-r--r--   0 xuming     (501) staff       (20)     3373 2023-06-14 14:12:57.000000 text2vec-1.2.0/text2vec/cosent_dataset.py
--rw-r--r--   0 xuming     (501) staff       (20)    13840 2023-06-15 02:51:06.000000 text2vec-1.2.0/text2vec/cosent_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     3252 2023-06-14 12:45:18.000000 text2vec-1.2.0/text2vec/ngram.py
--rw-r--r--   0 xuming     (501) staff       (20)    12378 2023-06-14 13:56:03.000000 text2vec-1.2.0/text2vec/sentence_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    14566 2023-06-15 02:51:06.000000 text2vec-1.2.0/text2vec/sentencebert_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     9658 2023-06-13 06:16:05.000000 text2vec-1.2.0/text2vec/similarity.py
--rw-r--r--   0 xuming     (501) staff       (20)     9136 2021-09-11 10:12:24.000000 text2vec-1.2.0/text2vec/stopwords.txt
--rw-r--r--   0 xuming     (501) staff       (20)     6358 2023-06-14 14:12:57.000000 text2vec-1.2.0/text2vec/text_matching_dataset.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-16 14:37:05.366204 text2vec-1.2.0/text2vec/utils/
--rw-r--r--   0 xuming     (501) staff       (20)        0 2021-09-11 10:12:24.000000 text2vec-1.2.0/text2vec/utils/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     6413 2022-01-21 13:50:54.000000 text2vec-1.2.0/text2vec/utils/distance.py
--rw-r--r--   0 xuming     (501) staff       (20)    15066 2022-03-11 08:18:40.000000 text2vec-1.2.0/text2vec/utils/get_file.py
--rw-r--r--   0 xuming     (501) staff       (20)     1595 2023-06-14 13:27:05.000000 text2vec-1.2.0/text2vec/utils/io_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     5630 2022-02-13 15:54:49.000000 text2vec-1.2.0/text2vec/utils/rank_bm25.py
--rw-r--r--   0 xuming     (501) staff       (20)      859 2022-02-25 17:04:46.000000 text2vec-1.2.0/text2vec/utils/stats_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     1916 2022-01-23 04:13:14.000000 text2vec-1.2.0/text2vec/utils/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)       84 2023-06-14 08:11:02.000000 text2vec-1.2.0/text2vec/version.py
--rw-r--r--   0 xuming     (501) staff       (20)     6180 2023-06-14 12:45:19.000000 text2vec-1.2.0/text2vec/word2vec.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-16 14:37:05.359066 text2vec-1.2.0/text2vec.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    45156 2023-06-16 14:37:04.000000 text2vec-1.2.0/text2vec.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)      751 2023-06-16 14:37:05.000000 text2vec-1.2.0/text2vec.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-06-16 14:37:04.000000 text2vec-1.2.0/text2vec.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2022-05-17 02:41:49.000000 text2vec-1.2.0/text2vec.egg-info/not-zip-safe
--rw-r--r--   0 xuming     (501) staff       (20)       74 2023-06-16 14:37:04.000000 text2vec-1.2.0/text2vec.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        9 2023-06-16 14:37:04.000000 text2vec-1.2.0/text2vec.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-21 03:03:37.425662 text2vec-1.2.1/
+-rw-r--r--   0 xuming     (501) staff       (20)    49036 2023-06-21 03:03:37.425133 text2vec-1.2.1/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    42020 2023-06-21 02:19:56.000000 text2vec-1.2.1/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)       38 2023-06-21 03:03:37.425895 text2vec-1.2.1/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1606 2023-06-14 08:11:02.000000 text2vec-1.2.1/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-21 03:03:37.386479 text2vec-1.2.1/text2vec/
+-rw-r--r--   0 xuming     (501) staff       (20)     1221 2023-06-14 14:22:28.000000 text2vec-1.2.1/text2vec/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3715 2023-06-14 14:12:57.000000 text2vec-1.2.1/text2vec/bertmatching_dataset.py
+-rw-r--r--   0 xuming     (501) staff       (20)    18322 2023-06-15 02:51:06.000000 text2vec-1.2.1/text2vec/bertmatching_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1803 2023-06-14 08:11:02.000000 text2vec-1.2.1/text2vec/bm25.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3377 2023-06-18 04:55:14.000000 text2vec-1.2.1/text2vec/cosent_dataset.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13840 2023-06-15 02:51:06.000000 text2vec-1.2.1/text2vec/cosent_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3252 2023-06-14 12:45:18.000000 text2vec-1.2.1/text2vec/ngram.py
+-rw-r--r--   0 xuming     (501) staff       (20)    12378 2023-06-20 03:07:55.000000 text2vec-1.2.1/text2vec/sentence_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    14566 2023-06-15 02:51:06.000000 text2vec-1.2.1/text2vec/sentencebert_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9813 2023-06-20 03:12:38.000000 text2vec-1.2.1/text2vec/similarity.py
+-rw-r--r--   0 xuming     (501) staff       (20)     9136 2021-09-11 10:12:24.000000 text2vec-1.2.1/text2vec/stopwords.txt
+-rw-r--r--   0 xuming     (501) staff       (20)     6358 2023-06-18 04:53:18.000000 text2vec-1.2.1/text2vec/text_matching_dataset.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-21 03:03:37.421648 text2vec-1.2.1/text2vec/utils/
+-rw-r--r--   0 xuming     (501) staff       (20)        0 2021-09-11 10:12:24.000000 text2vec-1.2.1/text2vec/utils/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6413 2022-01-21 13:50:54.000000 text2vec-1.2.1/text2vec/utils/distance.py
+-rw-r--r--   0 xuming     (501) staff       (20)    15066 2022-03-11 08:18:40.000000 text2vec-1.2.1/text2vec/utils/get_file.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1595 2023-06-14 13:27:05.000000 text2vec-1.2.1/text2vec/utils/io_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5630 2022-02-13 15:54:49.000000 text2vec-1.2.1/text2vec/utils/rank_bm25.py
+-rw-r--r--   0 xuming     (501) staff       (20)      859 2022-02-25 17:04:46.000000 text2vec-1.2.1/text2vec/utils/stats_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1916 2022-01-23 04:13:14.000000 text2vec-1.2.1/text2vec/utils/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)       84 2023-06-21 03:03:19.000000 text2vec-1.2.1/text2vec/version.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6180 2023-06-14 12:45:19.000000 text2vec-1.2.1/text2vec/word2vec.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-21 03:03:37.413588 text2vec-1.2.1/text2vec.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    49036 2023-06-21 03:03:37.000000 text2vec-1.2.1/text2vec.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)      751 2023-06-21 03:03:37.000000 text2vec-1.2.1/text2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-06-21 03:03:37.000000 text2vec-1.2.1/text2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2022-05-17 02:41:49.000000 text2vec-1.2.1/text2vec.egg-info/not-zip-safe
+-rw-r--r--   0 xuming     (501) staff       (20)       74 2023-06-21 03:03:37.000000 text2vec-1.2.1/text2vec.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        9 2023-06-21 03:03:37.000000 text2vec-1.2.1/text2vec.egg-info/top_level.txt
```

### Comparing `text2vec-1.2.0/PKG-INFO` & `text2vec-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2vec
-Version: 1.2.0
+Version: 1.2.1
 Summary: Text to vector Tool, encode text
 Home-page: https://github.com/shibing624/text2vec
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache License 2.0
 Description: [**🇨🇳中文**](https://github.com/shibing624/text2vec/blob/master/README.md) | [**🌐English**](https://github.com/shibing624/text2vec/blob/master/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/text2vec/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624) 
         
@@ -27,14 +27,16 @@
         
         
         **Text2vec**: Text to Vector, Get Sentence Embeddings. 文本向量化，把文本(包括词、句子、段落)表征为向量矩阵。
         
         **text2vec**实现了Word2Vec、RankBM25、BERT、Sentence-BERT、CoSENT等多种文本表征、文本相似度计算模型，并在文本语义匹配（相似度计算）任务上比较了各模型的效果。
         
         ### News
+        [2023/06/19] v1.2.1版本: 更新了中文匹配模型`shibing624/text2vec-base-chinese-nli`为新版[shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)，针对CoSENT的loss计算对排序敏感特点，人工挑选并整理出高质量的有相关性排序的STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)，在各评估集表现相对之前有提升；发布了适用于s2p的中文匹配模型[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)，详见[Release-v1.2.1](https://github.com/shibing624/text2vec/releases/tag/1.2.1)
+        
         [2023/06/15] v1.2.0版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)，基于`nghuyong/ernie-3.0-base-zh`模型，使用了中文NLI数据集[shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)全部语料训练的CoSENT文本匹配模型，在各评估集表现提升明显，详见[Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
         
         [2022/03/12] v1.1.4版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，基于中文STS训练集训练的CoSENT匹配模型。详见[Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
         
         
         **Guide**
         - [Feature](#Feature)
@@ -50,63 +52,72 @@
         - [Word2Vec](https://github.com/shibing624/text2vec/blob/master/text2vec/word2vec.py)：通过腾讯AI Lab开源的大规模高质量中文[词向量数据（800万中文词轻量版）](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) (文件名：light_Tencent_AILab_ChineseEmbedding.bin 密码: tawe）实现词向量检索，本项目实现了句子（词向量求平均）的word2vec向量表示
         - [SBERT(Sentence-BERT)](https://github.com/shibing624/text2vec/blob/master/text2vec/sentencebert_model.py)：权衡性能和效率的句向量表示模型，训练时通过有监督训练上层分类函数，文本匹配预测时直接句子向量做余弦，本项目基于PyTorch复现了Sentence-BERT模型的训练和预测
         - [CoSENT(Cosine Sentence)](https://github.com/shibing624/text2vec/blob/master/text2vec/cosent_model.py)：CoSENT模型提出了一种排序的损失函数，使训练过程更贴近预测，模型收敛速度和效果比Sentence-BERT更好，本项目基于PyTorch实现了CoSENT模型的训练和预测
         
         详细文本向量表示方法见wiki: [文本向量表示方法](https://github.com/shibing624/text2vec/wiki/%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95)
         # Evaluation
         
-        ### 文本匹配
+        文本匹配
+        
+        #### 英文匹配数据集的评测结果：
+        
         
-        - 英文匹配数据集的评测结果：
+        | Arch   | BaseModel                                        | Model                            | English-STS-B | 
+        |:-------|:------------------------------------------------|:-------------------------------------|:-------------:|
+        | GloVe  | glove                                           | Avg_word_embeddings_glove_6B_300d    |     61.77     |
+        | BERT   | bert-base-uncased                               | BERT-base-cls                        |     20.29     |
+        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg             |     59.04     |
+        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg-whiten(NLI) |     63.65     |
+        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls                   |     73.65     |
+        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg        |     77.96     |
+        | CoSENT | bert-base-uncased                               | CoSENT-base-first_last_avg           |     69.93     |
+        | CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg       |     79.68     |
+        
+        #### 中文匹配数据集的评测结果：
+        
+        
+        | Arch   | BaseModel                    | Model           | ATEC  |  BQ   | LCQMC | PAWSX | STS-B |  Avg  | 
+        |:-------|:----------------------------|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
+        | SBERT  | bert-base-chinese           | SBERT-bert-base     | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74 |
+        | SBERT  | hfl/chinese-macbert-base    | SBERT-macbert-base  | 47.28 | 68.63 | 79.42 | 55.59 | 64.82 | 63.15 |
+        | SBERT  | hfl/chinese-roberta-wwm-ext | SBERT-roberta-ext   | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 |
+        | CoSENT | bert-base-chinese           | CoSENT-bert-base    | 49.74 | 72.38 | 78.69 | 60.00 | 79.27 | 68.01 |
+        | CoSENT | hfl/chinese-macbert-base    | CoSENT-macbert-base | 50.39 | 72.93 | 79.17 | 60.86 | 79.30 | 68.53 |
+        | CoSENT | hfl/chinese-roberta-wwm-ext | CoSENT-roberta-ext  | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
+        
+        说明：
+        - 结果评测指标：spearman系数
+        - 为评测模型能力，结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
         
-        | Arch | Backbone | Model  | English-STS-B | 
-        | :-- | :--- | :--- | :-: |
-        | GloVe | glove | Avg_word_embeddings_glove_6B_300d | 61.77 |
-        | BERT | bert-base-uncased | BERT-base-cls | 20.29 |
-        | BERT | bert-base-uncased | BERT-base-first_last_avg | 59.04 |
-        | BERT | bert-base-uncased | BERT-base-first_last_avg-whiten(NLI) | 63.65 |
-        | SBERT | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls | 73.65 |
-        | SBERT | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg | 77.96 |
-        | SBERT | xlm-roberta-base | paraphrase-multilingual-MiniLM-L12-v2 | 84.42 |
-        | CoSENT | bert-base-uncased | CoSENT-base-first_last_avg | 69.93 |
-        | CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68 |
-        
-        - 中文匹配数据集的评测结果：
-        
-        | Arch | Backbone | Model  | ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | QPS |
-        | :-- | :--- | :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
-        | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 | **72.93** | **79.17** | **60.86** | **80.51** | **68.77**  | 3008 |
-        | CoSENT | Langboat/mengzi-bert-base | CoSENT-mengzi-base | **50.52** | 72.27 | 78.69 | 12.89 | 80.15 | 58.90 | 2502 |
-        | CoSENT | bert-base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 80.14 | 68.19 | 2653 |
-        | SBERT | bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74 | 3365 |
-        | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28 | 68.63 | **79.42** | 55.59 | 64.82 | 63.15 | 2948 |
-        | CoSENT | hfl/chinese-roberta-wwm-ext | CoSENT-roberta-ext | **50.81** | **71.45** | **79.31** | **61.56** | **81.13** | **68.85** | - |
-        | SBERT | hfl/chinese-roberta-wwm-ext | SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | - |
         
+        ### Release Models
         - 本项目release模型的中文匹配评测结果：
         
-        | Arch | BaseModel                    | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B |    Avg    |  QPS  |
-        | :-- |:-----------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:---------:|:-----:|
-        | Word2Vec | word2vec                     | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |   33.86   | 23769 |
-        | SBERT | xlm-roberta-base             | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |   41.99   | 3138  |
-        | CoSENT | hfl/chinese-macbert-base     | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | 48.25 | 3008  |
-        | CoSENT | hfl/chinese-lert-large       | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |   48.08   | 2092  |
-        | CoSENT | nghuyong/ernie-3.0-base-zh   | [shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)                                               | 51.26 | 68.72 | 79.13 | 34.28 | 80.70 |   **62.81**   | 3066  |
+        | Arch       | BaseModel                         | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc |    Avg    |  QPS  |
+        |:-----------|:----------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:|
+        | Word2Vec   | word2vec                          | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |  55.04  |  20.70  |   35.03   | 23769 |
+        | SBERT      | xlm-roberta-base                  | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |  63.01  |  52.28  |   46.46   | 3138  |
+        | Instructor | hfl/chinese-roberta-wwm-ext       | [moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base)                                                                                       | 41.27 | 63.81 | 74.87 | 12.20 | 76.96 |  75.83  |  60.55  |   57.93   | 2980  |
+        | CoSENT     | hfl/chinese-macbert-base          | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |  70.27  |  50.42  |   51.61   | 3008  |
+        | CoSENT     | hfl/chinese-lert-large            | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |  73.01  |  59.04  |   53.12   | 2092  |
+        | CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)                                     | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 |  70.60  |  53.08  |   59.87   | 3089  |
+        | CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)                                 | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 |  76.70  |  63.30  | **63.08** | 3066  |
         
         
         说明：
-        - 结果值是spearman系数
-        - 结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
-        - `shibing624/text2vec-base-chinese`模型，是用CoSENT方法训练，基于`hfl/chinese-macbert-base`在中文STS-B数据训练得到，并在中文STS-B测试集评估达到较好效果，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，中文通用语义匹配任务推荐使用
-        - `shibing624/text2vec-base-chinese-nli`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用中文NLI数据集[shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)全部语料训练得到，并在中文各NLI测试集评估达到SOTA，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)，中文s2s(句子vs句子)语义匹配任务推荐使用
+        - 结果评测指标：spearman系数
+        - 模型训练实验报告：[实验报告](https://github.com/shibing624/text2vec/blob/master/docs/model_report.md)
+        - `shibing624/text2vec-base-chinese`模型，是用CoSENT方法训练，基于`hfl/chinese-macbert-base`在中文STS-B数据训练得到，并在中文STS-B测试集评估达到较好效果，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传HF model hub，中文通用语义匹配任务推荐使用
+        - `shibing624/text2vec-base-chinese-sentence`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)训练得到，并在中文各NLI测试集评估达到较好效果，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2s(句子vs句子)语义匹配任务推荐使用
+        - `shibing624/text2vec-base-chinese-paraphrase`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-paraphrase-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-paraphrase-dataset)，数据集相对于[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)加入了s2p(sentence to paraphrase)数据，强化了其长文本的表征能力，并在中文各NLI测试集评估达到SOTA，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2p(句子vs段落)语义匹配任务推荐使用
         - `SBERT-macbert-base`模型，是用SBERT方法训练，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型
         - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
         - `w2v-light-tencent-chinese`是腾讯词向量的Word2Vec模型，CPU加载使用，适用于中文字面匹配任务和缺少数据的冷启动情况
         - 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base` 或者roberta模型：`--model_name uer/roberta-medium-wwm-chinese-cluecorpussmall`
-        - 中文匹配数据集下载[链接见下方](#数据集)
+        - 为测评模型的鲁棒性，加入了未训练过的SOHU测试集，用于测试模型的泛化能力；为达到开箱即用的实用效果，使用了搜集到的各中文匹配数据集，数据集也上传到HF datasets[链接见下方](#数据集)
         - 中文匹配任务实验表明，pooling最优是`EncoderType.FIRST_LAST_AVG`和`EncoderType.MEAN`，两者预测效果差异很小
         - 中文匹配评测结果复现，可以下载中文匹配数据集到`examples/data`，运行[tests/test_model_spearman.py](https://github.com/shibing624/text2vec/blob/master/tests/test_model_spearman.py)代码复现评测结果
         - QPS的GPU测试环境是Tesla V100，显存32GB
         
         # Demo
         
         Official Demo: https://www.mulanai.com/product/short_text_sim/
@@ -651,24 +662,25 @@
         ```
         
         
         ## 数据集
         
         - 本项目release的数据集：
         
-        | Dataset               | Introduce                                                           | Download Link                                                                                                                                                                                                                                                                                         |
-        |:----------------------|:--------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | shibing624/nli-zh-all | 中文语义匹配数据合集，整合了文本推理，相似，摘要，问答，指令微调等任务的820万高质量数据，并转化为匹配格式数据集           | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://huggingface.co/datasets/shibing624/nli-zh-all)                                                                                                                                                                                        |
-        | shibing624/snli-zh    | 中文SNLI和MultiNLI数据集，翻译自英文SNLI和MultiNLI                                       | [https://huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/shibing624/snli-zh)                                                                                                                                                                                              |
-        | shibing624/nli_zh     | 中文语义匹配数据集，整合了中文ATEC、BQ、LCQMC、PAWSX、STS-B共5个任务的数据集                   | [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh) </br> or </br> [百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ) </br> or </br> [github](https://github.com/shibing624/text2vec/releases/download/1.1.2/senteval_cn.zip) </br> |
-        | ATEC                  | 中文ATEC数据集，蚂蚁金服Q-Qpair数据集                                            | [ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)                                                                                                                                                                                                                                 |
-        | BQ                    | 中文BQ(Bank Question)数据集，银行Q-Qpair数据集                                 | [BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)                                                                                                                                                                                                                                                     |
-        | LCQMC                 | 中文LCQMC(large-scale Chinese question matching corpus)数据集，Q-Qpair数据集 | [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)                                                                                                                                                                                                                                               |
-        | PAWSX                 | 中文PAWS(Paraphrase Adversaries from Word Scrambling)数据集，Q-Qpair数据集   | [PAWSX](https://arxiv.org/abs/1908.11828)                                                                                                                                                                                                                                                             |
-        | STS-B                 | 中文STS-B数据集，中文自然语言推理数据集，从英文STS-B翻译为中文的数据集                            | [STS-B](https://github.com/pluto-junzeng/CNSD)                                                                                                                                                                                                                                                        |
+        | Dataset                    | Introduce                                                                | Download Link                                                                                                                                                                                                                                                                                         |
+        |:---------------------------|:-------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+        | shibing624/nli-zh-all      | 中文语义匹配数据合集，整合了文本推理，相似，摘要，问答，指令微调等任务的820万高质量数据，并转化为匹配格式数据集                | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://huggingface.co/datasets/shibing624/nli-zh-all)                                                                                                                                                                                        |
+        | shibing624/snli-zh         | 中文SNLI和MultiNLI数据集，翻译自英文SNLI和MultiNLI                                    | [https://huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/shibing624/snli-zh)                                                                                                                                                                                              |
+        | shibing624/nli_zh          | 中文语义匹配数据集，整合了中文ATEC、BQ、LCQMC、PAWSX、STS-B共5个任务的数据集                        | [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh) </br> or </br> [百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ) </br> or </br> [github](https://github.com/shibing624/text2vec/releases/download/1.1.2/senteval_cn.zip) </br> |
+        | shibing624/sts-sohu2021    | 中文语义匹配数据集，2021搜狐校园文本匹配算法大赛数据集                                            | [https://huggingface.co/datasets/shibing624/sts-sohu2021](https://huggingface.co/datasets/shibing624/sts-sohu2021)                                                                                                                                                                                    |
+        | ATEC                       | 中文ATEC数据集，蚂蚁金服Q-Qpair数据集                                                 | [ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)                                                                                                                                                                                                                                 |
+        | BQ                         | 中文BQ(Bank Question)数据集，银行Q-Qpair数据集                                      | [BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)                                                                                                                                                                                                                                                     |
+        | LCQMC                      | 中文LCQMC(large-scale Chinese question matching corpus)数据集，Q-Qpair数据集      | [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)                                                                                                                                                                                                                                               |
+        | PAWSX                      | 中文PAWS(Paraphrase Adversaries from Word Scrambling)数据集，Q-Qpair数据集        | [PAWSX](https://arxiv.org/abs/1908.11828)                                                                                                                                                                                                                                                             |
+        | STS-B                      | 中文STS-B数据集，中文自然语言推理数据集，从英文STS-B翻译为中文的数据集                                 | [STS-B](https://github.com/pluto-junzeng/CNSD)                                                                                                                                                                                                                                                        |
         
         
         常用英文匹配数据集：
         
         - 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/multi_nli
         - 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/snli
         - https://huggingface.co/datasets/metaeval/cnli
@@ -762,14 +774,15 @@
         - [将句子表示为向量（下）：无监督句子表示学习（sentence embedding）](https://www.cnblogs.com/llhthinker/p/10341841.html)
         - [A Simple but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx)
         - [四种计算文本相似度的方法对比[Yves Peirsman]](https://zhuanlan.zhihu.com/p/37104535)
         - [Improvements to BM25 and Language Models Examined](http://www.cs.otago.ac.nz/homepages/andrew/papers/2014-2.pdf)
         - [CoSENT：比Sentence-BERT更有效的句向量方案](https://kexue.fm/archives/8847)
         - [谈谈文本匹配和多轮检索](https://zhuanlan.zhihu.com/p/111769969)
         - [Sentence-transformers](https://www.sbert.net/examples/applications/computing-embeddings/README.html)
+        - [One Embedder, Any Task: Instruction-Finetuned Text Embeddings](https://arxiv.org/abs/2212.09741)
         
 Keywords: word embedding,text2vec,Chinese Text Similarity Calculation Tool,similarity,word2vec
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: text2vec Version: 1.2.0 Summary: Text to vector
+Metadata-Version: 2.1 Name: text2vec Version: 1.2.1 Summary: Text to vector
 Tool, encode text Home-page: https://github.com/shibing624/text2vec Author:
 XuMing Author-email: xuming624@qq.com License: Apache License 2.0 Description:
 [**ð¨ð³ä¸­æ**](https://github.com/shibing624/text2vec/blob/master/
 README.md) | [**ðEnglish**](https://github.com/shibing624/text2vec/blob/
 master/README_EN.md) | [**ðææ¡£/Docs**](https://github.com/shibing624/
 text2vec/wiki) | [**ð¤æ¨¡å/Models**](https://huggingface.co/shibing624)
                                     [Logo]
@@ -17,18 +17,28 @@
 shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues) [!
 [Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/
 wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact) **Text2vec**: Text to
 Vector, Get Sentence Embeddings. ææ¬åéåï¼æææ¬
 (åæ¬è¯ãå¥å­ãæ®µè½)è¡¨å¾ä¸ºåéç©éµã
 **text2vec**å®ç°äºWord2VecãRankBM25ãBERTãSentence-
 BERTãCoSENTç­å¤ç§ææ¬è¡¨å¾ãææ¬ç¸ä¼¼åº¦è®¡ç®æ¨¡åï¼å¹¶å¨ææ¬è¯­ä¹å¹éï¼ç¸ä¼¼åº¦è®¡ç®ï¼ä»»å¡ä¸æ¯è¾äºåæ¨¡åçææã
-### News [2023/06/15] v1.2.0çæ¬: åå¸äºä¸­æå¹éæ¨¡å[shibing624/
-text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-
-chinese-nli)ï¼åºäº`nghuyong/ernie-3.0-base-
-zh`æ¨¡åï¼ä½¿ç¨äºä¸­æNLIæ°æ®é[shibing624/nli_zh](https://
+### News [2023/06/19] v1.2.1çæ¬: æ´æ°äºä¸­æå¹éæ¨¡å`shibing624/
+text2vec-base-chinese-nli`ä¸ºæ°ç[shibing624/text2vec-base-chinese-sentence]
+(https://huggingface.co/shibing624/text2vec-base-chinese-
+sentence)ï¼éå¯¹CoSENTçlossè®¡ç®å¯¹æåºææç¹ç¹ï¼äººå·¥æéå¹¶æ´çåºé«è´¨éçæç¸å³æ§æåºçSTSæ°æ®é
+[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
+huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
+sentence-
+dataset)ï¼å¨åè¯ä¼°éè¡¨ç°ç¸å¯¹ä¹åææåï¼åå¸äºéç¨äºs2pçä¸­æå¹éæ¨¡å
+[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/
+shibing624/text2vec-base-chinese-paraphrase)ï¼è¯¦è§[Release-v1.2.1](https://
+github.com/shibing624/text2vec/releases/tag/1.2.1) [2023/06/15] v1.2.0çæ¬:
+åå¸äºä¸­æå¹éæ¨¡å[shibing624/text2vec-base-chinese-nli](https://
+huggingface.co/shibing624/text2vec-base-chinese-nli)ï¼åºäº`nghuyong/ernie-
+3.0-base-zh`æ¨¡åï¼ä½¿ç¨äºä¸­æNLIæ°æ®é[shibing624/nli_zh](https://
 huggingface.co/datasets/shibing624/
 nli_zh)å¨é¨è¯­æè®­ç»çCoSENTææ¬å¹éæ¨¡åï¼å¨åè¯ä¼°éè¡¨ç°æåææ¾ï¼è¯¦è§
 [Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
 [2022/03/12] v1.1.4çæ¬: åå¸äºä¸­æå¹éæ¨¡å[shibing624/text2vec-
 base-chinese](https://huggingface.co/shibing624/text2vec-base-
 chinese)ï¼åºäºä¸­æSTSè®­ç»éè®­ç»çCoSENTå¹éæ¨¡åãè¯¦è§
 [Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
@@ -47,88 +57,107 @@
 BERTæ¨¡åçè®­ç»åé¢æµ - [CoSENT(Cosine Sentence)](https://github.com/
 shibing624/text2vec/blob/master/text2vec/
 cosent_model.py)ï¼CoSENTæ¨¡åæåºäºä¸ç§æåºçæå¤±å½æ°ï¼ä½¿è®­ç»è¿ç¨æ´è´´è¿é¢æµï¼æ¨¡åæ¶æéåº¦åæææ¯Sentence-
 BERTæ´å¥½ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºCoSENTæ¨¡åçè®­ç»åé¢æµ
 è¯¦ç»ææ¬åéè¡¨ç¤ºæ¹æ³è§wiki: [ææ¬åéè¡¨ç¤ºæ¹æ³](https://
 github.com/shibing624/text2vec/wiki/
 %E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95) #
-Evaluation ### ææ¬å¹é - è±æå¹éæ°æ®éçè¯æµç»æï¼ | Arch |
-Backbone | Model | English-STS-B | | :-- | :--- | :--- | :-: | | GloVe | glove
-| Avg_word_embeddings_glove_6B_300d | 61.77 | | BERT | bert-base-uncased |
-BERT-base-cls | 20.29 | | BERT | bert-base-uncased | BERT-base-first_last_avg |
-59.04 | | BERT | bert-base-uncased | BERT-base-first_last_avg-whiten(NLI) |
-63.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-
-nli-cls | 73.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens |
-SBERT-base-nli-first_last_avg | 77.96 | | SBERT | xlm-roberta-base |
-paraphrase-multilingual-MiniLM-L12-v2 | 84.42 | | CoSENT | bert-base-uncased |
-CoSENT-base-first_last_avg | 69.93 | | CoSENT | sentence-transformers/bert-
-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68 | -
-ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | Backbone | Model | ATEC | BQ |
-LCQMC | PAWSX | STS-B | Avg | QPS | | :-- | :--- | :--- | :-: | :-: | :-: | :-:
-| :-: | :-: | :-: | | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base |
-50.39 | **72.93** | **79.17** | **60.86** | **80.51** | **68.77** | 3008 | |
-CoSENT | Langboat/mengzi-bert-base | CoSENT-mengzi-base | **50.52** | 72.27 |
-78.69 | 12.89 | 80.15 | 58.90 | 2502 | | CoSENT | bert-base-chinese | CoSENT-
-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 80.14 | 68.19 | 2653 | | SBERT |
-bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 |
-61.74 | 3365 | | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28
-| 68.63 | **79.42** | 55.59 | 64.82 | 63.15 | 2948 | | CoSENT | hfl/chinese-
-roberta-wwm-ext | CoSENT-roberta-ext | **50.81** | **71.45** | **79.31** |
-**61.56** | **81.13** | **68.85** | - | | SBERT | hfl/chinese-roberta-wwm-ext |
-SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | - | -
-æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ | Arch | BaseModel | Model
-| ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | QPS | | :-- |:---------------------
---------|:---------------------------------------------------------------------
------------------------------------------------------------------------------|:
------:|:-----:|:-----:|:-----:|:-----:|:---------:|:-----:| | Word2Vec |
+Evaluation ææ¬å¹é #### è±æå¹éæ°æ®éçè¯æµç»æï¼ | Arch |
+BaseModel | Model | English-STS-B | |:-------|:--------------------------------
+----------------|:-------------------------------------|:-------------:| |
+GloVe | glove | Avg_word_embeddings_glove_6B_300d | 61.77 | | BERT | bert-base-
+uncased | BERT-base-cls | 20.29 | | BERT | bert-base-uncased | BERT-base-
+first_last_avg | 59.04 | | BERT | bert-base-uncased | BERT-base-first_last_avg-
+whiten(NLI) | 63.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens
+| SBERT-base-nli-cls | 73.65 | | SBERT | sentence-transformers/bert-base-nli-
+mean-tokens | SBERT-base-nli-first_last_avg | 77.96 | | CoSENT | bert-base-
+uncased | CoSENT-base-first_last_avg | 69.93 | | CoSENT | sentence-
+transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68
+| #### ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | BaseModel | Model |
+ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | |:-------|:--------------------------
+--|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:| |
+SBERT | bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 |
+66.41 | 61.74 | | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28
+| 68.63 | 79.42 | 55.59 | 64.82 | 63.15 | | SBERT | hfl/chinese-roberta-wwm-ext
+| SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | | CoSENT
+| bert-base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 79.27
+| 68.01 | | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 |
+72.93 | 79.17 | 60.86 | 79.30 | 68.53 | | CoSENT | hfl/chinese-roberta-wwm-ext
+| CoSENT-roberta-ext | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
+è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
+ä¸ºè¯æµæ¨¡åè½åï¼ç»æååªç¨è¯¥æ°æ®éçtrainè®­ç»ï¼å¨testä¸è¯ä¼°å¾å°çè¡¨ç°ï¼æ²¡ç¨å¤é¨æ°æ®
+### Release Models - æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ |
+Arch | BaseModel | Model | ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-
+dc | Avg | QPS | |:-----------|:----------------------------------|:-----------
+-------------------------------------------------------------------------------
+--------------------------------------------------------|:-----:|:-----:|:----
+-:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:| | Word2Vec |
 word2vec | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/
-download.html) | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 33.86 | 23769 | | SBERT
-| xlm-roberta-base | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-
-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-
-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 | 41.99 | 3138 | |
-CoSENT | hfl/chinese-macbert-base | [shibing624/text2vec-base-chinese](https://
-huggingface.co/shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 |
-17.21 | 79.30 | 48.25 | 3008 | | CoSENT | hfl/chinese-lert-large |
+download.html) | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 55.04 | 20.70 | 35.03 |
+23769 | | SBERT | xlm-roberta-base | [sentence-transformers/paraphrase-
+multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/
+paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90
+| 63.01 | 52.28 | 46.46 | 3138 | | Instructor | hfl/chinese-roberta-wwm-ext |
+[moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base) | 41.27 | 63.81 |
+74.87 | 12.20 | 76.96 | 75.83 | 60.55 | 57.93 | 2980 | | CoSENT | hfl/chinese-
+macbert-base | [shibing624/text2vec-base-chinese](https://huggingface.co/
+shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |
+70.27 | 50.42 | 51.61 | 3008 | | CoSENT | hfl/chinese-lert-large |
 [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/
-text2vec-large-chinese) | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 | 48.08 | 2092
-| | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-base-chinese-
-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli) | 51.26 |
-68.72 | 79.13 | 34.28 | 80.70 | **62.81** | 3066 | è¯´æï¼ -
-ç»æå¼æ¯spearmanç³»æ° -
-ç»æååªç¨è¯¥æ°æ®éçtrainè®­ç»ï¼å¨testä¸è¯ä¼°å¾å°çè¡¨ç°ï¼æ²¡ç¨å¤é¨æ°æ®
-- `shibing624/text2vec-base-
+text2vec-large-chinese) | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 | 73.01 | 59.04
+| 53.12 | 2092 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-
+base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-
+sentence) | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 | 70.60 | 53.08 | 59.87 |
+3089 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-base-
+chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-
+paraphrase) | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 | 76.70 | 63.30 | **63.08**
+| 3066 | è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
+æ¨¡åè®­ç»å®éªæ¥åï¼[å®éªæ¥å](https://github.com/shibing624/
+text2vec/blob/master/docs/model_report.md) - `shibing624/text2vec-base-
 chinese`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`hfl/chinese-macbert-
 base`å¨ä¸­æSTS-Bæ°æ®è®­ç»å¾å°ï¼å¹¶å¨ä¸­æSTS-
 Bæµè¯éè¯ä¼°è¾¾å°è¾å¥½ææï¼è¿è¡[examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/
-training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ å°huggingfaceçæ¨¡ååº
-[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-
-base-chinese)ï¼ä¸­æéç¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `shibing624/
-text2vec-base-chinese-nli`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`nghuyong/
-ernie-3.0-base-zh`ç¨ä¸­æNLIæ°æ®é[shibing624/nli_zh](https://
-huggingface.co/datasets/shibing624/
-nli_zh)å¨é¨è¯­æè®­ç»å¾å°ï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°SOTAï¼è¿è¡
-[examples/training_sup_text_matching_model.py](https://github.com/shibing624/
-text2vec/blob/master/examples/
-training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ å°huggingfaceçæ¨¡ååº
-[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/
-text2vec-base-chinese-nli)ï¼ä¸­æs2s
-(å¥å­vså¥å­)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `SBERT-macbert-
-base`æ¨¡åï¼æ¯ç¨SBERTæ¹æ³è®­ç»ï¼è¿è¡[examples/
+training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼ä¸­æéç¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `shibing624/text2vec-
+base-chinese-sentence`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`nghuyong/
+ernie-3.0-base-zh`ç¨äººå·¥æéåçä¸­æSTSæ°æ®é[shibing624/nli-zh-
+all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/
+shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-
+dataset)è®­ç»å¾å°ï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°è¾å¥½ææï¼è¿è¡
+[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
+shibing624/text2vec/blob/master/examples/
+training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼ä¸­æs2s(å¥å­vså¥å­)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ -
+`shibing624/text2vec-base-chinese-
+paraphrase`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`nghuyong/ernie-3.0-base-
+zh`ç¨äººå·¥æéåçä¸­æSTSæ°æ®é[shibing624/nli-zh-all/text2vec-base-
+chinese-paraphrase-dataset](https://huggingface.co/datasets/shibing624/nli-zh-
+all/tree/main/text2vec-base-chinese-paraphrase-dataset)ï¼æ°æ®éç¸å¯¹äº
+[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
+huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
+sentence-dataset)å å¥äºs2p(sentence to
+paraphrase)æ°æ®ï¼å¼ºåäºå¶é¿ææ¬çè¡¨å¾è½åï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°SOTAï¼è¿è¡
+[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
+shibing624/text2vec/blob/master/examples/
+training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼ä¸­æs2p(å¥å­vsæ®µè½)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `SBERT-
+macbert-base`æ¨¡åï¼æ¯ç¨SBERTæ¹æ³è®­ç»ï¼è¿è¡[examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡å
 - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-
 v2`æ¨¡åæ¯ç¨SBERTè®­ç»ï¼æ¯`paraphrase-MiniLM-L12-
 v2`æ¨¡åçå¤è¯­è¨çæ¬ï¼æ¯æä¸­æãè±æç­ - `w2v-light-tencent-
 chinese`æ¯è¾è®¯è¯åéçWord2Vecæ¨¡åï¼CPUå è½½ä½¿ç¨ï¼éç¨äºä¸­æå­é¢å¹éä»»å¡åç¼ºå°æ°æ®çå·å¯å¨æåµ
 - åé¢è®­ç»æ¨¡ååå¯ä»¥éè¿transformersè°ç¨ï¼å¦MacBERTæ¨¡åï¼`--
 model_name hfl/chinese-macbert-base` æèrobertaæ¨¡åï¼`--model_name uer/
-roberta-medium-wwm-chinese-cluecorpussmall` - ä¸­æå¹éæ°æ®éä¸è½½
-[é¾æ¥è§ä¸æ¹](#æ°æ®é) -
+roberta-medium-wwm-chinese-cluecorpussmall` -
+ä¸ºæµè¯æ¨¡åçé²æ£æ§ï¼å å¥äºæªè®­ç»è¿çSOHUæµè¯éï¼ç¨äºæµè¯æ¨¡åçæ³åè½åï¼ä¸ºè¾¾å°å¼ç®±å³ç¨çå®ç¨ææï¼ä½¿ç¨äºæéå°çåä¸­æå¹éæ°æ®éï¼æ°æ®éä¹ä¸ä¼ å°HF
+datasets[é¾æ¥è§ä¸æ¹](#æ°æ®é) -
 ä¸­æå¹éä»»å¡å®éªè¡¨æï¼poolingæä¼æ¯`EncoderType.FIRST_LAST_AVG`å`EncoderType.MEAN`ï¼ä¸¤èé¢æµææå·®å¼å¾å°
 -
 ä¸­æå¹éè¯æµç»æå¤ç°ï¼å¯ä»¥ä¸è½½ä¸­æå¹éæ°æ®éå°`examples/
 data`ï¼è¿è¡[tests/test_model_spearman.py](https://github.com/shibing624/
 text2vec/blob/master/tests/test_model_spearman.py)ä»£ç å¤ç°è¯æµç»æ -
 QPSçGPUæµè¯ç¯å¢æ¯Tesla V100ï¼æ¾å­32GB # Demo Official Demo: https://
 www.mulanai.com/product/short_text_sim/ HuggingFace Demo: https://
@@ -402,36 +431,40 @@
 github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py) ###
 FastAPIæå¡ - å®è£ï¼ ```pip install fastapi uvicorn``` - å¯å¨æå¡ï¼
 example: [examples/fastapi_server_demo.py](https://github.com/shibing624/
 text2vec/blob/master/examples/fastapi_server_demo.py) ```shell cd examples
 python fastapi_server_demo.py ``` - è°ç¨æå¡ï¼ ```shell curl -X 'GET' \
 'http://0.0.0.0:8001/emb?q=hello' \ -H 'accept: application/json' ``` ##
 æ°æ®é - æ¬é¡¹ç®releaseçæ°æ®éï¼ | Dataset | Introduce | Download
-Link | |:----------------------|:----------------------------------------------
-----------------------|:-------------------------------------------------------
+Link | |:---------------------------|:-----------------------------------------
+--------------------------------|:---------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
---| | shibing624/nli-zh-all |
+------------| | shibing624/nli-zh-all |
 ä¸­æè¯­ä¹å¹éæ°æ®åéï¼æ´åäºææ¬æ¨çï¼ç¸ä¼¼ï¼æè¦ï¼é®ç­ï¼æä»¤å¾®è°ç­ä»»å¡ç820ä¸é«è´¨éæ°æ®ï¼å¹¶è½¬åä¸ºå¹éæ ¼å¼æ°æ®é
 | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://
 huggingface.co/datasets/shibing624/nli-zh-all) | | shibing624/snli-zh |
 ä¸­æSNLIåMultiNLIæ°æ®éï¼ç¿»è¯èªè±æSNLIåMultiNLI | [https://
 huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/
 shibing624/snli-zh) | | shibing624/nli_zh |
 ä¸­æè¯­ä¹å¹éæ°æ®éï¼æ´åäºä¸­æATECãBQãLCQMCãPAWSXãSTS-
 Bå±5ä¸ªä»»å¡çæ°æ®é | [https://huggingface.co/datasets/shibing624/
 nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)  or  [ç¾åº¦ç½ç
 (æåç :qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ)  or
 [github](https://github.com/shibing624/text2vec/releases/download/1.1.2/
-senteval_cn.zip)  | | ATEC | ä¸­æATECæ°æ®éï¼èèéæQ-Qpairæ°æ®é
-| [ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC) | | BQ
-| ä¸­æBQ(Bank Question)æ°æ®éï¼é¶è¡Q-Qpairæ°æ®é | [BQ](http://
-icrc.hitsz.edu.cn/info/1037/1162.htm) | | LCQMC | ä¸­æLCQMC(large-scale
-Chinese question matching corpus)æ°æ®éï¼Q-Qpairæ°æ®é | [LCQMC](http://
+senteval_cn.zip)  | | shibing624/sts-sohu2021 |
+ä¸­æè¯­ä¹å¹éæ°æ®éï¼2021æçæ ¡å­ææ¬å¹éç®æ³å¤§èµæ°æ®é
+| [https://huggingface.co/datasets/shibing624/sts-sohu2021](https://
+huggingface.co/datasets/shibing624/sts-sohu2021) | | ATEC |
+ä¸­æATECæ°æ®éï¼èèéæQ-Qpairæ°æ®é | [ATEC](https://github.com/
+IceFlameWorm/NLP_Datasets/tree/master/ATEC) | | BQ | ä¸­æBQ(Bank
+Question)æ°æ®éï¼é¶è¡Q-Qpairæ°æ®é | [BQ](http://icrc.hitsz.edu.cn/
+info/1037/1162.htm) | | LCQMC | ä¸­æLCQMC(large-scale Chinese question
+matching corpus)æ°æ®éï¼Q-Qpairæ°æ®é | [LCQMC](http://
 icrc.hitsz.edu.cn/Article/show/171.html) | | PAWSX | ä¸­æPAWS(Paraphrase
 Adversaries from Word Scrambling)æ°æ®éï¼Q-Qpairæ°æ®é | [PAWSX](https:/
 /arxiv.org/abs/1908.11828) | | STS-B | ä¸­æSTS-
 Bæ°æ®éï¼ä¸­æèªç¶è¯­è¨æ¨çæ°æ®éï¼ä»è±æSTS-
 Bç¿»è¯ä¸ºä¸­æçæ°æ®é | [STS-B](https://github.com/pluto-junzeng/CNSD) |
 å¸¸ç¨è±æå¹éæ°æ®éï¼ - å¤§åé¼é¼çmulti_nliåsnli: https://
 huggingface.co/datasets/multi_nli - å¤§åé¼é¼çmulti_nliåsnli: https://
@@ -473,16 +506,17 @@
 Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx) -
 [åç§è®¡ç®ææ¬ç¸ä¼¼åº¦çæ¹æ³å¯¹æ¯[Yves Peirsman]](https://
 zhuanlan.zhihu.com/p/37104535) - [Improvements to BM25 and Language Models
 Examined](http://www.cs.otago.ac.nz/homepages/andrew/papers/2014-2.pdf) -
 [CoSENTï¼æ¯Sentence-BERTæ´ææçå¥åéæ¹æ¡](https://kexue.fm/
 archives/8847) - [è°è°ææ¬å¹éåå¤è½®æ£ç´¢](https://
 zhuanlan.zhihu.com/p/111769969) - [Sentence-transformers](https://
-www.sbert.net/examples/applications/computing-embeddings/README.html) Keywords:
-word embedding,text2vec,Chinese Text Similarity Calculation
-Tool,similarity,word2vec Platform: UNKNOWN Classifier: Development Status :: 5
-- Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Education Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: Apache Software License
+www.sbert.net/examples/applications/computing-embeddings/README.html) - [One
+Embedder, Any Task: Instruction-Finetuned Text Embeddings](https://arxiv.org/
+abs/2212.09741) Keywords: word embedding,text2vec,Chinese Text Similarity
+Calculation Tool,similarity,word2vec Platform: UNKNOWN Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.6.0 Description-Content-Type: text/markdown
```

### Comparing `text2vec-1.2.0/README.md` & `text2vec-1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 
 **Text2vec**: Text to Vector, Get Sentence Embeddings. 文本向量化，把文本(包括词、句子、段落)表征为向量矩阵。
 
 **text2vec**实现了Word2Vec、RankBM25、BERT、Sentence-BERT、CoSENT等多种文本表征、文本相似度计算模型，并在文本语义匹配（相似度计算）任务上比较了各模型的效果。
 
 ### News
+[2023/06/19] v1.2.1版本: 更新了中文匹配模型`shibing624/text2vec-base-chinese-nli`为新版[shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)，针对CoSENT的loss计算对排序敏感特点，人工挑选并整理出高质量的有相关性排序的STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)，在各评估集表现相对之前有提升；发布了适用于s2p的中文匹配模型[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)，详见[Release-v1.2.1](https://github.com/shibing624/text2vec/releases/tag/1.2.1)
+
 [2023/06/15] v1.2.0版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)，基于`nghuyong/ernie-3.0-base-zh`模型，使用了中文NLI数据集[shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)全部语料训练的CoSENT文本匹配模型，在各评估集表现提升明显，详见[Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
 
 [2022/03/12] v1.1.4版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，基于中文STS训练集训练的CoSENT匹配模型。详见[Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
 
 
 **Guide**
 - [Feature](#Feature)
@@ -42,63 +44,72 @@
 - [Word2Vec](https://github.com/shibing624/text2vec/blob/master/text2vec/word2vec.py)：通过腾讯AI Lab开源的大规模高质量中文[词向量数据（800万中文词轻量版）](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) (文件名：light_Tencent_AILab_ChineseEmbedding.bin 密码: tawe）实现词向量检索，本项目实现了句子（词向量求平均）的word2vec向量表示
 - [SBERT(Sentence-BERT)](https://github.com/shibing624/text2vec/blob/master/text2vec/sentencebert_model.py)：权衡性能和效率的句向量表示模型，训练时通过有监督训练上层分类函数，文本匹配预测时直接句子向量做余弦，本项目基于PyTorch复现了Sentence-BERT模型的训练和预测
 - [CoSENT(Cosine Sentence)](https://github.com/shibing624/text2vec/blob/master/text2vec/cosent_model.py)：CoSENT模型提出了一种排序的损失函数，使训练过程更贴近预测，模型收敛速度和效果比Sentence-BERT更好，本项目基于PyTorch实现了CoSENT模型的训练和预测
 
 详细文本向量表示方法见wiki: [文本向量表示方法](https://github.com/shibing624/text2vec/wiki/%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95)
 # Evaluation
 
-### 文本匹配
+文本匹配
+
+#### 英文匹配数据集的评测结果：
+
 
-- 英文匹配数据集的评测结果：
+| Arch   | BaseModel                                        | Model                            | English-STS-B | 
+|:-------|:------------------------------------------------|:-------------------------------------|:-------------:|
+| GloVe  | glove                                           | Avg_word_embeddings_glove_6B_300d    |     61.77     |
+| BERT   | bert-base-uncased                               | BERT-base-cls                        |     20.29     |
+| BERT   | bert-base-uncased                               | BERT-base-first_last_avg             |     59.04     |
+| BERT   | bert-base-uncased                               | BERT-base-first_last_avg-whiten(NLI) |     63.65     |
+| SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls                   |     73.65     |
+| SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg        |     77.96     |
+| CoSENT | bert-base-uncased                               | CoSENT-base-first_last_avg           |     69.93     |
+| CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg       |     79.68     |
+
+#### 中文匹配数据集的评测结果：
+
+
+| Arch   | BaseModel                    | Model           | ATEC  |  BQ   | LCQMC | PAWSX | STS-B |  Avg  | 
+|:-------|:----------------------------|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
+| SBERT  | bert-base-chinese           | SBERT-bert-base     | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74 |
+| SBERT  | hfl/chinese-macbert-base    | SBERT-macbert-base  | 47.28 | 68.63 | 79.42 | 55.59 | 64.82 | 63.15 |
+| SBERT  | hfl/chinese-roberta-wwm-ext | SBERT-roberta-ext   | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 |
+| CoSENT | bert-base-chinese           | CoSENT-bert-base    | 49.74 | 72.38 | 78.69 | 60.00 | 79.27 | 68.01 |
+| CoSENT | hfl/chinese-macbert-base    | CoSENT-macbert-base | 50.39 | 72.93 | 79.17 | 60.86 | 79.30 | 68.53 |
+| CoSENT | hfl/chinese-roberta-wwm-ext | CoSENT-roberta-ext  | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
+
+说明：
+- 结果评测指标：spearman系数
+- 为评测模型能力，结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
 
-| Arch | Backbone | Model  | English-STS-B | 
-| :-- | :--- | :--- | :-: |
-| GloVe | glove | Avg_word_embeddings_glove_6B_300d | 61.77 |
-| BERT | bert-base-uncased | BERT-base-cls | 20.29 |
-| BERT | bert-base-uncased | BERT-base-first_last_avg | 59.04 |
-| BERT | bert-base-uncased | BERT-base-first_last_avg-whiten(NLI) | 63.65 |
-| SBERT | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls | 73.65 |
-| SBERT | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg | 77.96 |
-| SBERT | xlm-roberta-base | paraphrase-multilingual-MiniLM-L12-v2 | 84.42 |
-| CoSENT | bert-base-uncased | CoSENT-base-first_last_avg | 69.93 |
-| CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68 |
-
-- 中文匹配数据集的评测结果：
-
-| Arch | Backbone | Model  | ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | QPS |
-| :-- | :--- | :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
-| CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 | **72.93** | **79.17** | **60.86** | **80.51** | **68.77**  | 3008 |
-| CoSENT | Langboat/mengzi-bert-base | CoSENT-mengzi-base | **50.52** | 72.27 | 78.69 | 12.89 | 80.15 | 58.90 | 2502 |
-| CoSENT | bert-base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 80.14 | 68.19 | 2653 |
-| SBERT | bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74 | 3365 |
-| SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28 | 68.63 | **79.42** | 55.59 | 64.82 | 63.15 | 2948 |
-| CoSENT | hfl/chinese-roberta-wwm-ext | CoSENT-roberta-ext | **50.81** | **71.45** | **79.31** | **61.56** | **81.13** | **68.85** | - |
-| SBERT | hfl/chinese-roberta-wwm-ext | SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | - |
 
+### Release Models
 - 本项目release模型的中文匹配评测结果：
 
-| Arch | BaseModel                    | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B |    Avg    |  QPS  |
-| :-- |:-----------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:---------:|:-----:|
-| Word2Vec | word2vec                     | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |   33.86   | 23769 |
-| SBERT | xlm-roberta-base             | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |   41.99   | 3138  |
-| CoSENT | hfl/chinese-macbert-base     | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | 48.25 | 3008  |
-| CoSENT | hfl/chinese-lert-large       | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |   48.08   | 2092  |
-| CoSENT | nghuyong/ernie-3.0-base-zh   | [shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)                                               | 51.26 | 68.72 | 79.13 | 34.28 | 80.70 |   **62.81**   | 3066  |
+| Arch       | BaseModel                         | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc |    Avg    |  QPS  |
+|:-----------|:----------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:|
+| Word2Vec   | word2vec                          | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |  55.04  |  20.70  |   35.03   | 23769 |
+| SBERT      | xlm-roberta-base                  | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |  63.01  |  52.28  |   46.46   | 3138  |
+| Instructor | hfl/chinese-roberta-wwm-ext       | [moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base)                                                                                       | 41.27 | 63.81 | 74.87 | 12.20 | 76.96 |  75.83  |  60.55  |   57.93   | 2980  |
+| CoSENT     | hfl/chinese-macbert-base          | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |  70.27  |  50.42  |   51.61   | 3008  |
+| CoSENT     | hfl/chinese-lert-large            | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |  73.01  |  59.04  |   53.12   | 2092  |
+| CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)                                     | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 |  70.60  |  53.08  |   59.87   | 3089  |
+| CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)                                 | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 |  76.70  |  63.30  | **63.08** | 3066  |
 
 
 说明：
-- 结果值是spearman系数
-- 结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
-- `shibing624/text2vec-base-chinese`模型，是用CoSENT方法训练，基于`hfl/chinese-macbert-base`在中文STS-B数据训练得到，并在中文STS-B测试集评估达到较好效果，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，中文通用语义匹配任务推荐使用
-- `shibing624/text2vec-base-chinese-nli`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用中文NLI数据集[shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)全部语料训练得到，并在中文各NLI测试集评估达到SOTA，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)，中文s2s(句子vs句子)语义匹配任务推荐使用
+- 结果评测指标：spearman系数
+- 模型训练实验报告：[实验报告](https://github.com/shibing624/text2vec/blob/master/docs/model_report.md)
+- `shibing624/text2vec-base-chinese`模型，是用CoSENT方法训练，基于`hfl/chinese-macbert-base`在中文STS-B数据训练得到，并在中文STS-B测试集评估达到较好效果，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传HF model hub，中文通用语义匹配任务推荐使用
+- `shibing624/text2vec-base-chinese-sentence`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)训练得到，并在中文各NLI测试集评估达到较好效果，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2s(句子vs句子)语义匹配任务推荐使用
+- `shibing624/text2vec-base-chinese-paraphrase`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-paraphrase-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-paraphrase-dataset)，数据集相对于[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)加入了s2p(sentence to paraphrase)数据，强化了其长文本的表征能力，并在中文各NLI测试集评估达到SOTA，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2p(句子vs段落)语义匹配任务推荐使用
 - `SBERT-macbert-base`模型，是用SBERT方法训练，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型
 - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
 - `w2v-light-tencent-chinese`是腾讯词向量的Word2Vec模型，CPU加载使用，适用于中文字面匹配任务和缺少数据的冷启动情况
 - 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base` 或者roberta模型：`--model_name uer/roberta-medium-wwm-chinese-cluecorpussmall`
-- 中文匹配数据集下载[链接见下方](#数据集)
+- 为测评模型的鲁棒性，加入了未训练过的SOHU测试集，用于测试模型的泛化能力；为达到开箱即用的实用效果，使用了搜集到的各中文匹配数据集，数据集也上传到HF datasets[链接见下方](#数据集)
 - 中文匹配任务实验表明，pooling最优是`EncoderType.FIRST_LAST_AVG`和`EncoderType.MEAN`，两者预测效果差异很小
 - 中文匹配评测结果复现，可以下载中文匹配数据集到`examples/data`，运行[tests/test_model_spearman.py](https://github.com/shibing624/text2vec/blob/master/tests/test_model_spearman.py)代码复现评测结果
 - QPS的GPU测试环境是Tesla V100，显存32GB
 
 # Demo
 
 Official Demo: https://www.mulanai.com/product/short_text_sim/
@@ -643,24 +654,25 @@
 ```
 
 
 ## 数据集
 
 - 本项目release的数据集：
 
-| Dataset               | Introduce                                                           | Download Link                                                                                                                                                                                                                                                                                         |
-|:----------------------|:--------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| shibing624/nli-zh-all | 中文语义匹配数据合集，整合了文本推理，相似，摘要，问答，指令微调等任务的820万高质量数据，并转化为匹配格式数据集           | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://huggingface.co/datasets/shibing624/nli-zh-all)                                                                                                                                                                                        |
-| shibing624/snli-zh    | 中文SNLI和MultiNLI数据集，翻译自英文SNLI和MultiNLI                                       | [https://huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/shibing624/snli-zh)                                                                                                                                                                                              |
-| shibing624/nli_zh     | 中文语义匹配数据集，整合了中文ATEC、BQ、LCQMC、PAWSX、STS-B共5个任务的数据集                   | [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh) </br> or </br> [百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ) </br> or </br> [github](https://github.com/shibing624/text2vec/releases/download/1.1.2/senteval_cn.zip) </br> |
-| ATEC                  | 中文ATEC数据集，蚂蚁金服Q-Qpair数据集                                            | [ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)                                                                                                                                                                                                                                 |
-| BQ                    | 中文BQ(Bank Question)数据集，银行Q-Qpair数据集                                 | [BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)                                                                                                                                                                                                                                                     |
-| LCQMC                 | 中文LCQMC(large-scale Chinese question matching corpus)数据集，Q-Qpair数据集 | [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)                                                                                                                                                                                                                                               |
-| PAWSX                 | 中文PAWS(Paraphrase Adversaries from Word Scrambling)数据集，Q-Qpair数据集   | [PAWSX](https://arxiv.org/abs/1908.11828)                                                                                                                                                                                                                                                             |
-| STS-B                 | 中文STS-B数据集，中文自然语言推理数据集，从英文STS-B翻译为中文的数据集                            | [STS-B](https://github.com/pluto-junzeng/CNSD)                                                                                                                                                                                                                                                        |
+| Dataset                    | Introduce                                                                | Download Link                                                                                                                                                                                                                                                                                         |
+|:---------------------------|:-------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| shibing624/nli-zh-all      | 中文语义匹配数据合集，整合了文本推理，相似，摘要，问答，指令微调等任务的820万高质量数据，并转化为匹配格式数据集                | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://huggingface.co/datasets/shibing624/nli-zh-all)                                                                                                                                                                                        |
+| shibing624/snli-zh         | 中文SNLI和MultiNLI数据集，翻译自英文SNLI和MultiNLI                                    | [https://huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/shibing624/snli-zh)                                                                                                                                                                                              |
+| shibing624/nli_zh          | 中文语义匹配数据集，整合了中文ATEC、BQ、LCQMC、PAWSX、STS-B共5个任务的数据集                        | [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh) </br> or </br> [百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ) </br> or </br> [github](https://github.com/shibing624/text2vec/releases/download/1.1.2/senteval_cn.zip) </br> |
+| shibing624/sts-sohu2021    | 中文语义匹配数据集，2021搜狐校园文本匹配算法大赛数据集                                            | [https://huggingface.co/datasets/shibing624/sts-sohu2021](https://huggingface.co/datasets/shibing624/sts-sohu2021)                                                                                                                                                                                    |
+| ATEC                       | 中文ATEC数据集，蚂蚁金服Q-Qpair数据集                                                 | [ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)                                                                                                                                                                                                                                 |
+| BQ                         | 中文BQ(Bank Question)数据集，银行Q-Qpair数据集                                      | [BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)                                                                                                                                                                                                                                                     |
+| LCQMC                      | 中文LCQMC(large-scale Chinese question matching corpus)数据集，Q-Qpair数据集      | [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)                                                                                                                                                                                                                                               |
+| PAWSX                      | 中文PAWS(Paraphrase Adversaries from Word Scrambling)数据集，Q-Qpair数据集        | [PAWSX](https://arxiv.org/abs/1908.11828)                                                                                                                                                                                                                                                             |
+| STS-B                      | 中文STS-B数据集，中文自然语言推理数据集，从英文STS-B翻译为中文的数据集                                 | [STS-B](https://github.com/pluto-junzeng/CNSD)                                                                                                                                                                                                                                                        |
 
 
 常用英文匹配数据集：
 
 - 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/multi_nli
 - 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/snli
 - https://huggingface.co/datasets/metaeval/cnli
@@ -754,7 +766,8 @@
 - [将句子表示为向量（下）：无监督句子表示学习（sentence embedding）](https://www.cnblogs.com/llhthinker/p/10341841.html)
 - [A Simple but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx)
 - [四种计算文本相似度的方法对比[Yves Peirsman]](https://zhuanlan.zhihu.com/p/37104535)
 - [Improvements to BM25 and Language Models Examined](http://www.cs.otago.ac.nz/homepages/andrew/papers/2014-2.pdf)
 - [CoSENT：比Sentence-BERT更有效的句向量方案](https://kexue.fm/archives/8847)
 - [谈谈文本匹配和多轮检索](https://zhuanlan.zhihu.com/p/111769969)
 - [Sentence-transformers](https://www.sbert.net/examples/applications/computing-embeddings/README.html)
+- [One Embedder, Any Task: Instruction-Finetuned Text Embeddings](https://arxiv.org/abs/2212.09741)
```

#### html2text {}

```diff
@@ -14,18 +14,28 @@
 shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues) [!
 [Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/
 wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact) **Text2vec**: Text to
 Vector, Get Sentence Embeddings. ææ¬åéåï¼æææ¬
 (åæ¬è¯ãå¥å­ãæ®µè½)è¡¨å¾ä¸ºåéç©éµã
 **text2vec**å®ç°äºWord2VecãRankBM25ãBERTãSentence-
 BERTãCoSENTç­å¤ç§ææ¬è¡¨å¾ãææ¬ç¸ä¼¼åº¦è®¡ç®æ¨¡åï¼å¹¶å¨ææ¬è¯­ä¹å¹éï¼ç¸ä¼¼åº¦è®¡ç®ï¼ä»»å¡ä¸æ¯è¾äºåæ¨¡åçææã
-### News [2023/06/15] v1.2.0çæ¬: åå¸äºä¸­æå¹éæ¨¡å[shibing624/
-text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-
-chinese-nli)ï¼åºäº`nghuyong/ernie-3.0-base-
-zh`æ¨¡åï¼ä½¿ç¨äºä¸­æNLIæ°æ®é[shibing624/nli_zh](https://
+### News [2023/06/19] v1.2.1çæ¬: æ´æ°äºä¸­æå¹éæ¨¡å`shibing624/
+text2vec-base-chinese-nli`ä¸ºæ°ç[shibing624/text2vec-base-chinese-sentence]
+(https://huggingface.co/shibing624/text2vec-base-chinese-
+sentence)ï¼éå¯¹CoSENTçlossè®¡ç®å¯¹æåºææç¹ç¹ï¼äººå·¥æéå¹¶æ´çåºé«è´¨éçæç¸å³æ§æåºçSTSæ°æ®é
+[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
+huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
+sentence-
+dataset)ï¼å¨åè¯ä¼°éè¡¨ç°ç¸å¯¹ä¹åææåï¼åå¸äºéç¨äºs2pçä¸­æå¹éæ¨¡å
+[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/
+shibing624/text2vec-base-chinese-paraphrase)ï¼è¯¦è§[Release-v1.2.1](https://
+github.com/shibing624/text2vec/releases/tag/1.2.1) [2023/06/15] v1.2.0çæ¬:
+åå¸äºä¸­æå¹éæ¨¡å[shibing624/text2vec-base-chinese-nli](https://
+huggingface.co/shibing624/text2vec-base-chinese-nli)ï¼åºäº`nghuyong/ernie-
+3.0-base-zh`æ¨¡åï¼ä½¿ç¨äºä¸­æNLIæ°æ®é[shibing624/nli_zh](https://
 huggingface.co/datasets/shibing624/
 nli_zh)å¨é¨è¯­æè®­ç»çCoSENTææ¬å¹éæ¨¡åï¼å¨åè¯ä¼°éè¡¨ç°æåææ¾ï¼è¯¦è§
 [Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
 [2022/03/12] v1.1.4çæ¬: åå¸äºä¸­æå¹éæ¨¡å[shibing624/text2vec-
 base-chinese](https://huggingface.co/shibing624/text2vec-base-
 chinese)ï¼åºäºä¸­æSTSè®­ç»éè®­ç»çCoSENTå¹éæ¨¡åãè¯¦è§
 [Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
@@ -44,88 +54,107 @@
 BERTæ¨¡åçè®­ç»åé¢æµ - [CoSENT(Cosine Sentence)](https://github.com/
 shibing624/text2vec/blob/master/text2vec/
 cosent_model.py)ï¼CoSENTæ¨¡åæåºäºä¸ç§æåºçæå¤±å½æ°ï¼ä½¿è®­ç»è¿ç¨æ´è´´è¿é¢æµï¼æ¨¡åæ¶æéåº¦åæææ¯Sentence-
 BERTæ´å¥½ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºCoSENTæ¨¡åçè®­ç»åé¢æµ
 è¯¦ç»ææ¬åéè¡¨ç¤ºæ¹æ³è§wiki: [ææ¬åéè¡¨ç¤ºæ¹æ³](https://
 github.com/shibing624/text2vec/wiki/
 %E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95) #
-Evaluation ### ææ¬å¹é - è±æå¹éæ°æ®éçè¯æµç»æï¼ | Arch |
-Backbone | Model | English-STS-B | | :-- | :--- | :--- | :-: | | GloVe | glove
-| Avg_word_embeddings_glove_6B_300d | 61.77 | | BERT | bert-base-uncased |
-BERT-base-cls | 20.29 | | BERT | bert-base-uncased | BERT-base-first_last_avg |
-59.04 | | BERT | bert-base-uncased | BERT-base-first_last_avg-whiten(NLI) |
-63.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-
-nli-cls | 73.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens |
-SBERT-base-nli-first_last_avg | 77.96 | | SBERT | xlm-roberta-base |
-paraphrase-multilingual-MiniLM-L12-v2 | 84.42 | | CoSENT | bert-base-uncased |
-CoSENT-base-first_last_avg | 69.93 | | CoSENT | sentence-transformers/bert-
-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68 | -
-ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | Backbone | Model | ATEC | BQ |
-LCQMC | PAWSX | STS-B | Avg | QPS | | :-- | :--- | :--- | :-: | :-: | :-: | :-:
-| :-: | :-: | :-: | | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base |
-50.39 | **72.93** | **79.17** | **60.86** | **80.51** | **68.77** | 3008 | |
-CoSENT | Langboat/mengzi-bert-base | CoSENT-mengzi-base | **50.52** | 72.27 |
-78.69 | 12.89 | 80.15 | 58.90 | 2502 | | CoSENT | bert-base-chinese | CoSENT-
-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 80.14 | 68.19 | 2653 | | SBERT |
-bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 |
-61.74 | 3365 | | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28
-| 68.63 | **79.42** | 55.59 | 64.82 | 63.15 | 2948 | | CoSENT | hfl/chinese-
-roberta-wwm-ext | CoSENT-roberta-ext | **50.81** | **71.45** | **79.31** |
-**61.56** | **81.13** | **68.85** | - | | SBERT | hfl/chinese-roberta-wwm-ext |
-SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | - | -
-æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ | Arch | BaseModel | Model
-| ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | QPS | | :-- |:---------------------
---------|:---------------------------------------------------------------------
------------------------------------------------------------------------------|:
------:|:-----:|:-----:|:-----:|:-----:|:---------:|:-----:| | Word2Vec |
+Evaluation ææ¬å¹é #### è±æå¹éæ°æ®éçè¯æµç»æï¼ | Arch |
+BaseModel | Model | English-STS-B | |:-------|:--------------------------------
+----------------|:-------------------------------------|:-------------:| |
+GloVe | glove | Avg_word_embeddings_glove_6B_300d | 61.77 | | BERT | bert-base-
+uncased | BERT-base-cls | 20.29 | | BERT | bert-base-uncased | BERT-base-
+first_last_avg | 59.04 | | BERT | bert-base-uncased | BERT-base-first_last_avg-
+whiten(NLI) | 63.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens
+| SBERT-base-nli-cls | 73.65 | | SBERT | sentence-transformers/bert-base-nli-
+mean-tokens | SBERT-base-nli-first_last_avg | 77.96 | | CoSENT | bert-base-
+uncased | CoSENT-base-first_last_avg | 69.93 | | CoSENT | sentence-
+transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68
+| #### ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | BaseModel | Model |
+ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | |:-------|:--------------------------
+--|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:| |
+SBERT | bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 |
+66.41 | 61.74 | | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28
+| 68.63 | 79.42 | 55.59 | 64.82 | 63.15 | | SBERT | hfl/chinese-roberta-wwm-ext
+| SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | | CoSENT
+| bert-base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 79.27
+| 68.01 | | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 |
+72.93 | 79.17 | 60.86 | 79.30 | 68.53 | | CoSENT | hfl/chinese-roberta-wwm-ext
+| CoSENT-roberta-ext | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
+è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
+ä¸ºè¯æµæ¨¡åè½åï¼ç»æååªç¨è¯¥æ°æ®éçtrainè®­ç»ï¼å¨testä¸è¯ä¼°å¾å°çè¡¨ç°ï¼æ²¡ç¨å¤é¨æ°æ®
+### Release Models - æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ |
+Arch | BaseModel | Model | ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-
+dc | Avg | QPS | |:-----------|:----------------------------------|:-----------
+-------------------------------------------------------------------------------
+--------------------------------------------------------|:-----:|:-----:|:----
+-:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:| | Word2Vec |
 word2vec | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/
-download.html) | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 33.86 | 23769 | | SBERT
-| xlm-roberta-base | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-
-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-
-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 | 41.99 | 3138 | |
-CoSENT | hfl/chinese-macbert-base | [shibing624/text2vec-base-chinese](https://
-huggingface.co/shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 |
-17.21 | 79.30 | 48.25 | 3008 | | CoSENT | hfl/chinese-lert-large |
+download.html) | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 55.04 | 20.70 | 35.03 |
+23769 | | SBERT | xlm-roberta-base | [sentence-transformers/paraphrase-
+multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/
+paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90
+| 63.01 | 52.28 | 46.46 | 3138 | | Instructor | hfl/chinese-roberta-wwm-ext |
+[moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base) | 41.27 | 63.81 |
+74.87 | 12.20 | 76.96 | 75.83 | 60.55 | 57.93 | 2980 | | CoSENT | hfl/chinese-
+macbert-base | [shibing624/text2vec-base-chinese](https://huggingface.co/
+shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |
+70.27 | 50.42 | 51.61 | 3008 | | CoSENT | hfl/chinese-lert-large |
 [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/
-text2vec-large-chinese) | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 | 48.08 | 2092
-| | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-base-chinese-
-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli) | 51.26 |
-68.72 | 79.13 | 34.28 | 80.70 | **62.81** | 3066 | è¯´æï¼ -
-ç»æå¼æ¯spearmanç³»æ° -
-ç»æååªç¨è¯¥æ°æ®éçtrainè®­ç»ï¼å¨testä¸è¯ä¼°å¾å°çè¡¨ç°ï¼æ²¡ç¨å¤é¨æ°æ®
-- `shibing624/text2vec-base-
+text2vec-large-chinese) | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 | 73.01 | 59.04
+| 53.12 | 2092 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-
+base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-
+sentence) | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 | 70.60 | 53.08 | 59.87 |
+3089 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-base-
+chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-
+paraphrase) | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 | 76.70 | 63.30 | **63.08**
+| 3066 | è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
+æ¨¡åè®­ç»å®éªæ¥åï¼[å®éªæ¥å](https://github.com/shibing624/
+text2vec/blob/master/docs/model_report.md) - `shibing624/text2vec-base-
 chinese`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`hfl/chinese-macbert-
 base`å¨ä¸­æSTS-Bæ°æ®è®­ç»å¾å°ï¼å¹¶å¨ä¸­æSTS-
 Bæµè¯éè¯ä¼°è¾¾å°è¾å¥½ææï¼è¿è¡[examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/
-training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ å°huggingfaceçæ¨¡ååº
-[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-
-base-chinese)ï¼ä¸­æéç¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `shibing624/
-text2vec-base-chinese-nli`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`nghuyong/
-ernie-3.0-base-zh`ç¨ä¸­æNLIæ°æ®é[shibing624/nli_zh](https://
-huggingface.co/datasets/shibing624/
-nli_zh)å¨é¨è¯­æè®­ç»å¾å°ï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°SOTAï¼è¿è¡
-[examples/training_sup_text_matching_model.py](https://github.com/shibing624/
-text2vec/blob/master/examples/
-training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ å°huggingfaceçæ¨¡ååº
-[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/
-text2vec-base-chinese-nli)ï¼ä¸­æs2s
-(å¥å­vså¥å­)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `SBERT-macbert-
-base`æ¨¡åï¼æ¯ç¨SBERTæ¹æ³è®­ç»ï¼è¿è¡[examples/
+training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼ä¸­æéç¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `shibing624/text2vec-
+base-chinese-sentence`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`nghuyong/
+ernie-3.0-base-zh`ç¨äººå·¥æéåçä¸­æSTSæ°æ®é[shibing624/nli-zh-
+all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/
+shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-
+dataset)è®­ç»å¾å°ï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°è¾å¥½ææï¼è¿è¡
+[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
+shibing624/text2vec/blob/master/examples/
+training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼ä¸­æs2s(å¥å­vså¥å­)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ -
+`shibing624/text2vec-base-chinese-
+paraphrase`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`nghuyong/ernie-3.0-base-
+zh`ç¨äººå·¥æéåçä¸­æSTSæ°æ®é[shibing624/nli-zh-all/text2vec-base-
+chinese-paraphrase-dataset](https://huggingface.co/datasets/shibing624/nli-zh-
+all/tree/main/text2vec-base-chinese-paraphrase-dataset)ï¼æ°æ®éç¸å¯¹äº
+[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
+huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
+sentence-dataset)å å¥äºs2p(sentence to
+paraphrase)æ°æ®ï¼å¼ºåäºå¶é¿ææ¬çè¡¨å¾è½åï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°SOTAï¼è¿è¡
+[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
+shibing624/text2vec/blob/master/examples/
+training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼ä¸­æs2p(å¥å­vsæ®µè½)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `SBERT-
+macbert-base`æ¨¡åï¼æ¯ç¨SBERTæ¹æ³è®­ç»ï¼è¿è¡[examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡å
 - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-
 v2`æ¨¡åæ¯ç¨SBERTè®­ç»ï¼æ¯`paraphrase-MiniLM-L12-
 v2`æ¨¡åçå¤è¯­è¨çæ¬ï¼æ¯æä¸­æãè±æç­ - `w2v-light-tencent-
 chinese`æ¯è¾è®¯è¯åéçWord2Vecæ¨¡åï¼CPUå è½½ä½¿ç¨ï¼éç¨äºä¸­æå­é¢å¹éä»»å¡åç¼ºå°æ°æ®çå·å¯å¨æåµ
 - åé¢è®­ç»æ¨¡ååå¯ä»¥éè¿transformersè°ç¨ï¼å¦MacBERTæ¨¡åï¼`--
 model_name hfl/chinese-macbert-base` æèrobertaæ¨¡åï¼`--model_name uer/
-roberta-medium-wwm-chinese-cluecorpussmall` - ä¸­æå¹éæ°æ®éä¸è½½
-[é¾æ¥è§ä¸æ¹](#æ°æ®é) -
+roberta-medium-wwm-chinese-cluecorpussmall` -
+ä¸ºæµè¯æ¨¡åçé²æ£æ§ï¼å å¥äºæªè®­ç»è¿çSOHUæµè¯éï¼ç¨äºæµè¯æ¨¡åçæ³åè½åï¼ä¸ºè¾¾å°å¼ç®±å³ç¨çå®ç¨ææï¼ä½¿ç¨äºæéå°çåä¸­æå¹éæ°æ®éï¼æ°æ®éä¹ä¸ä¼ å°HF
+datasets[é¾æ¥è§ä¸æ¹](#æ°æ®é) -
 ä¸­æå¹éä»»å¡å®éªè¡¨æï¼poolingæä¼æ¯`EncoderType.FIRST_LAST_AVG`å`EncoderType.MEAN`ï¼ä¸¤èé¢æµææå·®å¼å¾å°
 -
 ä¸­æå¹éè¯æµç»æå¤ç°ï¼å¯ä»¥ä¸è½½ä¸­æå¹éæ°æ®éå°`examples/
 data`ï¼è¿è¡[tests/test_model_spearman.py](https://github.com/shibing624/
 text2vec/blob/master/tests/test_model_spearman.py)ä»£ç å¤ç°è¯æµç»æ -
 QPSçGPUæµè¯ç¯å¢æ¯Tesla V100ï¼æ¾å­32GB # Demo Official Demo: https://
 www.mulanai.com/product/short_text_sim/ HuggingFace Demo: https://
@@ -399,36 +428,40 @@
 github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py) ###
 FastAPIæå¡ - å®è£ï¼ ```pip install fastapi uvicorn``` - å¯å¨æå¡ï¼
 example: [examples/fastapi_server_demo.py](https://github.com/shibing624/
 text2vec/blob/master/examples/fastapi_server_demo.py) ```shell cd examples
 python fastapi_server_demo.py ``` - è°ç¨æå¡ï¼ ```shell curl -X 'GET' \
 'http://0.0.0.0:8001/emb?q=hello' \ -H 'accept: application/json' ``` ##
 æ°æ®é - æ¬é¡¹ç®releaseçæ°æ®éï¼ | Dataset | Introduce | Download
-Link | |:----------------------|:----------------------------------------------
-----------------------|:-------------------------------------------------------
+Link | |:---------------------------|:-----------------------------------------
+--------------------------------|:---------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
---| | shibing624/nli-zh-all |
+------------| | shibing624/nli-zh-all |
 ä¸­æè¯­ä¹å¹éæ°æ®åéï¼æ´åäºææ¬æ¨çï¼ç¸ä¼¼ï¼æè¦ï¼é®ç­ï¼æä»¤å¾®è°ç­ä»»å¡ç820ä¸é«è´¨éæ°æ®ï¼å¹¶è½¬åä¸ºå¹éæ ¼å¼æ°æ®é
 | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://
 huggingface.co/datasets/shibing624/nli-zh-all) | | shibing624/snli-zh |
 ä¸­æSNLIåMultiNLIæ°æ®éï¼ç¿»è¯èªè±æSNLIåMultiNLI | [https://
 huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/
 shibing624/snli-zh) | | shibing624/nli_zh |
 ä¸­æè¯­ä¹å¹éæ°æ®éï¼æ´åäºä¸­æATECãBQãLCQMCãPAWSXãSTS-
 Bå±5ä¸ªä»»å¡çæ°æ®é | [https://huggingface.co/datasets/shibing624/
 nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)  or  [ç¾åº¦ç½ç
 (æåç :qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ)  or
 [github](https://github.com/shibing624/text2vec/releases/download/1.1.2/
-senteval_cn.zip)  | | ATEC | ä¸­æATECæ°æ®éï¼èèéæQ-Qpairæ°æ®é
-| [ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC) | | BQ
-| ä¸­æBQ(Bank Question)æ°æ®éï¼é¶è¡Q-Qpairæ°æ®é | [BQ](http://
-icrc.hitsz.edu.cn/info/1037/1162.htm) | | LCQMC | ä¸­æLCQMC(large-scale
-Chinese question matching corpus)æ°æ®éï¼Q-Qpairæ°æ®é | [LCQMC](http://
+senteval_cn.zip)  | | shibing624/sts-sohu2021 |
+ä¸­æè¯­ä¹å¹éæ°æ®éï¼2021æçæ ¡å­ææ¬å¹éç®æ³å¤§èµæ°æ®é
+| [https://huggingface.co/datasets/shibing624/sts-sohu2021](https://
+huggingface.co/datasets/shibing624/sts-sohu2021) | | ATEC |
+ä¸­æATECæ°æ®éï¼èèéæQ-Qpairæ°æ®é | [ATEC](https://github.com/
+IceFlameWorm/NLP_Datasets/tree/master/ATEC) | | BQ | ä¸­æBQ(Bank
+Question)æ°æ®éï¼é¶è¡Q-Qpairæ°æ®é | [BQ](http://icrc.hitsz.edu.cn/
+info/1037/1162.htm) | | LCQMC | ä¸­æLCQMC(large-scale Chinese question
+matching corpus)æ°æ®éï¼Q-Qpairæ°æ®é | [LCQMC](http://
 icrc.hitsz.edu.cn/Article/show/171.html) | | PAWSX | ä¸­æPAWS(Paraphrase
 Adversaries from Word Scrambling)æ°æ®éï¼Q-Qpairæ°æ®é | [PAWSX](https:/
 /arxiv.org/abs/1908.11828) | | STS-B | ä¸­æSTS-
 Bæ°æ®éï¼ä¸­æèªç¶è¯­è¨æ¨çæ°æ®éï¼ä»è±æSTS-
 Bç¿»è¯ä¸ºä¸­æçæ°æ®é | [STS-B](https://github.com/pluto-junzeng/CNSD) |
 å¸¸ç¨è±æå¹éæ°æ®éï¼ - å¤§åé¼é¼çmulti_nliåsnli: https://
 huggingface.co/datasets/multi_nli - å¤§åé¼é¼çmulti_nliåsnli: https://
@@ -470,8 +503,10 @@
 Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx) -
 [åç§è®¡ç®ææ¬ç¸ä¼¼åº¦çæ¹æ³å¯¹æ¯[Yves Peirsman]](https://
 zhuanlan.zhihu.com/p/37104535) - [Improvements to BM25 and Language Models
 Examined](http://www.cs.otago.ac.nz/homepages/andrew/papers/2014-2.pdf) -
 [CoSENTï¼æ¯Sentence-BERTæ´ææçå¥åéæ¹æ¡](https://kexue.fm/
 archives/8847) - [è°è°ææ¬å¹éåå¤è½®æ£ç´¢](https://
 zhuanlan.zhihu.com/p/111769969) - [Sentence-transformers](https://
-www.sbert.net/examples/applications/computing-embeddings/README.html)
+www.sbert.net/examples/applications/computing-embeddings/README.html) - [One
+Embedder, Any Task: Instruction-Finetuned Text Embeddings](https://arxiv.org/
+abs/2212.09741)
```

### Comparing `text2vec-1.2.0/setup.py` & `text2vec-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/__init__.py` & `text2vec-1.2.1/text2vec/__init__.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/bertmatching_dataset.py` & `text2vec-1.2.1/text2vec/bertmatching_dataset.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/bertmatching_model.py` & `text2vec-1.2.1/text2vec/bertmatching_model.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/bm25.py` & `text2vec-1.2.1/text2vec/bm25.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/cosent_dataset.py` & `text2vec-1.2.1/text2vec/cosent_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,25 +31,25 @@
     if path.endswith('.jsonl'):
         data_list = load_jsonl(path)
         for entry in data_list:
             field1, field2 = get_field_names(entry)
             if not field1 or not field2:
                 continue
 
-            text_a, text_b, score = entry[field1], entry[field2], int(entry["label"])
+            text_a, text_b, score = entry[field1], entry[field2], float(entry["label"])
             data.append((text_a, score))
             data.append((text_b, score))
     else:
         with open(path, 'r', encoding='utf8') as f:
             for line in f:
                 line = line.strip().split('\t')
                 if len(line) != 3:
                     logger.warning(f'line size not match, pass: {line}')
                     continue
-                score = int(line[2])
+                score = float(line[2])
                 data.append((line[0], score))
                 data.append((line[1], score))
     return data
 
 
 class CosentTrainDataset(Dataset):
     """Cosent文本匹配训练数据集, 重写__getitem__和__len__方法"""
```

### Comparing `text2vec-1.2.0/text2vec/cosent_model.py` & `text2vec-1.2.1/text2vec/cosent_model.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/ngram.py` & `text2vec-1.2.1/text2vec/ngram.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/sentence_model.py` & `text2vec-1.2.1/text2vec/sentence_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 class SentenceModel:
     def __init__(
             self,
             model_name_or_path: str = "shibing624/text2vec-base-chinese",
             encoder_type: Union[str, EncoderType] = "MEAN",
-            max_seq_length: int = 128,
+            max_seq_length: int = 256,
             device: Optional[str] = None,
     ):
         """
         Initializes the base sentence model.
 
         :param model_name_or_path: The name of the model to load from the huggingface models library.
         :param encoder_type: The type of encoder to use, See the EncoderType enum for options:
```

### Comparing `text2vec-1.2.0/text2vec/sentencebert_model.py` & `text2vec-1.2.1/text2vec/sentencebert_model.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/similarity.py` & `text2vec-1.2.1/text2vec/similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,24 @@
 
 class Similarity:
     def __init__(
             self,
             model_name_or_path="shibing624/text2vec-base-chinese",
             similarity_type=SimilarityType.COSINE,
             embedding_type=EmbeddingType.BERT,
-            encoder_type=EncoderType.MEAN
+            encoder_type=EncoderType.MEAN,
+            max_seq_length=256,
     ):
         """
         Cal text similarity
         :param model_name_or_path: str, model path or name, default is None,
-            auto load paraphrase-multilingual-MiniLM-L12-v2
         :param similarity_type: SimilarityType, similarity type, default is COSINE
         :param embedding_type: EmbeddingType, embedding type, default is BERT
         :param encoder_type: EncoderType, encoder type, adjust with model_name_or_path
+        :param max_seq_length: int, max sequence length, default is 256
         """
         if embedding_type not in [EmbeddingType.BERT, EmbeddingType.WORD2VEC]:
             logger.warning('embedding_type set error, use default bert')
             embedding_type = EmbeddingType.BERT
         if similarity_type not in [SimilarityType.COSINE, SimilarityType.WMD]:
             logger.warning('similarity_type set error, use default cosine')
             similarity_type = SimilarityType.COSINE
@@ -66,15 +67,19 @@
                 # Default: Word2Vec("w2v-light-tencent-chinese")
                 self.model = Word2Vec(model_name_or_path)
             except ValueError as e:
                 logger.error(f"{model_name_or_path} is not Word2Vec model")
                 raise ValueError(e)
         elif self.embedding_type == EmbeddingType.BERT:
             try:
-                self.model = SentenceModel(model_name_or_path, encoder_type=self.encoder_type)
+                self.model = SentenceModel(
+                    model_name_or_path,
+                    encoder_type=self.encoder_type,
+                    max_seq_length=max_seq_length,
+                )
             except ValueError as e:
                 logger.error(f"{model_name_or_path} is not Bert model")
                 raise ValueError(e)
         else:
             raise ValueError('embedding_type error')
 
     def __str__(self):
```

### Comparing `text2vec-1.2.0/text2vec/stopwords.txt` & `text2vec-1.2.1/text2vec/stopwords.txt`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/text_matching_dataset.py` & `text2vec-1.2.1/text2vec/text_matching_dataset.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/utils/distance.py` & `text2vec-1.2.1/text2vec/utils/distance.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/utils/get_file.py` & `text2vec-1.2.1/text2vec/utils/get_file.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/utils/io_util.py` & `text2vec-1.2.1/text2vec/utils/io_util.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/utils/rank_bm25.py` & `text2vec-1.2.1/text2vec/utils/rank_bm25.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/utils/stats_util.py` & `text2vec-1.2.1/text2vec/utils/stats_util.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/utils/tokenizer.py` & `text2vec-1.2.1/text2vec/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec/word2vec.py` & `text2vec-1.2.1/text2vec/word2vec.py`

 * *Files identical despite different names*

### Comparing `text2vec-1.2.0/text2vec.egg-info/PKG-INFO` & `text2vec-1.2.1/text2vec.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2vec
-Version: 1.2.0
+Version: 1.2.1
 Summary: Text to vector Tool, encode text
 Home-page: https://github.com/shibing624/text2vec
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache License 2.0
 Description: [**🇨🇳中文**](https://github.com/shibing624/text2vec/blob/master/README.md) | [**🌐English**](https://github.com/shibing624/text2vec/blob/master/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/text2vec/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624) 
         
@@ -27,14 +27,16 @@
         
         
         **Text2vec**: Text to Vector, Get Sentence Embeddings. 文本向量化，把文本(包括词、句子、段落)表征为向量矩阵。
         
         **text2vec**实现了Word2Vec、RankBM25、BERT、Sentence-BERT、CoSENT等多种文本表征、文本相似度计算模型，并在文本语义匹配（相似度计算）任务上比较了各模型的效果。
         
         ### News
+        [2023/06/19] v1.2.1版本: 更新了中文匹配模型`shibing624/text2vec-base-chinese-nli`为新版[shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)，针对CoSENT的loss计算对排序敏感特点，人工挑选并整理出高质量的有相关性排序的STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)，在各评估集表现相对之前有提升；发布了适用于s2p的中文匹配模型[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)，详见[Release-v1.2.1](https://github.com/shibing624/text2vec/releases/tag/1.2.1)
+        
         [2023/06/15] v1.2.0版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)，基于`nghuyong/ernie-3.0-base-zh`模型，使用了中文NLI数据集[shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)全部语料训练的CoSENT文本匹配模型，在各评估集表现提升明显，详见[Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
         
         [2022/03/12] v1.1.4版本: 发布了中文匹配模型[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，基于中文STS训练集训练的CoSENT匹配模型。详见[Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
         
         
         **Guide**
         - [Feature](#Feature)
@@ -50,63 +52,72 @@
         - [Word2Vec](https://github.com/shibing624/text2vec/blob/master/text2vec/word2vec.py)：通过腾讯AI Lab开源的大规模高质量中文[词向量数据（800万中文词轻量版）](https://pan.baidu.com/s/1La4U4XNFe8s5BJqxPQpeiQ) (文件名：light_Tencent_AILab_ChineseEmbedding.bin 密码: tawe）实现词向量检索，本项目实现了句子（词向量求平均）的word2vec向量表示
         - [SBERT(Sentence-BERT)](https://github.com/shibing624/text2vec/blob/master/text2vec/sentencebert_model.py)：权衡性能和效率的句向量表示模型，训练时通过有监督训练上层分类函数，文本匹配预测时直接句子向量做余弦，本项目基于PyTorch复现了Sentence-BERT模型的训练和预测
         - [CoSENT(Cosine Sentence)](https://github.com/shibing624/text2vec/blob/master/text2vec/cosent_model.py)：CoSENT模型提出了一种排序的损失函数，使训练过程更贴近预测，模型收敛速度和效果比Sentence-BERT更好，本项目基于PyTorch实现了CoSENT模型的训练和预测
         
         详细文本向量表示方法见wiki: [文本向量表示方法](https://github.com/shibing624/text2vec/wiki/%E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95)
         # Evaluation
         
-        ### 文本匹配
+        文本匹配
+        
+        #### 英文匹配数据集的评测结果：
+        
         
-        - 英文匹配数据集的评测结果：
+        | Arch   | BaseModel                                        | Model                            | English-STS-B | 
+        |:-------|:------------------------------------------------|:-------------------------------------|:-------------:|
+        | GloVe  | glove                                           | Avg_word_embeddings_glove_6B_300d    |     61.77     |
+        | BERT   | bert-base-uncased                               | BERT-base-cls                        |     20.29     |
+        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg             |     59.04     |
+        | BERT   | bert-base-uncased                               | BERT-base-first_last_avg-whiten(NLI) |     63.65     |
+        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls                   |     73.65     |
+        | SBERT  | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg        |     77.96     |
+        | CoSENT | bert-base-uncased                               | CoSENT-base-first_last_avg           |     69.93     |
+        | CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg       |     79.68     |
+        
+        #### 中文匹配数据集的评测结果：
+        
+        
+        | Arch   | BaseModel                    | Model           | ATEC  |  BQ   | LCQMC | PAWSX | STS-B |  Avg  | 
+        |:-------|:----------------------------|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
+        | SBERT  | bert-base-chinese           | SBERT-bert-base     | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74 |
+        | SBERT  | hfl/chinese-macbert-base    | SBERT-macbert-base  | 47.28 | 68.63 | 79.42 | 55.59 | 64.82 | 63.15 |
+        | SBERT  | hfl/chinese-roberta-wwm-ext | SBERT-roberta-ext   | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 |
+        | CoSENT | bert-base-chinese           | CoSENT-bert-base    | 49.74 | 72.38 | 78.69 | 60.00 | 79.27 | 68.01 |
+        | CoSENT | hfl/chinese-macbert-base    | CoSENT-macbert-base | 50.39 | 72.93 | 79.17 | 60.86 | 79.30 | 68.53 |
+        | CoSENT | hfl/chinese-roberta-wwm-ext | CoSENT-roberta-ext  | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
+        
+        说明：
+        - 结果评测指标：spearman系数
+        - 为评测模型能力，结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
         
-        | Arch | Backbone | Model  | English-STS-B | 
-        | :-- | :--- | :--- | :-: |
-        | GloVe | glove | Avg_word_embeddings_glove_6B_300d | 61.77 |
-        | BERT | bert-base-uncased | BERT-base-cls | 20.29 |
-        | BERT | bert-base-uncased | BERT-base-first_last_avg | 59.04 |
-        | BERT | bert-base-uncased | BERT-base-first_last_avg-whiten(NLI) | 63.65 |
-        | SBERT | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-cls | 73.65 |
-        | SBERT | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-nli-first_last_avg | 77.96 |
-        | SBERT | xlm-roberta-base | paraphrase-multilingual-MiniLM-L12-v2 | 84.42 |
-        | CoSENT | bert-base-uncased | CoSENT-base-first_last_avg | 69.93 |
-        | CoSENT | sentence-transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68 |
-        
-        - 中文匹配数据集的评测结果：
-        
-        | Arch | Backbone | Model  | ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | QPS |
-        | :-- | :--- | :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
-        | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 | **72.93** | **79.17** | **60.86** | **80.51** | **68.77**  | 3008 |
-        | CoSENT | Langboat/mengzi-bert-base | CoSENT-mengzi-base | **50.52** | 72.27 | 78.69 | 12.89 | 80.15 | 58.90 | 2502 |
-        | CoSENT | bert-base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 80.14 | 68.19 | 2653 |
-        | SBERT | bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 | 61.74 | 3365 |
-        | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28 | 68.63 | **79.42** | 55.59 | 64.82 | 63.15 | 2948 |
-        | CoSENT | hfl/chinese-roberta-wwm-ext | CoSENT-roberta-ext | **50.81** | **71.45** | **79.31** | **61.56** | **81.13** | **68.85** | - |
-        | SBERT | hfl/chinese-roberta-wwm-ext | SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | - |
         
+        ### Release Models
         - 本项目release模型的中文匹配评测结果：
         
-        | Arch | BaseModel                    | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B |    Avg    |  QPS  |
-        | :-- |:-----------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:---------:|:-----:|
-        | Word2Vec | word2vec                     | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |   33.86   | 23769 |
-        | SBERT | xlm-roberta-base             | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |   41.99   | 3138  |
-        | CoSENT | hfl/chinese-macbert-base     | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 | 48.25 | 3008  |
-        | CoSENT | hfl/chinese-lert-large       | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |   48.08   | 2092  |
-        | CoSENT | nghuyong/ernie-3.0-base-zh   | [shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)                                               | 51.26 | 68.72 | 79.13 | 34.28 | 80.70 |   **62.81**   | 3066  |
+        | Arch       | BaseModel                         | Model                                                                                                                                             | ATEC  |  BQ   | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-dc |    Avg    |  QPS  |
+        |:-----------|:----------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:|
+        | Word2Vec   | word2vec                          | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/download.html)                                                                    | 20.00 | 31.49 | 59.46 | 2.57  | 55.78 |  55.04  |  20.70  |   35.03   | 23769 |
+        | SBERT      | xlm-roberta-base                  | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 |  63.01  |  52.28  |   46.46   | 3138  |
+        | Instructor | hfl/chinese-roberta-wwm-ext       | [moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base)                                                                                       | 41.27 | 63.81 | 74.87 | 12.20 | 76.96 |  75.83  |  60.55  |   57.93   | 2980  |
+        | CoSENT     | hfl/chinese-macbert-base          | [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)                                                       | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |  70.27  |  50.42  |   51.61   | 3008  |
+        | CoSENT     | hfl/chinese-lert-large            | [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)                                                   | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 |  73.01  |  59.04  |   53.12   | 2092  |
+        | CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-sentence)                                     | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 |  70.60  |  53.08  |   59.87   | 3089  |
+        | CoSENT     | nghuyong/ernie-3.0-base-zh        | [shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-paraphrase)                                 | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 |  76.70  |  63.30  | **63.08** | 3066  |
         
         
         说明：
-        - 结果值是spearman系数
-        - 结果均只用该数据集的train训练，在test上评估得到的表现，没用外部数据
-        - `shibing624/text2vec-base-chinese`模型，是用CoSENT方法训练，基于`hfl/chinese-macbert-base`在中文STS-B数据训练得到，并在中文STS-B测试集评估达到较好效果，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)，中文通用语义匹配任务推荐使用
-        - `shibing624/text2vec-base-chinese-nli`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用中文NLI数据集[shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)全部语料训练得到，并在中文各NLI测试集评估达到SOTA，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传到huggingface的模型库[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli)，中文s2s(句子vs句子)语义匹配任务推荐使用
+        - 结果评测指标：spearman系数
+        - 模型训练实验报告：[实验报告](https://github.com/shibing624/text2vec/blob/master/docs/model_report.md)
+        - `shibing624/text2vec-base-chinese`模型，是用CoSENT方法训练，基于`hfl/chinese-macbert-base`在中文STS-B数据训练得到，并在中文STS-B测试集评估达到较好效果，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型，模型文件已经上传HF model hub，中文通用语义匹配任务推荐使用
+        - `shibing624/text2vec-base-chinese-sentence`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)训练得到，并在中文各NLI测试集评估达到较好效果，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2s(句子vs句子)语义匹配任务推荐使用
+        - `shibing624/text2vec-base-chinese-paraphrase`模型，是用CoSENT方法训练，基于`nghuyong/ernie-3.0-base-zh`用人工挑选后的中文STS数据集[shibing624/nli-zh-all/text2vec-base-chinese-paraphrase-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-paraphrase-dataset)，数据集相对于[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-dataset)加入了s2p(sentence to paraphrase)数据，强化了其长文本的表征能力，并在中文各NLI测试集评估达到SOTA，运行[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model_jsonl_data.py)代码可训练模型，模型文件已经上传HF model hub，中文s2p(句子vs段落)语义匹配任务推荐使用
         - `SBERT-macbert-base`模型，是用SBERT方法训练，运行[examples/training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/blob/master/examples/training_sup_text_matching_model.py)代码可训练模型
         - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`模型是用SBERT训练，是`paraphrase-MiniLM-L12-v2`模型的多语言版本，支持中文、英文等
         - `w2v-light-tencent-chinese`是腾讯词向量的Word2Vec模型，CPU加载使用，适用于中文字面匹配任务和缺少数据的冷启动情况
         - 各预训练模型均可以通过transformers调用，如MacBERT模型：`--model_name hfl/chinese-macbert-base` 或者roberta模型：`--model_name uer/roberta-medium-wwm-chinese-cluecorpussmall`
-        - 中文匹配数据集下载[链接见下方](#数据集)
+        - 为测评模型的鲁棒性，加入了未训练过的SOHU测试集，用于测试模型的泛化能力；为达到开箱即用的实用效果，使用了搜集到的各中文匹配数据集，数据集也上传到HF datasets[链接见下方](#数据集)
         - 中文匹配任务实验表明，pooling最优是`EncoderType.FIRST_LAST_AVG`和`EncoderType.MEAN`，两者预测效果差异很小
         - 中文匹配评测结果复现，可以下载中文匹配数据集到`examples/data`，运行[tests/test_model_spearman.py](https://github.com/shibing624/text2vec/blob/master/tests/test_model_spearman.py)代码复现评测结果
         - QPS的GPU测试环境是Tesla V100，显存32GB
         
         # Demo
         
         Official Demo: https://www.mulanai.com/product/short_text_sim/
@@ -651,24 +662,25 @@
         ```
         
         
         ## 数据集
         
         - 本项目release的数据集：
         
-        | Dataset               | Introduce                                                           | Download Link                                                                                                                                                                                                                                                                                         |
-        |:----------------------|:--------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | shibing624/nli-zh-all | 中文语义匹配数据合集，整合了文本推理，相似，摘要，问答，指令微调等任务的820万高质量数据，并转化为匹配格式数据集           | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://huggingface.co/datasets/shibing624/nli-zh-all)                                                                                                                                                                                        |
-        | shibing624/snli-zh    | 中文SNLI和MultiNLI数据集，翻译自英文SNLI和MultiNLI                                       | [https://huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/shibing624/snli-zh)                                                                                                                                                                                              |
-        | shibing624/nli_zh     | 中文语义匹配数据集，整合了中文ATEC、BQ、LCQMC、PAWSX、STS-B共5个任务的数据集                   | [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh) </br> or </br> [百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ) </br> or </br> [github](https://github.com/shibing624/text2vec/releases/download/1.1.2/senteval_cn.zip) </br> |
-        | ATEC                  | 中文ATEC数据集，蚂蚁金服Q-Qpair数据集                                            | [ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)                                                                                                                                                                                                                                 |
-        | BQ                    | 中文BQ(Bank Question)数据集，银行Q-Qpair数据集                                 | [BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)                                                                                                                                                                                                                                                     |
-        | LCQMC                 | 中文LCQMC(large-scale Chinese question matching corpus)数据集，Q-Qpair数据集 | [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)                                                                                                                                                                                                                                               |
-        | PAWSX                 | 中文PAWS(Paraphrase Adversaries from Word Scrambling)数据集，Q-Qpair数据集   | [PAWSX](https://arxiv.org/abs/1908.11828)                                                                                                                                                                                                                                                             |
-        | STS-B                 | 中文STS-B数据集，中文自然语言推理数据集，从英文STS-B翻译为中文的数据集                            | [STS-B](https://github.com/pluto-junzeng/CNSD)                                                                                                                                                                                                                                                        |
+        | Dataset                    | Introduce                                                                | Download Link                                                                                                                                                                                                                                                                                         |
+        |:---------------------------|:-------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+        | shibing624/nli-zh-all      | 中文语义匹配数据合集，整合了文本推理，相似，摘要，问答，指令微调等任务的820万高质量数据，并转化为匹配格式数据集                | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://huggingface.co/datasets/shibing624/nli-zh-all)                                                                                                                                                                                        |
+        | shibing624/snli-zh         | 中文SNLI和MultiNLI数据集，翻译自英文SNLI和MultiNLI                                    | [https://huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/shibing624/snli-zh)                                                                                                                                                                                              |
+        | shibing624/nli_zh          | 中文语义匹配数据集，整合了中文ATEC、BQ、LCQMC、PAWSX、STS-B共5个任务的数据集                        | [https://huggingface.co/datasets/shibing624/nli_zh](https://huggingface.co/datasets/shibing624/nli_zh) </br> or </br> [百度网盘(提取码:qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ) </br> or </br> [github](https://github.com/shibing624/text2vec/releases/download/1.1.2/senteval_cn.zip) </br> |
+        | shibing624/sts-sohu2021    | 中文语义匹配数据集，2021搜狐校园文本匹配算法大赛数据集                                            | [https://huggingface.co/datasets/shibing624/sts-sohu2021](https://huggingface.co/datasets/shibing624/sts-sohu2021)                                                                                                                                                                                    |
+        | ATEC                       | 中文ATEC数据集，蚂蚁金服Q-Qpair数据集                                                 | [ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC)                                                                                                                                                                                                                                 |
+        | BQ                         | 中文BQ(Bank Question)数据集，银行Q-Qpair数据集                                      | [BQ](http://icrc.hitsz.edu.cn/info/1037/1162.htm)                                                                                                                                                                                                                                                     |
+        | LCQMC                      | 中文LCQMC(large-scale Chinese question matching corpus)数据集，Q-Qpair数据集      | [LCQMC](http://icrc.hitsz.edu.cn/Article/show/171.html)                                                                                                                                                                                                                                               |
+        | PAWSX                      | 中文PAWS(Paraphrase Adversaries from Word Scrambling)数据集，Q-Qpair数据集        | [PAWSX](https://arxiv.org/abs/1908.11828)                                                                                                                                                                                                                                                             |
+        | STS-B                      | 中文STS-B数据集，中文自然语言推理数据集，从英文STS-B翻译为中文的数据集                                 | [STS-B](https://github.com/pluto-junzeng/CNSD)                                                                                                                                                                                                                                                        |
         
         
         常用英文匹配数据集：
         
         - 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/multi_nli
         - 大名鼎鼎的multi_nli和snli: https://huggingface.co/datasets/snli
         - https://huggingface.co/datasets/metaeval/cnli
@@ -762,14 +774,15 @@
         - [将句子表示为向量（下）：无监督句子表示学习（sentence embedding）](https://www.cnblogs.com/llhthinker/p/10341841.html)
         - [A Simple but Tough-to-Beat Baseline for Sentence Embeddings[Sanjeev Arora and Yingyu Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx)
         - [四种计算文本相似度的方法对比[Yves Peirsman]](https://zhuanlan.zhihu.com/p/37104535)
         - [Improvements to BM25 and Language Models Examined](http://www.cs.otago.ac.nz/homepages/andrew/papers/2014-2.pdf)
         - [CoSENT：比Sentence-BERT更有效的句向量方案](https://kexue.fm/archives/8847)
         - [谈谈文本匹配和多轮检索](https://zhuanlan.zhihu.com/p/111769969)
         - [Sentence-transformers](https://www.sbert.net/examples/applications/computing-embeddings/README.html)
+        - [One Embedder, Any Task: Instruction-Finetuned Text Embeddings](https://arxiv.org/abs/2212.09741)
         
 Keywords: word embedding,text2vec,Chinese Text Similarity Calculation Tool,similarity,word2vec
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: text2vec Version: 1.2.0 Summary: Text to vector
+Metadata-Version: 2.1 Name: text2vec Version: 1.2.1 Summary: Text to vector
 Tool, encode text Home-page: https://github.com/shibing624/text2vec Author:
 XuMing Author-email: xuming624@qq.com License: Apache License 2.0 Description:
 [**ð¨ð³ä¸­æ**](https://github.com/shibing624/text2vec/blob/master/
 README.md) | [**ðEnglish**](https://github.com/shibing624/text2vec/blob/
 master/README_EN.md) | [**ðææ¡£/Docs**](https://github.com/shibing624/
 text2vec/wiki) | [**ð¤æ¨¡å/Models**](https://huggingface.co/shibing624)
                                     [Logo]
@@ -17,18 +17,28 @@
 shibing624/text2vec.svg)](https://github.com/shibing624/text2vec/issues) [!
 [Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/
 wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact) **Text2vec**: Text to
 Vector, Get Sentence Embeddings. ææ¬åéåï¼æææ¬
 (åæ¬è¯ãå¥å­ãæ®µè½)è¡¨å¾ä¸ºåéç©éµã
 **text2vec**å®ç°äºWord2VecãRankBM25ãBERTãSentence-
 BERTãCoSENTç­å¤ç§ææ¬è¡¨å¾ãææ¬ç¸ä¼¼åº¦è®¡ç®æ¨¡åï¼å¹¶å¨ææ¬è¯­ä¹å¹éï¼ç¸ä¼¼åº¦è®¡ç®ï¼ä»»å¡ä¸æ¯è¾äºåæ¨¡åçææã
-### News [2023/06/15] v1.2.0çæ¬: åå¸äºä¸­æå¹éæ¨¡å[shibing624/
-text2vec-base-chinese-nli](https://huggingface.co/shibing624/text2vec-base-
-chinese-nli)ï¼åºäº`nghuyong/ernie-3.0-base-
-zh`æ¨¡åï¼ä½¿ç¨äºä¸­æNLIæ°æ®é[shibing624/nli_zh](https://
+### News [2023/06/19] v1.2.1çæ¬: æ´æ°äºä¸­æå¹éæ¨¡å`shibing624/
+text2vec-base-chinese-nli`ä¸ºæ°ç[shibing624/text2vec-base-chinese-sentence]
+(https://huggingface.co/shibing624/text2vec-base-chinese-
+sentence)ï¼éå¯¹CoSENTçlossè®¡ç®å¯¹æåºææç¹ç¹ï¼äººå·¥æéå¹¶æ´çåºé«è´¨éçæç¸å³æ§æåºçSTSæ°æ®é
+[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
+huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
+sentence-
+dataset)ï¼å¨åè¯ä¼°éè¡¨ç°ç¸å¯¹ä¹åææåï¼åå¸äºéç¨äºs2pçä¸­æå¹éæ¨¡å
+[shibing624/text2vec-base-chinese-paraphrase](https://huggingface.co/
+shibing624/text2vec-base-chinese-paraphrase)ï¼è¯¦è§[Release-v1.2.1](https://
+github.com/shibing624/text2vec/releases/tag/1.2.1) [2023/06/15] v1.2.0çæ¬:
+åå¸äºä¸­æå¹éæ¨¡å[shibing624/text2vec-base-chinese-nli](https://
+huggingface.co/shibing624/text2vec-base-chinese-nli)ï¼åºäº`nghuyong/ernie-
+3.0-base-zh`æ¨¡åï¼ä½¿ç¨äºä¸­æNLIæ°æ®é[shibing624/nli_zh](https://
 huggingface.co/datasets/shibing624/
 nli_zh)å¨é¨è¯­æè®­ç»çCoSENTææ¬å¹éæ¨¡åï¼å¨åè¯ä¼°éè¡¨ç°æåææ¾ï¼è¯¦è§
 [Release-v1.2.0](https://github.com/shibing624/text2vec/releases/tag/1.2.0)
 [2022/03/12] v1.1.4çæ¬: åå¸äºä¸­æå¹éæ¨¡å[shibing624/text2vec-
 base-chinese](https://huggingface.co/shibing624/text2vec-base-
 chinese)ï¼åºäºä¸­æSTSè®­ç»éè®­ç»çCoSENTå¹éæ¨¡åãè¯¦è§
 [Release-v1.1.4](https://github.com/shibing624/text2vec/releases/tag/1.1.4)
@@ -47,88 +57,107 @@
 BERTæ¨¡åçè®­ç»åé¢æµ - [CoSENT(Cosine Sentence)](https://github.com/
 shibing624/text2vec/blob/master/text2vec/
 cosent_model.py)ï¼CoSENTæ¨¡åæåºäºä¸ç§æåºçæå¤±å½æ°ï¼ä½¿è®­ç»è¿ç¨æ´è´´è¿é¢æµï¼æ¨¡åæ¶æéåº¦åæææ¯Sentence-
 BERTæ´å¥½ï¼æ¬é¡¹ç®åºäºPyTorchå®ç°äºCoSENTæ¨¡åçè®­ç»åé¢æµ
 è¯¦ç»ææ¬åéè¡¨ç¤ºæ¹æ³è§wiki: [ææ¬åéè¡¨ç¤ºæ¹æ³](https://
 github.com/shibing624/text2vec/wiki/
 %E6%96%87%E6%9C%AC%E5%90%91%E9%87%8F%E8%A1%A8%E7%A4%BA%E6%96%B9%E6%B3%95) #
-Evaluation ### ææ¬å¹é - è±æå¹éæ°æ®éçè¯æµç»æï¼ | Arch |
-Backbone | Model | English-STS-B | | :-- | :--- | :--- | :-: | | GloVe | glove
-| Avg_word_embeddings_glove_6B_300d | 61.77 | | BERT | bert-base-uncased |
-BERT-base-cls | 20.29 | | BERT | bert-base-uncased | BERT-base-first_last_avg |
-59.04 | | BERT | bert-base-uncased | BERT-base-first_last_avg-whiten(NLI) |
-63.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens | SBERT-base-
-nli-cls | 73.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens |
-SBERT-base-nli-first_last_avg | 77.96 | | SBERT | xlm-roberta-base |
-paraphrase-multilingual-MiniLM-L12-v2 | 84.42 | | CoSENT | bert-base-uncased |
-CoSENT-base-first_last_avg | 69.93 | | CoSENT | sentence-transformers/bert-
-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68 | -
-ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | Backbone | Model | ATEC | BQ |
-LCQMC | PAWSX | STS-B | Avg | QPS | | :-- | :--- | :--- | :-: | :-: | :-: | :-:
-| :-: | :-: | :-: | | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base |
-50.39 | **72.93** | **79.17** | **60.86** | **80.51** | **68.77** | 3008 | |
-CoSENT | Langboat/mengzi-bert-base | CoSENT-mengzi-base | **50.52** | 72.27 |
-78.69 | 12.89 | 80.15 | 58.90 | 2502 | | CoSENT | bert-base-chinese | CoSENT-
-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 80.14 | 68.19 | 2653 | | SBERT |
-bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 | 66.41 |
-61.74 | 3365 | | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28
-| 68.63 | **79.42** | 55.59 | 64.82 | 63.15 | 2948 | | CoSENT | hfl/chinese-
-roberta-wwm-ext | CoSENT-roberta-ext | **50.81** | **71.45** | **79.31** |
-**61.56** | **81.13** | **68.85** | - | | SBERT | hfl/chinese-roberta-wwm-ext |
-SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | - | -
-æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ | Arch | BaseModel | Model
-| ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | QPS | | :-- |:---------------------
---------|:---------------------------------------------------------------------
------------------------------------------------------------------------------|:
------:|:-----:|:-----:|:-----:|:-----:|:---------:|:-----:| | Word2Vec |
+Evaluation ææ¬å¹é #### è±æå¹éæ°æ®éçè¯æµç»æï¼ | Arch |
+BaseModel | Model | English-STS-B | |:-------|:--------------------------------
+----------------|:-------------------------------------|:-------------:| |
+GloVe | glove | Avg_word_embeddings_glove_6B_300d | 61.77 | | BERT | bert-base-
+uncased | BERT-base-cls | 20.29 | | BERT | bert-base-uncased | BERT-base-
+first_last_avg | 59.04 | | BERT | bert-base-uncased | BERT-base-first_last_avg-
+whiten(NLI) | 63.65 | | SBERT | sentence-transformers/bert-base-nli-mean-tokens
+| SBERT-base-nli-cls | 73.65 | | SBERT | sentence-transformers/bert-base-nli-
+mean-tokens | SBERT-base-nli-first_last_avg | 77.96 | | CoSENT | bert-base-
+uncased | CoSENT-base-first_last_avg | 69.93 | | CoSENT | sentence-
+transformers/bert-base-nli-mean-tokens | CoSENT-base-nli-first_last_avg | 79.68
+| #### ä¸­æå¹éæ°æ®éçè¯æµç»æï¼ | Arch | BaseModel | Model |
+ATEC | BQ | LCQMC | PAWSX | STS-B | Avg | |:-------|:--------------------------
+--|:--------------------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:| |
+SBERT | bert-base-chinese | SBERT-bert-base | 46.36 | 70.36 | 78.72 | 46.86 |
+66.41 | 61.74 | | SBERT | hfl/chinese-macbert-base | SBERT-macbert-base | 47.28
+| 68.63 | 79.42 | 55.59 | 64.82 | 63.15 | | SBERT | hfl/chinese-roberta-wwm-ext
+| SBERT-roberta-ext | 48.29 | 69.99 | 79.22 | 44.10 | 72.42 | 62.80 | | CoSENT
+| bert-base-chinese | CoSENT-bert-base | 49.74 | 72.38 | 78.69 | 60.00 | 79.27
+| 68.01 | | CoSENT | hfl/chinese-macbert-base | CoSENT-macbert-base | 50.39 |
+72.93 | 79.17 | 60.86 | 79.30 | 68.53 | | CoSENT | hfl/chinese-roberta-wwm-ext
+| CoSENT-roberta-ext | 50.81 | 71.45 | 79.31 | 61.56 | 79.96 | 68.61 |
+è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
+ä¸ºè¯æµæ¨¡åè½åï¼ç»æååªç¨è¯¥æ°æ®éçtrainè®­ç»ï¼å¨testä¸è¯ä¼°å¾å°çè¡¨ç°ï¼æ²¡ç¨å¤é¨æ°æ®
+### Release Models - æ¬é¡¹ç®releaseæ¨¡åçä¸­æå¹éè¯æµç»æï¼ |
+Arch | BaseModel | Model | ATEC | BQ | LCQMC | PAWSX | STS-B | SOHU-dd | SOHU-
+dc | Avg | QPS | |:-----------|:----------------------------------|:-----------
+-------------------------------------------------------------------------------
+--------------------------------------------------------|:-----:|:-----:|:----
+-:|:-----:|:-----:|:-------:|:-------:|:---------:|:-----:| | Word2Vec |
 word2vec | [w2v-light-tencent-chinese](https://ai.tencent.com/ailab/nlp/en/
-download.html) | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 33.86 | 23769 | | SBERT
-| xlm-roberta-base | [sentence-transformers/paraphrase-multilingual-MiniLM-L12-
-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-
-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90 | 41.99 | 3138 | |
-CoSENT | hfl/chinese-macbert-base | [shibing624/text2vec-base-chinese](https://
-huggingface.co/shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 |
-17.21 | 79.30 | 48.25 | 3008 | | CoSENT | hfl/chinese-lert-large |
+download.html) | 20.00 | 31.49 | 59.46 | 2.57 | 55.78 | 55.04 | 20.70 | 35.03 |
+23769 | | SBERT | xlm-roberta-base | [sentence-transformers/paraphrase-
+multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/
+paraphrase-multilingual-MiniLM-L12-v2) | 18.42 | 38.52 | 63.96 | 10.14 | 78.90
+| 63.01 | 52.28 | 46.46 | 3138 | | Instructor | hfl/chinese-roberta-wwm-ext |
+[moka-ai/m3e-base](https://huggingface.co/moka-ai/m3e-base) | 41.27 | 63.81 |
+74.87 | 12.20 | 76.96 | 75.83 | 60.55 | 57.93 | 2980 | | CoSENT | hfl/chinese-
+macbert-base | [shibing624/text2vec-base-chinese](https://huggingface.co/
+shibing624/text2vec-base-chinese) | 31.93 | 42.67 | 70.16 | 17.21 | 79.30 |
+70.27 | 50.42 | 51.61 | 3008 | | CoSENT | hfl/chinese-lert-large |
 [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/
-text2vec-large-chinese) | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 | 48.08 | 2092
-| | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-base-chinese-
-nli](https://huggingface.co/shibing624/text2vec-base-chinese-nli) | 51.26 |
-68.72 | 79.13 | 34.28 | 80.70 | **62.81** | 3066 | è¯´æï¼ -
-ç»æå¼æ¯spearmanç³»æ° -
-ç»æååªç¨è¯¥æ°æ®éçtrainè®­ç»ï¼å¨testä¸è¯ä¼°å¾å°çè¡¨ç°ï¼æ²¡ç¨å¤é¨æ°æ®
-- `shibing624/text2vec-base-
+text2vec-large-chinese) | 32.61 | 44.59 | 69.30 | 14.51 | 79.44 | 73.01 | 59.04
+| 53.12 | 2092 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-
+base-chinese-sentence](https://huggingface.co/shibing624/text2vec-base-chinese-
+sentence) | 43.37 | 61.43 | 73.48 | 38.90 | 78.25 | 70.60 | 53.08 | 59.87 |
+3089 | | CoSENT | nghuyong/ernie-3.0-base-zh | [shibing624/text2vec-base-
+chinese-paraphrase](https://huggingface.co/shibing624/text2vec-base-chinese-
+paraphrase) | 44.89 | 63.58 | 74.24 | 40.90 | 78.93 | 76.70 | 63.30 | **63.08**
+| 3066 | è¯´æï¼ - ç»æè¯æµææ ï¼spearmanç³»æ° -
+æ¨¡åè®­ç»å®éªæ¥åï¼[å®éªæ¥å](https://github.com/shibing624/
+text2vec/blob/master/docs/model_report.md) - `shibing624/text2vec-base-
 chinese`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`hfl/chinese-macbert-
 base`å¨ä¸­æSTS-Bæ°æ®è®­ç»å¾å°ï¼å¹¶å¨ä¸­æSTS-
 Bæµè¯éè¯ä¼°è¾¾å°è¾å¥½ææï¼è¿è¡[examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/
-training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ å°huggingfaceçæ¨¡ååº
-[shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-
-base-chinese)ï¼ä¸­æéç¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `shibing624/
-text2vec-base-chinese-nli`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`nghuyong/
-ernie-3.0-base-zh`ç¨ä¸­æNLIæ°æ®é[shibing624/nli_zh](https://
-huggingface.co/datasets/shibing624/
-nli_zh)å¨é¨è¯­æè®­ç»å¾å°ï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°SOTAï¼è¿è¡
-[examples/training_sup_text_matching_model.py](https://github.com/shibing624/
-text2vec/blob/master/examples/
-training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ å°huggingfaceçæ¨¡ååº
-[shibing624/text2vec-base-chinese-nli](https://huggingface.co/shibing624/
-text2vec-base-chinese-nli)ï¼ä¸­æs2s
-(å¥å­vså¥å­)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `SBERT-macbert-
-base`æ¨¡åï¼æ¯ç¨SBERTæ¹æ³è®­ç»ï¼è¿è¡[examples/
+training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼ä¸­æéç¨è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `shibing624/text2vec-
+base-chinese-sentence`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`nghuyong/
+ernie-3.0-base-zh`ç¨äººå·¥æéåçä¸­æSTSæ°æ®é[shibing624/nli-zh-
+all/text2vec-base-chinese-sentence-dataset](https://huggingface.co/datasets/
+shibing624/nli-zh-all/tree/main/text2vec-base-chinese-sentence-
+dataset)è®­ç»å¾å°ï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°è¾å¥½ææï¼è¿è¡
+[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
+shibing624/text2vec/blob/master/examples/
+training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼ä¸­æs2s(å¥å­vså¥å­)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ -
+`shibing624/text2vec-base-chinese-
+paraphrase`æ¨¡åï¼æ¯ç¨CoSENTæ¹æ³è®­ç»ï¼åºäº`nghuyong/ernie-3.0-base-
+zh`ç¨äººå·¥æéåçä¸­æSTSæ°æ®é[shibing624/nli-zh-all/text2vec-base-
+chinese-paraphrase-dataset](https://huggingface.co/datasets/shibing624/nli-zh-
+all/tree/main/text2vec-base-chinese-paraphrase-dataset)ï¼æ°æ®éç¸å¯¹äº
+[shibing624/nli-zh-all/text2vec-base-chinese-sentence-dataset](https://
+huggingface.co/datasets/shibing624/nli-zh-all/tree/main/text2vec-base-chinese-
+sentence-dataset)å å¥äºs2p(sentence to
+paraphrase)æ°æ®ï¼å¼ºåäºå¶é¿ææ¬çè¡¨å¾è½åï¼å¹¶å¨ä¸­æåNLIæµè¯éè¯ä¼°è¾¾å°SOTAï¼è¿è¡
+[examples/training_sup_text_matching_model_jsonl_data.py](https://github.com/
+shibing624/text2vec/blob/master/examples/
+training_sup_text_matching_model_jsonl_data.py)ä»£ç å¯è®­ç»æ¨¡åï¼æ¨¡åæä»¶å·²ç»ä¸ä¼ HF
+model hubï¼ä¸­æs2p(å¥å­vsæ®µè½)è¯­ä¹å¹éä»»å¡æ¨èä½¿ç¨ - `SBERT-
+macbert-base`æ¨¡åï¼æ¯ç¨SBERTæ¹æ³è®­ç»ï¼è¿è¡[examples/
 training_sup_text_matching_model.py](https://github.com/shibing624/text2vec/
 blob/master/examples/training_sup_text_matching_model.py)ä»£ç å¯è®­ç»æ¨¡å
 - `sentence-transformers/paraphrase-multilingual-MiniLM-L12-
 v2`æ¨¡åæ¯ç¨SBERTè®­ç»ï¼æ¯`paraphrase-MiniLM-L12-
 v2`æ¨¡åçå¤è¯­è¨çæ¬ï¼æ¯æä¸­æãè±æç­ - `w2v-light-tencent-
 chinese`æ¯è¾è®¯è¯åéçWord2Vecæ¨¡åï¼CPUå è½½ä½¿ç¨ï¼éç¨äºä¸­æå­é¢å¹éä»»å¡åç¼ºå°æ°æ®çå·å¯å¨æåµ
 - åé¢è®­ç»æ¨¡ååå¯ä»¥éè¿transformersè°ç¨ï¼å¦MacBERTæ¨¡åï¼`--
 model_name hfl/chinese-macbert-base` æèrobertaæ¨¡åï¼`--model_name uer/
-roberta-medium-wwm-chinese-cluecorpussmall` - ä¸­æå¹éæ°æ®éä¸è½½
-[é¾æ¥è§ä¸æ¹](#æ°æ®é) -
+roberta-medium-wwm-chinese-cluecorpussmall` -
+ä¸ºæµè¯æ¨¡åçé²æ£æ§ï¼å å¥äºæªè®­ç»è¿çSOHUæµè¯éï¼ç¨äºæµè¯æ¨¡åçæ³åè½åï¼ä¸ºè¾¾å°å¼ç®±å³ç¨çå®ç¨ææï¼ä½¿ç¨äºæéå°çåä¸­æå¹éæ°æ®éï¼æ°æ®éä¹ä¸ä¼ å°HF
+datasets[é¾æ¥è§ä¸æ¹](#æ°æ®é) -
 ä¸­æå¹éä»»å¡å®éªè¡¨æï¼poolingæä¼æ¯`EncoderType.FIRST_LAST_AVG`å`EncoderType.MEAN`ï¼ä¸¤èé¢æµææå·®å¼å¾å°
 -
 ä¸­æå¹éè¯æµç»æå¤ç°ï¼å¯ä»¥ä¸è½½ä¸­æå¹éæ°æ®éå°`examples/
 data`ï¼è¿è¡[tests/test_model_spearman.py](https://github.com/shibing624/
 text2vec/blob/master/tests/test_model_spearman.py)ä»£ç å¤ç°è¯æµç»æ -
 QPSçGPUæµè¯ç¯å¢æ¯Tesla V100ï¼æ¾å­32GB # Demo Official Demo: https://
 www.mulanai.com/product/short_text_sim/ HuggingFace Demo: https://
@@ -402,36 +431,40 @@
 github.com/shibing624/text2vec/blob/master/examples/jina_client_demo.py) ###
 FastAPIæå¡ - å®è£ï¼ ```pip install fastapi uvicorn``` - å¯å¨æå¡ï¼
 example: [examples/fastapi_server_demo.py](https://github.com/shibing624/
 text2vec/blob/master/examples/fastapi_server_demo.py) ```shell cd examples
 python fastapi_server_demo.py ``` - è°ç¨æå¡ï¼ ```shell curl -X 'GET' \
 'http://0.0.0.0:8001/emb?q=hello' \ -H 'accept: application/json' ``` ##
 æ°æ®é - æ¬é¡¹ç®releaseçæ°æ®éï¼ | Dataset | Introduce | Download
-Link | |:----------------------|:----------------------------------------------
-----------------------|:-------------------------------------------------------
+Link | |:---------------------------|:-----------------------------------------
+--------------------------------|:---------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
---| | shibing624/nli-zh-all |
+------------| | shibing624/nli-zh-all |
 ä¸­æè¯­ä¹å¹éæ°æ®åéï¼æ´åäºææ¬æ¨çï¼ç¸ä¼¼ï¼æè¦ï¼é®ç­ï¼æä»¤å¾®è°ç­ä»»å¡ç820ä¸é«è´¨éæ°æ®ï¼å¹¶è½¬åä¸ºå¹éæ ¼å¼æ°æ®é
 | [https://huggingface.co/datasets/shibing624/nli-zh-all](https://
 huggingface.co/datasets/shibing624/nli-zh-all) | | shibing624/snli-zh |
 ä¸­æSNLIåMultiNLIæ°æ®éï¼ç¿»è¯èªè±æSNLIåMultiNLI | [https://
 huggingface.co/datasets/shibing624/snli-zh](https://huggingface.co/datasets/
 shibing624/snli-zh) | | shibing624/nli_zh |
 ä¸­æè¯­ä¹å¹éæ°æ®éï¼æ´åäºä¸­æATECãBQãLCQMCãPAWSXãSTS-
 Bå±5ä¸ªä»»å¡çæ°æ®é | [https://huggingface.co/datasets/shibing624/
 nli_zh](https://huggingface.co/datasets/shibing624/nli_zh)  or  [ç¾åº¦ç½ç
 (æåç :qkt6)](https://pan.baidu.com/s/1d6jSiU1wHQAEMWJi7JJWCQ)  or
 [github](https://github.com/shibing624/text2vec/releases/download/1.1.2/
-senteval_cn.zip)  | | ATEC | ä¸­æATECæ°æ®éï¼èèéæQ-Qpairæ°æ®é
-| [ATEC](https://github.com/IceFlameWorm/NLP_Datasets/tree/master/ATEC) | | BQ
-| ä¸­æBQ(Bank Question)æ°æ®éï¼é¶è¡Q-Qpairæ°æ®é | [BQ](http://
-icrc.hitsz.edu.cn/info/1037/1162.htm) | | LCQMC | ä¸­æLCQMC(large-scale
-Chinese question matching corpus)æ°æ®éï¼Q-Qpairæ°æ®é | [LCQMC](http://
+senteval_cn.zip)  | | shibing624/sts-sohu2021 |
+ä¸­æè¯­ä¹å¹éæ°æ®éï¼2021æçæ ¡å­ææ¬å¹éç®æ³å¤§èµæ°æ®é
+| [https://huggingface.co/datasets/shibing624/sts-sohu2021](https://
+huggingface.co/datasets/shibing624/sts-sohu2021) | | ATEC |
+ä¸­æATECæ°æ®éï¼èèéæQ-Qpairæ°æ®é | [ATEC](https://github.com/
+IceFlameWorm/NLP_Datasets/tree/master/ATEC) | | BQ | ä¸­æBQ(Bank
+Question)æ°æ®éï¼é¶è¡Q-Qpairæ°æ®é | [BQ](http://icrc.hitsz.edu.cn/
+info/1037/1162.htm) | | LCQMC | ä¸­æLCQMC(large-scale Chinese question
+matching corpus)æ°æ®éï¼Q-Qpairæ°æ®é | [LCQMC](http://
 icrc.hitsz.edu.cn/Article/show/171.html) | | PAWSX | ä¸­æPAWS(Paraphrase
 Adversaries from Word Scrambling)æ°æ®éï¼Q-Qpairæ°æ®é | [PAWSX](https:/
 /arxiv.org/abs/1908.11828) | | STS-B | ä¸­æSTS-
 Bæ°æ®éï¼ä¸­æèªç¶è¯­è¨æ¨çæ°æ®éï¼ä»è±æSTS-
 Bç¿»è¯ä¸ºä¸­æçæ°æ®é | [STS-B](https://github.com/pluto-junzeng/CNSD) |
 å¸¸ç¨è±æå¹éæ°æ®éï¼ - å¤§åé¼é¼çmulti_nliåsnli: https://
 huggingface.co/datasets/multi_nli - å¤§åé¼é¼çmulti_nliåsnli: https://
@@ -473,16 +506,17 @@
 Liang and Tengyu Ma, 2017]](https://openreview.net/forum?id=SyK00v5xx) -
 [åç§è®¡ç®ææ¬ç¸ä¼¼åº¦çæ¹æ³å¯¹æ¯[Yves Peirsman]](https://
 zhuanlan.zhihu.com/p/37104535) - [Improvements to BM25 and Language Models
 Examined](http://www.cs.otago.ac.nz/homepages/andrew/papers/2014-2.pdf) -
 [CoSENTï¼æ¯Sentence-BERTæ´ææçå¥åéæ¹æ¡](https://kexue.fm/
 archives/8847) - [è°è°ææ¬å¹éåå¤è½®æ£ç´¢](https://
 zhuanlan.zhihu.com/p/111769969) - [Sentence-transformers](https://
-www.sbert.net/examples/applications/computing-embeddings/README.html) Keywords:
-word embedding,text2vec,Chinese Text Similarity Calculation
-Tool,similarity,word2vec Platform: UNKNOWN Classifier: Development Status :: 5
-- Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Education Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: Apache Software License
+www.sbert.net/examples/applications/computing-embeddings/README.html) - [One
+Embedder, Any Task: Instruction-Finetuned Text Embeddings](https://arxiv.org/
+abs/2212.09741) Keywords: word embedding,text2vec,Chinese Text Similarity
+Calculation Tool,similarity,word2vec Platform: UNKNOWN Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.6.0 Description-Content-Type: text/markdown
```

### Comparing `text2vec-1.2.0/text2vec.egg-info/SOURCES.txt` & `text2vec-1.2.1/text2vec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

