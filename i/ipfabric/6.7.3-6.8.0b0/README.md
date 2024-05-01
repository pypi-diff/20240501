# Comparing `tmp/ipfabric-6.7.3.tar.gz` & `tmp/ipfabric-6.8.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric-6.7.3.tar", max compression
+gzip compressed data, was "ipfabric-6.8.0b0.tar", max compression
```

## Comparing `ipfabric-6.7.3.tar` & `ipfabric-6.8.0b0.tar`

### file list

```diff
@@ -1,90 +1,93 @@
--rw-r--r--   0        0        0     1294 2024-02-21 17:21:14.240240 ipfabric-6.7.3/ipfabric/__init__.py
--rw-r--r--   0        0        0    12155 2024-04-29 16:39:30.730052 ipfabric-6.7.3/ipfabric/api.py
--rw-r--r--   0        0        0    10196 2024-04-29 16:39:30.730052 ipfabric-6.7.3/ipfabric/auth.py
--rw-r--r--   0        0        0    23368 2024-04-29 16:39:30.731051 ipfabric-6.7.3/ipfabric/client.py
--rw-r--r--   0        0        0      693 2024-02-29 12:11:26.623633 ipfabric-6.7.3/ipfabric/diagrams/__init__.py
--rw-r--r--   0        0        0    18216 2024-03-29 13:49:06.793074 ipfabric-6.7.3/ipfabric/diagrams/graphs.py
--rw-r--r--   0        0        0     3625 2024-02-22 21:24:28.609926 ipfabric-6.7.3/ipfabric/diagrams/icmp.py
--rw-r--r--   0        0        0      867 2024-02-29 12:11:26.625974 ipfabric-6.7.3/ipfabric/diagrams/input_models/__init__.py
--rw-r--r--   0        0        0     3808 2024-02-29 12:11:26.627304 ipfabric-6.7.3/ipfabric/diagrams/input_models/constants.py
--rw-r--r--   0        0        0        0 2023-12-13 15:03:30.792953 ipfabric-6.7.3/ipfabric/diagrams/input_models/factory_defaults/__init__.py
--rw-r--r--   0        0        0     5792 2023-12-13 15:03:30.792953 ipfabric-6.7.3/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
--rw-r--r--   0        0        0     2173 2023-12-13 15:03:30.794172 ipfabric-6.7.3/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
--rw-r--r--   0        0        0    12911 2024-02-29 12:11:26.628310 ipfabric-6.7.3/ipfabric/diagrams/input_models/graph_parameters.py
--rw-r--r--   0        0        0    13870 2024-02-29 12:11:26.629771 ipfabric-6.7.3/ipfabric/diagrams/input_models/graph_settings.py
--rw-r--r--   0        0        0     5026 2024-02-29 12:11:26.630778 ipfabric-6.7.3/ipfabric/diagrams/input_models/shared_view.py
--rw-r--r--   0        0        0       90 2024-02-29 12:11:26.632075 ipfabric-6.7.3/ipfabric/diagrams/output_models/__init__.py
--rw-r--r--   0        0        0     5241 2024-02-29 12:11:26.633080 ipfabric-6.7.3/ipfabric/diagrams/output_models/graph_result.py
--rw-r--r--   0        0        0     2278 2024-01-25 18:33:47.040766 ipfabric-6.7.3/ipfabric/diagrams/output_models/protocols.py
--rw-r--r--   0        0        0     4556 2024-02-29 12:11:26.634080 ipfabric-6.7.3/ipfabric/diagrams/output_models/trace.py
--rw-r--r--   0        0        0     2283 2024-03-20 16:35:10.768244 ipfabric-6.7.3/ipfabric/exceptions.py
--rw-r--r--   0        0        0      670 2024-03-20 16:35:10.769326 ipfabric-6.7.3/ipfabric/models/__init__.py
--rw-r--r--   0        0        0    21981 2024-04-29 16:40:08.950110 ipfabric-6.7.3/ipfabric/models/device.py
--rw-r--r--   0        0        0     7677 2024-03-20 16:35:10.771408 ipfabric-6.7.3/ipfabric/models/intent.py
--rw-r--r--   0        0        0     2796 2023-07-31 14:49:28.275721 ipfabric-6.7.3/ipfabric/models/intent_check.py
--rw-r--r--   0        0        0    10641 2024-03-20 16:35:10.772481 ipfabric-6.7.3/ipfabric/models/inventory.py
--rw-r--r--   0        0        0     5787 2024-03-20 16:35:10.773517 ipfabric-6.7.3/ipfabric/models/jobs.py
--rw-r--r--   0        0        0     4128 2024-03-20 16:35:10.774564 ipfabric-6.7.3/ipfabric/models/oas.py
--rw-r--r--   0        0        0     1888 2024-03-20 16:35:10.774564 ipfabric-6.7.3/ipfabric/models/rbac.py
--rw-r--r--   0        0        0    27927 2024-03-20 16:35:10.775608 ipfabric-6.7.3/ipfabric/models/snapshot.py
--rw-r--r--   0        0        0     5759 2024-03-20 16:35:10.775608 ipfabric-6.7.3/ipfabric/models/snapshots.py
--rw-r--r--   0        0        0    23837 2024-03-20 16:35:10.776646 ipfabric-6.7.3/ipfabric/models/table.py
--rw-r--r--   0        0        0     4145 2024-03-20 16:35:10.777686 ipfabric-6.7.3/ipfabric/models/technology/__init__.py
--rw-r--r--   0        0        0     1504 2024-03-20 16:35:10.778718 ipfabric-6.7.3/ipfabric/models/technology/addressing.py
--rw-r--r--   0        0        0      661 2024-03-20 16:35:10.778718 ipfabric-6.7.3/ipfabric/models/technology/cloud.py
--rw-r--r--   0        0        0     2731 2024-03-20 16:35:10.779749 ipfabric-6.7.3/ipfabric/models/technology/dhcp.py
--rw-r--r--   0        0        0     1315 2024-03-20 16:35:10.780776 ipfabric-6.7.3/ipfabric/models/technology/fhrp.py
--rw-r--r--   0        0        0     8591 2024-03-20 16:35:10.781802 ipfabric-6.7.3/ipfabric/models/technology/interfaces.py
--rw-r--r--   0        0        0      462 2024-03-20 16:35:10.781802 ipfabric-6.7.3/ipfabric/models/technology/ip_telephony.py
--rw-r--r--   0        0        0     1086 2024-03-20 16:35:10.783360 ipfabric-6.7.3/ipfabric/models/technology/load_balancing.py
--rw-r--r--   0        0        0      643 2024-03-20 16:35:10.784362 ipfabric-6.7.3/ipfabric/models/technology/managed_networks.py
--rw-r--r--   0        0        0     7447 2024-03-20 16:35:10.785416 ipfabric-6.7.3/ipfabric/models/technology/management.py
--rw-r--r--   0        0        0     2604 2024-03-20 16:35:10.785466 ipfabric-6.7.3/ipfabric/models/technology/mpls.py
--rw-r--r--   0        0        0     3516 2024-03-20 16:35:10.786534 ipfabric-6.7.3/ipfabric/models/technology/multicast.py
--rw-r--r--   0        0        0     1002 2024-03-20 16:35:10.787589 ipfabric-6.7.3/ipfabric/models/technology/neighbors.py
--rw-r--r--   0        0        0      806 2024-03-20 16:35:10.787589 ipfabric-6.7.3/ipfabric/models/technology/oam.py
--rw-r--r--   0        0        0     4436 2024-03-20 16:35:10.788591 ipfabric-6.7.3/ipfabric/models/technology/platforms.py
--rw-r--r--   0        0        0     1579 2024-03-20 16:35:10.789626 ipfabric-6.7.3/ipfabric/models/technology/port_channels.py
--rw-r--r--   0        0        0     1424 2024-03-20 16:35:10.790651 ipfabric-6.7.3/ipfabric/models/technology/qos.py
--rw-r--r--   0        0        0     6912 2024-03-20 16:35:10.791753 ipfabric-6.7.3/ipfabric/models/technology/routing.py
--rw-r--r--   0        0        0     2962 2024-03-20 16:35:10.791753 ipfabric-6.7.3/ipfabric/models/technology/sdn.py
--rw-r--r--   0        0        0      604 2024-03-20 16:35:10.792841 ipfabric-6.7.3/ipfabric/models/technology/sdwan.py
--rw-r--r--   0        0        0     2620 2024-03-20 16:35:10.793894 ipfabric-6.7.3/ipfabric/models/technology/security.py
--rw-r--r--   0        0        0     2641 2024-03-20 16:35:10.793894 ipfabric-6.7.3/ipfabric/models/technology/stp.py
--rw-r--r--   0        0        0     1134 2024-03-20 16:35:10.794896 ipfabric-6.7.3/ipfabric/models/technology/vlans.py
--rw-r--r--   0        0        0     1145 2024-03-20 16:35:10.795936 ipfabric-6.7.3/ipfabric/models/technology/wireless.py
--rw-r--r--   0        0        0     2409 2024-03-20 16:35:10.795936 ipfabric-6.7.3/ipfabric/models/users.py
--rw-r--r--   0        0        0        0 2024-01-25 18:33:47.048277 ipfabric-6.7.3/ipfabric/oas/__init__.py
--rw-r--r--   0        0        0   326420 2024-03-20 16:35:10.799023 ipfabric-6.7.3/ipfabric/oas/v6.6.json
--rw-r--r--   0        0        0   327148 2024-03-20 16:35:10.801329 ipfabric-6.7.3/ipfabric/oas/v6.7.json
--rw-r--r--   0        0        0     1172 2024-03-20 16:35:10.803997 ipfabric-6.7.3/ipfabric/settings/__init__.py
--rw-r--r--   0        0        0     3641 2024-03-20 16:35:10.805129 ipfabric-6.7.3/ipfabric/settings/api_tokens.py
--rw-r--r--   0        0        0     6751 2024-03-20 16:35:10.806145 ipfabric-6.7.3/ipfabric/settings/attributes.py
--rw-r--r--   0        0        0     9119 2024-03-20 16:35:10.808322 ipfabric-6.7.3/ipfabric/settings/authentication.py
--rw-r--r--   0        0        0     1394 2024-03-20 16:35:10.809455 ipfabric-6.7.3/ipfabric/settings/discovery.py
--rw-r--r--   0        0        0     3266 2024-03-20 16:35:10.810505 ipfabric-6.7.3/ipfabric/settings/local_users.py
--rw-r--r--   0        0        0    14522 2024-03-29 13:49:06.795074 ipfabric-6.7.3/ipfabric/settings/rbac.py
--rw-r--r--   0        0        0     2284 2024-03-20 16:35:10.811555 ipfabric-6.7.3/ipfabric/settings/seeds.py
--rw-r--r--   0        0        0     3137 2024-03-20 16:35:10.812643 ipfabric-6.7.3/ipfabric/settings/settings.py
--rw-r--r--   0        0        0     2102 2024-03-20 16:35:10.813841 ipfabric-6.7.3/ipfabric/settings/site_separation.py
--rw-r--r--   0        0        0     4487 2024-03-20 16:35:10.814866 ipfabric-6.7.3/ipfabric/settings/vendor_api.py
--rw-r--r--   0        0        0     9120 2024-03-20 16:35:10.815971 ipfabric-6.7.3/ipfabric/settings/vendor_api_models.py
--rw-r--r--   0        0        0      644 2024-03-20 16:35:10.817051 ipfabric-6.7.3/ipfabric/tools/__init__.py
--rw-r--r--   0        0        0     8583 2024-03-20 16:35:10.818051 ipfabric-6.7.3/ipfabric/tools/configuration.py
--rw-r--r--   0        0        0     5656 2024-03-20 16:35:10.819099 ipfabric-6.7.3/ipfabric/tools/discovery_history.py
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.819099 ipfabric-6.7.3/ipfabric/tools/managed_rbac/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.820129 ipfabric-6.7.3/ipfabric/tools/managed_rbac/v6/7/__init__.py
--rw-r--r--   0        0        0    37895 2024-03-29 13:49:06.797076 ipfabric-6.7.3/ipfabric/tools/managed_rbac/v6/7/policies.json
--rw-r--r--   0        0        0     3383 2024-03-29 13:49:06.798242 ipfabric-6.7.3/ipfabric/tools/managed_rbac/v6/7/roles.json
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.821154 ipfabric-6.7.3/ipfabric/tools/managed_rbac/v6/__init__.py
--rw-r--r--   0        0        0     4730 2024-01-25 18:33:47.054282 ipfabric-6.7.3/ipfabric/tools/nist.py
--rw-r--r--   0        0        0     6782 2024-03-29 13:49:06.800107 ipfabric-6.7.3/ipfabric/tools/rbac.py
--rw-r--r--   0        0        0     4260 2024-03-20 16:35:10.822260 ipfabric-6.7.3/ipfabric/tools/restore_intents.py
--rw-r--r--   0        0        0    22669 2024-03-20 16:35:10.823261 ipfabric-6.7.3/ipfabric/tools/shared.py
--rw-r--r--   0        0        0     2644 2024-02-07 13:28:55.569790 ipfabric-6.7.3/ipfabric/tools/site_seperation_report.py
--rw-r--r--   0        0        0     2690 2023-12-13 15:03:30.822909 ipfabric-6.7.3/ipfabric/tools/vulnerabilities.py
--rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.7.3/LICENSE
--rw-r--r--   0        0        0     2787 2024-04-29 16:39:30.727537 ipfabric-6.7.3/NOTICES.md
--rw-r--r--   0        0        0     3300 2024-04-29 16:40:08.952111 ipfabric-6.7.3/pyproject.toml
--rw-r--r--   0        0        0     6226 2024-04-29 16:39:30.729045 ipfabric-6.7.3/README.md
--rw-r--r--   0        0        0     8376 1970-01-01 00:00:00.000000 ipfabric-6.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1294 2024-02-21 17:21:14.240240 ipfabric-6.8.0b0/ipfabric/__init__.py
+-rw-r--r--   0        0        0    11041 2024-04-29 16:40:32.514746 ipfabric-6.8.0b0/ipfabric/api.py
+-rw-r--r--   0        0        0    10300 2024-04-29 17:45:57.981047 ipfabric-6.8.0b0/ipfabric/auth.py
+-rw-r--r--   0        0        0    23030 2024-04-29 16:40:32.515823 ipfabric-6.8.0b0/ipfabric/client.py
+-rw-r--r--   0        0        0      693 2024-02-29 12:11:26.623633 ipfabric-6.8.0b0/ipfabric/diagrams/__init__.py
+-rw-r--r--   0        0        0    18216 2024-03-29 13:49:06.793074 ipfabric-6.8.0b0/ipfabric/diagrams/graphs.py
+-rw-r--r--   0        0        0     3625 2024-02-22 21:24:28.609926 ipfabric-6.8.0b0/ipfabric/diagrams/icmp.py
+-rw-r--r--   0        0        0      867 2024-02-29 12:11:26.625974 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/__init__.py
+-rw-r--r--   0        0        0     3808 2024-02-29 12:11:26.627304 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/constants.py
+-rw-r--r--   0        0        0        0 2023-12-13 15:03:30.792953 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/factory_defaults/__init__.py
+-rw-r--r--   0        0        0     5792 2023-12-13 15:03:30.792953 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
+-rw-r--r--   0        0        0     2173 2023-12-13 15:03:30.794172 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
+-rw-r--r--   0        0        0    12911 2024-02-29 12:11:26.628310 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/graph_parameters.py
+-rw-r--r--   0        0        0    13870 2024-02-29 12:11:26.629771 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/graph_settings.py
+-rw-r--r--   0        0        0     5026 2024-02-29 12:11:26.630778 ipfabric-6.8.0b0/ipfabric/diagrams/input_models/shared_view.py
+-rw-r--r--   0        0        0       90 2024-02-29 12:11:26.632075 ipfabric-6.8.0b0/ipfabric/diagrams/output_models/__init__.py
+-rw-r--r--   0        0        0     5241 2024-02-29 12:11:26.633080 ipfabric-6.8.0b0/ipfabric/diagrams/output_models/graph_result.py
+-rw-r--r--   0        0        0     2278 2024-01-25 18:33:47.040766 ipfabric-6.8.0b0/ipfabric/diagrams/output_models/protocols.py
+-rw-r--r--   0        0        0     4556 2024-02-29 12:11:26.634080 ipfabric-6.8.0b0/ipfabric/diagrams/output_models/trace.py
+-rw-r--r--   0        0        0     2283 2024-03-20 16:35:10.768244 ipfabric-6.8.0b0/ipfabric/exceptions.py
+-rw-r--r--   0        0        0      670 2024-03-20 16:35:10.769326 ipfabric-6.8.0b0/ipfabric/models/__init__.py
+-rw-r--r--   0        0        0    21375 2024-04-29 16:47:05.807340 ipfabric-6.8.0b0/ipfabric/models/device.py
+-rw-r--r--   0        0        0     7677 2024-03-20 16:35:10.771408 ipfabric-6.8.0b0/ipfabric/models/intent.py
+-rw-r--r--   0        0        0     2796 2023-07-31 14:49:28.275721 ipfabric-6.8.0b0/ipfabric/models/intent_check.py
+-rw-r--r--   0        0        0    10641 2024-03-20 16:35:10.772481 ipfabric-6.8.0b0/ipfabric/models/inventory.py
+-rw-r--r--   0        0        0     5827 2024-04-29 19:22:26.698442 ipfabric-6.8.0b0/ipfabric/models/jobs.py
+-rw-r--r--   0        0        0     4128 2024-03-20 16:35:10.774564 ipfabric-6.8.0b0/ipfabric/models/oas.py
+-rw-r--r--   0        0        0     1888 2024-03-20 16:35:10.774564 ipfabric-6.8.0b0/ipfabric/models/rbac.py
+-rw-r--r--   0        0        0    27947 2024-04-29 19:17:05.216570 ipfabric-6.8.0b0/ipfabric/models/snapshot.py
+-rw-r--r--   0        0        0     5755 2024-04-29 19:17:05.207890 ipfabric-6.8.0b0/ipfabric/models/snapshots.py
+-rw-r--r--   0        0        0    23837 2024-03-20 16:35:10.776646 ipfabric-6.8.0b0/ipfabric/models/table.py
+-rw-r--r--   0        0        0     4145 2024-03-20 16:35:10.777686 ipfabric-6.8.0b0/ipfabric/models/technology/__init__.py
+-rw-r--r--   0        0        0     1504 2024-03-20 16:35:10.778718 ipfabric-6.8.0b0/ipfabric/models/technology/addressing.py
+-rw-r--r--   0        0        0      661 2024-03-20 16:35:10.778718 ipfabric-6.8.0b0/ipfabric/models/technology/cloud.py
+-rw-r--r--   0        0        0     2731 2024-03-20 16:35:10.779749 ipfabric-6.8.0b0/ipfabric/models/technology/dhcp.py
+-rw-r--r--   0        0        0     1315 2024-03-20 16:35:10.780776 ipfabric-6.8.0b0/ipfabric/models/technology/fhrp.py
+-rw-r--r--   0        0        0     8591 2024-03-20 16:35:10.781802 ipfabric-6.8.0b0/ipfabric/models/technology/interfaces.py
+-rw-r--r--   0        0        0      462 2024-03-20 16:35:10.781802 ipfabric-6.8.0b0/ipfabric/models/technology/ip_telephony.py
+-rw-r--r--   0        0        0     1086 2024-03-20 16:35:10.783360 ipfabric-6.8.0b0/ipfabric/models/technology/load_balancing.py
+-rw-r--r--   0        0        0      643 2024-03-20 16:35:10.784362 ipfabric-6.8.0b0/ipfabric/models/technology/managed_networks.py
+-rw-r--r--   0        0        0     7447 2024-03-20 16:35:10.785416 ipfabric-6.8.0b0/ipfabric/models/technology/management.py
+-rw-r--r--   0        0        0     2604 2024-03-20 16:35:10.785466 ipfabric-6.8.0b0/ipfabric/models/technology/mpls.py
+-rw-r--r--   0        0        0     3516 2024-03-20 16:35:10.786534 ipfabric-6.8.0b0/ipfabric/models/technology/multicast.py
+-rw-r--r--   0        0        0     1002 2024-03-20 16:35:10.787589 ipfabric-6.8.0b0/ipfabric/models/technology/neighbors.py
+-rw-r--r--   0        0        0      806 2024-03-20 16:35:10.787589 ipfabric-6.8.0b0/ipfabric/models/technology/oam.py
+-rw-r--r--   0        0        0     4436 2024-03-20 16:35:10.788591 ipfabric-6.8.0b0/ipfabric/models/technology/platforms.py
+-rw-r--r--   0        0        0     1579 2024-03-20 16:35:10.789626 ipfabric-6.8.0b0/ipfabric/models/technology/port_channels.py
+-rw-r--r--   0        0        0     1424 2024-03-20 16:35:10.790651 ipfabric-6.8.0b0/ipfabric/models/technology/qos.py
+-rw-r--r--   0        0        0     6912 2024-03-20 16:35:10.791753 ipfabric-6.8.0b0/ipfabric/models/technology/routing.py
+-rw-r--r--   0        0        0     2962 2024-03-20 16:35:10.791753 ipfabric-6.8.0b0/ipfabric/models/technology/sdn.py
+-rw-r--r--   0        0        0      604 2024-03-20 16:35:10.792841 ipfabric-6.8.0b0/ipfabric/models/technology/sdwan.py
+-rw-r--r--   0        0        0     2620 2024-03-20 16:35:10.793894 ipfabric-6.8.0b0/ipfabric/models/technology/security.py
+-rw-r--r--   0        0        0     2641 2024-03-20 16:35:10.793894 ipfabric-6.8.0b0/ipfabric/models/technology/stp.py
+-rw-r--r--   0        0        0     1134 2024-03-20 16:35:10.794896 ipfabric-6.8.0b0/ipfabric/models/technology/vlans.py
+-rw-r--r--   0        0        0     1145 2024-03-20 16:35:10.795936 ipfabric-6.8.0b0/ipfabric/models/technology/wireless.py
+-rw-r--r--   0        0        0     2409 2024-03-20 16:35:10.795936 ipfabric-6.8.0b0/ipfabric/models/users.py
+-rw-r--r--   0        0        0        0 2024-01-25 18:33:47.048277 ipfabric-6.8.0b0/ipfabric/oas/__init__.py
+-rw-r--r--   0        0        0   327148 2024-03-20 16:35:10.801329 ipfabric-6.8.0b0/ipfabric/oas/v6.7.json
+-rw-r--r--   0        0        0   390704 2024-04-29 17:19:57.796133 ipfabric-6.8.0b0/ipfabric/oas/v6.8.json
+-rw-r--r--   0        0        0     1172 2024-03-20 16:35:10.803997 ipfabric-6.8.0b0/ipfabric/settings/__init__.py
+-rw-r--r--   0        0        0     3641 2024-03-20 16:35:10.805129 ipfabric-6.8.0b0/ipfabric/settings/api_tokens.py
+-rw-r--r--   0        0        0     7679 2024-04-30 12:35:22.770023 ipfabric-6.8.0b0/ipfabric/settings/attributes.py
+-rw-r--r--   0        0        0     9119 2024-03-20 16:35:10.808322 ipfabric-6.8.0b0/ipfabric/settings/authentication.py
+-rw-r--r--   0        0        0     1394 2024-03-20 16:35:10.809455 ipfabric-6.8.0b0/ipfabric/settings/discovery.py
+-rw-r--r--   0        0        0     3266 2024-03-20 16:35:10.810505 ipfabric-6.8.0b0/ipfabric/settings/local_users.py
+-rw-r--r--   0        0        0    14522 2024-03-29 13:49:06.795074 ipfabric-6.8.0b0/ipfabric/settings/rbac.py
+-rw-r--r--   0        0        0     2284 2024-03-20 16:35:10.811555 ipfabric-6.8.0b0/ipfabric/settings/seeds.py
+-rw-r--r--   0        0        0     3137 2024-03-20 16:35:10.812643 ipfabric-6.8.0b0/ipfabric/settings/settings.py
+-rw-r--r--   0        0        0     2102 2024-03-20 16:35:10.813841 ipfabric-6.8.0b0/ipfabric/settings/site_separation.py
+-rw-r--r--   0        0        0     4487 2024-03-20 16:35:10.814866 ipfabric-6.8.0b0/ipfabric/settings/vendor_api.py
+-rw-r--r--   0        0        0     9192 2024-04-30 12:41:49.057227 ipfabric-6.8.0b0/ipfabric/settings/vendor_api_models.py
+-rw-r--r--   0        0        0      644 2024-03-20 16:35:10.817051 ipfabric-6.8.0b0/ipfabric/tools/__init__.py
+-rw-r--r--   0        0        0     8583 2024-03-20 16:35:10.818051 ipfabric-6.8.0b0/ipfabric/tools/configuration.py
+-rw-r--r--   0        0        0     5656 2024-03-20 16:35:10.819099 ipfabric-6.8.0b0/ipfabric/tools/discovery_history.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.819099 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.820129 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/7/__init__.py
+-rw-r--r--   0        0        0    37895 2024-03-29 13:49:06.797076 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/7/policies.json
+-rw-r--r--   0        0        0     3383 2024-03-29 13:49:06.798242 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/7/roles.json
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.820129 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/8/__init__.py
+-rw-r--r--   0        0        0    37983 2024-04-29 17:29:33.012935 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/8/policies.json
+-rw-r--r--   0        0        0     3383 2024-03-29 13:49:06.798242 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/8/roles.json
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.821154 ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/__init__.py
+-rw-r--r--   0        0        0     4730 2024-01-25 18:33:47.054282 ipfabric-6.8.0b0/ipfabric/tools/nist.py
+-rw-r--r--   0        0        0     6782 2024-03-29 13:49:06.800107 ipfabric-6.8.0b0/ipfabric/tools/rbac.py
+-rw-r--r--   0        0        0     4260 2024-03-20 16:35:10.822260 ipfabric-6.8.0b0/ipfabric/tools/restore_intents.py
+-rw-r--r--   0        0        0    22669 2024-03-20 16:35:10.823261 ipfabric-6.8.0b0/ipfabric/tools/shared.py
+-rw-r--r--   0        0        0     2644 2024-02-07 13:28:55.569790 ipfabric-6.8.0b0/ipfabric/tools/site_seperation_report.py
+-rw-r--r--   0        0        0     2690 2023-12-13 15:03:30.822909 ipfabric-6.8.0b0/ipfabric/tools/vulnerabilities.py
+-rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.8.0b0/LICENSE
+-rw-r--r--   0        0        0     3469 2024-04-29 16:40:32.512687 ipfabric-6.8.0b0/NOTICES.md
+-rw-r--r--   0        0        0     3336 2024-05-01 15:35:30.792374 ipfabric-6.8.0b0/pyproject.toml
+-rw-r--r--   0        0        0     6227 2024-04-29 16:40:32.513685 ipfabric-6.8.0b0/README.md
+-rw-r--r--   0        0        0     8377 1970-01-01 00:00:00.000000 ipfabric-6.8.0b0/PKG-INFO
```

### Comparing `ipfabric-6.7.3/ipfabric/__init__.py` & `ipfabric-6.8.0b0/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/api.py` & `ipfabric-6.8.0b0/ipfabric/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from dataclasses import InitVar, field
 from functools import cached_property
 from typing import Dict
 from typing import Optional, Any, Union, Literal, List, Mapping, OrderedDict, Iterator
-from warnings import warn
 
 from dotenv import find_dotenv
 from httpx import Client, BaseTransport, URL, Response
 from httpx._client import EventHook
 from httpx._types import CertTypes, VerifyTypes
 from pydantic import ConfigDict, Field, InstanceOf
 from pydantic.dataclasses import dataclass
@@ -50,17 +49,14 @@
     )
     api_version: Optional[str] = Field(None, description="Defaults to SDK or API version.")
     snapshot_id: Optional[str] = Field(None, description="Defaults to '$last'.")
     auth: InitVar[Optional[Any]] = field(default=None)
     unloaded: bool = Field(False, description="Default False, do not load unloaded snapshot metadata.")
     env_file: InitVar[Optional[str]] = field(default=None)
     streaming: bool = Field(True, description="Default True; use streaming results instead of pagination.")
-    token: InitVar[Optional[str]] = field(default=None)
-    username: InitVar[Optional[str]] = field(default=None)
-    password: InitVar[Optional[str]] = field(default=None)
     verify: InitVar[Optional[VerifyTypes]] = field(default=None)
     timeout: InitVar[Optional[Union[TimeoutTypes, Literal["DEFAULT"]]]] = field(default="DEFAULT")
     proxy: InitVar[Optional[ProxyTypes]] = field(default=None)
     proxies: InitVar[Optional[ProxiesTypes]] = field(default=None)
     mounts: InitVar[Optional[Mapping[str, Optional[BaseTransport]]]] = field(default=None)
     cert: InitVar[Optional[CertTypes]] = field(default=None)
     event_hooks: InitVar[Optional[Mapping[str, List[EventHook]]]] = field(default=None)
@@ -76,46 +72,28 @@
     _user: Optional[User] = None
     _snapshots: Optional[Snapshots] = None
 
     def __post_init__(
         self,
         auth,
         env_file,
-        token,
-        username,
-        password,
         verify,
         timeout,
         proxy,
         proxies,
         mounts,
         cert,
         event_hooks,
         http2,
     ):
-        if token or (username and password):  # TODO: Remove v6.8
-            warn(
-                "`token=''` or `username='', password=''` authentication will be deprecated in v6.8.0.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-            logger.warning(
-                "Use of `token='<TOKEN>'` or `username='<USER>', password='<PASS>'` authentication will be deprecated "
-                "in v6.8.0, please use `auth='<TOKEN>'` or `auth=('<USER>','<PASS>')` instead.\n"
-                "This does not apply to .env file or environment variables (IPF_TOKEN, IPF_USERNAME, IPF_PASSWORD).\n"
-                "This is to support custom authentication methods that will be passed directly to HTTPX."
-            )
         setup = Setup(
             base_url=self.base_url,
             api_version=self.api_version,
             auth=auth,
             _env_file=env_file if env_file else find_dotenv(usecwd=True),
-            token=token,
-            username=username,
-            password=password,
             snapshot_id=self.snapshot_id,
             verify=verify,
             timeout=timeout,
             proxy=proxy,
             proxies=proxies,
             mounts=mounts,
             cert=cert,
```

### Comparing `ipfabric-6.7.3/ipfabric/auth.py` & `ipfabric-6.8.0b0/ipfabric/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,36 +37,37 @@
 
     def auth_flow(self, request: Request) -> Generator[Request, Response, None]:
         request.headers["X-API-Token"] = self._auth_header
         yield request
 
 
 class AccessToken(Auth):
-    def __init__(self, cookie_jar: CookieJar, username: str, password: str, base_url: URL):
+    def __init__(self, cookie_jar: CookieJar, username: str, password: str, base_url: URL, verify: VerifyTypes):
         self.cookie_jar = cookie_jar
-        self._login(username, password, base_url)
+        self._login(username, password, base_url, verify)
 
     def auth_flow(self, request: Request) -> Generator[Request, Response, None]:
         response = yield request
 
         if response.status_code == 401:
             response.read()
             if "API_EXPIRED_ACCESS_TOKEN" in response.text:
                 # Use refreshToken in Cookies to get new accessToken
                 resp = post(response.url.join("/api/auth/token"), cookies=self.cookie_jar)
                 resp.raise_for_status()  # Response updates accessToken in shared CookieJar
                 request.headers["Cookie"] = "accessToken=" + resp.cookies["accessToken"]  # Update request
                 yield request
         return response
 
-    def _login(self, username: str, password: str, base_url: URL) -> None:
+    def _login(self, username: str, password: str, base_url: URL, verify: VerifyTypes) -> None:
         resp = post(
             base_url.join("auth/login"),
             json=dict(username=username, password=password),
             cookies=self.cookie_jar,
+            verify=verify,
         )
         resp.raise_for_status()
 
 
 class MyInitSettingsSource(InitSettingsSource):
     def __init__(self, settings_cls, init_kwargs: Dict[str, Any]):
         timeout = init_kwargs.pop("timeout", "DEFAULT")
@@ -139,21 +140,21 @@
         self.api_version, self.os_version = self.check_version()
         self.base_url = self.base_url.join(f"api/{self.api_version}/")
         self.client.base_url = self.base_url
         if self.auth:
             if isinstance(self.auth, str):
                 self.client.auth = TokenAuth(self.auth)
             elif isinstance(self.auth, tuple):
-                self.client.auth = AccessToken(self._cookie_jar, self.auth[0], self.auth[1], self.base_url)
+                self.client.auth = AccessToken(self._cookie_jar, self.auth[0], self.auth[1], self.base_url, self.verify)
             else:
                 self.client.auth = self.auth
         elif self.token:
             self.client.auth = TokenAuth(self.token)
         elif self.username and self.password:
-            self.client.auth = AccessToken(self._cookie_jar, self.username, self.password, self.base_url)
+            self.client.auth = AccessToken(self._cookie_jar, self.username, self.password, self.base_url, self.verify)
 
     @property
     def update_attrs(self) -> dict:
         return {
             "base_url": self.base_url,
             "api_version": self.api_version,
             "_os_version": self.os_version,
```

### Comparing `ipfabric-6.7.3/ipfabric/client.py` & `ipfabric-6.8.0b0/ipfabric/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import re
 from json import loads, dumps
 from typing import Optional, Any, Union, Literal, List, Dict, overload
-from warnings import warn
 
 from httpx import InvalidURL, URL
 from pydantic import ConfigDict
 from pydantic.dataclasses import dataclass
 
 from ipfabric.api import IPFabricAPI
 from ipfabric.diagrams import Diagram
@@ -209,19 +208,14 @@
             data = self._ipf_pager(url, payload)
         elif data is False:
             res = self.post(url, json=payload)
             res.raise_for_status()
             data = res.json()["data"]
         return data
 
-    def _get_columns(self, url: str):  # TODO: Remove in v6.8
-        warn("This method will be removed in v6.8, please use `get_columns`.", DeprecationWarning, stacklevel=2)
-        logger.warning("This method will be removed in v6.8, please use `get_columns`.")
-        return self.get_columns(url=url)
-
     def get_columns(self, url: str, ui: bool = False) -> List[str]:
         """Checks OAS to find available columns.
 
         Args:
             url: API url to post
             ui: True to return columns available in the UI, default False
```

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/__init__.py` & `ipfabric-6.8.0b0/ipfabric/diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/graphs.py` & `ipfabric-6.8.0b0/ipfabric/diagrams/graphs.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/icmp.py` & `ipfabric-6.8.0b0/ipfabric/diagrams/icmp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/input_models/__init__.py` & `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/input_models/constants.py` & `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/constants.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json` & `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json` & `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/input_models/graph_parameters.py` & `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/graph_parameters.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/input_models/graph_settings.py` & `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/graph_settings.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/input_models/shared_view.py` & `ipfabric-6.8.0b0/ipfabric/diagrams/input_models/shared_view.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/output_models/graph_result.py` & `ipfabric-6.8.0b0/ipfabric/diagrams/output_models/graph_result.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/output_models/protocols.py` & `ipfabric-6.8.0b0/ipfabric/diagrams/output_models/protocols.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/diagrams/output_models/trace.py` & `ipfabric-6.8.0b0/ipfabric/diagrams/output_models/trace.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/exceptions.py` & `ipfabric-6.8.0b0/ipfabric/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/__init__.py` & `ipfabric-6.8.0b0/ipfabric/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/device.py` & `ipfabric-6.8.0b0/ipfabric/models/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,28 @@
 from ipaddress import IPv4Interface
 from collections import defaultdict
 from case_insensitive_dict import CaseInsensitiveDict
 from ipfabric.models.technology import Technology
 from ipfabric.tools.shared import create_filter
 
 from pydantic import BaseModel, Field, PrivateAttr
-from ipfabric.exceptions import deprecated_args_decorator
 
 logger = logging.getLogger("ipfabric")
 
 
 class DeviceConfig(BaseModel):
     status: str
     current: Optional[str] = Field(None, alias="currentConfig")
     start: Optional[str] = Field(None, alias="startupConfig")
 
 
 class Device(BaseModel):
     client: Optional[Any] = Field(None, exclude=True)
-    attributes: Optional[dict] = None
-    global_attributes: Optional[dict] = None
+    attributes: Optional[dict] = Field(default_factory=dict)
+    global_attributes: Optional[dict] = Field(default_factory=dict)
     domain: Optional[str] = None
     family: Optional[str] = None
     fqdn: Optional[str] = None
     hostname: str
     image: Optional[str] = None
     model: Optional[str] = None
     platform: Optional[str] = None
@@ -82,84 +81,72 @@
     def __eq__(self, other):
         return self.sn == other.sn if isinstance(other, Device) else str(other)
 
     def __hash__(self):
         return hash(self.sn)
 
     @property
-    def technology(self):
+    def technology(self) -> Technology:
         return Technology(client=self.client, sn=self.sn)
 
     @property
-    def site(self):
+    def site(self) -> str:
         return self.site_name
 
     @property
-    def local_attributes(self):
+    def local_attributes(self) -> dict:
         return self.attributes
 
     @classmethod
     def check_attribute(cls, attribute) -> True:
         if attribute not in cls.model_fields:
             raise AttributeError(f"Attribute {attribute} not in Device class.")
         return True
 
-    @deprecated_args_decorator(version="6.8.0")
-    def get_log_file(self, **kwargs) -> str:
+    def get_log_file(self) -> str:
         res = self.client.get("/os/logs/task/" + self.task_key)
         res.raise_for_status()
         return res.text
 
-    @deprecated_args_decorator(version="6.8.0")
-    def get_config(self, **kwargs) -> Union[None, DeviceConfig]:
+    def get_config(self) -> Union[None, DeviceConfig]:
         if not self.blob_key:
             logger.warning("Device Config not in Snapshot File. Please try using ipfabric.tools.DeviceConfigs")
             return None
         res = self.client.get("blobs/device-configuration/" + str(self.blob_key))
         res.raise_for_status()
         return DeviceConfig(**res.json())
 
-    @deprecated_args_decorator(version="6.8.0")
-    def interfaces(self, **kwargs) -> list:
+    def interfaces(self) -> list:
         return self.fetch_all("tables/inventory/interfaces")
 
-    @deprecated_args_decorator(version="6.8.0")
-    def pn(self, **kwargs) -> list:
+    def pn(self) -> list:
         return self.fetch_all("tables/inventory/pn")
 
-    @deprecated_args_decorator(version="6.8.0")
-    def switchport(self, **kwargs) -> list:
+    def switchport(self) -> list:
         return self.fetch_all("tables/interfaces/switchports")
 
-    @deprecated_args_decorator(version="6.8.0")
-    def managed_ip_ipv4(self, **kwargs) -> list:
+    def managed_ip_ipv4(self) -> list:
         return self.fetch_all("tables/addressing/managed-devs")
 
-    @deprecated_args_decorator(version="6.8.0")
-    def managed_ip_ipv6(self, **kwargs) -> list:
+    def managed_ip_ipv6(self) -> list:
         return self.fetch_all("tables/addressing/ipv6-managed-devs")
 
-    @deprecated_args_decorator(version="6.8.0")
-    def mac_table(self, **kwargs) -> list:
+    def mac_table(self) -> list:
         return self.fetch_all("tables/addressing/mac")
 
-    @deprecated_args_decorator(version="6.8.0")
-    def arp_table(self, **kwargs) -> list:
+    def arp_table(self) -> list:
         return self.fetch_all("tables/addressing/arp")
 
-    @deprecated_args_decorator(version="6.8.0")
-    def routes_ipv4(self, **kwargs) -> list:
+    def routes_ipv4(self) -> list:
         return self.fetch_all("tables/networks/routes")
 
-    @deprecated_args_decorator(version="6.8.0")
-    def routes_ipv6(self, **kwargs) -> list:
+    def routes_ipv6(self) -> list:
         return self.fetch_all("tables/networks/ipv6-routes")
 
-    @deprecated_args_decorator(version="6.8.0")
-    def neighbors_all(self, **kwargs) -> list:
+    def neighbors_all(self) -> list:
         return self.fetch_all("tables/neighbors/all")
 
     def trigger_backup(self):
         return self.client.trigger_backup(sn=self.sn)
 
     @overload
     def fetch_all(
@@ -240,14 +227,17 @@
 class DeviceDict(CaseInsensitiveDict):
     """CaseInsensitiveDict with functions to search or regex on dictionary keys."""
 
     def __init__(self, attribute, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.attribute = attribute
 
+    def __getitem__(self, key) -> Device:
+        return super().__getitem__(key)
+
     @staticmethod
     def _new_dict(a):
         return DeviceDict(attribute=a) if a == "sn" else DeviceDict(attribute=a)
 
     @overload
     def regex(self: DeviceDict[str, List[Device]], pattern: str, *flags: int) -> DeviceDict[str, List[Device]]: ...
```

### Comparing `ipfabric-6.7.3/ipfabric/models/intent.py` & `ipfabric-6.8.0b0/ipfabric/models/intent.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/intent_check.py` & `ipfabric-6.8.0b0/ipfabric/models/intent_check.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/inventory.py` & `ipfabric-6.8.0b0/ipfabric/models/inventory.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/jobs.py` & `ipfabric-6.8.0b0/ipfabric/models/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 SNAP_JOBS = {
     "load": "snapshotLoad",
     "unload": "snapshotUnload",
     "download": "snapshotDownload",
     "add": "discoveryAdd",
     "refresh": "discoveryRefresh",
     "delete": "deleteDevice",
+    "recalculate": "recalculateSites",
 }
 
 SNAP_ACTIONS = Literal["load", "unload", "download", "add", "refresh", "delete"]
 
 
 class Jobs(BaseModel):
     client: Any = Field(exclude=True)
```

### Comparing `ipfabric-6.7.3/ipfabric/models/oas.py` & `ipfabric-6.8.0b0/ipfabric/models/oas.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/rbac.py` & `ipfabric-6.8.0b0/ipfabric/models/rbac.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/snapshot.py` & `ipfabric-6.8.0b0/ipfabric/models/snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,32 +210,33 @@
 
     def _check_load_status(
         self,
         ts: int,
         wait_for_assurance: bool = True,
         timeout: int = 60,
         retry: int = 5,
+        action: str = 'load',
     ):
         load_job = self._jobs.check_snapshot_job(
-            self.snapshot_id, started=ts, action="load", timeout=timeout, retry=retry
+            self.snapshot_id, started=ts, action=action, timeout=timeout, retry=retry
         )
         if load_job and wait_for_assurance:
             return self._check_assurance_status(load_job["startedAt"], timeout, retry)
         elif not load_job:
             logger.error("Snapshot Load did not complete.")
             return False
         return True
 
     def _check_assurance_status(
         self,
         ts: int,
         timeout: int = 60,
         retry: int = 5,
     ):
-        ae_settings = self.get_assurance_engine_settings(self.client)
+        ae_settings = self.get_assurance_engine_settings()
         ae_status = False
         if ae_settings:
             ae_status = self._jobs.check_snapshot_assurance_jobs(
                 self.snapshot_id, ae_settings, started=ts, timeout=timeout, retry=retry
             )
             if not ae_status:
                 logger.error("Assurance Engine tasks did not complete")
```

### Comparing `ipfabric-6.7.3/ipfabric/models/snapshots.py` & `ipfabric-6.8.0b0/ipfabric/models/snapshots.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             results = self.client._ipf_pager("tables/management/snapshots", payload)
             if not results:
                 logger.error(f"Snapshot {snapshot_id} not found.")
                 return None
             get_results = self._get_snapshots()
             snapshot = self._create_snapshot_model(results[0], get_results)
             if snapshot.loaded:
-                snapshot.get_assurance_engine_settings(self)
+                snapshot.get_assurance_engine_settings()
             return snapshot
 
     def _create_snapshot_model(self, s, get_results):
         return Snapshot(
             client=self.client,
             **s,
             licensedDevCount=get_results[s["id"]].get("licensedDevCount", None),
```

### Comparing `ipfabric-6.7.3/ipfabric/models/table.py` & `ipfabric-6.8.0b0/ipfabric/models/table.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/__init__.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/addressing.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/addressing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/cloud.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/cloud.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/dhcp.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/dhcp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/fhrp.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/fhrp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/interfaces.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/interfaces.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/load_balancing.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/load_balancing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/managed_networks.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/managed_networks.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/management.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/management.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/mpls.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/mpls.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/multicast.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/multicast.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/neighbors.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/neighbors.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/oam.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/oam.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/platforms.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/platforms.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/port_channels.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/port_channels.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/qos.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/qos.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/routing.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/routing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/sdn.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/sdn.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/sdwan.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/sdwan.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/security.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/security.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/stp.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/stp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/vlans.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/vlans.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/technology/wireless.py` & `ipfabric-6.8.0b0/ipfabric/models/technology/wireless.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/models/users.py` & `ipfabric-6.8.0b0/ipfabric/models/users.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/oas/v6.6.json` & `ipfabric-6.8.0b0/ipfabric/oas/v6.7.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967572942974693%*

 * *Differences: {"'os/feature-flags'": "OrderedDict([('api_endpoint', '/os/feature-flags'), ('get', "*

 * *                       "OrderedDict([('api_endpoint', 'os/feature-flags'), ('method', 'get'), "*

 * *                       "('web_endpoint', None), ('columns', None), ('nested_columns', None), "*

 * *                       "('ui_columns', None), ('api_scope_id', "*

 * *                       "'1e216fd89041a5faf71e2e15c349ffedcd7aaef9'), ('summary', 'Return enabled "*

 * *                       "feature flags'), ('description', 'Returns objec […]*

```diff
@@ -1225,14 +1225,32 @@
             "ui_columns": null,
             "web_endpoint": null
         },
         "patch": null,
         "post": null,
         "put": null
     },
+    "os/feature-flags": {
+        "api_endpoint": "/os/feature-flags",
+        "delete": null,
+        "get": {
+            "api_endpoint": "os/feature-flags",
+            "api_scope_id": "1e216fd89041a5faf71e2e15c349ffedcd7aaef9",
+            "columns": null,
+            "description": "Returns object of enabled feature flags",
+            "method": "get",
+            "nested_columns": null,
+            "summary": "Return enabled feature flags",
+            "ui_columns": null,
+            "web_endpoint": null
+        },
+        "patch": null,
+        "post": null,
+        "put": null
+    },
     "os/generate-nimpee-cert": {
         "api_endpoint": "/os/generate-nimpee-cert",
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "os/generate-nimpee-cert",
@@ -3247,21 +3265,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/aci/dtep",
             "api_scope_id": "1e59228ef7e29180ad59f674a5069f708374daff",
             "columns": [
                 "siteName",
-                "hostname",
+                "type",
+                "id",
+                "dtepIp",
                 "sn",
                 "encap",
                 "role",
-                "dtepIp",
-                "type",
-                "id"
+                "hostname"
             ],
             "description": "IS-IS Dynamic Tunnel End Point inventory",
             "method": "post",
             "nested_columns": [
                 "type"
             ],
             "summary": "DTEP Inventory",
@@ -3282,31 +3300,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/aci/endpoints",
             "api_scope_id": "8377957b155db2db2fe4fdde54bba5a645e84612",
             "columns": [
-                "group",
-                "ipFlags",
+                "vrf",
                 "siteName",
+                "vrfVnid",
+                "encapId",
+                "group",
+                "id",
+                "mac",
                 "hostname",
-                "intName",
-                "vlanId",
-                "bdVnid",
                 "sn",
-                "vrf",
+                "ipFlags",
                 "macFlags",
-                "encapId",
+                "vlanId",
+                "vlanVnid",
                 "ip",
+                "bdVnid",
                 "encapType",
-                "vlanVnid",
-                "mac",
-                "id",
-                "vrfVnid"
+                "intName"
             ],
             "description": "Application Centric Infrastructure (ACI) endpoints inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "ACI Endpoint",
             "ui_columns": [
                 "hostname",
@@ -3334,26 +3352,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/aci/vlan",
             "api_scope_id": "521712216816bf6ffe1260cf9a8040adb3e341dd",
             "columns": [
-                "hwId",
-                "encapVlanId",
+                "bdVlanId",
                 "siteName",
-                "hostname",
-                "vlanId",
-                "sn",
+                "encapVlanId",
                 "vlanType",
-                "endpointCount",
+                "id",
                 "encapVlanType",
+                "endpointCount",
                 "fabricVxlanId",
-                "bdVlanId",
-                "id"
+                "sn",
+                "vlanId",
+                "hwId",
+                "hostname"
             ],
             "description": "Application Centric Infrastructure (ACI) VLANs inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "ACI VLAN",
             "ui_columns": [
                 "hostname",
@@ -3376,24 +3394,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/aci/vrf",
             "api_scope_id": "8800985b8f133246c0f03b4b3a3031ca625e6945",
             "columns": [
-                "contextId",
-                "vrfType",
-                "siteName",
-                "hostname",
-                "sn",
+                "vrfVxlanId",
                 "vrf",
+                "siteName",
+                "id",
+                "vrfType",
                 "endpointCount",
-                "vrfVxlanId",
-                "status",
-                "id"
+                "sn",
+                "contextId",
+                "hostname",
+                "status"
             ],
             "description": "Application Centric Infrastructure (ACI) virtual routing and forwarding instances inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "ACI VRF",
             "ui_columns": [
                 "hostname",
@@ -3415,24 +3433,24 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/arp",
             "api_scope_id": "22bb05c6b1f06bce692dd02f7113e0c944bae4ec",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
+                "id",
                 "proxy",
+                "vendor",
                 "sn",
+                "vlanId",
+                "intName",
+                "mac",
                 "vrf",
-                "vendor",
-                "ip",
-                "id",
-                "mac"
+                "hostname",
+                "ip"
             ],
             "description": "Address Resolution Protocol (ARP) collected fromt the network",
             "method": "post",
             "nested_columns": [],
             "summary": "ARP Table",
             "ui_columns": [
                 "hostname",
@@ -3454,19 +3472,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/duplicate-ip",
             "api_scope_id": "b57f0159953704683e4c6dbcb52fbf2c9ae4a657",
             "columns": [
-                "hostname",
-                "countIntUp",
-                "ip",
                 "id",
-                "count"
+                "countIntUp",
+                "count",
+                "hostname",
+                "ip"
             ],
             "description": "Duplicate IP adresses detected in the network",
             "method": "post",
             "nested_columns": [],
             "summary": "Duplicate IP",
             "ui_columns": [
                 "ip",
@@ -3483,27 +3501,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/hosts",
             "api_scope_id": "dd3e429da6bbb78f01b1a694d04b12a623e97cb6",
             "columns": [
-                "type",
+                "gateways",
                 "siteName",
-                "edges",
-                "accessPoints",
                 "vlan",
-                "dnsName",
-                "gateways",
-                "vrf",
+                "type",
+                "accessPoints",
+                "id",
                 "vendor",
-                "ip",
-                "uniqId",
                 "mac",
-                "id"
+                "edges",
+                "ip",
+                "vrf",
+                "dnsName",
+                "uniqId"
             ],
             "description": "Detected IPv4 users, hosts, and endpoints from discovered gateways",
             "method": "post",
             "nested_columns": [
                 "accessPoints",
                 "edges",
                 "gateways",
@@ -3531,25 +3549,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/ipv6-hosts",
             "api_scope_id": "80ba0a1528bd80b1b6235610789c3e36b9663e20",
             "columns": [
-                "siteName",
-                "edges",
-                "uniqId",
                 "gateways",
+                "siteName",
                 "vlan",
+                "type",
+                "id",
+                "ipv6",
+                "edges",
+                "mac",
                 "vrf",
                 "vendor",
-                "ipv6",
-                "id",
-                "type",
-                "mac"
+                "uniqId"
             ],
             "description": "Detected IPv6 users, hosts, and endpoints from discovered gateways",
             "method": "post",
             "nested_columns": [
                 "edges",
                 "gateways",
                 "type"
@@ -3575,26 +3593,26 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/ipv6-managed-devs",
             "api_scope_id": "adfde3593455992b53ceba8013eece37ea60c172",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
+                "stateL2",
+                "type",
+                "id",
                 "net",
                 "sn",
-                "vrf",
                 "stateL1",
-                "ip",
-                "stateL2",
-                "id",
-                "type",
-                "mac"
+                "vlanId",
+                "intName",
+                "mac",
+                "vrf",
+                "hostname",
+                "ip"
             ],
             "description": "IPv6 addressess configured on network interfaces",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed IPv6 addresses",
             "ui_columns": [
                 "hostname",
@@ -3619,24 +3637,24 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/ipv6-neighbors",
             "api_scope_id": "2c64d326d8d979b9084e63cb21021a8680693d4e",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
+                "id",
+                "ipv6",
                 "proxy",
+                "vendor",
                 "sn",
+                "vlanId",
+                "mac",
                 "vrf",
-                "vendor",
-                "ipv6",
-                "id",
-                "mac"
+                "hostname",
+                "intName"
             ],
             "description": "Neighbors detected with IPv6 neighbor discovery",
             "method": "post",
             "nested_columns": [],
             "summary": "IPv6 Neighbor discovery",
             "ui_columns": [
                 "hostname",
@@ -3658,29 +3676,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/mac",
             "api_scope_id": "a97aa4c973ddef344684436badc40fa5fd6d5e2b",
             "columns": [
-                "fabricPath",
                 "siteName",
-                "hostname",
-                "intName",
-                "vxlans",
                 "vlan",
-                "user",
+                "type",
+                "id",
                 "vni",
-                "sn",
                 "edge",
+                "source",
+                "sn",
+                "user",
                 "vendor",
-                "id",
-                "type",
+                "vxlans",
                 "mac",
-                "source"
+                "hostname",
+                "intName",
+                "fabricPath"
             ],
             "description": "Cumulative MAC address table",
             "method": "post",
             "nested_columns": [
                 "vxlans"
             ],
             "summary": "MAC Table",
@@ -3708,30 +3726,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/managed-devs",
             "api_scope_id": "d11dae27159ec2f8ad49b5ff3793346760547326",
             "columns": [
-                "dnsHostnameMatch",
-                "type",
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
-                "dnsReverseMatch",
-                "dnsName",
-                "sn",
-                "vrf",
-                "stateL1",
-                "ip",
                 "stateL2",
+                "type",
+                "dnsHostnameMatch",
+                "id",
                 "net",
                 "mac",
-                "id"
+                "sn",
+                "stateL1",
+                "vlanId",
+                "dnsReverseMatch",
+                "intName",
+                "ip",
+                "vrf",
+                "hostname",
+                "dnsName"
             ],
             "description": "Inventory of IP addresses configured on every managed network device",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed IPv4 addresses",
             "ui_columns": [
                 "hostname",
@@ -3758,17 +3776,17 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/path-lookup-first-hops",
             "api_scope_id": "b40b73f5f323984b20fae87347eceb5ee5d06359",
             "columns": [
-                "interfaces",
                 "sn",
-                "hostname"
+                "hostname",
+                "interfaces"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "interfaces"
             ],
             "summary": "POST /tables/addressing/path-lookup-first-hops",
@@ -3786,17 +3804,17 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/path-lookup-sources",
             "api_scope_id": "1dd5bc8efdd6c32a73ccb9cf9a40008a44662fa3",
             "columns": [
-                "dnsName",
                 "ip",
-                "id"
+                "id",
+                "dnsName"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/addressing/path-lookup-sources",
             "ui_columns": [
                 "id",
@@ -3812,20 +3830,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/path-lookup-sources-multicast",
             "api_scope_id": "e0c56ce09d5a8df4c115ef86691cf4dc05099bde",
             "columns": [
-                "dnsName",
-                "type",
                 "ip",
-                "id"
+                "id",
+                "dnsName",
+                "type"
             ],
-            "description": null,
+            "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/addressing/path-lookup-sources-multicast",
             "ui_columns": [
                 "id",
                 "dnsName",
                 "ip",
@@ -3840,19 +3858,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/path-lookup-sources-unicast",
             "api_scope_id": "08aa6e53a501e070c2941a182d7b6ffc72003179",
             "columns": [
-                "dnsName",
                 "ip",
-                "id"
+                "id",
+                "dnsName"
             ],
-            "description": null,
+            "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/addressing/path-lookup-sources-unicast",
             "ui_columns": [
                 "id",
                 "dnsName",
                 "ip"
@@ -3866,21 +3884,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/applications",
             "api_scope_id": "a2539bd51c8d19aeb19678f0a7fbb9997379861f",
             "columns": [
-                "apiUrl",
-                "endpointGroupsCount",
-                "name",
                 "slug",
                 "tenant",
                 "id",
-                "priority"
+                "priority",
+                "name",
+                "endpointGroupsCount",
+                "apiUrl"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) applications inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "APIC Applications",
             "ui_columns": [
                 "apiUrl",
@@ -3899,24 +3917,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/bridge-domains",
             "api_scope_id": "6c44dbdbc71937871ada66f59fcca23c4b83131a",
             "columns": [
-                "scope",
-                "apiUrl",
-                "pcTag",
-                "name",
+                "slug",
+                "tenant",
                 "vrfName",
                 "subnets",
-                "slug",
                 "type",
-                "tenant",
-                "id"
+                "id",
+                "pcTag",
+                "name",
+                "apiUrl",
+                "scope"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) bridge-domains inventory",
             "method": "post",
             "nested_columns": [
                 "subnets"
             ],
             "summary": "APIC Bridge Domains",
@@ -3940,23 +3958,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/contexts",
             "api_scope_id": "26bf59496c1aed1763b8d2eec18a9ce6323f2d1a",
             "columns": [
-                "isUnenforced",
-                "scope",
-                "apiUrl",
+                "slug",
+                "tenant",
+                "id",
                 "pcTag",
                 "name",
+                "isUnenforced",
                 "bridgeDomainsCount",
-                "slug",
-                "tenant",
-                "id"
+                "apiUrl",
+                "scope"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) contexts inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "APIC Contexts",
             "ui_columns": [
                 "apiUrl",
@@ -3977,26 +3995,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/contracts",
             "api_scope_id": "32009950f96b207cb23f48d6bb6aea004fffa677",
             "columns": [
-                "subjectName",
-                "contractName",
-                "consumerMatch",
-                "providerMatch",
                 "apiUrl",
-                "subjectFilters",
-                "serviceGraph",
-                "hasReverseFilterPorts",
                 "slug",
-                "contractScope",
                 "tenant",
-                "id"
+                "contractName",
+                "hasReverseFilterPorts",
+                "id",
+                "subjectFilters",
+                "contractScope",
+                "subjectName",
+                "providerMatch",
+                "consumerMatch",
+                "serviceGraph"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) contracts inventory'",
             "method": "post",
             "nested_columns": [
                 "subjectFilters"
             ],
             "summary": "APIC Contracts",
@@ -4023,22 +4041,22 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/controllers",
             "api_scope_id": "30ba8f81ceeb27989a0b15429c02b89bf50dea1b",
             "columns": [
                 "siteName",
-                "hostname",
-                "apiUrl",
-                "health",
-                "sn",
-                "name",
                 "ipv6Addresses",
+                "id",
+                "name",
+                "sn",
                 "ipAddresses",
-                "id"
+                "health",
+                "hostname",
+                "apiUrl"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) controllers inventory",
             "method": "post",
             "nested_columns": [
                 "ipAddresses",
                 "ipv6Addresses"
             ],
@@ -4061,25 +4079,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/endpoint-groups",
             "api_scope_id": "00e8efe24aeb7068affad09141dc91ffb0ddeb82",
             "columns": [
+                "slug",
+                "tenant",
                 "appName",
+                "isPreferredGroupMember",
+                "subnets",
+                "id",
                 "contractsCount",
-                "scope",
-                "apiUrl",
                 "pcTag",
                 "name",
-                "subnets",
-                "isPreferredGroupMember",
-                "slug",
-                "tenant",
-                "id"
+                "apiUrl",
+                "scope"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) endpoint-groups inventory",
             "method": "post",
             "nested_columns": [
                 "subnets"
             ],
             "summary": "Endpoint Groups",
@@ -4104,22 +4122,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/endpoint-groups/contracts",
             "api_scope_id": "e3e7838393599ff81d47a268fe05f96589fef66f",
             "columns": [
-                "appName",
-                "endpointGroupName",
-                "apiUrl",
-                "name",
                 "slug",
-                "type",
                 "tenant",
-                "id"
+                "appName",
+                "type",
+                "id",
+                "name",
+                "endpointGroupName",
+                "apiUrl"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) groups and associated contracts inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Endpoint Groups - Contracts",
             "ui_columns": [
                 "apiUrl",
@@ -4139,24 +4157,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/service-graphs",
             "api_scope_id": "0648458a01e6306ee2073026755a069597e66b82",
             "columns": [
-                "nodeName",
-                "functionType",
-                "apiUrl",
-                "device",
-                "name",
                 "functionTemplateType",
                 "slug",
-                "state",
                 "tenant",
-                "id"
+                "functionType",
+                "device",
+                "id",
+                "state",
+                "name",
+                "nodeName",
+                "apiUrl"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) Service Graphs",
             "method": "post",
             "nested_columns": [],
             "summary": "APIC Service Graphs",
             "ui_columns": [
                 "apiUrl",
@@ -4178,16 +4196,16 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/attributes/filters/keys",
             "api_scope_id": "6e4ae537964e8c367154a6d9c18b94364535fcd6",
             "columns": [
-                "keyName",
-                "id"
+                "id",
+                "keyName"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/attributes/filters/keys",
             "ui_columns": [
                 "id",
@@ -4202,17 +4220,17 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/attributes/filters/values",
             "api_scope_id": "e4451c800dbc427892d0966f1c820d051a5c157d",
             "columns": [
-                "value",
+                "id",
                 "keyName",
-                "id"
+                "value"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/attributes/filters/values",
             "ui_columns": [
                 "id",
@@ -4228,19 +4246,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/attributes/graphs",
             "api_scope_id": "5ca7fa1061686eb1a61f6ee42853a87db19d4011",
             "columns": [
-                "label",
-                "name",
                 "layout",
+                "id",
+                "name",
                 "path",
-                "id"
+                "label"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/attributes/graphs",
             "ui_columns": [
                 "id",
@@ -4258,16 +4276,16 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/attributes/settings/keys",
             "api_scope_id": "efa97310d5316b63bda987235c76a21fe91a8b34",
             "columns": [
-                "keyName",
-                "id"
+                "id",
+                "keyName"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/attributes/settings/keys",
             "ui_columns": [
                 "id",
@@ -4282,17 +4300,17 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/attributes/settings/values",
             "api_scope_id": "2f9242273faa847abbff98d212ad716aa8cd8975",
             "columns": [
-                "value",
+                "id",
                 "keyName",
-                "id"
+                "value"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/attributes/settings/values",
             "ui_columns": [
                 "id",
@@ -4308,19 +4326,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/attributes/summary",
             "api_scope_id": "3a5ed41ba4bfd6e5789905185b7accdb3039617a",
             "columns": [
-                "label",
-                "name",
                 "layout",
+                "id",
+                "name",
                 "path",
-                "id"
+                "label"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/attributes/summary",
             "ui_columns": [
                 "id",
@@ -4338,24 +4356,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/cloud/virtual-machines",
             "api_scope_id": "845ee1f3eeb63f6daabff1c11d5cfb1330eda9e1",
             "columns": [
-                "os",
+                "slug",
+                "image",
                 "siteName",
-                "hostname",
-                "sn",
-                "name",
                 "numberOfInterfaces",
-                "status",
-                "slug",
                 "id",
-                "image"
+                "name",
+                "os",
+                "sn",
+                "hostname",
+                "status"
             ],
             "description": "Public or private cloud virtual machines",
             "method": "post",
             "nested_columns": [],
             "summary": "Virtual Machines",
             "ui_columns": [
                 "hostname",
@@ -4376,28 +4394,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/cloud/virtual-machines-interfaces",
             "api_scope_id": "6ae9e708aaad8029584abab2d39014caef632261",
             "columns": [
+                "slug",
                 "siteName",
-                "hostname",
-                "intName",
-                "vmIntName",
+                "ipv6Addresses",
                 "vmName",
-                "sn",
+                "vmIntId",
+                "vmIntName",
                 "outAcl",
-                "ipv6Addresses",
-                "slug",
+                "id",
+                "sn",
                 "ipAddresses",
-                "inAcl",
-                "vmIntId",
                 "mac",
-                "id"
+                "inAcl",
+                "hostname",
+                "intName"
             ],
             "description": "Public or private cloud virtual machines interfaces",
             "method": "post",
             "nested_columns": [
                 "ipAddresses",
                 "ipv6Addresses",
                 "inAcl",
@@ -4427,33 +4445,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/received",
             "api_scope_id": "b05678b196ad2944a184f09d48042ffefbec040a",
             "columns": [
-                "siteName",
-                "sn",
-                "release",
-                "bootReply",
-                "ack",
-                "relayed",
-                "discover",
-                "bootRequest",
                 "total",
-                "hostname",
+                "id",
+                "bootRequest",
                 "dropped",
-                "request",
                 "nak",
+                "discover",
                 "received",
-                "decline",
-                "sent",
+                "hostname",
+                "release",
+                "request",
+                "ack",
+                "sn",
+                "bootReply",
                 "offer",
                 "inform",
-                "id"
+                "siteName",
+                "relayed",
+                "decline",
+                "sent"
             ],
             "description": "DHCP relay global statistics - received messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Global statistics - received",
             "ui_columns": [
                 "hostname",
@@ -4479,33 +4497,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/relayed",
             "api_scope_id": "1b26c6a2c608fc547040f5756b9ccd042fad1c48",
             "columns": [
-                "siteName",
-                "sn",
-                "release",
-                "bootReply",
-                "ack",
-                "relayed",
-                "discover",
-                "bootRequest",
                 "total",
-                "hostname",
+                "id",
+                "bootRequest",
                 "dropped",
-                "request",
                 "nak",
+                "discover",
                 "received",
-                "decline",
-                "sent",
+                "hostname",
+                "release",
+                "request",
+                "ack",
+                "sn",
+                "bootReply",
                 "offer",
                 "inform",
-                "id"
+                "siteName",
+                "relayed",
+                "decline",
+                "sent"
             ],
             "description": "DHCP relay global statistics - relayed messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Global statistics - Relayed",
             "ui_columns": [
                 "hostname",
@@ -4531,33 +4549,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/sent",
             "api_scope_id": "5eac1ba680f1f318a577ac4b184961323746dcad",
             "columns": [
-                "siteName",
-                "sn",
-                "release",
-                "bootReply",
-                "ack",
-                "relayed",
-                "discover",
-                "bootRequest",
                 "total",
-                "hostname",
+                "id",
+                "bootRequest",
                 "dropped",
-                "request",
                 "nak",
+                "discover",
                 "received",
-                "decline",
-                "sent",
+                "hostname",
+                "release",
+                "request",
+                "ack",
+                "sn",
+                "bootReply",
                 "offer",
                 "inform",
-                "id"
+                "siteName",
+                "relayed",
+                "decline",
+                "sent"
             ],
             "description": "DHCP relay global statistics - sent messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Global statistics - Sent",
             "ui_columns": [
                 "hostname",
@@ -4584,21 +4602,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/summary",
             "api_scope_id": "07d758f84c68ea84bcb21ca3411fb77db96f5b48",
             "columns": [
                 "siteName",
-                "hostname",
+                "id",
+                "sn",
                 "dropped",
+                "relayed",
                 "received",
-                "sn",
                 "sent",
-                "relayed",
-                "id"
+                "hostname"
             ],
             "description": "DHCP relay global statistics summary",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Global stats summary",
             "ui_columns": [
                 "hostname",
@@ -4617,30 +4635,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces",
             "api_scope_id": "b15866e556186706040db812bc17b82300e74890",
             "columns": [
+                "proxyOptions",
                 "siteName",
-                "hostname",
-                "intName",
-                "dropped",
+                "id",
                 "proxy",
-                "received",
                 "sn",
                 "name",
-                "vrf",
+                "dropped",
+                "received",
+                "options",
+                "relayed",
                 "sent",
                 "ip",
-                "relayed",
-                "proxyOptions",
-                "strategy",
-                "id",
-                "options"
+                "vrf",
+                "hostname",
+                "intName",
+                "strategy"
             ],
             "description": "DHCP relay interfaces inventory",
             "method": "post",
             "nested_columns": [
                 "options",
                 "proxyOptions"
             ],
@@ -4670,30 +4688,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces-stats/received",
             "api_scope_id": "71f56607fadf9778d20720b921d885c8eb4adfe0",
             "columns": [
-                "siteName",
-                "hostname",
-                "intName",
                 "total",
+                "siteName",
+                "nak",
+                "id",
+                "bootRequest",
+                "discover",
+                "ack",
+                "request",
                 "sn",
+                "bootReply",
                 "decline",
-                "bootRequest",
-                "release",
                 "offer",
-                "bootReply",
+                "release",
+                "hostname",
                 "inform",
-                "discover",
-                "request",
-                "ack",
-                "id",
-                "nak"
+                "intName"
             ],
             "description": "DHCP relay interfaces statistics - received messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Interfaces stats - Received",
             "ui_columns": [
                 "hostname",
@@ -4720,30 +4738,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces-stats/relayed",
             "api_scope_id": "59dc994dd10fd6a2759645e5fbd3e0b68213ebcc",
             "columns": [
-                "siteName",
-                "hostname",
-                "intName",
                 "total",
+                "siteName",
+                "nak",
+                "id",
+                "bootRequest",
+                "discover",
+                "ack",
+                "request",
                 "sn",
+                "bootReply",
                 "decline",
-                "bootRequest",
-                "release",
                 "offer",
-                "bootReply",
+                "release",
+                "hostname",
                 "inform",
-                "discover",
-                "request",
-                "ack",
-                "id",
-                "nak"
+                "intName"
             ],
             "description": "DHCP relay interfaces statistics - relayed messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Interfaces stats - Relayed",
             "ui_columns": [
                 "hostname",
@@ -4770,30 +4788,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces-stats/sent",
             "api_scope_id": "25ba9479038c2644d62f38ff4b4ac9f9b8b8370a",
             "columns": [
-                "siteName",
-                "hostname",
-                "intName",
                 "total",
+                "siteName",
+                "nak",
+                "id",
+                "bootRequest",
+                "discover",
+                "ack",
+                "request",
                 "sn",
+                "bootReply",
                 "decline",
-                "bootRequest",
-                "release",
                 "offer",
-                "bootReply",
+                "release",
+                "hostname",
                 "inform",
-                "discover",
-                "request",
-                "ack",
-                "id",
-                "nak"
+                "intName"
             ],
             "description": "DHCP relay interfaces statistics - sent messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Interfaces stats - Sent",
             "ui_columns": [
                 "hostname",
@@ -4820,21 +4838,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/excluded-ranges",
             "api_scope_id": "99d16794d1d2f025f1cd8f2d04da13b4edf0dae1",
             "columns": [
-                "serverId",
                 "siteName",
-                "hostname",
-                "sn",
                 "range",
+                "id",
                 "serverName",
-                "id"
+                "sn",
+                "hostname",
+                "serverId"
             ],
             "description": "DHCP server excluded ranges inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Server Excluded Ranges",
             "ui_columns": [
                 "hostname",
@@ -4851,21 +4869,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/interfaces",
             "api_scope_id": "3e0a61543fd85e7d14dca2b7bc33966a81a20e22",
             "columns": [
-                "serverId",
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
+                "id",
                 "serverName",
-                "id"
+                "sn",
+                "hostname",
+                "serverId",
+                "intName"
             ],
             "description": "DHCP server interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Server Interfaces",
             "ui_columns": [
                 "hostname",
@@ -4882,27 +4900,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/leases",
             "api_scope_id": "df053403d81a055d9dacd6ca83ce379a320233ab",
             "columns": [
-                "serverId",
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
-                "vrf",
-                "leaseExpiration",
+                "type",
                 "client",
-                "ip",
+                "id",
                 "state",
+                "leaseExpiration",
                 "serverName",
-                "type",
-                "id"
+                "sn",
+                "intName",
+                "vrf",
+                "hostname",
+                "serverId",
+                "ip"
             ],
             "description": "DHCP Server ",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Server Leases",
             "ui_columns": [
                 "hostname",
@@ -4925,27 +4943,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/pools",
             "api_scope_id": "0272de31f9cc4b2eb99c98019662373ad313eb72",
             "columns": [
-                "rangeOptions",
-                "serverId",
+                "rangeUsage",
                 "siteName",
-                "hostname",
+                "range",
+                "id",
+                "rangeType",
+                "rangeOptions",
+                "poolOptions",
+                "serverName",
                 "sn",
                 "name",
                 "vrf",
-                "rangeType",
-                "rangeUsage",
-                "range",
-                "serverName",
-                "poolOptions",
-                "id"
+                "hostname",
+                "serverId"
             ],
             "description": "DHCP Server pools inventory",
             "method": "post",
             "nested_columns": [
                 "poolOptions",
                 "rangeOptions"
             ],
@@ -4972,22 +4990,22 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/summary",
             "api_scope_id": "5bd9af227930616f4b790a7a4495e1c2a5607f64",
             "columns": [
                 "siteName",
-                "excludedRangesCount",
-                "hostname",
+                "leasesCount",
+                "id",
                 "poolsCount",
-                "sn",
-                "intNamesCount",
                 "serverName",
-                "id",
-                "leasesCount"
+                "sn",
+                "excludedRangesCount",
+                "hostname",
+                "intNamesCount"
             ],
             "description": "DHCP server summary information inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Server Summary",
             "ui_columns": [
                 "hostname",
@@ -5009,20 +5027,20 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/balancing",
             "api_scope_id": "9a13e4af94cf0b36dd961fbe07635442b812eb5d",
             "columns": [
                 "nei2",
                 "virtIp",
-                "nei1Sn",
-                "pct",
-                "vrf",
                 "nei1",
+                "id",
                 "nei2Sn",
-                "id"
+                "nei1Sn",
+                "vrf",
+                "pct"
             ],
             "description": "Balancing ratios for FHRP gateways",
             "method": "post",
             "nested_columns": [],
             "summary": "Active FHRP gateway balancing",
             "ui_columns": [
                 "nei1",
@@ -5040,25 +5058,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/glbp-forwarders",
             "api_scope_id": "e43daff2e67dcbd8f3dc23d0c0da851041b439d6",
             "columns": [
+                "siteName",
+                "active",
                 "group",
+                "id",
+                "state",
+                "sn",
                 "address",
-                "siteName",
+                "vrf",
                 "hostname",
                 "intName",
-                "sn",
-                "vrf",
-                "forwarder",
-                "active",
-                "state",
-                "id"
+                "forwarder"
             ],
             "description": "GLBP forwarders inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "GLBP forwarders",
             "ui_columns": [
                 "hostname",
@@ -5080,21 +5098,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/group-members",
             "api_scope_id": "8dde2c05e424950eabfe4c1f3d96f8c31cfa68d7",
             "columns": [
-                "virtualIp",
-                "virtualIpv6",
+                "devices",
+                "id",
+                "protocol",
                 "count",
+                "virtualIpv6",
                 "vrf",
-                "protocol",
-                "id",
-                "devices"
+                "virtualIp"
             ],
             "description": "HSRP/VRRP/GLBP Group members - gateway inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "HSRP/VRRP/GLBP Group members",
             "ui_columns": [
                 "virtualIp",
@@ -5113,32 +5131,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/group-state",
             "api_scope_id": "a93fab66e04c9ec69c28f3c780afe0faf0a40b1d",
             "columns": [
-                "group",
-                "virtualIp",
-                "virtualIpv6",
-                "siteName",
-                "hostname",
-                "intName",
-                "secondaryVirtualIpAddresses",
-                "standby",
-                "preempt",
-                "sn",
                 "vrf",
+                "siteName",
                 "active",
+                "group",
+                "id",
+                "priority",
+                "state",
                 "version",
                 "protocol",
-                "state",
-                "id",
+                "sn",
+                "virtualIpv6",
                 "count",
-                "priority"
+                "secondaryVirtualIpAddresses",
+                "preempt",
+                "hostname",
+                "standby",
+                "intName",
+                "virtualIp"
             ],
             "description": "HSRP/VRRP/GLBP Group State - detailed gateway inventory",
             "method": "post",
             "nested_columns": [
                 "secondaryVirtualIpAddresses"
             ],
             "summary": "HSRP/VRRP/GLBP Group State",
@@ -5170,18 +5188,18 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/stproot-alignment",
             "api_scope_id": "3bfd2b41fc7a20ee62a7bd41514b8f1619ef0a48",
             "columns": [
                 "siteName",
-                "hostname",
-                "sn",
                 "id",
+                "sn",
                 "count",
+                "hostname",
                 "vlans"
             ],
             "description": "Misaligned FHRP Gateways with STP Root",
             "method": "post",
             "nested_columns": [],
             "summary": "FHRP Gateway and STP Root Aligment",
             "ui_columns": [
@@ -5199,26 +5217,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/virtual-gateways",
             "api_scope_id": "1a71450017c72c31e8f659137c654bfd155f02ce",
             "columns": [
-                "virtualIp",
-                "virtualIpv6",
                 "siteName",
-                "hostname",
-                "intName",
+                "type",
+                "id",
+                "state",
+                "protocol",
                 "sn",
-                "vrf",
                 "virtualMac",
-                "protocol",
-                "state",
-                "type",
-                "id"
+                "virtualIpv6",
+                "vrf",
+                "hostname",
+                "intName",
+                "virtualIp"
             ],
             "description": "Virtual gateways inventory for Arista VARP",
             "method": "post",
             "nested_columns": [],
             "summary": "Arista VARP",
             "ui_columns": [
                 "hostname",
@@ -5241,19 +5259,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/global-attributes",
             "api_scope_id": "6190fa52f1dc472252730653d5b3f51aadc3c2b0",
             "columns": [
-                "hostname",
-                "sn",
-                "name",
                 "id",
-                "value"
+                "name",
+                "sn",
+                "value",
+                "hostname"
             ],
             "description": "Global attributes inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Global Attributes",
             "ui_columns": [
                 "id",
@@ -5271,25 +5289,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/connectivity-matrix",
             "api_scope_id": "a3137fc62a0e223ff0361957fb4b2b1f14ced97e",
             "columns": [
-                "localInt",
+                "localMedia",
                 "siteName",
-                "remoteMedia",
+                "id",
                 "remoteInt",
-                "remoteSn",
-                "localMedia",
+                "localInt",
                 "remoteHost",
                 "localHost",
                 "protocol",
-                "localSn",
-                "id"
+                "remoteSn",
+                "remoteMedia",
+                "localSn"
             ],
             "description": "Logical and physical connectivity matrix for variety of protocols",
             "method": "post",
             "nested_columns": [],
             "summary": "Connectivity matrix",
             "ui_columns": [
                 "localHost",
@@ -5310,35 +5328,38 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/connectivity-matrix/unmanaged-neighbors/detail",
             "api_scope_id": "bdc9d74ab378e68c5b0afa3604ad661aead4a70a",
             "columns": [
-                "localAddress",
-                "hostname",
-                "intName",
                 "siteName",
-                "subnet",
-                "sn",
-                "protocol",
+                "neiIpV6",
+                "localAddress",
+                "id",
                 "devType",
+                "localAddressV6",
                 "neiIp",
-                "id",
-                "source"
+                "protocol",
+                "sn",
+                "source",
+                "hostname",
+                "subnet",
+                "intName"
             ],
             "description": "Details for unmanaged neighbors detected via variety of protocols",
             "method": "post",
             "nested_columns": [],
             "summary": "Unmanaged Neighbors Detail",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "intName",
                 "neiIp",
+                "neiIpV6",
                 "protocol"
             ],
             "web_endpoint": "/technology/interfaces/connectivity-matrix/unmanaged-neighbors-detail"
         },
         "put": null
     },
     "tables/interfaces/connectivity-matrix/unmanaged-neighbors/summary": {
@@ -5346,44 +5367,46 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/connectivity-matrix/unmanaged-neighbors/summary",
             "api_scope_id": "50778eb92b26f715d12e836feb43136450a1ba6b",
             "columns": [
-                "xdpNeiCount",
-                "siteName",
-                "neighbor",
-                "sn",
+                "id",
+                "ipv6",
+                "ospfNeiCount",
                 "capabilities",
-                "ripNeiCount",
-                "eigrpNeiCount",
-                "ldpNeiCount",
-                "ip",
                 "cefPrfx",
-                "isisNeiCount",
-                "bgpNeiCount",
-                "bgpNeiAsn",
+                "ldpNeiCount",
                 "hostname",
                 "bgpReceivedPfx",
+                "isisNeiCount",
+                "bgpNeiAsn",
+                "sn",
                 "cefNeiCount",
-                "ospfNeiCount",
+                "eigrpNeiCount",
+                "xdpNeiCount",
+                "ip",
+                "siteName",
+                "ripNeiCount",
+                "neighbor",
                 "ospfv3NeiCount",
-                "id"
+                "bgpNeiCount"
             ],
             "description": "Summary for unmanaged neighbors detected via variety of protocols",
             "method": "post",
             "nested_columns": [
                 "capabilities"
             ],
             "summary": "Unmanaged Neighbors Summary",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "ip",
+                "ipv6",
                 "capabilities",
                 "bgpNeiCount",
                 "bgpNeiAsn",
                 "bgpReceivedPfx",
                 "xdpNeiCount",
                 "cefNeiCount",
                 "cefPrfx",
@@ -5403,31 +5426,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/counters/inbound",
             "api_scope_id": "9585e835675c9a6833b98059cdd94b3b10f3877e",
             "columns": [
-                "inGiants",
-                "inNoBuffer",
-                "hostname",
-                "inBytes",
-                "intName",
                 "inMcast",
+                "inBytes",
+                "inErr",
+                "inNoBuffer",
                 "siteName",
-                "inStompedCrc",
+                "inBcast",
+                "id",
+                "inGiants",
+                "inDrops",
+                "inCrc",
                 "inPkts",
-                "inRunts",
                 "sn",
-                "inCrc",
                 "inOverrun",
-                "inErr",
-                "inDrops",
-                "id",
-                "inBcast"
+                "inRunts",
+                "inStompedCrc",
+                "hostname",
+                "intName"
             ],
             "description": "Interfaces inbound counters - absolute values",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Counters - Inbound",
             "ui_columns": [
                 "hostname",
@@ -5455,32 +5478,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/counters/outbound",
             "api_scope_id": "8feb39afbeda7b063265225dcd0f0ac460f7d992",
             "columns": [
-                "outBytes",
                 "siteName",
-                "hostname",
-                "intName",
-                "outBabble",
-                "outDrops",
-                "outErr",
-                "outLateCollisions",
-                "sn",
                 "outCollisions",
-                "outMcast",
-                "outBufferDrop",
-                "outLostCarrier",
                 "outDeferred",
-                "outPkts",
-                "outNoCarrier",
+                "outErr",
                 "id",
-                "outBcast"
+                "outLostCarrier",
+                "outBufferDrop",
+                "sn",
+                "outDrops",
+                "outNoCarrier",
+                "outPkts",
+                "outBytes",
+                "outBcast",
+                "outLateCollisions",
+                "outMcast",
+                "hostname",
+                "intName",
+                "outBabble"
             ],
             "description": "Interfaces outbound counters - absolute values",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Counters - Oubound",
             "ui_columns": [
                 "hostname",
@@ -5510,22 +5533,22 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/bidirectional",
             "api_scope_id": "55d36efb15d823453e640a21479e832131ce9afe",
             "columns": [
                 "siteName",
-                "hostname",
-                "dropsRate",
+                "bytesRate",
+                "id",
                 "dropsPktsPct",
-                "intName",
                 "sn",
                 "impactDrops",
-                "bytesRate",
-                "id"
+                "dropsRate",
+                "hostname",
+                "intName"
             ],
             "description": "Input and Output interface drops combined providing a bidirectional view of drops on an interface",
             "method": "post",
             "nested_columns": [],
             "summary": "Bidirectional Interface Drops",
             "ui_columns": [
                 "hostname",
@@ -5546,21 +5569,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/bidirectional-device",
             "api_scope_id": "d450e0e8e4f75918fc478c05898c951fca66e293",
             "columns": [
                 "siteName",
-                "hostname",
-                "dropsRate",
+                "bytesRate",
+                "id",
                 "dropsPktsPct",
                 "sn",
                 "impactDrops",
-                "bytesRate",
-                "id"
+                "dropsRate",
+                "hostname"
             ],
             "description": "Input and Output drops of all interfaces on a device combined proviing a per-device view of bidirectional interface drops",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Bidirectional Interface Drops",
             "ui_columns": [
                 "hostname",
@@ -5579,23 +5602,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/inbound",
             "api_scope_id": "c12f0e948f78f3ad7c859768b1874f0187fa9e7f",
             "columns": [
-                "siteName",
-                "hostname",
-                "intName",
-                "inDropsRate",
-                "sn",
                 "inDropsPktsPct",
+                "inDropsRate",
+                "siteName",
+                "id",
                 "inImpactDrops",
+                "sn",
+                "hostname",
                 "inBytesRate",
-                "id"
+                "intName"
             ],
             "description": "Input interface drops represent packet loss caused by input buffer overflow",
             "method": "post",
             "nested_columns": [],
             "summary": "Inbound Interface Drops",
             "ui_columns": [
                 "hostname",
@@ -5615,22 +5638,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/inbound-device",
             "api_scope_id": "c38e8e6b75840aef445c1ebcccbc471b6767fd19",
             "columns": [
-                "siteName",
-                "hostname",
-                "inDropsRate",
-                "sn",
                 "inDropsPktsPct",
+                "inDropsRate",
+                "siteName",
+                "id",
                 "inImpactDrops",
-                "inBytesRate",
-                "id"
+                "sn",
+                "hostname",
+                "inBytesRate"
             ],
             "description": "Input drops of all interfaces on a device combined providing a per-device view of input interface drops",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Inbound Interface Drops",
             "ui_columns": [
                 "hostname",
@@ -5649,23 +5672,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/outbound",
             "api_scope_id": "17fbfe82210952b858a2cd2daddf7430aeafa502",
             "columns": [
+                "outDropsPktsPct",
                 "siteName",
-                "hostname",
-                "intName",
-                "outImpactDrops",
+                "id",
                 "outBytesRate",
                 "sn",
                 "outDropsRate",
-                "outDropsPktsPct",
-                "id"
+                "outImpactDrops",
+                "hostname",
+                "intName"
             ],
             "description": "Output interface drops represent outbound packet loss",
             "method": "post",
             "nested_columns": [],
             "summary": "Outbound Interface Drops",
             "ui_columns": [
                 "hostname",
@@ -5685,22 +5708,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/outbound-device",
             "api_scope_id": "cf72f642a249e5a614a1eb798f672840e42311e9",
             "columns": [
+                "outDropsPktsPct",
                 "siteName",
-                "hostname",
-                "outImpactDrops",
+                "id",
                 "outBytesRate",
                 "sn",
                 "outDropsRate",
-                "outDropsPktsPct",
-                "id"
+                "outImpactDrops",
+                "hostname"
             ],
             "description": "Output drops of all interfaces on a device combined providing a per-device view of output interface drops",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Outbound Interface Drops",
             "ui_columns": [
                 "hostname",
@@ -5719,26 +5742,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/duplex",
             "api_scope_id": "a1ccbb224b7191ef8c2b1c65ad28c2a3b2777ff6",
             "columns": [
-                "siteName",
-                "remoteMedia",
+                "localMedia",
                 "remoteIntName",
+                "siteName",
+                "id",
                 "localIntName",
+                "localHostname",
                 "remoteSn",
                 "remoteHostname",
-                "localMedia",
+                "localDuplex",
+                "remoteMedia",
                 "localSn",
                 "status",
-                "localHostname",
-                "localDuplex",
-                "id",
                 "remoteDuplex"
             ],
             "description": "Interface connectivity matrix including duplex information",
             "method": "post",
             "nested_columns": [],
             "summary": "Duplex interface matrix",
             "ui_columns": [
@@ -5762,23 +5785,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/bidirectional",
             "api_scope_id": "2cb7ec9e5e7c1354dc90b89a34497489148908f0",
             "columns": [
-                "errRate",
-                "siteName",
-                "hostname",
-                "intName",
                 "errPktsPct",
-                "sn",
+                "siteName",
                 "bytesRate",
+                "id",
+                "sn",
                 "impactErr",
-                "id"
+                "errRate",
+                "hostname",
+                "intName"
             ],
             "description": "Sum of inbound and outbound interface error impacts to provide a bidirectional view of overall impact of errors on an interface",
             "method": "post",
             "nested_columns": [],
             "summary": "Bidirectional Interface Errors",
             "ui_columns": [
                 "hostname",
@@ -5798,22 +5821,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/bidirectional-device",
             "api_scope_id": "da6bd6dabe772a333a496b2f1f29e4160020f2ca",
             "columns": [
-                "errRate",
-                "siteName",
-                "hostname",
                 "errPktsPct",
-                "sn",
+                "siteName",
                 "bytesRate",
+                "id",
+                "sn",
                 "impactErr",
-                "id"
+                "errRate",
+                "hostname"
             ],
             "description": "Bidirectional Input and Output errors of all interfaces on each device combined providing a per-device Impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Bidirectional Interface Errors",
             "ui_columns": [
                 "hostname",
@@ -5833,19 +5856,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/disabled",
             "api_scope_id": "44dbf28ae5ee9173b282db75edcf43abbb2d7baa",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
                 "errorReason",
-                "id"
+                "id",
+                "sn",
+                "hostname",
+                "intName"
             ],
             "description": "Interfaces in the network which has been automatically disabled due to an error",
             "method": "post",
             "nested_columns": [],
             "summary": "Error-Disabled interfaces",
             "ui_columns": [
                 "hostname",
@@ -5862,23 +5885,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/inbound",
             "api_scope_id": "468742fac6ba3687fe28cb1e4a6080d98dfeecb9",
             "columns": [
+                "inErrPktsPct",
                 "siteName",
-                "hostname",
+                "id",
                 "inErrRate",
-                "intName",
                 "sn",
-                "inErrPktsPct",
                 "inImpactErr",
+                "hostname",
                 "inBytesRate",
-                "id"
+                "intName"
             ],
             "description": "Input interface errors represent packet loss caused by input buffer overflow",
             "method": "post",
             "nested_columns": [],
             "summary": "Inbound Interface Errors",
             "ui_columns": [
                 "hostname",
@@ -5898,22 +5921,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/inbound-device",
             "api_scope_id": "ee8e51dfbce7c1bfb1980988d36f80f42a101a16",
             "columns": [
+                "inErrPktsPct",
                 "siteName",
-                "hostname",
+                "id",
                 "inErrRate",
                 "sn",
-                "inErrPktsPct",
                 "inImpactErr",
-                "inBytesRate",
-                "id"
+                "hostname",
+                "inBytesRate"
             ],
             "description": "Input errors of all interfaces on a device combined providing a per-device view of input interface errors",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Inbound Interface Errors",
             "ui_columns": [
                 "hostname",
@@ -5934,21 +5957,21 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/outbound",
             "api_scope_id": "f8e2d3777206f652f3941d24ab28bd764fe64d67",
             "columns": [
                 "outErrPktsPct",
                 "siteName",
-                "hostname",
-                "intName",
-                "outErrRate",
+                "id",
                 "outBytesRate",
-                "sn",
                 "outImpactErr",
-                "id"
+                "sn",
+                "outErrRate",
+                "hostname",
+                "intName"
             ],
             "description": "Output interface errors represent outbound packet loss",
             "method": "post",
             "nested_columns": [],
             "summary": "Outbound Interface Errors",
             "ui_columns": [
                 "hostname",
@@ -5970,20 +5993,20 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/outbound-device",
             "api_scope_id": "f50046c5c6c9803ae0e34b04d6219f54b9f7b846",
             "columns": [
                 "outErrPktsPct",
                 "siteName",
-                "hostname",
-                "outErrRate",
+                "id",
                 "outBytesRate",
-                "sn",
                 "outImpactErr",
-                "id"
+                "sn",
+                "outErrRate",
+                "hostname"
             ],
             "description": "Output errors of all interfaces on a device combined providing a per-device view of output interface errors",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Outbound Interface Errors",
             "ui_columns": [
                 "hostname",
@@ -6003,19 +6026,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/inconsistencies/details",
             "api_scope_id": "40d00675840b09d377ec2d55e4263a0361cfa2d1",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
+                "id",
                 "sn",
-                "id"
+                "vlanId",
+                "hostname",
+                "intName"
             ],
             "description": "VLANs that are not configured in any STP instance - detailed view",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs without STP instance - Detail",
             "ui_columns": [
                 "hostname",
@@ -6032,19 +6055,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/inconsistencies/summary",
             "api_scope_id": "66e774e452a0de72bffcbc2edb91bc5dcbd69230",
             "columns": [
-                "vlanCount",
-                "hostname",
                 "siteName",
+                "id",
+                "vlanCount",
                 "sn",
-                "id"
+                "hostname"
             ],
             "description": "VLANs that are not configured in any STP instance - summary view",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs without STP instance - Summary",
             "ui_columns": [
                 "hostname",
@@ -6061,21 +6084,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/load/bidirectional",
             "api_scope_id": "1803e43ebe8097525694112dd415016689a11322",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "pkts",
-                "bytes",
                 "sn",
-                "interval",
-                "id"
+                "hostname",
+                "bytes",
+                "intName",
+                "interval"
             ],
             "description": "Interfaces Bidirectional load inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Bidirectional load",
             "ui_columns": [
                 "hostname",
@@ -6094,22 +6117,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/load/inbound",
             "api_scope_id": "f13e3c4d12edc78761d9e77ac745fe56396ea422",
             "columns": [
-                "siteName",
-                "hostname",
                 "inBytes",
-                "intName",
+                "siteName",
+                "id",
                 "inPkts",
                 "sn",
-                "interval",
-                "id"
+                "hostname",
+                "intName",
+                "interval"
             ],
             "description": "Interfaces inbound load inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Inbound load",
             "ui_columns": [
                 "hostname",
@@ -6128,22 +6151,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/load/outbound",
             "api_scope_id": "6cb01cc705e980dec5a6ec78ba3a411fb0a50021",
             "columns": [
-                "outBytes",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "sn",
-                "interval",
                 "outPkts",
-                "id"
+                "outBytes",
+                "hostname",
+                "intName",
+                "interval"
             ],
             "description": "Interfaces outbound load inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Outbound load",
             "ui_columns": [
                 "hostname",
@@ -6162,25 +6185,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/mtu",
             "api_scope_id": "872798e56e1c263fed7403c72f8a22003fd986a7",
             "columns": [
-                "dstSn",
                 "srcDev",
                 "siteName",
+                "layer",
+                "dstMtu",
                 "srcMtu",
-                "dstDev",
-                "dstInt",
+                "id",
                 "srcInt",
-                "dstMtu",
-                "layer",
                 "srcSn",
-                "id"
+                "dstInt",
+                "dstSn",
+                "dstDev"
             ],
             "description": "Interface connectivity matrix including Maximum Transmission Unit (MTU) information",
             "method": "post",
             "nested_columns": [],
             "summary": "Maximum Transmission Unit Matrix",
             "ui_columns": [
                 "srcDev",
@@ -6202,23 +6225,23 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/port-channel/balance/inbound",
             "api_scope_id": "8dca3d9008c4106fd0ffb84fc81c5ce955059444",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "rate",
-                "sn",
-                "members",
+                "variance",
+                "id",
                 "ratios",
                 "protocol",
-                "id",
-                "variance"
+                "sn",
+                "rate",
+                "hostname",
+                "intName",
+                "members"
             ],
             "description": "Link Aggregation (LAG)/PortChannel/EtherChannel inbound balancing ratios",
             "method": "post",
             "nested_columns": [],
             "summary": "Port Link-Aggregation inbound",
             "ui_columns": [
                 "hostname",
@@ -6240,23 +6263,23 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/port-channel/balance/outbound",
             "api_scope_id": "f2c6640a91ce438523e14c42a3a979260923aec1",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "rate",
-                "sn",
-                "members",
+                "variance",
+                "id",
                 "ratios",
                 "protocol",
-                "id",
-                "variance"
+                "sn",
+                "rate",
+                "hostname",
+                "intName",
+                "members"
             ],
             "description": "Link Aggregation (LAG)/PortChannel/EtherChannel outbound balancing ratios",
             "method": "post",
             "nested_columns": [],
             "summary": "Port Link-Aggregation Outbound",
             "ui_columns": [
                 "hostname",
@@ -6278,21 +6301,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/port-channel/member-status",
             "api_scope_id": "af69f8a8b7ef9551dd624d74504a71c00a821e90",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
-                "members",
+                "id",
                 "mlagId",
                 "protocol",
-                "id"
+                "sn",
+                "hostname",
+                "intName",
+                "members"
             ],
             "description": "State of each link-aggregation member for all configured Link Aggregation (LAG)/PortChannels/EtherChannels",
             "method": "post",
             "nested_columns": [],
             "summary": "Port Link-Aggregation Member Status",
             "ui_columns": [
                 "hostname",
@@ -6311,23 +6334,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/pppoe",
             "api_scope_id": "8e8ccbd7823eab1014e0d1f4d649558ecfc441a1",
             "columns": [
+                "total",
                 "siteName",
+                "other",
                 "forwarded",
-                "intName",
-                "hostname",
-                "total",
-                "sn",
+                "id",
                 "local",
-                "other",
-                "id"
+                "sn",
+                "hostname",
+                "intName"
             ],
             "description": "Point-to-Point Protocol over Ethernet (PPPoE) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PPPoE interfaces",
             "ui_columns": [
                 "hostname",
@@ -6347,33 +6370,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/pppoe/sessions",
             "api_scope_id": "5cc25601bec2e60dd0856b57fa88b8ffcf6c50e0",
             "columns": [
-                "framedIp",
-                "identity",
-                "siteName",
+                "id",
                 "inPktsRate",
-                "sn",
-                "pppMaxPayload",
-                "localIntName",
+                "framedIp",
+                "virtualAccessIntName",
+                "outPktsRate",
+                "outIntName",
+                "outQosPolicy",
+                "hostname",
                 "inBytesRate",
                 "sessionId",
-                "hostname",
                 "isStaticRoute",
-                "virtualAccessIntName",
-                "outPktsRate",
+                "localIntName",
                 "inQosPolicy",
-                "outBytesRate",
                 "state",
-                "outIntName",
-                "outQosPolicy",
-                "id"
+                "sn",
+                "identity",
+                "siteName",
+                "outBytesRate",
+                "pppMaxPayload"
             ],
             "description": "Point-to-Point Protocol over Ethernet (PPPoE) interface sessions inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PPPoE sessions",
             "ui_columns": [
                 "hostname",
@@ -6403,28 +6426,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/all",
             "api_scope_id": "12d83131919fbbe887dac1acf741631ff44212d1",
             "columns": [
-                "lowerLimit",
+                "unit",
                 "currentTraffic",
-                "action",
-                "hostname",
-                "intName",
                 "siteName",
-                "snmpTrap",
+                "lowerLimit",
                 "upperLimit",
-                "sn",
-                "changes",
+                "id",
                 "state",
-                "unit",
                 "logUpperLimit",
-                "id"
+                "changes",
+                "sn",
+                "action",
+                "snmpTrap",
+                "hostname",
+                "intName"
             ],
             "description": "Details for storm control traffic detection - all traffic",
             "method": "post",
             "nested_columns": [],
             "summary": "Storm Control - All Traffic",
             "ui_columns": [
                 "hostname",
@@ -6449,28 +6472,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/broadcast",
             "api_scope_id": "0dbe90d070c013fead0bb1d3eaf12f99fc657222",
             "columns": [
-                "lowerLimit",
+                "unit",
                 "currentTraffic",
-                "action",
-                "hostname",
-                "intName",
                 "siteName",
-                "snmpTrap",
+                "lowerLimit",
                 "upperLimit",
-                "sn",
-                "changes",
+                "id",
                 "state",
-                "unit",
                 "logUpperLimit",
-                "id"
+                "changes",
+                "sn",
+                "action",
+                "snmpTrap",
+                "hostname",
+                "intName"
             ],
             "description": "Details for storm control traffic detection - broadcast",
             "method": "post",
             "nested_columns": [],
             "summary": "Storm Control - Broadcast",
             "ui_columns": [
                 "hostname",
@@ -6495,28 +6518,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/multicast",
             "api_scope_id": "42ef5f9a374112076110e811e281e958a1bf2ae4",
             "columns": [
-                "lowerLimit",
+                "unit",
                 "currentTraffic",
-                "action",
-                "hostname",
-                "intName",
                 "siteName",
-                "snmpTrap",
+                "lowerLimit",
                 "upperLimit",
-                "sn",
-                "changes",
+                "id",
                 "state",
-                "unit",
                 "logUpperLimit",
-                "id"
+                "changes",
+                "sn",
+                "action",
+                "snmpTrap",
+                "hostname",
+                "intName"
             ],
             "description": "Details for storm control traffic detection - unicast",
             "method": "post",
             "nested_columns": [],
             "summary": "Storm Control - Unicast",
             "ui_columns": [
                 "hostname",
@@ -6541,28 +6564,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/unicast",
             "api_scope_id": "6b658b47f5b8a2fff8ed759a262a5ecb6c8890dc",
             "columns": [
-                "lowerLimit",
+                "unit",
                 "currentTraffic",
-                "action",
-                "hostname",
-                "intName",
                 "siteName",
-                "snmpTrap",
+                "lowerLimit",
                 "upperLimit",
-                "sn",
-                "changes",
+                "id",
                 "state",
-                "unit",
                 "logUpperLimit",
-                "id"
+                "changes",
+                "sn",
+                "action",
+                "snmpTrap",
+                "hostname",
+                "intName"
             ],
             "description": "Details for storm control traffic detection - multicast",
             "method": "post",
             "nested_columns": [],
             "summary": "Storm Control - Multicast",
             "ui_columns": [
                 "hostname",
@@ -6587,31 +6610,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/switchports",
             "api_scope_id": "db92291d321f3cd7dc8ed226810dd6769427b50c",
             "columns": [
-                "mode",
-                "nativeVlan",
+                "macCount",
                 "siteName",
-                "hostname",
-                "intName",
                 "dscr",
-                "sn",
-                "voiceVlan",
+                "id",
+                "trunkVlan",
                 "dynamicMacCount",
+                "mode",
+                "devType",
                 "edge",
+                "sn",
                 "staticMacCount",
-                "trunkVlan",
+                "voiceVlan",
                 "encap",
-                "macCount",
+                "nativeVlan",
                 "accVlan",
-                "devType",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "Overview of all L2 Ethernet switchports",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Switchport",
             "ui_columns": [
                 "hostname",
@@ -6640,21 +6663,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/errors",
             "api_scope_id": "828e3070cf04347f7f9fe3cd6679130c5b5e76df",
             "columns": [
                 "siteName",
-                "intName",
-                "hostname",
                 "pn",
+                "id",
+                "errorLane",
                 "errorMessage",
                 "sn",
-                "id",
-                "errorLane"
+                "hostname",
+                "intName"
             ],
             "description": "Information oninterfaces transceivers errors messages and thresholds",
             "method": "post",
             "nested_columns": [],
             "summary": "Transceivers Errors",
             "ui_columns": [
                 "hostname",
@@ -6673,27 +6696,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/inventory",
             "api_scope_id": "b785b906c2aa75c8a6596ad065460cef328f46bd",
             "columns": [
-                "paramsList",
-                "tSn",
+                "tVendor",
                 "siteName",
-                "hostname",
-                "intName",
-                "pn",
                 "dscr",
+                "paramsList",
+                "pn",
+                "id",
+                "type",
                 "sn",
-                "l2",
                 "l1",
-                "tVendor",
-                "type",
-                "id"
+                "l2",
+                "tSn",
+                "hostname",
+                "intName"
             ],
             "description": "Interface transceivers inventory",
             "method": "post",
             "nested_columns": [
                 "paramsList"
             ],
             "summary": "Transceivers Inventory",
@@ -6719,38 +6742,38 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/statistics",
             "api_scope_id": "3f69d2448d97d72abb4298a0a11bfe678421fcc9",
             "columns": [
-                "deltaValueLow",
-                "siteName",
-                "sn",
+                "unit",
+                "statistic",
+                "pn",
+                "type",
+                "id",
+                "intName",
                 "vendor",
+                "tVendor",
+                "family",
+                "platform",
+                "thresholdLow",
+                "laneOrigIntName",
+                "hostname",
+                "flag",
+                "dscr",
                 "threshold",
+                "sn",
+                "deltaValueLow",
                 "lane",
-                "unit",
                 "model",
+                "siteName",
                 "deltaValueHigh",
-                "thresholdHigh",
-                "thresholdLow",
                 "value",
-                "hostname",
-                "intName",
-                "statistic",
-                "platform",
-                "tVendor",
-                "type",
-                "laneOrigIntName",
-                "pn",
-                "dscr",
-                "flag",
-                "family",
-                "id"
+                "thresholdHigh"
             ],
             "description": "Interface transceivers statistics",
             "method": "post",
             "nested_columns": [],
             "summary": "Transceivers Statistics",
             "ui_columns": [
                 "hostname",
@@ -6784,25 +6807,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/thresholds",
             "api_scope_id": "a40e0396c0197d37f2ba1592a045d2cfaa341e22",
             "columns": [
+                "lane",
                 "siteName",
-                "hostname",
-                "intName",
-                "level",
                 "pn",
-                "flag",
-                "sn",
-                "name",
-                "lane",
                 "type",
-                "id"
+                "id",
+                "level",
+                "name",
+                "sn",
+                "hostname",
+                "flag",
+                "intName"
             ],
             "description": "Interface transceivers triggered thresholds",
             "method": "post",
             "nested_columns": [],
             "summary": "Transceivers Triggered Thresholds",
             "ui_columns": [
                 "hostname",
@@ -6824,24 +6847,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/bidirectional",
             "api_scope_id": "83e4917aaf74ad60f01d76d4cbd9929745362bfa",
             "columns": [
+                "pktsRate",
+                "bcastRate",
+                "bytesRate",
                 "mcastRate",
-                "impactLoss",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "sn",
-                "bcastRate",
-                "pktsRate",
-                "bytesRate",
-                "id"
+                "impactLoss",
+                "hostname",
+                "intName"
             ],
             "description": "Bidirectional interface rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Bidirectional Interface Rates",
             "ui_columns": [
                 "hostname",
@@ -6862,23 +6885,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/bidirectional-device",
             "api_scope_id": "81f2c4d4e770942f7d338ea7da98c3ee9824fd06",
             "columns": [
+                "pktsRate",
+                "bcastRate",
+                "bytesRate",
                 "mcastRate",
-                "impactLoss",
                 "siteName",
-                "hostname",
+                "id",
                 "sn",
-                "bcastRate",
-                "pktsRate",
-                "bytesRate",
-                "id"
+                "impactLoss",
+                "hostname"
             ],
             "description": "Per-Device bidirectional transfer rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Bidirectional Transfer Rates",
             "ui_columns": [
                 "hostname",
@@ -6898,24 +6921,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/inbound",
             "api_scope_id": "cb0492b17a9d7fedb5c3a3aace3f40694e6f6da3",
             "columns": [
+                "inBcastRate",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "inImpactLoss",
-                "inPktsRate",
                 "sn",
-                "inBcastRate",
-                "inMcastRate",
+                "inPktsRate",
+                "intName",
+                "hostname",
                 "inBytesRate",
-                "id"
+                "inMcastRate"
             ],
             "description": "Inbound interface rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Inbound Interface Transfer Rates",
             "ui_columns": [
                 "hostname",
@@ -6936,23 +6959,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/inbound-device",
             "api_scope_id": "709b279b23ba8bafda8aefa88da761970434ef0a",
             "columns": [
+                "inBcastRate",
                 "siteName",
-                "hostname",
+                "id",
                 "inImpactLoss",
-                "inPktsRate",
                 "sn",
-                "inBcastRate",
-                "inMcastRate",
+                "inPktsRate",
+                "hostname",
                 "inBytesRate",
-                "id"
+                "inMcastRate"
             ],
             "description": "Per-Device inbound interface transfer rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Inbound Interface Transfer Rates",
             "ui_columns": [
                 "hostname",
@@ -6972,24 +6995,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/outbound",
             "api_scope_id": "6b1c68eeee092c5497798689c7e6b07ff5c11e07",
             "columns": [
-                "outPktsRate",
-                "hostname",
-                "intName",
+                "outMcastRate",
                 "siteName",
+                "outPktsRate",
+                "id",
                 "outBytesRate",
-                "sn",
-                "outImpactLoss",
-                "outMcastRate",
                 "outBcastRate",
-                "id"
+                "outImpactLoss",
+                "sn",
+                "hostname",
+                "intName"
             ],
             "description": "Outbound interface rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Outbound Interface Transfer Rates",
             "ui_columns": [
                 "hostname",
@@ -7010,23 +7033,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/outbound-device",
             "api_scope_id": "9b50ccd8960c187487f69d88019f07d791a3c330",
             "columns": [
-                "outPktsRate",
-                "hostname",
+                "outMcastRate",
                 "siteName",
+                "outPktsRate",
+                "id",
                 "outBytesRate",
-                "sn",
-                "outImpactLoss",
-                "outMcastRate",
                 "outBcastRate",
-                "id"
+                "outImpactLoss",
+                "sn",
+                "hostname"
             ],
             "description": "Per-Device outbound interface transfer rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Outbound Interface Transfer Rates",
             "ui_columns": [
                 "hostname",
@@ -7046,26 +7069,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/tunnels/ipv4",
             "api_scope_id": "9fe34a5d8c4ba0fc884a4d2f9d997b00c0eaf807",
             "columns": [
-                "tunnelSrcIp",
-                "tunnelProto",
-                "siteName",
-                "hostname",
-                "intName",
-                "tunnelDstIp",
-                "sn",
-                "vrf",
                 "tunnelSrcIntName",
                 "tunnelVrf",
+                "siteName",
+                "id",
+                "tunnelProto",
+                "sn",
                 "ipAddresses",
-                "id"
+                "tunnelDstIp",
+                "vrf",
+                "hostname",
+                "intName",
+                "tunnelSrcIp"
             ],
             "description": "IPv4 Tunnels inventory",
             "method": "post",
             "nested_columns": [
                 "ipAddresses"
             ],
             "summary": "IPv4 Tunnels",
@@ -7090,26 +7113,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/tunnels/ipv6",
             "api_scope_id": "d8ca81b4bcae5a87466caf73f6a51e3567bfa426",
             "columns": [
-                "tunnelProto",
-                "siteName",
-                "hostname",
-                "intName",
-                "sn",
-                "vrf",
+                "tunnelDstIpv6",
                 "tunnelSrcIntName",
                 "tunnelVrf",
+                "siteName",
                 "ipv6Addresses",
-                "tunnelDstIpv6",
+                "id",
+                "tunnelProto",
                 "tunnelSrcIpv6",
-                "id"
+                "sn",
+                "vrf",
+                "hostname",
+                "intName"
             ],
             "description": "IPv6 Tunnels inventory",
             "method": "post",
             "nested_columns": [
                 "ipv6Addresses"
             ],
             "summary": "IPv6 Tunnels",
@@ -7134,47 +7157,47 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/devices",
             "api_scope_id": "c701b81c3a91ebd953f0097a2fa520507745243f",
             "columns": [
-                "loginIp",
-                "siteName",
-                "domain",
-                "sn",
-                "processor",
-                "vendor",
-                "loginType",
-                "loginPort",
-                "hostnameProcessed",
-                "objectId",
                 "slug",
-                "model",
+                "icon",
+                "id",
+                "taskKey",
                 "uptime",
-                "rd",
-                "snHw",
-                "reload",
+                "processor",
                 "version",
-                "mac",
-                "image",
                 "memoryTotalBytes",
-                "taskKey",
-                "hostname",
+                "vendor",
+                "family",
                 "platform",
+                "snHw",
                 "memoryUsedBytes",
+                "loginIp",
                 "fqdn",
-                "icon",
                 "stpDomain",
-                "family",
-                "configReg",
-                "memoryUtilization",
+                "domain",
+                "hostname",
+                "image",
                 "hostnameOriginal",
+                "reload",
+                "sn",
+                "memoryUtilization",
+                "hostnameProcessed",
+                "loginPort",
+                "model",
+                "siteName",
+                "objectId",
+                "rd",
                 "devType",
-                "id"
+                "loginType",
+                "mac",
+                "configReg"
             ],
             "description": "Inventory of all logical or physical managed network infrastructure devices discovered",
             "method": "post",
             "nested_columns": [],
             "summary": "Device Inventory",
             "ui_columns": [
                 "hostname",
@@ -7216,22 +7239,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/discovery-history",
             "api_scope_id": "80270bc86b703bca1062673a80977e7e80ac05a9",
             "columns": [
+                "id",
+                "usernameNotes",
                 "loginIp",
-                "hostname",
                 "sn",
                 "loginType",
-                "username",
-                "usernameNotes",
                 "ts",
-                "id"
+                "hostname",
+                "username"
             ],
             "description": "This view shows all discovered devices in history (no matter which snapshot is selected). IP Fabric will remember used protocol and last successful credential. These informations are preferred in the next discovery run.",
             "method": "post",
             "nested_columns": [],
             "summary": "Discovery History",
             "ui_columns": [
                 "hostname",
@@ -7251,24 +7274,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/fans",
             "api_scope_id": "512962c963edf9758d1dfef99eb4e90fdf23ad8a",
             "columns": [
-                "siteName",
-                "hostname",
                 "deviceId",
-                "sn",
-                "fanSn",
-                "fanPid",
+                "siteName",
+                "fanId",
                 "fanState",
                 "id",
+                "sn",
                 "fanName",
-                "fanId"
+                "hostname",
+                "fanPid",
+                "fanSn"
             ],
             "description": "Fans detected in all network devices and their current state",
             "method": "post",
             "nested_columns": [],
             "summary": "Environment - Fans",
             "ui_columns": [
                 "hostname",
@@ -7289,42 +7312,42 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/interfaces",
             "api_scope_id": "fa462e10f3ff2a756fce2f862d6e08d913113cfd",
             "columns": [
-                "loginIp",
-                "siteName",
-                "sn",
-                "loginType",
-                "transceiverSn",
                 "slug",
-                "l1",
-                "duplex",
-                "reason",
-                "mtu",
-                "mac",
-                "errDisabled",
-                "media",
-                "transceiverPn",
-                "hostname",
-                "intName",
-                "nameOriginal",
-                "primaryIp",
-                "rel",
                 "speedValue",
-                "speed",
                 "id",
-                "hasTransceiver",
-                "speedType",
+                "nameOriginal",
+                "intName",
+                "transceiverPn",
+                "loginIp",
+                "l1",
+                "l2",
+                "rel",
+                "hostname",
                 "transceiverType",
+                "speed",
+                "duplex",
                 "dscr",
+                "primaryIp",
+                "mtu",
+                "transceiverSn",
                 "intNameAlias",
-                "l2"
+                "sn",
+                "hasTransceiver",
+                "siteName",
+                "media",
+                "speedType",
+                "loginType",
+                "reason",
+                "mac",
+                "errDisabled"
             ],
             "description": "Information on every detected physical or logical interface for all discovered devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Interface Inventory",
             "ui_columns": [
                 "hostname",
@@ -7360,22 +7383,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/modules",
             "api_scope_id": "d4769862d55464e1b9fdb16103a9f5432de432a6",
             "columns": [
-                "siteName",
-                "hostname",
                 "deviceId",
-                "moduleId",
-                "sn",
-                "moduleState",
+                "modulePid",
+                "siteName",
                 "id",
-                "modulePid"
+                "moduleState",
+                "sn",
+                "moduleId",
+                "hostname"
             ],
             "description": "Information about every detected modules and their current the state",
             "method": "post",
             "nested_columns": [],
             "summary": "Environment - Modules",
             "ui_columns": [
                 "hostname",
@@ -7394,27 +7417,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/phones",
             "api_scope_id": "adc2e1502c234d6ba717a50e15cb0d06d5853e1a",
             "columns": [
-                "phoneName",
-                "userMac",
+                "phoneInt",
                 "siteName",
-                "userIp",
-                "phoneMac",
+                "switchInt",
+                "switchSn",
+                "id",
                 "voiceVlan",
-                "switchHostname",
-                "vendor",
+                "userMac",
                 "phoneIp",
-                "phoneInt",
-                "switchSn",
-                "switchInt",
-                "id"
+                "phoneMac",
+                "phoneName",
+                "vendor",
+                "switchHostname",
+                "userIp"
             ],
             "description": "Inventory of all detected IP phones and endpoints connected to them",
             "method": "post",
             "nested_columns": [],
             "summary": "IP Phones and Connected Devices",
             "ui_columns": [
                 "phoneIp",
@@ -7438,27 +7461,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/pn",
             "api_scope_id": "efd238e0d15b04ad415446efaca80939e4186f72",
             "columns": [
-                "siteName",
-                "hostname",
-                "platform",
+                "deviceSn",
                 "deviceId",
+                "model",
+                "siteName",
                 "dscr",
-                "sn",
+                "platform",
+                "id",
                 "name",
-                "vid",
-                "vendor",
+                "sn",
                 "pid",
-                "model",
-                "deviceSn",
-                "id"
+                "vid",
+                "hostname",
+                "vendor"
             ],
             "description": "Modules and part numbers from inventory of network infrastructure devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Modules and Part Numbers Inventory",
             "ui_columns": [
                 "hostname",
@@ -7482,27 +7505,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/power-supplies",
             "api_scope_id": "8ccd4c725aefc8efa41dd74685da5711b3e550e2",
             "columns": [
-                "pwSupplyType",
-                "pwSupplyState",
-                "hostname",
-                "pwSupplyName",
+                "deviceId",
+                "model",
                 "pwSupplyId",
+                "pwSupplyName",
                 "siteName",
-                "deviceId",
-                "pwSupplySn",
+                "pwSupplyPid",
+                "id",
+                "pwSupplyState",
                 "sn",
+                "pwSupplyType",
                 "pwSupplyCircuit",
-                "pwSupplyPid",
-                "model",
-                "id"
+                "hostname",
+                "pwSupplySn"
             ],
             "description": "Power supplies detected in all network devices and their current state",
             "method": "post",
             "nested_columns": [],
             "summary": "Environment - Power Supplies",
             "ui_columns": [
                 "hostname",
@@ -7526,24 +7549,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/power-supplies-fans",
             "api_scope_id": "8fd8461fcc4364f29bc852f9dd78ac6b30b1314d",
             "columns": [
-                "fanVendor",
-                "hostname",
-                "siteName",
                 "deviceId",
-                "sn",
-                "fanSn",
+                "siteName",
+                "fanId",
                 "fanState",
                 "id",
+                "sn",
+                "fanVendor",
                 "fanName",
-                "fanId"
+                "hostname",
+                "fanSn"
             ],
             "description": "Power supplies fans detected in all network devices and their current state",
             "method": "post",
             "nested_columns": [],
             "summary": "Environment - Power Supplies Fans",
             "ui_columns": [
                 "hostname",
@@ -7564,26 +7587,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/sites",
             "api_scope_id": "a067b848a10f9ef2989c1fcb058982213cb56167",
             "columns": [
+                "routersCount",
                 "devicesCount",
                 "rDCount",
-                "stpDCount",
                 "siteName",
-                "routersCount",
-                "rDomains",
-                "networksCount",
-                "usersCount",
-                "vlanCount",
                 "switchesCount",
+                "id",
+                "stpDCount",
+                "vlanCount",
                 "stpDomains",
-                "id"
+                "rDomains",
+                "networksCount",
+                "usersCount"
             ],
             "description": "Sites inventory defined by site separation rules or attributes",
             "method": "post",
             "nested_columns": [],
             "summary": "Sites Inventory",
             "ui_columns": [
                 "siteName",
@@ -7605,20 +7628,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/families",
             "api_scope_id": "023573d36598f61c617939f256d986e21d878915",
             "columns": [
-                "devicesCount",
                 "modelsCount",
                 "platformsCount",
-                "vendor",
+                "devicesCount",
                 "family",
-                "id"
+                "id",
+                "vendor"
             ],
             "description": "Inventory covering vendor - families distribution",
             "method": "post",
             "nested_columns": [],
             "summary": "Vendor Families Overview",
             "ui_columns": [
                 "vendor",
@@ -7637,19 +7660,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/models",
             "api_scope_id": "feb805028154b351a6397fd18d468eba808d37ca",
             "columns": [
                 "devicesCount",
-                "platform",
-                "vendor",
-                "model",
                 "family",
-                "id"
+                "model",
+                "platform",
+                "id",
+                "vendor"
             ],
             "description": "Inventory covering vendor - families - platforms - models distribution",
             "method": "post",
             "nested_columns": [],
             "summary": "Vendor Models Overview",
             "ui_columns": [
                 "vendor",
@@ -7667,20 +7690,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/platforms",
             "api_scope_id": "062b8c7e2a3e2323c7b7c71542b6566ae4851697",
             "columns": [
-                "devicesCount",
                 "modelsCount",
-                "platform",
-                "vendor",
+                "devicesCount",
                 "family",
-                "id"
+                "platform",
+                "id",
+                "vendor"
             ],
             "description": "Inventory covering vendor - families - platforms distribution",
             "method": "post",
             "nested_columns": [],
             "summary": "Vendor Platforms Overview",
             "ui_columns": [
                 "vendor",
@@ -7698,20 +7721,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/vendors",
             "api_scope_id": "3aed3be2e793d01ef760cab3dc683ccbc2c95be7",
             "columns": [
-                "devicesCount",
                 "modelsCount",
                 "platformsCount",
+                "devicesCount",
+                "id",
                 "vendor",
-                "familiesCount",
-                "id"
+                "familiesCount"
             ],
             "description": "Inventory covering vendor distribution",
             "method": "post",
             "nested_columns": [],
             "summary": "Vendors Overview",
             "ui_columns": [
                 "vendor",
@@ -7729,22 +7752,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/temperature-sensors",
             "api_scope_id": "c05978e6cb1a054093bec04f7c99a0c4a7b746e1",
             "columns": [
-                "thermalState",
-                "siteName",
-                "hostname",
                 "deviceId",
-                "sn",
-                "thermalId",
                 "model",
+                "siteName",
+                "thermalId",
                 "id",
+                "sn",
+                "thermalState",
+                "hostname",
                 "thermalDescription"
             ],
             "description": "Status of temperature sensors",
             "method": "post",
             "nested_columns": [],
             "summary": "Environment - Temperature sensors",
             "ui_columns": [
@@ -7765,24 +7788,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/jobs",
             "api_scope_id": "5fd6f107524d27bc33de517ed329cbe6708ff06b",
             "columns": [
+                "status",
                 "finishedAt",
+                "isDone",
+                "id",
                 "startedAt",
-                "downloadFile",
                 "name",
                 "scheduledAt",
-                "status",
                 "username",
                 "snapshot",
-                "id",
-                "isDone"
+                "downloadFile"
             ],
             "description": "IP Fabric scheduled or running jobs",
             "method": "post",
             "nested_columns": [],
             "summary": "Platform Jobs",
             "ui_columns": [
                 "id",
@@ -7806,19 +7829,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/load-balancing/f5-partitions",
             "api_scope_id": "7b06a1adb684d5d9817314e5cbb000a7ac3321e2",
             "columns": [
                 "siteName",
-                "hostname",
+                "id",
+                "partitionName",
                 "partitionDescription",
                 "sn",
-                "partitionName",
-                "id"
+                "hostname"
             ],
             "description": "F5 Partitions inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "F5 Partitions",
             "ui_columns": [
                 "hostname",
@@ -7835,34 +7858,34 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/load-balancing/virtual-servers",
             "api_scope_id": "e9022c4ef969209a382862d4e53405880dbce711",
             "columns": [
-                "portName",
-                "siteName",
-                "poolsCount",
-                "sn",
+                "id",
                 "clientProfile",
+                "pools",
+                "protocolNumber",
                 "protocolName",
-                "virtualServerName",
-                "vrf",
-                "reason",
-                "portNumber",
+                "portName",
+                "poolsCount",
                 "availability",
-                "partition",
                 "hostname",
-                "protocolNumber",
-                "sourceNat",
-                "pools",
                 "vip",
-                "vip6",
+                "vrf",
+                "partition",
                 "state",
-                "id"
+                "sn",
+                "sourceNat",
+                "portNumber",
+                "siteName",
+                "reason",
+                "vip6",
+                "virtualServerName"
             ],
             "description": "Load balancing - virtual servers inventory",
             "method": "post",
             "nested_columns": [
                 "pools",
                 "vip",
                 "vip6"
@@ -7897,26 +7920,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/load-balancing/virtual-servers/pool-members",
             "api_scope_id": "b9a7e96661b01e097932614a33ca90a4da636eb3",
             "columns": [
-                "port",
-                "hostname",
+                "memberIpV6",
                 "siteName",
+                "port",
+                "id",
+                "state",
+                "poolName",
                 "memberIp",
                 "sn",
-                "vrf",
-                "memberIpV6",
-                "poolName",
-                "state",
-                "poolMemberName",
                 "availability",
-                "id"
+                "vrf",
+                "hostname",
+                "poolMemberName"
             ],
             "description": "Load balancing - virtual servers and pool members inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Virtual Servers - Pool members",
             "ui_columns": [
                 "hostname",
@@ -7940,32 +7963,33 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/load-balancing/virtual-servers/pools",
             "api_scope_id": "eacbfd8381e770faf6382444d34f45956921d0e0",
             "columns": [
                 "siteName",
-                "hostname",
+                "id",
+                "membersCount",
                 "sn",
-                "members",
+                "hostname",
                 "poolName",
-                "membersCount",
-                "id"
+                "members"
             ],
             "description": "Load balancing - virtual servers and pools inventory",
             "method": "post",
             "nested_columns": [
                 "members"
             ],
             "summary": "Virtual Servers - Pools",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "poolName",
-                "membersCount"
+                "membersCount",
+                "members"
             ],
             "web_endpoint": "/technology/load-balancing/virtual-servers-pools"
         },
         "put": null
     },
     "tables/management/banners/banners": {
         "api_endpoint": "/tables/management/banners/banners",
@@ -7973,19 +7997,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/banners/banners",
             "api_scope_id": "3b7234600756841ed802d76563f4484d92e4f3df",
             "columns": [
                 "siteName",
-                "hostname",
-                "text",
-                "sn",
                 "type",
-                "id"
+                "id",
+                "sn",
+                "hostname",
+                "text"
             ],
             "description": "Types and texts of the device banners",
             "method": "post",
             "nested_columns": [],
             "summary": "Device Banners",
             "ui_columns": [
                 "hostname",
@@ -8002,20 +8026,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/banners/summary",
             "api_scope_id": "63b5a7e866e79d5ac1ec87c8f9d862bdece3ba57",
             "columns": [
-                "motdBanner",
                 "siteName",
-                "hostname",
-                "sn",
                 "loginBanner",
-                "id"
+                "id",
+                "sn",
+                "motdBanner",
+                "hostname"
             ],
             "description": "Summary view for device banners",
             "method": "post",
             "nested_columns": [],
             "summary": "Banners Summary",
             "ui_columns": [
                 "hostname",
@@ -8032,25 +8056,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/changes/connectivity",
             "api_scope_id": "205a406d59d39c5b5c3c03c64dbe0ed2a1a6a4e1",
             "columns": [
-                "localInt",
-                "remoteMedia",
-                "remoteInt",
-                "remoteSn",
                 "localMedia",
+                "id",
+                "remoteInt",
+                "localInt",
                 "remoteHost",
                 "localHost",
-                "status",
                 "protocol",
+                "remoteSn",
+                "remoteMedia",
                 "localSn",
-                "id"
+                "status"
             ],
             "description": "Changes in connectivity matrix between selected snapshots",
             "method": "post",
             "nested_columns": [],
             "summary": "Changes in connectivity matrix",
             "ui_columns": [
                 "id",
@@ -8074,25 +8098,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/changes/devices",
             "api_scope_id": "bff34be4b27e5d76ec4a78857f2c7f0ca0b20530",
             "columns": [
+                "image",
+                "id",
                 "uptime",
                 "loginIp",
-                "hostname",
-                "sn",
                 "processor",
-                "configReg",
-                "status",
                 "reload",
                 "version",
-                "id",
-                "image"
+                "sn",
+                "configReg",
+                "hostname",
+                "status"
             ],
             "description": "Changes in discovered devices between selected snapshots",
             "method": "post",
             "nested_columns": [],
             "summary": "Changes in devices",
             "ui_columns": [
                 "id",
@@ -8116,22 +8140,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/changes/managed-devs",
             "api_scope_id": "74bfe2920e6c6ba589df4951acb573654641dcaa",
             "columns": [
-                "hostname",
-                "intName",
+                "type",
+                "id",
+                "net",
                 "sn",
-                "status",
+                "intName",
+                "hostname",
                 "ip",
-                "net",
-                "type",
-                "id"
+                "status"
             ],
             "description": "Changes in managed interface IP addresses between selected snapshots",
             "method": "post",
             "nested_columns": [],
             "summary": "Changes in Managed IP",
             "ui_columns": [
                 "id",
@@ -8152,23 +8176,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/changes/pn",
             "api_scope_id": "9449202b14ae1a0fea9fb19f82ac83682fe537e9",
             "columns": [
-                "hostname",
                 "deviceId",
                 "dscr",
-                "sn",
+                "id",
                 "name",
-                "vid",
-                "status",
+                "sn",
                 "pid",
-                "id"
+                "vid",
+                "hostname",
+                "status"
             ],
             "description": "Changes in part numbers between selected snapshots",
             "method": "post",
             "nested_columns": [],
             "summary": "Changes in Part Numbers",
             "ui_columns": [
                 "id",
@@ -8190,22 +8214,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/configuration",
             "api_scope_id": "e5cac6dcf2d741c053f58fbcda2b0d3f88dbf4a2",
             "columns": [
-                "lastCheckAt",
-                "hostname",
-                "sn",
-                "lastChangeAt",
-                "status",
                 "hash",
+                "id",
+                "lastChangeAt",
+                "sn",
+                "lastCheckAt",
                 "reason",
-                "id"
+                "hostname",
+                "status"
             ],
             "description": "Inventory of all captured configuration files",
             "method": "post",
             "nested_columns": [],
             "summary": "Configuration Files",
             "ui_columns": [
                 "id",
@@ -8280,24 +8304,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/configuration/saved",
             "api_scope_id": "953130708a830c65095c48804e9c0fc647964b3e",
             "columns": [
-                "uptime",
+                "siteName",
+                "startupConfigExists",
                 "blobKey",
+                "id",
+                "uptime",
                 "loginIp",
-                "siteName",
+                "sn",
                 "hostname",
                 "currentConfigExists",
-                "sn",
-                "status",
-                "startupConfigExists",
-                "id"
+                "status"
             ],
             "description": "Compare the current and startup configuration files",
             "method": "post",
             "nested_columns": [],
             "summary": "Saved Config Consistency",
             "ui_columns": [
                 "hostname",
@@ -8315,21 +8339,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/connectivity-errors",
             "api_scope_id": "8ff0b8fbbd918cc544206aa0d4b4feaecf1cc544",
             "columns": [
-                "sshType",
                 "telnetType",
+                "sshType",
+                "id",
                 "date",
-                "ip",
-                "sshMsg",
                 "telnetMsg",
-                "id"
+                "ip",
+                "sshMsg"
             ],
             "description": "Observe connectivity errors for failed configuration file downloads",
             "method": "post",
             "nested_columns": [],
             "summary": "Configuration Management Connectivity Errors",
             "ui_columns": [
                 "id",
@@ -8349,28 +8373,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/discovery-runs",
             "api_scope_id": "ad7a1cd54273549505a722cfd794af4cbc33dcfe",
             "columns": [
-                "deviceCount",
-                "interfaceActiveCount",
-                "tsStart",
-                "partNumbersCount",
-                "connectionCount",
-                "tsEnd",
-                "interfaceCount",
-                "userCount",
-                "managedIpCount",
                 "status",
+                "interfaceActiveCount",
                 "tsChange",
+                "tsEnd",
+                "id",
                 "isLastSnapshot",
                 "interfaceEdgeCount",
-                "id"
+                "userCount",
+                "tsStart",
+                "connectionCount",
+                "interfaceCount",
+                "partNumbersCount",
+                "deviceCount",
+                "managedIpCount"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "Changes",
             "ui_columns": [
                 "id",
@@ -8397,25 +8421,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/dns/servers",
             "api_scope_id": "f84fc1283440f332105f9414add605617ab09366",
             "columns": [
-                "type",
-                "searchDomains",
-                "hostname",
                 "siteName",
-                "sn",
-                "vrf",
+                "type",
+                "id",
                 "ipv6",
+                "sn",
                 "srcIntName",
+                "searchDomains",
+                "vrf",
+                "hostname",
                 "ip",
-                "parentId",
-                "id"
+                "parentId"
             ],
             "description": "Inventory of configured DNS servers on managed network devices",
             "method": "post",
             "nested_columns": [
                 "searchDomains"
             ],
             "summary": "DNS Servers",
@@ -8438,22 +8462,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/dns/settings",
             "api_scope_id": "1d4366f0342d43cc41c8dc28a22a1c300d4c4d05",
             "columns": [
-                "retry",
-                "hostname",
                 "siteName",
-                "sn",
-                "protocols",
+                "id",
                 "timeout",
+                "retry",
                 "dnsServersCount",
-                "id"
+                "sn",
+                "protocols",
+                "hostname"
             ],
             "description": "Inventory of additional DNS settings on managed network devices",
             "method": "post",
             "nested_columns": [
                 "protocols"
             ],
             "summary": "DNS Settings",
@@ -8474,25 +8498,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/netflow/collectors",
             "api_scope_id": "66a23028ec74211250e2fe8df9e612c509babd3b",
             "columns": [
-                "port",
-                "hostname",
                 "siteName",
+                "port",
+                "collector",
                 "srcInterface",
+                "id",
+                "version",
+                "protocol",
                 "sn",
                 "vrf",
-                "srcAddress",
-                "protocol",
-                "version",
-                "collector",
-                "id"
+                "hostname",
+                "srcAddress"
             ],
             "description": "Inventory of NetFlow collectors configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "NetFlow Collectors",
             "ui_columns": [
                 "hostname",
@@ -8516,20 +8540,20 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/netflow/devices",
             "api_scope_id": "3032ab06eb03a1554de2df293f6a22fd607959ff",
             "columns": [
                 "inactiveTimeout",
                 "siteName",
-                "hostname",
-                "activeTimeout",
-                "sn",
                 "countNetflowCollectors",
+                "id",
+                "sn",
+                "activeTimeout",
                 "countNetflowInterfaces",
-                "id"
+                "hostname"
             ],
             "description": "Managed network devices with configured NetFlow collectors",
             "method": "post",
             "nested_columns": [],
             "summary": "NetFlow Devices",
             "ui_columns": [
                 "hostname",
@@ -8549,19 +8573,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/netflow/interfaces",
             "api_scope_id": "480c1176444e47070d4a1cb5a067b19c5a994976",
             "columns": [
                 "siteName",
-                "hostname",
-                "interface",
-                "sn",
                 "directions",
-                "id"
+                "id",
+                "sn",
+                "interface",
+                "hostname"
             ],
             "description": "Inventory of interfaces participating in NetFlow collection",
             "method": "post",
             "nested_columns": [
                 "directions"
             ],
             "summary": "NetFlow Interfaces",
@@ -8580,22 +8604,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/overview",
             "api_scope_id": "71c12b11bddc390ec742bb6427ff1ab1638be831",
             "columns": [
-                "countSflowSources",
-                "hostname",
                 "siteName",
-                "sn",
+                "countSflowCollectors",
                 "countNetflowCollectors",
+                "id",
+                "sn",
                 "countNetflowInterfaces",
-                "countSflowCollectors",
-                "id"
+                "hostname",
+                "countSflowSources"
             ],
             "description": "Summary inventory of devices participating in either NetFlow or sFlow collection",
             "method": "post",
             "nested_columns": [],
             "summary": "Flow Overview",
             "ui_columns": [
                 "hostname",
@@ -8614,21 +8638,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/sflow/collectors",
             "api_scope_id": "8a006a5d361cca0e0d7ad0fd66dd9949d5ca73b4",
             "columns": [
-                "port",
-                "hostname",
                 "siteName",
+                "port",
+                "collector",
+                "id",
                 "sn",
                 "vrf",
-                "collector",
-                "id"
+                "hostname"
             ],
             "description": "Inventory of sFlow collectors configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "sFlow Collectors",
             "ui_columns": [
                 "hostname",
@@ -8646,26 +8670,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/sflow/devices",
             "api_scope_id": "5f4dda4c06013f386007d2cff645bd3dc2abe783",
             "columns": [
+                "ingressSampleRate",
                 "siteName",
-                "hostname",
+                "countSflowCollectors",
+                "id",
                 "agent",
-                "srcAddress6",
-                "egressSampleRate",
                 "sn",
+                "egressSampleRate",
                 "pollingInterval",
-                "srcAddress",
+                "srcAddress6",
+                "hostname",
                 "countSflowSources",
-                "countSflowCollectors",
-                "id",
-                "ingressSampleRate"
+                "srcAddress"
             ],
             "description": "Managed network devices with configured sFlow collectors",
             "method": "post",
             "nested_columns": [],
             "summary": "sFlow Devices",
             "ui_columns": [
                 "hostname",
@@ -8688,24 +8712,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/sflow/sources",
             "api_scope_id": "fb837401d54309a07526cf56705b77604d8ba2c3",
             "columns": [
+                "ingressSampleRate",
                 "siteName",
-                "hostname",
-                "egressSampleRate",
-                "sn",
-                "name",
-                "directions",
-                "pollingInterval",
                 "type",
+                "directions",
                 "id",
-                "ingressSampleRate"
+                "name",
+                "sn",
+                "egressSampleRate",
+                "pollingInterval",
+                "hostname"
             ],
             "description": "Inventory of sources participating in sFlow collection",
             "method": "post",
             "nested_columns": [
                 "directions"
             ],
             "summary": "sFlow Data Sources",
@@ -8728,30 +8752,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses",
             "api_scope_id": "f786373f6201bef7901c1bf4dc314f5264a2b73c",
             "columns": [
-                "description",
+                "licenseName",
+                "index",
+                "licenseType",
+                "reservationStatus",
+                "siteName",
                 "licenseEvalPeriodTotal",
-                "hostname",
-                "numberOfDetails",
+                "id",
+                "licenseInUse",
                 "licenseActive",
-                "siteName",
+                "numberOfDetails",
                 "sn",
-                "reservationStatus",
-                "status",
-                "index",
-                "licenseName",
                 "licensePeriodLeft",
                 "licenseCount",
-                "id",
-                "licenseType",
-                "licenseInUse"
+                "hostname",
+                "description",
+                "status"
             ],
             "description": "Licenses inventory for managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed Licenses",
             "ui_columns": [
                 "hostname",
@@ -8778,23 +8802,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses/cisco-smart-licenses/authorization",
             "api_scope_id": "917f80405318bb3e6b96e276670243646b73c25a",
             "columns": [
+                "lastCommunicationTime",
                 "siteName",
-                "hostname",
+                "id",
+                "authorizationTime",
                 "communicationDeadlineTime",
-                "lastCommunicationStatus",
                 "sn",
-                "status",
-                "lastCommunicationTime",
-                "authorizationTime",
-                "id"
+                "hostname",
+                "lastCommunicationStatus",
+                "status"
             ],
             "description": "Cisco smart license authorization inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco Smart License Authorization",
             "ui_columns": [
                 "hostname",
@@ -8814,24 +8838,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses/cisco-smart-licenses/registration",
             "api_scope_id": "b85a242f2218df05186feff2ab82ff5a51e700c6",
             "columns": [
-                "smartAccount",
+                "initialRegistrationTime",
                 "siteName",
-                "hostname",
                 "initialRegistrationStatus",
+                "registrationExpires",
+                "id",
                 "virtualAccount",
                 "sn",
-                "initialRegistrationTime",
-                "status",
-                "id",
-                "registrationExpires"
+                "smartAccount",
+                "hostname",
+                "status"
             ],
             "description": "Cisco smart license registration inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco Smart License Registration",
             "ui_columns": [
                 "hostname",
@@ -8852,21 +8876,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses/cisco-smart-licenses/reservations",
             "api_scope_id": "cf34c0ca4fb85974d8f90f46fbef5c956a546749",
             "columns": [
-                "siteName",
-                "hostname",
-                "sn",
-                "name",
                 "totalReservedCount",
+                "siteName",
                 "type",
-                "id"
+                "id",
+                "name",
+                "sn",
+                "hostname"
             ],
             "description": "Cisco smart license reservations inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco Smart License Reservations",
             "ui_columns": [
                 "hostname",
@@ -8885,20 +8909,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses/detail",
             "api_scope_id": "797b10d2df5344b4b49eb5ffb62806a75ff69980",
             "columns": [
                 "siteName",
-                "hostname",
-                "sn",
-                "name",
-                "license",
                 "id",
-                "detail"
+                "name",
+                "detail",
+                "sn",
+                "hostname",
+                "license"
             ],
             "description": "Licenses detailed inventory for managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed License detail",
             "ui_columns": [
                 "hostname",
@@ -8916,19 +8940,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses/summary",
             "api_scope_id": "56cd5ca1a301d8086eea37cf5b0f3f3f2a3079ab",
             "columns": [
                 "siteName",
-                "hostname",
-                "numberOfLicenses",
-                "sn",
                 "type",
-                "id"
+                "id",
+                "sn",
+                "hostname",
+                "numberOfLicenses"
             ],
             "description": "Licenses summary inventory including license type and number of licenses",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed License Summary",
             "ui_columns": [
                 "hostname",
@@ -8946,20 +8970,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/logging/local",
             "api_scope_id": "29756ab38005275650d8e2ed736a749407f8a4f2",
             "columns": [
                 "siteName",
-                "hostname",
-                "sn",
-                "fileName",
                 "type",
+                "id",
+                "fileName",
+                "sn",
                 "filters",
-                "id"
+                "hostname"
             ],
             "description": "Local system message logging targets and associated parameters",
             "method": "post",
             "nested_columns": [
                 "filters"
             ],
             "summary": "Local Logging Services",
@@ -8979,27 +9003,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/logging/remote",
             "api_scope_id": "5df3b4c4257934ea75d454e22f0227f5c3b2069f",
             "columns": [
-                "facility",
-                "port",
-                "hostname",
+                "host",
                 "siteName",
+                "port",
                 "srcInterface",
-                "host",
-                "sn",
-                "vrf",
-                "srcAddress",
-                "protocol",
                 "type",
+                "id",
+                "facility",
+                "protocol",
+                "sn",
                 "filters",
-                "id"
+                "vrf",
+                "hostname",
+                "srcAddress"
             ],
             "description": "Remote system message logging targets and associated parameters",
             "method": "post",
             "nested_columns": [
                 "filters"
             ],
             "summary": "Remote Logging Services",
@@ -9025,20 +9049,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/logging/summary",
             "api_scope_id": "5951a8aead84a9c584038cdf5df254a625d6c9ea",
             "columns": [
+                "countRemoteServices",
                 "siteName",
-                "hostname",
+                "id",
                 "sn",
-                "countRemoteServices",
                 "countLocalServices",
-                "id"
+                "hostname"
             ],
             "description": "Summary of the system message logging configuration for remote and local targets configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Logging Summary",
             "ui_columns": [
                 "hostname",
@@ -9055,29 +9079,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/ntp/sources",
             "api_scope_id": "8143afdb75d5e9a6723cbd4cc380555c2c944d74",
             "columns": [
-                "jitter",
-                "when",
                 "siteName",
-                "hostname",
-                "poll",
-                "offset",
-                "sn",
-                "reachable",
-                "reference",
-                "stratum",
                 "flags",
-                "reach",
                 "delay",
+                "reach",
                 "id",
-                "source"
+                "stratum",
+                "source",
+                "sn",
+                "offset",
+                "jitter",
+                "poll",
+                "reference",
+                "hostname",
+                "reachable",
+                "when"
             ],
             "description": "Detailed status of all NTP peerings configured on managed network devices",
             "method": "post",
             "nested_columns": [
                 "flags"
             ],
             "summary": "NTP Sources",
@@ -9105,21 +9129,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/ntp/summary",
             "api_scope_id": "bd057398905b7d0a1f542a44b0d7808e3b2a5a45",
             "columns": [
-                "siteName",
-                "hostname",
-                "reachableSources",
-                "sn",
                 "confSources",
                 "sources",
-                "id"
+                "siteName",
+                "id",
+                "sn",
+                "reachableSources",
+                "hostname"
             ],
             "description": "Summary view for managed network devices and their configured NTP peerings",
             "method": "post",
             "nested_columns": [
                 "sources"
             ],
             "summary": "NTP Summary",
@@ -9139,25 +9163,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/oam/unidirectional-link-detection/interfaces",
             "api_scope_id": "b15757f254cb2f507ab029c8b2a48389b9f83f5e",
             "columns": [
+                "operState",
                 "siteName",
-                "hostname",
-                "intName",
-                "portAdminState",
+                "id",
+                "neighborsCount",
+                "protocol",
                 "sn",
                 "bidState",
-                "portOperState",
-                "protocol",
-                "operState",
-                "neighborsCount",
-                "id"
+                "portAdminState",
+                "hostname",
+                "intName",
+                "portOperState"
             ],
             "description": "Unidirectional Link Detection (UDLD) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "UDLD Interfaces",
             "ui_columns": [
                 "hostname",
@@ -9179,23 +9203,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/oam/unidirectional-link-detection/neighbors",
             "api_scope_id": "b300075b857ff6a82d2646a72f27393cfa1753d3",
             "columns": [
-                "siteName",
-                "hostname",
-                "intName",
                 "deviceId",
+                "siteName",
+                "id",
+                "state",
                 "neighborHostname",
-                "portId",
                 "sn",
-                "state",
-                "id"
+                "portId",
+                "hostname",
+                "intName"
             ],
             "description": "Unidirectional Link Detection (UDLD) neighbors inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "UDLD Neighbors",
             "ui_columns": [
                 "hostname",
@@ -9215,28 +9239,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/osver-consistency",
             "api_scope_id": "7072e17771ff98bb019aab662d660c9b43167816",
             "columns": [
-                "maintenance",
-                "minor",
-                "pctModel",
+                "family",
+                "model",
+                "train",
                 "platform",
-                "pct",
-                "vendor",
                 "major",
-                "version",
-                "train",
-                "rebuild",
-                "model",
-                "family",
                 "id",
-                "count"
+                "pctModel",
+                "rebuild",
+                "version",
+                "minor",
+                "count",
+                "pct",
+                "vendor",
+                "maintenance"
             ],
             "description": "Operating system consistency table presents the variation of OS versions within each platform and family.",
             "method": "post",
             "nested_columns": [],
             "summary": "OS Version Consistency",
             "ui_columns": [
                 "vendor",
@@ -9262,25 +9286,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/port-mirroring",
             "api_scope_id": "33e21fcd65a0e77d842f7e5ac27090b0588f351a",
             "columns": [
+                "src",
                 "siteName",
-                "hostname",
+                "sessionId",
                 "dscr",
-                "sn",
-                "src",
-                "dst",
-                "status",
                 "type",
                 "id",
+                "dst",
                 "params",
-                "sessionId"
+                "sn",
+                "hostname",
+                "status"
             ],
             "description": "Port Mirroring table lists all SPAN, RSPAN and ERSPAN sessions configured in the network with their parameters",
             "method": "post",
             "nested_columns": [],
             "summary": "Port Mirroring",
             "ui_columns": [
                 "hostname",
@@ -9303,19 +9327,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/ptp/interfaces",
             "api_scope_id": "2e1545c12090b11848dcba90747f86c21b5c2877",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
+                "id",
                 "state",
-                "id"
+                "sn",
+                "hostname",
+                "intName"
             ],
             "description": "Precision Time Protocol (PTP) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PTP Interfaces",
             "ui_columns": [
                 "hostname",
@@ -9332,29 +9356,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/ptp/local-clock",
             "api_scope_id": "98f5bcd4708d7b2cc0067be361429a7b8ef49a57",
             "columns": [
-                "mode",
-                "priority2",
-                "siteName",
-                "hostname",
+                "priority1",
                 "meanPathDelay",
-                "offsetFromMaster",
+                "siteName",
                 "numberOfIfaces",
-                "domain",
+                "id",
+                "mode",
+                "source",
                 "sn",
-                "localClockIdentity",
-                "stepsRemoved",
+                "offsetFromMaster",
                 "deviceStatus",
-                "priority1",
-                "id",
-                "source"
+                "domain",
+                "priority2",
+                "localClockIdentity",
+                "hostname",
+                "stepsRemoved"
             ],
             "description": "Precision Time Protocol (PTP) local clock inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PTP Local clock",
             "ui_columns": [
                 "hostname",
@@ -9380,23 +9404,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/ptp/masters",
             "api_scope_id": "97e1325ac052d315a8b74d01428bb43740891ff8",
             "columns": [
-                "parentIPAddress",
-                "siteName",
-                "hostname",
                 "parentClockIdentity",
-                "priority2",
-                "sn",
                 "grandmasterClockIdentity",
                 "priority1",
-                "id"
+                "siteName",
+                "id",
+                "sn",
+                "parentIPAddress",
+                "priority2",
+                "hostname"
             ],
             "description": "Precision Time Protocol (PTP) masters inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PTP Masters",
             "ui_columns": [
                 "hostname",
@@ -9416,37 +9440,37 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/snapshots",
             "api_scope_id": "241f8bca75d6e0f568ec8ef5375e87b91ae20492",
             "columns": [
-                "locked",
-                "finishStatus",
-                "creatorUsername",
-                "deviceRemovedCount",
+                "id",
                 "unloadedSize",
-                "tsStart",
-                "tsChange",
                 "isLastSnapshot",
+                "interfaceCount",
+                "loadedSize",
+                "deviceRemovedCount",
+                "totalDevCount",
+                "sites",
+                "deviceAddedCount",
+                "tsChange",
                 "tsEnd",
+                "locked",
                 "note",
+                "status",
                 "interfaceActiveCount",
-                "name",
-                "loadedSize",
+                "creatorUsername",
+                "finishStatus",
                 "loading",
-                "status",
-                "totalDevCount",
-                "id",
                 "interfaceEdgeCount",
-                "interfaceCount",
                 "userCount",
+                "name",
                 "fromArchive",
-                "deviceAddedCount",
-                "sites"
+                "tsStart"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "sites"
             ],
             "summary": "POST /tables/management/snapshots",
@@ -9484,24 +9508,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/snmp/communities",
             "api_scope_id": "a6e5ab3146ba3c9827722721933cba16f12fbb21",
             "columns": [
-                "group",
                 "siteName",
-                "hostname",
-                "view",
+                "group",
+                "id",
                 "acl",
-                "sn",
-                "name",
                 "authorization",
+                "name",
+                "sn",
                 "prefixes",
-                "id"
+                "hostname",
+                "view"
             ],
             "description": "SNMP communities and the associated scope restrictions configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "SNMP Communities",
             "ui_columns": [
                 "hostname",
@@ -9522,27 +9546,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/snmp/summary",
             "api_scope_id": "2cf111de911fa7e51eb3b937cdd554585e768691",
             "columns": [
-                "communitiesCount",
+                "model",
                 "siteName",
-                "hostname",
-                "usersCount",
-                "sn",
-                "name",
-                "contact",
-                "vendor",
+                "id",
                 "localEngineId",
-                "trapHostsCount",
+                "vendor",
+                "contact",
+                "name",
+                "sn",
                 "location",
-                "model",
-                "id"
+                "usersCount",
+                "trapHostsCount",
+                "hostname",
+                "communitiesCount"
             ],
             "description": "Summary of SNMP protocol configuration on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "SNMP Summary",
             "ui_columns": [
                 "hostname",
@@ -9566,27 +9590,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/snmp/trap-hosts",
             "api_scope_id": "9d89048ea1bfeb940974f945b9a951f060872550",
             "columns": [
-                "dstHost",
+                "vrf",
                 "siteName",
-                "hostname",
+                "type",
                 "srcInterface",
+                "id",
+                "version",
                 "user",
                 "sn",
-                "vrf",
                 "community",
-                "srcIp",
                 "dstPort",
-                "version",
-                "type",
-                "id"
+                "srcIp",
+                "hostname",
+                "dstHost"
             ],
             "description": "Configured destination hosts for SNMP traps and SNMP inform requests",
             "method": "post",
             "nested_columns": [],
             "summary": "SNMP Hosts",
             "ui_columns": [
                 "hostname",
@@ -9610,23 +9634,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/snmp/users",
             "api_scope_id": "c74db4530690b81bc9356d33e5eb29502be8a530",
             "columns": [
-                "group",
                 "siteName",
-                "hostname",
-                "privacy",
+                "group",
+                "id",
                 "acl",
-                "sn",
                 "name",
-                "id",
-                "authentication"
+                "sn",
+                "authentication",
+                "hostname",
+                "privacy"
             ],
             "description": "SNMP users and the associated scope restrictions configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "SNMP Users",
             "ui_columns": [
                 "hostname",
@@ -9646,22 +9670,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/forwarding",
             "api_scope_id": "d8e037c5b3c9d6932a5d838f17f0d658982b50d3",
             "columns": [
+                "labelIn",
+                "nexthop",
                 "siteName",
-                "hostname",
+                "id",
                 "network",
-                "sn",
-                "nexthop",
-                "labelIn",
                 "prefix",
-                "id"
+                "sn",
+                "hostname"
             ],
             "description": "MPLS forwarding table maps labels to their associated next hops",
             "method": "post",
             "nested_columns": [
                 "nexthop"
             ],
             "summary": "MPLS Forwarding",
@@ -9682,32 +9706,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/circuit-cross-connect",
             "api_scope_id": "604b9e48353cdc825ec2ef56045b4182fba73e08",
             "columns": [
-                "ac",
-                "hostname",
+                "neiHostname",
                 "localLabel",
+                "upTrans",
                 "siteName",
+                "stateOrig",
                 "timeLastUp",
-                "neiSn",
-                "sn",
-                "name",
-                "receiveLsp",
-                "remoteLabel",
-                "upTrans",
-                "transmitLsp",
+                "id",
+                "ac",
                 "neiSiteName",
-                "stateOrig",
                 "state",
-                "neiHostname",
                 "neiIp",
-                "id"
+                "name",
+                "sn",
+                "neiSn",
+                "receiveLsp",
+                "transmitLsp",
+                "hostname",
+                "remoteLabel"
             ],
             "description": "L2 VPN circuit cross-connect inventory with associated parameters",
             "method": "post",
             "nested_columns": [
                 "ac"
             ],
             "summary": "Circuit Cross-Connect",
@@ -9735,32 +9759,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/curcit-cross-connect",
             "api_scope_id": "e563a4c649ced703ac8952f3722f242b157fb2f3",
             "columns": [
-                "ac",
-                "hostname",
+                "neiHostname",
                 "localLabel",
+                "upTrans",
                 "siteName",
+                "stateOrig",
                 "timeLastUp",
-                "neiSn",
-                "sn",
-                "name",
-                "receiveLsp",
-                "remoteLabel",
-                "upTrans",
-                "transmitLsp",
+                "id",
+                "ac",
                 "neiSiteName",
-                "stateOrig",
                 "state",
-                "neiHostname",
                 "neiIp",
-                "id"
+                "name",
+                "sn",
+                "neiSn",
+                "receiveLsp",
+                "transmitLsp",
+                "hostname",
+                "remoteLabel"
             ],
             "description": "L2 VPN circuit cross-connect inventory with associated parameters",
             "method": "post",
             "nested_columns": [
                 "ac"
             ],
             "summary": "Circuit Cross-Connect",
@@ -9788,27 +9812,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/point-to-multipoint",
             "api_scope_id": "fb24ca98d610d19369c2d436fff4b309b1f72ad9",
             "columns": [
-                "ac",
-                "hostname",
+                "neiHostname",
                 "siteName",
+                "id",
+                "bridgeDomain",
                 "localIntName",
-                "neiSn",
+                "ac",
+                "neiSiteName",
+                "neiIp",
                 "name",
-                "bridgeDomain",
                 "sn",
-                "neiSiteName",
                 "state",
-                "neiHostname",
-                "neiIp",
-                "id"
+                "neiSn",
+                "hostname"
             ],
             "description": "L2 VPN Virtual Private LAN Service (VPLS) circuits inventory with associated parameters",
             "method": "post",
             "nested_columns": [
                 "ac"
             ],
             "summary": "Point to multipoint - VPLS",
@@ -9833,36 +9857,36 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/point-to-point-vpws",
             "api_scope_id": "fe3360d96de49c731288cde73f4b3936a3e95377",
             "columns": [
-                "ac",
-                "siteName",
-                "routeTargetImport",
-                "sn",
+                "neiHostname",
                 "remoteId",
+                "stateOrig",
+                "id",
+                "neiSiteName",
+                "neiSn",
                 "localLabel",
-                "rd",
-                "routeTargetExport",
-                "neiHostname",
-                "signallingProtocol",
-                "group",
+                "routeTargetImport",
                 "hostname",
-                "neiSn",
-                "vcId",
-                "name",
-                "neiSiteName",
-                "stateOrig",
-                "neiIp",
-                "localId",
                 "remoteLabel",
+                "signallingProtocol",
                 "state",
-                "id"
+                "routeTargetExport",
+                "neiIp",
+                "sn",
+                "siteName",
+                "rd",
+                "group",
+                "ac",
+                "localId",
+                "name",
+                "vcId"
             ],
             "description": "Virtual private wire service (VPWS) Layer 2 VPNs inventory with associated parameters",
             "method": "post",
             "nested_columns": [
                 "routeTargetExport",
                 "routeTargetImport"
             ],
@@ -9897,27 +9921,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/pseudowires",
             "api_scope_id": "fc9af0690e54bee2e22a882b7fa126c55e37d92e",
             "columns": [
+                "neiHostname",
                 "localLabel",
-                "hostname",
-                "intName",
                 "siteName",
-                "neiSn",
-                "sn",
-                "remoteLabel",
-                "neiSiteName",
-                "state",
-                "neiHostname",
                 "type",
+                "id",
+                "state",
+                "neiSiteName",
                 "neiIp",
-                "id"
+                "sn",
+                "neiSn",
+                "hostname",
+                "intName",
+                "remoteLabel"
             ],
             "description": "L2 VPN pseudowires inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "All Pseudowires",
             "ui_columns": [
                 "hostname",
@@ -9941,19 +9965,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/pe-routers",
             "api_scope_id": "1cfed70287e758cc8071aeeeadc4756b1e2d1bcc",
             "columns": [
                 "siteName",
-                "hostname",
-                "ldpIntCount",
+                "id",
                 "sn",
                 "vrfCount",
-                "id"
+                "ldpIntCount",
+                "hostname"
             ],
             "description": "Provider Edge routers inventory participating in L3VPNs",
             "method": "post",
             "nested_columns": [],
             "summary": "PE Routers",
             "ui_columns": [
                 "hostname",
@@ -9970,25 +9994,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/pe-routes",
             "api_scope_id": "065884fa26510a46d9872f036030f82fb718b0f2",
             "columns": [
-                "dstSn",
-                "srcHostname",
-                "prefix",
-                "dstSiteName",
-                "rt",
-                "dstVrf",
                 "dstHostname",
-                "srcSn",
                 "id",
                 "srcVrf",
-                "srcSiteName"
+                "dstSiteName",
+                "srcSiteName",
+                "prefix",
+                "dstVrf",
+                "rt",
+                "srcHostname",
+                "srcSn",
+                "dstSn"
             ],
             "description": "Routes on PE in VRF including originating source PE",
             "method": "post",
             "nested_columns": [],
             "summary": "PE Routes",
             "ui_columns": [
                 "dstHostname",
@@ -10009,22 +10033,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/pe-vrfs",
             "api_scope_id": "bfa6fae289b59bc14e2948a07d67f8f1880d226a",
             "columns": [
-                "af",
-                "siteName",
-                "hostname",
                 "routeCount",
+                "siteName",
                 "rd",
+                "id",
                 "sn",
+                "af",
                 "vrf",
-                "id"
+                "hostname"
             ],
             "description": "VRF configured on PE routers with summary of routes in VRF",
             "method": "post",
             "nested_columns": [
                 "af"
             ],
             "summary": "VRFs on PE Routers",
@@ -10045,23 +10069,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/vrf-targets",
             "api_scope_id": "8be522685b7bba581fa7344211199166a09afab2",
             "columns": [
-                "af",
                 "siteName",
-                "hostname",
-                "exportRT",
+                "importRT",
                 "rd",
+                "id",
                 "sn",
-                "importRT",
+                "af",
+                "exportRT",
                 "vrf",
-                "id"
+                "hostname"
             ],
             "description": "Route targets import and export configured in VRF",
             "method": "post",
             "nested_columns": [
                 "exportRT",
                 "importRT"
             ],
@@ -10084,24 +10108,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/ldp/interfaces",
             "api_scope_id": "0a2ca2f54da9c530f16ff6c93e8ecd217dcd0ad5",
             "columns": [
-                "neiCount",
+                "siteName",
                 "localAddress",
-                "hostname",
-                "intName",
+                "id",
                 "localId",
-                "siteName",
                 "sn",
-                "timerHoldtime",
+                "neiCount",
                 "timerHello",
-                "id"
+                "hostname",
+                "intName",
+                "timerHoldtime"
             ],
             "description": "Label Distribution Protocol (LDP) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "LDP Interfaces",
             "ui_columns": [
                 "hostname",
@@ -10122,33 +10146,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/ldp/neighbors",
             "api_scope_id": "76fbda3767ec3045a39337cfd3ff1d54f1b8bc76",
             "columns": [
-                "localAddress",
-                "siteName",
-                "sn",
+                "neiHostname",
+                "id",
+                "neiSiteName",
+                "neiSn",
+                "neiId",
                 "neiDevType",
-                "target",
+                "intName",
                 "neiAddress",
-                "neiId",
-                "vrf",
-                "neiHostname",
-                "subnet",
+                "neiIntName",
+                "localAddress",
                 "hostname",
-                "intName",
+                "subnet",
+                "source",
+                "sn",
+                "siteName",
                 "currStateTime",
-                "neiSn",
-                "neiIntName",
-                "neiSiteName",
                 "devType",
-                "id",
-                "source"
+                "vrf",
+                "target"
             ],
             "description": "Label Distribution Protocol (LDP) neighbors inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "LDP Neighbors",
             "ui_columns": [
                 "hostname",
@@ -10170,28 +10194,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/rsvp/interfaces",
             "api_scope_id": "1c9518f9324c531a7e3c9ac6e83a25475115ac2c",
             "columns": [
-                "neiCount",
-                "allocatedBw",
-                "localAddress",
-                "hostname",
-                "intName",
-                "siteName",
+                "linkProtectionUnprotectedLsp",
                 "linkProtectionBypass",
+                "siteName",
+                "localAddress",
+                "linkProtectionLsp",
+                "id",
+                "allocatedBw",
+                "linkProtectionProtectedLsp",
+                "sn",
+                "neiCount",
                 "linkProtectionStatus",
                 "maxBw",
-                "sn",
-                "linkProtectionProtectedLsp",
-                "linkProtectionUnprotectedLsp",
-                "id",
-                "linkProtectionLsp"
+                "hostname",
+                "intName"
             ],
             "description": "Resource Reservation Protocol (RSVP) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "RSVP Interfaces",
             "ui_columns": [
                 "hostname",
@@ -10216,38 +10240,38 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/rsvp/neighbors",
             "api_scope_id": "ef6caf43c344e8cdfef7196e1793efd95c1b1645",
             "columns": [
+                "neiHostname",
+                "id",
+                "neiSiteName",
+                "neiSn",
+                "linkProtectionBackupLspsCount",
+                "intName",
+                "neiAddress",
+                "frrLspsCount",
                 "localAddress",
+                "linkProtectionLspName",
                 "frrStatus",
-                "siteName",
-                "sn",
+                "linkProtectionStatus",
+                "hostname",
                 "linkProtectionBypassLsp",
-                "linkProtectionBackupRoutesCount",
-                "linkProtectionBackupLspsCount",
-                "neiAddress",
-                "neiId",
-                "vrf",
-                "neiHostname",
+                "sn",
+                "linkProtectionBypassExplicitRoute",
+                "status",
                 "via",
-                "hostname",
-                "intName",
+                "siteName",
                 "currStateTime",
-                "neiSn",
-                "linkProtectionLspName",
-                "status",
-                "neiSiteName",
-                "linkProtectionBypassExplicitRoute",
                 "localId",
-                "linkProtectionStatus",
-                "frrLspsCount",
-                "id"
+                "linkProtectionBackupRoutesCount",
+                "vrf",
+                "neiId"
             ],
             "description": "Resource Reservation Protocol (RSVP) neighbors inventory",
             "method": "post",
             "nested_columns": [
                 "linkProtectionBypassExplicitRoute"
             ],
             "summary": "RSVP Neighbors",
@@ -10282,26 +10306,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/groups",
             "api_scope_id": "38cc3d8adec28713bc38d8d04415b811fc6672f4",
             "columns": [
-                "uptime",
-                "lastReporter",
+                "groupIp",
                 "siteName",
-                "hostname",
-                "intName",
-                "expires",
+                "lastReporter",
+                "type",
+                "id",
+                "uptime",
                 "sn",
+                "expires",
                 "sourceIp",
                 "vrf",
-                "groupIp",
-                "type",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "Internet Group Management Protocol (IGMP) groups inventory and their associated hosts",
             "method": "post",
             "nested_columns": [],
             "summary": "IGMP Groups",
             "ui_columns": [
                 "hostname",
@@ -10324,26 +10348,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/interfaces",
             "api_scope_id": "ad3146326a1275d2bcbab09d0e8e3a8c18f4ddea",
             "columns": [
+                "lastMemberQueryCount",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "queryInterval",
-                "sn",
-                "vrf",
-                "lastMemberQueryCount",
-                "lastMemberQueryInterval",
-                "querierIp",
                 "queryResponseTime",
                 "version",
-                "id"
+                "sn",
+                "lastMemberQueryInterval",
+                "vrf",
+                "hostname",
+                "intName",
+                "querierIp"
             ],
             "description": "Internet Group Management Protocol (IGMP) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "IGMP Interfaces",
             "ui_columns": [
                 "hostname",
@@ -10366,24 +10390,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/snooping/global",
             "api_scope_id": "f3b9756d2b115896e1e2370da8aea74fe48f9944",
             "columns": [
-                "siteName",
-                "hostname",
                 "v3enabled",
+                "siteName",
+                "id",
+                "enabled",
                 "v3reportSuppression",
-                "omf",
                 "sn",
-                "reportSuppression",
-                "enabled",
-                "id",
-                "v2fastLeave"
+                "omf",
+                "v2fastLeave",
+                "hostname",
+                "reportSuppression"
             ],
             "description": "Internet Group Management Protocol (IGMP) snooping global inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "IGMP Snooping",
             "ui_columns": [
                 "hostname",
@@ -10404,25 +10428,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/snooping/groups",
             "api_scope_id": "11b3b8381499a8e82f53cac2b28e304491788813",
             "columns": [
+                "groupIp",
                 "siteName",
-                "hostname",
-                "flood",
                 "vlan",
-                "intNameList",
+                "type",
+                "id",
+                "version",
                 "sn",
                 "sourceIp",
-                "groupIp",
-                "version",
-                "type",
-                "id"
+                "intNameList",
+                "hostname",
+                "flood"
             ],
             "description": "Internet Group Management Protocol (IGMP) snooping groups inventory",
             "method": "post",
             "nested_columns": [
                 "intNameList"
             ],
             "summary": "IGMP Snooping Groups",
@@ -10447,28 +10471,28 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/snooping/vlans",
             "api_scope_id": "1bac49fe53b01f55508ab37e0e676123d28da514",
             "columns": [
                 "siteName",
-                "hostname",
-                "v3reportSuppression",
-                "v2fastLeave",
                 "vlan",
-                "omf",
+                "floodingToVlan",
+                "id",
+                "enabled",
+                "v3reportSuppression",
+                "lookupMode",
                 "sn",
+                "omf",
                 "explicitTracking",
-                "querierIp",
-                "vlanVpc",
                 "reportSuppression",
-                "enabled",
-                "id",
-                "lookupMode",
-                "floodingToVlan"
+                "v2fastLeave",
+                "hostname",
+                "querierIp",
+                "vlanVpc"
             ],
             "description": "Internet Group Management Protocol (IGMP) snooping VLANs inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "IGMP Snooping Vlans",
             "ui_columns": [
                 "hostname",
@@ -10495,21 +10519,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/mac",
             "api_scope_id": "610c9297a0c6d81127c9b2a4b1ef38ffd268d948",
             "columns": [
                 "siteName",
-                "hostname",
                 "vlan",
-                "intNameList",
-                "sn",
-                "id",
                 "type",
-                "mac"
+                "id",
+                "mac",
+                "sn",
+                "intNameList",
+                "hostname"
             ],
             "description": "Multicast MAC Table inventory",
             "method": "post",
             "nested_columns": [
                 "intNameList"
             ],
             "summary": "Multicast MAC Table",
@@ -10530,37 +10554,37 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/interfaces",
             "api_scope_id": "68755dc320dd425915159c25fa4b0cc39a370575",
             "columns": [
-                "neiCount",
-                "queryTimer",
-                "hostname",
                 "drIp",
-                "intName",
-                "dr",
                 "siteName",
+                "id",
+                "priority",
+                "version",
                 "sn",
-                "vrf",
+                "neiCount",
+                "queryTimer",
                 "ip",
-                "version",
-                "id",
-                "priority"
+                "vrf",
+                "hostname",
+                "intName",
+                "isDr"
             ],
             "description": "Protocol-Independent Multicast (PIM) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PIM Interfaces",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
-                "dr",
+                "isDr",
                 "drIp",
                 "neiCount",
                 "priority",
                 "version",
                 "vrf"
             ],
             "web_endpoint": "/technology/multicast/pim/interfaces"
@@ -10572,53 +10596,53 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/neighbors",
             "api_scope_id": "5f49a26c60451da92a9d644c43b265f74f97be49",
             "columns": [
-                "localAddress",
-                "siteName",
-                "expires",
-                "sn",
-                "neiDevType",
+                "neiHostname",
+                "id",
+                "priority",
+                "neiSiteName",
                 "uptime",
-                "target",
-                "dr",
-                "neiAddress",
-                "vrf",
                 "version",
-                "neiHostname",
-                "subnet",
-                "hostname",
-                "intName",
                 "neiSn",
+                "neiDevType",
+                "intName",
+                "neiAddress",
                 "neiIntName",
-                "neiSiteName",
                 "flags",
-                "priority",
+                "localAddress",
+                "hostname",
+                "subnet",
+                "source",
+                "sn",
+                "siteName",
                 "mode",
                 "devType",
-                "id",
-                "source"
+                "expires",
+                "vrf",
+                "target",
+                "isDr"
             ],
             "description": "Protocol-Independent Multicast (PIM) neighbors inventory",
             "method": "post",
             "nested_columns": [
                 "flags"
             ],
             "summary": "PIM Neighbors",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
                 "localAddress",
                 "mode",
                 "flags",
-                "dr",
+                "isDr",
                 "priority",
                 "neiIntName",
                 "neiHostname",
                 "neiAddress",
                 "vrf",
                 "uptime"
             ],
@@ -10631,22 +10655,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/bsr",
             "api_scope_id": "c01133c1598bf86c392c132b8b3f6747a98008f7",
             "columns": [
-                "bsrRouters",
                 "siteName",
-                "hostname",
-                "sn",
-                "vrf",
                 "bsrIp",
+                "id",
                 "bsrRoutersCount",
-                "id"
+                "sn",
+                "bsrRouters",
+                "vrf",
+                "hostname"
             ],
             "description": "Protocol-Independent Multicast (PIM) rendezvous points (RP) inventory",
             "method": "post",
             "nested_columns": [
                 "bsrRouters"
             ],
             "summary": "PIM Bootstrap RP",
@@ -10667,23 +10691,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/mappings",
             "api_scope_id": "f3bd34f02855b4978032f2e49e05906674bbe8a6",
             "columns": [
-                "rpRouters",
-                "uptime",
                 "siteName",
-                "hostname",
-                "rpIp",
+                "id",
+                "uptime",
                 "sn",
+                "rpRouters",
+                "rpIp",
                 "vrf",
-                "groupsCount",
-                "id"
+                "hostname",
+                "groupsCount"
             ],
             "description": "Protocol-Independent Multicast (PIM) and rendezvous points (RP) mappings",
             "method": "post",
             "nested_columns": [
                 "rpRouters"
             ],
             "summary": "PIM Boostrap RP mappings",
@@ -10705,25 +10729,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/mappings-groups",
             "api_scope_id": "34d0e544083871a64602b364b0c0348985cf2662",
             "columns": [
-                "rpRouters",
-                "uptime",
                 "siteName",
-                "hostname",
-                "rpIp",
+                "id",
+                "uptime",
+                "groupNet",
+                "learnedFrom",
                 "sn",
-                "vrf",
+                "rpRouters",
                 "groupUptime",
-                "learnedFrom",
-                "id",
-                "groupNet"
+                "rpIp",
+                "vrf",
+                "hostname"
             ],
             "description": "Protocol-Independent Multicast (PIM) and rendezvous points (RP) mapping groups",
             "method": "post",
             "nested_columns": [
                 "rpRouters"
             ],
             "summary": "PIM Bootstrap RP mappings groups",
@@ -10747,21 +10771,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/overview",
             "api_scope_id": "4eef5c24a1ac421d259e76caf9e7b34c106a7f6e",
             "columns": [
-                "rpHostname",
-                "vrfList",
-                "siteName",
                 "routersCount",
-                "rpIp",
+                "siteName",
+                "vrfList",
+                "id",
+                "rpHostname",
                 "rpSn",
-                "id"
+                "rpIp"
             ],
             "description": "Rendezvous points (RP) routers inventory",
             "method": "post",
             "nested_columns": [
                 "vrfList"
             ],
             "summary": "RP Routers",
@@ -10781,33 +10805,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/counters",
             "api_scope_id": "a6764383fe5a005530269edb27703c1d789434a1",
             "columns": [
-                "siteName",
+                "id",
                 "inPktsRate",
-                "inPkts",
-                "sn",
+                "avgPkt",
+                "outPktsRate",
                 "rpfNeiIp",
-                "sourceNet",
-                "vrf",
-                "otherErrRate",
+                "rpfErr",
+                "outPkts",
                 "rpfErrRate",
-                "avgPkt",
+                "otherErr",
+                "hostname",
+                "sourceNet",
                 "inIntName",
                 "groupNet",
-                "otherErr",
+                "inPkts",
+                "sn",
+                "otherErrRate",
+                "siteName",
                 "group",
-                "hostname",
-                "outPkts",
-                "rpfErr",
-                "outPktsRate",
-                "id"
+                "vrf"
             ],
             "description": "Multicast routing table counters with RPF and other errors",
             "method": "post",
             "nested_columns": [],
             "summary": "MRoute Counters",
             "ui_columns": [
                 "hostname",
@@ -10838,19 +10862,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/first-hop-router",
             "api_scope_id": "a2d8d8caafa37b2b7cebcdb342ec755b40627a8f",
             "columns": [
                 "siteName",
-                "fwdCount",
-                "hostname",
                 "sourceCount",
+                "id",
                 "sn",
-                "id"
+                "fwdCount",
+                "hostname"
             ],
             "description": "Multicast first hop routers inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Multicast First Hop Routers",
             "ui_columns": [
                 "hostname",
@@ -10867,28 +10891,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/outgoing-interfaces",
             "api_scope_id": "218d0c9b6e89ee9f1c4cc3892b5bd99587c77202",
             "columns": [
+                "family",
+                "flags",
+                "siteName",
                 "group",
+                "id",
+                "age",
                 "mode",
-                "siteName",
-                "hostname",
-                "intName",
-                "sn",
                 "sourceNet",
-                "vrf",
                 "vendor",
-                "flags",
-                "age",
-                "family",
-                "id",
-                "groupNet"
+                "groupNet",
+                "sn",
+                "vrf",
+                "hostname",
+                "intName"
             ],
             "description": "Multicast routing table outgoing interface list detail",
             "method": "post",
             "nested_columns": [
                 "flags"
             ],
             "summary": "Multicast OIL",
@@ -10916,20 +10940,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/overview",
             "api_scope_id": "c2b90837f180df63efa3ab4f67c7114dd86d5a97",
             "columns": [
                 "siteName",
-                "hostname",
                 "activeRoutesCount",
+                "id",
                 "routesCount",
                 "sn",
                 "vrf",
-                "id"
+                "hostname"
             ],
             "description": "Overview of devices with multicast routes in mroute table",
             "method": "post",
             "nested_columns": [],
             "summary": "MRoute Overview",
             "ui_columns": [
                 "hostname",
@@ -10947,26 +10971,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/sources",
             "api_scope_id": "47addb3582a3f5c3e689abc9ddc5085427f7f44e",
             "columns": [
-                "group",
-                "mac",
-                "siteName",
-                "hostname",
-                "sn",
-                "vrf",
-                "sourceNet",
                 "incomingInt",
+                "oilCount",
+                "siteName",
                 "isLocal",
+                "group",
                 "id",
+                "sourceNet",
                 "groupNet",
-                "oilCount"
+                "sn",
+                "mac",
+                "vrf",
+                "hostname"
             ],
             "description": "Routers with multicast sources inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Routers with Multicast Sources",
             "ui_columns": [
                 "hostname",
@@ -10989,30 +11013,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/table",
             "api_scope_id": "a77fd5a614ecdb3c3d3f0fd09c8aff1119c7388b",
             "columns": [
-                "group",
+                "family",
+                "flags",
                 "siteName",
-                "hostname",
+                "group",
+                "id",
+                "age",
                 "rpfNeiIp",
-                "outIntNames",
-                "rpIp",
+                "sourceNet",
                 "inIntName",
+                "groupNet",
                 "sn",
-                "sourceNet",
+                "rpIp",
+                "outIntNames",
                 "vrf",
-                "vendor",
-                "flags",
-                "age",
-                "family",
-                "id",
-                "groupNet"
+                "hostname",
+                "vendor"
             ],
             "description": "Global multicast routing table",
             "method": "post",
             "nested_columns": [
                 "flags",
                 "outIntNames"
             ],
@@ -11042,29 +11066,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/neighbors/all",
             "api_scope_id": "f8a11e7f648c796c51d0edc3e8198382e9b22e11",
             "columns": [
-                "localInt",
-                "netDev",
-                "remoteIpv6List",
+                "remoteIp",
                 "siteName",
-                "remoteInt",
-                "remoteSn",
-                "protocols",
                 "capabilities",
+                "id",
+                "managedDev",
+                "remoteDevType",
+                "localInt",
+                "remoteInt",
                 "remoteHost",
                 "localHost",
-                "remoteDevType",
-                "managedDev",
+                "remoteSn",
+                "protocols",
+                "remoteIpv6List",
                 "localSn",
-                "id",
-                "remoteIp"
+                "netDev"
             ],
             "description": "Discovery protocol neighbors inventory (CDP, LLDP, mDP)",
             "method": "post",
             "nested_columns": [
                 "protocols",
                 "remoteIpv6List"
             ],
@@ -11092,29 +11116,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/neighbors/endpoints",
             "api_scope_id": "6f9d12326a55c51f87ae978c06f0c0a403441108",
             "columns": [
-                "localInt",
-                "netDev",
-                "remoteIpv6List",
+                "remoteIp",
                 "siteName",
-                "remoteInt",
-                "remoteSn",
-                "protocols",
                 "capabilities",
+                "id",
+                "managedDev",
+                "remoteDevType",
+                "localInt",
+                "remoteInt",
                 "remoteHost",
                 "localHost",
-                "remoteDevType",
-                "managedDev",
+                "remoteSn",
+                "protocols",
+                "remoteIpv6List",
                 "localSn",
-                "id",
-                "remoteIp"
+                "netDev"
             ],
             "description": "Endpoints viewed by discover protocols",
             "method": "post",
             "nested_columns": [
                 "protocols",
                 "remoteIpv6List"
             ],
@@ -11141,26 +11165,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/neighbors/unidirectional",
             "api_scope_id": "e354e80204b939083c3f7c3bec2f43fb297d22f3",
             "columns": [
-                "localInt",
-                "remoteIpv6List",
+                "remoteIp",
                 "siteName",
-                "remoteInt",
-                "remoteSn",
-                "protocols",
                 "capabilities",
+                "id",
+                "remoteInt",
+                "localInt",
                 "remoteHost",
                 "localHost",
-                "localSn",
-                "id",
-                "remoteIp"
+                "remoteSn",
+                "protocols",
+                "remoteIpv6List",
+                "localSn"
             ],
             "description": "Unidirectional discovery protocol relationship between managed network devices",
             "method": "post",
             "nested_columns": [
                 "remoteIpv6List",
                 "protocols"
             ],
@@ -11185,25 +11209,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/neighbors/unmanaged",
             "api_scope_id": "02f378dc295d5eaa5fb6e5e0957d19887132dd2e",
             "columns": [
-                "localInt",
-                "remoteIpv6List",
+                "remoteIp",
                 "siteName",
-                "remoteInt",
-                "protocols",
                 "capabilities",
+                "id",
+                "remoteInt",
+                "localInt",
                 "remoteHost",
                 "localHost",
-                "localSn",
-                "id",
-                "remoteIp"
+                "protocols",
+                "remoteIpv6List",
+                "localSn"
             ],
             "description": "Unmanaged neighbors detected by discovery protocols of managed network devices",
             "method": "post",
             "nested_columns": [
                 "protocols",
                 "remoteIpv6List"
             ],
@@ -11228,25 +11252,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks",
             "api_scope_id": "78d74b21341d6a85cdcbcbd23a17d9aaf8e03ea0",
             "columns": [
-                "siteName",
-                "vlanId",
-                "gwcount",
                 "gwV",
-                "hosts",
-                "vrf",
+                "siteName",
                 "gwcountV",
-                "mask",
-                "gw",
+                "hosts",
+                "id",
                 "net",
-                "id"
+                "vlanId",
+                "gw",
+                "mask",
+                "vrf",
+                "gwcount"
             ],
             "description": "Detected Layer 3 network (connected/direct/local) inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed Networks",
             "ui_columns": [
                 "siteName",
@@ -11267,18 +11291,18 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/domain",
             "api_scope_id": "f2253e88edbf0f0db2ad794d08be6aecf37390e7",
             "columns": [
                 "siteName",
-                "routers",
                 "rd",
-                "users",
+                "routers",
                 "id",
+                "users",
                 "networks"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/networks/domain",
             "ui_columns": [
@@ -11298,25 +11322,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/gateway-redundancy",
             "api_scope_id": "ae4a4ce3081fe067d9dc37056bfcdebb4b87d3f2",
             "columns": [
-                "siteName",
-                "vlanId",
-                "gwcount",
                 "gwV",
-                "hosts",
-                "vrf",
+                "siteName",
                 "gwcountV",
-                "mask",
-                "gw",
+                "hosts",
+                "id",
                 "net",
-                "id"
+                "vlanId",
+                "gw",
+                "mask",
+                "vrf",
+                "gwcount"
             ],
             "description": "Inventory of available gateways for each discovered network",
             "method": "post",
             "nested_columns": [],
             "summary": "Gateway Redundancy",
             "ui_columns": [
                 "siteName",
@@ -11335,26 +11359,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/ipv6-routes",
             "api_scope_id": "f3147d62d2934793c72f4fc2cc2f2dfe48cf1272",
             "columns": [
+                "nexthop",
                 "siteName",
-                "hostname",
-                "nhCount",
+                "nhLowestMetric",
+                "id",
                 "network",
+                "prefix",
+                "protocol",
+                "nhLowestAge",
                 "sn",
+                "nhCount",
                 "vrf",
-                "nexthop",
-                "nhLowestMetric",
-                "protocol",
-                "prefix",
-                "id",
-                "nhLowestAge"
+                "hostname"
             ],
             "description": "Global IPv6 routing table",
             "method": "post",
             "nested_columns": [
                 "nexthop"
             ],
             "summary": "IPv6 Routing Table",
@@ -11379,31 +11403,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/path-lookup-checks",
             "api_scope_id": "fd66c4e4b8932edbeaaf88675387bed884fffd18",
             "columns": [
-                "parameters",
-                "srcPorts",
-                "dstPorts",
                 "networkMode",
-                "receiver",
+                "passingTraffic",
                 "result",
-                "src",
                 "securedPath",
-                "vrf",
-                "dst",
-                "expectedPassingTraffic",
                 "settings",
                 "flags",
-                "protocol",
+                "dstPorts",
+                "src",
+                "srcPorts",
                 "type",
                 "id",
-                "passingTraffic"
+                "receiver",
+                "dst",
+                "protocol",
+                "expectedPassingTraffic",
+                "vrf",
+                "parameters"
             ],
             "description": "Saved path simulations inventory, including End-to-End settings intended and simulated result.",
             "method": "post",
             "nested_columns": [
                 "flags",
                 "result"
             ],
@@ -11430,26 +11454,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/policies/prefix-lists/ipv4",
             "api_scope_id": "5343e14f5a81bc4f16ee3efe2257078b10bf7abf",
             "columns": [
-                "action",
-                "hostname",
                 "siteName",
+                "maskEqual",
+                "id",
                 "maskMax",
-                "sn",
+                "sequence",
+                "prefix",
                 "name",
+                "sn",
+                "action",
                 "mask",
-                "maskEqual",
                 "maskMin",
-                "prefix",
-                "id",
-                "sequence"
+                "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/networks/policies/prefix-lists/ipv4",
             "ui_columns": [
                 "hostname",
@@ -11472,25 +11496,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/policies/prefix-lists/ipv6",
             "api_scope_id": "12910b3fba7152fb29785afe67e8d8a757df79a0",
             "columns": [
-                "action",
-                "hostname",
                 "siteName",
+                "maskEqual",
+                "id",
                 "maskMax",
-                "sn",
+                "sequence",
+                "prefix",
                 "name",
-                "maskEqual",
+                "sn",
+                "action",
                 "maskMin",
-                "prefix",
-                "id",
-                "sequence"
+                "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/networks/policies/prefix-lists/ipv6",
             "ui_columns": [
                 "hostname",
@@ -11512,27 +11536,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/policies/routing",
             "api_scope_id": "b05911a0cdc128efc32b4b8c7e523ddb79b298a6",
             "columns": [
-                "action",
-                "hostname",
                 "matchedBytes",
                 "siteName",
-                "continue",
-                "matchedPackets",
-                "sn",
-                "name",
                 "matchList",
-                "setList",
                 "type",
                 "id",
-                "sequence"
+                "sequence",
+                "name",
+                "sn",
+                "action",
+                "matchedPackets",
+                "setList",
+                "continue",
+                "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "matchList",
                 "setList"
             ],
@@ -11540,14 +11564,15 @@
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "name",
                 "type",
                 "sequence",
                 "action",
+                "matchList",
                 "setList",
                 "continue",
                 "matchedPackets",
                 "matchedBytes"
             ],
             "web_endpoint": "/technology/routing/policy/policies"
         },
@@ -11558,22 +11583,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/policies/routing/interfaces",
             "api_scope_id": "c718018bdcbca27e50ce8b156b9277bcb88b85c1",
             "columns": [
+                "addressFamily",
                 "siteName",
+                "id",
+                "name",
+                "sn",
                 "hostname",
                 "intName",
-                "addressFamily",
-                "sn",
-                "name",
-                "status",
-                "id"
+                "status"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/networks/policies/routing/interfaces",
             "ui_columns": [
                 "hostname",
@@ -11591,21 +11616,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/route-stability",
             "api_scope_id": "8ded207b292a9d31bbd7e77008b30a4f78d70b1e",
             "columns": [
-                "ribCount",
                 "presence",
-                "ratioInfo",
+                "ribCount",
                 "ratioCrit",
+                "id",
                 "prefix",
                 "ratioWarn",
-                "id"
+                "ratioInfo"
             ],
             "description": "Unique routed networks, the number of times route is observed, expressed in absolute and percentage values",
             "method": "post",
             "nested_columns": [],
             "summary": "Routing Stability",
             "ui_columns": [
                 "prefix",
@@ -11624,26 +11649,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/routes",
             "api_scope_id": "30e1e29a9e033f86d03a7512dc31fbb36ff1f113",
             "columns": [
+                "nexthop",
                 "siteName",
-                "hostname",
-                "nhCount",
+                "nhLowestMetric",
+                "id",
                 "network",
+                "prefix",
+                "protocol",
+                "nhLowestAge",
                 "sn",
+                "nhCount",
                 "vrf",
-                "nexthop",
-                "nhLowestMetric",
-                "protocol",
-                "prefix",
-                "id",
-                "nhLowestAge"
+                "hostname"
             ],
             "description": "Global IPv4 routing table",
             "method": "post",
             "nested_columns": [
                 "nexthop"
             ],
             "summary": "IPv4 Routing Table",
@@ -11669,24 +11694,24 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols",
             "api_scope_id": "eeb72ee377ca3c157bf8200a204e18f6e28d8492",
             "columns": [
                 "siteName",
-                "hostname",
-                "replicates",
-                "sn",
-                "vrf",
                 "subnets",
+                "id",
                 "memory",
                 "overhead",
+                "sn",
+                "networks",
                 "protocol",
-                "id",
-                "networks"
+                "vrf",
+                "hostname",
+                "replicates"
             ],
             "description": "Summary routing table information about routing protocols for all managed devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Network Routing Protocols Summary",
             "ui_columns": [
                 "hostname",
@@ -11708,23 +11733,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/bgp",
             "api_scope_id": "e2f318fc70da867d8e8e7d8ce3ba9e39135b46e1",
             "columns": [
-                "internal",
-                "hostname",
-                "siteName",
+                "external",
                 "as",
+                "siteName",
+                "id",
+                "local",
                 "sn",
+                "internal",
                 "vrf",
-                "local",
-                "external",
-                "id"
+                "hostname"
             ],
             "description": "Border Gateway Protocol (BGP) routes summary",
             "method": "post",
             "nested_columns": [],
             "summary": "BGP Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
@@ -11745,24 +11770,24 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/eigrp",
             "api_scope_id": "78fc4db6c1f540647668280b112bb33232d20668",
             "columns": [
                 "siteName",
-                "hostname",
-                "replicates",
-                "sn",
-                "vrf",
                 "subnets",
+                "id",
                 "memory",
                 "overhead",
+                "sn",
+                "networks",
                 "protocol",
-                "id",
-                "networks"
+                "vrf",
+                "hostname",
+                "replicates"
             ],
             "description": "Enhanced Interior Gateway Routing Protocol (EIGRP) routes summary",
             "method": "post",
             "nested_columns": [],
             "summary": "EIGRP Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
@@ -11783,22 +11808,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/isis",
             "api_scope_id": "38fae7a5d58999f7e6d6ae5e31d9b15dea8c7738",
             "columns": [
-                "level2",
+                "level1",
                 "siteName",
-                "hostname",
                 "interArea",
+                "id",
+                "level2",
                 "sn",
                 "vrf",
-                "level1",
-                "id"
+                "hostname"
             ],
             "description": "Intermediate System to Intermediate System (IS-IS) routes summary",
             "method": "post",
             "nested_columns": [],
             "summary": "IS-IS Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
@@ -11817,26 +11842,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/ospf",
             "api_scope_id": "395ba95624cadfd1c00e32e63d2eaf520623fa9d",
             "columns": [
-                "nssaEx2",
+                "vrf",
                 "external1",
-                "intraArea",
+                "interArea",
                 "process",
-                "hostname",
-                "nssaEx1",
                 "siteName",
-                "interArea",
+                "id",
+                "nssaEx1",
                 "sn",
-                "vrf",
-                "external2",
-                "id"
+                "nssaEx2",
+                "intraArea",
+                "hostname",
+                "external2"
             ],
             "description": "Open Shortest Path First routes summary",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPF Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
@@ -11859,25 +11884,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/ospfv3",
             "api_scope_id": "362c08e1e4e80909934abee4cb603c6b4f9b16ea",
             "columns": [
-                "nssaEx2",
+                "vrf",
                 "external1",
-                "intraArea",
+                "interArea",
                 "siteName",
-                "hostname",
+                "id",
                 "nssaEx1",
-                "interArea",
                 "sn",
-                "vrf",
-                "external2",
-                "id"
+                "nssaEx2",
+                "intraArea",
+                "hostname",
+                "external2"
             ],
             "description": "Open Shortest Path First v3 (OSPFv3) routes summary",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPFv3 Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
@@ -11900,24 +11925,24 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/rip",
             "api_scope_id": "d7c820202fd1854f4bd45067810489e694f1e9c9",
             "columns": [
                 "siteName",
-                "hostname",
-                "replicates",
-                "sn",
-                "vrf",
                 "subnets",
+                "id",
                 "memory",
                 "overhead",
+                "sn",
+                "networks",
                 "protocol",
-                "id",
-                "networks"
+                "vrf",
+                "hostname",
+                "replicates"
             ],
             "description": "Routing Information Protocol (RIP) routes summary",
             "method": "post",
             "nested_columns": [],
             "summary": "RIP Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
@@ -11938,24 +11963,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/cluster/srx",
             "api_scope_id": "187d681ac6b407b47f3de45fa632c75311e9f838",
             "columns": [
-                "group",
                 "siteName",
-                "hostname",
-                "sn",
-                "name",
                 "clusterId",
-                "state",
                 "type",
+                "group",
                 "id",
-                "priority"
+                "priority",
+                "state",
+                "name",
+                "sn",
+                "hostname"
             ],
             "description": "Juniper SRX Clusters inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Juniper SRX Cluster",
             "ui_columns": [
                 "hostname",
@@ -11976,21 +12001,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/devices",
             "api_scope_id": "cf5fe334d51107ed9476b3f5afbba0f3b2d1c8f1",
             "columns": [
-                "contextId",
                 "siteName",
-                "hostname",
+                "id",
                 "sn",
                 "contextType",
                 "contextName",
-                "id"
+                "contextId",
+                "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/platforms/devices",
             "ui_columns": [
                 "hostname",
@@ -12009,22 +12034,22 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/neighbors",
             "api_scope_id": "35aef73100f72ab0e0126c96f9b94f9a9bb466f5",
             "columns": [
                 "siteName",
-                "hostname",
-                "level",
-                "holdTime",
-                "interfaces",
-                "sn",
                 "systemId",
+                "holdTime",
+                "id",
                 "state",
-                "id"
+                "level",
+                "sn",
+                "hostname",
+                "interfaces"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "interfaces"
             ],
             "summary": "POST /tables/platforms/fabric-path/neighbors",
@@ -12046,22 +12071,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/routes",
             "api_scope_id": "6a0e223d15246ac72e63254b2cb0ad7769207162",
             "columns": [
-                "switchId",
                 "siteName",
-                "hostname",
+                "id",
+                "switchId",
+                "physicalInterfaces",
                 "localId",
                 "sn",
                 "subswitchId",
-                "physicalInterfaces",
-                "id"
+                "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "physicalInterfaces"
             ],
             "summary": "POST /tables/platforms/fabric-path/routes",
@@ -12083,20 +12108,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/summary",
             "api_scope_id": "f83cbf239cf378a0b65d964e461fb71820f0bd4a",
             "columns": [
                 "siteName",
-                "hostname",
-                "routesCount",
-                "sn",
                 "switchesCount",
+                "id",
                 "neighborsCount",
-                "id"
+                "routesCount",
+                "sn",
+                "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/platforms/fabric-path/summary",
             "ui_columns": [
                 "hostname",
@@ -12114,25 +12139,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/switches",
             "api_scope_id": "6a987ce761acb660c58e8a8afa3a6982b4d986b8",
             "columns": [
-                "switchId",
                 "siteName",
-                "hostname",
-                "emulatedAnycast",
-                "sn",
-                "local",
-                "systemId",
-                "static",
                 "flags",
+                "systemId",
+                "id",
                 "state",
-                "id"
+                "local",
+                "switchId",
+                "sn",
+                "emulatedAnycast",
+                "static",
+                "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "flags"
             ],
             "summary": "POST /tables/platforms/fabric-path/switches",
@@ -12156,22 +12181,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fex/interfaces",
             "api_scope_id": "e8d8e9697cbb8eb2b52897d2c0aa1c8ed2499dec",
             "columns": [
-                "fex",
+                "fexIntName",
+                "fexSn",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "sn",
-                "fexSn",
-                "fexIntName",
-                "id"
+                "hostname",
+                "fex",
+                "intName"
             ],
             "description": "Cisco Fabric EXtender (FEX) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco FEX Interfaces",
             "ui_columns": [
                 "hostname",
@@ -12189,21 +12214,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fex/modules",
             "api_scope_id": "e3be061e5ea5e1570781d59f69e82fdcc9577f67",
             "columns": [
-                "fex",
-                "sn",
-                "ver",
+                "model",
                 "parents",
                 "fexId",
-                "model",
-                "id"
+                "id",
+                "sn",
+                "ver",
+                "fex"
             ],
             "description": "Cisco Fabric EXtender (FEX) modules inventory",
             "method": "post",
             "nested_columns": [
                 "parents"
             ],
             "summary": "Cisco FEX Modules",
@@ -12224,26 +12249,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/pairs",
             "api_scope_id": "444b1dcf0a46e57d6e98d7bf9499cabea55e6b1b",
             "columns": [
-                "primaryStatus",
-                "primaryLinkIntName",
+                "secondaryHostname",
+                "primarySn",
                 "siteName",
-                "secondaryLinkIntName",
-                "primaryHostname",
+                "primaryLinkIntName",
+                "systemId",
+                "id",
+                "secondaryStatus",
                 "domain",
-                "secondaryHostname",
+                "secondaryLinkIntName",
+                "primaryStatus",
                 "secondarySn",
-                "secondaryStatus",
-                "systemId",
-                "primarySn",
-                "id"
+                "primaryHostname"
             ],
             "description": "Multi-chassis link aggregation group (MLAG) pairs inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "MLAG Pairs",
             "ui_columns": [
                 "siteName",
@@ -12265,26 +12290,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/peers",
             "api_scope_id": "c319cfac38fbb9ea69aca2ebcb8bd6b85bf09f1b",
             "columns": [
+                "remoteIp",
                 "siteName",
-                "hostname",
-                "domain",
-                "localIp",
-                "sn",
                 "systemId",
-                "status",
-                "linkIntName",
-                "role",
                 "type",
                 "id",
-                "remoteIp"
+                "linkIntName",
+                "sn",
+                "domain",
+                "localIp",
+                "role",
+                "hostname",
+                "status"
             ],
             "description": "Multi-chassis link aggregation group (MLAG) peer-links inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "MLAG Peer Links",
             "ui_columns": [
                 "hostname",
@@ -12308,20 +12333,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/switches",
             "api_scope_id": "e3664685096c7786e0d3ffba191e36ba7a5100cc",
             "columns": [
                 "siteName",
-                "hostname",
-                "domain",
-                "sn",
                 "systemId",
                 "type",
-                "id"
+                "id",
+                "sn",
+                "domain",
+                "hostname"
             ],
             "description": "Multi-chassis link aggregation group (MLAG) switches inventory",
             "method": "post",
             "nested_columns": [
                 "domain",
                 "systemId"
             ],
@@ -12343,23 +12368,23 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/vpc",
             "api_scope_id": "cecba1b8270e3d2ee71559886918522fc8ee42da",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
+                "sn",
                 "keepaliveStatus",
                 "domain",
-                "sn",
-                "status",
                 "role",
-                "id",
-                "configConsistStatus"
+                "configConsistStatus",
+                "hostname",
+                "intName",
+                "status"
             ],
             "description": "Cisco vPC (Virtual Port-Channel) domains and interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco vPC",
             "ui_columns": [
                 "hostname",
@@ -12380,23 +12405,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/poe/devices",
             "api_scope_id": "d5522f6c8199ccf6f7125941ac475625c47f533c",
             "columns": [
-                "operOnCount",
                 "siteName",
-                "hostname",
-                "sn",
                 "powerUsedSum",
-                "poeDeviceClassMax",
-                "powerFromPsSum",
+                "operOnCount",
                 "id",
-                "interfacesCount"
+                "poeDeviceClassMax",
+                "sn",
+                "interfacesCount",
+                "hostname",
+                "powerFromPsSum"
             ],
             "description": "Power over Ethernet (PoE) devices inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PoE devices",
             "ui_columns": [
                 "hostname",
@@ -12416,27 +12441,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/poe/interfaces",
             "api_scope_id": "a6a18c3800462f8f32e2278c7d9152db25430db8",
             "columns": [
-                "admin",
-                "poeDeviceName",
+                "powerUsed",
                 "siteName",
-                "intName",
-                "hostname",
+                "powerFromPs",
+                "id",
+                "powerMax",
                 "powerGranted",
                 "sn",
+                "admin",
+                "poeDeviceName",
+                "poeDeviceClass",
                 "oper",
-                "powerUsed",
-                "powerMax",
-                "powerFromPs",
-                "id",
-                "poeDeviceClass"
+                "hostname",
+                "intName"
             ],
             "description": "Power over Ethernet (PoE) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PoE Interfaces",
             "ui_columns": [
                 "hostname",
@@ -12460,24 +12485,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/poe/modules",
             "api_scope_id": "ec2a43566668c0449697b7c964d76d2ca20215fd",
             "columns": [
+                "wattsRemaining",
+                "siteName",
                 "wattsAvailable",
+                "id",
                 "wattsUsed",
-                "siteName",
-                "hostname",
+                "sn",
                 "wattsUsedPct",
                 "moduleId",
-                "sn",
-                "wattsRemaining",
-                "id",
-                "isPoE"
+                "isPoE",
+                "hostname"
             ],
             "description": "Power over Ethernet (PoE) and associated device modules inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PoE - Device Modules",
             "ui_columns": [
                 "hostname",
@@ -12498,22 +12523,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/stack",
             "api_scope_id": "da7ed9e38b0603a54f286215468a90798f076010",
             "columns": [
+                "master",
                 "siteName",
                 "connectionsCount",
-                "sn",
-                "master",
-                "uptimeLow",
-                "membersCount",
+                "id",
                 "uptimeDiff",
-                "id"
+                "membersCount",
+                "sn",
+                "uptimeLow"
             ],
             "description": "Discovered switch stacks, number of members in each stack, and the total number of stack ports",
             "method": "post",
             "nested_columns": [],
             "summary": "Switch stacks",
             "ui_columns": [
                 "master",
@@ -12532,25 +12557,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/stack/connections",
             "api_scope_id": "f94f12a874c98dc87364fc2b3274d4663aebac6a",
             "columns": [
-                "siteName",
-                "member",
-                "interfaces",
-                "sn",
-                "status",
+                "membersKnownCount",
                 "master",
+                "siteName",
+                "stackPort",
+                "id",
                 "membersCount",
+                "sn",
+                "member",
                 "neiSwitchId",
-                "membersKnownCount",
-                "stackPort",
-                "id"
+                "interfaces",
+                "status"
             ],
             "description": "Switch stack interfaces and their current state",
             "method": "post",
             "nested_columns": [
                 "interfaces"
             ],
             "summary": "Stack Ports",
@@ -12574,29 +12599,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/stack/members",
             "api_scope_id": "07dd88ff9bfac76fd033ed2652b9959d4350972f",
             "columns": [
-                "uptime",
-                "hwVer",
+                "master",
+                "image",
                 "siteName",
-                "member",
                 "pn",
-                "sn",
                 "connectionsCount",
-                "ver",
-                "master",
-                "role",
-                "state",
                 "id",
                 "memberSn",
-                "mac",
-                "image"
+                "state",
+                "uptime",
+                "sn",
+                "member",
+                "hwVer",
+                "ver",
+                "role",
+                "mac"
             ],
             "description": "Stack members and their current state",
             "method": "post",
             "nested_columns": [],
             "summary": "Stack Members",
             "ui_columns": [
                 "master",
@@ -12622,22 +12647,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/vdc/devices",
             "api_scope_id": "d94e8955d01b0b4503056bcf1a4e535aaca43fe3",
             "columns": [
-                "vdcId",
                 "siteName",
-                "hostname",
-                "stpDomain",
                 "rd",
-                "sn",
+                "id",
                 "snHw",
-                "id"
+                "sn",
+                "stpDomain",
+                "vdcId",
+                "hostname"
             ],
             "description": "Cisco Virtual Device Context (VDC) devices inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco VDC Devices",
             "ui_columns": [
                 "siteName",
@@ -12656,26 +12681,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/vss/chassis",
             "api_scope_id": "021e079d6db2f173e8722e92c09e815b79a668f0",
             "columns": [
+                "chassisId",
                 "siteName",
-                "currentStateTime",
-                "hostname",
+                "controlState",
+                "id",
+                "state",
+                "version",
                 "sn",
-                "chassisId",
                 "slot",
-                "version",
-                "state",
                 "fabricState",
-                "controlState",
-                "id",
-                "chassisSn"
+                "hostname",
+                "chassisSn",
+                "currentStateTime"
             ],
             "description": "Cisco Virtual Switching System (VSS) chassis information overview",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco VSS Chassis",
             "ui_columns": [
                 "hostname",
@@ -12698,24 +12723,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/vss/overview",
             "api_scope_id": "5ad3125d271b5320330be789aa30df1ff8983807",
             "columns": [
-                "operatingRedundancyMode",
-                "peerSwitchId",
-                "configuredRedundancyMode",
-                "hostname",
-                "domainNumber",
                 "siteName",
+                "configuredRedundancyMode",
+                "id",
                 "switchId",
+                "peerSwitchId",
+                "operatingRedundancyMode",
                 "sn",
+                "domainNumber",
                 "switchoverReason",
-                "id"
+                "hostname"
             ],
             "description": "Cisco Virtual Switching System (VSS) protocol overview",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco VSS Overview",
             "ui_columns": [
                 "hostname",
@@ -12736,21 +12761,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/vss/vsl",
             "api_scope_id": "c9e20e6789632450df1a0b2a834e16eec52b5d64",
             "columns": [
-                "portList",
                 "siteName",
-                "hostname",
-                "sn",
                 "flags",
                 "portChannel",
-                "id"
+                "id",
+                "sn",
+                "portList",
+                "hostname"
             ],
             "description": "Cisco virtual switch link (VSL) overview",
             "method": "post",
             "nested_columns": [
                 "flags",
                 "portList"
             ],
@@ -12771,22 +12796,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/policies",
             "api_scope_id": "f7e39c75db2bf6e5b61c52246ff3dd0da8207890",
             "columns": [
-                "description",
-                "isSystem",
                 "apiScopeIds",
+                "scopeType",
+                "id",
+                "name",
                 "attributeFilters",
                 "attributeScopeIds",
-                "name",
-                "scopeType",
-                "id"
+                "description",
+                "isSystem"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "apiScopeIds",
                 "attributeScopeIds"
             ],
@@ -12810,28 +12835,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/marking",
             "api_scope_id": "8e867f17d7bc390ac2617361dd25bac7f62a74cb",
             "columns": [
-                "value",
                 "siteName",
-                "intName",
-                "hostname",
-                "policy",
                 "parentPolicy",
+                "type",
+                "id",
+                "childPolicy",
                 "sn",
-                "match",
                 "packets",
-                "childPolicy",
+                "set",
                 "class",
-                "type",
-                "id",
-                "set"
+                "match",
+                "value",
+                "hostname",
+                "policy",
+                "intName"
             ],
             "description": "Quality of Service (QoS) marking policies",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Marking",
             "ui_columns": [
                 "hostname",
@@ -12856,35 +12881,35 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/policing",
             "api_scope_id": "aae6de361822629184e1caea9e9db97574b83bd9",
             "columns": [
-                "siteName",
-                "exceededBps",
-                "sn",
-                "conformedBytes",
-                "bc",
-                "match",
-                "childPolicy",
-                "cir",
-                "intName",
-                "hostname",
-                "conformedPkts",
-                "exceededBytes",
                 "type",
-                "action",
-                "exceededPkts",
-                "policy",
-                "parentPolicy",
+                "id",
                 "policeType",
+                "exceededBytes",
+                "policy",
+                "intName",
+                "cir",
+                "match",
                 "class",
+                "conformedPkts",
+                "hostname",
+                "bc",
+                "sn",
+                "childPolicy",
+                "exceededPkts",
                 "conformedBps",
-                "id"
+                "siteName",
+                "parentPolicy",
+                "conformedBytes",
+                "action",
+                "exceededBps"
             ],
             "description": "Quality of Service (QoS) policing rules'",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Policing",
             "ui_columns": [
                 "hostname",
@@ -12916,30 +12941,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/policy-maps",
             "api_scope_id": "c5c1ff8b85866f16e4fb1b1b1164ce48338d4653",
             "columns": [
-                "rateDrop",
                 "siteName",
-                "hostname",
-                "intName",
-                "rateOffered",
-                "policy",
                 "parentPolicy",
-                "bytes",
+                "rateDrop",
+                "type",
+                "id",
+                "rateInterval",
+                "childPolicy",
+                "rateOffered",
                 "sn",
-                "match",
                 "packets",
-                "childPolicy",
-                "rateInterval",
                 "class",
-                "type",
-                "id"
+                "match",
+                "policy",
+                "hostname",
+                "bytes",
+                "intName"
             ],
             "description": "Quality of Service (QoS) applied service policies to interfaces",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Applied Service-Policies",
             "ui_columns": [
                 "hostname",
@@ -12967,26 +12992,26 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/priority-queuing",
             "api_scope_id": "7f7a72478c960027cff50bf0a3196087f2d2c514",
             "columns": [
                 "siteName",
-                "intName",
-                "hostname",
-                "exDrops",
-                "policy",
                 "parentPolicy",
-                "sn",
-                "match",
+                "type",
+                "id",
                 "childPolicy",
+                "sn",
                 "strictPriority",
                 "class",
-                "type",
-                "id"
+                "match",
+                "exDrops",
+                "hostname",
+                "policy",
+                "intName"
             ],
             "description": "Quality of Service (QoS) policies and classes and associated parameters",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Priority Policies and Classes",
             "ui_columns": [
                 "hostname",
@@ -13010,32 +13035,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/queuing",
             "api_scope_id": "c2280632a9e108c34bd95e84cdc4cd78cbd6de05",
             "columns": [
-                "pktsOutput",
                 "queueDepth",
                 "siteName",
-                "intName",
-                "hostname",
-                "totalDrops",
-                "policy",
                 "parentPolicy",
-                "noBufferDrops",
-                "sn",
-                "match",
+                "type",
+                "totalDrops",
+                "pktsOutput",
+                "id",
+                "queueLimit",
                 "bandwidth",
                 "childPolicy",
-                "queueLimit",
-                "class",
+                "sn",
                 "bytesOutput",
-                "type",
-                "id"
+                "noBufferDrops",
+                "class",
+                "match",
+                "hostname",
+                "policy",
+                "intName"
             ],
             "description": "Quality of Service (QoS) policy and classes queing parameters",
             "method": "post",
             "nested_columns": [
                 "queueLimit"
             ],
             "summary": "QoS Queuing",
@@ -13066,35 +13091,35 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/random-drops",
             "api_scope_id": "aba7749bf3212fffdcf8ffd8aca552af3fe0b33e",
             "columns": [
-                "siteName",
-                "classRandom",
-                "sn",
-                "tailDropPkts",
+                "type",
+                "id",
                 "ranDropPkts",
-                "transBytes",
-                "maxThresh",
-                "match",
-                "tailDropBytes",
-                "childPolicy",
+                "policy",
                 "intName",
+                "minThresh",
+                "transBytes",
+                "class",
                 "hostname",
-                "markProb",
-                "type",
+                "sn",
+                "classRandom",
+                "tailDropPkts",
+                "childPolicy",
                 "transPkts",
-                "minThresh",
-                "policy",
-                "parentPolicy",
+                "tailDropBytes",
+                "maxThresh",
+                "markProb",
                 "ranDropBytes",
-                "class",
-                "id"
+                "siteName",
+                "parentPolicy",
+                "match"
             ],
             "description": "Inventory of classes with a random early drop detection action and associated parameters",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Classes with Random Drops",
             "ui_columns": [
                 "hostname",
@@ -13128,28 +13153,28 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/shaping",
             "api_scope_id": "63b4f74373646727d5fcd62596386a78ba5414c5",
             "columns": [
                 "be",
                 "siteName",
-                "intName",
-                "hostname",
-                "shapeType",
-                "policy",
-                "parentPolicy",
-                "sn",
-                "match",
-                "childPolicy",
                 "cir",
-                "targetRate",
-                "class",
+                "parentPolicy",
                 "type",
+                "targetRate",
                 "id",
-                "bc"
+                "childPolicy",
+                "bc",
+                "sn",
+                "class",
+                "match",
+                "shapeType",
+                "hostname",
+                "policy",
+                "intName"
             ],
             "description": "Quality of Service (QoS) classes and shaping information",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Shaping",
             "ui_columns": [
                 "hostname",
@@ -13176,25 +13201,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/reports/discovery-errors",
             "api_scope_id": "e5974cef09b170765ccc6956db6fd19707d1048f",
             "columns": [
+                "slug",
+                "objectId",
                 "hasLogFile",
+                "id",
+                "errorType",
+                "errorText",
                 "loginIp",
-                "dnsName",
+                "version",
                 "taskId",
                 "loginType",
-                "objectId",
-                "slug",
-                "errorText",
-                "version",
-                "errorType",
-                "id"
+                "dnsName"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/reports/discovery-errors",
             "ui_columns": [
                 "id",
@@ -13218,29 +13243,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/reports/discovery-tasks",
             "api_scope_id": "61217b3ed8eaa861461c820cfb09952ed8e74ede",
             "columns": [
+                "slug",
+                "objectId",
                 "hasLogFile",
-                "attemptCount",
-                "context",
-                "dnsName",
+                "id",
+                "errorType",
+                "vendor",
                 "errorMessage",
+                "context",
                 "errorReasons",
-                "vendor",
-                "status",
-                "ip",
-                "objectId",
-                "slug",
-                "errorType",
                 "mac",
-                "id",
-                "source"
+                "source",
+                "ip",
+                "attemptCount",
+                "dnsName",
+                "status"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "errorReasons"
             ],
             "summary": "POST /tables/reports/discovery-tasks",
@@ -13270,30 +13295,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/reports/eof/detail",
             "api_scope_id": "039af94f43c029e25022d25b6076ad7d6638ae62",
             "columns": [
-                "url",
-                "endMaintenance",
+                "deviceSn",
+                "family",
+                "model",
                 "siteName",
-                "endSupport",
-                "hostname",
-                "platform",
                 "dscr",
+                "platform",
+                "id",
+                "replacement",
                 "sn",
+                "endSupport",
+                "pid",
+                "url",
                 "endSale",
+                "hostname",
                 "vendor",
-                "pid",
-                "model",
-                "replacement",
-                "deviceSn",
-                "family",
-                "id"
+                "endMaintenance"
             ],
             "description": "End of Life (EoL) detailed information on all detected part number for managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Hardware EoL - Detail",
             "ui_columns": [
                 "hostname",
@@ -13320,24 +13345,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/reports/eof/summary",
             "api_scope_id": "61cd2bba1a3963371b948c297d85fe0c4e2758af",
             "columns": [
-                "url",
-                "endMaintenance",
-                "endSupport",
                 "dscr",
+                "id",
                 "pidCount",
+                "replacement",
+                "endSupport",
+                "pid",
+                "url",
                 "endSale",
                 "vendor",
-                "pid",
-                "replacement",
-                "id"
+                "endMaintenance"
             ],
             "description": "End of Life (EoL) summary information on all detected part number for managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Hardware EoL - Summary",
             "ui_columns": [
                 "pidCount",
@@ -13359,18 +13384,18 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/reports/settings-oui",
             "api_scope_id": "3266d5d60fcaa70b8c9e3b3162806abe2b63d73a",
             "columns": [
+                "id",
                 "enabled",
-                "vendor",
                 "oui",
-                "id"
+                "vendor"
             ],
             "description": "Internal database for Organizational Unique Identifier (OUI) to either allow ARP discovery or not",
             "method": "post",
             "nested_columns": [],
             "summary": "Settings for OUI Discovery",
             "ui_columns": [
                 "id",
@@ -13387,21 +13412,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/roles",
             "api_scope_id": "5fedc17c2d4dda62de3bf697f18cabd9179eb0aa",
             "columns": [
-                "isAdmin",
-                "description",
-                "isSystem",
-                "name",
                 "policyIds",
                 "type",
-                "id"
+                "id",
+                "name",
+                "isAdmin",
+                "description",
+                "isSystem"
             ],
             "description": "User management roles database used for user management policies",
             "method": "post",
             "nested_columns": [
                 "policyIds"
             ],
             "summary": "RBAC - User Management Roles",
@@ -13423,43 +13448,43 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/bgp/address-families",
             "api_scope_id": "ab00a7512b6b7830cc84b22c3218ba957dc2a35f",
             "columns": [
-                "totalReceivedPrefixes",
-                "localAddress",
-                "siteName",
-                "devType",
-                "sn",
-                "neiDevType",
+                "neiHostname",
+                "type",
+                "id",
+                "keepalive",
+                "neiSiteName",
                 "localAs",
+                "neiSn",
+                "neiDevType",
+                "neiAddress",
+                "family",
+                "localAddress",
+                "localAddressV6",
+                "dstInt",
+                "hostname",
+                "holdTime",
+                "state",
                 "source",
+                "sn",
+                "totalReceivedPrefixes",
+                "receivedPrefix",
                 "target",
-                "neiAddress",
-                "neiId",
-                "vrf",
-                "neiAs",
-                "neiHostname",
                 "neiAddressV6",
-                "hostname",
+                "siteName",
                 "currStateTime",
-                "holdTime",
-                "neiSn",
-                "neiSiteName",
-                "type",
+                "neiAs",
+                "devType",
                 "localId",
-                "receivedPrefix",
-                "dstInt",
-                "localAddressV6",
-                "state",
-                "family",
-                "id",
-                "keepalive"
+                "vrf",
+                "neiId"
             ],
             "description": "Border Gateway Protocol (BGP) and its address-families inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "BGP Address Families",
             "ui_columns": [
                 "hostname",
@@ -13493,44 +13518,44 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/bgp/neighbors",
             "api_scope_id": "dd990ba242bda2a2ae7c32b374007d4118f3d339",
             "columns": [
-                "totalReceivedPrefixes",
-                "localAddress",
-                "siteName",
-                "sn",
-                "neiDevType",
+                "neiHostname",
+                "type",
+                "id",
+                "keepalive",
+                "neiSiteName",
                 "localAs",
-                "source",
-                "routingPoliciesOut",
-                "target",
+                "neiSn",
+                "neiDevType",
                 "neiAddress",
-                "neiId",
-                "vrf",
-                "neiAs",
+                "localAddress",
                 "srcInt",
-                "neiHostname",
-                "routingPoliciesIn",
-                "neiAddressV6",
+                "localAddressV6",
+                "routingPoliciesOut",
+                "dstInt",
                 "hostname",
-                "currStateTime",
                 "holdTime",
-                "neiSn",
-                "neiSiteName",
-                "type",
-                "localId",
-                "dstInt",
-                "localAddressV6",
                 "state",
+                "routingPoliciesIn",
+                "source",
+                "sn",
+                "totalReceivedPrefixes",
+                "target",
+                "neiAddressV6",
+                "siteName",
+                "currStateTime",
+                "neiAs",
                 "devType",
-                "id",
-                "keepalive"
+                "localId",
+                "vrf",
+                "neiId"
             ],
             "description": "Border Gateway Protocol (BGP) neighbors inventory",
             "method": "post",
             "nested_columns": [
                 "routingPoliciesIn",
                 "routingPoliciesOut"
             ],
@@ -13568,24 +13593,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/eigrp/interfaces",
             "api_scope_id": "89245aacc9087285656253960f60db8626d4c79c",
             "columns": [
-                "neiCount",
                 "siteName",
-                "hostname",
-                "intName",
-                "timerHold",
+                "id",
                 "sn",
-                "vrf",
-                "localAsn",
+                "timerHold",
+                "neiCount",
                 "timerHello",
-                "id"
+                "vrf",
+                "hostname",
+                "intName",
+                "localAsn"
             ],
             "description": "Enhanced Interior Gateway Routing Protocol (EIGRP) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "EIGRP Interfaces",
             "ui_columns": [
                 "hostname",
@@ -13606,34 +13631,34 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/eigrp/neighbors",
             "api_scope_id": "b6e85f47108d926ca2d8f766f265e4252b8af2d6",
             "columns": [
-                "localAddress",
-                "siteName",
-                "sn",
-                "neiAsn",
-                "neiDevType",
-                "target",
-                "neiAddress",
-                "vrf",
                 "neiHostname",
+                "id",
+                "neiSiteName",
+                "neiSn",
+                "neiDevType",
+                "intName",
                 "localAsn",
-                "subnet",
+                "neiAddress",
+                "neiIntName",
+                "localAddress",
                 "hostname",
-                "intName",
+                "subnet",
+                "source",
+                "sn",
+                "siteName",
                 "currStateTime",
-                "neiSn",
-                "neiIntName",
-                "neiSiteName",
                 "devType",
-                "id",
-                "source"
+                "neiAsn",
+                "vrf",
+                "target"
             ],
             "description": "Enhanced Interior Gateway Routing Protocol (EIGRP) neighbors inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "EIGRP Neighbors",
             "ui_columns": [
                 "hostname",
@@ -13656,25 +13681,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/is-is/interfaces",
             "api_scope_id": "87fea9657fe0ceecd66e5224177421ca1f5ce7d4",
             "columns": [
-                "levelConfig",
-                "neiCount",
+                "snpa",
                 "siteName",
-                "hostname",
                 "circuitType",
-                "intName",
+                "circuitLevel",
+                "id",
                 "sn",
+                "levelConfig",
+                "neiCount",
                 "vrf",
-                "snpa",
-                "circuitLevel",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "Intermediate System to Intermediate System (IS-IS) interfaces inventory",
             "method": "post",
             "nested_columns": [
                 "levelConfig"
             ],
             "summary": "IS-IS Interfaces",
@@ -13697,31 +13722,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/is-is/levels",
             "api_scope_id": "36c54e7ed0ada944d83143b02fce5e1b6e3c5a50",
             "columns": [
+                "localPassive",
+                "localHoldTime",
                 "siteName",
-                "hostname",
-                "intName",
                 "localHello",
-                "remoteIntName",
                 "localPriority",
+                "id",
+                "state",
+                "localMetric",
                 "remoteSiteName",
-                "remoteSn",
                 "remoteHostname",
+                "remoteSn",
                 "sn",
-                "localPassive",
-                "localMetric",
-                "state",
-                "remoteMetric",
                 "localLevel",
-                "id",
-                "localHoldTime"
+                "hostname",
+                "intName",
+                "remoteMetric",
+                "remoteIntName"
             ],
             "description": "Intermediate System to Intermediate System (IS-IS) interface level config",
             "method": "post",
             "nested_columns": [],
             "summary": "IS-IS Levels",
             "ui_columns": [
                 "hostname",
@@ -13746,43 +13771,43 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/is-is/neighbors",
             "api_scope_id": "06df6fbcc2030512927e6815328eefec4f46828f",
             "columns": [
+                "neiHostname",
+                "id",
+                "neiSiteName",
+                "neiSn",
+                "neiSystemName",
+                "neiDevType",
+                "intName",
+                "neiAddress",
+                "neiIntName",
                 "localAddress",
-                "siteName",
+                "localAddressV6",
+                "hostname",
+                "subnet",
+                "state",
+                "source",
                 "sn",
-                "neiDevType",
+                "neiSnpa",
+                "neiAreas",
                 "localIsType",
-                "neiSystemName",
                 "target",
-                "neiAddress",
-                "neiId",
-                "vrf",
-                "neiHostname",
                 "neiAddressV6",
-                "neiSnpa",
-                "subnet",
-                "hostname",
-                "intName",
-                "currStateTime",
-                "neiSn",
-                "neiIntName",
-                "neiSiteName",
-                "neiIsType",
-                "localId",
-                "neiAreas",
                 "localAreas",
-                "localAddressV6",
-                "state",
+                "siteName",
+                "currStateTime",
                 "devType",
-                "id",
-                "source"
+                "localId",
+                "neiIsType",
+                "vrf",
+                "neiId"
             ],
             "description": "Intermediate System to Intermediate System (IS-IS) neighbors inventory",
             "method": "post",
             "nested_columns": [
                 "localAreas",
                 "neiAreas"
             ],
@@ -13815,21 +13840,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv4-databases",
             "api_scope_id": "94a94b1c9b12da2128990bf5be0eb070341c7ce1",
             "columns": [
                 "siteName",
-                "hostname",
-                "ipv6DatabaseServer",
-                "instanceId",
-                "sn",
                 "ipv4DatabaseServer",
+                "id",
                 "state",
-                "id"
+                "instanceId",
+                "sn",
+                "hostname",
+                "ipv6DatabaseServer"
             ],
             "description": "IPv4 LISP Mapping and Location Repository",
             "method": "post",
             "nested_columns": [],
             "summary": "LISP IPv4 Map Resolvers",
             "ui_columns": [
                 "hostname",
@@ -13849,19 +13874,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv4-routes",
             "api_scope_id": "001289a019fb26a672faf56dabb15568d05efb32",
             "columns": [
                 "siteName",
-                "hostname",
+                "id",
                 "instanceId",
-                "registeredIp",
                 "sn",
-                "id",
+                "registeredIp",
+                "hostname",
                 "eidPrefix"
             ],
             "description": "IPv4 LISP table, Address mapping and routing",
             "method": "post",
             "nested_columns": [],
             "summary": "LISP IPv4 Routes",
             "ui_columns": [
@@ -13881,21 +13906,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv6-databases",
             "api_scope_id": "ebc89ae2d2a9b56d704f231e22c958e0c6364cd2",
             "columns": [
                 "siteName",
-                "hostname",
-                "ipv6DatabaseServer",
-                "instanceId",
-                "sn",
                 "ipv4DatabaseServer",
+                "id",
                 "state",
-                "id"
+                "instanceId",
+                "sn",
+                "hostname",
+                "ipv6DatabaseServer"
             ],
             "description": "IPv6 LISP Mapping and Location Repository",
             "method": "post",
             "nested_columns": [],
             "summary": "LISP IPv6 Map Resolvers",
             "ui_columns": [
                 "hostname",
@@ -13915,19 +13940,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv6-routes",
             "api_scope_id": "a83be2b9707e15fbb5b8e2c616a10b2f91bb841a",
             "columns": [
                 "siteName",
-                "hostname",
+                "id",
                 "instanceId",
-                "registeredIp",
                 "sn",
-                "id",
+                "registeredIp",
+                "hostname",
                 "eidPrefix"
             ],
             "description": "IPv6 LISP table, Address mapping and routing",
             "method": "post",
             "nested_columns": [],
             "summary": "LISP IPv6 Routes",
             "ui_columns": [
@@ -13946,33 +13971,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf-v3/interfaces",
             "api_scope_id": "8f6d2fe138d03dac5eda01f1c8263d3638141228",
             "columns": [
-                "timerWait",
-                "siteName",
-                "instanceId",
-                "sn",
-                "timerDead",
+                "id",
+                "priority",
                 "cost",
-                "neiCount",
                 "timerRetransmit",
+                "processId",
+                "intName",
                 "area",
                 "networkType",
                 "timerHello",
+                "timerWait",
                 "hostname",
-                "intName",
-                "addressFamily",
-                "processId",
-                "priority",
                 "routerId",
                 "state",
-                "id"
+                "sn",
+                "addressFamily",
+                "siteName",
+                "timerDead",
+                "instanceId",
+                "neiCount"
             ],
             "description": "Open Shortest Path First v3 (OSPFv3) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPF v3 Interfaces",
             "ui_columns": [
                 "hostname",
@@ -14002,42 +14027,42 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf-v3/neighbors",
             "api_scope_id": "c31a9db0e79d5d487e0f933cf5d04a1bc755384e",
             "columns": [
-                "localAddress",
-                "siteName",
-                "sn",
+                "neiHostname",
+                "localCost",
+                "id",
+                "priority",
+                "neiSiteName",
+                "neiSn",
                 "neiDevType",
+                "intName",
+                "neiAddress",
+                "neiIntName",
+                "localAddress",
                 "neiCost",
-                "bdr",
-                "target",
+                "hostname",
                 "dr",
-                "neiAddress",
-                "neiId",
-                "vrf",
-                "localCost",
-                "neiHostname",
                 "subnet",
-                "hostname",
-                "intName",
-                "currStateTime",
-                "addressFamily",
-                "neiSn",
-                "neiIntName",
-                "neiSiteName",
-                "priority",
-                "neiArea",
                 "state",
+                "source",
+                "neiArea",
+                "sn",
+                "target",
+                "addressFamily",
+                "siteName",
+                "currStateTime",
                 "localArea",
                 "devType",
-                "id",
-                "source"
+                "bdr",
+                "vrf",
+                "neiId"
             ],
             "description": "Open Shortest Path First v3 (OSPFv3) neighbors inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPF v3 Neighbors",
             "ui_columns": [
                 "hostname",
@@ -14068,31 +14093,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf/interfaces",
             "api_scope_id": "84f41fd8a870c5a4d9dc9f88417e59666c493b9a",
             "columns": [
-                "timerWait",
-                "neiCount",
                 "siteName",
-                "hostname",
-                "intName",
+                "routerId",
+                "timerDead",
+                "area",
+                "id",
+                "priority",
+                "state",
                 "timerRetransmit",
+                "timerHello",
                 "sn",
-                "area",
-                "timerDead",
                 "networkType",
                 "processId",
-                "timerHello",
+                "neiCount",
                 "cost",
-                "routerId",
-                "state",
-                "id",
-                "priority"
+                "timerWait",
+                "hostname",
+                "intName"
             ],
             "description": "Open Shortest Path First (OSPF) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPF Interfaces",
             "ui_columns": [
                 "hostname",
@@ -14120,41 +14145,41 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf/neighbors",
             "api_scope_id": "7937e1737301106eca31020b0c44947fa0eabf0e",
             "columns": [
-                "localAddress",
-                "siteName",
-                "sn",
+                "neiHostname",
+                "localCost",
+                "id",
+                "priority",
+                "neiSiteName",
+                "neiSn",
                 "neiDevType",
+                "intName",
+                "neiAddress",
+                "neiIntName",
+                "localAddress",
                 "neiCost",
-                "bdr",
-                "target",
+                "hostname",
                 "dr",
-                "neiAddress",
-                "neiId",
-                "vrf",
-                "localCost",
-                "neiHostname",
                 "subnet",
-                "hostname",
-                "intName",
-                "currStateTime",
-                "neiSn",
-                "neiIntName",
-                "neiSiteName",
-                "priority",
-                "neiArea",
                 "state",
+                "source",
+                "neiArea",
+                "sn",
+                "target",
+                "siteName",
+                "currStateTime",
                 "localArea",
                 "devType",
-                "id",
-                "source"
+                "bdr",
+                "vrf",
+                "neiId"
             ],
             "description": "Open Shortest Path First (OSPF) neighbors inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPF Neighbors",
             "ui_columns": [
                 "hostname",
@@ -14184,25 +14209,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/rip/interfaces",
             "api_scope_id": "e13369c009bcf86cf61f1ac3b5c60d1eb15204c7",
             "columns": [
-                "neiCount",
+                "timerHolddown",
                 "siteName",
-                "hostname",
-                "intName",
+                "timerUpdate",
                 "verReceive",
-                "timerInvalid",
-                "sn",
-                "timerHolddown",
                 "verSend",
-                "timerUpdate",
+                "timerInvalid",
                 "id",
+                "sn",
+                "neiCount",
+                "hostname",
+                "intName",
                 "timerFlush"
             ],
             "description": "Routing Information Protocol (RIP) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "RIP Interfaces",
             "ui_columns": [
@@ -14226,32 +14251,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/rip/neighbors",
             "api_scope_id": "9a0af78f7deea13b3f3ab3a8e232d40a9929718a",
             "columns": [
-                "localAddress",
-                "hostname",
-                "intName",
+                "neiHostname",
                 "neiAddress",
-                "siteName",
+                "neiIntName",
                 "currStateTime",
-                "subnet",
-                "neiSn",
+                "localAddress",
+                "siteName",
+                "id",
+                "neiSiteName",
+                "devType",
+                "source",
                 "sn",
+                "neiSn",
                 "target",
-                "vrf",
-                "neiIntName",
                 "neiDevType",
-                "neiSiteName",
-                "neiHostname",
-                "devType",
-                "id",
-                "source"
+                "vrf",
+                "hostname",
+                "subnet",
+                "intName"
             ],
             "description": "Routing Information Protocol (RIP) neighbors inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "RIP Neighbors",
             "ui_columns": [
                 "hostname",
@@ -14271,16 +14296,16 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/scopes/api",
             "api_scope_id": "751705d05842f7c672be15f08a3b6b124f353c3a",
             "columns": [
-                "path",
                 "method",
+                "path",
                 "id"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/scopes/api",
             "ui_columns": [
@@ -14297,16 +14322,16 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/scopes/attributes",
             "api_scope_id": "ddacd53c6de2d12f2132ac504528ef0aa8c4f0e4",
             "columns": [
-                "attributeFilters",
-                "id"
+                "id",
+                "attributeFilters"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/scopes/attributes",
             "ui_columns": [
                 "id",
@@ -14321,26 +14346,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/sdwan/links",
             "api_scope_id": "4373ef2e727cfd894d709e6ee1c2adebc37299e2",
             "columns": [
-                "encapsulation",
-                "endpointIp",
+                "slug",
                 "siteName",
-                "hostname",
                 "port",
-                "interfaces",
+                "endpointIp",
+                "id",
+                "encapsulation",
                 "sn",
                 "name",
-                "slug",
                 "linkName",
-                "id",
-                "organization"
+                "organization",
+                "hostname",
+                "interfaces"
             ],
             "description": "Versa SD-WAN transport links inventory",
             "method": "post",
             "nested_columns": [
                 "interfaces"
             ],
             "summary": "Versa Transport links",
@@ -14365,25 +14390,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/sdwan/sites",
             "api_scope_id": "434860af8c796bee668e396b23a3800dabe67abc",
             "columns": [
-                "uptime",
-                "siteName",
-                "hostname",
-                "sn",
-                "name",
-                "status",
                 "slug",
                 "remoteMgmtIp",
-                "id",
+                "siteName",
                 "type",
-                "organization"
+                "id",
+                "uptime",
+                "sn",
+                "name",
+                "organization",
+                "hostname",
+                "status"
             ],
             "description": "Versa SD-WAN sites inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Versa Sites",
             "ui_columns": [
                 "hostname",
@@ -14406,23 +14431,23 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/accounting",
             "api_scope_id": "7d5d6fce92648a1e7036920a8a475acc81b47832",
             "columns": [
                 "siteName",
-                "hostname",
-                "nextMethods",
-                "primaryMethod",
-                "sn",
-                "name",
                 "secondaryMethod",
                 "type",
                 "id",
-                "params"
+                "name",
+                "params",
+                "primaryMethod",
+                "sn",
+                "nextMethods",
+                "hostname"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) accounting methods configured on managed network devices",
             "method": "post",
             "nested_columns": [
                 "nextMethods",
                 "params"
             ],
@@ -14447,23 +14472,23 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/authentication",
             "api_scope_id": "e2518f971c68f9282fc275f692f077cd22ecbec7",
             "columns": [
                 "siteName",
-                "hostname",
-                "nextMethods",
-                "primaryMethod",
-                "sn",
-                "name",
                 "secondaryMethod",
                 "type",
                 "id",
-                "params"
+                "name",
+                "params",
+                "primaryMethod",
+                "sn",
+                "nextMethods",
+                "hostname"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) authentication methods configured on managed network devices",
             "method": "post",
             "nested_columns": [
                 "nextMethods",
                 "params"
             ],
@@ -14488,23 +14513,23 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/authorization",
             "api_scope_id": "fbcbd2df73f1c55b18116b639ae16d52ae7a45ed",
             "columns": [
                 "siteName",
-                "hostname",
-                "nextMethods",
-                "primaryMethod",
-                "sn",
-                "name",
                 "secondaryMethod",
                 "type",
                 "id",
-                "params"
+                "name",
+                "params",
+                "primaryMethod",
+                "sn",
+                "nextMethods",
+                "hostname"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) authorization methods configured on managed network devices",
             "method": "post",
             "nested_columns": [
                 "nextMethods",
                 "params"
             ],
@@ -14528,29 +14553,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/lines",
             "api_scope_id": "23943cd1167404a7fb4c5a3d10da10fece0db4f0",
             "columns": [
-                "type",
-                "siteName",
-                "hostname",
-                "idType",
-                "outTransports",
-                "sn",
                 "authenServiceList",
-                "inAclAllVrfs",
+                "siteName",
                 "authorServiceList",
-                "idList",
-                "inAcl",
-                "inTransports",
+                "type",
                 "outAcl",
                 "id",
-                "accntServiceList"
+                "idList",
+                "inAclAllVrfs",
+                "outTransports",
+                "accntServiceList",
+                "sn",
+                "inTransports",
+                "idType",
+                "inAcl",
+                "hostname"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) lines configured on managed network devices",
             "method": "post",
             "nested_columns": [
                 "inTransports",
                 "outTransports"
             ],
@@ -14579,18 +14604,18 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/password-strength",
             "api_scope_id": "b0a1aacfd62f7cb433535972f64db404a46146a6",
             "columns": [
                 "siteName",
-                "hostname",
-                "passwordStrengthCheck",
+                "id",
                 "sn",
-                "id"
+                "passwordStrengthCheck",
+                "hostname"
             ],
             "description": "Inventory of managed network devices with enabled/disabled passowrd strength check",
             "method": "post",
             "nested_columns": [],
             "summary": "Password Strength",
             "ui_columns": [
                 "hostname",
@@ -14606,27 +14631,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/servers",
             "api_scope_id": "bfc77f153b2e7f31ef0423d152543d30a7cfee17",
             "columns": [
-                "port",
-                "hostname",
-                "intName",
+                "dstHostname",
+                "cfgName",
                 "siteName",
+                "port",
+                "type",
+                "id",
                 "srvGroupName",
-                "cfgName",
+                "protocol",
                 "sn",
-                "srcIp",
                 "ip",
-                "protocol",
-                "dstHostname",
-                "type",
-                "id"
+                "srcIp",
+                "hostname",
+                "intName"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "AAA Servers",
             "ui_columns": [
                 "hostname",
@@ -14650,21 +14675,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/users",
             "api_scope_id": "7efe128b51b65baa80516cf9482b93015424673a",
             "columns": [
-                "privilege",
                 "siteName",
-                "hostname",
+                "privilege",
+                "id",
                 "sn",
-                "username",
                 "groups",
-                "id"
+                "hostname",
+                "username"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) loca configured on managed network devices",
             "method": "post",
             "nested_columns": [
                 "groups"
             ],
             "summary": "AAA Local Users",
@@ -14684,67 +14709,67 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/acl",
             "api_scope_id": "2d1639f5c081d9043a7416cfc439f2d176a7148a",
             "columns": [
-                "interfaceOutZone",
-                "siteName",
-                "ruleNameNumeric",
-                "tcpFlags",
-                "ipSrcRegion",
-                "interfaceIn",
-                "sn",
-                "others",
-                "udpDst",
+                "vxlanSrcGrp",
                 "ipTtl",
-                "ipSrc",
-                "interfaceOut",
+                "id",
+                "l4Dst",
+                "tcpFlags",
+                "actionOriginal",
+                "udpSrc",
+                "description",
+                "ipProtocol",
+                "referencedTests",
+                "l4Src",
+                "active",
+                "ipDscp",
+                "l7Application",
                 "ipPacketLength",
+                "icmpType",
+                "ipPrecedence",
+                "mplsLabelIn",
+                "hostname",
+                "ipTos",
+                "ipSrc",
                 "srcPorts",
+                "policyName",
+                "interfaceOut",
+                "ipSrcRegion",
                 "ipv6Src",
-                "vxlanVni",
+                "tcpDst",
+                "icmpCode",
                 "ruleName",
-                "actionOriginal",
-                "ipDst",
-                "mplsLabelIn",
-                "ipFragmentOffset",
+                "interfaceOutZone",
                 "tcpSrc",
-                "icmpCode",
-                "referencedTests",
-                "icmpIcmpv6",
+                "optionsTracked",
+                "ipDstRegion",
+                "interfaceIn",
+                "vxlanVni",
+                "others",
+                "vxlanDstGrp",
+                "sn",
+                "udpDst",
+                "interfaceIntraZone",
+                "siteName",
+                "ipv6Dst",
                 "dstPorts",
-                "hostname",
-                "ipProtocol",
-                "interfaceInterZone",
                 "uid",
-                "l7Application",
-                "ipv6Dst",
-                "ipPrecedence",
-                "tcpDst",
-                "interfaceIntraZone",
-                "interfaceInZone",
-                "ipDstRegion",
-                "vxlanSrcGrp",
-                "ipDscp",
-                "l4Src",
-                "icmpType",
-                "description",
-                "ipTos",
+                "icmpIcmpv6",
+                "ipFragmentOffset",
+                "ruleNameNumeric",
+                "interfaceVrf",
                 "action",
+                "interfaceInZone",
                 "ruleNumber",
-                "policyName",
-                "interfaceVrf",
-                "l4Dst",
-                "vxlanDstGrp",
-                "optionsTracked",
-                "active",
-                "udpSrc",
-                "id"
+                "interfaceInterZone",
+                "ipDst"
             ],
             "description": "Detailed network access control list (ACL) information on managed network devices",
             "method": "post",
             "nested_columns": [
                 "interfaceIn",
                 "interfaceOut",
                 "interfaceInZone",
@@ -14832,19 +14857,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/acl/global-policies",
             "api_scope_id": "d5d1bac547ea78b54feae7edc6a6f1e6f17b1f65",
             "columns": [
                 "siteName",
-                "hostname",
-                "sn",
-                "outputPolicy",
                 "inputPolicy",
-                "id"
+                "outputPolicy",
+                "id",
+                "sn",
+                "hostname"
             ],
             "description": "Global access control list (ACL) policies configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Global ACL policies",
             "ui_columns": [
                 "hostname",
@@ -14862,20 +14887,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/acl/interfaces",
             "api_scope_id": "a942092c49050b26e00d4de74b495b885caffb97",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
                 "outAcl",
+                "id",
+                "sn",
                 "inAcl",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "Interfaces with packet filters or access control lists (ACL) applied",
             "method": "post",
             "nested_columns": [
                 "inAcl",
                 "outAcl"
             ],
@@ -14896,24 +14921,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/dhcp/bindings",
             "api_scope_id": "b812b5db4781705202cde2ec12001c2f08806f70",
             "columns": [
-                "leaseIp",
-                "type",
+                "leaseTimeout",
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
+                "type",
+                "id",
+                "leaseIp",
                 "sn",
-                "leaseTimeout",
+                "vlanId",
                 "mac",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "DHCP Snooping binding database inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Snooping Binding Database",
             "ui_columns": [
                 "hostname",
@@ -14934,31 +14959,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/dhcp/snooping",
             "api_scope_id": "5a9cb46d953e42a28ca098c8264985e8b31b69eb",
             "columns": [
-                "macVerification",
-                "dbWriteDelay",
+                "trustedPortList",
+                "dbLocation",
                 "siteName",
-                "hostname",
+                "circuitId",
+                "remoteId",
+                "insertion",
+                "id",
+                "enabled",
                 "vendorId",
                 "packetsDropped",
                 "sn",
-                "enabledVlanList",
-                "untrustedPolicy",
+                "hostname",
                 "packetsTotal",
-                "insertion",
-                "dbLocation",
-                "enabled",
-                "circuitId",
-                "trustedPortList",
-                "id",
-                "remoteId"
+                "macVerification",
+                "untrustedPolicy",
+                "enabledVlanList",
+                "dbWriteDelay"
             ],
             "description": "DHCP Snooping configuration parameters for managed network devices",
             "method": "post",
             "nested_columns": [
                 "enabledVlanList",
                 "trustedPortList"
             ],
@@ -14989,24 +15014,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/dmvpn",
             "api_scope_id": "3cdb4dcd074059f66ad395b16f8c998c3d4f836b",
             "columns": [
+                "peerNbma",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
+                "state",
                 "peerTunnel",
                 "sn",
-                "peerNbma",
                 "time",
-                "attrb",
-                "state",
-                "id"
+                "hostname",
+                "intName",
+                "attrb"
             ],
             "description": "dynamic multipoint virtual private network (DMVPN) tunnels inventory ",
             "method": "post",
             "nested_columns": [],
             "summary": "DMVPN Summary",
             "ui_columns": [
                 "hostname",
@@ -15027,26 +15052,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/enabled-telnet",
             "api_scope_id": "25300ae072614ab6593ce7189bf2ee5c046fe0a2",
             "columns": [
+                "image",
+                "siteName",
+                "id",
                 "uptime",
                 "loginIp",
-                "siteName",
-                "hostname",
-                "sn",
                 "processor",
-                "configReg",
-                "loginType",
                 "reload",
                 "version",
-                "id",
-                "image"
+                "sn",
+                "loginType",
+                "configReg",
+                "hostname"
             ],
             "description": "Managed network devices with enabled Telnet access",
             "method": "post",
             "nested_columns": [],
             "summary": "Telnet Access",
             "ui_columns": [
                 "hostname",
@@ -15070,39 +15095,41 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/ipsec/gateways",
             "api_scope_id": "59c972df31071ad177740ebaf89adcaea46b6ad4",
             "columns": [
-                "deadPeerDetection",
-                "siteName",
-                "intDscr",
-                "sn",
+                "peerId",
                 "profileName",
+                "remoteGwAddressV6",
+                "type",
                 "natTraversal",
-                "dhGroup",
-                "role",
+                "id",
                 "version",
+                "intName",
+                "keyLifeBytes",
                 "neighbors",
+                "remoteGwAddress",
+                "deadPeerDetection",
+                "keyLifeSeconds",
+                "localGwAddressV6",
                 "hostname",
+                "sn",
+                "dhGroup",
                 "encryption",
-                "intName",
-                "localGwAddress",
                 "status",
-                "type",
-                "authentication",
-                "keyLifeBytes",
+                "siteName",
+                "intDscr",
                 "mode",
                 "localId",
                 "authType",
-                "peerId",
-                "keyLifeSeconds",
-                "id",
-                "remoteGwAddress"
+                "authentication",
+                "localGwAddress",
+                "role"
             ],
             "description": "Internet Protocol Security (IPsec) gateways inventory",
             "method": "post",
             "nested_columns": [
                 "neighbors"
             ],
             "summary": "IPsec gateways",
@@ -15114,15 +15141,17 @@
                 "type",
                 "mode",
                 "role",
                 "status",
                 "intName",
                 "intDscr",
                 "localGwAddress",
+                "localGwAddressV6",
                 "remoteGwAddress",
+                "remoteGwAddressV6",
                 "neighbors",
                 "localId",
                 "peerId",
                 "encryption",
                 "authentication",
                 "dhGroup",
                 "keyLifeSeconds",
@@ -15140,56 +15169,62 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/ipsec/tunnels",
             "api_scope_id": "257769535da11554fef989811dcc6fdab52d2780",
             "columns": [
-                "encapsulation",
+                "remoteGwAddressV6",
+                "profileName",
+                "id",
+                "selectorRemoteAddress",
+                "selectorRemoteAddressV6",
+                "selectorRemotePort",
+                "protocol",
                 "ikeGateway",
-                "siteName",
+                "intName",
+                "keepAlive",
+                "keyLifeBytes",
+                "neighbors",
                 "routeBased",
-                "intDscr",
+                "remoteGwAddress",
+                "selectorProtocol",
+                "encapsulation",
+                "selectorLocalAddressV6",
+                "keyLifeSeconds",
+                "localGwAddressV6",
                 "selectorLocalAddress",
-                "selectorRemotePort",
+                "hostname",
+                "tunnelIntDscr",
+                "tunnelIntName",
                 "sn",
-                "selectorLocalPort",
-                "selectorRemoteAddress",
-                "profileName",
-                "keepAlive",
                 "dhGroup",
-                "tunnelIntName",
-                "neighbors",
-                "hostname",
+                "autoUp",
                 "encryption",
-                "intName",
-                "tunnelIntDscr",
-                "localGwAddress",
-                "selectorProtocol",
                 "status",
-                "protocol",
-                "autoUp",
+                "siteName",
+                "intDscr",
+                "selectorLocalPort",
                 "authentication",
-                "keyLifeBytes",
-                "keyLifeSeconds",
-                "id",
-                "remoteGwAddress"
+                "localGwAddress"
             ],
             "description": "Internet Protocol Security (IPsec) tunnels inventory",
             "method": "post",
             "nested_columns": [
                 "neighbors"
             ],
             "summary": "IPsec tunnels",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "profileName",
                 "localGwAddress",
+                "localGwAddressV6",
                 "remoteGwAddress",
+                "remoteGwAddressV6",
                 "neighbors",
                 "ikeGateway",
                 "intName",
                 "intDscr",
                 "routeBased",
                 "tunnelIntName",
                 "tunnelIntDscr",
@@ -15200,15 +15235,17 @@
                 "dhGroup",
                 "keyLifeSeconds",
                 "keyLifeBytes",
                 "keepAlive",
                 "autoUp",
                 "encapsulation",
                 "selectorLocalAddress",
+                "selectorLocalAddressV6",
                 "selectorRemoteAddress",
+                "selectorRemoteAddressV6",
                 "selectorLocalPort",
                 "selectorRemotePort",
                 "selectorProtocol"
             ],
             "web_endpoint": "/technology/security/ipsec/tunnels"
         },
         "put": null
@@ -15218,77 +15255,77 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/nat44",
             "api_scope_id": "4f46b9e59286735d7f4924e8e777c9aa8c55d45c",
             "columns": [
-                "interfaceOutZone",
-                "siteName",
-                "ruleNameNumeric",
+                "natUdpSrc",
+                "vxlanSrcGrp",
+                "ipTtl",
+                "id",
+                "l4Dst",
                 "tcpFlags",
+                "actionOriginal",
+                "udpSrc",
+                "description",
+                "ipProtocol",
+                "referencedTests",
+                "natTcpDst",
+                "l4Src",
+                "active",
                 "natTcpSrc",
-                "ipSrcRegion",
-                "natIpDst",
-                "interfaceIn",
-                "sn",
-                "others",
+                "ipDscp",
+                "l7Application",
+                "natL4Src",
                 "natUdpDst",
-                "udpDst",
-                "ipTtl",
-                "ipSrc",
-                "interfaceOut",
                 "ipPacketLength",
+                "icmpType",
+                "ipPrecedence",
+                "mplsLabelIn",
+                "hostname",
+                "ipTos",
+                "ipSrc",
                 "srcPorts",
+                "natIpPortDst",
+                "policyName",
+                "interfaceOut",
+                "ipSrcRegion",
                 "ipv6Src",
-                "vxlanVni",
+                "tcpDst",
+                "icmpCode",
                 "ruleName",
-                "natIpPortDst",
-                "actionOriginal",
-                "ipDst",
                 "natIpSrc",
-                "mplsLabelIn",
-                "ipFragmentOffset",
+                "natIpDst",
+                "interfaceOutZone",
                 "tcpSrc",
-                "natL4Src",
-                "icmpCode",
-                "referencedTests",
-                "natTcpDst",
-                "icmpIcmpv6",
+                "optionsTracked",
+                "ipDstRegion",
+                "interfaceIn",
+                "vxlanVni",
+                "others",
+                "vxlanDstGrp",
+                "sn",
+                "udpDst",
+                "interfaceIntraZone",
+                "natInterfaceSrc",
+                "siteName",
+                "ipv6Dst",
                 "dstPorts",
-                "hostname",
-                "ipProtocol",
-                "interfaceInterZone",
-                "uid",
-                "l7Application",
                 "natL4Dst",
-                "ipv6Dst",
-                "ipPrecedence",
-                "tcpDst",
-                "interfaceIntraZone",
-                "interfaceInZone",
-                "ipDstRegion",
-                "vxlanSrcGrp",
-                "ipDscp",
-                "l4Src",
-                "icmpType",
-                "description",
-                "ipTos",
+                "uid",
+                "icmpIcmpv6",
+                "ipFragmentOffset",
+                "ruleNameNumeric",
+                "interfaceVrf",
                 "action",
+                "interfaceInZone",
                 "ruleNumber",
-                "policyName",
-                "interfaceVrf",
-                "l4Dst",
-                "natInterfaceSrc",
-                "vxlanDstGrp",
-                "optionsTracked",
-                "active",
-                "udpSrc",
-                "natUdpSrc",
-                "id"
+                "interfaceInterZone",
+                "ipDst"
             ],
             "description": "Network Address Translation (IPv4 to IPv4)",
             "method": "post",
             "nested_columns": [
                 "interfaceIn",
                 "interfaceOut",
                 "interfaceInZone",
@@ -15389,23 +15426,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/object-groups",
             "api_scope_id": "88eb193dff9b57233051128d0bb232b199f8183c",
             "columns": [
-                "description",
-                "value",
+                "isLiteralValue",
                 "siteName",
-                "hostname",
-                "sn",
+                "id",
                 "name",
+                "sn",
                 "category",
-                "id",
-                "isLiteralValue"
+                "value",
+                "hostname",
+                "description"
             ],
             "description": "Security object groups and address books inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Security Object Groups",
             "ui_columns": [
                 "id",
@@ -15427,69 +15464,69 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/pbr",
             "api_scope_id": "07257c90ff5755111ebd4cc5599ade3c49faff28",
             "columns": [
-                "interfaceOutZone",
-                "siteName",
-                "ruleNameNumeric",
-                "tcpFlags",
-                "ipSrcRegion",
-                "interfaceIn",
-                "sn",
-                "others",
-                "udpDst",
+                "vxlanSrcGrp",
                 "ipTtl",
-                "ipSrc",
-                "interfaceOut",
-                "ipPacketLength",
-                "srcPorts",
-                "ipv6Src",
-                "vxlanVni",
-                "ruleName",
+                "id",
+                "l4Dst",
+                "tcpFlags",
                 "actionOriginal",
-                "ipDst",
-                "mplsLabelIn",
-                "ipFragmentOffset",
-                "tcpSrc",
-                "pbrActions",
-                "icmpCode",
-                "referencedTests",
-                "icmpIcmpv6",
-                "dstPorts",
-                "hostname",
+                "udpSrc",
+                "description",
                 "ipProtocol",
-                "interfaceInterZone",
-                "uid",
+                "referencedTests",
+                "l4Src",
+                "active",
+                "ipDscp",
                 "l7Application",
-                "ipv6Dst",
+                "ipPacketLength",
+                "icmpType",
                 "ipPrecedence",
+                "mplsLabelIn",
+                "pbrActions",
+                "hostname",
+                "ipTos",
+                "ipSrc",
+                "srcPorts",
+                "policyName",
+                "interfaceOut",
+                "ipSrcRegion",
+                "ipv6Src",
                 "tcpDst",
-                "interfaceIntraZone",
-                "interfaceInZone",
+                "icmpCode",
+                "ruleName",
+                "interfaceOutZone",
+                "tcpSrc",
+                "optionsTracked",
                 "ipDstRegion",
-                "vxlanSrcGrp",
-                "ipDscp",
-                "l4Src",
-                "icmpType",
-                "description",
-                "ipTos",
+                "interfaceIn",
+                "vxlanVni",
+                "others",
+                "vxlanDstGrp",
+                "sn",
                 "evalAclTests",
+                "udpDst",
+                "interfaceIntraZone",
+                "siteName",
+                "ipv6Dst",
+                "dstPorts",
+                "uid",
+                "icmpIcmpv6",
+                "ipFragmentOffset",
+                "ruleNameNumeric",
+                "interfaceVrf",
                 "action",
+                "interfaceInZone",
                 "ruleNumber",
-                "policyName",
-                "interfaceVrf",
-                "l4Dst",
-                "vxlanDstGrp",
-                "optionsTracked",
-                "active",
-                "udpSrc",
-                "id"
+                "interfaceInterZone",
+                "ipDst"
             ],
             "description": "Policy Based Routing (syntax search)",
             "method": "post",
             "nested_columns": [
                 "interfaceIn",
                 "interfaceOut",
                 "interfaceInZone",
@@ -15572,23 +15609,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/secure-ports/devices",
             "api_scope_id": "dc62404f4a804f2ead5a76056f0ad47fe1ee0246",
             "columns": [
-                "siteName",
-                "hostname",
-                "usersCount",
-                "sn",
-                "intTotalNetCount",
                 "intSecNetCount",
-                "intSecEdgeCount",
+                "intTotalNetCount",
+                "siteName",
                 "intTotalEdgeCount",
                 "id",
+                "intSecEdgeCount",
+                "sn",
+                "usersCount",
+                "hostname",
                 "methods"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "802.1x Secure ports - Devices",
             "ui_columns": [
@@ -15610,33 +15647,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/secure-ports/interfaces",
             "api_scope_id": "b281ade7334dbc7a22bfa0834f2fabcfa86c0573",
             "columns": [
-                "siteName",
-                "usersCount",
-                "intDscr",
-                "sn",
-                "vendor",
-                "model",
-                "voiceVlan",
+                "id",
                 "dynamicMacCount",
                 "method",
-                "hostname",
+                "vendor",
                 "intName",
-                "platform",
                 "monitorMode",
+                "platform",
                 "edge",
                 "switchportMode",
+                "hostname",
                 "state",
+                "sn",
                 "accVlan",
-                "devType",
-                "id"
+                "usersCount",
+                "model",
+                "siteName",
+                "intDscr",
+                "voiceVlan",
+                "devType"
             ],
             "description": "Network access control interfaces inventory",
             "method": "post",
             "nested_columns": [
                 "devType"
             ],
             "summary": "802.1x Secure ports - Interfaces",
@@ -15668,24 +15705,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/secure-ports/users",
             "api_scope_id": "35b2c2aef79451e7c6beb180645638348ffd30db",
             "columns": [
-                "userMac",
                 "siteName",
-                "hostname",
-                "intName",
                 "userState",
+                "id",
+                "state",
                 "sn",
                 "username",
                 "userMethod",
-                "state",
-                "id"
+                "hostname",
+                "intName",
+                "userMac"
             ],
             "description": "Network access control users inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "802.1x Secure ports - Users",
             "ui_columns": [
                 "hostname",
@@ -15707,20 +15744,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/zone-firewall/interfaces",
             "api_scope_id": "cf6f4dd1573e802aafae22e38df61998c70576d3",
             "columns": [
                 "siteName",
+                "id",
+                "isDefault",
+                "sn",
                 "hostname",
                 "intName",
-                "zone",
-                "sn",
-                "isDefault",
-                "id"
+                "zone"
             ],
             "description": "Security gateway interfaces participating in zone firewall policies",
             "method": "post",
             "nested_columns": [
                 "zone"
             ],
             "summary": "Zone Firewall - Interfaces",
@@ -15739,67 +15776,67 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/zone-firewall/policies",
             "api_scope_id": "6dc8f403807c3343f64b8b20f7b1f1b5de6d79cf",
             "columns": [
-                "interfaceOutZone",
-                "siteName",
-                "ruleNameNumeric",
-                "tcpFlags",
-                "ipSrcRegion",
-                "interfaceIn",
-                "sn",
-                "others",
-                "udpDst",
+                "vxlanSrcGrp",
                 "ipTtl",
-                "ipSrc",
-                "interfaceOut",
+                "id",
+                "l4Dst",
+                "tcpFlags",
+                "actionOriginal",
+                "udpSrc",
+                "description",
+                "ipProtocol",
+                "referencedTests",
+                "l4Src",
+                "active",
+                "ipDscp",
+                "l7Application",
                 "ipPacketLength",
+                "icmpType",
+                "ipPrecedence",
+                "mplsLabelIn",
+                "hostname",
+                "ipTos",
+                "ipSrc",
                 "srcPorts",
+                "policyName",
+                "interfaceOut",
+                "ipSrcRegion",
                 "ipv6Src",
-                "vxlanVni",
+                "tcpDst",
+                "icmpCode",
                 "ruleName",
-                "actionOriginal",
-                "ipDst",
-                "mplsLabelIn",
-                "ipFragmentOffset",
+                "interfaceOutZone",
                 "tcpSrc",
-                "icmpCode",
-                "referencedTests",
-                "icmpIcmpv6",
+                "optionsTracked",
+                "ipDstRegion",
+                "interfaceIn",
+                "vxlanVni",
+                "others",
+                "vxlanDstGrp",
+                "sn",
+                "udpDst",
+                "interfaceIntraZone",
+                "siteName",
+                "ipv6Dst",
                 "dstPorts",
-                "hostname",
-                "ipProtocol",
-                "interfaceInterZone",
                 "uid",
-                "l7Application",
-                "ipv6Dst",
-                "ipPrecedence",
-                "tcpDst",
-                "interfaceIntraZone",
-                "interfaceInZone",
-                "ipDstRegion",
-                "vxlanSrcGrp",
-                "ipDscp",
-                "l4Src",
-                "icmpType",
-                "description",
-                "ipTos",
+                "icmpIcmpv6",
+                "ipFragmentOffset",
+                "ruleNameNumeric",
+                "interfaceVrf",
                 "action",
+                "interfaceInZone",
                 "ruleNumber",
-                "policyName",
-                "interfaceVrf",
-                "l4Dst",
-                "vxlanDstGrp",
-                "optionsTracked",
-                "active",
-                "udpSrc",
-                "id"
+                "interfaceInterZone",
+                "ipDst"
             ],
             "description": "Security gateways zone policies details",
             "method": "post",
             "nested_columns": [
                 "interfaceIn",
                 "interfaceOut",
                 "interfaceInZone",
@@ -15896,26 +15933,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/serial-ports",
             "api_scope_id": "66ff0ffa77cd1a7268b05a4489bf132567fde0f0",
             "columns": [
-                "mode",
-                "parameters",
                 "siteName",
-                "hostname",
-                "pinout",
                 "flowControl",
                 "label",
+                "loggingLevel",
+                "id",
+                "connector",
+                "mode",
+                "pinout",
+                "parameters",
                 "sn",
                 "name",
-                "connector",
-                "loggingLevel",
-                "id"
+                "hostname"
             ],
             "description": "Serial Ports",
             "method": "post",
             "nested_columns": [],
             "summary": "Serial Ports",
             "ui_columns": [
                 "hostname",
@@ -15955,22 +15992,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/settings/jumphosts",
             "api_scope_id": "8733038e31573cb3aafe69bc020272f19f73dd35",
             "columns": [
-                "address",
-                "label",
-                "exclude",
-                "loginType",
                 "subnets",
                 "running",
+                "id",
                 "enabled",
-                "id"
+                "address",
+                "loginType",
+                "label",
+                "exclude"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "exclude",
                 "subnets"
             ],
@@ -15994,20 +16031,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/settings/ports",
             "api_scope_id": "1c73966d5d59dc31aef79269ff662ad80b5d6bb4",
             "columns": [
-                "port",
-                "label",
-                "excludeSubnets",
                 "subnets",
+                "port",
+                "id",
                 "protocol",
-                "id"
+                "label",
+                "excludeSubnets"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "excludeSubnets",
                 "subnets"
             ],
@@ -16029,19 +16066,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/snapshot-attributes",
             "api_scope_id": "4e31d8fdc457a0b4448e2e699dbde343807c2c2c",
             "columns": [
-                "hostname",
-                "sn",
-                "name",
                 "id",
-                "value"
+                "name",
+                "sn",
+                "value",
+                "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/snapshot-attributes",
             "ui_columns": [
                 "sn",
@@ -16058,54 +16095,54 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/snapshot-devices",
             "api_scope_id": "1361822c3b08544fddb94e9197cd19fd407b3215",
             "columns": [
-                "type",
-                "parentId",
-                "siteName",
-                "hostname",
-                "platform",
-                "sn",
-                "vendor",
-                "ipString",
                 "vTask",
-                "isSelected",
-                "version",
-                "model",
                 "settingsStates",
                 "family",
+                "model",
+                "siteName",
+                "type",
+                "platform",
+                "ipString",
                 "id",
+                "version",
+                "source",
+                "sn",
                 "isApiTask",
-                "source"
+                "isSelected",
+                "hostname",
+                "vendor",
+                "parentId"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "settingsStates"
             ],
             "summary": "POST /tables/snapshot-devices",
             "ui_columns": [
                 "id",
-                "family",
                 "hostname",
+                "siteName",
+                "vendor",
+                "family",
+                "version",
+                "platform",
+                "model",
                 "ipString",
                 "isApiTask",
                 "isSelected",
-                "model",
                 "parentId",
-                "platform",
-                "siteName",
                 "sn",
                 "source",
                 "type",
-                "vendor",
-                "version",
                 "settingsStates"
             ],
             "web_endpoint": null
         },
         "put": null
     },
     "tables/spanning-tree/bridges": {
@@ -16113,23 +16150,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/bridges",
             "api_scope_id": "a8b7ab7c4e689937629699543914a015b639b2eb",
             "columns": [
-                "mode",
                 "siteName",
-                "hostname",
+                "id",
+                "mode",
+                "sn",
                 "stpDomain",
-                "changeRate",
                 "virtPorts",
-                "sn",
-                "id",
-                "vlans"
+                "hostname",
+                "vlans",
+                "changeRate"
             ],
             "description": "Overview of all Spanning-Tree Protocol (STP) bridges, protocol types, VLANs",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Bridges",
             "ui_columns": [
                 "hostname",
@@ -16149,32 +16186,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/guards",
             "api_scope_id": "970f429fdc181a25cdd93996e41824609141c470",
             "columns": [
+                "model",
+                "bpduGuard",
                 "siteName",
-                "hostname",
-                "intName",
-                "stpDomain",
                 "platform",
+                "id",
                 "voiceVlan",
-                "bpduGuard",
                 "bpduFilter",
                 "dynamicMacCount",
+                "devType",
+                "vendor",
                 "sn",
+                "stpDomain",
                 "switchportMode",
-                "vendor",
-                "portfast",
-                "model",
                 "accVlan",
-                "devType",
+                "portfast",
+                "hostname",
                 "rootGuard",
-                "id"
+                "intName"
             ],
             "description": "Overview of all Spanning-Tree Protocol (STP) guards applied to interfaces",
             "method": "post",
             "nested_columns": [
                 "devType"
             ],
             "summary": "STP Guards",
@@ -16205,21 +16242,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/multiple-stp",
             "api_scope_id": "448aa070411d0084e2f21cdd3d29373b5db62a43",
             "columns": [
-                "dstSn",
+                "dstHostname",
                 "siteName",
+                "id",
+                "srcSn",
                 "srcHostname",
                 "stpCount",
-                "dstHostname",
-                "srcSn",
-                "id"
+                "dstSn"
             ],
             "description": "Detected multiple Spanning-Tree Protocol (STP) instances between two devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Multiple STPs",
             "ui_columns": [
                 "srcHostname",
@@ -16235,24 +16272,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/neighbor-ports-vlan-mismatch",
             "api_scope_id": "6992b7848d045065d0295a7d5c824ad35f1defa6",
             "columns": [
-                "dstSn",
-                "srcVlanCount",
+                "dstHostname",
                 "siteName",
-                "srcHostname",
-                "srcIntName",
+                "id",
                 "dstVlanCount",
-                "dstHostname",
-                "dstIntName",
                 "srcSn",
-                "id"
+                "srcHostname",
+                "dstIntName",
+                "srcVlanCount",
+                "dstSn",
+                "srcIntName"
             ],
             "description": "Neighbor trunk ports where there is a different number of VLANs on each side of the link",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Ports VLAN Mismatch",
             "ui_columns": [
                 "srcHostname",
@@ -16271,22 +16308,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/ports-multiple-neighbors",
             "api_scope_id": "fe5ed75e32932dc9b06c10be9c32644348877883",
             "columns": [
-                "dstSn",
+                "dstHostname",
                 "siteName",
+                "id",
+                "srcSn",
                 "srcHostname",
-                "srcIntName",
-                "dstHostname",
                 "dstIntName",
-                "srcSn",
-                "id"
+                "dstSn",
+                "srcIntName"
             ],
             "description": "Neighbor switchports where multiple Spanning-Tree Protocol (STP) peerings are detected",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Ports Multiple Neighbors",
             "ui_columns": [
                 "srcHostname",
@@ -16304,24 +16341,24 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/stp-cdp-ports-mismatch",
             "api_scope_id": "786c4b98cf35a27a04fc873cda9c6a60f48fdb9c",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "stpHostname",
-                "sn",
-                "stpSn",
+                "id",
                 "cdpHostname",
                 "cdpIntName",
+                "stpSn",
+                "sn",
+                "stpHostname",
                 "cdpSn",
                 "stpIntName",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "Port connections with mismatched hostname or interface name in STP and CDP protocols reading",
             "method": "post",
             "nested_columns": [],
             "summary": "STP/CDP Mismatch",
             "ui_columns": [
                 "hostname",
@@ -16340,20 +16377,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/instance-members",
             "api_scope_id": "88d315d3e4e98a23bdd1df2d5cd7e9593f4a60a4",
             "columns": [
-                "rootHostname",
+                "id",
                 "vlanId",
-                "rootId",
                 "vlanName",
-                "members",
-                "id"
+                "rootHostname",
+                "rootId",
+                "members"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "members"
             ],
             "summary": "POST /tables/spanning-tree/instance-members",
@@ -16374,27 +16411,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/instances",
             "api_scope_id": "51d1ebee0d39a16ff63fce2edac961c7b3154d83",
             "columns": [
+                "rootPriority",
                 "siteName",
-                "hostname",
-                "stpDomain",
-                "changeRate",
-                "edgesSum",
                 "virtPorts",
-                "vlanId",
+                "id",
+                "edgesSum",
+                "devs",
                 "sn",
-                "rootId",
+                "vlanId",
+                "stpDomain",
                 "vlanName",
-                "rootPriority",
-                "devs",
-                "id"
+                "rootId",
+                "hostname",
+                "changeRate"
             ],
             "description": "Spanning-Tree Protocol (STP) instances, root bridges and associated VLANs",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Instances",
             "ui_columns": [
                 "hostname",
@@ -16417,34 +16454,34 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/neighbors",
             "api_scope_id": "56f6391a3fc294d45b8e6b3677fd877fd1314c32",
             "columns": [
-                "siteName",
-                "sn",
-                "portRole",
-                "portStatus",
-                "vlanId",
-                "portRoleDst",
-                "portId",
-                "portIdDst",
                 "snDst",
-                "vlanName",
-                "portStatusDst",
+                "portIdDst",
+                "id",
                 "portPathCost",
-                "rootId",
-                "hostnameDst",
-                "hostname",
+                "vlanName",
                 "intName",
-                "intNameDst",
+                "hostnameDst",
                 "stpDomain",
+                "portId",
+                "hostname",
+                "portRole",
+                "portStatusDst",
+                "sn",
+                "vlanId",
+                "siteName",
                 "portPathCostDst",
-                "id"
+                "intNameDst",
+                "portRoleDst",
+                "rootId",
+                "portStatus"
             ],
             "description": "Spanning-Tree Protocol (STP) peering relationships of connected bridges",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Peerings",
             "ui_columns": [
                 "hostname",
@@ -16474,27 +16511,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/ports",
             "api_scope_id": "17cfb1b38ca20ac3e42b918aceb934443f60129e",
             "columns": [
-                "portStatus",
+                "portRole",
                 "siteName",
+                "id",
+                "portPathCost",
+                "sn",
                 "hostname",
-                "intName",
                 "stpDomain",
                 "vlanId",
-                "portId",
-                "sn",
-                "rootId",
                 "vlanName",
-                "portRole",
-                "portPathCost",
-                "id"
+                "portStatus",
+                "rootId",
+                "portId",
+                "intName"
             ],
             "description": "Spanning-Tree Protocol (STP) virtual ports inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Virtual Ports",
             "ui_columns": [
                 "hostname",
@@ -16518,20 +16555,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/radius",
             "api_scope_id": "a6087fe22f2ee5581335df689ea5d0b6d2868945",
             "columns": [
-                "srcDev",
-                "stpDomain",
-                "dstDev",
                 "stpMode",
                 "distance",
-                "id"
+                "id",
+                "stpDomain",
+                "srcDev",
+                "dstDev"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/spanning-tree/radius",
             "ui_columns": [
                 "id",
@@ -16550,21 +16587,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/topology",
             "api_scope_id": "7fabda7b35a8320c9edac7a31e9745c87bd81cc7",
             "columns": [
-                "root",
-                "stpDomain",
                 "siteName",
+                "id",
                 "vlanId",
-                "changeRate",
+                "stpDomain",
                 "vlanName",
-                "id"
+                "root",
+                "changeRate"
             ],
             "description": "Spanning-Tree Protocol (STP) instances with topology change compared to the last snapshot",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Stability",
             "ui_columns": [
                 "root",
@@ -16583,28 +16620,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/vlans",
             "api_scope_id": "d155d2c73814c14440c2d44b2d17ff429641d456",
             "columns": [
-                "bridgeId",
+                "rootPriority",
+                "bridgePriority",
                 "siteName",
-                "hostname",
-                "stpDomain",
-                "changeRate",
                 "virtPorts",
-                "vlanId",
+                "id",
                 "sn",
-                "rootId",
-                "bridgePriority",
                 "rootCost",
-                "rootPriority",
+                "stpDomain",
+                "vlanId",
                 "vlanName",
-                "id"
+                "bridgeId",
+                "rootId",
+                "hostname",
+                "changeRate"
             ],
             "description": "Spanning-Tree Protocol (STP) VLANs inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "STP VLANs",
             "ui_columns": [
                 "hostname",
@@ -16665,24 +16702,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/users",
             "api_scope_id": "55ebdafabb0a68c1e2caaae7ac68c58108c770ad",
             "columns": [
-                "domainSuffixes",
-                "ldapId",
-                "ssoProvider",
-                "username",
-                "email",
                 "timezone",
-                "roleIds",
                 "isLocal",
                 "id",
-                "roleNames"
+                "roleIds",
+                "domainSuffixes",
+                "email",
+                "roleNames",
+                "ldapId",
+                "username",
+                "ssoProvider"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "roleIds",
                 "roleNames"
             ],
@@ -16707,23 +16744,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vlan/device",
             "api_scope_id": "56568e03bc4cf792bd2296602128c8932d99d18b",
             "columns": [
+                "stdStatus",
                 "siteName",
-                "hostname",
-                "stpDomain",
-                "vlanId",
+                "id",
                 "sn",
+                "vlanId",
+                "stpDomain",
                 "vlanName",
-                "stdStatus",
-                "status",
-                "id"
+                "hostname",
+                "status"
             ],
             "description": "Virtual LAN (VLAN) inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs - Device Detail",
             "ui_columns": [
                 "hostname",
@@ -16744,19 +16781,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vlan/device-summary",
             "api_scope_id": "fc39974e11fc30a9488f6f2802d9292818974ef1",
             "columns": [
                 "siteName",
-                "hostname",
-                "totalVlanCount",
-                "sn",
+                "id",
                 "activeVlanCount",
-                "id"
+                "sn",
+                "hostname",
+                "totalVlanCount"
             ],
             "description": "Virtual LAN (VLAN) per managed network device",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs - Device Summary",
             "ui_columns": [
                 "hostname",
@@ -16773,19 +16810,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vlan/l3-gateways",
             "api_scope_id": "3985721e62fbfaac22bd269c4d08cab207df95e5",
             "columns": [
-                "vlanId",
-                "stpDomain",
-                "rootId",
                 "id",
-                "networks"
+                "networks",
+                "stpDomain",
+                "vlanId",
+                "rootId"
             ],
             "description": "Layer 3 Gateways to VLAN mappings",
             "method": "post",
             "nested_columns": [
                 "networks"
             ],
             "summary": "L3 Gateways",
@@ -16804,19 +16841,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vlan/network-summary",
             "api_scope_id": "ff4f2af574d3e9dae254a81d3987ba363b4c7063",
             "columns": [
-                "vlanId",
-                "devCount",
                 "dscr",
+                "id",
+                "vlanId",
                 "vlanName",
-                "id"
+                "devCount"
             ],
             "description": "Virtual LANs (VLAN) configured in network grouped by VLAN ID",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs - Network Summary",
             "ui_columns": [
                 "vlanId",
@@ -16834,19 +16871,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vlan/site-summary",
             "api_scope_id": "f9221b6c36b8576b46df1c8ec0847b68a68957e8",
             "columns": [
                 "siteName",
-                "devCount",
-                "vlanId",
                 "dscr",
+                "id",
+                "vlanId",
                 "vlanName",
-                "id"
+                "devCount"
             ],
             "description": "Virtual LANs (VLAN) configured in network grouped by VLAN ID with site information",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs - Summary per Site",
             "ui_columns": [
                 "siteName",
@@ -16865,20 +16902,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vrf/detail",
             "api_scope_id": "6b84960151fe991f1dd4f5a2b5888c4920a55965",
             "columns": [
                 "siteName",
-                "hostname",
                 "rd",
+                "id",
+                "intCount",
                 "sn",
                 "vrf",
-                "intCount",
-                "id"
+                "hostname"
             ],
             "description": "Virtual Routing and Forwadring instances per devices",
             "method": "post",
             "nested_columns": [],
             "summary": "VRF Devices",
             "ui_columns": [
                 "hostname",
@@ -16897,21 +16934,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vrf/interfaces",
             "api_scope_id": "aa24fef60e95afd2f2216784150dfdaea9cc1557",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
                 "rd",
+                "id",
                 "sn",
+                "networks",
                 "vrf",
-                "id",
-                "networks"
+                "hostname",
+                "intName"
             ],
             "description": "Virtual Routing and Forwadring instances per interfaces",
             "method": "post",
             "nested_columns": [
                 "networks"
             ],
             "summary": "VRF Interfaces",
@@ -16932,17 +16969,17 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vrf/summary",
             "api_scope_id": "97a2e35438a2a2cb3afb045f7faa765664573679",
             "columns": [
-                "vrf",
                 "id",
-                "devices"
+                "devices",
+                "vrf"
             ],
             "description": "Virtual Routing and Forwadring instances per devices summary",
             "method": "post",
             "nested_columns": [],
             "summary": "VRF Summary",
             "ui_columns": [
                 "vrf",
@@ -16957,28 +16994,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vxlan/interfaces",
             "api_scope_id": "5e2b2153f70005662761f89aa478843744f8e5ea",
             "columns": [
-                "sourcePrimaryIp",
-                "sourcePrimaryIpv6",
                 "siteName",
-                "hostname",
-                "intName",
-                "sourceSecondaryIpv6",
+                "hostLearningMode",
+                "sourcePrimaryIp",
                 "localRouterMac",
+                "id",
+                "sourceSecondaryIp",
+                "controlPlane",
                 "sn",
-                "sourceInt",
                 "encap",
-                "hostLearningMode",
-                "controlPlane",
-                "id",
-                "sourceSecondaryIp"
+                "sourceInt",
+                "sourceSecondaryIpv6",
+                "sourcePrimaryIpv6",
+                "hostname",
+                "intName"
             ],
             "description": "Virtual Tunnel End Point (VTEP) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "VTEP Interfaces",
             "ui_columns": [
                 "hostname",
@@ -17003,37 +17040,37 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vxlan/peers",
             "api_scope_id": "0b8ebbf68d3dbb9b557863ff4dc507cee018bc8b",
             "columns": [
-                "localAddress",
-                "siteName",
-                "sn",
-                "neiDevType",
-                "learnType",
-                "uptime",
-                "target",
-                "neiAddress",
-                "vni",
                 "neiHostname",
+                "id",
+                "uptime",
+                "neiSiteName",
                 "eVni",
-                "subnet",
-                "hostname",
-                "intName",
                 "neiSn",
+                "neiDevType",
+                "intName",
+                "neiAddress",
                 "neiIntName",
-                "neiSiteName",
                 "flags",
-                "routerMac",
+                "localAddress",
+                "hostname",
+                "subnet",
                 "state",
+                "source",
+                "sn",
+                "siteName",
+                "vni",
                 "devType",
-                "id",
-                "source"
+                "learnType",
+                "routerMac",
+                "target"
             ],
             "description": "Virtual Tunnel End Point (VTEP) peers matrix",
             "method": "post",
             "nested_columns": [],
             "summary": "VTEP Peers",
             "ui_columns": [
                 "hostname",
@@ -17060,26 +17097,26 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vxlan/vni",
             "api_scope_id": "26eb5f7ef155608cc045df062cc5b641dd877789",
             "columns": [
                 "bd",
-                "mode",
                 "siteName",
-                "intName",
-                "hostname",
-                "vniState",
+                "type",
+                "id",
                 "vni",
+                "mode",
                 "sn",
-                "vrf",
-                "mcastGroup",
+                "vniState",
                 "cfg",
-                "type",
-                "id"
+                "vrf",
+                "hostname",
+                "intName",
+                "mcastGroup"
             ],
             "description": "VXLAN network identifier (VNI) inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "VXLAN Network Identifier",
             "ui_columns": [
                 "hostname",
@@ -17104,20 +17141,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vxlan/vtep",
             "api_scope_id": "f78de74c207482ad3de80cf8828bf7ff74732426",
             "columns": [
                 "siteName",
-                "hostname",
-                "vniCount",
-                "sn",
-                "peersCount",
                 "id",
-                "interfacesCount"
+                "sn",
+                "vniCount",
+                "interfacesCount",
+                "hostname",
+                "peersCount"
             ],
             "description": "VXLAN tunnel endpoint (VTEP) inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "VXLAN Tunnel Endpoints",
             "ui_columns": [
                 "hostname",
@@ -17135,31 +17172,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/wireless/access-points",
             "api_scope_id": "989c3820c6d3d3fe8ce084b18c9b7210fc925581",
             "columns": [
+                "switchPort",
+                "clientCount",
                 "siteName",
                 "avgRssi",
-                "controllerSn",
-                "controller",
-                "apMac",
-                "clientCount",
-                "switchHostname",
                 "avgSignalToNoiseRatio",
-                "switchPort",
-                "bssidCount",
-                "ssid",
                 "switchSn",
-                "apName",
-                "apSn",
                 "id",
+                "apSn",
+                "bssidCount",
+                "apMac",
+                "controller",
+                "ssid",
+                "controllerSn",
                 "apPort",
-                "impact"
+                "apName",
+                "impact",
+                "switchHostname"
             ],
             "description": "Wireless access points inventory",
             "method": "post",
             "nested_columns": [
                 "ssid"
             ],
             "summary": "Wireless Access Points",
@@ -17187,36 +17224,36 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/wireless/clients",
             "api_scope_id": "ab2b47f3fc0061878d4d91037bdb2456264b9e55",
             "columns": [
-                "siteName",
-                "inPktsRate",
                 "client",
-                "ssid",
-                "bytesRate",
-                "policyManagerState",
-                "pktsRate",
+                "id",
+                "inPktsRate",
                 "signalToNoiseRatio",
-                "inBytesRate",
                 "frequency",
+                "pktsRate",
                 "bssid",
-                "apName",
+                "outPktsRate",
+                "policyManagerState",
+                "ssid",
                 "controllerSn",
+                "apName",
+                "clientIp",
+                "inBytesRate",
+                "uniqId",
+                "state",
                 "apSn",
-                "controller",
-                "outPktsRate",
+                "siteName",
                 "rssi",
-                "outBytesRate",
-                "state",
-                "uniqId",
-                "clientIp",
-                "id"
+                "bytesRate",
+                "controller",
+                "outBytesRate"
             ],
             "description": "Wireless clients inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Wireless Clients",
             "ui_columns": [
                 "controller",
@@ -17247,21 +17284,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/wireless/controllers",
             "api_scope_id": "57202e6caa54c5ebb4dd83da714200ad33fa543f",
             "columns": [
-                "apCount",
-                "siteName",
                 "clientCount",
-                "ssid",
-                "controllerSn",
+                "siteName",
+                "apCount",
                 "id",
-                "controller"
+                "controller",
+                "ssid",
+                "controllerSn"
             ],
             "description": "Wireless controllers inventory",
             "method": "post",
             "nested_columns": [
                 "ssid"
             ],
             "summary": "Wireless Controllers",
@@ -17282,25 +17319,25 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/wireless/radio",
             "api_scope_id": "a86fcefe3373c1206c2f3a0f4dd4e7366e28dd8a",
             "columns": [
                 "radioFreq",
-                "radioMac",
-                "radioDscr",
-                "siteName",
-                "wlanBssid",
+                "wlanSsid",
                 "clientCount",
-                "radioStatus",
-                "apName",
+                "siteName",
                 "id",
                 "apSn",
+                "radioDscr",
+                "wlanBssid",
+                "apName",
                 "mac",
-                "wlanSsid"
+                "radioStatus",
+                "radioMac"
             ],
             "description": "Wireless Radios & BSSID inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Wireless Radios & BSSID",
             "ui_columns": [
                 "apName",
@@ -17324,19 +17361,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/wireless/ssid-summary",
             "api_scope_id": "46afef4e48bcb78a68157f77a26fc4b11909442f",
             "columns": [
-                "radioCount",
-                "apCount",
                 "clientCount",
-                "ssid",
+                "apCount",
                 "id",
+                "radioCount",
+                "ssid",
                 "wlcCount"
             ],
             "description": "Wireless service set identifier (SSID) summary",
             "method": "post",
             "nested_columns": [],
             "summary": "Wireless SSID Summary",
             "ui_columns": [
```

### Comparing `ipfabric-6.7.3/ipfabric/oas/v6.7.json` & `ipfabric-6.8.0b0/ipfabric/oas/v6.8.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9942587283339098%*

 * *Differences: {"'attributes/local/update-from-global'": "OrderedDict([('api_endpoint', "*

 * *                                          "'/attributes/local/update-from-global'), ('get', None), "*

 * *                                          "('put', None), ('patch', None), ('post', "*

 * *                                          "OrderedDict([('api_endpoint', "*

 * *                                          "'attributes/local/update-from-global'), ('method', "*

 * *                                          "'post'), ('web_endpoint', None), ('c […]*

```diff
@@ -153,14 +153,50 @@
             "method": "put",
             "nested_columns": null,
             "summary": "Update local attribute",
             "ui_columns": null,
             "web_endpoint": null
         }
     },
+    "attributes/local/update-from-global": {
+        "api_endpoint": "/attributes/local/update-from-global",
+        "delete": null,
+        "get": null,
+        "patch": null,
+        "post": {
+            "api_endpoint": "attributes/local/update-from-global",
+            "api_scope_id": "ae41ca85b9cf147b4cd57d95d8cdd1a39b5c2ce8",
+            "columns": null,
+            "description": "Update local attributes from global for specified snapshot",
+            "method": "post",
+            "nested_columns": null,
+            "summary": "Update local attributes from global",
+            "ui_columns": null,
+            "web_endpoint": null
+        },
+        "put": null
+    },
+    "attributes/local/update-from-global/check-sites-recalculation": {
+        "api_endpoint": "/attributes/local/update-from-global/check-sites-recalculation",
+        "delete": null,
+        "get": null,
+        "patch": null,
+        "post": {
+            "api_endpoint": "attributes/local/update-from-global/check-sites-recalculation",
+            "api_scope_id": "521984bba948c061d3f2f2ffc94ab82235f3c4e4",
+            "columns": null,
+            "description": "Check if attributes update will trigger sites recalculation for specified snapshot",
+            "method": "post",
+            "nested_columns": null,
+            "summary": "Check if attributes update will trigger sites recalculation",
+            "ui_columns": null,
+            "web_endpoint": null
+        },
+        "put": null
+    },
     "auth/available-idps": {
         "api_endpoint": "/auth/available-idps",
         "delete": null,
         "get": {
             "api_endpoint": "auth/available-idps",
             "api_scope_id": "df53b2e939a8a2f4343f344fb8e7f5335e9afc6b",
             "columns": null,
@@ -3264,22 +3300,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/aci/dtep",
             "api_scope_id": "1e59228ef7e29180ad59f674a5069f708374daff",
             "columns": [
-                "siteName",
                 "type",
+                "siteName",
+                "sn",
                 "id",
                 "dtepIp",
-                "sn",
-                "encap",
                 "role",
-                "hostname"
+                "hostname",
+                "encap"
             ],
             "description": "IS-IS Dynamic Tunnel End Point inventory",
             "method": "post",
             "nested_columns": [
                 "type"
             ],
             "summary": "DTEP Inventory",
@@ -3300,31 +3336,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/aci/endpoints",
             "api_scope_id": "8377957b155db2db2fe4fdde54bba5a645e84612",
             "columns": [
-                "vrf",
                 "siteName",
-                "vrfVnid",
-                "encapId",
+                "sn",
                 "group",
                 "id",
-                "mac",
-                "hostname",
-                "sn",
+                "encapId",
+                "ip",
+                "bdVnid",
+                "intName",
                 "ipFlags",
-                "macFlags",
+                "hostname",
                 "vlanId",
                 "vlanVnid",
-                "ip",
-                "bdVnid",
-                "encapType",
-                "intName"
+                "vrf",
+                "vrfVnid",
+                "macFlags",
+                "mac",
+                "encapType"
             ],
             "description": "Application Centric Infrastructure (ACI) endpoints inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "ACI Endpoint",
             "ui_columns": [
                 "hostname",
@@ -3352,26 +3388,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/aci/vlan",
             "api_scope_id": "521712216816bf6ffe1260cf9a8040adb3e341dd",
             "columns": [
-                "bdVlanId",
-                "siteName",
+                "encapVlanType",
                 "encapVlanId",
-                "vlanType",
+                "siteName",
+                "sn",
                 "id",
-                "encapVlanType",
                 "endpointCount",
                 "fabricVxlanId",
-                "sn",
+                "hostname",
                 "vlanId",
+                "bdVlanId",
                 "hwId",
-                "hostname"
+                "vlanType"
             ],
             "description": "Application Centric Infrastructure (ACI) VLANs inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "ACI VLAN",
             "ui_columns": [
                 "hostname",
@@ -3395,23 +3431,23 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/aci/vrf",
             "api_scope_id": "8800985b8f133246c0f03b4b3a3031ca625e6945",
             "columns": [
                 "vrfVxlanId",
-                "vrf",
                 "siteName",
+                "sn",
                 "id",
-                "vrfType",
+                "status",
                 "endpointCount",
-                "sn",
-                "contextId",
                 "hostname",
-                "status"
+                "vrf",
+                "vrfType",
+                "contextId"
             ],
             "description": "Application Centric Infrastructure (ACI) virtual routing and forwarding instances inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "ACI VRF",
             "ui_columns": [
                 "hostname",
@@ -3432,27 +3468,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/arp",
             "api_scope_id": "22bb05c6b1f06bce692dd02f7113e0c944bae4ec",
             "columns": [
-                "siteName",
-                "id",
-                "proxy",
                 "vendor",
+                "siteName",
                 "sn",
-                "vlanId",
+                "id",
+                "ip",
                 "intName",
-                "mac",
-                "vrf",
+                "vlanId",
                 "hostname",
-                "ip"
+                "proxy",
+                "vrf",
+                "mac"
             ],
-            "description": "Address Resolution Protocol (ARP) collected fromt the network",
+            "description": "Cumulative ARP tables collected from all devices on all interfaces in all routing instances (VRFs).\n\nMultiple IP addresses can have the same MAC address - one MAC address can have multiple IP address mappings.\\\nIf the mapping was received via proxy ARP router then it will be noted here. Desired state is no proxy ARP in the network.",
             "method": "post",
             "nested_columns": [],
             "summary": "ARP Table",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -3473,20 +3509,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/duplicate-ip",
             "api_scope_id": "b57f0159953704683e4c6dbcb52fbf2c9ae4a657",
             "columns": [
                 "id",
-                "countIntUp",
+                "ip",
                 "count",
                 "hostname",
-                "ip"
+                "countIntUp"
             ],
-            "description": "Duplicate IP adresses detected in the network",
+            "description": "This table shows the list of duplicate IP adresses in the network which should be (according to best practices) unique. Virtual/Shared/similar on-purpose duplicate addresses are not included here.\n\nIP addresses should be unique throughout the network, except for highly specialized applications, such as geographical service distribution via anycast. Duplicate IPs usually signify a network fault, such as loss of keep alive link or misconfiguration, and can cause various degrees of issues from total loss of connectivity for a network segment to intermittent application reachability to complicating network infrastructure management.\n\nThis table should be empty except for anycast addresses.",
             "method": "post",
             "nested_columns": [],
             "summary": "Duplicate IP",
             "ui_columns": [
                 "ip",
                 "count",
                 "countIntUp",
@@ -3501,27 +3537,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/hosts",
             "api_scope_id": "dd3e429da6bbb78f01b1a694d04b12a623e97cb6",
             "columns": [
-                "gateways",
-                "siteName",
-                "vlan",
                 "type",
-                "accessPoints",
-                "id",
+                "siteName",
                 "vendor",
-                "mac",
-                "edges",
+                "id",
+                "accessPoints",
+                "uniqId",
                 "ip",
+                "edges",
+                "vlan",
                 "vrf",
-                "dnsName",
-                "uniqId"
+                "mac",
+                "gateways",
+                "dnsName"
             ],
             "description": "Detected IPv4 users, hosts, and endpoints from discovered gateways",
             "method": "post",
             "nested_columns": [
                 "accessPoints",
                 "edges",
                 "gateways",
@@ -3549,25 +3585,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/ipv6-hosts",
             "api_scope_id": "80ba0a1528bd80b1b6235610789c3e36b9663e20",
             "columns": [
-                "gateways",
-                "siteName",
-                "vlan",
                 "type",
+                "siteName",
+                "vendor",
                 "id",
                 "ipv6",
+                "uniqId",
                 "edges",
-                "mac",
+                "vlan",
                 "vrf",
-                "vendor",
-                "uniqId"
+                "mac",
+                "gateways"
             ],
             "description": "Detected IPv6 users, hosts, and endpoints from discovered gateways",
             "method": "post",
             "nested_columns": [
                 "edges",
                 "gateways",
                 "type"
@@ -3592,29 +3628,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/ipv6-managed-devs",
             "api_scope_id": "adfde3593455992b53ceba8013eece37ea60c172",
             "columns": [
-                "siteName",
-                "stateL2",
                 "type",
+                "siteName",
+                "sn",
                 "id",
+                "stateL2",
                 "net",
-                "sn",
+                "ip",
+                "intName",
                 "stateL1",
                 "vlanId",
-                "intName",
-                "mac",
-                "vrf",
                 "hostname",
-                "ip"
+                "vrf",
+                "mac"
             ],
-            "description": "IPv6 addressess configured on network interfaces",
+            "description": "Information about every IP address on every managed network infrastructure device.\n\nDNS checks on managed IP addresses are also performed to verify the DNS consistency.",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed IPv6 addresses",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "stateL1",
@@ -3636,25 +3672,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/ipv6-neighbors",
             "api_scope_id": "2c64d326d8d979b9084e63cb21021a8680693d4e",
             "columns": [
+                "vendor",
                 "siteName",
+                "sn",
                 "id",
                 "ipv6",
-                "proxy",
-                "vendor",
-                "sn",
+                "intName",
                 "vlanId",
-                "mac",
-                "vrf",
                 "hostname",
-                "intName"
+                "proxy",
+                "vrf",
+                "mac"
             ],
             "description": "Neighbors detected with IPv6 neighbor discovery",
             "method": "post",
             "nested_columns": [],
             "summary": "IPv6 Neighbor discovery",
             "ui_columns": [
                 "hostname",
@@ -3676,31 +3712,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/mac",
             "api_scope_id": "a97aa4c973ddef344684436badc40fa5fd6d5e2b",
             "columns": [
-                "siteName",
-                "vlan",
                 "type",
+                "siteName",
+                "sn",
+                "vendor",
                 "id",
                 "vni",
+                "fabricPath",
+                "vxlans",
                 "edge",
                 "source",
-                "sn",
+                "intName",
                 "user",
-                "vendor",
-                "vxlans",
-                "mac",
                 "hostname",
-                "intName",
-                "fabricPath"
+                "vlan",
+                "mac"
             ],
-            "description": "Cumulative MAC address table",
+            "description": "This table covers MAC tables collected from all devices. MAC address is shown along with edge network device and interface where it is connected.\\\nOne MAC address will be typically present many times in the table below. The reason is that the same MAC entry is present on different switches on different interfaces. However for the same MAC address:\n* There could be many entries where the \"Edge\" column is \"no\". Those are on transit switches in the network infrastructure.\n* For the \"user\" type of devices, there should be limited number (1-2) of entries where the \"Edge\" column is \"yes\". Those are the switches closest to the device itself.\n\n---\n\nTypes of devices can be as follows:\n* ap: is wireless access point\n* netDev: is networking device other than \"router\"\n* phone: is IP phone\n* router: is a native L3 routing device\n* virtual: is Virtual group or High availability\n* user: is user endpoint device\n* Unreachable",
             "method": "post",
             "nested_columns": [
                 "vxlans"
             ],
             "summary": "MAC Table",
             "ui_columns": [
                 "hostname",
@@ -3726,32 +3762,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/managed-devs",
             "api_scope_id": "d11dae27159ec2f8ad49b5ff3793346760547326",
             "columns": [
-                "siteName",
-                "stateL2",
+                "dnsReverseMatch",
                 "type",
-                "dnsHostnameMatch",
+                "siteName",
+                "sn",
                 "id",
+                "stateL2",
                 "net",
-                "mac",
-                "sn",
+                "ip",
+                "intName",
                 "stateL1",
                 "vlanId",
-                "dnsReverseMatch",
-                "intName",
-                "ip",
-                "vrf",
                 "hostname",
+                "dnsHostnameMatch",
+                "vrf",
+                "mac",
                 "dnsName"
             ],
-            "description": "Inventory of IP addresses configured on every managed network device",
+            "description": "Information about every IP address on every managed network infrastructure device.\n\nDNS checks on managed IP addresses are also performed to verify the DNS consistency.",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed IPv4 addresses",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "stateL1",
@@ -3776,17 +3812,17 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/path-lookup-first-hops",
             "api_scope_id": "b40b73f5f323984b20fae87347eceb5ee5d06359",
             "columns": [
-                "sn",
+                "interfaces",
                 "hostname",
-                "interfaces"
+                "sn"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "interfaces"
             ],
             "summary": "POST /tables/addressing/path-lookup-first-hops",
@@ -3832,16 +3868,16 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/addressing/path-lookup-sources-multicast",
             "api_scope_id": "e0c56ce09d5a8df4c115ef86691cf4dc05099bde",
             "columns": [
                 "ip",
                 "id",
-                "dnsName",
-                "type"
+                "type",
+                "dnsName"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/addressing/path-lookup-sources-multicast",
             "ui_columns": [
                 "id",
@@ -3884,21 +3920,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/applications",
             "api_scope_id": "a2539bd51c8d19aeb19678f0a7fbb9997379861f",
             "columns": [
-                "slug",
                 "tenant",
                 "id",
-                "priority",
+                "apiUrl",
                 "name",
-                "endpointGroupsCount",
-                "apiUrl"
+                "slug",
+                "priority",
+                "endpointGroupsCount"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) applications inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "APIC Applications",
             "ui_columns": [
                 "apiUrl",
@@ -3917,24 +3953,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/bridge-domains",
             "api_scope_id": "6c44dbdbc71937871ada66f59fcca23c4b83131a",
             "columns": [
-                "slug",
-                "tenant",
-                "vrfName",
-                "subnets",
                 "type",
+                "tenant",
                 "id",
-                "pcTag",
-                "name",
                 "apiUrl",
-                "scope"
+                "scope",
+                "subnets",
+                "name",
+                "slug",
+                "pcTag",
+                "vrfName"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) bridge-domains inventory",
             "method": "post",
             "nested_columns": [
                 "subnets"
             ],
             "summary": "APIC Bridge Domains",
@@ -3958,23 +3994,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/contexts",
             "api_scope_id": "26bf59496c1aed1763b8d2eec18a9ce6323f2d1a",
             "columns": [
-                "slug",
                 "tenant",
                 "id",
-                "pcTag",
+                "apiUrl",
+                "scope",
                 "name",
-                "isUnenforced",
+                "slug",
+                "pcTag",
                 "bridgeDomainsCount",
-                "apiUrl",
-                "scope"
+                "isUnenforced"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) contexts inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "APIC Contexts",
             "ui_columns": [
                 "apiUrl",
@@ -3995,26 +4031,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/contracts",
             "api_scope_id": "32009950f96b207cb23f48d6bb6aea004fffa677",
             "columns": [
+                "consumerMatch",
+                "tenant",
+                "id",
                 "apiUrl",
+                "providerMatch",
+                "contractScope",
                 "slug",
-                "tenant",
-                "contractName",
                 "hasReverseFilterPorts",
-                "id",
+                "serviceGraph",
                 "subjectFilters",
-                "contractScope",
                 "subjectName",
-                "providerMatch",
-                "consumerMatch",
-                "serviceGraph"
+                "contractName"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) contracts inventory'",
             "method": "post",
             "nested_columns": [
                 "subjectFilters"
             ],
             "summary": "APIC Contracts",
@@ -4041,22 +4077,22 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/controllers",
             "api_scope_id": "30ba8f81ceeb27989a0b15429c02b89bf50dea1b",
             "columns": [
                 "siteName",
-                "ipv6Addresses",
+                "sn",
                 "id",
+                "apiUrl",
                 "name",
-                "sn",
-                "ipAddresses",
                 "health",
                 "hostname",
-                "apiUrl"
+                "ipv6Addresses",
+                "ipAddresses"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) controllers inventory",
             "method": "post",
             "nested_columns": [
                 "ipAddresses",
                 "ipv6Addresses"
             ],
@@ -4079,25 +4115,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/endpoint-groups",
             "api_scope_id": "00e8efe24aeb7068affad09141dc91ffb0ddeb82",
             "columns": [
-                "slug",
-                "tenant",
-                "appName",
                 "isPreferredGroupMember",
-                "subnets",
+                "tenant",
                 "id",
+                "apiUrl",
+                "scope",
+                "subnets",
                 "contractsCount",
-                "pcTag",
+                "slug",
                 "name",
-                "apiUrl",
-                "scope"
+                "pcTag",
+                "appName"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) endpoint-groups inventory",
             "method": "post",
             "nested_columns": [
                 "subnets"
             ],
             "summary": "Endpoint Groups",
@@ -4122,22 +4158,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/endpoint-groups/contracts",
             "api_scope_id": "e3e7838393599ff81d47a268fe05f96589fef66f",
             "columns": [
-                "slug",
-                "tenant",
-                "appName",
                 "type",
+                "tenant",
                 "id",
+                "apiUrl",
                 "name",
+                "slug",
                 "endpointGroupName",
-                "apiUrl"
+                "appName"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) groups and associated contracts inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Endpoint Groups - Contracts",
             "ui_columns": [
                 "apiUrl",
@@ -4157,24 +4193,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/apic/service-graphs",
             "api_scope_id": "0648458a01e6306ee2073026755a069597e66b82",
             "columns": [
-                "functionTemplateType",
-                "slug",
-                "tenant",
-                "functionType",
                 "device",
+                "tenant",
                 "id",
-                "state",
+                "apiUrl",
+                "functionType",
                 "name",
+                "slug",
                 "nodeName",
-                "apiUrl"
+                "functionTemplateType",
+                "state"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) Service Graphs",
             "method": "post",
             "nested_columns": [],
             "summary": "APIC Service Graphs",
             "ui_columns": [
                 "apiUrl",
@@ -4246,19 +4282,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/attributes/graphs",
             "api_scope_id": "5ca7fa1061686eb1a61f6ee42853a87db19d4011",
             "columns": [
-                "layout",
                 "id",
+                "layout",
                 "name",
-                "path",
-                "label"
+                "label",
+                "path"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/attributes/graphs",
             "ui_columns": [
                 "id",
@@ -4326,19 +4362,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/attributes/summary",
             "api_scope_id": "3a5ed41ba4bfd6e5789905185b7accdb3039617a",
             "columns": [
-                "layout",
                 "id",
+                "layout",
                 "name",
-                "path",
-                "label"
+                "label",
+                "path"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/attributes/summary",
             "ui_columns": [
                 "id",
@@ -4356,33 +4392,35 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/cloud/virtual-machines",
             "api_scope_id": "845ee1f3eeb63f6daabff1c11d5cfb1330eda9e1",
             "columns": [
-                "slug",
-                "image",
+                "os",
                 "siteName",
-                "numberOfInterfaces",
+                "sn",
                 "id",
                 "name",
-                "os",
-                "sn",
-                "hostname",
-                "status"
+                "status",
+                "numberOfInterfaces",
+                "slug",
+                "image",
+                "vmId",
+                "hostname"
             ],
             "description": "Public or private cloud virtual machines",
             "method": "post",
             "nested_columns": [],
             "summary": "Virtual Machines",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "name",
+                "vmId",
                 "status",
                 "os",
                 "image",
                 "numberOfInterfaces",
                 "slug"
             ],
             "web_endpoint": "/technology/cloud/virtual-machines"
@@ -4394,28 +4432,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/cloud/virtual-machines-interfaces",
             "api_scope_id": "6ae9e708aaad8029584abab2d39014caef632261",
             "columns": [
-                "slug",
+                "inAcl",
                 "siteName",
-                "ipv6Addresses",
+                "sn",
+                "id",
                 "vmName",
+                "slug",
+                "intName",
                 "vmIntId",
+                "hostname",
+                "ipv6Addresses",
                 "vmIntName",
-                "outAcl",
-                "id",
-                "sn",
-                "ipAddresses",
                 "mac",
-                "inAcl",
-                "hostname",
-                "intName"
+                "outAcl",
+                "ipAddresses"
             ],
             "description": "Public or private cloud virtual machines interfaces",
             "method": "post",
             "nested_columns": [
                 "ipAddresses",
                 "ipv6Addresses",
                 "inAcl",
@@ -4446,32 +4484,32 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/received",
             "api_scope_id": "b05678b196ad2944a184f09d48042ffefbec040a",
             "columns": [
                 "total",
-                "id",
-                "bootRequest",
-                "dropped",
+                "siteName",
+                "sn",
                 "nak",
+                "inform",
                 "discover",
-                "received",
-                "hostname",
-                "release",
+                "sent",
                 "request",
-                "ack",
-                "sn",
+                "bootRequest",
+                "decline",
+                "hostname",
+                "relayed",
+                "dropped",
                 "bootReply",
+                "received",
+                "ack",
                 "offer",
-                "inform",
-                "siteName",
-                "relayed",
-                "decline",
-                "sent"
+                "release",
+                "id"
             ],
             "description": "DHCP relay global statistics - received messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Global statistics - received",
             "ui_columns": [
                 "hostname",
@@ -4498,32 +4536,32 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/relayed",
             "api_scope_id": "1b26c6a2c608fc547040f5756b9ccd042fad1c48",
             "columns": [
                 "total",
-                "id",
-                "bootRequest",
-                "dropped",
+                "siteName",
+                "sn",
                 "nak",
+                "inform",
                 "discover",
-                "received",
-                "hostname",
-                "release",
+                "sent",
                 "request",
-                "ack",
-                "sn",
+                "bootRequest",
+                "decline",
+                "hostname",
+                "relayed",
+                "dropped",
                 "bootReply",
+                "received",
+                "ack",
                 "offer",
-                "inform",
-                "siteName",
-                "relayed",
-                "decline",
-                "sent"
+                "release",
+                "id"
             ],
             "description": "DHCP relay global statistics - relayed messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Global statistics - Relayed",
             "ui_columns": [
                 "hostname",
@@ -4550,32 +4588,32 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/sent",
             "api_scope_id": "5eac1ba680f1f318a577ac4b184961323746dcad",
             "columns": [
                 "total",
-                "id",
-                "bootRequest",
-                "dropped",
+                "siteName",
+                "sn",
                 "nak",
+                "inform",
                 "discover",
-                "received",
-                "hostname",
-                "release",
+                "sent",
                 "request",
-                "ack",
-                "sn",
+                "bootRequest",
+                "decline",
+                "hostname",
+                "relayed",
+                "dropped",
                 "bootReply",
+                "received",
+                "ack",
                 "offer",
-                "inform",
-                "siteName",
-                "relayed",
-                "decline",
-                "sent"
+                "release",
+                "id"
             ],
             "description": "DHCP relay global statistics - sent messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Global statistics - Sent",
             "ui_columns": [
                 "hostname",
@@ -4602,21 +4640,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/summary",
             "api_scope_id": "07d758f84c68ea84bcb21ca3411fb77db96f5b48",
             "columns": [
                 "siteName",
-                "id",
                 "sn",
-                "dropped",
-                "relayed",
+                "id",
                 "received",
                 "sent",
-                "hostname"
+                "hostname",
+                "relayed",
+                "dropped"
             ],
             "description": "DHCP relay global statistics summary",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Global stats summary",
             "ui_columns": [
                 "hostname",
@@ -4635,29 +4673,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces",
             "api_scope_id": "b15866e556186706040db812bc17b82300e74890",
             "columns": [
-                "proxyOptions",
+                "options",
                 "siteName",
-                "id",
-                "proxy",
                 "sn",
-                "name",
-                "dropped",
+                "id",
                 "received",
-                "options",
-                "relayed",
-                "sent",
+                "name",
                 "ip",
-                "vrf",
-                "hostname",
                 "intName",
+                "sent",
+                "hostname",
+                "vrf",
+                "proxy",
+                "proxyOptions",
+                "relayed",
+                "dropped",
                 "strategy"
             ],
             "description": "DHCP relay interfaces inventory",
             "method": "post",
             "nested_columns": [
                 "options",
                 "proxyOptions"
@@ -4690,28 +4728,28 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces-stats/received",
             "api_scope_id": "71f56607fadf9778d20720b921d885c8eb4adfe0",
             "columns": [
                 "total",
                 "siteName",
+                "sn",
                 "nak",
                 "id",
-                "bootRequest",
+                "decline",
                 "discover",
+                "inform",
                 "ack",
+                "intName",
                 "request",
-                "sn",
-                "bootReply",
-                "decline",
+                "hostname",
+                "bootRequest",
                 "offer",
                 "release",
-                "hostname",
-                "inform",
-                "intName"
+                "bootReply"
             ],
             "description": "DHCP relay interfaces statistics - received messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Interfaces stats - Received",
             "ui_columns": [
                 "hostname",
@@ -4740,28 +4778,28 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces-stats/relayed",
             "api_scope_id": "59dc994dd10fd6a2759645e5fbd3e0b68213ebcc",
             "columns": [
                 "total",
                 "siteName",
+                "sn",
                 "nak",
                 "id",
-                "bootRequest",
+                "decline",
                 "discover",
+                "inform",
                 "ack",
+                "intName",
                 "request",
-                "sn",
-                "bootReply",
-                "decline",
+                "hostname",
+                "bootRequest",
                 "offer",
                 "release",
-                "hostname",
-                "inform",
-                "intName"
+                "bootReply"
             ],
             "description": "DHCP relay interfaces statistics - relayed messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Interfaces stats - Relayed",
             "ui_columns": [
                 "hostname",
@@ -4790,28 +4828,28 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces-stats/sent",
             "api_scope_id": "25ba9479038c2644d62f38ff4b4ac9f9b8b8370a",
             "columns": [
                 "total",
                 "siteName",
+                "sn",
                 "nak",
                 "id",
-                "bootRequest",
+                "decline",
                 "discover",
+                "inform",
                 "ack",
+                "intName",
                 "request",
-                "sn",
-                "bootReply",
-                "decline",
+                "hostname",
+                "bootRequest",
                 "offer",
                 "release",
-                "hostname",
-                "inform",
-                "intName"
+                "bootReply"
             ],
             "description": "DHCP relay interfaces statistics - sent messages",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Relay Interfaces stats - Sent",
             "ui_columns": [
                 "hostname",
@@ -4839,20 +4877,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/excluded-ranges",
             "api_scope_id": "99d16794d1d2f025f1cd8f2d04da13b4edf0dae1",
             "columns": [
                 "siteName",
-                "range",
-                "id",
-                "serverName",
                 "sn",
+                "serverId",
+                "id",
                 "hostname",
-                "serverId"
+                "serverName",
+                "range"
             ],
             "description": "DHCP server excluded ranges inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Server Excluded Ranges",
             "ui_columns": [
                 "hostname",
@@ -4870,20 +4908,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/interfaces",
             "api_scope_id": "3e0a61543fd85e7d14dca2b7bc33966a81a20e22",
             "columns": [
                 "siteName",
-                "id",
-                "serverName",
                 "sn",
-                "hostname",
                 "serverId",
-                "intName"
+                "id",
+                "intName",
+                "hostname",
+                "serverName"
             ],
             "description": "DHCP server interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Server Interfaces",
             "ui_columns": [
                 "hostname",
@@ -4900,29 +4938,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/leases",
             "api_scope_id": "df053403d81a055d9dacd6ca83ce379a320233ab",
             "columns": [
-                "siteName",
                 "type",
-                "client",
-                "id",
-                "state",
-                "leaseExpiration",
-                "serverName",
+                "siteName",
                 "sn",
+                "serverId",
+                "id",
+                "ip",
                 "intName",
-                "vrf",
                 "hostname",
-                "serverId",
-                "ip"
+                "serverName",
+                "leaseExpiration",
+                "vrf",
+                "client",
+                "state"
             ],
-            "description": "DHCP Server ",
+            "description": "DHCP Server",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Server Leases",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "intName",
@@ -4944,26 +4982,26 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/pools",
             "api_scope_id": "0272de31f9cc4b2eb99c98019662373ad313eb72",
             "columns": [
                 "rangeUsage",
+                "rangeOptions",
                 "siteName",
-                "range",
+                "sn",
+                "serverId",
                 "id",
-                "rangeType",
-                "rangeOptions",
                 "poolOptions",
-                "serverName",
-                "sn",
                 "name",
-                "vrf",
                 "hostname",
-                "serverId"
+                "serverName",
+                "vrf",
+                "range",
+                "rangeType"
             ],
             "description": "DHCP Server pools inventory",
             "method": "post",
             "nested_columns": [
                 "poolOptions",
                 "rangeOptions"
             ],
@@ -4989,23 +5027,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/summary",
             "api_scope_id": "5bd9af227930616f4b790a7a4495e1c2a5607f64",
             "columns": [
+                "sn",
                 "siteName",
-                "leasesCount",
                 "id",
-                "poolsCount",
-                "serverName",
-                "sn",
+                "intNamesCount",
                 "excludedRangesCount",
                 "hostname",
-                "intNamesCount"
+                "serverName",
+                "poolsCount",
+                "leasesCount"
             ],
             "description": "DHCP server summary information inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Server Summary",
             "ui_columns": [
                 "hostname",
@@ -5025,24 +5063,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/balancing",
             "api_scope_id": "9a13e4af94cf0b36dd961fbe07635442b812eb5d",
             "columns": [
-                "nei2",
-                "virtIp",
-                "nei1",
-                "id",
                 "nei2Sn",
-                "nei1Sn",
+                "id",
+                "nei1",
+                "virtIp",
                 "vrf",
-                "pct"
+                "nei2",
+                "pct",
+                "nei1Sn"
             ],
-            "description": "Balancing ratios for FHRP gateways",
+            "description": "First hop redundancy protocols (FHRP) such as HSRP, VRRP, and GLBP provide L3 default gateway redundancy for network hosts (endpoints) in one IP subnet (broadcast domain).\\\nWhen the FHRP pair shares more than one FHRP group (ie. multiple IP subnets have L3 default gateway on the same router pair), balancing may be employed for better capacity utilization.\\\nThis table presents the ratio of the FHRP active groups on the first neighbor to the FHRP active groups on the second neighbor.\n\n---\n\n\"Balancing Ratio\" column values:\n  * 100: All FHRP groups are active on the first router in FHRP pair (Gateway 1)\n  * 99-51: Majority of the FHRP groups are active on the first router in FHRP pair (Gateway 1)\n  * 50: All FHRP groups are evenly distributed between both routers in FHRP pair\n  * 49-1: Majority of the FHRP groups are active on the second router in FHRP pair (Gateway 2)\n  * 0: All FHRP groups are active on the second router in FHRP pair (Gateway 2)",
             "method": "post",
             "nested_columns": [],
             "summary": "Active FHRP gateway balancing",
             "ui_columns": [
                 "nei1",
                 "nei2",
                 "pct",
@@ -5058,27 +5096,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/glbp-forwarders",
             "api_scope_id": "e43daff2e67dcbd8f3dc23d0c0da851041b439d6",
             "columns": [
-                "siteName",
                 "active",
+                "siteName",
+                "sn",
                 "group",
                 "id",
-                "state",
-                "sn",
                 "address",
-                "vrf",
-                "hostname",
                 "intName",
-                "forwarder"
+                "hostname",
+                "forwarder",
+                "vrf",
+                "state"
             ],
-            "description": "GLBP forwarders inventory",
+            "description": "This table covers all GLBP forwarders in the network. Unlike HSRP and VRRP, GLBP member routers operate in active/active mode. Each router in a group (called active vritual forwarder, AVF) is used to forward the traffic from a subset of endpoints in a given subnet. Each AVF have its own unique virtual MAC address. Thus one GLBP group with one shared virtual IP address use multiple virtual MAC addresses for this virtual IP.\n\nOne router in a group, called the Active Virtual Gateway (AVG), responds to ARP requests for IP-to-MAC mapping of the default gateway IP address from the endpoints. According to configured AVF weights, AVG responds to endpoints with differents virtual MAC addresses (which belong to different AVFs). Usually one endpoint will always get the same MAC address of AVF based on hashing mechanism.\n\nThere are backup mechanisms in place to take over if either AVG of one of the AVFs fail.\n* If AVG fails, backup AVG will take over (router with second highest AVG priority)\n* If one of the AVF fails, one of the remaining AVFs start to process the traffic destined for the MAC address of the failed AVF. For some period of time, this AVF will process the traffic for two different virtual MAC addresses.\n* There should be only one active AVG in the group. Dual-active AVG scenarios are undesired.\n* There should be (at least) two members and thus two AVFs in each GLBP group. One AVF member in a group should be investigated.",
             "method": "post",
             "nested_columns": [],
             "summary": "GLBP forwarders",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -5100,21 +5138,21 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/group-members",
             "api_scope_id": "8dde2c05e424950eabfe4c1f3d96f8c31cfa68d7",
             "columns": [
                 "devices",
                 "id",
-                "protocol",
-                "count",
                 "virtualIpv6",
-                "vrf",
-                "virtualIp"
+                "virtualIp",
+                "count",
+                "protocol",
+                "vrf"
             ],
-            "description": "HSRP/VRRP/GLBP Group members - gateway inventory",
+            "description": "First hop redundancy protocols (FHRP) such as HSRP, VRRP, and GLBP provide gateway redundancy for network hosts (endpoints).\nA single IP address is served by one or more routers in active/standby or active/active configuration, depending on the protocol used.\\\nFHRP group member table covers all configured FHRP groups in the network and the members of each group. The state of each member is covered in the table as well.\n\nRedundancy protocols are not fully state aware due to limited two-way handshake, resulting in undesired active/active or down/standby scenarios when unidirectional links are present, causing traffic black holing. Only one router in FHRP group should be active and only one FHRP router in the group\n\n---\n\n* Only one protocol type should be used\n* There should be (at least) two members in each FHRP group. One member should be investigated.\n* There should be only one \"active/master\" and only one \"standby/backup\" router in each group. Dual-active scenarios are undesired.\n\nPossible FHRP protocols are:\n* HSRP - Hot Standby Redundancy protocol (RFC 2281, originally Cisco proprietary protocol)\n* VRRP - Virtual Router Redundancy protocol (RFC 3768)\n* GLBP - Gateway Load Balancing protocol (Cisco proprietary protocol)",
             "method": "post",
             "nested_columns": [],
             "summary": "HSRP/VRRP/GLBP Group members",
             "ui_columns": [
                 "virtualIp",
                 "virtualIpv6",
                 "protocol",
@@ -5131,34 +5169,34 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/group-state",
             "api_scope_id": "a93fab66e04c9ec69c28f3c780afe0faf0a40b1d",
             "columns": [
-                "vrf",
-                "siteName",
                 "active",
+                "secondaryVirtualIpAddresses",
+                "siteName",
+                "sn",
                 "group",
                 "id",
-                "priority",
-                "state",
-                "version",
-                "protocol",
-                "sn",
+                "standby",
                 "virtualIpv6",
+                "version",
+                "priority",
+                "virtualIp",
+                "intName",
                 "count",
-                "secondaryVirtualIpAddresses",
-                "preempt",
+                "protocol",
                 "hostname",
-                "standby",
-                "intName",
-                "virtualIp"
+                "vrf",
+                "state",
+                "preempt"
             ],
-            "description": "HSRP/VRRP/GLBP Group State - detailed gateway inventory",
+            "description": "First hop redundancy protocols (FHRP) such as HSRP, VRRP, and GLBP provide gateway redundancy for network hosts (endpoints).\nA single IP address is served by one or more routers in active/standby or active/active configuration, depending on the protocol used.\\\nFHRP group state table covers all L3 interfaces on all routers where any of the FHRP protocols are configured. Those interfaces perform the function of the virtual L3 default gateway for the endpoints in respective subnet. State table depicts if the interface is in active/master state (actively forwarding the traffic destined for virtual L3 default gateway) or in standby/backup state (waiting to take over in case the active FHRP router fails)\n\nRedundancy protocols are not fully state aware due to limited two-way handshake, resulting in undesired active/active or down/standby scenarios when unidirectional links are present, causing traffic black holing. Only one router in FHRP group should be active and only one FHRP router in the group\n\n---\n\n* Only one protocol type should be used\n* The priority of FHRP routers in one group should be different (higher numbers mean higher probability to become active/master). Preemptive behaviour is desired.\n* If there is one FHRP group on the interface, all routers should be members of the same group.\n* There should be (at least) two routers in each FHRP group. All such routers should have the same Virtual IP configured\n* Only \"active/master\" or \"standby/backup\" state should appear in the converged state. Other states are short-lived only.\n* There should be only one \"active/master\" and only one \"standby/backup\" router in each group\n\nPossible FHRP protocols are:\n* HSRP - Hot Standby Redundancy protocol (RFC 2281, originally Cisco proprietary protocol)\n* VRRP - Virtual Router Redundancy protocol (RFC 3768)\n* GLBP - Gateway Load Balancing protocol (Cisco proprietary protocol)",
             "method": "post",
             "nested_columns": [
                 "secondaryVirtualIpAddresses"
             ],
             "summary": "HSRP/VRRP/GLBP Group State",
             "ui_columns": [
                 "hostname",
@@ -5188,21 +5226,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/stproot-alignment",
             "api_scope_id": "3bfd2b41fc7a20ee62a7bd41514b8f1619ef0a48",
             "columns": [
                 "siteName",
-                "id",
                 "sn",
+                "vlans",
+                "id",
                 "count",
-                "hostname",
-                "vlans"
+                "hostname"
             ],
-            "description": "Misaligned FHRP Gateways with STP Root",
+            "description": "First hop redundancy protocols (FHRP) such as HSRP, VRRP, and GLBP provide L3 default gateway redundancy for network hosts (endpoints) in one IP subnet (broadcast domain).\\\nSpanning tree (STP) protocol provide the central point of switched links in one broadcast domain (VLAN) called the root switch for given VLAN.\\\nOn multilayer L2/L3 switches those protocols could meet on the same device.\n\nActive routing FHRP gateway (regardless if HSRP, VRRP or GLBP based) should be aligned with spanning tree (STP) root when both protocols are running on the same device. Different location of STP root and active FHRP gateway can cause unknown unicast floods, exponentially network load.",
             "method": "post",
             "nested_columns": [],
             "summary": "FHRP Gateway and STP Root Aligment",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "count",
@@ -5217,28 +5255,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/fhrp/virtual-gateways",
             "api_scope_id": "1a71450017c72c31e8f659137c654bfd155f02ce",
             "columns": [
-                "siteName",
                 "type",
-                "id",
-                "state",
-                "protocol",
+                "siteName",
                 "sn",
-                "virtualMac",
+                "id",
                 "virtualIpv6",
-                "vrf",
-                "hostname",
+                "virtualIp",
                 "intName",
-                "virtualIp"
+                "virtualMac",
+                "protocol",
+                "hostname",
+                "vrf",
+                "state"
             ],
-            "description": "Virtual gateways inventory for Arista VARP",
+            "description": "Virtual gateway protocols, Arista VARP, Aruba VSX Active gateway",
             "method": "post",
             "nested_columns": [],
             "summary": "Arista VARP",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -5259,17 +5297,17 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/global-attributes",
             "api_scope_id": "6190fa52f1dc472252730653d5b3f51aadc3c2b0",
             "columns": [
+                "sn",
                 "id",
                 "name",
-                "sn",
                 "value",
                 "hostname"
             ],
             "description": "Global attributes inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Global Attributes",
@@ -5289,27 +5327,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/connectivity-matrix",
             "api_scope_id": "a3137fc62a0e223ff0361957fb4b2b1f14ced97e",
             "columns": [
+                "remoteHost",
                 "localMedia",
+                "remoteMedia",
+                "localHost",
                 "siteName",
                 "id",
                 "remoteInt",
-                "localInt",
-                "remoteHost",
-                "localHost",
-                "protocol",
                 "remoteSn",
-                "remoteMedia",
+                "protocol",
+                "localInt",
                 "localSn"
             ],
-            "description": "Logical and physical connectivity matrix for variety of protocols",
+            "description": "This table covers the list of pairs of devices connected to each other. Pairing can be derived from local connection (via &quot;cdp/lldp&quot;\nprotocol), spanning tree binding (&quot;stp&quot; protocol) or routing next-hop neighbor (via &quot;cef/fib&quot; protocol)\\\nEach device pair is shown twice in this table - from the point of view of both devices\\\nLocal and remote media types should be the same in each pairing.",
             "method": "post",
             "nested_columns": [],
             "summary": "Connectivity matrix",
             "ui_columns": [
                 "localHost",
                 "localInt",
                 "siteName",
@@ -5328,27 +5366,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/connectivity-matrix/unmanaged-neighbors/detail",
             "api_scope_id": "bdc9d74ab378e68c5b0afa3604ad661aead4a70a",
             "columns": [
-                "siteName",
-                "neiIpV6",
                 "localAddress",
-                "id",
-                "devType",
-                "localAddressV6",
                 "neiIp",
-                "protocol",
+                "siteName",
                 "sn",
+                "id",
+                "localAddressV6",
                 "source",
+                "intName",
+                "protocol",
                 "hostname",
                 "subnet",
-                "intName"
+                "devType",
+                "neiIpV6"
             ],
             "description": "Details for unmanaged neighbors detected via variety of protocols",
             "method": "post",
             "nested_columns": [],
             "summary": "Unmanaged Neighbors Detail",
             "ui_columns": [
                 "hostname",
@@ -5367,34 +5405,34 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/connectivity-matrix/unmanaged-neighbors/summary",
             "api_scope_id": "50778eb92b26f715d12e836feb43136450a1ba6b",
             "columns": [
-                "id",
+                "siteName",
+                "sn",
+                "neighbor",
                 "ipv6",
-                "ospfNeiCount",
-                "capabilities",
-                "cefPrfx",
                 "ldpNeiCount",
+                "cefPrfx",
+                "ospfv3NeiCount",
                 "hostname",
-                "bgpReceivedPfx",
-                "isisNeiCount",
-                "bgpNeiAsn",
-                "sn",
-                "cefNeiCount",
                 "eigrpNeiCount",
                 "xdpNeiCount",
+                "cefNeiCount",
                 "ip",
-                "siteName",
+                "isisNeiCount",
+                "bgpNeiAsn",
+                "bgpReceivedPfx",
+                "id",
                 "ripNeiCount",
-                "neighbor",
-                "ospfv3NeiCount",
-                "bgpNeiCount"
+                "bgpNeiCount",
+                "ospfNeiCount",
+                "capabilities"
             ],
             "description": "Summary for unmanaged neighbors detected via variety of protocols",
             "method": "post",
             "nested_columns": [
                 "capabilities"
             ],
             "summary": "Unmanaged Neighbors Summary",
@@ -5426,31 +5464,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/counters/inbound",
             "api_scope_id": "9585e835675c9a6833b98059cdd94b3b10f3877e",
             "columns": [
+                "inBcast",
+                "inPkts",
+                "inNoBuffer",
                 "inMcast",
+                "inDrops",
                 "inBytes",
-                "inErr",
-                "inNoBuffer",
+                "inRunts",
                 "siteName",
-                "inBcast",
                 "id",
-                "inGiants",
-                "inDrops",
-                "inCrc",
-                "inPkts",
                 "sn",
-                "inOverrun",
-                "inRunts",
-                "inStompedCrc",
+                "inCrc",
+                "intName",
                 "hostname",
-                "intName"
+                "inStompedCrc",
+                "inGiants",
+                "inErr",
+                "inOverrun"
             ],
             "description": "Interfaces inbound counters - absolute values",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Counters - Inbound",
             "ui_columns": [
                 "hostname",
@@ -5478,32 +5516,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/counters/outbound",
             "api_scope_id": "8feb39afbeda7b063265225dcd0f0ac460f7d992",
             "columns": [
+                "outNoCarrier",
+                "outLateCollisions",
                 "siteName",
-                "outCollisions",
+                "sn",
                 "outDeferred",
-                "outErr",
                 "id",
-                "outLostCarrier",
-                "outBufferDrop",
-                "sn",
+                "outMcast",
+                "outBabble",
                 "outDrops",
-                "outNoCarrier",
-                "outPkts",
-                "outBytes",
+                "outCollisions",
+                "intName",
                 "outBcast",
-                "outLateCollisions",
-                "outMcast",
+                "outPkts",
                 "hostname",
-                "intName",
-                "outBabble"
+                "outBufferDrop",
+                "outErr",
+                "outBytes",
+                "outLostCarrier"
             ],
             "description": "Interfaces outbound counters - absolute values",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Counters - Oubound",
             "ui_columns": [
                 "hostname",
@@ -5532,23 +5570,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/bidirectional",
             "api_scope_id": "55d36efb15d823453e640a21479e832131ce9afe",
             "columns": [
-                "siteName",
-                "bytesRate",
-                "id",
                 "dropsPktsPct",
+                "siteName",
                 "sn",
                 "impactDrops",
+                "id",
+                "bytesRate",
+                "intName",
                 "dropsRate",
-                "hostname",
-                "intName"
+                "hostname"
             ],
             "description": "Input and Output interface drops combined providing a bidirectional view of drops on an interface",
             "method": "post",
             "nested_columns": [],
             "summary": "Bidirectional Interface Drops",
             "ui_columns": [
                 "hostname",
@@ -5568,20 +5606,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/bidirectional-device",
             "api_scope_id": "d450e0e8e4f75918fc478c05898c951fca66e293",
             "columns": [
-                "siteName",
-                "bytesRate",
-                "id",
                 "dropsPktsPct",
+                "siteName",
                 "sn",
                 "impactDrops",
+                "id",
+                "bytesRate",
                 "dropsRate",
                 "hostname"
             ],
             "description": "Input and Output drops of all interfaces on a device combined proviing a per-device view of bidirectional interface drops",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Bidirectional Interface Drops",
@@ -5602,23 +5640,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/inbound",
             "api_scope_id": "c12f0e948f78f3ad7c859768b1874f0187fa9e7f",
             "columns": [
-                "inDropsPktsPct",
-                "inDropsRate",
                 "siteName",
-                "id",
-                "inImpactDrops",
                 "sn",
-                "hostname",
+                "id",
+                "inDropsRate",
+                "intName",
                 "inBytesRate",
-                "intName"
+                "hostname",
+                "inImpactDrops",
+                "inDropsPktsPct"
             ],
             "description": "Input interface drops represent packet loss caused by input buffer overflow",
             "method": "post",
             "nested_columns": [],
             "summary": "Inbound Interface Drops",
             "ui_columns": [
                 "hostname",
@@ -5638,22 +5676,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/inbound-device",
             "api_scope_id": "c38e8e6b75840aef445c1ebcccbc471b6767fd19",
             "columns": [
-                "inDropsPktsPct",
-                "inDropsRate",
                 "siteName",
-                "id",
-                "inImpactDrops",
                 "sn",
+                "id",
+                "inDropsRate",
+                "inBytesRate",
                 "hostname",
-                "inBytesRate"
+                "inImpactDrops",
+                "inDropsPktsPct"
             ],
             "description": "Input drops of all interfaces on a device combined providing a per-device view of input interface drops",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Inbound Interface Drops",
             "ui_columns": [
                 "hostname",
@@ -5672,25 +5710,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/outbound",
             "api_scope_id": "17fbfe82210952b858a2cd2daddf7430aeafa502",
             "columns": [
-                "outDropsPktsPct",
+                "outDropsRate",
                 "siteName",
+                "sn",
+                "outDropsPktsPct",
                 "id",
                 "outBytesRate",
-                "sn",
-                "outDropsRate",
-                "outImpactDrops",
+                "intName",
                 "hostname",
-                "intName"
+                "outImpactDrops"
             ],
-            "description": "Output interface drops represent outbound packet loss",
+            "description": "Output interface drops represent packet loss caused by output buffer overflow. Output drops are one of the most prevalent reasons for packet loss in\nIP networks, and usually signifies path overutilization.",
             "method": "post",
             "nested_columns": [],
             "summary": "Outbound Interface Drops",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -5708,22 +5746,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/outbound-device",
             "api_scope_id": "cf72f642a249e5a614a1eb798f672840e42311e9",
             "columns": [
-                "outDropsPktsPct",
+                "outDropsRate",
                 "siteName",
+                "sn",
+                "outDropsPktsPct",
                 "id",
                 "outBytesRate",
-                "sn",
-                "outDropsRate",
-                "outImpactDrops",
-                "hostname"
+                "hostname",
+                "outImpactDrops"
             ],
             "description": "Output drops of all interfaces on a device combined providing a per-device view of output interface drops",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Outbound Interface Drops",
             "ui_columns": [
                 "hostname",
@@ -5743,28 +5781,28 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/duplex",
             "api_scope_id": "a1ccbb224b7191ef8c2b1c65ad28c2a3b2777ff6",
             "columns": [
                 "localMedia",
+                "localIntName",
                 "remoteIntName",
+                "remoteMedia",
                 "siteName",
                 "id",
-                "localIntName",
                 "localHostname",
-                "remoteSn",
                 "remoteHostname",
-                "localDuplex",
-                "remoteMedia",
-                "localSn",
+                "remoteDuplex",
+                "remoteSn",
                 "status",
-                "remoteDuplex"
+                "localDuplex",
+                "localSn"
             ],
-            "description": "Interface connectivity matrix including duplex information",
+            "description": "Most network equipment supports and prefers full duplex setting. There are few exceptions when half duplex operation is necessary, and in such a case\nall sides must be set for consistently half-duplex operation. Most frequent cause of half-duplex state is due to poor compatibility in historical\nEthernet standard implementations, or from legacy configuration.\n\nDuplex directly impacts both performance and capacity. Performance is further impacted due to wait times before sending traffic, imposed by the\nmandatory minimum interval dictated by CSMA/CD. Duplex issues cause packet loss due to alignment errors, input errors due to overvoltage that\nscrambles encoding on the link, and other collision induced performance degradation, worsened by often inconsistent duplex state of direct neighbors.",
             "method": "post",
             "nested_columns": [],
             "summary": "Duplex interface matrix",
             "ui_columns": [
                 "status",
                 "localHostname",
                 "localIntName",
@@ -5787,21 +5825,21 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/bidirectional",
             "api_scope_id": "2cb7ec9e5e7c1354dc90b89a34497489148908f0",
             "columns": [
                 "errPktsPct",
                 "siteName",
-                "bytesRate",
-                "id",
                 "sn",
                 "impactErr",
-                "errRate",
+                "id",
+                "bytesRate",
+                "intName",
                 "hostname",
-                "intName"
+                "errRate"
             ],
             "description": "Sum of inbound and outbound interface error impacts to provide a bidirectional view of overall impact of errors on an interface",
             "method": "post",
             "nested_columns": [],
             "summary": "Bidirectional Interface Errors",
             "ui_columns": [
                 "hostname",
@@ -5823,20 +5861,20 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/bidirectional-device",
             "api_scope_id": "da6bd6dabe772a333a496b2f1f29e4160020f2ca",
             "columns": [
                 "errPktsPct",
                 "siteName",
-                "bytesRate",
-                "id",
                 "sn",
                 "impactErr",
-                "errRate",
-                "hostname"
+                "id",
+                "bytesRate",
+                "hostname",
+                "errRate"
             ],
             "description": "Bidirectional Input and Output errors of all interfaces on each device combined providing a per-device Impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Bidirectional Interface Errors",
             "ui_columns": [
                 "hostname",
@@ -5856,21 +5894,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/disabled",
             "api_scope_id": "44dbf28ae5ee9173b282db75edcf43abbb2d7baa",
             "columns": [
                 "siteName",
-                "errorReason",
-                "id",
                 "sn",
+                "id",
+                "intName",
                 "hostname",
-                "intName"
+                "errorReason"
             ],
-            "description": "Interfaces in the network which has been automatically disabled due to an error",
+            "description": "This table shows all interfaces in the network which has been automatically disabled due to some kind of communication error.\\\nInterfaces are disabled due to violation of operational parameter, and should be self-healed by the automatic recovery timers, or recovered manually,\nensuring that the violation will not occur in the future.\\\nThere should be no interfaces disabled due to error.",
             "method": "post",
             "nested_columns": [],
             "summary": "Error-Disabled interfaces",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -5885,25 +5923,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/inbound",
             "api_scope_id": "468742fac6ba3687fe28cb1e4a6080d98dfeecb9",
             "columns": [
-                "inErrPktsPct",
                 "siteName",
-                "id",
-                "inErrRate",
                 "sn",
                 "inImpactErr",
-                "hostname",
+                "id",
+                "inErrPktsPct",
+                "intName",
                 "inBytesRate",
-                "intName"
+                "hostname",
+                "inErrRate"
             ],
-            "description": "Input interface errors represent packet loss caused by input buffer overflow",
+            "description": "Input interface errors signify the number of packets that had to be dropped because the packet could not be read. Input errors are caused by poor\nquality of physical wiring, ruptured cables, dirty connectors, network hardware faults, or other physical issues. Because input errors are closely\nassociated with the physical layer they are often referred to as hard errors.",
             "method": "post",
             "nested_columns": [],
             "summary": "Inbound Interface Errors",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -5921,22 +5959,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/inbound-device",
             "api_scope_id": "ee8e51dfbce7c1bfb1980988d36f80f42a101a16",
             "columns": [
-                "inErrPktsPct",
                 "siteName",
-                "id",
-                "inErrRate",
                 "sn",
                 "inImpactErr",
+                "id",
+                "inErrPktsPct",
+                "inBytesRate",
                 "hostname",
-                "inBytesRate"
+                "inErrRate"
             ],
             "description": "Input errors of all interfaces on a device combined providing a per-device view of input interface errors",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Inbound Interface Errors",
             "ui_columns": [
                 "hostname",
@@ -5956,24 +5994,24 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/outbound",
             "api_scope_id": "f8e2d3777206f652f3941d24ab28bd764fe64d67",
             "columns": [
                 "outErrPktsPct",
+                "outErrRate",
                 "siteName",
+                "sn",
                 "id",
                 "outBytesRate",
-                "outImpactErr",
-                "sn",
-                "outErrRate",
+                "intName",
                 "hostname",
-                "intName"
+                "outImpactErr"
             ],
-            "description": "Output interface errors represent outbound packet loss",
+            "description": "Output interface errors are caused by local controller or interface failures, such as local encapsulation failures, local hardware failures, and\nmisconfiguration of interface or controller, resulting in failure to properly transmit a packet. Most output errors are avoidable and should be fixed.",
             "method": "post",
             "nested_columns": [],
             "summary": "Outbound Interface Errors",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -5992,21 +6030,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/outbound-device",
             "api_scope_id": "f50046c5c6c9803ae0e34b04d6219f54b9f7b846",
             "columns": [
                 "outErrPktsPct",
+                "outErrRate",
                 "siteName",
+                "sn",
                 "id",
                 "outBytesRate",
-                "outImpactErr",
-                "sn",
-                "outErrRate",
-                "hostname"
+                "hostname",
+                "outImpactErr"
             ],
             "description": "Output errors of all interfaces on a device combined providing a per-device view of output interface errors",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Outbound Interface Errors",
             "ui_columns": [
                 "hostname",
@@ -6025,22 +6063,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/inconsistencies/details",
             "api_scope_id": "40d00675840b09d377ec2d55e4263a0361cfa2d1",
             "columns": [
+                "sn",
                 "siteName",
                 "id",
-                "sn",
+                "intName",
                 "vlanId",
-                "hostname",
-                "intName"
+                "hostname"
             ],
-            "description": "VLANs that are not configured in any STP instance - detailed view",
+            "description": "This table show VLANs which exist in the network and which are not covered by any STP instance.\n\nTo avoid L2 switching loops in Ethernet networks, some kind of loop pruning protocol should be run\nfor all VLANs.\n\nThis table should be empty.",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs without STP instance - Detail",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -6055,21 +6093,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/inconsistencies/summary",
             "api_scope_id": "66e774e452a0de72bffcbc2edb91bc5dcbd69230",
             "columns": [
+                "sn",
                 "siteName",
                 "id",
-                "vlanCount",
-                "sn",
-                "hostname"
+                "hostname",
+                "vlanCount"
             ],
-            "description": "VLANs that are not configured in any STP instance - summary view",
+            "description": "This table show VLANs which exist in the network and which are not covered by any STP instance.\n\nTo avoid L2 switching loops in Ethernet networks, some kind of loop pruning protocol should be run\nfor all VLANs.\n\nThis table should be empty.",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs without STP instance - Summary",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "vlanCount"
@@ -6083,22 +6121,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/load/bidirectional",
             "api_scope_id": "1803e43ebe8097525694112dd415016689a11322",
             "columns": [
+                "interval",
                 "siteName",
+                "sn",
                 "id",
                 "pkts",
-                "sn",
-                "hostname",
-                "bytes",
                 "intName",
-                "interval"
+                "bytes",
+                "hostname"
             ],
             "description": "Interfaces Bidirectional load inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Bidirectional load",
             "ui_columns": [
                 "hostname",
@@ -6117,22 +6155,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/load/inbound",
             "api_scope_id": "f13e3c4d12edc78761d9e77ac745fe56396ea422",
             "columns": [
+                "inPkts",
+                "interval",
                 "inBytes",
                 "siteName",
-                "id",
-                "inPkts",
                 "sn",
-                "hostname",
+                "id",
                 "intName",
-                "interval"
+                "hostname"
             ],
             "description": "Interfaces inbound load inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Inbound load",
             "ui_columns": [
                 "hostname",
@@ -6151,22 +6189,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/load/outbound",
             "api_scope_id": "6cb01cc705e980dec5a6ec78ba3a411fb0a50021",
             "columns": [
+                "interval",
                 "siteName",
-                "id",
                 "sn",
+                "id",
+                "intName",
                 "outPkts",
-                "outBytes",
                 "hostname",
-                "intName",
-                "interval"
+                "outBytes"
             ],
             "description": "Interfaces outbound load inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Outbound load",
             "ui_columns": [
                 "hostname",
@@ -6185,27 +6223,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/mtu",
             "api_scope_id": "872798e56e1c263fed7403c72f8a22003fd986a7",
             "columns": [
+                "srcSn",
                 "srcDev",
                 "siteName",
-                "layer",
-                "dstMtu",
-                "srcMtu",
-                "id",
                 "srcInt",
-                "srcSn",
                 "dstInt",
+                "id",
+                "layer",
+                "dstMtu",
                 "dstSn",
+                "srcMtu",
                 "dstDev"
             ],
-            "description": "Interface connectivity matrix including Maximum Transmission Unit (MTU) information",
+            "description": "Configured Maximum Transmission Unit (MTU) between two devices/ports (source and destination).\n\nMTU is maximum number of bytes that can be transferred on the interface in one frame/packet. More bytes must be fragmented into more packets.\nEncapsulation of transport protocols and tunnels use some bytes for overhead (header fields) and thus leaves less bytes for actual payload.\n\nMTU should be the same on all interfaces configured on the same link (it should reflect the actual transport capability of the link). You can easily\nfind MTU misconfiguration using this table.",
             "method": "post",
             "nested_columns": [],
             "summary": "Maximum Transmission Unit Matrix",
             "ui_columns": [
                 "srcDev",
                 "srcInt",
                 "siteName",
@@ -6224,26 +6262,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/port-channel/balance/inbound",
             "api_scope_id": "8dca3d9008c4106fd0ffb84fc81c5ce955059444",
             "columns": [
+                "members",
                 "siteName",
+                "sn",
                 "variance",
                 "id",
                 "ratios",
+                "intName",
                 "protocol",
-                "sn",
-                "rate",
                 "hostname",
-                "intName",
-                "members"
+                "rate"
             ],
-            "description": "Link Aggregation (LAG)/PortChannel/EtherChannel inbound balancing ratios",
+            "description": "This table shows how the INBOUND traffic is distributed over members in LAG (aka PortChannel aka EtherChannel). The goal is to distribute the traffic\namong the link members evenly - if 100 Mbps should be transferred over 4 links then 25 Mbps should be at each link in best case.\n\nTraffic balancing in real life cannot be completely even - per packet load balancing is not desired as it may disrupt some data flows due to\nout-of-order packets. Per-flow load balancing is desired.\\\nThe issue is:\n  * How to determine the data flows correctly - enough visibility to L2/L3/L4 header fields is required\n  * How to cope with single flows of large capacity - can those be split into multiple flows on the endpoints?\n\nPoor inbound load balancing signifies insufficient entropy on the upstream device. Inbound balancing can be fixed by changing hashing algorithm on the\netherchannel neighbor device.",
             "method": "post",
             "nested_columns": [],
             "summary": "Port Link-Aggregation inbound",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -6262,26 +6300,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/port-channel/balance/outbound",
             "api_scope_id": "f2c6640a91ce438523e14c42a3a979260923aec1",
             "columns": [
+                "members",
                 "siteName",
+                "sn",
                 "variance",
                 "id",
                 "ratios",
+                "intName",
                 "protocol",
-                "sn",
-                "rate",
                 "hostname",
-                "intName",
-                "members"
+                "rate"
             ],
-            "description": "Link Aggregation (LAG)/PortChannel/EtherChannel outbound balancing ratios",
+            "description": "This table shows how the OUTBOUND traffic is distributed over members in LAG (aka PortChannel aka EtherChannel). The goal is to distribute the\ntraffic among the link members evenly - if 100 Mbps should be transferred over 4 links then 25 Mbps should be at each link in best case.\n\nTraffic balancing in real life cannot be completely even - per packet load balancing is not desired as it may disrupt some data flows due to\nout-of-order packets. Per-flow load balancing is desired.\\\nThe issue is:\n\n* How to determine the data flows correctly - enough visibility to L2/L3/L4 header fields is required\n* How to cope with single flows of large capacity - can those be split into multiple flows on the endpoints?\n\nLow variance of transmitted traffic signifies good load distribution, optimum capacity, and performance. Poor load distribution impacts performance by\nadding queuing and scheduling delays, and inducing disproportionate session bandwidth or packet loss. Outbound balancing can be fixed by changing\nhashing algorithm on the device where etherchannel is configured.",
             "method": "post",
             "nested_columns": [],
             "summary": "Port Link-Aggregation Outbound",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -6300,24 +6338,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/port-channel/member-status",
             "api_scope_id": "af69f8a8b7ef9551dd624d74504a71c00a821e90",
             "columns": [
+                "members",
                 "siteName",
+                "sn",
                 "id",
-                "mlagId",
+                "intName",
                 "protocol",
-                "sn",
                 "hostname",
-                "intName",
-                "members"
+                "mlagId"
             ],
-            "description": "State of each link-aggregation member for all configured Link Aggregation (LAG)/PortChannels/EtherChannels",
+            "description": "This table covers the actual state of each member port of all configured LAGs (Portchannels/Etherchannels) in the network.\n\nAll of the member interfaces of an etherchannel should be either in up or down state, representing common operational behavior. When a dynamic\naggregation protocol detects an operational issue, it suspends the member interface. Such interfaces should be addressed as a priority due to a\npotentially damaging behavior that can result from inconsistently configured channels.\n\n  * (P) - member is up and bundled in channel (desired)\n  * (D) - member is down (port is not active)\n  * (I) - member is up but it is not bundled in channel (it is in individual state)\n  * (w) - member is up but it is waiting to be bundled in the channel (it is in waiting state)\n  * (S) - member is suspended - immediate attention is recommended",
             "method": "post",
             "nested_columns": [],
             "summary": "Port Link-Aggregation Member Status",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -6336,21 +6374,21 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/pppoe",
             "api_scope_id": "8e8ccbd7823eab1014e0d1f4d649558ecfc441a1",
             "columns": [
                 "total",
                 "siteName",
-                "other",
-                "forwarded",
+                "sn",
                 "id",
+                "forwarded",
                 "local",
-                "sn",
+                "intName",
                 "hostname",
-                "intName"
+                "other"
             ],
             "description": "Point-to-Point Protocol over Ethernet (PPPoE) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PPPoE interfaces",
             "ui_columns": [
                 "hostname",
@@ -6370,33 +6408,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/pppoe/sessions",
             "api_scope_id": "5cc25601bec2e60dd0856b57fa88b8ffcf6c50e0",
             "columns": [
-                "id",
-                "inPktsRate",
+                "siteName",
+                "sn",
+                "identity",
+                "inBytesRate",
+                "inQosPolicy",
+                "outQosPolicy",
+                "sessionId",
                 "framedIp",
+                "hostname",
                 "virtualAccessIntName",
                 "outPktsRate",
+                "state",
+                "localIntName",
                 "outIntName",
-                "outQosPolicy",
-                "hostname",
-                "inBytesRate",
-                "sessionId",
                 "isStaticRoute",
-                "localIntName",
-                "inQosPolicy",
-                "state",
-                "sn",
-                "identity",
-                "siteName",
+                "id",
                 "outBytesRate",
-                "pppMaxPayload"
+                "pppMaxPayload",
+                "inPktsRate"
             ],
             "description": "Point-to-Point Protocol over Ethernet (PPPoE) interface sessions inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PPPoE sessions",
             "ui_columns": [
                 "hostname",
@@ -6426,28 +6464,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/all",
             "api_scope_id": "12d83131919fbbe887dac1acf741631ff44212d1",
             "columns": [
+                "snmpTrap",
                 "unit",
-                "currentTraffic",
+                "changes",
                 "siteName",
-                "lowerLimit",
+                "sn",
                 "upperLimit",
                 "id",
-                "state",
-                "logUpperLimit",
-                "changes",
-                "sn",
+                "lowerLimit",
                 "action",
-                "snmpTrap",
+                "currentTraffic",
+                "intName",
                 "hostname",
-                "intName"
+                "logUpperLimit",
+                "state"
             ],
             "description": "Details for storm control traffic detection - all traffic",
             "method": "post",
             "nested_columns": [],
             "summary": "Storm Control - All Traffic",
             "ui_columns": [
                 "hostname",
@@ -6472,28 +6510,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/broadcast",
             "api_scope_id": "0dbe90d070c013fead0bb1d3eaf12f99fc657222",
             "columns": [
+                "snmpTrap",
                 "unit",
-                "currentTraffic",
+                "changes",
                 "siteName",
-                "lowerLimit",
+                "sn",
                 "upperLimit",
                 "id",
-                "state",
-                "logUpperLimit",
-                "changes",
-                "sn",
+                "lowerLimit",
                 "action",
-                "snmpTrap",
+                "currentTraffic",
+                "intName",
                 "hostname",
-                "intName"
+                "logUpperLimit",
+                "state"
             ],
             "description": "Details for storm control traffic detection - broadcast",
             "method": "post",
             "nested_columns": [],
             "summary": "Storm Control - Broadcast",
             "ui_columns": [
                 "hostname",
@@ -6518,28 +6556,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/multicast",
             "api_scope_id": "42ef5f9a374112076110e811e281e958a1bf2ae4",
             "columns": [
+                "snmpTrap",
                 "unit",
-                "currentTraffic",
+                "changes",
                 "siteName",
-                "lowerLimit",
+                "sn",
                 "upperLimit",
                 "id",
-                "state",
-                "logUpperLimit",
-                "changes",
-                "sn",
+                "lowerLimit",
                 "action",
-                "snmpTrap",
+                "currentTraffic",
+                "intName",
                 "hostname",
-                "intName"
+                "logUpperLimit",
+                "state"
             ],
             "description": "Details for storm control traffic detection - unicast",
             "method": "post",
             "nested_columns": [],
             "summary": "Storm Control - Unicast",
             "ui_columns": [
                 "hostname",
@@ -6564,28 +6602,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/unicast",
             "api_scope_id": "6b658b47f5b8a2fff8ed759a262a5ecb6c8890dc",
             "columns": [
+                "snmpTrap",
                 "unit",
-                "currentTraffic",
+                "changes",
                 "siteName",
-                "lowerLimit",
+                "sn",
                 "upperLimit",
                 "id",
-                "state",
-                "logUpperLimit",
-                "changes",
-                "sn",
+                "lowerLimit",
                 "action",
-                "snmpTrap",
+                "currentTraffic",
+                "intName",
                 "hostname",
-                "intName"
+                "logUpperLimit",
+                "state"
             ],
             "description": "Details for storm control traffic detection - multicast",
             "method": "post",
             "nested_columns": [],
             "summary": "Storm Control - Multicast",
             "ui_columns": [
                 "hostname",
@@ -6610,33 +6648,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/switchports",
             "api_scope_id": "db92291d321f3cd7dc8ed226810dd6769427b50c",
             "columns": [
-                "macCount",
                 "siteName",
-                "dscr",
-                "id",
-                "trunkVlan",
-                "dynamicMacCount",
-                "mode",
-                "devType",
-                "edge",
                 "sn",
+                "macCount",
+                "id",
                 "staticMacCount",
+                "edge",
+                "mode",
                 "voiceVlan",
-                "encap",
+                "intName",
+                "dscr",
                 "nativeVlan",
-                "accVlan",
                 "hostname",
-                "intName"
+                "accVlan",
+                "trunkVlan",
+                "devType",
+                "dynamicMacCount",
+                "encap"
             ],
-            "description": "Overview of all L2 Ethernet switchports",
+            "description": "Overview of all L2 Ethernet switchports in the network. Those are physical ports which extend the L2 segment(s) in thew switching domain.\n\nThis table includes the number of devices connected on each switchport as well",
             "method": "post",
             "nested_columns": [],
             "summary": "Interfaces Switchport",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -6663,21 +6701,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/errors",
             "api_scope_id": "828e3070cf04347f7f9fe3cd6679130c5b5e76df",
             "columns": [
                 "siteName",
-                "pn",
+                "sn",
                 "id",
+                "pn",
                 "errorLane",
-                "errorMessage",
-                "sn",
+                "intName",
                 "hostname",
-                "intName"
+                "errorMessage"
             ],
             "description": "Information oninterfaces transceivers errors messages and thresholds",
             "method": "post",
             "nested_columns": [],
             "summary": "Transceivers Errors",
             "ui_columns": [
                 "hostname",
@@ -6696,27 +6734,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/inventory",
             "api_scope_id": "b785b906c2aa75c8a6596ad065460cef328f46bd",
             "columns": [
+                "l1",
                 "tVendor",
-                "siteName",
-                "dscr",
-                "paramsList",
-                "pn",
-                "id",
                 "type",
-                "sn",
-                "l1",
                 "l2",
-                "tSn",
+                "siteName",
+                "sn",
+                "id",
+                "pn",
+                "intName",
+                "dscr",
                 "hostname",
-                "intName"
+                "paramsList",
+                "tSn"
             ],
             "description": "Interface transceivers inventory",
             "method": "post",
             "nested_columns": [
                 "paramsList"
             ],
             "summary": "Transceivers Inventory",
@@ -6742,38 +6780,38 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/statistics",
             "api_scope_id": "3f69d2448d97d72abb4298a0a11bfe678421fcc9",
             "columns": [
+                "model",
+                "type",
+                "siteName",
+                "sn",
+                "threshold",
+                "deltaValueHigh",
+                "dscr",
+                "value",
+                "thresholdHigh",
+                "family",
                 "unit",
-                "statistic",
                 "pn",
-                "type",
-                "id",
+                "deltaValueLow",
+                "lane",
                 "intName",
-                "vendor",
+                "hostname",
+                "laneOrigIntName",
                 "tVendor",
-                "family",
+                "statistic",
                 "platform",
                 "thresholdLow",
-                "laneOrigIntName",
-                "hostname",
                 "flag",
-                "dscr",
-                "threshold",
-                "sn",
-                "deltaValueLow",
-                "lane",
-                "model",
-                "siteName",
-                "deltaValueHigh",
-                "value",
-                "thresholdHigh"
+                "vendor",
+                "id"
             ],
             "description": "Interface transceivers statistics",
             "method": "post",
             "nested_columns": [],
             "summary": "Transceivers Statistics",
             "ui_columns": [
                 "hostname",
@@ -6807,25 +6845,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/thresholds",
             "api_scope_id": "a40e0396c0197d37f2ba1592a045d2cfaa341e22",
             "columns": [
-                "lane",
-                "siteName",
-                "pn",
                 "type",
+                "siteName",
+                "sn",
                 "id",
-                "level",
+                "pn",
                 "name",
-                "sn",
-                "hostname",
+                "lane",
+                "intName",
                 "flag",
-                "intName"
+                "level",
+                "hostname"
             ],
             "description": "Interface transceivers triggered thresholds",
             "method": "post",
             "nested_columns": [],
             "summary": "Transceivers Triggered Thresholds",
             "ui_columns": [
                 "hostname",
@@ -6848,23 +6886,23 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/bidirectional",
             "api_scope_id": "83e4917aaf74ad60f01d76d4cbd9929745362bfa",
             "columns": [
                 "pktsRate",
-                "bcastRate",
-                "bytesRate",
-                "mcastRate",
                 "siteName",
-                "id",
                 "sn",
+                "id",
                 "impactLoss",
+                "bytesRate",
+                "intName",
+                "mcastRate",
                 "hostname",
-                "intName"
+                "bcastRate"
             ],
             "description": "Bidirectional interface rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Bidirectional Interface Rates",
             "ui_columns": [
                 "hostname",
@@ -6886,22 +6924,22 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/bidirectional-device",
             "api_scope_id": "81f2c4d4e770942f7d338ea7da98c3ee9824fd06",
             "columns": [
                 "pktsRate",
-                "bcastRate",
-                "bytesRate",
-                "mcastRate",
                 "siteName",
-                "id",
                 "sn",
+                "id",
                 "impactLoss",
-                "hostname"
+                "bytesRate",
+                "mcastRate",
+                "hostname",
+                "bcastRate"
             ],
             "description": "Per-Device bidirectional transfer rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Bidirectional Transfer Rates",
             "ui_columns": [
                 "hostname",
@@ -6921,24 +6959,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/inbound",
             "api_scope_id": "cb0492b17a9d7fedb5c3a3aace3f40694e6f6da3",
             "columns": [
+                "inImpactLoss",
                 "inBcastRate",
                 "siteName",
-                "id",
-                "inImpactLoss",
                 "sn",
+                "id",
                 "inPktsRate",
-                "intName",
-                "hostname",
+                "inMcastRate",
                 "inBytesRate",
-                "inMcastRate"
+                "intName",
+                "hostname"
             ],
             "description": "Inbound interface rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Inbound Interface Transfer Rates",
             "ui_columns": [
                 "hostname",
@@ -6959,23 +6997,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/inbound-device",
             "api_scope_id": "709b279b23ba8bafda8aefa88da761970434ef0a",
             "columns": [
+                "inImpactLoss",
                 "inBcastRate",
                 "siteName",
-                "id",
-                "inImpactLoss",
                 "sn",
+                "id",
                 "inPktsRate",
-                "hostname",
+                "inMcastRate",
                 "inBytesRate",
-                "inMcastRate"
+                "hostname"
             ],
             "description": "Per-Device inbound interface transfer rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Inbound Interface Transfer Rates",
             "ui_columns": [
                 "hostname",
@@ -6995,24 +7033,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/outbound",
             "api_scope_id": "6b1c68eeee092c5497798689c7e6b07ff5c11e07",
             "columns": [
-                "outMcastRate",
+                "outBcastRate",
                 "siteName",
-                "outPktsRate",
+                "sn",
                 "id",
                 "outBytesRate",
-                "outBcastRate",
                 "outImpactLoss",
-                "sn",
+                "outMcastRate",
+                "intName",
                 "hostname",
-                "intName"
+                "outPktsRate"
             ],
             "description": "Outbound interface rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Outbound Interface Transfer Rates",
             "ui_columns": [
                 "hostname",
@@ -7033,23 +7071,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/outbound-device",
             "api_scope_id": "9b50ccd8960c187487f69d88019f07d791a3c330",
             "columns": [
-                "outMcastRate",
+                "outBcastRate",
                 "siteName",
-                "outPktsRate",
+                "sn",
                 "id",
                 "outBytesRate",
-                "outBcastRate",
                 "outImpactLoss",
-                "sn",
-                "hostname"
+                "outMcastRate",
+                "hostname",
+                "outPktsRate"
             ],
             "description": "Per-Device outbound interface transfer rates and cumulative loss impact",
             "method": "post",
             "nested_columns": [],
             "summary": "Per-Device Outbound Interface Transfer Rates",
             "ui_columns": [
                 "hostname",
@@ -7069,26 +7107,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/tunnels/ipv4",
             "api_scope_id": "9fe34a5d8c4ba0fc884a4d2f9d997b00c0eaf807",
             "columns": [
-                "tunnelSrcIntName",
-                "tunnelVrf",
-                "siteName",
-                "id",
                 "tunnelProto",
+                "siteName",
                 "sn",
-                "ipAddresses",
-                "tunnelDstIp",
-                "vrf",
-                "hostname",
+                "id",
+                "tunnelVrf",
                 "intName",
-                "tunnelSrcIp"
+                "tunnelSrcIp",
+                "hostname",
+                "vrf",
+                "tunnelDstIp",
+                "tunnelSrcIntName",
+                "ipAddresses"
             ],
             "description": "IPv4 Tunnels inventory",
             "method": "post",
             "nested_columns": [
                 "ipAddresses"
             ],
             "summary": "IPv4 Tunnels",
@@ -7113,26 +7151,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/interfaces/tunnels/ipv6",
             "api_scope_id": "d8ca81b4bcae5a87466caf73f6a51e3567bfa426",
             "columns": [
-                "tunnelDstIpv6",
-                "tunnelSrcIntName",
-                "tunnelVrf",
+                "tunnelProto",
                 "siteName",
-                "ipv6Addresses",
+                "sn",
                 "id",
-                "tunnelProto",
                 "tunnelSrcIpv6",
-                "sn",
-                "vrf",
+                "tunnelVrf",
+                "intName",
                 "hostname",
-                "intName"
+                "tunnelDstIpv6",
+                "ipv6Addresses",
+                "vrf",
+                "tunnelSrcIntName"
             ],
             "description": "IPv6 Tunnels inventory",
             "method": "post",
             "nested_columns": [
                 "ipv6Addresses"
             ],
             "summary": "IPv6 Tunnels",
@@ -7157,49 +7195,49 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/devices",
             "api_scope_id": "c701b81c3a91ebd953f0097a2fa520507745243f",
             "columns": [
-                "slug",
-                "icon",
-                "id",
-                "taskKey",
-                "uptime",
+                "hostnameProcessed",
+                "model",
+                "siteName",
+                "sn",
+                "loginType",
+                "objectId",
+                "hostnameOriginal",
                 "processor",
-                "version",
+                "mac",
                 "memoryTotalBytes",
-                "vendor",
+                "memoryUtilization",
+                "fqdn",
                 "family",
-                "platform",
+                "configReg",
+                "slug",
+                "hostname",
+                "loginPort",
                 "snHw",
-                "memoryUsedBytes",
-                "loginIp",
-                "fqdn",
+                "platform",
+                "devType",
+                "rd",
                 "stpDomain",
+                "vendor",
                 "domain",
-                "hostname",
+                "id",
+                "icon",
+                "loginIp",
+                "version",
                 "image",
-                "hostnameOriginal",
-                "reload",
-                "sn",
-                "memoryUtilization",
-                "hostnameProcessed",
-                "loginPort",
-                "model",
-                "siteName",
-                "objectId",
-                "rd",
-                "devType",
-                "loginType",
-                "mac",
-                "configReg"
+                "memoryUsedBytes",
+                "uptime",
+                "taskKey",
+                "reload"
             ],
-            "description": "Inventory of all logical or physical managed network infrastructure devices discovered",
+            "description": "Inventory of all logical managed network infrastructure devices that have been discovered and analyzed.\n\nThis table can be used for (but it is not limited to):\n\n* Verifying of the vendors and platforms of the network devices\n* Verifying of the operating system versions and images\n* Verifying if the boot settings (config register) are applied correctly\n* Verifying if the devices are stable and being rebooted often\n* Serial number and management IP address overview\n* Adherence to naming conventions (for device hostnames)",
             "method": "post",
             "nested_columns": [],
             "summary": "Device Inventory",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "rd",
@@ -7239,29 +7277,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/discovery-history",
             "api_scope_id": "80270bc86b703bca1062673a80977e7e80ac05a9",
             "columns": [
+                "sn",
+                "siteName",
                 "id",
-                "usernameNotes",
                 "loginIp",
-                "sn",
                 "loginType",
-                "ts",
                 "hostname",
-                "username"
+                "ts",
+                "username",
+                "usernameNotes"
             ],
             "description": "This view shows all discovered devices in history (no matter which snapshot is selected). IP Fabric will remember used protocol and last successful credential. These informations are preferred in the next discovery run.",
             "method": "post",
             "nested_columns": [],
             "summary": "Discovery History",
             "ui_columns": [
                 "hostname",
+                "siteName",
                 "loginIp",
                 "loginType",
                 "sn",
                 "ts",
                 "username",
                 "usernameNotes"
             ],
@@ -7274,26 +7314,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/fans",
             "api_scope_id": "512962c963edf9758d1dfef99eb4e90fdf23ad8a",
             "columns": [
-                "deviceId",
+                "fanPid",
                 "siteName",
-                "fanId",
-                "fanState",
-                "id",
                 "sn",
-                "fanName",
+                "id",
+                "fanState",
+                "fanSn",
+                "fanId",
+                "deviceId",
                 "hostname",
-                "fanPid",
-                "fanSn"
+                "fanName"
             ],
-            "description": "Fans detected in all network devices and their current state",
+            "description": "This table shows all fans found in all network devices and their current state.\n\nProper cooling is very important for almost all network devices as they produce heat by transporting data. Fan failure can cause overheating of the\ndevice and thus device outage (or permanent heat damage).\\\nDesired state is &quot;ok&quot;, &quot;normal&quot; etc.",
             "method": "post",
             "nested_columns": [],
             "summary": "Environment - Fans",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "deviceId",
@@ -7312,44 +7352,45 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/interfaces",
             "api_scope_id": "fa462e10f3ff2a756fce2f862d6e08d913113cfd",
             "columns": [
-                "slug",
-                "speedValue",
-                "id",
-                "nameOriginal",
-                "intName",
-                "transceiverPn",
-                "loginIp",
-                "l1",
+                "intNameAlias",
                 "l2",
-                "rel",
-                "hostname",
-                "transceiverType",
-                "speed",
-                "duplex",
+                "siteName",
+                "sn",
+                "hasTransceiver",
+                "loginType",
                 "dscr",
                 "primaryIp",
+                "mac",
+                "transceiverType",
                 "mtu",
-                "transceiverSn",
-                "intNameAlias",
-                "sn",
-                "hasTransceiver",
-                "siteName",
+                "bandwidth",
+                "reason",
+                "slug",
+                "intName",
+                "hostname",
+                "speedValue",
                 "media",
+                "l1",
                 "speedType",
-                "loginType",
-                "reason",
-                "mac",
-                "errDisabled"
+                "transceiverSn",
+                "transceiverPn",
+                "speed",
+                "rel",
+                "errDisabled",
+                "nameOriginal",
+                "id",
+                "loginIp",
+                "duplex"
             ],
-            "description": "Information on every detected physical or logical interface for all discovered devices",
+            "description": "Interface Inventory table represents information about every discovered interface in the network, including the state information as observed during the last analysis.",
             "method": "post",
             "nested_columns": [],
             "summary": "Interface Inventory",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "intNameAlias",
@@ -7358,14 +7399,15 @@
                 "l1",
                 "l2",
                 "reason",
                 "dscr",
                 "mac",
                 "duplex",
                 "speed",
+                "bandwidth",
                 "speedValue",
                 "speedType",
                 "media",
                 "errDisabled",
                 "mtu",
                 "primaryIp",
                 "hasTransceiver",
@@ -7383,24 +7425,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/modules",
             "api_scope_id": "d4769862d55464e1b9fdb16103a9f5432de432a6",
             "columns": [
-                "deviceId",
                 "modulePid",
                 "siteName",
-                "id",
                 "moduleState",
                 "sn",
-                "moduleId",
-                "hostname"
+                "id",
+                "deviceId",
+                "hostname",
+                "moduleId"
             ],
-            "description": "Information about every detected modules and their current the state",
+            "description": "This table shows all modules found in all network devices and their current state.\n\nSome network devices chassis are modular and can hold multiple expansion modules (or linecards) in the basic device chassis. Expansion module can\nbring more processing power, new functions or additional network interfaces.\\\nUsually there is multiple free positions (called slots) in the modular chassis. Basic chassis can work without the expansion modules, but the module\nitself cannot work without the basic chassis.",
             "method": "post",
             "nested_columns": [],
             "summary": "Environment - Modules",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "deviceId",
@@ -7417,29 +7459,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/phones",
             "api_scope_id": "adc2e1502c234d6ba717a50e15cb0d06d5853e1a",
             "columns": [
-                "phoneInt",
+                "userIp",
+                "phoneName",
+                "vendor",
                 "siteName",
-                "switchInt",
-                "switchSn",
+                "switchHostname",
                 "id",
+                "switchInt",
+                "phoneMac",
                 "voiceVlan",
-                "userMac",
                 "phoneIp",
-                "phoneMac",
-                "phoneName",
-                "vendor",
-                "switchHostname",
-                "userIp"
+                "phoneInt",
+                "switchSn",
+                "userMac"
             ],
-            "description": "Inventory of all detected IP phones and endpoints connected to them",
+            "description": "Table shows all discovered IP phones and endpoints connected to them. Switch interface column shows where the phone is connected in the network. If a switchport has voice VLAN configured, it is noted in the Voice VLAN column.\n\nFurther investigation would be suitable for following results:\n* If the phone is connected to correct port (may indicate unauthorized cabling change by the end user)\n* If the IP address and VLAN assignment for phone/endpoint is as expected (may indicate VLAN mismatch or DHCP problems)\n* If multiple endpoints are connected (may indicate unauthorized endpoints connected to network)\n* Only one switch (or low number of switches) connecting the IP phones (may indicate high availability problem)",
             "method": "post",
             "nested_columns": [],
             "summary": "IP Phones and Connected Devices",
             "ui_columns": [
                 "phoneIp",
                 "phoneName",
                 "phoneMac",
@@ -7462,26 +7504,26 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/pn",
             "api_scope_id": "efd238e0d15b04ad415446efaca80939e4186f72",
             "columns": [
                 "deviceSn",
-                "deviceId",
                 "model",
+                "vendor",
                 "siteName",
-                "dscr",
+                "sn",
                 "platform",
                 "id",
-                "name",
-                "sn",
-                "pid",
                 "vid",
+                "name",
+                "dscr",
+                "deviceId",
                 "hostname",
-                "vendor"
+                "pid"
             ],
             "description": "Modules and part numbers from inventory of network infrastructure devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Modules and Part Numbers Inventory",
             "ui_columns": [
                 "hostname",
@@ -7505,29 +7547,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/power-supplies",
             "api_scope_id": "8ccd4c725aefc8efa41dd74685da5711b3e550e2",
             "columns": [
-                "deviceId",
                 "model",
-                "pwSupplyId",
-                "pwSupplyName",
                 "siteName",
-                "pwSupplyPid",
-                "id",
-                "pwSupplyState",
                 "sn",
+                "pwSupplyId",
+                "id",
+                "pwSupplyName",
+                "pwSupplySn",
                 "pwSupplyType",
+                "pwSupplyState",
+                "pwSupplyPid",
                 "pwSupplyCircuit",
-                "hostname",
-                "pwSupplySn"
+                "deviceId",
+                "hostname"
             ],
-            "description": "Power supplies detected in all network devices and their current state",
+            "description": "This table shows all power supplies found in all network devices and their current state.\n\nDual power input is desired for most of the network devices to overcome power outage of one power feed line or one power supply failure. To check if\ndual power input is working on all devices, quick overview table can be very helpful.",
             "method": "post",
             "nested_columns": [],
             "summary": "Environment - Power Supplies",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "deviceId",
@@ -7549,26 +7591,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/power-supplies-fans",
             "api_scope_id": "8fd8461fcc4364f29bc852f9dd78ac6b30b1314d",
             "columns": [
-                "deviceId",
+                "fanVendor",
                 "siteName",
-                "fanId",
-                "fanState",
-                "id",
                 "sn",
-                "fanVendor",
-                "fanName",
+                "id",
+                "fanState",
+                "fanSn",
+                "fanId",
+                "deviceId",
                 "hostname",
-                "fanSn"
+                "fanName"
             ],
-            "description": "Power supplies fans detected in all network devices and their current state",
+            "description": "This table shows all fans on power supplies found in all network devices and their current state.\n\nFaulty fan on power supply can cause bad heat dissipation and subsequently can be the cause of the power supply itself",
             "method": "post",
             "nested_columns": [],
             "summary": "Environment - Power Supplies Fans",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "deviceId",
@@ -7587,28 +7629,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/sites",
             "api_scope_id": "a067b848a10f9ef2989c1fcb058982213cb56167",
             "columns": [
-                "routersCount",
-                "devicesCount",
+                "usersCount",
+                "switchesCount",
                 "rDCount",
+                "rDomains",
                 "siteName",
-                "switchesCount",
                 "id",
                 "stpDCount",
-                "vlanCount",
                 "stpDomains",
-                "rDomains",
+                "routersCount",
                 "networksCount",
-                "usersCount"
+                "devicesCount",
+                "vlanCount"
             ],
-            "description": "Sites inventory defined by site separation rules or attributes",
+            "description": "Sites are automatically calculated based on the administrative domain boundaries, such as carrier networks and other unmanaged infrastructure. A single unmanaged traceroute hop is not considered a site boundary, and unmanaged infrastructure is reconstructed from the probes.",
             "method": "post",
             "nested_columns": [],
             "summary": "Sites Inventory",
             "ui_columns": [
                 "siteName",
                 "devicesCount",
                 "usersCount",
@@ -7628,22 +7670,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/families",
             "api_scope_id": "023573d36598f61c617939f256d986e21d878915",
             "columns": [
-                "modelsCount",
-                "platformsCount",
-                "devicesCount",
                 "family",
+                "vendor",
+                "modelsCount",
                 "id",
-                "vendor"
+                "devicesCount",
+                "platformsCount"
             ],
-            "description": "Inventory covering vendor - families distribution",
+            "description": "This table represent Vendor / Family overview in the whole network",
             "method": "post",
             "nested_columns": [],
             "summary": "Vendor Families Overview",
             "ui_columns": [
                 "vendor",
                 "family",
                 "platformsCount",
@@ -7659,22 +7701,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/models",
             "api_scope_id": "feb805028154b351a6397fd18d468eba808d37ca",
             "columns": [
-                "devicesCount",
                 "family",
                 "model",
+                "vendor",
                 "platform",
                 "id",
-                "vendor"
+                "devicesCount"
             ],
-            "description": "Inventory covering vendor - families - platforms - models distribution",
+            "description": "This table represent Vendor / Family / Platform / Model overview in the whole network",
             "method": "post",
             "nested_columns": [],
             "summary": "Vendor Models Overview",
             "ui_columns": [
                 "vendor",
                 "family",
                 "platform",
@@ -7690,22 +7732,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/platforms",
             "api_scope_id": "062b8c7e2a3e2323c7b7c71542b6566ae4851697",
             "columns": [
-                "modelsCount",
-                "devicesCount",
                 "family",
+                "vendor",
+                "modelsCount",
                 "platform",
                 "id",
-                "vendor"
+                "devicesCount"
             ],
-            "description": "Inventory covering vendor - families - platforms distribution",
+            "description": "This table represent Vendor / Family / Platform overview in the whole network",
             "method": "post",
             "nested_columns": [],
             "summary": "Vendor Platforms Overview",
             "ui_columns": [
                 "vendor",
                 "family",
                 "platform",
@@ -7721,22 +7763,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/vendors",
             "api_scope_id": "3aed3be2e793d01ef760cab3dc683ccbc2c95be7",
             "columns": [
+                "vendor",
                 "modelsCount",
-                "platformsCount",
-                "devicesCount",
                 "id",
-                "vendor",
-                "familiesCount"
+                "familiesCount",
+                "devicesCount",
+                "platformsCount"
             ],
-            "description": "Inventory covering vendor distribution",
+            "description": "This table represent Vendor overview in the whole network",
             "method": "post",
             "nested_columns": [],
             "summary": "Vendors Overview",
             "ui_columns": [
                 "vendor",
                 "familiesCount",
                 "platformsCount",
@@ -7752,23 +7794,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/inventory/temperature-sensors",
             "api_scope_id": "c05978e6cb1a054093bec04f7c99a0c4a7b746e1",
             "columns": [
-                "deviceId",
                 "model",
                 "siteName",
-                "thermalId",
-                "id",
                 "sn",
-                "thermalState",
+                "id",
+                "thermalDescription",
+                "thermalId",
+                "deviceId",
                 "hostname",
-                "thermalDescription"
+                "thermalState"
             ],
             "description": "Status of temperature sensors",
             "method": "post",
             "nested_columns": [],
             "summary": "Environment - Temperature sensors",
             "ui_columns": [
                 "hostname",
@@ -7788,23 +7830,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/jobs",
             "api_scope_id": "5fd6f107524d27bc33de517ed329cbe6708ff06b",
             "columns": [
-                "status",
-                "finishedAt",
-                "isDone",
                 "id",
-                "startedAt",
                 "name",
                 "scheduledAt",
-                "username",
+                "isDone",
+                "finishedAt",
                 "snapshot",
+                "startedAt",
+                "status",
+                "username",
                 "downloadFile"
             ],
             "description": "IP Fabric scheduled or running jobs",
             "method": "post",
             "nested_columns": [],
             "summary": "Platform Jobs",
             "ui_columns": [
@@ -7829,21 +7871,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/load-balancing/f5-partitions",
             "api_scope_id": "7b06a1adb684d5d9817314e5cbb000a7ac3321e2",
             "columns": [
                 "siteName",
+                "sn",
                 "id",
-                "partitionName",
+                "hostname",
                 "partitionDescription",
-                "sn",
-                "hostname"
+                "partitionName"
             ],
-            "description": "F5 Partitions inventory",
+            "description": "List of F5 Partitions inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "F5 Partitions",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "partitionName",
@@ -7858,34 +7900,34 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/load-balancing/virtual-servers",
             "api_scope_id": "e9022c4ef969209a382862d4e53405880dbce711",
             "columns": [
-                "id",
-                "clientProfile",
-                "pools",
-                "protocolNumber",
-                "protocolName",
-                "portName",
-                "poolsCount",
-                "availability",
-                "hostname",
-                "vip",
-                "vrf",
                 "partition",
-                "state",
+                "siteName",
                 "sn",
+                "pools",
                 "sourceNat",
-                "portNumber",
-                "siteName",
+                "vrf",
                 "reason",
+                "hostname",
+                "protocolNumber",
+                "state",
+                "clientProfile",
+                "portName",
+                "protocolName",
+                "availability",
+                "poolsCount",
+                "virtualServerName",
+                "id",
                 "vip6",
-                "virtualServerName"
+                "vip",
+                "portNumber"
             ],
             "description": "Load balancing - virtual servers inventory",
             "method": "post",
             "nested_columns": [
                 "pools",
                 "vip",
                 "vip6"
@@ -7921,25 +7963,25 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/load-balancing/virtual-servers/pool-members",
             "api_scope_id": "b9a7e96661b01e097932614a33ca90a4da636eb3",
             "columns": [
                 "memberIpV6",
-                "siteName",
+                "poolName",
                 "port",
                 "id",
-                "state",
-                "poolName",
-                "memberIp",
+                "siteName",
                 "sn",
                 "availability",
-                "vrf",
                 "hostname",
-                "poolMemberName"
+                "vrf",
+                "memberIp",
+                "poolMemberName",
+                "state"
             ],
             "description": "Load balancing - virtual servers and pool members inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Virtual Servers - Pool members",
             "ui_columns": [
                 "hostname",
@@ -7962,21 +8004,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/load-balancing/virtual-servers/pools",
             "api_scope_id": "eacbfd8381e770faf6382444d34f45956921d0e0",
             "columns": [
+                "members",
+                "poolName",
                 "siteName",
+                "sn",
                 "id",
                 "membersCount",
-                "sn",
-                "hostname",
-                "poolName",
-                "members"
+                "hostname"
             ],
             "description": "Load balancing - virtual servers and pools inventory",
             "method": "post",
             "nested_columns": [
                 "members"
             ],
             "summary": "Virtual Servers - Pools",
@@ -7996,18 +8038,18 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/banners/banners",
             "api_scope_id": "3b7234600756841ed802d76563f4484d92e4f3df",
             "columns": [
-                "siteName",
                 "type",
-                "id",
                 "sn",
+                "siteName",
+                "id",
                 "hostname",
                 "text"
             ],
             "description": "Types and texts of the device banners",
             "method": "post",
             "nested_columns": [],
             "summary": "Device Banners",
@@ -8026,19 +8068,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/banners/summary",
             "api_scope_id": "63b5a7e866e79d5ac1ec87c8f9d862bdece3ba57",
             "columns": [
-                "siteName",
-                "loginBanner",
-                "id",
                 "sn",
+                "siteName",
                 "motdBanner",
+                "id",
+                "loginBanner",
                 "hostname"
             ],
             "description": "Summary view for device banners",
             "method": "post",
             "nested_columns": [],
             "summary": "Banners Summary",
             "ui_columns": [
@@ -8056,25 +8098,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/changes/connectivity",
             "api_scope_id": "205a406d59d39c5b5c3c03c64dbe0ed2a1a6a4e1",
             "columns": [
+                "remoteHost",
                 "localMedia",
+                "remoteMedia",
+                "localHost",
                 "id",
                 "remoteInt",
-                "localInt",
-                "remoteHost",
-                "localHost",
-                "protocol",
                 "remoteSn",
-                "remoteMedia",
-                "localSn",
-                "status"
+                "status",
+                "protocol",
+                "localInt",
+                "localSn"
             ],
             "description": "Changes in connectivity matrix between selected snapshots",
             "method": "post",
             "nested_columns": [],
             "summary": "Changes in connectivity matrix",
             "ui_columns": [
                 "id",
@@ -8098,25 +8140,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/changes/devices",
             "api_scope_id": "bff34be4b27e5d76ec4a78857f2c7f0ca0b20530",
             "columns": [
-                "image",
+                "configReg",
+                "sn",
                 "id",
-                "uptime",
                 "loginIp",
-                "processor",
-                "reload",
                 "version",
-                "sn",
-                "configReg",
+                "status",
+                "image",
                 "hostname",
-                "status"
+                "uptime",
+                "processor",
+                "reload"
             ],
             "description": "Changes in discovered devices between selected snapshots",
             "method": "post",
             "nested_columns": [],
             "summary": "Changes in devices",
             "ui_columns": [
                 "id",
@@ -8141,21 +8183,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/changes/managed-devs",
             "api_scope_id": "74bfe2920e6c6ba589df4951acb573654641dcaa",
             "columns": [
                 "type",
+                "sn",
                 "id",
+                "status",
                 "net",
-                "sn",
-                "intName",
-                "hostname",
                 "ip",
-                "status"
+                "intName",
+                "hostname"
             ],
             "description": "Changes in managed interface IP addresses between selected snapshots",
             "method": "post",
             "nested_columns": [],
             "summary": "Changes in Managed IP",
             "ui_columns": [
                 "id",
@@ -8176,23 +8218,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/changes/pn",
             "api_scope_id": "9449202b14ae1a0fea9fb19f82ac83682fe537e9",
             "columns": [
-                "deviceId",
-                "dscr",
+                "vid",
+                "sn",
                 "id",
                 "name",
-                "sn",
-                "pid",
-                "vid",
+                "status",
+                "dscr",
+                "deviceId",
                 "hostname",
-                "status"
+                "pid"
             ],
             "description": "Changes in part numbers between selected snapshots",
             "method": "post",
             "nested_columns": [],
             "summary": "Changes in Part Numbers",
             "ui_columns": [
                 "id",
@@ -8215,21 +8257,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/configuration",
             "api_scope_id": "e5cac6dcf2d741c053f58fbcda2b0d3f88dbf4a2",
             "columns": [
                 "hash",
-                "id",
-                "lastChangeAt",
                 "sn",
-                "lastCheckAt",
                 "reason",
+                "lastChangeAt",
+                "id",
+                "status",
                 "hostname",
-                "status"
+                "lastCheckAt"
             ],
             "description": "Inventory of all captured configuration files",
             "method": "post",
             "nested_columns": [],
             "summary": "Configuration Files",
             "ui_columns": [
                 "id",
@@ -8304,26 +8346,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/configuration/saved",
             "api_scope_id": "953130708a830c65095c48804e9c0fc647964b3e",
             "columns": [
+                "sn",
                 "siteName",
-                "startupConfigExists",
-                "blobKey",
+                "currentConfigExists",
                 "id",
-                "uptime",
                 "loginIp",
-                "sn",
+                "startupConfigExists",
+                "status",
+                "blobKey",
                 "hostname",
-                "currentConfigExists",
-                "status"
+                "uptime"
             ],
-            "description": "Compare the current and startup configuration files",
+            "description": "Saved configuration consistency table shows the status if the actual \"current\" configuration matches the saved \"startup\" configuration that will be applied when the device reboots.\\\nWith the expection of testing and the period of planned changes, \"current\" configuration should match \"startup\" at all times to ensure consistency in network behaviour after reboot.\\\nDesired state is \"saved\". When the configuraton state is changed, it should be saved on nearest ocassion.\n\n---\n\nWithin the IP FABRIC tool, the differences between the \"current\" and \"startup\" configuration can be shown after clicking on the button \"Difference\". Three types of comparison output are possible:\n* \"Inline diff\" - in the diff format (the changes only, unchanged lines are not shown)\n* \"Side by side\" - in the dual column text output. Startup config is in the left column, current config is in the right column.\n* \"Inline\" - in the diff format while the unchanged lines are shown\n\nColor coding is as follows:\n\n* Green color shows added lines\n* Red color shows deleted lines\n* Black+white shows unchanged lines",
             "method": "post",
             "nested_columns": [],
             "summary": "Saved Config Consistency",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "uptime",
@@ -8339,21 +8381,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/connectivity-errors",
             "api_scope_id": "8ff0b8fbbd918cc544206aa0d4b4feaecf1cc544",
             "columns": [
+                "id",
                 "telnetType",
                 "sshType",
-                "id",
-                "date",
-                "telnetMsg",
                 "ip",
-                "sshMsg"
+                "sshMsg",
+                "date",
+                "telnetMsg"
             ],
             "description": "Observe connectivity errors for failed configuration file downloads",
             "method": "post",
             "nested_columns": [],
             "summary": "Configuration Management Connectivity Errors",
             "ui_columns": [
                 "id",
@@ -8373,28 +8415,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/discovery-runs",
             "api_scope_id": "ad7a1cd54273549505a722cfd794af4cbc33dcfe",
             "columns": [
-                "status",
-                "interfaceActiveCount",
+                "connectionCount",
                 "tsChange",
-                "tsEnd",
+                "deviceCount",
                 "id",
-                "isLastSnapshot",
                 "interfaceEdgeCount",
-                "userCount",
-                "tsStart",
-                "connectionCount",
+                "managedIpCount",
                 "interfaceCount",
+                "status",
+                "isLastSnapshot",
+                "tsEnd",
+                "userCount",
                 "partNumbersCount",
-                "deviceCount",
-                "managedIpCount"
+                "interfaceActiveCount",
+                "tsStart"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "Changes",
             "ui_columns": [
                 "id",
@@ -8421,25 +8463,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/dns/servers",
             "api_scope_id": "f84fc1283440f332105f9414add605617ab09366",
             "columns": [
-                "siteName",
+                "parentId",
                 "type",
+                "searchDomains",
+                "siteName",
+                "sn",
                 "id",
                 "ipv6",
-                "sn",
                 "srcIntName",
-                "searchDomains",
-                "vrf",
-                "hostname",
                 "ip",
-                "parentId"
+                "hostname",
+                "vrf"
             ],
             "description": "Inventory of configured DNS servers on managed network devices",
             "method": "post",
             "nested_columns": [
                 "searchDomains"
             ],
             "summary": "DNS Servers",
@@ -8462,21 +8504,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/dns/settings",
             "api_scope_id": "1d4366f0342d43cc41c8dc28a22a1c300d4c4d05",
             "columns": [
-                "siteName",
-                "id",
-                "timeout",
                 "retry",
                 "dnsServersCount",
-                "sn",
                 "protocols",
+                "timeout",
+                "siteName",
+                "sn",
+                "id",
                 "hostname"
             ],
             "description": "Inventory of additional DNS settings on managed network devices",
             "method": "post",
             "nested_columns": [
                 "protocols"
             ],
@@ -8498,25 +8540,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/netflow/collectors",
             "api_scope_id": "66a23028ec74211250e2fe8df9e612c509babd3b",
             "columns": [
+                "srcAddress",
                 "siteName",
                 "port",
-                "collector",
-                "srcInterface",
+                "sn",
                 "id",
+                "srcInterface",
                 "version",
                 "protocol",
-                "sn",
-                "vrf",
                 "hostname",
-                "srcAddress"
+                "collector",
+                "vrf"
             ],
             "description": "Inventory of NetFlow collectors configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "NetFlow Collectors",
             "ui_columns": [
                 "hostname",
@@ -8538,24 +8580,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/netflow/devices",
             "api_scope_id": "3032ab06eb03a1554de2df293f6a22fd607959ff",
             "columns": [
-                "inactiveTimeout",
+                "countNetflowInterfaces",
                 "siteName",
-                "countNetflowCollectors",
-                "id",
                 "sn",
+                "id",
                 "activeTimeout",
-                "countNetflowInterfaces",
-                "hostname"
+                "inactiveTimeout",
+                "hostname",
+                "countNetflowCollectors"
             ],
-            "description": "Managed network devices with configured NetFlow collectors",
+            "description": "Overview of devices capturing and exporting flow data and associated global parameters",
             "method": "post",
             "nested_columns": [],
             "summary": "NetFlow Devices",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "countNetflowCollectors",
@@ -8572,19 +8614,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/netflow/interfaces",
             "api_scope_id": "480c1176444e47070d4a1cb5a067b19c5a994976",
             "columns": [
+                "interface",
                 "siteName",
-                "directions",
-                "id",
                 "sn",
-                "interface",
+                "id",
+                "directions",
                 "hostname"
             ],
             "description": "Inventory of interfaces participating in NetFlow collection",
             "method": "post",
             "nested_columns": [
                 "directions"
             ],
@@ -8604,22 +8646,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/overview",
             "api_scope_id": "71c12b11bddc390ec742bb6427ff1ab1638be831",
             "columns": [
-                "siteName",
+                "countNetflowInterfaces",
                 "countSflowCollectors",
-                "countNetflowCollectors",
-                "id",
+                "siteName",
                 "sn",
-                "countNetflowInterfaces",
+                "id",
                 "hostname",
-                "countSflowSources"
+                "countSflowSources",
+                "countNetflowCollectors"
             ],
             "description": "Summary inventory of devices participating in either NetFlow or sFlow collection",
             "method": "post",
             "nested_columns": [],
             "summary": "Flow Overview",
             "ui_columns": [
                 "hostname",
@@ -8640,19 +8682,19 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/sflow/collectors",
             "api_scope_id": "8a006a5d361cca0e0d7ad0fd66dd9949d5ca73b4",
             "columns": [
                 "siteName",
                 "port",
-                "collector",
-                "id",
                 "sn",
-                "vrf",
-                "hostname"
+                "id",
+                "hostname",
+                "collector",
+                "vrf"
             ],
             "description": "Inventory of sFlow collectors configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "sFlow Collectors",
             "ui_columns": [
                 "hostname",
@@ -8670,28 +8712,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/sflow/devices",
             "api_scope_id": "5f4dda4c06013f386007d2cff645bd3dc2abe783",
             "columns": [
+                "countSflowCollectors",
+                "srcAddress",
                 "ingressSampleRate",
                 "siteName",
-                "countSflowCollectors",
-                "id",
-                "agent",
                 "sn",
+                "id",
                 "egressSampleRate",
-                "pollingInterval",
                 "srcAddress6",
+                "agent",
                 "hostname",
                 "countSflowSources",
-                "srcAddress"
+                "pollingInterval"
             ],
-            "description": "Managed network devices with configured sFlow collectors",
+            "description": "Overview of devices capturing and exporting flow data and associated global parameters",
             "method": "post",
             "nested_columns": [],
             "summary": "sFlow Devices",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "countSflowCollectors",
@@ -8712,24 +8754,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/flow/sflow/sources",
             "api_scope_id": "fb837401d54309a07526cf56705b77604d8ba2c3",
             "columns": [
+                "type",
                 "ingressSampleRate",
                 "siteName",
-                "type",
-                "directions",
-                "id",
-                "name",
                 "sn",
+                "id",
                 "egressSampleRate",
-                "pollingInterval",
-                "hostname"
+                "directions",
+                "name",
+                "hostname",
+                "pollingInterval"
             ],
             "description": "Inventory of sources participating in sFlow collection",
             "method": "post",
             "nested_columns": [
                 "directions"
             ],
             "summary": "sFlow Data Sources",
@@ -8752,30 +8794,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses",
             "api_scope_id": "f786373f6201bef7901c1bf4dc314f5264a2b73c",
             "columns": [
+                "licenseActive",
+                "licenseEvalPeriodTotal",
                 "licenseName",
-                "index",
-                "licenseType",
-                "reservationStatus",
                 "siteName",
-                "licenseEvalPeriodTotal",
+                "sn",
+                "licenseCount",
                 "id",
                 "licenseInUse",
-                "licenseActive",
                 "numberOfDetails",
-                "sn",
                 "licensePeriodLeft",
-                "licenseCount",
+                "index",
+                "status",
+                "licenseType",
+                "reservationStatus",
                 "hostname",
-                "description",
-                "status"
+                "description"
             ],
             "description": "Licenses inventory for managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed Licenses",
             "ui_columns": [
                 "hostname",
@@ -8804,21 +8846,21 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses/cisco-smart-licenses/authorization",
             "api_scope_id": "917f80405318bb3e6b96e276670243646b73c25a",
             "columns": [
                 "lastCommunicationTime",
                 "siteName",
+                "sn",
                 "id",
                 "authorizationTime",
-                "communicationDeadlineTime",
-                "sn",
-                "hostname",
                 "lastCommunicationStatus",
-                "status"
+                "status",
+                "hostname",
+                "communicationDeadlineTime"
             ],
             "description": "Cisco smart license authorization inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco Smart License Authorization",
             "ui_columns": [
                 "hostname",
@@ -8838,24 +8880,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses/cisco-smart-licenses/registration",
             "api_scope_id": "b85a242f2218df05186feff2ab82ff5a51e700c6",
             "columns": [
-                "initialRegistrationTime",
                 "siteName",
-                "initialRegistrationStatus",
-                "registrationExpires",
-                "id",
-                "virtualAccount",
                 "sn",
+                "id",
+                "registrationExpires",
+                "status",
+                "initialRegistrationTime",
                 "smartAccount",
                 "hostname",
-                "status"
+                "initialRegistrationStatus",
+                "virtualAccount"
             ],
             "description": "Cisco smart license registration inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco Smart License Registration",
             "ui_columns": [
                 "hostname",
@@ -8876,20 +8918,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses/cisco-smart-licenses/reservations",
             "api_scope_id": "cf34c0ca4fb85974d8f90f46fbef5c956a546749",
             "columns": [
-                "totalReservedCount",
-                "siteName",
                 "type",
+                "sn",
+                "siteName",
+                "totalReservedCount",
                 "id",
                 "name",
-                "sn",
                 "hostname"
             ],
             "description": "Cisco smart license reservations inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco Smart License Reservations",
             "ui_columns": [
@@ -8909,20 +8951,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses/detail",
             "api_scope_id": "797b10d2df5344b4b49eb5ffb62806a75ff69980",
             "columns": [
                 "siteName",
+                "sn",
                 "id",
+                "license",
                 "name",
-                "detail",
-                "sn",
                 "hostname",
-                "license"
+                "detail"
             ],
             "description": "Licenses detailed inventory for managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed License detail",
             "ui_columns": [
                 "hostname",
@@ -8939,20 +8981,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/licenses/summary",
             "api_scope_id": "56cd5ca1a301d8086eea37cf5b0f3f3f2a3079ab",
             "columns": [
-                "siteName",
                 "type",
-                "id",
                 "sn",
-                "hostname",
-                "numberOfLicenses"
+                "siteName",
+                "id",
+                "numberOfLicenses",
+                "hostname"
             ],
             "description": "Licenses summary inventory including license type and number of licenses",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed License Summary",
             "ui_columns": [
                 "hostname",
@@ -8969,20 +9011,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/logging/local",
             "api_scope_id": "29756ab38005275650d8e2ed736a749407f8a4f2",
             "columns": [
-                "siteName",
-                "type",
-                "id",
                 "fileName",
-                "sn",
+                "type",
+                "siteName",
                 "filters",
+                "sn",
+                "id",
                 "hostname"
             ],
             "description": "Local system message logging targets and associated parameters",
             "method": "post",
             "nested_columns": [
                 "filters"
             ],
@@ -9003,27 +9045,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/logging/remote",
             "api_scope_id": "5df3b4c4257934ea75d454e22f0227f5c3b2069f",
             "columns": [
-                "host",
+                "srcAddress",
+                "type",
                 "siteName",
+                "filters",
                 "port",
-                "srcInterface",
-                "type",
                 "id",
-                "facility",
-                "protocol",
                 "sn",
-                "filters",
-                "vrf",
+                "srcInterface",
+                "protocol",
                 "hostname",
-                "srcAddress"
+                "facility",
+                "vrf",
+                "host"
             ],
             "description": "Remote system message logging targets and associated parameters",
             "method": "post",
             "nested_columns": [
                 "filters"
             ],
             "summary": "Remote Logging Services",
@@ -9049,20 +9091,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/logging/summary",
             "api_scope_id": "5951a8aead84a9c584038cdf5df254a625d6c9ea",
             "columns": [
-                "countRemoteServices",
                 "siteName",
-                "id",
                 "sn",
+                "id",
                 "countLocalServices",
-                "hostname"
+                "hostname",
+                "countRemoteServices"
             ],
             "description": "Summary of the system message logging configuration for remote and local targets configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Logging Summary",
             "ui_columns": [
                 "hostname",
@@ -9079,31 +9121,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/ntp/sources",
             "api_scope_id": "8143afdb75d5e9a6723cbd4cc380555c2c944d74",
             "columns": [
+                "offset",
+                "reachable",
+                "reference",
+                "id",
                 "siteName",
-                "flags",
-                "delay",
+                "sn",
+                "when",
+                "source",
                 "reach",
-                "id",
+                "delay",
                 "stratum",
-                "source",
-                "sn",
-                "offset",
-                "jitter",
-                "poll",
-                "reference",
                 "hostname",
-                "reachable",
-                "when"
+                "jitter",
+                "flags",
+                "poll"
             ],
-            "description": "Detailed status of all NTP peerings configured on managed network devices",
+            "description": "This table describes detailed status of all NTP peerings in the network.\n\nReference:\n* IP address- The IP address of the remote peer or server.\n* .ACST.- NTP manycast server.\n* .AUTH.- Authentication error.\n* .AUTO.- Autokey sequence error.\n* .BCST.- NTP broadcast server.\n* .CRYPT.- Autokey protocol error\n* .DENY.- Access denied by server.\n* .INIT.- Peer association initialized.\n* .IRIG.- Inter Range Instrumentation Group time code.\n* .LOCL.- The local clock on the host.\n* .MCST.- NTP multicast server.\n* .RATE.- NTP polling rate exceeded.\n* .STEP.- NTP step time change. The offset is less than 1000 millisecends but more than 125 milliseconds.\n* .TIME.- NTP association timeout.\n\nReach: NTP event can be succesful (=binary 1) or unsuccessful (=binary 0). The last event is moved to the rigthmost bit of the \"Reach\" value and the other bits are shifted left. Maximum value is 377 octal = 255 decimal = last eight NTP events were successful. Lowest value si zero = all last 8 NTP events were not successful.\n\nFlags: Following values are possible for each configured NTP peering:\n* \\* selected for sync, selected for synchronization, selectedconfigured, master (synced)configured, sys.peerconfigured, system peerconfigured  - actual NTP server\n* = polled in client mode, mode is client - configured, but not used\n* x configured, unreachable - configured, but not reachable",
             "method": "post",
             "nested_columns": [
                 "flags"
             ],
             "summary": "NTP Sources",
             "ui_columns": [
                 "hostname",
@@ -9129,23 +9171,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/ntp/summary",
             "api_scope_id": "bd057398905b7d0a1f542a44b0d7808e3b2a5a45",
             "columns": [
-                "confSources",
-                "sources",
                 "siteName",
-                "id",
                 "sn",
+                "id",
+                "sources",
+                "hostname",
                 "reachableSources",
-                "hostname"
+                "confSources"
             ],
-            "description": "Summary view for managed network devices and their configured NTP peerings",
+            "description": "NTP - Network Time Protocol - maintains the synchronization of the clock of network devices. NTP server (=time source) provides highly precise clock to NTP clients with the compensation of transport network delay.\n\nMany NTP servers can be configured but not all of them could be available for actual time synchronization. It is important that at least one NTP time source is synchronized to provide common time base for all machines (mainly for logging and troubleshooting)",
             "method": "post",
             "nested_columns": [
                 "sources"
             ],
             "summary": "NTP Summary",
             "ui_columns": [
                 "hostname",
@@ -9163,25 +9205,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/oam/unidirectional-link-detection/interfaces",
             "api_scope_id": "b15757f254cb2f507ab029c8b2a48389b9f83f5e",
             "columns": [
-                "operState",
+                "bidState",
+                "portOperState",
                 "siteName",
+                "sn",
                 "id",
+                "operState",
                 "neighborsCount",
-                "protocol",
-                "sn",
-                "bidState",
                 "portAdminState",
-                "hostname",
                 "intName",
-                "portOperState"
+                "protocol",
+                "hostname"
             ],
             "description": "Unidirectional Link Detection (UDLD) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "UDLD Interfaces",
             "ui_columns": [
                 "hostname",
@@ -9203,23 +9245,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/oam/unidirectional-link-detection/neighbors",
             "api_scope_id": "b300075b857ff6a82d2646a72f27393cfa1753d3",
             "columns": [
-                "deviceId",
                 "siteName",
-                "id",
-                "state",
-                "neighborHostname",
                 "sn",
+                "neighborHostname",
+                "id",
                 "portId",
+                "intName",
+                "deviceId",
                 "hostname",
-                "intName"
+                "state"
             ],
             "description": "Unidirectional Link Detection (UDLD) neighbors inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "UDLD Neighbors",
             "ui_columns": [
                 "hostname",
@@ -9241,28 +9283,28 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/osver-consistency",
             "api_scope_id": "7072e17771ff98bb019aab662d660c9b43167816",
             "columns": [
                 "family",
                 "model",
-                "train",
+                "vendor",
+                "rebuild",
                 "platform",
-                "major",
                 "id",
-                "pctModel",
-                "rebuild",
+                "maintenance",
                 "version",
-                "minor",
+                "major",
                 "count",
+                "pctModel",
                 "pct",
-                "vendor",
-                "maintenance"
+                "train",
+                "minor"
             ],
-            "description": "Operating system consistency table presents the variation of OS versions within each platform and family.",
+            "description": "Operating system consistency table presents the variation of OS versions within each platform\nfamily.\n\nSoftware installed for each platform should vary as least as possible to improve operational\nconsistency, ease troubleshooting, and improve root cause analysis. While it is operationally\ndifficult to introduce consistency as a standalone project, consistent software can be introduced as\npart of the lifecycle software upgrade project.",
             "method": "post",
             "nested_columns": [],
             "summary": "OS Version Consistency",
             "ui_columns": [
                 "vendor",
                 "family",
                 "platform",
@@ -9286,27 +9328,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/port-mirroring",
             "api_scope_id": "33e21fcd65a0e77d842f7e5ac27090b0588f351a",
             "columns": [
-                "src",
-                "siteName",
-                "sessionId",
-                "dscr",
                 "type",
+                "siteName",
+                "sn",
+                "params",
                 "id",
+                "src",
+                "status",
                 "dst",
-                "params",
-                "sn",
+                "dscr",
                 "hostname",
-                "status"
+                "sessionId"
             ],
-            "description": "Port Mirroring table lists all SPAN, RSPAN and ERSPAN sessions configured in the network with their parameters",
+            "description": "Port Mirroring table lists all SPAN, RSPAN and ERSPAN sessions configured in the network with all their parameters:\n* Session ID\n* Status\n* Source interface(s)\n* Destination interface(s)\n* Destination device (ERSPAN only)\n* Any applied policies (ACL, QoS)",
             "method": "post",
             "nested_columns": [],
             "summary": "Port Mirroring",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "sessionId",
@@ -9326,20 +9368,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/ptp/interfaces",
             "api_scope_id": "2e1545c12090b11848dcba90747f86c21b5c2877",
             "columns": [
+                "sn",
                 "siteName",
                 "id",
-                "state",
-                "sn",
+                "intName",
                 "hostname",
-                "intName"
+                "state"
             ],
             "description": "Precision Time Protocol (PTP) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PTP Interfaces",
             "ui_columns": [
                 "hostname",
@@ -9356,29 +9398,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/ptp/local-clock",
             "api_scope_id": "98f5bcd4708d7b2cc0067be361429a7b8ef49a57",
             "columns": [
-                "priority1",
-                "meanPathDelay",
+                "stepsRemoved",
+                "sn",
                 "siteName",
-                "numberOfIfaces",
+                "domain",
                 "id",
-                "mode",
-                "source",
-                "sn",
+                "numberOfIfaces",
                 "offsetFromMaster",
-                "deviceStatus",
-                "domain",
-                "priority2",
                 "localClockIdentity",
+                "mode",
+                "priority2",
+                "source",
+                "priority1",
                 "hostname",
-                "stepsRemoved"
+                "meanPathDelay",
+                "deviceStatus"
             ],
             "description": "Precision Time Protocol (PTP) local clock inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PTP Local clock",
             "ui_columns": [
                 "hostname",
@@ -9404,23 +9446,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/ptp/masters",
             "api_scope_id": "97e1325ac052d315a8b74d01428bb43740891ff8",
             "columns": [
-                "parentClockIdentity",
-                "grandmasterClockIdentity",
-                "priority1",
+                "sn",
                 "siteName",
                 "id",
-                "sn",
-                "parentIPAddress",
+                "parentClockIdentity",
                 "priority2",
-                "hostname"
+                "priority1",
+                "parentIPAddress",
+                "hostname",
+                "grandmasterClockIdentity"
             ],
             "description": "Precision Time Protocol (PTP) masters inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PTP Masters",
             "ui_columns": [
                 "hostname",
@@ -9440,37 +9482,37 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/snapshots",
             "api_scope_id": "241f8bca75d6e0f568ec8ef5375e87b91ae20492",
             "columns": [
-                "id",
-                "unloadedSize",
-                "isLastSnapshot",
-                "interfaceCount",
-                "loadedSize",
-                "deviceRemovedCount",
-                "totalDevCount",
+                "creatorUsername",
+                "fromArchive",
                 "sites",
                 "deviceAddedCount",
-                "tsChange",
-                "tsEnd",
-                "locked",
+                "tsStart",
                 "note",
+                "tsChange",
+                "interfaceEdgeCount",
+                "name",
                 "status",
-                "interfaceActiveCount",
-                "creatorUsername",
-                "finishStatus",
+                "deviceRemovedCount",
+                "interfaceCount",
+                "isLastSnapshot",
                 "loading",
-                "interfaceEdgeCount",
+                "loadedSize",
+                "finishStatus",
+                "tsEnd",
+                "totalDevCount",
+                "id",
+                "unloadedSize",
                 "userCount",
-                "name",
-                "fromArchive",
-                "tsStart"
+                "locked",
+                "interfaceActiveCount"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "sites"
             ],
             "summary": "POST /tables/management/snapshots",
@@ -9508,24 +9550,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/snmp/communities",
             "api_scope_id": "a6e5ab3146ba3c9827722721933cba16f12fbb21",
             "columns": [
+                "prefixes",
+                "authorization",
                 "siteName",
+                "sn",
                 "group",
                 "id",
-                "acl",
-                "authorization",
+                "view",
                 "name",
-                "sn",
-                "prefixes",
                 "hostname",
-                "view"
+                "acl"
             ],
             "description": "SNMP communities and the associated scope restrictions configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "SNMP Communities",
             "ui_columns": [
                 "hostname",
@@ -9546,27 +9588,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/snmp/summary",
             "api_scope_id": "2cf111de911fa7e51eb3b937cdd554585e768691",
             "columns": [
+                "contact",
                 "model",
+                "vendor",
                 "siteName",
+                "sn",
                 "id",
-                "localEngineId",
-                "vendor",
-                "contact",
+                "communitiesCount",
                 "name",
-                "sn",
                 "location",
-                "usersCount",
                 "trapHostsCount",
                 "hostname",
-                "communitiesCount"
+                "usersCount",
+                "localEngineId"
             ],
             "description": "Summary of SNMP protocol configuration on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "SNMP Summary",
             "ui_columns": [
                 "hostname",
@@ -9590,27 +9632,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/snmp/trap-hosts",
             "api_scope_id": "9d89048ea1bfeb940974f945b9a951f060872550",
             "columns": [
-                "vrf",
-                "siteName",
                 "type",
+                "siteName",
+                "sn",
                 "srcInterface",
                 "id",
+                "srcIp",
                 "version",
                 "user",
-                "sn",
-                "community",
-                "dstPort",
-                "srcIp",
                 "hostname",
-                "dstHost"
+                "vrf",
+                "dstHost",
+                "community",
+                "dstPort"
             ],
             "description": "Configured destination hosts for SNMP traps and SNMP inform requests",
             "method": "post",
             "nested_columns": [],
             "summary": "SNMP Hosts",
             "ui_columns": [
                 "hostname",
@@ -9635,22 +9677,22 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/management/snmp/users",
             "api_scope_id": "c74db4530690b81bc9356d33e5eb29502be8a530",
             "columns": [
                 "siteName",
+                "sn",
                 "group",
                 "id",
-                "acl",
                 "name",
-                "sn",
-                "authentication",
+                "privacy",
                 "hostname",
-                "privacy"
+                "acl",
+                "authentication"
             ],
             "description": "SNMP users and the associated scope restrictions configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "SNMP Users",
             "ui_columns": [
                 "hostname",
@@ -9670,24 +9712,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/forwarding",
             "api_scope_id": "d8e037c5b3c9d6932a5d838f17f0d658982b50d3",
             "columns": [
-                "labelIn",
-                "nexthop",
                 "siteName",
+                "sn",
                 "id",
+                "labelIn",
                 "network",
+                "hostname",
                 "prefix",
-                "sn",
-                "hostname"
+                "nexthop"
             ],
-            "description": "MPLS forwarding table maps labels to their associated next hops",
+            "description": "An MPLS forwarding table determines how MPLS handles received MPLS packets. When an MPLS packet arrives on an MPLS interface, MPLS looks up the outermost MPLS label of the received packet in the relevant MPLS forwarding table.\n\nThe entries in the MPLS forwarding table map labels to next hops. Each entry in the MPLS forwarding table points to an entry in the MPLS next-hop table. Each MPLS next hop points to either an interface or another MPLS next hop. The chain of MPLS next hops, which ends at an interface, informs MPLS which labels to push and where to send the MPLS packet.",
             "method": "post",
             "nested_columns": [
                 "nexthop"
             ],
             "summary": "MPLS Forwarding",
             "ui_columns": [
                 "hostname",
@@ -9706,32 +9748,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/circuit-cross-connect",
             "api_scope_id": "604b9e48353cdc825ec2ef56045b4182fba73e08",
             "columns": [
-                "neiHostname",
-                "localLabel",
-                "upTrans",
+                "neiIp",
+                "neiSiteName",
                 "siteName",
-                "stateOrig",
-                "timeLastUp",
+                "sn",
                 "id",
-                "ac",
-                "neiSiteName",
-                "state",
-                "neiIp",
+                "stateOrig",
+                "neiHostname",
                 "name",
-                "sn",
                 "neiSn",
+                "timeLastUp",
+                "upTrans",
+                "remoteLabel",
+                "localLabel",
+                "hostname",
                 "receiveLsp",
+                "ac",
                 "transmitLsp",
-                "hostname",
-                "remoteLabel"
+                "state"
             ],
             "description": "L2 VPN circuit cross-connect inventory with associated parameters",
             "method": "post",
             "nested_columns": [
                 "ac"
             ],
             "summary": "Circuit Cross-Connect",
@@ -9759,32 +9801,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/curcit-cross-connect",
             "api_scope_id": "e563a4c649ced703ac8952f3722f242b157fb2f3",
             "columns": [
-                "neiHostname",
-                "localLabel",
-                "upTrans",
+                "neiIp",
+                "neiSiteName",
                 "siteName",
-                "stateOrig",
-                "timeLastUp",
+                "sn",
                 "id",
-                "ac",
-                "neiSiteName",
-                "state",
-                "neiIp",
+                "stateOrig",
+                "neiHostname",
                 "name",
-                "sn",
                 "neiSn",
+                "timeLastUp",
+                "upTrans",
+                "remoteLabel",
+                "localLabel",
+                "hostname",
                 "receiveLsp",
+                "ac",
                 "transmitLsp",
-                "hostname",
-                "remoteLabel"
+                "state"
             ],
             "description": "L2 VPN circuit cross-connect inventory with associated parameters",
             "method": "post",
             "nested_columns": [
                 "ac"
             ],
             "summary": "Circuit Cross-Connect",
@@ -9812,27 +9854,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/point-to-multipoint",
             "api_scope_id": "fb24ca98d610d19369c2d436fff4b309b1f72ad9",
             "columns": [
-                "neiHostname",
-                "siteName",
-                "id",
-                "bridgeDomain",
+                "neiIp",
                 "localIntName",
-                "ac",
                 "neiSiteName",
-                "neiIp",
-                "name",
+                "siteName",
                 "sn",
-                "state",
+                "id",
+                "neiHostname",
+                "name",
                 "neiSn",
-                "hostname"
+                "bridgeDomain",
+                "hostname",
+                "ac",
+                "state"
             ],
             "description": "L2 VPN Virtual Private LAN Service (VPLS) circuits inventory with associated parameters",
             "method": "post",
             "nested_columns": [
                 "ac"
             ],
             "summary": "Point to multipoint - VPLS",
@@ -9857,36 +9899,36 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/point-to-point-vpws",
             "api_scope_id": "fe3360d96de49c731288cde73f4b3936a3e95377",
             "columns": [
+                "neiIp",
+                "siteName",
+                "sn",
+                "group",
                 "neiHostname",
-                "remoteId",
-                "stateOrig",
-                "id",
+                "routeTargetExport",
+                "ac",
                 "neiSiteName",
-                "neiSn",
+                "name",
+                "signallingProtocol",
+                "remoteLabel",
                 "localLabel",
-                "routeTargetImport",
                 "hostname",
-                "remoteLabel",
-                "signallingProtocol",
+                "vcId",
                 "state",
-                "routeTargetExport",
-                "neiIp",
-                "sn",
-                "siteName",
-                "rd",
-                "group",
-                "ac",
+                "remoteId",
                 "localId",
-                "name",
-                "vcId"
+                "neiSn",
+                "rd",
+                "id",
+                "stateOrig",
+                "routeTargetImport"
             ],
             "description": "Virtual private wire service (VPWS) Layer 2 VPNs inventory with associated parameters",
             "method": "post",
             "nested_columns": [
                 "routeTargetExport",
                 "routeTargetImport"
             ],
@@ -9921,27 +9963,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/pseudowires",
             "api_scope_id": "fc9af0690e54bee2e22a882b7fa126c55e37d92e",
             "columns": [
-                "neiHostname",
-                "localLabel",
-                "siteName",
+                "neiIp",
                 "type",
-                "id",
-                "state",
                 "neiSiteName",
-                "neiIp",
+                "siteName",
                 "sn",
+                "id",
+                "neiHostname",
                 "neiSn",
-                "hostname",
+                "remoteLabel",
                 "intName",
-                "remoteLabel"
+                "localLabel",
+                "hostname",
+                "state"
             ],
             "description": "L2 VPN pseudowires inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "All Pseudowires",
             "ui_columns": [
                 "hostname",
@@ -9964,20 +10006,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/pe-routers",
             "api_scope_id": "1cfed70287e758cc8071aeeeadc4756b1e2d1bcc",
             "columns": [
+                "sn",
                 "siteName",
                 "id",
-                "sn",
-                "vrfCount",
+                "hostname",
                 "ldpIntCount",
-                "hostname"
+                "vrfCount"
             ],
             "description": "Provider Edge routers inventory participating in L3VPNs",
             "method": "post",
             "nested_columns": [],
             "summary": "PE Routers",
             "ui_columns": [
                 "hostname",
@@ -9994,24 +10036,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/pe-routes",
             "api_scope_id": "065884fa26510a46d9872f036030f82fb718b0f2",
             "columns": [
-                "dstHostname",
+                "srcSn",
+                "dstVrf",
+                "srcSiteName",
                 "id",
-                "srcVrf",
+                "srcHostname",
+                "rt",
                 "dstSiteName",
-                "srcSiteName",
                 "prefix",
-                "dstVrf",
-                "rt",
-                "srcHostname",
-                "srcSn",
+                "srcVrf",
+                "dstHostname",
                 "dstSn"
             ],
             "description": "Routes on PE in VRF including originating source PE",
             "method": "post",
             "nested_columns": [],
             "summary": "PE Routes",
             "ui_columns": [
@@ -10033,22 +10075,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/pe-vrfs",
             "api_scope_id": "bfa6fae289b59bc14e2948a07d67f8f1880d226a",
             "columns": [
-                "routeCount",
-                "siteName",
                 "rd",
-                "id",
+                "siteName",
                 "sn",
-                "af",
+                "id",
+                "hostname",
                 "vrf",
-                "hostname"
+                "af",
+                "routeCount"
             ],
             "description": "VRF configured on PE routers with summary of routes in VRF",
             "method": "post",
             "nested_columns": [
                 "af"
             ],
             "summary": "VRFs on PE Routers",
@@ -10069,23 +10111,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/vrf-targets",
             "api_scope_id": "8be522685b7bba581fa7344211199166a09afab2",
             "columns": [
-                "siteName",
-                "importRT",
                 "rd",
-                "id",
+                "siteName",
                 "sn",
-                "af",
-                "exportRT",
+                "id",
+                "importRT",
+                "hostname",
                 "vrf",
-                "hostname"
+                "exportRT",
+                "af"
             ],
             "description": "Route targets import and export configured in VRF",
             "method": "post",
             "nested_columns": [
                 "exportRT",
                 "importRT"
             ],
@@ -10108,26 +10150,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/ldp/interfaces",
             "api_scope_id": "0a2ca2f54da9c530f16ff6c93e8ecd217dcd0ad5",
             "columns": [
-                "siteName",
                 "localAddress",
-                "id",
                 "localId",
+                "siteName",
                 "sn",
+                "id",
+                "intName",
                 "neiCount",
-                "timerHello",
                 "hostname",
-                "intName",
-                "timerHoldtime"
+                "timerHoldtime",
+                "timerHello"
             ],
-            "description": "Label Distribution Protocol (LDP) interfaces inventory",
+            "description": "LDP interfaces table lists all the LDP enabled interfaces, their IDs, number of neighbors and configured timers.",
             "method": "post",
             "nested_columns": [],
             "summary": "LDP Interfaces",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -10146,35 +10188,35 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/ldp/neighbors",
             "api_scope_id": "76fbda3767ec3045a39337cfd3ff1d54f1b8bc76",
             "columns": [
+                "siteName",
+                "sn",
                 "neiHostname",
-                "id",
+                "source",
+                "neiIntName",
+                "vrf",
                 "neiSiteName",
-                "neiSn",
-                "neiId",
-                "neiDevType",
                 "intName",
-                "neiAddress",
-                "neiIntName",
-                "localAddress",
                 "hostname",
-                "subnet",
-                "source",
-                "sn",
-                "siteName",
+                "neiDevType",
+                "target",
+                "neiAddress",
+                "neiSn",
                 "currStateTime",
+                "subnet",
+                "neiId",
                 "devType",
-                "vrf",
-                "target"
+                "localAddress",
+                "id"
             ],
-            "description": "Label Distribution Protocol (LDP) neighbors inventory",
+            "description": "LDP Neighbors table lists all the LDP neighbors, their interfaces, addressing and time the LDP session is established.",
             "method": "post",
             "nested_columns": [],
             "summary": "LDP Neighbors",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -10194,28 +10236,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/rsvp/interfaces",
             "api_scope_id": "1c9518f9324c531a7e3c9ac6e83a25475115ac2c",
             "columns": [
-                "linkProtectionUnprotectedLsp",
-                "linkProtectionBypass",
-                "siteName",
                 "localAddress",
-                "linkProtectionLsp",
-                "id",
-                "allocatedBw",
                 "linkProtectionProtectedLsp",
+                "siteName",
+                "linkProtectionUnprotectedLsp",
                 "sn",
-                "neiCount",
-                "linkProtectionStatus",
+                "id",
+                "linkProtectionBypass",
                 "maxBw",
+                "intName",
+                "neiCount",
                 "hostname",
-                "intName"
+                "linkProtectionLsp",
+                "allocatedBw",
+                "linkProtectionStatus"
             ],
             "description": "Resource Reservation Protocol (RSVP) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "RSVP Interfaces",
             "ui_columns": [
                 "hostname",
@@ -10240,38 +10282,38 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/mpls/rsvp/neighbors",
             "api_scope_id": "ef6caf43c344e8cdfef7196e1793efd95c1b1645",
             "columns": [
+                "siteName",
+                "sn",
                 "neiHostname",
-                "id",
-                "neiSiteName",
-                "neiSn",
-                "linkProtectionBackupLspsCount",
-                "intName",
-                "neiAddress",
+                "linkProtectionBackupRoutesCount",
                 "frrLspsCount",
-                "localAddress",
+                "vrf",
                 "linkProtectionLspName",
                 "frrStatus",
-                "linkProtectionStatus",
+                "neiSiteName",
+                "status",
+                "intName",
                 "hostname",
+                "localId",
+                "neiAddress",
+                "neiSn",
+                "linkProtectionBackupLspsCount",
                 "linkProtectionBypassLsp",
-                "sn",
-                "linkProtectionBypassExplicitRoute",
-                "status",
                 "via",
-                "siteName",
                 "currStateTime",
-                "localId",
-                "linkProtectionBackupRoutesCount",
-                "vrf",
-                "neiId"
+                "neiId",
+                "linkProtectionBypassExplicitRoute",
+                "localAddress",
+                "id",
+                "linkProtectionStatus"
             ],
             "description": "Resource Reservation Protocol (RSVP) neighbors inventory",
             "method": "post",
             "nested_columns": [
                 "linkProtectionBypassExplicitRoute"
             ],
             "summary": "RSVP Neighbors",
@@ -10306,26 +10348,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/groups",
             "api_scope_id": "38cc3d8adec28713bc38d8d04415b811fc6672f4",
             "columns": [
-                "groupIp",
-                "siteName",
                 "lastReporter",
+                "groupIp",
                 "type",
-                "id",
-                "uptime",
+                "siteName",
                 "sn",
+                "id",
                 "expires",
-                "sourceIp",
-                "vrf",
+                "intName",
                 "hostname",
-                "intName"
+                "sourceIp",
+                "uptime",
+                "vrf"
             ],
             "description": "Internet Group Management Protocol (IGMP) groups inventory and their associated hosts",
             "method": "post",
             "nested_columns": [],
             "summary": "IGMP Groups",
             "ui_columns": [
                 "hostname",
@@ -10348,25 +10390,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/interfaces",
             "api_scope_id": "ad3146326a1275d2bcbab09d0e8e3a8c18f4ddea",
             "columns": [
-                "lastMemberQueryCount",
                 "siteName",
+                "sn",
                 "id",
-                "queryInterval",
-                "queryResponseTime",
+                "lastMemberQueryCount",
                 "version",
-                "sn",
                 "lastMemberQueryInterval",
-                "vrf",
-                "hostname",
+                "queryResponseTime",
                 "intName",
+                "hostname",
+                "queryInterval",
+                "vrf",
                 "querierIp"
             ],
             "description": "Internet Group Management Protocol (IGMP) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "IGMP Interfaces",
             "ui_columns": [
@@ -10390,24 +10432,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/snooping/global",
             "api_scope_id": "f3b9756d2b115896e1e2370da8aea74fe48f9944",
             "columns": [
-                "v3enabled",
+                "reportSuppression",
                 "siteName",
-                "id",
-                "enabled",
-                "v3reportSuppression",
                 "sn",
+                "id",
                 "omf",
-                "v2fastLeave",
+                "enabled",
+                "v3enabled",
                 "hostname",
-                "reportSuppression"
+                "v3reportSuppression",
+                "v2fastLeave"
             ],
             "description": "Internet Group Management Protocol (IGMP) snooping global inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "IGMP Snooping",
             "ui_columns": [
                 "hostname",
@@ -10429,23 +10471,23 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/snooping/groups",
             "api_scope_id": "11b3b8381499a8e82f53cac2b28e304491788813",
             "columns": [
                 "groupIp",
-                "siteName",
-                "vlan",
                 "type",
+                "siteName",
+                "sn",
                 "id",
                 "version",
-                "sn",
+                "hostname",
                 "sourceIp",
+                "vlan",
                 "intNameList",
-                "hostname",
                 "flood"
             ],
             "description": "Internet Group Management Protocol (IGMP) snooping groups inventory",
             "method": "post",
             "nested_columns": [
                 "intNameList"
             ],
@@ -10470,29 +10512,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/snooping/vlans",
             "api_scope_id": "1bac49fe53b01f55508ab37e0e676123d28da514",
             "columns": [
-                "siteName",
-                "vlan",
-                "floodingToVlan",
-                "id",
-                "enabled",
+                "explicitTracking",
                 "v3reportSuppression",
-                "lookupMode",
+                "reportSuppression",
+                "vlanVpc",
+                "siteName",
                 "sn",
+                "id",
                 "omf",
-                "explicitTracking",
-                "reportSuppression",
+                "enabled",
                 "v2fastLeave",
                 "hostname",
                 "querierIp",
-                "vlanVpc"
+                "lookupMode",
+                "vlan",
+                "floodingToVlan"
             ],
             "description": "Internet Group Management Protocol (IGMP) snooping VLANs inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "IGMP Snooping Vlans",
             "ui_columns": [
                 "hostname",
@@ -10518,22 +10560,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/mac",
             "api_scope_id": "610c9297a0c6d81127c9b2a4b1ef38ffd268d948",
             "columns": [
-                "siteName",
-                "vlan",
                 "type",
+                "siteName",
+                "sn",
                 "id",
+                "hostname",
+                "vlan",
                 "mac",
-                "sn",
-                "intNameList",
-                "hostname"
+                "intNameList"
             ],
             "description": "Multicast MAC Table inventory",
             "method": "post",
             "nested_columns": [
                 "intNameList"
             ],
             "summary": "Multicast MAC Table",
@@ -10555,26 +10597,26 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/interfaces",
             "api_scope_id": "68755dc320dd425915159c25fa4b0cc39a370575",
             "columns": [
                 "drIp",
+                "isDr",
                 "siteName",
+                "sn",
                 "id",
-                "priority",
                 "version",
-                "sn",
-                "neiCount",
                 "queryTimer",
+                "priority",
                 "ip",
-                "vrf",
-                "hostname",
                 "intName",
-                "isDr"
+                "neiCount",
+                "hostname",
+                "vrf"
             ],
             "description": "Protocol-Independent Multicast (PIM) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PIM Interfaces",
             "ui_columns": [
                 "hostname",
@@ -10596,38 +10638,38 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/neighbors",
             "api_scope_id": "5f49a26c60451da92a9d644c43b265f74f97be49",
             "columns": [
+                "isDr",
+                "siteName",
+                "sn",
                 "neiHostname",
-                "id",
-                "priority",
+                "mode",
+                "source",
+                "neiIntName",
+                "vrf",
                 "neiSiteName",
-                "uptime",
-                "version",
-                "neiSn",
-                "neiDevType",
+                "expires",
+                "priority",
                 "intName",
-                "neiAddress",
-                "neiIntName",
-                "flags",
-                "localAddress",
                 "hostname",
+                "neiDevType",
+                "target",
+                "neiAddress",
+                "neiSn",
                 "subnet",
-                "source",
-                "sn",
-                "siteName",
-                "mode",
                 "devType",
-                "expires",
-                "vrf",
-                "target",
-                "isDr"
+                "flags",
+                "localAddress",
+                "id",
+                "version",
+                "uptime"
             ],
             "description": "Protocol-Independent Multicast (PIM) neighbors inventory",
             "method": "post",
             "nested_columns": [
                 "flags"
             ],
             "summary": "PIM Neighbors",
@@ -10656,21 +10698,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/bsr",
             "api_scope_id": "c01133c1598bf86c392c132b8b3f6747a98008f7",
             "columns": [
                 "siteName",
-                "bsrIp",
+                "sn",
                 "id",
+                "bsrIp",
                 "bsrRoutersCount",
-                "sn",
-                "bsrRouters",
+                "hostname",
                 "vrf",
-                "hostname"
+                "bsrRouters"
             ],
             "description": "Protocol-Independent Multicast (PIM) rendezvous points (RP) inventory",
             "method": "post",
             "nested_columns": [
                 "bsrRouters"
             ],
             "summary": "PIM Bootstrap RP",
@@ -10692,22 +10734,22 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/mappings",
             "api_scope_id": "f3bd34f02855b4978032f2e49e05906674bbe8a6",
             "columns": [
                 "siteName",
-                "id",
-                "uptime",
                 "sn",
-                "rpRouters",
+                "id",
                 "rpIp",
-                "vrf",
+                "groupsCount",
                 "hostname",
-                "groupsCount"
+                "rpRouters",
+                "uptime",
+                "vrf"
             ],
             "description": "Protocol-Independent Multicast (PIM) and rendezvous points (RP) mappings",
             "method": "post",
             "nested_columns": [
                 "rpRouters"
             ],
             "summary": "PIM Boostrap RP mappings",
@@ -10730,24 +10772,24 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/mappings-groups",
             "api_scope_id": "34d0e544083871a64602b364b0c0348985cf2662",
             "columns": [
                 "siteName",
+                "sn",
                 "id",
-                "uptime",
+                "groupUptime",
+                "rpIp",
                 "groupNet",
+                "hostname",
                 "learnedFrom",
-                "sn",
                 "rpRouters",
-                "groupUptime",
-                "rpIp",
-                "vrf",
-                "hostname"
+                "uptime",
+                "vrf"
             ],
             "description": "Protocol-Independent Multicast (PIM) and rendezvous points (RP) mapping groups",
             "method": "post",
             "nested_columns": [
                 "rpRouters"
             ],
             "summary": "PIM Bootstrap RP mappings groups",
@@ -10771,21 +10813,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/overview",
             "api_scope_id": "4eef5c24a1ac421d259e76caf9e7b34c106a7f6e",
             "columns": [
-                "routersCount",
                 "siteName",
-                "vrfList",
                 "id",
+                "rpIp",
+                "routersCount",
+                "vrfList",
                 "rpHostname",
-                "rpSn",
-                "rpIp"
+                "rpSn"
             ],
             "description": "Rendezvous points (RP) routers inventory",
             "method": "post",
             "nested_columns": [
                 "vrfList"
             ],
             "summary": "RP Routers",
@@ -10805,33 +10847,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/counters",
             "api_scope_id": "a6764383fe5a005530269edb27703c1d789434a1",
             "columns": [
-                "id",
-                "inPktsRate",
+                "inPkts",
+                "siteName",
+                "sn",
+                "group",
+                "rpfErr",
+                "otherErrRate",
+                "vrf",
+                "outPkts",
+                "hostname",
                 "avgPkt",
                 "outPktsRate",
                 "rpfNeiIp",
-                "rpfErr",
-                "outPkts",
                 "rpfErrRate",
-                "otherErr",
-                "hostname",
-                "sourceNet",
-                "inIntName",
                 "groupNet",
-                "inPkts",
-                "sn",
-                "otherErrRate",
-                "siteName",
-                "group",
-                "vrf"
+                "inIntName",
+                "id",
+                "inPktsRate",
+                "otherErr",
+                "sourceNet"
             ],
             "description": "Multicast routing table counters with RPF and other errors",
             "method": "post",
             "nested_columns": [],
             "summary": "MRoute Counters",
             "ui_columns": [
                 "hostname",
@@ -10861,18 +10903,18 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/first-hop-router",
             "api_scope_id": "a2d8d8caafa37b2b7cebcdb342ec755b40627a8f",
             "columns": [
+                "sn",
                 "siteName",
-                "sourceCount",
                 "id",
-                "sn",
+                "sourceCount",
                 "fwdCount",
                 "hostname"
             ],
             "description": "Multicast first hop routers inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Multicast First Hop Routers",
@@ -10892,27 +10934,27 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/outgoing-interfaces",
             "api_scope_id": "218d0c9b6e89ee9f1c4cc3892b5bd99587c77202",
             "columns": [
                 "family",
-                "flags",
+                "vendor",
                 "siteName",
-                "group",
-                "id",
+                "sn",
                 "age",
+                "id",
+                "group",
                 "mode",
-                "sourceNet",
-                "vendor",
                 "groupNet",
-                "sn",
-                "vrf",
+                "intName",
                 "hostname",
-                "intName"
+                "vrf",
+                "flags",
+                "sourceNet"
             ],
             "description": "Multicast routing table outgoing interface list detail",
             "method": "post",
             "nested_columns": [
                 "flags"
             ],
             "summary": "Multicast OIL",
@@ -10940,20 +10982,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/overview",
             "api_scope_id": "c2b90837f180df63efa3ab4f67c7114dd86d5a97",
             "columns": [
                 "siteName",
-                "activeRoutesCount",
+                "sn",
                 "id",
                 "routesCount",
-                "sn",
+                "hostname",
                 "vrf",
-                "hostname"
+                "activeRoutesCount"
             ],
             "description": "Overview of devices with multicast routes in mroute table",
             "method": "post",
             "nested_columns": [],
             "summary": "MRoute Overview",
             "ui_columns": [
                 "hostname",
@@ -10972,25 +11014,25 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/sources",
             "api_scope_id": "47addb3582a3f5c3e689abc9ddc5085427f7f44e",
             "columns": [
                 "incomingInt",
-                "oilCount",
-                "siteName",
                 "isLocal",
+                "siteName",
                 "group",
                 "id",
-                "sourceNet",
-                "groupNet",
                 "sn",
-                "mac",
+                "groupNet",
+                "hostname",
                 "vrf",
-                "hostname"
+                "oilCount",
+                "mac",
+                "sourceNet"
             ],
             "description": "Routers with multicast sources inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Routers with Multicast Sources",
             "ui_columns": [
                 "hostname",
@@ -11014,29 +11056,29 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/table",
             "api_scope_id": "a77fd5a614ecdb3c3d3f0fd09c8aff1119c7388b",
             "columns": [
                 "family",
-                "flags",
+                "vendor",
                 "siteName",
-                "group",
-                "id",
+                "sn",
                 "age",
+                "id",
+                "group",
                 "rpfNeiIp",
-                "sourceNet",
-                "inIntName",
-                "groupNet",
-                "sn",
                 "rpIp",
+                "groupNet",
                 "outIntNames",
-                "vrf",
                 "hostname",
-                "vendor"
+                "vrf",
+                "sourceNet",
+                "flags",
+                "inIntName"
             ],
             "description": "Global multicast routing table",
             "method": "post",
             "nested_columns": [
                 "flags",
                 "outIntNames"
             ],
@@ -11066,31 +11108,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/neighbors/all",
             "api_scope_id": "f8a11e7f648c796c51d0edc3e8198382e9b22e11",
             "columns": [
+                "remoteHost",
+                "protocols",
+                "remoteDevType",
+                "managedDev",
                 "remoteIp",
+                "localHost",
                 "siteName",
-                "capabilities",
                 "id",
-                "managedDev",
-                "remoteDevType",
-                "localInt",
                 "remoteInt",
-                "remoteHost",
-                "localHost",
                 "remoteSn",
-                "protocols",
                 "remoteIpv6List",
-                "localSn",
-                "netDev"
+                "localInt",
+                "netDev",
+                "capabilities",
+                "localSn"
             ],
-            "description": "Discovery protocol neighbors inventory (CDP, LLDP, mDP)",
+            "description": "This table shows all discovery protocol neighbors found by those discovery protocols.",
             "method": "post",
             "nested_columns": [
                 "protocols",
                 "remoteIpv6List"
             ],
             "summary": "Discovery Protocol Neighbors",
             "ui_columns": [
@@ -11116,31 +11158,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/neighbors/endpoints",
             "api_scope_id": "6f9d12326a55c51f87ae978c06f0c0a403441108",
             "columns": [
+                "remoteHost",
+                "protocols",
+                "remoteDevType",
+                "managedDev",
                 "remoteIp",
+                "localHost",
                 "siteName",
-                "capabilities",
                 "id",
-                "managedDev",
-                "remoteDevType",
-                "localInt",
                 "remoteInt",
-                "remoteHost",
-                "localHost",
                 "remoteSn",
-                "protocols",
                 "remoteIpv6List",
-                "localSn",
-                "netDev"
+                "localInt",
+                "netDev",
+                "capabilities",
+                "localSn"
             ],
-            "description": "Endpoints viewed by discover protocols",
+            "description": "This table shows all discovery protocol endpoints found by those discovery protocols.",
             "method": "post",
             "nested_columns": [
                 "protocols",
                 "remoteIpv6List"
             ],
             "summary": "Discovery Protocols - Endpoints",
             "ui_columns": [
@@ -11165,28 +11207,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/neighbors/unidirectional",
             "api_scope_id": "e354e80204b939083c3f7c3bec2f43fb297d22f3",
             "columns": [
+                "remoteHost",
+                "protocols",
                 "remoteIp",
                 "siteName",
-                "capabilities",
+                "localHost",
                 "id",
                 "remoteInt",
-                "localInt",
-                "remoteHost",
-                "localHost",
                 "remoteSn",
-                "protocols",
                 "remoteIpv6List",
+                "localInt",
+                "capabilities",
                 "localSn"
             ],
-            "description": "Unidirectional discovery protocol relationship between managed network devices",
+            "description": "Although both neighbors are managed, the local neighbor is not correctly seen by the remote neighbor. XDP sessions should be bidirectional\nwhen enabled.\\\nXDP settings on both neighbors should be synchronized.",
             "method": "post",
             "nested_columns": [
                 "remoteIpv6List",
                 "protocols"
             ],
             "summary": "Discovery Protocols - Unidirectional Neighbors",
             "ui_columns": [
@@ -11209,27 +11251,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/neighbors/unmanaged",
             "api_scope_id": "02f378dc295d5eaa5fb6e5e0957d19887132dd2e",
             "columns": [
+                "remoteHost",
+                "protocols",
                 "remoteIp",
                 "siteName",
-                "capabilities",
+                "localHost",
                 "id",
                 "remoteInt",
-                "localInt",
-                "remoteHost",
-                "localHost",
-                "protocols",
                 "remoteIpv6List",
+                "localInt",
+                "capabilities",
                 "localSn"
             ],
-            "description": "Unmanaged neighbors detected by discovery protocols of managed network devices",
+            "description": "Link layer neighbors such as CDP / LLDP / EDP protocols should be within a single administrative domain. Link layer discovery protocols generously share\nmanagement information without authentication by design, and should be within a single administrative domain. Running link layer discovery protocols\nsuch as CDP / LLDP / EDP between management domains poses a moderate security risk, and should not be used without consideration. Link layer discovery\nprotocols should be turned off or verified on these ports.\n\nRemote device is not reachable in this table. More information about the reason is in the Discovery Connectivity report.",
             "method": "post",
             "nested_columns": [
                 "protocols",
                 "remoteIpv6List"
             ],
             "summary": "Discovery protocols - Unmanaged Neighbors",
             "ui_columns": [
@@ -11252,27 +11294,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks",
             "api_scope_id": "78d74b21341d6a85cdcbcbd23a17d9aaf8e03ea0",
             "columns": [
-                "gwV",
-                "siteName",
-                "gwcountV",
+                "gw",
                 "hosts",
+                "siteName",
                 "id",
+                "gwcount",
                 "net",
                 "vlanId",
-                "gw",
                 "mask",
+                "gwcountV",
                 "vrf",
-                "gwcount"
+                "gwV"
             ],
-            "description": "Detected Layer 3 network (connected/direct/local) inventory",
+            "description": "Information about every discovered Layer 3 network (connected/direct/local) on the managed network infrastructure devices. Each line represents one physical segment or VLAN with assigned IP address.",
             "method": "post",
             "nested_columns": [],
             "summary": "Managed Networks",
             "ui_columns": [
                 "siteName",
                 "net",
                 "hosts",
@@ -11290,20 +11332,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/domain",
             "api_scope_id": "f2253e88edbf0f0db2ad794d08be6aecf37390e7",
             "columns": [
-                "siteName",
                 "rd",
-                "routers",
-                "id",
+                "siteName",
                 "users",
-                "networks"
+                "id",
+                "networks",
+                "routers"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/networks/domain",
             "ui_columns": [
                 "id",
@@ -11322,27 +11364,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/gateway-redundancy",
             "api_scope_id": "ae4a4ce3081fe067d9dc37056bfcdebb4b87d3f2",
             "columns": [
-                "gwV",
-                "siteName",
-                "gwcountV",
+                "gw",
                 "hosts",
+                "siteName",
                 "id",
+                "gwcount",
                 "net",
                 "vlanId",
-                "gw",
                 "mask",
+                "gwcountV",
                 "vrf",
-                "gwcount"
+                "gwV"
             ],
-            "description": "Inventory of available gateways for each discovered network",
+            "description": "The table presents the number of available gateways for each discovered network (physical or VLAN). It is desirable for networks serving hosts to have multiple routing gateways to avoid single point of failure.",
             "method": "post",
             "nested_columns": [],
             "summary": "Gateway Redundancy",
             "ui_columns": [
                 "siteName",
                 "net",
                 "hosts",
@@ -11359,28 +11401,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/ipv6-routes",
             "api_scope_id": "f3147d62d2934793c72f4fc2cc2f2dfe48cf1272",
             "columns": [
-                "nexthop",
+                "nhLowestAge",
                 "siteName",
-                "nhLowestMetric",
+                "sn",
                 "id",
                 "network",
-                "prefix",
-                "protocol",
-                "nhLowestAge",
-                "sn",
                 "nhCount",
+                "nhLowestMetric",
+                "protocol",
+                "hostname",
+                "prefix",
                 "vrf",
-                "hostname"
+                "nexthop"
             ],
-            "description": "Global IPv6 routing table",
+            "description": "The cumulative IPv6 Routing Table contains all entries from all routing tables and all VRFs collected from all managed network devices with L3 routing capability. Each line represents a corresponding entry from the source routing table, normalized into a standard terse view.",
             "method": "post",
             "nested_columns": [
                 "nexthop"
             ],
             "summary": "IPv6 Routing Table",
             "ui_columns": [
                 "hostname",
@@ -11403,33 +11445,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/path-lookup-checks",
             "api_scope_id": "fd66c4e4b8932edbeaaf88675387bed884fffd18",
             "columns": [
-                "networkMode",
                 "passingTraffic",
-                "result",
-                "securedPath",
+                "parameters",
                 "settings",
-                "flags",
-                "dstPorts",
-                "src",
                 "srcPorts",
                 "type",
+                "securedPath",
                 "id",
-                "receiver",
+                "src",
                 "dst",
+                "result",
+                "dstPorts",
+                "networkMode",
                 "protocol",
-                "expectedPassingTraffic",
                 "vrf",
-                "parameters"
+                "expectedPassingTraffic",
+                "receiver",
+                "flags"
             ],
-            "description": "Saved path simulations inventory, including End-to-End settings intended and simulated result.",
+            "description": "Path verifications table shows all the configured Path Verification rules, including End-to-End settings and intended and simulated result.",
             "method": "post",
             "nested_columns": [
                 "flags",
                 "result"
             ],
             "summary": "Saved Path Simulations",
             "ui_columns": [
@@ -11454,26 +11496,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/policies/prefix-lists/ipv4",
             "api_scope_id": "5343e14f5a81bc4f16ee3efe2257078b10bf7abf",
             "columns": [
+                "maskMin",
                 "siteName",
-                "maskEqual",
+                "sn",
                 "id",
-                "maskMax",
-                "sequence",
-                "prefix",
                 "name",
-                "sn",
+                "sequence",
                 "action",
+                "maskEqual",
+                "hostname",
                 "mask",
-                "maskMin",
-                "hostname"
+                "prefix",
+                "maskMax"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/networks/policies/prefix-lists/ipv4",
             "ui_columns": [
                 "hostname",
@@ -11496,25 +11538,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/policies/prefix-lists/ipv6",
             "api_scope_id": "12910b3fba7152fb29785afe67e8d8a757df79a0",
             "columns": [
+                "maskMin",
                 "siteName",
-                "maskEqual",
+                "sn",
                 "id",
-                "maskMax",
-                "sequence",
-                "prefix",
                 "name",
-                "sn",
+                "sequence",
                 "action",
-                "maskMin",
-                "hostname"
+                "maskEqual",
+                "hostname",
+                "prefix",
+                "maskMax"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/networks/policies/prefix-lists/ipv6",
             "ui_columns": [
                 "hostname",
@@ -11536,27 +11578,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/policies/routing",
             "api_scope_id": "b05911a0cdc128efc32b4b8c7e523ddb79b298a6",
             "columns": [
-                "matchedBytes",
-                "siteName",
-                "matchList",
+                "matchedPackets",
                 "type",
+                "siteName",
+                "sn",
                 "id",
-                "sequence",
                 "name",
-                "sn",
                 "action",
-                "matchedPackets",
-                "setList",
                 "continue",
-                "hostname"
+                "setList",
+                "hostname",
+                "matchedBytes",
+                "matchList",
+                "sequence"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "matchList",
                 "setList"
             ],
@@ -11583,22 +11625,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/policies/routing/interfaces",
             "api_scope_id": "c718018bdcbca27e50ce8b156b9277bcb88b85c1",
             "columns": [
-                "addressFamily",
                 "siteName",
+                "sn",
                 "id",
+                "addressFamily",
                 "name",
-                "sn",
-                "hostname",
+                "status",
                 "intName",
-                "status"
+                "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/networks/policies/routing/interfaces",
             "ui_columns": [
                 "hostname",
@@ -11616,23 +11658,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/route-stability",
             "api_scope_id": "8ded207b292a9d31bbd7e77008b30a4f78d70b1e",
             "columns": [
-                "presence",
-                "ribCount",
-                "ratioCrit",
                 "id",
-                "prefix",
                 "ratioWarn",
-                "ratioInfo"
+                "ratioCrit",
+                "presence",
+                "ribCount",
+                "ratioInfo",
+                "prefix"
             ],
-            "description": "Unique routed networks, the number of times route is observed, expressed in absolute and percentage values",
+            "description": "Routing consistency and stability analysis can be performed using the routing stability table. The table lists all unique routed networks, the number of times route is observed, expressed in absolute and percentage values, and percentage of routes that have next hop age below certain threshold signifying convergence.The table can be used to verify if similar routes are present in the same number of the routing tables, find starting point for troubleshooting convergence, or check route distribution across the network, including verifying presence of a default route.",
             "method": "post",
             "nested_columns": [],
             "summary": "Routing Stability",
             "ui_columns": [
                 "prefix",
                 "ribCount",
                 "ratioInfo",
@@ -11649,28 +11691,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/routes",
             "api_scope_id": "30e1e29a9e033f86d03a7512dc31fbb36ff1f113",
             "columns": [
-                "nexthop",
+                "nhLowestAge",
                 "siteName",
-                "nhLowestMetric",
+                "sn",
                 "id",
                 "network",
-                "prefix",
-                "protocol",
-                "nhLowestAge",
-                "sn",
                 "nhCount",
+                "nhLowestMetric",
+                "protocol",
+                "hostname",
+                "prefix",
                 "vrf",
-                "hostname"
+                "nexthop"
             ],
-            "description": "Global IPv4 routing table",
+            "description": "Cumulative routing table contains all entries from all routing tables and all VRFs collected from all managed network devices with L3 routing capability. Each line represents a corresponding entry from the source routing table, normalized into a standard terse view. Table can be filtered per site, per device, per route, number of next hops, lowest metric of next hops, or other next hop information. Individual routes can be looked up as a string, or as a route for a specific IP address. For example, IP address of 10.0.0.1 will return routes 10.0.0.0/24 and 0.0.0.0/0, but not 10.0.1.0/24.",
             "method": "post",
             "nested_columns": [
                 "nexthop"
             ],
             "summary": "IPv4 Routing Table",
             "ui_columns": [
                 "hostname",
@@ -11693,27 +11735,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols",
             "api_scope_id": "eeb72ee377ca3c157bf8200a204e18f6e28d8492",
             "columns": [
+                "sn",
                 "siteName",
-                "subnets",
                 "id",
+                "replicates",
+                "subnets",
                 "memory",
-                "overhead",
-                "sn",
-                "networks",
                 "protocol",
-                "vrf",
+                "networks",
                 "hostname",
-                "replicates"
+                "vrf",
+                "overhead"
             ],
-            "description": "Summary routing table information about routing protocols for all managed devices",
+            "description": "Summary routing table information about routing protocols on each device. Possible values for the \"Protocol\" column are\n\n* connected/direct/local - for locally connected networks\n* static - for static routes\n* rip - RIP dynamic routing protocol\n* eigrp - EIGRP dynamic routing protocol\n* ospf - OSPF dynamic routing protocol\n* is-is - IS-IS dynamic routing protocol\n* bgp - BGP dynamic routing protocol\n* nhrp - NHRP dynamic routing mechanism\n* application - installed by SDN controller or application\n* internal - not owned by any routing mechanism above",
             "method": "post",
             "nested_columns": [],
             "summary": "Network Routing Protocols Summary",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "protocol",
@@ -11733,25 +11775,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/bgp",
             "api_scope_id": "e2f318fc70da867d8e8e7d8ce3ba9e39135b46e1",
             "columns": [
-                "external",
-                "as",
+                "sn",
                 "siteName",
                 "id",
                 "local",
-                "sn",
                 "internal",
+                "hostname",
                 "vrf",
-                "hostname"
+                "as",
+                "external"
             ],
-            "description": "Border Gateway Protocol (BGP) routes summary",
+            "description": "This table covers total number of BGP routes of each type.\n\nBGP routes can be classified based on BGP origin attribute\n\nLocally generated BGP route has been created with the local aggregation or \"network\" command.",
             "method": "post",
             "nested_columns": [],
             "summary": "BGP Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "as",
@@ -11769,25 +11811,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/eigrp",
             "api_scope_id": "78fc4db6c1f540647668280b112bb33232d20668",
             "columns": [
+                "sn",
                 "siteName",
-                "subnets",
                 "id",
+                "replicates",
+                "subnets",
                 "memory",
-                "overhead",
-                "sn",
-                "networks",
                 "protocol",
-                "vrf",
+                "networks",
                 "hostname",
-                "replicates"
+                "vrf",
+                "overhead"
             ],
             "description": "Enhanced Interior Gateway Routing Protocol (EIGRP) routes summary",
             "method": "post",
             "nested_columns": [],
             "summary": "EIGRP Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
@@ -11808,24 +11850,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/isis",
             "api_scope_id": "38fae7a5d58999f7e6d6ae5e31d9b15dea8c7738",
             "columns": [
-                "level1",
-                "siteName",
                 "interArea",
+                "sn",
+                "siteName",
                 "id",
+                "level1",
                 "level2",
-                "sn",
-                "vrf",
-                "hostname"
+                "hostname",
+                "vrf"
             ],
-            "description": "Intermediate System to Intermediate System (IS-IS) routes summary",
+            "description": "IS-IS protocol summary table.\n\nIn IS-IS, routing between areas is organized hierarchically. This organization is accomplished by configuring Level 1 and Level 2 intermediate systems.\n\nLevel 1 systems route within an area. When the destination is outside an area, Level 1 systems route toward a Level 2 system. Level 2 intermediate systems route between areas and toward other ASs. No IS-IS area functions strictly as a backbone (such as area 0 in OSPF). All routers in one area must share the same topology database and run SPF algorithm on that.\n\nLevel 1 routers share intra-area routing information, and Level 2 routers share interarea information about IP addresses available within each area. IS-IS routers can act as both Level 1 and Level 2 routers, sharing intra-area routes with other Level 1 routers and interarea routes with other Level 2 routers.",
             "method": "post",
             "nested_columns": [],
             "summary": "IS-IS Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "level1",
@@ -11842,28 +11884,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/ospf",
             "api_scope_id": "395ba95624cadfd1c00e32e63d2eaf520623fa9d",
             "columns": [
-                "vrf",
-                "external1",
+                "intraArea",
                 "interArea",
-                "process",
+                "sn",
+                "nssaEx1",
                 "siteName",
                 "id",
-                "nssaEx1",
-                "sn",
-                "nssaEx2",
-                "intraArea",
+                "external2",
                 "hostname",
-                "external2"
+                "process",
+                "external1",
+                "vrf",
+                "nssaEx2"
             ],
-            "description": "Open Shortest Path First routes summary",
+            "description": "This table covers total number of OSPF routes of each type.\\\nOSPF routing domain can be split into multiple areas. SPF algorithm is run in each area independently, routers in the same OSPF area must share same topology information. Area 0 forms the backbone area interconnecting other (non-zero) areas. Area boundaries are on the routers (each OSPF interface can be in different area).\n\nOSPF route types (\"Network Type\") can be:\n* Intra-Area (O) - originated in local OSPF area by the \"network\" command\n* Inter-Area (O IA) - originated in OSPF area which is not presewnt on local router by the \"network\" command\n* External type 1 (O E1) - originated outside OSPF domain and inserted with \"redistribute\" command with type 1 (additive) metric\n* NSSA type 1 (O N1) - originated outside OSPF domain and inserted with \"redistribute\" command in NSSA area with type 1 (additive) metric\n* External type 2 (O E2) - originated outside OSPF domain and inserted with \"redistribute\" command with type 2 (fixed) metric\n* NSSA type 2 (O N2) - originated outside OSPF domain and inserted with \"redistribute\" command in NSSA area with type 2 (fixed) metric\n\nOrder of route types above also specifies the order of selection if multiple routes are available for the same prefix in the OSPF database.",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPF Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "process",
@@ -11884,27 +11926,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/ospfv3",
             "api_scope_id": "362c08e1e4e80909934abee4cb603c6b4f9b16ea",
             "columns": [
-                "vrf",
-                "external1",
+                "intraArea",
                 "interArea",
+                "sn",
+                "nssaEx1",
                 "siteName",
                 "id",
-                "nssaEx1",
-                "sn",
-                "nssaEx2",
-                "intraArea",
+                "external2",
                 "hostname",
-                "external2"
+                "vrf",
+                "external1",
+                "nssaEx2"
             ],
-            "description": "Open Shortest Path First v3 (OSPFv3) routes summary",
+            "description": "This table covers total number of OSPFv3 routes of each type.\\\nOSPFv3 routing domain can be split into multiple areas. SPF algorithm is run in each area independently, routers in the same OSPFv3 area must share same topology information. Area 0 forms the backbone area interconnecting other (non-zero) areas. Area boundaries are on the routers (each OSPFv3 interface can be in different area).\n\nOSPFv3 route types (\"Network Type\") can be:\n* Intra-Area (O) - originated in local OSPFv3 area by the \"network\" command\n* Inter-Area (O IA) - originated in OSPFv3 area which is not presewnt on local router by the \"network\" command\n* External type 1 (O E1) - originated outside OSPFv3 domain and inserted with \"redistribute\" command with type 1 (additive) metric\n* NSSA type 1 (O N1) - originated outside OSPFv3 domain and inserted with \"redistribute\" command in NSSA area with type 1 (additive) metric\n* External type 2 (O E2) - originated outside OSPFv3 domain and inserted with \"redistribute\" command with type 2 (fixed) metric\n* NSSA type 2 (O N2) - originated outside OSPFv3 domain and inserted with \"redistribute\" command in NSSA area with type 2 (fixed) metric\n\nOrder of route types above also specifies the order of selection if multiple routes are available for the same prefix in the OSPFv3 database.",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPFv3 Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "intraArea",
@@ -11924,25 +11966,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/rip",
             "api_scope_id": "d7c820202fd1854f4bd45067810489e694f1e9c9",
             "columns": [
+                "sn",
                 "siteName",
-                "subnets",
                 "id",
+                "replicates",
+                "subnets",
                 "memory",
-                "overhead",
-                "sn",
-                "networks",
                 "protocol",
-                "vrf",
+                "networks",
                 "hostname",
-                "replicates"
+                "vrf",
+                "overhead"
             ],
             "description": "Routing Information Protocol (RIP) routes summary",
             "method": "post",
             "nested_columns": [],
             "summary": "RIP Protocol Routes Summary",
             "ui_columns": [
                 "hostname",
@@ -11963,26 +12005,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/cluster/srx",
             "api_scope_id": "187d681ac6b407b47f3de45fa632c75311e9f838",
             "columns": [
-                "siteName",
-                "clusterId",
                 "type",
+                "siteName",
+                "sn",
                 "group",
                 "id",
-                "priority",
-                "state",
                 "name",
-                "sn",
-                "hostname"
+                "priority",
+                "clusterId",
+                "hostname",
+                "state"
             ],
-            "description": "Juniper SRX Clusters inventory",
+            "description": "Juniper SRX Cluster is a technology developed by Juniper. It creates one logical networking device with single management from multiple physical units.",
             "method": "post",
             "nested_columns": [],
             "summary": "Juniper SRX Cluster",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "clusterId",
@@ -12001,23 +12043,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/devices",
             "api_scope_id": "cf5fe334d51107ed9476b3f5afbba0f3b2d1c8f1",
             "columns": [
+                "sn",
                 "siteName",
                 "id",
-                "sn",
                 "contextType",
+                "hostname",
                 "contextName",
-                "contextId",
-                "hostname"
+                "contextId"
             ],
-            "description": "",
+            "description": "Logical Devices",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/platforms/devices",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "contextName",
@@ -12034,22 +12076,22 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/neighbors",
             "api_scope_id": "35aef73100f72ab0e0126c96f9b94f9a9bb466f5",
             "columns": [
                 "siteName",
-                "systemId",
-                "holdTime",
+                "sn",
                 "id",
-                "state",
+                "holdTime",
+                "interfaces",
+                "systemId",
                 "level",
-                "sn",
                 "hostname",
-                "interfaces"
+                "state"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "interfaces"
             ],
             "summary": "POST /tables/platforms/fabric-path/neighbors",
@@ -12071,21 +12113,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/routes",
             "api_scope_id": "6a0e223d15246ac72e63254b2cb0ad7769207162",
             "columns": [
-                "siteName",
-                "id",
                 "switchId",
-                "physicalInterfaces",
                 "localId",
+                "siteName",
                 "sn",
+                "id",
                 "subswitchId",
+                "physicalInterfaces",
                 "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "physicalInterfaces"
             ],
@@ -12107,20 +12149,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/summary",
             "api_scope_id": "f83cbf239cf378a0b65d964e461fb71820f0bd4a",
             "columns": [
-                "siteName",
                 "switchesCount",
+                "siteName",
+                "sn",
                 "id",
                 "neighborsCount",
                 "routesCount",
-                "sn",
                 "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/platforms/fabric-path/summary",
             "ui_columns": [
@@ -12139,25 +12181,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/switches",
             "api_scope_id": "6a987ce761acb660c58e8a8afa3a6982b4d986b8",
             "columns": [
+                "switchId",
                 "siteName",
-                "flags",
-                "systemId",
+                "sn",
                 "id",
-                "state",
+                "systemId",
+                "static",
                 "local",
-                "switchId",
-                "sn",
                 "emulatedAnycast",
-                "static",
-                "hostname"
+                "hostname",
+                "state",
+                "flags"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "flags"
             ],
             "summary": "POST /tables/platforms/fabric-path/switches",
@@ -12181,24 +12223,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fex/interfaces",
             "api_scope_id": "e8d8e9697cbb8eb2b52897d2c0aa1c8ed2499dec",
             "columns": [
-                "fexIntName",
-                "fexSn",
                 "siteName",
-                "id",
                 "sn",
-                "hostname",
+                "id",
+                "fexIntName",
+                "intName",
                 "fex",
-                "intName"
+                "hostname",
+                "fexSn"
             ],
-            "description": "Cisco Fabric EXtender (FEX) interfaces inventory",
+            "description": "Cisco Fabric EXtender (FEX) is a technology developed by Cisco. It creates single logical unit out of multiple physical switches (mostly Cisco Nexus).\nIt mimicks modular device with multiple expansion linecards - with the only exception that the modules are outside of the base chassis and could be\nlocated at different physical places. The remote linecard is called FEX - Fabric Extender and is connected to base/parent chassis with metallic or\nfiber cable like if the FEX was connected directly to the bus/fabric of the base/parent device.\n\nThis table lists all interfaces on all FEX modules present in the network.",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco FEX Interfaces",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -12216,21 +12258,21 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/fex/modules",
             "api_scope_id": "e3be061e5ea5e1570781d59f69e82fdcc9577f67",
             "columns": [
                 "model",
                 "parents",
-                "fexId",
-                "id",
                 "sn",
+                "id",
                 "ver",
-                "fex"
+                "fex",
+                "fexId"
             ],
-            "description": "Cisco Fabric EXtender (FEX) modules inventory",
+            "description": "Cisco Fabric EXtender (FEX) is a technology developed by Cisco. It creates single logical unit out of multiple physical switches (mostly Cisco Nexus). It mimicks modular device with multiple expansion linecards - with the only exception that the modules are outside of the base chassis and could be located at different physical places. The remote linecard is called FEX - Fabric Extender and is connected to base/parent chassis with metallic or fiber cable like if the FEX was connected directly to the bus/fabric of the base/parent device.\nThis table lists all FEX modules present in the network.",
             "method": "post",
             "nested_columns": [
                 "parents"
             ],
             "summary": "Cisco FEX Modules",
             "ui_columns": [
                 "fexId",
@@ -12250,25 +12292,25 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/pairs",
             "api_scope_id": "444b1dcf0a46e57d6e98d7bf9499cabea55e6b1b",
             "columns": [
                 "secondaryHostname",
-                "primarySn",
-                "siteName",
-                "primaryLinkIntName",
-                "systemId",
-                "id",
-                "secondaryStatus",
-                "domain",
-                "secondaryLinkIntName",
                 "primaryStatus",
                 "secondarySn",
-                "primaryHostname"
+                "secondaryStatus",
+                "domain",
+                "primaryLinkIntName",
+                "siteName",
+                "id",
+                "systemId",
+                "primarySn",
+                "primaryHostname",
+                "secondaryLinkIntName"
             ],
             "description": "Multi-chassis link aggregation group (MLAG) pairs inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "MLAG Pairs",
             "ui_columns": [
                 "siteName",
@@ -12290,26 +12332,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/peers",
             "api_scope_id": "c319cfac38fbb9ea69aca2ebcb8bd6b85bf09f1b",
             "columns": [
-                "remoteIp",
-                "siteName",
-                "systemId",
                 "type",
-                "id",
-                "linkIntName",
+                "siteName",
                 "sn",
                 "domain",
-                "localIp",
+                "id",
+                "remoteIp",
+                "systemId",
                 "role",
-                "hostname",
-                "status"
+                "status",
+                "linkIntName",
+                "localIp",
+                "hostname"
             ],
             "description": "Multi-chassis link aggregation group (MLAG) peer-links inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "MLAG Peer Links",
             "ui_columns": [
                 "hostname",
@@ -12332,23 +12374,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/switches",
             "api_scope_id": "e3664685096c7786e0d3ffba191e36ba7a5100cc",
             "columns": [
-                "siteName",
-                "systemId",
                 "type",
-                "id",
-                "sn",
+                "siteName",
                 "domain",
+                "sn",
+                "id",
+                "systemId",
                 "hostname"
             ],
-            "description": "Multi-chassis link aggregation group (MLAG) switches inventory",
+            "description": "Devices running multi-chassis link aggregation (including vendor-specific implementations Cisco vPC)",
             "method": "post",
             "nested_columns": [
                 "domain",
                 "systemId"
             ],
             "summary": "MLAG Switches",
             "ui_columns": [
@@ -12367,24 +12409,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/vpc",
             "api_scope_id": "cecba1b8270e3d2ee71559886918522fc8ee42da",
             "columns": [
-                "siteName",
-                "id",
-                "sn",
                 "keepaliveStatus",
                 "domain",
+                "siteName",
+                "sn",
+                "id",
                 "role",
-                "configConsistStatus",
-                "hostname",
+                "status",
                 "intName",
-                "status"
+                "hostname",
+                "configConsistStatus"
             ],
             "description": "Cisco vPC (Virtual Port-Channel) domains and interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco vPC",
             "ui_columns": [
                 "hostname",
@@ -12405,25 +12447,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/poe/devices",
             "api_scope_id": "d5522f6c8199ccf6f7125941ac475625c47f533c",
             "columns": [
-                "siteName",
-                "powerUsedSum",
+                "powerFromPsSum",
                 "operOnCount",
-                "id",
                 "poeDeviceClassMax",
                 "sn",
-                "interfacesCount",
+                "siteName",
+                "id",
+                "powerUsedSum",
                 "hostname",
-                "powerFromPsSum"
+                "interfacesCount"
             ],
-            "description": "Power over Ethernet (PoE) devices inventory",
+            "description": "This table shows the list of all Power over Ethernet (PoE) capable devices in the network.",
             "method": "post",
             "nested_columns": [],
             "summary": "PoE devices",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "interfacesCount",
@@ -12441,29 +12483,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/poe/interfaces",
             "api_scope_id": "a6a18c3800462f8f32e2278c7d9152db25430db8",
             "columns": [
-                "powerUsed",
-                "siteName",
                 "powerFromPs",
-                "id",
-                "powerMax",
-                "powerGranted",
-                "sn",
-                "admin",
                 "poeDeviceName",
-                "poeDeviceClass",
+                "sn",
                 "oper",
+                "powerMax",
+                "id",
+                "siteName",
+                "powerGranted",
+                "intName",
                 "hostname",
-                "intName"
+                "poeDeviceClass",
+                "powerUsed",
+                "admin"
             ],
-            "description": "Power over Ethernet (PoE) interfaces inventory",
+            "description": "This table shows the list of all Power over Ethernet (PoE) capable ports in the network and the status of devices powered on those ports.",
             "method": "post",
             "nested_columns": [],
             "summary": "PoE Interfaces",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -12485,24 +12527,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/poe/modules",
             "api_scope_id": "ec2a43566668c0449697b7c964d76d2ca20215fd",
             "columns": [
-                "wattsRemaining",
-                "siteName",
                 "wattsAvailable",
-                "id",
-                "wattsUsed",
+                "siteName",
                 "sn",
+                "id",
                 "wattsUsedPct",
-                "moduleId",
                 "isPoE",
-                "hostname"
+                "wattsRemaining",
+                "hostname",
+                "moduleId",
+                "wattsUsed"
             ],
             "description": "Power over Ethernet (PoE) and associated device modules inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "PoE - Device Modules",
             "ui_columns": [
                 "hostname",
@@ -12523,24 +12565,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/stack",
             "api_scope_id": "da7ed9e38b0603a54f286215468a90798f076010",
             "columns": [
-                "master",
-                "siteName",
+                "sn",
                 "connectionsCount",
+                "siteName",
                 "id",
-                "uptimeDiff",
+                "uptimeLow",
                 "membersCount",
-                "sn",
-                "uptimeLow"
+                "uptimeDiff",
+                "master"
             ],
-            "description": "Discovered switch stacks, number of members in each stack, and the total number of stack ports",
+            "description": "Stacking is proprietary technology which creates a single logical network device out of multiple standalone physical switches. This table shows all discovered switch stacks, number of members in each stack, and the total number of stack ports.",
             "method": "post",
             "nested_columns": [],
             "summary": "Switch stacks",
             "ui_columns": [
                 "master",
                 "siteName",
                 "membersCount",
@@ -12557,27 +12599,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/stack/connections",
             "api_scope_id": "f94f12a874c98dc87364fc2b3274d4663aebac6a",
             "columns": [
-                "membersKnownCount",
-                "master",
+                "sn",
                 "siteName",
-                "stackPort",
                 "id",
+                "interfaces",
+                "membersKnownCount",
+                "status",
                 "membersCount",
-                "sn",
-                "member",
+                "stackPort",
                 "neiSwitchId",
-                "interfaces",
-                "status"
+                "member",
+                "master"
             ],
-            "description": "Switch stack interfaces and their current state",
+            "description": "This table shows all switch stack interfaces and their current state.",
             "method": "post",
             "nested_columns": [
                 "interfaces"
             ],
             "summary": "Stack Ports",
             "ui_columns": [
                 "master",
@@ -12599,31 +12641,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/stack/members",
             "api_scope_id": "07dd88ff9bfac76fd033ed2652b9959d4350972f",
             "columns": [
-                "master",
-                "image",
-                "siteName",
-                "pn",
+                "hwVer",
+                "memberSn",
+                "sn",
                 "connectionsCount",
+                "siteName",
                 "id",
-                "memberSn",
-                "state",
+                "pn",
+                "role",
+                "image",
+                "ver",
                 "uptime",
-                "sn",
                 "member",
-                "hwVer",
-                "ver",
-                "role",
-                "mac"
+                "mac",
+                "state",
+                "master"
             ],
-            "description": "Stack members and their current state",
+            "description": "This table shows all individual stack members and their current state.",
             "method": "post",
             "nested_columns": [],
             "summary": "Stack Members",
             "ui_columns": [
                 "master",
                 "siteName",
                 "uptime",
@@ -12647,24 +12689,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/vdc/devices",
             "api_scope_id": "d94e8955d01b0b4503056bcf1a4e535aaca43fe3",
             "columns": [
-                "siteName",
                 "rd",
-                "id",
                 "snHw",
-                "sn",
                 "stpDomain",
+                "sn",
+                "siteName",
+                "id",
                 "vdcId",
                 "hostname"
             ],
-            "description": "Cisco Virtual Device Context (VDC) devices inventory",
+            "description": "Cisco Virtual Device Context (VDC) is a virtualization technology developed by Cisco. It creates multiple logical switches on single piece of hardware (mostly Cisco Nexus switches)",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco VDC Devices",
             "ui_columns": [
                 "siteName",
                 "rd",
                 "stpDomain",
@@ -12681,26 +12723,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/vss/chassis",
             "api_scope_id": "021e079d6db2f173e8722e92c09e815b79a668f0",
             "columns": [
+                "chassisSn",
                 "chassisId",
+                "currentStateTime",
                 "siteName",
-                "controlState",
+                "sn",
                 "id",
-                "state",
                 "version",
-                "sn",
-                "slot",
+                "controlState",
                 "fabricState",
                 "hostname",
-                "chassisSn",
-                "currentStateTime"
+                "slot",
+                "state"
             ],
             "description": "Cisco Virtual Switching System (VSS) chassis information overview",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco VSS Chassis",
             "ui_columns": [
                 "hostname",
@@ -12723,24 +12765,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/vss/overview",
             "api_scope_id": "5ad3125d271b5320330be789aa30df1ff8983807",
             "columns": [
+                "switchId",
                 "siteName",
-                "configuredRedundancyMode",
+                "sn",
                 "id",
-                "switchId",
+                "switchoverReason",
                 "peerSwitchId",
+                "hostname",
+                "configuredRedundancyMode",
                 "operatingRedundancyMode",
-                "sn",
-                "domainNumber",
-                "switchoverReason",
-                "hostname"
+                "domainNumber"
             ],
             "description": "Cisco Virtual Switching System (VSS) protocol overview",
             "method": "post",
             "nested_columns": [],
             "summary": "Cisco VSS Overview",
             "ui_columns": [
                 "hostname",
@@ -12762,20 +12804,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/platforms/vss/vsl",
             "api_scope_id": "c9e20e6789632450df1a0b2a834e16eec52b5d64",
             "columns": [
                 "siteName",
-                "flags",
-                "portChannel",
-                "id",
                 "sn",
+                "id",
                 "portList",
-                "hostname"
+                "hostname",
+                "portChannel",
+                "flags"
             ],
             "description": "Cisco virtual switch link (VSL) overview",
             "method": "post",
             "nested_columns": [
                 "flags",
                 "portList"
             ],
@@ -12797,21 +12839,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/policies",
             "api_scope_id": "f7e39c75db2bf6e5b61c52246ff3dd0da8207890",
             "columns": [
                 "apiScopeIds",
-                "scopeType",
-                "id",
-                "name",
                 "attributeFilters",
+                "id",
+                "isSystem",
                 "attributeScopeIds",
-                "description",
-                "isSystem"
+                "name",
+                "scopeType",
+                "description"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "apiScopeIds",
                 "attributeScopeIds"
             ],
@@ -12835,30 +12877,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/marking",
             "api_scope_id": "8e867f17d7bc390ac2617361dd25bac7f62a74cb",
             "columns": [
-                "siteName",
+                "packets",
                 "parentPolicy",
+                "policy",
                 "type",
+                "siteName",
+                "sn",
                 "id",
+                "match",
                 "childPolicy",
-                "sn",
-                "packets",
+                "intName",
+                "hostname",
                 "set",
-                "class",
-                "match",
                 "value",
-                "hostname",
-                "policy",
-                "intName"
+                "class"
             ],
-            "description": "Quality of Service (QoS) marking policies",
+            "description": "The table shows details of every class with a Quality of Service (QoS) marking action and the specific marking parameters of that class.",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Marking",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "policy",
@@ -12881,37 +12923,37 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/policing",
             "api_scope_id": "aae6de361822629184e1caea9e9db97574b83bd9",
             "columns": [
+                "parentPolicy",
                 "type",
-                "id",
-                "policeType",
-                "exceededBytes",
+                "siteName",
+                "sn",
+                "exceededPkts",
+                "match",
+                "childPolicy",
                 "policy",
+                "conformedBps",
+                "action",
                 "intName",
-                "cir",
-                "match",
-                "class",
-                "conformedPkts",
                 "hostname",
+                "conformedPkts",
                 "bc",
-                "sn",
-                "childPolicy",
-                "exceededPkts",
-                "conformedBps",
-                "siteName",
-                "parentPolicy",
+                "exceededBps",
+                "exceededBytes",
+                "policeType",
+                "cir",
+                "id",
                 "conformedBytes",
-                "action",
-                "exceededBps"
+                "class"
             ],
-            "description": "Quality of Service (QoS) policing rules'",
+            "description": "The table shows details of every class with a policing action and the specific policing parameters of that class.",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Policing",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -12941,32 +12983,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/policy-maps",
             "api_scope_id": "c5c1ff8b85866f16e4fb1b1b1164ce48338d4653",
             "columns": [
-                "siteName",
+                "packets",
                 "parentPolicy",
-                "rateDrop",
+                "policy",
                 "type",
-                "id",
-                "rateInterval",
-                "childPolicy",
-                "rateOffered",
+                "siteName",
                 "sn",
-                "packets",
-                "class",
+                "id",
                 "match",
-                "policy",
-                "hostname",
+                "childPolicy",
+                "rateDrop",
+                "intName",
+                "rateInterval",
                 "bytes",
-                "intName"
+                "hostname",
+                "rateOffered",
+                "class"
             ],
-            "description": "Quality of Service (QoS) applied service policies to interfaces",
+            "description": "The table shows details of every class of every applied service policy to an interface from every managed network devices. Each line represents an active class, which can be searched by the offered or drop rates, the matching parameters of the class, or the parent policy",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Applied Service-Policies",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -12991,29 +13033,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/priority-queuing",
             "api_scope_id": "7f7a72478c960027cff50bf0a3196087f2d2c514",
             "columns": [
-                "siteName",
                 "parentPolicy",
+                "policy",
+                "exDrops",
                 "type",
-                "id",
-                "childPolicy",
+                "siteName",
                 "sn",
-                "strictPriority",
-                "class",
+                "id",
                 "match",
-                "exDrops",
+                "childPolicy",
+                "intName",
                 "hostname",
-                "policy",
-                "intName"
+                "strictPriority",
+                "class"
             ],
-            "description": "Quality of Service (QoS) policies and classes and associated parameters",
+            "description": "The table shows details of every class with a priority action and the specific priority parameters of that class.",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Priority Policies and Classes",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -13035,34 +13077,34 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/queuing",
             "api_scope_id": "c2280632a9e108c34bd95e84cdc4cd78cbd6de05",
             "columns": [
-                "queueDepth",
-                "siteName",
                 "parentPolicy",
+                "policy",
+                "queueDepth",
                 "type",
-                "totalDrops",
-                "pktsOutput",
-                "id",
-                "queueLimit",
-                "bandwidth",
-                "childPolicy",
+                "siteName",
                 "sn",
-                "bytesOutput",
-                "noBufferDrops",
-                "class",
+                "bandwidth",
+                "id",
+                "pktsOutput",
+                "totalDrops",
                 "match",
+                "childPolicy",
+                "intName",
                 "hostname",
-                "policy",
-                "intName"
+                "noBufferDrops",
+                "bytesOutput",
+                "queueLimit",
+                "class"
             ],
-            "description": "Quality of Service (QoS) policy and classes queing parameters",
+            "description": "The table shows details of every class with queuing action and the specific queuing parameters of that class.",
             "method": "post",
             "nested_columns": [
                 "queueLimit"
             ],
             "summary": "QoS Queuing",
             "ui_columns": [
                 "hostname",
@@ -13091,37 +13133,37 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/random-drops",
             "api_scope_id": "aba7749bf3212fffdcf8ffd8aca552af3fe0b33e",
             "columns": [
+                "parentPolicy",
                 "type",
-                "id",
-                "ranDropPkts",
-                "policy",
-                "intName",
-                "minThresh",
-                "transBytes",
-                "class",
-                "hostname",
+                "siteName",
                 "sn",
                 "classRandom",
+                "match",
+                "markProb",
                 "tailDropPkts",
                 "childPolicy",
                 "transPkts",
-                "tailDropBytes",
                 "maxThresh",
-                "markProb",
+                "policy",
+                "minThresh",
+                "intName",
+                "hostname",
+                "tailDropBytes",
                 "ranDropBytes",
-                "siteName",
-                "parentPolicy",
-                "match"
+                "id",
+                "transBytes",
+                "ranDropPkts",
+                "class"
             ],
-            "description": "Inventory of classes with a random early drop detection action and associated parameters",
+            "description": "The table shows details of every class with a random early drop detection action and the specific random drop parameters of that class.\n\n---\n\nWRED - Weighted Random Early Drop Detection",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Classes with Random Drops",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "policy",
@@ -13151,32 +13193,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/qos/shaping",
             "api_scope_id": "63b4f74373646727d5fcd62596386a78ba5414c5",
             "columns": [
-                "be",
-                "siteName",
-                "cir",
                 "parentPolicy",
+                "policy",
+                "shapeType",
                 "type",
-                "targetRate",
-                "id",
-                "childPolicy",
-                "bc",
+                "siteName",
                 "sn",
-                "class",
+                "cir",
+                "id",
+                "be",
+                "targetRate",
                 "match",
-                "shapeType",
+                "bc",
+                "childPolicy",
+                "intName",
                 "hostname",
-                "policy",
-                "intName"
+                "class"
             ],
-            "description": "Quality of Service (QoS) classes and shaping information",
+            "description": "The table shows details of every class with shaping action and the specific parameters of that class.",
             "method": "post",
             "nested_columns": [],
             "summary": "QoS Shaping",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -13201,24 +13243,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/reports/discovery-errors",
             "api_scope_id": "e5974cef09b170765ccc6956db6fd19707d1048f",
             "columns": [
-                "slug",
-                "objectId",
-                "hasLogFile",
-                "id",
-                "errorType",
+                "taskId",
                 "errorText",
+                "id",
                 "loginIp",
                 "version",
-                "taskId",
                 "loginType",
+                "hasLogFile",
+                "slug",
+                "objectId",
+                "errorType",
                 "dnsName"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/reports/discovery-errors",
             "ui_columns": [
@@ -13243,29 +13285,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/reports/discovery-tasks",
             "api_scope_id": "61217b3ed8eaa861461c820cfb09952ed8e74ede",
             "columns": [
-                "slug",
-                "objectId",
-                "hasLogFile",
-                "id",
-                "errorType",
+                "attemptCount",
                 "vendor",
-                "errorMessage",
+                "id",
                 "context",
+                "hasLogFile",
+                "dnsName",
+                "objectId",
+                "ip",
+                "source",
+                "status",
+                "slug",
+                "errorType",
                 "errorReasons",
                 "mac",
-                "source",
-                "ip",
-                "attemptCount",
-                "dnsName",
-                "status"
+                "errorMessage"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "errorReasons"
             ],
             "summary": "POST /tables/reports/discovery-tasks",
@@ -13295,32 +13337,32 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/reports/eof/detail",
             "api_scope_id": "039af94f43c029e25022d25b6076ad7d6638ae62",
             "columns": [
-                "deviceSn",
                 "family",
+                "deviceSn",
+                "endMaintenance",
+                "replacement",
                 "model",
+                "vendor",
                 "siteName",
-                "dscr",
-                "platform",
-                "id",
-                "replacement",
                 "sn",
                 "endSupport",
-                "pid",
-                "url",
+                "id",
+                "platform",
                 "endSale",
+                "dscr",
                 "hostname",
-                "vendor",
-                "endMaintenance"
+                "url",
+                "pid"
             ],
-            "description": "End of Life (EoL) detailed information on all detected part number for managed network devices",
+            "description": "Network infrastructure vendors use end of life milestones to communicate stage of the product lifecycle, allowing sufficient time to migrate to a next generation product. Lifecycle extension beyond end of life defined by vendor is a viable strategy that delivers substantial benefits when risk is managed properly. With proper tools and procedures, network infrastructure equipment can efficiently serve long past official last day of life.",
             "method": "post",
             "nested_columns": [],
             "summary": "Hardware EoL - Detail",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "vendor",
@@ -13345,24 +13387,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/reports/eof/summary",
             "api_scope_id": "61cd2bba1a3963371b948c297d85fe0c4e2758af",
             "columns": [
-                "dscr",
-                "id",
-                "pidCount",
                 "replacement",
+                "endMaintenance",
+                "vendor",
                 "endSupport",
-                "pid",
-                "url",
+                "id",
                 "endSale",
-                "vendor",
-                "endMaintenance"
+                "dscr",
+                "pidCount",
+                "url",
+                "pid"
             ],
             "description": "End of Life (EoL) summary information on all detected part number for managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Hardware EoL - Summary",
             "ui_columns": [
                 "pidCount",
@@ -13415,18 +13457,18 @@
         "post": {
             "api_endpoint": "tables/roles",
             "api_scope_id": "5fedc17c2d4dda62de3bf697f18cabd9179eb0aa",
             "columns": [
                 "policyIds",
                 "type",
                 "id",
+                "isSystem",
                 "name",
                 "isAdmin",
-                "description",
-                "isSystem"
+                "description"
             ],
             "description": "User management roles database used for user management policies",
             "method": "post",
             "nested_columns": [
                 "policyIds"
             ],
             "summary": "RBAC - User Management Roles",
@@ -13448,43 +13490,43 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/bgp/address-families",
             "api_scope_id": "ab00a7512b6b7830cc84b22c3218ba957dc2a35f",
             "columns": [
-                "neiHostname",
                 "type",
-                "id",
+                "neiAs",
+                "siteName",
+                "sn",
+                "neiHostname",
+                "source",
+                "vrf",
                 "keepalive",
-                "neiSiteName",
-                "localAs",
-                "neiSn",
-                "neiDevType",
-                "neiAddress",
                 "family",
-                "localAddress",
-                "localAddressV6",
+                "neiSiteName",
                 "dstInt",
+                "totalReceivedPrefixes",
                 "hostname",
-                "holdTime",
+                "neiAddressV6",
+                "neiDevType",
                 "state",
-                "source",
-                "sn",
-                "totalReceivedPrefixes",
-                "receivedPrefix",
                 "target",
-                "neiAddressV6",
-                "siteName",
+                "localAs",
+                "localId",
+                "neiAddress",
+                "neiSn",
                 "currStateTime",
-                "neiAs",
+                "neiId",
                 "devType",
-                "localId",
-                "vrf",
-                "neiId"
+                "localAddress",
+                "id",
+                "holdTime",
+                "receivedPrefix",
+                "localAddressV6"
             ],
             "description": "Border Gateway Protocol (BGP) and its address-families inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "BGP Address Families",
             "ui_columns": [
                 "hostname",
@@ -13518,46 +13560,46 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/bgp/neighbors",
             "api_scope_id": "dd990ba242bda2a2ae7c32b374007d4118f3d339",
             "columns": [
-                "neiHostname",
                 "type",
-                "id",
+                "neiAs",
+                "siteName",
+                "sn",
+                "neiHostname",
+                "source",
+                "routingPoliciesIn",
+                "vrf",
                 "keepalive",
-                "neiSiteName",
-                "localAs",
-                "neiSn",
-                "neiDevType",
-                "neiAddress",
-                "localAddress",
                 "srcInt",
-                "localAddressV6",
-                "routingPoliciesOut",
+                "neiSiteName",
                 "dstInt",
+                "totalReceivedPrefixes",
                 "hostname",
-                "holdTime",
+                "neiAddressV6",
+                "neiDevType",
                 "state",
-                "routingPoliciesIn",
-                "source",
-                "sn",
-                "totalReceivedPrefixes",
+                "routingPoliciesOut",
                 "target",
-                "neiAddressV6",
-                "siteName",
+                "localAs",
+                "localId",
+                "neiAddress",
+                "neiSn",
                 "currStateTime",
-                "neiAs",
+                "neiId",
                 "devType",
-                "localId",
-                "vrf",
-                "neiId"
+                "localAddress",
+                "id",
+                "holdTime",
+                "localAddressV6"
             ],
-            "description": "Border Gateway Protocol (BGP) neighbors inventory",
+            "description": "BGP Neighbors table contain BGP neighborship relations (adjacencies, peerings) among the BGP routers in the network. BGP adjacency is TCP session formed between the BGP speakers (neighbors, peers)\nAdjacency must be manually configured by entering the neighbors IP address and specifying local Autonomous System Number (ASN) and neighbor ASN.\n\n\"ESTABLISHED\" is the desired state of BGP neighborship. States as \"OPENCONFIRM\", \"OPENSENT\", \"ACTIVE\", \"CONNECT\", \"IDLE\" should be only temporary during network reconvergence or during planned outage.\n\nIf the local and neighbor AS match, it is iBGP - internal BGP session. If the local and neighbor AS does not match it is eBGP - external BGP session. There are different rules on passing prefixes among the BGP neighbors:\n* INTERNAL - prefix learned from internal speaker is passed to extenal BGP speakers but is not passed to another internal BGP speaker\n* EXTERNAL - prefix learned from external speaker is passed to both external and internal BGP speakers\n\nBGP route selection criteria:\n1. Highest WEIGHT (Cisco only parameter)\n1. Highest LOCAL_PREF\n1. Locally originated BGP routes (added via \"network\", \"redistribute\" or \"aggregate\" commands)\n1. Shortest AS_PATH\n1. Lowest ORIGIN type\n1. Lowest MED attribute\n1. Prefer eBGP path over iBGP route\n1. Prefer the path with the lowest IGP metric to the BGP next hop",
             "method": "post",
             "nested_columns": [
                 "routingPoliciesIn",
                 "routingPoliciesOut"
             ],
             "summary": "BGP Neighbors",
             "ui_columns": [
@@ -13594,25 +13636,25 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/eigrp/interfaces",
             "api_scope_id": "89245aacc9087285656253960f60db8626d4c79c",
             "columns": [
                 "siteName",
-                "id",
                 "sn",
+                "id",
+                "localAsn",
                 "timerHold",
+                "intName",
                 "neiCount",
-                "timerHello",
-                "vrf",
                 "hostname",
-                "intName",
-                "localAsn"
+                "vrf",
+                "timerHello"
             ],
-            "description": "Enhanced Interior Gateway Routing Protocol (EIGRP) interfaces inventory",
+            "description": "Enhanced Interior Gateway Routing Protocol (EIGRP) is hybrid distance-vector/link-state dynamic routing protocol. Originally developed by Cisco Systems, is now open standard published in RFC7868.\n\nEIGRP Interfaces shows the list of all router interfaces where the EIGRP is running (eg. interfaces enabled for EIGRP operation).",
             "method": "post",
             "nested_columns": [],
             "summary": "EIGRP Interfaces",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -13631,36 +13673,36 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/eigrp/neighbors",
             "api_scope_id": "b6e85f47108d926ca2d8f766f265e4252b8af2d6",
             "columns": [
+                "siteName",
+                "sn",
                 "neiHostname",
-                "id",
+                "source",
+                "neiIntName",
+                "vrf",
+                "neiAsn",
                 "neiSiteName",
-                "neiSn",
-                "neiDevType",
                 "intName",
-                "localAsn",
-                "neiAddress",
-                "neiIntName",
-                "localAddress",
                 "hostname",
-                "subnet",
-                "source",
-                "sn",
-                "siteName",
+                "neiDevType",
+                "target",
+                "neiAddress",
+                "neiSn",
                 "currStateTime",
+                "subnet",
                 "devType",
-                "neiAsn",
-                "vrf",
-                "target"
+                "localAddress",
+                "id",
+                "localAsn"
             ],
-            "description": "Enhanced Interior Gateway Routing Protocol (EIGRP) neighbors inventory",
+            "description": "Enhanced Interior Gateway Routing Protocol (EIGRP) is hybrid distance-vector/link-state dynamic routing protocol. Originally developed by Cisco Systems, is now open standard published in RFC7868.\n\nEIGRP neighbor table keeps a record of neighborship relations among the EIGRP routers in the network - ie. IP addresses of routers that have a direct L2 connection with this router. Routers that are connected to this router indirectly, through another router, are not recorded in this table as they are not considered neighbors.\n\nWhen a router running EIGRP is connected to another router also running EIGRP, information is exchanged between the two routers. They form a relationship, known as an adjacency. The entire routing table is exchanged between both routers at this time. After the exchange has completed, only differential changes are sent.",
             "method": "post",
             "nested_columns": [],
             "summary": "EIGRP Neighbors",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -13681,27 +13723,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/is-is/interfaces",
             "api_scope_id": "87fea9657fe0ceecd66e5224177421ca1f5ce7d4",
             "columns": [
-                "snpa",
                 "siteName",
-                "circuitType",
-                "circuitLevel",
-                "id",
                 "sn",
-                "levelConfig",
+                "id",
+                "circuitType",
+                "intName",
                 "neiCount",
-                "vrf",
                 "hostname",
-                "intName"
+                "vrf",
+                "circuitLevel",
+                "snpa",
+                "levelConfig"
             ],
-            "description": "Intermediate System to Intermediate System (IS-IS) interfaces inventory",
+            "description": "IS-IS Interfaces shows the list of all router interfaces where the IS-IS is running (eg. where IS-IS Hello packets should be exchanged).\n\nIS-IS routers use IS-IS Hello PDUs to discover their neighbors. All IS-IS routers exchange IS-IS Hello PDUs every 10 seconds by default. Once neighbors are discovered and adjacency is formed, the Hellos act as keepalives to maintain the adjacency and inform changes in the adjacency parameters.\n\nIS-IS Hello PDUs are are of two types depending on the type of network- LAN Hellos and Point-to-point Hellos. LAN Hellos is further divided into L1 and L2 LAN Hellos. L1 LAN Hellos are used by L1 routers on Broadcast network, and L2 LAN Hellos are used by L2 routers on Broadcast network. Point-to-point Hellos are used on non-broadcast media such as point-to-point links, NBMA network, etc. L1 and L2 information is carried in the same point-to-point Hello PDU.\n\nA LAN Hello carries important information like System ID of the router originating the Hello, Priority which is used to elect the Designated IS or DIS (no Backup DIS is elected in IS-IS) and LAN ID which is the System ID of the DR plus one more octet (the Pseudonode ID) to differentiate this LAN ID from another LAN ID that might have the same DR.  It also uses CLV (Code, Length, Value) triplet to carry Area addresses (type 1), IS Neighbors (type 6), Authentication information (type 10), Protocols supported (type 129) and IP Interface address (type 132).\n\nIS-IS Adjacencies can be of 2 Levels:\n* Level-1 - Level-1 adjacencies is formed only between L1 and L1/L2 routers.\n* Level-2 - Level-2 adjacencies is formed only between L2 and L1/L2 routers.",
             "method": "post",
             "nested_columns": [
                 "levelConfig"
             ],
             "summary": "IS-IS Interfaces",
             "ui_columns": [
                 "hostname",
@@ -13722,31 +13764,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/is-is/levels",
             "api_scope_id": "36c54e7ed0ada944d83143b02fce5e1b6e3c5a50",
             "columns": [
-                "localPassive",
                 "localHoldTime",
+                "remoteIntName",
                 "siteName",
-                "localHello",
-                "localPriority",
+                "sn",
                 "id",
-                "state",
                 "localMetric",
-                "remoteSiteName",
                 "remoteHostname",
-                "remoteSn",
-                "sn",
-                "localLevel",
-                "hostname",
+                "localHello",
                 "intName",
-                "remoteMetric",
-                "remoteIntName"
+                "localPassive",
+                "hostname",
+                "remoteSiteName",
+                "localPriority",
+                "localLevel",
+                "state",
+                "remoteSn",
+                "remoteMetric"
             ],
             "description": "Intermediate System to Intermediate System (IS-IS) interface level config",
             "method": "post",
             "nested_columns": [],
             "summary": "IS-IS Levels",
             "ui_columns": [
                 "hostname",
@@ -13771,45 +13813,45 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/is-is/neighbors",
             "api_scope_id": "06df6fbcc2030512927e6815328eefec4f46828f",
             "columns": [
+                "siteName",
+                "sn",
                 "neiHostname",
-                "id",
-                "neiSiteName",
-                "neiSn",
+                "neiIsType",
+                "source",
+                "neiIntName",
+                "neiSnpa",
+                "vrf",
+                "localAreas",
                 "neiSystemName",
-                "neiDevType",
+                "neiSiteName",
                 "intName",
-                "neiAddress",
-                "neiIntName",
-                "localAddress",
-                "localAddressV6",
                 "hostname",
-                "subnet",
+                "neiAddressV6",
+                "neiDevType",
                 "state",
-                "source",
-                "sn",
-                "neiSnpa",
-                "neiAreas",
-                "localIsType",
                 "target",
-                "neiAddressV6",
-                "localAreas",
-                "siteName",
+                "localId",
+                "neiAddress",
+                "neiSn",
                 "currStateTime",
+                "subnet",
+                "neiId",
                 "devType",
-                "localId",
-                "neiIsType",
-                "vrf",
-                "neiId"
+                "localAddress",
+                "localIsType",
+                "id",
+                "localAddressV6",
+                "neiAreas"
             ],
-            "description": "Intermediate System to Intermediate System (IS-IS) neighbors inventory",
+            "description": "IS-IS Neighbors lists all formed IS-IS Adjacencies.\n\nIS-IS routers use IS-IS Hello PDUs to discover their neighbors. All IS-IS routers exchange IS-IS Hello PDUs every 10 seconds by default. Once neighbors are discovered and adjacency is formed, the Hellos act as keepalives to maintain the adjacency and inform changes in the adjacency parameters.\n\nIS-IS Hello PDUs are are of two types depending on the type of network- LAN Hellos and Point-to-point Hellos. LAN Hellos is further divided into L1 and L2 LAN Hellos. L1 LAN Hellos are used by L1 routers on Broadcast network, and L2 LAN Hellos are used by L2 routers on Broadcast network. Point-to-point Hellos are used on non-broadcast media such as point-to-point links, NBMA network, etc. L1 and L2 information is carried in the same point-to-point Hello PDU.\n\nA LAN Hello carries important information like System ID of the router originating the Hello, Priority which is used to elect the Designated IS or DIS (no Backup DIS is elected in IS-IS) and LAN ID which is the System ID of the DR plus one more octet (the Pseudonode ID) to differentiate this LAN ID from another LAN ID that might have the same DR.  It also uses CLV (Code, Length, Value) triplet to carry Area addresses (type 1), IS Neighbors (type 6), Authentication information (type 10), Protocols supported (type 129) and IP Interface address (type 132).\n\nIS-IS Adjacencies can be of 2 Levels:\n* Level-1 - Level-1 adjacencies is formed only between L1 and L1/L2 routers.\n* Level-2 - Level-2 adjacencies is formed only between L2 and L1/L2 routers.",
             "method": "post",
             "nested_columns": [
                 "localAreas",
                 "neiAreas"
             ],
             "summary": "IS-IS Neighbors",
             "ui_columns": [
@@ -13839,22 +13881,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv4-databases",
             "api_scope_id": "94a94b1c9b12da2128990bf5be0eb070341c7ce1",
             "columns": [
-                "siteName",
+                "sn",
                 "ipv4DatabaseServer",
+                "siteName",
                 "id",
-                "state",
                 "instanceId",
-                "sn",
                 "hostname",
-                "ipv6DatabaseServer"
+                "ipv6DatabaseServer",
+                "state"
             ],
             "description": "IPv4 LISP Mapping and Location Repository",
             "method": "post",
             "nested_columns": [],
             "summary": "LISP IPv4 Map Resolvers",
             "ui_columns": [
                 "hostname",
@@ -13873,21 +13915,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv4-routes",
             "api_scope_id": "001289a019fb26a672faf56dabb15568d05efb32",
             "columns": [
+                "eidPrefix",
+                "sn",
                 "siteName",
                 "id",
                 "instanceId",
-                "sn",
-                "registeredIp",
                 "hostname",
-                "eidPrefix"
+                "registeredIp"
             ],
             "description": "IPv4 LISP table, Address mapping and routing",
             "method": "post",
             "nested_columns": [],
             "summary": "LISP IPv4 Routes",
             "ui_columns": [
                 "hostname",
@@ -13905,22 +13947,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv6-databases",
             "api_scope_id": "ebc89ae2d2a9b56d704f231e22c958e0c6364cd2",
             "columns": [
-                "siteName",
+                "sn",
                 "ipv4DatabaseServer",
+                "siteName",
                 "id",
-                "state",
                 "instanceId",
-                "sn",
                 "hostname",
-                "ipv6DatabaseServer"
+                "ipv6DatabaseServer",
+                "state"
             ],
             "description": "IPv6 LISP Mapping and Location Repository",
             "method": "post",
             "nested_columns": [],
             "summary": "LISP IPv6 Map Resolvers",
             "ui_columns": [
                 "hostname",
@@ -13939,21 +13981,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv6-routes",
             "api_scope_id": "a83be2b9707e15fbb5b8e2c616a10b2f91bb841a",
             "columns": [
+                "eidPrefix",
+                "sn",
                 "siteName",
                 "id",
                 "instanceId",
-                "sn",
-                "registeredIp",
                 "hostname",
-                "eidPrefix"
+                "registeredIp"
             ],
             "description": "IPv6 LISP table, Address mapping and routing",
             "method": "post",
             "nested_columns": [],
             "summary": "LISP IPv6 Routes",
             "ui_columns": [
                 "hostname",
@@ -13971,35 +14013,35 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf-v3/interfaces",
             "api_scope_id": "8f6d2fe138d03dac5eda01f1c8263d3638141228",
             "columns": [
-                "id",
-                "priority",
-                "cost",
-                "timerRetransmit",
-                "processId",
-                "intName",
-                "area",
+                "siteName",
+                "instanceId",
+                "sn",
+                "timerDead",
                 "networkType",
-                "timerHello",
+                "timerRetransmit",
                 "timerWait",
+                "cost",
+                "priority",
+                "intName",
+                "neiCount",
                 "hostname",
-                "routerId",
+                "timerHello",
                 "state",
-                "sn",
+                "routerId",
+                "processId",
+                "id",
                 "addressFamily",
-                "siteName",
-                "timerDead",
-                "instanceId",
-                "neiCount"
+                "area"
             ],
-            "description": "Open Shortest Path First v3 (OSPFv3) interfaces inventory",
+            "description": "OSPF Interfaces shows the list of all router interfaces where the OSPF is running (eg. where OSPF LSA routing updates should be exchanged).\n\nOSPF Interface types (\"Network Type\") can be:\n* BROADCAST - in multiaccess networks such as Ethernet where more than 2 OSPF peers may exist on single link\n* NBMA - in multiaccess networks, but without the broadcast capability such as ATM networks, neighbors must be manually specified\n* POINT_TO_POINT (PTP) - on links there only 2 OSPF peers may exist\n* POINT_TO_MULTIPOINT (P2MP) - on links where selected devices (hubs) can discover and communciate with all OSPF speakers on the link such as Frame Relay. Other devices must communicate to the other peers via the hub router. Hub can broadcast hello packets to all routers.\n* POINT_TO_MULTIPOINT NBMA - same as P2MP but neighbors must be manually specified (broadcast is not available on the hub)\n* LOOPBACK - for loopback interfaces only",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPF v3 Interfaces",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -14027,44 +14069,44 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf-v3/neighbors",
             "api_scope_id": "c31a9db0e79d5d487e0f933cf5d04a1bc755384e",
             "columns": [
+                "siteName",
+                "sn",
                 "neiHostname",
+                "source",
+                "neiIntName",
+                "vrf",
+                "neiSiteName",
                 "localCost",
-                "id",
                 "priority",
-                "neiSiteName",
-                "neiSn",
-                "neiDevType",
                 "intName",
-                "neiAddress",
-                "neiIntName",
-                "localAddress",
-                "neiCost",
                 "hostname",
-                "dr",
-                "subnet",
+                "neiDevType",
                 "state",
-                "source",
-                "neiArea",
-                "sn",
                 "target",
-                "addressFamily",
-                "siteName",
+                "bdr",
+                "neiAddress",
+                "neiSn",
                 "currStateTime",
-                "localArea",
+                "subnet",
+                "neiId",
                 "devType",
-                "bdr",
-                "vrf",
-                "neiId"
+                "localAddress",
+                "id",
+                "addressFamily",
+                "neiArea",
+                "localArea",
+                "neiCost",
+                "dr"
             ],
-            "description": "Open Shortest Path First v3 (OSPFv3) neighbors inventory",
+            "description": "OSPF Neighbors table contains neighborship relations (adjacencies) among the OSPF routers in the network. Only routers that has formed OSPF adjancency\ncan exchange LSA messages. Adjacency can be formed automatically by detecting OSPF hello packets from neighbor and responding to them or by manually\nentering the neighbors IP address.\n\nFULL is the desired state of OSPF neighborship. States as 2WAY,DOWN or EXSTSART should be only temporary during network reconvergence.\n\nOn multiaccess links, the DR is Designated Router, BDR is Backup Designated Router (it should replace the DR in case the DR fail) and DROTHER is not\nneither DR nor BDR. Only DRs and BDRs actively exchange routing information with all OSPF routers on the link. DROTHERs still send hello packets to\nall OSPF routers (224.0.0.5), but the routing update is sent only to 224.0.0.6 - only DRs and BDRs listen to this multicast group. All routers should\nform neighborship to DR and BDR. DR and BDR also form adjacency to each other.\nDuring the DR/BDR election, Router Priority and Router ID is used (the higher the better). OSPF is not preemptive so early birds may become the DR\neven though they have lower priorities or IDs.\\\nOn point-to-point links there is no DR election and dash symbol \"-\" is displayed in the \"State Column\".",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPF v3 Neighbors",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -14093,33 +14135,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf/interfaces",
             "api_scope_id": "84f41fd8a870c5a4d9dc9f88417e59666c493b9a",
             "columns": [
+                "timerWait",
+                "processId",
+                "timerHello",
                 "siteName",
-                "routerId",
-                "timerDead",
-                "area",
+                "sn",
                 "id",
+                "timerDead",
                 "priority",
-                "state",
-                "timerRetransmit",
-                "timerHello",
-                "sn",
                 "networkType",
-                "processId",
+                "intName",
+                "area",
+                "hostname",
                 "neiCount",
+                "timerRetransmit",
                 "cost",
-                "timerWait",
-                "hostname",
-                "intName"
+                "routerId",
+                "state"
             ],
-            "description": "Open Shortest Path First (OSPF) interfaces inventory",
+            "description": "OSPF Interfaces shows the list of all router interfaces where the OSPF is running (eg. where OSPF LSA routing updates should be exchanged).\n\nOSPF Interface types (\"Network Type\") can be:\n* BROADCAST - in multiaccess networks such as Ethernet where more than 2 OSPF peers may exist on single link\n* NBMA - in multiaccess networks, but without the broadcast capability such as ATM networks, neighbors must be manually specified\n* POINT_TO_POINT (PTP) - on links there only 2 OSPF peers may exist\n* POINT_TO_MULTIPOINT (P2MP) - on links where selected devices (hubs) can discover and communciate with all OSPF speakers on the link such as Frame Relay. Other devices must communicate to the other peers via the hub router. Hub can broadcast hello packets to all routers.\n* POINT_TO_MULTIPOINT NBMA - same as P2MP but neighbors must be manually specified (broadcast is not available on the hub)\n* LOOPBACK - for loopback interfaces only",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPF Interfaces",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -14145,43 +14187,43 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf/neighbors",
             "api_scope_id": "7937e1737301106eca31020b0c44947fa0eabf0e",
             "columns": [
+                "siteName",
+                "sn",
                 "neiHostname",
+                "source",
+                "neiIntName",
+                "vrf",
+                "neiSiteName",
                 "localCost",
-                "id",
                 "priority",
-                "neiSiteName",
-                "neiSn",
-                "neiDevType",
                 "intName",
-                "neiAddress",
-                "neiIntName",
-                "localAddress",
-                "neiCost",
                 "hostname",
-                "dr",
-                "subnet",
+                "neiDevType",
                 "state",
-                "source",
-                "neiArea",
-                "sn",
                 "target",
-                "siteName",
+                "bdr",
+                "neiAddress",
+                "neiSn",
                 "currStateTime",
-                "localArea",
+                "subnet",
+                "neiId",
                 "devType",
-                "bdr",
-                "vrf",
-                "neiId"
+                "localAddress",
+                "id",
+                "neiArea",
+                "localArea",
+                "neiCost",
+                "dr"
             ],
-            "description": "Open Shortest Path First (OSPF) neighbors inventory",
+            "description": "OSPF Neighbors table contains neighborship relations (adjacencies) among the OSPF routers in the network. Only routers that has formed OSPF adjancency\ncan exchange LSA messages. Adjacency can be formed automatically by detecting OSPF hello packets from neighbor and responding to them or by manually\nentering the neighbors IP address.\n\nFULL is the desired state of OSPF neighborship. States as 2WAY,DOWN or EXSTSART should be only temporary during network reconvergence.\n\nOn multiaccess links, the DR is Designated Router, BDR is Backup Designated Router (it should replace the DR in case the DR fail) and DROTHER is not\nneither DR nor BDR. Only DRs and BDRs actively exchange routing information with all OSPF routers on the link. DROTHERs still send hello packets to\nall OSPF routers (224.0.0.5), but the routing update is sent only to 224.0.0.6 - only DRs and BDRs listen to this multicast group. All routers should\nform neighborship to DR and BDR. DR and BDR also form adjacency to each other.\\\nDuring the DR/BDR election, Router Priority and Router ID is used (the higher the better). OSPF is not preemptive so early birds may become the DR\neven though they have lower priorities or IDs.\\\nOn point-to-point links there is no DR election and dash symbol \"-\" is displayed in the \"State Column\".",
             "method": "post",
             "nested_columns": [],
             "summary": "OSPF Neighbors",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -14209,28 +14251,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/rip/interfaces",
             "api_scope_id": "e13369c009bcf86cf61f1ac3b5c60d1eb15204c7",
             "columns": [
-                "timerHolddown",
-                "siteName",
                 "timerUpdate",
                 "verReceive",
-                "verSend",
-                "timerInvalid",
-                "id",
+                "siteName",
                 "sn",
+                "id",
+                "timerHolddown",
+                "intName",
                 "neiCount",
                 "hostname",
-                "intName",
-                "timerFlush"
+                "timerInvalid",
+                "timerFlush",
+                "verSend"
             ],
-            "description": "Routing Information Protocol (RIP) interfaces inventory",
+            "description": "Routing Information Protocol (RIP) is the distance-vector dynamic routing protocol implementing hop count as routing metric. RIP version 1 and 2 are for IPv4, RIPng is for IPv6. Maximum hop count is 15, hop count of 16 marks unavailable destination.\n\nRIP Interfaces shows the list of all router interfaces where the RIP is running (eg. where RIP routing updates should be exchanged), and the number of neighbors connected through the interface.\n\nThe routing information protocol uses the following timers as part of its operation:\n* UPDATE TIMER - controls the interval between two gratuitous RIP Request messages. By default the value is 30 seconds. The RIP Request message is broadcasted to all its RIP enabled interfaces\n* INVALID TIMER - The invalid timer specifies how long a routing entry can be in the routing table without being updated. This is also called as expiration Timer. By default, the value is 180 seconds. After the timer expires the hop count of the routing entry will be set to 16, marking the destination as unreachable\n* HOLDDOWN TIMER - The hold-down timer is started per route entry, when the hop count is changing from lower value to higher value. This allows the route to get stabilized. During this time no update can be done to that routing entry. The default value of this timer is 180 seconds\n* FLUSH TIMER - The flush timer controls the time between the route is invalidated or marked as unreachable and removal of entry from the routing table. By default the value is 240 seconds. This is 60 seconds longer than Invalid timer. So for 60 seconds the router will be advertising about this unreachable route to all its neighbours. This timer must be set to a higher value than the invalid timer",
             "method": "post",
             "nested_columns": [],
             "summary": "RIP Interfaces",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -14251,34 +14293,34 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/rip/neighbors",
             "api_scope_id": "9a0af78f7deea13b3f3ab3a8e232d40a9929718a",
             "columns": [
-                "neiHostname",
-                "neiAddress",
-                "neiIntName",
-                "currStateTime",
+                "target",
                 "localAddress",
-                "siteName",
-                "id",
                 "neiSiteName",
-                "devType",
-                "source",
+                "siteName",
                 "sn",
+                "id",
+                "neiAddress",
+                "neiHostname",
                 "neiSn",
-                "target",
-                "neiDevType",
-                "vrf",
+                "source",
+                "neiIntName",
+                "intName",
+                "currStateTime",
                 "hostname",
                 "subnet",
-                "intName"
+                "vrf",
+                "devType",
+                "neiDevType"
             ],
-            "description": "Routing Information Protocol (RIP) neighbors inventory",
+            "description": "Routing Information Protocol (RIP) is the distance-vector dynamic routing protocol implementing hop count as routing metric. RIP version 1 and 2 are for IPv4, RIPng is for IPv6. Maximum hop count is 15, hop count of 16 marks unavailable destination.\n\nTable presents information about all RIP sources, which can be considered as neighbors. RIP routing protocol does not establish sessions and simply listens for incoming updates on UDP port 520. RIP Neighbors table can be used to verify presence or absence of RIP routing information source.",
             "method": "post",
             "nested_columns": [],
             "summary": "RIP Neighbors",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -14296,17 +14338,17 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/scopes/api",
             "api_scope_id": "751705d05842f7c672be15f08a3b6b124f353c3a",
             "columns": [
+                "id",
                 "method",
-                "path",
-                "id"
+                "path"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/scopes/api",
             "ui_columns": [
                 "id",
@@ -14346,26 +14388,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/sdwan/links",
             "api_scope_id": "4373ef2e727cfd894d709e6ee1c2adebc37299e2",
             "columns": [
-                "slug",
+                "organization",
+                "endpointIp",
+                "sn",
                 "siteName",
                 "port",
-                "endpointIp",
                 "id",
-                "encapsulation",
-                "sn",
+                "interfaces",
                 "name",
+                "slug",
+                "encapsulation",
                 "linkName",
-                "organization",
-                "hostname",
-                "interfaces"
+                "hostname"
             ],
             "description": "Versa SD-WAN transport links inventory",
             "method": "post",
             "nested_columns": [
                 "interfaces"
             ],
             "summary": "Versa Transport links",
@@ -14390,25 +14432,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/sdwan/sites",
             "api_scope_id": "434860af8c796bee668e396b23a3800dabe67abc",
             "columns": [
-                "slug",
-                "remoteMgmtIp",
-                "siteName",
+                "organization",
                 "type",
-                "id",
-                "uptime",
                 "sn",
+                "siteName",
+                "id",
                 "name",
-                "organization",
+                "status",
+                "slug",
+                "remoteMgmtIp",
                 "hostname",
-                "status"
+                "uptime"
             ],
             "description": "Versa SD-WAN sites inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Versa Sites",
             "ui_columns": [
                 "hostname",
@@ -14430,26 +14472,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/accounting",
             "api_scope_id": "7d5d6fce92648a1e7036920a8a475acc81b47832",
             "columns": [
-                "siteName",
-                "secondaryMethod",
                 "type",
+                "siteName",
+                "sn",
+                "params",
                 "id",
                 "name",
-                "params",
+                "secondaryMethod",
+                "hostname",
                 "primaryMethod",
-                "sn",
-                "nextMethods",
-                "hostname"
+                "nextMethods"
             ],
-            "description": "Authentication, Authorization and Accounting (AAA) accounting methods configured on managed network devices",
+            "description": "AAA Accounting lists the sequence of all accounting methods configured and applied to the network infrastructure devices.\nGeneral recommendation is to use centralized TACACS and RADIUS servers to log all accounting data for TACACS and RADIUS.",
             "method": "post",
             "nested_columns": [
                 "nextMethods",
                 "params"
             ],
             "summary": "AAA Accounting",
             "ui_columns": [
@@ -14471,26 +14513,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/authentication",
             "api_scope_id": "e2518f971c68f9282fc275f692f077cd22ecbec7",
             "columns": [
-                "siteName",
-                "secondaryMethod",
                 "type",
+                "siteName",
+                "sn",
+                "params",
                 "id",
                 "name",
-                "params",
+                "secondaryMethod",
+                "hostname",
                 "primaryMethod",
-                "sn",
-                "nextMethods",
-                "hostname"
+                "nextMethods"
             ],
-            "description": "Authentication, Authorization and Accounting (AAA) authentication methods configured on managed network devices",
+            "description": "Authentication lists the sequence of all authentication methods configured and applied to the network infrastructure devices.\nGeneral recommendation is to use centralized TACACS and RADIUS servers and not rely on local authentication or even turn it off completely (method none).",
             "method": "post",
             "nested_columns": [
                 "nextMethods",
                 "params"
             ],
             "summary": "AAA Authentication",
             "ui_columns": [
@@ -14512,26 +14554,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/authorization",
             "api_scope_id": "fbcbd2df73f1c55b18116b639ae16d52ae7a45ed",
             "columns": [
-                "siteName",
-                "secondaryMethod",
                 "type",
+                "siteName",
+                "sn",
+                "params",
                 "id",
                 "name",
-                "params",
+                "secondaryMethod",
+                "hostname",
                 "primaryMethod",
-                "sn",
-                "nextMethods",
-                "hostname"
+                "nextMethods"
             ],
-            "description": "Authentication, Authorization and Accounting (AAA) authorization methods configured on managed network devices",
+            "description": "AAA Authorization lists the sequence of all authorization methods configured and applied to the network infrastructure devices.\nGeneral recommendation is to use centralized TACACS and RADIUS servers and not rely on local authorization or even turn it off completely (method none).",
             "method": "post",
             "nested_columns": [
                 "nextMethods",
                 "params"
             ],
             "summary": "AAA Authorization",
             "ui_columns": [
@@ -14553,31 +14595,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/lines",
             "api_scope_id": "23943cd1167404a7fb4c5a3d10da10fece0db4f0",
             "columns": [
-                "authenServiceList",
-                "siteName",
-                "authorServiceList",
+                "outTransports",
+                "inAcl",
                 "type",
-                "outAcl",
+                "siteName",
+                "sn",
                 "id",
+                "authorServiceList",
                 "idList",
                 "inAclAllVrfs",
-                "outTransports",
-                "accntServiceList",
-                "sn",
+                "outAcl",
+                "hostname",
                 "inTransports",
+                "accntServiceList",
                 "idType",
-                "inAcl",
-                "hostname"
+                "authenServiceList"
             ],
-            "description": "Authentication, Authorization and Accounting (AAA) lines configured on managed network devices",
+            "description": "AAA Lines lists all lines (vty, console, aux) configured on the network infrastructure devices, with information about Authentication, Authorization and Accounting policy applied to them.",
             "method": "post",
             "nested_columns": [
                 "inTransports",
                 "outTransports"
             ],
             "summary": "AAA Lines",
             "ui_columns": [
@@ -14603,19 +14645,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/password-strength",
             "api_scope_id": "b0a1aacfd62f7cb433535972f64db404a46146a6",
             "columns": [
+                "sn",
                 "siteName",
                 "id",
-                "sn",
-                "passwordStrengthCheck",
-                "hostname"
+                "hostname",
+                "passwordStrengthCheck"
             ],
             "description": "Inventory of managed network devices with enabled/disabled passowrd strength check",
             "method": "post",
             "nested_columns": [],
             "summary": "Password Strength",
             "ui_columns": [
                 "hostname",
@@ -14631,29 +14673,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/servers",
             "api_scope_id": "bfc77f153b2e7f31ef0423d152543d30a7cfee17",
             "columns": [
-                "dstHostname",
-                "cfgName",
+                "type",
                 "siteName",
                 "port",
-                "type",
-                "id",
-                "srvGroupName",
-                "protocol",
                 "sn",
-                "ip",
+                "id",
                 "srcIp",
+                "ip",
+                "intName",
+                "cfgName",
+                "protocol",
                 "hostname",
-                "intName"
+                "srvGroupName",
+                "dstHostname"
             ],
-            "description": "Authentication, Authorization and Accounting (AAA) configured on managed network devices",
+            "description": "AAA Servers lists all TACACS and RADIUS servers configured on the network infrastructure devices, with detailed information about Server Group name, source interface and IP address used for connecting to the server and destination port.",
             "method": "post",
             "nested_columns": [],
             "summary": "AAA Servers",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "protocol",
@@ -14676,20 +14718,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/aaa/users",
             "api_scope_id": "7efe128b51b65baa80516cf9482b93015424673a",
             "columns": [
                 "siteName",
-                "privilege",
-                "id",
                 "sn",
+                "id",
                 "groups",
                 "hostname",
-                "username"
+                "username",
+                "privilege"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) loca configured on managed network devices",
             "method": "post",
             "nested_columns": [
                 "groups"
             ],
             "summary": "AAA Local Users",
@@ -14709,67 +14751,67 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/acl",
             "api_scope_id": "2d1639f5c081d9043a7416cfc439f2d176a7148a",
             "columns": [
-                "vxlanSrcGrp",
+                "siteName",
+                "uid",
+                "sn",
+                "interfaceIntraZone",
                 "ipTtl",
-                "id",
-                "l4Dst",
-                "tcpFlags",
-                "actionOriginal",
+                "ipFragmentOffset",
+                "policyName",
+                "mplsLabelIn",
+                "ipSrcRegion",
+                "interfaceInZone",
+                "vxlanVni",
+                "ruleNameNumeric",
+                "srcPorts",
                 "udpSrc",
-                "description",
+                "interfaceInterZone",
                 "ipProtocol",
-                "referencedTests",
-                "l4Src",
-                "active",
-                "ipDscp",
-                "l7Application",
-                "ipPacketLength",
                 "icmpType",
-                "ipPrecedence",
-                "mplsLabelIn",
+                "action",
+                "l4Dst",
                 "hostname",
-                "ipTos",
-                "ipSrc",
-                "srcPorts",
-                "policyName",
-                "interfaceOut",
-                "ipSrcRegion",
-                "ipv6Src",
-                "tcpDst",
                 "icmpCode",
+                "tcpFlags",
+                "referencedTests",
+                "ipPrecedence",
                 "ruleName",
-                "interfaceOutZone",
-                "tcpSrc",
-                "optionsTracked",
+                "ipPacketLength",
+                "ipSrc",
+                "icmpIcmpv6",
                 "ipDstRegion",
-                "interfaceIn",
-                "vxlanVni",
-                "others",
-                "vxlanDstGrp",
-                "sn",
-                "udpDst",
-                "interfaceIntraZone",
-                "siteName",
+                "ipTos",
                 "ipv6Dst",
+                "ipDst",
+                "l4Src",
+                "tcpDst",
+                "actionOriginal",
+                "udpDst",
+                "description",
+                "optionsTracked",
+                "interfaceOut",
+                "active",
+                "vxlanSrcGrp",
+                "vxlanDstGrp",
+                "id",
+                "ipDscp",
+                "tcpSrc",
                 "dstPorts",
-                "uid",
-                "icmpIcmpv6",
-                "ipFragmentOffset",
-                "ruleNameNumeric",
+                "interfaceOutZone",
+                "interfaceIn",
+                "l7Application",
+                "ipv6Src",
                 "interfaceVrf",
-                "action",
-                "interfaceInZone",
                 "ruleNumber",
-                "interfaceInterZone",
-                "ipDst"
+                "others"
             ],
             "description": "Detailed network access control list (ACL) information on managed network devices",
             "method": "post",
             "nested_columns": [
                 "interfaceIn",
                 "interfaceOut",
                 "interfaceInZone",
@@ -14857,18 +14899,18 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/acl/global-policies",
             "api_scope_id": "d5d1bac547ea78b54feae7edc6a6f1e6f17b1f65",
             "columns": [
                 "siteName",
+                "sn",
+                "id",
                 "inputPolicy",
                 "outputPolicy",
-                "id",
-                "sn",
                 "hostname"
             ],
             "description": "Global access control list (ACL) policies configured on managed network devices",
             "method": "post",
             "nested_columns": [],
             "summary": "Global ACL policies",
             "ui_columns": [
@@ -14886,23 +14928,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/acl/interfaces",
             "api_scope_id": "a942092c49050b26e00d4de74b495b885caffb97",
             "columns": [
+                "inAcl",
                 "siteName",
-                "outAcl",
-                "id",
                 "sn",
-                "inAcl",
+                "id",
+                "intName",
                 "hostname",
-                "intName"
+                "outAcl"
             ],
-            "description": "Interfaces with packet filters or access control lists (ACL) applied",
+            "description": "IP Access lists applied on all interfaces in the network are shown in this table.\\\nACLs shown in this table are used for packet filtering. If the actual packet header field matches criteria, then the packet is either denied/filtered out or permitted for further transport. Criteria are specified mainly by packet header fields:\n* Network protocol tranported in the packet - mainly IP, TCP or UDP\n* Source IP address and L4 port\n* Destination IP address and L4 port\n---\n\nACE - access control entry: One rule with criteria and action if the criteria are met\\\nACL - access control list: Set of ACEs with same usage in an order specified by sequence numbers (ACEs are interpreted starting with lowest sequence number up to highest one)",
             "method": "post",
             "nested_columns": [
                 "inAcl",
                 "outAcl"
             ],
             "summary": "ACL and Filter Interfaces",
             "ui_columns": [
@@ -14921,24 +14963,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/dhcp/bindings",
             "api_scope_id": "b812b5db4781705202cde2ec12001c2f08806f70",
             "columns": [
-                "leaseTimeout",
-                "siteName",
                 "type",
-                "id",
-                "leaseIp",
+                "siteName",
                 "sn",
+                "id",
+                "intName",
+                "leaseTimeout",
                 "vlanId",
-                "mac",
                 "hostname",
-                "intName"
+                "leaseIp",
+                "mac"
             ],
             "description": "DHCP Snooping binding database inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "DHCP Snooping Binding Database",
             "ui_columns": [
                 "hostname",
@@ -14959,31 +15001,31 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/dhcp/snooping",
             "api_scope_id": "5a9cb46d953e42a28ca098c8264985e8b31b69eb",
             "columns": [
-                "trustedPortList",
-                "dbLocation",
+                "packetsDropped",
+                "dbWriteDelay",
                 "siteName",
-                "circuitId",
-                "remoteId",
-                "insertion",
+                "sn",
                 "id",
+                "untrustedPolicy",
                 "enabled",
-                "vendorId",
-                "packetsDropped",
-                "sn",
+                "insertion",
+                "circuitId",
+                "enabledVlanList",
                 "hostname",
-                "packetsTotal",
+                "dbLocation",
+                "trustedPortList",
                 "macVerification",
-                "untrustedPolicy",
-                "enabledVlanList",
-                "dbWriteDelay"
+                "vendorId",
+                "packetsTotal",
+                "remoteId"
             ],
             "description": "DHCP Snooping configuration parameters for managed network devices",
             "method": "post",
             "nested_columns": [
                 "enabledVlanList",
                 "trustedPortList"
             ],
@@ -15014,26 +15056,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/dmvpn",
             "api_scope_id": "3cdb4dcd074059f66ad395b16f8c998c3d4f836b",
             "columns": [
-                "peerNbma",
                 "siteName",
-                "id",
-                "state",
-                "peerTunnel",
                 "sn",
+                "id",
+                "peerNbma",
                 "time",
-                "hostname",
+                "peerTunnel",
+                "attrb",
                 "intName",
-                "attrb"
+                "hostname",
+                "state"
             ],
-            "description": "dynamic multipoint virtual private network (DMVPN) tunnels inventory ",
+            "description": "DMVPN - Dynamic Multipoint VPN is a Cisco technology used to deploy secure WAN links over public Internet in a scalable manner. IPsec tunnels are dynamically set up from the remote locations (spokes) to HQ locations (VPN hubs).\\\nEach line represents one IPsec tunnel.\n\nTunnels should be in the \"UP\" state. Other states like \"IKE\" or \"NHRP\" should be short-lived only and are not desirable for long periods of time.\\\nUndesirable tunnels are also the ones with \"I\" - incomplete attribute.\n",
             "method": "post",
             "nested_columns": [],
             "summary": "DMVPN Summary",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "intName",
@@ -15052,28 +15094,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/enabled-telnet",
             "api_scope_id": "25300ae072614ab6593ce7189bf2ee5c046fe0a2",
             "columns": [
-                "image",
+                "configReg",
                 "siteName",
+                "sn",
                 "id",
-                "uptime",
                 "loginIp",
-                "processor",
-                "reload",
                 "version",
-                "sn",
                 "loginType",
-                "configReg",
-                "hostname"
+                "image",
+                "hostname",
+                "uptime",
+                "processor",
+                "reload"
             ],
-            "description": "Managed network devices with enabled Telnet access",
+            "description": "The table presents managed devices where telnet protocol is enabled.\n\nClear text management protocol is considered a security violation by many governmental and industrial regulations. While limited use of telnet can be acceptable under certain circumstances, such as restricted use only to specific management subnets, it is highly recommended to migrate to SSH protocol for management command line access.\n\nThis table should be empty.\n",
             "method": "post",
             "nested_columns": [],
             "summary": "Telnet Access",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "sn",
@@ -15095,43 +15137,43 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/ipsec/gateways",
             "api_scope_id": "59c972df31071ad177740ebaf89adcaea46b6ad4",
             "columns": [
-                "peerId",
-                "profileName",
-                "remoteGwAddressV6",
+                "remoteGwAddress",
                 "type",
+                "siteName",
+                "sn",
+                "mode",
+                "role",
+                "dhGroup",
+                "localGwAddress",
                 "natTraversal",
-                "id",
-                "version",
-                "intName",
-                "keyLifeBytes",
                 "neighbors",
-                "remoteGwAddress",
-                "deadPeerDetection",
+                "remoteGwAddressV6",
+                "status",
+                "intName",
                 "keyLifeSeconds",
-                "localGwAddressV6",
                 "hostname",
-                "sn",
-                "dhGroup",
-                "encryption",
-                "status",
-                "siteName",
                 "intDscr",
-                "mode",
+                "peerId",
                 "localId",
-                "authType",
                 "authentication",
-                "localGwAddress",
-                "role"
+                "profileName",
+                "authType",
+                "localGwAddressV6",
+                "id",
+                "version",
+                "encryption",
+                "keyLifeBytes",
+                "deadPeerDetection"
             ],
-            "description": "Internet Protocol Security (IPsec) gateways inventory",
+            "description": "Table contains IKE phase 1 tunnels. Purpose of IKE phase 1 is establish a secure authenticated communication channel to generate a shared secret key to encrypt further IKE communications (IPsec phase 2). Some crucial parameters have to match on both sides of connection to establish IKE phase 1:  version, authentication, proposals (encryption, authentication, key exchange).",
             "method": "post",
             "nested_columns": [
                 "neighbors"
             ],
             "summary": "IPsec gateways",
             "ui_columns": [
                 "hostname",
@@ -15169,49 +15211,49 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/ipsec/tunnels",
             "api_scope_id": "257769535da11554fef989811dcc6fdab52d2780",
             "columns": [
-                "remoteGwAddressV6",
-                "profileName",
-                "id",
                 "selectorRemoteAddress",
+                "remoteGwAddress",
+                "siteName",
+                "sn",
+                "encapsulation",
+                "dhGroup",
+                "localGwAddress",
                 "selectorRemoteAddressV6",
-                "selectorRemotePort",
-                "protocol",
+                "selectorLocalPort",
                 "ikeGateway",
-                "intName",
-                "keepAlive",
-                "keyLifeBytes",
                 "neighbors",
-                "routeBased",
-                "remoteGwAddress",
+                "remoteGwAddressV6",
+                "status",
                 "selectorProtocol",
-                "encapsulation",
                 "selectorLocalAddressV6",
+                "intName",
                 "keyLifeSeconds",
-                "localGwAddressV6",
-                "selectorLocalAddress",
                 "hostname",
-                "tunnelIntDscr",
-                "tunnelIntName",
-                "sn",
-                "dhGroup",
-                "autoUp",
-                "encryption",
-                "status",
-                "siteName",
+                "protocol",
+                "selectorRemotePort",
                 "intDscr",
-                "selectorLocalPort",
+                "autoUp",
+                "routeBased",
                 "authentication",
-                "localGwAddress"
+                "keepAlive",
+                "tunnelIntName",
+                "profileName",
+                "localGwAddressV6",
+                "id",
+                "tunnelIntDscr",
+                "encryption",
+                "selectorLocalAddress",
+                "keyLifeBytes"
             ],
-            "description": "Internet Protocol Security (IPsec) tunnels inventory",
+            "description": "Table contains IKE phase 2 tunnels (IPsec tunnels), which can protect data communication. IPsec tunnels can leverage two protocols \u2013 AH, ESP. AH offer only authentication and integrity. ESP adds also encryption. Both protocols support two modes \u2013 tunnel, transport. The main difference is that tunnel mode uses new IP header while transport modes use original IP datagram. Traffic selectors define traffic which will be protected. We can forward traffic to tunnel either by routing table (route based vpn) or by firewall policy (policy based vpn). Some crucial parameters have to match on both sides of connection to establish IKE phase 2:  protocol, type, proposals (encryption, authentication, key exchange)",
             "method": "post",
             "nested_columns": [
                 "neighbors"
             ],
             "summary": "IPsec tunnels",
             "ui_columns": [
                 "hostname",
@@ -15255,77 +15297,77 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/nat44",
             "api_scope_id": "4f46b9e59286735d7f4924e8e777c9aa8c55d45c",
             "columns": [
-                "natUdpSrc",
-                "vxlanSrcGrp",
+                "siteName",
+                "uid",
+                "sn",
+                "interfaceIntraZone",
                 "ipTtl",
-                "id",
-                "l4Dst",
-                "tcpFlags",
-                "actionOriginal",
+                "ipFragmentOffset",
+                "policyName",
+                "mplsLabelIn",
+                "ipSrcRegion",
+                "interfaceInZone",
+                "vxlanVni",
+                "ruleNameNumeric",
+                "srcPorts",
+                "natIpSrc",
                 "udpSrc",
-                "description",
+                "natIpDst",
+                "interfaceInterZone",
                 "ipProtocol",
-                "referencedTests",
-                "natTcpDst",
-                "l4Src",
-                "active",
                 "natTcpSrc",
-                "ipDscp",
-                "l7Application",
-                "natL4Src",
-                "natUdpDst",
-                "ipPacketLength",
                 "icmpType",
-                "ipPrecedence",
-                "mplsLabelIn",
+                "action",
+                "l4Dst",
                 "hostname",
-                "ipTos",
-                "ipSrc",
-                "srcPorts",
-                "natIpPortDst",
-                "policyName",
-                "interfaceOut",
-                "ipSrcRegion",
-                "ipv6Src",
-                "tcpDst",
                 "icmpCode",
+                "tcpFlags",
+                "referencedTests",
+                "ipPrecedence",
+                "natL4Dst",
+                "natInterfaceSrc",
                 "ruleName",
-                "natIpSrc",
-                "natIpDst",
-                "interfaceOutZone",
-                "tcpSrc",
-                "optionsTracked",
+                "ipPacketLength",
+                "ipSrc",
+                "icmpIcmpv6",
                 "ipDstRegion",
-                "interfaceIn",
-                "vxlanVni",
-                "others",
-                "vxlanDstGrp",
-                "sn",
-                "udpDst",
-                "interfaceIntraZone",
-                "natInterfaceSrc",
-                "siteName",
+                "ipTos",
                 "ipv6Dst",
+                "ipDst",
+                "l4Src",
+                "tcpDst",
+                "actionOriginal",
+                "natUdpSrc",
+                "udpDst",
+                "natUdpDst",
+                "description",
+                "optionsTracked",
+                "interfaceOut",
+                "active",
+                "vxlanSrcGrp",
+                "vxlanDstGrp",
+                "natTcpDst",
+                "id",
+                "ipDscp",
+                "tcpSrc",
                 "dstPorts",
-                "natL4Dst",
-                "uid",
-                "icmpIcmpv6",
-                "ipFragmentOffset",
-                "ruleNameNumeric",
+                "interfaceOutZone",
+                "natIpPortDst",
+                "interfaceIn",
+                "natL4Src",
+                "l7Application",
+                "ipv6Src",
                 "interfaceVrf",
-                "action",
-                "interfaceInZone",
                 "ruleNumber",
-                "interfaceInterZone",
-                "ipDst"
+                "others"
             ],
             "description": "Network Address Translation (IPv4 to IPv4)",
             "method": "post",
             "nested_columns": [
                 "interfaceIn",
                 "interfaceOut",
                 "interfaceInZone",
@@ -15426,22 +15468,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/object-groups",
             "api_scope_id": "88eb193dff9b57233051128d0bb232b199f8183c",
             "columns": [
-                "isLiteralValue",
                 "siteName",
+                "sn",
                 "id",
                 "name",
-                "sn",
                 "category",
-                "value",
+                "isLiteralValue",
                 "hostname",
+                "value",
                 "description"
             ],
             "description": "Security object groups and address books inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "Security Object Groups",
             "ui_columns": [
@@ -15464,69 +15506,69 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/pbr",
             "api_scope_id": "07257c90ff5755111ebd4cc5599ade3c49faff28",
             "columns": [
-                "vxlanSrcGrp",
+                "siteName",
+                "uid",
+                "sn",
+                "interfaceIntraZone",
                 "ipTtl",
-                "id",
-                "l4Dst",
-                "tcpFlags",
-                "actionOriginal",
+                "ipFragmentOffset",
+                "policyName",
+                "mplsLabelIn",
+                "ipSrcRegion",
+                "interfaceInZone",
+                "vxlanVni",
+                "pbrActions",
+                "ruleNameNumeric",
+                "srcPorts",
                 "udpSrc",
-                "description",
+                "interfaceInterZone",
                 "ipProtocol",
-                "referencedTests",
-                "l4Src",
-                "active",
-                "ipDscp",
-                "l7Application",
-                "ipPacketLength",
                 "icmpType",
-                "ipPrecedence",
-                "mplsLabelIn",
-                "pbrActions",
+                "action",
+                "l4Dst",
                 "hostname",
-                "ipTos",
-                "ipSrc",
-                "srcPorts",
-                "policyName",
-                "interfaceOut",
-                "ipSrcRegion",
-                "ipv6Src",
-                "tcpDst",
                 "icmpCode",
+                "tcpFlags",
+                "referencedTests",
+                "ipPrecedence",
                 "ruleName",
-                "interfaceOutZone",
-                "tcpSrc",
-                "optionsTracked",
-                "ipDstRegion",
-                "interfaceIn",
-                "vxlanVni",
-                "others",
-                "vxlanDstGrp",
-                "sn",
                 "evalAclTests",
-                "udpDst",
-                "interfaceIntraZone",
-                "siteName",
+                "ipPacketLength",
+                "ipSrc",
+                "icmpIcmpv6",
+                "ipDstRegion",
+                "ipTos",
                 "ipv6Dst",
+                "ipDst",
+                "l4Src",
+                "tcpDst",
+                "actionOriginal",
+                "udpDst",
+                "description",
+                "optionsTracked",
+                "interfaceOut",
+                "active",
+                "vxlanSrcGrp",
+                "vxlanDstGrp",
+                "id",
+                "ipDscp",
+                "tcpSrc",
                 "dstPorts",
-                "uid",
-                "icmpIcmpv6",
-                "ipFragmentOffset",
-                "ruleNameNumeric",
+                "interfaceOutZone",
+                "interfaceIn",
+                "l7Application",
+                "ipv6Src",
                 "interfaceVrf",
-                "action",
-                "interfaceInZone",
                 "ruleNumber",
-                "interfaceInterZone",
-                "ipDst"
+                "others"
             ],
             "description": "Policy Based Routing (syntax search)",
             "method": "post",
             "nested_columns": [
                 "interfaceIn",
                 "interfaceOut",
                 "interfaceInZone",
@@ -15610,25 +15652,25 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/secure-ports/devices",
             "api_scope_id": "dc62404f4a804f2ead5a76056f0ad47fe1ee0246",
             "columns": [
                 "intSecNetCount",
-                "intTotalNetCount",
+                "sn",
                 "siteName",
-                "intTotalEdgeCount",
                 "id",
                 "intSecEdgeCount",
-                "sn",
-                "usersCount",
+                "methods",
+                "intTotalNetCount",
                 "hostname",
-                "methods"
+                "usersCount",
+                "intTotalEdgeCount"
             ],
-            "description": "",
+            "description": "This table lists all 802.1x enabled network (not user) devices in the network. Only 802.1x security method is supported.\n\nSecurity can be deployed on network (non-edge) and on edge ports of the device. Not all ports need to have 802.1x security enabled.",
             "method": "post",
             "nested_columns": [],
             "summary": "802.1x Secure ports - Devices",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "methods",
@@ -15647,35 +15689,35 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/secure-ports/interfaces",
             "api_scope_id": "b281ade7334dbc7a22bfa0834f2fabcfa86c0573",
             "columns": [
-                "id",
-                "dynamicMacCount",
-                "method",
-                "vendor",
-                "intName",
-                "monitorMode",
-                "platform",
-                "edge",
-                "switchportMode",
-                "hostname",
-                "state",
+                "model",
+                "siteName",
                 "sn",
+                "voiceVlan",
+                "monitorMode",
                 "accVlan",
                 "usersCount",
-                "model",
-                "siteName",
+                "dynamicMacCount",
+                "switchportMode",
+                "intName",
+                "hostname",
                 "intDscr",
-                "voiceVlan",
-                "devType"
+                "state",
+                "platform",
+                "devType",
+                "method",
+                "vendor",
+                "id",
+                "edge"
             ],
-            "description": "Network access control interfaces inventory",
+            "description": "This table lists all 802.1x Secure Interfaces in the network. Only 802.1x security method is supported.\n\nThe interfaces should be in the state \"authorized\" or \"empty\". \"Unauthorized\" interface state indicate that the device was not authorized or no device attempted authorization on that interface.",
             "method": "post",
             "nested_columns": [
                 "devType"
             ],
             "summary": "802.1x Secure ports - Interfaces",
             "ui_columns": [
                 "hostname",
@@ -15705,26 +15747,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/secure-ports/users",
             "api_scope_id": "35b2c2aef79451e7c6beb180645638348ffd30db",
             "columns": [
-                "siteName",
                 "userState",
-                "id",
-                "state",
                 "sn",
+                "siteName",
+                "id",
+                "intName",
+                "hostname",
                 "username",
                 "userMethod",
-                "hostname",
-                "intName",
+                "state",
                 "userMac"
             ],
-            "description": "Network access control users inventory",
+            "description": "802.1x Secure ports - Users",
             "method": "post",
             "nested_columns": [],
             "summary": "802.1x Secure ports - Users",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "siteName",
@@ -15744,22 +15786,22 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/zone-firewall/interfaces",
             "api_scope_id": "cf6f4dd1573e802aafae22e38df61998c70576d3",
             "columns": [
                 "siteName",
+                "sn",
                 "id",
                 "isDefault",
-                "sn",
-                "hostname",
+                "zone",
                 "intName",
-                "zone"
+                "hostname"
             ],
-            "description": "Security gateway interfaces participating in zone firewall policies",
+            "description": "This table shows the interfaces in the network which are members of any security zone (and thus zone firewall policies are enforced on them)",
             "method": "post",
             "nested_columns": [
                 "zone"
             ],
             "summary": "Zone Firewall - Interfaces",
             "ui_columns": [
                 "hostname",
@@ -15776,69 +15818,69 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/security/zone-firewall/policies",
             "api_scope_id": "6dc8f403807c3343f64b8b20f7b1f1b5de6d79cf",
             "columns": [
-                "vxlanSrcGrp",
+                "siteName",
+                "uid",
+                "sn",
+                "interfaceIntraZone",
                 "ipTtl",
-                "id",
-                "l4Dst",
-                "tcpFlags",
-                "actionOriginal",
+                "ipFragmentOffset",
+                "policyName",
+                "mplsLabelIn",
+                "ipSrcRegion",
+                "interfaceInZone",
+                "vxlanVni",
+                "ruleNameNumeric",
+                "srcPorts",
                 "udpSrc",
-                "description",
+                "interfaceInterZone",
                 "ipProtocol",
-                "referencedTests",
-                "l4Src",
-                "active",
-                "ipDscp",
-                "l7Application",
-                "ipPacketLength",
                 "icmpType",
-                "ipPrecedence",
-                "mplsLabelIn",
+                "action",
+                "l4Dst",
                 "hostname",
-                "ipTos",
-                "ipSrc",
-                "srcPorts",
-                "policyName",
-                "interfaceOut",
-                "ipSrcRegion",
-                "ipv6Src",
-                "tcpDst",
                 "icmpCode",
+                "tcpFlags",
+                "referencedTests",
+                "ipPrecedence",
                 "ruleName",
-                "interfaceOutZone",
-                "tcpSrc",
-                "optionsTracked",
+                "ipPacketLength",
+                "ipSrc",
+                "icmpIcmpv6",
                 "ipDstRegion",
-                "interfaceIn",
-                "vxlanVni",
-                "others",
-                "vxlanDstGrp",
-                "sn",
-                "udpDst",
-                "interfaceIntraZone",
-                "siteName",
+                "ipTos",
                 "ipv6Dst",
+                "ipDst",
+                "l4Src",
+                "tcpDst",
+                "actionOriginal",
+                "udpDst",
+                "description",
+                "optionsTracked",
+                "interfaceOut",
+                "active",
+                "vxlanSrcGrp",
+                "vxlanDstGrp",
+                "id",
+                "ipDscp",
+                "tcpSrc",
                 "dstPorts",
-                "uid",
-                "icmpIcmpv6",
-                "ipFragmentOffset",
-                "ruleNameNumeric",
+                "interfaceOutZone",
+                "interfaceIn",
+                "l7Application",
+                "ipv6Src",
                 "interfaceVrf",
-                "action",
-                "interfaceInZone",
                 "ruleNumber",
-                "interfaceInterZone",
-                "ipDst"
+                "others"
             ],
-            "description": "Security gateways zone policies details",
+            "description": "This table covers all Zone Firewall Policies configured in the network",
             "method": "post",
             "nested_columns": [
                 "interfaceIn",
                 "interfaceOut",
                 "interfaceInZone",
                 "interfaceOutZone",
                 "interfaceIntraZone",
@@ -15933,28 +15975,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/serial-ports",
             "api_scope_id": "66ff0ffa77cd1a7268b05a4489bf132567fde0f0",
             "columns": [
-                "siteName",
                 "flowControl",
-                "label",
-                "loggingLevel",
-                "id",
-                "connector",
-                "mode",
                 "pinout",
                 "parameters",
+                "siteName",
                 "sn",
+                "id",
                 "name",
-                "hostname"
+                "mode",
+                "loggingLevel",
+                "hostname",
+                "label",
+                "connector"
             ],
-            "description": "Serial Ports",
+            "description": "Serial Ports description",
             "method": "post",
             "nested_columns": [],
             "summary": "Serial Ports",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "name",
@@ -15992,22 +16034,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/settings/jumphosts",
             "api_scope_id": "8733038e31573cb3aafe69bc020272f19f73dd35",
             "columns": [
-                "subnets",
-                "running",
                 "id",
-                "enabled",
+                "running",
                 "address",
+                "enabled",
                 "loginType",
-                "label",
-                "exclude"
+                "subnets",
+                "exclude",
+                "label"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "exclude",
                 "subnets"
             ],
@@ -16031,20 +16073,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/settings/ports",
             "api_scope_id": "1c73966d5d59dc31aef79269ff662ad80b5d6bb4",
             "columns": [
-                "subnets",
+                "excludeSubnets",
                 "port",
                 "id",
+                "subnets",
                 "protocol",
-                "label",
-                "excludeSubnets"
+                "label"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "excludeSubnets",
                 "subnets"
             ],
@@ -16066,17 +16108,17 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/snapshot-attributes",
             "api_scope_id": "4e31d8fdc457a0b4448e2e699dbde343807c2c2c",
             "columns": [
+                "sn",
                 "id",
                 "name",
-                "sn",
                 "value",
                 "hostname"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/snapshot-attributes",
@@ -16095,31 +16137,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/snapshot-devices",
             "api_scope_id": "1361822c3b08544fddb94e9197cd19fd407b3215",
             "columns": [
-                "vTask",
-                "settingsStates",
                 "family",
+                "parentId",
                 "model",
-                "siteName",
                 "type",
+                "siteName",
+                "sn",
                 "platform",
-                "ipString",
                 "id",
+                "vendor",
+                "ipString",
                 "version",
                 "source",
-                "sn",
-                "isApiTask",
-                "isSelected",
                 "hostname",
-                "vendor",
-                "parentId"
+                "isSelected",
+                "settingsStates",
+                "isApiTask"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "settingsStates"
             ],
             "summary": "POST /tables/snapshot-devices",
@@ -16150,25 +16191,25 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/bridges",
             "api_scope_id": "a8b7ab7c4e689937629699543914a015b639b2eb",
             "columns": [
+                "changeRate",
+                "stpDomain",
                 "siteName",
+                "sn",
+                "vlans",
                 "id",
                 "mode",
-                "sn",
-                "stpDomain",
-                "virtPorts",
                 "hostname",
-                "vlans",
-                "changeRate"
+                "virtPorts"
             ],
-            "description": "Overview of all Spanning-Tree Protocol (STP) bridges, protocol types, VLANs",
+            "description": "Overview of all Spanning tree bridges. Protocol types, VLANs are covered.\n\n---\n\nSTP Virtual Port: L2 port in the switched network which is a subject of STP protocol (subject of decision process of determining root ports and designated ports which are subsequently used for L2 link pruning)\n\nSTP Instance: Basic STP entity based on one STP protocol. It consists of root bridge, non-root bridges and active and blocked virtual ports. One pruned tree is calculated as the result of one instance.\n\n* In stp and rstp, one STP instance is used by all VLANs (they share the same topology)\n* In pvst and rapid-pvst, one STP instance is used by one VLAN only (each VLAN calculates its STP instance)\n* In mst, one STP instance may match arbitrary number of VLANs depending on the MST configuration\nSwitching Domain: Contiguously interconnected STP instances representing single L2 failure domain (where one STP instance can cause problems for other instances). Neighboring Bridges in one domain communicate with L2 protocols. One Bridge (Ethernet switch) can be member of one Switching Domain only.\n\n---\n\nSpanning tree protocol can be:\n\n* \"stp\": original spanning tree protocol, IEEE 802.1D\n* \"pvst\": per-VLAN spanning tree developed by Cisco Systems (tree for each VLAN, pvst+ for standard 802.1q trunks)\n* \"rstp\": rapid spanning protocol, IEEE 802.1w\n* \"rapid-pvst\": per-VLAN rapid spanning tree developed by Cisco Systems (tree for each VLAN)\n* \"mst\" or \"mstp\": multiple spanning tree protocol, IEEE 802.1s",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Bridges",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "stpDomain",
@@ -16186,34 +16227,34 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/guards",
             "api_scope_id": "970f429fdc181a25cdd93996e41824609141c470",
             "columns": [
-                "model",
+                "switchportMode",
+                "stpDomain",
                 "bpduGuard",
-                "siteName",
+                "model",
+                "portfast",
+                "rootGuard",
                 "platform",
                 "id",
-                "voiceVlan",
                 "bpduFilter",
-                "dynamicMacCount",
-                "devType",
-                "vendor",
+                "siteName",
                 "sn",
-                "stpDomain",
-                "switchportMode",
-                "accVlan",
-                "portfast",
+                "vendor",
+                "voiceVlan",
+                "intName",
                 "hostname",
-                "rootGuard",
-                "intName"
+                "accVlan",
+                "devType",
+                "dynamicMacCount"
             ],
-            "description": "Overview of all Spanning-Tree Protocol (STP) guards applied to interfaces",
+            "description": "This table covers various STP guard mechanisms usually applied on STP Interfaces. Those guards can be:\n* STP Portfast: if no STP switches are connected on the port, then the usual 50 sec STP port setup can be shortened up to 2 seconds\n* BPDU Guard: if no STP switches are connected on the port then no BPDU messages should appear. If they do, it is usually misconfiguration or miscabling and thus BPDU Guard will shut down such port\n* Root Guard: if BPDU from the switch with BPDU priority with better chance to be elected as root is received on this port, then the port is shutdown. It can indicate that rogue root switch or miscofigured BPDU priority switch exist in the network (the switch tries to be root on the place where it should not be present)\n* BPDU Filter: all BPDU messages will be filtered (both in and out). This can be extremely dangerous of configured without a good reason.\n\nSTP Portfast has its access and trunk version. Portfast trunk is usually applied facing servers with multiple VLANs configured. Please ensure that there is no software switch configured on that server.\n\nOther STP aids that can be encountered in the network are:\n* Loop Guard: Once a port was participating in STP process as root port and the port suddenly stops receiving BPDU messages, then it may indicate problem with upstream switch or unidirectional link - in all cases possibility of a loop in a network. Loop Guard will shut down the switchport in that case and thus limiting the chance for the loop to be created.\n* UDLD (unidirectional link detection): L2 mechanism that uses small packets to see if the L2 link is bidirectional. No STP messages are analyzed, works generally for all unidirectional situations\n\n---\n\nRecommended application of various STP Guards is:\n* No guards on edge ports where switch may or may not be (for example ports to other network infrastructures, lab networks, VMWare vSwitches etc)\n* STP Portfast + BPDU Guard on every edge switch port (with no STP switches connected, such as endpoint PCs, printers etc). Those features should be applied together, portfast without BPDU Guard should be avoided\n* BPDU Filter: Never use unless there is very good reason to do so - on a link with SP switch/router or on L2 DCI link where only one link exist or another L2 loop-avoidance mechanism is used. BPDU Filter ports should NOT be common switchport configuration, only limited exception. Those switchports should be examined first in any STP problems\n* UDLD on fiber links where two independent fibers are used for one link\n* UDLD on links with media converters which hide the remote port state\n* UDLD on leased SP links which hide the remote port state\n* Loop Guard on ports which should be root ports\n* Root Guard on selected designated ports - not to be used on ports which may become root ports after failover to secondary root",
             "method": "post",
             "nested_columns": [
                 "devType"
             ],
             "summary": "STP Guards",
             "ui_columns": [
                 "hostname",
@@ -16242,23 +16283,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/multiple-stp",
             "api_scope_id": "448aa070411d0084e2f21cdd3d29373b5db62a43",
             "columns": [
-                "dstHostname",
+                "srcSn",
                 "siteName",
                 "id",
-                "srcSn",
                 "srcHostname",
                 "stpCount",
+                "dstHostname",
                 "dstSn"
             ],
-            "description": "Detected multiple Spanning-Tree Protocol (STP) instances between two devices",
+            "description": "This table show neighbor switchports where there are multiple STP instances between them.\n\nThere should be only one STP instance beween two bridges/switches.\n\nThis table should be empty.",
             "method": "post",
             "nested_columns": [],
             "summary": "Multiple STPs",
             "ui_columns": [
                 "srcHostname",
                 "dstHostname",
                 "stpCount"
@@ -16272,26 +16313,26 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/neighbor-ports-vlan-mismatch",
             "api_scope_id": "6992b7848d045065d0295a7d5c824ad35f1defa6",
             "columns": [
-                "dstHostname",
+                "srcSn",
                 "siteName",
                 "id",
-                "dstVlanCount",
-                "srcSn",
                 "srcHostname",
-                "dstIntName",
+                "dstVlanCount",
+                "srcIntName",
                 "srcVlanCount",
-                "dstSn",
-                "srcIntName"
+                "dstIntName",
+                "dstHostname",
+                "dstSn"
             ],
-            "description": "Neighbor trunk ports where there is a different number of VLANs on each side of the link",
+            "description": "This table show neighbor switchports where there is different number of VLANs on both sides on the neighborship.\n\nAllowed VLANs on both sides of L2 neighborship (ie. on the trunk link) should be the same. If it is not, then on one side the VLANs might be configured errorneously.\n\nThis table should be empty.",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Ports VLAN Mismatch",
             "ui_columns": [
                 "srcHostname",
                 "srcIntName",
                 "srcVlanCount",
@@ -16308,24 +16349,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/ports-multiple-neighbors",
             "api_scope_id": "fe5ed75e32932dc9b06c10be9c32644348877883",
             "columns": [
-                "dstHostname",
+                "srcSn",
                 "siteName",
                 "id",
-                "srcSn",
                 "srcHostname",
+                "srcIntName",
                 "dstIntName",
-                "dstSn",
-                "srcIntName"
+                "dstHostname",
+                "dstSn"
             ],
-            "description": "Neighbor switchports where multiple Spanning-Tree Protocol (STP) peerings are detected",
+            "description": "This table show neighbor switchports where multiple neighbors are present.\n\nThis state may indicate L1 device such as hub or multiaccess Ethernet media operating in the Network.\n\nOn LAGs (PortChannels, Etherchannels) it may also indicate multichassis LAG configurations, which is mostly correct.",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Ports Multiple Neighbors",
             "ui_columns": [
                 "srcHostname",
                 "srcIntName",
                 "dstIntName",
@@ -16340,27 +16381,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/stp-cdp-ports-mismatch",
             "api_scope_id": "786c4b98cf35a27a04fc873cda9c6a60f48fdb9c",
             "columns": [
+                "cdpHostname",
                 "siteName",
+                "sn",
                 "id",
-                "cdpHostname",
                 "cdpIntName",
-                "stpSn",
-                "sn",
-                "stpHostname",
-                "cdpSn",
-                "stpIntName",
+                "intName",
                 "hostname",
-                "intName"
+                "stpIntName",
+                "cdpSn",
+                "stpSn",
+                "stpHostname"
             ],
-            "description": "Port connections with mismatched hostname or interface name in STP and CDP protocols reading",
+            "description": "This table show neighbor switchports where there is different hostname or interface name of the remote (Dst) switch gathered via STP and via CDP protocols.\n\nCDP and STP hostnames and switchport identifications should be the same.\n\nThis table should be empty.",
             "method": "post",
             "nested_columns": [],
             "summary": "STP/CDP Mismatch",
             "ui_columns": [
                 "hostname",
                 "intName",
                 "stpHostname",
@@ -16377,20 +16418,20 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/instance-members",
             "api_scope_id": "88d315d3e4e98a23bdd1df2d5cd7e9593f4a60a4",
             "columns": [
+                "members",
                 "id",
-                "vlanId",
-                "vlanName",
                 "rootHostname",
+                "vlanName",
                 "rootId",
-                "members"
+                "vlanId"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "members"
             ],
             "summary": "POST /tables/spanning-tree/instance-members",
@@ -16411,29 +16452,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/instances",
             "api_scope_id": "51d1ebee0d39a16ff63fce2edac961c7b3154d83",
             "columns": [
-                "rootPriority",
+                "changeRate",
+                "stpDomain",
                 "siteName",
-                "virtPorts",
+                "sn",
+                "devs",
                 "id",
                 "edgesSum",
-                "devs",
-                "sn",
-                "vlanId",
-                "stpDomain",
                 "vlanName",
                 "rootId",
+                "vlanId",
                 "hostname",
-                "changeRate"
+                "virtPorts",
+                "rootPriority"
             ],
-            "description": "Spanning-Tree Protocol (STP) instances, root bridges and associated VLANs",
+            "description": "Overview of all Spanning tree instances. Root bridges, VLANs are covered.\n\nSpanning tree (=instance) size proportionally degrades quality of instance state, and should not be expanded unnecessarily. Keeping instance size to the minimum improves overall spanning tree health, such as limiting fault propagation, and improving convergence speed.\n\n---\n\nSTP Virtual Port: L2 port in the switched network which is a subject of STP protocol (subject of decision process of determining root ports and designated ports which are subsequently used for L2 link pruning)\n\nSTP Instance: Basic STP entity based on one STP protocol. It consists of root bridge, non-root bridges and active and blocked virtual ports. One pruned tree is calculated as the result of one instance.\n\n  In stp and rstp, one STP instance is used by all VLANs (they share the same topology)\n  In pvst and rapid-pvst, one STP instance is used by one VLAN only (each VLAN calculates its STP instance)\n  In mst, one STP instance may match arbitrary number of VLANs depending on the MST configuration\n\nSwitching Domain: Contiguously interconnected STP instances representing single L2 failure domain (where one STP instance can cause problems for other instances). Neighboring Bridges in one domain communicate with L2 protocols. One Bridge (Ethernet switch) can be member of one Switching Domain only.\n\n---\n\nSpanning tree protocol can be:\n* \"stp\": original spanning tree protocol, IEEE 802.1D\n* \"pvst\": per-VLAN spanning tree developed by Cisco Systems (tree for each VLAN, pvst+ for standard 802.1q trunks)\n* \"rstp\": rapid spanning protocol, IEEE 802.1w\n* \"rapid-pvst\": per-VLAN rapid spanning tree developed by Cisco Systems (tree for each VLAN)\n* \"mst\" or \"mstp\": multiple spanning tree protocol, IEEE 802.1s",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Instances",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "stpDomain",
@@ -16454,36 +16495,36 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/neighbors",
             "api_scope_id": "56f6391a3fc294d45b8e6b3677fd877fd1314c32",
             "columns": [
-                "snDst",
-                "portIdDst",
-                "id",
-                "portPathCost",
-                "vlanName",
-                "intName",
+                "siteName",
                 "hostnameDst",
-                "stpDomain",
+                "sn",
                 "portId",
-                "hostname",
                 "portRole",
-                "portStatusDst",
-                "sn",
-                "vlanId",
-                "siteName",
                 "portPathCostDst",
-                "intNameDst",
+                "portStatusDst",
+                "portIdDst",
+                "portPathCost",
+                "snDst",
+                "intName",
+                "hostname",
                 "portRoleDst",
                 "rootId",
-                "portStatus"
+                "stpDomain",
+                "intNameDst",
+                "id",
+                "vlanName",
+                "portStatus",
+                "vlanId"
             ],
-            "description": "Spanning-Tree Protocol (STP) peering relationships of connected bridges",
+            "description": "STP \"Neighbor\" information - STP \"peering\" relationships between couples of directly connected STP Bridges (switches).\\\nEach line describes neighborship of two STP Bridges:\n* Src - local bridge\n* Dst - remote bridge\n\nIf there is \"alternate\" or \"backup\" port role on one bridge and \"designated\" role on second bridge, then the first port should be in \"blocking\" status (not \"forwarding\") to avoid the L2 switching loop.\n\nVirtual ports are ports in a particular VLAN. A single trunk will participate in multiple spanning tree instances, one for every VLAN allowed on the port, including native VLAN.\n\n---\n\nSTP Virtual Port: L2 port in the switched network which is a subject of STP protocol (subject of decision process of determining root ports and designated ports which are subsequently used for L2 link pruning)\n\nSTP Instance: Basic STP entity based on one STP protocol. It consists of root bridge, non-root bridges and active and blocked virtual ports. One pruned tree is calculated as the result of one instance.\n* In stp and rstp, one STP instance is used by all VLANs (they share the same topology)\n* In pvst and rapid-pvst, one STP instance is used by one VLAN only (each VLAN calculates its STP instance)\n* In mst, one STP instance may match arbitrary number of VLANs depending on the MST configuration\n\nSwitching Domain: Contiguously interconnected STP instances representing single L2 failure domain (where one STP instance can cause problems for other instances). Neighboring Bridges in one domain communicate with L2 protocols. One Bridge (Ethernet switch) can be member of one Switching Domain only.\n\n---\n\nSTP port role can be one of the following:\n* \"root\": The port that receives the best BPDU on a bridge is the root port. This is the port that is the closest to the root bridge in terms of path cost.\n* \"designated\": The port not facing the root but forwarding traffic (while lowest cost) from another segment. On a given segment, there can only be one path toward the root bridge. If there are two, there is a bridging loop in the network and all but one designated ports (the one with lowest oath cost) must be blocked\n* \"alternate\" or \"backup\": The port that is neither root port nor designated port\n\nSTP port status can be one of the following:\n* \"forwarding\": Active port in operation forwarding data and learning MAC addresses. (Desired port state on active tree)\n* \"learning\": Port in operation not forwarding data but learning MAC addresses. Transient state for about 15 seconds, not permanent.\n* \"listening\": Port in operation not forwarding data and not learning MAC addresses. Transient state for about 15 seconds, not permanent.\n* \"blocking\": Port put aside active topology (and thus not forwarding data and not learning MAC adresses) to avoid L2 loops in the network\n* \"disabled\": Port which is administratively shutdown\n* \"broken\": Port put into inconsistent state due to VLAN (including the native VLAN) or protocol mismatch",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Peerings",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "stpDomain",
@@ -16511,29 +16552,29 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/ports",
             "api_scope_id": "17cfb1b38ca20ac3e42b918aceb934443f60129e",
             "columns": [
-                "portRole",
+                "stpDomain",
                 "siteName",
-                "id",
-                "portPathCost",
                 "sn",
-                "hostname",
-                "stpDomain",
-                "vlanId",
+                "id",
+                "portId",
+                "portRole",
                 "vlanName",
-                "portStatus",
+                "intName",
                 "rootId",
-                "portId",
-                "intName"
+                "portStatus",
+                "hostname",
+                "vlanId",
+                "portPathCost"
             ],
-            "description": "Spanning-Tree Protocol (STP) virtual ports inventory",
+            "description": "Layer 2 information about every STP Virtual Port discovered in the network.\n\nVirtual ports are ports in a particular VLAN. A single trunk will participate in multiple spanning tree instances, one for every VLAN allowed on the port, including native VLAN.\n\n---\nSTP Virtual Port: L2 port in the switched network which is a subject of STP protocol (subject of decision process of determining root ports and designated ports which are subsequently used for L2 link pruning)\n\nSTP Instance: Basic STP entity based on one STP protocol. It consists of root bridge, non-root bridges and active and blocked virtual ports. One pruned tree is calculated as the result of one instance.\n  * In stp and rstp, one STP instance is used by all VLANs (they share the same topology)\n  * In pvst and rapid-pvst, one STP instance is used by one VLAN only (each VLAN calculates its STP instance)\n  * In mst, one STP instance may match arbitrary number of VLANs depending on the MST configuration\n\nSwitching Domain: Contiguously interconnected STP instances representing single L2 failure domain (where one STP instance can cause problems for other instances). Neighboring Bridges in one domain communicate with L2 protocols. One Bridge (Ethernet switch) can be member of one Switching Domain only.\n\n---\n\nSTP port role can be one of the following:\n* \"root\" The port that receives the best BPDU on a bridge is the root port. This is the port that is the closest to the root bridge in terms of path cost.\n* \"designated\" The port not facing the root but forwarding traffic (while lowest cost) from another segment. On a given segment, there can only be one path toward the root bridge. If there are two, there is a bridging loop in the network and all but one designated ports (the one with lowest oath cost) must be blocked\n* \"alternate\" or \"backup\": The port that is neither root port nor designated port\n\nSTP port status can be one of the following:\n* \"forwarding\": Active port in operation forwarding data and learning MAC addresses. (Desired port state on active tree)\n* \"learning\": Port in operation not forwarding data but learning MAC addresses. Transient state for about 15 seconds, not permanent.\n* \"listening\": Port in operation not forwarding data and not learning MAC addresses. Transient state for about 15 seconds, not permanent.\n* \"blocking\": Port put aside active topology (and thus not forwarding data and not learning MAC adresses) to avoid L2 loops in the network\n* \"disabled\": Port which is administratively shutdown\n* \"broken\": Port put into inconsistent state due to VLAN (including the native VLAN) or protocol mismatch",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Virtual Ports",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "stpDomain",
@@ -16555,19 +16596,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/radius",
             "api_scope_id": "a6087fe22f2ee5581335df689ea5d0b6d2868945",
             "columns": [
-                "stpMode",
                 "distance",
-                "id",
                 "stpDomain",
                 "srcDev",
+                "stpMode",
+                "id",
                 "dstDev"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [],
             "summary": "POST /tables/spanning-tree/radius",
             "ui_columns": [
@@ -16587,23 +16628,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/topology",
             "api_scope_id": "7fabda7b35a8320c9edac7a31e9745c87bd81cc7",
             "columns": [
+                "changeRate",
+                "stpDomain",
                 "siteName",
                 "id",
-                "vlanId",
-                "stpDomain",
                 "vlanName",
                 "root",
-                "changeRate"
+                "vlanId"
             ],
-            "description": "Spanning-Tree Protocol (STP) instances with topology change compared to the last snapshot",
+            "description": "The table presents Spanning Tree instances with non-zero Change BPDU rate.\n\nLayer 2 topology stability reflects changes or convergence events occurring within spanning tree instances, and how many users these converge events affect. Ideally, convergence events should not occur at all, however a small number of convergence events can be acceptable due to topology change notifications generated by port state changes on bridges running legacy spanning tree mode.\n\n---\nSTP Virtual Port: L2 port in the switched network which is a subject of STP protocol (subject of decision process of determining root ports and designated ports which are subsequently used for L2 link pruning)\n\nSTP Instance: Basic STP entity based on one STP protocol. It consists of root bridge, non-root bridges and active and blocked virtual ports. One pruned tree is calculated as the result of one instance.\n* In stp and rstp, one STP instance is used by all VLANs (they share the same topology)\n* In pvst and rapid-pvst, one STP instance is used by one VLAN only (each VLAN calculates its STP instance)\n* In mst, one STP instance may match arbitrary number of VLANs depending on the MST configuration\n\nSwitching Domain: Contiguously interconnected STP instances representing single L2 failure domain (where one STP instance can cause problems for other instances). Neighboring Bridges in one domain communicate with L2 protocols. One Bridge (Ethernet switch) can be member of one Switching Domain only.",
             "method": "post",
             "nested_columns": [],
             "summary": "STP Stability",
             "ui_columns": [
                 "root",
                 "siteName",
                 "stpDomain",
@@ -16620,30 +16661,30 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/vlans",
             "api_scope_id": "d155d2c73814c14440c2d44b2d17ff429641d456",
             "columns": [
-                "rootPriority",
-                "bridgePriority",
-                "siteName",
-                "virtPorts",
-                "id",
-                "sn",
+                "bridgeId",
+                "changeRate",
                 "rootCost",
                 "stpDomain",
-                "vlanId",
-                "vlanName",
-                "bridgeId",
+                "siteName",
+                "sn",
+                "id",
+                "bridgePriority",
                 "rootId",
+                "vlanName",
+                "vlanId",
                 "hostname",
-                "changeRate"
+                "virtPorts",
+                "rootPriority"
             ],
-            "description": "Spanning-Tree Protocol (STP) VLANs inventory",
+            "description": "Layer 2 information about every VLAN (Virtual LAN network) discovered in the network.\n\n---\n\nSTP Virtual Port: L2 port in the switched network which is a subject of STP protocol (subject of decision process of determining root ports and designated ports which are subsequently used for L2 link pruning)\n\nSTP Instance: Basic STP entity based on one STP protocol. It consists of root bridge, non-root bridges and active and blocked virtual ports. One pruned tree is calculated as the result of one instance.\n*  In stp and rstp, one STP instance is used by all VLANs (they share the same topology)\n*  In pvst and rapid-pvst, one STP instance is used by one VLAN only (each VLAN calculates its STP instance)\n*  In mst, one STP instance may match arbitrary number of VLANs depending on the MST configuration\n\nSwitching Domain: Contiguously interconnected STP instances representing single L2 failure domain (where one STP instance can cause problems for other instances). Neighboring Bridges in one domain communicate with L2 protocols. One Bridge (Ethernet switch) can be member of one Switching Domain only.",
             "method": "post",
             "nested_columns": [],
             "summary": "STP VLANs",
             "ui_columns": [
                 "hostname",
                 "siteName",
                 "stpDomain",
@@ -16702,24 +16743,24 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/users",
             "api_scope_id": "55ebdafabb0a68c1e2caaae7ac68c58108c770ad",
             "columns": [
-                "timezone",
+                "ldapId",
                 "isLocal",
+                "roleNames",
+                "ssoProvider",
                 "id",
-                "roleIds",
-                "domainSuffixes",
                 "email",
-                "roleNames",
-                "ldapId",
+                "domainSuffixes",
+                "timezone",
                 "username",
-                "ssoProvider"
+                "roleIds"
             ],
             "description": "",
             "method": "post",
             "nested_columns": [
                 "roleIds",
                 "roleNames"
             ],
@@ -16744,23 +16785,23 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vlan/device",
             "api_scope_id": "56568e03bc4cf792bd2296602128c8932d99d18b",
             "columns": [
-                "stdStatus",
+                "stpDomain",
+                "sn",
                 "siteName",
                 "id",
-                "sn",
-                "vlanId",
-                "stpDomain",
+                "status",
                 "vlanName",
+                "stdStatus",
                 "hostname",
-                "status"
+                "vlanId"
             ],
             "description": "Virtual LAN (VLAN) inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs - Device Detail",
             "ui_columns": [
                 "hostname",
@@ -16781,19 +16822,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vlan/device-summary",
             "api_scope_id": "fc39974e11fc30a9488f6f2802d9292818974ef1",
             "columns": [
                 "siteName",
+                "sn",
                 "id",
+                "totalVlanCount",
                 "activeVlanCount",
-                "sn",
-                "hostname",
-                "totalVlanCount"
+                "hostname"
             ],
             "description": "Virtual LAN (VLAN) per managed network device",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs - Device Summary",
             "ui_columns": [
                 "hostname",
@@ -16810,19 +16851,19 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vlan/l3-gateways",
             "api_scope_id": "3985721e62fbfaac22bd269c4d08cab207df95e5",
             "columns": [
-                "id",
-                "networks",
                 "stpDomain",
+                "id",
+                "rootId",
                 "vlanId",
-                "rootId"
+                "networks"
             ],
             "description": "Layer 3 Gateways to VLAN mappings",
             "method": "post",
             "nested_columns": [
                 "networks"
             ],
             "summary": "L3 Gateways",
@@ -16841,21 +16882,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vlan/network-summary",
             "api_scope_id": "ff4f2af574d3e9dae254a81d3987ba363b4c7063",
             "columns": [
-                "dscr",
+                "devCount",
                 "id",
-                "vlanId",
                 "vlanName",
-                "devCount"
+                "dscr",
+                "vlanId"
             ],
-            "description": "Virtual LANs (VLAN) configured in network grouped by VLAN ID",
+            "description": "List of all VLANs configured in network. Grouped by VLAN ID. You can use this table for example to check free VLANs in your network.",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs - Network Summary",
             "ui_columns": [
                 "vlanId",
                 "vlanName",
                 "dscr",
@@ -16871,21 +16912,21 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vlan/site-summary",
             "api_scope_id": "f9221b6c36b8576b46df1c8ec0847b68a68957e8",
             "columns": [
                 "siteName",
-                "dscr",
+                "devCount",
                 "id",
-                "vlanId",
                 "vlanName",
-                "devCount"
+                "dscr",
+                "vlanId"
             ],
-            "description": "Virtual LANs (VLAN) configured in network grouped by VLAN ID with site information",
+            "description": "List of all VLANs configured on the site. Grouped by VLAN ID. You can use this table for example to check free VLANs on site.",
             "method": "post",
             "nested_columns": [],
             "summary": "VLANs - Summary per Site",
             "ui_columns": [
                 "siteName",
                 "vlanId",
                 "vlanName",
@@ -16901,21 +16942,21 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vrf/detail",
             "api_scope_id": "6b84960151fe991f1dd4f5a2b5888c4920a55965",
             "columns": [
-                "siteName",
                 "rd",
-                "id",
-                "intCount",
+                "siteName",
                 "sn",
-                "vrf",
-                "hostname"
+                "intCount",
+                "id",
+                "hostname",
+                "vrf"
             ],
             "description": "Virtual Routing and Forwadring instances per devices",
             "method": "post",
             "nested_columns": [],
             "summary": "VRF Devices",
             "ui_columns": [
                 "hostname",
@@ -16933,22 +16974,22 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vrf/interfaces",
             "api_scope_id": "aa24fef60e95afd2f2216784150dfdaea9cc1557",
             "columns": [
-                "siteName",
                 "rd",
-                "id",
+                "siteName",
                 "sn",
-                "networks",
-                "vrf",
+                "id",
+                "intName",
                 "hostname",
-                "intName"
+                "networks",
+                "vrf"
             ],
             "description": "Virtual Routing and Forwadring instances per interfaces",
             "method": "post",
             "nested_columns": [
                 "networks"
             ],
             "summary": "VRF Interfaces",
@@ -16969,16 +17010,16 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vrf/summary",
             "api_scope_id": "97a2e35438a2a2cb3afb045f7faa765664573679",
             "columns": [
-                "id",
                 "devices",
+                "id",
                 "vrf"
             ],
             "description": "Virtual Routing and Forwadring instances per devices summary",
             "method": "post",
             "nested_columns": [],
             "summary": "VRF Summary",
             "ui_columns": [
@@ -16994,28 +17035,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vxlan/interfaces",
             "api_scope_id": "5e2b2153f70005662761f89aa478843744f8e5ea",
             "columns": [
-                "siteName",
-                "hostLearningMode",
-                "sourcePrimaryIp",
-                "localRouterMac",
-                "id",
                 "sourceSecondaryIp",
-                "controlPlane",
+                "sourcePrimaryIp",
+                "siteName",
                 "sn",
-                "encap",
                 "sourceInt",
+                "id",
                 "sourceSecondaryIpv6",
-                "sourcePrimaryIpv6",
+                "controlPlane",
+                "intName",
+                "hostLearningMode",
                 "hostname",
-                "intName"
+                "localRouterMac",
+                "sourcePrimaryIpv6",
+                "encap"
             ],
             "description": "Virtual Tunnel End Point (VTEP) interfaces inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "VTEP Interfaces",
             "ui_columns": [
                 "hostname",
@@ -17040,37 +17081,37 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vxlan/peers",
             "api_scope_id": "0b8ebbf68d3dbb9b557863ff4dc507cee018bc8b",
             "columns": [
+                "siteName",
+                "sn",
+                "vni",
+                "learnType",
                 "neiHostname",
-                "id",
-                "uptime",
-                "neiSiteName",
+                "source",
+                "neiIntName",
+                "routerMac",
                 "eVni",
-                "neiSn",
-                "neiDevType",
+                "neiSiteName",
                 "intName",
-                "neiAddress",
-                "neiIntName",
-                "flags",
-                "localAddress",
                 "hostname",
-                "subnet",
+                "neiDevType",
                 "state",
-                "source",
-                "sn",
-                "siteName",
-                "vni",
+                "target",
+                "neiAddress",
+                "neiSn",
+                "subnet",
                 "devType",
-                "learnType",
-                "routerMac",
-                "target"
+                "flags",
+                "localAddress",
+                "id",
+                "uptime"
             ],
             "description": "Virtual Tunnel End Point (VTEP) peers matrix",
             "method": "post",
             "nested_columns": [],
             "summary": "VTEP Peers",
             "ui_columns": [
                 "hostname",
@@ -17096,27 +17137,27 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vxlan/vni",
             "api_scope_id": "26eb5f7ef155608cc045df062cc5b641dd877789",
             "columns": [
-                "bd",
-                "siteName",
+                "cfg",
                 "type",
+                "siteName",
+                "sn",
+                "vniState",
                 "id",
                 "vni",
                 "mode",
-                "sn",
-                "vniState",
-                "cfg",
-                "vrf",
-                "hostname",
+                "bd",
                 "intName",
-                "mcastGroup"
+                "mcastGroup",
+                "hostname",
+                "vrf"
             ],
             "description": "VXLAN network identifier (VNI) inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "VXLAN Network Identifier",
             "ui_columns": [
                 "hostname",
@@ -17141,20 +17182,20 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/vxlan/vtep",
             "api_scope_id": "f78de74c207482ad3de80cf8828bf7ff74732426",
             "columns": [
                 "siteName",
-                "id",
                 "sn",
-                "vniCount",
-                "interfacesCount",
+                "id",
                 "hostname",
-                "peersCount"
+                "vniCount",
+                "peersCount",
+                "interfacesCount"
             ],
             "description": "VXLAN tunnel endpoint (VTEP) inventory",
             "method": "post",
             "nested_columns": [],
             "summary": "VXLAN Tunnel Endpoints",
             "ui_columns": [
                 "hostname",
@@ -17172,33 +17213,33 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/wireless/access-points",
             "api_scope_id": "989c3820c6d3d3fe8ce084b18c9b7210fc925581",
             "columns": [
-                "switchPort",
                 "clientCount",
+                "switchPort",
+                "bssidCount",
                 "siteName",
-                "avgRssi",
-                "avgSignalToNoiseRatio",
-                "switchSn",
+                "impact",
+                "switchHostname",
                 "id",
-                "apSn",
-                "bssidCount",
+                "apPort",
+                "avgSignalToNoiseRatio",
+                "apName",
                 "apMac",
-                "controller",
+                "apSn",
                 "ssid",
                 "controllerSn",
-                "apPort",
-                "apName",
-                "impact",
-                "switchHostname"
+                "controller",
+                "avgRssi",
+                "switchSn"
             ],
-            "description": "Wireless access points inventory",
+            "description": "Details of all of the Wireless Access Points in the network, including the number of clients associated to each APs. Further investigation would be suitable for following results:\n* Zero number of clients on any AP (may indicate that it is not used)\n* Highly disproportional number of clients among APs (may indicate unexpected load on part of the wireless infrastructure)\n* High number of clients eg. higher than 25-30 (may indicate RF overload and thus low throughput)\n* Only one AP (may indicate high availability problem)\n* Only one switch (or low number of switches) connecting the APs (may indicate high availability problem)\n* Low average signal strength (may indicate low coverage or high signal attenuation)\n* Low average signal to noise ratio (may indicate interference with another or non-Wifi RF noise)",
             "method": "post",
             "nested_columns": [
                 "ssid"
             ],
             "summary": "Wireless Access Points",
             "ui_columns": [
                 "controller",
@@ -17224,38 +17265,38 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/wireless/clients",
             "api_scope_id": "ab2b47f3fc0061878d4d91037bdb2456264b9e55",
             "columns": [
-                "client",
-                "id",
-                "inPktsRate",
-                "signalToNoiseRatio",
-                "frequency",
-                "pktsRate",
+                "siteName",
+                "inBytesRate",
                 "bssid",
-                "outPktsRate",
-                "policyManagerState",
-                "ssid",
                 "controllerSn",
                 "apName",
-                "clientIp",
-                "inBytesRate",
                 "uniqId",
+                "ssid",
+                "controller",
+                "outPktsRate",
                 "state",
+                "bytesRate",
                 "apSn",
-                "siteName",
+                "frequency",
                 "rssi",
-                "bytesRate",
-                "controller",
-                "outBytesRate"
+                "client",
+                "pktsRate",
+                "signalToNoiseRatio",
+                "id",
+                "outBytesRate",
+                "inPktsRate",
+                "policyManagerState",
+                "clientIp"
             ],
-            "description": "Wireless clients inventory",
+            "description": "Details of all of the wireless clients associated to the Access Points. Further investigation would be suitable for following results:\n* Which SSIDs are present (may indicate client misconfiguration)\n* If the IP address assignment is as expected (may indicate VLAN mismatch or DHCP problems)\n* If there are wireless clients which are not associated for considerable amount of time (may indicate credentials problem)\n* High amount of transferred data (may indicate virus infection or inappropropriate client use)\n* Low signal strength (may indicate low coverage or high signal attenuation)\n* Low signal to noise ratio (may indicate interference with another or non-Wifi RF noise)",
             "method": "post",
             "nested_columns": [],
             "summary": "Wireless Clients",
             "ui_columns": [
                 "controller",
                 "siteName",
                 "apName",
@@ -17286,21 +17327,21 @@
         "patch": null,
         "post": {
             "api_endpoint": "tables/wireless/controllers",
             "api_scope_id": "57202e6caa54c5ebb4dd83da714200ad33fa543f",
             "columns": [
                 "clientCount",
                 "siteName",
-                "apCount",
                 "id",
-                "controller",
                 "ssid",
-                "controllerSn"
+                "controllerSn",
+                "controller",
+                "apCount"
             ],
-            "description": "Wireless controllers inventory",
+            "description": "Overview of the Wireless Controllers in the network, showing the number of Access Points registered to each controller, and the total number of clients associated to the registered APs. Further investigation would be suitable for following results:\n* Zero number of APs or clients on any WLC (may indicate that it is not used)\n* Highly disproportional number of APs or clients among WLCs (may indicate unexpected load on part of the wireless infrastructure)\n* Only one WLC (may indicate high availability problem)",
             "method": "post",
             "nested_columns": [
                 "ssid"
             ],
             "summary": "Wireless Controllers",
             "ui_columns": [
                 "controller",
@@ -17318,28 +17359,28 @@
         "delete": null,
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/wireless/radio",
             "api_scope_id": "a86fcefe3373c1206c2f3a0f4dd4e7366e28dd8a",
             "columns": [
-                "radioFreq",
-                "wlanSsid",
                 "clientCount",
+                "wlanBssid",
                 "siteName",
+                "wlanSsid",
                 "id",
+                "radioMac",
+                "radioStatus",
+                "apName",
+                "radioFreq",
                 "apSn",
                 "radioDscr",
-                "wlanBssid",
-                "apName",
-                "mac",
-                "radioStatus",
-                "radioMac"
+                "mac"
             ],
-            "description": "Wireless Radios & BSSID inventory",
+            "description": "This table covers BSSID mapping to each Radio circuit on each wireless Access Point in the Network. Many APs today employ multiple Radio circuits to cover multiple frequency ranges.\\\nSSID ASCII identifiers are included in the table as well to ease the mapping.",
             "method": "post",
             "nested_columns": [],
             "summary": "Wireless Radios & BSSID",
             "ui_columns": [
                 "apName",
                 "siteName",
                 "apSn",
@@ -17362,19 +17403,19 @@
         "get": null,
         "patch": null,
         "post": {
             "api_endpoint": "tables/wireless/ssid-summary",
             "api_scope_id": "46afef4e48bcb78a68157f77a26fc4b11909442f",
             "columns": [
                 "clientCount",
-                "apCount",
                 "id",
                 "radioCount",
                 "ssid",
-                "wlcCount"
+                "wlcCount",
+                "apCount"
             ],
             "description": "Wireless service set identifier (SSID) summary",
             "method": "post",
             "nested_columns": [],
             "summary": "Wireless SSID Summary",
             "ui_columns": [
                 "ssid",
```

### Comparing `ipfabric-6.7.3/ipfabric/settings/__init__.py` & `ipfabric-6.8.0b0/ipfabric/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/settings/api_tokens.py` & `ipfabric-6.8.0b0/ipfabric/settings/api_tokens.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/settings/attributes.py` & `ipfabric-6.8.0b0/ipfabric/settings/attributes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import re
+from datetime import datetime
 from typing import Optional, List, Any
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from ipfabric.exceptions import deprecated_args_decorator
 
@@ -155,26 +156,45 @@
         """
         Deletes attributes by Attribute
         :param attributes: dict: Attribute dictionaries
         :return:
         """
         return self.delete_attribute_by_id(*[str(i["id"]) for i in attributes])
 
-    def update_local_attr_from_global(self) -> bool:
-        """Currently can only update devices that are in the snapshot."""
+    def update_local_attr_from_global(
+        self,
+        wait_for_load: bool = True,
+        # wait_for_assurance: bool = True,  # TODO: NIM-14475 - 6.8.2 fix
+        timeout: int = 60,
+        retry: int = 5,
+    ) -> bool:
+        """
+        Updates Snapshot Local Attributes based on Global.
+        Returns True is successfully completed, False if the snapshot load did not complete if required.
+        """
+        wait_for_assurance = False
         if not self.snapshot_id:
             raise ImportError("Please initialize Attributes class with a snapshot_id.")
-        g_attrs = self.client.fetch_all("tables/global-attributes", columns=["name", "value", "sn"], snapshot=False)
-        if not g_attrs:
-            raise ValueError("No Global Attributes found.")
-
-        local_attrs = self.all()
-        if local_attrs:
-            self.delete_attribute(*local_attrs)
-
-        if self.client.api_version < "v6.7":  # TODO: Remove in v6.9 or v7.0
-            local_sn = {
-                i["sn"] for i in self.client.inventory.devices.all(columns=["sn"], snapshot_id=self.snapshot_id)
-            }
-            g_attrs = [g for g in g_attrs if g["sn"] in local_sn]
-        self.set_attributes_by_sn(g_attrs)
+        recalc = self.check_sites_recalculation()
+        ts = int(datetime.now().timestamp() * 1000)
+        resp = self.client.post("/attributes/local/update-from-global", json={"snapshot": self.snapshot_id})
+        resp.raise_for_status()
+
+        if recalc and (wait_for_load or wait_for_assurance):
+            if not self.client.snapshots[self.snapshot_id]._check_load_status(
+                    ts, wait_for_assurance, timeout, retry, 'recalculate'
+            ):
+                return False
+        self.client.snapshots[self.snapshot_id]._refresh_status()
+        if self.client.snapshots[self.snapshot_id].loaded and self.client.snapshot_id == self.snapshot_id:
+            self.client.devices.update()
         return True
+
+    def check_sites_recalculation(self) -> bool:
+        """Checks if updating local attributes requires recalculation."""
+        if not self.snapshot_id:
+            raise ImportError("Please initialize Attributes class with a snapshot_id.")
+        resp = self.client.post(
+            "/attributes/local/update-from-global/check-sites-recalculation", json={"snapshot": self.snapshot_id}
+        )
+        resp.raise_for_status()
+        return resp.json()["needsRecalculation"]
```

### Comparing `ipfabric-6.7.3/ipfabric/settings/authentication.py` & `ipfabric-6.8.0b0/ipfabric/settings/authentication.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/settings/discovery.py` & `ipfabric-6.8.0b0/ipfabric/settings/discovery.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/settings/local_users.py` & `ipfabric-6.8.0b0/ipfabric/settings/local_users.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/settings/rbac.py` & `ipfabric-6.8.0b0/ipfabric/settings/rbac.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/settings/seeds.py` & `ipfabric-6.8.0b0/ipfabric/settings/seeds.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/settings/settings.py` & `ipfabric-6.8.0b0/ipfabric/settings/settings.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/settings/site_separation.py` & `ipfabric-6.8.0b0/ipfabric/settings/site_separation.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/settings/vendor_api.py` & `ipfabric-6.8.0b0/ipfabric/settings/vendor_api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/settings/vendor_api_models.py` & `ipfabric-6.8.0b0/ipfabric/settings/vendor_api_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,25 +326,27 @@
 class Versa(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, DefaultRateLimiterSettings, BaseModel):
     """
     Versa vendor api support
     """
 
     paginationLimit: int = 1000
     type: Literal["versa"] = "versa"
+    combinedDiscovery: bool = True
     maxConcurrentRequests: int = 10
     maxCapacity: int = 100
     refillRate: int = 2
 
 
 class Viptela(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, DefaultRateLimiterSettings, BaseModel):
     """
     Viptela vendor api support
     """
 
     type: Literal["viptela"] = "viptela"
+    combinedDiscovery: bool = True
     maxConcurrentRequests: int = 25
 
 
 class NSXT(VendorAPI, RejectUnauthorized, UserAuthBaseUrl, BaseModel):
     """
     NSXT vendor api support
     """
```

### Comparing `ipfabric-6.7.3/ipfabric/tools/__init__.py` & `ipfabric-6.8.0b0/ipfabric/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/tools/configuration.py` & `ipfabric-6.8.0b0/ipfabric/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/tools/discovery_history.py` & `ipfabric-6.8.0b0/ipfabric/tools/discovery_history.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/tools/managed_rbac/v6/7/policies.json` & `ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/7/policies.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/tools/managed_rbac/v6/7/roles.json` & `ipfabric-6.8.0b0/ipfabric/tools/managed_rbac/v6/7/roles.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/tools/nist.py` & `ipfabric-6.8.0b0/ipfabric/tools/nist.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/tools/rbac.py` & `ipfabric-6.8.0b0/ipfabric/tools/rbac.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/tools/restore_intents.py` & `ipfabric-6.8.0b0/ipfabric/tools/restore_intents.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/tools/shared.py` & `ipfabric-6.8.0b0/ipfabric/tools/shared.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/tools/site_seperation_report.py` & `ipfabric-6.8.0b0/ipfabric/tools/site_seperation_report.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/ipfabric/tools/vulnerabilities.py` & `ipfabric-6.8.0b0/ipfabric/tools/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/LICENSE` & `ipfabric-6.8.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.3/NOTICES.md` & `ipfabric-6.8.0b0/NOTICES.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Old Deprecation & Other Important Notices
 
+## v6.8.0: Deprecations
+
+In `ipfabric>=v6.8.0` the following has been changed/deprecated:
+
+- The use of `token='<TOKEN>'` or `username='<USER>', password='<PASS>'` in `IPFClient()` will be removed:
+  - Token: `IPFClient(auth='TOKEN')`
+  - User/Pass: `IPFClient(auth=('USER', 'PASS'))`
+  - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`
+- Methods found in `ipfabric.models.Device` class will no longer accept the `IPFClient` argument being passed.
+  - Example: `ipf.devices.all[0].interfaces(ipf)` -> `ipf.devices.all[0].interfaces()`
+- `IPFClient()._get_columns()` will be removed in place of `IPFClient().get_columns()`
+
 ## v6.5.0: Streaming Defaulted to True
 
 **STREAMING HAS BEEN DEFAULTED TO TRUE IN `v6.5.0`**
 
 In IP Fabric version `6.3.0` the option to return table data using a streaming
 GET request instead of a paginated POST request has been added.
```

### Comparing `ipfabric-6.7.3/pyproject.toml` & `ipfabric-6.8.0b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric"
-version = "v6.7.3"
+version = "v6.8.0b0"
 description = "Python package for interacting with IP Fabric"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
     "Solution Architecture <solution.architecture@ipfabric.io>"
 ]
 license = "MIT"
@@ -24,19 +24,18 @@
 pydantic = "^2.5.3"
 pydantic-settings = "^2.1.0"
 pydantic-extra-types = "^2.3.0"
 python-dateutil = "^2.8.2"
 pytz = ">=2023.1,<2025"
 python-dotenv = "^1.0"
 macaddress = "~2.0.2"
-deepdiff = "^6.7.1"
+deepdiff = ">=6.7.1, <8.0"  # TODO: Switch to v7 in 6.9
 case-insensitive-dictionary = "^0.2.1"
 importlib_resources = {version = "^5.13", python = "<3.9"}  # TODO: Remove after Python 3.8 https://importlib-resources.readthedocs.io/en/latest/using.html#migrating-from-legacy
 
-
 pandas = [
     {version = "^2.0.0", optional = true, python = "<3.9"},  # TODO: Remove after Python 3.8
     {version = "^2.1.4", optional = true, python = ">=3.9"}
 ]
 openpyxl = {version = "^3.1.2", optional = true}
 tabulate = {version = ">=0.8.9,<0.10.0",  optional = true}
 python-json-logger = {version = "^2.0.7",  optional = true}
```

### Comparing `ipfabric-6.7.3/README.md` & `ipfabric-6.8.0b0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 help enterprise network and security teams with network assurance and automation across multi-domain heterogeneous
 environments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP
 Fabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless
 digital transformation. 
 
 ## Upcoming Deprecation Notices
 
-In `ipfabric>=v6.8.0` the following will be changed/deprecated:
+In `ipfabric>=v6.8.0` the following has been changed/deprecated:
 
 - The use of `token='<TOKEN>'` or `username='<USER>', password='<PASS>'` in `IPFClient()` will be removed:
   - Token: `IPFClient(auth='TOKEN')`
   - User/Pass: `IPFClient(auth=('USER', 'PASS'))`
   - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`
 - Methods found in `ipfabric.models.Device` class will no longer accept the `IPFClient` argument being passed.
   - Example: `ipf.devices.all[0].interfaces(ipf)` -> `ipf.devices.all[0].interfaces()`
```

### Comparing `ipfabric-6.7.3/PKG-INFO` & `ipfabric-6.8.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric
-Version: 6.7.3
+Version: 6.8.0b0
 Summary: Python package for interacting with IP Fabric
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.8,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: examples
 Provides-Extra: pd
 Requires-Dist: case-insensitive-dictionary (>=0.2.1,<0.3.0)
-Requires-Dist: deepdiff (>=6.7.1,<7.0.0)
+Requires-Dist: deepdiff (>=6.7.1,<8.0)
 Requires-Dist: h2 (>=4.1.0,<5.0.0)
 Requires-Dist: httpx (>=0.26,<0.28)
 Requires-Dist: importlib_resources (>=5.13,<6.0) ; python_version < "3.9"
 Requires-Dist: macaddress (>=2.0.2,<2.1.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0) ; extra == "examples" or extra == "all"
 Requires-Dist: pandas (>=2.0.0,<3.0.0) ; (python_version < "3.9") and (extra == "examples" or extra == "pd" or extra == "all")
 Requires-Dist: pandas (>=2.1.4,<3.0.0) ; (python_version >= "3.9") and (extra == "examples" or extra == "pd" or extra == "all")
@@ -53,15 +53,15 @@
 help enterprise network and security teams with network assurance and automation across multi-domain heterogeneous
 environments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP
 Fabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless
 digital transformation. 
 
 ## Upcoming Deprecation Notices
 
-In `ipfabric>=v6.8.0` the following will be changed/deprecated:
+In `ipfabric>=v6.8.0` the following has been changed/deprecated:
 
 - The use of `token='<TOKEN>'` or `username='<USER>', password='<PASS>'` in `IPFClient()` will be removed:
   - Token: `IPFClient(auth='TOKEN')`
   - User/Pass: `IPFClient(auth=('USER', 'PASS'))`
   - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`
 - Methods found in `ipfabric.models.Device` class will no longer accept the `IPFClient` argument being passed.
   - Example: `ipf.devices.all[0].interfaces(ipf)` -> `ipf.devices.all[0].interfaces()`
```

