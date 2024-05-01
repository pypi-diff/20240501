# Comparing `tmp/surfkit-0.1.93.tar.gz` & `tmp/surfkit-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfkit-0.1.93.tar", max compression
+gzip compressed data, was "surfkit-0.1.95.tar", max compression
```

## Comparing `surfkit-0.1.93.tar` & `surfkit-0.1.95.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1069 2024-04-09 16:39:37.152115 surfkit-0.1.93/LICENSE
--rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.93/README.md
--rw-r--r--   0        0        0      734 2024-04-29 20:30:25.198562 surfkit-0.1.93/pyproject.toml
--rw-r--r--   0        0        0     1725 2024-04-25 22:12:14.558746 surfkit-0.1.93/surfkit/agent.py
--rw-r--r--   0        0        0     7728 2024-04-29 20:07:35.622937 surfkit-0.1.93/surfkit/cli/main.py
--rw-r--r--   0        0        0      926 2024-04-29 19:57:18.519637 surfkit-0.1.93/surfkit/cli/new.py
--rw-r--r--   0        0        0    13462 2024-04-29 19:56:21.528849 surfkit-0.1.93/surfkit/cli/templates/agent.py
--rw-r--r--   0        0        0        0 2024-04-09 16:39:37.166494 surfkit-0.1.93/surfkit/cli/templates/device.py
--rw-r--r--   0        0        0      866 2024-04-29 19:58:42.750756 surfkit-0.1.93/surfkit/cli/util.py
--rw-r--r--   0        0        0     2053 2024-04-17 19:36:14.985684 surfkit-0.1.93/surfkit/config.py
--rw-r--r--   0        0        0     2007 2024-04-17 19:23:41.286231 surfkit-0.1.93/surfkit/db/conn.py
--rw-r--r--   0        0        0      982 2024-04-17 16:29:32.098357 surfkit-0.1.93/surfkit/db/models.py
--rw-r--r--   0        0        0      238 2024-04-17 19:35:04.174976 surfkit-0.1.93/surfkit/env.py
--rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.93/surfkit/hub.py
--rw-r--r--   0        0        0     9144 2024-04-26 03:39:53.635637 surfkit-0.1.93/surfkit/llm.py
--rw-r--r--   0        0        0     2649 2024-04-26 03:40:29.954908 surfkit-0.1.93/surfkit/models.py
--rw-r--r--   0        0        0     3034 2024-04-25 17:18:59.281584 surfkit-0.1.93/surfkit/runtime/agent/base.py
--rw-r--r--   0        0        0     7381 2024-04-25 17:19:06.360421 surfkit-0.1.93/surfkit/runtime/agent/docker.py
--rw-r--r--   0        0        0    27130 2024-04-25 17:19:11.347240 surfkit-0.1.93/surfkit/runtime/agent/kube.py
--rw-r--r--   0        0        0      910 2024-04-19 03:20:06.559203 surfkit-0.1.93/surfkit/runtime/agent/load.py
--rw-r--r--   0        0        0     1425 2024-04-11 22:52:18.482166 surfkit-0.1.93/surfkit/runtime/container/base.py
--rw-r--r--   0        0        0     5983 2024-04-16 16:34:59.842004 surfkit-0.1.93/surfkit/runtime/container/docker.py
--rw-r--r--   0        0        0    16077 2024-04-11 22:50:31.352813 surfkit-0.1.93/surfkit/runtime/container/kube.py
--rw-r--r--   0        0        0     1028 2024-04-11 16:49:49.850218 surfkit-0.1.93/surfkit/runtime/container/load.py
--rw-r--r--   0        0        0      402 2024-04-11 18:32:09.170609 surfkit-0.1.93/surfkit/runtime/vm/base.py
--rw-r--r--   0        0        0     9920 2024-04-17 20:04:44.519945 surfkit-0.1.93/surfkit/types.py
--rw-r--r--   0        0        0      793 2024-04-25 20:53:50.784539 surfkit-0.1.93/surfkit/util.py
--rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 surfkit-0.1.93/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-09 16:39:37.152115 surfkit-0.1.95/LICENSE
+-rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.95/README.md
+-rw-r--r--   0        0        0      756 2024-04-30 19:55:48.733834 surfkit-0.1.95/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 21:28:15.523878 surfkit-0.1.95/surfkit/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-25 22:12:14.558746 surfkit-0.1.95/surfkit/agent.py
+-rw-r--r--   0        0        0    16244 2024-04-30 18:58:40.398487 surfkit-0.1.95/surfkit/cli/main.py
+-rw-r--r--   0        0        0      926 2024-04-29 19:57:18.519637 surfkit-0.1.95/surfkit/cli/new.py
+-rw-r--r--   0        0        0    17058 2024-04-30 03:19:26.328281 surfkit-0.1.95/surfkit/cli/templates/agent.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:39:37.166494 surfkit-0.1.95/surfkit/cli/templates/device.py
+-rw-r--r--   0        0        0      866 2024-04-29 19:58:42.750756 surfkit-0.1.95/surfkit/cli/util.py
+-rw-r--r--   0        0        0     2053 2024-04-17 19:36:14.985684 surfkit-0.1.95/surfkit/config.py
+-rw-r--r--   0        0        0     2263 2024-04-30 02:59:37.720164 surfkit-0.1.95/surfkit/db/conn.py
+-rw-r--r--   0        0        0     1033 2024-04-30 17:33:05.888950 surfkit-0.1.95/surfkit/db/models.py
+-rw-r--r--   0        0        0      238 2024-04-17 19:35:04.174976 surfkit-0.1.95/surfkit/env.py
+-rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.95/surfkit/hub.py
+-rw-r--r--   0        0        0     2634 2024-04-30 18:17:40.076017 surfkit-0.1.95/surfkit/models.py
+-rw-r--r--   0        0        0     3552 2024-04-30 18:18:31.505935 surfkit-0.1.95/surfkit/runtime/agent/base.py
+-rw-r--r--   0        0        0     9362 2024-04-30 17:53:07.043767 surfkit-0.1.95/surfkit/runtime/agent/docker.py
+-rw-r--r--   0        0        0    28584 2024-04-30 18:00:00.255715 surfkit-0.1.95/surfkit/runtime/agent/kube.py
+-rw-r--r--   0        0        0     1187 2024-04-30 16:00:13.133177 surfkit-0.1.95/surfkit/runtime/agent/load.py
+-rw-r--r--   0        0        0    11193 2024-04-30 18:15:04.806912 surfkit-0.1.95/surfkit/runtime/agent/process.py
+-rw-r--r--   0        0        0     1425 2024-04-11 22:52:18.482166 surfkit-0.1.95/surfkit/runtime/container/base.py
+-rw-r--r--   0        0        0     5983 2024-04-16 16:34:59.842004 surfkit-0.1.95/surfkit/runtime/container/docker.py
+-rw-r--r--   0        0        0    16077 2024-04-11 22:50:31.352813 surfkit-0.1.95/surfkit/runtime/container/kube.py
+-rw-r--r--   0        0        0     1028 2024-04-11 16:49:49.850218 surfkit-0.1.95/surfkit/runtime/container/load.py
+-rw-r--r--   0        0        0      402 2024-04-11 18:32:09.170609 surfkit-0.1.95/surfkit/runtime/vm/base.py
+-rw-r--r--   0        0        0    14338 2024-04-30 17:45:57.825243 surfkit-0.1.95/surfkit/types.py
+-rw-r--r--   0        0        0     1516 2024-04-30 17:09:57.207060 surfkit-0.1.95/surfkit/util.py
+-rw-r--r--   0        0        0     1344 1970-01-01 00:00:00.000000 surfkit-0.1.95/PKG-INFO
```

### Comparing `surfkit-0.1.93/LICENSE` & `surfkit-0.1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.93/pyproject.toml` & `surfkit-0.1.95/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surfkit"
-version = "0.1.93"
+version = "0.1.95"
 description = "A toolkit to build GUI surfing AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -18,14 +18,15 @@
 kubernetes = "^29.0.0"
 devicebay = "^0.1.11"
 litellm = "^1.35.8"
 agentdesk = "^0.2.65"
 tiktoken = "^0.6.0"
 taskara = "^0.1.42"
 rich = "^13.7.1"
