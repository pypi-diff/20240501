# Comparing `tmp/flickr_photos_api-2.1.1.tar.gz` & `tmp/flickr_photos_api-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flickr_photos_api-2.1.1.tar", last modified: Tue Apr 30 15:01:29 2024, max compression
+gzip compressed data, was "flickr_photos_api-2.1.2.tar", last modified: Wed May  1 08:33:38 2024, max compression
```

## Comparing `flickr_photos_api-2.1.1.tar` & `flickr_photos_api-2.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 15:01:29.579090 flickr_photos_api-2.1.1/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.1.1/LICENSE-APACHE
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.1.1/LICENSE-MIT
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 15:01:29.578897 flickr_photos_api-2.1.1/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.1/README.md
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.1/pyproject.toml
--rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-04-30 15:01:29.579132 flickr_photos_api-2.1.1/setup.cfg
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 15:01:29.574394 flickr_photos_api-2.1.1/src/
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 15:01:29.576160 flickr_photos_api-2.1.1/src/flickr_photos_api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1234 2024-04-30 15:00:50.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/__init__.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 15:01:29.577971 flickr_photos_api-2.1.1/src/flickr_photos_api/api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)      564 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/api/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5267 2024-04-30 12:27:45.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/api/base.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    12674 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/api/collection_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1994 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/api/comment_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2234 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/api/from_url_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/api/license_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     9409 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/api/single_photo_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     8414 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/api/user_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1836 2024-04-30 12:27:45.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/exceptions.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/py.typed
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3956 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/types.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.1.1/src/flickr_photos_api/utils.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 15:01:29.578695 flickr_photos_api-2.1.1/src/flickr_photos_api.egg-info/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-04-30 15:01:29.000000 flickr_photos_api-2.1.1/src/flickr_photos_api.egg-info/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)      827 2024-04-30 15:01:29.000000 flickr_photos_api-2.1.1/src/flickr_photos_api.egg-info/SOURCES.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-04-30 15:01:29.000000 flickr_photos_api-2.1.1/src/flickr_photos_api.egg-info/dependency_links.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-04-30 15:01:29.000000 flickr_photos_api-2.1.1/src/flickr_photos_api.egg-info/requires.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-04-30 15:01:29.000000 flickr_photos_api-2.1.1/src/flickr_photos_api.egg-info/top_level.txt
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-04-30 15:01:29.578234 flickr_photos_api-2.1.1/tests/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     6546 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.1/tests/test_errors.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.1.1/tests/test_utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.962478 flickr_photos_api-2.1.2/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.1.2/LICENSE-APACHE
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.1.2/LICENSE-MIT
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-01 08:33:38.962300 flickr_photos_api-2.1.2/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.2/README.md
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.2/pyproject.toml
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-05-01 08:33:38.962516 flickr_photos_api-2.1.2/setup.cfg
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.957796 flickr_photos_api-2.1.2/src/
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.959660 flickr_photos_api-2.1.2/src/flickr_photos_api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1172 2024-05-01 08:33:33.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/__init__.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.961598 flickr_photos_api-2.1.2/src/flickr_photos_api/api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      564 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5267 2024-04-30 12:27:45.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/base.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    12615 2024-05-01 08:33:33.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/collection_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1994 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/comment_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2234 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/from_url_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 12:06:13.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/license_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     8836 2024-05-01 08:33:33.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/single_photo_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     8414 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/api/user_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1836 2024-04-30 12:27:45.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/exceptions.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/py.typed
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3562 2024-05-01 08:33:33.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/types.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.1.2/src/flickr_photos_api/utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.962114 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-01 08:33:38.000000 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      827 2024-05-01 08:33:38.000000 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-05-01 08:33:38.000000 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-05-01 08:33:38.000000 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/requires.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-05-01 08:33:38.000000 flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/top_level.txt
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-01 08:33:38.961829 flickr_photos_api-2.1.2/tests/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     6546 2024-04-30 14:50:54.000000 flickr_photos_api-2.1.2/tests/test_errors.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.1.2/tests/test_utils.py
```

### Comparing `flickr_photos_api-2.1.1/LICENSE-APACHE` & `flickr_photos_api-2.1.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/LICENSE-MIT` & `flickr_photos_api-2.1.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/PKG-INFO` & `flickr_photos_api-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.1.1
+Version: 2.1.2
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_photos_api-2.1.1/README.md` & `flickr_photos_api-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/pyproject.toml` & `flickr_photos_api-2.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/__init__.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,19 +24,18 @@
     PhotosInAlbum,
     PhotosInGallery,
     PhotosInGroup,
     AlbumInfo,
     GalleryInfo,
     GroupInfo,
     SinglePhotoInfo,
