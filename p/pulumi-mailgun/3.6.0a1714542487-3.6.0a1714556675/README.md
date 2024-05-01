# Comparing `tmp/pulumi_mailgun-3.6.0a1714542487.tar.gz` & `tmp/pulumi_mailgun-3.6.0a1714556675.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_mailgun-3.6.0a1714542487.tar", last modified: Wed May  1 05:55:55 2024, max compression
+gzip compressed data, was "pulumi_mailgun-3.6.0a1714556675.tar", last modified: Wed May  1 09:48:23 2024, max compression
```

## Comparing `pulumi_mailgun-3.6.0a1714542487.tar` & `pulumi_mailgun-3.6.0a1714556675.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    36352 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    13364 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/domain_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    12904 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/route.py
--rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-01 05:55:55.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-01 05:55:55.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:55:55.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 05:55:55.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 05:55:55.000000 pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-01 05:55:49.000000 pulumi_mailgun-3.6.0a1714542487/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:55:55.963474 pulumi_mailgun-3.6.0a1714542487/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:48:23.061973 pulumi_mailgun-3.6.0a1714556675/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-01 09:48:23.061973 pulumi_mailgun-3.6.0a1714556675/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:48:23.057973 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:48:23.061973 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40741 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13364 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/domain_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14709 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:48:23.061973 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-01 09:48:23.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-01 09:48:23.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:48:23.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 09:48:23.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 09:48:23.000000 pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-01 09:48:16.000000 pulumi_mailgun-3.6.0a1714556675/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 09:48:23.061973 pulumi_mailgun-3.6.0a1714556675/setup.cfg
```

### Comparing `pulumi_mailgun-3.6.0a1714542487/PKG-INFO` & `pulumi_mailgun-3.6.0a1714556675/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mailgun
-Version: 3.6.0a1714542487
+Version: 3.6.0a1714556675
 Summary: A Pulumi package for creating and managing Mailgun resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mailgun
 Keywords: pulumi,mailgun
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mailgun-3.6.0a1714542487/README.md` & `pulumi_mailgun-3.6.0a1714556675/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/__init__.py` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/_inputs.py` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/_utilities.py` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/config/vars.py` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/domain.py` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,38 +12,44 @@
 from ._inputs import *
 
 __all__ = ['DomainArgs', 'Domain']
 
 @pulumi.input_type
 class DomainArgs:
     def __init__(__self__, *,
+                 click_tracking: Optional[pulumi.Input[bool]] = None,
                  dkim_key_size: Optional[pulumi.Input[int]] = None,
                  dkim_selector: Optional[pulumi.Input[str]] = None,
                  force_dkim_authority: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  open_tracking: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  smtp_password: Optional[pulumi.Input[str]] = None,
                  spam_action: Optional[pulumi.Input[str]] = None,
+                 web_scheme: Optional[pulumi.Input[str]] = None,
                  wildcard: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Domain resource.
+        :param pulumi.Input[bool] click_tracking: (Enum: `yes` or `no`) The click tracking settings for the domain. Default: `no`
         :param pulumi.Input[int] dkim_key_size: The length of your domain’s generated DKIM key. Default value is `1024`.
         :param pulumi.Input[str] dkim_selector: The name of your DKIM selector if you want to specify it whereas MailGun will make it's own choice.
         :param pulumi.Input[bool] force_dkim_authority: If set to true, the domain will be the DKIM authority for itself even if the root domain is registered on the same mailgun account. If set to false, the domain will have the same DKIM authority as the root domain registered on the same mailgun account. The default is `false`.
         :param pulumi.Input[str] name: The domain to add to Mailgun
         :param pulumi.Input[bool] open_tracking: (Enum: `yes` or `no`) The open tracking settings for the domain. Default: `no`
         :param pulumi.Input[str] region: The region where domain will be created. Default value is `us`.
         :param pulumi.Input[str] smtp_password: Password for SMTP authentication
         :param pulumi.Input[str] spam_action: `disabled` or `tag` Disable, no spam
                filtering will occur for inbound messages. Tag, messages
                will be tagged with a spam header. Default value is `disabled`.
+        :param pulumi.Input[str] web_scheme: (`http` or `https`) The tracking web scheme. Default: `http`
         :param pulumi.Input[bool] wildcard: Boolean that determines whether
                the domain will accept email for sub-domains.
         """
+        if click_tracking is not None:
+            pulumi.set(__self__, "click_tracking", click_tracking)
         if dkim_key_size is not None:
             pulumi.set(__self__, "dkim_key_size", dkim_key_size)
         if dkim_selector is not None:
             pulumi.set(__self__, "dkim_selector", dkim_selector)
         if force_dkim_authority is not None:
             pulumi.set(__self__, "force_dkim_authority", force_dkim_authority)
         if name is not None:
@@ -52,18 +58,32 @@
             pulumi.set(__self__, "open_tracking", open_tracking)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if smtp_password is not None:
             pulumi.set(__self__, "smtp_password", smtp_password)
         if spam_action is not None:
             pulumi.set(__self__, "spam_action", spam_action)
+        if web_scheme is not None:
+            pulumi.set(__self__, "web_scheme", web_scheme)
         if wildcard is not None:
             pulumi.set(__self__, "wildcard", wildcard)
 
     @property
+    @pulumi.getter(name="clickTracking")
+    def click_tracking(self) -> Optional[pulumi.Input[bool]]:
+        """
+        (Enum: `yes` or `no`) The click tracking settings for the domain. Default: `no`
+        """
+        return pulumi.get(self, "click_tracking")
+
+    @click_tracking.setter
+    def click_tracking(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "click_tracking", value)
+
+    @property
     @pulumi.getter(name="dkimKeySize")
     def dkim_key_size(self) -> Optional[pulumi.Input[int]]:
         """
         The length of your domain’s generated DKIM key. Default value is `1024`.
         """
         return pulumi.get(self, "dkim_key_size")
 
@@ -154,14 +174,26 @@
         return pulumi.get(self, "spam_action")
 
     @spam_action.setter
     def spam_action(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "spam_action", value)
 
     @property
+    @pulumi.getter(name="webScheme")
+    def web_scheme(self) -> Optional[pulumi.Input[str]]:
+        """
+        (`http` or `https`) The tracking web scheme. Default: `http`
+        """
+        return pulumi.get(self, "web_scheme")
+
+    @web_scheme.setter
+    def web_scheme(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "web_scheme", value)
+
+    @property
     @pulumi.getter
     def wildcard(self) -> Optional[pulumi.Input[bool]]:
         """
         Boolean that determines whether
         the domain will accept email for sub-domains.
         """
         return pulumi.get(self, "wildcard")
@@ -170,30 +202,33 @@
     def wildcard(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "wildcard", value)
 
 
 @pulumi.input_type
 class _DomainState:
     def __init__(__self__, *,
+                 click_tracking: Optional[pulumi.Input[bool]] = None,
                  dkim_key_size: Optional[pulumi.Input[int]] = None,
                  dkim_selector: Optional[pulumi.Input[str]] = None,
                  force_dkim_authority: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  open_tracking: Optional[pulumi.Input[bool]] = None,
                  receiving_records: Optional[pulumi.Input[Sequence[pulumi.Input['DomainReceivingRecordArgs']]]] = None,
                  receiving_records_sets: Optional[pulumi.Input[Sequence[pulumi.Input['DomainReceivingRecordsSetArgs']]]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  sending_records: Optional[pulumi.Input[Sequence[pulumi.Input['DomainSendingRecordArgs']]]] = None,
                  sending_records_sets: Optional[pulumi.Input[Sequence[pulumi.Input['DomainSendingRecordsSetArgs']]]] = None,
                  smtp_login: Optional[pulumi.Input[str]] = None,
                  smtp_password: Optional[pulumi.Input[str]] = None,
                  spam_action: Optional[pulumi.Input[str]] = None,
+                 web_scheme: Optional[pulumi.Input[str]] = None,
                  wildcard: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Domain resources.
+        :param pulumi.Input[bool] click_tracking: (Enum: `yes` or `no`) The click tracking settings for the domain. Default: `no`
         :param pulumi.Input[int] dkim_key_size: The length of your domain’s generated DKIM key. Default value is `1024`.
         :param pulumi.Input[str] dkim_selector: The name of your DKIM selector if you want to specify it whereas MailGun will make it's own choice.
         :param pulumi.Input[bool] force_dkim_authority: If set to true, the domain will be the DKIM authority for itself even if the root domain is registered on the same mailgun account. If set to false, the domain will have the same DKIM authority as the root domain registered on the same mailgun account. The default is `false`.
         :param pulumi.Input[str] name: The domain to add to Mailgun
         :param pulumi.Input[bool] open_tracking: (Enum: `yes` or `no`) The open tracking settings for the domain. Default: `no`
         :param pulumi.Input[Sequence[pulumi.Input['DomainReceivingRecordArgs']]] receiving_records: A list of DNS records for receiving validation.  **Deprecated** Use `receiving_records_set` instead.
         :param pulumi.Input[Sequence[pulumi.Input['DomainReceivingRecordsSetArgs']]] receiving_records_sets: A set of DNS records for receiving validation.
@@ -201,17 +236,20 @@
         :param pulumi.Input[Sequence[pulumi.Input['DomainSendingRecordArgs']]] sending_records: A list of DNS records for sending validation. **Deprecated** Use `sending_records_set` instead.
         :param pulumi.Input[Sequence[pulumi.Input['DomainSendingRecordsSetArgs']]] sending_records_sets: A set of DNS records for sending validation.
         :param pulumi.Input[str] smtp_login: The login email for the SMTP server.
         :param pulumi.Input[str] smtp_password: Password for SMTP authentication
         :param pulumi.Input[str] spam_action: `disabled` or `tag` Disable, no spam
                filtering will occur for inbound messages. Tag, messages
                will be tagged with a spam header. Default value is `disabled`.
+        :param pulumi.Input[str] web_scheme: (`http` or `https`) The tracking web scheme. Default: `http`
         :param pulumi.Input[bool] wildcard: Boolean that determines whether
                the domain will accept email for sub-domains.
         """
+        if click_tracking is not None:
+            pulumi.set(__self__, "click_tracking", click_tracking)
         if dkim_key_size is not None:
             pulumi.set(__self__, "dkim_key_size", dkim_key_size)
         if dkim_selector is not None:
             pulumi.set(__self__, "dkim_selector", dkim_selector)
         if force_dkim_authority is not None:
             pulumi.set(__self__, "force_dkim_authority", force_dkim_authority)
         if name is not None:
@@ -236,18 +274,32 @@
             pulumi.set(__self__, "sending_records_sets", sending_records_sets)
         if smtp_login is not None:
             pulumi.set(__self__, "smtp_login", smtp_login)
         if smtp_password is not None:
             pulumi.set(__self__, "smtp_password", smtp_password)
         if spam_action is not None:
             pulumi.set(__self__, "spam_action", spam_action)
+        if web_scheme is not None:
+            pulumi.set(__self__, "web_scheme", web_scheme)
         if wildcard is not None:
             pulumi.set(__self__, "wildcard", wildcard)
 
     @property
+    @pulumi.getter(name="clickTracking")
+    def click_tracking(self) -> Optional[pulumi.Input[bool]]:
+        """
+        (Enum: `yes` or `no`) The click tracking settings for the domain. Default: `no`
+        """
+        return pulumi.get(self, "click_tracking")
+
+    @click_tracking.setter
+    def click_tracking(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "click_tracking", value)
+
+    @property
     @pulumi.getter(name="dkimKeySize")
     def dkim_key_size(self) -> Optional[pulumi.Input[int]]:
         """
         The length of your domain’s generated DKIM key. Default value is `1024`.
         """
         return pulumi.get(self, "dkim_key_size")
 
@@ -404,14 +456,26 @@
         return pulumi.get(self, "spam_action")
 
     @spam_action.setter
     def spam_action(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "spam_action", value)
 
     @property
+    @pulumi.getter(name="webScheme")
+    def web_scheme(self) -> Optional[pulumi.Input[str]]:
+        """
+        (`http` or `https`) The tracking web scheme. Default: `http`
+        """
+        return pulumi.get(self, "web_scheme")
+
+    @web_scheme.setter
+    def web_scheme(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "web_scheme", value)
+
+    @property
     @pulumi.getter
     def wildcard(self) -> Optional[pulumi.Input[bool]]:
         """
         Boolean that determines whether
         the domain will accept email for sub-domains.
         """
         return pulumi.get(self, "wildcard")
@@ -422,22 +486,24 @@
 
 
 class Domain(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 click_tracking: Optional[pulumi.Input[bool]] = None,
                  dkim_key_size: Optional[pulumi.Input[int]] = None,
                  dkim_selector: Optional[pulumi.Input[str]] = None,
                  force_dkim_authority: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  open_tracking: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  smtp_password: Optional[pulumi.Input[str]] = None,
                  spam_action: Optional[pulumi.Input[str]] = None,
+                 web_scheme: Optional[pulumi.Input[str]] = None,
                  wildcard: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Provides a Mailgun App resource. This can be used to
         create and manage applications on Mailgun.
 
         After DNS records are set, domain verification should be triggered manually using [PUT /domains/\\<domain\\>/verify](https://documentation.mailgun.com/en/latest/api-domains.html#domains)
@@ -465,24 +531,26 @@
 
         ```sh
         $ pulumi import mailgun:index/domain:Domain test us:example.domain.com
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] click_tracking: (Enum: `yes` or `no`) The click tracking settings for the domain. Default: `no`
         :param pulumi.Input[int] dkim_key_size: The length of your domain’s generated DKIM key. Default value is `1024`.
         :param pulumi.Input[str] dkim_selector: The name of your DKIM selector if you want to specify it whereas MailGun will make it's own choice.
         :param pulumi.Input[bool] force_dkim_authority: If set to true, the domain will be the DKIM authority for itself even if the root domain is registered on the same mailgun account. If set to false, the domain will have the same DKIM authority as the root domain registered on the same mailgun account. The default is `false`.
         :param pulumi.Input[str] name: The domain to add to Mailgun
         :param pulumi.Input[bool] open_tracking: (Enum: `yes` or `no`) The open tracking settings for the domain. Default: `no`
         :param pulumi.Input[str] region: The region where domain will be created. Default value is `us`.
         :param pulumi.Input[str] smtp_password: Password for SMTP authentication
         :param pulumi.Input[str] spam_action: `disabled` or `tag` Disable, no spam
                filtering will occur for inbound messages. Tag, messages
                will be tagged with a spam header. Default value is `disabled`.
