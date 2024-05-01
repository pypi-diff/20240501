# Comparing `tmp/edgegap_scheduling-1.1.0.tar.gz` & `tmp/edgegap_scheduling-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_scheduling-1.1.0.tar", max compression
+gzip compressed data, was "edgegap_scheduling-1.2.0.tar", max compression
```

## Comparing `edgegap_scheduling-1.1.0.tar` & `edgegap_scheduling-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1993 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/LICENSE
--rw-r--r--   0        0        0     2164 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/README.md
--rw-r--r--   0        0        0       17 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/BUILD
--rw-r--r--   0        0        0      280 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/__init__.py
--rw-r--r--   0        0        0      128 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/_depends.py
--rw-r--r--   0        0        0     4233 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/_runner.py
--rw-r--r--   0        0        0     4477 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/_scheduler.py
--rw-r--r--   0        0        0     1289 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/_signature.py
--rw-r--r--   0        0        0      482 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/_singleton.py
--rw-r--r--   0        0        0     1233 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/_sleep.py
--rw-r--r--   0        0        0      188 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/_state.py
--rw-r--r--   0        0        0     4220 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/_task.py
--rw-r--r--   0        0        0       17 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/errors/BUILD
--rw-r--r--   0        0        0      132 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/errors/__init__.py
--rw-r--r--   0        0        0      103 2024-04-30 16:04:37.495396 edgegap_scheduling-1.1.0/edgegap_scheduling/errors/_errors.py
--rw-r--r--   0        0        0      501 2024-04-30 16:04:54.559540 edgegap_scheduling-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 edgegap_scheduling-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2164 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/BUILD
+-rw-r--r--   0        0        0      281 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/__init__.py
+-rw-r--r--   0        0        0      128 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_depends.py
+-rw-r--r--   0        0        0     4269 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_runner.py
+-rw-r--r--   0        0        0     4436 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_scheduler.py
+-rw-r--r--   0        0        0     1303 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_signature.py
+-rw-r--r--   0        0        0      482 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_singleton.py
+-rw-r--r--   0        0        0     1233 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_sleep.py
+-rw-r--r--   0        0        0      188 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_state.py
+-rw-r--r--   0        0        0     4221 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/_task.py
+-rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/errors/BUILD
+-rw-r--r--   0        0        0      133 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/errors/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-01 17:52:18.963014 edgegap_scheduling-1.2.0/edgegap_scheduling/errors/_errors.py
+-rw-r--r--   0        0        0      702 2024-05-01 17:52:46.827698 edgegap_scheduling-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 edgegap_scheduling-1.2.0/PKG-INFO
```

### Comparing `edgegap_scheduling-1.1.0/LICENSE` & `edgegap_scheduling-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.1.0/README.md` & `edgegap_scheduling-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.1.0/edgegap_scheduling/_runner.py` & `edgegap_scheduling-1.2.0/edgegap_scheduling/_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 
 from pydantic import BaseModel
 
 from ._signature import TaskSignature
 from ._state import TaskState
 from ._task import Task
 
-logger = logging.getLogger("scheduling.Runner")
+logger = logging.getLogger('scheduling.Runner')
 
 
 class TaskRunner:
     def __init__(self, task: Task, sleep: Callable):
         super().__init__()
         self.__task = task
         self.__sleep = sleep
         self.__signature = TaskSignature(task.identifier, task.name, task.func)
 
     def __str__(self):
-        return f"Runner: {self.__task}"
+        return f'Runner: {self.__task}'
 
     @property
     def should_schedule(self) -> bool:
         return self.__task.need_to_loop
 
     def get_task(self) -> Task:
         return self.__task.model_copy()
 
     def update_task(
-            self,
-            every: str | None,
-            delay: str | None,
-            parameters: dict | None = None
+        self,
+        every: str | None,
+        delay: str | None,
+        parameters: dict | None = None,
     ):
         if isinstance(every, str):
             self.__task.every = every or None
 
         if isinstance(delay, str):
             self.__task.delay = delay or None
 
