# Comparing `tmp/cleese_stim-2.0.0.tar.gz` & `tmp/cleese_stim-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleese_stim-2.0.0.tar", last modified: Wed Feb  2 23:39:40 2022, max compression
+gzip compressed data, was "cleese_stim-2.1.0.tar", last modified: Wed May  1 06:04:05 2024, max compression
```

## Comparing `cleese_stim-2.0.0.tar` & `cleese_stim-2.1.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)        0 2022-02-02 23:39:40.126920 cleese_stim-2.0.0/
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)     1073 2022-01-13 20:20:26.000000 cleese_stim-2.0.0/LICENSE
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)     2382 2022-02-02 23:39:40.126920 cleese_stim-2.0.0/PKG-INFO
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)     1699 2022-02-02 23:26:01.000000 cleese_stim-2.0.0/README.md
-drwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)        0 2022-02-02 23:39:40.123586 cleese_stim-2.0.0/cleese_stim/
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)      123 2022-02-02 23:22:22.000000 cleese_stim-2.0.0/cleese_stim/__init__.py
--rwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)     2026 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/cleese_stim/cleese.py
-drwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)        0 2022-02-02 23:39:40.123586 cleese_stim-2.0.0/cleese_stim/engines/
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)       87 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/cleese_stim/engines/__init__.py
--rwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)      657 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/cleese_stim/engines/engine.py
--rwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)    19815 2022-02-02 12:34:16.000000 cleese_stim-2.0.0/cleese_stim/engines/mediapipe.py
-drwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)        0 2022-02-02 23:39:40.126920 cleese_stim-2.0.0/cleese_stim/engines/phase_vocoder/
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)       33 2022-02-01 14:55:05.000000 cleese_stim-2.0.0/cleese_stim/engines/phase_vocoder/__init__.py
--rwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)     4383 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/cleese_stim/engines/phase_vocoder/cleeseBPF.py
--rwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)     4634 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/cleese_stim/engines/phase_vocoder/cleeseEngine.py
--rwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)    12927 2022-02-01 15:10:35.000000 cleese_stim-2.0.0/cleese_stim/engines/phase_vocoder/cleeseProcess.py
-drwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)        0 2022-02-02 23:39:40.126920 cleese_stim-2.0.0/cleese_stim/third_party/
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)        0 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/cleese_stim/third_party/__init__.py
-drwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)        0 2022-02-02 23:39:40.126920 cleese_stim-2.0.0/cleese_stim/third_party/mls/
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)        0 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/cleese_stim/third_party/mls/__init__.py
--rwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)    10362 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/cleese_stim/third_party/mls/demo.py
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)    15363 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/cleese_stim/third_party/mls/img_utils.py
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)    15137 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/cleese_stim/third_party/mls/img_utils_pytorch.py
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)     5112 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/cleese_stim/third_party/mls/interp_torch.py
-drwxr-xr-x   0 nemirwen  (1000) nemirwen  (1000)        0 2022-02-02 23:39:40.123586 cleese_stim-2.0.0/cleese_stim.egg-info/
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)     2382 2022-02-02 23:39:40.000000 cleese_stim-2.0.0/cleese_stim.egg-info/PKG-INFO
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)      840 2022-02-02 23:39:40.000000 cleese_stim-2.0.0/cleese_stim.egg-info/SOURCES.txt
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)        1 2022-02-02 23:39:40.000000 cleese_stim-2.0.0/cleese_stim.egg-info/dependency_links.txt
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)        1 2022-01-26 16:37:10.000000 cleese_stim-2.0.0/cleese_stim.egg-info/not-zip-safe
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)       74 2022-02-02 23:39:40.000000 cleese_stim-2.0.0/cleese_stim.egg-info/requires.txt
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)       12 2022-02-02 23:39:40.000000 cleese_stim-2.0.0/cleese_stim.egg-info/top_level.txt
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)       98 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/pyproject.toml
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)      833 2022-02-02 23:39:40.126920 cleese_stim-2.0.0/setup.cfg
--rw-r--r--   0 nemirwen  (1000) nemirwen  (1000)       38 2022-01-26 22:41:27.000000 cleese_stim-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.339438 cleese_stim-2.1.0/cleese_stim/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2026 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/cleese.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/cleese_stim/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/audio_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/bpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/phase_vocoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/cleese_stim/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/audio_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/cleese_stim/third_party/mls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/mls/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10362 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/mls/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/mls/img_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15137 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/mls/img_utils_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/mls/interp_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/yin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/cleese_stim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-01 06:04:05.347438 cleese_stim-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/setup.py
```

### Comparing `cleese_stim-2.0.0/LICENSE` & `cleese_stim-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.0.0/PKG-INFO` & `cleese_stim-2.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: cleese_stim
-Version: 2.0.0
+Version: 2.1.0
 Summary: Audio and visual stimuli generation tool
 Home-page: https://github.com/neuro-team-femto/cleese
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/neuro-team-femto/cleese/issues
 Keywords: sound manipulation,phase vocoder
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Sociology
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mediapipe
+Requires-Dist: msvc-runtime; platform_system == "Windows"
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: tomli
 
 ![cleese](tutorial/pics/silly-walk.jpg)
 
 CLEESE ("Ministry of Silly Speech") is a sound and image manipulation tool
 designed to generate an infinite number of possible stimuli; be it
 natural-sounding expressive variations around an original speech recording, or
 variations on the expression of a human face.
