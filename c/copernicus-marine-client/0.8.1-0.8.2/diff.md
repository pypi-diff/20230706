# Comparing `tmp/copernicus_marine_client-0.8.1.tar.gz` & `tmp/copernicus_marine_client-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicus_marine_client-0.8.1.tar", max compression
+gzip compressed data, was "copernicus_marine_client-0.8.2.tar", max compression
```

## Comparing `copernicus_marine_client-0.8.1.tar` & `copernicus_marine_client-0.8.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0    10980 2023-07-04 07:18:13.630269 copernicus_marine_client-0.8.1/README.md
--rw-r--r--   0        0        0     3074 2023-07-03 07:22:16.275799 copernicus_marine_client-0.8.1/copernicus_marine_client/__init__.py
--rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544268 copernicus_marine_client-0.8.1/copernicus_marine_client/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    22216 2023-06-30 15:09:13.269129 copernicus_marine_client-0.8.1/copernicus_marine_client/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0     6199 2023-07-03 12:56:17.483906 copernicus_marine_client-0.8.1/copernicus_marine_client/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544602 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/__init__.py
--rw-r--r--   0        0        0      924 2023-07-04 09:12:23.081236 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     3773 2023-07-04 07:33:17.711168 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     4424 2023-07-04 07:31:26.527623 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_login.py
--rw-r--r--   0        0        0     9246 2023-07-04 07:31:41.140486 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_native.py
--rw-r--r--   0        0        0    18511 2023-07-04 07:31:40.674207 copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     4798 2023-07-03 12:00:07.546495 copernicus_marine_client-0.8.1/copernicus_marine_client/configuration_files_creator.py
--rw-r--r--   0        0        0     7410 2023-07-03 12:56:17.484867 copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_ftp.py
--rw-r--r--   0        0        0     4542 2023-07-03 12:00:07.546849 copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_motu.py
--rw-r--r--   0        0        0    10512 2023-07-03 12:00:07.547043 copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_opendap.py
--rw-r--r--   0        0        0     6561 2023-07-03 12:56:17.485055 copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_s3native.py
--rw-r--r--   0        0        0     6606 2023-07-04 07:18:13.631652 copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_zarr.py
--rw-r--r--   0        0        0      917 2023-06-29 09:51:23.593091 copernicus_marine_client-0.8.1/copernicus_marine_client/logging_conf.json
--rw-r--r--   0        0        0      888 2023-07-04 09:12:47.259688 copernicus_marine_client-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    12575 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.1/setup.py
--rw-r--r--   0        0        0    11919 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     9103 2023-07-05 07:04:24.236147 copernicus_marine_client-0.8.2/README.md
+-rw-r--r--   0        0        0     3171 2023-07-06 10:59:48.043538 copernicus_marine_client-0.8.2/copernicus_marine_client/__init__.py
+-rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544268 copernicus_marine_client-0.8.2/copernicus_marine_client/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    22216 2023-07-04 12:57:10.517378 copernicus_marine_client-0.8.2/copernicus_marine_client/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0     6086 2023-07-06 15:00:15.185228 copernicus_marine_client-0.8.2/copernicus_marine_client/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544602 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      994 2023-07-06 10:59:48.043727 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     3773 2023-07-04 07:33:17.711168 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     4811 2023-07-05 07:04:24.237360 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_login.py
+-rw-r--r--   0        0        0     7914 2023-07-05 07:04:24.237641 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_native.py
+-rw-r--r--   0        0        0    16597 2023-07-06 15:00:15.185721 copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     5504 2023-07-05 07:04:24.238384 copernicus_marine_client-0.8.2/copernicus_marine_client/configuration_files_creator.py
+-rw-r--r--   0        0        0     7410 2023-07-06 14:15:57.965380 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_ftp.py
+-rw-r--r--   0        0        0     4542 2023-07-03 12:00:07.546849 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_motu.py
+-rw-r--r--   0        0        0     8265 2023-07-06 14:10:45.282837 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_opendap.py
+-rw-r--r--   0        0        0     6561 2023-07-06 06:34:51.194727 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_s3native.py
+-rw-r--r--   0        0        0     3964 2023-07-06 15:00:15.186118 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_zarr.py
+-rw-r--r--   0        0        0     4387 2023-07-06 14:10:45.283346 copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/subset_xarray.py
+-rw-r--r--   0        0        0      768 2023-07-04 13:23:10.163027 copernicus_marine_client-0.8.2/copernicus_marine_client/logging_conf.json
+-rw-r--r--   0        0        0      888 2023-07-06 15:00:49.565238 copernicus_marine_client-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    10635 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.2/setup.py
+-rw-r--r--   0        0        0    10042 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.2/PKG-INFO
```

### Comparing `copernicus_marine_client-0.8.1/README.md` & `copernicus_marine_client-0.8.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: copernicus-marine-client
+Version: 0.8.2
+Summary: 
+Author: jsouchard
+Author-email: jsouchard@mercator-ocean.fr
+Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.3)
+Requires-Dist: cachier (>=2.0.2)
+Requires-Dist: click (>=8.0.4)
+Requires-Dist: dask (>=2022.1.1)
+Requires-Dist: motuclient (==1.8.4)
+Requires-Dist: netCDF4 (>=1.6.3)
+Requires-Dist: numpy (>=1.0)
+Requires-Dist: owslib (>=0.27.2)
+Requires-Dist: pydap (>=3.2.2)
+Requires-Dist: pystac (>=1.7.2)
+Requires-Dist: requests (>=2.27.1)
+Requires-Dist: s3fs (>=2023.6.0,<2024.0.0)
+Requires-Dist: setuptools (>=62.0.0)
+Requires-Dist: tqdm (>=4.65.0)
+Requires-Dist: xarray (>=2023.3.0)
+Requires-Dist: zarr (>=2.13.3)
+Description-Content-Type: text/markdown
+
 # Copernicus Marine Service client
 
 A library to facilitate the access of Copernicus Marine Service products and datasets.
 
 ## Introduction
 
 This package allows to recover products and datasets information from Command Line Interface or with Python code,
