# Comparing `tmp/qtgql-0.124.0.tar.gz` & `tmp/qtgql-0.125.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.124.0.tar", max compression
+gzip compressed data, was "qtgql-0.125.0.tar", max compression
```

## Comparing `qtgql-0.124.0.tar` & `qtgql-0.125.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1064 2023-07-04 13:43:19.926438 qtgql-0.124.0/LICENSE
--rw-r--r--   0        0        0     1055 2023-07-04 13:43:19.926438 qtgql-0.124.0/README.md
--rw-r--r--   0        0        0     4428 2023-07-04 13:43:39.250570 qtgql-0.124.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1939 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1548 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3091 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-07-04 13:43:19.938439 qtgql-0.124.0/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     3961 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    15274 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0      749 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0        0 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4164 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1704 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3573 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     1850 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0      448 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
--rw-r--r--   0        0        0     1051 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4641 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     2645 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
--rw-r--r--   0        0        0     3884 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     4956 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3231 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    17078 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1147 2023-07-04 13:43:19.942439 qtgql-0.124.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.124.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-05 14:38:49.517554 qtgql-0.125.0/LICENSE
+-rw-r--r--   0        0        0     1055 2023-07-05 14:38:49.517554 qtgql-0.125.0/README.md
+-rw-r--r--   0        0        0     4428 2023-07-05 14:39:11.521675 qtgql-0.125.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1939 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1685 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3091 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     3366 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    14721 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0      864 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4164 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1704 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3347 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     1890 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0     1072 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4706 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     2677 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     3913 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     5150 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3237 2023-07-05 14:38:49.529554 qtgql-0.125.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    18075 2023-07-05 14:38:49.533554 qtgql-0.125.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1147 2023-07-05 14:38:49.533554 qtgql-0.125.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.125.0/PKG-INFO
```

### Comparing `qtgql-0.124.0/LICENSE` & `qtgql-0.125.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/README.md` & `qtgql-0.125.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/pyproject.toml` & `qtgql-0.125.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.124.0"
+version = "0.125.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/cli.py` & `qtgql-0.125.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/qtgqlcodegen/config.py` & `qtgql-0.125.0/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/qtgqlcodegen/core/cppref.py` & `qtgql-0.125.0/qtgqlcodegen/core/cppref.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,14 +43,20 @@
             return f"{self.attr}{self.inner.accessor}{self.inner.attr.build()}"
         return self.attr
 
     @cached_property
     def name(self) -> str:
         return self.build()
 
+    @cached_property
+    def last(self) -> str:
+        if self.inner:
+            return self.inner.attr.last
+        return self.attr
+
 
 def QtGqlNs() -> CppAttribute:
     return CppAttribute(
         attr="qtgql",
     )
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.125.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/qtgqlcodegen/core/template.py` & `qtgql-0.125.0/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/qtgqlcodegen/generator.py` & `qtgql-0.125.0/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/qtgqlcodegen/operation/definitions.py` & `qtgql-0.125.0/qtgqlcodegen/operation/definitions.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,34 +51,14 @@
         return self.origin.name in self.type_info.schema_type_info.root_types_names
 
     @cached_property
     def type_name(self) -> str:
         return self.type.member_type
 
     @cached_property
