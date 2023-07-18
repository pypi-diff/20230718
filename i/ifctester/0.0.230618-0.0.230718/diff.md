# Comparing `tmp/ifctester-0.0.230618.tar.gz` & `tmp/ifctester-0.0.230718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifctester-0.0.230618.tar", last modified: Sun Jun 18 01:55:22 2023, max compression
+gzip compressed data, was "ifctester-0.0.230718.tar", last modified: Tue Jul 18 02:03:38 2023, max compression
```

## Comparing `ifctester-0.0.230618.tar` & `ifctester-0.0.230718.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:55:22.835736 ifctester-0.0.230618/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-18 01:55:22.835736 ifctester-0.0.230618/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-18 01:55:13.000000 ifctester-0.0.230618/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:55:22.835736 ifctester-0.0.230618/ifctester/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-18 01:55:13.000000 ifctester-0.0.230618/ifctester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-18 01:55:13.000000 ifctester-0.0.230618/ifctester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40966 2023-06-18 01:55:13.000000 ifctester-0.0.230618/ifctester/facet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-18 01:55:13.000000 ifctester-0.0.230618/ifctester/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-06-18 01:55:13.000000 ifctester-0.0.230618/ifctester/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:55:22.835736 ifctester-0.0.230618/ifctester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-18 01:55:22.000000 ifctester-0.0.230618/ifctester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-18 01:55:22.000000 ifctester-0.0.230618/ifctester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:55:22.000000 ifctester-0.0.230618/ifctester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 01:55:22.000000 ifctester-0.0.230618/ifctester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 01:55:22.000000 ifctester-0.0.230618/ifctester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-18 01:55:15.000000 ifctester-0.0.230618/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:55:22.835736 ifctester-0.0.230618/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:55:22.835736 ifctester-0.0.230618/test/
--rw-r--r--   0 runner    (1001) docker     (123)    88513 2023-06-18 01:55:13.000000 ifctester-0.0.230618/test/test_facet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-18 01:55:13.000000 ifctester-0.0.230618/test/test_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:38.716851 ifctester-0.0.230718/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-18 02:03:38.716851 ifctester-0.0.230718/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-18 02:03:27.000000 ifctester-0.0.230718/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:38.716851 ifctester-0.0.230718/ifctester/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-18 02:03:27.000000 ifctester-0.0.230718/ifctester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-18 02:03:27.000000 ifctester-0.0.230718/ifctester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46023 2023-07-18 02:03:27.000000 ifctester-0.0.230718/ifctester/facet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-07-18 02:03:27.000000 ifctester-0.0.230718/ifctester/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-07-18 02:03:27.000000 ifctester-0.0.230718/ifctester/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:38.716851 ifctester-0.0.230718/ifctester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-18 02:03:38.000000 ifctester-0.0.230718/ifctester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-18 02:03:38.000000 ifctester-0.0.230718/ifctester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:03:38.000000 ifctester-0.0.230718/ifctester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 02:03:38.000000 ifctester-0.0.230718/ifctester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 02:03:38.000000 ifctester-0.0.230718/ifctester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-18 02:03:30.000000 ifctester-0.0.230718/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 02:03:38.716851 ifctester-0.0.230718/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:38.716851 ifctester-0.0.230718/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    88738 2023-07-18 02:03:27.000000 ifctester-0.0.230718/test/test_facet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-07-18 02:03:27.000000 ifctester-0.0.230718/test/test_ids.py
```

### Comparing `ifctester-0.0.230618/PKG-INFO` & `ifctester-0.0.230718/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.230618
+Version: 0.0.230718
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Bug Tracker, https://github.com/ifcopenshell/ifcopenshell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -27,15 +27,15 @@
 # add specification to it
 my_spec = ids.Specification(name="My first specification")
 my_spec.applicability.append(ids.Entity(name="IFCWALL"))
 property = ids.Property(
     name="IsExternal", 
     value="TRUE", 
     propertySet="Pset_WallCommon", 
-    measure="IfcBoolean",
+    datatype="IfcBoolean",
     uri="https://identifier.buildingsmart.org/uri/.../prop/LoadBearing", 
     instructions="Walls need to be load bearing.",
     minOccurs=1,
     maxOccurs="unbounded")
 my_spec.requirements.append(property)
 my_ids.specifications.append(my_spec)
```

### Comparing `ifctester-0.0.230618/README.md` & `ifctester-0.0.230718/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # add specification to it
 my_spec = ids.Specification(name="My first specification")
 my_spec.applicability.append(ids.Entity(name="IFCWALL"))
 property = ids.Property(
     name="IsExternal", 
     value="TRUE", 
     propertySet="Pset_WallCommon", 
-    measure="IfcBoolean",
+    datatype="IfcBoolean",
     uri="https://identifier.buildingsmart.org/uri/.../prop/LoadBearing", 
     instructions="Walls need to be load bearing.",
     minOccurs=1,
     maxOccurs="unbounded")
 my_spec.requirements.append(property)
 my_ids.specifications.append(my_spec)
```

### Comparing `ifctester-0.0.230618/ifctester/__init__.py` & `ifctester-0.0.230718/ifctester/__init__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230618/ifctester/__main__.py` & `ifctester-0.0.230718/ifctester/__main__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230618/ifctester/facet.py` & `ifctester-0.0.230718/ifctester/facet.py`

 * *Files 10% similar despite different names*

```diff
@@ -127,14 +127,17 @@
         self.requirement_templates = [
             "Shall be {name} data of type {predefinedType}",
             "Shall be {name} data",
         ]
         super().__init__(name, predefinedType, instructions)
 
     def filter(self, ifc_file, elements):
+        if isinstance(elements, list):
+            return super().filter(ifc_file, elements)
+
         if isinstance(self.name, str):
             try:
                 results = ifc_file.by_type(self.name, include_subtypes=False)
             except:
                 # If the user has specified a class that doesn't exist in the version
                 results = []
         else:
@@ -176,29 +179,50 @@
         ]
         self.requirement_templates = [
             "The {name} shall be {value}",
             "The {name} shall be provided",
         ]
         super().__init__(name, value, minOccurs, maxOccurs, instructions)
 
+    def filter(self, ifc_file, elements):
+        if isinstance(elements, list):
+            return super().filter(ifc_file, elements)
+
+        results = []
+        schema = ifcopenshell.ifcopenshell_wrapper.schema_by_name(ifc_file.schema)
+        for entity in schema.entities():
+            for attribute in entity.attributes():
+                if attribute.name() == self.name:
+                    results.extend(ifc_file.by_type(entity.name(), include_subtypes=False))
+
+        # TODO: perhaps we should consider value in the filter
+
+        return results
+
     def __call__(self, inst, logger=None):
         if self.minOccurs == 0 and self.maxOccurs != 0:
             return AttributeResult(True)
 
         if isinstance(self.name, str):
             names = [self.name]
-            values = [getattr(inst, self.name, None)]
+            attribute_type = inst.wrapped_data.get_attribute_category(self.name)
+            if attribute_type == 1:  # Forward attribute
+                values = [getattr(inst, self.name, None)]
+            else:
+                values = [None]
         else:
             info = inst.get_info()
             names = []
             values = []
             for k, v in info.items():
                 if k == self.name:
-                    names.append(k)
-                    values.append(v)
+                    attribute_type = inst.wrapped_data.get_attribute_category(k)
+                    if attribute_type == 1:  # Forward attribute
+                        names.append(k)
+                        values.append(v)
 
         is_pass = bool(values)
         reason = None
 
         if not is_pass:
             reason = {"type": "NOVALUE"}
 
@@ -275,15 +299,17 @@
             "Shall be classified using {system}",
             "Shall be classified as {value}",
             "Shall be classified",
         ]
         super().__init__(value, system, uri, minOccurs, maxOccurs, instructions)
 
     def filter(self, ifc_file, elements):
-        pass
+        if isinstance(elements, list):
+            return super().filter(ifc_file, elements)
+        return ifc_file.by_type("IfcObjectDefinition")
 
     def __call__(self, inst, logger=None):
         if self.minOccurs == 0 and self.maxOccurs != 0:
             return ClassificationResult(True)
 
         leaf_references = ifcopenshell.util.classification.get_references(inst)
 
@@ -313,17 +339,17 @@
             return ClassificationResult(not is_pass, {"type": "PROHIBITED"})
         return ClassificationResult(is_pass, reason)
 
 
 class PartOf(Facet):
     def __init__(
         self,
-        entity=None,
+        entity="IFCWALL",
         predefinedType=None,
-        relation="IfcRelAggregates",
+        relation=None,
         minOccurs=None,
         maxOccurs=None,
         instructions=None,
     ):
         self.parameters = ["entity", "predefinedType", "@relation", "@minOccurs", "@maxOccurs", "@instructions"]
         self.applicability_templates = [
             "An element with an {relation} relationship with an {entity}",
@@ -331,14 +357,19 @@
         ]
         self.requirement_templates = [
             "An element must have an {relation} relationship with an {entity}",
             "An element must have an {relation} relationship",
         ]
         super().__init__(entity, predefinedType, relation, minOccurs, maxOccurs, instructions)
 
+    def filter(self, ifc_file, elements):
+        if isinstance(elements, list):
+            return super().filter(ifc_file, elements)
+        return list(ifc_file)  # Lazy
+
     def asdict(self):
         results = super().asdict()
         entity = {}
         if "entity" in results:
             entity["name"] = results["entity"]
             del results["entity"]
         if "predefinedType" in results:
@@ -355,15 +386,31 @@
         return super().parse(xml)
 
     def __call__(self, inst, logger=None):
         if self.minOccurs == 0 and self.maxOccurs != 0:
             return PartOfResult(True)
 
         reason = None
-        if self.relation == "IfcRelAggregates":
+        if not self.relation:
+            is_pass = False
+            ancestors = []
+            parent = self.get_parent(inst)
+            while parent:
+                ancestors.append(parent.is_a())
+                if parent.is_a().upper() == self.entity:
+                    if self.predefinedType:
+                        if ifcopenshell.util.element.get_predefined_type(parent) == self.predefinedType:
+                            is_pass = True
+                    else:
+                        is_pass = True
+                    break
+                parent = self.get_parent(parent)
+            if not is_pass:
+                reason = {"type": "ENTITY", "actual": ancestors}
+        elif self.relation == "IFCRELAGGREGATES":
             aggregate = ifcopenshell.util.element.get_aggregate(inst)
             is_pass = aggregate is not None
             if not is_pass:
                 reason = {"type": "NOVALUE"}
             if is_pass and self.entity:
                 is_pass = False
                 ancestors = []
@@ -375,15 +422,15 @@
                                 is_pass = True
                         else:
                             is_pass = True
                         break
                     aggregate = ifcopenshell.util.element.get_aggregate(aggregate)
                 if not is_pass:
                     reason = {"type": "ENTITY", "actual": ancestors}
-        elif self.relation == "IfcRelAssignsToGroup":
+        elif self.relation == "IFCRELASSIGNSTOGROUP":
             group = None
             for rel in getattr(inst, "HasAssignments", []) or []:
                 if rel.is_a("IfcRelAssignsToGroup"):
                     group = rel.RelatingGroup
                     break
             is_pass = group is not None
             if not is_pass:
@@ -393,29 +440,29 @@
                     is_pass = False
                     reason = {"type": "ENTITY", "actual": group.is_a().upper()}
                 if self.predefinedType:
                     predefined_type = ifcopenshell.util.element.get_predefined_type(group)
                     if predefined_type != self.predefinedType:
                         is_pass = False
                         reason = {"type": "PREDEFINEDTYPE", "actual": predefined_type}
-        elif self.relation == "IfcRelContainedInSpatialStructure":
+        elif self.relation == "IFCRELCONTAINEDINSPATIALSTRUCTURE":
             container = ifcopenshell.util.element.get_container(inst)
             is_pass = container is not None
             if not is_pass:
                 reason = {"type": "NOVALUE"}
             if is_pass and self.entity:
                 if container.is_a().upper() != self.entity:
                     is_pass = False
                     reason = {"type": "ENTITY", "actual": container.is_a().upper()}
                 if self.predefinedType:
                     predefined_type = ifcopenshell.util.element.get_predefined_type(container)
                     if predefined_type != self.predefinedType:
                         is_pass = False
                         reason = {"type": "PREDEFINEDTYPE", "actual": predefined_type}
-        elif self.relation == "IfcRelNests":
+        elif self.relation == "IFCRELNESTS":
             nest = self.get_nested_whole(inst)
             is_pass = nest is not None
             if not is_pass:
                 reason = {"type": "NOVALUE"}
             if is_pass and self.entity:
                 is_pass = False
                 ancestors = []
@@ -427,66 +474,131 @@
                                 is_pass = True
                         else:
                             is_pass = True
                         break
                     nest = self.get_nested_whole(nest)
                 if not is_pass:
                     reason = {"type": "ENTITY", "actual": ancestors}
+        elif self.relation == "IFCRELVOIDSELEMENT":
+            building_element = self.get_voided_element(inst)
+            is_pass = building_element is not None
+            if not is_pass:
+                reason = {"type": "NOVALUE"}
+            if is_pass and self.entity:
+                is_pass = False
+                if building_element.is_a().upper() == self.entity:
+                    if self.predefinedType:
+                        if ifcopenshell.util.element.get_predefined_type(building_element) == self.predefinedType:
+                            is_pass = True
+                    else:
+                        is_pass = True
+                if not is_pass:
+                    reason = {"type": "ENTITY", "actual": building_element}
+        elif self.relation == "IFCRELFILLSELEMENT":
+            opening = self.filled_opening(inst)
+            is_pass = opening is not None
+            if not is_pass:
+                reason = {"type": "NOVALUE"}
+            if is_pass and self.entity:
+                is_pass = False
+                if opening.is_a().upper() == self.entity:
+                    if self.predefinedType:
+                        if ifcopenshell.util.element.get_predefined_type(opening) == self.predefinedType:
+                            is_pass = True
+                    else:
+                        is_pass = True
+                if not is_pass:
+                    reason = {"type": "ENTITY", "actual": opening}
 
         if self.maxOccurs == 0:
             return PartOfResult(not is_pass, {"type": "PROHIBITED"})
         return PartOfResult(is_pass, reason)
 
     def get_nested_whole(self, element):
         for rel in getattr(element, "Nests", []) or []:
             return rel.RelatingObject
 
