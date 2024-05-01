# Comparing `tmp/surfkit-0.1.97.tar.gz` & `tmp/surfkit-0.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfkit-0.1.97.tar", max compression
+gzip compressed data, was "surfkit-0.1.98.tar", max compression
```

## Comparing `surfkit-0.1.97.tar` & `surfkit-0.1.98.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1069 2024-04-09 16:39:37.152115 surfkit-0.1.97/LICENSE
--rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.97/README.md
--rw-r--r--   0        0        0      756 2024-05-01 02:16:18.897241 surfkit-0.1.97/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 21:28:15.523878 surfkit-0.1.97/surfkit/__init__.py
--rw-r--r--   0        0        0     1849 2024-04-30 20:04:26.117959 surfkit-0.1.97/surfkit/agent.py
--rw-r--r--   0        0        0    16234 2024-05-01 02:02:40.677176 surfkit-0.1.97/surfkit/cli/main.py
--rw-r--r--   0        0        0      926 2024-04-29 19:57:18.519637 surfkit-0.1.97/surfkit/cli/new.py
--rw-r--r--   0        0        0    17058 2024-04-30 03:19:26.328281 surfkit-0.1.97/surfkit/cli/templates/agent.py
--rw-r--r--   0        0        0        0 2024-04-09 16:39:37.166494 surfkit-0.1.97/surfkit/cli/templates/device.py
--rw-r--r--   0        0        0      866 2024-04-29 19:58:42.750756 surfkit-0.1.97/surfkit/cli/util.py
--rw-r--r--   0        0        0     2053 2024-04-17 19:36:14.985684 surfkit-0.1.97/surfkit/config.py
--rw-r--r--   0        0        0     2263 2024-04-30 02:59:37.720164 surfkit-0.1.97/surfkit/db/conn.py
--rw-r--r--   0        0        0     1033 2024-04-30 17:33:05.888950 surfkit-0.1.97/surfkit/db/models.py
--rw-r--r--   0        0        0      238 2024-04-17 19:35:04.174976 surfkit-0.1.97/surfkit/env.py
--rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.97/surfkit/hub.py
--rw-r--r--   0        0        0     2634 2024-04-30 18:17:40.076017 surfkit-0.1.97/surfkit/models.py
--rw-r--r--   0        0        0     3543 2024-05-01 02:03:25.109376 surfkit-0.1.97/surfkit/runtime/agent/base.py
--rw-r--r--   0        0        0     9356 2024-05-01 02:03:41.708645 surfkit-0.1.97/surfkit/runtime/agent/docker.py
--rw-r--r--   0        0        0    28578 2024-05-01 02:04:01.750740 surfkit-0.1.97/surfkit/runtime/agent/kube.py
--rw-r--r--   0        0        0     1187 2024-04-30 16:00:13.133177 surfkit-0.1.97/surfkit/runtime/agent/load.py
--rw-r--r--   0        0        0    11187 2024-05-01 02:04:40.092850 surfkit-0.1.97/surfkit/runtime/agent/process.py
--rw-r--r--   0        0        0     1425 2024-04-11 22:52:18.482166 surfkit-0.1.97/surfkit/runtime/container/base.py
--rw-r--r--   0        0        0     5983 2024-04-16 16:34:59.842004 surfkit-0.1.97/surfkit/runtime/container/docker.py
--rw-r--r--   0        0        0    16077 2024-04-11 22:50:31.352813 surfkit-0.1.97/surfkit/runtime/container/kube.py
--rw-r--r--   0        0        0     1028 2024-04-11 16:49:49.850218 surfkit-0.1.97/surfkit/runtime/container/load.py
--rw-r--r--   0        0        0      402 2024-04-11 18:32:09.170609 surfkit-0.1.97/surfkit/runtime/vm/base.py
--rw-r--r--   0        0        0    14338 2024-04-30 17:45:57.825243 surfkit-0.1.97/surfkit/types.py
--rw-r--r--   0        0        0     1516 2024-04-30 17:09:57.207060 surfkit-0.1.97/surfkit/util.py
--rw-r--r--   0        0        0     1344 1970-01-01 00:00:00.000000 surfkit-0.1.97/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-09 16:39:37.152115 surfkit-0.1.98/LICENSE
+-rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.98/README.md
+-rw-r--r--   0        0        0      756 2024-05-01 17:41:28.640573 surfkit-0.1.98/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 21:28:15.523878 surfkit-0.1.98/surfkit/__init__.py
+-rw-r--r--   0        0        0     1921 2024-05-01 02:53:14.821990 surfkit-0.1.98/surfkit/agent.py
+-rw-r--r--   0        0        0    16409 2024-05-01 14:51:16.439451 surfkit-0.1.98/surfkit/cli/main.py
+-rw-r--r--   0        0        0      926 2024-04-29 19:57:18.519637 surfkit-0.1.98/surfkit/cli/new.py
+-rw-r--r--   0        0        0    17058 2024-04-30 03:19:26.328281 surfkit-0.1.98/surfkit/cli/templates/agent.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:39:37.166494 surfkit-0.1.98/surfkit/cli/templates/device.py
+-rw-r--r--   0        0        0      866 2024-04-29 19:58:42.750756 surfkit-0.1.98/surfkit/cli/util.py
+-rw-r--r--   0        0        0     2053 2024-04-17 19:36:14.985684 surfkit-0.1.98/surfkit/config.py
+-rw-r--r--   0        0        0     2263 2024-04-30 02:59:37.720164 surfkit-0.1.98/surfkit/db/conn.py
+-rw-r--r--   0        0        0     1216 2024-05-01 14:46:55.707656 surfkit-0.1.98/surfkit/db/models.py
+-rw-r--r--   0        0        0      238 2024-04-17 19:35:04.174976 surfkit-0.1.98/surfkit/env.py
+-rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.98/surfkit/hub.py
+-rw-r--r--   0        0        0     2687 2024-05-01 17:42:12.432805 surfkit-0.1.98/surfkit/models.py
+-rw-r--r--   0        0        0     3543 2024-05-01 02:03:25.109376 surfkit-0.1.98/surfkit/runtime/agent/base.py
+-rw-r--r--   0        0        0     9356 2024-05-01 02:03:41.708645 surfkit-0.1.98/surfkit/runtime/agent/docker.py
+-rw-r--r--   0        0        0    28578 2024-05-01 02:04:01.750740 surfkit-0.1.98/surfkit/runtime/agent/kube.py
+-rw-r--r--   0        0        0     1187 2024-04-30 16:00:13.133177 surfkit-0.1.98/surfkit/runtime/agent/load.py
+-rw-r--r--   0        0        0    11187 2024-05-01 02:04:40.092850 surfkit-0.1.98/surfkit/runtime/agent/process.py
+-rw-r--r--   0        0        0     1425 2024-04-11 22:52:18.482166 surfkit-0.1.98/surfkit/runtime/container/base.py
+-rw-r--r--   0        0        0     5983 2024-04-16 16:34:59.842004 surfkit-0.1.98/surfkit/runtime/container/docker.py
+-rw-r--r--   0        0        0    16077 2024-04-11 22:50:31.352813 surfkit-0.1.98/surfkit/runtime/container/kube.py
+-rw-r--r--   0        0        0     1028 2024-04-11 16:49:49.850218 surfkit-0.1.98/surfkit/runtime/container/load.py
+-rw-r--r--   0        0        0      402 2024-04-11 18:32:09.170609 surfkit-0.1.98/surfkit/runtime/vm/base.py
+-rw-r--r--   0        0        0     7230 2024-05-01 17:41:48.899239 surfkit-0.1.98/surfkit/server/routes.py
+-rw-r--r--   0        0        0    14338 2024-04-30 17:45:57.825243 surfkit-0.1.98/surfkit/types.py
+-rw-r--r--   0        0        0     1516 2024-04-30 17:09:57.207060 surfkit-0.1.98/surfkit/util.py
+-rw-r--r--   0        0        0     1344 1970-01-01 00:00:00.000000 surfkit-0.1.98/PKG-INFO
```

### Comparing `surfkit-0.1.97/LICENSE` & `surfkit-0.1.98/LICENSE`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/pyproject.toml` & `surfkit-0.1.98/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surfkit"
-version = "0.1.97"
+version = "0.1.98"
 description = "A toolkit to build GUI surfing AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -18,15 +18,15 @@
 kubernetes = "^29.0.0"
 devicebay = "^0.1.11"
 litellm = "^1.35.8"
 agentdesk = "^0.2.65"
 tiktoken = "^0.6.0"
 rich = "^13.7.1"
 skillpacks = "^0.1.3"
-taskara = "^0.1.44"
+taskara = "^0.1.45"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.4"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `surfkit-0.1.97/surfkit/agent.py` & `surfkit-0.1.98/surfkit/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 C = TypeVar("C", bound="BaseModel")
 T = TypeVar("T", bound="TaskAgent")
 
 
 class TaskAgent(Generic[C, T], ABC):
     """An agent that works on tasks"""
 