+        :param pulumi.Input[str] web_scheme: (`http` or `https`) The tracking web scheme. Default: `http`
         :param pulumi.Input[bool] wildcard: Boolean that determines whether
                the domain will accept email for sub-domains.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -530,40 +598,44 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 click_tracking: Optional[pulumi.Input[bool]] = None,
                  dkim_key_size: Optional[pulumi.Input[int]] = None,
                  dkim_selector: Optional[pulumi.Input[str]] = None,
                  force_dkim_authority: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  open_tracking: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  smtp_password: Optional[pulumi.Input[str]] = None,
                  spam_action: Optional[pulumi.Input[str]] = None,
+                 web_scheme: Optional[pulumi.Input[str]] = None,
                  wildcard: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DomainArgs.__new__(DomainArgs)
 
+            __props__.__dict__["click_tracking"] = click_tracking
             __props__.__dict__["dkim_key_size"] = dkim_key_size
             __props__.__dict__["dkim_selector"] = dkim_selector
             __props__.__dict__["force_dkim_authority"] = force_dkim_authority
             __props__.__dict__["name"] = name
             __props__.__dict__["open_tracking"] = open_tracking
             __props__.__dict__["region"] = region
             __props__.__dict__["smtp_password"] = None if smtp_password is None else pulumi.Output.secret(smtp_password)
             __props__.__dict__["spam_action"] = spam_action