+    def get_voided_element(self, element):
+        for rel in getattr(element, "VoidsElements", []) or []:
+            return rel.RelatingBuildingElement
+
+    def get_filled_opening(self, element):
+        for rel in getattr(element, "FillsVoids", []) or []:
+            return rel.RelatingOpeningElement
+
+    def get_parent(self, element):
+        parent = ifcopenshell.util.element.get_aggregate(element)
+        if not parent:
+            parent = ifcopenshell.util.element.get_container(element, should_get_direct=True)
+        if not parent:
+            for rel in getattr(element, "HasAssignments", []) or []:
+                if rel.is_a("IfcRelAssignsToGroup"):
+                    parent = rel.RelatingGroup
+                    break
+        if not parent:
+            self.get_nested_whole(element)
+        if not parent:
+            self.get_voided_element(element)
+        if not parent:
+            self.get_filled_opening(element)
+        return parent
+
 
 class Property(Facet):
     def __init__(
         self,
         propertySet="Property_Set",
         name="PropertyName",
         value=None,
-        measure=None,
+        datatype=None,
         uri=None,
         minOccurs=None,
         maxOccurs=None,
         instructions=None,
     ):
         self.parameters = [
             "propertySet",
             "name",
             "value",
-            "@measure",
+            "@datatype",
             "@uri",
             "@minOccurs",
             "@maxOccurs",
             "@instructions",
         ]
         self.applicability_templates = [
             "Elements with {name} data of {value} in the dataset {propertySet}",
             "Elements with {name} data in the dataset {propertySet}",
         ]
         self.requirement_templates = [
             "{name} data shall be {value} and in the dataset {propertySet}",
             "{name} data shall be provided in the dataset {propertySet}",
         ]
-        super().__init__(propertySet, name, value, measure, uri, minOccurs, maxOccurs, instructions)
+        super().__init__(propertySet, name, value, datatype, uri, minOccurs, maxOccurs, instructions)
+
+    def filter(self, ifc_file, elements):
+        if isinstance(elements, list):
+            return super().filter(ifc_file, elements)
+        if ifc_file.schema == "IFC2X3":
+            return ifc_file.by_type("IfcObjectDefinition")
+        return (
+            ifc_file.by_type("IfcObjectDefinition")
+            + ifc_file.by_type("IfcMaterialDefinition")
+            + ifc_file.by_type("IfcProfileDef")
+        )
 
     def __call__(self, inst, logger=None):
         if self.minOccurs == 0 and self.maxOccurs != 0:
             return PropertyResult(True)
 
-        all_psets = ifcopenshell.util.element.get_psets(inst)
-
         if isinstance(self.propertySet, str):
-            pset = all_psets.get(self.propertySet, None)
+            pset = ifcopenshell.util.element.get_pset(inst, self.propertySet)
             psets = {self.propertySet: pset} if pset else {}
         else:
+            all_psets = ifcopenshell.util.element.get_psets(inst)
             psets = {k: v for k, v in all_psets.items() if k == self.propertySet}
 
         is_pass = bool(psets)
         reason = None
 
         if not is_pass:
             reason = {"type": "NOPSET"}
@@ -521,17 +633,17 @@
                         continue
                     if not isinstance(prop_entity, ifcopenshell.entity_instance):
                         # Predefined properties are special :(
                         pass
                     elif prop_entity.is_a("IfcPropertySingleValue"):
                         data_type = prop_entity.NominalValue.is_a()
 
-                        if data_type != self.measure:
+                        if data_type != self.datatype:
                             is_pass = False
-                            reason = {"type": "MEASURE", "actual": data_type}
+                            reason = {"type": "DATATYPE", "actual": data_type}
                             break
 
                         unit = ifcopenshell.util.unit.get_property_unit(prop_entity, inst.wrapped_data.file)
                         if unit and getattr(unit, "Name", None):
                             # TODO support unnamed derived units
                             props[pset_name][prop_entity.Name] = ifcopenshell.util.unit.convert(
                                 prop_entity.NominalValue.wrappedValue,
@@ -540,17 +652,17 @@
                                 None,
                                 ifcopenshell.util.unit.si_type_names[unit.UnitType],
                             )
                     elif prop_entity.is_a("IfcPhysicalSimpleQuantity"):
                         prop_schema = prop_entity.wrapped_data.declaration().as_entity()
                         data_type = prop_schema.attribute_by_index(3).type_of_attribute().declared_type().name()
 
-                        if data_type != self.measure:
+                        if data_type != self.datatype:
                             is_pass = False
-                            reason = {"type": "MEASURE", "actual": data_type}
+                            reason = {"type": "DATATYPE", "actual": data_type}
                             break
 
                         unit = ifcopenshell.util.unit.get_property_unit(prop_entity, inst.wrapped_data.file)
                         if unit:
                             props[pset_name][prop_entity.Name] = ifcopenshell.util.unit.convert(
                                 prop_entity[3],
                                 getattr(unit, "Prefix", None),
@@ -560,27 +672,27 @@
                             )
                     elif prop_entity.is_a("IfcPropertyEnumeratedValue"):
                         if not prop_entity.EnumerationValues:
                             is_pass = False
                             reason = {"type": "NOVALUE"}
                             break
                         data_type = prop_entity.EnumerationValues[0].is_a()
-                        if data_type != self.measure:
+                        if data_type != self.datatype:
                             is_pass = False
-                            reason = {"type": "MEASURE", "actual": data_type}
+                            reason = {"type": "DATATYPE", "actual": data_type}
                             break
                     elif prop_entity.is_a("IfcPropertyListValue"):
                         if not prop_entity.ListValues:
                             is_pass = False
                             reason = {"type": "NOVALUE"}
                             break
                         data_type = prop_entity.ListValues[0].is_a()
-                        if data_type != self.measure:
+                        if data_type != self.datatype:
                             is_pass = False
