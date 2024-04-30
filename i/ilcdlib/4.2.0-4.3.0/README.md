# Comparing `tmp/ilcdlib-4.2.0.tar.gz` & `tmp/ilcdlib-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-4.2.0.tar", max compression
+gzip compressed data, was "ilcdlib-4.3.0.tar", max compression
```

## Comparing `ilcdlib-4.2.0.tar` & `ilcdlib-4.3.0.tar`

### file list

```diff
@@ -1,62 +1,66 @@
--rw-r--r--   0        0        0    11357 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/LICENSE
--rw-r--r--   0        0        0     4949 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/README.md
--rw-r--r--   0        0        0     3525 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    17587 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0      837 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/compat/__init__.py
--rw-r--r--   0        0        0     1158 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/compat/pydantic.py
--rw-r--r--   0        0        0     1796 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     4407 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     7064 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     3361 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     6003 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     4173 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     7981 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     4224 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3930 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3798 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0     3331 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/validation.py
--rw-r--r--   0        0        0      837 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10064 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     6864 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     2170 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/epditaly.py
--rw-r--r--   0        0        0     1329 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     1156 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/itb.py
--rw-r--r--   0        0        0     2217 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3532 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    32351 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     2067 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7667 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0     2669 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     3128 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     2588 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1735 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1122 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/sanitizing/text.py
--rw-r--r--   0        0        0      837 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0    10951 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     2770 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/soda4lca/api_client_4x.py
--rw-r--r--   0        0        0     1206 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     3951 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/LICENSE
+-rw-r--r--   0        0        0     4949 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/README.md
+-rw-r--r--   0        0        0     3525 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    17587 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0      837 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/compat/__init__.py
+-rw-r--r--   0        0        0     1158 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/compat/pydantic.py
+-rw-r--r--   0        0        0     1835 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0     4934 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/data/category_mapping/epdnorge.csv
+-rw-r--r--   0        0        0    51577 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/data/category_mapping/oekobaudat.csv
+-rw-r--r--   0        0        0   172140 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     6454 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     7064 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     3361 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     4173 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     7981 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     4224 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3788 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3331 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     6864 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     2170 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/epditaly.py
+-rw-r--r--   0        0        0     2341 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/epdnorge.py
+-rw-r--r--   0        0        0     1329 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     2105 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/itb.py
+-rw-r--r--   0        0        0     3876 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3644 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    35343 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2248 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7895 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0    10680 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/category.py
+-rw-r--r--   0        0        0     3603 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     3522 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     6247 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1866 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0    11347 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     2755 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/soda4lca/api_client_4x.py
+-rw-r--r--   0        0        0     1206 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     6465 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.3.0/PKG-INFO
```

### Comparing `ilcdlib-4.2.0/LICENSE` & `ilcdlib-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/README.md` & `ilcdlib-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/pyproject.toml` & `ilcdlib-4.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "4.2.0"
+version = "4.3.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/__init__.py` & `ilcdlib-4.3.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/__main__.py` & `ilcdlib-4.3.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/__version__.py` & `ilcdlib-4.3.0/src/ilcdlib/__version__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/cli.py` & `ilcdlib-4.3.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/common.py` & `ilcdlib-4.3.0/src/ilcdlib/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/compat/__init__.py` & `ilcdlib-4.3.0/src/ilcdlib/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/compat/pydantic.py` & `ilcdlib-4.3.0/src/ilcdlib/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/const.py` & `ilcdlib-4.3.0/src/ilcdlib/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #  Find out more at www.BuildingTransparency.org
 #
 from enum import StrEnum
 
 ILCD_IDENTIFICATION: tuple[str] = ("ILCD_EPD",)
 PDF_ATTACHMENT = "PDF"
 URL_ATTACHMENT = "URL"
+OPENEPD_PRODUCT_CLASS_NAME = "openEPD"
 
 
 class IlcdContactClass(StrEnum):
     """Enumeration of ILCD contact classes."""
 
     Person = "Persons"
     Company = "Organisations"
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-4.3.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/category.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/compliance.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/contact.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/exchage.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/exchage.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/flow.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/lcia.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/material.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/source.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/unit.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from dataclasses import dataclass
 
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader
 from ilcdlib.mapping.common import BaseDataMapper