+            __props__.__dict__["web_scheme"] = web_scheme
             __props__.__dict__["wildcard"] = wildcard
             __props__.__dict__["receiving_records"] = None
             __props__.__dict__["receiving_records_sets"] = None
             __props__.__dict__["sending_records"] = None
             __props__.__dict__["sending_records_sets"] = None
             __props__.__dict__["smtp_login"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["smtpPassword"])
@@ -574,35 +646,38 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            click_tracking: Optional[pulumi.Input[bool]] = None,
             dkim_key_size: Optional[pulumi.Input[int]] = None,
             dkim_selector: Optional[pulumi.Input[str]] = None,
             force_dkim_authority: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             open_tracking: Optional[pulumi.Input[bool]] = None,
             receiving_records: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DomainReceivingRecordArgs']]]]] = None,
             receiving_records_sets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DomainReceivingRecordsSetArgs']]]]] = None,
             region: Optional[pulumi.Input[str]] = None,
             sending_records: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DomainSendingRecordArgs']]]]] = None,
             sending_records_sets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DomainSendingRecordsSetArgs']]]]] = None,
             smtp_login: Optional[pulumi.Input[str]] = None,
             smtp_password: Optional[pulumi.Input[str]] = None,
             spam_action: Optional[pulumi.Input[str]] = None,
