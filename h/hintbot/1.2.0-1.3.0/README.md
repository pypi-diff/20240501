# Comparing `tmp/hintbot-1.2.0.tar.gz` & `tmp/hintbot-1.3.0.tar.gz`

## Comparing `hintbot-1.2.0.tar` & `hintbot-1.3.0.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 hintbot-1.2.0/.copier-answers.yml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hintbot-1.2.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.2.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hintbot-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 hintbot-1.2.0/RELEASE.md
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 hintbot-1.2.0/install.json
--rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.2.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hintbot-1.2.0/setup.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hintbot-1.2.0/tsconfig.json
--rw-r--r--   0        0        0   220911 2020-02-02 00:00:00.000000 hintbot-1.2.0/yarn.lock
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 hintbot-1.2.0/example/assignment4.ipynb
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/_version.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/application.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/handlers.py
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/package.json
--rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/schemas/hintbot/package.json.orig
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/schemas/hintbot/plugin.json
--rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/static/496.116a981237ad27c0bb8f.js
--rw-r--r--   0        0        0     7450 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/static/747.ded73249030e62fecded.js
--rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/static/remoteEntry.f3930c09f071042e569d.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hintbot-1.2.0/jupyter-config/server-config/hintbot.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.2.0/schema/plugin.json
--rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/createHintBanner.ts
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/handler.ts
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/index.ts
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/requestHint.ts
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/showHintTypeDialog.tsx
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/showReflectionDialog.tsx
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 hintbot-1.2.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.2.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hintbot-1.2.0/style/index.js
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 hintbot-1.2.0/.gitignore
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 hintbot-1.2.0/LICENSE
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 hintbot-1.2.0/README.md
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 hintbot-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 hintbot-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 hintbot-1.3.0/.copier-answers.yml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hintbot-1.3.0/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.3.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hintbot-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 hintbot-1.3.0/RELEASE.md
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 hintbot-1.3.0/install.json
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.3.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hintbot-1.3.0/setup.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hintbot-1.3.0/tsconfig.json
+-rw-r--r--   0        0        0   220911 2020-02-02 00:00:00.000000 hintbot-1.3.0/yarn.lock
+-rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 hintbot-1.3.0/example/assignment1.ipynb
+-rw-r--r--   0        0        0    10402 2020-02-02 00:00:00.000000 hintbot-1.3.0/example/assignment2.ipynb
+-rw-r--r--   0        0        0    12043 2020-02-02 00:00:00.000000 hintbot-1.3.0/example/assignment3.ipynb
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 hintbot-1.3.0/example/assignment4.ipynb
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/_version.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/application.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/handlers.py
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/labextension/package.json
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/labextension/schemas/hintbot/package.json.orig
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/labextension/schemas/hintbot/plugin.json
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/labextension/static/496.48e8a8a41e7a4f0b36b7.js
+-rw-r--r--   0        0        0     7450 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/labextension/static/747.ded73249030e62fecded.js
+-rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/labextension/static/remoteEntry.ce3d37020c7d1238fa01.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hintbot-1.3.0/hintbot/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hintbot-1.3.0/jupyter-config/server-config/hintbot.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.3.0/schema/plugin.json
+-rw-r--r--   0        0        0     8212 2020-02-02 00:00:00.000000 hintbot-1.3.0/src/createHintBanner.ts
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hintbot-1.3.0/src/handler.ts
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 hintbot-1.3.0/src/index.ts
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 hintbot-1.3.0/src/requestHint.ts
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hintbot-1.3.0/src/showHintTypeDialog.tsx
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 hintbot-1.3.0/src/showReflectionDialog.tsx
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 hintbot-1.3.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.3.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hintbot-1.3.0/style/index.js
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 hintbot-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 hintbot-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 hintbot-1.3.0/README.md
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 hintbot-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 hintbot-1.3.0/PKG-INFO
```

### Comparing `hintbot-1.2.0/RELEASE.md` & `hintbot-1.3.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/package.json` & `hintbot-1.3.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.3.0'"}*

```diff
@@ -203,9 +203,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.2.0"
+    "version": "1.3.0"
 }
```

