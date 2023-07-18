# Comparing `tmp/SpiNNMachine-2016.001.zip` & `tmp/SpiNNMachine-3.0.0.zip`

## zipinfo {}

```diff
@@ -1,29 +1,33 @@
-Zip file size: 23923 bytes, number of entries: 27
--rw-rw-rw-  2.0 fat      277 b- defN 16-Apr-28 13:46 SpiNNMachine-2016.001/PKG-INFO
--rw-rw-rw-  2.0 fat     1115 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/README
--rw-rw-rw-  2.0 fat       64 b- defN 16-Apr-28 13:46 SpiNNMachine-2016.001/setup.cfg
--rw-rw-rw-  2.0 fat      409 b- defN 16-Apr-19 15:31 SpiNNMachine-2016.001/setup.py
--rw-rw-rw-  2.0 fat        1 b- defN 16-Apr-28 13:46 SpiNNMachine-2016.001/SpiNNMachine.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat      277 b- defN 16-Apr-28 13:46 SpiNNMachine-2016.001/SpiNNMachine.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      749 b- defN 16-Apr-28 13:46 SpiNNMachine-2016.001/SpiNNMachine.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat       14 b- defN 16-Apr-28 13:46 SpiNNMachine-2016.001/SpiNNMachine.egg-info/top_level.txt
--rw-rw-rw-  2.0 fat     7854 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/chip.py
--rw-rw-rw-  2.0 fat     2127 b- defN 14-Aug-10 19:39 SpiNNMachine-2016.001/spinn_machine/exceptions.py
--rw-rw-rw-  2.0 fat     5959 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/link.py
--rw-rw-rw-  2.0 fat     9957 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/machine.py
--rw-rw-rw-  2.0 fat     6415 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/multicast_routing_entry.py
--rw-rw-rw-  2.0 fat     3310 b- defN 16-Apr-19 10:50 SpiNNMachine-2016.001/spinn_machine/processor.py
--rw-rw-rw-  2.0 fat     6191 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/router.py
--rw-rw-rw-  2.0 fat     2200 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/sdram.py
--rw-rw-rw-  2.0 fat     1064 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/spinnaker_link_data.py
--rw-rw-rw-  2.0 fat    21055 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/virtual_machine.py
--rw-rw-rw-  2.0 fat     2620 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/__init__.py
--rw-rw-rw-  2.0 fat      514 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/tags/abstract_tag.py
--rw-rw-rw-  2.0 fat     2139 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/tags/iptag.py
--rw-rw-rw-  2.0 fat     2284 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/tags/reverse_iptag.py
--rw-rw-rw-  2.0 fat        0 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/tags/__init__.py
--rw-rw-rw-  2.0 fat     2984 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/utilities/ordered_set.py
--rw-rw-rw-  2.0 fat     2553 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/utilities/progress_bar.py
--rw-rw-rw-  2.0 fat     3202 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/utilities/utilities.py
--rw-rw-rw-  2.0 fat        0 b- defN 16-Apr-01 15:10 SpiNNMachine-2016.001/spinn_machine/utilities/__init__.py
-27 files, 85334 bytes uncompressed, 19177 bytes compressed:  77.5%
+Zip file size: 28539 bytes, number of entries: 31
+-rw-rw-rw-  2.0 fat      274 b- defN 16-Sep-02 09:06 SpiNNMachine-3.0.0/PKG-INFO
+-rw-rw-rw-  2.0 fat     1115 b- defN 16-Apr-01 15:10 SpiNNMachine-3.0.0/README
+-rw-rw-rw-  2.0 fat       64 b- defN 16-Sep-02 09:06 SpiNNMachine-3.0.0/setup.cfg
+-rw-rw-rw-  2.0 fat      455 b- defN 16-Sep-02 09:05 SpiNNMachine-3.0.0/setup.py
+-rw-rw-rw-  2.0 fat        1 b- defN 16-Sep-02 09:06 SpiNNMachine-3.0.0/SpiNNMachine.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat      274 b- defN 16-Sep-02 09:06 SpiNNMachine-3.0.0/SpiNNMachine.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      937 b- defN 16-Sep-02 09:06 SpiNNMachine-3.0.0/SpiNNMachine.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat       14 b- defN 16-Sep-02 09:06 SpiNNMachine-3.0.0/SpiNNMachine.egg-info/top_level.txt
+-rw-rw-rw-  2.0 fat     8001 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/chip.py
+-rw-rw-rw-  2.0 fat     2310 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/core_subset.py
+-rw-rw-rw-  2.0 fat     3959 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/core_subsets.py
+-rw-rw-rw-  2.0 fat     2127 b- defN 14-Aug-10 19:39 SpiNNMachine-3.0.0/spinn_machine/exceptions.py
+-rw-rw-rw-  2.0 fat     5996 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/link.py
+-rw-rw-rw-  2.0 fat    21422 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/machine.py
+-rw-rw-rw-  2.0 fat     6824 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/multicast_routing_entry.py
+-rw-rw-rw-  2.0 fat     3405 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/processor.py
+-rw-rw-rw-  2.0 fat     6253 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/router.py
+-rw-rw-rw-  2.0 fat      685 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/sdram.py
+-rw-rw-rw-  2.0 fat    30585 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/virtual_machine.py
+-rw-rw-rw-  2.0 fat     2620 b- defN 16-Apr-01 15:10 SpiNNMachine-3.0.0/spinn_machine/__init__.py
+-rw-rw-rw-  2.0 fat     1256 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/link_data_objects/abstract_link_data.py
+-rw-rw-rw-  2.0 fat      714 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/link_data_objects/fpga_link_data.py
+-rw-rw-rw-  2.0 fat      683 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/link_data_objects/spinnaker_link_data.py
+-rw-rw-rw-  2.0 fat        0 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/link_data_objects/__init__.py
+-rw-rw-rw-  2.0 fat      514 b- defN 16-Apr-01 15:10 SpiNNMachine-3.0.0/spinn_machine/tags/abstract_tag.py
+-rw-rw-rw-  2.0 fat     2204 b- defN 16-Jul-11 11:48 SpiNNMachine-3.0.0/spinn_machine/tags/iptag.py
+-rw-rw-rw-  2.0 fat     2284 b- defN 16-Apr-01 15:10 SpiNNMachine-3.0.0/spinn_machine/tags/reverse_iptag.py
+-rw-rw-rw-  2.0 fat        0 b- defN 16-Apr-01 15:10 SpiNNMachine-3.0.0/spinn_machine/tags/__init__.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/utilities/ordered_set.py
+-rw-rw-rw-  2.0 fat     2692 b- defN 16-Sep-01 16:05 SpiNNMachine-3.0.0/spinn_machine/utilities/progress_bar.py
+-rw-rw-rw-  2.0 fat        0 b- defN 16-Apr-01 15:10 SpiNNMachine-3.0.0/spinn_machine/utilities/__init__.py
+31 files, 110767 bytes uncompressed, 23131 bytes compressed:  79.1%
```