-from ilcdlib.mapping.units import default_units_uuid_mapper
+from ilcdlib.mapping.units import default_units_mapper
 from ilcdlib.type import LangDef
 from ilcdlib.utils import none_throws
 from ilcdlib.xml_parser import T_ET
 
 
 @dataclass(kw_only=True)
 class UnitDto:
@@ -39,15 +39,15 @@
     """Read an ILCD Unit Group XML file."""
 
     def __init__(
         self,
         element: T_ET.Element,
         data_provider: BaseIlcdMediumSpecificReader,
         *,
-        unit_mapper: BaseDataMapper[str, str] = default_units_uuid_mapper,
+        unit_mapper: BaseDataMapper[str, str] = default_units_mapper,
     ):
         super().__init__(data_provider)
         self._entity = element
         self.unit_mapper = unit_mapper
 
     def get_uuid(self) -> str:
         """Get the UUID of the entity described by this data set."""
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/entity/validation.py` & `ilcdlib-4.3.0/src/ilcdlib/entity/validation.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-4.3.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/epd/cli.py` & `ilcdlib-4.3.0/src/ilcdlib/epd/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/epd/dialect/epditaly.py` & `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/epditaly.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/epd/dialect/itb.py` & `ilcdlib-4.3.0/src/ilcdlib/mapping/properties.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from ilcdlib.epd.reader import IlcdEpdReader
+from ilcdlib.mapping.common import SimpleDataMapper
 
 
-class ItbIlcdXmlEpdReader(IlcdEpdReader):
-    """Reader for EPDs in the Itb specific ILCD XML format."""
+class PropertiesUUIDMapper(SimpleDataMapper[str]):
+    """A data mapper that maps units ILCD UUIDs to standartized names."""
 
-    @classmethod
-    def is_known_url(cls, url: str) -> bool:
-        """Return whether the URL recognized as a known Itb URL."""
-        return "itb" in url.lower()
+    DATABASE = {
+        "7e18d0ad-e78e-47a0-8e96-1c0a581902e2": "mass",
+        "838aaa23-0117-11db-92e3-0800200c9a66": "length",
+    }
+
+
+default_properties_uuid_mapper = PropertiesUUIDMapper()
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/itb.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,38 +13,41 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from ilcdlib.dto import ProductClassDef
+from ilcdlib.dto import IlcdContactInfo, OpenEpdIlcdOrg, ValidationDto
 from ilcdlib.epd.reader import IlcdEpdReader
-from ilcdlib.utils import none_throws
+from ilcdlib.type import LangDef
 
 
-class OekobauDatIlcdXmlEpdReader(IlcdEpdReader):
-    """Reader for EPDs in the Oekobau.DAT specific ILCD XML format."""
+class ItbIlcdXmlEpdReader(IlcdEpdReader):
+    """Reader for EPDs in the Itb specific ILCD XML format."""
 
     @classmethod
     def is_known_url(cls, url: str) -> bool:
-        """Return whether the URL recognized as a known Environdec URL."""
-        return "oekobaudat" in url.lower()
+        """Return whether the URL recognized as a known Itb URL."""
+        return "itb" in url.lower()
 
-    def post_init(self):
-        """Configure Oekobau.DAT specific settings."""
-        self.xml_parser.xml_ns["epd2019"] = self.xml_parser.xml_ns["epd2019_indata"]
-
-    def _product_classes_to_openepd(self, classes: dict[str, list[ProductClassDef]]) -> dict[str, list[str] | str]:
+    def get_third_party_verifier_email(self, validations: list[ValidationDto]) -> OpenEpdIlcdOrg | None:
         """
-        Convert the product classes to OpenEPD format.
+        Return first third party verifier email.
 
-        The Oekobau.DAT format according to openEPD is a string containing full id and
-        the name of the most specific class. Example: "1.1.01 Cement"
+        ITB contains personal info instead of organization info.
         """
