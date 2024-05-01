# Comparing `tmp/edgegap_service-1.1.0.tar.gz` & `tmp/edgegap_service-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-1.1.0.tar", max compression
+gzip compressed data, was "edgegap_service-1.2.0.tar", max compression
```

## Comparing `edgegap_service-1.1.0.tar` & `edgegap_service-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1993 2024-04-30 16:04:37.495396 edgegap_service-1.1.0/LICENSE
--rw-r--r--   0        0        0     2188 2024-04-30 16:04:37.495396 edgegap_service-1.1.0/README.md
--rw-r--r--   0        0        0       17 2024-04-30 16:04:37.495396 edgegap_service-1.1.0/edgegap_service/BUILD
--rw-r--r--   0        0        0      164 2024-04-30 16:04:37.495396 edgegap_service-1.1.0/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2653 2024-04-30 16:04:37.495396 edgegap_service-1.1.0/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      733 2024-04-30 16:04:37.495396 edgegap_service-1.1.0/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      714 2024-04-30 16:04:37.495396 edgegap_service-1.1.0/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2208 2024-04-30 16:04:37.495396 edgegap_service-1.1.0/edgegap_service/_logging.py
--rw-r--r--   0        0        0     2902 2024-04-30 16:04:37.495396 edgegap_service-1.1.0/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7671 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/_templating.py
--rw-r--r--   0        0        0       17 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/health/BUILD
--rw-r--r--   0        0        0      101 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1478 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/health/_model.py
--rw-r--r--   0        0        0       17 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/health/checks/BUILD
--rw-r--r--   0        0        0      234 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0     1880 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0     4286 2024-04-30 16:04:37.499396 edgegap_service-1.1.0/edgegap_service/static/images/favicon.ico
--rw-r--r--   0        0        0      772 2024-04-30 16:04:46.743474 edgegap_service-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2188 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/BUILD
+-rw-r--r--   0        0        0      165 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2657 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      735 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      717 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2213 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_logging.py
+-rw-r--r--   0        0        0     2890 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7661 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/_templating.py
+-rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/BUILD
+-rw-r--r--   0        0        0      102 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/BUILD
+-rw-r--r--   0        0        0      235 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0     1880 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-05-01 17:52:18.963014 edgegap_service-1.2.0/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      972 2024-05-01 17:52:38.063483 edgegap_service-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.2.0/PKG-INFO
```

### Comparing `edgegap_service-1.1.0/LICENSE` & `edgegap_service-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.1.0/README.md` & `edgegap_service-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.1.0/edgegap_service/_configuration.py` & `edgegap_service-1.2.0/edgegap_service/_configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from typing import Callable, Optional
 
+from edgegap_scheduling import Scheduler
 from edgegap_settings import ProjectBaseSettings, SettingsFactory
 from fastapi import APIRouter
 from pydantic import BaseModel, ConfigDict, Field
 
