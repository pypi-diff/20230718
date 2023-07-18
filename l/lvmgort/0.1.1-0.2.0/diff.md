# Comparing `tmp/lvmgort-0.1.1.tar.gz` & `tmp/lvmgort-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvmgort-0.1.1.tar", max compression
+gzip compressed data, was "lvmgort-0.2.0.tar", max compression
```

## Comparing `lvmgort-0.1.1.tar` & `lvmgort-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1504 2023-07-14 22:08:11.780650 lvmgort-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      713 2023-07-14 22:08:11.781031 lvmgort-0.1.1/README.md
--rw-r--r--   0        0        0     2665 2023-07-14 22:08:11.794285 lvmgort-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      540 2023-07-14 22:08:11.795162 lvmgort-0.1.1/src/gort/__init__.py
--rw-r--r--   0        0        0      713 2023-07-14 22:08:11.795511 lvmgort-0.1.1/src/gort/__main__.py
--rw-r--r--   0        0        0     6727 2023-07-14 22:08:11.795895 lvmgort-0.1.1/src/gort/core.py
--rw-r--r--   0        0        0      386 2023-07-14 22:08:11.796299 lvmgort-0.1.1/src/gort/devices/__init__.py
--rw-r--r--   0        0        0     3604 2023-07-14 22:08:11.796655 lvmgort-0.1.1/src/gort/devices/ag.py
--rw-r--r--   0        0        0     2917 2023-07-14 22:08:11.797012 lvmgort-0.1.1/src/gort/devices/enclosure.py
--rw-r--r--   0        0        0    12353 2023-07-14 22:08:11.797381 lvmgort-0.1.1/src/gort/devices/guider.py
--rw-r--r--   0        0        0     1446 2023-07-14 22:08:11.797701 lvmgort-0.1.1/src/gort/devices/nps.py
--rw-r--r--   0        0        0    16357 2023-07-14 22:08:11.798098 lvmgort-0.1.1/src/gort/devices/spec.py
--rw-r--r--   0        0        0    24865 2023-07-14 22:08:11.798519 lvmgort-0.1.1/src/gort/devices/telescope.py
--rw-r--r--   0        0        0     5088 2023-07-14 22:08:11.799030 lvmgort-0.1.1/src/gort/etc/lvmgort.yml
--rw-r--r--   0        0        0     3511 2023-07-14 22:08:11.799343 lvmgort-0.1.1/src/gort/exceptions.py
--rw-r--r--   0        0        0    14444 2023-07-14 22:08:11.799967 lvmgort-0.1.1/src/gort/gort.py
--rw-r--r--   0        0        0     4582 2023-07-14 22:08:11.800754 lvmgort-0.1.1/src/gort/kubernetes.py
--rw-r--r--   0        0        0     1002 2023-07-14 22:08:11.801127 lvmgort-0.1.1/src/gort/maskbits.py
--rw-r--r--   0        0        0    16601 2023-07-14 22:08:11.801560 lvmgort-0.1.1/src/gort/observer.py
--rw-r--r--   0        0        0    17411 2023-07-14 22:08:11.802025 lvmgort-0.1.1/src/gort/tile.py
--rw-r--r--   0        0        0    15629 2023-07-14 22:08:11.802492 lvmgort-0.1.1/src/gort/tools.py
--rw-r--r--   0        0        0     8584 2023-07-14 22:08:11.802931 lvmgort-0.1.1/src/gort/transforms.py
--rw-r--r--   0        0        0     5161 2023-07-14 22:08:11.803310 lvmgort-0.1.1/src/gort/websocket.py
--rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 lvmgort-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-18 21:35:09.855142 lvmgort-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0      713 2023-07-18 21:35:09.855506 lvmgort-0.2.0/README.md
+-rw-r--r--   0        0        0     2727 2023-07-18 21:35:09.869620 lvmgort-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      574 2023-07-18 21:35:09.870478 lvmgort-0.2.0/src/gort/__init__.py
+-rw-r--r--   0        0        0      713 2023-07-18 21:35:09.870770 lvmgort-0.2.0/src/gort/__main__.py
+-rw-r--r--   0        0        0     6727 2023-07-18 21:35:09.871081 lvmgort-0.2.0/src/gort/core.py
+-rw-r--r--   0        0        0      386 2023-07-18 21:35:09.871441 lvmgort-0.2.0/src/gort/devices/__init__.py
+-rw-r--r--   0        0        0     3604 2023-07-18 21:35:09.871756 lvmgort-0.2.0/src/gort/devices/ag.py
+-rw-r--r--   0        0        0     2917 2023-07-18 21:35:09.874482 lvmgort-0.2.0/src/gort/devices/enclosure.py
+-rw-r--r--   0        0        0    12438 2023-07-18 21:35:09.874920 lvmgort-0.2.0/src/gort/devices/guider.py
+-rw-r--r--   0        0        0     1446 2023-07-18 21:35:09.875271 lvmgort-0.2.0/src/gort/devices/nps.py
+-rw-r--r--   0        0        0    27651 2023-07-18 21:35:09.875735 lvmgort-0.2.0/src/gort/devices/spec.py
+-rw-r--r--   0        0        0    25965 2023-07-18 21:35:09.876229 lvmgort-0.2.0/src/gort/devices/telescope.py
+-rw-r--r--   0        0        0     2511 2023-07-18 21:35:09.876679 lvmgort-0.2.0/src/gort/etc/calibration_schema.json
+-rw-r--r--   0        0        0     5082 2023-07-18 21:35:09.877019 lvmgort-0.2.0/src/gort/etc/lvmgort.yml
+-rw-r--r--   0        0        0     3555 2023-07-18 21:35:09.877406 lvmgort-0.2.0/src/gort/exceptions.py
+-rw-r--r--   0        0        0    16443 2023-07-18 21:35:09.877820 lvmgort-0.2.0/src/gort/gort.py
+-rw-r--r--   0        0        0     4582 2023-07-18 21:35:09.878203 lvmgort-0.2.0/src/gort/kubernetes.py
+-rw-r--r--   0        0        0     1002 2023-07-18 21:35:09.878518 lvmgort-0.2.0/src/gort/maskbits.py
+-rw-r--r--   0        0        0    16766 2023-07-18 21:35:09.878919 lvmgort-0.2.0/src/gort/observer.py
+-rw-r--r--   0        0        0    17411 2023-07-18 21:35:09.879337 lvmgort-0.2.0/src/gort/tile.py
+-rw-r--r--   0        0        0    16862 2023-07-18 21:35:09.879781 lvmgort-0.2.0/src/gort/tools.py
+-rw-r--r--   0        0        0     8584 2023-07-18 21:35:09.880173 lvmgort-0.2.0/src/gort/transforms.py
+-rw-r--r--   0        0        0     5939 2023-07-18 21:35:09.880531 lvmgort-0.2.0/src/gort/websocket.py
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 lvmgort-0.2.0/PKG-INFO
```

### Comparing `lvmgort-0.1.1/LICENSE.md` & `lvmgort-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.1/README.md` & `lvmgort-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.1/pyproject.toml` & `lvmgort-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lvmgort"
-version = "0.1.1"
+version = "0.2.0"
 description = "The brains of LVM observing"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmgort"
 repository = "https://github.com/sdss/lvmgort"
 documentation = "https://lvmgort.readthedocs.org"
