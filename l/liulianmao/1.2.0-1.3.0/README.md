# Comparing `tmp/liulianmao-1.2.0.tar.gz` & `tmp/liulianmao-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liulianmao-1.2.0.tar", max compression
+gzip compressed data, was "liulianmao-1.3.0.tar", max compression
```

## Comparing `liulianmao-1.2.0.tar` & `liulianmao-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,25 @@
--rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-1.2.0/LICENSE
--rw-r--r--   0        0        0      781 2024-04-09 02:24:00.217950 liulianmao-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3830 2024-04-05 10:51:08.732993 liulianmao-1.2.0/README.md
--rw-r--r--   0        0        0       84 2024-04-03 13:08:57.859474 liulianmao-1.2.0/src/liulianmao/__init__.py
--rw-r--r--   0        0        0     4200 2024-04-09 02:48:15.775349 liulianmao-1.2.0/src/liulianmao/__main__.py
--rw-r--r--   0        0        0        0 2024-04-03 12:56:28.446436 liulianmao-1.2.0/src/liulianmao/client/__init__.py
--rw-r--r--   0        0        0     6925 2024-04-06 12:29:52.522613 liulianmao-1.2.0/src/liulianmao/client/core.py
--rw-r--r--   0        0        0      608 2024-04-05 06:17:08.745870 liulianmao-1.2.0/src/liulianmao/client/langchain.py
--rw-r--r--   0        0        0      117 2024-04-01 16:47:06.824622 liulianmao-1.2.0/src/liulianmao/module/__init__.py
--rw-r--r--   0        0        0     2803 2024-04-08 07:16:31.906417 liulianmao-1.2.0/src/liulianmao/module/authentication.py
--rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-1.2.0/src/liulianmao/module/const.py
--rw-r--r--   0        0        0      605 2024-04-01 17:40:59.131588 liulianmao-1.2.0/src/liulianmao/module/log.py
--rw-r--r--   0        0        0     2120 2024-04-07 04:12:04.940254 liulianmao-1.2.0/src/liulianmao/module/model.py
--rw-r--r--   0        0        0     1409 2024-04-05 08:42:44.890771 liulianmao-1.2.0/src/liulianmao/module/storage.py
--rw-r--r--   0        0        0        0 2024-04-03 12:56:52.620830 liulianmao-1.2.0/src/liulianmao/tool/__init__.py
--rw-r--r--   0        0        0     3728 2024-04-01 11:33:08.073130 liulianmao-1.2.0/src/liulianmao/tool/ls.py
--rw-r--r--   0        0        0     4765 1970-01-01 00:00:00.000000 liulianmao-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-1.3.0/LICENSE
+-rw-r--r--   0        0        0      781 2024-05-01 15:26:09.878471 liulianmao-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7095 2024-05-01 14:58:58.387675 liulianmao-1.3.0/README.md
+-rw-r--r--   0        0        0       84 2024-04-03 13:08:57.859474 liulianmao-1.3.0/src/liulianmao/__init__.py
+-rw-r--r--   0        0        0     5020 2024-05-01 15:13:48.542866 liulianmao-1.3.0/src/liulianmao/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:56:28.446436 liulianmao-1.3.0/src/liulianmao/client/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-05 06:18:07.214401 liulianmao-1.3.0/src/liulianmao/client/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    20033 2024-05-01 15:22:42.210544 liulianmao-1.3.0/src/liulianmao/client/__pycache__/core.cpython-311.pyc
+-rw-r--r--   0        0        0    13563 2024-05-01 15:22:08.167782 liulianmao-1.3.0/src/liulianmao/client/core.py
+-rw-r--r--   0        0        0      608 2024-04-05 06:17:08.745870 liulianmao-1.3.0/src/liulianmao/client/langchain.py
+-rw-r--r--   0        0        0      119 2024-04-14 08:22:48.496972 liulianmao-1.3.0/src/liulianmao/module/__init__.py
+-rw-r--r--   0        0        0      318 2024-04-14 08:28:05.811497 liulianmao-1.3.0/src/liulianmao/module/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4697 2024-04-14 08:28:05.814494 liulianmao-1.3.0/src/liulianmao/module/__pycache__/authentication.cpython-311.pyc
+-rw-r--r--   0        0        0      931 2024-04-05 06:18:07.722094 liulianmao-1.3.0/src/liulianmao/module/__pycache__/const.cpython-311.pyc
+-rw-r--r--   0        0        0     1056 2024-04-05 06:18:07.342514 liulianmao-1.3.0/src/liulianmao/module/__pycache__/log.cpython-311.pyc
+-rw-r--r--   0        0        0     2497 2024-04-14 10:19:38.564221 liulianmao-1.3.0/src/liulianmao/module/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0        0        0     2481 2024-05-01 14:56:53.609585 liulianmao-1.3.0/src/liulianmao/module/__pycache__/storage.cpython-311.pyc
+-rw-r--r--   0        0        0     2864 2024-04-14 08:22:48.515590 liulianmao-1.3.0/src/liulianmao/module/authentication.py
+-rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-1.3.0/src/liulianmao/module/const.py
+-rw-r--r--   0        0        0      605 2024-04-01 17:40:59.131588 liulianmao-1.3.0/src/liulianmao/module/log.py
+-rw-r--r--   0        0        0     2347 2024-04-14 09:58:34.104170 liulianmao-1.3.0/src/liulianmao/module/model.py
+-rw-r--r--   0        0        0     1647 2024-05-01 14:53:06.868641 liulianmao-1.3.0/src/liulianmao/module/storage.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:56:52.620830 liulianmao-1.3.0/src/liulianmao/tool/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-01 11:33:08.073130 liulianmao-1.3.0/src/liulianmao/tool/ls.py
+-rw-r--r--   0        0        0     7995 1970-01-01 00:00:00.000000 liulianmao-1.3.0/PKG-INFO
```

### Comparing `liulianmao-1.2.0/LICENSE` & `liulianmao-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liulianmao-1.2.0/pyproject.toml` & `liulianmao-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liulianmao"
-version = "1.2.0"
+version = "1.3.0"
 description = "A LLM client for use from the command line or IDE."
 authors = ["快乐的老鼠宝宝 <laoshubaby@protonmail.com>"]
 license = "MIT"
 repository = "https://github.com/LaoshuBaby/liulianmao"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `liulianmao-1.2.0/src/liulianmao/__main__.py` & `liulianmao-1.3.0/src/liulianmao/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import argparse
 import os
 import sys
 from typing import List
 
+from module.log import logger
 
+
+@logger.catch(level="CRITICAL")
 def init_env():
     """
     Initialize the execution environment by setting system paths.
 
     This function checks whether the script is running from a PyInstaller
     bundle or a standard Python environment. It adjusts the system path
     accordingly to ensure that all necessary resources and modules are
@@ -20,16 +23,14 @@
         # Running in a normal Python environment
         current_dir = os.path.dirname(os.path.abspath(__file__))
         bundled_dir = current_dir
 
     parent_dir = os.path.dirname(bundled_dir)
 
     try:
-        from module.log import logger
-
         logger.debug(f'[ENV] "__file__" = {__file__}')
         logger.debug(f'[ENV] "bundled_dir" = {bundled_dir}')
         logger.debug(f'[ENV] "parent_dir" = {parent_dir}')
         logger.debug(f'[ENV] "os.getcwd()" = {os.getcwd()}')
         logger.debug(
             f'[ENV] "os.listdir(bundled_dir)" = {os.listdir(bundled_dir)}'
         )
@@ -46,14 +47,15 @@
             os.listdir(bundled_dir),
         )
 
     if parent_dir not in sys.path:
         sys.path.append(parent_dir)
 
 
+@logger.catch(level="CRITICAL")
 def main(recipe: List[str], actions: List[str]):
     """Execute the operations specified in the recipe list.
 
     根据提供的recipe列表和actions列表执行一系列操作。
 
     Args:
         recipe: A list of strings representing the operations to be processed.默认为["init", "chat"]。
@@ -88,44 +90,69 @@
     if FEATURE["langchain"]:
         # spec = importlib.util.find_spec('.langchain', package='client')
         # langchain = importlib.util.module_from_spec(spec)
         # spec.loader.exec_module(langchain)
         from client.langchain import main as langchain
 
     operations = {
+        "default": core.chat,
+        "models": core.models,
         "chat": core.chat,
         "talk": core.talk,
-        "models": core.models,
+        "draw": core.draw,
     }
 
+    logger.debug(f"[Recipe]: {recipe}")
     for operation_name in recipe:
         operation = operations.get(operation_name)
         if operation:
             operation()
         else:
             print(f"Operation {operation_name} is not defined.")
 
 
 if __name__ == "__main__":
     init_env()
-    default_recipe = ["chat"]
+    default_recipe = ["default"]
     parser = argparse.ArgumentParser(description="Process some operations.")
     parser.add_argument(
         "-q",
         "-question",
         "--question",
         action="store_true",
-        help="Read the question.txt file",
+        help="Open the question.txt file with default program",
     )
     parser.add_argument(
         "-c",
         "-config",
         "--config",
         action="store_true",
-        help="Read the config.txt file",
+        help="Open the config.txt file with default program",
+    )
+    parser.add_argument(
+        "-l",
+        "-log",
+        "--log",
+        action="store_true",
+        help="Open Log folder",
+    )
+    parser.add_argument(
+        "-k",
+        "-key",
+        "--key",
+        action="store_true",
+        help="Open OPENAI_API_KEY and OPENAI_BASE_URL files with default program",
+    )
+    parser.add_argument(
+        "-i",
+        help="Specify input file, read this file as question, not default question.txt",
+    )
+    parser.add_argument(
+        "-o",
+        help="Specify output file, write answer to this file, not default answer.txt",
     )
     parser.add_argument(
         "-r",
         "-recipe",
         "--recipe",
         nargs="*",
         default=default_recipe,
```

