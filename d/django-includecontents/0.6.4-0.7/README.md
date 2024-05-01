# Comparing `tmp/django_includecontents-0.6.4.tar.gz` & `tmp/django_includecontents-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_includecontents-0.6.4.tar", last modified: Sun Apr 21 23:17:50 2024, max compression
+gzip compressed data, was "django_includecontents-0.7.tar", last modified: Wed May  1 05:06:06 2024, max compression
```

## Comparing `django_includecontents-0.6.4.tar` & `django_includecontents-0.7.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     5368 2024-04-21 20:37:00.117665 django_includecontents-0.6.4/README.md
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.6.4/includecontents/__init__.py
--rw-r--r--   0        0        0     1000 2024-04-19 05:13:37.190112 django_includecontents-0.6.4/includecontents/backend.py
--rw-r--r--   0        0        0     4596 2024-04-19 05:31:33.346108 django_includecontents-0.6.4/includecontents/base.py
--rw-r--r--   0        0        0     1401 2024-04-09 04:42:05.196722 django_includecontents-0.6.4/includecontents/engine.py
--rw-r--r--   0        0        0     1663 2024-04-18 05:37:15.283141 django_includecontents-0.6.4/includecontents/loaders.py
--rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.6.4/includecontents/templatetags/__init__.py
--rw-r--r--   0        0        0    15829 2024-04-21 23:12:37.078245 django_includecontents-0.6.4/includecontents/templatetags/includecontents.py
--rw-r--r--   0        0        0     1220 2024-04-21 23:17:50.210404 django_includecontents-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      144 2024-04-19 05:31:17.752738 django_includecontents-0.6.4/tests/settings.py
--rw-r--r--   0        0        0      168 2024-04-18 05:37:15.283141 django_includecontents-0.6.4/tests/templates/components/card.html
--rw-r--r--   0        0        0      163 2024-04-21 20:37:00.117665 django_includecontents-0.6.4/tests/templates/components/card_extend.html
--rw-r--r--   0        0        0       42 2024-04-21 22:40:07.372787 django_includecontents-0.6.4/tests/templates/components/empty_props.html
--rw-r--r--   0        0        0       97 2024-04-21 23:11:42.498021 django_includecontents-0.6.4/tests/templates/components/nested_attrs.html
--rw-r--r--   0        0        0       81 2024-04-09 04:52:09.297567 django_includecontents-0.6.4/tests/templates/multiline.html
--rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.6.4/tests/templates/test_component/attrs.html
--rw-r--r--   0        0        0      162 2024-04-18 05:37:15.283141 django_includecontents-0.6.4/tests/templates/test_component/extend_class.html
--rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.6.4/tests/templates/test_component/index.html
--rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.6.4/tests/templates/test_component/missing_attr.html
--rw-r--r--   0        0        0       24 2024-04-09 21:51:57.449090 django_includecontents-0.6.4/tests/templates/test_component/missing_closing_tag.html
--rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.6.4/tests/templates/test_tag/basic.html
--rw-r--r--   0        0        0       54 2024-04-21 20:37:00.117665 django_includecontents-0.6.4/tests/templates/test_tag/inner.html
--rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.6.4/tests/templates/test_tag/with_attr.html
--rw-r--r--   0        0        0     2326 2024-04-21 23:12:48.301625 django_includecontents-0.6.4/tests/test_component.py
--rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.6.4/tests/test_multiline.py
--rw-r--r--   0        0        0      448 2024-04-21 23:14:49.298302 django_includecontents-0.6.4/tests/test_tag.py
--rw-r--r--   0        0        0     6384 1970-01-01 00:00:00.000000 django_includecontents-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     7760 2024-05-01 04:48:00.043238 django_includecontents-0.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.7/includecontents/__init__.py
+-rw-r--r--   0        0        0     1000 2024-04-19 05:13:37.190112 django_includecontents-0.7/includecontents/backend.py
+-rw-r--r--   0        0        0     4779 2024-05-01 04:41:54.339196 django_includecontents-0.7/includecontents/base.py
+-rw-r--r--   0        0        0     1401 2024-04-09 04:42:05.196722 django_includecontents-0.7/includecontents/engine.py
+-rw-r--r--   0        0        0     1663 2024-04-18 05:37:15.283141 django_includecontents-0.7/includecontents/loaders.py
+-rw-r--r--   0        0        0        0 2024-04-09 04:42:05.196722 django_includecontents-0.7/includecontents/templatetags/__init__.py
+-rw-r--r--   0        0        0    16458 2024-05-01 04:47:18.123159 django_includecontents-0.7/includecontents/templatetags/includecontents.py
+-rw-r--r--   0        0        0     1217 2024-05-01 05:06:06.539571 django_includecontents-0.7/pyproject.toml
+-rw-r--r--   0        0        0      144 2024-04-19 05:31:17.752738 django_includecontents-0.7/tests/settings.py
+-rw-r--r--   0        0        0      163 2024-04-21 20:37:00.117665 django_includecontents-0.7/tests/templates/components/card-extend.html
+-rw-r--r--   0        0        0      168 2024-04-18 05:37:15.283141 django_includecontents-0.7/tests/templates/components/card.html
+-rw-r--r--   0        0        0       42 2024-04-21 22:40:07.372787 django_includecontents-0.7/tests/templates/components/empty-props.html
+-rw-r--r--   0        0        0       35 2024-05-01 04:25:18.356900 django_includecontents-0.7/tests/templates/components/escape-props.html
+-rw-r--r--   0        0        0       97 2024-04-21 23:11:42.498021 django_includecontents-0.7/tests/templates/components/nested-attrs.html
+-rw-r--r--   0        0        0       81 2024-04-30 04:36:00.000113 django_includecontents-0.7/tests/templates/multiline.html
+-rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.7/tests/templates/test_component/attrs.html
+-rw-r--r--   0        0        0      162 2024-05-01 00:06:23.461690 django_includecontents-0.7/tests/templates/test_component/extend_class.html
+-rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.7/tests/templates/test_component/index.html
+-rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.7/tests/templates/test_component/missing_attr.html
+-rw-r--r--   0        0        0       24 2024-04-30 04:36:02.466786 django_includecontents-0.7/tests/templates/test_component/missing_closing_tag.html
+-rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.7/tests/templates/test_tag/basic.html
+-rw-r--r--   0        0        0       54 2024-04-21 20:37:00.117665 django_includecontents-0.7/tests/templates/test_tag/inner.html
+-rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.7/tests/templates/test_tag/with_attr.html
+-rw-r--r--   0        0        0     3371 2024-05-01 04:40:17.229002 django_includecontents-0.7/tests/test_component.py
+-rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.7/tests/test_multiline.py
+-rw-r--r--   0        0        0      924 2024-05-01 00:43:10.666578 django_includecontents-0.7/tests/test_tag.py
+-rw-r--r--   0        0        0     8773 1970-01-01 00:00:00.000000 django_includecontents-0.7/PKG-INFO
```

### Comparing `django_includecontents-0.6.4/README.md` & `django_includecontents-0.7/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 ```jinja
 {% load includecontents %}
 {% includecontents "hello.html" %}
     <p>World</p>
 {% endincludecontents %}
 ```
 
