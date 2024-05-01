# Comparing `tmp/SIRITVIS-1.1.7.1.tar.gz` & `tmp/SIRITVIS-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIRITVIS-1.1.7.1.tar", last modified: Sun Feb 25 22:17:45 2024, max compression
+gzip compressed data, was "SIRITVIS-1.1.8.tar", last modified: Sun Apr 28 11:12:56 2024, max compression
```

## Comparing `SIRITVIS-1.1.7.1.tar` & `SIRITVIS-1.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 deftwolf   (501) staff       (20)        0 2024-02-25 22:17:45.621653 SIRITVIS-1.1.7.1/
--rw-r--r--   0 deftwolf   (501) staff       (20)     1098 2023-10-29 13:23:38.000000 SIRITVIS-1.1.7.1/LICENSE
--rw-r--r--   0 deftwolf   (501) staff       (20)    12528 2024-02-25 22:17:45.621336 SIRITVIS-1.1.7.1/PKG-INFO
--rw-r--r--   0 deftwolf   (501) staff       (20)    10949 2024-02-25 22:01:39.000000 SIRITVIS-1.1.7.1/README.md
-drwxr-xr-x   0 deftwolf   (501) staff       (20)        0 2024-02-25 22:17:45.619834 SIRITVIS-1.1.7.1/SIRITVIS/
--rw-r--r--   0 deftwolf   (501) staff       (20)      416 2023-10-29 14:15:42.000000 SIRITVIS-1.1.7.1/SIRITVIS/__init__.py
--rw-r--r--   0 deftwolf   (501) staff       (20)    23681 2023-10-29 14:15:42.000000 SIRITVIS-1.1.7.1/SIRITVIS/cleaner.py
--rw-r--r--   0 deftwolf   (501) staff       (20)     3666 2023-11-13 11:49:14.000000 SIRITVIS-1.1.7.1/SIRITVIS/insta_streamer.py
--rw-r--r--   0 deftwolf   (501) staff       (20)     5279 2023-10-29 14:15:42.000000 SIRITVIS-1.1.7.1/SIRITVIS/reddit_streamer.py
--rw-r--r--   0 deftwolf   (501) staff       (20)    18524 2023-10-29 14:15:42.000000 SIRITVIS-1.1.7.1/SIRITVIS/topic_mapper.py
--rw-r--r--   0 deftwolf   (501) staff       (20)    32258 2024-02-21 22:17:46.000000 SIRITVIS-1.1.7.1/SIRITVIS/topic_model.py
--rw-r--r--   0 deftwolf   (501) staff       (20)     8641 2024-02-21 22:01:23.000000 SIRITVIS-1.1.7.1/SIRITVIS/topic_visualise.py
--rw-r--r--   0 deftwolf   (501) staff       (20)     6480 2023-10-29 14:15:42.000000 SIRITVIS-1.1.7.1/SIRITVIS/twitter_streamer.py
-drwxr-xr-x   0 deftwolf   (501) staff       (20)        0 2024-02-25 22:17:45.620901 SIRITVIS-1.1.7.1/SIRITVIS.egg-info/
--rw-r--r--   0 deftwolf   (501) staff       (20)    12528 2024-02-25 22:17:45.000000 SIRITVIS-1.1.7.1/SIRITVIS.egg-info/PKG-INFO
--rw-r--r--   0 deftwolf   (501) staff       (20)      387 2024-02-25 22:17:45.000000 SIRITVIS-1.1.7.1/SIRITVIS.egg-info/SOURCES.txt
--rw-r--r--   0 deftwolf   (501) staff       (20)        1 2024-02-25 22:17:45.000000 SIRITVIS-1.1.7.1/SIRITVIS.egg-info/dependency_links.txt
--rw-r--r--   0 deftwolf   (501) staff       (20)      425 2024-02-25 22:17:45.000000 SIRITVIS-1.1.7.1/SIRITVIS.egg-info/requires.txt
--rw-r--r--   0 deftwolf   (501) staff       (20)        9 2024-02-25 22:17:45.000000 SIRITVIS-1.1.7.1/SIRITVIS.egg-info/top_level.txt
--rw-r--r--   0 deftwolf   (501) staff       (20)       38 2024-02-25 22:17:45.621724 SIRITVIS-1.1.7.1/setup.cfg
--rw-r--r--   0 deftwolf   (501) staff       (20)     1996 2024-02-25 22:17:41.000000 SIRITVIS-1.1.7.1/setup.py
+drwxr-xr-x   0 deftwolf   (501) staff       (20)        0 2024-04-28 11:12:56.965258 SIRITVIS-1.1.8/
+-rw-r--r--   0 deftwolf   (501) staff       (20)     1098 2023-10-29 13:23:38.000000 SIRITVIS-1.1.8/LICENSE
+-rw-r--r--   0 deftwolf   (501) staff       (20)    12489 2024-04-28 11:12:56.964875 SIRITVIS-1.1.8/PKG-INFO
+-rw-r--r--   0 deftwolf   (501) staff       (20)    10949 2024-02-25 22:01:39.000000 SIRITVIS-1.1.8/README.md
+drwxr-xr-x   0 deftwolf   (501) staff       (20)        0 2024-04-28 11:12:56.963415 SIRITVIS-1.1.8/SIRITVIS/
+-rw-r--r--   0 deftwolf   (501) staff       (20)      416 2023-10-29 14:15:42.000000 SIRITVIS-1.1.8/SIRITVIS/__init__.py
+-rw-r--r--   0 deftwolf   (501) staff       (20)    23681 2023-10-29 14:15:42.000000 SIRITVIS-1.1.8/SIRITVIS/cleaner.py
+-rw-r--r--   0 deftwolf   (501) staff       (20)     3666 2023-11-13 11:49:14.000000 SIRITVIS-1.1.8/SIRITVIS/insta_streamer.py
+-rw-r--r--   0 deftwolf   (501) staff       (20)     5279 2023-10-29 14:15:42.000000 SIRITVIS-1.1.8/SIRITVIS/reddit_streamer.py
+-rw-r--r--   0 deftwolf   (501) staff       (20)    18782 2024-04-28 11:12:53.000000 SIRITVIS-1.1.8/SIRITVIS/topic_mapper.py
+-rw-r--r--   0 deftwolf   (501) staff       (20)    32389 2024-04-28 11:10:22.000000 SIRITVIS-1.1.8/SIRITVIS/topic_model.py
+-rw-r--r--   0 deftwolf   (501) staff       (20)     8748 2024-04-22 20:33:46.000000 SIRITVIS-1.1.8/SIRITVIS/topic_visualise.py
+-rw-r--r--   0 deftwolf   (501) staff       (20)     6480 2023-10-29 14:15:42.000000 SIRITVIS-1.1.8/SIRITVIS/twitter_streamer.py
+drwxr-xr-x   0 deftwolf   (501) staff       (20)        0 2024-04-28 11:12:56.964394 SIRITVIS-1.1.8/SIRITVIS.egg-info/
+-rw-r--r--   0 deftwolf   (501) staff       (20)    12489 2024-04-28 11:12:56.000000 SIRITVIS-1.1.8/SIRITVIS.egg-info/PKG-INFO
+-rw-r--r--   0 deftwolf   (501) staff       (20)      387 2024-04-28 11:12:56.000000 SIRITVIS-1.1.8/SIRITVIS.egg-info/SOURCES.txt
+-rw-r--r--   0 deftwolf   (501) staff       (20)        1 2024-04-28 11:12:56.000000 SIRITVIS-1.1.8/SIRITVIS.egg-info/dependency_links.txt
+-rw-r--r--   0 deftwolf   (501) staff       (20)      403 2024-04-28 11:12:56.000000 SIRITVIS-1.1.8/SIRITVIS.egg-info/requires.txt
+-rw-r--r--   0 deftwolf   (501) staff       (20)        9 2024-04-28 11:12:56.000000 SIRITVIS-1.1.8/SIRITVIS.egg-info/top_level.txt
+-rw-r--r--   0 deftwolf   (501) staff       (20)       38 2024-04-28 11:12:56.965312 SIRITVIS-1.1.8/setup.cfg
+-rw-r--r--   0 deftwolf   (501) staff       (20)     1961 2024-04-22 20:37:40.000000 SIRITVIS-1.1.8/setup.py
```

### Comparing `SIRITVIS-1.1.7.1/LICENSE` & `SIRITVIS-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SIRITVIS-1.1.7.1/PKG-INFO` & `SIRITVIS-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SIRITVIS
-Version: 1.1.7.1
+Version: 1.1.8
 Summary: SIRITVIS: Social Media Interaction Reaction Insights Topic Visualisation
 Home-page: https://github.com/CodeEagle22/SIRITVIS
 Author: Sagar Narwade, Gillian Kant, Benjamin Saefken, Benjamin Leiding
 Maintainer: Sagar Narwade
 Maintainer-email: sagarnarwade147@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -22,29 +22,28 @@
 Requires-Dist: gensim
 Requires-Dist: pyLDAvis==3.4.0
 Requires-Dist: matplotlib
 Requires-Dist: tweepy==3.9.0
 Requires-Dist: urllib3
 Requires-Dist: langdetect
 Requires-Dist: octis
