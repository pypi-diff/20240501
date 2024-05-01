# Comparing `tmp/carbon-black-cloud-sdk-1.5.1.tar.gz` & `tmp/carbon-black-cloud-sdk-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbon-black-cloud-sdk-1.5.1.tar", last modified: Tue Jan 30 18:32:19 2024, max compression
+gzip compressed data, was "carbon-black-cloud-sdk-1.5.2.tar", last modified: Wed May  1 16:18:37 2024, max compression
```

## Comparing `carbon-black-cloud-sdk-1.5.1.tar` & `carbon-black-cloud-sdk-1.5.2.tar`

### file list

```diff
@@ -1,142 +1,138 @@
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:19.119075 carbon-black-cloud-sdk-1.5.1/
--rw-rw-rw-   0        0        0     1094 2023-11-15 21:43:00.000000 carbon-black-cloud-sdk-1.5.1/LICENSE
--rw-rw-rw-   0        0        0       55 2023-08-14 15:19:35.000000 carbon-black-cloud-sdk-1.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7698 2024-01-30 18:32:19.120258 carbon-black-cloud-sdk-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     6760 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/README.md
--rw-rw-rw-   0        0        0        7 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/VERSION
--rw-rw-rw-   0        0        0      328 2024-01-30 18:32:19.125202 carbon-black-cloud-sdk-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     2325 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:17.958130 carbon-black-cloud-sdk-1.5.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:18.064710 carbon-black-cloud-sdk-1.5.1/src/carbon_black_cloud_sdk.egg-info/
--rw-rw-rw-   0        0        0     7698 2024-01-30 18:32:17.000000 carbon-black-cloud-sdk-1.5.1/src/carbon_black_cloud_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5391 2024-01-30 18:32:17.000000 carbon-black-cloud-sdk-1.5.1/src/carbon_black_cloud_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-30 18:32:17.000000 carbon-black-cloud-sdk-1.5.1/src/carbon_black_cloud_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-24 20:33:05.000000 carbon-black-cloud-sdk-1.5.1/src/carbon_black_cloud_sdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      322 2024-01-30 18:32:17.000000 carbon-black-cloud-sdk-1.5.1/src/carbon_black_cloud_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-30 18:32:17.000000 carbon-black-cloud-sdk-1.5.1/src/carbon_black_cloud_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:18.188244 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/
--rw-rw-rw-   0        0        0      275 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:18.229388 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/
--rw-rw-rw-   0        0        0      477 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/__init__.py
--rw-rw-rw-   0        0        0    67476 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/base.py
--rw-rw-rw-   0        0        0     9812 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/differential.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:18.268188 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/
--rw-rw-rw-   0        0        0     1765 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/device_summary.yaml
--rw-rw-rw-   0        0        0     2538 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/differential.yaml
--rw-rw-rw-   0        0        0      652 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/facet.yaml
--rw-rw-rw-   0        0        0     1217 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/result.yaml
--rw-rw-rw-   0        0        0     3989 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/run.yaml
--rw-rw-rw-   0        0        0     4212 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/template.yaml
--rw-rw-rw-   0        0        0    90065 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/base.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:18.293172 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/cache/
--rw-rw-rw-   0        0        0       50 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/cache/__init__.py
--rw-rw-rw-   0        0        0    11344 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/cache/lru.py
--rw-rw-rw-   0        0        0    35730 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/connection.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:18.393342 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/
--rw-rw-rw-   0        0        0      459 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/__init__.py
--rw-rw-rw-   0        0        0     2816 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/aws_sm_credential_provider.py
--rw-rw-rw-   0        0        0     2485 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/default.py
--rw-rw-rw-   0        0        0     2196 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/environ_credential_provider.py
--rw-rw-rw-   0        0        0     6531 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/file_credential_provider.py
--rw-rw-rw-   0        0        0     3517 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/keychain_credential_provider.py
--rw-rw-rw-   0        0        0     9173 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/registry_credential_provider.py
--rw-rw-rw-   0        0        0    10670 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credentials.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:18.448591 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/
--rw-rw-rw-   0        0        0      405 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/__init__.py
--rw-rw-rw-   0        0        0    21319 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/base.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:18.510484 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/
--rw-rw-rw-   0        0        0     4647 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/deviceInfo.yaml
--rw-rw-rw-   0        0        0     2189 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/enriched_event_facet.yaml
--rw-rw-rw-   0        0        0      358 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/policyInfo.yaml
--rw-rw-rw-   0        0        0     2997 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/recommendation.yaml
--rw-rw-rw-   0        0        0      153 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/recommendation_application.yaml
--rw-rw-rw-   0        0        0      543 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/recommendation_impact.yaml
--rw-rw-rw-   0        0        0      929 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/recommendation_new_rule.yaml
--rw-rw-rw-   0        0        0      686 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/recommendation_workflow.yaml
--rw-rw-rw-   0        0        0     2340 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/usbDevice.yaml
--rw-rw-rw-   0        0        0     1135 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/usbDeviceApproval.yaml
--rw-rw-rw-   0        0        0      425 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/usbDeviceBlock.yaml
--rw-rw-rw-   0        0        0    20836 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/recommendation.py
--rw-rw-rw-   0        0        0    36957 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/usb_device_control.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:18.563876 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/
--rw-rw-rw-   0        0        0      494 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/__init__.py
--rw-rw-rw-   0        0        0    29379 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/auth_events.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:18.615063 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/
--rw-rw-rw-   0        0        0     1189 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/auth_events.yaml
--rw-rw-rw-   0        0        0     2011 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/auth_events_facet.yaml
--rw-rw-rw-   0        0        0     2412 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/binary.yaml
--rw-rw-rw-   0        0        0      722 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/feed.yaml
--rw-rw-rw-   0        0        0      494 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/ioc_v2.yaml
--rw-rw-rw-   0        0        0      671 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/iocs.yaml
--rw-rw-rw-   0        0        0     1082 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/report.yaml
--rw-rw-rw-   0        0        0      248 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/report_severity.yaml
--rw-rw-rw-   0        0        0     1054 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/watchlist.yaml
--rw-rw-rw-   0        0        0    66298 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/threat_intelligence.py
--rw-rw-rw-   0        0        0     6586 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/ubs.py
--rw-rw-rw-   0        0        0    10648 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/errors.py
--rw-rw-rw-   0        0        0     7589 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/helpers.py
--rw-rw-rw-   0        0        0    60548 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/live_response_api.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:18.880474 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/
--rw-rw-rw-   0        0        0     1410 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/__init__.py
--rw-rw-rw-   0        0        0    74457 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/alerts.py
--rw-rw-rw-   0        0        0    30849 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/asset_groups.py
--rw-rw-rw-   0        0        0     1604 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/audit.py
--rw-rw-rw-   0        0        0     1642 2024-01-10 21:48:20.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/base.py
--rw-rw-rw-   0        0        0    52168 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/devices.py
--rw-rw-rw-   0        0        0    13540 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/events.py
--rw-rw-rw-   0        0        0    25992 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/grants.py
--rw-rw-rw-   0        0        0     9274 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/jobs.py
--rw-rw-rw-   0        0        0    40456 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/legacy_alerts.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:19.026948 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/
--rw-rw-rw-   0        0        0    22940 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/alert.yaml
--rw-rw-rw-   0        0        0    16748 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/alert_cb_analytic.yaml
--rw-rw-rw-   0        0        0     9391 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/alert_container_runtime.yaml
--rw-rw-rw-   0        0        0     8064 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/alert_device_control.yaml
--rw-rw-rw-   0        0        0    16249 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/alert_host_based_firewall.yaml
--rw-rw-rw-   0        0        0    16884 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/alert_intrusion_detection_system.yaml
--rw-rw-rw-   0        0        0      697 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/alert_note.yaml
--rw-rw-rw-   0        0        0    18200 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/alert_watchlist.yaml
--rw-rw-rw-   0        0        0     1268 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/asset_group.yaml
--rw-rw-rw-   0        0        0     9358 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/device.yaml
--rw-rw-rw-   0        0        0      487 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/device_facet.yaml
--rw-rw-rw-   0        0        0     1370 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/firewall_rule.yaml
--rw-rw-rw-   0        0        0      310 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/firewall_rule_group.yaml
--rw-rw-rw-   0        0        0     2627 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/grant.yaml
--rw-rw-rw-   0        0        0     2108 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/grouped_alert.yaml
--rw-rw-rw-   0        0        0     1461 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/job.yaml
--rw-rw-rw-   0        0        0      530 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/network_threat_metadata.yaml
--rw-rw-rw-   0        0        0     1491 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/observation.yaml
--rw-rw-rw-   0        0        0     2011 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/observation_facet.yaml
--rw-rw-rw-   0        0        0     6118 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/policy.yaml
--rw-rw-rw-   0        0        0     1173 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/policy_rule.yaml
--rw-rw-rw-   0        0        0      547 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/policy_ruleconfig.yaml
--rw-rw-rw-   0        0        0     2184 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/process_facets.yaml
--rw-rw-rw-   0        0        0     1288 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/profile.yaml
--rw-rw-rw-   0        0        0     1378 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/reputation_override.yaml
--rw-rw-rw-   0        0        0      395 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/stub.yaml
--rw-rw-rw-   0        0        0     1145 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/user.yaml
--rw-rw-rw-   0        0        0      998 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/workflow.yaml
--rw-rw-rw-   0        0        0     2711 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/network_threat_metadata.py
--rw-rw-rw-   0        0        0    27265 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/observations.py
--rw-rw-rw-   0        0        0    73326 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/policies.py
--rw-rw-rw-   0        0        0    30547 2024-01-18 23:25:26.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/policy_ruleconfigs.py
--rw-rw-rw-   0        0        0     4633 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/previewer.py
--rw-rw-rw-   0        0        0    44565 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/processes.py
--rw-rw-rw-   0        0        0    11751 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/reputation.py
--rw-rw-rw-   0        0        0    25022 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/users.py
--rw-rw-rw-   0        0        0    40913 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/vulnerability_assessment.py
--rw-rw-rw-   0        0        0    21817 2024-01-30 18:27:56.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/rest_api.py
--rw-rw-rw-   0        0        0     1455 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/utils.py
--rw-rw-rw-   0        0        0   118761 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/winerror.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:19.079472 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/
--rw-rw-rw-   0        0        0      457 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 18:32:19.115301 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/
--rw-rw-rw-   0        0        0     2560 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/computeResource.yaml
--rw-rw-rw-   0        0        0     1666 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/deviceVulnerabilitySummary.yaml
--rw-rw-rw-   0        0        0     1316 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/sensorKit.yaml
--rw-rw-rw-   0        0        0     5047 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/vulnerability.yaml
--rw-rw-rw-   0        0        0     1765 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/vulnerabilityAssetView.yaml
--rw-rw-rw-   0        0        0    11959 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/vulnerabilityOrgSummary.yaml
--rw-rw-rw-   0        0        0     5557 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/nsx_remediation.py
--rw-rw-rw-   0        0        0    11414 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/sensor_lifecycle.py
--rw-rw-rw-   0        0        0    71251 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/vm_workloads_search.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:37.296576 carbon-black-cloud-sdk-1.5.2/
+-rw-rw-rw-   0        0        0     1094 2023-11-15 21:43:00.000000 carbon-black-cloud-sdk-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-08-14 15:19:35.000000 carbon-black-cloud-sdk-1.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7693 2024-05-01 16:18:37.296576 carbon-black-cloud-sdk-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6755 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/README.md
+-rw-rw-rw-   0        0        0        7 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/VERSION
+-rw-rw-rw-   0        0        0      328 2024-05-01 16:18:37.296576 carbon-black-cloud-sdk-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     2325 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:35.817829 carbon-black-cloud-sdk-1.5.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:35.912195 carbon-black-cloud-sdk-1.5.2/src/carbon_black_cloud_sdk.egg-info/
+-rw-rw-rw-   0        0        0     7693 2024-05-01 16:18:35.000000 carbon-black-cloud-sdk-1.5.2/src/carbon_black_cloud_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5159 2024-05-01 16:18:35.000000 carbon-black-cloud-sdk-1.5.2/src/carbon_black_cloud_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 16:18:35.000000 carbon-black-cloud-sdk-1.5.2/src/carbon_black_cloud_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-24 20:33:05.000000 carbon-black-cloud-sdk-1.5.2/src/carbon_black_cloud_sdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      322 2024-05-01 16:18:35.000000 carbon-black-cloud-sdk-1.5.2/src/carbon_black_cloud_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-01 16:18:35.000000 carbon-black-cloud-sdk-1.5.2/src/carbon_black_cloud_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:36.084581 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/
+-rw-rw-rw-   0        0        0      275 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:36.147861 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/
+-rw-rw-rw-   0        0        0      477 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/__init__.py
+-rw-rw-rw-   0        0        0    67672 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/base.py
+-rw-rw-rw-   0        0        0     9812 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/differential.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:36.210611 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/
+-rw-rw-rw-   0        0        0     1765 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/device_summary.yaml
+-rw-rw-rw-   0        0        0     2538 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/differential.yaml
+-rw-rw-rw-   0        0        0      652 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/facet.yaml
+-rw-rw-rw-   0        0        0     1217 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/result.yaml
+-rw-rw-rw-   0        0        0     3989 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/run.yaml
+-rw-rw-rw-   0        0        0     4212 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/template.yaml
+-rw-rw-rw-   0        0        0    90717 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/base.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:36.241946 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/cache/
+-rw-rw-rw-   0        0        0       50 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/cache/__init__.py
+-rw-rw-rw-   0        0        0    11344 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/cache/lru.py
+-rw-rw-rw-   0        0        0    35730 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/connection.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:36.382042 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/
+-rw-rw-rw-   0        0        0      459 2023-08-14 15:19:36.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/__init__.py
+-rw-rw-rw-   0        0        0     2816 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/aws_sm_credential_provider.py
+-rw-rw-rw-   0        0        0     2485 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/default.py
+-rw-rw-rw-   0        0        0     2196 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/environ_credential_provider.py
+-rw-rw-rw-   0        0        0     7948 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/file_credential_provider.py
+-rw-rw-rw-   0        0        0     3517 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/keychain_credential_provider.py
+-rw-rw-rw-   0        0        0     9173 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/registry_credential_provider.py
+-rw-rw-rw-   0        0        0    10670 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credentials.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:36.470664 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/
+-rw-rw-rw-   0        0        0      405 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/__init__.py
+-rw-rw-rw-   0        0        0    21319 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/base.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:36.554753 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/
+-rw-rw-rw-   0        0        0     4647 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/deviceInfo.yaml
+-rw-rw-rw-   0        0        0     2189 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/enriched_event_facet.yaml
+-rw-rw-rw-   0        0        0      358 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/policyInfo.yaml
+-rw-rw-rw-   0        0        0     2997 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/recommendation.yaml
+-rw-rw-rw-   0        0        0      153 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/recommendation_application.yaml
+-rw-rw-rw-   0        0        0      543 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/recommendation_impact.yaml
+-rw-rw-rw-   0        0        0      929 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/recommendation_new_rule.yaml
+-rw-rw-rw-   0        0        0      686 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/recommendation_workflow.yaml
+-rw-rw-rw-   0        0        0     2340 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/usbDevice.yaml
+-rw-rw-rw-   0        0        0     1135 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/usbDeviceApproval.yaml
+-rw-rw-rw-   0        0        0      425 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/usbDeviceBlock.yaml
+-rw-rw-rw-   0        0        0    20836 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/recommendation.py
+-rw-rw-rw-   0        0        0    36957 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/usb_device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:36.620799 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/
+-rw-rw-rw-   0        0        0      494 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/__init__.py
+-rw-rw-rw-   0        0        0    29379 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/auth_events.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:36.688604 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/
+-rw-rw-rw-   0        0        0     1189 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/auth_events.yaml
+-rw-rw-rw-   0        0        0     2011 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/auth_events_facet.yaml
+-rw-rw-rw-   0        0        0     2412 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/binary.yaml
+-rw-rw-rw-   0        0        0      722 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/feed.yaml
+-rw-rw-rw-   0        0        0      494 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/ioc_v2.yaml
+-rw-rw-rw-   0        0        0      671 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/iocs.yaml
+-rw-rw-rw-   0        0        0     1082 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/report.yaml
+-rw-rw-rw-   0        0        0      248 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/report_severity.yaml
+-rw-rw-rw-   0        0        0     1054 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/watchlist.yaml
+-rw-rw-rw-   0        0        0    66298 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/threat_intelligence.py
+-rw-rw-rw-   0        0        0     6586 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/ubs.py
+-rw-rw-rw-   0        0        0    10648 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/errors.py
+-rw-rw-rw-   0        0        0     7589 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/helpers.py
+-rw-rw-rw-   0        0        0    60548 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/live_response_api.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:37.000892 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/
+-rw-rw-rw-   0        0        0     1410 2024-04-29 16:31:52.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/__init__.py
+-rw-rw-rw-   0        0        0    80450 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/alerts.py
+-rw-rw-rw-   0        0        0    30849 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/asset_groups.py
+-rw-rw-rw-   0        0        0    16559 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/audit.py
+-rw-rw-rw-   0        0        0     1642 2024-01-10 21:48:20.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/base.py
+-rw-rw-rw-   0        0        0    52106 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/devices.py
+-rw-rw-rw-   0        0        0    13826 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/events.py
+-rw-rw-rw-   0        0        0    25992 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/grants.py
+-rw-rw-rw-   0        0        0    10024 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/jobs.py
+-rw-rw-rw-   0        0        0    40456 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/legacy_alerts.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:37.157252 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/
+-rw-rw-rw-   0        0        0      697 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/alert_note.yaml
+-rw-rw-rw-   0        0        0     1268 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/asset_group.yaml
+-rw-rw-rw-   0        0        0      836 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/audit_log.yaml
+-rw-rw-rw-   0        0        0     9358 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/device.yaml
+-rw-rw-rw-   0        0        0      487 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/device_facet.yaml
+-rw-rw-rw-   0        0        0     1370 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/firewall_rule.yaml
+-rw-rw-rw-   0        0        0      310 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/firewall_rule_group.yaml
+-rw-rw-rw-   0        0        0     2627 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/grant.yaml
+-rw-rw-rw-   0        0        0     2108 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/grouped_alert.yaml
+-rw-rw-rw-   0        0        0     1461 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/job.yaml
+-rw-rw-rw-   0        0        0      530 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/network_threat_metadata.yaml
+-rw-rw-rw-   0        0        0     1491 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/observation.yaml
+-rw-rw-rw-   0        0        0     2011 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/observation_facet.yaml
+-rw-rw-rw-   0        0        0     6118 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/policy.yaml
+-rw-rw-rw-   0        0        0     1173 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/policy_rule.yaml
+-rw-rw-rw-   0        0        0      646 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/policy_ruleconfig.yaml
+-rw-rw-rw-   0        0        0     2184 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/process_facets.yaml
+-rw-rw-rw-   0        0        0     1288 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/profile.yaml
+-rw-rw-rw-   0        0        0     1378 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/reputation_override.yaml
+-rw-rw-rw-   0        0        0      395 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/stub.yaml
+-rw-rw-rw-   0        0        0     1145 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/user.yaml
+-rw-rw-rw-   0        0        0      998 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/workflow.yaml
+-rw-rw-rw-   0        0        0     2711 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/network_threat_metadata.py
+-rw-rw-rw-   0        0        0    27344 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/observations.py
+-rw-rw-rw-   0        0        0    74237 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/policies.py
+-rw-rw-rw-   0        0        0    34781 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/policy_ruleconfigs.py
+-rw-rw-rw-   0        0        0     4633 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/previewer.py
+-rw-rw-rw-   0        0        0    45818 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/processes.py
+-rw-rw-rw-   0        0        0    11751 2024-04-26 20:40:55.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/reputation.py
+-rw-rw-rw-   0        0        0    25022 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/users.py
+-rw-rw-rw-   0        0        0    41089 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/vulnerability_assessment.py
+-rw-rw-rw-   0        0        0    21817 2024-04-29 16:31:52.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/rest_api.py
+-rw-rw-rw-   0        0        0     7195 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/utils.py
+-rw-rw-rw-   0        0        0   118761 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/winerror.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:37.235379 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/
+-rw-rw-rw-   0        0        0      531 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/__init__.py
+-rw-rw-rw-   0        0        0    21887 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/compliance_assessment.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:18:37.296576 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/
+-rw-rw-rw-   0        0        0     1799 2024-05-01 16:15:29.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/compliance_benchmark.yaml
+-rw-rw-rw-   0        0        0     2560 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/computeResource.yaml
+-rw-rw-rw-   0        0        0     1666 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/deviceVulnerabilitySummary.yaml
+-rw-rw-rw-   0        0        0     1316 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/sensorKit.yaml
+-rw-rw-rw-   0        0        0     5047 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/vulnerability.yaml
+-rw-rw-rw-   0        0        0     1765 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/vulnerabilityAssetView.yaml
+-rw-rw-rw-   0        0        0    11959 2023-08-14 15:19:37.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/vulnerabilityOrgSummary.yaml
+-rw-rw-rw-   0        0        0     5557 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/nsx_remediation.py
+-rw-rw-rw-   0        0        0    11414 2023-11-15 21:43:01.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/sensor_lifecycle.py
+-rw-rw-rw-   0        0        0    71251 2024-04-26 20:40:56.000000 carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/vm_workloads_search.py
```

### Comparing `carbon-black-cloud-sdk-1.5.1/LICENSE` & `carbon-black-cloud-sdk-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/PKG-INFO` & `carbon-black-cloud-sdk-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-black-cloud-sdk
-Version: 1.5.1
+Version: 1.5.2
 Summary: VMware Carbon Black Cloud Python SDK
 Home-page: https://github.com/carbonblack/carbon-black-cloud-sdk-python
 Author: VMware Carbon Black
 Author-email: cb-developer-network@vmware.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -20,17 +20,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # VMware Carbon Black Cloud Python SDK
 
