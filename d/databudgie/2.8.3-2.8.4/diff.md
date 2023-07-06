# Comparing `tmp/databudgie-2.8.3.tar.gz` & `tmp/databudgie-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databudgie-2.8.3.tar", max compression
+gzip compressed data, was "databudgie-2.8.4.tar", max compression
```

## Comparing `databudgie-2.8.3.tar` & `databudgie-2.8.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     5139 2023-06-21 20:25:54.906850 databudgie-2.8.3/CHANGELOG.md
--rw-r--r--   0        0        0     1973 2023-06-21 20:25:54.906850 databudgie-2.8.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1053 2023-06-21 20:25:54.906850 databudgie-2.8.3/LICENSE
--rw-r--r--   0        0        0     1310 2023-06-21 20:25:54.906850 databudgie-2.8.3/README.md
--rw-r--r--   0        0        0     2883 2023-06-21 20:25:54.910850 databudgie-2.8.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/__init__.py
--rw-r--r--   0        0        0       69 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/__main__.py
--rw-r--r--   0        0        0       74 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/adapter/__init__.py
--rw-r--r--   0        0        0     7584 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/adapter/base.py
--rw-r--r--   0        0        0    11357 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/adapter/postgres.py
--rw-r--r--   0        0        0     7545 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/backup.py
--rw-r--r--   0        0        0      105 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/cli/__init__.py
--rw-r--r--   0        0        0     3071 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/cli/base.py
--rw-r--r--   0        0        0     6738 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/cli/commands.py
--rw-r--r--   0        0        0     4944 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/cli/config.py
--rw-r--r--   0        0        0     1112 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/compression.py
--rw-r--r--   0        0        0    11855 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/config.py
--rw-r--r--   0        0        0      105 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/manifest/__init__.py
--rw-r--r--   0        0        0     2348 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/manifest/manager.py
--rw-r--r--   0        0        0     1602 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/manifest/sqlalchemy.py
--rw-r--r--   0        0        0      565 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/match.py
--rw-r--r--   0        0        0     1564 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/output.py
--rw-r--r--   0        0        0        0 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/py.typed
--rw-r--r--   0        0        0     8014 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/restore.py
--rw-r--r--   0        0        0     1948 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/s3.py
--rw-r--r--   0        0        0    11836 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/storage.py
--rw-r--r--   0        0        0     4586 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/table_op.py
--rw-r--r--   0        0        0     2462 2023-06-21 20:25:54.910850 databudgie-2.8.3/src/databudgie/utils.py
--rw-r--r--   0        0        0     2580 1970-01-01 00:00:00.000000 databudgie-2.8.3/setup.py
--rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 databudgie-2.8.3/PKG-INFO
+-rw-r--r--   0        0        0     5139 2023-07-06 13:48:54.085334 databudgie-2.8.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1973 2023-07-06 13:48:54.085334 databudgie-2.8.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1053 2023-07-06 13:48:54.085334 databudgie-2.8.4/LICENSE
+-rw-r--r--   0        0        0     1310 2023-07-06 13:48:54.085334 databudgie-2.8.4/README.md
+-rw-r--r--   0        0        0     2889 2023-07-06 13:48:54.089334 databudgie-2.8.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/__main__.py
+-rw-r--r--   0        0        0       74 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/adapter/__init__.py
+-rw-r--r--   0        0        0     7653 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/adapter/base.py
+-rw-r--r--   0        0        0    11357 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/adapter/postgres.py
+-rw-r--r--   0        0        0     2974 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/api.py
+-rw-r--r--   0        0        0     7628 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/backup.py
+-rw-r--r--   0        0        0      105 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/cli/__init__.py
+-rw-r--r--   0        0        0     3071 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/cli/base.py
+-rw-r--r--   0        0        0     5913 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/cli/commands.py
+-rw-r--r--   0        0        0     4944 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/cli/config.py
+-rw-r--r--   0        0        0     1112 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/compression.py
+-rw-r--r--   0        0        0    11869 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/config.py
+-rw-r--r--   0        0        0      105 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/manifest/__init__.py
+-rw-r--r--   0        0        0     2348 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/manifest/manager.py
+-rw-r--r--   0        0        0     1602 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/manifest/sqlalchemy.py
+-rw-r--r--   0        0        0      565 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/match.py
+-rw-r--r--   0        0        0     1564 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/output.py
+-rw-r--r--   0        0        0        0 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/py.typed
+-rw-r--r--   0        0        0     8118 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/restore.py
+-rw-r--r--   0        0        0     1948 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/s3.py
+-rw-r--r--   0        0        0    11836 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/storage.py
+-rw-r--r--   0        0        0     5112 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/table_op.py
+-rw-r--r--   0        0        0     2845 2023-07-06 13:48:54.089334 databudgie-2.8.4/src/databudgie/utils.py
+-rw-r--r--   0        0        0     2587 1970-01-01 00:00:00.000000 databudgie-2.8.4/setup.py
+-rw-r--r--   0        0        0     2663 1970-01-01 00:00:00.000000 databudgie-2.8.4/PKG-INFO
```

### Comparing `databudgie-2.8.3/CHANGELOG.md` & `databudgie-2.8.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/CONTRIBUTING.md` & `databudgie-2.8.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/LICENSE` & `databudgie-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/README.md` & `databudgie-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/pyproject.toml` & `databudgie-2.8.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databudgie"
-version = "2.8.3"
+version = "2.8.4"
 packages = [
     { include = "databudgie", from = "src" },
 ]
 
 authors = [
   "Andrew Sosa <andrewso@known.is>",
   "Dan Cardin <ddcardin@gmail.com>",
@@ -26,15 +26,15 @@
 [tool.poetry.scripts]
 databudgie = "databudgie.__main__:run"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4"
 
 rich = "*"
-configly = {version = "*", extras = ["yaml"]}
+configly = {version = ">=1.0.0", extras = ["yaml"]}
 sqlalchemy = ">=1.3"
 strapp = {version = ">=0.2.7", extras = ["click", "sqlalchemy"] }
 click = ">=7.0.0"
 typing-extensions = {version = ">=3.10.0", python = "<3.8"}
 importlib-metadata = {version = "*", python = "<3.8"}
 
 boto3 = { version = "*", optional = true }
```

### Comparing `databudgie-2.8.3/src/databudgie/adapter/base.py` & `databudgie-2.8.4/src/databudgie/adapter/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,17 @@
         table_ops: list[TableOp],
         reverse: bool = False,
         console: Console = default_console,
     ) -> list[TableOp]:
         tables = set()
         dependent_table_ops = []
         for table_op in table_ops:
+            if table_op.full_name is None:
+                continue
+
             tables.add(table_op.full_name)
 
             if not table_op.raw_conf.follow_foreign_keys:
                 continue
 
             dependent_tables = self.collect_table_dependencies(table_op=table_op, console=console)
             for dependent_table in dependent_tables:
```

### Comparing `databudgie-2.8.3/src/databudgie/adapter/postgres.py` & `databudgie-2.8.4/src/databudgie/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/src/databudgie/backup.py` & `databudgie-2.8.4/src/databudgie/backup.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     # Backup schemas first
     schema_names = set()
     schemas = []
 
     for table_op in table_ops:
         schema_op = table_op.schema_op()
-        if schema_op.name in schemas:
+        if not schema_op or schema_op.name in schemas:
             continue
 
         if not table_op.raw_conf.ddl:
             continue
 
         schema_names.add(schema_op.name)
         schemas.append(schema_op)
@@ -111,28 +111,28 @@
             )
 
             console.trace(f"Wrote {schema_op.name} to {filename}")
 
         console.info("Finished backing up schema DDL")
 
         for table_op in table_ops:
-            if not table_op.raw_conf.ddl:
+            if not table_op.full_name or not table_op.raw_conf.ddl:
                 continue
 
-            progress.update(task, description=f"Backing up DDL: {table_op.full_name}")
+            progress.update(task, description=f"Backing up DDL: {table_op.pretty_name}")
             result = adapter.export_table_ddl(table_op.full_name)
 
             filename = storage.write_buffer(
                 join_paths(backup_config.ddl.location, table_op.location()),
                 io.BytesIO(result),
                 file_type=FileTypes.ddl,
                 name=table_op.full_name,
             )
 
