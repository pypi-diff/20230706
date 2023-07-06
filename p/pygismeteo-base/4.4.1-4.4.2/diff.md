# Comparing `tmp/pygismeteo_base-4.4.1.tar.gz` & `tmp/pygismeteo_base-4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygismeteo_base-4.4.1.tar", max compression
+gzip compressed data, was "pygismeteo_base-4.4.2.tar", max compression
```

## Comparing `pygismeteo_base-4.4.1.tar` & `pygismeteo_base-4.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/LICENSE
--rw-r--r--   0        0        0      553 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/README.md
--rw-r--r--   0        0        0       86 2023-04-21 20:36:29.353649 pygismeteo_base-4.4.1/pygismeteo_base/__init__.py
--rw-r--r--   0        0        0       92 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/constants.py
--rw-r--r--   0        0        0      925 2023-04-21 19:11:10.073668 pygismeteo_base-4.4.1/pygismeteo_base/current.py
--rw-r--r--   0        0        0      392 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/endpoint.py
--rw-r--r--   0        0        0      901 2023-04-21 19:29:03.763651 pygismeteo_base-4.4.1/pygismeteo_base/http.py
--rw-r--r--   0        0        0      366 2023-04-22 18:01:28.729243 pygismeteo_base-4.4.1/pygismeteo_base/models/__init__.py
--rw-r--r--   0        0        0     1812 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/current.py
--rw-r--r--   0        0        0      759 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/search_by_coordinates.py
--rw-r--r--   0        0        0      673 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/search_by_ip.py
--rw-r--r--   0        0        0      783 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/search_by_query.py
--rw-r--r--   0        0        0     2908 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/step24.py
--rw-r--r--   0        0        0     1786 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/step3.py
--rw-r--r--   0        0        0     1803 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/models/step6.py
--rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/py.typed
--rw-r--r--   0        0        0     1223 2023-04-22 07:03:15.526346 pygismeteo_base-4.4.1/pygismeteo_base/search.py
--rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.4.1/pygismeteo_base/step_n/__init__.py
--rw-r--r--   0        0        0     1452 2023-04-21 19:55:58.533667 pygismeteo_base-4.4.1/pygismeteo_base/step_n/abc.py
--rw-r--r--   0        0        0     1609 2023-04-21 19:56:30.993669 pygismeteo_base-4.4.1/pygismeteo_base/step_n/mixins.py
--rw-r--r--   0        0        0     1816 2023-04-22 18:10:34.669234 pygismeteo_base-4.4.1/pygismeteo_base/types.py
--rw-r--r--   0        0        0      400 2023-04-21 18:50:04.713658 pygismeteo_base-4.4.1/pygismeteo_base/typing_compat.py
--rw-r--r--   0        0        0      914 2023-04-22 07:03:10.606346 pygismeteo_base-4.4.1/pygismeteo_base/validators.py
--rw-r--r--   0        0        0     2706 2023-04-22 18:11:26.199232 pygismeteo_base-4.4.1/pyproject.toml
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 pygismeteo_base-4.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-06 15:19:32.784129 pygismeteo_base-4.4.2/LICENSE
+-rw-r--r--   0        0        0      517 2023-07-06 15:19:32.784129 pygismeteo_base-4.4.2/README.md
+-rw-r--r--   0        0        0       86 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/constants.py
+-rw-r--r--   0        0        0      939 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/current.py
+-rw-r--r--   0        0        0      392 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/endpoint.py
+-rw-r--r--   0        0        0      915 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/http.py
+-rw-r--r--   0        0        0      366 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/models/__init__.py
+-rw-r--r--   0        0        0     1914 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/models/current.py
+-rw-r--r--   0        0        0      861 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/models/search_by_coordinates.py
+-rw-r--r--   0        0        0      775 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/models/search_by_ip.py
+-rw-r--r--   0        0        0      885 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/models/search_by_query.py
+-rw-r--r--   0        0        0     3010 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/models/step24.py
+-rw-r--r--   0        0        0     1888 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/models/step3.py
+-rw-r--r--   0        0        0     1905 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/models/step6.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/py.typed
+-rw-r--r--   0        0        0     1223 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/search.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/step_n/__init__.py
+-rw-r--r--   0        0        0     1466 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/step_n/abc.py
+-rw-r--r--   0        0        0     1623 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/step_n/mixins.py
+-rw-r--r--   0        0        0     1816 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/types.py
+-rw-r--r--   0        0        0      400 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/typing_compat.py
+-rw-r--r--   0        0        0     1016 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pygismeteo_base/validators.py
+-rw-r--r--   0        0        0     2861 2023-07-06 15:19:32.788128 pygismeteo_base-4.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 pygismeteo_base-4.4.2/PKG-INFO
```

### Comparing `pygismeteo_base-4.4.1/LICENSE` & `pygismeteo_base-4.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/current.py` & `pygismeteo_base-4.4.2/pygismeteo_base/current.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,11 +21,13 @@
         )
         params = {
             "latitude": str(coords_validator.latitude),
             "longitude": str(coords_validator.longitude),
         }
         return self._endpoint, params
 