-        result = super()._product_classes_to_openepd(classes)
-        for classification_name, class_defs in classes.items():
-            if classification_name.lower() == "oekobau.dat" and len(class_defs) > 0:
-                last_class = class_defs[-1]
-                del result[classification_name]
-                result["oekobau.dat"] = " ".join((none_throws(last_class.id), none_throws(last_class.name)))
-        return result
+        verifier = self.get_third_party_verifier(validations)
+        if not verifier:
+            return None
+        contact = verifier.get_contact()
+        if contact is None:
+            return None
+        return IlcdContactInfo.parse_obj(contact).email
+
+    def get_product_description(self, lang: LangDef) -> str | None:
+        """Return the product description in the given language."""
+        return self._get_localized_text(
+            self.epd_el_tree,
+            ("process:processInformation", "process:technology", "process:technologicalApplicability"),
+            lang,
+        )
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/epd/factory.py` & `ilcdlib-4.3.0/src/ilcdlib/epd/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from typing import Type
 
 from ilcdlib.epd.dialect.environdec import EnvirondecIlcdXmlEpdReader
 from ilcdlib.epd.dialect.epditaly import EpdItalyIlcdXmlEpdReader
+from ilcdlib.epd.dialect.epdnorge import EpdNorgeIlcdXmlEpdReader
 from ilcdlib.epd.dialect.indata import IndataIlcdXmlEpdReader
 from ilcdlib.epd.dialect.itb import ItbIlcdXmlEpdReader
 from ilcdlib.epd.dialect.oekobaudat import OekobauDatIlcdXmlEpdReader
 from ilcdlib.epd.reader import IlcdEpdReader
 
 
 class EpdReaderFactory:
@@ -33,14 +34,15 @@
     __DIALECTS: dict[str, Type[IlcdEpdReader]] = {
         "environdec": EnvirondecIlcdXmlEpdReader,
         "indata": IndataIlcdXmlEpdReader,
         "oekobau.dat": OekobauDatIlcdXmlEpdReader,
         "oekobaudat": OekobauDatIlcdXmlEpdReader,
         "epditaly": EpdItalyIlcdXmlEpdReader,
         "itb": ItbIlcdXmlEpdReader,
+        "epdnorge": EpdNorgeIlcdXmlEpdReader,
     }
     DEFAULT_READER_CLASS = IlcdEpdReader
 
     def get_supported_dialects(self) -> list[str]:
         """Return a list of supported dialects."""
         return list(self.__DIALECTS.keys())
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/epd/reader.py` & `ilcdlib-4.3.0/src/ilcdlib/epd/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,35 +14,45 @@
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import datetime
+import itertools
 from typing import IO, Type
 
 from openepd.model.common import Amount, Measurement
 from openepd.model.epd import Epd
 from openepd.model.lcia import Impacts, ImpactSet, OutputFlowSet, ResourceUseSet
 from openepd.model.specs import Specs
 from openepd.model.standard import Standard
 
 from ilcdlib import const
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdEdpSupportReader
 from ilcdlib.const import IlcdDatasetType, IlcdTypeOfReview
-from ilcdlib.dto import ComplianceDto, IlcdReference, OpenEpdIlcdOrg, ProductClassDef, ValidationDto
+from ilcdlib.dto import (
+    CategoryCandidate,
+    ComplianceDto,
+    IlcdReference,
+    MappedCategory,
+    OpenEpdIlcdOrg,
+    ProductClassDef,
+    ValidationDto,
+)
 from ilcdlib.entity.compliance import IlcdComplianceListReader
 from ilcdlib.entity.contact import IlcdContactReader
 from ilcdlib.entity.exchage import IlcdExchangesReader
 from ilcdlib.entity.flow import IlcdExchangeDto, IlcdFlowReader
 from ilcdlib.entity.lcia import IlcdLciaResultsReader
 from ilcdlib.entity.material import MatMlMaterial
 from ilcdlib.entity.pcr import IlcdPcrReader
 from ilcdlib.entity.validation import IlcdValidationListReader
 from ilcdlib.extension import IlcdEpdExtension
