# Comparing `tmp/getbc-0.1.0.tar.gz` & `tmp/getbc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getbc-0.1.0.tar", last modified: Tue Apr  2 00:56:44 2024, max compression
+gzip compressed data, was "getbc-0.4.0.tar", last modified: Wed May  1 02:44:19 2024, max compression
```

## Comparing `getbc-0.1.0.tar` & `getbc-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-04-02 00:56:43.991698 getbc-0.1.0/
--rwxrwx---   0 root         (0) vboxsf     (999)    35149 2022-03-01 01:25:59.000000 getbc-0.1.0/LICENSE.txt
--rwxrwx---   0 root         (0) vboxsf     (999)     1553 2024-04-02 00:56:43.987797 getbc-0.1.0/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)      933 2024-04-01 01:08:01.000000 getbc-0.1.0/README.md
--rwxrwx---   0 root         (0) vboxsf     (999)       38 2024-04-02 00:56:43.991698 getbc-0.1.0/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (999)     1038 2024-04-02 00:51:18.000000 getbc-0.1.0/setup.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-04-02 00:56:43.944848 getbc-0.1.0/src/
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-04-02 00:56:43.983883 getbc-0.1.0/src/getbc.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (999)     1553 2024-04-02 00:56:43.000000 getbc-0.1.0/src/getbc.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)      211 2024-04-02 00:56:43.000000 getbc-0.1.0/src/getbc.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        1 2024-04-02 00:56:43.000000 getbc-0.1.0/src/getbc.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       37 2024-04-02 00:56:43.000000 getbc-0.1.0/src/getbc.egg-info/entry_points.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        6 2024-04-02 00:56:43.000000 getbc-0.1.0/src/getbc.egg-info/top_level.txt
--rwxrwx---   0 root         (0) vboxsf     (999)    15332 2024-04-02 00:53:37.000000 getbc-0.1.0/src/getbc.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-05-01 02:44:18.887367 getbc-0.4.0/
+-rwxrwx---   0 root         (0) vboxsf     (999)    35149 2022-03-01 01:25:59.000000 getbc-0.4.0/LICENSE.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)     1548 2024-05-01 02:44:18.884443 getbc-0.4.0/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)      928 2024-04-02 01:01:53.000000 getbc-0.4.0/README.md
+-rwxrwx---   0 root         (0) vboxsf     (999)       38 2024-05-01 02:44:18.888314 getbc-0.4.0/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (999)     1038 2024-04-18 04:13:14.000000 getbc-0.4.0/setup.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-05-01 02:44:18.834607 getbc-0.4.0/src/
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2024-05-01 02:44:18.879530 getbc-0.4.0/src/getbc.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (999)     1548 2024-05-01 02:44:18.000000 getbc-0.4.0/src/getbc.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)      211 2024-05-01 02:44:18.000000 getbc-0.4.0/src/getbc.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        1 2024-05-01 02:44:18.000000 getbc-0.4.0/src/getbc.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       37 2024-05-01 02:44:18.000000 getbc-0.4.0/src/getbc.egg-info/entry_points.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        6 2024-05-01 02:44:18.000000 getbc-0.4.0/src/getbc.egg-info/top_level.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)    16824 2024-04-30 23:21:24.000000 getbc-0.4.0/src/getbc.py
```

### Comparing `getbc-0.1.0/LICENSE.txt` & `getbc-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getbc-0.1.0/PKG-INFO` & `getbc-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getbc
-Version: 0.1.0
+Version: 0.4.0
 Summary: Make installing bomcheckgui easy
 Home-page: https://github.com/kcarlton55/getbc
 Author: Kenneth Edward Carlton
 Author-email: kencarlton55@gmail.com
 License: GPLv3+
 Keywords: bomcheckgui
 Classifier: Programming Language :: Python :: 3
@@ -13,31 +13,31 @@
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# **get-bc**
+# **getbc**
 
 
 ## **What the program does**
 This program's primary responsibilty is to make installing bomcheckgui
 to a person's local computer easy.  It creates a virtual environment
 for bomcheckgui and installs bomcheckgui and its dependencies there,
