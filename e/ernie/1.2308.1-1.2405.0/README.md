# Comparing `tmp/ernie-1.2308.1-py3-none-any.whl.zip` & `tmp/ernie-1.2405.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 18196 bytes, number of entries: 17
--rw-rw-r--  2.0 unx     1061 b- defN 23-Aug-04 07:32 ernie/__init__.py
--rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-31 18:23 ernie/aggregation_strategies.py
--rw-rw-r--  2.0 unx    13420 b- defN 23-Aug-04 07:09 ernie/ernie.py
--rw-rw-r--  2.0 unx     3026 b- defN 23-Aug-02 05:33 ernie/helper.py
--rw-rw-r--  2.0 unx     1758 b- defN 23-Jul-31 18:23 ernie/models.py
--rw-rw-r--  2.0 unx     4314 b- defN 23-Jul-31 18:23 ernie/split_strategies.py
--rw-rw-r--  2.0 unx       87 b- defN 23-Jul-31 18:24 test/__init__.py
--rw-rw-r--  2.0 unx     1414 b- defN 23-Jul-31 18:24 test/dump_load.py
--rw-rw-r--  2.0 unx      775 b- defN 23-Jul-31 18:24 test/load_csv.py
--rw-rw-r--  2.0 unx      973 b- defN 23-Jul-31 18:24 test/load_model.py
--rw-rw-r--  2.0 unx      714 b- defN 23-Jul-31 18:25 test/predict.py
--rw-rw-r--  2.0 unx    18131 b- defN 23-Jul-31 18:26 test/split_aggregate.py
--rw-rw-r--  2.0 unx    11358 b- defN 23-Aug-04 07:57 ernie-1.2308.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1016 b- defN 23-Aug-04 07:57 ernie-1.2308.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Aug-04 07:57 ernie-1.2308.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Aug-04 07:57 ernie-1.2308.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1295 b- defN 23-Aug-04 07:57 ernie-1.2308.1.dist-info/RECORD
-17 files, 61379 bytes uncompressed, 16110 bytes compressed:  73.8%
+Zip file size: 18157 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     1064 b- defN 24-Apr-30 23:17 ernie/__init__.py
+-rw-r--r--  2.0 unx     2068 b- defN 24-Apr-30 23:17 ernie/aggregation_strategies.py
+-rw-r--r--  2.0 unx    13843 b- defN 24-Apr-30 23:17 ernie/ernie.py
+-rw-r--r--  2.0 unx     3076 b- defN 24-Apr-30 23:17 ernie/helper.py
+-rw-r--r--  2.0 unx     1913 b- defN 24-Apr-30 23:17 ernie/models.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-Apr-30 23:17 ernie/split_strategies.py
+-rw-r--r--  2.0 unx       87 b- defN 24-Apr-25 15:26 test/__init__.py
+-rw-r--r--  2.0 unx     1414 b- defN 24-Apr-25 15:26 test/dump_load.py
+-rw-r--r--  2.0 unx      775 b- defN 24-Apr-25 15:26 test/load_csv.py
+-rw-r--r--  2.0 unx      973 b- defN 24-Apr-25 15:26 test/load_model.py
+-rw-r--r--  2.0 unx      714 b- defN 24-Apr-25 15:26 test/predict.py
+-rw-r--r--  2.0 unx    18131 b- defN 24-Apr-25 15:26 test/split_aggregate.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-Apr-30 23:40 ernie-1.2405.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      926 b- defN 24-Apr-30 23:40 ernie-1.2405.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 23:40 ernie-1.2405.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 24-Apr-30 23:40 ernie-1.2405.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1294 b- defN 24-Apr-30 23:40 ernie-1.2405.0.dist-info/RECORD
+17 files, 62251 bytes uncompressed, 16071 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: test/predict.py
 Comment: 
 
 Filename: test/split_aggregate.py
 Comment: 
 
-Filename: ernie-1.2308.1.dist-info/LICENSE
+Filename: ernie-1.2405.0.dist-info/LICENSE
 Comment: 
 
