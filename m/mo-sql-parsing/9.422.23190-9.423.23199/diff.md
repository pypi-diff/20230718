# Comparing `tmp/mo_sql_parsing-9.422.23190-py2.py3-none-any.whl.zip` & `tmp/mo_sql_parsing-9.423.23199-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 38385 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat     2597 b- defN 22-Dec-18 22:41 mo_sql_parsing/__init__.py
--rw-rw-rw-  2.0 fat    22449 b- defN 23-Jun-10 00:48 mo_sql_parsing/formatting.py
--rw-rw-rw-  2.0 fat    10666 b- defN 23-Jun-10 00:27 mo_sql_parsing/keywords.py
--rw-rw-rw-  2.0 fat    33848 b- defN 23-Jul-09 13:13 mo_sql_parsing/sql_parser.py
+Zip file size: 38292 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat     2530 b- defN 23-Jul-18 01:32 mo_sql_parsing/__init__.py
+-rw-rw-rw-  2.0 fat    22382 b- defN 23-Jul-18 01:32 mo_sql_parsing/formatting.py
+-rw-rw-rw-  2.0 fat    10695 b- defN 23-Jul-18 01:32 mo_sql_parsing/keywords.py
+-rw-rw-rw-  2.0 fat    33903 b- defN 23-Jul-18 01:32 mo_sql_parsing/sql_parser.py
 -rw-rw-rw-  2.0 fat     7321 b- defN 23-Mar-26 12:53 mo_sql_parsing/types.py
--rw-rw-rw-  2.0 fat    22999 b- defN 23-May-24 01:38 mo_sql_parsing/utils.py
--rw-rw-rw-  2.0 fat     2987 b- defN 23-Mar-26 12:53 mo_sql_parsing/windows.py
--rw-rw-rw-  2.0 fat    15922 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9345 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1134 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/RECORD
-13 files, 129395 bytes uncompressed, 36479 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat    22995 b- defN 23-Jul-18 01:32 mo_sql_parsing/utils.py
+-rw-rw-rw-  2.0 fat     2920 b- defN 23-Jul-18 01:32 mo_sql_parsing/windows.py
+-rw-rw-rw-  2.0 fat    15922 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9345 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/zip-safe
+?rw-rw-r--  2.0 fat     1134 b- defN 23-Jul-18 01:32 mo_sql_parsing-9.423.23199.dist-info/RECORD
+13 files, 129274 bytes uncompressed, 36386 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mo_sql_parsing/utils.py
 Comment: 
 
 Filename: mo_sql_parsing/windows.py
 Comment: 
 
-Filename: mo_sql_parsing-9.422.23190.dist-info/LICENSE
+Filename: mo_sql_parsing-9.423.23199.dist-info/LICENSE
 Comment: 
 
-Filename: mo_sql_parsing-9.422.23190.dist-info/METADATA
+Filename: mo_sql_parsing-9.423.23199.dist-info/METADATA
 Comment: 
 
-Filename: mo_sql_parsing-9.422.23190.dist-info/WHEEL
+Filename: mo_sql_parsing-9.423.23199.dist-info/WHEEL
 Comment: 
 
-Filename: mo_sql_parsing-9.422.23190.dist-info/top_level.txt
+Filename: mo_sql_parsing-9.423.23199.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_sql_parsing-9.422.23190.dist-info/zip-safe
+Filename: mo_sql_parsing-9.423.23199.dist-info/zip-safe
 Comment: 
 
-Filename: mo_sql_parsing-9.422.23190.dist-info/RECORD
+Filename: mo_sql_parsing-9.423.23199.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_sql_parsing/__init__.py

```diff
@@ -3,15 +3,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
-from __future__ import absolute_import, division, unicode_literals
 
 import json
 from threading import Lock
 
 from mo_parsing import debug
 
 from mo_sql_parsing.sql_parser import scrub
```

## mo_sql_parsing/formatting.py

```diff
@@ -3,15 +3,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Author: Beto Dealmeida (beto@dealmeida.net)
 #
 
-from __future__ import absolute_import, division, unicode_literals
 
 import re
 
 from mo_dots import split_field
 from mo_future import first, is_text, string_types, text
 from mo_parsing import listwrap
 
@@ -550,15 +549,15 @@
             return f"SELECT {param}"
 
     def distinct_on(self, json, prec):
         param = ", ".join(self.dispatch(s) for s in listwrap(json["distinct_on"]))
         return f"SELECT DISTINCT ON ({param})"
 
     def select_distinct(self, json, prec):
-        param = ", ".join(self.dispatch(s, precedence['select']) for s in listwrap(json["select_distinct"]))
+        param = ", ".join(self.dispatch(s, precedence["select"]) for s in listwrap(json["select_distinct"]))
         return f"SELECT DISTINCT {param}"
 
     def from_(self, json, prec):
         is_join = False
         from_ = json["from"]
         if isinstance(from_, dict) and "literal" in from_:
             content = ", ".join(self._literal(row) for row in from_["literal"])
```