@@ -74,68 +103,14 @@
 '''
 > copernicus marine login
 < Username :
 < Password :
 > INFO     - root - Configuration files stored in ${HOME}\.copernicus_marine_client
 '''
 
-
-Checkout the help:
-'''
-> copernicus-marine login --help
-Usage: copernicus-marine login [OPTIONS]
-
-  This command creates the configurations files used by the various download
-  services and store them in a directory that can be specified by the user. If
-  the user specified a different 'config_file_directory' from default one
-  ($HOME/.copernicus_marine_client), it needs to be passed also to the
-  download commands.
-
-  Examples:
-
-  Case 1 (Recommended):
-
-  With environment variables COPERNICUS_MARINE_CLIENT_USERNAME &
-  COPERNICUS_MARINE_CLIENT_PASSWORD specified:
-
-  > copernicus-marine login
-
-  Case 2:
-
-  > copernicus-marine login
-
-  < Username: [USER-INPUT]
-
-  < Password: [USER-INPUT]
-
-  Case 3:
-
-  > copernicus-marine login --username JOHN_DOE --password SECRETPASSWORD
-
-  Case 4: Specific directory for config_files
-
-  > copernicus-marine login --config-file-directory USER/SPECIFIED/PATH
-
-Options:
-  --username TEXT                 Search for environment variable:
-                                  COPERNICUS_MARINE_CLIENT_USERNAME if not,
-                                  ask for user input
-  --password TEXT                 Search for environment variable:
-                                  COPERNICUS_MARINE_CLIENT_PASSWORD if not,
-                                  ask for user input
-  --config-file-directory TEXT    Path to the directory where the
-                                  configuration files are stored
-  --assume-yes                    Flag to skip confirmation before overwriting
-                                  configuration files
-  --verbose [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]
-                                  Set the details printed to console by the
-                                  command (based on standard logging library).
-  --help                          Show this message and exit.
-'''
-
 ### Command *subset*
 
 Download a dataset subset, based on dataset id, variable names and attributes slices:
 
 ```txt
 > copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
 
@@ -298,9 +273,9 @@
     maximal_depth: Optional[float] = None
     start_datetime: Optional[datetime] = None
     end_datetime: Optional[datetime] = None
     output_directory: Optional[str] = None
     output_filename: Optional[str] = None
     assume_yes: Optional[bool] = None
     force_protocol: Optional[str] = None
-    dry_run: Optional[bool] = None
 ```
+
```

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/__init__.py` & `copernicus_marine_client-0.8.2/copernicus_marine_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """
 .
 """
 
+import importlib.metadata
+
+__version__ = importlib.metadata.version("copernicus-marine-client")
+
 from copernicus_marine_client.catalogue_parser.catalogue_parser import (
     CopernicusMarineCatalogue as CopernicusMarineCatalogue,
 )
 from copernicus_marine_client.catalogue_parser.catalogue_parser import (
     CopernicusMarineDatasetCoordinates as CopernicusMarineDatasetCoordinates,
 )
 from copernicus_marine_client.catalogue_parser.catalogue_parser import (
```

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/catalogue_parser/catalogue_parser.py` & `copernicus_marine_client-0.8.2/copernicus_marine_client/catalogue_parser/catalogue_parser.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/catalogue_parser/request_structure.py` & `copernicus_marine_client-0.8.2/copernicus_marine_client/catalogue_parser/request_structure.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 @dataclass
 class SubsetRequest:
     dataset_url: Optional[str] = None
     dataset_id: Optional[str] = None
     output_directory: str = ""
     assume_yes: bool = False
-    dry_run: bool = False
     variables: Optional[List[str]] = None
     minimal_longitude: Optional[float] = None
     maximal_longitude: Optional[float] = None
     minimal_latitude: Optional[float] = None
     maximal_latitude: Optional[float] = None
     minimal_depth: Optional[float] = None
     maximal_depth: Optional[float] = None
@@ -62,15 +61,15 @@
             ]:
                 new_value = float(value) if value is not None else None
             elif key in [
                 "start_datetime",
                 "end_datetime",
             ]:
                 new_value = datetime_parser(value) if value else None
-            elif key in ["assume_yes", "dry_run"]:
+            elif key in ["assume_yes"]:
                 new_value = (
                     True if value in [True, "true", "True", 1] else False
                 )
             elif key in ["variables"]:
                 new_value = list(value) if value is not None else None
             else:
                 new_value = str(value) if value else None
