# Comparing `tmp/ome_types-0.4.0a3.tar.gz` & `tmp/ome_types-0.4.0a4.tar.gz`

## Comparing `ome_types-0.4.0a3.tar` & `ome_types-0.4.0a4.tar`

### file list

```diff
@@ -1,42 +1,44 @@
--rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_autogen/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_autogen/__main__.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_autogen/_config.py
--rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_autogen/_generator.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_autogen/_transformer.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_autogen/_util.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_autogen/main.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/__init__.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/_conversion.py
--rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/ome-2016-06.xsd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/py.typed
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/units.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/_mixins/__init__.py
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/_mixins/_base_type.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/_mixins/_bin_data.py
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/_mixins/_ids.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/_mixins/_instrument.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/_mixins/_ome.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/_mixins/_reference.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/_mixins/_structured_annotations.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/_mixins/_util.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/model/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/model/_color.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/model/_shape_union.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/model/_user_sequence.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/ome_types/model/simple_types.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/xsdata_pydantic_basemodel/__init__.py
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/xsdata_pydantic_basemodel/bindings.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/xsdata_pydantic_basemodel/compat.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/xsdata_pydantic_basemodel/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/xsdata_pydantic_basemodel/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/xsdata_pydantic_basemodel/hooks/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/xsdata_pydantic_basemodel/hooks/class_type.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/src/xsdata_pydantic_basemodel/hooks/cli.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/LICENSE
--rw-r--r--   0        0        0     9347 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/README.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/hatch_build.py
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/pyproject.toml
--rw-r--r--   0        0        0    11283 2020-02-02 00:00:00.000000 ome_types-0.4.0a3/PKG-INFO
+-rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_autogen/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_autogen/__main__.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_autogen/_config.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_autogen/_generator.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_autogen/_transformer.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_autogen/_util.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_autogen/main.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/__init__.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/_conversion.py
+-rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/ome-2016-06.xsd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/py.typed
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/units.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/_mixins/__init__.py
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/_mixins/_base_type.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/_mixins/_bin_data.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/_mixins/_ids.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/_mixins/_instrument.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/_mixins/_ome.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/_mixins/_pixels.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/_mixins/_reference.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/_mixins/_util.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/model/__init__.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/model/_color.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/model/_converters.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/model/_shape_union.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/model/_structured_annotations.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/model/_user_sequence.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/ome_types/model/simple_types.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/xsdata_pydantic_basemodel/__init__.py
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/xsdata_pydantic_basemodel/bindings.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/xsdata_pydantic_basemodel/compat.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/xsdata_pydantic_basemodel/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/xsdata_pydantic_basemodel/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/xsdata_pydantic_basemodel/hooks/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/xsdata_pydantic_basemodel/hooks/class_type.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/src/xsdata_pydantic_basemodel/hooks/cli.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/LICENSE
+-rw-r--r--   0        0        0     9347 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/hatch_build.py
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/pyproject.toml
+-rw-r--r--   0        0        0    11283 2020-02-02 00:00:00.000000 ome_types-0.4.0a4/PKG-INFO
```

