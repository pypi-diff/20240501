# Comparing `tmp/roadtx-1.7.0.tar.gz` & `tmp/roadtx-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadtx-1.7.0.tar", last modified: Tue Dec  5 15:25:37 2023, max compression
+gzip compressed data, was "roadtx-1.7.1.tar", last modified: Mon Apr 29 12:05:55 2024, max compression
```

## Comparing `roadtx-1.7.0.tar` & `roadtx-1.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 15:25:37.981400 roadtx-1.7.0/
--rw-r--r--   0 vsts      (1001) docker     (127)      749 2023-12-05 15:25:37.981400 roadtx-1.7.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 15:25:37.977400 roadtx-1.7.0/roadtools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 15:25:37.981400 roadtx-1.7.0/roadtools/roadtx/
--rw-r--r--   0 vsts      (1001) docker     (127)    17458 2023-12-05 15:24:06.000000 roadtx-1.7.0/roadtools/roadtx/federation.py
--rw-r--r--   0 vsts      (1001) docker     (127)   208284 2023-12-05 15:24:06.000000 roadtx-1.7.0/roadtools/roadtx/firstpartyscopes.json
--rw-r--r--   0 vsts      (1001) docker     (127)     7865 2023-12-05 15:24:06.000000 roadtx-1.7.0/roadtools/roadtx/keepass.py
--rw-r--r--   0 vsts      (1001) docker     (127)    68498 2023-12-05 15:24:06.000000 roadtx-1.7.0/roadtools/roadtx/main.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18595 2023-12-05 15:24:06.000000 roadtx-1.7.0/roadtools/roadtx/selenium.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-12-05 15:25:37.981400 roadtx-1.7.0/roadtx.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      749 2023-12-05 15:25:37.000000 roadtx-1.7.0/roadtx.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      371 2023-12-05 15:25:37.000000 roadtx-1.7.0/roadtx.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-05 15:25:37.000000 roadtx-1.7.0/roadtx.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2023-12-05 15:25:37.000000 roadtx-1.7.0/roadtx.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-12-05 15:25:34.000000 roadtx-1.7.0/roadtx.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       74 2023-12-05 15:25:37.000000 roadtx-1.7.0/roadtx.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       10 2023-12-05 15:25:37.000000 roadtx-1.7.0/roadtx.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2023-12-05 15:25:37.981400 roadtx-1.7.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1130 2023-12-05 15:24:06.000000 roadtx-1.7.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 12:05:55.526741 roadtx-1.7.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)      778 2024-04-29 12:05:55.526741 roadtx-1.7.1/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 12:05:55.518741 roadtx-1.7.1/roadtools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 12:05:55.522741 roadtx-1.7.1/roadtools/roadtx/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17458 2024-04-29 12:04:09.000000 roadtx-1.7.1/roadtools/roadtx/federation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   208284 2024-04-29 12:04:09.000000 roadtx-1.7.1/roadtools/roadtx/firstpartyscopes.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     7865 2024-04-29 12:04:09.000000 roadtx-1.7.1/roadtools/roadtx/keepass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    72108 2024-04-29 12:04:09.000000 roadtx-1.7.1/roadtools/roadtx/main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18740 2024-04-29 12:04:09.000000 roadtx-1.7.1/roadtools/roadtx/selenium.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 12:05:55.522741 roadtx-1.7.1/roadtx.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      778 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      371 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-29 12:05:52.000000 roadtx-1.7.1/roadtx.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       10 2024-04-29 12:05:55.000000 roadtx-1.7.1/roadtx.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-29 12:05:55.526741 roadtx-1.7.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1157 2024-04-29 12:04:09.000000 roadtx-1.7.1/setup.py
```

### Comparing `roadtx-1.7.0/roadtools/roadtx/federation.py` & `roadtx-1.7.1/roadtools/roadtx/federation.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.7.0/roadtools/roadtx/firstpartyscopes.json` & `roadtx-1.7.1/roadtools/roadtx/firstpartyscopes.json`

 * *Files identical despite different names*

### Comparing `roadtx-1.7.0/roadtools/roadtx/keepass.py` & `roadtx-1.7.1/roadtools/roadtx/keepass.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.7.0/roadtools/roadtx/main.py` & `roadtx-1.7.1/roadtools/roadtx/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import sys
 import os
 import json
 import codecs
 import binascii
 import base64
