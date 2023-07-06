# Comparing `tmp/piel-0.0.36.tar.gz` & `tmp/piel-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.36.tar", last modified: Mon Jul  3 00:29:53 2023, max compression
+gzip compressed data, was "piel-0.0.37.tar", last modified: Thu Jul  6 07:06:39 2023, max compression
```

## Comparing `piel-0.0.36.tar` & `piel-0.0.37.tar`

### file list

```diff
@@ -1,296 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.465236 piel-0.0.36/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-03 00:29:32.000000 piel-0.0.36/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-03 00:29:32.000000 piel-0.0.36/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-03 00:29:32.000000 piel-0.0.36/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-03 00:29:53.465236 piel-0.0.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-03 00:29:32.000000 piel-0.0.36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 00:29:32.000000 piel-0.0.36/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/cli/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/cocotb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/cocotb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/cocotb/core/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/cocotb/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/components/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/components/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/config/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/config/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/file_system/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/gdsfactory/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/gdsfactory/netlist/
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/gdsfactory/netlist/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    39300 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/integration/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.433236 piel-0.0.36/docs/autoapi/piel/integration/openlane_gdsfactory_core/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/integration/sax_cocotb/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/integration/sax_cocotb/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/integration/sax_qutip/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/integration/sax_qutip/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/frequency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/frequency/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/frequency/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/frequency/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/frequency/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/coupler_simple/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/coupler_simple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/directional_coupler_length/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/directional_coupler_real/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.437236 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/directional_coupler_simple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/grating_coupler/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/grating_coupler/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/mmi1x2/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/mmi1x2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/mmi2x2/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/mmi2x2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/photonic/straight_waveguide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/frequency/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/frequency/utils/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/logic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/logic/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/logic/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/logic/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/logic/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/logic/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/logic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/logic/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/logic/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/logic/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/logic/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/physical/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/physical/electrical/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/physical/electrical/cable/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/physical/electrical/cable/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/physical/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/physical/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/physical/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/physical/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/physical/electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/physical/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/physical/geometry/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/physical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/physical/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/physical/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/physical/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/physical/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.441236 piel-0.0.36/docs/autoapi/piel/models/physical/thermal/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/physical/thermal/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/models/physical/units/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/physical/units/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/models/transient/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/models/transient/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/transient/electrical/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/models/transient/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/transient/electro_optic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/models/transient/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/transient/electronic/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/transient/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/models/transient/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/transient/opto_electronic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/models/transient/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/transient/photonic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/models/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/openlane/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/openlane/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/openlane/migrate/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/openlane/parse/
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/openlane/parse/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/openlane/parse/sta_rpt/
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/openlane/parse/sta_rpt/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/openlane/parse/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/openlane/parse/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/openlane/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/openlane/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/openlane/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/openlane/v1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/openlane/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/openlane/v2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/parametric/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/parametric/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/project_structure/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/project_structure/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.445236 piel-0.0.36/docs/autoapi/piel/sax/
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/sax/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.449236 piel-0.0.36/docs/autoapi/piel/sax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-07-03 00:29:32.000000 piel-0.0.36/docs/autoapi/piel/sax/utils/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-03 00:29:32.000000 piel-0.0.36/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 00:29:32.000000 piel-0.0.36/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.425236 piel-0.0.36/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.425236 piel-0.0.36/docs/examples/designs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.425236 piel-0.0.36/docs/examples/designs/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.425236 piel-0.0.36/docs/examples/designs/simple_design/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.449236 piel-0.0.36/docs/examples/designs/simple_design/simple_design/tb/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-03 00:29:32.000000 piel-0.0.36/docs/examples/designs/simple_design/simple_design/tb/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.449236 piel-0.0.36/docs/examples/designs/simple_design/simple_design/tb/default/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-03 00:29:32.000000 piel-0.0.36/docs/examples/designs/simple_design/simple_design/tb/default/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-03 00:29:32.000000 piel-0.0.36/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 00:29:32.000000 piel-0.0.36/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-03 00:29:32.000000 piel-0.0.36/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.429236 piel-0.0.36/docs/sections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.449236 piel-0.0.36/docs/sections/about/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/about/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/about/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.449236 piel-0.0.36/docs/sections/codesign/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/codesign/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.449236 piel-0.0.36/docs/sections/components/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/components/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.449236 piel-0.0.36/docs/sections/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/environment/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.449236 piel-0.0.36/docs/sections/microservices/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.449236 piel-0.0.36/docs/sections/microservices/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/microservices/dependencies/cocotb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/microservices/dependencies/gdsfactory.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/microservices/dependencies/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/microservices/dependencies/openlane.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/microservices/dependencies/sax.rst
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/microservices/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.449236 piel-0.0.36/docs/sections/microservices/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/microservices/integration/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/microservices/integration/sax_qutip.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.449236 piel-0.0.36/docs/sections/models/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-03 00:29:32.000000 piel-0.0.36/docs/sections/models/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.453236 piel-0.0.36/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-03 00:29:32.000000 piel-0.0.36/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-03 00:29:32.000000 piel-0.0.36/piel/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.453236 piel-0.0.36/piel/cocotb/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 00:29:32.000000 piel-0.0.36/piel/cocotb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-03 00:29:32.000000 piel-0.0.36/piel/cocotb/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.453236 piel-0.0.36/piel/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-03 00:29:32.000000 piel-0.0.36/piel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-03 00:29:32.000000 piel-0.0.36/piel/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-03 00:29:32.000000 piel-0.0.36/piel/file_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.453236 piel-0.0.36/piel/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 00:29:32.000000 piel-0.0.36/piel/gdsfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-03 00:29:32.000000 piel-0.0.36/piel/gdsfactory/netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.457236 piel-0.0.36/piel/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-03 00:29:32.000000 piel-0.0.36/piel/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-03 00:29:32.000000 piel-0.0.36/piel/integration/openlane_gdsfactory_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 00:29:32.000000 piel-0.0.36/piel/integration/sax_cocotb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-03 00:29:32.000000 piel-0.0.36/piel/integration/sax_qutip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.457236 piel-0.0.36/piel/models/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.457236 piel-0.0.36/piel/models/frequency/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.457236 piel-0.0.36/piel/models/frequency/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.457236 piel-0.0.36/piel/models/frequency/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/electro_optic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.457236 piel-0.0.36/piel/models/frequency/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.457236 piel-0.0.36/piel/models/frequency/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.457236 piel-0.0.36/piel/models/frequency/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/photonic/coupler_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/photonic/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/photonic/directional_coupler_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/photonic/directional_coupler_real.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/photonic/directional_coupler_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/photonic/grating_coupler.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/photonic/mmi1x2.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/photonic/mmi2x2.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/photonic/straight_waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/frequency/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.457236 piel-0.0.36/piel/models/logic/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/logic/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/logic/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/logic/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/logic/electro_optic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/logic/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/logic/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/logic/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/logic/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/logic/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/logic/photonic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/physical/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/physical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/physical/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/physical/electrical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/physical/electrical/cable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/physical/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/physical/electro_optic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/physical/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/physical/electronic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/physical/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/physical/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/physical/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/physical/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/physical/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/physical/thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/physical/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/transient/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/transient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/transient/electrical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/transient/electrical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/transient/electro_optic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/transient/electro_optic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/transient/electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/transient/electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.461236 piel-0.0.36/piel/models/transient/opto_electronic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/transient/opto_electronic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.465236 piel-0.0.36/piel/models/transient/photonic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/transient/photonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:32.000000 piel-0.0.36/piel/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.465236 piel-0.0.36/piel/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-03 00:29:32.000000 piel-0.0.36/piel/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-03 00:29:32.000000 piel-0.0.36/piel/openlane/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.465236 piel-0.0.36/piel/openlane/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 00:29:32.000000 piel-0.0.36/piel/openlane/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-03 00:29:32.000000 piel-0.0.36/piel/openlane/parse/run_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-07-03 00:29:32.000000 piel-0.0.36/piel/openlane/parse/sta_rpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-03 00:29:32.000000 piel-0.0.36/piel/openlane/parse/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-03 00:29:32.000000 piel-0.0.36/piel/openlane/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-07-03 00:29:32.000000 piel-0.0.36/piel/openlane/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 00:29:32.000000 piel-0.0.36/piel/openlane/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-03 00:29:32.000000 piel-0.0.36/piel/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-03 00:29:32.000000 piel-0.0.36/piel/project_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.465236 piel-0.0.36/piel/sax/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 00:29:32.000000 piel-0.0.36/piel/sax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-03 00:29:32.000000 piel-0.0.36/piel/sax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.453236 piel-0.0.36/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-03 00:29:53.000000 piel-0.0.36/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-03 00:29:53.000000 piel-0.0.36/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 00:29:53.000000 piel-0.0.36/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 00:29:53.000000 piel-0.0.36/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 00:29:53.000000 piel-0.0.36/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 00:29:53.000000 piel-0.0.36/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 00:29:53.000000 piel-0.0.36/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-03 00:29:53.469236 piel-0.0.36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-03 00:29:32.000000 piel-0.0.36/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.465236 piel-0.0.36/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 00:29:32.000000 piel-0.0.36/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.465236 piel-0.0.36/tests/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 00:29:32.000000 piel-0.0.36/tests/gdsfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-03 00:29:32.000000 piel-0.0.36/tests/gdsfactory/test_netlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 00:29:53.465236 piel-0.0.36/tests/sax/
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-03 00:29:32.000000 piel-0.0.36/tests/sax/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-03 00:29:32.000000 piel-0.0.36/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-06 07:06:18.000000 piel-0.0.37/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 07:06:18.000000 piel-0.0.37/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-06 07:06:18.000000 piel-0.0.37/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-06 07:06:39.006881 piel-0.0.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-06 07:06:18.000000 piel-0.0.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-06 07:06:18.000000 piel-0.0.37/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-06 07:06:18.000000 piel-0.0.37/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 07:06:18.000000 piel-0.0.37/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.986880 piel-0.0.37/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.986880 piel-0.0.37/docs/examples/designs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.986880 piel-0.0.37/docs/examples/designs/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.986880 piel-0.0.37/docs/examples/designs/simple_design/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/examples/designs/simple_design/simple_design/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-06 07:06:18.000000 piel-0.0.37/docs/examples/designs/simple_design/simple_design/tb/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/examples/designs/simple_design/simple_design/tb/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-06 07:06:18.000000 piel-0.0.37/docs/examples/designs/simple_design/simple_design/tb/default/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-06 07:06:18.000000 piel-0.0.37/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-06 07:06:18.000000 piel-0.0.37/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-06 07:06:18.000000 piel-0.0.37/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.986880 piel-0.0.37/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/about/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/about/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/codesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/codesign/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/components/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/environment/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/microservices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/microservices/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/dependencies/cocotb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/dependencies/gdsfactory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/dependencies/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/dependencies/openlane.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/dependencies/sax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/microservices/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/integration/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/microservices/integration/sax_qutip.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/docs/sections/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-06 07:06:18.000000 piel-0.0.37/docs/sections/models/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.994880 piel-0.0.37/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-06 07:06:18.000000 piel-0.0.37/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-06 07:06:18.000000 piel-0.0.37/piel/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/cocotb/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 07:06:18.000000 piel-0.0.37/piel/cocotb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-07-06 07:06:18.000000 piel-0.0.37/piel/cocotb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-06 07:06:18.000000 piel-0.0.37/piel/cocotb/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-06 07:06:18.000000 piel-0.0.37/piel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-06 07:06:18.000000 piel-0.0.37/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-06 07:06:18.000000 piel-0.0.37/piel/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-06 07:06:18.000000 piel-0.0.37/piel/file_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 07:06:18.000000 piel-0.0.37/piel/gdsfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-06 07:06:18.000000 piel-0.0.37/piel/gdsfactory/netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 07:06:18.000000 piel-0.0.37/piel/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-06 07:06:18.000000 piel-0.0.37/piel/integration/openlane_gdsfactory_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-06 07:06:18.000000 piel-0.0.37/piel/integration/sax_cocotb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-06 07:06:18.000000 piel-0.0.37/piel/integration/sax_qutip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/frequency/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/frequency/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/frequency/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/electro_optic/ideal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/frequency/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel/models/frequency/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/frequency/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/directional_coupler_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/directional_coupler_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/directional_coupler_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/grating_coupler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/mmi1x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/mmi2x2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/photonic/straight_waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/frequency/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/electro_optic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/electro_optic/signal_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/logic/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/logic/photonic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/electrical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/electrical/cable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/electro_optic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/electronic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/physical/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/physical/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/electrical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/electrical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/electro_optic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/opto_electronic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/opto_electronic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.002881 piel-0.0.37/piel/models/transient/photonic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/transient/photonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:18.000000 piel-0.0.37/piel/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/piel/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/piel/openlane/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/parse/run_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/parse/sta_rpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-06 07:06:18.000000 piel-0.0.37/piel/openlane/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-06 07:06:18.000000 piel-0.0.37/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-06 07:06:18.000000 piel-0.0.37/piel/project_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/piel/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 07:06:18.000000 piel-0.0.37/piel/sax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-06 07:06:18.000000 piel-0.0.37/piel/sax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.998880 piel-0.0.37/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 07:06:38.000000 piel-0.0.37/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-06 07:06:39.006881 piel-0.0.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-06 07:06:18.000000 piel-0.0.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-06 07:06:18.000000 piel-0.0.37/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/tests/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 07:06:18.000000 piel-0.0.37/tests/gdsfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-06 07:06:18.000000 piel-0.0.37/tests/gdsfactory/test_netlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.990880 piel-0.0.37/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:38.990880 piel-0.0.37/tests/models/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/tests/models/logic/electro_optic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-06 07:06:18.000000 piel-0.0.37/tests/models/logic/electro_optic/test_signal_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:06:39.006881 piel-0.0.37/tests/sax/
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-06 07:06:18.000000 piel-0.0.37/tests/sax/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-06 07:06:18.000000 piel-0.0.37/tests/test_piel.py
```

### Comparing `piel-0.0.36/CONTRIBUTING.rst` & `piel-0.0.37/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/LICENSE` & `piel-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/PKG-INFO` & `piel-0.0.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.36
+Version: 0.0.37
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `piel-0.0.36/README.md` & `piel-0.0.37/README.md`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/docs/Makefile` & `piel-0.0.37/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/docs/autoapi/piel/integration/openlane_gdsfactory_core/index.rst` & `piel-0.0.37/piel/integration/openlane_gdsfactory_core.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,51 @@
-:py:mod:`piel.integration.openlane_gdsfactory_core`
-===================================================
+"""
+There are a number of ways to generate gdsfactory integration.
 
-.. py:module:: piel.integration.openlane_gdsfactory_core
+It is worth noting that GDSFactory has already the following PDKs installed:
+* SKY130nm https://gdsfactory.github.io/skywater130/
+* GF180nm https://gdsfactory.github.io/gf180/
+"""
+import gdsfactory as gf
+from ..config import piel_path_types
+from ..file_system import check_path_exists
+from ..openlane.migrate import get_design_from_openlane_migration
+from ..openlane.utils import find_design_run
+
+
+def create_gdsfactory_component_from_openlane(
+    design_name_v1: str | None = None,
+    design_directory: piel_path_types | None = None,
+    run_name: str | None = None,
+    v1: bool = True,
+) -> gf.Component:
+    """
+    This function cretes a gdsfactory layout component that can be included in the network codesign of the device, or that can be used for interconnection codesign.
+
+    It will look into the latest design run and extract the final OpenLane-generated GDS. You do not have to have run this with OpenLane2 as it just looks at the latest run.
+
+    Args:
+        design_name_v1(str): Design name of the v1 design that can be found within `$OPENLANE_ROOT/"<latest>"/designs`.
+        design_directory(piel_path_types): Design directory PATH.
+        run_name(str): Name of the run to extract the GDS from. If None, it will look at the latest run.
+        v1(bool): If True, it will import the design from the OpenLane v1 configuration.
+
+    Returns:
+        component(gf.Component): GDSFactory component.
+    """
+    design_name, design_directory = get_design_from_openlane_migration(
+        v1=v1, design_name_v1=design_name_v1, design_directory=design_directory
+    )
+    latest_design_run_directory = find_design_run(design_directory, run_name=run_name)
+    final_gds_run = (
+        latest_design_run_directory
+        / "results"
+        / "final"
+        / "gds"
+        / (design_name + ".gds")
+    )
+    check_path_exists(final_gds_run, raise_errors=True)
+    component = gf.import_gds(final_gds_run, name=design_name)
+    return component
 
