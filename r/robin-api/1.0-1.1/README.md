# Comparing `tmp/robin_api-1.0.tar.gz` & `tmp/robin_api-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin_api-1.0.tar", last modified: Wed May  1 19:57:46 2024, max compression
+gzip compressed data, was "robin_api-1.1.tar", last modified: Wed May  1 20:15:58 2024, max compression
```

## Comparing `robin_api-1.0.tar` & `robin_api-1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 19:57:46.747012 robin_api-1.0/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    11337 2024-04-30 18:06:24.000000 robin_api-1.0/LICENSE
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      210 2024-05-01 19:41:22.000000 robin_api-1.0/MANIFEST.in
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     4539 2024-05-01 19:57:46.747012 robin_api-1.0/PKG-INFO
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     4092 2024-05-01 19:32:03.000000 robin_api-1.0/README.md
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 19:57:46.743012 robin_api-1.0/robin_api/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      765 2024-05-01 02:52:51.000000 robin_api-1.0/robin_api/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     6473 2024-05-01 04:43:31.000000 robin_api-1.0/robin_api/_client.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5102 2024-04-30 23:37:44.000000 robin_api-1.0/robin_api/_compat.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      404 2024-04-30 23:05:14.000000 robin_api-1.0/robin_api/_constants.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3573 2024-04-30 20:26:30.000000 robin_api-1.0/robin_api/_exceptions.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    18240 2024-05-01 18:18:56.000000 robin_api-1.0/robin_api/_models.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      881 2024-05-01 04:56:26.000000 robin_api-1.0/robin_api/_resource.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     7217 2024-04-30 23:44:46.000000 robin_api-1.0/robin_api/_streaming.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     9696 2024-04-30 23:36:19.000000 robin_api-1.0/robin_api/_types.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 19:57:46.743012 robin_api-1.0/robin_api/_utils/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      219 2024-05-01 02:38:52.000000 robin_api-1.0/robin_api/_utils/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1553 2024-05-01 02:38:37.000000 robin_api-1.0/robin_api/_utils/_utils.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 19:57:46.747012 robin_api-1.0/robin_api/resources/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      139 2024-05-01 00:03:13.000000 robin_api-1.0/robin_api/resources/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3660 2024-05-01 18:32:37.000000 robin_api-1.0/robin_api/resources/completions.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 19:57:46.747012 robin_api-1.0/robin_api/types/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      692 2024-05-01 17:26:33.000000 robin_api-1.0/robin_api/types/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1139 2024-05-01 16:49:41.000000 robin_api-1.0/robin_api/types/completion.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      401 2024-05-01 00:30:19.000000 robin_api-1.0/robin_api/types/completion_usage.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 19:57:46.747012 robin_api-1.0/robin_api.egg-info/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      456 2024-05-01 19:57:46.000000 robin_api-1.0/robin_api.egg-info/SOURCES.txt
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)       38 2024-05-01 19:57:46.747012 robin_api-1.0/setup.cfg
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      673 2024-05-01 19:57:41.000000 robin_api-1.0/setup.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:15:58.699107 robin_api-1.1/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    11337 2024-04-30 18:06:24.000000 robin_api-1.1/LICENSE
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      210 2024-05-01 19:41:22.000000 robin_api-1.1/MANIFEST.in
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     2958 2024-05-01 20:15:58.699107 robin_api-1.1/PKG-INFO
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     2511 2024-05-01 20:03:11.000000 robin_api-1.1/README.md
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:15:58.695107 robin_api-1.1/robin_api/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      765 2024-05-01 02:52:51.000000 robin_api-1.1/robin_api/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     6473 2024-05-01 04:43:31.000000 robin_api-1.1/robin_api/_client.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5102 2024-04-30 23:37:44.000000 robin_api-1.1/robin_api/_compat.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      404 2024-04-30 23:05:14.000000 robin_api-1.1/robin_api/_constants.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3573 2024-04-30 20:26:30.000000 robin_api-1.1/robin_api/_exceptions.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    18240 2024-05-01 18:18:56.000000 robin_api-1.1/robin_api/_models.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      881 2024-05-01 04:56:26.000000 robin_api-1.1/robin_api/_resource.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     7217 2024-04-30 23:44:46.000000 robin_api-1.1/robin_api/_streaming.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     9696 2024-04-30 23:36:19.000000 robin_api-1.1/robin_api/_types.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:15:58.695107 robin_api-1.1/robin_api/_utils/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      219 2024-05-01 02:38:52.000000 robin_api-1.1/robin_api/_utils/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1553 2024-05-01 02:38:37.000000 robin_api-1.1/robin_api/_utils/_utils.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:15:58.699107 robin_api-1.1/robin_api/resources/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      139 2024-05-01 00:03:13.000000 robin_api-1.1/robin_api/resources/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3830 2024-05-01 20:13:11.000000 robin_api-1.1/robin_api/resources/completions.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:15:58.699107 robin_api-1.1/robin_api/types/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      692 2024-05-01 17:26:33.000000 robin_api-1.1/robin_api/types/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1139 2024-05-01 16:49:41.000000 robin_api-1.1/robin_api/types/completion.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      401 2024-05-01 00:30:19.000000 robin_api-1.1/robin_api/types/completion_usage.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-01 20:15:58.699107 robin_api-1.1/robin_api.egg-info/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      456 2024-05-01 20:15:58.000000 robin_api-1.1/robin_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)       38 2024-05-01 20:15:58.699107 robin_api-1.1/setup.cfg
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      673 2024-05-01 20:15:57.000000 robin_api-1.1/setup.py
```

### Comparing `robin_api-1.0/LICENSE` & `robin_api-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/README.md` & `robin_api-1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,38 @@
-Nombre del Proyecto: RobinApi Framework
+# RobinApi Framework
 
