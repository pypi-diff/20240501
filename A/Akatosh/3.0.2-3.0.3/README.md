# Comparing `tmp/akatosh-3.0.2.tar.gz` & `tmp/akatosh-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akatosh-3.0.2.tar", max compression
+gzip compressed data, was "akatosh-3.0.3.tar", max compression
```

## Comparing `akatosh-3.0.2.tar` & `akatosh-3.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      546 2024-05-01 01:03:37.389203 akatosh-3.0.2/Akatosh/__init__.py
--rw-r--r--   0        0        0     4911 2024-05-01 01:03:37.390209 akatosh-3.0.2/Akatosh/entity.py
--rw-r--r--   0        0        0     6051 2024-05-01 03:23:36.963728 akatosh-3.0.2/Akatosh/event.py
--rw-r--r--   0        0        0     5230 2024-05-01 01:03:37.391211 akatosh-3.0.2/Akatosh/resource.py
--rw-r--r--   0        0        0     7286 2024-05-01 03:19:13.357671 akatosh-3.0.2/Akatosh/universe.py
--rw-r--r--   0        0        0      321 2024-05-01 05:15:06.777438 akatosh-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     2324 2024-05-01 01:03:37.392209 akatosh-3.0.2/README.md
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 akatosh-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0      546 2024-05-01 01:03:37.389203 akatosh-3.0.3/Akatosh/__init__.py
+-rw-r--r--   0        0        0     5333 2024-05-01 06:18:14.039666 akatosh-3.0.3/Akatosh/entity.py
+-rw-r--r--   0        0        0     6273 2024-05-01 06:22:47.670314 akatosh-3.0.3/Akatosh/event.py
+-rw-r--r--   0        0        0     5230 2024-05-01 01:03:37.391211 akatosh-3.0.3/Akatosh/resource.py
+-rw-r--r--   0        0        0     7286 2024-05-01 03:19:13.357671 akatosh-3.0.3/Akatosh/universe.py
+-rw-r--r--   0        0        0      321 2024-05-01 06:25:25.462460 akatosh-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2324 2024-05-01 01:03:37.392209 akatosh-3.0.3/README.md
+-rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 akatosh-3.0.3/PKG-INFO
```

### Comparing `akatosh-3.0.2/Akatosh/__init__.py` & `akatosh-3.0.3/Akatosh/__init__.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.2/Akatosh/entity.py` & `akatosh-3.0.3/Akatosh/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,21 +34,26 @@
         self._till = till
         self._created = False
         self._terminated = False
         self._priority = priority
 
         # create an instant creation event
         self._creation = Event(
-            at, inf, self._create, f"{self} Creation", once=True, priority=self.priority
+            at=at,
+            till=till,
+            action=self._create,
+            label=f"{self} Creation",
+            once=True,
+            priority=self.priority,
         )
         self._termination = Event(
-            till,
-            inf,
-            self._terminate,
-            f"{self} Termination",
+            at=till,
+            till=till,
+            action=self._terminate,
+            label=f"{self} Termination",
             once=True,
             priority=self.priority,
         )
 
         # create a queue for engaged events
         self._events: List[Event] = list()
 
@@ -75,14 +80,15 @@
             resource.collect(self, inf)
         logger.debug(f"Entity {self} terminated.")
 
     def event(
         self,
         at: float | Event,
         till: float | Event,
+        step: float = Mundus.time_step,
         label: Optional[str] = None,
         once: bool = False,
         priority: int = 0,
     ):
         """Decorator to add an event to the entity."""
 
         def _event(action: Callable):
@@ -96,19 +102,29 @@
                 while True:
                     if not self.created:
                         logger.warn(f"Entity {self} not created yet.")
                         await asyncio.sleep(0)
                     else:
                         break
 