## zipnote {}

```diff
@@ -1,82 +1,94 @@
-Filename: SpiNNMachine-2016.001/PKG-INFO
+Filename: SpiNNMachine-3.0.0/PKG-INFO
 Comment: 
 
-Filename: SpiNNMachine-2016.001/README
+Filename: SpiNNMachine-3.0.0/README
 Comment: 
 
-Filename: SpiNNMachine-2016.001/setup.cfg
+Filename: SpiNNMachine-3.0.0/setup.cfg
 Comment: 
 
-Filename: SpiNNMachine-2016.001/setup.py
+Filename: SpiNNMachine-3.0.0/setup.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/SpiNNMachine.egg-info/dependency_links.txt
+Filename: SpiNNMachine-3.0.0/SpiNNMachine.egg-info/dependency_links.txt
 Comment: 
 
-Filename: SpiNNMachine-2016.001/SpiNNMachine.egg-info/PKG-INFO
+Filename: SpiNNMachine-3.0.0/SpiNNMachine.egg-info/PKG-INFO
 Comment: 
 
-Filename: SpiNNMachine-2016.001/SpiNNMachine.egg-info/SOURCES.txt
+Filename: SpiNNMachine-3.0.0/SpiNNMachine.egg-info/SOURCES.txt
 Comment: 
 
-Filename: SpiNNMachine-2016.001/SpiNNMachine.egg-info/top_level.txt
+Filename: SpiNNMachine-3.0.0/SpiNNMachine.egg-info/top_level.txt
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/chip.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/chip.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/exceptions.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/core_subset.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/link.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/core_subsets.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/machine.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/exceptions.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/multicast_routing_entry.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/link.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/processor.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/machine.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/router.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/multicast_routing_entry.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/sdram.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/processor.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/spinnaker_link_data.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/router.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/virtual_machine.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/sdram.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/__init__.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/virtual_machine.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/tags/abstract_tag.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/__init__.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/tags/iptag.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/link_data_objects/abstract_link_data.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/tags/reverse_iptag.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/link_data_objects/fpga_link_data.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/tags/__init__.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/link_data_objects/spinnaker_link_data.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/utilities/ordered_set.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/link_data_objects/__init__.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/utilities/progress_bar.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/tags/abstract_tag.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/utilities/utilities.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/tags/iptag.py
 Comment: 
 
-Filename: SpiNNMachine-2016.001/spinn_machine/utilities/__init__.py
+Filename: SpiNNMachine-3.0.0/spinn_machine/tags/reverse_iptag.py
+Comment: 
+
+Filename: SpiNNMachine-3.0.0/spinn_machine/tags/__init__.py
+Comment: 
+
+Filename: SpiNNMachine-3.0.0/spinn_machine/utilities/ordered_set.py
+Comment: 
+
+Filename: SpiNNMachine-3.0.0/spinn_machine/utilities/progress_bar.py
+Comment: 
+
+Filename: SpiNNMachine-3.0.0/spinn_machine/utilities/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `SpiNNMachine-2016.001/README` & `SpiNNMachine-3.0.0/README`

 * *Files identical despite different names*

## Comparing `SpiNNMachine-2016.001/spinn_machine/chip.py` & `SpiNNMachine-3.0.0/spinn_machine/chip.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,45 @@
 
             * processor_id is the id of a processor
             * processor is the processor with processor_id
     """
 
     IPTAG_IDS = set(range(0, 8))
 
+    __slots__ = (
+        "_x", "_y", "_p", "_router", "_sdram", "_ip_address", "_virtual",
+        "_tag_ids", "_nearest_ethernet_x", "_nearest_ethernet_y"
+    )
+
     def __init__(self, x, y, processors, router, sdram, nearest_ethernet_x,
                  nearest_ethernet_y, ip_address=None, virtual=False,
                  tag_ids=IPTAG_IDS):
         """
 
         :param x: the x-coordinate of the chip's position in the\
-                    two-dimentional grid of chips
+                    two-dimensional grid of chips
         :type x: int
         :param y: the y-coordinate of the chip's position in the\
-                    two-dimentional grid of chips
+                    two-dimensional grid of chips
         :type y: int
         :param processors: an iterable of processor objects
         :type processors: iterable of\
                     :py:class:`spinn_machine.processor.Processor`
         :param router: a router for the chip
         :type router: :py:class:`spinn_machine.router.Router`
         :param sdram: an SDRAM for the chip
         :type sdram: :py:class:`spinn_machine.sdram.SDRAM`