+skillpacks = "^0.1.3"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.4"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `surfkit-0.1.93/surfkit/agent.py` & `surfkit-0.1.95/surfkit/agent.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.93/surfkit/cli/new.py` & `surfkit-0.1.95/surfkit/cli/new.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.93/surfkit/cli/templates/agent.py` & `surfkit-0.1.95/surfkit/cli/templates/agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import os
-
-from surfkit.types import AgentType
+from pathlib import Path
 
 
-def generate_dockerfile(package_name: str) -> None:
+def generate_dockerfile(agent_name: str) -> None:
     out = f"""
 FROM thehale/python-poetry:1.8.2-py3.10-slim
 
 COPY . /app
 WORKDIR /app
 
 RUN apt-get update && apt-get install -y openssh-client ntp
 RUN poetry install
 
 EXPOSE 9090
 
 # Run the application
-CMD ["uvicorn", "{package_name}.server:app", "--host=0.0.0.0", "--port=9090", "--log-level", "debug"]
+CMD ["uvicorn", "{agent_name.lower()}.server:app", "--host=0.0.0.0", "--port=9090", "--log-level", "debug"]
 """
     with open(f"Dockerfile", "w") as f:
         f.write(out)
 
 
 def generate_server(agent_name: str) -> None:
     out = f"""
@@ -29,17 +28,17 @@
 from taskara.server.models import SolveTaskModel, TaskModel, TasksModel
 from taskara.task import Task
 from surfkit.hub import Hub
 from surfkit.llm import LLMProvider
 from fastapi import FastAPI, BackgroundTasks
 from fastapi.middleware.cors import CORSMiddleware
 from contextlib import asynccontextmanager
+from tenacity import retry, stop_after_attempt, wait_fixed
 
 from .agent import Agent
-from .util import get_remote_task
 
 
 # Get the LLM provider from env
 llm_provider = LLMProvider.from_env()
 
 
 @asynccontextmanager
@@ -159,14 +158,39 @@
 @app.get("/v1/tasks/{{id}}", response_model=TaskModel)
 async def get_task(id: str):
     tasks = Task.find(id=id)
     if not tasks:
         raise Exception(f"Task {{id}} not found")
     return tasks[0].to_schema()
 
+    
+@retry(stop=stop_after_attempt(10), wait=wait_fixed(10))
+def get_remote_task(id: str, owner_id: str, server: str) -> Task:
+    HUB_API_KEY = os.environ.get("HUB_API_KEY")
+    if not HUB_API_KEY:
+        raise Exception("$HUB_API_KEY not set")
+
+    print("connecting to remote task: ", id, HUB_API_KEY)
+    try:
+        tasks = Task.find(
+            id=id,
+            remote=server,
+            owner_id=owner_id,
+        )
+        if not tasks:
+            raise Exception(f"Task {{id}} not found")
+        print("got remote task: ", tasks[0].__dict__)
+        return tasks[0]
+    except Exception as e:
+        print("error getting remote task: ", e)
+        raise e
+
+        
+if __name__ == "__main__":
+    uvicorn.run(app, host="0.0.0.0", port=9090, reload=True)
 """
     with open(f"{agent_name.lower()}/server.py", "w") as f:
         f.write(out)
 
 
 def generate_main(agent_name: str) -> None:
     out = f"""
@@ -288,15 +312,15 @@
 with open(args.agent_type) as f:
     agent_data = yaml.safe_load(f)
     agent_schema = AgentTypeModel(**agent_data)
 agent_type = AgentType.from_schema(agent_schema)
 
 # TODO: dynamically supply and provision devices
 console.print("Creating device...", style="green")
-print("\nprovider data: ", provider.to_data())
+print("provider data: ", provider.to_data())
 config = ProvisionConfig(provider=provider.to_data())
 device: Desktop = Desktop.ensure("gpt4v-demo", config=config)
 
 # View the desktop, we'll run in the background so it doesn't block
 device.view(background=True)
 
 if args.agent_runtime == "docker":
@@ -308,15 +332,15 @@
     kconf = KubeConnectConfig(namespace=args.namespace)
     conf = AgentRuntimeConfig(provider="kube", kube_config=kconf)
 else:
     raise ValueError("Unknown agent runtime")
 
 runtime = load_agent_runtime(conf)
 
-print("\ndevice schema: ", device.to_schema())
+print("device schema: ", device.to_schema())
 console.print("Running agent...", style="green")
 agent = runtime.run(agent_type, args.name, args.version, llm_providers_local=True)
 
 agent.proxy(DEFAULT_PROXY_PORT)
 console.print(f"Proxying agent to port {{DEFAULT_PROXY_PORT}}", style="green")
 
 task_model = SolveTaskModel(
@@ -327,50 +351,25 @@
 """
     with open(f"{agent_name.lower()}/__main__.py", "w") as f:
         f.write(out)
 
 
 def generate_agent(agent_name: str) -> None:
     out = f"""
-from typing import List, Tuple, Type
-import json
-import time
+from typing import List, Type
 import logging
 from typing import Final
-from copy import deepcopy
-import traceback
-import os
 
-from tenacity import (
-    retry,
-    stop_after_attempt,
-    before_sleep_log,
-)
 from devicebay import Device
 from agentdesk.device import Desktop
 from rich.console import Console
-from rich.json import JSON
 from surfkit.llm import LLMProvider
 from pydantic import BaseModel
-from modelscope.pipelines import pipeline
-from MobileAgent.icon_localization import load_model
-from modelscope.utils.constant import Tasks
 from surfkit.agent import TaskAgent
 from taskara import Task
-from threadmem import RoleThread
-
-from .instruct import (
-    system_prompt,
-    action_prompt,
-    ActionSelection,
-    reflection_prompt,
-    EndReflection,
-)
-from .util import remove_user_image_urls, clean_llm_json, ensure_download
-from .tool import SemanticDesktop
 
 logger: Final = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO)
 
 console = Console(force_terminal=True)
 
 llm_provider = LLMProvider.from_env()
@@ -472,48 +471,51 @@
 packages = [{{include = "{agent_name}"}}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sqlalchemy = "^2.0.27"
 pydantic = "^2.6.3"
 requests = "^2.31.0"
-surfkit - "^0.1.92"
+surfkit = "^0.1.92"
+tenacity = "^8.2.3"
 fastapi = {{version = "^0.109", extras = ["all"]}}
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 black = "^24.2.0"
 pytest = "^8.0.2"
 ipykernel = "^6.29.3"
 pytest-env = "^1.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 """