@@ -107,15 +106,14 @@
             # special case for variable, since it can have multiple values
             motu_api_request_dict.setdefault(arg, []).append(value)
         else:
             motu_api_request_dict[arg] = value
     subset_request = SubsetRequest(
         output_directory=".",
         assume_yes=False,
-        dry_run=False,
         output_filename=None,
         force_protocol=None,
     )
     conversion_dict = {
         "product-id": "dataset_id",
         "latitude-min": "minimal_latitude",
         "latitude-max": "maximal_latitude",
@@ -138,15 +136,14 @@
 class NativeRequest:
     dataset_url: Optional[str] = None
     dataset_id: Optional[str] = None
     no_directories: bool = False
     show_outputnames: bool = False
     output_directory: str = "."
     assume_yes: bool = False
-    dry_run: bool = False
     force_protocol: Optional[str] = None
     regex: Optional[str] = None
 
     def update(self, new_dict: dict):
         """Method to update values in NativeRequest object.
         Skips "None" values
         """
@@ -159,15 +156,14 @@
     def enforce_types(self):
         type_enforced_dict = {}
         for key, value in self.__dict__.items():
             if key in [
                 "no_directories",
                 "show_outputnames",
                 "assume_yes",
-                "dry_run",
             ]:
                 new_value = bool(value) if value is not None else None
             else:
                 new_value = str(value) if value else None
             type_enforced_dict[key] = new_value
         self.__dict__.update(type_enforced_dict)
```

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_describe.py` & `copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_describe.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_login.py` & `copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_login.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 import logging.config
 import os
-from typing import Tuple
+from typing import Literal, Optional, Tuple
 
 import click
 
 from copernicus_marine_client.configuration_files_creator import (
     check_copernicus_marine_credentials,
 )
 from copernicus_marine_client.configuration_files_creator import (
     main as configuration_files_creator,
 )
 from copernicus_marine_client.configuration_files_creator import (
-    retrieve_credentials_from_config_files,
+    retrieve_credential_from_config_files,
 )
 
 
 @click.group()
 def cli_group_login() -> None:
     pass
 
@@ -32,16 +32,16 @@
     ($HOME/.copernicus_marine_client), it needs to be passed also to the download
     commands.
 
     Examples:
 
     Case 1 (Recommended):
 
-    With environment variables COPERNICUS_MARINE_CLIENT_USERNAME &
-    COPERNICUS_MARINE_CLIENT_PASSWORD specified:
+    With environment variables COPERNICUS_MARINE_SERVICE_USERNAME &
+    COPERNICUS_MARINE_SERVICE_PASSWORD specified:
 
     > copernicus-marine login
 
     Case 2:
 
     > copernicus-marine login \n
     < Username: [USER-INPUT] \n
@@ -54,27 +54,29 @@
     Case 4: Specific directory for config_files
 
     > copernicus-marine login --config-file-directory USER/SPECIFIED/PATH
         """,
 )
 @click.option(
     "--username",
-    prompt=True,
-    envvar="COPERNICUS_MARINE_CLIENT_USERNAME",
+    prompt="username",
+    envvar="COPERNICUS_MARINE_SERVICE_USERNAME",
     hide_input=False,
-    help="Search for environment variable: COPERNICUS_MARINE_CLIENT_USERNAME"
-    + " if not, ask for user input",
+    help="If not set, search for environment variable"
+    + " COPERNICUS_MARINE_SERVICE_USERNAME"
+    + ", or else ask for user input",
 )
 @click.option(
     "--password",
-    prompt=True,
-    envvar="COPERNICUS_MARINE_CLIENT_PASSWORD",
+    prompt="password",
+    envvar="COPERNICUS_MARINE_SERVICE_PASSWORD",
     hide_input=True,
-    help="Search for environment variable: COPERNICUS_MARINE_CLIENT_PASSWORD"
-    + " if not, ask for user input",
+    help="If not set, search for environment variable"
+    + " COPERNICUS_MARINE_SERVICE_PASSWORD"
+    + ", or else ask for user input",
 )
 @click.option(
     "--config-file-directory",
     type=str,
     default=os.path.join(os.path.expanduser("~"), ".copernicus_marine_client"),
     help="Path to the directory where the configuration file is stored",
 )
@@ -111,36 +113,57 @@
         password=password,
         config_file_directory=config_file_directory,
         assume_yes=assume_yes,
     )
     logging.info(f"Configuration files stored in {config_file_directory}")
 
 
-def get_username_password(config_file_directory: str) -> Tuple[str, str]:
-    try:
-        username = os.environ.get("COPERNICUS_MARINE_CLIENT_USERNAME")
-        password = os.environ.get("COPERNICUS_MARINE_CLIENT_PASSWORD")
-        if not username or not password:
-            username, password = retrieve_credentials_from_config_files(
-                config_file_directory=config_file_directory,
-                host="my.cmems_du.eu",  # Same credentials for all hosts
-            )
-        else:
-            logging.debug("Credentials from environment variables")
-        if not username or not password:
-            raise TypeError("Null credentials")
-    except TypeError:
-        username = click.prompt("Username")
-        password = click.prompt("Password", hide_input=True)
-        logging.debug("Credentials from input prompt")
-    except FileNotFoundError:
-        username = click.prompt("Username")
-        password = click.prompt("Password", hide_input=True)
-        logging.debug("Credentials from input prompt")
-    if not username or not password:
-        raise TypeError("Null credentials")
+def get_credential(
+    credential: Optional[str],
+    credential_type: Literal["username", "password"],
+    hide_input: bool,
+    config_file_directory: str,
+) -> str:
+    if not credential:
+        credential = retrieve_credential_from_config_files(
+            credential_type=credential_type,
+            config_file_directory=config_file_directory,
+            host="my.cmems_du.eu",  # Same credentials for all hosts
+        )
+        if not credential:
+            credential = click.prompt(credential_type, hide_input=hide_input)
+            if not credential:
+                raise ValueError(f"{credential} cannot be None")
     else:
-        return (username, password)
+        logging.debug(
+            "Credentials loaded from function arguments or environment variable"
+        )
+    return credential
+
+
+def get_username_password(
+    username: Optional[str],
+    password: Optional[str],
+    config_file_directory: str,
+) -> Tuple[str, str]:
+    username = get_credential(
+        username,
+        "username",
+        hide_input=False,
+        config_file_directory=config_file_directory,
+    )
+    password = get_credential(
+        password,
+        "password",
+        hide_input=True,
+        config_file_directory=config_file_directory,
+    )
+    result_check = check_copernicus_marine_credentials(username, password)
+    if result_check:
+        logging.warning(
+            "Invalid credentials, your download will not be authenticated"
+        )
+    return (username, password)
 
 
 if __name__ == "__main__":
     cli_group_login()
```

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_native.py` & `copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_native.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 from copernicus_marine_client.catalogue_parser.request_structure import (
     NativeRequest,
     native_request_from_file,
 )
 from copernicus_marine_client.command_line_interface.group_login import (
     get_username_password,
 )
-from copernicus_marine_client.configuration_files_creator import (
-    check_copernicus_marine_credentials,
-)
 from copernicus_marine_client.download_functions.download_ftp import (
     download_ftp,
 )
 from copernicus_marine_client.download_functions.download_s3native import (
     download_s3native,
 )
 
@@ -73,20 +70,28 @@
     "-i",
     type=str,
     help="The dataset id",
 )
 @click.option(
     "--username",
     type=str,
+    envvar="COPERNICUS_MARINE_SERVICE_USERNAME",
     default=None,
+    help="If not set, search for environment variable"
+    + " COPERNICUS_MARINE_SERVICE_USERNAME"
+    + ", or else look for configuration files, or else ask for user input",
 )
 @click.option(
     "--password",
     type=str,
+    envvar="COPERNICUS_MARINE_SERVICE_PASSWORD",
     default=None,
+    help="If not set, search for environment variable"
+    + " COPERNICUS_MARINE_SERVICE_PASSWORD"
+    + ", or else look for configuration files, or else ask for user input",
 )
 @click.option(
     "--no-directories",
     "-nd",
     is_flag=True,
     help="Option to not recreate folder hierarchy" + " in ouput directory.",
     default=False,
@@ -121,21 +126,14 @@
 )
 @click.option(
     "--force-protocol",
     type=click.Choice(list(PROTOCOL_KEYS_ORDER.keys())),
     help="Force download through one of the available protocols",
 )
 @click.option(
-    "--dry-run",
-    is_flag=True,
-    default=False,
-    help="Flag to specify NOT to send the request to external server. "
-    "Returns the request instead",
-)
-@click.option(
     "--request-file",
     type=click.Path(),
     help="Option to pass a file containg CLI arguments. "
     "The file MUST follow the structure of dataclass 'NativeRequest'. ",
 )
 @click.option(
     "--log-level",
@@ -152,24 +150,23 @@
     default=None,
     help="The regular expression that must match the absolute paths of "
     "the files to download. ",
 )
 def native(
     dataset_url: str,
     dataset_id: str,
-    username: str,
-    password: str,
+    username: Optional[str],
+    password: Optional[str],
     no_directories: bool,
     show_outputnames: bool,
     output_directory: str,
     config_file_directory: str,
     assume_yes: bool,
     request_file: str,
     force_protocol: str,
-    dry_run: bool,
     log_level: str = "INFO",
     regex: Optional[str] = None,
 ):
     if log_level == "QUIET":
         logging.root.disabled = True
         logging.root.setLevel(level="CRITICAL")
     else:
@@ -191,30 +188,28 @@
         native_request.no_directories = no_directories
     if show_outputnames:
         native_request.show_outputnames = show_outputnames
     if assume_yes:
         native_request.assume_yes = assume_yes
     if force_protocol:
         native_request.force_protocol = force_protocol
-    if dry_run:
-        native_request.dry_run = dry_run
     if regex:
         native_request.regex = regex
 
     native_function(
         username,
         password,
         native_request,
         config_file_directory,
     )
 
 
 def native_function(
-    username: str,
-    password: str,
+    username: Optional[str],
+    password: Optional[str],
     native_request: NativeRequest,
     config_file_directory: str = os.path.join(
         os.path.expanduser("~"), ".copernicus_marine_client"
     ),
 ):
     # --- Protocol section
     if native_request.force_protocol:
@@ -244,70 +239,28 @@
         ):
             value_error = ValueError(
                 f"Forced protocol {native_request.force_protocol} does not match "
                 f"user-specified url {native_request.dataset_url}"
             )
             logging.error(value_error)
             raise value_error
-    # --- Credentials section
-    if not username:
-        username, password = get_username_password(config_file_directory)
-    else:
-        logging.debug("Credentials from function arguments")
-    try:
-        check_copernicus_marine_credentials(username, password)
-    except ConnectionRefusedError as credential_error_message:
-        if not native_request.dry_run:
-            logging.error(credential_error_message)
-            raise credential_error_message
-        else:
-            logging.warning(
-                "Invalid credentials, your download will not be authenticated"
-            )
+    username, password = get_username_password(
+        username,
+        password,
+        config_file_directory,
+    )
     # --- Download redirection by protocol
     if protocol == FTP_KEY:
-        if native_request.dry_run:
-            dry_run_message = (
-                "download_ftp("
-                + ", ".join(
-                    [
-                        f"{username}",
-                        "HIDING_PASSWORD",
-                        f"{native_request}",
-                    ]
-                )
-                + ")"
-            )
-            logger = logging.getLogger("blank_logger")
-            logger.warn(dry_run_message)
-            return dry_run_message
-
         download_summary = download_ftp(
             username,
             password,
             native_request,
         )
         logging.info(download_summary)
     elif protocol == S3NATIVE_KEY:
