# Comparing `tmp/sqlsynthgen-0.2.0.tar.gz` & `tmp/sqlsynthgen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlsynthgen-0.2.0.tar", max compression
+gzip compressed data, was "sqlsynthgen-0.3.0.tar", max compression
```

## Comparing `sqlsynthgen-0.2.0.tar` & `sqlsynthgen-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1082 2023-06-01 16:18:08.329813 sqlsynthgen-0.2.0/LICENSE
--rw-r--r--   0        0        0      247 2023-06-01 16:18:08.329813 sqlsynthgen-0.2.0/README.md
--rw-r--r--   0        0        0     1170 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/__init__.py
--rw-r--r--   0        0        0      637 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/base.py
--rw-r--r--   0        0        0     5411 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/create.py
--rw-r--r--   0        0        0     2946 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/json_schemas/config_schema.json
--rw-r--r--   0        0        0     7012 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/main.py
--rw-r--r--   0        0        0    14869 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/make.py
--rw-r--r--   0        0        0     3107 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/providers.py
--rw-r--r--   0        0        0     4632 2023-06-01 16:18:08.333813 sqlsynthgen-0.2.0/sqlsynthgen/settings.py
--rw-r--r--   0        0        0     2122 2023-06-01 16:18:08.337813 sqlsynthgen-0.2.0/sqlsynthgen/templates/ssg.py.j2
--rw-r--r--   0        0        0     2149 2023-06-01 16:18:08.337813 sqlsynthgen-0.2.0/sqlsynthgen/utils.py
--rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 sqlsynthgen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-06 13:13:39.539871 sqlsynthgen-0.3.0/LICENSE
+-rw-r--r--   0        0        0      247 2023-07-06 13:13:39.539871 sqlsynthgen-0.3.0/README.md
+-rw-r--r--   0        0        0     1263 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/base.py
+-rw-r--r--   0        0        0     5171 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/create.py
+-rw-r--r--   0        0        0     3146 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/json_schemas/config_schema.json
+-rw-r--r--   0        0        0     8755 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/main.py
+-rw-r--r--   0        0        0    18739 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/make.py
+-rw-r--r--   0        0        0     3117 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/providers.py
+-rw-r--r--   0        0        0     1817 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/remove.py
+-rw-r--r--   0        0        0     2418 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/settings.py
+-rw-r--r--   0        0        0     2815 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/templates/ssg.py.j2
+-rw-r--r--   0        0        0     5256 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/unique_generator.py
+-rw-r--r--   0        0        0     2559 2023-07-06 13:13:39.547870 sqlsynthgen-0.3.0/sqlsynthgen/utils.py
+-rw-r--r--   0        0        0     1465 1970-01-01 00:00:00.000000 sqlsynthgen-0.3.0/PKG-INFO
```

### Comparing `sqlsynthgen-0.2.0/LICENSE` & `sqlsynthgen-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlsynthgen-0.2.0/pyproject.toml` & `sqlsynthgen-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [tool.poetry]
 name = "sqlsynthgen"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Iain <25081046+Iain-S@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 pydantic = {extras = ["dotenv"], version = "^1.10.2"}
 psycopg2-binary = "^2.9.5"
 sqlalchemy-utils = "^0.38.3"
 mimesis = "^6.1.1"
 typer = "^0.7.0"
 pyyaml = "^5.0"
-sqlalchemy = "^1.4"
+sqlalchemy = {version = "^1.4", extras = ["asyncio"]}
 sphinx-rtd-theme = {version = "^1.2.0", optional = true}
 sphinxcontrib-napoleon = {version = "^0.7", optional = true}
 smartnoise-sql = "^0.2.11"
 jinja2 = "^3.1.2"
 black = "^23.3.0"
 jsonschema = "^4.17.3"
 sqlacodegen = "3.0.0rc1"
+asyncpg = "^0.27.0"
+greenlet = "^2.0.2"
+pymysql = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
 pylint = "^2.15.8"
 mypy = "^0.991"
 types-pyyaml = "^6.0.12.4"
 pydocstyle = "^6.3.0"