-.. autoapi-nested-parse::
 
-   There are a number of ways to generate gdsfactory integration.
-
-   It is worth noting that GDSFactory has already the following PDKs installed:
-   * SKY130nm https://gdsfactory.github.io/skywater130/
-   * GF180nm https://gdsfactory.github.io/gf180/
-
-
-
-Module Contents
----------------
-
-
-Functions
-~~~~~~~~~
-
-.. autoapisummary::
-
-   piel.integration.openlane_gdsfactory_core.create_gdsfactory_component_from_openlane
-
-
-
-.. py:function:: create_gdsfactory_component_from_openlane(design_name_v1: str | None = None, design_directory: str | pathlib.Path | None = None, run_name: str | None = None, v1: bool = True) -> gdsfactory.Component
-
-   This function cretes a gdsfactory layout component that can be included in the network codesign of the device, or that can be used for interconnection codesign.
-
-   It will look into the latest design run and extract the final OpenLane-generated GDS. You do not have to have run this with OpenLane2 as it just looks at the latest run.
-
-   :param design_name_v1: Design name of the v1 design that can be found within `$OPENLANE_ROOT/"<latest>"/designs`.
-   :type design_name_v1: str
-   :param design_directory: Design directory PATH.
-   :type design_directory: str
-   :param run_name: Name of the run to extract the GDS from. If None, it will look at the latest run.
-   :type run_name: str
-   :param v1: If True, it will import the design from the OpenLane v1 configuration.
-   :type v1: bool
-
-   :returns: GDSFactory component.
-   :rtype: component(gf.Component)
+__all__ = ["create_gdsfactory_component_from_openlane"]
```

### Comparing `piel-0.0.36/docs/autoapi/piel/integration/sax_qutip/index.rst` & `piel-0.0.37/piel/integration/sax_qutip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,95 @@
-:py:mod:`piel.integration.sax_qutip`
-====================================
+import qutip  # NOQA : F401
+import sax
+from ..config import nso
+from ..sax.utils import sax_to_s_parameters_standard_matrix
 
