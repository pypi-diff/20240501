# Comparing `tmp/studcamp_yandex_hse-0.1.1.tar.gz` & `tmp/studcamp_yandex_hse-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "studcamp_yandex_hse-0.1.1.tar", max compression
+gzip compressed data, was "studcamp_yandex_hse-0.1.2.tar", max compression
```

## Comparing `studcamp_yandex_hse-0.1.1.tar` & `studcamp_yandex_hse-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     4076 2024-04-28 13:09:29.174808 studcamp_yandex_hse-0.1.1/README.md
--rw-r--r--   0        0        0      919 2024-04-28 13:15:29.182566 studcamp_yandex_hse-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-27 13:13:54.534284 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/__init__.py
--rw-r--r--   0        0        0      249 2024-04-28 12:14:43.071215 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/__init__.py
--rw-r--r--   0        0        0      133 2024-04-27 23:37:33.787449 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/attention_based_model/__init__.py
--rw-r--r--   0        0        0     3648 2024-04-27 23:37:33.787823 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/attention_based_model/attention_extractor.py
--rw-r--r--   0        0        0     1299 2024-04-27 23:37:33.788140 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/attention_based_model/tags_extractor.py
--rw-r--r--   0        0        0       66 2024-04-27 23:37:33.788566 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/bart_based_model/__init__.py
--rw-r--r--   0        0        0     3148 2024-04-27 23:37:33.788881 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/bart_based_model/tag_sum_extractor.py
--rw-r--r--   0        0        0      801 2024-04-27 23:37:33.789296 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/base_extractor.py
--rw-r--r--   0        0        0       84 2024-04-27 23:37:33.789591 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/clusterizer_based_model/__init__.py
--rw-r--r--   0        0        0     2018 2024-04-28 12:14:43.072641 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/clusterizer_based_model/clusterizer.py
--rw-r--r--   0        0        0     1330 2024-04-27 23:37:33.790132 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/clusterizer_based_model/faiss.py
--rw-r--r--   0        0        0     1230 2024-04-27 23:37:33.790398 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/metrics.py
--rw-r--r--   0        0        0      205 2024-04-27 23:37:33.790656 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rake_based_model/__init__.py
--rw-r--r--   0        0        0     1398 2024-04-27 23:37:33.790916 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rake_based_model/keyphrases_extractor.py
--rw-r--r--   0        0        0     3082 2024-04-27 23:37:33.791175 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rake_based_model/tags_extractor.py
--rw-r--r--   0        0        0       58 2024-04-28 12:14:43.072825 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rut5_based_model/__init__.py
--rw-r--r--   0        0        0     1067 2024-04-28 12:14:43.073098 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rut5_based_model/rut5_extractor.py
--rw-r--r--   0        0        0        0 2024-04-27 23:37:33.791220 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/__init__.py
--rw-r--r--   0        0        0      138 2024-04-27 23:37:33.791733 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/__init__.py
--rw-r--r--   0        0        0      803 2024-04-27 23:37:33.791972 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/base_embedder.py
--rw-r--r--   0        0        0     1071 2024-04-27 23:37:33.792207 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/fasttext_embedder.py
--rw-r--r--   0        0        0     1378 2024-04-27 23:37:33.792453 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/rubert_embedder.py
--rw-r--r--   0        0        0      210 2024-04-27 23:37:33.792695 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/__init__.py
--rw-r--r--   0        0        0      308 2024-04-27 23:37:33.792946 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/base_normalizer.py
--rw-r--r--   0        0        0      956 2024-04-27 23:37:33.793212 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/nouns_keeper.py
--rw-r--r--   0        0        0      818 2024-04-27 23:37:33.793493 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/pipe.py
--rw-r--r--   0        0        0      694 2024-04-27 23:37:33.793749 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/punctuation_deleter.py
--rw-r--r--   0        0        0      850 2024-04-27 23:37:33.794009 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/stopwords_deleter.py
--rw-r--r--   0        0        0      130 2024-04-27 23:37:33.794376 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/__init__.py
--rw-r--r--   0        0        0     1686 2024-04-27 23:37:33.794642 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/base_ranker.py
--rw-r--r--   0        0        0     1183 2024-04-27 23:37:33.794908 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/max_distance_ranker.py
--rw-r--r--   0        0        0      933 2024-04-27 23:37:33.795293 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/text_sim_ranker.py
--rw-r--r--   0        0        0       50 2024-04-27 23:37:33.795681 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/summarizator/__init__.py
--rw-r--r--   0        0        0     1331 2024-04-27 23:37:33.795945 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/summarizator/bart_summarization.py
--rw-r--r--   0        0        0       58 2024-04-27 23:37:33.796180 studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/utils.py
--rw-r--r--   0        0        0     5067 1970-01-01 00:00:00.000000 studcamp_yandex_hse-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4372 2024-04-30 18:38:17.688231 studcamp_yandex_hse-0.1.2/README.md
+-rw-r--r--   0        0        0      996 2024-04-30 20:20:33.348068 studcamp_yandex_hse-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-27 13:13:54.534284 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/__init__.py
+-rw-r--r--   0        0        0      249 2024-04-28 12:14:43.071215 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-27 23:37:33.787449 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/attention_based_model/__init__.py
+-rw-r--r--   0        0        0     3648 2024-04-27 23:37:33.787823 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/attention_based_model/attention_extractor.py
+-rw-r--r--   0        0        0     1299 2024-04-27 23:37:33.788140 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/attention_based_model/tags_extractor.py
+-rw-r--r--   0        0        0       66 2024-04-27 23:37:33.788566 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/bart_based_model/__init__.py
+-rw-r--r--   0        0        0     3148 2024-04-27 23:37:33.788881 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/bart_based_model/tag_sum_extractor.py
+-rw-r--r--   0        0        0      801 2024-04-27 23:37:33.789296 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/base_extractor.py
+-rw-r--r--   0        0        0       84 2024-04-27 23:37:33.789591 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/clusterizer_based_model/__init__.py
+-rw-r--r--   0        0        0     2038 2024-04-30 12:12:44.848173 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/clusterizer_based_model/clusterizer.py
+-rw-r--r--   0        0        0     1345 2024-04-30 12:25:41.186959 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/clusterizer_based_model/faiss.py
+-rw-r--r--   0        0        0     1230 2024-04-27 23:37:33.790398 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/metrics.py
+-rw-r--r--   0        0        0      205 2024-04-27 23:37:33.790656 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/rake_based_model/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-27 23:37:33.790916 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/rake_based_model/keyphrases_extractor.py
+-rw-r--r--   0        0        0     3011 2024-04-30 12:15:20.088907 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/rake_based_model/tags_extractor.py
+-rw-r--r--   0        0        0       58 2024-04-28 12:14:43.072825 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/rut5_based_model/__init__.py
+-rw-r--r--   0        0        0     1067 2024-04-28 12:14:43.073098 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/rut5_based_model/rut5_extractor.py
+-rw-r--r--   0        0        0        0 2024-04-27 23:37:33.791220 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-27 23:37:33.791733 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/embedder/__init__.py
+-rw-r--r--   0        0        0      803 2024-04-27 23:37:33.791972 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/embedder/base_embedder.py
+-rw-r--r--   0        0        0     1071 2024-04-30 19:46:48.282008 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/embedder/fasttext_embedder.py
+-rw-r--r--   0        0        0     1378 2024-04-27 23:37:33.792453 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/embedder/rubert_embedder.py
+-rw-r--r--   0        0        0      210 2024-04-27 23:37:33.792695 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/normalizers/__init__.py
+-rw-r--r--   0        0        0      308 2024-04-27 23:37:33.792946 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/normalizers/base_normalizer.py
+-rw-r--r--   0        0        0      956 2024-04-27 23:37:33.793212 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/normalizers/nouns_keeper.py
+-rw-r--r--   0        0        0      818 2024-04-27 23:37:33.793493 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/normalizers/pipe.py
+-rw-r--r--   0        0        0      694 2024-04-27 23:37:33.793749 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/normalizers/punctuation_deleter.py
+-rw-r--r--   0        0        0      850 2024-04-27 23:37:33.794009 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/normalizers/stopwords_deleter.py
+-rw-r--r--   0        0        0      130 2024-04-27 23:37:33.794376 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/ranker/__init__.py
+-rw-r--r--   0        0        0     1686 2024-04-27 23:37:33.794642 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/ranker/base_ranker.py
+-rw-r--r--   0        0        0     1183 2024-04-27 23:37:33.794908 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/ranker/max_distance_ranker.py
+-rw-r--r--   0        0        0      933 2024-04-27 23:37:33.795293 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/ranker/text_sim_ranker.py
+-rw-r--r--   0        0        0       50 2024-04-27 23:37:33.795681 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/summarizator/__init__.py
+-rw-r--r--   0        0        0     1331 2024-04-27 23:37:33.795945 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/summarizator/bart_summarization.py
+-rw-r--r--   0        0        0       58 2024-04-27 23:37:33.796180 studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/utils.py
+-rw-r--r--   0        0        0     5524 1970-01-01 00:00:00.000000 studcamp_yandex_hse-0.1.2/PKG-INFO
```

### Comparing `studcamp_yandex_hse-0.1.1/README.md` & `studcamp_yandex_hse-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 <h3 align='left'> My team and I, within machine learning studcamp by Yandex and HSE, developed a whole module for "Text Tagging" problem, in terms of keywords extraction. </h3>
 
 <h3 align='left'> We had a big research. We've tried several extractive and abstractive methods. We will discuss it further.</h3>
 
 <h2>🚀 Demo</h2>
 