+            web_scheme: Optional[pulumi.Input[str]] = None,
             wildcard: Optional[pulumi.Input[bool]] = None) -> 'Domain':
         """
         Get an existing Domain resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] click_tracking: (Enum: `yes` or `no`) The click tracking settings for the domain. Default: `no`
         :param pulumi.Input[int] dkim_key_size: The length of your domain’s generated DKIM key. Default value is `1024`.
         :param pulumi.Input[str] dkim_selector: The name of your DKIM selector if you want to specify it whereas MailGun will make it's own choice.
         :param pulumi.Input[bool] force_dkim_authority: If set to true, the domain will be the DKIM authority for itself even if the root domain is registered on the same mailgun account. If set to false, the domain will have the same DKIM authority as the root domain registered on the same mailgun account. The default is `false`.
         :param pulumi.Input[str] name: The domain to add to Mailgun
         :param pulumi.Input[bool] open_tracking: (Enum: `yes` or `no`) The open tracking settings for the domain. Default: `no`
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DomainReceivingRecordArgs']]]] receiving_records: A list of DNS records for receiving validation.  **Deprecated** Use `receiving_records_set` instead.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DomainReceivingRecordsSetArgs']]]] receiving_records_sets: A set of DNS records for receiving validation.
@@ -610,38 +685,49 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DomainSendingRecordArgs']]]] sending_records: A list of DNS records for sending validation. **Deprecated** Use `sending_records_set` instead.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DomainSendingRecordsSetArgs']]]] sending_records_sets: A set of DNS records for sending validation.
         :param pulumi.Input[str] smtp_login: The login email for the SMTP server.
         :param pulumi.Input[str] smtp_password: Password for SMTP authentication
         :param pulumi.Input[str] spam_action: `disabled` or `tag` Disable, no spam
                filtering will occur for inbound messages. Tag, messages
                will be tagged with a spam header. Default value is `disabled`.
+        :param pulumi.Input[str] web_scheme: (`http` or `https`) The tracking web scheme. Default: `http`
         :param pulumi.Input[bool] wildcard: Boolean that determines whether
                the domain will accept email for sub-domains.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DomainState.__new__(_DomainState)
 
+        __props__.__dict__["click_tracking"] = click_tracking
         __props__.__dict__["dkim_key_size"] = dkim_key_size
         __props__.__dict__["dkim_selector"] = dkim_selector
         __props__.__dict__["force_dkim_authority"] = force_dkim_authority
         __props__.__dict__["name"] = name
         __props__.__dict__["open_tracking"] = open_tracking
         __props__.__dict__["receiving_records"] = receiving_records
         __props__.__dict__["receiving_records_sets"] = receiving_records_sets
         __props__.__dict__["region"] = region
         __props__.__dict__["sending_records"] = sending_records
         __props__.__dict__["sending_records_sets"] = sending_records_sets
         __props__.__dict__["smtp_login"] = smtp_login
         __props__.__dict__["smtp_password"] = smtp_password
         __props__.__dict__["spam_action"] = spam_action
+        __props__.__dict__["web_scheme"] = web_scheme
         __props__.__dict__["wildcard"] = wildcard
         return Domain(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="clickTracking")
+    def click_tracking(self) -> pulumi.Output[Optional[bool]]:
+        """
+        (Enum: `yes` or `no`) The click tracking settings for the domain. Default: `no`
+        """
+        return pulumi.get(self, "click_tracking")
+
+    @property
     @pulumi.getter(name="dkimKeySize")
     def dkim_key_size(self) -> pulumi.Output[Optional[int]]:
         """
         The length of your domain’s generated DKIM key. Default value is `1024`.
         """
         return pulumi.get(self, "dkim_key_size")
 
@@ -746,14 +832,22 @@
         `disabled` or `tag` Disable, no spam
         filtering will occur for inbound messages. Tag, messages
         will be tagged with a spam header. Default value is `disabled`.
         """
         return pulumi.get(self, "spam_action")
 
     @property
