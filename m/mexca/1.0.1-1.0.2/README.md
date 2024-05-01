# Comparing `tmp/mexca-1.0.1.tar.gz` & `tmp/mexca-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mexca-1.0.1.tar", last modified: Wed Jan 17 15:32:05 2024, max compression
+gzip compressed data, was "mexca-1.0.2.tar", last modified: Wed May  1 12:06:26 2024, max compression
```

## Comparing `mexca-1.0.1.tar` & `mexca-1.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:32:05.130931 mexca-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-17 15:31:38.000000 mexca-1.0.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-01-17 15:31:38.000000 mexca-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-17 15:31:38.000000 mexca-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-17 15:31:38.000000 mexca-1.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-01-17 15:32:05.130931 mexca-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-01-17 15:31:38.000000 mexca-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:32:05.118931 mexca-1.0.1/mexca/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:32:05.122931 mexca-1.0.1/mexca/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/audio/extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/audio/identification.py
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    38602 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:32:05.122931 mexca-1.0.1/mexca/text/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/text/sentiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/text/transcription.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:32:05.122931 mexca-1.0.1/mexca/video/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/video/anfl.py
--rw-r--r--   0 runner    (1001) docker     (127)    31826 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/video/extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/video/helper_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/video/mefarg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-01-17 15:31:38.000000 mexca-1.0.1/mexca/video/mefl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:32:05.126931 mexca-1.0.1/mexca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-01-17 15:32:05.000000 mexca-1.0.1/mexca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-01-17 15:32:05.000000 mexca-1.0.1/mexca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 15:32:05.000000 mexca-1.0.1/mexca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-17 15:32:05.000000 mexca-1.0.1/mexca.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 15:31:47.000000 mexca-1.0.1/mexca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-01-17 15:32:05.000000 mexca-1.0.1/mexca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-17 15:32:05.000000 mexca-1.0.1/mexca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-17 15:31:38.000000 mexca-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-01-17 15:32:05.134931 mexca-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-17 15:31:38.000000 mexca-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:32:05.126931 mexca-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_audio_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_audio_identification.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    17916 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_text_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_text_transcription.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_video_anfl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_video_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_video_helper_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_video_mefarg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-01-17 15:31:38.000000 mexca-1.0.1/tests/test_video_mefl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:26.578653 mexca-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-01 12:06:03.000000 mexca-1.0.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-01 12:06:03.000000 mexca-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 12:06:03.000000 mexca-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 12:06:03.000000 mexca-1.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-05-01 12:06:26.578653 mexca-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-01 12:06:03.000000 mexca-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:26.566653 mexca-1.0.2/mexca/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:26.566653 mexca-1.0.2/mexca/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/audio/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/audio/identification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38602 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:26.570653 mexca-1.0.2/mexca/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/text/sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/text/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:26.570653 mexca-1.0.2/mexca/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/video/anfl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32267 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/video/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/video/helper_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/video/mefarg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-05-01 12:06:03.000000 mexca-1.0.2/mexca/video/mefl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:26.574653 mexca-1.0.2/mexca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-05-01 12:06:26.000000 mexca-1.0.2/mexca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-01 12:06:26.000000 mexca-1.0.2/mexca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:06:26.000000 mexca-1.0.2/mexca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-01 12:06:26.000000 mexca-1.0.2/mexca.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:06:08.000000 mexca-1.0.2/mexca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-01 12:06:26.000000 mexca-1.0.2/mexca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 12:06:26.000000 mexca-1.0.2/mexca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-01 12:06:03.000000 mexca-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-01 12:06:26.578653 mexca-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 12:06:03.000000 mexca-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:06:26.574653 mexca-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_audio_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_audio_identification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17916 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_text_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_text_transcription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_video_anfl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_video_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_video_helper_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_video_mefarg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-01 12:06:03.000000 mexca-1.0.2/tests/test_video_mefl.py
```

### Comparing `mexca-1.0.1/CITATION.cff` & `mexca-1.0.2/CITATION.cff`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # YAML 1.2
 ---
-cff-version: "1.0.1"
+cff-version: "1.0.3"
 title: "mexca: Capture emotion expressions from multiple modalities in videos"
 authors:
   - family-names: Lüken
     given-names: Malte
     orcid: "https://orcid.org/0000-0001-7095-203X"
   - family-names: Viviani
     given-names: Eva
@@ -14,17 +14,17 @@
     orcid: "https://orcid.org/0000-0001-5666-1658"
   - family-names: Pipal
     given-names: Christian
     orcid: "https://orcid.org/0000-0002-5395-2035"
   - family-names: Schumacher
     given-names: Gijs
     orcid: "https://orcid.org/0000-0002-6503-4514"
-date-released: 2024-01-17
+date-released: 2024-05-01
 doi: 10.5281/zenodo.6976414
-version: "1.0.1"
+version: "1.0.3"
 repository-code: "https://github.com/mexca/mexca"
 keywords:
   - emotion
   - multimodal
   - expression
 message: "If you use this software, please cite it using these metadata."
 license: Apache-2.0
```

