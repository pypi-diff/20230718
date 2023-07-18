# Comparing `tmp/neointerface-3.1.9.tar.gz` & `tmp/neointerface-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neointerface-3.1.9.tar", last modified: Wed Dec 21 12:13:04 2022, max compression
+gzip compressed data, was "neointerface-3.3.1.tar", last modified: Tue Jul 18 11:02:48 2023, max compression
```

## Comparing `neointerface-3.1.9.tar` & `neointerface-3.3.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2022-12-21 12:13:04.307520 neointerface-3.1.9/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11346 2022-12-21 07:38:31.000000 neointerface-3.1.9/LICENSE
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11855 2022-12-21 12:13:04.307520 neointerface-3.1.9/PKG-INFO
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    41771 2022-12-21 12:06:58.000000 neointerface-3.1.9/README.md
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2022-12-21 12:13:04.307520 neointerface-3.1.9/neointerface/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       51 2022-12-21 07:38:31.000000 neointerface-3.1.9/neointerface/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)   110646 2022-12-21 07:38:31.000000 neointerface-3.1.9/neointerface/neointerface.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2022-12-21 12:13:04.307520 neointerface-3.1.9/neointerface.egg-info/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11855 2022-12-21 12:13:04.000000 neointerface-3.1.9/neointerface.egg-info/PKG-INFO
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      274 2022-12-21 12:13:04.000000 neointerface-3.1.9/neointerface.egg-info/SOURCES.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        1 2022-12-21 12:13:04.000000 neointerface-3.1.9/neointerface.egg-info/dependency_links.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      325 2022-12-21 12:13:04.000000 neointerface-3.1.9/neointerface.egg-info/requires.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       13 2022-12-21 12:13:04.000000 neointerface-3.1.9/neointerface.egg-info/top_level.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      103 2022-12-21 07:38:31.000000 neointerface-3.1.9/pyproject.toml
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       38 2022-12-21 12:13:04.307520 neointerface-3.1.9/setup.cfg
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     2105 2022-12-21 12:12:56.000000 neointerface-3.1.9/setup.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:02:48.683385 neointerface-3.3.1/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11346 2023-07-18 11:00:29.000000 neointerface-3.3.1/LICENSE
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11821 2023-07-18 11:02:48.683385 neointerface-3.3.1/PKG-INFO
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    43584 2023-07-18 11:00:29.000000 neointerface-3.3.1/README.md
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:02:48.683385 neointerface-3.3.1/logger/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:00:29.000000 neointerface-3.3.1/logger/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1227 2023-07-18 11:00:29.000000 neointerface-3.3.1/logger/logger.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:02:48.683385 neointerface-3.3.1/neointerface/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       51 2023-07-18 11:00:29.000000 neointerface-3.3.1/neointerface/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)   112072 2023-07-18 11:00:29.000000 neointerface-3.3.1/neointerface/neointerface.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:02:48.683385 neointerface-3.3.1/neointerface.egg-info/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11821 2023-07-18 11:02:48.000000 neointerface-3.3.1/neointerface.egg-info/PKG-INFO
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      310 2023-07-18 11:02:48.000000 neointerface-3.3.1/neointerface.egg-info/SOURCES.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        1 2023-07-18 11:02:48.000000 neointerface-3.3.1/neointerface.egg-info/dependency_links.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      325 2023-07-18 11:02:48.000000 neointerface-3.3.1/neointerface.egg-info/requires.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       20 2023-07-18 11:02:48.000000 neointerface-3.3.1/neointerface.egg-info/top_level.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      103 2023-07-18 11:00:29.000000 neointerface-3.3.1/pyproject.toml
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       38 2023-07-18 11:02:48.683385 neointerface-3.3.1/setup.cfg
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1996 2023-07-18 11:00:54.000000 neointerface-3.3.1/setup.py
```

### Comparing `neointerface-3.1.9/LICENSE` & `neointerface-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neointerface-3.1.9/PKG-INFO` & `neointerface-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neointerface
-Version: 3.1.9
+Version: 3.3.1
 Summary: A Python interface to use the Neo4j graph database
 Home-page: UNKNOWN
 Author: Alexey Kuznetsov, Julian West, Ben Grinsted, William McDermott
 License: 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
@@ -203,13 +203,13 @@
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
-Description: https://github.com/GSK-Biostatistics/neointerface#neointerface---neo4j-made-easy-for-python-programmers
+Description: https://github.com/GSK-Biostatistics/neointerface/blob/main/README.md
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `neointerface-3.1.9/README.md` & `neointerface-3.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 # them for common operations
 
 # EXAMPLE: find all the patients of a doctor named 'Hippocrates'
 cypher = "MATCH (p :patient)-[IS_TREATED_BY]->(d :doctor {name:'Hippocrates'}) RETURN p"
 result = db.query(cypher)
 print(result)   # SHOWS:  [{'p': {'gender': 'M', 'patient_id': 123}}]
 ```
