# Comparing `tmp/Akatosh-2.1.4.tar.gz` & `tmp/Akatosh-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-2.1.4.tar", last modified: Tue Jul 18 03:11:23 2023, max compression
+gzip compressed data, was "Akatosh-2.1.5.tar", last modified: Tue Jul 18 06:12:28 2023, max compression
```

## Comparing `Akatosh-2.1.4.tar` & `Akatosh-2.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 03:11:23.478625 Akatosh-2.1.4/
-drwxrwxrwx   0        0        0        0 2023-07-18 03:11:23.421059 Akatosh-2.1.4/Akatosh/
--rw-rw-rw-   0        0        0      242 2023-07-12 05:21:53.000000 Akatosh-2.1.4/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    13438 2023-07-18 01:59:16.000000 Akatosh-2.1.4/Akatosh/entity.py
--rw-rw-rw-   0        0        0    13327 2023-07-12 07:37:05.000000 Akatosh-2.1.4/Akatosh/event.py
--rw-rw-rw-   0        0        0      384 2023-07-12 04:33:32.000000 Akatosh-2.1.4/Akatosh/logger.py
--rw-rw-rw-   0        0        0     9111 2023-07-12 04:33:32.000000 Akatosh-2.1.4/Akatosh/resource.py
--rw-rw-rw-   0        0        0      201 2023-07-12 04:33:32.000000 Akatosh-2.1.4/Akatosh/states.py
--rw-rw-rw-   0        0        0     6148 2023-07-18 03:07:53.000000 Akatosh-2.1.4/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:11:23.455619 Akatosh-2.1.4/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-07-18 03:11:23.000000 Akatosh-2.1.4/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-18 03:11:23.000000 Akatosh-2.1.4/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 03:11:23.000000 Akatosh-2.1.4/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-18 03:11:23.000000 Akatosh-2.1.4/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2830 2023-07-18 03:11:23.463621 Akatosh-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-07-12 04:33:32.000000 Akatosh-2.1.4/README.md
--rw-rw-rw-   0        0        0      635 2023-07-18 03:10:59.000000 Akatosh-2.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 03:11:23.479620 Akatosh-2.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 06:12:28.896546 Akatosh-2.1.5/
+drwxrwxrwx   0        0        0        0 2023-07-18 06:12:28.838981 Akatosh-2.1.5/Akatosh/
+-rw-rw-rw-   0        0        0      242 2023-07-12 05:21:53.000000 Akatosh-2.1.5/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0    14879 2023-07-18 06:06:44.000000 Akatosh-2.1.5/Akatosh/entity.py
+-rw-rw-rw-   0        0        0    13327 2023-07-12 07:37:05.000000 Akatosh-2.1.5/Akatosh/event.py
+-rw-rw-rw-   0        0        0      384 2023-07-12 04:33:32.000000 Akatosh-2.1.5/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     9111 2023-07-12 04:33:32.000000 Akatosh-2.1.5/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      201 2023-07-12 04:33:32.000000 Akatosh-2.1.5/Akatosh/states.py
+-rw-rw-rw-   0        0        0     6148 2023-07-18 03:07:53.000000 Akatosh-2.1.5/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-07-18 06:12:28.884548 Akatosh-2.1.5/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2830 2023-07-18 06:12:28.000000 Akatosh-2.1.5/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-18 06:12:28.000000 Akatosh-2.1.5/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 06:12:28.000000 Akatosh-2.1.5/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 06:12:28.000000 Akatosh-2.1.5/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2830 2023-07-18 06:12:28.893546 Akatosh-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-07-12 04:33:32.000000 Akatosh-2.1.5/README.md
+-rw-rw-rw-   0        0        0      635 2023-07-18 06:11:53.000000 Akatosh-2.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 06:12:28.896546 Akatosh-2.1.5/setup.cfg
```

### Comparing `Akatosh-2.1.4/Akatosh/entity.py` & `Akatosh-2.1.5/Akatosh/entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import abstractmethod
 from collections.abc import Iterable
 from typing import Callable, Iterable, List
 from uuid import uuid4
 
 from Akatosh.universe import Mundus
 