-    def _get_params_by_id(self, id: int) -> Tuple[str, types.Params]:  # noqa: A002
+    def _get_params_by_id(
+        self, id: int  # noqa: A002
+    ) -> Tuple[str, types.Params]:
         id_validator = validators.LocalityID.parse_obj(id)
         url = f"{self._endpoint}/{id_validator.__root__}"
         return url, None
```

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/http.py` & `pygismeteo_base-4.4.2/pygismeteo_base/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 T = TypeVar("T")
 
 
 class BaseHttpClient(Generic[T]):
     __slots__ = ("session", "settings")
 
-    def __init__(self, session: Optional[T], settings: validators.Settings) -> None:
+    def __init__(
+        self, session: Optional[T], settings: validators.Settings
+    ) -> None:
         self.session = session
         self.settings = settings
 
     def _get_params_and_headers(
         self, params: types.Params
     ) -> Tuple[types.Params, types.Headers]:
         if self.settings.lang:
```

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/models/current.py` & `pygismeteo_base-4.4.2/pygismeteo_base/models/current.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Field
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field  # type: ignore[assignment]
 
 
 class Precipitation(BaseModel):
     type_ext: Optional[int] = None
     intensity: int
     correction: Optional[bool] = None
     amount: Optional[float] = None
```

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/models/search_by_coordinates.py` & `pygismeteo_base-4.4.2/pygismeteo_base/models/search_by_query.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from pydantic import BaseModel, Field
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field  # type: ignore[assignment]
 
 
 class District(BaseModel):
     name: str
-    name_p: str = Field(alias="nameP")
+    name_p: Optional[str] = Field(default=None, alias="nameP")
 
 
-class SubDistrict(BaseModel):
+class Country(BaseModel):
     name: str
-    name_p: str = Field(alias="nameP")
+    code: str
+    name_p: Optional[str] = Field(default=None, alias="nameP")
 
 
-class Country(BaseModel):
-    name: Optional[str] = None
-    code: str
+class SubDistrict(BaseModel):
+    name: str
     name_p: Optional[str] = Field(default=None, alias="nameP")
 
 
 class ModelItem(BaseModel):
     district: Optional[District] = None
     id: int
     sub_district: Optional[SubDistrict] = None
     url: str
     name_p: Optional[str] = Field(default=None, alias="nameP")
-    name: Optional[str] = None
-    distance: float
+    name: str
+    rate: int
+    weight: int
     kind: str
     country: Country
 
 
 class Model(BaseModel):
     __root__: List[ModelItem]
```

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/models/search_by_ip.py` & `pygismeteo_base-4.4.2/pygismeteo_base/models/search_by_coordinates.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import List, Optional
 