-<p align="center"> Streamlit  </p>
+![Streamlit Demo](./materials/streamlit-Info-2024-04-30-15-04-49.gif)
 
 <h2>🧪 Preprocessing</h2>
 
 *   **Embedder Module:** FastText/RuBert embeddings realisation
 *   **Normalizer Modlule:**  Nouns extraction + Punctuation removal + Stopwords removal (For extractive models)
 *   **Ranker Module:** Module which ranks the most significant words by distance in embedding space (max_distance_ranker) and by cosine similarity with text embeddings (text_sim_ranker)
 *   **Summarizator Module:** Module which summarizes the text with MBart model
@@ -33,14 +33,16 @@
 Here're some of the project's best features:
 
 *   Online model: Rake Based Model with 10-20 it/sec (The fastest)
 *   Offline models: Bart based model with summarisation or attention. 1-5 it/sec (The slowest)
 
 <h2>🛠️ Installation Steps:</h2>
 
+#### Please, use python@3.10
+
 <p>1. Installation</p>
 
 ```
 pip install studcamp-yandex-hse
 ```
 
 <p>2. Download russian FastText embeddings and RuT5 weights with the links below and paste it at the same level as your source .py file</p>
@@ -50,23 +52,30 @@
 Weights: https://drive.google.com/file/d/1aqVtoNRX3xDokthxuBNFwfcXQfkKeAMa/view?usp=sharing
 ```
 
 <p>3. Import</p>
 
 ```
 from studcamp_yandex_hse.models import RakeBasedTagger, BartBasedTagger, AttentionBasedTagger, ClusterizationBasedTagger, RuT5Tagger