+from ilcdlib.mapping.category import CategoryMapper, CsvCategoryMapper, NoopCategoryMapper
 from ilcdlib.mapping.compliance import StandardNameToLCIAMethodMapper, default_standard_names_to_lcia_mapper
 from ilcdlib.sanitizing.text import trim_text
 from ilcdlib.type import LangDef
 from ilcdlib.utils import (
     MarkdownSectionBuilder,
     create_ext,
     create_openepd_attachments,
@@ -427,14 +437,18 @@
             if verifier.validation_type in (
                 IlcdTypeOfReview.IndependentExternalReview,
                 IlcdTypeOfReview.AccreditedThirdPartyReview,
             ):
                 return verifier.org
         return None
 
+    def get_third_party_verifier_email(self, validations: list[ValidationDto]) -> OpenEpdIlcdOrg | None:
+        """Return first third party verifier email."""
+        return None
+
     def get_pcr_reader(self) -> IlcdPcrReader | None:
         """Return the reader for the PCR."""
         element = self._get_external_tree(
             self.epd_el_tree,
             (
                 "process:modellingAndValidation",
                 "process:LCIMethodAndAllocation",
@@ -631,23 +645,41 @@
     def get_output_flows(self, scenario_names: dict[str, str]) -> OutputFlowSet | None:
         """Return output flows."""
         reader = self.get_exchanges_reader()
         if reader is None:
             return None
         return reader.get_output_flows(scenario_names)
 
-    def _product_classes_to_openepd(self, classes: dict[str, list[ProductClassDef]]) -> dict[str, list[str] | str]:
-        result: dict[str, list[str] | str] = {}
+    def _product_classes_to_openepd(self, classes: dict[str, list[ProductClassDef]]) -> dict[str, str]:
+        result: dict[str, str] = {}
         for classification_name, class_defs in classes.items():
             if len(class_defs) > 0:
                 result[classification_name] = (
                     (class_defs[-1].id or "") + " " + " / ".join([none_throws(x.name) for x in class_defs])
                 ).strip()
         return result
 
+    def _get_mapped_categories(self, product_classes: dict[str, str]) -> list[MappedCategory]:
+        candidates: list[MappedCategory] = []
+        for classification_name, class_name in product_classes.items():
+            candidates += self.get_category_mapper(classification_name).map(class_name, [])  # type: ignore
+        return candidates
+
+    def _get_category_candidates(self, mapped_categories: list[MappedCategory]) -> list[CategoryCandidate]:
+        result: list[CategoryCandidate] = []
+        for mc in mapped_categories:
+
+            candidate = CategoryCandidate(category=mc.openepd_category_id)
+            result.append(candidate)
+        buckets = itertools.groupby(result, key=lambda x: x.category)
+        return [next(v) for k, v in buckets]
+
+    def _set_specs_for_category_candidate(self, candidate: CategoryCandidate):
+        pass
+
     def to_openepd_epd(
         self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None
     ) -> Epd:  # NOSONAR
         """Return the EPD as OpenEPD object."""
         if provider_domain is None:
             provider_domain = provider_domain_name_from_url(base_url)
         lang_code = lang if isinstance(lang, str) else None
@@ -693,33 +725,41 @@
             if mapped:
                 lcia_method = mapped
                 break
 
         epd_developer = self.get_data_entry_by(lang, base_url)
         epd_developer_contact = epd_developer.get_contact() if epd_developer else None
         ilcd_validations = self.get_ilcd_validations(lang, base_url, provider_domain)
+        product_classes = self._product_classes_to_openepd(self.get_product_classes())
+        # Category mapping
+        mapped_categories = self._get_mapped_categories(product_classes)
+        category_candidates = self._get_category_candidates(mapped_categories)
+        if const.OPENEPD_PRODUCT_CLASS_NAME not in product_classes and len(category_candidates) == 1:
+            product_classes[const.OPENEPD_PRODUCT_CLASS_NAME] = category_candidates[0].category
+        # Compose the final object
         epd = Epd(
             doctype="OpenEPD",
             language=lang_code,
             attachments=create_openepd_attachments(own_ref, base_url) if base_url else None,  # type: ignore
             declaration_url=own_ref.to_url(base_url) if own_ref and base_url else None,  # type: ignore
             product_name=product_name,
             product_description=trim_text(self.get_product_description(lang), 2000, ellipsis="..."),
             date_of_issue=date_to_datetime(self.get_date_published(), self.timezone),
             valid_until=date_to_datetime(self.get_validity_ends_date(), self.timezone),
             program_operator_doc_id=self.get_program_operator_id(),
             manufacturer=manufacturer,
             epd_developer=epd_developer,
             epd_developer_email=epd_developer_contact.email if epd_developer_contact else None,
             program_operator=program_operator,
-            product_classes=self._product_classes_to_openepd(self.get_product_classes()),
+            product_classes=product_classes,
             manufacturing_description=self.get_technology_description(lang),
             product_usage_description=self.get_technological_applicability(lang),
             lca_discussion=self.get_lca_discussion(lang),
             third_party_verifier=self.get_third_party_verifier(ilcd_validations),
+            third_party_verifier_email=self.get_third_party_verifier_email(ilcd_validations),
             pcr=pcr,
             declared_unit=declared_unit,
             impacts=self.get_impacts(scenario_names, lca_method=lcia_method),
             resource_uses=self.get_resource_uses(scenario_names),
             output_flows=self.get_output_flows(scenario_names),
             specs=specs,
             compliance=compliance,
@@ -733,14 +773,15 @@
 
         ilcd_ext = IlcdEpdExtension(
             dataset_type=self.get_dataset_type(),
             dataset_version=self.get_version(),
             dataset_uuid=self.get_uuid(),
             production_location=self.get_production_location(),
             epd_verifiers=ilcd_validations,
+            category_candidates=category_candidates,
         )
         if publisher:
             ilcd_ext.epd_publishers.append(publisher)
         epd.set_ext(ilcd_ext)
         return epd
 
     @classmethod
@@ -748,7 +789,32 @@
         """
         Return whether the URL recognized by this particular reader.
 
         This method should be overriden by the dialect and return true if the input URL is know url for this dialect.
         """
 
         return False
+
+    @classmethod
+    def _create_category_mapper(cls, classification_name: str) -> CsvCategoryMapper | None:
+        """
+        Create category mapper for this reader.
+
+        This method should be overriden by the dialect and return the category mapper for this dialect.
+        Never call this method directly. Use get_category_mapper() instead.
+        """
+        return None
+
+    def get_category_mapper(self, classification_name: str) -> CategoryMapper:
+        """Return the category mapper for this reader.
+
+        It will either return a cached on a class-level instance or create a new one if it does not exist.
+        """
+        if not hasattr(self.__class__, "_category_mapper"):
+            self.__class__._category_mappers = {}  # type: ignore[attr-defined]
+        mappers: dict[str, CategoryMapper] = self.__class__._category_mappers  # type: ignore[attr-defined]
+        if classification_name not in mappers:
+            mapper: CategoryMapper | None = self._create_category_mapper(classification_name)
+            if mapper is None:
+                mapper = NoopCategoryMapper()
+            mappers[classification_name] = mapper
+        return mappers[classification_name]
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/extension.py` & `ilcdlib-4.3.0/src/ilcdlib/extension.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,28 +17,32 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from openepd.model.base import OpenEpdExtension
 
 from ilcdlib import const
 from ilcdlib.compat.pydantic import pyd
-from ilcdlib.dto import IlcdContactInfo, OpenEpdIlcdOrg, ValidationDto
+from ilcdlib.dto import CategoryCandidate, IlcdContactInfo, OpenEpdIlcdOrg, ValidationDto
 
 
 class IlcdEpdExtension(OpenEpdExtension):
     """An ILCD extension for OpenEPD Epd object."""
 
     dataset_type: str | None = None
     dataset_version: str | None = None
     dataset_uuid: str | None = None
     production_location: str | None = None
     epd_publishers: list[OpenEpdIlcdOrg] = pyd.Field(default_factory=list, description="List of EPD publishers")
     epd_verifiers: list[ValidationDto] = pyd.Field(
         default_factory=list, description="List of EPD verifiers (both, external and internal)"
     )
+    category_candidates: list[CategoryCandidate] = pyd.Field(
+        default_factory=list,
+        description="List of category candidates for the EPD.",
+    )
 
     @classmethod
     def get_extension_name(cls) -> str:
         """Return the name of the extension to be used as a key in ext dict."""
         return const.ILCD_IDENTIFICATION[0]
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/http_common.py` & `ilcdlib-4.3.0/src/ilcdlib/http_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     def __init__(
         self,
         base_url: str,
         *,
         xml_parser: XmlParser | None = None,
         user_agent: str | None = None,
-        timeout: float | tuple[float, float] | None = None,
+        timeout: float | tuple[float, float] | None = (2.0, 60.0),
         retry_strategy: Retry | None = None,
         requests_per_sec: float = 10,
     ) -> None:
         """
         Create a new instance of the API client.
 
         :param base_url: common part that all request URLs start with
@@ -112,14 +112,15 @@
         Note: when `backoff_factor` is set, the time between attempts will be exponentially increased according to
         the following formula: `{backoff_factor} * (2 ** ({number_retries} - 1))`. For the factor of 2 the periods
         will be like this: 1, 2, 4, 8, 16, 32, 64, 128, 256, 512, ...
         :return:
         """
         return Retry(
             total=5,
+            connect=2,
             backoff_factor=2,
             respect_retry_after_header=True,
             status_forcelist=frozenset({413, 429, 500, 502, 503, 504}),
         )
 
     @property
     def base_url(self):
@@ -134,15 +135,17 @@
             headers["user-agent"] = self.user_agent
         return headers
 
     @property
     def _current_session(self) -> requests.Session:
         if self._session is None:
             self._session = requests.Session()
-            self._session.mount("", HTTPAdapter(max_retries=self._retry_strategy))
+            http_adapter = HTTPAdapter(max_retries=self._retry_strategy)
+            self._session.mount("https://", http_adapter)
+            self._session.mount("http://", http_adapter)
         return self._session
 
     def _on_before_do_request(self):
         """Run some custom logic before `do_request`. Can be overridden to check / refresh access tokens."""
         pass
 
     def download_by_url(self, url, method="get", **kwargs) -> BytesIO:
@@ -188,23 +191,26 @@
         params=None,
         data=None,
         json=None,
         files=None,
         headers=None,
         session: requests.Session | None = None,
         raise_for_status: bool = True,
+        timeout: float | tuple[float, float] | None = None,
         **kwargs,
     ) -> requests.Response:
         headers = headers or self.default_headers
 
         self._on_before_do_request()
 
         url = self._get_url_for_request(endpoint)
 
-        request_kwargs = dict(params=params, data=data, json=json, files=files, headers=headers, timeout=self.timeout)
+        request_kwargs = dict(
+            params=params, data=data, json=json, files=files, headers=headers, timeout=timeout or self.timeout
+        )
         request_kwargs.update(kwargs)
 
         s = session or self._current_session
 
         with self._throttler.throttle():
             response = s.request(method, url, **request_kwargs)
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-4.3.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/mapping/common.py` & `ilcdlib-4.3.0/src/ilcdlib/mapping/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #
 __all__ = (
     "BaseDataMapper",
     "SimpleDataMapper",
 )
 
 import abc
+import re
 from typing import Generic, TypeVar, cast
 
 T = TypeVar("T")
 K = TypeVar("K")
 
 
 class BaseDataMapper(Generic[T, K], abc.ABC):
@@ -71,7 +72,31 @@
         :param default_value: The default value to return if there is no mapping for input value.
         """
         for impact_name, keywords in self.KV.items():
             for keyword in keywords:
                 if str(keyword).strip().lower() in input_value.strip().lower():
                     return cast(T, impact_name)
         return default_value
+
+
+class RegexMapper(BaseDataMapper[str, T], Generic[T]):
+    """A data mapper that maps input values to output values using regex."""
+
+    PATTERNS: dict[str, str] = {}
+    _compiled_patterns: dict[str, re.Pattern]
+
+    def __init__(self) -> None:
+        self._compiled_patterns: dict[str, re.Pattern] = {
+            key: re.compile(pattern, re.IGNORECASE) for key, pattern in self.PATTERNS.items()
+        }
+
+    def map(self, input_value: str, default_value: T | None) -> T | None:
+        """
+        Map the input value to the output value using regex.
+
+        :param input_value: The input value to map.
+        :param default_value: The default value to return if there is no mapping for input value.
+        """
+        for impact_name, pattern in self._compiled_patterns.items():
+            if pattern.search(input_value.strip().lower()):
+                return cast(T, impact_name)
+        return default_value
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/mapping/compliance.py` & `ilcdlib-4.3.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/mapping/flows.py` & `ilcdlib-4.3.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-4.3.0/src/ilcdlib/mapping/impacts.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from ilcdlib.mapping.common import BaseDataMapper, K, KeyValueMapper, SimpleDataMapper
+from ilcdlib.mapping.common import BaseDataMapper, K, KeyValueMapper, RegexMapper, SimpleDataMapper
 from ilcdlib.utils import is_valid_uuid
 
 
 class ImpactsUUIDToOpenIdMapper(SimpleDataMapper[str]):
     """Map ILCD UUIDs to openEPD impact names."""
 
     DATABASE = {
@@ -44,35 +44,45 @@
 
 class ImpactsKeywordToOpenIdMapper(KeyValueMapper[str]):
     """Map keywords to openEPD impact names.""" ""
 
     KV = {
         "gwp-biogenic": ["biogenic"],
         "gwp-luluc": ["luluc"],
-        "gwp-fossil": ["fossil"],
-        "gwp-gwp_nonCO2": ["CO2"],
-        "gwp": ["gwp", "global warming"],
+        "gwp-nonCO2": ["CO2"],
         "ep-marine": ["marine"],
-        "ep-fresh": ["fresh", "fw"],
-        "ep-terr": ["terr"],
-        "ep": ["ep", "eutrophication"],
+        "ep-fresh": ["freshwater", "fw"],
+        "ep-terr": ["terrestrial"],
         "odp": ["odp", "depletion"],
         "ap": ["ap", "acidification"],
         "pocp": ["pocp", "photochemical", "smog", "ozone creation"],
     }
 
 
+class ImpactsRegexToOpenIdMapper(RegexMapper[str]):
+    """Map impact names using regex.""" ""
+
+    PATTERNS = {
+        "gwp-fossil": r"^(?!.*\bnon\b)(?=.*\b(fossil)\b)(?=.*\b(gwp|global warming)\b).*$",
+        "gwp": r"^(?!.*\b(fossil|luluc|CO2|total)\b)(?=.*\b(gwp|global warming)\b).*$",
+    }
+
+
 class DefaultImpactsToOpenIdMapper(BaseDataMapper[str, str]):
     """Map default impacts to openEPD impact names."""
 
     def __init__(self):
         self._uuid_mapper = ImpactsUUIDToOpenIdMapper()
         self._keyword_mapper = ImpactsKeywordToOpenIdMapper()
+        self._regex_mapper = ImpactsRegexToOpenIdMapper()
 
     def map(self, input_value: str, default_value: str | None) -> K | None:
         """Map the input value to the output value."""
         if is_valid_uuid(input_value):
             return self._uuid_mapper.map(input_value, default_value)
-        return self._keyword_mapper.map(input_value, default_value)
+        impact_name = self._keyword_mapper.map(input_value, None)
+        if not impact_name:
+            impact_name = self._regex_mapper.map(input_value, default_value)
+        return impact_name
 
 
 default_impacts_mapper = DefaultImpactsToOpenIdMapper()
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/mapping/indicators.py` & `ilcdlib-4.3.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-4.3.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/medium/archive.py` & `ilcdlib-4.3.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-4.3.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/reference_data.py` & `ilcdlib-4.3.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-4.3.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-4.3.0/src/ilcdlib/sanitizing/domain.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,15 +36,16 @@
         return url.removeprefix("www.")
 
 
 def cleanup_website(website: str | None) -> str | None:
     """
     Try to perform cleanup of the given website address.
 
-    If just domain name is given, add https:// and trailing slash.
+    If just domain name is given, add https:// and trailing slash. If there is a space, remove everything after it.
     """
     if website is None:
         return None
-    website = website.strip()
+    # Trim whitespace and remove any part after the first space
+    website = website.strip().partition(" ")[0]
     if not website.startswith("http"):
         return "https://" + website + "/"
     return website
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-4.3.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/sanitizing/text.py` & `ilcdlib-4.3.0/src/ilcdlib/sanitizing/text.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-4.3.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-4.3.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  Find out more at www.BuildingTransparency.org
 #
 from hashlib import sha1
 from io import BytesIO
 from typing import IO, Iterable, Type
 from urllib.parse import urlencode
 
-from requests import HTTPError, Response
+from requests import HTTPError, RequestException, Response
 
 from ilcdlib.dto import Category, IlcdReference, ListResponseMeta, ProcessBasicInfo, ProcessSearchResponse
 from ilcdlib.entity.category import CategorySystemReader
 from ilcdlib.http_common import BaseApiClient
 from ilcdlib.xml_parser import T_ET
 
 
@@ -86,44 +86,59 @@
             "get",
             f"/{self._urlencode(ref.entity_type)}/{self._urlencode(ref.entity_id)}/zipexport",
             params=params,
             stream=True,
         )
         return BytesIO(response.content)
 
-    def get_download_epd_document_link(self, process_uuid: str, version: str | None = None) -> str | None:
+    def _verify_url(self, url: str, http_method: str = "head") -> str | None:
+        """
+        Verify if the given URL exists (reachable from current host by given http method).
+
+        :return: URL if it exists, None otherwise
+        """
+        try:
+            self._do_request(http_method, url)
+        except RequestException:
+            return None
+        return url
+
+    def get_download_epd_document_link(
+        self, process_uuid: str, version: str | None = None, verify: bool = True
+    ) -> str | None:
         """
         Get link to download an EPD document (typically in PDF format).
 
         This method performs a check if the document exists and returns None if it doesn't.
 
         :param str process_uuid: UUID of the process
         :param str version: version of the process (optional)
+        :param verify: if True, the method will check if document behind url exists
         """
         params = dict()
         if version is not None:
             params["version"] = version
         url = f"{self.base_url}/processes/{self._urlencode(process_uuid)}/epd"
         if params:
             url += "?" + urlencode(params)
-        response = self._do_request("head", url, raise_for_status=False)
-        return url if response.ok else None
+        if verify:
+            return self._verify_url(url)
+        return url
 
     def get_entity_url(self, ref: IlcdReference, digital_file: str | None, verify: bool = False) -> str | None:
         """Get URL to download an ILCD entity or a digital file attached to it."""
         params = dict()
         if ref.entity_version is not None:
             params["version"] = ref.entity_version
         url = f"{self.base_url}/{ref.entity_type}/{self._urlencode(ref.entity_id)}"
         if digital_file is not None:
             url += f"/{self._urlencode(digital_file)}"
         url += "?" + urlencode(params)
         if verify:
-            response = self._do_request("head", url, raise_for_status=False)
-            return url if response.ok else None
+            return self._verify_url(url)
         return url
 
     def download_epd_document(self, process_uuid: str, version: str | None = None) -> IO[bytes]:
         """
         Download an EPD document (typically in PDF format).
 
         :param str process_uuid: UUID of the process
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/soda4lca/api_client_4x.py` & `ilcdlib-4.3.0/src/ilcdlib/soda4lca/api_client_4x.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         :param str category_system: category system
         :param str data_type: type of dataset
         :param str lang: language
         """
         xml_doc = self._do_xml_request(
             "get",
             "/processes/categories/",
-            params=dict(format="xml", lang=lang, catSystem="The International EPD System"),
+            params=dict(format="xml", lang=lang, catSystem=category_system),
         )
         reader = self.category_reader_cls(xml_doc)
         categories = reader.get_categories_flat_list_4x()
 
         result = categories.copy()
 
         for category in categories:
```

### Comparing `ilcdlib-4.2.0/src/ilcdlib/type.py` & `ilcdlib-4.3.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/src/ilcdlib/xml_parser.py` & `ilcdlib-4.3.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.2.0/PKG-INFO` & `ilcdlib-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 4.2.0
+Version: 4.3.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 4.2.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 4.3.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: open-source@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