+    @classmethod
+    def name(cls) -> str:
+        return cls.__name__
+
     @abstractmethod
     def solve_task(
         self,
         task: Task,
         device: Device,
         max_steps: int = 30,
     ) -> Task:
```

### Comparing `surfkit-0.1.97/surfkit/cli/main.py` & `surfkit-0.1.98/surfkit/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -515,20 +515,22 @@
         icon_url=icon_url,
     )
 
 
 @app.command(help="Use an agent to solve a task")
 def solve(
     description: str = typer.Option(..., help="Description of the task."),
-    agent_name: str = typer.Option(..., help="Name of the agent to use."),
+    agent_name: Optional[str] = typer.Option(None, help="Name of the agent to use."),
+    agent_type: Optional[str] = typer.Option(None, help="Type of agent to use."),
     max_steps: int = typer.Option(20, help="Maximum steps for the task."),
     starting_url: Optional[str] = typer.Option(
         None, help="Starting URL if applicable."
     ),
     runtime: str = typer.Option("docker", help="Runtime environment for the agent."),
+    kill: bool = typer.Option(False, help="Whether to kill the agent when done"),
 ):
     typer.echo(f"Solving task {description}...")
     from taskara.server.models import V1SolveTask
     from taskara import Task
 
     if runtime == "docker":
         from surfkit.runtime.agent.docker import (
```

### Comparing `surfkit-0.1.97/surfkit/cli/new.py` & `surfkit-0.1.98/surfkit/cli/new.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/cli/templates/agent.py` & `surfkit-0.1.98/surfkit/cli/templates/agent.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/cli/util.py` & `surfkit-0.1.98/surfkit/cli/util.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/config.py` & `surfkit-0.1.98/surfkit/config.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/db/conn.py` & `surfkit-0.1.98/surfkit/db/conn.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/db/models.py` & `surfkit-0.1.98/surfkit/db/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,7 +27,15 @@
     created = Column(Float, default=time.time)
     updated = Column(Float, default=time.time)
     resource_requests = Column(String, nullable=True)
     resource_limits = Column(String, nullable=True)
     llm_providers = Column(String, nullable=True)
     devices = Column(String, nullable=True)
     meters = Column(String, nullable=True)
+
+
+class AgentStatus(Base):
+    __tablename__ = "agent_status"
+
+    agent_id = Column(String, primary_key=True)
+    status = Column(String)
+    task_id = Column(String, nullable=True)
```

### Comparing `surfkit-0.1.97/surfkit/hub.py` & `surfkit-0.1.98/surfkit/hub.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/models.py` & `surfkit-0.1.98/surfkit/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,26 +98,31 @@
     args: dict = {}
 
 
 class V1AgentTypes(BaseModel):
     types: List[V1AgentType]
 
 
-class CreateAgentTypeModel(BaseModel):
+class V1CreateAgentType(BaseModel):
     id: str
     name: str
     description: str
     image: str
     env_opts: List[V1EnvVarOpt] = []
     supported_runtimes: List[str] = []
     versions: Dict[str, str] = {}
     public: bool = False
     icon: Optional[str] = None
 
 
+class V1Work:
+    remote: str
+    check_interval: int
+
+
 class V1UserProfile(BaseModel):
     email: Optional[str] = None
     display_name: Optional[str] = None
     handle: Optional[str] = None
     picture: Optional[str] = None
     created: Optional[int] = None
     updated: Optional[int] = None
```

### Comparing `surfkit-0.1.97/surfkit/runtime/agent/base.py` & `surfkit-0.1.98/surfkit/runtime/agent/base.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/runtime/agent/docker.py` & `surfkit-0.1.98/surfkit/runtime/agent/docker.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/runtime/agent/kube.py` & `surfkit-0.1.98/surfkit/runtime/agent/kube.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/runtime/agent/load.py` & `surfkit-0.1.98/surfkit/runtime/agent/load.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/runtime/agent/process.py` & `surfkit-0.1.98/surfkit/runtime/agent/process.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/runtime/container/base.py` & `surfkit-0.1.98/surfkit/runtime/container/base.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/runtime/container/docker.py` & `surfkit-0.1.98/surfkit/runtime/container/docker.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/runtime/container/kube.py` & `surfkit-0.1.98/surfkit/runtime/container/kube.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/runtime/container/load.py` & `surfkit-0.1.98/surfkit/runtime/container/load.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/types.py` & `surfkit-0.1.98/surfkit/types.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/surfkit/util.py` & `surfkit-0.1.98/surfkit/util.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.97/PKG-INFO` & `surfkit-0.1.98/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surfkit
-Version: 0.1.97
+Version: 0.1.98
 Summary: A toolkit to build GUI surfing AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Requires-Dist: litellm (>=1.35.8,<2.0.0)
 Requires-Dist: namesgenerator (>=0.3,<0.4)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: rootpath (>=0.1.1,<0.2.0)
 Requires-Dist: skillpacks (>=0.1.3,<0.2.0)
-Requires-Dist: taskara (>=0.1.44,<0.2.0)
+Requires-Dist: taskara (>=0.1.45,<0.2.0)
 Requires-Dist: threadmem (>=0.2.11,<0.3.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: toolfuse (>=0.1.15,<0.2.0)
 Description-Content-Type: text/markdown
 
 # SurfKit
```