-    SinglePhotoInfoWithSizes,
 )
 
 
-__version__ = "2.1.1"
+__version__ = "2.1.2"
 
 
 __all__ = [
     "FlickrApi",
     "FlickrApiException",
     "ResourceNotFound",
     "InvalidApiKey",
@@ -49,15 +48,14 @@
     "TakenGranularity",
     "Comment",
     "DateTaken",
     "Size",
     "SafetyLevel",
     "SinglePhoto",
     "SinglePhotoInfo",
-    "SinglePhotoInfoWithSizes",
     "CollectionOfPhotos",
     "PhotosFromUrl",
     "PhotosInAlbum",
     "PhotosInGallery",
     "PhotosInGroup",
     "AlbumInfo",
     "GalleryInfo",
```

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/api/__init__.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/api/base.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/api/base.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/api/collection_methods.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/api/collection_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .user_methods import UserMethods
 from ..types import (
     CollectionOfPhotos,
     GroupInfo,
     PhotosInAlbum,
     PhotosInGallery,
     PhotosInGroup,
-    SinglePhotoInfoWithSizes,
+    SinglePhoto,
     User,
     create_user,
 )
 from ..utils import (
     parse_date_posted,
     parse_date_taken,
     parse_location,
@@ -27,15 +27,15 @@
     parse_sizes,
 )
 
 
 class CollectionMethods(LicenseMethods, UserMethods):
     def _from_collection_photo(
         self, photo_elem: ET.Element, owner: User | None
-    ) -> SinglePhotoInfoWithSizes:
+    ) -> SinglePhoto:
         """
         Given a <photo> element from a collection response, extract all the photo info.
         """
         photo_id = photo_elem.attrib["id"]
 
         secret = photo_elem.attrib["secret"]
         server = photo_elem.attrib["server"]
@@ -80,15 +80,15 @@
         else:
             location = None
 
         count_comments = int(photo_elem.attrib["count_comments"])
         count_views = int(photo_elem.attrib["count_views"])
 
         assert owner["photos_url"].endswith("/")
-        photo_page_url = owner["photos_url"] + photo_id + "/"
+        url = owner["photos_url"] + photo_id + "/"
 
         sizes = parse_sizes(photo_elem)
 
         return {
             "id": photo_id,
             "secret": secret,
             "server": server,
@@ -101,15 +101,15 @@
             "description": description,
             "tags": tags,
             "date_posted": date_posted,
             "date_taken": date_taken,
             "location": location,
             "count_comments": count_comments,
             "count_views": count_views,
-            "photo_page_url": photo_page_url,
+            "url": url,
             "sizes": sizes,
         }
 
     extras = [
         "license",
         "date_upload",
         "date_taken",
```

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/api/comment_methods.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/api/comment_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/api/from_url_methods.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/api/from_url_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/api/license_methods.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/api/license_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/api/single_photo_methods.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/api/single_photo_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     parse_date_taken,
     parse_location,
     parse_safety_level,
 )
 
 
 class SinglePhotoMethods(LicenseMethods):
