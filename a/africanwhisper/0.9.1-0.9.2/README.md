# Comparing `tmp/africanwhisper-0.9.1.tar.gz` & `tmp/africanwhisper-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.9.1.tar", last modified: Fri Apr 26 18:33:56 2024, max compression
+gzip compressed data, was "africanwhisper-0.9.2.tar", max compression
```

## Comparing `africanwhisper-0.9.1.tar` & `africanwhisper-0.9.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.398248 africanwhisper-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-04-26 18:33:56.398248 africanwhisper-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-26 18:33:56.398248 africanwhisper-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.390248 africanwhisper-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.394248 africanwhisper-0.9.1/src/africanwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-04-26 18:33:56.000000 africanwhisper-0.9.1/src/africanwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-26 18:33:56.000000 africanwhisper-0.9.1/src/africanwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:33:56.000000 africanwhisper-0.9.1/src/africanwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-26 18:33:56.000000 africanwhisper-0.9.1/src/africanwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 18:33:56.000000 africanwhisper-0.9.1/src/africanwhisper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.394248 africanwhisper-0.9.1/src/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/peft_speech_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/peft_speech_inference_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/speech_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/speech_inference_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/deployment/transcription_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.394248 africanwhisper-0.9.1/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_audio_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_model_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/tests/test_transcription_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:56.394248 africanwhisper-0.9.1/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/audio_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/gradio_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/gradio_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/wandb_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-26 18:33:52.000000 africanwhisper-0.9.1/src/training/whisper_model_prep.py
+-rw-r--r--   0        0        0     1067 2024-05-01 10:55:03.102471 africanwhisper-0.9.2/LICENSE
+-rw-r--r--   0        0        0    11868 2024-05-01 10:55:03.102471 africanwhisper-0.9.2/README.md
+-rw-r--r--   0        0        0     1248 2024-05-01 10:55:03.110471 africanwhisper-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     8196 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/.DS_Store
+-rw-r--r--   0        0        0       60 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/.dockerignore
+-rw-r--r--   0        0        0      100 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/.env
+-rw-r--r--   0        0        0      361 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/Dockerfile
+-rw-r--r--   0        0        0        0 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/__init__.py
+-rw-r--r--   0        0        0     7479 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/app.py
+-rw-r--r--   0        0        0    11598 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/dashboard.json
+-rw-r--r--   0        0        0      538 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/docker-compose.yaml
+-rw-r--r--   0        0        0        0 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/__init__.py
+-rw-r--r--   0        0        0    18321 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/alignment.py
+-rw-r--r--   0        0        0    11001 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/asr.py
+-rw-r--r--   0        0        0     4894 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/audio.py
+-rw-r--r--   0        0        0     3276 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/diarize.py
+-rw-r--r--   0        0        0     3759 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/load_asr_model.py
+-rw-r--r--   0        0        0     4271 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/mel_filters.npz
+-rw-r--r--   0        0        0     9103 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/subtitles_processor.py
+-rw-r--r--   0        0        0     1126 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/types.py
+-rw-r--r--   0        0        0    14411 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/utils.py
+-rw-r--r--   0        0        0    11354 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/faster_whisper/vad.py
+-rw-r--r--   0        0        0     2847 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/main.py
+-rw-r--r--   0        0        0     3537 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/peft_speech_inference.py
+-rw-r--r--   0        0        0     1064 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/peft_speech_inference_cli.py
+-rw-r--r--   0        0        0      136 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/prometheus.yml
+-rw-r--r--   0        0        0      231 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/requirements.txt
+-rw-r--r--   0        0        0     7667 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/speech_inference.py
+-rw-r--r--   0        0        0     2451 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/speech_inference_cli.py
+-rw-r--r--   0        0        0     2027 2024-05-01 10:55:03.118471 africanwhisper-0.9.2/src/deployment/transcription_model.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/__init__.py
+-rw-r--r--   0        0        0     1910 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/audio_data_processor.py
+-rw-r--r--   0        0        0     1986 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/collator.py
+-rw-r--r--   0        0        0     4819 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/data_prep.py
+-rw-r--r--   0        0        0     1806 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/evaluation.py
+-rw-r--r--   0        0        0      688 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/gradio_demo.py
+-rw-r--r--   0        0        0     6318 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/gradio_inference.py
+-rw-r--r--   0        0        0     2595 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/load_data.py
+-rw-r--r--   0        0        0     2592 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/main.py
+-rw-r--r--   0        0        0     7356 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/model_trainer.py
+-rw-r--r--   0        0        0     7952 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/wandb_callback.py
+-rw-r--r--   0        0        0     4336 2024-05-01 10:55:03.122471 africanwhisper-0.9.2/src/training/whisper_model_prep.py
+-rw-r--r--   0        0        0    13625 1970-01-01 00:00:00.000000 africanwhisper-0.9.2/PKG-INFO
```

### Comparing `africanwhisper-0.9.1/LICENSE` & `africanwhisper-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/PKG-INFO` & `africanwhisper-0.9.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,7 @@
-Metadata-Version: 2.1
-Name: africanwhisper
-Version: 0.9.1
-Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
-Home-page: https://github.com/KevKibe/African-Whisper
-Author: Kevin Kibe
-Author-email: keviinkibe@gmail.com
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pip==24.0
-Requires-Dist: transformers==4.39.2
-Requires-Dist: datasets==2.17.0
-Requires-Dist: librosa==0.10.1
-Requires-Dist: evaluate==0.4.1
-Requires-Dist: jiwer==3.0.3
-Requires-Dist: bitsandbytes==0.42.0
-Requires-Dist: accelerate==0.28.0
-Requires-Dist: peft==0.9.0
-Requires-Dist: numpy==1.26.4
-Requires-Dist: wandb==0.16.6
-Requires-Dist: holoviews==1.18.3
-Requires-Dist: panel==1.3.8
-Requires-Dist: gradio==4.24.0
-Requires-Dist: pytube==15.0.0
-Requires-Dist: tf-keras==2.16.0
-Requires-Dist: tensorflow==2.16.1
-Requires-Dist: keras==3.1.1
-Requires-Dist: scipy==1.12.0
-Requires-Dist: tensorflow-probability==0.24.0
-Requires-Dist: yt-dlp==2023.11.14
-Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: faster-whisper==1.0.0
-Requires-Dist: pyannote.audio==3.1.1
-Requires-Dist: nltk==3.8.1
-Requires-Dist: torchvision==0.17.2
-Requires-Dist: ctranslate2==4.1.0
-Requires-Dist: pandas==2.2.1
-
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
   <a href="https://github.com/KevKibe/African-Whisper/commits/">
