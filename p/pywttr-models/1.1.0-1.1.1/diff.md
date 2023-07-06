# Comparing `tmp/pywttr_models-1.1.0.tar.gz` & `tmp/pywttr_models-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywttr_models-1.1.0.tar", max compression
+gzip compressed data, was "pywttr_models-1.1.1.tar", max compression
```

## Comparing `pywttr_models-1.1.0.tar` & `pywttr_models-1.1.1.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0     1065 2022-11-26 19:30:08.923605 pywttr_models-1.1.0/LICENSE
--rw-r--r--   0        0        0      875 2022-11-26 19:30:08.923605 pywttr_models-1.1.0/README.md
--rw-r--r--   0        0        0     2621 2022-11-26 19:33:57.122987 pywttr_models-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      828 2022-11-26 19:32:02.465798 pywttr_models-1.1.0/pywttr_models/__init__.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/af.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/am.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/ar.py
--rw-r--r--   0        0        0     4601 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/base.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/be.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/bn.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/ca.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/da.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/de.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/el.py
--rw-r--r--   0        0        0      266 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/en.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/et.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/fa.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/fr.py
--rw-r--r--   0        0        0      416 2022-11-26 19:32:12.458815 pywttr_models-1.1.0/pywttr_models/gl.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/hi.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/hu.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/ia.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/id.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/it.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/lt.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.924605 pywttr_models-1.1.0/pywttr_models/mg.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/nb.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/nl.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/oc.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/pl.py
--rw-r--r--   0        0        0      516 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/pt_br.py
--rw-r--r--   0        0        0        0 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/py.typed
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/ro.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/ru.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/ta.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/th.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/tr.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/uk.py
--rw-r--r--   0        0        0      416 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/vi.py
--rw-r--r--   0        0        0      516 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/zh_cn.py
--rw-r--r--   0        0        0      516 2022-11-26 19:30:08.925605 pywttr_models-1.1.0/pywttr_models/zh_tw.py
--rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 pywttr_models-1.1.0/setup.py
--rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 pywttr_models-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-06 15:16:43.811679 pywttr_models-1.1.1/LICENSE
+-rw-r--r--   0        0        0      515 2023-07-06 15:16:43.811679 pywttr_models-1.1.1/README.md
+-rw-r--r--   0        0        0     2772 2023-07-06 15:16:43.811679 pywttr_models-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      787 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/__init__.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/af.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/am.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/ar.py
+-rw-r--r--   0        0        0     4415 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/base.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/be.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/bn.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/ca.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/da.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/de.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/el.py
+-rw-r--r--   0        0        0      266 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/en.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/et.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/fa.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/fr.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/gl.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/hi.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/hu.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/ia.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/id.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/it.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/lt.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/mg.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/nb.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/nl.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/oc.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/pl.py
+-rw-r--r--   0        0        0      597 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/pt_br.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/py.typed
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/ro.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/ru.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/ta.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/th.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/tr.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/uk.py
+-rw-r--r--   0        0        0      416 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/vi.py
+-rw-r--r--   0        0        0      597 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/zh_cn.py
+-rw-r--r--   0        0        0      597 2023-07-06 15:16:43.815679 pywttr_models-1.1.1/pywttr_models/zh_tw.py
+-rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 pywttr_models-1.1.1/PKG-INFO
```

### Comparing `pywttr_models-1.1.0/LICENSE` & `pywttr_models-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywttr_models-1.1.0/pywttr_models/base.py` & `pywttr_models-1.1.1/pywttr_models/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 from typing import List
 
-from pydantic import BaseModel, Field
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:
+    from pydantic import BaseModel, Field  # type: ignore[assignment]
 
 
 class LangItem(BaseModel):
     value: str
 
 
 class WeatherDescItem(BaseModel):
@@ -14,38 +17,36 @@
 
 
 class WeatherIconUrlItem(BaseModel):
     value: str
 
 
 class CurrentConditionItem(BaseModel):
