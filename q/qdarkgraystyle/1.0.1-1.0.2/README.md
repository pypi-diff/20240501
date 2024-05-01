# Comparing `tmp/qdarkgraystyle-1.0.1.tar.gz` & `tmp/qdarkgraystyle-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qdarkgraystyle-1.0.1.tar", last modified: Mon Apr 30 03:38:42 2018, max compression
+gzip compressed data, was "dist/qdarkgraystyle-1.0.2.tar", last modified: Wed May  2 11:26:53 2018, max compression
```

## Comparing `qdarkgraystyle-1.0.1.tar` & `qdarkgraystyle-1.0.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2676 2018-04-30 03:37:59.000000 qdarkgraystyle-1.0.1/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2526 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1137 2018-04-30 03:37:59.000000 qdarkgraystyle-1.0.1/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/qdarkgraystyle.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/qdarkgraystyle.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/qdarkgraystyle.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4268 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/qdarkgraystyle.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/qdarkgraystyle.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2002 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/qdarkgraystyle.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/tests/test_example_pyqt5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      258 2018-04-30 03:37:59.000000 qdarkgraystyle-1.0.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4268 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/style.qrc
--rw-rw-r--   0 travis    (2000) travis    (2000)     1788 2018-04-30 03:37:59.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/compile_qrc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2428 2018-04-30 03:37:59.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    94915 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/pyqt5_style_rc.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-04-30 03:38:42.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      972 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_checked_disabled.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/right_arrow.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/left_arrow_disabled.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      598 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/close-pressed.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      187 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/Vsepartoolbar.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/right_arrow_disabled.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/down_arrow.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/checkbox_checked.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      940 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_checked.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      575 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_unchecked_focus.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      182 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/stylesheet-branch-more.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      158 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/up_arrow.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/down_arrow_disabled.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      728 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_unchecked.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      172 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/Hsepartoolbar.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      578 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/undock.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/Vmovetoolbar.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/branch_open.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      464 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/checkbox_unchecked.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      464 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/checkbox_unchecked_disabled.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      150 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/branch_open-on.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      195 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/transparent.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      491 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/checkbox_checked_disabled.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/branch_closed.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      714 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_checked_focus.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/checkbox_indeterminate_disabled.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      239 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/stylesheet-vline.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      220 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/Hmovetoolbar.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      129 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/sizegrip.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      598 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/close-hover.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/left_arrow.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      493 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/checkbox_indeterminate.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      404 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/checkbox_unchecked_focus.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      420 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/checkbox_checked_focus.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      224 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/stylesheet-branch-end.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      586 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/close.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      147 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/branch_closed-on.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/up_arrow_disabled.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      760 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_unchecked_disabled.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      420 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/rc/checkbox_indeterminate_focus.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    26461 2018-04-30 03:38:00.000000 qdarkgraystyle-1.0.1/qdarkgraystyle/style.qss
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2950 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2548 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1137 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/qdarkgraystyle.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/qdarkgraystyle.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/qdarkgraystyle.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4614 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/qdarkgraystyle.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/qdarkgraystyle.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2002 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/qdarkgraystyle.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/tests/test_example_pyqt5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      258 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4614 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/style.qrc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1788 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/compile_qrc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2591 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    94915 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/pyqt5_style_rc.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-05-02 11:26:53.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      972 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_checked_disabled.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      160 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/right_arrow.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/left_arrow_disabled.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      598 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/close-pressed.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      187 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/Vsepartoolbar.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      160 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/right_arrow_disabled.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/down_arrow.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      492 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/checkbox_checked.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      940 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_checked.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      575 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_unchecked_focus.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      182 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/stylesheet-branch-more.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      158 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/up_arrow.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/down_arrow_disabled.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      728 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_unchecked.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      172 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/Hsepartoolbar.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      578 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/undock.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      228 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/Vmovetoolbar.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/branch_open.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      464 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/checkbox_unchecked.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      464 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/checkbox_unchecked_disabled.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      150 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/branch_open-on.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      195 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/transparent.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      491 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/checkbox_checked_disabled.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      160 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/branch_closed.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_checked_focus.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      492 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/checkbox_indeterminate_disabled.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      239 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/stylesheet-vline.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      220 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/Hmovetoolbar.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      129 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/sizegrip.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      598 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/close-hover.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/left_arrow.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      493 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/checkbox_indeterminate.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      404 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/checkbox_unchecked_focus.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      420 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/checkbox_checked_focus.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      224 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/stylesheet-branch-end.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      586 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/close.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      147 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/branch_closed-on.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      159 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/up_arrow_disabled.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      760 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_unchecked_disabled.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      420 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/rc/checkbox_indeterminate_focus.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26461 2018-05-02 11:26:08.000000 qdarkgraystyle-1.0.2/qdarkgraystyle/style.qss
```

### Comparing `qdarkgraystyle-1.0.1/README.rst` & `qdarkgraystyle-1.0.2/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,22 @@
 
 or
 
 .. code:: bash
 
     pip install qdarkgraystyle
 