-Requires-Dist: topic-wizard==0.3.1
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: folium==0.14.0
 Requires-Dist: pickle4==0.0.1
 Requires-Dist: plotly==5.15.0
 Requires-Dist: nltk==3.6.2
 Requires-Dist: notebook==6.5.5
 Requires-Dist: ipywidgets
 Requires-Dist: tensorflow
 Requires-Dist: vaderSentiment
 Requires-Dist: ipyleaflet
 Requires-Dist: geopy
 Requires-Dist: Flask==2.2.5
 Requires-Dist: Flask-Caching==2.0.1
-Requires-Dist: wordcloud==1.8.2.2
+Requires-Dist: wordcloud==1.9.2
 Requires-Dist: ipython==7.34.0
 Requires-Dist: textblob==0.15.3
 Requires-Dist: apify-client==1.4.0
 Requires-Dist: instagram_private_api==1.6.0
```

### Comparing `SIRITVIS-1.1.7.1/README.md` & `SIRITVIS-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `SIRITVIS-1.1.7.1/SIRITVIS/cleaner.py` & `SIRITVIS-1.1.8/SIRITVIS/cleaner.py`

 * *Files identical despite different names*

### Comparing `SIRITVIS-1.1.7.1/SIRITVIS/insta_streamer.py` & `SIRITVIS-1.1.8/SIRITVIS/insta_streamer.py`

 * *Files identical despite different names*