-**Latest Version:** 1.5.1
+**Latest Version:** 1.5.2
 <br>
-**Release Date:** January 30, 2024
+**Release Date:** May 1, 2024
 
 [![Coverage Status](https://coveralls.io/repos/github/carbonblack/carbon-black-cloud-sdk-python/badge.svg?t=Id6Baf)](https://coveralls.io/github/carbonblack/carbon-black-cloud-sdk-python)
 [![Codeship Status for carbonblack/carbon-black-cloud-sdk-python](https://app.codeship.com/projects/9e55a370-a772-0138-aae4-129773225755/status?branch=develop)](https://app.codeship.com/projects/402767)
 
 
 
 ## Recent updates
```

### Comparing `carbon-black-cloud-sdk-1.5.1/README.md` & `carbon-black-cloud-sdk-1.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # VMware Carbon Black Cloud Python SDK
 
-**Latest Version:** 1.5.1
+**Latest Version:** 1.5.2
 <br>
-**Release Date:** January 30, 2024
+**Release Date:** May 1, 2024
 
 [![Coverage Status](https://coveralls.io/repos/github/carbonblack/carbon-black-cloud-sdk-python/badge.svg?t=Id6Baf)](https://coveralls.io/github/carbonblack/carbon-black-cloud-sdk-python)
 [![Codeship Status for carbonblack/carbon-black-cloud-sdk-python](https://app.codeship.com/projects/9e55a370-a772-0138-aae4-129773225755/status?branch=develop)](https://app.codeship.com/projects/402767)
 
 
 
 ## Recent updates
```

### Comparing `carbon-black-cloud-sdk-1.5.1/setup.py` & `carbon-black-cloud-sdk-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/carbon_black_cloud_sdk.egg-info/PKG-INFO` & `carbon-black-cloud-sdk-1.5.2/src/carbon_black_cloud_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-black-cloud-sdk
-Version: 1.5.1
+Version: 1.5.2
 Summary: VMware Carbon Black Cloud Python SDK
 Home-page: https://github.com/carbonblack/carbon-black-cloud-sdk-python
 Author: VMware Carbon Black
 Author-email: cb-developer-network@vmware.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -20,17 +20,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # VMware Carbon Black Cloud Python SDK
 
-**Latest Version:** 1.5.1
+**Latest Version:** 1.5.2
 <br>
-**Release Date:** January 30, 2024
+**Release Date:** May 1, 2024
 
 [![Coverage Status](https://coveralls.io/repos/github/carbonblack/carbon-black-cloud-sdk-python/badge.svg?t=Id6Baf)](https://coveralls.io/github/carbonblack/carbon-black-cloud-sdk-python)
 [![Codeship Status for carbonblack/carbon-black-cloud-sdk-python](https://app.codeship.com/projects/9e55a370-a772-0138-aae4-129773225755/status?branch=develop)](https://app.codeship.com/projects/402767)
 
 
 
 ## Recent updates
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/carbon_black_cloud_sdk.egg-info/SOURCES.txt` & `carbon-black-cloud-sdk-1.5.2/src/carbon_black_cloud_sdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -81,23 +81,17 @@
 src/cbc_sdk/platform/policies.py
 src/cbc_sdk/platform/policy_ruleconfigs.py
 src/cbc_sdk/platform/previewer.py
 src/cbc_sdk/platform/processes.py
 src/cbc_sdk/platform/reputation.py
 src/cbc_sdk/platform/users.py
 src/cbc_sdk/platform/vulnerability_assessment.py
-src/cbc_sdk/platform/models/alert.yaml
-src/cbc_sdk/platform/models/alert_cb_analytic.yaml
-src/cbc_sdk/platform/models/alert_container_runtime.yaml
-src/cbc_sdk/platform/models/alert_device_control.yaml
-src/cbc_sdk/platform/models/alert_host_based_firewall.yaml
-src/cbc_sdk/platform/models/alert_intrusion_detection_system.yaml
 src/cbc_sdk/platform/models/alert_note.yaml
-src/cbc_sdk/platform/models/alert_watchlist.yaml
 src/cbc_sdk/platform/models/asset_group.yaml
+src/cbc_sdk/platform/models/audit_log.yaml
 src/cbc_sdk/platform/models/device.yaml
 src/cbc_sdk/platform/models/device_facet.yaml
 src/cbc_sdk/platform/models/firewall_rule.yaml
 src/cbc_sdk/platform/models/firewall_rule_group.yaml
 src/cbc_sdk/platform/models/grant.yaml
 src/cbc_sdk/platform/models/grouped_alert.yaml
 src/cbc_sdk/platform/models/job.yaml
@@ -110,16 +104,18 @@
 src/cbc_sdk/platform/models/process_facets.yaml
 src/cbc_sdk/platform/models/profile.yaml
 src/cbc_sdk/platform/models/reputation_override.yaml
 src/cbc_sdk/platform/models/stub.yaml
 src/cbc_sdk/platform/models/user.yaml
 src/cbc_sdk/platform/models/workflow.yaml
 src/cbc_sdk/workload/__init__.py
+src/cbc_sdk/workload/compliance_assessment.py
 src/cbc_sdk/workload/nsx_remediation.py
 src/cbc_sdk/workload/sensor_lifecycle.py
 src/cbc_sdk/workload/vm_workloads_search.py
+src/cbc_sdk/workload/models/compliance_benchmark.yaml
 src/cbc_sdk/workload/models/computeResource.yaml
 src/cbc_sdk/workload/models/deviceVulnerabilitySummary.yaml
 src/cbc_sdk/workload/models/sensorKit.yaml
 src/cbc_sdk/workload/models/vulnerability.yaml
 src/cbc_sdk/workload/models/vulnerabilityAssetView.yaml
 src/cbc_sdk/workload/models/vulnerabilityOrgSummary.yaml
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/base.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -996,50 +996,50 @@
         result = resp.json()
 
         self._total_results = result["num_found"]
         self._count_valid = True
 
         return self._total_results
 
-    def _perform_query(self, start=0, rows=0):
+    def _perform_query(self, from_row=0, max_rows=0):
         """
         Performs the query and returns the results of the query in an iterable fashion.
 
         Args:
-            start (int): The row to start the query at (default 0).
-            rows (int): The maximum number of rows to be returned (default 0, meaning "all").
+            from_row (int): The row to start the query at (default 0).
+            max_rows (int): The maximum number of rows to be returned (default 0, meaning "all").
 
         Returns:
             Iterable: The iterated query.
         """
         url = self._doc_class.urlobject_history.format(
             self._cb.credentials.org_key
         )
-        current = start
+        current = from_row
         numrows = 0
         still_querying = True
         while still_querying:
-            request = self._build_request(start, rows)
+            request = self._build_request(from_row, max_rows)
             resp = self._cb.post_object(url, body=request)
             result = resp.json()
 
             self._total_results = result["num_found"]
             self._count_valid = True
 
             results = result.get("results", [])
             for item in results:
                 yield self._doc_class(self._cb, item)
                 current += 1
                 numrows += 1
 
-                if rows and numrows == rows:
+                if max_rows and numrows == max_rows:
                     still_querying = False
                     break
 
-            start = current
+            from_row = current
             if current >= self._total_results:
                 still_querying = False
                 break
 
     def _run_async_query(self, context):
         """
         Executed in the background to run an asynchronous query. Must be implemented in any inheriting classes.
@@ -1308,55 +1308,55 @@
         result = resp.json()
 
         self._total_results = result["num_found"]
         self._count_valid = True
 
         return self._total_results
 
-    def _perform_query(self, start=0, rows=0):
+    def _perform_query(self, from_row=0, max_rows=0):
         """
         Performs the query and returns the results of the query in an iterable fashion.
 
         Args:
-            start (int): The row to start the query at (default 0).
-            rows (int): The maximum number of rows to be returned (default 0, meaning "all").
+            from_row (int): The row to start the query at (default 0).
+            max_rows (int): The maximum number of rows to be returned (default 0, meaning "all").
 
         Returns:
             Iterable: The iterated query.
         """
         if self._run_id is None:
             raise ApiError("Can't retrieve results without a run ID")
 
         url = self._doc_class.urlobject.format(
             self._cb.credentials.org_key, self._run_id
         )
-        current = start
+        current = from_row
         numrows = 0
         still_querying = True
         while still_querying:
-            request = self._build_request(start, rows)
+            request = self._build_request(from_row, max_rows)
             resp = self._cb.post_object(url, body=request)
             result = resp.json()
 
             self._total_results = result["num_found"]
             if self._total_results > MAX_RESULTS_LIMIT:
                 self._total_results = MAX_RESULTS_LIMIT
             self._count_valid = True
 
             results = result.get("results", [])
             for item in results:
                 yield self._doc_class(self._cb, item)
                 current += 1
                 numrows += 1
 
-                if rows and numrows == rows:
+                if max_rows and numrows == max_rows:
                     still_querying = False
                     break
 
-            start = current
+            from_row = current
             if current >= self._total_results:
                 still_querying = False
                 break
 
     def scroll(self, rows=10000):
         """
         Iteratively fetch results across Live Query Runs or paginate all results beyond the 10k search limits.
@@ -1718,31 +1718,32 @@
         query = self._query_builder._collapse()
         if query:
             request["query"] = query
         if self._criteria:
             request["criteria"] = self._criteria
         return request
 
-    def _perform_query(self, rows=0):
+    def _perform_query(self, from_row=0, max_rows=0):
         """
         Performs the query and returns the results of the query in an iterable fashion.
 
         Args:
-            rows (int): The maximum number of rows to be returned (default 0, meaning "all").
+            from_row (int): Not used, inserted for compatibility.
+            max_rows (int): The maximum number of rows to be returned (default 0, meaning "all").
 
         Returns:
             Iterable: The iterated query.
         """
         if self._run_id is None:
             raise ApiError("Can't retrieve results without a run ID")
 
         url = self._doc_class.urlobject.format(
             self._cb.credentials.org_key, self._run_id
         )
-        request = self._build_request(rows)
+        request = self._build_request(max_rows)
         resp = self._cb.post_object(url, body=request)
         result = resp.json()
         results = result.get("terms", [])
         for item in results:
             yield self._doc_class(self._cb, item)
 
     def _init_async_query(self):
@@ -1853,50 +1854,50 @@
         result = resp.json()
 
         self._total_results = result["num_found"]
         self._count_valid = True
 
         return self._total_results
 
-    def _perform_query(self, start=0, rows=0):
+    def _perform_query(self, from_row=0, max_rows=0):
         """
         Performs the query and returns the results of the query in an iterable fashion.
 
         Args:
-            start (int): The row to start the query at (default 0).
-            rows (int): The maximum number of rows to be returned (default 0, meaning "all").
+            from_row (int): The row to start the query at (default 0).
+            max_rows (int): The maximum number of rows to be returned (default 0, meaning "all").
 
         Returns:
             Iterable: The iterated query.
         """
         url = self._doc_class.urlobject_history.format(
             self._cb.credentials.org_key
         )
-        current = start
+        current = from_row
         numrows = 0
         still_querying = True
         while still_querying:
-            request = self._build_request(start, rows)
+            request = self._build_request(from_row, max_rows)
             resp = self._cb.post_object(url, body=request)
             result = resp.json()
 
             self._total_results = result["num_found"]
             self._count_valid = True
 
             results = result.get("results", [])
             for item in results:
                 yield self._doc_class(self._cb, item)
                 current += 1
                 numrows += 1
 
-                if rows and numrows == rows:
+                if max_rows and numrows == max_rows:
                     still_querying = False
                     break
 
-            start = current
+            from_row = current
             if current >= self._total_results:
                 still_querying = False
                 break
 
     def _run_async_query(self, context):
         """
         Executed in the background to run an asynchronous query. Must be implemented in any inheriting classes.
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/differential.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/differential.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/device_summary.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/device_summary.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/differential.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/differential.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/facet.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/facet.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/result.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/result.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/run.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/run.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/audit_remediation/models/template.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/audit_remediation/models/template.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/base.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                 setattr(cls, field_name, FieldDescriptor(field_name, coerce_to=float))
             elif field_format == "byte":
                 setattr(cls, field_name, BinaryFieldDescriptor(field_name))
             else:
                 setattr(cls, field_name, FieldDescriptor(field_name))
 
         for fk_name, fk_info in iter(foreign_keys.items()):
-            setattr(cls, fk_name, ForeignKeyFieldDescriptor(fk_name, fk_info[0], fk_info[1]))
+            setattr(cls, fk_name, ForeignKeyFieldDescriptor(fk_name, fk_info[0], fk_info[1]))  # pragma: no cover
 
         return cls
 
 
 class FieldDescriptor(object):
     """Object that describes a field within a model instance."""
     def __init__(self, field_name, coerce_to=None, default_value=None):
@@ -786,14 +786,18 @@
 class UnrefreshableModel(NewBaseModel):
     """Represents a model that can't be refreshed, i.e. for which ``reset()`` is not a valid operation."""
 
     def refresh(self):  # pragma: no cover
         """Reload this object from the server."""
         raise ApiError("refresh() called on an unrefreshable model")
 
+    def _refresh(self):
+        """Override protected refresh"""
+        pass
+
 
 class MutableBaseModel(NewBaseModel):
     """Base model for objects that can have properties changed and then saved back to the server."""
     _new_object_http_method = "POST"
     _change_object_http_method = "PUT"
     _new_object_needs_primary_key = False
 
@@ -1018,15 +1022,15 @@
             query (solrq.Q): The parent query of this one.
         """
         self._query = query
 
     def _clone(self):
         return self.__class__(self._query)
 
-    def _perform_query(self):
+    def _perform_query(self, from_row=0, max_rows=-1):
         # This has the effect of generating an empty iterator.
         yield from ()
 
 
 class IterableQueryMixin:
     """A mix-in to provide iterability to a query."""
 
@@ -1042,37 +1046,32 @@
     def first(self):
         """
         Returns the first item that would be returned as the result of a query.
 
         Returns:
             obj: First query item
         """
-        res = self[:1]
-        if res is None or not len(res):
-            return None
-        return res[0]
+        return self.__getitem__(0)
 
     def one(self):
         """
         Returns the only item that would be returned by a query.
 
         Returns:
             obj: Sole query return item
 
         Raises:
             MoreThanOneResultError: If the query returns more than one item
             ObjectNotFoundError: If the query returns zero items
         """
-        res = self[:2]
-        if res is None:
-            return None
+        res = list(self._perform_query(from_row=0, max_rows=2))
         label = str(self._query) if self._query else "<unspecified>"
         if len(res) == 0:
             raise ObjectNotFoundError("query_uri", message="0 results for query {0:s}".format(label))
-        if len(res) > 1:
+        if len(res) > 1:  # pragma: no cover
             raise MoreThanOneResultError(
                 message="{0:d} results found for query {1:s}".format(len(self), label),
                 results=self.all()
             )
         return res[0]
 
     def __len__(self):
@@ -1107,16 +1106,16 @@
                     return results
             except TypeError:
                 log.debug(f"Unable to perform optimized query for {self.__class__.__name__}")
             results = list(self)
             return [results[ii] for ii in range(*item.indices(len(results)))]
         elif isinstance(item, int):
             results = list(self._perform_query(from_row=item, max_rows=1))
-            return results[item]
-        else:
+            return results[0]
+        else:  # pragma: no cover
             raise TypeError("Invalid argument type")
 
     def __iter__(self):
         """
         Returns an iterator over the items returned by this query.
 
         Returns:
@@ -1254,17 +1253,23 @@
         Returns:
             SimpleQuery: A new query with the extra "where" clause specified.
         """
         if not self._multiple_where_clauses_accepted:
             raise ApiError("Cannot have multiple 'where' clauses")
         return self.where(new_query)
 
-    def _perform_query(self):
-        for item in self.results:
+    def _perform_query(self, from_row=0, max_rows=-1):
+        returned_rows = 0
+        for index, item in enumerate(self.results):
+            if index < from_row:
+                continue
             yield item
+            returned_rows += 1
+            if 0 < max_rows <= returned_rows:
+                break
 
     def sort(self, new_sort):
         """
         Set the sorting for this query.
 
         Args:
             new_sort (object): The new sort criteria for this query.
@@ -1365,16 +1370,16 @@
             try:
                 return next(self._perform_query(item, 1))
             except StopIteration:
                 return None
         else:
             raise TypeError("invalid type")
 
-    def _perform_query(self, start=0, numrows=0):
-        for item in self._search(start=start, rows=numrows):
+    def _perform_query(self, from_row=0, max_rows=0):
+        for item in self._search(start=from_row, rows=max_rows):
             yield self._doc_class._new_object(self._cb, item)
 
     def batch_size(self, new_batch_size):
         """
         Set the batch size of the paginated query.
 
         Args:
@@ -1861,14 +1866,15 @@
         self._sort_by = []
         self._group_by = None
         self._batch_size = 500
         self._start = 0
         self._time_range = {}
         self._fields = ["*"]
         self._default_args = {}
+        self._collapse_field = []
 
     def _add_exclusions(self, key, newlist):
         """
         Updates a list of exclusion being collected for a query, by setting or appending items.
 
         Args:
             key (str): The key for the exclusion item to be set.
@@ -1964,14 +1970,16 @@
         if query:
             args['query'] = query
         if self._query_builder._process_guid is not None:
             args["process_guid"] = self._query_builder._process_guid
         if 'process_guid:' in args.get('query', ''):
             q = args['query'].split('process_guid:', 1)[1].split(' ', 1)[0]
             args["process_guid"] = q
+        if self._collapse_field:
+            args['collapse_field'] = self._collapse_field
 
         if args.get("sort", None) is not None and args.get("fields", None) is None:
             # Add default fields if only sort is specified
             args["fields"] = ["*"]
 
         return args
 
@@ -2404,16 +2412,21 @@
             query_parameters = {"limit": self._limit}
         else:
             query_parameters = {}
 
         result = self._cb.get_object(result_url, query_parameters=query_parameters)
         return self._doc_class(self._cb, model_unique_id=self._query_token, initial_data=result)
 
-    def _perform_query(self):
-        return self.results
+    def _perform_query(self, from_row=0, max_rows=-1):
+        if max_rows > 0:
+            return self.results[from_row:from_row + max_rows]
+        elif from_row > 0:
+            return self.results[from_row:]
+        else:
+            return self.results
 
     @property
     def results(self):
         """Save query results to self._results with self._search() method."""
         if not self._full_init:
             self._results = self._search()
             self._full_init = True
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/cache/lru.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/cache/lru.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/connection.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/connection.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/aws_sm_credential_provider.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/aws_sm_credential_provider.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/default.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/default.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/environ_credential_provider.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/environ_credential_provider.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/file_credential_provider.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/file_credential_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # * WARRANTIES OR CONDITIONS OF ANY KIND, WHETHER ORAL OR WRITTEN,
 # * EXPRESS OR IMPLIED. THE AUTHOR SPECIFICALLY DISCLAIMS ANY IMPLIED
 # * WARRANTIES OR CONDITIONS OF MERCHANTABILITY, SATISFACTORY QUALITY,
 # * NON-INFRINGEMENT AND FITNESS FOR A PARTICULAR PURPOSE.
 
 """Credentials provider that reads the credentials from a file."""
 
+import codecs
 import configparser
 import logging
 import os
 import sys
 from pathlib import Path
 from cbc_sdk.credentials import Credentials, CredentialProvider
 from cbc_sdk.errors import CredentialError
@@ -60,15 +61,15 @@
 
         Args:
             path (Path): The path to get the status of.
 
         Returns:
             os.stat_result: The resulting status.
         """
-        return path.stat()
+        return path.stat()  # pragma: no cover
 
     def _security_check(self, path):
         """
         Perform a security check on the specified path object.
 
         Args:
             path (Path): The path to be security-checked.
@@ -108,14 +109,39 @@
                 if self._specific_file_warn:
                     log.warning("Security warning: A future version of CBC SDK will disallow access to "
                                 "the following files altogether unless their permissions are updated.")
                     self._specific_file_warn = False
                 log.warning("Security warning: " + failmsg)
             return True
 
+    @staticmethod
+    def _get_encoding(file):
+        """
+        Detects which encoding a file is in.
+
+        Args:
+            file (Path): The file to be tested.
+
+        Returns:
+            str: The (possibly-guessed) encoding for the file.
+        """
+        try:
+            with open(file, "rb") as f:
+                prefix = bytearray(f.read(5))
+                if prefix.startswith(codecs.BOM_UTF8):
+                    return "utf_8_sig"
+                if prefix.startswith(codecs.BOM_UTF16_LE):
+                    return "utf_16_le"
+                if prefix.startswith(codecs.BOM_UTF16_BE):
+                    return "utf_16_be"
+                return "utf_8"
+        except OSError:  # pragma: no cover
+            log.warning(f"unable to read encoding of file {file}, assuming utf_8 encoding")
+            return "utf_8"
+
     def get_credentials(self, section=None):
         """
         Return a Credentials object containing the configured credentials.
 
         Args:
             section (str): The credential section to retrieve.
 
@@ -128,19 +154,28 @@
         if section is None:
             section = 'default'
         if self._cached_credentials is None:
             new_creds = {}
             cred_files = [p for p in self._search_path if self._security_check(p)]
             if not cred_files:
                 raise CredentialError(f"Unable to locate credential file(s) from {self._search_path}")
-            raw_cred_files = [str(p) for p in cred_files]  # needed to support 3.6.0 correctly & for error message
             try:
                 parser = configparser.ConfigParser()
-                parser.read(raw_cred_files)
+                for file in cred_files:
+                    encoding = self._get_encoding(file)
+                    if encoding.startswith("utf_16"):
+                        with open(file, 'rt', encoding=encoding) as f:
+                            # skip the BOM at the start of the file, because that seems to break ConfigParser
+                            ch = f.read(1)
+                            assert ch == "\ufeff"
+                            parser.read_file(f, source=str(file))
+                    else:
+                        # use string as filename parameter to maintain compatibility
+                        parser.read(str(file), encoding=encoding)
                 for sect in parser.sections():
                     new_creds[sect] = Credentials({name: value for (name, value) in parser.items(sect)})
             except configparser.Error as e:
-                raise CredentialError(f"Unable to read credential file(s) {raw_cred_files}") from e
+                raise CredentialError(f"Unable to read credential file(s) {cred_files}") from e
             self._cached_credentials = new_creds
         if section in self._cached_credentials:
             return self._cached_credentials[section]
         raise CredentialError(f"Section {section} not found in credential file(s)")
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/keychain_credential_provider.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/keychain_credential_provider.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credential_providers/registry_credential_provider.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credential_providers/registry_credential_provider.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/credentials.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/credentials.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/base.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/base.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/deviceInfo.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/deviceInfo.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/enriched_event_facet.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/enriched_event_facet.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/recommendation.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/recommendation.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/recommendation_impact.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/recommendation_impact.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/recommendation_new_rule.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/recommendation_new_rule.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/recommendation_workflow.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/recommendation_workflow.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/usbDevice.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/usbDevice.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/models/usbDeviceApproval.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/models/usbDeviceApproval.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/recommendation.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/recommendation.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/endpoint_standard/usb_device_control.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/endpoint_standard/usb_device_control.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/auth_events.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/auth_events.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/auth_events.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/auth_events.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/auth_events_facet.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/auth_events_facet.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/binary.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/binary.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/feed.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/feed.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/iocs.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/iocs.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/report.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/report.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/models/watchlist.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/models/watchlist.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/threat_intelligence.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/threat_intelligence.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/enterprise_edr/ubs.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/enterprise_edr/ubs.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/errors.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/helpers.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/live_response_api.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/live_response_api.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/__init__.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/alerts.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/alerts.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,35 @@
 # *
 # * DISCLAIMER. THIS PROGRAM IS PROVIDED TO YOU "AS IS" WITHOUT
 # * WARRANTIES OR CONDITIONS OF ANY KIND, WHETHER ORAL OR WRITTEN,
 # * EXPRESS OR IMPLIED. THE AUTHOR SPECIFICALLY DISCLAIMS ANY IMPLIED
 # * WARRANTIES OR CONDITIONS OF MERCHANTABILITY, SATISFACTORY QUALITY,
 # * NON-INFRINGEMENT AND FITNESS FOR A PARTICULAR PURPOSE.
 
-"""Model and Query Classes for Platform Alerts and Workflows"""
+"""
+The model and query classes for supporting alerts and alert workflows.
+
+*Alerts* indicate suspicious behavior and known threats in the monitored environment. They should be regularly
+reviewed to determine whether action must be taken or policies should be modified.  The Carbon Black Cloud Python
+SDK may be used to retrieve alerts, as well as manage the workflow by modifying alert status or closing alerts.
+
+The Carbon Black Cloud Python SDK currently implements the Alerts v7 API, as documented on
+`the Developer Network <https://developer.carbonblack.com/reference/carbon-black-cloud/platform/latest/alerts-api/>`_.
+It works with any Carbon Black Cloud product, although certain alert types are only generated by specific products.
+
+Typical usage example::
+
+    # assume "cb" is an instance of CBCloudAPI
+    query = cb.select(Alert).add_criteria("device_os", ["WINDOWS"]).set_minimum_severity(3)
+    query.set_time_range(range="-1d").set_rows(1000).add_exclusions("type", ["WATCHLIST"])
+    for alert in query:
+        print(f"Alert ID {alert.id} with severity {alert.severity} at {alert.detection_timestamp}")
+
+"""
+
 import time
 import datetime
 
 from cbc_sdk.errors import ApiError, ObjectNotFoundError, NonQueryableModel, FunctionalityDecommissioned
 from cbc_sdk.platform import PlatformModel
 from cbc_sdk.base import (BaseQuery,
                           QueryBuilder,
@@ -36,15 +56,24 @@
 """Alert Models"""
 
 MAX_RESULTS_LIMIT = 10000
 REQUEST_IGNORED_KEYS = ["_doc_class", "_cb", "_count_valid", "_total_results", "_query_builder", "_sortcriteria"]
 
 
 class Alert(PlatformModel):
-    """Represents a basic alert."""
+    """
+    Represents a basic alert within the Carbon Black Cloud.
+
+    ``Alert`` objects are typically located through a search (using ``AlertSearchQuery``) before they can be
+    operated on.
+
+    The complete list of alert fields is too large to be reproduced here; please see the list of available fields
+    for each alert type on `the Developer Network
+    <https://developer.carbonblack.com/reference/carbon-black-cloud/platform/latest/alert-search-fields>`_.
+    """
     REMAPPED_ALERTS_V6_TO_V7 = {
         "alert_classification.user_feedback": "determination_value",
         "cluster_name": "k8s_cluster",
         "create_time": "backend_timestamp",
         "created_by_event_id": "primary_event_id",
         "first_event_time": "first_event_timestamp",
         "last_event_time": "last_event_timestamp",
@@ -173,15 +202,14 @@
         "closure_reason": "remediation"
     }
 
     urlobject = "/api/alerts/v7/orgs/{0}/alerts"
     urlobject_single = "/api/alerts/v7/orgs/{0}/alerts/{1}"
     threat_urlobject_single = "/api/alerts/v7/orgs/{0}/threats/{1}"
     primary_key = "id"
-    swagger_meta_file = "platform/models/alert.yaml"
 
     def __init__(self, cb, model_unique_id, initial_data=None):
         """
         Initialize the Alert object.
 
         Args:
             cb (BaseAPI): Reference to API object used to communicate with the server.
@@ -192,141 +220,153 @@
         if model_unique_id is not None and initial_data is None:
             self._refresh()
 
     def get_process(self, async_mode=False):
         """
         Gets the process corresponding with the alert.
 
+        Required Permissions:
+            org.search.events (CREATE. READ)
+
         Args:
-            async_mode: True to request process in an asynchronous manner.
+            async_mode: ``True`` to request process in an asynchronous manner.
 
         Returns:
             Process: The process corresponding to the alert.
+
+        Note:
+            - When using asynchronous mode, this method returns a Python ``Future``.
+              You can call ``result()`` on the ``Future`` object to wait for completion and get the results.
         """
         process_guid = self._info.get("process_guid")
         if not process_guid:
             raise ApiError(f"Trying to get process details on an invalid process_id {process_guid}")
         if async_mode:
             return self._cb._async_submit(self._get_process)
         return self._get_process()
 
     def _get_process(self, *args, **kwargs):
         """
-        Implementation of the get_process.
+        Implementation of the ``get_process`` call.
+
+        Required Permissions:
+            org.search.events (CREATE. READ)
 
         Returns:
-            Process: The process corresponding to the alert. May return None if no process is found.
+            Process: The process corresponding to the alert. May return ``None`` if no process is found.
         """
         process_guid = self._info.get("process_guid")
         try:
             process = AsyncProcessQuery(Process, self._cb).where(process_guid=process_guid).one()
         except ObjectNotFoundError:
             return None
         return process
 
     def get_observations(self, timeout=0):
-        """Requests observations that are associated with the Alert.
+        """
+        Requests observations that are associated with the ``Alert``.
 
-         Uses Observations bulk get details.
+        Uses ``Observation.bulk_get_details``.
 
-        Returns:
-            list: Observations associated with the alert
+        Required Permissions:
+            org.search.events (READ, CREATE)
 
-        Note:
-            - When using asynchronous mode, this method returns a python future.
-              You can call result() on the future object to wait for completion and get the results.
+        Returns:
+            list[Observation]: Observations associated with the ``Alert``.
         """
         alert_id = self.get("id")
         if not alert_id:
             raise ApiError("Trying to get observations on an invalid alert_id {}".format(alert_id))
 
         obs = Observation.bulk_get_details(self._cb, alert_id=alert_id, timeout=timeout)
         return obs
 
     def get_history(self, threat=False):
         """
-        Get the actions taken on an Alert such as Notes added and workflow state changes.
+        Get the actions taken on an ``Alert`` such as ``Note``s added and workflow state changes.
+
+        Required Permissions:
+            org.alerts (READ)
 
         Args:
-            threat (bool): Whether to return the Alert or Threat history
+            threat (bool): If ``True``, the threat history is returned; if ``False``, the alert history is returned.
 
         Returns:
-            list: The dicts of each determination, note or workflow change
-
+            list: The ``dict``s of each determination, note or workflow change.
         """
         if threat:
             url = Alert.threat_urlobject_single.format(self._cb.credentials.org_key, self.threat_id)
         else:
             url = Alert.urlobject_single.format(self._cb.credentials.org_key, self._info[self.primary_key])
 
         url = f"{url}/history"
         resp = self._cb.get_object(url)
         return resp.get("history", [])
 
     def get_threat_tags(self):
         """
-        Gets the threat's tags
+        Gets the threat's tags.
 
         Required Permissions:
             org.alerts.tags (READ)
 
         Returns:
-            (list[str]): The list of current tags
+            list[str]: The list of current tags
         """
         url = Alert.threat_urlobject_single.format(self._cb.credentials.org_key, self.threat_id)
         url = f"{url}/tags"
         resp = self._cb.get_object(url)
         return resp.get("list", [])
 
     def add_threat_tags(self, tags):
         """
-        Adds tags to the threat
+        Adds tags to the threat.
 
         Required Permissions:
             org.alerts.tags (CREATE)
 
         Args:
-            tags (list[str]): List of tags to add to the threat
+            tags (list[str]): List of tags to add to the threat.
 
         Raises:
-            ApiError: If tags is not a list of strings
+            ApiError: If ``tags`` is not a list of strings.
 
         Returns:
-            (list[str]): The list of current tags
+            list[str]: The list of current tags.
         """
         if not isinstance(tags, list) or not isinstance(tags[0], str):
             raise ApiError("Tags must be a list of strings")
 
         url = Alert.threat_urlobject_single.format(self._cb.credentials.org_key, self.threat_id)
         url = f"{url}/tags"
         resp = self._cb.post_object(url, {"tags": tags})
         resp_json = resp.json()
         return resp_json.get("tags", [])
 
     def delete_threat_tag(self, tag):
         """
-        Delete a threat tag
+        Delete a threat tag.
 
         Required Permissions:
             org.alerts.tags (DELETE)
 
         Args:
-            tag (str): The tag to delete
+            tag (str): The tag to delete.
 
         Returns:
-            (list[str]): The list of current tags
+            (list[str]): The list of current tags.
         """
         url = Alert.threat_urlobject_single.format(self._cb.credentials.org_key, self.threat_id)
         url = f"{url}/tags/{tag}"
         resp = self._cb.delete_object(url)
         resp_json = resp.json()
         return resp_json.get("tags", [])
 
     class Note(PlatformModel):
-        """Represents a note within an alert."""
+        """Represents a note placed on an alert."""
         REMAPPED_NOTES_V6_TO_V7 = {
             "create_time": "create_timestamp",
         }
 
         REMAPPED_NOTES_V7_TO_V6 = {
             "create_timestamp": "create_time",
         }
@@ -335,35 +375,38 @@
         threat_urlobject = "/api/alerts/v7/orgs/{0}/threats/{1}/notes"
         primary_key = "id"
         swagger_meta_file = "platform/models/alert_note.yaml"
         _is_deleted = False
 
         def __init__(self, cb, alert, model_unique_id, threat_note=False, initial_data=None):
             """
-            Initialize the Note object.
+            Initialize the ``Note`` object.
 
             Args:
                 cb (BaseAPI): Reference to API object used to communicate with the server.
                 alert (Alert): The alert where the note is saved.
                 model_unique_id (str): ID of the note represented.
-                threat_note (bool): Whether the note is an Alert or Threat note
+                threat_note (bool): ``True`` if the note is a threat note, ``False`` if the note is an alert note.``
                 initial_data (dict): Initial data used to populate the note.
             """
             super(Alert.Note, self).__init__(cb, model_unique_id, initial_data)
             self._alert = alert
             self._threat_note = threat_note
             if model_unique_id is not None and initial_data is None:
                 self._refresh()
 
         def _refresh(self):
             """
             Rereads the alert data from the server.
 
+            Required Permissions:
+                org.alerts.notes (READ)
+
             Returns:
-                bool: True if refresh was successful, False if not.
+                bool: ``True`` if refresh was successful, ``False`` if not.
             """
             _exists_in_list = False
             if self._is_deleted:
                 raise ApiError("Cannot refresh a deleted Note")
 
             if self._threat_note:
                 if self._alert.threat_id:
@@ -396,15 +439,20 @@
 
             Raises:
                 ApiError: Always.
             """
             raise NonQueryableModel("Notes cannot be queried directly")
 
         def delete(self):
-            """Deletes a note from an alert."""
+            """
+            Deletes a note from an alert.
+
+            Required Permissions:
+                org.alerts.notes (DELETE)
+            """
             if self._threat_note:
                 url = self.threat_urlobject.format(self._cb.credentials.org_key, self._alert.threat_id)
             else:
                 url = self.urlobject.format(self._cb.credentials.org_key, self._alert.id)
 
             url = f"{url}/{self.id}"
             self._cb.delete_object(url)
@@ -449,36 +497,48 @@
             except AttributeError:
                 raise AttributeError("'{0}' object has no attribute '{1}'".format(self.__class__.__name__,
                                                                                   item))
                 # fall through to the rest of the logic...
 
     def notes_(self, threat_note=False):
         """
-        Retrieves all notes for an alert.
+        Retrieves all notes for this alert.
+
+        Required Permissions:
+            org.alerts.notes (READ)
 
         Args:
-            threat_note (bool): Whether to return the Alert notes or Threat notes
+            threat_note (bool): ``True`` to retrieve threat notes, ``False`` to retrieve alert notes.
+
+        Returns:
+            list[Note]: The list of notes for the alert.
         """
         if threat_note:
             url = Alert.Note.threat_urlobject.format(self._cb.credentials.org_key, self.threat_id)
         else:
             url = Alert.Note.urlobject.format(self._cb.credentials.org_key, self._info[self.primary_key])
 
         resp = self._cb.get_object(url)
         item_list = resp.get("results", [])
         return [Alert.Note(self._cb, self, item[Alert.Note.primary_key], threat_note, item)
                 for item in item_list]
 
     def create_note(self, note, threat_note=False):
         """
-        Creates a new note.
+        Creates a new note for this alert.
+
+        Required Permissions:
+            org.alerts.notes (CREATE)
 
         Args:
-            note (str): Note content to add
-            threat_note (bool): Whether to add the note to the Alert or Threat
+            note (str): Note content to add.
+            threat_note (bool): ``True`` to add this alert to the treat, ``False`` to add this note to the alert.
+
+        Returns:
+            Note: The newly-added note.
         """
         request = {"note": note}
         if threat_note:
             url = Alert.Note.threat_urlobject.format(self._cb.credentials.org_key, self.threat_id)
         else:
             url = Alert.Note.urlobject.format(self._cb.credentials.org_key, self._info[self.primary_key])
         resp = self._cb.post_object(url, request)
@@ -499,16 +559,19 @@
         """
         return AlertSearchQuery(cls, cb)
 
     def _refresh(self):
         """
         Rereads the alert data from the server.
 
+        Required Permissions:
+            org.alerts (READ)
+
         Returns:
-            bool: True if refresh was successful, False if not.
+            bool: ``True`` if refresh was successful, ``False`` if not.
         """
         url = self.urlobject_single.format(self._cb.credentials.org_key, self._model_unique_id)
         resp = self._cb.get_object(url)
         self._info = resp
         self._last_refresh_time = time.time()
         return True
 
@@ -523,90 +586,100 @@
         return self.workflow
 
     def deobfuscate_cmdline(self):
         """
         Deobfuscates the command line of the process pointed to by the alert and returns the deobfuscated result.
 
         Required Permissions:
-            script.deobfuscation(EXECUTE)
+            script.deobfuscation (EXECUTE)
 
         Returns:
-             dict: A dict containing information about the obfuscated command line, including the deobfuscated result.
+             dict: A ``dict`` containing information about the obfuscated command line, including the
+                deobfuscated result.
         """
         body = {"input": self.process_cmdline}
         result = self._cb.post_object(f"/tau/v2/orgs/{self._cb.credentials.org_key}/reveal", body)
         return result.json()
 
     def close(self, closure_reason=None, determination=None, note=None):
         """
         Closes this alert.
 
+        Note:
+            - This is an asynchronous call that returns a ``Job``. If you want to wait and block on the results
+              you can call ``await_completion()`` to get a ``Future`` then ``result()`` on the ``future`` object
+              to wait for completion and get the results.
+
+        Required Permissions:
+            org.alerts.close (EXECUTE), jobs.status (READ)
+
         Args:
             closure_reason (str): the closure reason for this alert, either "NO_REASON", "RESOLVED", \
             "RESOLVED_BENIGN_KNOWN_GOOD", "DUPLICATE_CLEANUP", "OTHER"
             determination (str): The determination status to set for the alert, either "TRUE_POSITIVE", \
             "FALSE_POSITIVE", or "NONE"
             note (str): The comment to set for the alert.
 
-        Note:
-            - This is an asynchronus call that returns a Job. If you want to wait and block on the results
-              you can call await_completion() to get a Futre then result() on the future object to wait for
-              completion and get the results.
+        Returns:
+            Job: The ``Job`` object for the alert workflow action.
 
         Example:
             >>> alert = cb.select(Alert, "708d7dbf-2020-42d4-9cbc-0cddd0ffa31a")
             >>> job = alert.close("RESOLVED", "FALSE_POSITIVE", "Normal behavior")
             >>> completed_job = job.await_completion().result()
             >>> alert.refresh()
-
-        Returns:
-            Job: The Job object for the alert workflow action.
         """
         job = self._cb.select(Alert).add_criteria("id", [self.get("id")]) \
-                                    ._update_status("CLOSED", closure_reason, note, determination)
+            ._update_status("CLOSED", closure_reason, note, determination)
 
         self._last_refresh_time = time.time()
         return job
 
     def update(self, status, closure_reason=None, determination=None, note=None):
         """
         Update the Alert with optional closure_reason, determination, note, or status.
 
+        Note:
+            - This is an asynchronous call that returns a ``Job``. If you want to wait and block on the results
+              you can call ``await_completion()`` to get a ``Future`` then ``result()`` on the ``future`` object
+              to wait for completion and get the results.
+
+        Required Permissions:
+            org.alerts.close (EXECUTE), jobs.status (READ)
+
         Args:
             status (str): The status to set for this alert, either "OPEN", "IN_PROGRESS", or "CLOSED".
-            closure_reason (str): the closure reason for this alert, either "NO_REASON", "RESOLVED", \
-            "RESOLVED_BENIGN_KNOWN_GOOD", "DUPLICATE_CLEANUP", "OTHER"
-            determination (str): The determination status to set for the alert, either "TRUE_POSITIVE", \
-            "FALSE_POSITIVE", or "NONE"
+            closure_reason (str): the closure reason for this alert, either "NO_REASON", "RESOLVED",
+                "RESOLVED_BENIGN_KNOWN_GOOD", "DUPLICATE_CLEANUP", "OTHER"
+            determination (str): The determination status to set for the alert, either "TRUE_POSITIVE",
+                "FALSE_POSITIVE", or "NONE"
             note (str): The comment to set for the alert.
 
-        Note:
-            - This is an asynchronus call that returns a Job. If you want to wait and block on the results
-              you can call await_completion() to get a Futre then result() on the future object to wait for
-              completion and get the results.
+        Returns:
+            Job: The ``Job`` object for the alert workflow action.
 
         Example:
             >>> alert = cb.select(Alert, "708d7dbf-2020-42d4-9cbc-0cddd0ffa31a")
             >>> job = alert.update("IN_PROGESS", "NO_REASON", "NONE", "Starting Investigation")
             >>> completed_job = job.await_completion().result()
             >>> alert.refresh()
-
-        Returns:
-            Job: The Job object for the alert workflow action.
         """
         job = self._cb.select(Alert).add_criteria("id", [self.get("id")]) \
-                                    ._update_status(status, closure_reason, note, determination)
+            ._update_status(status, closure_reason, note, determination)
 
         self._last_refresh_time = time.time()
         return job
 
     def _update_threat_workflow_status(self, state, remediation, comment):
         """
         Updates the workflow status of all future alerts with the same threat ID.
 
+        Required Permissions:
+            org.alerts.dismiss (EXECUTE)
+
         Args:
             state (str): The state to set for this alert, either "OPEN" or "DISMISSED".
             remediation (str): The remediation status to set for the alert.
             comment (str): The comment to set for the alert.
         """
         request = {"state": state}
         if remediation:
@@ -617,28 +690,34 @@
         resp = self._cb.post_object(url, request)
         return resp.json()
 
     def dismiss_threat(self, remediation=None, comment=None):
         """
         Dismisses all future alerts assigned to the threat_id.
 
+        Required Permissions:
+            org.alerts.dismiss (EXECUTE)
+
         Args:
             remediation (str): The remediation status to set for the alert.
             comment (str): The comment to set for the alert.
 
         Note:
             - If you want to dismiss all past and current open alerts associated to the threat use the following:
                 >>> cb.select(Alert).add_criteria("threat_id", [alert.threat_id]).close(...)
         """
         return self._update_threat_workflow_status("DISMISSED", remediation, comment)
 
     def update_threat(self, remediation=None, comment=None):
         """
         Updates all future alerts assigned to the threat_id to the OPEN state.
 
+        Required Permissions:
+            org.alerts.dismiss (EXECUTE)
+
         Args:
             remediation (str): The remediation status to set for the alert.
             comment (str): The comment to set for the alert.
 
         Note:
             - If you want to update all past and current alerts associated to the threat use the following:
                 >>> cb.select(Alert).add_criteria("threat_id", [alert.threat_id]).update(...)
@@ -646,14 +725,17 @@
         return self._update_threat_workflow_status("OPEN", remediation, comment)
 
     @staticmethod
     def search_suggestions(cb, query):
         """
         Returns suggestions for keys and field values that can be used in a search.
 
+        Required Permissions:
+            org.alerts (READ)
+
         Args:
             cb (CBCloudAPI): A reference to the CBCloudAPI object.
             query (str): A search query to use.
 
         Returns:
             list: A list of search suggestions expressed as dict objects.
 
@@ -703,21 +785,22 @@
         """
         try:
             original_item = item
             if item in Alert.DEPRECATED_FIELDS_NOT_IN_V7:
                 raise FunctionalityDecommissioned(
                     "Attribute '{0}' does not exist in object '{1}' because it was deprecated in "
                     "Alerts v7. In SDK 1.5.0 the".format(item, self.__class__.__name__))
-            if item in Alert.DEPRECATED_FIELDS_NOT_IN_V7_CONTAINER_ONLY and self.type == "CONTAINER_RUNTIME":
+            if (item in Alert.DEPRECATED_FIELDS_NOT_IN_V7_CONTAINER_ONLY
+                    and self._info.get('type', None) == "CONTAINER_RUNTIME"):
                 raise FunctionalityDecommissioned(
                     "Attribute '{0}' does not exist in object '{1}' because it was deprecated in "
                     "Alerts v7. In SDK 1.5.0 the".format(item, self.__class__.__name__))
 
             item = Alert.REMAPPED_ALERTS_V6_TO_V7.get(item, item)
-            if self.get("type") == "CONTAINER_RUNTIME":
+            if self._info.get('type', None) == "CONTAINER_RUNTIME":
                 item = Alert.REMAPPED_CONTAINER_ALERTS_V6_TO_V7.get(original_item, item)
             return super(Alert, self).__getattr__(item)
         except AttributeError:
             raise AttributeError("'{0}' object has no attribute '{1}'".format(self.__class__.__name__,
                                                                               item))
             # fall through to the rest of the logic...
 
@@ -784,18 +867,23 @@
             raise FunctionalityDecommissioned(
                 "Attribute '{0}' does not exist in object '{1}' because it was deprecated in "
                 "Alerts v7. In SDK 1.5.0 the".format(item, self.__class__.__name__))
         return super(Alert, self).get(item, default_val)
 
 
 class WatchlistAlert(Alert):
-    """Represents watch list alerts."""
+    """
+    A specialization of the base ``Alert`` class that represents a watchlist alert.
+
+    The complete list of alert fields is too large to be reproduced here; please see the list of available fields
+    for each alert type on `the Developer Network
+    <https://developer.carbonblack.com/reference/carbon-black-cloud/platform/latest/alert-search-fields>`_.
+    """
     urlobject = "/api/alerts/v7/orgs/{0}/alerts"
     type = ["WATCHLIST"]
-    swagger_meta_file = "platform/models/alert_watchlist.yaml"
 
     @classmethod
     def _query_implementation(cls, cb, **kwargs):
         """
         Returns the appropriate query object for this alert type.
 
         Args:
@@ -815,25 +903,30 @@
             >>> watchlist_alert = cb.select(Alert, "f643d11f-59ab-478f-92c3-4198ca9b8230")
             >>> watchlist_objects = watchlist_alert.get_watchlist_objects()
 
         Returns:
             list[Watchlist]: A list of Watchlist objects.
         """
         watchlist_objects = []
-        for watchlist in self.get("watchlists"):
+        for watchlist in self._info.get("watchlists"):
             watchlist_id = watchlist.get("id")
             watchlist_objects.append(self._cb.select(Watchlist, watchlist_id))
         return watchlist_objects
 
 
 class CBAnalyticsAlert(Alert):
-    """Represents CB Analytics alerts."""
+    """
+    A specialization of the base ``Alert`` class that represents a CB Analytics alert.
+
+    The complete list of alert fields is too large to be reproduced here; please see the list of available fields
+    for each alert type on `the Developer Network
+    <https://developer.carbonblack.com/reference/carbon-black-cloud/platform/latest/alert-search-fields>`_.
+    """
     urlobject = "/api/alerts/v7/orgs/{0}/alerts"
     type = ["CB_ANALYTICS"]
-    swagger_meta_file = "platform/models/alert_cb_analytic.yaml"
 
     @classmethod
     def _query_implementation(cls, cb, **kwargs):
         """
         Returns the appropriate query object for this alert type.
 
         Args:
@@ -842,15 +935,16 @@
 
         Returns:
             AlertSearchQuery: The query object for this alert type.
         """
         return AlertSearchQuery(cls, cb).add_criteria("type", ["CB_ANALYTICS"])
 
     def get_events(self, timeout=0, async_mode=False):
-        """Removed in CBC SDK 1.5.0 because Enriched Events are deprecated.
+        """
+        Removed in CBC SDK 1.5.0 because Enriched Events are deprecated.
 
         Previously requested enriched events detailed results.  Update to use get_observations() instead.
         See `Developer Network Observations Migration
         <https://developer.carbonblack.com/reference/carbon-black-cloud/guides/api-migration/observations-migration>`_
         for more details.
 
         Args:
@@ -868,17 +962,22 @@
             FunctionalityDecommissioned: If the requested attribute is no longer available.
         """
         raise FunctionalityDecommissioned("get_events method does not exist in in SDK v1.5.0 "
                                           "because Enriched Events have been deprecated.  The")
 
 
 class DeviceControlAlert(Alert):
-    """Represents Device Control alerts."""
+    """
+    A specialization of the base ``Alert`` class that represents a Device Control alert.
+
+    The complete list of alert fields is too large to be reproduced here; please see the list of available fields
+    for each alert type on `the Developer Network
+    <https://developer.carbonblack.com/reference/carbon-black-cloud/platform/latest/alert-search-fields>`_.
+    """
     urlobject = "/api/alerts/v7/orgs/{0}/alerts"
-    swagger_meta_file = "platform/models/alert_device_control.yaml"
 
     @classmethod
     def _query_implementation(cls, cb, **kwargs):
         """
         Returns the appropriate query object for this alert type.
 
         Args:
@@ -888,17 +987,22 @@
         Returns:
             AlertSearchQuery: The query object for this alert type.
         """
         return AlertSearchQuery(cls, cb).add_criteria("type", ["DEVICE_CONTROL"])
 
 
 class ContainerRuntimeAlert(Alert):
-    """Represents Container Runtime alerts."""
+    """
+    A specialization of the base ``Alert`` class that represents a Container Runtime alert.
+
+    The complete list of alert fields is too large to be reproduced here; please see the list of available fields
+    for each alert type on `the Developer Network
+    <https://developer.carbonblack.com/reference/carbon-black-cloud/platform/latest/alert-search-fields>`_.
+    """
     urlobject = "/api/alerts/v7/orgs/{0}/alerts"
-    swagger_meta_file = "platform/models/alert_container_runtime.yaml"
     type = ["CONTAINER_RUNTIME"]
 
     @classmethod
     def _query_implementation(cls, cb, **kwargs):
         """
         Returns the appropriate query object for this alert type.
 
@@ -909,39 +1013,48 @@
         Returns:
             AlertSearchQuery: The query object for this alert type.
         """
         return AlertSearchQuery(cls, cb).add_criteria("type", ["CONTAINER_RUNTIME"])
 
 
 class HostBasedFirewallAlert(Alert):
-    """Represents Host Based Firewall alerts."""
+    """
+    A specialization of the base ``Alert`` class that represents a host-based firewall alert.
+
+    The complete list of alert fields is too large to be reproduced here; please see the list of available fields
+    for each alert type on `the Developer Network
+    <https://developer.carbonblack.com/reference/carbon-black-cloud/platform/latest/alert-search-fields>`_.
+    """
     urlobject = "/api/alerts/v7/orgs/{0}/alerts"
-    swagger_meta_file = "platform/models/alert_host_based_firewall.yaml"
     type = ["HOST_BASED_FIREWALL"]
 
     @classmethod
     def _query_implementation(cls, cb, **kwargs):
         """
         Returns the appropriate query object for this alert type.
 
         Args:
             cb (BaseAPI): Reference to API object used to communicate with the server.
-            cb (BaseAPI): Reference to API object used to communicate with the server.
             **kwargs (dict): Not used, retained for compatibility.
 
         Returns:
             AlertSearchQuery: The query object for this alert type.
         """
         return AlertSearchQuery(cls, cb).add_criteria("type", ["HOST_BASED_FIREWALL"])
 
 
 class IntrusionDetectionSystemAlert(Alert):
-    """Represents Intrusion Detection System alerts."""
+    """
+    A specialization of the base ``Alert`` class that represents an intrusion detection system alert.
+
+    The complete list of alert fields is too large to be reproduced here; please see the list of available fields
+    for each alert type on `the Developer Network
+    <https://developer.carbonblack.com/reference/carbon-black-cloud/platform/latest/alert-search-fields>`_.
+    """
     urlobject = "/api/alerts/v7/orgs/{0}/alerts"
-    swagger_meta_file = "platform/models/alert_intrusion_detection_system.yaml"
     type = ["INTRUSION_DETECTION_SYSTEM"]
 
     @classmethod
     def _query_implementation(cls, cb, **kwargs):
         """
         Returns the appropriate query object for this alert type.
 
@@ -952,30 +1065,34 @@
         Returns:
             AlertSearchQuery: The query object for this alert type.
         """
         return AlertSearchQuery(cls, cb).add_criteria("type", ["INTRUSION_DETECTION_SYSTEM"])
 
     def get_network_threat_metadata(self):
         """
-        The NetworkThreatMetadata associated with this IDS alert if it exists.
+        Retrun the ``NetworkThreatMetadata`` associated with this IDS alert if it exists.
 
         Example:
             >>> alert_threat_metadata = ids_alert.get_network_threat_metadata()
 
         Returns:
             NetworkThreatMetadata: The NetworkThreatMetadata associated with this IDS alert.
         """
         tms_rule_id = self.get("tms_rule_id")
         if tms_rule_id:
             return self._cb.select(NetworkThreatMetadata, tms_rule_id)
         return None
 
 
 class GroupedAlert(PlatformModel):
-    """Represents Grouped alerts."""
+    """
+    Represents alerts that have been grouped together based on a common characteristic.
+
+    This allows viewing of similar alerts across multiple endpoints.
+    """
     urlobject = "/api/alerts/v7/orgs/{0}/grouped_alerts"
     swagger_meta_file = "platform/models/grouped_alert.yaml"
 
     def __init__(self, cb, model_unique_id, initial_data=None):
         """
         Initialize the Grouped Alert object.
 
@@ -1058,21 +1175,26 @@
 
 
 """Alert Queries"""
 
 
 class AlertSearchQuery(BaseQuery, QueryBuilderSupportMixin, IterableQueryMixin, LegacyAlertSearchQueryCriterionMixin,
                        CriteriaBuilderSupportMixin, ExclusionBuilderSupportMixin):
-    """Represents a query that is used to locate Alert objects."""
+    """
+    Query object that is used to locate ``Alert`` objects.
+
+    The ``AlertSearchQuery`` is constructed via SDK functions like the ``select()`` method on ``CBCloudAPI``.
+    The user would then add a query and/or criteria to it before iterating over the results.
+    """
     DEPRECATED_FACET_FIELDS = ["ALERT_TYPE", "CATEGORY", "REPUTATION", "WORKFLOW", "TAG", "POLICY_ID",
                                "POLICY_NAME", "APPLICATION_HASH", "APPLICATION_NAME", "STATUS", "POLICY_APPLIED_STATE"]
 
     def __init__(self, doc_class, cb):
         """
-        Initialize the AlertSearchQuery.
+        Initialize the ``AlertSearchQuery``.
 
         Args:
             doc_class (class): The model class that will be returned by this query.
             cb (BaseAPI): Reference to API object used to communicate with the server.
         """
         self._doc_class = doc_class
         self._cb = cb
@@ -1246,17 +1368,17 @@
 
     def _create_valid_time_filter(self, kwargs):
         """
         Verifies that an alert criteria key has the timerange functionality
 
         Args:
             kwargs (dict): Used to specify start= for start time, end= for end time, and range= for range. Values are
-            either timestamp ISO 8601 strings or datetime objects for start and end time. For range the time range to
-            execute the result search, ending on the current time. Should be in the form "-2w",
-            where y=year, w=week, d=day, h=hour, m=minute, s=second.
+                either timestamp ISO 8601 strings or datetime objects for start and end time. For range the time
+                range to execute the result search, ending on the current time. Should be in the form "-2w",
+                where y=year, w=week, d=day, h=hour, m=minute, s=second.
 
         Returns:
             filter object to be applied to the global time range or a specific field
         """
         time_filter = {}
         if kwargs.get("start", None) and kwargs.get("end", None):
             if kwargs.get("range", None):
@@ -1372,14 +1494,17 @@
         url = self._doc_class.urlobject.format(self._cb.credentials.org_key) + tail_end
         return url
 
     def _count(self):
         """
         Returns the number of results from the run of this query.
 
+        Required Permissions:
+            org.alerts (READ)
+
         Returns:
             int: The number of results from the run of this query.
         """
         if self._count_valid:
             return self._total_results
 
         url = self._build_url("/_search")
@@ -1388,29 +1513,32 @@
         result = resp.json()
 
         self._total_results = result["num_found"]
         self._count_valid = True
 
         return self._total_results
 
-    def _perform_query(self, from_row=1, max_rows=-1):
+    def _perform_query(self, from_row=0, max_rows=-1):
         """
         Performs the query and returns the results of the query in an iterable fashion.
 
         Alerts v6 API uses base 1 instead of 0.
 
+        Required Permissions:
+            org.alerts (READ)
+
         Args:
-            from_row (int): The row to start the query at (default 1).
+            from_row (int): The row to start the query at (default 0).
             max_rows (int): The maximum number of rows to be returned (default -1, meaning "all").
 
         Returns:
             Iterable: The iterated query.
         """
         url = self._build_url("/_search")
-        current = from_row
+        current = from_row + 1
         numrows = 0
         still_querying = True
         while still_querying:
             request = self._build_request(current, max_rows)
             resp = self._cb.post_object(url, body=request)
             result = resp.json()
 
@@ -1445,23 +1573,26 @@
                 current += 1
                 numrows += 1
 
                 if max_rows > 0 and numrows == max_rows:
                     still_querying = False
                     break
 
-            from_row = current
+            from_row = current - 1
             if current >= self._total_results:
                 still_querying = False
                 break
 
     def facets(self, fieldlist, max_rows=0):
         """
         Return information about the facets for this alert by search, using the defined criteria.
 
+        Required Permissions:
+            org.alerts (READ)
+
         Args:
             fieldlist (list): List of facet field names.
             max_rows (int): The maximum number of rows to return. 0 means return all rows.
 
         Returns:
             list: A list of facet information specified as dicts.
             error: invalid enum
@@ -1486,23 +1617,26 @@
         result = resp.json()
         return result.get("results", [])
 
     def _update_status(self, status, closure_reason, note, determination):
         """
         Updates the status of all alerts matching the given query.
 
+        Required Permissions:
+            org.alerts.close (EXECUTE), jobs.status (READ)
+
         Args:
             status (str): The status to set for this alert, either "OPEN", "IN_PROGRESS", or "CLOSED".
             closure_reason (str): the closure reason for this alert, either "TRUE_POSITIVE", "FALSE_POSITIVE", or "NONE"
             note (str): The comment to set for the alert.
-            determination (str): The determination status to set for the alert, either "NO_REASON", "RESOLVED", \
-            "RESOLVED_BENIGN_KNOWN_GOOD", "DUPLICATE_CLEANUP", "OTHER"
+            determination (str): The determination status to set for the alert, either "NO_REASON", "RESOLVED",
+                "RESOLVED_BENIGN_KNOWN_GOOD", "DUPLICATE_CLEANUP", "OTHER"
 
         Returns:
-            Job: The Job object for the bulk workflow action.
+            Job: The ``Job`` object for the bulk workflow action.
         """
         request = self._build_request(0, -1)
         del request["rows"]
 
         if status:
             request["status"] = status
         if closure_reason is not None:
@@ -1515,55 +1649,61 @@
         output = resp.json()
         return Job(self._cb, output["request_id"])
 
     def update(self, status, closure_reason=None, determination=None, note=None):
         """
         Update all alerts matching the given query.
 
+        Required Permissions:
+            org.alerts.close (EXECUTE), jobs.status (READ)
+
         Args:
             status (str): The status to set for this alert, either "OPEN", "IN_PROGRESS", or "CLOSED".
             closure_reason (str): the closure reason for this alert, either "NO_REASON", "RESOLVED", \
             "RESOLVED_BENIGN_KNOWN_GOOD", "DUPLICATE_CLEANUP", "OTHER"
             determination (str): The determination status to set for the alert, either "TRUE_POSITIVE", \
             "FALSE_POSITIVE", or "NONE"
             note (str): The comment to set for the alert.
 
         Returns:
-            Job: The Job object for the bulk workflow action.
+            Job: The ``Job`` object for the bulk workflow action.
 
         Note:
-            - This is an asynchronus call that returns a Job. If you want to wait and block on the results
-              you can call await_completion() to get a Futre then result() on the future object to wait for
-              completion and get the results.
+            - This is an asynchronous call that returns a ``Job``. If you want to wait and block on the results
+              you can call ``await_completion()`` to get a ``Future`` then ``result()`` on the ``Future`` object
+              to wait for completion and get the results.
 
         Example:
             >>> alert_query = cb.select(Alert).add_criteria("threat_id", ["19261158DBBF00775959F8AA7F7551A1"])
             >>> job = alert_query.update("IN_PROGESS", "NO_REASON", "NONE", "Starting Investigation")
             >>> completed_job = job.await_completion().result()
         """
         return self._update_status(status, closure_reason, note, determination)
 
     def close(self, closure_reason=None, determination=None, note=None, ):
         """
         Close all alerts matching the given query. The alerts will be left in a CLOSED state after this request.
 
+        Required Permissions:
+            org.alerts.close (EXECUTE), jobs.status (READ)
+
         Args:
             closure_reason (str): the closure reason for this alert, either "NO_REASON", "RESOLVED", \
             "RESOLVED_BENIGN_KNOWN_GOOD", "DUPLICATE_CLEANUP", "OTHER"
             determination (str): The determination status to set for the alert, either "TRUE_POSITIVE", \
             "FALSE_POSITIVE", or "NONE"
             note (str): The comment to set for the alert.
 
         Returns:
-            Job: The Job object for the bulk workflow action.
+            Job: The ``Job`` object for the bulk workflow action.
 
         Note:
-            - This is an asynchronus call that returns a Job. If you want to wait and block on the results
-              you can call await_completion() to get a Futre then result() on the future object to wait for
-              completion and get the results.
+            - This is an asynchronous call that returns a ``Job``. If you want to wait and block on the results
+              you can call ``await_completion()`` to get a ``Future`` then ``result()`` on the ``Future`` object
+              to wait for completion and get the results.
 
         Example:
             >>> alert_query = cb.select(Alert).add_criteria("threat_id", ["19261158DBBF00775959F8AA7F7551A1"])
             >>> job = alert_query.close("RESOLVED", "FALSE_POSITIVE", "Normal behavior")
             >>> completed_job = job.await_completion().result()
         """
         return self._update_status("CLOSED", closure_reason, note, determination)
@@ -1631,36 +1771,42 @@
             self._criteria["remote_is_private"] = is_private
         else:
             self._exclusions["remote_is_private"] = is_private
         return self
 
     def set_group_by(self, field):
         """
-        Converts the AlertSearchQuery to a GroupAlertSearchQuery grouped by the argument
+        Converts the ``AlertSearchQuery`` to a ``GroupAlertSearchQuery`` grouped by the argument.
 
         Args:
-            field (string): The field to group by, defaults to "threat_id"
+            field (string): The field to group by, defaults to "threat_id."
 
         Returns:
-            AlertSearchQuery
+            GroupedAlertSearchQuery: New query instance.
 
         Note:
             Does not preserve sort criterion
         """
         grouped_alert_search_query = self._cb.select(GroupedAlert)
         for key, value in vars(grouped_alert_search_query).items():
             if hasattr(self, key) and key not in REQUEST_IGNORED_KEYS:
                 setattr(grouped_alert_search_query, key, self.__getattribute__(key))
         grouped_alert_search_query.set_group_by(field)
 
         return grouped_alert_search_query
 
 
 class GroupedAlertSearchQuery(AlertSearchQuery):
-    """Represents a query that is used to group Alert objects by a given field."""
+    """
+    Query object that is used to locate ``Alert`` objects.
+
+    This query is constructed by using the ``select()`` method on ``CBCloudAPI`` to create an ``AlertSearchQuery,``
+    then using that query's ``set_group_by()`` method to specify grouping.
+    """
+
     def __init__(self, *args, **kwargs):
         """Initialize the GroupAlertSearchQuery."""
         super().__init__(*args, **kwargs)
         self._group_by = "THREAT_ID"
 
     def set_group_by(self, field):
         """
@@ -1687,40 +1833,45 @@
         request = super(GroupedAlertSearchQuery, self)._build_request(from_row, max_rows, add_sort=True)
         request["group_by"] = {"field": self._group_by}
 
         return request
 
     def get_alert_search_query(self):
         """
-        Converts the GroupedAlertSearchQuery into a nongrouped AlertSearchQuery
+        Converts the ``GroupedAlertSearchQuery`` into a nongrouped ``AlertSearchQuery``.
 
-        Returns: AlertSearchQuery
+        Returns:
+            AlertSearchQuery: New query instance.
 
-        Note: Does not preserve sort criterion
+        Note:
+            Does not preserve sort criterion.
         """
         alert_search_query = self._cb.select(Alert)
         for key, value in vars(alert_search_query).items():
             if hasattr(self, key) and key not in REQUEST_IGNORED_KEYS:
                 setattr(alert_search_query, key, self.__getattribute__(key))
 
         return alert_search_query
 
-    def _perform_query(self, from_row=1, max_rows=-1):
+    def _perform_query(self, from_row=0, max_rows=-1):
         """
         Performs the query and returns the results of the query in an iterable fashion.
 
+        Required Permissions:
+            org.alerts (READ)
+
         Args:
-            from_row (int): The row to start the query at (default 1).
+            from_row (int): The row to start the query at (default 0).
             max_rows (int): The maximum number of rows to be returned (default -1, meaning "all").
 
         Returns:
             Iterable: The iterated query.
         """
         url = self._build_url("/_search")
-        current = from_row
+        current = from_row + 1
         numrows = 0
         still_querying = True
         while still_querying:
             request = self._build_request(current, max_rows)
             resp = self._cb.post_object(url, body=request)
             result = resp.json()
 
@@ -1740,15 +1891,15 @@
                 current += 1
                 numrows += 1
 
                 if max_rows > 0 and numrows == max_rows:
                     still_querying = False
                     break
 
-            from_row = current
+            from_row = current - 1
             if current >= self._total_results:
                 still_querying = False
                 break
 
     def close(self, closure_reason=None, determination=None, note=None):
         """
         Closing all alerts matching a grouped alert query is not implemented.
@@ -1778,23 +1929,25 @@
         """
         raise NotImplementedError("this method is not implemented")
 
     def facets(self, fieldlist, max_rows=0, filter_values=False):
         """
         Return information about the facets for this alert by search, using the defined criteria.
 
+        Required Permissions:
+            org.alerts (READ)
+
         Args:
             fieldlist (list): List of facet field names.
             max_rows (int): The maximum number of rows to return. 0 means return all rows.
             filter_values (boolean): A flag to indicate whether any filters on a term should be applied to facet
-            calculation. When false (default), a filter on the term is ignored while calculating facets
+                calculation. When ``False`` (default), a filter on the term is ignored while calculating facets.
 
         Returns:
-            list: A list of facet information specified as dicts.
-            error: invalid enum
+            list: A list of facet information specified as ``dict``s.
 
         Raises:
             FunctionalityDecommissioned: If the requested attribute is no longer available.
             ApiError: If the facet field is not valid
         """
         for field in fieldlist:
             if field in GroupedAlertSearchQuery.DEPRECATED_FACET_FIELDS:
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/asset_groups.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/asset_groups.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/base.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/base.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/devices.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -995,33 +995,30 @@
         result = resp.json()
 
         self._total_results = result["num_found"]
         self._count_valid = True
 
         return self._total_results
 
-    def _perform_query(self, from_row=1, max_rows=-1):
+    def _perform_query(self, from_row=0, max_rows=-1):
         """
         Performs the query and returns the results of the query in an iterable fashion.
 
-        Note:
-            Device v6 API uses base 1 instead of 0.
-
         Required Permissions:
             device(READ)
 
         Args:
-            from_row (int): The row to start the query at (default 1).
+            from_row (int): The row to start the query at (default 0).
             max_rows (int): The maximum number of rows to be returned (default -1, meaning "all").
 
         Yields:
             Device: The individual devices which match the query.
         """
         url = self._build_url("/_search")
-        current = from_row
+        current = from_row + 1
         numrows = 0
         still_querying = True
         while still_querying:
             request = self._build_request(current, max_rows)
             resp = self._cb.post_object(url, body=request)
             result = resp.json()
 
@@ -1034,15 +1031,15 @@
                 current += 1
                 numrows += 1
 
                 if max_rows > 0 and numrows == max_rows:
                     still_querying = False
                     break
 
-            from_row = current
+            from_row = current - 1
             if current >= self._total_results:
                 still_querying = False
                 break
 
     def _run_async_query(self, context):
         """
         Executed in the background to run an asynchronous query on devices.
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/events.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,15 +213,16 @@
             resp = self._cb.post_object(url, body=args)
             result = resp.json()
 
             self._total_results = result.get("num_available", 0)
             self._total_segments = result.get("total_segments", 0)
             self._processed_segments = result.get("processed_segments", 0)
             self._count_valid = True
-            if self._processed_segments != self._total_segments:
+            if self._processed_segments != self._total_segments \
+                    and len(result.get('results', [])) != self._total_results:
                 retry_counter = 0 if self._processed_segments > last_processed_segments else retry_counter + 1
                 last_processed_segments = max(last_processed_segments, self._processed_segments)
                 if retry_counter == MAX_EVENT_SEARCH_RETRIES:
                     raise TimeoutError(url, resp.status_code, "excessive number of retries in event query")
                 time.sleep(1 + retry_counter / 10)
                 continue  # loop until we get all segments back
 
@@ -276,16 +277,21 @@
         if self._query_builder._process_guid is not None:
             args["process_guid"] = self._query_builder._process_guid
         if 'process_guid:' in args.get('query', ""):
             q = args['query'].split('process_guid:', 1)[1].split(' ', 1)[0]
             args["process_guid"] = q
         return args
 
-    def _perform_query(self):
-        return self.results
+    def _perform_query(self, from_row=0, max_rows=-1):
+        if max_rows > 0:
+            return self.results[from_row:from_row + max_rows]
+        elif from_row > 0:
+            return self.results[from_row:]
+        else:
+            return self.results
 
     def _submit(self):
         args = self._get_query_parameters()
         # args["process_guid"] is used in the URL but not the args
         process_guid = args.pop("process_guid", None)
         # a GUID is required for this API call
         if process_guid is None:
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/grants.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/grants.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/jobs.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/jobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 """Model and Query Classes for Jobs API"""
 
 import io
 import logging
 import time
 from cbc_sdk.base import NewBaseModel, BaseQuery, IterableQueryMixin, AsyncQueryMixin
-from cbc_sdk.errors import ObjectNotFoundError, ServerError
+from cbc_sdk.errors import ObjectNotFoundError, ServerError, ApiError
+from cbc_sdk.utils import BackoffHandler
 
 
 log = logging.getLogger(__name__)
 
 
 class Job(NewBaseModel):
     """Represents a job currently executing in the background."""
@@ -56,114 +57,132 @@
 
         Returns:
             JobQuery: The query object for this object type.
         """
         return JobQuery(cls, cb)
 
     def _refresh(self):
-        """Reload this object from the server."""
+        """
+        Reload this object from the server.
+
+        Required Permissions:
+            jobs.status (READ)
+        """
         url = self.urlobject_single.format(self._cb.credentials.org_key, self._model_unique_id)
         resp = self._cb.get_object(url)
         self._info = resp
         self._full_init = True
         self._last_refresh_time = time.time()
         return True
 
     def get_progress(self):
         """
         Get and return the current progress information for the job.
 
         Required Permissions:
-            jobs.status(READ)
+            jobs.status (READ)
 
         Returns:
             int: Total number of items to be operated on by this job.
             int: Total number of items for which operation has been completed.
             str: Current status message for the job.
         """
         url = self.urlobject_single.format(self._cb.credentials.org_key, self._model_unique_id) + "/progress"
         resp = self._cb.get_object(url)
         self._info['progress'] = resp
         return resp['num_total'], resp['num_completed'], resp.get('message', None)
 
-    def _await_completion(self):
+    def _await_completion(self, timeout=0):
         """
         Waits for this job to complete by examining the progress data.
 
         Required Permissions:
-            jobs.status(READ)
+            jobs.status (READ)
+
+        Args:
+            timeout (int): The timeout for this wait in milliseconds. If this is 0, the default value will be used.
 
         Returns:
             Job: This object.
+
+        Raises:
+            TimeoutError: If the wait times out.
         """
-        progress_data = (1, 0, '')
-        do_sleep = False
-        errorcount = 0
-        while progress_data[1] < progress_data[0]:
-            if do_sleep:
-                time.sleep(0.5)
-            try:
-                progress_data = self.get_progress()
-            except (ServerError, ObjectNotFoundError):
-                errorcount += 1
-                if errorcount == 3:
-                    raise
-                progress_data = (1, 0, '')
-            do_sleep = True
+        backoff = BackoffHandler(self._cb, timeout=timeout)
+        with backoff as b:
+            errorcount = 0
+            status = ""
+            while status not in ("FAILED", "COMPLETED"):
+                b.pause()
+                try:
+                    self._refresh()
+                    if self.status != status:
+                        status = self.status
+                        b.reset()
+                except (ServerError, ObjectNotFoundError):
+                    errorcount += 1
+                    if errorcount == 3:
+                        raise
+                    status = ""
+            if status == "FAILED":
+                raise ApiError(f"Job {self.id} reports failure")
         return self
 
-    def await_completion(self):
+    def await_completion(self, timeout=0):
         """
-        Create a Python Future to check for job completion and return results when available.
+        Create a Python ``Future`` to check for job completion and return results when available.
 
-        Returns a Future object which can be used to await results that are ready to fetch. This function call
+        Returns a ``Future`` object which can be used to await results that are ready to fetch. This function call
         does not block.
 
         Required Permissions:
-            jobs.status(READ)
+            jobs.status (READ)
+
+        Args:
+            timeout (int): The timeout for this wait in milliseconds. If this is 0, the default value will be used.
 
         Returns:
-            Future: A future which can be used to wait for this job's completion. When complete, the result of the
-                    Future will be this object.
+            Future: A ``Future`` which can be used to wait for this job's completion. When complete, the result of the
+                    ``Future`` will be this object.
         """
-        return self._cb._async_submit(lambda arg, kwarg: arg[0]._await_completion(), self)
+        return self._cb._async_submit(lambda arg, kwarg: arg[0]._await_completion(timeout), self)
 
     def get_output_as_stream(self, output):
         """
         Export the results from the job, writing the results to the given stream.
 
         Required Permissions:
-            jobs.status(READ)
+            jobs.status (READ)
 
         Args:
             output (RawIOBase): Stream to write the CSV data from the request to.
         """
         url = self.urlobject_single.format(self._cb.credentials.org_key, self._model_unique_id) + '/download'
         self._cb.api_request_stream('GET', url, output)
 
     def get_output_as_string(self):
         """
         Export the results from the job, returning the results as a string.
 
         Required Permissions:
-            jobs.status(READ)
+            jobs.status (READ)
 
         Returns:
             str: The results from the job.
         """
         with io.BytesIO() as buffer:
             self.get_output_as_stream(buffer)
             return str(buffer.getvalue(), 'utf-8')
 
     def get_output_as_file(self, filename):
         """
         Export the results from the job, writing the results to the given file.
 
         Required Permissions:
-            jobs.status(READ)
+            jobs.status (READ)
 
         Args:
             filename (str): Name of the file to write the results to.
         """
         with io.open(filename, 'wb') as file:
             self.get_output_as_stream(file)
 
@@ -171,15 +190,15 @@
         """
         Export the results from the job, returning the data as iterated lines of text.
 
         This is only intended for output that can reasonably be represented as lines of text, such as plain text or
         CSV.  If a job outputs structured text like JSON or XML, this method should not be used.
 
         Required Permissions:
-            jobs.status(READ)
+            jobs.status (READ)
 
         Returns:
             iterable: An iterable that can be used to get each line of text in turn as a string.
         """
         url = self.urlobject_single.format(self._cb.credentials.org_key, self._model_unique_id) + '/download'
         yield from self._cb.api_request_iterate('GET', url)
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/legacy_alerts.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/legacy_alerts.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/alert_container_runtime.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/device.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,247 +1,340 @@
 type: object
 properties:
-  alert_notes_present:
+  activation_code:
+    type: string
+    description: Device activation code
+  activation_code_expiry_time:
+    type: string
+    description: When the expiration code expires and cannot be used to register a device
+  ad_group_id:
+    type: integer
+    format: int64
+    description: Device's AD group
+  asset_group:
+    type: array
+    description: The asset groups that this device is a member of.
+    items:
+      type: object
+      properties:
+        id:
+          type: string
+          description: The ID of the asset group the device belongs to.
+        name:
+          type: string
+          description: The name of the asset group the device belongs to.
+        membership_type:
+          type: string
+          description: The type of membership this device has in the asset group.
+          enum:
+            - DYNAMIC
+            - MANUAL
+  av_ave_version:
+    type: string
+    description: AVE version (part of AV Version)
+  av_engine:
+    type: string
+    example: '4.3.0.203-ave.8.3.42.106:avpack.8.4.2.36:vdf.8.12.142.100'
+    description: Current AV version
+  av_last_scan_time:
+    type: string
+    description: Last AV scan time
+  av_master:
     type: boolean
-    description: True if notes are present on the alert ID. False if notes are not present.
-  alert_url:
+    description: Whether the device is an AV Master (?)
+  av_pack_version:
     type: string
-    description: Link to the alerts page for this alert. Does not vary by alert type
-  backend_timestamp:
+    description: Pack version (part of AV Version)
+  av_product_version:
     type: string
-    format: date-time
-    description: Timestamp when the Carbon Black Cloud processed and enabled the alert for searching. Corresponds to the Created column on the Alerts page.
-  backend_update_timestamp:
-    type: string
-    format: date-time
-    description: Timestamp when the Carbon Black Cloud initiated and processed an update to an alert. Corresponds to the Updated column on the Alerts page.   Note that changes made by users do not change this date; those changes are reflected on `user_update_timestamp`
-  connection_type:
-    type: string
-    enum:
-    - INTERNAL_INBOUND
-    - INTERNAL_OUTBOUND
-    - INGRESS
-    - EGRESS
-    description: Connection Type
-  detection_timestamp:
-    type: string
-    format: date-time
-    description: For sensor-sent alerts, this is the time of the event on the sensor. For alerts generated on the backend, this is the time the backend system triggered the alert.
-  determination:
-    description: User-updatable determination of the alert
-    type: object
-    properties:
-      change_timestamp:
-        type: string
-        format: date-time
-        description:  When the determination was updated.
-      changed_by:
-        type: string
-        description: User the determination was changed by.
-      changed_by_type:
-        type: string
-        description:
-        enum:
-        - SYSTEM
-        - USER
-        - API
-        - AUTOMATION
-      value:
-        type: string
-        description: Determination of the alert set by a user
-        enum:
-        - NONE
-        - TRUE_POSITIVE
-        - FALSE_POSITIVE
-  egress_group_id:
+    description: AV Product version (part of AV Version)
+  av_status:
+    type: array
+    description: AV Statuses
+    items:
+      type: string
+      enum:
+        - AV_NOT_REGISTERED
+        - AV_REGISTERED
+        - AV_DEREGISTERED
+        - AV_ACTIVE
+        - AV_BYPASS
+        - NOT_INSTALLED
+        - INSTALLED
+        - UNINSTALLED
+        - INSTALLED_SERVER
+        - UNINSTALLED_SERVER
+        - FULLY_ENABLED
+        - FULLY_DISABLED
+        - SIGNATURE_UPDATE_DISABLED
+        - ONACCESS_SCAN_DISABLED
+        - ONDEMOND_SCAN_DISABLED
+        - ONDEMAND_SCAN_DISABLED
+        - PRODUCT_UPDATE_DISABLED
+  av_update_servers:
+    type: array
+    description: Device's AV servers
+    items:
+      type: string
+  av_vdf_version:
     type: string
-    description: Unique identifier for the egress group
-  egress_group_name:
+    description: VDF version (part of AV Version)
+  current_sensor_policy_name:
     type: string
-    description: Name of the egress group
-  first_event_timestamp:
+    description: Current MSM policy name
+  deregistered_time:
     type: string
     format: date-time
-    description: Timestamp when the first event in the alert occurred
-  id:
-    type: string
-    description: Unique IDs of alerts
-  ip_reputation:
+    description: When the device was deregistered with the PSC backend
+  device_id:
     type: integer
     format: int64
-    description: Range of reputations to accept for the remote IP  0- unknown  1-20 high risk  21-40 suspicious  41-60 moderate  61-80 low risk  81-100 trustworthy There must be two values in this list. The first is the lower end of the range (inclusive) the second is the upper end of the range (inclusive)
-  is_updated:
-    type: boolean
-    description: Boolean that describes whether or not this is the original copy of the alert
-  k8s_cluster:
+    description: ID of the device
+  device_meta_data_item_list:
+    type: array
+    description: MSM Device metadata
+    items:
+      type: object
+      properties:
+        key_name:
+          type: string
+        key_value:
+          type: string
+        position:
+          type: integer
+          format: int32
+  device_owner_id:
+    type: integer
+    format: int64
+    description: ID of the user who owns the device
+  email:
     type: string
-    description: K8s Cluster name
-  k8s_kind:
+    description: Email of the user who owns the device
+  encoded_activation_code:
     type: string
-    description: K8s Workload kind
-  k8s_namespace:
+    description: Encoded device activation code
+  first_name:
     type: string
-    description: K8s namespace
-  k8s_pod_name:
+    description: First name of the user who owns the device
+  id:
+    type: integer
+    format: int64
+    description: ID of the device
+  last_contact_time:
     type: string
-    description: Name of the pod within a workload
-  k8s_policy:
+    format: date-time
+    description: Time the device last checked into the PSC backend
+  last_device_policy_changed_time:
     type: string
-    description: Name of the K8s policy
-  k8s_policy_id:
+    format: date-time
+    description: Last time the device's policy was changed
+  last_device_policy_requested_time:
+    type: string
+    format: date-time
+    description: Last time the device requested policy updates
+  last_external_ip_address:
     type: string
-    description: Unique identifier for the K8s policy
-  k8s_rule:
+    description: Device's external IP
+  last_internal_ip_address:
     type: string
-    description: Name of the K8s policy rule
-  k8s_rule_id:
+    description: Device's internal IP
+  last_location:
     type: string
-    description: Unique identifier for the K8s policy rule
-  k8s_workload_name:
+    description: Location of the device (on-/off-premises)
+    enum:
+      - UNKNOWN
+      - ONSITE
+      - OFFSITE
+  last_name:
     type: string
-    description:  K8s Workload Name
-  last_event_timestamp:
+    description: Last name of the user who owns the device
+  last_policy_updated_time:
     type: string
     format: date-time
-    description: Timestamp when the last event in the alert occurred
-  netconn_local_ip:
+    description: Last time the device was MSM processed
+  last_reported_time:
     type: string
-    description: IP address of the remote side of the network connection; stored as dotted decimal
-  netconn_local_ipv4:
+    format: date-time
+    description: Time when device last reported an event to PSC backend
+  last_reset_time:
     type: string
-    description: IPv4 address of the local side of the network connection; stored as a dotted decimal. Only one of ipv4 and ipv6 fields will be populated.
-  netconn_local_ipv6:
+    format: date-time
+    description: When the sensor was last reset
+  last_shutdown_time:
     type: string
-    description: IPv6 address of the local side of the network connection; stored as a string without octet-separating colon characters. Only one of ipv4 and ipv6 fields will be populated.
-  netconn_local_port:
-    type: integer
-    format: int64
-    description: TCP or UDP port used by the local side of the network connection
-  netconn_protocol:
+    format: date-time
+    description: When the device last shut down
+  linux_kernel_version:
     type: string
-    description: Network protocol of the network connection
-  netconn_remote_domain:
+    description: Linux kernel version
+  login_user_name:
     type: string
-    description: Domain name (FQDN) associated with the remote end of the network connection, if available
-  netconn_remote_ip:
+    description: Last acive logged in username
+  mac_address:
     type: string
-    description: IP address of the local side of the network connection; stored as dotted decimal
-  netconn_remote_ipv4:
+    description: Device's hardware MAC address
+  middle_name:
     type: string
-    description: IPv4 address of the remote side of the network connection; stored as dotted decimal. Only one of ipv4 and ipv6 fields will be populated.
-  netconn_remote_ipv6:
+    description: Middle name of the user who owns the device
+  name:
     type: string
-    description: IPv6 address of the remote side of the network connection; stored as a string without octet-separating colon characters. Only one of ipv4 and ipv6 fields will be populated.
-  netconn_remote_port:
+    description: Device Hostname
+  organization_id:
     type: integer
     format: int64
-    description: TCP or UDP port used by the remote side of the network connection; same as netconn_port and event_network_remote_port
-  org_key:
+    example: 1000
+    description: Org ID to which the device belongs
+  organization_name:
     type: string
-    description: Unique alphanumeric string that identifies your organization in the Carbon Black Cloud
-  policy_applied:
+    description: Name of the org that owns this device
+  os:
     type: string
+    example: WINDOWS
+    description: Device type
     enum:
-    - APPLIED
-    - NOT_APPLIED
-    description: Indicates whether or not a policy has been applied to any event associated with this alert
-  primary_event_id:
-    type: string
-    description: ID of the primary event in the alert
-  reason:
-    type: string
-    description: A spoken language written explanation of the what and why the alert occurred and any action taken, usually consisting of 1 to 3 sentences.
-  reason_code:
+      - WINDOWS
+      - ANDROID
+      - MAC
+      - IOS
+      - LINUX
+      - OTHER
+  os_version:
+    type: string
+    example: 'Windows 7 x86 SP: 1'
+    description: Version of the OS
+  passive_mode:
+    type: boolean
+    description: Whether the device is in passive mode (bypass?)
+  policy_id:
+    type: integer
+    format: int64
+    description: ID of the policy this device is using
+  policy_name:
     type: string
-    description: A unique short-hand code or GUID identifying the particular alert reason
-  remote_is_private:
+    description: Name of the policy this device is using
+  policy_override:
     type: boolean
-    description: Is the remote information private
-  remote_k8s_kind:
+    description: Manually assigned policy (overrides mass sensor management)
+  quarantined:
+    type: boolean
+    description: Whether the device is quarantined
+  registered_time:
     type: string
-    description: Kind of remote workload; set if the remote side is another workload in the same cluster
-  remote_k8s_namespace:
+    format: date-time
+    description: When the device was registered with the PSC backend
+  scan_last_action_time:
     type: string
-    description: Namespace within the remote workload’s cluster; set if the remote side is another workload in the same cluster
-  remote_k8s_pod_name:
+    format: date-time
+    description: Not used. Intended for when the background scan was last active
+  scan_last_complete_time:
     type: string
-    description: Remote workload pod name; set if the remote side is another workload in the same cluster
-  remote_k8s_workload_name:
+    format: date-time
+    description: Not Used. Intended for when the background scan was last completed
+  scan_status:
     type: string
-    description: Name of the remote workload; set if the remote side is another workload in the same cluster
-  run_state:
+    description: Not Used. Intended for Background scan status
+    enum:
+      - NEVER_RUN
+      - STOPPED
+      - IN_PROGRESS
+      - COMPLETED
+  sensor_out_of_date:
+    type: boolean
+    description: Whether the device is out of date
+  sensor_states:
+    type: array
+    description: Active sensor states
+    items:
+      type: string
+      enum:
+        - ACTIVE
+        - PANICS_DETECTED
+        - LOOP_DETECTED
+        - DB_CORRUPTION_DETECTED
+        - CSR_ACTION
+        - REPUX_ACTION
+        - DRIVER_INIT_ERROR
+        - REMGR_INIT_ERROR
+        - UNSUPPORTED_OS
+        - SENSOR_UPGRADE_IN_PROGRESS
+        - SENSOR_UNREGISTERED
+        - WATCHDOG
+        - SENSOR_RESET_IN_PROGRESS
+        - DRIVER_INIT_REBOOT_REQUIRED
+        - DRIVER_LOAD_NOT_GRANTED
+        - SENSOR_SHUTDOWN
+        - SENSOR_MAINTENANCE
+        - FULL_DISK_ACCESS_NOT_GRANTED
+        - DEBUG_MODE_ENABLED
+        - AUTO_UPDATE_DISABLED
+        - SELF_PROTECT_DISABLED
+        - VDI_MODE_ENABLED
+        - POC_MODE_ENABLED
+        - SECURITY_CENTER_OPTLN_DISABLED
+        - LIVE_RESPONSE_RUNNING
+        - LIVE_RESPONSE_NOT_RUNNING
+        - LIVE_RESPONSE_KILLED
+        - LIVE_RESPONSE_NOT_KILLED
+        - LIVE_RESPONSE_ENABLED
+        - LIVE_RESPONSE_DISABLED
+        - DRIVER_KERNEL
+        - DRIVER_USERSPACE
+        - DRIVER_LOAD_PENDING
+        - OS_VERSION_MISMATCH
+  sensor_version:
+    type: string
+    example: 3.4.0.0
+    description: Version of the PSC sensor
+  status:
     type: string
+    description: Device status
     enum:
-    - DID_NOT_RUN
-    - RAN
-    - UNKNOWN
-    description: Whether the threat in the alert actually ran
-  sensor_action:
+      - PENDING
+      - REGISTERED
+      - UNINSTALLED
+      - DEREGISTERED
+      - ACTIVE
+      - INACTIVE
+      - ERROR
+      - ALL
+      - BYPASS_ON
+      - BYPASS
+      - QUARANTINE
+      - SENSOR_OUTOFDATE
+      - DELETED
+      - LIVE
+  target_priority_type:
     type: string
+    example: MISSION_CRITICAL
+    description: Priority of the device
     enum:
-    - ALLOW
-    - ALLOW_AND_LOG
-    - DENY
-    - TERMINATE
-    description: Actions taken by the sensor, according to the rules of a policy
-  severity:
+      - LOW
+      - MEDIUM
+      - HIGH
+      - MISSION_CRITICAL
+  uninstall_code:
+    type: string
+    description: Code to enter to uninstall this device
+  vdi_base_device:
     type: integer
     format: int64
-    description:  integer representation of the impact of alert if true positive
-  tags:
-    type: array
-    description: Tags added to the threat ID of the alert
-    items:
-      type: string
-  threat_id:
-    type: string
-    description: ID assigned to a group of alerts with common criteria, based on alert type
-  threat_notes_present:
+    description: VDI Base device
+  virtual_machine:
     type: boolean
-    description: True if notes are present on the threat ID. False if notes are not present.
-  type:
+    description: Whether this device is a Virtual Machine (VMware AppDefense integration
+  virtualization_provider:
+    type: string
+    description: VM Virtualization Provider
+  windows_platform:
+    type: string
+    description: 'Type of windows platform (client/server, x86/x64)'
+    enum:
+      - CLIENT_X86
+      - CLIENT_X64
+      - SERVER_X86
+      - SERVER_X64
+  deployment_type:
     type: string
+    description: Classification determined by the device lifecycle management policy
     enum:
-    - CB_ANALYTICS
-    - WATCHLIST
-    - DEVICE_CONTROL
-    - CONTAINER_RUNTIME
-    - HOST_BASED_FIREWALL
-    - INTRUSION_DETECTION_SYSTEM
-    - NETWORK_TRAFFIC_ANALYSIS
-    description: Type of alert generated
-  user_update_timestamp:
-    type: string
-    format: date-time
-    description: Timestamp of the last property of an alert changed by a user, such as the alert workflow or determination
-  workflow:
-    type: object
-    description: Current workflow state of an alert. The workflow represents the flow from `OPEN` to `IN_PROGRESS` to `CLOSED` and captures who moved the alert into the current state. The history of these state transitions is available via the alert history route.
-    properties:
-      change_timestamp:
-        type: string
-        format: date-time
-        description: When the last status change occurred
-      workflow_changed_by:
-        type: string
-        description: Who (or what) made the last status change
-      workflow_changed_by_rule_id:
-        type: string
-        description:
-      workflow_changed_by_type:
-        type: string
-        enum:
-        - SYSTEM
-        - USER
-        - API
-        - AUTOMATION
-        description:
-      workflow_closure_reason:
-        type: string  `NO_REASON`, `RESOLVED`, `RESOLVED_BENIGN_KNOWN_GOOD`, `DUPLICATE_CLEANUP`, `OTHER`
-        description: A more detailed description of why the alert was resolved
-      workflow_status:
-        type: string
-        enum:
-        - OPEN
-        - IN_PROGRESS
-        - CLOSED
-        description: primary value used to determine if the alert is active or inactive and displayed in the UI by default
+      - ENDPOINT
+      - WORKLOAD
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/alert_device_control.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/policy.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,229 +1,179 @@
 type: object
 properties:
-  alert_notes_present:
-    type: boolean
-    description: True if notes are present on the alert ID. False if notes are not present.
-  alert_url:
-    type: string
-    description: Link to the alerts page for this alert. Does not vary by alert type
-  backend_timestamp:
-    type: string
-    format: date-time
-    description: Timestamp when the Carbon Black Cloud processed and enabled the alert for searching. Corresponds to the Created column on the Alerts page.
-  backend_update_timestamp:
-    type: string
-    format: date-time
-    description: Timestamp when the Carbon Black Cloud initiated and processed an update to an alert. Corresponds to the Updated column on the Alerts page.   Note that changes made by users do not change this date; those changes are reflected on `user_update_timestamp`
-  detection_timestamp:
-    type: string
-    format: date-time
-    description: For sensor-sent alerts, this is the time of the event on the sensor. For alerts generated on the backend, this is the time the backend system triggered the alert.
-  determination:
-    description: User-updatable determination of the alert
-    type: object
-    properties:
-      change_timestamp:
-        type: string
-        format: date-time
-        description:  When the determination was updated.
-      changed_by:
-        type: string
-        description: User the determination was changed by.
-      changed_by_type:
-        type: string
-        description:
-        enum:
-        - SYSTEM
-        - USER
-        - API
-        - AUTOMATION
-      value:
-        type: string
-        description: Determination of the alert set by a user
-        enum:
-        - NONE
-        - TRUE_POSITIVE
-        - FALSE_POSITIVE
-  device_external_ip:
-    type: string
-    description: IP address of the endpoint according to the Carbon Black Cloud; can differ from device_internal_ip due to network proxy or NAT; either IPv4 (dotted decimal notation) or IPv6 (proprietary format)
-  device_id:
+  id:
     type: integer
-    format: int64
-    description: ID of devices
-  device_internal_ip:
-    type: string
-    description: IP address of the endpoint reported by the sensor; either IPv4 (dotted decimal notation) or IPv6 (proprietary format)
-  device_location:
+    description: The policy identifier
+  name:
     type: string
-    enum:
-    - ONSITE
-    - OFFSITE
-    - UNKNOWN
-    description: Whether the device was on or off premises when the alert started, based on the current IP address and the device’s registered DNS domain suffix
-  device_name:
+    description: Defined name for the policy
+  org_key:
     type: string
-    description: Device name
-  device_os:
+    description: The organization key associated with the console instance
+  priority_level:
     type: string
+    description: The priority level designated for policy
     enum:
-    - WINDOWS
-    - ANDROID
-    - MAC
-    - LINUX
-    - OTHER
-    description: Device Operating Systems
-  device_os_version:
-    type: string
-    example: Windows 10 x64
-    description: The operating system and version of the endpoint. Requires Windows CBC sensor version 3.5 or later.
-  device_policy:
-    type: string
-    description: Device policy
-  device_policy_id:
+      - LOW
+      - MEDIUM
+      - HIGH
+      - MISSION_CRITICAL
+  position:
     type: integer
-    format: int64
-    description: Device policy id
-  device_target_value:
-    type: string
-    enum:
-    - LOW
-    - MEDIUM
-    - HIGH
-    - MISSION_CRITICAL
-    description:  Target value assigned to the device, set from the policy
-  device_uem_id:
-    type: string
-    description: Device correlation with WS1/EUC, required for our Workspace ONE Intelligence integration to function
-  device_username:
-    type: string
-    description: Logged on user during the alert. This is filled on a best-effort
-      approach. If the user is not available it may be populated with the device
-      owner (empty for Container Runtime alerts)
-  external_device_friendly_name:
-    type: string
-    description: Human-readable external device names
-  first_event_timestamp:
-    type: string
-    format: date-time
-    description: Timestamp when the first event in the alert occurred
-  id:
-    type: string
-    description: Unique IDs of alerts
-  is_updated:
+    description: Relative priority of this policy within the organization. Lower values indicate higher priority.
+  is_system:
     type: boolean
-    description: Boolean that describes whether or not this is the original copy of the alert
-  last_event_timestamp:
-    type: string
-    format: date-time
-    description: Timestamp when the last event in the alert occurred
-  org_key:
-    type: string
-    description: Unique alphanumeric string that identifies your organization in the Carbon Black Cloud
-  policy_applied:
+    description: Indicates that the policy was created by VMware
+  description:
     type: string
-    enum:
-    - APPLIED
-    - NOT_APPLIED
-    description: Indicates whether or not a policy has been applied to any event associated with this alert
-  primary_event_id:
-    type: string
-    description: ID of the primary event in the alert
-  product_id:
-    type: string
-    description: IDs of the product that identifies USB devices
-  product_name:
-    type: string
-    description: Names of the product that identifies USB devices
-  reason:
-    type: string
-    description: A spoken language written explanation of the what and why the alert occurred and any action taken, usually consisting of 1 to 3 sentences.
-  reason_code:
-    type: string
-    description: A unique short-hand code or GUID identifying the particular alert reason
-  run_state:
-    type: string
-    enum:
-    - DID_NOT_RUN
-    - RAN
-    - UNKNOWN
-    description: Whether the threat in the alert actually ran
-  sensor_action:
-    type: string
-    enum:
-    - ALLOW
-    - ALLOW_AND_LOG
-    - DENY
-    - TERMINATE
-    description: Actions taken by the sensor, according to the rules of a policy
-  serial_number:
-    type: string
-    description: Serial numbers of the specific devices
-  severity:
+    description: The description of the policy
+  auto_deregister_inactive_vdi_interval_ms:
+    type: integer
+    description: The time in milliseconds to wait after a VDI is inactive before setting the VDI to a DEREGISTERED state
+  auto_delete_known_bad_hashes_delay:
     type: integer
-    format: int64
-    description:  integer representation of the impact of alert if true positive
-  tags:
+    description: Enables the Carbon Black Cloud to automatically delete known malware after a specified time in milliseconds
+  av_settings:
+    type: object
+    description: Anti-Virus settings for endpoints and workloads assigned to the policy
+    properties:
+      avira_protection_cloud:
+        type: object
+        description: Third-party partner settings for unknown reputation binary analysis
+        properties:
+          enabled:
+            type: boolean
+            description: Whether unknown reputation binary analysis is enabled
+          max_exe_delay:
+            type: integer
+            description: Time before sending unknown binary for analysis in seconds
+            minimum: 2
+            maximum: 500
+          max_file_size:
+            type: integer
+            description: Maximum file size to send for analysis in MB
+            minimum: 15
+            maximum: 100
+          risk_level:
+            type: integer
+            description: Risk level to send for analysis
+            minimum: 0
+            maximum: 7
+      on_access_scan:
+        type: object
+        description: Local scan settings
+        properties:
+          enabled:
+            type: boolean
+            description: Whether local scan is enabled
+          mode:
+            type: string
+            description: The local scan mode for new files or all files
+            enum:
+              - NORMAL
+              - AGGRESSIVE
+      on_demand_scan:
+        type: object
+        description: Background scan settings
+        properties:
+          enabled:
+            type: boolean
+            description: Whether background scan is enabled
+          profile:
+            type: string
+            description: The background scan mode which limits the maximum number of files scanned per minute.
+            enum:
+              - NORMAL
+              - AGGRESSIVE
+          schedule:
+            type: object
+            description: The schedule for when the one time background scan will be performed
+          scan_usb:
+            type: string
+            description: Whether USB devices are scanned
+            enum:
+              - AUTOSCAN
+              - DISABLED
+          scan_cd_dvd:
+            type: string
+            description: Whether a CD or DVD is scanned
+            enum:
+              - AUTOSCAN
+              - DISABLED
+      signature_update:
+        type: object
+        description: Signature pack update settings
+        properties:
+          enabled:
+            type: boolean
+            description: Whether signature updates are enabled
+          schedule:
+            type: object
+            description: The schedule to update signatures
+      update_servers:
+        type: object
+        description: Servers for updating signatures
+        properties:
+          servers_override:
+            type: array
+            description: Update servers to override offsite/onsite settings
+            items:
+              type: string
+          servers_for_onsite_devices:
+            type: array
+            description: Update servers for internal devices
+            items:
+              type: object
+              properties:
+                server:
+                  type: string
+                preferred:
+                  type: boolean
+          servers_for_offsite_devices:
+            type: array
+            description: Update servers for offsite devices
+            items:
+              type: string
+  rules:
+    type: array
+    description: Permission or prevention rules
+    items: !include platform/models/policy_rule.yaml
+  directory_action_rules:
     type: array
-    description: Tags added to the threat ID of the alert
+    description: Rules to deny or allow the deployed sensors to send uploads from specific paths
     items:
-      type: string
-  threat_id:
-    type: string
-    description: ID assigned to a group of alerts with common criteria, based on alert type
-  threat_notes_present:
-    type: boolean
-    description: True if notes are present on the threat ID. False if notes are not present.
-  type:
-    type: string
-    enum:
-    - CB_ANALYTICS
-    - WATCHLIST
-    - DEVICE_CONTROL
-    - CONTAINER_RUNTIME
-    - HOST_BASED_FIREWALL
-    - INTRUSION_DETECTION_SYSTEM
-    - NETWORK_TRAFFIC_ANALYSIS
-    description: Type of alert generated
-  user_update_timestamp:
-    type: string
-    format: date-time
-    description: Timestamp of the last property of an alert changed by a user, such as the alert workflow or determination
-  vendor_id:
-    type: string
-    description: IDs of the vendors who produced the devices
-  vendor_name:
-    type: string
-    description: Names of the vendors who produced the devices
-  workflow:
+      type: object
+      properties:
+        file_upload:
+          type: boolean
+          description: Allow the deployed sensor to upload from path
+        protection:
+          type: boolean
+          description: Deny the deployed sensor from uploading at path
+        path:
+          type: string
+          description: The path to a file or directory
+  sensor_settings:
+    type: array
+    description: Settings to configure sensor behavior and capabilities
+    items:
+      type: object
+      properties:
+        name:
+          type: string
+          description: Name of the sensor setting
+        value:
+          type: string
+          description: Value for the sensor setting
+  managed_detection_response_permissions:
     type: object
-    description: Current workflow state of an alert. The workflow represents the flow from `OPEN` to `IN_PROGRESS` to `CLOSED` and captures who moved the alert into the current state. The history of these state transitions is available via the alert history route.
+    description: Permissions for Managed Detection and Response analysts to perform remediations on endpoints and workloads assigned to the policy
     properties:
-      change_timestamp:
-        type: string
-        format: date-time
-        description: When the last status change occurred
-      workflow_changed_by:
-        type: string
-        description: Who (or what) made the last status change
-      workflow_changed_by_rule_id:
-        type: string
-        description:
-      workflow_changed_by_type:
-        type: string
-        enum:
-        - SYSTEM
-        - USER
-        - API
-        - AUTOMATION
-        description:
-      workflow_closure_reason:
-        type: string  `NO_REASON`, `RESOLVED`, `RESOLVED_BENIGN_KNOWN_GOOD`, `DUPLICATE_CLEANUP`, `OTHER`
-        description: A more detailed description of why the alert was resolved
-      workflow_status:
-        type: string
-        enum:
-        - OPEN
-        - IN_PROGRESS
-        - CLOSED
-        description: primary value used to determine if the alert is active or inactive and displayed in the UI by default
+      policy_modification:
+        type: boolean
+        description: Allow MDR team to modify the policy
+      quarantine:
+        type: boolean
+        description: Allow MDR team to quarantine endpoints and workloads associated with the policy
+  version:
+    type: integer
+    description: Version of the policy
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/alert_note.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/alert_note.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/asset_group.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/asset_group.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/firewall_rule.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/firewall_rule.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/grant.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/grant.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/grouped_alert.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/grouped_alert.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/job.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/job.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/network_threat_metadata.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/network_threat_metadata.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/observation.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/observation.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/observation_facet.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/observation_facet.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/policy_rule.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/policy_rule.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/policy_ruleconfig.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/policy_ruleconfig.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -14,7 +14,10 @@
     description: Indicates where the rule config was inherited from
   category:
     type: string
     description: The category for this rule config
   parameters:
     type: object
     description: The parameters associated with this rule config
+  exclusions:
+    type: object
+    description: The exclusions associated with this rule config
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/process_facets.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/process_facets.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/profile.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/profile.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/reputation_override.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/reputation_override.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/user.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/user.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/models/workflow.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/models/workflow.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/network_threat_metadata.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/network_threat_metadata.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/observations.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/observations.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,14 +265,17 @@
         output = cb.get_object(url, query_params)
         return output["suggestions"]
 
     @staticmethod
     def bulk_get_details(cb, alert_id=None, observation_ids=None, timeout=0):
         """Bulk get details
 
+        Required Permissions:
+            org.search.events (READ, CREATE)
+
         Args:
             cb (CBCloudAPI): A reference to the CBCloudAPI object.
             alert_id (str):  An alert id to fetch associated observations
             observation_ids (list): A list of observation ids to fetch
             timeout (int): Observations details request timeout in milliseconds.  This may never be greater than
                 the configured default timeout.  If this value is 0, the configured default timeout is used.
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/policies.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 """Policy implementation as part of Platform API"""
 import copy
 import json
 from types import MappingProxyType
 from cbc_sdk.base import MutableBaseModel, BaseQuery, IterableQueryMixin, AsyncQueryMixin
 from cbc_sdk.platform.devices import Device
 from cbc_sdk.platform.policy_ruleconfigs import (PolicyRuleConfig, CorePreventionRuleConfig,
-                                                 HostBasedFirewallRuleConfig, DataCollectionRuleConfig)
+                                                 HostBasedFirewallRuleConfig, DataCollectionRuleConfig,
+                                                 BypassRuleConfig)
 from cbc_sdk.platform.previewer import DevicePolicyChangePreview
 from cbc_sdk.errors import ApiError, ServerError, InvalidObjectError
 
 
 SPECIFIC_RULECONFIGS = MappingProxyType({
     "core_prevention": CorePreventionRuleConfig,
     "host_based_firewall": HostBasedFirewallRuleConfig,
-    "data_collection": DataCollectionRuleConfig
+    "data_collection": DataCollectionRuleConfig,
+    "bypass": BypassRuleConfig
 })
 
 
 class Policy(MutableBaseModel):
     """
     Represents a policy within the organization.
 
@@ -693,14 +695,36 @@
 
         Returns:
             list: A list of PolicyRuleConfig objects.
         """
         return [rconf for rconf in self.object_rule_configs.values()]
 
     @property
+    def bypass_rule_configs(self):
+        """
+        Returns a dictionary of bypass rule configuration IDs and objects for this Policy.
+
+        Returns:
+            dict: A dictionary with bypass rule configuration IDs as keys and BypassRuleConfig objects
+                  as values.
+        """
+        return {key: rconf for (key, rconf) in self.object_rule_configs.items()
+                if isinstance(rconf, BypassRuleConfig)}
+
+    @property
+    def bypass_rule_configs_list(self):
+        """
+        Returns a list of bypass rule configuration objects for this Policy.
+
+        Returns:
+            list: A list of BypassRuleConfig objects.
+        """
+        return [rconf for rconf in self.object_rule_configs.values() if isinstance(rconf, BypassRuleConfig)]
+
+    @property
     def core_prevention_rule_configs(self):
         """
         Returns a dictionary of core prevention rule configuration IDs and objects for this Policy.
 
         Returns:
             dict: A dictionary with core prevention rule configuration IDs as keys and CorePreventionRuleConfig objects
                   as values.
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/policy_ruleconfigs.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/policy_ruleconfigs.py`

 * *Files 9% similar despite different names*

```diff
@@ -259,16 +259,18 @@
         else:
             raise InvalidObjectError(f"invalid core prevention ID: {self._model_unique_id}")
         return True
 
     def _update_ruleconfig(self):
         """Perform the internal update of the rule configuration object."""
         url = self.urlobject_single.format(self._cb.credentials.org_key, self._parent._model_unique_id)
-        body = [{"id": self.id, "parameters": self.parameters}]
-        self._cb.put_object(url, body)
+        body = {"id": self.id, "parameters": self.parameters}
+        if "exclusions" in self._info:
+            body["exclusions"] = self.exclusions
+        self._cb.put_object(url, [body])
 
     def _delete_ruleconfig(self):
         """Perform the internal delete of the rule configuration object."""
         url = self.urlobject_single.format(self._cb.credentials.org_key, self._parent._model_unique_id) + f"/{self.id}"
         self._cb.delete_object(url)
         self._info["parameters"] = copy.deepcopy({"WindowsAssignmentMode": "BLOCK"})  # mirror server side
 
@@ -288,24 +290,34 @@
         Args:
             mode (str): The new mode to set, either "REPORT" or "BLOCK". The default is "BLOCK".
         """
         if mode not in ("REPORT", "BLOCK"):
             raise ApiError(f"invalid assignment mode: {mode}")
         self.set_parameter("WindowsAssignmentMode", mode)
 
+    def replace_exclusions(self, exclusions):
+        """
+        Replaces all the exclusions for a bypasss rule configuration
+
+        Args:
+           exclusions(dict): The entire exclusion set to be replaced
+        """
+        self._mark_changed(True)
+        self._info['exclusions'] = exclusions
+
 
 class HostBasedFirewallRuleConfig(PolicyRuleConfig):
     """Represents a host-based firewall rule configuration in the policy."""
     urlobject = "/policyservice/v1/orgs/{0}/policies"
     urlobject_single = "/policyservice/v1/orgs/{0}/policies/{1}/rule_configs/host_based_firewall"
     swagger_meta_file = "platform/models/policy_ruleconfig.yaml"
 
     def __init__(self, cb, parent, model_unique_id=None, initial_data=None, force_init=False, full_doc=False):
         """
-        Initialize the CorePreventionRuleConfig object.
+        Initialize the HostBasedFirewallRuleConfig object.
 
         Args:
             cb (BaseAPI): Reference to API object used to communicate with the server.
             parent (Policy): The "parent" policy of this rule configuration.
             model_unique_id (str): ID of the rule configuration.
             initial_data (dict): Initial data used to populate the rule configuration.
             force_init (bool): If True, forces the object to be refreshed after constructing.  Default False.
@@ -639,23 +651,23 @@
 
     Create one of these objects, associating it with a Policy, and set its properties, then call its save() method to
     add the rule configuration to the policy. This requires the org.policies(UPDATE) permission.
 
     To update a DataCollectionRuleConfig, change the values of its property fields, then call its save() method.  This
     requires the org.policies(UPDATE) permission.
 
-    To delete an existing CorePreventionRuleConfig, call its delete() method. This requires the org.policies(DELETE)
+    To delete an existing DataCollectionRuleConfig, call its delete() method. This requires the org.policies(DELETE)
     permission.
     """
     urlobject_single = "/policyservice/v1/orgs/{0}/policies/{1}/rule_configs/data_collection"
     swagger_meta_file = "platform/models/policy_ruleconfig.yaml"
 
     def __init__(self, cb, parent, model_unique_id=None, initial_data=None, force_init=False, full_doc=False):
         """
-        Initialize the CorePreventionRuleConfig object.
+        Initialize the DataCollectionRuleConfig object.
 
         Args:
             cb (BaseAPI): Reference to API object used to communicate with the server.
             parent (Policy): The "parent" policy of this rule configuration.
             model_unique_id (str): ID of the rule configuration.
             initial_data (dict): Initial data used to populate the rule configuration.
             force_init (bool): If True, forces the object to be refreshed after constructing.  Default False.
@@ -692,7 +704,98 @@
         body = [{"id": self.id, "parameters": self.parameters}]
         self._cb.put_object(url, body)
 
     def _delete_ruleconfig(self):
         """Perform the internal delete of the rule configuration object."""
         url = self.urlobject_single.format(self._cb.credentials.org_key, self._parent._model_unique_id) + f"/{self.id}"
         self._cb.delete_object(url)
+
+
+class BypassRuleConfig(PolicyRuleConfig):
+    """
+    Represents a bypass rule configuration in the policy.
+
+    Create one of these objects, associating it with a Policy, and set its properties, then call its save() method to
+    add the rule configuration to the policy. This requires the org.policies(UPDATE) permission.
+
+    To update a BypassRuleConfig, change the values of its property fields, then call its save() method.  This
+    requires the org.policies(UPDATE) permission.
+
+    To delete an existing BypassRuleConfig, call its delete() method. This requires the org.policies(DELETE)
+    permission.
+    """
+    urlobject_single = "/policyservice/v1/orgs/{0}/policies/{1}/rule_configs/bypass"
+    swagger_meta_file = "platform/models/policy_ruleconfig.yaml"
+
+    def __init__(self, cb, parent, model_unique_id=None, initial_data=None, force_init=False, full_doc=False):
+        """
+        Initialize the BypassRuleConfig object.
+
+        Args:
+            cb (BaseAPI): Reference to API object used to communicate with the server.
+            parent (Policy): The "parent" policy of this rule configuration.
+            model_unique_id (str): ID of the rule configuration.
+            initial_data (dict): Initial data used to populate the rule configuration.
+            force_init (bool): If True, forces the object to be refreshed after constructing.  Default False.
+            full_doc (bool): If True, object is considered "fully" initialized. Default False.
+        """
+        super(BypassRuleConfig, self).__init__(cb, parent, model_unique_id, initial_data, force_init, full_doc)
+
+    def _refresh(self):
+        """
+        Refreshes the rule configuration object from the server.
+
+        Required Permissions:
+            org.policies (READ)
+
+        Returns:
+            bool: True if the refresh was successful.
+
+        Raises:
+            InvalidObjectError: If the object is unparented or its ID is invalid.
+        """
+        url = self.urlobject_single.format(self._cb.credentials.org_key, self._parent._model_unique_id)
+        return_data = self._cb.get_object(url)
+        ruleconfig_data = [d for d in return_data.get("results", []) if d.get("id", "") == self._model_unique_id]
+        if ruleconfig_data:
+            self._info = ruleconfig_data[0]
+            self._mark_changed(False)
+        else:
+            raise InvalidObjectError(f"invalid data collection ID: {self._model_unique_id}")
+        return True
+
+    def _update_ruleconfig(self):
+        """Perform the internal update of the rule configuration object."""
+        url = self.urlobject_single.format(self._cb.credentials.org_key, self._parent._model_unique_id)
+        body = {"id": self.id}
+        if "exclusions" in self._info:
+            body["exclusions"] = self.exclusions
+
+        self._cb.put_object(url, body)
+
+    def _delete_ruleconfig(self):
+        """Perform the internal delete of the rule configuration object."""
+        url = self.urlobject_single.format(self._cb.credentials.org_key, self._parent._model_unique_id)
+        self._cb.delete_object(url)
+
+    def replace_exclusions(self, exclusions):
+        """
+        Replaces all the exclusions for a bypasss rule configuration
+
+        Args:
+           exclusions(dict): The entire exclusion set to be replaced
+        """
+        self._mark_changed(True)
+        self._info['exclusions'] = exclusions
+
+    @property
+    def parameter_names(self):
+        """Not Supported"""
+        raise Exception("Not Suppported")
+
+    def get_parameter(self, name, default_value=None):
+        """Not Supported"""
+        raise Exception("Not Suppported")
+
+    def set_parameter(self, name, value):
+        """Not Supported"""
+        raise Exception("Not Suppported")
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/previewer.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/previewer.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/processes.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 class Process(UnrefreshableModel):
     """
     Information about a process running on one of the endpoints connected to the Carbon Black Cloud.
 
     Objects of this type are retrieved through queries to the Carbon Black Cloud server, such as via
     ``AsyncProcessQuery``.
 
+    Processes have many fields, too many to list here; for a complete list of available fields, visit
+    `the Search Fields page
+    <https://developer.carbonblack.com/reference/carbon-black-cloud/platform/latest/platform-search-fields/>`_
+    on the Carbon Black Developer Network, and filter on the ``PROCESS`` route.
+
     Examples:
         >>> # use the Process GUID directly
         >>> process = api.select(Process, "WNEXFKQ7-00050603-0000066c-00000000-1d6c9acb43e29bb")
 
         >>> # use the Process GUID in a where() clause
         >>> process_query = api.select(Process).where(process_guid=
         ...    "WNEXFKQ7-00050603-0000066c-00000000-1d6c9acb43e29bb")
@@ -658,14 +663,26 @@
         if not isinstance(rows, int):
             raise ApiError(f"Rows must be an integer. {rows} is a {type(rows)}.")
         if rows > 10000:
             raise ApiError("Maximum allowed value for rows is 10000")
         self._batch_size = rows
         return self
 
+    def set_collapse_field(self, field):
+        """
+        Sets the 'collapse_field' query parameter, which queries the file name depending on field.
+
+        Args:
+            field (list): query parameters to get file details.
+        """
+        if not isinstance(field, list):
+            raise ApiError(f"Field must be list. {field} is a {type(field)}.")
+        self._collapse_field = field
+        return self
+
     def _submit(self):
         """
         Submits the query to the server.
 
         Required Permissions:
             org.search.events(CREATE)
         """
@@ -1019,23 +1036,36 @@
             query_parameters = {"format": "tree"}
             result = self._cb.get_object(result_url, query_parameters=query_parameters)
             if result["exception"] == "":
                 yield self._doc_class(self._cb, model_unique_id=self._query_token, initial_data=result["tree"])
             else:
                 raise ApiError(f"Failed to get Process Tree: {result['exception']}")
 
-    def _perform_query(self):
+    def _perform_query(self, from_row=0, max_rows=-1):
         """
         Iterate over the results of the query.
 
         Required Permissions:
             org.search.events(CREATE, READ)
+
+        Args:
+            from_row (int): Row to start iterating from (default 0).
+            max_rows(int): Number of rows to enumerate (default -1, meaning "all rows").
+
+        Yields:
+            Process.Summary or Process.Tree: The enumerated results.
         """
-        for item in self.results:
+        returned_rows = 0
+        for ndx, item in enumerate(self.results):
+            if ndx < from_row:
+                continue
             yield item
+            returned_rows += 1
+            if 0 < max_rows <= returned_rows:
+                break
 
     @property
     def results(self):
         """
         Return the results of this query.  If the query has not yet been run, it is run to determine the results.
 
         Required Permissions:
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/reputation.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/reputation.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/users.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/users.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/platform/vulnerability_assessment.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/platform/vulnerability_assessment.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,18 +290,22 @@
         """
         if severity and severity not in self.VALID_SEVERITY:
             raise ApiError("Invalid severity")
         else:
             self._severity = severity
         return self
 
-    def _perform_query(self):
+    def _perform_query(self, from_row=0, max_rows=-1):
         """
         Performs the query and returns the Vulnerability.OrgSummary
 
+        Args:
+            from_row (int): Not used, retained for compatibility.
+            max_rows (int): Not used, retained for compatibility.
+
         Returns:
             Vulnerability.OrgSummary: The vulnerabilty summary for an organization
         """
         query_params = {}
         if self._vcenter_uuid:
             url = "/vcenters/{}/vulnerabilities/summary".format(self._vcenter_uuid)
         else:
```

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/rest_api.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/rest_api.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/winerror.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/winerror.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/computeResource.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/computeResource.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/deviceVulnerabilitySummary.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/deviceVulnerabilitySummary.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/sensorKit.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/sensorKit.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/vulnerability.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/vulnerability.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/vulnerabilityAssetView.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/vulnerabilityAssetView.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/models/vulnerabilityOrgSummary.yaml` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/models/vulnerabilityOrgSummary.yaml`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/nsx_remediation.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/nsx_remediation.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/sensor_lifecycle.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/sensor_lifecycle.py`

 * *Files identical despite different names*

### Comparing `carbon-black-cloud-sdk-1.5.1/src/cbc_sdk/workload/vm_workloads_search.py` & `carbon-black-cloud-sdk-1.5.2/src/cbc_sdk/workload/vm_workloads_search.py`

 * *Files identical despite different names*

