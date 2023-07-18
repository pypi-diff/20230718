# Comparing `tmp/neoteroi_mkdocs-1.0.2.tar.gz` & `tmp/neoteroi_mkdocs-1.0.3.tar.gz`

## Comparing `neoteroi_mkdocs-1.0.2.tar` & `neoteroi_mkdocs-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/py.typed
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/__init__.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/domain.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/py.typed
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/__init__.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/domain.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/git.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/py.typed
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/txt.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/__init__.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/align.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/images.py
--rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/processors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/py.typed
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/files.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/source.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/text.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/web.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/tables/__init__.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/tables/spantable.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/oad/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/oad/py.typed
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/__init__.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/domain.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/py.typed
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/timeutil.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/gantt/__init__.py
--rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/gantt/html.py
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/spantable/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/spantable/py.typed
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/__init__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/domain.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/py.typed
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/LICENSE
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/README.md
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/py.typed
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/domain.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/py.typed
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/__init__.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/domain.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/git.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/py.typed
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/txt.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/__init__.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/align.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/images.py
+-rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/processors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/py.typed
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/files.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/source.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/text.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/web.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/tables/__init__.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/tables/spantable.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/oad/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/oad/py.typed
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/__init__.py
+-rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/domain.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/py.typed
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/timeutil.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/gantt/__init__.py
+-rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/gantt/html.py
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/spantable/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/spantable/py.typed
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/domain.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/py.typed
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/README.md
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 neoteroi_mkdocs-1.0.3/PKG-INFO
```

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/__init__.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,14 +30,19 @@
                 item["image"] = Image.from_obj(item["image"])
 
     def build_html(self, parent, obj, props) -> None:
         """Builds the HTML for the given input object."""
         if not isinstance(obj, list):
             raise TypeError("Expected a list of items describing cards.")
 
+        if self.root_config:
+            new_props = dict(**self.root_config)
+            new_props.update(props)
+            props = new_props
+
         self.norm_obj(obj)
         builder = CardsHTMLBuilder(create_instance(CardsViewOptions, props))
         builder.build_html(parent, Cards(create_instances(CardItem, obj)))
 
 
 class CardsEmbeddedProcessor(BaseCardsProcessor, EmbeddedBlockProcessor):
     """
@@ -51,22 +56,32 @@
     Markdown (e.g. file, URL, database).
     """
 
 
 class CardsExtension(Extension):
     """Extension that includes cards."""
 
-    config = {
-        "priority": [12, "The priority to be configured for the extension."],
-    }
+    def __init__(self, *args, **kwargs):
+        self.config = {
+            "priority": [12, "The priority to be configured for the extension."],
+            "blank_target": [False, 'Whether to generate links with target="_blank"'],
+        }
+        super().__init__(*args, **kwargs)
 
     def extendMarkdown(self, md):
         md.registerExtension(self)
         priority = self.getConfig("priority")
 
+        configs = self.getConfigs()
+        del configs["priority"]
+
         md.parser.blockprocessors.register(
-            CardsEmbeddedProcessor(md.parser), "cards", priority + 0.1
+            CardsEmbeddedProcessor(md.parser).with_root_config(configs),
+            "cards",
+            priority + 0.1,
         )
 
         md.parser.blockprocessors.register(
-            CardsSourceProcessor(md.parser), "cards-from-source", priority
+            CardsSourceProcessor(md.parser).with_root_config(configs),
+            "cards-from-source",
+            priority,
         )
```

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/cards/html.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/cards/html.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
 import xml.etree.ElementTree as etree
 from dataclasses import dataclass
 
-from neoteroi.mkdocs.markdown.images import build_image_html
+from neoteroi.mkdocs.markdown.images import build_icon_html, build_image_html
 
 from .domain import CardItem, Cards
 
 logger = logging.getLogger("MARKDOWN")
 
 
 @dataclass
 class CardsViewOptions:
     id: str = ""
     class_name: str = ""
     cols: int = 3
     image_bg: bool = False
+    blank_target: bool = False
 
     def __post_init__(self):
         if isinstance(self.cols, str):
             self.cols = int(self.cols)
 
 
 class CardsHTMLBuilder:
@@ -40,35 +41,51 @@
     def _get_root_class(self):
         base_class = f"nt-cards nt-grid cols-{self.options.cols}"
 
         if self.options.class_name:
             return base_class + " " + self.options.class_name
         return base_class
 
