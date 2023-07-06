# Comparing `tmp/sunweg-1.0.0.tar.gz` & `tmp/sunweg-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunweg-1.0.0.tar", last modified: Mon Feb 27 22:26:31 2023, max compression
+gzip compressed data, was "sunweg-2.0.0b0.tar", last modified: Thu Jul  6 10:36:08 2023, max compression
```

## Comparing `sunweg-1.0.0.tar` & `sunweg-2.0.0b0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:26:31.873641 sunweg-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-27 22:26:22.000000 sunweg-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-27 22:26:31.873641 sunweg-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-02-27 22:26:22.000000 sunweg-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 22:26:31.873641 sunweg-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-27 22:26:22.000000 sunweg-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:26:31.873641 sunweg-1.0.0/sunweg/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-27 22:26:22.000000 sunweg-1.0.0/sunweg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-02-27 22:26:22.000000 sunweg-1.0.0/sunweg/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-27 22:26:22.000000 sunweg-1.0.0/sunweg/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-02-27 22:26:22.000000 sunweg-1.0.0/sunweg/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-02-27 22:26:22.000000 sunweg-1.0.0/sunweg/plant.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-02-27 22:26:22.000000 sunweg-1.0.0/sunweg/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:26:31.873641 sunweg-1.0.0/sunweg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-27 22:26:31.000000 sunweg-1.0.0/sunweg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-27 22:26:31.000000 sunweg-1.0.0/sunweg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 22:26:31.000000 sunweg-1.0.0/sunweg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-27 22:26:31.000000 sunweg-1.0.0/sunweg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-27 22:26:31.000000 sunweg-1.0.0/sunweg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 22:26:31.873641 sunweg-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-27 22:26:22.000000 sunweg-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-27 22:26:22.000000 sunweg-1.0.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-02-27 22:26:22.000000 sunweg-1.0.0/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/sunweg/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/plant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/sunweg/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/sunweg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 10:36:08.000000 sunweg-2.0.0b0/sunweg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-06 10:36:08.000000 sunweg-2.0.0b0/sunweg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:36:08.000000 sunweg-2.0.0b0/sunweg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 10:36:08.000000 sunweg-2.0.0b0/sunweg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 10:36:08.000000 sunweg-2.0.0b0/sunweg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:08.682124 sunweg-2.0.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-06 10:35:54.000000 sunweg-2.0.0b0/tests/test_api.py
```

### Comparing `sunweg-1.0.0/LICENSE` & `sunweg-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `sunweg-1.0.0/PKG-INFO` & `sunweg-2.0.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunweg
-Version: 1.0.0
+Version: 2.0.0b0
 Summary: A library to retrieve data from sunweg.net
 Home-page: https://github.com/rokam/sunweg
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 # SunWeg
 
 [![Python build](https://github.com/rokam/sunweg/actions/workflows/python-build.yml/badge.svg)](https://github.com/rokam/sunweg/actions/workflows/python-build.yml)
 ![Python tests](https://raw.githubusercontent.com/rokam/sunweg/badges/tests.svg)
 ![Python coverage](https://raw.githubusercontent.com/rokam/sunweg/badges/coverage.svg)
 ![Python fake8](https://raw.githubusercontent.com/rokam/sunweg/badges/flake8.svg)
 
-Python lib for WEG solar energy platform, https://sunweg.net/
+Python lib for WEG solar energy platform, [SunWEG.net](https://sunweg.net/)
 
 ## Usage
 
 ``` python
 from sunweg.api import APIHelper
 
 api = APIHelper('username','password')