-.. py:module:: piel.integration.sax_qutip
+__all__ = ["sax_to_ideal_qutip_unitary", "standard_s_parameters_to_ideal_qutip_unitary"]
 
 
-Module Contents
----------------
+def standard_s_parameters_to_ideal_qutip_unitary(
+    s_parameters_standard_matrix: nso.ndarray,
+):
+    """
+    This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
+    dimensions of the matrix can be observed.
 
+    I think this means we need to transpose the output of the filtered sax SDense matrix to map it to a QuTip matrix.
+    Note that the documentation and formatting of the standard `sax` mapping to a S-parameter standard notation is already in described in piel/piel/sax/utils.py.
 
-Functions
-~~~~~~~~~
+    From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly. https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
 
-.. autoapisummary::
+    For example, a ``qutip`` representation of an s-gate gate would be:
 
-   piel.integration.sax_qutip.standard_s_parameters_to_ideal_qutip_unitary
-   piel.integration.sax_qutip.sax_to_ideal_qutip_unitary
+    ..code-block:: python
+        import numpy as np
+        import qutip
 
+        # S-Gate
+        s_gate_matrix = np.array([[1.,   0],
+                                 [0., 1.j]])
+        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
+    In mathematical notation, this S-gate would be written as:
 
-.. py:function:: standard_s_parameters_to_ideal_qutip_unitary(s_parameters_standard_matrix: piel.config.nso.ndarray)
+    ..math::
+        S = \\begin{bmatrix}
+            1 & 0 \\
+            0 & i \\
+        \\end{bmatrix}
 
-   This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
-   dimensions of the matrix can be observed.
+    Args:
+        s_parameters_standard_matrix (nso.ndarray): A dictionary of S-parameters in the form of a SDict from `sax`.
 
-   I think this means we need to transpose the output of the filtered sax SDense matrix to map it to a QuTip matrix.
-   Note that the documentation and formatting of the standard `sax` mapping to a S-parameter standard notation is already in described in piel/piel/sax/utils.py.
+    Returns:
+        qobj_unitary (qutip.Qobj): A QuTip QObj representation of the S-parameters in a unitary matrix.
+    """
+    # TODO make a function any SAX input.
+    qobj_unitary = qutip.Qobj(s_parameters_standard_matrix)
+    return qobj_unitary
 