-The database constructed so far, as seen in the Neo4j browser:
+The database constructed so far, as seen in the Neo4j [browser](https://browser.neo4j.io/):
 ![The database constructed so far, as seen in the Neo4j browser](docs/Example_database.png)
 
 ## From Pandas dataframe to Neo4j and back
 Let's say that you have a Pandas dataframe such as:
 ```python
 import pandas as pd
 df_original = pd.DataFrame({"patient_id": [100, 200], "name": ["Jack", "Jill"]})
@@ -106,15 +106,26 @@
 > 
 >**NODE 2**, with properties "patient_id"=200 and "name"="Jill"
 
 If you want them back as a dataframe, just do:
 ```python
 df_new = db.get_df("my_label")
 ```
+## From dictionary to Neo4j
+If you have a dictionary, for example:
+```python
+dictionary = {"class": "Dataset", "name": "DM", "Column": [{"name": "USUBJID"}, {"name": "DMDTC", "type": "datetime"}]}
+```
+Load it into the Neo4j database simply with:
+```python
+db.load_dict(dictionary, label="Dataset")
+```
+where *db* is the instantiated NeoInterface class from the earlier example, and label is the label to assign to the root node.
 
+![image](docs/load_dict.png)
 
 
 # Instantiating the Class
 
 
 
 ## NeoInterface()
@@ -133,14 +144,19 @@
     :param debug:       Flag indicating whether a debug mode is to be used by all methods of this class
     :param autoconnect  Flag indicating whether the class should establish connection to database at initialization
 
 
 
 --- 
 
+# Mini-UI
+A mini user interface over some of the NeoInterface functionality is included in this repository. Simply set you environment variables to connect to Neo4j(NEO4J_HOST, NEO4J_USER and NEO4J_PASSWORD) and run 
+```source app.sh```
+on Unix.
+
 
 # GENERAL METHODS
 
 
 
 ## version()
 name | arguments| return
@@ -222,14 +238,16 @@
 
 
 ## query_expanded()
 name | arguments| return
 -----| ---------| -------
 *query_expanded*| q: str, params = None, flatten = False| []
 
+**NOTE: This procedure will be deprecated, use query(... return_type: str = 'neo4j.Result') instead**
+
     Expanded version of query(), meant to extract additional info for queries that return Graph Data Types,
     i.e. nodes, relationships or paths,
     such as "MATCH (n) RETURN n", or "MATCH (n1)-[r]->(n2) RETURN r"
 
     For example, if nodes were returned, and their Neo4j internal IDs and/or labels are desired
     (in addition to all the properties and their values)
 
@@ -645,14 +663,39 @@
     :param drop_constraints:Flag indicating whether to also ditch all constraints (by default, True)
     :return:                None
 
 
 
 ---
 
+
+## set_fields()
+name | arguments| return
+-----| ---------| -------
+*set_fields*| labels, set_dict, properties_condition=None, cypher_clause=None, cypher_dict=None| None
+
+    EXAMPLE - locate the "car" with vehicle id 123 and set its color to white and price to 7000
+            set_fields(labels = "car", set_dict = {"color": "white", "price": 7000},
+                       properties_condition = {"vehicle id": 123})
+
+        LIMITATION: blanks are allowed in the keys of properties_condition, but not in those of set_dict
+
+        :param labels:                  A string, or list/tuple of strings, representing Neo4j labels
+        :param set_dict:                A dictionary of field name/values to create/update the node's attributes
+                                            (note: no blanks are allowed in the keys)
+        :param properties_condition:
+        :param cypher_clause:
+        :param cypher_dict:
+        :return:                        None
+
+
+
+---
+
+
 ## extract_entities()
 name | arguments| return
 -----| ---------| -------
 *extract_entities*| mode='merge', label=None, cypher=None, cypher_dict=None, target_label=None, property_mapping={}, relationship=None, direction=None| None
                          
     Create new nodes using data from other nodes
```

### Comparing `neointerface-3.1.9/neointerface/neointerface.py` & `neointerface-3.3.1/neointerface/neointerface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from neo4j import GraphDatabase  # The Neo4j python connectivity library "Neo4j Python Driver"
 from neo4j import __version__ as neo4j_driver_version  # The version of the Neo4j driver being used
 import neo4j.graph  # To check returned data types
 from neo4j.time import DateTime, Date  # to convert neo4j.time.DateTime's to python datetimes (and Dates)
 import numpy as np
 import pandas as pd
-import inspect
 import os
 import requests
 import re
 import json
 import time
 import collections
+import logging
 from urllib.parse import quote
-from typing import Union
+from typing import Union, List
 from warnings import warn
 from networkx import MultiDiGraph
 from neo4j.graph import Node, Relationship, Path
+from logger.logger import logger
 
 
 class NeoInterface:
     """
     High level class to interact with neo4j from Python.
     It provides a higher-level wrapper around the Neo4j python connectivity library "Neo4j Python Driver",
     documented at: https://neo4j.com/docs/api/python-driver/current/api.html
@@ -56,28 +57,31 @@
         If unable to create a Neo4j driver object, raise an Exception reminding the user to check whether the Neo4j database is running
 
         :param host:        URL to connect to database with.  DEFAULT: read from NEO4J_HOST environmental variable
         :param credentials: Pair of strings (tuple or list) containing, respectively, the database username and password
                             DEFAULT: read from NEO4J_USER and NEO4J_PASSWORD environmental variables
                             if None then no authentication is used
         :param apoc:        Flag indicating whether apoc library is used on Neo4j database to connect to
-        :param verbose:     Flag indicating whether a verbose mode is to be used by all methods of this class
-        :param debug:       Flag indicating whether a debug mode is to be used by all methods of this class
+        :param verbose:     Flag indicating whether ANY logs will be displayed
+        :param debug:       Flag indicating whether logs will be in debug or info mode
         :param autoconnect  Flag indicating whether the class should establish connection to database at initialization
         """
         self.verbose = verbose
-        self.debug = debug
         self.autoconnect = autoconnect
         self.host = host
         self.credentials = credentials
         self.apoc = apoc
         self.rdf = rdf
         self.rdf_host = rdf_host
         if self.verbose:
-            print("---------------- Initializing NeoInterface -------------------")
+            logger.info("\t\tInitializing NeoInterface")
+            if debug:
+                logging.getLogger('neointerface').setLevel(logging.DEBUG)
+            else:
+                logging.getLogger('neointerface').setLevel(logging.INFO)
         if self.autoconnect:  # TODO: add test for autoconnect == False
             # Attempt to create a driver object
             self.connect()
 
             # Extra initializations if APOC custom procedures (note: APOC must also be enabled on the database)
             # if apoc:
             # self.setup_all_apoc_custom()
@@ -98,44 +102,44 @@
         except Exception as ex:
             error_msg = f"CHECK IF NEO4J IS RUNNING! While instantiating the NeoInterface object, failed to create the driver: {ex}"
             raise Exception(error_msg)
         else:
             self.test_connection()
 
         if self.verbose:
-            print(f"Connection to {self.host} established")
+            logger.info(f"Connection to {self.host} established")
 
     def test_connection(self):
         try:
             self.query("RETURN 10")
         except Exception as ex:
             error_msg = f"Connection to {self.host} was unsuccessful! Check if NEO4J is running and/or that your credentials are correct."
             raise Exception(error_msg)
 
     def rdf_config(self) -> None:
         try:
             self.query("CALL n10s.graphconfig.init({handleVocabUris:'IGNORE'});")
         except:
-            if self.debug:
-                print("Config already created, make sure the config is correct")
+            if self.verbose:
+                logger.debug("Config already created, make sure the config is correct")
         self.create_constraint(label="Resource", key="uri", type="UNIQUE", name="n10s_unique_uri")
 
     def rdf_setup_connection(self) -> None:
         self.rdf_config()
         if not self.rdf_host:
             self.rdf_host = os.environ.get("NEO4J_RDF_HOST")
         if not self.rdf_host:
             bolt_port = re.findall(r'\:\d+', self.host)[0]
-            self.rdf_host = self.host.replace(bolt_port, ":7474").replace("bolt", "http").replace("neoj", "http")
+            self.rdf_host = self.host.replace(bolt_port, ":7474").replace("bolt", "http").replace("neo4j", "http")
             self.rdf_host += ("" if self.rdf_host.endswith("/") else "/") + "rdf/"
         try:
             get_response = json.loads(requests.get(f"{self.rdf_host}ping", auth=self.credentials).text)
             if self.verbose:
                 if "here!" in get_response.values():
-                    print(f"Connection to {self.rdf_host} established")
+                    logger.info(f"Connection to {self.rdf_host} established")
         except:
             error_msg = f"CHECK IF RDF ENDPOINT IS SET UP CORRECTLY! While instantiating the NeoInterface object, failed to connect to {self.rdf_host}"
             raise Exception(error_msg)
 
     def version(self) -> str:
         # Return the version of the Neo4j driver being used.  EXAMPLE: "4.2.1"
         return neo4j_driver_version
@@ -152,15 +156,15 @@
     ############################################################################################
     #                                                                                          #
     #                           METHODS TO RUN GENERIC QUERIES                                 #
     #                                                                                          #
     ############################################################################################
 
     def query(self, q: str, params=None, return_type: str = 'data', convert_dates: bool = True) -> Union[
-        list, neo4j.Result, pd.DataFrame, MultiDiGraph]:
+              list, neo4j.Result, pd.DataFrame, MultiDiGraph]:
         """
         Runs a general Cypher query
         :param q:       A Cypher query
         :param params:  An optional Cypher dictionary
                         EXAMPLE, assuming that the cypher string contains the substrings "$node_id":
                                 {'node_id': 20}
         :param return_type: type of the returned result 'data'/'neo4j.Result'/'pd'/'nx'
@@ -224,15 +228,15 @@
                 flattened_dictionaries = []
                 for r in result_data:
                     flattened_dictionaries.append(self.flatten(r))  # pd.json_normalise() might be a better choice
                 return pd.DataFrame(flattened_dictionaries)
             elif return_type == 'nx':
                 return self.nx_graph_from_cypher(result)
 
-    def query_expanded(self, q: str, params=None, flatten=False) -> []:
+    def query_expanded(self, q: str, params=None, flatten=False) -> list:
         """
         Expanded version of query(), meant to extract additional info for queries that return Graph Data Types,
         i.e. nodes, relationships or paths,
         such as "MATCH (n) RETURN n", or "MATCH (n1)-[r]->(n2) RETURN r"
 
         For example, if nodes were returned, and their Neo4j internal IDs and/or labels are desired
         (in addition to all the properties and their values)