+from studcamp_yandex_hse.processing.embedder import FastTextEmbedder
+```
+
+<p>4. Init FastTextEmbedder (We need to pass the instance as argument for Rake and Clusterized models)</p>
+
+```
+ft_emb_model = FastTextEmbedder()
 ```
 
-<p>3. Init tagger</p>
+<p>5. Init Model</p>
 
 ```
-tagger = RakeBasedTagger()
+tagger = RakeBasedTagger(ft_emb_model)
 ```
 
-<p>4. Get tags</p>
+<p>6. Get tags</p>
 
 ```
 text = '...'
 top_n = 5
 
 tagger.extract(some_text, top_n)
 ```
```

### Comparing `studcamp_yandex_hse-0.1.1/pyproject.toml` & `studcamp_yandex_hse-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "studcamp-yandex-hse"
-version = "0.1.1"
+version = "0.1.2"
 description = "Text-tagging project within Yandex x HSE StudCamp event"
 authors = ["deniskazhekin <deniskazhekin@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "studcamp_yandex_hse" }]
 
 [tool.poetry.dependencies]
@@ -17,14 +17,18 @@
 fasttext-wheel = "^0.9.2"
 rake-nltk = "^1.0.6"
 sentencepiece = "^0.2.0"
 faiss-cpu = "^1.8.0"
 pre-commit = "^3.7.0"
 accelerate = "^0.29.3"
 peft = "^0.10.0"
+streamlit = "^1.33.0"
+dvc = "^3.50.1"
+dvc-gdrive = "^3.0.1"
+gdown = "^5.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 119
```

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/attention_based_model/attention_extractor.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/attention_based_model/attention_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/attention_based_model/tags_extractor.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/attention_based_model/tags_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/bart_based_model/tag_sum_extractor.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/bart_based_model/tag_sum_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/base_extractor.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/base_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/clusterizer_based_model/clusterizer.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/clusterizer_based_model/clusterizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 
 class DBSCANFaissTagger(BaseExtractor):
     """
     A class for extracting tags based on the clusterization idea
     """
 
-    def __init__(self) -> None:
+    def __init__(self, ft_emb_model) -> None:
         self.normalizer = NormalizersPipe(
             [
                 PunctDeleter(),
                 StopwordsDeleter("russian"),
                 NounsKeeper("russian"),
             ],
             final_split=True,
         )
-        self.embedder = FastTextEmbedder()
-        self.faiss = FaissKeywordExtractor()
+        self.embedder = ft_emb_model
+        self.faiss = FaissKeywordExtractor(ft_emb_model)
 
     def extract(self, text: str, top_n: int) -> list:
         """
         Main method to extract tags from text.
         :param text: source text
         :param top_n: parameter for the number of tags to extract
         :return: tags extracted from the text
```

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/metrics.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/metrics.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rake_based_model/keyphrases_extractor.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/rake_based_model/keyphrases_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rake_based_model/tags_extractor.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/rake_based_model/tags_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 class TagsExtractor(BaseExtractor):
     """
     A class used to extract tags from text based on keyword extraction, normalization, and ranking.
 
     Args:
+        ft_emb_model (FastTextEmbedder): FastText model used for word embeddings.
         language (str): Language used for text processing. Defaults to 'russian'.
-        fasttext_model_path (str): Path to the FastText model used for word embeddings.
         min_cnt_keyword (int): Minimum count for a keyword to be included in the tag results.
 
     Attributes:
         extractor (RakeKeyphrasesExtractor): Keyword extractor configured for specific language.
         normalizer (NormalizersPipe): Pipeline of text normalizers.
         ranker (MaxDistanceRanker):
             Ranking mechanism for keywords based on distance metrics in embedding space.
@@ -30,29 +30,28 @@
     Methods:
         extract(text: str, top_n: int) -> np.ndarray:
             Extracts and returns top_n tags from the given text.
     """
 
     def __init__(
         self,
+        ft_emb_model: FastTextEmbedder,
         language: str = "russian",
-        fasttext_model_path: str = "cc.ru.300.bin",
         min_cnt_keyword: int = 2,
     ) -> None:
         self.extractor = RakeKeyphrasesExtractor(language=language)
         self.normalizer = NormalizersPipe(
             [
                 PunctDeleter(),
                 StopwordsDeleter(language),
                 NounsKeeper(language),
             ],
             final_split=True,
         )
-        embedder = FastTextEmbedder(fasttext_model_path)
-        self.ranker = MaxDistanceRanker(embedder)
+        self.ranker = MaxDistanceRanker(ft_emb_model)
         self.min_cnt_keyword = min_cnt_keyword
 
     def extract(
         self,
         text: str,
         top_n: int,
     ) -> np.ndarray:
```

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/models/rut5_based_model/rut5_extractor.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/models/rut5_based_model/rut5_extractor.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/base_embedder.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/embedder/base_embedder.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/fasttext_embedder.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/embedder/fasttext_embedder.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/embedder/rubert_embedder.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/embedder/rubert_embedder.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/nouns_keeper.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/normalizers/nouns_keeper.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/pipe.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/normalizers/pipe.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/punctuation_deleter.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/normalizers/punctuation_deleter.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/normalizers/stopwords_deleter.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/normalizers/stopwords_deleter.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/base_ranker.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/ranker/base_ranker.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/max_distance_ranker.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/ranker/max_distance_ranker.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/ranker/text_sim_ranker.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/ranker/text_sim_ranker.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/studcamp_yandex_hse/processing/summarizator/bart_summarization.py` & `studcamp_yandex_hse-0.1.2/studcamp_yandex_hse/processing/summarizator/bart_summarization.py`

 * *Files identical despite different names*

### Comparing `studcamp_yandex_hse-0.1.1/PKG-INFO` & `studcamp_yandex_hse-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 Metadata-Version: 2.1
 Name: studcamp-yandex-hse
-Version: 0.1.1
+Version: 0.1.2
 Summary: Text-tagging project within Yandex x HSE StudCamp event
 License: MIT
 Author: deniskazhekin
 Author-email: deniskazhekin@yandex.ru
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: accelerate (>=0.29.3,<0.30.0)
+Requires-Dist: dvc (>=3.50.1,<4.0.0)
+Requires-Dist: dvc-gdrive (>=3.0.1,<4.0.0)
 Requires-Dist: faiss-cpu (>=1.8.0,<2.0.0)
 Requires-Dist: fasttext-wheel (>=0.9.2,<0.10.0)
+Requires-Dist: gdown (>=5.1.0,<6.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: peft (>=0.10.0,<0.11.0)
 Requires-Dist: pre-commit (>=3.7.0,<4.0.0)
 Requires-Dist: pymorphy2 (>=0.9.1,<0.10.0)
 Requires-Dist: rake-nltk (>=1.0.6,<2.0.0)
 Requires-Dist: scipy (==1.10.1)
 Requires-Dist: sentence-transformers (>=2.7.0,<3.0.0)
 Requires-Dist: sentencepiece (>=0.2.0,<0.3.0)
+Requires-Dist: streamlit (>=1.33.0,<2.0.0)
 Requires-Dist: transformers (>=4.40.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center" id="title">Studcamp Yandex x HSE</h1>
 
 <h2 align="center" id="title">Text Tagging</h2>
 
 <h3 align='left'> My team and I, within machine learning studcamp by Yandex and HSE, developed a whole module for "Text Tagging" problem, in terms of keywords extraction. </h3>
 
 <h3 align='left'> We had a big research. We've tried several extractive and abstractive methods. We will discuss it further.</h3>
 
 <h2>🚀 Demo</h2>
 
-<p align="center"> Streamlit  </p>
+![Streamlit Demo](./materials/streamlit-Info-2024-04-30-15-04-49.gif)
 
 <h2>🧪 Preprocessing</h2>
 
 *   **Embedder Module:** FastText/RuBert embeddings realisation
 *   **Normalizer Modlule:**  Nouns extraction + Punctuation removal + Stopwords removal (For extractive models)
 *   **Ranker Module:** Module which ranks the most significant words by distance in embedding space (max_distance_ranker) and by cosine similarity with text embeddings (text_sim_ranker)
 *   **Summarizator Module:** Module which summarizes the text with MBart model
@@ -59,14 +63,16 @@
 Here're some of the project's best features:
 
 *   Online model: Rake Based Model with 10-20 it/sec (The fastest)
 *   Offline models: Bart based model with summarisation or attention. 1-5 it/sec (The slowest)
 
 <h2>🛠️ Installation Steps:</h2>
 
+#### Please, use python@3.10
+
 <p>1. Installation</p>
 
 ```
 pip install studcamp-yandex-hse
 ```
 
 <p>2. Download russian FastText embeddings and RuT5 weights with the links below and paste it at the same level as your source .py file</p>
@@ -76,23 +82,30 @@
 Weights: https://drive.google.com/file/d/1aqVtoNRX3xDokthxuBNFwfcXQfkKeAMa/view?usp=sharing
 ```
 
 <p>3. Import</p>
 
 ```
 from studcamp_yandex_hse.models import RakeBasedTagger, BartBasedTagger, AttentionBasedTagger, ClusterizationBasedTagger, RuT5Tagger
+from studcamp_yandex_hse.processing.embedder import FastTextEmbedder
+```
+
+<p>4. Init FastTextEmbedder (We need to pass the instance as argument for Rake and Clusterized models)</p>
+
+```
+ft_emb_model = FastTextEmbedder()
 ```
 
-<p>3. Init tagger</p>
+<p>5. Init Model</p>
 
 ```
-tagger = RakeBasedTagger()
+tagger = RakeBasedTagger(ft_emb_model)
 ```
 
-<p>4. Get tags</p>
+<p>6. Get tags</p>
 
 ```
 text = '...'
 top_n = 5
 
 tagger.extract(some_text, top_n)
 ```
```