-   From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly. https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
 
-   For example, a ``qutip`` representation of an s-gate gate would be:
+def sax_to_ideal_qutip_unitary(sax_input: sax.SType):
+    """
+    This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
+    dimensions of the matrix can be observed.
 
-   ..code-block:: python
-       import numpy as np
-       import qutip
+    I think this means we need to transpose the output of the filtered sax SDense matrix to map it to a QuTip matrix.
+    Note that the documentation and formatting of the standard `sax` mapping to a S-parameter standard notation is already in described in piel/piel/sax/utils.py.
 
-       # S-Gate
-       s_gate_matrix = np.array([[1.,   0],
-                                [0., 1.j]])
-       s_gate = qutip.Qobj(mat, dims=[[2], [2]])
+    From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly. https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
 
-   In mathematical notation, this S-gate would be written as:
+    For example, a ``qutip`` representation of an s-gate gate would be:
 
-   ..math::
-       S = \begin{bmatrix}
-           1 & 0 \
-           0 & i \
-       \end{bmatrix}
+    ..code-block:: python
 
-   :param s_parameters_standard_matrix: A dictionary of S-parameters in the form of a SDict from `sax`.
-   :type s_parameters_standard_matrix: nso.ndarray
+        import numpy as np
+        import qutip
+        # S-Gate
+        s_gate_matrix = np.array([[1.,   0],
+                                 [0., 1.j]])
+        s_gate = qutip.Qobj(mat, dims=[[2], [2]])
 
-   :returns: A QuTip QObj representation of the S-parameters in a unitary matrix.
-   :rtype: qobj_unitary (qutip.Qobj)
+    In mathematical notation, this S-gate would be written as:
 
+    ..math::
 
-.. py:function:: sax_to_ideal_qutip_unitary(sax_input: sax.SType)
+        S = \\begin{bmatrix}
+            1 & 0 \\
+            0 & i \\
+        \\end{bmatrix}
 
-   This function converts the calculated S-parameters into a standard Unitary matrix topology so that the shape and
-   dimensions of the matrix can be observed.
+    Args:
+        sax_input (sax.SType): A dictionary of S-parameters in the form of a SDict from `sax`.
 
-   I think this means we need to transpose the output of the filtered sax SDense matrix to map it to a QuTip matrix.
-   Note that the documentation and formatting of the standard `sax` mapping to a S-parameter standard notation is already in described in piel/piel/sax/utils.py.
+    Returns:
 
-   From this stage we can implement a ``QObj`` matrix accordingly and perform simulations accordingly. https://qutip.org/docs/latest/guide/qip/qip-basics.html#unitaries
-
-   For example, a ``qutip`` representation of an s-gate gate would be:
-
-   ..code-block:: python
-
-       import numpy as np
-       import qutip
-       # S-Gate
-       s_gate_matrix = np.array([[1.,   0],
-                                [0., 1.j]])
-       s_gate = qutip.Qobj(mat, dims=[[2], [2]])
-
-   In mathematical notation, this S-gate would be written as:
-
-   ..math::
-
-       S = \begin{bmatrix}
-           1 & 0 \
-           0 & i \
-       \end{bmatrix}
-
-   :param sax_input: A dictionary of S-parameters in the form of a SDict from `sax`.
-   :type sax_input: sax.SType
-
-   Returns:
+    """
+    # TODO make a function any SAX input.
+    (
+        s_parameters_standard_matrix,
+        input_ports_index_tuple_order,
+    ) = sax_to_s_parameters_standard_matrix(sax_input)
+    qobj_unitary = standard_s_parameters_to_ideal_qutip_unitary(
+        s_parameters_standard_matrix
+    )
+    return qobj_unitary
```

### Comparing `piel-0.0.36/docs/conf.py` & `piel-0.0.37/docs/conf.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/docs/examples/designs/simple_design/simple_design/tb/default/Makefile` & `piel-0.0.37/docs/examples/designs/simple_design/simple_design/tb/default/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/docs/index.rst` & `piel-0.0.37/docs/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/docs/make.bat` & `piel-0.0.37/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/docs/sections/microservices/dependencies/cocotb.rst` & `piel-0.0.37/docs/sections/microservices/dependencies/cocotb.rst`

 * *Files 23% similar despite different names*

```diff
@@ -56,10 +56,12 @@
 00000370: 6c61 746f 725f 7375 7070 6f72 742e 6874  lator_support.ht
 00000380: 6d6c 3e60 5f5f 0a2d 2020 6047 4844 4c20  ml>`__.-  `GHDL 
 00000390: 3c68 7474 7073 3a2f 2f64 6f63 732e 636f  <https://docs.co
 000003a0: 636f 7462 2e6f 7267 2f65 6e2f 7374 6162  cotb.org/en/stab
 000003b0: 6c65 2f73 696d 756c 6174 6f72 5f73 7570  le/simulator_sup
 000003c0: 706f 7274 2e68 746d 6c3e 605f 5f0a 0a2e  port.html>`__...
 000003d0: 2e20 746f 6374 7265 653a 3a0a 2020 2020  . toctree::.    
-000003e0: 2e2e 2f2e 2e2f 2e2e 2f61 7574 6f61 7069  ../../../autoapi
-000003f0: 2f70 6965 6c2f 636f 636f 7462 2f69 6e64  /piel/cocotb/ind
-00000400: 6578 2e72 7374 0a                        ex.rst.
+000003e0: 636f 636f 7462 5f75 7365 6675 6c5f 636f  cocotb_useful_co
+000003f0: 6d6d 616e 6473 0a20 2020 202e 2e2f 2e2e  mmands.    ../..
+00000400: 2f2e 2e2f 6175 746f 6170 692f 7069 656c  /../autoapi/piel
+00000410: 2f63 6f63 6f74 622f 696e 6465 782e 7273  /cocotb/index.rs
+00000420: 740a                                     t.
```