-and creates a desktop link to bomcheckgui.  It can also check for 
-program upgrades and can uninstall bomcheckgui.  Note: this program 
+and creates a desktop link to bomcheckgui.  It can also check for
+program upgrades and can uninstall bomcheckgui.  Note: this program
 only works on Microsoft Windows, and only works with a standard python
 installation as compared to a variation of python like the Anaconda
 python distribution.
 
 ## **How to install**
 Assuming that you already have Python on your machine, use the package
 manager software [pip](https://en.wikipedia.org/wiki/Pip_(package_manager))
 that comes with Python and run this from a command line:
 
-`pip install get-bc`
+`pip install getbc`
 
-Once installed, run get-bc from a cmd module.  When you run it, it will
+Once installed, run getbc from a cmd module.  When you run it, it will
 give instruction on how to proceed.
```

### Comparing `getbc-0.1.0/README.md` & `getbc-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# **get-bc**
+# **getbc**
 
 
 ## **What the program does**
 This program's primary responsibilty is to make installing bomcheckgui
 to a person's local computer easy.  It creates a virtual environment
 for bomcheckgui and installs bomcheckgui and its dependencies there,
-and creates a desktop link to bomcheckgui.  It can also check for 
-program upgrades and can uninstall bomcheckgui.  Note: this program 
+and creates a desktop link to bomcheckgui.  It can also check for
+program upgrades and can uninstall bomcheckgui.  Note: this program
 only works on Microsoft Windows, and only works with a standard python
 installation as compared to a variation of python like the Anaconda
 python distribution.
 
 ## **How to install**
 Assuming that you already have Python on your machine, use the package
 manager software [pip](https://en.wikipedia.org/wiki/Pip_(package_manager))
 that comes with Python and run this from a command line:
 
-`pip install get-bc`
+`pip install getbc`
 
-Once installed, run get-bc from a cmd module.  When you run it, it will
+Once installed, run getbc from a cmd module.  When you run it, it will
 give instruction on how to proceed.
```

### Comparing `getbc-0.1.0/setup.py` & `getbc-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='getbc',   # name people will use to pip install
     python_requires='>=3.8',
-    version='0.1.0',
+    version='0.4.0',
     description='Make installing bomcheckgui easy',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='GPLv3+',
     py_modules=['getbc'],
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `getbc-0.1.0/src/getbc.egg-info/PKG-INFO` & `getbc-0.4.0/src/getbc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getbc
-Version: 0.1.0
+Version: 0.4.0
 Summary: Make installing bomcheckgui easy
 Home-page: https://github.com/kcarlton55/getbc
 Author: Kenneth Edward Carlton
 Author-email: kencarlton55@gmail.com
 License: GPLv3+
 Keywords: bomcheckgui
 Classifier: Programming Language :: Python :: 3
@@ -13,31 +13,31 @@
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# **get-bc**
+# **getbc**
 
 
 ## **What the program does**
 This program's primary responsibilty is to make installing bomcheckgui
 to a person's local computer easy.  It creates a virtual environment
 for bomcheckgui and installs bomcheckgui and its dependencies there,
-and creates a desktop link to bomcheckgui.  It can also check for 
-program upgrades and can uninstall bomcheckgui.  Note: this program 
+and creates a desktop link to bomcheckgui.  It can also check for
+program upgrades and can uninstall bomcheckgui.  Note: this program
 only works on Microsoft Windows, and only works with a standard python
 installation as compared to a variation of python like the Anaconda
 python distribution.
 
 ## **How to install**
 Assuming that you already have Python on your machine, use the package
 manager software [pip](https://en.wikipedia.org/wiki/Pip_(package_manager))
 that comes with Python and run this from a command line:
 
-`pip install get-bc`
+`pip install getbc`
 
-Once installed, run get-bc from a cmd module.  When you run it, it will
+Once installed, run getbc from a cmd module.  When you run it, it will
 give instruction on how to proceed.
```

### Comparing `getbc-0.1.0/src/getbc.py` & `getbc-0.4.0/src/getbc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Mar  7 22:14:14 2024
-
 @author: Kenneth E. Carlton
 
+This script file is written in the computer language called python.  This
+script's primary purpose is to install the program called bomcheckgui onto your
+local computer.  Bomcheckgui compares side-by-side CAD BOMs to ERP BOMs.  For
+this program to work you must have a python interpreter prorgram loaded on your
+computer.  E.g. https://www.python.org/.
+
+To run this script, open a MS cmd prompt window in the directory where getbc.py
+resides and enter this command:
+
+    py getbc.py
 """
-__version__ = '0.1.0'
+__version__ = '0.4.0'
 __author__ = 'Kenneth E. Carlton'
 
 #import pdb # use with pdb.set_trace()
 import  argparse, webbrowser, os
 import sys
 from pathlib import Path
 import requests
@@ -20,33 +29,40 @@
 except:
     pass
 
 
 def get_version():
     return __version__
 
+try:
+    fileName = Path(__file__).stem
+except:
+    fileName = 'getbc'
+
 
 def main():
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter,
                         description=
-                        "This program's primary purpose is to install bomcheckgui, "
-                        "though it can also be used to activate bomcheckgui's virtual "
-                        "environment, view bomcheck's help files, etc.  To install "
-                        "bomcheckgui do: " + Path(__file__).stem +  " --install."
-                        ' (without the period).  Note that before any of these '
-                        'actions adds or removes any files to your computer, the '
-                        'program will explain what it is about to do, and then will '
-                        'pause and ask for your confirmation.')
+                        "This program's primary purpose is to install bomcheckgui "
+                        "to your local PC, though it can also be used to activate "
+                        "bomcheckgui's virtual environment, upgrade to the latest "
+                        "version of bomcheckgui, etc.  To install "
+                        "bomcheckgui do: py " + fileName +  ".py --install."
+                        " (without the period).  Note that before any of getbc's "
+                        'commands makes any changes to your computer, '
+                        'an explanation will be given about what it is about '
+                        'to occur, and then pause and ask for your confirmation '
+                        'before proceeding.')
+    parser.add_argument('-mh', '--morehelp', action='store_true', default=False,
+                        help="More help about using getbc"),
     parser.add_argument('-a', '--about', action='version',
                         version="Author: " + __author__ +
                         ".  Initial creation: Mar 7, 2024.  "
-                        + Path(__file__).stem + ' version: ' + __version__,
+                        + fileName + "'s version no.: " + __version__,
                         help="Show author, creation date, and version, then exit"),
-    parser.add_argument('--bomcheckhelp', action='store_true', default=False,
-                        help="Open a webpage showing bomcheck's help files"),
     parser.add_argument('-c', '--copy', action='store_true', default=False,
                         help = 'copy to clipboard: ' + str(activate)),
     parser.add_argument('--install', action='store_true', default=False,
                         help='Create a virtual environment named ' + venvname +
                         ' and install bomcheckgui and bomcheck into it; and ' +
                        'create a link to bomcheckgui on the desktop'),
     parser.add_argument('--uninstall', action='store_true', default=False,
@@ -54,52 +70,55 @@
                         'all traces of bomcheckgui, including the bc-venv folder that ' +
                         'contained these scripts.)'),
     parser.add_argument('--upgrade', action='store_true', default=False,
                         help='Show the currently installed software versions and '
                         'show the latest available software versions.  Upgrade '
                         'to newer versions if newer versions are availabe.'),
     parser.add_argument('-v', '--version', action='version', version=__version__,
-                        help="Show " + Path(__file__).stem + "'s version number and exit")
+                        help="Show " + fileName + "'s version number and exit")
 
     if len(sys.argv)==1:
         parser.print_help(sys.stderr)
         sys.exit(1)
     args = parser.parse_args()
 
     getbc(vars(args))  # vars() method returns the __dict__ attribute of args
 
 
 def getbc(dic):
     ''' central hub that calls functions '''
+    global flag
     if not sys.platform == 'win32':
-        print('Sorry.  This program currenly works only on a MS Windows OS.')
-        return
-    elif dic.get('bomcheckhelp', False):
-        bomcheckhelp()
+        flag = False
+        print("This program works only on a MS Windows' OS, and with a regular type of python\n"
+              'installation instead of, for example, a python installation like Anaconda\n\n')
+    if dic.get('morehelp', False):
+        morehelp()
     elif dic.get('copy', False):
         copy()
     elif dic.get('install', False):
         install()
     elif dic.get('uninstall', False):
         uninstall()
     elif dic.get('upgrade', False):
         upgrade()
 
 
-def bomcheckhelp():
+def morehelp():
+    print('Opening browser to show help located on the web...')
     version = 'master'
     bomcheck_help = ('https://htmlpreview.github.io/?https://github.com/'
-             'kcarlton55/bomcheck/blob/' + version + '/help_files/bomcheck_help.html')
+             'kcarlton55/getbc/blob/' + version + '/help_files/getbc_help.html')
     webbrowser.open(bomcheck_help)
 
 
 def copy():
     if not Path.exists(activate):
         print('\nA virtual environment is not yet set up.  To set one up enter:\n\n' +
-              Path(__file__).stem + ' --install')
+              fileName + ' --install')
         return
     try:
         cb.setText(str(activate), mode=cb.Clipboard)
         print('\nPaste the below to activate a virtual environment.  To deactivate, type: \n'
               'deactivate.  When activated your command prompt will look someting like: \n'
               '(bc-venv) c:\\dir1\\dir2>\n')
         print('This has been copied to the clipboard:\n ' + str(activate))
@@ -139,102 +158,112 @@
           "    installed.  Pip's function will be to download bomcheckgui from its home\n"
           '    at https://pypi.org/ and install it on your computer.\n'
           '4)  The fourth will install bomcheckgui, along with any dependencies including\n'
           '    bomcheck, into the currently active virtual environment (' + venvname + ').\n'
           '5)  Create a link to bomcheckgui on your deskop.\n'
         )
 
-    if not Path.exists(venvpathname) and not Path.exists(Path(linkto)):
+    if not Path.exists(venvpathname) and not Path.exists(Path(linkto)) and flag:
         x = input('Execute commands (takes a couple of minutes). Continue? (Y/N) ')
         if x.lower().strip()[0] == 'y':
             print('working...')
             command = (create_bc_venv + ' && ' +
                        activatevenv + ' && ' +
                        upgradepip +  ' && ' +
                        installbomcheckgui + ' && ' +
                        createdesktoplink + ' && ' +
                        'echo All 5 of 5 commands executed successfully')
             os.system(command)
             if Path.exists(Path(linkto)):
                 print('\nA link has been added to your desktop to run bomcheckgui\n')
             print('If you would like to run bomcheck or bomcheckgui from the cmd console')
-            print('do: ' + Path(__file__).stem + ' -c')
+            print('do: py ' + fileName + '.py -c')
+    elif not flag:
+        print('You are not running a MS OS.  No action will be taken')
     else:
         print('Virtual directory and/or desktop link already exists.  No action will be taken.')
 
 def uninstall():
     ''' refence:
     https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/rmdir
     '''
     delete_bc_venv= 'rmdir ' + str(venvpathname) + ' /s /q'
     delete_dektop_bomcheckgui = 'del "' + str(linkto) + '"'
+    local_app_folder = os.getenv('LOCALAPPDATA')
+    config_folder = os.path.join(local_app_folder, 'bomcheck')
+    delete_config_folder = 'rmdir ' + str(config_folder) + ' /s /q'
+
     print('\nYou are about to uninstall bomcheck, bomcheckgui, their virtual environment,\n'
           'and the bomcheckgui link from your desktop.\n\n'
 
           '1) ' + delete_dektop_bomcheckgui + '\n'
-          '2) ' + delete_bc_venv + '\n\n'
+          '2) ' + delete_bc_venv + '\n'
+          '3) ' + delete_config_folder + '\n\n'
 
           '1) Delete the desktop link to bomcheckgui.exe\n'
           '2) Delete the folder named bc-venv and all its contents.  This will delete\n'
-          "   bomcheckgui's virtual environment.\n\n"
+          "   bomcheckgui, bomcheck, and their virtual environment named bc-venv.\n"
+          '3) Delete the file named config.txt and the folder in which it resides.\n'
+          '   config.txt contains user settings genterated from bomcheckgui.\n\n'
 
           'If any of these commands does not succeed due to non-existant paths, etc., an\n'
-          'error message that you can ignore will show\n')
-
+          'error message that you can ignore will show.\n')
 
-    x = input('Execute commands (can take about a minute). Continue? (Y/N) ')
-    print()
-    if x.lower().strip()[0] == 'y':
-        print('working...')
-        os.system(delete_dektop_bomcheckgui)
-        os.system(delete_bc_venv)
+    if flag:
+        x = input('Execute commands (can take about a minute). Continue? (Y/N) ')
+        print()
+        if x.lower().strip()[0] == 'y':
+            print('working...')
+            os.system(delete_dektop_bomcheckgui)
+            os.system(delete_bc_venv)
+            os.system(delete_config_folder)
+    else:
+        print('You are not running a MS OS.  No action will be taken.')
 
 
 def upgrade():
     ''' Upgrade getbc, bomcheck, and bomcheckgui to the latest versions.
     '''
     # dictionary of commands and explanaton of those commands.
-    dic = {'getbc':  ['py -m pip install --upgrade ' + Path(__file__).stem,
-                     'Upgrade ' + Path(__file__).stem + ' to the latest version.\n'
-                     '(' + Path(__file__).stem + 'is located in the base environment.)'],
+    dic = {'getbc':  ['py -m pip install --upgrade ' + fileName,
+                     'Upgrade ' + fileName + ' to the latest version.\n'
+                     '(' + fileName + 'is located in the base environment.)'],
            'activt': [str(activate),
                      'Active the virtual environment where bomcheck and bomcheckgui \n'
                      '   are stored (i.e., at ' + str(venvpathname) + ').'],
            'bc': ['py -m pip install --upgrade bomcheck',
                   'Upgrade bomcheck to the latest version.'],
            'bcgui': ['py -m pip install --upgrade bomcheckgui',
                      'Upgrade bomcheckgui to the latest version.']}
 
     latest_getbc = latest('getbc')
     local_getbc = local('getbc')
     latest_bc = latest('bomcheck')
     local_bc = local('bomcheck')
-    latest_bcgui = local('bomcheckgui')
+    latest_bcgui = latest('bomcheckgui')
     local_bcgui = local('bomcheckgui')
 
     print()
-    print(('Latest version of ' + Path(__file__).stem + ': ' +
+    print(('Latest version of ' + fileName + ': ' +
            '.'.join([str(i) for i in latest_getbc]))    if latest_getbc else '')
-    print(('Local version of ' + Path(__file__).stem + ': ' +
+    print(('Local version of ' + fileName + ': ' +
            '.'.join([str(i) for i in local_getbc]))     if local_getbc else '')
     print(('Latest version of bomcheck: ' +
            '.'.join([str(i) for i in latest_bc]))       if latest_bc else '')
     print(('Local version of bomcheck: ' +
            '.'.join([str(i) for i in local_bc]))        if local_bc else '')
     print(('Latest version of bomcheckgui: ' +
            '.'.join([str(i) for i in latest_bcgui]))    if latest_bcgui else '')
     print(('Local version of bomcheckgui: ' +
            '.'.join([str(i) for i in local_bcgui]))     if local_bcgui else '')
 
     # Collect commands that need executed, and their help info
     cmdlist = []
     infolist = []
-    if latest_getbc > local_getbc:
-        cmdlist.append(dic['getbc'][0])
-        infolist.append(dic['getbc'][1])
+
     if (latest_bc > local_bc) or (latest_bcgui > local_bcgui):
         cmdlist.append(dic['activt'][0])
         infolist.append(dic['activt'][1])
     if latest_bc > local_bc:
         cmdlist.append(dic['bc'][0])
         infolist.append(dic['bc'][1])
     if latest_bcgui > local_bcgui:
@@ -250,23 +279,28 @@
             print(str(i) + ') ' + cmd)
         print('')
         i = 0
         for info in infolist:
             i += 1
             print(str(i) + ') ' + info)
     else:
-        print('\nEverything is up-to-date.')
+        print("\nbomcheckgui and/or bomcheck is up-to-date. No action will be taken.")
+        if latest_getbc > local_getbc:
+            print('This program is not designed to update getbc')
         return
 
     print()
-    x = input('Execute commands (takes a couple of minutes). Continue? (Y/N) ')
-    if x.lower().strip()[0] == 'y':
-        print('working...')
-        commands = ' && '.join(cmdlist) + ' && echo commands executed successfully'
-        os.system(commands)
+    if flag:
+        x = input('Execute commands (takes a couple of minutes). Continue? (Y/N) ')
+        if x.lower().strip()[0] == 'y':
+            print('working...')
+            commands = ' && '.join(cmdlist) + ' && echo commands executed successfully'
+            os.system(commands)
+        else:
+            print('You are not running a MS OS.  No action will be taken.')
 
 
 def local(package):
     ''' Look on the local computer and find out the version no. of "package".
 
     Parameters
     ----------
@@ -281,15 +315,15 @@
        is not found on pypi.org, return [-1, -1, -1]
     '''
 
     if package == 'bomcheck':
         package = Path.joinpath(venvpathname, 'lib', 'site-packages', 'bomcheck.py')
     elif package == 'bomcheckgui':
         package = Path.joinpath(venvpathname, 'lib', 'site-packages', 'bomcheckgui.py')
-    elif package == Path(__file__).stem:
+    elif package == fileName:
         return [int(i) for i in __version__.split('.')]
     else:
         print('Bad argument given to function "local"')
 
     if Path.exists(package):
         with open(package, 'r') as fp:
             lines = fp.readlines()
@@ -350,29 +384,34 @@
     elif desktop2:
         return desktop2[0]
     else:
         desktopnotfound = True
         return str(Path.home())
 
 
+
+
+
+
+
+
+
 try:
     app = QApplication(sys.argv)
     cb=app.clipboard()
 except:
     pass
 
 
 venvname = 'bc-venv'
 venvpathname = Path.joinpath(Path.home(), venvname)
 activate = Path.joinpath(Path.home(), venvname, 'Scripts', 'activate.bat')
-#desktop = Path('~/Desktop/')
-#linkto =   Path.joinpath(desktop.expanduser(), 'bomcheckgui.exe')
 linkto = os.path.join(findDesktop(), 'bomcheckgui.exe')
 linkfrom = Path.joinpath(Path.home(), venvname, 'Scripts', 'bomcheckgui.exe')
-
+flag = True
 
 
 if __name__=='__main__':
     main()
```

