# Comparing `tmp/iderare-pheno-0.5.0.tar.gz` & `tmp/iderare_pheno-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iderare-pheno-0.5.0.tar", last modified: Wed Apr 10 10:18:15 2024, max compression
+gzip compressed data, was "iderare_pheno-0.6.2.tar", last modified: Wed May  1 16:38:40 2024, max compression
```

## Comparing `iderare-pheno-0.5.0.tar` & `iderare_pheno-0.6.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.531985 iderare-pheno-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-10 10:18:15.531985 iderare-pheno-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.439985 iderare-pheno-0.5.0/iderare_pheno/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.435985 iderare-pheno-0.5.0/iderare_pheno/phenotype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.475985 iderare-pheno-0.5.0/iderare_pheno/phenotype/data/
--rw-r--r--   0 runner    (1001) docker     (127) 19051578 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/data/genes_to_phenotype.txt
--rw-r--r--   0 runner    (1001) docker     (127)  9995624 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/data/hp.obo
--rw-r--r--   0 runner    (1001) docker     (127) 31896677 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/data/phenotype.hpoa
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.527985 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/
--rw-r--r--   0 runner    (1001) docker     (127)   196778 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/icd102omim_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   224561 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv
--rw-r--r--   0 runner    (1001) docker     (127)  6033462 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)  7205315 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   218406 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   232073 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)  1298790 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/simrec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/streamlit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.531985 iderare-pheno-0.5.0/iderare_pheno/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/templates/template_iderare.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/iderare_pheno/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:15.531985 iderare-pheno-0.5.0/iderare_pheno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-10 10:18:15.000000 iderare-pheno-0.5.0/iderare_pheno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-10 10:18:15.000000 iderare-pheno-0.5.0/iderare_pheno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:18:15.000000 iderare-pheno-0.5.0/iderare_pheno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-10 10:18:15.000000 iderare-pheno-0.5.0/iderare_pheno.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 10:18:15.000000 iderare-pheno-0.5.0/iderare_pheno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-10 10:17:53.000000 iderare-pheno-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:18:15.531985 iderare-pheno-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:38:39.998533 iderare_pheno-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-01 16:38:21.000000 iderare_pheno-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11599 2024-05-01 16:38:39.998533 iderare_pheno-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-05-01 16:38:21.000000 iderare_pheno-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:38:39.906533 iderare_pheno-0.6.2/iderare_pheno/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 16:38:21.000000 iderare_pheno-0.6.2/iderare_pheno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-01 16:38:21.000000 iderare_pheno-0.6.2/iderare_pheno/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-01 16:38:21.000000 iderare_pheno-0.6.2/iderare_pheno/fhir_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:38:39.902533 iderare_pheno-0.6.2/iderare_pheno/phenotype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:38:39.942533 iderare_pheno-0.6.2/iderare_pheno/phenotype/data/
+-rw-r--r--   0 runner    (1001) docker     (127) 19051578 2024-05-01 16:38:21.000000 iderare_pheno-0.6.2/iderare_pheno/phenotype/data/genes_to_phenotype.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  9995624 2024-05-01 16:38:21.000000 iderare_pheno-0.6.2/iderare_pheno/phenotype/data/hp.obo
+-rw-r--r--   0 runner    (1001) docker     (127) 31896677 2024-05-01 16:38:21.000000 iderare_pheno-0.6.2/iderare_pheno/phenotype/data/phenotype.hpoa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:38:39.994533 iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/
+-rw-r--r--   0 runner    (1001) docker     (127)   196778 2024-05-01 16:38:21.000000 iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/icd102omim_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   224561 2024-05-01 16:38:21.000000 iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  6033462 2024-05-01 16:38:21.000000 iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  7205315 2024-05-01 16:38:22.000000 iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   218406 2024-05-01 16:38:22.000000 iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   232073 2024-05-01 16:38:22.000000 iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  1298790 2024-05-01 16:38:22.000000 iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:38:22.000000 iderare_pheno-0.6.2/iderare_pheno/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-01 16:38:22.000000 iderare_pheno-0.6.2/iderare_pheno/simrec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-01 16:38:22.000000 iderare_pheno-0.6.2/iderare_pheno/streamlit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:38:39.994533 iderare_pheno-0.6.2/iderare_pheno/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-01 16:38:22.000000 iderare_pheno-0.6.2/iderare_pheno/templates/template_iderare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-01 16:38:22.000000 iderare_pheno-0.6.2/iderare_pheno/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-01 16:38:22.000000 iderare_pheno-0.6.2/iderare_pheno/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:38:39.998533 iderare_pheno-0.6.2/iderare_pheno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11599 2024-05-01 16:38:39.000000 iderare_pheno-0.6.2/iderare_pheno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-01 16:38:39.000000 iderare_pheno-0.6.2/iderare_pheno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:38:39.000000 iderare_pheno-0.6.2/iderare_pheno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-01 16:38:39.000000 iderare_pheno-0.6.2/iderare_pheno.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 16:38:39.000000 iderare_pheno-0.6.2/iderare_pheno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-01 16:38:22.000000 iderare_pheno-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:38:39.998533 iderare_pheno-0.6.2/setup.cfg
```

### Comparing `iderare-pheno-0.5.0/LICENSE` & `iderare_pheno-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/PKG-INFO` & `iderare_pheno-0.6.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.5.0
+Version: 0.6.2
 Author-email: Ivan William Harsono <ivanwilliam.md@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -48,46 +48,46 @@
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: hpo3
 Requires-Dist: scikit-learn
 Requires-Dist: pyyaml
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
-Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
+Requires-Dist: mypy<1.11,>=1.0; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
-Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev"
-Requires-Dist: furo==2024.1.29; extra == "dev"
+Requires-Dist: Sphinx<7.4.0,>=4.3.0; extra == "dev"
+Requires-Dist: furo==2024.4.27; extra == "dev"
 Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==1.23.3; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 
-# [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/)
+# [IDeRare-Pheno](https://pypi.org/project/iderare_pheno/)
 
 <p align="center">
     <a href="https://github.com/ivanwilliammd/iderare-pheno/actions">
         <img alt="CI" src="https://github.com/ivanwilliammd/iderare-pheno/workflows/Main/badge.svg">
     </a>
     <a href="https://pypi.org/project/iderare_pheno/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/iderare_pheno">
     </a>
-    <a href="https://iderare-pheno.readthedocs.io/en/latest/?badge=latest">
+<!--     <a href="https://iderare-pheno.readthedocs.io/en/latest/?badge=latest">
         <img src="https://readthedocs.org/projects/iderare-pheno/badge/?version=latest" alt="Documentation Status" />
-    </a>
+    </a> -->
     <a href="https://github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/github/license/ivanwilliammd/iderare-pheno.svg?color=blue&cachedrop">
     </a>
     <a href="https://bioinformatics-ivanwilliamharsono.streamlit.app/IDeRare_Pheno">
         <img alt="Streamlit" src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg">
     <br/>
 </p>
@@ -108,21 +108,20 @@
 <sup>g</sup>Bioinformatics Core Facilities - IMERI, Faculty of Medicine, Universitas Indonesia, Jalan Salemba Raya number 6, Jakarta, 10430, Indonesia .<br>
 <sup>h</sup>Department of Child Health, Dr. Cipto Mangunkusumo Hospital, Faculty of Medicine, University of Indonesia, Jakarta, Indonesia. <br>
 
 
 **Note:** Currently IDeRare paper is being considered journal submission. The citation will be updated once the paper is published.
 
 ## Quick links
