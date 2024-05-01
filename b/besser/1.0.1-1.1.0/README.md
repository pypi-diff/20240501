# Comparing `tmp/besser-1.0.1.tar.gz` & `tmp/besser-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besser-1.0.1.tar", last modified: Fri Apr 26 09:30:14 2024, max compression
+gzip compressed data, was "besser-1.1.0.tar", last modified: Wed May  1 21:35:02 2024, max compression
```

## Comparing `besser-1.0.1.tar` & `besser-1.1.0.tar`

### file list

```diff
@@ -1,110 +1,120 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.991981 besser-1.0.1/
--rw-rw-rw-   0        0        0     3712 2024-04-26 09:30:14.990982 besser-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2804 2024-04-19 11:55:41.000000 besser-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.902433 besser-1.0.1/besser/
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.908433 besser-1.0.1/besser/BUML/
--rw-rw-rw-   0        0        0        0 2023-11-29 15:43:44.000000 besser-1.0.1/besser/BUML/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.909433 besser-1.0.1/besser/BUML/metamodel/
--rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.0.1/besser/BUML/metamodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.911433 besser-1.0.1/besser/BUML/metamodel/gui/
--rw-rw-rw-   0        0        0       29 2024-03-07 10:53:16.000000 besser-1.0.1/besser/BUML/metamodel/gui/__init__.py
--rw-rw-rw-   0        0        0    25750 2024-03-08 08:46:02.000000 besser-1.0.1/besser/BUML/metamodel/gui/graphical_ui.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.914433 besser-1.0.1/besser/BUML/metamodel/object/
--rw-rw-rw-   0        0        0       21 2024-03-07 08:52:50.000000 besser-1.0.1/besser/BUML/metamodel/object/__init__.py
--rw-rw-rw-   0        0        0    10058 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/metamodel/object/object.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.916456 besser-1.0.1/besser/BUML/metamodel/ocl/
--rw-rw-rw-   0        0        0       20 2024-03-11 12:02:13.000000 besser-1.0.1/besser/BUML/metamodel/ocl/__init__.py
--rw-rw-rw-   0        0        0    10785 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/metamodel/ocl/rules.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.919434 besser-1.0.1/besser/BUML/metamodel/structural/
--rw-rw-rw-   0        0        0       25 2024-03-11 12:02:25.000000 besser-1.0.1/besser/BUML/metamodel/structural/__init__.py
--rw-rw-rw-   0        0        0    43485 2024-04-19 11:55:28.000000 besser-1.0.1/besser/BUML/metamodel/structural/structural.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.921460 besser-1.0.1/besser/BUML/notations/
--rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.0.1/besser/BUML/notations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.926438 besser-1.0.1/besser/BUML/notations/objectPlantUML/
--rw-rw-rw-   0        0        0     5938 2024-03-07 08:40:30.000000 besser-1.0.1/besser/BUML/notations/objectPlantUML/ODLexer.py
--rw-rw-rw-   0        0        0     4994 2024-03-07 16:34:33.000000 besser-1.0.1/besser/BUML/notations/objectPlantUML/ODListener.py
--rw-rw-rw-   0        0        0    25828 2024-03-07 08:40:30.000000 besser-1.0.1/besser/BUML/notations/objectPlantUML/ODParser.py
--rw-rw-rw-   0        0        0        0 2024-03-07 08:40:30.000000 besser-1.0.1/besser/BUML/notations/objectPlantUML/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.939492 besser-1.0.1/besser/BUML/notations/ocl/
--rw-rw-rw-   0        0        0    23268 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/BOCLLexer.py
--rw-rw-rw-   0        0        0    41633 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/BOCLListener.py
--rw-rw-rw-   0        0        0   212929 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/BOCLParser.py
--rw-rw-rw-   0        0        0     4732 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/FactoryInstance.py
--rw-rw-rw-   0        0        0     1080 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/OCLWrapper.py
--rw-rw-rw-   0        0        0    12723 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/RootHandler.py
--rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.0.1/besser/BUML/notations/ocl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.945433 besser-1.0.1/besser/BUML/notations/structuralPlantUML/
--rw-rw-rw-   0        0        0    10331 2024-01-06 10:27:58.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py
--rw-rw-rw-   0        0        0     6394 2024-01-06 10:27:59.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py
--rw-rw-rw-   0        0        0    51575 2024-01-06 10:27:59.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py
--rw-rw-rw-   0        0        0      203 2024-01-04 12:38:28.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/__init__.py
--rw-rw-rw-   0        0        0     9121 2024-01-15 16:13:03.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py
--rw-rw-rw-   0        0        0     1432 2024-01-15 16:10:59.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py
--rw-rw-rw-   0        0        0        0 2024-01-15 16:06:49.000000 besser-1.0.1/besser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.948449 besser-1.0.1/besser/generators/
--rw-rw-rw-   0        0        0       34 2023-10-23 15:26:16.000000 besser-1.0.1/besser/generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.950435 besser-1.0.1/besser/generators/django/
--rw-rw-rw-   0        0        0       31 2023-11-24 11:35:33.000000 besser-1.0.1/besser/generators/django/__init__.py
--rw-rw-rw-   0        0        0     1756 2024-01-15 16:11:55.000000 besser-1.0.1/besser/generators/django/django_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.953466 besser-1.0.1/besser/generators/django/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.1/besser/generators/django/templates/__init__.py
--rw-rw-rw-   0        0        0      608 2023-11-24 11:35:33.000000 besser-1.0.1/besser/generators/django/templates/django_fields.py.j2
--rw-rw-rw-   0        0        0     3213 2023-11-24 11:36:43.000000 besser-1.0.1/besser/generators/django/templates/django_template.py.j2
--rw-rw-rw-   0        0        0     1166 2024-03-08 16:36:51.000000 besser-1.0.1/besser/generators/generator_interface.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.956461 besser-1.0.1/besser/generators/python_classes/
--rw-rw-rw-   0        0        0       39 2023-11-03 14:54:15.000000 besser-1.0.1/besser/generators/python_classes/__init__.py
--rw-rw-rw-   0        0        0     1724 2024-01-15 16:13:59.000000 besser-1.0.1/besser/generators/python_classes/python_classes_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.959452 besser-1.0.1/besser/generators/python_classes/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.1/besser/generators/python_classes/templates/__init__.py
--rw-rw-rw-   0        0        0     1461 2024-01-05 14:02:17.000000 besser-1.0.1/besser/generators/python_classes/templates/class_parameters.py.j2
--rw-rw-rw-   0        0        0     1496 2024-01-04 17:15:56.000000 besser-1.0.1/besser/generators/python_classes/templates/python_classes_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.962434 besser-1.0.1/besser/generators/rest_api/
--rw-rw-rw-   0        0        0       33 2024-03-07 08:29:25.000000 besser-1.0.1/besser/generators/rest_api/__init__.py
--rw-rw-rw-   0        0        0     2720 2024-03-07 13:36:29.000000 besser-1.0.1/besser/generators/rest_api/rest_api_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.964440 besser-1.0.1/besser/generators/rest_api/templates/
--rw-rw-rw-   0        0        0        0 2024-03-07 08:29:25.000000 besser-1.0.1/besser/generators/rest_api/templates/__init__.py
--rw-rw-rw-   0        0        0     7985 2024-03-07 13:36:29.000000 besser-1.0.1/besser/generators/rest_api/templates/fast_api_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.967455 besser-1.0.1/besser/generators/sql/
--rw-rw-rw-   0        0        0       28 2023-11-03 14:54:15.000000 besser-1.0.1/besser/generators/sql/__init__.py
--rw-rw-rw-   0        0        0     2191 2024-01-15 16:14:26.000000 besser-1.0.1/besser/generators/sql/sql_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.970451 besser-1.0.1/besser/generators/sql/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.1/besser/generators/sql/templates/__init__.py
--rw-rw-rw-   0        0        0     4633 2023-11-24 11:35:33.000000 besser-1.0.1/besser/generators/sql/templates/sql_dialects.sql.j2
--rw-rw-rw-   0        0        0     3608 2023-11-24 11:35:33.000000 besser-1.0.1/besser/generators/sql/templates/sql_template.sql.j2
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.972453 besser-1.0.1/besser/generators/sql_alchemy/
--rw-rw-rw-   0        0        0       36 2023-11-23 14:47:36.000000 besser-1.0.1/besser/generators/sql_alchemy/__init__.py
--rw-rw-rw-   0        0        0     1994 2024-01-15 16:14:45.000000 besser-1.0.1/besser/generators/sql_alchemy/sql_alchemy_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.974475 besser-1.0.1/besser/generators/sql_alchemy/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.1/besser/generators/sql_alchemy/templates/__init__.py
--rw-rw-rw-   0        0        0     3632 2024-01-11 16:19:34.000000 besser-1.0.1/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.977450 besser-1.0.1/besser/utilities/
--rw-rw-rw-   0        0        0       50 2024-01-04 13:03:26.000000 besser-1.0.1/besser/utilities/__init__.py
--rw-rw-rw-   0        0        0     2709 2024-03-08 14:36:21.000000 besser-1.0.1/besser/utilities/image_to_buml.py
--rw-rw-rw-   0        0        0     2106 2024-01-15 16:16:07.000000 besser-1.0.1/besser/utilities/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.989983 besser-1.0.1/besser.egg-info/
--rw-rw-rw-   0        0        0     3712 2024-04-26 09:30:14.000000 besser-1.0.1/besser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2024-04-26 09:30:14.000000 besser-1.0.1/besser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 09:30:14.000000 besser-1.0.1/besser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      230 2024-04-26 09:30:14.000000 besser-1.0.1/besser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-26 09:30:14.000000 besser-1.0.1/besser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-10-23 15:26:16.000000 besser-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      242 2024-03-11 12:49:37.000000 besser-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0      659 2024-04-26 09:30:14.992968 besser-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.978451 besser-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.980960 besser-1.0.1/tests/gui/
--rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/gui/__init__.py
--rw-rw-rw-   0        0        0     2480 2024-03-11 13:08:13.000000 besser-1.0.1/tests/gui/gui_model.py
--rw-rw-rw-   0        0        0     5271 2024-03-08 09:35:33.000000 besser-1.0.1/tests/gui/test_gui.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.981967 besser-1.0.1/tests/notations/
--rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/notations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.984971 besser-1.0.1/tests/object/
--rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/object/__init__.py
--rw-rw-rw-   0        0        0    10547 2024-04-26 08:06:13.000000 besser-1.0.1/tests/object/library_object.py
--rw-rw-rw-   0        0        0     3879 2024-03-07 16:31:15.000000 besser-1.0.1/tests/object/test_object_mm.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.986974 besser-1.0.1/tests/ocl/
--rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/ocl/__init__.py
--rw-rw-rw-   0        0        0     7566 2024-04-26 08:06:13.000000 besser-1.0.1/tests/ocl/test_ocl_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.988985 besser-1.0.1/tests/structural/
--rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/structural/__init__.py
--rw-rw-rw-   0        0        0    10194 2024-01-15 16:18:42.000000 besser-1.0.1/tests/structural/test_structural.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.115845 besser-1.1.0/
+-rw-rw-rw-   0        0        0     3777 2024-05-01 21:35:02.114846 besser-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2804 2024-04-29 14:01:22.000000 besser-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.007321 besser-1.1.0/besser/
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.016795 besser-1.1.0/besser/BUML/
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:43:44.000000 besser-1.1.0/besser/BUML/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.018792 besser-1.1.0/besser/BUML/metamodel/
+-rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.1.0/besser/BUML/metamodel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.020788 besser-1.1.0/besser/BUML/metamodel/gui/
+-rw-rw-rw-   0        0        0       29 2024-03-07 10:53:16.000000 besser-1.1.0/besser/BUML/metamodel/gui/__init__.py
+-rw-rw-rw-   0        0        0    25750 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/metamodel/gui/graphical_ui.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.023560 besser-1.1.0/besser/BUML/metamodel/object/
+-rw-rw-rw-   0        0        0       21 2024-03-07 08:52:50.000000 besser-1.1.0/besser/BUML/metamodel/object/__init__.py
+-rw-rw-rw-   0        0        0    10058 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/metamodel/object/object.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.025909 besser-1.1.0/besser/BUML/metamodel/ocl/
+-rw-rw-rw-   0        0        0       20 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/metamodel/ocl/__init__.py
+-rw-rw-rw-   0        0        0    18910 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/metamodel/ocl/rules.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.028244 besser-1.1.0/besser/BUML/metamodel/structural/
+-rw-rw-rw-   0        0        0       25 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/metamodel/structural/__init__.py
+-rw-rw-rw-   0        0        0    42656 2024-05-01 21:18:56.000000 besser-1.1.0/besser/BUML/metamodel/structural/structural.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.030734 besser-1.1.0/besser/BUML/notations/
+-rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.1.0/besser/BUML/notations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.036732 besser-1.1.0/besser/BUML/notations/objectPlantUML/
+-rw-rw-rw-   0        0        0     5938 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/objectPlantUML/ODLexer.py
+-rw-rw-rw-   0        0        0     4994 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/objectPlantUML/ODListener.py
+-rw-rw-rw-   0        0        0    25828 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/objectPlantUML/ODParser.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/objectPlantUML/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.050327 besser-1.1.0/besser/BUML/notations/ocl/
+-rw-rw-rw-   0        0        0    23268 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/BOCLLexer.py
+-rw-rw-rw-   0        0        0    41633 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/BOCLListener.py
+-rw-rw-rw-   0        0        0   212929 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/BOCLParser.py
+-rw-rw-rw-   0        0        0     4732 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/FactoryInstance.py
+-rw-rw-rw-   0        0        0     1080 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/OCLWrapper.py
+-rw-rw-rw-   0        0        0    12723 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/RootHandler.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.058329 besser-1.1.0/besser/BUML/notations/structuralPlantUML/
+-rw-rw-rw-   0        0        0    10331 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py
+-rw-rw-rw-   0        0        0     6394 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py
+-rw-rw-rw-   0        0        0    51575 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py
+-rw-rw-rw-   0        0        0      203 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/__init__.py
+-rw-rw-rw-   0        0        0     9121 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py
+-rw-rw-rw-   0        0        0     1432 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py
+-rw-rw-rw-   0        0        0        0 2024-01-15 16:06:49.000000 besser-1.1.0/besser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.060328 besser-1.1.0/besser/generators/
+-rw-rw-rw-   0        0        0       34 2023-10-23 15:26:16.000000 besser-1.1.0/besser/generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.063330 besser-1.1.0/besser/generators/backend/
+-rw-rw-rw-   0        0        0       32 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/backend/__init__.py
+-rw-rw-rw-   0        0        0     3276 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/backend/backend_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.065330 besser-1.1.0/besser/generators/django/
+-rw-rw-rw-   0        0        0       31 2023-11-24 11:35:33.000000 besser-1.1.0/besser/generators/django/__init__.py
+-rw-rw-rw-   0        0        0     1756 2024-01-15 16:11:55.000000 besser-1.1.0/besser/generators/django/django_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.068330 besser-1.1.0/besser/generators/django/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.0/besser/generators/django/templates/__init__.py
+-rw-rw-rw-   0        0        0      608 2023-11-24 11:35:33.000000 besser-1.1.0/besser/generators/django/templates/django_fields.py.j2
+-rw-rw-rw-   0        0        0     3580 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/django/templates/django_template.py.j2
+-rw-rw-rw-   0        0        0     1166 2024-04-29 14:01:22.000000 besser-1.1.0/besser/generators/generator_interface.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.072329 besser-1.1.0/besser/generators/pydantic_classes/
+-rw-rw-rw-   0        0        0       41 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/pydantic_classes/__init__.py
+-rw-rw-rw-   0        0        0     2593 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/pydantic_classes/pydantic_classes_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.074330 besser-1.1.0/besser/generators/pydantic_classes/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/pydantic_classes/templates/__init__.py
+-rw-rw-rw-   0        0        0     3409 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/pydantic_classes/templates/pydantic_classes_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.077334 besser-1.1.0/besser/generators/python_classes/
+-rw-rw-rw-   0        0        0       39 2023-11-03 14:54:15.000000 besser-1.1.0/besser/generators/python_classes/__init__.py
+-rw-rw-rw-   0        0        0     1722 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/python_classes/python_classes_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.081335 besser-1.1.0/besser/generators/python_classes/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.0/besser/generators/python_classes/templates/__init__.py
+-rw-rw-rw-   0        0        0     1461 2024-01-05 14:02:17.000000 besser-1.1.0/besser/generators/python_classes/templates/class_parameters.py.j2
+-rw-rw-rw-   0        0        0     1496 2024-01-04 17:15:56.000000 besser-1.1.0/besser/generators/python_classes/templates/python_classes_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.083335 besser-1.1.0/besser/generators/rest_api/
+-rw-rw-rw-   0        0        0       33 2024-03-07 08:29:25.000000 besser-1.1.0/besser/generators/rest_api/__init__.py
+-rw-rw-rw-   0        0        0     4716 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/rest_api/rest_api_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.087335 besser-1.1.0/besser/generators/rest_api/templates/
+-rw-rw-rw-   0        0        0        0 2024-03-07 08:29:25.000000 besser-1.1.0/besser/generators/rest_api/templates/__init__.py
+-rw-rw-rw-   0        0        0    11014 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/rest_api/templates/backend_fast_api_template.py.j2
+-rw-rw-rw-   0        0        0     4987 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/rest_api/templates/fast_api_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.089334 besser-1.1.0/besser/generators/sql/
+-rw-rw-rw-   0        0        0       28 2023-11-03 14:54:15.000000 besser-1.1.0/besser/generators/sql/__init__.py
+-rw-rw-rw-   0        0        0     2191 2024-01-15 16:14:26.000000 besser-1.1.0/besser/generators/sql/sql_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.092845 besser-1.1.0/besser/generators/sql/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.0/besser/generators/sql/templates/__init__.py
+-rw-rw-rw-   0        0        0     4633 2023-11-24 11:35:33.000000 besser-1.1.0/besser/generators/sql/templates/sql_dialects.sql.j2
+-rw-rw-rw-   0        0        0     3608 2023-11-24 11:35:33.000000 besser-1.1.0/besser/generators/sql/templates/sql_template.sql.j2
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.094845 besser-1.1.0/besser/generators/sql_alchemy/
+-rw-rw-rw-   0        0        0       36 2023-11-23 14:47:36.000000 besser-1.1.0/besser/generators/sql_alchemy/__init__.py
+-rw-rw-rw-   0        0        0     1994 2024-01-15 16:14:45.000000 besser-1.1.0/besser/generators/sql_alchemy/sql_alchemy_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.096844 besser-1.1.0/besser/generators/sql_alchemy/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.0/besser/generators/sql_alchemy/templates/__init__.py
+-rw-rw-rw-   0        0        0     3695 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.100845 besser-1.1.0/besser/utilities/
+-rw-rw-rw-   0        0        0       50 2024-01-04 13:03:26.000000 besser-1.1.0/besser/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2897 2024-05-01 21:18:56.000000 besser-1.1.0/besser/utilities/image_to_buml.py
+-rw-rw-rw-   0        0        0     2106 2024-01-15 16:16:07.000000 besser-1.1.0/besser/utilities/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.113847 besser-1.1.0/besser.egg-info/
+-rw-rw-rw-   0        0        0     3777 2024-05-01 21:35:01.000000 besser-1.1.0/besser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3529 2024-05-01 21:35:01.000000 besser-1.1.0/besser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 21:35:01.000000 besser-1.1.0/besser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      263 2024-05-01 21:35:01.000000 besser-1.1.0/besser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-01 21:35:01.000000 besser-1.1.0/besser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-10-23 15:26:16.000000 besser-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      277 2024-05-01 21:18:56.000000 besser-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0      659 2024-05-01 21:35:02.116848 besser-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.101845 besser-1.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.103845 besser-1.1.0/tests/gui/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/gui/__init__.py
+-rw-rw-rw-   0        0        0     2479 2024-05-01 21:33:29.000000 besser-1.1.0/tests/gui/gui_model.py
+-rw-rw-rw-   0        0        0     5271 2024-04-29 14:01:22.000000 besser-1.1.0/tests/gui/test_gui.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.105846 besser-1.1.0/tests/notations/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/notations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.108845 besser-1.1.0/tests/object/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/object/__init__.py
+-rw-rw-rw-   0        0        0    10547 2024-04-29 14:01:22.000000 besser-1.1.0/tests/object/library_object.py
+-rw-rw-rw-   0        0        0     3879 2024-04-29 14:01:22.000000 besser-1.1.0/tests/object/test_object_mm.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.109845 besser-1.1.0/tests/ocl/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/ocl/__init__.py
+-rw-rw-rw-   0        0        0     7566 2024-04-29 14:01:22.000000 besser-1.1.0/tests/ocl/test_ocl_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.111845 besser-1.1.0/tests/structural/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/structural/__init__.py
+-rw-rw-rw-   0        0        0    10194 2024-01-15 16:18:42.000000 besser-1.1.0/tests/structural/test_structural.py
```

### Comparing `besser-1.0.1/PKG-INFO` & `besser-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besser
-Version: 1.0.1
+Version: 1.1.0
 Summary: BESSER
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besser.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER/issues
 Keywords: uml,code generation,python