### Comparing `piel-0.0.36/docs/sections/microservices/dependencies/openlane.rst` & `piel-0.0.37/docs/sections/microservices/dependencies/openlane.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/docs/sections/microservices/dependencies/sax.rst` & `piel-0.0.37/docs/sections/microservices/dependencies/sax.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/docs/sections/microservices/integration/sax_qutip.rst` & `piel-0.0.37/docs/sections/microservices/integration/sax_qutip.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/__init__.py` & `piel-0.0.37/piel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 os.environ["PIEL_PACKAGE_DIRECTORY"] = str(
     pathlib.Path(__file__).parent.parent.resolve()
 )
 
 __author__ = """Dario Quintero"""
 __email__ = "darioaquintero@gmail.com"
-__version__ = "0.0.36"
+__version__ = "0.0.37"
```

### Comparing `piel-0.0.36/piel/cocotb/core.py` & `piel-0.0.37/piel/cocotb/core.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/config.py` & `piel-0.0.37/piel/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 We create a set of parameters that can be used throughout the project for optimisation.
-"""
 
-"""
 The numerical solver is normally delegated for as `numpy` but there are cases where a much faster solver is desired, and where different functioanlity is required. For example, `sax` uses `JAX` for its numerical solver. In this case, we will create a global numerical solver that we can use throughout the project, and that can be extended and solved accordingly for the particular project requirements.
 """
+import pathlib
 import sys
+import types
+
 
 if "jax" in sys.modules:
     import jax.numpy as jnp
 
     numerical_solver = jnp
 elif "numpy" in sys.modules:
     import numpy
@@ -17,12 +18,14 @@
     numerical_solver = numpy
 else:
     import numpy
 
     numerical_solver = numpy
 
 nso = numerical_solver
+piel_path_types = str | pathlib.Path | types.ModuleType
 
 __all__ = [
     "numerical_solver",
     "nso",
+    "piel_path_types",
 ]
```

### Comparing `piel-0.0.36/piel/defaults.py` & `piel-0.0.37/piel/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/file_system.py` & `piel-0.0.37/piel/file_system.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,65 +2,76 @@
 import json
 import openlane
 import os
 import pathlib
 import shutil
 import stat
 import subprocess
+import types
 from typing import Literal
+from .config import piel_path_types
 
 
 def check_path_exists(
-    path: str | pathlib.Path,
+    path: piel_path_types,
     raise_errors: bool = False,
 ) -> bool:
     """
     Checks if a directory exists.
 
     Args:
-        path(str | pathlib.Path): Input path.
+        path(piel_path_types): Input path.
 
     Returns:
         directory_exists(bool): True if directory exists.
     """
     directory_exists = False
     path = return_path(path)
     if path.exists():
         directory_exists = True
     else:
         if raise_errors:
             raise ValueError("Path: " + str(path) + " does not exist.")
     return directory_exists
 
 
-def check_example_design(design_name: str | pathlib.Path = "simple_design") -> bool:
+def check_example_design(
+    design_name: str = "simple_design",
+    designs_directory: piel_path_types | None = None,
+) -> bool:
     """
     We copy the example simple_design from docs to the `/foss/designs` in the `iic-osic-tools` environment.
 
     Args:
         design_name(str): Name of the design to check.
+        designs_directory(piel_path_types): Directory that contains the DESIGNS environment flag.
+        # TODO
 
     Returns:
         None
     """
+    if designs_directory is None:
+        designs_directory = pathlib.Path(os.environ["DESIGNS"])
+
     design_folder = (
-        pathlib.Path(os.environ["DESIGNS"]) / design_name
+        designs_directory / design_name
     )  # TODO verify this copying operation
     return design_folder.exists()
 
 
 def copy_source_folder(
-    source_directory: str | pathlib.Path, target_directory: str | pathlib.Path
+    source_directory: piel_path_types,
+    target_directory: piel_path_types,
 ) -> None:
     """
     Copies the files from a source_directory to a target_directory
 
     Args:
