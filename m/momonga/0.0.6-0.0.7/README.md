# Comparing `tmp/momonga-0.0.6-py3-none-any.whl.zip` & `tmp/momonga-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15369 bytes, number of entries: 11
--rw-rw-r--  2.0 unx      136 b- defN 24-Apr-20 08:49 momonga/__init__.py
--rw-rw-r--  2.0 unx    15034 b- defN 24-Apr-26 01:36 momonga/momonga.py
--rw-rw-r--  2.0 unx      959 b- defN 24-Apr-23 04:16 momonga/momonga_exception.py
--rw-rw-r--  2.0 unx     2698 b- defN 24-Apr-24 09:24 momonga/momonga_response.py
--rw-rw-r--  2.0 unx    11915 b- defN 24-Apr-26 00:54 momonga/momonga_session_manager.py
--rw-rw-r--  2.0 unx     9392 b- defN 24-Apr-24 09:23 momonga/momonga_sk_wrapper.py
--rw-rw-r--  2.0 unx     1061 b- defN 24-Apr-26 01:38 momonga-0.0.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx    10353 b- defN 24-Apr-26 01:38 momonga-0.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-26 01:38 momonga-0.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Apr-26 01:38 momonga-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      883 b- defN 24-Apr-26 01:38 momonga-0.0.6.dist-info/RECORD
-11 files, 52531 bytes uncompressed, 13883 bytes compressed:  73.6%
+Zip file size: 15390 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      136 b- defN 24-Apr-30 02:44 momonga/__init__.py
+-rw-r--r--  2.0 unx    15140 b- defN 24-Apr-30 17:27 momonga/momonga.py
+-rw-r--r--  2.0 unx      959 b- defN 24-Apr-30 02:44 momonga/momonga_exception.py
+-rw-r--r--  2.0 unx     2698 b- defN 24-Apr-30 02:44 momonga/momonga_response.py
+-rw-r--r--  2.0 unx    11915 b- defN 24-Apr-30 02:44 momonga/momonga_session_manager.py
+-rw-r--r--  2.0 unx     9392 b- defN 24-Apr-30 02:44 momonga/momonga_sk_wrapper.py
+-rw-r--r--  2.0 unx     1061 b- defN 24-Apr-30 17:29 momonga-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10355 b- defN 24-Apr-30 17:29 momonga-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 17:29 momonga-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-30 17:29 momonga-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      883 b- defN 24-Apr-30 17:29 momonga-0.0.7.dist-info/RECORD
+11 files, 52639 bytes uncompressed, 13904 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: momonga/momonga_session_manager.py
 Comment: 
 
 Filename: momonga/momonga_sk_wrapper.py
 Comment: 
 
-Filename: momonga-0.0.6.dist-info/LICENSE
+Filename: momonga-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: momonga-0.0.6.dist-info/METADATA
+Filename: momonga-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: momonga-0.0.6.dist-info/WHEEL
+Filename: momonga-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: momonga-0.0.6.dist-info/top_level.txt
+Filename: momonga-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: momonga-0.0.6.dist-info/RECORD
+Filename: momonga-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## momonga/momonga.py