-from edgegap_scheduling import Scheduler
 from ._environment import EnvironmentConfiguration
 from ._logging import LoggingConfiguration
 from .health.checks import CheckInterface
 
 
 class ServiceConfiguration(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
-    name: str = Field(..., description="The name of the Service")
-    version: str = Field(..., description="The version of the Service")
-    description: str = Field(..., description="The description of the Service")
-    routers: list[APIRouter] = Field([], description="The FastAPI routers")
-    root_dir: str = Field(..., description="The Root Directory of the Service")
-    static_dir: str = Field(default="static", description="The Static Directory of the Service")
-    html_index_path: str | None = Field(default=None, description="The full path to the html index file")
-    checks: list[type(CheckInterface)] = Field([], description="The list of Checks to run on the Service")
-    depend: Optional[Callable] = Field(default=None, description="The Base Depend Attribute for DB Session")
-    port: int = Field(default=8000, description="The Port of the Service")
-    host: str = Field(default="0.0.0.0", description="The Host of the Service")
-    workers: int = Field(default=1, description="Numbers of Workers, (if you use the scheduler, keep to 1)")
-    timeout: int = Field(default=300, description="Default Timeout for Connection")
-    worker_class: str = Field(default="uvicorn.workers.UvicornWorker", description="The worker class for ASGI")
-    scheduler: Scheduler | None = Field(default=None, description="A Scheduler to start at boot")
-    startup_functions: list[Callable] = Field(default=[], description="All function will be called on startup")
+    name: str = Field(..., description='The name of the Service')
+    version: str = Field(..., description='The version of the Service')
+    description: str = Field(..., description='The description of the Service')
+    routers: list[APIRouter] = Field([], description='The FastAPI routers')
+    root_dir: str = Field(..., description='The Root Directory of the Service')
+    static_dir: str = Field(default='static', description='The Static Directory of the Service')
+    html_index_path: str | None = Field(default=None, description='The full path to the html index file')
+    checks: list[type(CheckInterface)] = Field([], description='The list of Checks to run on the Service')
+    depend: Optional[Callable] = Field(default=None, description='The Base Depend Attribute for DB Session')
+    port: int = Field(default=8000, description='The Port of the Service')
+    host: str = Field(default='0.0.0.0', description='The Host of the Service')
+    workers: int = Field(default=1, description='Numbers of Workers, (if you use the scheduler, keep to 1)')
+    timeout: int = Field(default=300, description='Default Timeout for Connection')
+    worker_class: str = Field(default='uvicorn.workers.UvicornWorker', description='The worker class for ASGI')
+    scheduler: Scheduler | None = Field(default=None, description='A Scheduler to start at boot')
+    startup_functions: list[Callable] = Field(default=[], description='All function will be called on startup')
     env_config: EnvironmentConfiguration = Field(
         default=SettingsFactory.from_settings(EnvironmentConfiguration),
-        description="The Configuration coming from the Environment Variables"
+        description='The Configuration coming from the Environment Variables',
     )
     log_config: LoggingConfiguration = Field(
         default=LoggingConfiguration(),
-        description="The Configuration for the Logging, will be passed as DictConfig to Python logging system"
+        description='The Configuration for the Logging, will be passed as DictConfig to Python logging system',
     )
     settings: ProjectBaseSettings | None = Field(
         default=None,
-        description="Project Specific Settings to hold in the Service"
+        description='Project Specific Settings to hold in the Service',
     )
     tags_definition: list[dict] = Field(
         default=[],
-        description="See https://fastapi.tiangolo.com/tutorial/metadata/#use-your-tags for details"
+        description='See https://fastapi.tiangolo.com/tutorial/metadata/#use-your-tags for details',
     )
```

### Comparing `edgegap_service-1.1.0/edgegap_service/_documentation.py` & `edgegap_service-1.2.0/edgegap_service/_documentation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from fastapi import FastAPI, templating, Request, responses
+from fastapi import FastAPI, Request, responses, templating
 
 
 class DocumentationRoute:
     @staticmethod
     def init_documentation(app: FastAPI, file_name: str, templates: templating.Jinja2Templates):
-        @app.get("/", response_class=responses.HTMLResponse, include_in_schema=False)
+        @app.get('/', response_class=responses.HTMLResponse, include_in_schema=False)
         async def root(request: Request):
             urls = {
-                "Docs": f"{request.base_url}docs",
-                "Redoc": f"{request.base_url}redoc",
+                'Docs': f'{request.base_url}docs',
+                'Redoc': f'{request.base_url}redoc',
             }
 
             return templates.TemplateResponse(
                 name=file_name,
                 context={
-                    "request": request,
-                    "urls": urls,
-                    "title": getattr(app, 'title')
-                }
+                    'request': request,
+                    'urls': urls,
+                    'title': getattr(app, 'title'),
+                },
             )