-                            reason = {"type": "MEASURE", "actual": data_type}
+                            reason = {"type": "DATATYPE", "actual": data_type}
                             break
                         unit = ifcopenshell.util.unit.get_property_unit(prop_entity, inst.wrapped_data.file)
                         if unit:
                             props[pset_name][prop_entity.Name] = [
                                 ifcopenshell.util.unit.convert(
                                     v,
                                     getattr(unit, "Prefix", None),
@@ -593,17 +705,17 @@
                     elif prop_entity.is_a("IfcPropertyBoundedValue"):
                         values = []
                         for attribute in ["UpperBoundValue", "LowerBoundValue", "SetPointValue"]:
                             value = getattr(prop_entity, attribute)
                             if value is not None:
                                 data_type = value.is_a()
                                 values.append(value.wrappedValue)
-                        if data_type != self.measure:
+                        if data_type != self.datatype:
                             is_pass = False
-                            reason = {"type": "MEASURE", "actual": data_type}
+                            reason = {"type": "DATATYPE", "actual": data_type}
                             break
                         unit = ifcopenshell.util.unit.get_property_unit(prop_entity, inst.wrapped_data.file)
                         if unit:
                             values = [
                                 ifcopenshell.util.unit.convert(
                                     v,
                                     getattr(unit, "Prefix", None),
@@ -618,15 +730,15 @@
                         values = []
                         units = ifcopenshell.util.unit.get_property_unit(prop_entity, inst.wrapped_data.file)
                         for attribute in ["Defining", "Defined"]:
                             column_values = props[pset_name][prop_entity.Name][f"{attribute}Values"]
                             if not column_values:
                                 continue
                             data_type = column_values[0].is_a()
-                            if data_type == self.measure:
+                            if data_type == self.datatype:
                                 column_values = [v.wrappedValue for v in column_values]
                                 unit = units[f"{attribute}Unit"]
                                 if unit:
                                     column_values = [
                                         ifcopenshell.util.unit.convert(
                                             v,
                                             getattr(unit, "Prefix", None),
@@ -635,15 +747,15 @@
                                             ifcopenshell.util.unit.si_type_names[unit.UnitType],
                                         )
                                         for v in column_values
                                     ]
                                 values.extend(column_values)
                         if not values:
                             is_pass = False
-                            reason = {"type": "MEASURE", "actual": data_type}
+                            reason = {"type": "DATATYPE", "actual": data_type}
                             break
                         props[pset_name][prop_entity.Name] = values
                     else:
                         is_property_supported_class = False
 
                 if not is_property_supported_class:
                     is_pass = False
@@ -720,14 +832,19 @@
         ]
         self.requirement_templates = [
             "Shall have a material of {value}",
             "Shall have a material",
         ]
         super().__init__(value, uri, minOccurs, maxOccurs, instructions)
 
+    def filter(self, ifc_file, elements):
+        if isinstance(elements, list):
+            return super().filter(ifc_file, elements)
+        return ifc_file.by_type("IfcObjectDefinition")
+
     def __call__(self, inst, logger=None):
         if self.minOccurs == 0 and self.maxOccurs != 0:
             return MaterialResult(True)
 
         material = ifcopenshell.util.element.get_material(inst, should_skip_usage=True)
 
         is_pass = material is not None
@@ -913,15 +1030,15 @@
 
 class PropertyResult(Result):
     def to_string(self):
         if self.reason["type"] == "NOPSET":
             return "The required property set does not exist"
         elif self.reason["type"] == "NOVALUE":
             return "The property set does not contain the required property"
-        elif self.reason["type"] == "MEASURE":
+        elif self.reason["type"] == "DATATYPE":
             return f"The data type \"{str(self.reason['actual'])}\" does not match the requirements"
         elif self.reason["type"] == "VALUE":
             if isinstance(self.reason["actual"], list):
                 if len(self.reason["actual"]) == 1:
                     return f"The property value \"{str(self.reason['actual'][0])}\" does not match the requirements"
                 else:
                     return f"The property values \"{str(self.reason['actual'])}\" do not match the requirements"
```

### Comparing `ifctester-0.0.230618/ifctester/ids.py` & `ifctester-0.0.230718/ifctester/ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,26 +196,22 @@
             facet.failed_entities.clear()
         self.status = None
 
     def validate(self, ifc_file, filter_version=False):
         if filter_version and ifc_file.schema not in self.ifcVersion:
             return
 
-        elements = []
+        elements = None
         
+        # This is a broadphase filter of applicability. We almost never want to
+        # test every single class in an IFC model.
         for i, facet in enumerate(self.applicability):
-            # Usually, we rely on an entity applicability to give us our first
-            # shortlist of elements, as it's the most efficient way to filter
-            # elements. If this does not exist, then we have no choice but to
-            # check everything.
-            if i == 0 and not isinstance(facet, Entity):
-                elements = list(ifc_file)
             elements = facet.filter(ifc_file, elements)
 
-        for element in elements:
+        for element in elements or []:
             is_applicable = True
             for facet in self.applicability:
                 if isinstance(facet, Entity):
                     continue
                 if not bool(facet(element)):
                     is_applicable = False
                     break
```

### Comparing `ifctester-0.0.230618/ifctester/reporter.py` & `ifctester-0.0.230718/ifctester/reporter.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230618/ifctester.egg-info/PKG-INFO` & `ifctester-0.0.230718/ifctester.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.230618
+Version: 0.0.230718
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Bug Tracker, https://github.com/ifcopenshell/ifcopenshell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -27,15 +27,15 @@
 # add specification to it
 my_spec = ids.Specification(name="My first specification")
 my_spec.applicability.append(ids.Entity(name="IFCWALL"))
 property = ids.Property(
     name="IsExternal", 
     value="TRUE", 
     propertySet="Pset_WallCommon", 
-    measure="IfcBoolean",
+    datatype="IfcBoolean",
     uri="https://identifier.buildingsmart.org/uri/.../prop/LoadBearing", 
     instructions="Walls need to be load bearing.",
     minOccurs=1,
     maxOccurs="unbounded")
 my_spec.requirements.append(property)
 my_ids.specifications.append(my_spec)
```

### Comparing `ifctester-0.0.230618/pyproject.toml` & `ifctester-0.0.230718/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ifctester"
-version = "0.0.230618"
+version = "0.0.230718"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "IFC model auditing tool with support for IDS"
 readme = "README.md"
 keywords = ["IFC", "IDS", "BIM"]
 classifiers = [
```

### Comparing `ifctester-0.0.230618/test/test_facet.py` & `ifctester-0.0.230718/test/test_facet.py`

 * *Files 3% similar despite different names*

```diff
@@ -834,139 +834,139 @@
             "propertySet": {"simpleValue": "Property_Set"},
             "name": {"simpleValue": "PropertyName"},
         }
         facet = Property(
             propertySet="propertySet",
             name="name",
             value="value",
-            measure="measure",
+            datatype="datatype",
             uri="https://test.com",
             minOccurs="0",
             maxOccurs="unbounded",
             instructions="instructions",
         )
         assert facet.asdict() == {
             "propertySet": {"simpleValue": "propertySet"},
             "name": {"simpleValue": "name"},
             "value": {"simpleValue": "value"},
-            "@measure": "measure",
+            "@datatype": "datatype",
             "@uri": "https://test.com",
             "@minOccurs": "0",
             "@maxOccurs": "unbounded",
             "@instructions": "instructions",
         }
 
     def test_filtering_using_a_property_facet(self):
         set_facet("property")
 
         ifc = self.setup_ifc()
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcLabel")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         run("Elements with no properties always fail", facet=facet, inst=element, expected=False)
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"AnotherProperty": "AnotherValue"})
         run("Elements with a matching pset but no property also fail", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"AnotherProperty": None})
         run("Properties with a null value fail", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
         run("A name check will match any property with any string value", facet=facet, inst=element, expected=True)
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcLabel")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
         run("A required facet checks all parameters as normal", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcLabel", minOccurs=0, maxOccurs=0)
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcLabel", minOccurs=0, maxOccurs=0)
         run("A prohibited facet returns the opposite of a required facet", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcLabel", minOccurs=0)
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcLabel", minOccurs=0)
         run("An optional facet always passes regardless of outcome 1/2", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Bar", measure="IfcLabel", minOccurs=0)
+        facet = Property(propertySet="Foo_Bar", name="Bar", datatype="IfcLabel", minOccurs=0)
         run("An optional facet always passes regardless of outcome 2/2", facet=facet, inst=element, expected=True)
 
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ""})
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcLogical")
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcLogical")
         run("An empty string is considered falsey and will not pass", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcLogical("UNKNOWN")})
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcDuration")
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcDuration")
         run("A logical unknown is considered falsey and will not pass", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcDuration("P0D")})
         run("A zero duration will pass", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcBoolean")
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcBoolean")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcBoolean(True)})
         run("A property set to true will pass a name check", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": False})
         run(
             "A property set to false is still considered a value and will pass a name check",
             facet=facet,
             inst=element,
             expected=True,
         )
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="Bar", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="Bar", datatype="IfcLabel")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
         run("Specifying a value performs a case-sensitive match 1/2", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "bar"})
         run("Specifying a value performs a case-sensitive match 2/2", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Baz"})
         run("Specifying a value fails against different values", facet=facet, inst=element, expected=False)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="♫Don'tÄrgerhôtelЊет", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="♫Don'tÄrgerhôtelЊет", datatype="IfcLabel")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "♫Don'tÄrgerhôtelЊет"})
         run("Non-ascii characters are treated without encoding", facet=facet, inst=element, expected=True)
 
         identifier = "123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345"
         facet = Property(
-            propertySet="Foo_Bar", name="Foo", value=identifier + "_extra_characters", measure="IfcIdentifier"
+            propertySet="Foo_Bar", name="Foo", value=identifier + "_extra_characters", datatype="IfcIdentifier"
         )
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcIdentifier(identifier)})
         run("IDS does not handle string truncation such as for identifiers", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="1", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="1", datatype="IfcLabel")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "1"})
         run("A number specified as a string is treated as a string", facet=facet, inst=element, expected=True)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42", measure="IfcInteger")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="42", datatype="IfcInteger")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcInteger(42)})
         run("Integer values are checked using type casting 1/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.", measure="IfcInteger")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.", datatype="IfcInteger")
         run("Integer values are checked using type casting 2/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.0", measure="IfcInteger")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.0", datatype="IfcInteger")
         run("Integer values are checked using type casting 3/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.3", measure="IfcInteger")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.3", datatype="IfcInteger")
         run("Integer values are checked using type casting 4/4", facet=facet, inst=element, expected=False)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42", measure="IfcReal")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="42", datatype="IfcReal")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.0)})
         run("Real values are checked using type casting 1/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.0", measure="IfcReal")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.0", datatype="IfcReal")
         run("Real values are checked using type casting 2/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.3", measure="IfcReal")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.3", datatype="IfcReal")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.3)})
         run("Real values are checked using type casting 3/3", facet=facet, inst=element, expected=True)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42,3", measure="IfcReal")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="42,3", datatype="IfcReal")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.3)})
         run("Only specifically formatted numbers are allowed 1/4", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="123,4.5", measure="IfcReal")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="123,4.5", datatype="IfcReal")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(1234.5)})
         run("Only specifically formatted numbers are allowed 2/4", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="1.2345e3", measure="IfcReal")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="1.2345e3", datatype="IfcReal")
         run("Only specifically formatted numbers are allowed 3/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="1.2345E3", measure="IfcReal")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="1.2345E3", datatype="IfcReal")
         run("Only specifically formatted numbers are allowed 4/4", facet=facet, inst=element, expected=True)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.", measure="IfcReal")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.", datatype="IfcReal")
         ifcopenshell.api.run(
             "pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.0 * (1.0 + 1e-6))}
         )
         run("Floating point numbers are compared with a 1e-6 tolerance 1/4", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run(
             "pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.0 * (1.0 - 1e-6))}
         )
@@ -976,31 +976,31 @@
         )
         run("Floating point numbers are compared with a 1e-6 tolerance 3/4", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run(
             "pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.0 * (1.0 - 2e-6))}
         )
         run("Floating point numbers are compared with a 1e-6 tolerance 4/4", facet=facet, inst=element, expected=False)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="TRUE", measure="IfcBoolean")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="TRUE", datatype="IfcBoolean")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcBoolean(False)})
         run("Booleans must be specified as uppercase strings 1/3", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="FALSE", measure="IfcBoolean")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="FALSE", datatype="IfcBoolean")
         run("Booleans must be specified as uppercase strings 2/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="False", measure="IfcBoolean")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="False", datatype="IfcBoolean")
         run("Booleans must be specified as uppercase strings 3/3", facet=facet, inst=element, expected=False)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="2022-01-01", measure="IfcDate")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="2022-01-01", datatype="IfcDate")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcDate("2022-01-01")})
         run("Dates are treated as strings 1/2", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run(
             "pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcDate("2022-01-01+00:00")}
         )
         run("Dates are treated as strings 2/2", facet=facet, inst=element, expected=False)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="PT16H", measure="IfcDuration")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="PT16H", datatype="IfcDuration")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcDuration("PT16H")})
         run("Durations are treated as strings 1/2", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcDuration("P2D")})
         run("Durations are treated as strings 1/2", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
@@ -1009,73 +1009,73 @@
         ifcopenshell.api.run(
             "pset.edit_pset",
             ifc,
             pset=pset,
             properties={"Status": ["EXISTING", "DEMOLISH"]},
             pset_template=pset_template,
         )
-        facet = Property(propertySet="Pset_WallCommon", name="Status", value="EXISTING", measure="IfcLabel")
+        facet = Property(propertySet="Pset_WallCommon", name="Status", value="EXISTING", datatype="IfcLabel")
         run("Any matching value in an enumerated property will pass 1/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Pset_WallCommon", name="Status", value="DEMOLISH", measure="IfcLabel")
+        facet = Property(propertySet="Pset_WallCommon", name="Status", value="DEMOLISH", datatype="IfcLabel")
         run("Any matching value in an enumerated property will pass 2/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Pset_WallCommon", name="Status", value="NEW", measure="IfcLabel")
+        facet = Property(propertySet="Pset_WallCommon", name="Status", value="NEW", datatype="IfcLabel")
         run("Any matching value in an enumerated property will pass 3/3", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         list_property = ifc.createIfcPropertyListValue(
             Name="Foo", ListValues=[ifc.createIfcLabel("X"), ifc.createIfcLabel("Y")]
         )
         pset.HasProperties = [list_property]
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="X", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="X", datatype="IfcLabel")
         run("Any matching value in a list property will pass 1/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="Y", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="Y", datatype="IfcLabel")
         run("Any matching value in a list property will pass 2/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="Z", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="Z", datatype="IfcLabel")
         run("Any matching value in a list property will pass 3/3", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         bounded_property = ifc.createIfcPropertyBoundedValue(
             Name="Foo",
             UpperBoundValue=ifc.createIfcLengthMeasure(5000),
             LowerBoundValue=ifc.createIfcLengthMeasure(1000),
             SetPointValue=ifc.createIfcLengthMeasure(3000),
         )
         pset.HasProperties = [bounded_property]
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="1", measure="IfcLengthMeasure")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="1", datatype="IfcLengthMeasure")
         run("Any matching value in a bounded property will pass 1/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="5", measure="IfcLengthMeasure")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="5", datatype="IfcLengthMeasure")
         run("Any matching value in a bounded property will pass 2/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="3", measure="IfcLengthMeasure")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="3", datatype="IfcLengthMeasure")
         run("Any matching value in a bounded property will pass 3/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="2", measure="IfcLengthMeasure")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="2", datatype="IfcLengthMeasure")
         run("Any matching value in a bounded property will pass 4/4", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         table_property = ifc.createIfcPropertyTableValue(
             Name="Foo", DefiningValues=[ifc.createIfcLabel("X")], DefinedValues=[ifc.createIfcLengthMeasure(1000)]
         )
         pset.HasProperties = [table_property]
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="X", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="X", datatype="IfcLabel")
         run("Any matching value in a table property will pass 1/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="1", measure="IfcLengthMeasure")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="1", datatype="IfcLengthMeasure")
         run("Any matching value in a table property will pass 2/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="Y", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="Y", datatype="IfcLabel")
         run("Any matching value in a table property will pass 3/3", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         pset.HasProperties = [ifc.createIfcPropertyReferenceValue(Name="Foo")]
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcLabel")
         run("Reference properties are treated as objects and not supported", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcDoor")
         pset = ifc.create_entity(
             "IfcDoorPanelProperties",
             GlobalId=ifcopenshell.guid.new(),
@@ -1086,84 +1086,84 @@
         ifc.create_entity(
             "IfcRelDefinesByProperties",
             GlobalId=ifcopenshell.guid.new(),
             RelatedObjects=[element],
             RelatingPropertyDefinition=pset,
         )
         facet = Property(
-            propertySet="Foo_Bar", name="PanelOperation", value="SWINGING", measure="IfcDoorPanelOperationEnum"
+            propertySet="Foo_Bar", name="PanelOperation", value="SWINGING", datatype="IfcDoorPanelOperationEnum"
         )
         run("Predefined properties are supported but discouraged 1/2", facet=facet, inst=element, expected=True)
         facet = Property(
-            propertySet="Foo_Bar", name="PanelOperation", value="SWONGING", measure="IfcDoorPanelOperationEnum"
+            propertySet="Foo_Bar", name="PanelOperation", value="SWONGING", datatype="IfcDoorPanelOperationEnum"
         )
         run("Predefined properties are supported but discouraged 2/2", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcLengthMeasure")
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcLengthMeasure")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         qto = ifcopenshell.api.run("pset.add_qto", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_qto", ifc, qto=qto, properties={"Foo": ifc.createIfcLengthMeasure(42)})
         run("A name check will match any quantity with any value", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcAreaMeasure")
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcAreaMeasure")
         run("Quantities must also match the appropriate measure", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         complex_property = ifc.createIfcComplexProperty(Name="Foo", UsageName="RabbitAgilityTraining")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=complex_property, properties={"Rabbits": "Awesome"})
         pset.HasProperties = [complex_property]
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcLabel")
         run("Complex properties are not supported 1/2", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo", name="Rabbits", measure="IfcLabel")
+        facet = Property(propertySet="Foo", name="Rabbits", datatype="IfcLabel")
         run("Complex properties are not supported 2/2", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         qto = ifcopenshell.api.run("pset.add_qto", ifc, product=element, name="Foo_Bar")
         complex_quantity = ifc.createIfcPhysicalComplexQuantity(Name="Foo", Discrimination="FurThickness")
         ifcopenshell.api.run(
             "pset.edit_qto", ifc, qto=complex_quantity, properties={"MyLength": ifc.createIfcLengthMeasure(42)}
         )
         qto.Quantities = [complex_quantity]
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcLengthMeasure")
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcLengthMeasure")
         run("Complex properties are not supported 1/2", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo", name="MyLength", measure="IfcLengthMeasure")
+        facet = Property(propertySet="Foo", name="MyLength", datatype="IfcLengthMeasure")
         run("Complex properties are not supported 2/2", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         restriction = Restriction(options={"pattern": "Foo_.*"})
-        facet = Property(propertySet=restriction, name="Foo", measure="IfcLabel")
+        facet = Property(propertySet=restriction, name="Foo", datatype="IfcLabel")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
         run("All matching property sets must satisfy requirements 1/3", facet=facet, inst=element, expected=True)
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Baz")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"AnotherProperty": "AnotherValue"})
         run("All matching property sets must satisfy requirements 2/3", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
         run("All matching property sets must satisfy requirements 3/3", facet=facet, inst=element, expected=True)
 
         ifc = self.setup_ifc()
         restriction = Restriction(options={"pattern": "Foo.*"})
-        facet = Property(propertySet="Foo_Bar", name=restriction, value="x", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name=restriction, value="x", datatype="IfcLabel")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foobar": "x"})
         run("All matching properties must satisfy requirements 1/3", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foobar": "x", "Foobaz": "x"})
         run("All matching properties must satisfy requirements 2/3", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foobar": "x", "Foobaz": "y"})
         run("All matching properties must satisfy requirements 3/3", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         restriction1 = Restriction(options={"pattern": "Foo.*"})
         restriction2 = Restriction(options={"enumeration": ["x", "y"]})
-        facet = Property(propertySet="Foo_Bar", name=restriction1, value=restriction2, measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name=restriction1, value=restriction2, datatype="IfcLabel")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foobar": "x", "Foobaz": "y"})
         run(
             "If multiple properties are matched, all values must satisfy requirements 1/2",
             facet=facet,
             inst=element,
@@ -1174,24 +1174,24 @@
             "If multiple properties are matched, all values must satisfy requirements 2/2",
             facet=facet,
             inst=element,
             expected=False,
         )
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="2", measure="IfcTimeMeasure")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="2", datatype="IfcTimeMeasure")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcMassMeasure(2)})
         run("Measures are used to specify an IFC data type 1/2", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcTimeMeasure(2)})
         run("Measures are used to specify an IFC data type 2/2", facet=facet, inst=element, expected=True)
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="2", measure="IfcLengthMeasure")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="2", datatype="IfcLengthMeasure")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcLengthMeasure(2)})
         run(
             "Unit conversions shall take place to IDS-nominated standard units 1/2",
             facet=facet,
             inst=element,
@@ -1207,27 +1207,27 @@
 
         ifc = self.setup_ifc()
         wall = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         wall_type = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWallType")
         ifcopenshell.api.run("type.assign_type", ifc, related_object=wall, relating_type=wall_type)
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=wall_type, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
-        facet = Property(propertySet="Foo_Bar", name="Foo", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IfcLabel")
         run("Properties can be inherited from the type 1/2", facet=facet, inst=wall, expected=True)
         run("Properties can be inherited from the type 2/2", facet=facet, inst=wall_type, expected=True)
 
         ifc = self.setup_ifc()
         wall = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         wall_type = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWallType")
         ifcopenshell.api.run("type.assign_type", ifc, related_object=wall, relating_type=wall_type)
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=wall_type, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Baz"})
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=wall, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="Bar", measure="IfcLabel")
+        facet = Property(propertySet="Foo_Bar", name="Foo", value="Bar", datatype="IfcLabel")
         run("Properties can be overriden by an occurrence 1/2", facet=facet, inst=wall, expected=True)
         run("Properties can be overriden by an occurrence 2/2", facet=facet, inst=wall_type, expected=False)
 
     def setup_ifc(self):
         ifc = ifcopenshell.file()
         ifc.createIfcProject()
         # Milli prefix used to check measurement conversions
@@ -1396,172 +1396,172 @@
         facet = Material(value="Foo")
         run("Occurrences can override materials from their types", facet=facet, inst=element, expected=True)
 
 
 class TestPartOf:
     def test_creating_a_partof_facet(self):
         facet = PartOf()
-        assert facet.asdict() == {"@relation": "IfcRelAggregates"}
+        assert facet.asdict() == {"entity": {"name": {"simpleValue": "IFCWALL"}}}
         facet = PartOf(
             entity="IfcGroup",
             predefinedType="predefinedType",
-            relation="IfcRelAssignsToGroup",
+            relation="IFCRELASSIGNSTOGROUP",
             minOccurs="0",
             maxOccurs="unbounded",
             instructions="instructions",
         )
         assert facet.asdict() == {
             "entity": {
                 "name": {"simpleValue": "IfcGroup"},
                 "predefinedType": {"simpleValue": "predefinedType"},
             },
-            "@relation": "IfcRelAssignsToGroup",
+            "@relation": "IFCRELASSIGNSTOGROUP",
             "@minOccurs": "0",
             "@maxOccurs": "unbounded",
             "@instructions": "instructions",
         }
 
     def test_filtering_using_a_partof_facet(self):
         set_facet("partof")
 
         ifc = ifcopenshell.file()
 
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcElementAssembly")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
-        facet = PartOf(relation="IfcRelAggregates")
+        facet = PartOf(entity="IFCELEMENTASSEMBLY", relation="IFCRELAGGREGATES")
         run("A non aggregated element fails an aggregate relationship", facet=facet, inst=subelement, expected=False)
         ifcopenshell.api.run("aggregate.assign_object", ifc, product=subelement, relating_object=element)
         run("The aggregated whole fails an aggregate relationship", facet=facet, inst=element, expected=False)
         run("The aggregated part passes an aggregate relationship", facet=facet, inst=subelement, expected=True)
 
         run("A required facet checks all parameters as normal", facet=facet, inst=subelement, expected=True)
-        facet = PartOf(relation="IfcRelAggregates", minOccurs=0, maxOccurs=0)
+        facet = PartOf(entity="IFCELEMENTASSEMBLY", relation="IFCRELAGGREGATES", minOccurs=0, maxOccurs=0)
         run("A prohibited facet returns the opposite of a required facet", facet=facet, inst=subelement, expected=False)
-        facet = PartOf(relation="IfcRelAggregates", minOccurs=0)
+        facet = PartOf(entity="IFCELEMENTASSEMBLY", relation="IFCRELAGGREGATES", minOccurs=0)
         run("An optional facet always passes regardless of outcome 1/2", facet=facet, inst=element, expected=True)
         run("An optional facet always passes regardless of outcome 2/2", facet=facet, inst=subelement, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSlab")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcBeam")
         ifcopenshell.api.run("aggregate.assign_object", ifc, product=subelement, relating_object=element)
-        facet = PartOf(entity="IFCSLAB", relation="IfcRelAggregates")
+        facet = PartOf(entity="IFCSLAB", relation="IFCRELAGGREGATES")
         run("An aggregate may specify the entity of the whole 1/2", facet=facet, inst=subelement, expected=True)
-        facet = PartOf(entity="IFCWALL", relation="IfcRelAggregates")
+        facet = PartOf(entity="IFCWALL", relation="IFCRELAGGREGATES")
         run("An aggregate may specify the entity of the whole 2/2", facet=facet, inst=subelement, expected=False)
 
         element.PredefinedType = "BASESLAB"
-        facet = PartOf(entity="IFCSLAB", predefinedType="BASESLAB", relation="IfcRelAggregates")
+        facet = PartOf(entity="IFCSLAB", predefinedType="BASESLAB", relation="IFCRELAGGREGATES")
         run(
             "An aggregate may specify the predefined type of the whole 1/2", facet=facet, inst=subelement, expected=True
         )
-        facet = PartOf(entity="IFCSLAB", predefinedType="SLABRADOR", relation="IfcRelAggregates")
+        facet = PartOf(entity="IFCSLAB", predefinedType="SLABRADOR", relation="IFCRELAGGREGATES")
         run(
             "An aggregate may specify the predefined type of the whole 2/2",
             facet=facet,
             inst=subelement,
             expected=False,
         )
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcElementAssembly")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSlab")
         subsubelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcBeam")
         ifcopenshell.api.run("aggregate.assign_object", ifc, product=subelement, relating_object=element)
         ifcopenshell.api.run("aggregate.assign_object", ifc, product=subsubelement, relating_object=subelement)
-        facet = PartOf(entity="IFCELEMENTASSEMBLY", relation="IfcRelAggregates")
+        facet = PartOf(entity="IFCELEMENTASSEMBLY", relation="IFCRELAGGREGATES")
         run("An aggregate entity may pass any ancestral whole passes", facet=facet, inst=subsubelement, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcElementAssembly")
         group = ifcopenshell.api.run("group.add_group", ifc)
-        facet = PartOf(relation="IfcRelAssignsToGroup")
+        facet = PartOf(entity="IFCGROUP", relation="IFCRELASSIGNSTOGROUP")
         run("A non grouped element fails a group relationship", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("group.assign_group", ifc, products=[element], group=group)
         run("A grouped element passes a group relationship", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcElementAssembly")
         group = ifc.createIfcInventory()
-        facet = PartOf(entity="IFCGROUP", relation="IfcRelAssignsToGroup")
+        facet = PartOf(entity="IFCGROUP", relation="IFCRELASSIGNSTOGROUP")
         ifcopenshell.api.run("group.assign_group", ifc, products=[element], group=group)
         run("A group entity must match exactly 1/2", facet=facet, inst=element, expected=False)
-        facet = PartOf(entity="IFCINVENTORY", relation="IfcRelAssignsToGroup")
+        facet = PartOf(entity="IFCINVENTORY", relation="IFCRELASSIGNSTOGROUP")
         run("A group entity must match exactly 2/2", facet=facet, inst=element, expected=True)
 
         group.ObjectType = "BUNNY"
-        facet = PartOf(entity="IFCINVENTORY", predefinedType="BUNNARY", relation="IfcRelAssignsToGroup")
+        facet = PartOf(entity="IFCINVENTORY", predefinedType="BUNNARY", relation="IFCRELASSIGNSTOGROUP")
         run("A group predefined type must match exactly 2/2", facet=facet, inst=element, expected=False)
-        facet = PartOf(entity="IFCINVENTORY", predefinedType="BUNNY", relation="IfcRelAssignsToGroup")
+        facet = PartOf(entity="IFCINVENTORY", predefinedType="BUNNY", relation="IFCRELASSIGNSTOGROUP")
         run("A group predefined type must match exactly 2/2", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcElementAssembly")
         container = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSpace")
-        facet = PartOf(relation="IfcRelContainedInSpatialStructure")
+        facet = PartOf(entity="IFCSPACE", relation="IFCRELCONTAINEDINSPATIALSTRUCTURE")
         run("Any contained element passes a containment relationship 1/2", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("spatial.assign_container", ifc, product=element, relating_structure=container)
         run("Any contained element passes a containment relationship 2/2", facet=facet, inst=element, expected=True)
         run("The container itself always fails", facet=facet, inst=container, expected=False)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcElementAssembly")
         container = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSpace")
         ifcopenshell.api.run("spatial.assign_container", ifc, product=element, relating_structure=container)
-        facet = PartOf(relation="IfcRelContainedInSpatialStructure", entity="IFCSITE")
+        facet = PartOf(relation="IFCRELCONTAINEDINSPATIALSTRUCTURE", entity="IFCSITE")
         run("The container entity must match exactly 1/2", facet=facet, inst=element, expected=False)
-        facet = PartOf(relation="IfcRelContainedInSpatialStructure", entity="IFCSPACE")
+        facet = PartOf(relation="IFCRELCONTAINEDINSPATIALSTRUCTURE", entity="IFCSPACE")
         run("The container entity must match exactly 2/2", facet=facet, inst=element, expected=True)
 
         container.ObjectType = "BURROW"
-        facet = PartOf(relation="IfcRelContainedInSpatialStructure", entity="IFCSPACE", predefinedType="WARREN")
+        facet = PartOf(relation="IFCRELCONTAINEDINSPATIALSTRUCTURE", entity="IFCSPACE", predefinedType="WARREN")
         run("The container predefined type must match exactly 1/2", facet=facet, inst=element, expected=False)
-        facet = PartOf(relation="IfcRelContainedInSpatialStructure", entity="IFCSPACE", predefinedType="BURROW")
+        facet = PartOf(relation="IFCRELCONTAINEDINSPATIALSTRUCTURE", entity="IFCSPACE", predefinedType="BURROW")
         run("The container predefined type must match exactly 2/2", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSlab")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcBeam")
         ifcopenshell.api.run("aggregate.assign_object", ifc, product=subelement, relating_object=element)
         container = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSpace")
         ifcopenshell.api.run("spatial.assign_container", ifc, product=element, relating_structure=container)
-        facet = PartOf(relation="IfcRelContainedInSpatialStructure", entity="IFCSPACE")
+        facet = PartOf(relation="IFCRELCONTAINEDINSPATIALSTRUCTURE", entity="IFCSPACE")
         run("The container may be indirect", facet=facet, inst=subelement, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcFurniture")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcDiscreteAccessory")
         ifcopenshell.api.run("nest.assign_object", ifc, related_object=subelement, relating_object=element)
-        facet = PartOf(relation="IfcRelNests")
+        facet = PartOf(entity="IFCFURNITURE", relation="IFCRELNESTS")
         run("Any nested part passes a nest relationship", facet=facet, inst=subelement, expected=True)
         run("Any nested whole fails a nest relationship", facet=facet, inst=element, expected=False)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcFurniture")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcDiscreteAccessory")
         ifcopenshell.api.run("nest.assign_object", ifc, related_object=subelement, relating_object=element)
-        facet = PartOf(relation="IfcRelNests", entity="IFCBEAM")
+        facet = PartOf(relation="IFCRELNESTS", entity="IFCBEAM")
         run("The nest entity must match exactly 1/2", facet=facet, inst=subelement, expected=False)
-        facet = PartOf(relation="IfcRelNests", entity="IFCFURNITURE")
+        facet = PartOf(relation="IFCRELNESTS", entity="IFCFURNITURE")
         run("The nest entity must match exactly 2/2", facet=facet, inst=subelement, expected=True)
 
         element.PredefinedType = "USERDEFINED"
         element.ObjectType = "WATERBOTTLE"
-        facet = PartOf(relation="IfcRelNests", entity="IFCFURNITURE", predefinedType="LITTERBOX")
+        facet = PartOf(relation="IFCRELNESTS", entity="IFCFURNITURE", predefinedType="LITTERBOX")
         run("The nest predefined type must match exactly 1/2", facet=facet, inst=subelement, expected=False)
-        facet = PartOf(relation="IfcRelNests", entity="IFCFURNITURE", predefinedType="WATERBOTTLE")
+        facet = PartOf(relation="IFCRELNESTS", entity="IFCFURNITURE", predefinedType="WATERBOTTLE")
         run("The nest predefined type must match exactly 2/2", facet=facet, inst=subelement, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcFurniture")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcDiscreteAccessory")
         subsubelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcMechanicalFastener")
         ifcopenshell.api.run("nest.assign_object", ifc, related_object=subelement, relating_object=element)
         ifcopenshell.api.run("nest.assign_object", ifc, related_object=subsubelement, relating_object=subelement)
-        facet = PartOf(relation="IfcRelNests", entity="IFCFURNITURE")
+        facet = PartOf(relation="IFCRELNESTS", entity="IFCFURNITURE")
         run("Nesting may be indirect", facet=facet, inst=subsubelement, expected=True)
 
 
 class TestRestriction:
     def test_creating_a_restriction(self):
         restriction = Restriction(options={"enumeration": ["foo", "bar"]})
         assert restriction.asdict() == {"@base": "xs:string", "xs:enumeration": [{"@value": "foo"}, {"@value": "bar"}]}
```

### Comparing `ifctester-0.0.230618/test/test_ids.py` & `ifctester-0.0.230718/test/test_ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     def test_create_an_ids_with_minimal_information(self):
         specs = ids.Ids()
         assert specs.asdict() == {
             "@xmlns": "http://standards.buildingsmart.org/IDS",
             "@xmlns:xs": "http://www.w3.org/2001/XMLSchema",
             "@xmlns:xsi": "http://www.w3.org/2001/XMLSchema-instance",
-            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS/ids_05.xsd",
+            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS/ids_09.xsd",
             "info": {"title": "Untitled"},
             "specifications": {"specification": []},
         }
 
     def test_create_an_ids_with_all_possible_information(self):
         specs = ids.Ids(
             title="title",
@@ -68,15 +68,15 @@
             purpose="purpose",
             milestone="milestone",
         )
         assert specs.asdict() == {
             "@xmlns": "http://standards.buildingsmart.org/IDS",
             "@xmlns:xs": "http://www.w3.org/2001/XMLSchema",
             "@xmlns:xsi": "http://www.w3.org/2001/XMLSchema-instance",
-            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS/ids_05.xsd",
+            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS/ids_09.xsd",
             "info": {
                 "title": "title",
                 "copyright": "copyright",
                 "version": "version",
                 "description": "description",
                 "author": "author@test.com",
                 "date": "2020-01-01",
@@ -88,15 +88,15 @@
 
     def test_check_invalid_ids_information(self):
         specs = ids.Ids(title=None, author="author", date="9999-99-99")
         assert specs.asdict() == {
             "@xmlns": "http://standards.buildingsmart.org/IDS",
             "@xmlns:xs": "http://www.w3.org/2001/XMLSchema",
             "@xmlns:xsi": "http://www.w3.org/2001/XMLSchema-instance",
-            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS/ids_05.xsd",
+            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS/ids_09.xsd",
             "info": {"title": "Untitled"},
             "specifications": {"specification": []},
         }
 
     def test_authoring_an_ids_with_no_specifications_is_invalid(self):
         specs = ids.Ids()
         with pytest.raises(xmlschema.validators.exceptions.XMLSchemaChildrenValidationError):
```