-Filename: ernie-1.2308.1.dist-info/METADATA
+Filename: ernie-1.2405.0.dist-info/METADATA
 Comment: 
 
-Filename: ernie-1.2308.1.dist-info/WHEEL
+Filename: ernie-1.2405.0.dist-info/WHEEL
 Comment: 
 
-Filename: ernie-1.2308.1.dist-info/top_level.txt
+Filename: ernie-1.2405.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ernie-1.2308.1.dist-info/RECORD
+Filename: ernie-1.2405.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ernie/__init__.py

```diff
@@ -1,39 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from .ernie import *  # noqa: F401, F403
-from tensorflow.python.client import device_lib
 import logging
 
-__version__ = '1.2308.1'
+from tensorflow.python.client import device_lib
+
+from .ernie import *  # noqa: F401, F403
+
+__version__ = '1.2405.0'
 
 logging.getLogger().setLevel(logging.WARNING)
-logging.getLogger("transformers.tokenization_utils").setLevel(logging.ERROR)
+logging.getLogger('transformers.tokenization_utils').setLevel(logging.ERROR)
 logging.basicConfig(
     format='%(asctime)-15s [%(levelname)s] %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S'
 )
 
 
 def _get_cpu_name():
     import cpuinfo
     cpu_info = cpuinfo.get_cpu_info()
     cpu_name = f"{cpu_info['brand_raw']}, {cpu_info['count']} vCores"
     return cpu_name
 
 
 def _get_gpu_name():
-    gpu_name = \
-        device_lib\
-        .list_local_devices()[3]\
-        .physical_device_desc\
-        .split(',')[1]\
-        .split('name:')[1]\
+    gpu_name = (
+        device_lib
+        .list_local_devices()[3]
+        .physical_device_desc
+        .split(',')[1]
+        .split('name:')[1]
         .strip()
+    )
     return gpu_name
 
 
 device_name = _get_cpu_name()
 device_type = 'CPU'
 
 try:
```

## ernie/aggregation_strategies.py

```diff
@@ -1,16 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from statistics import mean
 
 
 class AggregationStrategy:
+
     def __init__(
-        self, method, max_items=None, top_items=True, sorting_class_index=1
+        self,
+        method,
+        max_items=None,
+        top_items=True,
+        sorting_class_index=1,
     ):
         self.method = method
         self.max_items = max_items
         self.top_items = top_items
         self.sorting_class_index = sorting_class_index
 
     def aggregate(self, softmax_tuples):
@@ -40,18 +45,30 @@
         softmax_tuple = tuple(softmax_list)
         return softmax_tuple
 
 
 class AggregationStrategies:
     Mean = AggregationStrategy(method=mean)
     MeanTopFiveBinaryClassification = AggregationStrategy(
-        method=mean, max_items=5, top_items=True, sorting_class_index=1
+        method=mean,
+        max_items=5,
+        top_items=True,
+        sorting_class_index=1,
     )
     MeanTopTenBinaryClassification = AggregationStrategy(
-        method=mean, max_items=10, top_items=True, sorting_class_index=1
+        method=mean,
+        max_items=10,
+        top_items=True,
+        sorting_class_index=1,
     )
     MeanTopFifteenBinaryClassification = AggregationStrategy(
-        method=mean, max_items=15, top_items=True, sorting_class_index=1
+        method=mean,
+        max_items=15,
+        top_items=True,
+        sorting_class_index=1,
     )
     MeanTopTwentyBinaryClassification = AggregationStrategy(
-        method=mean, max_items=20, top_items=True, sorting_class_index=1
+        method=mean,
+        max_items=20,
+        top_items=True,
+        sorting_class_index=1,
     )
```

## ernie/ernie.py