-    def property_type(self) -> str:
-        """
-
-        :return: C++ property type that will be exposed to QML.
-        """
-        tp = self.type
-        if tp.is_queried_object_type or tp.is_queried_interface:
-            return f"{self.type_name} *"
-
-        if cs := tp.is_custom_scalar:
-            return cs.to_qt_type
-
-        if model := tp.is_model:
-            if model.of_type.is_queried_object_type:
-                return f"qtgql::bases::ListModelABC<{model.of_type.type_name()}> *"
-            raise NotImplementedError
-
-        return f"{self.type_name} &"
-
-    @cached_property
     def build_variables_tuple_for_field_arguments(self) -> str:
         # operation might not use an argument that has default value, ignore what's ignored.
         # see https://github.com/qtgql/qtgql/issues/272 for more details.
         if self.cached_by_args and self.variable_uses:
             assert len(self.concrete.arguments) == len(self.variable_uses)
             return (
                 "{"
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.125.0/qtgqlcodegen/operation/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-from collections import defaultdict
 from typing import TYPE_CHECKING
 
 import graphql
 from graphql import OperationDefinitionNode, OperationType, language as gql_lang
 from graphql.language import visitor
 
 from qtgqlcodegen.core.graphql_ref import (
@@ -191,42 +190,35 @@
 
 def _evaluate_union(
     type_info: OperationTypeInfo,
     concrete: QtGqlUnion,
     selection_set: gql_lang.SelectionSetNode,
     path: str,
 ) -> QtGqlQueriedUnion:
-    choices: defaultdict[str, dict[str, QtGqlQueriedField]] = defaultdict(dict)
+    choices: dict[str, QtGqlQueriedObjectType] = {}
+    if not has_typename_selection(selection_set):
+        inject_typename_selection(selection_set)
     for selection in selection_set.selections:
+        if is_field_node(selection):
+            continue  # __typename selection
         fragment = is_inline_fragment(selection)
         assert fragment
         type_name = fragment.type_condition.name.value
         # unions support only object types http://spec.graphql.org/October2021/#sec-Unions
         resolved_type = require(concrete.get_by_name(type_name))
-        if not has_typename_selection(fragment.selection_set):
-            inject_typename_selection(fragment.selection_set)
-        if not has_id_selection(fragment.selection_set) and resolved_type.implements_node:
-            inject_id_selection(fragment.selection_set)
-
-        for selection_node in fragment.selection_set.selections:
-            inner_field_node = require(is_field_node(selection_node))
-            if not is_type_name_selection(inner_field_node):
-                concrete_field = resolved_type.fields_dict[inner_field_node.name.value]
-                __f = _evaluate_field(
-                    type_info=type_info,
-                    concrete_field=concrete_field,
-                    field_node=inner_field_node,
-                    path=path,
-                    origin=resolved_type,
-                )
-                choices[type_name][concrete_field.name] = __f
+        choices[type_name] = _evaluate_object_type(
+            type_info=type_info,
+            concrete=resolved_type,
+            selection_set=fragment.selection_set,
+            path=path,
+        )
 
     return QtGqlQueriedUnion(
         concrete=concrete,
-        choices=choices,
+        choices=tuple(choices.values()),
     )
 
 
 def _unwrap_interface_fragments(
     type_info: SchemaTypeInfo,
     parent_concrete: QtGqlObjectType | QtGqlInterface,
     selection_set: gql_lang.SelectionSetNode,
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/operation/template.py` & `qtgql-0.125.0/qtgqlcodegen/operation/template.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, ClassVar
 
 from attr import define
 
+from qtgqlcodegen.core.cppref import QtGqlTypes
 from qtgqlcodegen.core.template import template_env
 
 if TYPE_CHECKING:
     from qtgqlcodegen.config import QtGqlConfig
     from qtgqlcodegen.operation.definitions import QtGqlOperationDefinition
 
 
 @define(slots=False)
 class OperationTemplateContext:
     operation: QtGqlOperationDefinition
     config: QtGqlConfig
     debug: bool = False
+    qtgql_types: ClassVar[type[QtGqlTypes]] = QtGqlTypes
 
     @property
     def ns(self) -> str:
         return self.operation.name.lower()
 
     @property
     def schema_ns(self) -> str:
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/schema/definitions.py` & `qtgql-0.125.0/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.125.0/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/qtgqlcodegen/schema/template.py` & `qtgql-0.125.0/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.125.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.125.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 , 👉proxy_field.build_variables_tuple_for_field_arguments👈
 {% endif -%}
 {% endset -%}
 if (!data.value("👉proxy_field.name👈").isNull()){
 {% if proxy_field.type.is_queried_object_type -%}
 👉 setter_name 👈(👉proxy_field.type.deserializer_name👈(data.value("👉proxy_field.name👈").toObject(), 👉operation_pointer👈) 👉 setter_end 👈);
 
-{% elif proxy_field.type.is_queried_interface -%}
+{% elif proxy_field.type.is_queried_interface or  proxy_field.type.is_queried_union -%}
 auto 👉proxy_field.name👈_data = data.value("👉proxy_field.name👈").toObject();
 auto 👉proxy_field.name👈_typename  = 👉proxy_field.name👈_data.value("__typename").toString();
 {%set type_cond -%}👉proxy_field.name👈_typename{% endset -%}
 {% for choice in proxy_field.type.choices -%}
 {% set do_on_meets -%}
 👉 setter_name 👈(👉choice.deserializer_name👈(👉proxy_field.name👈_data, 👉operation_pointer👈) 👉 setter_end 👈);
 {% endset -%}
@@ -24,15 +24,14 @@
 {% elif proxy_field.type.is_model -%}
 {% if proxy_field.type.is_model.of_type.is_queried_object_type -%}
 👉proxy_field.concrete.type.member_type👈 obj_list;
 for (const auto& node: data.value("👉proxy_field.name👈").toArray()){
 obj_list.append(👉 proxy_field.type.is_model.of_type.is_queried_object_type.deserializer_name 👈(node.toObject(), 👉operation_pointer👈));
 };
 👉 setter_name 👈(obj_list👉 setter_end 👈);
-
 {% elif proxy_field.type.is_model.is_interface -%}
 👉 setter_name 👈(qtgql::ListModel(
         parent=parent,
         data=[👉proxy_field.type.is_model.is_interface.name👈.from_dict(parent, data=node, config=inner_config, metadata=👉operation_pointer👈) for
 node in field_data],)👉 setter_end 👈);
 {% elif proxy_field.type.is_model.is_union -%}
 model_data = []
@@ -53,14 +52,10 @@
 {% endif %}
 {% elif proxy_field.type.is_custom_scalar -%}
 auto new_👉proxy_field.name👈 = 👉 proxy_field.type.is_custom_scalar.type_name() 👈();
 new_👉proxy_field.name👈.deserialize(data.value("👉proxy_field.name👈"));
 👉 setter_name 👈(new_👉proxy_field.name👈 👉 setter_end 👈);
 {% elif proxy_field.type.is_enum -%}
 👉 setter_name 👈(Enums::👉proxy_field.type.is_enum.map_name👈::by_name(data.value("👉proxy_field.name👈").toString())👉 setter_end 👈);
-{% elif proxy_field.type.is_union -%}
-type_name = field_data['__typename']
-choice = inner_👉config_name👈.choices[type_name]
-👉 setter_name 👈(__TYPE_MAP__[type_name].from_dict(parent, field_data, choice, 👉operation_pointer👈)👉 setter_end 👈);;
 {% endif -%} 👉 do_after_deserialized 👈
 };
 {%- endmacro %}
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.125.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 👉field.private_name👈 = new 👉field.type_name👈(👉operation_pointer👈, 👉 instance_of_concrete 👈);
 {% elif field.type.is_model and field.type.is_model.of_type.is_queried_object_type %}
 auto init_list_👉 field.name 👈 =  std::make_unique<QList<👉field.type.of_type.name👈*>>();
 for (const auto & node: 👉 instance_of_concrete 👈){
 init_list_👉 field.name 👈->append(new 👉field.type.of_type.name👈(👉operation_pointer👈, node));
 }
 👉field.private_name👈 = new qtgql::bases::ListModelABC<👉 field.type.of_type.name 👈>(this, std::move(init_list_👉 field.name 👈));
-{% elif field.type.is_queried_interface %}
+{% elif field.type.is_queried_interface or  field.type.is_queried_union %}
 auto concrete_👉field.name👈 = 👉 instance_of_concrete 👈;
 auto 👉field.name👈_typename = concrete_👉field.name👈->__typename();
 {%set type_cond -%}👉field.name👈_typename{% endset -%}
 {% for choice in field.type.choices -%}
 {% set do_on_meets -%}
-👉field.private_name👈 = qobject_cast<👉 field.type.name 👈*>(new 👉choice.type_name()👈(👉operation_pointer👈, std::static_pointer_cast<👉 choice.concrete.name 👈>(concrete_👉field.name👈)));
+👉field.private_name👈 = qobject_cast<👉 field.type.property_type 👈>(new 👉choice.type_name()👈(👉operation_pointer👈, std::static_pointer_cast<👉 choice.concrete.name 👈>(concrete_👉field.name👈)));
 {% endset -%}
 👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
 {% endfor %}
 {% endif -%}
 {% endmacro -%}
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp` & `qtgql-0.125.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% macro proxy_type_fields(t, context) -%}
 Q_OBJECT
 Q_PROPERTY(QString  __typeName READ __typename CONSTANT)
 
 {% for f in t.fields -%}
-Q_PROPERTY(const 👉 f.property_type 👈 👉 f.name 👈 READ 👉 f.concrete.getter_name 👈 NOTIFY 👉 f.concrete.signal_name 👈);
+Q_PROPERTY(const 👉 f.type.property_type 👈 👉 f.name 👈 READ 👉 f.concrete.getter_name 👈 NOTIFY 👉 f.concrete.signal_name 👈);
 {% endfor %}
 signals:
 {%for f in t.fields -%}
 void 👉 f.concrete.signal_name 👈();
 {% endfor %}
 {# members -#}
 {% if context.debug -%}
@@ -17,13 +17,13 @@
 {% endif -%}
 {% if t.concrete.is_root -%} {# // root types are singletons, no need for shared ptr -#}
 👉context.schema_ns👈::👉 t.concrete.name 👈 * m_inst;
 {% else -%}
 const std::shared_ptr<👉context.schema_ns👈::👉 t.concrete.name 👈> m_inst;
 {% endif -%}
 {% for ref_field in t.references -%}
-const 👉ref_field.property_type👈 m_👉ref_field.name👈 = {};
+const 👉ref_field.type.property_type👈 👉ref_field.private_name👈 = {};
 {% endfor %}
 {%- for model_field in t.models -%}
-👉 model_field.property_type 👈 👉model_field.private_name👈;
+👉 model_field.type.property_type 👈 👉model_field.private_name👈;
 {% endfor %}
 {% endmacro %}
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.125.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {% set setter_end -%}
 {% if proxy_field.variable_uses -%}
 , 👉private_name👈_args
 {% endif -%}
 {%- endset -%}
 {%- set setter_name -%}inst->👉 proxy_field.concrete.setter_name 👈{% endset -%}
 
-{%- if proxy_field.is_root and f_concrete.type.is_object_type or f_concrete.type.is_interface -%}
+{%- if proxy_field.is_root and f_concrete.type.is_object_type or f_concrete.type.is_interface or f_concrete.type.is_union -%}
 {#- // root fields that has no default value might not have value even if they are not optional -#}
 {% if proxy_field.variable_uses  -%}
 if (!inst->👉private_name👈.contains(👉private_name👈_args))
 {% else -%}
 if (!👉current👈)
 {% endif %}
 {
@@ -62,15 +62,15 @@
 {% elif proxy_field.type.is_model %}
 👉deserialize_concrete_field(proxy_field)👈
 {% elif proxy_field.type.is_enum %}
 auto new_👉f_concrete.name👈= Enums::👉proxy_field.type.is_enum.map_name👈::by_name(data.value("👉proxy_field.name👈").toString());
 if (👉current👈 != new_👉f_concrete.name👈){
 👉 setter_name 👈(new_👉f_concrete.name👈 👉 setter_end 👈);
 }
-{% elif proxy_field.type.is_queried_interface %}
+{% elif proxy_field.type.is_queried_interface or proxy_field.type.is_queried_union %}
 auto 👉f_concrete.name👈_data = data.value("👉f_concrete.name👈").toObject();
 auto 👉f_concrete.name👈_typename  = 👉f_concrete.name👈_data.value("__typename").toString();
 {%set type_cond -%}👉f_concrete.name👈_typename{% endset -%}
 {% for choice in proxy_field.type.choices %}
 {% set do_on_meets -%}
 {% if choice.implements_node %}
 if (👉current👈 && 👉current👈->get_id() == 👉f_concrete.name👈_data.value("id").toString()){
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp` & `qtgql-0.125.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -31,23 +31,23 @@
     {% endif %}
 {% elif field.type.is_queried_object_type -%}
 auto operation = qobject_cast<👉operation.name👈*>(this->parent());
 auto concrete = 👉new_concrete👈;
 delete 👉field.private_name👈;
 👉field.private_name👈 = new 👉field.type.name👈(operation, concrete);
 emit 👉 field.concrete.signal_name 👈();
-{% elif field.type.is_queried_interface -%}
+{% elif field.type.is_queried_interface or field.type.is_queried_union -%}
 auto operation = qobject_cast<👉operation.name👈*>(this->parent());
 auto concrete = 👉new_concrete👈;
 delete 👉field.private_name👈;
 auto 👉field.name👈_typename = concrete->__typename();
 {%set type_cond -%}👉field.name👈_typename{% endset -%}
 {% for choice in field.type.choices %}
 {% set do_on_meets -%}
-👉field.private_name👈 = qobject_cast<const 👉field.type.name👈 *>(new 👉choice.name👈(operation, std::static_pointer_cast<👉choice.concrete.name👈>(concrete)));
+👉field.private_name👈 = qobject_cast<👉field.type.property_type👈>(new 👉choice.name👈(operation, std::static_pointer_cast<👉choice.concrete.name👈>(concrete)));
 {% endset -%}
 👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
 {% endfor %}
 emit 👉 field.concrete.signal_name 👈();
 {% else -%}
 emit 👉 field.concrete.signal_name 👈();
 {% endif -%}
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.125.0/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 }
 {% endfor %}
 
 
 {% for t in context.operation.narrowed_types -%}
 // Constructor
 {% set base_name -%}
-👉 "QObject" if not t.base_interface else t.base_interface.name 👈
+👉 context.qtgql_types.ObjectTypeABC.last if not t.base_interface else t.base_interface.name 👈
 {% endset -%}
 {% if t.concrete.is_root -%}
 👉 t.name 👈::👉 t.name 👈(👉 context.operation.name 👈 * operation): 👉 base_name 👈::👉 base_name 👈(operation){
     m_inst = 👉 t.concrete.name 👈::instance();
     auto m_inst_ptr = m_inst;
 {% else -%}
     👉 t.name 👈::👉 t.name 👈(👉 context.operation.name 👈 * operation, const std::shared_ptr<👉 t.concrete.name 👈> &inst)
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.125.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -21,44 +21,44 @@
 {% for t in context.operation.narrowed_types -%}
 void update_👉 t.name 👈(👉 t.concrete.member_type_arg 👈 inst, const QJsonObject &data, const 👉 context.operation.name 👈 * operation);
 {% endfor -%}
 };
 
 // ------------ Narrowed Interfaces ------------
 {% for t in context.operation.interfaces -%}
-class 👉 t.name 👈: public QObject{
+class 👉 t.name 👈: public 👉 context.qtgql_types.ObjectTypeABC.name 👈{
 👉 proxy_type_fields(t, context) 👈
 public:
-    using QObject::QObject;
+    using 👉 context.qtgql_types.ObjectTypeABC.name 👈::👉 context.qtgql_types.ObjectTypeABC.last 👈;
 {% for f in t.fields -%}
-[[nodiscard]] inline virtual const 👉 f.property_type 👈  👉 f.concrete.getter_name 👈() const {
+[[nodiscard]] inline virtual const 👉 f.type.property_type 👈  👉 f.concrete.getter_name 👈() const {
 throw qtgql::exceptions::InterfaceDirectAccessError("👉t.concrete.name👈");
 }
 {% endfor %}
 public:
 [[nodiscard]] virtual const QString & __typename() const{
     throw qtgql::exceptions::InterfaceDirectAccessError("👉t.concrete.name👈");
 }
 };
 {% endfor %}
 // ------------ Narrowed Object types ------------
 {% for t in context.operation.narrowed_types %}
-class 👉 t.name 👈: public 👉 "QObject" if not t.base_interface else t.base_interface.name 👈{
+class 👉 t.name 👈: public 👉 context.qtgql_types.ObjectTypeABC.name if not t.base_interface else t.base_interface.name 👈{
 👉 proxy_type_fields(t, context) 👈
 public:
 {% if t.concrete.is_root -%}
 👉 t.name 👈(👉 context.operation.name 👈 * operation);
 {% else -%}
 👉 t.name 👈(👉 context.operation.name 👈 * operation, const std::shared_ptr<👉 t.concrete.name 👈> &inst);
 {% endif %}
 public:
 {% for f in t.fields -%}
-[[nodiscard]] inline const 👉 f.property_type 👈  👉 f.concrete.getter_name 👈() const {
-{%- if f.type.is_queried_object_type or f.type.is_model or f.type.is_queried_interface %}
-return m_👉f.name👈;
+[[nodiscard]] inline const 👉 f.type.property_type 👈  👉 f.concrete.getter_name 👈() const {
+{% if f.type.is_queried_object_type or f.type.is_model or f.type.is_queried_interface or f.type.is_queried_union %}
+return 👉f.private_name👈;
 {%- else -%}
 return m_inst->👉 f.concrete.getter_name 👈();
 {%- endif -%}
 };
 {% endfor -%}
 public:
 [[nodiscard]] const QString & __typename() const {% if t.base_interface -%}final{% endif %}{
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.125.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 {% else %}
 QTGQL_STATIC_MAKE_SHARED(👉 type.name 👈)
 {% endif %}
 
 👉 type.name 👈()= default;
 
 public:
-inline const QString & __typename() final{
+inline const QString & __typename() const final{
 static const QString ret = "👉 type.name 👈";
 return ret;
 };
 };
 {% endfor %}
 
 }
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/types.py` & `qtgql-0.125.0/qtgqlcodegen/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from collections import defaultdict
 from functools import cached_property
 from typing import TYPE_CHECKING, cast
 
 import attrs
 from attr import define
 
 from qtgqlcodegen.core.cppref import CppAttribute, QtGqlBasesNs, QtGqlTypes
@@ -76,14 +75,21 @@
     def type_name(self) -> str:
         """
         :returns: The C++ "real" type mostly this would be the member type as well.
         """
         raise NotImplementedError
 
     @property
+    def property_type(self) -> str:
+        """
+        :return: The QProperty type, usually will lay in the proxy.
+        """
+        return f"{self.type_name()} &"  # default for scalars this should suffice.
+
+    @property
     def default_value(self) -> str:
         """
 
         :return: C++ default value initializer for this type
         """
         return "{}"
 
@@ -154,29 +160,39 @@
         return f"QList<{self.of_type.member_type}>"
 
     def type_name(self) -> str:
         raise NotImplementedError(
             "models have no valid type for schema concretes, call member_type",
         )
 
+    @property
+    def property_type(self) -> str:
+        if self.of_type.is_queried_object_type:
+            return f"qtgql::bases::ListModelABC<{self.of_type.type_name()}> *"
+        raise NotImplementedError
+
 
 @define
 class QtGqlUnion(QtGqlTypeABC):
     types: tuple[QtGqlObjectType | QtGqlDeferredType, ...]
 
     @property
     def is_union(self) -> QtGqlUnion | None:
         return self
 
     def type_name(self) -> str:
-        raise NotImplementedError
+        return f"{QtGqlTypes.ObjectTypeABC.name}"
+
+    @property
+    def member_type(self) -> str:
+        return f"std::shared_ptr<{self.type_name()}>"
 
     @property
     def default_value(self) -> str:
-        raise NotImplementedError
+        return "{}"
 
     def get_by_name(self, name: str) -> QtGqlObjectType | None:
         for possible in self.types:
             if possible.name == name:
                 return cast(QtGqlObjectType, possible)
 
 
@@ -228,14 +244,18 @@
     def fget_type(self) -> str:
         return self.to_qt_type
 
     @property
     def getter_is_constable(self) -> bool:
         return False
 
+    @property
+    def property_type(self) -> str:
+        return self.to_qt_type
+
 
 @define(slots=False)
 class BaseQtGqlObjectType(QtGqlTypeABC):
     name: str
     fields_dict: dict[str, QtGqlFieldDefinition]
     docstring: str | None = ""
 
@@ -423,15 +443,15 @@
         return f"{self.namespaced_name}(0)"
 
     def json_repr(self, attr_name: str | None = None) -> str:
         return f"Enums::{self.map_name}::name_by_value({attr_name})"
 
 
 @define
-class QtGqlQueriedTypeABC:
+class QtGqlQueriedTypeABC(ABC):
     concrete: QtGqlTypeABC
 
 
 @define(slots=False, repr=False)
 class QtGqlQueriedObjectType(QtGqlQueriedTypeABC, QtGqlTypeABC):
     name: str
     concrete: QtGqlObjectType
@@ -457,18 +477,32 @@
     @property
     def updater_name(self) -> str:
         return f"updaters::update_{self.name}"
 
     def type_name(self) -> str:
         return self.name
 
+    @property
+    def property_type(self) -> str:
+        return f"{self.type_name()} *"
+
     @cached_property
     def references(self) -> list[QtGqlQueriedField]:
+        """
+        :return: Fields that should be treated with special care by the operation.
+        They can't just return the field of the concrete.
+        """
         return [
-            f for f in self.fields if f.type.is_queried_object_type or f.type.is_queried_interface
+            f
+            for f in self.fields
+            if (
+                f.type.is_queried_object_type
+                or f.type.is_queried_interface
+                or f.type.is_queried_union
+            )
         ]
 
     @cached_property
     def models(self) -> list[QtGqlQueriedField]:
         return [f for f in self.fields if f.type.is_model]
 
     @cached_property
@@ -488,25 +522,27 @@
     def is_queried_interface(self) -> QtGqlQueriedInterface | None:
         return self
 
 
 @define(slots=False, repr=False)
 class QtGqlQueriedUnion(QtGqlQueriedTypeABC, QtGqlTypeABC):
     concrete: QtGqlUnion
-    choices: defaultdict[str, dict[str, QtGqlQueriedField]] = attrs.Factory(
-        lambda: defaultdict(dict),
-    )
+    choices: tuple[QtGqlQueriedObjectType, ...]
 
     @property
     def is_queried_union(self) -> QtGqlQueriedUnion | None:
         return self
 
     def type_name(self) -> str:
         return self.concrete.type_name()
 
+    @property
+    def property_type(self) -> str:
+        return f"{QtGqlTypes.ObjectTypeABC.name} *"
+
 
 def ScalarsNs() -> CppAttribute:
     return QtGqlBasesNs().ns_add("scalars")
 
 
 def DefaultsNs() -> CppAttribute:
     return QtGqlBasesNs().ns_add("DEFAULTS")
```

### Comparing `qtgql-0.124.0/qtgqlcodegen/utils.py` & `qtgql-0.125.0/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.124.0/PKG-INFO` & `qtgql-0.125.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.124.0
+Version: 0.125.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

