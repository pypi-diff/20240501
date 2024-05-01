# Comparing `tmp/nextstrain-sphinx-theme-2023.2.tar.gz` & `tmp/nextstrain_sphinx_theme-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextstrain-sphinx-theme-2023.2.tar", last modified: Tue Jul 25 23:38:49 2023, max compression
+gzip compressed data, was "nextstrain_sphinx_theme-2024.1.tar", last modified: Wed May  1 18:24:18 2024, max compression
```

## Comparing `nextstrain-sphinx-theme-2023.2.tar` & `nextstrain_sphinx_theme-2024.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.541207 nextstrain-sphinx-theme-2023.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-25 23:38:49.541207 nextstrain-sphinx-theme-2023.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.533207 nextstrain-sphinx-theme-2023.2/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.533207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.533207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.537207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.537207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.537207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/css/nextstrain.css
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.537207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/js/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.541207 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)    39937 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   111024 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)    44598 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    29403 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)   190685 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    32452 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:38:49.541207 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 23:38:49.000000 nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:38:49.541207 nextstrain-sphinx-theme-2023.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-25 23:38:31.000000 nextstrain-sphinx-theme-2023.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.278881 nextstrain_sphinx_theme-2024.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-01 18:24:18.278881 nextstrain_sphinx_theme-2024.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.270881 nextstrain_sphinx_theme-2024.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.270881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.270881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.270881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.270881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.274881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/css/nextstrain.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.274881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/js/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.274881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39937 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111024 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    23997 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44598 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    29403 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)   190685 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14190 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32452 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.278881 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:24:18.278881 nextstrain_sphinx_theme-2024.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/setup.py
```

### Comparing `nextstrain-sphinx-theme-2023.2/LICENSE` & `nextstrain_sphinx_theme-2024.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/PKG-INFO` & `nextstrain_sphinx_theme-2024.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-sphinx-theme
-Version: 2023.2
+Version: 2024.1
 Summary: Nextstrain theme for Sphinx and Read The Docs
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,14 +12,17 @@
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 License-File: LICENSE
+Requires-Dist: sphinx_rtd_theme>=1.0.0
+Requires-Dist: sphinx-better-subsection
+Requires-Dist: sphinx-copybutton
 
 Nextstrain Sphinx Theme
 =======================
 
 A `Sphinx theme`_ for Nextstrain's documentation, based on `Read The Docs`_'
 default theme (sphinx_rtd_theme_).
```

### Comparing `nextstrain-sphinx-theme-2023.2/README.rst` & `nextstrain_sphinx_theme-2024.1/README.rst`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/__init__.py` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/breadcrumbs.html` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/footer.html` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/footer.html`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         {{ name |e }}
       {% if link %}</a>{% endif %}
     </span>
     {% endmacro %}
     {{ TeamMember(name="Trevor Bedford", image="trevor-bedford.jpg", link="http://bedford.io/team/trevor-bedford/") }},
     {{ TeamMember(name="Richard Neher", image="richard-neher.jpg", link="https://neherlab.org/richard-neher.html") }},
     {{ TeamMember(name="Ivan Aksamentov", image="ivan-aksamentov.jpg", link="https://neherlab.org/ivan-aksamentov.html") }},
+    {{ TeamMember(name="John SJ Anderson", image="john-sj-anderson.jpg", link="https://bedford.io/team/john-sj-anderson/") }},
+    {{ TeamMember(name="Kim Andrews", image="kim-andrews.jpg", link="https://bedford.io/team/kim-andrews/") }},
     {{ TeamMember(name="Jennifer Chang", image="jennifer-chang.jpg", link="https://bedford.io/team/jennifer-chang/") }},
     {{ TeamMember(name="James Hadfield", image="james-hadfield.jpg", link="http://bedford.io/team/james-hadfield/") }},
     {{ TeamMember(name="Emma Hodcroft", image="emma-hodcroft.jpg", link="http://emmahodcroft.com/") }},
     {{ TeamMember(name="John Huddleston", image="john-huddleston.jpg", link="http://bedford.io/team/john-huddleston/") }},
     {{ TeamMember(name="Jover Lee", image="jover-lee.jpg", link="http://bedford.io/team/jover-lee/") }},
     {{ TeamMember(name="Victor Lin", image="victor-lin.png", link="https://bedford.io/team/victor-lin/") }},
     {{ TeamMember(name="Cornelius Roemer", image="cornelius-roemer.jpg", link="https://neherlab.org/cornelius-roemer.html") }},
```

#### html2text {}