### Comparing `hintbot-1.2.0/tsconfig.json` & `hintbot-1.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/yarn.lock` & `hintbot-1.3.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/example/assignment4.ipynb` & `hintbot-1.3.0/example/assignment4.ipynb`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/hintbot/__init__.py` & `hintbot-1.3.0/hintbot/__init__.py`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/hintbot/handlers.py` & `hintbot-1.3.0/hintbot/handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import json
 import os
 import requests
 import tornado
+import base64
+from dotenv import load_dotenv
 from jupyter_server.base.handlers import JupyterHandler
 from jupyter_server.extension.handler import ExtensionHandlerMixin
+load_dotenv()
 
-HOST_URL = "https://gpt-hints-api-202402-3d06c421464e.herokuapp.com/feedback_generation/query/"
+HOST_URL = os.getenv('HOST_URL')
 
 STATUS = {
     "Loading": 0,
     "Success": 1,
     "Cancelled": 2,
     "Error": 3
 }
@@ -29,30 +32,38 @@
             if self.status == STATUS["Cancelled"]:
                 print('Cancelled')
                 return
 
             yield tornado.gen.sleep(1)
             self._timer += 1
 
-            if self._timer % 10 == 0:
-                response = requests.get(
+            if self._timer % 5 == 0:
+
+                response = requests.post(
                     HOST_URL,
-                    params={"request_id": self._request_id},
+                    json={
+                        "method": "GET",
+                        "port": "9002",
+                        "path": "feedback_generation/query/",
+                        "params": {
+                            "request_id": self._request_id
+                        }
+                    },
                     timeout=10
                 )
                 print(response.json(), self._timer)
 
                 if response.status_code != 200:
                     print("Error")
                     self.status = STATUS["Error"]
                     return
 
-                if response.json()["job_finished"]:
+                if json.loads(response.json()["body"])["job_finished"]:
                     print("Success")
-                    self.result = response.json()
+                    self.result = response.json()["body"]
                     self.status = STATUS["Success"]
                     return
 
         print("Timeout")
         self.status = STATUS["Error"] # Timeout
 
     def cancel(self):
@@ -81,34 +92,41 @@
     async def post(self, resource):
         try:
             body = json.loads(self.request.body)
             if resource == "hint":
                 # hint_type = body.get('hint_type')
                 problem_id = body.get('problem_id')
                 buggy_notebook_path = body.get('buggy_notebook_path')
+                f = open(buggy_notebook_path, "rb")
                 response = requests.post(
+                    # f'{HOST_URL}/feedback_generation/query/?method=POST&port=9002&student_id=x&problem_id={problem_id}',
                     HOST_URL,
-                    data={
-                        "student_id": "x",
-                        # "hint_type": hint_type,
-                        "problem_id": problem_id,
+                    json={
+                        "method": "POST",
+                        "port": "9002",
+                        "path": "feedback_generation/query/",
+                        "body": {
+                            "student_id": "x",
+                            "problem_id": problem_id,
+                            "file": json.dumps(json.load(f)),
+                        }
                     },
-                    files={"file": ("notebook.ipynb", open(buggy_notebook_path, "rb"))},
+                    # files={"file": ("notebook.json", open(buggy_notebook_path, "rb"))},
                     timeout=10
                 )
-
+                f.close()
                 if response.status_code == 200:
-                    request_id = response.json()["request_id"]
+                    request_id = json.loads(response.json()["body"])["request_id"]
                     print(f"Received ticket: {request_id}, waiting for the hint to be generated...")
 
                     newjob = Job(time_limit=240, request_id=request_id)
                     newjob.run()
                     self.extensionapp.jobs[problem_id] = newjob
 
-                    self.write(json.dumps(response.json()))
+                    self.write(response.json()["body"])
                 else:
                     self.write("request ticket error")
 
             elif resource == "check":
                 problem_id = body.get('problem_id')
                 self.write({
                     "status": self.extensionapp.jobs.get(problem_id).status,
```

### Comparing `hintbot-1.2.0/hintbot/labextension/package.json` & `hintbot-1.3.0/hintbot/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788773148148149%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ce3d37020c7d1238fa01.js'}}",*

 * * "'version'": "'1.3.0'"}*

```diff
@@ -105,15 +105,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/educational-technology-collective/hintbot",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f3930c09f071042e569d.js",
+            "load": "static/remoteEntry.ce3d37020c7d1238fa01.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "hintbot"
                 },
@@ -208,9 +208,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.2.0"
+    "version": "1.3.0"
 }
```

### Comparing `hintbot-1.2.0/hintbot/labextension/schemas/hintbot/package.json.orig` & `hintbot-1.3.0/hintbot/labextension/schemas/hintbot/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.3.0'"}*

```diff
@@ -203,9 +203,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.2.0"
+    "version": "1.3.0"
 }
```

### Comparing `hintbot-1.2.0/hintbot/labextension/schemas/hintbot/plugin.json` & `hintbot-1.3.0/hintbot/labextension/schemas/hintbot/plugin.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/hintbot/labextension/static/496.116a981237ad27c0bb8f.js` & `hintbot-1.3.0/hintbot/labextension/static/496.48e8a8a41e7a4f0b36b7.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 "use strict";
 (self.webpackChunkhintbot = self.webpackChunkhintbot || []).push([
     [496], {
         496: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => p
+                default: () => b
             });
-            var o = n(99),
-                a = n(947),
-                i = n(464),
+            var o = n(832),
+                a = n(184),
+                i = n(756),
                 r = n(882),
                 s = n(637),
                 l = n(29),
                 d = n.n(l);
             class c extends i.ReactWidget {
                 constructor(e) {
                     super(), this._message = "", this._message = e
@@ -38,35 +38,35 @@
                     className: "jp-Dialog-button jp-mod-reject jp-mod-styled"
                 }), i.Dialog.createButton({
                     label: "Submit",
                     className: "jp-Dialog-button jp-mod-accept jp-mod-styled"
                 })],
                 hasClose: !1
             });
-            var m = n(671),
-                h = n(818);
+            var h = n(363),
+                m = n(520);
             async function g(e = "", t = {}) {
-                const n = h.ServerConnection.makeSettings(),
-                    o = m.URLExt.join(n.baseUrl, "hintbot", e);
+                const n = m.ServerConnection.makeSettings(),
+                    o = h.URLExt.join(n.baseUrl, "hintbot", e);
                 let a;
                 try {
-                    a = await h.ServerConnection.makeRequest(o, t, n)
+                    a = await m.ServerConnection.makeRequest(o, t, n)
                 } catch (e) {
-                    throw new h.ServerConnection.NetworkError(e)
+                    throw new m.ServerConnection.NetworkError(e)
                 }
                 let i = await a.text();
                 if (i.length > 0) try {
                     i = JSON.parse(i)
                 } catch (e) {
                     console.log("Not a JSON response body.", a)
                 }
-                if (!a.ok) throw new h.ServerConnection.ResponseError(a, i.message || i);
+                if (!a.ok) throw new m.ServerConnection.ResponseError(a, i.message || i);
                 return i
             }
-            const b = async (e, t, n, o) => {
+            const p = async (e, t, n, o) => {
                 var a;
                 const r = null === (a = o.getMetadata("nbgrader")) || void 0 === a ? void 0 : a.grade_id,
                     s = o.getMetadata("remaining_hints");
                 if (document.getElementById("hint-banner"))(0, i.showDialog)({
                     title: "Please review previous hint first.",
                     buttons: [i.Dialog.createButton({
                         label: "Dismiss",
@@ -161,53 +161,56 @@
                                                         }
                                                     }, o, !0)
                                                 })), l.innerText = n, d.remove();
                                                 const i = document.createElement("div");
                                                 i.id = "hint-banner-buttons-container";
                                                 const c = document.createElement("div");
                                                 c.id = "hint-banner-buttons";
-                                                const m = document.createElement("button");
-                                                m.classList.add("hint-banner-button"), m.innerText = "Helpful 👍";
                                                 const h = document.createElement("button");
-                                                h.classList.add("hint-banner-button"), h.innerText = "Unhelpful 👎";
+                                                h.classList.add("hint-banner-button"), h.innerText = "Helpful 👍";
+                                                const m = document.createElement("button");
+                                                m.classList.add("hint-banner-button"), m.innerText = "Unhelpful 👎";
                                                 const g = async i => {
                                                     if (t.exporters.forEach((o => {
                                                             t.publishEvent(e, {
                                                                 eventName: "HintEvaluated",
                                                                 eventTime: Date.now(),
                                                                 eventInfo: {
                                                                     gradeId: r,
                                                                     requestId: a,
                                                                     hintContent: n,
                                                                     evaluation: i
                                                                 }
                                                             }, o, !0)
                                                         })), o) {
-                                                        const o = await u("Write a brief statement of what you learned from the hint and how you will use it to solve the problem.");
-                                                        "Submit" === o.button.label && (l.remove(), s.remove()), t.exporters.forEach((i => {
+                                                        const o = ["Considering the hint you just received and your solution thus far, what steps will you take next to move forward on the question?", "Considering the hint you just received and your solution thus far, are there other topics from the course material you should be incorporating into your solution?", "Considering the hint you just received and your solution thus far, was your general approach a good one, or should you change to an alternative approach to solve the step of the question you are working on?"],
+                                                            i = Math.floor(Math.random() * o.length),
+                                                            d = await u(o[i]);
+                                                        "Submit" === d.button.label && (l.remove(), s.remove()), t.exporters.forEach((o => {
                                                             t.publishEvent(e, {
                                                                 eventName: "PostReflection",
                                                                 eventTime: Date.now(),
                                                                 eventInfo: {
-                                                                    status: o.button.label,
+                                                                    status: d.button.label,
                                                                     gradeId: r,
                                                                     requestId: a,
                                                                     hintContent: n,
-                                                                    reflection: o.value
+                                                                    prompt: i,
+                                                                    reflection: d.value
                                                                 }
-                                                            }, i, !0)
+                                                            }, o, !0)
                                                         }))
                                                     } else l.remove(), s.remove()
                                                 };
-                                                m.onclick = () => {
+                                                h.onclick = () => {
                                                     g("helpful")
-                                                }, h.onclick = () => {
+                                                }, m.onclick = () => {
                                                     g("unhelpful")
-                                                }, c.appendChild(h), c.appendChild(m), i.appendChild(c), l.appendChild(i)
-                                            })(c.result.feedback, a);
+                                                }, c.appendChild(m), c.appendChild(h), i.appendChild(c), l.appendChild(i)
+                                            })(JSON.parse(c.result).feedback, a);
                                             else {
                                                 if (2 !== c.status) throw clearInterval(n), new Error(a);
                                                 console.log("cancelled"), clearInterval(n), (n => {
                                                     l.remove(), s.remove(), (0, i.showDialog)({
                                                         title: "Hint Request Cancelled",
                                                         buttons: [i.Dialog.createButton({
                                                             label: "Dismiss",
@@ -246,26 +249,29 @@
                                             }
                                         }, o, !1)
                                     }))
                                 })(n)
                             }
                         })(e, n, o, l), o.setMetadata("remaining_hints", s - 1), document.getElementById(r).innerText = `Hint (${s-1} left for this question)`, e.context.save(), a) {
                         document.getElementById("hint-banner").style.filter = "blur(10px)";
-                        const t = await u("Write a brief statement of what the problem is that you are facing and why you think your solution is not working.");
-                        document.getElementById("hint-banner").style.filter = "none", n.exporters.forEach((o => {
+                        const t = ["Considering your submission and the feedback you have gotten from the system thus far, what are the steps you think must be followed in order to answer this question, and which step is the one you are currently stuck on?", "Considering your submission and the feedback you have gotten from the system thus far, which topics in the course do you think are most relevant to the current problem you are facing?", "Considering your submission and the feedback you have gotten from the system thus far, is there an alternative approach which you can try to to solve the step of the question you are working on?"],
+                            o = Math.floor(Math.random() * t.length),
+                            a = await u(t[o]);
+                        document.getElementById("hint-banner").style.filter = "none", n.exporters.forEach((t => {
                             n.publishEvent(e, {
                                 eventName: "PreReflection",
                                 eventTime: Date.now(),
                                 eventInfo: {
-                                    status: t.button.label,
+                                    status: a.button.label,
                                     gradeId: r,
-                                    reflection: t.value
+                                    prompt: o,
+                                    reflection: a.value
                                 }
-                            }, o, !0)
-                        })), "Cancel" === t.button.label && await g("cancel", {
+                            }, t, !0)
+                        })), "Cancel" === a.button.label && await g("cancel", {
                             method: "POST",
                             body: JSON.stringify({
                                 problem_id: r
                             })
                         })
                     }
                 }