```

### Comparing `edgegap_service-1.1.0/edgegap_service/_environment.py` & `edgegap_service-1.2.0/edgegap_service/_environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from edgegap_settings import EnvironmentField
 from pydantic_settings import BaseSettings
 
 
 class EnvironmentConfiguration(BaseSettings):
     log_level: str = EnvironmentField(
-        key="LOG_LEVEL",
-        description="The logging Level",
-        default="DEBUG"
+        key='LOG_LEVEL',
+        description='The logging Level',
+        default='DEBUG',
     )
 
     log_format: str = EnvironmentField(
-        key="LOG_FORMAT",
-        description="The Logging Format",
-        default="%(asctime)s | %(levelname)s | %(name)s | %(message)s"
+        key='LOG_FORMAT',
+        description='The Logging Format',
+        default='%(asctime)s | %(levelname)s | %(name)s | %(message)s',
     )
 
     log_access_format: str = EnvironmentField(
-        key="LOG_ACCESS_FORMAT",
-        description="The Logging Format for API Access",
-        default="%(asctime)s | %(levelname)s | %(name)s | %(client_addr)s - [%(request_line)s] %(status_code)s"
+        key='LOG_ACCESS_FORMAT',
+        description='The Logging Format for API Access',
+        default='%(asctime)s | %(levelname)s | %(name)s | %(client_addr)s - [%(request_line)s] %(status_code)s',
     )
```

### Comparing `edgegap_service-1.1.0/edgegap_service/_scheduling.py` & `edgegap_service-1.2.0/edgegap_service/_scheduling.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,69 @@
-from fastapi import (
-    FastAPI,
-    HTTPException
-)
+from edgegap_scheduling import SchedulingSingleton, Task, errors
+from fastapi import FastAPI, HTTPException
 from fastapi.routing import APIRouter
 from pydantic import BaseModel, Field
 
-from edgegap_scheduling import SchedulingSingleton, Task, errors
-
 
 class TaskParameters(BaseModel):
-    parameters: dict | None = Field(default=None, description="The parameters to update in the tasks")
+    parameters: dict | None = Field(default=None, description='The parameters to update in the tasks')
 
 
 class UpdateTask(TaskParameters):
-    every: str | None = Field(default=None, description="The interval to run the Task")
-    delay: str | None = Field(default=None, description="Delay before starting the Task")
+    every: str | None = Field(default=None, description='The interval to run the Task')
+    delay: str | None = Field(default=None, description='Delay before starting the Task')
 
 
 class SchedulingAPI:
-    tags = ["Scheduling"]
+    tags = ['Scheduling']
 
     def __init__(self):
         self.__instance = SchedulingSingleton.scheduler()
 
     def init_scheduling_api(self, app: FastAPI):
-        router = APIRouter(prefix="/scheduling/tasks", tags=self.tags)
+        router = APIRouter(prefix='/scheduling/tasks', tags=self.tags)
 
-        @router.get("/", description="Get all Tasks")
+        @router.get('/', description='Get all Tasks')
         async def get_tasks() -> list[Task]:
             return await self.__instance.list()
 
-        @router.get("/{identifier}", description="Get One Task")
+        @router.get('/{identifier}', description='Get One Task')
         async def get_task(identifier: str) -> Task:
             try:
                 return await self.__instance.get(identifier)
             except ValueError as e:
                 raise HTTPException(status_code=404, detail=str(e))
 
-        @router.post("/{identifier}", description="Start a stopped Task")
+        @router.post('/{identifier}', description='Start a stopped Task')
         async def start_task(identifier: str) -> Task:
             try:
                 return await self.__instance.start(identifier)
             except ValueError as e:
                 raise HTTPException(status_code=404, detail=str(e))
 
-        @router.patch("/{identifier}", description="Update the Interval of a Task")
+        @router.patch('/{identifier}', description='Update the Interval of a Task')
         async def update_task(identifier: str, task: UpdateTask) -> Task:
             try:
                 return await self.__instance.update(
                     identifier=identifier,
                     every=task.every,
                     delay=task.delay,
-                    parameters=task.parameters
+                    parameters=task.parameters,
                 )
             except ValueError as e:
                 raise HTTPException(status_code=404, detail=str(e))
 