-
-- [Documentation](https://iderare-pheno.readthedocs.io/)
+- [IDeRare full pipeline - Phenotype and Genotype](https://github.com/ivanwilliammd/IDeRare)
 - [PyPI Package](https://pypi.org/project/iderare-pheno/)
 - [License](https://github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE)
 - [Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb)
 - Interactive Webapps Implementation of at [Streamlit](https://bioinformatics-ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno)
-
+<!-- - [Documentation](https://iderare-pheno.readthedocs.io/) -->
 
 ## What does it do?
 
 This script is recommended if you would like to do conversion, linkage analysis, similarity scoring, and gene-disease recommendation based on the phenotype data provided at [clinical_data.txt](clinical_data.txt). Full feature : 
 1. Convert the phenotype data to HPO code (accept mixed SNOMED, LOINC, and HPO code)
 2. Similarity scoring of differential diagnosis
 3. Linkage analysis of differential diagnosis (accept mixed SNOMED, ICD-10, ORPHA, OMIM code), include dendrogram tree visualization.
@@ -172,18 +171,68 @@
 
 <!-- end install source -->
 
 ## Importing the library
 
 ```python
 from iderare_pheno.converter import term2omim, term2orpha, term2hpo, batchconvert
-from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation, hpo2name
+from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation, hpo2name, omim2name
 from iderare_pheno.utils import linkage_dendrogram, list2tsv, generate_yml
 ```
-As the complete readthedocs.io is still ongoing, please kindly refer to this [Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb)
+As the complete readthedocs.io is being finalized, please kindly refer to this [Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb)
+
+Note : for Streamlit implementation, use ```iderare_pheno.streamlit_utils``` instead of ```iderare_pheno.utils```, this was done to prevent file to automatically saving and showing dendrogram in Streamlit.
+```python
+from iderare_pheno.streamlit_utils import linkage_dendrogram, list2tsv, generate_yml
+```
+
+For Python FastAPI implementation and FHIR code extraction / parsing and deploying wsgi app, ensure you have installed the dependencies below:
+```bash
+pip install fastapi uvicorn a2wsgi
+```
+
+Then prepare your passenger wsgi app and main FastAPI app as below:
+
+#### passenger_wsgi.py
+```python
+import os
+import sys
+from a2wsgi import ASGIMiddleware
+
+# Adjust the path to your FastAPI application directory if needed
+app_dir = os.path.join(os.path.dirname(__file__), 'app')
+sys.path.insert(0, app_dir)
+
+# Import your FastAPI application
+from app.main import app  # Assuming your FastAPI app instance is named 'app'
+
+# Application callable for Passenger WSGI
+def application(environ, start_response):
+    return ASGIMiddleware(app)(environ, start_response)
+```
+
+#### app/main.py
+```python
+from fastapi.responses import RedirectResponse
+from iderare_pheno.fhir_parser import *
+
+@app.get("/")
+async def welcome():
+    return RedirectResponse(status_code=302, url="/docs")
+
+@app.get("/health")
+async def health() -> Response :
+    return {"status_code" : 200, "detail" : "The services is running, try to explore the API from Postman Collection"}
+
+if __name__ == "__main__":
+    import uvicorn
+    uvicorn.run(app, host="0.0.0.0", port=8000)
+```
+
+Now you could access your http://localhost:8000 and redirected to Swagger to see the documentation of the available FastAPI endpoint. Demo example could be accessed via Postman Collection at [here](https://www.postman.com/ivanwilliamharsono/workspace/iderare-pheno/overview)
 
 
 ## Team
 
 <!-- start team -->
 
 **iderare-pheno** is developed and maintained by the author(s), To learn more about who specifically contributed to this codebase, see [our contributors](https://github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.5.0 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.6.2 Author-email: Ivan
 William Harsono
 gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ivan William
 Harsono Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -27,28 +27,28 @@
 Audience :: Science/Research Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering
 :: Medical Science Apps. Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pandas Requires-Dist: numpy
 Requires-Dist: matplotlib Requires-Dist: scipy Requires-Dist: hpo3 Requires-
 Dist: scikit-learn Requires-Dist: pyyaml Provides-Extra: dev Requires-Dist:
-ruff; extra == "dev" Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-
+ruff; extra == "dev" Requires-Dist: mypy<1.11,>=1.0; extra == "dev" Requires-
 Dist: types-PyYAML; extra == "dev" Requires-Dist: black<25.0,>=23.0; extra ==
 "dev" Requires-Dist: black[jupyter]; extra == "dev" Requires-Dist:
 isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-cov; extra
 == "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist: build;
 extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist: wheel;
-extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-
-Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-parser<2.1,>=1.0;
+extra == "dev" Requires-Dist: Sphinx<7.4.0,>=4.3.0; extra == "dev" Requires-
+Dist: furo==2024.4.27; extra == "dev" Requires-Dist: myst-parser<2.1,>=1.0;
 extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev" Requires-Dist:
 sphinx-autodoc-typehints==1.23.3; extra == "dev" Requires-Dist: packaging;
-extra == "dev" # [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/)
-             _[_C_I_]_[_P_y_P_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_S_t_r_e_a_m_l_i_t_]
+extra == "dev" # [IDeRare-Pheno](https://pypi.org/project/iderare_pheno/)
+                        _[_C_I_]_[_P_y_P_I_]_[_L_i_c_e_n_s_e_]_[_S_t_r_e_a_m_l_i_t_]
 IDeRare or "Indonesia Exome Rare Disease Variant Discovery Pipeline" is a
 simple and ready to use variant discovery pipeline to discover rare disease
 variants from exome sequencing data. This repository is **the first part** of
 IDeRare workflow for **phenotype analysis**. For complete pipeline for
 _**phenotype-genotype analysis**_, kindly refer to [IDeRare Github repository]
 (https://github.com/ivanwilliammd/IDeRare). ## Authored by Ivan William
 Harsonoa, Yulia Arianib, Beben Benyaminc,d,e, Fadilah Fadilahf,g, Dwi Ari
@@ -65,47 +65,72 @@
 fDepartment of Medical Chemistry, Faculty of Medicine, Universitas Indonesia,
 Jalan Salemba Raya number 4, Jakarta, 10430, Indonesia.
 gBioinformatics Core Facilities - IMERI, Faculty of Medicine, Universitas
 Indonesia, Jalan Salemba Raya number 6, Jakarta, 10430, Indonesia .
 hDepartment of Child Health, Dr. Cipto Mangunkusumo Hospital, Faculty of
 Medicine, University of Indonesia, Jakarta, Indonesia.
 **Note:** Currently IDeRare paper is being considered journal submission. The
-citation will be updated once the paper is published. ## Quick links -
-[Documentation](https://iderare-pheno.readthedocs.io/) - [PyPI Package](https:/
-/pypi.org/project/iderare-pheno/) - [License](https://github.com/ivanwilliammd/
-iderare-pheno/blob/main/LICENSE) - [Interactive Playbook Example](https://
-github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb) - Interactive
-Webapps Implementation of at [Streamlit](https://bioinformatics-
-ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno) ## What does it do? This
-script is recommended if you would like to do conversion, linkage analysis,
-similarity scoring, and gene-disease recommendation based on the phenotype data
-provided at [clinical_data.txt](clinical_data.txt). Full feature : 1. Convert
-the phenotype data to HPO code (accept mixed SNOMED, LOINC, and HPO code) 2.
-Similarity scoring of differential diagnosis 3. Linkage analysis of
-differential diagnosis (accept mixed SNOMED, ICD-10, ORPHA, OMIM code), include
-dendrogram tree visualization. - This should help clinician to **systematically
-doing work-up and excluding similar diagnosis together** based on the
-patient\'s phenotype. 4. Gene and disease recommendation based on the phenotype
-data similarity scoring between **phenotype** and OMIM gene and disease
-databank. 5. Linkage analysis of recommended causative gene and disease based
-on phenotype data (include dendrogram tree visualization). - This should help
-clinician to **explore / enrich their differential diagnosis** based on the
-patient\'s phenotype. 6. Example of the clinical data provided at [Clinical
-Information Example section](#clinical-information-example) ## Installation
-**iderare-pheno** requires Python 3.8 or later. ### Installing with `pip`
-**iderare-pheno** is available [on PyPI](https://pypi.org/project/iderare-
-pheno/). Just run ```bash pip install iderare-pheno ``` ### Installing from
-source To install **iderare-pheno** from source, first clone [the repository]
-(https://github.com/ivanwilliammd/iderare-pheno): ```bash git clone https://
-github.com/ivanwilliammd/iderare-pheno.git cd iderare_pheno ``` Then run
-```bash pip install -e . ``` ## Importing the library ```python from
+citation will be updated once the paper is published. ## Quick links - [IDeRare
+full pipeline - Phenotype and Genotype](https://github.com/ivanwilliammd/
+IDeRare) - [PyPI Package](https://pypi.org/project/iderare-pheno/) - [License]
+(https://github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE) -
+[Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/
+blob/main/Playbook.ipynb) - Interactive Webapps Implementation of at
+[Streamlit](https://bioinformatics-ivanwilliamharsono.streamlitapp.com/
+IDeRare_Pheno) ## What does it do? This script is recommended if you would like
+to do conversion, linkage analysis, similarity scoring, and gene-disease
+recommendation based on the phenotype data provided at [clinical_data.txt]
+(clinical_data.txt). Full feature : 1. Convert the phenotype data to HPO code
+(accept mixed SNOMED, LOINC, and HPO code) 2. Similarity scoring of
+differential diagnosis 3. Linkage analysis of differential diagnosis (accept
+mixed SNOMED, ICD-10, ORPHA, OMIM code), include dendrogram tree visualization.
+- This should help clinician to **systematically doing work-up and excluding
+similar diagnosis together** based on the patient\'s phenotype. 4. Gene and
+disease recommendation based on the phenotype data similarity scoring between
+**phenotype** and OMIM gene and disease databank. 5. Linkage analysis of
+recommended causative gene and disease based on phenotype data (include
+dendrogram tree visualization). - This should help clinician to **explore /
+enrich their differential diagnosis** based on the patient\'s phenotype. 6.
+Example of the clinical data provided at [Clinical Information Example section]
+(#clinical-information-example) ## Installation **iderare-pheno** requires
+Python 3.8 or later. ### Installing with `pip` **iderare-pheno** is available
+[on PyPI](https://pypi.org/project/iderare-pheno/). Just run ```bash pip
+install iderare-pheno ``` ### Installing from source To install **iderare-
+pheno** from source, first clone [the repository](https://github.com/
+ivanwilliammd/iderare-pheno): ```bash git clone https://github.com/
+ivanwilliammd/iderare-pheno.git cd iderare_pheno ``` Then run ```bash pip
+install -e . ``` ## Importing the library ```python from
 iderare_pheno.converter import term2omim, term2orpha, term2hpo, batchconvert
 from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation,
-hpo2name from iderare_pheno.utils import linkage_dendrogram, list2tsv,
-generate_yml ``` As the complete readthedocs.io is still ongoing, please kindly
-refer to this [Interactive Playbook Example](https://github.com/ivanwilliammd/
-iderare-pheno/blob/main/Playbook.ipynb) ## Team **iderare-pheno** is developed
-and maintained by the author(s), To learn more about who specifically
-contributed to this codebase, see [our contributors](https://github.com/
-ivanwilliammd/iderare-pheno/graphs/contributors) page. ## License **iderare-
-pheno** license is derived from [IDeRare](https://github.com/ivanwilliammd/
-iderare)
+hpo2name, omim2name from iderare_pheno.utils import linkage_dendrogram,
+list2tsv, generate_yml ``` As the complete readthedocs.io is being finalized,
+please kindly refer to this [Interactive Playbook Example](https://github.com/
+ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb) Note : for Streamlit
+implementation, use ```iderare_pheno.streamlit_utils``` instead of
+```iderare_pheno.utils```, this was done to prevent file to automatically
+saving and showing dendrogram in Streamlit. ```python from
+iderare_pheno.streamlit_utils import linkage_dendrogram, list2tsv, generate_yml
+``` For Python FastAPI implementation and FHIR code extraction / parsing and
+deploying wsgi app, ensure you have installed the dependencies below: ```bash
+pip install fastapi uvicorn a2wsgi ``` Then prepare your passenger wsgi app and
+main FastAPI app as below: #### passenger_wsgi.py ```python import os import
+sys from a2wsgi import ASGIMiddleware # Adjust the path to your FastAPI
+application directory if needed app_dir = os.path.join(os.path.dirname
+(__file__), 'app') sys.path.insert(0, app_dir) # Import your FastAPI
+application from app.main import app # Assuming your FastAPI app instance is
+named 'app' # Application callable for Passenger WSGI def application(environ,
+start_response): return ASGIMiddleware(app)(environ, start_response) ``` ####
+app/main.py ```python from fastapi.responses import RedirectResponse from
+iderare_pheno.fhir_parser import * @app.get("/") async def welcome(): return
+RedirectResponse(status_code=302, url="/docs") @app.get("/health") async def
+health() -> Response : return {"status_code" : 200, "detail" : "The services is
+running, try to explore the API from Postman Collection"} if __name__ ==
+"__main__": import uvicorn uvicorn.run(app, host="0.0.0.0", port=8000) ``` Now
+you could access your http://localhost:8000 and redirected to Swagger to see
+the documentation of the available FastAPI endpoint. Demo example could be
+accessed via Postman Collection at [here](https://www.postman.com/
+ivanwilliamharsono/workspace/iderare-pheno/overview) ## Team **iderare-pheno**
+is developed and maintained by the author(s), To learn more about who
+specifically contributed to this codebase, see [our contributors](https://
+github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page. ## License
+**iderare-pheno** license is derived from [IDeRare](https://github.com/
+ivanwilliammd/iderare)
```

### Comparing `iderare-pheno-0.5.0/README.md` & `iderare_pheno-0.6.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,377 +1,498 @@
 00000000: 2320 5b49 4465 5261 7265 2d50 6865 6e6f  # [IDeRare-Pheno
-00000010: 5d28 6874 7470 733a 2f2f 6964 6572 6172  ](https://iderar
-00000020: 652d 7068 656e 6f2e 7265 6164 7468 6564  e-pheno.readthed
-00000030: 6f63 732e 696f 2f29 0a0a 3c70 2061 6c69  ocs.io/)..<p ali
-00000040: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
-00000050: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000060: 2f2f 6769 7468 7562 2e63 6f6d 2f69 7661  //github.com/iva
-00000070: 6e77 696c 6c69 616d 6d64 2f69 6465 7261  nwilliammd/idera
-00000080: 7265 2d70 6865 6e6f 2f61 6374 696f 6e73  re-pheno/actions
-00000090: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
-000000a0: 616c 743d 2243 4922 2073 7263 3d22 6874  alt="CI" src="ht
-000000b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000000c0: 2f69 7661 6e77 696c 6c69 616d 6d64 2f69  /ivanwilliammd/i
-000000d0: 6465 7261 7265 2d70 6865 6e6f 2f77 6f72  derare-pheno/wor
-000000e0: 6b66 6c6f 7773 2f4d 6169 6e2f 6261 6467  kflows/Main/badg
-000000f0: 652e 7376 6722 3e0a 2020 2020 3c2f 613e  e.svg">.    </a>
-00000100: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00000110: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000120: 726f 6a65 6374 2f69 6465 7261 7265 5f70  roject/iderare_p
-00000130: 6865 6e6f 2f22 3e0a 2020 2020 2020 2020  heno/">.        
-00000140: 3c69 6d67 2061 6c74 3d22 5079 5049 2220  <img alt="PyPI" 
-00000150: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000160: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000170: 2f76 2f69 6465 7261 7265 5f70 6865 6e6f  /v/iderare_pheno
-00000180: 223e 0a20 2020 203c 2f61 3e0a 2020 2020  ">.    </a>.    
-00000190: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000001a0: 2f69 6465 7261 7265 2d70 6865 6e6f 2e72  /iderare-pheno.r
-000001b0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000001c0: 2f6c 6174 6573 742f 3f62 6164 6765 3d6c  /latest/?badge=l
-000001d0: 6174 6573 7422 3e0a 2020 2020 2020 2020  atest">.        
-000001e0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000001f0: 2f2f 7265 6164 7468 6564 6f63 732e 6f72  //readthedocs.or
-00000200: 672f 7072 6f6a 6563 7473 2f69 6465 7261  g/projects/idera
-00000210: 7265 2d70 6865 6e6f 2f62 6164 6765 2f3f  re-pheno/badge/?
-00000220: 7665 7273 696f 6e3d 6c61 7465 7374 2220  version=latest" 
-00000230: 616c 743d 2244 6f63 756d 656e 7461 7469  alt="Documentati
-00000240: 6f6e 2053 7461 7475 7322 202f 3e0a 2020  on Status" />.  
-00000250: 2020 3c2f 613e 0a20 2020 203c 6120 6872    </a>.    <a hr
-00000260: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00000270: 7562 2e63 6f6d 2f69 7661 6e77 696c 6c69  ub.com/ivanwilli
-00000280: 616d 6d64 2f69 6465 7261 7265 2d70 6865  ammd/iderare-phe
-00000290: 6e6f 2f62 6c6f 622f 6d61 696e 2f4c 4943  no/blob/main/LIC
-000002a0: 454e 5345 223e 0a20 2020 2020 2020 203c  ENSE">.        <
-000002b0: 696d 6720 616c 743d 224c 6963 656e 7365  img alt="License
-000002c0: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-000002d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-000002e0: 7468 7562 2f6c 6963 656e 7365 2f69 7661  thub/license/iva
-000002f0: 6e77 696c 6c69 616d 6d64 2f69 6465 7261  nwilliammd/idera
-00000300: 7265 2d70 6865 6e6f 2e73 7667 3f63 6f6c  re-pheno.svg?col
-00000310: 6f72 3d62 6c75 6526 6361 6368 6564 726f  or=blue&cachedro
-00000320: 7022 3e0a 2020 2020 3c2f 613e 0a20 2020  p">.    </a>.   
-00000330: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000340: 2f2f 6269 6f69 6e66 6f72 6d61 7469 6373  //bioinformatics
-00000350: 2d69 7661 6e77 696c 6c69 616d 6861 7273  -ivanwilliamhars
-00000360: 6f6e 6f2e 7374 7265 616d 6c69 742e 6170  ono.streamlit.ap
-00000370: 702f 4944 6552 6172 655f 5068 656e 6f22  p/IDeRare_Pheno"
-00000380: 3e0a 2020 2020 2020 2020 3c69 6d67 2061  >.        <img a
-00000390: 6c74 3d22 5374 7265 616d 6c69 7422 2073  lt="Streamlit" s
-000003a0: 7263 3d22 6874 7470 733a 2f2f 7374 6174  rc="https://stat
-000003b0: 6963 2e73 7472 6561 6d6c 6974 2e69 6f2f  ic.streamlit.io/
-000003c0: 6261 6467 6573 2f73 7472 6561 6d6c 6974  badges/streamlit
-000003d0: 5f62 6164 6765 5f62 6c61 636b 5f77 6869  _badge_black_whi
-000003e0: 7465 2e73 7667 223e 0a20 2020 203c 6272  te.svg">.    <br
-000003f0: 2f3e 0a3c 2f70 3e0a 0a49 4465 5261 7265  />.</p>..IDeRare
-00000400: 206f 7220 2249 6e64 6f6e 6573 6961 2045   or "Indonesia E
-00000410: 786f 6d65 2052 6172 6520 4469 7365 6173  xome Rare Diseas
-00000420: 6520 5661 7269 616e 7420 4469 7363 6f76  e Variant Discov
-00000430: 6572 7920 5069 7065 6c69 6e65 2220 6973  ery Pipeline" is
-00000440: 2061 2073 696d 706c 6520 616e 6420 7265   a simple and re
-00000450: 6164 7920 746f 2075 7365 2076 6172 6961  ady to use varia
-00000460: 6e74 2064 6973 636f 7665 7279 2070 6970  nt discovery pip
-00000470: 656c 696e 6520 746f 2064 6973 636f 7665  eline to discove
-00000480: 7220 7261 7265 2064 6973 6561 7365 2076  r rare disease v
-00000490: 6172 6961 6e74 7320 6672 6f6d 2065 786f  ariants from exo
-000004a0: 6d65 2073 6571 7565 6e63 696e 6720 6461  me sequencing da
-000004b0: 7461 2e20 0a0a 5468 6973 2072 6570 6f73  ta. ..This repos
-000004c0: 6974 6f72 7920 6973 202a 2a74 6865 2066  itory is **the f
-000004d0: 6972 7374 2070 6172 742a 2a20 6f66 2049  irst part** of I
-000004e0: 4465 5261 7265 2077 6f72 6b66 6c6f 7720  DeRare workflow 
-000004f0: 666f 7220 2a2a 7068 656e 6f74 7970 6520  for **phenotype 
-00000500: 616e 616c 7973 6973 2a2a 2e20 466f 7220  analysis**. For 
-00000510: 636f 6d70 6c65 7465 2070 6970 656c 696e  complete pipelin
-00000520: 6520 666f 7220 5f2a 2a70 6865 6e6f 7479  e for _**phenoty
-00000530: 7065 2d67 656e 6f74 7970 6520 616e 616c  pe-genotype anal
-00000540: 7973 6973 2a2a 5f2c 206b 696e 646c 7920  ysis**_, kindly 
-00000550: 7265 6665 7220 746f 205b 4944 6552 6172  refer to [IDeRar
-00000560: 6520 4769 7468 7562 2072 6570 6f73 6974  e Github reposit
-00000570: 6f72 795d 2868 7474 7073 3a2f 2f67 6974  ory](https://git
-00000580: 6875 622e 636f 6d2f 6976 616e 7769 6c6c  hub.com/ivanwill
-00000590: 6961 6d6d 642f 4944 6552 6172 6529 2e0a  iammd/IDeRare)..
-000005a0: 0a23 2320 4175 7468 6f72 6564 2062 7920  .## Authored by 
-000005b0: 0a49 7661 6e20 5769 6c6c 6961 6d20 4861  .Ivan William Ha
-000005c0: 7273 6f6e 6f3c 7375 703e 613c 2f73 7570  rsono<sup>a</sup
-000005d0: 3e2c 2059 756c 6961 2041 7269 616e 693c  >, Yulia Ariani<
-000005e0: 7375 703e 623c 2f73 7570 3e2c 2042 6562  sup>b</sup>, Beb
-000005f0: 656e 2042 656e 7961 6d69 6e3c 7375 703e  en Benyamin<sup>
-00000600: 632c 642c 653c 2f73 7570 3e2c 2046 6164  c,d,e</sup>, Fad
-00000610: 696c 6168 2046 6164 696c 6168 3c73 7570  ilah Fadilah<sup
-00000620: 3e66 2c67 3c2f 7375 703e 2c20 4477 6920  >f,g</sup>, Dwi 
-00000630: 4172 6920 5075 6a69 616e 746f 3c73 7570  Ari Pujianto<sup
-00000640: 3e62 3c2f 7375 703e 2c20 4375 7420 4e75  >b</sup>, Cut Nu
-00000650: 7275 6c20 4861 6669 6661 683c 7375 703e  rul Hafifah<sup>
-00000660: 683c 2f73 7570 3e0a 0a3c 7375 703e 613c  h</sup>..<sup>a<
-00000670: 2f73 7570 3e44 6f63 746f 7261 6c20 5072  /sup>Doctoral Pr
-00000680: 6f67 7261 6d20 696e 2042 696f 6d65 6469  ogram in Biomedi
-00000690: 6361 6c20 5363 6965 6e63 6573 2c20 4661  cal Sciences, Fa
-000006a0: 6375 6c74 7920 6f66 204d 6564 6963 696e  culty of Medicin
-000006b0: 652c 2055 6e69 7665 7273 6974 6173 2049  e, Universitas I
-000006c0: 6e64 6f6e 6573 6961 2c20 4a61 6b61 7274  ndonesia, Jakart
-000006d0: 612c 2049 6e64 6f6e 6573 6961 2e3c 6272  a, Indonesia.<br
-000006e0: 3e20 0a3c 7375 703e 623c 2f73 7570 3e44  > .<sup>b</sup>D
-000006f0: 6570 6172 746d 656e 7420 6f66 204d 6564  epartment of Med
-00000700: 6963 616c 2042 696f 6c6f 6779 2c20 4661  ical Biology, Fa
-00000710: 6375 6c74 7920 6f66 204d 6564 6963 696e  culty of Medicin
-00000720: 652c 2055 6e69 7665 7273 6974 6173 2049  e, Universitas I
-00000730: 6e64 6f6e 6573 6961 2c20 4a61 6b61 7274  ndonesia, Jakart
-00000740: 612c 2049 6e64 6f6e 6573 6961 2e3c 6272  a, Indonesia.<br
-00000750: 3e20 0a3c 7375 703e 633c 2f73 7570 3e41  > .<sup>c</sup>A
-00000760: 7573 7472 616c 6961 6e20 4365 6e74 7265  ustralian Centre
-00000770: 2066 6f72 2050 7265 6369 7369 6f6e 2048   for Precision H
-00000780: 6561 6c74 682c 2055 6e69 7665 7273 6974  ealth, Universit
-00000790: 7920 6f66 2053 6f75 7468 2041 7573 7472  y of South Austr
-000007a0: 616c 6961 2c20 4164 656c 6169 6465 2c20  alia, Adelaide, 
-000007b0: 5341 2c20 3530 3030 2c20 4175 7374 7261  SA, 5000, Austra
-000007c0: 6c69 612e 203c 6272 3e0a 3c73 7570 3e64  lia. <br>.<sup>d
-000007d0: 3c2f 7375 703e 556e 6953 4120 416c 6c69  </sup>UniSA Alli
-000007e0: 6564 2048 6561 6c74 6820 616e 6420 4875  ed Health and Hu
-000007f0: 6d61 6e20 5065 7266 6f72 6d61 6e63 652c  man Performance,
-00000800: 2055 6e69 7665 7273 6974 7920 6f66 2053   University of S
-00000810: 6f75 7468 2041 7573 7472 616c 6961 2c20  outh Australia, 
-00000820: 4164 656c 6169 6465 2c20 5341 2c20 3530  Adelaide, SA, 50
-00000830: 3030 2c20 4175 7374 7261 6c69 612e 203c  00, Australia. <
-00000840: 6272 3e0a 3c73 7570 3e65 3c2f 7375 703e  br>.<sup>e</sup>
-00000850: 536f 7574 6820 4175 7374 7261 6c69 616e  South Australian
-00000860: 2048 6561 6c74 6820 616e 6420 4d65 6469   Health and Medi
-00000870: 6361 6c20 5265 7365 6172 6368 2049 6e73  cal Research Ins
-00000880: 7469 7475 7465 2028 5341 484d 5249 292c  titute (SAHMRI),
-00000890: 2055 6e69 7665 7273 6974 7920 6f66 2053   University of S
-000008a0: 6f75 7468 2041 7573 7472 616c 6961 2c20  outh Australia, 
-000008b0: 4164 656c 6169 6465 2c20 5341 2c20 3530  Adelaide, SA, 50
-000008c0: 3030 2c20 4175 7374 7261 6c69 612e 203c  00, Australia. <
-000008d0: 6272 3e0a 3c73 7570 3e66 3c2f 7375 703e  br>.<sup>f</sup>
-000008e0: 4465 7061 7274 6d65 6e74 206f 6620 4d65  Department of Me
-000008f0: 6469 6361 6c20 4368 656d 6973 7472 792c  dical Chemistry,
-00000900: 2046 6163 756c 7479 206f 6620 4d65 6469   Faculty of Medi
-00000910: 6369 6e65 2c20 556e 6976 6572 7369 7461  cine, Universita
-00000920: 7320 496e 646f 6e65 7369 612c 204a 616c  s Indonesia, Jal
-00000930: 616e 2053 616c 656d 6261 2052 6179 6120  an Salemba Raya 
-00000940: 6e75 6d62 6572 2034 2c20 4a61 6b61 7274  number 4, Jakart
-00000950: 612c 2031 3034 3330 2c20 496e 646f 6e65  a, 10430, Indone
-00000960: 7369 612e 3c62 723e 0a3c 7375 703e 673c  sia.<br>.<sup>g<
-00000970: 2f73 7570 3e42 696f 696e 666f 726d 6174  /sup>Bioinformat
-00000980: 6963 7320 436f 7265 2046 6163 696c 6974  ics Core Facilit
-00000990: 6965 7320 2d20 494d 4552 492c 2046 6163  ies - IMERI, Fac
-000009a0: 756c 7479 206f 6620 4d65 6469 6369 6e65  ulty of Medicine
-000009b0: 2c20 556e 6976 6572 7369 7461 7320 496e  , Universitas In
-000009c0: 646f 6e65 7369 612c 204a 616c 616e 2053  donesia, Jalan S
-000009d0: 616c 656d 6261 2052 6179 6120 6e75 6d62  alemba Raya numb
-000009e0: 6572 2036 2c20 4a61 6b61 7274 612c 2031  er 6, Jakarta, 1
-000009f0: 3034 3330 2c20 496e 646f 6e65 7369 6120  0430, Indonesia 
-00000a00: 2e3c 6272 3e0a 3c73 7570 3e68 3c2f 7375  .<br>.<sup>h</su
-00000a10: 703e 4465 7061 7274 6d65 6e74 206f 6620  p>Department of 
-00000a20: 4368 696c 6420 4865 616c 7468 2c20 4472  Child Health, Dr
-00000a30: 2e20 4369 7074 6f20 4d61 6e67 756e 6b75  . Cipto Mangunku
-00000a40: 7375 6d6f 2048 6f73 7069 7461 6c2c 2046  sumo Hospital, F
-00000a50: 6163 756c 7479 206f 6620 4d65 6469 6369  aculty of Medici
-00000a60: 6e65 2c20 556e 6976 6572 7369 7479 206f  ne, University o
-00000a70: 6620 496e 646f 6e65 7369 612c 204a 616b  f Indonesia, Jak
-00000a80: 6172 7461 2c20 496e 646f 6e65 7369 612e  arta, Indonesia.
-00000a90: 203c 6272 3e0a 0a0a 2a2a 4e6f 7465 3a2a   <br>...**Note:*
-00000aa0: 2a20 4375 7272 656e 746c 7920 4944 6552  * Currently IDeR
-00000ab0: 6172 6520 7061 7065 7220 6973 2062 6569  are paper is bei
-00000ac0: 6e67 2063 6f6e 7369 6465 7265 6420 6a6f  ng considered jo
-00000ad0: 7572 6e61 6c20 7375 626d 6973 7369 6f6e  urnal submission
-00000ae0: 2e20 5468 6520 6369 7461 7469 6f6e 2077  . The citation w
-00000af0: 696c 6c20 6265 2075 7064 6174 6564 206f  ill be updated o
-00000b00: 6e63 6520 7468 6520 7061 7065 7220 6973  nce the paper is
-00000b10: 2070 7562 6c69 7368 6564 2e0a 0a23 2320   published...## 
-00000b20: 5175 6963 6b20 6c69 6e6b 730a 0a2d 205b  Quick links..- [
-00000b30: 446f 6375 6d65 6e74 6174 696f 6e5d 2868  Documentation](h
-00000b40: 7474 7073 3a2f 2f69 6465 7261 7265 2d70  ttps://iderare-p
-00000b50: 6865 6e6f 2e72 6561 6474 6865 646f 6373  heno.readthedocs
-00000b60: 2e69 6f2f 290a 2d20 5b50 7950 4920 5061  .io/).- [PyPI Pa
-00000b70: 636b 6167 655d 2868 7474 7073 3a2f 2f70  ckage](https://p
-00000b80: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000b90: 6964 6572 6172 652d 7068 656e 6f2f 290a  iderare-pheno/).
-00000ba0: 2d20 5b4c 6963 656e 7365 5d28 6874 7470  - [License](http
-00000bb0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
-00000bc0: 7661 6e77 696c 6c69 616d 6d64 2f69 6465  vanwilliammd/ide
-00000bd0: 7261 7265 2d70 6865 6e6f 2f62 6c6f 622f  rare-pheno/blob/
-00000be0: 6d61 696e 2f4c 4943 454e 5345 290a 2d20  main/LICENSE).- 
-00000bf0: 5b49 6e74 6572 6163 7469 7665 2050 6c61  [Interactive Pla
-00000c00: 7962 6f6f 6b20 4578 616d 706c 655d 2868  ybook Example](h
-00000c10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000c20: 6d2f 6976 616e 7769 6c6c 6961 6d6d 642f  m/ivanwilliammd/
-00000c30: 6964 6572 6172 652d 7068 656e 6f2f 626c  iderare-pheno/bl
-00000c40: 6f62 2f6d 6169 6e2f 506c 6179 626f 6f6b  ob/main/Playbook
-00000c50: 2e69 7079 6e62 290a 2d20 496e 7465 7261  .ipynb).- Intera
-00000c60: 6374 6976 6520 5765 6261 7070 7320 496d  ctive Webapps Im
-00000c70: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
-00000c80: 6174 205b 5374 7265 616d 6c69 745d 2868  at [Streamlit](h
-00000c90: 7474 7073 3a2f 2f62 696f 696e 666f 726d  ttps://bioinform
-00000ca0: 6174 6963 732d 6976 616e 7769 6c6c 6961  atics-ivanwillia
-00000cb0: 6d68 6172 736f 6e6f 2e73 7472 6561 6d6c  mharsono.streaml
-00000cc0: 6974 6170 702e 636f 6d2f 4944 6552 6172  itapp.com/IDeRar
-00000cd0: 655f 5068 656e 6f29 0a0a 0a23 2320 5768  e_Pheno)...## Wh
-00000ce0: 6174 2064 6f65 7320 6974 2064 6f3f 0a0a  at does it do?..
-00000cf0: 5468 6973 2073 6372 6970 7420 6973 2072  This script is r
-00000d00: 6563 6f6d 6d65 6e64 6564 2069 6620 796f  ecommended if yo
-00000d10: 7520 776f 756c 6420 6c69 6b65 2074 6f20  u would like to 
-00000d20: 646f 2063 6f6e 7665 7273 696f 6e2c 206c  do conversion, l
-00000d30: 696e 6b61 6765 2061 6e61 6c79 7369 732c  inkage analysis,
-00000d40: 2073 696d 696c 6172 6974 7920 7363 6f72   similarity scor
-00000d50: 696e 672c 2061 6e64 2067 656e 652d 6469  ing, and gene-di
-00000d60: 7365 6173 6520 7265 636f 6d6d 656e 6461  sease recommenda
-00000d70: 7469 6f6e 2062 6173 6564 206f 6e20 7468  tion based on th
-00000d80: 6520 7068 656e 6f74 7970 6520 6461 7461  e phenotype data
-00000d90: 2070 726f 7669 6465 6420 6174 205b 636c   provided at [cl
-00000da0: 696e 6963 616c 5f64 6174 612e 7478 745d  inical_data.txt]
-00000db0: 2863 6c69 6e69 6361 6c5f 6461 7461 2e74  (clinical_data.t
-00000dc0: 7874 292e 2046 756c 6c20 6665 6174 7572  xt). Full featur
-00000dd0: 6520 3a20 0a31 2e20 436f 6e76 6572 7420  e : .1. Convert 
-00000de0: 7468 6520 7068 656e 6f74 7970 6520 6461  the phenotype da
-00000df0: 7461 2074 6f20 4850 4f20 636f 6465 2028  ta to HPO code (
-00000e00: 6163 6365 7074 206d 6978 6564 2053 4e4f  accept mixed SNO
-00000e10: 4d45 442c 204c 4f49 4e43 2c20 616e 6420  MED, LOINC, and 
-00000e20: 4850 4f20 636f 6465 290a 322e 2053 696d  HPO code).2. Sim
-00000e30: 696c 6172 6974 7920 7363 6f72 696e 6720  ilarity scoring 
-00000e40: 6f66 2064 6966 6665 7265 6e74 6961 6c20  of differential 
-00000e50: 6469 6167 6e6f 7369 730a 332e 204c 696e  diagnosis.3. Lin
-00000e60: 6b61 6765 2061 6e61 6c79 7369 7320 6f66  kage analysis of
-00000e70: 2064 6966 6665 7265 6e74 6961 6c20 6469   differential di
-00000e80: 6167 6e6f 7369 7320 2861 6363 6570 7420  agnosis (accept 
-00000e90: 6d69 7865 6420 534e 4f4d 4544 2c20 4943  mixed SNOMED, IC
-00000ea0: 442d 3130 2c20 4f52 5048 412c 204f 4d49  D-10, ORPHA, OMI
-00000eb0: 4d20 636f 6465 292c 2069 6e63 6c75 6465  M code), include
-00000ec0: 2064 656e 6472 6f67 7261 6d20 7472 6565   dendrogram tree
-00000ed0: 2076 6973 7561 6c69 7a61 7469 6f6e 2e0a   visualization..
-00000ee0: 2020 2020 2d20 5468 6973 2073 686f 756c      - This shoul
-00000ef0: 6420 6865 6c70 2063 6c69 6e69 6369 616e  d help clinician
-00000f00: 2074 6f20 2a2a 7379 7374 656d 6174 6963   to **systematic
-00000f10: 616c 6c79 2064 6f69 6e67 2077 6f72 6b2d  ally doing work-
-00000f20: 7570 2061 6e64 2065 7863 6c75 6469 6e67  up and excluding
-00000f30: 2073 696d 696c 6172 2064 6961 676e 6f73   similar diagnos
-00000f40: 6973 2074 6f67 6574 6865 722a 2a20 6261  is together** ba
-00000f50: 7365 6420 6f6e 2074 6865 2070 6174 6965  sed on the patie
-00000f60: 6e74 5c27 7320 7068 656e 6f74 7970 652e  nt\'s phenotype.
-00000f70: 0a34 2e20 4765 6e65 2061 6e64 2064 6973  .4. Gene and dis
-00000f80: 6561 7365 2072 6563 6f6d 6d65 6e64 6174  ease recommendat
-00000f90: 696f 6e20 6261 7365 6420 6f6e 2074 6865  ion based on the
-00000fa0: 2070 6865 6e6f 7479 7065 2064 6174 6120   phenotype data 
-00000fb0: 7369 6d69 6c61 7269 7479 2073 636f 7269  similarity scori
-00000fc0: 6e67 2062 6574 7765 656e 202a 2a70 6865  ng between **phe
-00000fd0: 6e6f 7479 7065 2a2a 2061 6e64 204f 4d49  notype** and OMI
-00000fe0: 4d20 6765 6e65 2061 6e64 2064 6973 6561  M gene and disea
-00000ff0: 7365 2064 6174 6162 616e 6b2e 0a35 2e20  se databank..5. 
-00001000: 4c69 6e6b 6167 6520 616e 616c 7973 6973  Linkage analysis
-00001010: 206f 6620 7265 636f 6d6d 656e 6465 6420   of recommended 
-00001020: 6361 7573 6174 6976 6520 6765 6e65 2061  causative gene a
-00001030: 6e64 2064 6973 6561 7365 2062 6173 6564  nd disease based
-00001040: 206f 6e20 7068 656e 6f74 7970 6520 6461   on phenotype da
-00001050: 7461 2028 696e 636c 7564 6520 6465 6e64  ta (include dend
-00001060: 726f 6772 616d 2074 7265 6520 7669 7375  rogram tree visu
-00001070: 616c 697a 6174 696f 6e29 2e0a 2020 2020  alization)..    
-00001080: 2d20 5468 6973 2073 686f 756c 6420 6865  - This should he
-00001090: 6c70 2063 6c69 6e69 6369 616e 2074 6f20  lp clinician to 
-000010a0: 2a2a 6578 706c 6f72 6520 2f20 656e 7269  **explore / enri
-000010b0: 6368 2074 6865 6972 2064 6966 6665 7265  ch their differe
-000010c0: 6e74 6961 6c20 6469 6167 6e6f 7369 732a  ntial diagnosis*
-000010d0: 2a20 6261 7365 6420 6f6e 2074 6865 2070  * based on the p
-000010e0: 6174 6965 6e74 5c27 7320 7068 656e 6f74  atient\'s phenot
-000010f0: 7970 652e 0a36 2e20 4578 616d 706c 6520  ype..6. Example 
-00001100: 6f66 2074 6865 2063 6c69 6e69 6361 6c20  of the clinical 
-00001110: 6461 7461 2070 726f 7669 6465 6420 6174  data provided at
-00001120: 205b 436c 696e 6963 616c 2049 6e66 6f72   [Clinical Infor
-00001130: 6d61 7469 6f6e 2045 7861 6d70 6c65 2073  mation Example s
-00001140: 6563 7469 6f6e 5d28 2363 6c69 6e69 6361  ection](#clinica
-00001150: 6c2d 696e 666f 726d 6174 696f 6e2d 6578  l-information-ex
-00001160: 616d 706c 6529 0a0a 0a23 2320 496e 7374  ample)...## Inst
-00001170: 616c 6c61 7469 6f6e 0a0a 3c21 2d2d 2073  allation..<!-- s
-00001180: 7461 7274 2070 7920 7665 7273 696f 6e20  tart py version 
-00001190: 2d2d 3e0a 0a2a 2a69 6465 7261 7265 2d70  -->..**iderare-p
-000011a0: 6865 6e6f 2a2a 2072 6571 7569 7265 7320  heno** requires 
-000011b0: 5079 7468 6f6e 2033 2e38 206f 7220 6c61  Python 3.8 or la
-000011c0: 7465 722e 0a0a 3c21 2d2d 2065 6e64 2070  ter...<!-- end p
-000011d0: 7920 7665 7273 696f 6e20 2d2d 3e0a 0a23  y version -->..#
-000011e0: 2323 2049 6e73 7461 6c6c 696e 6720 7769  ## Installing wi
-000011f0: 7468 2060 7069 7060 0a0a 3c21 2d2d 2073  th `pip`..<!-- s
-00001200: 7461 7274 2069 6e73 7461 6c6c 2070 6970  tart install pip
-00001210: 202d 2d3e 0a0a 2a2a 6964 6572 6172 652d   -->..**iderare-
-00001220: 7068 656e 6f2a 2a20 6973 2061 7661 696c  pheno** is avail
-00001230: 6162 6c65 205b 6f6e 2050 7950 495d 2868  able [on PyPI](h
-00001240: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00001250: 7072 6f6a 6563 742f 6964 6572 6172 652d  project/iderare-
-00001260: 7068 656e 6f2f 292e 204a 7573 7420 7275  pheno/). Just ru
-00001270: 6e0a 0a60 6060 6261 7368 0a70 6970 2069  n..```bash.pip i
-00001280: 6e73 7461 6c6c 2069 6465 7261 7265 2d70  nstall iderare-p
-00001290: 6865 6e6f 0a60 6060 0a0a 3c21 2d2d 2065  heno.```..<!-- e
-000012a0: 6e64 2069 6e73 7461 6c6c 2070 6970 202d  nd install pip -
-000012b0: 2d3e 0a0a 2323 2320 496e 7374 616c 6c69  ->..### Installi
-000012c0: 6e67 2066 726f 6d20 736f 7572 6365 0a0a  ng from source..
-000012d0: 3c21 2d2d 2073 7461 7274 2069 6e73 7461  <!-- start insta
-000012e0: 6c6c 2073 6f75 7263 6520 2d2d 3e0a 0a54  ll source -->..T
-000012f0: 6f20 696e 7374 616c 6c20 2a2a 6964 6572  o install **ider
-00001300: 6172 652d 7068 656e 6f2a 2a20 6672 6f6d  are-pheno** from
-00001310: 2073 6f75 7263 652c 2066 6972 7374 2063   source, first c
-00001320: 6c6f 6e65 205b 7468 6520 7265 706f 7369  lone [the reposi
-00001330: 746f 7279 5d28 6874 7470 733a 2f2f 6769  tory](https://gi
-00001340: 7468 7562 2e63 6f6d 2f69 7661 6e77 696c  thub.com/ivanwil
-00001350: 6c69 616d 6d64 2f69 6465 7261 7265 2d70  liammd/iderare-p
-00001360: 6865 6e6f 293a 0a0a 6060 6062 6173 680a  heno):..```bash.
-00001370: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
-00001380: 2f2f 6769 7468 7562 2e63 6f6d 2f69 7661  //github.com/iva
-00001390: 6e77 696c 6c69 616d 6d64 2f69 6465 7261  nwilliammd/idera
-000013a0: 7265 2d70 6865 6e6f 2e67 6974 0a63 6420  re-pheno.git.cd 
-000013b0: 6964 6572 6172 655f 7068 656e 6f0a 6060  iderare_pheno.``
-000013c0: 600a 0a54 6865 6e20 7275 6e0a 0a60 6060  `..Then run..```
-000013d0: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
-000013e0: 202d 6520 2e0a 6060 600a 0a3c 212d 2d20   -e ..```..<!-- 
-000013f0: 656e 6420 696e 7374 616c 6c20 736f 7572  end install sour
-00001400: 6365 202d 2d3e 0a0a 2323 2049 6d70 6f72  ce -->..## Impor
-00001410: 7469 6e67 2074 6865 206c 6962 7261 7279  ting the library
-00001420: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00001430: 2069 6465 7261 7265 5f70 6865 6e6f 2e63   iderare_pheno.c
-00001440: 6f6e 7665 7274 6572 2069 6d70 6f72 7420  onverter import 
-00001450: 7465 726d 326f 6d69 6d2c 2074 6572 6d32  term2omim, term2
-00001460: 6f72 7068 612c 2074 6572 6d32 6870 6f2c  orpha, term2hpo,
-00001470: 2062 6174 6368 636f 6e76 6572 740a 6672   batchconvert.fr
-00001480: 6f6d 2069 6465 7261 7265 5f70 6865 6e6f  om iderare_pheno
-00001490: 2e73 696d 7265 6320 696d 706f 7274 2068  .simrec import h
-000014a0: 706f 326f 6d69 6d5f 7369 6d69 6c61 7269  po2omim_similari
-000014b0: 7479 2c20 6f6d 696d 5f72 6563 6f6d 6d65  ty, omim_recomme
-000014c0: 6e64 6174 696f 6e2c 2068 706f 326e 616d  ndation, hpo2nam
-000014d0: 650a 6672 6f6d 2069 6465 7261 7265 5f70  e.from iderare_p
-000014e0: 6865 6e6f 2e75 7469 6c73 2069 6d70 6f72  heno.utils impor
-000014f0: 7420 6c69 6e6b 6167 655f 6465 6e64 726f  t linkage_dendro
-00001500: 6772 616d 2c20 6c69 7374 3274 7376 2c20  gram, list2tsv, 
-00001510: 6765 6e65 7261 7465 5f79 6d6c 0a60 6060  generate_yml.```
-00001520: 0a41 7320 7468 6520 636f 6d70 6c65 7465  .As the complete
-00001530: 2072 6561 6474 6865 646f 6373 2e69 6f20   readthedocs.io 
-00001540: 6973 2073 7469 6c6c 206f 6e67 6f69 6e67  is still ongoing
-00001550: 2c20 706c 6561 7365 206b 696e 646c 7920  , please kindly 
-00001560: 7265 6665 7220 746f 2074 6869 7320 5b49  refer to this [I
-00001570: 6e74 6572 6163 7469 7665 2050 6c61 7962  nteractive Playb
-00001580: 6f6f 6b20 4578 616d 706c 655d 2868 7474  ook Example](htt
-00001590: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000015a0: 6976 616e 7769 6c6c 6961 6d6d 642f 6964  ivanwilliammd/id
-000015b0: 6572 6172 652d 7068 656e 6f2f 626c 6f62  erare-pheno/blob
-000015c0: 2f6d 6169 6e2f 506c 6179 626f 6f6b 2e69  /main/Playbook.i
-000015d0: 7079 6e62 290a 0a0a 2323 2054 6561 6d0a  pynb)...## Team.
-000015e0: 0a3c 212d 2d20 7374 6172 7420 7465 616d  .<!-- start team
-000015f0: 202d 2d3e 0a0a 2a2a 6964 6572 6172 652d   -->..**iderare-
-00001600: 7068 656e 6f2a 2a20 6973 2064 6576 656c  pheno** is devel
-00001610: 6f70 6564 2061 6e64 206d 6169 6e74 6169  oped and maintai
-00001620: 6e65 6420 6279 2074 6865 2061 7574 686f  ned by the autho
-00001630: 7228 7329 2c20 546f 206c 6561 726e 206d  r(s), To learn m
-00001640: 6f72 6520 6162 6f75 7420 7768 6f20 7370  ore about who sp
-00001650: 6563 6966 6963 616c 6c79 2063 6f6e 7472  ecifically contr
-00001660: 6962 7574 6564 2074 6f20 7468 6973 2063  ibuted to this c
-00001670: 6f64 6562 6173 652c 2073 6565 205b 6f75  odebase, see [ou
-00001680: 7220 636f 6e74 7269 6275 746f 7273 5d28  r contributors](
-00001690: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000016a0: 6f6d 2f69 7661 6e77 696c 6c69 616d 6d64  om/ivanwilliammd
-000016b0: 2f69 6465 7261 7265 2d70 6865 6e6f 2f67  /iderare-pheno/g
-000016c0: 7261 7068 732f 636f 6e74 7269 6275 746f  raphs/contributo
-000016d0: 7273 2920 7061 6765 2e0a 0a3c 212d 2d20  rs) page...<!-- 
-000016e0: 656e 6420 7465 616d 202d 2d3e 0a0a 2323  end team -->..##
-000016f0: 204c 6963 656e 7365 0a0a 3c21 2d2d 2073   License..<!-- s
-00001700: 7461 7274 206c 6963 656e 7365 202d 2d3e  tart license -->
-00001710: 0a0a 2a2a 6964 6572 6172 652d 7068 656e  ..**iderare-phen
-00001720: 6f2a 2a20 6c69 6365 6e73 6520 6973 2064  o** license is d
-00001730: 6572 6976 6564 2066 726f 6d20 5b49 4465  erived from [IDe
-00001740: 5261 7265 5d28 6874 7470 733a 2f2f 6769  Rare](https://gi
-00001750: 7468 7562 2e63 6f6d 2f69 7661 6e77 696c  thub.com/ivanwil
-00001760: 6c69 616d 6d64 2f69 6465 7261 7265 290a  liammd/iderare).
-00001770: 0a3c 212d 2d20 656e 6420 6c69 6365 6e73  .<!-- end licens
-00001780: 6520 2d2d 3e0a                           e -->.
+00000010: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+00000020: 7267 2f70 726f 6a65 6374 2f69 6465 7261  rg/project/idera
+00000030: 7265 5f70 6865 6e6f 2f29 0a0a 3c70 2061  re_pheno/)..<p a
+00000040: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+00000050: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000060: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
+00000070: 7661 6e77 696c 6c69 616d 6d64 2f69 6465  vanwilliammd/ide
+00000080: 7261 7265 2d70 6865 6e6f 2f61 6374 696f  rare-pheno/actio
+00000090: 6e73 223e 0a20 2020 2020 2020 203c 696d  ns">.        <im
+000000a0: 6720 616c 743d 2243 4922 2073 7263 3d22  g alt="CI" src="
+000000b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000c0: 6f6d 2f69 7661 6e77 696c 6c69 616d 6d64  om/ivanwilliammd
+000000d0: 2f69 6465 7261 7265 2d70 6865 6e6f 2f77  /iderare-pheno/w
+000000e0: 6f72 6b66 6c6f 7773 2f4d 6169 6e2f 6261  orkflows/Main/ba
+000000f0: 6467 652e 7376 6722 3e0a 2020 2020 3c2f  dge.svg">.    </
+00000100: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000110: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000120: 2f70 726f 6a65 6374 2f69 6465 7261 7265  /project/iderare
+00000130: 5f70 6865 6e6f 2f22 3e0a 2020 2020 2020  _pheno/">.      
+00000140: 2020 3c69 6d67 2061 6c74 3d22 5079 5049    <img alt="PyPI
+00000150: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000160: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000170: 7069 2f76 2f69 6465 7261 7265 5f70 6865  pi/v/iderare_phe
+00000180: 6e6f 223e 0a20 2020 203c 2f61 3e0a 3c21  no">.    </a>.<!
+00000190: 2d2d 2020 2020 203c 6120 6872 6566 3d22  --     <a href="
+000001a0: 6874 7470 733a 2f2f 6964 6572 6172 652d  https://iderare-
+000001b0: 7068 656e 6f2e 7265 6164 7468 6564 6f63  pheno.readthedoc
+000001c0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f3f  s.io/en/latest/?
+000001d0: 6261 6467 653d 6c61 7465 7374 223e 0a20  badge=latest">. 
+000001e0: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+000001f0: 2268 7474 7073 3a2f 2f72 6561 6474 6865  "https://readthe
+00000200: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
+00000210: 732f 6964 6572 6172 652d 7068 656e 6f2f  s/iderare-pheno/
+00000220: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+00000230: 6174 6573 7422 2061 6c74 3d22 446f 6375  atest" alt="Docu
+00000240: 6d65 6e74 6174 696f 6e20 5374 6174 7573  mentation Status
+00000250: 2220 2f3e 0a20 2020 203c 2f61 3e20 2d2d  " />.    </a> --
+00000260: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
+00000270: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000280: 6d2f 6976 616e 7769 6c6c 6961 6d6d 642f  m/ivanwilliammd/
+00000290: 6964 6572 6172 652d 7068 656e 6f2f 626c  iderare-pheno/bl
+000002a0: 6f62 2f6d 6169 6e2f 4c49 4345 4e53 4522  ob/main/LICENSE"
+000002b0: 3e0a 2020 2020 2020 2020 3c69 6d67 2061  >.        <img a
+000002c0: 6c74 3d22 4c69 6365 6e73 6522 2073 7263  lt="License" src
+000002d0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000002e0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+000002f0: 6c69 6365 6e73 652f 6976 616e 7769 6c6c  license/ivanwill
+00000300: 6961 6d6d 642f 6964 6572 6172 652d 7068  iammd/iderare-ph
+00000310: 656e 6f2e 7376 673f 636f 6c6f 723d 626c  eno.svg?color=bl
+00000320: 7565 2663 6163 6865 6472 6f70 223e 0a20  ue&cachedrop">. 
+00000330: 2020 203c 2f61 3e0a 2020 2020 3c61 2068     </a>.    <a h
+00000340: 7265 663d 2268 7474 7073 3a2f 2f62 696f  ref="https://bio
+00000350: 696e 666f 726d 6174 6963 732d 6976 616e  informatics-ivan
+00000360: 7769 6c6c 6961 6d68 6172 736f 6e6f 2e73  williamharsono.s
+00000370: 7472 6561 6d6c 6974 2e61 7070 2f49 4465  treamlit.app/IDe
+00000380: 5261 7265 5f50 6865 6e6f 223e 0a20 2020  Rare_Pheno">.   
+00000390: 2020 2020 203c 696d 6720 616c 743d 2253       <img alt="S
+000003a0: 7472 6561 6d6c 6974 2220 7372 633d 2268  treamlit" src="h
+000003b0: 7474 7073 3a2f 2f73 7461 7469 632e 7374  ttps://static.st
+000003c0: 7265 616d 6c69 742e 696f 2f62 6164 6765  reamlit.io/badge
+000003d0: 732f 7374 7265 616d 6c69 745f 6261 6467  s/streamlit_badg
+000003e0: 655f 626c 6163 6b5f 7768 6974 652e 7376  e_black_white.sv
+000003f0: 6722 3e0a 2020 2020 3c62 722f 3e0a 3c2f  g">.    <br/>.</
+00000400: 703e 0a0a 4944 6552 6172 6520 6f72 2022  p>..IDeRare or "
+00000410: 496e 646f 6e65 7369 6120 4578 6f6d 6520  Indonesia Exome 
+00000420: 5261 7265 2044 6973 6561 7365 2056 6172  Rare Disease Var
+00000430: 6961 6e74 2044 6973 636f 7665 7279 2050  iant Discovery P
+00000440: 6970 656c 696e 6522 2069 7320 6120 7369  ipeline" is a si
+00000450: 6d70 6c65 2061 6e64 2072 6561 6479 2074  mple and ready t
+00000460: 6f20 7573 6520 7661 7269 616e 7420 6469  o use variant di
+00000470: 7363 6f76 6572 7920 7069 7065 6c69 6e65  scovery pipeline
+00000480: 2074 6f20 6469 7363 6f76 6572 2072 6172   to discover rar
+00000490: 6520 6469 7365 6173 6520 7661 7269 616e  e disease varian
+000004a0: 7473 2066 726f 6d20 6578 6f6d 6520 7365  ts from exome se
+000004b0: 7175 656e 6369 6e67 2064 6174 612e 200a  quencing data. .
+000004c0: 0a54 6869 7320 7265 706f 7369 746f 7279  .This repository
+000004d0: 2069 7320 2a2a 7468 6520 6669 7273 7420   is **the first 
+000004e0: 7061 7274 2a2a 206f 6620 4944 6552 6172  part** of IDeRar
+000004f0: 6520 776f 726b 666c 6f77 2066 6f72 202a  e workflow for *
+00000500: 2a70 6865 6e6f 7479 7065 2061 6e61 6c79  *phenotype analy
+00000510: 7369 732a 2a2e 2046 6f72 2063 6f6d 706c  sis**. For compl
+00000520: 6574 6520 7069 7065 6c69 6e65 2066 6f72  ete pipeline for
+00000530: 205f 2a2a 7068 656e 6f74 7970 652d 6765   _**phenotype-ge
+00000540: 6e6f 7479 7065 2061 6e61 6c79 7369 732a  notype analysis*
+00000550: 2a5f 2c20 6b69 6e64 6c79 2072 6566 6572  *_, kindly refer
+00000560: 2074 6f20 5b49 4465 5261 7265 2047 6974   to [IDeRare Git
+00000570: 6875 6220 7265 706f 7369 746f 7279 5d28  hub repository](
+00000580: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000590: 6f6d 2f69 7661 6e77 696c 6c69 616d 6d64  om/ivanwilliammd
+000005a0: 2f49 4465 5261 7265 292e 0a0a 2323 2041  /IDeRare)...## A
+000005b0: 7574 686f 7265 6420 6279 200a 4976 616e  uthored by .Ivan
+000005c0: 2057 696c 6c69 616d 2048 6172 736f 6e6f   William Harsono
+000005d0: 3c73 7570 3e61 3c2f 7375 703e 2c20 5975  <sup>a</sup>, Yu
+000005e0: 6c69 6120 4172 6961 6e69 3c73 7570 3e62  lia Ariani<sup>b
+000005f0: 3c2f 7375 703e 2c20 4265 6265 6e20 4265  </sup>, Beben Be
+00000600: 6e79 616d 696e 3c73 7570 3e63 2c64 2c65  nyamin<sup>c,d,e
+00000610: 3c2f 7375 703e 2c20 4661 6469 6c61 6820  </sup>, Fadilah 
+00000620: 4661 6469 6c61 683c 7375 703e 662c 673c  Fadilah<sup>f,g<
+00000630: 2f73 7570 3e2c 2044 7769 2041 7269 2050  /sup>, Dwi Ari P
+00000640: 756a 6961 6e74 6f3c 7375 703e 623c 2f73  ujianto<sup>b</s
+00000650: 7570 3e2c 2043 7574 204e 7572 756c 2048  up>, Cut Nurul H
+00000660: 6166 6966 6168 3c73 7570 3e68 3c2f 7375  afifah<sup>h</su
+00000670: 703e 0a0a 3c73 7570 3e61 3c2f 7375 703e  p>..<sup>a</sup>
+00000680: 446f 6374 6f72 616c 2050 726f 6772 616d  Doctoral Program
+00000690: 2069 6e20 4269 6f6d 6564 6963 616c 2053   in Biomedical S
+000006a0: 6369 656e 6365 732c 2046 6163 756c 7479  ciences, Faculty
+000006b0: 206f 6620 4d65 6469 6369 6e65 2c20 556e   of Medicine, Un
+000006c0: 6976 6572 7369 7461 7320 496e 646f 6e65  iversitas Indone
+000006d0: 7369 612c 204a 616b 6172 7461 2c20 496e  sia, Jakarta, In
+000006e0: 646f 6e65 7369 612e 3c62 723e 200a 3c73  donesia.<br> .<s
+000006f0: 7570 3e62 3c2f 7375 703e 4465 7061 7274  up>b</sup>Depart
+00000700: 6d65 6e74 206f 6620 4d65 6469 6361 6c20  ment of Medical 
+00000710: 4269 6f6c 6f67 792c 2046 6163 756c 7479  Biology, Faculty
+00000720: 206f 6620 4d65 6469 6369 6e65 2c20 556e   of Medicine, Un
+00000730: 6976 6572 7369 7461 7320 496e 646f 6e65  iversitas Indone
+00000740: 7369 612c 204a 616b 6172 7461 2c20 496e  sia, Jakarta, In
+00000750: 646f 6e65 7369 612e 3c62 723e 200a 3c73  donesia.<br> .<s
+00000760: 7570 3e63 3c2f 7375 703e 4175 7374 7261  up>c</sup>Austra
+00000770: 6c69 616e 2043 656e 7472 6520 666f 7220  lian Centre for 
+00000780: 5072 6563 6973 696f 6e20 4865 616c 7468  Precision Health
+00000790: 2c20 556e 6976 6572 7369 7479 206f 6620  , University of 
+000007a0: 536f 7574 6820 4175 7374 7261 6c69 612c  South Australia,
+000007b0: 2041 6465 6c61 6964 652c 2053 412c 2035   Adelaide, SA, 5
+000007c0: 3030 302c 2041 7573 7472 616c 6961 2e20  000, Australia. 
+000007d0: 3c62 723e 0a3c 7375 703e 643c 2f73 7570  <br>.<sup>d</sup
+000007e0: 3e55 6e69 5341 2041 6c6c 6965 6420 4865  >UniSA Allied He
+000007f0: 616c 7468 2061 6e64 2048 756d 616e 2050  alth and Human P
+00000800: 6572 666f 726d 616e 6365 2c20 556e 6976  erformance, Univ
+00000810: 6572 7369 7479 206f 6620 536f 7574 6820  ersity of South 
+00000820: 4175 7374 7261 6c69 612c 2041 6465 6c61  Australia, Adela
+00000830: 6964 652c 2053 412c 2035 3030 302c 2041  ide, SA, 5000, A
+00000840: 7573 7472 616c 6961 2e20 3c62 723e 0a3c  ustralia. <br>.<
+00000850: 7375 703e 653c 2f73 7570 3e53 6f75 7468  sup>e</sup>South
+00000860: 2041 7573 7472 616c 6961 6e20 4865 616c   Australian Heal
+00000870: 7468 2061 6e64 204d 6564 6963 616c 2052  th and Medical R
+00000880: 6573 6561 7263 6820 496e 7374 6974 7574  esearch Institut
+00000890: 6520 2853 4148 4d52 4929 2c20 556e 6976  e (SAHMRI), Univ
+000008a0: 6572 7369 7479 206f 6620 536f 7574 6820  ersity of South 
+000008b0: 4175 7374 7261 6c69 612c 2041 6465 6c61  Australia, Adela
+000008c0: 6964 652c 2053 412c 2035 3030 302c 2041  ide, SA, 5000, A
+000008d0: 7573 7472 616c 6961 2e20 3c62 723e 0a3c  ustralia. <br>.<
+000008e0: 7375 703e 663c 2f73 7570 3e44 6570 6172  sup>f</sup>Depar
+000008f0: 746d 656e 7420 6f66 204d 6564 6963 616c  tment of Medical
+00000900: 2043 6865 6d69 7374 7279 2c20 4661 6375   Chemistry, Facu
+00000910: 6c74 7920 6f66 204d 6564 6963 696e 652c  lty of Medicine,
+00000920: 2055 6e69 7665 7273 6974 6173 2049 6e64   Universitas Ind
+00000930: 6f6e 6573 6961 2c20 4a61 6c61 6e20 5361  onesia, Jalan Sa
+00000940: 6c65 6d62 6120 5261 7961 206e 756d 6265  lemba Raya numbe
+00000950: 7220 342c 204a 616b 6172 7461 2c20 3130  r 4, Jakarta, 10
+00000960: 3433 302c 2049 6e64 6f6e 6573 6961 2e3c  430, Indonesia.<
+00000970: 6272 3e0a 3c73 7570 3e67 3c2f 7375 703e  br>.<sup>g</sup>
+00000980: 4269 6f69 6e66 6f72 6d61 7469 6373 2043  Bioinformatics C
+00000990: 6f72 6520 4661 6369 6c69 7469 6573 202d  ore Facilities -
+000009a0: 2049 4d45 5249 2c20 4661 6375 6c74 7920   IMERI, Faculty 
+000009b0: 6f66 204d 6564 6963 696e 652c 2055 6e69  of Medicine, Uni
+000009c0: 7665 7273 6974 6173 2049 6e64 6f6e 6573  versitas Indones
+000009d0: 6961 2c20 4a61 6c61 6e20 5361 6c65 6d62  ia, Jalan Salemb
+000009e0: 6120 5261 7961 206e 756d 6265 7220 362c  a Raya number 6,
+000009f0: 204a 616b 6172 7461 2c20 3130 3433 302c   Jakarta, 10430,
+00000a00: 2049 6e64 6f6e 6573 6961 202e 3c62 723e   Indonesia .<br>
+00000a10: 0a3c 7375 703e 683c 2f73 7570 3e44 6570  .<sup>h</sup>Dep
+00000a20: 6172 746d 656e 7420 6f66 2043 6869 6c64  artment of Child
+00000a30: 2048 6561 6c74 682c 2044 722e 2043 6970   Health, Dr. Cip
+00000a40: 746f 204d 616e 6775 6e6b 7573 756d 6f20  to Mangunkusumo 
+00000a50: 486f 7370 6974 616c 2c20 4661 6375 6c74  Hospital, Facult
+00000a60: 7920 6f66 204d 6564 6963 696e 652c 2055  y of Medicine, U
+00000a70: 6e69 7665 7273 6974 7920 6f66 2049 6e64  niversity of Ind
+00000a80: 6f6e 6573 6961 2c20 4a61 6b61 7274 612c  onesia, Jakarta,
+00000a90: 2049 6e64 6f6e 6573 6961 2e20 3c62 723e   Indonesia. <br>
+00000aa0: 0a0a 0a2a 2a4e 6f74 653a 2a2a 2043 7572  ...**Note:** Cur
+00000ab0: 7265 6e74 6c79 2049 4465 5261 7265 2070  rently IDeRare p
+00000ac0: 6170 6572 2069 7320 6265 696e 6720 636f  aper is being co
+00000ad0: 6e73 6964 6572 6564 206a 6f75 726e 616c  nsidered journal
+00000ae0: 2073 7562 6d69 7373 696f 6e2e 2054 6865   submission. The
+00000af0: 2063 6974 6174 696f 6e20 7769 6c6c 2062   citation will b
+00000b00: 6520 7570 6461 7465 6420 6f6e 6365 2074  e updated once t
+00000b10: 6865 2070 6170 6572 2069 7320 7075 626c  he paper is publ
+00000b20: 6973 6865 642e 0a0a 2323 2051 7569 636b  ished...## Quick
+00000b30: 206c 696e 6b73 0a2d 205b 4944 6552 6172   links.- [IDeRar
+00000b40: 6520 6675 6c6c 2070 6970 656c 696e 6520  e full pipeline 
+00000b50: 2d20 5068 656e 6f74 7970 6520 616e 6420  - Phenotype and 
+00000b60: 4765 6e6f 7479 7065 5d28 6874 7470 733a  Genotype](https:
+00000b70: 2f2f 6769 7468 7562 2e63 6f6d 2f69 7661  //github.com/iva
+00000b80: 6e77 696c 6c69 616d 6d64 2f49 4465 5261  nwilliammd/IDeRa
+00000b90: 7265 290a 2d20 5b50 7950 4920 5061 636b  re).- [PyPI Pack
+00000ba0: 6167 655d 2868 7474 7073 3a2f 2f70 7970  age](https://pyp
+00000bb0: 692e 6f72 672f 7072 6f6a 6563 742f 6964  i.org/project/id
+00000bc0: 6572 6172 652d 7068 656e 6f2f 290a 2d20  erare-pheno/).- 
+00000bd0: 5b4c 6963 656e 7365 5d28 6874 7470 733a  [License](https:
+00000be0: 2f2f 6769 7468 7562 2e63 6f6d 2f69 7661  //github.com/iva
+00000bf0: 6e77 696c 6c69 616d 6d64 2f69 6465 7261  nwilliammd/idera
+00000c00: 7265 2d70 6865 6e6f 2f62 6c6f 622f 6d61  re-pheno/blob/ma
+00000c10: 696e 2f4c 4943 454e 5345 290a 2d20 5b49  in/LICENSE).- [I
+00000c20: 6e74 6572 6163 7469 7665 2050 6c61 7962  nteractive Playb
+00000c30: 6f6f 6b20 4578 616d 706c 655d 2868 7474  ook Example](htt
+00000c40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000c50: 6976 616e 7769 6c6c 6961 6d6d 642f 6964  ivanwilliammd/id
+00000c60: 6572 6172 652d 7068 656e 6f2f 626c 6f62  erare-pheno/blob
+00000c70: 2f6d 6169 6e2f 506c 6179 626f 6f6b 2e69  /main/Playbook.i
+00000c80: 7079 6e62 290a 2d20 496e 7465 7261 6374  pynb).- Interact
+00000c90: 6976 6520 5765 6261 7070 7320 496d 706c  ive Webapps Impl
+00000ca0: 656d 656e 7461 7469 6f6e 206f 6620 6174  ementation of at
+00000cb0: 205b 5374 7265 616d 6c69 745d 2868 7474   [Streamlit](htt
+00000cc0: 7073 3a2f 2f62 696f 696e 666f 726d 6174  ps://bioinformat
+00000cd0: 6963 732d 6976 616e 7769 6c6c 6961 6d68  ics-ivanwilliamh
+00000ce0: 6172 736f 6e6f 2e73 7472 6561 6d6c 6974  arsono.streamlit
+00000cf0: 6170 702e 636f 6d2f 4944 6552 6172 655f  app.com/IDeRare_
+00000d00: 5068 656e 6f29 0a3c 212d 2d20 2d20 5b44  Pheno).<!-- - [D
+00000d10: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+00000d20: 7470 733a 2f2f 6964 6572 6172 652d 7068  tps://iderare-ph
+00000d30: 656e 6f2e 7265 6164 7468 6564 6f63 732e  eno.readthedocs.
+00000d40: 696f 2f29 202d 2d3e 0a0a 2323 2057 6861  io/) -->..## Wha
+00000d50: 7420 646f 6573 2069 7420 646f 3f0a 0a54  t does it do?..T
+00000d60: 6869 7320 7363 7269 7074 2069 7320 7265  his script is re
+00000d70: 636f 6d6d 656e 6465 6420 6966 2079 6f75  commended if you
+00000d80: 2077 6f75 6c64 206c 696b 6520 746f 2064   would like to d
+00000d90: 6f20 636f 6e76 6572 7369 6f6e 2c20 6c69  o conversion, li
+00000da0: 6e6b 6167 6520 616e 616c 7973 6973 2c20  nkage analysis, 
+00000db0: 7369 6d69 6c61 7269 7479 2073 636f 7269  similarity scori
+00000dc0: 6e67 2c20 616e 6420 6765 6e65 2d64 6973  ng, and gene-dis
+00000dd0: 6561 7365 2072 6563 6f6d 6d65 6e64 6174  ease recommendat
+00000de0: 696f 6e20 6261 7365 6420 6f6e 2074 6865  ion based on the
+00000df0: 2070 6865 6e6f 7479 7065 2064 6174 6120   phenotype data 
+00000e00: 7072 6f76 6964 6564 2061 7420 5b63 6c69  provided at [cli
+00000e10: 6e69 6361 6c5f 6461 7461 2e74 7874 5d28  nical_data.txt](
+00000e20: 636c 696e 6963 616c 5f64 6174 612e 7478  clinical_data.tx
+00000e30: 7429 2e20 4675 6c6c 2066 6561 7475 7265  t). Full feature
+00000e40: 203a 200a 312e 2043 6f6e 7665 7274 2074   : .1. Convert t
+00000e50: 6865 2070 6865 6e6f 7479 7065 2064 6174  he phenotype dat
+00000e60: 6120 746f 2048 504f 2063 6f64 6520 2861  a to HPO code (a
+00000e70: 6363 6570 7420 6d69 7865 6420 534e 4f4d  ccept mixed SNOM
+00000e80: 4544 2c20 4c4f 494e 432c 2061 6e64 2048  ED, LOINC, and H
+00000e90: 504f 2063 6f64 6529 0a32 2e20 5369 6d69  PO code).2. Simi
+00000ea0: 6c61 7269 7479 2073 636f 7269 6e67 206f  larity scoring o
+00000eb0: 6620 6469 6666 6572 656e 7469 616c 2064  f differential d
+00000ec0: 6961 676e 6f73 6973 0a33 2e20 4c69 6e6b  iagnosis.3. Link
+00000ed0: 6167 6520 616e 616c 7973 6973 206f 6620  age analysis of 
+00000ee0: 6469 6666 6572 656e 7469 616c 2064 6961  differential dia
+00000ef0: 676e 6f73 6973 2028 6163 6365 7074 206d  gnosis (accept m
+00000f00: 6978 6564 2053 4e4f 4d45 442c 2049 4344  ixed SNOMED, ICD
+00000f10: 2d31 302c 204f 5250 4841 2c20 4f4d 494d  -10, ORPHA, OMIM
+00000f20: 2063 6f64 6529 2c20 696e 636c 7564 6520   code), include 
+00000f30: 6465 6e64 726f 6772 616d 2074 7265 6520  dendrogram tree 
+00000f40: 7669 7375 616c 697a 6174 696f 6e2e 0a20  visualization.. 
+00000f50: 2020 202d 2054 6869 7320 7368 6f75 6c64     - This should
+00000f60: 2068 656c 7020 636c 696e 6963 6961 6e20   help clinician 
+00000f70: 746f 202a 2a73 7973 7465 6d61 7469 6361  to **systematica
+00000f80: 6c6c 7920 646f 696e 6720 776f 726b 2d75  lly doing work-u
+00000f90: 7020 616e 6420 6578 636c 7564 696e 6720  p and excluding 
+00000fa0: 7369 6d69 6c61 7220 6469 6167 6e6f 7369  similar diagnosi
+00000fb0: 7320 746f 6765 7468 6572 2a2a 2062 6173  s together** bas
+00000fc0: 6564 206f 6e20 7468 6520 7061 7469 656e  ed on the patien
+00000fd0: 745c 2773 2070 6865 6e6f 7479 7065 2e0a  t\'s phenotype..
+00000fe0: 342e 2047 656e 6520 616e 6420 6469 7365  4. Gene and dise
+00000ff0: 6173 6520 7265 636f 6d6d 656e 6461 7469  ase recommendati
+00001000: 6f6e 2062 6173 6564 206f 6e20 7468 6520  on based on the 
+00001010: 7068 656e 6f74 7970 6520 6461 7461 2073  phenotype data s
+00001020: 696d 696c 6172 6974 7920 7363 6f72 696e  imilarity scorin
+00001030: 6720 6265 7477 6565 6e20 2a2a 7068 656e  g between **phen
+00001040: 6f74 7970 652a 2a20 616e 6420 4f4d 494d  otype** and OMIM
+00001050: 2067 656e 6520 616e 6420 6469 7365 6173   gene and diseas
+00001060: 6520 6461 7461 6261 6e6b 2e0a 352e 204c  e databank..5. L
+00001070: 696e 6b61 6765 2061 6e61 6c79 7369 7320  inkage analysis 
+00001080: 6f66 2072 6563 6f6d 6d65 6e64 6564 2063  of recommended c
+00001090: 6175 7361 7469 7665 2067 656e 6520 616e  ausative gene an
+000010a0: 6420 6469 7365 6173 6520 6261 7365 6420  d disease based 
+000010b0: 6f6e 2070 6865 6e6f 7479 7065 2064 6174  on phenotype dat
+000010c0: 6120 2869 6e63 6c75 6465 2064 656e 6472  a (include dendr
+000010d0: 6f67 7261 6d20 7472 6565 2076 6973 7561  ogram tree visua
+000010e0: 6c69 7a61 7469 6f6e 292e 0a20 2020 202d  lization)..    -
+000010f0: 2054 6869 7320 7368 6f75 6c64 2068 656c   This should hel
+00001100: 7020 636c 696e 6963 6961 6e20 746f 202a  p clinician to *
+00001110: 2a65 7870 6c6f 7265 202f 2065 6e72 6963  *explore / enric
+00001120: 6820 7468 6569 7220 6469 6666 6572 656e  h their differen
+00001130: 7469 616c 2064 6961 676e 6f73 6973 2a2a  tial diagnosis**
+00001140: 2062 6173 6564 206f 6e20 7468 6520 7061   based on the pa
+00001150: 7469 656e 745c 2773 2070 6865 6e6f 7479  tient\'s phenoty
+00001160: 7065 2e0a 362e 2045 7861 6d70 6c65 206f  pe..6. Example o
+00001170: 6620 7468 6520 636c 696e 6963 616c 2064  f the clinical d
+00001180: 6174 6120 7072 6f76 6964 6564 2061 7420  ata provided at 
+00001190: 5b43 6c69 6e69 6361 6c20 496e 666f 726d  [Clinical Inform
+000011a0: 6174 696f 6e20 4578 616d 706c 6520 7365  ation Example se
+000011b0: 6374 696f 6e5d 2823 636c 696e 6963 616c  ction](#clinical
+000011c0: 2d69 6e66 6f72 6d61 7469 6f6e 2d65 7861  -information-exa
+000011d0: 6d70 6c65 290a 0a0a 2323 2049 6e73 7461  mple)...## Insta
+000011e0: 6c6c 6174 696f 6e0a 0a3c 212d 2d20 7374  llation..<!-- st
+000011f0: 6172 7420 7079 2076 6572 7369 6f6e 202d  art py version -
+00001200: 2d3e 0a0a 2a2a 6964 6572 6172 652d 7068  ->..**iderare-ph
+00001210: 656e 6f2a 2a20 7265 7175 6972 6573 2050  eno** requires P
+00001220: 7974 686f 6e20 332e 3820 6f72 206c 6174  ython 3.8 or lat
+00001230: 6572 2e0a 0a3c 212d 2d20 656e 6420 7079  er...<!-- end py
+00001240: 2076 6572 7369 6f6e 202d 2d3e 0a0a 2323   version -->..##
+00001250: 2320 496e 7374 616c 6c69 6e67 2077 6974  # Installing wit
+00001260: 6820 6070 6970 600a 0a3c 212d 2d20 7374  h `pip`..<!-- st
+00001270: 6172 7420 696e 7374 616c 6c20 7069 7020  art install pip 
+00001280: 2d2d 3e0a 0a2a 2a69 6465 7261 7265 2d70  -->..**iderare-p
+00001290: 6865 6e6f 2a2a 2069 7320 6176 6169 6c61  heno** is availa
+000012a0: 626c 6520 5b6f 6e20 5079 5049 5d28 6874  ble [on PyPI](ht
+000012b0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000012c0: 726f 6a65 6374 2f69 6465 7261 7265 2d70  roject/iderare-p
+000012d0: 6865 6e6f 2f29 2e20 4a75 7374 2072 756e  heno/). Just run
+000012e0: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
+000012f0: 7374 616c 6c20 6964 6572 6172 652d 7068  stall iderare-ph
+00001300: 656e 6f0a 6060 600a 0a3c 212d 2d20 656e  eno.```..<!-- en
+00001310: 6420 696e 7374 616c 6c20 7069 7020 2d2d  d install pip --
+00001320: 3e0a 0a23 2323 2049 6e73 7461 6c6c 696e  >..### Installin
+00001330: 6720 6672 6f6d 2073 6f75 7263 650a 0a3c  g from source..<
+00001340: 212d 2d20 7374 6172 7420 696e 7374 616c  !-- start instal
+00001350: 6c20 736f 7572 6365 202d 2d3e 0a0a 546f  l source -->..To
+00001360: 2069 6e73 7461 6c6c 202a 2a69 6465 7261   install **idera
+00001370: 7265 2d70 6865 6e6f 2a2a 2066 726f 6d20  re-pheno** from 
+00001380: 736f 7572 6365 2c20 6669 7273 7420 636c  source, first cl
+00001390: 6f6e 6520 5b74 6865 2072 6570 6f73 6974  one [the reposit
+000013a0: 6f72 795d 2868 7474 7073 3a2f 2f67 6974  ory](https://git
+000013b0: 6875 622e 636f 6d2f 6976 616e 7769 6c6c  hub.com/ivanwill
+000013c0: 6961 6d6d 642f 6964 6572 6172 652d 7068  iammd/iderare-ph
+000013d0: 656e 6f29 3a0a 0a60 6060 6261 7368 0a67  eno):..```bash.g
+000013e0: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+000013f0: 2f67 6974 6875 622e 636f 6d2f 6976 616e  /github.com/ivan
+00001400: 7769 6c6c 6961 6d6d 642f 6964 6572 6172  williammd/iderar
+00001410: 652d 7068 656e 6f2e 6769 740a 6364 2069  e-pheno.git.cd i
+00001420: 6465 7261 7265 5f70 6865 6e6f 0a60 6060  derare_pheno.```
+00001430: 0a0a 5468 656e 2072 756e 0a0a 6060 6062  ..Then run..```b
+00001440: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+00001450: 2d65 202e 0a60 6060 0a0a 3c21 2d2d 2065  -e ..```..<!-- e
+00001460: 6e64 2069 6e73 7461 6c6c 2073 6f75 7263  nd install sourc
+00001470: 6520 2d2d 3e0a 0a23 2320 496d 706f 7274  e -->..## Import
+00001480: 696e 6720 7468 6520 6c69 6272 6172 790a  ing the library.
+00001490: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+000014a0: 6964 6572 6172 655f 7068 656e 6f2e 636f  iderare_pheno.co
+000014b0: 6e76 6572 7465 7220 696d 706f 7274 2074  nverter import t
+000014c0: 6572 6d32 6f6d 696d 2c20 7465 726d 326f  erm2omim, term2o
+000014d0: 7270 6861 2c20 7465 726d 3268 706f 2c20  rpha, term2hpo, 
+000014e0: 6261 7463 6863 6f6e 7665 7274 0a66 726f  batchconvert.fro
+000014f0: 6d20 6964 6572 6172 655f 7068 656e 6f2e  m iderare_pheno.
+00001500: 7369 6d72 6563 2069 6d70 6f72 7420 6870  simrec import hp
+00001510: 6f32 6f6d 696d 5f73 696d 696c 6172 6974  o2omim_similarit
+00001520: 792c 206f 6d69 6d5f 7265 636f 6d6d 656e  y, omim_recommen
+00001530: 6461 7469 6f6e 2c20 6870 6f32 6e61 6d65  dation, hpo2name
+00001540: 2c20 6f6d 696d 326e 616d 650a 6672 6f6d  , omim2name.from
+00001550: 2069 6465 7261 7265 5f70 6865 6e6f 2e75   iderare_pheno.u
+00001560: 7469 6c73 2069 6d70 6f72 7420 6c69 6e6b  tils import link
+00001570: 6167 655f 6465 6e64 726f 6772 616d 2c20  age_dendrogram, 
+00001580: 6c69 7374 3274 7376 2c20 6765 6e65 7261  list2tsv, genera
+00001590: 7465 5f79 6d6c 0a60 6060 0a41 7320 7468  te_yml.```.As th
+000015a0: 6520 636f 6d70 6c65 7465 2072 6561 6474  e complete readt
+000015b0: 6865 646f 6373 2e69 6f20 6973 2062 6569  hedocs.io is bei
+000015c0: 6e67 2066 696e 616c 697a 6564 2c20 706c  ng finalized, pl
+000015d0: 6561 7365 206b 696e 646c 7920 7265 6665  ease kindly refe
+000015e0: 7220 746f 2074 6869 7320 5b49 6e74 6572  r to this [Inter
+000015f0: 6163 7469 7665 2050 6c61 7962 6f6f 6b20  active Playbook 
+00001600: 4578 616d 706c 655d 2868 7474 7073 3a2f  Example](https:/
+00001610: 2f67 6974 6875 622e 636f 6d2f 6976 616e  /github.com/ivan
+00001620: 7769 6c6c 6961 6d6d 642f 6964 6572 6172  williammd/iderar
+00001630: 652d 7068 656e 6f2f 626c 6f62 2f6d 6169  e-pheno/blob/mai
+00001640: 6e2f 506c 6179 626f 6f6b 2e69 7079 6e62  n/Playbook.ipynb
+00001650: 290a 0a4e 6f74 6520 3a20 666f 7220 5374  )..Note : for St
+00001660: 7265 616d 6c69 7420 696d 706c 656d 656e  reamlit implemen
+00001670: 7461 7469 6f6e 2c20 7573 6520 6060 6069  tation, use ```i
+00001680: 6465 7261 7265 5f70 6865 6e6f 2e73 7472  derare_pheno.str
+00001690: 6561 6d6c 6974 5f75 7469 6c73 6060 6020  eamlit_utils``` 
+000016a0: 696e 7374 6561 6420 6f66 2060 6060 6964  instead of ```id
+000016b0: 6572 6172 655f 7068 656e 6f2e 7574 696c  erare_pheno.util
+000016c0: 7360 6060 2c20 7468 6973 2077 6173 2064  s```, this was d
+000016d0: 6f6e 6520 746f 2070 7265 7665 6e74 2066  one to prevent f
+000016e0: 696c 6520 746f 2061 7574 6f6d 6174 6963  ile to automatic
+000016f0: 616c 6c79 2073 6176 696e 6720 616e 6420  ally saving and 
+00001700: 7368 6f77 696e 6720 6465 6e64 726f 6772  showing dendrogr
+00001710: 616d 2069 6e20 5374 7265 616d 6c69 742e  am in Streamlit.
+00001720: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00001730: 6964 6572 6172 655f 7068 656e 6f2e 7374  iderare_pheno.st
+00001740: 7265 616d 6c69 745f 7574 696c 7320 696d  reamlit_utils im
+00001750: 706f 7274 206c 696e 6b61 6765 5f64 656e  port linkage_den
+00001760: 6472 6f67 7261 6d2c 206c 6973 7432 7473  drogram, list2ts
+00001770: 762c 2067 656e 6572 6174 655f 796d 6c0a  v, generate_yml.
+00001780: 6060 600a 0a46 6f72 2050 7974 686f 6e20  ```..For Python 
+00001790: 4661 7374 4150 4920 696d 706c 656d 656e  FastAPI implemen
+000017a0: 7461 7469 6f6e 2061 6e64 2046 4849 5220  tation and FHIR 
+000017b0: 636f 6465 2065 7874 7261 6374 696f 6e20  code extraction 
+000017c0: 2f20 7061 7273 696e 6720 616e 6420 6465  / parsing and de
+000017d0: 706c 6f79 696e 6720 7773 6769 2061 7070  ploying wsgi app
+000017e0: 2c20 656e 7375 7265 2079 6f75 2068 6176  , ensure you hav
+000017f0: 6520 696e 7374 616c 6c65 6420 7468 6520  e installed the 
+00001800: 6465 7065 6e64 656e 6369 6573 2062 656c  dependencies bel
+00001810: 6f77 3a0a 6060 6062 6173 680a 7069 7020  ow:.```bash.pip 
+00001820: 696e 7374 616c 6c20 6661 7374 6170 6920  install fastapi 
+00001830: 7576 6963 6f72 6e20 6132 7773 6769 0a60  uvicorn a2wsgi.`
+00001840: 6060 0a0a 5468 656e 2070 7265 7061 7265  ``..Then prepare
+00001850: 2079 6f75 7220 7061 7373 656e 6765 7220   your passenger 
+00001860: 7773 6769 2061 7070 2061 6e64 206d 6169  wsgi app and mai
+00001870: 6e20 4661 7374 4150 4920 6170 7020 6173  n FastAPI app as
+00001880: 2062 656c 6f77 3a0a 0a23 2323 2320 7061   below:..#### pa
+00001890: 7373 656e 6765 725f 7773 6769 2e70 790a  ssenger_wsgi.py.
+000018a0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+000018b0: 206f 730a 696d 706f 7274 2073 7973 0a66   os.import sys.f
+000018c0: 726f 6d20 6132 7773 6769 2069 6d70 6f72  rom a2wsgi impor
+000018d0: 7420 4153 4749 4d69 6464 6c65 7761 7265  t ASGIMiddleware
+000018e0: 0a0a 2320 4164 6a75 7374 2074 6865 2070  ..# Adjust the p
+000018f0: 6174 6820 746f 2079 6f75 7220 4661 7374  ath to your Fast
+00001900: 4150 4920 6170 706c 6963 6174 696f 6e20  API application 
+00001910: 6469 7265 6374 6f72 7920 6966 206e 6565  directory if nee
+00001920: 6465 640a 6170 705f 6469 7220 3d20 6f73  ded.app_dir = os
+00001930: 2e70 6174 682e 6a6f 696e 286f 732e 7061  .path.join(os.pa
+00001940: 7468 2e64 6972 6e61 6d65 285f 5f66 696c  th.dirname(__fil
+00001950: 655f 5f29 2c20 2761 7070 2729 0a73 7973  e__), 'app').sys
+00001960: 2e70 6174 682e 696e 7365 7274 2830 2c20  .path.insert(0, 
+00001970: 6170 705f 6469 7229 0a0a 2320 496d 706f  app_dir)..# Impo
+00001980: 7274 2079 6f75 7220 4661 7374 4150 4920  rt your FastAPI 
+00001990: 6170 706c 6963 6174 696f 6e0a 6672 6f6d  application.from
+000019a0: 2061 7070 2e6d 6169 6e20 696d 706f 7274   app.main import
+000019b0: 2061 7070 2020 2320 4173 7375 6d69 6e67   app  # Assuming
+000019c0: 2079 6f75 7220 4661 7374 4150 4920 6170   your FastAPI ap
+000019d0: 7020 696e 7374 616e 6365 2069 7320 6e61  p instance is na
+000019e0: 6d65 6420 2761 7070 270a 0a23 2041 7070  med 'app'..# App
+000019f0: 6c69 6361 7469 6f6e 2063 616c 6c61 626c  lication callabl
+00001a00: 6520 666f 7220 5061 7373 656e 6765 7220  e for Passenger 
+00001a10: 5753 4749 0a64 6566 2061 7070 6c69 6361  WSGI.def applica
+00001a20: 7469 6f6e 2865 6e76 6972 6f6e 2c20 7374  tion(environ, st
+00001a30: 6172 745f 7265 7370 6f6e 7365 293a 0a20  art_response):. 
+00001a40: 2020 2072 6574 7572 6e20 4153 4749 4d69     return ASGIMi
+00001a50: 6464 6c65 7761 7265 2861 7070 2928 656e  ddleware(app)(en
+00001a60: 7669 726f 6e2c 2073 7461 7274 5f72 6573  viron, start_res
+00001a70: 706f 6e73 6529 0a60 6060 0a0a 2323 2323  ponse).```..####
+00001a80: 2061 7070 2f6d 6169 6e2e 7079 0a60 6060   app/main.py.```
+00001a90: 7079 7468 6f6e 0a66 726f 6d20 6661 7374  python.from fast
+00001aa0: 6170 692e 7265 7370 6f6e 7365 7320 696d  api.responses im
+00001ab0: 706f 7274 2052 6564 6972 6563 7452 6573  port RedirectRes
+00001ac0: 706f 6e73 650a 6672 6f6d 2069 6465 7261  ponse.from idera
+00001ad0: 7265 5f70 6865 6e6f 2e66 6869 725f 7061  re_pheno.fhir_pa
+00001ae0: 7273 6572 2069 6d70 6f72 7420 2a0a 0a40  rser import *..@
+00001af0: 6170 702e 6765 7428 222f 2229 0a61 7379  app.get("/").asy
+00001b00: 6e63 2064 6566 2077 656c 636f 6d65 2829  nc def welcome()
+00001b10: 3a0a 2020 2020 7265 7475 726e 2052 6564  :.    return Red
+00001b20: 6972 6563 7452 6573 706f 6e73 6528 7374  irectResponse(st
+00001b30: 6174 7573 5f63 6f64 653d 3330 322c 2075  atus_code=302, u
+00001b40: 726c 3d22 2f64 6f63 7322 290a 0a40 6170  rl="/docs")..@ap
+00001b50: 702e 6765 7428 222f 6865 616c 7468 2229  p.get("/health")
+00001b60: 0a61 7379 6e63 2064 6566 2068 6561 6c74  .async def healt
+00001b70: 6828 2920 2d3e 2052 6573 706f 6e73 6520  h() -> Response 
+00001b80: 3a0a 2020 2020 7265 7475 726e 207b 2273  :.    return {"s
+00001b90: 7461 7475 735f 636f 6465 2220 3a20 3230  tatus_code" : 20
+00001ba0: 302c 2022 6465 7461 696c 2220 3a20 2254  0, "detail" : "T
+00001bb0: 6865 2073 6572 7669 6365 7320 6973 2072  he services is r
+00001bc0: 756e 6e69 6e67 2c20 7472 7920 746f 2065  unning, try to e
+00001bd0: 7870 6c6f 7265 2074 6865 2041 5049 2066  xplore the API f
+00001be0: 726f 6d20 506f 7374 6d61 6e20 436f 6c6c  rom Postman Coll
+00001bf0: 6563 7469 6f6e 227d 0a0a 6966 205f 5f6e  ection"}..if __n
+00001c00: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
+00001c10: 5f5f 223a 0a20 2020 2069 6d70 6f72 7420  __":.    import 
+00001c20: 7576 6963 6f72 6e0a 2020 2020 7576 6963  uvicorn.    uvic
+00001c30: 6f72 6e2e 7275 6e28 6170 702c 2068 6f73  orn.run(app, hos
+00001c40: 743d 2230 2e30 2e30 2e30 222c 2070 6f72  t="0.0.0.0", por
+00001c50: 743d 3830 3030 290a 6060 600a 0a4e 6f77  t=8000).```..Now
+00001c60: 2079 6f75 2063 6f75 6c64 2061 6363 6573   you could acces
+00001c70: 7320 796f 7572 2068 7474 703a 2f2f 6c6f  s your http://lo
+00001c80: 6361 6c68 6f73 743a 3830 3030 2061 6e64  calhost:8000 and
+00001c90: 2072 6564 6972 6563 7465 6420 746f 2053   redirected to S
+00001ca0: 7761 6767 6572 2074 6f20 7365 6520 7468  wagger to see th
+00001cb0: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
+00001cc0: 6f66 2074 6865 2061 7661 696c 6162 6c65  of the available
+00001cd0: 2046 6173 7441 5049 2065 6e64 706f 696e   FastAPI endpoin
+00001ce0: 742e 2044 656d 6f20 6578 616d 706c 6520  t. Demo example 
+00001cf0: 636f 756c 6420 6265 2061 6363 6573 7365  could be accesse
+00001d00: 6420 7669 6120 506f 7374 6d61 6e20 436f  d via Postman Co
+00001d10: 6c6c 6563 7469 6f6e 2061 7420 5b68 6572  llection at [her
+00001d20: 655d 2868 7474 7073 3a2f 2f77 7777 2e70  e](https://www.p
+00001d30: 6f73 746d 616e 2e63 6f6d 2f69 7661 6e77  ostman.com/ivanw
+00001d40: 696c 6c69 616d 6861 7273 6f6e 6f2f 776f  illiamharsono/wo
+00001d50: 726b 7370 6163 652f 6964 6572 6172 652d  rkspace/iderare-
+00001d60: 7068 656e 6f2f 6f76 6572 7669 6577 290a  pheno/overview).
+00001d70: 0a0a 2323 2054 6561 6d0a 0a3c 212d 2d20  ..## Team..<!-- 
+00001d80: 7374 6172 7420 7465 616d 202d 2d3e 0a0a  start team -->..
+00001d90: 2a2a 6964 6572 6172 652d 7068 656e 6f2a  **iderare-pheno*
+00001da0: 2a20 6973 2064 6576 656c 6f70 6564 2061  * is developed a
+00001db0: 6e64 206d 6169 6e74 6169 6e65 6420 6279  nd maintained by
+00001dc0: 2074 6865 2061 7574 686f 7228 7329 2c20   the author(s), 
+00001dd0: 546f 206c 6561 726e 206d 6f72 6520 6162  To learn more ab
+00001de0: 6f75 7420 7768 6f20 7370 6563 6966 6963  out who specific
+00001df0: 616c 6c79 2063 6f6e 7472 6962 7574 6564  ally contributed
+00001e00: 2074 6f20 7468 6973 2063 6f64 6562 6173   to this codebas
+00001e10: 652c 2073 6565 205b 6f75 7220 636f 6e74  e, see [our cont
+00001e20: 7269 6275 746f 7273 5d28 6874 7470 733a  ributors](https:
+00001e30: 2f2f 6769 7468 7562 2e63 6f6d 2f69 7661  //github.com/iva
+00001e40: 6e77 696c 6c69 616d 6d64 2f69 6465 7261  nwilliammd/idera
+00001e50: 7265 2d70 6865 6e6f 2f67 7261 7068 732f  re-pheno/graphs/
+00001e60: 636f 6e74 7269 6275 746f 7273 2920 7061  contributors) pa
+00001e70: 6765 2e0a 0a3c 212d 2d20 656e 6420 7465  ge...<!-- end te
+00001e80: 616d 202d 2d3e 0a0a 2323 204c 6963 656e  am -->..## Licen
+00001e90: 7365 0a0a 3c21 2d2d 2073 7461 7274 206c  se..<!-- start l
+00001ea0: 6963 656e 7365 202d 2d3e 0a0a 2a2a 6964  icense -->..**id
+00001eb0: 6572 6172 652d 7068 656e 6f2a 2a20 6c69  erare-pheno** li
+00001ec0: 6365 6e73 6520 6973 2064 6572 6976 6564  cense is derived
+00001ed0: 2066 726f 6d20 5b49 4465 5261 7265 5d28   from [IDeRare](
+00001ee0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001ef0: 6f6d 2f69 7661 6e77 696c 6c69 616d 6d64  om/ivanwilliammd
+00001f00: 2f69 6465 7261 7265 290a 0a3c 212d 2d20  /iderare)..<!-- 
+00001f10: 656e 6420 6c69 6365 6e73 6520 2d2d 3e0a  end license -->.
```

### Comparing `iderare-pheno-0.5.0/iderare_pheno/converter.py` & `iderare_pheno-0.6.2/iderare_pheno/converter.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/phenotype/data/genes_to_phenotype.txt` & `iderare_pheno-0.6.2/iderare_pheno/phenotype/data/genes_to_phenotype.txt`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/phenotype/data/hp.obo` & `iderare_pheno-0.6.2/iderare_pheno/phenotype/data/hp.obo`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/phenotype/data/phenotype.hpoa` & `iderare_pheno-0.6.2/iderare_pheno/phenotype/data/phenotype.hpoa`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/icd102omim_subset.tsv` & `iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/icd102omim_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv` & `iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv` & `iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv` & `iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv` & `iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv` & `iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv` & `iderare_pheno-0.6.2/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/simrec.py` & `iderare_pheno-0.6.2/iderare_pheno/simrec.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/streamlit_utils.py` & `iderare_pheno-0.6.2/iderare_pheno/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/templates/template_iderare.yml` & `iderare_pheno-0.6.2/iderare_pheno/templates/template_iderare.yml`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno/utils.py` & `iderare_pheno-0.6.2/iderare_pheno/utils.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.5.0/iderare_pheno.egg-info/PKG-INFO` & `iderare_pheno-0.6.2/iderare_pheno.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.5.0
+Version: 0.6.2
 Author-email: Ivan William Harsono <ivanwilliam.md@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -48,46 +48,46 @@
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: hpo3
 Requires-Dist: scikit-learn
 Requires-Dist: pyyaml
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
-Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
+Requires-Dist: mypy<1.11,>=1.0; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
-Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev"
-Requires-Dist: furo==2024.1.29; extra == "dev"
+Requires-Dist: Sphinx<7.4.0,>=4.3.0; extra == "dev"
+Requires-Dist: furo==2024.4.27; extra == "dev"
 Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==1.23.3; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 
-# [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/)
+# [IDeRare-Pheno](https://pypi.org/project/iderare_pheno/)
 
 <p align="center">
     <a href="https://github.com/ivanwilliammd/iderare-pheno/actions">
         <img alt="CI" src="https://github.com/ivanwilliammd/iderare-pheno/workflows/Main/badge.svg">
     </a>
     <a href="https://pypi.org/project/iderare_pheno/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/iderare_pheno">
     </a>
-    <a href="https://iderare-pheno.readthedocs.io/en/latest/?badge=latest">
+<!--     <a href="https://iderare-pheno.readthedocs.io/en/latest/?badge=latest">
         <img src="https://readthedocs.org/projects/iderare-pheno/badge/?version=latest" alt="Documentation Status" />
-    </a>
+    </a> -->
     <a href="https://github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/github/license/ivanwilliammd/iderare-pheno.svg?color=blue&cachedrop">
     </a>
     <a href="https://bioinformatics-ivanwilliamharsono.streamlit.app/IDeRare_Pheno">
         <img alt="Streamlit" src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg">
     <br/>
 </p>
@@ -108,21 +108,20 @@
 <sup>g</sup>Bioinformatics Core Facilities - IMERI, Faculty of Medicine, Universitas Indonesia, Jalan Salemba Raya number 6, Jakarta, 10430, Indonesia .<br>
 <sup>h</sup>Department of Child Health, Dr. Cipto Mangunkusumo Hospital, Faculty of Medicine, University of Indonesia, Jakarta, Indonesia. <br>
 
 
 **Note:** Currently IDeRare paper is being considered journal submission. The citation will be updated once the paper is published.
 
 ## Quick links
-
-- [Documentation](https://iderare-pheno.readthedocs.io/)
+- [IDeRare full pipeline - Phenotype and Genotype](https://github.com/ivanwilliammd/IDeRare)
 - [PyPI Package](https://pypi.org/project/iderare-pheno/)
 - [License](https://github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE)
 - [Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb)
 - Interactive Webapps Implementation of at [Streamlit](https://bioinformatics-ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno)
-
+<!-- - [Documentation](https://iderare-pheno.readthedocs.io/) -->
 
 ## What does it do?
 
 This script is recommended if you would like to do conversion, linkage analysis, similarity scoring, and gene-disease recommendation based on the phenotype data provided at [clinical_data.txt](clinical_data.txt). Full feature : 
 1. Convert the phenotype data to HPO code (accept mixed SNOMED, LOINC, and HPO code)
 2. Similarity scoring of differential diagnosis
 3. Linkage analysis of differential diagnosis (accept mixed SNOMED, ICD-10, ORPHA, OMIM code), include dendrogram tree visualization.
@@ -172,18 +171,68 @@
 
 <!-- end install source -->
 
 ## Importing the library
 
 ```python
 from iderare_pheno.converter import term2omim, term2orpha, term2hpo, batchconvert
-from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation, hpo2name
+from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation, hpo2name, omim2name
 from iderare_pheno.utils import linkage_dendrogram, list2tsv, generate_yml
 ```
-As the complete readthedocs.io is still ongoing, please kindly refer to this [Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb)
+As the complete readthedocs.io is being finalized, please kindly refer to this [Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb)
+
+Note : for Streamlit implementation, use ```iderare_pheno.streamlit_utils``` instead of ```iderare_pheno.utils```, this was done to prevent file to automatically saving and showing dendrogram in Streamlit.
+```python
+from iderare_pheno.streamlit_utils import linkage_dendrogram, list2tsv, generate_yml
+```
+
+For Python FastAPI implementation and FHIR code extraction / parsing and deploying wsgi app, ensure you have installed the dependencies below:
+```bash
+pip install fastapi uvicorn a2wsgi
+```
+
+Then prepare your passenger wsgi app and main FastAPI app as below:
+
+#### passenger_wsgi.py
+```python
+import os
+import sys
+from a2wsgi import ASGIMiddleware
+
+# Adjust the path to your FastAPI application directory if needed
+app_dir = os.path.join(os.path.dirname(__file__), 'app')
+sys.path.insert(0, app_dir)
+
+# Import your FastAPI application
+from app.main import app  # Assuming your FastAPI app instance is named 'app'
+
+# Application callable for Passenger WSGI
+def application(environ, start_response):
+    return ASGIMiddleware(app)(environ, start_response)
+```
+
+#### app/main.py
+```python
+from fastapi.responses import RedirectResponse
+from iderare_pheno.fhir_parser import *
+
+@app.get("/")
+async def welcome():
+    return RedirectResponse(status_code=302, url="/docs")
+
+@app.get("/health")
+async def health() -> Response :
+    return {"status_code" : 200, "detail" : "The services is running, try to explore the API from Postman Collection"}
+
+if __name__ == "__main__":
+    import uvicorn
+    uvicorn.run(app, host="0.0.0.0", port=8000)
+```
+
+Now you could access your http://localhost:8000 and redirected to Swagger to see the documentation of the available FastAPI endpoint. Demo example could be accessed via Postman Collection at [here](https://www.postman.com/ivanwilliamharsono/workspace/iderare-pheno/overview)
 
 
 ## Team
 
 <!-- start team -->
 
 **iderare-pheno** is developed and maintained by the author(s), To learn more about who specifically contributed to this codebase, see [our contributors](https://github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.5.0 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.6.2 Author-email: Ivan
 William Harsono
 gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ivan William
 Harsono Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -27,28 +27,28 @@
 Audience :: Science/Research Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering
 :: Medical Science Apps. Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pandas Requires-Dist: numpy
 Requires-Dist: matplotlib Requires-Dist: scipy Requires-Dist: hpo3 Requires-
 Dist: scikit-learn Requires-Dist: pyyaml Provides-Extra: dev Requires-Dist:
-ruff; extra == "dev" Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-
+ruff; extra == "dev" Requires-Dist: mypy<1.11,>=1.0; extra == "dev" Requires-
 Dist: types-PyYAML; extra == "dev" Requires-Dist: black<25.0,>=23.0; extra ==
 "dev" Requires-Dist: black[jupyter]; extra == "dev" Requires-Dist:
 isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-cov; extra
 == "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist: build;
 extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist: wheel;
-extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-
-Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-parser<2.1,>=1.0;
+extra == "dev" Requires-Dist: Sphinx<7.4.0,>=4.3.0; extra == "dev" Requires-
+Dist: furo==2024.4.27; extra == "dev" Requires-Dist: myst-parser<2.1,>=1.0;
 extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev" Requires-Dist:
 sphinx-autodoc-typehints==1.23.3; extra == "dev" Requires-Dist: packaging;
-extra == "dev" # [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/)
-             _[_C_I_]_[_P_y_P_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_S_t_r_e_a_m_l_i_t_]
+extra == "dev" # [IDeRare-Pheno](https://pypi.org/project/iderare_pheno/)
+                        _[_C_I_]_[_P_y_P_I_]_[_L_i_c_e_n_s_e_]_[_S_t_r_e_a_m_l_i_t_]
 IDeRare or "Indonesia Exome Rare Disease Variant Discovery Pipeline" is a
 simple and ready to use variant discovery pipeline to discover rare disease
 variants from exome sequencing data. This repository is **the first part** of
 IDeRare workflow for **phenotype analysis**. For complete pipeline for
 _**phenotype-genotype analysis**_, kindly refer to [IDeRare Github repository]
 (https://github.com/ivanwilliammd/IDeRare). ## Authored by Ivan William
 Harsonoa, Yulia Arianib, Beben Benyaminc,d,e, Fadilah Fadilahf,g, Dwi Ari
@@ -65,47 +65,72 @@
 fDepartment of Medical Chemistry, Faculty of Medicine, Universitas Indonesia,
 Jalan Salemba Raya number 4, Jakarta, 10430, Indonesia.
 gBioinformatics Core Facilities - IMERI, Faculty of Medicine, Universitas
 Indonesia, Jalan Salemba Raya number 6, Jakarta, 10430, Indonesia .
 hDepartment of Child Health, Dr. Cipto Mangunkusumo Hospital, Faculty of
 Medicine, University of Indonesia, Jakarta, Indonesia.
 **Note:** Currently IDeRare paper is being considered journal submission. The
-citation will be updated once the paper is published. ## Quick links -
-[Documentation](https://iderare-pheno.readthedocs.io/) - [PyPI Package](https:/
-/pypi.org/project/iderare-pheno/) - [License](https://github.com/ivanwilliammd/
-iderare-pheno/blob/main/LICENSE) - [Interactive Playbook Example](https://
-github.com/ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb) - Interactive
-Webapps Implementation of at [Streamlit](https://bioinformatics-
-ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno) ## What does it do? This
-script is recommended if you would like to do conversion, linkage analysis,
-similarity scoring, and gene-disease recommendation based on the phenotype data
-provided at [clinical_data.txt](clinical_data.txt). Full feature : 1. Convert
-the phenotype data to HPO code (accept mixed SNOMED, LOINC, and HPO code) 2.
-Similarity scoring of differential diagnosis 3. Linkage analysis of
-differential diagnosis (accept mixed SNOMED, ICD-10, ORPHA, OMIM code), include
-dendrogram tree visualization. - This should help clinician to **systematically
-doing work-up and excluding similar diagnosis together** based on the
-patient\'s phenotype. 4. Gene and disease recommendation based on the phenotype
-data similarity scoring between **phenotype** and OMIM gene and disease
-databank. 5. Linkage analysis of recommended causative gene and disease based
-on phenotype data (include dendrogram tree visualization). - This should help
-clinician to **explore / enrich their differential diagnosis** based on the
-patient\'s phenotype. 6. Example of the clinical data provided at [Clinical
-Information Example section](#clinical-information-example) ## Installation
-**iderare-pheno** requires Python 3.8 or later. ### Installing with `pip`
-**iderare-pheno** is available [on PyPI](https://pypi.org/project/iderare-
-pheno/). Just run ```bash pip install iderare-pheno ``` ### Installing from
-source To install **iderare-pheno** from source, first clone [the repository]
-(https://github.com/ivanwilliammd/iderare-pheno): ```bash git clone https://
-github.com/ivanwilliammd/iderare-pheno.git cd iderare_pheno ``` Then run
-```bash pip install -e . ``` ## Importing the library ```python from
+citation will be updated once the paper is published. ## Quick links - [IDeRare
+full pipeline - Phenotype and Genotype](https://github.com/ivanwilliammd/
+IDeRare) - [PyPI Package](https://pypi.org/project/iderare-pheno/) - [License]
+(https://github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE) -
+[Interactive Playbook Example](https://github.com/ivanwilliammd/iderare-pheno/
+blob/main/Playbook.ipynb) - Interactive Webapps Implementation of at
+[Streamlit](https://bioinformatics-ivanwilliamharsono.streamlitapp.com/
+IDeRare_Pheno) ## What does it do? This script is recommended if you would like
+to do conversion, linkage analysis, similarity scoring, and gene-disease
+recommendation based on the phenotype data provided at [clinical_data.txt]
+(clinical_data.txt). Full feature : 1. Convert the phenotype data to HPO code
+(accept mixed SNOMED, LOINC, and HPO code) 2. Similarity scoring of
+differential diagnosis 3. Linkage analysis of differential diagnosis (accept
+mixed SNOMED, ICD-10, ORPHA, OMIM code), include dendrogram tree visualization.
+- This should help clinician to **systematically doing work-up and excluding
+similar diagnosis together** based on the patient\'s phenotype. 4. Gene and
+disease recommendation based on the phenotype data similarity scoring between
+**phenotype** and OMIM gene and disease databank. 5. Linkage analysis of
+recommended causative gene and disease based on phenotype data (include
+dendrogram tree visualization). - This should help clinician to **explore /
+enrich their differential diagnosis** based on the patient\'s phenotype. 6.
+Example of the clinical data provided at [Clinical Information Example section]
+(#clinical-information-example) ## Installation **iderare-pheno** requires
+Python 3.8 or later. ### Installing with `pip` **iderare-pheno** is available
+[on PyPI](https://pypi.org/project/iderare-pheno/). Just run ```bash pip
+install iderare-pheno ``` ### Installing from source To install **iderare-
+pheno** from source, first clone [the repository](https://github.com/
+ivanwilliammd/iderare-pheno): ```bash git clone https://github.com/
+ivanwilliammd/iderare-pheno.git cd iderare_pheno ``` Then run ```bash pip
+install -e . ``` ## Importing the library ```python from
 iderare_pheno.converter import term2omim, term2orpha, term2hpo, batchconvert
 from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation,
-hpo2name from iderare_pheno.utils import linkage_dendrogram, list2tsv,
-generate_yml ``` As the complete readthedocs.io is still ongoing, please kindly
-refer to this [Interactive Playbook Example](https://github.com/ivanwilliammd/
-iderare-pheno/blob/main/Playbook.ipynb) ## Team **iderare-pheno** is developed
-and maintained by the author(s), To learn more about who specifically
-contributed to this codebase, see [our contributors](https://github.com/
-ivanwilliammd/iderare-pheno/graphs/contributors) page. ## License **iderare-
-pheno** license is derived from [IDeRare](https://github.com/ivanwilliammd/
-iderare)
+hpo2name, omim2name from iderare_pheno.utils import linkage_dendrogram,
+list2tsv, generate_yml ``` As the complete readthedocs.io is being finalized,
+please kindly refer to this [Interactive Playbook Example](https://github.com/
+ivanwilliammd/iderare-pheno/blob/main/Playbook.ipynb) Note : for Streamlit
+implementation, use ```iderare_pheno.streamlit_utils``` instead of
+```iderare_pheno.utils```, this was done to prevent file to automatically
+saving and showing dendrogram in Streamlit. ```python from
+iderare_pheno.streamlit_utils import linkage_dendrogram, list2tsv, generate_yml
+``` For Python FastAPI implementation and FHIR code extraction / parsing and
+deploying wsgi app, ensure you have installed the dependencies below: ```bash
+pip install fastapi uvicorn a2wsgi ``` Then prepare your passenger wsgi app and
+main FastAPI app as below: #### passenger_wsgi.py ```python import os import
+sys from a2wsgi import ASGIMiddleware # Adjust the path to your FastAPI
+application directory if needed app_dir = os.path.join(os.path.dirname
+(__file__), 'app') sys.path.insert(0, app_dir) # Import your FastAPI
+application from app.main import app # Assuming your FastAPI app instance is
+named 'app' # Application callable for Passenger WSGI def application(environ,
+start_response): return ASGIMiddleware(app)(environ, start_response) ``` ####
+app/main.py ```python from fastapi.responses import RedirectResponse from
+iderare_pheno.fhir_parser import * @app.get("/") async def welcome(): return
+RedirectResponse(status_code=302, url="/docs") @app.get("/health") async def
+health() -> Response : return {"status_code" : 200, "detail" : "The services is
+running, try to explore the API from Postman Collection"} if __name__ ==
+"__main__": import uvicorn uvicorn.run(app, host="0.0.0.0", port=8000) ``` Now
+you could access your http://localhost:8000 and redirected to Swagger to see
+the documentation of the available FastAPI endpoint. Demo example could be
+accessed via Postman Collection at [here](https://www.postman.com/
+ivanwilliamharsono/workspace/iderare-pheno/overview) ## Team **iderare-pheno**
+is developed and maintained by the author(s), To learn more about who
+specifically contributed to this codebase, see [our contributors](https://
+github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page. ## License
+**iderare-pheno** license is derived from [IDeRare](https://github.com/
+ivanwilliammd/iderare)
```

### Comparing `iderare-pheno-0.5.0/iderare_pheno.egg-info/SOURCES.txt` & `iderare_pheno-0.6.2/iderare_pheno.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 iderare_pheno/__init__.py
 iderare_pheno/converter.py
+iderare_pheno/fhir_parser.py
 iderare_pheno/py.typed
 iderare_pheno/simrec.py
 iderare_pheno/streamlit_utils.py
 iderare_pheno/utils.py
 iderare_pheno/version.py
 iderare_pheno.egg-info/PKG-INFO
 iderare_pheno.egg-info/SOURCES.txt
```

### Comparing `iderare-pheno-0.5.0/pyproject.toml` & `iderare_pheno-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,28 +34,28 @@
 Repository = "https://github.com/ivanwilliammd/iderare-pheno"
 Changelog = "https://github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md"
 Documentation = "https://iderare-pheno.readthedocs.io/"
 
 [project.optional-dependencies]
 dev = [
     "ruff",
-    "mypy>=1.0,<1.10",
+    "mypy>=1.0,<1.11",
     "types-PyYAML",
     "black>=23.0,<25.0",
     "black[jupyter]",
     "isort>=5.12,<5.14",
     "pytest",
     "pytest-sphinx",
     "pytest-cov",
     "twine>=1.11.0",
     "build",
     "setuptools",
     "wheel",
-    "Sphinx>=4.3.0,<7.3.0",
-    "furo==2024.1.29",
+    "Sphinx>=4.3.0,<7.4.0",
+    "furo==2024.4.27",
     "myst-parser>=1.0,<2.1",
     "sphinx-copybutton==0.5.2",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.23.3",
     "packaging"
 ]
```

