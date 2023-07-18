# Comparing `tmp/turms-0.4.2.tar.gz` & `tmp/turms-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turms-0.4.2.tar", max compression
+gzip compressed data, was "turms-0.4.3.tar", max compression
```

## Comparing `turms-0.4.2.tar` & `turms-0.4.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     4881 2023-03-18 12:48:25.735186 turms-0.4.2/README.md
--rw-r--r--   0        0        0     1645 2023-05-01 10:12:24.287494 turms-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.744547 turms-0.4.2/turms/__init__.py
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.744647 turms-0.4.2/turms/cli/__init__.py
--rw-r--r--   0        0        0     8877 2023-05-01 10:12:04.859637 turms-0.4.2/turms/cli/main.py
--rw-r--r--   0        0        0      549 2023-03-18 14:44:25.565090 turms-0.4.2/turms/cli/watch.py
--rw-r--r--   0        0        0    11821 2023-05-01 10:12:04.859848 turms-0.4.2/turms/config.py
--rw-r--r--   0        0        0      799 2023-03-18 12:48:25.744917 turms-0.4.2/turms/errors.py
--rw-r--r--   0        0        0     4520 2023-03-18 14:44:25.565351 turms-0.4.2/turms/helpers.py
--rw-r--r--   0        0        0      750 2023-03-18 12:48:25.745032 turms-0.4.2/turms/mocks.py
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.745083 turms-0.4.2/turms/parsers/__init__.py
--rw-r--r--   0        0        0      525 2023-03-18 12:48:25.745145 turms-0.4.2/turms/parsers/base.py
--rw-r--r--   0        0        0     2102 2023-03-18 12:48:25.745211 turms-0.4.2/turms/parsers/polyfill.py
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.745260 turms-0.4.2/turms/plugins/__init__.py
--rw-r--r--   0        0        0     1007 2023-03-18 14:44:25.565461 turms-0.4.2/turms/plugins/base.py
--rw-r--r--   0        0        0     3718 2023-03-18 14:44:25.565640 turms-0.4.2/turms/plugins/enums.py
--rw-r--r--   0        0        0    10361 2023-03-18 14:44:25.565767 turms-0.4.2/turms/plugins/fragments.py
--rw-r--r--   0        0        0    28213 2023-03-18 14:44:25.566020 turms-0.4.2/turms/plugins/funcs.py
--rw-r--r--   0        0        0     8477 2023-03-18 14:44:25.566166 turms-0.4.2/turms/plugins/inputs.py
--rw-r--r--   0        0        0    13761 2023-03-18 14:44:25.566303 turms-0.4.2/turms/plugins/objects.py
--rw-r--r--   0        0        0     9775 2023-03-18 14:44:25.566430 turms-0.4.2/turms/plugins/operations.py
--rw-r--r--   0        0        0    33581 2023-03-18 14:44:25.566568 turms-0.4.2/turms/plugins/strawberry.py
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.746147 turms-0.4.2/turms/processors/__init__.py
--rw-r--r--   0        0        0      685 2023-03-18 12:48:25.746208 turms-0.4.2/turms/processors/base.py
--rw-r--r--   0        0        0      751 2023-03-18 12:48:25.746259 turms-0.4.2/turms/processors/black.py
--rw-r--r--   0        0        0      968 2023-03-18 12:48:25.746301 turms-0.4.2/turms/processors/disclaimer.py
--rw-r--r--   0        0        0      573 2023-03-18 12:48:25.746348 turms-0.4.2/turms/processors/isort.py
--rw-r--r--   0        0        0     8277 2023-03-18 14:44:25.566725 turms-0.4.2/turms/processors/merge.py
--rw-r--r--   0        0        0    20443 2023-03-18 14:44:25.566832 turms-0.4.2/turms/recurse.py
--rw-r--r--   0        0        0     6239 2023-03-18 14:44:25.567091 turms-0.4.2/turms/referencer.py
--rw-r--r--   0        0        0    16522 2023-03-18 14:44:25.567350 turms-0.4.2/turms/registry.py
--rw-r--r--   0        0        0    12975 2023-03-18 14:44:25.567666 turms-0.4.2/turms/run.py
--rw-r--r--   0        0        0        0 2023-03-18 12:48:25.746858 turms-0.4.2/turms/stylers/__init__.py
--rw-r--r--   0        0        0     1112 2023-03-18 12:48:25.746926 turms-0.4.2/turms/stylers/appender.py
--rw-r--r--   0        0        0     2817 2023-03-18 12:48:25.746981 turms-0.4.2/turms/stylers/base.py
--rw-r--r--   0        0        0     1163 2023-03-18 12:48:25.747037 turms-0.4.2/turms/stylers/capitalize.py
--rw-r--r--   0        0        0     1438 2023-03-18 12:48:25.747085 turms-0.4.2/turms/stylers/default.py
--rw-r--r--   0        0        0      727 2023-03-18 12:48:25.747135 turms-0.4.2/turms/stylers/snake_case.py
--rw-r--r--   0        0        0    19484 2023-03-18 14:44:25.567814 turms-0.4.2/turms/utils.py
--rw-r--r--   0        0        0     6259 1970-01-01 00:00:00.000000 turms-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     4881 2023-03-18 12:48:25.735186 turms-0.4.3/README.md
+-rw-r--r--   0        0        0     1673 2023-07-18 13:26:32.891137 turms-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.744547 turms-0.4.3/turms/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.744647 turms-0.4.3/turms/cli/__init__.py
+-rw-r--r--   0        0        0     8877 2023-05-01 10:12:04.859637 turms-0.4.3/turms/cli/main.py
+-rw-r--r--   0        0        0      549 2023-03-18 14:44:25.565090 turms-0.4.3/turms/cli/watch.py
+-rw-r--r--   0        0        0    11821 2023-05-01 10:12:04.859848 turms-0.4.3/turms/config.py
+-rw-r--r--   0        0        0      799 2023-03-18 12:48:25.744917 turms-0.4.3/turms/errors.py
+-rw-r--r--   0        0        0     4520 2023-03-18 14:44:25.565351 turms-0.4.3/turms/helpers.py
+-rw-r--r--   0        0        0      750 2023-03-18 12:48:25.745032 turms-0.4.3/turms/mocks.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.745083 turms-0.4.3/turms/parsers/__init__.py
+-rw-r--r--   0        0        0      525 2023-03-18 12:48:25.745145 turms-0.4.3/turms/parsers/base.py
+-rw-r--r--   0        0        0     2102 2023-03-18 12:48:25.745211 turms-0.4.3/turms/parsers/polyfill.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.745260 turms-0.4.3/turms/plugins/__init__.py
+-rw-r--r--   0        0        0     1007 2023-03-18 14:44:25.565461 turms-0.4.3/turms/plugins/base.py
+-rw-r--r--   0        0        0     3718 2023-03-18 14:44:25.565640 turms-0.4.3/turms/plugins/enums.py
+-rw-r--r--   0        0        0    10361 2023-03-18 14:44:25.565767 turms-0.4.3/turms/plugins/fragments.py
+-rw-r--r--   0        0        0    28634 2023-07-18 13:24:23.839568 turms-0.4.3/turms/plugins/funcs.py
+-rw-r--r--   0        0        0     8477 2023-03-18 14:44:25.566166 turms-0.4.3/turms/plugins/inputs.py
+-rw-r--r--   0        0        0    13761 2023-03-18 14:44:25.566303 turms-0.4.3/turms/plugins/objects.py
+-rw-r--r--   0        0        0    12737 2023-07-18 13:24:23.839900 turms-0.4.3/turms/plugins/operations.py
+-rw-r--r--   0        0        0    33580 2023-07-18 13:24:23.840259 turms-0.4.3/turms/plugins/strawberry.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.746147 turms-0.4.3/turms/processors/__init__.py
+-rw-r--r--   0        0        0      685 2023-03-18 12:48:25.746208 turms-0.4.3/turms/processors/base.py
+-rw-r--r--   0        0        0      751 2023-03-18 12:48:25.746259 turms-0.4.3/turms/processors/black.py
+-rw-r--r--   0        0        0      968 2023-03-18 12:48:25.746301 turms-0.4.3/turms/processors/disclaimer.py
+-rw-r--r--   0        0        0      573 2023-03-18 12:48:25.746348 turms-0.4.3/turms/processors/isort.py
+-rw-r--r--   0        0        0     8277 2023-03-18 14:44:25.566725 turms-0.4.3/turms/processors/merge.py
+-rw-r--r--   0        0        0    21002 2023-07-03 13:22:26.586564 turms-0.4.3/turms/recurse.py
+-rw-r--r--   0        0        0     6239 2023-03-18 14:44:25.567091 turms-0.4.3/turms/referencer.py
+-rw-r--r--   0        0        0    16522 2023-03-18 14:44:25.567350 turms-0.4.3/turms/registry.py
+-rw-r--r--   0        0        0    15575 2023-07-18 13:24:23.840561 turms-0.4.3/turms/run.py
+-rw-r--r--   0        0        0        0 2023-03-18 12:48:25.746858 turms-0.4.3/turms/stylers/__init__.py
+-rw-r--r--   0        0        0     1112 2023-03-18 12:48:25.746926 turms-0.4.3/turms/stylers/appender.py
+-rw-r--r--   0        0        0     2817 2023-03-18 12:48:25.746981 turms-0.4.3/turms/stylers/base.py
+-rw-r--r--   0        0        0     1163 2023-03-18 12:48:25.747037 turms-0.4.3/turms/stylers/capitalize.py
+-rw-r--r--   0        0        0     1438 2023-03-18 12:48:25.747085 turms-0.4.3/turms/stylers/default.py
+-rw-r--r--   0        0        0      727 2023-03-18 12:48:25.747135 turms-0.4.3/turms/stylers/snake_case.py
+-rw-r--r--   0        0        0    19484 2023-03-18 14:44:25.567814 turms-0.4.3/turms/utils.py
+-rw-r--r--   0        0        0     6259 1970-01-01 00:00:00.000000 turms-0.4.3/PKG-INFO
```

### Comparing `turms-0.4.2/README.md` & `turms-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/pyproject.toml` & `turms-0.4.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turms"
-version = "0.4.2"
+version = "0.4.3"
 description = "graphql-codegen powered by pydantic"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 readme = "README.md"
 packages = [{ include = "turms" }]
 homepage = "https://jhnnsrs.github.io/turms"
 repository = "https://github.com/jhnnsrs/turms"
