# Comparing `tmp/hubmap-api-py-client-0.0.7.tar.gz` & `tmp/hubmap-api-py-client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hubmap-api-py-client-0.0.7.tar", last modified: Mon May  3 20:21:40 2021, max compression
+gzip compressed data, was "dist/hubmap-api-py-client-0.0.9.tar", last modified: Tue May 25 13:19:50 2021, max compression
```

## Comparing `hubmap-api-py-client-0.0.7.tar` & `hubmap-api-py-client-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,48 @@
-drwxr-xr-x   0 jc         (501) staff       (20)        0 2021-05-03 20:21:40.000000 hubmap-api-py-client-0.0.7/
--rw-r--r--   0 jc         (501) staff       (20)     6199 2021-05-03 20:21:40.000000 hubmap-api-py-client-0.0.7/PKG-INFO
--rw-r--r--   0 jc         (501) staff       (20)     5106 2021-05-03 17:23:08.000000 hubmap-api-py-client-0.0.7/README.md
-drwxr-xr-x   0 jc         (501) staff       (20)        0 2021-05-03 20:21:40.000000 hubmap-api-py-client-0.0.7/hubmap_api_py_client/
--rw-r--r--   0 jc         (501) staff       (20)       81 2021-05-03 17:23:08.000000 hubmap-api-py-client-0.0.7/hubmap_api_py_client/__init__.py
--rw-r--r--   0 jc         (501) staff       (20)       39 2021-05-03 17:23:08.000000 hubmap-api-py-client-0.0.7/hubmap_api_py_client/errors.py
--rw-r--r--   0 jc         (501) staff       (20)    13256 2021-05-03 17:23:08.000000 hubmap-api-py-client-0.0.7/hubmap_api_py_client/external.py
--rw-r--r--   0 jc         (501) staff       (20)     4013 2021-05-03 17:23:08.000000 hubmap-api-py-client-0.0.7/hubmap_api_py_client/internal.py
-drwxr-xr-x   0 jc         (501) staff       (20)        0 2021-05-03 20:21:40.000000 hubmap-api-py-client-0.0.7/hubmap_api_py_client.egg-info/
--rw-r--r--   0 jc         (501) staff       (20)     6199 2021-05-03 20:21:40.000000 hubmap-api-py-client-0.0.7/hubmap_api_py_client.egg-info/PKG-INFO
--rw-r--r--   0 jc         (501) staff       (20)      377 2021-05-03 20:21:40.000000 hubmap-api-py-client-0.0.7/hubmap_api_py_client.egg-info/SOURCES.txt
--rw-r--r--   0 jc         (501) staff       (20)        1 2021-05-03 20:21:40.000000 hubmap-api-py-client-0.0.7/hubmap_api_py_client.egg-info/dependency_links.txt
--rw-r--r--   0 jc         (501) staff       (20)       16 2021-05-03 20:21:40.000000 hubmap-api-py-client-0.0.7/hubmap_api_py_client.egg-info/requires.txt
--rw-r--r--   0 jc         (501) staff       (20)       21 2021-05-03 20:21:40.000000 hubmap-api-py-client-0.0.7/hubmap_api_py_client.egg-info/top_level.txt
--rw-r--r--   0 jc         (501) staff       (20)      102 2021-05-03 20:21:40.000000 hubmap-api-py-client-0.0.7/setup.cfg
--rw-r--r--   0 jc         (501) staff       (20)      960 2021-05-03 17:23:08.000000 hubmap-api-py-client-0.0.7/setup.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/.github/
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 sean      (1000) sean      (1000)       91 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/.github/ISSUE_TEMPLATE/bug.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)      107 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)      112 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/.github/ISSUE_TEMPLATE/question.md
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/.github/workflows/
+-rw-rw-r--   0 sean      (1000) sean      (1000)      643 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/.github/workflows/ci.yml
+-rw-rw-r--   0 sean      (1000) sean      (1000)      145 2021-05-06 21:16:15.000000 hubmap-api-py-client-0.0.9/.gitignore
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1780 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/CHANGELOG.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1074 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/LICENSE
+-rw-rw-r--   0 sean      (1000) sean      (1000)     6264 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/PKG-INFO
+-rw-rw-r--   0 sean      (1000) sean      (1000)     7433 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/README-Client.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)      254 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/README-contrib.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)      919 2021-05-06 21:16:15.000000 hubmap-api-py-client-0.0.9/README-external.ResultsList.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1267 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/README-external.ResultsSet.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)     5163 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/README.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)        6 2021-05-25 13:19:49.000000 hubmap-api-py-client-0.0.9/VERSION
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/examples/
+-rw-rw-r--   0 sean      (1000) sean      (1000)      934 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/examples/differential-expression.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1054 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/examples/error-handling.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)      858 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/examples/repr.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)      955 2021-05-06 21:16:15.000000 hubmap-api-py-client-0.0.9/examples/results-list-iterator.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1891 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/examples/select_cells.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1061 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/examples/select_clusters.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1369 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/examples/select_datasets.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1070 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/examples/select_genes.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)      878 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/examples/select_organs.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)      284 2021-04-22 17:12:11.000000 hubmap-api-py-client-0.0.9/examples/select_proteins.md
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1338 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/examples/set-operations.md
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/hubmap_api_py_client/
+-rw-rw-r--   0 sean      (1000) sean      (1000)       81 2021-05-06 12:55:12.000000 hubmap-api-py-client-0.0.9/hubmap_api_py_client/__init__.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)       39 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/hubmap_api_py_client/errors.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)    14014 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/hubmap_api_py_client/external.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     4116 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/hubmap_api_py_client/internal.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/hubmap_api_py_client.egg-info/
+-rw-rw-r--   0 sean      (1000) sean      (1000)     6264 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/hubmap_api_py_client.egg-info/PKG-INFO
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1031 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/hubmap_api_py_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)        1 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/hubmap_api_py_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)       16 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/hubmap_api_py_client.egg-info/requires.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)       21 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/hubmap_api_py_client.egg-info/top_level.txt
+-rwxrwxr-x   0 sean      (1000) sean      (1000)      607 2021-04-22 17:12:11.000000 hubmap-api-py-client-0.0.9/publish.sh
+-rw-rw-r--   0 sean      (1000) sean      (1000)       77 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/requirements-dev.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)      113 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/requirements-lower-bound.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)      131 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/requirements.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)      102 2021-05-25 13:19:50.000000 hubmap-api-py-client-0.0.9/setup.cfg
+-rw-rw-r--   0 sean      (1000) sean      (1000)      960 2021-03-17 03:25:34.000000 hubmap-api-py-client-0.0.9/setup.py
+-rwxrwxr-x   0 sean      (1000) sean      (1000)     1192 2021-05-25 13:04:32.000000 hubmap-api-py-client-0.0.9/test.sh
```

### Comparing `hubmap-api-py-client-0.0.7/PKG-INFO` & `hubmap-api-py-client-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubmap-api-py-client
-Version: 0.0.7
+Version: 0.0.9
 Summary: Client for the HuBMAP Cells API
 Home-page: https://github.com/hubmapconsortium/hubmap-api-py-client
 Author: Chuck McCallum
 Author-email: mccallucc+cells_client@gmail.com
 License: UNKNOWN
 Description: # hubmap-api-py-client
         [![PyPI version](https://badge.fury.io/py/hubmap-api-py-client.svg)](https://pypi.org/project/hubmap-api-py-client/)
@@ -29,37 +29,38 @@
         >>> from os import environ
         >>> from hubmap_api_py_client import Client
         >>> client = Client(environ['API_ENDPOINT'])
         
         >>> [m for m in dir(client) if m.startswith('select_')]
         ['select_cells', 'select_clusters', 'select_datasets', 'select_genes', 'select_organs', 'select_proteins']
         
-        >>> cells_with_vim = client.select_cells(where='gene', has=['VIM > 0.5'], genomic_modality='rna')
-        >>> assert len(cells_with_vim) > 0
+        >>> gene_symbol = client.select_genes().get_list()[0]['gene_symbol']
+        >>> cells_with_gene = client.select_cells(where='gene', has=[f'{gene_symbol} > 0.5'], genomic_modality='rna')
+        >>> assert len(cells_with_gene) > 0
         
         # Select cells from the datasets with the following UUIDs:
-        >>> dataset_a_uuid = '68159e4bd6a2cea1cd66e8f3050cfcb7'
-        >>> dataset_b_uuid = 'e8d642084fc5ec8b5d348ebab96a4b22'
+        >>> dataset_a_uuid = client.select_datasets().get_list()[0]['uuid']
+        >>> dataset_b_uuid = client.select_datasets().get_list()[1]['uuid']
         >>> cells_in_a_len = len(client.select_cells(where='dataset', has=[dataset_a_uuid]))
         >>> cells_in_b_len = len(client.select_cells(where='dataset', has=[dataset_b_uuid]))
         >>> cells_in_datasets = client.select_cells(where='dataset', has=[dataset_a_uuid, dataset_b_uuid])
         >>> cells_in_datasets_len = len(cells_in_datasets)
         >>> assert cells_in_datasets_len > 0
         >>> assert cells_in_datasets_len == cells_in_a_len + cells_in_b_len
         
         # Combine criteria with intersection:
-        >>> cells_with_vim_in_datasets = cells_with_vim & cells_in_datasets
-        >>> assert len(cells_with_vim_in_datasets) > 10
+        >>> cells_with_gene_in_datasets = cells_with_gene & cells_in_datasets
+        >>> assert len(cells_with_gene_in_datasets) > 0
         
         # Get a list; should run quickly:
-        >>> cell_list = cells_with_vim_in_datasets.get_list()
+        >>> cell_list = cells_with_gene_in_datasets.get_list()
         
         >>> cells = cell_list[0:10]
-        >>> assert len(cells) == 10
-        >>> assert cells[0].keys() == {'cell_id', 'modality', 'dataset', 'organ', 'clusters', 'protein_mean', 'protein_total', 'protein_covar'}
+        >>> assert len(cells) > 0
+        >>> assert cells[0].keys() == {'cell_id', 'modality', 'dataset', 'organ', 'clusters'}
         
         ```
         
         More documentation:
         - [Examples](https://github.com/hubmapconsortium/hubmap-api-py-client/blob/main/examples/)
         - [`Client` pydoc](https://github.com/hubmapconsortium/hubmap-api-py-client/blob/main/README-Client.txt)
         - [`ResultsSet` pydoc](https://github.com/hubmapconsortium/hubmap-api-py-client/blob/main/README-external.ResultsSet.txt)
```

### Comparing `hubmap-api-py-client-0.0.7/README.md` & `hubmap-api-py-client-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,37 +21,38 @@
 >>> from os import environ
 >>> from hubmap_api_py_client import Client
 >>> client = Client(environ['API_ENDPOINT'])
 
 >>> [m for m in dir(client) if m.startswith('select_')]
 ['select_cells', 'select_clusters', 'select_datasets', 'select_genes', 'select_organs', 'select_proteins']
 
->>> cells_with_vim = client.select_cells(where='gene', has=['VIM > 0.5'], genomic_modality='rna')
->>> assert len(cells_with_vim) > 0
+>>> gene_symbol = client.select_genes().get_list()[0]['gene_symbol']
+>>> cells_with_gene = client.select_cells(where='gene', has=[f'{gene_symbol} > 0.5'], genomic_modality='rna')
+>>> assert len(cells_with_gene) > 0
 
 # Select cells from the datasets with the following UUIDs:
->>> dataset_a_uuid = '68159e4bd6a2cea1cd66e8f3050cfcb7'
->>> dataset_b_uuid = 'e8d642084fc5ec8b5d348ebab96a4b22'
+>>> dataset_a_uuid = client.select_datasets().get_list()[0]['uuid']
+>>> dataset_b_uuid = client.select_datasets().get_list()[1]['uuid']
 >>> cells_in_a_len = len(client.select_cells(where='dataset', has=[dataset_a_uuid]))
 >>> cells_in_b_len = len(client.select_cells(where='dataset', has=[dataset_b_uuid]))
 >>> cells_in_datasets = client.select_cells(where='dataset', has=[dataset_a_uuid, dataset_b_uuid])
 >>> cells_in_datasets_len = len(cells_in_datasets)
 >>> assert cells_in_datasets_len > 0
 >>> assert cells_in_datasets_len == cells_in_a_len + cells_in_b_len
 
 # Combine criteria with intersection:
->>> cells_with_vim_in_datasets = cells_with_vim & cells_in_datasets
->>> assert len(cells_with_vim_in_datasets) > 10
+>>> cells_with_gene_in_datasets = cells_with_gene & cells_in_datasets
+>>> assert len(cells_with_gene_in_datasets) > 0
 
 # Get a list; should run quickly:
->>> cell_list = cells_with_vim_in_datasets.get_list()
+>>> cell_list = cells_with_gene_in_datasets.get_list()
 
 >>> cells = cell_list[0:10]
->>> assert len(cells) == 10
->>> assert cells[0].keys() == {'cell_id', 'modality', 'dataset', 'organ', 'clusters', 'protein_mean', 'protein_total', 'protein_covar'}
+>>> assert len(cells) > 0
+>>> assert cells[0].keys() == {'cell_id', 'modality', 'dataset', 'organ', 'clusters'}
 
 ```
 
 More documentation:
 - [Examples](https://github.com/hubmapconsortium/hubmap-api-py-client/blob/main/examples/)
 - [`Client` pydoc](https://github.com/hubmapconsortium/hubmap-api-py-client/blob/main/README-Client.txt)
 - [`ResultsSet` pydoc](https://github.com/hubmapconsortium/hubmap-api-py-client/blob/main/README-external.ResultsSet.txt)
```

### Comparing `hubmap-api-py-client-0.0.7/hubmap_api_py_client/external.py` & `hubmap-api-py-client-0.0.9/hubmap_api_py_client/external.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
     def __repr__(self):
         return f'<Client base_url={self.client.base_url}>'
 
     def _query(
             self,
             input_type=None, output_type=None, has=None,
-            genomic_modality=None, p_value=None, logical_operator=None,
+            genomic_modality=None, p_value=None, logical_operator=None, min_cell_percentage=None,
             ResultsSetSubclass=None):
         if not isinstance(has, list) and input_type is not None:
             raise TypeError(f'"has" parameter must be a list, not {has}')
         handle = self.client.hubmap_query(input_type, output_type, has, genomic_modality,
-                                          p_value, logical_operator)
+                                          p_value, logical_operator, min_cell_percentage)
         return ResultsSetSubclass(
             self.client, handle,
             input_type=input_type, output_type=output_type,
             query=has
         )
 
 
@@ -198,14 +198,21 @@
         genomic_modality=None,
         logical_operator=None:
         self._query(
             input_type=where, output_type=output_type, has=has,
             genomic_modality=genomic_modality,
             logical_operator=logical_operator,
             ResultsSetSubclass=ResultsSetSubclass),
+        'min_cells': lambda self, where=None, has=None,
+            genomic_modality=None, logical_operator=None, min_cell_percentage=None:
+        self._query(
+            input_type=where, output_type=output_type, has=has,
+            genomic_modality=genomic_modality,
+            min_cell_percentage=min_cell_percentage,
+            ResultsSetSubclass=ResultsSetSubclass),
         'where_has': lambda self, where=None, has=None:
         self._query(
             input_type=where, output_type=output_type, has=has,
             ResultsSetSubclass=ResultsSetSubclass),
     }
     method = lambda_lookup[args_type]
     method.__doc__ = doc