@@ -13,30 +15,34 @@
 
 class Entity:
     def __init__(
         self,
         label: str | None = None,
         create_at: int | float | Callable | None = None,
         terminate_at: int | float | Callable | None = None,
+        precursor: Entity | List[Entity] | None = None,
     ) -> None:
         """Create a entity.
 
         Args:
             label (str | None, optional): short description of the entity. Defaults to None.
             create_at (int | float | Callable | None, optional): when the life cycle of this entity should start. Defaults to None, then must call create() method manually.
             terminate_at (int | float | Callable | None, optional): when the life cycle of this entity should end. Defaults to None, then must call terminate() method manually.
         """
         self._id = uuid4().int
         self._label = label
         self._state: List[str] = list()
         self._occupied_resources: List[Resource] = list()
         self._registered_lists: List[EntityList] = list()
         self._creation: InstantEvent = None  # type: ignore
+        self._created_at: int | float = float()
         self._termination: InstantEvent = None  # type: ignore
+        self._terminated_at: int | float = float()
         self._events: List[Event] = list()
+        self._precursor = precursor
 
         if create_at is not None:
             if callable(create_at):
                 self.create(at=round(create_at(), Mundus.resolution))
             else:
                 self.create(at=round(create_at, Mundus.resolution))
 
@@ -49,33 +55,53 @@
     def create(self, at: int | float) -> None:
         """The creation of the entity."""
 
         def _create():
             if self.terminated:
                 raise RuntimeError(f"Entity {self.label} is already terminated.")
             self._state.append(State.CREATED)
+            self._created_at = Mundus.now
             self.on_creation()
             logger.debug(f"Entity {self.label} created at {Mundus.now}")
 
-        self._creation = InstantEvent(
-            at=at, action=_create, label=f"Creation of {self.label}", priority=-2
-        )
+        if self.precursor is None:
+            self._creation = InstantEvent(
+                at=at, action=_create, label=f"Creation of {self.label}", priority=-2
+            )
+        else:
+            if isinstance(self.precursor, list):
+                self._creation = InstantEvent(
+                    at=at,
+                    action=_create,
+                    label=f"Creation of {self.label}",
+                    priority=-2,
+                    precursor=[e._termination for e in self.precursor],
+                )
+            else:
+                self._creation = InstantEvent(
+                    at=at,
+                    action=_create,
+                    label=f"Creation of {self.label}",
+                    priority=-2,
+                    precursor=self.precursor._termination,
+                )
 
     @abstractmethod
     def on_creation(self):
         """Callback function upon creation of the entity"""
         pass
 
     def terminate(self, at: int | float) -> None:
         """The termination of the entity. This will release all occupied resource, remove the entity from all entity lists, and cancel all unfinished events."""
 
         def _terminate():
             if not self.created:
                 raise RuntimeError(f"Entity {self.label} is not created yet.")
             self._state.append(State.TERMINATED)
+            self._terminated_at = Mundus.now
             self.release_resources()
             self.unregister_from_lists()
             self.cancel_unfinished_events()
             self.on_termination()
             logger.debug(f"Entity {self.label} terminated at {Mundus.now}")
 
         self._termination = InstantEvent(
@@ -239,33 +265,48 @@
 
     @property
     def created(self):
         """Return True if the entity is created."""
         return State.CREATED in self.state
 
     @property
+    def created_at(self):
+        """Return the time when the entity is created."""
+        return self._created_at
+
+    @property
     def terminated(self):
         """Return True if the entity is terminated."""
         return State.TERMINATED in self.state
 
     @property
+    def terminated_at(self):
+        """Return the time when the entity is terminated."""
+        return self._terminated_at
+
+    @property
     def ocupied_resources(self):
         """Return the resources occupied by the entity."""
         return self._occupied_resources
 
     @property
     def registered_lists(self):
         """Return the entity lists contains the entity."""
         return self._registered_lists
 
     @property
     def events(self):
         """Return the events engaged by the entity."""
         return self._events
 
+    @property
+    def precursor(self):
+        """Return the precursor(s) of the entity."""
+        return self._precursor
+
 
 class EntityList(list):
     """Customized list for entities. This list ensures all items are entities and unique. When an entity is terminated, it will be removed from all entity lists automatically."""
 
     def __init__(self, iterable: Iterable[Entity] = [], label: str | None = None):
         """Create a list for entities, with optional label.
```

### Comparing `Akatosh-2.1.4/Akatosh/event.py` & `Akatosh-2.1.5/Akatosh/event.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.4/Akatosh/resource.py` & `Akatosh-2.1.5/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.4/Akatosh/universe.py` & `Akatosh-2.1.5/Akatosh/universe.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.4/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.1.5/Akatosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.4
+Version: 2.1.5
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.4/PKG-INFO` & `Akatosh-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.4
+Version: 2.1.5
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.4/README.md` & `Akatosh-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.4/pyproject.toml` & `Akatosh-2.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "2.1.4"
+version = "2.1.5"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