-        :param nearest_ethernet_x: the nearest ethernet x coord
+        :param nearest_ethernet_x: the nearest Ethernet x coord
         :type nearest_ethernet_x: int or None
-        :param nearest_ethernet_y: the nearest ethernet y coord
+        :param nearest_ethernet_y: the nearest Ethernet y coord
         :type nearest_ethernet_y: int or None
-        :param ip_address: the IP address of the chip or None if no ethernet\
+        :param ip_address: the IP address of the chip or None if no Ethernet\
                     attached
         :type ip_address: str
-        :param virtual: boolean which defines if this chip isa  virutal one or\
-         not
+        :param virtual: boolean which defines if this chip is a virtual one
          :type virtual: bool
 
         :raise spinn_machine.exceptions.SpinnMachineAlreadyExistsException: If\
                     processors contains any two processors with the same\
                     processor_id
         """
         self._x = x
@@ -133,15 +137,15 @@
         """
         return self._p.itervalues()
 
     @property
     def virtual(self):
         """ boolean which defines if the chip is virtual or not
 
-        :return: if the chip is virutal
+        :return: if the chip is virtual
         :rtype: boolean
         :raise None: this method does not raise any known exceptions
         """
         return self._virtual
 
     def __iter__(self):
         """ Get an iterable of processor identifiers and processors
@@ -174,36 +178,36 @@
         """
         return self._sdram
 
     @property
     def ip_address(self):
         """ The IP address of the chip
 
-        :return: IP address of the chip, or None if there is no ethernet\
+        :return: IP address of the chip, or None if there is no Ethernet\
                     connected to the chip
         :rtype: str
         :raise None: does not raise any known exceptions
         """
         return self._ip_address
 
     @property
     def nearest_ethernet_x(self):