+    @pulumi.getter(name="webScheme")
+    def web_scheme(self) -> pulumi.Output[Optional[str]]:
+        """
+        (`http` or `https`) The tracking web scheme. Default: `http`
+        """
+        return pulumi.get(self, "web_scheme")
+
+    @property
     @pulumi.getter
     def wildcard(self) -> pulumi.Output[Optional[bool]]:
         """
         Boolean that determines whether
         the domain will accept email for sub-domains.
         """
         return pulumi.get(self, "wildcard")
```

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/domain_credential.py` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/domain_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/get_domain.py` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/get_domain.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 ]
 
 @pulumi.output_type
 class GetDomainResult:
     """
     A collection of values returned by getDomain.
     """
-    def __init__(__self__, dkim_key_size=None, dkim_selector=None, force_dkim_authority=None, id=None, name=None, open_tracking=None, receiving_records=None, receiving_records_sets=None, region=None, sending_records=None, sending_records_sets=None, smtp_login=None, smtp_password=None, spam_action=None, wildcard=None):
+    def __init__(__self__, click_tracking=None, dkim_key_size=None, dkim_selector=None, force_dkim_authority=None, id=None, name=None, open_tracking=None, receiving_records=None, receiving_records_sets=None, region=None, sending_records=None, sending_records_sets=None, smtp_login=None, smtp_password=None, spam_action=None, web_scheme=None, wildcard=None):
+        if click_tracking and not isinstance(click_tracking, bool):
+            raise TypeError("Expected argument 'click_tracking' to be a bool")
+        pulumi.set(__self__, "click_tracking", click_tracking)
         if dkim_key_size and not isinstance(dkim_key_size, int):
             raise TypeError("Expected argument 'dkim_key_size' to be a int")
         pulumi.set(__self__, "dkim_key_size", dkim_key_size)
         if dkim_selector and not isinstance(dkim_selector, str):
             raise TypeError("Expected argument 'dkim_selector' to be a str")
         pulumi.set(__self__, "dkim_selector", dkim_selector)
         if force_dkim_authority and not isinstance(force_dkim_authority, bool):
@@ -61,19 +64,30 @@
         pulumi.set(__self__, "smtp_login", smtp_login)
         if smtp_password and not isinstance(smtp_password, str):
             raise TypeError("Expected argument 'smtp_password' to be a str")
         pulumi.set(__self__, "smtp_password", smtp_password)
         if spam_action and not isinstance(spam_action, str):
             raise TypeError("Expected argument 'spam_action' to be a str")
         pulumi.set(__self__, "spam_action", spam_action)
+        if web_scheme and not isinstance(web_scheme, str):
+            raise TypeError("Expected argument 'web_scheme' to be a str")
+        pulumi.set(__self__, "web_scheme", web_scheme)
         if wildcard and not isinstance(wildcard, bool):
             raise TypeError("Expected argument 'wildcard' to be a bool")
         pulumi.set(__self__, "wildcard", wildcard)
 
     @property
+    @pulumi.getter(name="clickTracking")
+    def click_tracking(self) -> Optional[bool]:
+        """
+        The click tracking setting.
+        """
+        return pulumi.get(self, "click_tracking")
+
+    @property
     @pulumi.getter(name="dkimKeySize")
     def dkim_key_size(self) -> Optional[int]:
         return pulumi.get(self, "dkim_key_size")
 
     @property
     @pulumi.getter(name="dkimSelector")
     def dkim_selector(self) -> Optional[str]:
@@ -99,14 +113,17 @@
         The name of the record.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="openTracking")
     def open_tracking(self) -> Optional[bool]:
+        """
+        The open tracking setting.
+        """
         return pulumi.get(self, "open_tracking")
 
     @property
     @pulumi.getter(name="receivingRecords")
     def receiving_records(self) -> Sequence['outputs.GetDomainReceivingRecordResult']:
         """
         A list of DNS records for receiving validation.
@@ -163,53 +180,65 @@
     def spam_action(self) -> Optional[str]:
         """
         The spam filtering setting.
         """
         return pulumi.get(self, "spam_action")
 
     @property
+    @pulumi.getter(name="webScheme")
+    def web_scheme(self) -> Optional[str]:
+        """
+        The tracking web scheme.
+        """
+        return pulumi.get(self, "web_scheme")
+
+    @property
     @pulumi.getter
     def wildcard(self) -> Optional[bool]:
         """
         Whether or not the domain will accept email for sub-domains.
         """
         return pulumi.get(self, "wildcard")
 
 
 class AwaitableGetDomainResult(GetDomainResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetDomainResult(
+            click_tracking=self.click_tracking,
             dkim_key_size=self.dkim_key_size,
             dkim_selector=self.dkim_selector,
             force_dkim_authority=self.force_dkim_authority,
             id=self.id,
             name=self.name,
             open_tracking=self.open_tracking,
             receiving_records=self.receiving_records,
             receiving_records_sets=self.receiving_records_sets,
             region=self.region,
             sending_records=self.sending_records,
             sending_records_sets=self.sending_records_sets,
             smtp_login=self.smtp_login,
             smtp_password=self.smtp_password,
             spam_action=self.spam_action,
+            web_scheme=self.web_scheme,
             wildcard=self.wildcard)
 
 
-def get_domain(dkim_key_size: Optional[int] = None,
+def get_domain(click_tracking: Optional[bool] = None,
+               dkim_key_size: Optional[int] = None,
                dkim_selector: Optional[str] = None,
                force_dkim_authority: Optional[bool] = None,
                name: Optional[str] = None,
                open_tracking: Optional[bool] = None,
                region: Optional[str] = None,
                smtp_password: Optional[str] = None,
                spam_action: Optional[str] = None,
+               web_scheme: Optional[str] = None,
                wildcard: Optional[bool] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDomainResult:
     """
     `Domain` provides details about a Mailgun domain.
 
     ## Example Usage
 
@@ -227,60 +256,69 @@
         records=[
             f{domain.receiving_records[0].priority} {domain.receiving_records[0].value}.,
             f{domain.receiving_records[1].priority} {domain.receiving_records[1].value}.,
         ])
     ```
 
 
