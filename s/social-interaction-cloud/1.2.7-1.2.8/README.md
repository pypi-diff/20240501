# Comparing `tmp/social_interaction_cloud-1.2.7.tar.gz` & `tmp/social_interaction_cloud-1.2.8.tar.gz`

## Comparing `social_interaction_cloud-1.2.7.tar` & `social_interaction_cloud-1.2.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.7/src/social_interaction_cloud/__init__.py
--rw-r--r--   0        0        0    42012 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.7/src/social_interaction_cloud/abstract_connector.py
--rw-r--r--   0        0        0    46356 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.7/src/social_interaction_cloud/basic_connector.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.7/src/social_interaction_cloud/choregraphe_to_json.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.7/src/social_interaction_cloud/detection_result_pb2.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.7/src/social_interaction_cloud/tracking_result_pb2.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.7/LICENSE
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.7/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.8/src/social_interaction_cloud/__init__.py
+-rw-r--r--   0        0        0    42281 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.8/src/social_interaction_cloud/abstract_connector.py
+-rw-r--r--   0        0        0    46836 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.8/src/social_interaction_cloud/basic_connector.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.8/src/social_interaction_cloud/choregraphe_to_json.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.8/src/social_interaction_cloud/detection_result_pb2.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.8/src/social_interaction_cloud/tracking_result_pb2.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.8/LICENSE
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.8/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 social_interaction_cloud-1.2.8/PKG-INFO
```

### Comparing `social_interaction_cloud-1.2.7/src/social_interaction_cloud/abstract_connector.py` & `social_interaction_cloud-1.2.8/src/social_interaction_cloud/abstract_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
                                        'dialogflow_agent', 'dialogflow_record'],
             self.device_types['robot']: ['action_gesture', 'action_eyecolour', 'action_earcolour', 'action_headcolour',
                                          'action_idle', 'action_turn', 'action_wakeup', 'action_rest',
                                          'action_set_breathing', 'action_posture', 'action_stiffness',
                                          'action_play_motion', 'action_record_motion',  # 'action_motion_file',
                                          'action_led_color', 'action_led_animation',
                                          'memory_create_interactant', 'memory_set_session',
-                                         'memory_set_entry', 'memory_get_entry', 'memory_delete_entry',
+                                         'memory_set_entry', 'memory_get_entry', 'memory_get_entry_by_field',
+                                         'memory_delete_entry',
                                          'memory_get_entries', 'memory_delete_entries',
                                          'memory_get_all_entries',
                                          'memory_set_interactant_data', 'memory_get_interactant_data',
                                          'memory_delete_interactant_data',
                                          'memory_get_interactant_data_all', 'memory_get_all_interactants',
                                          'memory_set_interactant', 'memory_set_dialog_history',
                                          'memory_get_dialog_history_all',
@@ -629,14 +630,17 @@
 
     def set_memory_entry(self, interactant_id: str, entry_type: str, entry_data: dict):
         self.__send('memory_set_entry', f'{interactant_id};{entry_type};{dumps(entry_data)}')
 
     def get_memory_entry(self, interactant_id: str, entry_type: str, entry_id: str):
         self.__send('memory_get_entry', f'{interactant_id};{entry_type};{entry_id}')
 
+    def get_memory_entry_by_field(self, interactant_id: str, entry_type: str, key: str, value: str):
+        self.__send('memory_get_entry_by_field', f'{interactant_id};{entry_type};{key};{value}')
+
     def delete_memory_entry(self, interactant_id: str, entry_type: str, entry_id: str):
         self.__send('memory_delete_entry', f'{interactant_id};{entry_type};{entry_id}')
 
     def get_memory_entries(self, interactant_id: str, entry_type: str):
         self.__send('memory_get_entries', f'{interactant_id};{entry_type}')
 
     def delete_memory_entries(self, interactant_id: str, entry_type: str):
```

### Comparing `social_interaction_cloud-1.2.7/src/social_interaction_cloud/basic_connector.py` & `social_interaction_cloud-1.2.8/src/social_interaction_cloud/basic_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,14 +686,20 @@
 
     def get_memory_entry(self, interactant_id: str, entry_type: str, entry_id: str,
                          callback: callable = None, sync: bool = True, load: bool = False) -> None:
         self.__process_action(super(BasicSICConnector, self).get_memory_entry, interactant_id, entry_type, entry_id,
                               callback=callback, event='Entry', sync=sync, load=load,
                               listener_type=ListenerType.MEMORY)
 
+    def get_memory_entry_by_field(self, interactant_id: str, entry_type: str, key: str, value: str,
+                         callback: callable = None, sync: bool = True, load: bool = False) -> None:
+        self.__process_action(super(BasicSICConnector, self).get_memory_entry_by_field, interactant_id, entry_type, key, value,
+                              callback=callback, event='Entry', sync=sync, load=load,
+                              listener_type=ListenerType.MEMORY)
+
     def delete_memory_entry(self, interactant_id: str, entry_type: str, entry_id: str,
                            callback: callable = None, sync: bool = True, load: bool = False):
         self.__process_action(super(BasicSICConnector, self).delete_memory_entry, interactant_id, entry_type, entry_id,
                               callback=callback, event='EntryDeleted', sync=sync, load=load)
 
     def get_memory_entries(self, interactant_id: str, entry_type: str, callback: callable = None,
                            sync: bool = True, load: bool = False):
```

### Comparing `social_interaction_cloud-1.2.7/src/social_interaction_cloud/choregraphe_to_json.py` & `social_interaction_cloud-1.2.8/src/social_interaction_cloud/choregraphe_to_json.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.7/src/social_interaction_cloud/detection_result_pb2.py` & `social_interaction_cloud-1.2.8/src/social_interaction_cloud/detection_result_pb2.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.7/src/social_interaction_cloud/tracking_result_pb2.py` & `social_interaction_cloud-1.2.8/src/social_interaction_cloud/tracking_result_pb2.py`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.7/LICENSE` & `social_interaction_cloud-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `social_interaction_cloud-1.2.7/pyproject.toml` & `social_interaction_cloud-1.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "social_interaction_cloud"
-version = "1.2.7"
+version = "1.2.8"
 authors = [
   { name="Mike Ligthart", email="m.e.u.ligthart@vu.nl" },
 ]
 description = "Connector to the Social Interaction Cloud"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `social_interaction_cloud-1.2.7/PKG-INFO` & `social_interaction_cloud-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: social_interaction_cloud
-Version: 1.2.7
+Version: 1.2.8
 Summary: Connector to the Social Interaction Cloud
 Project-URL: Source, https://bitbucket.org/socialroboticshub/connectors/src/master/python/sic/
 Project-URL: Wiki, https://socialrobotics.atlassian.net/wiki/spaces/CBSR/overview
 Author-email: Mike Ligthart <m.e.u.ligthart@vu.nl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

