# Comparing `tmp/gradio_image_annotation-0.0.4.tar.gz` & `tmp/gradio_image_annotation-0.0.5.tar.gz`

## Comparing `gradio_image_annotation-0.0.4.tar` & `gradio_image_annotation-0.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/package-lock.json
--rwxr-xr-x   0        0        0     1084 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/.github/workflows/python-publish.yml
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/backend/gradio_image_annotation/__init__.py
--rwxr-xr-x   0        0        0    13664 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/backend/gradio_image_annotation/image_annotator.py
--rwxr-xr-x   0        0        0    28802 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/backend/gradio_image_annotation/image_annotator.pyi
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/backend/gradio_image_annotation/templates/component/__vite-browser-external-2447137e.js
--rw-r--r--   0        0        0   312863 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/backend/gradio_image_annotation/templates/component/index.js
--rw-r--r--   0        0        0    24083 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/backend/gradio_image_annotation/templates/component/style.css
--rw-r--r--   0        0        0    78109 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/backend/gradio_image_annotation/templates/component/wrapper-6f348d45-f837cf34.js
--rw-r--r--   0        0        0   152936 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/backend/gradio_image_annotation/templates/example/index.js
--rw-r--r--   0        0        0    21565 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/backend/gradio_image_annotation/templates/example/style.css
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/demo/__init__.py
--rwxr-xr-x   0        0        0     1556 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/demo/css.css
--rw-r--r--   0        0        0    11398 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/demo/space.py
--rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/Example.svelte
--rwxr-xr-x   0        0        0     3269 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/Index.svelte
--rwxr-xr-x   0        0        0    40890 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/package-lock.json
--rwxr-xr-x   0        0        0      803 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/package.json
--rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/AnnotatedImageData.ts
--rwxr-xr-x   0        0        0    10911 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/Box.ts
--rwxr-xr-x   0        0        0     9475 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/Canvas.svelte
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/ClearImage.svelte
--rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/Colors.js
--rwxr-xr-x   0        0        0     4481 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/ImageAnnotator.svelte
--rwxr-xr-x   0        0        0     1760 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/ImageCanvas.svelte
--rwxr-xr-x   0        0        0     3709 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/ModalBox.svelte
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/index.ts
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/utils.ts
--rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/icons/Add.svelte
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/icons/index.ts
--rw-r--r--   0        0        0    12537 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/CHANGELOG.md
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/Dropdown.stories.svelte
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/Example.svelte
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/Index.svelte
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/LICENSE
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/Multiselect.stories.svelte
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/README.md
--rw-r--r--   0        0        0    12541 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/dropdown.test.ts
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/package.json
--rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/shared/Dropdown.svelte
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/shared/DropdownOptions.svelte
--rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/shared/Multiselect.svelte
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/shared/utils.ts
--rwxr-xr-x   0        0        0   174681 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/images/demo_1.png
--rwxr-xr-x   0        0        0  1110082 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/images/demo_2.png
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/LICENSE
--rwxr-xr-x   0        0        0    11498 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/README.md
--rwxr-xr-x   0        0        0     1982 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/package-lock.json
+-rwxr-xr-x   0        0        0     1084 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/backend/gradio_image_annotation/__init__.py
+-rwxr-xr-x   0        0        0    13664 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/backend/gradio_image_annotation/image_annotator.py
+-rwxr-xr-x   0        0        0    28802 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/backend/gradio_image_annotation/image_annotator.pyi
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/backend/gradio_image_annotation/templates/component/__vite-browser-external-2447137e.js
+-rw-r--r--   0        0        0   313293 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/backend/gradio_image_annotation/templates/component/index.js
+-rw-r--r--   0        0        0    24083 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/backend/gradio_image_annotation/templates/component/style.css
+-rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/backend/gradio_image_annotation/templates/component/wrapper-6f348d45-19fa94bf.js
+-rw-r--r--   0        0        0   153371 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/backend/gradio_image_annotation/templates/example/index.js
+-rw-r--r--   0        0        0    21565 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/backend/gradio_image_annotation/templates/example/style.css
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/demo/__init__.py
+-rwxr-xr-x   0        0        0     1556 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/demo/app.py
+-rwxr-xr-x   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/demo/css.css
+-rwxr-xr-x   0        0        0    11398 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/demo/space.py
+-rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/Example.svelte
+-rwxr-xr-x   0        0        0     3269 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/Index.svelte
+-rwxr-xr-x   0        0        0    40890 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/package-lock.json
+-rwxr-xr-x   0        0        0      803 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/package.json
+-rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/AnnotatedImageData.ts
+-rwxr-xr-x   0        0        0    10911 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/Box.ts
+-rwxr-xr-x   0        0        0     9795 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/Canvas.svelte
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/ClearImage.svelte
+-rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/Colors.js
+-rwxr-xr-x   0        0        0     4481 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/ImageAnnotator.svelte
+-rwxr-xr-x   0        0        0     1760 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/ImageCanvas.svelte
+-rwxr-xr-x   0        0        0     3893 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/ModalBox.svelte
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/index.ts
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/utils.ts
+-rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/icons/Add.svelte
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/icons/index.ts
+-rwxr-xr-x   0        0        0    12537 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/CHANGELOG.md
+-rwxr-xr-x   0        0        0      980 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/Dropdown.stories.svelte
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/Example.svelte
+-rwxr-xr-x   0        0        0     2722 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/Index.svelte
+-rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/LICENSE
+-rwxr-xr-x   0        0        0      868 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/Multiselect.stories.svelte
+-rwxr-xr-x   0        0        0     1218 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/README.md
+-rwxr-xr-x   0        0        0    12541 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/dropdown.test.ts
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/package.json
+-rwxr-xr-x   0        0        0     7987 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/shared/Dropdown.svelte
+-rwxr-xr-x   0        0        0     3715 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/shared/DropdownOptions.svelte
+-rwxr-xr-x   0        0        0    10367 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/shared/Multiselect.svelte
+-rwxr-xr-x   0        0        0     1405 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/shared/utils.ts
+-rwxr-xr-x   0        0        0   174681 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/images/demo_1.png
+-rwxr-xr-x   0        0        0  1110082 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/images/demo_2.png
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0    11498 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/README.md
+-rwxr-xr-x   0        0        0     2072 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.5/PKG-INFO
```

### Comparing `gradio_image_annotation-0.0.4/.github/workflows/python-publish.yml` & `gradio_image_annotation-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/backend/gradio_image_annotation/image_annotator.py` & `gradio_image_annotation-0.0.5/backend/gradio_image_annotation/image_annotator.py`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/backend/gradio_image_annotation/image_annotator.pyi` & `gradio_image_annotation-0.0.5/backend/gradio_image_annotation/image_annotator.pyi`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/backend/gradio_image_annotation/templates/component/index.js` & `gradio_image_annotation-0.0.5/backend/gradio_image_annotation/templates/component/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
     get_slot_changes: Qa,
     get_spread_update: Ka,
     init: $a,
     insert: eu,
     safe_not_equal: tu,
     set_dynamic_element_data: Es,
     set_style: Pe,
-    toggle_class: tt,
+    toggle_class: nt,
     transition_in: pr,
     transition_out: wr,
     update_slot_base: nu
 } = window.__gradio__svelte__internal;
 
 function iu(t) {
     let e, n, i;
@@ -52,30 +52,30 @@
         c() {
             e = Ya(
                 /*tag*/
                 t[14]
             ), s && s.c(), Es(
                 /*tag*/
                 t[14]
-            )(e, r), tt(
+            )(e, r), nt(
                 e,
                 "hidden",
                 /*visible*/
                 t[10] === !1
-            ), tt(
+            ), nt(
                 e,
                 "padded",
                 /*padding*/
                 t[6]
-            ), tt(
+            ), nt(
                 e,
                 "border_focus",
                 /*border_mode*/
                 t[5] === "focus"
-            ), tt(e, "hide-container", ! /*explicit_call*/
+            ), nt(e, "hide-container", ! /*explicit_call*/
                 t[8] && ! /*container*/
                 t[9]), Pe(
                 e,
                 "height",
                 /*get_dimension*/
                 t[15](
                     /*height*/
@@ -147,30 +147,30 @@
                         )
                     },
                     (!i || u & /*elem_classes*/
                         8 && n !== (n = "block " + /*elem_classes*/
                             a[3].join(" ") + " svelte-1t38q2d")) && {
                         class: n
                     }
-                ])), tt(
+                ])), nt(
                     e,
                     "hidden",
                     /*visible*/
                     a[10] === !1
-                ), tt(
+                ), nt(
                     e,
                     "padded",
                     /*padding*/
                     a[6]
-                ), tt(
+                ), nt(
                     e,
                     "border_focus",
                     /*border_mode*/
                     a[5] === "focus"
-                ), tt(e, "hide-container", ! /*explicit_call*/
+                ), nt(e, "hide-container", ! /*explicit_call*/
                     a[8] && ! /*container*/
                     a[9]), u & /*height*/
                 1 && Pe(
                     e,
                     "height",
                     /*get_dimension*/
                     a[15](
@@ -268,47 +268,47 @@
     } = e, {
         type: h = "normal"
     } = e, {
         test_id: c = void 0
     } = e, {
         explicit_call: d = !1
     } = e, {
-        container: m = !0
+        container: b = !0
     } = e, {
-        visible: b = !0
+        visible: p = !0
     } = e, {
-        allow_overflow: p = !0
+        allow_overflow: g = !0
     } = e, {
         scale: y = null
     } = e, {
         min_width: w = 0
     } = e, C = h === "fieldset" ? "fieldset" : "div";
     const P = (E) => {
         if (E !== void 0) {
             if (typeof E == "number")
                 return E + "px";
             if (typeof E == "string")
                 return E;
         }
     };
     return t.$$set = (E) => {
-        "height" in E && n(0, s = E.height), "width" in E && n(1, o = E.width), "elem_id" in E && n(2, r = E.elem_id), "elem_classes" in E && n(3, a = E.elem_classes), "variant" in E && n(4, u = E.variant), "border_mode" in E && n(5, f = E.border_mode), "padding" in E && n(6, _ = E.padding), "type" in E && n(16, h = E.type), "test_id" in E && n(7, c = E.test_id), "explicit_call" in E && n(8, d = E.explicit_call), "container" in E && n(9, m = E.container), "visible" in E && n(10, b = E.visible), "allow_overflow" in E && n(11, p = E.allow_overflow), "scale" in E && n(12, y = E.scale), "min_width" in E && n(13, w = E.min_width), "$$scope" in E && n(17, l = E.$$scope);
+        "height" in E && n(0, s = E.height), "width" in E && n(1, o = E.width), "elem_id" in E && n(2, r = E.elem_id), "elem_classes" in E && n(3, a = E.elem_classes), "variant" in E && n(4, u = E.variant), "border_mode" in E && n(5, f = E.border_mode), "padding" in E && n(6, _ = E.padding), "type" in E && n(16, h = E.type), "test_id" in E && n(7, c = E.test_id), "explicit_call" in E && n(8, d = E.explicit_call), "container" in E && n(9, b = E.container), "visible" in E && n(10, p = E.visible), "allow_overflow" in E && n(11, g = E.allow_overflow), "scale" in E && n(12, y = E.scale), "min_width" in E && n(13, w = E.min_width), "$$scope" in E && n(17, l = E.$$scope);
     }, [
         s,
         o,
         r,
         a,
         u,
         f,
         _,
         c,
         d,
-        m,
         b,
         p,
+        g,
         y,
         w,
         C,
         P,
         h,
         l,
         i
@@ -421,30 +421,30 @@
 const {
     SvelteComponent: ku,
     attr: ks,
     check_outros: Su,
     create_component: Cu,
     create_slot: Au,
     destroy_component: Bu,
-    detach: ui,
+    detach: _i,
     element: Tu,
     empty: Hu,
     get_all_dirty_from_scope: Pu,
     get_slot_changes: Nu,
     group_outros: Lu,
     init: Iu,
-    insert: fi,
+    insert: hi,
     mount_component: Mu,
     safe_not_equal: Ou,
     set_data: Du,
     space: Ru,
     text: Uu,
-    toggle_class: Rt,
-    transition_in: vn,
-    transition_out: ci,
+    toggle_class: Ft,
+    transition_in: Sn,
+    transition_out: di,
     update_slot_base: Fu
 } = window.__gradio__svelte__internal;
 
 function Ss(t) {
     let e, n;
     return e = new Eu({
         props: {
@@ -467,18 +467,18 @@
             l & /*$$scope, info*/
                 10 && (s.$$scope = {
                     dirty: l,
                     ctx: i
                 }), e.$set(s);
         },
         i(i) {
-            n || (vn(e.$$.fragment, i), n = !0);
+            n || (Sn(e.$$.fragment, i), n = !0);
         },
         o(i) {
-            ci(e.$$.fragment, i), n = !1;
+            di(e.$$.fragment, i), n = !1;
         },
         d(i) {
             Bu(e, i);
         }
     };
 }
 
@@ -488,26 +488,26 @@
         c() {
             e = Uu(
                 /*info*/
                 t[1]
             );
         },
         m(n, i) {
-            fi(n, e, i);
+            hi(n, e, i);
         },
         p(n, i) {
             i & /*info*/
                 2 && Du(
                     e,
                     /*info*/
                     n[1]
                 );
         },
         d(n) {
-            n && ui(e);
+            n && _i(e);
         }
     };
 }
 
 function zu(t) {
     let e, n, i, l;
     const s = (
@@ -523,25 +523,25 @@
         );
     let r = (
         /*info*/
         t[1] && Ss(t)
     );
     return {
         c() {
-            e = Tu("span"), o && o.c(), n = Ru(), r && r.c(), i = Hu(), ks(e, "data-testid", "block-info"), ks(e, "class", "svelte-22c38v"), Rt(e, "sr-only", ! /*show_label*/
-                t[0]), Rt(e, "hide", ! /*show_label*/
-                t[0]), Rt(
+            e = Tu("span"), o && o.c(), n = Ru(), r && r.c(), i = Hu(), ks(e, "data-testid", "block-info"), ks(e, "class", "svelte-22c38v"), Ft(e, "sr-only", ! /*show_label*/
+                t[0]), Ft(e, "hide", ! /*show_label*/
+                t[0]), Ft(
                 e,
                 "has-info",
                 /*info*/
                 t[1] != null
             );
         },
         m(a, u) {
-            fi(a, e, u), o && o.m(e, null), fi(a, n, u), r && r.m(a, u), fi(a, i, u), l = !0;
+            hi(a, e, u), o && o.m(e, null), hi(a, n, u), r && r.m(a, u), hi(a, i, u), l = !0;
         },
         p(a, [u]) {
             o && o.p && (!l || u & /*$$scope*/
                     8) && Fu(
                     o,
                     s,
                     a,
@@ -555,37 +555,37 @@
                         null
                     ) : Pu(
                         /*$$scope*/
                         a[3]
                     ),
                     null
                 ), (!l || u & /*show_label*/
-                    1) && Rt(e, "sr-only", ! /*show_label*/
+                    1) && Ft(e, "sr-only", ! /*show_label*/
                     a[0]), (!l || u & /*show_label*/
-                    1) && Rt(e, "hide", ! /*show_label*/
+                    1) && Ft(e, "hide", ! /*show_label*/
                     a[0]), (!l || u & /*info*/
-                    2) && Rt(
+                    2) && Ft(
                     e,
                     "has-info",
                     /*info*/
                     a[1] != null
                 ), /*info*/
                 a[1] ? r ? (r.p(a, u), u & /*info*/
-                    2 && vn(r, 1)) : (r = Ss(a), r.c(), vn(r, 1), r.m(i.parentNode, i)) : r && (Lu(), ci(r, 1, 1, () => {
+                    2 && Sn(r, 1)) : (r = Ss(a), r.c(), Sn(r, 1), r.m(i.parentNode, i)) : r && (Lu(), di(r, 1, 1, () => {
                     r = null;
                 }), Su());
         },
         i(a) {
-            l || (vn(o, a), vn(r), l = !0);
+            l || (Sn(o, a), Sn(r), l = !0);
         },
         o(a) {
-            ci(o, a), ci(r), l = !1;
+            di(o, a), di(r), l = !1;
         },
         d(a) {
-            a && (ui(e), ui(n), ui(i)), o && o.d(a), r && r.d(a);
+            a && (_i(e), _i(n), _i(i)), o && o.d(a), r && r.d(a);
         }
     };
 }
 
 function ju(t, e, n) {
     let {
         $$slots: i = {},
@@ -606,47 +606,47 @@
             info: 1
         });
     }
 }
 const {
     SvelteComponent: Gu,
     append: Zi,
-    attr: Vn,
+    attr: Zn,
     create_component: xu,
     destroy_component: Vu,
     detach: Xu,
     element: Cs,
     init: Wu,
     insert: Zu,
     mount_component: Yu,
     safe_not_equal: Ju,
     set_data: Qu,
     space: Ku,
     text: $u,
-    toggle_class: nt,
+    toggle_class: it,
     transition_in: ef,
     transition_out: tf
 } = window.__gradio__svelte__internal;
 
 function nf(t) {
     let e, n, i, l, s, o;
     return i = new /*Icon*/
     t[1]({}), {
         c() {
             e = Cs("label"), n = Cs("span"), xu(i.$$.fragment), l = Ku(), s = $u(
                 /*label*/
                 t[0]
-            ), Vn(n, "class", "svelte-9gxdi0"), Vn(e, "for", ""), Vn(e, "data-testid", "block-label"), Vn(e, "class", "svelte-9gxdi0"), nt(e, "hide", ! /*show_label*/
-                t[2]), nt(e, "sr-only", ! /*show_label*/
-                t[2]), nt(
+            ), Zn(n, "class", "svelte-9gxdi0"), Zn(e, "for", ""), Zn(e, "data-testid", "block-label"), Zn(e, "class", "svelte-9gxdi0"), it(e, "hide", ! /*show_label*/
+                t[2]), it(e, "sr-only", ! /*show_label*/
+                t[2]), it(
                 e,
                 "float",
                 /*float*/
                 t[4]
-            ), nt(
+            ), it(
                 e,
                 "hide-label",
                 /*disable*/
                 t[3]
             );
         },
         m(r, a) {
@@ -655,25 +655,25 @@
         p(r, [a]) {
             (!o || a & /*label*/
                 1) && Qu(
                 s,
                 /*label*/
                 r[0]
             ), (!o || a & /*show_label*/
-                4) && nt(e, "hide", ! /*show_label*/
+                4) && it(e, "hide", ! /*show_label*/
                 r[2]), (!o || a & /*show_label*/
-                4) && nt(e, "sr-only", ! /*show_label*/
+                4) && it(e, "sr-only", ! /*show_label*/
                 r[2]), (!o || a & /*float*/
-                16) && nt(
+                16) && it(
                 e,
                 "float",
                 /*float*/
                 r[4]
             ), (!o || a & /*disable*/
-                8) && nt(
+                8) && it(
                 e,
                 "hide-label",
                 /*disable*/
                 r[3]
             );
         },
         i(r) {
@@ -726,18 +726,18 @@
     element: Dl,
     init: ff,
     insert: Er,
     listen: cf,
     mount_component: _f,
     safe_not_equal: hf,
     set_data: df,
-    set_style: Xn,
+    set_style: Yn,
     space: mf,
     text: gf,
-    toggle_class: Oe,
+    toggle_class: Me,
     transition_in: bf,
     transition_out: pf
 } = window.__gradio__svelte__internal;
 
 function As(t) {
     let e, n;
     return {
@@ -768,20 +768,20 @@
     let e, n, i, l, s, o, r, a = (
         /*show_label*/
         t[2] && As(t)
     );
     return l = new /*Icon*/
     t[0]({}), {
         c() {
-            e = Dl("button"), a && a.c(), n = mf(), i = Dl("div"), af(l.$$.fragment), Qe(i, "class", "svelte-lpi64a"), Oe(
+            e = Dl("button"), a && a.c(), n = mf(), i = Dl("div"), af(l.$$.fragment), Qe(i, "class", "svelte-lpi64a"), Me(
                     i,
                     "small",
                     /*size*/
                     t[4] === "small"
-                ), Oe(
+                ), Me(
                     i,
                     "large",
                     /*size*/
                     t[4] === "large"
                 ), e.disabled = /*disabled*/
                 t[7], Qe(
                     e,
@@ -794,40 +794,40 @@
                     /*hasPopup*/
                     t[8]
                 ), Qe(
                     e,
                     "title",
                     /*label*/
                     t[1]
-                ), Qe(e, "class", "svelte-lpi64a"), Oe(
+                ), Qe(e, "class", "svelte-lpi64a"), Me(
                     e,
                     "pending",
                     /*pending*/
                     t[3]
-                ), Oe(
+                ), Me(
                     e,
                     "padded",
                     /*padded*/
                     t[5]
-                ), Oe(
+                ), Me(
                     e,
                     "highlight",
                     /*highlight*/
                     t[6]
-                ), Oe(
+                ), Me(
                     e,
                     "transparent",
                     /*transparent*/
                     t[9]
-                ), Xn(e, "color", ! /*disabled*/
+                ), Yn(e, "color", ! /*disabled*/
                     t[7] && /*_color*/
                     t[11] ? (
                         /*_color*/
                         t[11]
-                    ) : "var(--block-label-text-color)"), Xn(e, "--bg-color", /*disabled*/
+                    ) : "var(--block-label-text-color)"), Yn(e, "--bg-color", /*disabled*/
                     t[7] ? "auto" : (
                         /*background*/
                         t[10]
                     ));
         },
         m(u, f) {
             Er(u, e, f), a && a.m(e, null), Ol(e, n), Ol(e, i), _f(l, i, null), s = !0, o || (r = cf(
@@ -836,21 +836,21 @@
                 /*click_handler*/
                 t[13]
             ), o = !0);
         },
         p(u, [f]) {
             /*show_label*/
             u[2] ? a ? a.p(u, f) : (a = As(u), a.c(), a.m(e, n)) : a && (a.d(1), a = null), (!s || f & /*size*/
-                    16) && Oe(
+                    16) && Me(
                     i,
                     "small",
                     /*size*/
                     u[4] === "small"
                 ), (!s || f & /*size*/
-                    16) && Oe(
+                    16) && Me(
                     i,
                     "large",
                     /*size*/
                     u[4] === "large"
                 ), (!s || f & /*disabled*/
                     128) && (e.disabled = /*disabled*/
                     u[7]), (!s || f & /*label*/
@@ -868,45 +868,45 @@
                 ), (!s || f & /*label*/
                     2) && Qe(
                     e,
                     "title",
                     /*label*/
                     u[1]
                 ), (!s || f & /*pending*/
-                    8) && Oe(
+                    8) && Me(
                     e,
                     "pending",
                     /*pending*/
                     u[3]
                 ), (!s || f & /*padded*/
-                    32) && Oe(
+                    32) && Me(
                     e,
                     "padded",
                     /*padded*/
                     u[5]
                 ), (!s || f & /*highlight*/
-                    64) && Oe(
+                    64) && Me(
                     e,
                     "highlight",
                     /*highlight*/
                     u[6]
                 ), (!s || f & /*transparent*/
-                    512) && Oe(
+                    512) && Me(
                     e,
                     "transparent",
                     /*transparent*/
                     u[9]
                 ), f & /*disabled, _color*/
-                2176 && Xn(e, "color", ! /*disabled*/
+                2176 && Yn(e, "color", ! /*disabled*/
                     u[7] && /*_color*/
                     u[11] ? (
                         /*_color*/
                         u[11]
                     ) : "var(--block-label-text-color)"), f & /*disabled, background*/
-                1152 && Xn(e, "--bg-color", /*disabled*/
+                1152 && Yn(e, "--bg-color", /*disabled*/
                     u[7] ? "auto" : (
                         /*background*/
                         u[10]
                     ));
         },
         i(u) {
             s || (bf(l.$$.fragment, u), s = !0);
@@ -951,40 +951,40 @@
         {
             color: c = "var(--block-label-text-color)"
         } = e,
         {
             transparent: d = !1
         } = e,
         {
-            background: m = "var(--background-fill-primary)"
+            background: b = "var(--background-fill-primary)"
         } = e;
 
-    function b(p) {
-        rf.call(this, t, p);
+    function p(g) {
+        rf.call(this, t, g);
     }
-    return t.$$set = (p) => {
-        "Icon" in p && n(0, l = p.Icon), "label" in p && n(1, s = p.label), "show_label" in p && n(2, o = p.show_label), "pending" in p && n(3, r = p.pending), "size" in p && n(4, a = p.size), "padded" in p && n(5, u = p.padded), "highlight" in p && n(6, f = p.highlight), "disabled" in p && n(7, _ = p.disabled), "hasPopup" in p && n(8, h = p.hasPopup), "color" in p && n(12, c = p.color), "transparent" in p && n(9, d = p.transparent), "background" in p && n(10, m = p.background);
+    return t.$$set = (g) => {
+        "Icon" in g && n(0, l = g.Icon), "label" in g && n(1, s = g.label), "show_label" in g && n(2, o = g.show_label), "pending" in g && n(3, r = g.pending), "size" in g && n(4, a = g.size), "padded" in g && n(5, u = g.padded), "highlight" in g && n(6, f = g.highlight), "disabled" in g && n(7, _ = g.disabled), "hasPopup" in g && n(8, h = g.hasPopup), "color" in g && n(12, c = g.color), "transparent" in g && n(9, d = g.transparent), "background" in g && n(10, b = g.background);
     }, t.$$.update = () => {
         t.$$.dirty & /*highlight, color*/
             4160 && n(11, i = f ? "var(--color-accent)" : c);
     }, [
         l,
         s,
         o,
         r,
         a,
         u,
         f,
         _,
         h,
         d,
-        m,
+        b,
         i,
         c,
-        b
+        p
     ];
 }
 class as extends of {
     constructor(e) {
         super(), ff(this, e, vf, wf, hf, {
             Icon: 0,
             label: 1,
@@ -1010,15 +1010,15 @@
     detach: Cf,
     element: Bs,
     get_all_dirty_from_scope: Af,
     get_slot_changes: Bf,
     init: Tf,
     insert: Hf,
     safe_not_equal: Pf,
-    toggle_class: it,
+    toggle_class: lt,
     transition_in: Nf,
     transition_out: Lf,
     update_slot_base: If
 } = window.__gradio__svelte__internal;
 
 function Mf(t) {
     let e, n, i;
@@ -1031,30 +1031,30 @@
             t,
             /*$$scope*/
             t[4],
             null
         );
     return {
         c() {
-            e = Bs("div"), n = Bs("div"), s && s.c(), Yi(n, "class", "icon svelte-3w3rth"), Yi(e, "class", "empty svelte-3w3rth"), Yi(e, "aria-label", "Empty value"), it(
+            e = Bs("div"), n = Bs("div"), s && s.c(), Yi(n, "class", "icon svelte-3w3rth"), Yi(e, "class", "empty svelte-3w3rth"), Yi(e, "aria-label", "Empty value"), lt(
                 e,
                 "small",
                 /*size*/
                 t[0] === "small"
-            ), it(
+            ), lt(
                 e,
                 "large",
                 /*size*/
                 t[0] === "large"
-            ), it(
+            ), lt(
                 e,
                 "unpadded_box",
                 /*unpadded_box*/
                 t[1]
-            ), it(
+            ), lt(
                 e,
                 "small_parent",
                 /*parent_height*/
                 t[3]
             );
         },
         m(o, r) {
@@ -1076,33 +1076,33 @@
                     null
                 ) : Af(
                     /*$$scope*/
                     o[4]
                 ),
                 null
             ), (!i || r & /*size*/
-                1) && it(
+                1) && lt(
                 e,
                 "small",
                 /*size*/
                 o[0] === "small"
             ), (!i || r & /*size*/
-                1) && it(
+                1) && lt(
                 e,
                 "large",
                 /*size*/
                 o[0] === "large"
             ), (!i || r & /*unpadded_box*/
-                2) && it(
+                2) && lt(
                 e,
                 "unpadded_box",
                 /*unpadded_box*/
                 o[1]
             ), (!i || r & /*parent_height*/
-                8) && it(
+                8) && lt(
                 e,
                 "small_parent",
                 /*parent_height*/
                 o[3]
             );
         },
         i(o) {
@@ -1183,29 +1183,29 @@
             unpadded_box: 1
         });
     }
 }
 const {
     SvelteComponent: Uf,
     append: Ji,
-    attr: Ue,
+    attr: Re,
     detach: Ff,
     init: qf,
     insert: zf,
     noop: Qi,
     safe_not_equal: jf,
     set_style: Ge,
-    svg_element: Wn
+    svg_element: Jn
 } = window.__gradio__svelte__internal;
 
 function Gf(t) {
     let e, n, i, l;
     return {
         c() {
-            e = Wn("svg"), n = Wn("g"), i = Wn("path"), l = Wn("path"), Ue(i, "d", "M18,6L6.087,17.913"), Ge(i, "fill", "none"), Ge(i, "fill-rule", "nonzero"), Ge(i, "stroke-width", "2px"), Ue(n, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), Ue(l, "d", "M4.364,4.364L19.636,19.636"), Ge(l, "fill", "none"), Ge(l, "fill-rule", "nonzero"), Ge(l, "stroke-width", "2px"), Ue(e, "width", "100%"), Ue(e, "height", "100%"), Ue(e, "viewBox", "0 0 24 24"), Ue(e, "version", "1.1"), Ue(e, "xmlns", "http://www.w3.org/2000/svg"), Ue(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), Ue(e, "xml:space", "preserve"), Ue(e, "stroke", "currentColor"), Ge(e, "fill-rule", "evenodd"), Ge(e, "clip-rule", "evenodd"), Ge(e, "stroke-linecap", "round"), Ge(e, "stroke-linejoin", "round");
+            e = Jn("svg"), n = Jn("g"), i = Jn("path"), l = Jn("path"), Re(i, "d", "M18,6L6.087,17.913"), Ge(i, "fill", "none"), Ge(i, "fill-rule", "nonzero"), Ge(i, "stroke-width", "2px"), Re(n, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), Re(l, "d", "M4.364,4.364L19.636,19.636"), Ge(l, "fill", "none"), Ge(l, "fill-rule", "nonzero"), Ge(l, "stroke-width", "2px"), Re(e, "width", "100%"), Re(e, "height", "100%"), Re(e, "viewBox", "0 0 24 24"), Re(e, "version", "1.1"), Re(e, "xmlns", "http://www.w3.org/2000/svg"), Re(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), Re(e, "xml:space", "preserve"), Re(e, "stroke", "currentColor"), Ge(e, "fill-rule", "evenodd"), Ge(e, "clip-rule", "evenodd"), Ge(e, "stroke-linecap", "round"), Ge(e, "stroke-linejoin", "round");
         },
         m(s, o) {
             zf(s, e, o), Ji(e, n), Ji(n, i), Ji(e, l);
         },
         p: Qi,
         i: Qi,
         o: Qi,
@@ -1218,28 +1218,28 @@
     constructor(e) {
         super(), qf(this, e, null, Gf, jf, {});
     }
 }
 const {
     SvelteComponent: xf,
     append: Vf,
-    attr: mn,
+    attr: wn,
     detach: Xf,
     init: Wf,
     insert: Zf,
     noop: Ki,
     safe_not_equal: Yf,
     svg_element: Ts
 } = window.__gradio__svelte__internal;
 
 function Jf(t) {
     let e, n;
     return {
         c() {
-            e = Ts("svg"), n = Ts("path"), mn(n, "d", "M23,20a5,5,0,0,0-3.89,1.89L11.8,17.32a4.46,4.46,0,0,0,0-2.64l7.31-4.57A5,5,0,1,0,18,7a4.79,4.79,0,0,0,.2,1.32l-7.31,4.57a5,5,0,1,0,0,6.22l7.31,4.57A4.79,4.79,0,0,0,18,25a5,5,0,1,0,5-5ZM23,4a3,3,0,1,1-3,3A3,3,0,0,1,23,4ZM7,19a3,3,0,1,1,3-3A3,3,0,0,1,7,19Zm16,9a3,3,0,1,1,3-3A3,3,0,0,1,23,28Z"), mn(n, "fill", "currentColor"), mn(e, "id", "icon"), mn(e, "xmlns", "http://www.w3.org/2000/svg"), mn(e, "viewBox", "0 0 32 32");
+            e = Ts("svg"), n = Ts("path"), wn(n, "d", "M23,20a5,5,0,0,0-3.89,1.89L11.8,17.32a4.46,4.46,0,0,0,0-2.64l7.31-4.57A5,5,0,1,0,18,7a4.79,4.79,0,0,0,.2,1.32l-7.31,4.57a5,5,0,1,0,0,6.22l7.31,4.57A4.79,4.79,0,0,0,18,25a5,5,0,1,0,5-5ZM23,4a3,3,0,1,1-3,3A3,3,0,0,1,23,4ZM7,19a3,3,0,1,1,3-3A3,3,0,0,1,7,19Zm16,9a3,3,0,1,1,3-3A3,3,0,0,1,23,28Z"), wn(n, "fill", "currentColor"), wn(e, "id", "icon"), wn(e, "xmlns", "http://www.w3.org/2000/svg"), wn(e, "viewBox", "0 0 32 32");
         },
         m(i, l) {
             Zf(i, e, l), Vf(e, n);
         },
         p: Ki,
         i: Ki,
         o: Ki,
@@ -1252,28 +1252,28 @@
     constructor(e) {
         super(), Wf(this, e, null, Jf, Yf, {});
     }
 }
 const {
     SvelteComponent: Kf,
     append: $f,
-    attr: Ut,
+    attr: qt,
     detach: ec,
     init: tc,
     insert: nc,
     noop: $i,
     safe_not_equal: ic,
     svg_element: Hs
 } = window.__gradio__svelte__internal;
 
 function lc(t) {
     let e, n;
     return {
         c() {
-            e = Hs("svg"), n = Hs("path"), Ut(n, "fill", "currentColor"), Ut(n, "d", "M26 24v4H6v-4H4v4a2 2 0 0 0 2 2h20a2 2 0 0 0 2-2v-4zm0-10l-1.41-1.41L17 20.17V2h-2v18.17l-7.59-7.58L6 14l10 10l10-10z"), Ut(e, "xmlns", "http://www.w3.org/2000/svg"), Ut(e, "width", "100%"), Ut(e, "height", "100%"), Ut(e, "viewBox", "0 0 32 32");
+            e = Hs("svg"), n = Hs("path"), qt(n, "fill", "currentColor"), qt(n, "d", "M26 24v4H6v-4H4v4a2 2 0 0 0 2 2h20a2 2 0 0 0 2-2v-4zm0-10l-1.41-1.41L17 20.17V2h-2v18.17l-7.59-7.58L6 14l10 10l10-10z"), qt(e, "xmlns", "http://www.w3.org/2000/svg"), qt(e, "width", "100%"), qt(e, "height", "100%"), qt(e, "viewBox", "0 0 32 32");
         },
         m(i, l) {
             nc(i, e, l), $f(e, n);
         },
         p: $i,
         i: $i,
         o: $i,
@@ -1286,28 +1286,28 @@
     constructor(e) {
         super(), tc(this, e, null, lc, ic, {});
     }
 }
 const {
     SvelteComponent: oc,
     append: rc,
-    attr: Ft,
+    attr: zt,
     detach: ac,
     init: uc,
     insert: fc,
     noop: el,
     safe_not_equal: cc,
     svg_element: Ps
 } = window.__gradio__svelte__internal;
 
 function _c(t) {
     let e, n;
     return {
         c() {
-            e = Ps("svg"), n = Ps("path"), Ft(n, "d", "M5 8l4 4 4-4z"), Ft(e, "class", "dropdown-arrow svelte-145leq6"), Ft(e, "xmlns", "http://www.w3.org/2000/svg"), Ft(e, "width", "100%"), Ft(e, "height", "100%"), Ft(e, "viewBox", "0 0 18 18");
+            e = Ps("svg"), n = Ps("path"), zt(n, "d", "M5 8l4 4 4-4z"), zt(e, "class", "dropdown-arrow svelte-145leq6"), zt(e, "xmlns", "http://www.w3.org/2000/svg"), zt(e, "width", "100%"), zt(e, "height", "100%"), zt(e, "viewBox", "0 0 18 18");
         },
         m(i, l) {
             fc(i, e, l), rc(e, n);
         },
         p: el,
         i: el,
         o: el,
@@ -1320,28 +1320,28 @@
     constructor(e) {
         super(), uc(this, e, null, _c, cc, {});
     }
 }
 const {
     SvelteComponent: dc,
     append: mc,
-    attr: Fe,
+    attr: Ue,
     detach: gc,
     init: bc,
     insert: pc,
     noop: tl,
     safe_not_equal: wc,
     svg_element: Ns
 } = window.__gradio__svelte__internal;
 
 function vc(t) {
     let e, n;
     return {
         c() {
-            e = Ns("svg"), n = Ns("path"), Fe(n, "d", "M17 3a2.828 2.828 0 1 1 4 4L7.5 20.5 2 22l1.5-5.5L17 3z"), Fe(e, "xmlns", "http://www.w3.org/2000/svg"), Fe(e, "width", "100%"), Fe(e, "height", "100%"), Fe(e, "viewBox", "0 0 24 24"), Fe(e, "fill", "none"), Fe(e, "stroke", "currentColor"), Fe(e, "stroke-width", "1.5"), Fe(e, "stroke-linecap", "round"), Fe(e, "stroke-linejoin", "round"), Fe(e, "class", "feather feather-edit-2");
+            e = Ns("svg"), n = Ns("path"), Ue(n, "d", "M17 3a2.828 2.828 0 1 1 4 4L7.5 20.5 2 22l1.5-5.5L17 3z"), Ue(e, "xmlns", "http://www.w3.org/2000/svg"), Ue(e, "width", "100%"), Ue(e, "height", "100%"), Ue(e, "viewBox", "0 0 24 24"), Ue(e, "fill", "none"), Ue(e, "stroke", "currentColor"), Ue(e, "stroke-width", "1.5"), Ue(e, "stroke-linecap", "round"), Ue(e, "stroke-linejoin", "round"), Ue(e, "class", "feather feather-edit-2");
         },
         m(i, l) {
             pc(i, e, l), mc(e, n);
         },
         p: tl,
         i: tl,
         o: tl,
@@ -1360,22 +1360,22 @@
     append: nl,
     attr: oe,
     detach: kc,
     init: Sc,
     insert: Cc,
     noop: il,
     safe_not_equal: Ac,
-    svg_element: Zn
+    svg_element: Qn
 } = window.__gradio__svelte__internal;
 
 function Bc(t) {
     let e, n, i, l;
     return {
         c() {
-            e = Zn("svg"), n = Zn("rect"), i = Zn("circle"), l = Zn("polyline"), oe(n, "x", "3"), oe(n, "y", "3"), oe(n, "width", "18"), oe(n, "height", "18"), oe(n, "rx", "2"), oe(n, "ry", "2"), oe(i, "cx", "8.5"), oe(i, "cy", "8.5"), oe(i, "r", "1.5"), oe(l, "points", "21 15 16 10 5 21"), oe(e, "xmlns", "http://www.w3.org/2000/svg"), oe(e, "width", "100%"), oe(e, "height", "100%"), oe(e, "viewBox", "0 0 24 24"), oe(e, "fill", "none"), oe(e, "stroke", "currentColor"), oe(e, "stroke-width", "1.5"), oe(e, "stroke-linecap", "round"), oe(e, "stroke-linejoin", "round"), oe(e, "class", "feather feather-image");
+            e = Qn("svg"), n = Qn("rect"), i = Qn("circle"), l = Qn("polyline"), oe(n, "x", "3"), oe(n, "y", "3"), oe(n, "width", "18"), oe(n, "height", "18"), oe(n, "rx", "2"), oe(n, "ry", "2"), oe(i, "cx", "8.5"), oe(i, "cy", "8.5"), oe(i, "r", "1.5"), oe(l, "points", "21 15 16 10 5 21"), oe(e, "xmlns", "http://www.w3.org/2000/svg"), oe(e, "width", "100%"), oe(e, "height", "100%"), oe(e, "viewBox", "0 0 24 24"), oe(e, "fill", "none"), oe(e, "stroke", "currentColor"), oe(e, "stroke-width", "1.5"), oe(e, "stroke-linecap", "round"), oe(e, "stroke-linejoin", "round"), oe(e, "class", "feather feather-image");
         },
         m(s, o) {
             Cc(s, e, o), nl(e, n), nl(e, i), nl(e, l);
         },
         p: il,
         i: il,
         o: il,
@@ -1388,28 +1388,28 @@
     constructor(e) {
         super(), Sc(this, e, null, Bc, Ac, {});
     }
 };
 const {
     SvelteComponent: Tc,
     append: Hc,
-    attr: qt,
+    attr: jt,
     detach: Pc,
     init: Nc,
     insert: Lc,
     noop: ll,
     safe_not_equal: Ic,
     svg_element: Ls
 } = window.__gradio__svelte__internal;
 
 function Mc(t) {
     let e, n;
     return {
         c() {
-            e = Ls("svg"), n = Ls("path"), qt(n, "fill", "currentColor"), qt(n, "d", "M13.75 2a2.25 2.25 0 0 1 2.236 2.002V4h1.764A2.25 2.25 0 0 1 20 6.25V11h-1.5V6.25a.75.75 0 0 0-.75-.75h-2.129c-.404.603-1.091 1-1.871 1h-3.5c-.78 0-1.467-.397-1.871-1H6.25a.75.75 0 0 0-.75.75v13.5c0 .414.336.75.75.75h4.78a3.99 3.99 0 0 0 .505 1.5H6.25A2.25 2.25 0 0 1 4 19.75V6.25A2.25 2.25 0 0 1 6.25 4h1.764a2.25 2.25 0 0 1 2.236-2h3.5Zm2.245 2.096L16 4.25c0-.052-.002-.103-.005-.154ZM13.75 3.5h-3.5a.75.75 0 0 0 0 1.5h3.5a.75.75 0 0 0 0-1.5ZM15 12a3 3 0 0 0-3 3v5c0 .556.151 1.077.415 1.524l3.494-3.494a2.25 2.25 0 0 1 3.182 0l3.494 3.494c.264-.447.415-.968.415-1.524v-5a3 3 0 0 0-3-3h-5Zm0 11a2.985 2.985 0 0 1-1.524-.415l3.494-3.494a.75.75 0 0 1 1.06 0l3.494 3.494A2.985 2.985 0 0 1 20 23h-5Zm5-7a1 1 0 1 1 0-2a1 1 0 0 1 0 2Z"), qt(e, "xmlns", "http://www.w3.org/2000/svg"), qt(e, "width", "100%"), qt(e, "height", "100%"), qt(e, "viewBox", "0 0 24 24");
+            e = Ls("svg"), n = Ls("path"), jt(n, "fill", "currentColor"), jt(n, "d", "M13.75 2a2.25 2.25 0 0 1 2.236 2.002V4h1.764A2.25 2.25 0 0 1 20 6.25V11h-1.5V6.25a.75.75 0 0 0-.75-.75h-2.129c-.404.603-1.091 1-1.871 1h-3.5c-.78 0-1.467-.397-1.871-1H6.25a.75.75 0 0 0-.75.75v13.5c0 .414.336.75.75.75h4.78a3.99 3.99 0 0 0 .505 1.5H6.25A2.25 2.25 0 0 1 4 19.75V6.25A2.25 2.25 0 0 1 6.25 4h1.764a2.25 2.25 0 0 1 2.236-2h3.5Zm2.245 2.096L16 4.25c0-.052-.002-.103-.005-.154ZM13.75 3.5h-3.5a.75.75 0 0 0 0 1.5h3.5a.75.75 0 0 0 0-1.5ZM15 12a3 3 0 0 0-3 3v5c0 .556.151 1.077.415 1.524l3.494-3.494a2.25 2.25 0 0 1 3.182 0l3.494 3.494c.264-.447.415-.968.415-1.524v-5a3 3 0 0 0-3-3h-5Zm0 11a2.985 2.985 0 0 1-1.524-.415l3.494-3.494a.75.75 0 0 1 1.06 0l3.494 3.494A2.985 2.985 0 0 1 20 23h-5Zm5-7a1 1 0 1 1 0-2a1 1 0 0 1 0 2Z"), jt(e, "xmlns", "http://www.w3.org/2000/svg"), jt(e, "width", "100%"), jt(e, "height", "100%"), jt(e, "viewBox", "0 0 24 24");
         },
         m(i, l) {
             Lc(i, e, l), Hc(e, n);
         },
         p: ll,
         i: ll,
         o: ll,
@@ -1421,32 +1421,32 @@
 class Cr extends Tc {
     constructor(e) {
         super(), Nc(this, e, null, Mc, Ic, {});
     }
 }
 const {
     SvelteComponent: Oc,
-    append: Yn,
+    append: Kn,
     attr: re,
     detach: Dc,
     init: Rc,
     insert: Uc,
     noop: sl,
     safe_not_equal: Fc,
-    svg_element: gn
+    svg_element: vn
 } = window.__gradio__svelte__internal;
 
 function qc(t) {
     let e, n, i, l, s;
     return {
         c() {
-            e = gn("svg"), n = gn("path"), i = gn("path"), l = gn("line"), s = gn("line"), re(n, "d", "M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"), re(i, "d", "M19 10v2a7 7 0 0 1-14 0v-2"), re(l, "x1", "12"), re(l, "y1", "19"), re(l, "x2", "12"), re(l, "y2", "23"), re(s, "x1", "8"), re(s, "y1", "23"), re(s, "x2", "16"), re(s, "y2", "23"), re(e, "xmlns", "http://www.w3.org/2000/svg"), re(e, "width", "100%"), re(e, "height", "100%"), re(e, "viewBox", "0 0 24 24"), re(e, "fill", "none"), re(e, "stroke", "currentColor"), re(e, "stroke-width", "2"), re(e, "stroke-linecap", "round"), re(e, "stroke-linejoin", "round"), re(e, "class", "feather feather-mic");
+            e = vn("svg"), n = vn("path"), i = vn("path"), l = vn("line"), s = vn("line"), re(n, "d", "M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"), re(i, "d", "M19 10v2a7 7 0 0 1-14 0v-2"), re(l, "x1", "12"), re(l, "y1", "19"), re(l, "x2", "12"), re(l, "y2", "23"), re(s, "x1", "8"), re(s, "y1", "23"), re(s, "x2", "16"), re(s, "y2", "23"), re(e, "xmlns", "http://www.w3.org/2000/svg"), re(e, "width", "100%"), re(e, "height", "100%"), re(e, "viewBox", "0 0 24 24"), re(e, "fill", "none"), re(e, "stroke", "currentColor"), re(e, "stroke-width", "2"), re(e, "stroke-linecap", "round"), re(e, "stroke-linejoin", "round"), re(e, "class", "feather feather-mic");
         },
         m(o, r) {
-            Uc(o, e, r), Yn(e, n), Yn(e, i), Yn(e, l), Yn(e, s);
+            Uc(o, e, r), Kn(e, n), Kn(e, i), Kn(e, l), Kn(e, s);
         },
         p: sl,
         i: sl,
         o: sl,
         d(o) {
             o && Dc(e);
         }
@@ -1456,28 +1456,28 @@
     constructor(e) {
         super(), Rc(this, e, null, qc, Fc, {});
     }
 }
 const {
     SvelteComponent: jc,
     append: ol,
-    attr: be,
+    attr: ge,
     detach: Gc,
     init: xc,
     insert: Vc,
     noop: rl,
     safe_not_equal: Xc,
-    svg_element: Jn
+    svg_element: $n
 } = window.__gradio__svelte__internal;
 
 function Wc(t) {
     let e, n, i, l;
     return {
         c() {
-            e = Jn("svg"), n = Jn("path"), i = Jn("polyline"), l = Jn("line"), be(n, "d", "M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"), be(i, "points", "17 8 12 3 7 8"), be(l, "x1", "12"), be(l, "y1", "3"), be(l, "x2", "12"), be(l, "y2", "15"), be(e, "xmlns", "http://www.w3.org/2000/svg"), be(e, "width", "90%"), be(e, "height", "90%"), be(e, "viewBox", "0 0 24 24"), be(e, "fill", "none"), be(e, "stroke", "currentColor"), be(e, "stroke-width", "2"), be(e, "stroke-linecap", "round"), be(e, "stroke-linejoin", "round"), be(e, "class", "feather feather-upload");
+            e = $n("svg"), n = $n("path"), i = $n("polyline"), l = $n("line"), ge(n, "d", "M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"), ge(i, "points", "17 8 12 3 7 8"), ge(l, "x1", "12"), ge(l, "y1", "3"), ge(l, "x2", "12"), ge(l, "y2", "15"), ge(e, "xmlns", "http://www.w3.org/2000/svg"), ge(e, "width", "90%"), ge(e, "height", "90%"), ge(e, "viewBox", "0 0 24 24"), ge(e, "fill", "none"), ge(e, "stroke", "currentColor"), ge(e, "stroke-width", "2"), ge(e, "stroke-linecap", "round"), ge(e, "stroke-linejoin", "round"), ge(e, "class", "feather feather-upload");
         },
         m(s, o) {
             Vc(s, e, o), ol(e, n), ol(e, i), ol(e, l);
         },
         p: rl,
         i: rl,
         o: rl,
@@ -1490,28 +1490,28 @@
     constructor(e) {
         super(), xc(this, e, null, Wc, Xc, {});
     }
 };
 const {
     SvelteComponent: Zc,
     append: Is,
-    attr: lt,
+    attr: st,
     detach: Yc,
     init: Jc,
     insert: Qc,
     noop: al,
     safe_not_equal: Kc,
     svg_element: ul
 } = window.__gradio__svelte__internal;
 
 function $c(t) {
     let e, n, i;
     return {
         c() {
-            e = ul("svg"), n = ul("path"), i = ul("path"), lt(n, "fill", "currentColor"), lt(n, "d", "M12 2c-4.963 0-9 4.038-9 9c0 3.328 1.82 6.232 4.513 7.79l-2.067 1.378A1 1 0 0 0 6 22h12a1 1 0 0 0 .555-1.832l-2.067-1.378C19.18 17.232 21 14.328 21 11c0-4.962-4.037-9-9-9zm0 16c-3.859 0-7-3.141-7-7c0-3.86 3.141-7 7-7s7 3.14 7 7c0 3.859-3.141 7-7 7z"), lt(i, "fill", "currentColor"), lt(i, "d", "M12 6c-2.757 0-5 2.243-5 5s2.243 5 5 5s5-2.243 5-5s-2.243-5-5-5zm0 8c-1.654 0-3-1.346-3-3s1.346-3 3-3s3 1.346 3 3s-1.346 3-3 3z"), lt(e, "xmlns", "http://www.w3.org/2000/svg"), lt(e, "width", "100%"), lt(e, "height", "100%"), lt(e, "viewBox", "0 0 24 24");
+            e = ul("svg"), n = ul("path"), i = ul("path"), st(n, "fill", "currentColor"), st(n, "d", "M12 2c-4.963 0-9 4.038-9 9c0 3.328 1.82 6.232 4.513 7.79l-2.067 1.378A1 1 0 0 0 6 22h12a1 1 0 0 0 .555-1.832l-2.067-1.378C19.18 17.232 21 14.328 21 11c0-4.962-4.037-9-9-9zm0 16c-3.859 0-7-3.141-7-7c0-3.86 3.141-7 7-7s7 3.14 7 7c0 3.859-3.141 7-7 7z"), st(i, "fill", "currentColor"), st(i, "d", "M12 6c-2.757 0-5 2.243-5 5s2.243 5 5 5s5-2.243 5-5s-2.243-5-5-5zm0 8c-1.654 0-3-1.346-3-3s1.346-3 3-3s3 1.346 3 3s-1.346 3-3 3z"), st(e, "xmlns", "http://www.w3.org/2000/svg"), st(e, "width", "100%"), st(e, "height", "100%"), st(e, "viewBox", "0 0 24 24");
         },
         m(l, s) {
             Qc(l, e, s), Is(e, n), Is(e, i);
         },
         p: al,
         i: al,
         o: al,
@@ -1881,22 +1881,22 @@
             s = t[i + 1];
         if (i += 2, (l === "optionalAccess" || l === "optionalCall") && n == null)
             return;
         l === "access" || l === "optionalAccess" ? (e = n, n = s(n)) : (l === "call" || l === "optionalCall") && (n = s((...o) => n.call(e, ...o)), e = void 0);
     }
     return n;
 }
-class _i extends Error {
+class mi extends Error {
     constructor(e) {
         super(e), this.name = "ShareError";
     }
 }
 async function i_(t, e) {
     if (window.__gradio_space__ == null)
-        throw new _i("Must be on Spaces to share.");
+        throw new mi("Must be on Spaces to share.");
     let n, i, l;
     if (e === "url") {
         const a = await fetch(t);
         n = await a.blob(), i = a.headers.get("content-type") || "", l = a.headers.get("content-disposition") || "";
     } else
         n = l_(t), i = t.split(";")[0].split(":")[1], l = "file" + i.split("/")[1];
     const s = new File([n], l, {
@@ -1909,17 +1909,17 @@
                 "Content-Type": s.type,
                 "X-Requested-With": "XMLHttpRequest"
             }
         });
     if (!o.ok) {
         if (n_([o, "access", (a) => a.headers, "access", (a) => a.get, "call", (a) => a("content-type"), "optionalAccess", (a) => a.includes, "call", (a) => a("application/json")])) {
             const a = await o.json();
-            throw new _i(`Upload failed: ${a.error}`);
+            throw new mi(`Upload failed: ${a.error}`);
         }
-        throw new _i("Upload failed.");
+        throw new mi("Upload failed.");
     }
     return await o.text();
 }
 
 function l_(t) {
     for (var e = t.split(","), n = e[0].match(/:(.*?);/)[1], i = atob(e[1]), l = i.length, s = new Uint8Array(l); l--;)
         s[l] = i.charCodeAt(l);
@@ -1999,15 +1999,15 @@
             n(3, r = !0);
             const u = await l(s);
             i("share", {
                 description: u
             });
         } catch (u) {
             console.error(u);
-            let f = u instanceof _i ? u.message : "Share failed.";
+            let f = u instanceof mi ? u.message : "Share failed.";
             i("error", f);
         } finally {
             n(3, r = !1);
         }
     };
     return t.$$set = (u) => {
         "formatter" in u && n(0, l = u.formatter), "value" in u && n(1, s = u.value), "i18n" in u && n(2, o = u.i18n);
@@ -2020,48 +2020,48 @@
             value: 1,
             i18n: 2
         });
     }
 }
 const {
     SvelteComponent: b_,
-    append: St,
+    append: Ct,
     attr: Rl,
     check_outros: p_,
     create_component: Br,
     destroy_component: Tr,
-    detach: hi,
+    detach: gi,
     element: Ul,
     group_outros: w_,
     init: v_,
-    insert: di,
+    insert: bi,
     mount_component: Hr,
     safe_not_equal: y_,
     set_data: Fl,
     space: ql,
-    text: yn,
+    text: Cn,
     toggle_class: Os,
-    transition_in: pi,
-    transition_out: wi
+    transition_in: yi,
+    transition_out: Ei
 } = window.__gradio__svelte__internal;
 
 function E_(t) {
     let e, n;
     return e = new Ar({}), {
         c() {
             Br(e.$$.fragment);
         },
         m(i, l) {
             Hr(e, i, l), n = !0;
         },
         i(i) {
-            n || (pi(e.$$.fragment, i), n = !0);
+            n || (yi(e.$$.fragment, i), n = !0);
         },
         o(i) {
-            wi(e.$$.fragment, i), n = !1;
+            Ei(e.$$.fragment, i), n = !1;
         },
         d(i) {
             Tr(e, i);
         }
     };
 }
 
@@ -2071,18 +2071,18 @@
         c() {
             Br(e.$$.fragment);
         },
         m(i, l) {
             Hr(e, i, l), n = !0;
         },
         i(i) {
-            n || (pi(e.$$.fragment, i), n = !0);
+            n || (yi(e.$$.fragment, i), n = !0);
         },
         o(i) {
-            wi(e.$$.fragment, i), n = !1;
+            Ei(e.$$.fragment, i), n = !1;
         },
         d(i) {
             Tr(e, i);
         }
     };
 }
 
@@ -2095,29 +2095,29 @@
             /*message*/
             (t[2] || /*i18n*/
                 t[1]("upload_text.click_to_upload")) + ""
         ),
         a;
     return {
         c() {
-            e = Ul("span"), n = yn("- "), l = yn(i), s = yn(" -"), o = ql(), a = yn(r), Rl(e, "class", "or svelte-kzcjhc");
+            e = Ul("span"), n = Cn("- "), l = Cn(i), s = Cn(" -"), o = ql(), a = Cn(r), Rl(e, "class", "or svelte-kzcjhc");
         },
         m(u, f) {
-            di(u, e, f), St(e, n), St(e, l), St(e, s), di(u, o, f), di(u, a, f);
+            bi(u, e, f), Ct(e, n), Ct(e, l), Ct(e, s), bi(u, o, f), bi(u, a, f);
         },
         p(u, f) {
             f & /*i18n*/
                 2 && i !== (i = /*i18n*/
                     u[1]("common.or") + "") && Fl(l, i), f & /*message, i18n*/
                 6 && r !== (r = /*message*/
                     (u[2] || /*i18n*/
                         u[1]("upload_text.click_to_upload")) + "") && Fl(a, r);
         },
         d(u) {
-            u && (hi(e), hi(o), hi(a));
+            u && (gi(e), gi(o), gi(a));
         }
     };
 }
 
 function S_(t) {
     let e, n, i, l, s, o = (
             /*i18n*/
@@ -2130,67 +2130,67 @@
                 t[5].file
             ) + ""
         ),
         r, a, u;
     const f = [k_, E_],
         _ = [];
 
-    function h(d, m) {
+    function h(d, b) {
         return (
             /*type*/
             d[0] === "clipboard" ? 0 : 1
         );
     }
     i = h(t), l = _[i] = f[i](t);
     let c = (
         /*mode*/
         t[3] !== "short" && Ds(t)
     );
     return {
         c() {
-            e = Ul("div"), n = Ul("span"), l.c(), s = ql(), r = yn(o), a = ql(), c && c.c(), Rl(n, "class", "icon-wrap svelte-kzcjhc"), Os(
+            e = Ul("div"), n = Ul("span"), l.c(), s = ql(), r = Cn(o), a = ql(), c && c.c(), Rl(n, "class", "icon-wrap svelte-kzcjhc"), Os(
                 n,
                 "hovered",
                 /*hovered*/
                 t[4]
             ), Rl(e, "class", "wrap svelte-kzcjhc");
         },
-        m(d, m) {
-            di(d, e, m), St(e, n), _[i].m(n, null), St(e, s), St(e, r), St(e, a), c && c.m(e, null), u = !0;
+        m(d, b) {
+            bi(d, e, b), Ct(e, n), _[i].m(n, null), Ct(e, s), Ct(e, r), Ct(e, a), c && c.m(e, null), u = !0;
         },
-        p(d, [m]) {
-            let b = i;
-            i = h(d), i !== b && (w_(), wi(_[b], 1, 1, () => {
-                    _[b] = null;
-                }), p_(), l = _[i], l || (l = _[i] = f[i](d), l.c()), pi(l, 1), l.m(n, null)), (!u || m & /*hovered*/
+        p(d, [b]) {
+            let p = i;
+            i = h(d), i !== p && (w_(), Ei(_[p], 1, 1, () => {
+                    _[p] = null;
+                }), p_(), l = _[i], l || (l = _[i] = f[i](d), l.c()), yi(l, 1), l.m(n, null)), (!u || b & /*hovered*/
                     16) && Os(
                     n,
                     "hovered",
                     /*hovered*/
                     d[4]
-                ), (!u || m & /*i18n, type*/
+                ), (!u || b & /*i18n, type*/
                     3) && o !== (o = /*i18n*/
                     d[1](
                         /*defs*/
                         d[5][
                             /*type*/
                             d[0]
                         ] || /*defs*/
                         d[5].file
                     ) + "") && Fl(r, o), /*mode*/
-                d[3] !== "short" ? c ? c.p(d, m) : (c = Ds(d), c.c(), c.m(e, null)) : c && (c.d(1), c = null);
+                d[3] !== "short" ? c ? c.p(d, b) : (c = Ds(d), c.c(), c.m(e, null)) : c && (c.d(1), c = null);
         },
         i(d) {
-            u || (pi(l), u = !0);
+            u || (yi(l), u = !0);
         },
         o(d) {
-            wi(l), u = !1;
+            Ei(l), u = !1;
         },
         d(d) {
-            d && hi(e), _[i].d(), c && c.d();
+            d && gi(e), _[i].d(), c && c.d();
         }
     };
 }
 
 function C_(t, e, n) {
     let {
         type: i = "file"
@@ -2227,28 +2227,28 @@
         });
     }
 }
 const {
     SvelteComponent: A_,
     append: fl,
     attr: Ye,
-    check_outros: En,
-    create_component: Li,
-    destroy_component: Ii,
-    detach: fn,
-    element: Un,
+    check_outros: An,
+    create_component: Oi,
+    destroy_component: Di,
+    detach: _n,
+    element: jn,
     empty: B_,
-    group_outros: kn,
+    group_outros: Bn,
     init: T_,
-    insert: cn,
-    listen: Mi,
-    mount_component: Oi,
+    insert: hn,
+    listen: Ri,
+    mount_component: Ui,
     safe_not_equal: H_,
     space: cl,
-    toggle_class: ct,
+    toggle_class: _t,
     transition_in: fe,
     transition_out: Ae
 } = window.__gradio__svelte__internal;
 
 function Rs(t) {
     let e, n = (
             /*sources*/
@@ -2268,243 +2268,243 @@
         ),
         u, f = n && Us(t),
         _ = l && Fs(t),
         h = o && qs(t),
         c = a && zs(t);
     return {
         c() {
-            e = Un("span"), f && f.c(), i = cl(), _ && _.c(), s = cl(), h && h.c(), r = cl(), c && c.c(), Ye(e, "class", "source-selection svelte-1jp3vgd"), Ye(e, "data-testid", "source-select");
+            e = jn("span"), f && f.c(), i = cl(), _ && _.c(), s = cl(), h && h.c(), r = cl(), c && c.c(), Ye(e, "class", "source-selection svelte-1jp3vgd"), Ye(e, "data-testid", "source-select");
         },
-        m(d, m) {
-            cn(d, e, m), f && f.m(e, null), fl(e, i), _ && _.m(e, null), fl(e, s), h && h.m(e, null), fl(e, r), c && c.m(e, null), u = !0;
+        m(d, b) {
+            hn(d, e, b), f && f.m(e, null), fl(e, i), _ && _.m(e, null), fl(e, s), h && h.m(e, null), fl(e, r), c && c.m(e, null), u = !0;
         },
-        p(d, m) {
-            m & /*sources*/
+        p(d, b) {
+            b & /*sources*/
                 2 && (n = /*sources*/
-                    d[1].includes("upload")), n ? f ? (f.p(d, m), m & /*sources*/
-                    2 && fe(f, 1)) : (f = Us(d), f.c(), fe(f, 1), f.m(e, i)) : f && (kn(), Ae(f, 1, 1, () => {
+                    d[1].includes("upload")), n ? f ? (f.p(d, b), b & /*sources*/
+                    2 && fe(f, 1)) : (f = Us(d), f.c(), fe(f, 1), f.m(e, i)) : f && (Bn(), Ae(f, 1, 1, () => {
                     f = null;
-                }), En()), m & /*sources*/
+                }), An()), b & /*sources*/
                 2 && (l = /*sources*/
-                    d[1].includes("microphone")), l ? _ ? (_.p(d, m), m & /*sources*/
-                    2 && fe(_, 1)) : (_ = Fs(d), _.c(), fe(_, 1), _.m(e, s)) : _ && (kn(), Ae(_, 1, 1, () => {
+                    d[1].includes("microphone")), l ? _ ? (_.p(d, b), b & /*sources*/
+                    2 && fe(_, 1)) : (_ = Fs(d), _.c(), fe(_, 1), _.m(e, s)) : _ && (Bn(), Ae(_, 1, 1, () => {
                     _ = null;
-                }), En()), m & /*sources*/
+                }), An()), b & /*sources*/
                 2 && (o = /*sources*/
-                    d[1].includes("webcam")), o ? h ? (h.p(d, m), m & /*sources*/
-                    2 && fe(h, 1)) : (h = qs(d), h.c(), fe(h, 1), h.m(e, r)) : h && (kn(), Ae(h, 1, 1, () => {
+                    d[1].includes("webcam")), o ? h ? (h.p(d, b), b & /*sources*/
+                    2 && fe(h, 1)) : (h = qs(d), h.c(), fe(h, 1), h.m(e, r)) : h && (Bn(), Ae(h, 1, 1, () => {
                     h = null;
-                }), En()), m & /*sources*/
+                }), An()), b & /*sources*/
                 2 && (a = /*sources*/
-                    d[1].includes("clipboard")), a ? c ? (c.p(d, m), m & /*sources*/
-                    2 && fe(c, 1)) : (c = zs(d), c.c(), fe(c, 1), c.m(e, null)) : c && (kn(), Ae(c, 1, 1, () => {
+                    d[1].includes("clipboard")), a ? c ? (c.p(d, b), b & /*sources*/
+                    2 && fe(c, 1)) : (c = zs(d), c.c(), fe(c, 1), c.m(e, null)) : c && (Bn(), Ae(c, 1, 1, () => {
                     c = null;
-                }), En());
+                }), An());
         },
         i(d) {
             u || (fe(f), fe(_), fe(h), fe(c), u = !0);
         },
         o(d) {
             Ae(f), Ae(_), Ae(h), Ae(c), u = !1;
         },
         d(d) {
-            d && fn(e), f && f.d(), _ && _.d(), h && h.d(), c && c.d();
+            d && _n(e), f && f.d(), _ && _.d(), h && h.d(), c && c.d();
         }
     };
 }
 
 function Us(t) {
     let e, n, i, l, s;
     return n = new Ar({}), {
         c() {
-            e = Un("button"), Li(n.$$.fragment), Ye(e, "class", "icon svelte-1jp3vgd"), Ye(e, "aria-label", "Upload file"), ct(
+            e = jn("button"), Oi(n.$$.fragment), Ye(e, "class", "icon svelte-1jp3vgd"), Ye(e, "aria-label", "Upload file"), _t(
                 e,
                 "selected",
                 /*active_source*/
                 t[0] === "upload" || ! /*active_source*/
                 t[0]
             );
         },
         m(o, r) {
-            cn(o, e, r), Oi(n, e, null), i = !0, l || (s = Mi(
+            hn(o, e, r), Ui(n, e, null), i = !0, l || (s = Ri(
                 e,
                 "click",
                 /*click_handler*/
                 t[6]
             ), l = !0);
         },
         p(o, r) {
             (!i || r & /*active_source*/
-                1) && ct(
+                1) && _t(
                 e,
                 "selected",
                 /*active_source*/
                 o[0] === "upload" || ! /*active_source*/
                 o[0]
             );
         },
         i(o) {
             i || (fe(n.$$.fragment, o), i = !0);
         },
         o(o) {
             Ae(n.$$.fragment, o), i = !1;
         },
         d(o) {
-            o && fn(e), Ii(n), l = !1, s();
+            o && _n(e), Di(n), l = !1, s();
         }
     };
 }
 
 function Fs(t) {
     let e, n, i, l, s;
     return n = new zc({}), {
         c() {
-            e = Un("button"), Li(n.$$.fragment), Ye(e, "class", "icon svelte-1jp3vgd"), Ye(e, "aria-label", "Record audio"), ct(
+            e = jn("button"), Oi(n.$$.fragment), Ye(e, "class", "icon svelte-1jp3vgd"), Ye(e, "aria-label", "Record audio"), _t(
                 e,
                 "selected",
                 /*active_source*/
                 t[0] === "microphone"
             );
         },
         m(o, r) {
-            cn(o, e, r), Oi(n, e, null), i = !0, l || (s = Mi(
+            hn(o, e, r), Ui(n, e, null), i = !0, l || (s = Ri(
                 e,
                 "click",
                 /*click_handler_1*/
                 t[7]
             ), l = !0);
         },
         p(o, r) {
             (!i || r & /*active_source*/
-                1) && ct(
+                1) && _t(
                 e,
                 "selected",
                 /*active_source*/
                 o[0] === "microphone"
             );
         },
         i(o) {
             i || (fe(n.$$.fragment, o), i = !0);
         },
         o(o) {
             Ae(n.$$.fragment, o), i = !1;
         },
         d(o) {
-            o && fn(e), Ii(n), l = !1, s();
+            o && _n(e), Di(n), l = !1, s();
         }
     };
 }
 
 function qs(t) {
     let e, n, i, l, s;
     return n = new e_({}), {
         c() {
-            e = Un("button"), Li(n.$$.fragment), Ye(e, "class", "icon svelte-1jp3vgd"), Ye(e, "aria-label", "Capture from camera"), ct(
+            e = jn("button"), Oi(n.$$.fragment), Ye(e, "class", "icon svelte-1jp3vgd"), Ye(e, "aria-label", "Capture from camera"), _t(
                 e,
                 "selected",
                 /*active_source*/
                 t[0] === "webcam"
             );
         },
         m(o, r) {
-            cn(o, e, r), Oi(n, e, null), i = !0, l || (s = Mi(
+            hn(o, e, r), Ui(n, e, null), i = !0, l || (s = Ri(
                 e,
                 "click",
                 /*click_handler_2*/
                 t[8]
             ), l = !0);
         },
         p(o, r) {
             (!i || r & /*active_source*/
-                1) && ct(
+                1) && _t(
                 e,
                 "selected",
                 /*active_source*/
                 o[0] === "webcam"
             );
         },
         i(o) {
             i || (fe(n.$$.fragment, o), i = !0);
         },
         o(o) {
             Ae(n.$$.fragment, o), i = !1;
         },
         d(o) {
-            o && fn(e), Ii(n), l = !1, s();
+            o && _n(e), Di(n), l = !1, s();
         }
     };
 }
 
 function zs(t) {
     let e, n, i, l, s;
     return n = new Cr({}), {
         c() {
-            e = Un("button"), Li(n.$$.fragment), Ye(e, "class", "icon svelte-1jp3vgd"), Ye(e, "aria-label", "Paste from clipboard"), ct(
+            e = jn("button"), Oi(n.$$.fragment), Ye(e, "class", "icon svelte-1jp3vgd"), Ye(e, "aria-label", "Paste from clipboard"), _t(
                 e,
                 "selected",
                 /*active_source*/
                 t[0] === "clipboard"
             );
         },
         m(o, r) {
-            cn(o, e, r), Oi(n, e, null), i = !0, l || (s = Mi(
+            hn(o, e, r), Ui(n, e, null), i = !0, l || (s = Ri(
                 e,
                 "click",
                 /*click_handler_3*/
                 t[9]
             ), l = !0);
         },
         p(o, r) {
             (!i || r & /*active_source*/
-                1) && ct(
+                1) && _t(
                 e,
                 "selected",
                 /*active_source*/
                 o[0] === "clipboard"
             );
         },
         i(o) {
             i || (fe(n.$$.fragment, o), i = !0);
         },
         o(o) {
             Ae(n.$$.fragment, o), i = !1;
         },
         d(o) {
-            o && fn(e), Ii(n), l = !1, s();
+            o && _n(e), Di(n), l = !1, s();
         }
     };
 }
 
 function P_(t) {
     let e, n, i = (
         /*unique_sources*/
         t[2].length > 1 && Rs(t)
     );
     return {
         c() {
             i && i.c(), e = B_();
         },
         m(l, s) {
-            i && i.m(l, s), cn(l, e, s), n = !0;
+            i && i.m(l, s), hn(l, e, s), n = !0;
         },
         p(l, [s]) {
             /*unique_sources*/
             l[2].length > 1 ? i ? (i.p(l, s), s & /*unique_sources*/
-                4 && fe(i, 1)) : (i = Rs(l), i.c(), fe(i, 1), i.m(e.parentNode, e)) : i && (kn(), Ae(i, 1, 1, () => {
+                4 && fe(i, 1)) : (i = Rs(l), i.c(), fe(i, 1), i.m(e.parentNode, e)) : i && (Bn(), Ae(i, 1, 1, () => {
                 i = null;
-            }), En());
+            }), An());
         },
         i(l) {
             n || (fe(i), n = !0);
         },
         o(l) {
             Ae(i), n = !1;
         },
         d(l) {
-            l && fn(e), i && i.d(l);
+            l && _n(e), i && i.d(l);
         }
     };
 }
 
 function N_(t, e, n) {
     let i, {
             sources: l
@@ -2550,24 +2550,24 @@
             active_source: 0,
             handle_clear: 4,
             handle_select: 5
         });
     }
 }
 
-function Kt(t) {
+function en(t) {
     let e = ["", "k", "M", "G", "T", "P", "E", "Z"],
         n = 0;
     for (; t > 1e3 && n < e.length - 1;)
         t /= 1e3, n++;
     let i = e[n];
     return (Number.isInteger(t) ? t : t.toFixed(1)) + i;
 }
 
-function Ht() {}
+function Pt() {}
 
 function I_(t) {
     return t();
 }
 
 function M_(t) {
     t.forEach(I_);
@@ -2581,15 +2581,15 @@
     return t != t ? e == e : t !== e || t && typeof t == "object" || typeof t == "function";
 }
 
 function R_(t, ...e) {
     if (t == null) {
         for (const i of e)
             i(void 0);
-        return Ht;
+        return Pt;
     }
     const n = t.subscribe(...e);
     return n.unsubscribe ? () => n.unsubscribe() : n;
 }
 
 function js(t) {
     const e = typeof t == "string" && t.match(/^\s*(-?[\d.]+)([^\s]*)\s*$/);
@@ -2597,34 +2597,34 @@
         /** @type {number} */
         t,
         "px"
     ];
 }
 const Nr = typeof window < "u";
 let Gs = Nr ? () => window.performance.now() : () => Date.now(),
-    Lr = Nr ? (t) => requestAnimationFrame(t) : Ht;
-const nn = /* @__PURE__ */ new Set();
+    Lr = Nr ? (t) => requestAnimationFrame(t) : Pt;
+const sn = /* @__PURE__ */ new Set();
 
 function Ir(t) {
-    nn.forEach((e) => {
-        e.c(t) || (nn.delete(e), e.f());
-    }), nn.size !== 0 && Lr(Ir);
+    sn.forEach((e) => {
+        e.c(t) || (sn.delete(e), e.f());
+    }), sn.size !== 0 && Lr(Ir);
 }
 
 function U_(t) {
     let e;
-    return nn.size === 0 && Lr(Ir), {
+    return sn.size === 0 && Lr(Ir), {
         promise: new Promise((n) => {
-            nn.add(e = {
+            sn.add(e = {
                 c: t,
                 f: n
             });
         }),
         abort() {
-            nn.delete(e);
+            sn.delete(e);
         }
     };
 }
 
 function F_(t) {
     const e = t - 1;
     return e * e * e + 1;
@@ -2644,87 +2644,87 @@
         f = a * (1 - o),
         [_, h] = js(l),
         [c, d] = js(s);
     return {
         delay: e,
         duration: n,
         easing: i,
-        css: (m, b) => `
-			transform: ${u} translate(${(1 - m) * _}${h}, ${(1 - m) * c}${d});
-			opacity: ${a - f * b}`
+        css: (b, p) => `
+			transform: ${u} translate(${(1 - b) * _}${h}, ${(1 - b) * c}${d});
+			opacity: ${a - f * p}`
     };
 }
-const zt = [];
+const Gt = [];
 
 function q_(t, e) {
     return {
-        subscribe: Fn(t, e).subscribe
+        subscribe: Gn(t, e).subscribe
     };
 }
 
-function Fn(t, e = Ht) {
+function Gn(t, e = Pt) {
     let n;
     const i = /* @__PURE__ */ new Set();
 
     function l(r) {
         if (D_(t, r) && (t = r, n)) {
-            const a = !zt.length;
+            const a = !Gt.length;
             for (const u of i)
-                u[1](), zt.push(u, t);
+                u[1](), Gt.push(u, t);
             if (a) {
-                for (let u = 0; u < zt.length; u += 2)
-                    zt[u][0](zt[u + 1]);
-                zt.length = 0;
+                for (let u = 0; u < Gt.length; u += 2)
+                    Gt[u][0](Gt[u + 1]);
+                Gt.length = 0;
             }
         }
     }
 
     function s(r) {
         l(r(t));
     }
 
-    function o(r, a = Ht) {
+    function o(r, a = Pt) {
         const u = [r, a];
-        return i.add(u), i.size === 1 && (n = e(l, s) || Ht), r(t), () => {
+        return i.add(u), i.size === 1 && (n = e(l, s) || Pt), r(t), () => {
             i.delete(u), i.size === 0 && n && (n(), n = null);
         };
     }
     return {
         set: l,
         update: s,
         subscribe: o
     };
 }
 
-function _n(t, e, n) {
+function dn(t, e, n) {
     const i = !Array.isArray(t),
         l = i ? [t] : t;
     if (!l.every(Boolean))
         throw new Error("derived() expects stores as input, got a falsy value");
     const s = e.length < 2;
     return q_(n, (o, r) => {
         let a = !1;
         const u = [];
         let f = 0,
-            _ = Ht;
+            _ = Pt;
         const h = () => {
                 if (f)
                     return;
                 _();
                 const d = e(i ? u[0] : u, o, r);
-                s ? o(d) : _ = O_(d) ? d : Ht;
+                s ? o(d) : _ = O_(d) ? d : Pt;
             },
             c = l.map(
-                (d, m) => R_(
+                (d, b) => R_(
                     d,
-                    (b) => {
-                        u[m] = b, f &= ~(1 << m), a && h();
+                    (p) => {
+                        u[b] = p, f &= ~(1 << b), a && h();
                     },
                     () => {
-                        f |= 1 << m;
+                        f |= 1 << b;
                     }
                 )
             );
         return a = !0, h(),
             function() {
                 M_(c), _(), a = !1;
             };
@@ -2756,99 +2756,99 @@
             return l;
         } else
             throw new Error(`Cannot spring ${typeof n} values`);
     }
 }
 
 function Xs(t, e = {}) {
-    const n = Fn(t),
+    const n = Gn(t),
         {
             stiffness: i = 0.15,
             damping: l = 0.8,
             precision: s = 0.01
         } = e;
     let o, r, a, u = t,
         f = t,
         _ = 1,
         h = 0,
         c = !1;
 
-    function d(b, p = {}) {
-        f = b;
+    function d(p, g = {}) {
+        f = p;
         const y = a = {};
-        return t == null || p.hard || m.stiffness >= 1 && m.damping >= 1 ? (c = !0, o = Gs(), u = b, n.set(t = f), Promise.resolve()) : (p.soft && (h = 1 / ((p.soft === !0 ? 0.5 : +p.soft) * 60), _ = 0), r || (o = Gs(), c = !1, r = U_((w) => {
+        return t == null || g.hard || b.stiffness >= 1 && b.damping >= 1 ? (c = !0, o = Gs(), u = p, n.set(t = f), Promise.resolve()) : (g.soft && (h = 1 / ((g.soft === !0 ? 0.5 : +g.soft) * 60), _ = 0), r || (o = Gs(), c = !1, r = U_((w) => {
             if (c)
                 return c = !1, r = null, !1;
             _ = Math.min(_ + h, 1);
             const C = {
                     inv_mass: _,
-                    opts: m,
+                    opts: b,
                     settled: !0,
                     dt: (w - o) * 60 / 1e3
                 },
                 P = zl(C, u, t, f);
             return o = w, u = t, n.set(t = P), C.settled && (r = null), !C.settled;
         })), new Promise((w) => {
             r.promise.then(() => {
                 y === a && w();
             });
         }));
     }
-    const m = {
+    const b = {
         set: d,
-        update: (b, p) => d(b(f, t), p),
+        update: (p, g) => d(p(f, t), g),
         subscribe: n.subscribe,
         stiffness: i,
         damping: l,
         precision: s
     };
-    return m;
+    return b;
 }
 const {
     SvelteComponent: z_,
-    append: qe,
+    append: Fe,
     attr: z,
     component_subscribe: Ws,
     detach: j_,
     element: G_,
     init: x_,
     insert: V_,
     noop: Zs,
     safe_not_equal: X_,
-    set_style: Qn,
-    svg_element: ze,
+    set_style: ei,
+    svg_element: qe,
     toggle_class: Ys
 } = window.__gradio__svelte__internal, {
     onMount: W_
 } = window.__gradio__svelte__internal;
 
 function Z_(t) {
     let e, n, i, l, s, o, r, a, u, f, _, h;
     return {
         c() {
-            e = G_("div"), n = ze("svg"), i = ze("g"), l = ze("path"), s = ze("path"), o = ze("path"), r = ze("path"), a = ze("g"), u = ze("path"), f = ze("path"), _ = ze("path"), h = ze("path"), z(l, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), z(l, "fill", "#FF7C00"), z(l, "fill-opacity", "0.4"), z(l, "class", "svelte-43sxxs"), z(s, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), z(s, "fill", "#FF7C00"), z(s, "class", "svelte-43sxxs"), z(o, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), z(o, "fill", "#FF7C00"), z(o, "fill-opacity", "0.4"), z(o, "class", "svelte-43sxxs"), z(r, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), z(r, "fill", "#FF7C00"), z(r, "class", "svelte-43sxxs"), Qn(i, "transform", "translate(" + /*$top*/
+            e = G_("div"), n = qe("svg"), i = qe("g"), l = qe("path"), s = qe("path"), o = qe("path"), r = qe("path"), a = qe("g"), u = qe("path"), f = qe("path"), _ = qe("path"), h = qe("path"), z(l, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), z(l, "fill", "#FF7C00"), z(l, "fill-opacity", "0.4"), z(l, "class", "svelte-43sxxs"), z(s, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), z(s, "fill", "#FF7C00"), z(s, "class", "svelte-43sxxs"), z(o, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), z(o, "fill", "#FF7C00"), z(o, "fill-opacity", "0.4"), z(o, "class", "svelte-43sxxs"), z(r, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), z(r, "fill", "#FF7C00"), z(r, "class", "svelte-43sxxs"), ei(i, "transform", "translate(" + /*$top*/
                 t[1][0] + "px, " + /*$top*/
-                t[1][1] + "px)"), z(u, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), z(u, "fill", "#FF7C00"), z(u, "fill-opacity", "0.4"), z(u, "class", "svelte-43sxxs"), z(f, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), z(f, "fill", "#FF7C00"), z(f, "class", "svelte-43sxxs"), z(_, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), z(_, "fill", "#FF7C00"), z(_, "fill-opacity", "0.4"), z(_, "class", "svelte-43sxxs"), z(h, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), z(h, "fill", "#FF7C00"), z(h, "class", "svelte-43sxxs"), Qn(a, "transform", "translate(" + /*$bottom*/
+                t[1][1] + "px)"), z(u, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), z(u, "fill", "#FF7C00"), z(u, "fill-opacity", "0.4"), z(u, "class", "svelte-43sxxs"), z(f, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), z(f, "fill", "#FF7C00"), z(f, "class", "svelte-43sxxs"), z(_, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), z(_, "fill", "#FF7C00"), z(_, "fill-opacity", "0.4"), z(_, "class", "svelte-43sxxs"), z(h, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), z(h, "fill", "#FF7C00"), z(h, "class", "svelte-43sxxs"), ei(a, "transform", "translate(" + /*$bottom*/
                 t[2][0] + "px, " + /*$bottom*/
                 t[2][1] + "px)"), z(n, "viewBox", "-1200 -1200 3000 3000"), z(n, "fill", "none"), z(n, "xmlns", "http://www.w3.org/2000/svg"), z(n, "class", "svelte-43sxxs"), z(e, "class", "svelte-43sxxs"), Ys(
                 e,
                 "margin",
                 /*margin*/
                 t[0]
             );
         },
         m(c, d) {
-            V_(c, e, d), qe(e, n), qe(n, i), qe(i, l), qe(i, s), qe(i, o), qe(i, r), qe(n, a), qe(a, u), qe(a, f), qe(a, _), qe(a, h);
+            V_(c, e, d), Fe(e, n), Fe(n, i), Fe(i, l), Fe(i, s), Fe(i, o), Fe(i, r), Fe(n, a), Fe(a, u), Fe(a, f), Fe(a, _), Fe(a, h);
         },
         p(c, [d]) {
             d & /*$top*/
-                2 && Qn(i, "transform", "translate(" + /*$top*/
+                2 && ei(i, "transform", "translate(" + /*$top*/
                     c[1][0] + "px, " + /*$top*/
                     c[1][1] + "px)"), d & /*$bottom*/
-                4 && Qn(a, "transform", "translate(" + /*$bottom*/
+                4 && ei(a, "transform", "translate(" + /*$bottom*/
                     c[2][0] + "px, " + /*$bottom*/
                     c[2][1] + "px)"), d & /*margin*/
                 1 && Ys(
                     e,
                     "margin",
                     /*margin*/
                     c[0]
@@ -2889,41 +2889,41 @@
         super(), x_(this, e, Y_, Z_, X_, {
             margin: 0
         });
     }
 }
 const {
     SvelteComponent: Q_,
-    append: Ct,
+    append: At,
     attr: We,
     binding_callbacks: Js,
     check_outros: Mr,
     create_component: K_,
     create_slot: $_,
     destroy_component: eh,
     destroy_each: Or,
-    detach: M,
+    detach: O,
     element: Ke,
-    empty: hn,
-    ensure_array_like: vi,
+    empty: mn,
+    ensure_array_like: ki,
     get_all_dirty_from_scope: th,
     get_slot_changes: nh,
     group_outros: Dr,
     init: ih,
-    insert: O,
+    insert: D,
     mount_component: lh,
     noop: jl,
     safe_not_equal: sh,
-    set_data: Re,
-    set_style: at,
+    set_data: De,
+    set_style: ut,
     space: Ze,
     text: le,
-    toggle_class: De,
-    transition_in: ln,
-    transition_out: sn,
+    toggle_class: Oe,
+    transition_in: on,
+    transition_out: rn,
     update_slot_base: oh
 } = window.__gradio__svelte__internal, {
     tick: rh
 } = window.__gradio__svelte__internal, {
     onDestroy: ah
 } = window.__gradio__svelte__internal, uh = (t) => ({}), Qs = (t) => ({});
 
@@ -2955,20 +2955,20 @@
             Qs
         );
     return {
         c() {
             e = Ke("span"), i = le(n), l = Ze(), r && r.c(), We(e, "class", "error svelte-1yserjw");
         },
         m(a, u) {
-            O(a, e, u), Ct(e, i), O(a, l, u), r && r.m(a, u), s = !0;
+            D(a, e, u), At(e, i), D(a, l, u), r && r.m(a, u), s = !0;
         },
         p(a, u) {
             (!s || u[0] & /*i18n*/
                 2) && n !== (n = /*i18n*/
-                a[1]("common.error") + "") && Re(i, n), r && r.p && (!s || u[0] & /*$$scope*/
+                a[1]("common.error") + "") && De(i, n), r && r.p && (!s || u[0] & /*$$scope*/
                 268435456) && oh(
                 r,
                 o,
                 a,
                 /*$$scope*/
                 a[28],
                 s ? nh(
@@ -2981,21 +2981,21 @@
                     /*$$scope*/
                     a[28]
                 ),
                 Qs
             );
         },
         i(a) {
-            s || (ln(r, a), s = !0);
+            s || (on(r, a), s = !0);
         },
         o(a) {
-            sn(r, a), s = !1;
+            rn(r, a), s = !1;
         },
         d(a) {
-            a && (M(e), M(l)), r && r.d(a);
+            a && (O(e), O(l)), r && r.d(a);
         }
     };
 }
 
 function ch(t) {
     let e, n, i, l, s, o, r, a, u, f = (
         /*variant*/
@@ -3025,115 +3025,115 @@
     }
     let h = _(t),
         c = h && h(t),
         d = (
             /*timer*/
             t[5] && io(t)
         );
-    const m = [ph, bh],
-        b = [];
+    const b = [ph, bh],
+        p = [];
 
-    function p(w, C) {
+    function g(w, C) {
         return (
             /*last_progress_level*/
             w[15] != null ? 0 : (
                 /*show_progress*/
                 w[6] === "full" ? 1 : -1
             )
         );
     }
-    ~(s = p(t)) && (o = b[s] = m[s](t));
+    ~(s = g(t)) && (o = p[s] = b[s](t));
     let y = ! /*timer*/
         t[5] && fo(t);
     return {
         c() {
-            f && f.c(), e = Ze(), n = Ke("div"), c && c.c(), i = Ze(), d && d.c(), l = Ze(), o && o.c(), r = Ze(), y && y.c(), a = hn(), We(n, "class", "progress-text svelte-1yserjw"), De(
+            f && f.c(), e = Ze(), n = Ke("div"), c && c.c(), i = Ze(), d && d.c(), l = Ze(), o && o.c(), r = Ze(), y && y.c(), a = mn(), We(n, "class", "progress-text svelte-1yserjw"), Oe(
                 n,
                 "meta-text-center",
                 /*variant*/
                 t[8] === "center"
-            ), De(
+            ), Oe(
                 n,
                 "meta-text",
                 /*variant*/
                 t[8] === "default"
             );
         },
         m(w, C) {
-            f && f.m(w, C), O(w, e, C), O(w, n, C), c && c.m(n, null), Ct(n, i), d && d.m(n, null), O(w, l, C), ~s && b[s].m(w, C), O(w, r, C), y && y.m(w, C), O(w, a, C), u = !0;
+            f && f.m(w, C), D(w, e, C), D(w, n, C), c && c.m(n, null), At(n, i), d && d.m(n, null), D(w, l, C), ~s && p[s].m(w, C), D(w, r, C), y && y.m(w, C), D(w, a, C), u = !0;
         },
         p(w, C) {
             /*variant*/
             w[8] === "default" && /*show_eta_bar*/
                 w[18] && /*show_progress*/
                 w[6] === "full" ? f ? f.p(w, C) : (f = eo(w), f.c(), f.m(e.parentNode, e)) : f && (f.d(1), f = null), h === (h = _(w)) && c ? c.p(w, C) : (c && c.d(1), c = h && h(w), c && (c.c(), c.m(n, i))), /*timer*/
                 w[5] ? d ? d.p(w, C) : (d = io(w), d.c(), d.m(n, null)) : d && (d.d(1), d = null), (!u || C[0] & /*variant*/
-                    256) && De(
+                    256) && Oe(
                     n,
                     "meta-text-center",
                     /*variant*/
                     w[8] === "center"
                 ), (!u || C[0] & /*variant*/
-                    256) && De(
+                    256) && Oe(
                     n,
                     "meta-text",
                     /*variant*/
                     w[8] === "default"
                 );
             let P = s;
-            s = p(w), s === P ? ~s && b[s].p(w, C) : (o && (Dr(), sn(b[P], 1, 1, () => {
-                    b[P] = null;
-                }), Mr()), ~s ? (o = b[s], o ? o.p(w, C) : (o = b[s] = m[s](w), o.c()), ln(o, 1), o.m(r.parentNode, r)) : o = null), /*timer*/
+            s = g(w), s === P ? ~s && p[s].p(w, C) : (o && (Dr(), rn(p[P], 1, 1, () => {
+                    p[P] = null;
+                }), Mr()), ~s ? (o = p[s], o ? o.p(w, C) : (o = p[s] = b[s](w), o.c()), on(o, 1), o.m(r.parentNode, r)) : o = null), /*timer*/
                 w[5] ? y && (y.d(1), y = null) : y ? y.p(w, C) : (y = fo(w), y.c(), y.m(a.parentNode, a));
         },
         i(w) {
-            u || (ln(o), u = !0);
+            u || (on(o), u = !0);
         },
         o(w) {
-            sn(o), u = !1;
+            rn(o), u = !1;
         },
         d(w) {
-            w && (M(e), M(n), M(l), M(r), M(a)), f && f.d(w), c && c.d(), d && d.d(), ~s && b[s].d(w), y && y.d(w);
+            w && (O(e), O(n), O(l), O(r), O(a)), f && f.d(w), c && c.d(), d && d.d(), ~s && p[s].d(w), y && y.d(w);
         }
     };
 }
 
 function eo(t) {
     let e, n = `translateX(${/*eta_level*/
   (t[17] || 0) * 100 - 100}%)`;
     return {
         c() {
-            e = Ke("div"), We(e, "class", "eta-bar svelte-1yserjw"), at(e, "transform", n);
+            e = Ke("div"), We(e, "class", "eta-bar svelte-1yserjw"), ut(e, "transform", n);
         },
         m(i, l) {
-            O(i, e, l);
+            D(i, e, l);
         },
         p(i, l) {
             l[0] & /*eta_level*/
                 131072 && n !== (n = `translateX(${/*eta_level*/
-      (i[17] || 0) * 100 - 100}%)`) && at(e, "transform", n);
+      (i[17] || 0) * 100 - 100}%)`) && ut(e, "transform", n);
         },
         d(i) {
-            i && M(e);
+            i && O(e);
         }
     };
 }
 
 function _h(t) {
     let e;
     return {
         c() {
             e = le("processing |");
         },
         m(n, i) {
-            O(n, e, i);
+            D(n, e, i);
         },
         p: jl,
         d(n) {
-            n && M(e);
+            n && O(e);
         }
     };
 }
 
 function hh(t) {
     let e, n = (
             /*queue_position*/
@@ -3144,70 +3144,70 @@
         c() {
             e = le("queue: "), i = le(n), l = le("/"), s = le(
                 /*queue_size*/
                 t[3]
             ), o = le(" |");
         },
         m(r, a) {
-            O(r, e, a), O(r, i, a), O(r, l, a), O(r, s, a), O(r, o, a);
+            D(r, e, a), D(r, i, a), D(r, l, a), D(r, s, a), D(r, o, a);
         },
         p(r, a) {
             a[0] & /*queue_position*/
                 4 && n !== (n = /*queue_position*/
-                    r[2] + 1 + "") && Re(i, n), a[0] & /*queue_size*/
-                8 && Re(
+                    r[2] + 1 + "") && De(i, n), a[0] & /*queue_size*/
+                8 && De(
                     s,
                     /*queue_size*/
                     r[3]
                 );
         },
         d(r) {
-            r && (M(e), M(i), M(l), M(s), M(o));
+            r && (O(e), O(i), O(l), O(s), O(o));
         }
     };
 }
 
 function dh(t) {
-    let e, n = vi(
+    let e, n = ki(
             /*progress*/
             t[7]
         ),
         i = [];
     for (let l = 0; l < n.length; l += 1)
         i[l] = no($s(t, n, l));
     return {
         c() {
             for (let l = 0; l < i.length; l += 1)
                 i[l].c();
-            e = hn();
+            e = mn();
         },
         m(l, s) {
             for (let o = 0; o < i.length; o += 1)
                 i[o] && i[o].m(l, s);
-            O(l, e, s);
+            D(l, e, s);
         },
         p(l, s) {
             if (s[0] & /*progress*/
                 128) {
-                n = vi(
+                n = ki(
                     /*progress*/
                     l[7]
                 );
                 let o;
                 for (o = 0; o < n.length; o += 1) {
                     const r = $s(l, n, o);
                     i[o] ? i[o].p(r, s) : (i[o] = no(r), i[o].c(), i[o].m(e.parentNode, e));
                 }
                 for (; o < i.length; o += 1)
                     i[o].d(1);
                 i.length = n.length;
             }
         },
         d(l) {
-            l && M(e), Or(i, l);
+            l && O(e), Or(i, l);
         }
     };
 }
 
 function to(t) {
     let e, n = (
             /*p*/
@@ -3225,105 +3225,105 @@
     let a = r(t),
         u = a(t);
     return {
         c() {
             u.c(), e = Ze(), i = le(n), l = le(" | "), o = le(s);
         },
         m(f, _) {
-            u.m(f, _), O(f, e, _), O(f, i, _), O(f, l, _), O(f, o, _);
+            u.m(f, _), D(f, e, _), D(f, i, _), D(f, l, _), D(f, o, _);
         },
         p(f, _) {
             a === (a = r(f)) && u ? u.p(f, _) : (u.d(1), u = a(f), u && (u.c(), u.m(e.parentNode, e))), _[0] & /*progress*/
                 128 && n !== (n = /*p*/
-                    f[38].unit + "") && Re(i, n);
+                    f[38].unit + "") && De(i, n);
         },
         d(f) {
-            f && (M(e), M(i), M(l), M(o)), u.d(f);
+            f && (O(e), O(i), O(l), O(o)), u.d(f);
         }
     };
 }
 
 function mh(t) {
-    let e = Kt(
+    let e = en(
             /*p*/
             t[38].index || 0
         ) + "",
         n;
     return {
         c() {
             n = le(e);
         },
         m(i, l) {
-            O(i, n, l);
+            D(i, n, l);
         },
         p(i, l) {
             l[0] & /*progress*/
-                128 && e !== (e = Kt(
+                128 && e !== (e = en(
                     /*p*/
                     i[38].index || 0
-                ) + "") && Re(n, e);
+                ) + "") && De(n, e);
         },
         d(i) {
-            i && M(n);
+            i && O(n);
         }
     };
 }
 
 function gh(t) {
-    let e = Kt(
+    let e = en(
             /*p*/
             t[38].index || 0
         ) + "",
-        n, i, l = Kt(
+        n, i, l = en(
             /*p*/
             t[38].length
         ) + "",
         s;
     return {
         c() {
             n = le(e), i = le("/"), s = le(l);
         },
         m(o, r) {
-            O(o, n, r), O(o, i, r), O(o, s, r);
+            D(o, n, r), D(o, i, r), D(o, s, r);
         },
         p(o, r) {
             r[0] & /*progress*/
-                128 && e !== (e = Kt(
+                128 && e !== (e = en(
                     /*p*/
                     o[38].index || 0
-                ) + "") && Re(n, e), r[0] & /*progress*/
-                128 && l !== (l = Kt(
+                ) + "") && De(n, e), r[0] & /*progress*/
+                128 && l !== (l = en(
                     /*p*/
                     o[38].length
-                ) + "") && Re(s, l);
+                ) + "") && De(s, l);
         },
         d(o) {
-            o && (M(n), M(i), M(s));
+            o && (O(n), O(i), O(s));
         }
     };
 }
 
 function no(t) {
     let e, n = (
         /*p*/
         t[38].index != null && to(t)
     );
     return {
         c() {
-            n && n.c(), e = hn();
+            n && n.c(), e = mn();
         },
         m(i, l) {
-            n && n.m(i, l), O(i, e, l);
+            n && n.m(i, l), D(i, e, l);
         },
         p(i, l) {
             /*p*/
             i[38].index != null ? n ? n.p(i, l) : (n = to(i), n.c(), n.m(e.parentNode, e)) : n && (n.d(1), n = null);
         },
         d(i) {
-            i && M(e), n && n.d(i);
+            i && O(e), n && n.d(i);
         }
     };
 }
 
 function io(t) {
     let e, n = (
             /*eta*/
@@ -3335,29 +3335,29 @@
         c() {
             e = le(
                 /*formatted_timer*/
                 t[20]
             ), i = le(n), l = le("s");
         },
         m(s, o) {
-            O(s, e, o), O(s, i, o), O(s, l, o);
+            D(s, e, o), D(s, i, o), D(s, l, o);
         },
         p(s, o) {
             o[0] & /*formatted_timer*/
-                1048576 && Re(
+                1048576 && De(
                     e,
                     /*formatted_timer*/
                     s[20]
                 ), o[0] & /*eta, formatted_eta*/
                 524289 && n !== (n = /*eta*/
                     s[0] ? `/${/*formatted_eta*/
-      s[19]}` : "") && Re(i, n);
+      s[19]}` : "") && De(i, n);
         },
         d(s) {
-            s && (M(e), M(i), M(l));
+            s && (O(e), O(i), O(l));
         }
     };
 }
 
 function bh(t) {
     let e, n;
     return e = new J_({
@@ -3377,18 +3377,18 @@
         p(i, l) {
             const s = {};
             l[0] & /*variant*/
                 256 && (s.margin = /*variant*/
                     i[8] === "default"), e.$set(s);
         },
         i(i) {
-            n || (ln(e.$$.fragment, i), n = !0);
+            n || (on(e.$$.fragment, i), n = !0);
         },
         o(i) {
-            sn(e.$$.fragment, i), n = !1;
+            rn(e.$$.fragment, i), n = !1;
         },
         d(i) {
             eh(e, i);
         }
     };
 }
 
@@ -3397,71 +3397,71 @@
   t[15] * 100}%`,
         r = (
             /*progress*/
             t[7] != null && lo(t)
         );
     return {
         c() {
-            e = Ke("div"), n = Ke("div"), r && r.c(), i = Ze(), l = Ke("div"), s = Ke("div"), We(n, "class", "progress-level-inner svelte-1yserjw"), We(s, "class", "progress-bar svelte-1yserjw"), at(s, "width", o), We(l, "class", "progress-bar-wrap svelte-1yserjw"), We(e, "class", "progress-level svelte-1yserjw");
+            e = Ke("div"), n = Ke("div"), r && r.c(), i = Ze(), l = Ke("div"), s = Ke("div"), We(n, "class", "progress-level-inner svelte-1yserjw"), We(s, "class", "progress-bar svelte-1yserjw"), ut(s, "width", o), We(l, "class", "progress-bar-wrap svelte-1yserjw"), We(e, "class", "progress-level svelte-1yserjw");
         },
         m(a, u) {
-            O(a, e, u), Ct(e, n), r && r.m(n, null), Ct(e, i), Ct(e, l), Ct(l, s), t[30](s);
+            D(a, e, u), At(e, n), r && r.m(n, null), At(e, i), At(e, l), At(l, s), t[30](s);
         },
         p(a, u) {
             /*progress*/
             a[7] != null ? r ? r.p(a, u) : (r = lo(a), r.c(), r.m(n, null)) : r && (r.d(1), r = null), u[0] & /*last_progress_level*/
                 32768 && o !== (o = `${/*last_progress_level*/
-      a[15] * 100}%`) && at(s, "width", o);
+      a[15] * 100}%`) && ut(s, "width", o);
         },
         i: jl,
         o: jl,
         d(a) {
-            a && M(e), r && r.d(), t[30](null);
+            a && O(e), r && r.d(), t[30](null);
         }
     };
 }
 
 function lo(t) {
-    let e, n = vi(
+    let e, n = ki(
             /*progress*/
             t[7]
         ),
         i = [];
     for (let l = 0; l < n.length; l += 1)
         i[l] = uo(Ks(t, n, l));
     return {
         c() {
             for (let l = 0; l < i.length; l += 1)
                 i[l].c();
-            e = hn();
+            e = mn();
         },
         m(l, s) {
             for (let o = 0; o < i.length; o += 1)
                 i[o] && i[o].m(l, s);
-            O(l, e, s);
+            D(l, e, s);
         },
         p(l, s) {
             if (s[0] & /*progress_level, progress*/
                 16512) {
-                n = vi(
+                n = ki(
                     /*progress*/
                     l[7]
                 );
                 let o;
                 for (o = 0; o < n.length; o += 1) {
                     const r = Ks(l, n, o);
                     i[o] ? i[o].p(r, s) : (i[o] = uo(r), i[o].c(), i[o].m(e.parentNode, e));
                 }
                 for (; o < i.length; o += 1)
                     i[o].d(1);
                 i.length = n.length;
             }
         },
         d(l) {
-            l && M(e), Or(i, l);
+            l && O(e), Or(i, l);
         }
     };
 }
 
 function so(t) {
     let e, n, i, l, s = (
             /*i*/
@@ -3482,47 +3482,47 @@
         ),
         a = (
             /*progress_level*/
             t[14] != null && ao(t)
         );
     return {
         c() {
-            s && s.c(), e = Ze(), o && o.c(), n = Ze(), r && r.c(), i = Ze(), a && a.c(), l = hn();
+            s && s.c(), e = Ze(), o && o.c(), n = Ze(), r && r.c(), i = Ze(), a && a.c(), l = mn();
         },
         m(u, f) {
-            s && s.m(u, f), O(u, e, f), o && o.m(u, f), O(u, n, f), r && r.m(u, f), O(u, i, f), a && a.m(u, f), O(u, l, f);
+            s && s.m(u, f), D(u, e, f), o && o.m(u, f), D(u, n, f), r && r.m(u, f), D(u, i, f), a && a.m(u, f), D(u, l, f);
         },
         p(u, f) {
             /*p*/
             u[38].desc != null ? o ? o.p(u, f) : (o = oo(u), o.c(), o.m(n.parentNode, n)) : o && (o.d(1), o = null), /*p*/
                 u[38].desc != null && /*progress_level*/
                 u[14] && /*progress_level*/
                 u[14][
                     /*i*/
                     u[40]
                 ] != null ? r || (r = ro(), r.c(), r.m(i.parentNode, i)) : r && (r.d(1), r = null), /*progress_level*/
                 u[14] != null ? a ? a.p(u, f) : (a = ao(u), a.c(), a.m(l.parentNode, l)) : a && (a.d(1), a = null);
         },
         d(u) {
-            u && (M(e), M(n), M(i), M(l)), s && s.d(u), o && o.d(u), r && r.d(u), a && a.d(u);
+            u && (O(e), O(n), O(i), O(l)), s && s.d(u), o && o.d(u), r && r.d(u), a && a.d(u);
         }
     };
 }
 
 function wh(t) {
     let e;
     return {
         c() {
             e = le(" /");
         },
         m(n, i) {
-            O(n, e, i);
+            D(n, e, i);
         },
         d(n) {
-            n && M(e);
+            n && O(e);
         }
     };
 }
 
 function oo(t) {
     let e = (
             /*p*/
@@ -3530,38 +3530,38 @@
         ),
         n;
     return {
         c() {
             n = le(e);
         },
         m(i, l) {
-            O(i, n, l);
+            D(i, n, l);
         },
         p(i, l) {
             l[0] & /*progress*/
                 128 && e !== (e = /*p*/
-                    i[38].desc + "") && Re(n, e);
+                    i[38].desc + "") && De(n, e);
         },
         d(i) {
-            i && M(n);
+            i && O(n);
         }
     };
 }
 
 function ro(t) {
     let e;
     return {
         c() {
             e = le("-");
         },
         m(n, i) {
-            O(n, e, i);
+            D(n, e, i);
         },
         d(n) {
-            n && M(e);
+            n && O(e);
         }
     };
 }
 
 function ao(t) {
     let e = (100 * /*progress_level*/
             (t[14][
@@ -3570,26 +3570,26 @@
             ] || 0)).toFixed(1) + "",
         n, i;
     return {
         c() {
             n = le(e), i = le("%");
         },
         m(l, s) {
-            O(l, n, s), O(l, i, s);
+            D(l, n, s), D(l, i, s);
         },
         p(l, s) {
             s[0] & /*progress_level*/
                 16384 && e !== (e = (100 * /*progress_level*/
                     (l[14][
                         /*i*/
                         l[40]
-                    ] || 0)).toFixed(1) + "") && Re(n, e);
+                    ] || 0)).toFixed(1) + "") && De(n, e);
         },
         d(l) {
-            l && (M(n), M(i));
+            l && (O(n), O(i));
         }
     };
 }
 
 function uo(t) {
     let e, n = (
         /*p*/
@@ -3598,56 +3598,56 @@
             t[14][
                 /*i*/
                 t[40]
             ] != null) && so(t)
     );
     return {
         c() {
-            n && n.c(), e = hn();
+            n && n.c(), e = mn();
         },
         m(i, l) {
-            n && n.m(i, l), O(i, e, l);
+            n && n.m(i, l), D(i, e, l);
         },
         p(i, l) {
             /*p*/
             i[38].desc != null || /*progress_level*/
                 i[14] && /*progress_level*/
                 i[14][
                     /*i*/
                     i[40]
                 ] != null ? n ? n.p(i, l) : (n = so(i), n.c(), n.m(e.parentNode, e)) : n && (n.d(1), n = null);
         },
         d(i) {
-            i && M(e), n && n.d(i);
+            i && O(e), n && n.d(i);
         }
     };
 }
 
 function fo(t) {
     let e, n;
     return {
         c() {
             e = Ke("p"), n = le(
                 /*loading_text*/
                 t[9]
             ), We(e, "class", "loading svelte-1yserjw");
         },
         m(i, l) {
-            O(i, e, l), Ct(e, n);
+            D(i, e, l), At(e, n);
         },
         p(i, l) {
             l[0] & /*loading_text*/
-                512 && Re(
+                512 && De(
                     n,
                     /*loading_text*/
                     i[9]
                 );
         },
         d(i) {
-            i && M(e);
+            i && O(e);
         }
     };
 }
 
 function vh(t) {
     let e, n, i, l, s;
     const o = [ch, fh],
@@ -3662,127 +3662,127 @@
             )
         );
     }
     return ~(n = a(t)) && (i = r[n] = o[n](t)), {
         c() {
             e = Ke("div"), i && i.c(), We(e, "class", l = "wrap " + /*variant*/
                 t[8] + " " + /*show_progress*/
-                t[6] + " svelte-1yserjw"), De(e, "hide", ! /*status*/
+                t[6] + " svelte-1yserjw"), Oe(e, "hide", ! /*status*/
                 t[4] || /*status*/
                 t[4] === "complete" || /*show_progress*/
-                t[6] === "hidden"), De(
+                t[6] === "hidden"), Oe(
                 e,
                 "translucent",
                 /*variant*/
                 t[8] === "center" && /*status*/
                 (t[4] === "pending" || /*status*/
                     t[4] === "error") || /*translucent*/
                 t[11] || /*show_progress*/
                 t[6] === "minimal"
-            ), De(
+            ), Oe(
                 e,
                 "generating",
                 /*status*/
                 t[4] === "generating"
-            ), De(
+            ), Oe(
                 e,
                 "border",
                 /*border*/
                 t[12]
-            ), at(
+            ), ut(
                 e,
                 "position",
                 /*absolute*/
                 t[10] ? "absolute" : "static"
-            ), at(
+            ), ut(
                 e,
                 "padding",
                 /*absolute*/
                 t[10] ? "0" : "var(--size-8) 0"
             );
         },
         m(u, f) {
-            O(u, e, f), ~n && r[n].m(e, null), t[31](e), s = !0;
+            D(u, e, f), ~n && r[n].m(e, null), t[31](e), s = !0;
         },
         p(u, f) {
             let _ = n;
-            n = a(u), n === _ ? ~n && r[n].p(u, f) : (i && (Dr(), sn(r[_], 1, 1, () => {
+            n = a(u), n === _ ? ~n && r[n].p(u, f) : (i && (Dr(), rn(r[_], 1, 1, () => {
                     r[_] = null;
-                }), Mr()), ~n ? (i = r[n], i ? i.p(u, f) : (i = r[n] = o[n](u), i.c()), ln(i, 1), i.m(e, null)) : i = null), (!s || f[0] & /*variant, show_progress*/
+                }), Mr()), ~n ? (i = r[n], i ? i.p(u, f) : (i = r[n] = o[n](u), i.c()), on(i, 1), i.m(e, null)) : i = null), (!s || f[0] & /*variant, show_progress*/
                     320 && l !== (l = "wrap " + /*variant*/
                         u[8] + " " + /*show_progress*/
                         u[6] + " svelte-1yserjw")) && We(e, "class", l), (!s || f[0] & /*variant, show_progress, status, show_progress*/
-                    336) && De(e, "hide", ! /*status*/
+                    336) && Oe(e, "hide", ! /*status*/
                     u[4] || /*status*/
                     u[4] === "complete" || /*show_progress*/
                     u[6] === "hidden"), (!s || f[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
-                    2384) && De(
+                    2384) && Oe(
                     e,
                     "translucent",
                     /*variant*/
                     u[8] === "center" && /*status*/
                     (u[4] === "pending" || /*status*/
                         u[4] === "error") || /*translucent*/
                     u[11] || /*show_progress*/
                     u[6] === "minimal"
                 ), (!s || f[0] & /*variant, show_progress, status*/
-                    336) && De(
+                    336) && Oe(
                     e,
                     "generating",
                     /*status*/
                     u[4] === "generating"
                 ), (!s || f[0] & /*variant, show_progress, border*/
-                    4416) && De(
+                    4416) && Oe(
                     e,
                     "border",
                     /*border*/
                     u[12]
                 ), f[0] & /*absolute*/
-                1024 && at(
+                1024 && ut(
                     e,
                     "position",
                     /*absolute*/
                     u[10] ? "absolute" : "static"
                 ), f[0] & /*absolute*/
-                1024 && at(
+                1024 && ut(
                     e,
                     "padding",
                     /*absolute*/
                     u[10] ? "0" : "var(--size-8) 0"
                 );
         },
         i(u) {
-            s || (ln(i), s = !0);
+            s || (on(i), s = !0);
         },
         o(u) {
-            sn(i), s = !1;
+            rn(i), s = !1;
         },
         d(u) {
-            u && M(e), ~n && r[n].d(), t[31](null);
+            u && O(e), ~n && r[n].d(), t[31](null);
         }
     };
 }
-let Kn = [],
+let ti = [],
     _l = !1;
 async function yh(t, e = !0) {
     if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && e !== !0)) {
-        if (Kn.push(t), !_l)
+        if (ti.push(t), !_l)
             _l = !0;
         else
             return;
         await rh(), requestAnimationFrame(() => {
             let n = [0, 0];
-            for (let i = 0; i < Kn.length; i++) {
-                const s = Kn[i].getBoundingClientRect();
+            for (let i = 0; i < ti.length; i++) {
+                const s = ti[i].getBoundingClientRect();
                 (i === 0 || s.top + window.scrollY <= n[0]) && (n[0] = s.top + window.scrollY, n[1] = i);
             }
             window.scrollTo({
                 top: n[0] - 20,
                 behavior: "smooth"
-            }), _l = !1, Kn = [];
+            }), _l = !1, ti = [];
         });
     }
 }
 
 function Eh(t, e, n) {
     let i, {
             $$slots: l = {},
@@ -3812,21 +3812,21 @@
         {
             show_progress: c = "full"
         } = e,
         {
             message: d = null
         } = e,
         {
-            progress: m = null
+            progress: b = null
         } = e,
         {
-            variant: b = "default"
+            variant: p = "default"
         } = e,
         {
-            loading_text: p = "Loading..."
+            loading_text: g = "Loading..."
         } = e,
         {
             absolute: y = !0
         } = e,
         {
             translucent: w = !1
         } = e,
@@ -3838,83 +3838,83 @@
         } = e,
         E, N = !1,
         v = 0,
         A = 0,
         B = null,
         L = null,
         x = 0,
-        J = null,
-        ce, te = null,
-        ke = !0;
-    const ye = () => {
-        n(0, r = n(26, B = n(19, S = null))), n(24, v = performance.now()), n(25, A = 0), N = !0, me();
+        Y = null,
+        _e, te = null,
+        Ee = !0;
+    const ve = () => {
+        n(0, r = n(26, B = n(19, S = null))), n(24, v = performance.now()), n(25, A = 0), N = !0, de();
     };
 
-    function me() {
+    function de() {
         requestAnimationFrame(() => {
-            n(25, A = (performance.now() - v) / 1e3), N && me();
+            n(25, A = (performance.now() - v) / 1e3), N && de();
         });
     }
 
-    function _e() {
+    function ce() {
         n(25, A = 0), n(0, r = n(26, B = n(19, S = null))), N && (N = !1);
     }
     ah(() => {
-        N && _e();
+        N && ce();
     });
     let S = null;
 
-    function k(g) {
-        Js[g ? "unshift" : "push"](() => {
-            te = g, n(16, te), n(7, m), n(14, J), n(15, ce);
+    function k(m) {
+        Js[m ? "unshift" : "push"](() => {
+            te = m, n(16, te), n(7, b), n(14, Y), n(15, _e);
         });
     }
 
-    function I(g) {
-        Js[g ? "unshift" : "push"](() => {
-            E = g, n(13, E);
+    function I(m) {
+        Js[m ? "unshift" : "push"](() => {
+            E = m, n(13, E);
         });
     }
-    return t.$$set = (g) => {
-        "i18n" in g && n(1, o = g.i18n), "eta" in g && n(0, r = g.eta), "queue_position" in g && n(2, a = g.queue_position), "queue_size" in g && n(3, u = g.queue_size), "status" in g && n(4, f = g.status), "scroll_to_output" in g && n(21, _ = g.scroll_to_output), "timer" in g && n(5, h = g.timer), "show_progress" in g && n(6, c = g.show_progress), "message" in g && n(22, d = g.message), "progress" in g && n(7, m = g.progress), "variant" in g && n(8, b = g.variant), "loading_text" in g && n(9, p = g.loading_text), "absolute" in g && n(10, y = g.absolute), "translucent" in g && n(11, w = g.translucent), "border" in g && n(12, C = g.border), "autoscroll" in g && n(23, P = g.autoscroll), "$$scope" in g && n(28, s = g.$$scope);
+    return t.$$set = (m) => {
+        "i18n" in m && n(1, o = m.i18n), "eta" in m && n(0, r = m.eta), "queue_position" in m && n(2, a = m.queue_position), "queue_size" in m && n(3, u = m.queue_size), "status" in m && n(4, f = m.status), "scroll_to_output" in m && n(21, _ = m.scroll_to_output), "timer" in m && n(5, h = m.timer), "show_progress" in m && n(6, c = m.show_progress), "message" in m && n(22, d = m.message), "progress" in m && n(7, b = m.progress), "variant" in m && n(8, p = m.variant), "loading_text" in m && n(9, g = m.loading_text), "absolute" in m && n(10, y = m.absolute), "translucent" in m && n(11, w = m.translucent), "border" in m && n(12, C = m.border), "autoscroll" in m && n(23, P = m.autoscroll), "$$scope" in m && n(28, s = m.$$scope);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
             218103809 && (r === null && n(0, r = B), r != null && B !== r && (n(27, L = (performance.now() - v) / 1e3 + r), n(19, S = L.toFixed(1)), n(26, B = r))), t.$$.dirty[0] & /*eta_from_start, timer_diff*/
             167772160 && n(17, x = L === null || L <= 0 || !A ? null : Math.min(A / L, 1)), t.$$.dirty[0] & /*progress*/
-            128 && m != null && n(18, ke = !1), t.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
-            114816 && (m != null ? n(14, J = m.map((g) => {
-                if (g.index != null && g.length != null)
-                    return g.index / g.length;
-                if (g.progress != null)
-                    return g.progress;
-            })) : n(14, J = null), J ? (n(15, ce = J[J.length - 1]), te && (ce === 0 ? n(16, te.style.transition = "0", te) : n(16, te.style.transition = "150ms", te))) : n(15, ce = void 0)), t.$$.dirty[0] & /*status*/
-            16 && (f === "pending" ? ye() : _e()), t.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
+            128 && b != null && n(18, Ee = !1), t.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
+            114816 && (b != null ? n(14, Y = b.map((m) => {
+                if (m.index != null && m.length != null)
+                    return m.index / m.length;
+                if (m.progress != null)
+                    return m.progress;
+            })) : n(14, Y = null), Y ? (n(15, _e = Y[Y.length - 1]), te && (_e === 0 ? n(16, te.style.transition = "0", te) : n(16, te.style.transition = "150ms", te))) : n(15, _e = void 0)), t.$$.dirty[0] & /*status*/
+            16 && (f === "pending" ? ve() : ce()), t.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
             10493968 && E && _ && (f === "pending" || f === "complete") && yh(E, P), t.$$.dirty[0] & /*status, message*/
             4194320, t.$$.dirty[0] & /*timer_diff*/
             33554432 && n(20, i = A.toFixed(1));
     }, [
         r,
         o,
         a,
         u,
         f,
         h,
         c,
-        m,
         b,
         p,
+        g,
         y,
         w,
         C,
         E,
-        J,
-        ce,
+        Y,
+        _e,
         te,
         x,
-        ke,
+        Ee,
         S,
         i,
         _,
         d,
         P,
         v,
         A,
@@ -4007,34 +4007,34 @@
             type: Ur(l.headers, "content-type")
         });
         return URL.createObjectURL(s);
     });
 }
 const {
     SvelteComponent: Hh,
-    assign: yi,
+    assign: Si,
     check_outros: qr,
     compute_rest_props: co,
     create_slot: us,
-    detach: Di,
+    detach: Fi,
     element: zr,
     empty: jr,
     exclude_internal_props: Ph,
     get_all_dirty_from_scope: fs,
     get_slot_changes: cs,
     get_spread_update: Gr,
     group_outros: xr,
     init: Nh,
-    insert: Ri,
+    insert: qi,
     listen: Vr,
     prevent_default: Lh,
     safe_not_equal: Ih,
-    set_attributes: Ei,
-    transition_in: Pt,
-    transition_out: Nt,
+    set_attributes: Ci,
+    transition_in: Nt,
+    transition_out: Lt,
     update_slot_base: _s
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: Mh
 } = window.__gradio__svelte__internal;
 
 function Oh(t) {
     let e, n, i, l, s;
@@ -4065,21 +4065,21 @@
                 )
             },
             /*$$restProps*/
             t[6]
         ],
         u = {};
     for (let f = 0; f < a.length; f += 1)
-        u = yi(u, a[f]);
+        u = Si(u, a[f]);
     return {
         c() {
-            e = zr("a"), r && r.c(), Ei(e, u);
+            e = zr("a"), r && r.c(), Ci(e, u);
         },
         m(f, _) {
-            Ri(f, e, _), r && r.m(e, null), i = !0, l || (s = Vr(
+            qi(f, e, _), r && r.m(e, null), i = !0, l || (s = Vr(
                 e,
                 "click",
                 /*dispatch*/
                 t[3].bind(null, "click")
             ), l = !0);
         },
         p(f, _) {
@@ -4097,15 +4097,15 @@
                     _,
                     null
                 ) : fs(
                     /*$$scope*/
                     f[7]
                 ),
                 null
-            ), Ei(e, u = Gr(a, [
+            ), Ci(e, u = Gr(a, [
                 (!i || _ & /*href*/
                     1) && {
                     href: (
                         /*href*/
                         f[0]
                     )
                 }, {
@@ -4122,21 +4122,21 @@
                 },
                 _ & /*$$restProps*/
                 64 && /*$$restProps*/
                 f[6]
             ]));
         },
         i(f) {
-            i || (Pt(r, f), i = !0);
+            i || (Nt(r, f), i = !0);
         },
         o(f) {
-            Nt(r, f), i = !1;
+            Lt(r, f), i = !1;
         },
         d(f) {
-            f && Di(e), r && r.d(f), l = !1, s();
+            f && Fi(e), r && r.d(f), l = !1, s();
         }
     };
 }
 
 function Dh(t) {
     let e, n, i, l;
     const s = [Uh, Rh],
@@ -4149,30 +4149,30 @@
         );
     }
     return e = r(t), n = o[e] = s[e](t), {
         c() {
             n.c(), i = jr();
         },
         m(a, u) {
-            o[e].m(a, u), Ri(a, i, u), l = !0;
+            o[e].m(a, u), qi(a, i, u), l = !0;
         },
         p(a, u) {
             let f = e;
-            e = r(a), e === f ? o[e].p(a, u) : (xr(), Nt(o[f], 1, 1, () => {
+            e = r(a), e === f ? o[e].p(a, u) : (xr(), Lt(o[f], 1, 1, () => {
                 o[f] = null;
-            }), qr(), n = o[e], n ? n.p(a, u) : (n = o[e] = s[e](a), n.c()), Pt(n, 1), n.m(i.parentNode, i));
+            }), qr(), n = o[e], n ? n.p(a, u) : (n = o[e] = s[e](a), n.c()), Nt(n, 1), n.m(i.parentNode, i));
         },
         i(a) {
-            l || (Pt(n), l = !0);
+            l || (Nt(n), l = !0);
         },
         o(a) {
-            Nt(n), l = !1;
+            Lt(n), l = !1;
         },
         d(a) {
-            a && Di(i), o[e].d(a);
+            a && Fi(i), o[e].d(a);
         }
     };
 }
 
 function Rh(t) {
     let e, n, i, l;
     const s = (
@@ -4193,21 +4193,21 @@
                     /*href*/
                     t[0]
                 )
             }
         ],
         a = {};
     for (let u = 0; u < r.length; u += 1)
-        a = yi(a, r[u]);
+        a = Si(a, r[u]);
     return {
         c() {
-            e = zr("a"), o && o.c(), Ei(e, a);
+            e = zr("a"), o && o.c(), Ci(e, a);
         },
         m(u, f) {
-            Ri(u, e, f), o && o.m(e, null), n = !0, i || (l = Vr(e, "click", Lh(
+            qi(u, e, f), o && o.m(e, null), n = !0, i || (l = Vr(e, "click", Lh(
                 /*wasm_click_handler*/
                 t[5]
             )), i = !0);
         },
         p(u, f) {
             o && o.p && (!n || f & /*$$scope*/
                 128) && _s(
@@ -4223,35 +4223,35 @@
                     f,
                     null
                 ) : fs(
                     /*$$scope*/
                     u[7]
                 ),
                 null
-            ), Ei(e, a = Gr(r, [
+            ), Ci(e, a = Gr(r, [
                 f & /*$$restProps*/
                 64 && /*$$restProps*/
                 u[6],
                 (!n || f & /*href*/
                     1) && {
                     href: (
                         /*href*/
                         u[0]
                     )
                 }
             ]));
         },
         i(u) {
-            n || (Pt(o, u), n = !0);
+            n || (Nt(o, u), n = !0);
         },
         o(u) {
-            Nt(o, u), n = !1;
+            Lt(o, u), n = !1;
         },
         d(u) {
-            u && Di(e), o && o.d(u), i = !1, l();
+            u && Fi(e), o && o.d(u), i = !1, l();
         }
     };
 }
 
 function Uh(t) {
     let e;
     const n = (
@@ -4290,18 +4290,18 @@
                     /*$$scope*/
                     l[7]
                 ),
                 null
             );
         },
         i(l) {
-            e || (Pt(i, l), e = !0);
+            e || (Nt(i, l), e = !0);
         },
         o(l) {
-            Nt(i, l), e = !1;
+            Lt(i, l), e = !1;
         },
         d(l) {
             i && i.d(l);
         }
     };
 }
 
@@ -4319,30 +4319,30 @@
                 ))), e ? 0 : 1;
     }
     return n = a(t, -1), i = r[n] = o[n](t), {
         c() {
             i.c(), l = jr();
         },
         m(u, f) {
-            r[n].m(u, f), Ri(u, l, f), s = !0;
+            r[n].m(u, f), qi(u, l, f), s = !0;
         },
         p(u, [f]) {
             let _ = n;
-            n = a(u, f), n === _ ? r[n].p(u, f) : (xr(), Nt(r[_], 1, 1, () => {
+            n = a(u, f), n === _ ? r[n].p(u, f) : (xr(), Lt(r[_], 1, 1, () => {
                 r[_] = null;
-            }), qr(), i = r[n], i ? i.p(u, f) : (i = r[n] = o[n](u), i.c()), Pt(i, 1), i.m(l.parentNode, l));
+            }), qr(), i = r[n], i ? i.p(u, f) : (i = r[n] = o[n](u), i.c()), Nt(i, 1), i.m(l.parentNode, l));
         },
         i(u) {
-            s || (Pt(i), s = !0);
+            s || (Nt(i), s = !0);
         },
         o(u) {
-            Nt(i), s = !1;
+            Lt(i), s = !1;
         },
         d(u) {
-            u && Di(l), r[n].d(u);
+            u && Fi(l), r[n].d(u);
         }
     };
 }
 
 function qh(t, e, n) {
     const i = ["href", "download"];
     let l = co(e, i),
@@ -4368,31 +4368,31 @@
             throw new Error("Wasm worker proxy is not available.");
         const d = new URL(r).pathname;
         n(2, f = !0), _.httpRequest({
             method: "GET",
             path: d,
             headers: {},
             query_string: ""
-        }).then((m) => {
-            if (m.status !== 200)
+        }).then((b) => {
+            if (b.status !== 200)
                 throw new Error(`Failed to get file ${d} from the Wasm worker.`);
-            const b = new Blob(
-                    [m.body], {
-                        type: Ur(m.headers, "content-type")
+            const p = new Blob(
+                    [b.body], {
+                        type: Ur(b.headers, "content-type")
                     }
                 ),
-                p = URL.createObjectURL(b),
+                g = URL.createObjectURL(p),
                 y = document.createElement("a");
-            y.href = p, y.download = a, y.click(), URL.revokeObjectURL(p);
+            y.href = g, y.download = a, y.click(), URL.revokeObjectURL(g);
         }).finally(() => {
             n(2, f = !1);
         });
     }
     return t.$$set = (c) => {
-        e = yi(yi({}, e), Ph(c)), n(6, l = co(e, i)), "href" in c && n(0, r = c.href), "download" in c && n(1, a = c.download), "$$scope" in c && n(7, o = c.$$scope);
+        e = Si(Si({}, e), Ph(c)), n(6, l = co(e, i)), "href" in c && n(0, r = c.href), "download" in c && n(1, a = c.download), "$$scope" in c && n(7, o = c.$$scope);
     }, [
         r,
         a,
         f,
         u,
         _,
         h,
@@ -4590,15 +4590,15 @@
         mime_type: r,
         alt_text: a
     }) {
         this.path = e, this.url = n, this.orig_name = i, this.size = l, this.blob = n ? void 0 : s, this.is_stream = o, this.mime_type = r, this.alt_text = a;
     }
 }
 const Zr = "This application is too busy. Keep trying!",
-    gt = "Connection errored out.";
+    bt = "Connection errored out.";
 let Yr;
 
 function Jh(t, e) {
     return {
         post_data: n,
         upload_files: i,
         client: l,
@@ -4613,15 +4613,15 @@
             var f = await t(o, {
                 method: "POST",
                 body: JSON.stringify(r),
                 headers: u
             });
         } catch {
             return [{
-                error: gt
+                error: bt
             }, 500];
         }
         let _, h;
         try {
             _ = await f.json(), h = f.status;
         } catch (c) {
             _ = {
@@ -4632,86 +4632,86 @@
     }
     async function i(o, r, a, u) {
         const f = {};
         a && (f.Authorization = `Bearer ${a}`);
         const _ = 1e3,
             h = [];
         for (let d = 0; d < r.length; d += _) {
-            const m = r.slice(d, d + _),
-                b = new FormData();
-            m.forEach((y) => {
-                b.append("files", y);
+            const b = r.slice(d, d + _),
+                p = new FormData();
+            b.forEach((y) => {
+                p.append("files", y);
             });
             try {
                 const y = u ? `${o}/upload?upload_id=${u}` : `${o}/upload`;
                 var c = await t(y, {
                     method: "POST",
-                    body: b,
+                    body: p,
                     headers: f
                 });
             } catch {
                 return {
-                    error: gt
+                    error: bt
                 };
             }
-            const p = await c.json();
-            h.push(...p);
+            const g = await c.json();
+            h.push(...g);
         }
         return {
             files: h
         };
     }
     async function l(o, r = {}) {
         return new Promise(async (a) => {
             const {
                 status_callback: u,
                 hf_token: f
             } = r, _ = {
-                predict: ce,
+                predict: _e,
                 submit: te,
-                view_api: _e,
-                component_server: me
+                view_api: ce,
+                component_server: de
             };
             if ((typeof window > "u" || !("WebSocket" in window)) && !global.Websocket) {
-                const S = await import("./wrapper-6f348d45-f837cf34.js");
+                const S = await import("./wrapper-6f348d45-19fa94bf.js");
                 Yr = (await import("./__vite-browser-external-2447137e.js")).Blob, global.WebSocket = S.WebSocket;
             }
             const {
                 ws_protocol: h,
                 http_protocol: c,
                 host: d,
-                space_id: m
-            } = await Gh(o, f), b = Math.random().toString(36).substring(2), p = {};
+                space_id: b
+            } = await Gh(o, f), p = Math.random().toString(36).substring(2), g = {};
             let y = !1,
                 w = {},
                 C = {},
                 P = null;
             const E = {},
                 N = /* @__PURE__ */ new Set();
             let v, A = {},
                 B = !1;
-            f && m && (B = await $h(m, f));
+            f && b && (B = await $h(b, f));
             async function L(S) {
                 if (v = S, window.location.protocol === "https:" && (v.root = v.root.replace("http://", "https://")), A = xh((S == null ? void 0 : S.dependencies) || []), v.auth_required)
                     return {
                         config: v,
                         ..._
                     };
                 try {
-                    x = await _e(v);
+                    x = await ce(v);
                 } catch (k) {
                     console.error(`Could not get api details: ${k.message}`);
                 }
                 return {
                     config: v,
                     ..._
                 };
             }
             let x;
-            async function J(S) {
+            async function Y(S) {
                 if (u && u(S), S.status === "running")
                     try {
                         v = await po(
                             t,
                             `${c}//${d}`,
                             f
                         );
@@ -4731,577 +4731,577 @@
                     t,
                     `${c}//${d}`,
                     f
                 );
                 const S = await L(v);
                 a(S);
             } catch (S) {
-                console.error(S), m ? xl(
-                    m,
-                    Wr.test(m) ? "space_name" : "subdomain",
-                    J
+                console.error(S), b ? xl(
+                    b,
+                    Wr.test(b) ? "space_name" : "subdomain",
+                    Y
                 ) : u && u({
                     status: "error",
                     message: "Could not load this space.",
                     load_status: "error",
                     detail: "NOT_FOUND"
                 });
             }
 
-            function ce(S, k, I) {
-                let g = !1,
+            function _e(S, k, I) {
+                let m = !1,
                     T = !1,
                     ae;
                 if (typeof S == "number")
                     ae = v.dependencies[S];
                 else {
-                    const Q = S.replace(/^\//, "");
-                    ae = v.dependencies[A[Q]];
+                    const J = S.replace(/^\//, "");
+                    ae = v.dependencies[A[J]];
                 }
                 if (ae.types.continuous)
                     throw new Error(
                         "Cannot call predict on this function as it may run forever. Use submit instead"
                     );
-                return new Promise((Q, Se) => {
+                return new Promise((J, ke) => {
                     const He = te(S, k, I);
-                    let D;
-                    He.on("data", (H) => {
-                        T && (He.destroy(), Q(H)), g = !0, D = H;
-                    }).on("status", (H) => {
-                        H.stage === "error" && Se(H), H.stage === "complete" && (T = !0, g && (He.destroy(), Q(D)));
+                    let R;
+                    He.on("data", (Se) => {
+                        T && (He.destroy(), J(Se)), m = !0, R = Se;
+                    }).on("status", (Se) => {
+                        Se.stage === "error" && ke(Se), Se.stage === "complete" && (T = !0, m && (He.destroy(), J(R)));
                     });
                 });
             }
 
-            function te(S, k, I, g = null) {
+            function te(S, k, I, m = null) {
                 let T, ae;
                 if (typeof S == "number")
                     T = S, ae = x.unnamed_endpoints[T];
                 else {
                     const K = S.replace(/^\//, "");
                     T = A[K], ae = x.named_endpoints[S.trim()];
                 }
                 if (typeof T != "number")
                     throw new Error(
                         "There is no endpoint matching that name of fn_index matching that number."
                     );
-                let Q, Se, He = v.protocol ?? "ws";
-                const D = typeof S == "number" ? "/predict" : S;
-                let H, R = null,
-                    j = !1;
-                const X = {};
-                let he = "";
-                typeof window < "u" && (he = new URLSearchParams(window.location.search).toString()), s(`${v.root}`, k, ae, f).then(
+                let J, ke, He = v.protocol ?? "ws";
+                const R = typeof S == "number" ? "/predict" : S;
+                let Se, H = null,
+                    U = !1;
+                const Q = {};
+                let j = "";
+                typeof window < "u" && (j = new URLSearchParams(window.location.search).toString()), s(`${v.root}`, k, ae, f).then(
                     (K) => {
-                        if (H = {
+                        if (Se = {
                                 data: K || [],
                                 event_data: I,
                                 fn_index: T,
-                                trigger_id: g
+                                trigger_id: m
                             }, e0(T, v))
-                            q({
+                            M({
                                 type: "status",
-                                endpoint: D,
+                                endpoint: R,
                                 stage: "pending",
                                 queue: !1,
                                 fn_index: T,
                                 time: /* @__PURE__ */ new Date()
                             }), n(
-                                `${v.root}/run${D.startsWith("/") ? D : `/${D}`}${he ? "?" + he : ""}`, {
-                                    ...H,
-                                    session_hash: b
+                                `${v.root}/run${R.startsWith("/") ? R : `/${R}`}${j ? "?" + j : ""}`, {
+                                    ...Se,
+                                    session_hash: p
                                 },
                                 f
-                            ).then(([ne, Y]) => {
-                                const de = ne.data;
-                                Y == 200 ? (q({
+                            ).then(([ne, Z]) => {
+                                const he = ne.data;
+                                Z == 200 ? (M({
                                     type: "data",
-                                    endpoint: D,
+                                    endpoint: R,
                                     fn_index: T,
-                                    data: de,
+                                    data: he,
                                     time: /* @__PURE__ */ new Date()
-                                }), q({
+                                }), M({
                                     type: "status",
-                                    endpoint: D,
+                                    endpoint: R,
                                     fn_index: T,
                                     stage: "complete",
                                     eta: ne.average_duration,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
-                                })) : q({
+                                })) : M({
                                     type: "status",
                                     stage: "error",
-                                    endpoint: D,
+                                    endpoint: R,
                                     fn_index: T,
                                     message: ne.error,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
                                 });
                             }).catch((ne) => {
-                                q({
+                                M({
                                     type: "status",
                                     stage: "error",
                                     message: ne.message,
-                                    endpoint: D,
+                                    endpoint: R,
                                     fn_index: T,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
                                 });
                             });
                         else if (He == "ws") {
-                            q({
+                            M({
                                 type: "status",
                                 stage: "pending",
                                 queue: !0,
-                                endpoint: D,
+                                endpoint: R,
                                 fn_index: T,
                                 time: /* @__PURE__ */ new Date()
                             });
                             let ne = new URL(`${h}://${Xr(
                 d,
                 v.path,
                 !0
               )}
-							/queue/join${he ? "?" + he : ""}`);
-                            B && ne.searchParams.set("__sign", B), Q = new WebSocket(ne), Q.onclose = (Y) => {
-                                Y.wasClean || q({
+							/queue/join${j ? "?" + j : ""}`);
+                            B && ne.searchParams.set("__sign", B), J = new WebSocket(ne), J.onclose = (Z) => {
+                                Z.wasClean || M({
                                     type: "status",
                                     stage: "error",
                                     broken: !0,
-                                    message: gt,
+                                    message: bt,
                                     queue: !0,
-                                    endpoint: D,
+                                    endpoint: R,
                                     fn_index: T,
                                     time: /* @__PURE__ */ new Date()
                                 });
-                            }, Q.onmessage = function(Y) {
-                                const de = JSON.parse(Y.data),
+                            }, J.onmessage = function(Z) {
+                                const he = JSON.parse(Z.data),
                                     {
                                         type: ue,
                                         status: V,
-                                        data: Z
+                                        data: W
                                     } = ml(
-                                        de,
-                                        p[T]
+                                        he,
+                                        g[T]
                                     );
-                                if (ue === "update" && V && !j)
-                                    q({
+                                if (ue === "update" && V && !U)
+                                    M({
                                         type: "status",
-                                        endpoint: D,
+                                        endpoint: R,
                                         fn_index: T,
                                         time: /* @__PURE__ */ new Date(),
                                         ...V
-                                    }), V.stage === "error" && Q.close();
+                                    }), V.stage === "error" && J.close();
                                 else if (ue === "hash") {
-                                    Q.send(JSON.stringify({
+                                    J.send(JSON.stringify({
                                         fn_index: T,
-                                        session_hash: b
+                                        session_hash: p
                                     }));
                                     return;
                                 } else
-                                    ue === "data" ? Q.send(JSON.stringify({
-                                        ...H,
-                                        session_hash: b
-                                    })) : ue === "complete" ? j = V : ue === "log" ? q({
+                                    ue === "data" ? J.send(JSON.stringify({
+                                        ...Se,
+                                        session_hash: p
+                                    })) : ue === "complete" ? U = V : ue === "log" ? M({
                                         type: "log",
-                                        log: Z.log,
-                                        level: Z.level,
-                                        endpoint: D,
+                                        log: W.log,
+                                        level: W.level,
+                                        endpoint: R,
                                         fn_index: T
-                                    }) : ue === "generating" && q({
+                                    }) : ue === "generating" && M({
                                         type: "status",
                                         time: /* @__PURE__ */ new Date(),
                                         ...V,
                                         stage: V == null ? void 0 : V.stage,
                                         queue: !0,
-                                        endpoint: D,
+                                        endpoint: R,
                                         fn_index: T
                                     });
-                                Z && (q({
+                                W && (M({
                                     type: "data",
                                     time: /* @__PURE__ */ new Date(),
-                                    data: Z.data,
-                                    endpoint: D,
+                                    data: W.data,
+                                    endpoint: R,
                                     fn_index: T
-                                }), j && (q({
+                                }), U && (M({
                                     type: "status",
                                     time: /* @__PURE__ */ new Date(),
-                                    ...j,
+                                    ...U,
                                     stage: V == null ? void 0 : V.stage,
                                     queue: !0,
-                                    endpoint: D,
+                                    endpoint: R,
                                     fn_index: T
-                                }), Q.close()));
+                                }), J.close()));
                             }, _o(v.version || "2.0.0", "3.6") < 0 && addEventListener(
                                 "open",
-                                () => Q.send(JSON.stringify({
-                                    hash: b
+                                () => J.send(JSON.stringify({
+                                    hash: p
                                 }))
                             );
                         } else if (He == "sse") {
-                            q({
+                            M({
                                 type: "status",
                                 stage: "pending",
                                 queue: !0,
-                                endpoint: D,
+                                endpoint: R,
                                 fn_index: T,
                                 time: /* @__PURE__ */ new Date()
                             });
-                            var ge = new URLSearchParams({
+                            var me = new URLSearchParams({
                                 fn_index: T.toString(),
-                                session_hash: b
+                                session_hash: p
                             }).toString();
                             let ne = new URL(
-                                `${v.root}/queue/join?${he ? he + "&" : ""}${ge}`
+                                `${v.root}/queue/join?${j ? j + "&" : ""}${me}`
                             );
-                            Se = e(ne), Se.onmessage = async function(Y) {
-                                const de = JSON.parse(Y.data),
+                            ke = e(ne), ke.onmessage = async function(Z) {
+                                const he = JSON.parse(Z.data),
                                     {
                                         type: ue,
                                         status: V,
-                                        data: Z
+                                        data: W
                                     } = ml(
-                                        de,
-                                        p[T]
+                                        he,
+                                        g[T]
                                     );
-                                if (ue === "update" && V && !j)
-                                    q({
+                                if (ue === "update" && V && !U)
+                                    M({
                                         type: "status",
-                                        endpoint: D,
+                                        endpoint: R,
                                         fn_index: T,
                                         time: /* @__PURE__ */ new Date(),
                                         ...V
-                                    }), V.stage === "error" && Se.close();
+                                    }), V.stage === "error" && ke.close();
                                 else if (ue === "data") {
-                                    R = de.event_id;
-                                    let [mt, xa] = await n(
+                                    H = he.event_id;
+                                    let [gt, xa] = await n(
                                         `${v.root}/queue/data`, {
-                                            ...H,
-                                            session_hash: b,
-                                            event_id: R
+                                            ...Se,
+                                            session_hash: p,
+                                            event_id: H
                                         },
                                         f
                                     );
-                                    xa !== 200 && (q({
+                                    xa !== 200 && (M({
                                         type: "status",
                                         stage: "error",
-                                        message: gt,
+                                        message: bt,
                                         queue: !0,
-                                        endpoint: D,
+                                        endpoint: R,
                                         fn_index: T,
                                         time: /* @__PURE__ */ new Date()
-                                    }), Se.close());
+                                    }), ke.close());
                                 } else
-                                    ue === "complete" ? j = V : ue === "log" ? q({
+                                    ue === "complete" ? U = V : ue === "log" ? M({
                                         type: "log",
-                                        log: Z.log,
-                                        level: Z.level,
-                                        endpoint: D,
+                                        log: W.log,
+                                        level: W.level,
+                                        endpoint: R,
                                         fn_index: T
-                                    }) : ue === "generating" && q({
+                                    }) : ue === "generating" && M({
                                         type: "status",
                                         time: /* @__PURE__ */ new Date(),
                                         ...V,
                                         stage: V == null ? void 0 : V.stage,
                                         queue: !0,
-                                        endpoint: D,
+                                        endpoint: R,
                                         fn_index: T
                                     });
-                                Z && (q({
+                                W && (M({
                                     type: "data",
                                     time: /* @__PURE__ */ new Date(),
-                                    data: Z.data,
-                                    endpoint: D,
+                                    data: W.data,
+                                    endpoint: R,
                                     fn_index: T
-                                }), j && (q({
+                                }), U && (M({
                                     type: "status",
                                     time: /* @__PURE__ */ new Date(),
-                                    ...j,
+                                    ...U,
                                     stage: V == null ? void 0 : V.stage,
                                     queue: !0,
-                                    endpoint: D,
+                                    endpoint: R,
                                     fn_index: T
-                                }), Se.close()));
+                                }), ke.close()));
                             };
                         } else
-                            (He == "sse_v1" || He == "sse_v2") && (q({
+                            (He == "sse_v1" || He == "sse_v2") && (M({
                                 type: "status",
                                 stage: "pending",
                                 queue: !0,
-                                endpoint: D,
+                                endpoint: R,
                                 fn_index: T,
                                 time: /* @__PURE__ */ new Date()
                             }), n(
-                                `${v.root}/queue/join?${he}`, {
-                                    ...H,
-                                    session_hash: b
+                                `${v.root}/queue/join?${j}`, {
+                                    ...Se,
+                                    session_hash: p
                                 },
                                 f
-                            ).then(([ne, Y]) => {
-                                if (Y === 503)
-                                    q({
+                            ).then(([ne, Z]) => {
+                                if (Z === 503)
+                                    M({
                                         type: "status",
                                         stage: "error",
                                         message: Zr,
                                         queue: !0,
-                                        endpoint: D,
+                                        endpoint: R,
                                         fn_index: T,
                                         time: /* @__PURE__ */ new Date()
                                     });
-                                else if (Y !== 200)
-                                    q({
+                                else if (Z !== 200)
+                                    M({
                                         type: "status",
                                         stage: "error",
-                                        message: gt,
+                                        message: bt,
                                         queue: !0,
-                                        endpoint: D,
+                                        endpoint: R,
                                         fn_index: T,
                                         time: /* @__PURE__ */ new Date()
                                     });
                                 else {
-                                    R = ne.event_id;
-                                    let de = async function(ue) {
+                                    H = ne.event_id;
+                                    let he = async function(ue) {
                                         try {
                                             const {
                                                 type: V,
-                                                status: Z,
-                                                data: mt
+                                                status: W,
+                                                data: gt
                                             } = ml(
                                                 ue,
-                                                p[T]
+                                                g[T]
                                             );
                                             if (V == "heartbeat")
                                                 return;
-                                            if (V === "update" && Z && !j)
-                                                q({
+                                            if (V === "update" && W && !U)
+                                                M({
                                                     type: "status",
-                                                    endpoint: D,
+                                                    endpoint: R,
                                                     fn_index: T,
                                                     time: /* @__PURE__ */ new Date(),
-                                                    ...Z
+                                                    ...W
                                                 });
                                             else if (V === "complete")
-                                                j = Z;
+                                                U = W;
                                             else if (V == "unexpected_error")
-                                                console.error("Unexpected error", Z == null ? void 0 : Z.message), q({
+                                                console.error("Unexpected error", W == null ? void 0 : W.message), M({
                                                     type: "status",
                                                     stage: "error",
-                                                    message: (Z == null ? void 0 : Z.message) || "An Unexpected Error Occurred!",
+                                                    message: (W == null ? void 0 : W.message) || "An Unexpected Error Occurred!",
                                                     queue: !0,
-                                                    endpoint: D,
+                                                    endpoint: R,
                                                     fn_index: T,
                                                     time: /* @__PURE__ */ new Date()
                                                 });
                                             else if (V === "log") {
-                                                q({
+                                                M({
                                                     type: "log",
-                                                    log: mt.log,
-                                                    level: mt.level,
-                                                    endpoint: D,
+                                                    log: gt.log,
+                                                    level: gt.level,
+                                                    endpoint: R,
                                                     fn_index: T
                                                 });
                                                 return;
                                             } else
-                                                V === "generating" && (q({
+                                                V === "generating" && (M({
                                                     type: "status",
                                                     time: /* @__PURE__ */ new Date(),
-                                                    ...Z,
-                                                    stage: Z == null ? void 0 : Z.stage,
+                                                    ...W,
+                                                    stage: W == null ? void 0 : W.stage,
                                                     queue: !0,
-                                                    endpoint: D,
+                                                    endpoint: R,
                                                     fn_index: T
-                                                }), mt && He === "sse_v2" && Me(R, mt));
-                                            mt && (q({
+                                                }), gt && He === "sse_v2" && je(H, gt));
+                                            gt && (M({
                                                 type: "data",
                                                 time: /* @__PURE__ */ new Date(),
-                                                data: mt.data,
-                                                endpoint: D,
+                                                data: gt.data,
+                                                endpoint: R,
                                                 fn_index: T
-                                            }), j && q({
+                                            }), U && M({
                                                 type: "status",
                                                 time: /* @__PURE__ */ new Date(),
-                                                ...j,
-                                                stage: Z == null ? void 0 : Z.stage,
+                                                ...U,
+                                                stage: W == null ? void 0 : W.stage,
                                                 queue: !0,
-                                                endpoint: D,
+                                                endpoint: R,
                                                 fn_index: T
-                                            })), ((Z == null ? void 0 : Z.stage) === "complete" || (Z == null ? void 0 : Z.stage) === "error") && (E[R] && delete E[R], R in C && delete C[R]);
+                                            })), ((W == null ? void 0 : W.stage) === "complete" || (W == null ? void 0 : W.stage) === "error") && (E[H] && delete E[H], H in C && delete C[H]);
                                         } catch (V) {
-                                            console.error("Unexpected client exception", V), q({
+                                            console.error("Unexpected client exception", V), M({
                                                 type: "status",
                                                 stage: "error",
                                                 message: "An Unexpected Error Occurred!",
                                                 queue: !0,
-                                                endpoint: D,
+                                                endpoint: R,
                                                 fn_index: T,
                                                 time: /* @__PURE__ */ new Date()
-                                            }), ye();
+                                            }), ve();
                                         }
                                     };
-                                    R in w && (w[R].forEach(
-                                        (ue) => de(ue)
-                                    ), delete w[R]), E[R] = de, N.add(R), y || ke();
+                                    H in w && (w[H].forEach(
+                                        (ue) => he(ue)
+                                    ), delete w[H]), E[H] = he, N.add(H), y || Ee();
                                 }
                             }));
                     }
                 );
 
-                function Me(K, ge) {
-                    !C[K] ? (C[K] = [], ge.data.forEach((Y, de) => {
-                        C[K][de] = Y;
-                    })) : ge.data.forEach((Y, de) => {
+                function je(K, me) {
+                    !C[K] ? (C[K] = [], me.data.forEach((Z, he) => {
+                        C[K][he] = Z;
+                    })) : me.data.forEach((Z, he) => {
                         let ue = Wh(
-                            C[K][de],
-                            Y
+                            C[K][he],
+                            Z
                         );
-                        C[K][de] = ue, ge.data[de] = ue;
+                        C[K][he] = ue, me.data[he] = ue;
                     });
                 }
 
-                function q(K) {
-                    const ne = X[K.type] || [];
-                    ne == null || ne.forEach((Y) => Y(K));
+                function M(K) {
+                    const ne = Q[K.type] || [];
+                    ne == null || ne.forEach((Z) => Z(K));
                 }
 
-                function Vi(K, ge) {
-                    const ne = X,
-                        Y = ne[K] || [];
-                    return ne[K] = Y, Y == null || Y.push(ge), {
-                        on: Vi,
-                        off: xn,
-                        cancel: Xi,
-                        destroy: Wi
+                function tt(K, me) {
+                    const ne = Q,
+                        Z = ne[K] || [];
+                    return ne[K] = Z, Z == null || Z.push(me), {
+                        on: tt,
+                        off: Ut,
+                        cancel: bn,
+                        destroy: pn
                     };
                 }
 
-                function xn(K, ge) {
-                    const ne = X;
-                    let Y = ne[K] || [];
-                    return Y = Y == null ? void 0 : Y.filter((de) => de !== ge), ne[K] = Y, {
-                        on: Vi,
-                        off: xn,
-                        cancel: Xi,
-                        destroy: Wi
+                function Ut(K, me) {
+                    const ne = Q;
+                    let Z = ne[K] || [];
+                    return Z = Z == null ? void 0 : Z.filter((he) => he !== me), ne[K] = Z, {
+                        on: tt,
+                        off: Ut,
+                        cancel: bn,
+                        destroy: pn
                     };
                 }
-                async function Xi() {
+                async function bn() {
                     const K = {
                         stage: "complete",
                         queue: !1,
                         time: /* @__PURE__ */ new Date()
                     };
-                    j = K, q({
+                    U = K, M({
                         ...K,
                         type: "status",
-                        endpoint: D,
+                        endpoint: R,
                         fn_index: T
                     });
-                    let ge = {};
-                    He === "ws" ? (Q && Q.readyState === 0 ? Q.addEventListener("open", () => {
-                        Q.close();
-                    }) : Q.close(), ge = {
+                    let me = {};
+                    He === "ws" ? (J && J.readyState === 0 ? J.addEventListener("open", () => {
+                        J.close();
+                    }) : J.close(), me = {
                         fn_index: T,
-                        session_hash: b
-                    }) : (Se.close(), ge = {
-                        event_id: R
+                        session_hash: p
+                    }) : (ke.close(), me = {
+                        event_id: H
                     });
                     try {
                         await t(`${v.root}/reset`, {
                             headers: {
                                 "Content-Type": "application/json"
                             },
                             method: "POST",
-                            body: JSON.stringify(ge)
+                            body: JSON.stringify(me)
                         });
                     } catch {
                         console.warn(
                             "The `/reset` endpoint could not be called. Subsequent endpoint results may be unreliable."
                         );
                     }
                 }
 
-                function Wi() {
-                    for (const K in X)
-                        X[K].forEach((ge) => {
-                            xn(K, ge);
+                function pn() {
+                    for (const K in Q)
+                        Q[K].forEach((me) => {
+                            Ut(K, me);
                         });
                 }
                 return {
-                    on: Vi,
-                    off: xn,
-                    cancel: Xi,
-                    destroy: Wi
+                    on: tt,
+                    off: Ut,
+                    cancel: bn,
+                    destroy: pn
                 };
             }
 
-            function ke() {
+            function Ee() {
                 y = !0;
                 let S = new URLSearchParams({
-                        session_hash: b
+                        session_hash: p
                     }).toString(),
                     k = new URL(`${v.root}/queue/data?${S}`);
                 P = e(k), P.onmessage = async function(I) {
-                    let g = JSON.parse(I.data);
-                    const T = g.event_id;
+                    let m = JSON.parse(I.data);
+                    const T = m.event_id;
                     if (!T)
                         await Promise.all(
                             Object.keys(E).map(
-                                (ae) => E[ae](g)
+                                (ae) => E[ae](m)
                             )
                         );
                     else if (E[T]) {
-                        g.msg === "process_completed" && (N.delete(T), N.size === 0 && ye());
+                        m.msg === "process_completed" && (N.delete(T), N.size === 0 && ve());
                         let ae = E[T];
-                        window.setTimeout(ae, 0, g);
+                        window.setTimeout(ae, 0, m);
                     } else
-                        w[T] || (w[T] = []), w[T].push(g);
+                        w[T] || (w[T] = []), w[T].push(m);
                 }, P.onerror = async function(I) {
                     await Promise.all(
                         Object.keys(E).map(
-                            (g) => E[g]({
+                            (m) => E[m]({
                                 msg: "unexpected_error",
-                                message: gt
+                                message: bt
                             })
                         )
-                    ), ye();
+                    ), ve();
                 };
             }
 
-            function ye() {
+            function ve() {
                 y = !1, P == null || P.close();
             }
-            async function me(S, k, I) {
-                var g;
+            async function de(S, k, I) {
+                var m;
                 const T = {
                     "Content-Type": "application/json"
                 };
                 f && (T.Authorization = `Bearer ${f}`);
-                let ae, Q = v.components.find(
-                    (D) => D.id === S
+                let ae, J = v.components.find(
+                    (R) => R.id === S
                 );
-                (g = Q == null ? void 0 : Q.props) != null && g.root_url ? ae = Q.props.root_url : ae = v.root;
-                const Se = await t(
+                (m = J == null ? void 0 : J.props) != null && m.root_url ? ae = J.props.root_url : ae = v.root;
+                const ke = await t(
                     `${ae}/component_server/`, {
                         method: "POST",
                         body: JSON.stringify({
                             data: I,
                             component_id: S,
                             fn_name: k,
-                            session_hash: b
+                            session_hash: p
                         }),
                         headers: T
                     }
                 );
-                if (!Se.ok)
+                if (!ke.ok)
                     throw new Error(
-                        "Could not connect to component server: " + Se.statusText
+                        "Could not connect to component server: " + ke.statusText
                     );
-                return await Se.json();
+                return await ke.json();
             }
-            async function _e(S) {
+            async function ce(S) {
                 if (x)
                     return x;
                 const k = {
                     "Content-Type": "application/json"
                 };
                 f && (k.Authorization = `Bearer ${f}`);
                 let I;
@@ -5313,17 +5313,17 @@
                                 config: JSON.stringify(S)
                             }),
                             headers: k
                         }
                     ) : I = await t(`${S.root}/info`, {
                         headers: k
                     }), !I.ok)
-                    throw new Error(gt);
-                let g = await I.json();
-                return "api" in g && (g = g.api), g.named_endpoints["/predict"] && !g.unnamed_endpoints[0] && (g.unnamed_endpoints[0] = g.named_endpoints["/predict"]), Kh(g, S, A);
+                    throw new Error(bt);
+                let m = await I.json();
+                return "api" in m && (m = m.api), m.named_endpoints["/predict"] && !m.unnamed_endpoints[0] && (m.unnamed_endpoints[0] = m.named_endpoints["/predict"]), Kh(m, S, A);
             }
         });
     }
     async function s(o, r, a, u) {
         const f = await Gl(
             r,
             void 0,
@@ -5351,24 +5351,24 @@
                     type: c
                 };
             })
         ).then((_) => (_.forEach(({
             path: h,
             file_url: c,
             type: d,
-            name: m
+            name: b
         }) => {
             if (d === "Gallery")
                 bo(r, c, h);
             else if (c) {
-                const b = new hs({
+                const p = new hs({
                     path: c,
-                    orig_name: m
+                    orig_name: b
                 });
-                bo(r, b, h);
+                bo(r, p, h);
             }
         }), r));
     }
 }
 const {
     post_data: fb,
     upload_files: Qh,
@@ -5749,29 +5749,29 @@
     return t.$$typeof === o0;
 }
 
 function a0(t) {
     return Array.isArray(t) ? [] : {};
 }
 
-function Mn(t, e) {
-    return e.clone !== !1 && e.isMergeableObject(t) ? on(a0(t), t, e) : t;
+function Un(t, e) {
+    return e.clone !== !1 && e.isMergeableObject(t) ? an(a0(t), t, e) : t;
 }
 
 function u0(t, e, n) {
     return t.concat(e).map(function(i) {
-        return Mn(i, n);
+        return Un(i, n);
     });
 }
 
 function f0(t, e) {
     if (!e.customMerge)
-        return on;
+        return an;
     var n = e.customMerge(t);
-    return typeof n == "function" ? n : on;
+    return typeof n == "function" ? n : an;
 }
 
 function c0(t) {
     return Object.getOwnPropertySymbols ? Object.getOwnPropertySymbols(t).filter(function(e) {
         return Object.propertyIsEnumerable.call(t, e);
     }) : [];
 }
@@ -5791,50 +5791,50 @@
 function _0(t, e) {
     return Jr(t, e) && !(Object.hasOwnProperty.call(t, e) && Object.propertyIsEnumerable.call(t, e));
 }
 
 function h0(t, e, n) {
     var i = {};
     return n.isMergeableObject(t) && wo(t).forEach(function(l) {
-        i[l] = Mn(t[l], n);
+        i[l] = Un(t[l], n);
     }), wo(e).forEach(function(l) {
-        _0(t, l) || (Jr(t, l) && n.isMergeableObject(e[l]) ? i[l] = f0(l, n)(t[l], e[l], n) : i[l] = Mn(e[l], n));
+        _0(t, l) || (Jr(t, l) && n.isMergeableObject(e[l]) ? i[l] = f0(l, n)(t[l], e[l], n) : i[l] = Un(e[l], n));
     }), i;
 }
 
-function on(t, e, n) {
-    n = n || {}, n.arrayMerge = n.arrayMerge || u0, n.isMergeableObject = n.isMergeableObject || n0, n.cloneUnlessOtherwiseSpecified = Mn;
+function an(t, e, n) {
+    n = n || {}, n.arrayMerge = n.arrayMerge || u0, n.isMergeableObject = n.isMergeableObject || n0, n.cloneUnlessOtherwiseSpecified = Un;
     var i = Array.isArray(e),
         l = Array.isArray(t),
         s = i === l;
-    return s ? i ? n.arrayMerge(t, e, n) : h0(t, e, n) : Mn(e, n);
+    return s ? i ? n.arrayMerge(t, e, n) : h0(t, e, n) : Un(e, n);
 }
-on.all = function(e, n) {
+an.all = function(e, n) {
     if (!Array.isArray(e))
         throw new Error("first argument should be an array");
     return e.reduce(function(i, l) {
-        return on(i, l, n);
+        return an(i, l, n);
     }, {});
 };
-var d0 = on,
+var d0 = an,
     m0 = d0;
 const g0 = /* @__PURE__ */ t0(m0);
 var Vl = function(t, e) {
     return Vl = Object.setPrototypeOf || {
         __proto__: []
     }
     instanceof Array && function(n, i) {
         n.__proto__ = i;
     } || function(n, i) {
         for (var l in i)
             Object.prototype.hasOwnProperty.call(i, l) && (n[l] = i[l]);
     }, Vl(t, e);
 };
 
-function Ui(t, e) {
+function zi(t, e) {
     if (typeof e != "function" && e !== null)
         throw new TypeError("Class extends value " + String(e) + " is not a constructor or null");
     Vl(t, e);
 
     function n() {
         this.constructor = t;
     }
@@ -5853,26 +5853,26 @@
 
 function gl(t, e, n) {
     if (n || arguments.length === 2)
         for (var i = 0, l = e.length, s; i < l; i++)
             (s || !(i in e)) && (s || (s = Array.prototype.slice.call(e, 0, i)), s[i] = e[i]);
     return t.concat(s || Array.prototype.slice.call(e));
 }
-var U;
+var F;
 (function(t) {
     t[t.EXPECT_ARGUMENT_CLOSING_BRACE = 1] = "EXPECT_ARGUMENT_CLOSING_BRACE", t[t.EMPTY_ARGUMENT = 2] = "EMPTY_ARGUMENT", t[t.MALFORMED_ARGUMENT = 3] = "MALFORMED_ARGUMENT", t[t.EXPECT_ARGUMENT_TYPE = 4] = "EXPECT_ARGUMENT_TYPE", t[t.INVALID_ARGUMENT_TYPE = 5] = "INVALID_ARGUMENT_TYPE", t[t.EXPECT_ARGUMENT_STYLE = 6] = "EXPECT_ARGUMENT_STYLE", t[t.INVALID_NUMBER_SKELETON = 7] = "INVALID_NUMBER_SKELETON", t[t.INVALID_DATE_TIME_SKELETON = 8] = "INVALID_DATE_TIME_SKELETON", t[t.EXPECT_NUMBER_SKELETON = 9] = "EXPECT_NUMBER_SKELETON", t[t.EXPECT_DATE_TIME_SKELETON = 10] = "EXPECT_DATE_TIME_SKELETON", t[t.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE = 11] = "UNCLOSED_QUOTE_IN_ARGUMENT_STYLE", t[t.EXPECT_SELECT_ARGUMENT_OPTIONS = 12] = "EXPECT_SELECT_ARGUMENT_OPTIONS", t[t.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE = 13] = "EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE", t[t.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE = 14] = "INVALID_PLURAL_ARGUMENT_OFFSET_VALUE", t[t.EXPECT_SELECT_ARGUMENT_SELECTOR = 15] = "EXPECT_SELECT_ARGUMENT_SELECTOR", t[t.EXPECT_PLURAL_ARGUMENT_SELECTOR = 16] = "EXPECT_PLURAL_ARGUMENT_SELECTOR", t[t.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT = 17] = "EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT", t[t.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT = 18] = "EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT", t[t.INVALID_PLURAL_ARGUMENT_SELECTOR = 19] = "INVALID_PLURAL_ARGUMENT_SELECTOR", t[t.DUPLICATE_PLURAL_ARGUMENT_SELECTOR = 20] = "DUPLICATE_PLURAL_ARGUMENT_SELECTOR", t[t.DUPLICATE_SELECT_ARGUMENT_SELECTOR = 21] = "DUPLICATE_SELECT_ARGUMENT_SELECTOR", t[t.MISSING_OTHER_CLAUSE = 22] = "MISSING_OTHER_CLAUSE", t[t.INVALID_TAG = 23] = "INVALID_TAG", t[t.INVALID_TAG_NAME = 25] = "INVALID_TAG_NAME", t[t.UNMATCHED_CLOSING_TAG = 26] = "UNMATCHED_CLOSING_TAG", t[t.UNCLOSED_TAG = 27] = "UNCLOSED_TAG";
-})(U || (U = {}));
+})(F || (F = {}));
 var ee;
 (function(t) {
     t[t.literal = 0] = "literal", t[t.argument = 1] = "argument", t[t.number = 2] = "number", t[t.date = 3] = "date", t[t.time = 4] = "time", t[t.select = 5] = "select", t[t.plural = 6] = "plural", t[t.pound = 7] = "pound", t[t.tag = 8] = "tag";
 })(ee || (ee = {}));
-var rn;
+var un;
 (function(t) {
     t[t.number = 0] = "number", t[t.dateTime = 1] = "dateTime";
-})(rn || (rn = {}));
+})(un || (un = {}));
 
 function vo(t) {
     return t.type === ee.literal;
 }
 
 function b0(t) {
     return t.type === ee.argument;
@@ -5903,19 +5903,19 @@
 }
 
 function na(t) {
     return t.type === ee.tag;
 }
 
 function ia(t) {
-    return !!(t && typeof t == "object" && t.type === rn.number);
+    return !!(t && typeof t == "object" && t.type === un.number);
 }
 
 function Xl(t) {
-    return !!(t && typeof t == "object" && t.type === rn.dateTime);
+    return !!(t && typeof t == "object" && t.type === un.dateTime);
 }
 var la = /[ \xA0\u1680\u2000-\u200A\u202F\u205F\u3000]/,
     w0 = /(?:[Eec]{1,6}|G{1,5}|[Qq]{1,5}|(?:[yYur]+|U{1,5})|[ML]{1,5}|d{1,2}|D{1,3}|F{1}|[abB]{1,5}|[hkHK]{1,2}|w{1,2}|W{1}|m{1,2}|s{1,2}|[zZOvVxX]{1,4})(?=([^']*'[^']*')*[^']*$)/g;
 
 function v0(t) {
     var e = {};
     return t.replace(w0, function(n) {
@@ -6214,15 +6214,15 @@
         var o = ra(l.stem);
         o && (e = G(G({}, e), o));
         var r = C0(l.stem);
         r && (e = G(G({}, e), r));
     }
     return e;
 }
-var $n = {
+var ni = {
     AX: [
         "H"
     ],
     BQ: [
         "H"
     ],
     CP: [
@@ -7592,21 +7592,21 @@
                 return "K";
             default:
                 throw new Error("Invalid hourCycle");
         }
     var n = t.language,
         i;
     n !== "root" && (i = t.maximize().region);
-    var l = $n[i || ""] || $n[n || ""] || $n["".concat(n, "-001")] || $n["001"];
+    var l = ni[i || ""] || ni[n || ""] || ni["".concat(n, "-001")] || ni["001"];
     return l[0];
 }
 var bl, H0 = new RegExp("^".concat(la.source, "*")),
     P0 = new RegExp("".concat(la.source, "*$"));
 
-function F(t, e) {
+function q(t, e) {
     return {
         start: t,
         end: e
     };
 }
 var N0 = !!String.prototype.startsWith,
     L0 = !!String.fromCodePoint,
@@ -7750,20 +7750,20 @@
                 } else {
                     if (s === 125 && e > 0)
                         break;
                     if (s === 35 && (n === "plural" || n === "selectordinal")) {
                         var r = this.clonePosition();
                         this.bump(), l.push({
                             type: ee.pound,
-                            location: F(r, this.clonePosition())
+                            location: q(r, this.clonePosition())
                         });
                     } else if (s === 60 && !this.ignoreTag && this.peek() === 47) {
                         if (i)
                             break;
-                        return this.error(U.UNMATCHED_CLOSING_TAG, F(this.clonePosition(), this.clonePosition()));
+                        return this.error(F.UNMATCHED_CLOSING_TAG, q(this.clonePosition(), this.clonePosition()));
                     } else if (s === 60 && !this.ignoreTag && Jl(this.peek() || 0)) {
                         var o = this.parseTag(e, n);
                         if (o.err)
                             return o;
                         l.push(o.val);
                     } else {
                         var o = this.parseLiteral(e, n);
@@ -7782,42 +7782,42 @@
             this.bump();
             var l = this.parseTagName();
             if (this.bumpSpace(), this.bumpIf("/>"))
                 return {
                     val: {
                         type: ee.literal,
                         value: "<".concat(l, "/>"),
-                        location: F(i, this.clonePosition())
+                        location: q(i, this.clonePosition())
                     },
                     err: null
                 };
             if (this.bumpIf(">")) {
                 var s = this.parseMessage(e + 1, n, !0);
                 if (s.err)
                     return s;
                 var o = s.val,
                     r = this.clonePosition();
                 if (this.bumpIf("</")) {
                     if (this.isEOF() || !Jl(this.char()))
-                        return this.error(U.INVALID_TAG, F(r, this.clonePosition()));
+                        return this.error(F.INVALID_TAG, q(r, this.clonePosition()));
                     var a = this.clonePosition(),
                         u = this.parseTagName();
-                    return l !== u ? this.error(U.UNMATCHED_CLOSING_TAG, F(a, this.clonePosition())) : (this.bumpSpace(), this.bumpIf(">") ? {
+                    return l !== u ? this.error(F.UNMATCHED_CLOSING_TAG, q(a, this.clonePosition())) : (this.bumpSpace(), this.bumpIf(">") ? {
                         val: {
                             type: ee.tag,
                             value: l,
                             children: o,
-                            location: F(i, this.clonePosition())
+                            location: q(i, this.clonePosition())
                         },
                         err: null
-                    } : this.error(U.INVALID_TAG, F(r, this.clonePosition())));
+                    } : this.error(F.INVALID_TAG, q(r, this.clonePosition())));
                 } else
-                    return this.error(U.UNCLOSED_TAG, F(i, this.clonePosition()));
+                    return this.error(F.UNCLOSED_TAG, q(i, this.clonePosition()));
             } else
-                return this.error(U.INVALID_TAG, F(i, this.clonePosition()));
+                return this.error(F.INVALID_TAG, q(i, this.clonePosition()));
         }, t.prototype.parseTagName = function() {
             var e = this.offset();
             for (this.bump(); !this.isEOF() && x0(this.char());)
                 this.bump();
             return this.message.slice(e, this.offset());
         }, t.prototype.parseLiteral = function(e, n) {
             for (var i = this.clonePosition(), l = "";;) {
@@ -7834,15 +7834,15 @@
                 var r = this.tryParseLeftAngleBracket();
                 if (r) {
                     l += r;
                     continue;
                 }
                 break;
             }
-            var a = F(i, this.clonePosition());
+            var a = q(i, this.clonePosition());
             return {
                 val: {
                     type: ee.literal,
                     value: l,
                     location: a
                 },
                 err: null
@@ -7888,152 +7888,152 @@
             if (this.isEOF())
                 return null;
             var i = this.char();
             return i === 60 || i === 123 || i === 35 && (n === "plural" || n === "selectordinal") || i === 125 && e > 0 ? null : (this.bump(), Zl(i));
         }, t.prototype.parseArgument = function(e, n) {
             var i = this.clonePosition();
             if (this.bump(), this.bumpSpace(), this.isEOF())
-                return this.error(U.EXPECT_ARGUMENT_CLOSING_BRACE, F(i, this.clonePosition()));
+                return this.error(F.EXPECT_ARGUMENT_CLOSING_BRACE, q(i, this.clonePosition()));
             if (this.char() === 125)
-                return this.bump(), this.error(U.EMPTY_ARGUMENT, F(i, this.clonePosition()));
+                return this.bump(), this.error(F.EMPTY_ARGUMENT, q(i, this.clonePosition()));
             var l = this.parseIdentifierIfPossible().value;
             if (!l)
-                return this.error(U.MALFORMED_ARGUMENT, F(i, this.clonePosition()));
+                return this.error(F.MALFORMED_ARGUMENT, q(i, this.clonePosition()));
             if (this.bumpSpace(), this.isEOF())
-                return this.error(U.EXPECT_ARGUMENT_CLOSING_BRACE, F(i, this.clonePosition()));
+                return this.error(F.EXPECT_ARGUMENT_CLOSING_BRACE, q(i, this.clonePosition()));
             switch (this.char()) {
                 case 125:
                     return this.bump(), {
                         val: {
                             type: ee.argument,
                             // value does not include the opening and closing braces.
                             value: l,
-                            location: F(i, this.clonePosition())
+                            location: q(i, this.clonePosition())
                         },
                         err: null
                     };
                 case 44:
-                    return this.bump(), this.bumpSpace(), this.isEOF() ? this.error(U.EXPECT_ARGUMENT_CLOSING_BRACE, F(i, this.clonePosition())) : this.parseArgumentOptions(e, n, l, i);
+                    return this.bump(), this.bumpSpace(), this.isEOF() ? this.error(F.EXPECT_ARGUMENT_CLOSING_BRACE, q(i, this.clonePosition())) : this.parseArgumentOptions(e, n, l, i);
                 default:
-                    return this.error(U.MALFORMED_ARGUMENT, F(i, this.clonePosition()));
+                    return this.error(F.MALFORMED_ARGUMENT, q(i, this.clonePosition()));
             }
         }, t.prototype.parseIdentifierIfPossible = function() {
             var e = this.clonePosition(),
                 n = this.offset(),
                 i = Yl(this.message, n),
                 l = n + i.length;
             this.bumpTo(l);
             var s = this.clonePosition(),
-                o = F(e, s);
+                o = q(e, s);
             return {
                 value: i,
                 location: o
             };
         }, t.prototype.parseArgumentOptions = function(e, n, i, l) {
             var s, o = this.clonePosition(),
                 r = this.parseIdentifierIfPossible().value,
                 a = this.clonePosition();
             switch (r) {
                 case "":
-                    return this.error(U.EXPECT_ARGUMENT_TYPE, F(o, a));
+                    return this.error(F.EXPECT_ARGUMENT_TYPE, q(o, a));
                 case "number":
                 case "date":
                 case "time": {
                     this.bumpSpace();
                     var u = null;
                     if (this.bumpIf(",")) {
                         this.bumpSpace();
                         var f = this.clonePosition(),
                             _ = this.parseSimpleArgStyleIfPossible();
                         if (_.err)
                             return _;
                         var h = z0(_.val);
                         if (h.length === 0)
-                            return this.error(U.EXPECT_ARGUMENT_STYLE, F(this.clonePosition(), this.clonePosition()));
-                        var c = F(f, this.clonePosition());
+                            return this.error(F.EXPECT_ARGUMENT_STYLE, q(this.clonePosition(), this.clonePosition()));
+                        var c = q(f, this.clonePosition());
                         u = {
                             style: h,
                             styleLocation: c
                         };
                     }
                     var d = this.tryParseArgumentClose(l);
                     if (d.err)
                         return d;
-                    var m = F(l, this.clonePosition());
+                    var b = q(l, this.clonePosition());
                     if (u && So(u == null ? void 0 : u.style, "::", 0)) {
-                        var b = q0(u.style.slice(2));
+                        var p = q0(u.style.slice(2));
                         if (r === "number") {
-                            var _ = this.parseNumberSkeletonFromString(b, u.styleLocation);
+                            var _ = this.parseNumberSkeletonFromString(p, u.styleLocation);
                             return _.err ? _ : {
                                 val: {
                                     type: ee.number,
                                     value: i,
-                                    location: m,
+                                    location: b,
                                     style: _.val
                                 },
                                 err: null
                             };
                         } else {
-                            if (b.length === 0)
-                                return this.error(U.EXPECT_DATE_TIME_SKELETON, m);
-                            var p = b;
-                            this.locale && (p = B0(b, this.locale));
+                            if (p.length === 0)
+                                return this.error(F.EXPECT_DATE_TIME_SKELETON, b);
+                            var g = p;
+                            this.locale && (g = B0(p, this.locale));
                             var h = {
-                                    type: rn.dateTime,
-                                    pattern: p,
+                                    type: un.dateTime,
+                                    pattern: g,
                                     location: u.styleLocation,
-                                    parsedOptions: this.shouldParseSkeletons ? v0(p) : {}
+                                    parsedOptions: this.shouldParseSkeletons ? v0(g) : {}
                                 },
                                 y = r === "date" ? ee.date : ee.time;
                             return {
                                 val: {
                                     type: y,
                                     value: i,
-                                    location: m,
+                                    location: b,
                                     style: h
                                 },
                                 err: null
                             };
                         }
                     }
                     return {
                         val: {
                             type: r === "number" ? ee.number : r === "date" ? ee.date : ee.time,
                             value: i,
-                            location: m,
+                            location: b,
                             style: (s = u == null ? void 0 : u.style) !== null && s !== void 0 ? s : null
                         },
                         err: null
                     };
                 }
                 case "plural":
                 case "selectordinal":
                 case "select": {
                     var w = this.clonePosition();
                     if (this.bumpSpace(), !this.bumpIf(","))
-                        return this.error(U.EXPECT_SELECT_ARGUMENT_OPTIONS, F(w, G({}, w)));
+                        return this.error(F.EXPECT_SELECT_ARGUMENT_OPTIONS, q(w, G({}, w)));
                     this.bumpSpace();
                     var C = this.parseIdentifierIfPossible(),
                         P = 0;
                     if (r !== "select" && C.value === "offset") {
                         if (!this.bumpIf(":"))
-                            return this.error(U.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, F(this.clonePosition(), this.clonePosition()));
+                            return this.error(F.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, q(this.clonePosition(), this.clonePosition()));
                         this.bumpSpace();
-                        var _ = this.tryParseDecimalInteger(U.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, U.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE);
+                        var _ = this.tryParseDecimalInteger(F.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, F.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE);
                         if (_.err)
                             return _;
                         this.bumpSpace(), C = this.parseIdentifierIfPossible(), P = _.val;
                     }
                     var E = this.tryParsePluralOrSelectOptions(e, r, n, C);
                     if (E.err)
                         return E;
                     var d = this.tryParseArgumentClose(l);
                     if (d.err)
                         return d;
-                    var N = F(l, this.clonePosition());
+                    var N = q(l, this.clonePosition());
                     return r === "select" ? {
                         val: {
                             type: ee.select,
                             value: i,
                             options: Co(E.val),
                             location: N
                         },
@@ -8047,30 +8047,30 @@
                             pluralType: r === "plural" ? "cardinal" : "ordinal",
                             location: N
                         },
                         err: null
                     };
                 }
                 default:
-                    return this.error(U.INVALID_ARGUMENT_TYPE, F(o, a));
+                    return this.error(F.INVALID_ARGUMENT_TYPE, q(o, a));
             }
         }, t.prototype.tryParseArgumentClose = function(e) {
-            return this.isEOF() || this.char() !== 125 ? this.error(U.EXPECT_ARGUMENT_CLOSING_BRACE, F(e, this.clonePosition())) : (this.bump(), {
+            return this.isEOF() || this.char() !== 125 ? this.error(F.EXPECT_ARGUMENT_CLOSING_BRACE, q(e, this.clonePosition())) : (this.bump(), {
                 val: !0,
                 err: null
             });
         }, t.prototype.parseSimpleArgStyleIfPossible = function() {
             for (var e = 0, n = this.clonePosition(); !this.isEOF();) {
                 var i = this.char();
                 switch (i) {
                     case 39: {
                         this.bump();
                         var l = this.clonePosition();
                         if (!this.bumpUntil("'"))
-                            return this.error(U.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE, F(l, this.clonePosition()));
+                            return this.error(F.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE, q(l, this.clonePosition()));
                         this.bump();
                         break;
                     }
                     case 123: {
                         e += 1, this.bump();
                         break;
                     }
@@ -8094,72 +8094,72 @@
                 err: null
             };
         }, t.prototype.parseNumberSkeletonFromString = function(e, n) {
             var i = [];
             try {
                 i = E0(e);
             } catch {
-                return this.error(U.INVALID_NUMBER_SKELETON, n);
+                return this.error(F.INVALID_NUMBER_SKELETON, n);
             }
             return {
                 val: {
-                    type: rn.number,
+                    type: un.number,
                     tokens: i,
                     location: n,
                     parsedOptions: this.shouldParseSkeletons ? A0(i) : {}
                 },
                 err: null
             };
         }, t.prototype.tryParsePluralOrSelectOptions = function(e, n, i, l) {
             for (var s, o = !1, r = [], a = /* @__PURE__ */ new Set(), u = l.value, f = l.location;;) {
                 if (u.length === 0) {
                     var _ = this.clonePosition();
                     if (n !== "select" && this.bumpIf("=")) {
-                        var h = this.tryParseDecimalInteger(U.EXPECT_PLURAL_ARGUMENT_SELECTOR, U.INVALID_PLURAL_ARGUMENT_SELECTOR);
+                        var h = this.tryParseDecimalInteger(F.EXPECT_PLURAL_ARGUMENT_SELECTOR, F.INVALID_PLURAL_ARGUMENT_SELECTOR);
                         if (h.err)
                             return h;
-                        f = F(_, this.clonePosition()), u = this.message.slice(_.offset, this.offset());
+                        f = q(_, this.clonePosition()), u = this.message.slice(_.offset, this.offset());
                     } else
                         break;
                 }
                 if (a.has(u))
-                    return this.error(n === "select" ? U.DUPLICATE_SELECT_ARGUMENT_SELECTOR : U.DUPLICATE_PLURAL_ARGUMENT_SELECTOR, f);
+                    return this.error(n === "select" ? F.DUPLICATE_SELECT_ARGUMENT_SELECTOR : F.DUPLICATE_PLURAL_ARGUMENT_SELECTOR, f);
                 u === "other" && (o = !0), this.bumpSpace();
                 var c = this.clonePosition();
                 if (!this.bumpIf("{"))
-                    return this.error(n === "select" ? U.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT : U.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT, F(this.clonePosition(), this.clonePosition()));
+                    return this.error(n === "select" ? F.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT : F.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT, q(this.clonePosition(), this.clonePosition()));
                 var d = this.parseMessage(e + 1, n, i);
                 if (d.err)
                     return d;
-                var m = this.tryParseArgumentClose(c);
-                if (m.err)
-                    return m;
+                var b = this.tryParseArgumentClose(c);
+                if (b.err)
+                    return b;
                 r.push([
                     u, {
                         value: d.val,
-                        location: F(c, this.clonePosition())
+                        location: q(c, this.clonePosition())
                     }
                 ]), a.add(u), this.bumpSpace(), s = this.parseIdentifierIfPossible(), u = s.value, f = s.location;
             }
-            return r.length === 0 ? this.error(n === "select" ? U.EXPECT_SELECT_ARGUMENT_SELECTOR : U.EXPECT_PLURAL_ARGUMENT_SELECTOR, F(this.clonePosition(), this.clonePosition())) : this.requiresOtherClause && !o ? this.error(U.MISSING_OTHER_CLAUSE, F(this.clonePosition(), this.clonePosition())) : {
+            return r.length === 0 ? this.error(n === "select" ? F.EXPECT_SELECT_ARGUMENT_SELECTOR : F.EXPECT_PLURAL_ARGUMENT_SELECTOR, q(this.clonePosition(), this.clonePosition())) : this.requiresOtherClause && !o ? this.error(F.MISSING_OTHER_CLAUSE, q(this.clonePosition(), this.clonePosition())) : {
                 val: r,
                 err: null
             };
         }, t.prototype.tryParseDecimalInteger = function(e, n) {
             var i = 1,
                 l = this.clonePosition();
             this.bumpIf("+") || this.bumpIf("-") && (i = -1);
             for (var s = !1, o = 0; !this.isEOF();) {
                 var r = this.char();
                 if (r >= 48 && r <= 57)
                     s = !0, o = o * 10 + (r - 48), this.bump();
                 else
                     break;
             }
-            var a = F(l, this.clonePosition());
+            var a = q(l, this.clonePosition());
             return s ? (o *= i, U0(o) ? {
                 val: o,
                 err: null
             } : this.error(n, a)) : this.error(e, a);
         }, t.prototype.offset = function() {
             return this.position.offset;
         }, t.prototype.isEOF = function() {
@@ -8262,15 +8262,15 @@
 function X0(t, e) {
     e === void 0 && (e = {}), e = G({
         shouldParseSkeletons: !0,
         requiresOtherClause: !0
     }, e);
     var n = new j0(t, e).parse();
     if (n.err) {
-        var i = SyntaxError(U[n.err.kind]);
+        var i = SyntaxError(F[n.err.kind]);
         throw i.location = n.err.location, i.originalMessage = n.err.message, i;
     }
     return e != null && e.captureLocation || Ql(n.val), n.val;
 }
 
 function pl(t, e) {
     var n = e && e.cache ? e.cache : K0,
@@ -8333,177 +8333,177 @@
             return new ms();
         }
     },
     wl = {
         variadic: Y0,
         monadic: J0
     },
-    an;
+    fn;
 (function(t) {
     t.MISSING_VALUE = "MISSING_VALUE", t.INVALID_VALUE = "INVALID_VALUE", t.MISSING_INTL_API = "MISSING_INTL_API";
-})(an || (an = {}));
-var Fi = (
+})(fn || (fn = {}));
+var ji = (
         /** @class */
         function(t) {
-            Ui(e, t);
+            zi(e, t);
 
             function e(n, i, l) {
                 var s = t.call(this, n) || this;
                 return s.code = i, s.originalMessage = l, s;
             }
             return e.prototype.toString = function() {
                 return "[formatjs Error: ".concat(this.code, "] ").concat(this.message);
             }, e;
         }(Error)
     ),
     Bo = (
         /** @class */
         function(t) {
-            Ui(e, t);
+            zi(e, t);
 
             function e(n, i, l, s) {
-                return t.call(this, 'Invalid values for "'.concat(n, '": "').concat(i, '". Options are "').concat(Object.keys(l).join('", "'), '"'), an.INVALID_VALUE, s) || this;
+                return t.call(this, 'Invalid values for "'.concat(n, '": "').concat(i, '". Options are "').concat(Object.keys(l).join('", "'), '"'), fn.INVALID_VALUE, s) || this;
             }
             return e;
-        }(Fi)
+        }(ji)
     ),
     $0 = (
         /** @class */
         function(t) {
-            Ui(e, t);
+            zi(e, t);
 
             function e(n, i, l) {
-                return t.call(this, 'Value for "'.concat(n, '" must be of type ').concat(i), an.INVALID_VALUE, l) || this;
+                return t.call(this, 'Value for "'.concat(n, '" must be of type ').concat(i), fn.INVALID_VALUE, l) || this;
             }
             return e;
-        }(Fi)
+        }(ji)
     ),
     ed = (
         /** @class */
         function(t) {
-            Ui(e, t);
+            zi(e, t);
 
             function e(n, i) {
-                return t.call(this, 'The intl string context variable "'.concat(n, '" was not provided to the string "').concat(i, '"'), an.MISSING_VALUE, i) || this;
+                return t.call(this, 'The intl string context variable "'.concat(n, '" was not provided to the string "').concat(i, '"'), fn.MISSING_VALUE, i) || this;
             }
             return e;
-        }(Fi)
+        }(ji)
     ),
-    Ee;
+    ye;
 (function(t) {
     t[t.literal = 0] = "literal", t[t.object = 1] = "object";
-})(Ee || (Ee = {}));
+})(ye || (ye = {}));
 
 function td(t) {
     return t.length < 2 ? t : t.reduce(function(e, n) {
         var i = e[e.length - 1];
-        return !i || i.type !== Ee.literal || n.type !== Ee.literal ? e.push(n) : i.value += n.value, e;
+        return !i || i.type !== ye.literal || n.type !== ye.literal ? e.push(n) : i.value += n.value, e;
     }, []);
 }
 
 function nd(t) {
     return typeof t == "function";
 }
 
-function mi(t, e, n, i, l, s, o) {
+function pi(t, e, n, i, l, s, o) {
     if (t.length === 1 && vo(t[0]))
         return [{
-            type: Ee.literal,
+            type: ye.literal,
             value: t[0].value
         }];
     for (var r = [], a = 0, u = t; a < u.length; a++) {
         var f = u[a];
         if (vo(f)) {
             r.push({
-                type: Ee.literal,
+                type: ye.literal,
                 value: f.value
             });
             continue;
         }
         if (p0(f)) {
             typeof s == "number" && r.push({
-                type: Ee.literal,
+                type: ye.literal,
                 value: n.getNumberFormat(e).format(s)
             });
             continue;
         }
         var _ = f.value;
         if (!(l && _ in l))
             throw new ed(_, o);
         var h = l[_];
         if (b0(f)) {
             (!h || typeof h == "string" || typeof h == "number") && (h = typeof h == "string" || typeof h == "number" ? String(h) : ""), r.push({
-                type: typeof h == "string" ? Ee.literal : Ee.object,
+                type: typeof h == "string" ? ye.literal : ye.object,
                 value: h
             });
             continue;
         }
         if (Kr(f)) {
             var c = typeof f.style == "string" ? i.date[f.style] : Xl(f.style) ? f.style.parsedOptions : void 0;
             r.push({
-                type: Ee.literal,
+                type: ye.literal,
                 value: n.getDateTimeFormat(e, c).format(h)
             });
             continue;
         }
         if ($r(f)) {
             var c = typeof f.style == "string" ? i.time[f.style] : Xl(f.style) ? f.style.parsedOptions : i.time.medium;
             r.push({
-                type: Ee.literal,
+                type: ye.literal,
                 value: n.getDateTimeFormat(e, c).format(h)
             });
             continue;
         }
         if (Qr(f)) {
             var c = typeof f.style == "string" ? i.number[f.style] : ia(f.style) ? f.style.parsedOptions : void 0;
             c && c.scale && (h = h * (c.scale || 1)), r.push({
-                type: Ee.literal,
+                type: ye.literal,
                 value: n.getNumberFormat(e, c).format(h)
             });
             continue;
         }
         if (na(f)) {
             var d = f.children,
-                m = f.value,
-                b = l[m];
-            if (!nd(b))
-                throw new $0(m, "function", o);
-            var p = mi(d, e, n, i, l, s),
-                y = b(p.map(function(P) {
+                b = f.value,
+                p = l[b];
+            if (!nd(p))
+                throw new $0(b, "function", o);
+            var g = pi(d, e, n, i, l, s),
+                y = p(g.map(function(P) {
                     return P.value;
                 }));
             Array.isArray(y) || (y = [y]), r.push.apply(r, y.map(function(P) {
                 return {
-                    type: typeof P == "string" ? Ee.literal : Ee.object,
+                    type: typeof P == "string" ? ye.literal : ye.object,
                     value: P
                 };
             }));
         }
         if (ea(f)) {
             var w = f.options[h] || f.options.other;
             if (!w)
                 throw new Bo(f.value, h, Object.keys(f.options), o);
-            r.push.apply(r, mi(w.value, e, n, i, l));
+            r.push.apply(r, pi(w.value, e, n, i, l));
             continue;
         }
         if (ta(f)) {
             var w = f.options["=".concat(h)];
             if (!w) {
                 if (!Intl.PluralRules)
-                    throw new Fi(`Intl.PluralRules is not available in this environment.
+                    throw new ji(`Intl.PluralRules is not available in this environment.
 Try polyfilling it using "@formatjs/intl-pluralrules"
-`, an.MISSING_INTL_API, o);
+`, fn.MISSING_INTL_API, o);
                 var C = n.getPluralRules(e, {
                     type: f.pluralType
                 }).select(h - (f.offset || 0));
                 w = f.options[C] || f.options.other;
             }
             if (!w)
                 throw new Bo(f.value, h, Object.keys(f.options), o);
-            r.push.apply(r, mi(w.value, e, n, i, l, h - (f.offset || 0)));
+            r.push.apply(r, pi(w.value, e, n, i, l, h - (f.offset || 0)));
             continue;
         }
     }
     return td(r);
 }
 
 function id(t, e) {
@@ -8575,19 +8575,19 @@
                     dateTime: {},
                     pluralRules: {}
                 }, this.format = function(o) {
                     var r = s.formatToParts(o);
                     if (r.length === 1)
                         return r[0].value;
                     var a = r.reduce(function(u, f) {
-                        return !u.length || f.type !== Ee.literal || typeof u[u.length - 1] != "string" ? u.push(f.value) : u[u.length - 1] += f.value, u;
+                        return !u.length || f.type !== ye.literal || typeof u[u.length - 1] != "string" ? u.push(f.value) : u[u.length - 1] += f.value, u;
                     }, []);
                     return a.length <= 1 ? a[0] || "" : a;
                 }, this.formatToParts = function(o) {
-                    return mi(s.ast, s.locales, s.formatters, s.formats, o, void 0, s.message);
+                    return pi(s.ast, s.locales, s.formatters, s.formats, o, void 0, s.message);
                 }, this.resolvedOptions = function() {
                     return {
                         locale: s.resolvedLocale.toString()
                     };
                 }, this.getAst = function() {
                     return s.ast;
                 }, this.locales = n, this.resolvedLocale = t.resolveLocale(n), typeof e == "string") {
@@ -8691,31 +8691,31 @@
                 }
             }
             i = i[n[l]];
         } else
             i = void 0;
     return i;
 }
-const ut = {},
-    ad = (t, e, n) => n && (e in ut || (ut[e] = {}), t in ut[e] || (ut[e][t] = n), n),
+const ft = {},
+    ad = (t, e, n) => n && (e in ft || (ft[e] = {}), t in ft[e] || (ft[e][t] = n), n),
     ha = (t, e) => {
         if (e == null)
             return;
-        if (e in ut && t in ut[e])
-            return ut[e][t];
-        const n = qi(e);
+        if (e in ft && t in ft[e])
+            return ft[e][t];
+        const n = Gi(e);
         for (let i = 0; i < n.length; i++) {
             const l = n[i],
                 s = fd(l, t);
             if (s)
                 return ad(t, e, s);
         }
     };
 let gs;
-const qn = Fn({});
+const xn = Gn({});
 
 function ud(t) {
     return gs[t] || null;
 }
 
 function da(t) {
     return t in gs;
@@ -8727,76 +8727,76 @@
     const n = ud(t);
     return rd(n, e);
 }
 
 function cd(t) {
     if (t == null)
         return;
-    const e = qi(t);
+    const e = Gi(t);
     for (let n = 0; n < e.length; n++) {
         const i = e[n];
         if (da(i))
             return i;
     }
 }
 
 function _d(t, ...e) {
-    delete ut[t], qn.update((n) => (n[t] = g0.all([n[t] || {}, ...e]), n));
+    delete ft[t], xn.update((n) => (n[t] = g0.all([n[t] || {}, ...e]), n));
 }
-_n(
-    [qn],
+dn(
+    [xn],
     ([t]) => Object.keys(t)
 );
-qn.subscribe((t) => gs = t);
-const gi = {};
+xn.subscribe((t) => gs = t);
+const wi = {};
 
 function hd(t, e) {
-    gi[t].delete(e), gi[t].size === 0 && delete gi[t];
+    wi[t].delete(e), wi[t].size === 0 && delete wi[t];
 }
 
 function ma(t) {
-    return gi[t];
+    return wi[t];
 }
 
 function dd(t) {
-    return qi(t).map((e) => {
+    return Gi(t).map((e) => {
         const n = ma(e);
         return [e, n ? [...n] : []];
     }).filter(([, e]) => e.length > 0);
 }
 
 function Kl(t) {
-    return t == null ? !1 : qi(t).some(
+    return t == null ? !1 : Gi(t).some(
         (e) => {
             var n;
             return (n = ma(e)) == null ? void 0 : n.size;
         }
     );
 }
 
 function md(t, e) {
     return Promise.all(
         e.map((i) => (hd(t, i), i().then((l) => l.default || l)))
     ).then((i) => _d(t, ...i));
 }
-const bn = {};
+const yn = {};
 
 function ga(t) {
     if (!Kl(t))
-        return t in bn ? bn[t] : Promise.resolve();
+        return t in yn ? yn[t] : Promise.resolve();
     const e = dd(t);
-    return bn[t] = Promise.all(
+    return yn[t] = Promise.all(
         e.map(
             ([n, i]) => md(n, i)
         )
     ).then(() => {
         if (Kl(t))
             return ga(t);
-        delete bn[t];
-    }), bn[t];
+        delete yn[t];
+    }), yn[t];
 }
 const gd = {
         number: {
             scientific: {
                 notation: "scientific"
             },
             engineering: {
@@ -8864,18 +8864,18 @@
         formats: gd,
         warnOnMissingMessages: !0,
         handleMissingMessage: void 0,
         ignoreTag: !0
     },
     pd = bd;
 
-function un() {
+function cn() {
     return pd;
 }
-const yl = Fn(!1);
+const yl = Gn(!1);
 var wd = Object.defineProperty,
     vd = Object.defineProperties,
     yd = Object.getOwnPropertyDescriptors,
     To = Object.getOwnPropertySymbols,
     Ed = Object.prototype.hasOwnProperty,
     kd = Object.prototype.propertyIsEnumerable,
     Ho = (t, e, n) => e in t ? wd(t, e, {
@@ -8890,192 +8890,192 @@
         if (To)
             for (var n of To(e))
                 kd.call(e, n) && Ho(t, n, e[n]);
         return t;
     },
     Cd = (t, e) => vd(t, yd(e));
 let $l;
-const ki = Fn(null);
+const Ai = Gn(null);
 
 function Po(t) {
     return t.split("-").map((e, n, i) => i.slice(0, n + 1).join("-")).reverse();
 }
 
-function qi(t, e = un().fallbackLocale) {
+function Gi(t, e = cn().fallbackLocale) {
     const n = Po(t);
     return e ? [... /* @__PURE__ */ new Set([...n, ...Po(e)])] : n;
 }
 
-function Dt() {
+function Rt() {
     return $l ?? void 0;
 }
-ki.subscribe((t) => {
+Ai.subscribe((t) => {
     $l = t ?? void 0, typeof window < "u" && t != null && document.documentElement.setAttribute("lang", t);
 });
 const Ad = (t) => {
         if (t && cd(t) && Kl(t)) {
             const {
                 loadingDelay: e
-            } = un();
+            } = cn();
             let n;
-            return typeof window < "u" && Dt() != null && e ? n = window.setTimeout(
+            return typeof window < "u" && Rt() != null && e ? n = window.setTimeout(
                 () => yl.set(!0),
                 e
             ) : yl.set(!0), ga(t).then(() => {
-                ki.set(t);
+                Ai.set(t);
             }).finally(() => {
                 clearTimeout(n), yl.set(!1);
             });
         }
-        return ki.set(t);
+        return Ai.set(t);
     },
-    zn = Cd(Sd({}, ki), {
+    Vn = Cd(Sd({}, Ai), {
         set: Ad
     }),
-    zi = (t) => {
+    xi = (t) => {
         const e = /* @__PURE__ */ Object.create(null);
         return (i) => {
             const l = JSON.stringify(i);
             return l in e ? e[l] : e[l] = t(i);
         };
     };
 var Bd = Object.defineProperty,
-    Si = Object.getOwnPropertySymbols,
+    Bi = Object.getOwnPropertySymbols,
     ba = Object.prototype.hasOwnProperty,
     pa = Object.prototype.propertyIsEnumerable,
     No = (t, e, n) => e in t ? Bd(t, e, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
         value: n
     }) : t[e] = n,
     bs = (t, e) => {
         for (var n in e || (e = {}))
             ba.call(e, n) && No(t, n, e[n]);
-        if (Si)
-            for (var n of Si(e))
+        if (Bi)
+            for (var n of Bi(e))
                 pa.call(e, n) && No(t, n, e[n]);
         return t;
     },
-    dn = (t, e) => {
+    gn = (t, e) => {
         var n = {};
         for (var i in t)
             ba.call(t, i) && e.indexOf(i) < 0 && (n[i] = t[i]);
-        if (t != null && Si)
-            for (var i of Si(t))
+        if (t != null && Bi)
+            for (var i of Bi(t))
                 e.indexOf(i) < 0 && pa.call(t, i) && (n[i] = t[i]);
         return n;
     };
-const On = (t, e) => {
+const Fn = (t, e) => {
         const {
             formats: n
-        } = un();
+        } = cn();
         if (t in n && e in n[t])
             return n[t][e];
         throw new Error(`[svelte-i18n] Unknown "${e}" ${t} format.`);
     },
-    Td = zi(
+    Td = xi(
         (t) => {
             var e = t,
                 {
                     locale: n,
                     format: i
                 } = e,
-                l = dn(e, ["locale", "format"]);
+                l = gn(e, ["locale", "format"]);
             if (n == null)
                 throw new Error('[svelte-i18n] A "locale" must be set to format numbers');
-            return i && (l = On("number", i)), new Intl.NumberFormat(n, l);
+            return i && (l = Fn("number", i)), new Intl.NumberFormat(n, l);
         }
     ),
-    Hd = zi(
+    Hd = xi(
         (t) => {
             var e = t,
                 {
                     locale: n,
                     format: i
                 } = e,
-                l = dn(e, ["locale", "format"]);
+                l = gn(e, ["locale", "format"]);
             if (n == null)
                 throw new Error('[svelte-i18n] A "locale" must be set to format dates');
-            return i ? l = On("date", i) : Object.keys(l).length === 0 && (l = On("date", "short")), new Intl.DateTimeFormat(n, l);
+            return i ? l = Fn("date", i) : Object.keys(l).length === 0 && (l = Fn("date", "short")), new Intl.DateTimeFormat(n, l);
         }
     ),
-    Pd = zi(
+    Pd = xi(
         (t) => {
             var e = t,
                 {
                     locale: n,
                     format: i
                 } = e,
-                l = dn(e, ["locale", "format"]);
+                l = gn(e, ["locale", "format"]);
             if (n == null)
                 throw new Error(
                     '[svelte-i18n] A "locale" must be set to format time values'
                 );
-            return i ? l = On("time", i) : Object.keys(l).length === 0 && (l = On("time", "short")), new Intl.DateTimeFormat(n, l);
+            return i ? l = Fn("time", i) : Object.keys(l).length === 0 && (l = Fn("time", "short")), new Intl.DateTimeFormat(n, l);
         }
     ),
     Nd = (t = {}) => {
         var e = t,
             {
-                locale: n = Dt()
+                locale: n = Rt()
             } = e,
-            i = dn(e, [
+            i = gn(e, [
                 "locale"
             ]);
         return Td(bs({
             locale: n
         }, i));
     },
     Ld = (t = {}) => {
         var e = t,
             {
-                locale: n = Dt()
+                locale: n = Rt()
             } = e,
-            i = dn(e, [
+            i = gn(e, [
                 "locale"
             ]);
         return Hd(bs({
             locale: n
         }, i));
     },
     Id = (t = {}) => {
         var e = t,
             {
-                locale: n = Dt()
+                locale: n = Rt()
             } = e,
-            i = dn(e, [
+            i = gn(e, [
                 "locale"
             ]);
         return Pd(bs({
             locale: n
         }, i));
     },
-    Md = zi(
+    Md = xi(
         // eslint-disable-next-line @typescript-eslint/no-non-null-assertion
-        (t, e = Dt()) => new od(t, e, un().formats, {
-            ignoreTag: un().ignoreTag
+        (t, e = Rt()) => new od(t, e, cn().formats, {
+            ignoreTag: cn().ignoreTag
         })
     ),
     Od = (t, e = {}) => {
         var n, i, l, s;
         let o = e;
         typeof t == "object" && (o = t, t = o.id);
         const {
             values: r,
-            locale: a = Dt(),
+            locale: a = Rt(),
             default: u
         } = o;
         if (a == null)
             throw new Error(
                 "[svelte-i18n] Cannot format a message without first setting the initial locale."
             );
         let f = ha(t, a);
         if (!f)
-            f = (s = (l = (i = (n = un()).handleMissingMessage) == null ? void 0 : i.call(n, {
+            f = (s = (l = (i = (n = cn()).handleMissingMessage) == null ? void 0 : i.call(n, {
                 locale: a,
                 id: t,
                 defaultValue: u
             })) != null ? l : u) != null ? s : t;
         else if (typeof f != "string")
             return console.warn(
                 `[svelte-i18n] Message with id "${t}" must be of type "string", found: "${typeof f}". Gettin its value through the "$format" method is deprecated; use the "json" method instead.`
@@ -9092,73 +9092,73 @@
             );
         }
         return _;
     },
     Dd = (t, e) => Id(e).format(t),
     Rd = (t, e) => Ld(e).format(t),
     Ud = (t, e) => Nd(e).format(t),
-    Fd = (t, e = Dt()) => ha(t, e);
-_n([zn, qn], () => Od);
-_n([zn], () => Dd);
-_n([zn], () => Rd);
-_n([zn], () => Ud);
-_n([zn, qn], () => Fd);
+    Fd = (t, e = Rt()) => ha(t, e);
+dn([Vn, xn], () => Od);
+dn([Vn], () => Dd);
+dn([Vn], () => Rd);
+dn([Vn], () => Ud);
+dn([Vn, xn], () => Fd);
 const {
     SvelteComponent: qd,
     append: Te,
-    attr: Et,
+    attr: kt,
     detach: wa,
-    element: kt,
+    element: St,
     init: zd,
     insert: va,
     noop: Lo,
     safe_not_equal: jd,
-    set_data: Ci,
+    set_data: Ti,
     set_style: El,
     space: es,
-    text: $t,
+    text: tn,
     toggle_class: Io
 } = window.__gradio__svelte__internal, {
     onMount: Gd,
     createEventDispatcher: xd,
     getContext: Vd
 } = window.__gradio__svelte__internal;
 
 function Mo(t) {
-    let e, n, i, l, s = Sn(
+    let e, n, i, l, s = Tn(
             /*file_to_display*/
             t[2]
         ) + "",
         o, r, a, u, f = (
             /*file_to_display*/
             t[2].orig_name + ""
         ),
         _;
     return {
         c() {
-            e = kt("div"), n = kt("span"), i = kt("div"), l = kt("progress"), o = $t(s), a = es(), u = kt("span"), _ = $t(f), El(l, "visibility", "hidden"), El(l, "height", "0"), El(l, "width", "0"), l.value = r = Sn(
+            e = St("div"), n = St("span"), i = St("div"), l = St("progress"), o = tn(s), a = es(), u = St("span"), _ = tn(f), El(l, "visibility", "hidden"), El(l, "height", "0"), El(l, "width", "0"), l.value = r = Tn(
                 /*file_to_display*/
                 t[2]
-            ), Et(l, "max", "100"), Et(l, "class", "svelte-cr2edf"), Et(i, "class", "progress-bar svelte-cr2edf"), Et(u, "class", "file-name svelte-cr2edf"), Et(e, "class", "file svelte-cr2edf");
+            ), kt(l, "max", "100"), kt(l, "class", "svelte-cr2edf"), kt(i, "class", "progress-bar svelte-cr2edf"), kt(u, "class", "file-name svelte-cr2edf"), kt(e, "class", "file svelte-cr2edf");
         },
         m(h, c) {
             va(h, e, c), Te(e, n), Te(n, i), Te(i, l), Te(l, o), Te(e, a), Te(e, u), Te(u, _);
         },
         p(h, c) {
             c & /*file_to_display*/
-                4 && s !== (s = Sn(
+                4 && s !== (s = Tn(
                     /*file_to_display*/
                     h[2]
-                ) + "") && Ci(o, s), c & /*file_to_display*/
-                4 && r !== (r = Sn(
+                ) + "") && Ti(o, s), c & /*file_to_display*/
+                4 && r !== (r = Tn(
                     /*file_to_display*/
                     h[2]
                 )) && (l.value = r), c & /*file_to_display*/
                 4 && f !== (f = /*file_to_display*/
-                    h[2].orig_name + "") && Ci(_, f);
+                    h[2].orig_name + "") && Ti(_, f);
         },
         d(h) {
             h && wa(e);
         }
     };
 }
 
@@ -9173,30 +9173,30 @@
         ),
         a, u, f, _ = (
             /*file_to_display*/
             t[2] && Mo(t)
         );
     return {
         c() {
-            e = kt("div"), n = kt("span"), i = $t("Uploading "), s = $t(l), o = es(), a = $t(r), u = $t("..."), f = es(), _ && _.c(), Et(n, "class", "uploading svelte-cr2edf"), Et(e, "class", "wrap svelte-cr2edf"), Io(
+            e = St("div"), n = St("span"), i = tn("Uploading "), s = tn(l), o = es(), a = tn(r), u = tn("..."), f = es(), _ && _.c(), kt(n, "class", "uploading svelte-cr2edf"), kt(e, "class", "wrap svelte-cr2edf"), Io(
                 e,
                 "progress",
                 /*progress*/
                 t[1]
             );
         },
         m(h, c) {
             va(h, e, c), Te(e, n), Te(n, i), Te(n, s), Te(n, o), Te(n, a), Te(n, u), Te(e, f), _ && _.m(e, null);
         },
         p(h, [c]) {
             c & /*files_with_progress*/
                 1 && l !== (l = /*files_with_progress*/
-                    h[0].length + "") && Ci(s, l), c & /*files_with_progress*/
+                    h[0].length + "") && Ti(s, l), c & /*files_with_progress*/
                 1 && r !== (r = /*files_with_progress*/
-                    h[0].length > 1 ? "files" : "file") && Ci(a, r), /*file_to_display*/
+                    h[0].length > 1 ? "files" : "file") && Ti(a, r), /*file_to_display*/
                 h[2] ? _ ? _.p(h, c) : (_ = Mo(h), _.c(), _.m(e, null)) : _ && (_.d(1), _ = null), c & /*progress*/
                 2 && Io(
                     e,
                     "progress",
                     /*progress*/
                     h[1]
                 );
@@ -9205,22 +9205,22 @@
         o: Lo,
         d(h) {
             h && wa(e), _ && _.d();
         }
     };
 }
 
-function Sn(t) {
+function Tn(t) {
     return t.progress * 100 / (t.size || 0) || 0;
 }
 
 function Wd(t) {
     let e = 0;
     return t.forEach((n) => {
-        e += Sn(n);
+        e += Tn(n);
     }), document.documentElement.style.setProperty("--upload-progress-width", (e / t.length).toFixed(2) + "%"), e / t.length;
 }
 
 function Zd(t, e, n) {
     let {
         upload_id: i
     } = e, {
@@ -9229,22 +9229,22 @@
         files: s
     } = e, o, r = !1, a, u, f = s.map((d) => ({
         ...d,
         progress: 0
     }));
     const _ = xd();
 
-    function h(d, m) {
-        n(0, f = f.map((b) => (b.orig_name === d && (b.progress += m), b)));
+    function h(d, b) {
+        n(0, f = f.map((p) => (p.orig_name === d && (p.progress += b), p)));
     }
     const c = Vd("EventSource_factory");
     return Gd(() => {
         o = c(new URL(`${l}/upload_progress?upload_id=${i}`)), o.onmessage = async function(d) {
-            const m = JSON.parse(d.data);
-            r || n(1, r = !0), m.msg === "done" ? (o.close(), _("done")) : (n(6, a = m), h(m.orig_name, m.chunk_size));
+            const b = JSON.parse(d.data);
+            r || n(1, r = !0), b.msg === "done" ? (o.close(), _("done")) : (n(6, a = b), h(b.orig_name, b.chunk_size));
         };
     }), t.$$set = (d) => {
         "upload_id" in d && n(3, i = d.upload_id), "root" in d && n(4, l = d.root), "files" in d && n(5, s = d.files);
     }, t.$$.update = () => {
         t.$$.dirty & /*files_with_progress*/
             1 && Wd(f), t.$$.dirty & /*current_file_upload, files_with_progress*/
             65 && n(2, u = a || f[0]);
@@ -9266,40 +9266,40 @@
             files: 5
         });
     }
 }
 const {
     SvelteComponent: Jd,
     append: Oo,
-    attr: we,
+    attr: pe,
     binding_callbacks: Qd,
-    bubble: bt,
+    bubble: pt,
     check_outros: ya,
     create_component: Kd,
     create_slot: Ea,
     destroy_component: $d,
-    detach: ji,
+    detach: Vi,
     element: ts,
     empty: ka,
     get_all_dirty_from_scope: Sa,
     get_slot_changes: Ca,
     group_outros: Aa,
     init: em,
-    insert: Gi,
+    insert: Xi,
     listen: Ne,
     mount_component: tm,
-    prevent_default: pt,
+    prevent_default: wt,
     run_all: nm,
     safe_not_equal: im,
     set_style: Ba,
     space: lm,
-    stop_propagation: wt,
-    toggle_class: ve,
-    transition_in: ft,
-    transition_out: Lt,
+    stop_propagation: vt,
+    toggle_class: we,
+    transition_in: ct,
+    transition_out: It,
     update_slot_base: Ta
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: sm,
     tick: om,
     getContext: rm
 } = window.__gradio__svelte__internal;
 
@@ -9314,78 +9314,78 @@
             t,
             /*$$scope*/
             t[21],
             null
         );
     return {
         c() {
-            e = ts("button"), h && h.c(), n = lm(), i = ts("input"), we(i, "aria-label", "file upload"), we(i, "data-testid", "file-upload"), we(i, "type", "file"), we(
+            e = ts("button"), h && h.c(), n = lm(), i = ts("input"), pe(i, "aria-label", "file upload"), pe(i, "data-testid", "file-upload"), pe(i, "type", "file"), pe(
                     i,
                     "accept",
                     /*accept_file_types*/
                     t[12]
                 ), i.multiple = l = /*file_count*/
-                t[5] === "multiple" || void 0, we(i, "webkitdirectory", s = /*file_count*/
-                    t[5] === "directory" || void 0), we(i, "mozdirectory", o = /*file_count*/
-                    t[5] === "directory" || void 0), we(i, "class", "svelte-1aq8tno"), we(e, "tabindex", r = /*hidden*/
-                    t[7] ? -1 : 0), we(e, "class", "svelte-1aq8tno"), ve(
+                t[5] === "multiple" || void 0, pe(i, "webkitdirectory", s = /*file_count*/
+                    t[5] === "directory" || void 0), pe(i, "mozdirectory", o = /*file_count*/
+                    t[5] === "directory" || void 0), pe(i, "class", "svelte-1aq8tno"), pe(e, "tabindex", r = /*hidden*/
+                    t[7] ? -1 : 0), pe(e, "class", "svelte-1aq8tno"), we(
                     e,
                     "hidden",
                     /*hidden*/
                     t[7]
-                ), ve(
+                ), we(
                     e,
                     "center",
                     /*center*/
                     t[3]
-                ), ve(
+                ), we(
                     e,
                     "boundedheight",
                     /*boundedheight*/
                     t[2]
-                ), ve(
+                ), we(
                     e,
                     "flex",
                     /*flex*/
                     t[4]
                 ), Ba(e, "height", "100%");
         },
         m(c, d) {
-            Gi(c, e, d), h && h.m(e, null), Oo(e, n), Oo(e, i), t[30](i), a = !0, u || (f = [
+            Xi(c, e, d), h && h.m(e, null), Oo(e, n), Oo(e, i), t[30](i), a = !0, u || (f = [
                 Ne(
                     i,
                     "change",
                     /*load_files_from_upload*/
                     t[15]
                 ),
-                Ne(e, "drag", wt(pt(
+                Ne(e, "drag", vt(wt(
                     /*drag_handler*/
                     t[23]
                 ))),
-                Ne(e, "dragstart", wt(pt(
+                Ne(e, "dragstart", vt(wt(
                     /*dragstart_handler*/
                     t[24]
                 ))),
-                Ne(e, "dragend", wt(pt(
+                Ne(e, "dragend", vt(wt(
                     /*dragend_handler*/
                     t[25]
                 ))),
-                Ne(e, "dragover", wt(pt(
+                Ne(e, "dragover", vt(wt(
                     /*dragover_handler*/
                     t[26]
                 ))),
-                Ne(e, "dragenter", wt(pt(
+                Ne(e, "dragenter", vt(wt(
                     /*dragenter_handler*/
                     t[27]
                 ))),
-                Ne(e, "dragleave", wt(pt(
+                Ne(e, "dragleave", vt(wt(
                     /*dragleave_handler*/
                     t[28]
                 ))),
-                Ne(e, "drop", wt(pt(
+                Ne(e, "drop", vt(wt(
                     /*drop_handler*/
                     t[29]
                 ))),
                 Ne(
                     e,
                     "click",
                     /*open_file_upload*/
@@ -9427,90 +9427,90 @@
                     null
                 ) : Sa(
                     /*$$scope*/
                     c[21]
                 ),
                 null
             ), (!a || d[0] & /*accept_file_types*/
-                4096) && we(
+                4096) && pe(
                 i,
                 "accept",
                 /*accept_file_types*/
                 c[12]
             ), (!a || d[0] & /*file_count*/
                 32 && l !== (l = /*file_count*/
                     c[5] === "multiple" || void 0)) && (i.multiple = l), (!a || d[0] & /*file_count*/
                 32 && s !== (s = /*file_count*/
-                    c[5] === "directory" || void 0)) && we(i, "webkitdirectory", s), (!a || d[0] & /*file_count*/
+                    c[5] === "directory" || void 0)) && pe(i, "webkitdirectory", s), (!a || d[0] & /*file_count*/
                 32 && o !== (o = /*file_count*/
-                    c[5] === "directory" || void 0)) && we(i, "mozdirectory", o), (!a || d[0] & /*hidden*/
+                    c[5] === "directory" || void 0)) && pe(i, "mozdirectory", o), (!a || d[0] & /*hidden*/
                 128 && r !== (r = /*hidden*/
-                    c[7] ? -1 : 0)) && we(e, "tabindex", r), (!a || d[0] & /*hidden*/
-                128) && ve(
+                    c[7] ? -1 : 0)) && pe(e, "tabindex", r), (!a || d[0] & /*hidden*/
+                128) && we(
                 e,
                 "hidden",
                 /*hidden*/
                 c[7]
             ), (!a || d[0] & /*center*/
-                8) && ve(
+                8) && we(
                 e,
                 "center",
                 /*center*/
                 c[3]
             ), (!a || d[0] & /*boundedheight*/
-                4) && ve(
+                4) && we(
                 e,
                 "boundedheight",
                 /*boundedheight*/
                 c[2]
             ), (!a || d[0] & /*flex*/
-                16) && ve(
+                16) && we(
                 e,
                 "flex",
                 /*flex*/
                 c[4]
             );
         },
         i(c) {
-            a || (ft(h, c), a = !0);
+            a || (ct(h, c), a = !0);
         },
         o(c) {
-            Lt(h, c), a = !1;
+            It(h, c), a = !1;
         },
         d(c) {
-            c && ji(e), h && h.d(c), t[30](null), u = !1, nm(f);
+            c && Vi(e), h && h.d(c), t[30](null), u = !1, nm(f);
         }
     };
 }
 
 function um(t) {
     let e, n, i = ! /*hidden*/
         t[7] && Do(t);
     return {
         c() {
             i && i.c(), e = ka();
         },
         m(l, s) {
-            i && i.m(l, s), Gi(l, e, s), n = !0;
+            i && i.m(l, s), Xi(l, e, s), n = !0;
         },
         p(l, s) {
             /*hidden*/
-            l[7] ? i && (Aa(), Lt(i, 1, 1, () => {
+            l[7] ? i && (Aa(), It(i, 1, 1, () => {
                 i = null;
             }), ya()) : i ? (i.p(l, s), s[0] & /*hidden*/
-                128 && ft(i, 1)) : (i = Do(l), i.c(), ft(i, 1), i.m(e.parentNode, e));
+                128 && ct(i, 1)) : (i = Do(l), i.c(), ct(i, 1), i.m(e.parentNode, e));
         },
         i(l) {
-            n || (ft(i), n = !0);
+            n || (ct(i), n = !0);
         },
         o(l) {
-            Lt(i), n = !1;
+            It(i), n = !1;
         },
         d(l) {
-            l && ji(e), i && i.d(l);
+            l && Vi(e), i && i.d(l);
         }
     };
 }
 
 function fm(t) {
     let e, n, i, l, s;
     const o = (
@@ -9522,39 +9522,39 @@
             t,
             /*$$scope*/
             t[21],
             null
         );
     return {
         c() {
-            e = ts("button"), r && r.c(), we(e, "tabindex", n = /*hidden*/
-                t[7] ? -1 : 0), we(e, "class", "svelte-1aq8tno"), ve(
+            e = ts("button"), r && r.c(), pe(e, "tabindex", n = /*hidden*/
+                t[7] ? -1 : 0), pe(e, "class", "svelte-1aq8tno"), we(
                 e,
                 "hidden",
                 /*hidden*/
                 t[7]
-            ), ve(
+            ), we(
                 e,
                 "center",
                 /*center*/
                 t[3]
-            ), ve(
+            ), we(
                 e,
                 "boundedheight",
                 /*boundedheight*/
                 t[2]
-            ), ve(
+            ), we(
                 e,
                 "flex",
                 /*flex*/
                 t[4]
             ), Ba(e, "height", "100%");
         },
         m(a, u) {
-            Gi(a, e, u), r && r.m(e, null), i = !0, l || (s = Ne(
+            Xi(a, e, u), r && r.m(e, null), i = !0, l || (s = Ne(
                 e,
                 "click",
                 /*paste_clipboard*/
                 t[8]
             ), l = !0);
         },
         p(a, u) {
@@ -9574,48 +9574,48 @@
                 ) : Sa(
                     /*$$scope*/
                     a[21]
                 ),
                 null
             ), (!i || u[0] & /*hidden*/
                 128 && n !== (n = /*hidden*/
-                    a[7] ? -1 : 0)) && we(e, "tabindex", n), (!i || u[0] & /*hidden*/
-                128) && ve(
+                    a[7] ? -1 : 0)) && pe(e, "tabindex", n), (!i || u[0] & /*hidden*/
+                128) && we(
                 e,
                 "hidden",
                 /*hidden*/
                 a[7]
             ), (!i || u[0] & /*center*/
-                8) && ve(
+                8) && we(
                 e,
                 "center",
                 /*center*/
                 a[3]
             ), (!i || u[0] & /*boundedheight*/
-                4) && ve(
+                4) && we(
                 e,
                 "boundedheight",
                 /*boundedheight*/
                 a[2]
             ), (!i || u[0] & /*flex*/
-                16) && ve(
+                16) && we(
                 e,
                 "flex",
                 /*flex*/
                 a[4]
             );
         },
         i(a) {
-            i || (ft(r, a), i = !0);
+            i || (ct(r, a), i = !0);
         },
         o(a) {
-            Lt(r, a), i = !1;
+            It(r, a), i = !1;
         },
         d(a) {
-            a && ji(e), r && r.d(a), l = !1, s();
+            a && Vi(e), r && r.d(a), l = !1, s();
         }
     };
 }
 
 function Do(t) {
     let e, n;
     return e = new Yd({
@@ -9647,18 +9647,18 @@
                     i[6]), l[0] & /*upload_id*/
                 1024 && (s.upload_id = /*upload_id*/
                     i[10]), l[0] & /*file_data*/
                 2048 && (s.files = /*file_data*/
                     i[11]), e.$set(s);
         },
         i(i) {
-            n || (ft(e.$$.fragment, i), n = !0);
+            n || (ct(e.$$.fragment, i), n = !0);
         },
         o(i) {
-            Lt(e.$$.fragment, i), n = !1;
+            It(e.$$.fragment, i), n = !1;
         },
         d(i) {
             $d(e, i);
         }
     };
 }
 
@@ -9677,30 +9677,30 @@
         );
     }
     return e = r(t), n = o[e] = s[e](t), {
         c() {
             n.c(), i = ka();
         },
         m(a, u) {
-            o[e].m(a, u), Gi(a, i, u), l = !0;
+            o[e].m(a, u), Xi(a, i, u), l = !0;
         },
         p(a, u) {
             let f = e;
-            e = r(a), e === f ? o[e].p(a, u) : (Aa(), Lt(o[f], 1, 1, () => {
+            e = r(a), e === f ? o[e].p(a, u) : (Aa(), It(o[f], 1, 1, () => {
                 o[f] = null;
-            }), ya(), n = o[e], n ? n.p(a, u) : (n = o[e] = s[e](a), n.c()), ft(n, 1), n.m(i.parentNode, i));
+            }), ya(), n = o[e], n ? n.p(a, u) : (n = o[e] = s[e](a), n.c()), ct(n, 1), n.m(i.parentNode, i));
         },
         i(a) {
-            l || (ft(n), l = !0);
+            l || (ct(n), l = !0);
         },
         o(a) {
-            Lt(n), l = !1;
+            It(n), l = !1;
         },
         d(a) {
-            a && ji(i), o[e].d(a);
+            a && Vi(i), o[e].d(a);
         }
     };
 }
 
 function Ro(t) {
     let e, n = t[0],
         i = 1;
@@ -9751,52 +9751,52 @@
     } = e, {
         root: h
     } = e, {
         hidden: c = !1
     } = e, {
         format: d = "file"
     } = e, {
-        uploading: m = !1
-    } = e, b, p, y;
+        uploading: b = !1
+    } = e, p, g, y;
     const w = rm("upload_files");
     let C;
     const P = sm();
 
     function E() {
         n(17, o = !o);
     }
 
     function N() {
         navigator.clipboard.read().then(async (k) => {
             for (let I = 0; I < k.length; I++) {
-                const g = k[I].types.find((T) => T.startsWith("image/"));
-                if (g) {
-                    k[I].getType(g).then(async (T) => {
-                        const ae = new File([T], `clipboard.${g.replace("image/", "")}`);
+                const m = k[I].types.find((T) => T.startsWith("image/"));
+                if (m) {
+                    k[I].getType(m).then(async (T) => {
+                        const ae = new File([T], `clipboard.${m.replace("image/", "")}`);
                         await B([ae]);
                     });
                     break;
                 }
             }
         });
     }
 
     function v() {
         _ || (n(13, C.value = "", C), C.click());
     }
     async function A(k) {
-        await om(), n(10, b = Math.random().toString(36).substring(2, 15)), n(1, m = !0);
-        const I = await Zh(k, h, b, w);
-        return P("load", f === "single" ? Ro([I, "optionalAccess", (g) => g[0]]) : I), n(1, m = !1), I || [];
+        await om(), n(10, p = Math.random().toString(36).substring(2, 15)), n(1, b = !0);
+        const I = await Zh(k, h, p, w);
+        return P("load", f === "single" ? Ro([I, "optionalAccess", (m) => m[0]]) : I), n(1, b = !1), I || [];
     }
     async function B(k) {
         if (!k.length)
             return;
-        let I = k.map((g) => new File([g], g.name));
-        return n(11, p = await Yh(I)), await A(p);
+        let I = k.map((m) => new File([m], m.name));
+        return n(11, g = await Yh(I)), await A(g);
     }
     async function L(k) {
         const I = k.target;
         if (I.files)
             if (d != "blob")
                 await B(Array.from(I.files));
             else {
@@ -9804,92 +9804,92 @@
                     P("load", I.files[0]);
                     return;
                 }
                 P("load", I.files);
             }
     }
     async function x(k) {
-        if (n(17, o = !1), !Ro([k, "access", (g) => g.dataTransfer, "optionalAccess", (g) => g.files]))
+        if (n(17, o = !1), !Ro([k, "access", (m) => m.dataTransfer, "optionalAccess", (m) => m.files]))
             return;
-        const I = Array.from(k.dataTransfer.files).filter((g) => {
-            const T = "." + g.name.split(".").pop();
-            return T && _m(s, T, g.type) || (T && Array.isArray(s) ? s.includes(T) : T === s) ? !0 : (P("error", `Invalid file type only ${s} allowed.`), !1);
+        const I = Array.from(k.dataTransfer.files).filter((m) => {
+            const T = "." + m.name.split(".").pop();
+            return T && _m(s, T, m.type) || (T && Array.isArray(s) ? s.includes(T) : T === s) ? !0 : (P("error", `Invalid file type only ${s} allowed.`), !1);
         });
         await B(I);
     }
 
-    function J(k) {
-        bt.call(this, t, k);
+    function Y(k) {
+        pt.call(this, t, k);
     }
 
-    function ce(k) {
-        bt.call(this, t, k);
+    function _e(k) {
+        pt.call(this, t, k);
     }
 
     function te(k) {
-        bt.call(this, t, k);
+        pt.call(this, t, k);
     }
 
-    function ke(k) {
-        bt.call(this, t, k);
+    function Ee(k) {
+        pt.call(this, t, k);
     }
 
-    function ye(k) {
-        bt.call(this, t, k);
+    function ve(k) {
+        pt.call(this, t, k);
     }
 
-    function me(k) {
-        bt.call(this, t, k);
+    function de(k) {
+        pt.call(this, t, k);
     }
 
-    function _e(k) {
-        bt.call(this, t, k);
+    function ce(k) {
+        pt.call(this, t, k);
     }
 
     function S(k) {
         Qd[k ? "unshift" : "push"](() => {
             C = k, n(13, C);
         });
     }
     return t.$$set = (k) => {
-        "filetype" in k && n(0, s = k.filetype), "dragging" in k && n(17, o = k.dragging), "boundedheight" in k && n(2, r = k.boundedheight), "center" in k && n(3, a = k.center), "flex" in k && n(4, u = k.flex), "file_count" in k && n(5, f = k.file_count), "disable_click" in k && n(18, _ = k.disable_click), "root" in k && n(6, h = k.root), "hidden" in k && n(7, c = k.hidden), "format" in k && n(19, d = k.format), "uploading" in k && n(1, m = k.uploading), "$$scope" in k && n(21, l = k.$$scope);
+        "filetype" in k && n(0, s = k.filetype), "dragging" in k && n(17, o = k.dragging), "boundedheight" in k && n(2, r = k.boundedheight), "center" in k && n(3, a = k.center), "flex" in k && n(4, u = k.flex), "file_count" in k && n(5, f = k.file_count), "disable_click" in k && n(18, _ = k.disable_click), "root" in k && n(6, h = k.root), "hidden" in k && n(7, c = k.hidden), "format" in k && n(19, d = k.format), "uploading" in k && n(1, b = k.uploading), "$$scope" in k && n(21, l = k.$$scope);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*filetype*/
             1 && (s == null || typeof s == "string" ? n(12, y = s) : (n(0, s = s.map((k) => k.startsWith(".") ? k : k + "/*")), n(12, y = s.join(", "))));
     }, [
         s,
-        m,
+        b,
         r,
         a,
         u,
         f,
         h,
         c,
         N,
         v,
-        b,
         p,
+        g,
         y,
         C,
         E,
         L,
         x,
         o,
         _,
         d,
         B,
         l,
         i,
-        J,
-        ce,
-        te,
-        ke,
-        ye,
-        me,
+        Y,
         _e,
+        te,
+        Ee,
+        ve,
+        de,
+        ce,
         S
     ];
 }
 class dm extends Jd {
     constructor(e) {
         super(), em(
             this,
@@ -9925,29 +9925,29 @@
     get load_files() {
         return this.$$.ctx[20];
     }
 }
 const {
     SvelteComponent: mm,
     append: Uo,
-    attr: pe,
+    attr: be,
     detach: gm,
     init: bm,
     insert: pm,
     noop: kl,
     safe_not_equal: wm,
-    set_style: st,
+    set_style: ot,
     svg_element: Sl
 } = window.__gradio__svelte__internal;
 
 function vm(t) {
     let e, n, i;
     return {
         c() {
-            e = Sl("svg"), n = Sl("line"), i = Sl("line"), pe(n, "x1", "4"), pe(n, "y1", "12"), pe(n, "x2", "20"), pe(n, "y2", "12"), st(n, "fill", "none"), st(n, "stroke-width", "2px"), pe(i, "x1", "12"), pe(i, "y1", "4"), pe(i, "x2", "12"), pe(i, "y2", "20"), st(i, "fill", "none"), st(i, "stroke-width", "2px"), pe(e, "width", "100%"), pe(e, "height", "100%"), pe(e, "viewBox", "0 0 24 24"), pe(e, "version", "1.1"), pe(e, "xmlns", "http://www.w3.org/2000/svg"), pe(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), pe(e, "xml:space", "preserve"), pe(e, "stroke", "currentColor"), st(e, "fill-rule", "evenodd"), st(e, "clip-rule", "evenodd"), st(e, "stroke-linecap", "round"), st(e, "stroke-linejoin", "round");
+            e = Sl("svg"), n = Sl("line"), i = Sl("line"), be(n, "x1", "4"), be(n, "y1", "12"), be(n, "x2", "20"), be(n, "y2", "12"), ot(n, "fill", "none"), ot(n, "stroke-width", "2px"), be(i, "x1", "12"), be(i, "y1", "4"), be(i, "x2", "12"), be(i, "y2", "20"), ot(i, "fill", "none"), ot(i, "stroke-width", "2px"), be(e, "width", "100%"), be(e, "height", "100%"), be(e, "viewBox", "0 0 24 24"), be(e, "version", "1.1"), be(e, "xmlns", "http://www.w3.org/2000/svg"), be(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), be(e, "xml:space", "preserve"), be(e, "stroke", "currentColor"), ot(e, "fill-rule", "evenodd"), ot(e, "clip-rule", "evenodd"), ot(e, "stroke-linecap", "round"), ot(e, "stroke-linejoin", "round");
         },
         m(l, s) {
             pm(l, e, s), Uo(e, n), Uo(e, i);
         },
         p: kl,
         i: kl,
         o: kl,
@@ -10163,30 +10163,30 @@
 const {
     SvelteComponent: qm,
     append: Na,
     attr: ie,
     bubble: zm,
     check_outros: jm,
     create_slot: La,
-    detach: jn,
-    element: xi,
+    detach: Xn,
+    element: Wi,
     empty: Gm,
     get_all_dirty_from_scope: Ia,
     get_slot_changes: Ma,
     group_outros: xm,
     init: Vm,
-    insert: Gn,
+    insert: Wn,
     listen: Xm,
     safe_not_equal: Wm,
     set_style: Be,
     space: Oa,
-    src_url_equal: Ai,
-    toggle_class: en,
-    transition_in: Bi,
-    transition_out: Ti,
+    src_url_equal: Hi,
+    toggle_class: nn,
+    transition_in: Pi,
+    transition_out: Ni,
     update_slot_base: Da
 } = window.__gradio__svelte__internal;
 
 function Zm(t) {
     let e, n, i, l, s, o, r = (
         /*icon*/
         t[7] && Go(t)
@@ -10200,39 +10200,39 @@
             t,
             /*$$scope*/
             t[11],
             null
         );
     return {
         c() {
-            e = xi("button"), r && r.c(), n = Oa(), u && u.c(), ie(e, "class", i = /*size*/
+            e = Wi("button"), r && r.c(), n = Oa(), u && u.c(), ie(e, "class", i = /*size*/
                     t[4] + " " + /*variant*/
                     t[3] + " " + /*elem_classes*/
                     t[1].join(" ") + " svelte-8huxfn"), ie(
                     e,
                     "id",
                     /*elem_id*/
                     t[0]
                 ), e.disabled = /*disabled*/
-                t[8], en(e, "hidden", ! /*visible*/
+                t[8], nn(e, "hidden", ! /*visible*/
                     t[2]), Be(
                     e,
                     "flex-grow",
                     /*scale*/
                     t[9]
                 ), Be(
                     e,
                     "width",
                     /*scale*/
                     t[9] === 0 ? "fit-content" : null
                 ), Be(e, "min-width", typeof /*min_width*/ t[10] == "number" ? `calc(min(${/*min_width*/
       t[10]}px, 100%))` : null);
         },
         m(f, _) {
-            Gn(f, e, _), r && r.m(e, null), Na(e, n), u && u.m(e, null), l = !0, s || (o = Xm(
+            Wn(f, e, _), r && r.m(e, null), Na(e, n), u && u.m(e, null), l = !0, s || (o = Xm(
                 e,
                 "click",
                 /*click_handler*/
                 t[13]
             ), s = !0);
         },
         p(f, _) {
@@ -10264,15 +10264,15 @@
                     e,
                     "id",
                     /*elem_id*/
                     f[0]
                 ), (!l || _ & /*disabled*/
                     256) && (e.disabled = /*disabled*/
                     f[8]), (!l || _ & /*size, variant, elem_classes, visible*/
-                    30) && en(e, "hidden", ! /*visible*/
+                    30) && nn(e, "hidden", ! /*visible*/
                     f[2]), _ & /*scale*/
                 512 && Be(
                     e,
                     "flex-grow",
                     /*scale*/
                     f[9]
                 ), _ & /*scale*/
@@ -10282,21 +10282,21 @@
                     /*scale*/
                     f[9] === 0 ? "fit-content" : null
                 ), _ & /*min_width*/
                 1024 && Be(e, "min-width", typeof /*min_width*/ f[10] == "number" ? `calc(min(${/*min_width*/
       f[10]}px, 100%))` : null);
         },
         i(f) {
-            l || (Bi(u, f), l = !0);
+            l || (Pi(u, f), l = !0);
         },
         o(f) {
-            Ti(u, f), l = !1;
+            Ni(u, f), l = !1;
         },
         d(f) {
-            f && jn(e), r && r.d(), u && u.d(f), s = !1, o();
+            f && Xn(e), r && r.d(), u && u.d(f), s = !1, o();
         }
     };
 }
 
 function Ym(t) {
     let e, n, i, l, s = (
         /*icon*/
@@ -10311,15 +10311,15 @@
             t,
             /*$$scope*/
             t[11],
             null
         );
     return {
         c() {
-            e = xi("a"), s && s.c(), n = Oa(), r && r.c(), ie(
+            e = Wi("a"), s && s.c(), n = Oa(), r && r.c(), ie(
                 e,
                 "href",
                 /*link*/
                 t[6]
             ), ie(e, "rel", "noopener noreferrer"), ie(
                 e,
                 "aria-disabled",
@@ -10329,16 +10329,16 @@
                 t[4] + " " + /*variant*/
                 t[3] + " " + /*elem_classes*/
                 t[1].join(" ") + " svelte-8huxfn"), ie(
                 e,
                 "id",
                 /*elem_id*/
                 t[0]
-            ), en(e, "hidden", ! /*visible*/
-                t[2]), en(
+            ), nn(e, "hidden", ! /*visible*/
+                t[2]), nn(
                 e,
                 "disabled",
                 /*disabled*/
                 t[8]
             ), Be(
                 e,
                 "flex-grow",
@@ -10354,15 +10354,15 @@
                 "width",
                 /*scale*/
                 t[9] === 0 ? "fit-content" : null
             ), Be(e, "min-width", typeof /*min_width*/ t[10] == "number" ? `calc(min(${/*min_width*/
       t[10]}px, 100%))` : null);
         },
         m(a, u) {
-            Gn(a, e, u), s && s.m(e, null), Na(e, n), r && r.m(e, null), l = !0;
+            Wn(a, e, u), s && s.m(e, null), Na(e, n), r && r.m(e, null), l = !0;
         },
         p(a, u) {
             /*icon*/
             a[7] ? s ? s.p(a, u) : (s = xo(a), s.c(), s.m(e, n)) : s && (s.d(1), s = null), r && r.p && (!l || u & /*$$scope*/
                     2048) && Da(
                     r,
                     o,
@@ -10399,17 +10399,17 @@
                         a[1].join(" ") + " svelte-8huxfn")) && ie(e, "class", i), (!l || u & /*elem_id*/
                     1) && ie(
                     e,
                     "id",
                     /*elem_id*/
                     a[0]
                 ), (!l || u & /*size, variant, elem_classes, visible*/
-                    30) && en(e, "hidden", ! /*visible*/
+                    30) && nn(e, "hidden", ! /*visible*/
                     a[2]), (!l || u & /*size, variant, elem_classes, disabled*/
-                    282) && en(
+                    282) && nn(
                     e,
                     "disabled",
                     /*disabled*/
                     a[8]
                 ), u & /*scale*/
                 512 && Be(
                     e,
@@ -10429,69 +10429,69 @@
                     /*scale*/
                     a[9] === 0 ? "fit-content" : null
                 ), u & /*min_width*/
                 1024 && Be(e, "min-width", typeof /*min_width*/ a[10] == "number" ? `calc(min(${/*min_width*/
       a[10]}px, 100%))` : null);
         },
         i(a) {
-            l || (Bi(r, a), l = !0);
+            l || (Pi(r, a), l = !0);
         },
         o(a) {
-            Ti(r, a), l = !1;
+            Ni(r, a), l = !1;
         },
         d(a) {
-            a && jn(e), s && s.d(), r && r.d(a);
+            a && Xn(e), s && s.d(), r && r.d(a);
         }
     };
 }
 
 function Go(t) {
     let e, n, i;
     return {
         c() {
-            e = xi("img"), ie(e, "class", "button-icon svelte-8huxfn"), Ai(e.src, n = /*icon*/
+            e = Wi("img"), ie(e, "class", "button-icon svelte-8huxfn"), Hi(e.src, n = /*icon*/
                 t[7].url) || ie(e, "src", n), ie(e, "alt", i = `${/*value*/
       t[5]} icon`);
         },
         m(l, s) {
-            Gn(l, e, s);
+            Wn(l, e, s);
         },
         p(l, s) {
             s & /*icon*/
-                128 && !Ai(e.src, n = /*icon*/
+                128 && !Hi(e.src, n = /*icon*/
                     l[7].url) && ie(e, "src", n), s & /*value*/
                 32 && i !== (i = `${/*value*/
       l[5]} icon`) && ie(e, "alt", i);
         },
         d(l) {
-            l && jn(e);
+            l && Xn(e);
         }
     };
 }
 
 function xo(t) {
     let e, n, i;
     return {
         c() {
-            e = xi("img"), ie(e, "class", "button-icon svelte-8huxfn"), Ai(e.src, n = /*icon*/
+            e = Wi("img"), ie(e, "class", "button-icon svelte-8huxfn"), Hi(e.src, n = /*icon*/
                 t[7].url) || ie(e, "src", n), ie(e, "alt", i = `${/*value*/
       t[5]} icon`);
         },
         m(l, s) {
-            Gn(l, e, s);
+            Wn(l, e, s);
         },
         p(l, s) {
             s & /*icon*/
-                128 && !Ai(e.src, n = /*icon*/
+                128 && !Hi(e.src, n = /*icon*/
                     l[7].url) && ie(e, "src", n), s & /*value*/
                 32 && i !== (i = `${/*value*/
       l[5]} icon`) && ie(e, "alt", i);
         },
         d(l) {
-            l && jn(e);
+            l && Xn(e);
         }
     };
 }
 
 function Jm(t) {
     let e, n, i, l;
     const s = [Ym, Zm],
@@ -10505,30 +10505,30 @@
         );
     }
     return e = r(t), n = o[e] = s[e](t), {
         c() {
             n.c(), i = Gm();
         },
         m(a, u) {
-            o[e].m(a, u), Gn(a, i, u), l = !0;
+            o[e].m(a, u), Wn(a, i, u), l = !0;
         },
         p(a, [u]) {
             let f = e;
-            e = r(a), e === f ? o[e].p(a, u) : (xm(), Ti(o[f], 1, 1, () => {
+            e = r(a), e === f ? o[e].p(a, u) : (xm(), Ni(o[f], 1, 1, () => {
                 o[f] = null;
-            }), jm(), n = o[e], n ? n.p(a, u) : (n = o[e] = s[e](a), n.c()), Bi(n, 1), n.m(i.parentNode, i));
+            }), jm(), n = o[e], n ? n.p(a, u) : (n = o[e] = s[e](a), n.c()), Pi(n, 1), n.m(i.parentNode, i));
         },
         i(a) {
-            l || (Bi(n), l = !0);
+            l || (Pi(n), l = !0);
         },
         o(a) {
-            Ti(n), l = !1;
+            Ni(n), l = !1;
         },
         d(a) {
-            a && jn(i), o[e].d(a);
+            a && Xn(i), o[e].d(a);
         }
     };
 }
 
 function Qm(t, e, n) {
     let {
         $$slots: i = {},
@@ -10550,37 +10550,37 @@
     } = e, {
         icon: h = null
     } = e, {
         disabled: c = !1
     } = e, {
         scale: d = null
     } = e, {
-        min_width: m = void 0
+        min_width: b = void 0
     } = e;
 
-    function b(p) {
-        zm.call(this, t, p);
+    function p(g) {
+        zm.call(this, t, g);
     }
-    return t.$$set = (p) => {
-        "elem_id" in p && n(0, s = p.elem_id), "elem_classes" in p && n(1, o = p.elem_classes), "visible" in p && n(2, r = p.visible), "variant" in p && n(3, a = p.variant), "size" in p && n(4, u = p.size), "value" in p && n(5, f = p.value), "link" in p && n(6, _ = p.link), "icon" in p && n(7, h = p.icon), "disabled" in p && n(8, c = p.disabled), "scale" in p && n(9, d = p.scale), "min_width" in p && n(10, m = p.min_width), "$$scope" in p && n(11, l = p.$$scope);
+    return t.$$set = (g) => {
+        "elem_id" in g && n(0, s = g.elem_id), "elem_classes" in g && n(1, o = g.elem_classes), "visible" in g && n(2, r = g.visible), "variant" in g && n(3, a = g.variant), "size" in g && n(4, u = g.size), "value" in g && n(5, f = g.value), "link" in g && n(6, _ = g.link), "icon" in g && n(7, h = g.icon), "disabled" in g && n(8, c = g.disabled), "scale" in g && n(9, d = g.scale), "min_width" in g && n(10, b = g.min_width), "$$scope" in g && n(11, l = g.$$scope);
     }, [
         s,
         o,
         r,
         a,
         u,
         f,
         _,
         h,
         c,
         d,
-        m,
+        b,
         l,
         i,
-        b
+        p
     ];
 }
 class Vo extends qm {
     constructor(e) {
         super(), Vm(this, e, Qm, Jm, Wm, {
             elem_id: 0,
             elem_classes: 1,
@@ -10595,33 +10595,33 @@
             min_width: 10
         });
     }
 }
 const {
     SvelteComponent: Km,
     add_render_callback: Ra,
-    append: ei,
+    append: ii,
     attr: Ie,
     binding_callbacks: Xo,
     check_outros: $m,
     create_bidirectional_transition: Wo,
     destroy_each: e1,
-    detach: Bn,
-    element: Hi,
+    detach: Nn,
+    element: Li,
     empty: t1,
     ensure_array_like: Zo,
     group_outros: n1,
     init: i1,
-    insert: Tn,
+    insert: Ln,
     listen: ns,
     prevent_default: l1,
     run_all: s1,
     safe_not_equal: o1,
     set_data: r1,
-    set_style: jt,
+    set_style: xt,
     space: is,
     text: a1,
     toggle_class: xe,
     transition_in: Bl,
     transition_out: Yo
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: u1
@@ -10638,32 +10638,32 @@
             t[1]
         ),
         r = [];
     for (let a = 0; a < o.length; a += 1)
         r[a] = Ko(Jo(t, o, a));
     return {
         c() {
-            e = Hi("ul");
+            e = Li("ul");
             for (let a = 0; a < r.length; a += 1)
                 r[a].c();
-            Ie(e, "class", "options svelte-yuohum"), Ie(e, "role", "listbox"), jt(
+            Ie(e, "class", "options svelte-yuohum"), Ie(e, "role", "listbox"), xt(
                 e,
                 "bottom",
                 /*bottom*/
                 t[9]
-            ), jt(e, "max-height", `calc(${/*max_height*/
-      t[10]}px - var(--window-padding))`), jt(
+            ), xt(e, "max-height", `calc(${/*max_height*/
+      t[10]}px - var(--window-padding))`), xt(
                 e,
                 "width",
                 /*input_width*/
                 t[8] + "px"
             );
         },
         m(a, u) {
-            Tn(a, e, u);
+            Ln(a, e, u);
             for (let f = 0; f < r.length; f += 1)
                 r[f] && r[f].m(e, null);
             t[20](e), i = !0, l || (s = ns(e, "mousedown", l1(
                 /*mousedown_handler*/
                 t[19]
             )), l = !0);
         },
@@ -10680,23 +10680,23 @@
                     r[f] ? r[f].p(_, u) : (r[f] = Ko(_), r[f].c(), r[f].m(e, null));
                 }
                 for (; f < r.length; f += 1)
                     r[f].d(1);
                 r.length = o.length;
             }
             u & /*bottom*/
-                512 && jt(
+                512 && xt(
                     e,
                     "bottom",
                     /*bottom*/
                     a[9]
                 ), u & /*max_height*/
-                1024 && jt(e, "max-height", `calc(${/*max_height*/
+                1024 && xt(e, "max-height", `calc(${/*max_height*/
       a[10]}px - var(--window-padding))`), u & /*input_width*/
-                256 && jt(
+                256 && xt(
                     e,
                     "width",
                     /*input_width*/
                     a[8] + "px"
                 );
         },
         i(a) {
@@ -10710,15 +10710,15 @@
         o(a) {
             a && (n || (n = Wo(e, xs, {
                 duration: 200,
                 y: 5
             }, !1)), n.run(0)), i = !1;
         },
         d(a) {
-            a && Bn(e), e1(r, a), t[20](null), a && n && n.end(), l = !1, s();
+            a && Nn(e), e1(r, a), t[20](null), a && n && n.end(), l = !1, s();
         }
     };
 }
 
 function Ko(t) {
     let e, n, i, l = (
             /*choices*/
@@ -10726,15 +10726,15 @@
                 /*index*/
                 t[24]
             ][0] + ""
         ),
         s, o, r, a, u;
     return {
         c() {
-            e = Hi("li"), n = Hi("span"), n.textContent = "✓", i = is(), s = a1(l), o = is(), Ie(n, "class", "inner-item svelte-yuohum"), xe(n, "hide", ! /*selected_indices*/
+            e = Li("li"), n = Li("span"), n.textContent = "✓", i = is(), s = a1(l), o = is(), Ie(n, "class", "inner-item svelte-yuohum"), xe(n, "hide", ! /*selected_indices*/
                 t[4].includes(
                     /*index*/
                     t[24]
                 )), Ie(e, "class", "item svelte-yuohum"), Ie(e, "data-index", r = /*index*/
                 t[24]), Ie(e, "aria-label", a = /*choices*/
                 t[0][
                     /*index*/
@@ -10768,15 +10768,15 @@
                 "dark:bg-gray-600",
                 /*index*/
                 t[24] === /*active_index*/
                 t[5]
             );
         },
         m(f, _) {
-            Tn(f, e, _), ei(e, n), ei(e, i), ei(e, s), ei(e, o);
+            Ln(f, e, _), ii(e, n), ii(e, i), ii(e, s), ii(e, o);
         },
         p(f, _) {
             _ & /*selected_indices, filtered_indices*/
                 18 && xe(n, "hide", ! /*selected_indices*/
                     f[4].includes(
                         /*index*/
                         f[24]
@@ -10826,15 +10826,15 @@
                     "dark:bg-gray-600",
                     /*index*/
                     f[24] === /*active_index*/
                     f[5]
                 );
         },
         d(f) {
-            f && Bn(e);
+            f && Nn(e);
         }
     };
 }
 
 function f1(t) {
     let e, n, i, l, s;
     Ra(
@@ -10844,18 +10844,18 @@
     let o = (
         /*show_options*/
         t[2] && ! /*disabled*/
         t[3] && Qo(t)
     );
     return {
         c() {
-            e = Hi("div"), n = is(), o && o.c(), i = t1(), Ie(e, "class", "reference");
+            e = Li("div"), n = is(), o && o.c(), i = t1(), Ie(e, "class", "reference");
         },
         m(r, a) {
-            Tn(r, e, a), t[18](e), Tn(r, n, a), o && o.m(r, a), Tn(r, i, a), l || (s = [
+            Ln(r, e, a), t[18](e), Ln(r, n, a), o && o.m(r, a), Ln(r, i, a), l || (s = [
                 ns(
                     window,
                     "scroll",
                     /*scroll_listener*/
                     t[12]
                 ),
                 ns(
@@ -10877,20 +10877,20 @@
         i(r) {
             Bl(o);
         },
         o(r) {
             Yo(o);
         },
         d(r) {
-            r && (Bn(e), Bn(n), Bn(i)), t[18](null), o && o.d(r), l = !1, s1(s);
+            r && (Nn(e), Nn(n), Nn(i)), t[18](null), o && o.d(r), l = !1, s1(s);
         }
     };
 }
 
-function ti(t) {
+function li(t) {
     let e, n = t[0],
         i = 1;
     for (; i < t.length;) {
         const l = t[i],
             s = t[i + 1];
         if (i += 2, (l === "optionalAccess" || l === "optionalCall") && n == null)
             return;
@@ -10908,37 +10908,37 @@
         show_options: s = !1
     } = e, {
         disabled: o = !1
     } = e, {
         selected_indices: r = []
     } = e, {
         active_index: a = null
-    } = e, u, f, _, h, c, d, m, b, p;
+    } = e, u, f, _, h, c, d, b, p, g;
 
     function y() {
         const {
             top: B,
             bottom: L
         } = c.getBoundingClientRect();
-        n(14, u = B), n(15, f = p - L);
+        n(14, u = B), n(15, f = g - L);
     }
     let w = null;
 
     function C() {
         s && (w !== null && clearTimeout(w), w = setTimeout(
             () => {
                 y(), w = null;
             },
             10
         ));
     }
     const P = u1();
 
     function E() {
-        n(11, p = window.innerHeight);
+        n(11, g = window.innerHeight);
     }
 
     function N(B) {
         Xo[B ? "unshift" : "push"](() => {
             c = B, n(6, c);
         });
     }
@@ -10955,51 +10955,51 @@
         if (t.$$.dirty & /*show_options, refElement, listElement, selected_indices, distance_from_bottom, distance_from_top, input_height*/
             114900) {
             if (s && c) {
                 if (d && r.length > 0) {
                     let L = d.querySelectorAll("li");
                     for (const x of Array.from(L))
                         if (x.getAttribute("data-index") === r[0].toString()) {
-                            ti([
+                            li([
                                 d,
                                 "optionalAccess",
-                                (J) => J.scrollTo,
+                                (Y) => Y.scrollTo,
                                 "optionalCall",
-                                (J) => J(0, x.offsetTop)
+                                (Y) => Y(0, x.offsetTop)
                             ]);
                             break;
                         }
                 }
                 y();
-                const B = ti([
+                const B = li([
                     c,
                     "access",
                     (L) => L.parentElement,
                     "optionalAccess",
                     (L) => L.getBoundingClientRect,
                     "call",
                     (L) => L()
                 ]);
-                n(16, _ = ti([B, "optionalAccess", (L) => L.height]) || 0), n(8, h = ti([B, "optionalAccess", (L) => L.width]) || 0);
+                n(16, _ = li([B, "optionalAccess", (L) => L.height]) || 0), n(8, h = li([B, "optionalAccess", (L) => L.width]) || 0);
             }
-            f > u ? (n(10, b = f), n(9, m = null)) : (n(9, m = `${f + _}px`), n(10, b = u - _));
+            f > u ? (n(10, p = f), n(9, b = null)) : (n(9, b = `${f + _}px`), n(10, p = u - _));
         }
     }, [
         i,
         l,
         s,
         o,
         r,
         a,
         c,
         d,
         h,
-        m,
         b,
         p,
+        g,
         C,
         P,
         u,
         f,
         _,
         E,
         N,
@@ -11043,36 +11043,36 @@
                 l = t.key === "ArrowUp" ? -1 : 1;
             e = n[h1(i + l, n.length)];
         }
     return [!0, e];
 }
 const {
     SvelteComponent: g1,
-    append: vt,
+    append: yt,
     attr: Le,
     binding_callbacks: b1,
     check_outros: p1,
     create_component: ls,
     destroy_component: ss,
     detach: ps,
-    element: Vt,
+    element: Wt,
     group_outros: w1,
     init: v1,
     insert: ws,
-    listen: pn,
+    listen: En,
     mount_component: os,
     run_all: y1,
     safe_not_equal: E1,
     set_data: k1,
     set_input_value: er,
     space: Tl,
     text: S1,
-    toggle_class: Gt,
-    transition_in: Xt,
-    transition_out: Cn
+    toggle_class: Vt,
+    transition_in: Zt,
+    transition_out: Hn
 } = window.__gradio__svelte__internal, {
     onMount: C1
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: A1,
     afterUpdate: B1
 } = window.__gradio__svelte__internal;
 
@@ -11102,24 +11102,24 @@
     };
 }
 
 function tr(t) {
     let e, n, i;
     return n = new hc({}), {
         c() {
-            e = Vt("div"), ls(n.$$.fragment), Le(e, "class", "icon-wrap svelte-1m1zvyj");
+            e = Wt("div"), ls(n.$$.fragment), Le(e, "class", "icon-wrap svelte-1m1zvyj");
         },
         m(l, s) {
             ws(l, e, s), os(n, e, null), i = !0;
         },
         i(l) {
-            i || (Xt(n.$$.fragment, l), i = !0);
+            i || (Zt(n.$$.fragment, l), i = !0);
         },
         o(l) {
-            Cn(n.$$.fragment, l), i = !1;
+            Hn(n.$$.fragment, l), i = !1;
         },
         d(l) {
             l && ps(e), ss(n);
         }
     };
 }
 
@@ -11139,15 +11139,15 @@
                 default: [T1]
             },
             $$scope: {
                 ctx: t
             }
         }
     });
-    let m = ! /*disabled*/
+    let b = ! /*disabled*/
         t[3] && tr();
     return _ = new _1({
         props: {
             show_options: (
                 /*show_options*/
                 t[12]
             ),
@@ -11177,163 +11177,163 @@
         }
     }), _.$on(
         "change",
         /*handle_option_selected*/
         t[16]
     ), {
         c() {
-            e = Vt("div"), ls(n.$$.fragment), i = Tl(), l = Vt("div"), s = Vt("div"), o = Vt("div"), r = Vt("input"), u = Tl(), m && m.c(), f = Tl(), ls(_.$$.fragment), Le(r, "role", "listbox"), Le(r, "aria-controls", "dropdown-options"), Le(
+            e = Wt("div"), ls(n.$$.fragment), i = Tl(), l = Wt("div"), s = Wt("div"), o = Wt("div"), r = Wt("input"), u = Tl(), b && b.c(), f = Tl(), ls(_.$$.fragment), Le(r, "role", "listbox"), Le(r, "aria-controls", "dropdown-options"), Le(
                     r,
                     "aria-expanded",
                     /*show_options*/
                     t[12]
                 ), Le(
                     r,
                     "aria-label",
                     /*label*/
                     t[0]
                 ), Le(r, "class", "border-none svelte-1m1zvyj"), r.disabled = /*disabled*/
                 t[3], Le(r, "autocomplete", "off"), r.readOnly = a = ! /*filterable*/
-                t[7], Gt(r, "subdued", ! /*choices_names*/
+                t[7], Vt(r, "subdued", ! /*choices_names*/
                     t[13].includes(
                         /*input_text*/
                         t[9]
                     ) && ! /*allow_custom_value*/
-                    t[6]), Le(o, "class", "secondary-wrap svelte-1m1zvyj"), Le(s, "class", "wrap-inner svelte-1m1zvyj"), Gt(
+                    t[6]), Le(o, "class", "secondary-wrap svelte-1m1zvyj"), Le(s, "class", "wrap-inner svelte-1m1zvyj"), Vt(
                     s,
                     "show_options",
                     /*show_options*/
                     t[12]
-                ), Le(l, "class", "wrap svelte-1m1zvyj"), Le(e, "class", "svelte-1m1zvyj"), Gt(
+                ), Le(l, "class", "wrap svelte-1m1zvyj"), Le(e, "class", "svelte-1m1zvyj"), Vt(
                     e,
                     "container",
                     /*container*/
                     t[5]
                 );
         },
-        m(b, p) {
-            ws(b, e, p), os(n, e, null), vt(e, i), vt(e, l), vt(l, s), vt(s, o), vt(o, r), er(
+        m(p, g) {
+            ws(p, e, g), os(n, e, null), yt(e, i), yt(e, l), yt(l, s), yt(s, o), yt(o, r), er(
                 r,
                 /*input_text*/
                 t[9]
-            ), t[29](r), vt(o, u), m && m.m(o, null), vt(l, f), os(_, l, null), h = !0, c || (d = [
-                pn(
+            ), t[29](r), yt(o, u), b && b.m(o, null), yt(l, f), os(_, l, null), h = !0, c || (d = [
+                En(
                     r,
                     "input",
                     /*input_input_handler*/
                     t[28]
                 ),
-                pn(
+                En(
                     r,
                     "keydown",
                     /*handle_key_down*/
                     t[19]
                 ),
-                pn(
+                En(
                     r,
                     "keyup",
                     /*keyup_handler*/
                     t[30]
                 ),
-                pn(
+                En(
                     r,
                     "blur",
                     /*handle_blur*/
                     t[18]
                 ),
-                pn(
+                En(
                     r,
                     "focus",
                     /*handle_focus*/
                     t[17]
                 )
             ], c = !0);
         },
-        p(b, p) {
+        p(p, g) {
             const y = {};
-            p[0] & /*show_label*/
+            g[0] & /*show_label*/
                 16 && (y.show_label = /*show_label*/
-                    b[4]), p[0] & /*info*/
+                    p[4]), g[0] & /*info*/
                 2 && (y.info = /*info*/
-                    b[1]), p[0] & /*label*/
-                1 | p[1] & /*$$scope*/
+                    p[1]), g[0] & /*label*/
+                1 | g[1] & /*$$scope*/
                 4 && (y.$$scope = {
-                    dirty: p,
-                    ctx: b
-                }), n.$set(y), (!h || p[0] & /*show_options*/
+                    dirty: g,
+                    ctx: p
+                }), n.$set(y), (!h || g[0] & /*show_options*/
                     4096) && Le(
                     r,
                     "aria-expanded",
                     /*show_options*/
-                    b[12]
-                ), (!h || p[0] & /*label*/
+                    p[12]
+                ), (!h || g[0] & /*label*/
                     1) && Le(
                     r,
                     "aria-label",
                     /*label*/
-                    b[0]
-                ), (!h || p[0] & /*disabled*/
+                    p[0]
+                ), (!h || g[0] & /*disabled*/
                     8) && (r.disabled = /*disabled*/
-                    b[3]), (!h || p[0] & /*filterable*/
+                    p[3]), (!h || g[0] & /*filterable*/
                     128 && a !== (a = ! /*filterable*/
-                        b[7])) && (r.readOnly = a), p[0] & /*input_text*/
+                        p[7])) && (r.readOnly = a), g[0] & /*input_text*/
                 512 && r.value !== /*input_text*/
-                b[9] && er(
+                p[9] && er(
                     r,
                     /*input_text*/
-                    b[9]
-                ), (!h || p[0] & /*choices_names, input_text, allow_custom_value*/
-                    8768) && Gt(r, "subdued", ! /*choices_names*/
-                    b[13].includes(
+                    p[9]
+                ), (!h || g[0] & /*choices_names, input_text, allow_custom_value*/
+                    8768) && Vt(r, "subdued", ! /*choices_names*/
+                    p[13].includes(
                         /*input_text*/
-                        b[9]
+                        p[9]
                     ) && ! /*allow_custom_value*/
-                    b[6]), /*disabled*/
-                b[3] ? m && (w1(), Cn(m, 1, 1, () => {
-                    m = null;
-                }), p1()) : m ? p[0] & /*disabled*/
-                8 && Xt(m, 1) : (m = tr(), m.c(), Xt(m, 1), m.m(o, null)), (!h || p[0] & /*show_options*/
-                    4096) && Gt(
+                    p[6]), /*disabled*/
+                p[3] ? b && (w1(), Hn(b, 1, 1, () => {
+                    b = null;
+                }), p1()) : b ? g[0] & /*disabled*/
+                8 && Zt(b, 1) : (b = tr(), b.c(), Zt(b, 1), b.m(o, null)), (!h || g[0] & /*show_options*/
+                    4096) && Vt(
                     s,
                     "show_options",
                     /*show_options*/
-                    b[12]
+                    p[12]
                 );
             const w = {};
-            p[0] & /*show_options*/
+            g[0] & /*show_options*/
                 4096 && (w.show_options = /*show_options*/
-                    b[12]), p[0] & /*choices*/
+                    p[12]), g[0] & /*choices*/
                 4 && (w.choices = /*choices*/
-                    b[2]), p[0] & /*filtered_indices*/
+                    p[2]), g[0] & /*filtered_indices*/
                 1024 && (w.filtered_indices = /*filtered_indices*/
-                    b[10]), p[0] & /*disabled*/
+                    p[10]), g[0] & /*disabled*/
                 8 && (w.disabled = /*disabled*/
-                    b[3]), p[0] & /*selected_index*/
+                    p[3]), g[0] & /*selected_index*/
                 2048 && (w.selected_indices = /*selected_index*/
-                    b[11] === null ? [] : [
+                    p[11] === null ? [] : [
                         /*selected_index*/
-                        b[11]
-                    ]), p[0] & /*active_index*/
+                        p[11]
+                    ]), g[0] & /*active_index*/
                 16384 && (w.active_index = /*active_index*/
-                    b[14]), _.$set(w), (!h || p[0] & /*container*/
-                    32) && Gt(
+                    p[14]), _.$set(w), (!h || g[0] & /*container*/
+                    32) && Vt(
                     e,
                     "container",
                     /*container*/
-                    b[5]
+                    p[5]
                 );
         },
-        i(b) {
-            h || (Xt(n.$$.fragment, b), Xt(m), Xt(_.$$.fragment, b), h = !0);
+        i(p) {
+            h || (Zt(n.$$.fragment, p), Zt(b), Zt(_.$$.fragment, p), h = !0);
         },
-        o(b) {
-            Cn(n.$$.fragment, b), Cn(m), Cn(_.$$.fragment, b), h = !1;
+        o(p) {
+            Hn(n.$$.fragment, p), Hn(b), Hn(_.$$.fragment, p), h = !1;
         },
-        d(b) {
-            b && ps(e), ss(n), t[29](null), m && m.d(), ss(_), c = !1, y1(d);
+        d(p) {
+            p && ps(e), ss(n), t[29](null), b && b.d(), ss(_), c = !1, y1(d);
         }
     };
 }
 
 function P1(t, e, n) {
     let {
         label: i
@@ -11351,109 +11351,109 @@
         show_label: _
     } = e, {
         container: h = !0
     } = e, {
         allow_custom_value: c = !1
     } = e, {
         filterable: d = !0
-    } = e, m, b = !1, p, y, w = "", C = "", P = !1, E = [], N = null, v = null, A;
+    } = e, b, p = !1, g, y, w = "", C = "", P = !1, E = [], N = null, v = null, A;
     const B = A1();
     s ? (A = a.map((S) => S[1]).indexOf(s), v = A, v === -1 ? (o = s, v = null) : ([w, o] = a[v], C = w), x()) : a.length > 0 && (A = 0, v = 0, [w, s] = a[v], o = s, C = w);
 
     function L() {
-        n(13, p = a.map((S) => S[0])), n(24, y = a.map((S) => S[1]));
+        n(13, g = a.map((S) => S[0])), n(24, y = a.map((S) => S[1]));
     }
 
     function x() {
-        L(), s === void 0 || Array.isArray(s) && s.length === 0 ? (n(9, w = ""), n(11, v = null)) : y.includes(s) ? (n(9, w = p[y.indexOf(s)]), n(11, v = y.indexOf(s))) : c ? (n(9, w = s), n(11, v = null)) : (n(9, w = ""), n(11, v = null)), n(27, A = v);
+        L(), s === void 0 || Array.isArray(s) && s.length === 0 ? (n(9, w = ""), n(11, v = null)) : y.includes(s) ? (n(9, w = g[y.indexOf(s)]), n(11, v = y.indexOf(s))) : c ? (n(9, w = s), n(11, v = null)) : (n(9, w = ""), n(11, v = null)), n(27, A = v);
     }
 
-    function J(S) {
+    function Y(S) {
         if (n(11, v = parseInt(S.detail.target.dataset.index)), isNaN(v)) {
             n(11, v = null);
             return;
         }
-        n(12, b = !1), n(14, N = null), m.blur();
+        n(12, p = !1), n(14, N = null), b.blur();
     }
 
-    function ce(S) {
-        n(10, E = a.map((k, I) => I)), n(12, b = !0), B("focus");
+    function _e(S) {
+        n(10, E = a.map((k, I) => I)), n(12, p = !0), B("focus");
     }
 
     function te() {
-        c ? n(20, s = w) : n(9, w = p[y.indexOf(s)]), n(12, b = !1), n(14, N = null), B("blur");
+        c ? n(20, s = w) : n(9, w = g[y.indexOf(s)]), n(12, p = !1), n(14, N = null), B("blur");
     }
 
-    function ke(S) {
-        n(12, [b, N] = m1(S, N, E), b, (n(14, N), n(2, a), n(23, u), n(6, c), n(9, w), n(10, E), n(8, m), n(25, C), n(11, v), n(27, A), n(26, P), n(24, y))), S.key === "Enter" && (N !== null ? (n(11, v = N), n(12, b = !1), m.blur(), n(14, N = null)) : p.includes(w) ? (n(11, v = p.indexOf(w)), n(12, b = !1), n(14, N = null), m.blur()) : c && (n(20, s = w), n(11, v = null), n(12, b = !1), n(14, N = null), m.blur()), B("enter", s));
+    function Ee(S) {
+        n(12, [p, N] = m1(S, N, E), p, (n(14, N), n(2, a), n(23, u), n(6, c), n(9, w), n(10, E), n(8, b), n(25, C), n(11, v), n(27, A), n(26, P), n(24, y))), S.key === "Enter" && (N !== null ? (n(11, v = N), n(12, p = !1), b.blur(), n(14, N = null)) : g.includes(w) ? (n(11, v = g.indexOf(w)), n(12, p = !1), n(14, N = null), b.blur()) : c && (n(20, s = w), n(11, v = null), n(12, p = !1), n(14, N = null), b.blur()), B("enter", s));
     }
     B1(() => {
         n(21, r = !1), n(26, P = !0);
     }), C1(() => {
-        m.focus();
+        b.focus();
     });
 
-    function ye() {
+    function ve() {
         w = this.value, n(9, w), n(11, v), n(27, A), n(26, P), n(2, a), n(24, y);
     }
 
-    function me(S) {
+    function de(S) {
         b1[S ? "unshift" : "push"](() => {
-            m = S, n(8, m);
+            b = S, n(8, b);
         });
     }
-    const _e = (S) => B("key_up", {
+    const ce = (S) => B("key_up", {
         key: S.key,
         input_value: w
     });
     return t.$$set = (S) => {
         "label" in S && n(0, i = S.label), "info" in S && n(1, l = S.info), "value" in S && n(20, s = S.value), "value_is_output" in S && n(21, r = S.value_is_output), "choices" in S && n(2, a = S.choices), "disabled" in S && n(3, f = S.disabled), "show_label" in S && n(4, _ = S.show_label), "container" in S && n(5, h = S.container), "allow_custom_value" in S && n(6, c = S.allow_custom_value), "filterable" in S && n(7, d = S.filterable);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*selected_index, old_selected_index, initialized, choices, choices_values*/
             218105860 && v !== A && v !== null && P && (n(9, [w, s] = a[v], w, (n(20, s), n(11, v), n(27, A), n(26, P), n(2, a), n(24, y))), n(27, A = v), B("select", {
                 index: v,
                 value: y[v],
                 selected: !0
             })), t.$$.dirty[0] & /*value, old_value, value_is_output*/
             7340032 && s != o && (x(), d1(B, s, r), n(22, o = s)), t.$$.dirty[0] & /*choices*/
             4 && L(), t.$$.dirty[0] & /*choices, old_choices, allow_custom_value, input_text, filtered_indices, filter_input*/
-            8390468 && a !== u && (c || x(), n(23, u = a), n(10, E = $o(a, w)), !c && E.length > 0 && n(14, N = E[0]), m == document.activeElement && n(12, b = !0)), t.$$.dirty[0] & /*input_text, old_input_text, choices, allow_custom_value, filtered_indices*/
+            8390468 && a !== u && (c || x(), n(23, u = a), n(10, E = $o(a, w)), !c && E.length > 0 && n(14, N = E[0]), b == document.activeElement && n(12, p = !0)), t.$$.dirty[0] & /*input_text, old_input_text, choices, allow_custom_value, filtered_indices*/
             33556036 && w !== C && (n(10, E = $o(a, w)), n(25, C = w), !c && E.length > 0 && n(14, N = E[0]));
     }, [
         i,
         l,
         a,
         f,
         _,
         h,
         c,
         d,
-        m,
+        b,
         w,
         E,
         v,
-        b,
         p,
+        g,
         N,
         B,
-        J,
-        ce,
+        Y,
+        _e,
         te,
-        ke,
+        Ee,
         s,
         r,
         o,
         u,
         y,
         C,
         P,
         A,
-        ye,
-        me,
-        _e
+        ve,
+        de,
+        ce
     ];
 }
 class N1 extends g1 {
     constructor(e) {
         super(), v1(
             this,
             e,
@@ -11475,28 +11475,28 @@
             [-1, -1]
         );
     }
 }
 const {
     SvelteComponent: L1,
     append: Je,
-    attr: ni,
-    create_component: ii,
-    destroy_component: li,
+    attr: si,
+    create_component: oi,
+    destroy_component: ri,
     detach: vs,
-    element: yt,
+    element: Et,
     init: I1,
     insert: ys,
-    mount_component: si,
+    mount_component: ai,
     safe_not_equal: M1,
-    set_style: oi,
+    set_style: ui,
     space: Hl,
     text: Ua,
-    transition_in: ri,
-    transition_out: ai
+    transition_in: fi,
+    transition_out: ci
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: O1
 } = window.__gradio__svelte__internal, {
     onMount: D1,
     onDestroy: R1
 } = window.__gradio__svelte__internal;
 
@@ -11527,19 +11527,19 @@
         d(n) {
             n && vs(e);
         }
     };
 }
 
 function q1(t) {
-    let e, n, i, l, s, o, r, a, u, f, _, h, c, d, m;
+    let e, n, i, l, s, o, r, a, u, f, _, h, c, d, b;
     return s = new N1({
         props: {
             value: (
-                /*label*/
+                /*currentLabel*/
                 t[0]
             ),
             label: "Label",
             choices: (
                 /*choices*/
                 t[2]
             ),
@@ -11553,15 +11553,15 @@
     ), s.$on(
         "enter",
         /*onDropDownEnter*/
         t[6]
     ), a = new Fm({
         props: {
             value: (
-                /*color*/
+                /*currentColor*/
                 t[1]
             ),
             label: "Color",
             show_label: !1
         }
     }), a.$on(
         "change",
@@ -11575,147 +11575,155 @@
             $$scope: {
                 ctx: t
             }
         }
     }), _.$on(
         "click",
         /*click_handler*/
-        t[8]
+        t[10]
     ), d = new Vo({
         props: {
             variant: "primary",
             $$slots: {
                 default: [F1]
             },
             $$scope: {
                 ctx: t
             }
         }
     }), d.$on(
         "click",
         /*click_handler_1*/
-        t[9]
+        t[11]
     ), {
         c() {
-            e = yt("div"), n = yt("div"), i = yt("span"), l = yt("div"), ii(s.$$.fragment), o = Hl(), r = yt("div"), ii(a.$$.fragment), u = Hl(), f = yt("div"), ii(_.$$.fragment), h = Hl(), c = yt("div"), ii(d.$$.fragment), oi(l, "margin-right", "10px"), oi(r, "margin-right", "40px"), oi(r, "margin-bottom", "8px"), oi(f, "margin-right", "8px"), ni(i, "class", "model-content svelte-hkn2q1"), ni(n, "class", "modal-container svelte-hkn2q1"), ni(e, "class", "modal svelte-hkn2q1"), ni(e, "id", "model-box-edit");
+            e = Et("div"), n = Et("div"), i = Et("span"), l = Et("div"), oi(s.$$.fragment), o = Hl(), r = Et("div"), oi(a.$$.fragment), u = Hl(), f = Et("div"), oi(_.$$.fragment), h = Hl(), c = Et("div"), oi(d.$$.fragment), ui(l, "margin-right", "10px"), ui(r, "margin-right", "40px"), ui(r, "margin-bottom", "8px"), ui(f, "margin-right", "8px"), si(i, "class", "model-content svelte-hkn2q1"), si(n, "class", "modal-container svelte-hkn2q1"), si(e, "class", "modal svelte-hkn2q1"), si(e, "id", "model-box-edit");
         },
-        m(b, p) {
-            ys(b, e, p), Je(e, n), Je(n, i), Je(i, l), si(s, l, null), Je(i, o), Je(i, r), si(a, r, null), Je(i, u), Je(i, f), si(_, f, null), Je(i, h), Je(i, c), si(d, c, null), m = !0;
+        m(p, g) {
+            ys(p, e, g), Je(e, n), Je(n, i), Je(i, l), ai(s, l, null), Je(i, o), Je(i, r), ai(a, r, null), Je(i, u), Je(i, f), ai(_, f, null), Je(i, h), Je(i, c), ai(d, c, null), b = !0;
         },
-        p(b, [p]) {
+        p(p, [g]) {
             const y = {};
-            p & /*label*/
-                1 && (y.value = /*label*/
-                    b[0]), p & /*choices*/
+            g & /*currentLabel*/
+                1 && (y.value = /*currentLabel*/
+                    p[0]), g & /*choices*/
                 4 && (y.choices = /*choices*/
-                    b[2]), s.$set(y);
+                    p[2]), s.$set(y);
             const w = {};
-            p & /*color*/
-                2 && (w.value = /*color*/
-                    b[1]), a.$set(w);
+            g & /*currentColor*/
+                2 && (w.value = /*currentColor*/
+                    p[1]), a.$set(w);
             const C = {};
-            p & /*$$scope*/
-                4096 && (C.$$scope = {
-                    dirty: p,
-                    ctx: b
+            g & /*$$scope*/
+                16384 && (C.$$scope = {
+                    dirty: g,
+                    ctx: p
                 }), _.$set(C);
             const P = {};
-            p & /*$$scope*/
-                4096 && (P.$$scope = {
-                    dirty: p,
-                    ctx: b
+            g & /*$$scope*/
+                16384 && (P.$$scope = {
+                    dirty: g,
+                    ctx: p
                 }), d.$set(P);
         },
-        i(b) {
-            m || (ri(s.$$.fragment, b), ri(a.$$.fragment, b), ri(_.$$.fragment, b), ri(d.$$.fragment, b), m = !0);
+        i(p) {
+            b || (fi(s.$$.fragment, p), fi(a.$$.fragment, p), fi(_.$$.fragment, p), fi(d.$$.fragment, p), b = !0);
         },
-        o(b) {
-            ai(s.$$.fragment, b), ai(a.$$.fragment, b), ai(_.$$.fragment, b), ai(d.$$.fragment, b), m = !1;
+        o(p) {
+            ci(s.$$.fragment, p), ci(a.$$.fragment, p), ci(_.$$.fragment, p), ci(d.$$.fragment, p), b = !1;
         },
-        d(b) {
-            b && vs(e), li(s), li(a), li(_), li(d);
+        d(p) {
+            p && vs(e), ri(s), ri(a), ri(_), ri(d);
         }
     };
 }
 
 function z1(t, e, n) {
     let {
         label: i = ""
     } = e, {
-        choices: l = []
+        currentLabel: l = ""
+    } = e, {
+        choices: s = []
+    } = e, {
+        choicesColors: o = []
     } = e, {
-        choicesColors: s = []
+        color: r = ""
     } = e, {
-        color: o = ""
+        currentColor: a = ""
     } = e;
-    const r = O1();
+    const u = O1();
 
-    function a(m) {
-        r("change", {
-            label: i,
-            color: o,
-            ok: m
+    function f(g) {
+        u("change", {
+            label: l,
+            color: a,
+            ok: g
         });
     }
 
-    function u(m) {
+    function _(g) {
         const {
-            detail: b
-        } = m;
-        let p = b;
-        Number.isInteger(p) ? (Array.isArray(s) && p < s.length && n(1, o = s[p]), Array.isArray(l) && p < l.length && n(0, i = l[p][0])) : n(0, i = p);
+            detail: y
+        } = g;
+        let w = y;
+        Number.isInteger(w) ? (Array.isArray(o) && w < o.length && n(1, a = o[w]), Array.isArray(s) && w < s.length && n(0, l = s[w][0])) : n(0, l = w);
     }
 
-    function f(m) {
+    function h(g) {
         const {
-            detail: b
-        } = m;
-        n(1, o = b);
+            detail: y
+        } = g;
+        n(1, a = y);
     }
 
-    function _(m) {
-        u(m), a(!0);
+    function c(g) {
+        _(g), f(!0);
     }
 
-    function h(m) {
-        switch (m.key) {
+    function d(g) {
+        switch (g.key) {
             case "Enter":
-                a(!0);
+                f(!0);
                 break;
         }
     }
     D1(() => {
-        document.addEventListener("keydown", h);
+        document.addEventListener("keydown", d), n(0, l = i), n(1, a = r);
     }), R1(() => {
-        document.removeEventListener("keydown", h);
+        document.removeEventListener("keydown", d);
     });
-    const c = () => a(!1),
-        d = () => a(!0);
-    return t.$$set = (m) => {
-        "label" in m && n(0, i = m.label), "choices" in m && n(2, l = m.choices), "choicesColors" in m && n(7, s = m.choicesColors), "color" in m && n(1, o = m.color);
+    const b = () => f(!1),
+        p = () => f(!0);
+    return t.$$set = (g) => {
+        "label" in g && n(7, i = g.label), "currentLabel" in g && n(0, l = g.currentLabel), "choices" in g && n(2, s = g.choices), "choicesColors" in g && n(8, o = g.choicesColors), "color" in g && n(9, r = g.color), "currentColor" in g && n(1, a = g.currentColor);
     }, [
-        i,
-        o,
         l,
         a,
-        u,
+        s,
         f,
         _,
-        s,
+        h,
         c,
-        d
+        i,
+        o,
+        r,
+        b,
+        p
     ];
 }
 class Fa extends L1 {
     constructor(e) {
         super(), I1(this, e, z1, q1, M1, {
-            label: 0,
+            label: 7,
+            currentLabel: 0,
             choices: 2,
-            choicesColors: 7,
-            color: 1
+            choicesColors: 8,
+            color: 9,
+            currentColor: 1
         });
     }
 }
 const Ve = (t, e, n) => Math.min(Math.max(t, e), n);
 
 function Pl(t, e) {
     if (t.startsWith("rgba"))
@@ -11726,28 +11734,28 @@
     const [i, l, s] = n;
     return `rgba(${i}, ${l}, ${s}, ${e})`;
 }
 class Nl {
     constructor(e, n, i, l, s, o, r, a, u, f, _ = "rgb(255, 255, 255)", h = 0.5, c = 25, d = 1) {
         this.stopDrag = () => {
             this.isDragging = !1, document.removeEventListener("mousemove", this.handleDrag), document.removeEventListener("mouseup", this.stopDrag);
-        }, this.handleDrag = (m) => {
+        }, this.handleDrag = (b) => {
             if (this.isDragging) {
-                let b = m.clientX - this.offsetMouseX - this.xmin,
-                    p = m.clientY - this.offsetMouseY - this.ymin;
+                let p = b.clientX - this.offsetMouseX - this.xmin,
+                    g = b.clientY - this.offsetMouseY - this.ymin;
                 const y = this.canvasXmax - this.canvasXmin,
                     w = this.canvasYmax - this.canvasYmin;
-                b = Ve(b, -this.xmin, y - this.xmax), p = Ve(p, -this.ymin, w - this.ymax), this.xmin += b, this.ymin += p, this.xmax += b, this.ymax += p, this.updateHandles(), this.renderCallBack();
+                p = Ve(p, -this.xmin, y - this.xmax), g = Ve(g, -this.ymin, w - this.ymax), this.xmin += p, this.ymin += g, this.xmax += p, this.ymax += g, this.updateHandles(), this.renderCallBack();
             }
-        }, this.handleResize = (m) => {
+        }, this.handleResize = (b) => {
             if (this.isResizing) {
-                const b = m.clientX,
-                    p = m.clientY,
-                    y = b - this.resizeHandles[this.resizingHandleIndex].xmin - this.offsetMouseX,
-                    w = p - this.resizeHandles[this.resizingHandleIndex].ymin - this.offsetMouseY,
+                const p = b.clientX,
+                    g = b.clientY,
+                    y = p - this.resizeHandles[this.resizingHandleIndex].xmin - this.offsetMouseX,
+                    w = g - this.resizeHandles[this.resizingHandleIndex].ymin - this.offsetMouseY,
                     C = this.canvasXmax - this.canvasXmin,
                     P = this.canvasYmax - this.canvasYmin;
                 switch (this.resizingHandleIndex) {
                     case 0:
                         this.xmin += y, this.ymin += w, this.xmin = Ve(this.xmin, 0, this.xmax - this.minSize), this.ymin = Ve(this.ymin, 0, this.ymax - this.minSize);
                         break;
                     case 1:
@@ -11871,78 +11879,78 @@
     "rgb(255, 240, 245)",
     "rgb(255, 193, 37)",
     "rgb(255, 193, 7)",
     "rgb(255, 250, 138)"
 ];
 const {
     SvelteComponent: j1,
-    append: Wt,
-    attr: At,
+    append: Yt,
+    attr: Bt,
     binding_callbacks: G1,
     bubble: nr,
     check_outros: Ll,
-    create_component: Hn,
-    destroy_component: Pn,
-    detach: Zt,
-    element: tn,
+    create_component: In,
+    destroy_component: Mn,
+    detach: Jt,
+    element: ln,
     empty: x1,
     group_outros: Il,
     init: V1,
-    insert: Yt,
-    listen: rt,
-    mount_component: Nn,
+    insert: Qt,
+    listen: at,
+    mount_component: On,
     noop: X1,
     run_all: qa,
     safe_not_equal: W1,
-    space: Ln,
+    space: Dn,
     transition_in: Ce,
-    transition_out: je
+    transition_out: ze
 } = window.__gradio__svelte__internal, {
     onMount: Z1,
     onDestroy: Y1,
     createEventDispatcher: J1
 } = window.__gradio__svelte__internal;
 
 function ir(t) {
     let e, n, i, l, s, o, r, a, u, f, _, h;
     return i = new ym({}), o = new yc({}), u = new kr({}), {
         c() {
-            e = tn("span"), n = tn("button"), Hn(i.$$.fragment), l = Ln(), s = tn("button"), Hn(o.$$.fragment), r = Ln(), a = tn("button"), Hn(u.$$.fragment), At(n, "class", "icon svelte-182gnnj"), At(s, "class", "icon svelte-182gnnj"), At(a, "class", "icon svelte-182gnnj"), At(e, "class", "canvas-control svelte-182gnnj");
+            e = ln("span"), n = ln("button"), In(i.$$.fragment), l = Dn(), s = ln("button"), In(o.$$.fragment), r = Dn(), a = ln("button"), In(u.$$.fragment), Bt(n, "class", "icon svelte-182gnnj"), Bt(s, "class", "icon svelte-182gnnj"), Bt(a, "class", "icon svelte-182gnnj"), Bt(e, "class", "canvas-control svelte-182gnnj");
         },
         m(c, d) {
-            Yt(c, e, d), Wt(e, n), Nn(i, n, null), Wt(e, l), Wt(e, s), Nn(o, s, null), Wt(e, r), Wt(e, a), Nn(u, a, null), f = !0, _ || (h = [
-                rt(
+            Qt(c, e, d), Yt(e, n), On(i, n, null), Yt(e, l), Yt(e, s), On(o, s, null), Yt(e, r), Yt(e, a), On(u, a, null), f = !0, _ || (h = [
+                at(
                     n,
                     "click",
                     /*click_handler*/
                     t[22]
                 ),
-                rt(
+                at(
                     s,
                     "click",
                     /*click_handler_1*/
                     t[23]
                 ),
-                rt(
+                at(
                     a,
                     "click",
                     /*click_handler_2*/
                     t[24]
                 )
             ], _ = !0);
         },
         p: X1,
         i(c) {
             f || (Ce(i.$$.fragment, c), Ce(o.$$.fragment, c), Ce(u.$$.fragment, c), f = !0);
         },
         o(c) {
-            je(i.$$.fragment, c), je(o.$$.fragment, c), je(u.$$.fragment, c), f = !1;
+            ze(i.$$.fragment, c), ze(o.$$.fragment, c), ze(u.$$.fragment, c), f = !1;
         },
         d(c) {
-            c && Zt(e), Pn(i), Pn(o), Pn(u), _ = !1, qa(h);
+            c && Jt(e), Mn(i), Mn(o), Mn(u), _ = !1, qa(h);
         }
     };
 }
 
 function lr(t) {
     let e, n;
     return e = new Fa({
@@ -11967,15 +11975,15 @@
                     ].label
                 ) : ""
             ),
             color: (
                 /*selectedBox*/
                 t[5] >= 0 && /*selectedBox*/
                 t[5] < /*value*/
-                t[0].boxes.length ? Dn(
+                t[0].boxes.length ? qn(
                     /*value*/
                     t[0].boxes[
                         /*selectedBox*/
                         t[5]
                     ].color
                 ) : ""
             )
@@ -11986,18 +11994,18 @@
         t[14]
     ), e.$on(
         "enter{onModalEditChange}",
         /*enter_onModalEditChange_handler*/
         t[25]
     ), {
         c() {
-            Hn(e.$$.fragment);
+            In(e.$$.fragment);
         },
         m(i, l) {
-            Nn(e, i, l), n = !0;
+            On(e, i, l), n = !0;
         },
         p(i, l) {
             const s = {};
             l[0] & /*choices*/
                 4 && (s.choices = /*choices*/
                     i[2]), l[0] & /*choicesColors*/
                 8 && (s.choicesColors = /*choicesColors*/
@@ -12011,30 +12019,30 @@
                             /*selectedBox*/
                             i[5]
                         ].label
                     ) : ""), l[0] & /*selectedBox, value*/
                 33 && (s.color = /*selectedBox*/
                     i[5] >= 0 && /*selectedBox*/
                     i[5] < /*value*/
-                    i[0].boxes.length ? Dn(
+                    i[0].boxes.length ? qn(
                         /*value*/
                         i[0].boxes[
                             /*selectedBox*/
                             i[5]
                         ].color
                     ) : ""), e.$set(s);
         },
         i(i) {
             n || (Ce(e.$$.fragment, i), n = !0);
         },
         o(i) {
-            je(e.$$.fragment, i), n = !1;
+            ze(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            Pn(e, i);
+            Mn(e, i);
         }
     };
 }
 
 function sr(t) {
     let e, n;
     return e = new Fa({
@@ -12050,33 +12058,33 @@
             color: Array.isArray(
                     /*choicesColors*/
                     t[3]
                 ) && /*choicesColors*/
                 t[3].length > 0 ? (
                     /*choicesColors*/
                     t[3][0]
-                ) : Dn(Xe[
+                ) : qn(Xe[
                     /*value*/
                     t[0].boxes.length % Xe.length
                 ])
         }
     }), e.$on(
         "change",
         /*onModalNewChange*/
         t[11]
     ), e.$on(
         "enter{onModalNewChange}",
         /*enter_onModalNewChange_handler*/
         t[26]
     ), {
         c() {
-            Hn(e.$$.fragment);
+            In(e.$$.fragment);
         },
         m(i, l) {
-            Nn(e, i, l), n = !0;
+            On(e, i, l), n = !0;
         },
         p(i, l) {
             const s = {};
             l[0] & /*choices*/
                 4 && (s.choices = /*choices*/
                     i[2]), l[0] & /*choicesColors*/
                 8 && (s.choicesColors = /*choicesColors*/
@@ -12084,27 +12092,27 @@
                 9 && (s.color = Array.isArray(
                         /*choicesColors*/
                         i[3]
                     ) && /*choicesColors*/
                     i[3].length > 0 ? (
                         /*choicesColors*/
                         i[3][0]
-                    ) : Dn(Xe[
+                    ) : qn(Xe[
                         /*value*/
                         i[0].boxes.length % Xe.length
                     ])), e.$set(s);
         },
         i(i) {
             n || (Ce(e.$$.fragment, i), n = !0);
         },
         o(i) {
-            je(e.$$.fragment, i), n = !1;
+            ze(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            Pn(e, i);
+            Mn(e, i);
         }
     };
 }
 
 function Q1(t) {
     let e, n, i, l, s, o, r, a, u, f = (
             /*interactive*/
@@ -12116,85 +12124,85 @@
         ),
         h = (
             /*newModalVisible*/
             t[7] && sr(t)
         );
     return {
         c() {
-            e = tn("div"), n = tn("canvas"), i = Ln(), f && f.c(), l = Ln(), _ && _.c(), s = Ln(), h && h.c(), o = x1(), At(n, "class", "canvas-annotator svelte-182gnnj"), At(e, "class", "canvas-container svelte-182gnnj"), At(e, "tabindex", "-1");
+            e = ln("div"), n = ln("canvas"), i = Dn(), f && f.c(), l = Dn(), _ && _.c(), s = Dn(), h && h.c(), o = x1(), Bt(n, "class", "canvas-annotator svelte-182gnnj"), Bt(e, "class", "canvas-container svelte-182gnnj"), Bt(e, "tabindex", "-1");
         },
         m(c, d) {
-            Yt(c, e, d), Wt(e, n), t[21](n), Yt(c, i, d), f && f.m(c, d), Yt(c, l, d), _ && _.m(c, d), Yt(c, s, d), h && h.m(c, d), Yt(c, o, d), r = !0, a || (u = [
-                rt(
+            Qt(c, e, d), Yt(e, n), t[21](n), Qt(c, i, d), f && f.m(c, d), Qt(c, l, d), _ && _.m(c, d), Qt(c, s, d), h && h.m(c, d), Qt(c, o, d), r = !0, a || (u = [
+                at(
                     n,
                     "mousedown",
                     /*handleMouseDown*/
                     t[8]
                 ),
-                rt(
+                at(
                     n,
                     "mouseup",
                     /*handleMouseUp*/
                     t[9]
                 ),
-                rt(
+                at(
                     n,
                     "dblclick",
                     /*handleDoubleClick*/
                     t[13]
                 ),
-                rt(
+                at(
                     e,
                     "focusin",
                     /*handleCanvasFocus*/
                     t[16]
                 ),
-                rt(
+                at(
                     e,
                     "focusout",
                     /*handleCanvasBlur*/
                     t[17]
                 )
             ], a = !0);
         },
         p(c, d) {
             /*interactive*/
             c[1] ? f ? (f.p(c, d), d[0] & /*interactive*/
-                    2 && Ce(f, 1)) : (f = ir(c), f.c(), Ce(f, 1), f.m(l.parentNode, l)) : f && (Il(), je(f, 1, 1, () => {
+                    2 && Ce(f, 1)) : (f = ir(c), f.c(), Ce(f, 1), f.m(l.parentNode, l)) : f && (Il(), ze(f, 1, 1, () => {
                     f = null;
                 }), Ll()), /*editModalVisible*/
                 c[6] ? _ ? (_.p(c, d), d[0] & /*editModalVisible*/
-                    64 && Ce(_, 1)) : (_ = lr(c), _.c(), Ce(_, 1), _.m(s.parentNode, s)) : _ && (Il(), je(_, 1, 1, () => {
+                    64 && Ce(_, 1)) : (_ = lr(c), _.c(), Ce(_, 1), _.m(s.parentNode, s)) : _ && (Il(), ze(_, 1, 1, () => {
                     _ = null;
                 }), Ll()), /*newModalVisible*/
                 c[7] ? h ? (h.p(c, d), d[0] & /*newModalVisible*/
-                    128 && Ce(h, 1)) : (h = sr(c), h.c(), Ce(h, 1), h.m(o.parentNode, o)) : h && (Il(), je(h, 1, 1, () => {
+                    128 && Ce(h, 1)) : (h = sr(c), h.c(), Ce(h, 1), h.m(o.parentNode, o)) : h && (Il(), ze(h, 1, 1, () => {
                     h = null;
                 }), Ll());
         },
         i(c) {
             r || (Ce(f), Ce(_), Ce(h), r = !0);
         },
         o(c) {
-            je(f), je(_), je(h), r = !1;
+            ze(f), ze(_), ze(h), r = !1;
         },
         d(c) {
-            c && (Zt(e), Zt(i), Zt(l), Zt(s), Zt(o)), t[21](null), f && f.d(c), _ && _.d(c), h && h.d(c), a = !1, qa(u);
+            c && (Jt(e), Jt(i), Jt(l), Jt(s), Jt(o)), t[21](null), f && f.d(c), _ && _.d(c), h && h.d(c), a = !1, qa(u);
         }
     };
 }
 
 function or(t) {
     var e = parseInt(t.slice(1, 3), 16),
         n = parseInt(t.slice(3, 5), 16),
         i = parseInt(t.slice(5, 7), 16);
     return "rgb(" + e + ", " + n + ", " + i + ")";
 }
 
-function Dn(t) {
+function qn(t) {
     const e = t.match(/(\d+(\.\d+)?)/g),
         n = parseInt(e[0]),
         i = parseInt(e[1]),
         l = parseInt(e[2]);
     return "#" + (1 << 24 | n << 16 | i << 8 | l).toString(16).slice(1);
 }
 
@@ -12209,212 +12217,220 @@
         boxMinSize: o = 25
     } = e, {
         value: r
     } = e, {
         choices: a = []
     } = e, {
         choicesColors: u = []
-    } = e, f, _, h = null, c = -1, d = 0, m = 0, b = 0, p = 0, y = 1, w = 0, C = 0, P = !1, E = !1;
+    } = e, f, _, h = null, c = -1, d = 0, b = 0, p = 0, g = 0, y = 1, w = 0, C = 0, P = !1, E = !1;
     const N = J1();
 
     function v() {
         if (_) {
-            _.clearRect(0, 0, f.width, f.height), h !== null && _.drawImage(h, d, m, w, C);
+            _.clearRect(0, 0, f.width, f.height), h !== null && _.drawImage(h, d, b, w, C);
             for (const H of r.boxes.slice().reverse())
                 H.render(_);
         }
     }
 
     function A(H) {
-        n(5, c = H), r.boxes.forEach((R) => {
-            R.setSelected(!1);
+        n(5, c = H), r.boxes.forEach((U) => {
+            U.setSelected(!1);
         }), H >= 0 && H < r.boxes.length && r.boxes[H].setSelected(!0), v();
     }
 
     function B(H) {
         if (!l)
             return;
-        const R = f.getBoundingClientRect(),
-            j = H.clientX - R.left,
-            X = H.clientY - R.top;
-        for (const [he, Me] of r.boxes.entries()) {
-            const q = Me.indexOfPointInsideHandle(j, X);
-            if (q >= 0) {
-                A(he), Me.startResize(q, H);
+        const U = f.getBoundingClientRect(),
+            Q = H.clientX - U.left,
+            j = H.clientY - U.top;
+        for (const [je, M] of r.boxes.entries()) {
+            const tt = M.indexOfPointInsideHandle(Q, j);
+            if (tt >= 0) {
+                A(je), M.startResize(tt, H);
                 return;
             }
         }
-        for (const [he, Me] of r.boxes.entries())
-            if (Me.isPointInsideBox(j, X)) {
-                A(he), Me.startDrag(H);
+        for (const [je, M] of r.boxes.entries())
+            if (M.isPointInsideBox(Q, j)) {
+                A(je), M.startDrag(H);
                 return;
             }
         A(-1);
     }
 
     function L(H) {
         N("change");
     }
 
     function x(H) {
         if (l)
             switch (H.key) {
                 case "Delete":
-                    me();
+                    de();
                     break;
             }
     }
 
-    function J() {
+    function Y() {
         n(7, E = !0);
     }
 
-    function ce(H) {
+    function _e(H) {
         n(7, E = !1);
         const {
-            detail: R
+            detail: U
         } = H;
-        let j = R.label,
-            X = R.color;
-        if (R.ok) {
-            X === null || X === "" ? X = Xe[r.boxes.length % Xe.length] : X = or(X);
-            let Me = new Nl(v, d, m, b, p, j, Math.round(f.width / 3), Math.round(f.height / 3), Math.round(2 * f.width / 3), Math.round(2 * f.height / 3), X, s, o, y);
-            n(0, r.boxes = [Me, ...r.boxes], r), v(), N("change");
+        let Q = U.label,
+            j = U.color;
+        if (U.ok) {
+            j === null || j === "" ? j = Xe[r.boxes.length % Xe.length] : j = or(j);
+            let M = d + (p - d) / 3,
+                tt = p - (p - d) / 3,
+                Ut = b + (g - b) / 3,
+                bn = g - (g - b) / 3,
+                pn = new Nl(v, d, b, p, g, Q, Math.round(M), Math.round(Ut), Math.round(tt), Math.round(bn), j, s, o, y);
+            n(0, r.boxes = [pn, ...r.boxes], r), v(), N("change");
         }
     }
 
     function te() {
         c >= 0 && c < r.boxes.length && n(6, P = !0);
     }
 
-    function ke(H) {
+    function Ee(H) {
         l && te();
     }
 
-    function ye(H) {
+    function ve(H) {
         n(6, P = !1);
         const {
-            detail: R
+            detail: U
         } = H;
-        let j = R.label,
-            X = R.color;
-        if (R.ok && c >= 0 && c < r.boxes.length) {
-            let Me = r.boxes[c];
-            Me.label = j, Me.color = or(X), v(), N("change");
+        let Q = U.label,
+            j = U.color;
+        if (U.ok && c >= 0 && c < r.boxes.length) {
+            let M = r.boxes[c];
+            M.label = Q, M.color = or(j), v(), N("change");
         }
     }
 
-    function me() {
+    function de() {
         c >= 0 && c < r.boxes.length && (r.boxes.splice(c, 1), A(-1), N("change"));
     }
 
-    function _e() {
+    function ce() {
         if (f) {
             if (y = 1, n(4, f.width = f.clientWidth, f), h !== null)
                 if (h.width > f.width)
-                    y = f.width / h.width, w = h.width * y, C = h.height * y, d = 0, m = 0, b = w, p = C, n(4, f.height = C, f);
+                    y = f.width / h.width, w = h.width * y, C = h.height * y, d = 0, b = 0, p = w, g = C, n(4, f.height = C, f);
                 else {
                     w = h.width, C = h.height;
                     var H = (f.width - w) / 2;
-                    d = H, m = 0, b = H + w, p = h.height, n(4, f.height = C, f);
+                    d = H, b = 0, p = H + w, g = h.height, n(4, f.height = C, f);
                 }
             else
-                d = 0, m = 0, b = f.width, p = f.height, n(4, f.height = f.clientHeight, f);
-            if (b > 0 && p > 0)
-                for (const R of r.boxes)
-                    R.canvasXmin = d, R.canvasYmin = m, R.canvasXmax = b, R.canvasYmax = p, R.setScaleFactor(y);
+                d = 0, b = 0, p = f.width, g = f.height, n(4, f.height = f.clientHeight, f);
+            if (p > 0 && g > 0)
+                for (const U of r.boxes)
+                    U.canvasXmin = d, U.canvasYmin = b, U.canvasXmax = p, U.canvasYmax = g, U.setScaleFactor(y);
             v(), N("change");
         }
     }
-    const S = new ResizeObserver(_e);
+    const S = new ResizeObserver(ce);
 
     function k() {
         let H = [];
-        for (let R = 0; R < r.boxes.length; R++) {
-            let j = r.boxes[R];
-            if (!(j instanceof Nl)) {
-                let X = "",
-                    he = "";
-                j.hasOwnProperty("color") ? (X = j.color, Array.isArray(X) && X.length === 3 && (X = `rgb(${X[0]}, ${X[1]}, ${X[2]})`)) : X = Xe[H.length % Xe.length], j.hasOwnProperty("label") && (he = j.label), j = new Nl(v, d, m, b, p, he, j.xmin, j.ymin, j.xmax, j.ymax, X, s, o, y);
+        for (let U = 0; U < r.boxes.length; U++) {
+            let Q = r.boxes[U];
+            if (!(Q instanceof Nl)) {
+                let j = "",
+                    je = "";
+                Q.hasOwnProperty("color") ? (j = Q.color, Array.isArray(j) && j.length === 3 && (j = `rgb(${j[0]}, ${j[1]}, ${j[2]})`)) : j = Xe[H.length % Xe.length], Q.hasOwnProperty("label") && (je = Q.label), Q = new Nl(v, d, b, p, g, je, Q.xmin, Q.ymin, Q.xmax, Q.ymax, j, s, o, y);
             }
-            H.push(j);
+            H.push(Q);
         }
         n(0, r.boxes = H, r);
     }
+
+    function I() {
+        i !== null && (h === null || h.src != i) && (h = new Image(), h.src = i, h.onload = function() {
+            ce(), v();
+        });
+    }
     Z1(() => {
         if (Array.isArray(a) && a.length > 0 && (!Array.isArray(u) || u.length == 0))
             for (let H = 0; H < a.length; H++) {
-                let R = Xe[H % Xe.length];
-                u.push(Dn(R));
+                let U = Xe[H % Xe.length];
+                u.push(qn(U));
             }
-        _ = f.getContext("2d"), S.observe(f), i !== null && (h = new Image(), h.src = i, h.onload = function() {
-            _e(), v();
-        }), _e(), v();
+        _ = f.getContext("2d"), S.observe(f), I(), ce(), v();
     });
 
-    function I() {
+    function m() {
         document.addEventListener("keydown", x);
     }
 
-    function g() {
+    function T() {
         document.removeEventListener("keydown", x);
     }
     Y1(() => {
         document.removeEventListener("keydown", x);
     });
 
-    function T(H) {
+    function ae(H) {
         G1[H ? "unshift" : "push"](() => {
             f = H, n(4, f);
         });
     }
-    const ae = () => J(),
-        Q = () => te(),
-        Se = () => me();
+    const J = () => Y(),
+        ke = () => te(),
+        He = () => de();
 
-    function He(H) {
+    function R(H) {
         nr.call(this, t, H);
     }
 
-    function D(H) {
+    function Se(H) {
         nr.call(this, t, H);
     }
     return t.$$set = (H) => {
         "imageUrl" in H && n(18, i = H.imageUrl), "interactive" in H && n(1, l = H.interactive), "boxAlpha" in H && n(19, s = H.boxAlpha), "boxMinSize" in H && n(20, o = H.boxMinSize), "value" in H && n(0, r = H.value), "choices" in H && n(2, a = H.choices), "choicesColors" in H && n(3, u = H.choicesColors);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*value*/
-            1 && k();
+            1 && (I(), k(), ce(), v());
     }, [
         r,
         l,
         a,
         u,
         f,
         c,
         P,
         E,
         B,
         L,
-        J,
-        ce,
+        Y,
+        _e,
         te,
-        ke,
-        ye,
-        me,
-        I,
-        g,
+        Ee,
+        ve,
+        de,
+        m,
+        T,
         i,
         s,
         o,
-        T,
         ae,
-        Q,
-        Se,
+        J,
+        ke,
         He,
-        D
+        R,
+        Se
     ];
 }
 class $1 extends j1 {
     constructor(e) {
         super(), V1(
             this,
             e,
@@ -12543,27 +12559,27 @@
     } = e, {
         boxMinSize: a
     } = e, {
         value: u
     } = e, f, _;
     const h = cg();
 
-    function c(m) {
-        u = m, n(0, u);
+    function c(b) {
+        u = b, n(0, u);
     }
     const d = () => h("change");
-    return t.$$set = (m) => {
-        "src" in m && n(8, i = m.src), "interactive" in m && n(1, l = m.interactive), "boxesAlpha" in m && n(2, s = m.boxesAlpha), "labelList" in m && n(3, o = m.labelList), "labelColors" in m && n(4, r = m.labelColors), "boxMinSize" in m && n(5, a = m.boxMinSize), "value" in m && n(0, u = m.value);
+    return t.$$set = (b) => {
+        "src" in b && n(8, i = b.src), "interactive" in b && n(1, l = b.interactive), "boxesAlpha" in b && n(2, s = b.boxesAlpha), "labelList" in b && n(3, o = b.labelList), "labelColors" in b && n(4, r = b.labelColors), "boxMinSize" in b && n(5, a = b.boxMinSize), "value" in b && n(0, u = b.value);
     }, t.$$.update = () => {
         if (t.$$.dirty & /*src, latest_src*/
             768) {
             n(6, f = i), n(9, _ = i);
-            const m = i;
-            Th(m).then((b) => {
-                _ === m && n(6, f = b);
+            const b = i;
+            Th(b).then((p) => {
+                _ === b && n(6, f = p);
             });
         }
     }, [
         u,
         l,
         s,
         o,
@@ -12588,38 +12604,38 @@
             boxMinSize: 5,
             value: 0
         });
     }
 }
 const {
     SvelteComponent: dg,
-    add_flush_callback: Pi,
-    append: wn,
-    attr: An,
-    bind: Ni,
-    binding_callbacks: Rn,
+    add_flush_callback: Ii,
+    append: kn,
+    attr: Pn,
+    bind: Mi,
+    binding_callbacks: zn,
     bubble: Ml,
-    check_outros: Jt,
-    create_component: _t,
+    check_outros: Kt,
+    create_component: ht,
     create_slot: mg,
-    destroy_component: ht,
-    detach: Bt,
-    element: In,
+    destroy_component: dt,
+    detach: Tt,
+    element: Rn,
     empty: gg,
     get_all_dirty_from_scope: bg,
     get_slot_changes: pg,
-    group_outros: Qt,
+    group_outros: $t,
     init: wg,
-    insert: Tt,
-    mount_component: dt,
+    insert: Ht,
+    mount_component: mt,
     noop: vg,
     safe_not_equal: yg,
-    space: xt,
+    space: Xt,
     toggle_class: rr,
-    transition_in: W,
+    transition_in: X,
     transition_out: se,
     update_slot_base: Eg
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: kg
 } = window.__gradio__svelte__internal;
 
 function ar(t) {
@@ -12639,18 +12655,18 @@
             },
             $$scope: {
                 ctx: t
             }
         }
     }), {
         c() {
-            _t(e.$$.fragment);
+            ht(e.$$.fragment);
         },
         m(i, l) {
-            dt(e, i, l), n = !0;
+            mt(e, i, l), n = !0;
         },
         p(i, l) {
             const s = {};
             l[0] & /*value*/
                 2 && (s.href = /*value*/
                     i[1].image.url), l[0] & /*value*/
                 2 && (s.download = /*value*/
@@ -12658,21 +12674,21 @@
                 256 | l[1] & /*$$scope*/
                 16 && (s.$$scope = {
                     dirty: l,
                     ctx: i
                 }), e.$set(s);
         },
         i(i) {
-            n || (W(e.$$.fragment, i), n = !0);
+            n || (X(e.$$.fragment, i), n = !0);
         },
         o(i) {
             se(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            ht(e, i);
+            dt(e, i);
         }
     };
 }
 
 function Sg(t) {
     let e, n;
     return e = new as({
@@ -12681,33 +12697,33 @@
             label: (
                 /*i18n*/
                 t[8]("common.download")
             )
         }
     }), {
         c() {
-            _t(e.$$.fragment);
+            ht(e.$$.fragment);
         },
         m(i, l) {
-            dt(e, i, l), n = !0;
+            mt(e, i, l), n = !0;
         },
         p(i, l) {
             const s = {};
             l[0] & /*i18n*/
                 256 && (s.label = /*i18n*/
                     i[8]("common.download")), e.$set(s);
         },
         i(i) {
-            n || (W(e.$$.fragment, i), n = !0);
+            n || (X(e.$$.fragment, i), n = !0);
         },
         o(i) {
             se(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            ht(e, i);
+            dt(e, i);
         }
     };
 }
 
 function ur(t) {
     let e, n;
     return e = new g_({
@@ -12731,35 +12747,35 @@
         t[26]
     ), e.$on(
         "error",
         /*error_handler*/
         t[27]
     ), {
         c() {
-            _t(e.$$.fragment);
+            ht(e.$$.fragment);
         },
         m(i, l) {
-            dt(e, i, l), n = !0;
+            mt(e, i, l), n = !0;
         },
         p(i, l) {
             const s = {};
             l[0] & /*i18n*/
                 256 && (s.i18n = /*i18n*/
                     i[8]), l[0] & /*value*/
                 2 && (s.value = /*value*/
                     i[1]), e.$set(s);
         },
         i(i) {
-            n || (W(e.$$.fragment, i), n = !0);
+            n || (X(e.$$.fragment, i), n = !0);
         },
         o(i) {
             se(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            ht(e, i);
+            dt(e, i);
         }
     };
 }
 
 function fr(t) {
     let e, n, i;
     return n = new as({
@@ -12769,28 +12785,28 @@
         }
     }), n.$on(
         "click",
         /*clear*/
         t[23]
     ), {
         c() {
-            e = In("div"), _t(n.$$.fragment);
+            e = Rn("div"), ht(n.$$.fragment);
         },
         m(l, s) {
-            Tt(l, e, s), dt(n, e, null), i = !0;
+            Ht(l, e, s), mt(n, e, null), i = !0;
         },
         p: vg,
         i(l) {
-            i || (W(n.$$.fragment, l), i = !0);
+            i || (X(n.$$.fragment, l), i = !0);
         },
         o(l) {
             se(n.$$.fragment, l), i = !1;
         },
         d(l) {
-            l && Bt(e), ht(n);
+            l && Tt(e), dt(n);
         }
     };
 }
 
 function cr(t) {
     let e;
     const n = (
@@ -12829,15 +12845,15 @@
                     /*$$scope*/
                     l[35]
                 ),
                 null
             );
         },
         i(l) {
-            e || (W(i, l), e = !0);
+            e || (X(i, l), e = !0);
         },
         o(l) {
             se(i, l), e = !1;
         },
         d(l) {
             i && i.d(l);
         }
@@ -12850,31 +12866,31 @@
         t[1] === null && cr(t)
     );
     return {
         c() {
             i && i.c(), e = gg();
         },
         m(l, s) {
-            i && i.m(l, s), Tt(l, e, s), n = !0;
+            i && i.m(l, s), Ht(l, e, s), n = !0;
         },
         p(l, s) {
             /*value*/
             l[1] === null ? i ? (i.p(l, s), s[0] & /*value*/
-                2 && W(i, 1)) : (i = cr(l), i.c(), W(i, 1), i.m(e.parentNode, e)) : i && (Qt(), se(i, 1, 1, () => {
+                2 && X(i, 1)) : (i = cr(l), i.c(), X(i, 1), i.m(e.parentNode, e)) : i && ($t(), se(i, 1, 1, () => {
                 i = null;
-            }), Jt());
+            }), Kt());
         },
         i(l) {
-            n || (W(i), n = !0);
+            n || (X(i), n = !0);
         },
         o(l) {
             se(i), n = !1;
         },
         d(l) {
-            l && Bt(e), i && i.d(l);
+            l && Tt(e), i && i.d(l);
         }
     };
 }
 
 function _r(t) {
     let e, n, i, l;
 
@@ -12908,29 +12924,29 @@
         )
     };
     return (
         /*value*/
         t[1] !== void 0 && (o.value = /*value*/
             t[1]), n = new za({
             props: o
-        }), Rn.push(() => Ni(n, "value", s)), n.$on(
+        }), zn.push(() => Mi(n, "value", s)), n.$on(
             "change",
             /*change_handler*/
             t[33]
         ), {
             c() {
-                e = In("div"), _t(n.$$.fragment), An(e, "class", "image-frame svelte-1gjdske"), rr(
+                e = Rn("div"), ht(n.$$.fragment), Pn(e, "class", "image-frame svelte-1gjdske"), rr(
                     e,
                     "selectable",
                     /*selectable*/
                     t[5]
                 );
             },
             m(r, a) {
-                Tt(r, e, a), dt(n, e, null), l = !0;
+                Ht(r, e, a), mt(n, e, null), l = !0;
             },
             p(r, a) {
                 const u = {};
                 a[0] & /*boxesAlpha*/
                     4096 && (u.boxesAlpha = /*boxesAlpha*/
                         r[12]), a[0] & /*labelList*/
                     8192 && (u.labelList = /*labelList*/
@@ -12940,30 +12956,30 @@
                     32768 && (u.boxMinSize = /*boxMinSize*/
                         r[15]), a[0] & /*interactive*/
                     128 && (u.interactive = /*interactive*/
                         r[7]), a[0] & /*value*/
                     2 && (u.src = /*value*/
                         r[1].image.url), !i && a[0] & /*value*/
                     2 && (i = !0, u.value = /*value*/
-                        r[1], Pi(() => i = !1)), n.$set(u), (!l || a[0] & /*selectable*/
+                        r[1], Ii(() => i = !1)), n.$set(u), (!l || a[0] & /*selectable*/
                         32) && rr(
                         e,
                         "selectable",
                         /*selectable*/
                         r[5]
                     );
             },
             i(r) {
-                l || (W(n.$$.fragment, r), l = !0);
+                l || (X(n.$$.fragment, r), l = !0);
             },
             o(r) {
                 se(n.$$.fragment, r), l = !1;
             },
             d(r) {
-                r && Bt(e), ht(n);
+                r && Tt(e), dt(n);
             }
         }
     );
 }
 
 function hr(t) {
     let e, n, i;
@@ -12986,70 +13002,70 @@
         )
     };
     return (
         /*active_source*/
         t[0] !== void 0 && (s.active_source = /*active_source*/
             t[0]), e = new L_({
             props: s
-        }), Rn.push(() => Ni(e, "active_source", l)), {
+        }), zn.push(() => Mi(e, "active_source", l)), {
             c() {
-                _t(e.$$.fragment);
+                ht(e.$$.fragment);
             },
             m(o, r) {
-                dt(e, o, r), i = !0;
+                mt(e, o, r), i = !0;
             },
             p(o, r) {
                 const a = {};
                 r[0] & /*sources*/
                     16 && (a.sources = /*sources*/
                         o[4]), !n && r[0] & /*active_source*/
                     1 && (n = !0, a.active_source = /*active_source*/
-                        o[0], Pi(() => n = !1)), e.$set(a);
+                        o[0], Ii(() => n = !1)), e.$set(a);
             },
             i(o) {
-                i || (W(e.$$.fragment, o), i = !0);
+                i || (X(e.$$.fragment, o), i = !0);
             },
             o(o) {
                 se(e.$$.fragment, o), i = !1;
             },
             d(o) {
-                ht(e, o);
+                dt(e, o);
             }
         }
     );
 }
 
 function Ag(t) {
     let e, n, i, l, s, o, r, a, u, f, _, h, c, d = (
             /*sources*/
             (t[4].length > 1 || /*sources*/
                 t[4].includes("clipboard")) && /*value*/
             t[1] === null && /*interactive*/
             t[7]
         ),
-        m;
+        b;
     e = new sf({
         props: {
             show_label: (
                 /*show_label*/
                 t[3]
             ),
             Icon: Sr,
             label: (
                 /*label*/
                 t[2] || "Image Annotator"
             )
         }
     });
-    let b = (
+    let p = (
             /*showDownloadButton*/
             t[10] && /*value*/
             t[1] !== null && ar(t)
         ),
-        p = (
+        g = (
             /*showShareButton*/
             t[9] && /*value*/
             t[1] !== null && ur(t)
         ),
         y = (
             /*showClearButton*/
             t[11] && /*value*/
@@ -13088,15 +13104,15 @@
     };
     /*uploading*/
     t[16] !== void 0 && (P.uploading = /*uploading*/
             t[16]), /*dragging*/
         t[17] !== void 0 && (P.dragging = /*dragging*/
             t[17]), u = new dm({
             props: P
-        }), t[28](u), Rn.push(() => Ni(u, "uploading", w)), Rn.push(() => Ni(u, "dragging", C)), u.$on(
+        }), t[28](u), zn.push(() => Mi(u, "uploading", w)), zn.push(() => Mi(u, "dragging", C)), u.$on(
             "load",
             /*handle_upload*/
             t[19]
         ), u.$on(
             "error",
             /*error_handler_1*/
             t[31]
@@ -13104,42 +13120,42 @@
     let E = (
             /*value*/
             t[1] !== null && _r(t)
         ),
         N = d && hr(t);
     return {
         c() {
-            _t(e.$$.fragment), n = xt(), i = In("div"), b && b.c(), l = xt(), p && p.c(), s = xt(), y && y.c(), o = xt(), r = In("div"), a = In("div"), _t(u.$$.fragment), h = xt(), E && E.c(), c = xt(), N && N.c(), An(i, "class", "icon-buttons svelte-1gjdske"), An(a, "class", "upload-container svelte-1gjdske"), An(r, "data-testid", "image"), An(r, "class", "image-container svelte-1gjdske");
+            ht(e.$$.fragment), n = Xt(), i = Rn("div"), p && p.c(), l = Xt(), g && g.c(), s = Xt(), y && y.c(), o = Xt(), r = Rn("div"), a = Rn("div"), ht(u.$$.fragment), h = Xt(), E && E.c(), c = Xt(), N && N.c(), Pn(i, "class", "icon-buttons svelte-1gjdske"), Pn(a, "class", "upload-container svelte-1gjdske"), Pn(r, "data-testid", "image"), Pn(r, "class", "image-container svelte-1gjdske");
         },
         m(v, A) {
-            dt(e, v, A), Tt(v, n, A), Tt(v, i, A), b && b.m(i, null), wn(i, l), p && p.m(i, null), wn(i, s), y && y.m(i, null), Tt(v, o, A), Tt(v, r, A), wn(r, a), dt(u, a, null), wn(a, h), E && E.m(a, null), wn(r, c), N && N.m(r, null), m = !0;
+            mt(e, v, A), Ht(v, n, A), Ht(v, i, A), p && p.m(i, null), kn(i, l), g && g.m(i, null), kn(i, s), y && y.m(i, null), Ht(v, o, A), Ht(v, r, A), kn(r, a), mt(u, a, null), kn(a, h), E && E.m(a, null), kn(r, c), N && N.m(r, null), b = !0;
         },
         p(v, A) {
             const B = {};
             A[0] & /*show_label*/
                 8 && (B.show_label = /*show_label*/
                     v[3]), A[0] & /*label*/
                 4 && (B.label = /*label*/
                     v[2] || "Image Annotator"), e.$set(B), /*showDownloadButton*/
                 v[10] && /*value*/
-                v[1] !== null ? b ? (b.p(v, A), A[0] & /*showDownloadButton, value*/
-                    1026 && W(b, 1)) : (b = ar(v), b.c(), W(b, 1), b.m(i, l)) : b && (Qt(), se(b, 1, 1, () => {
-                    b = null;
-                }), Jt()), /*showShareButton*/
-                v[9] && /*value*/
-                v[1] !== null ? p ? (p.p(v, A), A[0] & /*showShareButton, value*/
-                    514 && W(p, 1)) : (p = ur(v), p.c(), W(p, 1), p.m(i, s)) : p && (Qt(), se(p, 1, 1, () => {
+                v[1] !== null ? p ? (p.p(v, A), A[0] & /*showDownloadButton, value*/
+                    1026 && X(p, 1)) : (p = ar(v), p.c(), X(p, 1), p.m(i, l)) : p && ($t(), se(p, 1, 1, () => {
                     p = null;
-                }), Jt()), /*showClearButton*/
+                }), Kt()), /*showShareButton*/
+                v[9] && /*value*/
+                v[1] !== null ? g ? (g.p(v, A), A[0] & /*showShareButton, value*/
+                    514 && X(g, 1)) : (g = ur(v), g.c(), X(g, 1), g.m(i, s)) : g && ($t(), se(g, 1, 1, () => {
+                    g = null;
+                }), Kt()), /*showClearButton*/
                 v[11] && /*value*/
                 v[1] !== null && /*interactive*/
                 v[7] ? y ? (y.p(v, A), A[0] & /*showClearButton, value, interactive*/
-                    2178 && W(y, 1)) : (y = fr(v), y.c(), W(y, 1), y.m(i, null)) : y && (Qt(), se(y, 1, 1, () => {
+                    2178 && X(y, 1)) : (y = fr(v), y.c(), X(y, 1), y.m(i, null)) : y && ($t(), se(y, 1, 1, () => {
                     y = null;
-                }), Jt());
+                }), Kt());
             const L = {};
             A[0] & /*value*/
                 2 && (L.hidden = /*value*/
                     v[1] !== null), A[0] & /*active_source*/
                 1 && (L.filetype = /*active_source*/
                     v[0] === "clipboard" ? "clipboard" : "image/*"), A[0] & /*root*/
                 64 && (L.root = /*root*/
@@ -13148,38 +13164,38 @@
                     v[4].includes("upload")), A[0] & /*value*/
                 2 | A[1] & /*$$scope*/
                 16 && (L.$$scope = {
                     dirty: A,
                     ctx: v
                 }), !f && A[0] & /*uploading*/
                 65536 && (f = !0, L.uploading = /*uploading*/
-                    v[16], Pi(() => f = !1)), !_ && A[0] & /*dragging*/
+                    v[16], Ii(() => f = !1)), !_ && A[0] & /*dragging*/
                 131072 && (_ = !0, L.dragging = /*dragging*/
-                    v[17], Pi(() => _ = !1)), u.$set(L), /*value*/
+                    v[17], Ii(() => _ = !1)), u.$set(L), /*value*/
                 v[1] !== null ? E ? (E.p(v, A), A[0] & /*value*/
-                    2 && W(E, 1)) : (E = _r(v), E.c(), W(E, 1), E.m(a, null)) : E && (Qt(), se(E, 1, 1, () => {
+                    2 && X(E, 1)) : (E = _r(v), E.c(), X(E, 1), E.m(a, null)) : E && ($t(), se(E, 1, 1, () => {
                     E = null;
-                }), Jt()), A[0] & /*sources, value, interactive*/
+                }), Kt()), A[0] & /*sources, value, interactive*/
                 146 && (d = /*sources*/
                     (v[4].length > 1 || /*sources*/
                         v[4].includes("clipboard")) && /*value*/
                     v[1] === null && /*interactive*/
                     v[7]), d ? N ? (N.p(v, A), A[0] & /*sources, value, interactive*/
-                    146 && W(N, 1)) : (N = hr(v), N.c(), W(N, 1), N.m(r, null)) : N && (Qt(), se(N, 1, 1, () => {
+                    146 && X(N, 1)) : (N = hr(v), N.c(), X(N, 1), N.m(r, null)) : N && ($t(), se(N, 1, 1, () => {
                     N = null;
-                }), Jt());
+                }), Kt());
         },
         i(v) {
-            m || (W(e.$$.fragment, v), W(b), W(p), W(y), W(u.$$.fragment, v), W(E), W(N), m = !0);
+            b || (X(e.$$.fragment, v), X(p), X(g), X(y), X(u.$$.fragment, v), X(E), X(N), b = !0);
         },
         o(v) {
-            se(e.$$.fragment, v), se(b), se(p), se(y), se(u.$$.fragment, v), se(E), se(N), m = !1;
+            se(e.$$.fragment, v), se(p), se(g), se(y), se(u.$$.fragment, v), se(E), se(N), b = !1;
         },
         d(v) {
-            v && (Bt(n), Bt(i), Bt(o), Bt(r)), ht(e, v), b && b.d(), p && p.d(), y && y.d(), t[28](null), ht(u), E && E.d(), N && N.d();
+            v && (Tt(n), Tt(i), Tt(o), Tt(r)), dt(e, v), p && p.d(), g && g.d(), y && y.d(), t[28](null), dt(u), E && E.d(), N && N.d();
         }
     };
 }
 
 function Bg(t, e, n) {
     let {
         $$slots: i = {},
@@ -13201,87 +13217,87 @@
     } = e, {
         i18n: h
     } = e, {
         showShareButton: c
     } = e, {
         showDownloadButton: d
     } = e, {
-        showClearButton: m
+        showClearButton: b
     } = e, {
-        boxesAlpha: b
+        boxesAlpha: p
     } = e, {
-        labelList: p
+        labelList: g
     } = e, {
         labelColors: y
     } = e, {
         boxMinSize: w
     } = e, C, P = !1, {
         active_source: E = null
     } = e;
 
     function N({
-        detail: g
+        detail: m
     }) {
-        n(1, s = new Sh()), n(1, s.image = g, s), A("upload");
+        n(1, s = new Sh()), n(1, s.image = m, s), A("upload");
     }
 
     function v() {
         x(), A("clear"), A("change");
     }
     const A = kg();
     let B = !1;
-    async function L(g) {
-        switch (g) {
+    async function L(m) {
+        switch (m) {
             case "clipboard":
                 C.paste_clipboard();
                 break;
         }
     }
 
     function x() {
         n(1, s = null);
     }
-    const J = async (g) => g === null ? "" : `<img src="${await i_(g.image, "base64")}" />`;
+    const Y = async (m) => m === null ? "" : `<img src="${await i_(m.image, "base64")}" />`;
 
-    function ce(g) {
-        Ml.call(this, t, g);
+    function _e(m) {
+        Ml.call(this, t, m);
     }
 
-    function te(g) {
-        Ml.call(this, t, g);
+    function te(m) {
+        Ml.call(this, t, m);
     }
 
-    function ke(g) {
-        Rn[g ? "unshift" : "push"](() => {
-            C = g, n(18, C);
+    function Ee(m) {
+        zn[m ? "unshift" : "push"](() => {
+            C = m, n(18, C);
         });
     }
 
-    function ye(g) {
-        P = g, n(16, P);
+    function ve(m) {
+        P = m, n(16, P);
     }
 
-    function me(g) {
-        B = g, n(17, B);
+    function de(m) {
+        B = m, n(17, B);
     }
 
-    function _e(g) {
-        Ml.call(this, t, g);
+    function ce(m) {
+        Ml.call(this, t, m);
     }
 
-    function S(g) {
-        s = g, n(1, s);
+    function S(m) {
+        s = m, n(1, s);
     }
     const k = () => A("change");
 
-    function I(g) {
-        E = g, n(0, E), n(4, a);
+    function I(m) {
+        E = m, n(0, E), n(4, a);
     }
-    return t.$$set = (g) => {
-        "value" in g && n(1, s = g.value), "label" in g && n(2, o = g.label), "show_label" in g && n(3, r = g.show_label), "sources" in g && n(4, a = g.sources), "selectable" in g && n(5, u = g.selectable), "root" in g && n(6, f = g.root), "interactive" in g && n(7, _ = g.interactive), "i18n" in g && n(8, h = g.i18n), "showShareButton" in g && n(9, c = g.showShareButton), "showDownloadButton" in g && n(10, d = g.showDownloadButton), "showClearButton" in g && n(11, m = g.showClearButton), "boxesAlpha" in g && n(12, b = g.boxesAlpha), "labelList" in g && n(13, p = g.labelList), "labelColors" in g && n(14, y = g.labelColors), "boxMinSize" in g && n(15, w = g.boxMinSize), "active_source" in g && n(0, E = g.active_source), "$$scope" in g && n(35, l = g.$$scope);
+    return t.$$set = (m) => {
+        "value" in m && n(1, s = m.value), "label" in m && n(2, o = m.label), "show_label" in m && n(3, r = m.show_label), "sources" in m && n(4, a = m.sources), "selectable" in m && n(5, u = m.selectable), "root" in m && n(6, f = m.root), "interactive" in m && n(7, _ = m.interactive), "i18n" in m && n(8, h = m.i18n), "showShareButton" in m && n(9, c = m.showShareButton), "showDownloadButton" in m && n(10, d = m.showDownloadButton), "showClearButton" in m && n(11, b = m.showClearButton), "boxesAlpha" in m && n(12, p = m.boxesAlpha), "labelList" in m && n(13, g = m.labelList), "labelColors" in m && n(14, y = m.labelColors), "boxMinSize" in m && n(15, w = m.boxMinSize), "active_source" in m && n(0, E = m.active_source), "$$scope" in m && n(35, l = m.$$scope);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*uploading*/
             65536 && P && x(), t.$$.dirty[0] & /*dragging*/
             131072 && A("drag", B), t.$$.dirty[0] & /*active_source, sources*/
             17 && !E && a && n(0, E = a[0]);
     }, [
         E,
@@ -13291,35 +13307,35 @@
         a,
         u,
         f,
         _,
         h,
         c,
         d,
-        m,
         b,
         p,
+        g,
         y,
         w,
         P,
         B,
         C,
         N,
         v,
         A,
         L,
         x,
         i,
-        J,
-        ce,
-        te,
-        ke,
-        ye,
-        me,
+        Y,
         _e,
+        te,
+        Ee,
+        ve,
+        de,
+        ce,
         S,
         k,
         I,
         l
     ];
 }
 class Tg extends dg {
@@ -13361,16 +13377,16 @@
     detach: Mg,
     element: Og,
     group_outros: Dg,
     init: Rg,
     insert: Ug,
     mount_component: Fg,
     safe_not_equal: qg,
-    toggle_class: ot,
-    transition_in: bi,
+    toggle_class: rt,
+    transition_in: vi,
     transition_out: rs
 } = window.__gradio__svelte__internal;
 
 function dr(t) {
     let e, n;
     return e = new za({
         props: {
@@ -13392,15 +13408,15 @@
             const s = {};
             l & /*samples_dir, value*/
                 3 && (s.src = /*samples_dir*/
                     i[1] + /*value*/
                     i[0].path), e.$set(s);
         },
         i(i) {
-            n || (bi(e.$$.fragment, i), n = !0);
+            n || (vi(e.$$.fragment, i), n = !0);
         },
         o(i) {
             rs(e.$$.fragment, i), n = !1;
         },
         d(i) {
             Ig(e, i);
         }
@@ -13410,72 +13426,72 @@
 function zg(t) {
     let e, n, i = (
         /*value*/
         t[0] && dr(t)
     );
     return {
         c() {
-            e = Og("div"), i && i.c(), Pg(e, "class", "container svelte-1sgcyba"), ot(
+            e = Og("div"), i && i.c(), Pg(e, "class", "container svelte-1sgcyba"), rt(
                 e,
                 "table",
                 /*type*/
                 t[2] === "table"
-            ), ot(
+            ), rt(
                 e,
                 "gallery",
                 /*type*/
                 t[2] === "gallery"
-            ), ot(
+            ), rt(
                 e,
                 "selected",
                 /*selected*/
                 t[3]
-            ), ot(
+            ), rt(
                 e,
                 "border",
                 /*value*/
                 t[0]
             );
         },
         m(l, s) {
             Ug(l, e, s), i && i.m(e, null), n = !0;
         },
         p(l, [s]) {
             /*value*/
             l[0] ? i ? (i.p(l, s), s & /*value*/
-                1 && bi(i, 1)) : (i = dr(l), i.c(), bi(i, 1), i.m(e, null)) : i && (Dg(), rs(i, 1, 1, () => {
+                1 && vi(i, 1)) : (i = dr(l), i.c(), vi(i, 1), i.m(e, null)) : i && (Dg(), rs(i, 1, 1, () => {
                 i = null;
             }), Ng()), (!n || s & /*type*/
-                4) && ot(
+                4) && rt(
                 e,
                 "table",
                 /*type*/
                 l[2] === "table"
             ), (!n || s & /*type*/
-                4) && ot(
+                4) && rt(
                 e,
                 "gallery",
                 /*type*/
                 l[2] === "gallery"
             ), (!n || s & /*selected*/
-                8) && ot(
+                8) && rt(
                 e,
                 "selected",
                 /*selected*/
                 l[3]
             ), (!n || s & /*value*/
-                1) && ot(
+                1) && rt(
                 e,
                 "border",
                 /*value*/
                 l[0]
             );
         },
         i(l) {
-            n || (bi(i), n = !0);
+            n || (vi(i), n = !0);
         },
         o(l) {
             rs(i), n = !1;
         },
         d(l) {
             l && Mg(e), i && i.d();
         }
@@ -13509,25 +13525,25 @@
 const {
     SvelteComponent: Gg,
     add_flush_callback: mr,
     assign: xg,
     bind: gr,
     binding_callbacks: br,
     check_outros: Vg,
-    create_component: It,
-    destroy_component: Mt,
+    create_component: Mt,
+    destroy_component: Ot,
     detach: ja,
     empty: Xg,
     flush: $,
     get_spread_object: Wg,
     get_spread_update: Zg,
     group_outros: Yg,
     init: Jg,
     insert: Ga,
-    mount_component: Ot,
+    mount_component: Dt,
     safe_not_equal: Qg,
     space: Kg,
     transition_in: $e,
     transition_out: et
 } = window.__gradio__svelte__internal;
 
 function $g(t) {
@@ -13541,18 +13557,18 @@
             },
             $$scope: {
                 ctx: t
             }
         }
     }), {
         c() {
-            It(e.$$.fragment);
+            Mt(e.$$.fragment);
         },
         m(i, l) {
-            Ot(e, i, l), n = !0;
+            Dt(e, i, l), n = !0;
         },
         p(i, l) {
             const s = {};
             l[1] & /*$$scope*/
                 32 && (s.$$scope = {
                     dirty: l,
                     ctx: i
@@ -13561,15 +13577,15 @@
         i(i) {
             n || ($e(e.$$.fragment, i), n = !0);
         },
         o(i) {
             et(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            Mt(e, i);
+            Ot(e, i);
         }
     };
 }
 
 function eb(t) {
     let e, n;
     return e = new Pr({
@@ -13579,33 +13595,33 @@
                 t[23].i18n
             ),
             type: "clipboard",
             mode: "short"
         }
     }), {
         c() {
-            It(e.$$.fragment);
+            Mt(e.$$.fragment);
         },
         m(i, l) {
-            Ot(e, i, l), n = !0;
+            Dt(e, i, l), n = !0;
         },
         p(i, l) {
             const s = {};
             l[0] & /*gradio*/
                 8388608 && (s.i18n = /*gradio*/
                     i[23].i18n), e.$set(s);
         },
         i(i) {
             n || ($e(e.$$.fragment, i), n = !0);
         },
         o(i) {
             et(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            Mt(e, i);
+            Ot(e, i);
         }
     };
 }
 
 function tb(t) {
     let e, n;
     return e = new Pr({
@@ -13614,54 +13630,54 @@
                 /*gradio*/
                 t[23].i18n
             ),
             type: "image"
         }
     }), {
         c() {
-            It(e.$$.fragment);
+            Mt(e.$$.fragment);
         },
         m(i, l) {
-            Ot(e, i, l), n = !0;
+            Dt(e, i, l), n = !0;
         },
         p(i, l) {
             const s = {};
             l[0] & /*gradio*/
                 8388608 && (s.i18n = /*gradio*/
                     i[23].i18n), e.$set(s);
         },
         i(i) {
             n || ($e(e.$$.fragment, i), n = !0);
         },
         o(i) {
             et(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            Mt(e, i);
+            Ot(e, i);
         }
     };
 }
 
 function nb(t) {
     let e, n;
     return e = new Sr({}), {
         c() {
-            It(e.$$.fragment);
+            Mt(e.$$.fragment);
         },
         m(i, l) {
-            Ot(e, i, l), n = !0;
+            Dt(e, i, l), n = !0;
         },
         i(i) {
             n || ($e(e.$$.fragment, i), n = !0);
         },
         o(i) {
             et(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            Mt(e, i);
+            Ot(e, i);
         }
     };
 }
 
 function ib(t) {
     let e, n, i, l;
     const s = [tb, eb, $g],
@@ -13832,18 +13848,18 @@
             t[34]
         ), i.$on(
             "error",
             /*error_handler*/
             t[35]
         ), {
             c() {
-                It(e.$$.fragment), n = Kg(), It(i.$$.fragment);
+                Mt(e.$$.fragment), n = Kg(), Mt(i.$$.fragment);
             },
             m(h, c) {
-                Ot(e, h, c), Ga(h, n, c), Ot(i, h, c), o = !0;
+                Dt(e, h, c), Ga(h, n, c), Dt(i, h, c), o = !0;
             },
             p(h, c) {
                 const d = c[0] & /*gradio, loading_status*/
                     8388610 ? Zg(r, [
                         c[0] & /*gradio*/
                         8388608 && {
                             autoscroll: (
@@ -13861,62 +13877,62 @@
                         c[0] & /*loading_status*/
                         2 && Wg(
                             /*loading_status*/
                             h[1]
                         )
                     ]) : {};
                 e.$set(d);
-                const m = {};
+                const b = {};
                 c[0] & /*_selectable*/
-                    1024 && (m.selectable = /*_selectable*/
+                    1024 && (b.selectable = /*_selectable*/
                         h[10]), c[0] & /*root*/
-                    128 && (m.root = /*root*/
+                    128 && (b.root = /*root*/
                         h[7]), c[0] & /*sources*/
-                    16384 && (m.sources = /*sources*/
+                    16384 && (b.sources = /*sources*/
                         h[14]), c[0] & /*interactive*/
-                    262144 && (m.interactive = /*interactive*/
+                    262144 && (b.interactive = /*interactive*/
                         h[18]), c[0] & /*show_download_button*/
-                    32768 && (m.showDownloadButton = /*show_download_button*/
+                    32768 && (b.showDownloadButton = /*show_download_button*/
                         h[15]), c[0] & /*show_share_button*/
-                    65536 && (m.showShareButton = /*show_share_button*/
+                    65536 && (b.showShareButton = /*show_share_button*/
                         h[16]), c[0] & /*show_clear_button*/
-                    131072 && (m.showClearButton = /*show_clear_button*/
+                    131072 && (b.showClearButton = /*show_clear_button*/
                         h[17]), c[0] & /*gradio*/
-                    8388608 && (m.i18n = /*gradio*/
+                    8388608 && (b.i18n = /*gradio*/
                         h[23].i18n), c[0] & /*boxes_alpha*/
-                    524288 && (m.boxesAlpha = /*boxes_alpha*/
+                    524288 && (b.boxesAlpha = /*boxes_alpha*/
                         h[19]), c[0] & /*label_list*/
-                    1048576 && (m.labelList = /*label_list*/
+                    1048576 && (b.labelList = /*label_list*/
                         h[20]), c[0] & /*label_colors*/
-                    2097152 && (m.labelColors = /*label_colors*/
+                    2097152 && (b.labelColors = /*label_colors*/
                         h[21]), c[0] & /*box_min_size*/
-                    4194304 && (m.boxMinSize = /*box_min_size*/
+                    4194304 && (b.boxMinSize = /*box_min_size*/
                         h[22]), c[0] & /*label*/
-                    32 && (m.label = /*label*/
+                    32 && (b.label = /*label*/
                         h[5]), c[0] & /*show_label*/
-                    64 && (m.show_label = /*show_label*/
+                    64 && (b.show_label = /*show_label*/
                         h[6]), c[0] & /*gradio, active_source*/
                     41943040 | c[1] & /*$$scope*/
-                    32 && (m.$$scope = {
+                    32 && (b.$$scope = {
                         dirty: c,
                         ctx: h
                     }), !l && c[0] & /*active_source*/
-                    33554432 && (l = !0, m.active_source = /*active_source*/
+                    33554432 && (l = !0, b.active_source = /*active_source*/
                         h[25], mr(() => l = !1)), !s && c[0] & /*value*/
-                    1 && (s = !0, m.value = /*value*/
-                        h[0], mr(() => s = !1)), i.$set(m);
+                    1 && (s = !0, b.value = /*value*/
+                        h[0], mr(() => s = !1)), i.$set(b);
             },
             i(h) {
                 o || ($e(e.$$.fragment, h), $e(i.$$.fragment, h), o = !0);
             },
             o(h) {
                 et(e.$$.fragment, h), et(i.$$.fragment, h), o = !1;
             },
             d(h) {
-                h && ja(n), Mt(e, h), Mt(i, h);
+                h && ja(n), Ot(e, h), Ot(i, h);
             }
         }
     );
 }
 
 function sb(t) {
     let e, n;
@@ -13966,18 +13982,18 @@
             },
             $$scope: {
                 ctx: t
             }
         }
     }), {
         c() {
-            It(e.$$.fragment);
+            Mt(e.$$.fragment);
         },
         m(i, l) {
-            Ot(e, i, l), n = !0;
+            Dt(e, i, l), n = !0;
         },
         p(i, l) {
             const s = {};
             l[0] & /*visible*/
                 16 && (s.visible = /*visible*/
                     i[4]), l[0] & /*dragging*/
                 16777216 && (s.border_mode = /*dragging*/
@@ -14005,15 +14021,15 @@
         i(i) {
             n || ($e(e.$$.fragment, i), n = !0);
         },
         o(i) {
             et(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            Mt(e, i);
+            Ot(e, i);
         }
     };
 }
 
 function ob(t, e, n) {
     let {
         elem_id: i = ""
@@ -14036,19 +14052,19 @@
     } = e, {
         _selectable: h = !1
     } = e, {
         container: c = !0
     } = e, {
         scale: d = null
     } = e, {
-        min_width: m = void 0
+        min_width: b = void 0
     } = e, {
-        loading_status: b
+        loading_status: p
     } = e, {
-        sources: p = ["upload", "clipboard"]
+        sources: g = ["upload", "clipboard"]
     } = e, {
         show_download_button: y
     } = e, {
         show_share_button: w
     } = e, {
         show_clear_button: C
     } = e, {
@@ -14061,77 +14077,77 @@
         label_colors: v
     } = e, {
         box_min_size: A
     } = e, {
         gradio: B
     } = e, L, x = null;
 
-    function J(g) {
-        x = g, n(25, x);
+    function Y(m) {
+        x = m, n(25, x);
     }
 
-    function ce(g) {
-        o = g, n(0, o);
+    function _e(m) {
+        o = m, n(0, o);
     }
     const te = () => B.dispatch("change"),
-        ke = () => B.dispatch("edit"),
-        ye = () => {
+        Ee = () => B.dispatch("edit"),
+        ve = () => {
             B.dispatch("clear");
         },
-        me = ({
-            detail: g
-        }) => n(24, L = g),
-        _e = () => B.dispatch("upload"),
+        de = ({
+            detail: m
+        }) => n(24, L = m),
+        ce = () => B.dispatch("upload"),
         S = ({
-            detail: g
-        }) => B.dispatch("select", g),
+            detail: m
+        }) => B.dispatch("select", m),
         k = ({
-            detail: g
-        }) => B.dispatch("share", g),
+            detail: m
+        }) => B.dispatch("share", m),
         I = ({
-            detail: g
+            detail: m
         }) => {
-            n(1, b = b || {}), n(1, b.status = "error", b), B.dispatch("error", g);
+            n(1, p = p || {}), n(1, p.status = "error", p), B.dispatch("error", m);
         };
-    return t.$$set = (g) => {
-        "elem_id" in g && n(2, i = g.elem_id), "elem_classes" in g && n(3, l = g.elem_classes), "visible" in g && n(4, s = g.visible), "value" in g && n(0, o = g.value), "label" in g && n(5, r = g.label), "show_label" in g && n(6, a = g.show_label), "root" in g && n(7, u = g.root), "height" in g && n(8, f = g.height), "width" in g && n(9, _ = g.width), "_selectable" in g && n(10, h = g._selectable), "container" in g && n(11, c = g.container), "scale" in g && n(12, d = g.scale), "min_width" in g && n(13, m = g.min_width), "loading_status" in g && n(1, b = g.loading_status), "sources" in g && n(14, p = g.sources), "show_download_button" in g && n(15, y = g.show_download_button), "show_share_button" in g && n(16, w = g.show_share_button), "show_clear_button" in g && n(17, C = g.show_clear_button), "interactive" in g && n(18, P = g.interactive), "boxes_alpha" in g && n(19, E = g.boxes_alpha), "label_list" in g && n(20, N = g.label_list), "label_colors" in g && n(21, v = g.label_colors), "box_min_size" in g && n(22, A = g.box_min_size), "gradio" in g && n(23, B = g.gradio);
+    return t.$$set = (m) => {
+        "elem_id" in m && n(2, i = m.elem_id), "elem_classes" in m && n(3, l = m.elem_classes), "visible" in m && n(4, s = m.visible), "value" in m && n(0, o = m.value), "label" in m && n(5, r = m.label), "show_label" in m && n(6, a = m.show_label), "root" in m && n(7, u = m.root), "height" in m && n(8, f = m.height), "width" in m && n(9, _ = m.width), "_selectable" in m && n(10, h = m._selectable), "container" in m && n(11, c = m.container), "scale" in m && n(12, d = m.scale), "min_width" in m && n(13, b = m.min_width), "loading_status" in m && n(1, p = m.loading_status), "sources" in m && n(14, g = m.sources), "show_download_button" in m && n(15, y = m.show_download_button), "show_share_button" in m && n(16, w = m.show_share_button), "show_clear_button" in m && n(17, C = m.show_clear_button), "interactive" in m && n(18, P = m.interactive), "boxes_alpha" in m && n(19, E = m.boxes_alpha), "label_list" in m && n(20, N = m.label_list), "label_colors" in m && n(21, v = m.label_colors), "box_min_size" in m && n(22, A = m.box_min_size), "gradio" in m && n(23, B = m.gradio);
     }, [
         o,
-        b,
+        p,
         i,
         l,
         s,
         r,
         a,
         u,
         f,
         _,
         h,
         c,
         d,
-        m,
-        p,
+        b,
+        g,
         y,
         w,
         C,
         P,
         E,
         N,
         v,
         A,
         B,
         L,
         x,
-        J,
-        ce,
-        te,
-        ke,
-        ye,
-        me,
+        Y,
         _e,
+        te,
+        Ee,
+        ve,
+        de,
+        ce,
         S,
         k,
         I
     ];
 }
 class db extends Gg {
     constructor(e) {
```

### Comparing `gradio_image_annotation-0.0.4/backend/gradio_image_annotation/templates/component/style.css` & `gradio_image_annotation-0.0.5/backend/gradio_image_annotation/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/backend/gradio_image_annotation/templates/component/wrapper-6f348d45-f837cf34.js` & `gradio_image_annotation-0.0.5/backend/gradio_image_annotation/templates/component/wrapper-6f348d45-19fa94bf.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -915,15 +915,15 @@
     getPayloadLength64() {
         if (this._bufferedBytes < 8) {
             this._loop = !1;
             return;
         }
         const e = this.consume(8),
             t = e.readUInt32BE(0);
-        return t > Math.pow(2, 53 - 32) - 1 ? (this._loop = !1, g(
+        return t > Math.pow(2, 21) - 1 ? (this._loop = !1, g(
             RangeError,
             "Unsupported WebSocket frame: payload length > 2^53 - 1",
             !1,
             1009,
             "WS_ERR_UNSUPPORTED_DATA_PAYLOAD_LENGTH"
         )) : (this._payloadLength = t * Math.pow(2, 32) + e.readUInt32BE(4), this.haveLength());
     }
@@ -1857,16 +1857,15 @@
      * @param {(String|Buffer)} [data] The reason why the connection is
      *     closing
      * @public
      */
     close(e, t) {
         if (this.readyState !== d.CLOSED) {
             if (this.readyState === d.CONNECTING) {
-                const r = "WebSocket was closed before the connection was established";
-                b(this, this._req, r);
+                b(this, this._req, "WebSocket was closed before the connection was established");
                 return;
             }
             if (this.readyState === d.CLOSING) {
                 this._closeFrameSent && (this._closeFrameReceived || this._receiver._writableState.errorEmitted) && this._socket.end();
                 return;
             }
             this._readyState = d.CLOSING, this._sender.close(e, t, !this._isServer, (r) => {
@@ -1962,16 +1961,15 @@
      * Forcibly close the connection.
      *
      * @public
      */
     terminate() {
         if (this.readyState !== d.CLOSED) {
             if (this.readyState === d.CONNECTING) {
-                const e = "WebSocket was closed before the connection was established";
-                b(this, this._req, e);
+                b(this, this._req, "WebSocket was closed before the connection was established");
                 return;
             }
             this._socket && (this._readyState = d.CLOSING, this._socket.destroy());
         }
     }
 };
 Object.defineProperty(m, "CONNECTING", {
```

### Comparing `gradio_image_annotation-0.0.4/backend/gradio_image_annotation/templates/example/index.js` & `gradio_image_annotation-0.0.5/backend/gradio_image_annotation/templates/example/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,466 +1,466 @@
 const {
-    setContext: yu,
-    getContext: er
-} = window.__gradio__svelte__internal, tr = "WORKER_PROXY_CONTEXT_KEY";
+    setContext: Su,
+    getContext: rr
+} = window.__gradio__svelte__internal, sr = "WORKER_PROXY_CONTEXT_KEY";
 
-function nr() {
-    return er(tr);
+function or() {
+    return rr(sr);
 }
 
-function ir(e) {
+function ar(e) {
     return e.host === window.location.host || e.host === "localhost:7860" || e.host === "127.0.0.1:7860" || // Ref: https://github.com/gradio-app/gradio/blob/v3.32.0/js/app/src/Index.svelte#L194
         e.host === "lite.local";
 }
 
-function rr(e, t) {
+function lr(e, t) {
     const n = t.toLowerCase();
     for (const [i, r] of Object.entries(e))
         if (i.toLowerCase() === n)
             return r;
 }
 
-function sr(e) {
+function ur(e) {
     if (e == null)
         return !1;
     const t = new URL(e);
-    return !(!ir(t) || t.protocol !== "http:" && t.protocol !== "https:");
+    return !(!ar(t) || t.protocol !== "http:" && t.protocol !== "https:");
 }
-async function or(e) {
-    if (e == null || !sr(e))
+async function fr(e) {
+    if (e == null || !ur(e))
         return e;
-    const t = nr();
+    const t = or();
     if (t == null)
         return e;
     const i = new URL(e).pathname;
     return t.httpRequest({
         method: "GET",
         path: i,
         headers: {},
         query_string: ""
     }).then((r) => {
         if (r.status !== 200)
             throw new Error(`Failed to get file ${i} from the Wasm worker.`);
         const s = new Blob([r.body], {
-            type: rr(r.headers, "content-type")
+            type: lr(r.headers, "content-type")
         });
         return URL.createObjectURL(s);
     });
 }
 const {
-    SvelteComponent: ar,
+    SvelteComponent: hr,
     append: Tt,
     attr: X,
-    detach: lr,
-    init: ur,
-    insert: fr,
-    noop: Ct,
-    safe_not_equal: hr,
+    detach: cr,
+    init: mr,
+    insert: _r,
+    noop: Pt,
+    safe_not_equal: dr,
     set_style: Z,
-    svg_element: Ze
+    svg_element: Je
 } = window.__gradio__svelte__internal;
 
-function cr(e) {
+function br(e) {
     let t, n, i, r;
     return {
         c() {
-            t = Ze("svg"), n = Ze("g"), i = Ze("path"), r = Ze("path"), X(i, "d", "M18,6L6.087,17.913"), Z(i, "fill", "none"), Z(i, "fill-rule", "nonzero"), Z(i, "stroke-width", "2px"), X(n, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), X(r, "d", "M4.364,4.364L19.636,19.636"), Z(r, "fill", "none"), Z(r, "fill-rule", "nonzero"), Z(r, "stroke-width", "2px"), X(t, "width", "100%"), X(t, "height", "100%"), X(t, "viewBox", "0 0 24 24"), X(t, "version", "1.1"), X(t, "xmlns", "http://www.w3.org/2000/svg"), X(t, "xmlns:xlink", "http://www.w3.org/1999/xlink"), X(t, "xml:space", "preserve"), X(t, "stroke", "currentColor"), Z(t, "fill-rule", "evenodd"), Z(t, "clip-rule", "evenodd"), Z(t, "stroke-linecap", "round"), Z(t, "stroke-linejoin", "round");
+            t = Je("svg"), n = Je("g"), i = Je("path"), r = Je("path"), X(i, "d", "M18,6L6.087,17.913"), Z(i, "fill", "none"), Z(i, "fill-rule", "nonzero"), Z(i, "stroke-width", "2px"), X(n, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), X(r, "d", "M4.364,4.364L19.636,19.636"), Z(r, "fill", "none"), Z(r, "fill-rule", "nonzero"), Z(r, "stroke-width", "2px"), X(t, "width", "100%"), X(t, "height", "100%"), X(t, "viewBox", "0 0 24 24"), X(t, "version", "1.1"), X(t, "xmlns", "http://www.w3.org/2000/svg"), X(t, "xmlns:xlink", "http://www.w3.org/1999/xlink"), X(t, "xml:space", "preserve"), X(t, "stroke", "currentColor"), Z(t, "fill-rule", "evenodd"), Z(t, "clip-rule", "evenodd"), Z(t, "stroke-linecap", "round"), Z(t, "stroke-linejoin", "round");
         },
         m(s, u) {
-            fr(s, t, u), Tt(t, n), Tt(n, i), Tt(t, r);
+            _r(s, t, u), Tt(t, n), Tt(n, i), Tt(t, r);
         },
-        p: Ct,
-        i: Ct,
-        o: Ct,
+        p: Pt,
+        i: Pt,
+        o: Pt,
         d(s) {
-            s && lr(t);
+            s && cr(t);
         }
     };
 }
-class mr extends ar {
+class gr extends hr {
     constructor(t) {
-        super(), ur(this, t, null, cr, hr, {});
+        super(), mr(this, t, null, br, dr, {});
     }
 }
 const {
-    SvelteComponent: _r,
-    append: dr,
-    attr: fe,
-    detach: br,
-    init: gr,
-    insert: pr,
-    noop: Pt,
-    safe_not_equal: vr,
+    SvelteComponent: pr,
+    append: vr,
+    attr: he,
+    detach: yr,
+    init: Er,
+    insert: wr,
+    noop: It,
+    safe_not_equal: xr,
     svg_element: En
 } = window.__gradio__svelte__internal;
 
-function yr(e) {
+function Sr(e) {
     let t, n;
     return {
         c() {
-            t = En("svg"), n = En("path"), fe(n, "d", "M5 8l4 4 4-4z"), fe(t, "class", "dropdown-arrow svelte-145leq6"), fe(t, "xmlns", "http://www.w3.org/2000/svg"), fe(t, "width", "100%"), fe(t, "height", "100%"), fe(t, "viewBox", "0 0 18 18");
+            t = En("svg"), n = En("path"), he(n, "d", "M5 8l4 4 4-4z"), he(t, "class", "dropdown-arrow svelte-145leq6"), he(t, "xmlns", "http://www.w3.org/2000/svg"), he(t, "width", "100%"), he(t, "height", "100%"), he(t, "viewBox", "0 0 18 18");
         },
         m(i, r) {
-            pr(i, t, r), dr(t, n);
+            wr(i, t, r), vr(t, n);
         },
-        p: Pt,
-        i: Pt,
-        o: Pt,
+        p: It,
+        i: It,
+        o: It,
         d(i) {
-            i && br(t);
+            i && yr(t);
         }
     };
 }
-class Er extends _r {
+class Hr extends pr {
     constructor(t) {
-        super(), gr(this, t, null, yr, vr, {});
+        super(), Er(this, t, null, Sr, xr, {});
     }
 }
 const {
-    SvelteComponent: wr,
-    append: xr,
+    SvelteComponent: Ar,
+    append: Br,
     attr: V,
-    detach: Sr,
-    init: Hr,
-    insert: Ar,
-    noop: It,
-    safe_not_equal: Br,
+    detach: Cr,
+    init: Tr,
+    insert: Pr,
+    noop: Nt,
+    safe_not_equal: Ir,
     svg_element: wn
 } = window.__gradio__svelte__internal;
 
-function Tr(e) {
+function Nr(e) {
     let t, n;
     return {
         c() {
             t = wn("svg"), n = wn("path"), V(n, "d", "M17 3a2.828 2.828 0 1 1 4 4L7.5 20.5 2 22l1.5-5.5L17 3z"), V(t, "xmlns", "http://www.w3.org/2000/svg"), V(t, "width", "100%"), V(t, "height", "100%"), V(t, "viewBox", "0 0 24 24"), V(t, "fill", "none"), V(t, "stroke", "currentColor"), V(t, "stroke-width", "1.5"), V(t, "stroke-linecap", "round"), V(t, "stroke-linejoin", "round"), V(t, "class", "feather feather-edit-2");
         },
         m(i, r) {
-            Ar(i, t, r), xr(t, n);
+            Pr(i, t, r), Br(t, n);
         },
-        p: It,
-        i: It,
-        o: It,
+        p: Nt,
+        i: Nt,
+        o: Nt,
         d(i) {
-            i && Sr(t);
+            i && Cr(t);
         }
     };
 }
-class Cr extends wr {
+class Or extends Ar {
     constructor(t) {
-        super(), Hr(this, t, null, Tr, Br, {});
+        super(), Tr(this, t, null, Nr, Ir, {});
     }
 }
 const {
-    SvelteComponent: Pr,
+    SvelteComponent: Lr,
     append: xn,
     attr: D,
-    detach: Ir,
-    init: Nr,
-    insert: Or,
-    noop: Nt,
-    safe_not_equal: Mr,
+    detach: Mr,
+    init: Rr,
+    insert: kr,
+    noop: Ot,
+    safe_not_equal: Dr,
     set_style: ne,
-    svg_element: Ot
+    svg_element: Lt
 } = window.__gradio__svelte__internal;
 
-function Lr(e) {
+function Ur(e) {
     let t, n, i;
     return {
         c() {
-            t = Ot("svg"), n = Ot("line"), i = Ot("line"), D(n, "x1", "4"), D(n, "y1", "12"), D(n, "x2", "20"), D(n, "y2", "12"), ne(n, "fill", "none"), ne(n, "stroke-width", "2px"), D(i, "x1", "12"), D(i, "y1", "4"), D(i, "x2", "12"), D(i, "y2", "20"), ne(i, "fill", "none"), ne(i, "stroke-width", "2px"), D(t, "width", "100%"), D(t, "height", "100%"), D(t, "viewBox", "0 0 24 24"), D(t, "version", "1.1"), D(t, "xmlns", "http://www.w3.org/2000/svg"), D(t, "xmlns:xlink", "http://www.w3.org/1999/xlink"), D(t, "xml:space", "preserve"), D(t, "stroke", "currentColor"), ne(t, "fill-rule", "evenodd"), ne(t, "clip-rule", "evenodd"), ne(t, "stroke-linecap", "round"), ne(t, "stroke-linejoin", "round");
+            t = Lt("svg"), n = Lt("line"), i = Lt("line"), D(n, "x1", "4"), D(n, "y1", "12"), D(n, "x2", "20"), D(n, "y2", "12"), ne(n, "fill", "none"), ne(n, "stroke-width", "2px"), D(i, "x1", "12"), D(i, "y1", "4"), D(i, "x2", "12"), D(i, "y2", "20"), ne(i, "fill", "none"), ne(i, "stroke-width", "2px"), D(t, "width", "100%"), D(t, "height", "100%"), D(t, "viewBox", "0 0 24 24"), D(t, "version", "1.1"), D(t, "xmlns", "http://www.w3.org/2000/svg"), D(t, "xmlns:xlink", "http://www.w3.org/1999/xlink"), D(t, "xml:space", "preserve"), D(t, "stroke", "currentColor"), ne(t, "fill-rule", "evenodd"), ne(t, "clip-rule", "evenodd"), ne(t, "stroke-linecap", "round"), ne(t, "stroke-linejoin", "round");
         },
         m(r, s) {
-            Or(r, t, s), xn(t, n), xn(t, i);
+            kr(r, t, s), xn(t, n), xn(t, i);
         },
-        p: Nt,
-        i: Nt,
-        o: Nt,
+        p: Ot,
+        i: Ot,
+        o: Ot,
         d(r) {
-            r && Ir(t);
+            r && Mr(t);
         }
     };
 }
-class Rr extends Pr {
+class Gr extends Lr {
     constructor(t) {
-        super(), Nr(this, t, null, Lr, Mr, {});
+        super(), Rr(this, t, null, Ur, Dr, {});
     }
 }
 const {
-    SvelteComponent: kr,
-    attr: Dr,
-    create_slot: Ur,
-    detach: Gr,
-    element: Fr,
-    get_all_dirty_from_scope: zr,
-    get_slot_changes: jr,
-    init: Xr,
-    insert: Vr,
-    safe_not_equal: qr,
-    transition_in: Wr,
-    transition_out: Yr,
-    update_slot_base: Zr
+    SvelteComponent: Fr,
+    attr: zr,
+    create_slot: jr,
+    detach: Xr,
+    element: Vr,
+    get_all_dirty_from_scope: qr,
+    get_slot_changes: Wr,
+    init: Yr,
+    insert: Zr,
+    safe_not_equal: Qr,
+    transition_in: Jr,
+    transition_out: Kr,
+    update_slot_base: $r
 } = window.__gradio__svelte__internal;
 
-function Qr(e) {
+function es(e) {
     let t, n;
     const i = (
             /*#slots*/
             e[1].default
         ),
-        r = Ur(
+        r = jr(
             i,
             e,
             /*$$scope*/
             e[0],
             null
         );
     return {
         c() {
-            t = Fr("div"), r && r.c(), Dr(t, "class", "svelte-1hnfib2");
+            t = Vr("div"), r && r.c(), zr(t, "class", "svelte-1hnfib2");
         },
         m(s, u) {
-            Vr(s, t, u), r && r.m(t, null), n = !0;
+            Zr(s, t, u), r && r.m(t, null), n = !0;
         },
         p(s, [u]) {
             r && r.p && (!n || u & /*$$scope*/
-                1) && Zr(
+                1) && $r(
                 r,
                 i,
                 s,
                 /*$$scope*/
                 s[0],
-                n ? jr(
+                n ? Wr(
                     i,
                     /*$$scope*/
                     s[0],
                     u,
                     null
-                ) : zr(
+                ) : qr(
                     /*$$scope*/
                     s[0]
                 ),
                 null
             );
         },
         i(s) {
-            n || (Wr(r, s), n = !0);
+            n || (Jr(r, s), n = !0);
         },
         o(s) {
-            Yr(r, s), n = !1;
+            Kr(r, s), n = !1;
         },
         d(s) {
-            s && Gr(t), r && r.d(s);
+            s && Xr(t), r && r.d(s);
         }
     };
 }
 
-function Jr(e, t, n) {
+function ts(e, t, n) {
     let {
         $$slots: i = {},
         $$scope: r
     } = t;
     return e.$$set = (s) => {
         "$$scope" in s && n(0, r = s.$$scope);
     }, [r, i];
 }
-class Kr extends kr {
+class ns extends Fr {
     constructor(t) {
-        super(), Xr(this, t, Jr, Qr, qr, {});
+        super(), Yr(this, t, ts, es, Qr, {});
     }
 }
 const {
-    SvelteComponent: $r,
+    SvelteComponent: is,
     attr: Sn,
-    check_outros: es,
-    create_component: ts,
-    create_slot: ns,
-    destroy_component: is,
-    detach: ot,
-    element: rs,
-    empty: ss,
-    get_all_dirty_from_scope: os,
-    get_slot_changes: as,
-    group_outros: ls,
-    init: us,
-    insert: at,
-    mount_component: fs,
-    safe_not_equal: hs,
-    set_data: cs,
-    space: ms,
-    text: _s,
-    toggle_class: he,
-    transition_in: Me,
-    transition_out: lt,
-    update_slot_base: ds
+    check_outros: rs,
+    create_component: ss,
+    create_slot: os,
+    destroy_component: as,
+    detach: lt,
+    element: ls,
+    empty: us,
+    get_all_dirty_from_scope: fs,
+    get_slot_changes: hs,
+    group_outros: cs,
+    init: ms,
+    insert: ut,
+    mount_component: _s,
+    safe_not_equal: ds,
+    set_data: bs,
+    space: gs,
+    text: ps,
+    toggle_class: ce,
+    transition_in: Le,
+    transition_out: ft,
+    update_slot_base: vs
 } = window.__gradio__svelte__internal;
 
 function Hn(e) {
     let t, n;
-    return t = new Kr({
+    return t = new ns({
         props: {
             $$slots: {
-                default: [bs]
+                default: [ys]
             },
             $$scope: {
                 ctx: e
             }
         }
     }), {
         c() {
-            ts(t.$$.fragment);
+            ss(t.$$.fragment);
         },
         m(i, r) {
-            fs(t, i, r), n = !0;
+            _s(t, i, r), n = !0;
         },
         p(i, r) {
             const s = {};
             r & /*$$scope, info*/
                 10 && (s.$$scope = {
                     dirty: r,
                     ctx: i
                 }), t.$set(s);
         },
         i(i) {
-            n || (Me(t.$$.fragment, i), n = !0);
+            n || (Le(t.$$.fragment, i), n = !0);
         },
         o(i) {
-            lt(t.$$.fragment, i), n = !1;
+            ft(t.$$.fragment, i), n = !1;
         },
         d(i) {
-            is(t, i);
+            as(t, i);
         }
     };
 }
 
-function bs(e) {
+function ys(e) {
     let t;
     return {
         c() {
-            t = _s(
+            t = ps(
                 /*info*/
                 e[1]
             );
         },
         m(n, i) {
-            at(n, t, i);
+            ut(n, t, i);
         },
         p(n, i) {
             i & /*info*/
-                2 && cs(
+                2 && bs(
                     t,
                     /*info*/
                     n[1]
                 );
         },
         d(n) {
-            n && ot(t);
+            n && lt(t);
         }
     };
 }
 
-function gs(e) {
+function Es(e) {
     let t, n, i, r;
     const s = (
             /*#slots*/
             e[2].default
         ),
-        u = ns(
+        u = os(
             s,
             e,
             /*$$scope*/
             e[3],
             null
         );
     let o = (
         /*info*/
         e[1] && Hn(e)
     );
     return {
         c() {
-            t = rs("span"), u && u.c(), n = ms(), o && o.c(), i = ss(), Sn(t, "data-testid", "block-info"), Sn(t, "class", "svelte-22c38v"), he(t, "sr-only", ! /*show_label*/
-                e[0]), he(t, "hide", ! /*show_label*/
-                e[0]), he(
+            t = ls("span"), u && u.c(), n = gs(), o && o.c(), i = us(), Sn(t, "data-testid", "block-info"), Sn(t, "class", "svelte-22c38v"), ce(t, "sr-only", ! /*show_label*/
+                e[0]), ce(t, "hide", ! /*show_label*/
+                e[0]), ce(
                 t,
                 "has-info",
                 /*info*/
                 e[1] != null
             );
         },
         m(a, f) {
-            at(a, t, f), u && u.m(t, null), at(a, n, f), o && o.m(a, f), at(a, i, f), r = !0;
+            ut(a, t, f), u && u.m(t, null), ut(a, n, f), o && o.m(a, f), ut(a, i, f), r = !0;
         },
         p(a, [f]) {
             u && u.p && (!r || f & /*$$scope*/
-                    8) && ds(
+                    8) && vs(
                     u,
                     s,
                     a,
                     /*$$scope*/
                     a[3],
-                    r ? as(
+                    r ? hs(
                         s,
                         /*$$scope*/
                         a[3],
                         f,
                         null
-                    ) : os(
+                    ) : fs(
                         /*$$scope*/
                         a[3]
                     ),
                     null
                 ), (!r || f & /*show_label*/
-                    1) && he(t, "sr-only", ! /*show_label*/
+                    1) && ce(t, "sr-only", ! /*show_label*/
                     a[0]), (!r || f & /*show_label*/
-                    1) && he(t, "hide", ! /*show_label*/
+                    1) && ce(t, "hide", ! /*show_label*/
                     a[0]), (!r || f & /*info*/
-                    2) && he(
+                    2) && ce(
                     t,
                     "has-info",
                     /*info*/
                     a[1] != null
                 ), /*info*/
                 a[1] ? o ? (o.p(a, f), f & /*info*/
-                    2 && Me(o, 1)) : (o = Hn(a), o.c(), Me(o, 1), o.m(i.parentNode, i)) : o && (ls(), lt(o, 1, 1, () => {
+                    2 && Le(o, 1)) : (o = Hn(a), o.c(), Le(o, 1), o.m(i.parentNode, i)) : o && (cs(), ft(o, 1, 1, () => {
                     o = null;
-                }), es());
+                }), rs());
         },
         i(a) {
-            r || (Me(u, a), Me(o), r = !0);
+            r || (Le(u, a), Le(o), r = !0);
         },
         o(a) {
-            lt(u, a), lt(o), r = !1;
+            ft(u, a), ft(o), r = !1;
         },
         d(a) {
-            a && (ot(t), ot(n), ot(i)), u && u.d(a), o && o.d(a);
+            a && (lt(t), lt(n), lt(i)), u && u.d(a), o && o.d(a);
         }
     };
 }
 
-function ps(e, t, n) {
+function ws(e, t, n) {
     let {
         $$slots: i = {},
         $$scope: r
     } = t, {
         show_label: s = !0
     } = t, {
         info: u = void 0
     } = t;
     return e.$$set = (o) => {
         "show_label" in o && n(0, s = o.show_label), "info" in o && n(1, u = o.info), "$$scope" in o && n(3, r = o.$$scope);
     }, [s, u, i, r];
 }
-class hi extends $r {
+class hi extends is {
     constructor(t) {
-        super(), us(this, t, ps, gs, hs, {
+        super(), ms(this, t, ws, Es, ds, {
             show_label: 0,
             info: 1
         });
     }
 }
-const vs = [{
+const xs = [{
         color: "red",
         primary: 600,
         secondary: 100
     }, {
         color: "green",
         primary: 600,
         secondary: 100
@@ -786,122 +786,122 @@
             600: "#e11d48",
             700: "#be123c",
             800: "#9f1239",
             900: "#881337",
             950: "#4c0519"
         }
     };
-vs.reduce(
+xs.reduce(
     (e, {
         color: t,
         primary: n,
         secondary: i
     }) => ({
         ...e,
         [t]: {
             primary: An[t][n],
             secondary: An[t][i]
         }
     }), {}
 );
 const {
-    SvelteComponent: ys,
+    SvelteComponent: Ss,
     append: Bn,
     attr: Mt,
-    bubble: Tn,
-    create_component: Es,
-    destroy_component: ws,
+    bubble: Cn,
+    create_component: Hs,
+    destroy_component: As,
     detach: ci,
-    element: Cn,
-    init: xs,
+    element: Tn,
+    init: Bs,
     insert: mi,
-    listen: Lt,
-    mount_component: Ss,
-    run_all: Hs,
-    safe_not_equal: As,
-    set_data: Bs,
+    listen: Rt,
+    mount_component: Cs,
+    run_all: Ts,
+    safe_not_equal: Ps,
+    set_data: Is,
     set_input_value: Pn,
-    space: Ts,
-    text: Cs,
-    transition_in: Ps,
-    transition_out: Is
+    space: Ns,
+    text: Os,
+    transition_in: Ls,
+    transition_out: Ms
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: Ns,
-    afterUpdate: Os
+    createEventDispatcher: Rs,
+    afterUpdate: ks
 } = window.__gradio__svelte__internal;
 
-function Ms(e) {
+function Ds(e) {
     let t;
     return {
         c() {
-            t = Cs(
+            t = Os(
                 /*label*/
                 e[1]
             );
         },
         m(n, i) {
             mi(n, t, i);
         },
         p(n, i) {
             i & /*label*/
-                2 && Bs(
+                2 && Is(
                     t,
                     /*label*/
                     n[1]
                 );
         },
         d(n) {
             n && ci(t);
         }
     };
 }
 
-function Ls(e) {
+function Us(e) {
     let t, n, i, r, s, u, o;
     return n = new hi({
         props: {
             show_label: (
                 /*show_label*/
                 e[4]
             ),
             info: (
                 /*info*/
                 e[2]
             ),
             $$slots: {
-                default: [Ms]
+                default: [Ds]
             },
             $$scope: {
                 ctx: e
             }
         }
     }), {
         c() {
-            t = Cn("label"), Es(n.$$.fragment), i = Ts(), r = Cn("input"), Mt(r, "type", "color"), r.disabled = /*disabled*/
+            t = Tn("label"), Hs(n.$$.fragment), i = Ns(), r = Tn("input"), Mt(r, "type", "color"), r.disabled = /*disabled*/
                 e[3], Mt(r, "class", "svelte-16l8u73"), Mt(t, "class", "block");
         },
         m(a, f) {
-            mi(a, t, f), Ss(n, t, null), Bn(t, i), Bn(t, r), Pn(
+            mi(a, t, f), Cs(n, t, null), Bn(t, i), Bn(t, r), Pn(
                 r,
                 /*value*/
                 e[0]
             ), s = !0, u || (o = [
-                Lt(
+                Rt(
                     r,
                     "input",
                     /*input_input_handler*/
                     e[8]
                 ),
-                Lt(
+                Rt(
                     r,
                     "focus",
                     /*focus_handler*/
                     e[6]
                 ),
-                Lt(
+                Rt(
                     r,
                     "blur",
                     /*blur_handler*/
                     e[7]
                 )
             ], u = !0);
         },
@@ -921,261 +921,261 @@
                 1 && Pn(
                     r,
                     /*value*/
                     a[0]
                 );
         },
         i(a) {
-            s || (Ps(n.$$.fragment, a), s = !0);
+            s || (Ls(n.$$.fragment, a), s = !0);
         },
         o(a) {
-            Is(n.$$.fragment, a), s = !1;
+            Ms(n.$$.fragment, a), s = !1;
         },
         d(a) {
-            a && ci(t), ws(n), u = !1, Hs(o);
+            a && ci(t), As(n), u = !1, Ts(o);
         }
     };
 }
 
-function Rs(e, t, n) {
+function Gs(e, t, n) {
     let {
         value: i = "#000000"
     } = t, {
         value_is_output: r = !1
     } = t, {
         label: s
     } = t, {
         info: u = void 0
     } = t, {
         disabled: o = !1
     } = t, {
         show_label: a = !0
     } = t;
-    const f = Ns();
+    const f = Rs();
 
     function l() {
         f("change", i), r || f("input");
     }
-    Os(() => {
+    ks(() => {
         n(5, r = !1);
     });
 
-    function h(g) {
-        Tn.call(this, e, g);
+    function h(b) {
+        Cn.call(this, e, b);
     }
 
-    function c(g) {
-        Tn.call(this, e, g);
+    function m(b) {
+        Cn.call(this, e, b);
     }
 
     function _() {
         i = this.value, n(0, i);
     }
-    return e.$$set = (g) => {
-        "value" in g && n(0, i = g.value), "value_is_output" in g && n(5, r = g.value_is_output), "label" in g && n(1, s = g.label), "info" in g && n(2, u = g.info), "disabled" in g && n(3, o = g.disabled), "show_label" in g && n(4, a = g.show_label);
+    return e.$$set = (b) => {
+        "value" in b && n(0, i = b.value), "value_is_output" in b && n(5, r = b.value_is_output), "label" in b && n(1, s = b.label), "info" in b && n(2, u = b.info), "disabled" in b && n(3, o = b.disabled), "show_label" in b && n(4, a = b.show_label);
     }, e.$$.update = () => {
         e.$$.dirty & /*value*/
             1 && l();
     }, [
         i,
         s,
         u,
         o,
         a,
         r,
         h,
-        c,
+        m,
         _
     ];
 }
-class ks extends ys {
+class Fs extends Ss {
     constructor(t) {
-        super(), xs(this, t, Rs, Ls, As, {
+        super(), Bs(this, t, Gs, Us, Ps, {
             value: 0,
             value_is_output: 5,
             label: 1,
             info: 2,
             disabled: 3,
             show_label: 4
         });
     }
 }
 
-function we() {}
+function xe() {}
 
-function Ds(e) {
+function zs(e) {
     return e();
 }
 
-function Us(e) {
-    e.forEach(Ds);
+function js(e) {
+    e.forEach(zs);
 }
 
-function Gs(e) {
+function Xs(e) {
     return typeof e == "function";
 }
 
-function Fs(e, t) {
+function Vs(e, t) {
     return e != e ? t == t : e !== t || e && typeof e == "object" || typeof e == "function";
 }
 
-function zs(e, ...t) {
+function qs(e, ...t) {
     if (e == null) {
         for (const i of t)
             i(void 0);
-        return we;
+        return xe;
     }
     const n = e.subscribe(...t);
     return n.unsubscribe ? () => n.unsubscribe() : n;
 }
 
 function In(e) {
     const t = typeof e == "string" && e.match(/^\s*(-?[\d.]+)([^\s]*)\s*$/);
     return t ? [parseFloat(t[1]), t[2] || "px"] : [
         /** @type {number} */
         e,
         "px"
     ];
 }
 
-function js(e) {
+function Ws(e) {
     const t = e - 1;
     return t * t * t + 1;
 }
 
 function Nn(e, {
     delay: t = 0,
     duration: n = 400,
-    easing: i = js,
+    easing: i = Ws,
     x: r = 0,
     y: s = 0,
     opacity: u = 0
 } = {}) {
     const o = getComputedStyle(e),
         a = +o.opacity,
         f = o.transform === "none" ? "" : o.transform,
         l = a * (1 - u),
-        [h, c] = In(r),
-        [_, g] = In(s);
+        [h, m] = In(r),
+        [_, b] = In(s);
     return {
         delay: t,
         duration: n,
         easing: i,
-        css: (m, d) => `
-			transform: ${f} translate(${(1 - m) * h}${c}, ${(1 - m) * _}${g});
+        css: (g, d) => `
+			transform: ${f} translate(${(1 - g) * h}${m}, ${(1 - g) * _}${b});
 			opacity: ${a - l * d}`
     };
 }
-const ce = [];
+const me = [];
 
-function Xs(e, t) {
+function Ys(e, t) {
     return {
-        subscribe: pt(e, t).subscribe
+        subscribe: yt(e, t).subscribe
     };
 }
 
-function pt(e, t = we) {
+function yt(e, t = xe) {
     let n;
     const i = /* @__PURE__ */ new Set();
 
     function r(o) {
-        if (Fs(e, o) && (e = o, n)) {
-            const a = !ce.length;
+        if (Vs(e, o) && (e = o, n)) {
+            const a = !me.length;
             for (const f of i)
-                f[1](), ce.push(f, e);
+                f[1](), me.push(f, e);
             if (a) {
-                for (let f = 0; f < ce.length; f += 2)
-                    ce[f][0](ce[f + 1]);
-                ce.length = 0;
+                for (let f = 0; f < me.length; f += 2)
+                    me[f][0](me[f + 1]);
+                me.length = 0;
             }
         }
     }
 
     function s(o) {
         r(o(e));
     }
 
-    function u(o, a = we) {
+    function u(o, a = xe) {
         const f = [o, a];
-        return i.add(f), i.size === 1 && (n = t(r, s) || we), o(e), () => {
+        return i.add(f), i.size === 1 && (n = t(r, s) || xe), o(e), () => {
             i.delete(f), i.size === 0 && n && (n(), n = null);
         };
     }
     return {
         set: r,
         update: s,
         subscribe: u
     };
 }
 
-function Be(e, t, n) {
+function Ce(e, t, n) {
     const i = !Array.isArray(e),
         r = i ? [e] : e;
     if (!r.every(Boolean))
         throw new Error("derived() expects stores as input, got a falsy value");
     const s = t.length < 2;
-    return Xs(n, (u, o) => {
+    return Ys(n, (u, o) => {
         let a = !1;
         const f = [];
         let l = 0,
-            h = we;
-        const c = () => {
+            h = xe;
+        const m = () => {
                 if (l)
                     return;
                 h();
-                const g = t(i ? f[0] : f, u, o);
-                s ? u(g) : h = Gs(g) ? g : we;
+                const b = t(i ? f[0] : f, u, o);
+                s ? u(b) : h = Xs(b) ? b : xe;
             },
             _ = r.map(
-                (g, m) => zs(
-                    g,
+                (b, g) => qs(
+                    b,
                     (d) => {
-                        f[m] = d, l &= ~(1 << m), a && c();
+                        f[g] = d, l &= ~(1 << g), a && m();
                     },
                     () => {
-                        l |= 1 << m;
+                        l |= 1 << g;
                     }
                 )
             );
-        return a = !0, c(),
+        return a = !0, m(),
             function() {
-                Us(_), h(), a = !1;
+                js(_), h(), a = !1;
             };
     });
 }
 new Intl.Collator(0, {
     numeric: 1
 }).compare;
 const {
-    SvelteComponent: Vs,
+    SvelteComponent: Zs,
     append: _i,
     attr: N,
-    bubble: qs,
-    check_outros: Ws,
+    bubble: Qs,
+    check_outros: Js,
     create_slot: di,
     detach: Ve,
-    element: vt,
-    empty: Ys,
+    element: Et,
+    empty: Ks,
     get_all_dirty_from_scope: bi,
     get_slot_changes: gi,
-    group_outros: Zs,
-    init: Qs,
+    group_outros: $s,
+    init: eo,
     insert: qe,
-    listen: Js,
-    safe_not_equal: Ks,
+    listen: to,
+    safe_not_equal: no,
     set_style: F,
     space: pi,
-    src_url_equal: ct,
-    toggle_class: ye,
-    transition_in: mt,
-    transition_out: _t,
+    src_url_equal: _t,
+    toggle_class: Ee,
+    transition_in: dt,
+    transition_out: bt,
     update_slot_base: vi
 } = window.__gradio__svelte__internal;
 
-function $s(e) {
+function io(e) {
     let t, n, i, r, s, u, o = (
         /*icon*/
         e[7] && On(e)
     );
     const a = (
             /*#slots*/
             e[12].default
@@ -1185,39 +1185,39 @@
             e,
             /*$$scope*/
             e[11],
             null
         );
     return {
         c() {
-            t = vt("button"), o && o.c(), n = pi(), f && f.c(), N(t, "class", i = /*size*/
+            t = Et("button"), o && o.c(), n = pi(), f && f.c(), N(t, "class", i = /*size*/
                     e[4] + " " + /*variant*/
                     e[3] + " " + /*elem_classes*/
                     e[1].join(" ") + " svelte-8huxfn"), N(
                     t,
                     "id",
                     /*elem_id*/
                     e[0]
                 ), t.disabled = /*disabled*/
-                e[8], ye(t, "hidden", ! /*visible*/
+                e[8], Ee(t, "hidden", ! /*visible*/
                     e[2]), F(
                     t,
                     "flex-grow",
                     /*scale*/
                     e[9]
                 ), F(
                     t,
                     "width",
                     /*scale*/
                     e[9] === 0 ? "fit-content" : null
                 ), F(t, "min-width", typeof /*min_width*/ e[10] == "number" ? `calc(min(${/*min_width*/
       e[10]}px, 100%))` : null);
         },
         m(l, h) {
-            qe(l, t, h), o && o.m(t, null), _i(t, n), f && f.m(t, null), r = !0, s || (u = Js(
+            qe(l, t, h), o && o.m(t, null), _i(t, n), f && f.m(t, null), r = !0, s || (u = to(
                 t,
                 "click",
                 /*click_handler*/
                 e[13]
             ), s = !0);
         },
         p(l, h) {
@@ -1249,15 +1249,15 @@
                     t,
                     "id",
                     /*elem_id*/
                     l[0]
                 ), (!r || h & /*disabled*/
                     256) && (t.disabled = /*disabled*/
                     l[8]), (!r || h & /*size, variant, elem_classes, visible*/
-                    30) && ye(t, "hidden", ! /*visible*/
+                    30) && Ee(t, "hidden", ! /*visible*/
                     l[2]), h & /*scale*/
                 512 && F(
                     t,
                     "flex-grow",
                     /*scale*/
                     l[9]
                 ), h & /*scale*/
@@ -1267,44 +1267,44 @@
                     /*scale*/
                     l[9] === 0 ? "fit-content" : null
                 ), h & /*min_width*/
                 1024 && F(t, "min-width", typeof /*min_width*/ l[10] == "number" ? `calc(min(${/*min_width*/
       l[10]}px, 100%))` : null);
         },
         i(l) {
-            r || (mt(f, l), r = !0);
+            r || (dt(f, l), r = !0);
         },
         o(l) {
-            _t(f, l), r = !1;
+            bt(f, l), r = !1;
         },
         d(l) {
             l && Ve(t), o && o.d(), f && f.d(l), s = !1, u();
         }
     };
 }
 
-function eo(e) {
+function ro(e) {
     let t, n, i, r, s = (
         /*icon*/
-        e[7] && Mn(e)
+        e[7] && Ln(e)
     );
     const u = (
             /*#slots*/
             e[12].default
         ),
         o = di(
             u,
             e,
             /*$$scope*/
             e[11],
             null
         );
     return {
         c() {
-            t = vt("a"), s && s.c(), n = pi(), o && o.c(), N(
+            t = Et("a"), s && s.c(), n = pi(), o && o.c(), N(
                 t,
                 "href",
                 /*link*/
                 e[6]
             ), N(t, "rel", "noopener noreferrer"), N(
                 t,
                 "aria-disabled",
@@ -1314,16 +1314,16 @@
                 e[4] + " " + /*variant*/
                 e[3] + " " + /*elem_classes*/
                 e[1].join(" ") + " svelte-8huxfn"), N(
                 t,
                 "id",
                 /*elem_id*/
                 e[0]
-            ), ye(t, "hidden", ! /*visible*/
-                e[2]), ye(
+            ), Ee(t, "hidden", ! /*visible*/
+                e[2]), Ee(
                 t,
                 "disabled",
                 /*disabled*/
                 e[8]
             ), F(
                 t,
                 "flex-grow",
@@ -1343,15 +1343,15 @@
       e[10]}px, 100%))` : null);
         },
         m(a, f) {
             qe(a, t, f), s && s.m(t, null), _i(t, n), o && o.m(t, null), r = !0;
         },
         p(a, f) {
             /*icon*/
-            a[7] ? s ? s.p(a, f) : (s = Mn(a), s.c(), s.m(t, n)) : s && (s.d(1), s = null), o && o.p && (!r || f & /*$$scope*/
+            a[7] ? s ? s.p(a, f) : (s = Ln(a), s.c(), s.m(t, n)) : s && (s.d(1), s = null), o && o.p && (!r || f & /*$$scope*/
                     2048) && vi(
                     o,
                     u,
                     a,
                     /*$$scope*/
                     a[11],
                     r ? gi(
@@ -1384,17 +1384,17 @@
                         a[1].join(" ") + " svelte-8huxfn")) && N(t, "class", i), (!r || f & /*elem_id*/
                     1) && N(
                     t,
                     "id",
                     /*elem_id*/
                     a[0]
                 ), (!r || f & /*size, variant, elem_classes, visible*/
-                    30) && ye(t, "hidden", ! /*visible*/
+                    30) && Ee(t, "hidden", ! /*visible*/
                     a[2]), (!r || f & /*size, variant, elem_classes, disabled*/
-                    282) && ye(
+                    282) && Ee(
                     t,
                     "disabled",
                     /*disabled*/
                     a[8]
                 ), f & /*scale*/
                 512 && F(
                     t,
@@ -1414,111 +1414,111 @@
                     /*scale*/
                     a[9] === 0 ? "fit-content" : null
                 ), f & /*min_width*/
                 1024 && F(t, "min-width", typeof /*min_width*/ a[10] == "number" ? `calc(min(${/*min_width*/
       a[10]}px, 100%))` : null);
         },
         i(a) {
-            r || (mt(o, a), r = !0);
+            r || (dt(o, a), r = !0);
         },
         o(a) {
-            _t(o, a), r = !1;
+            bt(o, a), r = !1;
         },
         d(a) {
             a && Ve(t), s && s.d(), o && o.d(a);
         }
     };
 }
 
 function On(e) {
     let t, n, i;
     return {
         c() {
-            t = vt("img"), N(t, "class", "button-icon svelte-8huxfn"), ct(t.src, n = /*icon*/
+            t = Et("img"), N(t, "class", "button-icon svelte-8huxfn"), _t(t.src, n = /*icon*/
                 e[7].url) || N(t, "src", n), N(t, "alt", i = `${/*value*/
       e[5]} icon`);
         },
         m(r, s) {
             qe(r, t, s);
         },
         p(r, s) {
             s & /*icon*/
-                128 && !ct(t.src, n = /*icon*/
+                128 && !_t(t.src, n = /*icon*/
                     r[7].url) && N(t, "src", n), s & /*value*/
                 32 && i !== (i = `${/*value*/
       r[5]} icon`) && N(t, "alt", i);
         },
         d(r) {
             r && Ve(t);
         }
     };
 }
 
-function Mn(e) {
+function Ln(e) {
     let t, n, i;
     return {
         c() {
-            t = vt("img"), N(t, "class", "button-icon svelte-8huxfn"), ct(t.src, n = /*icon*/
+            t = Et("img"), N(t, "class", "button-icon svelte-8huxfn"), _t(t.src, n = /*icon*/
                 e[7].url) || N(t, "src", n), N(t, "alt", i = `${/*value*/
       e[5]} icon`);
         },
         m(r, s) {
             qe(r, t, s);
         },
         p(r, s) {
             s & /*icon*/
-                128 && !ct(t.src, n = /*icon*/
+                128 && !_t(t.src, n = /*icon*/
                     r[7].url) && N(t, "src", n), s & /*value*/
                 32 && i !== (i = `${/*value*/
       r[5]} icon`) && N(t, "alt", i);
         },
         d(r) {
             r && Ve(t);
         }
     };
 }
 
-function to(e) {
+function so(e) {
     let t, n, i, r;
-    const s = [eo, $s],
+    const s = [ro, io],
         u = [];
 
     function o(a, f) {
         return (
             /*link*/
             a[6] && /*link*/
             a[6].length > 0 ? 0 : 1
         );
     }
     return t = o(e), n = u[t] = s[t](e), {
         c() {
-            n.c(), i = Ys();
+            n.c(), i = Ks();
         },
         m(a, f) {
             u[t].m(a, f), qe(a, i, f), r = !0;
         },
         p(a, [f]) {
             let l = t;
-            t = o(a), t === l ? u[t].p(a, f) : (Zs(), _t(u[l], 1, 1, () => {
+            t = o(a), t === l ? u[t].p(a, f) : ($s(), bt(u[l], 1, 1, () => {
                 u[l] = null;
-            }), Ws(), n = u[t], n ? n.p(a, f) : (n = u[t] = s[t](a), n.c()), mt(n, 1), n.m(i.parentNode, i));
+            }), Js(), n = u[t], n ? n.p(a, f) : (n = u[t] = s[t](a), n.c()), dt(n, 1), n.m(i.parentNode, i));
         },
         i(a) {
-            r || (mt(n), r = !0);
+            r || (dt(n), r = !0);
         },
         o(a) {
-            _t(n), r = !1;
+            bt(n), r = !1;
         },
         d(a) {
             a && Ve(i), u[t].d(a);
         }
     };
 }
 
-function no(e, t, n) {
+function oo(e, t, n) {
     let {
         $$slots: i = {},
         $$scope: r
     } = t, {
         elem_id: s = ""
     } = t, {
         elem_classes: u = []
@@ -1529,48 +1529,48 @@
     } = t, {
         size: f = "lg"
     } = t, {
         value: l = null
     } = t, {
         link: h = null
     } = t, {
-        icon: c = null
+        icon: m = null
     } = t, {
         disabled: _ = !1
     } = t, {
-        scale: g = null
+        scale: b = null
     } = t, {
-        min_width: m = void 0
+        min_width: g = void 0
     } = t;
 
-    function d(b) {
-        qs.call(this, e, b);
+    function d(c) {
+        Qs.call(this, e, c);
     }
-    return e.$$set = (b) => {
-        "elem_id" in b && n(0, s = b.elem_id), "elem_classes" in b && n(1, u = b.elem_classes), "visible" in b && n(2, o = b.visible), "variant" in b && n(3, a = b.variant), "size" in b && n(4, f = b.size), "value" in b && n(5, l = b.value), "link" in b && n(6, h = b.link), "icon" in b && n(7, c = b.icon), "disabled" in b && n(8, _ = b.disabled), "scale" in b && n(9, g = b.scale), "min_width" in b && n(10, m = b.min_width), "$$scope" in b && n(11, r = b.$$scope);
+    return e.$$set = (c) => {
+        "elem_id" in c && n(0, s = c.elem_id), "elem_classes" in c && n(1, u = c.elem_classes), "visible" in c && n(2, o = c.visible), "variant" in c && n(3, a = c.variant), "size" in c && n(4, f = c.size), "value" in c && n(5, l = c.value), "link" in c && n(6, h = c.link), "icon" in c && n(7, m = c.icon), "disabled" in c && n(8, _ = c.disabled), "scale" in c && n(9, b = c.scale), "min_width" in c && n(10, g = c.min_width), "$$scope" in c && n(11, r = c.$$scope);
     }, [
         s,
         u,
         o,
         a,
         f,
         l,
         h,
-        c,
+        m,
         _,
+        b,
         g,
-        m,
         r,
         i,
         d
     ];
 }
-class Ln extends Vs {
+class Mn extends Zs {
     constructor(t) {
-        super(), Qs(this, t, no, to, Ks, {
+        super(), eo(this, t, oo, so, no, {
             elem_id: 0,
             elem_classes: 1,
             visible: 2,
             variant: 3,
             size: 4,
             value: 5,
             link: 6,
@@ -1578,121 +1578,121 @@
             disabled: 8,
             scale: 9,
             min_width: 10
         });
     }
 }
 
-function io(e) {
+function ao(e) {
     return e && e.__esModule && Object.prototype.hasOwnProperty.call(e, "default") ? e.default : e;
 }
-var ro = function(t) {
-    return so(t) && !oo(t);
+var lo = function(t) {
+    return uo(t) && !fo(t);
 };
 
-function so(e) {
+function uo(e) {
     return !!e && typeof e == "object";
 }
 
-function oo(e) {
+function fo(e) {
     var t = Object.prototype.toString.call(e);
-    return t === "[object RegExp]" || t === "[object Date]" || uo(e);
+    return t === "[object RegExp]" || t === "[object Date]" || mo(e);
 }
-var ao = typeof Symbol == "function" && Symbol.for,
-    lo = ao ? Symbol.for("react.element") : 60103;
+var ho = typeof Symbol == "function" && Symbol.for,
+    co = ho ? Symbol.for("react.element") : 60103;
 
-function uo(e) {
-    return e.$$typeof === lo;
+function mo(e) {
+    return e.$$typeof === co;
 }
 
-function fo(e) {
+function _o(e) {
     return Array.isArray(e) ? [] : {};
 }
 
 function ze(e, t) {
-    return t.clone !== !1 && t.isMergeableObject(e) ? xe(fo(e), e, t) : e;
+    return t.clone !== !1 && t.isMergeableObject(e) ? Se(_o(e), e, t) : e;
 }
 
-function ho(e, t, n) {
+function bo(e, t, n) {
     return e.concat(t).map(function(i) {
         return ze(i, n);
     });
 }
 
-function co(e, t) {
+function go(e, t) {
     if (!t.customMerge)
-        return xe;
+        return Se;
     var n = t.customMerge(e);
-    return typeof n == "function" ? n : xe;
+    return typeof n == "function" ? n : Se;
 }
 
-function mo(e) {
+function po(e) {
     return Object.getOwnPropertySymbols ? Object.getOwnPropertySymbols(e).filter(function(t) {
         return Object.propertyIsEnumerable.call(e, t);
     }) : [];
 }
 
 function Rn(e) {
-    return Object.keys(e).concat(mo(e));
+    return Object.keys(e).concat(po(e));
 }
 
 function yi(e, t) {
     try {
         return t in e;
     } catch {
         return !1;
     }
 }
 
-function _o(e, t) {
+function vo(e, t) {
     return yi(e, t) && !(Object.hasOwnProperty.call(e, t) && Object.propertyIsEnumerable.call(e, t));
 }
 
-function bo(e, t, n) {
+function yo(e, t, n) {
     var i = {};
     return n.isMergeableObject(e) && Rn(e).forEach(function(r) {
         i[r] = ze(e[r], n);
     }), Rn(t).forEach(function(r) {
-        _o(e, r) || (yi(e, r) && n.isMergeableObject(t[r]) ? i[r] = co(r, n)(e[r], t[r], n) : i[r] = ze(t[r], n));
+        vo(e, r) || (yi(e, r) && n.isMergeableObject(t[r]) ? i[r] = go(r, n)(e[r], t[r], n) : i[r] = ze(t[r], n));
     }), i;
 }
 
-function xe(e, t, n) {
-    n = n || {}, n.arrayMerge = n.arrayMerge || ho, n.isMergeableObject = n.isMergeableObject || ro, n.cloneUnlessOtherwiseSpecified = ze;
+function Se(e, t, n) {
+    n = n || {}, n.arrayMerge = n.arrayMerge || bo, n.isMergeableObject = n.isMergeableObject || lo, n.cloneUnlessOtherwiseSpecified = ze;
     var i = Array.isArray(t),
         r = Array.isArray(e),
         s = i === r;
-    return s ? i ? n.arrayMerge(e, t, n) : bo(e, t, n) : ze(t, n);
+    return s ? i ? n.arrayMerge(e, t, n) : yo(e, t, n) : ze(t, n);
 }
-xe.all = function(t, n) {
+Se.all = function(t, n) {
     if (!Array.isArray(t))
         throw new Error("first argument should be an array");
     return t.reduce(function(i, r) {
-        return xe(i, r, n);
+        return Se(i, r, n);
     }, {});
 };
-var go = xe,
-    po = go;
-const vo = /* @__PURE__ */ io(po);
-var Zt = function(e, t) {
-    return Zt = Object.setPrototypeOf || {
+var Eo = Se,
+    wo = Eo;
+const xo = /* @__PURE__ */ ao(wo);
+var Qt = function(e, t) {
+    return Qt = Object.setPrototypeOf || {
         __proto__: []
     }
     instanceof Array && function(n, i) {
         n.__proto__ = i;
     } || function(n, i) {
         for (var r in i)
             Object.prototype.hasOwnProperty.call(i, r) && (n[r] = i[r]);
-    }, Zt(e, t);
+    }, Qt(e, t);
 };
 
-function yt(e, t) {
+function wt(e, t) {
     if (typeof t != "function" && t !== null)
         throw new TypeError("Class extends value " + String(t) + " is not a constructor or null");
-    Zt(e, t);
+    Qt(e, t);
 
     function n() {
         this.constructor = e;
     }
     e.prototype = t === null ? Object.create(t) : (n.prototype = t.prototype, new n());
 }
 var A = function() {
@@ -1702,38 +1702,38 @@
             for (var s in n)
                 Object.prototype.hasOwnProperty.call(n, s) && (t[s] = n[s]);
         }
         return t;
     }, A.apply(this, arguments);
 };
 
-function Rt(e, t, n) {
+function kt(e, t, n) {
     if (n || arguments.length === 2)
         for (var i = 0, r = t.length, s; i < r; i++)
             (s || !(i in t)) && (s || (s = Array.prototype.slice.call(t, 0, i)), s[i] = t[i]);
     return e.concat(s || Array.prototype.slice.call(t));
 }
 var S;
 (function(e) {
     e[e.EXPECT_ARGUMENT_CLOSING_BRACE = 1] = "EXPECT_ARGUMENT_CLOSING_BRACE", e[e.EMPTY_ARGUMENT = 2] = "EMPTY_ARGUMENT", e[e.MALFORMED_ARGUMENT = 3] = "MALFORMED_ARGUMENT", e[e.EXPECT_ARGUMENT_TYPE = 4] = "EXPECT_ARGUMENT_TYPE", e[e.INVALID_ARGUMENT_TYPE = 5] = "INVALID_ARGUMENT_TYPE", e[e.EXPECT_ARGUMENT_STYLE = 6] = "EXPECT_ARGUMENT_STYLE", e[e.INVALID_NUMBER_SKELETON = 7] = "INVALID_NUMBER_SKELETON", e[e.INVALID_DATE_TIME_SKELETON = 8] = "INVALID_DATE_TIME_SKELETON", e[e.EXPECT_NUMBER_SKELETON = 9] = "EXPECT_NUMBER_SKELETON", e[e.EXPECT_DATE_TIME_SKELETON = 10] = "EXPECT_DATE_TIME_SKELETON", e[e.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE = 11] = "UNCLOSED_QUOTE_IN_ARGUMENT_STYLE", e[e.EXPECT_SELECT_ARGUMENT_OPTIONS = 12] = "EXPECT_SELECT_ARGUMENT_OPTIONS", e[e.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE = 13] = "EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE", e[e.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE = 14] = "INVALID_PLURAL_ARGUMENT_OFFSET_VALUE", e[e.EXPECT_SELECT_ARGUMENT_SELECTOR = 15] = "EXPECT_SELECT_ARGUMENT_SELECTOR", e[e.EXPECT_PLURAL_ARGUMENT_SELECTOR = 16] = "EXPECT_PLURAL_ARGUMENT_SELECTOR", e[e.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT = 17] = "EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT", e[e.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT = 18] = "EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT", e[e.INVALID_PLURAL_ARGUMENT_SELECTOR = 19] = "INVALID_PLURAL_ARGUMENT_SELECTOR", e[e.DUPLICATE_PLURAL_ARGUMENT_SELECTOR = 20] = "DUPLICATE_PLURAL_ARGUMENT_SELECTOR", e[e.DUPLICATE_SELECT_ARGUMENT_SELECTOR = 21] = "DUPLICATE_SELECT_ARGUMENT_SELECTOR", e[e.MISSING_OTHER_CLAUSE = 22] = "MISSING_OTHER_CLAUSE", e[e.INVALID_TAG = 23] = "INVALID_TAG", e[e.INVALID_TAG_NAME = 25] = "INVALID_TAG_NAME", e[e.UNMATCHED_CLOSING_TAG = 26] = "UNMATCHED_CLOSING_TAG", e[e.UNCLOSED_TAG = 27] = "UNCLOSED_TAG";
 })(S || (S = {}));
 var I;
 (function(e) {
     e[e.literal = 0] = "literal", e[e.argument = 1] = "argument", e[e.number = 2] = "number", e[e.date = 3] = "date", e[e.time = 4] = "time", e[e.select = 5] = "select", e[e.plural = 6] = "plural", e[e.pound = 7] = "pound", e[e.tag = 8] = "tag";
 })(I || (I = {}));
-var Se;
+var He;
 (function(e) {
     e[e.number = 0] = "number", e[e.dateTime = 1] = "dateTime";
-})(Se || (Se = {}));
+})(He || (He = {}));
 
 function kn(e) {
     return e.type === I.literal;
 }
 
-function yo(e) {
+function So(e) {
     return e.type === I.argument;
 }
 
 function Ei(e) {
     return e.type === I.number;
 }
 
@@ -1749,35 +1749,35 @@
     return e.type === I.select;
 }
 
 function Hi(e) {
     return e.type === I.plural;
 }
 
-function Eo(e) {
+function Ho(e) {
     return e.type === I.pound;
 }
 
 function Ai(e) {
     return e.type === I.tag;
 }
 
 function Bi(e) {
-    return !!(e && typeof e == "object" && e.type === Se.number);
+    return !!(e && typeof e == "object" && e.type === He.number);
 }
 
-function Qt(e) {
-    return !!(e && typeof e == "object" && e.type === Se.dateTime);
+function Jt(e) {
+    return !!(e && typeof e == "object" && e.type === He.dateTime);
 }
-var Ti = /[ \xA0\u1680\u2000-\u200A\u202F\u205F\u3000]/,
-    wo = /(?:[Eec]{1,6}|G{1,5}|[Qq]{1,5}|(?:[yYur]+|U{1,5})|[ML]{1,5}|d{1,2}|D{1,3}|F{1}|[abB]{1,5}|[hkHK]{1,2}|w{1,2}|W{1}|m{1,2}|s{1,2}|[zZOvVxX]{1,4})(?=([^']*'[^']*')*[^']*$)/g;
+var Ci = /[ \xA0\u1680\u2000-\u200A\u202F\u205F\u3000]/,
+    Ao = /(?:[Eec]{1,6}|G{1,5}|[Qq]{1,5}|(?:[yYur]+|U{1,5})|[ML]{1,5}|d{1,2}|D{1,3}|F{1}|[abB]{1,5}|[hkHK]{1,2}|w{1,2}|W{1}|m{1,2}|s{1,2}|[zZOvVxX]{1,4})(?=([^']*'[^']*')*[^']*$)/g;
 
-function xo(e) {
+function Bo(e) {
     var t = {};
-    return e.replace(wo, function(n) {
+    return e.replace(Ao, function(n) {
         var i = n.length;
         switch (n[0]) {
             case "G":
                 t.era = i === 4 ? "long" : i === 5 ? "narrow" : "short";
                 break;
             case "y":
                 t.year = i === 2 ? "2-digit" : "numeric";
@@ -1858,21 +1858,21 @@
             case "X":
             case "x":
                 throw new RangeError("`Z/O/v/V/X/x` (timeZone) patterns are not supported, use `z` instead");
         }
         return "";
     }), t;
 }
-var So = /[\t-\r \x85\u200E\u200F\u2028\u2029]/i;
+var Co = /[\t-\r \x85\u200E\u200F\u2028\u2029]/i;
 
-function Ho(e) {
+function To(e) {
     if (e.length === 0)
         throw new Error("Number skeleton cannot be empty");
-    for (var t = e.split(So).filter(function(c) {
-            return c.length > 0;
+    for (var t = e.split(Co).filter(function(m) {
+            return m.length > 0;
         }), n = [], i = 0, r = t; i < r.length; i++) {
         var s = r[i],
             u = s.split("/");
         if (u.length === 0)
             throw new Error("Invalid number skeleton");
         for (var o = u[0], a = u.slice(1), f = 0, l = a; f < l.length; f++) {
             var h = l[f];
@@ -1883,25 +1883,25 @@
             stem: o,
             options: a
         });
     }
     return n;
 }
 
-function Ao(e) {
+function Po(e) {
     return e.replace(/^(.*?)-/, "");
 }
 var Dn = /^\.(?:(0+)(\*)?|(#+)|(0+)(#+))$/g,
-    Ci = /^(@+)?(\+|#+)?[rs]?$/g,
-    Bo = /(\*)(0+)|(#+)(0+)|(0+)/g,
+    Ti = /^(@+)?(\+|#+)?[rs]?$/g,
+    Io = /(\*)(0+)|(#+)(0+)|(0+)/g,
     Pi = /^(0+)$/;
 
 function Un(e) {
     var t = {};
-    return e[e.length - 1] === "r" ? t.roundingPriority = "morePrecision" : e[e.length - 1] === "s" && (t.roundingPriority = "lessPrecision"), e.replace(Ci, function(n, i, r) {
+    return e[e.length - 1] === "r" ? t.roundingPriority = "morePrecision" : e[e.length - 1] === "s" && (t.roundingPriority = "lessPrecision"), e.replace(Ti, function(n, i, r) {
         return typeof r != "string" ? (t.minimumSignificantDigits = i.length, t.maximumSignificantDigits = i.length) : r === "+" ? t.minimumSignificantDigits = i.length : i[0] === "#" ? t.maximumSignificantDigits = i.length : (t.minimumSignificantDigits = i.length, t.maximumSignificantDigits = i.length + (typeof r == "string" ? r.length : 0)), "";
     }), t;
 }
 
 function Ii(e) {
     switch (e) {
         case "sign-auto":
@@ -1939,15 +1939,15 @@
         case "+_":
             return {
                 signDisplay: "never"
             };
     }
 }
 
-function To(e) {
+function No(e) {
     var t;
     if (e[0] === "E" && e[1] === "E" ? (t = {
             notation: "engineering"
         }, e = e.slice(2)) : e[0] === "E" && (t = {
             notation: "scientific"
         }, e = e.slice(1)), t) {
         var n = e.slice(0, 2);
@@ -1960,15 +1960,15 @@
 
 function Gn(e) {
     var t = {},
         n = Ii(e);
     return n || t;
 }
 
-function Co(e) {
+function Oo(e) {
     for (var t = {}, n = 0, i = e; n < i.length; n++) {
         var r = i[n];
         switch (r.stem) {
             case "percent":
             case "%":
                 t.style = "percent";
                 continue;
@@ -1984,15 +1984,15 @@
                 continue;
             case "precision-integer":
             case ".":
                 t.maximumFractionDigits = 0;
                 continue;
             case "measure-unit":
             case "unit":
-                t.style = "unit", t.unit = Ao(r.options[0]);
+                t.style = "unit", t.unit = Po(r.options[0]);
                 continue;
             case "compact-short":
             case "K":
                 t.notation = "compact", t.compactDisplay = "short";
                 continue;
             case "compact-long":
             case "KK":
@@ -2029,19 +2029,19 @@
                 continue;
             case "scale":
                 t.scale = parseFloat(r.options[0]);
                 continue;
             case "integer-width":
                 if (r.options.length > 1)
                     throw new RangeError("integer-width stems only accept a single optional option");
-                r.options[0].replace(Bo, function(a, f, l, h, c, _) {
+                r.options[0].replace(Io, function(a, f, l, h, m, _) {
                     if (f)
                         t.minimumIntegerDigits = l.length;
                     else {
-                        if (h && c)
+                        if (h && m)
                             throw new Error("We currently do not support maximum integer digits");
                         if (_)
                             throw new Error("We currently do not support exact integer digits");
                     }
                     return "";
                 });
                 continue;
@@ -2049,35 +2049,35 @@
         if (Pi.test(r.stem)) {
             t.minimumIntegerDigits = r.stem.length;
             continue;
         }
         if (Dn.test(r.stem)) {
             if (r.options.length > 1)
                 throw new RangeError("Fraction-precision stems only accept a single optional option");
-            r.stem.replace(Dn, function(a, f, l, h, c, _) {
-                return l === "*" ? t.minimumFractionDigits = f.length : h && h[0] === "#" ? t.maximumFractionDigits = h.length : c && _ ? (t.minimumFractionDigits = c.length, t.maximumFractionDigits = c.length + _.length) : (t.minimumFractionDigits = f.length, t.maximumFractionDigits = f.length), "";
+            r.stem.replace(Dn, function(a, f, l, h, m, _) {
+                return l === "*" ? t.minimumFractionDigits = f.length : h && h[0] === "#" ? t.maximumFractionDigits = h.length : m && _ ? (t.minimumFractionDigits = m.length, t.maximumFractionDigits = m.length + _.length) : (t.minimumFractionDigits = f.length, t.maximumFractionDigits = f.length), "";
             });
             var s = r.options[0];
             s === "w" ? t = A(A({}, t), {
                 trailingZeroDisplay: "stripIfInteger"
             }) : s && (t = A(A({}, t), Un(s)));
             continue;
         }
-        if (Ci.test(r.stem)) {
+        if (Ti.test(r.stem)) {
             t = A(A({}, t), Un(r.stem));
             continue;
         }
         var u = Ii(r.stem);
         u && (t = A(A({}, t), u));
-        var o = To(r.stem);
+        var o = No(r.stem);
         o && (t = A(A({}, t), o));
     }
     return t;
 }
-var Qe = {
+var Ke = {
     AX: [
         "H"
     ],
     BQ: [
         "H"
     ],
     CP: [
@@ -3407,35 +3407,35 @@
         "hB",
         "hb",
         "H",
         "h"
     ]
 };
 
-function Po(e, t) {
+function Lo(e, t) {
     for (var n = "", i = 0; i < e.length; i++) {
         var r = e.charAt(i);
         if (r === "j") {
             for (var s = 0; i + 1 < e.length && e.charAt(i + 1) === r;)
                 s++, i++;
             var u = 1 + (s & 1),
                 o = s < 2 ? 1 : 3 + (s >> 1),
                 a = "a",
-                f = Io(t);
+                f = Mo(t);
             for ((f == "H" || f == "k") && (o = 0); o-- > 0;)
                 n += a;
             for (; u-- > 0;)
                 n = f + n;
         } else
             r === "J" ? n += "H" : n += r;
     }
     return n;
 }
 
-function Io(e) {
+function Mo(e) {
     var t = e.hourCycle;
     if (t === void 0 && // @ts-ignore hourCycle(s) is not identified yet
         e.hourCycles && // @ts-ignore
         e.hourCycles.length && (t = e.hourCycles[0]), t)
         switch (t) {
             case "h24":
                 return "k";
@@ -3447,83 +3447,83 @@
                 return "K";
             default:
                 throw new Error("Invalid hourCycle");
         }
     var n = e.language,
         i;
     n !== "root" && (i = e.maximize().region);
-    var r = Qe[i || ""] || Qe[n || ""] || Qe["".concat(n, "-001")] || Qe["001"];
+    var r = Ke[i || ""] || Ke[n || ""] || Ke["".concat(n, "-001")] || Ke["001"];
     return r[0];
 }
-var kt, No = new RegExp("^".concat(Ti.source, "*")),
-    Oo = new RegExp("".concat(Ti.source, "*$"));
+var Dt, Ro = new RegExp("^".concat(Ci.source, "*")),
+    ko = new RegExp("".concat(Ci.source, "*$"));
 
 function H(e, t) {
     return {
         start: e,
         end: t
     };
 }
-var Mo = !!String.prototype.startsWith,
-    Lo = !!String.fromCodePoint,
-    Ro = !!Object.fromEntries,
-    ko = !!String.prototype.codePointAt,
-    Do = !!String.prototype.trimStart,
-    Uo = !!String.prototype.trimEnd,
-    Go = !!Number.isSafeInteger,
-    Fo = Go ? Number.isSafeInteger : function(e) {
+var Do = !!String.prototype.startsWith,
+    Uo = !!String.fromCodePoint,
+    Go = !!Object.fromEntries,
+    Fo = !!String.prototype.codePointAt,
+    zo = !!String.prototype.trimStart,
+    jo = !!String.prototype.trimEnd,
+    Xo = !!Number.isSafeInteger,
+    Vo = Xo ? Number.isSafeInteger : function(e) {
         return typeof e == "number" && isFinite(e) && Math.floor(e) === e && Math.abs(e) <= 9007199254740991;
     },
-    Jt = !0;
+    Kt = !0;
 try {
-    var zo = Oi("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
-    Jt = ((kt = zo.exec("a")) === null || kt === void 0 ? void 0 : kt[0]) === "a";
+    var qo = Oi("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
+    Kt = ((Dt = qo.exec("a")) === null || Dt === void 0 ? void 0 : Dt[0]) === "a";
 } catch {
-    Jt = !1;
+    Kt = !1;
 }
-var Fn = Mo ? (
+var Fn = Do ? (
         // Native
         function(t, n, i) {
             return t.startsWith(n, i);
         }
     ) : (
         // For IE11
         function(t, n, i) {
             return t.slice(i, i + n.length) === n;
         }
     ),
-    Kt = Lo ? String.fromCodePoint : (
+    $t = Uo ? String.fromCodePoint : (
         // IE11
         function() {
             for (var t = [], n = 0; n < arguments.length; n++)
                 t[n] = arguments[n];
             for (var i = "", r = t.length, s = 0, u; r > s;) {
                 if (u = t[s++], u > 1114111)
                     throw RangeError(u + " is not a valid code point");
                 i += u < 65536 ? String.fromCharCode(u) : String.fromCharCode(((u -= 65536) >> 10) + 55296, u % 1024 + 56320);
             }
             return i;
         }
     ),
     zn = (
         // native
-        Ro ? Object.fromEntries : (
+        Go ? Object.fromEntries : (
             // Ponyfill
             function(t) {
                 for (var n = {}, i = 0, r = t; i < r.length; i++) {
                     var s = r[i],
                         u = s[0],
                         o = s[1];
                     n[u] = o;
                 }
                 return n;
             }
         )
     ),
-    Ni = ko ? (
+    Ni = Fo ? (
         // Native
         function(t, n) {
             return t.codePointAt(n);
         }
     ) : (
         // IE 11
         function(t, n) {
@@ -3531,60 +3531,60 @@
             if (!(n < 0 || n >= i)) {
                 var r = t.charCodeAt(n),
                     s;
                 return r < 55296 || r > 56319 || n + 1 === i || (s = t.charCodeAt(n + 1)) < 56320 || s > 57343 ? r : (r - 55296 << 10) + (s - 56320) + 65536;
             }
         }
     ),
-    jo = Do ? (
+    Wo = zo ? (
         // Native
         function(t) {
             return t.trimStart();
         }
     ) : (
         // Ponyfill
         function(t) {
-            return t.replace(No, "");
+            return t.replace(Ro, "");
         }
     ),
-    Xo = Uo ? (
+    Yo = jo ? (
         // Native
         function(t) {
             return t.trimEnd();
         }
     ) : (
         // Ponyfill
         function(t) {
-            return t.replace(Oo, "");
+            return t.replace(ko, "");
         }
     );
 
 function Oi(e, t) {
     return new RegExp(e, t);
 }
-var $t;
-if (Jt) {
+var en;
+if (Kt) {
     var jn = Oi("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
-    $t = function(t, n) {
+    en = function(t, n) {
         var i;
         jn.lastIndex = n;
         var r = jn.exec(t);
         return (i = r[1]) !== null && i !== void 0 ? i : "";
     };
 } else
-    $t = function(t, n) {
+    en = function(t, n) {
         for (var i = [];;) {
             var r = Ni(t, n);
-            if (r === void 0 || Mi(r) || Yo(r))
+            if (r === void 0 || Li(r) || Ko(r))
                 break;
             i.push(r), n += r >= 65536 ? 2 : 1;
         }
-        return Kt.apply(void 0, i);
+        return $t.apply(void 0, i);
     };
-var Vo = (
+var Zo = (
     /** @class */
     function() {
         function e(t, n) {
             n === void 0 && (n = {}), this.message = t, this.position = {
                 offset: 0,
                 line: 1,
                 column: 1
@@ -3611,15 +3611,15 @@
                             type: I.pound,
                             location: H(o, this.clonePosition())
                         });
                     } else if (s === 60 && !this.ignoreTag && this.peek() === 47) {
                         if (i)
                             break;
                         return this.error(S.UNMATCHED_CLOSING_TAG, H(this.clonePosition(), this.clonePosition()));
-                    } else if (s === 60 && !this.ignoreTag && en(this.peek() || 0)) {
+                    } else if (s === 60 && !this.ignoreTag && tn(this.peek() || 0)) {
                         var u = this.parseTag(t, n);
                         if (u.err)
                             return u;
                         r.push(u.val);
                     } else {
                         var u = this.parseLiteral(t, n);
                         if (u.err)
@@ -3648,15 +3648,15 @@
             if (this.bumpIf(">")) {
                 var s = this.parseMessage(t + 1, n, !0);
                 if (s.err)
                     return s;
                 var u = s.val,
                     o = this.clonePosition();
                 if (this.bumpIf("</")) {
-                    if (this.isEOF() || !en(this.char()))
+                    if (this.isEOF() || !tn(this.char()))
                         return this.error(S.INVALID_TAG, H(o, this.clonePosition()));
                     var a = this.clonePosition(),
                         f = this.parseTagName();
                     return r !== f ? this.error(S.UNMATCHED_CLOSING_TAG, H(a, this.clonePosition())) : (this.bumpSpace(), this.bumpIf(">") ? {
                         val: {
                             type: I.tag,
                             value: r,
@@ -3667,15 +3667,15 @@
                     } : this.error(S.INVALID_TAG, H(o, this.clonePosition())));
                 } else
                     return this.error(S.UNCLOSED_TAG, H(i, this.clonePosition()));
             } else
                 return this.error(S.INVALID_TAG, H(i, this.clonePosition()));
         }, e.prototype.parseTagName = function() {
             var t = this.offset();
-            for (this.bump(); !this.isEOF() && Wo(this.char());)
+            for (this.bump(); !this.isEOF() && Jo(this.char());)
                 this.bump();
             return this.message.slice(t, this.offset());
         }, e.prototype.parseLiteral = function(t, n) {
             for (var i = this.clonePosition(), r = "";;) {
                 var s = this.tryParseQuote(n);
                 if (s) {
                     r += s;
@@ -3700,15 +3700,15 @@
                     value: r,
                     location: a
                 },
                 err: null
             };
         }, e.prototype.tryParseLeftAngleBracket = function() {
             return !this.isEOF() && this.char() === 60 && (this.ignoreTag || // If at the opening tag or closing tag position, bail.
-                !qo(this.peek() || 0)) ? (this.bump(), "<") : null;
+                !Qo(this.peek() || 0)) ? (this.bump(), "<") : null;
         }, e.prototype.tryParseQuote = function(t) {
             if (this.isEOF() || this.char() !== 39)
                 return null;
             switch (this.peek()) {
                 case 39:
                     return this.bump(), this.bump(), "'";
                 case 123:
@@ -3734,20 +3734,20 @@
                         this.bump();
                         break;
                     }
                 else
                     n.push(i);
                 this.bump();
             }
-            return Kt.apply(void 0, n);
+            return $t.apply(void 0, n);
         }, e.prototype.tryParseUnquoted = function(t, n) {
             if (this.isEOF())
                 return null;
             var i = this.char();
-            return i === 60 || i === 123 || i === 35 && (n === "plural" || n === "selectordinal") || i === 125 && t > 0 ? null : (this.bump(), Kt(i));
+            return i === 60 || i === 123 || i === 35 && (n === "plural" || n === "selectordinal") || i === 125 && t > 0 ? null : (this.bump(), $t(i));
         }, e.prototype.parseArgument = function(t, n) {
             var i = this.clonePosition();
             if (this.bump(), this.bumpSpace(), this.isEOF())
                 return this.error(S.EXPECT_ARGUMENT_CLOSING_BRACE, H(i, this.clonePosition()));
             if (this.char() === 125)
                 return this.bump(), this.error(S.EMPTY_ARGUMENT, H(i, this.clonePosition()));
             var r = this.parseIdentifierIfPossible().value;
@@ -3770,15 +3770,15 @@
                     return this.bump(), this.bumpSpace(), this.isEOF() ? this.error(S.EXPECT_ARGUMENT_CLOSING_BRACE, H(i, this.clonePosition())) : this.parseArgumentOptions(t, n, r, i);
                 default:
                     return this.error(S.MALFORMED_ARGUMENT, H(i, this.clonePosition()));
             }
         }, e.prototype.parseIdentifierIfPossible = function() {
             var t = this.clonePosition(),
                 n = this.offset(),
-                i = $t(this.message, n),
+                i = en(this.message, n),
                 r = n + i.length;
             this.bumpTo(r);
             var s = this.clonePosition(),
                 u = H(t, s);
             return {
                 value: i,
                 location: u
@@ -3797,114 +3797,114 @@
                     var f = null;
                     if (this.bumpIf(",")) {
                         this.bumpSpace();
                         var l = this.clonePosition(),
                             h = this.parseSimpleArgStyleIfPossible();
                         if (h.err)
                             return h;
-                        var c = Xo(h.val);
-                        if (c.length === 0)
+                        var m = Yo(h.val);
+                        if (m.length === 0)
                             return this.error(S.EXPECT_ARGUMENT_STYLE, H(this.clonePosition(), this.clonePosition()));
                         var _ = H(l, this.clonePosition());
                         f = {
-                            style: c,
+                            style: m,
                             styleLocation: _
                         };
                     }
-                    var g = this.tryParseArgumentClose(r);
-                    if (g.err)
-                        return g;
-                    var m = H(r, this.clonePosition());
+                    var b = this.tryParseArgumentClose(r);
+                    if (b.err)
+                        return b;
+                    var g = H(r, this.clonePosition());
                     if (f && Fn(f == null ? void 0 : f.style, "::", 0)) {
-                        var d = jo(f.style.slice(2));
+                        var d = Wo(f.style.slice(2));
                         if (o === "number") {
                             var h = this.parseNumberSkeletonFromString(d, f.styleLocation);
                             return h.err ? h : {
                                 val: {
                                     type: I.number,
                                     value: i,
-                                    location: m,
+                                    location: g,
                                     style: h.val
                                 },
                                 err: null
                             };
                         } else {
                             if (d.length === 0)
-                                return this.error(S.EXPECT_DATE_TIME_SKELETON, m);
-                            var b = d;
-                            this.locale && (b = Po(d, this.locale));
-                            var c = {
-                                    type: Se.dateTime,
-                                    pattern: b,
+                                return this.error(S.EXPECT_DATE_TIME_SKELETON, g);
+                            var c = d;
+                            this.locale && (c = Lo(d, this.locale));
+                            var m = {
+                                    type: He.dateTime,
+                                    pattern: c,
                                     location: f.styleLocation,
-                                    parsedOptions: this.shouldParseSkeletons ? xo(b) : {}
+                                    parsedOptions: this.shouldParseSkeletons ? Bo(c) : {}
                                 },
                                 y = o === "date" ? I.date : I.time;
                             return {
                                 val: {
                                     type: y,
                                     value: i,
-                                    location: m,
-                                    style: c
+                                    location: g,
+                                    style: m
                                 },
                                 err: null
                             };
                         }
                     }
                     return {
                         val: {
                             type: o === "number" ? I.number : o === "date" ? I.date : I.time,
                             value: i,
-                            location: m,
+                            location: g,
                             style: (s = f == null ? void 0 : f.style) !== null && s !== void 0 ? s : null
                         },
                         err: null
                     };
                 }
                 case "plural":
                 case "selectordinal":
                 case "select": {
                     var p = this.clonePosition();
                     if (this.bumpSpace(), !this.bumpIf(","))
                         return this.error(S.EXPECT_SELECT_ARGUMENT_OPTIONS, H(p, A({}, p)));
                     this.bumpSpace();
                     var B = this.parseIdentifierIfPossible(),
-                        T = 0;
+                        C = 0;
                     if (o !== "select" && B.value === "offset") {
                         if (!this.bumpIf(":"))
                             return this.error(S.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, H(this.clonePosition(), this.clonePosition()));
                         this.bumpSpace();
                         var h = this.tryParseDecimalInteger(S.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, S.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE);
                         if (h.err)
                             return h;
-                        this.bumpSpace(), B = this.parseIdentifierIfPossible(), T = h.val;
+                        this.bumpSpace(), B = this.parseIdentifierIfPossible(), C = h.val;
                     }
                     var O = this.tryParsePluralOrSelectOptions(t, o, n, B);
                     if (O.err)
                         return O;
-                    var g = this.tryParseArgumentClose(r);
-                    if (g.err)
-                        return g;
-                    var C = H(r, this.clonePosition());
+                    var b = this.tryParseArgumentClose(r);
+                    if (b.err)
+                        return b;
+                    var T = H(r, this.clonePosition());
                     return o === "select" ? {
                         val: {
                             type: I.select,
                             value: i,
                             options: zn(O.val),
-                            location: C
+                            location: T
                         },
                         err: null
                     } : {
                         val: {
                             type: I.plural,
                             value: i,
                             options: zn(O.val),
-                            offset: T,
+                            offset: C,
                             pluralType: o === "plural" ? "cardinal" : "ordinal",
-                            location: C
+                            location: T
                         },
                         err: null
                     };
                 }
                 default:
                     return this.error(S.INVALID_ARGUMENT_TYPE, H(u, a));
             }
@@ -3947,54 +3947,54 @@
             return {
                 val: this.message.slice(n.offset, this.offset()),
                 err: null
             };
         }, e.prototype.parseNumberSkeletonFromString = function(t, n) {
             var i = [];
             try {
-                i = Ho(t);
+                i = To(t);
             } catch {
                 return this.error(S.INVALID_NUMBER_SKELETON, n);
             }
             return {
                 val: {
-                    type: Se.number,
+                    type: He.number,
                     tokens: i,
                     location: n,
-                    parsedOptions: this.shouldParseSkeletons ? Co(i) : {}
+                    parsedOptions: this.shouldParseSkeletons ? Oo(i) : {}
                 },
                 err: null
             };
         }, e.prototype.tryParsePluralOrSelectOptions = function(t, n, i, r) {
             for (var s, u = !1, o = [], a = /* @__PURE__ */ new Set(), f = r.value, l = r.location;;) {
                 if (f.length === 0) {
                     var h = this.clonePosition();
                     if (n !== "select" && this.bumpIf("=")) {
-                        var c = this.tryParseDecimalInteger(S.EXPECT_PLURAL_ARGUMENT_SELECTOR, S.INVALID_PLURAL_ARGUMENT_SELECTOR);
-                        if (c.err)
-                            return c;
+                        var m = this.tryParseDecimalInteger(S.EXPECT_PLURAL_ARGUMENT_SELECTOR, S.INVALID_PLURAL_ARGUMENT_SELECTOR);
+                        if (m.err)
+                            return m;
                         l = H(h, this.clonePosition()), f = this.message.slice(h.offset, this.offset());
                     } else
                         break;
                 }
                 if (a.has(f))
                     return this.error(n === "select" ? S.DUPLICATE_SELECT_ARGUMENT_SELECTOR : S.DUPLICATE_PLURAL_ARGUMENT_SELECTOR, l);
                 f === "other" && (u = !0), this.bumpSpace();
                 var _ = this.clonePosition();
                 if (!this.bumpIf("{"))
                     return this.error(n === "select" ? S.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT : S.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT, H(this.clonePosition(), this.clonePosition()));
-                var g = this.parseMessage(t + 1, n, i);
+                var b = this.parseMessage(t + 1, n, i);
+                if (b.err)
+                    return b;
+                var g = this.tryParseArgumentClose(_);
                 if (g.err)
                     return g;
-                var m = this.tryParseArgumentClose(_);
-                if (m.err)
-                    return m;
                 o.push([
                     f, {
-                        value: g.val,
+                        value: b.val,
                         location: H(_, this.clonePosition())
                     }
                 ]), a.add(f), this.bumpSpace(), s = this.parseIdentifierIfPossible(), f = s.value, l = s.location;
             }
             return o.length === 0 ? this.error(n === "select" ? S.EXPECT_SELECT_ARGUMENT_SELECTOR : S.EXPECT_PLURAL_ARGUMENT_SELECTOR, H(this.clonePosition(), this.clonePosition())) : this.requiresOtherClause && !u ? this.error(S.MISSING_OTHER_CLAUSE, H(this.clonePosition(), this.clonePosition())) : {
                 val: o,
                 err: null
@@ -4007,15 +4007,15 @@
                 var o = this.char();
                 if (o >= 48 && o <= 57)
                     s = !0, u = u * 10 + (o - 48), this.bump();
                 else
                     break;
             }
             var a = H(r, this.clonePosition());
-            return s ? (u *= i, Fo(u) ? {
+            return s ? (u *= i, Vo(u) ? {
                 val: u,
                 err: null
             } : this.error(n, a)) : this.error(t, a);
         }, e.prototype.offset = function() {
             return this.position.offset;
         }, e.prototype.isEOF = function() {
             return this.offset() === this.message.length;
@@ -4067,364 +4067,364 @@
                     break;
                 if (n > t)
                     throw Error("targetOffset ".concat(t, " is at invalid UTF-16 code unit boundary"));
                 if (this.bump(), this.isEOF())
                     break;
             }
         }, e.prototype.bumpSpace = function() {
-            for (; !this.isEOF() && Mi(this.char());)
+            for (; !this.isEOF() && Li(this.char());)
                 this.bump();
         }, e.prototype.peek = function() {
             if (this.isEOF())
                 return null;
             var t = this.char(),
                 n = this.offset(),
                 i = this.message.charCodeAt(n + (t >= 65536 ? 2 : 1));
             return i ?? null;
         }, e;
     }()
 );
 
-function en(e) {
+function tn(e) {
     return e >= 97 && e <= 122 || e >= 65 && e <= 90;
 }
 
-function qo(e) {
-    return en(e) || e === 47;
+function Qo(e) {
+    return tn(e) || e === 47;
 }
 
-function Wo(e) {
+function Jo(e) {
     return e === 45 || e === 46 || e >= 48 && e <= 57 || e === 95 || e >= 97 && e <= 122 || e >= 65 && e <= 90 || e == 183 || e >= 192 && e <= 214 || e >= 216 && e <= 246 || e >= 248 && e <= 893 || e >= 895 && e <= 8191 || e >= 8204 && e <= 8205 || e >= 8255 && e <= 8256 || e >= 8304 && e <= 8591 || e >= 11264 && e <= 12271 || e >= 12289 && e <= 55295 || e >= 63744 && e <= 64975 || e >= 65008 && e <= 65533 || e >= 65536 && e <= 983039;
 }
 
-function Mi(e) {
+function Li(e) {
     return e >= 9 && e <= 13 || e === 32 || e === 133 || e >= 8206 && e <= 8207 || e === 8232 || e === 8233;
 }
 
-function Yo(e) {
+function Ko(e) {
     return e >= 33 && e <= 35 || e === 36 || e >= 37 && e <= 39 || e === 40 || e === 41 || e === 42 || e === 43 || e === 44 || e === 45 || e >= 46 && e <= 47 || e >= 58 && e <= 59 || e >= 60 && e <= 62 || e >= 63 && e <= 64 || e === 91 || e === 92 || e === 93 || e === 94 || e === 96 || e === 123 || e === 124 || e === 125 || e === 126 || e === 161 || e >= 162 && e <= 165 || e === 166 || e === 167 || e === 169 || e === 171 || e === 172 || e === 174 || e === 176 || e === 177 || e === 182 || e === 187 || e === 191 || e === 215 || e === 247 || e >= 8208 && e <= 8213 || e >= 8214 && e <= 8215 || e === 8216 || e === 8217 || e === 8218 || e >= 8219 && e <= 8220 || e === 8221 || e === 8222 || e === 8223 || e >= 8224 && e <= 8231 || e >= 8240 && e <= 8248 || e === 8249 || e === 8250 || e >= 8251 && e <= 8254 || e >= 8257 && e <= 8259 || e === 8260 || e === 8261 || e === 8262 || e >= 8263 && e <= 8273 || e === 8274 || e === 8275 || e >= 8277 && e <= 8286 || e >= 8592 && e <= 8596 || e >= 8597 && e <= 8601 || e >= 8602 && e <= 8603 || e >= 8604 && e <= 8607 || e === 8608 || e >= 8609 && e <= 8610 || e === 8611 || e >= 8612 && e <= 8613 || e === 8614 || e >= 8615 && e <= 8621 || e === 8622 || e >= 8623 && e <= 8653 || e >= 8654 && e <= 8655 || e >= 8656 && e <= 8657 || e === 8658 || e === 8659 || e === 8660 || e >= 8661 && e <= 8691 || e >= 8692 && e <= 8959 || e >= 8960 && e <= 8967 || e === 8968 || e === 8969 || e === 8970 || e === 8971 || e >= 8972 && e <= 8991 || e >= 8992 && e <= 8993 || e >= 8994 && e <= 9e3 || e === 9001 || e === 9002 || e >= 9003 && e <= 9083 || e === 9084 || e >= 9085 && e <= 9114 || e >= 9115 && e <= 9139 || e >= 9140 && e <= 9179 || e >= 9180 && e <= 9185 || e >= 9186 && e <= 9254 || e >= 9255 && e <= 9279 || e >= 9280 && e <= 9290 || e >= 9291 && e <= 9311 || e >= 9472 && e <= 9654 || e === 9655 || e >= 9656 && e <= 9664 || e === 9665 || e >= 9666 && e <= 9719 || e >= 9720 && e <= 9727 || e >= 9728 && e <= 9838 || e === 9839 || e >= 9840 && e <= 10087 || e === 10088 || e === 10089 || e === 10090 || e === 10091 || e === 10092 || e === 10093 || e === 10094 || e === 10095 || e === 10096 || e === 10097 || e === 10098 || e === 10099 || e === 10100 || e === 10101 || e >= 10132 && e <= 10175 || e >= 10176 && e <= 10180 || e === 10181 || e === 10182 || e >= 10183 && e <= 10213 || e === 10214 || e === 10215 || e === 10216 || e === 10217 || e === 10218 || e === 10219 || e === 10220 || e === 10221 || e === 10222 || e === 10223 || e >= 10224 && e <= 10239 || e >= 10240 && e <= 10495 || e >= 10496 && e <= 10626 || e === 10627 || e === 10628 || e === 10629 || e === 10630 || e === 10631 || e === 10632 || e === 10633 || e === 10634 || e === 10635 || e === 10636 || e === 10637 || e === 10638 || e === 10639 || e === 10640 || e === 10641 || e === 10642 || e === 10643 || e === 10644 || e === 10645 || e === 10646 || e === 10647 || e === 10648 || e >= 10649 && e <= 10711 || e === 10712 || e === 10713 || e === 10714 || e === 10715 || e >= 10716 && e <= 10747 || e === 10748 || e === 10749 || e >= 10750 && e <= 11007 || e >= 11008 && e <= 11055 || e >= 11056 && e <= 11076 || e >= 11077 && e <= 11078 || e >= 11079 && e <= 11084 || e >= 11085 && e <= 11123 || e >= 11124 && e <= 11125 || e >= 11126 && e <= 11157 || e === 11158 || e >= 11159 && e <= 11263 || e >= 11776 && e <= 11777 || e === 11778 || e === 11779 || e === 11780 || e === 11781 || e >= 11782 && e <= 11784 || e === 11785 || e === 11786 || e === 11787 || e === 11788 || e === 11789 || e >= 11790 && e <= 11798 || e === 11799 || e >= 11800 && e <= 11801 || e === 11802 || e === 11803 || e === 11804 || e === 11805 || e >= 11806 && e <= 11807 || e === 11808 || e === 11809 || e === 11810 || e === 11811 || e === 11812 || e === 11813 || e === 11814 || e === 11815 || e === 11816 || e === 11817 || e >= 11818 && e <= 11822 || e === 11823 || e >= 11824 && e <= 11833 || e >= 11834 && e <= 11835 || e >= 11836 && e <= 11839 || e === 11840 || e === 11841 || e === 11842 || e >= 11843 && e <= 11855 || e >= 11856 && e <= 11857 || e === 11858 || e >= 11859 && e <= 11903 || e >= 12289 && e <= 12291 || e === 12296 || e === 12297 || e === 12298 || e === 12299 || e === 12300 || e === 12301 || e === 12302 || e === 12303 || e === 12304 || e === 12305 || e >= 12306 && e <= 12307 || e === 12308 || e === 12309 || e === 12310 || e === 12311 || e === 12312 || e === 12313 || e === 12314 || e === 12315 || e === 12316 || e === 12317 || e >= 12318 && e <= 12319 || e === 12320 || e === 12336 || e === 64830 || e === 64831 || e >= 65093 && e <= 65094;
 }
 
-function tn(e) {
+function nn(e) {
     e.forEach(function(t) {
         if (delete t.location, Si(t) || Hi(t))
             for (var n in t.options)
-                delete t.options[n].location, tn(t.options[n].value);
+                delete t.options[n].location, nn(t.options[n].value);
         else
-            Ei(t) && Bi(t.style) || (wi(t) || xi(t)) && Qt(t.style) ? delete t.style.location : Ai(t) && tn(t.children);
+            Ei(t) && Bi(t.style) || (wi(t) || xi(t)) && Jt(t.style) ? delete t.style.location : Ai(t) && nn(t.children);
     });
 }
 
-function Zo(e, t) {
+function $o(e, t) {
     t === void 0 && (t = {}), t = A({
         shouldParseSkeletons: !0,
         requiresOtherClause: !0
     }, t);
-    var n = new Vo(e, t).parse();
+    var n = new Zo(e, t).parse();
     if (n.err) {
         var i = SyntaxError(S[n.err.kind]);
         throw i.location = n.err.location, i.originalMessage = n.err.message, i;
     }
-    return t != null && t.captureLocation || tn(n.val), n.val;
+    return t != null && t.captureLocation || nn(n.val), n.val;
 }
 
-function Dt(e, t) {
-    var n = t && t.cache ? t.cache : ta,
-        i = t && t.serializer ? t.serializer : ea,
-        r = t && t.strategy ? t.strategy : Jo;
+function Ut(e, t) {
+    var n = t && t.cache ? t.cache : sa,
+        i = t && t.serializer ? t.serializer : ra,
+        r = t && t.strategy ? t.strategy : ta;
     return r(e, {
         cache: n,
         serializer: i
     });
 }
 
-function Qo(e) {
+function ea(e) {
     return e == null || typeof e == "number" || typeof e == "boolean";
 }
 
-function Li(e, t, n, i) {
-    var r = Qo(i) ? i : n(i),
+function Mi(e, t, n, i) {
+    var r = ea(i) ? i : n(i),
         s = t.get(r);
     return typeof s > "u" && (s = e.call(this, i), t.set(r, s)), s;
 }
 
 function Ri(e, t, n) {
     var i = Array.prototype.slice.call(arguments, 3),
         r = n(i),
         s = t.get(r);
     return typeof s > "u" && (s = e.apply(this, i), t.set(r, s)), s;
 }
 
-function hn(e, t, n, i, r) {
+function cn(e, t, n, i, r) {
     return n.bind(t, e, i, r);
 }
 
-function Jo(e, t) {
-    var n = e.length === 1 ? Li : Ri;
-    return hn(e, this, n, t.cache.create(), t.serializer);
+function ta(e, t) {
+    var n = e.length === 1 ? Mi : Ri;
+    return cn(e, this, n, t.cache.create(), t.serializer);
 }
 
-function Ko(e, t) {
-    return hn(e, this, Ri, t.cache.create(), t.serializer);
+function na(e, t) {
+    return cn(e, this, Ri, t.cache.create(), t.serializer);
 }
 
-function $o(e, t) {
-    return hn(e, this, Li, t.cache.create(), t.serializer);
+function ia(e, t) {
+    return cn(e, this, Mi, t.cache.create(), t.serializer);
 }
-var ea = function() {
+var ra = function() {
     return JSON.stringify(arguments);
 };
 
-function cn() {
+function mn() {
     this.cache = /* @__PURE__ */ Object.create(null);
 }
-cn.prototype.get = function(e) {
+mn.prototype.get = function(e) {
     return this.cache[e];
 };
-cn.prototype.set = function(e, t) {
+mn.prototype.set = function(e, t) {
     this.cache[e] = t;
 };
-var ta = {
+var sa = {
         create: function() {
-            return new cn();
+            return new mn();
         }
     },
-    Ut = {
-        variadic: Ko,
-        monadic: $o
+    Gt = {
+        variadic: na,
+        monadic: ia
     },
-    He;
+    Ae;
 (function(e) {
     e.MISSING_VALUE = "MISSING_VALUE", e.INVALID_VALUE = "INVALID_VALUE", e.MISSING_INTL_API = "MISSING_INTL_API";
-})(He || (He = {}));
-var Et = (
+})(Ae || (Ae = {}));
+var xt = (
         /** @class */
         function(e) {
-            yt(t, e);
+            wt(t, e);
 
             function t(n, i, r) {
                 var s = e.call(this, n) || this;
                 return s.code = i, s.originalMessage = r, s;
             }
             return t.prototype.toString = function() {
                 return "[formatjs Error: ".concat(this.code, "] ").concat(this.message);
             }, t;
         }(Error)
     ),
     Xn = (
         /** @class */
         function(e) {
-            yt(t, e);
+            wt(t, e);
 
             function t(n, i, r, s) {
-                return e.call(this, 'Invalid values for "'.concat(n, '": "').concat(i, '". Options are "').concat(Object.keys(r).join('", "'), '"'), He.INVALID_VALUE, s) || this;
+                return e.call(this, 'Invalid values for "'.concat(n, '": "').concat(i, '". Options are "').concat(Object.keys(r).join('", "'), '"'), Ae.INVALID_VALUE, s) || this;
             }
             return t;
-        }(Et)
+        }(xt)
     ),
-    na = (
+    oa = (
         /** @class */
         function(e) {
-            yt(t, e);
+            wt(t, e);
 
             function t(n, i, r) {
-                return e.call(this, 'Value for "'.concat(n, '" must be of type ').concat(i), He.INVALID_VALUE, r) || this;
+                return e.call(this, 'Value for "'.concat(n, '" must be of type ').concat(i), Ae.INVALID_VALUE, r) || this;
             }
             return t;
-        }(Et)
+        }(xt)
     ),
-    ia = (
+    aa = (
         /** @class */
         function(e) {
-            yt(t, e);
+            wt(t, e);
 
             function t(n, i) {
-                return e.call(this, 'The intl string context variable "'.concat(n, '" was not provided to the string "').concat(i, '"'), He.MISSING_VALUE, i) || this;
+                return e.call(this, 'The intl string context variable "'.concat(n, '" was not provided to the string "').concat(i, '"'), Ae.MISSING_VALUE, i) || this;
             }
             return t;
-        }(Et)
+        }(xt)
     ),
     U;
 (function(e) {
     e[e.literal = 0] = "literal", e[e.object = 1] = "object";
 })(U || (U = {}));
 
-function ra(e) {
+function la(e) {
     return e.length < 2 ? e : e.reduce(function(t, n) {
         var i = t[t.length - 1];
         return !i || i.type !== U.literal || n.type !== U.literal ? t.push(n) : i.value += n.value, t;
     }, []);
 }
 
-function sa(e) {
+function ua(e) {
     return typeof e == "function";
 }
 
-function ut(e, t, n, i, r, s, u) {
+function ht(e, t, n, i, r, s, u) {
     if (e.length === 1 && kn(e[0]))
         return [{
             type: U.literal,
             value: e[0].value
         }];
     for (var o = [], a = 0, f = e; a < f.length; a++) {
         var l = f[a];
         if (kn(l)) {
             o.push({
                 type: U.literal,
                 value: l.value
             });
             continue;
         }
-        if (Eo(l)) {
+        if (Ho(l)) {
             typeof s == "number" && o.push({
                 type: U.literal,
                 value: n.getNumberFormat(t).format(s)
             });
             continue;
         }
         var h = l.value;
         if (!(r && h in r))
-            throw new ia(h, u);
-        var c = r[h];
-        if (yo(l)) {
-            (!c || typeof c == "string" || typeof c == "number") && (c = typeof c == "string" || typeof c == "number" ? String(c) : ""), o.push({
-                type: typeof c == "string" ? U.literal : U.object,
-                value: c
+            throw new aa(h, u);
+        var m = r[h];
+        if (So(l)) {
+            (!m || typeof m == "string" || typeof m == "number") && (m = typeof m == "string" || typeof m == "number" ? String(m) : ""), o.push({
+                type: typeof m == "string" ? U.literal : U.object,
+                value: m
             });
             continue;
         }
         if (wi(l)) {
-            var _ = typeof l.style == "string" ? i.date[l.style] : Qt(l.style) ? l.style.parsedOptions : void 0;
+            var _ = typeof l.style == "string" ? i.date[l.style] : Jt(l.style) ? l.style.parsedOptions : void 0;
             o.push({
                 type: U.literal,
-                value: n.getDateTimeFormat(t, _).format(c)
+                value: n.getDateTimeFormat(t, _).format(m)
             });
             continue;
         }
         if (xi(l)) {
-            var _ = typeof l.style == "string" ? i.time[l.style] : Qt(l.style) ? l.style.parsedOptions : i.time.medium;
+            var _ = typeof l.style == "string" ? i.time[l.style] : Jt(l.style) ? l.style.parsedOptions : i.time.medium;
             o.push({
                 type: U.literal,
-                value: n.getDateTimeFormat(t, _).format(c)
+                value: n.getDateTimeFormat(t, _).format(m)
             });
             continue;
         }
         if (Ei(l)) {
             var _ = typeof l.style == "string" ? i.number[l.style] : Bi(l.style) ? l.style.parsedOptions : void 0;
-            _ && _.scale && (c = c * (_.scale || 1)), o.push({
+            _ && _.scale && (m = m * (_.scale || 1)), o.push({
                 type: U.literal,
-                value: n.getNumberFormat(t, _).format(c)
+                value: n.getNumberFormat(t, _).format(m)
             });
             continue;
         }
         if (Ai(l)) {
-            var g = l.children,
-                m = l.value,
-                d = r[m];
-            if (!sa(d))
-                throw new na(m, "function", u);
-            var b = ut(g, t, n, i, r, s),
-                y = d(b.map(function(T) {
-                    return T.value;
+            var b = l.children,
+                g = l.value,
+                d = r[g];
+            if (!ua(d))
+                throw new oa(g, "function", u);
+            var c = ht(b, t, n, i, r, s),
+                y = d(c.map(function(C) {
+                    return C.value;
                 }));
-            Array.isArray(y) || (y = [y]), o.push.apply(o, y.map(function(T) {
+            Array.isArray(y) || (y = [y]), o.push.apply(o, y.map(function(C) {
                 return {
-                    type: typeof T == "string" ? U.literal : U.object,
-                    value: T
+                    type: typeof C == "string" ? U.literal : U.object,
+                    value: C
                 };
             }));
         }
         if (Si(l)) {
-            var p = l.options[c] || l.options.other;
+            var p = l.options[m] || l.options.other;
             if (!p)
-                throw new Xn(l.value, c, Object.keys(l.options), u);
-            o.push.apply(o, ut(p.value, t, n, i, r));
+                throw new Xn(l.value, m, Object.keys(l.options), u);
+            o.push.apply(o, ht(p.value, t, n, i, r));
             continue;
         }
         if (Hi(l)) {
-            var p = l.options["=".concat(c)];
+            var p = l.options["=".concat(m)];
             if (!p) {
                 if (!Intl.PluralRules)
-                    throw new Et(`Intl.PluralRules is not available in this environment.
+                    throw new xt(`Intl.PluralRules is not available in this environment.
 Try polyfilling it using "@formatjs/intl-pluralrules"
-`, He.MISSING_INTL_API, u);
+`, Ae.MISSING_INTL_API, u);
                 var B = n.getPluralRules(t, {
                     type: l.pluralType
-                }).select(c - (l.offset || 0));
+                }).select(m - (l.offset || 0));
                 p = l.options[B] || l.options.other;
             }
             if (!p)
-                throw new Xn(l.value, c, Object.keys(l.options), u);
-            o.push.apply(o, ut(p.value, t, n, i, r, c - (l.offset || 0)));
+                throw new Xn(l.value, m, Object.keys(l.options), u);
+            o.push.apply(o, ht(p.value, t, n, i, r, m - (l.offset || 0)));
             continue;
         }
     }
-    return ra(o);
+    return la(o);
 }
 
-function oa(e, t) {
+function fa(e, t) {
     return t ? A(A(A({}, e || {}), t || {}), Object.keys(e).reduce(function(n, i) {
         return n[i] = A(A({}, e[i]), t[i] || {}), n;
     }, {})) : e;
 }
 
-function aa(e, t) {
+function ha(e, t) {
     return t ? Object.keys(e).reduce(function(n, i) {
-        return n[i] = oa(e[i], t[i]), n;
+        return n[i] = fa(e[i], t[i]), n;
     }, A({}, e)) : e;
 }
 
-function Gt(e) {
+function Ft(e) {
     return {
         create: function() {
             return {
                 get: function(t) {
                     return e[t];
                 },
                 set: function(t, n) {
                     e[t] = n;
                 }
             };
         }
     };
 }
 
-function la(e) {
+function ca(e) {
     return e === void 0 && (e = {
         number: {},
         dateTime: {},
         pluralRules: {}
     }), {
-        getNumberFormat: Dt(function() {
+        getNumberFormat: Ut(function() {
             for (var t, n = [], i = 0; i < arguments.length; i++)
                 n[i] = arguments[i];
-            return new((t = Intl.NumberFormat).bind.apply(t, Rt([void 0], n, !1)))();
+            return new((t = Intl.NumberFormat).bind.apply(t, kt([void 0], n, !1)))();
         }, {
-            cache: Gt(e.number),
-            strategy: Ut.variadic
+            cache: Ft(e.number),
+            strategy: Gt.variadic
         }),
-        getDateTimeFormat: Dt(function() {
+        getDateTimeFormat: Ut(function() {
             for (var t, n = [], i = 0; i < arguments.length; i++)
                 n[i] = arguments[i];
-            return new((t = Intl.DateTimeFormat).bind.apply(t, Rt([void 0], n, !1)))();
+            return new((t = Intl.DateTimeFormat).bind.apply(t, kt([void 0], n, !1)))();
         }, {
-            cache: Gt(e.dateTime),
-            strategy: Ut.variadic
+            cache: Ft(e.dateTime),
+            strategy: Gt.variadic
         }),
-        getPluralRules: Dt(function() {
+        getPluralRules: Ut(function() {
             for (var t, n = [], i = 0; i < arguments.length; i++)
                 n[i] = arguments[i];
-            return new((t = Intl.PluralRules).bind.apply(t, Rt([void 0], n, !1)))();
+            return new((t = Intl.PluralRules).bind.apply(t, kt([void 0], n, !1)))();
         }, {
-            cache: Gt(e.pluralRules),
-            strategy: Ut.variadic
+            cache: Ft(e.pluralRules),
+            strategy: Gt.variadic
         })
     };
 }
-var ua = (
+var ma = (
     /** @class */
     function() {
         function e(t, n, i, r) {
             var s = this;
             if (n === void 0 && (n = e.defaultLocale), this.formatterCache = {
                     number: {},
                     dateTime: {},
@@ -4434,15 +4434,15 @@
                     if (o.length === 1)
                         return o[0].value;
                     var a = o.reduce(function(f, l) {
                         return !f.length || l.type !== U.literal || typeof f[f.length - 1] != "string" ? f.push(l.value) : f[f.length - 1] += l.value, f;
                     }, []);
                     return a.length <= 1 ? a[0] || "" : a;
                 }, this.formatToParts = function(u) {
-                    return ut(s.ast, s.locales, s.formatters, s.formats, u, void 0, s.message);
+                    return ht(s.ast, s.locales, s.formatters, s.formats, u, void 0, s.message);
                 }, this.resolvedOptions = function() {
                     return {
                         locale: s.resolvedLocale.toString()
                     };
                 }, this.getAst = function() {
                     return s.ast;
                 }, this.locales = n, this.resolvedLocale = e.resolveLocale(n), typeof t == "string") {
@@ -4452,26 +4452,26 @@
                     ignoreTag: r == null ? void 0 : r.ignoreTag,
                     locale: this.resolvedLocale
                 });
             } else
                 this.ast = t;
             if (!Array.isArray(this.ast))
                 throw new TypeError("A message must be provided as a String or AST.");
-            this.formats = aa(e.formats, i), this.formatters = r && r.formatters || la(this.formatterCache);
+            this.formats = ha(e.formats, i), this.formatters = r && r.formatters || ca(this.formatterCache);
         }
         return Object.defineProperty(e, "defaultLocale", {
             get: function() {
                 return e.memoizedDefaultLocale || (e.memoizedDefaultLocale = new Intl.NumberFormat().resolvedOptions().locale), e.memoizedDefaultLocale;
             },
             enumerable: !1,
             configurable: !0
         }), e.memoizedDefaultLocale = null, e.resolveLocale = function(t) {
             var n = Intl.NumberFormat.supportedLocalesOf(t);
             return n.length > 0 ? new Intl.Locale(n[0]) : new Intl.Locale(typeof t == "string" ? t : t[0]);
-        }, e.__parse = Zo, e.formats = {
+        }, e.__parse = $o, e.formats = {
             number: {
                 integer: {
                     maximumFractionDigits: 0
                 },
                 currency: {
                     style: "currency"
                 },
@@ -4525,15 +4525,15 @@
                     timeZoneName: "short"
                 }
             }
         }, e;
     }()
 );
 
-function fa(e, t) {
+function _a(e, t) {
     if (t == null)
         return;
     if (t in e)
         return e[t];
     const n = t.split(".");
     let i = e;
     for (let r = 0; r < n.length; r++)
@@ -4547,113 +4547,113 @@
             }
             i = i[n[r]];
         } else
             i = void 0;
     return i;
 }
 const se = {},
-    ha = (e, t, n) => n && (t in se || (se[t] = {}), e in se[t] || (se[t][e] = n), n),
+    da = (e, t, n) => n && (t in se || (se[t] = {}), e in se[t] || (se[t][e] = n), n),
     ki = (e, t) => {
         if (t == null)
             return;
         if (t in se && e in se[t])
             return se[t][e];
-        const n = wt(t);
+        const n = St(t);
         for (let i = 0; i < n.length; i++) {
             const r = n[i],
-                s = ma(r, e);
+                s = ga(r, e);
             if (s)
-                return ha(e, t, s);
+                return da(e, t, s);
         }
     };
-let mn;
-const We = pt({});
+let _n;
+const We = yt({});
 
-function ca(e) {
-    return mn[e] || null;
+function ba(e) {
+    return _n[e] || null;
 }
 
 function Di(e) {
-    return e in mn;
+    return e in _n;
 }
 
-function ma(e, t) {
+function ga(e, t) {
     if (!Di(e))
         return null;
-    const n = ca(e);
-    return fa(n, t);
+    const n = ba(e);
+    return _a(n, t);
 }
 
-function _a(e) {
+function pa(e) {
     if (e == null)
         return;
-    const t = wt(e);
+    const t = St(e);
     for (let n = 0; n < t.length; n++) {
         const i = t[n];
         if (Di(i))
             return i;
     }
 }
 
-function da(e, ...t) {
-    delete se[e], We.update((n) => (n[e] = vo.all([n[e] || {}, ...t]), n));
+function va(e, ...t) {
+    delete se[e], We.update((n) => (n[e] = xo.all([n[e] || {}, ...t]), n));
 }
-Be(
+Ce(
     [We],
     ([e]) => Object.keys(e)
 );
-We.subscribe((e) => mn = e);
-const ft = {};
+We.subscribe((e) => _n = e);
+const ct = {};
 
-function ba(e, t) {
-    ft[e].delete(t), ft[e].size === 0 && delete ft[e];
+function ya(e, t) {
+    ct[e].delete(t), ct[e].size === 0 && delete ct[e];
 }
 
 function Ui(e) {
-    return ft[e];
+    return ct[e];
 }
 
-function ga(e) {
-    return wt(e).map((t) => {
+function Ea(e) {
+    return St(e).map((t) => {
         const n = Ui(t);
         return [t, n ? [...n] : []];
     }).filter(([, t]) => t.length > 0);
 }
 
-function nn(e) {
-    return e == null ? !1 : wt(e).some(
+function rn(e) {
+    return e == null ? !1 : St(e).some(
         (t) => {
             var n;
             return (n = Ui(t)) == null ? void 0 : n.size;
         }
     );
 }
 
-function pa(e, t) {
+function wa(e, t) {
     return Promise.all(
-        t.map((i) => (ba(e, i), i().then((r) => r.default || r)))
-    ).then((i) => da(e, ...i));
+        t.map((i) => (ya(e, i), i().then((r) => r.default || r)))
+    ).then((i) => va(e, ...i));
 }
 const Ne = {};
 
 function Gi(e) {
-    if (!nn(e))
+    if (!rn(e))
         return e in Ne ? Ne[e] : Promise.resolve();
-    const t = ga(e);
+    const t = Ea(e);
     return Ne[e] = Promise.all(
         t.map(
-            ([n, i]) => pa(n, i)
+            ([n, i]) => wa(n, i)
         )
     ).then(() => {
-        if (nn(e))
+        if (rn(e))
             return Gi(e);
         delete Ne[e];
     }), Ne[e];
 }
-const va = {
+const xa = {
         number: {
             scientific: {
                 notation: "scientific"
             },
             engineering: {
                 notation: "engineering"
             },
@@ -4709,287 +4709,287 @@
                 hour: "numeric",
                 minute: "numeric",
                 second: "numeric",
                 timeZoneName: "short"
             }
         }
     },
-    ya = {
+    Sa = {
         fallbackLocale: null,
         loadingDelay: 200,
-        formats: va,
+        formats: xa,
         warnOnMissingMessages: !0,
         handleMissingMessage: void 0,
         ignoreTag: !0
     },
-    Ea = ya;
+    Ha = Sa;
 
-function Ae() {
-    return Ea;
+function Be() {
+    return Ha;
 }
-const Ft = pt(!1);
-var wa = Object.defineProperty,
-    xa = Object.defineProperties,
-    Sa = Object.getOwnPropertyDescriptors,
+const zt = yt(!1);
+var Aa = Object.defineProperty,
+    Ba = Object.defineProperties,
+    Ca = Object.getOwnPropertyDescriptors,
     Vn = Object.getOwnPropertySymbols,
-    Ha = Object.prototype.hasOwnProperty,
-    Aa = Object.prototype.propertyIsEnumerable,
-    qn = (e, t, n) => t in e ? wa(e, t, {
+    Ta = Object.prototype.hasOwnProperty,
+    Pa = Object.prototype.propertyIsEnumerable,
+    qn = (e, t, n) => t in e ? Aa(e, t, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
         value: n
     }) : e[t] = n,
-    Ba = (e, t) => {
+    Ia = (e, t) => {
         for (var n in t || (t = {}))
-            Ha.call(t, n) && qn(e, n, t[n]);
+            Ta.call(t, n) && qn(e, n, t[n]);
         if (Vn)
             for (var n of Vn(t))
-                Aa.call(t, n) && qn(e, n, t[n]);
+                Pa.call(t, n) && qn(e, n, t[n]);
         return e;
     },
-    Ta = (e, t) => xa(e, Sa(t));
-let rn;
-const dt = pt(null);
+    Na = (e, t) => Ba(e, Ca(t));
+let sn;
+const gt = yt(null);
 
 function Wn(e) {
     return e.split("-").map((t, n, i) => i.slice(0, n + 1).join("-")).reverse();
 }
 
-function wt(e, t = Ae().fallbackLocale) {
+function St(e, t = Be().fallbackLocale) {
     const n = Wn(e);
     return t ? [... /* @__PURE__ */ new Set([...n, ...Wn(t)])] : n;
 }
 
 function ue() {
-    return rn ?? void 0;
+    return sn ?? void 0;
 }
-dt.subscribe((e) => {
-    rn = e ?? void 0, typeof window < "u" && e != null && document.documentElement.setAttribute("lang", e);
+gt.subscribe((e) => {
+    sn = e ?? void 0, typeof window < "u" && e != null && document.documentElement.setAttribute("lang", e);
 });
-const Ca = (e) => {
-        if (e && _a(e) && nn(e)) {
+const Oa = (e) => {
+        if (e && pa(e) && rn(e)) {
             const {
                 loadingDelay: t
-            } = Ae();
+            } = Be();
             let n;
             return typeof window < "u" && ue() != null && t ? n = window.setTimeout(
-                () => Ft.set(!0),
+                () => zt.set(!0),
                 t
-            ) : Ft.set(!0), Gi(e).then(() => {
-                dt.set(e);
+            ) : zt.set(!0), Gi(e).then(() => {
+                gt.set(e);
             }).finally(() => {
-                clearTimeout(n), Ft.set(!1);
+                clearTimeout(n), zt.set(!1);
             });
         }
-        return dt.set(e);
+        return gt.set(e);
     },
-    Ye = Ta(Ba({}, dt), {
-        set: Ca
+    Ye = Na(Ia({}, gt), {
+        set: Oa
     }),
-    xt = (e) => {
+    Ht = (e) => {
         const t = /* @__PURE__ */ Object.create(null);
         return (i) => {
             const r = JSON.stringify(i);
             return r in t ? t[r] : t[r] = e(i);
         };
     };
-var Pa = Object.defineProperty,
-    bt = Object.getOwnPropertySymbols,
+var La = Object.defineProperty,
+    pt = Object.getOwnPropertySymbols,
     Fi = Object.prototype.hasOwnProperty,
     zi = Object.prototype.propertyIsEnumerable,
-    Yn = (e, t, n) => t in e ? Pa(e, t, {
+    Yn = (e, t, n) => t in e ? La(e, t, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
         value: n
     }) : e[t] = n,
-    _n = (e, t) => {
+    dn = (e, t) => {
         for (var n in t || (t = {}))
             Fi.call(t, n) && Yn(e, n, t[n]);
-        if (bt)
-            for (var n of bt(t))
+        if (pt)
+            for (var n of pt(t))
                 zi.call(t, n) && Yn(e, n, t[n]);
         return e;
     },
     Te = (e, t) => {
         var n = {};
         for (var i in e)
             Fi.call(e, i) && t.indexOf(i) < 0 && (n[i] = e[i]);
-        if (e != null && bt)
-            for (var i of bt(e))
+        if (e != null && pt)
+            for (var i of pt(e))
                 t.indexOf(i) < 0 && zi.call(e, i) && (n[i] = e[i]);
         return n;
     };
 const je = (e, t) => {
         const {
             formats: n
-        } = Ae();
+        } = Be();
         if (e in n && t in n[e])
             return n[e][t];
         throw new Error(`[svelte-i18n] Unknown "${t}" ${e} format.`);
     },
-    Ia = xt(
+    Ma = Ht(
         (e) => {
             var t = e,
                 {
                     locale: n,
                     format: i
                 } = t,
                 r = Te(t, ["locale", "format"]);
             if (n == null)
                 throw new Error('[svelte-i18n] A "locale" must be set to format numbers');
             return i && (r = je("number", i)), new Intl.NumberFormat(n, r);
         }
     ),
-    Na = xt(
+    Ra = Ht(
         (e) => {
             var t = e,
                 {
                     locale: n,
                     format: i
                 } = t,
                 r = Te(t, ["locale", "format"]);
             if (n == null)
                 throw new Error('[svelte-i18n] A "locale" must be set to format dates');
             return i ? r = je("date", i) : Object.keys(r).length === 0 && (r = je("date", "short")), new Intl.DateTimeFormat(n, r);
         }
     ),
-    Oa = xt(
+    ka = Ht(
         (e) => {
             var t = e,
                 {
                     locale: n,
                     format: i
                 } = t,
                 r = Te(t, ["locale", "format"]);
             if (n == null)
                 throw new Error(
                     '[svelte-i18n] A "locale" must be set to format time values'
                 );
             return i ? r = je("time", i) : Object.keys(r).length === 0 && (r = je("time", "short")), new Intl.DateTimeFormat(n, r);
         }
     ),
-    Ma = (e = {}) => {
+    Da = (e = {}) => {
         var t = e,
             {
                 locale: n = ue()
             } = t,
             i = Te(t, [
                 "locale"
             ]);
-        return Ia(_n({
+        return Ma(dn({
             locale: n
         }, i));
     },
-    La = (e = {}) => {
+    Ua = (e = {}) => {
         var t = e,
             {
                 locale: n = ue()
             } = t,
             i = Te(t, [
                 "locale"
             ]);
-        return Na(_n({
+        return Ra(dn({
             locale: n
         }, i));
     },
-    Ra = (e = {}) => {
+    Ga = (e = {}) => {
         var t = e,
             {
                 locale: n = ue()
             } = t,
             i = Te(t, [
                 "locale"
             ]);
-        return Oa(_n({
+        return ka(dn({
             locale: n
         }, i));
     },
-    ka = xt(
+    Fa = Ht(
         // eslint-disable-next-line @typescript-eslint/no-non-null-assertion
-        (e, t = ue()) => new ua(e, t, Ae().formats, {
-            ignoreTag: Ae().ignoreTag
+        (e, t = ue()) => new ma(e, t, Be().formats, {
+            ignoreTag: Be().ignoreTag
         })
     ),
-    Da = (e, t = {}) => {
+    za = (e, t = {}) => {
         var n, i, r, s;
         let u = t;
         typeof e == "object" && (u = e, e = u.id);
         const {
             values: o,
             locale: a = ue(),
             default: f
         } = u;
         if (a == null)
             throw new Error(
                 "[svelte-i18n] Cannot format a message without first setting the initial locale."
             );
         let l = ki(e, a);
         if (!l)
-            l = (s = (r = (i = (n = Ae()).handleMissingMessage) == null ? void 0 : i.call(n, {
+            l = (s = (r = (i = (n = Be()).handleMissingMessage) == null ? void 0 : i.call(n, {
                 locale: a,
                 id: e,
                 defaultValue: f
             })) != null ? r : f) != null ? s : e;
         else if (typeof l != "string")
             return console.warn(
                 `[svelte-i18n] Message with id "${e}" must be of type "string", found: "${typeof l}". Gettin its value through the "$format" method is deprecated; use the "json" method instead.`
             ), l;
         if (!o)
             return l;
         let h = l;
         try {
-            h = ka(l, a).format(o);
-        } catch (c) {
-            c instanceof Error && console.warn(
+            h = Fa(l, a).format(o);
+        } catch (m) {
+            m instanceof Error && console.warn(
                 `[svelte-i18n] Message "${e}" has syntax error:`,
-                c.message
+                m.message
             );
         }
         return h;
     },
-    Ua = (e, t) => Ra(t).format(e),
-    Ga = (e, t) => La(t).format(e),
-    Fa = (e, t) => Ma(t).format(e),
-    za = (e, t = ue()) => ki(e, t);
-Be([Ye, We], () => Da);
-Be([Ye], () => Ua);
-Be([Ye], () => Ga);
-Be([Ye], () => Fa);
-Be([Ye, We], () => za);
+    ja = (e, t) => Ga(t).format(e),
+    Xa = (e, t) => Ua(t).format(e),
+    Va = (e, t) => Da(t).format(e),
+    qa = (e, t = ue()) => ki(e, t);
+Ce([Ye, We], () => za);
+Ce([Ye], () => ja);
+Ce([Ye], () => Xa);
+Ce([Ye], () => Va);
+Ce([Ye, We], () => qa);
 const {
-    SvelteComponent: ja,
+    SvelteComponent: Wa,
     add_render_callback: ji,
-    append: Je,
+    append: $e,
     attr: j,
     binding_callbacks: Zn,
-    check_outros: Xa,
+    check_outros: Ya,
     create_bidirectional_transition: Qn,
-    destroy_each: Va,
+    destroy_each: Za,
     detach: Re,
-    element: gt,
-    empty: qa,
+    element: vt,
+    empty: Qa,
     ensure_array_like: Jn,
-    group_outros: Wa,
-    init: Ya,
+    group_outros: Ja,
+    init: Ka,
     insert: ke,
-    listen: sn,
-    prevent_default: Za,
-    run_all: Qa,
-    safe_not_equal: Ja,
-    set_data: Ka,
-    set_style: me,
-    space: on,
-    text: $a,
+    listen: on,
+    prevent_default: $a,
+    run_all: el,
+    safe_not_equal: tl,
+    set_data: nl,
+    set_style: _e,
+    space: an,
+    text: il,
     toggle_class: Q,
-    transition_in: zt,
+    transition_in: jt,
     transition_out: Kn
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: el
+    createEventDispatcher: rl
 } = window.__gradio__svelte__internal;
 
 function $n(e, t, n) {
     const i = e.slice();
     return i[24] = t[n], i;
 }
 
@@ -4999,35 +4999,35 @@
             e[1]
         ),
         o = [];
     for (let a = 0; a < u.length; a += 1)
         o[a] = ti($n(e, u, a));
     return {
         c() {
-            t = gt("ul");
+            t = vt("ul");
             for (let a = 0; a < o.length; a += 1)
                 o[a].c();
-            j(t, "class", "options svelte-yuohum"), j(t, "role", "listbox"), me(
+            j(t, "class", "options svelte-yuohum"), j(t, "role", "listbox"), _e(
                 t,
                 "bottom",
                 /*bottom*/
                 e[9]
-            ), me(t, "max-height", `calc(${/*max_height*/
-      e[10]}px - var(--window-padding))`), me(
+            ), _e(t, "max-height", `calc(${/*max_height*/
+      e[10]}px - var(--window-padding))`), _e(
                 t,
                 "width",
                 /*input_width*/
                 e[8] + "px"
             );
         },
         m(a, f) {
             ke(a, t, f);
             for (let l = 0; l < o.length; l += 1)
                 o[l] && o[l].m(t, null);
-            e[20](t), i = !0, r || (s = sn(t, "mousedown", Za(
+            e[20](t), i = !0, r || (s = on(t, "mousedown", $a(
                 /*mousedown_handler*/
                 e[19]
             )), r = !0);
         },
         p(a, f) {
             if (f & /*filtered_indices, choices, selected_indices, active_index*/
                 51) {
@@ -5041,23 +5041,23 @@
                     o[l] ? o[l].p(h, f) : (o[l] = ti(h), o[l].c(), o[l].m(t, null));
                 }
                 for (; l < o.length; l += 1)
                     o[l].d(1);
                 o.length = u.length;
             }
             f & /*bottom*/
-                512 && me(
+                512 && _e(
                     t,
                     "bottom",
                     /*bottom*/
                     a[9]
                 ), f & /*max_height*/
-                1024 && me(t, "max-height", `calc(${/*max_height*/
+                1024 && _e(t, "max-height", `calc(${/*max_height*/
       a[10]}px - var(--window-padding))`), f & /*input_width*/
-                256 && me(
+                256 && _e(
                     t,
                     "width",
                     /*input_width*/
                     a[8] + "px"
                 );
         },
         i(a) {
@@ -5071,15 +5071,15 @@
         o(a) {
             a && (n || (n = Qn(t, Nn, {
                 duration: 200,
                 y: 5
             }, !1)), n.run(0)), i = !1;
         },
         d(a) {
-            a && Re(t), Va(o, a), e[20](null), a && n && n.end(), r = !1, s();
+            a && Re(t), Za(o, a), e[20](null), a && n && n.end(), r = !1, s();
         }
     };
 }
 
 function ti(e) {
     let t, n, i, r = (
             /*choices*/
@@ -5087,15 +5087,15 @@
                 /*index*/
                 e[24]
             ][0] + ""
         ),
         s, u, o, a, f;
     return {
         c() {
-            t = gt("li"), n = gt("span"), n.textContent = "✓", i = on(), s = $a(r), u = on(), j(n, "class", "inner-item svelte-yuohum"), Q(n, "hide", ! /*selected_indices*/
+            t = vt("li"), n = vt("span"), n.textContent = "✓", i = an(), s = il(r), u = an(), j(n, "class", "inner-item svelte-yuohum"), Q(n, "hide", ! /*selected_indices*/
                 e[4].includes(
                     /*index*/
                     e[24]
                 )), j(t, "class", "item svelte-yuohum"), j(t, "data-index", o = /*index*/
                 e[24]), j(t, "aria-label", a = /*choices*/
                 e[0][
                     /*index*/
@@ -5129,28 +5129,28 @@
                 "dark:bg-gray-600",
                 /*index*/
                 e[24] === /*active_index*/
                 e[5]
             );
         },
         m(l, h) {
-            ke(l, t, h), Je(t, n), Je(t, i), Je(t, s), Je(t, u);
+            ke(l, t, h), $e(t, n), $e(t, i), $e(t, s), $e(t, u);
         },
         p(l, h) {
             h & /*selected_indices, filtered_indices*/
                 18 && Q(n, "hide", ! /*selected_indices*/
                     l[4].includes(
                         /*index*/
                         l[24]
                     )), h & /*choices, filtered_indices*/
                 3 && r !== (r = /*choices*/
                     l[0][
                         /*index*/
                         l[24]
-                    ][0] + "") && Ka(s, r), h & /*filtered_indices*/
+                    ][0] + "") && nl(s, r), h & /*filtered_indices*/
                 2 && o !== (o = /*index*/
                     l[24]) && j(t, "data-index", o), h & /*choices, filtered_indices*/
                 3 && a !== (a = /*choices*/
                     l[0][
                         /*index*/
                         l[24]
                     ][0]) && j(t, "aria-label", a), h & /*selected_indices, filtered_indices*/
@@ -5192,325 +5192,325 @@
         },
         d(l) {
             l && Re(t);
         }
     };
 }
 
-function tl(e) {
+function sl(e) {
     let t, n, i, r, s;
     ji(
         /*onwindowresize*/
         e[17]
     );
     let u = (
         /*show_options*/
         e[2] && ! /*disabled*/
         e[3] && ei(e)
     );
     return {
         c() {
-            t = gt("div"), n = on(), u && u.c(), i = qa(), j(t, "class", "reference");
+            t = vt("div"), n = an(), u && u.c(), i = Qa(), j(t, "class", "reference");
         },
         m(o, a) {
             ke(o, t, a), e[18](t), ke(o, n, a), u && u.m(o, a), ke(o, i, a), r || (s = [
-                sn(
+                on(
                     window,
                     "scroll",
                     /*scroll_listener*/
                     e[12]
                 ),
-                sn(
+                on(
                     window,
                     "resize",
                     /*onwindowresize*/
                     e[17]
                 )
             ], r = !0);
         },
         p(o, [a]) {
             /*show_options*/
             o[2] && ! /*disabled*/
                 o[3] ? u ? (u.p(o, a), a & /*show_options, disabled*/
-                    12 && zt(u, 1)) : (u = ei(o), u.c(), zt(u, 1), u.m(i.parentNode, i)) : u && (Wa(), Kn(u, 1, 1, () => {
+                    12 && jt(u, 1)) : (u = ei(o), u.c(), jt(u, 1), u.m(i.parentNode, i)) : u && (Ja(), Kn(u, 1, 1, () => {
                     u = null;
-                }), Xa());
+                }), Ya());
         },
         i(o) {
-            zt(u);
+            jt(u);
         },
         o(o) {
             Kn(u);
         },
         d(o) {
-            o && (Re(t), Re(n), Re(i)), e[18](null), u && u.d(o), r = !1, Qa(s);
+            o && (Re(t), Re(n), Re(i)), e[18](null), u && u.d(o), r = !1, el(s);
         }
     };
 }
 
-function Ke(e) {
+function et(e) {
     let t, n = e[0],
         i = 1;
     for (; i < e.length;) {
         const r = e[i],
             s = e[i + 1];
         if (i += 2, (r === "optionalAccess" || r === "optionalCall") && n == null)
             return;
         r === "access" || r === "optionalAccess" ? (t = n, n = s(n)) : (r === "call" || r === "optionalCall") && (n = s((...u) => n.call(t, ...u)), t = void 0);
     }
     return n;
 }
 
-function nl(e, t, n) {
+function ol(e, t, n) {
     let {
         choices: i
     } = t, {
         filtered_indices: r
     } = t, {
         show_options: s = !1
     } = t, {
         disabled: u = !1
     } = t, {
         selected_indices: o = []
     } = t, {
         active_index: a = null
-    } = t, f, l, h, c, _, g, m, d, b;
+    } = t, f, l, h, m, _, b, g, d, c;
 
     function y() {
         const {
             top: x,
-            bottom: L
+            bottom: M
         } = _.getBoundingClientRect();
-        n(14, f = x), n(15, l = b - L);
+        n(14, f = x), n(15, l = c - M);
     }
     let p = null;
 
     function B() {
         s && (p !== null && clearTimeout(p), p = setTimeout(
             () => {
                 y(), p = null;
             },
             10
         ));
     }
-    const T = el();
+    const C = rl();
 
     function O() {
-        n(11, b = window.innerHeight);
+        n(11, c = window.innerHeight);
     }
 
-    function C(x) {
+    function T(x) {
         Zn[x ? "unshift" : "push"](() => {
             _ = x, n(6, _);
         });
     }
-    const w = (x) => T("change", x);
+    const E = (x) => C("change", x);
 
     function k(x) {
         Zn[x ? "unshift" : "push"](() => {
-            g = x, n(7, g);
+            b = x, n(7, b);
         });
     }
     return e.$$set = (x) => {
         "choices" in x && n(0, i = x.choices), "filtered_indices" in x && n(1, r = x.filtered_indices), "show_options" in x && n(2, s = x.show_options), "disabled" in x && n(3, u = x.disabled), "selected_indices" in x && n(4, o = x.selected_indices), "active_index" in x && n(5, a = x.active_index);
     }, e.$$.update = () => {
         if (e.$$.dirty & /*show_options, refElement, listElement, selected_indices, distance_from_bottom, distance_from_top, input_height*/
             114900) {
             if (s && _) {
-                if (g && o.length > 0) {
-                    let L = g.querySelectorAll("li");
-                    for (const W of Array.from(L))
+                if (b && o.length > 0) {
+                    let M = b.querySelectorAll("li");
+                    for (const W of Array.from(M))
                         if (W.getAttribute("data-index") === o[0].toString()) {
-                            Ke([
-                                g,
+                            et([
+                                b,
                                 "optionalAccess",
                                 (ee) => ee.scrollTo,
                                 "optionalCall",
                                 (ee) => ee(0, W.offsetTop)
                             ]);
                             break;
                         }
                 }
                 y();
-                const x = Ke([
+                const x = et([
                     _,
                     "access",
-                    (L) => L.parentElement,
+                    (M) => M.parentElement,
                     "optionalAccess",
-                    (L) => L.getBoundingClientRect,
+                    (M) => M.getBoundingClientRect,
                     "call",
-                    (L) => L()
+                    (M) => M()
                 ]);
-                n(16, h = Ke([x, "optionalAccess", (L) => L.height]) || 0), n(8, c = Ke([x, "optionalAccess", (L) => L.width]) || 0);
+                n(16, h = et([x, "optionalAccess", (M) => M.height]) || 0), n(8, m = et([x, "optionalAccess", (M) => M.width]) || 0);
             }
-            l > f ? (n(10, d = l), n(9, m = null)) : (n(9, m = `${l + h}px`), n(10, d = f - h));
+            l > f ? (n(10, d = l), n(9, g = null)) : (n(9, g = `${l + h}px`), n(10, d = f - h));
         }
     }, [
         i,
         r,
         s,
         u,
         o,
         a,
         _,
-        g,
-        c,
+        b,
         m,
+        g,
         d,
-        b,
+        c,
         B,
-        T,
+        C,
         f,
         l,
         h,
         O,
-        C,
-        w,
+        T,
+        E,
         k
     ];
 }
-class il extends ja {
+class al extends Wa {
     constructor(t) {
-        super(), Ya(this, t, nl, tl, Ja, {
+        super(), Ka(this, t, ol, sl, tl, {
             choices: 0,
             filtered_indices: 1,
             show_options: 2,
             disabled: 3,
             selected_indices: 4,
             active_index: 5
         });
     }
 }
 
-function rl(e, t) {
+function ll(e, t) {
     return (e % t + t) % t;
 }
 
 function ni(e, t) {
     return e.reduce((n, i, r) => ((!t || i[0].toLowerCase().includes(t.toLowerCase())) && n.push(r), n), []);
 }
 
-function sl(e, t, n) {
+function ul(e, t, n) {
     e("change", t), n || e("input");
 }
 
-function ol(e, t, n) {
+function fl(e, t, n) {
     if (e.key === "Escape")
         return [!1, t];
     if ((e.key === "ArrowDown" || e.key === "ArrowUp") && n.length >= 0)
         if (t === null)
             t = e.key === "ArrowDown" ? n[0] : n[n.length - 1];
         else {
             const i = n.indexOf(t),
                 r = e.key === "ArrowUp" ? -1 : 1;
-            t = n[rl(i + r, n.length)];
+            t = n[ll(i + r, n.length)];
         }
     return [!0, t];
 }
 const {
-    SvelteComponent: al,
+    SvelteComponent: hl,
     append: oe,
     attr: z,
-    binding_callbacks: ll,
-    check_outros: ul,
-    create_component: an,
-    destroy_component: ln,
-    detach: dn,
-    element: de,
-    group_outros: fl,
-    init: hl,
-    insert: bn,
+    binding_callbacks: cl,
+    check_outros: ml,
+    create_component: ln,
+    destroy_component: un,
+    detach: bn,
+    element: be,
+    group_outros: _l,
+    init: dl,
+    insert: gn,
     listen: Oe,
-    mount_component: un,
-    run_all: cl,
-    safe_not_equal: ml,
-    set_data: _l,
+    mount_component: fn,
+    run_all: bl,
+    safe_not_equal: gl,
+    set_data: pl,
     set_input_value: ii,
-    space: jt,
-    text: dl,
-    toggle_class: _e,
-    transition_in: be,
-    transition_out: Le
+    space: Xt,
+    text: vl,
+    toggle_class: de,
+    transition_in: ge,
+    transition_out: Me
 } = window.__gradio__svelte__internal, {
-    onMount: bl
+    onMount: yl
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: gl,
-    afterUpdate: pl
+    createEventDispatcher: El,
+    afterUpdate: wl
 } = window.__gradio__svelte__internal;
 
-function vl(e) {
+function xl(e) {
     let t;
     return {
         c() {
-            t = dl(
+            t = vl(
                 /*label*/
                 e[0]
             );
         },
         m(n, i) {
-            bn(n, t, i);
+            gn(n, t, i);
         },
         p(n, i) {
             i[0] & /*label*/
-                1 && _l(
+                1 && pl(
                     t,
                     /*label*/
                     n[0]
                 );
         },
         d(n) {
-            n && dn(t);
+            n && bn(t);
         }
     };
 }
 
 function ri(e) {
     let t, n, i;
-    return n = new Er({}), {
+    return n = new Hr({}), {
         c() {
-            t = de("div"), an(n.$$.fragment), z(t, "class", "icon-wrap svelte-1m1zvyj");
+            t = be("div"), ln(n.$$.fragment), z(t, "class", "icon-wrap svelte-1m1zvyj");
         },
         m(r, s) {
-            bn(r, t, s), un(n, t, null), i = !0;
+            gn(r, t, s), fn(n, t, null), i = !0;
         },
         i(r) {
-            i || (be(n.$$.fragment, r), i = !0);
+            i || (ge(n.$$.fragment, r), i = !0);
         },
         o(r) {
-            Le(n.$$.fragment, r), i = !1;
+            Me(n.$$.fragment, r), i = !1;
         },
         d(r) {
-            r && dn(t), ln(n);
+            r && bn(t), un(n);
         }
     };
 }
 
-function yl(e) {
-    let t, n, i, r, s, u, o, a, f, l, h, c, _, g;
+function Sl(e) {
+    let t, n, i, r, s, u, o, a, f, l, h, m, _, b;
     n = new hi({
         props: {
             show_label: (
                 /*show_label*/
                 e[4]
             ),
             info: (
                 /*info*/
                 e[1]
             ),
             $$slots: {
-                default: [vl]
+                default: [xl]
             },
             $$scope: {
                 ctx: e
             }
         }
     });
-    let m = ! /*disabled*/
+    let g = ! /*disabled*/
         e[3] && ri();
-    return h = new il({
+    return h = new al({
         props: {
             show_options: (
                 /*show_options*/
                 e[12]
             ),
             choices: (
                 /*choices*/
@@ -5538,49 +5538,49 @@
         }
     }), h.$on(
         "change",
         /*handle_option_selected*/
         e[16]
     ), {
         c() {
-            t = de("div"), an(n.$$.fragment), i = jt(), r = de("div"), s = de("div"), u = de("div"), o = de("input"), f = jt(), m && m.c(), l = jt(), an(h.$$.fragment), z(o, "role", "listbox"), z(o, "aria-controls", "dropdown-options"), z(
+            t = be("div"), ln(n.$$.fragment), i = Xt(), r = be("div"), s = be("div"), u = be("div"), o = be("input"), f = Xt(), g && g.c(), l = Xt(), ln(h.$$.fragment), z(o, "role", "listbox"), z(o, "aria-controls", "dropdown-options"), z(
                     o,
                     "aria-expanded",
                     /*show_options*/
                     e[12]
                 ), z(
                     o,
                     "aria-label",
                     /*label*/
                     e[0]
                 ), z(o, "class", "border-none svelte-1m1zvyj"), o.disabled = /*disabled*/
                 e[3], z(o, "autocomplete", "off"), o.readOnly = a = ! /*filterable*/
-                e[7], _e(o, "subdued", ! /*choices_names*/
+                e[7], de(o, "subdued", ! /*choices_names*/
                     e[13].includes(
                         /*input_text*/
                         e[9]
                     ) && ! /*allow_custom_value*/
-                    e[6]), z(u, "class", "secondary-wrap svelte-1m1zvyj"), z(s, "class", "wrap-inner svelte-1m1zvyj"), _e(
+                    e[6]), z(u, "class", "secondary-wrap svelte-1m1zvyj"), z(s, "class", "wrap-inner svelte-1m1zvyj"), de(
                     s,
                     "show_options",
                     /*show_options*/
                     e[12]
-                ), z(r, "class", "wrap svelte-1m1zvyj"), z(t, "class", "svelte-1m1zvyj"), _e(
+                ), z(r, "class", "wrap svelte-1m1zvyj"), z(t, "class", "svelte-1m1zvyj"), de(
                     t,
                     "container",
                     /*container*/
                     e[5]
                 );
         },
-        m(d, b) {
-            bn(d, t, b), un(n, t, null), oe(t, i), oe(t, r), oe(r, s), oe(s, u), oe(u, o), ii(
+        m(d, c) {
+            gn(d, t, c), fn(n, t, null), oe(t, i), oe(t, r), oe(r, s), oe(s, u), oe(u, o), ii(
                 o,
                 /*input_text*/
                 e[9]
-            ), e[29](o), oe(u, f), m && m.m(u, null), oe(r, l), un(h, r, null), c = !0, _ || (g = [
+            ), e[29](o), oe(u, f), g && g.m(u, null), oe(r, l), fn(h, r, null), m = !0, _ || (b = [
                 Oe(
                     o,
                     "input",
                     /*input_input_handler*/
                     e[28]
                 ),
                 Oe(
@@ -5605,101 +5605,101 @@
                     o,
                     "focus",
                     /*handle_focus*/
                     e[17]
                 )
             ], _ = !0);
         },
-        p(d, b) {
+        p(d, c) {
             const y = {};
-            b[0] & /*show_label*/
+            c[0] & /*show_label*/
                 16 && (y.show_label = /*show_label*/
-                    d[4]), b[0] & /*info*/
+                    d[4]), c[0] & /*info*/
                 2 && (y.info = /*info*/
-                    d[1]), b[0] & /*label*/
-                1 | b[1] & /*$$scope*/
+                    d[1]), c[0] & /*label*/
+                1 | c[1] & /*$$scope*/
                 4 && (y.$$scope = {
-                    dirty: b,
+                    dirty: c,
                     ctx: d
-                }), n.$set(y), (!c || b[0] & /*show_options*/
+                }), n.$set(y), (!m || c[0] & /*show_options*/
                     4096) && z(
                     o,
                     "aria-expanded",
                     /*show_options*/
                     d[12]
-                ), (!c || b[0] & /*label*/
+                ), (!m || c[0] & /*label*/
                     1) && z(
                     o,
                     "aria-label",
                     /*label*/
                     d[0]
-                ), (!c || b[0] & /*disabled*/
+                ), (!m || c[0] & /*disabled*/
                     8) && (o.disabled = /*disabled*/
-                    d[3]), (!c || b[0] & /*filterable*/
+                    d[3]), (!m || c[0] & /*filterable*/
                     128 && a !== (a = ! /*filterable*/
-                        d[7])) && (o.readOnly = a), b[0] & /*input_text*/
+                        d[7])) && (o.readOnly = a), c[0] & /*input_text*/
                 512 && o.value !== /*input_text*/
                 d[9] && ii(
                     o,
                     /*input_text*/
                     d[9]
-                ), (!c || b[0] & /*choices_names, input_text, allow_custom_value*/
-                    8768) && _e(o, "subdued", ! /*choices_names*/
+                ), (!m || c[0] & /*choices_names, input_text, allow_custom_value*/
+                    8768) && de(o, "subdued", ! /*choices_names*/
                     d[13].includes(
                         /*input_text*/
                         d[9]
                     ) && ! /*allow_custom_value*/
                     d[6]), /*disabled*/
-                d[3] ? m && (fl(), Le(m, 1, 1, () => {
-                    m = null;
-                }), ul()) : m ? b[0] & /*disabled*/
-                8 && be(m, 1) : (m = ri(), m.c(), be(m, 1), m.m(u, null)), (!c || b[0] & /*show_options*/
-                    4096) && _e(
+                d[3] ? g && (_l(), Me(g, 1, 1, () => {
+                    g = null;
+                }), ml()) : g ? c[0] & /*disabled*/
+                8 && ge(g, 1) : (g = ri(), g.c(), ge(g, 1), g.m(u, null)), (!m || c[0] & /*show_options*/
+                    4096) && de(
                     s,
                     "show_options",
                     /*show_options*/
                     d[12]
                 );
             const p = {};
-            b[0] & /*show_options*/
+            c[0] & /*show_options*/
                 4096 && (p.show_options = /*show_options*/
-                    d[12]), b[0] & /*choices*/
+                    d[12]), c[0] & /*choices*/
                 4 && (p.choices = /*choices*/
-                    d[2]), b[0] & /*filtered_indices*/
+                    d[2]), c[0] & /*filtered_indices*/
                 1024 && (p.filtered_indices = /*filtered_indices*/
-                    d[10]), b[0] & /*disabled*/
+                    d[10]), c[0] & /*disabled*/
                 8 && (p.disabled = /*disabled*/
-                    d[3]), b[0] & /*selected_index*/
+                    d[3]), c[0] & /*selected_index*/
                 2048 && (p.selected_indices = /*selected_index*/
                     d[11] === null ? [] : [
                         /*selected_index*/
                         d[11]
-                    ]), b[0] & /*active_index*/
+                    ]), c[0] & /*active_index*/
                 16384 && (p.active_index = /*active_index*/
-                    d[14]), h.$set(p), (!c || b[0] & /*container*/
-                    32) && _e(
+                    d[14]), h.$set(p), (!m || c[0] & /*container*/
+                    32) && de(
                     t,
                     "container",
                     /*container*/
                     d[5]
                 );
         },
         i(d) {
-            c || (be(n.$$.fragment, d), be(m), be(h.$$.fragment, d), c = !0);
+            m || (ge(n.$$.fragment, d), ge(g), ge(h.$$.fragment, d), m = !0);
         },
         o(d) {
-            Le(n.$$.fragment, d), Le(m), Le(h.$$.fragment, d), c = !1;
+            Me(n.$$.fragment, d), Me(g), Me(h.$$.fragment, d), m = !1;
         },
         d(d) {
-            d && dn(t), ln(n), e[29](null), m && m.d(), ln(h), _ = !1, cl(g);
+            d && bn(t), un(n), e[29](null), g && g.d(), un(h), _ = !1, bl(b);
         }
     };
 }
 
-function El(e, t, n) {
+function Hl(e, t, n) {
     let {
         label: i
     } = t, {
         info: r = void 0
     } = t, {
         value: s = []
     } = t, u = [], {
@@ -5707,124 +5707,124 @@
     } = t, {
         choices: a
     } = t, f, {
         disabled: l = !1
     } = t, {
         show_label: h
     } = t, {
-        container: c = !0
+        container: m = !0
     } = t, {
         allow_custom_value: _ = !1
     } = t, {
-        filterable: g = !0
-    } = t, m, d = !1, b, y, p = "", B = "", T = !1, O = [], C = null, w = null, k;
-    const x = gl();
-    s ? (k = a.map((E) => E[1]).indexOf(s), w = k, w === -1 ? (u = s, w = null) : ([p, u] = a[w], B = p), W()) : a.length > 0 && (k = 0, w = 0, [p, s] = a[w], u = s, B = p);
+        filterable: b = !0
+    } = t, g, d = !1, c, y, p = "", B = "", C = !1, O = [], T = null, E = null, k;
+    const x = El();
+    s ? (k = a.map((w) => w[1]).indexOf(s), E = k, E === -1 ? (u = s, E = null) : ([p, u] = a[E], B = p), W()) : a.length > 0 && (k = 0, E = 0, [p, s] = a[E], u = s, B = p);
 
-    function L() {
-        n(13, b = a.map((E) => E[0])), n(24, y = a.map((E) => E[1]));
+    function M() {
+        n(13, c = a.map((w) => w[0])), n(24, y = a.map((w) => w[1]));
     }
 
     function W() {
-        L(), s === void 0 || Array.isArray(s) && s.length === 0 ? (n(9, p = ""), n(11, w = null)) : y.includes(s) ? (n(9, p = b[y.indexOf(s)]), n(11, w = y.indexOf(s))) : _ ? (n(9, p = s), n(11, w = null)) : (n(9, p = ""), n(11, w = null)), n(27, k = w);
+        M(), s === void 0 || Array.isArray(s) && s.length === 0 ? (n(9, p = ""), n(11, E = null)) : y.includes(s) ? (n(9, p = c[y.indexOf(s)]), n(11, E = y.indexOf(s))) : _ ? (n(9, p = s), n(11, E = null)) : (n(9, p = ""), n(11, E = null)), n(27, k = E);
     }
 
-    function ee(E) {
-        if (n(11, w = parseInt(E.detail.target.dataset.index)), isNaN(w)) {
-            n(11, w = null);
+    function ee(w) {
+        if (n(11, E = parseInt(w.detail.target.dataset.index)), isNaN(E)) {
+            n(11, E = null);
             return;
         }
-        n(12, d = !1), n(14, C = null), m.blur();
+        n(12, d = !1), n(14, T = null), g.blur();
     }
 
-    function St(E) {
-        n(10, O = a.map((vn, Bt) => Bt)), n(12, d = !0), x("focus");
+    function At(w) {
+        n(10, O = a.map((yn, Ze) => Ze)), n(12, d = !0), x("focus");
     }
 
-    function Ce() {
-        _ ? n(20, s = p) : n(9, p = b[y.indexOf(s)]), n(12, d = !1), n(14, C = null), x("blur");
+    function Pe() {
+        _ ? n(20, s = p) : n(9, p = c[y.indexOf(s)]), n(12, d = !1), n(14, T = null), x("blur");
     }
 
-    function Ht(E) {
-        n(12, [d, C] = ol(E, C, O), d, (n(14, C), n(2, a), n(23, f), n(6, _), n(9, p), n(10, O), n(8, m), n(25, B), n(11, w), n(27, k), n(26, T), n(24, y))), E.key === "Enter" && (C !== null ? (n(11, w = C), n(12, d = !1), m.blur(), n(14, C = null)) : b.includes(p) ? (n(11, w = b.indexOf(p)), n(12, d = !1), n(14, C = null), m.blur()) : _ && (n(20, s = p), n(11, w = null), n(12, d = !1), n(14, C = null), m.blur()), x("enter", s));
+    function Bt(w) {
+        n(12, [d, T] = fl(w, T, O), d, (n(14, T), n(2, a), n(23, f), n(6, _), n(9, p), n(10, O), n(8, g), n(25, B), n(11, E), n(27, k), n(26, C), n(24, y))), w.key === "Enter" && (T !== null ? (n(11, E = T), n(12, d = !1), g.blur(), n(14, T = null)) : c.includes(p) ? (n(11, E = c.indexOf(p)), n(12, d = !1), n(14, T = null), g.blur()) : _ && (n(20, s = p), n(11, E = null), n(12, d = !1), n(14, T = null), g.blur()), x("enter", s));
     }
-    pl(() => {
-        n(21, o = !1), n(26, T = !0);
-    }), bl(() => {
-        m.focus();
+    wl(() => {
+        n(21, o = !1), n(26, C = !0);
+    }), yl(() => {
+        g.focus();
     });
 
-    function At() {
-        p = this.value, n(9, p), n(11, w), n(27, k), n(26, T), n(2, a), n(24, y);
+    function Ct() {
+        p = this.value, n(9, p), n(11, E), n(27, k), n(26, C), n(2, a), n(24, y);
     }
 
-    function Pe(E) {
-        ll[E ? "unshift" : "push"](() => {
-            m = E, n(8, m);
+    function Ie(w) {
+        cl[w ? "unshift" : "push"](() => {
+            g = w, n(8, g);
         });
     }
-    const Ie = (E) => x("key_up", {
-        key: E.key,
+    const fe = (w) => x("key_up", {
+        key: w.key,
         input_value: p
     });
-    return e.$$set = (E) => {
-        "label" in E && n(0, i = E.label), "info" in E && n(1, r = E.info), "value" in E && n(20, s = E.value), "value_is_output" in E && n(21, o = E.value_is_output), "choices" in E && n(2, a = E.choices), "disabled" in E && n(3, l = E.disabled), "show_label" in E && n(4, h = E.show_label), "container" in E && n(5, c = E.container), "allow_custom_value" in E && n(6, _ = E.allow_custom_value), "filterable" in E && n(7, g = E.filterable);
+    return e.$$set = (w) => {
+        "label" in w && n(0, i = w.label), "info" in w && n(1, r = w.info), "value" in w && n(20, s = w.value), "value_is_output" in w && n(21, o = w.value_is_output), "choices" in w && n(2, a = w.choices), "disabled" in w && n(3, l = w.disabled), "show_label" in w && n(4, h = w.show_label), "container" in w && n(5, m = w.container), "allow_custom_value" in w && n(6, _ = w.allow_custom_value), "filterable" in w && n(7, b = w.filterable);
     }, e.$$.update = () => {
         e.$$.dirty[0] & /*selected_index, old_selected_index, initialized, choices, choices_values*/
-            218105860 && w !== k && w !== null && T && (n(9, [p, s] = a[w], p, (n(20, s), n(11, w), n(27, k), n(26, T), n(2, a), n(24, y))), n(27, k = w), x("select", {
-                index: w,
-                value: y[w],
+            218105860 && E !== k && E !== null && C && (n(9, [p, s] = a[E], p, (n(20, s), n(11, E), n(27, k), n(26, C), n(2, a), n(24, y))), n(27, k = E), x("select", {
+                index: E,
+                value: y[E],
                 selected: !0
             })), e.$$.dirty[0] & /*value, old_value, value_is_output*/
-            7340032 && s != u && (W(), sl(x, s, o), n(22, u = s)), e.$$.dirty[0] & /*choices*/
-            4 && L(), e.$$.dirty[0] & /*choices, old_choices, allow_custom_value, input_text, filtered_indices, filter_input*/
-            8390468 && a !== f && (_ || W(), n(23, f = a), n(10, O = ni(a, p)), !_ && O.length > 0 && n(14, C = O[0]), m == document.activeElement && n(12, d = !0)), e.$$.dirty[0] & /*input_text, old_input_text, choices, allow_custom_value, filtered_indices*/
-            33556036 && p !== B && (n(10, O = ni(a, p)), n(25, B = p), !_ && O.length > 0 && n(14, C = O[0]));
+            7340032 && s != u && (W(), ul(x, s, o), n(22, u = s)), e.$$.dirty[0] & /*choices*/
+            4 && M(), e.$$.dirty[0] & /*choices, old_choices, allow_custom_value, input_text, filtered_indices, filter_input*/
+            8390468 && a !== f && (_ || W(), n(23, f = a), n(10, O = ni(a, p)), !_ && O.length > 0 && n(14, T = O[0]), g == document.activeElement && n(12, d = !0)), e.$$.dirty[0] & /*input_text, old_input_text, choices, allow_custom_value, filtered_indices*/
+            33556036 && p !== B && (n(10, O = ni(a, p)), n(25, B = p), !_ && O.length > 0 && n(14, T = O[0]));
     }, [
         i,
         r,
         a,
         l,
         h,
-        c,
+        m,
         _,
+        b,
         g,
-        m,
         p,
         O,
-        w,
+        E,
         d,
-        b,
-        C,
+        c,
+        T,
         x,
         ee,
-        St,
-        Ce,
-        Ht,
+        At,
+        Pe,
+        Bt,
         s,
         o,
         u,
         f,
         y,
         B,
-        T,
+        C,
         k,
-        At,
-        Pe,
-        Ie
+        Ct,
+        Ie,
+        fe
     ];
 }
-class wl extends al {
+class Al extends hl {
     constructor(t) {
-        super(), hl(
+        super(), dl(
             this,
             t,
-            El,
-            yl,
-            ml, {
+            Hl,
+            Sl,
+            gl, {
                 label: 0,
                 info: 1,
                 value: 20,
                 value_is_output: 21,
                 choices: 2,
                 disabled: 3,
                 show_label: 4,
@@ -5834,73 +5834,73 @@
             },
             null,
             [-1, -1]
         );
     }
 }
 const {
-    SvelteComponent: xl,
+    SvelteComponent: Bl,
     append: $,
-    attr: $e,
-    create_component: et,
-    destroy_component: tt,
-    detach: gn,
+    attr: tt,
+    create_component: nt,
+    destroy_component: it,
+    detach: pn,
     element: ae,
-    init: Sl,
-    insert: pn,
-    mount_component: nt,
-    safe_not_equal: Hl,
-    set_style: it,
-    space: Xt,
+    init: Cl,
+    insert: vn,
+    mount_component: rt,
+    safe_not_equal: Tl,
+    set_style: st,
+    space: Vt,
     text: Xi,
-    transition_in: rt,
-    transition_out: st
+    transition_in: ot,
+    transition_out: at
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: Al
+    createEventDispatcher: Pl
 } = window.__gradio__svelte__internal, {
-    onMount: Bl,
-    onDestroy: Tl
+    onMount: Il,
+    onDestroy: Nl
 } = window.__gradio__svelte__internal;
 
-function Cl(e) {
+function Ol(e) {
     let t;
     return {
         c() {
             t = Xi("Cancel");
         },
         m(n, i) {
-            pn(n, t, i);
+            vn(n, t, i);
         },
         d(n) {
-            n && gn(t);
+            n && pn(t);
         }
     };
 }
 
-function Pl(e) {
+function Ll(e) {
     let t;
     return {
         c() {
             t = Xi("OK");
         },
         m(n, i) {
-            pn(n, t, i);
+            vn(n, t, i);
         },
         d(n) {
-            n && gn(t);
+            n && pn(t);
         }
     };
 }
 
-function Il(e) {
-    let t, n, i, r, s, u, o, a, f, l, h, c, _, g, m;
-    return s = new wl({
+function Ml(e) {
+    let t, n, i, r, s, u, o, a, f, l, h, m, _, b, g;
+    return s = new Al({
         props: {
             value: (
-                /*label*/
+                /*currentLabel*/
                 e[0]
             ),
             label: "Label",
             choices: (
                 /*choices*/
                 e[2]
             ),
@@ -5911,225 +5911,233 @@
         "change",
         /*onDropDownChange*/
         e[4]
     ), s.$on(
         "enter",
         /*onDropDownEnter*/
         e[6]
-    ), a = new ks({
+    ), a = new Fs({
         props: {
             value: (
-                /*color*/
+                /*currentColor*/
                 e[1]
             ),
             label: "Color",
             show_label: !1
         }
     }), a.$on(
         "change",
         /*onColorChange*/
         e[5]
-    ), h = new Ln({
+    ), h = new Mn({
         props: {
             $$slots: {
-                default: [Cl]
+                default: [Ol]
             },
             $$scope: {
                 ctx: e
             }
         }
     }), h.$on(
         "click",
         /*click_handler*/
-        e[8]
-    ), g = new Ln({
+        e[10]
+    ), b = new Mn({
         props: {
             variant: "primary",
             $$slots: {
-                default: [Pl]
+                default: [Ll]
             },
             $$scope: {
                 ctx: e
             }
         }
-    }), g.$on(
+    }), b.$on(
         "click",
         /*click_handler_1*/
-        e[9]
+        e[11]
     ), {
         c() {
-            t = ae("div"), n = ae("div"), i = ae("span"), r = ae("div"), et(s.$$.fragment), u = Xt(), o = ae("div"), et(a.$$.fragment), f = Xt(), l = ae("div"), et(h.$$.fragment), c = Xt(), _ = ae("div"), et(g.$$.fragment), it(r, "margin-right", "10px"), it(o, "margin-right", "40px"), it(o, "margin-bottom", "8px"), it(l, "margin-right", "8px"), $e(i, "class", "model-content svelte-hkn2q1"), $e(n, "class", "modal-container svelte-hkn2q1"), $e(t, "class", "modal svelte-hkn2q1"), $e(t, "id", "model-box-edit");
+            t = ae("div"), n = ae("div"), i = ae("span"), r = ae("div"), nt(s.$$.fragment), u = Vt(), o = ae("div"), nt(a.$$.fragment), f = Vt(), l = ae("div"), nt(h.$$.fragment), m = Vt(), _ = ae("div"), nt(b.$$.fragment), st(r, "margin-right", "10px"), st(o, "margin-right", "40px"), st(o, "margin-bottom", "8px"), st(l, "margin-right", "8px"), tt(i, "class", "model-content svelte-hkn2q1"), tt(n, "class", "modal-container svelte-hkn2q1"), tt(t, "class", "modal svelte-hkn2q1"), tt(t, "id", "model-box-edit");
         },
-        m(d, b) {
-            pn(d, t, b), $(t, n), $(n, i), $(i, r), nt(s, r, null), $(i, u), $(i, o), nt(a, o, null), $(i, f), $(i, l), nt(h, l, null), $(i, c), $(i, _), nt(g, _, null), m = !0;
+        m(d, c) {
+            vn(d, t, c), $(t, n), $(n, i), $(i, r), rt(s, r, null), $(i, u), $(i, o), rt(a, o, null), $(i, f), $(i, l), rt(h, l, null), $(i, m), $(i, _), rt(b, _, null), g = !0;
         },
-        p(d, [b]) {
+        p(d, [c]) {
             const y = {};
-            b & /*label*/
-                1 && (y.value = /*label*/
-                    d[0]), b & /*choices*/
+            c & /*currentLabel*/
+                1 && (y.value = /*currentLabel*/
+                    d[0]), c & /*choices*/
                 4 && (y.choices = /*choices*/
                     d[2]), s.$set(y);
             const p = {};
-            b & /*color*/
-                2 && (p.value = /*color*/
+            c & /*currentColor*/
+                2 && (p.value = /*currentColor*/
                     d[1]), a.$set(p);
             const B = {};
-            b & /*$$scope*/
-                4096 && (B.$$scope = {
-                    dirty: b,
+            c & /*$$scope*/
+                16384 && (B.$$scope = {
+                    dirty: c,
                     ctx: d
                 }), h.$set(B);
-            const T = {};
-            b & /*$$scope*/
-                4096 && (T.$$scope = {
-                    dirty: b,
+            const C = {};
+            c & /*$$scope*/
+                16384 && (C.$$scope = {
+                    dirty: c,
                     ctx: d
-                }), g.$set(T);
+                }), b.$set(C);
         },
         i(d) {
-            m || (rt(s.$$.fragment, d), rt(a.$$.fragment, d), rt(h.$$.fragment, d), rt(g.$$.fragment, d), m = !0);
+            g || (ot(s.$$.fragment, d), ot(a.$$.fragment, d), ot(h.$$.fragment, d), ot(b.$$.fragment, d), g = !0);
         },
         o(d) {
-            st(s.$$.fragment, d), st(a.$$.fragment, d), st(h.$$.fragment, d), st(g.$$.fragment, d), m = !1;
+            at(s.$$.fragment, d), at(a.$$.fragment, d), at(h.$$.fragment, d), at(b.$$.fragment, d), g = !1;
         },
         d(d) {
-            d && gn(t), tt(s), tt(a), tt(h), tt(g);
+            d && pn(t), it(s), it(a), it(h), it(b);
         }
     };
 }
 
-function Nl(e, t, n) {
+function Rl(e, t, n) {
     let {
         label: i = ""
     } = t, {
-        choices: r = []
+        currentLabel: r = ""
+    } = t, {
+        choices: s = []
+    } = t, {
+        choicesColors: u = []
     } = t, {
-        choicesColors: s = []
+        color: o = ""
     } = t, {
-        color: u = ""
+        currentColor: a = ""
     } = t;
-    const o = Al();
+    const f = Pl();
 
-    function a(m) {
-        o("change", {
-            label: i,
-            color: u,
-            ok: m
+    function l(c) {
+        f("change", {
+            label: r,
+            color: a,
+            ok: c
         });
     }
 
-    function f(m) {
+    function h(c) {
         const {
-            detail: d
-        } = m;
-        let b = d;
-        Number.isInteger(b) ? (Array.isArray(s) && b < s.length && n(1, u = s[b]), Array.isArray(r) && b < r.length && n(0, i = r[b][0])) : n(0, i = b);
+            detail: y
+        } = c;
+        let p = y;
+        Number.isInteger(p) ? (Array.isArray(u) && p < u.length && n(1, a = u[p]), Array.isArray(s) && p < s.length && n(0, r = s[p][0])) : n(0, r = p);
     }
 
-    function l(m) {
+    function m(c) {
         const {
-            detail: d
-        } = m;
-        n(1, u = d);
+            detail: y
+        } = c;
+        n(1, a = y);
     }
 
-    function h(m) {
-        f(m), a(!0);
+    function _(c) {
+        h(c), l(!0);
     }
 
-    function c(m) {
-        switch (m.key) {
+    function b(c) {
+        switch (c.key) {
             case "Enter":
-                a(!0);
+                l(!0);
                 break;
         }
     }
-    Bl(() => {
-        document.addEventListener("keydown", c);
-    }), Tl(() => {
-        document.removeEventListener("keydown", c);
+    Il(() => {
+        document.addEventListener("keydown", b), n(0, r = i), n(1, a = o);
+    }), Nl(() => {
+        document.removeEventListener("keydown", b);
     });
-    const _ = () => a(!1),
-        g = () => a(!0);
-    return e.$$set = (m) => {
-        "label" in m && n(0, i = m.label), "choices" in m && n(2, r = m.choices), "choicesColors" in m && n(7, s = m.choicesColors), "color" in m && n(1, u = m.color);
+    const g = () => l(!1),
+        d = () => l(!0);
+    return e.$$set = (c) => {
+        "label" in c && n(7, i = c.label), "currentLabel" in c && n(0, r = c.currentLabel), "choices" in c && n(2, s = c.choices), "choicesColors" in c && n(8, u = c.choicesColors), "color" in c && n(9, o = c.color), "currentColor" in c && n(1, a = c.currentColor);
     }, [
-        i,
-        u,
         r,
         a,
-        f,
+        s,
         l,
         h,
-        s,
+        m,
         _,
-        g
+        i,
+        u,
+        o,
+        g,
+        d
     ];
 }
-class Vi extends xl {
+class Vi extends Bl {
     constructor(t) {
-        super(), Sl(this, t, Nl, Il, Hl, {
-            label: 0,
+        super(), Cl(this, t, Rl, Ml, Tl, {
+            label: 7,
+            currentLabel: 0,
             choices: 2,
-            choicesColors: 7,
-            color: 1
+            choicesColors: 8,
+            color: 9,
+            currentColor: 1
         });
     }
 }
 const J = (e, t, n) => Math.min(Math.max(e, t), n);
 
-function Vt(e, t) {
+function qt(e, t) {
     if (e.startsWith("rgba"))
         return e.replace(/[\d.]+$/, t.toString());
     const n = e.match(/\d+/g);
     if (!n || n.length !== 3)
         return `rgba(50, 50, 50, ${t})`;
     const [i, r, s] = n;
     return `rgba(${i}, ${r}, ${s}, ${t})`;
 }
-class qt {
-    constructor(t, n, i, r, s, u, o, a, f, l, h = "rgb(255, 255, 255)", c = 0.5, _ = 25, g = 1) {
+class Wt {
+    constructor(t, n, i, r, s, u, o, a, f, l, h = "rgb(255, 255, 255)", m = 0.5, _ = 25, b = 1) {
         this.stopDrag = () => {
             this.isDragging = !1, document.removeEventListener("mousemove", this.handleDrag), document.removeEventListener("mouseup", this.stopDrag);
-        }, this.handleDrag = (m) => {
+        }, this.handleDrag = (g) => {
             if (this.isDragging) {
-                let d = m.clientX - this.offsetMouseX - this.xmin,
-                    b = m.clientY - this.offsetMouseY - this.ymin;
+                let d = g.clientX - this.offsetMouseX - this.xmin,
+                    c = g.clientY - this.offsetMouseY - this.ymin;
                 const y = this.canvasXmax - this.canvasXmin,
                     p = this.canvasYmax - this.canvasYmin;
-                d = J(d, -this.xmin, y - this.xmax), b = J(b, -this.ymin, p - this.ymax), this.xmin += d, this.ymin += b, this.xmax += d, this.ymax += b, this.updateHandles(), this.renderCallBack();
+                d = J(d, -this.xmin, y - this.xmax), c = J(c, -this.ymin, p - this.ymax), this.xmin += d, this.ymin += c, this.xmax += d, this.ymax += c, this.updateHandles(), this.renderCallBack();
             }
-        }, this.handleResize = (m) => {
+        }, this.handleResize = (g) => {
             if (this.isResizing) {
-                const d = m.clientX,
-                    b = m.clientY,
+                const d = g.clientX,
+                    c = g.clientY,
                     y = d - this.resizeHandles[this.resizingHandleIndex].xmin - this.offsetMouseX,
-                    p = b - this.resizeHandles[this.resizingHandleIndex].ymin - this.offsetMouseY,
+                    p = c - this.resizeHandles[this.resizingHandleIndex].ymin - this.offsetMouseY,
                     B = this.canvasXmax - this.canvasXmin,
-                    T = this.canvasYmax - this.canvasYmin;
+                    C = this.canvasYmax - this.canvasYmin;
                 switch (this.resizingHandleIndex) {
                     case 0:
                         this.xmin += y, this.ymin += p, this.xmin = J(this.xmin, 0, this.xmax - this.minSize), this.ymin = J(this.ymin, 0, this.ymax - this.minSize);
                         break;
                     case 1:
                         this.xmax += y, this.ymin += p, this.xmax = J(this.xmax, this.xmin + this.minSize, B), this.ymin = J(this.ymin, 0, this.ymax - this.minSize);
                         break;
                     case 2:
-                        this.xmax += y, this.ymax += p, this.xmax = J(this.xmax, this.xmin + this.minSize, B), this.ymax = J(this.ymax, this.ymin + this.minSize, T);
+                        this.xmax += y, this.ymax += p, this.xmax = J(this.xmax, this.xmin + this.minSize, B), this.ymax = J(this.ymax, this.ymin + this.minSize, C);
                         break;
                     case 3:
-                        this.xmin += y, this.ymax += p, this.xmin = J(this.xmin, 0, this.xmax - this.minSize), this.ymax = J(this.ymax, this.ymin + this.minSize, T);
+                        this.xmin += y, this.ymax += p, this.xmin = J(this.xmin, 0, this.xmax - this.minSize), this.ymax = J(this.ymax, this.ymin + this.minSize, C);
                         break;
                 }
                 this.updateHandles(), this.renderCallBack();
             }
         }, this.stopResize = () => {
             this.isResizing = !1, document.removeEventListener("mousemove", this.handleResize), document.removeEventListener("mouseup", this.stopResize);
-        }, this.renderCallBack = t, this.canvasXmin = n, this.canvasYmin = i, this.canvasXmax = r, this.canvasYmax = s, this.scaleFactor = g, this.label = u, this.isDragging = !1, [this.xmin, this.ymin] = this.toBoxCoordinates(o, a), [this.xmax, this.ymax] = this.toBoxCoordinates(f, l), this.isResizing = !1, this.isSelected = !1, this.offsetMouseX = 0, this.offsetMouseY = 0, this.resizeHandleSize = 8, this.updateHandles(), this.resizingHandleIndex = -1, this.minSize = _, this.color = h, this.alpha = c;
+        }, this.renderCallBack = t, this.canvasXmin = n, this.canvasYmin = i, this.canvasXmax = r, this.canvasYmax = s, this.scaleFactor = b, this.label = u, this.isDragging = !1, [this.xmin, this.ymin] = this.toBoxCoordinates(o, a), [this.xmax, this.ymax] = this.toBoxCoordinates(f, l), this.isResizing = !1, this.isSelected = !1, this.offsetMouseX = 0, this.offsetMouseY = 0, this.resizeHandleSize = 8, this.updateHandles(), this.resizingHandleIndex = -1, this.minSize = _, this.color = h, this.alpha = m;
     }
     toJSON() {
         return {
             label: this.label,
             xmin: this.xmin,
             ymin: this.ymin,
             xmax: this.xmax,
@@ -6179,23 +6187,23 @@
         return t = t + this.canvasXmin, n = n + this.canvasYmin, [t, n];
     }
     toBoxCoordinates(t, n) {
         return t = t - this.canvasXmin, n = n - this.canvasYmin, [t, n];
     }
     render(t) {
         let n, i;
-        if (t.beginPath(), [n, i] = this.toCanvasCoordinates(this.xmin, this.ymin), t.rect(n, i, this.getWidth(), this.getHeight()), t.fillStyle = Vt(this.color, this.alpha), t.fill(), this.isSelected ? t.lineWidth = 4 : t.lineWidth = 2, t.strokeStyle = Vt(this.color, 1), t.stroke(), t.closePath(), this.label !== null && this.label.trim() !== "") {
+        if (t.beginPath(), [n, i] = this.toCanvasCoordinates(this.xmin, this.ymin), t.rect(n, i, this.getWidth(), this.getHeight()), t.fillStyle = qt(this.color, this.alpha), t.fill(), this.isSelected ? t.lineWidth = 4 : t.lineWidth = 2, t.strokeStyle = qt(this.color, 1), t.stroke(), t.closePath(), this.label !== null && this.label.trim() !== "") {
             this.isSelected ? t.font = "bold 14px Arial" : t.font = "12px Arial";
             const r = t.measureText(this.label).width + 10,
                 s = 20;
             let u = this.xmin,
                 o = this.ymin - s;
             t.fillStyle = "white", [u, o] = this.toCanvasCoordinates(u, o), t.fillRect(u, o, r, s), t.lineWidth = 1, t.strokeStyle = "black", t.strokeRect(u, o, r, s), t.fillStyle = "black", t.fillText(this.label, u + 5, o + 15);
         }
-        t.fillStyle = Vt(this.color, 1);
+        t.fillStyle = qt(this.color, 1);
         for (const r of this.resizeHandles)
             [n, i] = this.toCanvasCoordinates(r.xmin, r.ymin), t.fillRect(
                 n,
                 i,
                 r.xmax - r.xmin,
                 r.ymax - r.ymin
             );
@@ -6231,50 +6239,50 @@
     "rgb(34, 139, 34)",
     "rgb(255, 240, 245)",
     "rgb(255, 193, 37)",
     "rgb(255, 193, 7)",
     "rgb(255, 250, 138)"
 ];
 const {
-    SvelteComponent: Ol,
-    append: ge,
+    SvelteComponent: kl,
+    append: pe,
     attr: le,
-    binding_callbacks: Ml,
+    binding_callbacks: Dl,
     bubble: si,
-    check_outros: Wt,
+    check_outros: Yt,
     create_component: De,
     destroy_component: Ue,
-    detach: pe,
-    element: Ee,
-    empty: Ll,
-    group_outros: Yt,
-    init: Rl,
-    insert: ve,
+    detach: ve,
+    element: we,
+    empty: Ul,
+    group_outros: Zt,
+    init: Gl,
+    insert: ye,
     listen: re,
     mount_component: Ge,
-    noop: kl,
+    noop: Fl,
     run_all: qi,
-    safe_not_equal: Dl,
+    safe_not_equal: zl,
     space: Fe,
     transition_in: G,
     transition_out: q
 } = window.__gradio__svelte__internal, {
-    onMount: Ul,
-    onDestroy: Gl,
-    createEventDispatcher: Fl
+    onMount: jl,
+    onDestroy: Xl,
+    createEventDispatcher: Vl
 } = window.__gradio__svelte__internal;
 
 function oi(e) {
-    let t, n, i, r, s, u, o, a, f, l, h, c;
-    return i = new Rr({}), u = new Cr({}), f = new mr({}), {
+    let t, n, i, r, s, u, o, a, f, l, h, m;
+    return i = new Gr({}), u = new Or({}), f = new gr({}), {
         c() {
-            t = Ee("span"), n = Ee("button"), De(i.$$.fragment), r = Fe(), s = Ee("button"), De(u.$$.fragment), o = Fe(), a = Ee("button"), De(f.$$.fragment), le(n, "class", "icon svelte-182gnnj"), le(s, "class", "icon svelte-182gnnj"), le(a, "class", "icon svelte-182gnnj"), le(t, "class", "canvas-control svelte-182gnnj");
+            t = we("span"), n = we("button"), De(i.$$.fragment), r = Fe(), s = we("button"), De(u.$$.fragment), o = Fe(), a = we("button"), De(f.$$.fragment), le(n, "class", "icon svelte-182gnnj"), le(s, "class", "icon svelte-182gnnj"), le(a, "class", "icon svelte-182gnnj"), le(t, "class", "canvas-control svelte-182gnnj");
         },
-        m(_, g) {
-            ve(_, t, g), ge(t, n), Ge(i, n, null), ge(t, r), ge(t, s), Ge(u, s, null), ge(t, o), ge(t, a), Ge(f, a, null), l = !0, h || (c = [
+        m(_, b) {
+            ye(_, t, b), pe(t, n), Ge(i, n, null), pe(t, r), pe(t, s), Ge(u, s, null), pe(t, o), pe(t, a), Ge(f, a, null), l = !0, h || (m = [
                 re(
                     n,
                     "click",
                     /*click_handler*/
                     e[22]
                 ),
                 re(
@@ -6287,23 +6295,23 @@
                     a,
                     "click",
                     /*click_handler_2*/
                     e[24]
                 )
             ], h = !0);
         },
-        p: kl,
+        p: Fl,
         i(_) {
             l || (G(i.$$.fragment, _), G(u.$$.fragment, _), G(f.$$.fragment, _), l = !0);
         },
         o(_) {
             q(i.$$.fragment, _), q(u.$$.fragment, _), q(f.$$.fragment, _), l = !1;
         },
         d(_) {
-            _ && pe(t), Ue(i), Ue(u), Ue(f), h = !1, qi(c);
+            _ && ve(t), Ue(i), Ue(u), Ue(f), h = !1, qi(m);
         }
     };
 }
 
 function ai(e) {
     let t, n;
     return t = new Vi({
@@ -6462,33 +6470,33 @@
         },
         d(i) {
             Ue(t, i);
         }
     };
 }
 
-function zl(e) {
+function ql(e) {
     let t, n, i, r, s, u, o, a, f, l = (
             /*interactive*/
             e[1] && oi(e)
         ),
         h = (
             /*editModalVisible*/
             e[6] && ai(e)
         ),
-        c = (
+        m = (
             /*newModalVisible*/
             e[7] && li(e)
         );
     return {
         c() {
-            t = Ee("div"), n = Ee("canvas"), i = Fe(), l && l.c(), r = Fe(), h && h.c(), s = Fe(), c && c.c(), u = Ll(), le(n, "class", "canvas-annotator svelte-182gnnj"), le(t, "class", "canvas-container svelte-182gnnj"), le(t, "tabindex", "-1");
+            t = we("div"), n = we("canvas"), i = Fe(), l && l.c(), r = Fe(), h && h.c(), s = Fe(), m && m.c(), u = Ul(), le(n, "class", "canvas-annotator svelte-182gnnj"), le(t, "class", "canvas-container svelte-182gnnj"), le(t, "tabindex", "-1");
         },
-        m(_, g) {
-            ve(_, t, g), ge(t, n), e[21](n), ve(_, i, g), l && l.m(_, g), ve(_, r, g), h && h.m(_, g), ve(_, s, g), c && c.m(_, g), ve(_, u, g), o = !0, a || (f = [
+        m(_, b) {
+            ye(_, t, b), pe(t, n), e[21](n), ye(_, i, b), l && l.m(_, b), ye(_, r, b), h && h.m(_, b), ye(_, s, b), m && m.m(_, b), ye(_, u, b), o = !0, a || (f = [
                 re(
                     n,
                     "mousedown",
                     /*handleMouseDown*/
                     e[8]
                 ),
                 re(
@@ -6513,37 +6521,37 @@
                     t,
                     "focusout",
                     /*handleCanvasBlur*/
                     e[17]
                 )
             ], a = !0);
         },
-        p(_, g) {
+        p(_, b) {
             /*interactive*/
-            _[1] ? l ? (l.p(_, g), g[0] & /*interactive*/
-                    2 && G(l, 1)) : (l = oi(_), l.c(), G(l, 1), l.m(r.parentNode, r)) : l && (Yt(), q(l, 1, 1, () => {
+            _[1] ? l ? (l.p(_, b), b[0] & /*interactive*/
+                    2 && G(l, 1)) : (l = oi(_), l.c(), G(l, 1), l.m(r.parentNode, r)) : l && (Zt(), q(l, 1, 1, () => {
                     l = null;
-                }), Wt()), /*editModalVisible*/
-                _[6] ? h ? (h.p(_, g), g[0] & /*editModalVisible*/
-                    64 && G(h, 1)) : (h = ai(_), h.c(), G(h, 1), h.m(s.parentNode, s)) : h && (Yt(), q(h, 1, 1, () => {
+                }), Yt()), /*editModalVisible*/
+                _[6] ? h ? (h.p(_, b), b[0] & /*editModalVisible*/
+                    64 && G(h, 1)) : (h = ai(_), h.c(), G(h, 1), h.m(s.parentNode, s)) : h && (Zt(), q(h, 1, 1, () => {
                     h = null;
-                }), Wt()), /*newModalVisible*/
-                _[7] ? c ? (c.p(_, g), g[0] & /*newModalVisible*/
-                    128 && G(c, 1)) : (c = li(_), c.c(), G(c, 1), c.m(u.parentNode, u)) : c && (Yt(), q(c, 1, 1, () => {
-                    c = null;
-                }), Wt());
+                }), Yt()), /*newModalVisible*/
+                _[7] ? m ? (m.p(_, b), b[0] & /*newModalVisible*/
+                    128 && G(m, 1)) : (m = li(_), m.c(), G(m, 1), m.m(u.parentNode, u)) : m && (Zt(), q(m, 1, 1, () => {
+                    m = null;
+                }), Yt());
         },
         i(_) {
-            o || (G(l), G(h), G(c), o = !0);
+            o || (G(l), G(h), G(m), o = !0);
         },
         o(_) {
-            q(l), q(h), q(c), o = !1;
+            q(l), q(h), q(m), o = !1;
         },
         d(_) {
-            _ && (pe(t), pe(i), pe(r), pe(s), pe(u)), e[21](null), l && l.d(_), h && h.d(_), c && c.d(_), a = !1, qi(f);
+            _ && (ve(t), ve(i), ve(r), ve(s), ve(u)), e[21](null), l && l.d(_), h && h.d(_), m && m.d(_), a = !1, qi(f);
         }
     };
 }
 
 function ui(e) {
     var t = parseInt(e.slice(1, 3), 16),
         n = parseInt(e.slice(3, 5), 16),
@@ -6555,267 +6563,275 @@
     const t = e.match(/(\d+(\.\d+)?)/g),
         n = parseInt(t[0]),
         i = parseInt(t[1]),
         r = parseInt(t[2]);
     return "#" + (1 << 24 | n << 16 | i << 8 | r).toString(16).slice(1);
 }
 
-function jl(e, t, n) {
+function Wl(e, t, n) {
     let {
         imageUrl: i = null
     } = t, {
         interactive: r
     } = t, {
         boxAlpha: s = 0.5
     } = t, {
         boxMinSize: u = 25
     } = t, {
         value: o
     } = t, {
         choices: a = []
     } = t, {
         choicesColors: f = []
-    } = t, l, h, c = null, _ = -1, g = 0, m = 0, d = 0, b = 0, y = 1, p = 0, B = 0, T = !1, O = !1;
-    const C = Fl();
+    } = t, l, h, m = null, _ = -1, b = 0, g = 0, d = 0, c = 0, y = 1, p = 0, B = 0, C = !1, O = !1;
+    const T = Vl();
 
-    function w() {
+    function E() {
         if (h) {
-            h.clearRect(0, 0, l.width, l.height), c !== null && h.drawImage(c, g, m, p, B);
+            h.clearRect(0, 0, l.width, l.height), m !== null && h.drawImage(m, b, g, p, B);
             for (const v of o.boxes.slice().reverse())
                 v.render(h);
         }
     }
 
     function k(v) {
         n(5, _ = v), o.boxes.forEach((P) => {
             P.setSelected(!1);
-        }), v >= 0 && v < o.boxes.length && o.boxes[v].setSelected(!0), w();
+        }), v >= 0 && v < o.boxes.length && o.boxes[v].setSelected(!0), E();
     }
 
     function x(v) {
         if (!r)
             return;
         const P = l.getBoundingClientRect(),
             R = v.clientX - P.left,
-            M = v.clientY - P.top;
+            L = v.clientY - P.top;
         for (const [te, Y] of o.boxes.entries()) {
-            const yn = Y.indexOfPointInsideHandle(R, M);
-            if (yn >= 0) {
-                k(te), Y.startResize(yn, v);
+            const Qe = Y.indexOfPointInsideHandle(R, L);
+            if (Qe >= 0) {
+                k(te), Y.startResize(Qe, v);
                 return;
             }
         }
         for (const [te, Y] of o.boxes.entries())
-            if (Y.isPointInsideBox(R, M)) {
+            if (Y.isPointInsideBox(R, L)) {
                 k(te), Y.startDrag(v);
                 return;
             }
         k(-1);
     }
 
-    function L(v) {
-        C("change");
+    function M(v) {
+        T("change");
     }
 
     function W(v) {
         if (r)
             switch (v.key) {
                 case "Delete":
-                    Pe();
+                    Ie();
                     break;
             }
     }
 
     function ee() {
         n(7, O = !0);
     }
 
-    function St(v) {
+    function At(v) {
         n(7, O = !1);
         const {
             detail: P
         } = v;
         let R = P.label,
-            M = P.color;
+            L = P.color;
         if (P.ok) {
-            M === null || M === "" ? M = K[o.boxes.length % K.length] : M = ui(M);
-            let Y = new qt(w, g, m, d, b, R, Math.round(l.width / 3), Math.round(l.height / 3), Math.round(2 * l.width / 3), Math.round(2 * l.height / 3), M, s, u, y);
-            n(0, o.boxes = [Y, ...o.boxes], o), w(), C("change");
+            L === null || L === "" ? L = K[o.boxes.length % K.length] : L = ui(L);
+            let Y = b + (d - b) / 3,
+                Qe = d - (d - b) / 3,
+                tr = g + (c - g) / 3,
+                nr = c - (c - g) / 3,
+                ir = new Wt(E, b, g, d, c, R, Math.round(Y), Math.round(tr), Math.round(Qe), Math.round(nr), L, s, u, y);
+            n(0, o.boxes = [ir, ...o.boxes], o), E(), T("change");
         }
     }
 
-    function Ce() {
-        _ >= 0 && _ < o.boxes.length && n(6, T = !0);
+    function Pe() {
+        _ >= 0 && _ < o.boxes.length && n(6, C = !0);
     }
 
-    function Ht(v) {
-        r && Ce();
+    function Bt(v) {
+        r && Pe();
     }
 
-    function At(v) {
-        n(6, T = !1);
+    function Ct(v) {
+        n(6, C = !1);
         const {
             detail: P
         } = v;
         let R = P.label,
-            M = P.color;
+            L = P.color;
         if (P.ok && _ >= 0 && _ < o.boxes.length) {
             let Y = o.boxes[_];
-            Y.label = R, Y.color = ui(M), w(), C("change");
+            Y.label = R, Y.color = ui(L), E(), T("change");
         }
     }
 
-    function Pe() {
-        _ >= 0 && _ < o.boxes.length && (o.boxes.splice(_, 1), k(-1), C("change"));
+    function Ie() {
+        _ >= 0 && _ < o.boxes.length && (o.boxes.splice(_, 1), k(-1), T("change"));
     }
 
-    function Ie() {
+    function fe() {
         if (l) {
-            if (y = 1, n(4, l.width = l.clientWidth, l), c !== null)
-                if (c.width > l.width)
-                    y = l.width / c.width, p = c.width * y, B = c.height * y, g = 0, m = 0, d = p, b = B, n(4, l.height = B, l);
+            if (y = 1, n(4, l.width = l.clientWidth, l), m !== null)
+                if (m.width > l.width)
+                    y = l.width / m.width, p = m.width * y, B = m.height * y, b = 0, g = 0, d = p, c = B, n(4, l.height = B, l);
                 else {
-                    p = c.width, B = c.height;
+                    p = m.width, B = m.height;
                     var v = (l.width - p) / 2;
-                    g = v, m = 0, d = v + p, b = c.height, n(4, l.height = B, l);
+                    b = v, g = 0, d = v + p, c = m.height, n(4, l.height = B, l);
                 }
             else
-                g = 0, m = 0, d = l.width, b = l.height, n(4, l.height = l.clientHeight, l);
-            if (d > 0 && b > 0)
+                b = 0, g = 0, d = l.width, c = l.height, n(4, l.height = l.clientHeight, l);
+            if (d > 0 && c > 0)
                 for (const P of o.boxes)
-                    P.canvasXmin = g, P.canvasYmin = m, P.canvasXmax = d, P.canvasYmax = b, P.setScaleFactor(y);
-            w(), C("change");
+                    P.canvasXmin = b, P.canvasYmin = g, P.canvasXmax = d, P.canvasYmax = c, P.setScaleFactor(y);
+            E(), T("change");
         }
     }
-    const E = new ResizeObserver(Ie);
+    const w = new ResizeObserver(fe);
 
-    function vn() {
+    function yn() {
         let v = [];
         for (let P = 0; P < o.boxes.length; P++) {
             let R = o.boxes[P];
-            if (!(R instanceof qt)) {
-                let M = "",
+            if (!(R instanceof Wt)) {
+                let L = "",
                     te = "";
-                R.hasOwnProperty("color") ? (M = R.color, Array.isArray(M) && M.length === 3 && (M = `rgb(${M[0]}, ${M[1]}, ${M[2]})`)) : M = K[v.length % K.length], R.hasOwnProperty("label") && (te = R.label), R = new qt(w, g, m, d, b, te, R.xmin, R.ymin, R.xmax, R.ymax, M, s, u, y);
+                R.hasOwnProperty("color") ? (L = R.color, Array.isArray(L) && L.length === 3 && (L = `rgb(${L[0]}, ${L[1]}, ${L[2]})`)) : L = K[v.length % K.length], R.hasOwnProperty("label") && (te = R.label), R = new Wt(E, b, g, d, c, te, R.xmin, R.ymin, R.xmax, R.ymax, L, s, u, y);
             }
             v.push(R);
         }
         n(0, o.boxes = v, o);
     }
-    Ul(() => {
+
+    function Ze() {
+        i !== null && (m === null || m.src != i) && (m = new Image(), m.src = i, m.onload = function() {
+            fe(), E();
+        });
+    }
+    jl(() => {
         if (Array.isArray(a) && a.length > 0 && (!Array.isArray(f) || f.length == 0))
             for (let v = 0; v < a.length; v++) {
                 let P = K[v % K.length];
                 f.push(Xe(P));
             }
-        h = l.getContext("2d"), E.observe(l), i !== null && (c = new Image(), c.src = i, c.onload = function() {
-            Ie(), w();
-        }), Ie(), w();
+        h = l.getContext("2d"), w.observe(l), Ze(), fe(), E();
     });
 
-    function Bt() {
+    function Wi() {
         document.addEventListener("keydown", W);
     }
 
-    function Wi() {
+    function Yi() {
         document.removeEventListener("keydown", W);
     }
-    Gl(() => {
+    Xl(() => {
         document.removeEventListener("keydown", W);
     });
 
-    function Yi(v) {
-        Ml[v ? "unshift" : "push"](() => {
+    function Zi(v) {
+        Dl[v ? "unshift" : "push"](() => {
             l = v, n(4, l);
         });
     }
-    const Zi = () => ee(),
-        Qi = () => Ce(),
-        Ji = () => Pe();
+    const Qi = () => ee(),
+        Ji = () => Pe(),
+        Ki = () => Ie();
 
-    function Ki(v) {
+    function $i(v) {
         si.call(this, e, v);
     }
 
-    function $i(v) {
+    function er(v) {
         si.call(this, e, v);
     }
     return e.$$set = (v) => {
         "imageUrl" in v && n(18, i = v.imageUrl), "interactive" in v && n(1, r = v.interactive), "boxAlpha" in v && n(19, s = v.boxAlpha), "boxMinSize" in v && n(20, u = v.boxMinSize), "value" in v && n(0, o = v.value), "choices" in v && n(2, a = v.choices), "choicesColors" in v && n(3, f = v.choicesColors);
     }, e.$$.update = () => {
         e.$$.dirty[0] & /*value*/
-            1 && vn();
+            1 && (Ze(), yn(), fe(), E());
     }, [
         o,
         r,
         a,
         f,
         l,
         _,
-        T,
+        C,
         O,
         x,
-        L,
+        M,
         ee,
-        St,
-        Ce,
-        Ht,
         At,
         Pe,
         Bt,
+        Ct,
+        Ie,
         Wi,
+        Yi,
         i,
         s,
         u,
-        Yi,
         Zi,
         Qi,
         Ji,
         Ki,
-        $i
+        $i,
+        er
     ];
 }
-class Xl extends Ol {
+class Yl extends kl {
     constructor(t) {
-        super(), Rl(
+        super(), Gl(
             this,
             t,
-            jl,
-            zl,
-            Dl, {
+            Wl,
+            ql,
+            zl, {
                 imageUrl: 18,
                 interactive: 1,
                 boxAlpha: 19,
                 boxMinSize: 20,
                 value: 0,
                 choices: 2,
                 choicesColors: 3
             },
             null,
             [-1, -1]
         );
     }
 }
 const {
-    SvelteComponent: Vl,
-    add_flush_callback: ql,
-    bind: Wl,
-    binding_callbacks: Yl,
-    create_component: Zl,
-    destroy_component: Ql,
-    init: Jl,
-    mount_component: Kl,
-    safe_not_equal: $l,
-    transition_in: eu,
-    transition_out: tu
+    SvelteComponent: Zl,
+    add_flush_callback: Ql,
+    bind: Jl,
+    binding_callbacks: Kl,
+    create_component: $l,
+    destroy_component: eu,
+    init: tu,
+    mount_component: nu,
+    safe_not_equal: iu,
+    transition_in: ru,
+    transition_out: su
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: nu
+    createEventDispatcher: ou
 } = window.__gradio__svelte__internal;
 
-function iu(e) {
+function au(e) {
     let t, n, i;
 
     function r(u) {
         e[10](u);
     }
     let s = {
         interactive: (
@@ -6842,26 +6858,26 @@
             /*resolved_src*/
             e[6]
         )
     };
     return (
         /*value*/
         e[0] !== void 0 && (s.value = /*value*/
-            e[0]), t = new Xl({
+            e[0]), t = new Yl({
             props: s
-        }), Yl.push(() => Wl(t, "value", r)), t.$on(
+        }), Kl.push(() => Jl(t, "value", r)), t.$on(
             "change",
             /*change_handler*/
             e[11]
         ), {
             c() {
-                Zl(t.$$.fragment);
+                $l(t.$$.fragment);
             },
             m(u, o) {
-                Kl(t, u, o), i = !0;
+                nu(t, u, o), i = !0;
             },
             p(u, [o]) {
                 const a = {};
                 o & /*interactive*/
                     2 && (a.interactive = /*interactive*/
                         u[1]), o & /*boxesAlpha*/
                     4 && (a.boxAlpha = /*boxesAlpha*/
@@ -6871,30 +6887,30 @@
                     16 && (a.choicesColors = /*labelColors*/
                         u[4]), o & /*boxMinSize*/
                     32 && (a.boxMinSize = /*boxMinSize*/
                         u[5]), o & /*resolved_src*/
                     64 && (a.imageUrl = /*resolved_src*/
                         u[6]), !n && o & /*value*/
                     1 && (n = !0, a.value = /*value*/
-                        u[0], ql(() => n = !1)), t.$set(a);
+                        u[0], Ql(() => n = !1)), t.$set(a);
             },
             i(u) {
-                i || (eu(t.$$.fragment, u), i = !0);
+                i || (ru(t.$$.fragment, u), i = !0);
             },
             o(u) {
-                tu(t.$$.fragment, u), i = !1;
+                su(t.$$.fragment, u), i = !1;
             },
             d(u) {
-                Ql(t, u);
+                eu(t, u);
             }
         }
     );
 }
 
-function ru(e, t, n) {
+function lu(e, t, n) {
     let {
         src: i = void 0
     } = t, {
         interactive: r
     } = t, {
         boxesAlpha: s
     } = t, {
@@ -6902,122 +6918,122 @@
     } = t, {
         labelColors: o
     } = t, {
         boxMinSize: a
     } = t, {
         value: f
     } = t, l, h;
-    const c = nu();
+    const m = ou();
 
-    function _(m) {
-        f = m, n(0, f);
+    function _(g) {
+        f = g, n(0, f);
     }
-    const g = () => c("change");
-    return e.$$set = (m) => {
-        "src" in m && n(8, i = m.src), "interactive" in m && n(1, r = m.interactive), "boxesAlpha" in m && n(2, s = m.boxesAlpha), "labelList" in m && n(3, u = m.labelList), "labelColors" in m && n(4, o = m.labelColors), "boxMinSize" in m && n(5, a = m.boxMinSize), "value" in m && n(0, f = m.value);
+    const b = () => m("change");
+    return e.$$set = (g) => {
+        "src" in g && n(8, i = g.src), "interactive" in g && n(1, r = g.interactive), "boxesAlpha" in g && n(2, s = g.boxesAlpha), "labelList" in g && n(3, u = g.labelList), "labelColors" in g && n(4, o = g.labelColors), "boxMinSize" in g && n(5, a = g.boxMinSize), "value" in g && n(0, f = g.value);
     }, e.$$.update = () => {
         if (e.$$.dirty & /*src, latest_src*/
             768) {
             n(6, l = i), n(9, h = i);
-            const m = i;
-            or(m).then((d) => {
-                h === m && n(6, l = d);
+            const g = i;
+            fr(g).then((d) => {
+                h === g && n(6, l = d);
             });
         }
     }, [
         f,
         r,
         s,
         u,
         o,
         a,
         l,
-        c,
+        m,
         i,
         h,
         _,
-        g
+        b
     ];
 }
-class su extends Vl {
+class uu extends Zl {
     constructor(t) {
-        super(), Jl(this, t, ru, iu, $l, {
+        super(), tu(this, t, lu, au, iu, {
             src: 8,
             interactive: 1,
             boxesAlpha: 2,
             labelList: 3,
             labelColors: 4,
             boxMinSize: 5,
             value: 0
         });
     }
 }
 const {
-    SvelteComponent: ou,
-    attr: au,
-    check_outros: lu,
-    create_component: uu,
-    destroy_component: fu,
-    detach: hu,
-    element: cu,
-    group_outros: mu,
-    init: _u,
-    insert: du,
-    mount_component: bu,
-    safe_not_equal: gu,
+    SvelteComponent: fu,
+    attr: hu,
+    check_outros: cu,
+    create_component: mu,
+    destroy_component: _u,
+    detach: du,
+    element: bu,
+    group_outros: gu,
+    init: pu,
+    insert: vu,
+    mount_component: yu,
+    safe_not_equal: Eu,
     toggle_class: ie,
-    transition_in: ht,
-    transition_out: fn
+    transition_in: mt,
+    transition_out: hn
 } = window.__gradio__svelte__internal;
 
 function fi(e) {
     let t, n;
-    return t = new su({
+    return t = new uu({
         props: {
             src: (
                 /*samples_dir*/
                 e[1] + /*value*/
                 e[0].path
             ),
             alt: ""
         }
     }), {
         c() {
-            uu(t.$$.fragment);
+            mu(t.$$.fragment);
         },
         m(i, r) {
-            bu(t, i, r), n = !0;
+            yu(t, i, r), n = !0;
         },
         p(i, r) {
             const s = {};
             r & /*samples_dir, value*/
                 3 && (s.src = /*samples_dir*/
                     i[1] + /*value*/
                     i[0].path), t.$set(s);
         },
         i(i) {
-            n || (ht(t.$$.fragment, i), n = !0);
+            n || (mt(t.$$.fragment, i), n = !0);
         },
         o(i) {
-            fn(t.$$.fragment, i), n = !1;
+            hn(t.$$.fragment, i), n = !1;
         },
         d(i) {
-            fu(t, i);
+            _u(t, i);
         }
     };
 }
 
-function pu(e) {
+function wu(e) {
     let t, n, i = (
         /*value*/
         e[0] && fi(e)
     );
     return {
         c() {
-            t = cu("div"), i && i.c(), au(t, "class", "container svelte-1sgcyba"), ie(
+            t = bu("div"), i && i.c(), hu(t, "class", "container svelte-1sgcyba"), ie(
                 t,
                 "table",
                 /*type*/
                 e[2] === "table"
             ), ie(
                 t,
                 "gallery",
@@ -7032,22 +7048,22 @@
                 t,
                 "border",
                 /*value*/
                 e[0]
             );
         },
         m(r, s) {
-            du(r, t, s), i && i.m(t, null), n = !0;
+            vu(r, t, s), i && i.m(t, null), n = !0;
         },
         p(r, [s]) {
             /*value*/
             r[0] ? i ? (i.p(r, s), s & /*value*/
-                1 && ht(i, 1)) : (i = fi(r), i.c(), ht(i, 1), i.m(t, null)) : i && (mu(), fn(i, 1, 1, () => {
+                1 && mt(i, 1)) : (i = fi(r), i.c(), mt(i, 1), i.m(t, null)) : i && (gu(), hn(i, 1, 1, () => {
                 i = null;
-            }), lu()), (!n || s & /*type*/
+            }), cu()), (!n || s & /*type*/
                 4) && ie(
                 t,
                 "table",
                 /*type*/
                 r[2] === "table"
             ), (!n || s & /*type*/
                 4) && ie(
@@ -7066,46 +7082,46 @@
                 t,
                 "border",
                 /*value*/
                 r[0]
             );
         },
         i(r) {
-            n || (ht(i), n = !0);
+            n || (mt(i), n = !0);
         },
         o(r) {
-            fn(i), n = !1;
+            hn(i), n = !1;
         },
         d(r) {
-            r && hu(t), i && i.d();
+            r && du(t), i && i.d();
         }
     };
 }
 
-function vu(e, t, n) {
+function xu(e, t, n) {
     let {
         value: i
     } = t, {
         samples_dir: r
     } = t, {
         type: s
     } = t, {
         selected: u = !1
     } = t;
     return e.$$set = (o) => {
         "value" in o && n(0, i = o.value), "samples_dir" in o && n(1, r = o.samples_dir), "type" in o && n(2, s = o.type), "selected" in o && n(3, u = o.selected);
     }, [i, r, s, u];
 }
-class Eu extends ou {
+class Hu extends fu {
     constructor(t) {
-        super(), _u(this, t, vu, pu, gu, {
+        super(), pu(this, t, xu, wu, Eu, {
             value: 0,
             samples_dir: 1,
             type: 2,
             selected: 3
         });
     }
 }
 export {
-    Eu as
+    Hu as
     default
 };
```

### Comparing `gradio_image_annotation-0.0.4/backend/gradio_image_annotation/templates/example/style.css` & `gradio_image_annotation-0.0.5/backend/gradio_image_annotation/templates/example/style.css`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/demo/app.py` & `gradio_image_annotation-0.0.5/demo/app.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -31,26 +31,26 @@
         {k: box[k]
             for k in box if k in ("xmin", "ymin", "xmax", "ymax", "label")}
         for box in annotations["boxes"]
     ]
 
 
 with gr.Blocks() as demo:
-    with gr.Tab("Crop"):
-        with gr.Row():
-            annotator_crop = image_annotator(example, image_type="numpy")
-            image_crop = gr.Image()
-        button_crop = gr.Button("Crop")
-        button_crop.click(crop, annotator_crop, image_crop)
     with gr.Tab("Object annotation"):
         annotator = image_annotator(
             {"image": "https://gradio-builds.s3.amazonaws.com/demo-files/base.png"},
             label_list=["Person", "Vehicle"],
             label_colors=[(0, 255, 0), (255, 0, 0)],
         )
         button_get = gr.Button("Get bounding boxes")
         json_boxes = gr.JSON()
         button_get.click(get_boxes_json, annotator, json_boxes)
+    with gr.Tab("Crop"):
+        with gr.Row():
+            annotator_crop = image_annotator(example, image_type="numpy")
+            image_crop = gr.Image()
+        button_crop = gr.Button("Crop")
+        button_crop.click(crop, annotator_crop, image_crop)
 
 
 if __name__ == "__main__":
     demo.launch()
```

### Comparing `gradio_image_annotation-0.0.4/demo/css.css` & `gradio_image_annotation-0.0.5/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/demo/space.py` & `gradio_image_annotation-0.0.5/demo/space.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,29 +71,29 @@
         {k: box[k]
             for k in box if k in ("xmin", "ymin", "xmax", "ymax", "label")}
         for box in annotations["boxes"]
     ]
 
 
 with gr.Blocks() as demo:
-    with gr.Tab("Crop"):
-        with gr.Row():
-            annotator_crop = image_annotator(example, image_type="numpy")
-            image_crop = gr.Image()
-        button_crop = gr.Button("Crop")
-        button_crop.click(crop, annotator_crop, image_crop)
     with gr.Tab("Object annotation"):
         annotator = image_annotator(
             {"image": "https://gradio-builds.s3.amazonaws.com/demo-files/base.png"},
             label_list=["Person", "Vehicle"],
             label_colors=[(0, 255, 0), (255, 0, 0)],
         )
         button_get = gr.Button("Get bounding boxes")
         json_boxes = gr.JSON()
         button_get.click(get_boxes_json, annotator, json_boxes)
+    with gr.Tab("Crop"):
+        with gr.Row():
+            annotator_crop = image_annotator(example, image_type="numpy")
+            image_crop = gr.Image()
+        button_crop = gr.Button("Crop")
+        button_crop.click(crop, annotator_crop, image_crop)
 
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
 """, elem_classes=["md-custom"], header_links=True)
```

### Comparing `gradio_image_annotation-0.0.4/frontend/Example.svelte` & `gradio_image_annotation-0.0.5/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/Index.svelte` & `gradio_image_annotation-0.0.5/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/package-lock.json` & `gradio_image_annotation-0.0.5/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/package.json` & `gradio_image_annotation-0.0.5/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/Box.ts` & `gradio_image_annotation-0.0.5/frontend/shared/Box.ts`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/Canvas.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/Canvas.svelte`

 * *Files 3% similar despite different names*

```diff
@@ -131,25 +131,29 @@
 		let ok = detail.ok;
 		if (ok) {
 			if (color === null || color === "") {
 				color = Colors[value.boxes.length % Colors.length];
 			} else {
 				color = colorHexToRGB(color);
 			}
+			let xmin = canvasXmin + ((canvasXmax - canvasXmin) / 3);
+			let xmax = canvasXmax - ((canvasXmax - canvasXmin) / 3);
+			let ymin = canvasYmin + ((canvasYmax - canvasYmin) / 3);
+			let ymax = canvasYmax - ((canvasYmax - canvasYmin) / 3);
 			let box = new Box(
 				draw,
 				canvasXmin,
 				canvasYmin,
 				canvasXmax,
 				canvasYmax,
 				label,
-				Math.round(canvas.width / 3),
-				Math.round(canvas.height / 3),
-				Math.round((2*canvas.width) / 3),
-				Math.round((2*canvas.height) / 3),
+				Math.round(xmin),
+				Math.round(ymin),
+				Math.round(xmax),
+				Math.round(ymax),
 				color,
 				boxAlpha,
 				boxMinSize,
 				scaleFactor
 			);
 			value.boxes = [box, ...value.boxes];
 			draw();
@@ -278,15 +282,31 @@
 			newBoxes.push(box);
 		}
 		value.boxes = newBoxes;
 	}
 
 	$: {
 		value;
+		setImage();
 		parseInputBoxes();
+		resize();
+		draw();
+	}
+
+	function setImage(){
+		if (imageUrl !== null) {
+			if (image === null || image.src != imageUrl) {
+				image = new Image();
+				image.src = imageUrl;
+				image.onload = function(){
+					resize();
+					draw();
+				}
+			}
+		}
 	}
 
 	onMount(() => {
 		if (Array.isArray(choices) && choices.length > 0) {
 			if (!Array.isArray(choicesColors) || choicesColors.length == 0) {
 				for (let i = 0; i < choices.length; i++) {
 					let color = Colors[i % Colors.length];
@@ -294,22 +314,15 @@
 				}
 			}
 		}
 
 		ctx = canvas.getContext("2d");
 		observer.observe(canvas);
 
-		if (imageUrl !== null){
-			image = new Image();
-			image.src = imageUrl;
-			image.onload = function(){
-				resize();
-				draw();
-			}
-		}
+		setImage();
 		resize();
 		draw();
 	});
 	
 	function handleCanvasFocus() {
 		document.addEventListener("keydown", handleKeyPress);
 	}
```

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/ClearImage.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/ClearImage.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/ImageAnnotator.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/ImageAnnotator.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/ImageCanvas.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/ImageCanvas.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/ModalBox.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/ModalBox.svelte`

 * *Files 13% similar despite different names*

```diff
@@ -2,49 +2,51 @@
 	import { BaseColorPicker } from "@gradio/colorpicker";
     import { BaseButton } from "@gradio/button";
     import { BaseDropdown } from "./patched_dropdown/Index.svelte";
 	import { createEventDispatcher } from "svelte";
     import { onMount, onDestroy } from "svelte";
 
     export let label = "";
+    export let currentLabel = "";
     export let choices = [];  // [(label, i)]
     export let choicesColors = [];
     export let color = "";
+    export let currentColor = "";
     
     const dispatch = createEventDispatcher<{
 		change: object;
 	}>();
 
     function dispatchChange(ok: boolean) {
         dispatch("change", {
-            label: label,
-            color: color,
+            label: currentLabel,
+            color: currentColor,
             ok: ok
         });
     }
 
     function onDropDownChange(event) {
         const { detail } = event;
 		let choice = detail;
 
         if (Number.isInteger(choice)) {
             if (Array.isArray(choicesColors) && choice < choicesColors.length) {
-                color = choicesColors[choice];
+                currentColor = choicesColors[choice];
             }
             if (Array.isArray(choices) && choice < choices.length) {
-                label = choices[choice][0];
+                currentLabel = choices[choice][0];
             }
         } else {
-            label = choice;
+            currentLabel = choice;
         }
     }
 
     function onColorChange(event) {
         const { detail } = event;
-		color = detail;
+		currentColor = detail;
     }
 
     function onDropDownEnter(event) {
         onDropDownChange(event);
         dispatchChange(true);
     }
 
@@ -54,39 +56,41 @@
                 dispatchChange(true);
 				break;
 		}
 	}
 
 	onMount(() => {
 		document.addEventListener("keydown", handleKeyPress);
+        currentLabel = label;
+        currentColor = color;
 	});
     
 	onDestroy(() => {
         document.removeEventListener("keydown", handleKeyPress);
   	});
 
 </script>
 
 <div class="modal" id="model-box-edit">
     <div class="modal-container">
         <span class="model-content">
             <div style="margin-right: 10px;">
                 <BaseDropdown
-                    value={label}
+                    value={currentLabel}
                     label="Label"
                     {choices}
                     show_label={false}
                     allow_custom_value={true}
                     on:change={onDropDownChange}
                     on:enter={onDropDownEnter}
                 />
             </div>
             <div style="margin-right: 40px; margin-bottom: 8px;">
                 <BaseColorPicker
-                    value={color}
+                    value={currentColor}
                     label="Color"
                     show_label={false}
                     on:change={onColorChange}
                 />
             </div>
             <div style="margin-right: 8px;">
                 <BaseButton
```

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/utils.ts` & `gradio_image_annotation-0.0.5/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/CHANGELOG.md` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/Dropdown.stories.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/Dropdown.stories.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/Example.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/Index.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/LICENSE` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/LICENSE`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/Multiselect.stories.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/Multiselect.stories.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/README.md` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/README.md`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/dropdown.test.ts` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/dropdown.test.ts`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/shared/Dropdown.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/shared/Dropdown.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/shared/DropdownOptions.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/shared/DropdownOptions.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/shared/Multiselect.svelte` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/shared/Multiselect.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/frontend/shared/patched_dropdown/shared/utils.ts` & `gradio_image_annotation-0.0.5/frontend/shared/patched_dropdown/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/images/demo_1.png` & `gradio_image_annotation-0.0.5/images/demo_1.png`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/images/demo_2.png` & `gradio_image_annotation-0.0.5/images/demo_2.png`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/LICENSE` & `gradio_image_annotation-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.4/README.md` & `gradio_image_annotation-0.0.5/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -46,29 +46,29 @@
         {k: box[k]
             for k in box if k in ("xmin", "ymin", "xmax", "ymax", "label")}
         for box in annotations["boxes"]
     ]
 
 
 with gr.Blocks() as demo:
-    with gr.Tab("Crop"):
-        with gr.Row():
-            annotator_crop = image_annotator(example, image_type="numpy")
-            image_crop = gr.Image()
-        button_crop = gr.Button("Crop")
-        button_crop.click(crop, annotator_crop, image_crop)
     with gr.Tab("Object annotation"):
         annotator = image_annotator(
             {"image": "https://gradio-builds.s3.amazonaws.com/demo-files/base.png"},
             label_list=["Person", "Vehicle"],
             label_colors=[(0, 255, 0), (255, 0, 0)],
         )
         button_get = gr.Button("Get bounding boxes")
         json_boxes = gr.JSON()
         button_get.click(get_boxes_json, annotator, json_boxes)
+    with gr.Tab("Crop"):
+        with gr.Row():
+            annotator_crop = image_annotator(example, image_type="numpy")
+            image_crop = gr.Image()
+        button_crop = gr.Button("Crop")
+        button_crop.click(crop, annotator_crop, image_crop)
 
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
```

### Comparing `gradio_image_annotation-0.0.4/pyproject.toml` & `gradio_image_annotation-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_image_annotation"
-version = "0.0.4"
+version = "0.0.5"
 description = "A Gradio component that can be used to annotate images with bounding boxes."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "Edgar Gracia" }]
 keywords = ["gradio-custom-component", "gradio-template-Image", "bounding box", "annotator", "annotate", "boxes"]
 # Add dependencies here
@@ -36,11 +36,11 @@
 Repository = "https://github.com/edgarGracia/gradio_image_annotator.git"
 Issues = "https://github.com/edgarGracia/gradio_image_annotator/issues"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_image_annotation/templates", "*.pyi", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates"]
+artifacts = ["/backend/gradio_image_annotation/templates", "*.pyi", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates", "backend/gradio_image_annotation/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_image_annotation"]
```

### Comparing `gradio_image_annotation-0.0.4/PKG-INFO` & `gradio_image_annotation-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_image_annotation
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Gradio component that can be used to annotate images with bounding boxes.
 Project-URL: Repository, https://github.com/edgarGracia/gradio_image_annotator.git
 Project-URL: Issues, https://github.com/edgarGracia/gradio_image_annotator/issues
 Author: Edgar Gracia
 License-Expression: MIT
 License-File: LICENSE
 Keywords: annotate,annotator,bounding box,boxes,gradio-custom-component,gradio-template-Image
@@ -75,29 +75,29 @@
         {k: box[k]
             for k in box if k in ("xmin", "ymin", "xmax", "ymax", "label")}
         for box in annotations["boxes"]
     ]
 
 
 with gr.Blocks() as demo:
-    with gr.Tab("Crop"):
-        with gr.Row():
-            annotator_crop = image_annotator(example, image_type="numpy")
-            image_crop = gr.Image()
-        button_crop = gr.Button("Crop")
-        button_crop.click(crop, annotator_crop, image_crop)
     with gr.Tab("Object annotation"):
         annotator = image_annotator(
             {"image": "https://gradio-builds.s3.amazonaws.com/demo-files/base.png"},
             label_list=["Person", "Vehicle"],
             label_colors=[(0, 255, 0), (255, 0, 0)],
         )
         button_get = gr.Button("Get bounding boxes")
         json_boxes = gr.JSON()
         button_get.click(get_boxes_json, annotator, json_boxes)
+    with gr.Tab("Crop"):
+        with gr.Row():
+            annotator_crop = image_annotator(example, image_type="numpy")
+            image_crop = gr.Image()
+        button_crop = gr.Button("Crop")
+        button_crop.click(crop, annotator_crop, image_crop)
 
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
```