@@ -52,71 +52,74 @@
         self.__task.sleep_at = None
         self.__task.begin_at = None
         self.__task.stopped_at = None
 
     async def start(self):
         if self.__task.safe_to_start:
             try:
-                logger.info(f"Starting {self.__task}")
+                logger.info(f'Starting {self.__task}')
                 self.__update_task_start()
 
                 if self.__task.should_delay:
                     await self.__sleep(self.__task.identifier, self.__task.delay_in_seconds)
 
                 if self.__task.need_to_loop:
                     await self.__loop()
                     self.__task.state = TaskState.STOPPED
-                    logger.info(f"{self.__task} Stopped")
+                    logger.info(f'{self.__task} Stopped')
                 else:
                     await self.__run()
                     self.__task.state = TaskState.COMPLETED
-                    logger.info(f"{self.__task} Completed")
+                    logger.info(f'{self.__task} Completed')
             except Exception as e:
-                logger.exception(f"{self.__task} raised an exception: {e}")
+                logger.exception(f'{self.__task} raised an exception: {e}')
                 self.__task.state = TaskState.ERROR
                 self.__task.error = str(e)
 
             self.__task.stopped_at = datetime.now(tz=timezone.utc)
 
     async def __loop(self):
         while self.__task.state == TaskState.RUNNING:
             try:
                 self.__task.begin_at = datetime.now(tz=timezone.utc)
                 await self.__run()
             except Exception as e:
                 if self.__task.continue_on_exception:
-                    logger.exception(f"{self.__task} raised an exception, continuing since defined by the task: {e}")
+                    logger.exception(f'{self.__task} raised an exception, continuing since defined by the task: {e}')
                 else:
                     raise e
 
             if self.__task.every_in_seconds is None:
-                logger.warning(f"Every changed in task {self.__task.name} without stopping it first!")
+                logger.warning(f'Every changed in task {self.__task.name} without stopping it first!')
                 break
 
             sleep_duration = self.__task.next_sleep_duration
 
             if sleep_duration <= 0 and self.__task.remove_running_time:
-                logger.warning(f"{self.__task.name} process for too long and the sleep duration is zero!")
+                logger.warning(f'{self.__task.name} process for too long and the sleep duration is zero!')
 
             elif sleep_duration is None:
                 sleep_duration = self.__task.every_in_seconds
 
             self.__task.sleep_at = datetime.now(tz=timezone.utc)
+
             await self.__sleep(self.__task.identifier, sleep_duration)
 
     async def __run(self, parameters: BaseModel | type[BaseModel] | None = None):
         arguments, generators = self.__signature.get_arguments(parameters or self.__task.parameters)
 
-        for name, generator in generators.items():
-            arguments[name] = next(generator)
-
-        await self.__task.func(**arguments)
-
-        for generator in generators.values():
-            generator.close()
+        try:
+            for name, generator in generators.items():
+                arguments[name] = next(generator)
+
+            await self.__task.func(**arguments)
+
+        finally:
+            for generator in generators.values():
+                generator.close()
 
     def stop(self) -> bool:
         can_stop = self.__task.state == TaskState.RUNNING
 
         if can_stop:
             self.__task.state = TaskState.STOPPING
```

### Comparing `edgegap_scheduling-1.1.0/edgegap_scheduling/_scheduler.py` & `edgegap_scheduling-1.2.0/edgegap_scheduling/_scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,141 +1,141 @@
 import asyncio
 import logging
 
-from edgegap_logging import Format, Color
+from edgegap_logging import Color, Format
 from pydantic import BaseModel
 
 from ._runner import TaskRunner
 from ._sleep import AsyncSleep
 from ._task import Task
 from .errors import ManualRunNotAllowedError
 
 
 class Scheduler:
-
     def __init__(self, timeout: int = 10):
         self.timeout = timeout
         self.__runners: dict[str, TaskRunner] = {}