-from pydantic import BaseModel, Field
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field  # type: ignore[assignment]
 
 
 class District(BaseModel):
     name: str
     name_p: str = Field(alias="nameP")
 
 
@@ -17,16 +20,21 @@
 
 class Country(BaseModel):
     name: Optional[str] = None
     code: str
     name_p: Optional[str] = Field(default=None, alias="nameP")
 
 
-class Model(BaseModel):
+class ModelItem(BaseModel):
     district: Optional[District] = None
     id: int
     sub_district: Optional[SubDistrict] = None
     url: str
     name_p: Optional[str] = Field(default=None, alias="nameP")
     name: Optional[str] = None
+    distance: float
     kind: str
     country: Country
+
+
+class Model(BaseModel):
+    __root__: List[ModelItem]
```

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/models/step24.py` & `pygismeteo_base-4.4.2/pygismeteo_base/models/step24.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from pydantic import BaseModel, Field
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field  # type: ignore[assignment]
 
 
 class Precipitation(BaseModel):
     type_ext: Optional[int] = None
     intensity: int
     amount: float
     type: int
```

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/models/step3.py` & `pygismeteo_base-4.4.2/pygismeteo_base/models/step3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from pydantic import BaseModel, Field
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field  # type: ignore[assignment]
 
 
 class Precipitation(BaseModel):
     type_ext: Optional[int] = None
     intensity: int
     correction: Optional[bool] = None
     amount: Optional[float] = None
