# Comparing `tmp/edgegap_settings-1.1.0.tar.gz` & `tmp/edgegap_settings-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_settings-1.1.0.tar", max compression
+gzip compressed data, was "edgegap_settings-1.2.0.tar", max compression
```

## Comparing `edgegap_settings-1.1.0.tar` & `edgegap_settings-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1993 2024-04-30 16:04:37.499396 edgegap_settings-1.1.0/LICENSE
--rw-r--r--   0        0        0     2182 2024-04-30 16:04:37.499396 edgegap_settings-1.1.0/README.md
--rw-r--r--   0        0        0       17 2024-04-30 16:04:37.499396 edgegap_settings-1.1.0/edgegap_settings/BUILD
--rw-r--r--   0        0        0      358 2024-04-30 16:04:37.499396 edgegap_settings-1.1.0/edgegap_settings/__init__.py
--rw-r--r--   0        0        0      531 2024-04-30 16:04:37.499396 edgegap_settings-1.1.0/edgegap_settings/_apm.py
--rw-r--r--   0        0        0      872 2024-04-30 16:04:37.499396 edgegap_settings-1.1.0/edgegap_settings/_base.py
--rw-r--r--   0        0        0      119 2024-04-30 16:04:37.499396 edgegap_settings-1.1.0/edgegap_settings/_configuration.py
--rw-r--r--   0        0        0     3016 2024-04-30 16:04:37.499396 edgegap_settings-1.1.0/edgegap_settings/_factory.py
--rw-r--r--   0        0        0      963 2024-04-30 16:04:37.499396 edgegap_settings-1.1.0/edgegap_settings/_fields.py
--rw-r--r--   0        0        0      427 2024-04-30 16:04:37.499396 edgegap_settings-1.1.0/edgegap_settings/_logstash.py
--rw-r--r--   0        0        0      567 2024-04-30 16:04:42.827441 edgegap_settings-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 edgegap_settings-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2182 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/BUILD
+-rw-r--r--   0        0        0      359 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/_apm.py
+-rw-r--r--   0        0        0      872 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/_base.py
+-rw-r--r--   0        0        0      119 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/_configuration.py
+-rw-r--r--   0        0        0     2998 2024-05-01 17:52:18.963014 edgegap_settings-1.2.0/edgegap_settings/_factory.py
+-rw-r--r--   0        0        0      917 2024-05-01 17:52:18.967014 edgegap_settings-1.2.0/edgegap_settings/_fields.py
+-rw-r--r--   0        0        0      427 2024-05-01 17:52:18.967014 edgegap_settings-1.2.0/edgegap_settings/_logstash.py
+-rw-r--r--   0        0        0      741 2024-05-01 17:52:35.219413 edgegap_settings-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 edgegap_settings-1.2.0/PKG-INFO
```

### Comparing `edgegap_settings-1.1.0/LICENSE` & `edgegap_settings-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.1.0/README.md` & `edgegap_settings-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.1.0/edgegap_settings/_base.py` & `edgegap_settings-1.2.0/edgegap_settings/_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 from ._apm import ApmSettings
 from ._factory import SettingsFactory
 from ._fields import ConsulField
 from ._logstash import LogStashSettings
 
 
 class ProjectBaseSettings(BaseSettings):
-    name: str = ConsulField(key="NAME", description="The name of the project")
-    host: str = ConsulField(key="HOST", default="localhost", description="The host address of the project")
-    port: int = ConsulField(key="PORT", default=5000, description="The port of the project")
-    debug: bool = ConsulField(key="DEBUG", default=False, description="Enable debugging for project")
-    enabled: bool = ConsulField(key="ENABLED", default=True, description="If the project is Enabled (Deprecated)")
+    name: str = ConsulField(key='NAME', description='The name of the project')
+    host: str = ConsulField(key='HOST', default='localhost', description='The host address of the project')
+    port: int = ConsulField(key='PORT', default=5000, description='The port of the project')
+    debug: bool = ConsulField(key='DEBUG', default=False, description='Enable debugging for project')
+    enabled: bool = ConsulField(key='ENABLED', default=True, description='If the project is Enabled (Deprecated)')
     apm: ApmSettings = SettingsFactory.from_settings(ApmSettings)
     logstash: LogStashSettings = SettingsFactory.from_settings(LogStashSettings)
```

### Comparing `edgegap_settings-1.1.0/edgegap_settings/_factory.py` & `edgegap_settings-1.2.0/edgegap_settings/_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from edgegap_consul import ConsulReader, ConsulReaderFactory
 from edgegap_logging import DefaultFormatter
 from pydantic import ValidationError
 from pydantic_settings import BaseSettings
 
 load_dotenv()
 
