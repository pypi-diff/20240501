# Comparing `tmp/upb_lib-0.5.4.tar.gz` & `tmp/upb_lib-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upb_lib-0.5.4.tar", max compression
+gzip compressed data, was "upb_lib-0.5.5.tar", max compression
```

## Comparing `upb_lib-0.5.4.tar` & `upb_lib-0.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      267 2021-11-11 16:09:56.350069 upb_lib-0.5.4/CHANGELOG.md
--rw-r--r--   0        0        0     6734 2023-01-26 15:49:21.898249 upb_lib-0.5.4/README.md
--rw-r--r--   0        0        0    13075 2023-01-26 15:49:21.898815 upb_lib-0.5.4/bin/cmdr.py
--rwxr-xr-x   0        0        0     1306 2023-05-09 21:14:29.185676 upb_lib-0.5.4/bin/simple
--rwxr-xr-x   0        0        0     2912 2023-01-26 15:49:21.899343 upb_lib-0.5.4/bin/upb
--rwxr-xr-x   0        0        0    24791 2023-05-09 21:08:39.586101 upb_lib-0.5.4/bin/upb.upe
--rw-r--r--   0        0        0      745 2023-05-09 20:40:20.724502 upb_lib-0.5.4/pyproject.toml
--rw-r--r--   0        0        0       54 2021-11-11 16:09:56.351490 upb_lib-0.5.4/upb_lib/__init__.py
--rw-r--r--   0        0        0     5149 2021-11-11 16:09:56.351596 upb_lib-0.5.4/upb_lib/const.py
--rw-r--r--   0        0        0     5695 2023-01-26 15:49:21.900869 upb_lib-0.5.4/upb_lib/devices.py
--rw-r--r--   0        0        0     3657 2021-11-11 16:09:56.351783 upb_lib-0.5.4/upb_lib/elements.py
--rw-r--r--   0        0        0     5088 2023-01-26 15:49:08.219407 upb_lib-0.5.4/upb_lib/links.py
--rw-r--r--   0        0        0     5168 2023-01-26 15:49:21.901489 upb_lib-0.5.4/upb_lib/message.py
--rw-r--r--   0        0        0     3281 2023-05-09 21:15:03.160993 upb_lib-0.5.4/upb_lib/parse_upstart.py
--rw-r--r--   0        0        0     7683 2023-01-26 15:49:21.902025 upb_lib-0.5.4/upb_lib/proto.py
--rw-r--r--   0        0        0     7862 2023-01-26 15:49:21.902417 upb_lib-0.5.4/upb_lib/upb.py
--rw-r--r--   0        0        0     1943 2023-01-26 15:49:21.902690 upb_lib-0.5.4/upb_lib/util.py
--rw-r--r--   0        0        0     7516 1970-01-01 00:00:00.000000 upb_lib-0.5.4/setup.py
--rw-r--r--   0        0        0     7518 1970-01-01 00:00:00.000000 upb_lib-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      267 2021-11-11 16:09:56.350069 upb_lib-0.5.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2021-11-11 16:09:56.350154 upb_lib-0.5.5/LICENCE
+-rw-r--r--   0        0        0     6734 2023-01-26 15:49:21.898249 upb_lib-0.5.5/README.md
+-rw-r--r--   0        0        0    13075 2023-01-26 15:49:21.898815 upb_lib-0.5.5/bin/cmdr.py
+-rwxr-xr-x   0        0        0     1306 2023-05-09 21:14:29.185676 upb_lib-0.5.5/bin/simple
+-rwxr-xr-x   0        0        0     2912 2023-01-26 15:49:21.899343 upb_lib-0.5.5/bin/upb
+-rwxr-xr-x   0        0        0    24791 2023-05-09 21:08:39.586101 upb_lib-0.5.5/bin/upb.upe
+-rw-r--r--   0        0        0      752 2024-05-01 18:35:45.301341 upb_lib-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0       54 2021-11-11 16:09:56.351490 upb_lib-0.5.5/upb_lib/__init__.py
+-rw-r--r--   0        0        0     5149 2021-11-11 16:09:56.351596 upb_lib-0.5.5/upb_lib/const.py
+-rw-r--r--   0        0        0     5695 2023-01-26 15:49:21.900869 upb_lib-0.5.5/upb_lib/devices.py
+-rw-r--r--   0        0        0     3657 2021-11-11 16:09:56.351783 upb_lib-0.5.5/upb_lib/elements.py
+-rw-r--r--   0        0        0     5088 2023-01-26 15:49:08.219407 upb_lib-0.5.5/upb_lib/links.py
+-rw-r--r--   0        0        0     5168 2023-01-26 15:49:21.901489 upb_lib-0.5.5/upb_lib/message.py
+-rw-r--r--   0        0        0     3281 2023-05-09 21:15:03.160993 upb_lib-0.5.5/upb_lib/parse_upstart.py
+-rw-r--r--   0        0        0     7683 2023-01-26 15:49:21.902025 upb_lib-0.5.5/upb_lib/proto.py
+-rw-r--r--   0        0        0     7872 2024-05-01 18:31:21.320538 upb_lib-0.5.5/upb_lib/upb.py
+-rw-r--r--   0        0        0     1943 2023-01-26 15:49:21.902690 upb_lib-0.5.5/upb_lib/util.py
+-rw-r--r--   0        0        0     7375 1970-01-01 00:00:00.000000 upb_lib-0.5.5/PKG-INFO
```

### Comparing `upb_lib-0.5.4/README.md` & `upb_lib-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/bin/cmdr.py` & `upb_lib-0.5.5/bin/cmdr.py`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/bin/simple` & `upb_lib-0.5.5/bin/simple`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/bin/upb` & `upb_lib-0.5.5/bin/upb`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/bin/upb.upe` & `upb_lib-0.5.5/bin/upb.upe`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/pyproject.toml` & `upb_lib-0.5.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "upb-lib"
-version = "0.5.4"
+version = "0.5.5"
 description = "Library for interacting with UPB PIM."
 homepage = "https://github.com/gwww/upb-lib"
 authors = ["Glenn Waters <gwwaters+upb@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
   'Development Status :: 4 - Beta',
   'Intended Audience :: Developers',
 ]
 include = ["CHANGELOG.md", "bin/**/*"]
 exclude = ["test"]
 
 [tool.poetry.dependencies]