-        """ the x coord of the nearest ethernet chip
+        """ the x coord of the nearest Ethernet chip
 
-        :return: the x coord of the nearest ethernet chip
+        :return: the x coord of the nearest Ethernet chip
         :rtype: int
         :raise None: does not raise any known exceptions
         """
         return self._nearest_ethernet_x
 
     @property
     def nearest_ethernet_y(self):
-        """ the y coord of the nearest ethernet chip
+        """ the y coord of the nearest Ethernet chip
 
-        :return: the y coord of the nearest ethernet chip
+        :return: the y coord of the nearest Ethernet chip
         :rtype: int
         :raise None: does not raise any known exceptions
         """
         return self._nearest_ethernet_y
 
     @property
     def tag_ids(self):
```

## Comparing `SpiNNMachine-2016.001/spinn_machine/exceptions.py` & `SpiNNMachine-3.0.0/spinn_machine/exceptions.py`

 * *Files identical despite different names*

## Comparing `SpiNNMachine-2016.001/spinn_machine/link.py` & `SpiNNMachine-3.0.0/spinn_machine/link.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,24 @@
 """
 from spinn_machine.exceptions import SpinnMachineAlreadyExistsException
 
 
 class Link(object):
     """ Represents a directional link between chips in the machine
     """
-    
+
+    __slots__ = (
+        "_destination_x", "_destination_y", "_multicast_default_from",
+        "_multicast_default_to", "_source_link_id", "_source_x", "_source_y"
+    )
+
     def __init__(self, source_x, source_y, source_link_id, destination_x,
                  destination_y, multicast_default_from, multicast_default_to):
         """
-        
+
         :param source_x: The x-coordinate of the source chip of the link
         :type source_x: int
         :param source_y: The y-coordinate of the source chip of the link
         :type source_y: int
         :param source_link_id: The id of the link in the source chip
         :type source_link_id: int
         :param destination_x: The x-coordinate of the destination chip of the\
@@ -44,112 +49,112 @@
         self._source_x = source_x
         self._source_y = source_y
         self._source_link_id = source_link_id
         self._destination_x = destination_x
         self._destination_y = destination_y
         self._multicast_default_from = multicast_default_from
         self._multicast_default_to = multicast_default_to
-    
+
     @property
     def source_x(self):
         """ The x-coordinate of the source chip of this link
-        
+
         :return: The x-coordinate
         :rtype: int
         """
         return self._source_x
-    
+
     @property
     def source_y(self):
         """ The y-coordinate of the source chip of this link
-        
+
         :return: The y-coordinate
         :rtype: int
         """
         return self._source_y
-    
+
     @property
     def source_link_id(self):
         """ The id of the link on the source chip
-        
+
         :return: The link id
         :rtype: int
         """
         return self._source_link_id
-    
+
     @property
     def destination_x(self):
         """ The x-coordinate of the destination chip of this link
-        
+
         :return: The x-coordinate
         :rtype: int
         """
         return self._destination_x
-    
+
     @property
     def destination_y(self):
         """ The y-coordinate of the destination chip of this link
-        
+
         :return: The y-coordinate
         :rtype: int
         """
         return self._destination_y
-    
+
     @property
     def multicast_default_from(self):
         """ The id of the link for which this link is the default
-        
+
         :return: The id of a link, or None if no such link
         :rtype: int
         """
         return self._multicast_default_from
-    
+
     @multicast_default_from.setter
     def multicast_default_from(self, multicast_default_from):
         """ Sets the id of the link for which this link is the default,\
             if not already set
-            
+
         :param multicast_default_from: The id of a link
         :type multicast_default_from: int
         :raise spinn_machine.exceptions.SpinnMachineAlreadyExistsException: If\
                     a value has already been set
         """
         if self._multicast_default_from is not None:
             raise SpinnMachineAlreadyExistsException(
                 "multicast_default_from", str(self._multicast_default_from))
         self._multicast_default_from = multicast_default_from