-        self.logger = logging.getLogger("scheduling.Scheduler")
+        self.logger = logging.getLogger('scheduling.Scheduler')
         self.__async_sleep = AsyncSleep()
 
     def task(
-            self,
-            every: str = None,
-            name: str = None,
-            delay: str = None,
-            identifier: str = None,
-            continue_on_exception: bool = True,
-            manual_run_allowed: bool = False,
-            remove_running_time: bool = False,
-            parameters: BaseModel | type[BaseModel] | None = None
+        self,
+        every: str = None,
+        name: str = None,
+        delay: str = None,
+        identifier: str = None,
+        continue_on_exception: bool = True,
+        manual_run_allowed: bool = False,
+        remove_running_time: bool = False,
+        parameters: BaseModel | type[BaseModel] | None = None,
     ):
         def decorator(func):
             task = Task(
                 name=name or func.__name__,
-                identifier=identifier or name.lower().replace(" ", "_"),
+                identifier=identifier or name.lower().replace(' ', '_'),
                 func=func,
                 every=every,
                 delay=delay,
                 continue_on_exception=continue_on_exception,
                 manual_run_allowed=manual_run_allowed,
                 remove_running_time=remove_running_time,
-                parameters=parameters if isinstance(parameters, BaseModel) or parameters is None else parameters()
+                parameters=parameters if isinstance(parameters, BaseModel) or parameters is None else parameters(),
             )
             runner = TaskRunner(
                 task=task,
-                sleep=self.__async_sleep.sleep
+                sleep=self.__async_sleep.sleep,
             )
             self.__register(task.identifier, runner)
 
         return decorator
 
     def __register(self, identifier: str, runner: TaskRunner) -> None:
         if identifier in self.__runners.keys():
-            raise Exception(f"Task {Format.squared(identifier, Color.RED)} already exists")
+            raise Exception(f'Task {Format.squared(identifier, Color.RED)} already exists')
 
         self.__runners[identifier] = runner
 
     def __get_or_raise(self, identifier: str) -> TaskRunner:
         runner = self.__runners.get(identifier)
 
         if runner is None:
-            raise ValueError(f"Task [{identifier}] does not exist")
+            raise ValueError(f'Task [{identifier}] does not exist')
 
         return runner
 
     async def get(self, identifier) -> Task:
         runner = self.__get_or_raise(identifier)
         return runner.get_task()
 
     async def update(
-            self, identifier: str,
-            every: str | None,
-            delay: str | None,
-            parameters: dict | None
+        self,
+        identifier: str,
+        every: str | None,
+        delay: str | None,
+        parameters: dict | None,
     ) -> Task:
         runner = self.__get_or_raise(identifier)
         runner.update_task(
             every=every,
             delay=delay,
-            parameters=parameters
+            parameters=parameters,
         )
 
         return runner.get_task()
 
     async def list(self) -> list[Task]:
         return [runner.get_task() for runner in self.__runners.values()]
 
     async def start(self, identifier: str) -> Task:
         runner = self.__get_or_raise(identifier)
-        self.logger.info(f"Starting {runner}")
+        self.logger.info(f'Starting {runner}')
         task = runner.get_task()
 
         if task.safe_to_start:
             asyncio.ensure_future(runner.start())
         else:
-            task.message = "Task already started"
+            task.message = 'Task already started'
 
         return task
 
     async def start_all(self):
-        self.logger.info("Starting All Tasks")
+        self.logger.info('Starting All Tasks')
         for runner in self.__runners.values():
             if runner.should_schedule:
                 await runner.start()
 
     async def stop(self, identifier: str) -> Task:
         runner = self.__get_or_raise(identifier)
-        self.logger.info(f"Stopping {runner}")
+        self.logger.info(f'Stopping {runner}')
         can_stop = runner.stop()
         task = runner.get_task()
 
         if can_stop:
             await self.__async_sleep.cancel_one(identifier)
         else:
-            task.message = "Could not stop the task since it is not in a running state"
+            task.message = 'Could not stop the task since it is not in a running state'
 
         return task
 
     async def run(self, name: str, parameters: dict | None = None) -> Task:
         runner = self.__get_or_raise(name)
 
         task = runner.get_task()
 
         if not task.manual_run_allowed:
-            raise ManualRunNotAllowedError(f"Task [{name}] is not allowed to be run manually")
+            raise ManualRunNotAllowedError(f'Task [{name}] is not allowed to be run manually')
 
         params = task.parameters.model_copy(update=parameters) if isinstance(parameters, dict) else None
 
         await runner.run(params)
 
         return runner.get_task()
 
     async def stop_all(self):
-        self.logger.info(f"Stopping All Running Tasks")
+        self.logger.info('Stopping All Running Tasks')
 
         for runner in self.__runners.values():
             runner.stop()
-            self.logger.info(f"Stopping {runner}")
+            self.logger.info(f'Stopping {runner}')
 
         count = await self.__async_sleep.cancel_all()
-        self.logger.info(f"{count} tasks stopped")
+        self.logger.info(f'{count} tasks stopped')
```

### Comparing `edgegap_scheduling-1.1.0/edgegap_scheduling/_signature.py` & `edgegap_scheduling-1.2.0/edgegap_scheduling/_signature.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import inspect
 import logging
 from types import GeneratorType
-from typing import Callable, Any
+from typing import Any, Callable
 
 from pydantic import BaseModel
 
 from ._depends import Depends
 
 
 class TaskSignature:
     def __init__(self, identifier: str, name: str, func: Callable):
         self.__identifier = identifier
         self.__name = name
         self.__func = func
 
-    def get_arguments(self, parameters: BaseModel | type[BaseModel] | None = None) -> tuple[
-        dict[str, Any], dict[str, Any]]:
+    def get_arguments(
+        self,
+        parameters: BaseModel | type[BaseModel] | None = None,
+    ) -> tuple[dict[str, Any], dict[str, Any]]:
         specs = {}
         generators = {}
         signature = inspect.signature(self.__func)
 
         for name, param in signature.parameters.items():
             match param.annotation:
                 case logging.Logger:
-                    specs[name] = logging.getLogger(f"scheduling.{self.__identifier}")
+                    specs[name] = logging.getLogger(f'scheduling.{self.__identifier}')
                 case parameters.__class__:
                     specs[name] = parameters
                 case parameters:
                     specs[name] = parameters()
 
             match param.default:
                 case Depends():
```

### Comparing `edgegap_scheduling-1.1.0/edgegap_scheduling/_sleep.py` & `edgegap_scheduling-1.2.0/edgegap_scheduling/_sleep.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.1.0/edgegap_scheduling/_task.py` & `edgegap_scheduling-1.2.0/edgegap_scheduling/_task.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from datetime import datetime, timezone
 from typing import Callable
 
-from edgegap_logging import Format, Color
+from edgegap_logging import Color, Format
 from pydantic import BaseModel, Field, computed_field
 from pytimeparse import parse
 
 from ._state import TaskState
 
 
 class Task(BaseModel):