### Comparing `liulianmao-1.2.0/src/liulianmao/client/langchain.py` & `liulianmao-1.3.0/src/liulianmao/client/langchain.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.2.0/src/liulianmao/module/authentication.py` & `liulianmao-1.3.0/src/liulianmao/module/authentication.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,58 +14,62 @@
     def get_valid_value(value: str) -> Optional[str]:
         """判断字符串是否有效，如果有效则返回该字符串，否则返回None。"""
         value = value.strip()
         if value and not value.startswith("#"):
             return value
         return None
 
+    def read_and_log_file(file_path: str) -> Optional[str]:
+        """读取文件，并记录每一行，返回第一个有效值。"""
+        if isfile(file_path):
+            try:
+                with open(file_path) as f:
+                    values = f.read().split("\n")
+                    logger.trace("[Authentication]\n" + str(values))
+                    for value in values:
+                        valid_value = get_valid_value(value)
+                        if valid_value:
+                            return valid_value
+            except Exception as e:
+                logger.error(
+                    f"Error reading from file: {file_path}, Error: {e}"
+                )
+        return None
+
     def get_from_env(var_name: str) -> Optional[str]:
         """尝试从环境变量获取值。"""
         return os.environ.get(var_name)
 
     def get_from_user_folder(var_name: str) -> Optional[str]:
         """尝试从用户目录的文件夹读取。"""