@@ -331,16 +335,16 @@
 
             return data_as_list
 
     @staticmethod
     def nx_graph_from_cypher(data):
         """Constructs a networkx graph from the results of a neo4j cypher query.
         Example of use:
-        >>> result = session.run(query)
-        >>> G = nx_graph_from_cypher(result.data())
+        / >>> result = session.run(query)
+        / >>> G = nx_graph_from_cypher(result.data())
 
         Nodes have fields 'labels' (frozenset) and 'properties' (dicts). Node IDs correspond to the neo4j graph.
         Edges have fields 'type_' (string) denoting the type of relation, and 'properties' (dict)."""
 
         G = MultiDiGraph()
 
         def add_node(node):
@@ -434,28 +438,32 @@
 
         EXAMPLES: fetch_single_field("car", "price", properties_condition={"car_make": "Toyota"})
                         will RETURN a list of prices of all the Toyota models
                   fetch_single_field("car", "price", properties_condition={"car_make": "Toyota"}, clause="n.price < 50000")
                         will RETURN a list of prices of all the Toyota models that cost less than 50000
 
         :param field_name:  A string with the name of the desired field (attribute)
+        :param labels: see get_nodes()
+        :param properties_condition: get_nodes()
+        :param cypher_clause: see get_nodes()
+        :param cypher_dict:  see get_nodes()
 
         For more information on the other parameters, see get_nodes()
 
         :return:  A list of the values of the field_name attribute in the nodes that match the specified conditions
         """
 
         record_list = self.get_nodes(labels, properties_condition=properties_condition,
                                      cypher_clause=cypher_clause, cypher_dict=cypher_dict)
         single_field_list = [record.get(field_name) for record in record_list]
 
         return single_field_list
 
     def get_nodes(self, labels="", properties_condition=None, cypher_clause=None, cypher_dict=None,
-                  return_nodeid=False, return_labels=False) -> [{}]:
+                  return_nodeid=False, return_labels=False) -> List[dict]:
         """
         EXAMPLES:
             get_nodes("")       # Get ALL nodes
             get_nodes("client")
             get_nodes("client", properties_condition = {"gender": "M", "ethnicity": "white"})
             get_nodes("client", cypher_clause = "n.age > 40 OR n.income < 50000")
             get_nodes("client", cypher_clause = "n.age > $some_age", cypher_dict = {"$some_age": 40})
@@ -503,16 +511,16 @@
                             ]
         # TODO: provide an option to specify the desired fields
         """
         (cypher, cypher_dict) = self._match_nodes(labels=labels, properties_condition=properties_condition,
                                                   cypher_clause=cypher_clause, cypher_dict=cypher_dict)
         cypher += " RETURN n"
 
-        if self.debug:
-            print(f"""
+        if self.verbose:
+            logger.debug(f"""
             In get_nodes().
             query: {cypher}
             parameters: {cypher_dict}
             """)
 
         result_list = self.query_expanded(cypher, cypher_dict, flatten=True)
         if return_nodeid and return_labels:
@@ -621,15 +629,15 @@
 
         # Construct the Cypher string
         cypher = f"MATCH (n {cypher_labels} {clause_from_properties})"
 
         if (cypher_clause != "") and (cypher_clause is not None):
             cypher += f" WHERE {cypher_clause}"
 