+    :param bool click_tracking: The click tracking setting.
     :param str name: The name of the domain.
+    :param bool open_tracking: The open tracking setting.
     :param str region: The region where domain will be created. Default value is `us`.
     :param str smtp_password: The password to the SMTP server.
     :param str spam_action: The spam filtering setting.
+    :param str web_scheme: The tracking web scheme.
     :param bool wildcard: Whether or not the domain will accept email for sub-domains.
     """
     __args__ = dict()
+    __args__['clickTracking'] = click_tracking
     __args__['dkimKeySize'] = dkim_key_size
     __args__['dkimSelector'] = dkim_selector
     __args__['forceDkimAuthority'] = force_dkim_authority
     __args__['name'] = name
     __args__['openTracking'] = open_tracking
     __args__['region'] = region
     __args__['smtpPassword'] = smtp_password
     __args__['spamAction'] = spam_action
+    __args__['webScheme'] = web_scheme
     __args__['wildcard'] = wildcard
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('mailgun:index/getDomain:getDomain', __args__, opts=opts, typ=GetDomainResult).value
 
     return AwaitableGetDomainResult(
+        click_tracking=pulumi.get(__ret__, 'click_tracking'),
         dkim_key_size=pulumi.get(__ret__, 'dkim_key_size'),
         dkim_selector=pulumi.get(__ret__, 'dkim_selector'),
         force_dkim_authority=pulumi.get(__ret__, 'force_dkim_authority'),
         id=pulumi.get(__ret__, 'id'),
         name=pulumi.get(__ret__, 'name'),
         open_tracking=pulumi.get(__ret__, 'open_tracking'),
         receiving_records=pulumi.get(__ret__, 'receiving_records'),
         receiving_records_sets=pulumi.get(__ret__, 'receiving_records_sets'),
         region=pulumi.get(__ret__, 'region'),
         sending_records=pulumi.get(__ret__, 'sending_records'),
         sending_records_sets=pulumi.get(__ret__, 'sending_records_sets'),
         smtp_login=pulumi.get(__ret__, 'smtp_login'),
         smtp_password=pulumi.get(__ret__, 'smtp_password'),
         spam_action=pulumi.get(__ret__, 'spam_action'),
+        web_scheme=pulumi.get(__ret__, 'web_scheme'),
         wildcard=pulumi.get(__ret__, 'wildcard'))
 
 
 @_utilities.lift_output_func(get_domain)
-def get_domain_output(dkim_key_size: Optional[pulumi.Input[Optional[int]]] = None,
+def get_domain_output(click_tracking: Optional[pulumi.Input[Optional[bool]]] = None,
+                      dkim_key_size: Optional[pulumi.Input[Optional[int]]] = None,
                       dkim_selector: Optional[pulumi.Input[Optional[str]]] = None,
                       force_dkim_authority: Optional[pulumi.Input[Optional[bool]]] = None,
                       name: Optional[pulumi.Input[str]] = None,
                       open_tracking: Optional[pulumi.Input[Optional[bool]]] = None,
                       region: Optional[pulumi.Input[Optional[str]]] = None,
                       smtp_password: Optional[pulumi.Input[Optional[str]]] = None,
                       spam_action: Optional[pulumi.Input[Optional[str]]] = None,
+                      web_scheme: Optional[pulumi.Input[Optional[str]]] = None,
                       wildcard: Optional[pulumi.Input[Optional[bool]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainResult]:
     """
     `Domain` provides details about a Mailgun domain.
 
     ## Example Usage
 