### Comparing `mexca-1.0.1/LICENSE` & `mexca-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/PKG-INFO` & `mexca-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mexca
-Version: 1.0.1
+Version: 1.0.2
 Summary: Emotion expression capture from multiple modalities.
 Home-page: https://github.com/mexca/mexca
 Author: Malte Luken
 Author-email: m.luken@esciencecenter.nl
 Project-URL: Bug Tracker, https://github.com/mexca/mexca/issues
 Keywords: emotion,multimodal,expression
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,17 +25,17 @@
 Requires-Dist: polars==0.19.8
 Requires-Dist: pydantic==2.4.2
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: srt>=3.5.2
 Requires-Dist: tqdm>=4.64.0
 Provides-Extra: vid
-Requires-Dist: facenet-pytorch==2.5.2; extra == "vid"
-Requires-Dist: gdown==4.6.0; extra == "vid"
+Requires-Dist: facenet-pytorch==2.5.3; extra == "vid"
 Requires-Dist: av==10.0; extra == "vid"
+Requires-Dist: huggingface-hub==0.17.3; extra == "vid"
 Requires-Dist: scikit-learn==1.3.1; extra == "vid"
 Requires-Dist: spectralcluster==0.2.16; extra == "vid"
 Requires-Dist: torch>=2.0; extra == "vid"
 Provides-Extra: spe
 Requires-Dist: pyannote.audio==3.1.1; extra == "spe"
 Requires-Dist: pyannote.core>=5.0; extra == "spe"
 Requires-Dist: torch>=2.0; extra == "spe"
@@ -95,14 +95,18 @@
 
 <div align="center">
 <img src="mexca_logo.png" width="400">
 </div>
 
 mexca is an open-source Python package which aims to capture human emotion expressions from videos in a single pipeline.
 
+Check out our preprint:
+
+Lüken, M., Moodley, K., Viviani, E., Pipal, C., & Schumacher, G. (2024, January 18). MEXCA - A simple and robust pipeline for capturing emotion expressions in faces, vocalization, and speech. *PsyArXiv*. https://doi.org/10.31234/osf.io/56svb
+
 ## How To Use Mexca
 
 mexca implements the customizable yet easy-to-use Multimodal Emotion eXpression Capture Amsterdam (MEXCA) pipeline for extracting emotion expression features from videos.
 It contains building blocks that can be used to extract features for individual modalities (i.e., facial expressions, voice, and dialogue/spoken text).
 The blocks can also be integrated into a single pipeline to extract the features from all modalities at once.
 Next to extracting features, mexca can also identify the speakers shown in the video by clustering speaker and face representations.
 This allows users to compare emotion expressions across speakers, time, and contexts.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mexca-1.0.1/README.md` & `mexca-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 <div align="center">
 <img src="mexca_logo.png" width="400">
 </div>
 
 mexca is an open-source Python package which aims to capture human emotion expressions from videos in a single pipeline.
 