-It also provides a simple Django template engine that extends this tag to work
-like an HTML component.
+It also provides an optional Django template engine that extends this tag to
+work like an HTML component.
 
-In this example, it will include and render `components/card.html`:
+In this example, it will include and render `components/pretty-card.html`:
 
 ```html
-<include:card title="Hello">
+<include:pretty-card title="Hello">
   <p>World</p>
-</include:card>
+</include:pretty-card>
 ```
 
 This engine also allows for multi-line template tags. For example:
 
 ```jinja
 {% if 
   user.is_authenticated
@@ -35,44 +35,42 @@
 
 ## Installation
 
 ```bash
 pip install django-includecontents
 ```
 
-To use the custom template engine, replace the default `DjangoTemplates` backend in your settings:
+Either install the custom template engine or just add this app to your `INSTALLED_APPS`.
+
+### Template engine installation
+
+Replace the default `DjangoTemplates` backend in your settings:
 
 ```python
 TEMPLATES = [
     {
         'BACKEND': 'includecontents.backend.Templates',
         ...
     },
 ]
 ```
 
-This engine also adds `includecontents` to the built-in tags so there is no need to load it.
+This engine also adds `includecontents` to the built-in tag libraries so there is no need to load it in your templates.
+
+### Basic installation
 
-If you don't want the custom engine, just add this app to your `INSTALLED_APPS` and load the tag in your templates:
+Alternatively, add this app to your `INSTALLED_APPS` and use `{% load includecontents %}` in your templates:
 
 ```python
 INSTALLED_APPS = [
     ...
     'includecontents',
 ]
 ```
 
-```jinja
-{% load includecontents %}
-
-...
-
-{% includecontents %}...{% endincludecontents %}
-```
-
 ## Template tag usage
 
 The `includecontents` tag works like the `include` tag but the contents is rendered and passed to the included template as a `contents` variable.
 
 ```jinja
 {% includecontents "hello.html" %}
     <p>World</p>
