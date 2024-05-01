# Comparing `tmp/ncmlistdownloader-1.0.8.240501.tar.gz` & `tmp/ncmlistdownloader-1.1.0.240430a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.8.240501.tar", last modified: Wed May  1 11:08:23 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.1.0.240430a1.tar", last modified: Tue Apr 30 04:28:02 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.8.240501.tar` & `ncmlistdownloader-1.1.0.240430a1.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 11:08:23.741439 ncmlistdownloader-1.0.8.240501/
--rw-rw-rw-   0        0        0    35181 2024-02-12 02:33:29.000000 ncmlistdownloader-1.0.8.240501/LICENSE
--rw-rw-rw-   0        0        0       18 2024-02-15 05:12:55.000000 ncmlistdownloader-1.0.8.240501/MANIFEST.in
--rw-rw-rw-   0        0        0     1409 2024-05-01 11:08:23.735442 ncmlistdownloader-1.0.8.240501/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 11:08:23.558441 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1425 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:08:23.658443 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/cmd/
--rw-rw-rw-   0        0        0     1789 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/cmd/__init__.py
--rw-rw-rw-   0        0        0      651 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/cmd/common.py
--rw-rw-rw-   0        0        0     1685 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/cmd/download.py
--rw-rw-rw-   0        0        0     2689 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/cmd/find_from_id.py
--rw-rw-rw-   0        0        0     1664 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/cmd/json_io.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:08:23.684441 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2862 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2161 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2376 2024-05-01 11:07:45.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1791 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:08:23.707443 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6233 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/downloader/__init__.py
--rw-rw-rw-   0        0        0     1110 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/downloader/json_list_io.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:08:23.711443 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     4034 2024-05-01 11:07:29.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:08:23.714439 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2296 2024-04-30 12:51:28.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:08:23.725443 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     9323 2024-05-01 11:07:22.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 11:08:23.732441 ncmlistdownloader-1.0.8.240501/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1409 2024-05-01 11:08:23.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      834 2024-05-01 11:08:23.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 11:08:23.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-01 11:08:23.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-05-01 11:08:23.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-01 11:08:23.000000 ncmlistdownloader-1.0.8.240501/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 11:08:23.742440 ncmlistdownloader-1.0.8.240501/setup.cfg
--rw-rw-rw-   0        0        0     1923 2024-05-01 11:07:46.000000 ncmlistdownloader-1.0.8.240501/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:28:02.838891 ncmlistdownloader-1.1.0.240430a1/
+-rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.1.0.240430a1/LICENSE
+-rw-rw-rw-   0        0        0     1399 2024-04-30 04:28:02.835898 ncmlistdownloader-1.1.0.240430a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 04:28:02.770075 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1425 2024-04-29 10:18:45.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:28:02.804980 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0     1789 2024-04-29 10:16:10.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/cmd/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-04-29 10:21:56.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/cmd/common.py
+-rw-rw-rw-   0        0        0     1685 2024-04-29 10:22:02.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/cmd/download.py
+-rw-rw-rw-   0        0        0     2689 2024-04-29 10:22:08.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/cmd/find_from_id.py
+-rw-rw-rw-   0        0        0     1664 2024-04-29 10:23:33.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/cmd/json_io.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:28:02.816948 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2862 2024-04-29 10:21:37.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2161 2024-04-29 10:21:11.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2376 2024-04-29 14:57:26.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1791 2024-04-29 10:20:35.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:28:02.821936 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6233 2024-04-29 10:20:23.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/downloader/__init__.py
+-rw-rw-rw-   0        0        0     1110 2024-04-30 04:27:30.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/downloader/json_list_io.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:28:02.823931 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3965 2024-04-29 10:20:17.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:28:02.826923 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2296 2024-04-29 10:19:56.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:28:02.828929 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     9302 2024-04-29 14:55:43.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:28:02.834909 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1399 2024-04-30 04:28:02.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      822 2024-04-30 04:28:02.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 04:28:02.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-30 04:28:02.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-30 04:28:02.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-30 04:28:02.000000 ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 04:28:02.838891 ncmlistdownloader-1.1.0.240430a1/setup.cfg
+-rw-rw-rw-   0        0        0     1925 2024-04-30 04:27:26.000000 ncmlistdownloader-1.1.0.240430a1/setup.py
```

### Comparing `ncmlistdownloader-1.0.8.240501/LICENSE` & `ncmlistdownloader-1.1.0.240430a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/PKG-INFO` & `ncmlistdownloader-1.1.0.240430a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.8.240501
+Version: 1.1.0.240430a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/cmd/__init__.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/cmd/common.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/cmd/common.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/cmd/download.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/cmd/download.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/cmd/find_from_id.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/cmd/find_from_id.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/cmd/json_io.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/cmd/json_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/common/global_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 PLAYLIST_API = json_file["PLAYLIST_API"]
 SONG_INFO_API = json_file["SONG_INFO_API"]
 SONG_FILE_API = json_file["SONG_FILE_API"]
 SONG_FILE_API_2 = json_file["SONG_FILE_API_2"]
 SEARCH_API = "https://music.163.com/weapi/cloudsearch/get/web?csrf_token="
 LYRIC_API = json_file["LYRIC_API"]
 CMD_VERSION = "Ver.1.0.4.240427"