## mo_sql_parsing/keywords.py

```diff
@@ -138,15 +138,19 @@
 UNPIVOT = keyword("unpivot")
 VIEW = keyword("view")
 
 # COMPOUND KEYWORDS
 
 
 joins = (
-    (Optional(CROSS | OUTER | INNER | NATURAL | ((FULL | LEFT | RIGHT) + Optional(INNER | OUTER))) + JOIN + Optional(LATERAL))
+    (
+        Optional(CROSS | OUTER | INNER | NATURAL | ((FULL | LEFT | RIGHT) + Optional(INNER | OUTER)))
+        + JOIN
+        + Optional(LATERAL)
+    )
     | LATERAL + Optional(VIEW + Optional(OUTER))
     | (CROSS | OUTER) + APPLY
 ) / (lambda tokens: " ".join(tokens).lower())
 
 UNION_ALL = (UNION + ALL).set_parser_name("union_all")
 WITHIN_GROUP = Group(WITHIN + GROUP).set_parser_name("within_group")
 SELECT_DISTINCT = Group(SELECT + DISTINCT).set_parser_name("select distinct")
@@ -435,9 +439,8 @@
     "m": "minute",
     "h": "hour",
     "d": "day",
     "w": "week",
     "M": "month",
     "y": "year",
     "c": "century",
-
 }
```

## mo_sql_parsing/sql_parser.py

```diff
@@ -505,15 +505,15 @@
             & Optional(
                 FETCH
                 + Optional(keyword("first") | keyword("next"))
                 + expression("fetch")
                 + rows
                 + Optional(keyword("only"))
             )
-            & Optional(assign("limit", expression))
+            & Optional(LIMIT + ((expression("offset") + "," + expression("limit")) | expression("limit")))
         )
 
         # https://www.postgresql.org/docs/current/sql-select.html
         #  [ FOR { UPDATE | NO KEY UPDATE | SHARE | KEY SHARE } [ OF table_name [, ...] ] [ NOWAIT | SKIP LOCKED ] [...] ]
         for_update = Optional(Group(
             FOR
             + (keyword("update") | keyword("share") | keyword("no key update") | keyword("key share"))("mode")
@@ -567,16 +567,16 @@
 
         table_constraint_definition = Optional(CONSTRAINT + identifier("name")) + (
             assign("primary key", index_type + index_column_names + index_options)
             | (
                 Optional(flag("unique"))
                 + Optional(INDEX | KEY)
                 + Optional(identifier("name"))
-                + index_type
                 + index_column_names
+                + index_type
                 + index_options
             )("index")
             | assign("check", LB + expression + RB)
             | table_def_foreign_key("foreign_key")
         )
 
         table_element = table_constraint_definition("constraint") | column_definition("columns")
```

## mo_sql_parsing/utils.py