-                event = Event(at, till, action, label, once, priority)
+                event = Event(
+                    at=at,
+                    till=till,
+                    step=step,
+                    action=action,
+                    label=label,
+                    once=once,
+                    priority=priority,
+                )
                 self.events.append(event)
                 logger.debug(f"Event {event} added to entity {self}.")
 
-            Event(at, at, __event, f"{label} Engagement", True)
+            Event(
+                at=at, till=at, action=__event, label=f"{label} Engagement", once=True
+            )
 
         return _event
 
     def acquire(self, resource: Resource, amount: float) -> bool:
         """Acquire a amount from the resource."""
         if resource.distribute(self, amount):
             return True
```

### Comparing `akatosh-3.0.2/Akatosh/event.py` & `akatosh-3.0.3/Akatosh/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 class Event:
 
     def __init__(
         self,
         at: float | Event,
         till: float | Event,
         action: Callable,
+        step: float = Mundus.time_step,
         label: Optional[str] = None,
         once: bool = False,
         priority: int = 0,
     ) -> None:
         """Create an event which happens at a certain time and ends at a certain time.
 
         Args:
@@ -36,14 +37,15 @@
         self._started = False
         self._acted = False
         self._ended = False
         self._paused = False
         self._label = label
         self._once = once
         self._priority = priority
+        self._step = step
         self._next = 0
         Mundus.pending_events.append(self)
         if self.priority > Mundus.max_event_priority:
             Mundus._max_event_priority = self.priority
 
     async def __call__(self) -> Any:
         """Make the event callable, so it can be awaited like a coroutine."""
@@ -72,14 +74,16 @@
 
             if (
                 self.started == True
                 and self.ended == False
                 and self.paused == False
                 and self.next == Mundus.time
             ):
+                self._next += max(Mundus.time_step, self.step)
+                self._next = round(self._next, Mundus.time_resolution)
                 if asyncio.iscoroutinefunction(self._action):
                     await self._action()
                 else:
                     self._action()
                 self._acted = True
                 logger.debug(f"Event {self} acted.")
                 if self._once == True:
@@ -89,25 +93,19 @@
 
             if self.ended == False:
                 if isinstance(self.till, Event):
                     if self.till.ended == True:
                         self._ended = True
                         logger.debug(f"Event {self} ended.")
                         return
-                    else:
-                        self._next += Mundus.time_step
-                        self._next = round(self._next, Mundus.time_resolution)
                 else:
                     if self.till <= Mundus.time:
                         self._ended = True
                         logger.debug(f"Event {self} ended.")
                         return
-                    else:
-                        self._next += Mundus.time_step
-                        self._next = round(self._next, Mundus.time_resolution)
             await asyncio.sleep(0)
 
     def __str__(self) -> str:
         """Return the label of the event if it has one, otherwise return the id of the event."""
         if self.label is None:
             return f"Event {id(self)}"
         return self.label
@@ -168,19 +166,33 @@
         return self._priority
 
     @property
     def next(self):
         """Return the next time the event acts."""
         return self._next
 
+    @property
+    def step(self):
+        """Return the time step of the event, which overwrites the simulation time step."""
+        return self._step
+
 
 def event(
     at: float | Event,
     till: float | Event,
+    step: float = Mundus.time_step,
     label: Optional[str] = None,
     once: bool = False,
     priority: int = 0,
 ):
     def _event(action: Callable) -> Event:
-        return Event(at, till, action, label, once, priority)
+        return Event(
+            at=at,
+            till=till,
+            step=step,
+            action=action,
+            label=label,
+            once=once,
+            priority=priority,
+        )
 
     return _event
```

### Comparing `akatosh-3.0.2/Akatosh/resource.py` & `akatosh-3.0.3/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.2/Akatosh/universe.py` & `akatosh-3.0.3/Akatosh/universe.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.2/README.md` & `akatosh-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.2/PKG-INFO` & `akatosh-3.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 3.0.2
+Version: 3.0.3
 Summary: 
 Author: Innovation Central Perth Maintainer
 Author-email: ryf0510@live.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