+The *PySide* and *PyQt4* support was dropped in version *1.0.0*. To use `qdarkgraystyle` with *PySide* or *PyQt4* or with *Python 2.7*, please use the version *0.0.3*.
+
+.. code:: bash
+
+    pip install qdarkgraystyle==0.0.3
+
+The support to *PySide2* will be add in future.
+
 Usage
 ============
 
 Here is an example using PyQt5.
 
 .. code:: python
 
@@ -58,14 +66,15 @@
 .. code:: bash
 
     python example/example_pyqt5.py
 
 You can run the script without installing `qdarkgraystyle`. You only need to have
 PyQt5 installed on your system.
 
+
 Contribute
 ==========
 
 - Issue Tracker: https://github.com/mstuttgart/qdarkgraystyle/issues
 - Source Code: https://github.com/mstuttgart/qdarkgraystyle
 
 Snapshots
```

### Comparing `qdarkgraystyle-1.0.1/setup.py` & `qdarkgraystyle-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     author='Michell Stuttgart',
     author_email='michellstut@gmail.com',
     description='A dark gray stylesheet for PyQt/PySide applications',
     long_description=readme,
 
     install_requires=[
         'PyQt5>=5.6',
+        'deprecated',
     ],
     classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Environment :: X11 Applications :: Qt',
           'Environment :: Win32 (MS Windows)',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
```

### Comparing `qdarkgraystyle-1.0.1/LICENSE` & `qdarkgraystyle-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle.egg-info/PKG-INFO` & `qdarkgraystyle-1.0.2/qdarkgraystyle.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: qdarkgraystyle
-Version: 1.0.1
+Version: 1.0.2
 Summary: A dark gray stylesheet for PyQt/PySide applications
 Home-page: https://github.com/mstuttgart/qdarkgraystyle
 Author: Michell Stuttgart
 Author-email: michellstut@gmail.com
 License: MIT License
 Description: QDarkGray Stylesheet
         ====================
@@ -34,14 +34,22 @@
         
         or
         
         .. code:: bash
         
             pip install qdarkgraystyle
         
+        The *PySide* and *PyQt4* support was dropped in version *1.0.0*. To use `qdarkgraystyle` with *PySide* or *PyQt4* or with *Python 2.7*, please use the version *0.0.3*.
+        
+        .. code:: bash
+        
+            pip install qdarkgraystyle==0.0.3
+        
+        The support to *PySide2* will be add in future.
+        
         Usage
         ============
         
         Here is an example using PyQt5.
         
         .. code:: python
         
@@ -66,14 +74,15 @@
         .. code:: bash
         
             python example/example_pyqt5.py
         
         You can run the script without installing `qdarkgraystyle`. You only need to have
         PyQt5 installed on your system.
         
+        
         Contribute
         ==========
         
         - Issue Tracker: https://github.com/mstuttgart/qdarkgraystyle/issues
         - Source Code: https://github.com/mstuttgart/qdarkgraystyle
         
         Snapshots