@@ -141,16 +101,18 @@
 
 ## Step 4: Preprocess the Dataset
 ```python
 # Load and preprocess the dataset
 processed_dataset = process.load_dataset(
     feature_extractor=feature_extractor,
     tokenizer=tokenizer,
-    processor=feature_processor
-)
+    processor=feature_processor,
+    num_samples = None # Number of samples to load from each dataset
+                       # Set None to load the entire dataset
+                       # Example: num_samples = 100 will load 100 samples from each dataset
 ```
 
 ## Step 5: Train the Model
 
 ```python
 from training.model_trainer import Trainer
 
@@ -192,15 +154,16 @@
 demo = WhisperDemo(model_name, huggingface_read_token)
 demo.generate_demo()
 ```
 
 ## Step 7: Test Model using Audio File
 
 ```python
-from deployment.speech_inference import SpeechInference
+# Using a PEFT fine-tuned model
+from deployment.peft_speech_inference import SpeechInference
 
 model_name = "your-finetuned-model-name-on-huggingface-hub"   # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " "
 task = "desired-task"                                         # either 'translate' or 'transcribe'
 audiofile_dir = "location-of-audio-file"                      # filetype should be .mp3 or .wav
 
 # Initialize the SpeechInference class and run inference
@@ -211,17 +174,52 @@
 # Access different parts of the output
 print(transcription.text)                                       # The entire text transcription.
 print(transcription.chunks)                                     # List of individual text chunks with timestamps.
 print(transcription.timestamps)                                 # List of timestamps for each chunk.
 print(transcription.chunk_texts)                                # List of texts for each chunk.
 
 ```
+```python
+# Using a fully fine-tuned model
+from deployment.speech_inference import SpeechTranscriptionPipeline, ModelOptimization
+
+model_name = "your-finetuned-model-name-on-huggingface-hub"   # e.g., "KevinKibe/whisper-small-af"
+huggingface_read_token = " "
+task = "desired-task"                                         # either 'translate' or 'transcribe'
+audiofile_dir = "location-of-audio-file"                      # filetype should be .mp3 or .wav
+
+# Optimize model for better results
+model_optimizer = ModelOptimization(model_name=model_name)
+model_optimizer.convert_model_to_optimized_format()
+model = model_optimizer.load_transcription_model()
+
+# Initiate the transcription model
+inference = SpeechTranscriptionPipeline(
+        audio_file_path=audiofile_dir,
+        task=task,
+        huggingface_read_token=huggingface_read_token
+    )
+
+# To get transcriptions
+transcription = inference.transcribe_audio(model=model)
+print(transcription)
+
+# To get transcriptions with speaker labels
+alignment_result = inference.align_transcription(transcription)
+diarization_result = inference.diarize_audio(alignment_result)
+print(diarization_result)
+
+#To generate subtitles(.srt format), will be saved in root directory
+inference.generate_subtitles(transcription, alignment_result, diarization_result)
+```
 
 # 🖥️ Using the CLI
 
+## Step 1: Clone and Install Dependencies
+
 - Clone the Repository: Clone or download the application code to your local machine.
 ```bash
 git clone https://github.com/KevKibe/African-Whisper.git
 ```
 
 - Create a virtual environment for the project and activate it.
 ```bash
@@ -234,22 +232,28 @@
 pip install -r requirements.txt
 ```
 - Navigate to:
 ```bash
 cd src
 ```
 
+## Step 2: Finetune the Model
+
 - To start the training , use the following command:
 ```bash
-python -m training.main --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --language_abbr LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft # leave this out to opt-out of using PEFT
+python -m training.main --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --language_abbr LANGUAGE_ABBREVIATION LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft
+
+Flags:
+# --use_peft: Optional flag to use PEFT finetuning. leave it out to perform full finetuning
 ```
 - Find a description of these commands [here](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/PARAMETERS.md).
 
-### Inference
+## Step 3: Get Inference
 
+### Install ffmpeg
 - To get inference from your fine-tuned model, follow these steps:
 
 - Ensure that ffmpeg is installed by running the following commands:
 
 ```bash
 # on Ubuntu or Debian
 sudo apt update && sudo apt install ffmpeg
@@ -262,43 +266,49 @@
 
 # on Windows using Chocolatey (https://chocolatey.org/)
 choco install ffmpeg
 
 # on Windows using Scoop (https://scoop.sh/)
 scoop install ffmpeg
 ```
+### To get inference on Gradio UI
 
-- To get the Gradio inference URL:
+- To get the Gradio UI URL:
 ```bash
 python -m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE 
 ```
 - **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
 - **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
 
-
+### To get inference on CLI
 ```bash
 cd src/deployment
 ```
 - Create a `.env` file using `nano .env` command and add these keys and save the file.
 ```python
 MODEL_NAME = "your-finetuned-model"
 HUGGINGFACE_READ_TOKEN = "huggingface-read-token"
 ```
 
 - To perform transcriptions and translations:
 
 ```bash
-# If your model is peft finetuned
-python -m deployment.peft_speech_inference_cli --audio_file audio-filename --task 
+# PEFT FINETUNED MODELS
+python -m deployment.peft_speech_inference_cli --audio_file FILENAME --task TASK 
+
+# FULLY FINETUNED MODELS
+python -m deployment.speech_inference_cli --audio_file FILENAME --task TASK --perform_diarization --perform_alignment
+
+Flags:
+# --perform_diarization: Optional flag to perform speaker diarization.
+# --perform_alignment: Optional flag to perform alignment.
 
-# If your model is fully finetuned
-python -m deployment.speech_inference_cli --audio_file audio-filename --task task --perform_diarization --perform_alignment
 ```
 
-## 🛳️ Deployment
+## 🛳️ Step 4: Deployment
 
 - To deploy your fine-tuned model as a REST API endpoint, follow these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
 
 
 ## Contributing 
 Contributions are welcome and encouraged.