-Descripción:
+**Descripción:**  
 RobinApi Framework es una solución integral diseñada para facilitar la interacción eficiente con APIs de modelos de lenguaje de aprendizaje automático (LLM) y la gestión avanzada de datos vectoriales. Este framework proporciona herramientas robustas para la carga y almacenamiento de archivos en una base de datos vectorial optimizada, permitiendo a los usuarios aprovechar completamente la búsqueda y recuperación de datos basados en contenido. Además, RobinApi Framework incluye endpoints dedicados para realizar consultas complejas, permitiendo a los usuarios extraer información valiosa y realizar análisis profundos sobre los datos almacenados. Ideal para desarrolladores que buscan integrar capacidades de LLM en sus aplicaciones y gestionar grandes volúmenes de datos de manera eficiente, RobinApi Framework se destaca por su flexibilidad, escalabilidad y facilidad de uso.
 
-Características principales:
+**Características principales:**
 
-Consumo de API de LLM: Interfaces optimizadas para la interacción con modelos de lenguaje, facilitando la integración y el manejo de respuestas en tiempo real.
-Gestión de archivos en base de datos vectorial: Carga, almacenamiento y gestión eficiente de archivos con búsqueda vectorial, ideal para aplicaciones que requieren acceso rápido y preciso a grandes volúmenes de datos.
-Endpoints para consultas: Funcionalidades específicas para formular preguntas y obtener respuestas basadas en los datos almacenados, soportando una amplia variedad de consultas analíticas y de búsqueda.
-Alta configurabilidad y seguridad: Configuración detallada de parámetros y protocolos de seguridad avanzados para proteger la información y garantizar el rendimiento.
-
-Project Name: RobinApi Framework
-
-Description:
-RobinApi Framework is a comprehensive solution designed to facilitate efficient interactions with machine learning language model (LLM) APIs and advanced vector data management. This framework provides robust tools for uploading and storing files in an optimized vector database, enabling users to fully leverage content-based data search and retrieval. Additionally, RobinApi Framework includes dedicated endpoints for conducting complex queries, allowing users to extract valuable information and perform in-depth analyses on stored data. Ideal for developers looking to integrate LLM capabilities into their applications and manage large volumes of data efficiently, RobinApi Framework stands out for its flexibility, scalability, and ease of use.
-
-Key Features:
-
-LLM API Consumption: Optimized interfaces for interacting with language models, facilitating integration and real-time response handling.
-File Management in Vector Database: Efficient upload, storage, and management of files with vector search, ideal for applications requiring fast and accurate access to large data volumes.
-Endpoints for Queries: Specific functionalities to ask questions and receive answers based on stored data, supporting a wide variety of analytical and search queries.
-High Configurability and Security: Detailed parameter settings and advanced security protocols to protect information and ensure performance.
-Ideal for:
-Software developers, data scientists, and system engineers interested in integrating LLM technology and advanced vector data management into their projects.
+- **Consumo de API de LLM:** Interfaces optimizadas para la interacción con modelos de lenguaje, facilitando la integración y el manejo de respuestas en tiempo real.
+- **Gestión de archivos en base de datos vectorial:** Carga, almacenamiento y gestión eficiente de archivos con búsqueda vectorial, ideal para aplicaciones que requieren acceso rápido y preciso a grandes volúmenes de datos.
+- **Endpoints para consultas:** Funcionalidades específicas para formular preguntas y obtener respuestas basadas en los datos almacenados, soportando una amplia variedad de consultas analíticas y de búsqueda.
+- **Alta configurabilidad y seguridad:** Configuración detallada de parámetros y protocolos de seguridad avanzados para proteger la información y garantizar el rendimiento.
 