-    with open(f"{agent_name.lower()}/pyproject.toml", "w") as f:
+    with open(f"pyproject.toml", "w") as f:
         f.write(out)
 
 
 def generate_agentfile(
     name: str, description: str, image_repo: str, icon_url: str
 ) -> None:
 
     out = f"""
 api_version: v1alpha
 kind: TaskAgent
 name: "{name}"
 description: "{description}"
+cmd: "poetry run python -m {name.lower()}.server"
 image: "{image_repo}:latest"
 versions:
   latest: "{image_repo}:latest"
 runtimes:
   - type: "agent"
     preference:
+      - "venv"
       - "docker"
       - "kube"
 llm_providers:
   preference:
     - "gpt-4-turbo"
     - "anthropic/claude-3-opus-20240229"
 public: True
@@ -521,9 +523,185 @@
 resource_requests:
   cpu: "1"
   memory: "2Gi"
 resource_limits:
   cpu: "2"
   memory: "4Gi"
 """
-    with open(f"{name.lower()}/agent.yaml", "w") as f:
+    with open(f"agent.yaml", "w") as f:
         f.write(out)
+
+
+def generate_gitignore() -> None:
+
+    out = """
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
+
+.data/
+"""
+    file_path = Path(".gitignore")
+
+    if file_path.exists():
+        with file_path.open("a") as file:
+            file.write("\ndata/\n")
+    else:
+        with file_path.open("w") as file:
+            file.write(out)
```

### Comparing `surfkit-0.1.93/surfkit/cli/util.py` & `surfkit-0.1.95/surfkit/cli/util.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.93/surfkit/config.py` & `surfkit-0.1.95/surfkit/config.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.93/surfkit/db/conn.py` & `surfkit-0.1.95/surfkit/db/conn.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 import os
+import time
 
 from sqlalchemy import create_engine, Engine
 from sqlalchemy.orm import sessionmaker
 
 from .models import Base
 
 
 DB_TYPE = os.environ.get("DB_TYPE", "sqlite")
 
 
 def get_pg_conn() -> Engine:
-    # Env Vars
-    db_user = os.environ.get("DB_USER")
-    if not db_user:
-        raise ValueError("$DB_USER must be set to a valid postgres db user")
-
-    db_password = os.environ.get("DB_PASS")
-    if not db_password:
-        raise ValueError("$DB_PASS must be set to a valid postgres db user password")
-
-    db_host = os.environ.get("DB_HOST")
-    if not db_user:
-        raise ValueError("$DB_HOST must be set to a running postgres server")
-
-    db_name = os.environ.get("DB_NAME")
-    if not db_name:
-        raise ValueError("$DB_NAME must be set to a postgres db name")
+    # Helper function to get environment variable with fallback
+    def get_env_var(key: str) -> str:
+        task_key = f"SURFKIT_{key}"
+        value = os.environ.get(task_key)
+        if value is None:
+            value = os.environ.get(key)
+            if value is None:
+                raise ValueError(f"${key} must be set")
+        return value
+
+    # Retrieve environment variables with fallbacks
+    db_user = get_env_var("DB_USER")
+    db_password = get_env_var("DB_PASS")
+    db_host = get_env_var("DB_HOST")
+    db_name = get_env_var("DB_NAME")
 
     print(f"\nconnecting to db on postgres host '{db_host}' with db '{db_name}'")
     engine = create_engine(
         f"postgresql+psycopg2://{db_user}:{db_password}@{db_host}/{db_name}",
         client_encoding="utf8",
     )
 
     return engine
 
 
 def get_sqlite_conn() -> Engine:
-    print("\nconnecting to local sqlite db ./data/surfkit.db")
-    os.makedirs(os.path.dirname("./data/surfkit.db"), exist_ok=True)
-    engine = create_engine("sqlite:///./data/surfkit.db")
+    db_name = os.environ.get("SURFKIT_DB_NAME", "surfkit.db")
+    db_path = os.environ.get("SURFKIT_DB_PATH", "./.data")
+    db_test = os.environ.get("SURFKIT_DB_TEST", "false") == "true"
+    if db_test:
+        db_name = f"threads_test_{int(time.time())}.db"
+    print(f"connecting to local sqlite db ./.data/{db_name}")
+    os.makedirs(os.path.dirname(f"{db_path}/{db_name}"), exist_ok=True)
+    engine = create_engine(f"sqlite:///{db_path}/{db_name}")
     return engine
 
 
 if DB_TYPE == "postgres":
     engine = get_pg_conn()
 else:
     engine = get_sqlite_conn()
```

### Comparing `surfkit-0.1.93/surfkit/db/models.py` & `surfkit-0.1.95/surfkit/db/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 class AgentTypeRecord(Base):
     __tablename__ = "agent_types"
 
     id = Column(String, primary_key=True, default=lambda: str(uuid.uuid4()))
     name = Column(String, unique=True, index=True)
     description = Column(String)
+    kind = Column(String)
+    cmd = Column(String)
     image = Column(String)
     versions = Column(String, nullable=True)
     repo = Column(String, nullable=True)
     env_opts = Column(String)
     runtimes = Column(String)
     owner_id = Column(String)
     public = Column(Boolean)
