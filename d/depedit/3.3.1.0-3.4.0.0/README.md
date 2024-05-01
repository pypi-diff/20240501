# Comparing `tmp/depedit-3.3.1.0.tar.gz` & `tmp/depedit-3.4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depedit-3.3.1.0.tar", last modified: Sun Jan 14 22:29:14 2024, max compression
+gzip compressed data, was "depedit-3.4.0.0.tar", last modified: Wed May  1 21:23:17 2024, max compression
```

## Comparing `depedit-3.3.1.0.tar` & `depedit-3.4.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-01-14 22:29:14.168955 depedit-3.3.1.0/
--rw-rw-rw-   0        0        0    11560 2015-10-19 14:53:17.000000 depedit-3.3.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      728 2024-01-14 22:29:14.168955 depedit-3.3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3047 2022-08-20 14:24:59.000000 depedit-3.3.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-14 22:29:14.143341 depedit-3.3.1.0/depedit/
--rw-rw-rw-   0        0        0       48 2019-01-05 19:27:46.000000 depedit-3.3.1.0/depedit/__init__.py
--rw-rw-rw-   0        0        0       93 2021-04-30 14:53:22.000000 depedit-3.3.1.0/depedit/__main__.py
--rw-rw-rw-   0        0        0    42152 2021-03-03 19:46:21.000000 depedit-3.3.1.0/depedit/depedit - Copy.py
--rw-rw-rw-   0        0        0    68014 2024-01-14 22:26:13.000000 depedit-3.3.1.0/depedit/depedit.py
-drwxrwxrwx   0        0        0        0 2024-01-14 22:29:14.153333 depedit-3.3.1.0/depedit.egg-info/
--rw-rw-rw-   0        0        0      728 2024-01-14 22:29:14.000000 depedit-3.3.1.0/depedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2024-01-14 22:29:14.000000 depedit-3.3.1.0/depedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-14 22:29:14.000000 depedit-3.3.1.0/depedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-01-14 22:29:14.000000 depedit-3.3.1.0/depedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-14 22:29:14.000000 depedit-3.3.1.0/depedit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-14 22:29:14.172462 depedit-3.3.1.0/setup.cfg
--rw-rw-rw-   0        0        0      816 2024-01-14 22:25:39.000000 depedit-3.3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:23:17.174068 depedit-3.4.0.0/
+-rw-rw-rw-   0        0        0    11560 2015-10-19 14:53:17.000000 depedit-3.4.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      728 2024-05-01 21:23:17.173093 depedit-3.4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3047 2022-08-20 14:24:59.000000 depedit-3.4.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 21:23:17.156068 depedit-3.4.0.0/depedit/
+-rw-rw-rw-   0        0        0       48 2019-01-05 19:27:46.000000 depedit-3.4.0.0/depedit/__init__.py
+-rw-rw-rw-   0        0        0       93 2021-04-30 14:53:22.000000 depedit-3.4.0.0/depedit/__main__.py
+-rw-rw-rw-   0        0        0    42152 2021-03-03 19:46:21.000000 depedit-3.4.0.0/depedit/depedit - Copy.py
+-rw-rw-rw-   0        0        0    69748 2024-05-01 21:20:01.000000 depedit-3.4.0.0/depedit/depedit.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:23:17.171069 depedit-3.4.0.0/depedit.egg-info/
+-rw-rw-rw-   0        0        0      728 2024-05-01 21:23:16.000000 depedit-3.4.0.0/depedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-05-01 21:23:17.000000 depedit-3.4.0.0/depedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 21:23:16.000000 depedit-3.4.0.0/depedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-01 21:23:16.000000 depedit-3.4.0.0/depedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-01 21:23:16.000000 depedit-3.4.0.0/depedit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 21:23:17.175069 depedit-3.4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      816 2024-05-01 21:19:38.000000 depedit-3.4.0.0/setup.py
```

### Comparing `depedit-3.3.1.0/LICENSE.txt` & `depedit-3.4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `depedit-3.3.1.0/PKG-INFO` & `depedit-3.4.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: depedit
-Version: 3.3.1.0
+Version: 3.4.0.0
 Summary: A simple configurable tool for manipulating dependency trees
 Home-page: https://github.com/amir-zeldes/depedit
-Download-URL: https://github.com/amir-zeldes/depedit/releases/tag/3.3.1.0
+Download-URL: https://github.com/amir-zeldes/depedit/releases/tag/3.4.0.0
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
 Keywords: NLP,parsing,syntax,dependencies,dependency,tree,treebank,conll,conllu,ud,enhanced
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `depedit-3.3.1.0/README.md` & `depedit-3.4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `depedit-3.3.1.0/depedit/depedit - Copy.py` & `depedit-3.4.0.0/depedit/depedit - Copy.py`

 * *Files identical despite different names*

