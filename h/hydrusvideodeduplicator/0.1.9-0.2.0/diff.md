# Comparing `tmp/hydrusvideodeduplicator-0.1.9.tar.gz` & `tmp/hydrusvideodeduplicator-0.2.0.tar.gz`

## Comparing `hydrusvideodeduplicator-0.1.9.tar` & `hydrusvideodeduplicator-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,39 @@
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/README.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    13902 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/pdq_utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq.py
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq_faiss.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/vpdq_util.py
--rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/README.md
--rw-r--r--   0        0        0    36568 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/utils.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/tests/__init__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/LICENSE
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/README.md
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/Dockerfile
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/docker-compose.yml
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/docker-entrypoint.sh
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    15720 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36873 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/hasher/__init__.py
+-rw-r--r--   0        0        0    24236 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/hasher/pdq_hasher.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tests/__init__.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tests/hash256_test.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tests/matrix_test.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tests/pdq_test.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tools/__init__.py
+-rw-r--r--   0        0        0    12530 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/tools/pdq_photo_hasher_tool.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/types/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/types/containers.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/types/exceptions.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/types/hash256.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/utils/__init__.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/pdqhashing/utils/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/vpdqpy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/vpdqpy/__main__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/vpdqpy/typing_utils.py
+-rw-r--r--   0        0        0     6420 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/src/vpdqpy/vpdqpy.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/README.md
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.0/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,72 @@
 import logging
-from typing import Optional, Annotated, List
+from typing import Annotated, List, Optional
 
 import typer
-import hydrusvideodeduplicator.hydrus_api as hydrus_api
 from rich import print as rprint
 
+import hydrusvideodeduplicator.hydrus_api as hydrus_api
+
 from .__about__ import __version__
-from .config import HYDRUS_API_KEY, HYDRUS_API_URL
+from .config import HYDRUS_API_KEY, HYDRUS_API_URL, HYDRUS_QUERY, REQUESTS_CA_BUNDLE
 from .dedup import HydrusVideoDeduplicator
 
-from .vpdq_util import VPDQ_QUERY_MATCH_THRESHOLD_PERCENT
-
 """
 Parameters:
 - api_key will be read from env var $HYDRUS_API_KEY or .env file
 - api_url will be read from env var $HYDRUS_API_URL or .env file
 - to add custom queries, do
   --custom-query="series:twilight" --custom-query="character:edward" ... etc for each query
 - threshold is the min % matching to be considered similar. 100% is identical.
 - verbose turns on logging
 - debug turns on logging and sets the logging level to debug
 """
 rprint(f"[blue] Hydrus Video Deduplicator {__version__} [/]")
 
-def main(api_key: Annotated[Optional[str], typer.Option(help="Hydrus API Key")] = None,
-        api_url: Annotated[Optional[str], typer.Option(help="Hydrus API URL")] = HYDRUS_API_URL,
-        overwrite:  Annotated[Optional[bool], typer.Option(help="Overwrite existing perceptual hashes")] = False,
-        query: Annotated[Optional[List[str]], typer.Option(help="Custom Hydrus tag query")] = None,
-        threshold: Annotated[Optional[float], typer.Option(help="Similarity threshold for a pair of videos where 100 is identical")] = VPDQ_QUERY_MATCH_THRESHOLD_PERCENT,
-        skip_hashing: Annotated[Optional[bool], typer.Option(help="Skip perceptual hashing and just search for duplicates")] = False,
-        verbose:  Annotated[Optional[bool], typer.Option(hidden=True)] = False,
-        debug: Annotated[Optional[bool], typer.Option(hidden=True)] = False,
-        ):
 
-    threshold = threshold/100.
+def main(
+    api_key: Annotated[Optional[str], typer.Option(help="Hydrus API Key")] = None,
+    api_url: Annotated[Optional[str], typer.Option(help="Hydrus API URL")] = HYDRUS_API_URL,
+    overwrite: Annotated[Optional[bool], typer.Option(help="Overwrite existing perceptual hashes")] = False,
+    query: Annotated[Optional[List[str]], typer.Option(help="Custom Hydrus tag query")] = HYDRUS_QUERY,
+    threshold: Annotated[
+        Optional[float], typer.Option(help="Similarity threshold for a pair of videos where 100 is identical")
+    ] = 75.0,
+    skip_hashing: Annotated[
+        Optional[bool], typer.Option(help="Skip perceptual hashing and just search for duplicates")
+    ] = False,
+    verify_cert: Annotated[
+        Optional[str], typer.Option(help="Path to TLS cert. This forces verification.")
+    ] = REQUESTS_CA_BUNDLE,
+    clear_search_cache: Annotated[
+        Optional[bool], typer.Option(help="Clear the cache that tracks what files have already been compared")
+    ] = False,
+    verbose: Annotated[Optional[bool], typer.Option(help="Verbose logging")] = False,
+    debug: Annotated[Optional[bool], typer.Option(hidden=True)] = False,
+):
 
     # CLI debug parameter sets log level to info or debug
-    loglevel: logging._Level = logging.WARNING
+    loglevel = logging.WARNING
     if debug:
         loglevel = logging.DEBUG
         verbose = True
 
-    logging.basicConfig(format=' %(asctime)s - %(name)s: %(message)s',
-                        datefmt='%H:%M:%S',
-                        level=loglevel)
+    logging.basicConfig(format=' %(asctime)s - %(name)s: %(message)s', datefmt='%H:%M:%S', level=loglevel)
     logging.info("Starting Hydrus Video Deduplicator")
-    
+
     # Verbose sets whether logs are shown to the user at all.
     # Logs are separate from printing in this program.
     if not verbose:
         logging.disable()
 