```

### Comparing `surfkit-0.1.93/surfkit/hub.py` & `surfkit-0.1.95/surfkit/hub.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.93/surfkit/models.py` & `surfkit-0.1.95/surfkit/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,117 @@
 from typing import List, Optional, Dict, Any
 
 from pydantic import BaseModel
 
 
-class Action(BaseModel):
+class V1Action(BaseModel):
     """An action"""
 
     name: str
     parameters: Dict[str, Any]
 
 
-class ActionSelection(BaseModel):
+class V1ActionSelection(BaseModel):
     """An action selection from the model"""
 
     observation: str
     reason: str
-    action: Action
+    action: V1Action
 
 
-class EnvVarOptModel(BaseModel):
+class V1DeviceConfig(BaseModel):
     name: str
-    description: Optional[str] = None
-    required: bool = False
-    default: Optional[str] = None
-    secret: bool = False
-    options: List[str] = []
-
-
-class LLMProviders(BaseModel):
-    preference: List[str] = []
+    provision: bool = False
 
 
-class DeviceConfig(BaseModel):
-    name: str
-    provision: bool = False
+class V1DevicesConfig(BaseModel):
+    preference: List[V1DeviceConfig] = []
 
 
-class DevicesConfig(BaseModel):
-    preference: List[DeviceConfig] = []
+class V1Runtime(BaseModel):
+    type: str
+    preference: List[str] = []
 
 
-class LLMProviderOption(BaseModel):
-    model: str
-    env_var: EnvVarOptModel
+class V1ResourceLimits(BaseModel):
+    cpu: str = "2"
+    memory: str = "2Gi"
 
 
-class LLMProviderModel(BaseModel):
-    options: List[LLMProviderOption]
+class V1ResourceRequests(BaseModel):
+    cpu: str = "1"
+    memory: str = "500m"
+    gpu: Optional[str] = None
 
 
-class MeterModel(BaseModel):
+class V1EnvVarOpt(BaseModel):
     name: str
-    unit: str
-    cost: float
     description: Optional[str] = None
+    required: bool = False
+    default: Optional[str] = None
+    secret: bool = False
+    options: List[str] = []
 
 
-class RuntimeModel(BaseModel):
-    type: str
+class V1LLMProviders(BaseModel):
     preference: List[str] = []
 
 
-class ResourceLimitsModel(BaseModel):
-    cpu: str = "2"
-    memory: str = "2Gi"
-
-
-class ResourceRequestsModel(BaseModel):
-    cpu: str = "1"
-    memory: str = "500m"
-    gpu: Optional[str] = None
+class V1Meter(BaseModel):
+    name: str
+    unit: str
+    cost: float
+    description: Optional[str] = None
 
 
-class AgentTypeModel(BaseModel):
+class V1AgentType(BaseModel):
     version: Optional[str] = None
     kind: Optional[str] = None
     id: Optional[str] = None
     name: str
     description: str
+    cmd: str
     owner_id: Optional[str] = None
     repo: Optional[str] = None
     image: Optional[str] = None
     versions: Optional[Dict[str, str]] = None
-    env_opts: List[EnvVarOptModel] = []
-    runtimes: List[RuntimeModel] = []
+    env_opts: List[V1EnvVarOpt] = []
+    runtimes: List[V1Runtime] = []
     created: Optional[float] = None
     updated: Optional[float] = None
     public: bool = False
     icon: Optional[str] = None
-    resource_requests: ResourceRequestsModel = ResourceRequestsModel()
-    resource_limits: ResourceLimitsModel = ResourceLimitsModel()
-    llm_providers: Optional[LLMProviders] = None
-    devices: List[DeviceConfig] = []
-    meters: List[MeterModel] = []
+    resource_requests: V1ResourceRequests = V1ResourceRequests()
+    resource_limits: V1ResourceLimits = V1ResourceLimits()
+    llm_providers: Optional[V1LLMProviders] = None
+    devices: List[V1DeviceConfig] = []
+    meters: List[V1Meter] = []
+
+
+class V1AgentInstance(BaseModel):
+    name: str
+    type: V1AgentType
+    runtime: str
+    port: int = 9090
+
+
+class V1Find(BaseModel):
+    args: dict = {}
 
 
-class AgentTypesModel(BaseModel):
-    types: List[AgentTypeModel]
+class V1AgentTypes(BaseModel):
+    types: List[V1AgentType]
 
 
 class CreateAgentTypeModel(BaseModel):
     id: str
     name: str
     description: str
     image: str
-    env_opts: List[EnvVarOptModel] = []
+    env_opts: List[V1EnvVarOpt] = []
     supported_runtimes: List[str] = []
     versions: Dict[str, str] = {}
     public: bool = False
     icon: Optional[str] = None
 
 
 class V1UserProfile(BaseModel):
