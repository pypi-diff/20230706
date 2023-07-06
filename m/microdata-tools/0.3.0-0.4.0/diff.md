# Comparing `tmp/microdata_tools-0.3.0.tar.gz` & `tmp/microdata_tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdata_tools-0.3.0.tar", max compression
+gzip compressed data, was "microdata_tools-0.4.0.tar", max compression
```

## Comparing `microdata_tools-0.3.0.tar` & `microdata_tools-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,31 @@
--rw-r--r--   0        0        0     1074 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     2238 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/README.md
--rw-r--r--   0        0        0      176 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/__init__.py
--rw-r--r--   0        0        0     5947 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/_decrypt.py
--rw-r--r--   0        0        0     4840 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/_encrypt.py
--rw-r--r--   0        0        0     1159 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/_utils.py
--rw-r--r--   0        0        0      193 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/exceptions.py
--rw-r--r--   0        0        0     2243 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/package_dataset.py
--rw-r--r--   0        0        0     2905 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/microdata_tools/unpackage_dataset.py
--rw-r--r--   0        0        0      534 2023-06-26 18:09:25.096910 microdata_tools-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 microdata_tools-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     2238 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/README.md
+-rw-r--r--   0        0        0      384 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/__init__.py
+-rw-r--r--   0        0        0     4372 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/packaging/__init__.py
+-rw-r--r--   0        0        0     6072 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/packaging/_decrypt.py
+-rw-r--r--   0        0        0     4950 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/packaging/_encrypt.py
+-rw-r--r--   0        0        0     1188 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/packaging/_utils.py
+-rw-r--r--   0        0        0      238 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/packaging/exceptions/__init__.py
+-rw-r--r--   0        0        0     5345 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/__init__.py
+-rw-r--r--   0        0        0     2557 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/adapter/local_storage.py
+-rw-r--r--   0        0        0     5776 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/temporal_attributes.py
+-rw-r--r--   0        0        0      757 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_id_types.py
+-rw-r--r--   0        0        0     1609 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json
+-rw-r--r--   0        0        0     2091 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/FAMILIE.json
+-rw-r--r--   0        0        0     1525 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/FORETAK.json
+-rw-r--r--   0        0        0     2124 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/HUSHOLDNING.json
+-rw-r--r--   0        0        0     1429 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/JOBB.json
+-rw-r--r--   0        0        0     1378 2023-07-06 13:22:03.687958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/KJORETOY.json
+-rw-r--r--   0        0        0   232471 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/KOMMUNE.json
+-rw-r--r--   0        0        0     1242 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/KURS.json
+-rw-r--r--   0        0        0     1202 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/PERSON.json
+-rw-r--r--   0        0        0     1535 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/VIRKSOMHET.json
+-rw-r--r--   0        0        0     1181 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/components/unit_type_variables/__init__.py
+-rw-r--r--   0        0        0      502 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/exceptions/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/model/__init__.py
+-rw-r--r--   0        0        0     5733 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/model/metadata.py
+-rw-r--r--   0        0        0     5278 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/steps/data_reader.py
+-rw-r--r--   0        0        0    12162 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/steps/dataset_validator.py
+-rw-r--r--   0        0        0     1652 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/microdata_tools/validation/steps/metadata_reader.py
+-rw-r--r--   0        0        0      603 2023-07-06 13:22:03.691958 microdata_tools-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 microdata_tools-0.4.0/PKG-INFO
```

### Comparing `microdata_tools-0.3.0/LICENSE.md` & `microdata_tools-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.3.0/README.md` & `microdata_tools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.3.0/microdata_tools/_decrypt.py` & `microdata_tools-0.4.0/microdata_tools/packaging/_decrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 from typing import List, Tuple
 
 from cryptography.fernet import Fernet, InvalidToken
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import padding
 