-        source_directory(str): Source directory.
-        target_directory(str): Target directory.
+        source_directory(piel_path_types): Source directory.
+        target_directory(piel_path_types): Target directory.
 
     Returns:
         None
     """
     source_directory = return_path(source_directory)
     target_directory = return_path(target_directory)
     if target_directory.exists():
@@ -83,21 +94,21 @@
         copy_function=shutil.copy2,
         ignore_dangling_symlinks=False,
         dirs_exist_ok=False,
     )
 
 
 def convert_list_to_path_list(
-    input_list: list[str | pathlib.Path],
+    input_list: list[piel_path_types],
 ) -> list[pathlib.Path]:
     """
     Converts a list of strings or pathlib.Path to a list of pathlib.Path.
 
     Args:
-        input_list(list[str | pathlib.Path]): Input list.
+        input_list(list[piel_path_types]): Input list.
 
     Returns:
         output_list(list[pathlib.Path]): Output list.
     """
     output_list = []
     for item in input_list:
         item = return_path(item)
@@ -148,24 +159,24 @@
         if path.is_dir():
             shutil.rmtree(path)
         elif path.is_file():
             path.unlink()
 
 
 def delete_path_list_in_directory(
-    directory_path: str | pathlib.Path,
+    directory_path: piel_path_types,
     path_list: list,
     ignore_confirmation: bool = False,
     validate_individual: bool = False,
 ) -> None:
     """
     Deletes a list of files in a directory.
 
     Args:
-        directory_path(str | pathlib.Path): Input path.
+        directory_path(piel_path_types): Input path.
         path_list(list): List of files.
         ignore_confirmation(bool): Ignore confirmation. Default: False.
         validate_individual(bool): Validate individual files. Default: False.
 
     Returns:
         None
     """
@@ -196,55 +207,55 @@
                     if path.exists():
                         delete_path(path)
             elif answer.upper() in ["N", "NO"]:
                 print("Skipping deletion of: " + str(path_list))
 
 
 def get_files_recursively_in_directory(
-    path: str | pathlib.Path,
+    path: piel_path_types,
     extension: str = "*",
 ):
     """
     Returns a list of files in a directory.
 
     Args:
-        path(str | pathlib.Path): Input path.
+        path(piel_path_types): Input path.
         extension(str): File extension.
 
     Returns:
         file_list(list): List of files.
     """
     path = return_path(path)
     file_list = []
     for x in os.walk(str(path.resolve())):
         for file_path in glob.glob(os.path.join(x[0], f"*.{extension}")):
             file_list.append(file_path)
     return file_list
 
 
-def permit_script_execution(script_path: str | pathlib.Path) -> None:
+def permit_script_execution(script_path: piel_path_types) -> None:
     """
     Permits the execution of a script.
 
     Args:
-        script_path(str): Script path.
+        script_path(piel_path_types): Script path.
 
     Returns:
         None
     """
     script = return_path(script_path)
     script.chmod(script.stat().st_mode | stat.S_IEXEC)
 
 
-def permit_directory_all(directory_path: str | pathlib.Path) -> None:
+def permit_directory_all(directory_path: piel_path_types) -> None:
     """
     Permits a directory to be read, written and executed. Use with care as it can be a source for security issues.
 
     Args:
-        directory_path(str | pathlib.Path): Input path.
+        directory_path(piel_path_types): Input path.
 
     Returns:
         None
     """
     directory_path = return_path(directory_path)
     try:
         directory_path.chmod(0o777)
@@ -254,31 +265,31 @@
                 "Could not change permissions of directory: "
                 + str(directory_path.resolve())
                 + " to 777. Your Python executable might not have the required permissions. Restructure your project directory so Python does not have to change permissions."
             )
         )
 
 
-def read_json(path: str | pathlib.Path) -> dict:
+def read_json(path: piel_path_types) -> dict:
     """
     Reads a JSON file.
 
     Args:
-        path(str | pathlib.Path): Input path.
+        path(piel_path_types): Input path.
 
     Returns:
         json_data(dict): JSON data.
     """
     path = return_path(path)
     with open(path, "r") as json_file:
         json_data = json.load(json_file)
     return json_data
 
 
-def return_path(input_path: str | pathlib.Path) -> pathlib.Path:
+def return_path(input_path: piel_path_types) -> pathlib.Path:
     """
     Returns a pathlib.Path to be able to perform operations accordingly internally.
 
     This allows us to maintain compatibility between POSIX and Windows systems.
 
     Args:
         input_path(str): Input path.
@@ -286,27 +297,29 @@
     Returns:
         pathlib.Path: Pathlib path.
     """
     if type(input_path) == str:
         output_path = pathlib.Path(input_path)
     elif isinstance(input_path, pathlib.Path):
         output_path = input_path
+    elif isinstance(input_path, types.ModuleType):
+        output_path = pathlib.Path(input_path.__file__).parent
     else:
         raise ValueError(
             "input_path: " + str(input_path) + " is of type: " + str(type(input_path))
         )
     return output_path
 
 
-def run_script(script_path: str | pathlib.Path) -> None:
+def run_script(script_path: piel_path_types) -> None:
     """
     Runs a script on the filesystem `script_path`.
 
     Args:
-        script_path(str): Script path.
+        script_path(piel_path_types): Script path.
 
     Returns:
         None
     """
     script = return_path(script_path)
     subprocess.run(str(script.resolve()), check=True, capture_output=True)
 
@@ -338,23 +351,23 @@
     design_folder = os.environ["DESIGNS"] + "/" + example_name
     copy_source_folder(
         source_directory=example_design_folder, target_directory=design_folder
     )
 
 
 def write_script(
-    directory_path: str | pathlib.Path,
+    directory_path: piel_path_types,
     script: str,
     script_name: str,
 ) -> None:
     """
     Records a `script_name` in the `scripts` project directory.
 
     Args:
-        directory_path(str): Design directory.
+        directory_path(piel_path_types): Design directory.
         script(str): Script to write.
         script_name(str): Name of the script.
 
     Returns:
         None
     """
     directory_path = return_path(directory_path)
```

### Comparing `piel-0.0.36/piel/gdsfactory/netlist.py` & `piel-0.0.37/piel/gdsfactory/netlist.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Literal
 
 __all__ = ["get_input_ports_index", "get_matched_ports_tuple_index"]
 
 
 def get_matched_ports_tuple_index(
     ports_index: dict,
-    sorting_algorithm: Literal["prefix"] = "prefix",
+    selected_ports_tuple: tuple,
+    sorting_algorithm: Literal["prefix", "selected_ports"] = "prefix",
     prefix: str = "in",
 ) -> (tuple, tuple):
     """
     This function returns the input ports of a component. However, input ports may have different sets of prefixes
     and suffixes. This function implements different sorting algorithms for different ports names. The default
     algorithm is `prefix`, which sorts the ports by their prefix. The Endianness implementation means that the tuple
     order is determined according to the last numerical index order of the port numbering. Returns just a tuple of