-    
+
     @property
     def multicast_default_to(self):
         """ The id of the link to which to send default routed multicast
-        
+
         :return: The id of a link, or None if no such link
         :rtype: int
         """
         return self._multicast_default_to
-    
+
     @multicast_default_to.setter
     def multicast_default_to(self, multicast_default_to):
         """ Sets the id of the link to which to send default routed multicast
-            
+
         :param multicast_default_to: The id of a link
         :type multicast_default_to: int
         :raise spinn_machine.exceptions.SpinnMachineAlreadyExistsException: If\
                     a value has already been set
         """
         if self._multicast_default_to is not None:
             raise SpinnMachineAlreadyExistsException(
                 "multicast_default_to", str(self._multicast_default_to))
         self._multicast_default_to = multicast_default_to
-    
+
     def __str__(self):
         return ("[Link: source_x={}, source_y={}, source_link_id={},"
                 " destination_x={}, destination_y={}, default_from={},"
                 " default_to={}]".format(self._source_x, self._source_y,
                                          self._source_link_id,
                                          self._destination_x,
                                          self._destination_y,
                                          self._multicast_default_from,
                                          self._multicast_default_to))
-    
+
     def __repr__(self):
         return self.__str__()
```

## Comparing `SpiNNMachine-2016.001/spinn_machine/multicast_routing_entry.py` & `SpiNNMachine-3.0.0/spinn_machine/multicast_routing_entry.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 from spinn_machine.exceptions import SpinnMachineInvalidParameterException
 
 
 class MulticastRoutingEntry(object):
     """ Represents an entry in a multicast routing table
     """
 
+    __slots__ = (
+        "_routing_entry_key", "_mask", "_defaultable", "_processor_ids",
+        "_link_ids"
+    )
+
     def __init__(self, routing_entry_key, mask, processor_ids, link_ids,
                  defaultable):
         """
 
         :param routing_entry_key: The routing key_combo
         :type routing_entry_key: int
         :param mask: The route key_combo mask
@@ -22,15 +27,15 @@
         :param defaultable: if this entry is defaultable (it receives packets \
         from its directly opposite route position)
         :type defaultable: bool
         :raise spinn_machine.exceptions.SpinnMachineAlreadyExistsException:
                     * If processor_ids contains the same id more than once
                     * If link_ids contains the same id more than once
         """
