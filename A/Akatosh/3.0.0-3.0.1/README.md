# Comparing `tmp/akatosh-3.0.0.tar.gz` & `tmp/akatosh-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akatosh-3.0.0.tar", max compression
+gzip compressed data, was "akatosh-3.0.1.tar", max compression
```

## Comparing `akatosh-3.0.0.tar` & `akatosh-3.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      546 2024-04-10 03:45:43.677095 akatosh-3.0.0/Akatosh/__init__.py
--rw-r--r--   0        0        0     4911 2024-04-22 03:58:25.918223 akatosh-3.0.0/Akatosh/entity.py
--rw-r--r--   0        0        0     5591 2024-04-22 03:58:25.996779 akatosh-3.0.0/Akatosh/event.py
--rw-r--r--   0        0        0     5230 2024-04-22 03:53:18.056982 akatosh-3.0.0/Akatosh/resource.py
--rw-r--r--   0        0        0     5576 2024-04-22 03:58:25.939267 akatosh-3.0.0/Akatosh/universe.py
--rw-r--r--   0        0        0      340 2024-04-22 02:03:33.682580 akatosh-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2324 2024-04-19 03:36:27.289023 akatosh-3.0.0/README.md
--rw-r--r--   0        0        0     2666 1970-01-01 00:00:00.000000 akatosh-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      546 2024-05-01 01:03:37.389203 akatosh-3.0.1/Akatosh/__init__.py
+-rw-r--r--   0        0        0     4911 2024-05-01 01:03:37.390209 akatosh-3.0.1/Akatosh/entity.py
+-rw-r--r--   0        0        0     6051 2024-05-01 03:23:36.963728 akatosh-3.0.1/Akatosh/event.py
+-rw-r--r--   0        0        0     5230 2024-05-01 01:03:37.391211 akatosh-3.0.1/Akatosh/resource.py
+-rw-r--r--   0        0        0     7286 2024-05-01 03:19:13.357671 akatosh-3.0.1/Akatosh/universe.py
+-rw-r--r--   0        0        0      322 2024-05-01 03:32:45.315243 akatosh-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2324 2024-05-01 01:03:37.392209 akatosh-3.0.1/README.md
+-rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 akatosh-3.0.1/PKG-INFO
```

### Comparing `akatosh-3.0.0/Akatosh/__init__.py` & `akatosh-3.0.1/Akatosh/__init__.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.0/Akatosh/entity.py` & `akatosh-3.0.1/Akatosh/entity.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.0/Akatosh/event.py` & `akatosh-3.0.1/Akatosh/event.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import asyncio
+import time
 from typing import Any, Callable, Optional
 from . import logger
 from .universe import Mundus
 
 
 class Event:
 