```

#### html2text {}

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.9.1 Summary: A package
-for fast fine-tuning and API endpoint deployment of Whisper model specifically
-developed to accelerate Automatic Speech Recognition(ASR) for African
-Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
-Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.0
-Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
-jiwer==3.0.3 Requires-Dist: bitsandbytes==0.42.0 Requires-Dist:
-accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: numpy==1.26.4
-Requires-Dist: wandb==0.16.6 Requires-Dist: holoviews==1.18.3 Requires-Dist:
-panel==1.3.8 Requires-Dist: gradio==4.24.0 Requires-Dist: pytube==15.0.0
-Requires-Dist: tf-keras==2.16.0 Requires-Dist: tensorflow==2.16.1 Requires-
-Dist: keras==3.1.1 Requires-Dist: scipy==1.12.0 Requires-Dist: tensorflow-
-probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14 Requires-Dist: python-
-dotenv==1.0.1 Requires-Dist: faster-whisper==1.0.0 Requires-Dist:
-pyannote.audio==3.1.1 Requires-Dist: nltk==3.8.1 Requires-Dist:
-torchvision==0.17.2 Requires-Dist: ctranslate2==4.1.0 Requires-Dist:
-pandas==2.2.1
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 *Enhancing Automatic Speech Recognition (ASR): translation and transcription
 capabilities for African languages by providing seamless fine-tuning and
 deploying pipelines for Whisper Model*.
 ![Diagram](diagram-1.png) ## Features - ð§ Fine-tune the [Whisper](https://
@@ -61,81 +42,104 @@
 Step 3: Prepare the Model ```python from training.data_prep import DataPrep #
 Initialize the DataPrep class and prepare the model process = DataPrep
 ( huggingface_read_token, dataset_name, language_abbr, model_id,
 processing_task, use_peft ) tokenizer, feature_extractor, feature_processor,
 model = process.prepare_model() ``` ## Step 4: Preprocess the Dataset ```python
 # Load and preprocess the dataset processed_dataset = process.load_dataset
 ( feature_extractor=feature_extractor, tokenizer=tokenizer,
-processor=feature_processor ) ``` ## Step 5: Train the Model ```python from
-training.model_trainer import Trainer # Initialize the Trainer class and train
-the model trainer = Trainer( huggingface_write_token, model_id,
+processor=feature_processor, num_samples = None # Number of samples to load
+from each dataset # Set None to load the entire dataset # Example: num_samples
+= 100 will load 100 samples from each dataset ``` ## Step 5: Train the Model
+```python from training.model_trainer import Trainer # Initialize the Trainer
+class and train the model trainer = Trainer( huggingface_write_token, model_id,
 processed_dataset, model, feature_processor, feature_extractor, tokenizer,
 wandb_api_key, use_peft ) trainer.train( max_steps=100, learning_rate=1e-3,
 per_device_train_batch_size=96, per_device_eval_batch_size=64,
 optim="adamw_bnb_8bit" ) # Optional parameters for training: # max_steps (int):
 The maximum number of training steps (default is 100). # learning_rate (float):
 The learning rate for training (default is 1e-5). # per_device_train_batch_size
 (int): The batch size per GPU for training (default is 96). #
 per_device_eval_batch_size (int): The batch size per GPU for evaluation
 (default is 64). # optim (str): The optimizer used for training (default is
 "adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI ```python from
 training.gradio_inference import WhisperDemo # Generate a demo model_name =
 "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-
 small-af" demo = WhisperDemo(model_name, huggingface_read_token)
-demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python from
-deployment.speech_inference import SpeechInference model_name = "your-
+demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python #
+Using a PEFT fine-tuned model from deployment.peft_speech_inference import
+SpeechInference model_name = "your-finetuned-model-name-on-huggingface-hub" #
+e.g., "KevinKibe/whisper-small-af" huggingface_read_token = " " task =
+"desired-task" # either 'translate' or 'transcribe' audiofile_dir = "location-
+of-audio-file" # filetype should be .mp3 or .wav # Initialize the
+SpeechInference class and run inference inference = SpeechInference(model_name,
+huggingface_read_token) pipeline = inference.pipe_initialization()
+transcription = inference.output(pipeline, audiofile_dir, task) # Access
+different parts of the output print(transcription.text) # The entire text
+transcription. print(transcription.chunks) # List of individual text chunks
+with timestamps. print(transcription.timestamps) # List of timestamps for each
+chunk. print(transcription.chunk_texts) # List of texts for each chunk. ```
+```python # Using a fully fine-tuned model from deployment.speech_inference
+import SpeechTranscriptionPipeline, ModelOptimization model_name = "your-
 finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " " task = "desired-task" # either 'translate' or
 'transcribe' audiofile_dir = "location-of-audio-file" # filetype should be .mp3
-or .wav # Initialize the SpeechInference class and run inference inference =
-SpeechInference(model_name, huggingface_read_token) pipeline =
-inference.pipe_initialization() transcription = inference.output(pipeline,
-audiofile_dir, task) # Access different parts of the output print
-(transcription.text) # The entire text transcription. print
-(transcription.chunks) # List of individual text chunks with timestamps. print
-(transcription.timestamps) # List of timestamps for each chunk. print
-(transcription.chunk_texts) # List of texts for each chunk. ``` # ð¥ï¸ Using
-the CLI - Clone the Repository: Clone or download the application code to your
-local machine. ```bash git clone https://github.com/KevKibe/African-Whisper.git
-``` - Create a virtual environment for the project and activate it. ```bash
-python3 -m venv env source venv/bin/activate ``` - Install dependencies by
-running this command ```bash pip install -r requirements.txt ``` - Navigate to:
-```bash cd src ``` - To start the training , use the following command: ```bash
-python -m training.main --huggingface_read_token
-YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token
-YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --
-language_abbr LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task
-PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft # leave this
-out to opt-out of using PEFT ``` - Find a description of these commands [here]
-(https://github.com/KevKibe/African-Whisper/blob/master/DOCS/PARAMETERS.md).
-### Inference - To get inference from your fine-tuned model, follow these
-steps: - Ensure that ffmpeg is installed by running the following commands:
-```bash # on Ubuntu or Debian sudo apt update && sudo apt install ffmpeg # on
-Arch Linux sudo pacman -S ffmpeg # on MacOS using Homebrew (https://brew.sh/
-) brew install ffmpeg # on Windows using Chocolatey (https://chocolatey.org/
-) choco install ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop
-install ffmpeg ``` - To get the Gradio inference URL: ```bash python -
+or .wav # Optimize model for better results model_optimizer = ModelOptimization
+(model_name=model_name) model_optimizer.convert_model_to_optimized_format()
+model = model_optimizer.load_transcription_model() # Initiate the transcription
+model inference = SpeechTranscriptionPipeline( audio_file_path=audiofile_dir,
+task=task, huggingface_read_token=huggingface_read_token ) # To get
+transcriptions transcription = inference.transcribe_audio(model=model) print
+(transcription) # To get transcriptions with speaker labels alignment_result =
+inference.align_transcription(transcription) diarization_result =
+inference.diarize_audio(alignment_result) print(diarization_result) #To
+generate subtitles(.srt format), will be saved in root directory
+inference.generate_subtitles(transcription, alignment_result,
+diarization_result) ``` # ð¥ï¸ Using the CLI ## Step 1: Clone and Install
+Dependencies - Clone the Repository: Clone or download the application code to
+your local machine. ```bash git clone https://github.com/KevKibe/African-
+Whisper.git ``` - Create a virtual environment for the project and activate it.
+```bash python3 -m venv env source venv/bin/activate ``` - Install dependencies
+by running this command ```bash pip install -r requirements.txt ``` - Navigate
+to: ```bash cd src ``` ## Step 2: Finetune the Model - To start the training ,
+use the following command: ```bash python -m training.main --
+huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE --
+huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name
+AUDIO_DATASET_NAME --language_abbr LANGUAGE_ABBREVIATION LANGUAGE_ABBREVIATION
+--model_id MODEL_ID --processing_task PROCESSING_TASK --wandb_api_key
+YOUR_WANDB_API_KEY_HERE --use_peft Flags: # --use_peft: Optional flag to use
+PEFT finetuning. leave it out to perform full finetuning ``` - Find a
+description of these commands [here](https://github.com/KevKibe/African-
+Whisper/blob/master/DOCS/PARAMETERS.md). ## Step 3: Get Inference ### Install
+ffmpeg - To get inference from your fine-tuned model, follow these steps: -
+Ensure that ffmpeg is installed by running the following commands: ```bash # on
+Ubuntu or Debian sudo apt update && sudo apt install ffmpeg # on Arch Linux
+sudo pacman -S ffmpeg # on MacOS using Homebrew (https://brew.sh/) brew install
+ffmpeg # on Windows using Chocolatey (https://chocolatey.org/) choco install
+ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop install ffmpeg ```
+### To get inference on Gradio UI - To get the Gradio UI URL: ```bash python -
 m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --
 huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE ``` - **--
 model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
 This should match the model's identifier on the Hugging Face Model Hub. - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face.
-```bash cd src/deployment ``` - Create a `.env` file using `nano .env` command
-and add these keys and save the file. ```python MODEL_NAME = "your-finetuned-
-model" HUGGINGFACE_READ_TOKEN = "huggingface-read-token" ``` - To perform
-transcriptions and translations: ```bash # If your model is peft finetuned
-python -m deployment.peft_speech_inference_cli --audio_file audio-filename --
-task # If your model is fully finetuned python -
-m deployment.speech_inference_cli --audio_file audio-filename --task task --
-perform_diarization --perform_alignment ``` ## ð³ï¸ Deployment - To deploy
-your fine-tuned model as a REST API endpoint, follow these [instructions]
-(https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
-Contributing Contributions are welcome and encouraged. Before contributing,
-please take a moment to review our [Contribution Guidelines](https://
-github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for
-important information on how to contribute to this project. If you're unsure
-about anything or need assistance, don't hesitate to reach out to us or open an
-issue to discuss your ideas. We look forward to your contributions! ## License
-This project is licensed under the MIT License - see the [LICENSE](https://
-github.com/KevKibe/African-Whisper/blob/main/LICENSE) file for details. ##
-Contact For any enquiries, please reach out to me through keviinkibe@gmail.com
+access. It allows you to download datasets and models from Hugging Face. ### To
+get inference on CLI ```bash cd src/deployment ``` - Create a `.env` file using
+`nano .env` command and add these keys and save the file. ```python MODEL_NAME
+= "your-finetuned-model" HUGGINGFACE_READ_TOKEN = "huggingface-read-token" ```
+- To perform transcriptions and translations: ```bash # PEFT FINETUNED MODELS
+python -m deployment.peft_speech_inference_cli --audio_file FILENAME --task
+TASK # FULLY FINETUNED MODELS python -m deployment.speech_inference_cli --
+audio_file FILENAME --task TASK --perform_diarization --perform_alignment
+Flags: # --perform_diarization: Optional flag to perform speaker diarization. #
+--perform_alignment: Optional flag to perform alignment. ``` ## ð³ï¸ Step 4:
+Deployment - To deploy your fine-tuned model as a REST API endpoint, follow
+these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/
+DOCS/deployment.md). ## Contributing Contributions are welcome and encouraged.
+Before contributing, please take a moment to review our [Contribution
+Guidelines](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/
+CONTRIBUTING.md) for important information on how to contribute to this
+project. If you're unsure about anything or need assistance, don't hesitate to
+reach out to us or open an issue to discuss your ideas. We look forward to your
+contributions! ## License This project is licensed under the MIT License - see
+the [LICENSE](https://github.com/KevKibe/African-Whisper/blob/main/LICENSE)
+file for details. ## Contact For any enquiries, please reach out to me through
+keviinkibe@gmail.com
```

### Comparing `africanwhisper-0.9.1/src/africanwhisper.egg-info/PKG-INFO` & `africanwhisper-0.9.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.9.1
-Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
+Version: 0.9.2
+Summary: A package for fast fine-tuning and API endpoint deployment of the Whisper model, specifically developed to accelerate Automatic Speech Recognition (ASR) for African languages.
 Home-page: https://github.com/KevKibe/African-Whisper
+License: MIT
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
-License: MIT
-Requires-Python: >=3.8
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: accelerate (==0.28.0)
+Requires-Dist: bitsandbytes (==0.42.0)
+Requires-Dist: ctranslate2 (==4.1.0)
+Requires-Dist: datasets (==2.17.0)
+Requires-Dist: evaluate (==0.4.1)
+Requires-Dist: faster-whisper (==1.0.0)
+Requires-Dist: gradio (==4.24.0)
+Requires-Dist: holoviews (==1.18.3)
+Requires-Dist: jiwer (==3.0.3)
+Requires-Dist: keras (==3.1.1)
+Requires-Dist: librosa (==0.10.1)
+Requires-Dist: nltk (==3.8.1)
+Requires-Dist: numpy (==1.26.4)
+Requires-Dist: pandas (==2.0.3)
+Requires-Dist: panel (==1.3.8)
+Requires-Dist: peft (==0.9.0)
+Requires-Dist: pyannote-audio (==3.1.1)
+Requires-Dist: python-dotenv (==1.0.1)
+Requires-Dist: pytube (==15.0.0)
+Requires-Dist: scipy (==1.12.0)
+Requires-Dist: tensorflow (==2.16.1)
+Requires-Dist: tensorflow-probability (==0.24.0)
+Requires-Dist: tf-keras (==2.16.0)
+Requires-Dist: torchvision (==0.17.2)
+Requires-Dist: transformers (==4.39.2)
+Requires-Dist: wandb (==0.16.6)
+Requires-Dist: yt-dlp (==2023.11.14)
+Project-URL: Repository, https://github.com/KevKibe/African-Whisper
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pip==24.0
-Requires-Dist: transformers==4.39.2
-Requires-Dist: datasets==2.17.0
-Requires-Dist: librosa==0.10.1
-Requires-Dist: evaluate==0.4.1
-Requires-Dist: jiwer==3.0.3
-Requires-Dist: bitsandbytes==0.42.0
-Requires-Dist: accelerate==0.28.0
-Requires-Dist: peft==0.9.0
-Requires-Dist: numpy==1.26.4
-Requires-Dist: wandb==0.16.6
-Requires-Dist: holoviews==1.18.3
-Requires-Dist: panel==1.3.8
-Requires-Dist: gradio==4.24.0
-Requires-Dist: pytube==15.0.0
-Requires-Dist: tf-keras==2.16.0
-Requires-Dist: tensorflow==2.16.1
-Requires-Dist: keras==3.1.1
-Requires-Dist: scipy==1.12.0
-Requires-Dist: tensorflow-probability==0.24.0
-Requires-Dist: yt-dlp==2023.11.14
-Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: faster-whisper==1.0.0
-Requires-Dist: pyannote.audio==3.1.1
-Requires-Dist: nltk==3.8.1
-Requires-Dist: torchvision==0.17.2
-Requires-Dist: ctranslate2==4.1.0
-Requires-Dist: pandas==2.2.1
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
@@ -141,16 +146,18 @@
 
 ## Step 4: Preprocess the Dataset
 ```python
 # Load and preprocess the dataset
 processed_dataset = process.load_dataset(
     feature_extractor=feature_extractor,
     tokenizer=tokenizer,
-    processor=feature_processor
-)
+    processor=feature_processor,
+    num_samples = None # Number of samples to load from each dataset
+                       # Set None to load the entire dataset
+                       # Example: num_samples = 100 will load 100 samples from each dataset
 ```
 
 ## Step 5: Train the Model
 
 ```python
 from training.model_trainer import Trainer
 
@@ -192,15 +199,16 @@
 demo = WhisperDemo(model_name, huggingface_read_token)
 demo.generate_demo()
 ```
 
 ## Step 7: Test Model using Audio File
 
 ```python
-from deployment.speech_inference import SpeechInference
+# Using a PEFT fine-tuned model
+from deployment.peft_speech_inference import SpeechInference
 
 model_name = "your-finetuned-model-name-on-huggingface-hub"   # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " "
 task = "desired-task"                                         # either 'translate' or 'transcribe'
 audiofile_dir = "location-of-audio-file"                      # filetype should be .mp3 or .wav
 
 # Initialize the SpeechInference class and run inference
@@ -211,17 +219,52 @@
 # Access different parts of the output
 print(transcription.text)                                       # The entire text transcription.
 print(transcription.chunks)                                     # List of individual text chunks with timestamps.
 print(transcription.timestamps)                                 # List of timestamps for each chunk.
 print(transcription.chunk_texts)                                # List of texts for each chunk.
 
 ```
+```python
+# Using a fully fine-tuned model
+from deployment.speech_inference import SpeechTranscriptionPipeline, ModelOptimization
+
+model_name = "your-finetuned-model-name-on-huggingface-hub"   # e.g., "KevinKibe/whisper-small-af"
+huggingface_read_token = " "
+task = "desired-task"                                         # either 'translate' or 'transcribe'
+audiofile_dir = "location-of-audio-file"                      # filetype should be .mp3 or .wav
+
+# Optimize model for better results
+model_optimizer = ModelOptimization(model_name=model_name)
+model_optimizer.convert_model_to_optimized_format()
+model = model_optimizer.load_transcription_model()
+
+# Initiate the transcription model
+inference = SpeechTranscriptionPipeline(
+        audio_file_path=audiofile_dir,
+        task=task,
+        huggingface_read_token=huggingface_read_token
+    )
+
+# To get transcriptions
+transcription = inference.transcribe_audio(model=model)
+print(transcription)
+
+# To get transcriptions with speaker labels
+alignment_result = inference.align_transcription(transcription)
+diarization_result = inference.diarize_audio(alignment_result)
+print(diarization_result)
+
+#To generate subtitles(.srt format), will be saved in root directory
+inference.generate_subtitles(transcription, alignment_result, diarization_result)
+```
 
 # 🖥️ Using the CLI
 
+## Step 1: Clone and Install Dependencies
+
 - Clone the Repository: Clone or download the application code to your local machine.
 ```bash
 git clone https://github.com/KevKibe/African-Whisper.git
 ```
 
 - Create a virtual environment for the project and activate it.
 ```bash
@@ -234,22 +277,28 @@
 pip install -r requirements.txt
 ```
 - Navigate to:
 ```bash
 cd src
 ```
 
+## Step 2: Finetune the Model
+
 - To start the training , use the following command:
 ```bash
-python -m training.main --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --language_abbr LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft # leave this out to opt-out of using PEFT
+python -m training.main --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --language_abbr LANGUAGE_ABBREVIATION LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft
+
+Flags:
+# --use_peft: Optional flag to use PEFT finetuning. leave it out to perform full finetuning
 ```
 - Find a description of these commands [here](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/PARAMETERS.md).
 
-### Inference
+## Step 3: Get Inference
 
+### Install ffmpeg
 - To get inference from your fine-tuned model, follow these steps:
 
 - Ensure that ffmpeg is installed by running the following commands:
 
 ```bash
 # on Ubuntu or Debian
 sudo apt update && sudo apt install ffmpeg
@@ -262,43 +311,49 @@
 
 # on Windows using Chocolatey (https://chocolatey.org/)
 choco install ffmpeg
 
 # on Windows using Scoop (https://scoop.sh/)
 scoop install ffmpeg
 ```
+### To get inference on Gradio UI
 
-- To get the Gradio inference URL:
+- To get the Gradio UI URL:
 ```bash
 python -m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE 
 ```
 - **--model_name**: Name of the fine-tuned model to use in your huggingfacehub repo. This should match the model's identifier on the Hugging Face Model Hub.
 - **--huggingface_read_token**: Your Hugging Face authentication token for read access. It allows you to download datasets and models from Hugging Face.
 
-
+### To get inference on CLI
 ```bash
 cd src/deployment
 ```
 - Create a `.env` file using `nano .env` command and add these keys and save the file.
 ```python
 MODEL_NAME = "your-finetuned-model"
 HUGGINGFACE_READ_TOKEN = "huggingface-read-token"
 ```
 
 - To perform transcriptions and translations:
 
 ```bash
-# If your model is peft finetuned
-python -m deployment.peft_speech_inference_cli --audio_file audio-filename --task 
+# PEFT FINETUNED MODELS
+python -m deployment.peft_speech_inference_cli --audio_file FILENAME --task TASK 
+
+# FULLY FINETUNED MODELS
+python -m deployment.speech_inference_cli --audio_file FILENAME --task TASK --perform_diarization --perform_alignment
+
+Flags:
+# --perform_diarization: Optional flag to perform speaker diarization.
+# --perform_alignment: Optional flag to perform alignment.
 
-# If your model is fully finetuned
-python -m deployment.speech_inference_cli --audio_file audio-filename --task task --perform_diarization --perform_alignment
 ```
 
-## 🛳️ Deployment
+## 🛳️ Step 4: Deployment
 
 - To deploy your fine-tuned model as a REST API endpoint, follow these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md).
 
 
 ## Contributing 
 Contributions are welcome and encouraged.
 
@@ -310,7 +365,8 @@
 
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/KevKibe/African-Whisper/blob/main/LICENSE) file for details.
 
 ## Contact
 For any enquiries, please reach out to me through keviinkibe@gmail.com
+
```

#### html2text {}

```diff
@@ -1,26 +1,31 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.9.1 Summary: A package
-for fast fine-tuning and API endpoint deployment of Whisper model specifically
-developed to accelerate Automatic Speech Recognition(ASR) for African
-Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
-Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.0
-Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
-jiwer==3.0.3 Requires-Dist: bitsandbytes==0.42.0 Requires-Dist:
-accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: numpy==1.26.4
-Requires-Dist: wandb==0.16.6 Requires-Dist: holoviews==1.18.3 Requires-Dist:
-panel==1.3.8 Requires-Dist: gradio==4.24.0 Requires-Dist: pytube==15.0.0
-Requires-Dist: tf-keras==2.16.0 Requires-Dist: tensorflow==2.16.1 Requires-
-Dist: keras==3.1.1 Requires-Dist: scipy==1.12.0 Requires-Dist: tensorflow-
-probability==0.24.0 Requires-Dist: yt-dlp==2023.11.14 Requires-Dist: python-
-dotenv==1.0.1 Requires-Dist: faster-whisper==1.0.0 Requires-Dist:
-pyannote.audio==3.1.1 Requires-Dist: nltk==3.8.1 Requires-Dist:
-torchvision==0.17.2 Requires-Dist: ctranslate2==4.1.0 Requires-Dist:
-pandas==2.2.1
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.9.2 Summary: A package
+for fast fine-tuning and API endpoint deployment of the Whisper model,
+specifically developed to accelerate Automatic Speech Recognition (ASR) for
+African languages. Home-page: https://github.com/KevKibe/African-Whisper
+License: MIT Author: Kevin Kibe Author-email: keviinkibe@gmail.com Requires-
+Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Dist: accelerate (==0.28.0) Requires-Dist:
+bitsandbytes (==0.42.0) Requires-Dist: ctranslate2 (==4.1.0) Requires-Dist:
+datasets (==2.17.0) Requires-Dist: evaluate (==0.4.1) Requires-Dist: faster-
+whisper (==1.0.0) Requires-Dist: gradio (==4.24.0) Requires-Dist: holoviews
+(==1.18.3) Requires-Dist: jiwer (==3.0.3) Requires-Dist: keras (==3.1.1)
+Requires-Dist: librosa (==0.10.1) Requires-Dist: nltk (==3.8.1) Requires-Dist:
+numpy (==1.26.4) Requires-Dist: pandas (==2.0.3) Requires-Dist: panel (==1.3.8)
+Requires-Dist: peft (==0.9.0) Requires-Dist: pyannote-audio (==3.1.1) Requires-
+Dist: python-dotenv (==1.0.1) Requires-Dist: pytube (==15.0.0) Requires-Dist:
+scipy (==1.12.0) Requires-Dist: tensorflow (==2.16.1) Requires-Dist:
+tensorflow-probability (==0.24.0) Requires-Dist: tf-keras (==2.16.0) Requires-
+Dist: torchvision (==0.17.2) Requires-Dist: transformers (==4.39.2) Requires-
+Dist: wandb (==0.16.6) Requires-Dist: yt-dlp (==2023.11.14) Project-URL:
+Repository, https://github.com/KevKibe/African-Whisper Description-Content-
+Type: text/markdown
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 *Enhancing Automatic Speech Recognition (ASR): translation and transcription
 capabilities for African languages by providing seamless fine-tuning and
 deploying pipelines for Whisper Model*.
 ![Diagram](diagram-1.png) ## Features - ð§ Fine-tune the [Whisper](https://
@@ -61,81 +66,104 @@
 Step 3: Prepare the Model ```python from training.data_prep import DataPrep #
 Initialize the DataPrep class and prepare the model process = DataPrep
 ( huggingface_read_token, dataset_name, language_abbr, model_id,
 processing_task, use_peft ) tokenizer, feature_extractor, feature_processor,
 model = process.prepare_model() ``` ## Step 4: Preprocess the Dataset ```python
 # Load and preprocess the dataset processed_dataset = process.load_dataset
 ( feature_extractor=feature_extractor, tokenizer=tokenizer,
-processor=feature_processor ) ``` ## Step 5: Train the Model ```python from
-training.model_trainer import Trainer # Initialize the Trainer class and train
-the model trainer = Trainer( huggingface_write_token, model_id,
+processor=feature_processor, num_samples = None # Number of samples to load
+from each dataset # Set None to load the entire dataset # Example: num_samples
+= 100 will load 100 samples from each dataset ``` ## Step 5: Train the Model
+```python from training.model_trainer import Trainer # Initialize the Trainer
+class and train the model trainer = Trainer( huggingface_write_token, model_id,
 processed_dataset, model, feature_processor, feature_extractor, tokenizer,
 wandb_api_key, use_peft ) trainer.train( max_steps=100, learning_rate=1e-3,
 per_device_train_batch_size=96, per_device_eval_batch_size=64,
 optim="adamw_bnb_8bit" ) # Optional parameters for training: # max_steps (int):
 The maximum number of training steps (default is 100). # learning_rate (float):
 The learning rate for training (default is 1e-5). # per_device_train_batch_size
 (int): The batch size per GPU for training (default is 96). #
 per_device_eval_batch_size (int): The batch size per GPU for evaluation
 (default is 64). # optim (str): The optimizer used for training (default is
 "adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI ```python from
 training.gradio_inference import WhisperDemo # Generate a demo model_name =
 "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-
 small-af" demo = WhisperDemo(model_name, huggingface_read_token)
-demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python from
-deployment.speech_inference import SpeechInference model_name = "your-
+demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python #
+Using a PEFT fine-tuned model from deployment.peft_speech_inference import
+SpeechInference model_name = "your-finetuned-model-name-on-huggingface-hub" #
+e.g., "KevinKibe/whisper-small-af" huggingface_read_token = " " task =
+"desired-task" # either 'translate' or 'transcribe' audiofile_dir = "location-
+of-audio-file" # filetype should be .mp3 or .wav # Initialize the
+SpeechInference class and run inference inference = SpeechInference(model_name,
+huggingface_read_token) pipeline = inference.pipe_initialization()
+transcription = inference.output(pipeline, audiofile_dir, task) # Access
+different parts of the output print(transcription.text) # The entire text
+transcription. print(transcription.chunks) # List of individual text chunks
+with timestamps. print(transcription.timestamps) # List of timestamps for each
+chunk. print(transcription.chunk_texts) # List of texts for each chunk. ```
+```python # Using a fully fine-tuned model from deployment.speech_inference
+import SpeechTranscriptionPipeline, ModelOptimization model_name = "your-
 finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " " task = "desired-task" # either 'translate' or
 'transcribe' audiofile_dir = "location-of-audio-file" # filetype should be .mp3
-or .wav # Initialize the SpeechInference class and run inference inference =
-SpeechInference(model_name, huggingface_read_token) pipeline =
-inference.pipe_initialization() transcription = inference.output(pipeline,
-audiofile_dir, task) # Access different parts of the output print
-(transcription.text) # The entire text transcription. print
-(transcription.chunks) # List of individual text chunks with timestamps. print
-(transcription.timestamps) # List of timestamps for each chunk. print
-(transcription.chunk_texts) # List of texts for each chunk. ``` # ð¥ï¸ Using
-the CLI - Clone the Repository: Clone or download the application code to your
-local machine. ```bash git clone https://github.com/KevKibe/African-Whisper.git
-``` - Create a virtual environment for the project and activate it. ```bash
-python3 -m venv env source venv/bin/activate ``` - Install dependencies by
-running this command ```bash pip install -r requirements.txt ``` - Navigate to:
-```bash cd src ``` - To start the training , use the following command: ```bash
-python -m training.main --huggingface_read_token
-YOUR_HUGGING_FACE_READ_TOKEN_HERE --huggingface_write_token
-YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name AUDIO_DATASET_NAME --
-language_abbr LANGUAGE_ABBREVIATION --model_id MODEL_ID --processing_task
-PROCESSING_TASK --wandb_api_key YOUR_WANDB_API_KEY_HERE --use_peft # leave this
-out to opt-out of using PEFT ``` - Find a description of these commands [here]
-(https://github.com/KevKibe/African-Whisper/blob/master/DOCS/PARAMETERS.md).
-### Inference - To get inference from your fine-tuned model, follow these
-steps: - Ensure that ffmpeg is installed by running the following commands:
-```bash # on Ubuntu or Debian sudo apt update && sudo apt install ffmpeg # on
-Arch Linux sudo pacman -S ffmpeg # on MacOS using Homebrew (https://brew.sh/
-) brew install ffmpeg # on Windows using Chocolatey (https://chocolatey.org/
-) choco install ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop
-install ffmpeg ``` - To get the Gradio inference URL: ```bash python -
+or .wav # Optimize model for better results model_optimizer = ModelOptimization
+(model_name=model_name) model_optimizer.convert_model_to_optimized_format()
+model = model_optimizer.load_transcription_model() # Initiate the transcription
+model inference = SpeechTranscriptionPipeline( audio_file_path=audiofile_dir,
+task=task, huggingface_read_token=huggingface_read_token ) # To get
+transcriptions transcription = inference.transcribe_audio(model=model) print
+(transcription) # To get transcriptions with speaker labels alignment_result =
+inference.align_transcription(transcription) diarization_result =
+inference.diarize_audio(alignment_result) print(diarization_result) #To
+generate subtitles(.srt format), will be saved in root directory
+inference.generate_subtitles(transcription, alignment_result,
+diarization_result) ``` # ð¥ï¸ Using the CLI ## Step 1: Clone and Install
+Dependencies - Clone the Repository: Clone or download the application code to
+your local machine. ```bash git clone https://github.com/KevKibe/African-
+Whisper.git ``` - Create a virtual environment for the project and activate it.
+```bash python3 -m venv env source venv/bin/activate ``` - Install dependencies
+by running this command ```bash pip install -r requirements.txt ``` - Navigate
+to: ```bash cd src ``` ## Step 2: Finetune the Model - To start the training ,
+use the following command: ```bash python -m training.main --
+huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE --
+huggingface_write_token YOUR_HUGGING_FACE_WRITE_TOKEN_HERE --dataset_name
+AUDIO_DATASET_NAME --language_abbr LANGUAGE_ABBREVIATION LANGUAGE_ABBREVIATION
+--model_id MODEL_ID --processing_task PROCESSING_TASK --wandb_api_key
+YOUR_WANDB_API_KEY_HERE --use_peft Flags: # --use_peft: Optional flag to use
+PEFT finetuning. leave it out to perform full finetuning ``` - Find a
+description of these commands [here](https://github.com/KevKibe/African-
+Whisper/blob/master/DOCS/PARAMETERS.md). ## Step 3: Get Inference ### Install
+ffmpeg - To get inference from your fine-tuned model, follow these steps: -
+Ensure that ffmpeg is installed by running the following commands: ```bash # on
+Ubuntu or Debian sudo apt update && sudo apt install ffmpeg # on Arch Linux
+sudo pacman -S ffmpeg # on MacOS using Homebrew (https://brew.sh/) brew install
+ffmpeg # on Windows using Chocolatey (https://chocolatey.org/) choco install
+ffmpeg # on Windows using Scoop (https://scoop.sh/) scoop install ffmpeg ```
+### To get inference on Gradio UI - To get the Gradio UI URL: ```bash python -
 m training.gradio_demo --model_name YOUR_FINETUNED-MODEL --
 huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE ``` - **--
 model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
 This should match the model's identifier on the Hugging Face Model Hub. - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
-access. It allows you to download datasets and models from Hugging Face.
-```bash cd src/deployment ``` - Create a `.env` file using `nano .env` command
-and add these keys and save the file. ```python MODEL_NAME = "your-finetuned-
-model" HUGGINGFACE_READ_TOKEN = "huggingface-read-token" ``` - To perform
-transcriptions and translations: ```bash # If your model is peft finetuned
-python -m deployment.peft_speech_inference_cli --audio_file audio-filename --
-task # If your model is fully finetuned python -
-m deployment.speech_inference_cli --audio_file audio-filename --task task --
-perform_diarization --perform_alignment ``` ## ð³ï¸ Deployment - To deploy
-your fine-tuned model as a REST API endpoint, follow these [instructions]
-(https://github.com/KevKibe/African-Whisper/blob/master/DOCS/deployment.md). ##
-Contributing Contributions are welcome and encouraged. Before contributing,
-please take a moment to review our [Contribution Guidelines](https://
-github.com/KevKibe/African-Whisper/blob/master/DOCS/CONTRIBUTING.md) for
-important information on how to contribute to this project. If you're unsure
-about anything or need assistance, don't hesitate to reach out to us or open an
-issue to discuss your ideas. We look forward to your contributions! ## License
-This project is licensed under the MIT License - see the [LICENSE](https://
-github.com/KevKibe/African-Whisper/blob/main/LICENSE) file for details. ##
-Contact For any enquiries, please reach out to me through keviinkibe@gmail.com
+access. It allows you to download datasets and models from Hugging Face. ### To
+get inference on CLI ```bash cd src/deployment ``` - Create a `.env` file using
+`nano .env` command and add these keys and save the file. ```python MODEL_NAME
+= "your-finetuned-model" HUGGINGFACE_READ_TOKEN = "huggingface-read-token" ```
+- To perform transcriptions and translations: ```bash # PEFT FINETUNED MODELS
+python -m deployment.peft_speech_inference_cli --audio_file FILENAME --task
+TASK # FULLY FINETUNED MODELS python -m deployment.speech_inference_cli --
+audio_file FILENAME --task TASK --perform_diarization --perform_alignment
+Flags: # --perform_diarization: Optional flag to perform speaker diarization. #
+--perform_alignment: Optional flag to perform alignment. ``` ## ð³ï¸ Step 4:
+Deployment - To deploy your fine-tuned model as a REST API endpoint, follow
+these [instructions](https://github.com/KevKibe/African-Whisper/blob/master/
+DOCS/deployment.md). ## Contributing Contributions are welcome and encouraged.
+Before contributing, please take a moment to review our [Contribution
+Guidelines](https://github.com/KevKibe/African-Whisper/blob/master/DOCS/
+CONTRIBUTING.md) for important information on how to contribute to this
+project. If you're unsure about anything or need assistance, don't hesitate to
+reach out to us or open an issue to discuss your ideas. We look forward to your
+contributions! ## License This project is licensed under the MIT License - see
+the [LICENSE](https://github.com/KevKibe/African-Whisper/blob/main/LICENSE)
+file for details. ## Contact For any enquiries, please reach out to me through
+keviinkibe@gmail.com
```

### Comparing `africanwhisper-0.9.1/src/deployment/app.py` & `africanwhisper-0.9.2/src/deployment/app.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/deployment/main.py` & `africanwhisper-0.9.2/src/deployment/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/deployment/peft_speech_inference.py` & `africanwhisper-0.9.2/src/deployment/peft_speech_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/deployment/peft_speech_inference_cli.py` & `africanwhisper-0.9.2/src/deployment/peft_speech_inference_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     model_name = os.getenv("MODEL_NAME")
     huggingface_read_token = os.getenv("HUGGINGFACE_READ_TOKEN")
     
 
     speech_inference = SpeechInference(model_name=model_name, huggingface_read_token=huggingface_read_token)
     pipe = speech_inference.pipe_initialization()
     
-    if not os.path.exists(args.input_file):
-        print(f"Error: Input file '{args.input_file}' does not exist.")
+    if not os.path.exists(args.audio_file):
+        print(f"Error: Input file '{args.audio_file}' does not exist.")
         return
     
-    transcription = speech_inference.output(pipe=pipe, input=args.input_file, task=args.task)
+    transcription = speech_inference.output(pipe=pipe, input=args.audio_file, task=args.task)
     print(transcription.text)
 
 if __name__ == "__main__":
     main()
```

### Comparing `africanwhisper-0.9.1/src/deployment/speech_inference.py` & `africanwhisper-0.9.2/src/deployment/speech_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         """
         Initializes the ModelOptimization class.
 
         Args:
             model_name (str): Name of the model to be converted or loaded.
         """
         self.model_name = model_name
-        self.device =  0 if torch.cuda.is_available() else "cpu"
+        self.device =  "cuda" if torch.cuda.is_available() else "cpu"
 
     def convert_model_to_optimized_format(self) -> None:
         """
         Converts the specified model to CTranslate2 format if not already in that format.
         """
         output_dir = self.model_name
         if not os.path.exists(output_dir):
@@ -59,15 +59,15 @@
             "initial_prompt": None,
             "suppress_tokens": [-1],
             "suppress_numerals": True,
         }
         model_dir = None
         compute_type = "bfloat16" if torch.cuda.is_available() and torch.cuda.is_bf16_supported() else "float32"
         model = load_asr_model(
-            self.model_name,
+            whisper_arch = self.model_name,
             device=self.device,
             device_index=0,
             download_root=model_dir,
             compute_type=compute_type,
             language=None,
             asr_options=asr_options,
             vad_options={"vad_onset": 0.500, "vad_offset": 0.363},
```

### Comparing `africanwhisper-0.9.1/src/deployment/speech_inference_cli.py` & `africanwhisper-0.9.2/src/deployment/speech_inference_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import argparse
 from deployment.speech_inference import SpeechTranscriptionPipeline, ModelOptimization
 
+
 def main():
     parser = argparse.ArgumentParser(description="Speech inference using ASR and optional alignment and diarization.")
-    parser.add_argument("--audio_file", type=argparse.FileType("rb"), help="The audio file to transcribe")
+    parser.add_argument("--audio_file", type=str, help="Path to the input audio file for transcription.")
     parser.add_argument("--task", choices=["transcribe", "translate"], help="Task to perform, e.g., 'transcribe' or 'translate'")
     parser.add_argument("--batch_size", type=int, default=24, help="Batch size for transcription")
     parser.add_argument("--chunk_size", type=int, default=30, help="Chunk size for transcription")
     parser.add_argument("--perform_diarization", action="store_true", help="Perform diarization on the audio file")
     parser.add_argument("--perform_alignment", action="store_true", help="Perform alignment on the audio file")
     args = parser.parse_args()
 
@@ -19,15 +20,15 @@
     # Initialize model optimization
     model_optimizer = ModelOptimization(model_name=model_name)
     model_optimizer.convert_model_to_optimized_format()
     model = model_optimizer.load_transcription_model()
 
     # Initialize the speech transcription pipeline
     inference = SpeechTranscriptionPipeline(
-        audio_file_path=args.file.name,
+        audio_file_path=args.audio_file,
         task=args.task,
         batch_size=args.batch_size,
         chunk_size=args.chunk_size,
         huggingface_read_token=huggingface_read_token
     )
 
     # Transcribe the audio
```

### Comparing `africanwhisper-0.9.1/src/deployment/transcription_model.py` & `africanwhisper-0.9.2/src/deployment/transcription_model.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/training/audio_data_processor.py` & `africanwhisper-0.9.2/src/training/audio_data_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/training/collator.py` & `africanwhisper-0.9.2/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/training/data_prep.py` & `africanwhisper-0.9.2/src/training/data_prep.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,31 +77,38 @@
         return (
             self.tokenizer,
             self.feature_extractor,
             self.feature_processor,
             self.model,
         )
 
-    def load_dataset(self, feature_extractor: WhisperFeatureExtractor, tokenizer: WhisperTokenizer, processor: WhisperProcessor) -> DatasetDict:
+    def load_dataset(
+        self,  
+        feature_extractor: WhisperFeatureExtractor, 
+        tokenizer: WhisperTokenizer, 
+        processor: WhisperProcessor,
+        num_samples: int = None,) -> DatasetDict:
         """
         Retrieves and preprocesses the specified dataset for model training and evaluation.
 
         Parameters:
         feature_extractor (PreTrainedFeatureExtractor): The feature extractor instance to be used for
                                                         audio data preprocessing.
         tokenizer (PreTrainedTokenizer): The tokenizer instance for processing textual data associated
                                          with the audio samples.
+        processor (WhisperProcessor): The processor instance for processing the audio samples.
+        num_samples(int): Number of training samples to load from each dataset eg if num_samples = 100, 200 samples, 100 from each dataset will be loaded. 
 
         Returns:
             DatasetDict: A dictionary containing the preprocessed 'train' and 'test' splits of the dataset,
                         ready for use in model training and evaluation. Each split has been cleaned and
                         processed to include only the necessary features for model input.
         """
 
-        dataset = self.data_loader.load_dataset()
+        dataset = self.data_loader.load_dataset(num_samples = num_samples)
         print(f"Training dataset size: {self.data_loader.count_examples(dataset['train'])}")
         print(f"Test dataset size: {self.data_loader.count_examples(dataset['test'])}")
         processor = AudioDataProcessor(dataset, feature_extractor, tokenizer, processor)
         dataset['train']= dataset['train'].map(processor.resampled_dataset, remove_columns=list(next(iter(dataset['train'])).keys()))
         dataset['test']= dataset['test'].map(processor.resampled_dataset)
         return dataset
```

### Comparing `africanwhisper-0.9.1/src/training/evaluation.py` & `africanwhisper-0.9.2/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/training/gradio_demo.py` & `africanwhisper-0.9.2/src/training/gradio_demo.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/training/gradio_inference.py` & `africanwhisper-0.9.2/src/training/gradio_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/training/load_data.py` & `africanwhisper-0.9.2/src/training/load_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,42 +23,45 @@
             dataset_name (str): Name of the dataset.
             language_abbr (str): Language abbreviation for the dataset.
         """
         self.huggingface_token = huggingface_token
         self.dataset_name = dataset_name
         self.language_abbr = language_abbr
     
-    def load_dataset(self):
+    def load_dataset(self, num_samples: int = None):
         """Load datasets for each language abbreviation and concatenate train/test splits.
 
+        Parameters:
+            num_samples(int): Number of training samples to load from each dataset eg if num_samples = 100, 200 samples, 100 from each dataset will be loaded.   
+            
         Returns:
             dict: A dictionary containing concatenated train and test splits for each language.
         """
         data = {}
         for lang in self.language_abbr:
             dataset = load_dataset(self.dataset_name, lang, streaming=True, token=self.huggingface_token, trust_remote_code=True)
-            train_split = dataset['train']
+            train_split = dataset['train'].take(num_samples)
             test_split = dataset['test']
             if "train" in data:
                 data["train"] = concatenate_datasets([data["train"], train_split])
             else:
                 data["train"] = train_split
             if "test" in data:
                 data["test"] = concatenate_datasets([data["test"], test_split])
             else:
                 data["test"] = test_split
         return data
-        
+    
     def count_examples(self, dataset: IterableDataset) -> int:
         """
         Count the number of examples in the dataset.
 
         Args:
             dataset (IterableDataset): The dataset to count examples from.
 
         Returns:
             int: The number of examples in the dataset.
         """
         count = 0
         for _ in dataset:
             count += 1
-        return count
+        return count
```

### Comparing `africanwhisper-0.9.1/src/training/main.py` & `africanwhisper-0.9.2/src/training/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/training/model_trainer.py` & `africanwhisper-0.9.2/src/training/model_trainer.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/training/wandb_callback.py` & `africanwhisper-0.9.2/src/training/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.9.1/src/training/whisper_model_prep.py` & `africanwhisper-0.9.2/src/training/whisper_model_prep.py`

 * *Files identical despite different names*