-CORE_VERSION_SETUP = "1.0.8.240501"
+CORE_VERSION_SETUP = "1.0.6.240429"
 CORE_VERSION = "Core.Ver." + CORE_VERSION_SETUP
 CMD_START_WORDS = [
     f"163ListDownloader CMD Ver - {CMD_VERSION}",
     "Made by CooooldWind_",
     "Here's the Gitee/GitHub Page, click a star if you like it~",
     "Gitee: https://gitee.com/CooooldWind/163ListDownloader_NexT/issues",
     "GitHub: https://github.com/CooooldWind/163ListDownloader_NexT/issues",
```

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/downloader/json_list_io.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/downloader/json_list_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/editer/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 ncmlistdownloader/Editer/__init__.py
-Core.Ver.1.0.8.240501
+Core.Ver.1.0.5.240429
 Author: CooooldWind_
 """
 
 from PIL import Image
 from mutagen.flac import FLAC, Picture
 from mutagen.id3 import ID3, APIC, USLT, Encoding
 from mutagen.easyid3 import EasyID3
-from mutagen.mp3 import MP3
 from ncmlistdownloader.common import get_type, artist_turn_str
 
 expection_word_front = 'Opening files with the suffix ".'
 lyric_expection_word_front = 'Opening cover files with the suffix ".'
 cover_expection_word_front = 'Opening cover files with the suffix ".'
 expection_word_end = '" is not supported.'
 
@@ -25,16 +24,15 @@
     1. `filename`: 文件名, 字符串, 仅mp3/flac格式
     2. `info`: 信息, 里面需要 `'album'` , `'artist'`, `'title'`
     """
     type = get_type(filename)
     if type == "mp3":
         file = EasyID3(filename)
     elif type == "flac":
-        try: file = FLAC(filename)
-        except: return -1
+        file = FLAC(filename)
     else:
         raise Exception(expection_word_front + type + expection_word_end)
     if not info:
         raise ValueError(
             '"info" must be a dict(). See the comment for detail infomatiom.'
         )
     file["title"] = info["title"]
@@ -52,22 +50,23 @@
     1. `filename`: 文件名, 字符串, 仅mp3/flac格式
     2. `cover_filename`: 封面的文件名, 字符串, 仅jpg格式
     """
     type = get_type(filename)
     if type == "mp3":
         file = ID3(filename)
     elif type == "flac":
-        try: file = FLAC(filename)
-        except: return -1
+        file = FLAC(filename)
     else:
         raise Exception(expection_word_front + type + expection_word_end)
     cover_type = get_type(cover_filename)
     if cover_type != "jpg" and cover_type != "jpeg":
         raise Exception(cover_expection_word_front + cover_type + expection_word_end)
     with open(cover_filename, "rb") as cover_file:
+        print(cover_filename)
+        print(filename)
         if type == "mp3":
             file["APIC"] = APIC(
                 encoding=3,
                 mime="image/jpeg",
                 type=3,
                 desc="Cover",
                 data=cover_file.read(),
@@ -91,16 +90,15 @@
     1. `filename`: 文件名, 字符串, 仅mp3/flac格式
     2. `lyric_filename`: 歌词的文件名, 字符串, 仅lrc格式
     """
     type = get_type(filename)
     if type == "mp3":
         file = ID3(filename)
     elif type == "flac":
-        try: file = FLAC(filename)
-        except: return -1
+        file = FLAC(filename)
     else:
         raise Exception(expection_word_front + type + expection_word_end)
     lyric_type = get_type(lyric_filename)
     if lyric_type != "lrc":
         raise Exception(lyric_expection_word_front + lyric_type + expection_word_end)
     with open(lyric_filename, "rb+") as lyric_file:
         lyric = lyric_file.read()
```

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader/song/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ncmlistdownloader/song/__init__.py
-Core.Ver.1.0.8.240501
+Core.Ver.1.0.6.240429
 Author: CooooldWind_
 """
 
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.thread_test import best_thread
 from ncmlistdownloader.downloader import *
@@ -86,18 +86,18 @@
         获取歌曲信息
         ----------
         无参数。
         """
         self.raw_info = NeteaseParams(
             url=SONG_INFO_API,
             encode_data=self.encode_data).get_resource()["songs"][0]
-        self.title = clean(self.raw_info["name"])
-        self.album = clean(self.raw_info["al"]["name"])
+        self.title = self.raw_info["name"]
+        self.album = self.raw_info["al"]["name"]
         for i in self.raw_info["ar"]:
-            self.artist.append(clean(i["name"]))
+            self.artist.append(i["name"])
         self.artist_str = artist_turn_str(self.artist)
         self.processed_info = {
             "album": self.album,
             "title": self.title,
             "artist": self.artist,
             "id": self.id,
         }
```

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.8.240501
+Version: 1.1.0.240430a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.8.240501/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.1.0.240430a1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-MANIFEST.in
 setup.py
 ncmlistdownloader/__init__.py
 ncmlistdownloader.egg-info/PKG-INFO
 ncmlistdownloader.egg-info/SOURCES.txt
 ncmlistdownloader.egg-info/dependency_links.txt
 ncmlistdownloader.egg-info/entry_points.txt
 ncmlistdownloader.egg-info/requires.txt
```

### Comparing `ncmlistdownloader-1.0.8.240501/setup.py` & `ncmlistdownloader-1.1.0.240430a1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 # from ncmlistdownloader.common.global_args import CORE_VERSION_SETUP
 setup(
     classifiers=[
         # 发展时期
-        # 'Development Status :: 3 - Alpha',
+        'Development Status :: 3 - Alpha',
         # 'Development Status :: 4 - Beta',
-        "Development Status :: 5 - Production/Stable",
+        # "Development Status :: 5 - Production/Stable",
         # 开发的目标用户
         "Intended Audience :: Customer Service",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         # 属于什么类型
         "Topic :: Communications :: File Sharing",
         "Topic :: Internet",
@@ -28,15 +28,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     name="ncmlistdownloader",
-    version="1.0.8.240501",
+    version="1.1.0.240430a1",
     description="获取网易云音乐歌单数据，下载音乐，主动添加元信息。",
     author="CooooldWind_",
     url="https://gitee.com/Cooooldwind/163ListDownloader_NexT",
     packages=find_packages(),
     install_requires=[
         "pycryptodome",
         "pillow",
```