-        self._routing_key_entry = routing_entry_key
+        self._routing_entry_key = routing_entry_key
         self._mask = mask
         self._defaultable = defaultable
 
         if (routing_entry_key & mask) != routing_entry_key:
             raise SpinnMachineInvalidParameterException(
                 "key_mask_combo and mask",
                 "{} and {}".format(routing_entry_key, mask),
@@ -57,15 +62,15 @@
     @property
     def routing_entry_key(self):
         """ The routing key
 
         :return: The routing key
         :rtype: int
         """
-        return self._routing_key_entry
+        return self._routing_entry_key
 
     @property
     def mask(self):
         """ The routing mask
 
         :return: The routing mask
         :rtype: int
@@ -167,7 +172,18 @@
     def __repr__(self):
         return "{}:{}:{}:{}:{}".format(
             self._routing_key_entry, self._mask, self._defaultable,
             self._processor_ids, self._link_ids)
 
     def __str__(self):
         return self.__repr__()
+
+    def __getstate__(self):
+        return dict(
+            (slot, getattr(self, slot))
+            for slot in self.__slots__
+            if hasattr(self, slot)
+        )
+
+    def __setstate__(self, state):
+        for slot, value in state.items():
+            setattr(self, slot, value)
```

## Comparing `SpiNNMachine-2016.001/spinn_machine/processor.py` & `SpiNNMachine-3.0.0/spinn_machine/processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from spinn_machine.exceptions import SpinnMachineInvalidParameterException
 
 
 class Processor(object):
     """ A processor object included in a chip
     """
 
-    # ticks per 1 millisecond time step
-    CPU_AVAILABLE = 200000
-    DTCM_AVAILABLE = 2 ** 15
+    CLOCK_SPEED = 200 * 1000 * 1000
+    DTCM_AVAILABLE = 2 ** 16
 
-    def __init__(self, processor_id, clock_speed, is_monitor=False,
+    __slots__ = (
+        "_processor_id", "_clock_speed", "_is_monitor", "_dtcm_available"
+    )
+
+    def __init__(self, processor_id, clock_speed=CLOCK_SPEED, is_monitor=False,
                  dtcm_available=DTCM_AVAILABLE):
         """
 
         :param processor_id: id of the processor in the chip
         :type processor_id: int
         :param clock_speed: The number of cpu cycles per second of the\
                     processor
@@ -43,32 +46,32 @@
         :rtype: int
         :raise None: does not raise any known exceptions
         """
         return self._processor_id
 
     @property
     def dtcm_available(self):
-        """the amount of dtcm avilable on this processor
+        """ The amount of DTCM available on this processor
 
-        :return: the amount of dtcm avilable on this processor
+        :return: the amount of DTCM available on this processor
         :rtype: int
         :raise None: does not raise any known exceptions
 
         """
         return self._dtcm_available
 
     @property
     def cpu_cycles_available(self):
-        """the amount of cpu cycles available from this processor
+        """ The number of cpu cycles available from this processor per ms
 
-        :return: the amount of cpu cycles avilable on this processor
+        :return: the number of cpu cycles available on this processor
         :rtype: int
         :raise None: does not raise any known exceptions
         """
-        return Processor.CPU_AVAILABLE
+        return self._clock_speed / 1000.0
 
     @property
     def clock_speed(self):
         """ The clock speed of the processor in cycles per second
 
         :return: The clock speed in cycles per second
         :rtype: int
```

## Comparing `SpiNNMachine-2016.001/spinn_machine/router.py` & `SpiNNMachine-3.0.0/spinn_machine/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,21 @@
             * source_link_id is the id of a link
             * link is the link with id source_link_id
     """
     ROUTER_DEFAULT_AVAILABLE_ENTRIES = 1024
 
     ROUTER_DEFAULT_CLOCK_SPEED = 150 * 1024 * 1024
 
+    __slots__ = (
+        "_clock_speed", "_emergency_routing_enabled", "_links",
+        "_n_available_multicast_entries"
+    )
+
     def __init__(
-            self, links, emergency_routing_enabled,
+            self, links, emergency_routing_enabled=False,
             clock_speed=ROUTER_DEFAULT_CLOCK_SPEED,
             n_available_multicast_entries=ROUTER_DEFAULT_AVAILABLE_ENTRIES):
         """
         :param links: iterable of links
         :type links: iterable of :py:class:`spinn_machine.link.Link`
         :param emergency_routing_enabled: Determines if the router emergency\
                     routing is operating
@@ -151,19 +156,18 @@
                 self._emergency_routing_enabled,
                 self._n_available_multicast_entries, self._links.values()))
 
     def __repr__(self):
         return self.__str__()
 
     def get_neighbouring_chips_coords(self):
-        """utility method to convert links into x and y coords for placers
+        """ Utility method to convert links into x and y coordinates
 
-        :return: iterable list of destination coords in x and y dictonary
+        :return: iterable list of destination coordinates in x and y dict
         :rtype: iterable of dict
-        :raise None: this method does not raise any known excpetion
 
         """
         next_hop_chips_coords = list()
         for link in self.links:
             next_hop_chips_coords.append(
                 {'x': link.destination_x, 'y': link.destination_y})
         return next_hop_chips_coords
```

## Comparing `SpiNNMachine-2016.001/spinn_machine/spinnaker_link_data.py` & `SpiNNMachine-3.0.0/spinn_machine/link_data_objects/abstract_link_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,37 @@
-"""
-SpinnakerLinkData
-"""
+from six import add_metaclass
+from abc import ABCMeta
 
 
-class SpinnakerLinkData(object):
+@add_metaclass(ABCMeta)
+class AbstractLinkData(object):
     """ Data object for spinnaker links
     """
 
-    def __init__(self, spinnaker_link_id, connected_chip_x, connected_chip_y,
-                 connected_link):
-        self._spinnaker_link_id = spinnaker_link_id
+    __slots__ = (
+        "_board_address",
+        "_connected_chip_x",
+        "_connected_chip_y",
+        "_connected_link"
+    )
+
+    def __init__(self, connected_chip_x, connected_chip_y, connected_link,
+                 board_address):
+        self._board_address = board_address
         self._connected_chip_x = connected_chip_x
         self._connected_chip_y = connected_chip_y
         self._connected_link = connected_link
 
     @property
-    def spinnaker_link_id(self):
-        """ Get the id of the spinnaker link
+    def board_address(self):
+        """
+        property method for board address
+        :return:
         """
