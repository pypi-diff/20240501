# Comparing `tmp/flickr_photos_api-2.1.2.tar.gz` & `tmp/flickr_photos_api-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flickr_photos_api-2.1.2.tar", last modified: Wed May  1 08:33:38 2024, max compression
+gzip compressed data, was "flickr_photos_api-2.2.0.tar", last modified: Wed May  1 09:51:54 2024, max compression
```

## Comparing `flickr_photos_api-2.1.2.tar` & `flickr_photos_api-2.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.962478 flickr_photos_api-2.1.2/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.1.2/LICENSE-APACHE
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.1.2/LICENSE-MIT
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-01 08:33:38.962300 flickr_photos_api-2.1.2/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.2/README.md
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.2/pyproject.toml
--rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-05-01 08:33:38.962516 flickr_photos_api-2.1.2/setup.cfg
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.957796 flickr_photos_api-2.1.2/src/
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.959660 flickr_photos_api-2.1.2/src/flickr_photos_api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1172 2024-05-01 08:33:33.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/__init__.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.961598 flickr_photos_api-2.1.2/src/flickr_photos_api/api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)      564 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5267 2024-04-30 12:27:45.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/base.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    12615 2024-05-01 08:33:33.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/collection_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1994 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/comment_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2234 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/from_url_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/license_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     8836 2024-05-01 08:33:33.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/single_photo_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     8414 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/user_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1836 2024-04-30 12:27:45.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/exceptions.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/py.typed
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3562 2024-05-01 08:33:33.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/types.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/utils.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.962114 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-01 08:33:38.000000 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)      827 2024-05-01 08:33:38.000000 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/SOURCES.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-05-01 08:33:38.000000 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/dependency_links.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-05-01 08:33:38.000000 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/requires.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-05-01 08:33:38.000000 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/top_level.txt
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.961829 flickr_photos_api-2.1.2/tests/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     6546 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.2/tests/test_errors.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.1.2/tests/test_utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 09:51:54.165045 flickr_photos_api-2.2.0/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.2.0/LICENSE-APACHE
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.2.0/LICENSE-MIT
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-01 09:51:54.164842 flickr_photos_api-2.2.0/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 12:06:13.000000 flickr_photos_api-2.2.0/README.md
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 14:50:54.000000 flickr_photos_api-2.2.0/pyproject.toml
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-05-01 09:51:54.165085 flickr_photos_api-2.2.0/setup.cfg
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 09:51:54.159798 flickr_photos_api-2.2.0/src/
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 09:51:54.161688 flickr_photos_api-2.2.0/src/flickr_photos_api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1222 2024-05-01 09:51:49.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/__init__.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 09:51:54.163996 flickr_photos_api-2.2.0/src/flickr_photos_api/api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      640 2024-05-01 09:51:49.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/api/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5267 2024-04-30 12:27:45.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/api/base.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    12615 2024-05-01 08:33:33.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/api/collection_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1994 2024-04-30 12:06:13.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/api/comment_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1862 2024-05-01 09:51:49.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/api/commons_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2234 2024-04-30 14:50:54.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/api/from_url_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 12:06:13.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/api/license_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     8836 2024-05-01 08:33:33.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/api/single_photo_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     8414 2024-04-30 14:50:54.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/api/user_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1836 2024-04-30 12:27:45.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/exceptions.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/py.typed
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3793 2024-05-01 09:51:49.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/types.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.2.0/src/flickr_photos_api/utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 09:51:54.164626 flickr_photos_api-2.2.0/src/flickr_photos_api.egg-info/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-01 09:51:54.000000 flickr_photos_api-2.2.0/src/flickr_photos_api.egg-info/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      872 2024-05-01 09:51:54.000000 flickr_photos_api-2.2.0/src/flickr_photos_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-05-01 09:51:54.000000 flickr_photos_api-2.2.0/src/flickr_photos_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-05-01 09:51:54.000000 flickr_photos_api-2.2.0/src/flickr_photos_api.egg-info/requires.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-05-01 09:51:54.000000 flickr_photos_api-2.2.0/src/flickr_photos_api.egg-info/top_level.txt
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 09:51:54.164353 flickr_photos_api-2.2.0/tests/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     6546 2024-04-30 14:50:54.000000 flickr_photos_api-2.2.0/tests/test_errors.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.2.0/tests/test_utils.py
```

### Comparing `flickr_photos_api-2.1.2/LICENSE-APACHE` & `flickr_photos_api-2.2.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/LICENSE-MIT` & `flickr_photos_api-2.2.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/PKG-INFO` & `flickr_photos_api-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.1.2
+Version: 2.2.0
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_photos_api-2.1.2/README.md` & `flickr_photos_api-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/pyproject.toml` & `flickr_photos_api-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/__init__.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     ResourceNotFound,
     LicenseNotFound,
     UnrecognisedFlickrApiException,
     UserDeleted,
 )
 from .types import (
     Comment,
+    CommonsInstitution,
     License,
     User,
     UserInfo,
     TakenGranularity,
     DateTaken,
     LocationInfo,
     Size,
@@ -27,15 +28,15 @@
     AlbumInfo,
     GalleryInfo,
     GroupInfo,
     SinglePhotoInfo,
 )
 
 