@@ -294,24 +300,24 @@
                                     className: "jp-mod-accept jp-mod-styled"
                                 })],
                                 hasClose: !1
                             })).button.label && (await (async (e, t, n) => {
                                 var o, a, i, r;
                                 const s = t.get("hintQuantity").composite,
                                     l = null === (o = e.content.model) || void 0 === o ? void 0 : o.cells;
-                                if (l && e.model.getMetadata("etc_identifier") && "7ca0093b-b622-4463-8696-65f1e0f33522" === e.model.getMetadata("etc_identifier"))
+                                if (l)
                                     for (let o = 0; o < l.length; o++)
-                                        if (l.get(o).getMetadata("nbgrader") && "markdown" === (null === (a = l.get(o).getMetadata("nbgrader")) || void 0 === a ? void 0 : a.cell_type) && (null === (i = l.get(o).getMetadata("nbgrader")) || void 0 === i ? void 0 : i.grade_id) && "cell-018440eg2f1b6a62" !== (null === (r = l.get(o).getMetadata("nbgrader")) || void 0 === r ? void 0 : r.grade_id)) {
+                                        if (l.get(o).getMetadata("nbgrader") && "markdown" === (null === (a = l.get(o).getMetadata("nbgrader")) || void 0 === a ? void 0 : a.cell_type) && (null === (i = l.get(o).getMetadata("nbgrader")) || void 0 === i ? void 0 : i.grade_id) && !["cell-d4da7eb9acee2a6d", "cell-a839e7b47494b4c2", "cell-018440ed2f1b6a62", "cell-018440eg2f1b6a62"].includes(null === (r = l.get(o).getMetadata("nbgrader")) || void 0 === r ? void 0 : r.grade_id)) {
                                             const a = document.createElement("button");
-                                            a.classList.add("hint-button"), a.id = l.get(o).getMetadata("nbgrader").grade_id, a.onclick = () => b(e, t, n, l.get(o)), e.content.widgets[o].node.appendChild(a), void 0 === l.get(o).getMetadata("remaining_hints") ? (l.get(o).setMetadata("remaining_hints", s), a.innerText = `Hint (${s} left for this question)`) : a.innerText = `Hint (${l.get(o).getMetadata("remaining_hints")} left for this question)`
+                                            a.classList.add("hint-button"), a.id = l.get(o).getMetadata("nbgrader").grade_id, a.onclick = () => p(e, t, n, l.get(o)), e.content.widgets[o].node.appendChild(a), void 0 === l.get(o).getMetadata("remaining_hints") ? (l.get(o).setMetadata("remaining_hints", s), a.innerText = `Hint (${s} left for this question)`) : a.innerText = `Hint (${l.get(o).getMetadata("remaining_hints")} left for this question)`
                                         }
                             })(t, l, o), a.remove(), o.exporters.forEach((e => o.publishEvent(t, {
                                 eventName: "HintBotActivated",
                                 eventTime: Date.now()
                             }, e, !1))))
                         }
                     }))
                 }