-        @router.delete("/{identifier}", description="Stop a running Task")
+        @router.delete('/{identifier}', description='Stop a running Task')
         async def stop_task(identifier: str) -> Task:
             try:
                 return await self.__instance.stop(identifier)
             except ValueError as e:
                 raise HTTPException(status_code=404, detail=str(e))
 
-        @router.post("/run/{identifier}")
+        @router.post('/run/{identifier}')
         async def run_rask(identifier: str, task_parameters: TaskParameters | None) -> Task:
             try:
                 return await self.__instance.run(identifier, task_parameters.parameters)
             except ValueError as e:
                 raise HTTPException(status_code=404, detail=str(e))
             except errors.ManualRunNotAllowedError as e:
                 raise HTTPException(status_code=403, detail=str(e))
```

### Comparing `edgegap_service-1.1.0/edgegap_service/_service.py` & `edgegap_service-1.2.0/edgegap_service/_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,193 +2,190 @@
 import inspect
 import logging
 import os
 from logging.config import dictConfig
 from pathlib import Path
 
 from edgegap_logging import Color, Format
+from edgegap_scheduling import Scheduler
 from edgegap_settings import ProjectBaseSettings
-from elasticapm.contrib.starlette import make_apm_client, ElasticAPM
-from fastapi import (
-    FastAPI,
-    staticfiles,
-    templating
-)
+from elasticapm.contrib.starlette import ElasticAPM, make_apm_client
+from fastapi import FastAPI, staticfiles, templating
 
-from edgegap_scheduling import Scheduler
 from ._configuration import ServiceConfiguration
 from ._documentation import DocumentationRoute
 from ._scheduling import SchedulingAPI
 from ._templating import TemplateRenderer
 from .health import HealthCheck
 
 current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 
 
 class ServiceFactory:
-
     def __init__(self, configuration: ServiceConfiguration) -> None:
         self.__configuration = configuration
         self.__static_folder = os.path.join(self.__configuration.root_dir, self.__configuration.static_dir)
         self.__logger: logging.Logger | None = None
         self.__app: FastAPI = None
 
     def create_app(self) -> FastAPI:
         self.__app = FastAPI(
             title=self.__configuration.name,
             description=self.__configuration.description,
             configuration=self.__configuration,
-            openapi_tags=self.__configuration.tags_definition
+            openapi_tags=self.__configuration.tags_definition,
         )
 
         Path(self.__static_folder).mkdir(parents=True, exist_ok=True)
 
         for router in self.__configuration.routers:
             self.__app.include_router(router)
 
         self.__app.mount(
-            "/static",
+            '/static',
             staticfiles.StaticFiles(
                 directory=self.__static_folder,
-                packages=[("edgegap_service", "static")]
-            ), name="static"
+                packages=[('edgegap_service', 'static')],
+            ),
+            name='static',
         )
 
         self.__logger = self.__init_logging()
 
-        service_string = f"{self.__configuration.name} ({self.__configuration.version})"
+        service_string = f'{self.__configuration.name} ({self.__configuration.version})'
         self.__logger.info(
-            f"Service {Format.squared(service_string, Color.GREEN)} is initializing"
+            f'Service {Format.squared(service_string, Color.GREEN)} is initializing',
         )
 
         self.__init_root()
         self.__init_health()
         self.__init_template_renderer()
         self.__init_apm()
         self.__init_startup_functions()
         self.__init_scheduling()
         self.__init_sigterm()
 
         return self.__app
 
     def __init_root(self):