@@ -39,13 +43,13 @@
 Burred, Emmanuel Ponsot and Jean-Julien Aucouturier (STMS, IRCAM/CNRS/Sorbonne
 Université, Paris), with collaboration from Pascal Belin (Institut des
 Neurosciences de la Timone, Aix-Marseille Université), with generous funding
 from the European Research Council (CREAM 335536, 2014-2019, PI: JJ
 Aucouturier), and support for face deformation was added by Lara Kermarec
 (2022).
 
-A tutorial notebook is available [here](tutorial.ipynb).
+Jupyter notebooks are available as tutorials form
+[sound manipulation](tutorial_audio.ipynb) and
+[image manipulation](tutorial_images.ipynb).
 
 The user manual in PDF format is available
 [here](https://github.com/creamlab/cleese/raw/master/doc/CLEESE_manual_v2.0.pdf).
-
-
```

### Comparing `cleese_stim-2.0.0/README.md` & `cleese_stim-2.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,11 +21,13 @@
 Burred, Emmanuel Ponsot and Jean-Julien Aucouturier (STMS, IRCAM/CNRS/Sorbonne
 Université, Paris), with collaboration from Pascal Belin (Institut des
 Neurosciences de la Timone, Aix-Marseille Université), with generous funding
 from the European Research Council (CREAM 335536, 2014-2019, PI: JJ
 Aucouturier), and support for face deformation was added by Lara Kermarec
 (2022).
 
-A tutorial notebook is available [here](tutorial.ipynb).
+Jupyter notebooks are available as tutorials form
+[sound manipulation](tutorial_audio.ipynb) and
+[image manipulation](tutorial_images.ipynb).
 
 The user manual in PDF format is available
 [here](https://github.com/creamlab/cleese/raw/master/doc/CLEESE_manual_v2.0.pdf).
```

### Comparing `cleese_stim-2.0.0/cleese_stim/cleese.py` & `cleese_stim-2.1.0/cleese_stim/cleese.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.0.0/cleese_stim/engines/engine.py` & `cleese_stim-2.1.0/cleese_stim/engines/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from abc import ABC, abstractmethod
 
 
 class Engine(ABC):
 
     @staticmethod
     @abstractmethod
-    def load_file(filename):
+    def load_file(file_name):
         raise NotImplementedError()
 
     @staticmethod
     @abstractmethod
     def process(data, config, **kwargs):
         raise NotImplementedError()
```

### Comparing `cleese_stim-2.0.0/cleese_stim/engines/phase_vocoder/cleeseBPF.py` & `cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/bpf.py`

 * *Files 10% similar despite different names*

```diff
@@ -119,18 +119,25 @@
 
 def createBPFfreqs(config):
 
     sr = config["main"]["sr"]
     band_count = config["eq"]["band"]["count"]
 
     if config["eq"]["scale"] == "linear":
-        eqFreqVec = np.linspace(0., sr/float(2), band_count+1)
+        min_freq = float(config["eq"]["min_freq"])
+        max_freq = float(config["eq"]["max_freq"])
+        eqFreqVec = np.linspace(min_freq, max_freq, band_count+1)
+
     elif config["eq"]["scale"] == "mel":
-        minMel = 0
-        maxMel = freq2mel(sr/float(2))
+        minMel = freq2mel(config["eq"]["min_freq"])
+        if np.isnan(config["eq"]["max_freq"]):
+            maxMel = freq2mel(sr/float(2))
+        else:
+            maxMel = freq2mel(config["eq"]["max_freq"])
+
         melPerBin = (maxMel-minMel)/(band_count)
         eqFreqVec = melPerBin*np.ones(band_count)
         eqFreqVec = np.insert(eqFreqVec, 0, minMel)
         Vmel2freq = np.vectorize(mel2freq)
         eqFreqVec = Vmel2freq(np.cumsum(eqFreqVec))
 
     return eqFreqVec
```

### Comparing `cleese_stim-2.0.0/cleese_stim/engines/phase_vocoder/cleeseEngine.py` & `cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/audio_engine.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.0.0/cleese_stim/engines/phase_vocoder/cleeseProcess.py` & `cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/phase_vocoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 import os
 import numpy as np
 import scipy.io.wavfile as wav
 import scipy.signal as sig
 import time
 import shutil
 
-from .cleeseBPF import (
+from .bpf import (
         createBPFtimeVec,
         createBPFfreqs,
         createBPF,)
-from .cleeseEngine import (
+from .audio_engine import (
         stft,
         istft,
         istft_resamp,
         phaseVocoder_varHop,)
 from ..engine import Engine
 from ...cleese import log, load_config
 
+from .utils import load_file, wav_read, wav_write, extract_pitch 
+
 
 class PhaseVocoder(Engine):
 
     @staticmethod
     def generate_stimuli(soundData, config, BPF=None, sample_rate=None,
                          sample_format=None,
                          timeVec=None):
@@ -121,15 +123,15 @@
             for i in range(0, numFiles):
 
                 log(currTrString+' variation '+str(i+1)+'/'+str(numFiles))
                 currFileNo = "%08u" % (i+1)
 
                 if config["main"]['chain'] and t > 0:
                     if file_output:
-                        waveIn, sr, sampleFormat = PhaseVocoder.wavRead(
+                        waveIn, sr, sampleFormat = PhaseVocoder.wav_read(
                                 currOutFile[i])
                     else:
                         waveIn = waveOut
                     config["main"]['inSamples'] = len(waveIn)
                     config["main"]['sr'] = sr
                     duration = len(waveIn) / float(sr)
                     BPFtime, numPoints, endOnTrans = createBPFtimeVec(
@@ -193,74 +195,52 @@
                         waveOut = waveIn * BPF[:, 1]
                     else:
                         gainVec = np.interp(np.linspace(
                                 0, duration, config["main"]['inSamples']),
                                 BPF[:, 0], BPF[:, 1])
                         waveOut = waveIn * gainVec
 
-                if file_output:
-                    # normalize
-                    if np.max(np.abs(waveOut)) >= 1.0:
-                        waveOut = waveOut/np.max(np.abs(waveOut))*0.999
-
-                    PhaseVocoder.wavWrite(waveOut, fileName=currOutFile[i],
-                                          sr=sr, sampleFormat=sampleFormat)
+                # if gain > 1.0, normalize to avoid clipping
+                if np.max(np.abs(waveOut)) >= 1.0:
+                    waveOut = waveOut/np.max(np.abs(waveOut))*0.999
+                
+                if file_output:            
+                    PhaseVocoder.wav_write(waveOut, file_name=currOutFile[i],
+                                          sr=sr, sample_format=sampleFormat)
 
         if not file_output:
             return waveOut, BPF
 
     @staticmethod
-    def load_file(fileName):
-
-        sampleRate, wave = wav.read(fileName)
-
-        sampleFormat = wave.dtype
+    def name():
+        return "phase_vocoder"
 
-        if sampleFormat in ('int16', 'int32'):
-            # convert to float
-            if sampleFormat == 'int16':
-                n_bits = 16
-            elif sampleFormat == 'int32':
-                n_bits = 32
-            wave = wave/(float(2**(n_bits - 1)))
-            wave = wave.astype('float32')
-
-        attributes = {
-            "sample_rate": sampleRate,
-            "sample_format": sampleFormat,
-        }
-        return wave, attributes
+    @staticmethod
+    def load_file(file_name): 
+        return load_file(file_name)
 
     @staticmethod
-    def name():
-        return "phase_vocoder"
+    def wav_read(file_name):
+        return wav_read(file_name)
 
     @staticmethod
-    def wavRead(filename):
-        wave, attr = PhaseVocoder.load_file(filename)
-        return wave, attr["sample_rate"], attr["sample_format"]
+    def wav_write(wave_out, file_name, sr, sample_format='int16'):
+        return wav_write(wave_out, file_name, sr, sample_format)
 
     @staticmethod
-    def wavWrite(waveOut, fileName, sr, sampleFormat='int16'):
+    def extract_pitch(x, sr, win=.02, bounds=[70,400], interpolate=True):
+        return extract_pitch(x, sr, win=.02, bounds=[70,400], interpolate=True)
 
-        if sampleFormat == 'int16':
-            waveOutFormat = waveOut * 2**15
-        elif sampleFormat == 'int32':
-            waveOutFormat = waveOut * 2**31
-        else:
-            waveOutFormat = waveOut
-        waveOutFormat = waveOutFormat.astype(sampleFormat)
-        wav.write(fileName, sr, waveOutFormat)
 
     @staticmethod
-    def create_BPF(trans, config_file, time_points, num_points, eq_freqs=None):
+    def create_BPF(trans, config_file, time_points, num_points, end_on_transition, eq_freqs=None):
         config = load_config(config_file)
         if config is None:
             return
-        return createBPF(trans, config, time_points, num_points, eq_freqs)
+        return createBPF(trans, config, time_points, num_points, end_on_transition, eq_freqs)
 
 
 def processWithSTFT(waveIn, config, BPF):
 
     sr = config["main"]['sr']
     inSamples = config["main"]['inSamples']
 
@@ -288,27 +268,28 @@
 
     # interpolate in frequency
     interpBPF = np.zeros((n_fft//2+1, numSeg))
     for i in range(0, numSeg):
         currBinVec = freqMat[i, :]/sr*2 * (n_fft//2+1)
         # piecewise-linear spectral envelope
         interpBPF[:, i] = np.interp(np.arange(0, n_fft//2+1),
-                                    currBinVec, amplMat[i, :])
+                                    currBinVec, amplMat[i, :],
+                                    left=0, right=0)
 
     # interpolate in time
     filterMat = np.zeros(stftMat.shape)
     if numSeg == 1:
         filterMat = np.tile(interpBPF, (1, stftMat.shape[1]))
     else:
         frameVec = timeVec*sr/synHop
         for i in range(0, n_fft//2+1):
             filterMat[i, :] = np.interp(np.arange(0, numFrames),
                                         frameVec, interpBPF[i, :])
 
-    stftMat *= filterMat
+    stftMat *= np.power(10,filterMat/20)
 
     waveOut = istft(stftMat, win, n_fft, synHop)
 
     return waveOut
 
 
 def processWithPV(waveIn, config, BPF, doPitchShift=False):
```

### Comparing `cleese_stim-2.0.0/cleese_stim/third_party/mls/demo.py` & `cleese_stim-2.1.0/cleese_stim/third_party/mls/demo.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.0.0/cleese_stim/third_party/mls/img_utils.py` & `cleese_stim-2.1.0/cleese_stim/third_party/mls/img_utils.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.0.0/cleese_stim/third_party/mls/img_utils_pytorch.py` & `cleese_stim-2.1.0/cleese_stim/third_party/mls/img_utils_pytorch.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.0.0/cleese_stim/third_party/mls/interp_torch.py` & `cleese_stim-2.1.0/cleese_stim/third_party/mls/interp_torch.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.0.0/cleese_stim.egg-info/PKG-INFO` & `cleese_stim-2.1.0/cleese_stim.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
-Name: cleese-stim
-Version: 2.0.0
+Name: cleese_stim
+Version: 2.1.0
 Summary: Audio and visual stimuli generation tool
 Home-page: https://github.com/neuro-team-femto/cleese
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/neuro-team-femto/cleese/issues
 Keywords: sound manipulation,phase vocoder
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Sociology
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mediapipe
+Requires-Dist: msvc-runtime; platform_system == "Windows"
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: tomli
 
 ![cleese](tutorial/pics/silly-walk.jpg)
 
 CLEESE ("Ministry of Silly Speech") is a sound and image manipulation tool
 designed to generate an infinite number of possible stimuli; be it
 natural-sounding expressive variations around an original speech recording, or
 variations on the expression of a human face.
@@ -39,13 +43,13 @@
 Burred, Emmanuel Ponsot and Jean-Julien Aucouturier (STMS, IRCAM/CNRS/Sorbonne
 Université, Paris), with collaboration from Pascal Belin (Institut des
 Neurosciences de la Timone, Aix-Marseille Université), with generous funding
 from the European Research Council (CREAM 335536, 2014-2019, PI: JJ
 Aucouturier), and support for face deformation was added by Lara Kermarec
 (2022).
 
-A tutorial notebook is available [here](tutorial.ipynb).
+Jupyter notebooks are available as tutorials form
+[sound manipulation](tutorial_audio.ipynb) and
+[image manipulation](tutorial_images.ipynb).
 
 The user manual in PDF format is available
 [here](https://github.com/creamlab/cleese/raw/master/doc/CLEESE_manual_v2.0.pdf).
-
-
```

### Comparing `cleese_stim-2.0.0/setup.cfg` & `cleese_stim-2.1.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cleese_stim
-version = attr: cleese_stim.__version__
+version = 2.1.0
 description = Audio and visual stimuli generation tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = sound manipulation, phase vocoder
 license = MIT License
 url = https://github.com/neuro-team-femto/cleese
 project_urls =
```