```diff
@@ -467,16 +467,16 @@
 def to_when_call(tokens):
     tok = tokens
     return Call("when", [tok["when"]], {"then": tok["then"]})
 
 
 def to_match_expr(tokens):
     if "expr" in tokens:
-        return Call("and", [tokens["cond"], tokens['expr']])
-    return tokens['cond']
+        return Call("and", [tokens["cond"], tokens["expr"]])
+    return tokens["cond"]
 
 
 def to_join_call(tokens):
     op = " ".join(tokens["op"])
     if tokens["join"]["name"]:
         output = {op: {"name": tokens["join"]["name"], "value": tokens["join"]["value"]}}
     else:
@@ -772,15 +772,15 @@
 # STRINGS
 ansi_string = Regex(r"\'(\'\'|[^'])*\'") / single_literal
 regex_string = (Regex(r'r\"(\\\"|[^"])*\"') | Regex(r"r\'(\\\'|[^'])*\'")) / literal_regex
 mysql_doublequote_string = Regex(r'\"(\"\"|[^"])*\"') / double_literal
 
 # BASIC IDENTIFIERS
 ansi_ident = Regex(r'\"(\"\"|[^"])*\"') / double_column
-mysql_backtick_ident = Regex(r"\`(\`\`|[^`])*\`") / backtick_column
+mysql_backtick_ident = Regex(r"`(``|[^`])*`") / backtick_column
 sqlserver_ident = Regex(r"\[(\]\]|[^\]])*\]") / square_column
 
 copy_params = (
     "ALLOW_DUPLICATE",
     "AWS_KEY_ID",
     "AWS_SECRET_KEY",
     "AWS_TOKEN",
```

## mo_sql_parsing/windows.py

```diff
@@ -3,15 +3,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
-from __future__ import absolute_import, division, unicode_literals
 
 from mo_sql_parsing.keywords import *
 from mo_sql_parsing.utils import *
 
 
 # https://docs.microsoft.com/en-us/sql/t-sql/queries/select-over-clause-transact-sql?view=sql-server-ver15
```

## Comparing `mo_sql_parsing-9.422.23190.dist-info/LICENSE` & `mo_sql_parsing-9.423.23199.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_sql_parsing-9.422.23190.dist-info/METADATA` & `mo_sql_parsing-9.423.23199.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.422.23190
+Version: 9.423.23199
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
@@ -16,15 +16,15 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mo-dots (==9.417.23168)
 Requires-Dist: mo-future (==7.416.23168)
 Requires-Dist: mo-imports (==7.416.23168)
-Requires-Dist: mo-parsing (==8.421.23188)
+Requires-Dist: mo-parsing (==8.423.23199)
 Provides-Extra: dev
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 Requires-Dist: mo-files ; extra == 'tests'
 Requires-Dist: mo-streams ; extra == 'tests'
 Requires-Dist: zstandard ; extra == 'tests'
```

## Comparing `mo_sql_parsing-9.422.23190.dist-info/RECORD` & `mo_sql_parsing-9.423.23199.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-mo_sql_parsing/__init__.py,sha256=qu67hMKaz6Rn_c0idUNZ9e_BvFuxXsDZRuwQmmGYqpI,2597
-mo_sql_parsing/formatting.py,sha256=tItgfyUsmHx8iyL-mf2MnS9vAcCrpbUxqIRZTPRYKC4,22449
-mo_sql_parsing/keywords.py,sha256=4huuey_x1Q2ervkRWMqj4woMsmmSlDDCFhKCViN5jDs,10666
-mo_sql_parsing/sql_parser.py,sha256=Jr7WkLQNX1nrLOhthysWiu30iLM49w6fj-Pl7c_1LtA,33848
+mo_sql_parsing/__init__.py,sha256=ZbsunSI2YPlPkveviGXQuv_YjCmofsrVOOu6qb500gM,2530
+mo_sql_parsing/formatting.py,sha256=Nzcrs6aWLQRK0hd8QvyPZ4hMF1onIhyvE2iBrtKF-Fw,22382
+mo_sql_parsing/keywords.py,sha256=nFTOQv7VOTDI4Ud3oSJh0-II9FGH4wWXmFRwZ5R3uzk,10695
+mo_sql_parsing/sql_parser.py,sha256=b0haZF7j7pzWNyZHCbwuu5dN3BBPSddm2Xem3yc5MkQ,33903
 mo_sql_parsing/types.py,sha256=4nnewHeuD_q3W7muesXsSS4JW73TM17YgBjlxQkOfpo,7321
-mo_sql_parsing/utils.py,sha256=1vVp9zi1uqq04Y9K0Y4yAfrqMyPhyXr7U06s4NXiqrc,22999
-mo_sql_parsing/windows.py,sha256=DNYTT34qFS8lfaDEg4oXigmYoSA72_LyHLgIQjBSpWI,2987
-mo_sql_parsing-9.422.23190.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
-mo_sql_parsing-9.422.23190.dist-info/METADATA,sha256=3aZMXKcxfoVPiF34bQuQ1ysjkG5-TftNgKWFn1DDC8c,9345
-mo_sql_parsing-9.422.23190.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_sql_parsing-9.422.23190.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
-mo_sql_parsing-9.422.23190.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-mo_sql_parsing-9.422.23190.dist-info/RECORD,,
+mo_sql_parsing/utils.py,sha256=au9Z9qebVGYikMj7sae1m7-cs1PRRNem80HVxmW6h30,22995
+mo_sql_parsing/windows.py,sha256=KelC9CZopR53tb0xAPxWsbxt59ieR_kNmM37FFcMjzE,2920
+mo_sql_parsing-9.423.23199.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
+mo_sql_parsing-9.423.23199.dist-info/METADATA,sha256=6nXYUdvoVeyN8VQTE3vfMWGDnTnVz7z6bg00Eoa5dJk,9345
+mo_sql_parsing-9.423.23199.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_sql_parsing-9.423.23199.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
+mo_sql_parsing-9.423.23199.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+mo_sql_parsing-9.423.23199.dist-info/RECORD,,
```