-python = ">= 3.7"
+python = ">= 3.11"
 pytz = ">= 2021"
-pyserial-asyncio = ">= 0.5"
+pyserial-asyncio-fast = ">= 0.11"
 
 [tool.poetry.dev-dependencies]
 pytest = ">= 7.2"
 urwid = ">= 2.0"
 attrs = ">= 21.2"
 colorlog = ">= 4.0"
 black = ">= 22.3"
```

### Comparing `upb_lib-0.5.4/upb_lib/const.py` & `upb_lib-0.5.5/upb_lib/const.py`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/upb_lib/devices.py` & `upb_lib-0.5.5/upb_lib/devices.py`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/upb_lib/elements.py` & `upb_lib-0.5.5/upb_lib/elements.py`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/upb_lib/links.py` & `upb_lib-0.5.5/upb_lib/links.py`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/upb_lib/message.py` & `upb_lib-0.5.5/upb_lib/message.py`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/upb_lib/parse_upstart.py` & `upb_lib-0.5.5/upb_lib/parse_upstart.py`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/upb_lib/proto.py` & `upb_lib-0.5.5/upb_lib/proto.py`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/upb_lib/upb.py` & `upb_lib-0.5.5/upb_lib/upb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Master class that combines all UPB pieces together."""
 
 import asyncio
 import logging
 from functools import partial
 
-import serial_asyncio
+import serial_asyncio_fast
 
 from .const import PimCommand
 from .devices import UpbAddr, UpbDevices
 from .links import Links
 from .message import MessageDecode, MessageEncode
 from .parse_upstart import process_upstart_file
 from .proto import Connection
@@ -60,15 +60,15 @@
             self._connected,
             self._disconnected,
             self._got_data,
             self._timeout,
         )
         try:
             if scheme == "serial":
-                await serial_asyncio.create_serial_connection(
+                await serial_asyncio_fast.create_serial_connection(
                     self.loop, conn, dest, baudrate=param
                 )
             else:
                 await asyncio.wait_for(
                     self.loop.create_connection(conn, host=dest, port=param, ssl=None),
                     timeout=5,
                 )
```

### Comparing `upb_lib-0.5.4/upb_lib/util.py` & `upb_lib-0.5.5/upb_lib/util.py`

 * *Files identical despite different names*

### Comparing `upb_lib-0.5.4/setup.py` & `upb_lib-0.5.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,137 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: upb-lib
+Version: 0.5.5
+Summary: Library for interacting with UPB PIM.
+Home-page: https://github.com/gwww/upb-lib
+License: MIT
+Author: Glenn Waters
+Author-email: gwwaters+upb@gmail.com
+Requires-Python: >=3.11
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pyserial-asyncio-fast (>=0.11)
+Requires-Dist: pytz (>=2021)
+Description-Content-Type: text/markdown
 