+    # Clear cache
+    if clear_search_cache:
+        HydrusVideoDeduplicator.clear_search_cache()
+        rprint("[green] Cleared search cache.")
+
     # CLI overwrites env vars
     if not api_key:
         api_key = HYDRUS_API_KEY
     if not api_url:
         api_url = HYDRUS_API_URL
 
     # Check for necessary variables
@@ -65,16 +77,19 @@
     if not api_url:
         print("Hydrus URL not set. Exiting...")
         raise typer.Exit(code=1)
 
     print(f"Connecting to {api_url}")
     # Client connection
     # TODO: Try to connect with https first and then fallback to http with a strong warning
-    _client = hydrus_api.Client(api_url=api_url,
-                                access_key=api_key)
+    _client = hydrus_api.Client(
+        api_url=api_url,
+        access_key=api_key,
+        verify_cert=verify_cert,
+    )
 
     error_connecting = True
     error_connecting_exception_msg = ""
     error_connecting_exception = ""
     try:
         superdeduper = HydrusVideoDeduplicator(_client)
     except hydrus_api.InsufficientAccess as exc:
@@ -86,41 +101,50 @@
     except hydrus_api.ServerError as exc:
         error_connecting_exception_msg = "Unknown Server Error."
         error_connecting_exception = exc
     except hydrus_api.APIError as exc:
         error_connecting_exception_msg = "API Error"
         error_connecting_exception = exc
     except hydrus_api.ConnectionError as exc:
-        error_connecting_exception_msg = "Failed to connect to Hydrus. Is your Hydrus instance running?"
+        # Probably SSL error
+        if "SSL" in str(exc):
+            error_connecting_exception_msg = "Failed to connect to Hydrus. SSL certificate verification failed."
+        # Probably tried using http instead of https when client is https
+        elif "Connection aborted" in str(exc):
+            error_connecting_exception_msg = (
+                "Failed to connect to Hydrus. Does your Hydrus Client API http/https setting match your --api-url?"
+            )
+        else:
+            error_connecting_exception_msg = "Failed to connect to Hydrus. Is your Hydrus instance running?"
         error_connecting_exception = exc
     else:
         error_connecting = False
-    
+
     if error_connecting:
         logging.fatal("FATAL ERROR HAS OCCURRED")
         logging.fatal(error_connecting_exception)
         rprint(f"[red] {error_connecting_exception_msg} ")
         raise typer.Exit(code=1)
 
     # Deduplication parameters
 
     if debug:
         superdeduper.hydlog.setLevel(logging.DEBUG)
         superdeduper._DEBUG = True
 
     if threshold < 0:
-        rprint(f"[red] ERROR: Invalid similarity threshold. Must be between 0 and 100.")
+        rprint("[red] ERROR: Invalid similarity threshold. Must be between 0 and 100.")
         raise typer.Exit(code=1)
     superdeduper.threshold = threshold
 
+    superdeduper.clear_trashed_files_from_db()
+
     # Run all deduplicate functionality
-    superdeduper.deduplicate(overwrite=overwrite,
-                             custom_query=query,
-                             skip_hashing=skip_hashing)
+    superdeduper.deduplicate(overwrite=overwrite, custom_query=query, skip_hashing=skip_hashing)
 
-    typer.Exit()
+    raise typer.Exit()
 
 
 try:
     typer.run(main)
-except KeyboardInterrupt:
-    typer.Exit()
+except KeyboardInterrupt as exc:
+    raise typer.Exit(-1) from exc
```

### Comparing `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 import os
 from pathlib import Path
 from platform import uname
+import json
 
 from dotenv import load_dotenv
 from appdirs import AppDirs
 
 load_dotenv()
-HYDRUS_API_KEY=os.getenv("HYDRUS_API_KEY")
+HYDRUS_API_KEY = os.getenv("HYDRUS_API_KEY")
+
 
 def in_wsl() -> bool:
     return 'microsoft-standard' in uname().release
 
+
 _DEFAULT_IP = "localhost"
 _DEFAULT_PORT = "45869"
 # If you're in WSL you probably want to connect to your Windows Hydrus Client by default
 if in_wsl():
     from socket import gethostname
+
     _DEFAULT_IP = f"{gethostname()}.local"
 
-HYDRUS_API_URL=os.getenv("HYDRUS_API_URL", f"http://{_DEFAULT_IP}:{_DEFAULT_PORT}")
+HYDRUS_API_URL = os.getenv("HYDRUS_API_URL", f"https://{_DEFAULT_IP}:{_DEFAULT_PORT}")
 
 # Service name of where to store perceptual hash tag for video files
-HYDRUS_LOCAL_TAG_SERVICE_NAME=os.getenv("HYDRUS_LOCAL_TAG_SERVICE_NAME", "my tags")
+HYDRUS_LOCAL_TAG_SERVICE_NAME = os.getenv("HYDRUS_LOCAL_TAG_SERVICE_NAME", "my tags")
 
 # ~/.local/share/hydrusvideodeduplicator/ on Linux