-        var_file_path = join(get_user_folder(), PROJECT_FOLDER, var_name)
-        if isfile(var_file_path):
-            try:
-                with open(var_file_path) as f:
-                    values = f.read().split("\n")
-                    for value in values:
-                        if get_valid_value(value):
-                            return value
-            except Exception as e:
-                logger.error(f"Error reading {var_name} from user folder file: {e}")
-        return None
+        """复用read_and_log_file函数。"""
+        value = read_and_log_file(
+            join(get_user_folder(), PROJECT_FOLDER, var_name)
+        )
+        return value
 
     def get_from_current_dir(var_name: str) -> Optional[str]:
         """尝试从当前文件所在目录读取。"""
-        var_file_path = join(dirname(abspath(__file__)), var_name)
-        if isfile(var_file_path):
-            try:
-                with open(var_file_path) as f:
-                    values = f.read().split("\n")
-                    for value in values:
-                        if get_valid_value(value):
-                            return value
-            except Exception as e:
-                logger.error(f"Error reading {var_name} from current directory file: {e}")
-        return None
-
+        """复用read_and_log_file函数。"""
+        value = read_and_log_file(join(dirname(abspath(__file__)), var_name))
+        return value
 
     # 定义尝试顺序
     attempts = [get_from_user_folder, get_from_current_dir, get_from_env]
 
     for attempt in attempts:
         result = attempt(var_name)
         if result is not None:
             logger.trace("[Authentication]\n" + f"{var_name} = {result}")
             return result
 
     # 如果所有尝试都失败了，记录错误并返回默认值