```

### Comparing `surfkit-0.1.93/surfkit/runtime/agent/base.py` & `surfkit-0.1.95/surfkit/runtime/agent/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 from typing import List, TypeVar, Type, Generic, Union, Iterator, Optional
 from abc import ABC, abstractmethod
 
 from pydantic import BaseModel
 from taskara.server.models import SolveTaskModel
 
 from surfkit.types import AgentType
+from surfkit.models import V1AgentInstance
 
 R = TypeVar("R", bound="AgentRuntime")
 C = TypeVar("C", bound="BaseModel")
 
 
 class AgentInstance:
     """A running agent instance"""
 
-    def __init__(self, name: str, type: AgentType, runtime: "AgentRuntime") -> None:
+    def __init__(
+        self, name: str, type: AgentType, runtime: "AgentRuntime", port: int = 9090
+    ) -> None:
         self._runtime = runtime
         self._type = type
         self._name = name
+        self._port = port
 
     @property
     def type(self) -> AgentType:
         return self._type
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def runtime(self) -> "AgentRuntime":
         return self._runtime
 
+    @property
+    def port(self) -> int:
+        return self._port
+
     def proxy(
         self,
         local_port: Optional[int] = None,
         pod_port: int = 9090,
         background: bool = True,
     ) -> None:
         return self._runtime.proxy(self._name, local_port, pod_port, background)