```diff
@@ -1,9 +1,10 @@
 
 import datetime
+import time
 import queue
 import logging
 
 from .momonga_exception import *
 from .momonga_response import *
 from .momonga_session_manager import MomongaSessionManager
 from .momonga_session_manager import logger as session_manager_logger
@@ -125,29 +126,30 @@
         self.transaction_id += 1
         tx_payload = self.__build_request_payload(self.transaction_id,
                                                   epc,
                                                   edt)
         while not self.session_manager.recv_q.empty():
             self.session_manager.recv_q.get() # drops stored data
 
-        for _ in range(12):
+        for _ in range(10):
             self.session_manager.xmitter(tx_payload)
             while True:
                 try:
                     res = self.session_manager.recv_q.get(timeout=12)
                 except queue.Empty:
                     logger.warning('Timed out to obtain a response for "%X" request.' % (epc))
                     break
                 if res.startswith('EVENT 21'):
                     param = res.split()[-1]
                     if param == '00':
                         logger.info('Successfully transmitted a packet for "%X" request.' % (epc))
                         continue
                     elif param == '01':
                         logger.warning('Retransmitting the packet for "%X" request.' % (epc))
+                        time.sleep(3)
                         break # to rexmit
                     elif param == '02':
                         logger.warning('Transmitting neighbor solicitation packets.' % (epc))
                         continue
                 elif res.startswith('EVENT 02'):
                     logger.info('Received a neighbor advertisement packet.' % (epc))
                     continue
@@ -173,18 +175,20 @@
         logger.error('Gave up to obtain a response for "%X" request. Close Momonga and open it again.' % (epc))
         raise MomongaNeedToReopen('Gave up to obtain a response for "%X" request. Close Momonga and open it again.' % (epc))
 
     def __prepare_to_get_cumulative_energy(self) -> None:
         if self.energy_coefficient is None:
             try:
                 self.energy_coefficient = self.get_coefficient_for_cumulative_energy()
+                time.sleep(3)
             except MomongaResponseNotPossible:
                 self.energy_coefficient = 1
         if self.energy_unit is None:
             self.energy_unit = self.get_unit_for_cumulative_energy()
+            time.sleep(3)
 
     def get_operation_status(self) -> int:
         res = self.__request(0x80)
         status = int.from_bytes(res.get('edt'), 'big')
         if status == 0x30:   # turned on
             status = True
         elif status == 0x31: # turned off
```

## Comparing `momonga-0.0.6.dist-info/LICENSE` & `momonga-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `momonga-0.0.6.dist-info/METADATA` & `momonga-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: momonga
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Route B Library: A Communicator for Low-voltage Smart Electric Energy Meters
 Home-page: https://github.com/nbtk/momonga
 Author: nbtk
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyserial ~=3.5
+Requires-Dist: pyserial (~=3.5)
 
 # Momonga
 Python Route B Library: A Communicator for Low-voltage Smart Electric Energy Meters
 
 # Description
 MomongaはBルートサービスを利用してスマートメーターと通信するライブラリです。ターゲットデバイスはROHM社製Wi-SUNモジュールBP35C2を搭載したラトックシステムRS-WSUHA-Pです。
```

## Comparing `momonga-0.0.6.dist-info/RECORD` & `momonga-0.0.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 momonga/__init__.py,sha256=iWnaMiIWmYho2GfBZJiZ82rlo4znFfQlqNXkGwNXhLg,136
-momonga/momonga.py,sha256=7pLTNyIQNfSsK8D-GLF2IZTdlKq3i1UMh85tAoAf0vw,15034
+momonga/momonga.py,sha256=BmTl-i5IssvczksHOhqvVtcKm5Y_1cGf1KXhMokyrto,15140
 momonga/momonga_exception.py,sha256=IPcOVNU7mpm-upYTLLo6gIxFHzjCXxs-YwzhIej8PMU,959
 momonga/momonga_response.py,sha256=_t_aaA6z5cpZVGWIkir7J_fgwYabPSNrpBAiS36Ro7c,2698
 momonga/momonga_session_manager.py,sha256=jcOgnpXPdXvzqifyEBDsWMrjyAmuFTPlVaNi1vHbgvY,11915
 momonga/momonga_sk_wrapper.py,sha256=xaffyj3D3Mt84LljroJ07j-GHJTpsXTMp695vztZbz4,9392
-momonga-0.0.6.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
-momonga-0.0.6.dist-info/METADATA,sha256=c1S___K6HrTZSqHm5GkprsanPaPL9ZNDPHLf4sgoAX0,10353
-momonga-0.0.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-momonga-0.0.6.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
-momonga-0.0.6.dist-info/RECORD,,
+momonga-0.0.7.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
+momonga-0.0.7.dist-info/METADATA,sha256=yUQY1fdITvXo2loinVcj3qWQo48MFTRE0FuIbiJGfgY,10355
+momonga-0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+momonga-0.0.7.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
+momonga-0.0.7.dist-info/RECORD,,
```