-            }, p = v
+            }, b = v
         }
     }
 ]);
```

### Comparing `hintbot-1.2.0/hintbot/labextension/static/747.ded73249030e62fecded.js` & `hintbot-1.3.0/hintbot/labextension/static/747.ded73249030e62fecded.js`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/hintbot/labextension/static/remoteEntry.f3930c09f071042e569d.js` & `hintbot-1.3.0/hintbot/labextension/static/remoteEntry.ce3d37020c7d1238fa01.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -43,18 +43,18 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        496: "116a981237ad27c0bb8f",
+        496: "48e8a8a41e7a4f0b36b7",
         747: "ded73249030e62fecded"
     } [e] + ".js?v=" + {
-        496: "116a981237ad27c0bb8f",
+        496: "48e8a8a41e7a4f0b36b7",
         747: "ded73249030e62fecded"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => S.e(496).then((() => () => S(496))),
                         from: i,
                         eager: !1
                     })
-                })("hintbot", "1.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("hintbot", "1.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -213,23 +213,23 @@
     }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
         var a = S.I(r);
         return a && a.then ? a.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), v = c(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), b = {}, g = {
         29: () => h("default", "react", [1, 18, 2, 0]),
-        99: () => h("default", "@jupyterlab/settingregistry", [1, 4, 1, 6]),
-        464: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        184: () => h("default", "@jupyterlab/notebook", [1, 4, 1, 8]),
+        363: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 8]),
+        520: () => h("default", "@jupyterlab/services", [1, 7, 1, 8]),
         637: () => v("default", "jupyterlab-pioneer", [1, 1, 3, 0]),
-        671: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
-        818: () => h("default", "@jupyterlab/services", [1, 7, 1, 6]),
-        882: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        947: () => h("default", "@jupyterlab/notebook", [1, 4, 1, 6])
+        756: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
+        832: () => h("default", "@jupyterlab/settingregistry", [1, 4, 1, 8]),
+        882: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0])
     }, m = {
-        496: [29, 99, 464, 637, 671, 818, 882, 947]
+        496: [29, 184, 363, 520, 637, 756, 832, 882]
     }, S.f.consumes = (e, r) => {
         S.o(m, e) && m[e].forEach((e => {
             if (S.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
```