-    feels_like_c: str = Field(..., alias="FeelsLikeC")
-    feels_like_f: str = Field(..., alias="FeelsLikeF")
+    feels_like_c: str = Field(alias="FeelsLikeC")
+    feels_like_f: str = Field(alias="FeelsLikeF")
     cloudcover: str
     humidity: str
-    local_obs_date_time: str = Field(..., alias="localObsDateTime")
+    local_obs_date_time: str = Field(alias="localObsDateTime")
     observation_time: str
-    precip_inches: str = Field(..., alias="precipInches")
-    precip_mm: str = Field(..., alias="precipMM")
+    precip_inches: str = Field(alias="precipInches")
+    precip_mm: str = Field(alias="precipMM")
     pressure: str
-    pressure_inches: str = Field(..., alias="pressureInches")
-    temp_c: str = Field(..., alias="temp_C")
-    temp_f: str = Field(..., alias="temp_F")
-    uv_index: str = Field(..., alias="uvIndex")
+    pressure_inches: str = Field(alias="pressureInches")
+    temp_c: str = Field(alias="temp_C")
+    temp_f: str = Field(alias="temp_F")
+    uv_index: str = Field(alias="uvIndex")
     visibility: str
-    visibility_miles: str = Field(..., alias="visibilityMiles")
-    weather_code: str = Field(..., alias="weatherCode")
-    weather_desc: List[WeatherDescItem] = Field(..., alias="weatherDesc")
-    weather_icon_url: List[WeatherIconUrlItem] = Field(
-        ..., alias="weatherIconUrl"
-    )
-    winddir16_point: str = Field(..., alias="winddir16Point")
-    winddir_degree: str = Field(..., alias="winddirDegree")
-    windspeed_kmph: str = Field(..., alias="windspeedKmph")
-    windspeed_miles: str = Field(..., alias="windspeedMiles")
+    visibility_miles: str = Field(alias="visibilityMiles")
+    weather_code: str = Field(alias="weatherCode")
+    weather_desc: List[WeatherDescItem] = Field(alias="weatherDesc")
+    weather_icon_url: List[WeatherIconUrlItem] = Field(alias="weatherIconUrl")
+    winddir16_point: str = Field(alias="winddir16Point")
+    winddir_degree: str = Field(alias="winddirDegree")
+    windspeed_kmph: str = Field(alias="windspeedKmph")
+    windspeed_miles: str = Field(alias="windspeedMiles")
 
 
 class AreaNameItem(BaseModel):
     value: str
 
 
 class CountryItem(BaseModel):
@@ -57,21 +58,21 @@
 
 
 class WeatherUrlItem(BaseModel):
     value: str
 
 
 class NearestAreaItem(BaseModel):
-    area_name: List[AreaNameItem] = Field(..., alias="areaName")
+    area_name: List[AreaNameItem] = Field(alias="areaName")
     country: List[CountryItem]
     latitude: str
     longitude: str
     population: str
     region: List[RegionItem]
-    weather_url: List[WeatherUrlItem] = Field(..., alias="weatherUrl")
+    weather_url: List[WeatherUrlItem] = Field(alias="weatherUrl")
 
 
 class RequestItem(BaseModel):
     query: str
     type: str
 
 
@@ -89,67 +90,65 @@
 
 
 class WeatherIconUrlItem1(BaseModel):
     value: str
 
 
 class HourlyItem(BaseModel):