+import time
 from urllib.parse import quote_plus
 from roadtools.roadlib.auth import Authentication, get_data
 from roadtools.roadlib.constants import WELLKNOWN_CLIENTS, WELLKNOWN_RESOURCES, WELLKNOWN_USER_AGENTS
 from roadtools.roadlib.deviceauth import DeviceAuthentication
 from roadtools.roadtx.selenium import SeleniumAuthentication
 from roadtools.roadtx.federation import EncryptedPFX, SAMLSigner, encode_object_guid
 import pyotp
@@ -28,19 +29,19 @@
     auth = Authentication()
     auth_parser = subparsers.add_parser('gettokens', aliases=['auth','gettoken'], help='Authenticate to Azure AD and get access/refresh tokens. Supports various authentication methods.')
     auth.get_sub_argparse(auth_parser, for_rr=False)
 
     # Construct device module
     device_parser = subparsers.add_parser('device', help='Register or join devices to Azure AD')
     device_parser.add_argument('-a',
-                                '--action',
-                                action='store',
-                                choices=['join','register','delete'],
-                                default='join',
-                                help='Action to perform (default: join)')
+                               '--action',
+                               action='store',
+                               choices=['join','register','delete'],
+                               default='join',
+                               help='Action to perform (default: join)')
     device_parser.add_argument('-c', '--cert-pem', action='store', metavar='file', help='Certificate file to save device cert to (default: <devicename>.pem)')
     device_parser.add_argument('-k', '--key-pem', action='store', metavar='file', help='Private key file for certificate (default: <devicename>.key)')
     device_parser.add_argument('-n', '--name', action='store', help='Device display name (default: DESKTOP-<RANDOM>)')
     device_parser.add_argument('--access-token', action='store', help='Access token for device registration service. If not specified, taken from .roadtools_auth')
     device_parser.add_argument('--device-type', action='store', help='Device OS type (default: Windows)')
     device_parser.add_argument('--os-version', action='store', help='Device OS version (default: 10.0.19041.928)')
     device_parser.add_argument('--deviceticket', action='store', help='Device MSA ticket to match with existing device')
@@ -120,14 +121,21 @@
     prtauth_parser.add_argument('--tokenfile',
                                 action='store',
                                 help='File to store the credentials (default: .roadtools_auth)',
                                 default='.roadtools_auth')
     prtauth_parser.add_argument('--tokens-stdout',
                                 action='store_true',
                                 help='Do not store tokens on disk, pipe to stdout instead')
+    prtauth_parser.add_argument('-ua', '--user-agent', action='store',
+                                help='Custom user agent to use. Default: Python requests user agent')
+    prtauth_parser.add_argument('-t',
+                                '--tenant',
+                                action='store',
+                                help='Tenant ID or domain to auth to')
+
 
     # Application auth
     # appauth_parser = subparsers.add_parser('appauth', help='Authenticate as an application')
     # helptext = 'Client ID (application ID) to use when authenticating.'
     # appauth_parser.add_argument('-c',
     #                             '--client',
     #                             action='store',
@@ -159,14 +167,18 @@
                                  default='1b730954-1685-4b74-9bfd-dac224a7b894')
     codeauth_parser.add_argument('-p', '--password', action='store', metavar='PASSWORD', help='Password secret of the appliction if not a public app')
     codeauth_parser.add_argument('-r',
                                  '--resource',
                                  action='store',
                                  help='Resource to authenticate to. Either a full URL or alias (list with roadtx listaliases)',
                                  default='https://graph.windows.net')
+    codeauth_parser.add_argument('-s',
+                                 '--scope',
+                                 action='store',
+                                 help='Scope to use. Will automatically switch to v2.0 auth endpoint if specified. If unsure use -r instead.')
     codeauth_parser.add_argument('-ru', '--redirect-url', action='store', metavar='URL',
                                  help='Redirect URL used when authenticating (default: https://login.microsoftonline.com/common/oauth2/nativeclient)',
                                  default="https://login.microsoftonline.com/common/oauth2/nativeclient")
     codeauth_parser.add_argument('-t',
                                  '--tenant',
                                  action='store',
                                  help='Tenant ID or domain to auth to')