@@ -20,14 +20,16 @@
 Requires-Dist: textX==3.1.1
 Requires-Dist: jinja2==3.1.2
 Requires-Dist: antlr4-python3-runtime==4.13.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: fastapi==0.110.0
 Requires-Dist: pydantic==2.6.3
 Requires-Dist: uvicorn==0.28.0
+Requires-Dist: SQLAlchemy==2.0.29
+Requires-Dist: httpx==0.27.0
 
 # BESSER
 
 BESSER is a [low-modeling](https://modeling-languages.com/welcome-to-the-low-modeling-revolution/) [low-code](https://modeling-languages.com/low-code-vs-model-driven/) open-source platform. BESSER (Building bEtter Smart Software fastER) is funded thanks to an [FNR Pearl grant](https://modeling-languages.com/a-smart-low-code-platform-for-smart-software-in-luxembourg-goodbye-barcelona/) led by the [Luxembourg Institute of Science and Technology](https://www.list.lu/) with the participation of the [Snt/University of Luxembourg](https://www.uni.lu/snt-en/) and open to all your contributions!
 
 The BESSER low-code platform is built on top of our Python-based personal interpretation of a "Universal Modeling Language" (yes, heavily inspired and a simplified version of the better known UML, the Unified Modeling Language)
```

### Comparing `besser-1.0.1/README.md` & `besser-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/metamodel/gui/graphical_ui.py` & `besser-1.1.0/besser/BUML/metamodel/gui/graphical_ui.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/metamodel/object/object.py` & `besser-1.1.0/besser/BUML/metamodel/object/object.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/metamodel/ocl/rules.py` & `besser-1.1.0/besser/BUML/notations/ocl/RootHandler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,365 +1,325 @@
-from typing import Any
-from besser.BUML.metamodel.structural import Class, NamedElement, TypedElement, Type, PrimitiveDataType, Property, Constraint
+from besser.BUML.notations.ocl.FactoryInstance import Factory
+class Root_Handler:
+    def __init__(self,ocl=None,dm=None,om=None):
+        context = None
+        if ocl is not None:
+            context = ocl.context
+        self.root = None
+        self.dm = dm
+        self.om = om
+        self.factory = Factory(context)
+        self.all =[]
+        self.context = context
+        self.invariant = False
+        self.pre = False
+        self.post = False
+        self.if_else_roots = []
+
+    def get_root(self):
+        return self.root
+    def get_inv(self):
+        return self.invariant
+    def set_inv(self,inv):
+        self.invariant = inv
+    def set_post(self,post):
+        self.post = post
+    def get_post(self):
+        return self.post
 
-
-class OCLExpression(TypedElement):
-    def __init__(self, name: str, type: Type):
-        super().__init__(name, type)
-        self._source = None
-        self._referredOperation = None
-
-    @property
-    def source(self) ->Any:
-        return self._source
-    @source.setter
-    def source(self, source)->Any:
-        self._source = source
-    @property
-    def referredOperation(self)->Any:
-        return self._referredOperation
-
-    @referredOperation.setter
-    def referredOperation(self, op):
-        self._referredOperation = op
-
-
-
-    def __str__(self) -> str:
-        pass
-
-
-# A literal value part of an OCL expression
-class LiteralExpression(OCLExpression):
-    def __init__(self, name: str, type: Type, value: Any):
-        super().__init__(name, type)
-        self.value: Any = value
-
-    @property
-    def value(self) -> Any:
-        return self.__value
-
-    @value.setter
-    def value(self, value: Any):
-        self.__value = value
-
-    def __str__(self) -> str:
-        return str(self.value)
-
-class IntegerLiteralExpression(LiteralExpression):
-    def __init__(self, name: str, value: int):
-        super().__init__(name, type=PrimitiveDataType(name="int"), value=value)
-
-    def __repr__(self):
-        return f'IntegerLiteralExpression({self.value})'
-
-
-# Expression that returns the value of a given Property
-class PropertyCallExpression(OCLExpression):
-    def __init__(self, name: str, property: Property):
-        super().__init__(name, Type(property.type))
-        self.property: Property = property
-
-    def __repr__(self):
-        return f'PropertyCallExpression({self.property.name})'
-
-    def __str__(self) -> str:
-        return str(self.property.name)
-
-    @property
-    def property(self) -> Property:
-        return self.__property
-
-    @property.setter
-    def property(self, property: Property):
-        self.__property = property
-
-
-# Expression that returns the value of a given Operation on a given set of ordered arguments
-# The operation could also be a reference to any operation in an existing class but for now we stick to simple
-# arithmetic comparison operations from the standard OCL library
-class OperationCallExpression(OCLExpression):
-    def __init__(self, name: str, operation: str, arguments: list[OCLExpression]):
-        super().__init__(name, Type(PrimitiveDataType("bool")))  # Type for now is always boolean, it should be the return type of the operation
-        self.operation: str = operation
-        self.arguments: list[OCLExpression] = arguments
-
-    def __repr__(self):
-        return f'OperationCallExpression({self.operation},{self.arguments})'
-
-    @property
-    def operation(self) -> str:
-        return self.__operation
-
-    @operation.setter
-    def operation(self, operation: str):
-        self.__operation = operation
-
-    @property
-    def arguments(self) -> list[OCLExpression]:
-        return self.__arguments
-
-    @arguments.setter
-    def arguments(self, arguments: list[OCLExpression]):
-        self.__arguments = arguments
-    def add(self,item):
-        self.arguments.append(item)
-    def __str__(self) -> str:
-        toRet= ""
-        for arg in self.arguments:
-            # print(type(arg))
-            toRet = toRet+"  \n "+ str(arg)
-        return toRet
-        # return f'{self.arguments[0]} {self.operation} {self.arguments[1]}'
-
-# A class to represents OCL constriants, i.e. constraints written with the OCL language
-class OCLConstraint(Constraint):
-    def __init__(self, name: str, context: Class, expression: OCLExpression, language: str = "OCL"):
-        super().__init__(name, context, expression, language)
-
-
-class IfExp(OCLExpression):
-    def __init__(self, name: str, type: Type,ifcond = None, elseExp = None, thenExp = None,):
-        # self.ifOwner = null
-        super().__init__(name, type)
-
-        self._ifCondition = None
-        self._else_expression = None
-        self._then_expression = None
-
-    @property
-    def ifCondition (self) -> OCLExpression:
-        return self._ifCondition
-
-    @property
-    def elseCondition(self) -> OCLExpression:
-        return self._else_expression
-    @property
-    def thenExpression(self) ->OCLExpression:
-        return self._then_expression
-
-    @ifCondition.setter
-    def ifCondition (self,if_cond):
-        self._ifCondition = if_cond
-
-    @elseCondition.setter
-    def elseCondition(self,else_cond):
-        self._else_expression = else_cond
-    @thenExpression.setter
-    def thenExpression(self, then_expression):
-        self._then_expression = then_expression
-class VariableExp(OCLExpression):
-    def __init__(self,name: str, type: Type):
-        super().__init__(name, type)
-        self.name = name
-        self.variable = Variable(name,type)
-
-    def set_refferred_variable (self,val):
-        val.replace('self.','')
-        self.variable.set_value(val)
-    def getVal(self):
-        return self.variable.get_value()
-
-    def __str__(self):
-        return self.name
-
-class Variable(OCLExpression):
-    def __init__(self,name: str, type: Type):
-        super().__init__(name, type)
-
-    def set_value(self, val):
-        self.representatedParameter = Parameter(val)
-    def get_value(self):
-        return self.representatedParameter.get_value()
-
-# class Property:
-#     def __init__(self):
-#         self.referringExp = []
-#         self.val = None
-
-class TypeExp(OCLExpression):
-        def __init__(self,name: str, type: Type):
-            super().__init__(name, type)
-
-            self.referedType = Classifier(name)
-class Parameter:
-    def __init__(self,val):
-        self.value =val
-
-    def get_value(self):
-        return self.value
-
-
-class StateExp(OCLExpression):
-        def __init__(self,name: str, type: Type):
-            super().__init__(name, type)
-
-            self.referedState = State()
-class State:
-    def __init__(self):
-        self.stateExp = []
-
-class RealLiteralExpression(LiteralExpression):
-    def __init__(self, name: str, value: float):
-        super().__init__(name, type=PrimitiveDataType(name="float"), value=value)
-
-    def __repr__(self):
-        return f'RealLiteralExpression({self.value})'
-
-
-class Classifier:
-    def __init__(self, name= None):
-        self.name = name
-    pass
-class CallExp(OCLExpression):
-    pass
-class FeatureCallExp(CallExp):
-    pass
-class LiteralExp(OCLExpression):
-    pass
-class InvalidLiteralExp(LiteralExp):
-    pass
-class LoopExp(CallExp):
-    def __init__(self,name: str, type: Type):
-        super().__init__(name, type)
-
-        self.name = name
-        self.type = type
-        self.body = []
-        self.iterator = []
-
-    def __str__(self):
-        stringToRet = "LoopExpression: " +str(self.name)
-        for it in self.iterator:
-            stringToRet = stringToRet + "\nIterator: " + str(it)
-        for body in self.body:
-            stringToRet = stringToRet + "\nbody: " + str(body)
-        return stringToRet
-
-
-    def add_body(self,body):
-        self.body.append(body)
-    @property
+    def set_body(self,body):
+        self.body = body
     def get_body(self):
         return self.body
-    def addIterator(self,iterator):
-        self.iterator.append(iterator)
-    # @property
-    # def set_iterator (self,iterator):
-    #     self.iterator = iterator
-    @property
-    def get_iterator(self):
-        return self.iterator
-
-
-class MessageExp(OCLExpression):
-    pass
-class NavigationCallExp(OCLExpression):
-    pass
-class NullLiteralExp(LiteralExp):
-    pass
-
-class PrimitiveLiteralExp(LiteralExp):
-    pass
-class NumericLiteralExp(PrimitiveLiteralExp):
-    pass
-class IterateExp(LoopExp):
-    def __init__(self,name: str, type: Type):
-        super().__init__(name, type)
-
-        self.result=Variable()
-
-class IteratorExp(LoopExp):
-    def __init__(self,name: str, type: Type):
-        super().__init__(name, type)
-        self.name = name
-        self.type = type
-    pass
-    def __str__(self):
-        return self.name +":" +self.type
-
-class LetExp(OCLExpression):
-    def __init__(self, name: str, type: Type):
-        super().__init__(name, type)
-        self.OCLExpression = None
-        self.variable = None
-class BooleanLiteralExpression(LiteralExpression):
-    def __init__(self, name: str, value: bool):
-        super().__init__(name, type=PrimitiveDataType(name="bool"), value=value)
-
-    def __repr__(self):
-        return f'BooleanLiteralExpression({self.value})'
-class StringLiteralExpression(LiteralExpression):
-    def __init__(self, name: str, value: str):
-        super().__init__(name, type=PrimitiveDataType(name="str"), value=value)
-
-    def __repr__(self):
-        return f'StringLiteralExpression({self.value})'
-
-class InfixOperator:
-    def __init__(self,operator):
-        self.operator = operator
-    def get_infix_operator(self):
-        return self.operator
-    def __str__(self):
-        return self.operator
-
-class DataType(Classifier):
-    def __init__(self,name):
-        super().__init__(name)
-
-class CollectionType(DataType):
-    def __init__(self,name):
-        super().__init__(name)
-
-class OrderedSetType(CollectionType):
-    def __init__(self,name):
-        super().__init__(name)
-
-class SequenceType(CollectionType):
-    def __init__(self,name):
-        super().__init__(name)
-
-class BagType(CollectionType):
-    def __init__(self,name):
-        super().__init__(name)
-
-class SetType(CollectionType):
-    def __init__(self,name):
-        super().__init__(name)
-
-
-class CollectionLiteralExp(LiteralExp):
-    def __init__(self, name, type):
-        super().__init__(name,type)
-        self.kind = type
-        self.collectionItems = []
-    def __str__(self):
-        toRet= str(self.kind) +": "
-        for item in self.collectionItems:
-            toRet = toRet + str(item)
-        return toRet
-    def add(self, item):
-        self.collectionItems.append(item)
-
-class CollectionLiteralPart(TypedElement):
-    def __init__(self, name):
-        super().__init__(name,type = "NP")
-
-
-class CollectionItem(CollectionLiteralPart):
-    def __init__(self, name,item):
-        super().__init__(name)
-        self.value = item
-    def set(self,  value):
-        self.value = value
-    def __str__(self):
-        return str(self.value)+","
-    def get(self):
-        return self.value
-class CollectionRange(CollectionLiteralPart):
-    def __init__(self, name):
-        super().__init__(name)
-        self.first = None
-        self.last = None
+    def set_pre(self,pre):
+        self.pre=pre
+    def get_pre(self):
+        return self.pre
+    def create_property (self,prop):
+        return self.factory.create_property_Call_Expression(prop,"NP")
+    def handle_property(self,prop):
+        self.add_to_root(self.factory.create_property_Call_Expression(prop,"NP"))
+
+    def get_root(self):
+        return self.root
+    def get_context_name(self):
+        return self.context_name
+    def set_context_name(self,name):
+        self.context_name = name
+    def create_if_else_exp(self,name,type):
+        self.if_else_roots.append(None)
+        return self.factory.create_if_else_exp(name,type)
+    def pop(self):
+        if len(self.all)!=0:
+            self.add_to_root(self.all.pop())
+    def checkNumberOrVariable(self, txt):
+        if txt.isnumeric():
+            if "." in txt:
+                return "real"
+            else:
+                return "int"
+        elif "'" in txt:
+            return "str"
+        elif txt == "True" or txt == "False":
+            return "bool"
+        else:
+            return "var"
+
+    def _add_root(self,root,op):
+        if len(self.all) == 0:
+            if root is None:
+                root = op
+            else:
+                op.source = root
+                root = op
+        else:
+            self.all[-1].add_body(op)
+        return root
+    def getTop(self,last = False):
+        currentHead = self.if_else_roots.pop()
+        if not last:
+            self.if_else_roots.append(None)
+        return currentHead
+    def add_to_root(self, op):
+        self.last_added = op
+        if len(self.if_else_roots) != 0:
+            self.if_else_roots.append(self._add_root(self.if_else_roots.pop(),op))
+            pass
+        else:
+            self.root = self._add_root(self.root, op)
+        pass
+    def pop_root(self,root):
+
+        if self.root == self.last_coll_exp:
+            self.root = None
+            return self.last_coll_exp
+        if hasattr(root, "arguments"):
+            if self.last_coll_exp in root.arguments:
+                root.arguments.remove(self.last_coll_exp)
+                return self.last_coll_exp
+            for args in root.arguments:
+                self.pop_root(args)
+
+    def print(self):
+        self.handlePrint(self.root)
+    def handle_ID(self,id):
+        varID =self.factory.create_variable_expression(id,None)
+        self.add_to_root(varID)
+        # print('\x1b[6;30;42m' + 'handled ID, verify me!!!' + '\x1b[0m')
+        pass
+    def create_ordered_set(self):
+        type = self.factory.create_ordered_set_type()
+        return self.factory.create_collection_literal_expression("orderedSet", type)
+
+    def create_set(self):
+        type = self.factory.create_set_type()
+        return self.factory.create_collection_literal_expression("set", type)
+
+    def create_sub_ordered_set(self):
+        type = self.factory.create_ordered_set_type()
+        return self.factory.create_collection_literal_expression("subOrderedSet", type)
+    def create_sequence(self):
+        type = self.factory.create_sequence_type ()
+        return self.factory.create_collection_literal_expression("sequence",type)
+    def create_sub_sequence(self):
+        type = self.factory.create_sub_sequence_type ()
+        return self.factory.create_collection_literal_expression("subsequence",type)
+
+    def create_bag(self):
+        type = self.factory.create_bag_type()
+        return self.factory.create_collection_literal_expression("bag",type = type)
+
+    def create_type_exp(self,classifier):
+        return self.factory.create_type_exp(classifier)
+
+    def create_infinix_op(self,op):
+        self.factory.create_infix_operator(op)
+    def handle_and_with_function_call(self, text):
+        op = None
+        inF = None
+        if text[0:3] == "and":
+            inF = self.factory.create_infix_operator("AND")
+            op = self.factory.create_operation_call_expression(name = "AND")
+        if text[0:2] == "or":
+            inF = self.factory.create_infix_operator("OR")
+            op = self.factory.create_operation_call_expression(name = "OR")
+        op.arguments.append(inF)
+        self.add_to_root(op)
+        pass
+    def create_operation_call_exp(self,name):
+        return self.factory.create_operation_call_expression(name=name)
+    def get_factory(self):
+        return self.factory
+    def handle_bag(self,  collectionLiteral, operator):
+        infixOperator = None
+        if operator is not None:
+            infixOperator = self.factory.create_infix_operator(operator)
+
+        if infixOperator is not None:
+            operationCallExp = self.factory.create_operation_call_expression(None,collectionLiteral,infixOperator,None,True)
+
+        self.add_to_root(operationCallExp)
+    def handle_adding_to_root(self, expression, op=None):
+        if op is not None:
+            expression.referredOperation(op)
+        self.add_to_root(expression)
+        pass
+    def handlePrimaryExp(self,primaryExp,operator):
+        pass
+
+    def handle_collection(self,oclExp):
+
+        collectionOperator = None
+        if "forAll" in oclExp[0:8]:
+            collectionOperator = "forAll"
+            pass
+        elif "exists" in oclExp[0:8]:
+            collectionOperator = "exists"
+            pass
+        elif "collect" in oclExp[0:9]:
+            collectionOperator = "collect"
+            pass
+        elif "select" in oclExp[0:8]:
+            collectionOperator = "select"
+            pass
+
+        # print("Collection Operator: " + collectionOperator)
+        self.handleColl(oclExp,collectionOperator)
+
+        pass
+    def handle_single_variable(self, variable_name,sign):
+        op = self.factory.create_operation_call_expression(name = "operation")
+        infinix_op = self.factory.create_infix_operator(sign)
+        prop = self.factory.create_property_Call_Expression(variable_name,"NI")
+        op.arguments.append(infinix_op)
+        op.arguments.append(prop)
+        self.add_to_root(op)
+        pass
+    def verify(self,item):
+        referredOP= None
+        if 'and' in item[0:3]:
+            item = item[3:]
+            referredOP= 'AND'
+        if 'or' in item[0:2]:
+            item = item[2:]
+            referredOP = 'OR'
+        prop = self.factory.create_property_Call_Expression(item, 'NI')
+        if referredOP is None:
+            # prop= self.factory.create_property_Call_Expression(item,'NI')
+            self.add_to_root(prop)
+        else:
+            opCallExp = self.factory.create_operation_call_expression(name="and")
+            opCallExp.referredOperation = self.factory.create_infix_operator(referredOP)
+            self.add_to_root(opCallExp)
+        pass
+    def getClass(self,name):
+        for type in self.dm.types:
+            if name == type.name:
+                return type
+        raise Exception ("Class not found")
+        pass
+    def handleColl(self, forAllExp,collectionOperator):
+
+        self.all.append(self.factory.create_loop_expression(collectionOperator))
+        without_arrow = forAllExp.replace("->", '')
+        without_collOp = without_arrow.replace(collectionOperator+"(", '')
+        if "|" in without_collOp:
+            iterator = without_collOp.split("|")[0]
+            multiple_variable = iterator.split(',')
+            for variable in multiple_variable:
+                iteratorParts = variable.split(':')
+                iteratorVariableName = iteratorParts[0]
+                if ":" in variable:
+                    iteratorclass =self.getClass(iteratorParts[1])
+                else:
+                    iteratorclass = "NotMentioned"
+                iteratorExp = self.factory.create_iterator_expression(iteratorVariableName ,iteratorclass)
+                self.all[-1].addIterator(iteratorExp)
+
+
+        pass
+    def handle_binary_expression(self, expression, operator,inbetween= None,beforeSign = None):
+        expressionParts = expression.split(operator)
+
+        leftside = self.checkNumberOrVariable(expressionParts[0])
+        rightside = self.checkNumberOrVariable(expressionParts[1])
+
+        leftPart = None
+        rightPart = None
+
+        if "var" in leftside:
+            leftPart = self.factory.create_property_Call_Expression(expressionParts[0], type="NP",iterators=self.all)
+        elif "int" in leftside:
+            leftPart = self.factory.create_integer_literal_expression("NP", int(expressionParts[0]))
+        elif "real" in leftside:
+            leftPart = self.factory.create_real_literal_expression("NP", float(expressionParts[0]))
+        elif "bool" in leftside:
+            leftPart = self.factory.create_boolean_literal_expression("NP", bool(expressionParts[0]))
+        elif "str" in leftside:
+            leftPart = self.factory.create_string_literal_expression("str", expressionParts[0].replace("'",""))
+
+        if "var" in rightside:
+            rightPart = self.factory.create_property_Call_Expression(expressionParts[1], type="NP",iterators=self.all)
+        elif "int" in rightside:
+            rightPart = self.factory.create_integer_literal_expression("NP", int(expressionParts[1]))
+        elif "real" in rightside:
+            rightPart = self.factory.create_real_literal_expression("NP", float(expressionParts[1]))
+        elif "bool" in rightside:
+            rightPart = self.factory.create_boolean_literal_expression("NP", bool(expressionParts[1]))
+        elif "str" in rightside:
+            rightPart = self.factory.create_string_literal_expression("str", expressionParts[1].replace("'",""))
+
+        infixOperator = self.factory.create_infix_operator(operator)
+        beforeOp = None
+        if beforeSign is not None:
+            beforeOp = self.factory.create_infix_operator(beforeSign)
+        inBetweenOp = None
+        if inbetween is not None and len(inbetween)>0:
+            inBetweenOp = self.factory.create_infix_operator(inbetween)
+        opeartion_call_exp = self.factory.create_operation_call_expression(leftPart, rightPart, infixOperator,
+                                                                           inBetweenOp,beforeOp)
+        self.add_to_root(opeartion_call_exp)
+
+
+        pass
+    def handleBinaryFunc(self,operator,number):
+
+        num = self.checkNumberOrVariable(number)
+
+        if "int" in num:
+            rightPart = self.factory.create_integer_literal_expression("NP", int(number))
 
+        if "real" in num:
+            rightPart = self.factory.create_real_literal_expression("NP", float(number))
+        op = self.factory.create_infix_operator(operator)
+        self.last_added.arguments.append(op)
+        self.last_added.arguments.append(rightPart)
+
+    def handle_last_opnum(self,operator,number):
+        op= self.factory.create_operation_call_expression(name='callExp')
+        op.arguments.append(self.factory.create_infix_operator(operator))
+        num = self.checkNumberOrVariable(number)
+
+        if "int" in num:
+           rightPart = self.factory.create_integer_literal_expression("NP", int(number))
+
+        if "real" in num:
+            rightPart = self.factory.create_real_literal_expression("NP", float(number))
+
+        op.arguments.append(
+            rightPart
+        )
+        self.add_to_root(op)
+    def handlePrint(self, root):
+        if root == None:
+            return
+        if hasattr(root, 'arguments'):
+            print(root.arguments)
+            print(root.referredOperation())
+            self.handlePrint(root.source())
+
+        if hasattr(root,'body'):
+            print(root.name)
+            print(root.iterator)
+            for item in root.body:
+                print(item)
```

### Comparing `besser-1.0.1/besser/BUML/metamodel/structural/structural.py` & `besser-1.1.0/besser/BUML/metamodel/structural/structural.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,40 +298,36 @@
         name (str): The name of the property.
         property_type (Type): The type of the property.
         owner (Type): The type that owns the property.
         multiplicity (Multiplicity): The multiplicity of the property.
         visibility (str): The visibility of the property ('public', 'private', etc.).
         is_composite (bool): Indicates whether the property is a composite.
         is_navigable (bool): Indicates whether the property is navigable in a relationship.
-        is_aggregation (bool): Indicates whether the property represents an aggregation.
         is_id (bool): Indicates whether the property is an id.
         is_read_only (bool): Indicates whether the property is read only.
 
     Attributes:
         name (str): Inherited from TypedElement, represents the name of the property.
         property_type (Type): Inherited from TypedElement, represents the type of the property.
         owner (Type): The type that owns the property.
         multiplicity (Multiplicity): The multiplicity of the property.
         visibility (str): Inherited from TypedElement, represents the visibility of the property.
         is_composite (bool): Indicates whether the property is a composite.
         is_navigable (bool): Indicates whether the property is navigable in a relationship.
-        is_aggregation (bool): Indicates whether the property represents an aggregation.
         is_id (bool): Indicates whether the property is an id.
         is_read_only (bool): Indicates whether the property is read only.
     """
     
     def __init__(self, name: str, property_type: Type, owner: Type = None, multiplicity: Multiplicity = Multiplicity(1, 1), 
-                 visibility: str = 'public', is_composite: bool = False, is_navigable: bool = True, is_aggregation: bool = False,
-                 is_id: bool = False, is_read_only: bool = False):
+                 visibility: str = 'public', is_composite: bool = False, is_navigable: bool = True, is_id: bool = False, is_read_only: bool = False):
         super().__init__(name, property_type, visibility)
         self.owner: Type = owner
         self.multiplicity: Multiplicity = multiplicity
         self.is_composite: bool = is_composite
         self.is_navigable: bool = is_navigable
-        self.is_aggregation: bool = is_aggregation
         self.is_id: bool = is_id
         self.is_read_only: bool = is_read_only
 
     @property
     def owner(self) -> Type:
         """Type: Get the owner type of the property."""
         return self.__owner
@@ -373,24 +369,14 @@
         """bool: Get wheter the property is navigable."""
         return self.__is_navigable
 
     @is_navigable.setter
     def is_navigable(self, is_navigable: bool):
         """bool: Set wheter the property is navigable."""
         self.__is_navigable = is_navigable
-
-    @property
-    def is_aggregation(self) -> bool:
-        """bool: Get wheter the property represents an aggregation."""
-        return self.__is_aggregation
-
-    @is_aggregation.setter
-    def is_aggregation(self, is_aggregation: bool):
-        """bool: Set wheter the property represents an aggregation."""
-        self.__is_aggregation = is_aggregation
     
     @property
     def is_id(self) -> bool:
         """bool: Get wheter the property is an id."""
         return self.__is_id
 
     @is_id.setter
@@ -671,16 +657,14 @@
         
         Raises:
             ValueError: if the associaiton ends are not exactly two, or if both ends are tagged as agregation, or 
             if both ends are tagged as composition.
         """
         if len(ends) != 2:
             raise ValueError("A binary must have exactly two ends")
-        if list(ends)[0].is_aggregation == True and list(ends)[1].is_aggregation == True:
-            raise ValueError("The aggregation attribute cannot be tagged at both ends")
         if list(ends)[0].is_composite == True and list(ends)[1].is_composite == True:
             raise ValueError("The composition attribute cannot be tagged at both ends")
         super(BinaryAssociation, BinaryAssociation).ends.fset(self, ends)
 
     def __repr__(self):
         return f'BinaryAssociation({self.name}, {self.ends})'
```

### Comparing `besser-1.0.1/besser/BUML/notations/objectPlantUML/ODLexer.py` & `besser-1.1.0/besser/BUML/notations/objectPlantUML/ODLexer.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/objectPlantUML/ODListener.py` & `besser-1.1.0/besser/BUML/notations/objectPlantUML/ODListener.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/objectPlantUML/ODParser.py` & `besser-1.1.0/besser/BUML/notations/objectPlantUML/ODParser.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/ocl/BOCLLexer.py` & `besser-1.1.0/besser/BUML/notations/ocl/BOCLLexer.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/ocl/BOCLListener.py` & `besser-1.1.0/besser/BUML/notations/ocl/BOCLListener.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/ocl/BOCLParser.py` & `besser-1.1.0/besser/BUML/notations/ocl/BOCLParser.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/ocl/FactoryInstance.py` & `besser-1.1.0/besser/BUML/notations/ocl/FactoryInstance.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/ocl/OCLWrapper.py` & `besser-1.1.0/besser/BUML/notations/ocl/OCLWrapper.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py` & `besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py` & `besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py` & `besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py` & `besser-1.1.0/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py` & `besser-1.1.0/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/generators/django/django_generator.py` & `besser-1.1.0/besser/generators/django/django_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/generators/django/templates/django_fields.py.j2` & `besser-1.1.0/besser/generators/django/templates/django_fields.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/generators/django/templates/django_template.py.j2` & `besser-1.1.0/besser/generators/sql/templates/sql_template.sql.j2`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-{# Django model template generator #}
-{% import "django_fields.py.j2" as django_fields %}
-{# django_fields.j2 should contain mappings to Django's ORM field types #}
-from django.db import models
-
-{% set processed_associations = [] %}
+{% import "sql_dialects.sql.j2" as sql_templates %}
+{# Iterate over classes and generate CREATE TABLE statements #}
 {% for class_obj in model.classes_sorted_by_inheritance() %}
-    {% set generals = namespace(names=[]) %}
-    {% for parent in class_obj.parents() %}
-        {% set _ = generals.names.append(parent.name) %}
-    {% endfor %}
-    {% set inheritance = generals.names | join(', ') %}
-class {{ class_obj.name }}({{ inheritance | default('models.Model', true) }}):
-    {% for attr in class_obj.attributes %}
-    {{ attr.name }} = {{ django_fields.get_field(attr.type.name, attr.properties) }}
-    {%- endfor %}
-    {% for association in class_obj.associations %}
-        {% if association.ends|length == 2 and association.name not in processed_associations %}
-            {% set ns = namespace(end1=None, end2=None) %}
-            {% for end in association.ends %}
-                {% set ns.end1=end if end.type.name == class_obj.name else ns.end1 %}
-                {% set ns.end2=end if end.type.name != class_obj.name else ns.end2 %}
-            {% endfor %}
-            {% set class1_name = ns.end1.type.name %}
-            {% set class2_name = ns.end2.type.name %}
-            {% if ns.end1.multiplicity.max > 1 and ns.end2.multiplicity.max > 1 %}
-            {# N:M Relationship: Use ManyToManyField in Django #}
-    {{ class2_name.lower() }} = models.ManyToManyField('{{ class2_name }}')
-                {% do processed_associations.append(association.name) %}
-            {% elif ns.end1.multiplicity.max > 1 and ns.end2.multiplicity.max == 1 %}
-            {# N:1 Relationship: Use ForeignKey in Django #}
-    {{ class2_name.lower() }} = models.ForeignKey('{{ class2_name }}', on_delete=models.CASCADE)
-                {% do processed_associations.append(association.name) %}
-            {% elif ns.end1.multiplicity.max == 1 and ns.end2.multiplicity.max == 1 %}
-            {# 1:1 Relationship: Use OneToOneField in Django #}
-    {{ class2_name.lower() }} = models.OneToOneField('{{ class2_name }}', on_delete=models.CASCADE)
-                {% do processed_associations.append(association.name) %}
+    {% set class_name = class_obj.name %}
+    {% set attributes = class_obj.attributes %}
+    {{- sql_templates.create_table(class_name, attributes, types, sql_dialect) }}
+    {# Handling generalizations (inheritance) #}
+    {% if class_obj.generalizations %}
+        {% for generalization in class_obj.generalizations %}
+            {% if generalization.specific.name == class_name %}
+                {{- sql_templates.add_generalization(class_name, generalization, sql_dialect) }}
             {% endif %}
-        {% endif %}
-    {% endfor %}
-
-    def __str__(self):
-        return str(self.id)
-
+        {% endfor %}
+    {% endif %}
 {% endfor %}
-
+{# Iterate over associations and generate SQL statements based on association type #}
 {% for association in model.associations %}
-    {% if association.name not in processed_associations %}
-{# Nary relationship handling (intermediate table) #}
-class {{ association.name|capitalize }}(models.Model):
+    {% if association.ends|length == 2 -%}
+        {% set ns = namespace(end1=None, end2=None) %}
+        {% for end in association.ends %}
+            {% set ns.end1=end if loop.index == 1 else ns.end1 %}
+            {% set ns.end2=end if loop.index == 2 else ns.end2 %}
+        {% endfor %}
+        {% set class1_name = ns.end1.type.name %}
+        {% set class2_name = ns.end2.type.name %}
+        {# Check multiplicity and generate appropriate SQL statement #}
+        {% if ns.end1.multiplicity.max > 1 and ns.end2.multiplicity.max > 1 %}
+        {# N:M Relationship: Create intermediate table #}
+            {{- sql_templates.create_nm_table(class1_name, class2_name, sql_dialect) }}
+        {% elif ns.end1.multiplicity.max > 1 and ns.end2.multiplicity.max == 1 %}
+        {# N:1 Relationship: Add reference to Nary end #}
+            {{- sql_templates.alter_table(class1_name, class2_name, class2_name, class2_name, sql_dialect) }}
+        {% elif ns.end1.multiplicity.max == 1 and ns.end2.multiplicity.max > 1 %}
+        {# 1:N Relationship: Add reference to Nary end #}
+            {{- sql_templates.alter_table(class2_name, class1_name, class1_name, class1_name, sql_dialect) }}
+        {% elif ns.end1.multiplicity.max == 1 and ns.end2.multiplicity.max == 1 %}
+        {# 1:1 Relationship: Add unique reference to one of the ends #}
+            {{- sql_templates.alter_table(class1_name, class2_name, class2_name, class2_name, sql_dialect) }}
+        {% endif %}
+    {% else %}
+    {# Convert Nary relationship to Binary relationships and intermediate table #}
+        {% set intermediate_class = association.name %}
+        {{- sql_templates.create_table(intermediate_class, [], types, sql_dialect) }}
+        {% set end_intermediate_multiplicity_max = 9999 %}
         {% for end in association.ends %}
-            {% set class_name = end.type.name %}
-            {% if end.multiplicity.max > 1 %}
-                {# N:M Relationship: Use ManyToManyField in Django  intermediate table #}
-    {{ class_name.lower() }} = models.ManyToManyField({{ class_name }})
-            {% else %}
-                {# 1:N Relationship: Use ForeignKey in Django  intermediate table #}
-    {{ class_name.lower() }} = models.ForeignKey({{ class_name }}, on_delete=models.CASCADE)
+            {# Check multiplicity and generate appropriate SQL statement #}
+            {% set class1_name = intermediate_class %}
+            {% set class2_name = end.type.name %}
+            {# End of intermediate table should have multiplicity of the original end to the class #}
+            {% if end.multiplicity.max > 1 and end_intermediate_multiplicity_max > 1 %}
+            {# N:M Relationship: Create intermediate table #}
+                {{- sql_templates.create_nm_table(class1_name, class2_name, sql_dialect) }}
+            {% elif end.multiplicity.max == 1 and end_intermediate_multiplicity_max > 1 %}
+                {# 1:N Relationship: Add reference to Nary end #}
+                {{- sql_templates.alter_table(class1_name, class2_name, class2_name, class2_name, sql_dialect) }}
             {% endif %}
         {% endfor %}
     {% endif %}
-
-{% endfor %}
+{%- endfor %}
```

### Comparing `besser-1.0.1/besser/generators/generator_interface.py` & `besser-1.1.0/besser/generators/generator_interface.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/generators/python_classes/python_classes_generator.py` & `besser-1.1.0/besser/generators/python_classes/python_classes_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from jinja2 import Environment, FileSystemLoader
 from besser.BUML.metamodel.structural import DomainModel
 from besser.generators import GeneratorInterface
 
-class Python_Generator(GeneratorInterface):
+class PythonGenerator(GeneratorInterface):
     """
-    Python_Generator is a class that implements the GeneratorInterface and is responsible for generating
+    PythonGenerator is a class that implements the GeneratorInterface and is responsible for generating
     the Python domain model code based on the input B-UML model.
 
     Args:
         model (DomainModel): An instance of the DomainModel class representing the B-UML model.
         output_dir (str, optional): The output directory where the generated code will be saved. Defaults to None.
     """
     def __init__(self, model: DomainModel, output_dir: str = None):
```

### Comparing `besser-1.0.1/besser/generators/python_classes/templates/class_parameters.py.j2` & `besser-1.1.0/besser/generators/python_classes/templates/class_parameters.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/generators/python_classes/templates/python_classes_template.py.j2` & `besser-1.1.0/besser/generators/python_classes/templates/python_classes_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/generators/rest_api/rest_api_generator.py` & `besser-1.1.0/besser/generators/backend/backend_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,59 @@
 import os
 from jinja2 import Environment, FileSystemLoader
 from besser.BUML.metamodel.structural import DomainModel
 from besser.generators import GeneratorInterface
+from besser.generators.rest_api import RESTAPIGenerator
+from besser.generators.sql_alchemy import SQLAlchemyGenerator
+from besser.generators.pydantic_classes import PydanticGenerator
 
-class RESTAPIGenerator(GeneratorInterface):
+
+class BackendGenerator(GeneratorInterface):
     """
-    Rest_API_Generator is a class that implements the GeneratorInterface and is responsible for generating
-    the Rest API domain model code based on the input B-UML model. This version of the generator allows
-    specifying which HTTP methods (e.g., GET, POST, PATCH) should be included in the generated code. It can
-    generate code for one or more specified methods, enabling more customizable API endpoint generation.
+    BackendGenerator is a class that implements the GeneratorInterface and is responsible for generating
+    a Backend model code with a REST API using FAST API framework, SQLAlchemy and a Pydantic model based on the input B-UML model .
 
     Args:
         model (DomainModel): An instance of the DomainModel class representing the B-UML model.
-        http_methods (list): A list of strings representing the HTTP methods for which code should be generated.
-                         Each element should be one of "GET", "POST", "PUT","PATCH","DELETE". This allows generating
-                         only the parts of the API that are needed.
+        http_methods (list, optional): A list of HTTP methods to be used in the REST API. Defaults to All.
+        nested_creations (bool, optional): This parameter specifies how entities are linked in the API request. If set to True, the API expects 
+                                identifiers and links entities based on these IDs. If set to False, the API handles the creation of 
+                                new entities based on the data provided in the request. Defaults to True
         output_dir (str, optional): The output directory where the generated code will be saved. Defaults to None.
     """
-    def __init__(self, model: DomainModel, http_methods: list = None, output_dir: str = None):
+
+    def __init__(self, model: DomainModel, http_methods: list = None, nested_creations: bool = False, output_dir: str = None):
+        if output_dir is None:
+            output_dir = os.getcwd()  # set to current directory if output_dir is None
         super().__init__(model, output_dir)
-        allowed_methods = ["GET", "POST", "PUT", "PATCH", "DELETE"]
+        allowed_methods = ["GET", "POST", "PUT", "DELETE"]
         if not http_methods:
             http_methods = allowed_methods
         else:
             http_methods = [method for method in http_methods if method in allowed_methods]
         self.http_methods = http_methods
+        self.nested_creations = nested_creations
 
     def generate(self):
         """
-        Generates Rest API model code based on the provided B-UML model and saves it to the specified output directory.
-        If the output directory was not specified, the code generated will be stored in the <current directory>/output
+        Generates Backend model code based on the provided B-UML model and saves it to the specified output directory.
+        If the output directory was not specified, the code generated will be stored in the <current directory>/output_backend
         folder.
 
         Returns:
-            None, but store the generated code as a file named rest_api.py 
+            None, but store the generated code as files main_api.py, sql_alchemy.py and pydantic_classes.py
         """
-        file_path = self.build_generation_path(file_name="rest_api.py")
-        templates_path = os.path.join(os.path.dirname(
-            os.path.abspath(__file__)), "templates")
-        env = Environment(loader=FileSystemLoader(templates_path),
-                           trim_blocks=True, lstrip_blocks=True, extensions=['jinja2.ext.do'])
-        template = env.get_template('fast_api_template.py.j2')
-        with open(file_path, mode="w") as f:
-            generated_code = template.render(classes=self.model.classes_sorted_by_inheritance(), http_methods=self.http_methods)
-            f.write(generated_code)
-            print("Code generated in the location: " + file_path)
+        if self.output_dir is ".":
+            backend_folder_path = "."
+        else:
+            backend_folder_path = os.path.join(self.output_dir, "output_backend")
+            os.makedirs(backend_folder_path, exist_ok=True)
+            print(f"Backend folder created at {backend_folder_path}")
+
+        rest_api = RESTAPIGenerator(model=self.model, http_methods=self.http_methods, nested_creations=self.nested_creations, output_dir=backend_folder_path, backend=True)
+        rest_api.generate()
+
+        sql_alchemy = SQLAlchemyGenerator(model=self.model, output_dir=backend_folder_path)
+        sql_alchemy.generate()
+
+        pydantic_model = PydanticGenerator(model=self.model, output_dir=backend_folder_path, backend=True, nested_creations=self.nested_creations)
+        pydantic_model.generate()
```

### Comparing `besser-1.0.1/besser/generators/sql/sql_generator.py` & `besser-1.1.0/besser/generators/sql/sql_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/generators/sql/templates/sql_dialects.sql.j2` & `besser-1.1.0/besser/generators/sql/templates/sql_dialects.sql.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/generators/sql_alchemy/sql_alchemy_generator.py` & `besser-1.1.0/besser/generators/sql_alchemy/sql_alchemy_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2` & `besser-1.1.0/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2`

 * *Files 2% similar despite different names*

```diff
@@ -85,12 +85,13 @@
         {%- if end.multiplicity.max > 1 %}
 {{class.name}}.{{end.name}}: Mapped[List["{{end.type.name}}"]] = relationship("{{end.type.name}}"
             {%- if ns.end_own.multiplicity.max > 1 -%}
                 , secondary={{ end.owner.name.lower() }}
             {%- endif %}, back_populates="{{ns.end_own.name}}")
         {%- endif %}
         {%- if end.multiplicity.max == 1 %}
-{{class.name}}.{{end.type.name.lower()}}_id: Mapped["{{end.type.name}}"] = mapped_column(ForeignKey("{{end.type.name.lower()}}.id"))
+{{class.name}}.{{end.type.name.lower()}}_id: Mapped["{{end.type.name}}"] = mapped_column(ForeignKey("{{end.type.name.lower()}}.id")
+{%- if end.multiplicity.min > 0 %}, nullable=False{% endif %})
 {{class.name}}.{{end.name}}: Mapped["{{end.type.name}}"] = relationship("{{end.type.name}}", back_populates="{{ns.end_own.name}}")
         {%- endif %}
     {%- endfor %}
 {%- endfor %}
```

### Comparing `besser-1.0.1/besser/utilities/image_to_buml.py` & `besser-1.1.0/besser/utilities/image_to_buml.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,18 @@
         }
         ],
         "max_tokens": 500
     }
 
     response = requests.post("https://api.openai.com/v1/chat/completions", headers=headers, json=payload)
     response_data = json.loads(response.text)