-        return (cypher, cypher_dict)
+        return cypher, cypher_dict
 
     def _prepare_labels(self, labels) -> str:
         """
         Turn the given string, or list/tuple of strings - representing Neo4j labels - into a string
         suitable for inclusion in a Cypher query.
         Blanks ARE allowed in names.
         EXAMPLES:
@@ -649,69 +657,69 @@
 
         cypher_labels = ""
         for single_label in labels:
             cypher_labels += f":`{single_label}`"  # EXAMPLE: ":`label 1`:`label 2`"
 
         return cypher_labels
 
-    def get_parents_and_children(self, node_id: int) -> {}:
+    def get_parents_and_children(self, node_id: int) -> dict:
         """
         Fetch all the nodes connected to the given one by INbound relationships to it (its "parents"),
         as well as by OUTbound relationships to it (its "children")
 
         :param node_id: An integer with a Neo4j internal node ID
         :return:        A dictionary with 2 keys: 'parent_list' and 'child_list'
                         The values are lists of dictionaries with 3 keys: "id", "label", "rel"
                             EXAMPLE of individual items in either parent_list or child_list:
                             {'id': 163, 'labels': ['Subject'], 'rel': 'HAS_TREATMENT'}
         """
         with self.driver.session() as new_session:
             # Fetch the parents
             cypher = f"MATCH (parent)-[inbound]->(n) WHERE id(n) = {node_id} " \
                      "RETURN id(parent) AS id, labels(parent) AS labels, type(inbound) AS rel"
-            if self.debug:
-                print(f"""
+            if self.verbose:
+                logger.debug(f"""
                 query: {cypher}            
                 """)
             result_obj = new_session.run(cypher)  # A new neo4j.Result object
             parent_list = result_obj.data()
             # EXAMPLE of parent_list:
             #       [{'id': 163, 'labels': ['Subject'], 'rel': 'HAS_TREATMENT'},
             #        {'id': 150, 'labels': ['Subject'], 'rel': 'HAS_TREATMENT'}]
             if self.verbose:
-                print(f"parent_list for node {node_id}:", parent_list)
+                logger.info(f"parent_list for node {node_id}: {parent_list}")
 
             # Fetch the children
             cypher = f"MATCH (n)-[outbound]->(child) WHERE id(n) = {node_id} " \
                      "RETURN id(child) AS id, labels(child) AS labels, type(outbound) AS rel"