@@ -105,44 +103,46 @@
   </div>
   {% endif %}
 </div>
 ```
 
 ## HTML Components Usage
 
+This requires the custom template engine to be installed.
+
 Create a `components` directory in your templates directory. This is where you will put your component templates that are used via the HTML component format.
 These components are normal Django templates that will be rendered with an isolated context. The context is passed to the component via component's attributes.
 
-Components must be CamelCase and not match any standard HTML tags.
+Components not match any standard HTML tags. Actually, it's best practice to name them as HTML custom elements (1 or more ASCII letters; a hyphen; 1 or more more ASCII letters, digits or hyphens).
 
-For example, a `components/card.html` template could look like:
+For example, a `components/my-card.html` template could look like:
 
 ```html
 <div class="card">
   <h2>{{ title }}</h2>
   <div class="content">
     {{ contents }}
   </div>
 </div>
 ```
 
 Which will allow you to use it like this (without the need to load any template library):
 
 ```html
-<include:card title="Hello">
+<include:my-card title="Hello">
   <p>World</p>
-</include:card>
+</include:my-card>
 ```
 
 You can use named [`{% contents %}` blocks](#named-contents-blocks), just like with the `includecontents` tag.
 
 Some HTML formatters (like prettier) insist on quoting HTML attribute values, you can avoid this by optionally wrapping template values in `{}`:
 
 ```html
-<include:card title={mytitle}></include:card>
+<include:my-card title={mytitle} />
 ``` 
 
 ### Component Props
 
 You can define the required or default props of the component in a comment at the top of its template that begins with `props `  (or `def ` to match what JinjaX uses). An exception will be raised if a required prop is not provided.
 
 Any other attributes passed to the component that are not listed in this definition will be added to an `attrs` context variable that can render them as HTML attributes.
@@ -167,15 +167,15 @@
 
 If you want to provide multiple groups of undefined attributes, you can use `group.name` as the format.
 Then render them with `{{ attrs.group }}` (or `{% attrs.group %}` if you want fallback values).
 
 For example to call a component like this:
 
 ```html