```

### Comparing `sunweg-1.0.0/README.md` & `sunweg-2.0.0b0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SunWeg
 
 [![Python build](https://github.com/rokam/sunweg/actions/workflows/python-build.yml/badge.svg)](https://github.com/rokam/sunweg/actions/workflows/python-build.yml)
 ![Python tests](https://raw.githubusercontent.com/rokam/sunweg/badges/tests.svg)
 ![Python coverage](https://raw.githubusercontent.com/rokam/sunweg/badges/coverage.svg)
 ![Python fake8](https://raw.githubusercontent.com/rokam/sunweg/badges/flake8.svg)
 
-Python lib for WEG solar energy platform, https://sunweg.net/
+Python lib for WEG solar energy platform, [SunWEG.net](https://sunweg.net/)
 
 ## Usage
 
 ``` python
 from sunweg.api import APIHelper
 
 api = APIHelper('username','password')
```

### Comparing `sunweg-1.0.0/setup.py` & `sunweg-2.0.0b0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 requires = [
     "requests",
 ]
 
 setuptools.setup(
     name="sunweg",
-    version="1.0.0",
+    version="2.0.0b",
     author="rokam",
     author_email="lucas@mindello.com.br",
     description="A library to retrieve data from sunweg.net",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rokam/sunweg",
```

### Comparing `sunweg-1.0.0/sunweg/api.py` & `sunweg-2.0.0b0/sunweg/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,18 +118,17 @@
                 ),
                 kwh_per_kwp=float(str(result["KWHporkWp"]).replace(",", "."))
                 if result["KWHporkWp"] != ""
                 else float(0),
                 performance_rate=result["taxaPerformance"],
                 saving=result["economia"],
                 today_energy=float(
-                    str(result["energiaGeradaHoje"])
-                    .replace(" kWh", "")
-                    .replace(",", ".")
+                    str(result["energiaGeradaHoje"]).split(" ")[0].replace(",", ".")
                 ),
+                today_energy_metric=str(result["energiaGeradaHoje"]).split(" ")[1],
                 total_energy=float(result["energiaacumuladanumber"]),
                 total_carbon_saving=result["reduz_carbono_total_number"],
                 last_update=datetime.strptime(
                     result["ultimaAtualizacao"], "%Y-%m-%d %H:%M:%S"
                 ),
             )
 
@@ -166,24 +165,25 @@
         try:
             result = self._get(SUNWEG_INVERTER_DETAIL_PATH + str(id))
             inverter = Inverter(
                 id=id,
                 name=result["inversor"]["nome"],
                 sn=result["inversor"]["esn"],
                 total_energy=float(
-                    result["energiaAcumulada"].replace(" kWh", "").replace(",", ".")
+                    result["energiaAcumulada"].split(" ")[0].replace(",", ".")
                 ),
+                total_energy_metric=result["energiaAcumulada"].split(" ")[1],
                 today_energy=float(
-                    result["energiaDoDia"].replace(" kWh", "").replace(",", ".")
+                    result["energiaDoDia"].split(" ")[0].replace(",", ".")
                 ),
+                today_energy_metric=result["energiaDoDia"].split(" ")[1],
                 power_factor=float(result["fatorpotencia"].replace(",", ".")),
                 frequency=result["frequencia"],
-                power=float(
-                    result["potenciaativa"].replace(" kW", "").replace(",", ".")
-                ),
+                power=float(result["potenciaativa"].split(" ")[0].replace(",", ".")),
+                power_metric=result["potenciaativa"].split(" ")[1],
                 status=Status(int(result["statusInversor"])),
                 temperature=result["temperatura"],
             )
 
             self._populate_MPPT(result=result, inverter=inverter)
 
             return inverter
@@ -201,24 +201,27 @@
         :type inverter: Inverter
         :param retry: reauthenticate if token expired and retry
         :type retry: bool
         """
         try:
             result = self._get(SUNWEG_INVERTER_DETAIL_PATH + str(inverter.id))
             inverter.total_energy = float(
-                result["energiaAcumulada"].replace(" kWh", "").replace(",", ".")
+                result["energiaAcumulada"].split(" ")[0].replace(",", ".")
             )
+            inverter.total_energy_metric = (result["energiaAcumulada"].split(" ")[1],)
             inverter.today_energy = float(
-                result["energiaDoDia"].replace(" kWh", "").replace(",", ".")
+                result["energiaDoDia"].split(" ")[0].replace(",", ".")
             )
+            inverter.today_energy_metric = (result["energiaDoDia"].split(" ")[1],)
             inverter.power_factor = float(result["fatorpotencia"].replace(",", "."))
             inverter.frequency = result["frequencia"]
             inverter.power = float(
-                result["potenciaativa"].replace(" kW", "").replace(",", ".")
+                result["potenciaativa"].split(" ")[0].replace(",", ".")
             )
+            inverter.power_metric = (result["potenciaativa"].split(" ")[1],)
 
             self._populate_MPPT(result=result, inverter=inverter)
         except LoginError:
             if retry:
                 self.authenticate()
                 self.complete_inverter(inverter, False)
```

### Comparing `sunweg-1.0.0/sunweg/const.py` & `sunweg-2.0.0b0/sunweg/const.py`

 * *Files identical despite different names*

### Comparing `sunweg-1.0.0/sunweg/device.py` & `sunweg-2.0.0b0/sunweg/device.py`

 * *Files 24% similar despite different names*

```diff
@@ -201,51 +201,63 @@
         self,
         id: int,
         name: str,
         sn: str,
         status: Status,
         temperature: int,
         total_energy: float = 0,
+        total_energy_metric: str = "",
         today_energy: float = 0,
+        today_energy_metric: str = "",
         power_factor: float = 0,
         frequency: float = 0,
         power: float = 0,
+        power_metric: str = "",
     ) -> None:
         """
         Initialize Inverter.
 
         :param id: inverter id
         :type id: int
         :param name: inverter name
         :type name: str
         :param sn: inverter serial number
         :type sn: str
         :param status: inverter status
         :type status: Status
         :param temperature: inverter temperature
         :type temperature: int
-        :param total_energy: total generated energy in kWh
+        :param total_energy: total generated energy
         :type total_energy: float
-        :param today_energy: total generated energy today in kWh
+        :param total_energy_metric: total generated energy metric
+        :type total_energy_metric: str
+        :param today_energy: total generated energy today
         :type today_energy: float
+        :param today_energy: total generated energy today metric
+        :type today_energy: str
         :param power_factor: inverter power factor
         :type power_factor: float
         :param frequency: inverter output frequency in Hz
         :type frequency: float
-        :param power: inverter output power in W
+        :param power: inverter output power
         :type power: float
+        :param power: inverter output power metric
+        :type power: str
         """
         self._id = id
         self._name = name
         self._sn = sn
         self._total_energy = total_energy
+        self._total_energy_metric = total_energy_metric
         self._today_energy = today_energy
+        self._today_energy_metric = today_energy_metric
         self._power_factor = power_factor
         self._frequency = frequency
         self._power = power
+        self._power_metric = power_metric
         self._status = status
         self._temperature = temperature
         self._phases: list[Phase] = []
         self._mppts: list[MPPT] = []
 
     @property
     def id(self) -> int:
@@ -296,52 +308,92 @@
         :rtype: int
         """
         return self._temperature
 
     @property
     def today_energy(self) -> float:
         """
-        Get inverter today generated energy in kWh.
+        Get inverter today generated energy.
 
-        :return: inverter today generated energy in kWh
+        :return: inverter today generated energy
         :rtype: float
         """
         return self._today_energy
 
     @today_energy.setter
     def today_energy(self, value: float) -> None:
         """
-        Set inverter today generated energy in kWh.
+        Set inverter today generated energy.
 
-        :param value: inverter today generated energy in kWh
+        :param value: inverter today generated energy
         :type value: float
         """
         self._today_energy = value
 
     @property
+    def today_energy_metric(self) -> str:
+        """
+        Get inverter today generated energy metric.
+
+        :return: inverter today generated energy metric
+        :rtype: str
+        """
+        return self._today_energy_metric
+
+    @today_energy_metric.setter
+    def today_energy_metric(self, value: str) -> None:
+        """
+        Set inverter today generated energy metric.
+
+        :param value: inverter today generated energy metric
+        :type value: str
+        """
+        self._today_energy_metric = value
+
+    @property
     def total_energy(self) -> float:
         """
-        Get inverter total generated energy in kWh.
+        Get inverter total generated energy.
 
-        :return: inverter total generated energy in kWh
+        :return: inverter total generated energy
         :rtype: float
         """
         return self._total_energy
 
     @total_energy.setter
     def total_energy(self, value: float) -> None:
         """
-        Set inverter total generated energy in kWh.
+        Set inverter total generated energy.
 
-        :param value: inverter total generated energy in kWh
+        :param value: inverter total generated energy
         :type value: float
         """
         self._total_energy = value
 
     @property
+    def total_energy_metric(self) -> str:
+        """
+        Get inverter total generated energy metric.
+
+        :return: inverter total generated energy metric
+        :rtype: str
+        """
+        return self._total_energy_metric
+
+    @total_energy_metric.setter
+    def total_energy_metric(self, value: str) -> None:
+        """
+        Set inverter total generated energy metric.
+
+        :param value: inverter total generated energy metric
+        :type value: str
+        """
+        self._total_energy_metric = value
+
+    @property
     def power_factor(self) -> float:
         """
         Get inverter power factor.
 
         :return: inverter power factor
         :rtype: float
         """
@@ -376,32 +428,52 @@
         :type value: float
         """
         self._frequency = value
 
     @property
     def power(self) -> float:
         """
-        Get inverter output power in W.
+        Get inverter output power.
 
-        :return: inverter output power in W
+        :return: inverter output power
         :rtype: float
         """
         return self._power
 
     @power.setter
     def power(self, value: float) -> None:
         """
-        Set inverter output power in W.
+        Set inverter output power.
 
-        :param value: inverter output power in W
+        :param value: inverter output power
         :type value: float
         """
         self._power = value
 
     @property
+    def power_metric(self) -> str:
+        """
+        Get inverter output power metric.
+
+        :return: inverter output power metric
+        :rtype: str
+        """
+        return self._power_metric
+
+    @power_metric.setter
+    def power_metric(self, value: str) -> None:
+        """
+        Set inverter output power metric.
+
+        :param value: inverter output power metric
+        :type value: float
+        """
+        self._power_metric = value
+
+    @property
     def is_complete(self) -> bool:
         """
         Is inverter data complete.
 
         :return: True when inverter data is complete
         :rtype: bool
         """
```

### Comparing `sunweg-1.0.0/sunweg/plant.py` & `sunweg-2.0.0b0/sunweg/plant.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         id: int,
         name: str,
         total_power: float,
         kwh_per_kwp: float,
         performance_rate: float,
         saving: float,
         today_energy: float,
+        today_energy_metric: str,
         total_energy: float,
         total_carbon_saving: float,
         last_update: datetime,
     ) -> None:
         """
         Initialize Plant.
 
@@ -31,30 +32,33 @@
         :type total_power: float
         :param kwh_per_kwp: plant kWh/kWp
         :type kwh_per_kwp: float
         :param performance_rate: plant performance rate
         :type performance_rate: float
         :param saving: total saving in R$
         :type saving: float
-        :param today_energy: today generated energy in kWh
+        :param today_energy: today generated energy
         :type today_energy: float
+        :param today_energy_metric: today generated energy metric
+        :type today_energy_metric: str
         :param total_energy: total generated energy in kWh
         :type total_energy: float
         :param total_carbon_saving: total of CO2 saved
         :type total_carbon_saving: float
         :param last_update: when the data was updated
         :type last_update: datetime
         """
         self._id = id
         self._name = name
         self._total_power = total_power
         self._kwh_per_kwp = kwh_per_kwp
         self._performance_rate = performance_rate
         self._saving = saving
         self._today_energy = today_energy
+        self._today_energy_metric = today_energy_metric
         self._total_energy = total_energy
         self._total_carbon_saving = total_carbon_saving
         self._last_update = last_update
         self._inverters: list[Inverter] = []
 
     @property
     def id(self) -> int:
@@ -115,22 +119,32 @@
         :rtype: float
         """
         return self._saving
 
     @property
     def today_energy(self) -> float:
         """
-        Get plant today generated energy in kWh.
+        Get plant today generated energy.
 
-        :return: plant today generated energy in kWh
+        :return: plant today generated energy
         :rtype: float
         """
         return self._today_energy
 
     @property
+    def today_energy_metric(self) -> str:
+        """
+        Get plant today generated energy metric.
+
+        :return: plant today generated energy metric
+        :rtype: str
+        """
+        return self._today_energy_metric
+
+    @property
     def total_energy(self) -> float:
         """
         Get plant total generated energy in kWh.
 
         :return: plant total generated energy in kWh
         :rtype: float
         """
```

### Comparing `sunweg-1.0.0/sunweg.egg-info/PKG-INFO` & `sunweg-2.0.0b0/sunweg.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunweg
-Version: 1.0.0
+Version: 2.0.0b0
 Summary: A library to retrieve data from sunweg.net
 Home-page: https://github.com/rokam/sunweg
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 # SunWeg
 
 [![Python build](https://github.com/rokam/sunweg/actions/workflows/python-build.yml/badge.svg)](https://github.com/rokam/sunweg/actions/workflows/python-build.yml)
 ![Python tests](https://raw.githubusercontent.com/rokam/sunweg/badges/tests.svg)
 ![Python coverage](https://raw.githubusercontent.com/rokam/sunweg/badges/coverage.svg)
 ![Python fake8](https://raw.githubusercontent.com/rokam/sunweg/badges/flake8.svg)
 
-Python lib for WEG solar energy platform, https://sunweg.net/
+Python lib for WEG solar energy platform, [SunWEG.net](https://sunweg.net/)
 
 ## Usage
 
 ``` python
 from sunweg.api import APIHelper
 
 api = APIHelper('username','password')
```

### Comparing `sunweg-1.0.0/tests/common.py` & `sunweg-2.0.0b0/tests/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,28 +9,32 @@
     id=1,
     name="Plant",
     total_power=29.2,
     kwh_per_kwp=0.1,
     performance_rate=0,
     saving=0,
     today_energy=123.1,
+    today_energy_metric="kWh",
     total_energy=321.1,
     total_carbon_saving=12.1,
     last_update=datetime.now(),
 )
 
 INVERTER_MOCK = Inverter(
     id=1,
     name="Inverter",
     sn="1234ABC",
     total_energy=321.1,
+    total_energy_metric="kWh",
     today_energy=123.1,
+    today_energy_metric="kWh",
     power_factor=0.2,
     frequency=60,
     power=29,
+    power_metric="kW",
     status=Status.OK,
     temperature=70,
 )
 
 MPPT_MOCK = MPPT("MPPT")
 
 STRING_MOCK = String(name="String", voltage=523.1, amperage=12.1, status=Status.OK)
```

### Comparing `sunweg-1.0.0/tests/test_api.py` & `sunweg-2.0.0b0/tests/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,29 +117,33 @@
             assert plant.name == "Plant Name"
             assert plant.total_power == 25.23
             assert plant.last_update == datetime(2023, 2, 25, 8, 4, 22)
             assert plant.kwh_per_kwp == 1.2
             assert plant.performance_rate == 1.48
             assert plant.saving == 12.786912
             assert plant.today_energy == 1.23
+            assert plant.today_energy_metric == "kWh"
             assert plant.total_carbon_saving == 0.012296
             assert plant.total_energy == 23.2
             assert plant.__str__().startswith("<class 'sunweg.plant.Plant'>")
             assert len(plant.inverters) == 1
             for inverter in plant.inverters:
                 assert inverter.id == 21255
                 assert inverter.name == "Inverter Name"
                 assert inverter.frequency == 0
                 assert inverter.power == 0.0
+                assert inverter.power_metric == ""
                 assert inverter.power_factor == 0.0
                 assert inverter.sn == "1234ABC"
                 assert inverter.status == Status.ERROR
                 assert inverter.temperature == 80
                 assert inverter.today_energy == 0.0
+                assert inverter.today_energy_metric == ""
                 assert inverter.total_energy == 0.0
+                assert inverter.total_energy_metric == ""
                 assert not inverter.is_complete
 
     def test_plant_401(self) -> None:
         """Test plant with expired token."""
         with patch(
             "requests.Session.post",
             return_value=self.responses["auth_success_response.json"],
@@ -159,20 +163,23 @@
             api = APIHelper("user@acme.com", "password")
             inverter = api.inverter(21255)
             assert inverter is not None
             assert inverter.id == 21255
             assert inverter.name == "Inverter Name"
             assert inverter.frequency == 0
             assert inverter.power == 0.0
+            assert inverter.power_metric == "kW"
             assert inverter.power_factor == 0.0
             assert inverter.sn == "1234ABC"
             assert inverter.status == Status.OK
             assert inverter.temperature == 80
             assert inverter.today_energy == 0.0
+            assert inverter.today_energy_metric == "kWh"
             assert inverter.total_energy == 23.2
+            assert inverter.today_energy_metric == "kWh"
             strings: list[String] = []
             for mppt in inverter.mppts:
                 assert mppt.__str__().startswith("<class 'sunweg.device.MPPT'>")
                 assert mppt.name != ""
                 strings.extend(mppt.strings)
             assert len(strings) == 4
             assert len(inverter.phases) == 3
```