-            if self.debug:
-                print(f"""
+            if self.verbose:
+                logger.debug(f"""
                 query: {cypher}      
                 """)
             result_obj = new_session.run(cypher)  # A new neo4j.Result object
             child_list = result_obj.data()
             # EXAMPLE of child_list:
             #       [{'id': 107, 'labels': ['Source Data Row'], 'rel': 'FROM_DATA'},
             #        {'id': 103, 'labels': ['Source Data Row'], 'rel': 'FROM_DATA'}]
             if self.verbose:
-                print(f"child_list for node {node_id}:", child_list)
+                logger.info(f"child_list for node {node_id}: {child_list}")
 
         return {'parent_list': parent_list, 'child_list': child_list}
 
-    def get_labels(self) -> [str]:
+    def get_labels(self) -> List[str]:
         """
         Extract and return a list of all the Neo4j labels present in the database.
         No particular order should be expected.
         TODO: test when there are nodes that have multiple labels
         :return:    A list of strings
         """
         results = self.query("call db.labels() yield label return label")
         return [x['label'] for x in results]
 
-    def get_relationshipTypes(self) -> [str]:
+    def get_relationshipTypes(self) -> List[str]:
         """
         Extract and return a list of all the Neo4j relationship types present in the database.
         No particular order should be expected.
         :return:    A list of strings
         """
         results = self.query("call db.relationshipTypes() yield relationshipType return relationshipType")
         return [x['relationshipType'] for x in results]
@@ -721,16 +729,16 @@
         CALL db.schema.nodeTypeProperties() 
         YIELD nodeLabels, propertyName
         WHERE $label in nodeLabels and propertyName IS NOT NULL
         RETURN DISTINCT propertyName 
         ORDER BY propertyName
         """
         params = {'label': label}
-        if self.debug:
-            print("q : ", q, " | params : ", params)
+        if self.verbose:
+            logger.debug(f"q : {q} | params : {params}")
         return [res['propertyName'] for res in self.query(q, params)]
 
     #########################################################################################
     #                                                                                       #
     #                           METHODS TO GET/CREATE/MODIFY SCHEMA                         #
     #                                                                                       #
     #########################################################################################
@@ -822,16 +830,16 @@
                 1                [person]          [sex]
                 
         then existing_standard_names will be:  [('car', 'color_make'), ('person', 'sex')]
         """
 
         if (label, key) not in existing_standard_name_pairs:
             q = f'CREATE INDEX `{label}.{key}` FOR (s:`{label}`) ON (s.`{key}`)'
-            if self.debug:
-                print(f"""
+            if self.verbose:
+                logger.debug(f"""
                 query: {q}
                 """)
             self.query(q)
             return True
         else:
             return False
 
@@ -859,16 +867,16 @@
         # a standard name for a constraint is assigned: `{label}.{key}.{type}` if name was not provided
         cname = (name if name else f"`{label}.{key}.{type}`")
         if cname in list(existing_constraints['name']):
             return False
 
         try:
             q = f'CREATE CONSTRAINT {cname} ON (s:`{label}`) ASSERT s.`{key}` IS UNIQUE'
-            if self.debug:
-                print(f"""
+            if self.verbose:
+                logger.debug(f"""
                 query: {q}
                 """)
             self.query(q)
             # Note: creation of a constraint will crash if another constraint, or index, already exists
             #           for the specified label and key
             return True
         except Exception:
@@ -879,16 +887,16 @@
         Eliminate the index with the specified name.
 
         :param name:    Name of the index to eliminate
         :return:        True if successful or False otherwise (for example, if the index doesn't exist)
         """
         try:
             q = f"DROP INDEX `{name}`"
-            if self.debug:
-                print(f"""
+            if self.verbose:
+                logger.debug(f"""
                 query: {q}
                 """)
             self.query(q)  # Note: it crashes if the index doesn't exist
             return True
         except Exception:
             return False
 
@@ -914,16 +922,16 @@
         Eliminate the constraint with the specified name.
 
         :param name:    Name of the constraint to eliminate
         :return:        True if successful or False otherwise (for example, if the constraint doesn't exist)
         """
         try:
             q = f"DROP CONSTRAINT `{name}`"
-            if self.debug:
-                print(f"""
+            if self.verbose:
+                logger.debug(f"""
                 query: {q}
                 """)
             self.query(q)  # Note: it crashes if the constraint doesn't exist
             return True
         except Exception:
             return False
 
@@ -968,16 +976,16 @@
 
         # Turn labels (string or list/tuple of labels) into a string suitable for inclusion into Cypher
         cypher_labels = self._prepare_labels(labels)
 
         # Assemble the complete Cypher query
         cypher = f"CREATE (n {cypher_labels} {attributes_str}) RETURN n"
 
-        if self.debug:
-            print(f"""
+        if self.verbose:
+            logger.debug(f"""
                 In create_node_by_label_and_dict().
                 query: {cypher}
                 parameters: {data_dictionary}
                 """)
 
         result_list = self.query_expanded(cypher, data_dictionary, flatten=True)
         return result_list[0]['neo4j_id']  # Return the Neo4j internal ID of the node just created
@@ -988,35 +996,36 @@
         Optionally, only delete nodes with the specified labels, or only keep nodes with the given labels.
         Note: the keep_labels list has higher priority; if a label occurs in both lists, it will be kept.
         IMPORTANT: it does NOT clear indexes; "ghost" labels may remain!  To get rid of those, run drop_all_indexes()
 
         :param delete_labels:   An optional string, or list of strings, indicating specific labels to DELETE
         :param keep_labels:     An optional string or list of strings, indicating specific labels to KEEP
                                     (keep_labels has higher priority over delete_labels)
+        :param batch_size:      Number of operations to run in a single neo4j transaction.
         :return:                None
         """
         if (delete_labels is None) and (keep_labels is None):
             # Delete ALL nodes AND ALL relationship from the database; for efficiency, do it all at once
             if self.verbose:
-                print(f" --- Deleting all nodes in the database ---")
+                logger.info(f" --- Deleting all nodes in the database ---")
 
             if batch_size:  # In order to avoid memory errors, delete data in batches
                 q = f"""
                       call apoc.periodic.iterate(
                       'MATCH (n) RETURN n',
                       'DETACH DELETE(n)',        
                       {{batchSize:{str(batch_size)}, parallel:false}})
                       YIELD total, batches, failedBatches
                       RETURN total, batches, failedBatches                                                                    
                      """
             else:
                 q = "MATCH (n) DETACH DELETE(n)"
 
-            if self.debug:
-                print(f"""
+            if self.verbose:
+                logger.debug(f"""
                 query: {q}
                 """)
 
             self.query(q)
             return
 
         if not delete_labels:
@@ -1033,18 +1042,18 @@
                 keep_labels = [keep_labels]  # If a string was passed, turn it into a list
 
         # Delete all nodes with labels in the delete_labels list,
         #   EXCEPT for any label in the keep_labels list
         for label in delete_labels:
             if not (label in keep_labels):
                 if self.verbose:
-                    print(f" --- Deleting nodes with label: `{label}` ---")
+                    logger.info(f" --- Deleting nodes with label: `{label}` ---")
                 q = f"MATCH (x:`{label}`) DETACH DELETE x"
-                if self.debug:
-                    print(f"""
+                if self.verbose:
+                    logger.debug(f"""
                     query: {q}                        
                     """)
                 self.query(q)
 
     def clean_slate(self, keep_labels=None, drop_indexes=True, drop_constraints=True) -> None:
         """
         Use this to get rid of absolutely everything in the database.
@@ -1052,15 +1061,15 @@
         :param keep_labels:     An optional list of strings, indicating specific labels to KEEP
         :param drop_indexes:    Flag indicating whether to also ditch all indexes (by default, True)
         :param drop_constraints:Flag indicating whether to also ditch all constraints (by default, True)
         :return:                None
         """
         if drop_indexes:
             self.drop_all_indexes(including_constraints=drop_constraints)
-            #TODO: check if self.rdf the dropped constraint fon Resource.uri does not cause trouble
+            # TODO: check if self.rdf the dropped constraint fon Resource.uri does not cause trouble
 
         if self.rdf:
             self.delete_nodes_by_label(
                 keep_labels=(keep_labels + ['_GraphConfig'] if keep_labels else ['_GraphConfig']))
         else:
             self.delete_nodes_by_label(keep_labels=keep_labels)
 
@@ -1096,27 +1105,27 @@
         cypher = cypher_match + set_clause
 
         # Example of cypher:
         # "MATCH (n:car {`vehicle id`: $par_1}) SET n.`color` = color, n.`price` = $field2"
         # Example of data binding:
         #       {"par_1": 123, "color": "white", "price": 7000}
 
-        if self.debug:
-            print("cypher: ", cypher)
-            print("data_binding: ", cypher_dict)
+        if self.verbose:
+            logger.debug(f"cypher: {cypher}")
+            logger.debug(f"data_binding: {cypher_dict}")
 
         self.query(cypher, cypher_dict)
 
     def extract_entities(self,
                          mode='merge',
                          label=None,
                          cypher=None,
                          cypher_dict=None,
                          target_label=None,
-                         property_mapping={},
+                         property_mapping=None,
                          relationship=None,
                          direction='<'
                          ):
         """
         :param mode:str; assert mode in ['merge', 'create']
         :param label:str; label of the nodes to extract data from
         :param cypher: str; only of label not provided: cypher that returns id(node) of the nodes to extract data from
@@ -1134,14 +1143,17 @@
             to to the property names of the target class where the data is extracted to
             		if list: properties of the extracted node (as per the list) will extracted and will be named same as
             		in the source node
         :param relationship: type of the relationship (to/from the extraction node) to create
         :param direction: direction of the relationship to create (>: to the extraction node, <: from the extraction node)
         :return: None
         """
+        if property_mapping is None:
+            property_mapping = {}
+
         assert mode in ['merge', 'create']
         assert direction in ['>', '<']
         assert type(property_mapping) in [dict, list]
         assert type(target_label) in [list, str] or target_label is None
         if target_label:
             if type(target_label) == str:
                 target_label = [target_label]
@@ -1162,16 +1174,16 @@
                 q_match_part = """
                 CALL apoc.cypher.run($cypher, $cypher_dict) YIELD value
                 MATCH (data) WHERE id(data) = value['id(node)'] 
                 RETURN data                               
                 """
                 q_match_altered = True
             else:
-                if self.debug:
-                    print("ERROR: not all parameters have been supplied in cypher_dict, missing: ", missing_params)
+                if self.verbose:
+                    logger.debug(f"ERROR: not all parameters have been supplied in cypher_dict, missing: {missing_params}")
 
         rel_left = ('' if direction == '>' else '<')
         rel_right = ('>' if direction == '>' else '')
         q = f"""
                     call apoc.periodic.iterate(
                    $q_match_part
                    ,
@@ -1187,18 +1199,18 @@
                """
         inner_params = {'target_label': target_label,
                         'mapping': property_mapping}
         if q_match_altered:
             inner_params = {**inner_params, 'cypher': cypher, 'cypher_dict': cypher_dict}
         params = {'q_match_part': q_match_part, 'target_label': target_label, 'inner_params': inner_params}
         res = self.query(q, params)
-        if self.debug:
-            print("        Query : ", q)
-            print("        Query parameters: ", params)
-            print("        Result of above query : ", res, "\n")
+        if self.verbose:
+            logger.debug(f"        Query : {q}")
+            logger.debug(f"        Query parameters: {params}")
+            logger.debug(f"        Result of above query : {res}\n")
 
     #########################################################################################
     #                                                                                       #
     #                           METHODS TO CREATE NEW RELATIONSHIPS                         #
     #                                                                                       #
     #########################################################################################
 
@@ -1242,20 +1254,20 @@
         if cond_right_rel.startswith("<"):
             cond_right_rel_mark1 = "<"
         if cond_right_rel.endswith(">"):
             cond_right_rel_mark2 = ">"
         cond_right_rel_type = re.sub(r'^(\<)?(.*?)(\>)?$', r'\2', cond_right_rel)
         if cond_cypher:
             if self.verbose:
-                print(
+                logger.info(
                     f"Using cypher condition to link nodes. Labels: {left_class}, {right_class}; Cypher: {cond_cypher}")
-                periodic_part1 = """
-                CALL apoc.cypher.run($cypher, $cypher_dict) YIELD value
-                RETURN value.`left` as left, value.`right` as right                                                
-                """
+            periodic_part1 = """
+            CALL apoc.cypher.run($cypher, $cypher_dict) YIELD value
+            RETURN value.`left` as left, value.`right` as right                                                
+            """
         else:
             periodic_part1 = f'''
             MATCH (left){cond_left_rel_mark1}-[:`{cond_left_rel_type}`*0..1]-{cond_left_rel_mark2}(sdr:`{cond_via_node}`),
             (sdr){cond_right_rel_mark1}-[:`{cond_right_rel_type}`*0..1]-{cond_right_rel_mark2}(right)
             WHERE left:`{left_class}` and right:`{right_class}` 
             RETURN left, right 
             '''
@@ -1266,17 +1278,17 @@
                MERGE (left)-[:`{relationship}`]->(right)          
             ',        
             {{batchSize:10000, parallel:false, params: {{cypher: $cypher, cypher_dict: $cypher_dict}}}})
             YIELD total, batches, failedBatches
             RETURN total, batches, failedBatches
         """
         params = {'cypher': cond_cypher, 'cypher_dict': cond_cypher_dict}
-        if self.debug:
-            print("        Query : ", q)
-            print("        Query parameters: ", params)
+        if self.verbose:
+            logger.debug(f"        Query : {q}")
+            logger.debug(f"        Query parameters: {params}")
         self.query(q, params)
 
     def link_nodes_on_matching_property(self, label1: str, label2: str, property1: str, rel: str,
                                         property2=None) -> None:
         """
         Locate any pair of Neo4j nodes where all of the following hold:
                             1) the first one has label1
@@ -1294,16 +1306,16 @@
         :param rel:         Name to give to all relationships that get created
         :return:            None
         """
         if not property2:
             property2 = property1
         q = f'''MATCH (x:`{label1}`), (y:`{label2}`) WHERE x.`{property1}` = y.`{property2}` 
                 MERGE (x)-[:{rel}]->(y)'''
-        if self.debug:
-            print(f"""
+        if self.verbose:
+            logger.debug(f"""
             query: {q}
             """)
         self.query(q)
 
     def link_nodes_on_matching_property_value(self, label1: str, label2: str, prop_name: str, prop_value: str,
                                               rel: str) -> None:
         """
@@ -1320,16 +1332,16 @@
         :param prop_name:   Name of property that must be present in both nodes
         :param prop_value:  A STRING value that the above property must have in both nodes
         :param rel:         Name to give to all relationships that get created
         :return:            None
         """
         q = f'''MATCH (x:`{label1}`), (y:`{label2}`) WHERE x.`{prop_name}` = "{prop_value}" AND y.`{prop_name}` = "{prop_value}" 
                 MERGE (x)-[:{rel}]->(y)'''
-        if self.debug:
-            print(f"""
+        if self.verbose:
+            logger.debug(f"""
             query: {q}
             """)
         self.query(q)
 
     def link_nodes_by_ids(self, node_id1: int, node_id2: int, rel: str, rel_props=None) -> None:
         """
         Locate the pair of Neo4j nodes with the given Neo4j internal ID's.
@@ -1354,16 +1366,16 @@
         MERGE (x)-[:`{rel}` {cypher_rel_props}]->(y)
         """
 
         # Extend the (possibly empty) Cypher data dictionary, to also include a value for the key "node_id1" and "node_id2"
         cypher_dict["node_id1"] = node_id1
         cypher_dict["node_id2"] = node_id2
 
-        if self.debug:
-            print(f"""
+        if self.verbose:
+            logger.debug(f"""
             query: {q}
             parameters: {cypher_dict}
             """)
 
         self.query(q, cypher_dict)
 
     #####################################################################################################
@@ -1434,15 +1446,15 @@
         if ignore_nan:
             for col, dtype in df.dtypes.iteritems():
                 if dtype in ['float64', 'int64']:
                     numeric_columns.append(col)
 
         if merge and not merge_overwrite and primary_key in numeric_columns:
             assert not (df[primary_key].isna().any()), f"Cannot merge node on NULL value in {primary_key}. " \
-            "Use merge_overwrite=True or eliminate missing values"
+             "Use merge_overwrite=True or eliminate missing values"
 
         op = 'MERGE' if (merge and primary_key) else 'CREATE'  # A MERGE or CREATE operation, as needed
         res = []
         for df_chunk in np.array_split(df, int(len(df.index) / max_chunk_size) + 1):  # Split the operation into batches
             if numeric_columns:
                 cypher = f'''
                 WITH $data AS data 
@@ -1457,16 +1469,16 @@
                 cypher = f'''
                 WITH $data AS data 
                 UNWIND data AS record {op} (x:`{label}`{primary_key_s}) 
                 SET x{('' if merge_overwrite else '+')}=record 
                 RETURN id(x) as node_id 
                 '''
                 cypher_dict = {'data': df_chunk.to_dict(orient='records')}
-            if self.debug:
-                print(f"""
+            if self.verbose:
+                logger.debug(f"""
                 query: {cypher}
                 parameters: {cypher_dict}
                 """)
             res_chunk = self.query(cypher, cypher_dict)
             if res_chunk:
                 res += [r['node_id'] for r in res_chunk]
         return res
@@ -1553,14 +1565,17 @@
             dct = json.load(jsonfile)
         neo = NeoInterface()
         neo.load_arrows_dict(dct)
 
         :param dct: python dict to load
         :param merge_on: None or dict with label as key and list of properties as value - the properties will be used
         as identProps in apoc.merge.node, the rest of the properties will be used as onCreateProps and onMatchProps
+        :param always_create: Optional list of labels to be CREATED rather than MERGED
+        :param timestamp: Bool, if true includes an additional "_timestamp" property on node CREATION or MERGE equal to
+                          cypher timestamp()
         :return: result of the corresponding Neo4j query
         """
         assert merge_on is None or isinstance(merge_on, dict)
         if not merge_on:
             merge_on = {}
         for key, item in merge_on.items():
             assert isinstance(item, list)
@@ -1685,15 +1700,15 @@
         :param data_dict:   A Python dictionary
         :return:            A pair consisting of a string suitable for Cypher queries,
                                 and a corresponding data-binding dictionary.
                             If the passed dictionary is empty or None,
                                 the pair returned is ("", {})
         """
         if data_dict is None or data_dict == {}:
-            return ("", {})
+            return "", {}
 
         rel_props_list = []  # A list of strings
         data_dictionary = {}
         parameter_count = 1  # Sequential integers used in the data dictionary, such as "par_1", "par_2", etc.
         for prop_key, prop_value in data_dict.items():
             parameter_token = f"par_{parameter_count}"  # EXAMPLE: "par_3"
 
@@ -1702,15 +1717,15 @@
             data_dictionary[parameter_token] = prop_value
             parameter_count += 1
 
         rel_props_str = ", ".join(rel_props_list)
 
         rel_props_str = "{" + rel_props_str + "}"
 
-        return (rel_props_str, data_dictionary)
+        return rel_props_str, data_dictionary
 
     ############################################################################################
     #                                                                                          #
     #                           METHODS TO SUPPORT DEBUGGING                                   #
     #                                                                                          #
     ############################################################################################
 
@@ -1747,15 +1762,15 @@
 
     ############################################################################################
     #                                                                                          #
     #                           METHODS TO SUPPORT JSON IMPORT/EXPORT                          #
     #                                                                                          #
     ############################################################################################
 
-    def export_dbase_json(self) -> {}:
+    def export_dbase_json(self) -> dict:
         """
         Export the entire Neo4j database as a JSON string
         EXAMPLE:
         { 'nodes': 2,
           'relationships': 1,
           'properties': 6,
           'data': '[{"type":"node","id":"3","labels":["User"],"properties":{"name":"Adam","age":32,"male":true}},\n
@@ -1816,16 +1831,16 @@
         """
 
         try:
             json_list = json.loads(json_str)  # Turn the string (representing a JSON list) into a list
         except Exception as ex:
             raise Exception(f"Incorrectly-formatted JSON string. {ex}")
 
-        if self.debug:
-            print("json_list: ", json_list)
+        if self.verbose:
+            logger.debug(f"json_list: {json_list}")
 
         assert type(json_list) == list, "The JSON string does not represent the expected list"
 
         id_shifting = {}  # To map the Neo4j internal ID's specified in the JSON data dump
         #       into the ID's of newly-created nodes
 
         # Do an initial pass for correctness, to try to avoid partial imports
@@ -1857,32 +1872,32 @@
                     raise Exception(
                         f"Item in list index {i} is marked as 'relationship' but its 'end' value lacks an 'id'.  Nothing imported.  Item: {item}")
 
         # First, process all the nodes, and in the process create the id_shifting map
         num_nodes_imported = 0
         for item in json_list:
             if item["type"] == "node":
-                if self.debug:
-                    print("ADDING NODE: ", item)
-                    print(f'     Creating node with label `{item["labels"][0]}` and properties {item["properties"]}')
+                if self.verbose:
+                    logger.debug(f"ADDING NODE: {item}")
+                    logger.debug(f'     Creating node with label `{item["labels"][0]}` and properties {item["properties"]}')
                 old_id = int(item["id"])
                 new_id = self.create_node_by_label_and_dict(item["labels"][0], item[
                     "properties"])  # TODO: Only the 1st label is used for now
                 id_shifting[old_id] = new_id
                 num_nodes_imported += 1
 
-        if self.debug:
-            print("id_shifting map:", id_shifting)
+        if self.verbose:
+            logger.debug(f"id_shifting map: {id_shifting}")
 
         # Then process all the relationships, linking to the correct (newly-created) nodes by using the id_shifting map
         num_rels_imported = 0
         for item in json_list:
             if item["type"] == "relationship":
-                if self.debug:
-                    print("ADDING RELATIONSHIP: ", item)
+                if self.verbose:
+                    logger.debug(f"ADDING RELATIONSHIP: {item}")
 
                 rel_name = item["label"]
                 rel_props = item.get(
                     "properties")  # Also works if no "properties" is present (relationships may lack it)
 
                 start_id_original = int(item["start"]["id"])
                 end_id_original = int(item["end"]["id"])
@@ -1899,18 +1914,18 @@
     ############################################################################################
     #                                                                                          #
     #                           METHODS TO SUPPORT RDF PROCEDURES                              #
     #                                                                                          #
     ############################################################################################
 
     def rdf_generate_uri(self,
-                         dct={},
+                         dct=None,
                          include_label_in_uri=True,
                          prefix='neo4j://graph.schema#',
-                         add_prefixes=[],
+                         add_prefixes=None,
                          sep='/',
                          uri_prop='uri') -> None:
         """
         A method that
             - on the neo4j nodes with labels equal to keys of :dict dictionary
             - sets additional label Resource (for handling in RDF)
             - sets property with name :uri_prop with value that starts with prefix followed by a string
@@ -1944,16 +1959,23 @@
                 set URI on 'Vehicle' nodes using node's property "producer"
                     uri = 'neo4j://graph.schema#Vehicle/Toyota'
                 set URI on 'Model' nodes using node's property "name" and neighbouring node's property "producer"
                     uri = 'neo4j://graph.schema#Model/Toyota/Prius'
         :param prefix: a prefix for uri
         :param add_prefixes: list of prefixes to prepend uri with (after prefix), list joined with :sep separator
         :param sep: separator for joining add_perfixes and the primary keys into uri
+        :param include_label_in_uri: Bool includes label in URI as the first element after prefix
+        :param uri_prop: string URI property name, defaults to 'uri'
         :return: None
         """
+        if dct is None:
+            dct = {}
+        if add_prefixes is None:
+            add_prefixes = []
+
         for label, config in dct.items():
             assert isinstance(label, str)
             assert any(isinstance(config, t) for t in [list, str, dict])
             where = ""
             neighbours = False
             neighbours_query = ""
             if isinstance(config, str):
@@ -2021,30 +2043,33 @@
                 'properties': properties_ext
             }
             if neighbours:
                 cypher_dict.update({
                     'neighbours': config['neighbours']
                 })
 
-            if self.debug:
-                print(f"""
+            if self.verbose:
+                logger.debug(f"""
                 query: {cypher}
                 parameters: {cypher_dict}
                 """)
             self.query(cypher, cypher_dict)
             self._rdf_uri_cleanup()
 
-    def rdf_get_subgraph(self, cypher: str, cypher_dict={}, format="Turtle-star") -> str:
+    def rdf_get_subgraph(self, cypher: str, cypher_dict=None, format="Turtle-star") -> str:
         """
         A method that returns an RDF serialization of a subgraph specified by :cypher query
         :param cypher: cypher query to return a subgraph
         :param cypher_dict: parameters required for the cypher query
         :param format: RDF format in which to serialize output
         :return: str - RDF serialization of subgraph
         """
+        if cypher_dict is None:
+            cypher_dict = {}
+
         self._rdf_subgraph_cleanup()
         url = self.rdf_host + "neo4j/cypher"
         j = ({'cypher': cypher, 'format': format, 'cypherParams': cypher_dict})
         response = requests.post(
             url=url,
             json=j,
             auth=self.credentials)
@@ -2052,16 +2077,16 @@
         # see https://community.neo4j.com/t/export-procedure-that-returns-serialized-rdf/38781/2
         return response.text
 
     def rdf_import_fetch(self, url: str, format="Turtle-star"):
         cypher = "CALL n10s.rdf.import.fetch ($url, $format) YIELD terminationStatus, triplesLoaded, triplesParsed, " \
                  "namespaces, extraInfo, callParams"
         cypher_dict = {'url': url, 'format': format}
-        if self.debug:
-            print(f"""
+        if self.verbose:
+            logger.debug(f"""
                 query: {cypher}
                 parameters: {cypher_dict}
                 """)
         return self.query(cypher, cypher_dict)
 
     def rdf_import_subgraph_inline(self, rdf: str, format="Turtle-star"):
         """
@@ -2077,16 +2102,16 @@
         cypher = """
         CALL n10s.rdf.import.inline($rdf, $format) 
         YIELD triplesParsed, triplesLoaded, extraInfo 
         RETURN *
         """
         # cypher_dict = {'rdf':rdf.encode('utf-8').decode('utf-8'), 'format': format}
         cypher_dict = {'rdf': rdf, 'format': format}
-        if self.debug:
-            print(f"""
+        if self.verbose:
+            logger.debug(f"""
             query: {cypher}
             parameters: {cypher_dict}
             """)
         res = self.query(cypher, cypher_dict)
         self._rdf_subgraph_cleanup()
         if len(res) > 0:
             return res[0]
@@ -2099,16 +2124,16 @@
         cypher = """
             UNWIND $labels as label
             CALL apoc.refactor.rename.label(label, apoc.text.regreplace(label, '%20', ' '))
             YIELD batches, failedBatches, total, failedOperations 
             RETURN batches, failedBatches, total, failedOperations
         """
         cypher_dict = {'labels': [label for label in self.get_labels() if "%20" in label]}
-        if self.debug:
-            print(f"""
+        if self.verbose:
+            logger.debug(f"""
             query: {cypher}
             parameters: {cypher_dict}
             """)
         self.query(cypher, cypher_dict)
 
         # in case properties with spaces where serialized new properties with spaces being replaced with %20 could have been created
         # this helper function is supposed to revert the change
@@ -2122,16 +2147,16 @@
             'REMOVE node.`' + propertyName + '`'        
             ,
             {}
         ) YIELD value
         RETURN value['node']
         """
         cypher_dict2 = {}
-        if self.debug:
-            print(f"""
+        if self.verbose:
+            logger.debug(f"""
             query: {cypher2}
             parameters: {cypher_dict2}
             """)
         self.query(cypher2, cypher_dict2)
 
         self._rdf_uri_cleanup()
 
@@ -2141,16 +2166,16 @@
         MATCH (n)
         WHERE n.uri is not null
         SET n.uri = apoc.text.replace(n.uri, '%23', '#')
         SET n.uri = apoc.text.replace(n.uri, '%2F', '/')
         SET n.uri = apoc.text.replace(n.uri, '%3A', ':')
         """
         cypher_dict3 = {}
-        if self.debug:
-            print(f"""
+        if self.verbose:
+            logger.debug(f"""
             query: {cypher3}
             parameters: {cypher_dict3}
             """)
         self.query(cypher3, cypher_dict3)
 
     def rdf_get_graph_onto(self):
         """
```

### Comparing `neointerface-3.1.9/neointerface.egg-info/PKG-INFO` & `neointerface-3.3.1/neointerface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neointerface
-Version: 3.1.9
+Version: 3.3.1
 Summary: A Python interface to use the Neo4j graph database
 Home-page: UNKNOWN
 Author: Alexey Kuznetsov, Julian West, Ben Grinsted, William McDermott
 License: 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
@@ -203,13 +203,13 @@
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
-Description: https://github.com/GSK-Biostatistics/neointerface#neointerface---neo4j-made-easy-for-python-programmers
+Description: https://github.com/GSK-Biostatistics/neointerface/blob/main/README.md
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `neointerface-3.1.9/setup.py` & `neointerface-3.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import setuptools
 import os
 
-with open("README.md", "r") as fh:
-    long_description = "https://github.com/GSK-Biostatistics/neointerface#neointerface---neo4j-made-easy-for-python-programmers"
-
 def read_text(file_name: str):
     return open(os.path.join(file_name)).read()
 
+
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 required = []
 dependency_links = []
 
 # Do not add to required lines pointing to Git repositories
@@ -26,18 +24,18 @@
             print('Dependency to a git repository should have the format:')
             print('git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name')
     else:
         required.append(line)
 
 setuptools.setup(
     name="neointerface",                     # This is the name of the package
-    version="3.1.9",                         # The initial release version
+    version="3.3.1",                         # The initial release version
     author="Alexey Kuznetsov, Julian West, Ben Grinsted, William McDermott",  # Full name of the authors
     description="A Python interface to use the Neo4j graph database",
-    long_description=long_description,      # Long description read from the the readme file
+    long_description="https://github.com/GSK-Biostatistics/neointerface/blob/main/README.md",      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     license=read_text("LICENSE"),
```