-DEDUP_DATABASE_DIR=AppDirs("hydrusvideodeduplicator").user_data_dir
-DEDUP_DATABASE_DIR=os.getenv("DEDUP_DATABASE_DIR", DEDUP_DATABASE_DIR)
-DEDUP_DATABASE_DIR=Path(DEDUP_DATABASE_DIR)
-
-DEDUP_DATABASE_NAME=os.getenv("DEDUP_DATABASE_NAME", "videohashes")
-DEDUP_DATABASE_FILE=Path(DEDUP_DATABASE_DIR, f"{DEDUP_DATABASE_NAME}.sqlite")
+DEDUP_DATABASE_DIR = AppDirs("hydrusvideodeduplicator").user_data_dir
+DEDUP_DATABASE_DIR = os.getenv("DEDUP_DATABASE_DIR", DEDUP_DATABASE_DIR)
+DEDUP_DATABASE_DIR = Path(DEDUP_DATABASE_DIR)
+
+DEDUP_DATABASE_NAME = os.getenv("DEDUP_DATABASE_NAME", "videohashes")
+DEDUP_DATABASE_FILE = Path(DEDUP_DATABASE_DIR, f"{DEDUP_DATABASE_NAME}.sqlite")
+
+REQUESTS_CA_BUNDLE = os.getenv("REQUESTS_CA_BUNDLE")
+
+HYDRUS_QUERY = os.getenv("HYDRUS_QUERY")
+if HYDRUS_QUERY is not None:
+    try:
+        HYDRUS_QUERY = json.loads(HYDRUS_QUERY)
+    except json.decoder.JSONDecodeError as exc:
+        print("ERROR:", exc)
+        print("Invalid query passed as environment variable.")
+        exit(-1)
```

### Comparing `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/dedup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,277 +1,342 @@
-import os
-from io import IOBase
+from __future__ import annotations
+
 import logging
-import tempfile
+import os
 from itertools import islice
-import json
 from pathlib import Path
-import subprocess
+from typing import TYPE_CHECKING
 
-import hydrusvideodeduplicator.hydrus_api as hydrus_api
-import hydrusvideodeduplicator.hydrus_api.utils
-from tqdm import tqdm
+from joblib import Parallel, delayed
 from rich import print as rprint
 from sqlitedict import SqliteDict
+from tqdm import tqdm
 
-from .config import DEDUP_DATABASE_FILE, DEDUP_DATABASE_DIR, DEDUP_DATABASE_NAME
-from .dedup_util import find_tag_in_tags, get_file_names_hydrus, cleanup_defunct_processes
-from .vpdq import VPDQSignal
-
-from .vpdq_util import (
-    VPDQ_QUERY_MATCH_THRESHOLD_PERCENT,
-)
+if TYPE_CHECKING:
+    pass
 
-class HydrusVideoDeduplicator():
+import hydrusvideodeduplicator.hydrus_api as hydrus_api
+import hydrusvideodeduplicator.hydrus_api.utils
+from vpdqpy.vpdqpy import Vpdq
+
+from .config import DEDUP_DATABASE_DIR, DEDUP_DATABASE_FILE, DEDUP_DATABASE_NAME
+from .dedup_util import database_accessible, find_tag_in_tags, get_file_names_hydrus
+
+
+class HydrusVideoDeduplicator:
     hydlog = logging.getLogger("hydlog")
-    threshold: float = 0.8
+    threshold: float = 75.0
     _DEBUG = False
 
-    REQUIRED_PERMISSIONS = (
-        hydrus_api.Permission.IMPORT_URLS,
-        hydrus_api.Permission.IMPORT_FILES,
-        hydrus_api.Permission.ADD_TAGS,
-        hydrus_api.Permission.SEARCH_FILES,
-        hydrus_api.Permission.MANAGE_PAGES,
-        hydrus_api.Permission.MANAGE_DATABASE,
-        hydrus_api.Permission.ADD_NOTES,
-        hydrus_api.Permission.MANAGE_FILE_RELATIONSHIPS,
-    )
-
-    def __init__(self, client: hydrus_api.Client,
-                 verify_connection: bool = True):
+    def __init__(self, client: hydrus_api.Client, verify_connection: bool = True):
         self.client = client
         if verify_connection:
             self.verify_api_connection()
         self.hydlog.setLevel(logging.WARNING)
-        
+
         # Commonly used things from the Hydrus database
         # If any of these are large they should probably be lazily loaded
         self.all_services = self.client.get_services()
 
     # Verify client connection and permissions
     # Will throw a hydrus_api.APIError if something is wrong
     def verify_api_connection(self):
-        self.hydlog.info(f"Client API version: v{self.client.VERSION} | Endpoint API version: v{self.client.get_api_version()['version']}")
+        self.hydlog.info(
+            f"Client API version: v{self.client.VERSION} | Endpoint API version: v{self.client.get_api_version()['version']}"
+        )
         hydrus_api.utils.verify_permissions(self.client, hydrus_api.utils.Permission)
-    
+
     # This is the master function of the class
     def deduplicate(self, overwrite: bool = False, custom_query: list | None = None, skip_hashing: bool | None = False):
-        # Add perceptual hashes to videos
-        search_tags = ["system:filetype=video"]
+        # Add perceptual hashes to video files
+        # system:filetype tags are really inconsistent
+        search_tags = ['system:filetype=video, gif, apng', 'system:has duration']
+
+        query = False
         if custom_query is not None:
-            custom_query = [x for x in custom_query if x.strip()] # Remove whitespace and empty strings
+            custom_query = [x for x in custom_query if x.strip()]  # Remove whitespace and empty strings
             if len(custom_query) > 0:
                 search_tags.extend(custom_query)
                 rprint(f"[yellow] Custom Query: {custom_query}")
+                query = True
 
-        if not skip_hashing:
-            self._add_perceptual_hashes_to_db(overwrite=overwrite, custom_query=custom_query)
-        else:
+        video_hashes = None
+        if skip_hashing:
             rprint("[yellow] Skipping perceptual hashing")
+            if query:
+                video_hashes = set(self._retrieve_video_hashes(search_tags))
+        else:
+            video_hashes = self._retrieve_video_hashes(search_tags)
+            self._add_perceptual_hashes_to_db(overwrite=overwrite, video_hashes=video_hashes)
+
+        self._find_potential_duplicates(limited_video_hashes=video_hashes)
 
-        self._find_potential_duplicates()
         self.hydlog.info("Deduplication done.")
 