+    def _get_link_properties(self, item: CardItem):
+        assert item.url is not None
+        props = {"href": item.url}
+
+        if self.options.blank_target:
+            props.update(target="_blank", rel="noopener")
+        return props
+
     def build_html(self, parent, cards: Cards):
         root_element = etree.SubElement(
             parent, "div", {"class": self._get_root_class()}
         )
 
         for item in cards.items:
             self.build_item_html(root_element, item)
 
     def build_item_html(self, parent, item: CardItem):
         item_element = etree.SubElement(parent, "div", self.get_item_props(item))
 
         if item.url:
-            first_child = etree.SubElement(item_element, "a", {"href": item.url})
+            first_child = etree.SubElement(
+                item_element, "a", self._get_link_properties(item)
+            )
         else:
             first_child = etree.SubElement(
                 item_element, "div", {"class": "nt-card-wrap"}
             )
 
         wrapper_element = etree.SubElement(first_child, "div", {})
 
-        self.build_image_html(wrapper_element, item)
+        if item.image:
+            self.build_image_html(wrapper_element, item)
+        elif item.icon:
+            build_icon_html(
+                etree.SubElement(wrapper_element, "div", {"class": "nt-card-icon"}),
+                item.icon,
+            )
 
         text_wrapper = etree.SubElement(
             wrapper_element, "div", {"class": "nt-card-content"}
         )
 
         title_element = etree.SubElement(text_wrapper, "p", {"class": "nt-card-title"})
         title_element.text = item.title
```

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/__init__.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/domain.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/domain.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/git.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/git.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/html.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/html.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/contribs/txt.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/contribs/txt.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/__init__.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/align.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/align.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/images.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/images.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/processors.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     while i <= index:
         block = items.pop(0)
         yield block + "\n"
         i += 1
 
 
 class BaseProcessor(ABC):
+    root_config: dict = {}
     parsers: Iterable[TextParser] = (YAMLParser(), JSONParser(), CSVParser())
 
     @property
     @abstractmethod
     def name(self) -> str:
         """Returns the name of the tag that will be handled by this processor."""
 
@@ -139,14 +140,18 @@
             else:
                 new_lines.append(line)
         if new_lines:
             blocks.insert(0, "\n".join(new_lines))
 
         return match
 
+    def with_root_config(self, props):
+        self.__dict__["root_config"] = props
+        return self
+
 
 class SourceBlockProcessor(BlockProcessor, BaseProcessor):
     """
     Base class for inline processors that read information from a file or URL source
     and handle it to create an HTML element, like:
 
     [timeline(./example.yaml)]
```

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/utils.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/utils.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/files.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/files.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/text.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/text.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/data/web.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/data/web.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/tables/__init__.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/markdown/tables/spantable.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/markdown/tables/spantable.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/oad/__init__.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/oad/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/domain.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/domain.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/timeutil.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/timeutil.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/gantt/__init__.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/gantt/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/projects/gantt/html.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/projects/gantt/html.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/spantable/__init__.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/spantable/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/__init__.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/__init__.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/neoteroi/mkdocs/timeline/html.py` & `neoteroi_mkdocs-1.0.3/neoteroi/mkdocs/timeline/html.py`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/LICENSE` & `neoteroi_mkdocs-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/README.md` & `neoteroi_mkdocs-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/pyproject.toml` & `neoteroi_mkdocs-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neoteroi_mkdocs-1.0.2/PKG-INFO` & `neoteroi_mkdocs-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neoteroi-mkdocs
-Version: 1.0.2
+Version: 1.0.3
 Summary: Plugins for MkDocs and Python Markdown
 Project-URL: Homepage, https://github.com/Neoteroi/mkdocs-plugins
 Project-URL: Bug Tracker, https://github.com/Neoteroi/mkdocs-plugins/issues
 Author-email: Roberto Prevato <roberto.prevato@gmail.com>
 License-File: LICENSE
 Keywords: Markdown,MkDocs,OpenAPI,Swagger,documentation,extensions,plugins
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neoteroi-mkdocs Version: 1.0.2 Summary: Plugins for
+Metadata-Version: 2.1 Name: neoteroi-mkdocs Version: 1.0.3 Summary: Plugins for
 MkDocs and Python Markdown Project-URL: Homepage, https://github.com/Neoteroi/
 mkdocs-plugins Project-URL: Bug Tracker, https://github.com/Neoteroi/mkdocs-
 plugins/issues Author-email: Roberto Prevato
 prevato@gmail.com> License-File: LICENSE Keywords:
 Markdown,MkDocs,OpenAPI,Swagger,documentation,extensions,plugins Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
```

