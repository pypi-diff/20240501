# Comparing `tmp/aranet4-2.3.3.tar.gz` & `tmp/aranet4-2.3.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aranet4-2.3.3.tar", last modified: Tue Apr  9 09:01:54 2024, max compression
+gzip compressed data, was "aranet4-2.3.4b1.tar", last modified: Wed May  1 05:41:17 2024, max compression
```

## Comparing `aranet4-2.3.3.tar` & `aranet4-2.3.4b1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-09 09:01:54.865465 aranet4-2.3.3/
--rw-r--r--   0 pi        (1000) pi        (1000)     1071 2023-12-06 11:57:48.000000 aranet4-2.3.3/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     6464 2024-04-09 09:01:54.849465 aranet4-2.3.3/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     6079 2023-12-06 11:57:48.000000 aranet4-2.3.3/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-09 09:01:54.829465 aranet4-2.3.3/aranet4/
--rw-r--r--   0 pi        (1000) pi        (1000)      129 2024-04-09 08:59:45.000000 aranet4-2.3.3/aranet4/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7886 2024-04-09 08:58:58.000000 aranet4-2.3.3/aranet4/aranetctl.py
--rw-r--r--   0 pi        (1000) pi        (1000)    35482 2024-04-09 08:57:17.000000 aranet4-2.3.3/aranet4/client.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-09 09:01:54.845466 aranet4-2.3.3/aranet4.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     6464 2024-04-09 09:01:53.000000 aranet4-2.3.3/aranet4.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      273 2024-04-09 09:01:54.000000 aranet4-2.3.3/aranet4.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-09 09:01:53.000000 aranet4-2.3.3/aranet4.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       60 2024-04-09 09:01:53.000000 aranet4-2.3.3/aranet4.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2024-04-09 09:01:53.000000 aranet4-2.3.3/aranet4.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2024-04-09 09:01:53.000000 aranet4-2.3.3/aranet4.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-04-09 09:01:54.865465 aranet4-2.3.3/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      746 2024-04-09 08:59:53.000000 aranet4-2.3.3/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-01 05:41:17.819982 aranet4-2.3.4b1/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1071 2023-12-06 11:57:48.000000 aranet4-2.3.4b1/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     6929 2024-05-01 05:41:17.819982 aranet4-2.3.4b1/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     6542 2024-04-29 07:47:15.000000 aranet4-2.3.4b1/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-01 05:41:17.799982 aranet4-2.3.4b1/aranet4/
+-rw-r--r--   0 pi        (1000) pi        (1000)      131 2024-05-01 05:40:47.000000 aranet4-2.3.4b1/aranet4/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9078 2024-05-01 05:40:58.000000 aranet4-2.3.4b1/aranet4/aranetctl.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    40171 2024-05-01 05:40:42.000000 aranet4-2.3.4b1/aranet4/client.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-01 05:41:17.815982 aranet4-2.3.4b1/aranet4.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6929 2024-05-01 05:41:16.000000 aranet4-2.3.4b1/aranet4.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      273 2024-05-01 05:41:17.000000 aranet4-2.3.4b1/aranet4.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-01 05:41:16.000000 aranet4-2.3.4b1/aranet4.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       60 2024-05-01 05:41:16.000000 aranet4-2.3.4b1/aranet4.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       15 2024-05-01 05:41:16.000000 aranet4-2.3.4b1/aranet4.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        8 2024-05-01 05:41:16.000000 aranet4-2.3.4b1/aranet4.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-05-01 05:41:17.823982 aranet4-2.3.4b1/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      748 2024-05-01 05:40:47.000000 aranet4-2.3.4b1/setup.py
```

### Comparing `aranet4-2.3.3/LICENSE` & `aranet4-2.3.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aranet4-2.3.3/PKG-INFO` & `aranet4-2.3.4b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,94 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.3.3
+Version: 2.3.4b1
 Summary: Aranet Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # Aranet4 Python client