@@ -471,14 +483,17 @@
     injauth_parser.add_argument('-f', '--prt-file', default="roadtx.prt", action='store', metavar='FILE', help='PRT storage file (default: roadtx.prt)')
     injauth_parser.add_argument('--prt',
                                 action='store',
                                 help='Primary Refresh Token')
     injauth_parser.add_argument('--prt-sessionkey',
                                 action='store',
                                 help='Primary Refresh Token session key (as hex key)')
+    injauth_parser.add_argument('--prt-cookie',
+                                action='store',
+                                help='Primary Refresh Token cookie from ROADtoken (JWT)')
     injauth_parser.add_argument('--tokenfile',
                                 action='store',
                                 help='File to store the credentials (default: .roadtools_auth)',
                                 default='.roadtools_auth')
     injauth_parser.add_argument('--tokens-stdout',
                                 action='store_true',
                                 help='Do not store tokens on disk, pipe to stdout instead')
@@ -529,21 +544,30 @@
     samltoken_parser.add_argument('--pfx-base64', action='store', metavar='BASE64', help='PFX file as base64 string')
     samltoken_parser.add_argument('-i', '--issuer', action='store', required=True, help='Token issuer, must match the federated domain name (without http/https, example: federated.mycompany.com)')
     samltoken_parser.add_argument('-u', '--unique-id', action='store', help='Unique ID of user to spoof (immutableId in roadrecon)')
     samltoken_parser.add_argument('-g', '--guid', action='store', help='GUID of user to spoof (from AD), if not specifying the unique id')
     samltoken_parser.add_argument('-m', '--mfa', action='store_true', help='Include MFA claim in token')
     samltoken_parser.add_argument('--upn', action='store', required=True, help='userPrincipalName of user to spoof')
 
+    # PRT cookie creations
+    prtcookie_parser = subparsers.add_parser('prtcookie', help='Create a PRT cookie from a PRT for external usage')
+    prtcookie_parser.add_argument('-f', '--prt-file', default="roadtx.prt", action='store', metavar='FILE', help='PRT storage file (default: roadtx.prt)')
+    prtcookie_parser.add_argument('--prt',
+                                  action='store',
+                                  help='Primary Refresh Token')
+    prtcookie_parser.add_argument('--prt-sessionkey',
+                                  action='store',
+                                  help='Primary Refresh Token session key (as hex key)')
 
     if len(sys.argv) < 2:
         parser.print_help()
         sys.exit(1)
         return
 
-    deviceauth = DeviceAuthentication()
+    deviceauth = DeviceAuthentication(auth)
     args = parser.parse_args()
     seleniumproxy = None
 
     if args.proxy:
         auth.proxies = deviceauth.proxies = {
             'https': f'http://{args.proxy}'
         }
@@ -637,14 +661,17 @@
             else:
                 print('You must either supply a PRT and session key on the command line or a file that contains them')
                 return
             print("Renewing PRT")
             prtdata = deviceauth.renew_prt()
             deviceauth.saveprt(prtdata, args.prt_file)
     elif args.command == 'prtauth':
+        auth.set_user_agent(args.user_agent)
+        if args.tenant:
+            auth.tenant = args.tenant
         if args.prt and args.prt_sessionkey:
             deviceauth.setprt(args.prt, args.prt_sessionkey)
         elif args.prt_file and deviceauth.loadprt(args.prt_file):
             pass
         else:
             print('You must either supply a PRT and session key on the command line or a file that contains them')
             return
@@ -691,15 +718,20 @@
                 print('Decrypted data (hex)')
                 print(binascii.hexlify(data))
 
     elif args.command == 'codeauth':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
         auth.tenant = args.tenant
-        auth.authenticate_with_code_native(args.code, args.redirect_url, client_secret=args.password)
+        if args.scope:
+            # Switch to identity platform v2 and use scope instead of resource
+            auth.scope = args.scope
+            auth.authenticate_with_code_native_v2(args.code, args.redirect_url, client_secret=args.password)
+        else:
+            auth.authenticate_with_code_native(args.code, args.redirect_url, client_secret=args.password)
         auth.outfile = args.tokenfile
         auth.save_tokens(args)
     elif args.command == 'desktopsso':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
         auth.set_user_agent(args.user_agent)
         auth.tenant = args.tenant