```diff
@@ -1,42 +1,36 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+import logging
+import time
+
 import numpy as np
 import pandas as pd
-from transformers import (
-    AutoTokenizer,
-    AutoModel,
-    AutoConfig,
-    TFAutoModelForSequenceClassification,
-)
-from tensorflow import keras
+import tf_keras as keras
 from sklearn.model_selection import train_test_split
-import logging
-import time
+from transformers import (AutoConfig, AutoModel, AutoTokenizer,
+                          TFAutoModelForSequenceClassification)
+
+from .aggregation_strategies import AggregationStrategies  # noqa: F401
+from .aggregation_strategies import AggregationStrategy
+from .helper import copy_dir, get_features, make_dir, remove_dir, softmax
 from .models import Models, ModelsByFamily  # noqa: F401
-from .split_strategies import (  # noqa: F401
-    SplitStrategy,
-    SplitStrategies,
-    RegexExpressions
-)
-from .aggregation_strategies import (  # noqa: F401
-    AggregationStrategy,
-    AggregationStrategies
-)
-from .helper import (get_features, softmax, remove_dir, make_dir, copy_dir)
+from .split_strategies import (RegexExpressions, SplitStrategies,  # noqa: F401
+                               SplitStrategy)
 
 AUTOSAVE_PATH = './ernie-autosave/'
 
 
 def clean_autosave():
     remove_dir(AUTOSAVE_PATH)
 
 
 class SentenceClassifier:
+
     def __init__(
         self,
         model_name=Models.BertBaseUncased,
         model_path=None,
         max_length=64,
         labels_no=2,
         tokenizer_kwargs=None,
@@ -86,33 +80,39 @@
         if csv_path is not None:
             dataframe = pd.read_csv(csv_path, **read_csv_kwargs)
 
         sentences = list(dataframe[dataframe.columns[0]])
         labels = dataframe[dataframe.columns[1]].values
 
         (
-            training_sentences, validation_sentences, training_labels,
-            validation_labels
+            training_sentences,
+            validation_sentences,
+            training_labels,
+            validation_labels,
         ) = train_test_split(
             sentences,
             labels,
             test_size=validation_split,
             shuffle=True,
             random_state=random_state,
-            stratify=stratify
+            stratify=stratify,
         )
 
         self._training_features = get_features(
-            self._tokenizer, training_sentences, training_labels
+            self._tokenizer,
+            training_sentences,
+            training_labels,
         )
 
         self._training_size = len(training_sentences)
 
         self._validation_features = get_features(
-            self._tokenizer, validation_sentences, validation_labels
+            self._tokenizer,
+            validation_sentences,
+            validation_labels,
         )
         self._validation_split = len(validation_sentences)
 
         logging.info(f'training_size: {self._training_size}')
         logging.info(f'validation_split: {self._validation_split}')
 
         self._loaded_data = True
@@ -136,27 +136,31 @@
         if not self._loaded_data:
             raise Exception('Data has not been loaded.')
 
         if optimizer_kwargs is None:
             optimizer_kwargs = {
                 'learning_rate': learning_rate,
                 'epsilon': epsilon,
-                'clipnorm': clipnorm
+                'clipnorm': clipnorm,
             }
         optimizer = optimizer_function(**optimizer_kwargs)
 
         if loss_kwargs is None:
             loss_kwargs = {'from_logits': True}
         loss = loss_function(**loss_kwargs)
 
         if accuracy_kwargs is None:
             accuracy_kwargs = {'name': 'accuracy'}
         accuracy = accuracy_function(**accuracy_kwargs)
 
-        self._model.compile(optimizer=optimizer, loss=loss, metrics=[accuracy])
+        self._model.compile(
+            optimizer=optimizer,
+            loss=loss,
+            metrics=[accuracy],
+        )
 
         training_features = self._training_features.shuffle(
             self._training_size
         ).batch(training_batch_size).repeat(-1)
         validation_features = self._validation_features.batch(
             validation_batch_size
         )
@@ -174,15 +178,15 @@
         for i in range(epochs):
             self._model.fit(
                 training_features,
                 epochs=1,
                 validation_data=validation_features,
                 steps_per_epoch=training_steps,
                 validation_steps=validation_steps,
-                **kwargs
+                **kwargs,
             )
 
         # The fine-tuned model does not have the same input interface
         # after being exported and loaded again.
         self._reload_model()
 
     def predict_one(
@@ -253,16 +257,18 @@
             batch_size = sentences_number
 
         for i in range(0, sentences_number, batch_size):
             input_ids_list = []
             attention_mask_list = []
 
             stop_index = i + batch_size
-            stop_index = stop_index if stop_index < sentences_number \
-                else sentences_number
+            stop_index = (
+                stop_index
+                if stop_index < sentences_number else sentences_number
+            )
 
             for j in range(i, stop_index):
                 features = self._tokenizer.encode_plus(
                     sentences[j],
                     add_special_tokens=True,
                     max_length=self._tokenizer.model_max_length,
                 )
@@ -328,15 +334,16 @@
             )
 
         # Old models didn't use to have a tokenizer folder
         except OSError:
             self._tokenizer = AutoTokenizer.from_pretrained(model_path)
             self._config = AutoConfig.from_pretrained(model_path)
         self._model = TFAutoModelForSequenceClassification.from_pretrained(
-            model_path, from_pt=False
+            model_path,
+            from_pt=False,
         )
 
     def _get_model_family(self):
         model_family = ''.join(self._model.name[2:].split('_')[:2])
         return model_family
 
     def _load_remote_model(
@@ -365,61 +372,71 @@
                 model_name,
                 from_pt=False,
             )
 
         # PyTorch model
         except OSError:
             try:
-                self._model = \
+                self._model = (
                     TFAutoModelForSequenceClassification.from_pretrained(
                         model_name,
-                        from_pt=True
+                        from_pt=True,
                     )
+                )
 
             # Loading a TF model from a PyTorch checkpoint is not supported
             # when using a model identifier name
             except OSError:
                 model = AutoModel.from_pretrained(model_name)
                 model.save_pretrained(temporary_path)
-                self._model = \
+                self._model = (
                     TFAutoModelForSequenceClassification.from_pretrained(
                         temporary_path,
-                        from_pt=True
+                        from_pt=True,
                     )
+                )
 
         # Clean the model's last layer if the provided properties are different
         clean_last_layer = False
         for key, value in model_kwargs.items():
             if not hasattr(self._model.config, key):
                 clean_last_layer = True
                 break
 
             if getattr(self._model.config, key) != value:
                 clean_last_layer = True
                 break
 
         if clean_last_layer:
             try:
-                getattr(self._model, self._get_model_family()
-                        ).save_pretrained(temporary_path)
+                getattr(
+                    self._model,
+                    self._get_model_family(),
+                ).save_pretrained(temporary_path)
                 self._model = self._model.__class__.from_pretrained(
-                    temporary_path, from_pt=False, **model_kwargs
+                    temporary_path,
+                    from_pt=False,
+                    **model_kwargs,
                 )
 
             # The model is itself the main layer
             except AttributeError:
                 # TensorFlow model
                 try:
                     self._model = self._model.__class__.from_pretrained(
-                        model_name, from_pt=False, **model_kwargs
+                        model_name,
+                        from_pt=False,
+                        **model_kwargs,
                     )
 
                 # PyTorch Model
                 except (OSError, TypeError):
                     model = AutoModel.from_pretrained(model_name)
                     model.save_pretrained(temporary_path)
                     self._model = self._model.__class__.from_pretrained(
-                        temporary_path, from_pt=True, **model_kwargs
+                        temporary_path,
+                        from_pt=True,
+                        **model_kwargs,
                     )
 
         remove_dir(temporary_path)
         assert self._tokenizer and self._model
```

