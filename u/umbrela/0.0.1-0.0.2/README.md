# Comparing `tmp/umbrela-0.0.1-py3-none-any.whl.zip` & `tmp/umbrela-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 16098 bytes, number of entries: 15
+Zip file size: 16104 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 24-May-01 17:25 prompts/__init__.py
 -rw-r--r--  2.0 unx     1231 b- defN 24-May-01 01:05 prompts/qrel_fewshot_bing.txt
 -rw-r--r--  2.0 unx        0 b- defN 24-May-01 17:11 umbrela/__init__.py
 -rw-r--r--  2.0 unx     2648 b- defN 24-May-01 01:04 umbrela/gpt_judge.py
 -rw-r--r--  2.0 unx      751 b- defN 24-Apr-30 23:41 umbrela/llm_judge.py
 -rw-r--r--  2.0 unx     2377 b- defN 24-May-01 01:04 umbrela/osllm_judge.py
 -rw-r--r--  2.0 unx     3315 b- defN 24-May-01 01:04 umbrela/vicuna_judge.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-01 17:25 umbrela/utils/__init__.py
 -rw-r--r--  2.0 unx     1884 b- defN 24-May-01 01:04 umbrela/utils/common_utils.py
--rw-r--r--  2.0 unx     3038 b- defN 24-Apr-30 05:09 umbrela/utils/qrel_utils.py
--rw-r--r--  2.0 unx    10766 b- defN 24-May-01 17:49 umbrela-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    13073 b- defN 24-May-01 17:49 umbrela-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-01 17:49 umbrela-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-May-01 17:49 umbrela-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1181 b- defN 24-May-01 17:49 umbrela-0.0.1.dist-info/RECORD
-15 files, 40372 bytes uncompressed, 14152 bytes compressed:  64.9%
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-01 18:15 umbrela/utils/qrel_utils.py
+-rw-r--r--  2.0 unx    10766 b- defN 24-May-01 18:16 umbrela-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13073 b- defN 24-May-01 18:16 umbrela-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-01 18:16 umbrela-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-May-01 18:16 umbrela-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1181 b- defN 24-May-01 18:16 umbrela-0.0.2.dist-info/RECORD
+15 files, 40374 bytes uncompressed, 14158 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: umbrela/utils/common_utils.py
 Comment: 
 
 Filename: umbrela/utils/qrel_utils.py
 Comment: 
 
-Filename: umbrela-0.0.1.dist-info/LICENSE
+Filename: umbrela-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: umbrela-0.0.1.dist-info/METADATA
+Filename: umbrela-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: umbrela-0.0.1.dist-info/WHEEL
+Filename: umbrela-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: umbrela-0.0.1.dist-info/top_level.txt
+Filename: umbrela-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: umbrela-0.0.1.dist-info/RECORD
+Filename: umbrela-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## umbrela/utils/qrel_utils.py

```diff
@@ -76,15 +76,15 @@
     query_mappings = get_topics(topic_mapping[qrel])
     return query_mappings
 
 
 def get_index_reader(qrel):
     # Index reader
     if qrel in ["dl19-passage", "dl20-passage"]:
-        index_reader = IndexReader("indexes/lucene-index-msmarco-passage")
+        index_reader = IndexReader.from_prebuilt_index("msmarco-v1-passage")
     else:
         index_reader = None
     return index_reader
 
 
 def generate_examples_prompt(qrel, few_shot_count):
     qrel_data = get_qrels(qrel)
```

## Comparing `umbrela-0.0.1.dist-info/LICENSE` & `umbrela-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `umbrela-0.0.1.dist-info/METADATA` & `umbrela-0.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umbrela
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Package for generating query-passage relevance assessment labels.
 Author-email: Shivani Upadhyay <sjupadhyay@uwaterloo.ca>, Ronak Pradeep <rpradeep@uwaterloo.ca>, Jimmy Lin <jimmylin@uwaterloo.ca>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