@@ -53,14 +54,26 @@
         ]
         # This sorts in numerical order
         matched_ports_list.sort()
         matched_ports_name_tuple_order = tuple(matched_ports_list)
         matches_ports_index_tuple_order = tuple(
             [ports_index[port] for port in matched_ports_list]
         )
+    elif sorting_algorithm == "selected_ports":
+        matched_ports_list = selected_ports_tuple
+        matched_ports_name_tuple_order = tuple(matched_ports_list)
+        matches_ports_index_tuple_order = tuple(
+            [ports_index[port] for port in matched_ports_list]
+        )
+    else:
+        raise ValueError(
+            "matches_ports_index_tuple_order "
+            + str(matches_ports_index_tuple_order)
+            + " not defined."
+        )
     return matches_ports_index_tuple_order, matched_ports_name_tuple_order
 
 
 def get_input_ports_index(
     ports_index: dict,
     sorting_algorithm: Literal["prefix"] = "prefix",
     prefix: str = "in",
```

### Comparing `piel-0.0.36/piel/models/frequency/photonic/defaults.py` & `piel-0.0.37/piel/models/frequency/defaults.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .straight_waveguide import waveguide
-from .mmi2x2 import mmi2x2_50_50
+from .photonic.straight_waveguide import waveguide
+from .photonic.mmi2x2 import mmi2x2_50_50
 
 
 # Default model dictionary library that can be overwritten for specific modelling applications.
 __default_models_dictionary__ = {
     "bend_euler": waveguide,
     "mmi2x2": mmi2x2_50_50,
     "straight": waveguide,
```

### Comparing `piel-0.0.36/piel/models/frequency/photonic/directional_coupler_length.py` & `piel-0.0.37/piel/models/frequency/photonic/directional_coupler_length.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/models/frequency/photonic/directional_coupler_real.py` & `piel-0.0.37/piel/models/frequency/photonic/directional_coupler_real.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/models/frequency/photonic/grating_coupler.py` & `piel-0.0.37/piel/models/frequency/photonic/grating_coupler.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/models/frequency/photonic/straight_waveguide.py` & `piel-0.0.37/piel/models/frequency/photonic/straight_waveguide.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 """
 Translated from https://github.com/flaport/sax or https://github.com/flaport/photontorch/tree/master
 """
 import sax
 from ....config import nso
 
+__all__ = ["ideal_active_waveguide", "waveguide", "simple_straight"]
+
 
 def waveguide(wl=1.55, wl0=1.55, neff=2.34, ng=3.4, length=10.0, loss=0.0):
     dwl = wl - wl0
     dneff_dwl = (ng - neff) / wl0
     neff = neff - dwl * dneff_dwl
     phase = 2 * nso.pi * neff * length / wl
     amplitude = nso.asarray(10 ** (-loss * length / 20), dtype=complex)
     transmission = amplitude * nso.exp(1j * phase)
     sdict = sax.reciprocal({("o1", "o2"): transmission})
     return sdict
 
 
+def ideal_active_waveguide(
+    wl=1.55, wl0=1.55, neff=2.34, ng=3.4, length=10.0, loss=0.0, active_phase_rad=0.0
+):
+    dwl = wl - wl0
+    dneff_dwl = (ng - neff) / wl0
+    neff = neff - dwl * dneff_dwl
+    phase = (2 * nso.pi * neff * length / wl) + active_phase_rad
+    amplitude = nso.asarray(10 ** (-loss * length / 20), dtype=complex)
+    transmission = amplitude * nso.exp(1j * phase)
+    sdict = sax.reciprocal({("o1", "o2"): transmission})
+    return sdict
+
+
 def simple_straight(length=10.0, width=0.5):
     S = {("o1", "o2"): 1.0}  # we'll improve this model later!
     return sax.reciprocal(S)
-
-
-__all__ = ["waveguide", "simple_straight"]
```

### Comparing `piel-0.0.36/piel/openlane/migrate.py` & `piel-0.0.37/piel/openlane/migrate.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/openlane/parse/run_output.py` & `piel-0.0.37/piel/openlane/parse/run_output.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/openlane/parse/sta_rpt.py` & `piel-0.0.37/piel/openlane/parse/sta_rpt.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/openlane/parse/utils.py` & `piel-0.0.37/piel/openlane/parse/utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/openlane/v1.py` & `piel-0.0.37/piel/openlane/v1.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/openlane/v2.py` & `piel-0.0.37/piel/openlane/v2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-import json
 import openlane
+from ..config import piel_path_types
+from ..file_system import return_path, read_json
 from piel.defaults import test_spm_open_lane_configuration
 
 
 def run_openlane_flow(
     configuration: dict | None = test_spm_open_lane_configuration,
-    design_directory: str = "/foss/designs/spm",
+    design_directory: piel_path_types = "/foss/designs/spm",
 ) -> None:
     """
     Runs the OpenLane flow.
 
     Args:
         configuration(dict): OpenLane configuration dictionary. If none is present it will default to the config.json file on the design_directory.
-        design_directory(str): Design directory PATH.
+        design_directory(piel_path_types): Design directory PATH.
 
     Returns:
         None
     """
+    design_directory = return_path(design_directory)
     if configuration is None:
         # Get extract configuration file from config.json on directory
-        config_json_filepath = design_directory + "/config.json"
-        config_json = open(config_json_filepath)
-        configuration = json.load(config_json)
+        config_json_filepath = design_directory / "config.json"
+        configuration = read_json(config_json_filepath)
 
     Classic = openlane.Flow.get("Classic")
 
     flow = Classic(
         config=configuration,
-        design_dir=design_directory,
+        design_dir=str(design_directory.resolve()),
     )
 
     flow.start()
 
 
 __all__ = ["run_openlane_flow"]
```

### Comparing `piel-0.0.36/piel/parametric.py` & `piel-0.0.37/piel/parametric.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/piel/project_structure.py` & `piel-0.0.37/piel/project_structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
 This file allows us to automate several aspects of creating a fully compatible project structure.
 """
-import pathlib
+from .config import piel_path_types
 from .file_system import return_path, write_script, read_json, check_path_exists
 
 
-def read_configuration(design_directory: str | pathlib.Path) -> dict:
+def read_configuration(design_directory: piel_path_types) -> dict:
     """
     This function reads the configuration file found in the design directory.
 
     Args:
-        design_directory(str): Design directory PATH.
+        design_directory(piel_path_types): Design directory PATH.
 
     Returns:
         config_dictionary(dict): Configuration dictionary.
     """
     design_directory = return_path(design_directory)
     config_path = design_directory / "config.json"
     check_path_exists(config_path, raise_errors=True)
     config_dictionary = read_json(config_path)
     return config_dictionary
 
 
-def create_setup_py_from_config_json(design_directory: str | pathlib.Path) -> None:
+def create_setup_py_from_config_json(design_directory: piel_path_types) -> None:
     """
     This function creates a setup.py file from the config.json file found in the design directory.
 
     Args:
-        design_directory(str): Design directory PATH.
+        design_directory(piel_path_types): Design directory PATH or module name.
 
     Returns:
         None
     """
     design_directory = return_path(design_directory)
     config_json_path = design_directory / "config.json"
     config_dictionary = read_json(config_json_path)
```

### Comparing `piel-0.0.36/piel/sax/utils.py` & `piel-0.0.37/piel/sax/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     # TODO look into jnp.at method https://github.com/flaport/sax/blob/a87c3bf8c792dc227779e5d010627897f4cd8278/sax/typing_.py#L355
     input_ports_index = {key: all_ports_index[key] for key in input_ports_order}
     return input_ports_index
 
 
 def sax_to_s_parameters_standard_matrix(
     sax_input: sax.SType,
+    input_ports_order: tuple | None = None,
 ) -> tuple:
     """
     A ``sax`` S-parameter SDict is provided as a dictionary of tuples with (port0, port1) as the key. This
     determines the direction of the scattering relationship. It means that the number of terms in an S-parameter
     matrix is the number of ports squared.
 
     In order to generalise, this function returns both the S-parameter matrices and the indexing ports based on the
@@ -132,35 +133,62 @@
             a_{n}
         \\end{bmatrix}
 
     TODO check with Floris, does this mean we need to transpose the matrix?
 
     Args:
         sax_input (sax.SType): The sax S-parameter dictionary.
+        input_ports_order (tuple): The ports order tuple containing the names and order of the input ports.
 
     Returns:
         tuple: The S-parameter matrix and the input ports index tuple in the standard S-parameter notation.
     """
     dense_s_parameter_matrix, dense_s_parameter_index = sax.sdense(sax_input)
+    # print(dense_s_parameter_index)
+    all_ports_list = dense_s_parameter_index.keys()
     # Now we get the indexes of the input ports that we care about to restructure the dense matrix with the columns
     # we care about.
-    (
-        input_ports_index_tuple_order,
-        input_matched_ports_name_tuple_order,
-    ) = get_matched_ports_tuple_index(ports_index=dense_s_parameter_index, prefix="in")
-    (
-        output_ports_index_tuple_order,
-        output_matched_ports_name_tuple_order,
-    ) = get_matched_ports_tuple_index(ports_index=dense_s_parameter_index, prefix="out")
+    if input_ports_order is not None:
+        output_ports_order = tuple(set(all_ports_list) - set(input_ports_order))
+        (
+            input_ports_index_tuple_order,
+            input_matched_ports_name_tuple_order,
+        ) = get_matched_ports_tuple_index(
+            ports_index=dense_s_parameter_index,
+            selected_ports_tuple=input_ports_order,
+            sorting_algorithm="selected_ports",
+        )
+        (
+            output_ports_index_tuple_order,
+            output_matched_ports_name_tuple_order,
+        ) = get_matched_ports_tuple_index(
+            ports_index=dense_s_parameter_index,
+            selected_ports_tuple=output_ports_order,
+            sorting_algorithm="selected_ports",
+        )
+    else:
+        (
+            input_ports_index_tuple_order,
+            input_matched_ports_name_tuple_order,
+        ) = get_matched_ports_tuple_index(
+            ports_index=dense_s_parameter_index, prefix="in"
+        )
+        (
+            output_ports_index_tuple_order,
+            output_matched_ports_name_tuple_order,
+        ) = get_matched_ports_tuple_index(
+            ports_index=dense_s_parameter_index, prefix="out"
+        )
+
     # We now select the SDense columns that we care about.
     s_parameters_standard_matrix = dense_s_parameter_matrix[
         [output_ports_index_tuple_order]
     ][0]
     # Now we select the SDense rows that we care about after transposing the matrix.
     s_parameters_standard_matrix = s_parameters_standard_matrix[
         :, [input_ports_index_tuple_order][0]
     ]
     # TODO verify matrix transpose for unitary match.
-    return s_parameters_standard_matrix.T, input_ports_index_tuple_order
+    return s_parameters_standard_matrix.T, input_matched_ports_name_tuple_order
 
 
 snet = sax_to_s_parameters_standard_matrix
```

### Comparing `piel-0.0.36/piel.egg-info/PKG-INFO` & `piel-0.0.37/piel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.36
+Version: 0.0.37
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `piel-0.0.36/setup.py` & `piel-0.0.37/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from setuptools import setup, find_packages
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 requirements = [
+    "bokeh",
+    "jupyter_bokeh",
     "Click>=7.0",
     "cocotb",
     "gdsfactory",
     "openlane",
     "pandas",
     "sax",
     "qutip",
@@ -63,10 +65,10 @@
     include_package_data=True,
     keywords="piel",
     name="piel",
     packages=find_packages(include=["piel", "piel.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/daquintero/piel",
-    version="0.0.36",
+    version="0.0.37",
     zip_safe=False,
 )
```

### Comparing `piel-0.0.36/tests/gdsfactory/test_netlist.py` & `piel-0.0.37/tests/gdsfactory/test_netlist.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/tests/sax/test_utils.py` & `piel-0.0.37/tests/sax/test_utils.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.36/tests/test_piel.py` & `piel-0.0.37/tests/test_piel.py`

 * *Files identical despite different names*