-    @classmethod
-    # dir is where you're writing the video file
-    def _add_perceptual_hash_to_db(cls, video_hash: str, video: str | bytes, video_dir: Path | str, db) -> None:
-        with tempfile.NamedTemporaryFile(mode="w+b", dir=video_dir) as tmp_vid_file:
-            # Write video to file to be able to calculate hash
-            tmp_vid_file.write(video)
-            tmp_vid_file.seek(0)
-
-            ffprobe_cmd = [
-                        'ffprobe',
-                        '-v',
-                        'error',
-                        '-select_streams',
-                        'v:0',
-                        '-show_entries',
-                        'stream=codec_name',
-                        '-of',
-                        'default=noprint_wrappers=1:nokey=1',
-                        tmp_vid_file.name
-                        ]
-
-            # Execute the ffprobe command and capture the output
-            video_codec = subprocess.check_output(ffprobe_cmd).decode('utf-8').strip()
-
-            # These are found by trial and error. If you find an unsupported codec, create an issue on GitHub please.
-            # Unsupported codecs appear to be an OpenCV issue more than an FFmpeg issue but I can't solve it at the moment.
-            # For now, just transcode the video to avc1
-            unsupported_codecs = ["av1"]
-
-            if video_codec in unsupported_codecs:
-                rprint(f"[yellow] Video file has unsupported codec: {video_codec}")
-                rprint("[yellow] Falling back to transcoding (this may take a bit)")
-
-                try:
-
-                    with tempfile.NamedTemporaryFile(mode="w+b", dir=video_dir, suffix=".mp4") as tmp_vid_file_transcoded:
-                        ffmpeg_cmd = [
-                            'ffmpeg',
-                            '-y',
-                            '-i',
-                            tmp_vid_file.name,
-                            '-c:v',
-                            'libx264',
-                            '-preset',
-                            'veryfast',
-                            '-crf',
-                            '28',
-                            tmp_vid_file_transcoded.name,
-                        ]
-
-                        # Execute the ffmpeg command
-                        with open(os.devnull, "w") as devnull: subprocess.call(ffmpeg_cmd, stdout=devnull, stderr=devnull)
-
-                        perceptual_hash = VPDQSignal.hash_from_file(tmp_vid_file_transcoded.name)
-
-                        rprint("[yellow] Fallback to transcode successful.")
-                except:
-                    rprint("[red] Transcode and/or hashing the transcode failed.")
-            else:
-                perceptual_hash = VPDQSignal.hash_from_file(tmp_vid_file.name)
+    @staticmethod
+    def _calculate_perceptual_hash(video: str | bytes) -> str:
+        perceptual_hash = Vpdq.vpdq_to_json(Vpdq.computeHash(video))
+        assert perceptual_hash != "[]"
+        return perceptual_hash
+
+    def _retrieve_video_hashes(self, search_tags) -> list:
+        all_video_hashes = self.client.search_files(
+            search_tags,
+            file_sort_type=hydrus_api.FileSortType.FILE_SIZE,
+            return_hashes=True,
+            file_sort_asc=True,
+            return_file_ids=False,
+        )["hashes"]
+        return all_video_hashes
 
-            
-            row = db.get(video_hash, {})
-            row["perceptual_hash"] = perceptual_hash
-            db[video_hash] = row
-            cls.hydlog.debug(f"Perceptual hash calculated and added to DB.")
-    
-    # Add perceptual hash for videos to the database
-    def _add_perceptual_hashes_to_db(self, overwrite: bool, custom_query: list | None = None) -> None:
-
-        # Create database folder if it doesn't already exist
-        if os.path.exists(DEDUP_DATABASE_FILE):
-            with SqliteDict(str(DEDUP_DATABASE_FILE), tablename = "videos") as hashdb:
-                rprint(f"[green] Database found with {len(hashdb)} videos already hashed.")
-                self.hydlog.info(f"Found existing DB of length {len(hashdb)}, size {os.path.getsize(DEDUP_DATABASE_FILE)}")
-        else:
-            rprint(f"[yellow] Database not found. Creating one at {DEDUP_DATABASE_FILE}")
-            os.makedirs(DEDUP_DATABASE_DIR, exist_ok=True)
+    def _add_perceptual_hashes_to_db(self, overwrite: bool, video_hashes=set | list) -> None:
+        # Create database folder
+        try:
+            os.makedirs(DEDUP_DATABASE_DIR, exist_ok=False)
+            # Exception before this log if directory already exists
             self.hydlog.info(f"Created DB dir {DEDUP_DATABASE_DIR}")
+        except OSError:
+            pass
 