```

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle.egg-info/SOURCES.txt` & `qdarkgraystyle-1.0.2/qdarkgraystyle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/tests/test_example_pyqt5.py` & `qdarkgraystyle-1.0.2/tests/test_example_pyqt5.py`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/PKG-INFO` & `qdarkgraystyle-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: qdarkgraystyle
-Version: 1.0.1
+Version: 1.0.2
 Summary: A dark gray stylesheet for PyQt/PySide applications
 Home-page: https://github.com/mstuttgart/qdarkgraystyle
 Author: Michell Stuttgart
 Author-email: michellstut@gmail.com
 License: MIT License
 Description: QDarkGray Stylesheet
         ====================
@@ -34,14 +34,22 @@
         
         or
         
         .. code:: bash
         
             pip install qdarkgraystyle
         
+        The *PySide* and *PyQt4* support was dropped in version *1.0.0*. To use `qdarkgraystyle` with *PySide* or *PyQt4* or with *Python 2.7*, please use the version *0.0.3*.
+        
+        .. code:: bash
+        
+            pip install qdarkgraystyle==0.0.3
+        
+        The support to *PySide2* will be add in future.
+        
         Usage
         ============
         
         Here is an example using PyQt5.
         
         .. code:: python
         
@@ -66,14 +74,15 @@
         .. code:: bash
         
             python example/example_pyqt5.py
         
         You can run the script without installing `qdarkgraystyle`. You only need to have
         PyQt5 installed on your system.
         
+        
         Contribute
         ==========
         
         - Issue Tracker: https://github.com/mstuttgart/qdarkgraystyle/issues
         - Source Code: https://github.com/mstuttgart/qdarkgraystyle
         
         Snapshots
```

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/style.qrc` & `qdarkgraystyle-1.0.2/qdarkgraystyle/style.qrc`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/compile_qrc.py` & `qdarkgraystyle-1.0.2/qdarkgraystyle/compile_qrc.py`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/__init__.py` & `qdarkgraystyle-1.0.2/qdarkgraystyle/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,21 +27,22 @@
 Initialise the QDarkGrayStyleSheet module when used with python.
 
 This modules provides a function to transparently load the stylesheets
 with the correct rc file.
 """
 import logging
 import platform
+from deprecated import deprecated
 
 from PyQt5 import QtCore
 
 from qdarkgraystyle import compile_qrc, pyqt5_style_rc
 
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 
 def _logger():
     return logging.getLogger('qdarkgraystyle')
 
 
 def load_stylesheet():
@@ -67,7 +68,11 @@
                 background-color: #31363b;
                 text-align: center;
                 height: 12px;
             }
             '''
             stylesheet += mac_fix
         return stylesheet
+
+@deprecated(version='1.0.0', reason="You should use load_stylesheet")
+def load_stylesheet_pyqt5():
+    return load_stylesheet()
```

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/pyqt5_style_rc.py` & `qdarkgraystyle-1.0.2/qdarkgraystyle/pyqt5_style_rc.py`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_checked_disabled.png` & `qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_checked_disabled.png`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/rc/close-pressed.png` & `qdarkgraystyle-1.0.2/qdarkgraystyle/rc/close-pressed.png`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_checked.png` & `qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_checked.png`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_unchecked_focus.png` & `qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_unchecked_focus.png`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_unchecked.png` & `qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_unchecked.png`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/rc/undock.png` & `qdarkgraystyle-1.0.2/qdarkgraystyle/rc/undock.png`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_checked_focus.png` & `qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_checked_focus.png`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/rc/close-hover.png` & `qdarkgraystyle-1.0.2/qdarkgraystyle/rc/close-hover.png`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/rc/close.png` & `qdarkgraystyle-1.0.2/qdarkgraystyle/rc/close.png`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/rc/radio_unchecked_disabled.png` & `qdarkgraystyle-1.0.2/qdarkgraystyle/rc/radio_unchecked_disabled.png`

 * *Files identical despite different names*

### Comparing `qdarkgraystyle-1.0.1/qdarkgraystyle/style.qss` & `qdarkgraystyle-1.0.2/qdarkgraystyle/style.qss`

 * *Files identical despite different names*