-            console.trace(f"Uploaded {table_op.full_name} to {filename}")
+            console.trace(f"Uploaded {table_op.pretty_name} to {filename}")
             table_names.append(table_op.full_name)
 
     console.info("Finished backing up DDL")
 
     # On the restore-side, the tables may not already exist (at the extreme, you
     # might start with an empty database), so we need to record the set of tables
     # being backed up.
@@ -154,19 +154,19 @@
 
     table_sequences = adapter.collect_table_sequences()
 
     with Progress(console) as progress:
         task = progress.add_task("Backing up sequence positions", total=len(table_ops))
 
         for table_op in table_ops:
-            progress.update(task, description=f"Backing up sequence position: {table_op.full_name}")
-
-            if not table_op.raw_conf.sequences:
+            if not table_op.full_name or not table_op.raw_conf.sequences:
                 continue
 
+            progress.update(task, description=f"Backing up sequence position: {table_op.pretty_name}")
+
             sequences = table_sequences.get(table_op.full_name)
             if not sequences:
                 continue
 
             sequence_values = {}
             for sequence in sequences:
                 sequence_values[sequence] = adapter.collect_sequence_value(sequence)
@@ -178,15 +178,15 @@
             filename = storage.write_buffer(
                 join_paths(path, "sequences"),
                 io.BytesIO(result),
                 file_type=FileTypes.sequences,
                 name=table_op.full_name,
             )
 
-            console.trace(f"Wrote {table_op.full_name} sequences to {filename}")
+            console.trace(f"Wrote {table_op.pretty_name} sequences to {filename}")
 
     console.info("Finished backing up sequence positions")
 
 
 def backup_tables(
     table_ops: Sequence[TableOp],
     storage: StorageBackend,
@@ -194,15 +194,15 @@
     adapter: Adapter,
     console: Console = default_console,
 ) -> None:
     with Progress(console) as progress:
         task = progress.add_task("Backing up tables", total=len(table_ops))
 
         for table_op in table_ops:
-            progress.update(task, description=f"Backing up table: {table_op.full_name}")
+            progress.update(task, description=f"Backing up table: {table_op.pretty_name}")
 
             if not table_op.raw_conf.data:
                 continue
 
             with capture_failures(strict=table_op.raw_conf.strict):
                 backup(
                     table_op=table_op,
@@ -229,20 +229,20 @@
         adapter: the selected behavior adapter
         storage: the storage backend to use for backing up the data.
         console: Console used for output
     """
     path = table_op.location()
 
     if table_op.raw_conf.skip_if_exists and storage.path_exists(path):
-        console.trace(f"Skipping {table_op.full_name} due to `skip_if_exists`")
+        console.trace(f"Skipping {table_op.pretty_name} due to `skip_if_exists`")
         return
 
     buffer = adapter.export_query(table_op.query())
 
     # path.join will handle optionally trailing slashes in the location
     compression = table_op.raw_conf.compression
 
     filename = storage.write_buffer(
         path, buffer, file_type=FileTypes.data, name=table_op.full_name, compression=compression
     )
 
-    console.trace(f"Uploaded {table_op.full_name} to {filename}")
+    console.trace(f"Uploaded {table_op.pretty_name} to {filename}")
```

### Comparing `databudgie-2.8.3/src/databudgie/cli/base.py` & `databudgie-2.8.4/src/databudgie/cli/base.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/src/databudgie/cli/commands.py` & `databudgie-2.8.4/src/databudgie/cli/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-import os
 from typing import Iterable, Optional, Tuple
 
 import click
 from sqlalchemy.orm import Session
 
+from databudgie import api
 from databudgie.cli.base import resolver
 from databudgie.cli.config import (
-    CliConfig,
-    collect_config,
     file_loaders,
     pretty_print,
 )
 from databudgie.config import (
     BackupConfig,
     ConfigError,
     RestoreConfig,
     RootConfig,
 )
 from databudgie.manifest.manager import Manifest
 from databudgie.output import Console
-from databudgie.storage import StorageBackend
 
 
 @resolver.group()
 @click.option("--strict/--no-strict", is_flag=True, default=None)
 @click.option("--color/--no-color", is_flag=True, default=True)
 @click.option(
     "-a",
@@ -81,51 +78,42 @@
     "--raw-config-format",
     default="json",
     help="The assumed format of --raw-config. Defaults to `json`. Must be one of: `yml`, `yaml`, `json`, `toml`.",
     type=click.Choice(file_loaders),
 )
 @click.version_option()
 def cli(
-    strict: bool,
-    config: Iterable[str],
+    strict: bool = False,
+    config: Iterable[str] = (),
     verbose: int = 0,
     color: bool = True,
     conn: Optional[str] = None,
     adapter: Optional[str] = None,
     ddl: Optional[bool] = None,
     url: Optional[str] = None,
     table: Optional[Tuple[str, ...]] = None,
     exclude: Optional[Tuple[str, ...]] = None,
     location: Optional[str] = None,
     dry_run: bool = False,
     stats: bool = False,
     raw_config: Optional[str] = None,
     raw_config_format: str = "json",
 ):
-    if color is False:
-        os.environ["NO_COLOR"] = "true"
-
-    if conn and url:
-        raise click.UsageError("--url and --connection are mutually exclusive options")
-
-    cli_config = CliConfig(
-        ddl=ddl,
-        tables=list(table) if table else None,
-        exclude=list(exclude) if exclude else None,
-        url=url,
-        location=location,
-        adapter=adapter,
-        strict=strict,
-        connection=conn,
-    )
-
     try:
-        root_config = collect_config(
-            cli_config=cli_config,
-            file_names=config,
+        root_config = api.root_config(
+            strict=strict,
+            config=config,
+            color=color,
+            conn=conn,
+            adapter=adapter,
+            ddl=ddl,
+            url=url,
+            table=table,
+            exclude=exclude,
+            location=location,
             raw_config=raw_config,
             raw_config_format=raw_config_format,
         )
     except ConfigError as e:
         raise click.UsageError(*e.args)
 
     resolver.register_values(
@@ -145,35 +133,28 @@
     console: Console,
     backup_manifest: Optional[Manifest] = None,
     backup_id: Optional[int] = None,
     stats: bool = False,
     dry_run: bool = False,
 ):
     """Perform backup."""
-    from databudgie.backup import backup_all
-
-    if backup_manifest and backup_id:
-        backup_manifest.set_transaction_id(backup_id)
-
-    storage = StorageBackend.from_config(
-        backup_config,
-        manifest=backup_manifest,
-        record_stats=stats,
-        perform_writes=not dry_run,
-    )
-
     try:
-        backup_all(backup_db, backup_config, storage=storage, console=console)
+        api.backup(
+            backup_db,
+            backup_config,
+            manifest=backup_manifest,
+            console=console,
+            stats=stats,
+            dry_run=dry_run,
+            transaction_id=backup_id,
+        )
     except Exception as e:
         console.trace(e)
         raise click.ClickException(str(e))
 
-    if stats:
-        storage.print_stats()
-
 
 @resolver.command(cli, "restore")
 @click.option("--restore-id", default=None, help="Restore manifest id.")
 @click.option(
     "--clean/--no-clean",
     is_flag=True,
     default=None,
@@ -194,43 +175,32 @@
     restore_id: Optional[int] = None,
     clean: Optional[bool] = None,
     yes: bool = False,
     stats: bool = False,
     dry_run: bool = False,
 ):
     """Perform restore."""
-    from databudgie.restore import restore_all
-
-    if restore_manifest and restore_id:
-        restore_manifest.set_transaction_id(restore_id)
-
-    restore_config.ddl.clean = clean or restore_config.ddl.clean
-
-    if not yes and restore_config.ddl.clean:
+    if not yes and (clean or restore_config.ddl.clean):
         message = "About to delete the database! input 'y' if that's what you want: "
         if input(message) != "y":  # nosec
             return
 
-    if dry_run:
-        raise click.UsageError("--dry-run is not (yet) supported for restore")
-
-    storage = StorageBackend.from_config(
-        restore_config,
-        manifest=restore_manifest,
-        record_stats=stats,
-        perform_writes=not dry_run,
-    )
-
     try:
-        restore_all(restore_db, restore_config=restore_config, storage=storage, console=console)
+        api.restore(
+            db=restore_db,
+            config=restore_config,
+            console=console,
+            manifest=restore_manifest,
+            transaction_id=restore_id,
+            clean=clean,
+            stats=stats,
+            dry_run=dry_run,
+        )
     except Exception as e:
         console.trace(e)
         raise click.ClickException(*e.args)
 
-    if stats:
-        storage.print_stats()
-
 
 @resolver.command(cli, "config")
 def config_cli(root_config: RootConfig):
     """Print dereferenced and populated config."""
     pretty_print(root_config)
```

### Comparing `databudgie-2.8.3/src/databudgie/cli/config.py` & `databudgie-2.8.4/src/databudgie/cli/config.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/src/databudgie/compression.py` & `databudgie-2.8.4/src/databudgie/compression.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/src/databudgie/config.py` & `databudgie-2.8.4/src/databudgie/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
             if connection is not None:
                 result[k] = connection
         return result
 
 
 @dataclass
 class BackupTableConfig(Config):
-    name: str
+    name: str | None = None
     location: str = "backups/{table}"
     query: str = "select * from {table}"
     compression: str | None = None
     exclude: list = field(default_factory=list)
     ddl: bool = True
     sequences: bool = True
     data: bool = True
```

### Comparing `databudgie-2.8.3/src/databudgie/manifest/manager.py` & `databudgie-2.8.4/src/databudgie/manifest/manager.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/src/databudgie/manifest/sqlalchemy.py` & `databudgie-2.8.4/src/databudgie/manifest/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/src/databudgie/match.py` & `databudgie-2.8.4/src/databudgie/match.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/src/databudgie/output.py` & `databudgie-2.8.4/src/databudgie/output.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/src/databudgie/restore.py` & `databudgie-2.8.4/src/databudgie/restore.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     )
 
     schema_names = set()
     schema_ops = []
 
     for table_op in table_ops:
         schema_op = table_op.schema_op()
-        if schema_op.name in schema_names:
+        if not schema_op or schema_op.name in schema_names:
             continue
 
         if not table_op.raw_conf.ddl:
             continue
 
         schema_names.add(schema_op.name)
         schema_ops.append(schema_op)
@@ -195,15 +195,15 @@
 def truncate_tables(table_ops: Sequence[TableOp], adapter: Adapter, console: Console):
     with Progress(console) as progress:
         task = progress.add_task("Truncating Tables", total=len(table_ops))
 
         for table_op in table_ops:
             data = table_op.raw_conf.data
             truncate = table_op.raw_conf.truncate
-            if not data or not truncate:
+            if not data or not truncate or table_op.full_name is None:
                 continue
 
             progress.update(task, description=f"[trace]Truncating {table_op.full_name}[/trace]", advance=1)
             adapter.truncate_table(table_op.full_name)
 
     console.info("Finished truncating tables")
 
@@ -216,15 +216,15 @@
     storage: StorageBackend,
     console: Console = default_console,
 ) -> None:
     with Progress(console) as progress:
         task = progress.add_task("Restoring tables", total=len(table_ops))
 
         for table_op in table_ops:
-            if not table_op.raw_conf.data:
+            if not table_op.full_name or not table_op.raw_conf.data:
                 continue
 
             progress.update(task, description=f"Restoring table: {table_op.full_name}")
 
             with capture_failures(strict=table_op.raw_conf.strict):
                 restore(
                     session,
@@ -242,14 +242,16 @@
     *,
     adapter: Adapter,
     storage: StorageBackend,
     table_op: TableOp,
     console: Console = default_console,
 ) -> None:
     """Restore a CSV file from S3 to the database."""
+    assert table_op.full_name
+
     # Force table_name to be fully qualified
     schema, table = parse_table(table_op.full_name)
     table_name = f"{schema}.{table}"
 
     strategy: str = table_op.raw_conf.strategy
     compression = table_op.raw_conf.compression
```

### Comparing `databudgie-2.8.3/src/databudgie/s3.py` & `databudgie-2.8.4/src/databudgie/s3.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/src/databudgie/storage.py` & `databudgie-2.8.4/src/databudgie/storage.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.8.3/src/databudgie/table_op.py` & `databudgie-2.8.4/src/databudgie/table_op.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,17 +37,17 @@
      * `raw_conf`: directly relates to the raw table config in a backup/restore config.
 
     Note all `TableOp` records should correspond to concrete tables. That is, given some
     globbed input table "public.*", a `TableOp` will only be produced for a concrete
     table matching that criteria.
     """
 
-    schema: str
-    table_name: str
-    full_name: str
+    schema: str | None
+    table_name: str | None
+    full_name: str | None
     raw_conf: T
 
     @classmethod
     def from_name(cls, full_name: str, raw_conf: T):
         schema, table_name = parse_table(full_name)
         return cls(schema=schema, table_name=table_name, full_name=full_name, raw_conf=raw_conf)
 
@@ -57,17 +57,28 @@
     def query(self) -> str:
         query = getattr(self.raw_conf, "query")  # RestoreTableConfig has no query attribute
         if query is None:
             query = "SELECT * FROM {table}"
 
         return query.format(table=self.full_name)
 
-    def schema_op(self) -> SchemaOp:
+    def schema_op(self) -> SchemaOp | None:
+        if self.schema is None:
+            return None
+
         return SchemaOp(self.schema, self.raw_conf)
 
+    @property
+    def pretty_name(self) -> str:
+        if self.full_name:
+            return self.full_name
+
+        assert isinstance(self.raw_conf, BackupTableConfig)
+        return self.raw_conf.query
+
 
 def expand_table_ops(
     session: Session,
     tables: Sequence[T],
     existing_tables: list[str],
     storage: StorageBackend,
     *,
@@ -85,16 +96,21 @@
     # Avoid hardcoding things like "public", we hardcode this elsewhere, this
     # should probably be moved upstream.
     insp = inspect(session.connection())
     default_schema_name = insp.default_schema_name
 
     # expand table globs into fully qualified mappings to the config.
     matching_tables: dict[str, list[T]] = {}
+    unnamed_tables: list[T] = []
     for table_conf in tables:
         pattern = table_conf.name
+        if pattern is None:
+            unnamed_tables.append(table_conf)
+            continue
+
         if "." not in pattern:
             pattern = f"{default_schema_name}.{pattern}"
 
         expanded_tables = expand_table_globs(existing_tables, pattern)
         if warn_for_unused_tables and not expanded_tables:
             console.warn(f"Skipping table definition `{pattern}` which did not match any tables.")
             continue
@@ -124,8 +140,11 @@
         if not table_confs:
             continue
 
         for table_conf in table_confs:
             table_op = TableOp.from_name(table, raw_conf=table_conf)
             result.append(table_op)
 
+    for unnamed_table in unnamed_tables:
+        result.append(TableOp(None, None, None, unnamed_table))
+
     return result
```

### Comparing `databudgie-2.8.3/src/databudgie/utils.py` & `databudgie-2.8.4/src/databudgie/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,18 +77,29 @@
 
     if not real_components:
         return ""
 
     if len(real_components) == 1:
         return real_components[0]
 
-    first_component, *rest_components = real_components
+    bucket = None
     normalized_components = []
-    for c in rest_components:
+    for index, c in enumerate(real_components):
+        normalized_c = c
         if is_s3_path(c):
-            normalized_c = S3Location(c).key
+            s3_location = S3Location(c)
+            if bucket is None:
+                bucket = s3_location.bucket
+            else:
+                if bucket != s3_location.bucket:
+                    raise ValueError(f"Path contains two different buckets: {bucket}, {s3_location.bucket}")
+            normalized_c = s3_location.key
         else:
-            normalized_c = c.strip("/")
+            if index != 0:
+                normalized_c = c.lstrip("/")
 
         normalized_components.append(normalized_c)
 
-    return os.path.join(first_component, *normalized_components)
+    if bucket:
+        normalized_components.insert(0, f"s3://{bucket}")
+
+    return os.path.join(*normalized_components)
```

### Comparing `databudgie-2.8.3/setup.py` & `databudgie-2.8.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['databudgie', 'databudgie.adapter', 'databudgie.cli', 'databudgie.manifest']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=7.0.0',
- 'configly[yaml]',
+ 'configly[yaml]>=1.0.0',
  'rich',
  'sqlalchemy>=1.3',
  'strapp[click,sqlalchemy]>=0.2.7']
 
 extras_require = \
 {':python_version < "3.8"': ['typing-extensions>=3.10.0', 'importlib-metadata'],
  'psycopg2': ['psycopg2>=2.7'],
@@ -24,15 +24,15 @@
  's3': ['boto3']}
 
 entry_points = \
 {'console_scripts': ['databudgie = databudgie.__main__:run']}
 
 setup_kwargs = {
     'name': 'databudgie',
-    'version': '2.8.3',
+    'version': '2.8.4',
     'description': 'Ergonomic and flexible tool for database backup and restore',
     'long_description': '# Databudgie\n\n![Github Actions Build](https://github.com/schireson/databudgie/actions/workflows/build.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/schireson/databudgie/badge.svg?branch=main&t=6I0aU6)](https://coveralls.io/github/schireson/databudgie?branch=main)\n[![Documentation\nStatus](https://readthedocs.org/projects/databudgie/badge/?version=latest)](https://databudgie.readthedocs.io)\n\n![](docs/source/_static/databudgie.png)\n\nDatabudgie is a CLI & library for database performing targeted backup and\nrestore of database tables or arbitrary queries against database tables.\n\n# Usage\n\nA minimal config file might look like:\n\n```yaml\n# databudgie.yml or config.databudgie.yml\nbackup:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      query: "select * from {table} where store_id > 4"\n      location: s3://my-s3-bucket/databudgie/public.product\nrestore:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      location: s3://my-s3-bucket/databudgie/public.product\n```\n\nWith that config in place, backing up the defined tables (using the specified\nconfig) is as simple as `databudgie backup`; and restore `databudgie restore`.\n\n## Installation\n\n```bash\npip install databudgie\n```\n',
     'author': 'Andrew Sosa',
     'author_email': 'andrewso@known.is',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/schireson/databudgie',
```

### Comparing `databudgie-2.8.3/PKG-INFO` & `databudgie-2.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databudgie
-Version: 2.8.3
+Version: 2.8.4
 Summary: Ergonomic and flexible tool for database backup and restore
 Home-page: https://github.com/schireson/databudgie
 License: MIT
 Keywords: sqlalchemy,postgres,database,etl,s3
 Author: Andrew Sosa
 Author-email: andrewso@known.is
 Requires-Python: >=3.7,<4
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Archiving :: Backup
 Provides-Extra: psycopg2
 Provides-Extra: psycopg2-binary
 Provides-Extra: s3
 Requires-Dist: boto3; extra == "s3"
 Requires-Dist: click (>=7.0.0)
-Requires-Dist: configly[yaml]
+Requires-Dist: configly[yaml] (>=1.0.0)
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: psycopg2 (>=2.7); extra == "psycopg2"
 Requires-Dist: psycopg2-binary (>=2.7); extra == "psycopg2-binary"
 Requires-Dist: rich
 Requires-Dist: sqlalchemy (>=1.3)
 Requires-Dist: strapp[click,sqlalchemy] (>=0.2.7)
 Requires-Dist: typing-extensions (>=3.10.0); python_version < "3.8"
```