### Comparing `SIRITVIS-1.1.7.1/SIRITVIS/reddit_streamer.py` & `SIRITVIS-1.1.8/SIRITVIS/reddit_streamer.py`

 * *Files identical despite different names*

### Comparing `SIRITVIS-1.1.7.1/SIRITVIS/topic_mapper.py` & `SIRITVIS-1.1.8/SIRITVIS/topic_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,39 +31,44 @@
             model_file (str or dict): The path to the model file (if str) or the model dictionary (if dict).
         """
 
         assert isinstance(data_source, (str,pd.DataFrame)), "csv_file must be a string"
         assert isinstance(model_source, (str, dict)), "model_file must be a string path or a dictionary variable"
 
         # Read the data into a pandas DataFrame
-
-        if isinstance(data_source, str):
-            self.df = pd.read_csv(data_source)
-        else:
-            self.df = data_source
-
-        self.model_file = model_source
         try:
-          self.center_lat = self.df['center_coord_Y'].mean()
-          self.center_lon = self.df['center_coord_X'].mean()
-        except:
-          print("Make sure csv_file contains coordinate columns 'center_coord_Y' and 'center_coord_X'")
-        self.keyword_rankings = {}
-        self.country_dropdown = None
-        # Create an output widget to display download status
-        self.output_widget = Output()
-        
-        # Create an export button
-        self.export_button = Button(description="Export Map as HTML")
-        self.export_button.on_click(self.export_map)
+            if isinstance(data_source, str):
+                self.df = pd.read_csv(data_source)
+            else:
+                self.df = data_source
+
+            self.model_file = model_source
+            try:
+                self.center_lat = self.df['center_coord_Y'].mean()
+                self.center_lon = self.df['center_coord_X'].mean()
+            except:
+                print("Make sure csv_file contains coordinate columns 'center_coord_Y' and 'center_coord_X'")
+            self.keyword_rankings = {}
+            self.country_dropdown = None
+            # Create an output widget to display download status
+            self.output_widget = Output()
+            
+            # Create an export button
+            self.export_button = Button(description="Export Map as HTML")
+            self.export_button.on_click(self.export_map)
 
-     
+        
 
-        # Create dropdowns
-        self.create_dropdowns()
+            # Create dropdowns
+            self.create_dropdowns()
+        
+                
+        except KeyError:
+            print("KeyError: 'country' column does not exist in the dataset.")
+            return False  
 
     def perform_sentiment_analysis(self):
         # Initialize the sentiment analyzer
         analyzer = SentimentIntensityAnalyzer()
         sentiments = []
 
         # Perform sentiment classification for each text in the dataset
```

### Comparing `SIRITVIS-1.1.7.1/SIRITVIS/topic_model.py` & `SIRITVIS-1.1.8/SIRITVIS/topic_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,30 @@
 from tqdm.contrib.concurrent import process_map  # or thread_map
 from tqdm import tqdm
 from pathlib import Path
 from octis.dataset.dataset import Dataset
 from collections import Counter
 import nltk
 import math
-nltk.download('stopwords')
-import warnings
-# Suppress warnings
-warnings.filterwarnings("ignore")
+
 import ssl
+
 try:
     _create_unverified_https_context = ssl._create_unverified_context
 except AttributeError:
     pass
 else:
     ssl._create_default_https_context = _create_unverified_https_context
 
+nltk.download('stopwords')
+import warnings
+# Suppress warnings
+warnings.filterwarnings("ignore")
+
+
 # Adjust log level to suppress log messages
 import logging
 logging.getLogger().setLevel(logging.ERROR)
 
 """
 Maps the language to its corresponding spacy model
 """
@@ -400,15 +404,16 @@
 
             evaluation (str): Matrix to use for model evaluation (default: ['accuracy','topicdiversity','invertedrbo','jaccardsimilarity','coherence']).
 
         """
 
         valid_values = ['accuracy', 'topicdiversity', 'invertedrbo', 'jaccardsimilarity', 'coherence']
         assert isinstance(num_topics, int) and num_topics > 0, "num_topics should be a positive integer."