-    dew_point_c: str = Field(..., alias="DewPointC")
-    dew_point_f: str = Field(..., alias="DewPointF")
-    feels_like_c: str = Field(..., alias="FeelsLikeC")
-    feels_like_f: str = Field(..., alias="FeelsLikeF")
-    heat_index_c: str = Field(..., alias="HeatIndexC")
-    heat_index_f: str = Field(..., alias="HeatIndexF")
-    wind_chill_c: str = Field(..., alias="WindChillC")
-    wind_chill_f: str = Field(..., alias="WindChillF")
-    wind_gust_kmph: str = Field(..., alias="WindGustKmph")
-    wind_gust_miles: str = Field(..., alias="WindGustMiles")
+    dew_point_c: str = Field(alias="DewPointC")
+    dew_point_f: str = Field(alias="DewPointF")
+    feels_like_c: str = Field(alias="FeelsLikeC")
+    feels_like_f: str = Field(alias="FeelsLikeF")
+    heat_index_c: str = Field(alias="HeatIndexC")
+    heat_index_f: str = Field(alias="HeatIndexF")
+    wind_chill_c: str = Field(alias="WindChillC")
+    wind_chill_f: str = Field(alias="WindChillF")
+    wind_gust_kmph: str = Field(alias="WindGustKmph")
+    wind_gust_miles: str = Field(alias="WindGustMiles")
     chanceoffog: str
     chanceoffrost: str
     chanceofhightemp: str
     chanceofovercast: str
     chanceofrain: str
     chanceofremdry: str
     chanceofsnow: str
     chanceofsunshine: str
     chanceofthunder: str
     chanceofwindy: str
     cloudcover: str
     humidity: str
-    precip_inches: str = Field(..., alias="precipInches")
-    precip_mm: str = Field(..., alias="precipMM")
+    precip_inches: str = Field(alias="precipInches")
+    precip_mm: str = Field(alias="precipMM")
     pressure: str
-    pressure_inches: str = Field(..., alias="pressureInches")
-    temp_c: str = Field(..., alias="tempC")
-    temp_f: str = Field(..., alias="tempF")
+    pressure_inches: str = Field(alias="pressureInches")
+    temp_c: str = Field(alias="tempC")
+    temp_f: str = Field(alias="tempF")
     time: str
-    uv_index: str = Field(..., alias="uvIndex")
+    uv_index: str = Field(alias="uvIndex")
     visibility: str
-    visibility_miles: str = Field(..., alias="visibilityMiles")
-    weather_code: str = Field(..., alias="weatherCode")
-    weather_desc: List[WeatherDescItem1] = Field(..., alias="weatherDesc")
-    weather_icon_url: List[WeatherIconUrlItem1] = Field(
-        ..., alias="weatherIconUrl"
-    )
-    winddir16_point: str = Field(..., alias="winddir16Point")
-    winddir_degree: str = Field(..., alias="winddirDegree")
-    windspeed_kmph: str = Field(..., alias="windspeedKmph")
-    windspeed_miles: str = Field(..., alias="windspeedMiles")
+    visibility_miles: str = Field(alias="visibilityMiles")
+    weather_code: str = Field(alias="weatherCode")
+    weather_desc: List[WeatherDescItem1] = Field(alias="weatherDesc")
+    weather_icon_url: List[WeatherIconUrlItem1] = Field(alias="weatherIconUrl")
+    winddir16_point: str = Field(alias="winddir16Point")
+    winddir_degree: str = Field(alias="winddirDegree")
+    windspeed_kmph: str = Field(alias="windspeedKmph")
+    windspeed_miles: str = Field(alias="windspeedMiles")
 
 
 class WeatherItem(BaseModel):
     astronomy: List[AstronomyItem]
-    avgtemp_c: str = Field(..., alias="avgtempC")
-    avgtemp_f: str = Field(..., alias="avgtempF")
+    avgtemp_c: str = Field(alias="avgtempC")
+    avgtemp_f: str = Field(alias="avgtempF")
     date: str
-    maxtemp_c: str = Field(..., alias="maxtempC")
-    maxtemp_f: str = Field(..., alias="maxtempF")
-    mintemp_c: str = Field(..., alias="mintempC")
-    mintemp_f: str = Field(..., alias="mintempF")
-    sun_hour: str = Field(..., alias="sunHour")
-    total_snow_cm: str = Field(..., alias="totalSnow_cm")
-    uv_index: str = Field(..., alias="uvIndex")
+    maxtemp_c: str = Field(alias="maxtempC")
+    maxtemp_f: str = Field(alias="maxtempF")
+    mintemp_c: str = Field(alias="mintempC")
+    mintemp_f: str = Field(alias="mintempF")
+    sun_hour: str = Field(alias="sunHour")
+    total_snow_cm: str = Field(alias="totalSnow_cm")
+    uv_index: str = Field(alias="uvIndex")
 
 
 class Model(BaseModel):
     nearest_area: List[NearestAreaItem]
     request: List[RequestItem]