```diff
@@ -15,27 +15,30 @@
 {% macro TeamMember(name, image, link) %} {% if link %}_{_%_ _e_n_d_i_f_ _%_}_ _[_h_t_t_p_s_:_/_/
 _r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_n_e_x_t_s_t_r_a_i_n_/_n_e_x_t_s_t_r_a_i_n_._o_r_g_/_H_E_A_D_/_s_t_a_t_i_c_-_s_i_t_e_/_s_t_a_t_i_c_/
 _t_e_a_m_/_{_{_ _i_m_a_g_e_ _}_}_]_{_{_ _n_a_m_e_ _|_e_ _}_}_ _{_%_ _i_f_ _l_i_n_k_ _%_}{% endif %} {% endmacro %} {
 { TeamMember(name="Trevor Bedford", image="trevor-bedford.jpg", link="http://
 bedford.io/team/trevor-bedford/") }}, {{ TeamMember(name="Richard Neher",
 image="richard-neher.jpg", link="https://neherlab.org/richard-neher.html") }},
 {{ TeamMember(name="Ivan Aksamentov", image="ivan-aksamentov.jpg", link="https:
-//neherlab.org/ivan-aksamentov.html") }}, {{ TeamMember(name="Jennifer Chang",
-image="jennifer-chang.jpg", link="https://bedford.io/team/jennifer-chang/") }},
-{{ TeamMember(name="James Hadfield", image="james-hadfield.jpg", link="http://
-bedford.io/team/james-hadfield/") }}, {{ TeamMember(name="Emma Hodcroft",
-image="emma-hodcroft.jpg", link="http://emmahodcroft.com/") }}, {{ TeamMember
-(name="John Huddleston", image="john-huddleston.jpg", link="http://bedford.io/
-team/john-huddleston/") }}, {{ TeamMember(name="Jover Lee", image="jover-
-lee.jpg", link="http://bedford.io/team/jover-lee/") }}, {{ TeamMember
-(name="Victor Lin", image="victor-lin.png", link="https://bedford.io/team/
-victor-lin/") }}, {{ TeamMember(name="Cornelius Roemer", image="cornelius-
-roemer.jpg", link="https://neherlab.org/cornelius-roemer.html") }}, {
-{ TeamMember(name="Thomas Sibley", image="thomas-sibley.jpg", link="https://
-bedford.io/team/thomas-sibley/") }}
+//neherlab.org/ivan-aksamentov.html") }}, {{ TeamMember(name="John SJ
+Anderson", image="john-sj-anderson.jpg", link="https://bedford.io/team/john-sj-
+anderson/") }}, {{ TeamMember(name="Kim Andrews", image="kim-andrews.jpg",
+link="https://bedford.io/team/kim-andrews/") }}, {{ TeamMember(name="Jennifer
+Chang", image="jennifer-chang.jpg", link="https://bedford.io/team/jennifer-
+chang/") }}, {{ TeamMember(name="James Hadfield", image="james-hadfield.jpg",
+link="http://bedford.io/team/james-hadfield/") }}, {{ TeamMember(name="Emma
+Hodcroft", image="emma-hodcroft.jpg", link="http://emmahodcroft.com/") }}, {
+{ TeamMember(name="John Huddleston", image="john-huddleston.jpg", link="http://
+bedford.io/team/john-huddleston/") }}, {{ TeamMember(name="Jover Lee",
+image="jover-lee.jpg", link="http://bedford.io/team/jover-lee/") }}, {
+{ TeamMember(name="Victor Lin", image="victor-lin.png", link="https://
+bedford.io/team/victor-lin/") }}, {{ TeamMember(name="Cornelius Roemer",
+image="cornelius-roemer.jpg", link="https://neherlab.org/cornelius-
+roemer.html") }}, {{ TeamMember(name="Thomas Sibley", image="thomas-
+sibley.jpg", link="https://bedford.io/team/thomas-sibley/") }}
 Please see the _t_e_a_m_ _p_a_g_e for more details.
 
 All _s_o_u_r_c_e_ _c_o_d_e_ _f_o_r_ _N_e_x_t_s_t_r_a_i_n is freely available under the terms of an _o_p_e_n_-
 _s_o_u_r_c_e_ _l_i_c_e_n_s_e, typically _A_G_P_L_-_3_._0 or _M_I_T. Refer to specific projects for
 details. Screenshots may be used under a _C_C_-_B_Y_-_4_._0_ _l_i_c_e_n_s_e and attribution to
 nextstrain.org must be provided.
 This work is made possible by the open sharing of genetic data by research
```

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/layout.html` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/layout.html`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/css/nextstrain.css` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/css/nextstrain.css`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/favicon.ico` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/js/theme.js` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo-small.png` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo-small.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo.png` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/icon.png` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/icon.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-sphinx-theme
-Version: 2023.2
+Version: 2024.1
 Summary: Nextstrain theme for Sphinx and Read The Docs
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,14 +12,17 @@
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 License-File: LICENSE
+Requires-Dist: sphinx_rtd_theme>=1.0.0
+Requires-Dist: sphinx-better-subsection
+Requires-Dist: sphinx-copybutton
 
 Nextstrain Sphinx Theme
 =======================
 
 A `Sphinx theme`_ for Nextstrain's documentation, based on `Read The Docs`_'
 default theme (sphinx_rtd_theme_).
```

### Comparing `nextstrain-sphinx-theme-2023.2/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt` & `nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextstrain-sphinx-theme-2023.2/setup.py` & `nextstrain_sphinx_theme-2024.1/setup.py`

 * *Files identical despite different names*