-        if native_request.dry_run:
-            dry_run_message = (
-                "download_s3native("
-                + ", ".join(
-                    [
-                        f"{username}",
-                        "HIDING_PASSWORD",
-                        f"{native_request}",
-                    ]
-                )
-                + ")"
-            )
-            logger = logging.getLogger("blank_logger")
-            logger.warn(dry_run_message)
-            return dry_run_message
-
         download_summary = download_s3native(
             username,
             password,
             native_request,
         )
         logging.info(download_summary)
     else:
```

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/command_line_interface/group_subset.py` & `copernicus_marine_client-0.8.2/copernicus_marine_client/command_line_interface/group_subset.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,14 @@
     SubsetRequest,
     convert_motu_api_request_to_structure,
     subset_request_from_file,
 )
 from copernicus_marine_client.command_line_interface.group_login import (
     get_username_password,
 )
-from copernicus_marine_client.configuration_files_creator import (
-    check_copernicus_marine_credentials,
-)
 from copernicus_marine_client.download_functions.download_motu import (
     download_motu,
 )
 from copernicus_marine_client.download_functions.download_opendap import (
     download_opendap,
 )
 from copernicus_marine_client.download_functions.download_zarr import (
@@ -92,20 +89,28 @@
     "-i",
     type=str,
     help="The dataset id",
 )
 @click.option(
     "--username",
     type=str,
+    envvar="COPERNICUS_MARINE_SERVICE_USERNAME",
     default=None,
+    help="If not set, search for environment variable"
+    + " COPERNICUS_MARINE_SERVICE_USERNAME"
+    + ", or else look for configuration files, or else ask for user input",
 )
 @click.option(
     "--password",
     type=str,
+    envvar="COPERNICUS_MARINE_SERVICE_PASSWORD",
     default=None,
+    help="If not set, search for environment variable"
+    + " COPERNICUS_MARINE_SERVICE_PASSWORD"
+    + ", or else look for configuration files, or else ask for user input",
 )
 @click.option(
     "--variable",
     "-v",
     "variables",
     type=str,
     help="Specify dataset variables",
@@ -199,21 +204,14 @@
 )
 @click.option(
     "--force-protocol",
     type=click.Choice(list(PROTOCOL_KEYS_ORDER.keys())),
     help="Force download through one of the available protocols",
 )
 @click.option(
-    "--dry-run",
-    is_flag=True,
-    default=False,
-    help="Flag to specify NOT to send the request to external server. "
-    "Returns the request instead",
-)
-@click.option(
     "--request-file",
     type=click.Path(),
     help="Option to pass a filename corresponding to a file containg CLI arguments. "
     "The file MUST follow the structure of dataclass 'SubsetRequest'. ",
 )
 @click.option(
     "--motu-api-request",
@@ -250,15 +248,14 @@
     output_filename: Optional[str],
     force_protocol: Optional[str],
     request_file: Optional[str],
     output_directory: str,
     config_file_directory: str,
     motu_api_request: Optional[str],
     assume_yes: bool = False,
-    dry_run: bool = False,
     log_level: str = "INFO",
 ):
     if log_level == "QUIET":
         logging.root.disabled = True
         logging.root.setLevel(level="CRITICAL")
     else:
         logging.root.setLevel(level=log_level)
@@ -287,16 +284,14 @@
         "force_protocol": force_protocol,
     }
     subset_request.update(request_update_dict)
     # Specific treatment for default values:
     # In order to not overload arguments with default values
     if assume_yes:
         subset_request.assume_yes = assume_yes
-    if dry_run:
-        subset_request.dry_run = dry_run
     subset_function(
         username,
         password,
         subset_request,
         config_file_directory,
     )
 
@@ -346,30 +341,19 @@
                 logging.error(key_error)
                 raise key_error
             subset_request.dataset_url = get_dataset_url_from_id(
                 catalogue, subset_request.dataset_id, protocol
             )
     else:
         protocol = get_protocol_from_url(subset_request.dataset_url)
-    # --- Credentials section
-    if not username:
-        username, password = get_username_password(config_file_directory)
-    else:
-        logging.debug("Credentials from function arguments")
-    try:
-        check_copernicus_marine_credentials(username, password)
-    except ConnectionRefusedError as credential_error_message:
-        if not subset_request.dry_run:
-            logging.error(credential_error_message)
-            raise credential_error_message
-        else:
-            logging.warning(
-                "Invalid credentials, your download will not be authenticated"
-            )
-
+    username, password = get_username_password(
+        username,
+        password,
+        config_file_directory,
+    )
     # --- Download redirection by protocol
     if subset_request.force_protocol and (
         protocol != PROTOCOL_KEYS_ORDER[subset_request.force_protocol]
         and protocol not in PROTOCOL_KEYS_ORDER[subset_request.force_protocol]
     ):
         attribute_error = AttributeError(
             f"Dataset url ({subset_request.dataset_url}) does not match forced "
@@ -396,75 +380,29 @@
         ):
             subset_request.dataset_url = (
                 url_timechunked
                 if get_optimized_chunking(subset_request)
                 else url_geochunked
             )
         logging.info("Download Zarr files through S3")
-        if subset_request.dry_run:
-            dry_run_message = (
-                "download_zarr("
-                + ", ".join(
-                    [
-                        f"{username}",
-                        "HIDING_PASSWORD",
-                        f"{subset_request}",
-                    ]
-                )
-                + ")"
-            )
-            logger = logging.getLogger("blank_logger")
-            logger.warn(dry_run_message)
-            return dry_run_message
         output_name = download_zarr(
             username,
             password,
             subset_request,
         )
 
     elif protocol == OPENDAP_KEY:
         logging.info("Download through OPeNDAP")
-        if subset_request.dry_run:
-            dry_run_message = (
-                "download_opendap("
-                + ", ".join(
-                    [
-                        f"{username}",
-                        "HIDING_PASSWORD",
-                        f"{subset_request}",
-                    ]
-                )
-                + ")"
-            )
-            logger = logging.getLogger("blank_logger")
-            logger.warn(dry_run_message)
-            return dry_run_message
         output_name = download_opendap(
             username,
             password,
             subset_request,
         )
     elif protocol == MOTU_KEY:
         logging.info("Download through MOTU")
-        if subset_request.dry_run:
-            dry_run_message = (
-                "download_motu("
-                + ", ".join(
-                    [
-                        f"{username}",
-                        "HIDING_PASSWORD",
-                        f"{subset_request}",
-                        "NOT_PRINTING_CATALOGUE",
-                    ]
-                )
-                + ")"
-            )
-            logger = logging.getLogger("blank_logger")
-            logger.warn(dry_run_message)
-            return dry_run_message
         output_name = download_motu(
             username,
             password,
             subset_request,
             catalogue=catalogue,
         )
     elif not protocol:
```

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_ftp.py` & `copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_ftp.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_motu.py` & `copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_motu.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_opendap.py` & `copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_opendap.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import os
 import re
 from datetime import datetime
 from http.client import IncompleteRead
 from typing import List, Optional, Tuple
 
 import click