-from microdata_tools.exceptions import InvalidKeyError, InvalidTarFileContents
-from microdata_tools._utils import check_exists
+from microdata_tools.packaging.exceptions import (
+    InvalidKeyError,
+    InvalidTarFileContents,
+)
+from microdata_tools.packaging._utils import check_exists
 
 logger = logging.getLogger()
 
 
 def decrypt(rsa_keys_dir: Path, dataset_dir: Path, output_dir: Path):
     """
     Decrypts a dataset as follows:
@@ -38,15 +41,17 @@
 
     if not output_dataset_dir.exists():
         os.makedirs(output_dataset_dir)
 
     if chunk_dir.exists() and first_encrypted_chunk.exists():
         logger.info(f"Encrypted file found in {dataset_dir}")
 
-        with open(Path(rsa_keys_dir / "microdata_private_key.pem"), "rb") as key_file:
+        with open(
+            Path(rsa_keys_dir / "microdata_private_key.pem"), "rb"
+        ) as key_file:
             private_key = serialization.load_pem_private_key(
                 key_file.read(), password=None, backend=default_backend()
             )
 
         encrypted_symkey = Path(dataset_dir / f"{dataset_name}.symkey.encr")
         check_exists(encrypted_symkey)
 
@@ -94,15 +99,17 @@
 
         # Remove decrypted chunks
         shutil.rmtree(decrypted_dir)
 
     _copy_metadata_file(dataset_dir, dataset_name, output_dataset_dir)
 
 
-def _copy_decrypted_data_to_output_dir(dataset_dir, dataset_name, output_dataset_dir):
+def _copy_decrypted_data_to_output_dir(
+    dataset_dir, dataset_name, output_dataset_dir
+):
     data_file_path = dataset_dir / f"{dataset_name}.csv"
     shutil.copy(
         data_file_path,
         output_dataset_dir / f"{dataset_name}.csv",
     )
     os.remove(data_file_path)
 
@@ -112,15 +119,17 @@
     shutil.copy(
         metadata_file_path,
         output_dataset_dir / f"{dataset_name}.json",
     )
     os.remove(metadata_file_path)
 
 
-def untar_encrypted_dataset(input_file: Path, dataset_name: str, untar_dir: Path):
+def untar_encrypted_dataset(
+    input_file: Path, dataset_name: str, untar_dir: Path
+):
     with tarfile.open(input_file) as tar:
         _validate_tar_contents(tar.getnames(), dataset_name)
         tar.extractall(path=untar_dir)
 
 
 def _validate_tar_contents(files: List[str], dataset_name: str) -> None:
     if f"{dataset_name}.json" not in files:
@@ -145,23 +154,29 @@
                 f"Tar file for {dataset_name} does not contain the required "
                 f"{dataset_name}.md5 file"
             )
 
 
 def _combine_csv_files(input_dir: Path, output_file: Path) -> None:
     sorted_chunkpaths = _get_sorted_file_names(input_dir)
-    logger.debug(f"\nCombining {len(sorted_chunkpaths)} files into {output_file}")
+    logger.debug(
+        f"\nCombining {len(sorted_chunkpaths)} files into {output_file}"
+    )
 
     with open(output_file, "wb") as combined_file:
         for chunk_number, file_name in sorted_chunkpaths:
             with open(file_name, "rb") as chunk_file:
                 chunk_data = chunk_file.read()
                 combined_file.write(chunk_data)
 
 
 # Turn files_names in input dir into a dictionary with the chunk number as key
 # Then return the sorted dictionary
 def _get_sorted_file_names(directory: Path) -> List[Tuple]:
     try:
-        return sorted([(int(f.stem), f) for f in directory.iterdir() if f.is_file()])
+        return sorted(
+            [(int(f.stem), f) for f in directory.iterdir() if f.is_file()]
+        )
     except ValueError as e:
-        raise InvalidTarFileContents("Failed to sort files in chunk directory ") from e
+        raise InvalidTarFileContents(
+            "Failed to sort files in chunk directory "
+        ) from e
```

### Comparing `microdata_tools-0.3.0/microdata_tools/_encrypt.py` & `microdata_tools-0.4.0/microdata_tools/packaging/_encrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import padding
 
-from microdata_tools.exceptions import ValidationException
-from microdata_tools._utils import check_exists
+from microdata_tools.packaging.exceptions import ValidationException
+from microdata_tools.packaging._utils import check_exists
 
 logger = logging.getLogger()
 
 CHUNK_SIZE_BYTES = 250_000_000  # 250 MB per chunk
 
 
 def encrypt_dataset(
@@ -42,15 +42,17 @@
 
     # Read public key from file
     with open(public_key_location, "rb") as key_file:
         public_key = serialization.load_pem_public_key(
             key_file.read(), backend=default_backend()
         )
 
-    csv_files = [file for file in dataset_dir.iterdir() if file.suffix == ".csv"]
+    csv_files = [
+        file for file in dataset_dir.iterdir() if file.suffix == ".csv"
+    ]
 
     csv_file = csv_files[0]
     dataset_name = csv_file.stem
 
     if dataset_name != dataset_dir.stem:
         raise ValidationException(
             f"The csv file name {dataset_name} should match "
@@ -76,15 +78,17 @@
             data = file.read(CHUNK_SIZE_BYTES)
             if not data:
                 break
 
             chunk_count += 1
             encrypted = fernet.encrypt(data)
 
-            chunk_file = dataset_output_dir / "chunks" / f"{chunk_count}.csv.encr"
+            chunk_file = (
+                dataset_output_dir / "chunks" / f"{chunk_count}.csv.encr"
+            )
             with open(chunk_file, "wb") as chunk_output:
                 chunk_output.write(encrypted)
 
     logger.debug(f"Csv file {csv_file} encrypted into {chunk_count} chunks")
 
     encrypted_sym_key = public_key.encrypt(
         symkey,
@@ -95,15 +99,17 @@
         ),
     )
 
     # Store encrypted symkey to file
     with open(encrypted_symkey_file, "wb") as file:
         file.write(encrypted_sym_key)
 
-    logger.debug(f"Key file for {csv_file} encrypted into {encrypted_symkey_file}")
+    logger.debug(
+        f"Key file for {csv_file} encrypted into {encrypted_symkey_file}"
+    )
 
 
 def _tar_encrypted_dataset(input_dir: Path, dataset_name: str) -> None:
     """
     Creates a tar file from encrypted dataset files.
     Removes the input directory after successful completion.
     :param input_dir: the input directory containing the dataset directory