@@ -298,14 +336,17 @@
         records=[
             f{domain.receiving_records[0].priority} {domain.receiving_records[0].value}.,
             f{domain.receiving_records[1].priority} {domain.receiving_records[1].value}.,
         ])
     ```
 
 
+    :param bool click_tracking: The click tracking setting.
     :param str name: The name of the domain.
+    :param bool open_tracking: The open tracking setting.
     :param str region: The region where domain will be created. Default value is `us`.
     :param str smtp_password: The password to the SMTP server.
     :param str spam_action: The spam filtering setting.
+    :param str web_scheme: The tracking web scheme.
     :param bool wildcard: Whether or not the domain will accept email for sub-domains.
     """
     ...
```

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/outputs.py` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/provider.py` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/route.py` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/route.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun/webhook.py` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/PKG-INFO` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mailgun
-Version: 3.6.0a1714542487
+Version: 3.6.0a1714556675
 Summary: A Pulumi package for creating and managing Mailgun resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mailgun
 Keywords: pulumi,mailgun
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mailgun-3.6.0a1714542487/pulumi_mailgun.egg-info/SOURCES.txt` & `pulumi_mailgun-3.6.0a1714556675/pulumi_mailgun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1714542487/pyproject.toml` & `pulumi_mailgun-3.6.0a1714556675/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_mailgun"
   description = "A Pulumi package for creating and managing Mailgun resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "mailgun"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.6.0a1714542487"
+  version = "3.6.0a1714556675"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-mailgun"
 
 [build-system]
```