+Check out our preprint:
+
+Lüken, M., Moodley, K., Viviani, E., Pipal, C., & Schumacher, G. (2024, January 18). MEXCA - A simple and robust pipeline for capturing emotion expressions in faces, vocalization, and speech. *PsyArXiv*. https://doi.org/10.31234/osf.io/56svb
+
 ## How To Use Mexca
 
 mexca implements the customizable yet easy-to-use Multimodal Emotion eXpression Capture Amsterdam (MEXCA) pipeline for extracting emotion expression features from videos.
 It contains building blocks that can be used to extract features for individual modalities (i.e., facial expressions, voice, and dialogue/spoken text).
 The blocks can also be integrated into a single pipeline to extract the features from all modalities at once.
 Next to extracting features, mexca can also identify the speakers shown in the video by clustering speaker and face representations.
 This allows users to compare emotion expressions across speakers, time, and contexts.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mexca-1.0.1/mexca/audio/extraction.py` & `mexca-1.0.2/mexca/audio/extraction.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/mexca/audio/identification.py` & `mexca-1.0.2/mexca/audio/identification.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/mexca/container.py` & `mexca-1.0.2/mexca/container.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/mexca/data.py` & `mexca-1.0.2/mexca/data.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/mexca/pipeline.py` & `mexca-1.0.2/mexca/pipeline.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/mexca/text/sentiment.py` & `mexca-1.0.2/mexca/text/sentiment.py`

 * *Files 16% similar despite different names*

```diff
@@ -117,30 +117,36 @@
         )
 
         for i, sent in tqdm(
             enumerate(transcription.segments),
             total=len(transcription.segments),
             disable=not show_progress,
         ):
-            self.logger.debug("Extracting sentiment for sentence %s", i)
-            tokens = self.tokenizer(sent.data.text, return_tensors="pt").to(
-                self.device
-            )
-            output = self.classifier(**tokens)
-            logits = output.logits.detach().cpu().numpy()
-            scores = softmax(logits)[0]
+            # Catch extremely rare tokenization errors
+            try:
+                self.logger.debug("Extracting sentiment for sentence %s", i)
+                # Add padding to prevent tensor size mismatch runtime error
+                tokens = self.tokenizer(
+                    sent.data.text, padding=True, return_tensors="pt"
+                ).to(self.device)
+                output = self.classifier(**tokens)
+                logits = output.logits.detach().cpu().numpy()
+                scores = softmax(logits)[0]
+            except RuntimeError:
+                scores = (None, None, None)
+
             sentiment_annotation.segments.add(
                 Interval(
                     begin=sent.begin,
                     end=sent.end,
                     data=SentimentData(
                         text=sent.data.text,
-                        pos=float(scores[2]),
-                        neg=float(scores[0]),
-                        neu=float(scores[1]),
+                        pos=scores[2],
+                        neg=scores[0],
+                        neu=scores[1],
                     ),
                 )
             )
 
         del self.classifier
 
         return sentiment_annotation
```

### Comparing `mexca-1.0.1/mexca/text/transcription.py` & `mexca-1.0.2/mexca/text/transcription.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/mexca/utils.py` & `mexca-1.0.2/mexca/utils.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/mexca/video/anfl.py` & `mexca-1.0.2/mexca/video/anfl.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/mexca/video/extraction.py` & `mexca-1.0.2/mexca/video/extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,17 @@
         costs for long videos.
     embeddings_model : {'vggface2', 'casia-webface'}, default='vggface2'
         Pretrained Inception Resnet V1 model for computing face embeddings.
     post_min_face_size : tuple, default=(45.0, 45.0)
         Minimal width and height (in pixels) for filtering out faces after detection.
         This can be useful to exclude small faces before clustering their embeddings
         and can improve clustering performance.