### Comparing `ome_types-0.4.0a3/CHANGELOG.md` & `ome_types-0.4.0a4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_autogen/_config.py` & `ome_types-0.4.0a4/src/ome_autogen/_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,15 @@
 MIXIN_MODULE = "ome_types._mixins"
 MIXINS: list[tuple[str, str, bool]] = [
     (".*", f"{MIXIN_MODULE}._base_type.OMEType", False),  # base type on every class
     ("OME", f"{MIXIN_MODULE}._ome.OMEMixin", True),
     ("Instrument", f"{MIXIN_MODULE}._instrument.InstrumentMixin", False),
     ("Reference", f"{MIXIN_MODULE}._reference.ReferenceMixin", True),
     ("BinData", f"{MIXIN_MODULE}._bin_data.BinDataMixin", True),
-    (
-        "StructuredAnnotations",
-        f"{MIXIN_MODULE}._structured_annotations.StructuredAnnotationsMixin",
-        True,
-    ),
+    ("Pixels", f"{MIXIN_MODULE}._pixels.PixelsMixin", True),
 ]
 
 ALLOW_RESERVED_NAMES = {"type", "Type", "Union"}
 OME_FORMAT = "OME"
 
 
 def get_config(
```

### Comparing `ome_types-0.4.0a3/src/ome_autogen/_generator.py` & `ome_types-0.4.0a4/src/ome_autogen/_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,36 @@
 
 
 # from ome_types._mixins._base_type import AUTO_SEQUENCE
 # avoiding import to avoid build-time dependency on the ome-types package
 AUTO_SEQUENCE = "__auto_sequence__"
 
 
+class Override(NamedTuple):
+    element_name: str
+    class_name: str
+    module_name: str | None
+
+
+CLASS_OVERRIDES = [
+    Override("Color", "Color", "ome_types.model._color"),
+    Override("Union", "ShapeUnion", "ome_types.model._shape_union"),
+    Override(
+        "StructuredAnnotations",
+        "StructuredAnnotationList",
+        "ome_types.model._structured_annotations",
+    ),
+]
+IMPORT_PATTERNS = {
+    o.module_name: {o.class_name: [f": {o.class_name} ="]}
+    for o in CLASS_OVERRIDES
+    if o.module_name
+}
+
+
 class OmeGenerator(DataclassGenerator):
     @classmethod
     def init_filters(cls, config: GeneratorConfig) -> Filters:
         return OmeFilters(config)
 
     def render_module(
         self, resolver: DependenciesResolver, classes: list[Class]
@@ -52,27 +74,14 @@
 
         if aliases:
             mod += "\n\n" + "\n".join(aliases) + "\n"
 
         return mod
 
 
-class Override(NamedTuple):
-    element_name: str
-    class_name: str
-    module_name: str | None
-
-
-CLASS_OVERRIDES = [
-    Override("Color", "Color", "ome_types.model._color"),
-    Override("Union", "ShapeUnion", "ome_types.model._shape_union"),
-    Override("StructuredAnnotations", "StructuredAnnotations", None),
-]
-
-
 class OmeFilters(PydanticBaseFilters):
     def __init__(self, config: GeneratorConfig):
         super().__init__(config)
 
         # TODO: it would be nice to know how to get the schema we're processing from
         # the config.  For now, we just assume it's the OME schema and that's the
         # hardcoded default in _util.get_appinfo
@@ -93,27 +102,24 @@
         # in the class.jinja2 template, so we directly modify the attr object here.
         if attr.is_list:
             attr.name = self.appinfo.plurals.get(attr.name, f"{attr.name}s")
 
         for override in CLASS_OVERRIDES:
             if attr.name == override.element_name:
                 return override.class_name
-        return super().field_type(attr, parents)
+        type_name = super().field_type(attr, parents)
+        # we want to use datetime.datetime instead of XmlDateTime
+        return type_name.replace("XmlDateTime", "datetime")
 
     @classmethod
     def build_import_patterns(cls) -> dict[str, dict]:
         patterns = super().build_import_patterns()
-        patterns.update(
-            {
-                o.module_name: {o.class_name: [f": {o.class_name} ="]}
-                for o in CLASS_OVERRIDES
-                if o.module_name
-            }
-        )
+        patterns.update(IMPORT_PATTERNS)
         patterns["ome_types._mixins._util"] = {"new_uuid": ["default_factory=new_uuid"]}
+        patterns["datetime"] = {"datetime": ["datetime"]}
         return {key: patterns[key] for key in sorted(patterns)}
 
     def field_default_value(self, attr: Attr, ns_map: dict | None = None) -> str:
         if attr.tag == "Attribute" and attr.name == "ID":
             return repr(AUTO_SEQUENCE)
         for override in CLASS_OVERRIDES:
             if attr.name == override.element_name:
```

### Comparing `ome_types-0.4.0a3/src/ome_autogen/_transformer.py` & `ome_types-0.4.0a4/src/ome_autogen/_transformer.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_autogen/_util.py` & `ome_types-0.4.0a4/src/ome_autogen/_util.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_autogen/main.py` & `ome_types-0.4.0a4/src/ome_autogen/main.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_types/__init__.py` & `ome_types-0.4.0a4/src/ome_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_types/_conversion.py` & `ome_types-0.4.0a4/src/ome_types/_conversion.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_types/ome-2016-06.xsd` & `ome_types-0.4.0a4/src/ome_types/ome-2016-06.xsd`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_types/validation.py` & `ome_types-0.4.0a4/src/ome_types/validation.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_types/_mixins/_base_type.py` & `ome_types-0.4.0a4/src/ome_types/_mixins/_base_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import warnings
 from datetime import datetime
 from enum import Enum
 from textwrap import indent
-from typing import TYPE_CHECKING, Any, ClassVar, Optional, Sequence, Set, cast
+from typing import TYPE_CHECKING, Any, ClassVar, Optional, Sequence, Set, Tuple, cast
 
 from pydantic import BaseModel, validator
 
 from ome_types._mixins._ids import validate_id
 from ome_types.units import ureg
 
 if TYPE_CHECKING:
@@ -57,60 +57,61 @@
         underscore_attrs_are_private = True
         use_enum_values = False
         validate_all = True
 
     # allow use with weakref
     __slots__: ClassVar[Set[str]] = {"__weakref__"}  # type: ignore
 
-    def __init__(__pydantic_self__, **data: Any) -> None:
-        if "id" in __pydantic_self__.__fields__:
-            data.setdefault("id", AUTO_SEQUENCE)
+    _v = validator("id", pre=True, always=True, check_fields=False)(validate_id)
+
+    def __init__(self, **data: Any) -> None:
         super().__init__(**data)
+        field_names = set(self.__fields__.keys())
+        kwargs = set(data.keys())
+        if kwargs - field_names:
+            warnings.warn(f"Unrecognized fields: {kwargs - field_names}", stacklevel=2)
 
     def __init_subclass__(cls) -> None:
         """Add `*_quantity` property for fields that have both a value and a unit.
 
         where `*_quantity` is a pint `Quantity`.
         """
         for field in cls.__fields__:
             if _UNIT_FIELD.format(field) in cls.__fields__:
                 setattr(cls, _QUANTITY_FIELD.format(field), _quantity_property(field))
 
+    def __repr_args__(self) -> Sequence[Tuple[Optional[str], Any]]:
+        """Repr with only set values, and truncated sequences."""
+        args = []
+        for k, v in self._iter(exclude_defaults=True):
+            if isinstance(v, Sequence) and not isinstance(v, str):
+                # if this is a sequence with a long repr, just show the length
+                # and type
+                if len(repr(v).split(",")) > 5:
+                    type_name = self.__fields__[k].type_.__name__
+                    v = _RawRepr(f"[<{len(v)} {type_name}>]")
+            elif isinstance(v, Enum):
+                v = v.value
+            elif isinstance(v, datetime):
+                v = v.isoformat()
+            args.append((k, v))
+        return sorted(args, key=lambda f: f[0] not in ("name", "id"))
+
     def __repr__(self) -> str:
-        name = self.__class__.__qualname__
-        lines = []
-        for f in sorted(
-            self.__fields__.values(), key=lambda f: f.name not in ("name", "id")
-        ):
-            if f.name.endswith("_"):
-                continue  # pragma: no cover
-            # https://github.com/python/mypy/issues/6910
-            default = f.default_factory() if f.default_factory else f.default
-            current = getattr(self, f.name)
-            if current != default:
-                if isinstance(current, Sequence) and not isinstance(current, str):
-                    rep = f"[<{len(current)} {f.name.title()}>]"
-                elif isinstance(current, Enum):
-                    rep = repr(current.value)
-                elif isinstance(current, datetime):
-                    rep = f"datetime.fromisoformat({current.isoformat()!r})"
-                else:
-                    rep = repr(current)
-                lines.append(f"{f.name}={rep},")
+        lines = [f"{key}={val!r}," for key, val in self.__repr_args__()]
         if len(lines) == 1:
             body = lines[-1].rstrip(",")
         elif lines:
             body = "\n" + indent("\n".join(lines), "   ") + "\n"
         else:
             body = ""
-        return f"{name}({body})"
-
-    _v = validator("id", pre=True, always=True, check_fields=False)(validate_id)
+        return f"{self.__class__.__qualname__}({body})"
 
     def __getattr__(self, key: str) -> Any:
+        """Getattr that redirects deprecated names."""
         cls_name = self.__class__.__name__
         if key in DEPRECATED_NAMES and hasattr(self, DEPRECATED_NAMES[key]):
             new_key = DEPRECATED_NAMES[key]
             warnings.warn(
                 f"Attribute '{cls_name}.{key}' is deprecated, use {new_key!r} instead",
                 DeprecationWarning,
                 stacklevel=2,
@@ -127,7 +128,17 @@
         if value is None:
             return None
 
         unit = cast("Enum", getattr(self, _UNIT_FIELD.format(field_name)))
         return ureg.Quantity(value, unit.value.replace(" ", "_"))
 
     return property(quantity)
+
+
+class _RawRepr:
+    """Helper class to allow repr to show raw values for fields that are sequences."""
+
+    def __init__(self, raw: str) -> None:
+        self.raw = raw
+
+    def __repr__(self) -> str:
+        return self.raw
```

### Comparing `ome_types-0.4.0a3/src/ome_types/_mixins/_bin_data.py` & `ome_types-0.4.0a4/src/ome_types/_mixins/_bin_data.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_types/_mixins/_ids.py` & `ome_types-0.4.0a4/src/ome_types/_mixins/_ids.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_types/_mixins/_instrument.py` & `ome_types-0.4.0a4/src/ome_types/_mixins/_instrument.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_types/_mixins/_ome.py` & `ome_types-0.4.0a4/src/ome_types/_mixins/_ome.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_types/_mixins/_reference.py` & `ome_types-0.4.0a4/src/ome_types/_mixins/_reference.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/ome_types/model/__init__.py` & `ome_types-0.4.0a4/src/ome_types/model/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,7 +67,12 @@
         """Return a module spec to redirect to ome_types._autogenerated.ome_2016_06."""
         if fullname.startswith("ome_types.model."):
             return importlib.util.spec_from_loader(fullname, OME2016Loader(fullname))
         return None
 
 
 sys.meta_path.append(OMEMetaPathFinder())
+
+from ome_types.model._converters import register_converters  # noqa
+
+register_converters()
+del register_converters
```

### Comparing `ome_types-0.4.0a3/src/ome_types/model/_color.py` & `ome_types-0.4.0a4/src/ome_types/model/_color.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from contextlib import suppress
-from typing import Any, Tuple, Union
+from typing import Tuple, Union
 
 from pydantic import color
-from xsdata.formats.converter import Converter, converter
 
 __all__ = ["Color"]
 
 RGBA = Tuple[int, int, int, float]
 ColorType = Union[Tuple[int, int, int], RGBA, str, int]
 
 
@@ -30,18 +29,7 @@
     def __eq__(self, o: object) -> bool:
         if isinstance(o, Color):
             return self.as_int32() == o.as_int32()
         return NotImplemented  # pragma: no cover
 
     def __int__(self) -> int:
         return self.as_int32()
-
-
-class ColorConverter(Converter):
-    def serialize(self, value: Color, **kwargs: Any) -> str:
-        return str(value.as_int32())
-
-    def deserialize(self, value: Any, **kwargs: Any) -> Color:
-        return Color(value)
-
-
-converter.register_converter(Color, ColorConverter())
```

### Comparing `ome_types-0.4.0a3/src/ome_types/model/_shape_union.py` & `ome_types-0.4.0a4/src/ome_types/model/_shape_union.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from contextlib import suppress
-from typing import Dict, List, Type, Union
+from typing import Dict, Iterator, List, Type, Union
 
 from pydantic import Field, ValidationError, validator
 
 from ome_types._autogenerated.ome_2016_06.ellipse import Ellipse
 from ome_types._autogenerated.ome_2016_06.label import Label
 from ome_types._autogenerated.ome_2016_06.line import Line
 from ome_types._autogenerated.ome_2016_06.mask import Mask
@@ -54,7 +54,17 @@
                 kind = v.pop("kind").lower()
                 return _KINDS[kind](**v)
 
             for cls_ in _ShapeCls:
                 with suppress(ValidationError):
                     return cls_(**v)
         raise ValueError(f"Invalid shape: {v}")
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.__root__!r})"
+
+    # overriding BaseModel.__iter__ to behave more like a real Sequence
+    def __iter__(self) -> Iterator[ShapeType]:  # type: ignore[override]
+        yield from self.__root__  # type: ignore[misc]  # see NOTE above
+
+    def __eq__(self, _value: object) -> bool:
+        return _value == self.__root__
```

### Comparing `ome_types-0.4.0a3/src/ome_types/model/_user_sequence.py` & `ome_types-0.4.0a4/src/ome_types/model/_user_sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def __getitem__(self, _idx: slice) -> List[T]:
         ...
 
     def __getitem__(self, _idx: Union[int, slice]) -> Union[T, List[T]]:
         return self.__root__[_idx]  # type: ignore[return-value]
 
     def __len__(self) -> int:
-        return super().__len__()
+        return len(self.__root__)
 
     @overload
     def __setitem__(self, _idx: int, _val: T) -> None:
         ...
 
     @overload
     def __setitem__(self, _idx: slice, _val: Iterable[T]) -> None:
```

### Comparing `ome_types-0.4.0a3/src/ome_types/model/simple_types.py` & `ome_types-0.4.0a4/src/ome_types/model/simple_types.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/xsdata_pydantic_basemodel/bindings.py` & `ome_types-0.4.0a4/src/xsdata_pydantic_basemodel/bindings.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/xsdata_pydantic_basemodel/compat.py` & `ome_types-0.4.0a4/src/xsdata_pydantic_basemodel/compat.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/src/xsdata_pydantic_basemodel/generator.py` & `ome_types-0.4.0a4/src/xsdata_pydantic_basemodel/generator.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/.gitignore` & `ome_types-0.4.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/LICENSE` & `ome_types-0.4.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/README.md` & `ome_types-0.4.0a4/README.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/pyproject.toml` & `ome_types-0.4.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0a3/PKG-INFO` & `ome_types-0.4.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-types
-Version: 0.4.0a3
+Version: 0.4.0a4
 Summary: Python dataclasses for the OME data model
 Project-URL: Source, https://github.com/tlambert03/ome-types
 Project-URL: Tracker, https://github.com/tlambert03/ome-types/issues
 Project-URL: Documentation, https://ome-types.readthedocs.io/en/latest/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 License-File: LICENSE
```