@@ -47,17 +47,19 @@
 black = ["black"]
 isort = ["isort"]
 merge = ["libcst"]
 
 [tool.poetry.scripts]
 turms = "turms.cli.main:cli"
 
+
 [tool.poetry.group.dev.dependencies]
 libcst = "^0.4.9"
 ruff = "^0.0.257"
+pytest-snapshot = "^0.9.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.pydoc-markdown.loaders]]
 type = "python"
```

### Comparing `turms-0.4.2/turms/cli/main.py` & `turms-0.4.3/turms/cli/main.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/cli/watch.py` & `turms-0.4.3/turms/cli/watch.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/config.py` & `turms-0.4.3/turms/config.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/errors.py` & `turms-0.4.3/turms/errors.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/helpers.py` & `turms-0.4.3/turms/helpers.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/mocks.py` & `turms-0.4.3/turms/mocks.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/parsers/base.py` & `turms-0.4.3/turms/parsers/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/parsers/polyfill.py` & `turms-0.4.3/turms/parsers/polyfill.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/plugins/base.py` & `turms-0.4.3/turms/plugins/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/plugins/enums.py` & `turms-0.4.3/turms/plugins/enums.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/plugins/fragments.py` & `turms-0.4.3/turms/plugins/fragments.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/plugins/funcs.py` & `turms-0.4.3/turms/plugins/funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     prepend_async: str = "a"
     collapse_lonely: bool = True
     generate_protocol: bool = False
     global_args: List[Arg] = []
     global_kwargs: List[Kwarg] = []
     definitions: List[FunctionDefinition] = []
     extract_documentation: bool = True