@@ -300,25 +307,28 @@
                 more than one element. Must be one of ["and", "or"].
 
         Returns:
             ResultsSet
         '''
     ),
     'dataset': (
-        'where_has',
+        'min_cells',
         '''
         Select a set of datasets. If no params are provided, selects the set of all datasets.
         Otherwise, selects a set of datasets filtered based on parameters supplied.
 
         Args:
             where (str): The type of entity for which identifiers are supplied as input to query.
                 Must be one of ["dataset", "cell", "cluster"].
-            has (List[str]): A list of entity identifiers (dataset_uuids, etc) supplied as input to
-                the query.
-
+            has (List[str]): A list of entity identifiers or expressions (dataset_uuids, etc) supplied as
+                input to the query.
+            genomic_modality (str): Modality to consider in quantitative queries.
+                Required for queries in which "where" is "gene". Must be one of ["rna", "atac"].
+            min_cell_percentage (float): Minimum percentage of cells which must satisfy the quantitative
+                expression in "has"
         Returns:
             ResultsSet
         ''',
     ),
     'protein': (
         'where_has',
         '''
```

### Comparing `hubmap-api-py-client-0.0.7/hubmap_api_py_client/internal.py` & `hubmap-api-py-client-0.0.9/hubmap_api_py_client/internal.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 class InternalClient():
     def __init__(self, base_url):
         self.base_url = base_url
 
     def hubmap_query(
             self,
             input_type: str, output_type: str, input_set: List[str],
-            genomic_modality: str = None, p_value: float = None, logical_operator: str = None):
+            genomic_modality: str = None, p_value: float = None, logical_operator: str = None,
+            min_cell_percentage: float = None):
         '''
         This function takes query parameters and returns a query set token.
         '''
         request_url = self.base_url + output_type + "/"
         request_dict = {
             'input_type': input_type,
             'input_set': input_set,
             'genomic_modality': genomic_modality,
             'p_value': p_value,
-            'logical_operator': logical_operator
+            'logical_operator': logical_operator,
+            'min_cell_percentage': min_cell_percentage
         }
         return self._post_and_get_handle(request_url, request_dict)
 
     # These functions take two query set tokens and return an API token:
 
     def set_intersection(
             self, set_key_one: str, set_key_two: str, set_type: str) -> str:
```

### Comparing `hubmap-api-py-client-0.0.7/hubmap_api_py_client.egg-info/PKG-INFO` & `hubmap-api-py-client-0.0.9/hubmap_api_py_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubmap-api-py-client
-Version: 0.0.7
+Version: 0.0.9
 Summary: Client for the HuBMAP Cells API
 Home-page: https://github.com/hubmapconsortium/hubmap-api-py-client
 Author: Chuck McCallum
 Author-email: mccallucc+cells_client@gmail.com
 License: UNKNOWN
 Description: # hubmap-api-py-client
         [![PyPI version](https://badge.fury.io/py/hubmap-api-py-client.svg)](https://pypi.org/project/hubmap-api-py-client/)
@@ -29,37 +29,38 @@
         >>> from os import environ
         >>> from hubmap_api_py_client import Client
         >>> client = Client(environ['API_ENDPOINT'])
         
         >>> [m for m in dir(client) if m.startswith('select_')]
         ['select_cells', 'select_clusters', 'select_datasets', 'select_genes', 'select_organs', 'select_proteins']
         
-        >>> cells_with_vim = client.select_cells(where='gene', has=['VIM > 0.5'], genomic_modality='rna')
-        >>> assert len(cells_with_vim) > 0
+        >>> gene_symbol = client.select_genes().get_list()[0]['gene_symbol']
+        >>> cells_with_gene = client.select_cells(where='gene', has=[f'{gene_symbol} > 0.5'], genomic_modality='rna')
+        >>> assert len(cells_with_gene) > 0
         
         # Select cells from the datasets with the following UUIDs:
-        >>> dataset_a_uuid = '68159e4bd6a2cea1cd66e8f3050cfcb7'
-        >>> dataset_b_uuid = 'e8d642084fc5ec8b5d348ebab96a4b22'
+        >>> dataset_a_uuid = client.select_datasets().get_list()[0]['uuid']
+        >>> dataset_b_uuid = client.select_datasets().get_list()[1]['uuid']
         >>> cells_in_a_len = len(client.select_cells(where='dataset', has=[dataset_a_uuid]))
         >>> cells_in_b_len = len(client.select_cells(where='dataset', has=[dataset_b_uuid]))
         >>> cells_in_datasets = client.select_cells(where='dataset', has=[dataset_a_uuid, dataset_b_uuid])
         >>> cells_in_datasets_len = len(cells_in_datasets)
         >>> assert cells_in_datasets_len > 0
         >>> assert cells_in_datasets_len == cells_in_a_len + cells_in_b_len
         
         # Combine criteria with intersection:
-        >>> cells_with_vim_in_datasets = cells_with_vim & cells_in_datasets
-        >>> assert len(cells_with_vim_in_datasets) > 10
+        >>> cells_with_gene_in_datasets = cells_with_gene & cells_in_datasets
+        >>> assert len(cells_with_gene_in_datasets) > 0
         
         # Get a list; should run quickly:
-        >>> cell_list = cells_with_vim_in_datasets.get_list()
+        >>> cell_list = cells_with_gene_in_datasets.get_list()
         
         >>> cells = cell_list[0:10]
-        >>> assert len(cells) == 10
-        >>> assert cells[0].keys() == {'cell_id', 'modality', 'dataset', 'organ', 'clusters', 'protein_mean', 'protein_total', 'protein_covar'}
+        >>> assert len(cells) > 0
+        >>> assert cells[0].keys() == {'cell_id', 'modality', 'dataset', 'organ', 'clusters'}
         
         ```
         
         More documentation:
         - [Examples](https://github.com/hubmapconsortium/hubmap-api-py-client/blob/main/examples/)
         - [`Client` pydoc](https://github.com/hubmapconsortium/hubmap-api-py-client/blob/main/README-Client.txt)
         - [`ResultsSet` pydoc](https://github.com/hubmapconsortium/hubmap-api-py-client/blob/main/README-external.ResultsSet.txt)
```

### Comparing `hubmap-api-py-client-0.0.7/setup.py` & `hubmap-api-py-client-0.0.9/setup.py`

 * *Files identical despite different names*