-
+    if ('error' in response_data):
+        print("An error took place during the request to transform your given image:")
+        print(response_data['error']['message'])
+        return
     # Extracting the message
     messages = [choice['message'] for choice in response_data.get('choices', {})]
     message = messages[0]["content"]
     # Find the start and end positions of the desired chunk
     start_position = message.find("@startuml")
     end_position = message.find("@enduml", start_position)
```

### Comparing `besser-1.0.1/besser/utilities/utils.py` & `besser-1.1.0/besser/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/besser.egg-info/PKG-INFO` & `besser-1.1.0/besser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besser
-Version: 1.0.1
+Version: 1.1.0
 Summary: BESSER
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besser.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER/issues
 Keywords: uml,code generation,python
@@ -20,14 +20,16 @@
 Requires-Dist: textX==3.1.1
 Requires-Dist: jinja2==3.1.2
 Requires-Dist: antlr4-python3-runtime==4.13.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: fastapi==0.110.0
 Requires-Dist: pydantic==2.6.3
 Requires-Dist: uvicorn==0.28.0
+Requires-Dist: SQLAlchemy==2.0.29
+Requires-Dist: httpx==0.27.0
 
 # BESSER
 
 BESSER is a [low-modeling](https://modeling-languages.com/welcome-to-the-low-modeling-revolution/) [low-code](https://modeling-languages.com/low-code-vs-model-driven/) open-source platform. BESSER (Building bEtter Smart Software fastER) is funded thanks to an [FNR Pearl grant](https://modeling-languages.com/a-smart-low-code-platform-for-smart-software-in-luxembourg-goodbye-barcelona/) led by the [Luxembourg Institute of Science and Technology](https://www.list.lu/) with the participation of the [Snt/University of Luxembourg](https://www.uni.lu/snt-en/) and open to all your contributions!
 
 The BESSER low-code platform is built on top of our Python-based personal interpretation of a "Universal Modeling Language" (yes, heavily inspired and a simplified version of the better known UML, the Unified Modeling Language)
```

### Comparing `besser-1.0.1/besser.egg-info/SOURCES.txt` & `besser-1.1.0/besser.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -34,27 +34,34 @@
 besser/BUML/notations/structuralPlantUML/PlantUMLListener.py
 besser/BUML/notations/structuralPlantUML/PlantUMLParser.py
 besser/BUML/notations/structuralPlantUML/__init__.py
 besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py
 besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py
 besser/generators/__init__.py
 besser/generators/generator_interface.py
+besser/generators/backend/__init__.py
+besser/generators/backend/backend_generator.py
 besser/generators/django/__init__.py
 besser/generators/django/django_generator.py
 besser/generators/django/templates/__init__.py
 besser/generators/django/templates/django_fields.py.j2
 besser/generators/django/templates/django_template.py.j2
+besser/generators/pydantic_classes/__init__.py
+besser/generators/pydantic_classes/pydantic_classes_generator.py
+besser/generators/pydantic_classes/templates/__init__.py
+besser/generators/pydantic_classes/templates/pydantic_classes_template.py.j2
 besser/generators/python_classes/__init__.py
 besser/generators/python_classes/python_classes_generator.py
 besser/generators/python_classes/templates/__init__.py
 besser/generators/python_classes/templates/class_parameters.py.j2
 besser/generators/python_classes/templates/python_classes_template.py.j2
 besser/generators/rest_api/__init__.py
 besser/generators/rest_api/rest_api_generator.py
 besser/generators/rest_api/templates/__init__.py
+besser/generators/rest_api/templates/backend_fast_api_template.py.j2
 besser/generators/rest_api/templates/fast_api_template.py.j2
 besser/generators/sql/__init__.py
 besser/generators/sql/sql_generator.py
 besser/generators/sql/templates/__init__.py
 besser/generators/sql/templates/sql_dialects.sql.j2
 besser/generators/sql/templates/sql_template.sql.j2
 besser/generators/sql_alchemy/__init__.py
```

### Comparing `besser-1.0.1/setup.cfg` & `besser-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6573 7365 720d 0a76 6572 7369   = besser..versi
-00000020: 6f6e 203d 2031 2e30 2e31 0d0a 6175 7468  on = 1.0.1..auth
+00000020: 6f6e 203d 2031 2e31 2e30 0d0a 6175 7468  on = 1.1.0..auth
 00000030: 6f72 203d 204c 7578 656d 626f 7572 6720  or = Luxembourg 
 00000040: 496e 7374 6974 7574 6520 6f66 2053 6369  Institute of Sci
 00000050: 656e 6365 2061 6e64 2054 6563 686e 6f6c  ence and Technol
 00000060: 6f67 790d 0a64 6573 6372 6970 7469 6f6e  ogy..description
 00000070: 203d 2042 4553 5345 520d 0a6c 6f6e 675f   = BESSER..long_
 00000080: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000090: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
```

### Comparing `besser-1.0.1/tests/gui/gui_model.py` & `besser-1.1.0/tests/gui/gui_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from besser.BUML.metamodel.gui import *
 from besser.BUML.metamodel.structural import *
-from besser.generators.python_classes import Python_Generator
+from besser.generators.python_classes import PythonGenerator
 from besser.generators.django import DjangoGenerator
 from besser.generators.sql_alchemy import SQLAlchemyGenerator
 from besser.generators.sql import SQLGenerator
 
 
 ###################################################
 #   Library class - structural model definition   #
```

### Comparing `besser-1.0.1/tests/gui/test_gui.py` & `besser-1.1.0/tests/gui/test_gui.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/tests/object/library_object.py` & `besser-1.1.0/tests/object/library_object.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/tests/object/test_object_mm.py` & `besser-1.1.0/tests/object/test_object_mm.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/tests/ocl/test_ocl_parser.py` & `besser-1.1.0/tests/ocl/test_ocl_parser.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.1/tests/structural/test_structural.py` & `besser-1.1.0/tests/structural/test_structural.py`

 * *Files identical despite different names*

