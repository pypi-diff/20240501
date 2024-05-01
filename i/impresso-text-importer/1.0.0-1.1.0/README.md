# Comparing `tmp/impresso_text_importer-1.0.0.tar.gz` & `tmp/impresso_text_importer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impresso_text_importer-1.0.0.tar", last modified: Tue Dec 19 13:32:46 2023, max compression
+gzip compressed data, was "impresso_text_importer-1.1.0.tar", last modified: Wed May  1 09:32:05 2024, max compression
```

## Comparing `impresso_text_importer-1.0.0.tar` & `impresso_text_importer-1.1.0.tar`

### file list

```diff
@@ -1,106 +1,115 @@
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.909560 impresso_text_importer-1.0.0/
--rw-r--r--   0 piconti    (502) staff       (20)    34523 2023-11-15 16:15:53.000000 impresso_text_importer-1.0.0/LICENSE
--rw-r--r--   0 piconti    (502) staff       (20)    43366 2023-12-19 13:32:46.909337 impresso_text_importer-1.0.0/PKG-INFO
--rw-r--r--   0 piconti    (502) staff       (20)     2339 2023-12-19 13:31:05.000000 impresso_text_importer-1.0.0/README.md
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.905514 impresso_text_importer-1.0.0/impresso_text_importer.egg-info/
--rw-r--r--   0 piconti    (502) staff       (20)    43366 2023-12-19 13:32:46.000000 impresso_text_importer-1.0.0/impresso_text_importer.egg-info/PKG-INFO
--rw-r--r--   0 piconti    (502) staff       (20)     3363 2023-12-19 13:32:46.000000 impresso_text_importer-1.0.0/impresso_text_importer.egg-info/SOURCES.txt
--rw-r--r--   0 piconti    (502) staff       (20)        1 2023-12-19 13:32:46.000000 impresso_text_importer-1.0.0/impresso_text_importer.egg-info/dependency_links.txt
--rw-r--r--   0 piconti    (502) staff       (20)       87 2023-12-19 13:32:46.000000 impresso_text_importer-1.0.0/impresso_text_importer.egg-info/entry_points.txt
--rw-r--r--   0 piconti    (502) staff       (20)      107 2023-12-19 13:32:46.000000 impresso_text_importer-1.0.0/impresso_text_importer.egg-info/requires.txt
--rw-r--r--   0 piconti    (502) staff       (20)       14 2023-12-19 13:32:46.000000 impresso_text_importer-1.0.0/impresso_text_importer.egg-info/top_level.txt
--rw-r--r--   0 piconti    (502) staff       (20)     1650 2023-12-19 13:26:05.000000 impresso_text_importer-1.0.0/pyproject.toml
--rw-r--r--   0 piconti    (502) staff       (20)       38 2023-12-19 13:32:46.909634 impresso_text_importer-1.0.0/setup.cfg
--rw-r--r--   0 piconti    (502) staff       (20)       36 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/setup.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.888313 impresso_text_importer-1.0.0/tests/
--rw-r--r--   0 piconti    (502) staff       (20)      406 2023-10-12 13:38:49.000000 impresso_text_importer-1.0.0/tests/test_tokenization.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.889174 impresso_text_importer-1.0.0/text_importer/
--rw-r--r--   0 piconti    (502) staff       (20)       22 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/__init__.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.890506 impresso_text_importer-1.0.0/text_importer/importers/
--rw-r--r--   0 piconti    (502) staff       (20)      586 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/importers/__init__.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.891494 impresso_text_importer-1.0.0/text_importer/importers/bl/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/importers/bl/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)    10829 2023-12-19 13:24:25.000000 impresso_text_importer-1.0.0/text_importer/importers/bl/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)     8664 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/bl/detect.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.892652 impresso_text_importer-1.0.0/text_importer/importers/bnf/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/importers/bnf/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)    17147 2023-12-19 13:24:25.000000 impresso_text_importer-1.0.0/text_importer/importers/bnf/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)     8750 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/bnf/detect.py
--rw-r--r--   0 piconti    (502) staff       (20)     5301 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/bnf/helpers.py
--rw-r--r--   0 piconti    (502) staff       (20)     5938 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/bnf/parsers.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.893257 impresso_text_importer-1.0.0/text_importer/importers/bnf_en/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/importers/bnf_en/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)    15015 2023-12-19 13:24:25.000000 impresso_text_importer-1.0.0/text_importer/importers/bnf_en/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)    10736 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/bnf_en/detect.py
--rw-r--r--   0 piconti    (502) staff       (20)     7131 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)    19770 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/core.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.893895 impresso_text_importer-1.0.0/text_importer/importers/fedgaz/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/importers/fedgaz/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)    14820 2023-12-19 13:24:25.000000 impresso_text_importer-1.0.0/text_importer/importers/fedgaz/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)     8402 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/importers/fedgaz/show_canonical_boxes.py
--rw-r--r--   0 piconti    (502) staff       (20)    10112 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/generic_importer.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.895212 impresso_text_importer-1.0.0/text_importer/importers/lux/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/importers/lux/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)    25138 2023-12-19 13:24:25.000000 impresso_text_importer-1.0.0/text_importer/importers/lux/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)     4975 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/lux/detect.py
--rw-r--r--   0 piconti    (502) staff       (20)     4869 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/lux/helpers.py
--rw-r--r--   0 piconti    (502) staff       (20)     6789 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/importers/lux/test_dask_memory.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.896073 impresso_text_importer-1.0.0/text_importer/importers/mets_alto/
--rw-r--r--   0 piconti    (502) staff       (20)      169 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/importers/mets_alto/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)     5103 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/mets_alto/alto.py
--rw-r--r--   0 piconti    (502) staff       (20)     8177 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/mets_alto/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)     3673 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/mets_alto/mets.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.897306 impresso_text_importer-1.0.0/text_importer/importers/olive/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/importers/olive/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)    20253 2023-12-19 13:24:25.000000 impresso_text_importer-1.0.0/text_importer/importers/olive/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)     4100 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/olive/detect.py
--rw-r--r--   0 piconti    (502) staff       (20)    20319 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/olive/helpers.py
--rw-r--r--   0 piconti    (502) staff       (20)     8341 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/olive/parsers.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.897830 impresso_text_importer-1.0.0/text_importer/importers/onb_annop/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-12-15 09:14:25.000000 impresso_text_importer-1.0.0/text_importer/importers/onb_annop/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-12-15 09:14:32.000000 impresso_text_importer-1.0.0/text_importer/importers/onb_annop/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)     6678 2023-12-15 10:24:55.000000 impresso_text_importer-1.0.0/text_importer/importers/onb_annop/detect.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.898687 impresso_text_importer-1.0.0/text_importer/importers/rero/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/importers/rero/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)    19826 2023-12-19 13:24:25.000000 impresso_text_importer-1.0.0/text_importer/importers/rero/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)     5370 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/rero/detect.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.899350 impresso_text_importer-1.0.0/text_importer/importers/swa/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/importers/swa/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)     8189 2023-12-19 13:24:25.000000 impresso_text_importer-1.0.0/text_importer/importers/swa/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)     9313 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/importers/swa/detect.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.900903 impresso_text_importer-1.0.0/text_importer/importers/tetml/
--rw-r--r--   0 piconti    (502) staff       (20)       90 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/importers/tetml/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)     4659 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/importers/tetml/classes.py
--rw-r--r--   0 piconti    (502) staff       (20)     3554 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/importers/tetml/detect.py
--rw-r--r--   0 piconti    (502) staff       (20)    10289 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/importers/tetml/helpers.py
--rw-r--r--   0 piconti    (502) staff       (20)     5886 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/importers/tetml/parsers.py
--rw-r--r--   0 piconti    (502) staff       (20)    35091 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/importers/tetml/tetml2canonical.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.902052 impresso_text_importer-1.0.0/text_importer/impresso-schemas/
--rw-r--r--   0 piconti    (502) staff       (20)     1094 2023-09-06 15:35:23.000000 impresso_text_importer-1.0.0/text_importer/impresso-schemas/LICENSE
--rw-r--r--   0 piconti    (502) staff       (20)     1177 2023-09-06 15:35:23.000000 impresso_text_importer-1.0.0/text_importer/impresso-schemas/Makefile
--rw-r--r--   0 piconti    (502) staff       (20)     1188 2023-09-06 15:35:23.000000 impresso_text_importer-1.0.0/text_importer/impresso-schemas/README.md
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.886761 impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.902199 impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/linguistic_annotation/
--rw-r--r--   0 piconti    (502) staff       (20)     4645 2023-09-06 15:35:23.000000 impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/linguistic_annotation/ling_spacy.schema.json
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.902805 impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/newspaper/
--rw-r--r--   0 piconti    (502) staff       (20)     3508 2023-09-06 15:35:23.000000 impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/newspaper/contentitem.schema.json
--rw-r--r--   0 piconti    (502) staff       (20)     4461 2023-09-06 15:35:23.000000 impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/newspaper/issue.schema.json
--rw-r--r--   0 piconti    (502) staff       (20)     5053 2023-09-06 15:35:23.000000 impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/newspaper/page.schema.json
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.903094 impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/topic_model/
--rw-r--r--   0 piconti    (502) staff       (20)     1587 2023-09-06 15:35:23.000000 impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/topic_model/topic_assignment.schema.json
--rw-r--r--   0 piconti    (502) staff       (20)     1390 2023-09-06 15:35:23.000000 impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/topic_model/topic_description.schema.json
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2023-12-19 13:32:46.905308 impresso_text_importer-1.0.0/text_importer/scripts/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/scripts/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)      340 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/scripts/blimporter.py
--rw-r--r--   0 piconti    (502) staff       (20)      390 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/scripts/bnfen_importer.py
--rw-r--r--   0 piconti    (502) staff       (20)      380 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/scripts/bnfimporter.py
--rw-r--r--   0 piconti    (502) staff       (20)     8314 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/scripts/compress_canonical.py
--rw-r--r--   0 piconti    (502) staff       (20)      346 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/scripts/fedgazimporter.py
--rw-r--r--   0 piconti    (502) staff       (20)      348 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/scripts/luximporter.py
--rw-r--r--   0 piconti    (502) staff       (20)      412 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/scripts/oliveimporter.py
--rw-r--r--   0 piconti    (502) staff       (20)      356 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/scripts/reroimporter.py
--rw-r--r--   0 piconti    (502) staff       (20)      348 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/scripts/swaimporter.py
--rw-r--r--   0 piconti    (502) staff       (20)      343 2023-11-15 16:15:54.000000 impresso_text_importer-1.0.0/text_importer/scripts/tetmlimporter.py
--rw-r--r--   0 piconti    (502) staff       (20)     4230 2023-09-06 15:35:22.000000 impresso_text_importer-1.0.0/text_importer/scripts/upload.py
--rw-r--r--   0 piconti    (502) staff       (20)     1817 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/tokenization.py
--rw-r--r--   0 piconti    (502) staff       (20)     6002 2023-12-19 12:48:18.000000 impresso_text_importer-1.0.0/text_importer/utils.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.082597 impresso_text_importer-1.1.0/
+-rw-r--r--   0 piconti    (502) staff       (20)    34523 2023-11-15 16:15:53.000000 impresso_text_importer-1.1.0/LICENSE
+-rw-r--r--   0 piconti    (502) staff       (20)    43405 2024-05-01 09:32:05.082365 impresso_text_importer-1.1.0/PKG-INFO
+-rw-r--r--   0 piconti    (502) staff       (20)     2339 2024-04-30 12:10:12.000000 impresso_text_importer-1.1.0/README.md
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.080735 impresso_text_importer-1.1.0/impresso_text_importer.egg-info/
+-rw-r--r--   0 piconti    (502) staff       (20)    43405 2024-05-01 09:32:05.000000 impresso_text_importer-1.1.0/impresso_text_importer.egg-info/PKG-INFO
+-rw-r--r--   0 piconti    (502) staff       (20)     3724 2024-05-01 09:32:05.000000 impresso_text_importer-1.1.0/impresso_text_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 piconti    (502) staff       (20)        1 2024-05-01 09:32:05.000000 impresso_text_importer-1.1.0/impresso_text_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 piconti    (502) staff       (20)       87 2024-05-01 09:32:05.000000 impresso_text_importer-1.1.0/impresso_text_importer.egg-info/entry_points.txt
+-rw-r--r--   0 piconti    (502) staff       (20)      107 2024-05-01 09:32:05.000000 impresso_text_importer-1.1.0/impresso_text_importer.egg-info/requires.txt
+-rw-r--r--   0 piconti    (502) staff       (20)       14 2024-05-01 09:32:05.000000 impresso_text_importer-1.1.0/impresso_text_importer.egg-info/top_level.txt
+-rw-r--r--   0 piconti    (502) staff       (20)     1709 2024-05-01 08:39:12.000000 impresso_text_importer-1.1.0/pyproject.toml
+-rw-r--r--   0 piconti    (502) staff       (20)       38 2024-05-01 09:32:05.082637 impresso_text_importer-1.1.0/setup.cfg
+-rw-r--r--   0 piconti    (502) staff       (20)       36 2023-12-19 12:48:18.000000 impresso_text_importer-1.1.0/setup.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.059133 impresso_text_importer-1.1.0/tests/
+-rw-r--r--   0 piconti    (502) staff       (20)      406 2023-10-12 13:38:49.000000 impresso_text_importer-1.1.0/tests/test_tokenization.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.060393 impresso_text_importer-1.1.0/text_importer/
+-rw-r--r--   0 piconti    (502) staff       (20)       22 2024-04-30 12:29:32.000000 impresso_text_importer-1.1.0/text_importer/__init__.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.062007 impresso_text_importer-1.1.0/text_importer/importers/
+-rw-r--r--   0 piconti    (502) staff       (20)      586 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/importers/__init__.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.062756 impresso_text_importer-1.1.0/text_importer/importers/bl/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/importers/bl/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)    10851 2024-03-12 10:38:40.000000 impresso_text_importer-1.1.0/text_importer/importers/bl/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)     8329 2024-03-12 11:18:38.000000 impresso_text_importer-1.1.0/text_importer/importers/bl/detect.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.064386 impresso_text_importer-1.1.0/text_importer/importers/bnf/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/importers/bnf/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)    16855 2024-03-12 11:16:03.000000 impresso_text_importer-1.1.0/text_importer/importers/bnf/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)     8506 2024-04-29 16:35:42.000000 impresso_text_importer-1.1.0/text_importer/importers/bnf/detect.py
+-rw-r--r--   0 piconti    (502) staff       (20)     5260 2024-04-29 15:01:15.000000 impresso_text_importer-1.1.0/text_importer/importers/bnf/helpers.py
+-rw-r--r--   0 piconti    (502) staff       (20)     5545 2024-04-29 16:02:30.000000 impresso_text_importer-1.1.0/text_importer/importers/bnf/parsers.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.065072 impresso_text_importer-1.1.0/text_importer/importers/bnf_en/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/importers/bnf_en/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)    15004 2024-04-29 16:02:52.000000 impresso_text_importer-1.1.0/text_importer/importers/bnf_en/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)    15369 2024-04-29 13:54:21.000000 impresso_text_importer-1.1.0/text_importer/importers/bnf_en/detect.py
+-rw-r--r--   0 piconti    (502) staff       (20)     7002 2024-04-30 08:33:57.000000 impresso_text_importer-1.1.0/text_importer/importers/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)    21841 2024-04-30 08:33:54.000000 impresso_text_importer-1.1.0/text_importer/importers/core.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.065960 impresso_text_importer-1.1.0/text_importer/importers/fedgaz/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/importers/fedgaz/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)    15061 2024-04-29 15:25:59.000000 impresso_text_importer-1.1.0/text_importer/importers/fedgaz/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)     8402 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/importers/fedgaz/show_canonical_boxes.py
+-rw-r--r--   0 piconti    (502) staff       (20)    11084 2024-04-30 08:33:44.000000 impresso_text_importer-1.1.0/text_importer/importers/generic_importer.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.067399 impresso_text_importer-1.1.0/text_importer/importers/lux/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/importers/lux/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)    23383 2024-03-11 17:34:16.000000 impresso_text_importer-1.1.0/text_importer/importers/lux/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)     4873 2024-03-12 17:36:03.000000 impresso_text_importer-1.1.0/text_importer/importers/lux/detect.py
+-rw-r--r--   0 piconti    (502) staff       (20)     4831 2024-03-12 17:35:38.000000 impresso_text_importer-1.1.0/text_importer/importers/lux/helpers.py
+-rw-r--r--   0 piconti    (502) staff       (20)     6789 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/importers/lux/test_dask_memory.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.068481 impresso_text_importer-1.1.0/text_importer/importers/mets_alto/
+-rw-r--r--   0 piconti    (502) staff       (20)      169 2024-01-04 14:17:52.000000 impresso_text_importer-1.1.0/text_importer/importers/mets_alto/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)     4835 2024-03-12 17:32:51.000000 impresso_text_importer-1.1.0/text_importer/importers/mets_alto/alto.py
+-rw-r--r--   0 piconti    (502) staff       (20)     8178 2024-03-11 17:18:03.000000 impresso_text_importer-1.1.0/text_importer/importers/mets_alto/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)     3661 2024-04-29 15:35:11.000000 impresso_text_importer-1.1.0/text_importer/importers/mets_alto/mets.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.070088 impresso_text_importer-1.1.0/text_importer/importers/olive/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/importers/olive/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)    19243 2024-04-29 15:39:25.000000 impresso_text_importer-1.1.0/text_importer/importers/olive/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)     3976 2024-04-29 15:40:02.000000 impresso_text_importer-1.1.0/text_importer/importers/olive/detect.py
+-rw-r--r--   0 piconti    (502) staff       (20)    19528 2024-04-29 15:50:37.000000 impresso_text_importer-1.1.0/text_importer/importers/olive/helpers.py
+-rw-r--r--   0 piconti    (502) staff       (20)     8117 2024-04-29 15:50:30.000000 impresso_text_importer-1.1.0/text_importer/importers/olive/parsers.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.070559 impresso_text_importer-1.1.0/text_importer/importers/onb_annop/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-12-15 09:14:25.000000 impresso_text_importer-1.1.0/text_importer/importers/onb_annop/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-12-15 09:14:32.000000 impresso_text_importer-1.1.0/text_importer/importers/onb_annop/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)     6678 2023-12-15 10:24:55.000000 impresso_text_importer-1.1.0/text_importer/importers/onb_annop/detect.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.071558 impresso_text_importer-1.1.0/text_importer/importers/rero/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/importers/rero/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)    19711 2024-04-29 16:25:42.000000 impresso_text_importer-1.1.0/text_importer/importers/rero/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)     5272 2024-04-29 16:26:58.000000 impresso_text_importer-1.1.0/text_importer/importers/rero/detect.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.072244 impresso_text_importer-1.1.0/text_importer/importers/swa/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/importers/swa/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)     8311 2024-04-29 16:27:13.000000 impresso_text_importer-1.1.0/text_importer/importers/swa/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)     9262 2024-04-29 16:33:55.000000 impresso_text_importer-1.1.0/text_importer/importers/swa/detect.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.073760 impresso_text_importer-1.1.0/text_importer/importers/tetml/
+-rw-r--r--   0 piconti    (502) staff       (20)       90 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/importers/tetml/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)     4923 2024-03-11 17:55:35.000000 impresso_text_importer-1.1.0/text_importer/importers/tetml/classes.py
+-rw-r--r--   0 piconti    (502) staff       (20)     3554 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/importers/tetml/detect.py
+-rw-r--r--   0 piconti    (502) staff       (20)    10289 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/importers/tetml/helpers.py
+-rw-r--r--   0 piconti    (502) staff       (20)     5886 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/importers/tetml/parsers.py
+-rw-r--r--   0 piconti    (502) staff       (20)    35091 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/importers/tetml/tetml2canonical.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.075778 impresso_text_importer-1.1.0/text_importer/impresso-schemas/
+-rw-r--r--   0 piconti    (502) staff       (20)    34523 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/LICENSE
+-rw-r--r--   0 piconti    (502) staff       (20)     3200 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/Makefile
+-rw-r--r--   0 piconti    (502) staff       (20)      156 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/Pipfile
+-rw-r--r--   0 piconti    (502) staff       (20)     1538 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/Pipfile.lock
+-rw-r--r--   0 piconti    (502) staff       (20)     2721 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/README.md
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.057655 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.075992 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/entities/
+-rw-r--r--   0 piconti    (502) staff       (20)     5414 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/entities/entities.schema.json
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.076293 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/language_identification/
+-rw-r--r--   0 piconti    (502) staff       (20)     6296 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/language_identification/language_identification.schema.json
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.076516 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/linguistic_annotation/
+-rw-r--r--   0 piconti    (502) staff       (20)     4645 2023-09-06 15:35:23.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/linguistic_annotation/ling_spacy.schema.json
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.077252 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/newspaper/
+-rw-r--r--   0 piconti    (502) staff       (20)     3663 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/newspaper/contentitem.schema.json
+-rw-r--r--   0 piconti    (502) staff       (20)     5407 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/newspaper/issue.schema.json
+-rw-r--r--   0 piconti    (502) staff       (20)     6742 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/newspaper/page.schema.json
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.077659 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/topic_model/
+-rw-r--r--   0 piconti    (502) staff       (20)     1587 2023-09-06 15:35:23.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/topic_model/topic_assignment.schema.json
+-rw-r--r--   0 piconti    (502) staff       (20)     1390 2023-09-06 15:35:23.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/topic_model/topic_description.schema.json
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.077883 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/versioning/
+-rw-r--r--   0 piconti    (502) staff       (20)    10424 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/versioning/manifest.schema.json
+-rw-r--r--   0 piconti    (502) staff       (20)      106 2024-02-26 15:53:53.000000 impresso_text_importer-1.1.0/text_importer/impresso-schemas/requirements.txt
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-01 09:32:05.080507 impresso_text_importer-1.1.0/text_importer/scripts/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/scripts/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)      340 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/scripts/blimporter.py
+-rw-r--r--   0 piconti    (502) staff       (20)      390 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/scripts/bnfen_importer.py
+-rw-r--r--   0 piconti    (502) staff       (20)      380 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/scripts/bnfimporter.py
+-rw-r--r--   0 piconti    (502) staff       (20)     8314 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/scripts/compress_canonical.py
+-rw-r--r--   0 piconti    (502) staff       (20)      346 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/scripts/fedgazimporter.py
+-rw-r--r--   0 piconti    (502) staff       (20)      348 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/scripts/luximporter.py
+-rw-r--r--   0 piconti    (502) staff       (20)      412 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/scripts/oliveimporter.py
+-rw-r--r--   0 piconti    (502) staff       (20)      356 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/scripts/reroimporter.py
+-rw-r--r--   0 piconti    (502) staff       (20)      348 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/scripts/swaimporter.py
+-rw-r--r--   0 piconti    (502) staff       (20)      343 2023-11-15 16:15:54.000000 impresso_text_importer-1.1.0/text_importer/scripts/tetmlimporter.py
+-rw-r--r--   0 piconti    (502) staff       (20)     4230 2023-09-06 15:35:22.000000 impresso_text_importer-1.1.0/text_importer/scripts/upload.py
+-rw-r--r--   0 piconti    (502) staff       (20)     1817 2024-02-27 17:30:52.000000 impresso_text_importer-1.1.0/text_importer/tokenization.py
+-rw-r--r--   0 piconti    (502) staff       (20)    10476 2024-04-30 08:51:11.000000 impresso_text_importer-1.1.0/text_importer/utils.py
```

### Comparing `impresso_text_importer-1.0.0/LICENSE` & `impresso_text_importer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/PKG-INFO` & `impresso_text_importer-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: impresso_text_importer
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library to import newspaper data from a variety of OCR formats into Impresso's JSON format.
-Author-email: Maud Ehrmann <maud.ehrmann@epfl.ch>, Matteo Romanello <matteo.romanello@gmail.com>
+Author-email: Maud Ehrmann <maud.ehrmann@epfl.ch>, Matteo Romanello <matteo.romanello@gmail.com>, Pauline Conti <pauline.conti@epfl.ch>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -708,12 +708,12 @@
 
 ## License
 
 The second project 'impresso - Media Monitoring of the Past II. Beyond Borders: Connecting Historical Newspapers and Radio' is funded by the Swiss National Science Foundation (SNSF) under grant number [CRSII5_213585](https://data.snf.ch/grants/grant/213585) and the Luxembourg National Research Fund under grant No. 17498891.
 
 Aiming to develop and consolidate tools to process and explore large-scale collections of historical newspapers and radio archives, and to study the impact of this tooling on historical research practices, _Impresso II_ builds upon the first project – 'impresso - Media Monitoring of the Past' (grant number [CRSII5_173719](http://p3.snf.ch/project-173719), Sinergia program). More information at https://impresso-project.ch.
 
-Copyright (C) 2023  The *impresso* team (contributors to this program: Matteo Romanello, Maud Ehrmann, Alex Flückinger, Edoardo Tarek Hölzl, Pauline Conti).
+Copyright (C) 2024  The *impresso* team (contributors to this program: Matteo Romanello, Maud Ehrmann, Alex Flückinger, Edoardo Tarek Hölzl, Pauline Conti).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of merchantability or fitness for a particular purpose. See the [GNU Affero General Public License](https://github.com/impresso/impresso-text-acquisition/blob/master/LICENSE) for more details.
```

### Comparing `impresso_text_importer-1.0.0/README.md` & `impresso_text_importer-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 
 ## License
 
 The second project 'impresso - Media Monitoring of the Past II. Beyond Borders: Connecting Historical Newspapers and Radio' is funded by the Swiss National Science Foundation (SNSF) under grant number [CRSII5_213585](https://data.snf.ch/grants/grant/213585) and the Luxembourg National Research Fund under grant No. 17498891.
 
 Aiming to develop and consolidate tools to process and explore large-scale collections of historical newspapers and radio archives, and to study the impact of this tooling on historical research practices, _Impresso II_ builds upon the first project – 'impresso - Media Monitoring of the Past' (grant number [CRSII5_173719](http://p3.snf.ch/project-173719), Sinergia program). More information at https://impresso-project.ch.
 
-Copyright (C) 2023  The *impresso* team (contributors to this program: Matteo Romanello, Maud Ehrmann, Alex Flückinger, Edoardo Tarek Hölzl, Pauline Conti).
+Copyright (C) 2024  The *impresso* team (contributors to this program: Matteo Romanello, Maud Ehrmann, Alex Flückinger, Edoardo Tarek Hölzl, Pauline Conti).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of merchantability or fitness for a particular purpose. See the [GNU Affero General Public License](https://github.com/impresso/impresso-text-acquisition/blob/master/LICENSE) for more details.
```

### Comparing `impresso_text_importer-1.0.0/impresso_text_importer.egg-info/PKG-INFO` & `impresso_text_importer-1.1.0/impresso_text_importer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: impresso-text-importer
-Version: 1.0.0
+Name: impresso_text_importer
+Version: 1.1.0
 Summary: Library to import newspaper data from a variety of OCR formats into Impresso's JSON format.
-Author-email: Maud Ehrmann <maud.ehrmann@epfl.ch>, Matteo Romanello <matteo.romanello@gmail.com>
+Author-email: Maud Ehrmann <maud.ehrmann@epfl.ch>, Matteo Romanello <matteo.romanello@gmail.com>, Pauline Conti <pauline.conti@epfl.ch>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -708,12 +708,12 @@
 
 ## License
 
 The second project 'impresso - Media Monitoring of the Past II. Beyond Borders: Connecting Historical Newspapers and Radio' is funded by the Swiss National Science Foundation (SNSF) under grant number [CRSII5_213585](https://data.snf.ch/grants/grant/213585) and the Luxembourg National Research Fund under grant No. 17498891.
 
 Aiming to develop and consolidate tools to process and explore large-scale collections of historical newspapers and radio archives, and to study the impact of this tooling on historical research practices, _Impresso II_ builds upon the first project – 'impresso - Media Monitoring of the Past' (grant number [CRSII5_173719](http://p3.snf.ch/project-173719), Sinergia program). More information at https://impresso-project.ch.
 
-Copyright (C) 2023  The *impresso* team (contributors to this program: Matteo Romanello, Maud Ehrmann, Alex Flückinger, Edoardo Tarek Hölzl, Pauline Conti).
+Copyright (C) 2024  The *impresso* team (contributors to this program: Matteo Romanello, Maud Ehrmann, Alex Flückinger, Edoardo Tarek Hölzl, Pauline Conti).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of merchantability or fitness for a particular purpose. See the [GNU Affero General Public License](https://github.com/impresso/impresso-text-acquisition/blob/master/LICENSE) for more details.
```

### Comparing `impresso_text_importer-1.0.0/impresso_text_importer.egg-info/SOURCES.txt` & `impresso_text_importer-1.1.0/impresso_text_importer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -57,21 +57,27 @@
 text_importer/importers/tetml/classes.py
 text_importer/importers/tetml/detect.py
 text_importer/importers/tetml/helpers.py
 text_importer/importers/tetml/parsers.py
 text_importer/importers/tetml/tetml2canonical.py
 text_importer/impresso-schemas/LICENSE
 text_importer/impresso-schemas/Makefile
+text_importer/impresso-schemas/Pipfile
+text_importer/impresso-schemas/Pipfile.lock
 text_importer/impresso-schemas/README.md
+text_importer/impresso-schemas/requirements.txt
+text_importer/impresso-schemas/json/entities/entities.schema.json
+text_importer/impresso-schemas/json/language_identification/language_identification.schema.json
 text_importer/impresso-schemas/json/linguistic_annotation/ling_spacy.schema.json
 text_importer/impresso-schemas/json/newspaper/contentitem.schema.json
 text_importer/impresso-schemas/json/newspaper/issue.schema.json
 text_importer/impresso-schemas/json/newspaper/page.schema.json
 text_importer/impresso-schemas/json/topic_model/topic_assignment.schema.json
 text_importer/impresso-schemas/json/topic_model/topic_description.schema.json
+text_importer/impresso-schemas/json/versioning/manifest.schema.json
 text_importer/scripts/__init__.py
 text_importer/scripts/blimporter.py
 text_importer/scripts/bnfen_importer.py
 text_importer/scripts/bnfimporter.py
 text_importer/scripts/compress_canonical.py
 text_importer/scripts/fedgazimporter.py
 text_importer/scripts/luximporter.py
```

### Comparing `impresso_text_importer-1.0.0/pyproject.toml` & `impresso_text_importer-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "impresso_text_importer"
 authors = [
     {name="Maud Ehrmann", email="maud.ehrmann@epfl.ch"},
-    {name="Matteo Romanello", email="matteo.romanello@gmail.com"}
+    {name="Matteo Romanello", email="matteo.romanello@gmail.com"},
+    {name="Pauline Conti", email="pauline.conti@epfl.ch"}
 ]
 description = "Library to import newspaper data from a variety of OCR formats into Impresso's JSON format."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/__init__.py` & `impresso_text_importer-1.1.0/text_importer/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/bl/classes.py` & `impresso_text_importer-1.1.0/text_importer/importers/bl/classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,40 +7,46 @@
 
 import logging
 import os
 from time import strftime
 from typing import Any
 
 from bs4.element import Tag
-from text_importer.importers import (CONTENTITEM_TYPES, CONTENTITEM_TYPE_IMAGE, CONTENTITEM_TYPE_ADVERTISEMENT)
-from text_importer.importers.mets_alto import (MetsAltoNewspaperIssue,
-                                               MetsAltoNewspaperPage)
-from text_importer.utils import get_issue_schema, get_page_schema
+from text_importer.importers import (
+    CONTENTITEM_TYPES,
+    CONTENTITEM_TYPE_IMAGE,
+    CONTENTITEM_TYPE_ADVERTISEMENT,
+)
+from text_importer.importers.mets_alto import (
+    MetsAltoNewspaperIssue,
+    MetsAltoNewspaperPage,
+)
+from text_importer.utils import get_issue_schema, get_page_schema, get_reading_order
 
 IssueSchema = get_issue_schema()
 Pageschema = get_page_schema()
 
 logger = logging.getLogger(__name__)
 
-IIIF_ENDPOINT_URL = "https://impresso-project.ch/api/proxy/iiif/"
+IIIF_ENDPOINT_URI = "https://impresso-project.ch/api/proxy/iiif/"
 
 BL_PICTURE_TYPE = "picture"
 BL_AD_TYPE = "advert"
 
 
 class BlNewspaperPage(MetsAltoNewspaperPage):
     """Newspaper page in BL (Mets/Alto) format.
 
     Args:
         _id (str): Canonical page ID.
         number (int): Page number.
         filename (str): Name of the Alto XML page file.
         basedir (str): Base directory where Alto files are located.
         encoding (str, optional): Encoding of XML file. Defaults to 'utf-8'.
-    
+
     Attributes:
         id (str): Canonical Page ID (e.g. ``GDL-1900-01-02-a-p0004``).
         number (int): Page number.
         page_data (dict[str, Any]): Page data according to canonical format.
         issue (NewspaperIssue): Issue this page is from.
         filename (str): Name of the Alto XML page file.
         basedir (str): Base directory where Alto files are located.
@@ -50,21 +56,21 @@
     def add_issue(self, issue: MetsAltoNewspaperIssue) -> None:
         """Add the given `BlNewspaperIssue` as an attribute for this class.
 
         Args:
             issue (MetsAltoNewspaperIssue): Issue this page is from
         """
         self.issue = issue
-        self.page_data['iiif'] = os.path.join(IIIF_ENDPOINT_URL, self.id)
+        self.page_data["iiif_img_base_uri"] = os.path.join(IIIF_ENDPOINT_URI, self.id)
 
 
 class BlNewspaperIssue(MetsAltoNewspaperIssue):
     """Newspaper Issue in BL (Mets/Alto) format.
 
-    All functions defined in this child class are specific to parsing BL 
+    All functions defined in this child class are specific to parsing BL
     Mets/Alto format.
 
     Args:
         issue_dir (IssueDir): Identifying information about the issue.
 
     Attributes:
         id (str): Canonical Issue ID (e.g. ``GDL-1900-01-02-a``).
@@ -76,212 +82,229 @@
         pages (list): list of :obj:`NewspaperPage` instances from this issue.
         rights (str): Access rights applicable to this issue.
         image_properties (dict[str, Any]): metadata allowing to convert region
             OCR/OLR coordinates to iiif format compliant ones.
         ark_id (int): Issue ARK identifier, for the issue's pages' iiif links.
     """
 
-    
     def _find_pages(self) -> None:
         """Detect and create the issue pages using the relevant Alto XML files.
 
         Created `BlNewspaperPage` instances are added to the `pages` attribute.
 
         Raises:
             e: Creating a `BlNewspaperPage` raised an exception.
         """
         page_file_names = [
-            file for file in os.listdir(self.path)
-            if (not file.startswith('.') and 
-                '.xml' in file and 
-                'mets' not in file)
+            file
+            for file in os.listdir(self.path)
+            if (not file.startswith(".") and ".xml" in file and "mets" not in file)
         ]
         page_numbers = [
-            int(os.path.splitext(fname)[0].split('_')[-1]) 
-            for fname in page_file_names
+            int(os.path.splitext(fname)[0].split("_")[-1]) for fname in page_file_names
         ]
-        
+
         page_canonical_names = [
-            "{}-p{}".format(self.id, str(page_n).zfill(4)) 
-            for page_n in page_numbers
+            "{}-p{}".format(self.id, str(page_n).zfill(4)) for page_n in page_numbers
         ]
-        
+
         self.pages = []
-        for filename, page_no, page_id in zip(page_file_names, page_numbers, 
-                                              page_canonical_names):
+        for filename, page_no, page_id in zip(
+            page_file_names, page_numbers, page_canonical_names
+        ):
             try:
-                self.pages.append(BlNewspaperPage(page_id, page_no, 
-                                                  filename, self.path))
+                self.pages.append(
+                    BlNewspaperPage(page_id, page_no, filename, self.path)
+                )
             except Exception as e:
-                logger.error(f'Adding page {page_no} {page_id} {filename}',
-                             f'raised following exception: {e}')
+                msg = (
+                    f"Adding page {page_no} {page_id} {filename}",
+                    f"raised following exception: {e}",
+                )
+                logger.error(msg)
                 raise e
-    
-    def _get_part_dict(self, div: Tag, comp_role: str | None) -> dict[str,Any]:
+
+    def _get_part_dict(self, div: Tag, comp_role: str | None) -> dict[str, Any]:
         """Construct the parts for a certain div entry of METS.
 
         Args:
             div (Tag): Content item div
             comp_role (str | None): Role of the component
 
         Returns:
             dict[str, Any]: Parts dict for given div.
         """
-        comp_fileid = div.find('area', {'BETYPE': 'IDREF'}).get('FILEID')
-        comp_id = div.get('ID')
-        comp_page_no = int(div.parent.get('ORDER'))
+        comp_fileid = div.find("area", {"BETYPE": "IDREF"}).get("FILEID")
+        comp_id = div.get("ID")
+        comp_page_no = int(div.parent.get("ORDER"))
         if comp_role is None:
-            type_attr = div.get('TYPE')
+            type_attr = div.get("TYPE")
             comp_role = type_attr.lower() if type_attr else None
 
         return {
-            'comp_role': comp_role, 
-            'comp_id': comp_id, 
-            'comp_fileid': comp_fileid, 
-            'comp_page_no': int(comp_page_no)
+            "comp_role": comp_role,
+            "comp_id": comp_id,
+            "comp_fileid": comp_fileid,
+            "comp_page_no": int(comp_page_no),
         }
-    
+
     def _parse_content_parts(
         self, item_div: Tag, phys_map: Tag, structlink: Tag
-    ) -> list[dict[str,Any]]:
+    ) -> list[dict[str, Any]]:
         """Parse parts of issue's physical structure relating to the given item.
 
         Args:
             item_div (Tag): The div corresponding to the item
             phys_map (Tag): The physical structure of the Issue
             structlink (Tag): The structlink element of Mets file.
 
         Returns:
             list[dict[str, Any]]: List of dicts of each content part of item.
         """
         # Find all parts and their IDS
         tag = f"#{item_div.get('ID')}"
-        linkgrp = structlink.find('smLocatorLink', {'xlink:href': tag}).parent
-        
+        linkgrp = structlink.find("smLocatorLink", {"xlink:href": tag}).parent
+
         # Remove `#` from xlink:href
         parts_ids = [
-            x.get('xlink:href')[1:] for x in linkgrp.findAll('smLocatorLink') 
-            if x.get('xlink:href') != tag
+            x.get("xlink:href")[1:]
+            for x in linkgrp.findAll("smLocatorLink")
+            if x.get("xlink:href") != tag
         ]
         parts = []
         for p in parts_ids:
             # Get element in physical map
-            div = phys_map.find('div', {'ID': p})  
-            type_attr = div.get('TYPE')
+            div = phys_map.find("div", {"ID": p})
+            type_attr = div.get("TYPE")
             comp_role = type_attr.lower() if type_attr else None
-            
+
             # In that case, need to add all parts
-            if comp_role == 'page':  
-                for x in div.findAll('div'):
+            if comp_role == "page":
+                for x in div.findAll("div"):
                     parts.append(self._get_part_dict(x, None))
             else:
                 parts.append(self._get_part_dict(div, comp_role))
-        
-        return parts
 
-    def _parse_content_item(self, item_div: Tag, counter: int, 
-                            phys_structmap: Tag, structlink: Tag, 
-                            item_dmd_sec: Tag) -> dict[str, Any]:
+        return parts
 
+    def _parse_content_item(
+        self,
+        item_div: Tag,
+        counter: int,
+        phys_structmap: Tag,
+        structlink: Tag,
+        item_dmd_sec: Tag,
+    ) -> dict[str, Any]:
         """Parse the given content item.
-        
-        Doing this parsing means searching for all parts and 
+
+        Doing this parsing means searching for all parts and
         constructing unique IDs for each item.
 
         Args:
             item_div (Tag): The div of the content item.
             counter (int): The counter to get unique ordered IDs.
             phys_structmap (Tag): The physical structmap element of Mets file.
             structlink (Tag): The structlink element of Mets file.
             item_dmd_sec (Tag): Dmd section of Mets file of this specific item.
 
         Returns:
             dict[str, Any]: Canonical representation of the content item.
         """
-        div_type = item_div.get('TYPE').lower()
-        
+        div_type = item_div.get("TYPE").lower()
+
         if div_type == BL_PICTURE_TYPE:
             div_type = CONTENTITEM_TYPE_IMAGE
         elif div_type == BL_AD_TYPE:
             div_type = CONTENTITEM_TYPE_ADVERTISEMENT
-        
+
         # Check if new content item is found (or if we need more translation)
         if div_type not in CONTENTITEM_TYPES:
-            logger.warning(f"Found new content item type: {div_type}")
-        
+            logger.warning("Found new content item type: %s", div_type)
+
         metadata = {
-            'id': "{}-i{}".format(self.id, str(counter).zfill(4)),
-            'tp': div_type,
-            'pp': [],
+            "id": "{}-i{}".format(self.id, str(counter).zfill(4)),
+            "tp": div_type,
+            "pp": [],
         }
         # Get content item's language
-        lang = item_dmd_sec.findChild('languageTerm')
+        lang = item_dmd_sec.findChild("languageTerm")
         if lang is not None:
-            metadata['l'] = lang.text
-        
+            metadata["l"] = lang.text
+
         # Load physical struct map, and find all parts in physical map
         content_item = {
             "m": metadata,
             "l": {
-                "id": item_div.get('ID'),
-                "parts": self._parse_content_parts(item_div, 
-                                                   phys_structmap, 
-                                                   structlink)
-            }
+                "id": item_div.get("ID"),
+                "parts": self._parse_content_parts(
+                    item_div, phys_structmap, structlink
+                ),
+            },
         }
-        for p in content_item['l']['parts']:
+        for p in content_item["l"]["parts"]:
             pge_no = p["comp_page_no"]
-            if pge_no not in content_item['m']['pp']:
-                content_item['m']['pp'].append(pge_no)
-        
+            if pge_no not in content_item["m"]["pp"]:
+                content_item["m"]["pp"].append(pge_no)
+
         # TODO: add coordinates for images as well as iiif_link
         # + update approach for handling images
         return content_item
-    
+
     def _parse_content_items(self) -> list[dict[str, Any]]:
         """Extract content item elements from a Mets XML file.
 
         Returns:
             list[dict[str, Any]]: List of all content items and the relevant
                 information in canonical format for each one.
         """
         mets_doc = self.xml
         content_items = []
         # Get logical structure of issue
-        divs = (mets_doc.find('structMap', {'TYPE': 'LOGICAL'})
-                .find('div', {'TYPE': 'ISSUE'})
-                .findChildren('div'))
-        
+        divs = (
+            mets_doc.find("structMap", {"TYPE": "LOGICAL"})
+            .find("div", {"TYPE": "ISSUE"})
+            .findChildren("div")
+        )
+
         # Sort to have same naming
-        sorted_divs = sorted(divs, key=lambda x: x.get('DMDID').lower())
-        
+        sorted_divs = sorted(divs, key=lambda x: x.get("DMDID").lower())
+
         # Get all CI types
-        found_types = set(x.get('TYPE') for x in sorted_divs)
-        
-        phys_structmap = mets_doc.find('structMap', {'TYPE': 'PHYSICAL'})
-        structlink = mets_doc.find('structLink')
-        
+        found_types = set(x.get("TYPE") for x in sorted_divs)
+
+        phys_structmap = mets_doc.find("structMap", {"TYPE": "PHYSICAL"})
+        structlink = mets_doc.find("structLink")
+
         counter = 1
         for div in sorted_divs:
             # Parse Each contentitem
-            dmd_sec = mets_doc.find('dmdSec', {'ID': div.get('DMDID')})
+            dmd_sec = mets_doc.find("dmdSec", {"ID": div.get("DMDID")})
             content_items.append(
-                self._parse_content_item(div, counter, phys_structmap,
-                                         structlink, dmd_sec)
+                self._parse_content_item(
+                    div, counter, phys_structmap, structlink, dmd_sec
+                )
             )
             counter += 1
+
+        # compute the reading order for the issue's items
+        reading_order_dict = get_reading_order(content_items)
+
+        for ci in content_items:
+            # add the reading order
+            ci["m"]["ro"] = reading_order_dict[ci["m"]["id"]]
+
         return content_items
-    
+
     def _parse_mets(self) -> None:
 
         # No image properties in BL data
-        
+
         # Parse all the content items
         content_items = self._parse_content_items()
-        
+
         self.issue_data = {
             "cdt": strftime("%Y-%m-%d %H:%M:%S"),
             "i": content_items,
             "id": self.id,
             "ar": self.rights,
-            "pp": [p.id for p in self.pages]
+            "pp": [p.id for p in self.pages],
         }
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/bl/detect.py` & `impresso_text_importer-1.1.0/text_importer/importers/bl/detect.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,29 @@
 """This module contains helper functions to find BL OCR data to import.
 """
+
 import logging
 import os
 from collections import namedtuple
 from datetime import date
-from typing import List, Optional
 import zipfile
 
+from glob import glob
 from dask import bag as db
 from impresso_commons.path.path_fs import _apply_datefilter
-from glob import glob
-from text_importer.utils import get_access_right
 
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger(__name__)
 
-EDITIONS_MAPPINGS = {
-    1: 'a',
-    2: 'b',
-    3: 'c',
-    4: 'd',
-    5: 'e'
-    }
+EDITIONS_MAPPINGS = {1: "a", 2: "b", 3: "c", 4: "d", 5: "e"}
 
 BlIssueDir = namedtuple(
-        "IssueDirectory", [
-            'journal',
-            'date',
-            'edition',
-            'path',
-            'rights'
-            ]
-        )
+    "IssueDirectory", ["journal", "date", "edition", "path", "rights"]
+)
 """A light-weight data structure to represent a newspaper issue.
 
 This named tuple contains basic metadata about a newspaper issue. They
 can then be used to locate the relevant data in the filesystem or to create
 canonical identifiers for the issue and its pages.
 
 Note:
@@ -60,212 +47,217 @@
     rights='open_public'
 )
 """
 
 BL_ACCESS_RIGHTS = "closed"
 
 
-def _get_single_subdir(_dir: str) -> Optional[str]:
+def _get_single_subdir(_dir: str) -> str | None:
     """Check if the given dir only has one directory and return its basename.
 
     Args:
         _dir (str): Directory to check.
 
     Returns:
-        Optional[str]: Subdirectory's basename if it's unique, None otherwise.
+        str | None: Subdirectory's basename if it's unique, None otherwise.
     """
     sub_dirs = [x for x in os.listdir(_dir) if os.path.isdir(os.path.join(_dir, x))]
-    
+
     if len(sub_dirs) == 0:
-        logger.warning(f"Could not find issue in BLIP: {_dir}")
+        logger.warning("Could not find issue in BLIP: %s", _dir)
         return None
-    elif len(sub_dirs) > 1:
-        logger.warning(f"Found more than one issue in BLIP: {_dir}")
+    if len(sub_dirs) > 1:
+        logger.warning("Found more than one issue in BLIP: %s", _dir)
         return None
     return sub_dirs[0]
 
 
-def _get_journal_name(issue_path: str, blip_id: str) -> Optional[str]:
+def _get_journal_name(issue_path: str, blip_id: str) -> str | None:
     """Find the Journal name from within the Mets file.
 
     For BL, the journal name is not present in the directory structure.
     The BLIP Id is needed to fetch the right section. The BLIP ID is usually
     the top-level directory where the issue is located.
 
     Args:
         issue_path (str): Path to issue directory
         blip_id (str): BLIP ID of the issue.
 
     Returns:
-        Optional[str]: The name of the journal, or None if not found.
+        str | None: The name of the journal, or None if not found.
     """
     mets_file = [
         os.path.join(issue_path, f)
         for f in os.listdir(issue_path)
-        if 'mets.xml' in f.lower()
+        if "mets.xml" in f.lower()
     ]
     if len(mets_file) == 0:
-        logger.critical(f"Could not find METS file in {issue_path}")
+        logger.critical("Could not find METS file in %s", issue_path)
         return None
-    
+
     mets_file = mets_file[0]
-    
-    with open(mets_file, 'r', encoding="utf-8") as f:
+
+    with open(mets_file, "r", encoding="utf-8") as f:
         raw_xml = f.read()
-    
-    mets_doc = BeautifulSoup(raw_xml, 'xml')
-    
+
+    mets_doc = BeautifulSoup(raw_xml, "xml")
+
     dmd_sec = [
-        x for x in mets_doc.findAll('dmdSec') 
-        if x.get('ID') and blip_id in x.get('ID')
+        x for x in mets_doc.findAll("dmdSec") if x.get("ID") and blip_id in x.get("ID")
     ]
     if len(dmd_sec) != 1:
-        logger.critical(f"Could not get journal name for {issue_path}")
+        logger.critical("Could not get journal name for %s", issue_path)
         return None
-    
-    contents = dmd_sec[0].find('title').contents
+
+    contents = dmd_sec[0].find("title").contents
     if len(contents) != 1:
-        logger.critical(f"Could not get journal name for {issue_path}")
+        logger.critical("Could not get journal name for %s", issue_path)
         return None
-    
+
     title = contents[0]
     acronym = [x[0] for x in title.split(" ")]
 
     return "".join(acronym)
 
 
 def _extract_all(archive_dir: str, destination: str) -> None:
     """Extract all zip files in `archive_dir` into `destination`.
 
     Args:
         archive_dir (str): Directory containing all archives to extract.
         destination (str): Destination directory.
     """
-    
+
     archive_files = glob(os.path.join(archive_dir, "*.zip"))
-    logger.info(f"Found {len(archive_files)} files to extract")
-    
+    logger.info("Found %s files to extract", len(archive_files))
+
     for archive in archive_files:
-        with zipfile.ZipFile(archive, 'r') as zip_ref:
+        with zipfile.ZipFile(archive, "r") as zip_ref:
             zip_ref.extractall(destination)
 
 
-def dir2issue(path: str) -> Optional[BlIssueDir]: 
+def dir2issue(path: str) -> BlIssueDir | None:
     """Given the BLIP directory of an issue, create the `BlIssueDir` object.
-    
+
     TODO: update handling of rights and edition with full data.
 
     Args:
         path (str): The BLIP directory path
 
     Returns:
         Optional[BlIssueDir]: The corresponding Issue
     """
-    split = path.split('/')
+    split = path.split("/")
     journal, year, month_day = split[-3], int(split[-2]), split[-1]
     month, day = int(month_day[:2]), int(month_day[2:])
-    
-    return BlIssueDir(journal=journal, date=date(year, month, day), 
-                      edition='a', path=path, rights=BL_ACCESS_RIGHTS)
+
+    return BlIssueDir(
+        journal=journal,
+        date=date(year, month, day),
+        edition="a",
+        path=path,
+        rights=BL_ACCESS_RIGHTS,
+    )
 
 
-def detect_issues(
-    base_dir: str, access_rights: str, tmp_dir: str
-) -> list[BlIssueDir]:
+def detect_issues(base_dir: str, access_rights: str, tmp_dir: str) -> list[BlIssueDir]:
     """Detect newspaper issues to import within the filesystem.
 
     This function expects the directory structure that the BL used to
     organize the dump of Mets/Alto OCR data.
 
     Args:
-        base_dir (str): Path to the base directory of newspaper data, 
+        base_dir (str): Path to the base directory of newspaper data,
             this directory should contain `zip` files.
-        access_rights (str): Not used for this imported, but argument is 
-            kept for normality.
+        access_rights (str): Not used for this importer, but argument is
+            kept for uniformity.
         tmp_dir (str): Temporary directory to unzip archives.
 
     Returns:
         list[BlIssueDir]: List of `BlIssueDir` instances to import.
     """
     # Extract all zips to tmp_dir
     _extract_all(base_dir, tmp_dir)
-    
+
     # base_dir becomes extracted archives dir
     base_dir = tmp_dir
-    
+
     # Get all BLIP dirs (named with NLP ID)
     blip_dirs = [
-        x for x in os.listdir(base_dir) 
-        if os.path.isdir(os.path.join(base_dir, x))
+        x for x in os.listdir(base_dir) if os.path.isdir(os.path.join(base_dir, x))
     ]
     issues = []
-    
+
     for blip in blip_dirs:
         blip_path = os.path.join(base_dir, blip)
         dir_path, journal_dirs, files = next(os.walk(blip_path))
-        
+
         # First iterate on all journals in BLIP dir
         for journal in journal_dirs:
             journal_path = os.path.join(blip_path, journal)
-            dir_path, year_dirs, files = next(os.walk(journal_path))
-            
+            _, year_dirs, _ = next(os.walk(journal_path))
+
             # Then on years
             for year in year_dirs:
                 year_path = os.path.join(journal_path, year)
-                dir_path, month_day_dirs, files = next(os.walk(year_path))
+                _, month_day_dirs, _ = next(os.walk(year_path))
                 # Then on each issue
                 for month_day in month_day_dirs:
                     path = os.path.join(year_path, month_day)
                     issues.append(dir2issue(path))
-    
+
     return issues
 
 
 def select_issues(
     base_dir: str, config: dict, access_rights: str, tmp_dir: str
-) -> Optional[list[BlIssueDir]]:
+) -> list[BlIssueDir] | None:
     """SDetect selectively newspaper issues to import.
 
     The behavior is very similar to :func:`detect_issues` with the only
     difference that ``config`` specifies some rules to filter the data to
     import. See `this section <../importers.html#configuration-files>`__ for
     further details on how to configure filtering.
 
     Args:
         base_dir (str): Path to the base directory of newspaper data.
         config (dict): Config dictionary for filtering.
         access_rights (str): Path to ``access_rights.json`` file.
         tmp_dir (str): Temporary directory to unzip archives.
 
     Returns:
-        Optional[list[BlIssueDir]]: List of `BlIssueDir` instances to import.
+        list[BlIssueDir] | None: List of `BlIssueDir` instances to import.
     """
-    
+
     # read filters from json configuration (see config.example.json)
     try:
         filter_dict = config["newspapers"]
         exclude_list = config["exclude_newspapers"]
         year_flag = config["year_only"]
-    
+
     except KeyError:
-        logger.critical(f"The key [newspapers|exclude_newspapers|year_only] "
-                        "is missing in the config file.")
-        return
-    
+        logger.critical(
+            "The key [newspapers|exclude_newspapers|year_only] "
+            "is missing in the config file."
+        )
+        return None
+
     issues = detect_issues(base_dir, access_rights, tmp_dir)
     issue_bag = db.from_sequence(issues)
-    selected_issues = (
-        issue_bag.filter(
-            lambda i: (
-                len(filter_dict) == 0 or i.journal in filter_dict.keys()
-            ) and i.journal not in exclude_list
-        ).compute()
-    )
-    
+    selected_issues = issue_bag.filter(
+        lambda i: (len(filter_dict) == 0 or i.journal in filter_dict.keys())
+        and i.journal not in exclude_list
+    ).compute()
+
     exclude_flag = False if not exclude_list else True
-    filtered_issues = _apply_datefilter(
-        filter_dict, selected_issues, year_only=year_flag
-    ) if not exclude_flag else selected_issues
-    logger.info(f"{len(filtered_issues)} newspaper issues remained "
-                f"after applying filter: {filtered_issues}")
-    
+    filtered_issues = (
+        _apply_datefilter(filter_dict, selected_issues, year_only=year_flag)
+        if not exclude_flag
+        else selected_issues
+    )
+    logger.info(
+        "%s newspaper issues remained after applying filter: %s",
+        len(filtered_issues),
+        filtered_issues,
+    )
+
     return filtered_issues
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/bnf/classes.py` & `impresso_text_importer-1.1.0/text_importer/importers/bnf/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,124 +11,125 @@
 from glob import glob
 from time import strftime
 
 from bs4 import BeautifulSoup
 from impresso_commons.path import IssueDir
 
 from text_importer.importers import CONTENTITEM_TYPE_IMAGE
-from text_importer.importers.bnf.helpers import (BNF_CONTENT_TYPES, 
-                                                 add_div, type_translation)
-from text_importer.importers.bnf.parsers import (parse_div_parts, 
-                                                 parse_embedded_cis, 
-                                                 parse_printspace)
-from text_importer.importers.mets_alto import (MetsAltoNewspaperIssue, 
-                                               MetsAltoNewspaperPage)
-from text_importer.importers.mets_alto.alto import (distill_coordinates, 
-                                                    parse_style)
-from text_importer.utils import get_issue_schema, get_page_schema
+from text_importer.importers.bnf.helpers import (
+    BNF_CONTENT_TYPES,
+    add_div,
+    type_translation,
+)
+from text_importer.importers.bnf.parsers import (
+    parse_div_parts,
+    parse_embedded_cis,
+    parse_printspace,
+)
+from text_importer.importers.mets_alto import (
+    MetsAltoNewspaperIssue,
+    MetsAltoNewspaperPage,
+)
+from text_importer.importers.mets_alto.alto import distill_coordinates, parse_style
+from text_importer.utils import get_issue_schema, get_page_schema, get_reading_order
 
 IssueSchema = get_issue_schema()
 Pageschema = get_page_schema()
 
 logger = logging.getLogger(__name__)
 
-IIIF_ENDPOINT_URL = "https://gallica.bnf.fr/iiif"
-IIIF_MANIFEST_SUFFIX = "full/full/0/manifest.json"
-IIIF_IMAGE_SUFFIX = "full/0/default.jpg"
+IIIF_ENDPOINT_URI = "https://gallica.bnf.fr/iiif"
+IIIF_MANIFEST_SUFFIX = "manifest.json"
+IIIF_SUFFIX = "info.json"
 
 
 class BnfNewspaperPage(MetsAltoNewspaperPage):
     """Newspaper page in BNF (Mets/Alto) format.
 
     Args:
         _id (str): Canonical page ID.
         number (int): Page number.
         filename (str): Name of the Alto XML page file.
         basedir (str): Base directory where Alto files are located.
-    
+
     Attributes:
         id (str): Canonical Page ID (e.g. ``GDL-1900-01-02-a-p0004``).
         number (int): Page number.
         page_data (dict[str, Any]): Page data according to canonical format.
         issue (NewspaperIssue): Issue this page is from.
         filename (str): Name of the Alto XML page file.
         basedir (str): Base directory where Alto files are located.
         encoding (str, optional): Encoding of XML file. Defaults to 'utf-8'.
         is_gzip (bool): Whether the page's corresponding file is in .gzip.
         ark_link (str): IIIF Ark identifier for this page.
     """
-    
-    def __init__(self, _id: str, number: int, 
-                 filename: str, basedir: str) -> None:
-        
+
+    def __init__(self, _id: str, number: int, filename: str, basedir: str) -> None:
+
         self.is_gzip = filename.endswith("gz")
         super().__init__(_id, number, filename, basedir)
         self.ark_link = self.xml.find("fileIdentifier").getText()
-    
+
     def _parse_font_styles(self) -> None:
-        """Parse the styles at the page level.
-        """
+        """Parse the styles at the page level."""
         style_divs = self.xml.findAll("TextStyle")
-        
+
         styles = []
         for d in style_divs:
             styles.append(parse_style(d))
-        
-        self.page_data['s'] = styles
-    
+
+        self.page_data["s"] = styles
+
     def add_issue(self, issue: MetsAltoNewspaperIssue) -> None:
         self.issue = issue
-        iiif_url = os.path.join(IIIF_ENDPOINT_URL, 
-                                self.ark_link, 
-                                IIIF_MANIFEST_SUFFIX)
-        self.page_data['iiif'] = iiif_url
+        self.page_data["iiif_img_base_uri"] = os.path.join(
+            IIIF_ENDPOINT_URI, self.ark_link
+        )
         self._parse_font_styles()
-    
+
     def parse(self) -> None:
         doc = self.xml
-        
+
         mappings = {}
-        for ci in self.issue.issue_data['i']:
-            ci_id = ci['m']['id']
-            if 'parts' in ci['l']:
-                for part in ci['l']['parts']:
-                    mappings[part['comp_id']] = ci_id
-        
-        pselement = doc.find('PrintSpace')
+        for ci in self.issue.issue_data["i"]:
+            ci_id = ci["m"]["id"]
+            if "parts" in ci["l"]:
+                for part in ci["l"]["parts"]:
+                    mappings[part["comp_id"]] = ci_id
+
+        pselement = doc.find("PrintSpace")
         page_data, notes = parse_printspace(pselement, mappings)
-        self.page_data['cc'], self.page_data["r"] = self._convert_coordinates(
-            page_data
-        )
+        self.page_data["cc"], self.page_data["r"] = self._convert_coordinates(page_data)
         if len(notes) > 0:
-            self.page_data['n'] = notes
+            self.page_data["n"] = notes
 
     @property
     def xml(self) -> BeautifulSoup:
         """Read Alto XML file of the page and create a BeautifulSoup object.
 
         Redefined function as for some issues, the pages are in gz format.
 
         Returns:
             BeautifulSoup: BeautifulSoup object with Alto XML of the page.
         """
         if not self.is_gzip:
             return super(BnfNewspaperPage, self).xml
         else:
             alto_xml_path = os.path.join(self.basedir, self.filename)
-            with gzip.open(alto_xml_path, 'r') as f:
+            with gzip.open(alto_xml_path, "r") as f:
                 raw_xml = f.read()
-            
-            alto_doc = BeautifulSoup(raw_xml, 'xml')
+
+            alto_doc = BeautifulSoup(raw_xml, "xml")
             return alto_doc
 
 
 class BnfNewspaperIssue(MetsAltoNewspaperIssue):
     """Newspaper Issue in BNF (Mets/Alto) format.
 
-    All functions defined in this child class are specific to parsing BNF 
+    All functions defined in this child class are specific to parsing BNF
     Mets/Alto format.
 
     Args:
         issue_dir (IssueDir): Identifying information about the issue.
 
     Attributes:
         id (str): Canonical Issue ID (e.g. ``GDL-1900-01-02-a``).
@@ -141,284 +142,304 @@
         rights (str): Access rights applicable to this issue.
         image_properties (dict[str, Any]): metadata allowing to convert region
             OCR/OLR coordinates to iiif format compliant ones.
         ark_id (int): Issue ARK identifier, for the issue's pages' iiif links.
         issue_uid (str): Basename of the Mets XML file of this issue.
         secondary_date (datetime.date): Potential secondary date of issue.
     """
-    
+
     def __init__(self, issue_dir: IssueDir) -> None:
         self.issue_uid = os.path.basename(issue_dir.path)
         self.secondary_date = issue_dir.secondary_date
         super().__init__(issue_dir)
-    
+
     @property
     def xml(self) -> BeautifulSoup:
         """Read Mets XML file of the issue and create a BeautifulSoup object.
 
         Returns:
             BeautifulSoup: BeautifulSoup object with Mets XML of the issue.
         """
         mets_regex = os.path.join(self.path, "toc", f"*{self.issue_uid}.xml")
         mets_file = glob(mets_regex)
         if len(mets_file) == 0:
-            logger.critical(f"Could not find METS file in {self.path}")
+            logger.critical("Could not find METS file in %s", self.path)
             return None
         mets_file = mets_file[0]
-        with open(mets_file, 'r', encoding="utf-8") as f:
+        with open(mets_file, "r", encoding="utf-8") as f:
             raw_xml = f.read()
-        
-        mets_doc = BeautifulSoup(raw_xml, 'xml')
+
+        mets_doc = BeautifulSoup(raw_xml, "xml")
         return mets_doc
-    
+
     def _find_pages(self) -> None:
         """Detect and create the issue pages using the relevant Alto XML files.
 
         Created :obj:`BnfNewspaperPage` instances are added to :attr:`pages`.
 
         Raises:
             e: Instantiation of a page or adding it to :attr:`pages` failed.
         """
         ocr_path = os.path.join(self.path, "ocr")  # Pages in `ocr` folder
-        
+
         pages = [
-            (file, int(file.split('.')[0][1:]))
+            (file, int(file.split(".")[0][1:]))
             for file in os.listdir(ocr_path)
-            if not file.startswith('.') and '.xml' in file
+            if not file.startswith(".") and ".xml" in file
         ]
-        
+
         page_filenames, page_numbers = zip(*pages)
-        
+
         page_canonical_names = [
-            "{}-p{}".format(self.id, str(page_n).zfill(4)) 
-            for page_n in page_numbers
+            "{}-p{}".format(self.id, str(page_n).zfill(4)) for page_n in page_numbers
         ]
-        
+
         self.pages = {}
-        for filename, page_no, page_id in zip(page_filenames, page_numbers, 
-                                              page_canonical_names):
+        for filename, page_no, page_id in zip(
+            page_filenames, page_numbers, page_canonical_names
+        ):
             try:
-                self.pages[page_no] = BnfNewspaperPage(page_id, page_no, 
-                                                       filename, ocr_path)
+                self.pages[page_no] = BnfNewspaperPage(
+                    page_id, page_no, filename, ocr_path
+                )
             except Exception as e:
                 logger.error(
-                    f'Adding page {page_no} {page_id} {filename}',
-                    f'raised following exception: {e}'
+                    "Adding page %s %s %s raised following exception: %s",
+                    page_no,
+                    page_id,
+                    filename,
+                    e,
                 )
                 raise e
-    
-    def _get_divs_by_type(self, mets: BeautifulSoup) -> dict[str, list[tuple[str, str]]]:
+
+    def _get_divs_by_type(
+        self, mets: BeautifulSoup
+    ) -> dict[str, list[tuple[str, str]]]:
         """Parse `div` tags, flatten them and sort them by type.
 
         First, parse the `dmdSec` tags, and sort them by type.
-        Then, search for `div` tags in the `content` of the `structMap` that 
+        Then, search for `div` tags in the `content` of the `structMap` that
         don't have the `DMDID` attribute, and for which the type is in
-        `BNF_CONTENT_TYPES`. 
+        `BNF_CONTENT_TYPES`.
         Finally, flatten the sections into what they actually contain, and add
         the flattened sections to the return dict.
 
         Args:
             mets (BeautifulSoup): Contents of the Mets XML file.
 
         Returns:
             dict[str, list[tuple[str, str]]]: All the `div` sorted by type, the
                 values are the List of (div_id, div_label)
         """
         dmd_sections = [x for x in mets.findAll("dmdSec") if x.find("mods")]
         struct_map = mets.find("structMap", {"TYPE": "logical"})
         struct_content = struct_map.find("div", {"TYPE": "CONTENT"})
-        
+
         by_type = {}
-        
+
         # First parse DMD section and keep DIV IDs of referenced items
         for s in dmd_sections:  # Iterate on the DMD section
             divs = struct_map.findAll("div", {"DMDID": s.get("ID")})
-            
+
             if len(divs) > 1:  # Means this DMDID is a class of objects
                 if s.find("mods:classification") is not None:
                     _type = s.find("mods:classification").getText().lower()
                     for d in divs:
-                        by_type = add_div(by_type, _type, d.get("ID"), 
-                                          d.get("LABEL"))
+                        by_type = add_div(by_type, _type, d.get("ID"), d.get("LABEL"))
                 else:
-                    logger.warning(
-                        f"MultiDiv with no classification for {self.id}"
-                    )
+                    logger.warning("MultiDiv with no classification for %s", self.id)
             else:
                 div = divs[0]
                 _type = div.get("TYPE").lower()
-                by_type = add_div(by_type, _type, div.get("ID"), 
-                                  div.get("LABEL"))
-        
-        # Parse div sections that are direct children of CONTENT in the 
+                by_type = add_div(by_type, _type, div.get("ID"), div.get("LABEL"))
+
+        # Parse div sections that are direct children of CONTENT in the
         # logical structMap, and keep the ones without DMDID
         for c in struct_content.findChildren("div", recursive=False):
             if c.get("DMDID") is None and c.get("TYPE") is not None:
                 _type = c.get("TYPE").lower()
-                by_type = add_div(by_type, _type, c.get("ID"), 
-                                  c.get("LABEL"))
-        
-        if 'section' in by_type:
+                by_type = add_div(by_type, _type, c.get("ID"), c.get("LABEL"))
+
+        if "section" in by_type:
             by_type = self._flatten_sections(by_type, struct_content)
-        
+
         return by_type
-    
+
     def _flatten_sections(
         self, by_type: dict, struct_content
     ) -> dict[str, list[tuple[str, str]]]:
         """Flatten the sections of the issue.
-        
+
         This means making the children parts standalone CIs.
 
         Args:
             by_type (dict): Parsed `div` tags separated by type
             struct_content (_type_): _description_
 
         Returns:
             dict[str, list[tuple[str, str]]]: _description_
         """
         # Flatten the sections
-        for div_id, lab in by_type['section']:
+        for div_id, lab in by_type["section"]:
             # Get all divs of this section
-            div = struct_content.find("div", {"ID": div_id}) 
+            div = struct_content.find("div", {"ID": div_id})
             for d in div.findChildren("div", recursive=False):
                 dmdid = d.get("DMDID")
                 div_id = d.get("ID")
                 ci_type = d.get("TYPE").lower()
                 d_label = d.get("LABEL")
                 # This div needs to be added to the content items
-                if dmdid is None and ci_type in BNF_CONTENT_TYPES:  
+                if dmdid is None and ci_type in BNF_CONTENT_TYPES:
                     by_type = add_div(by_type, ci_type, div_id, d_label or lab)
                 elif dmdid is None:
-                    logging.debug(f" {self.id}: {div_id} of type {ci_type} "
-                                  "within section is not in CONTENT_TYPES")
-        del by_type['section']
+                    logging.debug(
+                        " %s: %s of type %s within section is not in CONTENT_TYPES",
+                        self.id,
+                        div_id,
+                        ci_type,
+                    )
+        del by_type["section"]
         return by_type
-    
-    def _parse_div(self, div_id: str, div_type: str, 
-                   label: str, item_counter: int, 
-                   mets_doc: BeautifulSoup) -> tuple[list[dict], int]:
+
+    def _parse_div(
+        self,
+        div_id: str,
+        div_type: str,
+        label: str,
+        item_counter: int,
+        mets_doc: BeautifulSoup,
+    ) -> tuple[list[dict], int]:
         """Parse the given `div_id` from the `structMap` of the METS file.
 
         Args:
             div_id (str): Unique ID of the div to parse
             div_type (str): Type of the div (should be in `BNF_CONTENT_TYPES`)
             label (str): Label of the div (title)
             item_counter (int): The current counter for CI IDs
             mets_doc (BeautifulSoup): Contents of the Mets XML file.
 
         Returns:
             tuple[list[dict], int]: _description_
         """
         article_div = mets_doc.find("div", {"ID": div_id})  # Get the tag
         # Try to get the body if there is one (we discard headings)
-        article_div = article_div.find("div", {"TYPE": "BODY"}) or article_div  
+        article_div = article_div.find("div", {"TYPE": "BODY"}) or article_div
         parts = parse_div_parts(article_div)  # Parse the parts of the tag
-        metadata = None
+        metadata, ci = None, None
         # If parts were found, create content item for this DIV
-        if len(parts) > 0:  
+        if len(parts) > 0:
             article_id = "{}-i{}".format(self.id, str(item_counter).zfill(4))
             metadata = {
-                'id': article_id,
-                'tp': type_translation[div_type],
-                'pp': [],
-                }
+                "id": article_id,
+                "tp": type_translation[div_type],
+                "pp": [],
+            }
             if label is not None:
-                metadata['t'] = label
-            ci = {
-                'm': metadata,
-                'l': {
-                    'parts': parts
-                    }
-                }
+                metadata["t"] = label
+            ci = {"m": metadata, "l": {"parts": parts}}
             item_counter += 1
         else:  # Otherwise, only parse embedded CIs
             article_id = None
 
-        embedded, item_counter = parse_embedded_cis(article_div, label, 
-                                                    self.id, article_id, 
-                                                    item_counter)
-        
+        embedded, item_counter = parse_embedded_cis(
+            article_div, label, self.id, article_id, item_counter
+        )
+
         if metadata is not None:
             embedded.append(ci)
+
         return embedded, item_counter
-    
-    def _get_image_iiif_link(self, ci_id: str, parts: list) -> str:
-        """Get the image iiif info uri given the ID of the CI.
 
+    def _get_image_iiif_link(self, ci_id: str, parts: list) -> tuple[list[int], str]:
+        """Get the image coordinates and iiif info uri given the ID of the CI.
         Args:
             ci_id (str): The ID of the image CI
             parts (list): Parts of the image
-
         Returns:
-            str: The iiif uri to the info.json for the page's image.
+            tuple[list[int], str]: The image coordinated and iiif uri to the
+                info.json for the page's image.
         """
-        image_part = [
-            p for p in parts 
-            if p['comp_role'] == CONTENTITEM_TYPE_IMAGE
-        ]
-        iiif_link = None
+        image_part = [p for p in parts if p["comp_role"] == CONTENTITEM_TYPE_IMAGE]
+        iiif_link, coords = None, None
         if len(image_part) == 0:
-            message = (f"Content item {ci_id} of type "
-                       f"{CONTENTITEM_TYPE_IMAGE} does not have image part.")
+            message = (
+                f"Content item {ci_id} of type "
+                f"{CONTENTITEM_TYPE_IMAGE} does not have image part."
+            )
             logger.warning(message)
         elif len(image_part) > 1:
-            message = (f"Content item {ci_id} of type "
-                       f"{CONTENTITEM_TYPE_IMAGE} has multiple image parts.")
+            message = (
+                f"Content item {ci_id} of type "
+                f"{CONTENTITEM_TYPE_IMAGE} has multiple image parts."
+            )
             logger.warning(message)
         else:
-            
-            image_part_id = image_part[0]['comp_id']
-            page = self.pages[image_part[0]['comp_page_no']]
+
+            image_part_id = image_part[0]["comp_id"]
+            page = self.pages[image_part[0]["comp_page_no"]]
             block = page.xml.find("Illustration", {"ID": image_part_id})
             if block is None:
-                logger.warning("Could not find image "
-                               f"{image_part_id} for CI {ci_id}")
+                logger.warning(
+                    "Could not find image %s for CI %s", image_part_id, ci_id
+                )
             else:
                 coords = distill_coordinates(block)
-                iiif_link = os.path.join(IIIF_ENDPOINT_URL, 
-                                         page.ark_link, 
-                                         ",".join(str(c) for c in coords),
-                                         IIIF_IMAGE_SUFFIX)
-        return iiif_link
-    
+                iiif_link = os.path.join(IIIF_ENDPOINT_URI, page.ark_link, IIIF_SUFFIX)
+
+        return coords, iiif_link
+
     def _parse_mets(self) -> None:
         """Parse the Mets XML file corresponding to this issue.
 
-        Once the :attr:`issue_data` is created, containing all the relevant 
+        Once the :attr:`issue_data` is created, containing all the relevant
         information in the canonical Issue format, the `BnfNewspaperIssue`
         instance is ready for serialization.
         """
-        
+
         mets_doc = self.xml
         # First get all the divs by type
         by_type = self._get_divs_by_type(mets_doc)
         item_counter = 1
         content_items = []
-        
+
         # Then start parsing them
         for div_type, divs in by_type.items():
             for div_id, div_label in divs:
-                cis, item_counter = self._parse_div(div_id, div_type, div_label, 
-                                                    item_counter, mets_doc)
+                cis, item_counter = self._parse_div(
+                    div_id, div_type, div_label, item_counter, mets_doc
+                )
                 content_items += cis
-        
+
         # Finally add the pages and iiif link
         for x in content_items:
-            x['m']['pp'] = list(set(c['comp_page_no'] for c in x['l']['parts']))
-            if x['m']['tp'] == CONTENTITEM_TYPE_IMAGE:
-                x['m']['iiif_link'] = self._get_image_iiif_link(x['m']['id'], 
-                                                                x['l']['parts'])
-        
+            x["m"]["pp"] = list(set(c["comp_page_no"] for c in x["l"]["parts"]))
+            if x["m"]["tp"] == CONTENTITEM_TYPE_IMAGE:
+                x["c"], x["m"]["iiif_link"] = self._get_image_iiif_link(
+                    x["m"]["id"], x["l"]["parts"]
+                )
+
+        # once the pages are added to the metadata, compute & add the reading order
+        reading_order_dict = get_reading_order(content_items)
+        for item in content_items:
+            item["m"]["ro"] = reading_order_dict[item["m"]["id"]]
+
         self.pages = list(self.pages.values())
-        
+
+        # Issue manifest iiif URI is in format {iiif_prefix}/{ark_id}/manifest.json
+        # By default, the ark id contains the page number,
+        iiif_manifest = os.path.join(
+            IIIF_ENDPOINT_URI,
+            os.path.dirname(self.pages[0].ark_link),
+            IIIF_MANIFEST_SUFFIX,
+        )
+
         self.issue_data = {
             "cdt": strftime("%Y-%m-%d %H:%M:%S"),
-            "i": content_items,
             "id": self.id,
+            "i": content_items,
             "ar": self.rights,
-            "pp": [p.id for p in self.pages]
+            "pp": [p.id for p in self.pages],
+            "iiif_manifest_uri": iiif_manifest,
         }
-
         # Note for newspapers with two dates (197 cases)
         if self.secondary_date is not None:
-            self.issue_data['n'] = [f"Secondary date {self.secondary_date}"]
+            self.issue_data["n"] = [f"Secondary date {self.secondary_date}"]
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/bnf/detect.py` & `impresso_text_importer-1.1.0/text_importer/importers/bnf/detect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This module contains helper functions to find BNF OCR data to import.
 """
+
 import json
 import logging
 import os
 import string
 from collections import namedtuple
 from typing import List, Optional
 
@@ -14,23 +15,16 @@
 from text_importer.importers.bnf.helpers import get_journal_name, parse_date
 from text_importer.importers.mets_alto.mets import get_dmd_sec
 from text_importer.utils import get_access_right
 
 logger = logging.getLogger(__name__)
 
 BnfIssueDir = namedtuple(
-        "IssueDirectory", [
-            'journal',
-            'date',
-            'edition',
-            'path',
-            'rights',
-            'secondary_date'
-            ]
-        )
+    "IssueDirectory", ["journal", "date", "edition", "path", "rights", "secondary_date"]
+)
 """A light-weight data structure to represent a newspaper issue.
 
 This named tuple contains basic metadata about a newspaper issue. They
 can then be used to locate the relevant data in the filesystem or to create
 canonical identifiers for the issue and its pages.
 
 Note:
@@ -61,38 +55,39 @@
     secondary_date = None
 )
 """
 
 DATE_FORMATS = ["%Y-%m-%d", "%Y/%m/%d"]
 DATE_SEPARATORS = ["/", "-"]
 
+
 def get_id(issue: BnfIssueDir) -> str:
     """Return an issue's canonical ID given its IssueDir.
 
     Args:
         issue (BnfIssueDir): IssueDir of issue.
 
     Returns:
         str: Canonical ID of issue.
     """
-    return "{}-{}-{:02}-{:02}-{}".format(issue.journal, issue.date.year, 
-                                         issue.date.month, issue.date.day, 
-                                         issue.edition)
+    return "{}-{}-{:02}-{:02}-{}".format(
+        issue.journal, issue.date.year, issue.date.month, issue.date.day, issue.edition
+    )
 
 
 def get_number(issue: BnfIssueDir) -> str:
     """Return an issue's original identifying number given its IssueDir.
 
     Args:
         issue (BnfIssueDir): IssueDir of issue.
 
     Returns:
         str: Identifying number in BNF's original file structure.
     """
-    return issue.path.split('/')[-1]
+    return issue.path.split("/")[-1]
 
 
 def assign_editions(issues: list[BnfIssueDir]) -> list[BnfIssueDir]:
     """Assign updated edition numbers to each issue of a given day.
 
     TFor BNF, the issues are not organized by date or edition in the file
     system. Hence, when multiple issues exist for a given day, an indexing
@@ -103,20 +98,22 @@
 
     Returns:
         list[BnfIssueDir]: List of issues with updated editions.
     """
     issues = sorted(issues, key=lambda x: x[1])
     new_issues = []
     for index, (i, n) in enumerate(issues):
-        i = BnfIssueDir(journal=i.journal,
-                        date=i.date,
-                        edition=string.ascii_lowercase[index],
-                        path=i.path,
-                        rights=i.rights,
-                        secondary_date=i.secondary_date)
+        i = BnfIssueDir(
+            journal=i.journal,
+            date=i.date,
+            edition=string.ascii_lowercase[index],
+            path=i.path,
+            rights=i.rights,
+            secondary_date=i.secondary_date,
+        )
         new_issues.append((i, n))
     return new_issues
 
 
 def dir2issue(issue_path: str, access_rights_dict: dict) -> BnfIssueDir:
     """Create a `BnfIssueDir` object from an archive path.
 
@@ -127,131 +124,133 @@
         issue_path (str): The path of the issue within the archive.
         access_rights_dict (dict): Access rights for this issue.
 
     Returns:
         BnfIssueDir: New `BnfIssueDir` object
     """
     manifest_file = os.path.join(issue_path, "manifest.xml")
-    
+
     issue = None
     if os.path.isfile(manifest_file):
-        with open(manifest_file) as f:
+        with open(manifest_file, encoding="utf-8") as f:
             manifest = BeautifulSoup(f, "xml")
-        
+
         try:
             # Issue info is in dmdSec of id "DMD.2"
-            issue_info = get_dmd_sec(manifest, "DMD.2")  
+            issue_info = get_dmd_sec(manifest, "DMD.2")
             journal = get_journal_name(issue_path)
             np_date, secondary_date = parse_date(
-                issue_info.find("date").contents[0], 
-                DATE_FORMATS, 
-                DATE_SEPARATORS
+                issue_info.find("date").contents[0], DATE_FORMATS, DATE_SEPARATORS
             )
             edition = "a"
             rights = get_access_right(journal, np_date, access_rights_dict)
-            issue = BnfIssueDir(journal=journal, date=np_date, 
-                                edition=edition, path=issue_path, 
-                                rights=rights, secondary_date=secondary_date)
+            issue = BnfIssueDir(
+                journal=journal,
+                date=np_date,
+                edition=edition,
+                path=issue_path,
+                rights=rights,
+                secondary_date=secondary_date,
+            )
         except ValueError as e:
             logger.info(e)
-            logger.error(f"Could not parse issue at {issue_path}")
+            logger.error("Could not parse issue at %s", issue_path)
     else:
-        logger.error(f"Could not find manifest in {issue_path}")
+        logger.error("Could not find manifest in %s", issue_path)
     return issue
 
 
-def detect_issues(
-    base_dir: str, access_rights: str = None
-) -> list[BnfIssueDir]:
+def detect_issues(base_dir: str, access_rights: str = None) -> list[BnfIssueDir]:
     """Detect BNF issues to import within the filesystem
 
     This function the directory structure used by BNF (one subdir by journal).
 
     Args:
         base_dir (str): Path to the base directory of newspaper data.
         access_rights (str, optional): Not used for this importer, but argument
             is kept for normality. Defaults to None.
 
     Returns:
         list[BnfIssueDir]: List of `BnfIssueDir` instances, to be imported.
     """
-    dir_path, dirs, files = next(os.walk(base_dir))
+    dir_path, dirs, _ = next(os.walk(base_dir))
     journal_dirs = [
-        os.path.join(dir_path, _dir) 
-        for _dir in dirs if not _dir.startswith("2")
+        os.path.join(dir_path, _dir) for _dir in dirs if not _dir.startswith("2")
     ]
     issue_dirs = [
         os.path.join(journal, _dir)
         for journal in journal_dirs
         for _dir in os.listdir(journal)
-        ]
-    
-    with open(access_rights, 'r') as f:
+    ]
+
+    with open(access_rights, "r", encoding="utf-8") as f:
         access_rights_dict = json.load(f)
     issue_dirs = [dir2issue(_dir, access_rights_dict) for _dir in issue_dirs]
     initial_length = len(issue_dirs)
     issue_dirs = [i for i in issue_dirs if i is not None]
-    
-    df = pd.DataFrame([
-        {"issue": i, "id": get_id(i), "number": get_number(i)} 
-        for i in issue_dirs
-    ])
-    vals = df.groupby('id').apply(
-        lambda x: x[['issue', 'number']].values.tolist()
-    ).values
-    
+
+    df = pd.DataFrame(
+        [{"issue": i, "id": get_id(i), "number": get_number(i)} for i in issue_dirs]
+    )
+    vals = (
+        df.groupby("id").apply(lambda x: x[["issue", "number"]].values.tolist()).values
+    )
+
     issue_dirs = [i if len(i) == 1 else assign_editions(i) for i in vals]
     issue_dirs = [j[0] for i in issue_dirs for j in i]
-    
-    logger.info(f"Removed {initial_length - len(issue_dirs)} problematic issues")
+
+    logger.info("Removed %s problematic issues", initial_length - len(issue_dirs))
     return [i for i in issue_dirs if i is not None]
 
 
 def select_issues(
     base_dir: str, config: dict, access_rights: str
 ) -> Optional[List[BnfIssueDir]]:
     """Detect selectively newspaper issues to import.
-    
+
     The behavior is very similar to :func:`detect_issues` with the only
     difference that ``config`` specifies some rules to filter the data to
     import. See `this section <../importers.html#configuration-files>`__ for
     further details on how to configure filtering.
 
     Args:
         base_dir (str): Path to the base directory of newspaper data.
         config (dict): Config dictionary for filtering.
-        access_rights (str): Not used for this imported, but argument is kept 
+        access_rights (str): Not used for this imported, but argument is kept
             for normality.
 
     Returns:
         Optional[List[BnfIssueDir]]: List of `BnfIssueDir` instances, to be imported.
     """
-    
+
     # read filters from json configuration (see config.example.json)
     try:
         filter_dict = config["newspapers"]
         exclude_list = config["exclude_newspapers"]
         year_flag = config["year_only"]
-    
+
     except KeyError:
-        logger.critical(f"The key [newspapers|exclude_newspapers|year_only] "
-                        "is missing in the config file.")
+        logger.critical(
+            "The key [newspapers|exclude_newspapers|year_only] "
+            "is missing in the config file."
+        )
         return
-    
+
     issues = detect_issues(base_dir, access_rights)
     issue_bag = db.from_sequence(issues)
-    selected_issues = (
-        issue_bag.filter(
-            lambda i: (
-                len(filter_dict) == 0 or i.journal in filter_dict.keys()
-            ) and i.journal not in exclude_list
-        ).compute()
-    )
-    
+    selected_issues = issue_bag.filter(
+        lambda i: (len(filter_dict) == 0 or i.journal in filter_dict.keys())
+        and i.journal not in exclude_list
+    ).compute()
     exclude_flag = False if not exclude_list else True
-    filtered_issues = _apply_datefilter(
-        filter_dict, selected_issues, year_only=year_flag
-    ) if not exclude_flag else selected_issues
-    logger.info(f"{len(filtered_issues)} newspaper issues remained "
-                f"after applying filter: {filtered_issues}")
-    
+    filtered_issues = (
+        _apply_datefilter(filter_dict, selected_issues, year_only=year_flag)
+        if not exclude_flag
+        else selected_issues
+    )
+    logger.info(
+        "%s newspaper issues remained after applying filter: %s",
+        len(filtered_issues),
+        filtered_issues,
+    )
+
     return filtered_issues
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/bnf/helpers.py` & `impresso_text_importer-1.1.0/text_importer/importers/bnf/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 """Set of helper functions for BNF importer"""
+
 import logging
 from datetime import datetime
-from typing import List, Optional, Tuple
+from typing import Optional
 
-from text_importer.importers import CONTENTITEM_TYPE_ADVERTISEMENT, CONTENTITEM_TYPE_ARTICLE, CONTENTITEM_TYPE_IMAGE, \
-    CONTENTITEM_TYPE_OBITUARY, CONTENTITEM_TYPE_TABLE
+from text_importer.importers import (
+    CONTENTITEM_TYPE_ADVERTISEMENT,
+    CONTENTITEM_TYPE_ARTICLE,
+    CONTENTITEM_TYPE_IMAGE,
+    CONTENTITEM_TYPE_OBITUARY,
+    CONTENTITEM_TYPE_TABLE,
+)
 
 # BNF types that do not have a direct `area` descendant
-BNF_CONTENT_TYPES = ["article", "advertisement", "illustration",
-                     "ornament", "freead", "table"]  
+BNF_CONTENT_TYPES = [
+    "article",
+    "advertisement",
+    "illustration",
+    "ornament",
+    "freead",
+    "table",
+]
 SECTION = "section"
 """
 Content types as defined in BNF Mets flavour. 
 These are the ones we are interested in parsing. 
 The `SECTION` type should be flattened, and shouldn't be part of content items,
 but it is needed to parse what's inside.
 """
 
 type_translation = {
-    'illustration': CONTENTITEM_TYPE_IMAGE,
-    'advertisement': CONTENTITEM_TYPE_ADVERTISEMENT,
-    'ornament': CONTENTITEM_TYPE_OBITUARY,
-    'table': CONTENTITEM_TYPE_TABLE,
-    'article': CONTENTITEM_TYPE_ARTICLE,
-    'freead': CONTENTITEM_TYPE_ADVERTISEMENT
+    "illustration": CONTENTITEM_TYPE_IMAGE,
+    "advertisement": CONTENTITEM_TYPE_ADVERTISEMENT,
+    "ornament": CONTENTITEM_TYPE_OBITUARY,
+    "table": CONTENTITEM_TYPE_TABLE,
+    "article": CONTENTITEM_TYPE_ARTICLE,
+    "freead": CONTENTITEM_TYPE_ADVERTISEMENT,
 }
 
 logger = logging.getLogger(__name__)
 
 
 def add_div(
     _dict: dict[str, tuple[str, str]], _type: str, div_id: str, label: str
 ) -> dict[str, tuple[str, str]]:
     """Adds a div item to the given dictionary (sorted by type).
-    
+
     The types used as keys should be in `BNF_CONTENT_TYPES` or `SECTION`.
 
     Args:
         _dict (dict[str, tuple[str, str]]): The dictionary where to add the div
         _type (str): The type of the new div to add.
         div_id (str): The div ID to add.
         label (str): The label of the div to add.
@@ -47,31 +59,33 @@
     """
     if _type in BNF_CONTENT_TYPES or _type == SECTION:
         if _type in _dict:
             _dict[_type].append((div_id, label))
         else:
             _dict[_type] = [(div_id, label)]
     else:
-        logger.warning(f"Tried to add div of type {_type}")
+        logger.warning("Tried to add div of type %s", _type)
+
     return _dict
 
 
 def get_journal_name(archive_path: str) -> str:
     """Return the Journal name from the path of the issue.
 
     It assumes the journal name is one directory above the issue.
 
     Args:
         archive_path (str): Path to the issue's archive
 
     Returns:
         str: Extracted journal name in lowercase.
     """
-    journal = archive_path.split('/')[-2].split('-')
+    journal = archive_path.split("/")[-2].split("-")
     journal = "".join(journal).lower()
+
     return journal
 
 
 def is_multi_date(date_string: str) -> bool:
     """Check whether a given date string is composed of more than one date.
 
     This check is based on the assumption that a full date is 10 chars long.
@@ -98,24 +112,25 @@
 
     Returns:
         list[Optional[str]]: Separated date or pair of None.
     """
     for s in separators:
         if len(date_string.split(s)) == 2:
             return date_string.split(s)
+
     return [None, None]
 
 
 def parse_date(
     date_string: str, formats: list[str], separators: list[str]
 ) -> tuple[datetime.date, Optional[datetime.date]]:
     """Parse a date given a list of formats.
 
     The input string can sometimes represent a pair of dates, in which case
-    they are both parsed if possible. 
+    they are both parsed if possible.
 
     Args:
         date_string (str): Date string to parse.
         formats (list[str]): Possible dates formats.
         separators (list[str]): List of possible date separators.
 
     Raises:
@@ -126,35 +141,36 @@
 
     Returns:
         tuple[datetime.date, Optional[datetime.date]]: Parsed date, potentially
             parsed pair of dates.
     """
     date, secondary = None, None
     # Date_string 1 and 2
-    ds_1, ds_2 = None, None  
-    
-    # Dates have at least 10 characters. 
+    ds_1, ds_2 = None, None
+
+    # Dates have at least 10 characters.
     # Some (very rarely) issues have only year/month
     if len(date_string) < 10:
-        raise ValueError("Could not parse date {}".format(date_string))
+        raise ValueError(f"Could not parse date {date_string}")
     # Here we potentially have two dates, take the first one
-    elif is_multi_date(date_string):  
-        logger.info(f"Got two dates {date_string}")
+    elif is_multi_date(date_string):
+        logger.info("Got two dates %s", date_string)
         ds_1, ds_2 = get_dates(date_string, separators)
-        
+
         if ds_1 is None:
-            raise ValueError("Could not parse date {}".format(date_string))
+            raise ValueError(f"Could not parse date {date_string}")
     else:
         ds_1 = date_string
-    
+
     # Now parse
     for f in formats:
         try:
             date = datetime.strptime(ds_1, f).date()
             if ds_2 is not None:
                 secondary = datetime.strptime(ds_2, f).date()
-        except ValueError as e:
+        except ValueError:
             pass
-    
+
     if date is None:
-        raise ValueError("Could not parse date {}".format(date_string))
+        raise ValueError(f"Could not parse date {date_string}")
+
     return date, secondary
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/bnf/parsers.py` & `impresso_text_importer-1.1.0/text_importer/importers/bnf/parsers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,173 +1,166 @@
 """Utility functions to parse BNF ALTO files."""
+
 import logging
-from typing import List, Dict, Optional, Tuple
 
 import bs4
 from bs4 import NavigableString
 from bs4.element import Tag
 
 from text_importer.importers.bnf.helpers import BNF_CONTENT_TYPES, type_translation
 from text_importer.importers.mets_alto.alto import parse_textline, distill_coordinates
 
 logger = logging.getLogger(__name__)
 
 
 def parse_printspace(
-    element: Tag, mappings: Dict[str, str]
+    element: Tag, mappings: dict[str, str]
 ) -> tuple[list[dict], list[str] | None]:
     """Parse the ``<PrintSpace>`` element of an ALTO XML document for BNF.
 
     Args:
         element (Tag): Input XML element (``<PrintSpace>``).
         mappings (Dict[str, str]): Description of parameter `mappings`.
 
     Returns:
         tuple[list[dict], list[str] | None]: Parsed regions and paragraphs, and
             potential notes on issues encountered during the parsing.
     """
-    
+
     regions = []
     notes = []
     for block in element.children:
-        
+
         if isinstance(block, bs4.element.NavigableString):
             continue
-        
-        block_id = block.get('ID')
+
+        block_id = block.get("ID")
         if block.name == "ComposedBlock":
             cb_regions, new_notes = parse_printspace(block, mappings)
             regions += cb_regions
             notes += new_notes
         else:
             if block_id in mappings:
                 part_of_contentitem = mappings[block_id]
             else:
                 part_of_contentitem = None
-            
+
             coordinates = distill_coordinates(block)
-            
+
             tmp = [
                 parse_textline(line_element)
-                for line_element in block.findAll('TextLine')
+                for line_element in block.findAll("TextLine")
             ]
-            
+
             if len(tmp) > 0:
                 lines, new_notes = list(zip(*tmp))
                 new_notes = [i for n in new_notes for i in n]
             else:
                 lines, new_notes = [], []
-            
-            paragraph = {
-                "c": coordinates,
-                "l": lines
-            }
-            
-            region = {
-                "c": coordinates,
-                "p": [paragraph]
-            }
-            
+
+            paragraph = {"c": coordinates, "l": lines}
+
+            region = {"c": coordinates, "p": [paragraph]}
+
             if part_of_contentitem:
-                region['pOf'] = part_of_contentitem
+                region["pOf"] = part_of_contentitem
             notes += new_notes
             regions.append(region)
+
     return regions, notes
 
 
 def parse_div_parts(div: Tag) -> list[dict[str, str | int]]:
     """Parse the parts of a given div element.
-    
-    Typically, any div of type in `BNF_CONTENT_TYPES` is composed of child 
+
+    Typically, any div of type in `BNF_CONTENT_TYPES` is composed of child
     divs. This is what this function parses.
-    Each element of the output contains keys {'comp_role', 'comp_id', 
+    Each element of the output contains keys {'comp_role', 'comp_id',
     'comp_fileid', 'comp_page_no'}.
 
     Args:
         div (Tag): Child div to parse.
 
     Returns:
-        list[dict[str, str | int]]: The list of parts of this Tag. 
+        list[dict[str, str | int]]: The list of parts of this Tag.
     """
     parts = []
     for child in div.children:
-        
+
         if isinstance(child, NavigableString):
             continue
         elif isinstance(child, Tag):
-            type_attr = child.get('TYPE')
+            type_attr = child.get("TYPE")
             comp_role = type_attr.lower() if type_attr else None
-            
+
             if comp_role not in BNF_CONTENT_TYPES:
-                areas = child.findAll('area')
+                areas = child.findAll("area")
                 for area in areas:
-                    comp_id = area.get('BEGIN')
-                    comp_fileid = area.get('FILEID')
+                    comp_id = area.get("BEGIN")
+                    comp_fileid = area.get("FILEID")
                     comp_page_no = int(comp_fileid.split(".")[1])
-                    
+
                     parts.append(
                         {
-                            'comp_role': comp_role,
-                            'comp_id': comp_id,
-                            'comp_fileid': comp_fileid,
-                            'comp_page_no': comp_page_no
+                            "comp_role": comp_role,
+                            "comp_id": comp_id,
+                            "comp_fileid": comp_fileid,
+                            "comp_page_no": comp_page_no,
                         }
                     )
     return parts
 
 
-def parse_embedded_cis(div: Tag, label: str, issue_id: str,
-                       parent_id: str | None, counter: int
+def parse_embedded_cis(
+    div: Tag, label: str, issue_id: str, parent_id: str | None, counter: int
 ) -> tuple[list[dict], int]:
     """Parse the div Tags embedded in the given one.
 
-    The input `div` should be of type in `BNF_CONTENT_TYPES` and should have 
+    The input `div` should be of type in `BNF_CONTENT_TYPES` and should have
     children of types also in that category.
-    Each child tag represents separate content items, which should thus be 
+    Each child tag represents separate content items, which should thus be
     processed separately.
 
     Args:
         div (Tag): The parent tag.
         label (str): The label of the parent tag.
         issue_id (str): The ID of the issue.
         parent_id (str | None): The ID of the parent tag (to put into pOf).
         counter (int): Counter for content items.
 
     Returns:
         tuple[list[dict], int]: The embedded CIs and resulting updated counter.
     """
     new_cis = []
     for child in div.children:
-        
+
         if isinstance(child, NavigableString):
             continue
         elif isinstance(child, Tag):
-            type_attr = child.get('TYPE')
+            type_attr = child.get("TYPE")
             comp_role = type_attr.lower() if type_attr else None
             if comp_role in BNF_CONTENT_TYPES:
                 if comp_role in type_translation:
                     impresso_type = type_translation[comp_role]
                 else:
-                    logger.warning(f"Type {comp_role} does not have translation")
+                    logger.warning("Type %s does not have translation", comp_role)
                     impresso_type = comp_role
-                
+
                 metadata = {
-                    'id': "{}-i{}".format(issue_id, str(counter).zfill(4)),
-                    'tp': impresso_type,
-                    'pp': [],
+                    "id": "{}-i{}".format(issue_id, str(counter).zfill(4)),
+                    "tp": impresso_type,
+                    "pp": [],
                 }
-                lab = child.get('LABEL') or label
-                
+                lab = child.get("LABEL") or label
+
                 if lab is not None:
-                    metadata['t'] = lab
-                # Check if the parent exists 
-                # (sometimes tables are embedded into articles, 
+                    metadata["t"] = lab
+                # Check if the parent exists
+                # (sometimes tables are embedded into articles,
                 # but the articles are empty)
                 if parent_id is not None:
-                    metadata['pOf'] = parent_id
-                new_ci = {
-                    'm': metadata,
-                    'l': {'parts': parse_div_parts(child)}
-                }
+                    metadata["pOf"] = parent_id
+                new_ci = {"m": metadata, "l": {"parts": parse_div_parts(child)}}
                 new_cis.append(new_ci)
                 counter += 1
+
     return new_cis, counter
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/bnf_en/classes.py` & `impresso_text_importer-1.1.0/text_importer/importers/bnf_en/classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,78 +10,82 @@
 from time import strftime
 from typing import Any, Optional
 
 from bs4 import BeautifulSoup
 from bs4.element import NavigableString, Tag
 from impresso_commons.path import IssueDir
 
-from text_importer.importers import (CONTENTITEM_TYPES, 
-                                     CONTENTITEM_TYPE_ADVERTISEMENT, 
-                                     CONTENTITEM_TYPE_IMAGE,
-                                     CONTENTITEM_TYPE_TABLE)
+from text_importer.importers import (
+    CONTENTITEM_TYPES,
+    CONTENTITEM_TYPE_ADVERTISEMENT,
+    CONTENTITEM_TYPE_IMAGE,
+    CONTENTITEM_TYPE_TABLE,
+)
 from text_importer.importers.bnf.helpers import BNF_CONTENT_TYPES
-from text_importer.importers.mets_alto import (MetsAltoNewspaperIssue,
-                                               MetsAltoNewspaperPage)
-from text_importer.utils import get_issue_schema, get_page_schema
+from text_importer.importers.mets_alto import (
+    MetsAltoNewspaperIssue,
+    MetsAltoNewspaperPage,
+)
+from text_importer.utils import get_issue_schema, get_page_schema, get_reading_order
 
 IssueSchema = get_issue_schema()
 Pageschema = get_page_schema()
 
 logger = logging.getLogger(__name__)
 
-IIIF_ENDPOINT_URL = "https://gallica.bnf.fr/iiif/ark:/12148/"
-IIIF_SUFFIX = "full/full/0/default.jpg"
+IIIF_ENDPOINT_URI = "https://gallica.bnf.fr/iiif/ark:/12148/"
+IIIF_SUFFIX = "info.json"
+IIIF_MANIFEST_SUFFIX = "manifest.json"
 SECTION_TYPE = "section"
 
 type_translation = {
-    'illustration': CONTENTITEM_TYPE_IMAGE,
-    'advertisement': CONTENTITEM_TYPE_ADVERTISEMENT,
-    }
+    "illustration": CONTENTITEM_TYPE_IMAGE,
+    "advertisement": CONTENTITEM_TYPE_ADVERTISEMENT,
+}
 
 
 class BnfEnNewspaperPage(MetsAltoNewspaperPage):
     """Newspaper page in BNF-EN (Mets/Alto) format.
 
     Args:
         _id (str): Canonical page ID.
         number (int): Page number.
         filename (str): Name of the Alto XML page file.
         basedir (str): Base directory where Alto files are located.
-    
+
     Attributes:
         id (str): Canonical Page ID (e.g. ``GDL-1900-01-02-a-p0004``).
         number (int): Page number.
         page_data (dict[str, Any]): Page data according to canonical format.
         issue (NewspaperIssue): Issue this page is from.
         filename (str): Name of the Alto XML page file.
         basedir (str): Base directory where Alto files are located.
         encoding (str, optional): Encoding of XML file. Defaults to 'utf-8'.
         is_gzip (bool): Whether the page's corresponding file is in .gzip.
         ark_link (str): IIIF Ark identifier for this page.
     """
-    
-    def __init__(self, _id: str, number: int, 
-                 filename: str, basedir: str) -> None:
+
+    def __init__(self, _id: str, number: int, filename: str, basedir: str) -> None:
         super().__init__(_id, number, filename, basedir)
-        
-        page_tag = self.xml.find('Page')
-        self.page_width = float(page_tag.get('WIDTH'))
-    
+
+        page_tag = self.xml.find("Page")
+        self.page_width = float(page_tag.get("WIDTH"))
+
     def add_issue(self, issue: MetsAltoNewspaperIssue) -> None:
         self.issue = issue
         ark = issue.ark_link
-        self.page_data['iiif'] = os.path.join(
-            IIIF_ENDPOINT_URL, ark, "f{}".format(self.number), IIIF_SUFFIX
+        self.page_data["iiif_img_base_uri"] = os.path.join(
+            IIIF_ENDPOINT_URI, ark, "f{}".format(self.number)
         )
 
 
 class BnfEnNewspaperIssue(MetsAltoNewspaperIssue):
     """Newspaper Issue in BNF-EN (Mets/Alto) format.
 
-    All functions defined in this child class are specific to parsing 
+    All functions defined in this child class are specific to parsing
     BNF-Europeana Mets/Alto format.
 
     Args:
         issue_dir (IssueDir): Identifying information about the issue.
 
     Attributes:
         id (str): Canonical Issue ID (e.g. ``GDL-1900-01-02-a``).
@@ -96,296 +100,317 @@
             OCR/OLR coordinates to iiif format compliant ones.
         ark_link (str): IIIF Ark Id for this issue fetched on the Gallica API.
     """
 
     def __init__(self, issue_dir: IssueDir) -> None:
         self.ark_link = issue_dir.ark_link
         super().__init__(issue_dir)
-    
+
     def _find_pages(self) -> None:
         """Detect and create the issue pages using the relevant Alto XML files.
-        
+
         Created NewspaperPage instances are added to pages.
 
         Raises:
             e: Creating a BnfEnlNewspaperPage` raised an exception.
         """
-        alto_path = os.path.join(self.path, 'ALTO')
-        
+        alto_path = os.path.join(self.path, "ALTO")
+
         if not os.path.exists(alto_path):
-            logger.critical(f"Could not find pages for {self.id}")
-        
+            msg = f"Could not find pages for {self.id}, non-existing path: {alto_path}"
+            logger.critical(msg)
+            raise ValueError(msg)
+
         page_file_names = [
             file
             for file in os.listdir(alto_path)
-            if not file.startswith('.') and '.xml' in file
-            ]
-        
+            if not file.startswith(".") and ".xml" in file
+        ]
+
         page_numbers = []
-        
+
         for fname in page_file_names:
-            page_no = fname.split('.')[0].split('-')[1]
+            page_no = fname.split(".")[0].split("-")[1]
             page_numbers.append(int(page_no))
-        
+
         page_canonical_names = [
-            "{}-p{}".format(self.id, str(page_n).zfill(4))
-            for page_n in page_numbers
-            ]
-        
+            "{}-p{}".format(self.id, str(page_n).zfill(4)) for page_n in page_numbers
+        ]
+
         self.pages = []
         for filename, page_no, page_id in zip(
-                page_file_names, page_numbers, page_canonical_names
-                ):
+            page_file_names, page_numbers, page_canonical_names
+        ):
             try:
                 self.pages.append(
-                        BnfEnNewspaperPage(
-                                page_id,
-                                page_no,
-                                filename,
-                                alto_path
-                                )
-                        )
+                    BnfEnNewspaperPage(page_id, page_no, filename, alto_path)
+                )
             except Exception as e:
-                logger.error(f'Adding page {page_no} {page_id} {filename}',
-                             f'raised following exception: {e}')
-                raise e
-    
+                msg = f"Adding page {page_no} {page_id} {filename} raised following exception: {e}"
+                logger.error(msg)
+                raise Exception(msg) from e
+
     def _parse_content_parts(self, content_div: Tag) -> list[dict[str, Any]]:
         """Parse given div's children tags to create legacy `parts` component.
 
         Given the div of a content item, this function parses the children and
         constructs the legacy `parts` component.
 
         Args:
             content_div (Tag): The div containing the content item.
 
         Returns:
             list[dict[str, Any]]: List of dicts of each content part of item.
         """
         parts = []
         for child in content_div.children:
-            
+
             if isinstance(child, NavigableString):
                 continue
             elif isinstance(child, Tag):
-                type_attr = child.get('TYPE')
+                type_attr = child.get("TYPE")
                 comp_role = type_attr.lower() if type_attr else None
-                areas = child.findAll('area')
+                areas = child.findAll("area")
                 for area in areas:
-                    comp_id = area.get('BEGIN')
-                    comp_fileid = area.get('FILEID')
-                    comp_page_no = int(comp_fileid.replace('ALTO', ''))
-                    
+                    comp_id = area.get("BEGIN")
+                    comp_fileid = area.get("FILEID")
+                    comp_page_no = int(comp_fileid.replace("ALTO", ""))
+
                     parts.append(
                         {
-                            'comp_role': comp_role,
-                            'comp_id': comp_id,
-                            'comp_fileid': comp_fileid,
-                            'comp_page_no': comp_page_no
+                            "comp_role": comp_role,
+                            "comp_id": comp_id,
+                            "comp_fileid": comp_fileid,
+                            "comp_page_no": comp_page_no,
                         }
                     )
         return parts
-    
+
     def _get_ci_language(self, dmdid: str, mets_doc: BeautifulSoup) -> Optional[str]:
         """Find the language code of the CI with given DMDID.
 
         Languages are usually in a dmdSec at the beginning of a METS file.
 
         Args:
             dmdid (str): Identifier of the content item in the dmd section.
-            mets_doc (BeautifulSoup): Contents of the Mets XML file. 
+            mets_doc (BeautifulSoup): Contents of the Mets XML file.
 
         Returns:
             Optional[str]: Language or None if not present in Mets file.
         """
         lang = mets_doc.find("dmdSec", {"ID": dmdid})
         if lang is None:
             return None
-        lang = lang.find("mods:languageTerm") 
+        lang = lang.find("mods:languageTerm")
         if lang is None:
             return None
         return lang.text
-    
+
     def _parse_content_item(
         self, item_div: Tag, counter: int, mets_doc: BeautifulSoup
     ) -> dict[str, Any]:
         """Parse a content item div and returns the dictionary representing it.
 
         Args:
             item_div (Tag): Div of content item.
-            counter (int): Number of content items already added (needed to 
+            counter (int): Number of content items already added (needed to
                 generate canonical id).
-            mets_doc (BeautifulSoup): Contents of the Mets XML file. 
+            mets_doc (BeautifulSoup): Contents of the Mets XML file.
 
         Returns:
             dict[str, Any]: Resulting content item in canonical format.
         """
-        div_type = item_div.get('TYPE').lower()
+        div_type = item_div.get("TYPE").lower()
         # Translate types
         if div_type in type_translation:
             div_type = type_translation[div_type]
-        
+
         # Check if new content item is found (or if we need more translation)
         if div_type not in CONTENTITEM_TYPES:
-            logger.warning(f"Found new content item type: {div_type}")
-        
+            logger.warning("Found new content item type: %s", div_type)
+
         metadata = {
-            'id': "{}-i{}".format(self.id, str(counter).zfill(4)),
-            'tp': div_type,
-            'pp': [],
-            't': item_div.get('LABEL')
+            "id": "{}-i{}".format(self.id, str(counter).zfill(4)),
+            "tp": div_type,
+            "pp": [],
+            "t": item_div.get("LABEL"),
         }
-        
+
         # Get CI language
-        language = self._get_ci_language(item_div.get('DMDID'), mets_doc)
+        language = self._get_ci_language(item_div.get("DMDID"), mets_doc)
         if language is not None:
-            metadata['l'] = language
-        
+            metadata["l"] = language
+
         content_item = {
             "m": metadata,
             "l": {
-                "id": item_div.get('ID'),
-                "parts": self._parse_content_parts(item_div)
-            }
+                "id": item_div.get("ID"),
+                "parts": self._parse_content_parts(item_div),
+            },
         }
-        for p in content_item['l']['parts']:
+        for p in content_item["l"]["parts"]:
             pge_no = p["comp_page_no"]
-            if pge_no not in content_item['m']['pp']:
-                content_item['m']['pp'].append(pge_no)
-        
+            if pge_no not in content_item["m"]["pp"]:
+                content_item["m"]["pp"].append(pge_no)
+
         if div_type in [CONTENTITEM_TYPE_IMAGE, CONTENTITEM_TYPE_TABLE]:
-            content_item['m']['c'], content_item['iiif_link'] = self._get_image_info(content_item)
+            content_item["c"], content_item["m"]["iiif_link"] = self._get_image_info(
+                content_item
+            )
+
         return content_item
-    
+
     def _decompose_section(self, div: Tag) -> list[Tag]:
         """Recursively decompose the given `section` div into individual items.
 
-        In Mets, sometimes textblocks and images are withing `Section` tags. 
+        In Mets, sometimes textblocks and images are withing `Section` tags.
         Those need to be recursively decomposed to reach the content item divs.
 
         Args:
             div (Tag): The `Section` div to decompose.
 
         Returns:
             list[Tag]: List of all children divs not of type `Section`.
         """
         logger.info("Decomposing section type")
-        section_divs = [d for d in div.findAll("div") if
-                        d.get('TYPE').lower() in BNF_CONTENT_TYPES]
+        section_divs = [
+            d for d in div.findAll("div") if d.get("TYPE").lower() in BNF_CONTENT_TYPES
+        ]
         # Sort to get same IDS
-        section_divs = sorted(section_divs, key=lambda x: x.get('ID').lower())  
-        
+        section_divs = sorted(section_divs, key=lambda x: x.get("ID").lower())
+
         final_divs = []
         # Now do it recursively
         for d in section_divs:
-            d_type = d.get('TYPE')
+            d_type = d.get("TYPE")
             if d_type is not None:
                 if d_type.lower() == SECTION_TYPE:
                     # Recursively decompose
-                    final_divs += self._decompose_section(d)  
+                    final_divs += self._decompose_section(d)
                 else:
                     final_divs.append(d)
+
         return final_divs
-    
+
     def _parse_content_items(self) -> list[dict[str, Any]]:
         """Extract content item elements from the issue's Mets XML file.
 
         Returns:
             list[dict[str, Any]]: List of content items in canonical format.
         """
         content_items = []
         doc = self.xml
-        
+
         dmd_sections = doc.findAll("dmdSec")
         struct_map = doc.find("div", {"TYPE": "CONTENT"})
-        # Sort to have same naming
-        sorted_divs = sorted(dmd_sections, key=lambda x: x.get('ID').lower())
-        
+
+        # Sort to have same namings - reading order is added separately later
+        sorted_divs = sorted(dmd_sections, key=lambda x: x.get("ID").lower())
+
         counter = 1
         for d in sorted_divs:
-            div = struct_map.findAll("div", {"DMDID": d.get('ID')})
+            div = struct_map.findAll("div", {"DMDID": d.get("ID")})
             if len(div) == 0:
                 continue
-            elif len(div) > 1:
-                logger.warning(f"Multiple divs matching {d.get('ID')} "
-                               f"in structmap for {self.id}")
+            if len(div) > 1:
+                logger.warning(
+                    "Multiple divs matching %s in structmap for %s",
+                    d.get("ID"),
+                    self.id,
+                )
             else:
                 div = div[0]
-                div_type = div.get('TYPE').lower()
+                div_type = div.get("TYPE").lower()
                 if div_type == SECTION_TYPE:
                     section_divs = self._decompose_section(div)
                     for sd in section_divs:
                         content_items.append(self._parse_content_item(sd, counter, doc))
                         counter += 1
                 else:
                     content_items.append(self._parse_content_item(div, counter, doc))
                     counter += 1
+
+        # add the reading order to the items metadata
+        reading_order_dict = get_reading_order(content_items)
+        for item in content_items:
+            item["m"]["ro"] = reading_order_dict[item["m"]["id"]]
+
         return content_items
-    
-    def _get_image_info(
-        self, content_item: dict[str, Any]
-    ) -> tuple[list[int], str]:
+
+    def _get_image_info(self, content_item: dict[str, Any]) -> tuple[list[int], str]:
         """Given an image content item, get its coordinates and iiif url.
 
         TODO: Find an approach to reduce the number of calls to page.xml
 
         Args:
             content_item (dict[str, Any]): Content item in canonical format.
 
         Returns:
             tuple[list[int], str]: Content item coordinates and iiif url.
         """
         # Fetch the legacy parts
-        
+
         # Images cannot be on multiple pages
-        num_pages = len(content_item['m']['pp'])
+        num_pages = len(content_item["m"]["pp"])
         assert num_pages == 1, "Image is on more than one page"
-        
-        page_nb = content_item['m']['pp'][0]
+
+        page_nb = content_item["m"]["pp"][0]
         page = [p for p in self.pages if p.number == page_nb][0]
-        parts = content_item['l']['parts']
-        
+        parts = content_item["l"]["parts"]
+
         assert len(parts) >= 1, f"No parts for image {content_item['m']['id']}"
-        
+
         if len(parts) > 1:
-            logger.info(f"Found multiple parts for image "
-                        f"{content_item['m']['id']}, selecting largest one")
-        
+            logger.info(
+                "Found multiple parts for image %s, selecting largest one",
+                content_item["m"]["id"],
+            )
+
         page_doc = page.xml
         coords = None
         max_area = 0
         # Image can have multiple parts, choose largest one (with max area)
         for part in parts:
-            comp_id = part['comp_id']
-            
+            comp_id = part["comp_id"]
+
             elements = page_doc.findAll(["ComposedBlock", "TextBlock"], {"ID": comp_id})
             assert len(elements) <= 1, "Image comp_id matches multiple TextBlock tags"
             if len(elements) == 0:
                 continue
-            
+
             element = elements[0]
-            hpos, vpos= element.get('HPOS'), element.get('VPOS')
-            width, height =  element.get('WIDTH'), element.get('HEIGHT')
-            
+            hpos, vpos = element.get("HPOS"), element.get("VPOS")
+            width, height = element.get("WIDTH"), element.get("HEIGHT")
+
             # Select largest image
             area = int(float(width)) * int(float(height))
             if area > max_area:
                 max_area = area
-                coords = [int(float(hpos)), int(float(vpos)), 
-                          int(float(width)), int(float(height))]
-        
+                coords = [
+                    int(float(hpos)),
+                    int(float(vpos)),
+                    int(float(width)),
+                    int(float(height)),
+                ]
+
         # coords = convert_coordinates(coords, self.image_properties[page.number], page.page_width)
-        iiif_link = os.path.join(IIIF_ENDPOINT_URL, self.ark_link, "f{}".format(page.number),
-                                 ",".join([str(x) for x in coords]), 'full', '0', 'default.jpg')
-        
+        iiif_link = os.path.join(
+            IIIF_ENDPOINT_URI, self.ark_link, f"f{page.number}", IIIF_SUFFIX
+        )
+
         return coords, iiif_link
-    
+
     def _parse_mets(self) -> None:
         content_items = self._parse_content_items()
-        
+
+        iiif_manifest = os.path.join(
+            IIIF_ENDPOINT_URI, self.ark_link, IIIF_MANIFEST_SUFFIX
+        )
+
         self.issue_data = {
             "cdt": strftime("%Y-%m-%d %H:%M:%S"),
-            "i": content_items,
             "id": self.id,
+            "i": content_items,
             "ar": self.rights,
-            "pp": [p.id for p in self.pages]
+            "pp": [p.id for p in self.pages],
+            "iiif_manifest_uri": iiif_manifest,
         }
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/bnf_en/detect.py` & `impresso_text_importer-1.1.0/text_importer/importers/swa/detect.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,37 @@
-"""This module contains helper functions to find BNF-EN OCR data to import.
+"""This module contains helper functions to find SWA OCR data to be imported.
 """
+
+import json
 import logging
 import os
 from collections import namedtuple
-from datetime import datetime, timedelta
-from string import ascii_lowercase
-from typing import Dict, List, Optional
-
-import requests
-from bs4 import BeautifulSoup
-from dask import bag as db
+from datetime import date
+from typing import Optional
+
+import dask.bag as db
+import pandas as pd
 from impresso_commons.path.path_fs import _apply_datefilter
-from tqdm import tqdm
-from multiprocessing import Pool, cpu_count
+
+from text_importer.utils import get_access_right
 
 logger = logging.getLogger(__name__)
 
-EDITIONS_MAPPINGS = {
-    1: 'a',
-    2: 'b',
-    3: 'c',
-    4: 'd',
-    5: 'e'
-    }
-
-BnfEnIssueDir = namedtuple(
-        "IssueDirectory", [
-            'journal',
-            'date',
-            'edition',
-            'path',
-            'rights',
-            'ark_link'
-            ]
-        )
-"""A light-weight data structure to represent a newspaper issue in BNF Europeana
+SwaIssueDir = namedtuple(
+    "IssueDirectory",
+    [
+        "journal",
+        "date",
+        "edition",
+        "path",
+        "rights",
+        "pages",
+    ],
+)
+"""A light-weight data structure to represent a SWA newspaper issue.
 
 This named tuple contains basic metadata about a newspaper issue. They
 can then be used to locate the relevant data in the filesystem or to create
 canonical identifiers for the issue and its pages.
 
 Note:
     In case of newspaper published multiple times per day, a lowercase letter
@@ -47,275 +40,243 @@
 
 Args:
     journal (str): Newspaper ID.
     date (datetime.date): Publication date or issue.
     edition (str): Edition of the newspaper issue ('a', 'b', 'c', etc.).
     path (str): Path to the directory containing the issue's OCR data.
     rights (str): Access rights on the data (open, closed, etc.).
-    ark_link (str): Unique IIIF identifier associated with this issue.
+    pages (list): list of tuples (page_canonical_id, alto_path), alto_path is
+        the path from within the archive.
 
 >>> from datetime import date
->>> i = BnfEnIssueDir('BLB', date(1845,12,28), 'a', './Le-Gaulois/18820208_1', 'open')
+>>> i = IssueDirectory(
+        journal='arbeitgeber', 
+        date=datetime.date(1908, 7, 4), 
+        edition='a', path='./SWA/impresso_ocr/schwar_000059110_DSV01_1908.zip',
+        rights='open_public', 
+        pages=[(
+            'arbeitgeber-1908-07-04-a-p0001', 
+            'schwar_000059110_DSV01_1908/ocr/schwar_000059110_DSV01_1908_alto/BAU_1_000059110_1908_0001.xml'
+        ), ...]
+    )
 """
 
-API_JOURNAL_URL = "https://gallica.bnf.fr/services/Issues?ark={ark}/date"
-API_ISSUE_URL = "https://gallica.bnf.fr/services/Issues?ark={ark}/date&date={year}"
-IIIF_URL = "https://gallica.bnf.fr/iiif/ark:/12148/{issue_id}"
-
-API_MAPPING = {
-    "oerennes": "cb32830550k",
-    "oecaen": "cb41193642z",
-    "lematin": "cb328123058",
-    "lepji": "cb32836564q",
-    "jdpl": "cb39294634r",
-    "legaulois": "cb32779904b",
-    "lepetitparisien": "cb34419111x",
-}
-
-
-def get_api_id(
-    journal: str, api_issue: tuple[str, datetime.date], edition: str
-) -> str:
-    """Construct an ID given a journal name, date and edition.
-
-    Args:
-        journal (str): Journal name
-        api_issue (tuple[str, datetime.date]): Tuple of information fetched 
-            from the Gallica API.
-        edition (str): Edition of the issue.
-
-    Returns:
-        str: Canonical issue Id composed of journal name, date and edition.
-    """
-    date = api_issue[1]
-    return "{}-{}-{:02}-{:02}-{}".format(journal, date.year, date.month, 
-                                         date.day, ascii_lowercase[edition])
 
+def _get_csv_file(directory: str) -> str:
+    """Detect and return the path to the CSV file in the given directory.
 
-def get_issues_iiif_arks(journal_ark: tuple[str, str]) -> list[tuple[str, str]]:
-    """Given a journal name and Ark, fetch its issues' Ark in the Gallica API.
-
-    Each fo the Europeana journals have a journal-level Ark id, as well as 
-    issue-level IIIF Ark ids that can be fetched from the Gallica API using 
-    the journal Ark. 
-    The API also provides the day of the year for the corresponding issue.
-    Using both information, this function recreates all the issue canonical
-    for each collection and maps them to their respective issue IIIF Ark ids.
+    In SWA format, a mapping from the original IDs to the impresso ones is
+    required, and provided in a single CSV file.
 
     Args:
-        journal_ark (tuple[str, str]): Pair of journal and associated Ark id.
-
-    Returns:
-        list[tuple[str, str]]: Pairs of issue canonical Ids and IIIF Ark Ids.
-    """
-    journal, ark = journal_ark
-    
-    def get_date(dayofyear: str, year: int) -> datetime.date:
-        """Return the date corresponding to a day of year.
-
-        Args:
-            dayofyear (str): Numbered day in a year.
-            year (int): Year in question.
-
-        Returns:
-            datetime.date: Date corresponding to the day of year.
-        """
-        start_date = datetime(year=year, month=1, day=1)
-        return start_date + timedelta(days=int(dayofyear) - 1)
-    
-    print("Fetching for {}".format(journal))
-    r = requests.get(API_JOURNAL_URL.format(ark=ark))
-    years = BeautifulSoup(r.content, "lxml").findAll("year")
-    years = [int(x.contents[0]) for x in years]
-    
-    links = []
-    for year in tqdm(years):
-        # API requrest
-        url = API_ISSUE_URL.format(ark=API_MAPPING[journal], year=year)
-        r = requests.get(url)
-        api_issues = BeautifulSoup(r.content, "lxml").findAll("issue")
-        # Parse dates and editions
-        api_issues = [
-            (i.get("ark"), get_date(i.get("dayofyear"), year)) 
-            for i in api_issues
-        ]
-        
-        editions = []
-        for i, issue in enumerate(api_issues):
-            if i == 0:
-                editions.append(0)
-            else:
-                previous_same = api_issues[i - 1][1] == issue[1]
-                if previous_same:
-                    editions.append(editions[-1] + 1)
-                else:
-                    editions.append(0)
-        
-        api_issues = [
-            (get_api_id(journal, i, edition), i[0]) 
-            for i, edition in zip(api_issues, editions)
-        ]
-        links += api_issues
-    return links
-
+        directory (str): directory in which the CSV file should be.
 
-def construct_iiif_arks() -> dict[str, str]:
-    """Fetch the IIIF ark ids for each issue and map them to each other.
+    Raises:
+        ValueError: No CSV file was found in the directory.
+        ValueError: Multiple CSV files were found in the directory.
 
     Returns:
-        dict[str, str]: Mapping from issue canonical id to IIIF Ark id.
+        str: Path of the the CSV file found.
     """
-    with Pool(4) as p:
-        results = p.map(get_issues_iiif_arks, list(API_MAPPING.items()))
-    
-    iiif_arks = []
-    for i in results:
-        iiif_arks += i
-    return dict(iiif_arks)
-
+    files = os.listdir(directory)
+    files = [f for f in files if f.endswith(".csv")]
+    if len(files) == 0:
+        raise ValueError(f"Could not find csv file in {directory}")
+    elif len(files) > 1:
+        raise ValueError(f"Found multiple csv files in {directory}")
 
-def get_id(journal: str, date: datetime.date, edition: str) -> str:
-    """Construct the canonical issue ID given the necessary information.
+    return os.path.join(directory, files[0])
 
-    Args:
-        journal (str): Journal name.
-        date (datetime.date): Publication date.
-        edition (str): Edition of the issue.
 
-    Returns:
-        str: Resulting issue canonical Id.
-    """
-    return "{}-{}-{:02}-{:02}-{}".format(journal, date.year, date.month, 
-                                         date.day, edition)
+def _parse_csv_apply(part: pd.DataFrame) -> pd.Series:
+    """Helper to parse csv document, meant to be used on a grouped partition.
 
+    For all the pages in the current issue, matches the pages' canonical ID to
+    the corresponding XML file.
 
-def parse_dir(_dir: str, journal: str) -> str:
-    """Parse a directory and return the corresponding ID.
+    Note:
+        This function is called internally by :func:`detect_issues`.
 
     Args:
-        _dir (str): The directory (in Windows FS).
-        journal (str): Journal name to construct ID.
+        part (pd.DataFrame): Partition for current issue.
 
     Returns:
-        str: Issue canonical id.
+        pd.Series: Pages and archives for the issue.
     """
-    date_edition = _dir.split('\\')[-1].split('_')
-    if len(date_edition) == 1:
-        edition = 'a'
-        date = date_edition[0]
-    else:
-        date = date_edition[0]
-        edition = EDITIONS_MAPPINGS[int(date_edition[1])]
-    year, month, day = date[:4], date[4:6], date[6:8]
-    return "{}-{}-{}-{}-{}".format(journal, year, month, day, edition)
+    res = []
+    archives = set()
+    for i, x in part.iterrows():
+        res.append((x.identifier_impresso, x.full_xml_path))
+        archives.add(x.goobi_name + ".zip")
+    return pd.Series({"pages": res, "archives": archives})
 
 
-def dir2issue(
-    path: str, access_rights: dict, iiif_arks: dict[str, str]
-) -> Optional[BnfEnIssueDir]:
-    """Create a `BnfEnIssueDir` object from a directory path.
+def _get_issuedir(
+    row: pd.Series, journal_root: str, access_rights: dict
+) -> Optional[SwaIssueDir]:
+    """Create a ``SwaIssueDir`` from a row of the CSV file.
+
+    Each row of the CSV file contains the issue manifest ID, used to derive
+    the issue canonical ID, and the path the XML files of the issue's pages.
 
     Note:
         This function is called internally by :func:`detect_issues`.
 
     Args:
-        path (str): Path of issue.
-        access_rights (dict): Access rights (for conformity).
-        iiif_arks (dict): Mapping from issue canonical ids to iiif ark ids. 
+        row (pd.Series): Row of the CSV file  to an issue.
+        journal_root (str): Path to archive for current issue.
+        access_rights (dict): access rights of the issue's journal.
 
     Returns:
-        Optional[BnfEnIssueDir]: `BnfEnIssueDir` for given issue if the ark id 
-            was found on the Gallica API, None otherwise.
+        Optional[SwaIssueDir]: New `SwaIssueDir` object for the issue.
     """
-    journal, issue = path.split('/')[-2:]
-    
-    date, edition = issue.split('_')[:2]
-    date = datetime.strptime(date, '%Y%m%d').date()
-    journal = journal.lower().replace('-', '').strip()
-    edition = EDITIONS_MAPPINGS[int(edition)]
-    
-    id_ = get_id(journal, date, edition)
-    
-    if id_ not in iiif_arks:
-        return None
-    
-    return BnfEnIssueDir(journal=journal, date=date, edition=edition, path=path,
-                         rights="open-public", ark_link=iiif_arks[id_])
+    if len(row.archives) > 1:
+        logger.debug(
+            "Issue %s has more than one archive %s", row.manifest_id, row.archives
+        )
 
+    archive = os.path.join(journal_root, list(row.archives)[0])
 
-def detect_issues(base_dir: str, access_rights: str) -> List[BnfEnIssueDir]:
+    if os.path.isfile(archive):
+        split = row.manifest_id.split("-")[:-1]
+        if len(split) == 5:
+            try:
+                journal, year, mo, day, edition = split
+                pub_date = date(int(year), int(mo), int(day))
+                rights = get_access_right(journal, pub_date, access_rights)
+                return SwaIssueDir(
+                    journal,
+                    pub_date,
+                    edition,
+                    path=archive,
+                    rights=rights,
+                    pages=row.pages,
+                )
+            except ValueError as e:
+                logger.debug(
+                    "Issue %s does not have a regular name: %s", row.manifest_id, e
+                )
+        else:
+            logger.debug("Issue %s does not have regular name", row.manifest_id)
+    else:
+        logger.debug("Issue %s does not have archive", row.manifest_id)
+    return None
+
+
+def detect_issues(base_dir: str, access_rights: str) -> list[SwaIssueDir]:
     """Detect newspaper issues to import within the filesystem.
 
-    This function expects the directory structure that BNF-EN used to
-    organize the dump of Mets/Alto OCR data.
+    This function expects the directory structure that SWA used to
+    organize the dump of Alto OCR data.
+
+    The access rights information is not in place yet, but needs
+    to be specified by the content provider (SWA).
+
+    TODO: Add the directory structure of SWA OCR data dumps.
 
     Args:
         base_dir (str): Path to the base directory of newspaper data.
-        access_rights (str): Not used for this importer (kept for conformity).
+        access_rights (str): Path to ``access_rights.json`` file.
 
     Returns:
-        List[BnfEnIssueDir]: List of `BnfEnIssueDir` instances to import.
+        list[SwaIssueDir]: list of ``SwaIssueDir`` instances, to be imported.
     """
-    dir_path, dirs, files = next(os.walk(base_dir))
+    dir_path, dirs, _ = next(os.walk(base_dir))
     journal_dirs = [os.path.join(dir_path, _dir) for _dir in dirs]
-    issue_dirs = [
-        os.path.join(journal, _dir)
-        for journal in journal_dirs
-        for _dir in os.listdir(journal)
-    ]
-    
-    iiif_arks = construct_iiif_arks()
-    issue_dirs = [dir2issue(_dir, None, iiif_arks) for _dir in issue_dirs]
-    
-    initial_length = len(issue_dirs)
-    issue_dirs = [i for i in issue_dirs if i is not None]
-    logger.info(f"Removed {initial_length-len(issue_dirs)} problematic issues")
-
-    return issue_dirs
-
-
-def select_issues(
-    base_dir: str, config: dict, access_rights: str
-) -> Optional[List[BnfEnIssueDir]]:
+    journal_dirs = [(d, _get_csv_file(d)) for d in journal_dirs]
+
+    with open(access_rights, "r", encoding="utf-8") as f:
+        ar_dict = json.load(f)
+
+    results = []
+    for journal_root, csv_file in journal_dirs:
+        if os.path.isfile(csv_file):
+            df = (
+                pd.read_csv(csv_file)
+                .groupby("manifest_id")
+                .apply(_parse_csv_apply)
+                .reset_index()
+            )
+            result = df.apply(lambda r: _get_issuedir(r, journal_root, ar_dict), axis=1)
+            result = result[~result.isna()].values.tolist()
+            results += result
+        else:
+            logger.warning("Could not find csv file %s", csv_file)
+
+    return results
+
+
+def select_issues(base_dir: str, config: dict, access_rights: str) -> list[SwaIssueDir]:
     """Detect selectively newspaper issues to import.
 
     The behavior is very similar to :func:`detect_issues` with the only
     difference that ``config`` specifies some rules to filter the data to
     import. See `this section <../importers.html#configuration-files>`__ for
     further details on how to configure filtering.
 
+        The access rights information is not in place yet, but needs
+        to be specified by the content provider (SWA).
+
     Args:
         base_dir (str): Path to the base directory of newspaper data.
         config (dict): Config dictionary for filtering.
-        access_rights (str): Not used for this importer (kept for conformity).
+        access_rights (str): Path to ``access_rights.json`` file.
 
     Returns:
-        Optional[List[BnfEnIssueDir]]: `BnfEnIssueDir` instances to import.
+        list[SwaIssueDir]: list of ``SwaIssueDir`` instances, to be imported.
     """
     try:
-        filter_dict = config["newspapers"]
+        filter_dict = config.get("newspapers")
         exclude_list = config["exclude_newspapers"]
         year_flag = config["year_only"]
-    
     except KeyError:
-        logger.critical(f"The key [newspapers|exclude_newspapers|year_only] "
-                        "is missing in the config file.")
-        return
-    
+        logger.critical(
+            "The key [newspapers|exclude_newspapers|year_only] "
+            "is missing in the config file."
+        )
+        return []
+
+    exclude_flag = False if not exclude_list else True
+    msg = (
+        f"got filter_dict: {filter_dict}, "
+        f"\nexclude_list: {exclude_list}, "
+        f"\nyear_flag: {year_flag}"
+        f"\nexclude_flag: {exclude_flag}"
+    )
+    logger.debug(msg)
+
+    filter_newspapers = (
+        set(filter_dict.keys()) if not exclude_list else set(exclude_list)
+    )
+    logger.debug(
+        "got filter_newspapers: %s, with exclude flag: %s",
+        filter_newspapers,
+        exclude_flag,
+    )
+
     issues = detect_issues(base_dir, access_rights)
+
     issue_bag = db.from_sequence(issues)
-    selected_issues = (
-        issue_bag.filter(
-            lambda i: (
-                len(filter_dict) == 0 or i.journal in filter_dict.keys()
-            ) and i.journal not in exclude_list
-        ).compute()
+    selected_issues = issue_bag.filter(
+        lambda i: (len(filter_dict) == 0 or i.journal in filter_dict.keys())
+        and i.journal not in exclude_list
+    ).compute()
+
+    logger.info(
+        "%s newspaper issues remained after applying filter: %s",
+        len(selected_issues),
+        selected_issues,
     )
-    
+
     exclude_flag = False if not exclude_list else True
-    filtered_issues = _apply_datefilter(
-        filter_dict, selected_issues, year_only=year_flag
-    ) if not exclude_flag else selected_issues
-    logger.info(f"{len(filtered_issues)} newspaper issues remained "
-                f"after applying filter: {filtered_issues}")
-    
-    return filtered_issues
+    filtered_issues = (
+        _apply_datefilter(filter_dict, selected_issues, year_only=year_flag)
+        if not exclude_flag
+        else selected_issues
+    )
+    logger.info(
+        "%s newspaper issues remained after applying filter: %s",
+        len(filtered_issues),
+        filtered_issues,
+    )
+
+    return selected_issues
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/classes.py` & `impresso_text_importer-1.1.0/text_importer/importers/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,40 +40,38 @@
         journal (str): Newspaper unique identifier or name.
         path (str): Path to directory containing the issue's OCR data.
         date (datetime.date): Publication date of issue.
         issue_data (dict[str, Any]): Issue data according to canonical format.
         pages (list): List of :obj:`NewspaperPage` instances from this issue.
         rights (str): Access rights applicable to this issue.
     """
-    
+
     def __init__(self, issue_dir: IssueDir) -> None:
-        self.id = canonical_path(issue_dir, path_type='dir').replace('/', '-')
+        self.id = canonical_path(issue_dir, path_type="dir").replace("/", "-")
         self.edition = issue_dir.edition
         self.journal = issue_dir.journal
         self.path = issue_dir.path
         self.date = issue_dir.date
         self.issue_data = {}
         self._notes = []
         self.pages = []
         self.rights = issue_dir.rights
-    
+
     @abstractmethod
     def _find_pages(self) -> None:
         """Detect and create the issue pages using the relevant Alto XML files.
 
         Created :obj:`NewspaperPage` instances are added to :attr:`pages`.
         """
-        pass
-    
+
     @property
     def issuedir(self) -> IssueDir:
-        """`IssueDir`: IssueDirectory corresponding to this issue.
-        """
+        """`IssueDir`: IssueDirectory corresponding to this issue."""
         return IssueDir(self.journal, self.date, self.edition, self.path)
-    
+
     def to_json(self) -> str:
         """Validate ``self.issue_data`` & serialize it to string.
 
         Note:
             Validation adds a substantial overhead to computing time. For
             serialization of large amounts of issues it is recommendable to
             bypass schema validation.
@@ -84,128 +82,124 @@
 
 class NewspaperPage(ABC):
     """Abstract class representing a newspaper page.
 
     Each text importer needs to define a subclass of ``NewspaperPage`` which
     specifies the logic to handle OCR data in a given format (e.g. Alto).
 
-    Args: 
+    Args:
         _id (str): Canonical Page ID (e.g. ``GDL-1900-01-02-a-p0004``).
         number (int): Page number.
 
     Attributes:
         id (str): Canonical Page ID (e.g. ``GDL-1900-01-02-a-p0004``).
         number (int): Page number.
         page_data (dict[str, Any]): Page data according to canonical format.
         issue (NewspaperIssue | None): Issue this page is from.
     """
-    
+
     def __init__(self, _id: str, number: int) -> None:
         self.id = _id
         self.number = number
         self.page_data = {}
         self.issue = None
-    
+
     def to_json(self) -> str:
         """Validate ``self.page.data`` & serialize it to string.
 
         Note:
             Validation adds a substantial overhead to computing time. For
             serialization of large amounts of pages it is recommendable to
             bypass schema validation.
         """
         page = Pageschema(**self.page_data)
         return page.serialize()
-    
+
     @abstractmethod
     def add_issue(self, issue: NewspaperIssue) -> None:
         """Add to a page object its parent, i.e. the newspaper issue.
 
         This allows each page to preserve contextual information coming from
         the newspaper issue.
 
         Args:
             issue (NewspaperIssue): Newspaper issue containing this page.
         """
-        pass
-    
+
     @abstractmethod
     def parse(self) -> None:
         """Process the page XML file and transform into canonical Page format.
 
         Note:
             This lazy behavior means that the page contents are not processed
             upon creation of the page object, but only once the ``parse()``
             method is called.
         """
-        pass
 
 
 class ZipArchive(object):
     """Archive document to be temporarily unpacked.
-    
+
     It is usually unpacked into a temp directory to avoid jamming the memory.
 
     Args:
         archive (ZipFile): Zip archive containing files with OCR data.
         temp_dir (str): Directory used for temporary storage of the contents.
 
     Attributes:
         name_list (list[str]): List of filenames in the archive.
         dir (str): Path to directory in which archive contents are.
     """
-    
+
     def __init__(self, archive: ZipFile, temp_dir: str) -> None:
-        logger.debug(f"Extracting archive in {temp_dir}")
+        logger.debug("Extracting archive in %s", temp_dir)
         self.name_list = archive.namelist()
         self.dir = temp_dir
         self.extract_archive(archive)
         archive.close()
-    
+
     def extract_archive(self, archive: ZipFile) -> None:
         """Recursively extract all files from the archive.
 
         Args:
             archive (ZipFile): Archive to unpack.
         """
         if not os.path.exists(self.dir):
-            logger.debug(f"Creating {self.dir}")
+            logger.debug("Creating %s", self.dir)
             try:
                 os.makedirs(self.dir)
-            except FileExistsError as e:
+            except FileExistsError:
                 pass
         for f in archive.filelist:
             if f.file_size > 0:
                 try:
                     archive.extract(f.filename, path=self.dir)
-                except FileExistsError as e:
+                except FileExistsError:
                     pass
-    
+
     def namelist(self) -> list[str]:
-        """list[str]: List of filenames in the archive.
-        """
+        """list[str]: List of filenames in the archive."""
         return self.name_list
-    
+
     def read(self, file: str) -> bytes:
         """Read given file in binary mode.
 
         Args:
             file (str): File to read.
 
         Returns:
             bytes: File contents as bytes.
         """
         path = os.path.join(self.dir, file)
-        with open(path, 'rb') as f:
+        with open(path, "rb") as f:
             f_bytes = f.read()
         return f_bytes
-    
+
     def cleanup(self) -> None:
-        """Recursively delete the unpacked archive.
-        """
-        logging.info(f"Deleting archive {self.dir}")
+        """Recursively delete the unpacked archive."""
+        logging.info("Deleting archive %s", self.dir)
         shutil.rmtree(self.dir)
         prev_dir = os.path.split(self.dir)[0]
         while os.path.isdir(prev_dir) and len(os.listdir(prev_dir)) == 0:
-            logging.info(f"Deleting {prev_dir}")
+            logging.info("Deleting %s", prev_dir)
             os.rmdir(prev_dir)
             prev_dir = os.path.split(prev_dir)[0]
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/core.py` & `impresso_text_importer-1.1.0/text_importer/importers/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,84 +17,85 @@
 import shutil
 from copy import copy
 from itertools import groupby
 from json import JSONDecodeError
 from pathlib import Path
 from time import strftime
 from typing import Tuple, Type
+from botocore.exceptions import BotoCoreError
 
 import jsonlines
 from dask import bag as db
 from dask.distributed import Client
 from filelock import FileLock
 from impresso_commons.path.path_fs import IssueDir, canonical_path
 from impresso_commons.text.rebuilder import cleanup
 from impresso_commons.utils import chunk
 from impresso_commons.utils.s3 import get_s3_resource
+from impresso_commons.versioning.data_manifest import DataManifest
+from impresso_commons.versioning.helpers import counts_for_canonical_issue
 from smart_open import open as smart_open_function
 
 from text_importer.importers.classes import NewspaperIssue, NewspaperPage
 from text_importer.importers.olive.classes import OliveNewspaperIssue
 from text_importer.importers.swa.classes import SWANewspaperIssue
 
 logger = logging.getLogger(__name__)
 
 
 def write_error(
     thing: NewspaperIssue | NewspaperPage | IssueDir,
-    error: Exception, 
-    failed_log: str
+    error: Exception,
+    failed_log: str | None,
 ) -> None:
     """Write the given error of a failed import to the `failed_log` file.
 
     Args:
         thing (NewspaperIssue | NewspaperPage | IssueDir): Object for which
             the error occurred.
         error (Exception): Error that occurred and should be logged.
         failed_log (str): Path to log file for failed imports.
     """
-    logger.error(f'Error when processing {thing}: {error}')
+    logger.error("Error when processing %s: %s", thing, error)
     logger.exception(error)
     if isinstance(thing, NewspaperPage):
         issuedir = thing.issue.issuedir
     elif isinstance(thing, NewspaperIssue):
         issuedir = thing.issuedir
     else:
         # if it's neither an issue nor a page it must be an issuedir
         issuedir = thing
 
-    note = (
-        f"{canonical_path(issuedir, path_type='dir').replace('/', '-')}: "
-        f"{error}"
-    )
+    note = f"{canonical_path(issuedir, path_type='dir').replace('/', '-')}: " f"{error}"
 
-    with open(failed_log, "a+") as f:
-        f.write(note + "\n")
+    if failed_log is not None:
+        with open(failed_log, "a+", encoding="utf-8") as f:
+            f.write(note + "\n")
 
 
 def dir2issue(
     issue: IssueDir,
     issue_class: Type[NewspaperIssue],
     failed_log: str | None = None,
-    image_dirs: str | None = None, 
-    temp_dir: str | None = None
+    image_dirs: str | None = None,
+    temp_dir: str | None = None,
 ) -> NewspaperIssue | None:
     """Instantiate a `NewspaperIssue` object from an `IssueDir`.
 
     Any instantiation leading to an exception is logged to a specific file
     only containing issues which could not be imported.
 
     Args:
         issue (IssueDir): `IssueDir` representing the issue to instantiate.
         issue_class (Type[NewspaperIssue]): Type of `NewspaperIssue` to use.
         failed_log (str | None, optional): Path to the log file used if the
             instantiation was not successful. Defaults to None.
         image_dirs (str | None, optional): Path to the directory containing the
             information on images, only for Olive importer. Defaults to None.
-        temp_dir (str | None, optional): Temporary directory to unpack the 
+        temp_dir (str | None, optional): Temporary directory to unpack the
             issue's zip archive into. Defaults to None.
 
     Returns:
         NewspaperIssue | None: A new `NewspaperIssue` instance, or `None` if
             the instantiation triggered an exception.
     """
     try:
@@ -110,16 +111,16 @@
         return None
 
 
 def dirs2issues(
     issues: list[IssueDir],
     issue_class: Type[NewspaperIssue],
     failed_log: str | None = None,
-    image_dirs: str | None = None, 
-    temp_dir: str | None = None
+    image_dirs: str | None = None,
+    temp_dir: str | None = None,
 ) -> list[NewspaperIssue]:
     """Instantiate the `NewspaperIssue` objects to import to Impresso's format.
 
     Any `NewspaperIssue` for which the instantiation is unsuccessful
     will be logged, along with the triggered error.
 
     Args:
@@ -133,27 +134,25 @@
             archives of issues into. Defaults to None.
 
     Returns:
         list[NewspaperIssue]: List of `NewspaperIssue` instances to import.
     """
     ret = []
     for issue in issues:
-        np_issue = dir2issue(
-            issue, issue_class, failed_log, image_dirs, temp_dir
-        )
+        np_issue = dir2issue(issue, issue_class, failed_log, image_dirs, temp_dir)
         if np_issue is not None:
             ret.append(np_issue)
     return ret
 
 
 def issue2pages(issue: NewspaperIssue) -> list[NewspaperPage]:
     """Flatten an issue into a list of their pages.
 
     As an issue consists of several pages, this function is useful
-    in order to process each page in a truly parallel fashion. 
+    in order to process each page in a truly parallel fashion.
 
     Args:
         issue (NewspaperIssue): Issue to collect the pages of.
 
     Returns:
         list[NewspaperPage]: List of pages of the given issue.
     """
@@ -161,64 +160,56 @@
     for page in issue.pages:
         page.add_issue(issue)
         pages.append(page)
     return pages
 
 
 def serialize_pages(
-    pages: list[NewspaperPage],
-    output_dir: str | None = None
+    pages: list[NewspaperPage], output_dir: str | None = None
 ) -> list[Tuple[IssueDir, str]]:
     """Serialize a list of pages to an output directory.
 
     Args:
         pages (list[NewspaperPage]): Input newspaper pages.
-        output_dir (str | None, optional): Path to the output directory. 
+        output_dir (str | None, optional): Path to the output directory.
             Defaults to None.
 
     Returns:
-        list[Tuple[IssueDir, str]]: A list of tuples (`IssueDir`, `path`), 
-            where the `IssueDir` object represents the issue to which pages 
+        list[Tuple[IssueDir, str]]: A list of tuples (`IssueDir`, `path`),
+            where the `IssueDir` object represents the issue to which pages
             belong, and `path` the path to the individual page JSON file.
     """
     result = []
 
     for page in pages:
 
         issue_dir = copy(page.issue.issuedir)
 
-        out_dir = os.path.join(
-            output_dir,
-            canonical_path(issue_dir, path_type="dir")
-        )
+        out_dir = os.path.join(output_dir, canonical_path(issue_dir, path_type="dir"))
 
         if not os.path.exists(out_dir):
             os.makedirs(out_dir)
 
         canonical_filename = canonical_path(
-            issue_dir,
-            "p" + str(page.number).zfill(4),
-            ".json"
+            issue_dir, "p" + str(page.number).zfill(4), ".json"
         )
 
         out_file = os.path.join(out_dir, canonical_filename)
 
-        with open(out_file, 'w', encoding='utf-8') as jsonfile:
+        with open(out_file, "w", encoding="utf-8") as jsonfile:
             json.dump(page.page_data, jsonfile)
-            logger.info(f"Written page \'{page.number}\' to {out_file}")
+            logger.info("Written page '%s' to %s", page.number, out_file)
         result.append((issue_dir, out_file))
 
-    # TODO: this can be deleted, I believe as it has no effect
+    # this can be deleted, I believe as it has no effect
     gc.collect()
     return result
 
 
-def process_pages(
-    pages: list[NewspaperPage], failed_log: str
-) -> list[NewspaperPage]:
+def process_pages(pages: list[NewspaperPage], failed_log: str) -> list[NewspaperPage]:
     """Given a list of pages, trigger the ``.parse()`` method of each page.
 
     Args:
         pages (list[NewspaperPage]): Input newspaper pages.
         failed_log (str): File path of failed log.
 
     Returns:
@@ -238,338 +229,378 @@
     issues: list[IssueDir],
     out_dir: str,
     s3_bucket: str | None,
     issue_class: Type[NewspaperIssue],
     image_dirs: str | None,
     temp_dir: str | None,
     chunk_size: int | None,
+    manifest: DataManifest,
     client: Client | None = None,
 ) -> None:
     """Import a bunch of newspaper issues.
 
     Args:
         issues (list[IssueDir]): Issues to import.
         out_dir (str): Output directory for the json files.
         s3_bucket (str | None): Output s3 bucket for the json files.
         issue_class (Type[NewspaperIssue]): Newspaper issue class to import,
             (Child of ``NewspaperIssue``).
-        image_dirs (str | None): Directory of images for Olive format, 
+        image_dirs (str | None): Directory of images for Olive format,
             (can be multiple).
         temp_dir (str | None): Temporary directory for extracting archives
             (applies only to importers make use of ``ZipArchive``).
         chunk_size (int | None): Chunk size in years used to process issues.
     """
-    msg = f'Issues to import: {len(issues)}'
+    msg = f"Issues to import: {len(issues)}"
     logger.info(msg)
     failed_log_path = os.path.join(
-        out_dir,
-        f'failed-{strftime("%Y-%m-%d-%H-%M-%S")}.log'
+        out_dir, f'failed-{strftime("%Y-%m-%d-%H-%M-%S")}.log'
     )
     if chunk_size is not None:
         csize = int(chunk_size)
         chunks = groupby(
-            sorted(issues, key=lambda x: x.date.year), 
-            lambda x: x.date.year - (x.date.year % csize)
+            sorted(issues, key=lambda x: x.date.year),
+            lambda x: x.date.year - (x.date.year % csize),
         )
 
         chunks = [(year, list(issues)) for year, issues in chunks]
-        logger.info(f"Dividing issues into chunks of {chunk_size} years "
-                    f"({len(chunks)} chunks in total)")
+        msg = (
+            f"Dividing issues into chunks of {chunk_size} years "
+            f"({len(chunks)} chunks in total)"
+        )
+        logger.info(msg)
         for year, issue_chunk in chunks:
-            logger.info(f"Chunk of period {year} - {year + csize - 1} covers "
-                        f"{len(issue_chunk)} issues")
+            msg = (
+                f"Chunk of period {year} - {year + csize - 1} covers "
+                f"{len(issue_chunk)} issues"
+            )
+            logger.info(msg)
     else:
         chunks = [(None, issues)]
 
     for year, issue_chunk in chunks:
         if year is None:
-            period = 'all years'
+            period = "all years"
         else:
-            period = f'{year} - {year + csize - 1}'
+            period = f"{year} - {year + csize - 1}"
 
         temp_issue_bag = db.from_sequence(issue_chunk, partition_size=20)
 
         issue_bag = temp_issue_bag.map_partitions(
             dirs2issues,
             issue_class=issue_class,
             failed_log=failed_log_path,
             image_dirs=image_dirs,
-            temp_dir=temp_dir
+            temp_dir=temp_dir,
         ).persist()
 
-        logger.info(f'Start compressing issues for {period}')
+        logger.info("Start compressing issues for %s", period)
 
         compressed_issue_files = (
-            issue_bag.groupby(lambda i: (i.journal, i.date.year)) 
-            .starmap(compress_issues, 
-                     output_dir=out_dir,
-                     failed_log=failed_log_path) 
+            issue_bag.groupby(lambda i: (i.journal, i.date.year))
+            .starmap(compress_issues, output_dir=out_dir, failed_log=failed_log_path)
             .compute()
         )
 
-        logger.info(f'Done compressing issues for {period}')
+        logger.info("Done compressing issues for %s, updating the manifest...", period)
+        # Once the issues were written to the fs without issues, add their info to the manifest
+        for index, (np_year, filepath, yearly_stats) in enumerate(
+            compressed_issue_files
+        ):
+            manifest.add_count_list_by_title_year(
+                np_year.split("-")[0], np_year.split("-")[1], yearly_stats
+            )
+            # remove the yearly stats from the filenames
+            compressed_issue_files[index] = (np_year, filepath)
 
-        logger.info(f'Start uploading issues for {period}')
+        logger.info("Start uploading issues for %s", period)
 
         # NOTE: As a function of the partitioning size and the number of issues,
         # the issues of a single year may be assigned to different partitions.
         # To prevent further processing before the compressed issues of a single year is completed,
         # the steps of compressing and uploading/deleting are separated from each other.
         # Moreover, the issues are deduplicated after compressing due to the unpredictable partitioning.
         # If not respected, the import may result in incomplete issue files and non-reproducible errors.
         # TODO: The issues should be processed within a dask dataframe instead of bag
         # to get cleaner code while ensuring proper partitioning.
 
-        (db.from_sequence(set(compressed_issue_files)) 
-         .starmap(upload_issues, bucket_name=s3_bucket)
-         .starmap(cleanup).compute())
+        (
+            db.from_sequence(set(compressed_issue_files))
+            .starmap(upload_issues, bucket_name=s3_bucket, failed_log=failed_log_path)
+            .starmap(cleanup)
+            .compute()
+        )
 
-        logger.info(f'Done uploading issues for {period}')
+        logger.info("Done uploading issues for %s", period)
 
         processed_issues = list(issue_bag)
         random.shuffle(processed_issues)
 
         chunks = chunk(processed_issues, 400)
 
         for chunk_n, chunk_of_issues in enumerate(chunks):
-            logger.info(f'Processing chunk {chunk_n} of pages for {period}')
+            logger.info("Processing chunk %s of pages for %s", chunk_n, period)
 
             pages_bag = (
                 db.from_sequence(chunk_of_issues, partition_size=2)
                 .map(issue2pages)
                 .flatten()
                 .map_partitions(process_pages, failed_log=failed_log_path)
                 .map_partitions(serialize_pages, output_dir=out_dir)
             )
 
-            pages_out_dir = os.path.join(out_dir, 'pages')
+            pages_out_dir = os.path.join(out_dir, "pages")
             Path(pages_out_dir).mkdir(exist_ok=True)
 
-            logger.info(f'Start compressing and uploading pages '
-                        f'of chunk {chunk_n} for {period}')
+            logger.info(
+                "Start compressing and uploading pages of chunk %s for %s",
+                chunk_n,
+                period,
+            )
             pages_bag = (
                 pages_bag.groupby(
-                    lambda x: canonical_path(
-                        x[0], path_type='dir'
-                    ).replace('/', '-')
+                    lambda x: canonical_path(x[0], path_type="dir").replace("/", "-")
                 )
                 .starmap(
-                    compress_pages, suffix='pages', output_dir=pages_out_dir
+                    compress_pages,
+                    suffix="pages",
+                    output_dir=pages_out_dir,
+                    failed_log=failed_log_path,
                 )
-                .starmap(upload_pages, bucket_name=s3_bucket) 
-                .starmap(cleanup) 
+                .starmap(
+                    upload_pages, bucket_name=s3_bucket, failed_log=failed_log_path
+                )
+                .starmap(cleanup)
                 .compute()
             )
 
-            logger.info(f'Done compressing and uploading pages '
-                        f'of chunk {chunk_n} for {period}')
+            logger.info(
+                "Done compressing and uploading pages of chunk %s for %s",
+                chunk_n,
+                period,
+            )
 
-        # free some dask memory 
+        # free some dask memory
         if client:
             # if client is defined here
-            client.cancel(issue_bag) 
+            client.cancel(issue_bag)
         else:
             del issue_bag
 
     remove_filelocks(out_dir)
 
+    # finalize and compute the manifest
+    manifest.compute(export_to_git_and_s3=True)
+    # manifest.validate_and_export_manifest(push_to_git=False)
+
     if temp_dir is not None and os.path.isdir(temp_dir):
         shutil.rmtree(temp_dir, ignore_errors=True)
 
     logger.info("---------- Done ----------")
 
     if client:
         # shutdown dask client once processing is done.
         client.shutdown()
 
 
 def compress_pages(
     key: str,
     json_files: list[str],
     output_dir: str,
-    suffix: str = ""
+    suffix: str = "",
+    failed_log: str | None = None,
 ) -> Tuple[str, str]:
     """Merge a set of JSON line files into a single compressed archive.
 
     Args:
         key (str): Canonical ID of the newspaper issue (e.g. GDL-1900-01-02-a).
         json_files (list[str]): Paths of input JSON line files.
         output_dir (str): Directory where to write the output file.
         suffix (str, optional): Suffix to add to the filename. Defaults to "".
 
     Returns:
         Tuple[str, str]: Sorting key [0] and path to serialized file [1].
     """
-    newspaper, year, month, day, edition = key.split('-')
+    newspaper, year, month, day, edition = key.split("-")
     suffix_string = "" if suffix == "" else f"-{suffix}"
-    filename = (
-        f'{newspaper}-{year}-{month}-{day}-{edition}'
-        f'{suffix_string}.jsonl.bz2'
-    )
+    filename = f"{newspaper}-{year}-{month}-{day}-{edition}{suffix_string}.jsonl.bz2"
     filepath = os.path.join(output_dir, filename)
-    logger.info(f'Compressing {len(json_files)} JSON files into {filepath}')
+    logger.info("Compressing %s JSON files into %s", len(json_files), filepath)
 
-    with smart_open_function(filepath, 'wb') as fout:
+    with smart_open_function(filepath, "wb") as fout:
         writer = jsonlines.Writer(fout)
 
         items_count = 0
         for issue, json_file in json_files:
 
-            with open(json_file, 'r') as inpf:
+            with open(json_file, "r", encoding="utf-8") as inpf:
                 try:
                     item = json.load(inpf)
                     writer.write(item)
                     items_count += 1
                 except JSONDecodeError as e:
-                    logger.error(f'Reading data from {json_file} failed')
+                    logger.error("Reading data from %s failed", json_file)
                     logger.exception(e)
+                    write_error(filepath, e, failed_log)
             logger.info(
-                f'Written {items_count} docs from {json_file} to {filepath}'
+                "Written %s docs from %s to %s", items_count, json_file, filepath
             )
 
         writer.close()
 
     return key, filepath
 
 
 def compress_issues(
     key: Tuple[str, int],
     issues: list[NewspaperIssue],
     output_dir: str | None = None,
     failed_log: str | None = None,
-) -> Tuple[str, str]:
+) -> Tuple[str, str, list[dict[str, int]]]:
     """Compress issues of the same Journal-year and save them in a json file.
 
     First check if the file exists, load it and then over-write/add the newly
     generated issues.
     The compressed ``.bz2`` output file is a JSON-line file, where each line
     corresponds to an individual and issue document in the canonical format.
+    Finally, yearly statistics are computed on the issues and included in the
+    returned values.
 
     Args:
-        key (Tuple[str, int]): Newspaper ID and year of input issues 
+        key (Tuple[str, int]): Newspaper ID and year of input issues
             (e.g. `(GDL, 1900)`).
         issues (list[NewspaperIssue]): A list of `NewspaperIssue` instances.
         output_dir (str | None, optional): Output directory. Defaults to None.
         failed_log (str | None, optional): Path to the log file used when an
             instantiation was not successful. Defaults to None.
 
     Returns:
-        Tuple[str, str]: Label following the template `<NEWSPAPER>-<YEAR>` and 
-            the path to the the compressed `.bz2` file.
+        Tuple[str, str]: Label following the template `<NEWSPAPER>-<YEAR>`, the path to
+            the the compressed `.bz2` file, and the statistics computed on the issues.
     """
     newspaper, year = key
-    filename = f'{newspaper}-{year}-issues.jsonl.bz2'
+    filename = f"{newspaper}-{year}-issues.jsonl.bz2"
     filepath = os.path.join(output_dir, filename)
-    logger.info(f'Compressing {len(issues)} JSON files into {filepath}')
+    logger.info("Compressing %s JSON files into %s", len(issues), filepath)
 
     # put a file lock to avoid the overwriting of files due to parallelization
     lock = FileLock(filepath + ".lock", timeout=13)
-
+    items = [issue.issue_data for issue in issues]
     try:
         with lock:
-            with smart_open_function(filepath, 'ab') as fout:
+            with smart_open_function(filepath, "ab") as fout:
                 writer = jsonlines.Writer(fout)
 
-                items = [issue.issue_data for issue in issues]
+                # items = [issue.issue_data for issue in issues]
                 writer.write_all(items)
 
-                logger.info(f'Written {len(items)} issues to {filepath}')
+                logger.info("Written %s issues to %s", len(items), filepath)
                 writer.close()
     except Exception as e:
-        logger.error(f"Error for {filepath}")
-        logger.exception(e)
+        logger.error("Error for %s: %s", filepath, e)
         write_error(filepath, e, failed_log)
+    else:
+        # Once the issues were written without problems, add their info to the manifest
+        yearly_stats = []
+        for i in items:
+            yearly_stats.append(counts_for_canonical_issue(i))
 
-    return f'{newspaper}-{year}', filepath
+    return f"{newspaper}-{year}", filepath, yearly_stats
 
 
 def upload_issues(
     sort_key: str,
     filepath: str,
-    bucket_name: str | None = None
+    bucket_name: str | None = None,
+    failed_log: str | None = None,
 ) -> Tuple[bool, str]:
     """Upload an issues JSON-line file to a given S3 bucket.
 
     `sort_key` is expected to be the concatenation of newspaper ID and year.
 
     Args:
         sort_key (str): Key used to group articles (e.g. "GDL-1900").
         filepath (str): Path of the file to upload to S3.
         bucket_name (str | None, optional): Name of S3 bucket where to upload
             the file. Defaults to None.
+        failed_log (str | None, optional): Path to file where to log errors.
 
     Returns:
         Tuple[bool, str]: Whether the upload was successful and the path to the
             uploaded file.
     """
     # create connection with bucket
     # copy contents to s3 key
-    newspaper, year = sort_key.split('-')
-    key_name = "{}/{}/{}".format(
-        newspaper,
-        "issues",
-        os.path.basename(filepath)
-    )
+    newspaper, _ = sort_key.split("-")
+    key_name = "{}/{}/{}".format(newspaper, "issues", os.path.basename(filepath))
     s3 = get_s3_resource()
     if bucket_name is not None:
         try:
             bucket = s3.Bucket(bucket_name)
             bucket.upload_file(filepath, key_name)
-            logger.info(f'Uploaded {filepath} to {key_name}')
+            logger.info("Uploaded %s to %s", filepath, key_name)
             return True, filepath
-        except Exception as e:
-            logger.error(f'The upload of {filepath} failed with error {e}')
+        except BotoCoreError as e:
+            logger.error("The upload of %s failed with error %s", filepath, e)
+            write_error(filepath, e, failed_log)
     else:
-        logger.info(f'Bucket name is None, not uploading issue {filepath}.')
+        logger.info("Bucket name is None, not uploading issue %s.", filepath)
     return False, filepath
 
 
-def upload_pages( 
+def upload_pages(
     sort_key: str,
     filepath: str,
-    bucket_name: str | None = None
+    bucket_name: str | None = None,
+    failed_log: str | None = None,
 ) -> Tuple[bool, str]:
     """Upload a page JSON file to a given S3 bucket.
 
     Args:
         sort_key (str): the key used to group articles (e.g. "GDL-1900").
         filepath (str): Path of the file to upload to S3.
         bucket_name (str | None, optional): Name of S3 bucket where to upload
             the file. Defaults to None.
+        failed_log (str | None, optional): Path to file where to log errors.
 
     Returns:
         Tuple[bool, str]: Whether the upload was successful and the path to the
             uploaded file.
     """
     # create connection with bucket
     # copy contents to s3 key
-    newspaper, year, month, day, edition = sort_key.split('-')
+    newspaper, year, _, _, _ = sort_key.split("-")
     key_name = "{}/pages/{}/{}".format(
-        newspaper,
-        f'{newspaper}-{year}',
-        os.path.basename(filepath)
+        newspaper, f"{newspaper}-{year}", os.path.basename(filepath)
     )
     s3 = get_s3_resource()
     if bucket_name is not None:
         try:
             bucket = s3.Bucket(bucket_name)
             bucket.upload_file(filepath, key_name)
-            logger.info(f'Uploaded {filepath} to {key_name}')
+            logger.info("Uploaded %s to %s", filepath, key_name)
             return True, filepath
-        except Exception as e:
-            logger.error(f'The upload of {filepath} failed with error {e}')
+        except BotoCoreError as e:
+            logger.error("The upload of %s failed with error %s", filepath, e)
+            write_error(filepath, e, failed_log)
     else:
-        logger.info(f'Bucket name is None, not uploading page {filepath}.')
+        logger.info("Bucket name is None, not uploading page %s.", filepath)
+
     return False, filepath
 
 
 def remove_filelocks(output_dir: str) -> None:
     """Remove all files ending with .lock in a directory.
 
     Args:
         output_dir (str): Path to directory containing file locks.
     """
     files = os.listdir(output_dir)
 
     for file in files:
-        if file.endswith(".lock"):
-            os.remove(os.path.join(output_dir, file))
+        try:
+            if file.endswith(".lock"):
+                os.remove(os.path.join(output_dir, file))
+        except FileNotFoundError as e:
+            logger.error(
+                "File %s could not be removed as it does not exist: %s.", file, e
+            )
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/fedgaz/classes.py` & `impresso_text_importer-1.1.0/text_importer/importers/fedgaz/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from text_importer.importers.classes import NewspaperIssue
 from text_importer.importers.tetml import TetmlNewspaperIssue, TetmlNewspaperPage
 from text_importer.importers.tetml.parsers import tetml_parser
 from text_importer.importers.tetml.helpers import compute_bb
 
 logger = logging.getLogger(__name__)
 
-IMPRESSO_IIIF_BASEURI = "https://impresso-project.ch/api/proxy/iiif/"
+IIIF_ENDPOINT_URI = "https://impresso-project.ch/api/proxy/iiif/"
 
 
 class TokPosition(namedtuple("TokPosition", "art page reg para line tok")):
     """Create a an identifier to store the position of the fuzzy match.
 
     :param int art: Article number.
     :param int page: Page number.
@@ -44,20 +44,20 @@
     """
 
     def parse(self):
         self.page_data = {
             "id": self.id,
             "cdt": strftime("%Y-%m-%d %H:%M:%S"),
             "cc": True,
-            "iiif": os.path.join(IMPRESSO_IIIF_BASEURI, self.id),
+            "iiif_img_base_uri": os.path.join(IIIF_ENDPOINT_URI, self.id),
             "r": self.page_content["r"],
         }
 
         if not self.page_data["r"]:
-            logger.warning(f"Page {self.id} has no OCR text")
+            logger.warning("Page %s has no OCR text", self.id)
 
 
 class FedgazNewspaperIssue(TetmlNewspaperIssue):
     """Class representing a issue in FedGaz TETML format.
 
     All functions defined in this child class are used to parse additional
     information specific for FedGaz and extend the generic TETML importer.
@@ -73,58 +73,62 @@
     :param IssueDir issue_dir: Newspaper issue with relevant information.
 
     """
 
     def __init__(self, issue_dir: IssueDir):
         NewspaperIssue.__init__(self, issue_dir)
 
-        logger.info(f"Starting to parse {self.id}")
+        logger.info("Starting to parse %s", self.id)
 
         # get all tetml files of this issue
         self.files = self._index_issue_files()
 
         # parse metadata that contains additional article information
         self.df = self._parse_metadata()
 
         # parse the indexed files
         self.article_data = self.parse_articles()
 
         # recompose articles according to their logical boundaries
         self._heuristic_article_segmentation(candidates_only=True)
 
         # using canonical ('m') and additional non-canonical ('meta') metadata
-        self.content_items = [{"m": art["m"], "meta": art["meta"]} for art in self.article_data]
+        self.content_items = [
+            {"m": art["m"], "meta": art["meta"]} for art in self.article_data
+        ]
 
         # instantiate the individual pages
         self._find_pages()
 
         self.issue_data = {
             "id": self.id,
             "cdt": strftime("%Y-%m-%d %H:%M:%S"),
             "s": None,  # TODO: ignore style for the time being
             "i": self.content_items,
             "pp": [p.id for p in self.pages],
             "ar": self.rights,
         }
 
-        logger.info(f"Finished parsing {self.id}")
+        logger.info("Finished parsing %s", self.id)
 
     def parse_articles(self):
         """
         Parse all articles of this issue
         """
 
         articles = []
         current_issue_page = 1  # start page of next article
         for i, fname in enumerate(self.files):
             try:
                 data = tetml_parser(fname)
 
                 # canonical identifier
-                data["m"]["id"] = canonical_path(self.issuedir, name=f"i{i+1:04}", extension="")
+                data["m"]["id"] = canonical_path(
+                    self.issuedir, name=f"i{i+1:04}", extension=""
+                )
 
                 # reference to content item per region
                 for page in data["pages"]:
                     for reg in page["r"]:
                         reg["pOf"] = data["m"]["id"]
 
                 data["m"]["tp"] = "article"  # type attribute
@@ -135,15 +139,15 @@
                 current_issue_page = page_end
 
                 data = self._redefine_from_metadata(data)
 
                 articles.append(data)
 
             except Exception as e:
-                logger.error(f"Parsing of {fname} failed for {self.id}")
+                logger.error("Parsing of %s failed for %s", fname, self.id)
                 raise e
 
         return articles
 
     def _find_pages(self):
         """
         Initialize all page objects per issue assuming that a particular page
@@ -158,15 +162,17 @@
                     can_pages = can_pages[:-1]
             except KeyError:
                 pass
 
             for can_page, page_content in zip(can_pages, art["pages"]):
                 can_id = f"{self.id}-p{can_page:04}"
                 self.pages.append(
-                    TetmlNewspaperPage(can_id, can_page, page_content, art["meta"]["tetml_path"])
+                    TetmlNewspaperPage(
+                        can_id, can_page, page_content, art["meta"]["tetml_path"]
+                    )
                 )
 
     def _parse_metadata(self, fname="metadata.tsv"):
         """
         Parse file with additional metadata
         """
 
@@ -182,19 +188,20 @@
                 dtype={"article_docid": str},
                 index_col="article_docid",
             )
             # discard rows from other issues as they are irrelevant
             date = pd.Timestamp(self.date)
             df = df[df["issue_date"] == date]
 
-        except FileNotFoundError:
-            raise FileNotFoundError(
-                f"File with additional metadata needs to be placed in \
-            the top newspaper directory and named {fname}"
+        except FileNotFoundError as e:
+            msg = (
+                "File with additional metadata needs to be placed in "
+                f"the top newspaper directory and named {fname}"
             )
+            raise FileNotFoundError(msg) from e
 
         return df
 
     def _redefine_from_metadata(self, data):
         """
         Use additional metadata from file to set attributes
         """
@@ -285,57 +292,63 @@
             # mask potential parenthesis
             title = title.replace("(", r"\(").replace(")", r"\)")
 
             # max corrections as a function of length
             max_cost_total = max(2, int(0.2 * len(title)))
             max_insert = int(0.3 * len(title))
             # scaled by 3 to make insertions very cheap to account for bad OCR
-            fuzzy_cost = "{i<=" + str(max_insert) + ",1i+3d+3s<=" + str(max_cost_total * 3) + r"}"
+            fuzzy_cost = (
+                "{i<="
+                + str(max_insert)
+                + ",1i+3d+3s<="
+                + str(max_cost_total * 3)
+                + r"}"
+            )
             # fuzzy match article headline to locate (bestmatch flag)
             pattern = r"(?b)(" + title + r")" + fuzzy_cost
 
             try:
                 match = regex.search(pattern, text)
                 match_pos = match.start(1)
                 # remap the match position to the position in the initial parsing
                 match_tok_pos = text[:match_pos].count(" ")
 
                 error_msg = (
                     f"Positive fuzzy match (sanity check):\n"
-                    + f'\ttitle: {art["m"]["t"]}\n'
-                    + f"\tpattern: {pattern}\n"
-                    + f"\tmatch: {match}"
+                    f'\ttitle: {art["m"]["t"]}\n'
+                    f"\tpattern: {pattern}\n"
+                    f"\tmatch: {match}"
                 )
 
                 logger.info(error_msg)
 
                 # accumalate the boundaries
                 to_do_new_boundaries.append(tok_pos[match_tok_pos])
 
             except AttributeError:
                 error_msg = (
                     f"Error while searching for the logical boundary.\n"
-                    + f"The fuzzy match failed to match anything in the following article:\n"
-                    + f"{art['meta']}\n"
-                    + f"Pattern:\n{pattern}"
+                    f"The fuzzy match failed to match anything in the following article:\n"
+                    f"{art['meta']}\n"
+                    f"Pattern:\n{pattern}"
                 )
                 logger.error(error_msg)
 
                 # page needs to be removed in any case regardless of matching,
                 # otherwise the relation to the corresponding tif file is broken
                 del self.article_data[i_art - 1]["pages"][-1]
 
         # do the actual reassigning
         for bound in to_do_new_boundaries:
             try:
                 self._set_new_article_boundary(bound)
             except Exception as e:
                 error_msg = (
-                    f"Error while drawing a new article boundary at position {bound} in the issue {self.id}.\n"
-                    + f"Error: {e}"
+                    f"Error while drawing a new article boundary at position {bound} "
+                    f"in the issue {self.id}.\n Error: {e}"
                 )
                 logger.error(error_msg)
 
     def _set_new_article_boundary(self, bndry: TokPosition):
         """
         Set new article boundary and reassign the remainder from the subsequent
         to the previous article.
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/fedgaz/show_canonical_boxes.py` & `impresso_text_importer-1.1.0/text_importer/importers/fedgaz/show_canonical_boxes.py`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/generic_importer.py` & `impresso_text_importer-1.1.0/text_importer/importers/generic_importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 """
 Functions and CLI script to convert any OCR data into Impresso's format.
 
 Usage:
-    <importer-name>importer.py --input-dir=<id> (--clear | --incremental) [--output-dir=<od> --image-dirs=<imd> --temp-dir=<td> --chunk-size=<cs> --s3-bucket=<b> --config-file=<cf> --log-file=<f> --verbose --scheduler=<sch> --access-rights=<ar>]
+    <importer-name>importer.py --input-dir=<id> (--clear | --incremental) [--output-dir=<od> --image-dirs=<imd> --temp-dir=<td> --chunk-size=<cs> --s3-bucket=<b> --config-file=<cf> --log-file=<f> --verbose --scheduler=<sch> --access-rights=<ar> --git-repo=<gr> --num-workers=<nw>]
     <importer-name>importer.py --version
 
 Options:
     --input-dir=<id>    Base directory containing one sub-directory for each journal
     --image-dirs=<imd>  Directory containing (canonical) images and their metadata (use `,` to separate multiple dirs)
     --output-dir=<od>   Base directory where to write the output files
     --temp-dir=<td>     Temporary directory to extract .zip archives
     --config-file=<cf>  Configuration file for selective import
     --s3-bucket=<b>     If provided, writes output to an S3 drive, in the specified bucket
     --scheduler=<sch>  Tell dask to use an existing scheduler (otherwise it'll create one)
     --log-file=<f>      Log file; when missing print log to stdout
     --access-rights=<ar>  Access right file if relevant (only for `olive` and `rero` importers)
     --chunk-size=<cs>   Chunk size in years used to group issues when importing
+    --git-repo=<gr>   Local path to the "impresso-text-acquisition" git directory (including it).
+    --num-workers=<nw>  Number of workers to use for local dask cluster
     --verbose   Verbose log messages (good for debugging)
     --clear    Removes the output folder (if already existing)
     --incremental   Skips issues already present in output directory 
     --version    Prints version and exits.
 
 """  # noqa: E501
 
 import json
 import logging
 import os
 import shutil
 import time
 from typing import Any, Type, Callable
 
-from dask.distributed import Client, LocalCluster
+from dask.distributed import Client
 from docopt import docopt
-from impresso_commons.path.path_fs import (KNOWN_JOURNALS,
-                                           detect_canonical_issues,
-                                           IssueDir)
+import git
+from impresso_commons.path.path_fs import (
+    KNOWN_JOURNALS,
+    detect_canonical_issues,
+    IssueDir,
+)
+
+from impresso_commons.versioning.data_manifest import DataManifest
 
 from text_importer import __version__
+
 from text_importer.importers.classes import NewspaperIssue
 from text_importer.importers.bl.classes import BlNewspaperIssue
 from text_importer.importers.core import import_issues
 from text_importer.utils import init_logger
 
 __author__ = "Matteo Romanello"
 __email__ = "matteo.romanello@epfl.ch"
@@ -68,49 +76,51 @@
                 time.sleep(3)
                 os.makedirs(out_dir)
         else:
             os.makedirs(out_dir)
 
 
 def get_dask_client(
-    scheduler: str | None, log_file: str | None, log_level: int
+    scheduler: str | None, log_file: str | None, log_level: int, n_workers: int | None
 ) -> Client:
     """Instantiate Dask client with given scheduler address or default values.
 
-    If a scheduler is given, a Dask scheduler and workers should have been 
+    If a scheduler is given, a Dask scheduler and workers should have been
     previously launched in terminals separate to the one used for the importer.
     If no scheduler is given, the created Dask distributed cluster will have 8
     workers, each with 2 threads.
 
     Args:
         scheduler (str | None): TCP address of the Dask scheduler to use.
         log_file (str | None): File to use for logging.
         log_level (int): Log level used, either INFO or DEBUG in verbose mode.
+        n_workers (int | None): Number of workers to use in local cluster
 
     Returns:
         Client: A client connected to and allowing to manage the Dask cluster.
     """
     if scheduler is None:
-        #cluster = LocalCluster(n_workers=32, memory_limit='auto', threads_per_worker=2)
-        #client = Client(cluster)
-        client = Client(n_workers=16, threads_per_worker=2)
+        # cluster = LocalCluster(n_workers=32, memory_limit='auto', threads_per_worker=2)
+        # client = Client(cluster)
+        if n_workers is not None:
+            client = Client(n_workers=n_workers, threads_per_worker=2)
+        else:
+            client = Client(n_workers=24, threads_per_worker=2)
     else:
         client = Client(scheduler)
-        client.run(
-            init_logger, _logger=logger, log_level=log_level, log_file=log_file
-        )
+        client.run(init_logger, _logger=logger, log_level=log_level, log_file=log_file)
     return client
 
 
 def apply_detect_func(
-    issue_class: Type[NewspaperIssue], 
-    input_dir: str, 
-    access_rights: str, 
-    detect_func: Callable[[str, str], list[IssueDir]], 
-    tmp_dir: str
+    issue_class: Type[NewspaperIssue],
+    input_dir: str,
+    access_rights: str,
+    detect_func: Callable[[str, str], list[IssueDir]],
+    tmp_dir: str,
 ) -> list[IssueDir]:
     """Apply the given `detect_func` function of the importer in use.
 
     Args:
         issue_class (Type[NewspaperIssue]): Type of issue importer in use.
         input_dir (str): Directory containing this importer's newspaper data.
         access_rights (str): Path to the access rights file for this importer.
@@ -118,134 +128,167 @@
             the issues present in `input_dir` to import.
         tmp_dir (str): Temporary directory used to unpack zip archives.
 
     Returns:
         list[IssueDir]: List of detected issues for this importer.
     """
     if issue_class is BlNewspaperIssue:
-        return detect_func(
-            input_dir, access_rights=access_rights, tmp_dir=tmp_dir
-        )
+        return detect_func(input_dir, access_rights=access_rights, tmp_dir=tmp_dir)
     else:
         return detect_func(input_dir, access_rights=access_rights)
 
 
 def apply_select_func(
-    issue_class: Type[NewspaperIssue], 
-    config: dict[str, Any], 
-    input_dir: str, 
-    access_rights: str, 
+    issue_class: Type[NewspaperIssue],
+    config: dict[str, Any],
+    input_dir: str,
+    access_rights: str,
     select_func: Callable[[str, str, str], list[IssueDir]],
-    tmp_dir: str
+    tmp_dir: str,
 ) -> list[IssueDir]:
     """Apply the given `select_func` function of the importer in use.
 
     Args:
         issue_class (Type[NewspaperIssue]): Type of issue importer in use.
         config (dict[str, Any]): Configuration to filter issues to import.
         input_dir (str): Directory containing this importer's newspaper data.
         access_rights (str): Path to the access rights file for this importer.
-        select_func (Callable[[str, str, str], list[IssueDir]]): Function 
+        select_func (Callable[[str, str, str], list[IssueDir]]): Function
             detecting and selecting the issues to import using `config`.
         tmp_dir (str): Temporary directory used to unpack zip archives.
 
     Returns:
         list[IssueDir]: List of selected issues for this importer and config.
     """
     if issue_class is BlNewspaperIssue:
         return select_func(
             input_dir, config=config, access_rights=access_rights, tmp_dir=tmp_dir
         )
-    else:
-        return select_func(input_dir, config=config, access_rights=access_rights)
+
+    return select_func(input_dir, config=config, access_rights=access_rights)
 
 
 def main(
     issue_class: NewspaperIssue,
-    detect_func: Callable[[str, str], list[IssueDir]], 
-    select_func: Callable[[str, str, str], list[IssueDir]]
+    detect_func: Callable[[str, str], list[IssueDir]],
+    select_func: Callable[[str, str, str], list[IssueDir]],
 ) -> None:
     """Import and convert newspapers to Impresso's format using CLI parameters.
 
     All imported newspapers have the same OCR format. For each newspaper issue
     imported, corresponding Issue and Page objects will be created before being
     serialized to json and uploaded to an S3 bucket, grouped by title and year.
 
     Args:
         issue_class (NewspaperIssue): Importer to use for the conversion
         detect_func (Callable[[str, str], list[IssueDir]]): `detect` function
             of the used importer.
-        select_func (Callable[[str, str, str], list[IssueDir]]): `select` 
+        select_func (Callable[[str, str, str], list[IssueDir]]): `select`
             function of the used importer.
     """
-    
+
     # store CLI parameters
     args = docopt(__doc__)
     inp_dir = args["--input-dir"]
     outp_dir = args["--output-dir"]
-    temp_dir = args['--temp-dir']
+    temp_dir = args["--temp-dir"]
     image_dirs = args["--image-dirs"]
     out_bucket = args["--s3-bucket"]
     log_file = args["--log-file"]
-    access_rights_file = args['--access-rights']
-    chunk_size = args['--chunk-size']
+    access_rights_file = args["--access-rights"]
+    chunk_size = args["--chunk-size"]
     scheduler = args["--scheduler"]
     clear_output = args["--clear"]
     incremental_output = args["--incremental"]
     log_level = logging.DEBUG if args["--verbose"] else logging.INFO
     print_version = args["--version"]
     config_file = args["--config-file"]
-    
+    repo_path = args["--git-repo"]
+    num_workers = args["--num-workers"]
+
     if print_version:
-        print(f'impresso-txt-importer v{__version__}')
+        print(f"impresso-txt-importer v{__version__}")
         return
-    
+
     init_logger(logger, log_level, log_file)
-    logger.info("CLI arguments received: {}".format(args))
-    
+    logger.info("CLI arguments received: %s", args)
+
     # start the dask local cluster
-    client = get_dask_client(scheduler, log_file, log_level)
-    
-    logger.info(f"Dask cluster: {client}")
-    
+    client = get_dask_client(scheduler, log_file, log_level, int(num_workers))
+
+    logger.info("Dask cluster: %s", client)
+
     # Checks if out dir exists (Creates it if not) and if should empty it
-    clear_output_dir(outp_dir, clear_output)  
-    
+    clear_output_dir(outp_dir, clear_output)
+
     # detect/select issues
     if config_file and os.path.isfile(config_file):
-        logger.info(f"Found config file: {os.path.realpath(config_file)}")
-        with open(config_file, 'r') as f:
+        logger.info("Found config file: %s", os.path.realpath(config_file))
+        with open(config_file, "r", encoding="utf-8") as f:
             config = json.load(f)
-        issues = apply_select_func(issue_class, config, input_dir=inp_dir, 
-                                   access_rights=access_rights_file, 
-                                   select_func=select_func, tmp_dir=temp_dir)
+        issues = apply_select_func(
+            issue_class,
+            config,
+            input_dir=inp_dir,
+            access_rights=access_rights_file,
+            select_func=select_func,
+            tmp_dir=temp_dir,
+        )
         logger.info(
-            f"{len(issues)} newspaper remained after applying filter: {issues}"
+            "%s newspaper remained after applying filter: %s", len(issues), issues
         )
     else:
         logger.info("No config file found.")
-        issues = apply_detect_func(issue_class, inp_dir, access_rights_file, 
-                                   detect_func=detect_func, tmp_dir=temp_dir)
-        logger.info(f'{len(issues)} newspaper issues detected')
-    
+        issues = apply_detect_func(
+            issue_class,
+            inp_dir,
+            access_rights_file,
+            detect_func=detect_func,
+            tmp_dir=temp_dir,
+        )
+        logger.info("%s newspaper issues detected", len(issues))
+
     if outp_dir is not None and os.path.exists(outp_dir) and incremental_output:
         issues_to_skip = [
             (issue.journal, issue.date, issue.edition)
             for issue in detect_canonical_issues(outp_dir, KNOWN_JOURNALS)
         ]
-        logger.debug(f"Issues to skip: {issues_to_skip}")
-        logger.info(f"{len(issues_to_skip)} issues to skip")
+        logger.debug("Issues to skip: %s", issues_to_skip)
+        logger.info("%s issues to skip", len(issues_to_skip))
         issues = list(
             filter(
-                lambda x: (x.journal, x.date, x.edition) not in issues_to_skip,
-                issues
+                lambda x: (x.journal, x.date, x.edition) not in issues_to_skip, issues
             )
         )
-        logger.debug(f"Remaining issues: {issues}")
-        logger.info(f"{len(issues)} remaining issues")
-    
-    logger.debug("Following issues will be imported:{}".format(issues))
-    
+        logger.debug("Remaining issues: %s", issues)
+        logger.info("%s remaining issues", len(issues))
+
+    logger.debug("Following issues will be imported: %s", issues)
+
     assert outp_dir is not None or out_bucket is not None
-    
-    import_issues(issues, outp_dir, out_bucket, issue_class, 
-                  image_dirs, temp_dir, chunk_size, client)
+
+    # ititialize manifest
+    if config_file:
+        newspapers = f" for titles {list(config['newspapers'].keys())}"
+    else:
+        newspapers = ""
+    manifest_note = f"Ingestion of {len(issues)} Newspaper issues into canonical format{newspapers}."
+
+    manifest = DataManifest(
+        data_stage="canonical",
+        s3_output_bucket=out_bucket,
+        git_repo=git.Repo(repo_path),
+        temp_dir=temp_dir,
+        notes=manifest_note,
+    )
+
+    import_issues(
+        issues,
+        outp_dir,
+        out_bucket,
+        issue_class,
+        image_dirs,
+        temp_dir,
+        chunk_size,
+        manifest,
+        client,
+    )
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/lux/classes.py` & `impresso_text_importer-1.1.0/text_importer/importers/rero/classes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,629 +1,524 @@
-"""This module contains the definition of the Luxembourg importer classes.
+"""This module contains the definition of the RERO importer classes.
 
 The classes define newspaper Issues and Pages objects which convert OCR data in
-the BNL (Blibliotheque Nationale du Luxembourg) version of the Mets/Alto format
-to a unified canoncial format.
+the RERO version of the Mets/Alto format to a unified canoncial format.
 Theses classes are subclasses of generic Mets/Alto importer classes.
 """
 
 import logging
 import os
-import re
 from time import strftime
 from typing import Any
 
 from bs4 import BeautifulSoup
 from bs4.element import NavigableString, Tag
 
-from text_importer.importers import (CONTENTITEM_TYPE_ADVERTISEMENT,
-                                     CONTENTITEM_TYPE_ARTICLE,
-                                     CONTENTITEM_TYPE_IMAGE,
-                                     CONTENTITEM_TYPE_OBITUARY,
-                                     CONTENTITEM_TYPE_TABLE,
-                                     CONTENTITEM_TYPE_WEATHER)
-from text_importer.importers.lux.helpers import (convert_coordinates, 
-                                                 encode_ark, 
-                                                 section_is_article, 
-                                                 div_has_body,
-                                                 find_section_articles, 
-                                                 remove_section_cis)
-from text_importer.importers.mets_alto.alto import parse_style
-from text_importer.importers.mets_alto import (MetsAltoNewspaperIssue,
-                                               MetsAltoNewspaperPage,
-                                               parse_mets_amdsec)
-from text_importer.utils import get_issue_schema, get_page_schema
+from text_importer.importers import CONTENTITEM_TYPE_IMAGE, CONTENTITEM_TYPES
+from text_importer.importers.mets_alto import (
+    MetsAltoNewspaperIssue,
+    MetsAltoNewspaperPage,
+    parse_mets_amdsec,
+)
+from text_importer.utils import get_issue_schema, get_page_schema, get_reading_order
 
 IssueSchema = get_issue_schema()
 Pageschema = get_page_schema()
 
 logger = logging.getLogger(__name__)
-IIIF_ENDPOINT_URL = "https://iiif.eluxemburgensia.lu/iiif/2"
 
+IIIF_ENDPOINT_URI = "https://impresso-project.ch/api/proxy/iiif/"
+IIIF_SUFFIX = "info.json"
+IIIF_IMAGE_SUFFIX = "full/full/0/default.jpg"
+
+# Types used in RERO2/RERO3 that are not in impresso schema
+SECTION_TYPE = "section"
+PICTURE_TYPE = "picture"
+ILLUSTRATION_TYPE = "illustration"
+
+
+def convert_coordinates(
+    coords: list[float], resolution: dict[str, float], page_width: float
+) -> list[int]:
+    """Convert the coordinates using true and coordinate system resolutions.
+
+    The coordinate system resolution is not necessarily the same as the true
+    resolution of the image. A conversion, or rescaling can thus be necessary.
+    Essentially computes fact = coordinate_width / true_width,
+    and converts using x/fact.
+
+    Args:
+        coords (list[float]): List of coordinates to convert
+        resolution (dict[str, float]): True resolution of the images (keys
+            `x_resolution` and `y_resolution` of the dict).
+        page_width (float): The page width used for the coordinate system.
+
+    Returns:
+        list[int]: The coordinates rescaled to match the true image resolution.
+    """
+    if resolution["x_resolution"] == 0 or resolution["y_resolution"] == 0:
+        return coords
+    factor = page_width / resolution["x_resolution"]
+    return [int(c / factor) for c in coords]
 
-class LuxNewspaperPage(MetsAltoNewspaperPage):
-    """Newspaper page in BNL (Mets/Alto) format.
+
+class ReroNewspaperPage(MetsAltoNewspaperPage):
+    """Newspaper page in RERO (Mets/Alto) format.
 
     Args:
         _id (str): Canonical page ID.
         number (int): Page number.
         filename (str): Name of the Alto XML page file.
         basedir (str): Base directory where Alto files are located.
-        encoding (str, optional): Encoding of XML file. Defaults to 'utf-8'.
-    
+
     Attributes:
         id (str): Canonical Page ID (e.g. ``GDL-1900-01-02-a-p0004``).
         number (int): Page number.
         page_data (dict[str, Any]): Page data according to canonical format.
         issue (NewspaperIssue): Issue this page is from.
         filename (str): Name of the Alto XML page file.
         basedir (str): Base directory where Alto files are located.
-        encoding (str, optional): Encoding of XML file.
+        encoding (str, optional): Encoding of XML file. Defaults to 'utf-8'.
+        page_width (float): The page width used for the coordinate system.
     """
-    
-    def _parse_font_styles(self) -> None:
-        """Parse section `<TextStyle>` of the XML file to extract the fonts.
-        """
-        style_divs = self.xml.findAll("TextStyle")
-        
-        styles = []
-        for d in style_divs:
-            styles.append(parse_style(d))
-        
-        self.page_data['s'] = styles
-    
+
+    def __init__(self, _id: str, number: int, filename: str, basedir: str) -> None:
+        super().__init__(_id, number, filename, basedir)
+
+        page_tag = self.xml.find("Page")
+        self.page_width = float(page_tag.get("WIDTH"))
+
     def add_issue(self, issue: MetsAltoNewspaperIssue) -> None:
         self.issue = issue
-        encoded_ark_id = encode_ark(self.issue.ark_id)
-        iiif_base_link = f'{IIIF_ENDPOINT_URL}/{encoded_ark_id}'
-        iiif_link = f'{iiif_base_link}%2fpages%2f{self.number}/info.json'
-        self.page_data['iiif'] = iiif_link
-        self._parse_font_styles()
-    
-    def _convert_coordinates(
-        self, page_regions: list[dict]
-    ) -> tuple[bool, list[dict]]:
+        self.page_data["iiif_img_base_uri"] = os.path.join(IIIF_ENDPOINT_URI, self.id)
+
+    # no coordinate conversion needed, but keeping it here for now
+    def _convert_coordinates(self, page_regions: list[dict]) -> tuple[bool, list[dict]]:
+        """Convert region coordinates to iiif format if possible.
+
+        Note:
+            Currently, no conversion of coordinates is needed.
+
+        Args:
+            page_regions (list[dict[str, Any]]): Page regions from canonical
+                page format.
+
+        Returns:
+            tuple[bool, list[dict[str, Any]]]: Whether the region coordinates
+                are in iiif format and page regions.
+        """
+        if self.issue is None:
+            logger.critical("Cannot convert coordinates if issue is unknown")
+
+        # Get page real resolution
+        image_properties = self.issue.image_properties[self.number]
+        x_res = image_properties["x_resolution"]
+        y_res = image_properties["y_resolution"]
+
+        # Those fields are 0 For RERO2
+        if x_res == 0 or y_res == 0:
+            return True, page_regions
+
+        # Then convert coordinates of all regions/paragraphs/lines/tokens
         success = False
         try:
-            img_props = self.issue.image_properties[self.number]
-            x_res = img_props['x_resolution']
-            y_res = img_props['y_resolution']
-            
             for region in page_regions:
-                
-                x, y, w, h = region['c']
-                region['c'] = convert_coordinates(x, y, w, h, 
-                                                  x_res, y_res)
-                
-                logger.debug(f"Page {self.number}: "
-                             f"{x},{y},{w},{h} => {region['c']}")
-                
-                for paragraph in region['p']:
-                    
-                    x, y, w, h = paragraph['c']
-                    paragraph['c'] = convert_coordinates(x, y, w, h, 
-                                                         x_res, y_res)
-                    
-                    logger.debug(f"(para) Page {self.number}: "
-                                 f"{x},{y},{w},{h} => {paragraph['c']}")
-                    
-                    for line in paragraph['l']:
-                        
-                        x, y, w, h = line['c']
-                        line['c'] = convert_coordinates(x, y, w, h, 
-                                                        x_res, y_res)
-                        
-                        logger.debug(f"(line) Page {self.number}: "
-                                     f"{x},{y},{w},{h} => {paragraph['c']}")
-                        
-                        for token in line['t']:
-                            x, y, w, h = token['c']
-                            token['c'] = convert_coordinates(x, y, w, h, 
-                                                             x_res, y_res)
-                            logger.debug(f"(token) Page {self.number}: "
-                                         f"{x},{y},{w},{h} => {token['c']}")
+                region["c"] = convert_coordinates(
+                    region["c"], image_properties, self.page_width
+                )
+                for paragraph in region["p"]:
+                    paragraph["c"] = convert_coordinates(
+                        paragraph["c"], image_properties, self.page_width
+                    )
+                    for line in paragraph["l"]:
+                        line["c"] = convert_coordinates(
+                            line["c"], image_properties, self.page_width
+                        )
+                        for token in line["t"]:
+                            token["c"] = convert_coordinates(
+                                token["c"], image_properties, self.page_width
+                            )
             success = True
         except Exception as e:
-            logger.error(f"Error {e} occurred when converting coordinates "
-                         f"for {self.id}")
-        finally:
-            return success, page_regions
+            logger.error(
+                "Error %s occurred when converting coordinates for %s", e, self.id
+            )
+        return success, page_regions
 
 
-class LuxNewspaperIssue(MetsAltoNewspaperIssue):
-    """Class representing an issue in BNL data.
+class ReroNewspaperIssue(MetsAltoNewspaperIssue):
+    """Newspaper Issue in RERO (Mets/Alto) format.
 
-    All functions defined in this child class are specific to parsing BNL 
-    (Luxembourg National Library) Mets/Alto format.
+    All functions defined in this child class are specific to parsing RERO
+    Mets/Alto format.
 
     Args:
         issue_dir (IssueDir): Identifying information about the issue.
 
     Attributes:
         id (str): Canonical Issue ID (e.g. ``GDL-1900-01-02-a``).
         edition (str): Lower case letter ordering issues of the same day.
         journal (str): Newspaper unique identifier or name.
         path (str): Path to directory containing the issue's OCR data.
         date (datetime.date): Publication date of issue.
-        issue_data (dict): Issue data according to canonical Issue format.
-        pages (list): List of :obj:`NewspaperPage` instances from this issue.
+        issue_data (dict[str, Any]): Issue data according to canonical format.
+        pages (list): list of :obj:`NewspaperPage` instances from this issue.
         rights (str): Access rights applicable to this issue.
-        image_properties (dict): metadata allowing to convert region OCR/OLR
-            coordinates to iiif format compliant ones.
+        image_properties (dict[str, Any]): metadata allowing to convert region
+            OCR/OLR coordinates to iiif format compliant ones.
         ark_id (int): Issue ARK identifier, for the issue's pages' iiif links.
     """
-    
+
     def _find_pages(self) -> None:
         """Detect and create the issue pages using the relevant Alto XML files.
 
-        Created :obj:`LuxoNewspaperPage` instances are added to :attr:`pages`.
+        Created :obj:`ReroNewspaperPage` instances are added to :attr:`pages`.
 
         Raises:
             e: Instantiation of a page or adding it to :attr:`pages` failed.
         """
-        # get the canonical names for pages in the newspaper issue by
-        # visiting the `text` sub-folder with the alto XML files
-        text_path = os.path.join(self.path, 'text')
-        page_file_names = [
-            file
-            for file in os.listdir(text_path)
-            if not file.startswith('.') and '.xml' in file
-            ]
-        
+        alto_path = os.path.join(self.path, "ALTO")
+
+        page_file_names = self._find_alto_files_or_retry(alto_path)
+
         page_numbers = []
-        page_match_exp = r'(.*?)(\d{5})(.*)'
-        
+
         for fname in page_file_names:
-            g = re.match(page_match_exp, fname)
-            page_no = g.group(2)
+            page_no = fname.split(".")[0]
             page_numbers.append(int(page_no))
-        
+
         page_canonical_names = [
-            "{}-p{}".format(self.id, str(page_n).zfill(4)) 
-            for page_n in page_numbers
+            "{}-p{}".format(self.id, str(page_n).zfill(4)) for page_n in page_numbers
         ]
-        
+
         self.pages = []
-        for filename, page_no, page_id in zip(page_file_names, page_numbers, 
-                                              page_canonical_names):
+        for filename, page_no, page_id in zip(
+            page_file_names, page_numbers, page_canonical_names
+        ):
             try:
                 self.pages.append(
-                    LuxNewspaperPage(page_id, page_no, filename, text_path)
+                    ReroNewspaperPage(page_id, page_no, filename, alto_path)
                 )
             except Exception as e:
-                logger.error(
-                        f'Adding page {page_no} {page_id} {filename}',
-                        f'raised following exception: {e}'
-                        )
+                msg = (
+                    f"Adding page {page_no} {page_id} {filename}",
+                    f"raised following exception: {e}",
+                )
+                logger.error(msg)
                 raise e
-    
-    def _parse_mets_div(self, div: Tag) -> list[dict[str, str | int]]:
+
+    def _find_alto_files_or_retry(self, alto_path: str) -> list[str]:
+        """List XML files present in given page file dir, retry up to 3 times.
+
+        During the processing, some IO errors can randomly happen when listing
+        the contents of the ALTO directory, preventing the correct parsing of
+        the issue. The error is raised after the third try.
+        If the Alto directory does not exist, only try once.
+
+        Args:
+            alto_path (str): Path to the directory with the Alto XML files.
+
+        Raises:
+            e: Given directory does not exist, or listing its contents failed
+                three times in a row.
+
+        Returns:
+            list[str]: List of paths of the pages' Alto XML files.
+        """
+        if not os.path.exists(alto_path):
+            logger.critical("Could not find pages for %s", self.id)
+            tries = 1
+
+        tries = 3
+        for i in range(tries):
+            try:
+                page_file_names = [
+                    file
+                    for file in os.listdir(alto_path)
+                    if not file.startswith(".") and ".xml" in file
+                ]
+                return page_file_names
+            except IOError as e:
+                if i < tries - 1:  # i is zero indexed
+                    msg = (
+                        f"Caught error for {self.id}, retrying (up to {tries} times) "
+                        f"to find pages. Error: {e}."
+                    )
+                    logger.warning(msg)
+                    continue
+                else:
+                    logger.warning("Reached maximum amount of errors for %s.", self.id)
+                    raise e
+
+    def _parse_content_parts(self, div: Tag) -> list[dict[str, str | int]]:
         """Parse the children of a content item div for its legacy `parts`.
 
         The `parts` are article-level metadata about the content item from the
         ORC and OLR processes. This information is located in an `<area>` tag.
 
         Args:
             div (Tag): The div containing the content item
 
         Returns:
             list[dict[str, str | int]]: information on different parts for the
                 content item (role, id, fileid, page)
         """
         parts = []
-        
         for child in div.children:
+
             if isinstance(child, NavigableString):
                 continue
             elif isinstance(child, Tag):
-                type_attr = child.get('TYPE')
+                type_attr = child.get("TYPE")
                 comp_role = type_attr.lower() if type_attr else None
-                areas = child.findAll('area')
+                areas = child.findAll("area")
                 for area in areas:
-                    comp_id = area.get('BEGIN')
-                    comp_fileid = area.get('FILEID')
-                    comp_page_no = int(comp_fileid.replace('ALTO', ''))
-                    
+                    comp_id = area.get("BEGIN")
+                    comp_fileid = area.get("FILEID")
+                    comp_page_no = int(comp_fileid.replace("ALTO", ""))
+
                     parts.append(
-                            {
-                                'comp_role': comp_role,
-                                'comp_id': comp_id,
-                                'comp_fileid': comp_fileid,
-                                'comp_page_no': comp_page_no
-                                }
-                            )
+                        {
+                            "comp_role": comp_role,
+                            "comp_id": comp_id,
+                            "comp_fileid": comp_fileid,
+                            "comp_page_no": comp_page_no,
+                        }
+                    )
         return parts
-    
-    def _parse_dmdsec(
-        self, mets_doc: BeautifulSoup
-    ) -> tuple[list[dict[str, Any]], int]:
-        """Parse `<dmdSec>` tags of Mets file to find some content items.
-        
-        Only articles and pictures are in this section and are identified
-        here. Those tags' `ID` attribute should contain `ARTICLE` or `PICT`.
 
-        The numbering of the content items (used for the canonical IDs) is
-        generated based on the sorting of the ID strings of the sections.
+    def _get_ci_language(self, dmdid: str, mets_doc: BeautifulSoup) -> str | None:
+        """Find the language code of the content item with given a `DMDID`.
+
+        Languages are usually in a `<dmdSec>` at the beginning of a METS file,
+        corresponding to the descriptive metadata.
 
         Args:
+            dmdid (str): Descriptive metadata id of a content item.
             mets_doc (BeautifulSoup): Contents of Mets XML file.
 
         Returns:
-            tuple[list[dict[str, Any]], int]: Parsed CI's and counter to keep
-                track of the item numbers.
+            str | None: Language if defined in the file else `None`.
         """
-        content_items = []
-        sections = mets_doc.findAll('dmdSec')
-        
-        # sort based on the ID string to pinpoint the generated canonical IDs
-        sections = sorted(
-            sections,
-            key=lambda elem: elem.get('ID').split("_")[1]
-        )
-        counter = 1
-        for section in sections:
-            section_id = section.get('ID')
-            
-            if "ARTICLE" in section_id or "PICT" in section_id:
-                # Get title Info
-                title_elements = section.find_all('titleInfo')
-                item_title = (
-                    title_elements[0].getText().replace('\n', ' ').strip() 
-                    if len(title_elements) > 0 else None
-                )
-                #TODO: case when len(title_elements)>1 ?
-                
-                # Prepare ci metadata
-                metadata = {
-                    'id': "{}-i{}".format(self.id, str(counter).zfill(4)),
-                    'pp': [],
-                    'tp': (
-                        CONTENTITEM_TYPE_ARTICLE 
-                        if "ARTICLE" in section_id 
-                        else CONTENTITEM_TYPE_IMAGE
-                    )
-                }
-                
-                # Find the parts
-                try:
-                    item_div = mets_doc.findAll('div', {'DMDID':section_id})[0]
-                    parts = self._parse_mets_div(item_div)
-                except IndexError:
-                    err_msg = f"<div DMID={section_id}> not found {self.path}"
-                    self._notes.append(err_msg)
-                    logger.error(err_msg)
-                    parts = []
-                    item_div = None
-                
-                if item_title:
-                    metadata['t'] = item_title
-                
-                # Finalize the item
-                item = {
-                    "m": metadata,
-                    "l": {
-                        "id": section_id,
-                        "parts": parts
-                        }
-                    }
-                
-                # TODO: keep language (there may be more than one)
-                # TODO: how to get language information for these CIs ?
-                if item['m']['tp'] == CONTENTITEM_TYPE_ARTICLE:
-                    lang = section.find_all('languageTerm')[0].getText()
-                    item['m']['l'] = lang
-                
-                # This has been added to not consider ads as pictures
-                if (not ((item_div is not None) and ("PICT" in section_id) and
-                         (item_div.get("TYPE") == "ADVERTISEMENT"))):
-                    content_items.append(item)
-                counter += 1
-        
-        return content_items, counter
-    
-    def _parse_structmap_divs(
-        self, start_counter: int, mets_doc: BeautifulSoup
-    ) -> tuple[list[dict[str, Any]], int]:
-        """Parse content items only in the Logical `<structMap>` of Mets file.
+        lang = mets_doc.find("dmdSec", {"ID": dmdid})
+        if lang is None:
+            return None
+        lang = lang.find("MODS:languageTerm")
+        if lang is None:
+            return None
+        return lang.text
+
+    def _parse_content_item(
+        self, item_div: Tag, counter: int, mets_doc: BeautifulSoup
+    ) -> dict[str, Any]:
+        """Parse a content item div and create the dictionary representing it.
+
+        The dictionary corresponding to a content item needs to be of a precise
+        format, following the canonical Issue schema.
+        The counter is used to generate the canonical ID for the content item.
 
         Args:
-            start_counter (int): item number to start with for the CIs found
+            item_div (Tag): Div of content item.
+            counter (int): Number of content items already added to the issue.
             mets_doc (BeautifulSoup): Contents of Mets XML file.
 
         Returns:
-            tuple[list[dict[str, Any]], int]: Parsed CI's and updated counter
-                to keep track of the item numbers.
+            dict[str, Any]: Content item in canonical format.
         """
-        content_items = []
-        counter = start_counter
-        element = mets_doc.find('structMap', {'TYPE': 'LOGICAL'})
-        
-        allowed_types = ["ADVERTISEMENT", "DEATH_NOTICE", "WEATHER"]
-        divs = []
-        
-        for div_type in allowed_types:
-            divs += element.findAll('div', {'TYPE': div_type})
-        
-        sorted_divs = sorted(
-            divs, key=lambda elem: elem.get('ID')
-        )
-        
-        for div in sorted_divs:
-            
-            div_type = div.get('TYPE').lower()
-            if div_type == 'advertisement':
-                content_item_type = CONTENTITEM_TYPE_ADVERTISEMENT
-            elif div_type == 'weather':
-                content_item_type = CONTENTITEM_TYPE_WEATHER
-            elif div_type == 'death_notice':
-                content_item_type = CONTENTITEM_TYPE_OBITUARY
-            else:
-                continue
-            
-            # TODO: how to get language information for these CIs ?
-            # The language of those CI should be in
-            # the DMDSEC of their parent section.
-            metadata = {
-                'id': "{}-i{}".format(self.id, str(counter).zfill(4)),
-                'tp': content_item_type,
-                'pp': [],
-                't': div.get('LABEL')
-            }
-            
-            item = {
-                "m": metadata,
-                "l": {
-                    "parts": self._parse_mets_div(div),  # Parse the parts
-                    "id": div.get('ID')
-                }
-            }
-            content_items.append(item)
-            counter += 1
-        return content_items, counter
-    
-    def _process_image_ci(
-        self, ci: dict[str, Any], mets_doc: BeautifulSoup
-    ) -> None:
-        """Process an image content item to complete its information.
+        div_type = item_div.get("TYPE").lower()
 
-        Args:
-            ci (dict[str, Any]): Image content item to be processed.
-            mets_doc (BeautifulSoup): Contents of Mets XML file.
-        """
-        item_div = mets_doc.findAll('div', {'DMDID': ci['l']['id']})
-        if len(item_div) > 0:
-            item_div = item_div[0]
-        else:
-            return
-        legacy_id = item_div.get('ID')
-        # Image is actually table
-        
-        if item_div.get('TYPE').lower() == "table":
-            ci['m']['tp'] = CONTENTITEM_TYPE_TABLE
-            for part in ci['l']['parts']:
-                page_no = part["comp_page_no"]
-                if page_no not in ci['m']['pp']:
-                    ci['m']['pp'].append(page_no)
-        
-        elif item_div.get('TYPE').lower() == "illustration":
-            
-            # filter content item part that is the actual image
-            # the other part is the caption
-            try:
-                part = [
-                    part
-                    for part in ci['l']['parts']
-                    if part['comp_role'] == 'image'
-                ][0]
-            except IndexError as e:
-                err_msg = f'{legacy_id} without image subpart'
-                err_msg += f"; {legacy_id} has {ci['l']['parts']}"
-                logger.error(err_msg)
-                self._notes.append(err_msg)
-                logger.exception(e)
-                return
-            
-            # for each "part" open the XML file of corresponding page
-            # get the coordinates and convert them
-            # some imgs are in fact tables (meaning they have text
-            # recognized)
-            
-            # find the corresponding page where it's located
-            curr_page = None
-            for page in self.pages:
-                if page.number == part['comp_page_no']:
-                    curr_page = page
-            
-            # add the page number to the content item
-            assert curr_page is not None
-            if curr_page.number not in ci['m']['pp']:
-                ci['m']['pp'].append(curr_page.number)
-            
-            try:
-                # parse the Alto file to fetch the coordinates
-                page_xml = curr_page.xml
-                
-                composed_block = page_xml.find('ComposedBlock', 
-                                                    {"ID": part['comp_id']})
-                
-                if composed_block:
-                    graphic_el = composed_block.find('GraphicalElement')
-                    
-                    if graphic_el is None:
-                        graphic_el = page_xml.find('Illustration')
-                else:
-                    graphic_el = page_xml.find('Illustration', 
-                                                    {"ID": part['comp_id']})
+        if div_type == PICTURE_TYPE or div_type == ILLUSTRATION_TYPE:
+            div_type = CONTENTITEM_TYPE_IMAGE
 
-                hpos = int(graphic_el.get('HPOS'))
-                vpos = int(graphic_el.get('VPOS'))
-                width = int(graphic_el.get('WIDTH'))
-                height = int(graphic_el.get('HEIGHT'))
-                img_props = self.image_properties[curr_page.number]
-                x_resolution = img_props['x_resolution']
-                y_resolution = img_props['y_resolution']
-                coordinates = convert_coordinates(hpos, vpos, height, width, 
-                                                  x_resolution, y_resolution)
-                encoded_ark_id = encode_ark(self.ark_id)
-                iiif_base_link = f'{IIIF_ENDPOINT_URL}/{encoded_ark_id}'
-                ci['m']['iiif_link'] = (
-                    f'{iiif_base_link}%2fpages%2f{curr_page.number}/info.json'
-                )
-                ci['c'] = list(coordinates)
-                del ci['l']['parts']
-            except Exception as e:
-                err_msg = 'An error occurred with {}'.format(
-                        os.path.join(
-                                curr_page.basedir,
-                                curr_page.filename
-                                )
-                        )
-                err_msg += f"<ComposedBlock> @ID {part['comp_id']} not found"
-                logger.error(err_msg)
-                self._notes.append(err_msg)
-                logger.exception(e)
-    
-    def _parse_section(
-        self, 
-        section: Tag, 
-        section_div: Tag, 
-        content_items: list[dict[str, Any]], 
-        counter: int
-    ) -> dict[str, Any]:
-        """Reconstruct the section using the div and previously created CIs.
-        
-        In the `l` field of the ci, an additional field `canonical_parts` 
-        points to articles that were added to this section. 
-        (Bugfix done by Edoardo)
+        # Check if new content item is found (or if we need more translation)
+        if div_type not in CONTENTITEM_TYPES:
+            logger.warning("Found new content item type: %s", div_type)
+
+        metadata = {
+            "id": "{}-i{}".format(self.id, str(counter).zfill(4)),
+            "tp": div_type,
+            "pp": [],
+            "t": item_div.get("LABEL"),
+        }
+
+        # Get CI language
+        language = self._get_ci_language(item_div.get("DMDID"), mets_doc)
+        if language is not None:
+            metadata["l"] = language
+
+        content_item = {
+            "m": metadata,
+            "l": {
+                "id": item_div.get("ID"),
+                "parts": self._parse_content_parts(item_div),
+            },
+        }
+        for p in content_item["l"]["parts"]:
+            pge_no = p["comp_page_no"]
+            if pge_no not in content_item["m"]["pp"]:
+                content_item["m"]["pp"].append(pge_no)
+
+        if content_item["m"]["tp"] == CONTENTITEM_TYPE_IMAGE:
+            (content_item["c"], content_item["m"]["iiif_link"]) = self._get_image_info(
+                content_item
+            )
+        return content_item
+
+    def _decompose_section(self, div: Tag) -> list[Tag]:
+        """Recursively decompose `Section` tags into a flat list of div tags.
+
+        In RERO3, sometimes textblocks and images are withing `Section` tags.
+        Those need to be recursively decomposed for all the content items to
+        be parsed.
 
         Args:
-            section (Tag): `<dmdSec>` section of the Mets XML file.
-            section_div (Tag): `<div>` section with corresponding DMDID.
-            content_items (list[dict[str, Any]]): Incomplete content items.
-            counter (int): Content item counter.
+            div (Tag): Tag of type `Section` containing other divs to extract.
 
         Returns:
-            dict[str, Any]: Content item of the reconstructed section.
+            list[Tag]: Flat list of div tags to parse.
         """
-        title_elements = section.find_all('titleInfo')
-        
-        item_title = title_elements[0].getText().replace('\n', ' ') \
-            .strip() if len(title_elements) > 0 else None
-        
-        metadata = {
-            'id': "{}-i{}".format(self.id, str(counter).zfill(4)),
-            'pp': [],
-            'tp': CONTENTITEM_TYPE_ARTICLE
-            }
-        if item_title:
-            metadata['t'] = item_title
-        
-        parts = self._parse_mets_div(section_div)
-        
-        old_cis = find_section_articles(section_div, content_items)
-        item = {
-            "m": metadata,
-            "l": {
-                "id": section_div.get('DMDID'),
-                "parts": parts,
-                "canonical_parts": old_cis
-                }
-            }
-        return item
-    
-    def _parse_sections(
-        self, 
-        content_items: list[dict[str, Any]], 
-        start_counter: int, 
-        mets_doc: BeautifulSoup
-    ) -> list[dict[str, Any]]:
-        """Reconstruct all the sections from the METS file (bugfix by Edoardo).
+        logger.info("Decomposing section type")
+        # Only consider those with DMDID
+        section_divs = [d for d in div.findAll("div") if d.get("DMDID") is not None]
+        # Sort to get same IDS
+        section_divs = sorted(section_divs, key=lambda x: x.get("ID").lower())
+
+        final_divs = []
+        # Now do it recursively
+        for d in section_divs:
+            d_type = d.get("TYPE")
+            if d_type is not None:
+                if d_type.lower() == SECTION_TYPE:
+                    # Recursively decompose if contents are also of Sections.
+                    final_divs += self._decompose_section(d)
+                else:
+                    final_divs.append(d)
+        return final_divs
+
+    def _parse_content_items(self, mets_doc: BeautifulSoup) -> list[dict[str, Any]]:
+        """Extract content item elements from the issue's Mets XML file.
 
         Args:
-            content_items (list[dict[str, Any]]): Current content items.
-            start_counter (int):  Content item counter.
-            mets_doc (BeautifulSoup): Contents of Mets XML file.
+            mets_doc (BeautifulSoup): Mets document as BeautifulSoup object.
 
         Returns:
-            list[dict[str, Any]]: Updated content items
+            list[dict[str, Any]]: Issue's content items in canonical format.
         """
-        counter = start_counter
-        sections = mets_doc.findAll('dmdSec')
-        
-        sections = sorted(
-                sections,
-                key=lambda elem: elem.get('ID').split("_")[1]
-                )
-        # First look for sections and get their ID
-        new_sections = []
-        for section in sections:
-            section_id = section.get('ID')
-            if 'SECT' in section_id:
-                div = mets_doc.find('div', {"DMDID": section_id})  # Get div
-                if div is None:
-                    err_msg = f"<div [DMID]={section_id}> not found {self.path}"
-                    self._notes.append(err_msg)
-                    logger.error(err_msg)
-                    continue
-                if div_has_body(div) and section_is_article(div):
-                    new_section = self._parse_section(section, div, 
-                                                      content_items, counter)
-                    new_sections.append(new_section)
+        content_items = []
+        divs = mets_doc.find("div", {"TYPE": "CONTENT"}).findChildren(
+            "div", recursive=False
+        )  # Children of "Content" tag
+
+        # Sort to have same naming
+        sorted_divs = sorted(divs, key=lambda x: x.get("ID").lower())
+
+        counter = 1
+        for div in sorted_divs:
+            # Parse Each contentitem
+            div_type = div.get("TYPE")
+            # To parse divs of type SECTION, need to get sub types with DMDID
+            if div_type is not None and (div_type.lower() == SECTION_TYPE):
+                section_divs = self._decompose_section(div)
+                for d in section_divs:
+                    content_items.append(self._parse_content_item(d, counter, mets_doc))
                     counter += 1
-        return new_sections
-    
+            else:
+                content_items.append(self._parse_content_item(div, counter, mets_doc))
+                counter += 1
+
+        # add the reading order to the items metadata
+        reading_order_dict = get_reading_order(content_items)
+        for item in content_items:
+            item["m"]["ro"] = reading_order_dict[item["m"]["id"]]
+
+        return content_items
+
     def _parse_mets(self) -> None:
         """Parse the Mets XML file corresponding to this issue.
 
-        Once the :attr:`issue_data` is created, containing all the relevant 
-        information in the canonical Issue format, the `LuxNewspaperIssue`
+        Once the :attr:`issue_data` is created, containing all the relevant
+        information in the canonical Issue format, the `ReroNewspaperIssue`
         instance is ready for serialization.
-
-        TODO: correct parsing to prevent need of reconstruction (if possible).
         """
         mets_doc = self.xml
-        
-        # explain
+
         self.image_properties = parse_mets_amdsec(
-            mets_doc, x_res='xOpticalResolution', y_res='yOpticalResolution'
-        )
-        
-        # First find `ARTICLE` and `PICTURE` content items
-        content_items, counter = self._parse_dmdsec(mets_doc)
-        # Then find other content items
-        new_cis, counter = self._parse_structmap_divs(counter, mets_doc)
-        content_items += new_cis
-        
-        # Reconstruct sections
-        section_cis = self._parse_sections(content_items, counter, mets_doc)
-        # Remove cis that are contained in sections
-        content_items, removed = remove_section_cis(content_items, section_cis)
-        
-        logger.debug("Removed {} as they are in sections".format(removed))
-        # Add sections to CIs
-        content_items += section_cis
-        # Set ark_id
-        ark_link = mets_doc.find('mets').get('OBJID')
-        self.ark_id = ark_link.replace('https://persist.lu/', '')
-        
-        for ci in content_items:
-            
-            # ci['l']['parts'] = self._parse_mets_div(item_div)
-            
-            if ci['m']['tp'] == 'image':
-                self._process_image_ci(ci, mets_doc)
-            elif ci['m']['tp']:
-                for part in ci['l']['parts']:
-                    page_no = part["comp_page_no"]
-                    if page_no not in ci['m']['pp']:
-                        ci['m']['pp'].append(page_no)
-        
+            mets_doc,
+            x_res="ImageWidth",
+            y_res="ImageLength",
+            x_res_default=0,
+            y_res_default=0,
+        )  # Parse the resolution of page images
+
+        # Parse all the content items
+        content_items = self._parse_content_items(mets_doc)
+
         self.issue_data = {
             "cdt": strftime("%Y-%m-%d %H:%M:%S"),
             "i": content_items,
             "id": self.id,
             "ar": self.rights,
-            "pp": [p.id for p in self.pages]
+            "pp": [p.id for p in self.pages],
         }
-        
-        if self._notes:
-            self.issue_data["n"] = "\n".join(self._notes)
+
+    def _get_image_info(self, content_item: dict[str, Any]) -> tuple[list[int], str]:
+        """Recover the coordinates and iiif link for an image content item.
+
+        The iiif link is embedded with the coordinates to directly crop the
+        newspaper page to the image.
+
+        Args:
+            content_item (dict[str, Any]): Content item of an image.
+
+        Returns:
+            tuple[list[int], str]: Coordinates on the page and iiif link
+        """
+        # Images cannot be on multiple pages
+        num_pages = len(content_item["m"]["pp"])
+        assert num_pages == 1, "Image is on more than one page"
+
+        page_nb = content_item["m"]["pp"][0]
+        page = [p for p in self.pages if p.number == page_nb][0]
+        parts = content_item["l"]["parts"]
+
+        assert len(parts) >= 1, f"No parts for image {content_item['m']['id']}"
+
+        if len(parts) > 1:
+            logger.info(
+                "Found multiple parts for image %s, selecting largest one",
+                content_item["m"]["id"],
+            )
+
+        coords = None
+        max_area = 0
+        # Image can have multiple parts, choose largest one (with max area)
+        for part in parts:
+            comp_id = part["comp_id"]
+
+            elements = page.xml.findAll(["ComposedBlock", "TextBlock"], {"ID": comp_id})
+            assert_msg = "Image comp_id matches multiple TextBlock tags"
+            assert len(elements) <= 1, assert_msg
+            if len(elements) == 0:
+                continue
+
+            element = elements[0]
+            hpos, vpos = element.get("HPOS"), element.get("VPOS")
+            width, height = element.get("WIDTH"), element.get("HEIGHT")
+
+            # Select largest image
+            area = int(float(width)) * int(float(height))
+            if area > max_area:
+                max_area = area
+                coords = [
+                    int(float(hpos)),
+                    int(float(vpos)),
+                    int(float(width)),
+                    int(float(height)),
+                ]
+
+        coords = convert_coordinates(
+            coords, self.image_properties[page.number], page.page_width
+        )
+
+        iiif_link = os.path.join(IIIF_ENDPOINT_URI, page.id, IIIF_SUFFIX)
+
+        return coords, iiif_link
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/lux/detect.py` & `impresso_text_importer-1.1.0/text_importer/importers/lux/detect.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,30 +7,18 @@
 from datetime import date
 
 from dask import bag as db
 from impresso_commons.path.path_fs import _apply_datefilter
 
 logger = logging.getLogger(__name__)
 
-EDITIONS_MAPPINGS = {
-    1: 'a',
-    2: 'b',
-    3: 'c',
-    4: 'd',
-    5: 'e'
-}
+EDITIONS_MAPPINGS = {1: "a", 2: "b", 3: "c", 4: "d", 5: "e"}
 
 LuxIssueDir = namedtuple(
-    "IssueDirectory", [
-        'journal',
-        'date',
-        'edition',
-        'path',
-        'rights'
-    ]
+    "IssueDirectory", ["journal", "date", "edition", "path", "rights"]
 )
 """A light-weight data structure to represent a newspaper issue.
 
 This named tuple contains basic metadata about a newspaper issue. They
 can then be used to locate the relevant data in the filesystem or to create
 canonical identifiers for the issue and its pages.
 
@@ -59,31 +47,27 @@
     Args:
         path (str): Path of issue.
 
     Returns:
         Rero2IssueDir: New `LuxIssueDir` object matching the path and rights.
     """
     issue_dir = os.path.basename(path)
-    local_id = issue_dir.split('_')[2]
-    issue_date = issue_dir.split('_')[3]
-    year, month, day = issue_date.split('-')
-    rights = 'open_public' if 'public_domain' in path else 'closed'
-
-    if len(issue_dir.split('_')) == 4:
-        edition = 'a'
-    elif len(issue_dir.split('_')) == 5:
-        edition = issue_dir.split('_')[4]
+    local_id = issue_dir.split("_")[2]
+    issue_date = issue_dir.split("_")[3]
+    year, month, day = issue_date.split("-")
+    rights = "open_public" if "public_domain" in path else "closed"
+
+    if len(issue_dir.split("_")) == 4:
+        edition = "a"
+    elif len(issue_dir.split("_")) == 5:
+        edition = issue_dir.split("_")[4]
         edition = EDITIONS_MAPPINGS[int(edition)]
 
     return LuxIssueDir(
-        local_id,
-        date(int(year), int(month), int(day)),
-        edition,
-        path,
-        rights
+        local_id, date(int(year), int(month), int(day)), edition, path, rights
     )
 
 
 def detect_issues(base_dir: str, ar: str = None) -> list[LuxIssueDir]:
     """Detect newspaper issues to import within the filesystem.
 
     This function expects the directory structure that BNL used to
@@ -93,21 +77,21 @@
         base_dir (str): Path to the base directory of newspaper data.
         ar (str, optional): Access rights, not used for this imported, but
             argument is kept for uniformity. Defaults to None.
 
     Returns:
         list[LuxIssueDir]: List of `LuxIssueDir` instances, to be imported.
     """
-    dir_path, dirs, files = next(os.walk(base_dir))
+    dir_path, dirs, _ = next(os.walk(base_dir))
     batches_dirs = [os.path.join(dir_path, dir) for dir in dirs]
     issue_dirs = [
         os.path.join(batch_dir, dir)
         for batch_dir in batches_dirs
         for dir in os.listdir(batch_dir)
-        if 'newspaper' in dir
+        if "newspaper" in dir
     ]
     return [dir2issue(_dir) for _dir in issue_dirs]
 
 
 def select_issues(
     base_dir: str, config: dict, access_rights: str
 ) -> list[LuxIssueDir] | None:
@@ -129,29 +113,32 @@
     """
     try:
         filter_dict = config["newspapers"]
         exclude_list = config["exclude_newspapers"]
         year_flag = config["year_only"]
 
     except KeyError:
-        logger.critical(f"The key [newspapers|exclude_newspapers|year_only] "
-                        "is missing in the config file.")
+        logger.critical(
+            "The key [newspapers|exclude_newspapers|year_only] "
+            "is missing in the config file."
+        )
         return
 
     issues = detect_issues(base_dir, access_rights)
     issue_bag = db.from_sequence(issues)
-    selected_issues = (
-        issue_bag.filter(
-            lambda i: (
-                len(filter_dict) == 0 or i.journal in filter_dict.keys()
-            ) and i.journal not in exclude_list
-        ).compute()
-    )
+    selected_issues = issue_bag.filter(
+        lambda i: (len(filter_dict) == 0 or i.journal in filter_dict.keys())
+        and i.journal not in exclude_list
+    ).compute()
 
     exclude_flag = False if not exclude_list else True
-    filtered_issues = _apply_datefilter(
-        filter_dict, selected_issues, year_only=year_flag
-    ) if not exclude_flag else selected_issues
-    logger.info(f"{len(filtered_issues)} newspaper issues remained "
-                f"after applying filter: {filtered_issues}")
+    filtered_issues = (
+        _apply_datefilter(filter_dict, selected_issues, year_only=year_flag)
+        if not exclude_flag
+        else selected_issues
+    )
+    msg = (
+        f"{len(filtered_issues)} newspaper issues remained "
+        f"after applying filter: {filtered_issues}"
+    )
+    logger.info(msg)
     return filtered_issues
-
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/lux/helpers.py` & `impresso_text_importer-1.1.0/text_importer/importers/lux/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from text_importer.importers import CONTENTITEM_TYPE_IMAGE
 from bs4.element import Tag
 from typing import Any
 
 NON_ARTICLE = ["advertisement", "death_notice"]
 
 
-def convert_coordinates(hpos: int, vpos: int, width: int, height: int,
-                        x_res: float, y_res: float) -> list[int]:
+def convert_coordinates(
+    hpos: int, vpos: int, width: int, height: int, x_res: float, y_res: float
+) -> list[int]:
     """Convert the coordinates to iiif-compliant ones using the resolution.
 
     - x = (coordinate['xResolution']/254.0) * coordinate['hpos']
     - y = (coordinate['yResolution']/254.0) * coordinate['vpos']
     - w = (coordinate['xResolution']/254.0) * coordinate['width']
     - h = (coordinate['yResolution']/254.0) * coordinate['height']
 
@@ -27,39 +28,40 @@
     """
     x = (x_res / 254) * hpos
     y = (y_res / 254) * vpos
     w = (x_res / 254) * width
     h = (y_res / 254) * height
     return [int(x), int(y), int(w), int(h)]
 
+
 def encode_ark(ark: str) -> str:
     """Replaces (encodes) backslashes in the Ark identifier.
 
     Args:
         ark (str): original ark identifier.
 
     Returns:
         str: New ark identifier with encoded backslashes.
     """
-    return ark.replace('/', '%2f')
+    return ark.replace("/", "%2f")
 
 
-def div_has_body(div: Tag, body_type='body') -> bool:
+def div_has_body(div: Tag, body_type="body") -> bool:
     """Checks if the given `div` has a body in it's direct children.
 
     Args:
         div (Tag): `div` element to check.
         body_type (str, optional): Content type of a body. Defaults to 'body'.
 
     Returns:
         bool: True if one or more of `div`'s direct children have a body.
     """
     children_types = set()
-    for i in div.findChildren('div', recursive=False):
-        child_type = i.get('TYPE')
+    for i in div.findChildren("div", recursive=False):
+        child_type = i.get("TYPE")
         if child_type is not None:
             children_types.add(child_type.lower())
     return body_type in children_types
 
 
 def section_is_article(section_div: Tag) -> bool:
     """Check if the given section `div` is an article.
@@ -70,76 +72,74 @@
     Args:
         section_div (Tag): section `div` to check.
 
     Returns:
         bool: True if given `div` is an article section.
     """
     types = []
-    for c in section_div.findChildren('div'):
-        _type = c.get('TYPE').lower()
-        if not (_type == 'body' or _type == 'body_content'):
+    for c in section_div.findChildren("div"):
+        _type = c.get("TYPE").lower()
+        if not (_type == "body" or _type == "body_content"):
             types.append(_type)
     return not all(t in NON_ARTICLE for t in types)
 
 
 def find_section_articles(
     section_div: Tag, content_items: list[dict[str, Any]]
 ) -> list[str]:
     """Parse the articles inside the section div and get their content item ID.
 
-    Recover the content item canonical ID corresponding to each article using 
+    Recover the content item canonical ID corresponding to each article using
     the legacy ID (from the OCR) of the articles found in `div`'s children.
 
     Args:
         section_div (Tag): `div` with the articles for which to get CI IDs.
         content_items (list[dict[str, Any]]): Content items already identified.
 
     Returns:
         list[str]: List of content item IDs for `div`'s children articles.
     """
     articles_lid = []
     for d in section_div.findChildren("div", {"TYPE": "ARTICLE"}):
-        article_id = d.get('DMDID')
+        article_id = d.get("DMDID")
         if article_id is not None:
             articles_lid.append(article_id)
-    
+
     children_art = []
     # Then search for corresponding content item
     for i in articles_lid:
         for ci in content_items:
-            if i == ci['l']['id']:
-                children_art.append(ci['m']['id'])
+            if i == ci["l"]["id"]:
+                children_art.append(ci["m"]["id"])
     return children_art
 
 
 def remove_section_cis(
     content_items: list[dict[str, Any]], sections: list[dict[str, Any]]
 ) -> tuple[list[dict[str, Any]], list[dict[str, Any]]]:
     """Remove undesired content items based on the formed sections.
 
     Some content items are contained within a section and should not be in the
-    content items. Given the recovered section content items, they can be 
+    content items. Given the recovered section content items, they can be
     removed.
 
     Args:
         content_items (list[dict[str, Any]]): Content items, to be filtered.
         sections (list[dict[str, Any]]): Formed section content items.
 
     Returns:
-        tuple[list[dict[str, Any]], list[dict[str, Any]]]: Filtered 
+        tuple[list[dict[str, Any]], list[dict[str, Any]]]: Filtered
             content items and ones that were removed.
     """
-    to_remove = [j for i in sections for j in i['l']['canonical_parts']]
+    to_remove = [j for i in sections for j in i["l"]["canonical_parts"]]
     if len(to_remove) == 0:
         return content_items, []
-        
+
     to_remove = set(to_remove)
     new_cis = []
     removed = []
     for ci in content_items:
-        if ci['m']['id'] not in to_remove or ci['m']['tp'] == CONTENTITEM_TYPE_IMAGE:
+        if ci["m"]["id"] not in to_remove or ci["m"]["tp"] == CONTENTITEM_TYPE_IMAGE:
             new_cis.append(ci)
-            removed.append(ci['m']['id'])
-    
-    return new_cis, list(to_remove)
-
+            removed.append(ci["m"]["id"])
 
+    return new_cis, list(to_remove)
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/lux/test_dask_memory.py` & `impresso_text_importer-1.1.0/text_importer/importers/lux/test_dask_memory.py`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/mets_alto/alto.py` & `impresso_text_importer-1.1.0/text_importer/importers/mets_alto/alto.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,150 +14,145 @@
     Args:
         element (Tag): Input XML tag containing coordinates to distill.
 
     Returns:
         list[int]: An ordered list of coordinates (``x``, ``y``, ``width``,
             ``height``).
     """
-    hpos = int(float(element.get('HPOS')))
-    vpos = int(float(element.get('VPOS')))
-    width = int(float(element.get('WIDTH')))
-    height = int(float(element.get('HEIGHT')))
-    
+    hpos = int(float(element.get("HPOS")))
+    vpos = int(float(element.get("VPOS")))
+    width = int(float(element.get("WIDTH")))
+    height = int(float(element.get("HEIGHT")))
+
     # NB: these coordinates need to be converted
     return [hpos, vpos, width, height]
 
 
 def parse_textline(element: Tag) -> tuple[dict, list[str]]:
     """Parse the ``<TextLine>`` element of an ALTO XML document.
 
     Args:
         element (Tag): Input XML element (``<TextLine>``).
 
     Returns:
         tuple[dict, list[str]]: Parsed lines or text in the canonical format
-            and notes about potential missing token coordinates. 
+            and notes about potential missing token coordinates.
     """
     line = {}
-    line['c'] = distill_coordinates(element)
+    line["c"] = distill_coordinates(element)
     tokens = []
-    
+
     notes = []
     for child in element.children:
-        
+
         if isinstance(child, bs4.element.NavigableString):
             continue
-        
-        if child.name == 'String':
-            
+
+        if child.name == "String":
+
             # Here we do this in case coordinates are not found for this String
             try:
                 coords = distill_coordinates(child)
-            except TypeError as e:
+            except TypeError:
                 notes.append(f"Token {child.get('ID')} does not have coordinates")
+                coords = None
                 continue
-            token = {
-                'c': coords,
-                'tx': child.get('CONTENT')
-            }
-            
-            if child.get('SUBS_TYPE') == "HypPart1":
+
+            token = {"c": coords, "tx": child.get("CONTENT")}
+
+            if child.get("SUBS_TYPE") == "HypPart1":
                 # token['tx'] += u"\u00AD"
-                token['tx'] += "-"
-                token['hy'] = True
-            elif child.get('SUBS_TYPE') == "HypPart2":
-                token['nf'] = child.get('SUBS_CONTENT')
-            
+                token["tx"] += "-"
+                token["hy"] = True
+            elif child.get("SUBS_TYPE") == "HypPart2":
+                token["nf"] = child.get("SUBS_CONTENT")
+
             tokens.append(token)
-    
-    line['t'] = tokens
+
+    line["t"] = tokens
     return line, notes
 
 
-def parse_printspace(element: Tag, mappings: dict[str, str]
+def parse_printspace(
+    element: Tag, mappings: dict[str, str]
 ) -> tuple[list[dict], list[str]]:
     """Parse the ``<PrintSpace>`` element of an ALTO XML document.
 
     This element contains all the OCR information about the content items of
-    a page, up to the lowest level of the hierarchy: the regions, paragraphs, 
+    a page, up to the lowest level of the hierarchy: the regions, paragraphs,
     lines and tokens, each with their corresponding coordinates.
-    
+
     Args:
         element (Tag): Input XML element (``<PrintSpace>``).
-        mappings (dict[str, str]): Mapping from OCR component ids to their 
+        mappings (dict[str, str]): Mapping from OCR component ids to their
             corresponding canonical Content Item ID.
 
     Returns:
         tuple[list[dict], list[str]]: List of page regions in the canonical
-            format and notes about potential parsing problems. 
+            format and notes about potential parsing problems.
     """
-    
+
     regions = []
     notes = []
     # in case of a blank page, the PrintSpace element is not found thus
     # it will be none
     if element:
         for block in element.children:
-            
+
             if isinstance(block, bs4.element.NavigableString):
                 continue
-            
-            block_id = block.get('ID')
+
+            block_id = block.get("ID")
             if block_id in mappings:
                 part_of_contentitem = mappings[block_id]
             else:
                 part_of_contentitem = None
-            
+
             coordinates = distill_coordinates(block)
-            
+
             tmp = [
                 parse_textline(line_element)
-                for line_element in block.findAll('TextLine')
+                for line_element in block.findAll("TextLine")
             ]
-            
+
             if len(tmp) > 0:
                 lines, new_notes = list(zip(*tmp))
                 new_notes = [i for n in new_notes for i in n]
             else:
                 lines, new_notes = [], []
-            
-            paragraph = {
-                "c": coordinates,
-                "l": lines
-            }
-            
-            region = {
-                "c": coordinates,
-                "p": [paragraph]
-            }
-            
+
+            paragraph = {"c": coordinates, "l": lines}
+
+            region = {"c": coordinates, "p": [paragraph]}
+
             if part_of_contentitem:
-                region['pOf'] = part_of_contentitem
-            
+                region["pOf"] = part_of_contentitem
+
             notes += new_notes
             regions.append(region)
     return regions, notes
 
+
 def parse_style(style_div: Tag) -> dict[str, float | str]:
     """Parse the font-style information in the ALTO files (for BNL and BNF).
 
     Args:
         style_div (Tag): Element of XML file containing font-style information.
 
     Returns:
         dict[str, float | str]: Parsed style for Issue canonical format.
     """
     font_family = style_div.get("FONTFAMILY")
     font_size = style_div.get("FONTSIZE")
     font_style = style_div.get("FONTSTYLE")
     font_id = style_div.get("ID")
-    
+
     font_name = font_family
     if font_style is not None:
         font_name = "{}-{}".format(font_name, font_style)
-    
+
     style = {
         "id": font_id,
-        "fs": float(font_size),
-        "f": font_name
+        "fs": float(font_size) if font_size != "" else None,
+        "f": font_name,
     }
     return style
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/mets_alto/classes.py` & `impresso_text_importer-1.1.0/text_importer/importers/mets_alto/classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class MetsAltoNewspaperPage(NewspaperPage):
     """Newspaper page in generic Alto format.
 
-    Note: 
+    Note:
         New Mets/Alto importers should sub-classes this class and implement
         its abstract methods (i.e. :meth:`~MetsAltoNewspaperPage.add_issue()`).
 
     Args:
         _id (str): Canonical page ID.
         number (int): Page number.
         filename (str): Name of the Alto XML page file.
@@ -44,96 +44,106 @@
         number (int): Page number.
         page_data (dict[str, Any]): Page data according to canonical format.
         issue (NewspaperIssue): Issue this page is from.
         filename (str): Name of the Alto XML page file.
         basedir (str): Base directory where Alto files are located.
         encoding (str, optional): Encoding of XML file.
     """
-    
-    def __init__(self, _id: str, number: int, filename: str,
-                 basedir: str, encoding: str = 'utf-8') -> None:
+
+    def __init__(
+        self,
+        _id: str,
+        number: int,
+        filename: str,
+        basedir: str,
+        encoding: str = "utf-8",
+    ) -> None:
         super().__init__(_id, number)
         self.filename = filename
         self.basedir = basedir
         self.encoding = encoding
         self.page_data = {
-            'id': _id,
-            'cdt': strftime("%Y-%m-%d %H:%M:%S"),
-            'r': []  # here go the page regions
-            }
-    
+            "id": _id,
+            "cdt": strftime("%Y-%m-%d %H:%M:%S"),
+            "r": [],  # here go the page regions
+        }
+
     @property
     def xml(self) -> BeautifulSoup:
         """Read Alto XML file of the page and create a BeautifulSoup object.
 
         Returns:
             BeautifulSoup: BeautifulSoup object with Alto XML of the page.
         """
         alto_xml_path = os.path.join(self.basedir, self.filename)
-        
+
         # In case of I/O error, retry twice,
         tries = 3
         for i in range(tries):
             try:
-                with open(alto_xml_path, 'r', encoding=self.encoding) as f:
+                with open(alto_xml_path, "r", encoding=self.encoding) as f:
                     raw_xml = f.read()
-                
-                alto_doc = BeautifulSoup(raw_xml, 'xml')
+
+                alto_doc = BeautifulSoup(raw_xml, "xml")
                 return alto_doc
             except IOError as e:
-                if i < tries - 1: # i is zero indexed
-                    logger.warning(f"Caught error for {self.id}, retrying (up to {tries} times) to read xml file. Error: {e}.")
+                if i < tries - 1:  # i is zero indexed
+                    msg = (
+                        f"Caught error for {self.id}, retrying (up to {tries} "
+                        f"times) to read xml file. Error: {e}."
+                    )
+                    logger.error(msg)
                     continue
                 else:
-                    logger.warning(f"Reached maximum amount of errors for {self.id}.")
+                    logger.error("Reached maximum amount of errors for %s.", self.id)
                     raise e
 
-    
-    def _convert_coordinates(self, page_regions: list[dict[str, Any]]
+    def _convert_coordinates(
+        self, page_regions: list[dict[str, Any]]
     ) -> tuple[bool, list[dict[str, Any]]]:
         """Convert region coordinates to iiif format if possible.
 
         Args:
             page_regions (list[dict[str, Any]]): Page regions from canonical
                 Page format.
 
         Returns:
             tuple[bool, list[dict[str, Any]]]: Whether the region coordinates
                 are in iiif format and page regions.
         """
         return True, page_regions
-    
+
     @abstractmethod
     def add_issue(self, issue: NewspaperIssue) -> None:
         pass
-    
+
     def parse(self) -> None:
         doc = self.xml
-        
+
         mappings = {}
-        for ci in self.issue.issue_data['i']:
-            ci_id = ci['m']['id']
-            if 'parts' in ci['l']:
-                for part in ci['l']['parts']:
-                    mappings[part['comp_id']] = ci_id
-        
-        pselement = doc.find('PrintSpace')
+        for ci in self.issue.issue_data["i"]:
+            ci_id = ci["m"]["id"]
+            if "parts" in ci["l"]:
+                for part in ci["l"]["parts"]:
+                    mappings[part["comp_id"]] = ci_id
+
+        pselement = doc.find("PrintSpace")
         page_regions, notes = alto.parse_printspace(pselement, mappings)
-        self.page_data['cc'], self.page_data["r"] = self._convert_coordinates(
+        self.page_data["cc"], self.page_data["r"] = self._convert_coordinates(
             page_regions
         )
         # Add notes for missing coordinates in SWA
         if len(notes) > 0:
-            self.page_data['n'] = notes
+            self.page_data["n"] = notes
 
 
 class MetsAltoNewspaperIssue(NewspaperIssue):
     """Newspaper issue in generic Mets/Alto format.
 
-    Note: 
+    Note:
         New Mets/Alto importers should sub-class this class and implement
         its abstract methods (i.e. ``_find_pages()``, ``_parse_mets()``).
 
     Args:
         issue_dir (IssueDir): Identifying information about the issue.
 
     Attributes:
@@ -141,37 +151,35 @@
         edition (str): Lower case letter ordering issues of the same day.
         journal (str): Newspaper unique identifier or name.
         path (str): Path to directory containing the issue's OCR data.
         date (datetime.date): Publication date of issue.
         issue_data (dict[str, Any]): Issue data according to canonical format.
         pages (list): list of :obj:`NewspaperPage` instances from this issue.
         rights (str): Access rights applicable to this issue.
-        image_properties (dict[str, Any]): metadata allowing to convert region 
+        image_properties (dict[str, Any]): metadata allowing to convert region
             OCR/OLR coordinates to iiif format compliant ones.
         ark_id (int): Issue ARK identifier, for the issue's pages' iiif links.
     """
-    
+
     def __init__(self, issue_dir: IssueDir) -> None:
         super().__init__(issue_dir)
         # create the canonical issue id
         self.image_properties = {}
         self.ark_id = None
-        
+
         self._find_pages()
         self._parse_mets()
-    
+
     @abstractmethod
     def _find_pages(self) -> None:
         pass
-    
+
     @abstractmethod
     def _parse_mets(self) -> None:
-        """Parse the Mets XML file corresponding to this issue.
-        """
-        pass
+        """Parse the Mets XML file corresponding to this issue."""
 
     @property
     def xml(self) -> BeautifulSoup:
         """Read Mets XML file of the issue and create a BeautifulSoup object.
 
         During the processing, some IO errors can randomly happen when listing
         the contents of the directory, or opening files, preventing the correct
@@ -179,41 +187,42 @@
         If the directory does not contain any Mets file, only try once.
 
         Note:
             By default the issue Mets file is the only file containing
             `mets.xml` in its file name and located in the directory
             `self.path`. Individual importers can overwrite this behavior
             if necessary.
-    
+
         Returns:
             BeautifulSoup: BeautifulSoup object with Mets XML of the issue.
         """
         tries = 3
         for i in range(tries):
             try:
                 mets_file = [
                     os.path.join(self.path, f)
                     for f in os.listdir(self.path)
-                    if 'mets.xml' in f.lower()
+                    if "mets.xml" in f.lower()
                 ]
                 if len(mets_file) == 0:
-                    logger.critical(f"Could not find METS file in {self.path}")
+                    logger.critical("Could not find METS file in %s", self.path)
                     tries = 1
-                    #return
-                
+                    # return
+
                 mets_file = mets_file[0]
 
-                with open(mets_file, 'r', encoding="utf-8") as f:
+                with open(mets_file, "r", encoding="utf-8") as f:
                     raw_xml = f.read()
-                
-                mets_doc = BeautifulSoup(raw_xml, 'xml')
+
+                mets_doc = BeautifulSoup(raw_xml, "xml")
                 return mets_doc
             except IOError as e:
-                if i < tries - 1: # i is zero indexed
-                    logger.warning(f"Caught error for {self.id}, "
-                                   f"retrying (up to {tries} times) to read "
-                                   f"xml file or listing the dir. Error: {e}.")
+                if i < tries - 1:  # i is zero indexed
+                    msg = (
+                        f"Caught error for {self.id}, retrying (up to {tries} times) "
+                        f"to read xml file or listing the dir. Error: {e}."
+                    )
+                    logger.warning(msg)
                     continue
                 else:
-                    logger.warning("Reached maximum amount of "
-                                   f"errors for {self.id}.")
-                    raise e
+                    logger.warning("Reached maximum amount of errors for %s.", self.id)
+                    raise e
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/mets_alto/mets.py` & `impresso_text_importer-1.1.0/text_importer/importers/mets_alto/mets.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,90 +17,90 @@
     Args:
         mets_doc (BeautifulSoup): BeautifulSoup object of Mets XML document.
 
     Returns:
         dict[int, str]: Mapping from page number to page image id.
     """
     image_filegroup = mets_doc.findAll(
-        'fileGrp', {"USE": lambda x: x and x.lower() == 'images'}
+        "fileGrp", {"USE": lambda x: x and x.lower() == "images"}
     )[0]
 
     return {
         int(child.get("SEQ")): child.get("ADMID")
-        for child in image_filegroup.findAll('file')
+        for child in image_filegroup.findAll("file")
     }
 
 
 def parse_mets_amdsec(
-    mets_doc: BeautifulSoup, 
-    x_res: str, 
-    y_res: str, 
-    x_res_default: int = 300, 
-    y_res_default: int = 300
+    mets_doc: BeautifulSoup,
+    x_res: str,
+    y_res: str,
+    x_res_default: int = 300,
+    y_res_default: int = 300,
 ) -> dict:
     """Parse the ``<amdsec>`` section of Mets XML to extract image properties.
 
     The ``<amdsec>`` section contains administrative metadata about the OCR, in
-    particular information about the image resolution allowing the coordinates 
+    particular information about the image resolution allowing the coordinates
     conversion to iiif format.
 
     Args:
         mets_doc (BeautifulSoup): BeautifulSoup object of Mets XML document.
         x_res (str): Name of field representing the X resolution.
         y_res (str): Name of field representing the Y resolution.
         x_res_default (int, optional): Default X_res. Defaults to 300.
         y_res_default (int, optional): Default Y res. Defaults to 300.
 
     Returns:
         dict: Parsed image properties with default values if the field was not
             found in the document.
     """
-    page_image_ids = parse_mets_filegroup(mets_doc) # Returns {page: im_id}
-    
+    page_image_ids = parse_mets_filegroup(mets_doc)  # Returns {page: im_id}
+
     amd_sections = {
         # Returns {page_id: amdsec}
-        image_id: mets_doc.findAll('amdSec', {'ID': image_id})[0]  
+        image_id: mets_doc.findAll("amdSec", {"ID": image_id})[0]
         for image_id in page_image_ids.values()
     }
-    
+
     image_properties_dict = {}
     for image_no, image_id in page_image_ids.items():
         amd_sect = amd_sections[image_id]
         try:
             x_res_val = (
-                int(amd_sect.find(x_res).text) 
-                if amd_sect.find(x_res) is not None 
+                int(amd_sect.find(x_res).text)
+                if amd_sect.find(x_res) is not None
                 else x_res_default
             )
             y_res_val = (
-                int(amd_sect.find(x_res).text) 
-                if amd_sect.find(x_res) is not None 
+                int(amd_sect.find(y_res).text)
+                if amd_sect.find(y_res) is not None
                 else x_res_default
             )
             image_properties_dict[image_no] = {
-                'x_resolution': x_res_val,
-                'y_resolution': y_res_val
+                "x_resolution": x_res_val,
+                "y_resolution": y_res_val,
             }
         # if it fails it's because of value < 1
         except Exception as e:
-            logger.debug(f'Error occured when parsing {e}')
+            logger.debug("Error occured when parsing %s", e)
             image_properties_dict[image_no] = {
-                'x_resolution': x_res_default,
-                'y_resolution': y_res_default
+                "x_resolution": x_res_default,
+                "y_resolution": y_res_default,
             }
     return image_properties_dict
 
 
-def get_dmd_sec(mets_doc: BeautifulSoup, filter: str) -> Tag:
+def get_dmd_sec(mets_doc: BeautifulSoup, _filter: str) -> Tag:
     """Extract the contents of a specific ``<dmdsec>`` from the Mets document.
 
-    The ``<dmdsec>`` section contains descriptive metadata. It's composed of 
+    The ``<dmdsec>`` section contains descriptive metadata. It's composed of
     several different subsections each identified with string IDs.
 
     Args:
         mets_doc (BeautifulSoup): BeautifulSoup object of Mets XML document.
-        filter (str): ID of the subsection of interest to filter the search.
+        _filter (str): ID of the subsection of interest to filter the search.
 
     Returns:
         Tag: Contents of the desired ``<dmdsec>`` of the Mets XML document.
     """
-    return mets_doc.find("dmdSec", {"ID": filter})
+    return mets_doc.find("dmdSec", {"ID": _filter})
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/olive/classes.py` & `impresso_text_importer-1.1.0/text_importer/importers/olive/classes.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,30 +12,34 @@
 from typing import Any
 from zipfile import ZipFile
 
 from impresso_commons.path import IssueDir
 from impresso_commons.path.path_fs import canonical_path
 
 from text_importer.importers.classes import NewspaperIssue, NewspaperPage, ZipArchive
-from text_importer.importers.olive.helpers import (combine_article_parts,
-                                                   convert_image_coordinates,
-                                                   convert_page_coordinates,
-                                                   get_clusters,
-                                                   recompose_page,
-                                                   recompose_ToC)
-from text_importer.importers.olive.parsers import (olive_image_parser,
-                                                   olive_parser,
-                                                   olive_toc_parser,
-                                                   parse_styles)
+from text_importer.importers.olive.helpers import (
+    combine_article_parts,
+    convert_image_coordinates,
+    convert_page_coordinates,
+    get_clusters,
+    recompose_page,
+    recompose_ToC,
+)
+from text_importer.importers.olive.parsers import (
+    olive_image_parser,
+    olive_parser,
+    olive_toc_parser,
+    parse_styles,
+)
 from text_importer.utils import get_issue_schema, get_page_schema
 
 logger = logging.getLogger(__name__)
 IssueSchema = get_issue_schema()
 Pageschema = get_page_schema()
-IMPRESSO_IIIF_BASEURI = "https://impresso-project.ch/api/proxy/iiif/"
+IIIF_ENDPOINT_URI = "https://impresso-project.ch/api/proxy/iiif/"
 
 
 class OliveNewspaperPage(NewspaperPage):
     """Newspaper page in Olive format.
 
     Args:
         _id (str): Canonical page ID.
@@ -50,91 +54,89 @@
         page_data (dict[str, Any]): Page data according to canonical format.
         issue (NewspaperIssue | None): Issue this page is from.
         toc_data (dict): Metadata about content items in the newspaper issue.
         image_info (dict): Metadata about the page image.
         page_xml (str): Path to the Olive XML file of the page.
         archive (ZipArchive): Archive of the issue this page is from.
     """
-    
-    def __init__(self, _id: str, number: int, toc_data: dict, 
-                 image_info: dict, page_xml: str) -> None:
+
+    def __init__(
+        self, _id: str, number: int, toc_data: dict, image_info: dict, page_xml: str
+    ) -> None:
         super().__init__(_id, number)
         self.toc_data = toc_data
         self.page_data = None
         self.image_info = image_info
         self.page_xml = page_xml
         self.archive = None
-    
+
     def parse(self) -> None:
         """Process the page XML file and transform into canonical Page format.
 
         Note:
             This lazy behavior means that the page contents are not processed
             upon creation of the page object, but only once the ``parse()``
             method is called.
 
         Raises:
             ValueError: No Newspaper issue has been added to this page.
         """
         if self.issue is None:
             raise ValueError(f"No NewspaperIssue for {self.id}")
-        
+
         element_ids = self.toc_data.keys()
         elements = {
             el["legacy"]["id"]: el
             for el in json.loads(self.issue.content_elements)
             if (el["legacy"]["id"] in element_ids)
         }
-        
+
         self.page_data = recompose_page(
-            self.id,
-            self.toc_data,
-            elements,
-            self.issue.clusters
+            self.id, self.toc_data, elements, self.issue.clusters
         )
-        
-        self.page_data['id'] = self.id
-        self.page_data['iiif'] = os.path.join(IMPRESSO_IIIF_BASEURI, self.id)
-        
-        if len(self.page_data['r']) == 0:
-            logger.warning(f"Page {self.id} has not OCR text")
-        
+
+        self.page_data["id"] = self.id
+        self.page_data["iiif_img_base_uri"] = os.path.join(IIIF_ENDPOINT_URI, self.id)
+
+        if len(self.page_data["r"]) == 0:
+            logger.warning("Page %s has not OCR text", self.id)
+
         self._convert_page_coords()
-        
+
         # if all(p.page_data is not None for p in self.issue.pages):
         #     # Means issue has been fully processed, can cleanup
         #     self.archive.cleanup()
-    
+
     def _convert_page_coords(self) -> None:
         """Convert page coordinates to the desired iiif format if possible.
 
         The conversion is attempted if `self.image_info` is defined, otherwise
         the page is simply skipped.
         """
-        self.page_data['cc'] = False
+        self.page_data["cc"] = False
         if self.image_info is not None:
             try:
-                box_strategy = self.image_info['strat']
-                image_name = self.image_info['s']
+                box_strategy = self.image_info["strat"]
+                image_name = self.image_info["s"]
                 was_converted = convert_page_coordinates(
                     self.page_data,
                     self.archive.read(self.page_xml),
                     image_name,
                     self.archive,
                     box_strategy,
-                    self.issue
+                    self.issue,
                 )
                 if was_converted:
-                    self.page_data['cc'] = True
+                    self.page_data["cc"] = True
             except Exception as e:
-                logger.error(f"Page {self.id} raised error: {e}")
-                logger.error(f"Couldn't convert coordinates in p. {self.id}")
+                logger.error("Page %s raised error: %s", self.id, e)
+                logger.error("Couldn't convert coordinates in p. %s", self.id)
         else:
-            logger.debug(f"Image {self.id} does not have image info")
-    
+            logger.debug("Image %s does not have image info", self.id)
+
     def add_issue(self, issue: NewspaperIssue) -> None:
         self.issue = issue
         self.archive = issue.archive
 
 
 class OliveNewspaperIssue(NewspaperIssue):
     """Newspaper Issue in Olive format.
@@ -142,76 +144,74 @@
     Upon object initialization the following things happen:
         - The Zip archive containing the issue is uncompressed.
         - The ToC file is parsed to determine the logical structure of the issue.
         - Page objects (instances of ``OliveNewspaperPage``) are initialized.
 
     Args:
         issue_dir (IssueDir): Identifying information about the issue.
-        image_dirs (str): Path to the directory with the page images. 
+        image_dirs (str): Path to the directory with the page images.
             Multiple paths should be separated by comma (",").
         temp_dir (str): Temporary directory to unpack ZipArchive objects.
 
     Attributes:
         id (str): Canonical Issue ID (e.g. ``GDL-1900-01-02-a``).
         edition (str): Lower case letter ordering issues of the same day.
         journal (str): Newspaper unique identifier or name.
         path (str): Path to directory containing the issue's OCR data.
         date (datetime.date): Publication date of issue.
         issue_data (dict[str, Any]): Issue data according to canonical format.
         pages (list): list of :obj:`NewspaperPage` instances from this issue.
         rights (str): Access rights applicable to this issue.
-        image_dirs (str): Path to the directory with the page images. 
+        image_dirs (str): Path to the directory with the page images.
             Multiple paths should be separated by comma (",").
         archive (ZipArchive): ZipArchive for this issue.
         toc_data (dict): Table of contents (ToC) data for this issue.
         content_elements (list[dict[str, Any]]): All content elements detected.
         content_items (list[dict[str, Any]]): Issue's recomposed content items.
         clusters (dict[str, list[str]]): Inverted index of legacy ids; values
             are clusters of articles, each indexed by one member.
     """
-    
+
     def __init__(self, issue_dir: IssueDir, image_dirs: str, temp_dir: str):
         super().__init__(issue_dir)
         self.image_dirs = image_dirs
-        logger.info(f"Starting to parse {self.id}")
-        
+        logger.info("Starting to parse %s", self.id)
+
         # First parse the archive and return it
         self.archive = self._parse_archive(temp_dir)
-        
+
         # Parse ToC
         self.toc_data = self._parse_toc()
-        
+
         # Parse image xml files with olive_image_parser
         images = self._parse_image_xml_files()
-        
+
         # Parse and recompose the ToC
         articles, self.content_elements = self._parse_articles()
         self.content_items = recompose_ToC(self.toc_data, articles, images)
-        
+
         self.clusters = get_clusters(articles)
-        
+
         # Work around to avoid non-pickle-able objects
         self.content_elements = json.dumps(self.content_elements)
         self._find_pages()
-        
+
         styles = self._parse_styles_gallery()  # Then parse the styles
-        
+
         self.issue_data = {
-                "id": self.id,
-                "cdt": strftime("%Y-%m-%d %H:%M:%S"),
-                "s": styles,
-                "i": self.content_items,
-                "pp": [p.id for p in self.pages],
-                "ar": self.rights
-                }
-        logger.info(f"Finished parsing {self.id}")
-    
-    def _parse_archive(
-        self, temp_dir: str, file: str = "Document.zip"
-    ) -> ZipArchive:
+            "id": self.id,
+            "cdt": strftime("%Y-%m-%d %H:%M:%S"),
+            "s": styles,
+            "i": self.content_items,
+            "pp": [p.id for p in self.pages],
+            "ar": self.rights,
+        }
+        logger.info("Finished parsing %s", self.id)
+
+    def _parse_archive(self, temp_dir: str, file: str = "Document.zip") -> ZipArchive:
         """Parse the archive containing the Olive OCR for this issue.
 
         Args:
             temp_dir (str): Temporary directory to unpack the archive.
             file (str, optional): Archive filename. Defaults to "Document.zip".
 
         Raises:
@@ -220,49 +220,46 @@
 
         Returns:
             ZipArchive: :obj:`ZipArchive` of the `file` with its contents.
         """
         archive_path = os.path.join(self.path, file)
         if os.path.isfile(archive_path):
             archive_tmp_path = os.path.join(
-                    temp_dir,
-                    canonical_path(self.issuedir, path_type='dir')
-                    )
-            
+                temp_dir, canonical_path(self.issuedir, path_type="dir")
+            )
+
             try:
                 archive = ZipFile(archive_path)
-                logger.debug((
-                        f"Contents of archive for {self.id}:"
-                        f" {archive.namelist()}"
-                ))
+                logger.debug(
+                    "Contents of archive for %s: %s", self.id, archive.namelist()
+                )
                 return ZipArchive(archive, archive_tmp_path)
             except Exception as e:
                 msg = f"Bad Zipfile for {self.id}, failed with error : {e}"
-                raise ValueError(msg)
+                raise ValueError(msg) from e
         else:
             msg = f"Could not find archive {file} for {self.id}"
             raise ValueError(msg)
-    
+
     def _get_page_xml_files(self) -> dict[int, str]:
         """Get all page XML files in `self.archive`, indexed by page number.
 
         Returns:
             dict[int, str]: Mapping from page number to XML file for each page.
         """
         page_xml = None
         if self.archive is not None:
             page_xml = {
-                    int(item.split("/")[0]): item
-                    for item in self.archive.namelist()
-                    if ".xml" in item and not item.startswith("._")
-                       and "/Pg" in item
-                    }
-        
+                int(item.split("/")[0]): item
+                for item in self.archive.namelist()
+                if ".xml" in item and not item.startswith("._") and "/Pg" in item
+            }
+
         return page_xml
-    
+
     def _parse_toc(self, file: str = "TOC.xml") -> dict[int, dict[str, dict]]:
         """Parse the XML file containing the issue's ToC.
 
         For each page, the resulting parsed ToC contains a dict mapping legacy
         content item IDs to their metadata.
 
         Args:
@@ -275,178 +272,184 @@
         Returns:
             dict[int, dict[str, dict]]: Parsed ToC dict
         """
         toc_path = os.path.join(self.path, file)
         try:
             toc_data = olive_toc_parser(toc_path, self.issuedir)
             logger.debug(toc_data)
-        except FileNotFoundError:
-            raise FileNotFoundError(f'Missing ToC.xml for {self.id}')
+        except FileNotFoundError as e:
+            msg = f"Missing ToC.xml for {self.id}"
+            raise FileNotFoundError(msg) from e
         except Exception as e:
-            logger.error(f'Corrupted ToC.xml for {self.id}')
+            logger.error("Corrupted ToC.xml for %s", self.id)
             raise e
         return toc_data
-    
+
     def _parse_image_xml_files(self) -> list[dict[str, str]]:
         """Find image XML files and extract the image metadata.
 
         Returns:
             list[dict[str, str]]: Metadata about all images in issue.
         """
         image_xml_files = [
-                item
-                for item in self.archive.namelist()
-                if ".xml" in item and not item.startswith("._") and "/Pc" in item
-                ]
-        
+            item
+            for item in self.archive.namelist()
+            if ".xml" in item and not item.startswith("._") and "/Pc" in item
+        ]
+
         images = []
         for image_file in image_xml_files:
             try:
                 image_data = olive_image_parser(self.archive.read(image_file))
                 # because of course there are empty files!
                 if image_data is not None:
                     images.append(image_data)
             except Exception as e:
                 # there are e.g. image file with empty coordinate attributes
                 msg = f"Parsing img file {image_file} in {self.id} failed"
                 logger.error(msg)
                 logger.error(e)
         return images
-    
+
     def _parse_styles_gallery(
-        self, file: str = 'styleGallery.txt'
+        self, file: str = "styleGallery.txt"
     ) -> list[dict[str, Any]]:
         """Parse the style file (plain text).
 
         Args:
             file (str, optional): Filename. Defaults to 'styleGallery.txt'.
 
         Returns:
             list[dict[str, Any]]: list of styles according to canonical format.
         """
         styles = []
         if file in self.archive.namelist():
             try:
                 styles = parse_styles(self.archive.read(file).decode())
             except Exception as e:
-                logger.warning((f"Parsing styles file {file}"
-                                f" for {self.id}, failed with error : {e}"))
+                msg = (
+                    f"Parsing styles file {file} for {self.id}, failed with error: {e}"
+                )
+                logger.warning(msg)
         else:
-            logger.warning(f"Could not find styles {file} for {self.id}")
+            logger.warning("Could not find styles %s for %s", file, self.id)
         return styles
-    
+
     def _parse_articles(self) -> tuple[list[dict], list[dict]]:
         """Parse the article and ad XML files for this issue.
 
-        Content elements are article parts, which are then grouped and 
+        Content elements are article parts, which are then grouped and
         combined to create each article.
 
         Returns:
             tuple[list[dict], list[dict]]: Parsed articles & content elements.
         """
         articles = []
         content_elements = []
         counter = 0
         # recompose each article by following the continuation links
         article_parts = []
         items = sorted(
             [
-            item
-            for item in self.archive.namelist()
-            if ".xml" in item and not item.startswith("._") and 
-                ("/Ar" in item or "/Ad" in item)
+                item
+                for item in self.archive.namelist()
+                if ".xml" in item
+                and not item.startswith("._")
+                and ("/Ar" in item or "/Ad" in item)
             ]
         )
-        
+
         while len(items) > 0:
             counter += 1
-            
+
             internal_deque = deque([items[0]])
             items = items[1:]
-            
+
             while len(internal_deque) > 0:
                 item = internal_deque.popleft()
                 try:
-                    xml_data = self.archive.read(item).decode('windows-1252')
+                    xml_data = self.archive.read(item).decode("windows-1252")
                     new_data = olive_parser(xml_data)
                 except Exception as e:
-                    logger.error(f'Parsing of {item} failed for {self.id}')
+                    logger.error("Parsing of %s failed for %s", item, self.id)
                     raise e
-                
+
                 # check if it needs to be parsed later on
-                if new_data["legacy"]['continuation_from'] is not None:
+                if new_data["legacy"]["continuation_from"] is not None:
                     target = new_data["legacy"]["continuation_from"]
                     target = [x for x in items if target in x]
                     if len(target) > 0:
                         items.append(item)
                         continue
-                
+
                 article_parts.append(new_data)
-                
-                if new_data["legacy"]['continuation_to'] is not None:
+
+                if new_data["legacy"]["continuation_to"] is not None:
                     next_id = new_data["legacy"]["continuation_to"]
                     next_id = [x for x in items if next_id in x][0]
                     internal_deque.append(next_id)
                     items.remove(next_id)
-            
+
             try:
                 content_elements += article_parts
                 combined_article = combine_article_parts(article_parts)
-                
+
                 if combined_article is not None:
                     articles.append(combined_article)
-                
+
                 article_parts = []
             except Exception as e:
                 raise e
         return articles, content_elements
-    
+
     def _get_image_info(self) -> dict[str, Any]:
         """Read `image-info.json` file for a given issue.
 
-        Go though all given image directories and only load the 
+        Go though all given image directories and only load the
         contents of the file corresponding to this issue.
 
         Raises:
             e: `image-info.json` file could not be decoded.
             ValueError: No `image-info.json` file was found
 
         Returns:
             dict[str, Any]: Contents of this issue's `image-info.json` file.
         """
         json_data = []
-        for im_dir in self.image_dirs.split(','):
+        for im_dir in self.image_dirs.split(","):
             issue_dir = os.path.join(
-                im_dir,
-                self.journal,
-                str(self.date).replace("-", "/"),
-                self.edition
+                im_dir, self.journal, str(self.date).replace("-", "/"), self.edition
+            )
+
+            issue_w_images = IssueDir(
+                journal=self.journal,
+                date=self.date,
+                edition=self.edition,
+                path=issue_dir,
             )
-            
-            issue_w_images = IssueDir(journal=self.journal, date=self.date, 
-                                      edition=self.edition, path=issue_dir)
-            
-            image_info_name = canonical_path(issue_w_images, name="image-info",
-                                             extension=".json")
-            
-            image_info_path = os.path.join(issue_w_images.path, 
-                                           image_info_name)
-            
+
+            image_info_name = canonical_path(
+                issue_w_images, name="image-info", extension=".json"
+            )
+
+            image_info_path = os.path.join(issue_w_images.path, image_info_name)
+
             if os.path.exists(image_info_path):
-                with open(image_info_path, 'r') as inp_file:
+                with open(image_info_path, "r") as inp_file:
                     try:
                         json_data = json.load(inp_file)
                         if len(json_data) == 0:
-                            logger.debug(f"Empty image info for {self.id}"
-                                         f"at {image_info_path}")
+                            msg = f"Empty image info for {self.id} at {image_info_path}"
+                            logger.debug(msg)
                         else:
                             return json_data
                     except Exception as e:
-                        logger.error(f"Decoding file {image_info_path}"
-                                     f"failed with '{e}'")
+                        logger.error(
+                            "Decoding file %s failed with '%s'", image_info_path, e
+                        )
                         raise e
         if len(json_data) == 0:
             raise ValueError(f"Could not find image info for {self.id}")
 
     def _find_pages(self) -> None:
         """Find page XML files and initialize page objects.
 
@@ -454,60 +457,59 @@
             ValueError: No page XML file was found.
         """
         if self.toc_data is not None:
             image_info = self._get_image_info()
             pages_xml = self._get_page_xml_files()
             for page_n, data in self.toc_data.items():
                 can_id = "{}-p{}".format(self.id, str(page_n).zfill(4))
-                image_info_records = [
-                    p for p in image_info
-                    if int(p['pg']) == page_n
-                ]
-                
+                image_info_records = [p for p in image_info if int(p["pg"]) == page_n]
+
                 if len(image_info_records) == 0:
                     image_info_record = None
                 else:
                     image_info_record = image_info_records[0]
-                
+
                 try:
                     page_xml = pages_xml[page_n]
-                except Exception:
-                    raise ValueError(f"Could not find page xml for {can_id}")
-                
+                except Exception as e:
+                    raise ValueError(f"Could not find page xml for {can_id}") from e
+
                 self._convert_images(image_info_record, page_n, page_xml)
-                
+
                 self.pages.append(
-                    OliveNewspaperPage(can_id, page_n, data,
-                                       image_info_record, page_xml)
+                    OliveNewspaperPage(
+                        can_id, page_n, data, image_info_record, page_xml
+                    )
                 )
-    
-    def _convert_images(self, image_info_record: dict[str, Any], 
-                        page_n: int, page_xml: dict[int, str]) -> None:
+
+    def _convert_images(
+        self, image_info_record: dict[str, Any], page_n: int, page_xml: dict[int, str]
+    ) -> None:
         """Convert a page's image information to canonical format.
 
         The coordinates are also converted to a iiif-compliant format.
 
         Args:
             image_info_record (dict[str, Any]): Page's images information.
             page_n (int): Corresponding page number.
             page_xml (dict[int, str]): Parsed contents of the page's XML.
         """
         if image_info_record is not None:
-            box_strategy = image_info_record['strat']
-            image_name = image_info_record['s']
+            box_strategy = image_info_record["strat"]
+            image_name = image_info_record["s"]
             images_in_page = [
                 content_item
                 for content_item in self.content_items
-                if content_item['m']['tp'] == "picture" and
-                    page_n in content_item['m']['pp']
+                if content_item["m"]["tp"] == "picture"
+                and page_n in content_item["m"]["pp"]
             ]
-            
+
             for image in images_in_page:
                 image = convert_image_coordinates(
                     image,
                     self.archive.read(page_xml),
                     image_name,
                     self.archive,
                     box_strategy,
-                    self.issuedir
+                    self.issuedir,
                 )
-                image['m']['tp'] = 'image'
+                image["m"]["tp"] = "image"
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/olive/detect.py` & `impresso_text_importer-1.1.0/text_importer/importers/olive/detect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 """This module contains functions to detect Olive OCR data to be imported.
 """
 
 import json
 from collections import namedtuple
 from typing import Any
 
-from impresso_commons.path.path_fs import (IssueDir, detect_issues,
-                                           select_issues)
+from impresso_commons.path.path_fs import IssueDir, detect_issues, select_issues
 
 from text_importer.utils import get_access_right
 
 OliveIssueDir = namedtuple(
-    "OliveIssueDirectory", [
-        'journal',
-        'date',
-        'edition',
-        'path',
-        'rights'
-    ]
+    "OliveIssueDirectory", ["journal", "date", "edition", "path", "rights"]
 )
 """A light-weight data structure to represent a newspaper issue.
 
 This named tuple contains basic metadata about a newspaper issue. They
 can then be used to locate the relevant data in the filesystem or to create
 canonical identifiers for the issue and its pages.
 
@@ -54,61 +47,52 @@
         issue_dir (IssueDir): Input ``IssueDir`` object.
         access_rights (dict[str, dict[str, str]]): Access rights information.
 
     Returns:
         OliveIssueDir: New ``OliveIssueDir`` object.
     """
     ar = get_access_right(issue_dir.journal, issue_dir.date, access_rights)
+
     return OliveIssueDir(
-        issue_dir.journal,
-        issue_dir.date,
-        issue_dir.edition,
-        issue_dir.path,
-        rights=ar
+        issue_dir.journal, issue_dir.date, issue_dir.edition, issue_dir.path, rights=ar
     )
 
 
 def olive_detect_issues(
     base_dir: str,
     access_rights: str,
     journal_filter: set | None = None,
-    exclude: bool = False
+    exclude: bool = False,
 ) -> list[OliveIssueDir]:
     """Detect newspaper issues to import within the filesystem.
 
     This function expects the directory structure that RERO used to
     organize the dump of Olive OCR data.
 
     Args:
         base_dir (str): Path to the base directory of newspaper data.
         access_rights (str): Path to ``access_rights.json`` file.
-        journal_filter (set | None, optional): IDs of newspapers to consider. 
+        journal_filter (set | None, optional): IDs of newspapers to consider.
             Defaults to None.
         exclude (bool, optional): Whether ``journal_filter`` should determine
             exclusion. Defaults to False.
 
     Returns:
         list[OliveIssueDir]: List of `OliveIssueDir` instances, to be imported.
     """
-    with open(access_rights, 'r') as f:
+    with open(access_rights, "r", encoding="utf-8") as f:
         access_rights_dict = json.load(f)
 
-    issues = detect_issues(
-        base_dir,
-        journal_filter=journal_filter,
-        exclude=exclude
-    )
+    issues = detect_issues(base_dir, journal_filter=journal_filter, exclude=exclude)
 
     return [dir2olivedir(x, access_rights_dict) for x in issues]
 
 
 def olive_select_issues(
-    base_dir: str,
-    config: dict[str, Any],
-    access_rights: str
+    base_dir: str, config: dict[str, Any], access_rights: str
 ) -> list[OliveIssueDir]:
     """Detect selectively newspaper issues to import.
 
     The behavior is very similar to :func:`olive_detect_issues` with the only
     difference that ``config`` specifies some rules to filter the data to
     import. See `this section <../importers.html#configuration-files>`__ for
     further details on how to configure filtering.
@@ -117,13 +101,13 @@
         base_dir (str): Path to the base directory of newspaper data.
         config (dict[str, Any]): Config dictionary for filtering.
         access_rights (str): Path to ``access_rights.json`` file.
 
     Returns:
         list[OliveIssueDir]: List of `OliveIssueDir` instances, to be imported.
     """
-    with open(access_rights, 'r') as f:
+    with open(access_rights, "r", encoding="utf-8") as f:
         access_rights_dict = json.load(f)
 
     issues = select_issues(config, base_dir)
 
     return [dir2olivedir(x, access_rights_dict) for x in issues]
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/olive/helpers.py` & `impresso_text_importer-1.1.0/text_importer/importers/olive/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,37 +31,37 @@
 
     Returns:
         dict[str, Any]: The new (merged) token.
     """
     merged_token = {
         "tx": "".join([token["tx"] for token in tokens]),
         "c": tokens[0]["c"][:2] + tokens[-1]["c"][2:],
-        "s": tokens[0]["s"]
+        "s": tokens[0]["s"],
     }
     logger.debug(
-        "(In-line pseudo tokens) Merged {} => {} in line \"{}\"".format(
-            "".join([t["tx"] for t in tokens]),
-            merged_token["tx"], 
-            line
-        )
+        '(In-line pseudo tokens) Merged %s => %s in line "%s"',
+        "".join([t["tx"] for t in tokens]),
+        merged_token["tx"],
+        line,
     )
+
     return merged_token
 
 
 def merge_pseudo_tokens(line: dict[str, list[Any]]) -> dict[str, list[Any]]:
     """Remove pseudo tokens from a line by merging them.
 
     Args:
         line (dict[str, list[Any]]): A line of OCR in JSON format.
 
     Returns:
         dict[str, list[Any]]: A new line object (with some merged tokens).
     """
     original_line = " ".join([t["tx"] for t in line["t"]])
-    qids = set([token["qid"] for token in line["t"] if "qid" in token])
+    qids = {token["qid"] for token in line["t"] if "qid" in token}
 
     inline_qids = []
 
     for qid in qids:
         tokens = [
             (i, token)
             for i, token in enumerate(line["t"])
@@ -78,18 +78,15 @@
         tokens = [
             (i, token)
             for i, token in enumerate(line["t"])
             if "qid" in token and token["qid"] == qid
         ]
 
         # remove tokens to merge from the line
-        tokens_to_merge = [
-            line["t"].pop(line["t"].index(token))
-            for i, token in tokens
-        ]
+        tokens_to_merge = [line["t"].pop(line["t"].index(token)) for i, token in tokens]
 
         if len(tokens_to_merge) >= 2:
             insertion_point = tokens[0][0]
             merged_token = merge_tokens(tokens_to_merge, original_line)
             line["t"].insert(insertion_point, merged_token)
 
     return line
@@ -111,104 +108,81 @@
             if token["tx"] == "-" and "nf" in token:
                 prev_token = line["t"][i - 1]
                 line["t"] = line["t"][:-2]
                 merged_token = {
                     "tx": "".join([prev_token["tx"], token["tx"]]),
                     "c": prev_token["c"][:2] + token["c"][2:],
                     "s": token["s"],
-                    "hy": token["hy"]
+                    "hy": token["hy"],
                 }
-                logger.debug(
-                    f"Merged {prev_token} and {token} => {merged_token}"
-                )
+                logger.debug("Merged %s and %s => %s", prev_token, token, merged_token)
                 line["t"].append(merged_token)
+
     return line
 
 
-def combine_article_parts(
-    article_parts: list[dict[str, Any]]
-) -> dict[str, Any]:
+def combine_article_parts(article_parts: list[dict[str, Any]]) -> dict[str, Any]:
     """Merge article parts into a single element.
 
     Olive format splits an article into multiple components whenever it spans
     over multiple pages. Thus, it is necessary to recompose multiple parts.
 
     Args:
         article_parts (list[dict[str, Any]]): One or more article parts.
 
     Returns:
         dict[str, Any]: Dict with keys `meta`, `fulltext`, `stats`,`legacy`.
     """
     if len(article_parts) > 1:
         # if an article has >1 part, retain the metadata
         # from the first item in the list
-        article_dict = {
-            "meta": {},
-            "fulltext": "",
-            "stats": {},
-            "legacy": {}
-        }
-        article_dict["legacy"]["id"] = [
-            ar["legacy"]["id"]
-            for ar in article_parts
-        ]
+        article_dict = {"meta": {}, "fulltext": "", "stats": {}, "legacy": {}}
+        article_dict["legacy"]["id"] = [ar["legacy"]["id"] for ar in article_parts]
         article_dict["legacy"]["source"] = [
-            ar["legacy"]["source"]
-            for ar in article_parts
+            ar["legacy"]["source"] for ar in article_parts
         ]
         article_dict["meta"]["type"] = {}
-        article_dict["meta"]["type"]["raw"] = (
-            article_parts[0]["meta"]["type"]["raw"]
-        )
+        article_dict["meta"]["type"]["raw"] = article_parts[0]["meta"]["type"]["raw"]
 
         article_dict["meta"]["title"] = article_parts[0]["meta"]["title"]
         article_dict["meta"]["page_no"] = [
-            int(n)
-            for ar in article_parts
-            for n in ar["meta"]["page_no"]
+            int(n) for ar in article_parts for n in ar["meta"]["page_no"]
         ]
 
         # TODO: remove from production
         if len(article_dict["meta"]["page_no"]) > 1:
             # pdb.set_trace()
             pass
 
         article_dict["meta"]["language"] = {}
         article_dict["meta"]["language"] = article_parts[0]["meta"]["language"]
-        article_dict["meta"]["issue_date"] = (
-            article_parts[0]["meta"]["issue_date"]
-        )
+        article_dict["meta"]["issue_date"] = article_parts[0]["meta"]["issue_date"]
     elif len(article_parts) == 1:
         article_dict = next(iter(article_parts))
     else:
         article_dict = None
+
     return article_dict
 
 
-def normalize_line(
-    line: dict[str, list[Any]], lang: str
-) -> dict[str, list[Any]]:
+def normalize_line(line: dict[str, list[Any]], lang: str) -> dict[str, list[Any]]:
     """Apply normalization rules to a line of OCR.
 
     The normalization rules that are applied depend on the language in which
     the text is written. This normalization is necessary because Olive, unlike
     e.g. Mets, does not encode explicitly the presence/absence of whitespaces.
 
     Args:
         line (dict[str, list[Any]]): A line of OCR text.
         lang (str): Language of the text.
 
     Returns:
         dict[str, list[Any]]: The new normalized line of text.
     """
-    mw_tokens = [
-        token
-        for token in line["t"]
-        if "qid" in token
-    ]
+    mw_tokens = [token for token in line["t"] if "qid" in token]
     # apply normalization only to those lines that contain at least one
     # multi-word token (denoted by presence of `qid` field)
     if len(mw_tokens) > 0:
         line = merge_pseudo_tokens(line)
         line = normalize_hyphenation(line)
 
     for i, token in enumerate(line["t"]):
@@ -216,70 +190,52 @@
             del token["nf"]
 
         if "qid" in token:
             del token["qid"]
 
         if i == 0 and i != len(line["t"]) - 1:
             insert_ws = insert_whitespace(
-                token["tx"],
-                line["t"][i + 1]["tx"],
-                None,
-                lang
+                token["tx"], line["t"][i + 1]["tx"], None, lang
             )
 
         elif i == 0 and i == len(line["t"]) - 1:
-            insert_ws = insert_whitespace(
-                token["tx"],
-                None,
-                None,
-                lang
-            )
+            insert_ws = insert_whitespace(token["tx"], None, None, lang)
 
         elif i == len(line["t"]) - 1:
             insert_ws = insert_whitespace(
-                token["tx"],
-                None,
-                line["t"][i - 1]["tx"],
-                lang
+                token["tx"], None, line["t"][i - 1]["tx"], lang
             )
 
         else:
             insert_ws = insert_whitespace(
-                token["tx"],
-                line["t"][i + 1]["tx"],
-                line["t"][i - 1]["tx"],
-                lang
+                token["tx"], line["t"][i + 1]["tx"], line["t"][i - 1]["tx"], lang
             )
         if not insert_ws:
             token["gn"] = True
 
     return line
 
 
 def keep_title(title: str) -> bool:
-    """Whether an element's title should be kept. 
+    """Whether an element's title should be kept.
 
-    The title should not be kept if it is one of "untitled article", 
+    The title should not be kept if it is one of "untitled article",
     "untitled ad", and "untitled picture".
 
     Args:
         title (str): Title to verify
 
     Returns:
         bool: False if given title is in the black list, True otherwise.
     """
-    black_list = [
-        "untitled article",
-        "untitled ad",
-        "untitled picture"
-    ]
+    black_list = ["untitled article", "untitled ad", "untitled picture"]
     if title.lower() in black_list:
         return False
-    else:
-        return True
+
+    return True
 
 
 def recompose_ToC(
     original_toc_data: dict[int, dict[str, dict]],
     articles: list[dict[str, Any]],
     images: list[dict[str, str]],
 ) -> list[dict[str, Any]]:
@@ -296,124 +252,123 @@
     Returns:
         list[dict[str, Any]]: List of final content items in the issue.
     """
     # Added deep copy because function changes toc_data
     toc_data = copy.deepcopy(original_toc_data)
     # concate content items from all pages into a single flat list
     content_items = [
-        toc_data[pn][elid]
-        for pn in toc_data.keys() for elid in toc_data[pn].keys()
+        toc_data[pn][elid] for pn in toc_data.keys() for elid in toc_data[pn].keys()
     ]
 
     # filter out those items that are part of a multipart article
     contents = []
-    sorted_content_items = sorted(content_items, key=itemgetter('seq'))
+    sorted_content_items = sorted(content_items, key=itemgetter("seq"))
     for item in sorted_content_items:
 
-        item['m'] = {}
+        item["m"] = {}
         item["l"] = {}
 
         if item["type"] == "Article" or item["type"] == "Ad":
 
             # find the corresponding item in `articles`
             # by using `legacy_id` as the search key
             # if not found (raises exception) means that it's one of the
             # multipart articles, and it's ok to skip it
-            legacy_id = item['legacy_id']
+            legacy_id = item["legacy_id"]
             article = None
             for ar in articles:
                 if isinstance(ar["legacy"]["id"], list):
                     if ar["legacy"]["id"][0] == legacy_id:
                         article = ar
                 else:
                     if ar["legacy"]["id"] == legacy_id:
                         article = ar
 
             try:
                 assert article is not None
             except Exception:
                 continue
 
-            item['m']["id"] = item["id"]
-            item['m']['pp'] = article["meta"]["page_no"]
-            item['m']['l'] = article["meta"]["language"]
-            item['m']['tp'] = article["meta"]["type"]["raw"].lower()
+            item["m"]["id"] = item["id"]
+            item["m"]["pp"] = article["meta"]["page_no"]
+            item["m"]["l"] = article["meta"]["language"]
+            item["m"]["tp"] = article["meta"]["type"]["raw"].lower()
 
             if keep_title(article["meta"]["title"]):
-                item['m']['t'] = article["meta"]["title"]
+                item["m"]["t"] = article["meta"]["title"]
 
             item["l"]["id"] = article["legacy"]["id"]
             item["l"]["source"] = article["legacy"]["source"]
 
         elif item["type"] == "Picture":
 
             # find in which page the image is
             page_no = [
                 page_no
                 for page_no in toc_data
-                if item['legacy_id'] in toc_data[page_no]
+                if item["legacy_id"] in toc_data[page_no]
             ]
 
             # get the new canonical id via the legacy id
-            item['m']['id'] = item['id']
-            item['m']['tp'] = item['type'].lower()
-            item['m']['pp'] = page_no
+            item["m"]["id"] = item["id"]
+            item["m"]["tp"] = item["type"].lower()
+            item["m"]["pp"] = page_no
 
             try:
-                image = [
-                    image
-                    for image in images
-                    if image['id'] == item['legacy_id']
-                ][0]
+                image = [image for image in images if image["id"] == item["legacy_id"]][
+                    0
+                ]
             except IndexError:
                 # if the image XML was faulty (e.g. because of missing
                 # coords, it won't find a corresping image item
-                logger.info(f"Image {item['legacy_id']} will be skipped")
+                logger.info("Image %s will be skipped", item["legacy_id"])
                 continue
 
             if keep_title(image["name"]):
-                item['m']['t'] = image["name"]
+                item["m"]["t"] = image["name"]
 
-            item['l']['id'] = item['legacy_id']
-            item['l']['res'] = image['resolution']
-            item['l']['path'] = image['filepath']
+            item["l"]["id"] = item["legacy_id"]
+            item["l"]["res"] = image["resolution"]
+            item["l"]["path"] = image["filepath"]
 
-            item['c'] = image['coords']
-            toc_item = toc_data[page_no[0]][item['legacy_id']]
+            item["c"] = image["coords"]
+            toc_item = toc_data[page_no[0]][item["legacy_id"]]
 
             if "embedded_into" in item:
-                cont_article_id = toc_item['embedded_into']
+                cont_article_id = toc_item["embedded_into"]
                 try:
                     containing_article = toc_data[page_no[0]][cont_article_id]
 
                     # content item entries exists in different shapes within
                     # the `toc_data` dict, depending on whether they have
                     # already been processed in this `for` loop or not
                     if (
-                        "m" in containing_article and
-                        len(containing_article['m'].keys()) > 0
+                        "m" in containing_article
+                        and len(containing_article["m"].keys()) > 0
                     ):
-                        item['pOf'] = containing_article['m']['id']
+                        item["pOf"] = containing_article["m"]["id"]
                     else:
-                        item['pOf'] = containing_article['id']
+                        item["pOf"] = containing_article["id"]
                 except Exception as e:
                     logger.error(
-                        f"Containing article for {item['m']['id']}"
-                        f" not found (error = {e})"
+                        "Containing article for %s not found (error = %s)",
+                        item["m"]["id"],
+                        e,
                     )
 
         # delete redundant fields
         if "embedded_into" in item:
-            del item['embedded_into']
-        del item['seq']
-        del item['legacy_id']
-        del item['type']
-        del item['id']
+            del item["embedded_into"]
+        del item["seq"]
+        del item["legacy_id"]
+        del item["type"]
+        del item["id"]
 
         contents.append(item)
+
     return contents
 
 
 def recompose_page(
     page_id: str,
     info_from_toc: dict[str, dict],
     page_elements: dict[str, dict],
@@ -432,55 +387,49 @@
         page_elements (dict[str, dict]): Page's articles or advertisements.
         clusters (dict[str, list[str]]): Inverted index of legacy ids; values
             are clusters of articles, each indexed by one member.
 
     Returns:
         dict[str, Any]: Page data according to impresso canonical format.
     """
-    page = {
-        "r": [],
-        "cdt": strftime("%Y-%m-%d %H:%M:%S")
-    }
-    ordered_elements = sorted(
-        list(info_from_toc.values()), key=itemgetter('seq')
-    )
+    page = {"r": [], "cdt": strftime("%Y-%m-%d %H:%M:%S")}
+    ordered_elements = sorted(list(info_from_toc.values()), key=itemgetter("seq"))
 
     id_mappings = {
-        legacy_id: info_from_toc[legacy_id]['id']
-        for legacy_id in info_from_toc
+        legacy_id: info_from_toc[legacy_id]["id"] for legacy_id in info_from_toc
     }
 
     # put together the regions while keeping the order in the page
     for el in ordered_elements:
 
         # keep only IDS of content items that are Ads or Articles
         # but escluding various other files in the archive
         if "Ar" not in el["legacy_id"] and "Ad" not in el["legacy_id"]:
             continue
 
         # this is to manage the situation of a multi-part article
         part_of = None
-        if el['legacy_id'] in clusters:
-            part_of = el['legacy_id']
+        if el["legacy_id"] in clusters:
+            part_of = el["legacy_id"]
         else:
             for key in clusters:
-                if el['legacy_id'] in clusters[key]:
+                if el["legacy_id"] in clusters[key]:
                     part_of = key
                     break
 
         if el["legacy_id"] in page_elements:
             element = page_elements[el["legacy_id"]]
         else:
             logger.error(
-                f"{el['id']}: {el['legacy_id']} not found in page {page_id}"
+                "%s: %s not found in page %s", el["id"], el["legacy_id"], page_id
             )
             continue
         mapped_id = id_mappings[part_of] if part_of in id_mappings else None
 
-        for i, region in enumerate(element["r"]):
+        for region in element["r"]:
             region["pOf"] = mapped_id
 
         page["r"] += element["r"]
 
     return page
 
 
@@ -493,88 +442,84 @@
 
     Returns:
         list[int]: Rescaled box coordinates.
     """
     box = " ".join([str(coord) for coord in coords])
     converted_box = compute_box(scale_factor, box)
     new_box = [int(c) for c in converted_box.split()]
-    logger.debug(f'Converted box coordinates: {box} => {converted_box}')
+    logger.debug("Converted box coordinates: %s => %s", box, converted_box)
+
     return new_box
 
 
 # TODO: move to the OliveNewspaperPage class as a method?
 # I cannot document using type info because of circular imports, which is a
 # sign that perhaps this function should rather be a method.
 def convert_page_coordinates(
     page: dict[str, Any],
     page_xml: str,
     page_image_name: str,
     zip_archive: ZipArchive,
     box_strategy: str,
-    issue: NewspaperIssue
+    issue: NewspaperIssue,
 ) -> bool:
     """Convert coordinates of all elements in a page that have coordinates.
 
     Note:
         This conversion is necessary since the coordinates recorded in the XML
-        file were computed on a different image than the one used for display 
+        file were computed on a different image than the one used for display
         in the impresso interface.
 
     Args:
         page (dict[str, Any]): Page data where coordinates should be converted.
         page_xml (str): Content of Olive page XML.
         page_image_name (str): Name of page image file.
         zip_archive (ZipArchive): Olive Zip archive.
         box_strategy (str): Conversion strategy to apply.
         issue (NewspaperIssue): Newspaper issue the page belongs to.
 
     Returns:
         bool: Whether the coordinate conversion was successful or not.
     """
-    start_t = time.clock()
+    start_t = time.time()
     scale_factor = get_scale_factor(
-        issue.path,
-        zip_archive,
-        page_xml,
-        box_strategy,
-        page_image_name
+        issue.path, zip_archive, page_xml, box_strategy, page_image_name
     )
     if scale_factor is not None:
-        for region in page['r']:
-            region['c'] = convert_box(region['c'], scale_factor)
-            for paragraph in region['p']:
-                for line in paragraph['l']:
-                    line['c'] = convert_box(line['c'], scale_factor)
-                    for token in line['t']:
-                        token['c'] = convert_box(token['c'], scale_factor)
-        end_t = time.clock()
+        for region in page["r"]:
+            region["c"] = convert_box(region["c"], scale_factor)
+            for paragraph in region["p"]:
+                for line in paragraph["l"]:
+                    line["c"] = convert_box(line["c"], scale_factor)
+                    for token in line["t"]:
+                        token["c"] = convert_box(token["c"], scale_factor)
+        end_t = time.time()
         t = end_t - start_t
         logger.debug(
-            f"Converted coordinates {page_image_name}"
-            f" in {issue.id} (took {t}s)"
+            "Converted coordinates %s in %s (took %ss)", page_image_name, issue.id, t
         )
         return True
-    else:
-        logger.info(f"Could not find scale factor for {page['id']}")
-        return False
+
+    logger.info("Could not find scale factor for %s", page["id"])
+    return False
 
 
 def convert_image_coordinates(
     image: dict[str, Any],
     page_xml: str,
     page_image_name: str,
     zip_archive: ZipArchive,
     box_strategy: str,
-    issue: IssueDir
+    issue: IssueDir,
 ) -> dict[str, Any]:
     """Convert coordinates of an Olive image element.
 
     Note:
         This conversion is necessary since the coordinates recorded in the XML
-        file were computed on a different image than the one used for display 
+        file were computed on a different image than the one used for display
         in the impresso interface.
 
     Args:
         image (dict[str, Any]): Image metadata.
         page_xml (str): Content of Olive page XML.
         page_image_name (str): Name of page image file.
         zip_archive (ZipArchive): Olive Zip archive.
@@ -582,42 +527,35 @@
         issue (IssueDir): IssueDie of the newspaper issue the page belongs to.
 
     Returns:
         dict[str, Any]: Updated image metadata based on the conversion.
     """
     try:
         scale_factor = get_scale_factor(
-            issue.path,
-            zip_archive,
-            page_xml,
-            box_strategy,
-            page_image_name
+            issue.path, zip_archive, page_xml, box_strategy, page_image_name
         )
-        image['c'] = convert_box(image['c'], scale_factor)
-        image['cc'] = True
+        image["c"] = convert_box(image["c"], scale_factor)
+        image["cc"] = True
     except Exception:
-        image['cc'] = False
+        image["cc"] = False
 
     return image
 
 
 def normalize_language(language: str) -> str:
     """Normalize the language's string representation.
 
     Args:
         language (str): Language to normalize.
 
     Returns:
         str: Normalized language, one of "fr", "en" and "de".
     """
-    mappings = {
-        "french": "fr",
-        "english": "en",
-        "german": "de"
-    }
+    mappings = {"french": "fr", "english": "en", "german": "de"}
+
     return mappings[language.lower()]
 
 
 def get_clusters(articles: list[dict[str, Any]]) -> dict[str, list[str]]:
     """Created inverted index of legacy ids to article clusters.
 
     Each cluster of articles is indexed by the legacy id of one its members.
@@ -632,8 +570,9 @@
     clusters = {}
     for ar in articles:
         legacy_id = ar["legacy"]["id"]
         if isinstance(legacy_id, list):
             clusters[legacy_id[0]] = legacy_id
         else:
             clusters[legacy_id] = [legacy_id]
+
     return clusters
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/olive/parsers.py` & `impresso_text_importer-1.1.0/text_importer/importers/olive/parsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import copy
 import re
 from typing import Any
 
 from bs4 import BeautifulSoup
 from impresso_commons.path.path_fs import canonical_path, IssueDir
 
-from text_importer.importers.olive.helpers import (normalize_language,
-                                                   normalize_line)
+from text_importer.importers.olive.helpers import normalize_language, normalize_line
 
 
 def parse_styles(text: str) -> list[dict[str, Any]]:
     """Turn Olive `styleGallery.txt` file into a dictionary.
 
     Style IDs may be referred to within the ``s`` property of token elements
     as defined in the impresso JSON schema for newspaper pages (see
@@ -32,21 +31,20 @@
     for line in text.split("\r\n"):
         if line == "":
             continue
 
         n, font, font_size, color = re.match(regex, line).groups()
         styles.append(
             {
-            "id": int(n),
-            "f": font.replace('"', ""),
-            "fs": float(font_size),
-            "rgb": [
-                int(i)
-                for i in color.replace("(", "").replace(")", "").split(",")
-            ]
+                "id": int(n),
+                "f": font.replace('"', ""),
+                "fs": float(font_size),
+                "rgb": [
+                    int(i) for i in color.replace("(", "").replace(")", "").split(",")
+                ],
             }
         )
 
     return styles
 
 
 def olive_image_parser(text: bytes) -> dict[str, str | list] | None:
@@ -60,154 +58,135 @@
     """
     soup = BeautifulSoup(text, "lxml")
     root = soup.find("xmd-entity")
 
     try:
         assert root is not None
         img = {
-            'id': root.get('id'),
-            'coords': root.img.get('box').split(),
-            'name': root.meta.get('name'),
-            'resolution': root.meta.get('images_resolution'),
-            'filepath': root.img.get('href')
+            "id": root.get("id"),
+            "coords": root.img.get("box").split(),
+            "name": root.meta.get("name"),
+            "resolution": root.meta.get("images_resolution"),
+            "filepath": root.img.get("href"),
         }
         return img
     except AssertionError:
         return None
 
 
 def olive_toc_parser(
-    toc_path: str, 
-    issue_dir: IssueDir, 
-    encoding: str = "windows-1252"
+    toc_path: str, issue_dir: IssueDir, encoding: str = "windows-1252"
 ) -> dict[int, dict[str, dict]]:
     """Parse the TOC.xml file (Olive format).
 
     For each page, the a dict containing page data is created; mapping content
-    item legacy IDs to their metadata. 
+    item legacy IDs to their metadata.
 
     Args:
         toc_path (str): Path to the ToC XML file.
         issue_dir (IssueDir): Corresponding ``IssueDir`` object.
         encoding (str, optional): File's encoding. Defaults to "windows-1252".
 
     Returns:
         dict[int, dict[str, dict]]: Dictionary where keys are page numbers and
             values the corresponding page data dictionary.
     """
-    with codecs.open(toc_path, 'r', encoding) as f:
+    with codecs.open(toc_path, "r", encoding) as f:
         text = f.read()
 
     toc_data = {}
 
     global_counter = 0
 
-    for page in BeautifulSoup(text, 'lxml').find_all('page'):
+    for page in BeautifulSoup(text, "lxml").find_all("page"):
         page_data = {}
 
         for n, entity in enumerate(page.find_all("entity")):
 
             global_counter += 1
             item_legacy_id = entity.get("id")
 
             item = {
                 "legacy_id": item_legacy_id,
                 "id": canonical_path(
-                        issue_dir,
-                        name=f"i{str(global_counter).zfill(4)}",
-                        extension=""
-                        ),
+                    issue_dir, name=f"i{str(global_counter).zfill(4)}", extension=""
+                ),
                 "type": entity.get("entity_type"),
-                "seq": n + 1
+                "seq": n + 1,
             }
 
             # if it's a picture we want to get also the article into which
             # the image is embedded
-            if item['type'].lower() == "picture":
+            if item["type"].lower() == "picture":
                 if entity.get("embedded_into") is not None:
-                    item['embedded_into'] = entity.get("embedded_into")
+                    item["embedded_into"] = entity.get("embedded_into")
 
             page_data[item_legacy_id] = item
 
-        toc_data[int(page.get('page_no'))] = page_data
+        toc_data[int(page.get("page_no"))] = page_data
 
     # gather the IDs of all content items int the issue
-    ids = [
-        toc_data[page][item]["id"]
-        for page in toc_data
-        for item in toc_data[page]
-    ]
+    ids = [toc_data[page][item]["id"] for page in toc_data for item in toc_data[page]]
 
     # check that these IDs are unique within the issue
     assert len(ids) == len(list(set(ids)))
 
     return toc_data
 
 
 def olive_parser(text: str) -> dict[str, dict | list]:
     """Parse an Olive XML file (e.g. from Le Temps corpus).
 
     The main logic implemented here was derived from
     <https://github.com/dhlab-epfl/LeTemps-preprocessing/>. Each XML file
     corresponds to one article, as detected by Olive.
-    The final dictionary has keys ``meta``, ``r``, ``stats`` and ``legacy``, 
+    The final dictionary has keys ``meta``, ``r``, ``stats`` and ``legacy``,
     each mapping to dictionaries or lists with the file's parsed contents.
 
     Args:
         text (str): Contents of the xml file to parse.
 
     Returns:
         dict[str, dict | list]: Dictionary with parsed contents.
     """
     soup = BeautifulSoup(text, "lxml")
     root = soup.find("xmd-entity")
-    page_no = root['page_no']
-    identifier = root['id']
-    language = root['language']
-    title = soup.meta['name']
-    entity_type = root['entity_type']
-    issue_date = soup.meta['issue_date']
+    page_no = root["page_no"]
+    identifier = root["id"]
+    language = root["language"]
+    title = soup.meta["name"]
+    entity_type = root["entity_type"]
+    issue_date = soup.meta["issue_date"]
 
     out = {
         "meta": {"language": None, "type": {}},
         "r": [],
         "stats": {},
         "legacy": {"continuation_from": None, "continuation_to": None},
     }
     out["meta"]["title"] = title
     out["meta"]["page_no"] = [int(page_no)]
     out["meta"]["language"] = normalize_language(language)
     out["meta"]["type"]["raw"] = entity_type
     out["meta"]["issue_date"] = issue_date
 
-    new_region = {
-        "c": [],
-        "p": []
-    }
+    new_region = {"c": [], "p": []}
 
-    new_paragraph = {
-        "l": []
-    }
+    new_paragraph = {"l": []}
 
-    new_line = {
-        "c": [],
-        "t": []
-    }
+    new_line = {"c": [], "t": []}
 
-    new_token = {
-        "c": [],
-        "tx": ""
-    }
+    new_token = {"c": [], "tx": ""}
 
     for primitive in soup.find_all("primitive"):
 
         # store coordinate of text areas (boxes) by page
         # 1) page number, 2) coordinate list
         region = copy.deepcopy(new_region)
-        region["c"] = [int(i) for i in primitive.get('box').split(" ")]
+        region["c"] = [int(i) for i in primitive.get("box").split(" ")]
 
         para = None
         line = None
         line_counter = 0
 
         for tag in primitive.find_all(recursive=False):
 
@@ -222,29 +201,29 @@
                     para["l"].append(line)
 
                 if tag.get("p") in ["S", "SA"] and line_counter > 0:
                     region["p"].append(para)
                     para = copy.deepcopy(new_paragraph)
 
                 line = copy.deepcopy(new_line)
-                line["c"] = [int(i) for i in tag.get('box').split(" ")]
+                line["c"] = [int(i) for i in tag.get("box").split(" ")]
                 line_counter += 1
 
             if tag.name in ["w", "q"]:
 
                 # store coordinates of each token
                 # 1) token, 2) page number, 3) coordinate list
                 t = copy.deepcopy(new_token)
-                t["c"] = [int(i) for i in tag.get('box').split(" ")]
+                t["c"] = [int(i) for i in tag.get("box").split(" ")]
                 t["tx"] = tag.string
-                t["s"] = int(tag.get('style_ref'))
+                t["s"] = int(tag.get("style_ref"))
 
-                if tag.name == "q" and tag.get('qid') is not None:
-                    qid = tag.get('qid')
-                    normalized_form = soup.find('qw', qid=qid).text
+                if tag.name == "q" and tag.get("qid") is not None:
+                    qid = tag.get("qid")
+                    normalized_form = soup.find("qw", qid=qid).text
                     t["nf"] = normalized_form
                     t["qid"] = qid
 
                 # append the token to the line
                 line["t"].append(t)
 
         # append orphan lines
@@ -254,20 +233,20 @@
 
         region["p"].append(para)
 
         if para is not None:
             out["r"].append(region)
 
     out["legacy"]["id"] = identifier
-    out["legacy"]["source"] = soup.link['source']
-    out["legacy"]["first_id"] = soup.link['first_id']
-    out["legacy"]["last_id"] = soup.link['last_id']
-    out["legacy"]["next_id"] = soup.link['next_id']
-    out["legacy"]["prev_id"] = soup.link['prev_id']
+    out["legacy"]["source"] = soup.link["source"]
+    out["legacy"]["first_id"] = soup.link["first_id"]
+    out["legacy"]["last_id"] = soup.link["last_id"]
+    out["legacy"]["next_id"] = soup.link["next_id"]
+    out["legacy"]["prev_id"] = soup.link["prev_id"]
 
-    if root.has_attr('continuation_from'):
-        out["legacy"]["continuation_from"] = root['continuation_from']
+    if root.has_attr("continuation_from"):
+        out["legacy"]["continuation_from"] = root["continuation_from"]
 
-    if root.has_attr('continuation_to'):
-        out["legacy"]["continuation_to"] = root['continuation_to']
+    if root.has_attr("continuation_to"):
+        out["legacy"]["continuation_to"] = root["continuation_to"]
 
     return out
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/onb_annop/detect.py` & `impresso_text_importer-1.1.0/text_importer/importers/onb_annop/detect.py`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/rero/detect.py` & `impresso_text_importer-1.1.0/text_importer/importers/rero/detect.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,30 +10,18 @@
 from dask import bag as db
 from impresso_commons.path.path_fs import _apply_datefilter
 
 from text_importer.utils import get_access_right
 
 logger = logging.getLogger(__name__)
 
-EDITIONS_MAPPINGS = {
-    1: 'a',
-    2: 'b',
-    3: 'c',
-    4: 'd',
-    5: 'e'
-}
+EDITIONS_MAPPINGS = {1: "a", 2: "b", 3: "c", 4: "d", 5: "e"}
 
 Rero2IssueDir = namedtuple(
-    "IssueDirectory", [
-        'journal',
-        'date',
-        'edition',
-        'path',
-        'rights'
-    ]
+    "IssueDirectory", ["journal", "date", "edition", "path", "rights"]
 )
 """A light-weight data structure to represent a newspaper issue.
 
 This named tuple contains basic metadata about a newspaper issue. They
 can then be used to locate the relevant data in the filesystem or to create
 canonical identifiers for the issue and its pages.
 
@@ -60,75 +48,80 @@
     Args:
         path (str): Path of issue.
         access_rights (dict): dictionary for access rights.
 
     Returns:
         Rero2IssueDir: New `Rero2IssueDir` object matching the path and rights.
     """
-    journal, issue = path.split('/')[-2:]
-    date, edition = issue.split('_')[:2]
-    date = datetime.strptime(date, '%Y%m%d').date()
+    journal, issue = path.split("/")[-2:]
+    date, edition = issue.split("_")[:2]
+    date = datetime.strptime(date, "%Y%m%d").date()
 
     edition = EDITIONS_MAPPINGS[int(edition)]
 
-    return Rero2IssueDir(journal=journal, date=date,
-                         edition=edition, path=path,
-                         rights=get_access_right(journal, date, access_rights))
+    return Rero2IssueDir(
+        journal=journal,
+        date=date,
+        edition=edition,
+        path=path,
+        rights=get_access_right(journal, date, access_rights),
+    )
 
 
 def detect_issues(
-    base_dir: str, access_rights: str, data_dir: str = 'data'
+    base_dir: str, access_rights: str, data_dir: str = "data"
 ) -> list[Rero2IssueDir]:
     """Detect newspaper issues to import within the filesystem.
 
     This function expects the directory structure that RERO used to
     organize the dump of Mets/Alto OCR data.
 
     TODO: add info on the file structure.
 
     Args:
         base_dir (str): Path to the base directory of newspaper data.
         access_rights (str): Path to ``access_rights.json`` file.
-        data_dir (str, optional): Directory where data is stored 
+        data_dir (str, optional): Directory where data is stored
             (usually `data/`). Defaults to 'data'.
 
     Returns:
         list[Rero2IssueDir]: list of `Rero2IssueDir` instances, to be imported.
     """
-    dir_path, dirs, files = next(os.walk(base_dir))
+    dir_path, dirs, _ = next(os.walk(base_dir))
     journal_dirs = [os.path.join(dir_path, _dir) for _dir in dirs]
     journal_dirs = [
         os.path.join(journal, _dir, _dir2)
         for journal in journal_dirs
         for _dir in os.listdir(journal)
         if _dir == data_dir
         for _dir2 in os.listdir(os.path.join(journal, _dir))
     ]
 
     issues_dirs = [
-        os.path.join(j_dir, l) 
-        for j_dir in journal_dirs 
+        os.path.join(j_dir, l)
+        for j_dir in journal_dirs
         for l in os.listdir(j_dir)
-        if '.DS_Store' not in l
+        if ".DS_Store" not in l
     ]
 
-    with open(access_rights, 'r') as f:
+    with open(access_rights, "r", encoding="utf-8") as f:
         access_rights_dict = json.load(f)
 
     return [dir2issue(_dir, access_rights_dict) for _dir in issues_dirs]
 
+
 def select_issues(
     base_dir: str, config: dict, access_rights: str
 ) -> list[Rero2IssueDir] | None:
     """Detect selectively newspaper issues to import.
 
     The behavior is very similar to :func:`detect_issues` with the only
     difference that ``config`` specifies some rules to filter the data to
     import. See `this section <../importers.html#configuration-files>`__ for
-    further details on how to configure filtering. 
+    further details on how to configure filtering.
 
     Args:
         base_dir (str): Path to the base directory of newspaper data.
         config (dict): Config dictionary for filtering.
         access_rights (str): Path to ``access_rights.json`` file.
 
     Returns:
@@ -137,33 +130,33 @@
     # read filters from json configuration (see config.example.json)
     try:
         filter_dict = config["newspapers"]
         exclude_list = config["exclude_newspapers"]
         year_flag = config["year_only"]
 
     except KeyError:
-        logger.critical(f"The key [newspapers|exclude_newspapers|year_only] "
-               "is missing in the config file.")
+        logger.critical(
+            "The key [newspapers|exclude_newspapers|year_only] "
+            "is missing in the config file."
+        )
         return
 
     issues = detect_issues(base_dir, access_rights)
     issue_bag = db.from_sequence(issues)
-    selected_issues = (
-        issue_bag.filter(
-            lambda i: (
-                len(filter_dict) == 0 or i.journal in filter_dict.keys()
-                ) and i.journal not in exclude_list
-        ).compute()
-    )
+    selected_issues = issue_bag.filter(
+        lambda i: (len(filter_dict) == 0 or i.journal in filter_dict.keys())
+        and i.journal not in exclude_list
+    ).compute()
 
     exclude_flag = False if not exclude_list else True
-    filtered_issues = _apply_datefilter(
-        filter_dict, selected_issues, year_only=year_flag
-    ) if not exclude_flag else selected_issues
+    filtered_issues = (
+        _apply_datefilter(filter_dict, selected_issues, year_only=year_flag)
+        if not exclude_flag
+        else selected_issues
+    )
 
     logger.info(
-        "{} newspaper issues remained after applying filter: {}".format(
-            len(filtered_issues),
-            filtered_issues
-        )
+        "%s newspaper issues remained after applying filter: %s",
+        len(filtered_issues),
+        filtered_issues,
     )
     return filtered_issues
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/swa/classes.py` & `impresso_text_importer-1.1.0/text_importer/importers/swa/classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,102 +12,102 @@
 
 from text_importer.importers.classes import NewspaperIssue, ZipArchive
 from text_importer.importers.mets_alto.alto import parse_printspace
 from text_importer.importers.mets_alto.classes import MetsAltoNewspaperPage
 from text_importer.importers.swa.detect import SwaIssueDir
 
 logger = logging.getLogger(__name__)
-IIIF_ENDPOINT_URL = "https://ub-sipi.ub.unibas.ch/impresso"
+IIIF_IMG_BASE_URI = "https://ub-sipi.ub.unibas.ch/impresso"
+IIIF_PRES_BASE_URI = "https://ub-iiifpresentation.ub.unibas.ch/impresso_sb"
+IIIF_MANIFEST_SUFFIX = "manifest"
 SWA_XML_ENCODING = "utf-8-sig"
 
 
 class SWANewspaperPage(MetsAltoNewspaperPage):
     """Newspaper page in SWA (Mets/Alto) format.
 
     Args:
         _id (str): Canonical page ID.
         number (int): Page number.
         alto_path (str): Full path to the Alto XML file.
-    
+
     Attributes:
         id (str): Canonical Page ID (e.g. ``GDL-1900-01-02-a-p0004``).
         number (int): Page number.
         page_data (dict[str, Any]): Page data according to canonical format.
         issue (NewspaperIssue): Issue this page is from.
         filename (str): Name of the Alto XML page file.
         basedir (str): Base directory where Alto files are located.
         encoding (str, optional): Encoding of XML file.
         iiif (str): The iiif URI to the newspaper page image.
     """
-    
+
     def __init__(self, _id: str, number: int, alto_path: str) -> None:
         self.alto_path = alto_path
         basedir, filename = os.path.split(alto_path)
-        super().__init__(_id, number, filename, basedir, 
-                         encoding=SWA_XML_ENCODING)
-        self.iiif = os.path.join(IIIF_ENDPOINT_URL, filename.split('.')[0])
-        self.page_data['iiif'] = self.iiif
-    
+        super().__init__(_id, number, filename, basedir, encoding=SWA_XML_ENCODING)
+        self.iiif = os.path.join(IIIF_IMG_BASE_URI, filename.split(".")[0])
+        self.page_data["iiif_img_base_uri"] = self.iiif
+
     def add_issue(self, issue: NewspaperIssue) -> None:
         self.issue = issue
- 
+
     @property
     def ci_id(self) -> str:
         """Return the content item ID of the page.
 
         Given that SWA data do not entail article-level segmentation,
         each page is considered as a content item. Thus, to mint the content
         item ID we take the canonical page ID and simply replace the "p"
         prefix with "i".
 
         Returns:
             str: Content item id.
         """
-        split = self.id.split('-')
-        split[-1] = split[-1].replace('p', 'i')
+        split = self.id.split("-")
+        split[-1] = split[-1].replace("p", "i")
         return "-".join(split)
-    
+
     @property
     def file_exists(self) -> bool:
         """Check whether the Alto XML file exists for this page.
 
         Returns:
             bool: True if the Alto XML file exists, False otherwise.
         """
-        return (os.path.exists(self.alto_path) and 
-                os.path.isfile(self.alto_path))
-    
+        return os.path.exists(self.alto_path) and os.path.isfile(self.alto_path)
+
     def parse(self) -> None:
         doc = self.xml
-        pselement = doc.find('PrintSpace')
+        pselement = doc.find("PrintSpace")
         ci_id = self.ci_id
-        
-        mappings = {k.get('ID'): ci_id for k in pselement.findAll('TextBlock')}
+
+        mappings = {k.get("ID"): ci_id for k in pselement.findAll("TextBlock")}
         page_data, notes = parse_printspace(pselement, mappings)
-        
-        self.page_data['cc'], self.page_data['r'] = True, page_data
-        
+
+        self.page_data["cc"], self.page_data["r"] = True, page_data
+
         # Add notes to page data
         if len(notes) > 0:
-            self.page_data['n'] = notes
+            self.page_data["n"] = notes
         return notes
-    
+
     def get_iiif_image(self) -> str:
         """Create the iiif URI to the full journal page image.
 
         Returns:
             str: iiif URI of the image of the full page.
         """
         return os.path.join(self.iiif, "full/full/0/default.jpg")
 
 
 class SWANewspaperIssue(NewspaperIssue):
     """Newspaper issue in SWA Mets/Alto format.
 
-    Note: 
+    Note:
         SWA is in ALTO format, but there isn't any Mets file. So in that case,
         issues are simply a collection of pages.
 
     Args:
         issue_dir (SwaIssueDir): Identifying information about the issue.
         temp_dir (str): Temporary directory to extract archives.
 
@@ -124,34 +124,39 @@
             issue's pages.
         temp_pages (list[tuple[str, str]]): Temporary list of pages found for
             this issue. A page is a tuple (page_canonical_id, alto_path), where
             alto_path is the path from within the archive.
         content_items (list[dict[str,Any]]): Content items from this issue.
         notes (list[str]): Notes of missing pages gathered while parsing.
     """
-    
+
     def __init__(self, issue_dir: SwaIssueDir, temp_dir: str) -> None:
         super().__init__(issue_dir)
         self.archive = self._parse_archive(temp_dir)
         self.temp_pages = issue_dir.pages
         self.content_items = []
-        
+
         self._notes = []
         self._find_pages()
         self._find_content_items()
-        
+
+        iiif_manifest = os.path.join(
+            IIIF_PRES_BASE_URI, f"{self.id}-issue", IIIF_MANIFEST_SUFFIX
+        )
+
         self.issue_data = {
-            'id': self.id,
-            'cdt': strftime("%Y-%m-%d %H:%M:%S"),
-            'i': self.content_items,
-            'ar': self.rights,
-            'pp': [p.id for p in self.pages],
-            'notes': self._notes
-            }
-    
+            "id": self.id,
+            "cdt": strftime("%Y-%m-%d %H:%M:%S"),
+            "i": self.content_items,
+            "ar": self.rights,
+            "pp": [p.id for p in self.pages],
+            "iiif_manifest_uri": iiif_manifest,
+            "notes": self._notes,
+        }
+
     def _parse_archive(self, temp_dir: str) -> ZipArchive:
         """Open and parse the Zip archive located at :attr:`path` if possible.
 
         Args:
             temp_dir (str): Temporary directory in which to unpack the archive.
 
         Raises:
@@ -161,56 +166,56 @@
         Returns:
             ZipArchive: Archive containing the pages XML files for the issue.
         """
         if os.path.isfile(self.path):
             try:
                 archive = ZipFile(self.path)
                 logger.debug(
-                        f"Contents of archive for {self.id}: {archive.namelist()}"
-                        )
+                    "Contents of archive for %s: %s", self.id, archive.namelist()
+                )
                 return ZipArchive(archive, temp_dir)
             except Exception as e:
                 msg = f"Bad Zipfile for {self.id}, failed with error : {e}"
                 raise ValueError(msg)
         else:
             msg = f"Could not find archive {self.path} for {self.id}"
             raise ValueError(msg)
-    
+
     def _find_pages(self) -> None:
         """Detect and create the issue pages using the relevant Alto XML files.
 
         Created :obj:`SWANewspaperPage` instances are added to :attr:`pages`.
 
         Raises:
             ValueError: No page was found for this issue..
         """
         for n, val in enumerate(sorted(self.temp_pages)):
             page_id, page_path = val
             page_path = os.path.join(self.archive.dir, page_path)
             page = SWANewspaperPage(page_id, n + 1, page_path)
-            
+
             # Check page existence
             if not page.file_exists:
                 self._notes.append(f"Alto file for {page_id} missing {page_path}")
             else:
                 self.pages.append(page)
-            
+
         if len(self.pages) == 0:
             raise ValueError(f"Could not find any page for {self.id}")
-    
+
     def _find_content_items(self) -> None:
         """Create content items for the pages in this issue.
 
         Given that SWA data do not entail article-level segmentation,
         each page is considered as a content item.
         """
         for page in sorted(self.pages, key=lambda x: x.id):
             page_number = page.number
-            ci_id = self.id + '-i' + str(page_number).zfill(4)
+            ci_id = self.id + "-i" + str(page_number).zfill(4)
             ci = {
-                'm': {
-                    'id': ci_id,
-                    'pp': [page_number],
-                    'tp': 'page',
-                    }
+                "m": {
+                    "id": ci_id,
+                    "pp": [page_number],
+                    "tp": "page",
                 }
+            }
             self.content_items.append(ci)
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/tetml/classes.py` & `impresso_text_importer-1.1.0/text_importer/importers/tetml/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Classes to handle the TETML OCR format."""
 
+import os
 import logging
 from pathlib import Path
 from time import strftime
 
 from impresso_commons.path import IssueDir
 from impresso_commons.path.path_fs import canonical_path
 
 from text_importer.importers.classes import NewspaperIssue, NewspaperPage
 from text_importer.importers.tetml.parsers import tetml_parser
 
 logger = logging.getLogger(__name__)
 
+IIIF_ENDPOINT_URI = "https://impresso-project.ch/api/proxy/iiif/"
+
 
 class TetmlNewspaperPage(NewspaperPage):
     """Generic class representing a page in Tetml format.
 
     :param int number: Page number.
     :param dict page_content: Nested article content of a single page
     :param str page_xml: Path to the Tetml file of the page.
@@ -30,19 +33,20 @@
 
     def parse(self):
 
         self.page_data = {
             "id": self.id,
             "cdt": strftime("%Y-%m-%d %H:%M:%S"),
             "cc": True,
+            "iiif_img_base_uri": os.path.join(IIIF_ENDPOINT_URI, self.id),
             "r": self.page_content["r"],
         }
 
         if not self.page_data["r"]:
-            logger.warning(f"Page {self.id} has no OCR text")
+            logger.warning("Page %s has no OCR text", self.id)
 
     def add_issue(self, issue: NewspaperIssue):
         if issue is None:
             raise ValueError(f"No NewspaperIssue for {self.id}")
 
         self.issue = issue
 
@@ -59,38 +63,40 @@
     :param IssueDir issue_dir: Newspaper issue with relevant information.
 
     """
 
     def __init__(self, issue_dir: IssueDir):
         super().__init__(issue_dir)
 
-        logger.info(f"Starting to parse {self.id}")
+        logger.info("Starting to parse %s", self.id)
 
         # get all tetml files of this issue
         self.files = self._index_issue_files()
 
         # parse the indexed files
         self.article_data = self.parse_articles()
 
         # using canonical ('m') and additional non-canonical ('meta') metadata
-        self.content_items = [{"m": art["m"], "meta": art["meta"]} for art in self.article_data]
+        self.content_items = [
+            {"m": art["m"], "meta": art["meta"]} for art in self.article_data
+        ]
 
         # instantiate the individual pages
         self._find_pages()
 
         self.issue_data = {
             "id": self.id,
             "cdt": strftime("%Y-%m-%d %H:%M:%S"),
             "s": None,  # TODO: ignore style for the time being
             "i": self.content_items,
             "pp": [p.id for p in self.pages],
             "ar": self.rights,
         }
 
-        logger.info(f"Finished parsing {self.id}")
+        logger.info("Finished parsing %s", self.id)
 
     def _index_issue_files(self, suffix=".tetml"):
         """
         Index all files with a tetml suffix in the current issue directory
         """
 
         return sorted([str(path) for path in Path(self.path).rglob("*" + suffix)])
@@ -103,15 +109,17 @@
         articles = []
         current_issue_page = 1  # start page of next article
         for i, fname in enumerate(self.files):
             try:
                 data = tetml_parser(fname)
 
                 # canonical identifier
-                data["m"]["id"] = canonical_path(self.issuedir, name=f"i{i+1:04}", extension="")
+                data["m"]["id"] = canonical_path(
+                    self.issuedir, name=f"i{i+1:04}", extension=""
+                )
 
                 # reference to content item per region
                 for page in data["pages"]:
                     for reg in page["r"]:
                         reg["pOf"] = data["m"]["id"]
 
                 data["m"]["tp"] = "article"  # type attribute
@@ -120,15 +128,15 @@
                 page_end = current_issue_page + data["meta"]["npages"]
                 data["m"]["pp"] = list(range(current_issue_page, page_end))
                 current_issue_page = page_end
 
                 articles.append(data)
 
             except Exception as e:
-                logger.error(f"Parsing of {fname} failed for {self.id}")
+                logger.error("Parsing of %s failed for %s", fname, self.id)
                 raise e
 
         return articles
 
     def _find_pages(self):
         """
         Initialize all page objects per issue assuming that a particular page
@@ -137,9 +145,11 @@
 
         for art in self.article_data:
             can_pages = art["m"]["pp"]
 
             for can_page, page_content in zip(can_pages, art["pages"]):
                 can_id = f"{self.id}-p{can_page:04}"
                 self.pages.append(
-                    TetmlNewspaperPage(can_id, can_page, page_content, art["meta"]["tetml_path"])
+                    TetmlNewspaperPage(
+                        can_id, can_page, page_content, art["meta"]["tetml_path"]
+                    )
                 )
```

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/tetml/detect.py` & `impresso_text_importer-1.1.0/text_importer/importers/tetml/detect.py`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/tetml/helpers.py` & `impresso_text_importer-1.1.0/text_importer/importers/tetml/helpers.py`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/tetml/parsers.py` & `impresso_text_importer-1.1.0/text_importer/importers/tetml/parsers.py`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/importers/tetml/tetml2canonical.py` & `impresso_text_importer-1.1.0/text_importer/importers/tetml/tetml2canonical.py`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/linguistic_annotation/ling_spacy.schema.json` & `impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/linguistic_annotation/ling_spacy.schema.json`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/newspaper/contentitem.schema.json` & `impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/newspaper/contentitem.schema.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9416666666666667%*

 * *Differences: {"'properties'": '{\'ro\': OrderedDict([(\'description\', "Reading order index of the content '*

 * *                 'item, for the table of contents view on the interface. If not defined, the CI '*

 * *                 'number (after \'i\' in the ID) should be used."), (\'type\', \'integer\')])}',*

 * * "'required'": "{insert: [(1, 'tp'), (2, 'olr'), (3, 'ts')]}"}*

```diff
@@ -94,14 +94,18 @@
         "rb": {
             "description": "text offsets of page regions (relative to 'ft' field)",
             "items": {
                 "type": "number"
             },
             "type": "array"
         },
+        "ro": {
+            "description": "Reading order index of the content item, for the table of contents view on the interface. If not defined, the CI number (after 'i' in the ID) should be used.",
+            "type": "integer"
+        },
         "s3v": {
             "description": "S3 version ID of the corresponding issue.json file",
             "type": "string"
         },
         "tp": {
             "description": "content item type (e.g. 'ar' for article, 'ad' for advertisement)",
             "type": "string"
@@ -109,12 +113,15 @@
         "ts": {
             "description": "timestamp of creation of the JSON file (e.g. '2018-09-18T08:00:08Z')",
             "pattern": "^[0-9]{4}-[0-9]{2}-[0-9]{2}T[0-9]{2}:[0-9]{2}:[0-9]{2}Z$",
             "type": "string"
         }
     },
     "required": [
-        "id"
+        "id",
+        "tp",
+        "olr",
+        "ts"
     ],
     "title": "Content Item",
     "type": "object"
 }
```

### Comparing `impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/newspaper/issue.schema.json` & `impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/newspaper/issue.schema.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9903243361146542%*

 * *Differences: {"'definitions'": "{'metadata': {'properties': {'tp': {'enum': {insert: [(6, 'page')]}}, "*

 * *                  '\'iiif_link\': {\'description\': "IIIF image link, depending on content item '*

 * *                  'type (if `tp == image`). Should follow the format: '*

 * *                  '\'{scheme}://{server}/{prefix}/{identifier}/info.json\'."}, \'ro\': '*

 * *                  'OrderedDict([(\'type\', \'integer\'), (\'description\', "Reading order index of '*

 * *                  'the content item, for the table of content […]*

```diff
@@ -5,41 +5,46 @@
         "metadata": {
             "properties": {
                 "id": {
                     "description": "Content item ID (e.g. `GDL-1900-01-02-a-i0001`).",
                     "type": "string"
                 },
                 "iiif_link": {
-                    "description": "IIIF image link, depending on content item type (if `tp == image`)",
+                    "description": "IIIF image link, depending on content item type (if `tp == image`). Should follow the format: '{scheme}://{server}/{prefix}/{identifier}/info.json'.",
                     "type": "string"
                 },
                 "l": {
                     "description": "Language of the content item.",
                     "type": "string"
                 },
                 "pp": {
                     "description": "Page numbers over which the content item spans.",
                     "items": {
                         "type": "integer"
                     },
                     "type": "array"
                 },
+                "ro": {
+                    "description": "Reading order index of the content item, for the table of contents view on the interface. If not defined, the CI number (after 'i' in the ID) should be used.",
+                    "type": "integer"
+                },
                 "t": {
                     "description": "Title of the content item.",
                     "type": "string"
                 },
                 "tp": {
                     "description": "Type of the content item.",
                     "enum": [
                         "article",
                         "ad",
                         "image",
                         "table",
                         "death_notice",
-                        "weather"
+                        "weather",
+                        "page"
                     ],
                     "type": "string"
                 }
             },
             "required": [
                 "id",
                 "pp",
@@ -64,28 +69,40 @@
             "type": "string"
         },
         "i": {
             "description": "The content items contained in the newspaper issue.",
             "items": {
                 "description": "A content item (e.g. article, advertisement, etc.)",
                 "properties": {
+                    "c": {
+                        "description": "Coordinates of image-region corresponding to the content-item depending on its type (if `tp == image`).",
+                        "items": {
+                            "type": "integer"
+                        },
+                        "minItems": 4,
+                        "type": "array"
+                    },
                     "m": {
                         "$ref": "#/definitions/metadata",
                         "description": "Metadata about the content item."
                     }
                 },
                 "required": [
                     "m"
                 ],
                 "type": "object"
             },
             "type": "array"
         },
         "id": {
-            "description": "Canonical ID of the newspaper issue (e.g. GDL-1900-01-02-a-i0001)",
+            "description": "Canonical ID of the newspaper issue (e.g. GDL-1900-01-02-a)",
+            "type": "string"
+        },
+        "iiif_manifest_uri": {
+            "description": "URI for the issue's manifest in the IIIF Presentation API, if the corresponding IIIF server has one.",
             "type": "string"
         },
         "n": {
             "description": "Notes.",
             "type": "string"
         },
         "pp": {
```

### Comparing `impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/topic_model/topic_assignment.schema.json` & `impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/topic_model/topic_assignment.schema.json`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/impresso-schemas/json/topic_model/topic_description.schema.json` & `impresso_text_importer-1.1.0/text_importer/impresso-schemas/json/topic_model/topic_description.schema.json`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/scripts/compress_canonical.py` & `impresso_text_importer-1.1.0/text_importer/scripts/compress_canonical.py`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/scripts/upload.py` & `impresso_text_importer-1.1.0/text_importer/scripts/upload.py`

 * *Files identical despite different names*

### Comparing `impresso_text_importer-1.0.0/text_importer/tokenization.py` & `impresso_text_importer-1.1.0/text_importer/tokenization.py`

 * *Files identical despite different names*

