# Comparing `tmp/strideutils-0.2.9.tar.gz` & `tmp/strideutils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strideutils-0.2.9.tar", max compression
+gzip compressed data, was "strideutils-0.3.0.tar", max compression
```

## Comparing `strideutils-0.2.9.tar` & `strideutils-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,32 @@
--rw-r--r--   0        0        0     1835 2024-04-26 19:50:03.632984 strideutils-0.2.9/README.md
--rw-r--r--   0        0        0      709 2024-04-26 19:50:03.632984 strideutils-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      373 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/Makefile
--rw-r--r--   0        0        0        0 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/__init__.py
--rw-r--r--   0        0        0     1233 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/coingecko.py
--rw-r--r--   0        0        0     5267 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/config_examples/strideutils_config.yaml.example
--rw-r--r--   0        0        0      443 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/config_examples/strideutils_secrets.yaml.example
--rw-r--r--   0        0        0     1270 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/cryptography.py
--rw-r--r--   0        0        0     1835 2024-04-26 19:50:03.632984 strideutils-0.2.9/strideutils/exec_tx.py
--rw-r--r--   0        0        0     1669 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/invariant_helpers.py
--rw-r--r--   0        0        0     1509 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/run_safely.py
--rw-r--r--   0        0        0     6793 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/sheets_connector.py
--rw-r--r--   0        0        0     1512 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/slack_connector.py
--rw-r--r--   0        0        0     5509 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/stride_alerts.py
--rw-r--r--   0        0        0    10449 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/stride_config.py
--rw-r--r--   0        0        0    33566 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/stride_requests.py
--rw-r--r--   0        0        0     2438 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/stride_upstash.py
--rw-r--r--   0        0        0     1064 2024-04-26 19:50:03.636984 strideutils-0.2.9/strideutils/twilio_connector.py
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1835 2024-05-01 20:33:11.841977 strideutils-0.3.0/README.md
+-rw-r--r--   0        0        0     1045 2024-05-01 20:33:11.841977 strideutils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      373 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/Makefile
+-rw-r--r--   0        0        0        0 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/__init__.py
+-rw-r--r--   0        0        0     5408 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/coingecko.py
+-rw-r--r--   0        0        0     5673 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/config_examples/strideutils_config.yaml.example
+-rw-r--r--   0        0        0      443 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/config_examples/strideutils_secrets.yaml.example
+-rw-r--r--   0        0        0     1270 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/cryptography.py
+-rw-r--r--   0        0        0     1835 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/exec_tx.py
+-rw-r--r--   0        0        0     1664 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/invariant_helpers.py
+-rw-r--r--   0        0        0     1551 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/run_safely.py
+-rw-r--r--   0        0        0     6793 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/sheets_connector.py
+-rw-r--r--   0        0        0     1512 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/slack_connector.py
+-rw-r--r--   0        0        0     5642 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/stride_alerts.py
+-rw-r--r--   0        0        0    12894 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/stride_config.py
+-rw-r--r--   0        0        0    31046 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/stride_requests.py
+-rw-r--r--   0        0        0     2438 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/stride_upstash.py
+-rw-r--r--   0        0        0     1064 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils/twilio_connector.py
+-rw-r--r--   0        0        0        0 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/__init__.pyi
+-rw-r--r--   0        0        0      257 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/coingecko.pyi
+-rw-r--r--   0        0        0      139 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/cryptography.pyi
+-rw-r--r--   0        0        0      511 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/exec_tx.pyi
+-rw-r--r--   0        0        0      237 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/invariant_helpers.pyi
+-rw-r--r--   0        0        0      290 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/run_safely.pyi
+-rw-r--r--   0        0        0      803 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/sheets_connector.pyi
+-rw-r--r--   0        0        0      242 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/slack_connector.pyi
+-rw-r--r--   0        0        0      987 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/stride_alerts.pyi
+-rw-r--r--   0        0        0     4591 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/stride_config.pyi
+-rw-r--r--   0        0        0     3977 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/stride_requests.pyi
+-rw-r--r--   0        0        0      419 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/stride_upstash.pyi
+-rw-r--r--   0        0        0      245 2024-05-01 20:33:11.841977 strideutils-0.3.0/strideutils-stubs/twilio_connector.pyi
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.3.0/PKG-INFO
```

### Comparing `strideutils-0.2.9/README.md` & `strideutils-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.9/strideutils/config_examples/strideutils_config.yaml.example` & `strideutils-0.3.0/strideutils/config_examples/strideutils_config.yaml.example`

 * *Files 10% similar despite different names*

```diff
@@ -21,133 +21,145 @@
   name: stride
   id: stride-1
   denom: ustrd
   ticker: STRD
   denom_decimals: 6
   api_endpoint:
   rpc_endpoint:
-  library_api:
-  library_rpc:
+  library_api_endpoint:
+  library_rpc_endpoint:
 
 # Host Zone Chains
 host_zones:
     cosmoshub:
       name: cosmoshub
       id: cosmoshub-4
       coingecko_name: cosmos
       denom: uatom
       ticker: ATOM
       denom_decimals: 6
+      denom_on_stride: ibc/27394FB092D2ECCD56123C74F36E4C1F926001CEADA9CA97EA622B25F41E5EB2
       inflation_frequency_hours: -1  # Every block
-      stride_token_hash: ibc/27394FB092D2ECCD56123C74F36E4C1F926001CEADA9CA97EA622B25F41E5EB2
       api_endpoint:
       rpc_endpoint:
 
     osmosis:
       name: osmosis
       id: osmosis-1
       denom: uosmo
       ticker: OSMO
       denom_decimals: 6
+      denom_on_stride: ibc/D24B4564BCD51D3D02D9987D92571EAC5915676A9BD6D9B0C1D0254CB8A5EA34
       inflation_frequency_hours: 24
