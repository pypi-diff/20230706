# Comparing `tmp/carbon_guard-0.6.0.tar.gz` & `tmp/carbon_guard-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbon_guard-0.6.0.tar", max compression
+gzip compressed data, was "carbon_guard-0.7.0.tar", max compression
```

## Comparing `carbon_guard-0.6.0.tar` & `carbon_guard-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,19 @@
--rw-r--r--   0        0        0    10851 2023-07-06 09:09:56.931843 carbon_guard-0.6.0/README.md
--rw-r--r--   0        0        0     1097 2023-07-06 09:09:56.931843 carbon_guard-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 09:09:56.931843 carbon_guard-0.6.0/src/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 09:09:56.931843 carbon_guard-0.6.0/src/cli/__init__.py
--rw-r--r--   0        0        0      312 2023-07-06 09:09:56.931843 carbon_guard-0.6.0/src/cli/async_helper.py
--rw-r--r--   0        0        0       76 2023-07-06 09:09:56.931843 carbon_guard-0.6.0/src/cli/parsers.py
--rw-r--r--   0        0        0     5374 2023-07-06 09:09:56.931843 carbon_guard-0.6.0/src/main.py
--rw-r--r--   0        0        0        0 2023-07-06 09:09:56.931843 carbon_guard-0.6.0/src/repos/__init__.py
--rw-r--r--   0        0        0     2887 2023-07-06 09:09:56.931843 carbon_guard-0.6.0/src/repos/carbon_intensity.py
--rw-r--r--   0        0        0    11291 1970-01-01 00:00:00.000000 carbon_guard-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0    16613 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/README.md
+-rw-r--r--   0        0        0     1178 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/cli/__init__.py
+-rw-r--r--   0        0        0      312 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/cli/async_helper.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/cli/command/__init__.py
+-rw-r--r--   0        0        0     1082 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/cli/command/check.py
+-rw-r--r--   0        0        0      404 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/cli/command/schedule.py
+-rw-r--r--   0        0        0      911 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/cli/parsers.py
+-rw-r--r--   0        0        0     5041 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/main.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/repos/carbon_intensity/__init__.py
+-rw-r--r--   0        0        0     1227 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/repos/carbon_intensity/co2_signal.py
+-rw-r--r--   0        0        0     1421 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/repos/carbon_intensity/file.py
+-rw-r--r--   0        0        0     1052 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/repos/carbon_intensity/in_memory.py
+-rw-r--r--   0        0        0     2034 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/repos/carbon_intensity/national_grid_eso.py
+-rw-r--r--   0        0        0     3389 2023-07-06 14:32:50.211308 carbon_guard-0.7.0/src/repos/carbon_intensity/protocol.py
+-rw-r--r--   0        0        0    17149 1970-01-01 00:00:00.000000 carbon_guard-0.7.0/PKG-INFO
```

### Comparing `carbon_guard-0.6.0/README.md` & `carbon_guard-0.7.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,65 @@
+Metadata-Version: 2.1
+Name: carbon-guard
+Version: 0.7.0
+Summary: 
+Author: Adam Gardner
+Author-email: adam.gardner@armakuni.com
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dateparser (>=1.1.8,<2.0.0)
+Requires-Dist: httpx[brotli,http2] (>=0.24.1,<0.25.0)
+Requires-Dist: pydantic[dotenv] (>=2.0,<3.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: types-dateparser (>=1.1.4.9,<2.0.0.0)
+Description-Content-Type: text/markdown
+
 # Carbon Guard 👮
 
 Carbon Guard is a unique and environmentally conscious GitHub Action & CLI App
 designed to help reduce the carbon footprint of your CI/CD pipelines. It
 works by monitoring real-time carbon intensity data and preventing
 pipelines from running when the carbon intensity is high.
 
 ## Usage
 
+
 ```shell,script(name="usage",expected_exit_code=0)
 poetry run carbon_guard --help
 ```
 
 ``` ,verify(script_name="usage",stream=stdout)
                                                                                 
- Usage: carbon_guard [OPTIONS]                                                  
+ Usage: carbon_guard [OPTIONS] COMMAND [ARGS]...                                
+                                                                                
+╭─ Options ────────────────────────────────────────────────────────────────────╮
+│ --install-completion          Install completion for the current shell.      │
+│ --show-completion             Show completion for the current shell, to copy │
+│                               it or customize the installation.              │
+│ --help                        Show this message and exit.                    │
+╰──────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ───────────────────────────────────────────────────────────────────╮
+│ check            Check the current carbon intensity.                         │
+│ schedule         Find the lowest carbon time.                                │
+╰──────────────────────────────────────────────────────────────────────────────╯
+
+```
+
+### Check
+
+```shell,script(name="usage-check",expected_exit_code=0)
+poetry run carbon_guard check --help
+```
+
+``` ,verify(script_name="usage-check",stream=stdout)
+                                                                                
+ Usage: carbon_guard check [OPTIONS]                                            
+                                                                                
+ Check the current carbon intensity.                                            
                                                                                 
 ╭─ Options ────────────────────────────────────────────────────────────────────╮
 │ *  --max-carbon-in…                       INTEGER           Set the max      │
 │                                                             carbon intensity │
 │                                                             in gCO2eq/kWh.   │
 │                                                             [env var:        │
 │                                                             MAX_CARBON_INTE… │
@@ -44,24 +86,24 @@
 │                                                             carbon intensity │
 │                                                             from in file     │
 │                                                             mode             │
 │                                                             [env var:        │
 │                                                             FROM_FILE_CARBO… │
 │                                                             [default:        │
 │                                                             .carbon_intensi… │
-│    --nation-grid-e…                       PARSE_URL         URL for the      │
-│                                                             National Grid    │
+│    --national-grid…                       HTTP_OR_HTTPS_UR  URL for the      │
+│                                           L                 National Grid    │
 │                                                             ESO Carbon       │
 │                                                             Intensity API    │
 │                                                             [env var:        │
 │                                                             NATIONAL_GRID_E… │
 │                                                             [default:        │
 │                                                             https://api.car… │
-│    --co2-signal-ca…                       PARSE_URL         URL for the CO2  │
-│                                                             Signal api       │
+│    --co2-signal-ca…                       HTTP_OR_HTTPS_UR  URL for the CO2  │
+│                                           L                 Signal api       │
 │                                                             [env var:        │
 │                                                             CO2_SIGNAL_API_… │
 │                                                             [default:        │
 │                                                             https://api.co2… │
 │    --co2-signal-ap…                       TEXT              Api key for the  │
 │                                                             CO2 Signal api,  │
 │                                                             required in CO2  │
@@ -79,42 +121,87 @@
 │    --help                                                   Show this        │
 │                                                             message and      │
 │                                                             exit.            │
 ╰──────────────────────────────────────────────────────────────────────────────╯
 
 ```
 
+### Schedule
+
+```shell,script(name="usage-schedule",expected_exit_code=0)
+poetry run carbon_guard schedule --help
+```
+
+``` ,verify(script_name="usage-schedule",stream=stdout)
+                                                                                
+ Usage: carbon_guard schedule [OPTIONS]                                         
+                                                                                
+ Find the lowest carbon time.                                                   
+                                                                                
+╭─ Options ────────────────────────────────────────────────────────────────────╮
+│ *  --within                     HUMAN_READABLE_DURATI  Time period to        │
+│                                 ON                     predict the lowest    │
+│                                                        intensity within      │
+│                                                        [env var: WITHIN]     │
+│                                                        [default: None]       │
+│                                                        [required]            │
+│    --data-source                [file|national-grid-e  Where to read carbon  │
+│                                 so-carbon-intensity]   intensity data from   │
+│                                                        [env var:             │
+│                                                        DATA_SOURCE]          │
+│                                                        [default:             │
+│                                                        national-grid-eso-ca… │
+│    --from-file-carbon-i…        PATH                   File to read carbon   │
+│                                                        intensity from in     │
+│                                                        file mode             │
+│                                                        [env var:             │
+│                                                        FROM_FILE_CARBON_INT… │
+│                                                        [default:             │
+│                                                        .carbon_intensity]    │
+│    --national-grid-eso-…        HTTP_OR_HTTPS_URL      URL for the National  │
+│                                                        Grid ESO Carbon       │
+│                                                        Intensity API         │
+│                                                        [env var:             │
+│                                                        NATIONAL_GRID_ESO_CA… │
+│                                                        [default:             │
+│                                                        https://api.carbonin… │
+│    --help                                              Show this message and │
+│                                                        exit.                 │
+╰──────────────────────────────────────────────────────────────────────────────╯
+
+```
+
 ### Common use case
 
 When comparing current carbon intensity levels to global carbon intensity
 based on gCO2eq/kWh.
 
 Comparing carbon levels with the expected outcome for high carbon intensity:
 
 ```shell,script(name="carbon_threshold_exceeded",  expected_exit_code=1)
 carbon_intensity_is 1000
-poetry run carbon_guard --max-carbon-intensity=999
+poetry run carbon_guard check --max-carbon-intensity=999
 ```
 
 ``` ,verify(script_name="carbon_threshold_exceeded", stream=stdout)
 Carbon intensity is 1000 gCO2eq/kWh, which is above the max of 999 gCO2eq/kWh
 ```
 
 You may also return a successful exit code even on high carbon intensity by passing the `--advise-only` flag.
 
 ```shell,script(name="carbon_threshold_exceeded_and_skipped",  expected_exit_code=0)
 carbon_intensity_is 1000
-poetry run carbon_guard --max-carbon-intensity=999 --advise-only
+poetry run carbon_guard check --max-carbon-intensity=999 --advise-only
 ```
 
 Comparing carbon levels with the expected outcome for low carbon intensity:
 
 ```shell,script(name="carbon_threshold_ok",  expected_exit_code=0)
 carbon_intensity_is 999
-poetry run carbon_guard --max-carbon-intensity=999
+poetry run carbon_guard check --max-carbon-intensity=999
 ```
 
 ``` ,verify(script_name="carbon_threshold_ok", stream=stdout)
 Carbon intensity is 999 gCO2eq/kWh, which is below or equal to the max of 999 gCO2eq/kWh
 ```
 
 ## Data Sources
@@ -126,53 +213,61 @@
 
 ## National Grid ESO Carbon Intensity
 
 Using the [national-grid-eso-carbon-intensity data source](https://carbonintensity.org.uk/).
 [**note**] this only supplies data for the United Kingdom.
 
 ```shell,script(name="national_grid_eso_carbon_threshold_ok",  expected_exit_code=0)
-poetry run carbon_guard --data-source national-grid-eso-carbon-intensity --max-carbon-intensity=100000
+poetry run carbon_guard check --data-source national-grid-eso-carbon-intensity --max-carbon-intensity=100000
 ```
 
 ``` ,skip()
 Carbon intensity is 98 gCO2eq/kWh, which is below or equal to the max of 100000 gCO2eq/kWh
 ```
 
+```shell,script(name="national_grid_eso_carbon_threshold_ok",  expected_exit_code=0)
+poetry run carbon_guard schedule --data-source national-grid-eso-carbon-intensity --within "1 hour"
+```
+
+``` ,skip()
+2023-07-07T09:30:00+00:00
+```
+
 ### CO2 Signal
 
 Using the [co2-signal data source](https://www.co2signal.com/)
-[**note**] This data source requires an account (free/paid) which will supply an API key for usage.
+[**note**] This data source requires an account (free/paid) which will supply an API key for usage, and does not support forecasting.
 
 ```shell,script(name="co2-signal-carbon-threshold-ok",  expected_exit_code=0)
 # export CO2_SIGNAL_API_KEY=<your_api_key_here>
-poetry run carbon_guard --data-source co2-signal --max-carbon-intensity=100000 --co2-signal-country-code=GB
+poetry run carbon_guard check --data-source co2-signal --max-carbon-intensity=100000 --co2-signal-country-code=GB
 ```
 
 ``` ,skip()
 Carbon intensity is 107 gCO2eq/kWh, which is below or equal to the max of 100000 gCO2eq/kWh
 ```
 
 #### Errors
 
 if you don't provide a `co2-signal-country-code` the call will fail.
 
 ```shell,script(name="co2-signal-no-country-code-error",  expected_exit_code=1)
 # export CO2_SIGNAL_API_KEY=<your_api_key_here>
-poetry run carbon_guard --data-source co2-signal --max-carbon-intensity=100000
+poetry run carbon_guard check --data-source co2-signal --max-carbon-intensity=100000
 ```
 
 ``` ,verify(script_name="co2-signal-no-country-code-error", stream=stdout)
 No country code provided to CO2 Signal Api.
 ```
 
 if you don't provide a `co2-signal-api-key` the call will fail.
 
 ```shell,script(name="co2-signal-no-api-key-error",  expected_exit_code=1)
 export CO2_SIGNAL_API_KEY=""
-poetry run carbon_guard --data-source co2-signal --max-carbon-intensity=100000 --co2-signal-country-code=GB
+poetry run carbon_guard check --data-source co2-signal --max-carbon-intensity=100000 --co2-signal-country-code=GB
 ```
 
 ``` ,verify(script_name="co2-signal-no-api-key-error", stream=stdout)
 No API key found for CO2 Signal API.
 ```
 
 ## Adding to your pipelines
@@ -213,8 +308,8 @@
 ### Other pipelines
 
 You can run in other pipelines as a command line tool
 
 ```shell, skip()
 pip install git+https://github.com/armakuni/carbon-guard.git
 carbon_guard --help
-```
+```
```

### Comparing `carbon_guard-0.6.0/pyproject.toml` & `carbon_guard-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 [tool.poetry]
 name = "carbon_guard"
-version = "0.6.0"
+version = "0.7.0"
 description = ""
 authors = [
   "Adam Gardner <adam.gardner@armakuni.com>",
   "Billie Thompson <billie.thompson@armakuni.com>",
 ]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typer = {extras = ["all"], version = "^0.9.0"}
 httpx = {extras = ["brotli", "http2"], version = "^0.24.1"}
 pydantic = {extras = ["dotenv"], version = "^2.0"}
+dateparser = "^1.1.8"
+types-dateparser = "^1.1.4.9"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 ruff = "^0.0.277"
 mypy = "^1.4.0"
 pytest = "^7.3.2"
 wiremock = "^2.5.0"
 pytest-asyncio = "^0.21.0"
+pytest-freezegun = "^0.4.2"
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `carbon_guard-0.6.0/src/main.py` & `carbon_guard-0.7.0/src/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-from enum import StrEnum
+import datetime as dt
 from pathlib import Path
 from typing import Optional
 
 import typer
 from httpx import URL
 from typing_extensions import Annotated
 
-from src.cli.async_helper import async_to_sync
-from src.cli.parsers import parse_url
-from src.repos.carbon_intensity import (
-    CarbonIntensityRepo,
-    CO2SignalCarbonIntensityRepo,
-    FromFileCarbonIntensityRepo,
-    NationalGridESOCarbonIntensityApiRepo,
+from src.cli.command.check import run as check_run
+from src.cli.command.schedule import run as schedule_run
+from src.cli.parsers import http_or_https_url, human_readable_duration
+from src.repos.carbon_intensity.protocol import (
+    CurrentIntensityDataSource,
+    ForecastLowIntensityDateDataSource,
+    MissingParameterError,
+    make_current_intensity_repo,
+    make_forecast_low_intensity_date_repo,
 )
 
 NATIONAL_GRID_ESO_CARBON_INTENSITY_API_BASE_URL: URL = URL(
     "https://api.carbonintensity.org.uk"
 )
 CO2_SIGNAL_API_BASE_URL: URL = URL("https://api.co2signal.com")
 FILE_FOR_INTENSITY_READING: str = ".carbon_intensity"
-SUCCESS_TEMPLATE: str = "Carbon intensity is {carbon_intensity} gCO2eq/kWh, which is below or equal to the max of {max_carbon_intensity} gCO2eq/kWh"
-FAILURE_TEMPLATE: str = "Carbon intensity is {carbon_intensity} gCO2eq/kWh, which is above the max of {max_carbon_intensity} gCO2eq/kWh"
 
+app = typer.Typer()
 
-class DataSource(StrEnum):
-    FILE = "file"
-    NATIONAL_GRID_ESO_CARBON_INTENSITY = "national-grid-eso-carbon-intensity"
-    CO2_SIGNAL = "co2-signal"
 
-
-def main(
+@app.command(help="Check the current carbon intensity.")
+def check(
     max_carbon_intensity: Annotated[
         int,
         typer.Option(
             envvar="MAX_CARBON_INTENSITY",
             help="Set the max carbon intensity in gCO2eq/kWh.",
         ),
     ],
@@ -42,42 +39,42 @@
         bool,
         typer.Option(
             envvar="ADVISE_ONLY",
             help="Do not exit with an error if the carbon intensity is above the max carbon intensity.",
         ),
     ] = False,
     data_source: Annotated[
-        DataSource,
+        CurrentIntensityDataSource,
         typer.Option(
             case_sensitive=False,
             envvar="DATA_SOURCE",
             help="Where to read carbon intensity data from",
         ),
-    ] = DataSource.NATIONAL_GRID_ESO_CARBON_INTENSITY,
+    ] = CurrentIntensityDataSource.NATIONAL_GRID_ESO_CARBON_INTENSITY,
     from_file_carbon_intensity_file_path: Annotated[
         Path,
         typer.Option(
             envvar="FROM_FILE_CARBON_INTENSITY_FILE_PATH",
             help="File to read carbon intensity from in file mode",
         ),
     ] = Path(FILE_FOR_INTENSITY_READING),
-    nation_grid_eso_carbon_intensity_api_base_url: Annotated[
+    national_grid_eso_carbon_intensity_api_base_url: Annotated[
         URL,
         typer.Option(
             envvar="NATIONAL_GRID_ESO_CARBON_INTENSITY_API_BASE_URL",
             help="URL for the National Grid ESO Carbon Intensity API",
-            parser=parse_url,
+            parser=http_or_https_url,
         ),
     ] = NATIONAL_GRID_ESO_CARBON_INTENSITY_API_BASE_URL,
     co2_signal_carbon_intensity_api_base_url: Annotated[
         URL,
         typer.Option(
             envvar="CO2_SIGNAL_API_BASE_URL",
             help="URL for the CO2 Signal api",
-            parser=parse_url,
+            parser=http_or_https_url,
         ),
     ] = CO2_SIGNAL_API_BASE_URL,
     co2_signal_api_key: Annotated[
         Optional[str],
         typer.Option(
             envvar="CO2_SIGNAL_API_KEY",
             help="Api key for the CO2 Signal api, required in CO2 Signal mode",
@@ -87,72 +84,78 @@
         Optional[str],
         typer.Option(
             envvar="CO2_SIGNAL_COUNTRY_CODE",
             help="Country code to get the carbon intensity from CO2 Signal api",
         ),
     ] = None,
 ) -> None:
-    carbon_intensity(
-        data_source,
-        advise_only,
-        from_file_carbon_intensity_file_path,
+    try:
+        intensity_repo = make_current_intensity_repo(
+            co2_signal_api_key,
+            co2_signal_carbon_intensity_api_base_url,
+            co2_signal_country_code,
+            data_source,
+            from_file_carbon_intensity_file_path,
+            national_grid_eso_carbon_intensity_api_base_url,
+        )
+    except MissingParameterError as e:
+        typer.echo(f"{e}")
+        raise typer.Exit(1) from e
+
+    check_run(
         max_carbon_intensity,
-        nation_grid_eso_carbon_intensity_api_base_url,
-        co2_signal_carbon_intensity_api_base_url,
-        co2_signal_api_key,
-        co2_signal_country_code,
+        advise_only,
+        intensity_repo,
     )
 
 
-@async_to_sync
-async def carbon_intensity(
-    data_source: DataSource,
-    advise_only: bool,
-    from_file_carbon_intensity_file_path: Path,
-    max_carbon_intensity: int,
-    national_grid_eso_carbon_intensity_api_base_url: URL,
-    co2_signal_carbon_intensity_api_base_url: URL,
-    co2_signal_api_key: Optional[str],
-    co2_signal_country_code: Optional[str],
+@app.command(help="Find the lowest carbon time.")
+def schedule(
+    within: Annotated[
+        dt.timedelta,
+        typer.Option(
+            envvar="WITHIN",
+            help="Time period to predict the lowest intensity within",  #
+            parser=human_readable_duration,
+        ),
+    ],
+    data_source: Annotated[
+        ForecastLowIntensityDateDataSource,
+        typer.Option(
+            case_sensitive=False,
+            envvar="DATA_SOURCE",
+            help="Where to read carbon intensity data from",
+        ),
+    ] = ForecastLowIntensityDateDataSource.NATIONAL_GRID_ESO_CARBON_INTENSITY,
+    from_file_carbon_intensity_file_path: Annotated[
+        Path,
+        typer.Option(
+            envvar="FROM_FILE_CARBON_INTENSITY_FILE_PATH",
+            help="File to read carbon intensity from in file mode",
+        ),
+    ] = Path(FILE_FOR_INTENSITY_READING),
+    national_grid_eso_carbon_intensity_api_base_url: Annotated[
+        URL,
+        typer.Option(
+            envvar="NATIONAL_GRID_ESO_CARBON_INTENSITY_API_BASE_URL",
+            help="URL for the National Grid ESO Carbon Intensity API",
+            parser=http_or_https_url,
+        ),
+    ] = NATIONAL_GRID_ESO_CARBON_INTENSITY_API_BASE_URL,
 ) -> None:
-    intensity_repo: CarbonIntensityRepo = FromFileCarbonIntensityRepo(
-        from_file_carbon_intensity_file_path
+    intensity_repo = make_forecast_low_intensity_date_repo(
+        data_source,
+        from_file_carbon_intensity_file_path,
+        national_grid_eso_carbon_intensity_api_base_url,
     )
-    match data_source:
-        case DataSource.FILE:
-            intensity_repo = intensity_repo
-        case DataSource.NATIONAL_GRID_ESO_CARBON_INTENSITY:
-            intensity_repo = NationalGridESOCarbonIntensityApiRepo(
-                base_url=national_grid_eso_carbon_intensity_api_base_url
-            )
-        case DataSource.CO2_SIGNAL:
-            if not co2_signal_country_code:
-                typer.echo("No country code provided to CO2 Signal Api.")
-                raise typer.Exit(1)
-
-            if not co2_signal_api_key:
-                typer.echo("No API key found for CO2 Signal API.")
-                raise typer.Exit(1)
-
-            intensity_repo = CO2SignalCarbonIntensityRepo(
-                base_url=co2_signal_carbon_intensity_api_base_url,
-                api_key=co2_signal_api_key,
-                country_code=co2_signal_country_code,
-            )
-    carbon_intensity = await intensity_repo.get_carbon_intensity()
-    if carbon_intensity > max_carbon_intensity:
-        typer.echo(
-            FAILURE_TEMPLATE.format(
-                max_carbon_intensity=max_carbon_intensity,
-                carbon_intensity=carbon_intensity,
-            )
-        )
-        raise typer.Exit(1 if not advise_only else 0)
-    typer.echo(
-        SUCCESS_TEMPLATE.format(
-            max_carbon_intensity=max_carbon_intensity, carbon_intensity=carbon_intensity
-        )
+    schedule_run(
+        within,
+        intensity_repo,
     )
 
 
 def run() -> None:
-    typer.run(main)
+    app()
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `carbon_guard-0.6.0/src/repos/carbon_intensity.py` & `carbon_guard-0.7.0/src/repos/carbon_intensity/national_grid_eso.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,64 @@
-from pathlib import Path
-from typing import Generator, Protocol
+import datetime as dt
+from urllib.parse import quote
 
-import httpx
-from httpx import URL, AsyncClient, Request, Response
-from pydantic import BaseModel, field_validator
-
-
-class CarbonIntensityRepo(Protocol):
-    async def get_carbon_intensity(self) -> int:
-        ...
-
-
-class InMemoryCarbonIntensityRepo(object):
-    def __init__(self, carbon_intensity: int) -> None:
-        self._carbon_intensity = carbon_intensity
-
-    async def get_carbon_intensity(self) -> int:
-        return self._carbon_intensity
-
-
-class FromFileCarbonIntensityRepo(object):
-    def __init__(self, file_path: Path) -> None:
-        self._file_path = file_path
-
-    async def get_carbon_intensity(self) -> int:
-        return int(self._file_path.read_text(encoding="utf8"))
+from httpx import URL, AsyncClient
+from pydantic import BaseModel, Field
 
 
 class NationalGridESOCarbonIntensityIntensity(BaseModel):
-    actual: int
+    actual: int | None
+    forecast: int
 
 
 class NationalGridESOCarbonIntensityData(BaseModel):
     intensity: NationalGridESOCarbonIntensityIntensity
+    from_: dt.datetime = Field(..., alias="from")
 
 
 class NationalGridESOCarbonIntensityResponse(BaseModel):
     data: list[NationalGridESOCarbonIntensityData]
 
-    @field_validator("data")
-    def ensure_data_is_not_empty(
-        cls, v: list[NationalGridESOCarbonIntensityData]
-    ) -> list[NationalGridESOCarbonIntensityData]:
-        if not v:
-            raise ValueError("data is empty")
-
-        return v
-
-
-class CO2SignalCarbonIntensityData(BaseModel):
-    carbonIntensity: int
-
-
-class CO2SignalCarbonIntensityResponse(BaseModel):
-    data: CO2SignalCarbonIntensityData
-
 
 class NationalGridESOCarbonIntensityApiRepo:
     def __init__(self, base_url: URL):
         self._client = AsyncClient(base_url=base_url, http2=True)
 
     async def get_carbon_intensity(self) -> int:
         response = await self._client.get("/intensity")
         response.raise_for_status()
 
         parsed_response = NationalGridESOCarbonIntensityResponse.model_validate_json(
             response.content
         )
 
-        return parsed_response.data[0].intensity.actual
+        if not parsed_response.data:
+            raise ValueError("data is empty")
+
+        first_item = parsed_response.data[0]
 
+        return first_item.intensity.actual or first_item.intensity.forecast
 
-class CO2SignalCarbonIntensityRepo:
-    def __init__(self, base_url: URL, api_key: str, country_code: str):
-        self._client = AsyncClient(
-            base_url=base_url, http2=True, auth=CO2SignalAuthClient(api_key=api_key)
+    async def get_best_time_to_run_within_period(
+        self, within: dt.timedelta
+    ) -> dt.datetime:
+        utcnow = dt.datetime.utcnow().replace(tzinfo=dt.timezone.utc)
+        start_time_escaped = quote(
+            utcnow.isoformat(timespec="minutes").replace("+00:00", "Z"), safe=":"
+        )
+        end_time_escaped = quote(
+            (utcnow + within).isoformat(timespec="minutes").replace("+00:00", "Z"),
+            safe=":",
         )
-        self._country_code = country_code
 
-    async def get_carbon_intensity(self) -> int:
         response = await self._client.get(
-            "/v1/latest", params={"countryCode": self._country_code}
+            f"/intensity/{start_time_escaped}/{end_time_escaped}"
         )
         response.raise_for_status()
 
-        parsed_response = CO2SignalCarbonIntensityResponse.model_validate_json(
-            response.content
+        parsed_response: NationalGridESOCarbonIntensityResponse = (
+            NationalGridESOCarbonIntensityResponse.model_validate_json(response.content)
         )
 
-        return parsed_response.data.carbonIntensity
-
-
-class CO2SignalAuthClient(httpx.Auth):
-    def __init__(self, api_key: str):
-        self._api_key = api_key
+        lowest_intensity = min(parsed_response.data, key=lambda x: x.intensity.forecast)
 
-    def auth_flow(self, request: Request) -> Generator[Request, Response, None]:
-        request.headers["auth-token"] = self._api_key
-        yield request
+        return lowest_intensity.from_
```

