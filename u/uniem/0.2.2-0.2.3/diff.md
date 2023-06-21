# Comparing `tmp/uniem-0.2.2.tar.gz` & `tmp/uniem-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniem-0.2.2.tar", max compression
+gzip compressed data, was "uniem-0.2.3.tar", max compression
```

## Comparing `uniem-0.2.2.tar` & `uniem-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-06-19 08:27:50.354983 uniem-0.2.2/LICENSE
--rw-r--r--   0        0        0     5252 2023-06-19 08:27:50.354983 uniem-0.2.2/README.md
--rw-r--r--   0        0        0      793 2023-06-19 08:27:50.366984 uniem-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      104 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/__init__.py
--rw-r--r--   0        0        0     7166 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/criteria.py
--rw-r--r--   0        0        0    10988 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/data.py
--rw-r--r--   0        0        0     1089 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/data_structures.py
--rw-r--r--   0        0        0    13985 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/finetuner.py
--rw-r--r--   0        0        0    13796 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/model.py
--rw-r--r--   0        0        0     6025 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/trainer.py
--rw-r--r--   0        0        0      658 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/types.py
--rw-r--r--   0        0        0     1663 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/utils.py
--rw-r--r--   0        0        0       22 2023-06-19 08:27:50.470985 uniem-0.2.2/uniem/version.py
--rw-r--r--   0        0        0     5887 1970-01-01 00:00:00.000000 uniem-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-21 03:51:44.156512 uniem-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5876 2023-06-21 03:51:44.156512 uniem-0.2.3/README.md
+-rw-r--r--   0        0        0      793 2023-06-21 03:51:44.168511 uniem-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/__init__.py
+-rw-r--r--   0        0        0     7166 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/criteria.py
+-rw-r--r--   0        0        0    10992 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/data.py
+-rw-r--r--   0        0        0     1109 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/data_structures.py
+-rw-r--r--   0        0        0    14138 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/finetuner.py
+-rw-r--r--   0        0        0    13796 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/model.py
+-rw-r--r--   0        0        0     6025 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/trainer.py
+-rw-r--r--   0        0        0      658 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/types.py
+-rw-r--r--   0        0        0     1663 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/utils.py
+-rw-r--r--   0        0        0       22 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/version.py
+-rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 uniem-0.2.3/PKG-INFO
```

### Comparing `uniem-0.2.2/LICENSE` & `uniem-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uniem-0.2.2/README.md` & `uniem-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # uniem
+[![Release](https://img.shields.io/pypi/v/uniem)](https://pypi.org/project/uniem/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/uniem)
+[![ci](https://github.com/wangyuxinwhy/uniem/actions/workflows/ci.yml/badge.svg)](https://github.com/wangyuxinwhy/uniem/actions/workflows/ci.yml)
+[![cd](https://github.com/wangyuxinwhy/uniem/actions/workflows/cd.yml/badge.svg)](https://github.com/wangyuxinwhy/uniem/actions/workflows/cd.yml)
 
 uniem 项目的目标是创建中文最好的通用文本嵌入模型。
 
 本项目主要包括模型的训练，微调和评测代码，模型与数据集会在 [HuggingFace](https://huggingface.co/) 社区上进行开源。
 
 ## 🌟 重要更新
 
@@ -54,37 +58,37 @@
 
 
 ### 文本分类
 
 - 数据集选择，选择开源在 HuggingFace 上的 6 种文本分类数据集，包括新闻、电商评论、股票评论、长文本等
 - 评测方式，使用 MTEB 的方式进行评测，报告 Accuracy。
 
-|                   | text2vec | m3e-small | m3e-base | openai | DMetaSoul   | uer     | erlangshen  |
-| ----------------- | -------- | --------- | -------- | ------ | ----------- | ------- | ----------- |
-| TNews             | 0.43     | 0.4443    | **0.4827**   | 0.4594 | 0.3084      | 0.3539  | 0.4361      |
-| JDIphone          | 0.8214   | 0.8293    | **0.8533**   | 0.746  | 0.7972      | 0.8283  | 0.8356      |
-| GubaEastmony      | 0.7472   | 0.712     | 0.7621   | 0.7574 | 0.735       | 0.7534  | **0.7787**      |
-| TYQSentiment      | 0.6099   | 0.6596    | **0.7188**   | 0.68   | 0.6437      | 0.6662  | 0.6444      |
-| StockComSentiment | 0.4307   | 0.4291    | 0.4363   | **0.4819** | 0.4309      | 0.4555  | 0.4482      |
-| IFlyTek           | 0.414    | 0.4263    | 0.4409   | **0.4486** | 0.3969      | 0.3762  | 0.4241      |
-| Average           | 0.5755   | 0.5834    | **0.6157**   | 0.5956 | 0.552016667 | 0.57225 | 0.594516667 |
+|                   | text2vec | m3e-small | m3e-base | m3e-large-0619 | openai | DMetaSoul   | uer     | erlangshen  |
+| ----------------- | -------- | --------- | -------- | ------ | ----------- | ------- | ----------- | ----------- |
+| TNews             | 0.43     | 0.4443    | 0.4827   | **0.4866** | 0.4594 | 0.3084      | 0.3539  | 0.4361      |
+| JDIphone          | 0.8214   | 0.8293    | 0.8533   | **0.8692** | 0.746  | 0.7972      | 0.8283  | 0.8356      |
+| GubaEastmony      | 0.7472   | 0.712     | 0.7621   | 0.7663 | 0.7574 | 0.735       | 0.7534  | **0.7787**      |
+| TYQSentiment      | 0.6099   | 0.6596    | 0.7188   | **0.7247** | 0.68   | 0.6437      | 0.6662  | 0.6444      |
+| StockComSentiment | 0.4307   | 0.4291    | 0.4363   | 0.4475 | **0.4819** | 0.4309      | 0.4555  | 0.4482      |
+| IFlyTek           | 0.414    | 0.4263    | 0.4409   | 0.4445 | **0.4486** | 0.3969      | 0.3762  | 0.4241      |
+| Average           | 0.5755   | 0.5834    | 0.6157   | **0.6231** | 0.5956 | 0.552016667 | 0.57225 | 0.594516667 |
 
 ### 检索排序
 
 - 数据集选择，使用 [T2Ranking](https://github.com/THUIR/T2Ranking/tree/main) 数据集，由于 T2Ranking 的数据集太大，openai 评测起来的时间成本和 api 费用有些高，所以我们只选择了 T2Ranking 中的前 10000 篇文章
 - 评测方式，使用 MTEB 的方式进行评测，报告 map@1, map@10, mrr@1, mrr@10, ndcg@1, ndcg@10
 
-|         | text2vec | openai-ada-002 | m3e-small | m3e-base | DMetaSoul | uer     | erlangshen |
-| ------- | -------- | -------------- | --------- | -------- | --------- | ------- | ---------- |
-| map@1   | 0.4684   | 0.6133         | 0.5574    | **0.626**    | 0.25203   | 0.08647 | 0.25394    |
-| map@10  | 0.5877   | 0.7423         | 0.6878    | **0.7656**   | 0.33312   | 0.13008 | 0.34714    |
-| mrr@1   | 0.5345   | 0.6931         | 0.6324    | **0.7047**   | 0.29258   | 0.10067 | 0.29447    |
-| mrr@10  | 0.6217   | 0.7668         | 0.712     | **0.7841**   | 0.36287   | 0.14516 | 0.3751     |
-| ndcg@1  | 0.5207   | 0.6764         | 0.6159    | **0.6881**   | 0.28358   | 0.09748 | 0.28578    |
-| ndcg@10 | 0.6346   | 0.7786         | 0.7262    | **0.8004**   | 0.37468   | 0.15783 | 0.39329    |
+|         | text2vec | openai-ada-002 | m3e-small | m3e-base | m3e-large-0619 | DMetaSoul | uer     | erlangshen |
+| ------- | -------- | -------------- | --------- | -------- | --------- | ------- | ---------- | ---------- |
+| map@1   | 0.4684   | 0.6133         | 0.5574    | **0.626**    | 0.6256 | 0.25203   | 0.08647 | 0.25394    |
+| map@10  | 0.5877   | 0.7423         | 0.6878    | **0.7656**   | 0.7627 | 0.33312   | 0.13008 | 0.34714    |
+| mrr@1   | 0.5345   | 0.6931         | 0.6324    | 0.7047   | **0.7063** | 0.29258   | 0.10067 | 0.29447    |
+| mrr@10  | 0.6217   | 0.7668         | 0.712     | **0.7841**   | 0.7827 | 0.36287   | 0.14516 | 0.3751     |
+| ndcg@1  | 0.5207   | 0.6764         | 0.6159    | 0.6881   | **0.6884** | 0.28358   | 0.09748 | 0.28578    |
+| ndcg@10 | 0.6346   | 0.7786         | 0.7262    | **0.8004**   | 0.7974 | 0.37468   | 0.15783 | 0.39329    |
 
 ## 🤝 Contributing
 
 如果您想要在 MTEB-zh 中添加评测数据集或者模型，欢迎提 issue 或者 PR，我会在第一时间进行支持，期待您的贡献！
 
 ## 📜 License
```

### Comparing `uniem-0.2.2/pyproject.toml` & `uniem-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniem"
-version = "0.2.2"
+version = "0.2.3"
 description = "unified embedding model"
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `uniem-0.2.2/uniem/criteria.py` & `uniem-0.2.3/uniem/criteria.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.2/uniem/data.py` & `uniem-0.2.3/uniem/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from torch.utils.data import Dataset, RandomSampler
 
 from uniem.data_structures import (
     PairRecord,
     RecordType,
     ScoredPairRecord,
     TripletRecord,
-    get_record_type,
+    infer_record_type,
     record_type_cls_map,
 )
 from uniem.types import Tokenizer
 
 
 class PairCollator:
     def __init__(self, tokenizer: Tokenizer, max_length: int | None = None) -> None:
@@ -136,15 +136,15 @@
         dataset: HfDataset | Sequence[dict],
         record_type: RecordType | str | None = None,
     ) -> None:
         self.dataset = dataset
         if record_type:
             self.record_type = RecordType(record_type)
         else:
-            self.record_type = get_record_type(dataset[0])
+            self.record_type = infer_record_type(dataset[0])
         self.record_cls = record_type_cls_map[self.record_type]
 
     def __getitem__(self, index: int):
         record = self.dataset[index]
         return self.record_cls(**record)
 
     def __len__(self):
```

### Comparing `uniem-0.2.2/uniem/data_structures.py` & `uniem-0.2.3/uniem/data_structures.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,22 +25,23 @@
 @dataclass(slots=True)
 class ScoredPairRecord:
     sentence1: str
     sentence2: str
     label: float
 
 
+# * Order matters
 record_type_cls_map: dict[RecordType, Any] = {
-    RecordType.PAIR: PairRecord,
-    RecordType.TRIPLET: TripletRecord,
     RecordType.SCORED_PAIR: ScoredPairRecord,
+    RecordType.TRIPLET: TripletRecord,
+    RecordType.PAIR: PairRecord,
 }
 
 
-def get_record_type(record: dict) -> RecordType:
+def infer_record_type(record: dict) -> RecordType:
     record_type_field_names_map = {
         record_type: [field.name for field in fields(record_cls)] for record_type, record_cls in record_type_cls_map.items()
     }
     for record_type, field_names in record_type_field_names_map.items():
         if all(field_name in record for field_name in field_names):
             return record_type
     raise ValueError(f'Unknown record type, record: {record}')
```

### Comparing `uniem-0.2.2/uniem/finetuner.py` & `uniem-0.2.3/uniem/finetuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from uniem.data import (
     FinetuneDataset,
     PairCollator,
     PrefixFinetuneDataset,
     ScoredPairCollator,
     TripletCollator,
 )
-from uniem.data_structures import RecordType, get_record_type
+from uniem.data_structures import RecordType, infer_record_type
 from uniem.model import (
     EmbedderForPairInBatchNegTrain,
     EmbedderForScoredPairTrain,
     EmbedderForTrain,
     EmbedderForTripletInBatchNegTrain,
     InBatchNegLossType,
     PoolingStrategy,
@@ -37,28 +37,32 @@
 
 
 class FineTuner:
     def __init__(
         self,
         model_name_or_path: str,
         dataset: RawDataset,
+        record_type: RecordType | str | None = None,
     ):
         self.model_name_or_path = model_name_or_path
         self.raw_dataset = dataset
         if isinstance(self.raw_dataset, dict):
             (
                 self.raw_train_dataset,
                 self.raw_validation_dataset,
             ) = split_dataset_dict(self.raw_dataset)
         else:
             self.raw_train_dataset, self.raw_validation_dataset = (
                 self.raw_dataset,
                 None,
             )
-        self.record_type = get_record_type(self.raw_train_dataset[0])  # type: ignore
+
+        record_type = RecordType(record_type) if isinstance(record_type, str) else record_type
+        self.record_type = record_type or infer_record_type(self.raw_train_dataset[0])
+
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_name_or_path)
 
     def create_finetune_datasets(
         self,
     ) -> tuple[FinetuneDataset, FinetuneDataset | None]:
         train_dataset = FinetuneDataset(self.raw_train_dataset)
         validation_dataset = FinetuneDataset(self.raw_validation_dataset) if self.raw_validation_dataset is not None else None
```

### Comparing `uniem-0.2.2/uniem/model.py` & `uniem-0.2.3/uniem/model.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.2/uniem/trainer.py` & `uniem-0.2.3/uniem/trainer.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.2/uniem/types.py` & `uniem-0.2.3/uniem/types.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.2/uniem/utils.py` & `uniem-0.2.3/uniem/utils.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.2/PKG-INFO` & `uniem-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniem
-Version: 0.2.2
+Version: 0.2.3
 Summary: unified embedding model
 License: MIT
 Author: wangyuxin
 Author-email: wangyuxin@mokahr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,18 @@
 Requires-Dist: datasets (>=2.12.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: transformers (>=4.28.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # uniem
+[![Release](https://img.shields.io/pypi/v/uniem)](https://pypi.org/project/uniem/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/uniem)
+[![ci](https://github.com/wangyuxinwhy/uniem/actions/workflows/ci.yml/badge.svg)](https://github.com/wangyuxinwhy/uniem/actions/workflows/ci.yml)
+[![cd](https://github.com/wangyuxinwhy/uniem/actions/workflows/cd.yml/badge.svg)](https://github.com/wangyuxinwhy/uniem/actions/workflows/cd.yml)
 
 uniem 项目的目标是创建中文最好的通用文本嵌入模型。
 
 本项目主要包括模型的训练，微调和评测代码，模型与数据集会在 [HuggingFace](https://huggingface.co/) 社区上进行开源。
 
 ## 🌟 重要更新
 
@@ -73,37 +77,37 @@
 
 
 ### 文本分类
 
 - 数据集选择，选择开源在 HuggingFace 上的 6 种文本分类数据集，包括新闻、电商评论、股票评论、长文本等
 - 评测方式，使用 MTEB 的方式进行评测，报告 Accuracy。
 
-|                   | text2vec | m3e-small | m3e-base | openai | DMetaSoul   | uer     | erlangshen  |
-| ----------------- | -------- | --------- | -------- | ------ | ----------- | ------- | ----------- |
-| TNews             | 0.43     | 0.4443    | **0.4827**   | 0.4594 | 0.3084      | 0.3539  | 0.4361      |
-| JDIphone          | 0.8214   | 0.8293    | **0.8533**   | 0.746  | 0.7972      | 0.8283  | 0.8356      |
-| GubaEastmony      | 0.7472   | 0.712     | 0.7621   | 0.7574 | 0.735       | 0.7534  | **0.7787**      |
-| TYQSentiment      | 0.6099   | 0.6596    | **0.7188**   | 0.68   | 0.6437      | 0.6662  | 0.6444      |
-| StockComSentiment | 0.4307   | 0.4291    | 0.4363   | **0.4819** | 0.4309      | 0.4555  | 0.4482      |
-| IFlyTek           | 0.414    | 0.4263    | 0.4409   | **0.4486** | 0.3969      | 0.3762  | 0.4241      |
-| Average           | 0.5755   | 0.5834    | **0.6157**   | 0.5956 | 0.552016667 | 0.57225 | 0.594516667 |
+|                   | text2vec | m3e-small | m3e-base | m3e-large-0619 | openai | DMetaSoul   | uer     | erlangshen  |
+| ----------------- | -------- | --------- | -------- | ------ | ----------- | ------- | ----------- | ----------- |
+| TNews             | 0.43     | 0.4443    | 0.4827   | **0.4866** | 0.4594 | 0.3084      | 0.3539  | 0.4361      |
+| JDIphone          | 0.8214   | 0.8293    | 0.8533   | **0.8692** | 0.746  | 0.7972      | 0.8283  | 0.8356      |
+| GubaEastmony      | 0.7472   | 0.712     | 0.7621   | 0.7663 | 0.7574 | 0.735       | 0.7534  | **0.7787**      |
+| TYQSentiment      | 0.6099   | 0.6596    | 0.7188   | **0.7247** | 0.68   | 0.6437      | 0.6662  | 0.6444      |
+| StockComSentiment | 0.4307   | 0.4291    | 0.4363   | 0.4475 | **0.4819** | 0.4309      | 0.4555  | 0.4482      |
+| IFlyTek           | 0.414    | 0.4263    | 0.4409   | 0.4445 | **0.4486** | 0.3969      | 0.3762  | 0.4241      |
+| Average           | 0.5755   | 0.5834    | 0.6157   | **0.6231** | 0.5956 | 0.552016667 | 0.57225 | 0.594516667 |
 
 ### 检索排序
 
 - 数据集选择，使用 [T2Ranking](https://github.com/THUIR/T2Ranking/tree/main) 数据集，由于 T2Ranking 的数据集太大，openai 评测起来的时间成本和 api 费用有些高，所以我们只选择了 T2Ranking 中的前 10000 篇文章
 - 评测方式，使用 MTEB 的方式进行评测，报告 map@1, map@10, mrr@1, mrr@10, ndcg@1, ndcg@10
 
-|         | text2vec | openai-ada-002 | m3e-small | m3e-base | DMetaSoul | uer     | erlangshen |
-| ------- | -------- | -------------- | --------- | -------- | --------- | ------- | ---------- |
-| map@1   | 0.4684   | 0.6133         | 0.5574    | **0.626**    | 0.25203   | 0.08647 | 0.25394    |
-| map@10  | 0.5877   | 0.7423         | 0.6878    | **0.7656**   | 0.33312   | 0.13008 | 0.34714    |
-| mrr@1   | 0.5345   | 0.6931         | 0.6324    | **0.7047**   | 0.29258   | 0.10067 | 0.29447    |
-| mrr@10  | 0.6217   | 0.7668         | 0.712     | **0.7841**   | 0.36287   | 0.14516 | 0.3751     |
-| ndcg@1  | 0.5207   | 0.6764         | 0.6159    | **0.6881**   | 0.28358   | 0.09748 | 0.28578    |
-| ndcg@10 | 0.6346   | 0.7786         | 0.7262    | **0.8004**   | 0.37468   | 0.15783 | 0.39329    |
+|         | text2vec | openai-ada-002 | m3e-small | m3e-base | m3e-large-0619 | DMetaSoul | uer     | erlangshen |
+| ------- | -------- | -------------- | --------- | -------- | --------- | ------- | ---------- | ---------- |
+| map@1   | 0.4684   | 0.6133         | 0.5574    | **0.626**    | 0.6256 | 0.25203   | 0.08647 | 0.25394    |
+| map@10  | 0.5877   | 0.7423         | 0.6878    | **0.7656**   | 0.7627 | 0.33312   | 0.13008 | 0.34714    |
+| mrr@1   | 0.5345   | 0.6931         | 0.6324    | 0.7047   | **0.7063** | 0.29258   | 0.10067 | 0.29447    |
+| mrr@10  | 0.6217   | 0.7668         | 0.712     | **0.7841**   | 0.7827 | 0.36287   | 0.14516 | 0.3751     |
+| ndcg@1  | 0.5207   | 0.6764         | 0.6159    | 0.6881   | **0.6884** | 0.28358   | 0.09748 | 0.28578    |
+| ndcg@10 | 0.6346   | 0.7786         | 0.7262    | **0.8004**   | 0.7974 | 0.37468   | 0.15783 | 0.39329    |
 
 ## 🤝 Contributing
 
 如果您想要在 MTEB-zh 中添加评测数据集或者模型，欢迎提 issue 或者 PR，我会在第一时间进行支持，期待您的贡献！
 
 ## 📜 License
```