-        assert isinstance(dataset_source, (str,pd.DataFrame)), "dataset_path should be a string or preprocessed dataset variable"
+        assert isinstance(dataset_source, (str, pd.DataFrame)), "dataset_path should be a string or preprocessed dataset variable"
+        # Check if learning_rate is a positive float
         assert isinstance(learning_rate, float) and learning_rate > 0, "learning_rate should be a positive float."
         assert isinstance(batch_size, int) and batch_size > 0, "batch_size should be a positive integer."
         assert activation in ['softplus', 'relu', 'sigmoid', 'swish', 'leakyrelu', 'rrelu', 'elu', 'selu', 'tanh'], "activation must be 'softplus', 'relu', 'sigmoid', 'swish', 'leakyrelu', 'rrelu', 'elu', 'selu' or 'tanh'."
         assert isinstance(num_layers, int) and num_layers > 0, "num_layers should be a positive integer."
         assert isinstance(num_neurons, int) and num_neurons > 0, "num_neurons should be a positive integer."
         assert isinstance(dropout, float) and 0 <= dropout <= 1, "dropout should be a float between 0 and 1."
         assert isinstance(num_epochs, int) and num_epochs > 0, "num_epochs should be a positive integer."
@@ -435,50 +440,56 @@
         self.df = None
         self.processed = None
         self.dataset = None
         self.nlda = None
         self.evaluation_results = None
         self.evaluation = evaluation
 