@@ -773,15 +805,15 @@
         if args.auth_url:
             url = args.auth_url
         else:
             url = auth.build_auth_url(args.redirect_url, 'code', args.scope)
         service = selauth.get_service(args.driver_path)
         if not service:
             return
-        selauth.driver = selauth.get_webdriver(service)
+        selauth.driver = selauth.get_webdriver(service, intercept=custom_ua)
         if custom_ua:
             result = selauth.selenium_login_with_custom_useragent(url, args.username, password, otpseed, keep=args.keep_open, capture=args.capture_code, federated=args.federated, devicecode=args.device_code)
         else:
             result = selauth.selenium_login(url, args.username, password, otpseed, keep=args.keep_open, capture=args.capture_code, federated=args.federated, devicecode=args.device_code)
         if args.capture_code:
             if result:
                 print(f'Captured auth code: {result}')
@@ -802,35 +834,50 @@
         else:
             print('You must either supply a PRT and session key on the command line or a file that contains them')
             return
         selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url, proxy=seleniumproxy)
         if args.auth_url:
             url = args.auth_url
         else:
+            if not args.tokens_stdout:
+                if args.scope:
+                    print(f'Running in token request mode - Requesting token with scope {auth.scope}\nIf you want a browser window instead, use the -url parameter to start browsing.')
+                else:
+                    print(f'Running in token request mode - Requesting token for {auth.resource_uri}\nIf you want a browser window instead, use the -url parameter to start browsing.')
             url = auth.build_auth_url(args.redirect_url, 'code', args.scope)
         service = selauth.get_service(args.driver_path)
         if not service:
             return
         selauth.driver = selauth.get_webdriver(service, intercept=True)
         result = selauth.selenium_login_with_prt(url, keep=args.keep_open, prtcookie=args.prt_cookie, capture=args.capture_code)
-        if not result:
+        if not result and not args.keep_open:
             return
         if args.capture_code:
             if result:
                 print(f'Captured auth code: {result}')
+            if not args.keep_open:
+                return
+        else:
+            auth.outfile = args.tokenfile
+            auth.save_tokens(args)
+        if args.keep_open:
+            try:
+                time.sleep(99999)
+            except KeyboardInterrupt:
+                return
             return
-        auth.outfile = args.tokenfile
-        auth.save_tokens(args)
     elif args.command == 'browserprtinject':
         auth.set_client_id(args.client)
         auth.set_resource_uri(args.resource)
         auth.set_user_agent(args.user_agent)
         auth.tenant = args.tenant
         if args.prt and args.prt_sessionkey:
             deviceauth.setprt(args.prt, args.prt_sessionkey)
+        elif args.prt_cookie:
+            pass
         elif args.prt_file and deviceauth.loadprt(args.prt_file):
             pass
         else:
             print('You must either supply a PRT and session key on the command line or a file that contains them')
             return
         selauth = SeleniumAuthentication(auth, deviceauth, args.redirect_url)
         if args.auth_url:
@@ -847,15 +894,15 @@
         else:
             password = args.password
             otpseed = None
         service = selauth.get_service(args.driver_path)
         if not service:
             return
         selauth.driver = selauth.get_webdriver(service, intercept=True)
-        if not selauth.selenium_login_with_prt(url, identity=args.username, password=password, otpseed=otpseed, keep=args.keep_open):
+        if not selauth.selenium_login_with_prt(url, identity=args.username, prtcookie=args.prt_cookie, password=password, otpseed=otpseed, keep=args.keep_open):
             return
         auth.outfile = args.tokenfile
         auth.save_tokens(args)
     elif args.command == 'prtenrich':
         if not args.no_prt:
             if args.prt and args.prt_sessionkey:
                 deviceauth.setprt(args.prt, args.prt_sessionkey)
@@ -952,15 +999,20 @@
         print(json.dumps(body, sort_keys=True, indent=4))
     elif args.command in ('getscope', 'findscope'):
         # Load scope data
         current_dir = os.path.abspath(os.path.dirname(__file__))
         datafile = os.path.join(current_dir, 'firstpartyscopes.json')
         with codecs.open(datafile,'r','utf-8') as infile:
             data = json.load(infile)
