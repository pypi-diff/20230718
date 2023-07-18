# Comparing `tmp/Akatosh-2.1.3.tar.gz` & `tmp/Akatosh-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-2.1.3.tar", last modified: Thu Jul 13 06:20:03 2023, max compression
+gzip compressed data, was "Akatosh-2.1.4.tar", last modified: Tue Jul 18 03:11:23 2023, max compression
```

## Comparing `Akatosh-2.1.3.tar` & `Akatosh-2.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 06:20:03.243374 Akatosh-2.1.3/
-drwxrwxrwx   0        0        0        0 2023-07-13 06:20:03.229376 Akatosh-2.1.3/Akatosh/
--rw-rw-rw-   0        0        0      242 2023-07-13 05:05:39.000000 Akatosh-2.1.3/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    13438 2023-07-13 06:17:06.000000 Akatosh-2.1.3/Akatosh/entity.py
--rw-rw-rw-   0        0        0    13327 2023-07-13 05:05:39.000000 Akatosh-2.1.3/Akatosh/event.py
--rw-rw-rw-   0        0        0      384 2023-07-11 12:42:40.000000 Akatosh-2.1.3/Akatosh/logger.py
--rw-rw-rw-   0        0        0     9111 2023-07-11 12:42:40.000000 Akatosh-2.1.3/Akatosh/resource.py
--rw-rw-rw-   0        0        0      201 2023-07-11 12:42:40.000000 Akatosh-2.1.3/Akatosh/states.py
--rw-rw-rw-   0        0        0     5356 2023-07-13 05:05:39.000000 Akatosh-2.1.3/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-07-13 06:20:03.239376 Akatosh-2.1.3/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-07-13 06:20:03.000000 Akatosh-2.1.3/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-13 06:20:03.000000 Akatosh-2.1.3/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 06:20:03.000000 Akatosh-2.1.3/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 06:20:03.000000 Akatosh-2.1.3/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2830 2023-07-13 06:20:03.241376 Akatosh-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-07-11 12:42:40.000000 Akatosh-2.1.3/README.md
--rw-rw-rw-   0        0        0      635 2023-07-13 06:18:52.000000 Akatosh-2.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-13 06:20:03.243374 Akatosh-2.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 03:11:23.478625 Akatosh-2.1.4/
+drwxrwxrwx   0        0        0        0 2023-07-18 03:11:23.421059 Akatosh-2.1.4/Akatosh/
+-rw-rw-rw-   0        0        0      242 2023-07-12 05:21:53.000000 Akatosh-2.1.4/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0    13438 2023-07-18 01:59:16.000000 Akatosh-2.1.4/Akatosh/entity.py
+-rw-rw-rw-   0        0        0    13327 2023-07-12 07:37:05.000000 Akatosh-2.1.4/Akatosh/event.py
+-rw-rw-rw-   0        0        0      384 2023-07-12 04:33:32.000000 Akatosh-2.1.4/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     9111 2023-07-12 04:33:32.000000 Akatosh-2.1.4/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      201 2023-07-12 04:33:32.000000 Akatosh-2.1.4/Akatosh/states.py
+-rw-rw-rw-   0        0        0     6148 2023-07-18 03:07:53.000000 Akatosh-2.1.4/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:11:23.455619 Akatosh-2.1.4/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2830 2023-07-18 03:11:23.000000 Akatosh-2.1.4/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-18 03:11:23.000000 Akatosh-2.1.4/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 03:11:23.000000 Akatosh-2.1.4/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 03:11:23.000000 Akatosh-2.1.4/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2830 2023-07-18 03:11:23.463621 Akatosh-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-07-12 04:33:32.000000 Akatosh-2.1.4/README.md
+-rw-rw-rw-   0        0        0      635 2023-07-18 03:10:59.000000 Akatosh-2.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 03:11:23.479620 Akatosh-2.1.4/setup.cfg
```

### Comparing `Akatosh-2.1.3/Akatosh/entity.py` & `Akatosh-2.1.4/Akatosh/entity.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.3/Akatosh/event.py` & `Akatosh-2.1.4/Akatosh/event.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.3/Akatosh/resource.py` & `Akatosh-2.1.4/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.3/Akatosh/universe.py` & `Akatosh-2.1.4/Akatosh/universe.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,78 +31,97 @@
         Args:
             till (int | float | None, optional): the end time of the simulated universe. Defaults to None.
 
         Raises:
             RuntimeError: raise if the event is in unknown state or being placed in wrong event queue.
         """
         while len(self.future_events) != 0:
+            
+            # stop simulation if world eater alduin is triggered.
             if self.alduin:
                 return
 
-            active_future_event = [
-                event for event in self.future_events if event.state == State.ACTIVE
+            # update the current time of the simulated universe.
+            valid_future_events = [
+                event
+                for event in self.future_events
+                if event.state == State.ACTIVE or event.state == State.INACTIVE
             ]
-            if len(active_future_event) == 0:
+            if len(valid_future_events) == 0:
                 return
-            _time = min(event.at for event in active_future_event)
+            _time = min(event.at for event in valid_future_events)
             if self.now < _time:
                 self._now = _time
-                if till is not None:
-                    if self.now > till:
-                        return
+                
+            # stop simulation if the end time is reached.
+            if till is not None:
+                if self.now > till:
+                    return
+                
             logger.debug(f"Time: {self.now}")
 
             logger.debug(
                 f"Future active events: {[(event.at, event.label) for event in self.future_events]}"
             )
 
-            for event in self.future_events[:]:
-                if event.at <= self.now:
-                    if event.state == State.ACTIVE or event.state == State.INACTIVE:
-                        logger.debug(f"Event {event.label} is triggered.")
-                        self.future_events.remove(event)
-                        self.current_events.append(event)
-                    elif event.state == State.CANCELED:
-                        raise RuntimeError(f"Event {event.label} is canceled but inside future events queue.")
-                    elif event.state == State.ENDED:
-                        raise RuntimeError(
-                            f"Event {event.label} is ended but inside future events queue."
-                        )
-                    else:
-                        raise RuntimeError(f"Event {event.label} is in unknown state.")
+            self.organise_events()
 
             logger.debug(
                 f"Current events: {[(event.priority, event.label) for event in self.current_events]}"
             )
 
-            while (
-                len(
-                    [
-                        event
-                        for event in self.current_events
-                        if event.state == State.ACTIVE
-                    ]
-                )
-                != 0
-            ):
-                priority = min(
-                    event.priority
+            await self.execute_current_events()
+            
+            
+
+    def organise_events(self):
+        """Organise the events in the future events queue. Valid event will be moved to the current events queue. Non-valid event will be moved to the past events queue.
+
+        Raises:
+            RuntimeError: raise if the event is in unknown state or being placed in wrong event queue.
+        """
+        for event in self.future_events[:]:
+            if event.at <= self.now:
+                if event.state == State.ACTIVE or event.state == State.INACTIVE:
+                    logger.debug(f"Event {event.label} is triggered.")
+                    self.future_events.remove(event)
+                    self.current_events.append(event)
+                elif event.state == State.CANCELED:
+                    raise RuntimeError(
+                            f"Event {event.label} is canceled but inside future events queue."
+                        )
+                elif event.state == State.ENDED:
+                    raise RuntimeError(
+                            f"Event {event.label} is ended but inside future events queue."
+                        )
+                else:
+                    raise RuntimeError(f"Event {event.label} is in unknown state.")
+
+    async def execute_current_events(self):
+        """Execute the current events queue based on priority. The event with the lowest priority will be executed first. The event with the same priority will be executed concurrently.
+        """
+        while (
+            len([event for event in self.current_events if event.state == State.ACTIVE])
+            != 0
+        ):
+            priority = min(
+                event.priority
+                for event in self.current_events
+                if event.state == State.ACTIVE
+            )
+            logger.debug(
+                f"Current Priority: {priority}, Executing events: {[event.label for event in self.current_events if event.priority == priority]}"
+            )
+            await asyncio.gather(
+                *[
+                    event._perform()
                     for event in self.current_events
-                    if event.state == State.ACTIVE
-                )
-                logger.debug(
-                    f"Current Priority: {priority}, Executing events: {[event.label for event in self.current_events if event.priority == priority]}"
-                )
-                await asyncio.gather(
-                    *[
-                        event._perform()
-                        for event in self.current_events
-                        if event.priority == priority
-                    ]
-                )
+                    if event.priority == priority
+                ]
+            )
 
     def simulate(self, till: int | float | None = None):
         """Start the simulation."""
         asyncio.run(self.akatosh(till))
 
     def set_logger(self, level: int):
         """Set the logger level."""
```

### Comparing `Akatosh-2.1.3/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.1.4/Akatosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.3
+Version: 2.1.4
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.3/PKG-INFO` & `Akatosh-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.3
+Version: 2.1.4
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.3/README.md` & `Akatosh-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.3/pyproject.toml` & `Akatosh-2.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "2.1.3"
+version = "2.1.4"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