-    logger.error(f"{var_name} not found in environment variables, user folder, or current directory file, using default.")
+    logger.error(
+        f"{var_name} not found in environment variables, user folder, or current directory file, using default."
+    )
     return default
 
 
 # 获取API URL和API KEY
 API_URL = get_env("OPENAI_BASE_URL", "https://api.openai.com")
 API_KEY = get_env(
     "OPENAI_API_KEY",
```

### Comparing `liulianmao-1.2.0/src/liulianmao/module/log.py` & `liulianmao-1.3.0/src/liulianmao/module/log.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.2.0/src/liulianmao/module/model.py` & `liulianmao-1.3.0/src/liulianmao/module/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,73 @@
 from .log import logger
 
 # 合并后的模型和变体信息
 MODEL_INFO = {
     "gpt-3.5-turbo": {
         "ratio": 0.75,
         "variants": [
-            "gpt3", "gpt-3", "gpt-3.5-turbo-0301", "gpt-3.5-turbo-0613",
-            "gpt-3.5-turbo-1106", "gpt-3.5-turbo-0125",  "gpt-3.5-turbo-instruct"
-        ]
+            "gpt3",
+            "gpt-3",
+            "gpt-3.5-turbo-0301",
+            "gpt-3.5-turbo-0613",
+            "gpt-3.5-turbo-1106",
+            "gpt-3.5-turbo-0125",
+            "gpt-3.5-turbo-instruct",
+        ],
     },
     "gpt-3.5-turbo-16k": {
         "ratio": 1.5,
-        "variants": [
-            "gpt-3.5-turbo-16k",
-            "gpt-3.5-turbo-16k-0613"
-        ]
+        "variants": ["gpt-3.5-turbo-16k", "gpt-3.5-turbo-16k-0613"],
     },
     "gpt-4-turbo-preview": {
         "ratio": 5.00,
         "variants": [
-            "gpt-4-1106-preview", "gpt-4-0125-preview", "gpt-4-turbo-preview", "gpt-4-turbo"
-        ]
+            "gpt-4-1106-preview",
+            "gpt-4-0125-preview",
+            "gpt-4-turbo-preview",
+            "gpt-4-turbo",
+        ],
     },
     "gpt-4": {
         "ratio": 15.00,
-        "variants": [
-            "gpt4", "GPT-4", "gpt-4-0314", "gpt-4-0613"
-        ]
+        "variants": ["gpt4", "GPT-4", "gpt-4-0314", "gpt-4-0613"],
     },
     "gpt-4-32k": {
         "ratio": 30.00,
-        "variants": [
-            "gpt-4-32k", "gpt-4-32k-0314", "gpt-4-32k-0613"
-        ]
+        "variants": ["gpt-4-32k", "gpt-4-32k-0314", "gpt-4-32k-0613"],
     },
     "gpt-4-vision-preview": {
         "ratio": None,  # Assuming we don't have a ratio for this model yet
-        "variants": [
-            "gpt-4-vision-preview"
-        ]
-    }
+        "variants": ["gpt-4-vision-preview"],
+    },
 }
 