-        folder = os.path.join(current_dir, "static", "html")
-        file_name = "index.html"
+        folder = os.path.join(current_dir, 'static', 'html')
+        file_name = 'index.html'
         is_defined = isinstance(self.__configuration.html_index_path, str)
 
         if is_defined:
             full_path = os.path.join(self.__configuration.root_dir, self.__configuration.html_index_path)
 
             if os.path.isfile(full_path):
                 folder = os.path.dirname(full_path)
                 file_name = os.path.basename(full_path)
 
         templates = templating.Jinja2Templates(directory=folder)
         DocumentationRoute.init_documentation(self.__app, file_name, templates)
         self.__logger.info(
-            f"Initialized root path and documentation with folder: {Format.squared(folder, Color.GREEN)}"
+            f'Initialized root path and documentation with folder: {Format.squared(folder, Color.GREEN)}',
         )
 
     def __init_health(self):
         health_check = HealthCheck(
             title=self.__configuration.name,
             version=self.__configuration.version,
             checks=self.__configuration.checks,
-            depend=self.__configuration.depend
+            depend=self.__configuration.depend,
         )
         health_check.init_health_check(self.__app)
 
         self.__logger.info(f"Initialized Health route at {Format.squared('/health', Color.GREEN)}")
 
     def __init_template_renderer(self):
         assert isinstance(
             TemplateRenderer.get_templates(configuration=self.__configuration),
-            templating.Jinja2Templates
+            templating.Jinja2Templates,
         )
-        self.__logger.info("Initialized Template Renderer")
+        self.__logger.info('Initialized Template Renderer')
 
     def __init_logging(self) -> logging.Logger:
         self.__init_logstash()
 
         dictConfig(self.__configuration.log_config.model_dump())
         logger = logging.getLogger(self.__configuration.name)
-        logger.info(f"Logging for service {Format.squared(self.__configuration.name, Color.GREEN)} is configured")
+        logger.info(f'Logging for service {Format.squared(self.__configuration.name, Color.GREEN)} is configured')
 
         if self.__configuration.settings and self.__configuration.settings.logstash.enabled:
-            logger.info(f"Logstash is enabled")
+            logger.info('Logstash is enabled')
 
         return logger
 
     def __init_apm(self):
         if isinstance(self.__configuration.settings, ProjectBaseSettings):
             apm = self.__configuration.settings.apm
 
             if apm.enabled:
-                self.__logger.info("Apm is enabled")
+                self.__logger.info('Apm is enabled')
                 client = make_apm_client({
                     'SERVICE_NAME': self.__configuration.name,
                     'SECRET_TOKEN': apm.token,
-                    'SERVER_URL': f"{apm.scheme}://{apm.server}:{apm.port}",
+                    'SERVER_URL': f'{apm.scheme}://{apm.server}:{apm.port}',
                 })
                 self.__app.add_middleware(ElasticAPM, client=client)
 
     def __init_logstash(self):
         if isinstance(self.__configuration.settings, ProjectBaseSettings):
             logstash = self.__configuration.settings.logstash
 
             if logstash.enabled:
                 formatter = {
-                    "logstash": {
-                        "class": "logstash_async.formatter.LogstashFormatter",
-                        "fmt": self.__configuration.env_config.log_format
-                    }
+                    'logstash': {
+                        'class': 'logstash_async.formatter.LogstashFormatter',
+                        'fmt': self.__configuration.env_config.log_format,
+                    },
                 }
                 handlers = {
-                    "logstash": {
-                        "class": "logstash_async.handler.AsynchronousLogstashHandler",
-                        "formatter": "logstash",
-                        "transport": "logstash_async.transport.TcpTransport",
-                        "args": "('%(host)s', %(port)s, '%(database_path)s', '%(transport)s', "
-                                "%(ssl_enable)s, %(ssl_verify)s, '%(keyfile)s', '%(certfile)s', "
-                                "'%(ca_certs)s', %(enable)s)",
-                        "host": logstash.server,
-                        "port": logstash.port,
-                        "enable": logstash.enabled,
-                        "ssl_enable": False,
-                        "ssl_verify": False,
-                        "database_path": None
-                    }
+                    'logstash': {
+                        'class': 'logstash_async.handler.AsynchronousLogstashHandler',
+                        'formatter': 'logstash',
+                        'transport': 'logstash_async.transport.TcpTransport',
+                        'args': "('%(host)s', %(port)s, '%(database_path)s', '%(transport)s', "
+                        "%(ssl_enable)s, %(ssl_verify)s, '%(keyfile)s', '%(certfile)s', "
+                        "'%(ca_certs)s', %(enable)s)",
+                        'host': logstash.server,
+                        'port': logstash.port,
+                        'enable': logstash.enabled,
+                        'ssl_enable': False,
+                        'ssl_verify': False,
+                        'database_path': None,
+                    },
                 }
