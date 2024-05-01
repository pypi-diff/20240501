# Comparing `tmp/vault_fix-1.3.3.tar.gz` & `tmp/vault_fix-1.4.0.tar.gz`

## Comparing `vault_fix-1.3.3.tar` & `vault_fix-1.4.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 vault_fix-1.3.3/.python-version
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/__init__.py
--rw-r--r--   0        0        0     8299 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/__main__.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/_log.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/_type.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/dump.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/load.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/_crypto/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/_crypto/constants.py
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/_crypto/message.py
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/_crypto/symmetric.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/serializers/__init__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/serializers/json.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 vault_fix-1.3.3/src/vault_fix/serializers/yaml.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/__init__.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/integration/__init__.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/integration/test_dump.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/integration/test_load.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/integration/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/unit/__init__.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/unit/fixtures.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/unit/test_aux.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/unit/test_dump.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/unit/test_load.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/unit/test_logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/unit/crypto/__init__.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/unit/crypto/test_message.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 vault_fix-1.3.3/tests/unit/crypto/test_symmetric.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 vault_fix-1.3.3/.gitignore
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 vault_fix-1.3.3/LICENSE.txt
--rw-r--r--   0        0        0    13811 2020-02-02 00:00:00.000000 vault_fix-1.3.3/README.md
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 vault_fix-1.3.3/pyproject.toml
--rw-r--r--   0        0        0    15978 2020-02-02 00:00:00.000000 vault_fix-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 vault_fix-1.4.0/.python-version
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/__init__.py
+-rw-r--r--   0        0        0     8299 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/__main__.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/_log.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/dump.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/load.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/_crypto/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/_crypto/constants.py
+-rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/_crypto/message.py
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/_crypto/symmetric.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/serializers/__init__.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/serializers/json.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 vault_fix-1.4.0/src/vault_fix/serializers/yaml.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/integration/test_dump.py
+-rw-r--r--   0        0        0     7024 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/integration/test_load.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/integration/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/unit/fixtures.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/unit/test_aux.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/unit/test_dump.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/unit/test_load.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/unit/test_logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/unit/crypto/__init__.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/unit/crypto/test_message.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 vault_fix-1.4.0/tests/unit/crypto/test_symmetric.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 vault_fix-1.4.0/.gitignore
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 vault_fix-1.4.0/LICENSE.txt
+-rw-r--r--   0        0        0    13810 2020-02-02 00:00:00.000000 vault_fix-1.4.0/README.md
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 vault_fix-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 vault_fix-1.4.0/PKG-INFO
```

### Comparing `vault_fix-1.3.3/src/vault_fix/__main__.py` & `vault_fix-1.4.0/src/vault_fix/__main__.py`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/src/vault_fix/_log.py` & `vault_fix-1.4.0/src/vault_fix/_log.py`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/src/vault_fix/dump.py` & `vault_fix-1.4.0/src/vault_fix/dump.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from typing import Callable, TextIO, Union
+from typing import Any, Callable, TextIO, Union
 
 import hvac
 
 from vault_fix._crypto import encrypt_fixture_data
 from vault_fix._crypto.symmetric import SymmetricCrypto