### Comparing `depedit-3.3.1.0/depedit/depedit.py` & `depedit-3.4.0.0/depedit/depedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from decimal import Decimal
 from collections import defaultdict
 from copy import copy, deepcopy
 from glob import glob
 import io
 from six import iteritems, iterkeys
 
-__version__ = "3.3.1.0"
+__version__ = "3.4.0.0"
 
 ALIASES = {"form":"text","upostag":"pos","xpostag":"cpos","feats":"morph","deprel":"func","deps":"head2","misc":"func2",
            "xpos": "cpos","upos":"pos"}
 
 
 def escape(string, symbol_to_mask, border_marker):
     inside = False
@@ -168,14 +168,15 @@
 
     @staticmethod
     def handle_aliases(orig_action):
         for source, target in iteritems(ALIASES):
             orig_action = orig_action.replace(":" + source + "=", ":" + target + "=")
             orig_action = orig_action.replace(":" + source + "+=", ":" + target + "+=")
             orig_action = orig_action.replace(":" + source + "-=", ":" + target + "-=")
+            orig_action = orig_action.replace(":" + source + ",=", ":" + target + ",=")
         return orig_action
 
     @staticmethod
     def normalize_shorthand(criterion_string):
         criterion_string = criterion_string.replace('.*', '.1,1000')
         temp = ""
         while temp != criterion_string:
@@ -199,14 +200,15 @@
 
     def validate(self):
         report = ""
         for definition in self.definitions:
             node = escape(definition.def_text, "&", "/")
             criteria = (_crit.replace("%%%%%", "&") for _crit in node.split("&"))
             for criterion in criteria:
+                criterion = escape(criterion, "=", "/")
                 if re.match(r"(text|pos|cpos|lemma|morph|storage[23]?|edom|func|head|func2|head2|num|form|upos|upostag|xpos|xpostag|feats|deprel|deps|misc|edep|ehead)!?=/[^/=]*/", criterion) is None:
                     if re.match(r"position!?=/(first|last|mid)/", criterion) is None:
                         if re.match(r"#S:[A-Za-z_]+!?=/[^/\t]+/",criterion) is None:
                             report += "Invalid node definition in column 1: " + criterion
         for relation in self.relations:
             if relation == "none" and len(self.relations) == 1:
                 if len(self.definitions) > 1:
@@ -220,15 +222,15 @@
                     if not re.match(r"(#[0-9]+(([>~]|\.([0-9]+(,[0-9]+)?)?)#[0-9]+)+|#[0-9]+:(text|pos|cpos|lemma|morph|storage[23]?|edom|"
                                     r"func|head|func2|head2|num|form|upos|upostag|xpos|xpostag|feats|deprel|deps|misc|edep|ehead)==#[0-9]+)",
                                     criterion):
                         report += "Column 2 relation setting invalid criterion: " + criterion + "."
         for action in self.actions:
             commands = action.split(";")
             for command in commands:  # Node action
-                if re.match(r"(#[0-9]+([>~]|><)#[0-9]+|#[0-9]+:(func|lemma|text|pos|cpos|morph|storage[23]?|edom|head|head2|func2|num|form|upos|upostag|xpos|xpostag|feats|deprel|deps|misc|edep|ehead|split)[\+-]?=[^;]*)$", command) is None:
+                if re.match(r"(#[0-9]+([>~]|><)#[0-9]+|#[0-9]+:(func|lemma|text|pos|cpos|morph|storage[23]?|edom|head|head2|func2|num|form|upos|upostag|xpos|xpostag|feats|deprel|deps|misc|edep|ehead|split)[\+,-]?=[^;]*)$", command) is None:
                     if re.match(r"#S:[A-Za-z_]+=[A-Za-z_]+$|last$|once$", command) is None:  # Sentence annotation action or quit
                         report += "Column 3 invalid action definition: " + command + " and the action was " + action
                         if "#" not in action:
                             report += " (no node declaration with #)"
                 if "split=" in action and "|" not in action:
                     report += "Split action specified but no split points marked with | in command: " + command + " in action " + action
 