@@ -38,14 +38,17 @@
 tqdm = "^4.65.0"
 kubernetes = "^26.1.0"
 astropy = "^5.3.1"
 websockets = "^11.0.3"
 peewee = "^3.16.2"
 psycopg2-binary = "^2.9.6"
 pandas = "^2.0.3"
+jsonschema = "^4.18.3"
+unclick = ">=0.1.0b5"
+rich = "^13.4.2"
 
 [tool.poetry.group.dev.dependencies]
 ipython = ">=8.0.0"
 matplotlib = ">=3.1.1"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 pytest = ">=5.2.2"
```

### Comparing `lvmgort-0.1.1/src/gort/__init__.py` & `lvmgort-0.2.0/src/gort/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sdsstools import get_config, get_logger, get_package_version
 
 
 # pip package name
 NAME = "lvmgort"
 
 # Loads config. config name is the package name.
-config = get_config(NAME)
+config = get_config(NAME, config_envvar="GORT_CONFIG_FILE")
 
 log = get_logger(NAME)
 log.sh.setLevel(logging.INFO)
 log.sh.formatter.print_time = True  # type:ignore
 
 
 # package name should be pip package name
```

### Comparing `lvmgort-0.1.1/src/gort/__main__.py` & `lvmgort-0.2.0/src/gort/__main__.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.1/src/gort/core.py` & `lvmgort-0.2.0/src/gort/core.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.1/src/gort/devices/ag.py` & `lvmgort-0.2.0/src/gort/devices/ag.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.1/src/gort/devices/enclosure.py` & `lvmgort-0.2.0/src/gort/devices/enclosure.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.1/src/gort/devices/guider.py` & `lvmgort-0.2.0/src/gort/devices/guider.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             if "measured_pointing" in reply.body:
                 self.separation = reply.body["measured_pointing"]["separation"]
 
     async def wait_until_guiding(
         self,
         guide_tolerance: float | None = None,
         timeout: float | None = None,
-    ) -> tuple[bool, GuiderStatus, float | None]:
+    ) -> tuple[bool, GuiderStatus, float | None, bool]:
         """Waits until the guider has converged.
 
         Parameters
         ----------
         guide_tolerance
             The minimum separation, in arcsec, between the measured and desired
             positions that needs to be reached before returning. If `None`,
@@ -81,14 +81,16 @@
         -------
         reached
             Whether the desired minimum separation was reached.
         status
             The current `.GS`.
         separation
             The current separation.
+        timedout
+            `True` if the acquisition timed out.
 
         """
 
         # Initial delay to allow time for the guider to switch to DRIFTING status.
         await asyncio.sleep(1)
 
         elapsed = 1
@@ -97,19 +99,19 @@
                 self.status is not None
                 and self.separation is not None
                 and self.status & GuiderStatus.GUIDING
                 and not self.status & GuiderStatus.DRIFTING
                 and (guide_tolerance is None or self.separation < guide_tolerance)
             )
             if has_acquired:
-                return (True, self.status, self.separation)
+                return (True, self.status, self.separation, False)
 
             elapsed += 1
             if timeout is not None and elapsed > timeout:
-                return (False, self.status, self.separation)
+                return (False, self.status, self.separation, True)
 
             await asyncio.sleep(1)
 
     async def expose(self, *args, continuous: bool = False, **kwargs):
         """Exposes this telescope cameras.
 
         Parameters
```

### Comparing `lvmgort-0.1.1/src/gort/devices/nps.py` & `lvmgort-0.2.0/src/gort/devices/nps.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.1/src/gort/devices/spec.py` & `lvmgort-0.2.0/src/gort/observer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,510 +1,480 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
 # @Author: José Sánchez-Gallego (gallegoj@uw.edu)
-# @Date: 2023-06-15
-# @Filename: spec.py
+# @Date: 2023-07-09
+# @Filename: observer.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import asyncio
-import json
-import pathlib
-import warnings
+import logging
+import re
 from contextlib import suppress
+from time import time
 
 from typing import TYPE_CHECKING
 
-from sdsstools.time import get_sjd
-
-from gort import config
-from gort.exceptions import GortSpecError
-from gort.gort import GortDevice, GortDeviceSet
-from gort.tools import is_notebook, move_mask_interval
+from gort.exceptions import GortObserverError
+from gort.tile import Coordinates
+from gort.tools import register_observation
 
 
 if TYPE_CHECKING:
-    from tqdm import tqdm as tqdm_type
-
-    from gort.core import ActorReply
-    from gort.gort import GortClient
-
+    from gort.gort import Gort
+    from gort.tile import Tile
 
-__all__ = ["Spectrograph", "SpectrographSet", "Exposure", "READOUT_TIME"]
 
+__all__ = ["GortObserver"]
 
-READOUT_TIME = 51
 
-
-class Exposure(asyncio.Future["Exposure"]):
-    """A class representing an exposure taken by a `.SpectrographSet`.
+class GortObserver:
+    """A class to handle tile observations.
 
     Parameters
     ----------
-    exp_no
-        The exposure sequence number.
-    spec_set
-        The `.SpectrographSet` commanding this exposure.
+    gort
+        The instance of `.Gort` used to communicate with the devices.
+    tile
+        The `.Tile` with the information about the observation.
+    mask_positions_pattern
+        The ``spec`` fibre mask positions to use.
 
     """
 
-    def __init__(self, exp_no: int, spec_set: SpectrographSet):
-        self.spec_set = spec_set
-        self.exp_no = exp_no
-
-        self.error: bool = False
-        self.reading: bool = False
+    def __init__(self, gort: Gort, tile: Tile, mask_positions_pattern: str = "P1-*"):
+        self.gort = gort
+        self.tile = tile
 
-        self._timer_task: asyncio.Task | None = None
-        self._tqdm: tqdm_type | None = None
+        self.mask_positions = self._get_mask_positions(mask_positions_pattern)
 
-        super().__init__()
+        self.guide_task: asyncio.Future | None = None
 
     def __repr__(self):
-        return (
-            f"<Exposure (exp_no={self.exp_no}, error={self.error}, "
-            f"reading={self.reading}, done={self.done()})>"
-        )
+        return f"<GortObserver (tile_id={self.tile.tile_id})>"
 
-    async def expose(
-        self,
-        exposure_time: float | None = None,
-        header: str | None = None,
-        async_readout: bool = False,
-        show_progress: bool = False,
-        **kwargs,
-    ):
-        """Exposes the spectrograph.
+    async def slew(self):
+        """Slew to the telescope fields."""
 
-        Parameters
-        ----------
-        exposure_time
-            The exposure time.
-        header
-            The header JSON string to pass to the ``lvmscp expose`` command.
-        async_readout
-            Returns after integration completes. Readout is initiated
-            but handled asynchronously and can be await by awaiting
-            the returned `.Exposure` object.
-        show_progress
-            Displays a progress bar with the elapsed exposure time.
-        kwargs
-            Keyword arguments to pass to ``lvmscp expose``.
+        cotasks = []
 
-        """
+        # Stops guiders.
+        await self.gort.guiders.stop()
 