```

### Comparing `sqlsynthgen-0.2.0/sqlsynthgen/create.py` & `sqlsynthgen-0.3.0/sqlsynthgen/create.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 """Functions and classes to create and populate the target database."""
 import logging
 from typing import Any, Dict, Generator, List, Tuple
 
-from sqlalchemy import create_engine, insert
+from sqlalchemy import insert
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.schema import CreateSchema
 
 from sqlsynthgen.settings import get_settings
-from sqlsynthgen.utils import create_engine_with_search_path
+from sqlsynthgen.utils import create_db_engine
 
 Story = Generator[Tuple[str, Dict[str, Any]], Dict[str, Any], None]
 
 
 def create_db_tables(metadata: Any) -> Any:
     """Create tables described by the sqlalchemy metadata object."""
     settings = get_settings()
 
-    engine = create_engine(settings.dst_postgres_dsn)
+    engine = create_db_engine(settings.dst_dsn)  # type: ignore
 
     # Create schema, if necessary.
     if settings.dst_schema:
         schema_name = settings.dst_schema
         if not engine.dialect.has_schema(engine, schema=schema_name):
             engine.execute(CreateSchema(schema_name, if_not_exists=True))
 
         # Recreate the engine, this time with a schema specified
-        engine = create_engine_with_search_path(
-            settings.dst_postgres_dsn, schema_name  # type: ignore
+        engine = create_db_engine(
+            settings.dst_dsn, schema_name=schema_name  # type: ignore
         )
 
     metadata.create_all(engine)
 
 
 def create_db_vocab(vocab_dict: Dict[str, Any]) -> None:
     """Load vocabulary tables from files."""
     settings = get_settings()
 
-    dst_engine = (
-        create_engine_with_search_path(
-            settings.dst_postgres_dsn, settings.dst_schema  # type: ignore
-        )
-        if settings.dst_schema
-        else create_engine(settings.dst_postgres_dsn)
+    dst_engine = create_db_engine(
+        settings.dst_dsn, schema_name=settings.dst_schema  # type: ignore
     )
 
     with dst_engine.connect() as dst_conn:
         for vocab_table in vocab_dict.values():
             try:
                 vocab_table.load(dst_conn)
             except IntegrityError:
@@ -59,20 +55,16 @@
     table_generator_dict: dict,
     story_generator_list: list,
     num_passes: int,
 ) -> None:
     """Connect to a database and populate it with data."""
     settings = get_settings()
 
-    dst_engine = (
-        create_engine_with_search_path(
-            settings.dst_postgres_dsn, settings.dst_schema  # type: ignore
-        )
-        if settings.dst_schema
-        else create_engine(settings.dst_postgres_dsn)
+    dst_engine = create_db_engine(
+        settings.dst_dsn, schema_name=settings.dst_schema  # type: ignore
     )
 
     with dst_engine.connect() as dst_conn:
         for _ in range(num_passes):
             populate(
                 dst_conn,
                 sorted_tables,
@@ -94,23 +86,24 @@
     # but we have to loop more manually to be able to use the `send` function.
     try:
         table_name, provided_values = next(story)
         while True:
             table = table_dict[table_name]
             if table.name in table_generator_dict:
                 table_generator = table_generator_dict[table.name]
-                default_values = table_generator(dst_conn).__dict__
+                default_values = table_generator(dst_conn)
             else:
                 default_values = {}
             insert_values = {**default_values, **provided_values}
             stmt = insert(table).values(insert_values)
             cursor = dst_conn.execute(stmt)
             # We need to return all the default values etc. to the generator,
             # because other parts of the story may refer to them.
-            final_values = {**insert_values, **dict(cursor.returned_defaults)}
+            return_values = dict(cursor.returned_defaults or {})
+            final_values = {**insert_values, **return_values}
             table_name, provided_values = story.send(final_values)
     except StopIteration:
         # The story has finished, it has no more rows to generate
         pass
 
 
 def populate(
@@ -143,9 +136,9 @@
             # We don't have a generator for this table, probably because it's a
             # vocabulary table.
             continue
         table_generator = table_generator_dict[table.name]
         # Run all the inserts for one table in a transaction
         with dst_conn.begin():
             for _ in range(table_generator.num_rows_per_pass):
-                stmt = insert(table).values(table_generator(dst_conn).__dict__)
+                stmt = insert(table).values(table_generator(dst_conn))
                 dst_conn.execute(stmt)
```

### Comparing `sqlsynthgen-0.2.0/sqlsynthgen/json_schemas/config_schema.json` & `sqlsynthgen-0.3.0/sqlsynthgen/json_schemas/config_schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880173294632524%*

 * *Differences: {"'properties'": "{'story_generators': {'items': {'properties': {'args': {'type': 'array'}, "*

 * *                 "'kwargs': OrderedDict([('type', 'object')])}}}, 'tables': {'patternProperties': "*

 * *                 "{'.*': {'properties': {'row_generators': {'items': {'properties': {'args': "*

 * *                 "{'type': 'array'}, 'kwargs': OrderedDict([('type', 'object')])}}}}}}}, "*

 * *                 "'max-unique-constraint-tries': OrderedDict([('type', 'integer')])}"}*

```diff
@@ -1,12 +1,15 @@
 {
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "description": "A SQLSynthGen configuration YAML file",
     "properties": {
+        "max-unique-constraint-tries": {
+            "type": "integer"
+        },
         "row_generators_module": {
             "type": "string"
         },
         "smartnoise-sql": {
             "patternProperties": {
                 ".*": {
                     "patternProperties": {
@@ -60,14 +63,17 @@
             "type": "array"
         },
         "story_generators": {
             "items": {
                 "additionalProperties": false,
                 "properties": {
                     "args": {
+                        "type": "array"
+                    },
+                    "kwargs": {
                         "type": "object"
                     },
                     "name": {
                         "type": "string"
                     },
                     "num_stories_per_pass": {
                         "type": "integer"
@@ -88,28 +94,28 @@
                         "num_rows_per_pass": {
                             "type": "integer"
                         },
                         "row_generators": {
                             "items": {
                                 "properties": {
                                     "args": {
-                                        "type": [
-                                            "object",
-                                            "null"
-                                        ]
+                                        "type": "array"
                                     },
                                     "columns_assigned": {
                                         "items": {
                                             "type": "string"
                                         },
                                         "type": [
                                             "array",
                                             "string"
                                         ]
                                     },
+                                    "kwargs": {
+                                        "type": "object"
+                                    },
                                     "name": {
                                         "type": "string"
                                     }
                                 },
                                 "type": "object"
                             },
                             "type": "array"
```

### Comparing `sqlsynthgen-0.2.0/sqlsynthgen/main.py` & `sqlsynthgen-0.3.0/sqlsynthgen/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,52 @@
 """Entrypoint for the SQLSynthGen package."""
+import asyncio
 import json
 import sys
 from pathlib import Path
 from types import ModuleType
 from typing import Final, Optional
 
 import typer
 import yaml
 from jsonschema.exceptions import ValidationError
 from jsonschema.validators import validate
 
 from sqlsynthgen.create import create_db_data, create_db_tables, create_db_vocab
 from sqlsynthgen.make import make_src_stats, make_table_generators, make_tables_file
-from sqlsynthgen.settings import get_settings
+from sqlsynthgen.remove import remove_db_data, remove_db_tables, remove_db_vocab
+from sqlsynthgen.settings import Settings, get_settings
 from sqlsynthgen.utils import import_file, read_yaml_file
 
 ORM_FILENAME: Final[str] = "orm.py"
 SSG_FILENAME: Final[str] = "ssg.py"
 STATS_FILENAME: Final[str] = "src-stats.yaml"
 CONFIG_SCHEMA_PATH: Final[Path] = (
     Path(__file__).parent / "json_schemas/config_schema.json"
 )
 
-app = typer.Typer()
+app = typer.Typer(no_args_is_help=True)
+
+
+def _check_file_non_existence(file_path: Path) -> None:
+    """Check that a given file does not exist. Exit with an error message if it does."""
+    if file_path.exists():
+        typer.echo(f"{file_path} should not already exist. Exiting...", err=True)
+        sys.exit(1)
+
+
+def _require_src_db_dsn(settings: Settings) -> str:
+    """Return the source DB DSN.
+
+    Check that source DB details have been set. Exit with error message if not.
+    """
+    if (src_dsn := settings.src_dsn) is None:
+        typer.echo("Missing source database connection details.", err=True)
+        sys.exit(1)
+    return src_dsn
 
 
 @app.command()
 def create_data(
     orm_file: str = typer.Option(ORM_FILENAME),
     ssg_file: str = typer.Option(SSG_FILENAME),
     num_passes: int = typer.Option(1),
@@ -81,16 +101,16 @@
     create_db_vocab(ssg_module.vocab_dict)
 
 
 @app.command()
 def create_tables(orm_file: str = typer.Option(ORM_FILENAME)) -> None:
     """Create schema from Python classes.
 
-    This CLI command creates Postgresql schema using object relational model
-    declared as Python tables. (eg.)
+    This CLI command creates the destination schema using object
+    relational model declared as Python tables.
 
     Example:
         $ sqlsynthgen create-tables
 
     Args:
         orm_file (str): Name of Python ORM file.
           Must be in the current working directory.
@@ -120,23 +140,19 @@
           Must be in the current working directory.
         ssg_file (str): Path to write the generators file to.
         config_file (str): Path to configuration file.
         stats_file (str): Path to source stats file (output of make-stats).
         force (bool): Overwrite the ORM file if exists. Default to False.
     """
     ssg_file_path = Path(ssg_file)
-    if ssg_file_path.exists() and not force:
-        typer.echo(f"{ssg_file} should not already exist. Exiting...", err=True)
-        sys.exit(1)
-
+    if not force:
+        _check_file_non_existence(ssg_file_path)
     settings = get_settings()
-    src_dsn = settings.src_postgres_dsn
-    if src_dsn is None:
-        typer.echo("Missing source database connection details.", err=True)
-        sys.exit(1)
+    # Check that src_dsn is set, even though we don't need it here.
+    _require_src_db_dsn(settings)
 
     orm_module: ModuleType = import_file(orm_file)
     generator_config = read_yaml_file(config_file) if config_file is not None else {}
     result: str = make_table_generators(
         orm_module, generator_config, stats_file, overwrite_files=force
     )
 
@@ -145,33 +161,33 @@
 
 @app.command()
 def make_stats(
     config_file: str = typer.Option(...),
     stats_file: str = typer.Option(STATS_FILENAME),
     force: bool = typer.Option(False, "--force", "-f"),
 ) -> None:
-    """Compute summary statistics from the source database, write them to a YAML file.
+    """Compute summary statistics from the source database.
+
+    Writes the statistics to a YAML file.
 
     Example:
         $ sqlsynthgen make_stats --config-file=example_config.yaml
     """
     stats_file_path = Path(stats_file)
-    if stats_file_path.exists() and not force:
-        typer.echo(f"{stats_file} should not already exist. Exiting...", err=True)
-        sys.exit(1)
+    if not force:
+        _check_file_non_existence(stats_file_path)
 
     config = read_yaml_file(config_file) if config_file is not None else {}
 
     settings = get_settings()
-    src_dsn = settings.src_postgres_dsn
-    if src_dsn is None:
-        typer.echo("Missing source database connection details.", err=True)
-        sys.exit(1)
+    src_dsn: str = _require_src_db_dsn(settings)
 
-    src_stats = make_src_stats(src_dsn, config)
+    src_stats = asyncio.get_event_loop().run_until_complete(
+        make_src_stats(src_dsn, config, settings.src_schema)
+    )
     stats_file_path.write_text(yaml.dump(src_stats), encoding="utf-8")
 
 
 @app.command()
 def make_tables(
     orm_file: str = typer.Option(ORM_FILENAME),
     force: bool = typer.Option(False, "--force", "-f"),
@@ -186,24 +202,19 @@
         $ sqlsynthgen make_tables
 
     Args:
         orm_file (str): Path to write the Python ORM file.
         force (bool): Overwrite ORM file, if exists. Default to False.
     """
     orm_file_path = Path(orm_file)
-    if orm_file_path.exists() and not force:
-        typer.echo(f"{orm_file} should not already exist. Exiting...", err=True)
-        sys.exit(1)
+    if not force:
+        _check_file_non_existence(orm_file_path)
 
     settings = get_settings()
-    if settings.src_postgres_dsn is None:
-        typer.echo("Missing source database connection details.", err=True)
-        sys.exit(1)
-
-    src_dsn = settings.src_postgres_dsn
+    src_dsn: str = _require_src_db_dsn(settings)
 
     content = make_tables_file(src_dsn, settings.src_schema)
     orm_file_path.write_text(content, encoding="utf-8")
 
 
 @app.command()
 def validate_config(config_file: Path) -> None:
@@ -213,9 +224,55 @@
     try:
         validate(config, schema_config)
     except ValidationError as e:
         typer.echo(e, err=True)
         sys.exit(1)
 
 
+@app.command()
+def remove_data(
+    orm_file: str = typer.Option(ORM_FILENAME),
+    ssg_file: str = typer.Option(SSG_FILENAME),
+    yes: bool = typer.Option(False, "--yes", prompt="Are you sure?"),
+) -> None:
+    """Truncate non-vocabulary tables in the destination schema."""
+    if yes:
+        orm_module = import_file(orm_file)
+        ssg_module = import_file(ssg_file)
+        remove_db_data(orm_module, ssg_module)
+    else:
+        typer.echo("Would truncate non-vocabulary tables if called with --yes")
+
+
+@app.command()
+def remove_vocab(
+    orm_file: str = typer.Option(ORM_FILENAME),
+    ssg_file: str = typer.Option(SSG_FILENAME),
+    yes: bool = typer.Option(False, "--yes", prompt="Are you sure?"),
+) -> None:
+    """Truncate vocabulary tables in the destination schema."""
+    if yes:
+        orm_module = import_file(orm_file)
+        ssg_module = import_file(ssg_file)
+        remove_db_vocab(orm_module, ssg_module)
+    else:
+        typer.echo("Would truncate vocabulary tables if called with --yes")
+
+
+@app.command()
+def remove_tables(
+    orm_file: str = typer.Option(ORM_FILENAME),
+    yes: bool = typer.Option(False, "--yes", prompt="Are you sure?"),
+) -> None:
+    """Drop all tables in the destination schema.
+
+    Does not drop the schema itself.
+    """
+    if yes:
+        orm_module = import_file(orm_file)
+        remove_db_tables(orm_module)
+    else:
+        typer.echo("Would remove tables if called with --yes")
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `sqlsynthgen-0.2.0/sqlsynthgen/providers.py` & `sqlsynthgen-0.3.0/sqlsynthgen/providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         min_dt: Any = dt.timedelta(seconds=0),
         # ints bigger than this cause trouble
         max_dt: Any = dt.timedelta(seconds=2**32),
     ) -> dt.timedelta:
         """Return a random timedelta object."""
         min_s = min_dt.total_seconds()
         max_s = max_dt.total_seconds()
-        seconds = random.randint(min_s, max_s)
+        seconds = random.randint(int(min_s), int(max_s))
         return dt.timedelta(seconds=seconds)
 
 
 class TimespanProvider(BaseProvider):
     """A Mimesis provider for timespans.
 
     A timespan consits of start datetime, end datetime, and the timedelta in between.
```

### Comparing `sqlsynthgen-0.2.0/sqlsynthgen/templates/ssg.py.j2` & `sqlsynthgen-0.3.0/sqlsynthgen/templates/ssg.py.j2`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This file was auto-generated by sqlsynthgen but can be edited manually."""
 from mimesis import Generic
 from mimesis.locales import Locale
 from sqlsynthgen.base import FileUploader
+from sqlsynthgen.unique_generator import UniqueGenerator
 
 generic = Generic(locale=Locale.EN_GB)
 
 {% for provider_import in provider_imports %}
 from sqlsynthgen.providers import {{ provider_import }}
 generic.add_provider({{ provider_import }})
 {% endfor %}
@@ -28,44 +29,57 @@
 {{ table_data.variable_name }} = FileUploader({{ tables_module.__name__ }}.{{ table_data.table_name }})
 {% endfor %}
 
 {% for table_data in tables %}
 class {{ table_data.class_name }}:
     num_rows_per_pass = {{ table_data.rows_per_pass }}
 
-    def __init__(self, dst_db_conn):
-    {% for column_data in table_data.columns %}
-        {% if column_data.primary_key %}
+    def __init__(self):
         pass
-        {% else %}
-        {{ column_data.variable_names}} = {{ column_data.generator_function }}({{ column_data.generator_arguments }})
+        {% for constraint in table_data.unique_constraints %}
+        self.unique_{{constraint.name}} = UniqueGenerator([
+                {% for col in constraint.columns %}
+                "{{col.name}}"{%- if not loop.last %}, {% endif %}
+                {% endfor %}
+            ],
+            "{{table_data.table_name}}",
+            {% if max_unique_constraint_tries is not none %}
+            max_tries={{max_unique_constraint_tries}},
+            {% endif %}
+        )
+        {% endfor %}
+
+    def __call__(self, dst_db_conn):
+        result = {}
+        {% for row_gen in table_data.row_gens %}
+        {% if not row_gen.primary_key %}
+        {% for vn in row_gen.variable_names %}
+        result["{{vn}}"]{%- if not loop.last %}, {% endif %}
+        {% endfor %} = {{ row_gen.function_call.function_name }}({{ row_gen.function_call.argument_values| join(", ") }})
         {% endif %}
-    {% endfor %}
+        {% endfor %}
+        return result
 {% endfor %}
 
 table_generator_dict = {
 {% for table_data in tables %}
-    "{{ table_data.table_name }}": {{ table_data.class_name }},
+    "{{ table_data.table_name }}": {{ table_data.class_name }}(),
 {% endfor %}
 }
 
 
 vocab_dict = {
 {% for table_data in vocabulary_tables %}
     "{{ table_data.dictionary_entry }}": {{ table_data.variable_name }},
 {% endfor %}
 }
 
 {% for gen_data in story_generators %}
 def {{ gen_data.wrapper_name }}(dst_db_conn):
-    return {{ gen_data.name }}(
-    {% for arg, val in gen_data["arguments"].items() %}
-        {{ arg }}={{ val }},
-    {% endfor %}
-    )
+    return {{ gen_data.function_call.function_name }}({{ gen_data.function_call.argument_values| join(", ") }})
 {% endfor %}
 
 story_generator_list = [
     {% for gen_data in story_generators %}
     {
         "name": {{ gen_data.wrapper_name }},
         "num_stories_per_pass": {{ gen_data.num_stories_per_pass }},
```

### Comparing `sqlsynthgen-0.2.0/sqlsynthgen/utils.py` & `sqlsynthgen-0.3.0/sqlsynthgen/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """Utility functions."""
 import os
 import sys
 from importlib import import_module
 from pathlib import Path
 from types import ModuleType
-from typing import Any
+from typing import Any, Optional
 
 import yaml
-from pydantic import PostgresDsn
 from sqlalchemy import create_engine, event, select
+from sqlalchemy.ext.asyncio import create_async_engine
 
 
 def read_yaml_file(path: str) -> Any:
     """Read a yaml file in to dictionary, given a path."""
     with open(path, "r", encoding="utf8") as f:
         config = yaml.safe_load(f)
     return config
 
 
-def import_file(file_name: str) -> ModuleType:
+def import_file(file_path: str) -> ModuleType:
     """Import a file.
 
-    This utility function returns file_name imported as a module.
+    This utility function returns file_path imported as a module.
 
     Args:
-        file_name (str): The name of a file in the current working directory.
+        file_path (str): The path of a file to import.
 
     Returns:
         ModuleType
     """
-    module_name = file_name[:-3]
+    module_name = os.path.splitext(os.path.basename(file_path))[0]
 
-    sys.path.append(os.getcwd())
+    sys.path.append(os.path.dirname(os.path.abspath(file_path)))
 
     try:
         module = import_module(module_name)
     finally:
         sys.path.pop()
 
     return module
@@ -47,29 +47,42 @@
     with engine.connect() as conn:
         result = [dict(row) for row in conn.execute(stmt)]
 
     with Path(yaml_file_name).open("w", newline="", encoding="utf-8") as yamlfile:
         yamlfile.write(yaml.dump(result))
 
 
-def create_engine_with_search_path(postgres_dsn: PostgresDsn, schema_name: str) -> Any:
-    """Create a SQLAlchemy Engine with an explicitly set schema."""
-    engine = create_engine(postgres_dsn)
-
-    @event.listens_for(engine, "connect", insert=True)
-    def connect(dbapi_connection: Any, _: Any) -> None:
-        set_search_path(dbapi_connection, schema_name)
+def create_db_engine(
+    db_dsn: str,
+    schema_name: Optional[str] = None,
+    use_asyncio: bool = False,
+    **kwargs: dict,
+) -> Any:
+    """Create a SQLAlchemy Engine."""
+    if use_asyncio:
+        async_dsn = db_dsn.replace("postgresql://", "postgresql+asyncpg://")
+        engine = create_async_engine(async_dsn, **kwargs)
+        event_engine = engine.sync_engine
+    else:
+        engine = create_engine(db_dsn, **kwargs)
+        event_engine = engine
+
+    if schema_name is not None:
+
+        @event.listens_for(event_engine, "connect", insert=True)
+        def connect(dbapi_connection: Any, _: Any) -> None:
+            set_search_path(dbapi_connection, schema_name)  # type: ignore
 
     return engine
 
 
 def set_search_path(connection: Any, schema: str) -> None:
     """Set the SEARCH_PATH for a PostgreSQL connection."""
     # https://docs.sqlalchemy.org/en/20/dialects/postgresql.html#remote-schema-table-introspection-and-postgresql-search-path
     existing_autocommit = connection.autocommit
     connection.autocommit = True
 
     cursor = connection.cursor()
-    cursor.execute(f'SET search_path to "{schema}";')
+    cursor.execute("SET search_path to %s;", (schema,))
     cursor.close()
 
     connection.autocommit = existing_autocommit
```

### Comparing `sqlsynthgen-0.2.0/PKG-INFO` & `sqlsynthgen-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: sqlsynthgen
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: Iain
 Author-email: 25081046+Iain-S@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: docs
+Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
+Requires-Dist: greenlet (>=2.0.2,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: mimesis (>=6.1.1,<7.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.2,<2.0.0)
+Requires-Dist: pymysql (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=5.0,<6.0)
 Requires-Dist: smartnoise-sql (>=0.2.11,<0.3.0)
 Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinxcontrib-napoleon (>=0.7,<0.8) ; extra == "docs"
 Requires-Dist: sqlacodegen (==3.0.0rc1)
-Requires-Dist: sqlalchemy (>=1.4,<2.0)
 Requires-Dist: sqlalchemy-utils (>=0.38.3,<0.39.0)
+Requires-Dist: sqlalchemy[asyncio] (>=1.4,<2.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # sqlsynthgen
 
 Synthetic data for SQL databases
```