-    identifier: str = Field(default=None, description="The identifier of the Task")
-    name: str = Field(..., description="The name of the Task")
-    every: str | None = Field(default=None, description="The interval to run the Task")
-    delay: str | None = Field(default=None, description="Delay before starting the Task")
-    state: TaskState = Field(default=TaskState.PENDING, description="The Current Task State")
-    func: Callable = Field(..., description="The function to call", exclude=True)
-    message: str | None = Field(default=None, description="The message from the Task or Runner")
-    error: str | None = Field(default=None, description="The error message")
-    started_at: datetime | None = Field(default=None, description="The start time of the Task")
-    begin_at: datetime | None = Field(default=None, description="The last time of the Task began")
-    sleep_at: datetime | None = Field(default=None, description="The last time where the Task slept")
-    stopped_at: datetime | None = Field(default=None, description="The Time the Task stopped")
-    continue_on_exception: bool = Field(default=True, description="If the Task continue after an exception")
-    manual_run_allowed: bool = Field(default=False, description="If the Task can be manually run")
-    remove_running_time: bool = Field(default=False, description="If the Sleep needs to remove the running time")
+    identifier: str = Field(default=None, description='The identifier of the Task')
+    name: str = Field(..., description='The name of the Task')
+    every: str | None = Field(default=None, description='The interval to run the Task')
+    delay: str | None = Field(default=None, description='Delay before starting the Task')
+    state: TaskState = Field(default=TaskState.PENDING, description='The Current Task State')
+    func: Callable = Field(..., description='The function to call', exclude=True)
+    message: str | None = Field(default=None, description='The message from the Task or Runner')
+    error: str | None = Field(default=None, description='The error message')
+    started_at: datetime | None = Field(default=None, description='The start time of the Task')
+    begin_at: datetime | None = Field(default=None, description='The last time of the Task began')
+    sleep_at: datetime | None = Field(default=None, description='The last time where the Task slept')
+    stopped_at: datetime | None = Field(default=None, description='The Time the Task stopped')
+    continue_on_exception: bool = Field(default=True, description='If the Task continue after an exception')
+    manual_run_allowed: bool = Field(default=False, description='If the Task can be manually run')
+    remove_running_time: bool = Field(default=False, description='If the Sleep needs to remove the running time')
     parameters: BaseModel | type[BaseModel] | None = Field(
         default=None,
-        description="The parameters of the Task to inject on runtime"
+        description='The parameters of the Task to inject on runtime',
     )
 
     def __str__(self):
         return (
-            f"Task {Format.squared(self.name, Color.GREEN)} - "
-            f"Every {Format.squared(self.every, Color.GREEN)} - "
-            f"Delay {Format.squared(self.delay, Color.GREEN)} - "
-            f"{self.state}"
+            f'Task {Format.squared(self.name, Color.GREEN)} - '
+            f'Every {Format.squared(self.every, Color.GREEN)} - '
+            f'Delay {Format.squared(self.delay, Color.GREEN)} - '
+            f'{self.state}'
         )
 
     @property
     def every_in_seconds(self) -> float | None:
         return parse(self.every) if isinstance(self.every, str) else None
 
     @property
@@ -49,49 +49,49 @@
     def should_delay(self) -> bool:
         return isinstance(self.delay_in_seconds, (float, int))
 
     @property
     def need_to_loop(self) -> bool:
         return isinstance(self.every_in_seconds, (float, int))
 
-    @computed_field(description="If the Task is safe to start")
+    @computed_field(description='If the Task is safe to start')
     @property
     def safe_to_start(self) -> bool:
         return self.state in [TaskState.PENDING, TaskState.COMPLETED, TaskState.STOPPED, TaskState.ERROR]
 
-    @computed_field(description="For how long the task did the processing before sleeping")
+    @computed_field(description='For how long the task did the processing before sleeping')
     @property
     def last_processing_duration(self) -> float | None:
         if self.begin_at and self.sleep_at:
             if self.begin_at < self.sleep_at:
                 return (self.sleep_at - self.begin_at).total_seconds()
 
-    @computed_field(description="If the task is currently processing or sleeping")
+    @computed_field(description='If the task is currently processing or sleeping')
     @property
     def is_processing(self) -> bool:
         is_running = False
 
         if self.begin_at and self.sleep_at:
             is_running = self.begin_at > self.sleep_at
         elif self.begin_at and self.sleep_at is None:
             is_running = True
 
         return is_running
 
-    @computed_field(description="If the task is currently sleeping (will be false if the task is not running)")
+    @computed_field(description='If the task is currently sleeping (will be false if the task is not running)')
     @property
     def is_sleeping(self) -> bool:
         is_sleeping = False
 
         if self.begin_at and self.sleep_at:
             is_sleeping = self.sleep_at > self.begin_at
 
         return is_sleeping
 
-    @computed_field(description="The Time to sleep remaining")
+    @computed_field(description='The Time to sleep remaining')
     @property
     def next_sleep_duration(self) -> float | None:
         if self.is_processing:
             time_since_start = (datetime.now(tz=timezone.utc) - self.begin_at).total_seconds()
             diff = max(self.every_in_seconds - time_since_start, 0)
 
             return self.every_in_seconds if not self.remove_running_time else diff
```

### Comparing `edgegap_scheduling-1.1.0/PKG-INFO` & `edgegap_scheduling-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-scheduling
-Version: 1.1.0
+Version: 1.2.0
 Summary: The Edgegap Scheduling library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