```

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/models/step6.py` & `pygismeteo_base-4.4.2/pygismeteo_base/models/step6.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from pydantic import BaseModel, Field
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field  # type: ignore[assignment]
 
 
 class Precipitation(BaseModel):
     type_ext: Optional[int] = None
     intensity: int
     correction: Optional[bool] = None
     amount: float
```

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/search.py` & `pygismeteo_base-4.4.2/pygismeteo_base/search.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/step_n/abc.py` & `pygismeteo_base-4.4.2/pygismeteo_base/step_n/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     def _model(self) -> types.StepNModel:
         pass
 
     @property
     @abstractmethod
     def _days_validator(
         self,
-    ) -> Type[Union[validators.Step3Days, validators.Step6Days, validators.Step24Days]]:
+    ) -> Type[
+        Union[validators.Step3Days, validators.Step6Days, validators.Step24Days]
+    ]:
         pass
 
     def _get_params_by_coordinates(
         self, latitude: float, longitude: float, *, days: types.StepNDays
     ) -> Tuple[str, types.Params]:
         coords_validator = validators.Coordinates(
             latitude=latitude, longitude=longitude
```

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/step_n/mixins.py` & `pygismeteo_base-4.4.2/pygismeteo_base/step_n/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     def _model(self) -> types.StepNModel:
         pass
 
     @property
     @abstractmethod
     def _days_validator(
         self,
-    ) -> Type[Union[validators.Step3Days, validators.Step6Days, validators.Step24Days]]:
+    ) -> Type[
+        Union[validators.Step3Days, validators.Step6Days, validators.Step24Days]
+    ]:
         pass
 
 
 class Step3Mixin(StepNMixin):
     __slots__ = ()
 
     @property
```

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/types.py` & `pygismeteo_base-4.4.2/pygismeteo_base/types.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.4.1/pygismeteo_base/validators.py` & `pygismeteo_base-4.4.2/pygismeteo_base/validators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
 from ipaddress import IPv4Address
 from typing import Optional
 
-from pydantic import BaseModel, Field
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field  # type: ignore[assignment]
 
 from . import types
 
 
 class Settings(BaseModel):
     lang: Optional[types.Lang] = Field(...)
     token: Optional[str] = Field(...)
```

### Comparing `pygismeteo_base-4.4.1/pyproject.toml` & `pygismeteo_base-4.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygismeteo-base"
-version = "4.4.1"
+version = "4.4.2"
 description = "Base for pygismeteo and aiopygismeteo"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/pygismeteo-base"
 classifiers = [
     "Environment :: Web Environment",
@@ -22,38 +22,40 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pydantic = "^1.9"
+pydantic = ">=1.9,<3"
 typing-extensions = { version = ">=3.7.4.3,<5", python = "<3.10" }
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
-mypy = "1.2.0"
+mypy = "1.4.1"
 pre-commit = "2.21.0"
-ruff = "0.0.262"
+ruff = "0.0.277"
 
 [tool.black]
 target-version = ["py37"]
+line-length = 80
 skip-magic-trailing-comma = true
 preview = true
 
 [tool.mypy]
 python_version = "3.7"
 disallow_subclassing_any = false
 disallow_untyped_calls = false
 disallow_untyped_decorators = false
 warn_unreachable = true
 local_partial_types = true
 enable_error_code = [
     "redundant-self",
     "redundant-expr",
+    "possibly-undefined",
     "truthy-bool",
     "truthy-iterable",
     "ignore-without-code",
     "unused-awaitable",
 ]
 strict = true
 plugins = ["pydantic.mypy"]
@@ -62,18 +64,18 @@
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
 [tool.ruff]
 target-version = "py37"
+line-length = 80
 select = ["ALL"]
 ignore = [
     "ANN",
-    "B008",
     "BLE001",
     "C901",
     "COM",
     "D100",
     "D101",
     "D102",
     "D103",
@@ -88,23 +90,27 @@
     "D400",
     "D401",
     "D407",
     "D415",
     "D417",
     "DJ008",
     "ERA001",
+    "FBT002",
     "PD901",
+    "PERF203",
     "PLR0911",
     "PLR0912",
     "PLR0913",
     "PLR0915",
     "PT012",
     "RUF001",
     "RUF002",
     "RUF003",
+    "RUF012",
+    "RUF013",
     "S110",
     "S112",
     "S308",
     "S311",
     "SIM105",
     "TCH001",
     "TCH002",
@@ -119,13 +125,16 @@
 [tool.ruff.flake8-unused-arguments]
 ignore-variadic-names = true
 
 [tool.ruff.isort]
 combine-as-imports = true
 required-imports = ["from __future__ import annotations"]
 
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [tool.ruff.pyupgrade]
 keep-runtime-typing = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pygismeteo_base-4.4.1/PKG-INFO` & `pygismeteo_base-4.4.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygismeteo-base
-Version: 4.4.1
+Version: 4.4.2
 Summary: Base for pygismeteo and aiopygismeteo
 Home-page: https://github.com/monosans/pygismeteo-base
 License: MIT
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
@@ -25,23 +25,23 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: pydantic (>=1.9,<2.0)
+Requires-Dist: pydantic (>=1.9,<3)
 Requires-Dist: typing-extensions (>=3.7.4.3,<5) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/monosans/pygismeteo-base
 Description-Content-Type: text/markdown
 
 # pygismeteo-base
 
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/pygismeteo-base/main.svg)](https://results.pre-commit.ci/latest/github/monosans/pygismeteo-base/main)
-[![PyPI Downloads](https://img.shields.io/pypi/dm/pygismeteo-base?logo=pypi)](https://pypi.org/project/pygismeteo-base/)
+[![CI](https://github.com/monosans/pygismeteo-base/actions/workflows/ci.yml/badge.svg)](https://github.com/monosans/pygismeteo-base/actions/workflows/ci.yml)
+[![Downloads](https://static.pepy.tech/badge/pygismeteo-base)](https://pepy.tech/project/pygismeteo-base)
 
 База для [pygismeteo](https://github.com/monosans/pygismeteo) и [aiopygismeteo](https://github.com/monosans/aiopygismeteo).
 
 ## License / Лицензия
 
 [MIT](https://github.com/monosans/pygismeteo-base/blob/main/LICENSE)
```