-        file_size = os.path.getsize(dataset_source)
-    
-        # Check if the file size is less than 1 MB
-        if file_size < 1024 * 1024:  # 1 MB = 1024 * 1024 bytes
-            print("Recommendation: Consider using a larger file with more data (at least 1 MB).")
-
         
 
     def read_data(self):
         """
         Reads the dataset from the provided file path.
         """
+        
+          
         try:
-            if isinstance(self.dataset_path, str):
+            if isinstance(self.dataset_path, pd.DataFrame):
+                self.df = self.dataset_path
+            elif isinstance(self.dataset_path, str):
                 if self.dataset_path.endswith('.pkl'):
                     self.df = pd.read_pickle(self.dataset_path).reset_index(drop=True)
                 elif self.dataset_path.endswith('.csv'):
                     self.df = pd.read_csv(self.dataset_path).reset_index(drop=True)
                 else:
                     print("Error: Invalid dataset file format. Only .pkl and .csv formats are supported.")
                     return False
             else:
                 self.df = self.dataset_path
+
+     
+            
+            
+
         except FileNotFoundError:
             print("Error: Dataset file not found.")
             return False
         except Exception as e:
             print("Error: Reading dataset failed:", e)
             return False
         return True
 
     def preprocess_data(self):
         """
         Preprocesses the data by removing 'RT', dropping NaN values, and saving the processed text to a file.
         """
-        
+        if len(self.df) < 200:
+                print("Warning: The dataset size is very small.")
+                self.df = pd.concat([self.df] * 40, ignore_index=True)  # Multiplying records 
+
         if self.df is None:
             print("Error: No data loaded. Call read_data() first.")
             return False
 
         try:
             self.processed = self.df['text'].str.replace('RT', '').dropna().reset_index()['text']
             self.processed = self.processed[self.processed.str.len() > 3]
```

### Comparing `SIRITVIS-1.1.7.1/SIRITVIS/topic_visualise.py` & `SIRITVIS-1.1.8/SIRITVIS/topic_visualise.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,87 +4,93 @@
 
 import glob
 from heapq import nlargest
 from sklearn.decomposition import NMF, LatentDirichletAllocation
 from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
 from sklearn.pipeline import make_pipeline
 from multiprocessing import Pool, cpu_count
-import numpy as np
+
 import os
-import matplotlib.pyplot as plt
 import pandas as pd
+import numpy as np
+import matplotlib.pyplot as plt
 from IPython.core.display import display, HTML
 import pyLDAvis
 from pyLDAvis.lda_model import prepare
 import warnings
 from wordcloud import WordCloud
 
 
+
 # Suppress warnings
 warnings.filterwarnings("ignore")
 
 # Adjust log level to suppress log messages
 import logging
 logging.getLogger().setLevel(logging.ERROR)
 
 class PyLDAvis():
-    def __init__(self, data_source,num_topics=10, text_column='text'):
+    def __init__(self, data_source, num_topics=10, text_column='text'):
         """
         Initialize the PyLDAvis class.
 
         Parameters:
         - data_source (str or DataFrame): The path to the CSV file or a DataFrame containing the data.
         - text_column (str): The name of the text column in the CSV file or DataFrame.
         """
-        assert isinstance(data_source, (str,pd.DataFrame)), "data_source should be a string path or preprocessed dataset variable"
+        assert isinstance(data_source, (str, pd.DataFrame)), "data_source should be a string path or preprocessed dataset variable"
         assert text_column is None or isinstance(text_column, str), "text_column must be a str"