@@ -916,20 +918,24 @@
                                         sys.stdout.write("! Warning: Rule is applying a *token* transformation to a *sentence* annotation node:\n")
                                         sys.stdout.write("  " + transformation.transformation_text + "\n")
                                         sys.stdout.write("  Applying the transformation to first token in sentence.\n")
                             prop = action[action.find(":") + 1:action.find("=")]
                             value = action[action.find("=") + 1:].strip()
                             add_val = False
                             subtract_val = False
+                            concat_val = False
                             if prop.endswith("+"):  # Add annotation, e.g. feats+=...
                                 add_val = True
                                 prop = prop[:-1]
                             elif prop.endswith("-"):  # Remove annotation, e.g. feats-=...
                                 subtract_val = True
                                 prop = prop[:-1]
+                            elif prop.endswith(","):  # Add to existing values, separated by , and alphabetized, e.g. Cxn=X,Y,Z
+                                concat_val = True
+                                prop = prop[:-1]
                             group_num_matches = re.findall(r"(\$[0-9]+[LU]?)", value)
                             if group_num_matches is not None:
                                 for g in group_num_matches:
                                     no_dollar = g[1:]
                                     case = ""
                                     if no_dollar[-1] == "U":
                                         case = "upper"
@@ -977,14 +983,33 @@
                                         if not ov.split("=")[0] in new_vals_keys:  # Else this needs to be overwritten
                                             kv.append(ov)
                                     value = "|".join(sorted(kv,key=lambda x:x.lower()))
                                     if value == "":
                                         value = "_"
                                 else:
                                     value = "_"
+                            elif concat_val:
+                                old_val = getattr(result[node_position],prop)
+                                new_vals = sorted(value.split("|"))
+                                new_vals_keys = defaultdict(set)
+                                for pair in new_vals:
+                                    this_key, this_val = pair.split("=")
+                                    new_vals_keys[this_key].add(this_val)
+                                if old_val != "_" and isinstance(old_val,str):  # Some values already exist
+                                    kv = []
+                                    for ov in sorted(old_val.split("|")):
+                                        this_key, this_val = ov.split("=")
+                                        if this_key not in new_vals_keys:  # Else this needs to be overwritten
+                                            kv.append(ov)
+                                        else:
+                                            kv.append(this_key + "=" + ",".join(sorted(list(new_vals_keys[this_key].union(set(this_val.split(",")))))))
+                                    value = "|".join(sorted(kv,key=lambda x:x.lower()))
+                                else:
+                                    value = "|".join(new_vals)
+
                             if prop == "edep":
                                 if value == "":  # Set empty edep
                                     result[node_position].edep = []
                                 elif len(result[node_position].edep) == 0:
                                     result[node_position].edep.append([None,value])
                                     sys.stderr.write("WARN: added an enhanced label before adding its edge in transformation:\n" +
                                                      str(transformation) + "\n")
```

### Comparing `depedit-3.3.1.0/depedit.egg-info/PKG-INFO` & `depedit-3.4.0.0/depedit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: depedit
-Version: 3.3.1.0
+Version: 3.4.0.0
 Summary: A simple configurable tool for manipulating dependency trees
 Home-page: https://github.com/amir-zeldes/depedit
-Download-URL: https://github.com/amir-zeldes/depedit/releases/tag/3.3.1.0
+Download-URL: https://github.com/amir-zeldes/depedit/releases/tag/3.4.0.0
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
 Keywords: NLP,parsing,syntax,dependencies,dependency,tree,treebank,conll,conllu,ud,enhanced
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `depedit-3.3.1.0/setup.py` & `depedit-3.4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 
 setup(
   name = 'depedit',
   packages = ['depedit'],
-  version = '3.3.1.0',
+  version = '3.4.0.0',
   description = 'A simple configurable tool for manipulating dependency trees',
   author = 'Amir Zeldes',
   author_email = 'amir.zeldes@georgetown.edu',
   url = 'https://github.com/amir-zeldes/depedit',
   install_requires=["six"],
   license='Apache License, Version 2.0',
-  download_url = 'https://github.com/amir-zeldes/depedit/releases/tag/3.3.1.0',
+  download_url = 'https://github.com/amir-zeldes/depedit/releases/tag/3.4.0.0',
   keywords = ['NLP', 'parsing', 'syntax', 'dependencies', 'dependency', 'tree', 'treebank', 'conll', 'conllu', 'ud', 'enhanced'],
   classifiers = ['Programming Language :: Python',
 'Programming Language :: Python :: 2',
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: Apache Software License',
 'Operating System :: OS Independent'],
 )
```