-        search_tags = ["system:filetype=video"]
-        if custom_query is not None:
-            custom_query = [x for x in custom_query if x.strip()] # Remove whitespace and empty strings
-            search_tags.extend(custom_query)
-        
-        with SqliteDict(str(DEDUP_DATABASE_FILE), tablename = "videos",autocommit=True) as hashdb:
-            print(f"Retrieving video file hashes...")
-            all_video_hashes = self.client.search_files(search_tags, file_sort_type=hydrus_api.FileSortType.FILE_SIZE, return_hashes=True, file_sort_asc=True, return_file_ids=False)["hashes"]
-            print("Calculating perceptual hashes:")
-            with tqdm(dynamic_ncols=True, total=len(all_video_hashes), unit="video", colour="BLUE") as pbar:
-                with tempfile.TemporaryDirectory() as tmp_dir_name:
-                    for chunk_video_hashes in hydrus_api.utils.yield_chunks(all_video_hashes, chunk_size=16):
-                        for video_hash in chunk_video_hashes:
-                            pbar.update(1)
-                            # Only calculate new hash if it's missing or if overwrite is true
-                            if not overwrite and video_hash in hashdb and hashdb[video_hash].get("perceptual_hash", None) is not None:
-                                continue
-                            
-                            try:
-                                video_response = self.client.get_file(hash_=video_hash)
-                                if video_response.content is None:
-                                    continue
-                            except hydrus_api.HydrusAPIException:
-                                rprint("[red] Error getting file from database.")
-                                continue
-
-                            try:
-                                self._add_perceptual_hash_to_db(video_hash=video_hash, video=video_response.content, video_dir=tmp_dir_name, db=hashdb)
-                            except KeyboardInterrupt:
-                                rprint("[red] Perceptual hash generation was interrupted!\n")
+        with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
+            dblen = len(hashdb)
+            dbsize = os.path.getsize(DEDUP_DATABASE_FILE)
+
+            if dblen > 0:
+                rprint(f"[blue] Database found with {dblen} videos already hashed.")
+                self.hydlog.info(f"Database found of length {dblen}, size {dbsize} bytes")
+            else:
+                self.hydlog.info(f"Database not found. Creating one at {DEDUP_DATABASE_FILE}")
+
+            try:
+                with tqdm(total=len(video_hashes), dynamic_ncols=True, unit="video", colour="BLUE") as pbar:
+                    count_since_last_commit = 0
+                    COMMIT_INTERVAL = 16
+
+                    for video_hash in video_hashes:
+                        pbar.update(1)
+                        # Only calculate new hash if it's missing or if overwrite is true
+                        if not overwrite and video_hash in hashdb and "perceptual_hash" in hashdb[video_hash]:
+                            continue
+
+                        # Get video file from Hydrus
+                        try:
+                            video_response = self.client.get_file(hash_=video_hash)
+                            # video_metadata = self.client.get_file_metadata(hashes=[video_hash], only_return_basic_information=False)
+                            # print(video_metadata)
+                        except hydrus_api.HydrusAPIException:
+                            rprint("[red] Failed to get video from Hydrus.")
+                            self.hydlog.error("Error getting video from Hydrus.")
+                            continue
+
+                        # Calculate perceptual_hash
+                        try:
+                            perceptual_hash = self._calculate_perceptual_hash(video_response.content)
+                        except Exception as exc:
+                            rprint("[red] Failed to calculate a perceptual hash.")
+                            self.hydlog.exception(exc)
+                            self.hydlog.error(f"Errored file hash: {video_hash}")
+                        else:
+                            # Write perceptual hash to DB
+                            row = hashdb.get(video_hash, {})
+                            row["perceptual_hash"] = perceptual_hash
+                            hashdb[video_hash] = row
+
+                            # Batch DB commits to avoid excessive writes
+                            count_since_last_commit += 1
+                            if count_since_last_commit >= COMMIT_INTERVAL:
                                 hashdb.commit()
-                                return None
-                            except:
-                                rprint("[red] Failed to calculate a perceptual hash.")
-                                self.hydlog.error(f"Errored file hash: {video_hash}")
-                            
-                        # Commit at the end of a chunk
-                        hashdb.commit()
-                        
-                        # Each call to vpdq causes a defunct process because they didn't clean up the FFmpeg command in C++
-                        # Otherwise, the program will fill with zombie processes
-                        cleanup_defunct_processes()
-
-            # Commit at the end of all processing
-            hashdb.commit()
-            
-        rprint("[green] Finished perceptual hash processing.\n")
-    
+                                count_since_last_commit = 0
+                                self.hydlog.debug("Committed perceptual hashes to database.")
+
+                            self.hydlog.debug("Perceptual hash calculated.")
+
+            except KeyboardInterrupt:
+                interrupt_msg = "Perceptual hash processing was interrupted!"
+                rprint(f"[yellow] {interrupt_msg}")
+                self.hydlog.error(interrupt_msg)
+
+            else:
+                rprint("[green] Finished perceptual hash processing.")
+
+            finally:
+                hashdb.commit()
+                self.hydlog.info("Finished perceptual hash processing.")
+
     def get_potential_duplicate_count_hydrus(self) -> int:
-        return self.client.get_potentials_count(file_service_keys=[self.all_services["all_local_files"][0]["service_key"]])["potential_duplicates_count"]
-    
-    # Return similarity of two bitstrings given a threshold
-    @staticmethod
-    def is_similar(a: str, b: str, min_percent_similarity: float = 0.8) -> bool:
-        return VPDQSignal.compare_hash(a, b, min_percent_similarity, min_percent_similarity)
+        return self.client.get_potentials_count(
+            file_service_keys=[self.all_services["all_local_files"][0]["service_key"]]
+        )["potential_duplicates_count"]
+
+    def compare_videos(self, video1_hash: str, video2_hash: str, video1_phash: str, video2_phash: str):
+        vpdq_hash1 = Vpdq.json_to_vpdq(video1_phash)
+        vpdq_hash2 = Vpdq.json_to_vpdq(video2_phash)
+        similar, similarity = Vpdq.is_similar(vpdq_hash1, vpdq_hash2, self.threshold)
+
+        if similar:
+            if self._DEBUG:
+                # Getting the file names will be VERY slow because of the API call
+                # file_names = get_file_names_hydrus(self.client, [video1_hash, video2_hash])
+                # self.hydlog.info(f"Duplicates filenames: {file_names}")
+                self.hydlog.info(f"\"Similar {similarity}%: {video1_hash}\" and \"{video2_hash}\"")
+
+            new_relationship = {
+                "hash_a": str(video1_hash),
+                "hash_b": str(video2_hash),
+                "relationship": int(hydrus_api.DuplicateStatus.POTENTIAL_DUPLICATES),
+                "do_default_content_merge": True,
+            }
 