-__version__ = "2.1.2"
+__version__ = "2.2.0"
 
 
 __all__ = [
     "FlickrApi",
     "FlickrApiException",
     "ResourceNotFound",
     "InvalidApiKey",
@@ -43,14 +44,15 @@
     "LicenseNotFound",
     "License",
     "LocationInfo",
     "User",
     "UserInfo",
     "TakenGranularity",
     "Comment",
+    "CommonsInstitution",
     "DateTaken",
     "Size",
     "SafetyLevel",
     "SinglePhoto",
     "SinglePhotoInfo",
     "CollectionOfPhotos",
     "PhotosFromUrl",
```

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/api/__init__.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from .base import HttpxImplementation as HttpxImplementation
 from .collection_methods import CollectionMethods
 from .comment_methods import CommentMethods
+from .commons_methods import FlickrCommonsMethods
 from .from_url_methods import FromUrlMethods
 from .license_methods import LicenseMethods
 from .single_photo_methods import SinglePhotoMethods
 from .user_methods import UserMethods
 
 
 class FlickrApiMethods(
     FromUrlMethods,
     CommentMethods,
+    FlickrCommonsMethods,
     CollectionMethods,
     SinglePhotoMethods,
     LicenseMethods,
     UserMethods,
 ):
     pass
```

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/api/base.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/api/base.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/api/collection_methods.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/api/collection_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/api/comment_methods.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/api/comment_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/api/from_url_methods.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/api/from_url_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/api/license_methods.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/api/license_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/api/single_photo_methods.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/api/single_photo_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/api/user_methods.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/api/user_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/exceptions.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/types.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,7 +163,19 @@
 class PhotosInGroup(CollectionOfPhotos):
     group: GroupInfo
 
 
 PhotosFromUrl = (
     SinglePhoto | CollectionOfPhotos | PhotosInAlbum | PhotosInGallery | PhotosInGroup
 )
+
+
+class CommonsInstitution(typing.TypedDict):
+    """
+    Represents an institution in the Flickr Commons programme.
+    """
+
+    user_id: str
+    date_launch: datetime.datetime
+    name: str
+    site_url: str
+    license_url: str
```

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api/utils.py` & `flickr_photos_api-2.2.0/src/flickr_photos_api/utils.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/PKG-INFO` & `flickr_photos_api-2.2.0/src/flickr_photos_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.1.2
+Version: 2.2.0
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/SOURCES.txt` & `flickr_photos_api-2.2.0/src/flickr_photos_api.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 src/flickr_photos_api.egg-info/dependency_links.txt
 src/flickr_photos_api.egg-info/requires.txt
 src/flickr_photos_api.egg-info/top_level.txt
 src/flickr_photos_api/api/__init__.py
 src/flickr_photos_api/api/base.py
 src/flickr_photos_api/api/collection_methods.py
 src/flickr_photos_api/api/comment_methods.py
+src/flickr_photos_api/api/commons_methods.py
 src/flickr_photos_api/api/from_url_methods.py
 src/flickr_photos_api/api/license_methods.py
 src/flickr_photos_api/api/single_photo_methods.py
 src/flickr_photos_api/api/user_methods.py
 tests/test_errors.py
 tests/test_utils.py
```

### Comparing `flickr_photos_api-2.1.2/tests/test_errors.py` & `flickr_photos_api-2.2.0/tests/test_errors.py`

 * *Files identical despite different names*