-    def get_single_photo_info(self, *, photo_id: str) -> SinglePhotoInfo:
+    def _get_single_photo_info(self, *, photo_id: str) -> SinglePhotoInfo:
         """
         Look up the information for a single photo.
 
         This uses the flickr.photos.getInfo API.
         """
         info_resp = self.call(
             method="flickr.photos.getInfo", params={"photo_id": photo_id}
@@ -77,17 +77,15 @@
 
         date_taken = parse_date_taken(
             value=dates["taken"],
             granularity=dates["takengranularity"],
             unknown=dates["takenunknown"] == "1",
         )
 
-        photo_page_url = find_required_text(
-            photo_elem, path='.//urls/url[@type="photopage"]'
-        )
+        url = find_required_text(photo_elem, path='.//urls/url[@type="photopage"]')
 
         count_comments = int(find_required_text(photo_elem, path="comments"))
         count_views = int(photo_elem.attrib["views"])
 
         # The originalformat parameter will only be returned if the user
         # allows downloads of the photo.
         #
@@ -140,18 +138,18 @@
             "description": description,
             "tags": tags,
             "date_posted": date_posted,
             "date_taken": date_taken,
             "location": location,
             "count_comments": count_comments,
             "count_views": count_views,
-            "photo_page_url": photo_page_url,
+            "url": url,
         }
 
-    def get_single_photo_sizes(self, *, photo_id: str) -> list[Size]:
+    def _get_single_photo_sizes(self, *, photo_id: str) -> list[Size]:
         """
         Look up the sizes for a single photo.
 
         This uses the flickr.photos.getSizes API.
         """
         sizes_resp = self.call(
             method="flickr.photos.getSizes", params={"photo_id": photo_id}
@@ -223,32 +221,18 @@
 
         return sizes
 
     def get_single_photo(self, *, photo_id: str) -> SinglePhoto:
         """
         Look up the information for a single photo.
         """
-        info = self.get_single_photo_info(photo_id=photo_id)
-        sizes = self.get_single_photo_sizes(photo_id=photo_id)
+        info = self._get_single_photo_info(photo_id=photo_id)
+        sizes = self._get_single_photo_sizes(photo_id=photo_id)
 
-        return {
-            "id": photo_id,
-            "title": info["title"],
-            "description": info["description"],
-            "owner": info["owner"],
-            "date_posted": info["date_posted"],
-            "date_taken": info["date_taken"],
-            "safety_level": info["safety_level"],
-            "license": info["license"],
-            "url": info["photo_page_url"],
-            "sizes": sizes,
-            "original_format": info["original_format"],
-            "tags": info["tags"],
-            "location": info["location"],
-        }
+        return {**info, "sizes": sizes}
 
     def is_photo_deleted(self, *, photo_id: str) -> bool:
         """
         Check if a photo has been deleted from Flickr.
         """
         try:
             self.call(method="flickr.photos.getInfo", params={"photo_id": photo_id})
```

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/api/user_methods.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/api/user_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/exceptions.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/types.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -116,39 +116,23 @@
     date_posted: datetime.datetime
     date_taken: DateTaken | None
     location: LocationInfo | None
 
     count_comments: int
     count_views: int
 
-    photo_page_url: str
-
-
-class SinglePhoto(typing.TypedDict):
-    id: str
-    title: str | None
-    description: str | None
-    owner: User
-    date_posted: datetime.datetime
-    date_taken: DateTaken | None
-    safety_level: SafetyLevel
-    license: License
     url: str
-    sizes: list[Size]
-    original_format: str | None
-    tags: list[str]
-    location: LocationInfo | None
 
 
-class SinglePhotoInfoWithSizes(SinglePhotoInfo):
+class SinglePhoto(SinglePhotoInfo):
     sizes: list[Size]
 
 
 class CollectionOfPhotos(typing.TypedDict):
-    photos: list[SinglePhotoInfoWithSizes]
+    photos: list[SinglePhoto]
 
     # Note: there are no parameters named like this in the Flickr API;
     # these names were chosen to match parameters that do exist like
     # `count_views` or `count_comments`.
     count_pages: int
     count_photos: int
```

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api/utils.py` & `flickr_photos_api-2.1.2/src/flickr_photos_api/utils.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api.egg-info/PKG-INFO` & `flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.1.1
+Version: 2.1.2
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_photos_api-2.1.1/src/flickr_photos_api.egg-info/SOURCES.txt` & `flickr_photos_api-2.1.2/src/flickr_photos_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.1.1/tests/test_errors.py` & `flickr_photos_api-2.1.2/tests/test_errors.py`

 * *Files identical despite different names*