-        self.file_path = data_source
-        self.column_name = text_column
+        self.data_source = data_source
+        self.text_column = text_column
         self.num_topics = num_topics
         self.lines = None
         self.tf_vectorizer = None
         self.dtms_tf = None
         self.tfidf_vectorizer = None
         self.dtms_tfidf = None
         self.lda_tf = None
         self.vis = None
 
     def visualize(self):
         """
-        Perform Latent Dirichlet Allocation (LDA) and prepare the visualization.
-
+        Perform Latent Dirichlet Allocation (LDA) and prepare the visualization. 
         Returns:
         - vis: The prepared visualization object.
         """
         try:
-
-            print('The visualisation is based on Latent Dirichlet Allocation (LDA) model.')
+            print('The visualization is based on Latent Dirichlet Allocation (LDA) model.')
+            
             # Read the CSV file or use the provided DataFrame
-            if isinstance(self.file_path, pd.DataFrame):
-                data = self.file_path
-            elif isinstance(self.file_path, str):
-                file_extension = os.path.splitext(self.file_path)[1]
+            if isinstance(self.data_source, pd.DataFrame):
+                data = self.data_source
+            elif isinstance(self.data_source, str):
+                file_extension = os.path.splitext(self.data_source)[1]
                 if file_extension == ".pkl":
                     # Read pickle file
-                    data = pd.read_pickle(self.file_path).dropna().reset_index(drop=True)
+                    data = pd.read_pickle(self.data_source).dropna().reset_index(drop=True)
                 elif file_extension == ".csv":
                     # Read CSV file
-                    data = pd.read_csv(self.file_path).dropna().reset_index(drop=True)
+                    data = pd.read_csv(self.data_source).dropna().reset_index(drop=True)
                 else:
                     print("Unsupported file format.")
                     return None
             else:
                 print("Invalid data type. Please provide either a DataFrame or a file path.")
                 return None
 
-            if self.column_name not in data.columns:
-                print(f"Error: The column '{self.column_name}' does not exist in the data.")
+            if self.text_column not in data.columns:
+                print(f"Error: The column '{self.text_column}' does not exist in the data.")
                 return None
 