-logger = logging.getLogger("settings.Factory")
+logger = logging.getLogger('settings.Factory')
 
 # Small Temporary formatting since this is most likely be called before any Logger Initialization
 fmt = DefaultFormatter()
 handler = logging.StreamHandler(sys.stdout)
 handler.setFormatter(fmt)
 logger.addHandler(handler)
 
@@ -25,56 +25,55 @@
     __consul_reader: ConsulReader = ConsulReaderFactory().from_env()
 
     @classmethod
     def from_settings(cls, settings: type(BaseSettings)) -> type(BaseSettings):
         name = settings.__name__
 
         if name not in cls.__mapping__.keys():
-            consul_prefix = settings.model_config.get("prefix")
+            consul_prefix = settings.model_config.get('prefix')
             data = {}
 
             for field_name, field in settings.model_fields.items():
                 if isinstance(field.json_schema_extra, dict):
-                    consul_key = field.json_schema_extra.get("consul_key")
-                    env_key = field.json_schema_extra.get("env_key")
+                    consul_key = field.json_schema_extra.get('consul_key')
+                    env_key = field.json_schema_extra.get('env_key')
                     value = None
 
                     # Check if in Environment Variable First
                     if isinstance(env_key, str):
                         value = os.environ.get(env_key, field.default)
 
                     # Consul Override Environment Variable
                     if isinstance(consul_prefix, str) and isinstance(consul_key, str):
-                        consul_full_key = f"{consul_prefix}/{consul_key}"
+                        consul_full_key = f'{consul_prefix}/{consul_key}'
                         value = cls.__from_consul(consul_full_key, field.default)
 
                     if value is not None:
                         data[field_name] = value
 
             try:
                 cls.__mapping__[name] = settings(**data)
             except ValidationError as e:
-                raise Exception("There was some errors during the Validation of your Settings, please adjust") from e
+                raise Exception('There was some errors during the Validation of your Settings, please adjust') from e
 
         return cls.__mapping__.get(name)
 
     @classmethod
     def __from_consul(cls, consul_full_key: str, default: Any = None) -> Any:
         exists, value = cls.__consul_reader.get(key=consul_full_key)
         has_default = default is not None
         has_value = value is not None
 
         if has_value:
             return value
         elif not has_value and has_default:
             if exists:
                 logger.warning(
-                    f"Key [{consul_full_key}] defined in Consul but the value was None,"
-                    f" will fallback to default value '{default}'"
+                    f'Key [{consul_full_key}] defined in Consul but the value was None,'
+                    f" will fallback to default value '{default}'",
                 )
             else:
                 logger.warning(
-                    f"Key [{consul_full_key}] does not exists in Consul but "
-                    f"default is defined to: '{default}'"
+                    f'Key [{consul_full_key}] does not exists in Consul but ' f"default is defined to: '{default}'",
                 )
         else:
-            raise Exception(f"Consul key [{consul_full_key}] is not defined and no default value")
+            raise Exception(f'Consul key [{consul_full_key}] is not defined and no default value')
```

### Comparing `edgegap_settings-1.1.0/edgegap_settings/_fields.py` & `edgegap_settings-1.2.0/edgegap_settings/_fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from typing import Any
 
 from pydantic import Field
 
 
 def ConsulField(  # noqa: C901
-        key: str = None,
-        default: Any = None,
-        description: str = None,
-        **kwargs
+    key: str = None,
+    default: Any = None,
+    description: str = None,
+    **kwargs,
 ) -> Any:
     return Field(
-        json_schema_extra={"consul_key": key},
+        json_schema_extra={'consul_key': key},
         default=default,
         description=description,
-        **kwargs
+        **kwargs,
     )
 
 
 def EnvironmentField(  # noqa: C901
-        key: str,
-        description: str = None,
-        default: Any = None,
-        **kwargs
+    key: str,
+    description: str = None,
+    default: Any = None,
+    **kwargs,
 ):
     return Field(
-        json_schema_extra={"env_key": key},
+        json_schema_extra={'env_key': key},
         default=default,
         description=description,
-        **kwargs
+        **kwargs,
     )
 
 
 def EnvConsulField(  # noqa: C901
-        env_key: str,
-        consul_key: str,
-        description: str = None,
-        default: Any = None,
-        **kwargs
+    env_key: str,
+    consul_key: str,
+    description: str = None,
+    default: Any = None,
+    **kwargs,
 ):
     return Field(
-        json_schema_extra={"env_key": env_key, "consul_key": consul_key},
+        json_schema_extra={'env_key': env_key, 'consul_key': consul_key},
         default=default,
         description=description,
-        **kwargs
+        **kwargs,
     )
```

### Comparing `edgegap_settings-1.1.0/PKG-INFO` & `edgegap_settings-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-settings
-Version: 1.1.0
+Version: 1.2.0
 Summary: The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

