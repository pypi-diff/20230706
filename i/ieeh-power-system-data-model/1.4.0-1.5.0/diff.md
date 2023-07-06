# Comparing `tmp/ieeh-power-system-data-model-1.4.0.tar.gz` & `tmp/ieeh-power-system-data-model-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieeh-power-system-data-model-1.4.0.tar", last modified: Tue Jun 27 14:03:55 2023, max compression
+gzip compressed data, was "ieeh-power-system-data-model-1.5.0.tar", last modified: Thu Jul  6 07:22:52 2023, max compression
```

## Comparing `ieeh-power-system-data-model-1.4.0.tar` & `ieeh-power-system-data-model-1.5.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      348 2023-06-27 14:02:54.083710 ieeh-power-system-data-model-1.4.0/AUTHORS.md
--rw-r--r--   0        0        0     1568 2023-06-27 14:02:54.083710 ieeh-power-system-data-model-1.4.0/LICENSE
--rw-r--r--   0        0        0     2680 2023-06-27 14:02:54.083710 ieeh-power-system-data-model-1.4.0/README.md
--rw-r--r--   0        0        0        1 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/__init__.py
--rw-r--r--   0        0        0     1068 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/base.py
--rw-r--r--   0        0        0      579 2023-06-27 14:03:46.848663 ieeh-power-system-data-model-1.4.0/psdm/meta.py
--rw-r--r--   0        0        0        1 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/__init__.py
--rw-r--r--   0        0        0     1047 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/active_power.py
--rw-r--r--   0        0        0     3880 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/case.py
--rw-r--r--   0        0        0     5062 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/controller.py
--rw-r--r--   0        0        0      432 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/external_grid.py
--rw-r--r--   0        0        0      539 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/load.py
--rw-r--r--   0        0        0     1091 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/reactive_power.py
--rw-r--r--   0        0        0      367 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/transformer.py
--rw-r--r--   0        0        0        1 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/__init__.py
--rw-r--r--   0        0        0      491 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/active_power.py
--rw-r--r--   0        0        0     1949 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/branch.py
--rw-r--r--   0        0        0      337 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/characteristic.py
--rw-r--r--   0        0        0      364 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/coupler.py
--rw-r--r--   0        0        0      697 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/external_grid.py
--rw-r--r--   0        0        0      361 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/fuse.py
--rw-r--r--   0        0        0     4056 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/load.py
--rw-r--r--   0        0        0     1409 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/load_model.py
--rw-r--r--   0        0        0      320 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/node.py
--rw-r--r--   0        0        0      486 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/reactive_power.py
--rw-r--r--   0        0        0      363 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/switch.py
--rw-r--r--   0        0        0     1011 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/topology.py
--rw-r--r--   0        0        0     2351 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/transformer.py
--rw-r--r--   0        0        0     1081 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology/windings.py
--rw-r--r--   0        0        0        1 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology_case/__init__.py
--rw-r--r--   0        0        0      501 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology_case/case.py
--rw-r--r--   0        0        0      399 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/psdm/topology_case/element_state.py
--rw-r--r--   0        0        0     2686 2023-06-27 14:03:46.872664 ieeh-power-system-data-model-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1441 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/tests/test_active_power.py
--rw-r--r--   0        0        0      659 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/tests/test_branch.py
--rw-r--r--   0        0        0     8953 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/tests/test_controller.py
--rw-r--r--   0        0        0     1449 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/tests/test_reactive_power.py
--rw-r--r--   0        0        0     1870 2023-06-27 14:02:54.087710 ieeh-power-system-data-model-1.4.0/tests/test_topology_load.py
--rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 ieeh-power-system-data-model-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      348 2023-07-06 07:21:54.195411 ieeh-power-system-data-model-1.5.0/AUTHORS.md
+-rw-r--r--   0        0        0     1568 2023-07-06 07:21:54.195411 ieeh-power-system-data-model-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2641 2023-07-06 07:21:54.195411 ieeh-power-system-data-model-1.5.0/README.md
+-rw-r--r--   0        0        0        1 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/__init__.py
+-rw-r--r--   0        0        0     1367 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/base.py
+-rw-r--r--   0        0        0      615 2023-07-06 07:22:44.064108 ieeh-power-system-data-model-1.5.0/psdm/meta.py
+-rw-r--r--   0        0        0        1 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/active_power.py
+-rw-r--r--   0        0        0     3687 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/case.py
+-rw-r--r--   0        0        0     5311 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/controller.py
+-rw-r--r--   0        0        0      432 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/external_grid.py
+-rw-r--r--   0        0        0      539 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/load.py
+-rw-r--r--   0        0        0      889 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/reactive_power.py
+-rw-r--r--   0        0        0      367 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/transformer.py
+-rw-r--r--   0        0        0        1 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/__init__.py
+-rw-r--r--   0        0        0      491 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/active_power.py
+-rw-r--r--   0        0        0     1956 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/branch.py
+-rw-r--r--   0        0        0      337 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/characteristic.py
+-rw-r--r--   0        0        0      364 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/coupler.py
+-rw-r--r--   0        0        0      697 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/external_grid.py
+-rw-r--r--   0        0        0      361 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/fuse.py
+-rw-r--r--   0        0        0     4776 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/load.py
+-rw-r--r--   0        0        0     1305 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/load_model.py
+-rw-r--r--   0        0        0      320 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/node.py
+-rw-r--r--   0        0        0      486 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/reactive_power.py
+-rw-r--r--   0        0        0      363 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/switch.py
+-rw-r--r--   0        0        0      699 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/topology.py
+-rw-r--r--   0        0        0     2275 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/transformer.py
+-rw-r--r--   0        0        0     1081 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology/windings.py
+-rw-r--r--   0        0        0        1 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology_case/__init__.py
+-rw-r--r--   0        0        0      425 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology_case/case.py
+-rw-r--r--   0        0        0      399 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/psdm/topology_case/element_state.py
+-rw-r--r--   0        0        0     2680 2023-07-06 07:22:44.088109 ieeh-power-system-data-model-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1441 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/tests/test_active_power.py
+-rw-r--r--   0        0        0      659 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/tests/test_branch.py
+-rw-r--r--   0        0        0     8953 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/tests/test_controller.py
+-rw-r--r--   0        0        0     1449 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/tests/test_reactive_power.py
+-rw-r--r--   0        0        0     2336 2023-07-06 07:21:54.199411 ieeh-power-system-data-model-1.5.0/tests/test_topology_load.py
+-rw-r--r--   0        0        0     3127 1970-01-01 00:00:00.000000 ieeh-power-system-data-model-1.5.0/PKG-INFO
```

### Comparing `ieeh-power-system-data-model-1.4.0/LICENSE` & `ieeh-power-system-data-model-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.4.0/README.md` & `ieeh-power-system-data-model-1.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # IEEH Power System Data Model
 
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 A data model for the description of electrical power systems.
 
 - [IEEH Power System Data Model](#ieeh-power-system-data-model)
-  - [Field of Application](#-field-of-application)
-  - [Installation](#-installation)
-  - [Development](#-development)
-  - [Attribution](#-attribution)
+  - [ Field of Application](#-field-of-application)
+  - [ Installation](#-installation)
+  - [ Development](#-development)
+  - [ Attribution](#-attribution)
 
 ## <div id="application" /> Field of Application
 
 This data model is intended to describe electrical power systems. It provides a hierarchical structure/schema to describe unique entity relations as well as parameter sets.
 
 The data model is structured as the following schema:
 
@@ -43,19 +43,20 @@
 
 Linux/Mac:
 
 ```bash
 curl -sSL https://raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py | python3 -
 ```
 
-Install [pdm-venv](https://github.com/pdm-project/pdm-venv)
-
+Or using pipx or pip:
+```bash
+pipx install pdm
+```
 ```bash
-pdm plugin add pdm-venv
-pdm config venv.in_project true
+pip install --user pdm
 ```
 
 Clone `power-system-data-model`
 
 ```bash
 git@github.com:ieeh-tu-dresden/power-system-data-model.git
 ```
@@ -86,10 +87,10 @@
 
 Please provide a link to this repository:
 
 <https://github.com/ieeh-tu-dresden/power-system-data-model>
 
 Please cite as:
 
-Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, _Power System Data Model - A data model for the description of electrical power systems_, Zenodo, 2023. <https://doi.org/10.5281/zenodo.7781375>.
+Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, _Power System Data Model - A data model for the description of electrical power systems_, Zenodo, 2023. <https://doi.org/10.5281/zenodo.8087079>.
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7781375.svg)](https://doi.org/10.5281/zenodo.7781375)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8087079.svg)](https://doi.org/10.5281/zenodo.8087079)
```

### Comparing `ieeh-power-system-data-model-1.4.0/psdm/meta.py` & `ieeh-power-system-data-model-1.5.0/psdm/meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # :author: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
 import datetime
+import typing as t
 import uuid
 
 import pydantic
 
 from psdm.base import Base
 
-VERSION = "1.4.0"
+VERSION = "1.5.0"
 
 
 class Meta(Base):
-    version = VERSION
+    version: t.ClassVar[str] = VERSION
     name: str
     date: datetime.date  # date of export
     id: uuid.UUID = pydantic.Field(default_factory=uuid.uuid4)  # noqa: A003
     project: str | None = None  # project the export is related to
```

### Comparing `ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/active_power.py` & `ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/active_power.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
 import pydantic
 
-from psdm.base import Base
+from psdm.topology.load import PowerBase
 from psdm.topology.load import validate_symmetry
 from psdm.topology.load import validate_total
 
 
-class ActivePower(Base):
+class ActivePower(PowerBase):
     value: float  # actual active power (three-phase)
     value_a: float  # actual active power (phase a)
     value_b: float  # actual active power (phase b)
     value_c: float  # actual active power (phase c)
     is_symmetrical: bool
 
-    @pydantic.root_validator(skip_on_failure=True)
-    def _validate_symmetry(cls, values: dict[str, float]) -> dict[str, float]:
-        return validate_symmetry(values)
-
-    @pydantic.root_validator(skip_on_failure=True)
-    def _validate_total(cls, values: dict[str, float]) -> dict[str, float]:
-        return validate_total(values)
+    @pydantic.model_validator(mode="after")  # type: ignore[arg-type]
+    def _validate_symmetry(cls, power: ActivePower) -> ActivePower:
+        return validate_symmetry(power)
+
+    @pydantic.model_validator(mode="after")  # type: ignore[arg-type]
+    def _validate_total(cls, power: ActivePower) -> ActivePower:
+        return validate_total(power)
```

### Comparing `ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/case.py` & `ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/case.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,32 +2,31 @@
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-import pydantic
 from loguru import logger
 
 from psdm.base import Base
 from psdm.meta import Meta
 from psdm.steadystate_case.external_grid import ExternalGrid
 from psdm.steadystate_case.load import Load
 from psdm.steadystate_case.transformer import Transformer
 
 if TYPE_CHECKING:
     from psdm.topology.topology import Topology
 
 
 class Case(Base):
     meta: Meta
-    loads: pydantic.conlist(Load, unique_items=True)  # type: ignore[valid-type]
-    transformers: pydantic.conlist(Transformer, unique_items=True)  # type: ignore[valid-type]
-    external_grids: pydantic.conlist(ExternalGrid, unique_items=True)  # type: ignore[valid-type]
+    loads: list[Load]
+    transformers: list[Transformer]
+    external_grids: list[ExternalGrid]
 
     def is_valid_topology(self, topology: Topology) -> bool:
         logger.info("Verifying steadystate case ...")
         if topology.meta != self.meta:
             logger.error("Metadata does not match.")
             return False
```

### Comparing `ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/controller.py` & `ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # :author: Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
 import enum
-from typing import Annotated
+import typing as t
 
 import pydantic
 
 from psdm.base import Base
 from psdm.base import CosphiDir
 
 
@@ -33,80 +33,84 @@
     B = "B"
     C = "C"
     AB = "AB"
     BC = "BC"
     CA = "CA"
 
 
-class ControlQConst(Base):
+class ControlType(Base):
+    control_strategy: t.ClassVar[ControlStrategy]
+
+
+class ControlQConst(ControlType):
     # q-setpoint control mode
     q_set: float  # Setpoint of reactive power. Counted demand based.
 
-    control_strategy = ControlStrategy.Q_CONST
+    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.Q_CONST
 
 
-class ControlUConst(Base):
+class ControlUConst(ControlType):
     # u-setpoint control mode
     u_set: float = pydantic.Field(ge=0)  # Setpoint of voltage.
     u_meas_ref: ControlledVoltageRef = ControlledVoltageRef.POS_SEQ  # voltage reference
 
-    control_strategy = ControlStrategy.U_CONST
+    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.U_CONST
 
 
-class ControlTanphiConst(Base):
+class ControlTanphiConst(ControlType):
     # cos(phi) control mode
     cosphi_dir: CosphiDir
     cosphi: float = pydantic.Field(ge=0, le=1)  # cos(phi) for calculation of Q in relation to P.
 
-    control_strategy = ControlStrategy.TANPHI_CONST
+    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.TANPHI_CONST
 
 
-class ControlCosphiConst(Base):
+class ControlCosphiConst(ControlType):
     # cos(phi) control mode
     cosphi_dir: CosphiDir
     cosphi: float = pydantic.Field(ge=0, le=1)  # cos(phi) for calculation of Q in relation to P.
 
-    control_strategy = ControlStrategy.COSPHI_CONST
+    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.COSPHI_CONST
 
 
-class ControlCosphiP(Base):
+class ControlCosphiP(ControlType):
     # cos(phi(P)) control mode
     cosphi_ue: float = pydantic.Field(
         ge=0,
         le=1,
     )  # under excited: cos(phi) for calculation of Q in relation to P.
     cosphi_oe: float = pydantic.Field(
         ge=0,
         le=1,
     )  # over excited: cos(phi) for calculation of Q in relation to P.
     p_threshold_ue: float = pydantic.Field(le=0)  # under excited: threshold for P.
     p_threshold_oe: float = pydantic.Field(le=0)  # over excited: threshold for P.
 
-    control_strategy = ControlStrategy.COSPHI_P
+    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.COSPHI_P
 
 
-class ControlCosphiU(Base):
+class ControlCosphiU(ControlType):
     # cos(phi(U)) control mode
     cosphi_ue: float = pydantic.Field(
         ...,
         ge=0,
         le=1,
     )  # under excited: cos(phi) for calculation of Q in relation to P.
     cosphi_oe: float = pydantic.Field(
         ...,
         ge=0,
         le=1,
     )  # over excited: cos(phi) for calculation of Q in relation to P.
     u_threshold_ue: float = pydantic.Field(..., ge=0)  # under excited: threshold for U.
     u_threshold_oe: float = pydantic.Field(..., ge=0)  # over excited: threshold for U.
 
-    control_strategy = ControlStrategy.COSPHI_U
+    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.COSPHI_U
 
 
-class ControlQU(Base):
+class ControlQU(ControlType):
     # Q(U) characteristic control mode
     m_tg_2015: float = pydantic.Field(
         ...,
         ge=0,
     )  # Droop/Slope based on technical guideline VDE-AR-N 4120:2015: '%/kV'-value --> Q = m_% * Pr * dU_kV
     m_tg_2018: float = pydantic.Field(
         ...,
@@ -120,46 +124,38 @@
     u_deadband_low: float = pydantic.Field(
         ...,
         ge=0,
     )  # Width of lower deadband (U_Q0 - U_1_low): per unit value related to Un
     q_max_ue: float = pydantic.Field(..., ge=0)  # Under excited limit of Q: absolut value
     q_max_oe: float = pydantic.Field(..., ge=0)  # Over excited limit of Q: absolut value
 
-    control_strategy = ControlStrategy.Q_U
+    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.Q_U
 
 
 def validate_pos(value: float | None) -> float | None:
     if value is not None and value < 0:
         raise ValueError
 
     return value
 
 
-class ControlQP(Base):
+class ControlQP(ControlType):
     # Q(P) characteristic control mode
     q_p_characteristic_name: str
     q_max_ue: float | None = None  # Under excited limit of Q: absolut value
     q_max_oe: float | None = None  # Over excited limit of Q: absolut value
 
-    control_strategy = ControlStrategy.Q_P
-
-    validate_q_max_ue = pydantic.validator("q_max_ue", allow_reuse=True)(validate_pos)
-    validate_q_max_oe = pydantic.validator("q_max_oe", allow_reuse=True)(validate_pos)
+    control_strategy: t.ClassVar[ControlStrategy] = ControlStrategy.Q_P
 
+    @pydantic.field_validator("q_max_ue", mode="before")
+    def validate_q_max_ue(cls, v: float | None) -> float | None:
+        return validate_pos(v)
 
-ControlType = Annotated[
-    ControlQConst
-    | ControlUConst
-    | ControlTanphiConst
-    | ControlCosphiConst
-    | ControlCosphiP
-    | ControlCosphiU
-    | ControlQU
-    | ControlQP,
-    pydantic.Field(discriminator="control_strategy"),
-]
+    @pydantic.field_validator("q_max_oe", mode="before")
+    def validate_q_max_oe(cls, v: float | None) -> float | None:
+        return validate_pos(v)
 
 
-class Controller(Base):
+class Controller(ControlType):
     node_target: str  # the controlled node (which can be differ from node the load is connected to)
     control_type: ControlType | None = None
     external_controller_name: str | None = None  # if external controller is specified --> name
```

### Comparing `ieeh-power-system-data-model-1.4.0/psdm/steadystate_case/load.py` & `ieeh-power-system-data-model-1.5.0/psdm/steadystate_case/load.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.4.0/psdm/topology/branch.py` & `ieeh-power-system-data-model-1.5.0/psdm/topology/branch.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class Branch(Base):
     node_1: str
     node_2: str
     name: str
     u_n: float  # nominal voltage of the branch connected nodes
-    i_r: float  # rated current of branch (thermal limit in continuous operation)
+    i_r: float | None  # rated current of branch (thermal limit in continuous operation)
     r1: float  # positive sequence values of PI-representation
     x1: float  # positive sequence values of PI-representation
     g1: float  # positive sequence values of PI-representation
     b1: float  # positive sequence values of PI-representation
     type: BranchType  # noqa: A003
     voltage_system_type: VoltageSystemType
     r0: float | None = None  # zero sequence values of PI-representation
```

### Comparing `ieeh-power-system-data-model-1.4.0/psdm/topology/external_grid.py` & `ieeh-power-system-data-model-1.5.0/psdm/topology/external_grid.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.4.0/psdm/topology/load_model.py` & `ieeh-power-system-data-model-1.5.0/psdm/topology/load_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 # :author: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>
 # :author: Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
-
 import pydantic
 
 from psdm.base import Base
 
-if TYPE_CHECKING:
-    from typing import Any
-
 
 class LoadModel(Base):
     """Load Representation Based on Polynomial Model.
 
     Load = Load0*(k_p*(U/U_0)^exp_p + k_i*(U/U_0)^exp_i + (1 - c_p - c_i)*(U/U_0)^exp_z)
     """
 
     name: str | None = None
     c_p: pydantic.confloat(ge=0, le=1) = 1.0  # type: ignore[valid-type]
     c_i: pydantic.confloat(ge=0, le=1) = 0.0  # type: ignore[valid-type]
-    c_z: float = 0
     exp_p: int = 0
     exp_i: int = 1
     exp_z: int = 2
 
-    @pydantic.root_validator
-    def validate_range_c(cls, values: dict[str, Any]) -> dict[str, Any]:
-        name = values["name"]
-        c_p = values["c_p"]
-        c_i = values["c_i"]
+    @pydantic.model_validator(mode="after")  # type: ignore[arg-type]
+    def validate_range_c(cls, load_model: LoadModel) -> LoadModel:
+        name = load_model.name
+        c_p = load_model.c_p
+        c_i = load_model.c_i
         if c_p + c_i > 1:
             msg = f"Load model {name!r}: Sum of components must not exceed 1, but {(c_p + c_i)=}."
             raise ValueError(msg)
 
-        return values
+        return load_model
 
-    @pydantic.root_validator
-    def compute_c_z(cls, values: dict[str, Any]) -> dict[str, Any]:
-        values["c_z"] = 1 - values["c_p"] - values["c_i"]
-        return values
+    @pydantic.computed_field  # type: ignore[misc]
+    @property
+    def c_z(self) -> int:
+        return 1 - self.c_p - self.c_i
```

### Comparing `ieeh-power-system-data-model-1.4.0/psdm/topology/topology.py` & `ieeh-power-system-data-model-1.5.0/psdm/topology/topology.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # :author: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
-import pydantic
-
 from psdm.base import Base
 from psdm.meta import Meta
 from psdm.topology.branch import Branch
 from psdm.topology.external_grid import ExternalGrid
 from psdm.topology.load import Load
 from psdm.topology.node import Node
 from psdm.topology.transformer import Transformer
 
 
 class Topology(Base):
     meta: Meta
-    branches: pydantic.conlist(Branch, unique_items=True)  # type: ignore[valid-type]
-    nodes: pydantic.conlist(Node, unique_items=True)  # type: ignore[valid-type]
-    loads: pydantic.conlist(Load, unique_items=True)  # type: ignore[valid-type]
-    transformers: pydantic.conlist(Transformer, unique_items=True)  # type: ignore[valid-type]
-    external_grids: pydantic.conlist(ExternalGrid, unique_items=True)  # type: ignore[valid-type]
+    branches: list[Branch]
+    nodes: list[Node]
+    loads: list[Load]
+    transformers: list[Transformer]
+    external_grids: list[ExternalGrid]
```

### Comparing `ieeh-power-system-data-model-1.4.0/psdm/topology/transformer.py` & `ieeh-power-system-data-model-1.5.0/psdm/topology/transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
 import enum
 
-import pydantic
-
 from psdm.base import Base
 from psdm.topology.windings import Winding
 
 
 class TapSide(enum.Enum):
     HV = "HV"
     MV = "MV"
@@ -68,15 +66,15 @@
     node_1: str
     node_2: str
     name: str
     number: int  # number of parallel units
     vector_group: VectorGroup  # specifier for connection of wiring e.g. DYn5
     i_0: float  # no-load current in %
     p_fe: float  # no-load losses (Iron losses)
-    windings: pydantic.conlist(Winding, unique_items=True)  # type: ignore[valid-type]  # winding object for each voltage level
+    windings: list[Winding]  # winding object for each voltage level
     phase_technology_type: TransformerPhaseTechnologyType | None = None  # three- or single-phase-transformer
     description: str | None = None
     tap_u_abs: float | None = None  # voltage deviation per tap position change in %
     tap_u_phi: float | None = None  # voltage angle deviation per tap position in °
     tap_max: int | None = None  # upper position of tap for tap control
     tap_min: int | None = None  # lower position of tap for tap control
     tap_neutral: int | None = None  # initial position where rated transformation ratio is specified
```

### Comparing `ieeh-power-system-data-model-1.4.0/psdm/topology/windings.py` & `ieeh-power-system-data-model-1.5.0/psdm/topology/windings.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.4.0/pyproject.toml` & `ieeh-power-system-data-model-1.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,21 @@
     { name = "Sasan Jacob Rasti", email = "sasan_jacob.rasti@tu-dresden.de" },
     { name = "Laura Fiedler", email = "laura.fiedler1@tu-dresden.de" },
     { name = "Maximilian Schmidt", email = "maximilian.schmidt@tu-dresden.de" },
     { name = "Sebastian Krahmer", email = "sebastian.krahmer@tu-dresden.de" },
 ]
 dependencies = [
     "loguru",
-    "pydantic",
+    "pydantic>=2.0",
 ]
 description = "A data model for describing power systems"
 name = "ieeh-power-system-data-model"
 readme = "README.md"
-requires-python = ">=3.10,<3.11"
-version = "1.4.0"
+requires-python = ">=3.10"
+version = "1.5.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/ieeh-tu-dresden/power-system-data-model"
 
@@ -44,15 +44,15 @@
 ]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-xdist",
 ]
 typing = [
-    "mypy @ git+https://github.com/python/mypy.git@master",
+    "mypy",
 ]
 
 [tool.ruff]
 extend-exclude = [
     "tests",
 ]
 ignore = [
@@ -79,37 +79,38 @@
 select = [
     "ALL",
 ]
 
 [tool.ruff.flake8-type-checking]
 runtime-evaluated-base-classes = [
     "psdm.base.Base",
+    "psdm.topology.load.PowerBase",
     "pydantic.BaseModel",
 ]
 
 [tool.ruff.isort]
 force-single-line = true
 
 [tool.ruff.pydocstyle]
 convention = "pep257"
 
 [tool.ruff.pep8-naming]
 classmethod-decorators = [
     "classmethod",
-    "pydantic.root_validator",
-    "pydantic.validator",
+    "pydantic.field_validator",
+    "pydantic.model_validator",
 ]
 
 [tool.black]
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
-version = "1.4.0"
+version = "1.5.0"
 version_files = [
     ".zenodo.json:version",
     "CITATION.cff:cff-version",
     "psdm/meta.py:VERSION",
     "pyproject.toml:version",
 ]
```

### Comparing `ieeh-power-system-data-model-1.4.0/tests/test_active_power.py` & `ieeh-power-system-data-model-1.5.0/tests/test_active_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.4.0/tests/test_branch.py` & `ieeh-power-system-data-model-1.5.0/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.4.0/tests/test_controller.py` & `ieeh-power-system-data-model-1.5.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.4.0/tests/test_reactive_power.py` & `ieeh-power-system-data-model-1.5.0/tests/test_reactive_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.4.0/PKG-INFO` & `ieeh-power-system-data-model-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: ieeh-power-system-data-model
-Version: 1.4.0
+Version: 1.5.0
 Summary: A data model for describing power systems
 Author-email: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>,Laura Fiedler <laura.fiedler1@tu-dresden.de>,Maximilian Schmidt <maximilian.schmidt@tu-dresden.de>,Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10
 Project-URL: Source, https://github.com/ieeh-tu-dresden/power-system-data-model
 Description-Content-Type: text/markdown
 
 # IEEH Power System Data Model
 
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 A data model for the description of electrical power systems.
 
 - [IEEH Power System Data Model](#ieeh-power-system-data-model)
-  - [Field of Application](#-field-of-application)
-  - [Installation](#-installation)
-  - [Development](#-development)
-  - [Attribution](#-attribution)
+  - [ Field of Application](#-field-of-application)
+  - [ Installation](#-installation)
+  - [ Development](#-development)
+  - [ Attribution](#-attribution)
 
 ## <div id="application" /> Field of Application
 
 This data model is intended to describe electrical power systems. It provides a hierarchical structure/schema to describe unique entity relations as well as parameter sets.
 
 The data model is structured as the following schema:
 
@@ -52,19 +52,20 @@
 
 Linux/Mac:
 
 ```bash
 curl -sSL https://raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py | python3 -
 ```
 
-Install [pdm-venv](https://github.com/pdm-project/pdm-venv)
-
+Or using pipx or pip:
+```bash
+pipx install pdm
+```
 ```bash
-pdm plugin add pdm-venv
-pdm config venv.in_project true
+pip install --user pdm
 ```
 
 Clone `power-system-data-model`
 
 ```bash
 git@github.com:ieeh-tu-dresden/power-system-data-model.git
 ```
@@ -95,11 +96,11 @@
 
 Please provide a link to this repository:
 
 <https://github.com/ieeh-tu-dresden/power-system-data-model>
 
 Please cite as:
 
-Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, _Power System Data Model - A data model for the description of electrical power systems_, Zenodo, 2023. <https://doi.org/10.5281/zenodo.7781375>.
+Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, _Power System Data Model - A data model for the description of electrical power systems_, Zenodo, 2023. <https://doi.org/10.5281/zenodo.8087079>.
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7781375.svg)](https://doi.org/10.5281/zenodo.7781375)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8087079.svg)](https://doi.org/10.5281/zenodo.8087079)
```

