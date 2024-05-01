# Comparing `tmp/iam_actions-1.2.20240429.tar.gz` & `tmp/iam_actions-1.2.20240430.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240429.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240430.tar", max compression
```

## Comparing `iam_actions-1.2.20240429.tar` & `iam_actions-1.2.20240430.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/README.md
--rw-r--r--   0        0        0      228 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/iam_actions/__init__.py
--rw-r--r--   0        0        0  4812377 2024-04-29 02:20:49.578845 iam_actions-1.2.20240429/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-29 02:19:44.966684 iam_actions-1.2.20240429/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-29 02:19:44.970684 iam_actions-1.2.20240429/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-29 02:19:44.970684 iam_actions-1.2.20240429/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-29 02:19:44.970684 iam_actions-1.2.20240429/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-29 02:19:44.970684 iam_actions-1.2.20240429/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-29 02:19:44.970684 iam_actions-1.2.20240429/iam_actions/generate/services.py
--rw-r--r--   0        0        0   625917 2024-04-29 02:20:49.578845 iam_actions-1.2.20240429/iam_actions/policies.json
--rw-r--r--   0        0        0   209050 2024-04-29 02:20:49.578845 iam_actions-1.2.20240429/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   607313 2024-04-29 02:20:49.578845 iam_actions-1.2.20240429/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-29 02:20:50.218846 iam_actions-1.2.20240429/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240429/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240429/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/README.md
+-rw-r--r--   0        0        0      228 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4816205 2024-04-30 02:19:11.333017 iam_actions-1.2.20240430/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-30 02:18:06.304433 iam_actions-1.2.20240430/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   626252 2024-04-30 02:19:11.333017 iam_actions-1.2.20240430/iam_actions/policies.json
+-rw-r--r--   0        0        0   209050 2024-04-30 02:19:11.333017 iam_actions-1.2.20240430/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   607639 2024-04-30 02:19:11.333017 iam_actions-1.2.20240430/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-30 02:19:12.009023 iam_actions-1.2.20240430/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240430/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240430/PKG-INFO
```

### Comparing `iam_actions-1.2.20240429/LICENSE` & `iam_actions-1.2.20240430/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240429/README.md` & `iam_actions-1.2.20240430/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240429/iam_actions/actions.json` & `iam_actions-1.2.20240430/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999258795712401%*

 * *Differences: {"'codepipeline'": "{'RollbackStage': {'access_level': 'Write', 'description': 'Grants permission "*

 * *                   "to rollback the stage to a previous successful execution', 'resources': "*

 * *                   "['stage']}}",*

 * * "'ec2'": "{'AcceptTransitGatewayMulticastDomainAssociations': {'condition_keys': {insert: [(3, "*

 * *          "'ec2:transitGatewayAttachmentId'), (4, 'ec2:transitGatewayMulticastDomainId')]}}, "*

 * *          "'AcceptTransitGatewayPeeringAttachment': {'condition_keys': {insert: [(3, "*

 * *     […]*

```diff
@@ -29453,20 +29453,22 @@
             "description": "Grants permission to resume the pipeline execution by retrying the last failed actions in a stage",
             "orphan": false,
             "resources": [
                 "stage"
             ]
         },
         "RollbackStage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RollbackStage",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to rollback the stage to a previous successful execution",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "stage"
+            ]
         },
         "StartPipelineExecution": {
             "access_level": "Write",
             "action": "StartPipelineExecution",
             "condition_keys": [],
             "description": "Grants permission to run the most recent revision through the pipeline",
             "orphan": false,
@@ -50003,44 +50005,48 @@
         },
         "AcceptTransitGatewayMulticastDomainAssociations": {
             "access_level": "Write",
             "action": "AcceptTransitGatewayMulticastDomainAssociations",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to accept a request to associate subnets with a transit gateway multicast domain",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-multicast-domain"
             ]
         },
         "AcceptTransitGatewayPeeringAttachment": {
             "access_level": "Write",
             "action": "AcceptTransitGatewayPeeringAttachment",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId"
             ],
             "description": "Grants permission to accept a transit gateway peering attachment request",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment"
             ]
         },
         "AcceptTransitGatewayVpcAttachment": {
             "access_level": "Write",
             "action": "AcceptTransitGatewayVpcAttachment",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId"
             ],
             "description": "Grants permission to accept a request to attach a VPC to a transit gateway",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment"
             ]
         },
@@ -50439,15 +50445,17 @@
             "action": "AssociateTransitGatewayMulticastDomain",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:AvailabilityZone",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SubnetID",
-                "ec2:Vpc"
+                "ec2:Vpc",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to associate an attachment and list of subnets with a transit gateway multicast domain",
             "orphan": false,
             "resources": [
                 "subnet",
                 "transit-gateway-attachment",
                 "transit-gateway-multicast-domain"
@@ -50455,30 +50463,34 @@
         },
         "AssociateTransitGatewayPolicyTable": {
             "access_level": "Write",
             "action": "AssociateTransitGatewayPolicyTable",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayPolicyTableId"
             ],
             "description": "Grants permission to associate a policy table with a transit gateway attachment",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-policy-table"
             ]
         },
         "AssociateTransitGatewayRouteTable": {
             "access_level": "Write",
             "action": "AssociateTransitGatewayRouteTable",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to associate an attachment with a transit gateway route table",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-route-table"
             ]
@@ -51205,15 +51217,17 @@
                 "ec2:NetworkInterfaceID",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:Subnet",
                 "ec2:SubnetID",
                 "ec2:Tenancy",
                 "ec2:Vpc",
-                "ec2:VpcID"
+                "ec2:VpcID",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayId"
             ],
             "description": "Grants permission to create one or more flow logs to capture IP traffic for a network interface",
             "orphan": false,
             "resources": [
                 "network-interface",
                 "subnet",
                 "transit-gateway",
@@ -51670,15 +51684,16 @@
                 "ec2:Region",
                 "ec2:RequesterVpc",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:RootDeviceType",
                 "ec2:Subnet",
                 "ec2:Tenancy",
                 "ec2:Vpc",
-                "ec2:VpcPeeringConnectionID"
+                "ec2:VpcPeeringConnectionID",
+                "ec2:transitGatewayId"
             ],
             "description": "Grants permission to create a path to analyze for reachability",
             "orphan": false,
             "resources": [
                 "instance",
                 "internet-gateway",
                 "network-insights-path",
@@ -52096,15 +52111,22 @@
                 "ec2:VolumeID",
                 "ec2:VolumeIops",
                 "ec2:VolumeSize",
                 "ec2:VolumeThroughput",
                 "ec2:VolumeType",
                 "ec2:Vpc",
                 "ec2:VpcID",
-                "ec2:VpcPeeringConnectionID"
+                "ec2:VpcPeeringConnectionID",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayConnectPeerId",
+                "ec2:transitGatewayId",
+                "ec2:transitGatewayMulticastDomainId",
+                "ec2:transitGatewayPolicyTableId",
+                "ec2:transitGatewayRouteTableAnnouncementId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to add or overwrite one or more tags for Amazon EC2 resources",
             "orphan": false,
             "resources": [
                 "capacity-reservation",
                 "capacity-reservation-fleet",
                 "carrier-gateway",
@@ -52264,29 +52286,31 @@
         },
         "CreateTransitGateway": {
             "access_level": "Write",
             "action": "CreateTransitGateway",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
-                "ec2:Region"
+                "ec2:Region",
+                "ec2:transitGatewayId"
             ],
             "description": "Grants permission to create a transit gateway",
             "orphan": false,
             "resources": [
                 "transit-gateway"
             ]
         },
         "CreateTransitGatewayConnect": {
             "access_level": "Write",
             "action": "CreateTransitGatewayConnect",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
-                "ec2:Region"
+                "ec2:Region",
+                "ec2:transitGatewayAttachmentId"
             ],
             "description": "Grants permission to create a Connect attachment from a specified transit gateway attachment",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment"
             ]
         },
@@ -52294,15 +52318,17 @@
             "access_level": "Write",
             "action": "CreateTransitGatewayConnectPeer",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayConnectPeerId"
             ],
             "description": "Grants permission to create a Connect peer between a transit gateway and an appliance",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-connect-peer"
             ]
@@ -52311,15 +52337,17 @@
             "access_level": "Write",
             "action": "CreateTransitGatewayMulticastDomain",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayId",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to create a multicast domain for a transit gateway",
             "orphan": false,
             "resources": [
                 "transit-gateway",
                 "transit-gateway-multicast-domain"
             ]
@@ -52328,15 +52356,17 @@
             "access_level": "Write",
             "action": "CreateTransitGatewayPeeringAttachment",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayId"
             ],
             "description": "Grants permission to request a transit gateway peering attachment between a requester and accepter transit gateway",
             "orphan": false,
             "resources": [
                 "transit-gateway",
                 "transit-gateway-attachment"
             ]
@@ -52345,30 +52375,34 @@
             "access_level": "Write",
             "action": "CreateTransitGatewayPolicyTable",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayId",
+                "ec2:transitGatewayPolicyTableId"
             ],
             "description": "Grants permission to create a transit gateway policy table",
             "orphan": false,
             "resources": [
                 "transit-gateway",
                 "transit-gateway-policy-table"
             ]
         },
         "CreateTransitGatewayPrefixListReference": {
             "access_level": "Write",
             "action": "CreateTransitGatewayPrefixListReference",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to create a transit gateway prefix list reference",
             "orphan": false,
             "resources": [
                 "prefix-list",
                 "transit-gateway-attachment",
                 "transit-gateway-route-table"
@@ -52376,15 +52410,17 @@
         },
         "CreateTransitGatewayRoute": {
             "access_level": "Write",
             "action": "CreateTransitGatewayRoute",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to create a static route for a transit gateway route table",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-route-table"
             ]
@@ -52393,15 +52429,17 @@
             "access_level": "Write",
             "action": "CreateTransitGatewayRouteTable",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to create a route table for a transit gateway",
             "orphan": false,
             "resources": [
                 "transit-gateway",
                 "transit-gateway-route-table"
             ]
@@ -52410,15 +52448,18 @@
             "access_level": "Write",
             "action": "CreateTransitGatewayRouteTableAnnouncement",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayRouteTableAnnouncementId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to create an announcement for a transit gateway route table",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-route-table",
                 "transit-gateway-route-table-announcement"
@@ -52433,15 +52474,17 @@
                 "aws:TagKeys",
                 "ec2:AvailabilityZone",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SubnetID",
                 "ec2:Tenancy",
                 "ec2:Vpc",
-                "ec2:VpcID"
+                "ec2:VpcID",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayId"
             ],
             "description": "Grants permission to attach a VPC to a transit gateway",
             "orphan": false,
             "resources": [
                 "subnet",
                 "transit-gateway",
                 "transit-gateway-attachment",
@@ -52665,15 +52708,17 @@
                 "ec2:Phase2IntegrityAlgorithms",
                 "ec2:Phase2LifetimeSeconds",
                 "ec2:Region",
                 "ec2:RekeyFuzzPercentage",
                 "ec2:RekeyMarginTimeSeconds",
                 "ec2:ReplayWindowSizePackets",
                 "ec2:ResourceTag/${TagKey}",
-                "ec2:RoutingType"
+                "ec2:RoutingType",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayId"
             ],
             "description": "Grants permission to create a VPN connection between a virtual private gateway or transit gateway and a customer gateway",
             "orphan": false,
             "resources": [
                 "customer-gateway",
                 "transit-gateway",
                 "transit-gateway-attachment",
@@ -53581,156 +53626,167 @@
         },
         "DeleteTransitGateway": {
             "access_level": "Write",
             "action": "DeleteTransitGateway",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayId"
             ],
             "description": "Grants permission to delete a transit gateway",
             "orphan": false,
             "resources": [
                 "transit-gateway"
             ]
         },
         "DeleteTransitGatewayConnect": {
             "access_level": "Write",
             "action": "DeleteTransitGatewayConnect",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId"
             ],
             "description": "Grants permission to delete a transit gateway connect attachment",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment"
             ]
         },
         "DeleteTransitGatewayConnectPeer": {
             "access_level": "Write",
             "action": "DeleteTransitGatewayConnectPeer",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayConnectPeerId"
             ],
             "description": "Grants permission to delete a transit gateway connect peer",
             "orphan": false,
             "resources": [
                 "transit-gateway-connect-peer"
             ]
         },
         "DeleteTransitGatewayMulticastDomain": {
             "access_level": "Write",
             "action": "DeleteTransitGatewayMulticastDomain",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to delete a transit gateway multicast domain",
             "orphan": false,
             "resources": [
                 "transit-gateway-multicast-domain"
             ]
         },
         "DeleteTransitGatewayPeeringAttachment": {
             "access_level": "Write",
             "action": "DeleteTransitGatewayPeeringAttachment",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId"
             ],
             "description": "Grants permission to delete a peering attachment from a transit gateway",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment"
             ]
         },
         "DeleteTransitGatewayPolicyTable": {
             "access_level": "Write",
             "action": "DeleteTransitGatewayPolicyTable",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayPolicyTableId"
             ],
             "description": "Grants permission to delete a transit gateway policy table",
             "orphan": false,
             "resources": [
                 "transit-gateway-policy-table"
             ]
         },
         "DeleteTransitGatewayPrefixListReference": {
             "access_level": "Write",
             "action": "DeleteTransitGatewayPrefixListReference",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to delete a transit gateway prefix list reference",
             "orphan": false,
             "resources": [
                 "prefix-list",
                 "transit-gateway-route-table"
             ]
         },
         "DeleteTransitGatewayRoute": {
             "access_level": "Write",
             "action": "DeleteTransitGatewayRoute",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to delete a route from a transit gateway route table",
             "orphan": false,
             "resources": [
                 "transit-gateway-route-table"
             ]
         },
         "DeleteTransitGatewayRouteTable": {
             "access_level": "Write",
             "action": "DeleteTransitGatewayRouteTable",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to delete a transit gateway route table",
             "orphan": false,
             "resources": [
                 "transit-gateway-route-table"
             ]
         },
         "DeleteTransitGatewayRouteTableAnnouncement": {
             "access_level": "Write",
             "action": "DeleteTransitGatewayRouteTableAnnouncement",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayRouteTableAnnouncementId"
             ],
             "description": "Grants permission to delete a transit gateway route table announcement",
             "orphan": false,
             "resources": [
                 "transit-gateway-route-table-announcement"
             ]
         },
         "DeleteTransitGatewayVpcAttachment": {
             "access_level": "Write",
             "action": "DeleteTransitGatewayVpcAttachment",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId"
             ],
             "description": "Grants permission to delete a VPC attachment from a transit gateway",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment"
             ]
         },
@@ -54018,15 +54074,16 @@
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:AvailabilityZone",
                 "ec2:NetworkInterfaceID",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:Subnet",
-                "ec2:Vpc"
+                "ec2:Vpc",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to deregister one or more network interface members from a group IP address in a transit gateway multicast domain",
             "orphan": false,
             "resources": [
                 "network-interface",
                 "transit-gateway-multicast-domain"
             ]
@@ -54037,15 +54094,16 @@
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:AvailabilityZone",
                 "ec2:NetworkInterfaceID",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:Subnet",
-                "ec2:Vpc"
+                "ec2:Vpc",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to deregister one or more network interface sources from a group IP address in a transit gateway multicast domain",
             "orphan": false,
             "resources": [
                 "network-interface",
                 "transit-gateway-multicast-domain"
             ]
@@ -56009,15 +56067,18 @@
         },
         "DisableTransitGatewayRouteTablePropagation": {
             "access_level": "Write",
             "action": "DisableTransitGatewayRouteTablePropagation",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayRouteTableAnnouncementId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to disable a resource attachment from propagating routes to the specified propagation route table",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-route-table",
                 "transit-gateway-route-table-announcement"
@@ -56265,15 +56326,17 @@
             "action": "DisassociateTransitGatewayMulticastDomain",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:AvailabilityZone",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SubnetID",
-                "ec2:Vpc"
+                "ec2:Vpc",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to disassociate one or more subnets from a transit gateway multicast domain",
             "orphan": false,
             "resources": [
                 "subnet",
                 "transit-gateway-attachment",
                 "transit-gateway-multicast-domain"
@@ -56281,30 +56344,34 @@
         },
         "DisassociateTransitGatewayPolicyTable": {
             "access_level": "Write",
             "action": "DisassociateTransitGatewayPolicyTable",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayPolicyTableId"
             ],
             "description": "Grants permission to disassociate a policy table from a transit gateway",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-policy-table"
             ]
         },
         "DisassociateTransitGatewayRouteTable": {
             "access_level": "Write",
             "action": "DisassociateTransitGatewayRouteTable",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to disassociate a resource attachment from a transit gateway route table",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-route-table"
             ]
@@ -56517,15 +56584,18 @@
         },
         "EnableTransitGatewayRouteTablePropagation": {
             "access_level": "Write",
             "action": "EnableTransitGatewayRouteTablePropagation",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayRouteTableAnnouncementId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to enable an attachment to propagate routes to a propagation route table",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-route-table",
                 "transit-gateway-route-table-announcement"
@@ -57232,43 +57302,46 @@
         },
         "GetTransitGatewayMulticastDomainAssociations": {
             "access_level": "List",
             "action": "GetTransitGatewayMulticastDomainAssociations",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to get information about the associations for a transit gateway multicast domain",
             "orphan": false,
             "resources": [
                 "transit-gateway-multicast-domain"
             ]
         },
         "GetTransitGatewayPolicyTableAssociations": {
             "access_level": "List",
             "action": "GetTransitGatewayPolicyTableAssociations",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayPolicyTableId"
             ],
             "description": "Grants permission to get information about associations for a transit gateway policy table",
             "orphan": false,
             "resources": [
                 "transit-gateway-policy-table"
             ]
         },
         "GetTransitGatewayPolicyTableEntries": {
             "access_level": "List",
             "action": "GetTransitGatewayPolicyTableEntries",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayPolicyTableId"
             ],
             "description": "Grants permission to get information about associations for a transit gateway policy table entry",
             "orphan": false,
             "resources": [
                 "transit-gateway-policy-table"
             ]
         },
@@ -58434,15 +58507,17 @@
             "access_level": "Write",
             "action": "ModifyTransitGateway",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Attribute",
                 "ec2:Attribute/${AttributeName}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to modify a transit gateway",
             "orphan": false,
             "resources": [
                 "transit-gateway",
                 "transit-gateway-route-table"
             ]
@@ -58451,15 +58526,17 @@
             "access_level": "Write",
             "action": "ModifyTransitGatewayPrefixListReference",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Attribute",
                 "ec2:Attribute/${AttributeName}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to modify a transit gateway prefix list reference",
             "orphan": false,
             "resources": [
                 "prefix-list",
                 "transit-gateway-attachment",
                 "transit-gateway-route-table"
@@ -58472,15 +58549,16 @@
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Attribute",
                 "ec2:Attribute/${AttributeName}",
                 "ec2:AvailabilityZone",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:SubnetID",
-                "ec2:Vpc"
+                "ec2:Vpc",
+                "ec2:transitGatewayAttachmentId"
             ],
             "description": "Grants permission to modify a VPC attachment on a transit gateway",
             "orphan": false,
             "resources": [
                 "subnet",
                 "transit-gateway-attachment"
             ]
@@ -59158,15 +59236,16 @@
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:AvailabilityZone",
                 "ec2:NetworkInterfaceID",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:Subnet",
-                "ec2:Vpc"
+                "ec2:Vpc",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to register one or more network interfaces as a member of a group IP address in a transit gateway multicast domain",
             "orphan": false,
             "resources": [
                 "network-interface",
                 "transit-gateway-multicast-domain"
             ]
@@ -59177,59 +59256,64 @@
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:AvailabilityZone",
                 "ec2:NetworkInterfaceID",
                 "ec2:Region",
                 "ec2:ResourceTag/${TagKey}",
                 "ec2:Subnet",
-                "ec2:Vpc"
+                "ec2:Vpc",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to register one or more network interfaces as a source of a group IP address in a transit gateway multicast domain",
             "orphan": false,
             "resources": [
                 "network-interface",
                 "transit-gateway-multicast-domain"
             ]
         },
         "RejectTransitGatewayMulticastDomainAssociations": {
             "access_level": "Write",
             "action": "RejectTransitGatewayMulticastDomainAssociations",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to reject requests to associate cross-account subnets with a transit gateway multicast domain",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-multicast-domain"
             ]
         },
         "RejectTransitGatewayPeeringAttachment": {
             "access_level": "Write",
             "action": "RejectTransitGatewayPeeringAttachment",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId"
             ],
             "description": "Grants permission to reject a transit gateway peering attachment request",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment"
             ]
         },
         "RejectTransitGatewayVpcAttachment": {
             "access_level": "Write",
             "action": "RejectTransitGatewayVpcAttachment",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId"
             ],
             "description": "Grants permission to reject a request to attach a VPC to a transit gateway",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment"
             ]
         },
@@ -59416,15 +59500,17 @@
         },
         "ReplaceTransitGatewayRoute": {
             "access_level": "Write",
             "action": "ReplaceTransitGatewayRoute",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to replace a route in a transit gateway route table",
             "orphan": false,
             "resources": [
                 "transit-gateway-attachment",
                 "transit-gateway-route-table"
             ]
@@ -59453,15 +59539,17 @@
             "orphan": false,
             "resources": []
         },
         "RequestSpotFleet": {
             "access_level": "Write",
             "action": "RequestSpotFleet",
             "condition_keys": [
+                "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
                 "ec2:AvailabilityZone",
                 "ec2:ImageID",
                 "ec2:ImageType",
                 "ec2:KeyPairName",
                 "ec2:KeyPairType",
                 "ec2:OutpostArn",
                 "ec2:Owner",
@@ -59908,29 +59996,31 @@
         },
         "SearchTransitGatewayMulticastGroups": {
             "access_level": "List",
             "action": "SearchTransitGatewayMulticastGroups",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayMulticastDomainId"
             ],
             "description": "Grants permission to search for groups, sources, and members in a transit gateway multicast domain",
             "orphan": false,
             "resources": [
                 "transit-gateway-multicast-domain"
             ]
         },
         "SearchTransitGatewayRoutes": {
             "access_level": "List",
             "action": "SearchTransitGatewayRoutes",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "ec2:Region",
-                "ec2:ResourceTag/${TagKey}"
+                "ec2:ResourceTag/${TagKey}",
+                "ec2:transitGatewayRouteTableId"
             ],
             "description": "Grants permission to search for routes in a transit gateway route table",
             "orphan": false,
             "resources": [
                 "transit-gateway-route-table"
             ]
         },
@@ -161635,14 +161725,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete a table in your account",
             "orphan": false,
             "resources": [
                 "table"
             ]
         },
+        "DescribeAccountSettings": {
+            "access_level": "Undocumented",
+            "action": "DescribeAccountSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeBatchLoadTask": {
             "access_level": "Read",
             "action": "DescribeBatchLoadTask",
             "condition_keys": [],
             "description": "Grants permission to describe a batch load task in your account",
             "orphan": false,
             "resources": []
@@ -161858,14 +161956,22 @@
             "orphan": false,
             "resources": [
                 "database",
                 "scheduled-query",
                 "table"
             ]
         },
+        "UpdateAccountSettings": {
+            "access_level": "Undocumented",
+            "action": "UpdateAccountSettings",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateDatabase": {
             "access_level": "Write",
             "action": "UpdateDatabase",
             "condition_keys": [],
             "description": "Grants permission to update a database in your account",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20240429/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240430/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240429/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240430/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240429/iam_actions/generate/generate.py` & `iam_actions-1.2.20240430/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240429/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240430/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240429/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240430/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240429/iam_actions/generate/services.py` & `iam_actions-1.2.20240430/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240429/iam_actions/policies.json` & `iam_actions-1.2.20240430/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999988528700868%*

 * *Differences: {"'serviceMap'": "{'Amazon Timestream': {'Actions': {insert: [(8, 'DescribeAccountSettings'), (32, "*

 * *                 "'UpdateAccountSettings')]}}, 'Amazon EC2': {'conditionKeys': {insert: [(112, "*

 * *                 "'ec2:transitGatewayAttachmentId'), (113, 'ec2:transitGatewayConnectPeerId'), "*

 * *                 "(114, 'ec2:transitGatewayId'), (115, 'ec2:transitGatewayMulticastDomainId'), "*

 * *                 "(116, 'ec2:transitGatewayPolicyTableId'), (117, "*

 * *                 "'ec2:transitGatewayRouteTableAnnou […]*

```diff
@@ -14623,15 +14623,22 @@
                 "ec2:VolumeThroughput",
                 "ec2:VolumeType",
                 "ec2:Vpc",
                 "ec2:VpcID",
                 "ec2:VpcPeeringConnectionID",
                 "ec2:VpceServiceName",
                 "ec2:VpceServiceOwner",
-                "ec2:VpceServicePrivateDnsName"
+                "ec2:VpceServicePrivateDnsName",
+                "ec2:transitGatewayAttachmentId",
+                "ec2:transitGatewayConnectPeerId",
+                "ec2:transitGatewayId",
+                "ec2:transitGatewayMulticastDomainId",
+                "ec2:transitGatewayPolicyTableId",
+                "ec2:transitGatewayRouteTableAnnouncementId",
+                "ec2:transitGatewayRouteTableId"
             ]
         },
         "Amazon EC2 Auto Scaling": {
             "ARNFormat": "arn:aws:autoscaling:${Region}:${Account}:${RelativeId}",
             "ARNRegex": "^arn:aws:autoscaling:.+:.+:.+",
             "Actions": [
                 "AttachInstances",
@@ -21533,14 +21540,15 @@
                 "CreateBatchLoadTask",
                 "CreateDatabase",
                 "CreateScheduledQuery",
                 "CreateTable",
                 "DeleteDatabase",
                 "DeleteScheduledQuery",
                 "DeleteTable",
+                "DescribeAccountSettings",
                 "DescribeBatchLoadTask",
                 "DescribeDatabase",
                 "DescribeEndpoints",
                 "DescribeScheduledQuery",
                 "DescribeTable",
                 "ExecuteScheduledQuery",
                 "GetAwsBackupStatus",
@@ -21556,14 +21564,15 @@
                 "Select",
                 "SelectValues",
                 "StartAwsBackupJob",
                 "StartAwsRestoreJob",
                 "TagResource",
                 "Unload",
                 "UntagResource",
+                "UpdateAccountSettings",
                 "UpdateDatabase",
                 "UpdateScheduledQuery",
                 "UpdateTable",
                 "WriteRecords"
             ],
             "HasResource": true,
             "StringPrefix": "timestream",
```

### Comparing `iam_actions-1.2.20240429/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240430/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240429/iam_actions/services.json` & `iam_actions-1.2.20240430/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999880019575399%*

 * *Differences: {"'ec2'": "{'ConditionKeys': {insert: [(112, 'ec2:transitGatewayAttachmentId'), (113, "*

 * *          "'ec2:transitGatewayConnectPeerId'), (114, 'ec2:transitGatewayId'), (115, "*

 * *          "'ec2:transitGatewayMulticastDomainId'), (116, 'ec2:transitGatewayPolicyTableId'), (117, "*

 * *          "'ec2:transitGatewayRouteTableAnnouncementId'), (118, "*

 * *          "'ec2:transitGatewayRouteTableId')]}}",*

 * * "'timestream'": "{'Actions': {insert: [(8, 'DescribeAccountSettings'), (32, "*

 * *                 "'UpdateAccountSettings') […]*

```diff
@@ -8096,15 +8096,22 @@
             "ec2:VolumeThroughput",
             "ec2:VolumeType",
             "ec2:Vpc",
             "ec2:VpcID",
             "ec2:VpcPeeringConnectionID",
             "ec2:VpceServiceName",
             "ec2:VpceServiceOwner",
-            "ec2:VpceServicePrivateDnsName"
+            "ec2:VpceServicePrivateDnsName",
+            "ec2:transitGatewayAttachmentId",
+            "ec2:transitGatewayConnectPeerId",
+            "ec2:transitGatewayId",
+            "ec2:transitGatewayMulticastDomainId",
+            "ec2:transitGatewayPolicyTableId",
+            "ec2:transitGatewayRouteTableAnnouncementId",
+            "ec2:transitGatewayRouteTableId"
         ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon EC2"
         ]
     },
     "ec2-instance-connect": {
@@ -22698,14 +22705,15 @@
             "CreateBatchLoadTask",
             "CreateDatabase",
             "CreateScheduledQuery",
             "CreateTable",
             "DeleteDatabase",
             "DeleteScheduledQuery",
             "DeleteTable",
+            "DescribeAccountSettings",
             "DescribeBatchLoadTask",
             "DescribeDatabase",
             "DescribeEndpoints",
             "DescribeScheduledQuery",
             "DescribeTable",
             "ExecuteScheduledQuery",
             "GetAwsBackupStatus",
@@ -22721,14 +22729,15 @@
             "Select",
             "SelectValues",
             "StartAwsBackupJob",
             "StartAwsRestoreJob",
             "TagResource",
             "Unload",
             "UntagResource",
+            "UpdateAccountSettings",
             "UpdateDatabase",
             "UpdateScheduledQuery",
             "UpdateTable",
             "WriteRecords"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
```

### Comparing `iam_actions-1.2.20240429/pyproject.toml` & `iam_actions-1.2.20240430/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240429"
+version = "1.2.20240430"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240429/setup.py` & `iam_actions-1.2.20240430/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240429',
+    'version': '1.2.20240430',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240429/PKG-INFO` & `iam_actions-1.2.20240430/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240429
+Version: 1.2.20240430
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