## ernie/helper.py

```diff
@@ -1,17 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from tensorflow import data, TensorShape, int64, int32
 from math import exp
 from os import makedirs
-from shutil import rmtree, move, copytree
+from shutil import copytree, move, rmtree
 
+from tensorflow import TensorShape, data, int32, int64
 
-def get_features(tokenizer, sentences, labels):
+
+def get_features(
+    tokenizer,
+    sentences,
+    labels,
+):
     features = []
     for i, sentence in enumerate(sentences):
         inputs = tokenizer.encode_plus(
             sentence,
             add_special_tokens=True,
             max_length=tokenizer.model_max_length,
         )
@@ -30,27 +35,30 @@
             token_type_ids = (
                 token_type_ids + [tokenizer.pad_token_type_id] * padding_length
             )
 
         else:
             attention_mask = [0] * padding_length + [1] * len(input_ids)
             input_ids = [tokenizer.pad_token_id] * padding_length + input_ids
-            token_type_ids = \
+            token_type_ids = (
                 [tokenizer.pad_token_type_id] * padding_length + token_type_ids
+            )
 
-        assert tokenizer.model_max_length \
-            == len(attention_mask) \
-            == len(input_ids) \
+        assert (
+            tokenizer.model_max_length
+            == len(attention_mask)
+            == len(input_ids)
             == len(token_type_ids)
+        )
 
         feature = {
             'input_ids': input_ids,
             'attention_mask': attention_mask,
             'token_type_ids': token_type_ids,
-            'label': int(labels[i])
+            'label': int(labels[i]),
         }
 
         features.append(feature)
 
     def gen():
         for feature in features:
             yield (
@@ -64,15 +72,15 @@
 
     dataset = data.Dataset.from_generator(
         gen,
         (
             {
                 'input_ids': int32,
                 'attention_mask': int32,
-                'token_type_ids': int32
+                'token_type_ids': int32,
             }, int64
         ),
         (
             {
                 'input_ids': TensorShape([None]),
                 'attention_mask': TensorShape([None]),
                 'token_type_ids': TensorShape([None]),
```

