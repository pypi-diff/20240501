# Comparing `tmp/zenodo_backpack-0.2.0.tar.gz` & `tmp/zenodo_backpack-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zenodo_backpack-0.2.0.tar", last modified: Fri Oct  7 06:17:06 2022, max compression
+gzip compressed data, was "zenodo_backpack-0.3.0.tar", last modified: Wed May  1 00:22:50 2024, max compression
```

## Comparing `zenodo_backpack-0.2.0.tar` & `zenodo_backpack-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 n10851381 (327562) default   (4743)        0 2022-10-07 06:17:06.092125 zenodo_backpack-0.2.0/
--rw-r--r--   0 n10851381 (327562) default   (4743)     4666 2022-10-07 06:17:06.089487 zenodo_backpack-0.2.0/PKG-INFO
--rw-r--r--   0 n10851381 (327562) default   (4743)     4022 2022-10-07 06:06:55.000000 zenodo_backpack-0.2.0/README.md
-drwxr-xr-x   0 n10851381 (327562) default   (4743)        0 2022-10-07 06:17:05.971123 zenodo_backpack-0.2.0/bin/
--rwxr-xr-x   0 n10851381 (327562) default   (4743)     5686 2022-10-07 06:06:55.000000 zenodo_backpack-0.2.0/bin/zenodo_backpack
--rw-r--r--   0 n10851381 (327562) default   (4743)       38 2022-10-07 06:17:06.095487 zenodo_backpack-0.2.0/setup.cfg
--rw-r--r--   0 n10851381 (327562) default   (4743)     1458 2022-10-07 06:06:55.000000 zenodo_backpack-0.2.0/setup.py
-drwxr-xr-x   0 n10851381 (327562) default   (4743)        0 2022-10-07 06:17:06.006124 zenodo_backpack-0.2.0/zenodo_backpack/
--rw-r--r--   0 n10851381 (327562) default   (4743)    19971 2022-10-07 06:06:55.000000 zenodo_backpack-0.2.0/zenodo_backpack/__init__.py
--rw-r--r--   0 n10851381 (327562) default   (4743)       22 2022-10-07 06:06:55.000000 zenodo_backpack-0.2.0/zenodo_backpack/version.py
-drwxr-xr-x   0 n10851381 (327562) default   (4743)        0 2022-10-07 06:17:06.069124 zenodo_backpack-0.2.0/zenodo_backpack.egg-info/
--rw-r--r--   0 n10851381 (327562) default   (4743)     4666 2022-10-07 06:17:05.000000 zenodo_backpack-0.2.0/zenodo_backpack.egg-info/PKG-INFO
--rw-r--r--   0 n10851381 (327562) default   (4743)      287 2022-10-07 06:17:05.000000 zenodo_backpack-0.2.0/zenodo_backpack.egg-info/SOURCES.txt
--rw-r--r--   0 n10851381 (327562) default   (4743)        1 2022-10-07 06:17:05.000000 zenodo_backpack-0.2.0/zenodo_backpack.egg-info/dependency_links.txt
--rw-r--r--   0 n10851381 (327562) default   (4743)       14 2022-10-07 06:17:05.000000 zenodo_backpack-0.2.0/zenodo_backpack.egg-info/requires.txt
--rw-r--r--   0 n10851381 (327562) default   (4743)       16 2022-10-07 06:17:05.000000 zenodo_backpack-0.2.0/zenodo_backpack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:50.772973 zenodo_backpack-0.3.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5686 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/bin/zenodo_backpack
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/test/test_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/zenodo_backpack/
+-rw-r--r--   0 runner    (1001) docker     (127)    21588 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/zenodo_backpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 00:22:34.000000 zenodo_backpack-0.3.0/zenodo_backpack/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:50.776973 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-01 00:22:50.000000 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-01 00:22:50.000000 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:50.000000 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 00:22:50.000000 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 00:22:50.000000 zenodo_backpack-0.3.0/zenodo_backpack.egg-info/top_level.txt
```

### Comparing `zenodo_backpack-0.2.0/PKG-INFO` & `zenodo_backpack-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: zenodo_backpack
-Version: 0.2.0
+Version: 0.3.0
 Summary: Manage data bundled with bioinformatic software through Zenodo DOI integration
 Home-page: https://github.com/centre-for-microbiome-research/zenodo_backpack
 Author: ['Alex Chklovski', 'Ben Woodcroft']
 Author-email: chklovski@gmail.com
 License: GPL3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: tqdm