@@ -130,15 +136,17 @@
     if chunk_dir.exists():
         chunk_files = [file for file in chunk_dir.iterdir()]
         if len(chunk_files) == 0:
             raise ValidationException(f"No files found in {chunk_dir}")
 
         md5_file = dataset_dir / f"{dataset_name}.md5"
         if not md5_file.exists():
-            raise ValidationException(f"The required file {md5_file} is missing")
+            raise ValidationException(
+                f"The required file {md5_file} is missing"
+            )
 
         files_to_tar.extend(
             [
                 dataset_dir / f"{dataset_name}.symkey.encr",
                 dataset_dir / f"{dataset_name}.md5",
             ]
         )
```

### Comparing `microdata_tools-0.3.0/microdata_tools/_utils.py` & `microdata_tools-0.4.0/microdata_tools/packaging/_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from pathlib import Path
 import hashlib
-from microdata_tools.exceptions import ValidationException, CsvConsistencyException
+from microdata_tools.packaging.exceptions import (
+    ValidationException,
+    CsvConsistencyException,
+)
 
 
 def check_exists(path: Path):
     if not path.exists():
         raise ValidationException(f"The path {path} does not exist")
 
 
@@ -23,14 +26,16 @@
 
 def write_checksum_to_file(csv_file: Path) -> None:
     hash_file = str(csv_file).replace(".csv", ".md5")
     with open(hash_file, "w") as file:
         file.write(calculate_checksum(csv_file))
 
 
-def compare_checksum_with_file(md5_file: Path, calculated_checksum: str) -> None:
+def compare_checksum_with_file(
+    md5_file: Path, calculated_checksum: str
+) -> None:
     with open(md5_file, "r") as file:
         checksum_from_file = file.readlines()[0]
         if calculated_checksum != checksum_from_file.strip():
             raise CsvConsistencyException(
                 "MD5 checksums do not match. The csv file may be corrupted!"
             )
```

### Comparing `microdata_tools-0.3.0/microdata_tools/unpackage_dataset.py` & `microdata_tools-0.4.0/microdata_tools/packaging/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,110 @@
 import logging
 import os
-from pathlib import Path
 import shutil