-def select_model(input_model_name, available_models, direct_debug:bool=False):
-    if direct_debug == True:
-        return input_model_name
+
+def select_model(
+    input_model_name, available_models, direct_debug: bool = False
+):
+    def log_and_return(model_name, ratio="NaN"):
+        """
+        辅助函数，用于记录日志并返回模型名称。
+        如果在直接调试模式下，比率记录为NaN；否则，记录实际的比率。
+        """
+        logger.info(f"[Model] {model_name} ({ratio} x)")
+        return model_name
+
+    if direct_debug:
+        # 直接调试模式下，不查找MODEL_INFO，直接记录日志并返回模型名称
+        return log_and_return(input_model_name)
+
     input_model_name = input_model_name.lower()
     for model_name, model_info in MODEL_INFO.items():
         variants = model_info["variants"]
         if input_model_name in variants:
             available_variants = [v for v in variants if v in available_models]
             if available_variants:
                 # 选择最新的变体
                 selected_variant = max(available_variants)
-                ratio = model_info["ratio"]
-                if ratio is not None:
-                    logger.info(f"[Model] {selected_variant} ({ratio}x)")
-                    return selected_variant
-                else:
-                    logger.error(f"[Model] No ratio defined for {selected_variant}.")
-                    return None
+                return log_and_return(
+                    selected_variant, model_info.get("ratio")
+                )
+
     logger.error("[Model] Model not found.")
     return None
```

### Comparing `liulianmao-1.2.0/src/liulianmao/module/storage.py` & `liulianmao-1.3.0/src/liulianmao/module/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,41 @@
 
 def init():
     # 假设file_list中的JSON字符串需要格式化
     file_list = [
         (["terminal", "question.txt"], "Hello World!"),
         (["terminal", "answer.txt"], "Hello! How can I assist you today?"),
         # 使用json.dumps()格式化JSON字符串，并指定缩进为4个空格
-        (["assets", "config.json"], json.dumps({
-            "model_type": "gpt-4-turbo-preview",
-            "system_message": {"content": "You are a helpful assistant."},
-            "settings": {"temperature": 0.5}
-        }, indent=4))
+        (
+            ["assets", "config.json"],
+            json.dumps(
+                {
+                    "model_type": "gpt-4-turbo-preview",
+                    "system_message": {
+                        "content": "You are a helpful assistant."
+                    },
+                    "settings": {"temperature": 0.5},
+                },
+                indent=4,
+            ),
+        ),
     ]
-    folder_list = ["logs", "audios", "terminal", "assets"]
+    folder_list = ["logs", "audios", "images", "terminal", "assets"]
 
     for folder in folder_list:
         folder_path = os.path.join(get_user_folder(), PROJECT_FOLDER, folder)
         if not os.path.exists(folder_path):
             os.makedirs(folder_path)
 
     for file_path_parts, default_content in file_list:
-        file_path = os.path.join(get_user_folder(), PROJECT_FOLDER, *file_path_parts)
+        file_path = os.path.join(
+            get_user_folder(), PROJECT_FOLDER, *file_path_parts
+        )
         try:
             with open(file_path, "r", encoding="utf-8") as file:
                 file.read()
         except FileNotFoundError:
-            logger.error(f"{'/'.join(file_path_parts)} not found. Creating a new file.")
+            logger.error(
+                f"{'/'.join(file_path_parts)} not found. Creating a new file."
+            )
             with open(file_path, "w", encoding="utf-8") as file:
-                file.write(default_content)
+                file.write(default_content)
```

### Comparing `liulianmao-1.2.0/src/liulianmao/tool/ls.py` & `liulianmao-1.3.0/src/liulianmao/tool/ls.py`

 * *Files identical despite different names*