@@ -25,26 +26,25 @@
             label (Optional[str], optional): Short description for the event. Defaults to None.
             once (bool, optional): whether this event should only happen once, regardless of at or till. Defaults to False.
             priority (int, optional): the priority of the event, event with lower value will happen before the events with a higher priority value. Defaults to 0.
 
         Raises:
             ValueError: _description_
         """
-        # if universe.time >= at:
-        #     raise ValueError(f"Event can only be scheduled for the future.")
         self._at = at
         self._till = till
         self._action = action
         self._started = False
         self._acted = False
         self._ended = False
         self._paused = False
         self._label = label
         self._once = once
         self._priority = priority
+        self._next = 0
         Mundus.pending_events.append(self)
         if self.priority > Mundus.max_event_priority:
             Mundus._max_event_priority = self.priority
 
     async def __call__(self) -> Any:
         """Make the event callable, so it can be awaited like a coroutine."""
         while True:
@@ -58,21 +58,28 @@
                 else:
                     await asyncio.sleep(0)
 
             if self.started == False:
                 if isinstance(self.at, Event):
                     if self.at.ended == True:
                         self._started = True
+                        self._next = Mundus.time
                         logger.debug(f"Event {self} started.")
                 else:
                     if self.at <= Mundus.time:
                         self._started = True
+                        self._next = Mundus.time
                         logger.debug(f"Event {self} started.")
 
-            if self.started == True and self.ended == False and self.paused == False:
+            if (
+                self.started == True
+                and self.ended == False
+                and self.paused == False
+                and self.next == Mundus.time
+            ):
                 if asyncio.iscoroutinefunction(self._action):
                     await self._action()
                 else:
                     self._action()
                 self._acted = True
                 logger.debug(f"Event {self} acted.")
                 if self._once == True:
@@ -82,23 +89,26 @@
 
             if self.ended == False:
                 if isinstance(self.till, Event):
                     if self.till.ended == True:
                         self._ended = True
                         logger.debug(f"Event {self} ended.")
                         return
+                    else:
+                        self._next += Mundus.time_step
+                        self._next = round(self._next, Mundus.time_resolution)
                 else:
                     if self.till <= Mundus.time:
                         self._ended = True
                         logger.debug(f"Event {self} ended.")
                         return
-            if Mundus.realtime == True:
-                await asyncio.sleep(Mundus.time_step)
-            else:
-                await asyncio.sleep(0)
+                    else:
+                        self._next += Mundus.time_step
+                        self._next = round(self._next, Mundus.time_resolution)
+            await asyncio.sleep(0)
 
     def __str__(self) -> str:
         """Return the label of the event if it has one, otherwise return the id of the event."""
         if self.label is None:
             return f"Event {id(self)}"
         return self.label
 
@@ -153,14 +163,19 @@
         return self._once
 
     @property
     def priority(self):
         """Return the priority of the event."""
         return self._priority
 
+    @property
+    def next(self):
+        """Return the next time the event acts."""
+        return self._next
+
 
 def event(
     at: float | Event,
     till: float | Event,
     label: Optional[str] = None,
     once: bool = False,
     priority: int = 0,
```

### Comparing `akatosh-3.0.0/Akatosh/resource.py` & `akatosh-3.0.1/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.0/Akatosh/universe.py` & `akatosh-3.0.1/Akatosh/universe.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,77 +20,95 @@
         return cls._instance
 
     def __init__(self) -> None:
         """The simulation universe."""
         self._time_resolution = 3
         self._time_step = round(1 / pow(10, self.time_resolution), self.time_resolution)
         self._time = 0
+        self._elapsed_time = 0
+        self._time_difference = 0
+        self._simulation_start_time = 0
+        self._simulation_end_time = 0
         self._realtime = False
         self._current_event_priority = 0
         self._max_event_priority = 0
         self._pending_events: List[Event] = list()
 
     def simulate(self, till: float):
         """Simulate the universe until the given time."""
 
         # Define the flow of time
         async def time_flow():
             """Flow of time."""
-            simulation_start_time = time.time()
+            self._simulation_start_time = time.perf_counter()
             while self.time < till:
-                logger.debug(f"Time:\t{self.time}")
+                logger.debug(f"Simulation time:\t{self.time}")
                 for event in self.pending_events:
                     asyncio.create_task(event())
                 self.pending_events.clear()
                 if self.realtime:
-                    start_time = time.time()
+                    logger.debug(f"Iteration started at Real Time: {time.perf_counter() - self.simulation_start_time:0.6f}")
                     # iterate through all event priorities
                     self._current_event_priority = 0
                     while self.current_event_priority <= self._max_event_priority:
                         logger.debug(
                             f"Current Event Priority: {self.current_event_priority}"
                         )
                         await asyncio.sleep(0)
                         self._current_event_priority += 1
                     # wait for the time step
-                    await asyncio.sleep(self.time_step)
-                    end_time = time.time()
-                    if end_time - start_time > self.time_step:
-                        logger.warning(
-                            f"Simulation time step exceeded real time by {round(end_time - start_time - self.time_step,6)}."
-                        )
-                    else:
-                        logger.debug(
-                            f"Simulation time step completed in {round(end_time - start_time, 3)} seconds."
-                        )
+                    self._time += self.time_step
+                    self._time = round(self.time, self.time_resolution)
+                    logger.debug(f"Iteration finished at Real Time: {time.perf_counter() - self.simulation_start_time:0.6f}")
+                    logger.debug(f"Waiting for next interation...")
+                    while time.perf_counter() - self.simulation_start_time < self.time:
+                        await asyncio.sleep(0)
+                    # self._elapsed_time = (
+                    #     time.perf_counter() - self.simulation_start_time
+                    # )
+                    # self._time_difference = self.time - self.elapsed_time
+                    # logger.debug(
+                    #     f"Current Real Time: {self.elapsed_time:0.3f}."
+                    # )
+                    # waiting_time = max(0, self.time_difference)
+                    # logger.debug(
+                    #     f"Waiting for {waiting_time:0.3f} seconds."
+                    # )
+                    # before = time.perf_counter()
+                    # await asyncio.sleep(waiting_time)
+                    # after = time.perf_counter()
+                    # logger.debug(
+                    #     f"Actual waiting time: {after - before:0.3f} seconds."
+                    # )
+                    
                 else:
                     # iterate through all event priorities
                     self._current_event_priority = 0
                     while self.current_event_priority <= self._max_event_priority:
                         logger.debug(
                             f"Current Event Priority: {self.current_event_priority}"
                         )
                         await asyncio.sleep(0)
                         self._current_event_priority += 1
                     # wait for the time step
+                    self._time += self.time_step
+                    self._time = round(self.time, self.time_resolution)
                     await asyncio.sleep(0)
-                self._time += self.time_step
-                self._time = round(self.time, self.time_resolution)
 
-            simulation_end_time = time.time()
+            self._simulation_end_time = time.perf_counter()
             if self.realtime:
                 logger.info(
-                    f"Simulation completed in {round(simulation_end_time - simulation_start_time, 6)} seconds, exceeding real time by {round(((simulation_end_time - simulation_start_time - till)/till)*100,2)}%."
+                    f"Simulation completed in {round(self.simulation_end_time - self.simulation_start_time, 6)} seconds, exceeding real time by {round(((self.simulation_end_time - self.simulation_start_time - till)/till)*100,2)}%."
                 )
 
-        asyncio.run(time_flow())
+        return time_flow()
 
-    def enable_realtime(self):
+    def enable_realtime(self, time_resolution: int = 3):
         """Enable the real time simulation. Time step will be adjusted to 0.1s."""
-        self.time_resolution = 1
+        self.time_resolution = time_resolution
         self._time_step = round(1 / pow(10, self.time_resolution), self.time_resolution)
         self._realtime = True
 
     def set_logging_level(self, level: int = logging.DEBUG):
         """Set the logging level. Default is DEBUG."""
         logger.setLevel(level)
 
@@ -135,9 +153,29 @@
         return self._current_event_priority
 
     @property
     def max_event_priority(self):
         """The maximum event priority."""
         return self._max_event_priority
 
+    @property
+    def elapsed_time(self):
+        """The real elapsed time of the simulation."""
+        return self._elapsed_time
+
+    @property
+    def time_difference(self):
+        """The time difference between the real time and simulation time."""
+        return self._time_difference
+
+    @property
+    def simulation_start_time(self):
+        """The time when the simulation started."""
+        return self._simulation_start_time
+
+    @property
+    def simulation_end_time(self):
+        """The time when the simulation ended."""
+        return self._simulation_end_time
+
 
 Mundus = Universe()
```

### Comparing `akatosh-3.0.0/README.md` & `akatosh-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.0/PKG-INFO` & `akatosh-3.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 3.0.0
+Version: 3.0.1
 Summary: 
 Author: Innovation Central Perth Maintainer
 Author-email: ryf0510@live.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorlog (>=6.8.2,<7.0.0)
-Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Akatosh
 
 `Akatosh` is a light-weighted disceret event simulation library. Unlike popular library `Simpy` which is progress-oriented and you have to write generator function for simulated events or events interaction, `Akatosh` is fully object-oriented that events are encapsulated as `InstantEvent`/`ContinousEvent` with states, priority and a life-cycle. The actual impact of events are simply regular python functions. You could create events all at once, or create event within event. In addition, `Akatosh` is async which means event that are happening at the same simulated time will be executed simultaneously for real, unless they have different priority.
 
 `Akatosh` also support `Resource`, provide all functionalities as it is in `Simpy` with extra utilities for telemetries collection and interaction with `Entity`. The `Entity` is unique to `Akatosh` which represents a abstract entity with a life-cycle, for example a follower. The `Entity` supports utility functions to interact with `Resource` and automatically releases all its occupied resources upon termination.
```