-packages = \
-['upb_lib']
+# Python UPB Powerline Interface library
 
-package_data = \
-{'': ['*']}
+Library for interacting with UPB PIM/CIM
 
-install_requires = \
-['pyserial-asyncio>=0.5', 'pytz>=2021']
-
-setup_kwargs = {
-    'name': 'upb-lib',
-    'version': '0.5.4',
-    'description': 'Library for interacting with UPB PIM.',
-    'long_description': '# Python UPB Powerline Interface library\n\nLibrary for interacting with UPB PIM/CIM\n\nhttps://github.com/gwww/upb-lib\n\n## Requirements\n\n- Python 3.7 (or higher)\n\n## Description\n\nThis package is created as a library to interact with an UPB PIM.\nThe motivation to write this was to use with the Home Assistant\nautomation platform. The library can be used for writing other UPB\napplications. The IO with the PIM is asynchronous over TCP or over the\nserial port.\n\n## Installation\n\n```bash\n    $ pip install upb_lib\n```\n\n## Overview\n\nSimplest thing right now is when in the root of the git repo that you have cloned is to enter the command `bin/simple`. This program requires that the environment variable `UPBPIM_URL` set to indicate how to connect to the PIM. For example, `serial:///dev/cu.KeySerial1` connects to the PIM on a serial port (`serial://`) `/dev/cu/KeySerial1`. On Windows something like `serial://COM1` might work.\n\nAlso required is a `UPStart` export file. The `bin/simple` program looks for it\nin the same directory as where the program is (i.e.: `bin`) and assumes that it is named `upb.upe`.\n\n## Configuration\n\nInitialization of the library takes the following parameters:\n\n`url`: This is the PIM to connect to. It is formatted as a URL. Two formats\nare supported: `serial://<device>` where `<device>` is the serial/USB port on which the PIM is connected; `tcp://<IP or domain>[:<port]` where IP or domain is where the device is connected on the network (perhaps using [ser2tcp](https://github.com/gwww/ser2tcp) or a PIM-U) and an optional `port` number with a default of 2101.\n\n`UPStartExportFile`: the path of where to read the export file generated through File->Export on the UpStart utility. This is optional but recommended.\n\n`tx_count`: (optional) The number of times every UPB message is transmitted (CNT portion of the control word). Defaults to 1. Setting the value to 2 may be required for networks that use a repeater.\n\n`flags`: (optional) A string that contains a set of comma separated flags. Each flag can take the form of <flag_name> or <flag_name>=<value>. Parse is simple with no escapes. So, values cannot contain commas or equals. Flags supported are:\n\n- `unlimited_blink_rate`: By default the minimum value that can be pass to blink a light or link is 30 (which is about 1/2 a second). When this flag is specified the minimum is 1.\n- `use_raw_rate`: By default the API takes the number of seconds as the rate in which to transition lights to their new level. The number of seconds is coverted to the closest rate value that UPB understands (see rate table below). For example, if a request is to transition a light to its new state in 8 seconds, the closest value that UPB supports is 6.6 seconds and that is the transition time that will be used. If the use raw rate flag is given on initializing this library then the rate value is assumed to be the UPB rate value. i.e.: not in seconds but is a value that UPB "understands".\n- `report_state`: By default the API does not ask for a state update from a device when issuing goto, fade start, or blink commands. Including this flag on startup of the library will cause a report state to be issued immediately following one of the mentioned state changing commands.\n- `no_sync`: By default when the library first starts a report state is sent to every device to synchronize the state of the UPB network with the library. This flag turns off the initial sync. This was put in place for debugging and is not expected to be used outside of that.\n- `heartbeat_timeout_sec`: Overrides the duration of idleness (no messages being received) after which the library will re-initialize the connection, possibly triggering a sync. Applies only to the `tcp` protocol, and defaults to 90 seconds. Setting the value to -1 disables this feature.\n\n## First use of the API\n\nRead the code in `bin/simple`. That is the short use of the API around. Beyond that look at the file `lights.py` and `links.py`. Any method in those files that has a description that starts with `(Helper)` are generally UPB actions.\n\n## Usage\n\n### Naming\nUPB device name are a concatenation of the UPB network ID, the UPB device ID, and the channel number of the device. An underscore separates the values. For example, for a single channel UPB device number 42 on UPB network 142 the device name used in the library would be `"142_42_0"`. For a multi-channel device the channel numbers start at 0.\n\nUPB Links are named as a concatenation of the UPB network ID and the link number. For example, link number 6 on UPB network 142 would be `"142_6"`.\n\nSee `bin/simple` for example code.\n\n### Transition Rate\nMany UPB commands take a `rate`. This API supports the rate as a number of seconds, which is different than what the protocol uses. The protocol allows a set of distinct rates, listed below. For example in the UPB protocol if the rate 7 is sent to a device then the fade rate (for example) would be 20 seconds.\n\nSince the API takes a value in seconds and any number of seconds can be specified, what the API does is convert the number of seconds to the closest rate. For example, if a rate of 24 seconds is passed to the API then the API will convert that to the nearest protocol rate value, which in this case is 7.\n\nThe values of the UPB protocol rate values and mapped to the number of seconds is as follows (at least for Simply Automated devices):\n\n```\n0 = Snap\n1 = 0.8 seconds\n2 = 1.6 seconds\n3 = 3.3 seconds\n4 = 5.0 seconds\n5 = 6.6 seconds\n6 = 10 seconds\n7 = 20 seconds\n8 = 30 seconds\n9 = 1 minute\n10 = 2 minutes\n11 = 5 minutes\n12 = 10 minutes\n13 = 15 minutes\n14 = 30 minutes\n15 = 1 hour\n```\n\n## Development\n\nThis project uses [poetry](https://poetry.eustace.io/) for development dependencies. Installation instructions are on their website.\n\nTo get started developing:\n\n```\ngit clone https://github.com/gwww/upb-lib.git\ncd upb\npoetry install\npoetry shell # Or activate the created virtual environment\nmake test # to ensure everything installed properly\n```\n\nThere is a `Makefile` in the root directory as well. The `make` command\nfollowed by one of the targets in the `Makefile` can be used. If you don\'t\nhave or wish to use `make` the `Makefile` serves as examples of common\ncommands that can be run.\n\n## Working with the UPB Protocol\n\nUseful information on the UPB protocol can be found in the following documents:\n  1. [UPB System Description](https://www.ipcf.org/doc/UPB_System_Description_v1.1.pdf)\n  1. [Powerline Interface Module Description](http://www.webmtn.com/webUniversity/upbDocs/PimComm1.6.pdf)\n\nUsing [ser2net](https://linux.die.net/man/8/ser2net) to proxy and examine\ncommands sent by [UpStart](https://pcswebstore.com/pages/upb-software) can also\nbe insightful.\n',
-    'author': 'Glenn Waters',
-    'author_email': 'gwwaters+upb@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/gwww/upb-lib',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7',
-}
+https://github.com/gwww/upb-lib
 