-            self.lines = data[self.column_name].tolist()
+            
+            if len(data) < 200:
+                print("Warning: The dataset size is very small.")
+                data = pd.concat([data] * 40, ignore_index=True)  # Multiplying records 
+
+            self.lines = data[self.text_column].tolist()
 
             # Create the TF vectorizer
             self.tf_vectorizer = CountVectorizer(strip_accents='unicode',
                                                 stop_words='english',
                                                 lowercase=True,
                                                 token_pattern=r'\b[a-zA-Z]{3,}\b',
                                                 max_df=0.5,
@@ -97,36 +103,29 @@
 
             # Perform Latent Dirichlet Allocation
             self.lda_tf = LatentDirichletAllocation(n_components=self.num_topics, random_state=0)
             self.lda_tf.fit(self.dtms_tf)
 
             # Prepare the visualization
             
-            
             self.vis = pyLDAvis.lda_model.prepare(self.lda_tf, self.dtms_tf, self.tf_vectorizer)
             pyLDAvis.enable_notebook()
             return pyLDAvis.display(self.vis)
-            
-        
-        except FileNotFoundError:
-            print("Error: File not found.")
-        except pd.errors.EmptyDataError:
-            print("Error: The CSV file is empty.")
+
+
         except ValueError as ve:
             if "max_df corresponds to fewer documents than min_df" in str(ve):
                 print(f"The dataset size is very small: {str(ve)}")
+            elif "NoneType' object has no attribute 'display_formatter" in str(ve):
+                print("Error: The file size is too small. Recommended file size is > 1 MB.")
             else:
                 print(f"An error occurred: {str(ve)}")
-        except Exception as e:
-            print(f"An unexpected error occurred: {str(e)}")
 
         
 
-    
-
 class Wordcloud():
     def __init__(self, data_source, text_column='text', save_image=False):
         """
         Initialize the Word_Cloud class.
 
         Parameters:
         - data_source (str or DataFrame): The path to the CSV file or a DataFrame containing the data.
```

### Comparing `SIRITVIS-1.1.7.1/SIRITVIS/twitter_streamer.py` & `SIRITVIS-1.1.8/SIRITVIS/twitter_streamer.py`

 * *Files identical despite different names*

### Comparing `SIRITVIS-1.1.7.1/SIRITVIS.egg-info/PKG-INFO` & `SIRITVIS-1.1.8/SIRITVIS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SIRITVIS
-Version: 1.1.7.1
+Version: 1.1.8
 Summary: SIRITVIS: Social Media Interaction Reaction Insights Topic Visualisation
 Home-page: https://github.com/CodeEagle22/SIRITVIS
 Author: Sagar Narwade, Gillian Kant, Benjamin Saefken, Benjamin Leiding
 Maintainer: Sagar Narwade
 Maintainer-email: sagarnarwade147@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -22,29 +22,28 @@
 Requires-Dist: gensim
 Requires-Dist: pyLDAvis==3.4.0
 Requires-Dist: matplotlib
 Requires-Dist: tweepy==3.9.0
 Requires-Dist: urllib3
 Requires-Dist: langdetect
 Requires-Dist: octis
-Requires-Dist: topic-wizard==0.3.1
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: folium==0.14.0
 Requires-Dist: pickle4==0.0.1
 Requires-Dist: plotly==5.15.0
 Requires-Dist: nltk==3.6.2
 Requires-Dist: notebook==6.5.5
 Requires-Dist: ipywidgets
 Requires-Dist: tensorflow
 Requires-Dist: vaderSentiment
 Requires-Dist: ipyleaflet
 Requires-Dist: geopy
 Requires-Dist: Flask==2.2.5
 Requires-Dist: Flask-Caching==2.0.1
-Requires-Dist: wordcloud==1.8.2.2
+Requires-Dist: wordcloud==1.9.2
 Requires-Dist: ipython==7.34.0
 Requires-Dist: textblob==0.15.3
 Requires-Dist: apify-client==1.4.0
 Requires-Dist: instagram_private_api==1.6.0
```

### Comparing `SIRITVIS-1.1.7.1/setup.py` & `SIRITVIS-1.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = ""
 except Exception as e:
     print("An error occurred while reading README.md:", str(e))
     long_description = ""
 
 setup(
     name='SIRITVIS',
-    version='1.1.7.1',
+    version='1.1.8',
     author='Sagar Narwade, Gillian Kant, Benjamin Saefken, Benjamin Leiding',
     description="SIRITVIS: Social Media Interaction Reaction Insights Topic Visualisation",
     long_description=long_description,
     long_description_content_type='text/markdown',  
     url="https://github.com/CodeEagle22/SIRITVIS",
     maintainer="Sagar Narwade",
     maintainer_email="sagarnarwade147@gmail.com",
@@ -32,29 +32,28 @@
         'gensim',
         'pyLDAvis==3.4.0',
         'matplotlib',
         'tweepy==3.9.0',
         'urllib3',
         'langdetect',
         'octis',
-        'topic-wizard==0.3.1',
         'scikit-learn==1.2.2',
         'folium==0.14.0',
         'pickle4==0.0.1',
         'plotly==5.15.0',
         'nltk==3.6.2',
         'notebook==6.5.5',
         'ipywidgets',
         'tensorflow',
         'vaderSentiment',
         'ipyleaflet',
         'geopy',
         'Flask==2.2.5',
         'Flask-Caching==2.0.1',
-        'wordcloud==1.8.2.2',
+        'wordcloud==1.9.2',
         'ipython==7.34.0',
         'textblob==0.15.3',
         'apify-client==1.4.0',
         'instagram_private_api==1.6.0'
     ],
     classifiers=[
         'Programming Language :: Python :: 3.10',
```

