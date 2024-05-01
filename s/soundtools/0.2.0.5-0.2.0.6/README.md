# Comparing `tmp/soundtools-0.2.0.5.tar.gz` & `tmp/soundtools-0.2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.2.0.5.tar", last modified: Tue Apr 23 10:58:29 2024, max compression
+gzip compressed data, was "soundtools-0.2.0.6.tar", last modified: Wed May  1 19:29:21 2024, max compression
```

## Comparing `soundtools-0.2.0.5.tar` & `soundtools-0.2.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 10:58:29.932450 soundtools-0.2.0.5/
--rw-rw-rw-   0        0        0      701 2024-04-23 10:58:29.929930 soundtools-0.2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 10:58:29.933450 soundtools-0.2.0.5/setup.cfg
--rw-rw-rw-   0        0        0      789 2024-04-23 10:58:18.000000 soundtools-0.2.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:58:29.917046 soundtools-0.2.0.5/soundtools/
--rw-rw-rw-   0        0        0      399 2024-04-23 10:58:06.000000 soundtools-0.2.0.5/soundtools/__init__.py
--rw-rw-rw-   0        0        0    37291 2024-04-23 10:58:00.000000 soundtools-0.2.0.5/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:58:29.920046 soundtools-0.2.0.5/soundtools.egg-info/
--rw-rw-rw-   0        0        0      701 2024-04-23 10:58:29.000000 soundtools-0.2.0.5/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-23 10:58:29.000000 soundtools-0.2.0.5/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 10:58:29.000000 soundtools-0.2.0.5/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-23 10:58:29.000000 soundtools-0.2.0.5/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 19:29:21.502435 soundtools-0.2.0.6/
+-rw-rw-rw-   0        0        0      701 2024-05-01 19:29:21.501434 soundtools-0.2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 19:29:21.502435 soundtools-0.2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-05-01 19:28:55.000000 soundtools-0.2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 19:29:21.471098 soundtools-0.2.0.6/soundtools/
+-rw-rw-rw-   0        0        0      399 2024-05-01 19:28:44.000000 soundtools-0.2.0.6/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    37237 2024-05-01 19:28:36.000000 soundtools-0.2.0.6/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-05-01 19:29:21.491167 soundtools-0.2.0.6/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-05-01 19:29:21.000000 soundtools-0.2.0.6/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-05-01 19:29:21.000000 soundtools-0.2.0.6/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 19:29:21.000000 soundtools-0.2.0.6/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-01 19:29:21.000000 soundtools-0.2.0.6/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.2.0.5/PKG-INFO` & `soundtools-0.2.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.0.5
+Version: 0.2.0.6
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.5
+version: 0.2.0.6
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

### Comparing `soundtools-0.2.0.5/setup.py` & `soundtools-0.2.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 setup(
 name='soundtools',
-version='0.2.0.5',
+version='0.2.0.6',
 description="used to work with sounds waves",
 long_description="""made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.5
+version: 0.2.0.6
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves""",
 author='Mohammad Erfan Karami',
```

### Comparing `soundtools-0.2.0.5/soundtools/soundtools.py` & `soundtools-0.2.0.6/soundtools/soundtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """### made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-### version: 0.2.0.5
+### version: 0.2.0.6
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves"""
 
@@ -235,16 +235,16 @@
         buf += vol*0.9 * np.sin(pi_2_samples_num * freq*2 / self.default_sample_rate)
         buf += vol * np.sin(pi_2_samples_num * freq*4 / self.default_sample_rate)
         buf += vol*0.6 * np.sin(pi_2_samples_num * freq*6 / self.default_sample_rate)
         buf += vol*0.7 * np.sin(pi_2_samples_num * freq*16 / self.default_sample_rate)
         buf += vol*0.5 * np.sin(pi_2_samples_num * freq*20 / self.default_sample_rate)
         buf += vol*0.3 * np.sin(pi_2_samples_num * freq*24 / self.default_sample_rate)
 
-        wave = (buf/7*1.424).astype(self.dtype)
-        # wave = (buf/7*1.4247).astype(self.dtype) # for better percision (might cause quality issues on high volumes)
+        wave = (buf/7*2.424).astype(self.dtype)
+        # wave = (buf/7*2.4247).astype(self.dtype) # for better percision (might cause quality issues on high volumes)
         return wave
     
     @cache_wave("marimb")
     def marimba(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates a "not even close to marimba" sound based on the given frequency, duration and amplitude or volume\n
         warning!: very annoying sound"""
         
@@ -607,18 +607,17 @@
         
         return duration
     
     
     def fix_volume(self, volume:float=0) -> float:
         if volume == 0:
             volume = self.DEFAULT_VOLUME
-        volume = abs(volume)
 
-        if volume >= 1:
-            volume = 1
+        if volume > self.max_amp:
+            volume = self.max_amp
         
         return volume
     
     
     def get_file_data(self, file_path: str) -> tuple[SoundBuffer, int]:
         """gets the file data and returns a tuple[wave, sample_rate]
         you ca access other information as shown below
@@ -688,19 +687,17 @@
         or can be a string representing the duration in seconds like this: \"2s\"
         ### note!:
         if duration or volume are not passed as arguments when using the function, the default for both are 1, and you can change the default as well
         ### example:
         >>> generate_note_buffer("a4", sine_wave, \"1.5s\", 1)"""
         duration = self.fix_duration(duration)
         volume = self.fix_volume(volume)
-        try:
-            note = float(note)
-            f = note
-        except ValueError:
-            note = note.upper()
+        if str(note)[0].isdigit():
+            f = float(note)
+        else:
             f = self._NOTES[note]
         
         buf = wave_type(f, duration, volume)
         return buf
     
     
     # creates a chord buffer but doesn't turn it into bytes
@@ -740,15 +737,15 @@
         for buffer in buffers[1:]:
             if buffer.size < s:
                 s = buffer.size
         
         s_bufs: SoundBuffer = buffers[0][:s]
         
         for buffer in buffers[1:]:
-            s_bufs += buffer
+            s_bufs += buffer[:s]
             
         return s_bufs / len(buffers)
     
     # creates a note buffer and plays it
     def play(self, note:str|float|int, wave_type: Wave, duration:str|float=0, volume:float=0) -> None:
         """generates then plays a note with the given arguments"""
         buf: bytes = self.generate_note_buffer(note, wave_type, duration, volume).tobytes()
```

### Comparing `soundtools-0.2.0.5/soundtools.egg-info/PKG-INFO` & `soundtools-0.2.0.6/soundtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.0.5
+Version: 0.2.0.6
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.5
+version: 0.2.0.6
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