+## Requirements
+
+- Python 3.7 (or higher)
+
+## Description
+
+This package is created as a library to interact with an UPB PIM.
+The motivation to write this was to use with the Home Assistant
+automation platform. The library can be used for writing other UPB
+applications. The IO with the PIM is asynchronous over TCP or over the
+serial port.
+
+## Installation
+
+```bash
+    $ pip install upb_lib
+```
+
+## Overview
+
+Simplest thing right now is when in the root of the git repo that you have cloned is to enter the command `bin/simple`. This program requires that the environment variable `UPBPIM_URL` set to indicate how to connect to the PIM. For example, `serial:///dev/cu.KeySerial1` connects to the PIM on a serial port (`serial://`) `/dev/cu/KeySerial1`. On Windows something like `serial://COM1` might work.
+
+Also required is a `UPStart` export file. The `bin/simple` program looks for it
+in the same directory as where the program is (i.e.: `bin`) and assumes that it is named `upb.upe`.
+
+## Configuration
+
+Initialization of the library takes the following parameters:
+
+`url`: This is the PIM to connect to. It is formatted as a URL. Two formats
+are supported: `serial://<device>` where `<device>` is the serial/USB port on which the PIM is connected; `tcp://<IP or domain>[:<port]` where IP or domain is where the device is connected on the network (perhaps using [ser2tcp](https://github.com/gwww/ser2tcp) or a PIM-U) and an optional `port` number with a default of 2101.
+
+`UPStartExportFile`: the path of where to read the export file generated through File->Export on the UpStart utility. This is optional but recommended.
+
+`tx_count`: (optional) The number of times every UPB message is transmitted (CNT portion of the control word). Defaults to 1. Setting the value to 2 may be required for networks that use a repeater.
+
+`flags`: (optional) A string that contains a set of comma separated flags. Each flag can take the form of <flag_name> or <flag_name>=<value>. Parse is simple with no escapes. So, values cannot contain commas or equals. Flags supported are:
+
+- `unlimited_blink_rate`: By default the minimum value that can be pass to blink a light or link is 30 (which is about 1/2 a second). When this flag is specified the minimum is 1.
+- `use_raw_rate`: By default the API takes the number of seconds as the rate in which to transition lights to their new level. The number of seconds is coverted to the closest rate value that UPB understands (see rate table below). For example, if a request is to transition a light to its new state in 8 seconds, the closest value that UPB supports is 6.6 seconds and that is the transition time that will be used. If the use raw rate flag is given on initializing this library then the rate value is assumed to be the UPB rate value. i.e.: not in seconds but is a value that UPB "understands".
+- `report_state`: By default the API does not ask for a state update from a device when issuing goto, fade start, or blink commands. Including this flag on startup of the library will cause a report state to be issued immediately following one of the mentioned state changing commands.
+- `no_sync`: By default when the library first starts a report state is sent to every device to synchronize the state of the UPB network with the library. This flag turns off the initial sync. This was put in place for debugging and is not expected to be used outside of that.
+- `heartbeat_timeout_sec`: Overrides the duration of idleness (no messages being received) after which the library will re-initialize the connection, possibly triggering a sync. Applies only to the `tcp` protocol, and defaults to 90 seconds. Setting the value to -1 disables this feature.
+
+## First use of the API
+
+Read the code in `bin/simple`. That is the short use of the API around. Beyond that look at the file `lights.py` and `links.py`. Any method in those files that has a description that starts with `(Helper)` are generally UPB actions.
+
+## Usage
+
+### Naming
+UPB device name are a concatenation of the UPB network ID, the UPB device ID, and the channel number of the device. An underscore separates the values. For example, for a single channel UPB device number 42 on UPB network 142 the device name used in the library would be `"142_42_0"`. For a multi-channel device the channel numbers start at 0.
+
+UPB Links are named as a concatenation of the UPB network ID and the link number. For example, link number 6 on UPB network 142 would be `"142_6"`.
+
+See `bin/simple` for example code.
+
+### Transition Rate
+Many UPB commands take a `rate`. This API supports the rate as a number of seconds, which is different than what the protocol uses. The protocol allows a set of distinct rates, listed below. For example in the UPB protocol if the rate 7 is sent to a device then the fade rate (for example) would be 20 seconds.
+
+Since the API takes a value in seconds and any number of seconds can be specified, what the API does is convert the number of seconds to the closest rate. For example, if a rate of 24 seconds is passed to the API then the API will convert that to the nearest protocol rate value, which in this case is 7.
+
+The values of the UPB protocol rate values and mapped to the number of seconds is as follows (at least for Simply Automated devices):
+
+```
+0 = Snap
+1 = 0.8 seconds
+2 = 1.6 seconds
+3 = 3.3 seconds
+4 = 5.0 seconds
+5 = 6.6 seconds
+6 = 10 seconds
+7 = 20 seconds
+8 = 30 seconds
+9 = 1 minute
+10 = 2 minutes
+11 = 5 minutes
+12 = 10 minutes
+13 = 15 minutes
+14 = 30 minutes
+15 = 1 hour
+```
+
+## Development
+
+This project uses [poetry](https://poetry.eustace.io/) for development dependencies. Installation instructions are on their website.
+
+To get started developing:
+
+```
+git clone https://github.com/gwww/upb-lib.git
+cd upb
+poetry install
+poetry shell # Or activate the created virtual environment
+make test # to ensure everything installed properly
+```
+
+There is a `Makefile` in the root directory as well. The `make` command
+followed by one of the targets in the `Makefile` can be used. If you don't
+have or wish to use `make` the `Makefile` serves as examples of common
+commands that can be run.
+
+## Working with the UPB Protocol
+
+Useful information on the UPB protocol can be found in the following documents:
+  1. [UPB System Description](https://www.ipcf.org/doc/UPB_System_Description_v1.1.pdf)
+  1. [Powerline Interface Module Description](http://www.webmtn.com/webUniversity/upbDocs/PimComm1.6.pdf)
+
+Using [ser2net](https://linux.die.net/man/8/ser2net) to proxy and examine
+commands sent by [UpStart](https://pcswebstore.com/pages/upb-software) can also
+be insightful.
 
-setup(**setup_kwargs)
```