-        if show_progress and exposure_time:
-            await self.start_timer(exposure_time)
+        # Slew telescopes.
+        self.write_to_log(f"Slewing to tile_id={self.tile.tile_id}.", level="info")
 
-        if (
-            exposure_time is None
-            and kwargs.get("flavour", "object") != "bias"
-            and not kwargs.get("bias", False)
-        ):
-            raise GortSpecError(
-                "Exposure time required for all flavours except bias.",
-                error_code=3,
-            )
+        sci = (self.tile.sci_coords.ra, self.tile.sci_coords.dec)
+        self.write_to_log(f"Science: {str(self.tile.sci_coords)}")
 
-        warnings.filterwarnings("ignore", message=".*cannot modify a done command.*")
-
-        self.spec_set.last_exposure = self
-
-        try:
-            await self.spec_set._send_command_all(
-                "expose",
-                exposure_time=exposure_time,
-                seqno=self.exp_no,
-                header=(header or "{}"),
-                async_readout=async_readout,
-                **kwargs,
+        spec = None
+        if self.tile.spec_coords and len(self.tile.spec_coords) > 0:
+            # For spec we slew to the fibre with which we'll observe first.
+            # This should save a bit of time converging.
+            spec_target = (self.tile.spec_coords[0].ra, self.tile.spec_coords[0].dec)
+            # spec = fibre_slew_coordinates(*spec_target, self.mask_positions[0])
+            spec = spec_target
+            self.write_to_log(
+                f"Spec: {self.tile.spec_coords[0]} on {self.mask_positions[0]}"
             )
 
-            self.reading = True
-
-            # Now launch the task that marks the Future done when the spec
-            # is IDLE. If async_readout=False then that will return immediately
-            # because the spec is already idle. If async_readout=True, this method
-            # will return now and the task will mark the Future done when readout
-            # complete (readout is ongoing and does not need to be launched).
-            monitor_task = asyncio.create_task(self._done_monitor())
-            if not async_readout:
-                await monitor_task
-            else:
-                self.spec_set.write_to_log("Returning with async readout ongoing.")
+        sky = {}
+        for skytel in ["SkyE", "SkyW"]:
+            if skytel.lower() in self.tile.sky_coords:
+                sky_coords_tel = self.tile.sky_coords[skytel.lower()]
+                sky[skytel.lower()] = (sky_coords_tel.ra, sky_coords_tel.dec)
+                self.write_to_log(f"{skytel}: {sky_coords_tel}")
+
+        cotasks.append(
+            self.gort.telescopes.goto(
+                sci=sci,
+                spec=spec,
+                skye=sky.get("skye", None),
+                skyw=sky.get("skyw", None),
+            )
+        )
 
-        except Exception as err:
-            await self.stop_timer()
-            self.error = True
-            raise GortSpecError(f"Exposure failed with error {err}", error_code=301)
+        # Move fibsel to first position.
+        fibsel = self.gort.telescopes.spec.fibsel
+        cotasks.append(fibsel.move_to_position(self.mask_positions[0]))
 
-        return self
+        # Execute.
+        await asyncio.gather(*cotasks)
 
-    async def start_timer(
+    async def acquire(
         self,
-        exposure_time: float,
-        readout_time: float | None = READOUT_TIME,
+        guide_tolerance: float = 3,
+        timeout: float = 180,
+        min_skies: int = 1,
+        require_spec: bool = False,
     ):
-        """Starts the tqdm timer."""
-
-        if is_notebook():
-            from tqdm.notebook import tqdm
-        else:
-            from tqdm import tqdm
-
-        async def update_timer(max_time: int):
-            while True:
-                if self._tqdm is None:
-                    return
-                if self._tqdm.n >= max_time:
-                    return
-                await asyncio.sleep(1)
-                self._tqdm.update()
-
-        def done_timer(*_):
-            if self._tqdm:
-                self._tqdm.close()
-                self._tqdm = None
-                self._timer_task = None
-
-        total_time = int(exposure_time + (readout_time or 0.0))
-        bar_format = "{l_bar}{bar}| {n_fmt}/{total_fmt}s"
-
-        self._tqdm = tqdm(total=total_time, bar_format=bar_format)
-        self._tqdm.refresh()
-
-        self._timer_task = asyncio.create_task(update_timer(total_time))
-        self._timer_task.add_done_callback(done_timer)
-
-        return self._timer_task
-
-    async def stop_timer(self):
-        """Cancels the timer."""
-
-        if self._tqdm:
-            # sys.stdout = sys.__stdout__
-            # sys.stderr = sys.__stderr__
-            self._tqdm.disable = True
-            self._tqdm.close()
-        self._tqdm = None
-
-        if self._timer_task and not self._timer_task.done():
-            self._timer_task.cancel()
-            with suppress(asyncio.CancelledError):
-                await self._timer_task
-        self._timer_task = None
-
-    def get_files(self):
-        """Returns the files written by the exposure."""
-
-        sjd = get_sjd()
-        data_path = pathlib.Path(config["specs"]["data_path"].format(SJD=sjd))
-
-        return list(data_path.glob(f"*-[0]*{self.exp_no}.fits.gz"))
-
-    async def _done_monitor(self):
-        """Waits until the spectrographs are idle, and marks the Future done."""
-
-        await self.spec_set._send_command_all("wait_until_idle", allow_errored=True)
-
-        for spec in self.spec_set.values():
-            reply = await spec.status()
-            if "ERROR" in reply["status_names"]:
-                self.error = True
-
-        self.reading = False
-
-        # Set the Future.
-        self.set_result(self)
-
-
-class Spectrograph(GortDevice):
-    """Class representing an LVM spectrograph functionality."""
-
-    def __init__(self, gort: GortClient, name: str, actor: str, **kwargs):
-        super().__init__(gort, name, actor)
-
-    async def status(self):
-        """Retrieves the status of the telescope."""
-
-        reply: ActorReply = await self.actor.commands.status()
-        flatten_reply = reply.flatten()
-
-        return flatten_reply.get("status", {})
-
-    async def is_idle(self):
-        """Returns `True` if the spectrograph is idle and ready to expose."""
-
-        status = await self.status()
-        names = status["status_names"]
-        return "IDLE" in names and "READOUT_PENDING" not in names
-
-    async def is_exposing(self):
-        """Returns `True` if the spectrograph is exposing."""
+        """Acquires the field in all the telescopes. Blocks until then.
 
-        status = await self.status()
-        return "EXPOSING" in status["status_names"]
-
-    async def is_reading(self):
-        """Returns `True` if the spectrograph is idle and ready to expose."""
+        Parameters
+        ----------
+        guide_tolerance
+            The guide tolerance in arcsec. A telescope will not be considered
+            to be guiding if its separation to the commanded field is larger
+            than this value.
+        timeout
+            The maximum time allowed for acquisition. In case of timeout
+            the acquired fields are evaluated and an exception is
+            raised if the acquisition failed.
+        min_skies
+            Minimum number of skies required to consider acquisition successful.
+        require_spec
+            Whether to require the ``spec`` telescope to be guiding.
+
+        Raises
+        ------
+        GortObserverError
+            If the acquisition failed or the minimum required telescopes are
+            not guiding.
 
-        status = await self.status()
-        return "READING" in status["status_names"]
+        """
 
-    async def expose(self, **kwargs):
-        """Exposes the spectrograph."""
+        # Determine telescopes on which to guide.
 
-        if not (await self.is_idle()):
-            raise GortSpecError(
-                "Spectrographs is not idle. Cannot expose.",
-                error_code=301,
+        guide_coros = []
+        guide_on_telescopes: list[str] = []
+        n_skies = 0
+        for tel in ["sci", "skye", "skyw", "spec"]:
+            coords = self.tile[tel]
+
+            if coords is None or (isinstance(coords, list) and len(coords) == 0):
+                continue
+
+            if tel == "spec" and isinstance(coords, list):
+                coords = coords[0]
+            assert isinstance(coords, Coordinates)
+
+            guide_on_telescopes.append(tel)
+            if "sky" in tel:
+                n_skies += 1
+
+            # Pixel in the MF on which to guide. Always None/central pixel
+            # except for sci if defined. For spec we guide on the pixel of the
+            # first fibre/mask position.
+            pixel = coords._mf_pixel if tel != "spec" else self.mask_positions[0]
+
+            guide_coros.append(
+                self.gort.guiders[tel].guide(
+                    ra=coords.ra,
+                    dec=coords.dec,
+                    guide_tolerance=guide_tolerance,
+                    pixel=pixel,
+                )
             )
 
-        self.write_to_log(f"Exposing spectrograph {self.name}.")
-
-        await self.actor.commands.expose(**kwargs)
-
-
-class SpectrographSet(GortDeviceSet[Spectrograph]):
-    """A set of LVM spectrographs."""
-
-    __DEVICE_CLASS__ = Spectrograph
-
-    def __init__(self, gort: GortClient, data: dict[str, dict], **kwargs):
-        super().__init__(gort, data, **kwargs)
-
-        self.last_exposure: Exposure | None = None
-
-    async def status(self) -> dict[str, dict]:
-        """Collects the status of each spectrograph."""
-
-        names = list(self)
-        statuses = await self.call_device_method(Spectrograph.status)
-
-        return dict(zip(names, statuses))
-
-    def get_seqno(self):
-        """Returns the next exposure sequence number."""
+        if "spec" not in guide_on_telescopes:
+            if require_spec:
+                raise GortObserverError("spec pointing not defined.", error_code=801)
+            else:
+                self.write_to_log("No standards. Blocking fibre mask.", "warning")
+                await self.gort.telescopes.spec.fibsel.move_relative(500)
+        if n_skies < min_skies:
+            raise GortObserverError("Not enough sky positions defined.", error_code=801)
+
+        # Start guide loop.
+        self.guide_task = asyncio.gather(*guide_coros)
+
+        await asyncio.sleep(5)
+
+        # Wait until convergence.
+        self.write_to_log("Waiting for guiders to converge.")
+        guide_status = await asyncio.gather(
+            *[
+                self.gort.guiders[tel].wait_until_guiding(timeout=timeout)
+                for tel in guide_on_telescopes
+            ]
+        )
 
-        next_exposure_number_path = config["specs"]["nextExposureNumber"]
-        with open(next_exposure_number_path, "r") as fd:
-            data = fd.read().strip()
-            seqno = int(data) if data != "" else 1
+        has_timedout = any([gs[3] for gs in guide_status])
+        if has_timedout:
+            self.write_to_log("Some acquisitions timed out.", "warnings")
 
-        return seqno
+        try:
+            n_skies_guiding = 0
+            for ii, tel in enumerate(guide_on_telescopes):
+                is_guiding = guide_status[ii][0]
+                if tel == "sci" and not is_guiding:
+                    raise GortObserverError(
+                        "Science telescope is not guiding.",
+                        error_code=801,
+                    )
+                if tel == "spec" and not is_guiding:
+                    if require_spec:
+                        raise GortObserverError(
+                            "Spec telescope is not guiding.",
+                            error_code=801,
+                        )
+                    else:
+                        self.write_to_log("Spec telescope is not guiding", "warning")
+                if "sky" in tel:
+                    if is_guiding:
+                        n_skies_guiding += 1
+                    else:
+                        self.write_to_log(f"{tel} telescope is not guiding.", "warning")
+
+            if n_skies_guiding < min_skies:
+                raise GortObserverError(
+                    "Not enough sky telescopes guiding.",
+                    error_code=801,
+                )
 
-    async def are_idle(self):
-        """Returns `True` if all the spectrographs are idle and ready to expose."""
+        except Exception:
+            self.write_to_log("Stopping guide loops.", "warning")
+            await self.gort.guiders.stop()
+            raise
 
-        return all(await self.call_device_method(Spectrograph.is_idle))
+        self.write_to_log("All telescopes are now guiding.")
 
     async def expose(
         self,
-        exposure_time: float | None = None,
-        tile_data: dict | None = None,
-        show_progress: bool = False,
-        async_readout: bool = False,
-        **kwargs,
+        exposure_time: float = 900.0,
+        show_progress: bool | None = None,
+        iterate_over_standards: bool = True,
     ):
-        """Exposes the spectrographs.
+        """Starts exposing the spectrographs.
 
         Parameters
         ----------
         exposure_time
-            The exposure time.
-        tile_data
-            Tile data to add to the headers.
+            The lenght of the exposure in seconds.
         show_progress
             Displays a progress bar with the elapsed exposure time.
-        async_readout
-            Returns after integration completes. Readout is initiated
-            but handled asynchronously and can be await by awaiting
-            the returned `.Exposure` object.
-        kwargs
-            Keyword arguments to pass to ``lvmscp expose``.
-
-        Returns
-        -------
-        exp_nos
-            The numbers of the exposed frames.
+        iterate_over_standards
+            Whether to move the spec telescope during intergration
+            to observe various standard stars in different fibres.
 
         """
 
-        if self.last_exposure is not None and not self.last_exposure.done():
-            self.write_to_log("Waiting for previous exposure to read out.", "warning")
-            await self.last_exposure
-
-        if not (await self.are_idle()):
-            raise GortSpecError(
-                "Spectrographs are not idle. Cannot expose.",
-                error_code=302,
-            )
-
-        if "count" in kwargs:
-            raise GortSpecError(
-                "Count cannot be used here. Use a loop instead.",
-                error_code=3,
+        standard_task: asyncio.Task | None = None
+        if iterate_over_standards:
+            standard_task = asyncio.create_task(
+                self._iterate_over_mask_positions(exposure_time)
             )
 
-        if kwargs.get("bias", False) or kwargs.get("flavour", "object") == "bias":
-            exposure_time = 0.0
+        tile_id = self.tile.tile_id
+        dither_pos = self.tile.dither_position
 
-        seqno = self.get_seqno()
-        self.write_to_log(f"Taking spectrograph exposure {seqno}.", level="info")
+        exp_tile_data = {
+            "tile_id": (tile_id or -999, "The tile_id of this observation"),
+            "dpos": (dither_pos, "Dither position"),
+        }
 
-        await self.reset()
+        self.write_to_log(f"Starting {exposure_time:.1f} s exposure.", "info")
 
-        if tile_data is not None:
-            header = json.dumps(tile_data)
-        else:
-            header = None
-
-        exposure = Exposure(seqno, self)
-        await exposure.expose(
+        exposure = await self.gort.specs.expose(
             exposure_time=exposure_time,
-            header=header,
-            async_readout=async_readout,
+            tile_data=exp_tile_data,
             show_progress=show_progress,
-            **kwargs,
         )
 
+        if standard_task is not None and not standard_task.done():
+            standard_task.cancel()
+            with suppress(asyncio.CancelledError):
+                await standard_task
+
+        if tile_id is not None:
+            self.write_to_log("Registering observation.")
+            registration_payload = {
+                "dither": dither_pos,
+                "tile_id": tile_id,
+                "jd": 0,
+                "seeing": 10,
+                "standards": [],
+                "skies": [],
+                "exposure_no": exposure.exp_no,
+            }
+            self.write_to_log(f"Registration payload {registration_payload}")
+            await register_observation(registration_payload)
+            self.write_to_log("Registration complete.")
+
         return exposure
 
-    async def reset(self):
-        """Reset the spectrographs."""
+    async def finish_observation(self):
+        """Finishes the observation, stops the guiders, etc."""
+
+        self.write_to_log("Finishing observation.", "info")
 
-        await self._send_command_all("reset")
+        if self.guide_task is not None and not self.guide_task.done():
+            await self.gort.guiders.stop()
+            await self.guide_task
 
-    async def calibrate(
+    def write_to_log(
         self,
-        sequence: str = "normal",
-        park_after: bool = True,
-        show_progress: bool = False,
+        message: str,
+        level: str = "debug",
+        header: str | None = None,
     ):
-        """Runs the calibration sequence.
+        """Writes a message to the log with a custom header.
 
         Parameters
         ----------
-        sequence
-            The calibration sequence to execute.
-        park_after
-            Park the telescopes after a successful calibration sequence.
-        show_progress
-            Displays a progress bar with the elapsed exposure time.
+        message
+            The message to log.
+        level
+            The level to use for logging: ``'debug'``, ``'info'``, ``'warning'``, or
+            ``'error'``.
+        header
+            The header to prepend to the message. By default uses the class name.
 
         """
 
-        # TODO: add some checks. Confirm HDs are open, specs connected, etc.
+        if header is None:
+            header = f"({self.__class__.__name__}) "
 
-        cal_config = config["specs"]["calibration"]
+        message = f"{header}{message}"
 
-        if sequence not in cal_config["sequences"]:
-            raise GortSpecError(f"Unknown sequence {sequence!r}.", error_code=303)
-        sequence_config = cal_config["sequences"][sequence]
+        level = logging.getLevelName(level.upper())
+        assert isinstance(level, int)
 
-        self.write_to_log("Moving telescopes to position.", level="info")
-        await self.gort.telescopes.goto_named_position(cal_config["position"])
+        self.gort.log.log(level, message)
 
-        calib_nps = self.gort.nps[cal_config["lamps_nps"]]
-        lamps_config = sequence_config.get("lamps", {})
+    def _get_mask_positions(self, pattern: str):
+        """Returns mask positions sorted by motor steps."""
 
-        fibsel_task: asyncio.Task | None = None
+        mask_config = self.gort.config["telescopes"]["mask_positions"]
+        all_positions = self.gort.telescopes.spec.fibsel.list_positions()
+        positions = [pos for pos in all_positions if re.match(pattern, pos)]
 
-        # Turn off all lamps.
-        self.write_to_log("Checking that all lamps are off.", level="info")
-        await calib_nps.all_off()
+        return sorted(positions, key=lambda p: mask_config[p])
 
-        self.write_to_log(f"Running calibration sequence {sequence!r}.", level="info")
+    async def _iterate_over_mask_positions(self, exposure_time: float):
+        """Iterates over the fibre mask positions.
 
-        try:
-            if "biases" in sequence_config:
-                self.write_to_log("Taking biases.", level="info")
-                nbias = sequence_config["biases"].get("count", 1)
-                for _ in range(nbias):
-                    await self.gort.specs.expose(flavour="bias")
-
-            if "darks" in sequence_config:
-                self.write_to_log("Taking darks.", level="info")
-                ndarks = sequence_config["darks"].get("count")
-                for idark in range(ndarks):
-                    await self.gort.specs.expose(
-                        flavour="dark",
-                        exposure_time=sequence_config["darks"]["exposure_time"],
-                        async_readout=idark == ndarks - 1,
-                    )
+        Moving the ``spec`` telescope to each one of the standard star,
+        acquires the new field, and adjusts the time to stay on each target.
 
-            for lamp in lamps_config:
-                warmup = lamps_config[lamp]["warmup"]
+        """
 
-                self.write_to_log(f"Warming up lamp {lamp} ({warmup} s).", level="info")
-                await calib_nps.on(lamp)
-                await asyncio.sleep(warmup)
-
-                exp_times = lamps_config[lamp]["exposure_times"]
-                n_exp_times = len(exp_times)
-                for ietime, exp_time in enumerate(exp_times):
-                    flavour = lamps_config[lamp]["flavour"]
-
-                    # Check if we are spinning the fibre selector and,
-                    # if so, launch the task.
-                    fibsel = lamps_config[lamp].get("fibsel", None)
-                    if fibsel:
-                        initial_position = fibsel.get("initial_position", None)
-                        positions = fibsel.get("positions", "P1-*")
-                        time_per_position = fibsel.get("time_per_position", None)
-                        total_time = exp_time if time_per_position is None else None
-
-                        if initial_position:
-                            # Move to the initial position before starting the exposure.
-                            await self.gort.telescopes.spec.fibsel.move_to_position(
-                                initial_position
-                            )
-
-                        # Launch the task.
-                        fibsel_task = asyncio.create_task(
-                            move_mask_interval(
-                                self.gort,
-                                positions,
-                                order_by_steps=True,
-                                total_time=total_time,
-                                time_per_position=time_per_position,
-                            )
-                        )
+        # TODO: record how long we exposed on each standard and save that
+        # information somewhere.
 
-                    self.write_to_log(f"Exposing for {exp_time} s.", level="info")
-                    await self.gort.specs.expose(
-                        flavour=flavour,
-                        exposure_time=exp_time,
-                        show_progress=show_progress,
-                        async_readout=ietime == n_exp_times - 1,
-                    )
+        # Time to acquire a standard.
+        ACQ_PER_STD = 30
 
-                    if fibsel_task:
-                        await fibsel_task
+        spec_coords = self.tile.spec_coords
 
-                self.write_to_log(f"Turning off {lamp}.")
-                await calib_nps.off(lamp)
+        # If we have zero or one standards, do nothing. The spec telescope
+        # is already pointing to the first mask position.
+        if len(spec_coords) <= 1:
+            return
 
-            if park_after:
-                await self.gort.telescopes.park()
+        guider_pixels: dict[str, tuple[float, float]]
+        guider_pixels = self.gort.config["guiders"]["devices"]["spec"]["named_pixels"]
 
-            if self.last_exposure and not self.last_exposure.done():
-                self.write_to_log("Awaiting last exposure readout.")
-                await self.last_exposure
+        # Time at which the exposure began.
+        t0 = time()
 
-        except Exception:
+        # Time to spend on each mask position.
+        n_stds = len(spec_coords)
+
+        # Calculate the time to actually be on target, taking into account
+        # how long we expect to take acquiring.
+        time_per_position = exposure_time / n_stds - ACQ_PER_STD
+        if time_per_position < 0:
             self.write_to_log(
-                "Errored while executing sequence. "
-                "Turning all the lamps off before raising.",
-                level="error",
+                "Exposure time is too short to observe this "
+                "many standards. I will do what I can."
             )
+            time_per_position = exposure_time / n_stds
 
-            # Stop the mask iteration task.
-            if fibsel_task and not fibsel_task.done():
-                fibsel_task.cancel()
+        # Time at which we started observing the last standard.
+        t0_last_std = t0
 
-            raise
+        # Number of standards observed.
+        n_observed = 1
+
+        # Index of current standard being observed.
+        current_std_idx = 0
+
+        while True:
+            await asyncio.sleep(1)
+
+            # We consider than if there is less 2 * ACQ_PER_STD left in the
+            # exposure there is no point in going to the next standard.
+            t_now = time()
+            if t_now - t0 > exposure_time - 2 * ACQ_PER_STD:
+                self.write_to_log("Exiting standard loop.")
+                self.write_to_log(f"Standards observed: {n_observed}/{n_stds}.", "info")
+                return
+
+            # Time to move to another standard?
+            if t_now - t0_last_std > time_per_position:
+                # Check that we haven't run out standards. If so,
+                # keep observing this one.
+                if len(spec_coords) == current_std_idx + 1:
+                    continue
+
+                # Increase current index and get coordinates.
+                current_std_idx += 1
+
+                # New coordinates to observe.
+                new_coords = spec_coords[current_std_idx]
+                new_mask_position = self.mask_positions[current_std_idx]
+
+                # Pixel on the MF corresponding to the new fibre/mask hole on
+                # which to guide. We use this tabulated list instead of
+                # offset_to_master_frame_pixel() because the latter coordinates
+                # are less precise as they do not include IFU rotation and more
+                # precise metrology.
+                new_guider_pixel = guider_pixels[new_mask_position]
+
+                self.write_to_log(
+                    f"Moving to standard #{current_std_idx+1} ({new_coords}) "
+                    f"on fibre {new_mask_position}.",
+                    "info",
+                )
+
+                # Finish guiding on spec telescope.
+                self.write_to_log("Stopping guiding on spec telescope.")
+                await self.gort.guiders["spec"].stop()
+
+                # TODO: some of these things can be concurrent.
+                spec_tel = self.gort.telescopes.spec
+
+                # Moving the mask to an intermediate position while we move around.
+                await spec_tel.fibsel.move_relative(500)
+
+                # Slew to new coordinates. We actually slew to the coordinates
+                # that make the new star close to the fibre that will observe it.
+                # slew_ra, slew_dec = fibre_slew_coordinates(
+                #     new_coords.ra,
+                #     new_coords.dec,
+                #     new_mask_position,
+                # )
+                # await spec_tel.goto_coordinates(ra=slew_ra, dec=slew_dec)
+
+                await spec_tel.goto_coordinates(ra=new_coords.ra, dec=new_coords.dec)
+
+                # Start to guide. Note that here we use the original coordinates
+                # of the star along with the pixel on the master frame on which to
+                # guide. See the note in fibre_slew_coordinates().
+                self.write_to_log("Starting to guide on spec telescope.")
+                asyncio.create_task(
+                    self.gort.guiders.spec.guide(
+                        ra=new_coords.ra,
+                        dec=new_coords.dec,
+                        guide_tolerance=5,
+                        pixel=new_guider_pixel,
+                    )
+                )
+
+                result = await self.gort.guiders.spec.wait_until_guiding(timeout=60)
+                if result[0] is False:
+                    self.write_to_log(
+                        "Failed to acquire standard position. Skipping.",
+                        "warning",
+                    )
+                    continue
+
+                self.write_to_log(f"Standard position {new_mask_position} acquired.")
+
+                # Move mask to uncover fibre.
+                await spec_tel.fibsel.move_to_position(new_mask_position)
 
-        finally:
-            await calib_nps.all_off()
+                n_observed += 1
+                t0_last_std = time()
```

### Comparing `lvmgort-0.1.1/src/gort/devices/telescope.py` & `lvmgort-0.2.0/src/gort/devices/telescope.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,63 +6,86 @@
 # @Filename: telescope.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import asyncio
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, ClassVar
 
 import numpy
 
 from gort import config
 from gort.exceptions import GortTelescopeError
 from gort.gort import GortDevice, GortDeviceSet
 from gort.tools import angular_separation
 
 
 if TYPE_CHECKING:
     from gort.core import ActorReply
     from gort.gort import GortClient
 
 
-__all__ = ["Telescope", "TelescopeSet", "KMirror", "FibSel", "Focuser"]
+__all__ = ["Telescope", "TelescopeSet", "KMirror", "FibSel", "Focuser", "MoTanDevice"]
 
 
-class KMirror(GortDevice):
+class MoTanDevice(GortDevice):
+    """A TwiceAsNice device."""
+
+    #: Artificial delay introduced to prevent all motors to slew at the same time.
+    SLEW_DELAY: ClassVar[float | dict[str, float]] = 0
+
+    async def slew_delay(self):
+        """Sleeps the :obj:`.SLEW_DELAY` amount."""
+
+        if isinstance(self.SLEW_DELAY, (float, int)):
+            await asyncio.sleep(self.SLEW_DELAY)
+        else:
+            await asyncio.sleep(self.SLEW_DELAY[self.name.split(".")[0]])
+
+
+class KMirror(MoTanDevice):
     """A device representing a K-mirror."""
 
+    SLEW_DELAY = {"sci": 1, "skye": 2, "skyw": 3}
+
     async def status(self):
         """Returns the status of the k-mirror."""
 
         return await self.actor.commands.status()
 
     async def home(self):
         """Homes the k-mirror."""
 
+        await self.slew_delay()
+
         self.write_to_log("Homing k-mirror.", level="info")
         await self.actor.commands.moveToHome()
         self.write_to_log("k-mirror homing complete.")
 
     async def park(self):
         """Park the k-mirror at 90 degrees."""
 
+        await self.slew_delay()
+
         await self.actor.commands.slewStop()
         await self.move(90)
 
     async def move(self, degs: float):
         """Move the k-mirror to a position in degrees. Does NOT track after the move.
 
         Parameters
         ----------
         degs
             The position to which to move the k-mirror, in degrees.
 
         """
 
+        await self.slew_delay()
+
         self.write_to_log(f"Moving k-mirror to {degs:.3f} degrees.", level="info")
 
         self.write_to_log("Stopping slew.")
         await self.actor.commands.slewStop()
 
         self.write_to_log("Moving k-mirror to absolute position.")
         await self.actor.commands.moveAbsolute(degs, "deg")
@@ -75,55 +98,69 @@
         ra
             Right ascension of the field to track, in degrees.
         dec
             Declination of the field to track, in degrees.
 
         """
 
+        await self.slew_delay()
+
         self.write_to_log(
             f"Slewing k-mirror to ra={ra:.6f} dec={dec:.6f} and tracking.",
             level="info",
         )
 
         await self.actor.commands.slewStart(ra / 15.0, dec)
 
 
-class Focuser(GortDevice):
+class Focuser(MoTanDevice):
     """A device representing a focuser."""
 
+    SLEW_DELAY = {"spec": 0, "sci": 1, "skye": 2, "skyw": 3}
+
     async def status(self):
         """Returns the status of the focuser."""
 
         return await self.actor.commands.status()
 
     async def home(self):
         """Homes the focuser."""
 
+        await self.slew_delay()
+
         self.write_to_log("Homing focuser.", level="info")
         await self.actor.commands.moveToHome()
         self.write_to_log("Focuser homing complete.")
 
     async def move(self, dts: float):
         """Move the focuser to a position in DT."""
 
+        await self.slew_delay()
+
         self.write_to_log(f"Moving focuser to {dts:.3f} DT.", level="info")
         await self.actor.commands.moveAbsolute(dts, "DT")
 
 
-class FibSel(GortDevice):
+class FibSel(MoTanDevice):
     """A device representing the fibre mask in the spectrophotometric telescope."""
 
+    # We really don't want a delay here because it would slow down the acquisition
+    # of new standards, and anyway the fibre selector usually moves by itself.
+    SLEW_DELAY = 0
+
     async def status(self):
         """Returns the status of the fibre selector."""
 
         return await self.actor.commands.status()
 
     async def home(self):
         """Homes the fibre selector."""
 
+        await self.slew_delay()
+
         self.write_to_log("Homing fibsel.", level="info")
         await self.actor.commands.moveToHome()
         self.write_to_log("Fibsel homing complete.")
 
     def list_positions(self) -> list[str]:
         """Returns a list of valid positions."""
 
@@ -152,20 +189,23 @@
             steps = mask_positions[position]
             self.write_to_log(f"Moving mask to {position}: {steps} DT.", level="info")
 
         else:
             steps = position
             self.write_to_log(f"Moving mask to {steps} DT.", level="info")
 
+        await self.slew_delay()
         await self.actor.commands.moveAbsolute(steps)
 
     async def move_relative(self, steps: float):
         """Move the mask a number of motor steps relative to the current position."""
 
         self.write_to_log(f"Moving fibre mask {steps} steps.")
+
+        await self.slew_delay()
         await self.actor.commands.moveRelative(steps)
 
 
 class Telescope(GortDevice):
     """Class representing an LVM telescope functionality."""
 
     def __init__(self, gort: GortClient, name: str, actor: str, **kwargs):
```

### Comparing `lvmgort-0.1.1/src/gort/etc/lvmgort.yml` & `lvmgort-0.2.0/src/gort/etc/lvmgort.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
----
 telescopes:
   devices:
     sci:
       actor: lvm.sci.pwi
       kmirror: lvm.sci.km
       focuser: lvm.sci.foc
     spec:
@@ -171,15 +170,15 @@
             flavour: flat
           Quartz:
             warmup: 120
             exposure_times: [270]
             flavour: flat
             fibsel:
               initial_position: P1-2
-              positions: P1-*
+              positions: P1-
               time_per_position: 20
           Argon:
             warmup: 120
             exposure_times: [30]
             flavour: arc
           Neon:
             warmup: 120
@@ -202,15 +201,15 @@
         lamps:
           Quartz:
             warmup: 20
             exposure_times: [120]
             flavour: flat
             fibsel:
               initial_position: P1-2
-              positions: P1-*
+              positions: P1-
               time_per_position: 10
         biases:
           count: 1
 
 ags:
   devices:
     sci:
```

### Comparing `lvmgort-0.1.1/src/gort/exceptions.py` & `lvmgort-0.2.0/src/gort/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,19 @@
 
         super(GortNotImplemented, self).__init__(message, error_code=1)
 
 
 class GortDeviceError(GortError):
     """A device error, which appends the name of the device to the error message."""
 
-    def __init__(self, message: str | None = None, error_code: int = 0) -> None:
+    def __init__(
+        self,
+        message: str | None = None,
+        error_code: int | ErrorCodes = 0,
+    ) -> None:
         from gort.gort import GortDevice
 
         if message is not None:
             stack = inspect.stack()
             f_locals = stack[1][0].f_locals
 
             if "self" in f_locals:
```

### Comparing `lvmgort-0.1.1/src/gort/gort.py` & `lvmgort-0.2.0/src/gort/gort.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from gort import config, log
 from gort.core import RemoteActor
 from gort.exceptions import GortError
 from gort.kubernetes import Kubernetes
 from gort.observer import GortObserver
 from gort.tile import Tile
-from gort.tools import run_in_executor
+from gort.tools import CustomRichHandler, get_rich_hadler, run_in_executor
 
 
 __all__ = ["GortClient", "Gort", "GortDeviceSet", "GortDevice"]
 
 
 DevType = TypeVar("DevType", bound="GortDeviceSet | GortDevice")
 
@@ -149,24 +149,41 @@
         verbosity
             The level of verbosity. Can be a string level name, an integer, or `None`,
             in which case the default verbosity will be used.
 
         """
 
         verbosity = verbosity or "warning"
-
         if isinstance(verbosity, int):
-            self.log.sh.setLevel(verbosity)
-            return
+            verbosity = logging.getLevelName(verbosity)
+
+        assert isinstance(verbosity, str)
 
         verbosity = verbosity.lower()
         if verbosity not in ["debug", "info", "warning"]:
             raise ValueError("Invalid verbosity value.")
 
-        self.log.sh.setLevel(logging.getLevelName(verbosity.upper()))
+        verbosity_level = logging.getLevelName(verbosity.upper())
+
+        # Disable the normal console logger.
+        self.log.sh.setLevel(10000)
+
+        # Check if we have added a rich logger. If so, change the level.
+        has_rich_handler = False
+        for handler in self.log.handlers:
+            if isinstance(handler, CustomRichHandler):
+                handler.setLevel(verbosity_level)
+                has_rich_handler = True
+
+        # If not, add a RichHandler.
+        if not has_rich_handler:
+            handler = get_rich_hadler(verbosity_level)
+            self.log.addHandler(handler)
+            if self.log.warnings_logger:
+                self.log.warnings_logger.addHandler(handler)
 
 
 GortDeviceType = TypeVar("GortDeviceType", bound="GortDevice")
 
 
 class GortDeviceSet(dict[str, GortDeviceType], Generic[GortDeviceType]):
     """A set to gort-managed devices.
@@ -440,30 +457,52 @@
 
     async def observe_tile(
         self,
         tile: Tile | int | None = None,
         ra: float | None = None,
         dec: float | None = None,
         use_scheduler: bool = False,
+        exposure_time: float = 900.0,
+        guide_tolerance: float = 3.0,
+        acquisition_timeout: float = 180.0,
+        show_progress: bool | None = None,
+        min_skies: int = 1,
+        require_spec: bool = False,
     ):
         """Performs all the operations necessary to observe a tile.
 
         Parameters
         ----------
         tile
             The ``tile_id`` to observe, or a `.Tile` object. If not provided,
             observes the next tile suggested by the scheduler (requires
             ``use_scheduler=True``).
         ra,dec
             The RA and Dec where to point the science telescopes. The other
             telescopes are pointed to calibrators that fit the science pointing.
-            Cannot be used with ``tile_id``.
+            Cannot be used with ``tile``.
         use_scheduler
             Whether to use the scheduler to determine the ``tile_id`` or
             select calibrators.
+        exposure_time
+            The length of the exposure in seconds.
+        guide_tolerance
+            The guide tolerance in arcsec. A telescope will not be considered
+            to be guiding if its separation to the commanded field is larger
+            than this value.
+        acquisition_timeout
+            The maximum time allowed for acquisition. In case of timeout
+            the acquired fields are evaluated and an exception is
+            raised if the acquisition failed.
+        show_progress
+            Displays a progress bar with the elapsed exposure time.
+        min_skies
+            Minimum number of skies required to consider acquisition successful.
+        require_spec
+            Whether to require the ``spec`` telescope to be guiding.
 
         """
 
         # Create tile.
         if isinstance(tile, Tile):
             pass
         elif tile is not None or (tile is None and ra is None and dec is None):
@@ -487,17 +526,25 @@
         observer = GortObserver(self, tile)
 
         try:
             # Slew telescopes and move fibsel mask.
             await observer.slew()
 
             # Start guiding.
-            await observer.acquire()
+            await observer.acquire(
+                min_skies=min_skies,
+                require_spec=require_spec,
+                guide_tolerance=guide_tolerance,
+                timeout=acquisition_timeout,
+            )
 
             # Exposing
-            exposure = await observer.expose()
+            exposure = await observer.expose(
+                exposure_time=exposure_time,
+                show_progress=show_progress,
+            )
 
         finally:
             # Finish observation.
             await observer.finish_observation()
 
         return exposure
```

### Comparing `lvmgort-0.1.1/src/gort/kubernetes.py` & `lvmgort-0.2.0/src/gort/kubernetes.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.1/src/gort/maskbits.py` & `lvmgort-0.2.0/src/gort/maskbits.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.1/src/gort/tile.py` & `lvmgort-0.2.0/src/gort/tile.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.1/src/gort/tools.py` & `lvmgort-0.2.0/src/gort/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 from typing import TYPE_CHECKING, Callable, Coroutine
 
 import httpx
 import peewee
 from astropy import units as uu
 from astropy.coordinates import angular_separation as astropy_angular_separation
+from rich.console import Console
+from rich.logging import RichHandler
+from rich.text import Text
+from rich.theme import Theme
 
 from gort import config
 
 
 if TYPE_CHECKING:
     from pyds9 import DS9
 
@@ -46,14 +50,16 @@
     "register_observation",
     "tqdm_timer",
     "get_ccd_frame_path",
     "move_mask_interval",
     "angular_separation",
     "get_db_connection",
     "run_in_executor",
+    "is_interactive",
+    "is_notebook",
 ]
 
 CAMERAS = [
     "sci.west",
     "sci.east",
     "skye.west",
     "skye.east",
@@ -309,14 +315,22 @@
             return False  # Terminal running IPython
         else:
             return False  # Other type (?)
     except NameError:
         return False  # Probably standard Python interpreter
 
 
+def is_interactive():
+    """Returns `True` is we are in an interactive session."""
+
+    import __main__ as main
+
+    return not hasattr(main, "__file__")
+
+
 def tqdm_timer(seconds: float):
     """Creates a task qith a tqdm progress bar."""
 
     if is_notebook():
         from tqdm.notebook import tqdm
     else:
         from tqdm import tqdm
@@ -526,7 +540,41 @@
             warnings.warn(ww.message, ww.category)
 
     else:
         with executor() as pool:
             result = await asyncio.get_running_loop().run_in_executor(pool, fn)
 
     return result
+
+
+class CustomRichHandler(RichHandler):
+    """A slightly custom ``RichHandler`` logging handler."""
+
+    def get_level_text(self, record):
+        """Get the level name from the record."""
+
+        level_name = record.levelname
+        level_text = Text.styled(
+            f"[{level_name}]:",
+            f"logging.level.{level_name.lower()}",
+        )
+        return level_text
+
+
+def get_rich_hadler(verbosity_level):
+    """Returns a custom rich handler."""
+
+    return CustomRichHandler(
+        level=verbosity_level,
+        log_time_format="%X",
+        show_path=False,
+        console=Console(
+            theme=Theme(
+                {
+                    "logging.level.debug": "magenta",
+                    "logging.level.warning": "yellow",
+                    "logging.level.critical": "red",
+                    "logging.level.error": "red",
+                }
+            )
+        ),
+    )
```

### Comparing `lvmgort-0.1.1/src/gort/transforms.py` & `lvmgort-0.2.0/src/gort/transforms.py`

 * *Files identical despite different names*

### Comparing `lvmgort-0.1.1/src/gort/websocket.py` & `lvmgort-0.2.0/src/gort/websocket.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,23 +11,21 @@
 import asyncio
 import json
 from functools import partial
 
 from typing import TYPE_CHECKING, Callable, Coroutine
 
 from websockets.legacy.protocol import broadcast
-from websockets.server import serve
+from websockets.server import WebSocketServerProtocol, serve
 
 from gort import config, log
 from gort.gort import Gort
 
 
 if TYPE_CHECKING:
-    from websockets.server import WebSocketServerProtocol
-
     from clu import AMQPReply
 
 
 __all__ = ["WebsocketServer"]
 
 
 CALLBACKS: dict[str, Callable] = {}
@@ -170,18 +168,39 @@
         final_message.update(message_kwargs)
 
         try:
             await client.send(json.dumps(final_message))
         except Exception as err:
             log.warning(f"Failed replying to WS client: {err}.")
 
-    @route("get_enclosure_status")
+    @route("enclosure_status")
     async def enclosure_status(
         self,
         client: WebSocketServerProtocol,
         command_id: str,
         **_,
     ):
         """Returns the enclosure status."""
 
         status = await self.gort.enclosure.status()
         await self.reply_to_client(client, command_id, status)
+
+    @route("enclosure_action")
+    async def enclosure_action(
+        self,
+        client: WebSocketServerProtocol,
+        command_id: str,
+        action: str | None = None,
+    ):
+        """Opens/closes/stops the enclosure."""
+
+        if action == "open":
+            await self.gort.enclosure.open()
+            await self.reply_to_client(client, command_id, {"text": "Dome open"})
+        elif action == "close":
+            await self.gort.enclosure.close()
+            await self.reply_to_client(client, command_id, {"text": "Dome closed"})
+        elif action == "stop":
+            await self.gort.enclosure.stop()
+            await self.reply_to_client(client, command_id, {"text": "Dome stopped"})
+        else:
+            await self.reply_to_client(client, command_id, {"error": "Invalid action"})
```

### Comparing `lvmgort-0.1.1/PKG-INFO` & `lvmgort-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lvmgort
-Version: 0.1.1
+Version: 0.2.0
 Summary: The brains of LVM observing
 Home-page: https://github.com/sdss/lvmgort
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<4.0
@@ -19,23 +19,26 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: astropy (>=5.3.1,<6.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: jsonschema (>=4.18.3,<5.0.0)
 Requires-Dist: kubernetes (>=26.1.0,<27.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: peewee (>=3.16.2,<4.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: sdss-clu (>=2.0.1,<3.0.0)
 Requires-Dist: sdsstools (>=1.1.0,<2.0.0)
 Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Requires-Dist: unclick (>=0.1.0b5)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Project-URL: Documentation, https://lvmgort.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/lvmgort
 Description-Content-Type: text/markdown
 
 # GORT
```