+    au_model : str, optional, default=None
+        Pretrained MEFARG model on Hugging Face Hub for extraction facial action unit activations. If `None`, uses the default model
+        `mexca/mefarg-open-graph-au-resnet50-stage-2`.
 
 
     """
 
     def __init__(
         self,
         num_faces: Optional[int],
@@ -224,14 +227,15 @@
         select_largest: bool = True,
         selection_method: Optional[str] = None,
         keep_all: bool = True,
         device: torch.device = torch.device(type="cpu"),
         max_cluster_frames: Optional[int] = None,
         embeddings_model: str = "vggface2",
         post_min_face_size: Tuple[float, float] = (45.0, 45.0),
+        au_model: Optional[str] = None,
     ):
         self.logger = logging.getLogger("mexca.video.FaceExtractor")
         self.min_face_size = min_face_size
         self.thresholds = thresholds
         self.factor = factor
         self.post_process = post_process
         self.select_largest = select_largest
@@ -240,14 +244,19 @@
         self.logger.debug("Initializing FaceExtractor on device %s", device)
         self.device = device
         self.embeddings_model = embeddings_model
         self.num_faces = num_faces
         self.max_cluster_frames = max_cluster_frames
         self.post_min_face_size = post_min_face_size
 
+        if au_model is None:
+            au_model = "mexca/mefarg-open-graph-au-resnet50-stage-2"
+
+        self.au_model = au_model
+
         # Lazy initialization: See getter functions
         self._detector = None
         self._encoder = None
         self._clusterer = None
         self._extractor = None
 
         self.logger.debug(ClassInitMessage())
@@ -318,16 +327,17 @@
     @property
     def extractor(self) -> MEFARG:
         """The MEFARG model for extracting action unit activations.
         See ME-GraphAU `model <https://github.com/CVI-SZU/ME-GraphAU>`_ and
         `paper <https://arxiv.org/abs/2205.01782>`_ for details.
         """
         if not self._extractor:
-            self._extractor = MEFARG.from_pretrained(device=self.device)
-            self._extractor.eval()
+            self._extractor = MEFARG.from_pretrained(self.au_model).to(
+                self.device
+            )
             self.logger.debug(
                 "Initialized MEFARG action unit feature extractor"
             )
         return self._extractor
 
     @extractor.deleter
     def extractor(self):
@@ -494,17 +504,17 @@
                     normalize,
                 ]
             )
 
             frm = transform(frm)
 
             with torch.no_grad():
-                aus = self.extractor(frm)
+                aus = self.extractor(frm.to(self.device))
 
-            aus_list.append(aus.numpy())
+            aus_list.append(aus.detach().cpu().numpy())
 
         return np.array(aus_list)
 
     @staticmethod
     def _compute_centroids(
         embs: np.ndarray, labels: np.ndarray
     ) -> Tuple[List[np.ndarray], Dict[Union[str, int, float], int]]:
```

### Comparing `mexca-1.0.1/mexca/video/helper_classes.py` & `mexca-1.0.2/mexca/video/helper_classes.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/mexca/video/mefl.py` & `mexca-1.0.2/mexca/video/mefl.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/mexca.egg-info/PKG-INFO` & `mexca-1.0.2/mexca.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mexca
-Version: 1.0.1
+Version: 1.0.2
 Summary: Emotion expression capture from multiple modalities.
 Home-page: https://github.com/mexca/mexca
 Author: Malte Luken
 Author-email: m.luken@esciencecenter.nl
 Project-URL: Bug Tracker, https://github.com/mexca/mexca/issues
 Keywords: emotion,multimodal,expression
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,17 +25,17 @@
 Requires-Dist: polars==0.19.8
 Requires-Dist: pydantic==2.4.2
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: srt>=3.5.2
 Requires-Dist: tqdm>=4.64.0
 Provides-Extra: vid
-Requires-Dist: facenet-pytorch==2.5.2; extra == "vid"
-Requires-Dist: gdown==4.6.0; extra == "vid"
+Requires-Dist: facenet-pytorch==2.5.3; extra == "vid"
 Requires-Dist: av==10.0; extra == "vid"
+Requires-Dist: huggingface-hub==0.17.3; extra == "vid"
 Requires-Dist: scikit-learn==1.3.1; extra == "vid"
 Requires-Dist: spectralcluster==0.2.16; extra == "vid"
 Requires-Dist: torch>=2.0; extra == "vid"
 Provides-Extra: spe
 Requires-Dist: pyannote.audio==3.1.1; extra == "spe"
 Requires-Dist: pyannote.core>=5.0; extra == "spe"
 Requires-Dist: torch>=2.0; extra == "spe"
@@ -95,14 +95,18 @@
 
 <div align="center">
 <img src="mexca_logo.png" width="400">
 </div>
 
 mexca is an open-source Python package which aims to capture human emotion expressions from videos in a single pipeline.
 
+Check out our preprint:
+
+Lüken, M., Moodley, K., Viviani, E., Pipal, C., & Schumacher, G. (2024, January 18). MEXCA - A simple and robust pipeline for capturing emotion expressions in faces, vocalization, and speech. *PsyArXiv*. https://doi.org/10.31234/osf.io/56svb
+
 ## How To Use Mexca
 
 mexca implements the customizable yet easy-to-use Multimodal Emotion eXpression Capture Amsterdam (MEXCA) pipeline for extracting emotion expression features from videos.
 It contains building blocks that can be used to extract features for individual modalities (i.e., facial expressions, voice, and dialogue/spoken text).
 The blocks can also be integrated into a single pipeline to extract the features from all modalities at once.
 Next to extracting features, mexca can also identify the speakers shown in the video by clustering speaker and face representations.
 This allows users to compare emotion expressions across speakers, time, and contexts.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mexca-1.0.1/mexca.egg-info/SOURCES.txt` & `mexca-1.0.2/mexca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/setup.cfg` & `mexca-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	expression
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = mexca
 project_urls = 
 	Bug Tracker = https://github.com/mexca/mexca/issues
 url = https://github.com/mexca/mexca
-version = 1.0.1
+version = 1.0.2
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 python_requires = >3.7,<3.11
 install_requires = 
@@ -47,17 +47,17 @@
 	transcribe = mexca.text.transcription:cli
 	extract-sentiment = mexca.text.sentiment:cli
 
 [options.data_files]
 
 [options.extras_require]
 vid = 
-	facenet-pytorch==2.5.2
-	gdown==4.6.0
+	facenet-pytorch==2.5.3
 	av==10.0
+	huggingface-hub==0.17.3
 	scikit-learn==1.3.1
 	spectralcluster==0.2.16
 	torch>=2.0
 spe = 
 	pyannote.audio==3.1.1
 	pyannote.core>=5.0
 	torch>=2.0
```

### Comparing `mexca-1.0.1/tests/test_audio_extraction.py` & `mexca-1.0.2/tests/test_audio_extraction.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/tests/test_audio_identification.py` & `mexca-1.0.2/tests/test_audio_identification.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/tests/test_container.py` & `mexca-1.0.2/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/tests/test_data.py` & `mexca-1.0.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/tests/test_pipeline.py` & `mexca-1.0.2/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/tests/test_text_sentiment.py` & `mexca-1.0.2/tests/test_text_sentiment.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/tests/test_text_transcription.py` & `mexca-1.0.2/tests/test_text_transcription.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/tests/test_utils.py` & `mexca-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/tests/test_video_anfl.py` & `mexca-1.0.2/tests/test_video_anfl.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/tests/test_video_extraction.py` & `mexca-1.0.2/tests/test_video_extraction.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/tests/test_video_helper_classes.py` & `mexca-1.0.2/tests/test_video_helper_classes.py`

 * *Files identical despite different names*

### Comparing `mexca-1.0.1/tests/test_video_mefl.py` & `mexca-1.0.2/tests/test_video_mefl.py`

 * *Files identical despite different names*