+Requires-Dist: requests
 
 # zenodo_backpack
 
 ZenodoBackpack provides a robust, standardised and repeatable approach to
 distributing and using backend databases that bioinformatic tools rely on. These
 databases are usually tool-specific and are often large enough in size that they
 cannot be uploaded as data to software repositories (e.g. PyPI imposes a limit
@@ -24,15 +27,15 @@
 ZenodoBackpack uploads/downloads data to/from [Zenodo](https://zenodo.org),
 which means that each dataset is associated with a DOI. Additionally, it
 encapsulates the uploaded data in a Zenodo Backpack format, which is really just
 a `CONTENTS.json` file and compresses the data in `.tar.gz` format before
 upload. The `CONTENTS.json` file includes md5sum values for each included file
 for robust verification.
 
-It contains two main methods, which can bee accessed through the
+It contains two main methods, which can be accessed through the
 `zenodo_backpack` script or accessed as a software library:
 
 **create**: turns a target directory into a zenodo_backpack-formatted .tar.gz archive with relevant checksum and version information, ready to be uploaded to Zenodo. It is necessary to provide a data version when doing so - furthermore, when uploading this backpack to zenodo.org, the version specified on the website **must** match that provided when the ZenodoBackpack was created. This allows version tracking and version validation of the data contained within the ZenodoBackpack. 
      
 **download_and_extract**: takes a DOI string to download, extract and verify a zenodo_backpack archive from Zenodo.org to target directory. This returns a ZenodoBackpack object that can be queried for information. 
     
 
@@ -71,18 +74,18 @@
 ```
 creator = zenodo_backpack.ZenodoBackpackCreator()
 creator.create("/path/to/payload_directory", "path/to/archive.tar.gz", "0.1")
 ```
 
 ### Download a backpack
 
-Download a backpack from Zenodo, defined by the DOI:
+Download a backpack from Zenodo, defined by the DOI. The version is optional, and if not provided, the latest version will be downloaded.:
 ```
 backpack_downloader = zenodo_backpack.ZenodoBackpackDownloader()
-backpack = backpack_downloader.download_and_extract('/path/to/download_directory', 'MY.DOI/111111')
+backpack = backpack_downloader.download_and_extract('/path/to/download_directory', 'MY.DOI/111111', version='MY.VERSION')
 ```
 
 ### Read a backpack that is already downloaded
 
 Defined by a path
 ```
 backpack = zenodo_backpack.acquire(path='/path/to/zenodobackpack/', md5sum=True)
@@ -98,18 +101,24 @@
 
 ```
 useful_data_path = zenodo_backpack.acquire(env_var_name='MyZenodoBackpack', version="1.5.2").payload_directory_string()
 ```
 
 # Installation
 
+zenodo_backpack can be installed from pypi:
+
+```
+pip install zenodo-backpack
+```
+
 The easiest way to install is using conda:
 
 ```
-conda install -c bioconda zenodo_backpack
+conda install -c conda-forge zenodo_backpack
 ```
 
 Alternatively, you can git clone the repository and either run the bin/zenodo_backpack executable or install it with setup tools using 
 
 ```
 python setup.py install
 ```
```

### Comparing `zenodo_backpack-0.2.0/README.md` & `zenodo_backpack-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ZenodoBackpack uploads/downloads data to/from [Zenodo](https://zenodo.org),
 which means that each dataset is associated with a DOI. Additionally, it
 encapsulates the uploaded data in a Zenodo Backpack format, which is really just
 a `CONTENTS.json` file and compresses the data in `.tar.gz` format before
 upload. The `CONTENTS.json` file includes md5sum values for each included file
 for robust verification.
 
-It contains two main methods, which can bee accessed through the
+It contains two main methods, which can be accessed through the
 `zenodo_backpack` script or accessed as a software library:
 
 **create**: turns a target directory into a zenodo_backpack-formatted .tar.gz archive with relevant checksum and version information, ready to be uploaded to Zenodo. It is necessary to provide a data version when doing so - furthermore, when uploading this backpack to zenodo.org, the version specified on the website **must** match that provided when the ZenodoBackpack was created. This allows version tracking and version validation of the data contained within the ZenodoBackpack. 
      
 **download_and_extract**: takes a DOI string to download, extract and verify a zenodo_backpack archive from Zenodo.org to target directory. This returns a ZenodoBackpack object that can be queried for information. 
     
 
@@ -56,18 +56,18 @@
 ```
 creator = zenodo_backpack.ZenodoBackpackCreator()
 creator.create("/path/to/payload_directory", "path/to/archive.tar.gz", "0.1")
 ```
 
 ### Download a backpack
 
-Download a backpack from Zenodo, defined by the DOI:
+Download a backpack from Zenodo, defined by the DOI. The version is optional, and if not provided, the latest version will be downloaded.:
 ```
 backpack_downloader = zenodo_backpack.ZenodoBackpackDownloader()
-backpack = backpack_downloader.download_and_extract('/path/to/download_directory', 'MY.DOI/111111')
+backpack = backpack_downloader.download_and_extract('/path/to/download_directory', 'MY.DOI/111111', version='MY.VERSION')
 ```
 
 ### Read a backpack that is already downloaded
 
 Defined by a path
 ```
 backpack = zenodo_backpack.acquire(path='/path/to/zenodobackpack/', md5sum=True)
@@ -83,18 +83,24 @@
 
 ```
 useful_data_path = zenodo_backpack.acquire(env_var_name='MyZenodoBackpack', version="1.5.2").payload_directory_string()
 ```
 
 # Installation
 
+zenodo_backpack can be installed from pypi:
+
+```
+pip install zenodo-backpack
+```
+
 The easiest way to install is using conda:
 
 ```
-conda install -c bioconda zenodo_backpack
+conda install -c conda-forge zenodo_backpack
 ```
 
 Alternatively, you can git clone the repository and either run the bin/zenodo_backpack executable or install it with setup tools using 
 
 ```
 python setup.py install
 ```
```

### Comparing `zenodo_backpack-0.2.0/bin/zenodo_backpack` & `zenodo_backpack-0.3.0/bin/zenodo_backpack`

 * *Files identical despite different names*

### Comparing `zenodo_backpack-0.2.0/setup.py` & `zenodo_backpack-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `zenodo_backpack-0.2.0/zenodo_backpack/__init__.py` & `zenodo_backpack-0.3.0/zenodo_backpack/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             raise ZenodoBackpackMalformedException(f"{logging_description} does not contain a CONTENTS.json file, so is not a valid ZenodoBackpack")
     else:
         raise ZenodoBackpackMalformedException(f"{logging_description} is not a directory so cannot hold a ZenodoBackpack")
 
 
 class ZenodoBackpackDownloader:
 
-    def download_and_extract(self, directory, doi, check_version=True, progress_bar=False, download_retries=3):
+    def download_and_extract(self, directory, doi, check_version=True, progress_bar=False, download_retries=3, version=None):
         """Actually do the download, to a given path. Also extract the archive,
         and then call verify on it.
 
         Parameters
         ----------
         directory: str
             Where to download to
@@ -145,24 +145,26 @@
             DOI of the Zenodo series
         progress_bar: bool
             If True, display graphical progress bar while downloading from Zenodo
         check_version: bool
             If True, check Zenodo metadata verifies
         download_retries: int
             Number of download attempts
+        version: None or str
+            If None, return the newest version. If specified, target that specific version.
 
         Returns a ZenodoBackpack object containing the downloaded files
         """
         self._make_sure_path_exists(directory)
 
         # get record via DOI, then read in json metadata from records_url
         if doi is not None:
 
-            recordID = self._retrieve_record_ID(doi)
-            metadata, files = self._retrieve_record_metadata(recordID)
+            example_recordID = self._retrieve_record_ID(doi)
+            metadata, files = self._retrieve_record_metadata(example_recordID, version)
 
             # create md5sums file for download
             with open(os.path.join(directory, 'md5sums.txt'), 'wt') as md5file:
                 for file in files:
                     fname = str(file['key']).split('/')[-1]
                     checksum = str(file['checksum']).split(':')[-1]
                     md5file.write('{},{}\n'.format(checksum, fname))
@@ -287,14 +289,15 @@
 
         logging.info('Verification success.')
 
     def _retrieve_record_ID(self, doi):
         """Parses provided DOI retrieve associated Zenodo URL which also contains record ID
         Arguments:
             DOI (str): published DOI associated with file uploaded to Zenodo
+            version: If None, return the newest version. If specified, target that specific version.
         Returns:
             recordID (str): last part of Zenodo url associated with DOI
         """
 
         if not doi.startswith('http'):
             doi = 'https://doi.org/' + doi
         try:
@@ -304,32 +307,64 @@
             raise ZenodoConnectionException('Connection error: {}'.format(e))
         if not r.ok:
             raise ZenodoConnectionException('DOI could not be resolved. Check your DOI is correct.')
 
         recordID = r.url.split('/')[-1].strip()
         return recordID
 
-    def _retrieve_record_metadata(self, recordID):
+    def _retrieve_record_json(self, recordID):
         """Parses provided recordID to access Zenodo API records and download metadata json
         Arguments:
             recordID (str): Zenodo record number
         Returns:
-            js (json object): json metadata file retrieved from Zenodo API.
-            js['files'] (list): list of files associated with recordID in question
+            json response from Zenodo API
         """
         records_url = 'https://zenodo.org/api/records/'
 
         try:
             r = requests.get(records_url + recordID, timeout=15.)
+            return json.loads(r.text)
+        except Exception as e:
+            raise ZenodoConnectionException('Error during metadata retrieval: {}'.format(e))
+
+    def _retrieve_versions_record_json(self, recordID, version):
+        """Parses provided recordID to access Zenodo API records and download metadata json
+        Arguments:
+            recordID (str): Zenodo record number
+            version: (str): Target that specific version.
+        Returns:
+            json response from Zenodo API
+        """
+        records_url = 'https://zenodo.org/api/records/'
+
+        try:
+            r = requests.get(records_url + recordID + '/versions', timeout=15.)
         except Exception as e:
             raise ZenodoConnectionException('Error during metadata retrieval: {}'.format(e))
 
-        if r.ok:
-            js = json.loads(r.text)
-            return js, js['files']
+        js = json.loads(r.text)
+        versions = js['hits']['hits']
+        for v in versions:
+            if v['metadata']['version'] == version:
+                return v
+
+    def _retrieve_record_metadata(self, recordID, version):
+        """Parses provided recordID to access Zenodo API records and download metadata json
+        Arguments:
+            recordID (str): Zenodo record number
+            version: (None or str): If None, return the newest version. If specified, target that specific version.
+        Returns:
+            js (json object): json metadata file retrieved from Zenodo API.
+            js['files'] (list): list of files associated with recordID in question
+        """
+        if version is None:
+            js = self._retrieve_record_json(recordID)
+        else:
+            js = self._retrieve_versions_record_json(recordID, version)
+        return js, js['files']
 
     def _check_hash(self, filename, checksum, metadata=True):
         """Compares MD5 sum of file to checksum
         Arguments:
             filename (str): Path of file to md5sum
             checkmsum: (str): md5 checksum
```

### Comparing `zenodo_backpack-0.2.0/zenodo_backpack.egg-info/PKG-INFO` & `zenodo_backpack-0.3.0/zenodo_backpack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
-Name: zenodo-backpack
-Version: 0.2.0
+Name: zenodo_backpack
+Version: 0.3.0
 Summary: Manage data bundled with bioinformatic software through Zenodo DOI integration
 Home-page: https://github.com/centre-for-microbiome-research/zenodo_backpack
 Author: ['Alex Chklovski', 'Ben Woodcroft']
 Author-email: chklovski@gmail.com
 License: GPL3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: tqdm
+Requires-Dist: requests
 
 # zenodo_backpack
 
 ZenodoBackpack provides a robust, standardised and repeatable approach to
 distributing and using backend databases that bioinformatic tools rely on. These
 databases are usually tool-specific and are often large enough in size that they
 cannot be uploaded as data to software repositories (e.g. PyPI imposes a limit
@@ -24,15 +27,15 @@
 ZenodoBackpack uploads/downloads data to/from [Zenodo](https://zenodo.org),
 which means that each dataset is associated with a DOI. Additionally, it
 encapsulates the uploaded data in a Zenodo Backpack format, which is really just
 a `CONTENTS.json` file and compresses the data in `.tar.gz` format before
 upload. The `CONTENTS.json` file includes md5sum values for each included file
 for robust verification.
 
-It contains two main methods, which can bee accessed through the
+It contains two main methods, which can be accessed through the
 `zenodo_backpack` script or accessed as a software library:
 
 **create**: turns a target directory into a zenodo_backpack-formatted .tar.gz archive with relevant checksum and version information, ready to be uploaded to Zenodo. It is necessary to provide a data version when doing so - furthermore, when uploading this backpack to zenodo.org, the version specified on the website **must** match that provided when the ZenodoBackpack was created. This allows version tracking and version validation of the data contained within the ZenodoBackpack. 
      
 **download_and_extract**: takes a DOI string to download, extract and verify a zenodo_backpack archive from Zenodo.org to target directory. This returns a ZenodoBackpack object that can be queried for information. 
     
 
@@ -71,18 +74,18 @@
 ```
 creator = zenodo_backpack.ZenodoBackpackCreator()
 creator.create("/path/to/payload_directory", "path/to/archive.tar.gz", "0.1")
 ```
 
 ### Download a backpack
 
-Download a backpack from Zenodo, defined by the DOI:
+Download a backpack from Zenodo, defined by the DOI. The version is optional, and if not provided, the latest version will be downloaded.:
 ```
 backpack_downloader = zenodo_backpack.ZenodoBackpackDownloader()
-backpack = backpack_downloader.download_and_extract('/path/to/download_directory', 'MY.DOI/111111')
+backpack = backpack_downloader.download_and_extract('/path/to/download_directory', 'MY.DOI/111111', version='MY.VERSION')
 ```
 
 ### Read a backpack that is already downloaded
 
 Defined by a path
 ```
 backpack = zenodo_backpack.acquire(path='/path/to/zenodobackpack/', md5sum=True)
@@ -98,18 +101,24 @@
 
 ```
 useful_data_path = zenodo_backpack.acquire(env_var_name='MyZenodoBackpack', version="1.5.2").payload_directory_string()
 ```
 
 # Installation
 
+zenodo_backpack can be installed from pypi:
+
+```
+pip install zenodo-backpack
+```
+
 The easiest way to install is using conda:
 
 ```
-conda install -c bioconda zenodo_backpack
+conda install -c conda-forge zenodo_backpack
 ```
 
 Alternatively, you can git clone the repository and either run the bin/zenodo_backpack executable or install it with setup tools using 
 
 ```
 python setup.py install
 ```
```