+    argument_key_is_styled: bool = False
 
     class Config:
         env_prefix = "TURMS_PLUGINS_FUNCS_"
 
 
 def camel_to_snake(name):
     name = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", name)
@@ -81,62 +82,56 @@
 
 def generate_async_func_name(
     o: OperationDefinitionNode,
     plugin_config: FuncsPluginConfig,
     config: GeneratorConfig,
     registry: ClassRegistry,
 ):
-
     return f"{plugin_config.prepend_async}{camel_to_snake(o.name.value)}"
 
 
 def generate_sync_func_name(
     o: OperationDefinitionNode,
     plugin_config: FuncsPluginConfig,
     config: GeneratorConfig,
     registry: ClassRegistry,
 ):
-
     return f"{plugin_config.prepend_sync}{camel_to_snake(o.name.value)}"
 
 
 def get_extra_args_for_onode(
     definition: FunctionDefinition,
     plugin_config: FuncsPluginConfig,
 ) -> List[Arg]:
-
     args = plugin_config.global_args
     return args + definition.extra_args
 
 
 def generate_passing_extra_args_for_onode(
     definition: FunctionDefinition, plugin_config: FuncsPluginConfig
 ):
-
     return [
         ast.Name(id=arg.key, ctx=ast.Load())
         for arg in get_extra_args_for_onode(definition, plugin_config)
     ]
 
 
 def generate_passing_extra_kwargs_for_onode(
     definition: FunctionDefinition, plugin_config: FuncsPluginConfig
 ):
-
     return [
         ast.keyword(arg=kwarg.key, value=ast.Name(id=kwarg.key, ctx=ast.Load()))
         for kwarg in get_extra_kwargs_for_onode(definition, plugin_config)
     ]
 
 
 def get_extra_kwargs_for_onode(
     definition: FunctionDefinition,
     plugin_config: FuncsPluginConfig,
 ) -> List[Kwarg]:
-
     kwargs = plugin_config.global_kwargs
 
     return kwargs + definition.extra_kwargs
 
 
 def get_definitions_for_onode(
     operation_definition: OperationDefinitionNode,
@@ -165,15 +160,14 @@
 def generate_parameters(
     definition: FunctionDefinition,
     operation_definition: OperationDefinitionNode,
     config: GeneratorConfig,
     plugin_config: FuncsPluginConfig,
     registry: ClassRegistry,
 ):
-
     extra_args = get_extra_args_for_onode(definition, plugin_config)
     pos_args = []
 
     for arg in extra_args:
         registry.register_import(arg.type)
         pos_args.append(
             ast.arg(
@@ -240,33 +234,42 @@
         posonlyargs=[],
         kwonlyargs=[],
         kw_defaults=[],
         defaults=kw_values,
     )
 
 
-def generate_variable_dict(o: OperationDefinitionNode, registry: ClassRegistry):
-
+def generate_variable_dict(
+    o: OperationDefinitionNode,
+    plugin_config: FuncsPluginConfig,
+    registry: ClassRegistry,
+):
     keys = []
     values = []
 
     for v in o.variable_definitions:
-        keys.append(ast.Constant(value=v.variable.name.value))
+        if plugin_config.argument_key_is_styled:
+            keys.append(
+                ast.Constant(
+                    value=registry.generate_parameter_name(v.variable.name.value)
+                )
+            )
+        else:
+            keys.append(ast.Constant(value=v.variable.name.value))
         values.append(
             ast.Name(
                 id=registry.generate_parameter_name(v.variable.name.value),
                 ctx=ast.Load(),
             )
         )
 
     return ast.Dict(keys=keys, values=values)
 
 
 def generate_document_arg(o: OperationDefinitionNode, registry: ClassRegistry):
-
     return ast.Name(id=get_operation_class_name(o, registry), ctx=ast.Load())
 
 
 def get_operation_class_name(
     o: OperationDefinitionNode, registry: ClassRegistry
 ) -> str:
     """Generates the name of the Operation Class for the given OperationDefinitionNode
@@ -352,15 +355,14 @@
 
 def get_return_type_string(
     o: OperationDefinitionNode,
     client_schema: GraphQLSchema,
     registry: ClassRegistry,
     collapse=True,
 ) -> Tuple[str, bool]:
-
     o_name = get_operation_class_name(o, registry)
 
     root = get_operation_root_type(client_schema, o)
 
     if collapse is True:
         potential_return_field = o.selection_set.selections[0]
         potential_return_type = get_field_def(
@@ -403,15 +405,14 @@
     o: OperationDefinitionNode,
     client_schema: GraphQLSchema,
     config: GeneratorConfig,
     plugin_config: FuncsPluginConfig,
     registry: ClassRegistry,
     collapse=False,
 ):
-
     x = get_operation_root_type(client_schema, o)
     o.__annotations__
 
     get_operation_class_name(o, registry)
 
     return_type = get_return_type_string(o, client_schema, registry, collapse)
 
@@ -492,21 +493,20 @@
                         definition, plugin_config
                     ),
                     args=generate_passing_extra_args_for_onode(
                         definition, plugin_config
                     )
                     + [
                         generate_document_arg(o, registry),
-                        generate_variable_dict(o, registry),
+                        generate_variable_dict(o, plugin_config, registry),
                     ],
                 )
             )
         )
     else:
-
         return ast.Return(
             value=ast.Attribute(
                 value=ast.Await(
                     value=ast.Call(
                         func=ast.Name(
                             id=definition.use.split(".")[-1],
                             ctx=ast.Load(),
@@ -515,15 +515,15 @@
                             definition, plugin_config
                         ),
                         args=generate_passing_extra_args_for_onode(
                             definition, plugin_config
                         )
                         + [
                             generate_document_arg(o, registry),
-                            generate_variable_dict(o, registry),
+                            generate_variable_dict(o, plugin_config, registry),
                         ],
                     )
                 ),
                 attr=registry.generate_node_name(
                     o.selection_set.selections[0].name.value
                 ),
                 ctx=ast.Load(),
@@ -550,15 +550,15 @@
                 ),
                 keywords=generate_passing_extra_kwargs_for_onode(
                     definition, plugin_config
                 ),
                 args=generate_passing_extra_args_for_onode(definition, plugin_config)
                 + [
                     generate_document_arg(o, registry),
-                    generate_variable_dict(o, registry),
+                    generate_variable_dict(o, plugin_config, registry),
                 ],
             )
         )
     else:
         return ast.Return(
             value=ast.Attribute(
                 value=ast.Call(
@@ -570,15 +570,15 @@
                         definition, plugin_config
                     ),
                     args=generate_passing_extra_args_for_onode(
                         definition, plugin_config
                     )
                     + [
                         generate_document_arg(o, registry),
-                        generate_variable_dict(o, registry),
+                        generate_variable_dict(o, plugin_config, registry),
                     ],
                 ),
                 attr=registry.generate_node_name(
                     o.selection_set.selections[0].name.value
                 ),
                 ctx=ast.Load(),
             )
@@ -605,15 +605,15 @@
                 ),
                 keywords=generate_passing_extra_kwargs_for_onode(
                     definition, plugin_config
                 ),
                 args=generate_passing_extra_args_for_onode(definition, plugin_config)
                 + [
                     generate_document_arg(o, registry),
-                    generate_variable_dict(o, registry),
+                    generate_variable_dict(o, plugin_config, registry),
                 ],
             ),
             body=[
                 ast.Expr(value=ast.Yield(value=ast.Name(id="event", ctx=ast.Load()))),
             ],
             orelse=[],
         )
@@ -627,15 +627,15 @@
                 ),
                 keywords=generate_passing_extra_kwargs_for_onode(
                     definition, plugin_config
                 ),
                 args=generate_passing_extra_args_for_onode(definition, plugin_config)
                 + [
                     generate_document_arg(o, registry),
-                    generate_variable_dict(o, registry),
+                    generate_variable_dict(o, plugin_config, registry),
                 ],
             ),
             body=[
                 ast.Expr(
                     value=ast.Yield(
                         value=ast.Attribute(
                             value=ast.Name(id="event", ctx=ast.Load()),
@@ -671,15 +671,15 @@
                 ),
                 keywords=generate_passing_extra_kwargs_for_onode(
                     definition, plugin_config
                 ),
                 args=generate_passing_extra_args_for_onode(definition, plugin_config)
                 + [
                     generate_document_arg(o, registry),
-                    generate_variable_dict(o, registry),
+                    generate_variable_dict(o, plugin_config, registry),
                 ],
             ),
             body=[
                 ast.Expr(value=ast.Yield(value=ast.Name(id="event", ctx=ast.Load()))),
             ],
             orelse=[],
         )
@@ -693,15 +693,15 @@
                 ),
                 keywords=generate_passing_extra_kwargs_for_onode(
                     definition, plugin_config
                 ),
                 args=generate_passing_extra_args_for_onode(definition, plugin_config)
                 + [
                     generate_document_arg(o, registry),
-                    generate_variable_dict(o, registry),
+                    generate_variable_dict(o, plugin_config, registry),
                 ],
             ),
             body=[
                 ast.Expr(
                     value=ast.Yield(
                         value=ast.Attribute(
                             value=ast.Name(id="event", ctx=ast.Load()),
@@ -871,21 +871,19 @@
 
     def generate_ast(
         self,
         client_schema: GraphQLSchema,
         config: GeneratorConfig,
         registry: ClassRegistry,
     ) -> List[ast.AST]:
-
         plugin_tree = []
 
         documents = parse_documents(
-                client_schema, self.config.funcs_glob or config.documents
+            client_schema, self.config.funcs_glob or config.documents
         )
-       
 
         operations = [
             node
             for node in documents.definitions
             if isinstance(node, OperationDefinitionNode)
         ]
```

### Comparing `turms-0.4.2/turms/plugins/inputs.py` & `turms-0.4.3/turms/plugins/inputs.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/plugins/objects.py` & `turms-0.4.3/turms/plugins/objects.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/plugins/operations.py` & `turms-0.4.3/turms/plugins/operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,25 +38,25 @@
     query_bases: List[str] = None
     arguments_bases: List[str] = None
     mutation_bases: List[str] = None
     subscription_bases: List[str] = None
     operations_glob: Optional[str]
     create_arguments: bool = True
     extract_documentation: bool = True
+    arguments_allow_population_by_field_name: bool = False
 
     class Config:
         env_prefix = "TURMS_PLUGINS_OPERATIONS_"
 
 
 def get_query_bases(
     config: GeneratorConfig,
     plugin_config: OperationsPluginConfig,
     registry: ClassRegistry,
 ):
-
     if plugin_config.query_bases:
         for base in plugin_config.query_bases:
             registry.register_import(base)
 
         return [
             ast.Name(id=base.split(".")[-1], ctx=ast.Load())
             for base in plugin_config.query_bases
@@ -72,15 +72,14 @@
 
 
 def get_mutation_bases(
     config: GeneratorConfig,
     plugin_config: OperationsPluginConfig,
     registry: ClassRegistry,
 ):
-
     if plugin_config.mutation_bases:
         for base in plugin_config.mutation_bases:
             registry.register_import(base)
 
         return [
             ast.Name(id=base.split(".")[-1], ctx=ast.Load())
             for base in plugin_config.mutation_bases
@@ -91,20 +90,51 @@
 
             return [
                 ast.Name(id=base.split(".")[-1], ctx=ast.Load())
                 for base in config.object_bases
             ]
 
 
-def get_arguments_bases(
+def generate_arguments_config(
+    operation: OperationDefinitionNode,
     config: GeneratorConfig,
     plugin_config: OperationsPluginConfig,
     registry: ClassRegistry,
 ):
+    config_fields = []
 
+    if plugin_config.arguments_allow_population_by_field_name:
+        config_fields.append(
+            ast.Assign(
+                targets=[
+                    ast.Name(id="allow_population_by_field_name", ctx=ast.Store())
+                ],
+                value=ast.Constant(value=True),
+            )
+        )
+
+    if len(config_fields) > 0:
+        return [
+            ast.ClassDef(
+                name="Config",
+                bases=[],
+                keywords=[],
+                body=config_fields,
+                decorator_list=[],
+            )
+        ]
+    else:
+        return []
+
+
+def get_arguments_bases(
+    config: GeneratorConfig,
+    plugin_config: OperationsPluginConfig,
+    registry: ClassRegistry,
+):
     if plugin_config.arguments_bases:
         for base in plugin_config.arguments_bases:
             registry.register_import(base)
 
         return [
             ast.Name(id=base.split(".")[-1], ctx=ast.Load())
             for base in plugin_config.arguments_bases
@@ -120,15 +150,14 @@
 
 
 def get_subscription_bases(
     config: GeneratorConfig,
     plugin_config: OperationsPluginConfig,
     registry: ClassRegistry,
 ):
-
     if plugin_config.subscription_bases:
         for base in plugin_config.subscription_bases:
             registry.register_import(base)
 
         return [
             ast.Name(id=base.split(".")[-1], ctx=ast.Load())
             for base in plugin_config.subscription_bases
@@ -146,15 +175,14 @@
 def generate_operation(
     o: OperationDefinitionNode,
     client_schema: GraphQLSchema,
     config: GeneratorConfig,
     plugin_config: OperationsPluginConfig,
     registry: ClassRegistry,
 ):
-
     tree = []
     assert o.name.value, "Operation names are required"
 
     # Generation means creating a class for the operation
     if o.operation == OperationType.MUTATION:
         class_name = registry.generate_mutation(o.name.value)
         extra_bases = get_mutation_bases(config, plugin_config, registry)
@@ -197,49 +225,95 @@
             ),
         ]
 
     query_document = language.print_ast(o)
     merged_document = replace_iteratively(query_document, registry)
 
     if plugin_config.create_arguments:
-
         arguments_body = []
 
         for v in o.variable_definitions:
-            if isinstance(v.type, NonNullTypeNode) and not v.default_value:
-                arguments_body += [
-                    ast.AnnAssign(
-                        target=ast.Name(
-                            id=registry.generate_parameter_name(v.variable.name.value),
-                            ctx=ast.Store(),
+            is_optional = not isinstance(v.type, NonNullTypeNode) or v.default_value
+            annotation = recurse_type_annotation(v.type, registry)
+            field_name = registry.generate_parameter_name(v.variable.name.value)
+            target = v.variable.name.value
+
+            if target != field_name:
+                registry.register_import("pydantic.Field")
+                if is_optional:
+                    assign = ast.AnnAssign(
+                        target=ast.Name(field_name, ctx=ast.Store()),
+                        annotation=annotation,
+                        value=ast.Call(
+                            func=ast.Name(id="Field", ctx=ast.Load()),
+                            args=[],
+                            keywords=[
+                                ast.keyword(
+                                    arg="alias", value=ast.Constant(value=target)
+                                ),
+                                ast.keyword(
+                                    arg="default",
+                                    value=ast.Constant(
+                                        value=parse_value_node(v.default_value)
+                                        if v.default_value
+                                        else None
+                                    ),
+                                ),
+                            ],
                         ),
-                        annotation=recurse_type_annotation(v.type, registry),
                         simple=1,
                     )
-                ]
-
-            if not isinstance(v.type, NonNullTypeNode) or v.default_value:
-                arguments_body += [
-                    ast.AnnAssign(
-                        target=ast.Name(
-                            id=registry.generate_parameter_name(v.variable.name.value),
-                            ctx=ast.Store(),
-                        ),
-                        annotation=recurse_type_annotation(
-                            v.type,
-                            registry,
+                else:
+                    assign = ast.AnnAssign(
+                        target=ast.Name(field_name, ctx=ast.Store()),
+                        annotation=annotation,
+                        value=ast.Call(
+                            func=ast.Name(id="Field", ctx=ast.Load()),
+                            args=[],
+                            keywords=[
+                                ast.keyword(
+                                    arg="alias", value=ast.Constant(value=target)
+                                )
+                            ],
                         ),
-                        value=ast.Constant(
-                            value=parse_value_node(v.default_value)
-                            if v.default_value
-                            else None
+                        simple=1,
+                    )
+            else:
+                if is_optional:
+                    assign = ast.AnnAssign(
+                        target=ast.Name(field_name, ctx=ast.Store()),
+                        annotation=annotation,
+                        value=ast.Call(
+                            func=ast.Name(id="Field", ctx=ast.Load()),
+                            args=[],
+                            keywords=[
+                                ast.keyword(
+                                    arg="default",
+                                    value=ast.Constant(
+                                        value=parse_value_node(v.default_value)
+                                        if v.default_value
+                                        else None
+                                    ),
+                                ),
+                            ],
                         ),
                         simple=1,
                     )
-                ]
+                else:
+                    assign = ast.AnnAssign(
+                        target=ast.Name(field_name, ctx=ast.Store()),
+                        annotation=annotation,
+                        simple=1,
+                    )
+
+            arguments_body += [assign]
+
+        arguments_body + generate_arguments_config(
+            o.operation, config, plugin_config, registry
+        )
 
         class_body_fields += [
             ast.ClassDef(
                 "Arguments",
                 bases=get_arguments_bases(config, plugin_config, registry=registry),
                 decorator_list=[],
                 keywords=[],
@@ -295,15 +369,14 @@
 
     def generate_ast(
         self,
         client_schema: GraphQLSchema,
         config: GeneratorConfig,
         registry: ClassRegistry,
     ) -> List[ast.AST]:
-
         plugin_tree = []
 
         documents = parse_documents(
             client_schema, self.config.operations_glob or config.documents
         )
 
         definitions = documents.definitions
```

### Comparing `turms-0.4.2/turms/plugins/strawberry.py` & `turms-0.4.3/turms/plugins/strawberry.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,25 +145,22 @@
 
 def default_generate_enums(
     client_schema: GraphQLSchema,
     config: GeneratorConfig,
     plugin_config: "StrawberryPluginConfig",
     registry: ClassRegistry,
 ):
-
     tree = []
 
     enum_types = {
         key: value
         for key, value in client_schema.type_map.items()
         if isinstance(value, GraphQLEnumType)
     }
 
-    registry.register_import("enum.Enum")
-
     for key, type in enum_types.items():
 
         directive_keywords = generate_directive_keywords(type.ast_node, plugin_config)
         if directive_keywords:
             decorator = ast.Call(
                 func=ast.Name(id="strawberry.enum", ctx=ast.Load()),
                 keywords=directive_keywords,
@@ -209,14 +206,16 @@
                     assign,
                     ast.Expr(value=ast.Constant(value=potential_comment)),
                 ]
 
             else:
                 fields += [assign]
 
+        registry.register_import("enum.Enum")
+
         tree.append(
             ast.ClassDef(
                 classname,
                 bases=[
                     ast.Name(id="Enum", ctx=ast.Load()),
                 ],
                 decorator_list=[decorator],
@@ -393,15 +392,15 @@
                 config,
                 plugin_config,
                 registry,
                 is_optional=True,
             )
         )
 
-    raise NotImplementedError(f"Unknown input type {repr(graphql_type)}") # pragma: no cover
+    raise NotImplementedError(f"Unknown object type {repr(graphql_type)}") # pragma: no cover
 
 
 def recurse_argument_annotation(
     graphql_type: GraphQLType,
     parent: str,
     config: GeneratorConfig,
     plugin_config: StrawberryPluginConfig,
@@ -522,15 +521,15 @@
                     )
                 ),
                 ctx=ast.Load(),
             )
 
         registry.register_import("typing.List")
         return list_builder(
-            generate_object_field_annotation(
+            recurse_argument_annotation(
                 graphql_type.of_type,
                 parent,
                 config,
                 plugin_config,
                 registry,
                 is_optional=True,
             )
```

### Comparing `turms-0.4.2/turms/processors/base.py` & `turms-0.4.3/turms/processors/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/processors/black.py` & `turms-0.4.3/turms/processors/black.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/processors/disclaimer.py` & `turms-0.4.3/turms/processors/disclaimer.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/processors/isort.py` & `turms-0.4.3/turms/processors/isort.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/processors/merge.py` & `turms-0.4.3/turms/processors/merge.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/recurse.py` & `turms-0.4.3/turms/recurse.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,14 +264,18 @@
 
                 inline_fragment_fields += [
                     generate_typename_field(
                         sub_node.type_condition.name.value, registry, config
                     )
                 ]
 
+                additional_bases = get_additional_bases_for_type(
+                    sub_node.type_condition.name.value, config, registry
+                )
+
                 for sub_sub_node in sub_node.selection_set.selections:
 
                     if isinstance(sub_sub_node, FieldNode):
                         sub_sub_node_type = client_schema.get_type(
                             sub_node.type_condition.name.value
                         )
 
@@ -285,17 +289,19 @@
                             field_type,
                             client_schema,
                             config,
                             subtree,
                             registry,
                         )
 
-                additional_bases = get_additional_bases_for_type(
-                    sub_node.type_condition.name.value, config, registry
-                )
+                    elif isinstance(sub_sub_node, FragmentSpreadNode):
+                        additional_bases.append(registry.reference_fragment(
+                            sub_sub_node.name.value, parent
+                        ))
+
                 cls = ast.ClassDef(
                     inline_fragment_name,
                     bases=additional_bases
                     + [
                         ast.Name(id=mother_class_name, ctx=ast.Load()),
                     ],
                     decorator_list=[],
@@ -339,14 +345,22 @@
                 registry.register_import("typing.Union")
                 return ast.Subscript(
                     value=ast.Name("Union", ctx=ast.Load()),
                     slice=union_slice,
                     ctx=ast.Load(),
                 )
         else:
+            if is_optional:
+                registry.register_import("typing.Optional")
+
+                return ast.Subscript(
+                    value=ast.Name("Optional", ctx=ast.Load()),
+                    slice=ast.Name(id=union_class_names[0], ctx=ast.Load()),
+                    ctx=ast.Load(),
+                )
             return ast.Name(id=union_class_names[0], ctx=ast.Load())
 
     if isinstance(type, GraphQLObjectType):
         pick_fields = []
         additional_bases = get_additional_bases_for_type(type.name, config, registry)
 
         target = target_from_node(node)
```

### Comparing `turms-0.4.2/turms/referencer.py` & `turms-0.4.3/turms/referencer.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/registry.py` & `turms-0.4.3/turms/registry.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/run.py` & `turms-0.4.3/turms/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     load_introspection_from_glob,
     load_introspection_from_url,
     load_dsl_from_glob,
     load_dsl_from_url,
     import_string,
 )
 from turms.plugins.base import Plugin
+from turms.parsers.base import Parser
+from turms.processors.base import Processor
 from turms.registry import ClassRegistry
 from turms.stylers.base import Styler
 from pydantic.error_wrappers import ValidationError
 
 from .errors import GenerationError
 import json
 import os
@@ -151,15 +153,14 @@
             f"Multiple config files found in {folder_path}. Please only have one of {SCANNABLE_FILE_NAMES}. Or use the --config flag to specify a config file."
         )
 
     return configs[0]
 
 
 def write_code_to_file(code: str, outdir: str, filepath: str):
-
     if not os.path.isdir(outdir):  # pragma: no cover
         os.makedirs(outdir)
 
     generated_file = os.path.join(
         outdir,
         filepath,
     )
@@ -238,15 +239,14 @@
     Args:
         project (GraphQLProject): The project
 
     Returns:
         GraphQLSchema: The schema
     """
     if isinstance(schema, dict):
-
         if len(schema.values()) == 1:
             key, value = list(schema.items())[0]
             try:
                 dsl_string = load_dsl_from_url(key, value.headers)
                 return build_ast_schema(parse(dsl_string))
             except Exception as e:
                 if allow_introspection:
@@ -373,23 +373,23 @@
         schema,
         plugins=plugins,
         stylers=stylers,
         skip_forwards=gen_config.skip_forwards,
         log=log,
     )
 
-    for styler in parsers:
-        generated_ast = styler.parse_ast(generated_ast)
-
-    generated = parse_asts_to_string(generated_ast)
-
-    for processor in processors:
-        generated = processor.run(generated, gen_config)
-
-    return generated
+    return generate_code(
+        gen_config,
+        schema,
+        plugins=plugins,
+        stylers=stylers,
+        parsers=parsers,
+        processors=processors,
+        log=log,
+    )
 
 
 def parse_asts_to_string(generated_ast: List[ast.AST]) -> str:
     module = ast.Module(body=generated_ast, type_ignores=[])
     return ast.unparse(ast.fix_missing_locations(module))
 
 
@@ -433,7 +433,99 @@
     global_tree = (
         registry.generate_imports() + registry.generate_builtins() + global_tree
     )
     if not skip_forwards:
         global_tree += registry.generate_forward_refs()
 
     return global_tree
+
+
+def parse_ast(
+    config: GeneratorConfig,
+    ast: List[ast.AST],
+    parsers: Optional[List[Parser]] = None,
+    log: LogFunction = lambda *args, **kwargs: print,
+) -> List[ast.AST]:
+    """Parses the ast with the plugins
+
+    Args:
+        ast (List[ast.AST]): The ast to parse
+        plugins (Optional[List[Plugin]], optional): The plugins to use. Defaults to [].
+        stylers (Optional[List[Styler]], optional): The plugins to use. Defaults to [].
+
+    Raises:
+        GenerationError: Errors involving the generation of the ast
+
+    Returns:
+        List[ast.AST]: The parsed ast (as list, not as module)
+    """
+
+    parsers = parsers or []
+
+    for parser in parsers:
+        try:
+            ast = parser.parse_ast(ast)
+        except Exception as e:
+            raise GenerationError(
+                f"{parser.__class__.__name__} failed!\n {str(e)}"
+            ) from e
+
+    return ast
+
+
+def process_code(
+    config: GeneratorConfig,
+    code: List[ast.AST],
+    processors: Optional[List[Processor]] = None,
+    log: LogFunction = lambda *args, **kwargs: print,
+) -> List[ast.AST]:
+    """Parses the ast with the plugins
+
+    Args:
+        ast (List[ast.AST]): The ast to parse
+        plugins (Optional[List[Plugin]], optional): The plugins to use. Defaults to [].
+        stylers (Optional[List[Styler]], optional): The plugins to use. Defaults to [].
+
+    Raises:
+        GenerationError: Errors involving the generation of the ast
+
+    Returns:
+        List[ast.AST]: The parsed ast (as list, not as module)
+    """
+
+    processors = processors or []
+
+    for processor in processors:
+        try:
+            code = processor.run(code, config)
+        except Exception as e:
+            raise GenerationError(
+                f"{processor.__class__.__name__} failed!\n {str(e)}"
+            ) from e
+
+    return code
+
+
+def generate_code(
+    config: GeneratorConfig,
+    schema: GraphQLSchema,
+    plugins: Optional[List[Plugin]] = None,
+    stylers: Optional[List[Styler]] = None,
+    parsers: Optional[List[Parser]] = None,
+    processors: Optional[List[Processor]] = None,
+    log: LogFunction = lambda *args, **kwargs: print,
+) -> str:
+    generated_ast = generate_ast(
+        config,
+        schema,
+        plugins=plugins,
+        stylers=stylers,
+        skip_forwards=config.skip_forwards,
+        log=log,
+    )
+
+    parsed_ast = parse_ast(config, generated_ast, parsers=parsers, log=log)
+    code = parse_asts_to_string(parsed_ast)
+
+    processed_code = process_code(config, code, processors=processors, log=log)
+
+    return processed_code
```

### Comparing `turms-0.4.2/turms/stylers/appender.py` & `turms-0.4.3/turms/stylers/appender.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/stylers/base.py` & `turms-0.4.3/turms/stylers/base.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/stylers/capitalize.py` & `turms-0.4.3/turms/stylers/capitalize.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/stylers/default.py` & `turms-0.4.3/turms/stylers/default.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/stylers/snake_case.py` & `turms-0.4.3/turms/stylers/snake_case.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/turms/utils.py` & `turms-0.4.3/turms/utils.py`

 * *Files identical despite different names*

### Comparing `turms-0.4.2/PKG-INFO` & `turms-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turms
-Version: 0.4.2
+Version: 0.4.3
 Summary: graphql-codegen powered by pydantic
 Home-page: https://jhnnsrs.github.io/turms
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 6 - Mature
```