-<include:field label="Name" name="first_name" value="John" input.class="wide"></include:field>
+<include:form-field label="Name" name="first_name" value="John" input.class="wide"></include:form-field>
 ```
 
 It could be defined like this:
 
 ```jinja
 {# props value, label="" #}
 
@@ -183,14 +183,34 @@
   {% if label %}{{ '<label>'|safe }}{% endif %}
   {{ label }}
   <input {% attrs.input type="text" value=value %}>
   {% if label %}{{ '</label>'|safe }}{% endif %}
 </div>
 ```
 
+#### Kebab-cased props
+
+Non-defined props can be "kebab-cased", for example: 
+
+```html
+<include:example my-prop="value">
+```
+
+To access a kebab-cased prop to a via the ``attrs`` variable, use its CamelCase equivalent. The ``{% attrs %}`` tag works with kebab-case fine though::
+
+```jinja
+{# props #}
+
+{% attrs my-prop="fallback" %}
+
+{% if attrs.myProp %}
+my-prop is explicitly set to {{ attrs.myProp }}
+{% endif %}
+```
+
 #### Extended / conditional classes
 
 Prepend your class list with `"& "` to have it extended rather than replaced:
 
 ```jinja
 {% attrs class="lg" %}        {# sets default class attribute to "lg" but can be overridden #}
 {% attrs class="& lg p-3" %}  {# always add 'lg p-3' classes #}
@@ -204,11 +224,71 @@
 {% attrs class:lg=large %} {# adds 'lg' class if large prop is truthy #}
 {% attrs class:lg %}       {# always adds 'lg' class #}
 ```
 
 You can use this same conditional format on the component attributes directly:
 
 ```html
-<include:card title="Hello" class:lg={is_large}>
+<include:my-card title="Hello" class:lg={is_large}>
   <p>World</p>
-</include:card>
+</include:my-card>
 ```
+
+#### Conditional classes in tailwindcss
+
+Add this transform in your `tailwind.config.js` so that Tailwind picks up the
+Svelte-like class directives:
+
+```js
+/** @type {import('tailwindcss').Config} */
+module.exports = {
+  content: {
+    files: ["**/*.{html,js}", "!node_modules"],
+    transform: {
+      // Also handle Svelte-like class:class-name directives
+      html: (content) => content.replace(/(\w):([-\w]+)/g, '$1 "$2" '),
+    },
+  },
+  ...
+```
+
+## Prettier formatting
+
+While not part of this package, `django-includecontents` plays very well with the [`prettier-plugin-jinja-template` plugin](https://www.npmjs.com/package/prettier-plugin-jinja-template) for Prettier.
+This plugin can provide consistent formatting for your Django (and Jinja, obviously) templates.
+
+First install it with `npm install --save-dev prettier-plugin-jinja-template`.
+
+Then create a `.prettierrc` file in your project root with the following content:
+
+```json
+{
+  "plugins": ["prettier-plugin-jinja-template"],
+  "overrides": [
+    {
+      "files": ["**/{templates,jinja2}/**/*.html"],
+      "options": {
+        "parser": "jinja-template",
+        "quoteAttributes": false
+      }
+    }
+  ]
+}
+```
+
+### VScode formatting
+
+To use this Prettier formatting within VScode, use the following two extensions:
+
+* [Django](https://marketplace.visualstudio.com/items?itemName=batisteo.vscode-django)
+* [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
+
+Add this to your settings (`Ctrl-P`, paste `>Preferences: Open Workspace Settings (JSON)`):
+
+```json
+{
+  "[django-html]": {
+    "editor.formatOnSave": true,
+    "editor.defaultFormatter": "esbenp.prettier-vscode"
+  },
+}
+```
```

### Comparing `django_includecontents-0.6.4/includecontents/backend.py` & `django_includecontents-0.7/includecontents/backend.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.6.4/includecontents/base.py` & `django_includecontents-0.7/includecontents/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,17 @@
             return nodelist
         except Exception as e:
             if self.engine.debug:
                 e.template_debug = self.get_exception_info(e, e.token)  # type: ignore
             raise
 
 
-tag_re = re.compile(r"({%.*?%}|{{.*?}}|{#.*?#}|</?include:.*?>)", re.DOTALL)
+tag_re = re.compile(
+    r"({%.*?%}|{{.*?}}|{#.*?#}|</?include:(?:\"[^\"]*\"|'[^']*'|.)*?>)", re.DOTALL
+)
 
 
 class Lexer(django.template.base.Lexer):
     def tokenize(self):
         """
         Return a list of tokens from a given template_string.
         """
@@ -70,26 +72,29 @@
                 django.template.base.TokenType.BLOCK,
                 token_string,
                 position,
                 lineno,
             )
         elif in_tag and token_string.startswith("<include:"):
             content = token_string[1:-1].strip()
+            self_closing = content.endswith("/")
+            if self_closing:
+                content = content[:-1].strip()
             # Strip {} from attributes
             bits = list(smart_split(content))
             tag_name = bits.pop(0)
             attrs = []
             for attr in bits:
                 if group := re.match(r"([-:.\w]+)=\{(.+)\}", attr):
                     attr = f"{group[1]}={group[2]}"
                 attrs.append(attr)
             # Build the includecontents tag
             content = [
                 "includecontents",
-                f"_{tag_name}",
+                f"_{tag_name}{'/' if self_closing else ''}",
                 f'"components/{tag_name[8:]}.html"',
             ]
             if attrs:
                 content.append("with")
                 content.extend(attrs)
             return django.template.base.Token(
                 django.template.base.TokenType.BLOCK,
```

### Comparing `django_includecontents-0.6.4/includecontents/engine.py` & `django_includecontents-0.7/includecontents/engine.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.6.4/includecontents/loaders.py` & `django_includecontents-0.7/includecontents/loaders.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.6.4/includecontents/templatetags/includecontents.py` & `django_includecontents-0.7/includecontents/templatetags/includecontents.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from typing import Any
 
 from django import template
 from django.template import TemplateSyntaxError, Variable
 from django.template.base import FilterExpression, NodeList, Parser, TokenType
 from django.template.context import Context
 from django.template.loader_tags import IncludeNode, construct_relative_path, do_include
-from django.utils.html import escape
+from django.utils.html import conditional_escape
 from django.utils.safestring import mark_safe
 from django.utils.text import smart_split
 
 from includecontents.base import Template
 
 register = template.Library()
 
-re_tag = re.compile(r"^includecontents _([A-Z]\w+)")
+re_camel_case = re.compile(r"(?<=.)([A-Z])")
 
 
 @register.tag
 def includecontents(parser, token):
     """
     An extension of the ``{% include %}`` tag which loads a template and
     renders it with the current context. It accepts all the standard
@@ -60,56 +60,63 @@
             {% else %}
                 <small>Default note only shown if named area wasn't provided.</small>
             {% endif %}
         </div>
     """
     bits = token.split_contents()
     # If this was an HTML tag, it's second element is the tag name prefixed with an
-    # underscore.
+    # underscore (and ending with a slash if it's self-closing).
     if len(bits) >= 2 and bits[1].startswith("_"):
         token_name = f"<{bits[1][1:]}>"
         # Rewrite the token name on the command stack for better error messages.
         parser.command_stack[-1] = (token_name,) + parser.command_stack[-1][1:]
         # Replace the token contents to use the rewritten token name.
         bits[1] = token_name
         del bits[0]
         # In tag mode, allow boolean attributes to be set without a value.
         for i, bit in enumerate(bits[3:], start=3):
             if "=" not in bit:
                 bits[i] = f"{bit}=True"
         # Split out nested attributes (those with a dot in the name).
         new_bits = []
-        nested_attrs = {}
-        for bit in bits:
-            if match := re.match(r"(^\w+[.:][-.\w:]+)(?:=(.+))?", bit):
+        advanced_attrs = {}
+        for i, bit in enumerate(bits):
+            if i < 3:
+                new_bits.append(bit)
+            elif match := re.match(r"(^\w+[.:][-.\w:]+)(?:=(.+))?", bit):
+                # Nested attrs can't be handled by the standard include tag.
                 attr, value = match.groups()
-                nested_attrs[attr] = parser.compile_filter(value or "True")
+                advanced_attrs[attr] = parser.compile_filter(value or "True")
+            elif "-" in bit.split("=", 1)[0]:
+                # Attributes with a dash also can't be handled by the standard include.
+                attr, value = bit.split("=", 1)
+                advanced_attrs[attr] = parser.compile_filter(value)
             else:
                 new_bits.append(bit)
         if new_bits and new_bits[-1] == "with":
             new_bits = new_bits[:-1]
         bits = new_bits
         token.contents = " ".join(bits)
     else:
         token_name = bits[0]
-        nested_attrs = {}
+        advanced_attrs = {}
     if len(bits) < 2:
         raise TemplateSyntaxError(
             f"{token_name} tag takes at least one argument: the name of the template"
         )
     nodelist, named_nodelists = get_contents_nodelists(parser, token_name)
     include_node = do_include(parser, token)
     include_node.origin = parser.origin
     isolated_context = (
         False if token_name.startswith("<") else include_node.isolated_context
     )
     include_node.isolated_context = False
     return IncludeContentsNode(
         token_name=token_name,
-        nested_attrs=nested_attrs,
+        nested_attrs=advanced_attrs,
         include_node=include_node,
         nodelist=nodelist,
         named_nodelists=named_nodelists,
         isolated_context=isolated_context,
     )
 
 
@@ -251,14 +258,16 @@
             template = template.template
         return template
 
 
 def get_contents_nodelists(
     parser: Parser, token_name: str
 ) -> tuple[NodeList, dict[str, NodeList]]:
+    if token_name.endswith("/>"):
+        return NodeList(), {}
     end_tag = (
         f"</{token_name[1:]}" if token_name.startswith("<") else f"end{token_name}"
     )
     named_nodelists = {}
     default = []
 
     while parser.tokens:
@@ -306,14 +315,16 @@
 
     def __getattr__(self, key):
         if key not in self._nested_attrs:
             raise AttributeError(key)
         return self._nested_attrs[key]
 
     def __getitem__(self, key):
+        if key not in self._attrs:
+            key = re_camel_case.sub(r"-\1", key).lower()
         return self._attrs[key]
 
     def __setitem__(self, key, value):
         if "." in key:
             nested_key, key = key.split(".", 1)
             nested_attrs = self._nested_attrs.setdefault(nested_key, Attrs())
             nested_attrs[key] = value
@@ -338,15 +349,15 @@
 
     def __len__(self):
         return len(self._attrs)
 
     def __str__(self):
         return mark_safe(
             " ".join(
-                (f'{key}="{escape(value)}"' if value is not True else key)
+                (f'{key}="{conditional_escape(value)}"' if value is not True else key)
                 for key, value in self.all_attrs()
                 if value is not None
             )
         )
 
     def all_attrs(self):
         extended = {}
```

### Comparing `django_includecontents-0.6.4/pyproject.toml` & `django_includecontents-0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "django-includecontents"
-version = "0.6.4"
+version = "0.7"
 description = "Django includecontents component-like tag"
 authors = [
     { name = "Chris Beaven", email = "smileychris@gmail.com" },
 ]
 dependencies = [
     "django",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Framework :: Django",
     "Framework :: Django :: 4.2",
     "Framework :: Django :: 5.0",
     "Programming Language :: Python :: 3",
```

### Comparing `django_includecontents-0.6.4/tests/test_component.py` & `django_includecontents-0.7/tests/test_component.py`

 * *Files 24% similar despite different names*

```diff
@@ -79,29 +79,64 @@
 </main>
 """
     )
 
 
 def test_empty_props():
     output = Template(
-        "Attrs: <include:empty_props id='1' hello></include:empty_props>"
+        "Attrs: <include:empty-props id='1' hello></include:empty-props>"
     ).render(Context())
     assert output == 'Attrs: id="1" hello/'
 
 
 def test_only_advanced_props():
     output = Template(
-        "Attrs: <include:empty_props inner.id='1'></include:empty_props>"
+        "Attrs: <include:empty-props inner.id='1'></include:empty-props>"
     ).render(Context())
     assert output == 'Attrs: /id="1"'
 
 
 def test_nested_attrs():
     output = Template(
-        "<include:nested_attrs inner.class='2' class='1'></include:nested_attrs>"
+        "<include:nested-attrs inner.class='2' class='1'></include:nested-attrs>"
     ).render(Context())
     assert (
         output
         == """\
 <div class="1 main"></div>
 <div class="2 inner"></div>"""
     )
+
+
+def test_self_closing():
+    output = Template("Attrs: <include:empty-props hello />").render(Context())
+    assert output == "Attrs: hello/"
+
+
+def test_kebab_props():
+    output = Template(
+        "Attrs: "
+        '<include:empty-props x-data="{foo: bar}" inner.hx-swap="innerHTML">'
+        "</include:empty-props>"
+    ).render(Context())
+    assert output == 'Attrs: x-data="{foo: bar}"/hx-swap="innerHTML"'
+
+
+def test_safe_constants():
+    output = Template(
+        """<include:escape-props test="2>1" another="3>2"></include:escape-props>"""
+    ).render(Context())
+    assert output == 'test="2>1" another="3>2"'
+
+
+def test_safe_constants_fallback():
+    output = Template("""<include:escape-props></include:escape-props>""").render(
+        Context()
+    )
+    assert output == 'test="5>4"'
+
+
+def test_escape_variables():
+    output = Template(
+        """<include:escape-props test=somevar another="3>2"></include:escape-props>"""
+    ).render(Context({"somevar": '2>1"'}))
+    assert output == 'test="2&gt;1&quot;" another="3>2"'
```

### Comparing `django_includecontents-0.6.4/PKG-INFO` & `django_includecontents-0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-includecontents
-Version: 0.6.4
+Version: 0.7
 Summary: Django includecontents component-like tag
 Author-Email: Chris Beaven <smileychris@gmail.com>
 License: MIT
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Programming Language :: Python :: 3
@@ -33,23 +33,23 @@
 ```jinja
 {% load includecontents %}
 {% includecontents "hello.html" %}
     <p>World</p>
 {% endincludecontents %}
 ```
 
-It also provides a simple Django template engine that extends this tag to work
-like an HTML component.
+It also provides an optional Django template engine that extends this tag to
+work like an HTML component.
 
-In this example, it will include and render `components/card.html`:
+In this example, it will include and render `components/pretty-card.html`:
 
 ```html
-<include:card title="Hello">
+<include:pretty-card title="Hello">
   <p>World</p>
-</include:card>
+</include:pretty-card>
 ```
 
 This engine also allows for multi-line template tags. For example:
 
 ```jinja
 {% if 
   user.is_authenticated
@@ -61,44 +61,42 @@
 
 ## Installation
 
 ```bash
 pip install django-includecontents
 ```
 
-To use the custom template engine, replace the default `DjangoTemplates` backend in your settings:
+Either install the custom template engine or just add this app to your `INSTALLED_APPS`.
+
+### Template engine installation
+
+Replace the default `DjangoTemplates` backend in your settings:
 
 ```python
 TEMPLATES = [
     {
         'BACKEND': 'includecontents.backend.Templates',
         ...
     },
 ]
 ```
 
-This engine also adds `includecontents` to the built-in tags so there is no need to load it.
+This engine also adds `includecontents` to the built-in tag libraries so there is no need to load it in your templates.
+
+### Basic installation
 
-If you don't want the custom engine, just add this app to your `INSTALLED_APPS` and load the tag in your templates:
+Alternatively, add this app to your `INSTALLED_APPS` and use `{% load includecontents %}` in your templates:
 
 ```python
 INSTALLED_APPS = [
     ...
     'includecontents',
 ]
 ```
 
-```jinja
-{% load includecontents %}
-
-...
-
-{% includecontents %}...{% endincludecontents %}
-```
-
 ## Template tag usage
 
 The `includecontents` tag works like the `include` tag but the contents is rendered and passed to the included template as a `contents` variable.
 
 ```jinja
 {% includecontents "hello.html" %}
     <p>World</p>
@@ -131,44 +129,46 @@
   </div>
   {% endif %}
 </div>
 ```
 
 ## HTML Components Usage
 
+This requires the custom template engine to be installed.
+
 Create a `components` directory in your templates directory. This is where you will put your component templates that are used via the HTML component format.
 These components are normal Django templates that will be rendered with an isolated context. The context is passed to the component via component's attributes.
 
-Components must be CamelCase and not match any standard HTML tags.
+Components not match any standard HTML tags. Actually, it's best practice to name them as HTML custom elements (1 or more ASCII letters; a hyphen; 1 or more more ASCII letters, digits or hyphens).
 
-For example, a `components/card.html` template could look like:
+For example, a `components/my-card.html` template could look like:
 
 ```html
 <div class="card">
   <h2>{{ title }}</h2>
   <div class="content">
     {{ contents }}
   </div>
 </div>
 ```
 
 Which will allow you to use it like this (without the need to load any template library):
 
 ```html
-<include:card title="Hello">
+<include:my-card title="Hello">
   <p>World</p>
-</include:card>
+</include:my-card>
 ```
 
 You can use named [`{% contents %}` blocks](#named-contents-blocks), just like with the `includecontents` tag.
 
 Some HTML formatters (like prettier) insist on quoting HTML attribute values, you can avoid this by optionally wrapping template values in `{}`:
 
 ```html
-<include:card title={mytitle}></include:card>
+<include:my-card title={mytitle} />
 ``` 
 
 ### Component Props
 
 You can define the required or default props of the component in a comment at the top of its template that begins with `props `  (or `def ` to match what JinjaX uses). An exception will be raised if a required prop is not provided.
 
 Any other attributes passed to the component that are not listed in this definition will be added to an `attrs` context variable that can render them as HTML attributes.
@@ -193,15 +193,15 @@
 
 If you want to provide multiple groups of undefined attributes, you can use `group.name` as the format.
 Then render them with `{{ attrs.group }}` (or `{% attrs.group %}` if you want fallback values).
 
 For example to call a component like this:
 
 ```html
-<include:field label="Name" name="first_name" value="John" input.class="wide"></include:field>
+<include:form-field label="Name" name="first_name" value="John" input.class="wide"></include:form-field>
 ```
 
 It could be defined like this:
 
 ```jinja
 {# props value, label="" #}
 
@@ -209,14 +209,34 @@
   {% if label %}{{ '<label>'|safe }}{% endif %}
   {{ label }}
   <input {% attrs.input type="text" value=value %}>
   {% if label %}{{ '</label>'|safe }}{% endif %}
 </div>
 ```
 
+#### Kebab-cased props
+
+Non-defined props can be "kebab-cased", for example: 
+
+```html
+<include:example my-prop="value">
+```
+
+To access a kebab-cased prop to a via the ``attrs`` variable, use its CamelCase equivalent. The ``{% attrs %}`` tag works with kebab-case fine though::
+
+```jinja
+{# props #}
+
+{% attrs my-prop="fallback" %}
+
+{% if attrs.myProp %}
+my-prop is explicitly set to {{ attrs.myProp }}
+{% endif %}
+```
+
 #### Extended / conditional classes
 
 Prepend your class list with `"& "` to have it extended rather than replaced:
 
 ```jinja
 {% attrs class="lg" %}        {# sets default class attribute to "lg" but can be overridden #}
 {% attrs class="& lg p-3" %}  {# always add 'lg p-3' classes #}
@@ -230,11 +250,71 @@
 {% attrs class:lg=large %} {# adds 'lg' class if large prop is truthy #}
 {% attrs class:lg %}       {# always adds 'lg' class #}
 ```
 
 You can use this same conditional format on the component attributes directly:
 
 ```html
-<include:card title="Hello" class:lg={is_large}>
+<include:my-card title="Hello" class:lg={is_large}>
   <p>World</p>
-</include:card>
+</include:my-card>
 ```
+
+#### Conditional classes in tailwindcss
+
+Add this transform in your `tailwind.config.js` so that Tailwind picks up the
+Svelte-like class directives:
+
+```js
+/** @type {import('tailwindcss').Config} */
+module.exports = {
+  content: {
+    files: ["**/*.{html,js}", "!node_modules"],
+    transform: {
+      // Also handle Svelte-like class:class-name directives
+      html: (content) => content.replace(/(\w):([-\w]+)/g, '$1 "$2" '),
+    },
+  },
+  ...
+```
+
+## Prettier formatting
+
+While not part of this package, `django-includecontents` plays very well with the [`prettier-plugin-jinja-template` plugin](https://www.npmjs.com/package/prettier-plugin-jinja-template) for Prettier.
+This plugin can provide consistent formatting for your Django (and Jinja, obviously) templates.
+
+First install it with `npm install --save-dev prettier-plugin-jinja-template`.
+
+Then create a `.prettierrc` file in your project root with the following content:
+
+```json
+{
+  "plugins": ["prettier-plugin-jinja-template"],
+  "overrides": [
+    {
+      "files": ["**/{templates,jinja2}/**/*.html"],
+      "options": {
+        "parser": "jinja-template",
+        "quoteAttributes": false
+      }
+    }
+  ]
+}
+```
+
+### VScode formatting
+
+To use this Prettier formatting within VScode, use the following two extensions:
+
+* [Django](https://marketplace.visualstudio.com/items?itemName=batisteo.vscode-django)
+* [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
+
+Add this to your settings (`Ctrl-P`, paste `>Preferences: Open Workspace Settings (JSON)`):
+
+```json
+{
+  "[django-html]": {
+    "editor.formatOnSave": true,
+    "editor.defaultFormatter": "esbenp.prettier-vscode"
+  },
+}
+```
```