-import numpy as np
 import requests
 import xarray as xr
 from dask.diagnostics import ProgressBar
 from pydap.net import HTTPError
 from xarray.backends import PydapDataStore
 
 from copernicus_marine_client.catalogue_parser.request_structure import (
     SubsetRequest,
 )
+from copernicus_marine_client.download_functions.subset_xarray import subset
 
 
 def __parse_limit(message: str) -> Optional[float]:
     match = re.search(r", max=.+\";", message)
     if match:
         limit = match.group().strip(', max=";')
         return float(limit)
@@ -51,88 +51,14 @@
         ds = ds.chunk({"time": i})
         ts = list(split_by_chunks(ds))
         if (ts[0].nbytes / (1000 * 1000)) < limit:
             return i
     return None
 
 
-def subset(
-    ds,
-    variables: Optional[List[str]] = None,
-    geographical_subset: Optional[
-        Tuple[
-            Optional[float], Optional[float], Optional[float], Optional[float]
-        ]
-    ] = None,
-    temporal_subset: Optional[
-        Tuple[Optional[datetime], Optional[datetime]]
-    ] = None,
-    depth_range: Optional[Tuple[Optional[float], Optional[float]]] = None,
-) -> xr.Dataset:
-
-    if variables:
-        ds = ds[np.array(variables)]
-
-    if geographical_subset:
-        (
-            minimal_latitude,
-            maximal_latitude,
-            minimal_longitude,
-            maximal_longitude,
-        ) = geographical_subset
-        if "latitude" in ds.coords:
-            ds = ds.sel(
-                latitude=slice(minimal_latitude, maximal_latitude),
-                longitude=slice(minimal_longitude, maximal_longitude),
-            )
-        elif "nav_lat" in ds.coords:
-            mask = (
-                (ds.nav_lon > minimal_longitude)
-                & (ds.nav_lon < maximal_longitude)
-                & (ds.nav_lat > minimal_latitude)
-                & (ds.nav_lat < maximal_latitude)
-            )
-            geoindex = np.argwhere(mask.values)
-            xmin = min(geoindex[:, 1])
-            xmax = max(geoindex[:, 1])
-            ymin = min(geoindex[:, 0])
-            ymax = max(geoindex[:, 0])
-
-            ds = ds.isel(
-                x=slice(xmin, xmax),
-                y=slice(ymin, ymax),
-            )
-        else:
-            ds = ds.sel(
-                lat=slice(minimal_latitude, maximal_latitude),
-                lon=slice(minimal_longitude, maximal_longitude),
-            )
-
-    if temporal_subset:
-        (start_datetime, end_datetime) = temporal_subset
-        if "time_counter" in ds.coords:
-            ds = ds.sel(time_counter=slice(start_datetime, end_datetime))
-        else:
-            ds = ds.sel(time=slice(start_datetime, end_datetime))
-
-    if (("depth" in ds.dims) or ("deptht" in ds.dims)) and (
-        depth_range is not None
-    ):
-        (
-            minimal_depth,
-            maximal_depth,
-        ) = depth_range
-        if "deptht" in ds.dims:
-            ds = ds.sel(deptht=slice(minimal_depth, maximal_depth))
-        else:
-            ds = ds.sel(depth=slice(minimal_depth, maximal_depth))
-
-    return ds
-
-
 def chunked_download(
     store: PydapDataStore,
     dataset: xr.Dataset,
     limit: Optional[int],
     error: HTTPError,
     output_directory: str,
     output_filename: str,
```

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/download_functions/download_s3native.py` & `copernicus_marine_client-0.8.2/copernicus_marine_client/download_functions/download_s3native.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.1/copernicus_marine_client/logging_conf.json` & `copernicus_marine_client-0.8.2/copernicus_marine_client/logging_conf.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'handlers'": "{delete: ['file']}"}*

```diff
@@ -16,20 +16,14 @@
             "stream": "ext://sys.stdout"
         },
         "console_blank": {
             "class": "logging.StreamHandler",
             "formatter": "blank",
             "level": "DEBUG",
             "stream": "ext://sys.stdout"
-        },
-        "file": {
-            "class": "logging.FileHandler",
-            "filename": "copernicus_marine.log",
-            "formatter": "simple",
-            "mode": "w"
         }
     },
     "loggers": {
         "blank_logger": {
             "handlers": [
                 "console_blank"
             ],
```

### Comparing `copernicus_marine_client-0.8.1/pyproject.toml` & `copernicus_marine_client-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicus-marine-client"
-version = "0.8.1"
+version = "0.8.2"
 description = ""
 authors = ["jsouchard <jsouchard@mercator-ocean.fr>"]
 readme = "README.md"
 packages = [{include = "copernicus_marine_client"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `copernicus_marine_client-0.8.1/setup.py` & `copernicus_marine_client-0.8.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
 entry_points = \
 {'console_scripts': ['copernicus-marine = '
                      'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicus-marine-client',
-    'version': '0.8.1',
+    'version': '0.8.2',
     'description': '',
-    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\n\nRetrieve information about all products as JSON:\n\n```txt\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```txt\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n```\n\n### Command *login*\n\nCreate the configuration files for access to the copernicus marine service:\n\'.dodsrc\', \'.netrc\', \'.motuclient-python.ini\'.\nThe directory to store these configuration files can be modified by the user using the "config-file-directory" option\nbut beware as it should also be passed to the *subset* and *native* command afterwards.\nBy default, if the configuration files already exist, the user is asked for confirmation to overwrite them.\n\nExample:\n\'\'\'\n> copernicus marine login\n< Username :\n< Password :\n> INFO     - root - Configuration files stored in ${HOME}\\.copernicus_marine_client\n\'\'\'\n\n\nCheckout the help:\n\'\'\'\n> copernicus-marine login --help\nUsage: copernicus-marine login [OPTIONS]\n\n  This command creates the configurations files used by the various download\n  services and store them in a directory that can be specified by the user. If\n  the user specified a different \'config_file_directory\' from default one\n  ($HOME/.copernicus_marine_client), it needs to be passed also to the\n  download commands.\n\n  Examples:\n\n  Case 1 (Recommended):\n\n  With environment variables COPERNICUS_MARINE_CLIENT_USERNAME &\n  COPERNICUS_MARINE_CLIENT_PASSWORD specified:\n\n  > copernicus-marine login\n\n  Case 2:\n\n  > copernicus-marine login\n\n  < Username: [USER-INPUT]\n\n  < Password: [USER-INPUT]\n\n  Case 3:\n\n  > copernicus-marine login --username JOHN_DOE --password SECRETPASSWORD\n\n  Case 4: Specific directory for config_files\n\n  > copernicus-marine login --config-file-directory USER/SPECIFIED/PATH\n\nOptions:\n  --username TEXT                 Search for environment variable:\n                                  COPERNICUS_MARINE_CLIENT_USERNAME if not,\n                                  ask for user input\n  --password TEXT                 Search for environment variable:\n                                  COPERNICUS_MARINE_CLIENT_PASSWORD if not,\n                                  ask for user input\n  --config-file-directory TEXT    Path to the directory where the\n                                  configuration files are stored\n  --assume-yes                    Flag to skip confirmation before overwriting\n                                  configuration files\n  --verbose [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]\n                                  Set the details printed to console by the\n                                  command (based on standard logging library).\n  --help                          Show this message and exit.\n\'\'\'\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```txt\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Username:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options). If the output-filename argument ends with \'.nc\' suffix, the file will be downloaded as a netCDF file.\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n\n```txt\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Username:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nOption `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.\n**Be aware that the regular expression must match the full absolute path of the files to filter.**\n\nExample:\n```\n> copernicus-marine native --login qgaudel -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"\nPassword:\nYou requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\n\nTotal size of the download: 9.82 MB\n\n\nDo you want to continue? [y/N]:\n```\n\n### The `--help` argument\n\nIn any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```python\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = "cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m"\nassert dataset_id in cmc.get_all_dataset_ids()\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [\n    variable for variable in dataset.variables if variable.short_name in ["zooc"]\n][0]\ncoordinates = {\n    coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value)\n    for coordinate in variable.coordinates\n}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n    dataset_id="cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m",\n    start_datetime="2023-04-20",\n    end_datetime="2023-04-21",\n    minimal_latitude=30.0,\n    maximal_latitude=30.1,\n    minimal_longitude=0.1,\n    maximal_longitude=0.2,\n    minimal_depth=100,\n    maximal_depth=1000,\n    variables=["zooc"],\n    force_protocol="zarr-map",\n    output_directory="data_folder",\n    output_filename="datastore.zarr",\n    assume_yes=True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(\n    login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request\n)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine="zarr", out_type="xarray")\n```\n\n## Installation\n\nUsing pip, for example:\n\n```shell\npip install copernicus-marine-client\n```\n\n## Technical details\n\nThis module is organized around two capabilities:\n\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```python\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n    dry_run: Optional[bool] = None\n```\n',
+    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\n\nRetrieve information about all products as JSON:\n\n```txt\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```txt\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n```\n\n### Command *login*\n\nCreate the configuration files for access to the copernicus marine service:\n\'.dodsrc\', \'.netrc\', \'.motuclient-python.ini\'.\nThe directory to store these configuration files can be modified by the user using the "config-file-directory" option\nbut beware as it should also be passed to the *subset* and *native* command afterwards.\nBy default, if the configuration files already exist, the user is asked for confirmation to overwrite them.\n\nExample:\n\'\'\'\n> copernicus marine login\n< Username :\n< Password :\n> INFO     - root - Configuration files stored in ${HOME}\\.copernicus_marine_client\n\'\'\'\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```txt\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Username:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options). If the output-filename argument ends with \'.nc\' suffix, the file will be downloaded as a netCDF file.\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n\n```txt\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Username:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nOption `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.\n**Be aware that the regular expression must match the full absolute path of the files to filter.**\n\nExample:\n```\n> copernicus-marine native --login qgaudel -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"\nPassword:\nYou requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\n\nTotal size of the download: 9.82 MB\n\n\nDo you want to continue? [y/N]:\n```\n\n### The `--help` argument\n\nIn any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```python\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = "cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m"\nassert dataset_id in cmc.get_all_dataset_ids()\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [\n    variable for variable in dataset.variables if variable.short_name in ["zooc"]\n][0]\ncoordinates = {\n    coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value)\n    for coordinate in variable.coordinates\n}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n    dataset_id="cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m",\n    start_datetime="2023-04-20",\n    end_datetime="2023-04-21",\n    minimal_latitude=30.0,\n    maximal_latitude=30.1,\n    minimal_longitude=0.1,\n    maximal_longitude=0.2,\n    minimal_depth=100,\n    maximal_depth=1000,\n    variables=["zooc"],\n    force_protocol="zarr-map",\n    output_directory="data_folder",\n    output_filename="datastore.zarr",\n    assume_yes=True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(\n    login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request\n)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine="zarr", out_type="xarray")\n```\n\n## Installation\n\nUsing pip, for example:\n\n```shell\npip install copernicus-marine-client\n```\n\n## Technical details\n\nThis module is organized around two capabilities:\n\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```python\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n```\n',
     'author': 'jsouchard',
     'author_email': 'jsouchard@mercator-ocean.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `copernicus_marine_client-0.8.1/PKG-INFO` & `copernicus_marine_client-0.8.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: copernicus-marine-client
-Version: 0.8.1
-Summary: 
-Author: jsouchard
-Author-email: jsouchard@mercator-ocean.fr
-Requires-Python: >=3.9
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.3)
-Requires-Dist: cachier (>=2.0.2)
-Requires-Dist: click (>=8.0.4)
-Requires-Dist: dask (>=2022.1.1)
-Requires-Dist: motuclient (==1.8.4)
-Requires-Dist: netCDF4 (>=1.6.3)
-Requires-Dist: numpy (>=1.0)
-Requires-Dist: owslib (>=0.27.2)
-Requires-Dist: pydap (>=3.2.2)
-Requires-Dist: pystac (>=1.7.2)
-Requires-Dist: requests (>=2.27.1)
-Requires-Dist: s3fs (>=2023.6.0,<2024.0.0)
-Requires-Dist: setuptools (>=62.0.0)
-Requires-Dist: tqdm (>=4.65.0)
-Requires-Dist: xarray (>=2023.3.0)
-Requires-Dist: zarr (>=2.13.3)
-Description-Content-Type: text/markdown
-
 # Copernicus Marine Service client
 
 A library to facilitate the access of Copernicus Marine Service products and datasets.
 
 ## Introduction
 
 This package allows to recover products and datasets information from Command Line Interface or with Python code,
@@ -103,68 +74,14 @@
 '''
 > copernicus marine login
 < Username :
 < Password :
 > INFO     - root - Configuration files stored in ${HOME}\.copernicus_marine_client
 '''
 
-
-Checkout the help:
-'''
-> copernicus-marine login --help
-Usage: copernicus-marine login [OPTIONS]
-
-  This command creates the configurations files used by the various download
-  services and store them in a directory that can be specified by the user. If
-  the user specified a different 'config_file_directory' from default one
-  ($HOME/.copernicus_marine_client), it needs to be passed also to the
-  download commands.
-
-  Examples:
-
-  Case 1 (Recommended):
-
-  With environment variables COPERNICUS_MARINE_CLIENT_USERNAME &
-  COPERNICUS_MARINE_CLIENT_PASSWORD specified:
-
-  > copernicus-marine login
-
-  Case 2:
-
-  > copernicus-marine login
-
-  < Username: [USER-INPUT]
-
-  < Password: [USER-INPUT]
-
-  Case 3:
-
-  > copernicus-marine login --username JOHN_DOE --password SECRETPASSWORD
-
-  Case 4: Specific directory for config_files
-
-  > copernicus-marine login --config-file-directory USER/SPECIFIED/PATH
-
-Options:
-  --username TEXT                 Search for environment variable:
-                                  COPERNICUS_MARINE_CLIENT_USERNAME if not,
-                                  ask for user input
-  --password TEXT                 Search for environment variable:
-                                  COPERNICUS_MARINE_CLIENT_PASSWORD if not,
-                                  ask for user input
-  --config-file-directory TEXT    Path to the directory where the
-                                  configuration files are stored
-  --assume-yes                    Flag to skip confirmation before overwriting
-                                  configuration files
-  --verbose [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]
-                                  Set the details printed to console by the
-                                  command (based on standard logging library).
-  --help                          Show this message and exit.
-'''
-
 ### Command *subset*
 
 Download a dataset subset, based on dataset id, variable names and attributes slices:
 
 ```txt
 > copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
 
@@ -327,10 +244,8 @@
     maximal_depth: Optional[float] = None
     start_datetime: Optional[datetime] = None
     end_datetime: Optional[datetime] = None
     output_directory: Optional[str] = None
     output_filename: Optional[str] = None
     assume_yes: Optional[bool] = None
     force_protocol: Optional[str] = None
-    dry_run: Optional[bool] = None
 ```
-
```