@@ -52,14 +60,23 @@
             follow (bool): If True, stream logs until the connection
 
         Returns:
             str: The logs from the pod.
         """
         return self._runtime.logs(self._name, follow)
 
+    def to_v1(self) -> V1AgentInstance:
+        """Convert to V1 API model"""
+        return V1AgentInstance(
+            name=self._name,
+            type=self._type.to_v1(),
+            runtime=self._runtime.name(),
+            port=self._port,
+        )
+
 
 class AgentRuntime(Generic[R, C], ABC):
 
     @classmethod
     def name(cls) -> str:
         return cls.__name__
 
@@ -88,15 +105,19 @@
     @abstractmethod
     def solve_task(
         self, agent_name: str, task: SolveTaskModel, follow_logs: bool = False
     ) -> None:
         pass
 
     @abstractmethod
-    def list(self) -> List[str]:
+    def list(self) -> List[AgentInstance]:
+        pass
+
+    @abstractmethod
+    def get(self, name: str) -> AgentInstance:
         pass
 
     @abstractmethod
     def proxy(
         self,
         name: str,
         local_port: Optional[int] = None,
```

### Comparing `surfkit-0.1.93/surfkit/runtime/agent/docker.py` & `surfkit-0.1.95/surfkit/runtime/agent/docker.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 
 import docker
 from docker.errors import NotFound
 from taskara.server.models import SolveTaskModel
 from agentdesk.util import find_open_port
 import requests
 from pydantic import BaseModel
+from mllm import Router
+
+from surfkit.models import V1AgentType
 
 from .base import AgentRuntime, AgentInstance
 from surfkit.types import AgentType
-from surfkit.llm import LLMProvider
 
 
 class ConnectConfig(BaseModel):
     timeout: Optional[int] = None
 
 
 class DockerAgentRuntime(AgentRuntime):
@@ -46,29 +48,30 @@
         llm_providers_local: bool = False,
         owner_id: Optional[str] = None,
     ) -> AgentInstance:
         labels = {
             "provisioner": "surfkit",
             "agent_type": agent_type.name,
             "agent_name": name,
+            "agent_type_model": agent_type.to_v1().model_dump_json(),
         }
 
         port = find_open_port(8001, 9000)
         print("running container")
 
         if llm_providers_local:
             if not agent_type.llm_providers:
                 raise ValueError(
                     "no llm providers in agent type, yet llm_providers_local is True"
                 )
             if not env_vars:
                 env_vars = {}
             found = {}
             for provider_name in agent_type.llm_providers.preference:
-                api_key_env = LLMProvider.provider_api_keys.get(provider_name)
+                api_key_env = Router.provider_api_keys.get(provider_name)
                 if not api_key_env:
                     raise ValueError(f"no api key env for provider {provider_name}")
                 key = os.getenv(api_key_env)
                 if not key:
                     print("no api key found locally for provider: ", provider_name)
                     continue
 
@@ -133,21 +136,61 @@
         local_port: Optional[int] = None,
         pod_port: int = 9090,
         background: bool = True,
     ) -> None:
         print("no proxy needed")
         return
 
-    def list(self) -> List[str]:
-        label_filter = {"label": ["provisioner=surfkit"]}
+    def list(self) -> List[AgentInstance]:
+        label_filter = {"label": "provisioner=surfkit"}
         containers = self.client.containers.list(filters=label_filter)
+        instances = []
+
+        for container in containers:
+            agent_type_model = container.labels.get("agent_type_model")  # type: ignore
+            if not agent_type_model:
+                continue  # Skip containers where the agent type model is not found
+
+            agentv1 = V1AgentType.model_validate_json(agent_type_model)
+            agent_type = AgentType.from_v1(agentv1)
+            agent_name = container.name  # type: ignore
+
+            # Extract port information
+            ports = container.attrs["NetworkSettings"]["Ports"]  # type: ignore
+            exposed_port = 9090  # Default application port inside container
+            host_port = ports.get(f"{exposed_port}/tcp")
+            if not host_port:
+                raise ValueError("No host port found for exposed container port")
+            port = int(host_port[0]["HostPort"])
+            instance = AgentInstance(agent_name, agent_type, self, port)
+            instances.append(instance)
+
+        return instances
 
-        container_names_or_ids = [container.name for container in containers]  # type: ignore
+    def get(self, name: str) -> AgentInstance:
+        try:
+            container = self.client.containers.get(name)
+            agent_type_model = container.labels.get("agent_type_model")  # type: ignore
+            if not agent_type_model:
+                raise ValueError("Expected agent type model in labels")
+
+            agentv1 = V1AgentType.model_validate_json(agent_type_model)
+            agent_type = AgentType.from_v1(agentv1)
+
+            # Extract port information
+            ports = container.attrs["NetworkSettings"]["Ports"]  # type: ignore
+            exposed_port = 9090  # Default application port inside container
+            host_port = ports.get(f"{exposed_port}/tcp")
+            if not host_port:
+                raise ValueError("Expected agent port in container network settings")
+            port = int(host_port[0]["HostPort"])
 
-        return container_names_or_ids
+            return AgentInstance(name, agent_type, self, port)
+        except NotFound:
+            raise ValueError(f"Container '{name}' not found")
 
     def delete(self, name: str) -> None:
         try:
             # Attempt to get the container by name
             container = self.client.containers.get(name)
 
             # If found, remove the container
```

### Comparing `surfkit-0.1.93/surfkit/runtime/agent/kube.py` & `surfkit-0.1.95/surfkit/runtime/agent/kube.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from curses.ascii import isdigit
 from typing import List, Optional, Tuple, Type, Union, Iterator
 import os
 import json
 import urllib.error
 import urllib.parse
 import urllib.request
 from tenacity import retry, stop_after_attempt, wait_fixed
@@ -22,19 +21,19 @@
 from kubernetes.client import Configuration
 from kubernetes.client.api import core_v1_api
 from namesgenerator import get_random_name
 from tenacity import retry
 from pydantic import BaseModel
 from taskara.server.models import SolveTaskModel
 from agentdesk.util import find_open_port
+from mllm import Router
 
 from .base import AgentRuntime, AgentInstance
 from surfkit.types import AgentType
-from surfkit.llm import LLMProvider
-from surfkit.models import ResourceLimitsModel, ResourceRequestsModel
+from surfkit.models import V1ResourceLimits, V1ResourceRequests, V1AgentType
 
 
 class GKEOpts(BaseModel):
     cluster_name: str
     region: str
     service_account_json: str
 
@@ -111,17 +110,18 @@
         except ApiException as e:
             print(f"Failed to create secret: {e}")
             raise
 
     def create(
         self,
         image: str,
+        type: AgentType,
         name: Optional[str] = None,
-        resource_requests: ResourceRequestsModel = ResourceRequestsModel(),
-        resource_limits: ResourceLimitsModel = ResourceLimitsModel(),
+        resource_requests: V1ResourceRequests = V1ResourceRequests(),
+        resource_limits: V1ResourceLimits = V1ResourceLimits(),
         env_vars: Optional[dict] = None,
         owner_id: Optional[str] = None,
     ) -> None:
         if not name:
             name = get_random_name("-")
             if not name:
                 raise ValueError("Could not generate a random name")
@@ -170,15 +170,20 @@
         # Pod creation
         pod = client.V1Pod(
             api_version="v1",
             kind="Pod",
             metadata=client.V1ObjectMeta(
                 name=name,
                 labels={"provisioner": "surfkit"},
-                annotations={"owner": owner_id},
+                annotations={
+                    "owner": owner_id,
+                    "agent_name": name,
+                    "agent_type": type.name,
+                    "agent_model": type.to_v1().model_dump_json(),
+                },
             ),
             spec=pod_spec,
         )
 
         try:
             created_pod: client.V1Pod = self.core_api.create_namespaced_pod(  # type: ignore
                 namespace=self.namespace, body=pod
@@ -573,19 +578,51 @@
                 pretty="true",
                 _preload_content=False,  # Important to return a generator when following
             )
         except ApiException as e:
             print(f"Failed to get logs for pod '{name}': {e}")
             raise
 
-    def list(self) -> List[str]:
-        pods = self.core_api.list_namespaced_pod(
-            namespace="default", label_selector="provisioner=surfkit"
-        )
-        return [pod.metadata.name for pod in pods.items]
+    def list(self) -> List[AgentInstance]:
+        instances = []
+        try:
+            pods = self.core_api.list_namespaced_pod(
+                namespace=self.namespace, label_selector="provisioner=surfkit"
+            )
+            for pod in pods.items:
+                agent_type_model = pod.metadata.annotations.get("agent_model")
+                if not agent_type_model:
+                    continue  # Skip if no agent model annotation
+
+                agent_type = AgentType.from_v1(
+                    V1AgentType.model_validate_json(agent_type_model)
+                )
+                name = pod.metadata.name
+
+                instances.append(AgentInstance(name, agent_type, self, 9090))
+        except ApiException as e:
+            print(f"Failed to list pods: {e}")
+            raise
+        return instances
+
+    def get(self, name: str) -> AgentInstance:
+        try:
+            pod = self.core_api.read_namespaced_pod(name=name, namespace=self.namespace)
+            agent_type_model = pod.metadata.annotations.get("agent_model")  # type: ignore
+            if not agent_type_model:
+                raise ValueError("Agent model annotation missing in pod metadata")
+
+            agent_type = AgentType.from_v1(
+                V1AgentType.model_validate_json(agent_type_model)
+            )
+
+            return AgentInstance(name, agent_type, self, 9090)
+        except ApiException as e:
+            print(f"Failed to get pod '{name}': {e}")
+            raise
 
     def delete(self, name: str) -> None:
         try:
             # Delete the pod
             self.core_api.delete_namespaced_pod(
                 name=name,
                 namespace="default",
@@ -636,15 +673,15 @@
                 raise ValueError(
                     "no llm providers in agent type, yet llm_providers_local is True"
                 )
             if not env_vars:
                 env_vars = {}
             found = {}
             for provider_name in agent_type.llm_providers.preference:
-                api_key_env = LLMProvider.provider_api_keys.get(provider_name)
+                api_key_env = Router.provider_api_keys.get(provider_name)
                 if not api_key_env:
                     raise ValueError(f"no api key env for provider {provider_name}")
                 key = os.getenv(api_key_env)
                 if not key:
                     print("no api key found locally for provider: ", provider_name)
                     continue
 
@@ -655,14 +692,15 @@
                 raise ValueError(
                     "no api keys found locally for any of the providers in the agent type"
                 )
             env_vars.update(found)
 
         self.create(
             image=img,
+            type=agent_type,
             name=name,
             resource_requests=agent_type.resource_requests,
             resource_limits=agent_type.resource_limits,
             env_vars=env_vars,
             owner_id=owner_id,
         )
```

### Comparing `surfkit-0.1.93/surfkit/runtime/agent/load.py` & `surfkit-0.1.95/surfkit/runtime/agent/load.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from typing import Optional, List
 
 from pydantic import BaseModel
 
 from .docker import DockerAgentRuntime, ConnectConfig as DockerConnectConfig
 from .kube import KubernetesAgentRuntime, ConnectConfig as KubeConnectConfig
+from .process import ProcessAgentRuntime, ConnectConfig as ProcessConnectConfig
 from .base import AgentRuntime
 
 
 class AgentRuntimeConfig(BaseModel):
     provider: Optional[str] = None
     docker_config: Optional[DockerConnectConfig] = None
     kube_config: Optional[KubeConnectConfig] = None
+    process_config: Optional[ProcessConnectConfig] = None
     preference: List[str] = ["kube", "docker"]
 
 
 def load_agent_runtime(cfg: AgentRuntimeConfig) -> AgentRuntime:
     for pref in cfg.preference:
         if pref == KubernetesAgentRuntime.name() and cfg.kube_config:
             return KubernetesAgentRuntime.connect(cfg.kube_config)
         elif pref == DockerAgentRuntime.name() and cfg.docker_config:
             return DockerAgentRuntime.connect(cfg.docker_config)
+        elif pref == ProcessAgentRuntime.name() and cfg.process_config:
+            return ProcessAgentRuntime.connect(cfg.process_config)
     raise ValueError(f"Unknown provider: {cfg.provider}")
```

### Comparing `surfkit-0.1.93/surfkit/runtime/container/base.py` & `surfkit-0.1.95/surfkit/runtime/container/base.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.93/surfkit/runtime/container/docker.py` & `surfkit-0.1.95/surfkit/runtime/container/docker.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.93/surfkit/runtime/container/kube.py` & `surfkit-0.1.95/surfkit/runtime/container/kube.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.93/surfkit/runtime/container/load.py` & `surfkit-0.1.95/surfkit/runtime/container/load.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.93/PKG-INFO` & `surfkit-0.1.95/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surfkit
-Version: 0.1.93
+Version: 0.1.95
 Summary: A toolkit to build GUI surfing AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0)
 Requires-Dist: litellm (>=1.35.8,<2.0.0)
 Requires-Dist: namesgenerator (>=0.3,<0.4)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: rootpath (>=0.1.1,<0.2.0)
+Requires-Dist: skillpacks (>=0.1.3,<0.2.0)
 Requires-Dist: taskara (>=0.1.42,<0.2.0)
 Requires-Dist: threadmem (>=0.2.11,<0.3.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: toolfuse (>=0.1.15,<0.2.0)
 Description-Content-Type: text/markdown
 
 # SurfKit
```

