# Comparing `tmp/wikibasedataconnector-0.0.1.tar.gz` & `tmp/wikibasedataconnector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikibasedataconnector-0.0.1.tar", last modified: Mon Mar  6 20:43:24 2023, max compression
+gzip compressed data, was "wikibasedataconnector-0.0.2.tar", last modified: Tue Jul 18 14:52:32 2023, max compression
```

## Comparing `wikibasedataconnector-0.0.1.tar` & `wikibasedataconnector-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:43:24.176426 wikibasedataconnector-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-06 20:43:16.000000 wikibasedataconnector-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-06 20:43:24.176426 wikibasedataconnector-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-06 20:43:16.000000 wikibasedataconnector-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-06 20:43:16.000000 wikibasedataconnector-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 20:43:24.176426 wikibasedataconnector-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:43:24.172426 wikibasedataconnector-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:43:24.172426 wikibasedataconnector-0.0.1/src/wikibasedataconnector/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-06 20:43:16.000000 wikibasedataconnector-0.0.1/src/wikibasedataconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-03-06 20:43:16.000000 wikibasedataconnector-0.0.1/src/wikibasedataconnector/wikibasedataconnector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:43:24.172426 wikibasedataconnector-0.0.1/src/wikibasedataconnector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-06 20:43:24.000000 wikibasedataconnector-0.0.1/src/wikibasedataconnector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-06 20:43:24.000000 wikibasedataconnector-0.0.1/src/wikibasedataconnector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 20:43:24.000000 wikibasedataconnector-0.0.1/src/wikibasedataconnector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-06 20:43:24.000000 wikibasedataconnector-0.0.1/src/wikibasedataconnector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-06 20:43:24.000000 wikibasedataconnector-0.0.1/src/wikibasedataconnector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:52:32.855184 wikibasedataconnector-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 14:52:24.000000 wikibasedataconnector-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-18 14:52:32.855184 wikibasedataconnector-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-18 14:52:24.000000 wikibasedataconnector-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-18 14:52:24.000000 wikibasedataconnector-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:52:32.855184 wikibasedataconnector-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:52:32.855184 wikibasedataconnector-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:52:32.855184 wikibasedataconnector-0.0.2/src/wikibasedataconnector/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 14:52:24.000000 wikibasedataconnector-0.0.2/src/wikibasedataconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16990 2023-07-18 14:52:24.000000 wikibasedataconnector-0.0.2/src/wikibasedataconnector/wikibasedataconnector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:52:32.855184 wikibasedataconnector-0.0.2/src/wikibasedataconnector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-18 14:52:32.000000 wikibasedataconnector-0.0.2/src/wikibasedataconnector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-18 14:52:32.000000 wikibasedataconnector-0.0.2/src/wikibasedataconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:52:32.000000 wikibasedataconnector-0.0.2/src/wikibasedataconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-18 14:52:32.000000 wikibasedataconnector-0.0.2/src/wikibasedataconnector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 14:52:32.000000 wikibasedataconnector-0.0.2/src/wikibasedataconnector.egg-info/top_level.txt
```

### Comparing `wikibasedataconnector-0.0.1/LICENSE` & `wikibasedataconnector-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wikibasedataconnector-0.0.1/pyproject.toml` & `wikibasedataconnector-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wikibasedataconnector"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Xentity Corporation", email="contact@xentity.com" },
 ]
 description = "Library used for mapping data easily into Wikibase Systems"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `wikibasedataconnector-0.0.1/src/wikibasedataconnector/wikibasedataconnector.py` & `wikibasedataconnector-0.0.2/src/wikibasedataconnector/wikibasedataconnector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """wikibot for the GeoScience Knowledgebase
 """
 import json
 from typing import Optional, Union
-import requests
+
 import pywikibot as pwb
+import requests
+
 
 class WBDC:
     """
     Constructor and functions
     """
     def __init__(self, site: str) -> None:
         self.site = pwb.Site('en', site)
         self.repo = self.site.data_repository()
         self.mapping_conf = None
         self.config = None
         self.page = None
         self.sparql_endpoint = None
         self.site.login()
 
-    def __add_item(self, page_info: dict, row: list) -> str:
+    def __add_item(self, page_info: dict, row: list, summary) -> str:
         """Generate new Item in GSKB
 
         Args:
             item (dict): minimal values needed to create item
 
         Returns:
             str: Item id generated
@@ -53,24 +55,25 @@
         }
         # params found at https://www.wikidata.org/w/api.php?action=help&modules=wbeditentity
         params = {
             'action': 'wbeditentity',
             'new': 'item',
             'data': json.dumps(data),
             'token': self.site.tokens['csrf'],
+            'summary': summary
         }
         try:
             req = self.site.simple_request(**params)
             results = req.submit()
             return results['entity']['id'] if 'id' in results['entity'] else None
         except Exception as exc:
             print(f'Failed to insert item {label}')
             print(exc)
 
-    def __add_prop(self, page_info: dict, row:list) -> Optional[str]:
+    def __add_prop(self, page_info: dict, row:list, summary) -> Optional[str]:
         """Generate new property in GSKB
 
         Args:
             prop (dict): minimal values needed to create property
 
         Returns:
             Optional[str]: property id generated
@@ -106,43 +109,43 @@
                 }
 
         # params found at https://www.wikidata.org/w/api.php?action=help&modules=wbeditentity
         params = {
             'action': 'wbeditentity',
             'new': 'property',
             'data': json.dumps(data),
-            'summary': 'bot adding in properties',
+            'summary': summary,
             'token': self.site.tokens['csrf']
         }
         try:
             req = self.site.simple_request(**params)
             results = req.submit()
             print(results)
             return results['entity']['id'] if 'id' in results['entity'] else None
         except Exception as exc:
             print(f'Failed to insert property {label}')
             print(exc)
 
-    def __add_source(self, claim: pwb.Claim, ref: dict, row: list) -> None:
+    def __add_source(self, claim: pwb.Claim, ref: dict, row: list, summary: str) -> None:
         """Add sources to claims on item
 
         Args:
             claim (pwb.Claim): Claim that the source is being added to
             ref (dict): References from conf file
             row (list): Data from file being read
         """
         prop_value = ref['config']['value']
         if ref['idx'] == -1:
             source = pwb.Claim(self.repo, prop_value)
             source.setTarget(ref['value'])
-            claim.addSource(source)
+            claim.addSource(source, summary=summary)
         else:
             source = pwb.Claim(self.repo, prop_value)
             source.setTarget(row[ref['idx']])
-            claim.addSource(source)
+            claim.addSource(source, summary=summary)
 
     def __create_page(self, page_id) -> Union[pwb.PropertyPage, pwb.ItemPage]:
         """
         creates either an item page or property page
         """
         if page_id is None:
             raise ValueError('There is no page id')
@@ -213,42 +216,43 @@
     async def process(self, row: list) -> None:
         """Process using mapping provided in the conf file
         """
         if 'mapping' not in self.mapping_conf:
             raise ValueError('Mapping is required')
         src = self.mapping_conf['source']
         page_info = self.mapping_conf['mapping']
+        summary = src['summary']
         if src['type'] == 'property':
             label = row[src['upsert']['idx']]
             prop_id = self.__search_item_id(label, src['type'])
             if prop_id is None:
-                prop_id = self.__add_prop(page_info, row)
+                prop_id = self.__add_prop(page_info, row, summary)
             self.__create_page(prop_id)
         elif src['upsert']['matchType'] == 'id':
             unique_id = row[src['upsert']['idx']]
             item_id = self.__get_item_id(unique_id)
             self.__create_page(item_id)
         else:
             label = row[src['upsert']['idx']]
             item_id = self.__search_item_id(label, src['type'])
             if item_id is None:
-                item_id = self.__add_item(page_info, row)
+                item_id = self.__add_item(page_info, row, summary)
             self.__create_page(item_id)
         for opt in page_info:
             if opt['type'] == 'label':
                 label = row[opt['idx']]
-                self.__upsert_label(label)
+                self.__upsert_label(label, summary)
             elif opt['type'] == 'description':
                 description = opt['config']['value'] if 'config' in opt else row[opt['idx']]
-                self.__upsert_description(description)
+                self.__upsert_description(description, summary)
             elif opt['type'] == 'aliases':
                 aliases = row[opt['idx']].split(', ') if row[opt['idx']]  != '' else []
-                self.__upsert_aliases(aliases)
+                self.__upsert_aliases(aliases, summary)
             elif opt['type'] == 'claim':
-                self.__upsert_claim(opt, row)
+                self.__upsert_claim(opt, row, summary)
 
     def __search_item_id(self, search_term: str, item_type: str) -> Optional[str]:
         """Makes an API call to find id within the GSKB
 
         Args:
             item (dict): item attributes in key/value pairs
 
@@ -281,111 +285,111 @@
         """Adds the mapping configuration
 
         Args:
             mapping (dict): Loaded JSON mapping
         """
         self.mapping_conf = mapping
 
-    def __set_claim_options(self, claim: pwb.Claim, target: dict, row: list, refs: dict) -> None:
+    def __set_claim_options(self, claim: pwb.Claim, target: dict, row: list, refs: dict, summary: str) -> None:
         """Add the target and qualifiers to the claim
 
         Args:
             claim (pwb.Claim): Claim of interest
             target (dict): Target from claim specified in conf
             row (list): Data from file being read
             refs (dict): References from conf
         """
         claim._type = target['type'] # pylint: disable=protected-access
         determined_target = self.__determine_target(target, row)
         claim.setTarget(determined_target)
-        self.__upsert_references(claim, refs, row)
+        self.__upsert_references(claim, refs, row, summary)
         for qualifier in target['qualifiers']:
-            self.__upsert_qualifier(claim, qualifier, row)
+            self.__upsert_qualifier(claim, qualifier, row, summary)
 
-    def __update_link(self, claim: pwb.Claim, ref: dict, row: list) -> None:
+    def __update_link(self, claim: pwb.Claim, ref: dict, row: list, summary: str) -> None:
         """Updates the url in claim if considered different
 
         Args:
             claim (pwb.Claim): Source Claim
             ref (dict): Reference to external urls
         """
         for i, _ in enumerate(claim.sources):
             ref_value = ref['config']['value']
             if ref_value in claim.sources[i]:
                 claim.removeSource(claim.sources[i][ref_value][0])
-                self.__add_source(claim, ref, row)
+                self.__add_source(claim, ref, row, summary)
 
-    def __upsert_claim(self, claim_dict: dict, row: list) -> None:
+    def __upsert_claim(self, claim_dict: dict, row: list, summary: str) -> None:
         """Inserts/Updates claims within page
 
         Args:
             claim_dict (dict): Structure of claim
         """
         claim_value = claim_dict['config']['value']
         claims = self.page.get()['claims']
         refs = self.mapping_conf['reference']
         # if claim value not found in claims at all
         if claim_value not in claims:
             for target in claim_dict['targets']:
                 claim = pwb.Claim(self.repo, claim_value)
-                self.__set_claim_options(claim, target, row, refs)
-                self.page.addClaim(claim, summary='Adding claim')
+                self.__set_claim_options(claim, target, row, refs, summary)
+                self.page.addClaim(claim, summary=summary)
         # if claim value found, but target not found
         else:
             for target in claim_dict['targets']:
                 match_found = False
                 # get target to make sure there is always one for comparison
                 determined_target = self.__determine_target(target, row)
                 for claim in claims[claim_value]:
                     if claim.target_equals(determined_target):
-                        self.__upsert_references(claim, refs, row)
+                        self.__upsert_references(claim, refs, row, summary)
                         for qualifier in target['qualifiers']:
-                            self.__upsert_qualifier(claim, qualifier, row)
+                            self.__upsert_qualifier(claim, qualifier, row, summary)
                         match_found = True
                 if not match_found:
                     new_claim = pwb.Claim(self.repo, claim_value)
-                    self.__set_claim_options(new_claim, target, row, refs)
-                    self.page.addClaim(new_claim, summary='Adding claim')
+                    self.__set_claim_options(new_claim, target, row, refs, summary)
+                    self.page.addClaim(new_claim, summary=summary)
 
-    def __upsert_aliases(self, aliases: str) -> None:
+    def __upsert_aliases(self, aliases: str, summary: str) -> None:
         """Adds or updates a label
 
         Args:
             label (str): Name of item
         """
         page_dict = self.page.get()
         same_aliases = (
         'en' in page_dict['aliases'] 
         and len(page_dict['aliases']['en']) == len(aliases)
         and set(page_dict['aliases']['en']) == set(aliases)
         )
         if not same_aliases:
-            self.page.editAliases({'en': aliases }, summary="Setting aliases")
+            self.page.editAliases({'en': aliases }, summary=summary)
 
-    def __upsert_description(self, desc: str) -> None:
+    def __upsert_description(self, desc: str, summary: str) -> None:
         """Adds or updates a description
 
         Args:
             desc (str): description of item
         """
         page_dict = self.page.get()
         if desc != page_dict['labels']['en']:
-            self.page.editDescriptions({'en': desc }, summary="Setting description")
+            self.page.editDescriptions({'en': desc }, summary=summary)
 
-    def __upsert_label(self, label: str) -> None:
+    def __upsert_label(self, label: str, summary: str) -> None:
         """Adds or updates a label
 
         Args:
             label (str): Name of item
         """
         page_dict = self.page.get()
         if label != page_dict['labels']['en']:
-            self.page.editLabels({'en': label }, summary="Setting label")
+            self.page.editLabels({'en': label }, summary=summary)
 
-    def __upsert_references(self, claim: pwb.Claim, refs: list, row: list) -> None:
+    def __upsert_references(self, claim: pwb.Claim, refs: list, row: list, summary: str) -> None:
         """Inserts/updates references into Claim
 
         Args:
             claim (pwb.Claim): Claim that the reference is being attached to
             refs (list): References provided by the conf file
             claim_dict (dict): Claim object provided by the conf file
             row (list): Data from file being read
@@ -394,36 +398,36 @@
             { key : value[0] for x in claim.sources for (key, value) in x.items() }
                 if isinstance(claim.sources, list)
                 else dict(claim.sources)
             )
         for ref in refs:
             value = ref['value'] if ref['idx'] == -1 else row[ref['idx']]
             if ref['config']['value'] not in sources:
-                self.__add_source(claim, ref, row)
+                self.__add_source(claim, ref, row, summary)
             if (ref['config']['value'] in sources
                 and value != sources[ref['config']['value']].target):
-                self.__update_link(claim, ref, row)
+                self.__update_link(claim, ref, row, summary)
 
-    def __upsert_qualifier(self, claim: pwb.Claim, qualifier_dict: dict, row: list) -> None:
-        """_summary_
+    def __upsert_qualifier(self, claim: pwb.Claim, qualifier_dict: dict, row: list, summary) -> None:
+        """Inserts/updates qualifier into Claim
 
         Args:
             claim (pwb.Claim): Claim that the qualifier is being added on to
             qualifier_dict (dict): qualifier found within claim object provided by the conf file
             row (list): Data from file being read
         """
         qual_claim = qualifier_dict['property']
         qualifier = pwb.Claim(self.repo, qual_claim)
         qualifier._type = qualifier_dict['type']# pylint: disable=protected-access
         target = self.__determine_target(qualifier_dict, row)
         qualifier.setTarget(target)
         if (qual_claim in claim.qualifiers
              and not claim.qualifiers[qual_claim][0].target_equals(target)):
             claim.removeQualifier(claim.qualifiers[qual_claim][0])
-            claim.addQualifier(qualifier, summary='Adding a qualifier')
+            claim.addQualifier(qualifier, summary=summary)
         elif not claim.has_qualifier(qual_claim, target):
-            claim.addQualifier(qualifier, summary='Adding a qualifier')
+            claim.addQualifier(qualifier, summary=summary)
 
 def wait(self, seconds): # pylint: disable=unused-argument
     """Override to remove default throttle of 5 secs
     """
 pwb.throttle.Throttle.wait = wait
```