-        resource, scope = args.scope.lower().rsplit('/', 1)
+        try:
+            resource, scope = args.scope.lower().rsplit('/', 1)
+        except ValueError:
+            print("No resource (API) specified in scope, defaulting to Microsoft Graph")
+            resource = "https://graph.microsoft.com"
+            scope = args.scope
         try:
             resourceid = data['resourceidentifiers'][resource.lower()]
         except KeyError:
             try:
                 resourceid = data['resourceidentifiers'][resource.lower() + '/']
             except KeyError:
                 print(f'The API {resource} is not a known resource')
@@ -1092,12 +1144,26 @@
         elif args.unique_id:
             uid = args.unique_id
         else:
             uid = encode_object_guid(args.guid)
         template, assertionid = signer.format_template(uid, args.upn, args.issuer, args.mfa)
         signed = signer.sign_xml(template, assertionid)
         print(signed.decode('utf-8'))
+    elif args.command == 'prtcookie':
+        if args.prt and args.prt_sessionkey:
+            deviceauth.setprt(args.prt, args.prt_sessionkey)
+        elif args.prt_file and deviceauth.loadprt(args.prt_file):
+            pass
+        else:
+            print('You must either supply a PRT and session key on the command line or a file that contains them')
+            return
+        challenge = auth.get_srv_challenge()['Nonce']
+        cookie = auth.create_prt_cookie_kdf_ver_2(deviceauth.prt, deviceauth.session_key, challenge)
+        print(f"PRT cookie: {cookie}")
+        print("Can be used in external browsers using the x-ms-RefreshTokenCredential header or cookie. Note that a PRT cookie is only valid for 5 minutes.")
+
+
 
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `roadtx-1.7.0/roadtools/roadtx/selenium.py` & `roadtx-1.7.1/roadtools/roadtx/selenium.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,23 +52,27 @@
                     'https': f'https://{self.proxy}',
                     'no_proxy': 'localhost,127.0.0.1'
                 },
                 'request_storage': 'memory'
             }
             firefox_options=FirefoxOptions()
             firefox_options.add_argument("-headless")
+            # Force intercept to add proxy
+            intercept = True
         elif self.proxy:
             options = {
                 'proxy': {
                     'http': f'http://{self.proxy}',
                     'https': f'https://{self.proxy}',
                     'no_proxy': 'localhost,127.0.0.1'
                 },
                 'request_storage': 'memory'
             }
+            # Force intercept to add proxy
+            intercept = True
         else:
             options = {'request_storage': 'memory'}
         if intercept and self.headless:
             firefox_options=FirefoxOptions()
             firefox_options.add_argument("-headless")
             driver = webdriver_wire.Firefox(service=service,  options=firefox_options, seleniumwire_options=options)
         elif intercept:
@@ -190,15 +194,15 @@
                 return True
             except TimeoutException:
                 if not keep:
                     driver.close()
                     raise AuthenticationException('Could not complete device code auth within the time limit (button not found: idSIButton9)')
         else:
             try:
-                WebDriverWait(driver, 120).until(lambda d: '?code=' in d.current_url)
+                WebDriverWait(driver, 1200).until(lambda d: '?code=' in d.current_url)
                 res = urlparse(driver.current_url)
                 params = parse_qs(res.query)
                 code = params['code'][0]
                 if not keep:
                     driver.close()
                 if capture:
                     return code
```

### Comparing `roadtx-1.7.0/setup.py` & `roadtx-1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name='roadtx',
-      version='1.7.0',
+      version='1.7.1',
       description='ROADtools Token eXchange',
       author='Dirk-jan Mollema',
       author_email='dirkjan@outsidersecurity.nl',
       url='https://github.com/dirkjanm/ROADtools/',
       license='MIT',
       classifiers=[
           'Intended Audience :: Information Technology',
@@ -14,21 +14,22 @@
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
       ],
       packages=['roadtools.roadtx'],
       package_data={'roadtools.roadtx': ['firstpartyscopes.json']},
       install_requires=[
-          'roadlib>=0.22',
+          'roadlib>=0.23',
           'requests',
           'selenium',
           'selenium-wire',
           'pyotp',
           'pycryptodomex',
-          'signxml'
+          'signxml',
+          'blinker<1.8.0'
       ],
       zip_safe=False,
       include_package_data=True,
       entry_points={
           'console_scripts': ['roadtx=roadtools.roadtx.main:main',]
       }
       )
```