-      stride_token_hash: ibc/D24B4564BCD51D3D02D9987D92571EAC5915676A9BD6D9B0C1D0254CB8A5EA34
       api_endpoint:
       rpc_endpoint:
 
     evmos:
       name: evmos
       id: evmos_9001-2
       denom: aevmos
       ticker: EVMOS
       denom_decimals: 18
+      denom_on_stride: ibc/4B322204B4F59D770680FE4D7A565DDC3F37BFF035474B717476C66A4F83DD72
       inflation_frequency_hours: 24
-      stride_token_hash: ibc/4B322204B4F59D770680FE4D7A565DDC3F37BFF035474B717476C66A4F83DD72
       api_endpoint:
       rpc_endpoint:
 
     injective:
       name: injective
       id: injective-1
       coingecko_name: injective-protocol
       denom: inj
       ticker: INJ
       denom_decimals: 18
+      denom_on_stride: ibc/A7454562FF29FE068F42F9DE4805ABEF54F599D1720B345D6518D9B5C64EA6D2
       inflation_frequency_hours: -1  # Every block
-      stride_token_hash: ibc/A7454562FF29FE068F42F9DE4805ABEF54F599D1720B345D6518D9B5C64EA6D2
       api_endpoint:
       rpc_endpoint:
 
     juno:
       name: juno
       id: juno-1
       denom: ujuno
       coingecko_name: juno-network
       ticker: JUNO
       denom_decimals: 6
+      denom_on_stride: ibc/DA356E369C3E5CF6A9F1DCD99CE8ED55FBD595E676A5CF033CE784C060492D5A
       inflation_frequency_hours: -1  # Every block
-      stride_token_hash: ibc/DA356E369C3E5CF6A9F1DCD99CE8ED55FBD595E676A5CF033CE784C060492D5A
       api_endpoint:
       rpc_endpoint:
 
     stargaze:
       name: stargaze
       id: stargaze-1
       denom: ustars
       ticker: STARS
       denom_decimals: 6
+      denom_on_stride: ibc/7EAE5BEF3A26B64AFBD89828AFDDB1DC7024A0276D22745201632C40E6E634D0
       inflation_frequency_hours: -1  # Every block
-      stride_token_hash: ibc/7EAE5BEF3A26B64AFBD89828AFDDB1DC7024A0276D22745201632C40E6E634D0
       api_endpoint:
       rpc_endpoint:
 
     terra:
       name: terra
       id: phoenix-1
       coingecko_name: terra
       denom: uluna
       ticker: LUNA
       denom_decimals: 6
+      denom_on_stride: ibc/E61BCB1126F42A2ED73B4CEA2221C9635BC2102F0417543C38071779F991942E
       inflation_frequency_hours: -1  # Every block
-      stride_token_hash: ibc/E61BCB1126F42A2ED73B4CEA2221C9635BC2102F0417543C38071779F991942E
       api_endpoint:
       rpc_endpoint:
 
     umee:
       name: umeee
       id: umee-1
       denom: uumee
       ticker: UMEE
       denom_decimals: 6
+      denom_on_stride: ibc/1A2271226209D309902AFF4F21BD21237CB514DD24EA2EE0423BF74C6135D8B8
       inflation_frequency_hours: -1  # Every block
-      stride_token_hash: ibc/1A2271226209D309902AFF4F21BD21237CB514DD24EA2EE0423BF74C6135D8B8
       api_endpoint:
       rpc_endpoint:
 
     comdex:
       name: comdex
       id: comdex-1
       denom: ucmdx
       ticker: CMDX
       denom_decimals: 6
+      denom_on_stride: ibc/EB66980014602E6BD50A1CB9FFB8FA694DC3EC10A48D2C1C649D732954F88D4A
       inflation_frequency_hours: -1  # Every block
-      stride_token_hash: ibc/EB66980014602E6BD50A1CB9FFB8FA694DC3EC10A48D2C1C649D732954F88D4A
       api_endpoint:
       rpc_endpoint:
 
     sommelier:
       name: sommelier
       id: sommelier-3
       denom: usomm
       ticker: SOMM
       denom_decimals: 6
+      denom_on_stride: ibc/B86EFF6D227E3E33D7E3B5E65D0C1BB5BD79CCB56D35A9D824F0DD5D52CA43BA
       inflation_frequency_hours: -1  # Every block
-      stride_token_hash: ibc/B86EFF6D227E3E33D7E3B5E65D0C1BB5BD79CCB56D35A9D824F0DD5D52CA43BA
       api_endpoint:
       rpc_endpoint:
 
+    celestia:
+      name: celestia
+      id: celestia
+      coingecko_name: celestia
+      denom: utia
+      ticker: TIA
+      denom_on_stride: ibc/BF3B4F53F3694B66E13C23107C84B6485BD2B96296BB7EC680EA77BBA75B4801
+      inflation_frequency_hours: -1  # Every block
+      api_endpoint: https://celestia-strd-api.polkachu.com
+      rpc_endpoint: https://celestia-strd-rpc.polkachu.com
+      ica_enabled: false
+
 # Other endpoints
 app_chains:
     neutron:
       name: neutron
       id: neutron-1
       api_endpoint:
     kava:
```

### Comparing `strideutils-0.2.9/strideutils/cryptography.py` & `strideutils-0.3.0/strideutils/cryptography.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.9/strideutils/exec_tx.py` & `strideutils-0.3.0/strideutils/exec_tx.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.9/strideutils/invariant_helpers.py` & `strideutils-0.3.0/strideutils/invariant_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     if str_output=True, this outputs the output as a pretty string instead of a DF
     '''
     df = []
     output = ""
     for zone in config.host_zones:
         host_zone_id = zone.id
-        host_zone = stride_requests.get_host_zone_json(host_zone_id)
+        host_zone = stride_requests.get_host_zone(host_zone_id)
 
         rr = host_zone['redemption_rate']
         min_rr, max_rr = host_zone['min_redemption_rate'], host_zone['max_redemption_rate']
         inner_min_rr, inner_max_rr = host_zone['min_inner_redemption_rate'], host_zone['max_inner_redemption_rate']
 
         tighter_bound_min = max(min_rr, inner_min_rr)
         tigher_bound_max = min(max_rr, inner_max_rr)
```

### Comparing `strideutils-0.2.9/strideutils/run_safely.py` & `strideutils-0.3.0/strideutils/run_safely.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         # Get the function name by first checking if there's a name attribute
         # (to cover cases where click was used)
         func_name = getattr(func, 'name', None) or func.__name__
         try:
             func()
             msg = [f':white_check_mark: {func_name}']
         except Exception:
+            print(traceback.format_exc())
             msg = [f':x: {func_name} ']
             tracebacks.append(f"{func_name} \n\n" + traceback.format_exc())
         msgs += msg
 
     count_succeeded_msg = f"{len(functions) - len(tracebacks)}/{len(functions)} {job_name} succeeded"
     if len(tracebacks) > 0:
         status_msg = f':x: {count_succeeded_msg}'
```

### Comparing `strideutils-0.2.9/strideutils/sheets_connector.py` & `strideutils-0.3.0/strideutils/sheets_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.9/strideutils/slack_connector.py` & `strideutils-0.3.0/strideutils/slack_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.9/strideutils/stride_alerts.py` & `strideutils-0.3.0/strideutils/stride_alerts.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 def notify(
     msgs: Union[str, List[str]],
     urgency,
     tag: Optional[Union[str, Iterable[str]]] = None,
     call: Optional[Union[str, Iterable[str]]] = None,
     beta_alert: bool = False,
+    debug_readme: str = config.alerts_playbook,
     debug_readme_section: str = "",
 ) -> None:
     """
     Post an alert in the proper channel and optionally call
 
     Args:
         msgs: A string or list of strings to notify on
@@ -55,15 +56,15 @@
         beta_alert: Modfies top-level message to not it's a work in progress
     """
     urgency = AlertType(urgency)
 
     msgs: List = cast(List, [msgs] if type(msgs) is str else msgs)
     top_level_message = str(msgs[0])
 
-    debug_msg = f"Read more: {config.alerts_playbook}{debug_readme_section}"
+    debug_msg = f"Read more: {debug_readme}{debug_readme_section}"
 
     channel = "#alerts-info"
     if urgency == AlertType.DEBUG:
         channel = "#alerts-debug"
     elif urgency == AlertType.INFO:
         channel = "#alerts-info"
     elif urgency == AlertType.WARNING:
@@ -84,14 +85,15 @@
 
 
 def raise_alert(
     urgency: Union[AlertType, str],
     tag: Optional[Union[str, Iterable[str]]] = None,
     call: Optional[Union[str, Iterable[str]]] = None,
     beta_alert: bool = False,
+    debug_readme: str = config.alerts_playbook,
     debug_readme_section: str = "",
 ) -> Callable:
     """
     Modify an alert to notify users based on severity
 
     The alert should have a return signature of
     msgs: Union[str, Iterable[str]]
@@ -118,14 +120,15 @@
             if msgs:
                 notify(
                     msgs=msgs,
                     urgency=urgency,
                     tag=tag,
                     call=call,
                     beta_alert=beta_alert,
+                    debug_readme=debug_readme,
                     debug_readme_section=debug_readme_section,
                 )
 
         return _func
 
     return _decorator
```

### Comparing `strideutils-0.2.9/strideutils/stride_config.py` & `strideutils-0.3.0/strideutils/stride_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 """
 This file loads and provide an object `config` to access all secrets, configs, and chain info
 """
 
 import itertools
 import os
 from dataclasses import dataclass, field, fields
-from typing import List, Optional, Union
+from typing import Any, List, Optional, Union
 
 import yaml
 
-MISSING_CONFIG_MSG = "Configuration or environment variable {x} is not set or unknown"
+MISSING_CONFIG_MSG = "Configuration or environment variable '{x}' is not set or unknown"
 
-ENV = None
-try:
-    ENV = os.environ['ENV']
-except KeyError:
-    raise ValueError(MISSING_CONFIG_MSG.format(x='ENV'))
+ENV = os.environ.get("ENV")
+if ENV not in ["DEV", "PROD"]:
+    raise ValueError("Environment variable 'ENV' must be set to either DEV or PROD")
 
 
+@dataclass
 class ConfigObj:
     """Raise an error if a config is not set."""
 
-    def __getattr__(self, name):
-        raise AttributeError(MISSING_CONFIG_MSG.format(x=name))
-
     def __getattribute__(self, name):
+        """
+        Called every time a field is attempted to be accessed
+        Falls back to getattr if the field is not found
+        """
         value = super().__getattribute__(name)
         if value == "" or value is None:
-            raise AttributeError  # induces a call to __getattr__
+            raise AttributeError(MISSING_CONFIG_MSG.format(x=name))
         return value
 
     def __iter__(self):
         """Allow iterating over set values"""
         for subfield in fields(self):
-            try:
-                value = getattr(self, subfield.name)
-            except AttributeError:
-                continue
-            yield value
+            if hasattr(self, subfield.name):
+                yield getattr(self, subfield.name)
+
+    def __contains__(self, field) -> bool:
+        """Allows for checking if an attribute is present with `in`"""
+        if not hasattr(self, field):
+            return False
+        return bool(getattr(self, field))
 
 
 class ConfigDict(dict):
     def __getitem__(self, key):
         """Raise an error if an unset key is indexed."""
-        try:
-            value = super().__getitem__(key)
-            if value == "" or value is None:
-                raise KeyError
-            return value
-        except KeyError:
+        if key not in self:
             raise KeyError(MISSING_CONFIG_MSG.format(x=key))
+        value = super().__getitem__(key)
+        if value == "" or value is None:
+            raise KeyError(MISSING_CONFIG_MSG.format(x=key))
+        return value
 
 
 # Use ConfigDict in the yaml parser
 class Loader(yaml.FullLoader):
     def construct_yaml_map(self, node):
         data = ConfigDict()
         yield data
@@ -62,47 +64,76 @@
 
 
 Loader.add_constructor('tag:yaml.org,2002:map', Loader.construct_yaml_map)
 
 
 @dataclass(repr=False)
 class ChainConfig(ConfigObj):
+    """Config relevant for all chains"""
+
     name: str = ""
     id: str = ""
-    # Optional. For looking up prices on coingecko if it differs from name
     coingecko_name: str = ""
     denom: str = ""
     denom_decimals: int = 6
-    inflation_frequency_hours: int = -1
     ticker: str = ""
-    stride_token_hash: str = ""
     api_endpoint: str = ""
     rpc_endpoint: str = ""
-    library_api: str = ""
-    library_rpc: str = ""
+
+    def __repr__(self) -> str:
+        return f"ChainConfig(name={self.name}, id={self.id})"
 
 
 @dataclass(repr=False)
-class HostZoneChainConfig(ConfigObj):
-    cosmoshub: ChainConfig = field(default_factory=ChainConfig)
-    osmosis: ChainConfig = field(default_factory=ChainConfig)
-    evmos: ChainConfig = field(default_factory=ChainConfig)
-    injective: ChainConfig = field(default_factory=ChainConfig)
-    juno: ChainConfig = field(default_factory=ChainConfig)
-    stargaze: ChainConfig = field(default_factory=ChainConfig)
-    terra: ChainConfig = field(default_factory=ChainConfig)
-    umee: ChainConfig = field(default_factory=ChainConfig)
-    comdex: ChainConfig = field(default_factory=ChainConfig)
-    sommelier: ChainConfig = field(default_factory=ChainConfig)
-    dydx: ChainConfig = field(default_factory=ChainConfig)
-    saga: ChainConfig = field(default_factory=ChainConfig)
+class StrideChainConfig(ChainConfig):
+    """Config specific to stride"""
+
+    library_api_endpoint: str = ""
+    library_rpc_endpoint: str = ""
+
+    def __repr__(self) -> str:
+        return f"StrideChainConfig(name={self.name}, id={self.id})"
+
+
+@dataclass(repr=False)
+class HostChainConfig(ChainConfig):
+    """Config specific to stride's host zones"""
+
+    # Frequency with which staking rewards are issued
+    # -1 indicates every block
+    inflation_frequency_hours: int = -1
+    # IBC denom of the native token as it sits on stride
+    denom_on_stride: str = ""
+    # Indicates whether the chain has ICA enabled
+    ica_enabled: bool = True
+
+    def __repr__(self) -> str:
+        return f"HostChainConfig(name={self.name}, id={self.id})"
+
+
+@dataclass(repr=False)
+class HostChainsConfig(ConfigObj):
+    cosmoshub: HostChainConfig = field(default_factory=HostChainConfig)
+    osmosis: HostChainConfig = field(default_factory=HostChainConfig)
+    evmos: HostChainConfig = field(default_factory=HostChainConfig)
+    injective: HostChainConfig = field(default_factory=HostChainConfig)
+    juno: HostChainConfig = field(default_factory=HostChainConfig)
+    stargaze: HostChainConfig = field(default_factory=HostChainConfig)
+    terra: HostChainConfig = field(default_factory=HostChainConfig)
+    umee: HostChainConfig = field(default_factory=HostChainConfig)
+    comdex: HostChainConfig = field(default_factory=HostChainConfig)
+    sommelier: HostChainConfig = field(default_factory=HostChainConfig)
+    dydx: HostChainConfig = field(default_factory=HostChainConfig)
+    saga: HostChainConfig = field(default_factory=HostChainConfig)
+    celestia: HostChainConfig = field(default_factory=HostChainConfig)
+    dymension: HostChainConfig = field(default_factory=HostChainConfig)
 
 
 @dataclass(repr=False)
-class AppConfig(ConfigObj):
+class AppChainsConfig(ConfigObj):
     neutron: ChainConfig = field(default_factory=ChainConfig)
     kava: ChainConfig = field(default_factory=ChainConfig)
     iris: ChainConfig = field(default_factory=ChainConfig)
     akash: ChainConfig = field(default_factory=ChainConfig)
     sentinel: ChainConfig = field(default_factory=ChainConfig)
     persistence: ChainConfig = field(default_factory=ChainConfig)
     cryptoorg: ChainConfig = field(default_factory=ChainConfig)
@@ -115,16 +146,14 @@
     secret: ChainConfig = field(default_factory=ChainConfig)
     axelar: ChainConfig = field(default_factory=ChainConfig)
     crescent: ChainConfig = field(default_factory=ChainConfig)
     mantle: ChainConfig = field(default_factory=ChainConfig)
     mars: ChainConfig = field(default_factory=ChainConfig)
     canto: ChainConfig = field(default_factory=ChainConfig)
     agoric: ChainConfig = field(default_factory=ChainConfig)
-    celestia: ChainConfig = field(default_factory=ChainConfig)
-    dymension: ChainConfig = field(default_factory=ChainConfig)
 
 
 @dataclass(repr=False)
 class Config(ConfigObj):
     ENV: str
     timezone: str = "US/Eastern"
 
@@ -161,31 +190,38 @@
     SLACK_SUCCESS_CHANNEL_ID: str = ""
     SLACK_INVARIANT_FAILURE_CHANNEL_ID: str = ""
     SLACK_PACKET_FAILURE_CHANNEL_ID: str = ""
     NUMIA_API_TOKEN: str = ""
     founders: List[str] = field(default_factory=lambda: ['riley', 'aidan', 'vishal'])
 
     # Chain configs
-    stride: ChainConfig = field(default_factory=ChainConfig)
-    host_zones: HostZoneChainConfig = field(default_factory=HostZoneChainConfig)
-    app_chains: AppConfig = field(default_factory=AppConfig)
+    stride: StrideChainConfig = field(default_factory=StrideChainConfig)
+    host_zones: HostChainsConfig = field(default_factory=HostChainsConfig)
+    app_chains: AppChainsConfig = field(default_factory=AppChainsConfig)
+
+    @property
+    def stakeibc_host_zones(self) -> List[HostChainConfig]:
+        return [host_zone for host_zone in self.host_zones if host_zone.ica_enabled]
 
     def _create_mappings(self) -> None:
         """
         Create a reverse map from attributes to ChainConfig if id, ticker, and denom are set.
         """
         name_to_zone = ConfigDict()
         id_to_zone = ConfigDict()
         ticker_to_zone = ConfigDict()
         denom_to_zone = ConfigDict()
-        stride_token_hash_to_zone = ConfigDict()
+        denom_on_stride_to_zone = ConfigDict()
 
         # Map host zones
         for chain_info in itertools.chain(self.host_zones, self.app_chains):
-            name_to_zone[chain_info.name] = chain_info
+            try:
+                name_to_zone[chain_info.name] = chain_info
+            except AttributeError:
+                pass
 
             try:
                 id_to_zone[chain_info.id] = chain_info
             except AttributeError:
                 pass
 
             try:
@@ -198,43 +234,43 @@
 
             try:
                 denom_to_zone[chain_info.denom] = chain_info
             except AttributeError:
                 pass
 
             try:
-                stride_token_hash_to_zone[chain_info.stride_token_hash] = chain_info
+                denom_on_stride_to_zone[chain_info.denom_on_stride] = chain_info
             except AttributeError:
                 pass
 
         self._name_to_zone = name_to_zone
         self._id_to_zone = id_to_zone
         self._ticker_to_zone = ticker_to_zone
         self._denom_to_zone = denom_to_zone
-        self._stride_token_hash = stride_token_hash_to_zone
+        self._denom_on_stride_to_zone = denom_on_stride_to_zone
 
     def __post_init__(self):
         self._create_mappings()
 
-    def get_chain(  # type: ignore[return]
+    def get_chain(
         self,
         name: Optional[str] = None,
         id: Optional[str] = None,
         ticker: Optional[str] = None,
         denom: Optional[str] = None,
-        stride_token_hash: Optional[str] = None,
-    ) -> ChainConfig:
+        denom_on_stride: Optional[str] = None,
+    ) -> Union[ChainConfig, StrideChainConfig, HostChainConfig]:
         """
         Fetch info about a host zone by name, id, ticker, denom, or token hash.
 
         Raises
             KeyError if a valid chain doesn't exist
         """
-        if sum(map(bool, [name, id, ticker, denom, stride_token_hash])) != 1:
-            raise ValueError("Exactly one of name, id, ticker, denom, or token hash must be specified.")
+        if sum(map(bool, [name, id, ticker, denom, denom_on_stride])) != 1:
+            raise KeyError("Exactly one of name, id, ticker, denom, or token hash must be specified.")
 
         if (
             name == self.stride.name
             or id == self.stride.id
             or ticker == self.stride.ticker
             or denom == self.stride.denom
         ):
@@ -243,59 +279,89 @@
             return self._name_to_zone[name]
         elif id:
             return self._id_to_zone[id]
         elif ticker:
             return self._ticker_to_zone[ticker]
         elif denom:
             return self._denom_to_zone[denom]
-        elif stride_token_hash:
-            return self._stride_token_hash[stride_token_hash]
+        return self._denom_on_stride_to_zone[denom_on_stride]
 
 
-# Load chain config
-def _load() -> Config:
+def _load_raw_config() -> dict[str, Any]:
     """
-    Load config dataclasses based on environment
+    Loads the raw config yaml into a dictionary
+    If STRIDEUTILS_CONFIG_PATH is set, it uses that for the config path, otherwise, it
+    looks for a config/config.yaml
     """
-    STRIDEUTILS_CONFIG_PATH = os.environ.get('STRIDEUTILS_CONFIG_PATH', 'config/config.yaml')
-    if not os.path.exists(STRIDEUTILS_CONFIG_PATH):
+    strideutils_config_path = os.environ.get('STRIDEUTILS_CONFIG_PATH', 'config/config.yaml')
+    if not os.path.exists(strideutils_config_path):
         raise ValueError(
-            'Shell var STRIDEUTILS_CONFIG_PATH is missing or the file does not exist.'
+            'Shell var STRIDEUTILS_CONFIG_PATH is missing or the file does not exist in the default location.'
             'The default file and location is config/config.yaml in the current working directory'
         )
 
-    with open(STRIDEUTILS_CONFIG_PATH, 'r') as f:
-        raw_config = yaml.load(f, Loader)
-        stride_chain_config = ChainConfig(**raw_config.get('stride'))
-        host_zone_config = HostZoneChainConfig(
-            **{name: ChainConfig(**info) for name, info in raw_config.get('host_zones').items()}
-        )
-        app_chain_config = AppConfig(
-            **{name: ChainConfig(**info) for name, info in raw_config.get('app_chains').items()}
-        )
+    with open(strideutils_config_path, 'r') as config_file:
+        raw_config = yaml.load(config_file, Loader)
+
+    return raw_config
+
+
+def _load_raw_secrets() -> dict[str, Optional[str]]:
+    """
+    Loads the secret variables into a dictionary
+    If this is running locally in dev mode, secrets are grabbed from the path defined by STRIDEUTILS_SECRETS_PATH
+    Otherwise, their loaded as environment variables
+    """
+    if ENV == "PROD":
+        return {secret.name: os.environ.get(secret.name) for secret in fields(Config) if os.environ.get(secret.name)}
+
+    if not (strideutils_secrets_path := os.environ.get('STRIDEUTILS_SECRETS_PATH')):
+        raise ValueError(MISSING_CONFIG_MSG.format(x='STRIDEUTILS_SECRETS_PATH'))
+
+    with open(strideutils_secrets_path, 'r') as f:
+        raw_secrets = yaml.load(f, Loader)
+        raw_secrets.update({'ENV': ENV})
+
+        return raw_secrets
+
+
+def _parse_raw_configs(raw_config: dict[str, Any], raw_secrets: dict[str, Optional[str]]) -> Config:
+    """
+    Builds the relevant config data classes from the raw jsons
+    """
+    host_chain_fields = [field.name for field in fields(HostChainsConfig)]
+    app_chain_fields = [field.name for field in fields(AppChainsConfig)]
+
+    host_chain_config_dict = {
+        name: HostChainConfig(**info) for name, info in raw_config["host_zones"].items() if name in host_chain_fields
+    }
+    app_chain_config_dict = {
+        name: ChainConfig(**info) for name, info in raw_config["app_chains"].items() if name in app_chain_fields
+    }
+
+    stride_chain_config = StrideChainConfig(**raw_config["stride"])
+    host_zone_config = HostChainsConfig(**host_chain_config_dict)
+    app_chain_config = AppChainsConfig(**app_chain_config_dict)
+
     chain_configs = {
         'stride': stride_chain_config,
         'host_zones': host_zone_config,
         'app_chains': app_chain_config,
     }
 
-    # Load secrets
-    if ENV == 'DEV':
-        if not (STRIDEUTILS_SECRETS_PATH := os.environ.get('STRIDEUTILS_SECRETS_PATH')):
-            raise ValueError(MISSING_CONFIG_MSG.format(x='STRIDEUTILS_SECRETS_PATH'))
-        with open(STRIDEUTILS_SECRETS_PATH, 'r') as f:
-            raw_secrets = yaml.load(f, Loader)
-            raw_secrets.update({'ENV': ENV})
-    elif ENV == 'PROD':
-        raw_secrets = {
-            secret.name: os.environ.get(secret.name) for secret in fields(Config) if os.environ.get(secret.name)
-        }
-
-    # Load vanilla configs
-    raw_secrets.update(raw_config)
-    # Overwrite prepped ChainConfigs
-    raw_secrets.update(chain_configs)
-    config = Config(**raw_secrets)
-    return config
+    # Load non-nested configs, then overwrite with the chain configs
+    config_dict = raw_secrets
+    config_dict.update(raw_config)
+    config_dict.update(chain_configs)
+    return Config(**config_dict)  # type: ignore
+
+
+def _init_config() -> Config:
+    """
+    Initializes the main config files
+    """
+    raw_config = _load_raw_config()
+    raw_secrets = _load_raw_secrets()
+    return _parse_raw_configs(raw_config, raw_secrets)
 
 
-config: Config = _load()
+config: Config = _init_config()
```

### Comparing `strideutils-0.2.9/strideutils/stride_requests.py` & `strideutils-0.3.0/strideutils/stride_requests.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 EPOCHS_QUERY = "Stridelabs/stride/epochs"
 
 RATE_LIMIT_QUERY = "Stride-Labs/ibc-rate-limiting/ratelimit/ratelimits"
 
 STAKETIA = "staketia"
 STAKEDYM = "stakedym"
 
+CELESTIA_CHAIN_ID = "celestia"
+DYMENSION_CHAIN_ID = "dymension_1100-1"
+
 MULTISIG_HOST_ZONE_QUERY = "Stride-Labs/stride/{module}/host_zone"
 MULTISIG_DELEGATION_RECORDS_QUERY = "Stride-Labs/stride/{module}/delegation_records"
 MULTISIG_UNBONDING_RECORDS_QUERY = "Stride-Labs/stride/{module}/unbonding_records"
 MULTISIG_REDEMPTION_RECORDS_QUERY = "Stride-Labs/stride/{module}/redemption_records"
 
 COSMWASM_CONTRACT_QUERY = "cosmwasm/wasm/v1/contract/{contract_address}/smart/{query}"
 
@@ -134,17 +137,19 @@
         # Update query url with next key
         encoded_pagination_key = urllib.parse.quote_plus(pagination_key)
         query_url = f"{endpoint}?pagination.key={encoded_pagination_key}"
 
     return data
 
 
-def get_all_host_zones() -> List[Dict]:
+def get_all_host_zones(include_multisig_hosts: bool = True) -> List[Dict]:
     """
     Queries all host zone structs, returning a list of each host zone json
+    By default, this queries both stakeibc and staketia/stakedym; however,
+    staketia/stakedym can be disabled by passing include_multisig_hosts = False
 
     Returns:
         A list of host zone structs
             e.g. [{'chain_id': 'comdex-1',
                   'bech32prefix': 'comdex',
                   'connection_id': 'connection-28',
                   'transfer_channel_id': 'channel-49',
@@ -180,19 +185,27 @@
                   'min_inner_redemption_rate': '1.138890000000000000',
                   'max_inner_redemption_rate': '1.171390000000000000',
                   'lsm_liquid_stake_enabled': False,
                   'halted': False},
                   ...more host zones]
 
     """
-    endpoint = f"{config.stride.api_endpoint}/{HOST_ZONE_QUERY}"
-    response = request(endpoint)
-    host_zones = response["host_zone"]
+    stakeibc_response = request(f"{config.stride.api_endpoint}/{HOST_ZONE_QUERY}")
+    stakeibc_host_zones = stakeibc_response["host_zone"]
+
+    if not include_multisig_hosts:
+        return stakeibc_host_zones
+
+    staketia_host_zone = get_host_zone(CELESTIA_CHAIN_ID, cast_types=False)
+    stakedym_host_zone = get_host_zone(DYMENSION_CHAIN_ID, cast_types=False)
+
+    stakedym_response = request(f"{config.stride.api_endpoint}/{MULTISIG_HOST_ZONE_QUERY.format(module=STAKEDYM)}")
+    stakedym_host_zone = stakedym_response["host_zone"]
 
-    return host_zones
+    return stakeibc_host_zones + [staketia_host_zone, stakedym_host_zone]
 
 
 def _cast_host_zone_fields(host_zone: Dict[str, Any]) -> Dict[str, Any]:
     """
     Casts the host zone int and float types
     """
     float_columns = [
@@ -209,103 +222,32 @@
         host_zone[column] = float(host_zone[column])
     for column in [c for c in int_columns if c in host_zone]:
         host_zone[column] = int(host_zone[column])
 
     return host_zone
 
 
-def get_host_zone_json(zone_id: str, cast_types: bool = True, **kwargs) -> Dict[str, Any]:
+def get_host_zone(chain_id: str, cast_types: bool = True, **kwargs) -> Dict[str, Any]:
     """
     Queries a stakeibc host zone, returning a dict with the host zone structure and fields casted
     """
-    if zone_id == "celestia":
-        return get_celestia_host_zone(cast_types=cast_types)
-    if zone_id == "dymension_1100-1":
-        return get_dymension_host_zone(cast_types=cast_types)
+    query = f"Stride-Labs/stride/stakeibc/host_zone/{chain_id}"
+    if chain_id in [CELESTIA_CHAIN_ID, DYMENSION_CHAIN_ID]:
+        query = MULTISIG_HOST_ZONE_QUERY.format(module=STAKETIA)
+    if chain_id == "dymension_1100-1":
+        query = MULTISIG_HOST_ZONE_QUERY.format(module=STAKEDYM)
 
-    endpoint = f"{config.stride.api_endpoint}/Stride-Labs/stride/stakeibc/host_zone/{zone_id}"
-    host_zone = request(endpoint, **kwargs)["host_zone"]
+    host_zone = request(f"{config.stride.api_endpoint}/{query}", **kwargs)["host_zone"]
 
     if cast_types:
         host_zone = _cast_host_zone_fields(host_zone)
 
     return host_zone
 
 
-# TODO: Consolidate celestia and dymension queries (API breaking)
-def get_celestia_host_zone(cast_types: bool = True) -> Dict[str, Any]:
-    """
-    Queries the celestia host zone from staketia
-
-    Example response:
-    {
-        'chain_id': 'celestia',
-        'native_token_denom': 'utia',
-        'native_token_ibc_denom': 'ibc/BF3B4F53F3694B66E13C23107C84B6485BD2B96296BB7EC680EA77BBA75B4801',
-        'transfer_channel_id': 'channel-162',
-        'delegation_address': 'celestia1d6ntc7s8gs86tpdyn422vsqc6uaz9cejnxz5p5',
-        'reward_address': 'celestia15up3hegy8zuqhy0p9m8luh0c984ptu2g5p4xpf',
-        'deposit_address': 'stride1d6ntc7s8gs86tpdyn422vsqc6uaz9cejp8nc04',
-        'redemption_address': 'stride15up3hegy8zuqhy0p9m8luh0c984ptu2gxqy20g',
-        'claim_address': 'stride13nw9fm4ua8pwzmsx9kdrhefl4puz0tp7ge3gxd',
-        'operator_address_on_stride': 'stride1ghhu67ttgmxrsyxljfl2tysyayswklvxs7pepw',
-        'safe_address_on_stride': 'stride18p7xg4hj2u3zpk0v9gq68pjyuuua5wa387sjjc',
-        'last_redemption_rate': '1.000000000000000000',
-        'redemption_rate': '1.000000000000000000',
-        'min_redemption_rate': '0.950000000000000000',
-        'max_redemption_rate': '1.100000000000000000',
-        'min_inner_redemption_rate': '0.950000000000000000',
-        'max_inner_redemption_rate': '1.100000000000000000',
-        'delegated_balance': '300000',
-        'unbonding_period_seconds': '1814400',
-        'halted': False
-    }
-    """
-    url = f"{config.stride.api_endpoint}/{MULTISIG_HOST_ZONE_QUERY.format(module=STAKETIA)}"
-    host_zone = request(url)["host_zone"]
-    if cast_types:
-        _cast_host_zone_fields(host_zone)
-    return host_zone
-
-
-def get_dymension_host_zone(cast_types: bool = True) -> Dict[str, Any]:
-    """
-    Queries the dymension host zone from stakedym
-
-    Example response:
-    {
-        'chain_id': 'dymension',
-        'native_token_denom': 'adym',
-        'native_token_ibc_denom': 'ibc/E1C22332C083574F3418481359733BA8887D171E76C80AD9237422AEABB66018',
-        'transfer_channel_id': 'channel-197',
-        'delegation_address': 'dym1gl9j2hyyukqvlmzzcxl99mqfgu4y4frgzlv3zz',
-        'reward_address': 'dym1ww3m6h5e3dk2musft9w8f2zu4rkuxgh6zwu0d0',
-        'deposit_address': 'stride1e7j8d6sdq272fqe2jfxjpgcagn04j75w9695fj',
-        'redemption_address': 'stride1jpsnc0ynufa2aheflj6mxzzzsu7nlwqk7ff69n',
-        'claim_address': 'stride1q8juddwptg5yxyghh3n243pp4w8ctpvpmf6ras',
-        'operator_address_on_stride': 'stride1ghhu67ttgmxrsyxljfl2tysyayswklvxs7pepw',
-        'safe_address_on_stride': 'stride1sj8gyqeqecqhqu7em67hn2tjzhpkdf8wz5plh7',
-        'last_redemption_rate': '1.000000000000000000',
-        'redemption_rate': '1.000000000000000000',
-        'min_redemption_rate': '0.950000000000000000',
-        'max_redemption_rate': '1.100000000000000000',
-        'min_inner_redemption_rate': '0.950000000000000000',
-        'max_inner_redemption_rate': '1.100000000000000000',
-        'delegated_balance': '300000',
-        'unbonding_period_seconds': '1814400',
-        'halted': False
-    }
-    """
-    url = f"{config.stride.api_endpoint}/{MULTISIG_HOST_ZONE_QUERY.format(module=STAKEDYM)}"
-    host_zone = request(url)["host_zone"]
-    if cast_types:
-        _cast_host_zone_fields(host_zone)
-    return host_zone
-
-
 def get_multisig_delegation_records(module: str, include_archived: bool = False) -> List[Dict]:
     """
     Queries the delegation records from staketia or stakedym
     Optionally include archive records
 
     Example response:
     [
@@ -415,28 +357,26 @@
     return query_list_with_pagination(url, rel_key="slashes", params=params)
 
 
 def get_redemption_rate(token: str) -> float:
     """
     Queries the redemption rate for a particular token
     """
-    js = get_host_zone_json(config.get_chain(ticker=token).id)
-    return float(js["redemption_rate"])
+    host_zone = get_host_zone(config.get_chain(ticker=token).id)
+    return float(host_zone["redemption_rate"])
 
 
 def get_tvl_in_utokens(host_zone_id: str) -> float:
     """
     Queries the stride TVL for a given zone (denominated in the native token)
     """
-    zone_info = config.get_chain(id=host_zone_id)
-    js = get_host_zone_json(host_zone_id)
-    delegation_key = "total_delegations"
-    if delegation_key not in js:
-        delegation_key = "delegated_balance"
-    return int(js[delegation_key]) / pow(10, zone_info.denom_decimals)
+    host_zone_config = config.get_chain(id=host_zone_id)
+    host_zone = get_host_zone(host_zone_id)
+    delegation_key = "total_delegations" if host_zone_config.ica_enabled else "delegated_balance"
+    return int(host_zone[delegation_key]) / pow(10, host_zone_config.denom_decimals)
 
 
 def get_latest_block(rpc_endpoint: str = config.stride.rpc_endpoint) -> int:
     """
     Queries the latest block time for a given chain
     """
     url = f"{rpc_endpoint}/status"
@@ -456,15 +396,15 @@
         raise ValueError("invalid address")
     return bech32.bech32_encode(new_prefix, cast(List[int], data))
 
 
 def get_balances(
     address: str,
     block_height: int = 0,
-    api_endpoint: str = config.stride.library_api,
+    api_endpoint: str = config.stride.api_endpoint,
     cache_response: bool = False,
 ) -> Dict[str, int]:
     """
     Returns the balance of the given address across all tokens,
     returned as a dictionary of token -> balance
     """
     url = f"{api_endpoint}/{ACCOUNT_BALANCE_QUERY.format(address=address)}"
@@ -472,15 +412,15 @@
     return {balance["denom"]: int(balance["amount"]) for balance in response["balances"]}
 
 
 def get_balance(
     address: str,
     denom: str,
     block_height: int = 0,
-    api_endpoint: str = config.stride.library_api,
+    api_endpoint: str = config.stride.api_endpoint,
     cache_response: bool = False,
 ) -> int:
     """
     Returns the balance for a given address and token
     """
     url = f"{api_endpoint}/{ACCOUNT_BALANCE_QUERY.format(address=address)}/by_denom"
     params = {"denom": denom}
@@ -500,15 +440,15 @@
     url = f"{api_endpoint}/{SUPPLY_QUERY}"
     params = {"denom": denom}
     resp = request(url, block_height=block_height, params=params, cache_response=cache_response)
     return int(resp["amount"]["amount"])
 
 
 @lru_cache
-def get_block_time(height: int, rpc_endpoint: str = config.stride.library_rpc) -> datetime.datetime:
+def get_block_time(height: int, rpc_endpoint: str = config.stride.library_rpc_endpoint) -> datetime.datetime:
     """
     Returns the timestamp of the given block height on a chain
     """
     url = f"{rpc_endpoint}/block?height={height}"
     resp = request(url)
     block_time = resp["result"]["block"]["header"]["time"]
     block_datetime = dateutil.parser.parse(block_time).replace(tzinfo=None)
@@ -611,15 +551,15 @@
     and distribute the given number of ustrd tokens over the specified number of days.
 
     The vested tokens will be distributed over the specified number of days, with the period
     length being the specified number of seconds.
 
     The output is a JSON object that can be used to create a vesting account on the Stride chain.
     """
-    timezone = pytz.timezone(config.TIMEZONE)
+    timezone = pytz.timezone(config.timezone)
     start_time = timezone.localize(datetime.datetime.strptime(start_time_in_local_tz, "%Y-%m-%d %H:%M"))
     start_time = start_time.astimezone(pytz.utc)
     start_time = int(start_time.timestamp())
 
     out = '{ "start_time": ' + str(start_time) + ',\n  "periods":[\n'
     num_periods = int(number_of_days * 24 * 60 * 60) // seconds_in_period
     tokens_per_period = int(total_tokens / num_periods)
@@ -639,15 +579,15 @@
 
 def get_block_height_in_past(
     time_in_past: datetime.timedelta = datetime.timedelta(hours=24),
     max_acceptable_error_seconds: int = 60 * 5,
     seconds_per_block: int = 6,
     prev_time: Optional[str] = None,
     verbose: bool = False,
-    rpc_endpoint: str = config.stride.library_rpc,
+    rpc_endpoint: str = config.stride.library_rpc_endpoint,
 ) -> int:
     """
     Gets the block height at a specified time by binary searching at different heights
 
     Args:
         time_in_past: target time to search for
         max_acceptable_error_seconds: max time delta before the height is considered find
@@ -782,15 +722,15 @@
 def get_host_zone_delegations(host_zone_id: str, ground_truth_included: bool = True) -> pd.DataFrame:
     """
     Given a host zone id, returns a Dataframe of validator delegations.
 
     If `ground_truth_included=True`, then will also return the "true" delegations
     on the host zone delegaiton account.
     """
-    host_zone = get_host_zone_json(host_zone_id)
+    host_zone = get_host_zone(host_zone_id)
     vdf = pd.DataFrame(host_zone["validators"])
     int_cols = [
         "weight",
         "delegation",
         "slash_query_progress_tracker",
         "slash_query_checkpoint",
         "shares_to_tokens_rate",
```

### Comparing `strideutils-0.2.9/strideutils/stride_upstash.py` & `strideutils-0.3.0/strideutils/stride_upstash.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.9/strideutils/twilio_connector.py` & `strideutils-0.3.0/strideutils/twilio_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.9/PKG-INFO` & `strideutils-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strideutils
-Version: 0.2.9
+Version: 0.3.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