+Python library and command line interface for [Aranet4](https://aranet.com/products/aranet4/), [Aranet2](https://aranet.com/products/aranet2/) and [Aranet Radiation](https://aranet.com/products/aranetradiation/) sensors.
+
 ## Installation
 1. Install aranet4 and its dependencies:
 ```
 pip3 install aranet4
 ```
 2. Pair Aranet4 device
 3. Run `aranetctl` or use as library
 
 **Note:** Smart Home Integrations must be enabled in Aranet4 mobile app for full support.
 
 ## aranetctl usage
 ```text
 $ aranetctl -h
-usage: aranetctl [-h] [-u URL] [-r] [-s DATE] [-e DATE] [-o FILE] [-w] [-l COUNT]
-                 [--xt] [--xh] [--xp] [--xc]
-                 device_mac
+usage: aranetctl.py [-h] [--scan] [-u URL] [-r] [-s DATE] [-e DATE] [-o FILE] [-w] [-l COUNT] [--xt] [--xh] [--xp] [--xc] [--set-interval MINUTES]
+                    [--set-integrations {on,off}] [--set-range {normal,extended}]
+                    [device_mac]
 
 positional arguments:
   device_mac            Aranet4 Bluetooth Address
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  -r, --records         Fetch historical log records
   --scan                Scan Aranet4 devices
+  -r, --records         Fetch historical log records
 
 Options for current reading:
   -u URL, --url URL     Remote url for current value push
 
 Filter History Log Records:
   -s DATE, --start DATE
-                        Records range start (UTC time, example:
-                        2019-09-29T14:00:00
+                        Records range start (UTC time, example: 2019-09-29T14:00:00
   -e DATE, --end DATE   Records range end (UTC time, example: 2019-09-30T14:00:00
   -o FILE, --output FILE
                         Save records to a file
   -w, --wait            Wait until new data point available
   -l COUNT, --last COUNT
                         Get <COUNT> last records
   --xt                  Don't get temperature records
   --xh                  Don't get humidity records
   --xp                  Don't get pressure records
   --xc                  Don't get co2 records
 
+Change device settings:
+  --set-interval MINUTES
+                        Change update interval
+  --set-integrations {on,off}
+                        Toggle Smart Home Integrations
+  --set-range {normal,extended}
+                        Change bluetooth range
+```
+### Scan devices
+Usage: `aranetctl --scan`
+
+Output:
+```
+=======================================
+  Name:     Aranet4 00001
+  Address:  AA:BB:CC:DD:EE:FF
+  RSSI:     -83 dBm
+---------------------------------------
+  CO2:            484 ppm
+  Temperature:    20.9 °C
+  Humidity:       43 %
+  Pressure:       1024.8 hPa
+  Battery:        3 %
+  Status Display: GREEN
+  Age:            9/60
 ```
 
+**Note:** To receive current measurements, Smart Home Integrations must be enabled and firmware version must be v1.2.0 or newer.
+
 ### Current Readings Example
 Usage: `aranetctl XX:XX:XX:XX:XX:XX`
 
 Output:
 ```
 --------------------------------------
 Connected: Aranet4 00000 | v0.3.1
@@ -124,40 +153,14 @@
 
 print("co2 reading:", current.co2)
 print("Temperature:", current.temperature)
 print("Humidity:", current.humidity)
 print("Pressure:", current.pressure)
 ```
 
-### Scanner Example
-Usage: `aranetctl --scan`
-
-Output:
-```
-=======================================
-  Name:     Aranet4 00000
-  Address:  XX:XX:XX:XX:XX:XX
-  RSSI:     -85 dBm
---------------------------------------
-  CO2:           662 pm
-  Temperature:   21.9 °C
-  Humidity:      48 %
-  Pressure:      1019.2 hPa
-  Battery:       34 %
-  Status disp.:  GREEN
-
-=======================================
-  Name:     Aranet4 00001
-  Address:  XX:XX:XX:XX:XX:XX
-  RSSI:     -91 dBm
-
-```
-
-**Note:** To receive current measurements, Smart Home Integrations must be enabled and firmware version must be v1.2.0 or newer.
-
 ### Logged Readings Example
 
 ```python
 import aranet4
 
 device_mac = "XX:XX:XX:XX:XX:XX"
```

### Comparing `aranet4-2.3.3/README.md` & `aranet4-2.3.4b1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,82 @@
+
 # Aranet4 Python client
+Python library and command line interface for [Aranet4](https://aranet.com/products/aranet4/), [Aranet2](https://aranet.com/products/aranet2/) and [Aranet Radiation](https://aranet.com/products/aranetradiation/) sensors.
+
 ## Installation
 1. Install aranet4 and its dependencies:
 ```
 pip3 install aranet4
 ```
 2. Pair Aranet4 device
 3. Run `aranetctl` or use as library
 
 **Note:** Smart Home Integrations must be enabled in Aranet4 mobile app for full support.
 
 ## aranetctl usage
 ```text
 $ aranetctl -h
-usage: aranetctl [-h] [-u URL] [-r] [-s DATE] [-e DATE] [-o FILE] [-w] [-l COUNT]
-                 [--xt] [--xh] [--xp] [--xc]
-                 device_mac
+usage: aranetctl.py [-h] [--scan] [-u URL] [-r] [-s DATE] [-e DATE] [-o FILE] [-w] [-l COUNT] [--xt] [--xh] [--xp] [--xc] [--set-interval MINUTES]
+                    [--set-integrations {on,off}] [--set-range {normal,extended}]
+                    [device_mac]
 
 positional arguments:
   device_mac            Aranet4 Bluetooth Address
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  -r, --records         Fetch historical log records
   --scan                Scan Aranet4 devices
+  -r, --records         Fetch historical log records
 
 Options for current reading:
   -u URL, --url URL     Remote url for current value push
 
 Filter History Log Records:
   -s DATE, --start DATE
-                        Records range start (UTC time, example:
-                        2019-09-29T14:00:00
+                        Records range start (UTC time, example: 2019-09-29T14:00:00
   -e DATE, --end DATE   Records range end (UTC time, example: 2019-09-30T14:00:00
   -o FILE, --output FILE
                         Save records to a file
   -w, --wait            Wait until new data point available
   -l COUNT, --last COUNT
                         Get <COUNT> last records
   --xt                  Don't get temperature records
   --xh                  Don't get humidity records
   --xp                  Don't get pressure records
   --xc                  Don't get co2 records
 
+Change device settings:
+  --set-interval MINUTES
+                        Change update interval
+  --set-integrations {on,off}
+                        Toggle Smart Home Integrations
+  --set-range {normal,extended}
+                        Change bluetooth range
+```
+### Scan devices
+Usage: `aranetctl --scan`
+
+Output:
+```
+=======================================
+  Name:     Aranet4 00001
+  Address:  AA:BB:CC:DD:EE:FF
+  RSSI:     -83 dBm
+---------------------------------------
+  CO2:            484 ppm
+  Temperature:    20.9 °C
+  Humidity:       43 %
+  Pressure:       1024.8 hPa
+  Battery:        3 %
+  Status Display: GREEN
+  Age:            9/60
 ```
 
+**Note:** To receive current measurements, Smart Home Integrations must be enabled and firmware version must be v1.2.0 or newer.
+
 ### Current Readings Example
 Usage: `aranetctl XX:XX:XX:XX:XX:XX`
 
 Output:
 ```
 --------------------------------------
 Connected: Aranet4 00000 | v0.3.1
@@ -112,40 +141,14 @@
 
 print("co2 reading:", current.co2)
 print("Temperature:", current.temperature)
 print("Humidity:", current.humidity)
 print("Pressure:", current.pressure)
 ```
 
-### Scanner Example
-Usage: `aranetctl --scan`
-
-Output:
-```
-=======================================
-  Name:     Aranet4 00000
-  Address:  XX:XX:XX:XX:XX:XX
-  RSSI:     -85 dBm
---------------------------------------
-  CO2:           662 pm
-  Temperature:   21.9 °C
-  Humidity:      48 %
-  Pressure:      1019.2 hPa
-  Battery:       34 %
-  Status disp.:  GREEN
-
-=======================================
-  Name:     Aranet4 00001
-  Address:  XX:XX:XX:XX:XX:XX
-  RSSI:     -91 dBm
-
-```
-
-**Note:** To receive current measurements, Smart Home Integrations must be enabled and firmware version must be v1.2.0 or newer.
-
 ### Logged Readings Example
 
 ```python
 import aranet4
 
 device_mac = "XX:XX:XX:XX:XX:XX"
```

### Comparing `aranet4-2.3.3/aranet4/aranetctl.py` & `aranet4-2.3.4b1/aranet4/aranetctl.py`

 * *Files 14% similar despite different names*

```diff
@@ -75,14 +75,36 @@
     history.add_argument(
         "--xc",
         dest="co2",
         default=True,
         action="store_false",
         help="Don't get co2 records",
     )
+    settings = parser.add_argument_group("Change device settings")
+    settings.add_argument(
+        "--set-interval",
+        dest="set_interval",
+        metavar="MINUTES",
+        type=int,
+        help="Change update interval"
+    )
+    settings.add_argument(
+        "--set-integrations",
+        dest="set_integrations",
+        type=str,
+        choices=["on", "off"],
+        help="Toggle Smart Home Integrations"
+    )
+    settings.add_argument(
+        "--set-range",
+        dest="set_btrange",
+        type=str,
+        choices=["normal", "extended"],
+        help="Change bluetooth range"
+    )
 
     return parser.parse_args(ctl_args)
 
 
 def print_records(records):
     """Format log records to be printed to screen"""
     char_repeat = 34
@@ -233,18 +255,36 @@
         if args.wait:
             wait_for_new_record(args.device_mac)
         records = client.get_all_records(args.device_mac, vars(args), True)
         print_records(records)
         if args.output:
             write_csv(args.output, records)
     else:
-        current = client.get_current_readings(args.device_mac)
-        print(current.toString())
-        if args.url:
-            post_data(args.url, current)
+        settings = {}
+
+        if args.set_interval:
+            settings['interval'] = args.set_interval
+
+        if args.set_integrations:
+            settings['integrations'] = args.set_integrations
+
+        if args.set_btrange:
+            settings['range'] = args.set_btrange
+
+        if settings:
+            result = client.set_settings(args.device_mac, settings, True)
+            for k in result:
+                val = settings[k]
+                ret = "SUCCESS" if result[k] else "FAILED"
+                print(f"Set {k} to \"{val}\": {ret}")
+        else:
+            current = client.get_current_readings(args.device_mac)
+            print(current.toString())
+            if args.url:
+                post_data(args.url, current)
 
 
 def entry_point():
     main(argv=sys.argv[1:])
 
 
 if __name__ == "__main__":
```

### Comparing `aranet4-2.3.3/aranet4/client.py` & `aranet4-2.3.4b1/aranet4/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -293,15 +293,15 @@
         elif param == Param.RADIATION_DOSE:
             invalid_reading_flag = value >> 15 == 1
             multiplier = 1 # nSv
         elif param == Param.RADIATION_DOSE_RATE:
             invalid_reading_flag = value >> 15 == 1
             multiplier = 10 # nSv/h
         elif param == Param.RADIATION_DOSE_INTEGRAL:
-            invalid_reading_flag = value >> 15 == 1
+            invalid_reading_flag = value >> 63 == 1
             multiplier = 1 # nSv
 
         if invalid_reading_flag:
             return -1
         if isinstance(multiplier, float):
             return round(value * multiplier, 1)
         return value * multiplier
@@ -364,26 +364,29 @@
     rssi: int = None
 
     def __init__(self, device = None, ad_data = None):
         self.device = device
 
         if device and ad_data:
             has_manufacturer_data = Aranet4.MANUFACTURER_ID in ad_data.manufacturer_data
-            self.rssi = ad_data.rssi
+            self.rssi = getattr(ad_data, 'rssi', None)
 
             if has_manufacturer_data:
                 mf_data = ManufacturerData()
                 raw_bytes = bytearray(ad_data.manufacturer_data[Aranet4.MANUFACTURER_ID])
                 if len(raw_bytes) < 5:
                     # invalid manufacturer data
                     return
 
-                cond_name = device.name and "Aranet4" in device.name
-                cond_len  = not device.name and len(raw_bytes) in [7,22]
-                if cond_name or cond_len:
+                # Passive scan may return result with no name.
+                valid_name = device.name and device.name.startswith(("Aranet4", "Aranet2", "Aranet\u2622"))
+                cond_name = valid_name and device.name.startswith("Aranet4")
+                cond_len = not valid_name and len(raw_bytes) in [7,22]
+
+                if cond_name or cond_len: # Should be Aranet4
                     raw_bytes.insert(0,0)
 
                 # Basic info
                 value_fmt = "<BBBB"
                 value = struct.unpack(value_fmt, raw_bytes[1:5])
                 mf_data.decode(value)
                 self.manufacturer_data = mf_data
@@ -450,14 +453,78 @@
 class Record:
     name: str
     version: str
     records_on_device: int
     filter: Filter
     value: List[RecordItem] = field(default_factory=list)
 
+@dataclass
+class SensorState:
+    """dataclass to store sensor state values"""
+
+    type: AranetType = AranetType.UNKNOWN
+    buzzerSetting: str = "unknown"
+    calibrationState: str = "unknown"
+    calibrationProgress: int = 0
+    warningPreset: str = "unknown"
+    isLoRaEnabled: bool = False
+    temperatureUnit: str = "unknwonw"
+    isPulseBeepOn: bool = False
+    isUsingCustomThreshold: bool = False
+    isAutomaticCalibrationEnabled: bool = False
+    radiationDisplayUnits: str = "unknwon"
+    isBuzzerAvailable: bool = False
+    bluetoothRange: str = "unknown"
+    isOpenForIntegration: bool = False
+
+    def decode(self, t):
+        n = t[0] == 242 # Aranet2
+        u = t[0] == 241 # Aranet4
+        l = t[0] == 244 # Aranet Radiation
+        c = format(ord(chr(t[1])), '08b')[::-1]
+        o = format(ord(chr(t[2])), '08b')[::-1]
+
+        if u:
+            self.type = AranetType.ARANET4
+        elif n:
+            self.type = AranetType.ARANET2
+        elif l:
+            self.type = AranetType.ARANET_RADIATION
+        else:
+            self.type = AranetType.UNKNOWN
+
+        self.buzzerSetting = self.cond(c[0], self.cond(c[1], "each", "once"), "off")
+        self.calibrationState = self.cond(u, self.parseCalibrationState(t[1]), "none")
+        self.calibrationProgress = self.cond(u, t[3], 0)
+        self.warningPreset = self.cond(n, self.cond(t[3] == 1, "ISO", "custom"), "none")
+        self.isLoRaEnabled = self.cond(c[4], True, False)
+        self.temperatureUnit = self.cond(l, "none", self.cond(c[5], "C", "F"))
+        self.isPulseBeepOn = self.cond(l, _eval(c[5]), False)
+        self.isUsingCustomThreshold = l and c[6]
+        self.isAutomaticCalibrationEnabled = u and c[7]
+        self.radiationDisplayUnits = self.cond(l, self.cond(c[7], "Sv", "rem"), "none")
+        self.isBuzzerAvailable = self.cond(u, _eval(o[0]), l)
+        self.bluetoothRange = self.cond(o[1], "extended", "normal")
+        self.isOpenForIntegration = _eval(o[7])
+
+    @staticmethod
+    def parseCalibrationState(e):
+        t = format(ord(chr(e)), '08b')[::-1]
+        return SensorState.cond(
+            t[3],
+            SensorState.cond(t[2], "inErrorState", "endRequest"),
+            SensorState.cond(t[2], "inProgress", "notActive")
+        )
+
+    @staticmethod
+    def cond(check, tru, fal):
+        if _eval(check):
+            return tru
+        return fal
+
 
 class HistoryHeader(NamedTuple):
     param: int
     interval: int
     total_readings: int
     ago: int
     start: int
@@ -490,14 +557,16 @@
     AR2_READ_CURRENT_READINGS_A = "f0cd3003-95da-4f4b-9ac8-aa55d312af0c" # data is same as other
     # aranet2 has different service uids. use rhose
     AR4_READ_INTERVAL = "f0cd2002-95da-4f4b-9ac8-aa55d312af0c"
     AR4_READ_SECONDS_SINCE_UPDATE = "f0cd2004-95da-4f4b-9ac8-aa55d312af0c"
     AR4_READ_TOTAL_READINGS = "f0cd2001-95da-4f4b-9ac8-aa55d312af0c"
     AR4_READ_HISTORY_READINGS_V1 = "f0cd2003-95da-4f4b-9ac8-aa55d312af0c"
     AR4_READ_HISTORY_READINGS_V2 = "f0cd2005-95da-4f4b-9ac8-aa55d312af0c"
+    AR4_READ_SENSOR_STATE = "f0cd1401-95da-4f4b-9ac8-aa55d312af0c"
+
 
     # Read / Generic servce
     GENERIC_READ_DEVICE_NAME = "00002a00-0000-1000-8000-00805f9b34fb"
 
     # Read / Common servce
     COMMON_READ_MANUFACTURER_NAME = "00002a29-0000-1000-8000-00805f9b34fb"
     COMMON_READ_MODEL_NUMBER = "00002a24-0000-1000-8000-00805f9b34fb"
@@ -722,34 +791,55 @@
             self.AR4_READ_HISTORY_READINGS_V1, delegate.handle_notification
         )
         while self.reading:
             await asyncio.sleep(0.1)
         await self.device.stop_notify(self.AR4_READ_HISTORY_READINGS_V1)
         return delegate.result
 
-    async def set_readings_interval(self, interval: int):
+    async def set_readings_interval(self, interval: int, verify: bool=True):
         """Set reading interval"""
         header = 0x90
         val = struct.pack("<BB", header, interval)
         await self.device.write_gatt_char(self.AR4_WRITE_CMD, val, True)
+        if verify:
+            iv = await self.get_interval()
+            return interval == (iv / 60)
+        return True
 
-    async def set_home_integration_enabled(self, enabled: bool):
+    async def set_home_integration_enabled(self, enabled: bool, verify: bool=True):
         """
         Toggle smart home integrations.
         This is required to receive measurements in advertisements.
         """
         header = 0x91
         val = struct.pack("<BB", header, 1 if enabled else 0)
         await self.device.write_gatt_char(self.AR4_WRITE_CMD, val, True)
+        if verify:
+            state = await self.get_sensor_state()
+            return enabled == state.isOpenForIntegration
+        return True
 
-    async def set_bluetooth_range(self, extended: bool):
+    async def set_bluetooth_range(self, extended: bool, verify: bool=True):
         """Set bluetooth range"""
-        header = 0x91
+        header = 0x92
         val = struct.pack("<BB", header, 1 if extended else 0)
         await self.device.write_gatt_char(self.AR4_WRITE_CMD, val, True)
+        if verify:
+            state = await self.get_sensor_state()
+            if extended:
+                return state.bluetoothRange == "extended"
+            else:
+                return state.bluetoothRange == "normal"
+
+    async def get_sensor_state(self):
+        """Return the count of how many datapoints are logged on device"""
+        raw_bytes = await self.device.read_gatt_char(self.AR4_READ_SENSOR_STATE)
+        state = SensorState()
+        state.decode(raw_bytes)
+        return state
 
 
 def _log_times(now, total, interval, ago):
     """Calculate the actual times datapoints were logged on device"""
     times = []
     start = now - datetime.timedelta(seconds=((total - 1) * interval) + ago)
     for idx in range(total):
@@ -810,19 +900,50 @@
     await monitor.connect()
     readings = await monitor.current_readings(details=True)
     readings.name = await monitor.get_name()
     readings.version = await monitor.get_version()
     readings.stored = await monitor.get_total_readings()
     return readings
 
+def _eval(val) -> bool:
+    falsy = ['0', 'false', 'disable', 'disabled', 'no', 'off', "none"]
+    if isinstance(val, str):
+        return val.lower() not in falsy
+    return bool(val)
+
+async def _set_settings(address, settings, verify: bool=True) -> dict:
+    """Change device settings. Returns changed count"""
+    monitor = Aranet4(address=address)
+    await monitor.connect()
+    status = {}
+
+    if 'interval' in settings:
+        intval = int(settings['interval'])
+        status['interval'] = await monitor.set_readings_interval(intval, verify)
+
+    if 'range' in settings:
+        extend = ['extend', 'extended', '1']
+        extend = settings['range'].lower() in extend
+        status['range'] = await monitor.set_bluetooth_range(extend, verify)
+
+    if 'integrations' in settings:
+        on = ['on', 'enable', 'enabled', '1']
+        on = settings['integrations'].lower() in on
+        status['integrations'] = await monitor.set_home_integration_enabled(on, verify)
+
+    return status
 
 def get_current_readings(mac_address: str) -> CurrentReading:
     """Get from the device the current measurements"""
     return asyncio.run(_current_reading(mac_address))
 
+def set_settings(mac_address: str, settings: dict, verify: bool=True) -> int:
+    """Get from the device the current measurements"""
+    return asyncio.run(_set_settings(mac_address, settings, verify))
+
 
 class Aranet4Scanner:
     """Aranet4 Scanner class - scan advertisements and process data, if available"""
 
     def _process_advertisement(self, device, ad_data):
         """Processes Aranet4 advertisement data"""
         adv = Aranet4Advertisement(device, ad_data)
@@ -961,15 +1082,15 @@
     else:
         rad_dose_val = _empty_reading(log_size)
     if rec_filter.incl_rad_dose_rate:
         rad_dose_rate_val = await monitor.get_records(
             Param.RADIATION_DOSE_RATE, log_size=log_size, start=begin, end=end
         )
     else:
-        rad_dose_total_val = _empty_reading(log_size)
+        rad_dose_rate_val = _empty_reading(log_size)
     if rec_filter.incl_rad_dose_total:
         rad_dose_total_val = await monitor.get_records(
             Param.RADIATION_DOSE_INTEGRAL, log_size=log_size, start=begin, end=end
         )
     else:
         rad_dose_total_val = _empty_reading(log_size)
 ####
```

### Comparing `aranet4-2.3.3/aranet4.egg-info/PKG-INFO` & `aranet4-2.3.4b1/aranet4.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,94 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.3.3
+Version: 2.3.4b1
 Summary: Aranet Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # Aranet4 Python client
+Python library and command line interface for [Aranet4](https://aranet.com/products/aranet4/), [Aranet2](https://aranet.com/products/aranet2/) and [Aranet Radiation](https://aranet.com/products/aranetradiation/) sensors.
+
 ## Installation
 1. Install aranet4 and its dependencies:
 ```
 pip3 install aranet4
 ```
 2. Pair Aranet4 device
 3. Run `aranetctl` or use as library
 
 **Note:** Smart Home Integrations must be enabled in Aranet4 mobile app for full support.
 
 ## aranetctl usage
 ```text
 $ aranetctl -h
-usage: aranetctl [-h] [-u URL] [-r] [-s DATE] [-e DATE] [-o FILE] [-w] [-l COUNT]
-                 [--xt] [--xh] [--xp] [--xc]
-                 device_mac
+usage: aranetctl.py [-h] [--scan] [-u URL] [-r] [-s DATE] [-e DATE] [-o FILE] [-w] [-l COUNT] [--xt] [--xh] [--xp] [--xc] [--set-interval MINUTES]
+                    [--set-integrations {on,off}] [--set-range {normal,extended}]
+                    [device_mac]
 
 positional arguments:
   device_mac            Aranet4 Bluetooth Address
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  -r, --records         Fetch historical log records
   --scan                Scan Aranet4 devices
+  -r, --records         Fetch historical log records
 
 Options for current reading:
   -u URL, --url URL     Remote url for current value push
 
 Filter History Log Records:
   -s DATE, --start DATE
-                        Records range start (UTC time, example:
-                        2019-09-29T14:00:00
+                        Records range start (UTC time, example: 2019-09-29T14:00:00
   -e DATE, --end DATE   Records range end (UTC time, example: 2019-09-30T14:00:00
   -o FILE, --output FILE
                         Save records to a file
   -w, --wait            Wait until new data point available
   -l COUNT, --last COUNT
                         Get <COUNT> last records
   --xt                  Don't get temperature records
   --xh                  Don't get humidity records
   --xp                  Don't get pressure records
   --xc                  Don't get co2 records
 
+Change device settings:
+  --set-interval MINUTES
+                        Change update interval
+  --set-integrations {on,off}
+                        Toggle Smart Home Integrations
+  --set-range {normal,extended}
+                        Change bluetooth range
+```
+### Scan devices
+Usage: `aranetctl --scan`
+
+Output:
+```
+=======================================
+  Name:     Aranet4 00001
+  Address:  AA:BB:CC:DD:EE:FF
+  RSSI:     -83 dBm
+---------------------------------------
+  CO2:            484 ppm
+  Temperature:    20.9 °C
+  Humidity:       43 %
+  Pressure:       1024.8 hPa
+  Battery:        3 %
+  Status Display: GREEN
+  Age:            9/60
 ```
 
+**Note:** To receive current measurements, Smart Home Integrations must be enabled and firmware version must be v1.2.0 or newer.
+
 ### Current Readings Example
 Usage: `aranetctl XX:XX:XX:XX:XX:XX`
 
 Output:
 ```
 --------------------------------------
 Connected: Aranet4 00000 | v0.3.1
@@ -124,40 +153,14 @@
 
 print("co2 reading:", current.co2)
 print("Temperature:", current.temperature)
 print("Humidity:", current.humidity)
 print("Pressure:", current.pressure)
 ```
 
-### Scanner Example
-Usage: `aranetctl --scan`
-
-Output:
-```
-=======================================
-  Name:     Aranet4 00000
-  Address:  XX:XX:XX:XX:XX:XX
-  RSSI:     -85 dBm
---------------------------------------
-  CO2:           662 pm
-  Temperature:   21.9 °C
-  Humidity:      48 %
-  Pressure:      1019.2 hPa
-  Battery:       34 %
-  Status disp.:  GREEN
-
-=======================================
-  Name:     Aranet4 00001
-  Address:  XX:XX:XX:XX:XX:XX
-  RSSI:     -91 dBm
-
-```
-
-**Note:** To receive current measurements, Smart Home Integrations must be enabled and firmware version must be v1.2.0 or newer.
-
 ### Logged Readings Example
 
 ```python
 import aranet4
 
 device_mac = "XX:XX:XX:XX:XX:XX"
```

### Comparing `aranet4-2.3.3/setup.py` & `aranet4-2.3.4b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aranet4",
-    version="2.3.3",
+    version="2.3.4b1",
     description="Aranet Python client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anrijs/Aranet4-Python",
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python',
```