-                self.__configuration.log_config.root["handlers"] = ["default", "logstash"]
-                self.__configuration.log_config.loggers["root"]["handlers"] = ["default", "logstash"]
+                self.__configuration.log_config.root['handlers'] = ['default', 'logstash']
+                self.__configuration.log_config.loggers['root']['handlers'] = ['default', 'logstash']
                 self.__configuration.log_config.formatters.update(formatter)
                 self.__configuration.log_config.handlers.update(handlers)
 
     def __init_scheduling(self):
         if isinstance(self.__configuration.scheduler, Scheduler):
-            @self.__app.on_event("startup")
+
+            @self.__app.on_event('startup')
             def start_scheduling():
                 SchedulingAPI().init_scheduling_api(self.__app)
                 asyncio.create_task(self.__configuration.scheduler.start_all())
 
     def __init_sigterm(self):
-        @self.__app.on_event("shutdown")
+        @self.__app.on_event('shutdown')
         def handle():
             try:
-                self.__logger.info(f"Shutting down {Format.squared(self.__configuration.name, Color.GREEN)}")
+                self.__logger.info(f'Shutting down {Format.squared(self.__configuration.name, Color.GREEN)}')
 
                 if isinstance(self.__configuration.scheduler, Scheduler):
                     asyncio.ensure_future(self.__configuration.scheduler.stop_all())
             except Exception as e:
                 self.__logger.exception(e)
 
     def __init_startup_functions(self):
-        @self.__app.on_event("startup")
+        @self.__app.on_event('startup')
         async def init_startup_functions():
             for func in self.__configuration.startup_functions:
                 try:
                     if inspect.iscoroutinefunction(func):
                         await func()
                     else:
                         func()
                 except Exception as e:
-                    self.__logger.exception(f"Could not initialize correctly one of the startup functions: {e}")
+                    self.__logger.exception(f'Could not initialize correctly one of the startup functions: {e}')
```

### Comparing `edgegap_service-1.1.0/edgegap_service/_templating.py` & `edgegap_service-1.2.0/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.1.0/edgegap_service/health/_health.py` & `edgegap_service-1.2.0/edgegap_service/health/_health.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 from typing import Callable
 
-from fastapi import (
-    FastAPI,
-    Depends,
-    responses,
-    Request
-)
+from fastapi import Depends, FastAPI, Request, responses
 
 from ._model import HealthResponse
 from .checks import CheckInterface
 
 
 class HealthCheck:
     def __init__(self, title: str, version: str, checks: list[type(CheckInterface)], depend: Callable):
@@ -22,30 +17,30 @@
         ]
         self.__depend = depend
 
     def init_health_check(self, app: FastAPI):
         def empty_depend():
             return None
 
-        @app.get("/health", response_model=HealthResponse, tags=["Monitoring"])
+        @app.get('/health', response_model=HealthResponse, tags=['Monitoring'])
         async def health(
-                request: Request,
-                session=Depends(self.__depend or empty_depend)
+            request: Request,
+            session=Depends(self.__depend or empty_depend),
         ) -> responses.JSONResponse:
             checks = []