+## Código de Ejemplo
 
+```python
 from robin_api import RobinAIClient
 
-
 client = RobinAIClient(api_key="API_KEY")
 
 value =  [
             {
                 "role": "system",
                 "content": "system_prompt"
             },
             {
                 "role": "user",
                 "content": "hola como estas, dame un poema de 100 palabras"
             }
-
 ]
 
 stream = client.completions.create(model="ROBIN_4", 
                             conversation = value, 
                             max_tokens = 512, stream = True, 
                             save_response = False,
                             temperature=1)
 for chunk in stream:
     if chunk.choices[0].delta.content is not None:
         print(chunk.choices[0].delta.content, end="")
-
-exit()
```

### Comparing `robin_api-1.0/robin_api/__init__.py` & `robin_api-1.1/robin_api/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/robin_api/_client.py` & `robin_api-1.1/robin_api/_client.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/robin_api/_compat.py` & `robin_api-1.1/robin_api/_compat.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/robin_api/_exceptions.py` & `robin_api-1.1/robin_api/_exceptions.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/robin_api/_models.py` & `robin_api-1.1/robin_api/_models.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/robin_api/_resource.py` & `robin_api-1.1/robin_api/_resource.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/robin_api/_streaming.py` & `robin_api-1.1/robin_api/_streaming.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/robin_api/_types.py` & `robin_api-1.1/robin_api/_types.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/robin_api/_utils/_utils.py` & `robin_api-1.1/robin_api/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/robin_api/resources/completions.py` & `robin_api-1.1/robin_api/resources/completions.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,23 +58,25 @@
                     "conversation": conversation,
                     "max_new_tokens": max_tokens,
                     "stream": stream,
                     "temperature": temperature,
                     "save_response": save_response
                 },
              ) as response:
-
-            for data in response.iter_bytes():
-                json_part = data.decode('utf-8').split("data: ", 1)[1]
-                if json_part.startswith("DONE"):
-                    break
-                objeto = json.loads(json_part)
-                ensure_list(objeto, 'choices')
-                completion_obj = construct_type_v2(type_=ChatCompletionChunk, value=objeto)
-                yield completion_obj
+            if response.status_code == 200:
+                for data in response.iter_bytes():
+                    json_part = data.decode('utf-8').split("data: ", 1)[1]
+                    if json_part.startswith("DONE"):
+                        break
+                    objeto = json.loads(json_part)
+                    ensure_list(objeto, 'choices')
+                    completion_obj = construct_type_v2(type_=ChatCompletionChunk, value=objeto)
+                    yield completion_obj
+            else:
+                raise ConnectionError(f"Error: {str(response.status_code)}")
                 
         
 
         """return self.client.http_client._post(
             "/completions",
             body=maybe_transform(
                 {
```

### Comparing `robin_api-1.0/robin_api/types/__init__.py` & `robin_api-1.1/robin_api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/robin_api/types/completion.py` & `robin_api-1.1/robin_api/types/completion.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.0/setup.py` & `robin_api-1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='robin_api',
-    version='1.0',
+    version='1.1',
     packages=['robin_api'],
     description="file",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'httpx',
         'pydantic',
```