-from vault_fix._type import NestedStrDict
 
 
 def dump_to_fixture_file(
     *,
     hvac: hvac.Client,
     fixture: TextIO,
     mount_point,
-    serializer: Callable[[NestedStrDict], str],
+    serializer: Callable[[dict[str, Any]], str],
     path: str = "/",
     password: Union[str, None] = None,
     dry_run: bool = False,
 ):
     fixture_data = dump(
         hvac=hvac,
         mount_point=mount_point,
@@ -30,33 +29,33 @@
         if p:
             fixture_data = {f"{p}/": fixture_data}
 
     if not dry_run:
         fixture.write(serializer(fixture_data))
 
 
-def dump(*, hvac: hvac.Client, mount_point: str, path: str) -> NestedStrDict:
+def dump(*, hvac: hvac.Client, mount_point: str, path: str) -> dict[str, Any]:
     """
     Dump all secrets in the hierarchy under ``path`` to a dict.
 
     NOTE: This method is relatively slow because it recursively discovers secrets data from Vault.
 
     :param hvac: Initialised hvac.Client object.
     :param mount_point: The mount_point in Vault where the secrets are stored.
     :param path: The path in Vault where the secrets are stored.
     :returns: Dictionary of secrets under ``{mount_point}/{path}``.
     """
     key: str
-    result: NestedStrDict = dict()
+    result = {}
 
     vault = hvac.secrets.kv.v2
-
+    path = path.strip("/")
     keys = vault.list_secrets(path=path, mount_point=mount_point).get("data", {}).get("keys", [])
 
     for key in keys:
         if key.endswith("/"):
             result[key] = dump(hvac=hvac, path=f"{path}/{key}", mount_point=mount_point)
         else:
-            data = vault.read_secret_version(path=f"{path}{key}", mount_point=mount_point)
+            data = vault.read_secret_version(path=f"{path}/{key}", mount_point=mount_point)
             result[key] = data.get("data", {}).get("data", {})
 
     return result
```

### Comparing `vault_fix-1.3.3/src/vault_fix/load.py` & `vault_fix-1.4.0/src/vault_fix/load.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-from typing import Callable, Generator, TextIO, Union
+from typing import Any, Callable, Generator, TextIO, Union
 
 import hvac
 
 from vault_fix._crypto import decrypt_fixture_data
 from vault_fix._crypto.symmetric import SymmetricCrypto
-from vault_fix._type import NestedStrDict
 
 
 def load_fixture_from_file(
     *,
     hvac: hvac.Client,
     fixture: TextIO,
     mount_point,
-    deserializer: Callable[[TextIO], NestedStrDict],
+    deserializer: Callable[[TextIO], dict[str, Any]],
     path: str = "/",
     password: Union[str, None] = None,
     dry_run: bool = False,
 ) -> None:
     fixture_data = deserializer(fixture)
     if password:
         cipher = SymmetricCrypto(password)
         fixture_data = decrypt_fixture_data(fixture_data, cipher)
     load(hvac=hvac, fixture=fixture_data, mount_point=mount_point, path=path, dry_run=dry_run)
 
 
-def load(*, hvac: hvac.Client, fixture: dict, mount_point: str, path: str, dry_run: bool = False) -> None:
+def load(*, hvac: hvac.Client, fixture: dict[str, Any], mount_point: str, path: str, dry_run: bool = False) -> None:
     """
     Imports a fixture from a dict.
 
     Format should be::
 
         {
             "some/": {
@@ -56,16 +55,16 @@
         if isinstance(secrets, str) and secrets.startswith("encrypted//"):
             raise RuntimeError("Fixture file is encrypted but not password was passed.")
         if not dry_run:
             hvac.secrets.kv.v2.create_or_update_secret(path=_path, secret=secrets, mount_point=mount_point)
 
 
 def _fixture_deserialize(
-    *, data: dict, parent: str = "/"
-) -> Generator[tuple[str, Union[str, NestedStrDict]], None, None]:
+    *, data: dict[str, Any], parent: str = "/"
+) -> Generator[tuple[str, Union[str, dict[str, Any]]], None, None]:
     """
     Changes a dictionary to a generator of tuples with paths as the first entry and secrets data as the second.
 
     This works only for structures that have a `/` in keys that are part of the path.
 
     This is meant to "deserialize" fixtures with a hierarchical structure to a flatter structure, that can be used in
     calls to the Vault API.
```

### Comparing `vault_fix-1.3.3/src/vault_fix/_crypto/__init__.py` & `vault_fix-1.4.0/src/vault_fix/_crypto/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
+from typing import Any
 
 from vault_fix._crypto.symmetric import SymmetricCrypto
-from vault_fix._type import NestedStrDict
 
 
-def decrypt_fixture_data(vaultFixture: dict, cipher: SymmetricCrypto) -> NestedStrDict:
+def decrypt_fixture_data(vaultFixture: dict[str, Any], cipher: SymmetricCrypto) -> dict[str, Any]:
     for path, data in vaultFixture.items():
         if path.endswith("/"):
             vaultFixture[path] = decrypt_fixture_data(data, cipher)
         else:
             vaultFixture[path] = json.loads(cipher.decrypt(data[11:]))
     return vaultFixture
 
 
-def encrypt_fixture_data(vaultFixture: dict, cipher: SymmetricCrypto) -> NestedStrDict:
+def encrypt_fixture_data(vaultFixture: dict[str, Any], cipher: SymmetricCrypto) -> dict[str, Any]:
     for path, data in vaultFixture.items():
         if path.endswith("/"):
             vaultFixture[path] = encrypt_fixture_data(data, cipher)
         else:
             vaultFixture[path] = f"encrypted//{cipher.encrypt(json.dumps(data, indent=None))}"
     return vaultFixture
```

### Comparing `vault_fix-1.3.3/src/vault_fix/_crypto/constants.py` & `vault_fix-1.4.0/src/vault_fix/_crypto/constants.py`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/src/vault_fix/_crypto/message.py` & `vault_fix-1.4.0/src/vault_fix/_crypto/message.py`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/src/vault_fix/_crypto/symmetric.py` & `vault_fix-1.4.0/src/vault_fix/_crypto/symmetric.py`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/tests/conftest.py` & `vault_fix-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/tests/integration/test_dump.py` & `vault_fix-1.4.0/tests/integration/test_dump.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import functools
-from typing import Callable
+from typing import Any, Callable
 from unittest import mock
 
 import hvac
 import pytest
 from typer.testing import CliRunner
 from vault_fix.__main__ import cli
-from vault_fix._type import NestedStrDict
 from vault_fix.serializers.json import json_serializer
 from vault_fix.serializers.yaml import yaml_serializer
 
 from tests.unit.fixtures import DUMPED_DATA_ENCRYPTED, DUMPED_DATA_PLAIN
 
 runner = CliRunner(mix_stderr=False)
 
@@ -31,16 +30,16 @@
     ],
 )
 def test_dump_to_fixture_file_cli(
     mock_hvac: hvac.Client,
     mock_urandom: mock.Mock,
     serializer_args: list[str],
     password_args: list[str],
-    serializer: Callable[[NestedStrDict], str],
-    expected: NestedStrDict,
+    serializer: Callable[[dict[str, Any]], str],
+    expected: dict[str, Any],
 ) -> None:
     with mock.patch("vault_fix.__main__._get_hvac_client", return_value=mock_hvac):
         args = ["dump", "secret", "/", *serializer_args, *password_args, "-t", "root"]
         result = runner.invoke(cli, args=args)
     assert result.exit_code == 0
     assert result.stdout == serializer(expected)
 
@@ -53,15 +52,15 @@
     mock_hvac.secrets.kv.v2.read_secret_version.side_effect = [
         {"data": {"data": {"pop-up-secret": "close-button-doesnt-work"}}},
     ]
     with mock.patch("vault_fix.__main__._get_hvac_client", return_value=mock_hvac):
         args = ["dump", "secret", "10-things-they-dont-want-you-to-know/advertisement/", "-t", "root"]
         result = runner.invoke(cli, args=args)
         mock_hvac.secrets.kv.v2.list_secrets.assert_called_once_with(
-            path="10-things-they-dont-want-you-to-know/advertisement/",
+            path="10-things-they-dont-want-you-to-know/advertisement",
             mount_point="secret",
         )
         mock_hvac.secrets.kv.v2.read_secret_version.assert_called_once_with(
             path="10-things-they-dont-want-you-to-know/advertisement/annoying-popup-secret",
             mount_point="secret",
         )
     assert result.exit_code == 0
```

### Comparing `vault_fix-1.3.3/tests/integration/test_load.py` & `vault_fix-1.4.0/tests/integration/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,33 +118,31 @@
                 mount_point="secret",
             ),
         ]
     )
 
 
 @pytest.mark.parametrize(
-    "deserializer_args, password_args, stdin_data",
+    "deserializer_args, stdin_data",
     [
-        pytest.param(["--deserializer", "json"], [], JSON_DUMPED_PLAIN, id="JSON-plain"),
-        pytest.param(["--deserializer", "yaml"], [], YAML_DUMPED_PLAIN, id="YAML-plain"),
+        pytest.param(["--deserializer", "json"], JSON_DUMPED_PLAIN, id="JSON-plain"),
+        pytest.param(["--deserializer", "yaml"], YAML_DUMPED_PLAIN, id="YAML-plain"),
     ],
 )
 def test_load_from_fixture_stdin_cli_path(
     mock_hvac: hvac.Client,
     deserializer_args: list[str],
-    password_args: list[str],
     stdin_data: str,
 ) -> None:
     with mock.patch("vault_fix.__main__._get_hvac_client", return_value=mock_hvac):
         args = [
             "load",
             "secret",
             "/10-things-they-dont-want-you-to-know/advertisement",
             *deserializer_args,
-            *password_args,
             "-t",
             "root",
         ]
         result = runner.invoke(cli, args=args, input=stdin_data)
     assert result.exit_code == 0
     assert mock_hvac.secrets.kv.v2.create_or_update_secret.call_count == 1
     mock_hvac.secrets.kv.v2.create_or_update_secret.assert_has_calls(
```

### Comparing `vault_fix-1.3.3/tests/unit/fixtures.py` & `vault_fix-1.4.0/tests/unit/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from vault_fix._type import NestedStrDict
 from vault_fix.serializers.json import json_serializer
 from vault_fix.serializers.yaml import yaml_serializer
 
 PASSWORD = "hunter2"
 SECRET_MESSAGE = "Some day this will be replaced by my lattice-based crypto"
 ENCRYPTED_SECRET_MESSAGE = (
     "AgCBEAEAAABTU1NTU1NTU1NTU1NTU1NTTk5OTk5OTk5OTk5OFEwDr/XfJIqIcrX6qrFIS/Kmgf"
     "KRMfYpJhtGLjCIT6YwKY4RRMrvT93JqJ0qb9mBkpWlGyeAi7pBB64RvbYg/584d+fgkNEvtQ=="
 )
-DUMPED_DATA_PLAIN: NestedStrDict = {
+DUMPED_DATA_PLAIN = {
     "10-things-they-dont-want-you-to-know/": {
         "advertisement/": {"annoying-popup-secret": {"pop-up-secret": "close-button-doesnt-work"}},
         "something-you-already-know/": {"secret-things-you-already-know": {"you-know-this": "click-bait-is-lame"}},
     }
 }
-DUMPED_DATA_ENCRYPTED: NestedStrDict = {
+
+DUMPED_DATA_ENCRYPTED = {
     "10-things-they-dont-want-you-to-know/": {
         "advertisement/": {
             "annoying-popup-secret": (
                 "encrypted//AgCBEADiBABTU1NTU1NTU1NTU1NTU1NTTk5OTk5OTk5OTk5OkGqg20Csh9zRs0iFnFmRDDH/gkBbWnbnD0bfYUd9YP2"
                 "e1yjW4oPbYxnCFSGVKum9P5aYLdEUtpQ6WfJpOQ=="
             )
         },
```

### Comparing `vault_fix-1.3.3/tests/unit/test_aux.py` & `vault_fix-1.4.0/tests/unit/test_aux.py`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/tests/unit/test_dump.py` & `vault_fix-1.4.0/tests/unit/test_dump.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import functools
 import io
-from typing import Callable
+from typing import Any, Callable
 from unittest import mock
 
 import hvac
 import pytest
-from vault_fix._type import NestedStrDict
 from vault_fix.dump import dump, dump_to_fixture_file
 from vault_fix.serializers.json import json_serializer
 from vault_fix.serializers.yaml import yaml_serializer
 
 from tests.unit.fixtures import DUMPED_DATA_ENCRYPTED, DUMPED_DATA_PLAIN
 
 
@@ -32,22 +31,59 @@
         pytest.param("donttellanyone", DUMPED_DATA_ENCRYPTED, id="encrypted"),
         pytest.param(None, DUMPED_DATA_PLAIN, id="plain"),
     ],
 )
 def test_dump_to_fixture_file(
     mock_hvac: hvac.Client,
     mock_urandom: mock.Mock,
-    serializer: Callable[[NestedStrDict], str],
+    serializer: Callable[[dict[str, Any]], str],
     password: str,
-    expected: NestedStrDict,
+    expected: dict[str, Any],
 ) -> None:
     data = io.StringIO()
     dump_to_fixture_file(
         hvac=mock_hvac,
         fixture=data,
         mount_point="secret",
         path="/",
         serializer=serializer,
         password=password,
     )
     data.seek(0)
     assert data.read() == serializer(expected)
+
+
+@pytest.mark.parametrize(
+    "path",
+    [
+        pytest.param("10-things-they-dont-want-you-to-know/advertisement", id="slash-no-prefix+no-suffix"),
+        pytest.param("/10-things-they-dont-want-you-to-know/advertisement", id="slash-prefix+no-suffix"),
+        pytest.param("/10-things-they-dont-want-you-to-know/advertisement/", id="slash-prefix+suffix"),
+        pytest.param("10-things-they-dont-want-you-to-know/advertisement/", id="slash-no-prefix+suffix"),
+    ],
+)
+def test_dump_from_fixture_path(path: str) -> None:
+    mock_hvac = mock.Mock(spec=hvac.Client)
+    mock_hvac.secrets.kv.v2.list_secrets.side_effect = [
+        {"data": {"keys": ["annoying-popup-secret"]}},
+    ]
+    mock_hvac.secrets.kv.v2.read_secret_version.side_effect = [
+        {"data": {"data": {"pop-up-secret": "close-button-doesnt-work"}}},
+    ]
+    data = io.StringIO()
+    with mock.patch("vault_fix.__main__._get_hvac_client", return_value=mock_hvac):
+        dump_to_fixture_file(
+            hvac=mock_hvac,
+            fixture=data,
+            mount_point="secret",
+            path=path,
+            serializer=yaml_serializer,
+            password=None,
+        )
+    mock_hvac.secrets.kv.v2.list_secrets.assert_called_once_with(
+        path="10-things-they-dont-want-you-to-know/advertisement",
+        mount_point="secret",
+    )
+    mock_hvac.secrets.kv.v2.read_secret_version.assert_called_once_with(
+        path="10-things-they-dont-want-you-to-know/advertisement/annoying-popup-secret",
+        mount_point="secret",
+    )
```

### Comparing `vault_fix-1.3.3/tests/unit/test_logging.py` & `vault_fix-1.4.0/tests/unit/test_logging.py`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/tests/unit/crypto/test_message.py` & `vault_fix-1.4.0/tests/unit/crypto/test_message.py`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/tests/unit/crypto/test_symmetric.py` & `vault_fix-1.4.0/tests/unit/crypto/test_symmetric.py`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/.gitignore` & `vault_fix-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/LICENSE.txt` & `vault_fix-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vault_fix-1.3.3/README.md` & `vault_fix-1.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Vault-fix
 
 vault-fix is a CLI utility and python package that helps exporting and importing secrets to and from [Vault] instances.
-You can use this either to load fixture files for local development (it's original purpose). Or to migrate data from
+You can use this either to load fixture files for local development (its original purpose). Or to migrate data from
 Vault instance to another, while secrets may be [encrypted](#Encrypting-output) and/or
 [piped to another vault-fix instance](#Directing-data-to-the-load-command) so the data is not persisted.
 
 ## Historical context
 
 vault-fix was created to address an issue with the default mode of [Vault instances in dev mode], for local development.
 Vault will start with ephemeral storage, i.e. in-memory, mounting a volume will not make it persistent. If you want to
```

### Comparing `vault_fix-1.3.3/pyproject.toml` & `vault_fix-1.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 description = "Tool for importing and exporting vault fixture files to and from vault dev mode instances."
 license = { file = "LICENSE.txt" }
 requires-python = ">=3.9"
 authors = [{ name = "Chris Snijder", email = "github@chrissnijder.nl" }]
 readme = "README.md"
 keywords = ["vault", "hasicorp", "fixture", "testing", "migration"]
 dependencies = [
-    "cryptography~=41.0.0",
-    "hvac~=1.1.0",
-    "pyyaml~=6.0",
-    "rich~=13.5.2",
-    "typer[all]~=0.9.0",
+    "cryptography>=42.0.5",
+    "hvac>=0.10.11",
+    "pyyaml>=6.0",
+    "rich>=13.5.2",
+    "typer[all]>=0.9.0",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: POSIX :: Linux",
@@ -28,22 +28,21 @@
     "Programming Language :: Python :: 3.11",
 ]
 [project.urls]
 Homepage = "https://github.com/SnijderC/vault-fixtures"
 
 [project.optional-dependencies]
 dev = [
-    "black>=23.3.0",
-    "coverage>=7.2.7",
+    "coverage>=7.4.4",
     "hatch>=1.7.0",
     "pip-tools>=7.1.0",
-    "pytest>=7.3.2",
-    "pytest-asyncio>=0.21.0",
-    "pytest-cov>=4.0.0",
-    "pytest-random-order>=1.1.0",
+    "pytest>=8.1.1",
+    "pytest-asyncio>=0.23.6",
+    "pytest-cov>=5.0.0",
+    "pytest-random-order>=1.1.1",
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.ruff]
```

### Comparing `vault_fix-1.3.3/PKG-INFO` & `vault_fix-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: vault-fix
-Version: 1.3.3
+Version: 1.4.0
 Summary: Tool for importing and exporting vault fixture files to and from vault dev mode instances.
 Project-URL: Homepage, https://github.com/SnijderC/vault-fixtures
 Author-email: Chris Snijder <github@chrissnijder.nl>
 License: Copyright 2023 Chris Snijder
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
@@ -27,34 +27,33 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
-Requires-Dist: cryptography~=41.0.0
-Requires-Dist: hvac~=1.1.0
-Requires-Dist: pyyaml~=6.0
-Requires-Dist: rich~=13.5.2
-Requires-Dist: typer[all]~=0.9.0
+Requires-Dist: cryptography>=42.0.5
+Requires-Dist: hvac>=0.10.11
+Requires-Dist: pyyaml>=6.0
+Requires-Dist: rich>=13.5.2
+Requires-Dist: typer[all]>=0.9.0
 Provides-Extra: dev
-Requires-Dist: black>=23.3.0; extra == 'dev'
-Requires-Dist: coverage>=7.2.7; extra == 'dev'
+Requires-Dist: coverage>=7.4.4; extra == 'dev'
 Requires-Dist: hatch>=1.7.0; extra == 'dev'
 Requires-Dist: pip-tools>=7.1.0; extra == 'dev'
-Requires-Dist: pytest-asyncio>=0.21.0; extra == 'dev'
-Requires-Dist: pytest-cov>=4.0.0; extra == 'dev'
-Requires-Dist: pytest-random-order>=1.1.0; extra == 'dev'
-Requires-Dist: pytest>=7.3.2; extra == 'dev'
+Requires-Dist: pytest-asyncio>=0.23.6; extra == 'dev'
+Requires-Dist: pytest-cov>=5.0.0; extra == 'dev'
+Requires-Dist: pytest-random-order>=1.1.1; extra == 'dev'
+Requires-Dist: pytest>=8.1.1; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Vault-fix
 
 vault-fix is a CLI utility and python package that helps exporting and importing secrets to and from [Vault] instances.
-You can use this either to load fixture files for local development (it's original purpose). Or to migrate data from
+You can use this either to load fixture files for local development (its original purpose). Or to migrate data from
 Vault instance to another, while secrets may be [encrypted](#Encrypting-output) and/or
 [piped to another vault-fix instance](#Directing-data-to-the-load-command) so the data is not persisted.
 
 ## Historical context
 
 vault-fix was created to address an issue with the default mode of [Vault instances in dev mode], for local development.
 Vault will start with ephemeral storage, i.e. in-memory, mounting a volume will not make it persistent. If you want to
```