-        return self._spinnaker_link_id
+        return self._board_address
 
     @property
     def connected_chip_x(self):
         """
         property method for connected chip x
         :return:
         """
```

## Comparing `SpiNNMachine-2016.001/spinn_machine/__init__.py` & `SpiNNMachine-3.0.0/spinn_machine/__init__.py`

 * *Files identical despite different names*

## Comparing `SpiNNMachine-2016.001/spinn_machine/tags/abstract_tag.py` & `SpiNNMachine-3.0.0/spinn_machine/tags/abstract_tag.py`

 * *Files identical despite different names*

## Comparing `SpiNNMachine-2016.001/spinn_machine/tags/iptag.py` & `SpiNNMachine-3.0.0/spinn_machine/tags/iptag.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,16 +35,18 @@
     @property
     def strip_sdp(self):
         """ Return if the SDP header is to be stripped
         """
         return self._strip_sdp
 
     def __str__(self):
-        return "IP Tag on {}: tag={} port={} ip_address={}".format(
-            self._board_address, self._tag, self._port, self._ip_address)
+        return (
+            "IP Tag on {}: tag={} port={} ip_address={} strip_sdp={}".format(
+                self._board_address, self._tag, self._port, self._ip_address,
+                self._strip_sdp))
 
     def __eq__(self, other):
         if not isinstance(other, IPTag):
             return False
         else:
             if (self._ip_address == other._ip_address and
                     self._strip_sdp == other._strip_sdp and
```

## Comparing `SpiNNMachine-2016.001/spinn_machine/tags/reverse_iptag.py` & `SpiNNMachine-3.0.0/spinn_machine/tags/reverse_iptag.py`

 * *Files identical despite different names*

## Comparing `SpiNNMachine-2016.001/spinn_machine/utilities/ordered_set.py` & `SpiNNMachine-3.0.0/spinn_machine/utilities/ordered_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import collections
 
 
 class _Node(object):
 
+    __slots__ = (
+        "_key", "_prev_node", "_next_node"
+    )
+
     def __init__(self, key, prev_node, next_node):
         self._key = key
         self._prev_node = prev_node
         self._next_node = next_node
 
     @property
     def key(self):
@@ -27,27 +31,31 @@
     @next_node.setter
     def next_node(self, next_node):
         self._next_node = next_node
 
 
 class OrderedSet(collections.MutableSet):
 
+    __slots__ = (
+        "_end", "_map"
+    )
+
     def __init__(self, iterable=None):
 
         # sentinel node for doubly linked list
         # prev_node of end points to end of list (for reverse iteration)
         # next_node of end points to start of list (for forward iteration)
         self._end = _Node(None, None, None)
         self._end.prev_node = self._end
         self._end.next_node = self._end
 
         # key --> _Node
         self._map = dict()
 
-        # ior is overridden in mutable set; calls add on each element
+        # or is overridden in mutable set; calls add on each element
         if iterable is not None:
             self |= iterable
 
     def __len__(self):
         return len(self._map)
 
     def __contains__(self, key):
```

## Comparing `SpiNNMachine-2016.001/spinn_machine/utilities/progress_bar.py` & `SpiNNMachine-3.0.0/spinn_machine/utilities/progress_bar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-"""
-ProgressBar
-"""
 from __future__ import print_function
 import logging
 import sys
 import math
 
 logger = logging.getLogger(__name__)
 
 
 class ProgressBar(object):
     """ Progress bar for telling the user where a task is up to
     """
     MAX_LENGTH_IN_CHARS = 60
 
+    __slots__ = (
+        "_total_number_of_things_to_do", "_currently_completed",
+        "_chars_per_thing", "_last_update", "_chars_done", "_string"
+    )
+
     def __init__(self, total_number_of_things_to_do,
                  string_describing_what_being_progressed):
         self._total_number_of_things_to_do = total_number_of_things_to_do
         self._currently_completed = 0
         self._chars_per_thing = None
         self._last_update = 0
         self._chars_done = 0
```