## ernie/models.py

```diff
@@ -27,29 +27,44 @@
     AlbertXLargeCased2 = 'albert-xlarge-v2'
     AlbertXXLargeCased2 = 'albert-xxlarge-v2'
 
 
 class ModelsByFamily:
     Bert = set(
         [
-            Models.BertBaseUncased, Models.BertBaseCased,
-            Models.BertLargeUncased, Models.BertLargeCased
+            Models.BertBaseUncased,
+            Models.BertBaseCased,
+            Models.BertLargeUncased,
+            Models.BertLargeCased,
         ]
     )
-    Roberta = set([Models.RobertaBaseCased, Models.RobertaLargeCased])
-    XLNet = set([Models.XLNetBaseCased, Models.XLNetLargeCased])
+    Roberta = set([
+        Models.RobertaBaseCased,
+        Models.RobertaLargeCased,
+    ])
+    XLNet = set([
+        Models.XLNetBaseCased,
+        Models.XLNetLargeCased,
+    ])
     DistilBert = set(
-        [Models.DistilBertBaseUncased, Models.DistilBertBaseMultilingualCased]
+        [
+            Models.DistilBertBaseUncased,
+            Models.DistilBertBaseMultilingualCased,
+        ]
     )
     Albert = set(
         [
-            Models.AlbertBaseCased, Models.AlbertLargeCased,
-            Models.AlbertXLargeCased, Models.AlbertXXLargeCased,
-            Models.AlbertBaseCased2, Models.AlbertLargeCased2,
-            Models.AlbertXLargeCased2, Models.AlbertXXLargeCased2
+            Models.AlbertBaseCased,
+            Models.AlbertLargeCased,
+            Models.AlbertXLargeCased,
+            Models.AlbertXXLargeCased,
+            Models.AlbertBaseCased2,
+            Models.AlbertLargeCased2,
+            Models.AlbertXLargeCased2,
+            Models.AlbertXXLargeCased2,
         ]
     )
     Supported = set(
         [
             getattr(Models, model_type) for model_type in
             filter(lambda x: x[:2] != '__', Models.__dict__.keys())
         ]
```

## ernie/split_strategies.py