-    # Sliding window duplicate comparisons
-    # Alternatively, I could scan duplicates while adding and never do it again. I should do that instead.
-    # Or, since dictionaries are ordered, store the index per hash where it ended its last search. If it's not the end, keep going until the end.
-    def _find_potential_duplicates(self): 
-        # Check if table and DB exists before iterating over it since it's in read mode not the "c" r/w create mode
+            self.client.set_file_relationships([new_relationship])
+
+    # Delete cache row in database
+    @staticmethod
+    def clear_search_cache():
         try:
-            with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="r") as hashdb:
-                pass
+            with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
+                for key in hashdb:
+                    row = hashdb[key]
+                    if "farthest_search_index" in row:
+                        del row["farthest_search_index"]
+                    hashdb[key] = row
+                hashdb.commit()
         except OSError:
-            rprint(f"[red] Database does not exist. Cannot search for duplicates.")
-            return None
-        except RuntimeError: # SqliteDict error when trying to create a table for a DB in read-only mode
-            rprint(f"[red] Database does not exist. Cannot search for duplicates.")
-            return None
+            rprint(f"[red] Database does not exist. Cannot clear search cache.")
 
-        # TODO: Add support for query where it will get a list of the hashes from
-        # the query and iterate over them instead of the entire hashdb
-
-        # TODO: This can be multiprocessed
+    # Sliding window duplicate comparisons
+    # Alternatively, I could scan duplicates when added and never do it again which would be one of the best ways without a VP tree
+    def _find_potential_duplicates(self, limited_video_hashes: list | set | None = None) -> None:
+        if not database_accessible(DEDUP_DATABASE_FILE, tablename="videos", verbose=True):
+            rprint(f"[red] Could not search for duplicates.")
+            return
 
         # Number of potential duplicates before adding more. Just for user info.
         pre_dedupe_count = self.get_potential_duplicate_count_hydrus()
 
-        similar_files_found_count = 0
-        
+        # BUG: If this process is interrupted, the farthest_search_index will not save for ANY entries.
+        #      I think it might be because every entry in the column needs an entry for SQlite but I'm not sure.
         video_counter = 0
-        with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="r") as hashdb:
-            with tqdm(dynamic_ncols=True, total=len(hashdb), desc="Finding duplicates", unit="video", colour="BLUE") as pbar:
-                for i, video_hash in enumerate(hashdb):
-                    pbar.update(1)
-                    video_counter+=1
-                    video_phash = hashdb[video_hash]["perceptual_hash"]
-                    # TODO: Are sqlite databases ordered?
-                    for video2_hash in islice(hashdb, i+1, None):
-                        video2_phash = hashdb[video2_hash]["perceptual_hash"]
-                        
-                        similar = HydrusVideoDeduplicator.is_similar(video_phash, video2_phash, self.threshold)
-                        
-                        if similar:
-                            similar_files_found_count += 1
-                            if self._DEBUG:
-                                #file_names = get_file_names_hydrus(self.client, [video_hash, video2_hash])
-                                #self.hydlog.info(f"Duplicates filenames: {file_names}")
-                                self.hydlog.info(f"\"Duplicates hashes: {video_hash}\" and \"{video2_hash}\"")
-                            
-                            new_relationship = {
-                                "hash_a": str(video_hash),
-                                "hash_b": str(video2_hash),
-                                "relationship": int(hydrus_api.DuplicateStatus.POTENTIAL_DUPLICATES),
-                                "do_default_content_merge": True,
-                            }
-                        
-                            # TODO: Defer this API call to speed up processing
-                            self.client.set_file_relationships([new_relationship])
+        with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
+            try:
+                if limited_video_hashes is not None:
+                    total = len(limited_video_hashes)
+                else:
+                    total = len(hashdb)
+
+                with tqdm(
+                    dynamic_ncols=True, total=total, desc="Finding duplicates", unit="video", colour="BLUE"
+                ) as pbar:
+                    # -1 is all cores, -2 is all cores but one
+                    with Parallel(n_jobs=-2) as parallel:
+                        if limited_video_hashes is not None:
+                            # Avoid checking if in hashdb for each hash. Just do it now.
+                            clean_all_retrieved_video_hashes = [
+                                video_hash for video_hash in limited_video_hashes if video_hash in hashdb
+                            ]
+
+                            for i, video1_hash in enumerate(clean_all_retrieved_video_hashes):
+                                video_counter += 1
+                                pbar.update(1)
+                                parallel(
+                                    delayed(self.compare_videos)(
+                                        video1_hash,
+                                        clean_all_retrieved_video_hashes[j],
+                                        hashdb[video1_hash]["perceptual_hash"],
+                                        hashdb[clean_all_retrieved_video_hashes[j]]["perceptual_hash"],
+                                    )
+                                    for j in range(i + 1, len(clean_all_retrieved_video_hashes))
+                                )
+
+                        else:
+                            count_since_last_commit = 0
+                            commit_interval = 32
+
+                            for i, video1_hash in enumerate(hashdb):
+                                video_counter += 1
+                                pbar.update(1)
+
+                                row = hashdb[video1_hash]
+
+                                # Store last furthest searched position in the database for each element
+                                # This way you only have to start searching at that place instead of at i+1 if it exists
+                                row.setdefault("farthest_search_index", i + 1)
+
+                                # This is not necessary but may increase speed by avoiding any of the code below
+                                if row["farthest_search_index"] >= len(hashdb) - 1:
+                                    continue
+
+                                parallel(
+                                    delayed(self.compare_videos)(
+                                        video1_hash,
+                                        video2_hash,
+                                        hashdb[video1_hash]["perceptual_hash"],
+                                        hashdb[video2_hash]["perceptual_hash"],
+                                    )
+                                    for video2_hash in islice(hashdb, row["farthest_search_index"], None)
+                                )
+
+                                # Update furthest search position to the current length of the table
+                                row["farthest_search_index"] = len(hashdb) - 1
+                                hashdb[video1_hash] = row
+                                count_since_last_commit += 1
+
+                                if count_since_last_commit >= commit_interval:
+                                    hashdb.commit()
+                                    count_since_last_commit = 0
+
+            except KeyboardInterrupt:
+                pass
+            finally:
+                hashdb.commit()
 
         # Statistics for user