### Comparing `hintbot-1.2.0/hintbot/labextension/static/third-party-licenses.json` & `hintbot-1.3.0/hintbot/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/schema/plugin.json` & `hintbot-1.3.0/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/src/createHintBanner.ts` & `hintbot-1.3.0/src/createHintBanner.ts`

 * *Files 5% similar despite different names*

```diff
@@ -92,16 +92,26 @@
             }
           },
           exporter,
           true
         );
       });
       if (postReflection) {
+        const postReflectionPrompts = [
+          'Considering the hint you just received and your solution thus far, what steps will you take next to move forward on the question?',
+          'Considering the hint you just received and your solution thus far, are there other topics from the course material you should be incorporating into your solution?',
+          'Considering the hint you just received and your solution thus far, was your general approach a good one, or should you change to an alternative approach to solve the step of the question you are working on?'
+        ];
+
+        const randomIndex = Math.floor(
+          Math.random() * postReflectionPrompts.length
+        );
+
         const dialogResult = await showReflectionDialog(
-          'Write a brief statement of what you learned from the hint and how you will use it to solve the problem.'
+          postReflectionPrompts[randomIndex]
         );
 
         if (dialogResult.button.label === 'Submit') {
           hintBanner.remove();
           hintBannerPlaceholder.remove();
         }
 
@@ -112,14 +122,15 @@
               eventName: 'PostReflection',
               eventTime: Date.now(),
               eventInfo: {
                 status: dialogResult.button.label,
                 gradeId: gradeId,
                 requestId: requestId,
                 hintContent: hintContent,
+                prompt: randomIndex,
                 reflection: dialogResult.value
                 // hintType: hintType
               }
             },
             exporter,
             true
           );
@@ -231,15 +242,15 @@
 
         if (response.status === STATUS['Loading']) {
           console.log('loading');
           return;
         } else if (response.status === STATUS['Success']) {
           console.log('success');
           clearInterval(intervalId);
-          hintRequestCompleted(response.result.feedback, requestId);
+          hintRequestCompleted(JSON.parse(response.result).feedback, requestId);
         } else if (response.status === STATUS['Cancelled']) {
           console.log('cancelled');
           clearInterval(intervalId);
           hintRequestCancelled(requestId);
         } else {
           clearInterval(intervalId);
           throw new Error(requestId);
```