```diff
@@ -14,36 +14,42 @@
         r'https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}'
         r'\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)'
     )
     domain = re.compile(r'\w+\.\w+')
 
 
 class SplitStrategy:
+
     def __init__(
         self,
         split_patterns,
         remove_patterns=None,
         group_splits=True,
-        remove_too_short_groups=True
+        remove_too_short_groups=True,
     ):
         if not isinstance(split_patterns, list):
             self.split_patterns = [split_patterns]
         else:
             self.split_patterns = split_patterns
 
-        if remove_patterns is not None \
-                and not isinstance(remove_patterns, list):
+        if (remove_patterns is not None
+                and not isinstance(remove_patterns, list)):
             self.remove_patterns = [remove_patterns]
         else:
             self.remove_patterns = remove_patterns
 
         self.group_splits = group_splits
         self.remove_too_short_groups = remove_too_short_groups
 
-    def split(self, text, tokenizer, split_patterns=None):
+    def split(
+        self,
+        text,
+        tokenizer,
+        split_patterns=None,
+    ):
         if split_patterns is None:
             if self.split_patterns is None:
                 return [text]
             split_patterns = self.split_patterns
 
         def len_in_tokens(text_):
             no_tokens = len(tokenizer.encode(text_, add_special_tokens=False))
@@ -73,54 +79,66 @@
                 else:
                     selected_splits.append(split)
 
             else:
                 if not self.group_splits:
                     selected_splits.append(split)
                 else:
-                    new_aggregated_splits = \
+                    new_aggregated_splits = (
                         f'{aggregated_splits} {split}'.strip()
+                    )
                     if len_in_tokens(new_aggregated_splits) <= max_tokens:
                         aggregated_splits = new_aggregated_splits
                     else:
                         selected_splits.append(aggregated_splits)
                         aggregated_splits = split
 
         if aggregated_splits:
             selected_splits.append(aggregated_splits)
 
-        remove_too_short_groups = len(selected_splits) > 1 \
-            and self.group_splits \
+        remove_too_short_groups = (
+            len(selected_splits) > 1 and self.group_splits
             and self.remove_too_short_groups
+        )
 
         if not remove_too_short_groups:
             final_splits = selected_splits
         else:
-            final_splits
+            final_splits = []
             min_length = tokenizer.model_max_length / 2
             for split in selected_splits:
                 if len_in_tokens(split) >= min_length:
                     final_splits.append(split)
 
         return final_splits
 
 
 class SplitStrategies:
     SentencesWithoutUrls = SplitStrategy(
         split_patterns=[
-            RegexExpressions.split_by_dot, RegexExpressions.split_by_semicolon,
-            RegexExpressions.split_by_colon, RegexExpressions.split_by_comma
+            RegexExpressions.split_by_dot,
+            RegexExpressions.split_by_semicolon,
+            RegexExpressions.split_by_colon,
+            RegexExpressions.split_by_comma,
+        ],
+        remove_patterns=[
+            RegexExpressions.url,
+            RegexExpressions.domain,
         ],
-        remove_patterns=[RegexExpressions.url, RegexExpressions.domain],
         remove_too_short_groups=False,
-        group_splits=False
+        group_splits=False,
     )
 
     GroupedSentencesWithoutUrls = SplitStrategy(
         split_patterns=[
-            RegexExpressions.split_by_dot, RegexExpressions.split_by_semicolon,
-            RegexExpressions.split_by_colon, RegexExpressions.split_by_comma
+            RegexExpressions.split_by_dot,
+            RegexExpressions.split_by_semicolon,
+            RegexExpressions.split_by_colon,
+            RegexExpressions.split_by_comma,
+        ],
+        remove_patterns=[
+            RegexExpressions.url,
+            RegexExpressions.domain,
         ],
-        remove_patterns=[RegexExpressions.url, RegexExpressions.domain],
         remove_too_short_groups=True,
-        group_splits=True
+        group_splits=True,
     )
```