-        # if user does duplicates processing while the script is running this count will be wrong.
-        if similar_files_found_count > 0:
-            rprint(f"[blue] {similar_files_found_count}/{video_counter} similar videos found")
-            post_dedupe_count = self.get_potential_duplicate_count_hydrus()
-            new_dedupes_count = post_dedupe_count-pre_dedupe_count
-            if new_dedupes_count > 0:
-                rprint(f"[green] {new_dedupes_count} new potential duplicates marked for processing!")
-            else:
-                rprint("[green] No new potential duplicates")
+        post_dedupe_count = self.get_potential_duplicate_count_hydrus()
+        new_dedupes_count = post_dedupe_count - pre_dedupe_count
+        if new_dedupes_count > 0:
+            rprint(f"[green] {new_dedupes_count} new potential duplicates marked for processing!")
         else:
-            rprint(f"[yellow] No potential duplicates found out of {video_counter} videos")
+            rprint("[green] No new potential duplicates found.")
+
+    @staticmethod
+    def batched(iterable, n):
+        "Batch data into tuples of length n. The last batch may be shorter."
+        # batched('ABCDEFG', 3) --> ABC DEF G
+        if n < 1:
+            raise ValueError('n must be at least one')
+        it = iter(iterable)
+        while batch := tuple(islice(it, n)):
+            yield batch
+
+    # Check if files are trashed
+    # Returns a dictionary of hash : trashed_or_not
+    def is_files_trashed_hydrus(self, file_hashes: list[str]) -> dict:
+        videos_metadata = self.client.get_file_metadata(hashes=file_hashes, only_return_basic_information=False)[
+            "metadata"
+        ]
+
+        result = {}
+        for video_metadata in videos_metadata:
+            video_hash = video_metadata['hash']
+            is_trashed = video_metadata['is_trashed']
+            is_deleted = video_metadata['is_deleted']
+            result[video_hash] = is_trashed or is_deleted
+        return result
+
+    # Delete trashed and deleted files from Hydrus from the database
+    def clear_trashed_files_from_db(self):
+        if not database_accessible(DEDUP_DATABASE_FILE, tablename="videos"):
+            return
+
+        try:
+            CHUNK_SIZE = 32
+            delete_count = 0
+            with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
+                for batched_keys in self.batched(hashdb, CHUNK_SIZE):
+                    is_trashed_result = self.is_files_trashed_hydrus(batched_keys)
+                    for result in is_trashed_result.items():
+                        if result[1] is True:
+                            del hashdb[result[0]]
+                            delete_count += 1
+                    hashdb.commit()
+            self.hydlog.info(f"Cleared {delete_count} trashed files from the database.")
+        except OSError:
+            rprint("[red] Error while clearing trashed files cache.")
```

### Comparing `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/LICENSE` & `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/__init__.py` & `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,35 +278,43 @@
     _SET_KINGS_PATH = "/manage_file_relationships/set_kings"
 
     def __init__(
         self,
         access_key: T.Optional[str] = None,
         api_url: str = DEFAULT_API_URL,
         session: T.Optional[requests.Session] = None,
+        verify_cert: T.Optional[str] = None, # Path to cert
     ) -> None:
         """
         See https://hydrusnetwork.github.io/hydrus/client_api.html for documentation.
         """
 
         self.access_key = access_key
         self.api_url = api_url.rstrip("/")
+        self._verify_cert = verify_cert
         self.session = session or requests.Session()
 
     def _api_request(self, method: str, path: str, **kwargs: T.Any) -> requests.Response:
         if self.access_key is not None:
             kwargs.setdefault("headers", {}).update({"Hydrus-Client-API-Access-Key": self.access_key})
 
         # Make sure we use our custom JSONEncoder that can serialize all objects that implement the iterable or mapping
         # protocol
         json_data = kwargs.pop("json", None)
         if json_data is not None:
             kwargs["data"] = json.dumps(json_data, cls=_ABCJSONEncoder)
             # Since we aren't using the json keyword-argument, we have to set the Content-Type manually
             kwargs["headers"]["Content-Type"] = "application/json"
 
+        if self._verify_cert == None:
+            kwargs["verify"] = False
+            requests.packages.urllib3.disable_warnings() 
+        else:
+            kwargs["verify"] = self._verify_cert
+        
         try:
             response = self.session.request(method, self.api_url + path, **kwargs)
         except requests.RequestException as error:
             # Re-raise connection and timeout errors as hydrus.ConnectionErrors so these are more easy to handle for
             # client applications
             raise ConnectionError(*error.args)
```

### Comparing `hydrusvideodeduplicator-0.1.9/src/hydrusvideodeduplicator/hydrus_api/utils.py` & `hydrusvideodeduplicator-0.2.0/src/hydrusvideodeduplicator/hydrus_api/utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.9/.gitignore` & `hydrusvideodeduplicator-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.9/LICENSE` & `hydrusvideodeduplicator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.9/README.md` & `hydrusvideodeduplicator-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 <div align="center">
   
  # Hydrus Video Deduplicator
-  <img src="https://github.com/appleappleapplenanner/hydrus-video-deduplicator/assets/104981058/968603d3-5a11-4a05-bbb4-7b91b71fb61d">
-
+  <img src="https://github.com/appleappleapplenanner/hydrus-video-deduplicator/assets/104981058/e65383e8-1978-46aa-88b6-6fdda9767367">
   
 Hydrus Video Deduplicator detects similar video files and marks them as potential duplicates through the Hydrus API
 
 </div>
 
 ---
 