### Comparing `hintbot-1.2.0/src/handler.ts` & `hintbot-1.3.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/src/index.ts` & `hintbot-1.3.0/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,27 @@
   notebookPanel: NotebookPanel,
   settings: ISettingRegistry.ISettings,
   pioneer: IJupyterLabPioneer
 ) => {
   const hintQuantity = settings.get('hintQuantity').composite as number;
   const cells = notebookPanel.content.model?.cells;
 
-  if (
-    cells &&
-    notebookPanel.model.getMetadata('etc_identifier') &&
-    notebookPanel.model.getMetadata('etc_identifier') ===
-      '7ca0093b-b622-4463-8696-65f1e0f33522'
-    // hardcode assignment identifier, to be removed after api service fully implemented
-  ) {
+  if (cells) {
     for (let i = 0; i < cells.length; i++) {
       if (
         cells.get(i).getMetadata('nbgrader') &&
         cells.get(i).getMetadata('nbgrader')?.cell_type === 'markdown' &&
         cells.get(i).getMetadata('nbgrader')?.grade_id &&
-        cells.get(i).getMetadata('nbgrader')?.grade_id !==
-          'cell-018440eg2f1b6a62' // hardcode question identifier, to be removed after notebook updated and deployed
+        ![
+          'cell-d4da7eb9acee2a6d',
+          'cell-a839e7b47494b4c2',
+          'cell-018440ed2f1b6a62',
+          'cell-018440eg2f1b6a62'
+        ].includes(cells.get(i).getMetadata('nbgrader')?.grade_id)
+        // hardcode question identifier, to be removed after notebook updated and deployed
       ) {
         const hintButton = document.createElement('button');
         hintButton.classList.add('hint-button');
         hintButton.id = cells.get(i).getMetadata('nbgrader').grade_id;
         hintButton.onclick = () =>
           requestHint(notebookPanel, settings, pioneer, cells.get(i));
         notebookPanel.content.widgets[i].node.appendChild(hintButton);
```

### Comparing `hintbot-1.2.0/src/requestHint.ts` & `hintbot-1.3.0/src/requestHint.ts`

 * *Files 18% similar despite different names*

```diff
@@ -113,28 +113,40 @@
       remainingHints - 1
     } left for this question)`;
     notebookPanel.context.save();
 
     if (preReflection) {
       document.getElementById('hint-banner').style.filter = 'blur(10px)';
 
+      const preReflectionPrompts = [
+        'Considering your submission and the feedback you have gotten from the system thus far, what are the steps you think must be followed in order to answer this question, and which step is the one you are currently stuck on?',
+        'Considering your submission and the feedback you have gotten from the system thus far, which topics in the course do you think are most relevant to the current problem you are facing?',
+        'Considering your submission and the feedback you have gotten from the system thus far, is there an alternative approach which you can try to to solve the step of the question you are working on?'
+      ];
+
+      const randomIndex = Math.floor(
+        Math.random() * preReflectionPrompts.length
+      );
+
       const dialogResult = await showReflectionDialog(
-        'Write a brief statement of what the problem is that you are facing and why you think your solution is not working.'
+        preReflectionPrompts[randomIndex]
       );
+
       document.getElementById('hint-banner').style.filter = 'none';
 
       pioneer.exporters.forEach(exporter => {
         pioneer.publishEvent(
           notebookPanel,
           {
             eventName: 'PreReflection',
             eventTime: Date.now(),
             eventInfo: {
               status: dialogResult.button.label,
               gradeId: gradeId,
+              prompt: randomIndex,
               reflection: dialogResult.value
               // hintType: hintType
             }
           },
           exporter,
           true
         );
```

### Comparing `hintbot-1.2.0/src/showHintTypeDialog.tsx` & `hintbot-1.3.0/src/showHintTypeDialog.tsx`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/src/showReflectionDialog.tsx` & `hintbot-1.3.0/src/showReflectionDialog.tsx`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/style/base.css` & `hintbot-1.3.0/style/base.css`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/.gitignore` & `hintbot-1.3.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -115,7 +115,9 @@
 # End of https://www.gitignore.io/api/python
 
 # OSX files
 .DS_Store
 
 # Yarn cache
 .yarn/
+
+.env
```

### Comparing `hintbot-1.2.0/LICENSE` & `hintbot-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/README.md` & `hintbot-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/pyproject.toml` & `hintbot-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hintbot-1.2.0/PKG-INFO` & `hintbot-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hintbot
-Version: 1.2.0
+Version: 1.3.0
 Dynamic: Keywords
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/educational-technology-collective/hintbot
 Project-URL: Bug Tracker, https://github.com/educational-technology-collective/hintbot/issues
 Project-URL: Repository, https://github.com/educational-technology-collective/hintbot.git
 Author-email: etc <mengyanw@umich.edu>
 License: BSD 3-Clause License
```