-            kwargs = {"session": session, 'request': request}
+            kwargs = {'session': session, 'request': request}
 
             for check in self.__checks:
                 checks.append(check.check(**kwargs))
 
             all_ok = all([check.ok for check in checks])
             response = HealthResponse(
                 name=self.__title,
                 version=self.__version,
                 all_ok=all_ok,
-                checks=checks
+                checks=checks,
             )
 
             return responses.JSONResponse(
                 content=response.model_dump(),
-                status_code=200 if all_ok else 500
+                status_code=200 if all_ok else 500,
             )
```

### Comparing `edgegap_service-1.1.0/edgegap_service/health/checks/_consul.py` & `edgegap_service-1.2.0/edgegap_service/health/checks/_consul.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from edgegap_consul import ConsulReaderFactory
 
 from ._interface import CheckInterface
 from ._model import CheckInstanceModel
 
 
 class ConsulCheck(CheckInterface):
-    __name__ = "Consul"
+    __name__ = 'Consul'
 
     def __init__(self, name: str = None):
         super().__init__(name)
         self.__reader = ConsulReaderFactory().from_env()
 
     def _check(self, **kwargs) -> CheckInstanceModel:
         try:
             ok = self.__reader.check()
-            message = "ok"
+            message = 'ok'
         except Exception as e:
             ok = False
             message = str(e)
 
         return CheckInstanceModel(ok=ok, message=message)
```

### Comparing `edgegap_service-1.1.0/edgegap_service/health/checks/_database.py` & `edgegap_service-1.2.0/edgegap_service/health/checks/_database.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from edgegap_database import DatabaseOperator
-from sqlmodel import select, Session
+from sqlmodel import Session, select
 
 from ._interface import CheckInterface
 from ._model import CheckInstanceModel
 
 
 class DatabaseCheck(CheckInterface):
-    __name__ = "Database"
+    __name__ = 'Database'
 
     def _check(self, **kwargs) -> CheckInstanceModel:
         ok = False
-        message = "No Session Supplied to Database Check"
+        message = 'No Session Supplied to Database Check'
 
         session = kwargs.get('session')
 
         if isinstance(session, Session):
             try:
                 operator = DatabaseOperator(session)
                 operator.exec(select(True))
                 ok = True
-                message = "ok"
+                message = 'ok'
             except Exception as e:
                 message = str(e)
 
         return CheckInstanceModel(ok=ok, message=message)
```

### Comparing `edgegap_service-1.1.0/edgegap_service/health/checks/_interface.py` & `edgegap_service-1.2.0/edgegap_service/health/checks/_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 
-from ._model import CheckModel, CheckInstanceModel
+from ._model import CheckInstanceModel, CheckModel
 
 
 class CheckInterface(abc.ABC):
     __name__: str
 
     def __init__(self, name: str = None):
         self.__name = name if isinstance(name, str) else self.__name__
```

### Comparing `edgegap_service-1.1.0/edgegap_service/static/html/index.html` & `edgegap_service-1.2.0/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.1.0/edgegap_service/static/images/favicon.ico` & `edgegap_service-1.2.0/edgegap_service/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.1.0/pyproject.toml` & `edgegap_service-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "1.1.0"
+version = "1.2.0"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
@@ -18,11 +18,20 @@
 edgegap-consul = "^1.0.0"
 edgegap-database = "^1.0.0"
 edgegap-settings = "^1.0.0"
 edgegap-scheduling = "^1.0.0"
 edgegap-logging = "^1.0.0"
 python-logstash-async = "^3.0.0"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.2.0"
+pytest-asyncio = "^0.23.6"
+pytest-mock = "^3.14.0"
+pytest-cov = "^5.0.0"
+ruff = "^0.4.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.ruff]
+extend = "../../../3rdparty/ruff/ruff.toml"
```

### Comparing `edgegap_service-1.1.0/PKG-INFO` & `edgegap_service-1.2.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 1.1.0
+Version: 1.2.0
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