@@ -17,14 +16,16 @@
 
 The perceptual hashes are stored in a database file in the running directory to avoid computing them every time.
 
 Once all perceptual hashes for all the videos in your database are computed, they are compared against each other to detect if they're similar. If they are similar, they will be marked as potential duplicates in Hydrus.
 
 The accuracy is extremely good because of [vpdq](https://github.com/facebook/ThreatExchange/tree/main/vpdq). You can adjust the threshold of similarity using `--threshold`. The default is 75%.
 
+For more information check out the [wiki](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki) and the [FAQ](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/faq)
+
 ---
 
 ## Installation:
 
 [Windows requires WSL](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/Installation#Windows)
 
 ### Linux:
@@ -44,20 +45,21 @@
 python3 -m hydrusvideodeduplicator --api-key="<your key>"
 ```
 
 ---
 
 ## TODO:
 - [ ] Option to rollback and remove potential duplicates
-- [x] Option to enter custom Hydrus tag search parameters
+- [ ] OR predicates for --query
 - [ ] Parallelize hashing and duplicate search
 - [ ] Automatically generate access key with Hydrus API
-- [x] Upload to PyPI
-- [ ] Windows compatibility without WSL
-- [ ] Docker container (?)
+- [x] Docker container
+- [ ] Upload Docker container to Docker Hub (GitHub Action)
+- [ ] Pure Python port of vpdq
+- [ ] Windows compatibility without WSL or Docker
 
 Please create an issue on Github if you have any problems or questions! Pull requests also welcome on this or my VideoHash fork. 
 
 There is a lot to improve and cleanup and I'm more experienced in C than Python, so fix stuff please.
 
 ---
```

### Comparing `hydrusvideodeduplicator-0.1.9/pyproject.toml` & `hydrusvideodeduplicator-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dynamic = ["version"]
 description = "Video deduplicator utility for Hydrus Network"
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
-  { name = "appleappleapplenanner", email = "" },
+  { name = "appleappleapplenanner", email = "applenannerapple@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
@@ -23,17 +23,21 @@
 dependencies = [
     "appdirs",
     "rich",
     "numpy",
     "tqdm",
     "python-dotenv",
     "typer",
-    "vpdq",
     "sqlitedict",
     "requests",
+    "psutil",
+    "joblib",
+    # Below is for vpdqpy
+    "Pillow",
+    "av",
 ]
 
 [project.urls]
 Documentation = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme"
 Issues = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues"
 Source = "https://github.com/appleappleapplenanner/hydrus-video-deduplicator"
```

### Comparing `hydrusvideodeduplicator-0.1.9/PKG-INFO` & `hydrusvideodeduplicator-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.1.9
+Version: 0.2.0
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/appleappleapplenanner/hydrus-video-deduplicator
-Author: appleappleapplenanner
+Author-email: appleappleapplenanner <applenannerapple@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: appdirs
+Requires-Dist: av
+Requires-Dist: joblib
 Requires-Dist: numpy
+Requires-Dist: pillow
+Requires-Dist: psutil
 Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: sqlitedict
 Requires-Dist: tqdm
 Requires-Dist: typer
-Requires-Dist: vpdq
 Description-Content-Type: text/markdown
 
 <div align="center">
   
  # Hydrus Video Deduplicator
-  <img src="https://github.com/appleappleapplenanner/hydrus-video-deduplicator/assets/104981058/968603d3-5a11-4a05-bbb4-7b91b71fb61d">
-
+  <img src="https://github.com/appleappleapplenanner/hydrus-video-deduplicator/assets/104981058/e65383e8-1978-46aa-88b6-6fdda9767367">
   
 Hydrus Video Deduplicator detects similar video files and marks them as potential duplicates through the Hydrus API
 
 </div>
 
 ---
 
@@ -44,14 +46,16 @@
 
 The perceptual hashes are stored in a database file in the running directory to avoid computing them every time.
 
 Once all perceptual hashes for all the videos in your database are computed, they are compared against each other to detect if they're similar. If they are similar, they will be marked as potential duplicates in Hydrus.
 
 The accuracy is extremely good because of [vpdq](https://github.com/facebook/ThreatExchange/tree/main/vpdq). You can adjust the threshold of similarity using `--threshold`. The default is 75%.
 
+For more information check out the [wiki](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki) and the [FAQ](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/faq)
+
 ---
 
 ## Installation:
 
 [Windows requires WSL](https://github.com/appleappleapplenanner/hydrus-video-deduplicator/wiki/Installation#Windows)
 
 ### Linux:
@@ -71,20 +75,21 @@
 python3 -m hydrusvideodeduplicator --api-key="<your key>"
 ```
 
 ---
 
 ## TODO:
 - [ ] Option to rollback and remove potential duplicates
-- [x] Option to enter custom Hydrus tag search parameters
+- [ ] OR predicates for --query
 - [ ] Parallelize hashing and duplicate search
 - [ ] Automatically generate access key with Hydrus API
-- [x] Upload to PyPI
-- [ ] Windows compatibility without WSL
-- [ ] Docker container (?)
+- [x] Docker container
+- [ ] Upload Docker container to Docker Hub (GitHub Action)
+- [ ] Pure Python port of vpdq
+- [ ] Windows compatibility without WSL or Docker
 
 Please create an issue on Github if you have any problems or questions! Pull requests also welcome on this or my VideoHash fork. 
 
 There is a lot to improve and cleanup and I'm more experienced in C than Python, so fix stuff please.
 
 ---
```