## Comparing `ernie-1.2308.1.dist-info/LICENSE` & `ernie-1.2405.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ernie-1.2308.1.dist-info/METADATA` & `ernie-1.2405.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ernie
-Version: 1.2308.1
+Version: 1.2405.0
 Summary: An Accessible Python Library for State-of-the-art Natural Language Processing. Built with HuggingFace's Transformers.
 Home-page: https://github.com/labteral/ernie
 Author: Rodrigo Martínez Castaño
 Author-email: dev@brunneis.com
 License: Apache License (Version 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -12,13 +12,13 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: transformers (<5.0.0,>=4.24.0)
-Requires-Dist: scikit-learn (<2.0.0,>=1.2.1)
-Requires-Dist: pandas (<2.0.0,>=1.5.3)
-Requires-Dist: tensorflow (<2.11.0,>=2.5.1)
-Requires-Dist: py-cpuinfo (<10.0.0,>=9.0.0)
+Requires-Dist: tf-keras
+Requires-Dist: transformers
+Requires-Dist: scikit-learn
+Requires-Dist: pandas
+Requires-Dist: py-cpuinfo
```

## Comparing `ernie-1.2308.1.dist-info/RECORD` & `ernie-1.2405.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-ernie/__init__.py,sha256=1b3F8tq3ORvwA9af9Fw4RFbVSC6iF2XmzBjZ-vdHTXM,1061
-ernie/aggregation_strategies.py,sha256=4UfPoHUdzhVWmZxQhUu9Ma6pHbvKyB9-VP7J13KzTOI,1934
-ernie/ernie.py,sha256=-sc2-tA-Nx1nQns8KewTsm3xRQw5RDRd_50M6zLl1Y4,13420
-ernie/helper.py,sha256=8-d0rF8SepFOxhE9oJgr9Vl5AHEop8af3KjVi6W-LNI,3026
-ernie/models.py,sha256=17CrjhCrNUP3_OKEBRlRimhs38dIfUmAoZOiIqRFJ9k,1758
-ernie/split_strategies.py,sha256=MJMsZ9Xis4Ffzx3MESiJpem2X_6Tg0eFGqxOIAeUbHs,4314
+ernie/__init__.py,sha256=gVF6QjiLOwx-orAOPo-_xLaJv5nsU8LaF-ajtvG_9yY,1064
+ernie/aggregation_strategies.py,sha256=AYp4QG4xh0ZgPGtpWgoGpwYsdgpnzZzPdda-pC7GQDA,2068
+ernie/ernie.py,sha256=XM3S0Yd-jYaa5C26Rr2_b32TnjyusnTpPlwD1WNPPl0,13843
+ernie/helper.py,sha256=YfLYeGgyi3BA3wiQNko2p7383rjAqtYXs62OugDyhFs,3076
+ernie/models.py,sha256=UMqtGQIPOACKow0uf5fqA35ISVvFqHFyHS26OHwjJP8,1913
+ernie/split_strategies.py,sha256=3A1x92SquI7e3qS6r64mmo69xLl0mWPyc1xoXdMG8v0,4512
 test/__init__.py,sha256=Vy72ITAa99WGby_RFX9sxvC-QUj3J3FrgDTOAovqAOM,87
 test/dump_load.py,sha256=tdd_OLWidDZtDEqGeWABPqP6Wi9D0VSUw7olebX2Ytg,1414
 test/load_csv.py,sha256=Z7Ka3PH44axCV4Ll44bSr7hLKr5n-h5mx-N_yYDOucs,775
 test/load_model.py,sha256=oN9mKif0GrvTdjmeOS4ReJJCCw12DfaWRqJR4ZpCoag,973
 test/predict.py,sha256=Me2bBayH-nHGfxEGcUo2jrlTNq5-IOS-OxONnQqOfrE,714
 test/split_aggregate.py,sha256=6l_318O8SO1Jt2nMvxQTskznd6aS1xGWX1cqr4Yj_84,18131
-ernie-1.2308.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-ernie-1.2308.1.dist-info/METADATA,sha256=9p6Q7qPTlLCARcNkOQ-lDwxDXuXcPwMKxwHTgnUZCxg,1016
-ernie-1.2308.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ernie-1.2308.1.dist-info/top_level.txt,sha256=IHK6af4HA-M8LcMpdIUJTH0DG1QRIai_1zA3kGcbwqI,11
-ernie-1.2308.1.dist-info/RECORD,,
+ernie-1.2405.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+ernie-1.2405.0.dist-info/METADATA,sha256=vkbph13uqwmBsNWg5VmdUGm6OKjE3oEPa-wOLvgm2hQ,926
+ernie-1.2405.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ernie-1.2405.0.dist-info/top_level.txt,sha256=IHK6af4HA-M8LcMpdIUJTH0DG1QRIai_1zA3kGcbwqI,11
+ernie-1.2405.0.dist-info/RECORD,,
```