-from typing import Union
-from microdata_tools._utils import (
+from pathlib import Path
+
+from microdata_tools.packaging._encrypt import (
+    _tar_encrypted_dataset,
+    encrypt_dataset,
+)
+from microdata_tools.packaging.exceptions import (
+    UnpackagingError,
+    ValidationException,
+)
+from microdata_tools.packaging._decrypt import decrypt, untar_encrypted_dataset
+from microdata_tools.packaging._utils import (
     check_exists,
+    write_checksum_to_file,
     compare_checksum_with_file,
     calculate_checksum,
 )
-from microdata_tools._decrypt import decrypt, untar_encrypted_dataset
+
 
 logger = logging.getLogger()
 
 
+def package_dataset(
+    rsa_keys_dir: Path, dataset_dir: Path, output_dir: Path
+) -> None:
+    """
+    Packages a dataset. It will encrypt and tar the dataset using
+    the provided RSA public key. Only the CSV file will be encrypted.
+    Creates a checksum file for the CSV file.
+
+    :param rsa_keys_dir:
+        directory containing public key file microdata_public_key.pem
+    :param dataset_dir:
+        directory containing the dataset files (CSV and JSON)
+    :param output_dir:
+        output directory
+    :return:
+        None
+    """
+
+    dataset_name = dataset_dir.stem
+    dataset_output_dir = output_dir / dataset_name
+    csv_files = [
+        file for file in dataset_dir.iterdir() if file.suffix == ".csv"
+    ]
+
+    try:
+        # check if json exists
+        check_exists(dataset_dir / f"{dataset_name}.json")
+
+        # Validate that there is only one csv file
+        if len(csv_files) > 1:
+            raise ValidationException(
+                f"There should only be one csv file in {dataset_dir}"
+            )
+
+        if len(csv_files) == 1:
+            write_checksum_to_file(csv_files[0])
+            encrypt_dataset(
+                rsa_keys_dir=rsa_keys_dir,
+                dataset_dir=dataset_dir,
+                output_dir=output_dir,
+            )
+        else:
+            if not dataset_output_dir.exists():
+                os.makedirs(dataset_output_dir)
+
+        if Path(dataset_dir / f"{dataset_name}.md5").exists():
+            shutil.copyfile(
+                dataset_dir / f"{dataset_name}.md5",
+                dataset_output_dir / f"{dataset_name}.md5",
+            )
+
+        shutil.copyfile(
+            dataset_dir / f"{dataset_name}.json",
+            dataset_output_dir / f"{dataset_name}.json",
+        )
+        _tar_encrypted_dataset(input_dir=output_dir, dataset_name=dataset_name)
+
+    except Exception as exe:
+        logger.error(f"Failed to package dataset {dataset_name}: {exe}")
+        raise exe
+
+
 def unpackage_dataset(
     packaged_file_path: Path,
     rsa_keys_dir: Path,
     output_dir: Path,
-    archive_dir: Union[Path, None],
 ) -> None:
     """
     Unpackages a dataset. It will untar and decrypt the dataset using
     the provided RSA private key. Only the CSV file will be decrypted.
     Validates the checksum of the CSV file.
 
     :param packaged_file_path:
         a Path to the .tar file containing the dataset files
     :param rsa_keys_dir:
         directory containing the private key file microdata_private_key.pem
     :param output_dir:
         output directory
-    :param archive_dir:
-        optional archive directory where the .tar file will be moved
     :return:
         None
     """
     check_exists(packaged_file_path)
     check_exists(rsa_keys_dir)
 
     if not output_dir.exists():
@@ -48,43 +117,25 @@
     dataset_dir = packaged_file_path.parent / dataset_name
     logger.info(f"Unpackaging {packaged_file_path}")
 
     try:
         untar_encrypted_dataset(packaged_file_path, dataset_name, dataset_dir)
         decrypt(rsa_keys_dir, dataset_dir, output_dir)
         _validate_csv_consistency(dataset_name, dataset_dir, output_dir)
-        if archive_dir is not None:
-            _archive(dataset_name, dataset_dir.parent, archive_dir, "unpackaged")
+
+        if Path(dataset_dir).exists():
+            shutil.rmtree(dataset_dir)
+
         logger.info(f"Unpackaged {packaged_file_path}")
     except Exception as exc:
-        if archive_dir is not None:
-            _archive(dataset_name, dataset_dir.parent, archive_dir, "failed")
         logger.exception(f"Failed to unpackage {dataset_name}", exc_info=exc)
+        raise UnpackagingError("Failed to unpackage dataset") from exc
 
 
 def _validate_csv_consistency(dataset_name, dataset_dir, output_dir):
     if Path(output_dir / dataset_name / f"{dataset_name}.csv").exists():
         calculated_checksum = calculate_checksum(
             output_dir / dataset_name / f"{dataset_name}.csv"
         )
         compare_checksum_with_file(
             dataset_dir / f"{dataset_name}.md5", calculated_checksum
         )
-
-
-def _archive(
-    dataset_name: str, input_dir: Path, archive_dir: Path, sub_dir: str
-) -> None:
-    archive_sub_dir = archive_dir / sub_dir
-
-    if not archive_sub_dir.exists():
-        os.makedirs(archive_sub_dir)
-
-    shutil.move(
-        input_dir / f"{dataset_name}.tar",
-        archive_sub_dir / f"{dataset_name}.tar",
-    )
-
-    if Path(input_dir / dataset_name).exists():
-        shutil.rmtree(input_dir / dataset_name)
-
-    logger.debug(f"Archived files for {dataset_name} in {archive_sub_dir}")
```

### Comparing `microdata_tools-0.3.0/pyproject.toml` & `microdata_tools-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [tool.poetry]
 name = "microdata-tools"
-version = "0.3.0"
+version = "0.4.0"
 description = "Tools for the microdata.no platform"
 authors = ["microdata-developers"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "microdata_tools"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<4.0"
 cryptography = "^41.0.1"
+pydantic = "^1.10.9"
+pyarrow = "^12.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.272"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 cryptography = "^41.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length=79
```

### Comparing `microdata_tools-0.3.0/PKG-INFO` & `microdata_tools-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: microdata-tools
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tools for the microdata.no platform
 License: MIT
 Author: microdata-developers
 Requires-Python: >=3.7.2,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=41.0.1,<42.0.0)
+Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Description-Content-Type: text/markdown
 
 # microdata-tools
 Tools for the [microdata.no](https://www.microdata.no/) platform
 
 ## Installation
 `microdata-tools` can be installed from PyPI using pip:
```