```

### Comparing `pywttr_models-1.1.0/pywttr_models/pt_br.py` & `pywttr_models-1.1.1/pywttr_models/zh_cn.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 from typing import List
 
-from pydantic import Field
+try:
+    from pydantic.v1 import Field
+except ImportError:
+    from pydantic import Field  # type: ignore[assignment]
 
 from . import base
 
 
 class CurrentConditionItem(base.CurrentConditionItem):
-    lang_pt_br: List[base.LangItem] = Field(..., alias="lang_pt-br")
+    lang_zh_cn: List[base.LangItem] = Field(alias="lang_zh-cn")
 
 
 class HourlyItem(base.HourlyItem):
-    lang_pt_br: List[base.LangItem] = Field(..., alias="lang_pt-br")
+    lang_zh_cn: List[base.LangItem] = Field(alias="lang_zh-cn")
 
 
 class WeatherItem(base.WeatherItem):
     hourly: List[HourlyItem]
 
 
 class Model(base.Model):
```

### Comparing `pywttr_models-1.1.0/pywttr_models/zh_tw.py` & `pywttr_models-1.1.1/pywttr_models/zh_tw.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 from typing import List
 
-from pydantic import Field
+try:
+    from pydantic.v1 import Field
+except ImportError:
+    from pydantic import Field  # type: ignore[assignment]
 
 from . import base
 
 
 class CurrentConditionItem(base.CurrentConditionItem):
-    lang_zh_tw: List[base.LangItem] = Field(..., alias="lang_zh-tw")
+    lang_zh_tw: List[base.LangItem] = Field(alias="lang_zh-tw")
 
 
 class HourlyItem(base.HourlyItem):
-    lang_zh_tw: List[base.LangItem] = Field(..., alias="lang_zh-tw")
+    lang_zh_tw: List[base.LangItem] = Field(alias="lang_zh-tw")
 
 
 class WeatherItem(base.WeatherItem):
     hourly: List[HourlyItem]
 
 
 class Model(base.Model):
```

### Comparing `pywttr_models-1.1.0/PKG-INFO` & `pywttr_models-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: pywttr-models
-Version: 1.1.0
+Version: 1.1.1
 Summary: Pydantic models for pywttr and aiopywttr
 Home-page: https://github.com/monosans/pywttr-models
 License: MIT
 Keywords: forecast,weather
 Author: monosans
 Author-email: hsyqixco@protonmail.com
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.7,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 1
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: pydantic (>=1.9,<2.0)
+Requires-Dist: pydantic (>=1.9,<3)
 Project-URL: Repository, https://github.com/monosans/pywttr-models
 Description-Content-Type: text/markdown
 
 # pywttr-models
 
-[![CI](https://github.com/monosans/pywttr-models/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/pywttr-models/actions/workflows/ci.yml)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/pywttr-models/main.svg)](https://results.pre-commit.ci/latest/github/monosans/pywttr-models/main)
-
-[Pydantic](https://github.com/samuelcolvin/pydantic) models for [pywttr](https://github.com/monosans/pywttr) and [aiopywttr](https://github.com/monosans/aiopywttr).
-
-## Usage for type annotation
-
-```python
-import pywttr_models
-
-
-def do_something(model: pywttr_models.en.Model):
-    ...
-```
+[![CI](https://github.com/monosans/pywttr-models/actions/workflows/ci.yml/badge.svg)](https://github.com/monosans/pywttr-models/actions/workflows/ci.yml)
+[![Downloads](https://static.pepy.tech/badge/pywttr-models)](https://pepy.tech/project/pywttr-models)
 
-Other languages may also be used instead of `en`. For a complete list of supported languages, follow the code completion in your IDE.
+[Pydantic](https://github.com/pydantic/pydantic) models for [pywttr](https://github.com/monosans/pywttr) and [aiopywttr](https://github.com/monosans/aiopywttr).
 
 ## License
 
 [MIT](https://github.com/monosans/pywttr-models/blob/main/LICENSE)
```

