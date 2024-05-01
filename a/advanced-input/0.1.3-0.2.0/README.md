# Comparing `tmp/advanced_input-0.1.3.tar.gz` & `tmp/advanced_input-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advanced_input-0.1.3.tar", last modified: Tue Apr 30 06:38:12 2024, max compression
+gzip compressed data, was "advanced_input-0.2.0.tar", last modified: Wed May  1 07:24:48 2024, max compression
```

## Comparing `advanced_input-0.1.3.tar` & `advanced_input-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 06:38:12.562041 advanced_input-0.1.3/
--rw-rw-rw-   0        0        0     1235 2020-07-21 09:29:29.000000 advanced_input-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1691 2024-04-30 06:38:12.561042 advanced_input-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2024-04-26 06:22:56.000000 advanced_input-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 06:38:12.518121 advanced_input-0.1.3/advanced_input/
--rw-rw-rw-   0        0        0      415 2024-04-26 06:35:29.000000 advanced_input-0.1.3/advanced_input/__init__.py
--rw-rw-rw-   0        0        0      316 2024-04-25 10:42:38.000000 advanced_input-0.1.3/advanced_input/constants.py
--rw-rw-rw-   0        0        0     2914 2024-04-30 06:19:39.000000 advanced_input-0.1.3/advanced_input/input.py
--rw-rw-rw-   0        0        0   107088 2024-04-30 06:20:02.000000 advanced_input-0.1.3/advanced_input/inputExtention.dll
-drwxrwxrwx   0        0        0        0 2024-04-30 06:38:12.529774 advanced_input-0.1.3/advanced_input.egg-info/
--rw-rw-rw-   0        0        0     1691 2024-04-30 06:38:12.000000 advanced_input-0.1.3/advanced_input.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-04-30 06:38:12.000000 advanced_input-0.1.3/advanced_input.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 06:38:12.000000 advanced_input-0.1.3/advanced_input.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-30 06:38:12.000000 advanced_input-0.1.3/advanced_input.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-12-08 11:06:28.000000 advanced_input-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      661 2024-04-30 06:38:12.564142 advanced_input-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 07:24:48.874633 advanced_input-0.2.0/
+-rw-rw-rw-   0        0        0     1235 2020-07-21 09:29:29.000000 advanced_input-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1685 2024-05-01 07:24:48.873631 advanced_input-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2024-04-26 06:22:56.000000 advanced_input-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 07:24:48.859021 advanced_input-0.2.0/advanced_input/
+-rw-rw-rw-   0        0        0      564 2024-05-01 07:02:14.000000 advanced_input-0.2.0/advanced_input/__init__.py
+-rw-rw-rw-   0        0        0      316 2024-04-25 10:42:38.000000 advanced_input-0.2.0/advanced_input/constants.py
+-rw-rw-rw-   0        0        0     3168 2024-05-01 07:18:53.000000 advanced_input-0.2.0/advanced_input/input.py
+-rw-rw-rw-   0        0        0     1245 2024-05-01 07:19:39.000000 advanced_input-0.2.0/advanced_input/inputExtention.c
+-rw-rw-rw-   0        0        0   107263 2024-05-01 07:19:44.000000 advanced_input-0.2.0/advanced_input/inputExtention.dll
+-rw-rw-rw-   0        0        0    16096 2024-05-01 07:22:41.000000 advanced_input-0.2.0/advanced_input/inputExtention.so
+drwxrwxrwx   0        0        0        0 2024-05-01 07:24:48.873631 advanced_input-0.2.0/advanced_input.egg-info/
+-rw-rw-rw-   0        0        0     1685 2024-05-01 07:24:48.000000 advanced_input-0.2.0/advanced_input.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-05-01 07:24:48.000000 advanced_input-0.2.0/advanced_input.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 07:24:48.000000 advanced_input-0.2.0/advanced_input.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-01 07:24:48.000000 advanced_input-0.2.0/advanced_input.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-12-08 11:06:28.000000 advanced_input-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      653 2024-05-01 07:24:48.875629 advanced_input-0.2.0/setup.cfg
```

### Comparing `advanced_input-0.1.3/LICENSE` & `advanced_input-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `advanced_input-0.1.3/PKG-INFO` & `advanced_input-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: advanced_input
-Version: 0.1.3
+Version: 0.2.0
 Summary: IO Extention
 Home-page: https://github.com/NightKey/advanced-input
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/advanced-input/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freeware
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Advanced Input
 
 Advanced input for python, where you can read in just one character or have inputs priority ordered.
```

### Comparing `advanced_input-0.1.3/README.md` & `advanced_input-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `advanced_input-0.1.3/advanced_input/input.py` & `advanced_input-0.2.0/advanced_input/input.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sys import stdin
+from sys import stdin, stdout
 from threading import Event, Thread
 from typing import Dict, List
 from .constants import PriorityOrder, EventWithType, EventType
 from time import sleep
 from os import path
 from platform import system
 import ctypes
@@ -10,34 +10,41 @@
 modul_name = "inputExtention" if system() == "Windows" else "inputExtention.so"
 inputExtention = ctypes.CDLL(path.join(path.dirname(__file__), modul_name))
 inputExtentionInit = inputExtention.init
 inputExtentionStop = inputExtention.stop
 is_input_ready = inputExtention.isInputReady
 is_input_ready.restype = ctypes.c_bool
 get_character_from_input = inputExtention.getCharacter
-get_character_from_input.restype = ctypes.c_char
+get_character_from_input.restype = ctypes.c_uint
 
 class AdvancedInput():
-    def __init__(self) -> None:
+    def __init__(self, encoding: str) -> None:
         self.last_input: str = ""
         self.order: Dict[PriorityOrder, List[EventWithType]] = {PriorityOrder.Low: [], PriorityOrder.Normal: [], PriorityOrder.High: []}
         self.stop_event = Event()
         self.main_thread: Thread = None
+        self.encoding = encoding
         inputExtentionInit()
 
     def __loop(self) -> None:
         while not self.stop_event.is_set():
+            counter = 0
             while not is_input_ready() and not self.stop_event.is_set():
+                counter += 1
+                if counter >= 5:
+                    stdout.flush()
+                    counter = 0
                 self.stop_event.wait(.1)
             if self.stop_event.is_set(): break
-            self.last_input = get_character_from_input().decode('cp850') #TODO: When C code is OS independent, make sure to cover this as well
+            tmp: int = get_character_from_input()
+            self.last_input: str = tmp.to_bytes(4, "little").decode(self.encoding).strip("\x00")
             for priority in reversed(PriorityOrder):
                 if (len(self.order[priority]) > 0):
                     currentEvent = self.order[priority].pop()
-                    if currentEvent.type == EventType.LINE:
+                    if currentEvent.type == EventType.LINE and self.last_input not in ["\n"]:
                         self.last_input += stdin.readline().rstrip()
                     currentEvent.set()
                     break
 
     def start(self) -> None:
         self.stop_event.clear()
         self.main_thread = Thread(target=self.__loop)
```

### Comparing `advanced_input-0.1.3/advanced_input/inputExtention.dll` & `advanced_input-0.2.0/advanced_input/inputExtention.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 06:20:02 2024
+Time/Date		Wed May  1 07:19:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	41
 SizeOfCode		0000000000001600
 SizeOfInitializedData	0000000000003800
 SizeOfUninitializedData	0000000000000200
 AddressOfEntryPoint	0000000000001330
@@ -26,156 +26,157 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00021000
 SizeOfHeaders		00000600
-CheckSum		00027ab7
+CheckSum		00021edf
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
 NumberOfRvaAndSizes	00000010
 
 The Data Directory
 Entry 0 0000000000008000 00000087 Export Directory [.edata (or where ever we found it)]
-Entry 1 0000000000009000 00000854 Import Directory [parts of .idata]
+Entry 1 0000000000009000 00000870 Import Directory [parts of .idata]
 Entry 2 0000000000000000 00000000 Resource Directory [.rsrc]
 Entry 3 0000000000005000 00000240 Exception Directory [.pdata]
 Entry 4 0000000000000000 00000000 Security Directory
 Entry 5 000000000000c000 00000078 Base Relocation Directory [.reloc]
 Entry 6 0000000000000000 00000000 Debug Directory
 Entry 7 0000000000000000 00000000 Description Directory
 Entry 8 0000000000000000 00000000 Special Directory
 Entry 9 0000000000004020 00000028 Thread Storage Directory [.tls]
 Entry a 0000000000000000 00000000 Load Configuration Directory
 Entry b 0000000000000000 00000000 Bound Import Directory
-Entry c 0000000000009248 00000190 Import Address Table Directory
+Entry c 0000000000009250 00000198 Import Address Table Directory
 Entry d 0000000000000000 00000000 Delay Import Directory
 Entry e 0000000000000000 00000000 CLR Runtime Header
 Entry f 0000000000000000 00000000 Reserved
 
 There is an import table in .idata at 0x29a1b9000
 
 The Import Tables (interpreted .idata section contents)
  vma:            Hint    Time      Forward  DLL       First
                  Table   Stamp     Chain    Name      Thunk
- 00009000	000090b8 00000000 00000000 000096d0 00009248
+ 00009000	000090b8 00000000 00000000 000096e8 00009250
 
 	DLL Name: KERNEL32.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	93d8	  293  DeleteCriticalSection
-	93f0	  331  EnterCriticalSection
-	9408	  644  GetLastError
-	9418	  914  InitializeCriticalSection
-	9434	 1008  LeaveCriticalSection
-	944c	 1444  Sleep
-	9454	 1480  TlsGetValue
-	9462	 1527  VirtualProtect
-	9474	 1529  VirtualQuery
+	93e8	  293  DeleteCriticalSection
+	9400	  331  EnterCriticalSection
+	9418	  644  GetLastError
+	9428	  914  InitializeCriticalSection
+	9444	 1008  LeaveCriticalSection
+	945c	 1444  Sleep
+	9464	 1480  TlsGetValue
+	9472	 1527  VirtualProtect
+	9484	 1529  VirtualQuery
 
- 00009014	00009108 00000000 00000000 000096e4 00009298
+ 00009014	00009108 00000000 00000000 000096fc 000092a0
 
 	DLL Name: api-ms-win-crt-conio-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	9484	   15  _getch
+	9494	   15  _getch
 
- 00009028	00009118 00000000 00000000 0000970c 000092a8
+ 00009028	00009118 00000000 00000000 00009724 000092b0
 
 	DLL Name: api-ms-win-crt-environment-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	948e	    1  __p__environ
-	949e	    2  __p__wenviron
+	949e	    1  __p__environ
+	94ae	    2  __p__wenviron
 
- 0000903c	00009130 00000000 00000000 00009740 000092c0
+ 0000903c	00009130 00000000 00000000 00009758 000092c8
 
 	DLL Name: api-ms-win-crt-heap-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	94ae	   24  _set_new_mode
-	94be	   25  calloc
-	94c8	   26  free
+	94be	   24  _set_new_mode
+	94ce	   25  calloc
+	94d8	   26  free
 
- 00009050	00009150 00000000 00000000 0000979c 000092e0
+ 00009050	00009150 00000000 00000000 000097b4 000092e8
 
 	DLL Name: api-ms-win-crt-runtime-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	94d0	    5  __p___argc
-	94de	    6  __p___argv
-	94ec	    7  __p___wargv
-	94fa	   25  _configure_narrow_argv
-	9514	   26  _configure_wide_argv
-	952c	   30  _crt_at_quick_exit
-	9542	   31  _crt_atexit
-	9550	   36  _execute_onexit_table
-	9568	   37  _exit
-	9570	   54  _initialize_narrow_environment
-	9592	   55  _initialize_onexit_table
-	95ae	   56  _initialize_wide_environment
-	95ce	   57  _initterm
-	95da	   63  _register_onexit_function
-	95f6	   88  abort
+	94e0	    5  __p___argc
+	94ee	    6  __p___argv
+	94fc	    7  __p___wargv
+	950a	   25  _configure_narrow_argv
+	9524	   26  _configure_wide_argv
+	953c	   30  _crt_at_quick_exit
+	9552	   31  _crt_atexit
+	9560	   36  _execute_onexit_table
+	9578	   37  _exit
+	9580	   54  _initialize_narrow_environment
+	95a2	   55  _initialize_onexit_table
+	95be	   56  _initialize_wide_environment
+	95de	   57  _initterm
+	95ea	   63  _register_onexit_function
+	9606	   88  abort
 
- 00009064	000091d0 00000000 00000000 000097d8 00009360
+ 00009064	000091d0 00000000 00000000 000097f4 00009368
 
 	DLL Name: api-ms-win-crt-stdio-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	95fe	    1  __acrt_iob_func
-	9610	    4  __stdio_common_vfprintf
-	962a	    8  __stdio_common_vfwprintf
-	9646	   84  _kbhit
-	9650	  169  fwrite
-	965a	  177  putchar
+	960e	    1  __acrt_iob_func
+	9620	    4  __stdio_common_vfprintf
+	963a	    8  __stdio_common_vfwprintf
+	9656	   84  _kbhit
+	9660	  150  fflush
+	966a	  169  fwrite
+	9674	  177  putchar
 
- 00009078	00009208 00000000 00000000 00009800 00009398
+ 00009078	00009210 00000000 00000000 0000981c 000093a8
 
 	DLL Name: api-ms-win-crt-string-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	9664	  168  strlen
-	966e	  171  strncmp
+	967e	  168  strlen
+	9688	  171  strncmp
 
- 0000908c	00009220 00000000 00000000 00009834 000093b0
+ 0000908c	00009228 00000000 00000000 00009850 000093c0
 
 	DLL Name: api-ms-win-crt-time-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	9678	    9  __daylight
-	9686	   11  __timezone
-	9694	   12  __tzname
-	96a0	   60  _tzset
+	9692	    9  __daylight
+	96a0	   11  __timezone
+	96ae	   12  __tzname
+	96ba	   60  _tzset
 
  000090a0	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x29a1b8000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		66308d92
+Time/Date stamp 		6631ed10
 Major/Minor 			0/0
 Name 				0000000000008050 inputExtention.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000004
 	[Name Pointer/Ordinal] Table	00000004
 Table Addresses
 	Export Address Table 		0000000000008028
 	Name Pointer Table 		0000000000008038
 	Ordinal Table 			0000000000008048
 
 Export Address Table -- Ordinal Base 1
-	[   0] +base[   1] 139a Export RVA
+	[   0] +base[   1] 13b8 Export RVA
 	[   1] +base[   2] 1380 Export RVA
-	[   2] +base[   3] 1387 Export RVA
-	[   3] +base[   4] 13bf Export RVA
+	[   2] +base[   3] 13a5 Export RVA
+	[   3] +base[   4] 13ec Export RVA
 
 [Ordinal/Name Pointer] Table
 	[   0] getCharacter
 	[   1] init
 	[   2] isInputReady
 	[   3] stop
 
@@ -184,55 +185,55 @@
  000000029a1b5000:	000000029a1b1000 000000029a1b100c 000000029a1b6000
  000000029a1b500c:	000000029a1b1010 000000029a1b11cf 000000029a1b6004
  000000029a1b5018:	000000029a1b11d0 000000029a1b1324 000000029a1b6018
  000000029a1b5024:	000000029a1b1330 000000029a1b1342 000000029a1b6028
  000000029a1b5030:	000000029a1b1350 000000029a1b135f 000000029a1b602c
  000000029a1b503c:	000000029a1b1360 000000029a1b136c 000000029a1b6030
  000000029a1b5048:	000000029a1b1370 000000029a1b1371 000000029a1b6034
- 000000029a1b5054:	000000029a1b1380 000000029a1b1387 000000029a1b6038
- 000000029a1b5060:	000000029a1b1387 000000029a1b139a 000000029a1b6040
- 000000029a1b506c:	000000029a1b139a 000000029a1b13bf 000000029a1b604c
- 000000029a1b5078:	000000029a1b13bf 000000029a1b13c6 000000029a1b6058
- 000000029a1b5084:	000000029a1b13d0 000000029a1b140a 000000029a1b6060
- 000000029a1b5090:	000000029a1b1410 000000029a1b147a 000000029a1b6068
- 000000029a1b509c:	000000029a1b1480 000000029a1b149f 000000029a1b6074
- 000000029a1b50a8:	000000029a1b14a0 000000029a1b14cf 000000029a1b6078
- 000000029a1b50b4:	000000029a1b14d0 000000029a1b1551 000000029a1b6080
- 000000029a1b50c0:	000000029a1b1560 000000029a1b1563 000000029a1b608c
- 000000029a1b50cc:	000000029a1b1570 000000029a1b15d9 000000029a1b6090
- 000000029a1b50d8:	000000029a1b15e0 000000029a1b1742 000000029a1b609c
- 000000029a1b50e4:	000000029a1b1750 000000029a1b1aad 000000029a1b60a8
- 000000029a1b50f0:	000000029a1b1ab0 000000029a1b1b20 000000029a1b60c0
- 000000029a1b50fc:	000000029a1b1b20 000000029a1b1b8f 000000029a1b60d0
- 000000029a1b5108:	000000029a1b1b90 000000029a1b1c11 000000029a1b60dc
- 000000029a1b5114:	000000029a1b1c20 000000029a1b1d12 000000029a1b60e8
- 000000029a1b5120:	000000029a1b1d20 000000029a1b1d4c 000000029a1b60f0
- 000000029a1b512c:	000000029a1b1d50 000000029a1b1da0 000000029a1b60f4
- 000000029a1b5138:	000000029a1b1da0 000000029a1b1e3d 000000029a1b60f8
- 000000029a1b5144:	000000029a1b1e40 000000029a1b1ec0 000000029a1b6104
- 000000029a1b5150:	000000029a1b1ec0 000000029a1b1ef7 000000029a1b6108
- 000000029a1b515c:	000000029a1b1f00 000000029a1b1f73 000000029a1b610c
- 000000029a1b5168:	000000029a1b1f80 000000029a1b1fb6 000000029a1b6110
- 000000029a1b5174:	000000029a1b1fc0 000000029a1b2049 000000029a1b6114
- 000000029a1b5180:	000000029a1b2050 000000029a1b2116 000000029a1b6118
- 000000029a1b518c:	000000029a1b2120 000000029a1b2123 000000029a1b611c
- 000000029a1b5198:	000000029a1b2170 000000029a1b2176 000000029a1b6120
- 000000029a1b51a4:	000000029a1b2180 000000029a1b2186 000000029a1b6124
- 000000029a1b51b0:	000000029a1b2190 000000029a1b21ae 000000029a1b6128
- 000000029a1b51bc:	000000029a1b21b0 000000029a1b21b3 000000029a1b6130
- 000000029a1b51c8:	000000029a1b21c0 000000029a1b222a 000000029a1b6134
- 000000029a1b51d4:	000000029a1b2230 000000029a1b229a 000000029a1b6144
- 000000029a1b51e0:	000000029a1b22a0 000000029a1b22be 000000029a1b6154
- 000000029a1b51ec:	000000029a1b22c0 000000029a1b22d5 000000029a1b615c
- 000000029a1b51f8:	000000029a1b22e0 000000029a1b230e 000000029a1b6160
- 000000029a1b5204:	000000029a1b2310 000000029a1b2345 000000029a1b6168
- 000000029a1b5210:	000000029a1b2350 000000029a1b2386 000000029a1b6170
- 000000029a1b521c:	000000029a1b2390 000000029a1b23c6 000000029a1b6178
- 000000029a1b5228:	000000029a1b24f0 000000029a1b2522 000000029a1b6180
- 000000029a1b5234:	000000029a1b2580 000000029a1b2585 000000029a1b6188
+ 000000029a1b5054:	000000029a1b1380 000000029a1b13a5 000000029a1b6038
+ 000000029a1b5060:	000000029a1b13a5 000000029a1b13b8 000000029a1b6044
+ 000000029a1b506c:	000000029a1b13b8 000000029a1b13ec 000000029a1b6050
+ 000000029a1b5078:	000000029a1b13ec 000000029a1b13f3 000000029a1b605c
+ 000000029a1b5084:	000000029a1b1400 000000029a1b143a 000000029a1b6064
+ 000000029a1b5090:	000000029a1b1440 000000029a1b14aa 000000029a1b606c
+ 000000029a1b509c:	000000029a1b14b0 000000029a1b14cf 000000029a1b6078
+ 000000029a1b50a8:	000000029a1b14d0 000000029a1b14ff 000000029a1b607c
+ 000000029a1b50b4:	000000029a1b1500 000000029a1b1581 000000029a1b6084
+ 000000029a1b50c0:	000000029a1b1590 000000029a1b1593 000000029a1b6090
+ 000000029a1b50cc:	000000029a1b15a0 000000029a1b1609 000000029a1b6094
+ 000000029a1b50d8:	000000029a1b1610 000000029a1b1772 000000029a1b60a0
+ 000000029a1b50e4:	000000029a1b1780 000000029a1b1add 000000029a1b60ac
+ 000000029a1b50f0:	000000029a1b1ae0 000000029a1b1b50 000000029a1b60c4
+ 000000029a1b50fc:	000000029a1b1b50 000000029a1b1bbf 000000029a1b60d4
+ 000000029a1b5108:	000000029a1b1bc0 000000029a1b1c41 000000029a1b60e0
+ 000000029a1b5114:	000000029a1b1c50 000000029a1b1d42 000000029a1b60ec
+ 000000029a1b5120:	000000029a1b1d50 000000029a1b1d7c 000000029a1b60f4
+ 000000029a1b512c:	000000029a1b1d80 000000029a1b1dd0 000000029a1b60f8
+ 000000029a1b5138:	000000029a1b1dd0 000000029a1b1e6d 000000029a1b60fc
+ 000000029a1b5144:	000000029a1b1e70 000000029a1b1ef0 000000029a1b6108
+ 000000029a1b5150:	000000029a1b1ef0 000000029a1b1f27 000000029a1b610c
+ 000000029a1b515c:	000000029a1b1f30 000000029a1b1fa3 000000029a1b6110
+ 000000029a1b5168:	000000029a1b1fb0 000000029a1b1fe6 000000029a1b6114
+ 000000029a1b5174:	000000029a1b1ff0 000000029a1b2079 000000029a1b6118
+ 000000029a1b5180:	000000029a1b2080 000000029a1b2146 000000029a1b611c
+ 000000029a1b518c:	000000029a1b2150 000000029a1b2153 000000029a1b6120
+ 000000029a1b5198:	000000029a1b21a0 000000029a1b21a6 000000029a1b6124
+ 000000029a1b51a4:	000000029a1b21b0 000000029a1b21b6 000000029a1b6128
+ 000000029a1b51b0:	000000029a1b21c0 000000029a1b21de 000000029a1b612c
+ 000000029a1b51bc:	000000029a1b21e0 000000029a1b21e3 000000029a1b6134
+ 000000029a1b51c8:	000000029a1b21f0 000000029a1b225a 000000029a1b6138
+ 000000029a1b51d4:	000000029a1b2260 000000029a1b22ca 000000029a1b6148
+ 000000029a1b51e0:	000000029a1b22d0 000000029a1b22ee 000000029a1b6158
+ 000000029a1b51ec:	000000029a1b22f0 000000029a1b2305 000000029a1b6160
+ 000000029a1b51f8:	000000029a1b2310 000000029a1b233e 000000029a1b6164
+ 000000029a1b5204:	000000029a1b2340 000000029a1b2375 000000029a1b616c
+ 000000029a1b5210:	000000029a1b2380 000000029a1b23b6 000000029a1b6174
+ 000000029a1b521c:	000000029a1b23c0 000000029a1b23f6 000000029a1b617c
+ 000000029a1b5228:	000000029a1b2530 000000029a1b2562 000000029a1b6184
+ 000000029a1b5234:	000000029a1b25c0 000000029a1b25c5 000000029a1b618c
 
 Dump of .xdata
  000000029a1b6000 (rva: 00006000): 000000029a1b1000 - 000000029a1b100c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  000000029a1b6004 (rva: 00006004): 000000029a1b1010 - 000000029a1b11cf
 	Version: 1, Flags: none
@@ -261,218 +262,219 @@
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  000000029a1b6030 (rva: 00006030): 000000029a1b1360 - 000000029a1b136c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  000000029a1b6034 (rva: 00006034): 000000029a1b1370 - 000000029a1b1371
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6038 (rva: 00006038): 000000029a1b1380 - 000000029a1b1387
+ 000000029a1b6038 (rva: 00006038): 000000029a1b1380 - 000000029a1b13a5
 	Version: 1, Flags: none
-	Nbr codes: 2, Prologue size: 0x04, Frame offset: 0x0, Frame reg: rbp
+	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
+	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 000000029a1b6040 (rva: 00006040): 000000029a1b1387 - 000000029a1b139a
+ 000000029a1b6044 (rva: 00006044): 000000029a1b13a5 - 000000029a1b13b8
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 000000029a1b604c (rva: 0000604c): 000000029a1b139a - 000000029a1b13bf
+ 000000029a1b6050 (rva: 00006050): 000000029a1b13b8 - 000000029a1b13ec
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 000000029a1b6058 (rva: 00006058): 000000029a1b13bf - 000000029a1b13c6
+ 000000029a1b605c (rva: 0000605c): 000000029a1b13ec - 000000029a1b13f3
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x04, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 000000029a1b6060 (rva: 00006060): 000000029a1b13d0 - 000000029a1b140a
+ 000000029a1b6064 (rva: 00006064): 000000029a1b1400 - 000000029a1b143a
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000029a1b6068 (rva: 00006068): 000000029a1b1410 - 000000029a1b147a
+ 000000029a1b606c (rva: 0000606c): 000000029a1b1440 - 000000029a1b14aa
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 000000029a1b6074 (rva: 00006074): 000000029a1b1480 - 000000029a1b149f
+ 000000029a1b6078 (rva: 00006078): 000000029a1b14b0 - 000000029a1b14cf
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6078 (rva: 00006078): 000000029a1b14a0 - 000000029a1b14cf
+ 000000029a1b607c (rva: 0000607c): 000000029a1b14d0 - 000000029a1b14ff
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000029a1b6080 (rva: 00006080): 000000029a1b14d0 - 000000029a1b1551
+ 000000029a1b6084 (rva: 00006084): 000000029a1b1500 - 000000029a1b1581
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 000000029a1b608c (rva: 0000608c): 000000029a1b1560 - 000000029a1b1563
+ 000000029a1b6090 (rva: 00006090): 000000029a1b1590 - 000000029a1b1593
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6090 (rva: 00006090): 000000029a1b1570 - 000000029a1b15d9
+ 000000029a1b6094 (rva: 00006094): 000000029a1b15a0 - 000000029a1b1609
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 000000029a1b609c (rva: 0000609c): 000000029a1b15e0 - 000000029a1b1742
+ 000000029a1b60a0 (rva: 000060a0): 000000029a1b1610 - 000000029a1b1772
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x50
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 000000029a1b60a8 (rva: 000060a8): 000000029a1b1750 - 000000029a1b1aad
+ 000000029a1b60ac (rva: 000060ac): 000000029a1b1780 - 000000029a1b1add
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x15, Frame offset: 0x4, Frame reg: rbp
 	  pc+0x15: FPReg: rbp = rsp + 0x40 (info = 0x0)
 	  pc+0x10: alloc small area: rsp = rsp - 0x48
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push r12
 	  pc+0x07: push r13
 	  pc+0x05: push r14
 	  pc+0x03: push r15
 	  pc+0x01: push rbp
- 000000029a1b60c0 (rva: 000060c0): 000000029a1b1ab0 - 000000029a1b1b20
+ 000000029a1b60c4 (rva: 000060c4): 000000029a1b1ae0 - 000000029a1b1b50
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 000000029a1b60d0 (rva: 000060d0): 000000029a1b1b20 - 000000029a1b1b8f
+ 000000029a1b60d4 (rva: 000060d4): 000000029a1b1b50 - 000000029a1b1bbf
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 000000029a1b60dc (rva: 000060dc): 000000029a1b1b90 - 000000029a1b1c11
+ 000000029a1b60e0 (rva: 000060e0): 000000029a1b1bc0 - 000000029a1b1c41
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 000000029a1b60e8 (rva: 000060e8): 000000029a1b1c20 - 000000029a1b1d12
+ 000000029a1b60ec (rva: 000060ec): 000000029a1b1c50 - 000000029a1b1d42
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 000000029a1b60f0 (rva: 000060f0): 000000029a1b1d20 - 000000029a1b1d4c
+ 000000029a1b60f4 (rva: 000060f4): 000000029a1b1d50 - 000000029a1b1d7c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b60f4 (rva: 000060f4): 000000029a1b1d50 - 000000029a1b1da0
+ 000000029a1b60f8 (rva: 000060f8): 000000029a1b1d80 - 000000029a1b1dd0
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b60f8 (rva: 000060f8): 000000029a1b1da0 - 000000029a1b1e3d
+ 000000029a1b60fc (rva: 000060fc): 000000029a1b1dd0 - 000000029a1b1e6d
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 000000029a1b6104 (rva: 00006104): 000000029a1b1e40 - 000000029a1b1ec0
+ 000000029a1b6108 (rva: 00006108): 000000029a1b1e70 - 000000029a1b1ef0
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6108 (rva: 00006108): 000000029a1b1ec0 - 000000029a1b1ef7
+ 000000029a1b610c (rva: 0000610c): 000000029a1b1ef0 - 000000029a1b1f27
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b610c (rva: 0000610c): 000000029a1b1f00 - 000000029a1b1f73
+ 000000029a1b6110 (rva: 00006110): 000000029a1b1f30 - 000000029a1b1fa3
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6110 (rva: 00006110): 000000029a1b1f80 - 000000029a1b1fb6
+ 000000029a1b6114 (rva: 00006114): 000000029a1b1fb0 - 000000029a1b1fe6
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6114 (rva: 00006114): 000000029a1b1fc0 - 000000029a1b2049
+ 000000029a1b6118 (rva: 00006118): 000000029a1b1ff0 - 000000029a1b2079
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6118 (rva: 00006118): 000000029a1b2050 - 000000029a1b2116
+ 000000029a1b611c (rva: 0000611c): 000000029a1b2080 - 000000029a1b2146
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b611c (rva: 0000611c): 000000029a1b2120 - 000000029a1b2123
+ 000000029a1b6120 (rva: 00006120): 000000029a1b2150 - 000000029a1b2153
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6120 (rva: 00006120): 000000029a1b2170 - 000000029a1b2176
+ 000000029a1b6124 (rva: 00006124): 000000029a1b21a0 - 000000029a1b21a6
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6124 (rva: 00006124): 000000029a1b2180 - 000000029a1b2186
+ 000000029a1b6128 (rva: 00006128): 000000029a1b21b0 - 000000029a1b21b6
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6128 (rva: 00006128): 000000029a1b2190 - 000000029a1b21ae
+ 000000029a1b612c (rva: 0000612c): 000000029a1b21c0 - 000000029a1b21de
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x38
- 000000029a1b6130 (rva: 00006130): 000000029a1b21b0 - 000000029a1b21b3
+ 000000029a1b6134 (rva: 00006134): 000000029a1b21e0 - 000000029a1b21e3
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6134 (rva: 00006134): 000000029a1b21c0 - 000000029a1b222a
+ 000000029a1b6138 (rva: 00006138): 000000029a1b21f0 - 000000029a1b225a
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 000000029a1b6144 (rva: 00006144): 000000029a1b2230 - 000000029a1b229a
+ 000000029a1b6148 (rva: 00006148): 000000029a1b2260 - 000000029a1b22ca
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 000000029a1b6154 (rva: 00006154): 000000029a1b22a0 - 000000029a1b22be
+ 000000029a1b6158 (rva: 00006158): 000000029a1b22d0 - 000000029a1b22ee
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 000000029a1b615c (rva: 0000615c): 000000029a1b22c0 - 000000029a1b22d5
+ 000000029a1b6160 (rva: 00006160): 000000029a1b22f0 - 000000029a1b2305
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6160 (rva: 00006160): 000000029a1b22e0 - 000000029a1b230e
+ 000000029a1b6164 (rva: 00006164): 000000029a1b2310 - 000000029a1b233e
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 000000029a1b6168 (rva: 00006168): 000000029a1b2310 - 000000029a1b2345
+ 000000029a1b616c (rva: 0000616c): 000000029a1b2340 - 000000029a1b2375
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x48
- 000000029a1b6170 (rva: 00006170): 000000029a1b2350 - 000000029a1b2386
+ 000000029a1b6174 (rva: 00006174): 000000029a1b2380 - 000000029a1b23b6
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000029a1b6178 (rva: 00006178): 000000029a1b2390 - 000000029a1b23c6
+ 000000029a1b617c (rva: 0000617c): 000000029a1b23c0 - 000000029a1b23f6
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000029a1b6180 (rva: 00006180): 000000029a1b24f0 - 000000029a1b2522
+ 000000029a1b6184 (rva: 00006184): 000000029a1b2530 - 000000029a1b2562
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x48
- 000000029a1b6188 (rva: 00006188): 000000029a1b2580 - 000000029a1b2585
+ 000000029a1b618c (rva: 0000618c): 000000029a1b25c0 - 000000029a1b25c5
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 
 
 PE File Base Relocations (interpreted .reloc section contents)
 
 Virtual Address: 00002000 Chunk size 12 (0xc) Number of fixups 2
-	reloc    0 offset  598 [2598] DIR64
+	reloc    0 offset  5d8 [25d8] DIR64
 	reloc    1 offset    0 [2000] ABSOLUTE
 
 Virtual Address: 00003000 Chunk size 40 (0x28) Number of fixups 16
 	reloc    0 offset   10 [3010] DIR64
 	reloc    1 offset   40 [3040] DIR64
 	reloc    2 offset   50 [3050] DIR64
 	reloc    3 offset   58 [3058] DIR64
@@ -517,29 +519,29 @@
 	reloc    0 offset   18 [a018] DIR64
 	reloc    1 offset   30 [a030] DIR64
 	reloc    2 offset   38 [a038] DIR64
 	reloc    3 offset    0 [a000] ABSOLUTE
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
-  0 .text         000015b8  000000029a1b1000  000000029a1b1000  00000600  2**4
+  0 .text         000015f8  000000029a1b1000  000000029a1b1000  00000600  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE, DATA
   1 .data         000000e0  000000029a1b3000  000000029a1b3000  00001c00  2**4
                   CONTENTS, ALLOC, LOAD, DATA
   2 .rdata        000006d0  000000029a1b4000  000000029a1b4000  00001e00  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   3 .pdata        00000240  000000029a1b5000  000000029a1b5000  00002600  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  4 .xdata        0000018c  000000029a1b6000  000000029a1b6000  00002a00  2**2
+  4 .xdata        00000190  000000029a1b6000  000000029a1b6000  00002a00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   5 .bss          00000110  000000029a1b7000  000000029a1b7000  00000000  2**4
                   ALLOC
   6 .edata        00000087  000000029a1b8000  000000029a1b8000  00002c00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  7 .idata        00000854  000000029a1b9000  000000029a1b9000  00002e00  2**2
+  7 .idata        00000870  000000029a1b9000  000000029a1b9000  00002e00  2**2
                   CONTENTS, ALLOC, LOAD, DATA
   8 .CRT          00000058  000000029a1ba000  000000029a1ba000  00003800  2**2
                   CONTENTS, ALLOC, LOAD, DATA
   9 .tls          00000010  000000029a1bb000  000000029a1bb000  00003a00  2**2
                   CONTENTS, ALLOC, LOAD, DATA
  10 .reloc        00000078  000000029a1bc000  000000029a1bc000  00003c00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
@@ -639,46 +641,46 @@
 AUX scnlen 0x18 nreloc 6 nlnno 0
 [ 75](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000310 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [ 77](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000060 inputExtention
 File 
 [ 79](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000000380 init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[ 81](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000387 isInputReady
-[ 82](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000039a getCharacter
-[ 83](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000003bf stop
+[ 81](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000003a5 isInputReady
+[ 82](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000003b8 getCharacter
+[ 83](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000003ec stop
 [ 84](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000380 .text
-AUX scnlen 0x46 nreloc 3 nlnno 0
+AUX scnlen 0x73 nreloc 5 nlnno 0
 [ 86](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [ 88](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [ 90](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000038 .xdata
-AUX scnlen 0x28 nreloc 0 nlnno 0
+AUX scnlen 0x2c nreloc 0 nlnno 0
 [ 92](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000054 .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
 [ 94](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000340 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [ 96](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000084 gccmain.c
 File 
-[ 98](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000003d0 __do_global_dtors
+[ 98](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000000400 __do_global_dtors
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [100](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000010 p.0
-[101](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000410 __do_global_ctors
+[101](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000440 __do_global_ctors
 [102](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001f0 .rdata$.refptr.__CTOR_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[104](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000480 __main
+[104](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000004b0 __main
 [105](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000020 initialized
-[106](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003d0 .text
+[106](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000400 .text
 AUX scnlen 0xcf nreloc 7 nlnno 0
 [108](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [110](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[112](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000060 .xdata
+[112](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000064 .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
 [114](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000084 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [116](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000019b4 .debug_info
 AUX scnlen 0x661 nreloc 17 nlnno 0
 [118](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004bf .debug_abbrev
 AUX scnlen 0x13f nreloc 0 nlnno 0
@@ -692,15 +694,15 @@
 AUX scnlen 0xe8 nreloc 0 nlnno 0
 [128](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000370 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [130](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000108 .debug_frame
 AUX scnlen 0x88 nreloc 6 nlnno 0
 [132](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000009a natstart.c
 File 
-[134](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004a0 .text
+[134](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [136](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [138](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .bss
 AUX scnlen 0xc nreloc 0 nlnno 0
 [140](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002015 .debug_info
 AUX scnlen 0x602 nreloc 10 nlnno 0
@@ -714,29 +716,29 @@
 AUX scnlen 0x18 nreloc 0 nlnno 0
 [150](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000272 .debug_line_str
 AUX scnlen 0x10e nreloc 0 nlnno 0
 [152](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [154](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000d2 tlssup.c
 File 
-[156](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000004a0 __dyn_tls_dtor
+[156](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000004d0 __dyn_tls_dtor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[158](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000004d0 __dyn_tls_init
+[158](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000500 __dyn_tls_init
 [159](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001e0 .rdata$.refptr._CRT_MT
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [161](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000048 __xd_a
 [162](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 __xd_z
-[163](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000560 __tlregdtor
-[164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004a0 .text
+[163](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000590 __tlregdtor
+[164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d0 .text
 AUX scnlen 0xc3 nreloc 5 nlnno 0
 [166](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [168](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[170](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000078 .xdata
+[170](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000007c .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
 [172](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000a8 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [174](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000038 .CRT$XLD
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [176](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .CRT$XLC
 AUX scnlen 0x8 nreloc 1 nlnno 0
@@ -770,15 +772,15 @@
 AUX scnlen 0xee nreloc 0 nlnno 0
 [206](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003d0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [208](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000190 .debug_frame
 AUX scnlen 0xa8 nreloc 6 nlnno 0
 [210](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000ee cinitexe.c
 File 
-[212](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000570 .text
+[212](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005a0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [214](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [216](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [218](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .CRT$XCZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
@@ -798,15 +800,15 @@
 AUX scnlen 0x3a nreloc 4 nlnno 0
 [234](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000046e .debug_line_str
 AUX scnlen 0x9f nreloc 0 nlnno 0
 [236](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000400 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [238](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000102 mingw_helpers.
 File 
-[240](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000570 .text
+[240](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005a0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [242](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [244](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [246](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002f59 .debug_info
 AUX scnlen 0x92 nreloc 5 nlnno 0
@@ -818,36 +820,36 @@
 AUX scnlen 0x3a nreloc 4 nlnno 0
 [254](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000050d .debug_line_str
 AUX scnlen 0xae nreloc 0 nlnno 0
 [256](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000430 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [258](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000131 pseudo-reloc.c
 File 
-[260](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000000570 __report_error
+[260](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000005a0 __report_error
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[262](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x00000000000005e0 mark_section_writable
+[262](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000000610 mark_section_writable
 [263](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000064 maxSections
 [264](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000068 the_secs
-[265](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000750 _pei386_runtime_relocator
+[265](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000780 _pei386_runtime_relocator
 [266](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000060 was_init.0
 [267](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000210 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [269](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000220 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [271](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000200 .rdata$.refptr.__ImageBase
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[273](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000570 .text
+[273](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005a0 .text
 AUX scnlen 0x53d nreloc 38 nlnno 0
 [275](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [277](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000060 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
 [279](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000060 .rdata
 AUX scnlen 0x15b nreloc 0 nlnno 0
-[281](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000090 .xdata
+[281](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000094 .xdata
 AUX scnlen 0x30 nreloc 0 nlnno 0
 [283](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000cc .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [285](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002feb .debug_info
 AUX scnlen 0x174b nreloc 165 nlnno 0
 [287](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000092a .debug_abbrev
 AUX scnlen 0x3d8 nreloc 0 nlnno 0
@@ -865,29 +867,29 @@
 AUX scnlen 0x14f nreloc 0 nlnno 0
 [301](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000460 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [303](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000238 .debug_frame
 AUX scnlen 0xe0 nreloc 6 nlnno 0
 [305](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000157 tlsthrd.c
 File 
-[307](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000000ab0 __mingwthr_run_key_dtors.part.0
+[307](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000000ae0 __mingwthr_run_key_dtors.part.0
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [309](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000a0 __mingwthr_cs
 [310](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 key_dtor_list
-[311](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000b20 ___w64_mingwthr_add_key_dtor
+[311](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000b50 ___w64_mingwthr_add_key_dtor
 [312](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000088 __mingwthr_cs_init
-[313](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000b90 ___w64_mingwthr_remove_key_dtor
-[314](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000c20 __mingw_TLScallback
-[315](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000ab0 .text
+[313](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000bc0 ___w64_mingwthr_remove_key_dtor
+[314](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000c50 __mingw_TLScallback
+[315](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000ae0 .text
 AUX scnlen 0x262 nreloc 34 nlnno 0
 [317](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [319](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .bss
 AUX scnlen 0x48 nreloc 0 nlnno 0
-[321](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000c0 .xdata
+[321](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000c4 .xdata
 AUX scnlen 0x30 nreloc 0 nlnno 0
 [323](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
 [325](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004736 .debug_info
 AUX scnlen 0xad3 nreloc 65 nlnno 0
 [327](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d02 .debug_abbrev
 AUX scnlen 0x261 nreloc 0 nlnno 0
@@ -903,15 +905,15 @@
 AUX scnlen 0x125 nreloc 0 nlnno 0
 [339](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000490 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [341](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000318 .debug_frame
 AUX scnlen 0x128 nreloc 8 nlnno 0
 [343](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000016b tlsmcrt.c
 File 
-[345](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d20 .text
+[345](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d50 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [347](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [349](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [351](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005209 .debug_info
 AUX scnlen 0x89 nreloc 5 nlnno 0
@@ -923,15 +925,15 @@
 AUX scnlen 0x3a nreloc 4 nlnno 0
 [359](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000082f .debug_line_str
 AUX scnlen 0x9c nreloc 0 nlnno 0
 [361](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [363](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000017f pseudo-reloc-list.c
 File 
-[365](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d20 .text
+[365](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d50 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [367](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [369](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .bss
 AUX scnlen 0x2 nreloc 0 nlnno 0
 [371](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005292 .debug_info
 AUX scnlen 0xd0 nreloc 6 nlnno 0
@@ -943,31 +945,31 @@
 AUX scnlen 0x3a nreloc 4 nlnno 0
 [379](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000008cb .debug_line_str
 AUX scnlen 0xba nreloc 0 nlnno 0
 [381](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004f0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [383](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001a9 pesect.c
 File 
-[385](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000000d20 _ValidateImageBase
+[385](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000000d50 _ValidateImageBase
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[387](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000d50 _FindPESection
-[388](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000da0 _FindPESectionByName
-[389](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000e40 __mingw_GetSectionForAddress
-[390](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000ec0 __mingw_GetSectionCount
-[391](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000f00 _FindPESectionExec
-[392](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000f80 _GetPEImageBase
-[393](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000fc0 _IsNonwritableInCurrentImage
-[394](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001050 __mingw_enum_import_library_names
-[395](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d20 .text
+[387](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000d80 _FindPESection
+[388](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000dd0 _FindPESectionByName
+[389](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000e70 __mingw_GetSectionForAddress
+[390](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000ef0 __mingw_GetSectionCount
+[391](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000f30 _FindPESectionExec
+[392](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000fb0 _GetPEImageBase
+[393](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000ff0 _IsNonwritableInCurrentImage
+[394](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001080 __mingw_enum_import_library_names
+[395](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d50 .text
 AUX scnlen 0x3f6 nreloc 9 nlnno 0
 [397](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [399](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[401](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .xdata
+[401](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f4 .xdata
 AUX scnlen 0x2c nreloc 0 nlnno 0
 [403](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000120 .pdata
 AUX scnlen 0x6c nreloc 27 nlnno 0
 [405](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005362 .debug_info
 AUX scnlen 0x14d2 nreloc 203 nlnno 0
 [407](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000fc1 .debug_abbrev
 AUX scnlen 0x28a nreloc 0 nlnno 0
@@ -985,24 +987,24 @@
 AUX scnlen 0xe5 nreloc 0 nlnno 0
 [421](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000520 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [423](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000440 .debug_frame
 AUX scnlen 0x128 nreloc 18 nlnno 0
 [425](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001d4 CRT_fp10.c
 File 
-[427](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001120 _fpreset
+[427](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001150 _fpreset
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[429](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001120 fpreset
-[430](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001120 .text
+[429](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001150 fpreset
+[430](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001150 .text
 AUX scnlen 0x3 nreloc 0 nlnno 0
 [432](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [434](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[436](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000011c .xdata
+[436](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000120 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [438](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000018c .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [440](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006834 .debug_info
 AUX scnlen 0x97 nreloc 6 nlnno 0
 [442](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000124b .debug_abbrev
 AUX scnlen 0x2d nreloc 0 nlnno 0
@@ -1012,39 +1014,39 @@
 AUX scnlen 0x58 nreloc 5 nlnno 0
 [448](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000a6a .debug_line_str
 AUX scnlen 0x9f nreloc 0 nlnno 0
 [450](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000550 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [452](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000568 .debug_frame
 AUX scnlen 0x30 nreloc 2 nlnno 0
-[454](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001130 .text
+[454](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001160 .text
 AUX scnlen 0x32 nreloc 0 nlnno 0
 [456](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [458](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[460](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001170 .text
+[460](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011a0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [462](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [464](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .bss
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [466](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000580 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [468](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001f0 dllentry.c
 File 
-[470](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001170 DllEntryPoint
+[470](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000011a0 DllEntryPoint
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[472](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001170 .text
+[472](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011a0 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
 [474](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [476](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[478](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000120 .xdata
+[478](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000124 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [480](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000198 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [482](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000068cb .debug_info
 AUX scnlen 0x1fa nreloc 6 nlnno 0
 [484](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001278 .debug_abbrev
 AUX scnlen 0x72 nreloc 0 nlnno 0
@@ -1056,23 +1058,23 @@
 AUX scnlen 0xce nreloc 0 nlnno 0
 [492](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005b0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [494](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000598 .debug_frame
 AUX scnlen 0x30 nreloc 2 nlnno 0
 [496](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000020c dllmain.c
 File 
-[498](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001180 DllMain
+[498](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000011b0 DllMain
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[500](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001180 .text
+[500](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011b0 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
 [502](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [504](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[506](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000124 .xdata
+[506](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000128 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [508](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001a4 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [510](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ac5 .debug_info
 AUX scnlen 0x1f4 nreloc 6 nlnno 0
 [512](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000012ea .debug_abbrev
 AUX scnlen 0x72 nreloc 0 nlnno 0
@@ -1084,23 +1086,23 @@
 AUX scnlen 0xd5 nreloc 0 nlnno 0
 [520](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005e0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [522](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005c8 .debug_frame
 AUX scnlen 0x30 nreloc 2 nlnno 0
 [524](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000022a ucrt_vfprintf.
 File 
-[526](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001190 vfprintf
+[526](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000011c0 vfprintf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[528](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001190 .text
+[528](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011c0 .text
 AUX scnlen 0x1e nreloc 1 nlnno 0
 [530](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [532](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[534](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000128 .xdata
+[534](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000012c .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [536](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001b0 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [538](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006cb9 .debug_info
 AUX scnlen 0x39d nreloc 14 nlnno 0
 [540](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000135c .debug_abbrev
 AUX scnlen 0x138 nreloc 0 nlnno 0
@@ -1114,40 +1116,40 @@
 AUX scnlen 0xe8 nreloc 0 nlnno 0
 [550](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000610 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [552](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005f8 .debug_frame
 AUX scnlen 0x38 nreloc 2 nlnno 0
 [554](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000279 ucrtbase_compa
 File 
-[556](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000011b0 _get_output_format
+[556](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000011e0 _get_output_format
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[558](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000011c0 __getmainargs
-[559](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001230 __wgetmainargs
-[560](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000012a0 _onexit
-[561](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000012c0 at_quick_exit
+[558](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000011f0 __getmainargs
+[559](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001260 __wgetmainargs
+[560](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000012d0 _onexit
+[561](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000012f0 at_quick_exit
 [562](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000260 .rdata$.refptr.__mingw_module_is_dll
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[564](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000012e0 _amsg_exit
-[565](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001310 __ms_fwprintf
-[566](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001350 tzset
+[564](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001310 _amsg_exit
+[565](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001340 __ms_fwprintf
+[566](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001380 tzset
 [567](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000240 .rdata$.refptr.__imp__tzset
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[569](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001390 _tzset
+[569](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013c0 _tzset
 [570](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000098 initial_daylight
 [571](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000009c initial_timezone
 [572](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000a0 initial_tznames
 [573](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b4 initial_tzname0
 [574](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b0 initial_tzname1
-[575](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011b0 .text
+[575](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011e0 .text
 AUX scnlen 0x216 nreloc 34 nlnno 0
 [577](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x78 nreloc 13 nlnno 0
 [579](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[581](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000130 .xdata
+[581](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000134 .xdata
 AUX scnlen 0x50 nreloc 0 nlnno 0
 [583](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001bc .pdata
 AUX scnlen 0x6c nreloc 27 nlnno 0
 [585](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c0 .rdata
 AUX scnlen 0x12 nreloc 0 nlnno 0
 [587](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000007056 .debug_info
 AUX scnlen 0x1185 nreloc 89 nlnno 0
@@ -1163,790 +1165,799 @@
 AUX scnlen 0x17 nreloc 0 nlnno 0
 [599](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d94 .debug_line_str
 AUX scnlen 0x160 nreloc 0 nlnno 0
 [601](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000640 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [603](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000630 .debug_frame
 AUX scnlen 0x190 nreloc 18 nlnno 0
-[605](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000013d0 .text
+[605](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001400 .text
 [606](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [607](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[608](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000824 .idata$7
-[609](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b0 .idata$5
-[610](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000220 .idata$4
-[611](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000678 .idata$6
-[612](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000013d8 .text
+[608](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000840 .idata$7
+[609](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c0 .idata$5
+[610](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000228 .idata$4
+[611](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000692 .idata$6
+[612](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001408 .text
 [613](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [614](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[615](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000828 .idata$7
-[616](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b8 .idata$5
-[617](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000228 .idata$4
-[618](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000686 .idata$6
-[619](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000013e0 .text
+[615](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000844 .idata$7
+[616](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c8 .idata$5
+[617](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000230 .idata$4
+[618](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006a0 .idata$6
+[619](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001410 .text
 [620](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [621](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[622](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000082c .idata$7
-[623](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c0 .idata$5
-[624](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000230 .idata$4
-[625](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000694 .idata$6
-[626](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000013e8 .text
+[622](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000848 .idata$7
+[623](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003d0 .idata$5
+[624](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000238 .idata$4
+[625](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ae .idata$6
+[626](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001418 .text
 [627](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [628](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[629](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000830 .idata$7
-[630](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c8 .idata$5
-[631](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000238 .idata$4
-[632](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006a0 .idata$6
+[629](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000084c .idata$7
+[630](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003d8 .idata$5
+[631](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000240 .idata$4
+[632](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ba .idata$6
 [633](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000287 fake
 File 
-[635](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000220 hname
-[636](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b0 fthunk
-[637](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000013f0 .text
+[635](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000228 hname
+[636](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c0 fthunk
+[637](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001420 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [639](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [641](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [643](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000008c .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[645](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000220 .idata$4
-[646](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b0 .idata$5
+[645](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000228 .idata$4
+[646](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c0 .idata$5
 [647](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002a3 fake
 File 
-[649](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000013f0 .text
+[649](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001420 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [651](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [653](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[655](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000240 .idata$4
+[655](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000248 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[657](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003d0 .idata$5
+[657](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003e0 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[659](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000834 .idata$7
+[659](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000850 .idata$7
 AUX scnlen 0x1f nreloc 0 nlnno 0
-[661](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000013f0 .text
+[661](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001420 .text
 [662](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [663](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[664](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007f8 .idata$7
-[665](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000398 .idata$5
-[666](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000208 .idata$4
-[667](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000664 .idata$6
-[668](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000013f8 .text
+[664](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000814 .idata$7
+[665](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a8 .idata$5
+[666](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000210 .idata$4
+[667](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000067e .idata$6
+[668](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001428 .text
 [669](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [670](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[671](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007fc .idata$7
-[672](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a0 .idata$5
-[673](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000210 .idata$4
-[674](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000066e .idata$6
+[671](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000818 .idata$7
+[672](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b0 .idata$5
+[673](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000218 .idata$4
+[674](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000688 .idata$6
 [675](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002b1 fake
 File 
-[677](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000208 hname
-[678](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000398 fthunk
-[679](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001400 .text
+[677](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000210 hname
+[678](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a8 fthunk
+[679](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001430 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [681](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [683](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [685](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000078 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[687](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000208 .idata$4
-[688](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000398 .idata$5
-[689](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002e9 fake
+[687](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000210 .idata$4
+[688](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a8 .idata$5
+[689](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002f0 fake
 File 
-[691](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001400 .text
+[691](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001430 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [693](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [695](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[697](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000218 .idata$4
+[697](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000220 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[699](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a8 .idata$5
+[699](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003b8 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[701](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000800 .idata$7
+[701](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000081c .idata$7
 AUX scnlen 0x21 nreloc 0 nlnno 0
-[703](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001400 .text
+[703](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001430 .text
 [704](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [705](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[706](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007c0 .idata$7
-[707](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000360 .idata$5
+[706](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007d8 .idata$7
+[707](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000368 .idata$5
 [708](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 .idata$4
-[709](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005fe .idata$6
-[710](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001408 .text
+[709](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000060e .idata$6
+[710](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001438 .text
 [711](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [712](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[713](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007c4 .idata$7
-[714](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000368 .idata$5
+[713](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007dc .idata$7
+[714](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000370 .idata$5
 [715](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d8 .idata$4
-[716](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000610 .idata$6
-[717](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001410 .text
+[716](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000620 .idata$6
+[717](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001440 .text
 [718](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [719](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[720](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007c8 .idata$7
-[721](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000370 .idata$5
+[720](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007e0 .idata$7
+[721](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000378 .idata$5
 [722](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e0 .idata$4
-[723](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000062a .idata$6
-[724](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001418 .text
+[723](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000063a .idata$6
+[724](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001448 .text
 [725](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [726](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[727](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007cc .idata$7
-[728](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000378 .idata$5
+[727](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007e4 .idata$7
+[728](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000380 .idata$5
 [729](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e8 .idata$4
-[730](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000646 .idata$6
-[731](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001420 .text
+[730](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000656 .idata$6
+[731](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001450 .text
 [732](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [733](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[734](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007d0 .idata$7
-[735](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000380 .idata$5
+[734](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007e8 .idata$7
+[735](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000388 .idata$5
 [736](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f0 .idata$4
-[737](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000650 .idata$6
-[738](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001428 .text
+[737](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000660 .idata$6
+[738](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001458 .text
 [739](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [740](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[741](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007d4 .idata$7
-[742](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000388 .idata$5
+[741](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007ec .idata$7
+[742](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000390 .idata$5
 [743](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f8 .idata$4
-[744](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000065a .idata$6
-[745](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002f7 fake
+[744](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000066a .idata$6
+[745](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001460 .text
+[746](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
+[747](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
+[748](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007f0 .idata$7
+[749](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000398 .idata$5
+[750](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000200 .idata$4
+[751](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000674 .idata$6
+[752](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002fe fake
 File 
-[747](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 hname
-[748](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000360 fthunk
-[749](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001430 .text
+[754](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 hname
+[755](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000368 fthunk
+[756](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001470 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[751](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[758](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[753](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[760](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[755](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000064 .idata$2
+[762](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000064 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[757](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 .idata$4
-[758](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000360 .idata$5
-[759](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000036e fake
+[764](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 .idata$4
+[765](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000368 .idata$5
+[766](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000375 fake
 File 
-[761](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001430 .text
+[768](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001470 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[763](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[770](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[765](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[772](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[767](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000200 .idata$4
+[774](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000208 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[769](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000390 .idata$5
+[776](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a0 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[771](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007d8 .idata$7
+[778](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007f4 .idata$7
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[773](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001430 .text
-[774](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
-[775](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[776](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000760 .idata$7
-[777](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e0 .idata$5
-[778](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 .idata$4
-[779](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004d0 .idata$6
-[780](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001438 .text
+[780](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001470 .text
 [781](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [782](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[783](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000764 .idata$7
+[783](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000778 .idata$7
 [784](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e8 .idata$5
-[785](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000158 .idata$4
-[786](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004de .idata$6
-[787](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001440 .text
+[785](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 .idata$4
+[786](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004e0 .idata$6
+[787](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001478 .text
 [788](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [789](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[790](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000768 .idata$7
+[790](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000077c .idata$7
 [791](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002f0 .idata$5
-[792](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000160 .idata$4
-[793](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ec .idata$6
-[794](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001448 .text
+[792](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000158 .idata$4
+[793](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ee .idata$6
+[794](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001480 .text
 [795](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [796](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[797](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000076c .idata$7
+[797](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000780 .idata$7
 [798](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002f8 .idata$5
-[799](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000168 .idata$4
-[800](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004fa .idata$6
-[801](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001450 .text
+[799](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000160 .idata$4
+[800](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004fc .idata$6
+[801](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001488 .text
 [802](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [803](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[804](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000770 .idata$7
+[804](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000784 .idata$7
 [805](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000300 .idata$5
-[806](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000170 .idata$4
-[807](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000514 .idata$6
-[808](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001458 .text
+[806](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000168 .idata$4
+[807](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000050a .idata$6
+[808](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001490 .text
 [809](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [810](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[811](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000774 .idata$7
+[811](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000788 .idata$7
 [812](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000308 .idata$5
-[813](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000178 .idata$4
-[814](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000052c .idata$6
-[815](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001460 .text
+[813](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000170 .idata$4
+[814](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000524 .idata$6
+[815](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001498 .text
 [816](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [817](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[818](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000778 .idata$7
+[818](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000078c .idata$7
 [819](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000310 .idata$5
-[820](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000180 .idata$4
-[821](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000542 .idata$6
-[822](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001468 .text
+[820](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000178 .idata$4
+[821](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000053c .idata$6
+[822](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014a0 .text
 [823](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [824](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[825](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000077c .idata$7
+[825](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000790 .idata$7
 [826](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000318 .idata$5
-[827](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000188 .idata$4
-[828](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000550 .idata$6
-[829](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001470 .text
+[827](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000180 .idata$4
+[828](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000552 .idata$6
+[829](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014a8 .text
 [830](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [831](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[832](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000780 .idata$7
+[832](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000794 .idata$7
 [833](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000320 .idata$5
-[834](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000190 .idata$4
-[835](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000568 .idata$6
-[836](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001478 .text
+[834](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000188 .idata$4
+[835](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000560 .idata$6
+[836](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014b0 .text
 [837](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [838](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[839](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000784 .idata$7
+[839](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000798 .idata$7
 [840](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000328 .idata$5
-[841](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000198 .idata$4
-[842](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000570 .idata$6
-[843](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001480 .text
+[841](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000190 .idata$4
+[842](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000578 .idata$6
+[843](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014b8 .text
 [844](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [845](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[846](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000788 .idata$7
+[846](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000079c .idata$7
 [847](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000330 .idata$5
-[848](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a0 .idata$4
-[849](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000592 .idata$6
-[850](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001488 .text
+[848](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000198 .idata$4
+[849](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000580 .idata$6
+[850](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014c0 .text
 [851](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [852](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[853](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000078c .idata$7
+[853](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007a0 .idata$7
 [854](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000338 .idata$5
-[855](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a8 .idata$4
-[856](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ae .idata$6
-[857](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001490 .text
+[855](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a0 .idata$4
+[856](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005a2 .idata$6
+[857](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014c8 .text
 [858](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [859](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[860](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000790 .idata$7
+[860](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007a4 .idata$7
 [861](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000340 .idata$5
-[862](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b0 .idata$4
-[863](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ce .idata$6
-[864](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001498 .text
+[862](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a8 .idata$4
+[863](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005be .idata$6
+[864](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014d0 .text
 [865](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [866](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[867](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000794 .idata$7
+[867](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007a8 .idata$7
 [868](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000348 .idata$5
-[869](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b8 .idata$4
-[870](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005da .idata$6
-[871](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014a0 .text
+[869](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b0 .idata$4
+[870](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005de .idata$6
+[871](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014d8 .text
 [872](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [873](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[874](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000798 .idata$7
+[874](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007ac .idata$7
 [875](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000350 .idata$5
-[876](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001c0 .idata$4
-[877](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005f6 .idata$6
-[878](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000037c fake
+[876](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b8 .idata$4
+[877](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ea .idata$6
+[878](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014e0 .text
+[879](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
+[880](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
+[881](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007b0 .idata$7
+[882](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000358 .idata$5
+[883](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001c0 .idata$4
+[884](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000606 .idata$6
+[885](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000383 fake
 File 
-[880](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 hname
-[881](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e0 fthunk
-[882](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014b0 .text
+[887](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 hname
+[888](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e8 fthunk
+[889](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014f0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[884](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[891](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[886](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[893](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[888](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .idata$2
+[895](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[890](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 .idata$4
-[891](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e0 .idata$5
-[892](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000039f fake
+[897](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 .idata$4
+[898](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e8 .idata$5
+[899](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003a6 fake
 File 
-[894](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014b0 .text
+[901](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014f0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[896](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[903](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[898](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[905](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[900](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c8 .idata$4
+[907](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c8 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[902](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000358 .idata$5
+[909](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000360 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[904](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000079c .idata$7
+[911](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007b4 .idata$7
 AUX scnlen 0x22 nreloc 0 nlnno 0
-[906](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014b0 .text
-[907](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
-[908](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[909](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000734 .idata$7
-[910](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c0 .idata$5
-[911](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 .idata$4
-[912](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ae .idata$6
-[913](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014b8 .text
+[913](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014f0 .text
 [914](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [915](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[916](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000738 .idata$7
+[916](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000074c .idata$7
 [917](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c8 .idata$5
-[918](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000138 .idata$4
+[918](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 .idata$4
 [919](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004be .idata$6
-[920](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014c0 .text
+[920](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014f8 .text
 [921](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [922](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[923](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000073c .idata$7
+[923](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000750 .idata$7
 [924](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002d0 .idata$5
-[925](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000140 .idata$4
-[926](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004c8 .idata$6
-[927](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003ad fake
+[925](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000138 .idata$4
+[926](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ce .idata$6
+[927](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001500 .text
+[928](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
+[929](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
+[930](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000754 .idata$7
+[931](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002d8 .idata$5
+[932](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000140 .idata$4
+[933](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004d8 .idata$6
+[934](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003b4 fake
 File 
-[929](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 hname
-[930](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c0 fthunk
-[931](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014d0 .text
+[936](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 hname
+[937](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c8 fthunk
+[938](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001510 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[933](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[940](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[935](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[942](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[937](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000003c .idata$2
+[944](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000003c .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[939](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 .idata$4
-[940](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c0 .idata$5
-[941](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003c9 fake
+[946](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 .idata$4
+[947](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c8 .idata$5
+[948](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003d0 fake
 File 
-[943](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014d0 .text
+[950](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001510 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[945](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[952](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[947](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[954](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[949](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000148 .idata$4
+[956](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000148 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[951](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002d8 .idata$5
+[958](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002e0 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[953](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000740 .idata$7
+[960](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000758 .idata$7
 AUX scnlen 0x1f nreloc 0 nlnno 0
-[955](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014d0 .text
-[956](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
-[957](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[958](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000704 .idata$7
-[959](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a8 .idata$5
-[960](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 .idata$4
-[961](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000048e .idata$6
-[962](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014d8 .text
+[962](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001510 .text
 [963](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [964](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[965](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000708 .idata$7
+[965](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000071c .idata$7
 [966](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b0 .idata$5
-[967](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000120 .idata$4
+[967](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 .idata$4
 [968](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000049e .idata$6
-[969](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003d7 fake
+[969](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001518 .text
+[970](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
+[971](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
+[972](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000720 .idata$7
+[973](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b8 .idata$5
+[974](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000120 .idata$4
+[975](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ae .idata$6
+[976](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003de fake
 File 
-[971](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 hname
-[972](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a8 fthunk
-[973](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014e0 .text
+[978](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 hname
+[979](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b0 fthunk
+[980](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001520 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[975](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[982](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[977](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[984](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[979](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000028 .idata$2
+[986](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000028 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[981](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 .idata$4
-[982](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a8 .idata$5
-[983](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003ec fake
+[988](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 .idata$4
+[989](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b0 .idata$5
+[990](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003f3 fake
 File 
-[985](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014e0 .text
+[992](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001520 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[987](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[994](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[989](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[996](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[991](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000128 .idata$4
+[998](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000128 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[993](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002b8 .idata$5
+[1000](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002c0 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[995](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000070c .idata$7
+[1002](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000724 .idata$7
 AUX scnlen 0x26 nreloc 0 nlnno 0
-[997](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014e0 .text
-[998](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
-[999](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1000](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e0 .idata$7
-[1001](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000298 .idata$5
-[1002](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 .idata$4
-[1003](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000484 .idata$6
-[1004](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003fa fake
+[1004](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001520 .text
+[1005](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
+[1006](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
+[1007](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f8 .idata$7
+[1008](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a0 .idata$5
+[1009](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 .idata$4
+[1010](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000494 .idata$6
+[1011](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000401 fake
 File 
-[1006](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 hname
-[1007](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000298 fthunk
-[1008](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014f0 .text
+[1013](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 hname
+[1014](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a0 fthunk
+[1015](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001530 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1010](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[1017](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1012](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1019](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1014](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .idata$2
+[1021](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[1016](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 .idata$4
-[1017](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000298 .idata$5
-[1018](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000408 fake
+[1023](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 .idata$4
+[1024](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a0 .idata$5
+[1025](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000040f fake
 File 
-[1020](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014f0 .text
+[1027](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001530 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1022](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[1029](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1024](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1031](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1026](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .idata$4
+[1033](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1028](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002a0 .idata$5
+[1035](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002a8 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1030](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006e4 .idata$7
+[1037](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006fc .idata$7
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[1032](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000465 ucrt_fprintf.c
+[1039](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000046c ucrt_fprintf.c
 File 
-[1034](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000014f0 fprintf
+[1041](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001530 fprintf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1036](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014f0 .text
+[1043](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001530 .text
 AUX scnlen 0x32 nreloc 1 nlnno 0
-[1038](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[1045](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[1040](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1047](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1042](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000180 .xdata
+[1049](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000184 .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1044](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000228 .pdata
+[1051](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000228 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[1046](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000081db .debug_info
+[1053](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000081db .debug_info
 AUX scnlen 0x3a2 nreloc 14 nlnno 0
-[1048](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000017b7 .debug_abbrev
+[1055](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000017b7 .debug_abbrev
 AUX scnlen 0x162 nreloc 0 nlnno 0
-[1050](sec 19)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000129a .debug_loclists
+[1057](sec 19)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000129a .debug_loclists
 AUX scnlen 0x46 nreloc 0 nlnno 0
-[1052](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002b0 .debug_aranges
+[1059](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002b0 .debug_aranges
 AUX scnlen 0x30 nreloc 2 nlnno 0
-[1054](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001856 .debug_line
+[1061](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001856 .debug_line
 AUX scnlen 0x8a nreloc 9 nlnno 0
-[1056](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000ef4 .debug_line_str
+[1063](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000ef4 .debug_line_str
 AUX scnlen 0xe5 nreloc 0 nlnno 0
-[1058](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000670 .rdata$zzz
+[1065](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000670 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
-[1060](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007c0 .debug_frame
+[1067](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007c0 .debug_frame
 AUX scnlen 0x38 nreloc 2 nlnno 0
-[1062](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001530 .text
-[1063](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
-[1064](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1065](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006cc .idata$7
-[1066](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000288 .idata$5
-[1067](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f8 .idata$4
-[1068](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000474 .idata$6
-[1069](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001538 .text
+[1069](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001570 .text
 [1070](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1071](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1072](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c8 .idata$7
-[1073](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 .idata$5
-[1074](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f0 .idata$4
-[1075](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000462 .idata$6
-[1076](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001540 .text
+[1072](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e4 .idata$7
+[1073](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000290 .idata$5
+[1074](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f8 .idata$4
+[1075](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000484 .idata$6
+[1076](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001578 .text
 [1077](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1078](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1079](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c4 .idata$7
-[1080](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000278 .idata$5
-[1081](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e8 .idata$4
-[1082](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000454 .idata$6
-[1083](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001548 .text
+[1079](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e0 .idata$7
+[1080](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000288 .idata$5
+[1081](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f0 .idata$4
+[1082](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000472 .idata$6
+[1083](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001580 .text
 [1084](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1085](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1086](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c0 .idata$7
-[1087](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000270 .idata$5
-[1088](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .idata$4
-[1089](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000044c .idata$6
-[1090](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001550 .text
+[1086](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006dc .idata$7
+[1087](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 .idata$5
+[1088](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e8 .idata$4
+[1089](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000464 .idata$6
+[1090](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001588 .text
 [1091](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1092](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1093](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006bc .idata$7
-[1094](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000268 .idata$5
-[1095](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d8 .idata$4
-[1096](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000434 .idata$6
-[1097](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001558 .text
+[1093](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d8 .idata$7
+[1094](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000278 .idata$5
+[1095](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .idata$4
+[1096](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000045c .idata$6
+[1097](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001590 .text
 [1098](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1099](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1100](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b8 .idata$7
-[1101](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000260 .idata$5
-[1102](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .idata$4
-[1103](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000418 .idata$6
-[1104](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001560 .text
+[1100](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d4 .idata$7
+[1101](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000270 .idata$5
+[1102](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d8 .idata$4
+[1103](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000444 .idata$6
+[1104](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001598 .text
 [1105](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1106](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1107](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b4 .idata$7
-[1108](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000258 .idata$5
-[1109](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c8 .idata$4
-[1110](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000408 .idata$6
-[1111](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001568 .text
+[1107](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d0 .idata$7
+[1108](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000268 .idata$5
+[1109](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .idata$4
+[1110](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000428 .idata$6
+[1111](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000015a0 .text
 [1112](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1113](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1114](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b0 .idata$7
-[1115](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000250 .idata$5
-[1116](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c0 .idata$4
-[1117](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003f0 .idata$6
-[1118](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001570 .text
+[1114](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006cc .idata$7
+[1115](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000260 .idata$5
+[1116](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c8 .idata$4
+[1117](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000418 .idata$6
+[1118](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000015a8 .text
 [1119](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1120](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1121](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ac .idata$7
-[1122](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000248 .idata$5
-[1123](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 .idata$4
-[1124](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003d8 .idata$6
-[1125](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000473 fake
+[1121](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c8 .idata$7
+[1122](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000258 .idata$5
+[1123](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c0 .idata$4
+[1124](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000400 .idata$6
+[1125](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000015b0 .text
+[1126](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
+[1127](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
+[1128](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c4 .idata$7
+[1129](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000250 .idata$5
+[1130](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 .idata$4
+[1131](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003e8 .idata$6
+[1132](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000047a fake
 File 
-[1127](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 hname
-[1128](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000248 fthunk
-[1129](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001580 .text
+[1134](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 hname
+[1135](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000250 fthunk
+[1136](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000015c0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1131](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
+[1138](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1133](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1140](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1135](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .idata$2
+[1142](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[1137](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 .idata$4
-[1138](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000248 .idata$5
-[1139](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000481 fake
+[1144](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 .idata$4
+[1145](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000250 .idata$5
+[1146](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000488 fake
 File 
-[1141](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001580 .text
+[1148](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000015c0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1143](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
+[1150](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1145](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1152](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1147](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000100 .idata$4
+[1154](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000100 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1149](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000290 .idata$5
+[1156](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000298 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1151](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006d0 .idata$7
+[1158](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006e8 .idata$7
 AUX scnlen 0xd nreloc 0 nlnno 0
-[1153](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000495 cygming-crtend
+[1160](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000049c cygming-crtend
 File 
-[1155](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000001580 register_frame_ctor
+[1162](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000015c0 register_frame_ctor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1157](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001580 .text
+[1164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000015c0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1159](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
+[1166](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1161](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1168](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1163](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001580 .text.startup
+[1170](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000015c0 .text.startup
 AUX scnlen 0x5 nreloc 1 nlnno 0
-[1165](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000188 .xdata.startup
+[1172](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000018c .xdata.startup
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[1167](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000234 .pdata.startup
+[1174](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000234 .pdata.startup
 AUX scnlen 0xc nreloc 3 nlnno 0
-[1169](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001598 .ctors.65535
+[1176](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000015d8 .ctors.65535
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[1171](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006a0 .rdata$zzz
+[1178](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006a0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
-[1173](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 __xc_z
-[1174](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001428 putchar
-[1175](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 ___RUNTIME_PSEUDO_RELOC_LIST__
-[1176](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013d0 __daylight
-[1177](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001410 __stdio_common_vfwprintf
-[1178](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000350 __imp_abort
-[1179](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __lib64_libkernel32_a_iname
-[1180](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a8 __imp___p__environ
-[1181](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __data_start__
-[1182](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015a8 ___DTOR_LIST__
-[1183](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000088 __imp_timezone
-[1184](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c8 __imp_calloc
-[1185](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e0 __imp___p___argc
-[1186](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000090 __imp_tzname
-[1187](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001480 _initialize_onexit_table
-[1188](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___tls_start__
-[1189](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000290 .refptr.__native_startup_state
-[1190](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000058 __imp_tzset
-[1191](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 __xl_a
-[1192](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001560 GetLastError
-[1193](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000338 __imp__initialize_wide_environment
-[1194](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __rt_psrelocs_start
-[1195](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000160 __dll_characteristics__
-[1196](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_stack_commit__
-[1197](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000834 __lib64_libapi_ms_win_crt_time_l1_1_0_a_iname
-[1198](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __mingw_module_is_dll
-[1199](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000200000 __size_of_stack_reserve__
-[1200](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000005 __major_subsystem_version__
-[1201](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xl_start__
-[1202](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000248 __imp_DeleteCriticalSection
-[1203](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __xl_d
-[1204](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 _tls_end
-[1205](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001f0 .refptr.__CTOR_LIST__
-[1206](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013e0 __tzname
-[1207](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001530 VirtualQuery
-[1208](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e8 __imp___p___argv
-[1209](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xi_start__
-[1210](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000068 __imp__amsg_exit
-[1211](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xi_end__
-[1212](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000260 .refptr.__mingw_module_is_dll
-[1213](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _tls_start
-[1214](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006e4 __lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname
-[1215](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000220 .refptr.__RUNTIME_PSEUDO_RELOC_LIST__
-[1216](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 _CRT_MT
-[1217](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001540 TlsGetValue
-[1218](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __bss_start__
-[1219](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000388 __imp_putchar
-[1220](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 ___RUNTIME_PSEUDO_RELOC_LIST_END__
-[1221](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003c0 __imp___tzname
-[1222](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_heap_commit__
-[1223](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000368 __imp___stdio_common_vfprintf
-[1224](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000258 __imp_GetLastError
-[1225](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001418 kbhit
-[1226](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000328 __imp__initialize_narrow_environment
-[1227](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 __mingw_initltsdrot_force
-[1228](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d0 __imp_free
-[1229](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000300 __imp__configure_wide_argv
-[1230](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000b8 __imp_at_quick_exit
-[1231](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014d0 __p__environ
-[1232](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000250 .refptr.__mingw_app_type
-[1233](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __mingw_initltssuo_force
-[1234](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001538 VirtualProtect
-[1235](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 _head_lib64_libapi_ms_win_crt_environment_l1_1_0_a
-[1236](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003c8 __imp__tzset
-[1237](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_start__
-[1238](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000268 __imp_LeaveCriticalSection
-[1239](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014a0 abort
-[1240](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000210 .refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
-[1241](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __imp___ms_fwprintf
-[1242](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_end__
-[1243](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll__
-[1244](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_os_version__
-[1245](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001438 __p___argv
-[1246](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000800 __lib64_libapi_ms_win_crt_string_l1_1_0_a_iname
-[1247](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001568 EnterCriticalSection
-[1248](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 _head_lib64_libapi_ms_win_crt_conio_l1_1_0_a
-[1249](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014b0 _set_new_mode
-[1250](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c0 .refptr.__xi_a
-[1251](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001e0 .refptr._CRT_MT
-[1252](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014e0 getch
-[1253](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000320 __imp__exit
-[1254](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __section_alignment__
-[1255](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000024 __native_dllmain_reason
-[1256](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014b8 calloc
-[1257](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 _tls_used
-[1258](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003d8 __IAT_end__
-[1259](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000008c _head_lib64_libapi_ms_win_crt_time_l1_1_0_a
-[1260](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __RUNTIME_PSEUDO_RELOC_LIST__
-[1261](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001548 Sleep
-[1262](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000e0 __data_end__
-[1263](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000380 __imp_fwrite
-[1264](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001590 __CTOR_LIST__
-[1265](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000298 __imp_getch
-[1266](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c0 __imp__set_new_mode
-[1267](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000003c _head_lib64_libapi_ms_win_crt_heap_l1_1_0_a
-[1268](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000078 __imp___getmainargs
-[1269](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _head_lib64_libkernel32_a
-[1270](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000110 __bss_end__
-[1271](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __xi_z
-[1272](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000018 pcinit
-[1273](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __native_vcclrit_reason
-[1274](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xc_end__
-[1275](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000280 .refptr.__native_startup_lock
-[1276](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000250 __imp_EnterCriticalSection
-[1277](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000004c _tls_index
-[1278](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001400 __acrt_iob_func
-[1279](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __native_startup_state
-[1280](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___crt_xc_start__
-[1281](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000378 __imp_kbhit
-[1282](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013f8 strncmp
-[1283](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001590 ___CTOR_LIST__
-[1284](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000230 .refptr.__dyn_tls_init_callback
-[1285](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000348 __imp__register_onexit_function
-[1286](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000078 _head_lib64_libapi_ms_win_crt_string_l1_1_0_a
-[1287](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __rt_psrelocs_size
-[1288](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001468 _execute_onexit_table
-[1289](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 .refptr.__ImageBase
-[1290](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000079c __lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname
-[1291](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f0 __imp___p___wargv
-[1292](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000398 __imp_strlen
-[1293](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000070 __imp___wgetmainargs
-[1294](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003b0 __imp___daylight
-[1295](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 __file_alignment__
-[1296](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000260 __imp_InitializeCriticalSection
-[1297](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014d8 __p__wenviron
-[1298](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001478 _initialize_narrow_environment
-[1299](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001458 _crt_at_quick_exit
-[1300](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001558 InitializeCriticalSection
-[1301](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000064 _head_lib64_libapi_ms_win_crt_stdio_l1_1_0_a
-[1302](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __imp_vfprintf
-[1303](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000004 __major_os_version__
-[1304](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000248 __IAT_start__
-[1305](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __xl_z
-[1306](sec  0)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __end__
-[1307](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000370 __imp___stdio_common_vfwprintf
-[1308](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000c0 __imp__onexit
-[1309](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015a8 __DTOR_LIST__
-[1310](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000330 __imp__initialize_onexit_table
-[1311](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __xi_a
-[1312](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000270 __imp_Sleep
-[1313](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001550 LeaveCriticalSection
-[1314](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __xc_a
-[1315](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000100000 __size_of_heap_reserve__
-[1316](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_start__
-[1317](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000003 __subsystem__
-[1318](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000278 __imp_TlsGetValue
-[1319](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b0 __imp___p__wenviron
-[1320](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000318 __imp__execute_onexit_table
-[1321](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003b8 __imp___timezone
-[1322](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000d0 __imp_fprintf
-[1323](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001450 _configure_wide_argv
-[1324](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000310 __imp__crt_atexit
-[1325](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000070c __lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname
-[1326](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001498 _register_onexit_function
-[1327](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001430 __p___argc
-[1328](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000280 __imp_VirtualProtect
-[1329](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __xl_c
-[1330](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___tls_end__
-[1331](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000240 .refptr.__imp__tzset
-[1332](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000288 __imp_VirtualQuery
-[1333](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000340 __imp__initterm
-[1334](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000044 __mingw_initltsdyn_force
-[1335](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007d8 __lib64_libapi_ms_win_crt_stdio_l1_1_0_a_iname
-[1336](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dyn_tls_init_callback
-[1337](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013d8 __timezone
-[1338](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000740 __lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname
-[1339](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001490 _initterm
-[1340](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001420 fwrite
-[1341](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003a0 __imp_strncmp
-[1342](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000360 __imp___acrt_iob_func
-[1343](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __major_image_version__
-[1344](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __loader_flags__
-[1345](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001130 ___chkstk_ms
-[1346](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __native_startup_lock
-[1347](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000270 .refptr.__native_dllmain_reason
-[1348](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __rt_psrelocs_end
-[1349](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000002 __minor_subsystem_version__
-[1350](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_image_version__
-[1351](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000308 __imp__crt_at_quick_exit
-[1352](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001470 _exit
-[1353](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a0 .refptr.__xc_a
-[1354](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001448 _configure_narrow_argv
-[1355](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013f0 strlen
-[1356](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d0 .refptr.__xi_z
-[1357](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001460 _crt_atexit
-[1358](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001570 DeleteCriticalSection
-[1359](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001488 _initialize_wide_environment
-[1360](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f8 __imp__configure_narrow_argv
-[1361](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 _head_lib64_libapi_ms_win_crt_runtime_l1_1_0_a
-[1362](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __RUNTIME_PSEUDO_RELOC_LIST_END__
-[1363](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b0 .refptr.__xc_z
-[1364](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000060 __imp__get_output_format
-[1365](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_end__
-[1366](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001408 __stdio_common_vfprintf
-[1367](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000080 __imp_daylight
-[1368](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001440 __p___wargv
-[1369](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014c0 free
-[1370](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __mingw_app_type
+[1180](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 __xc_z
+[1181](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001460 putchar
+[1182](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 ___RUNTIME_PSEUDO_RELOC_LIST__
+[1183](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001400 __daylight
+[1184](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001440 __stdio_common_vfwprintf
+[1185](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000358 __imp_abort
+[1186](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006e8 __lib64_libkernel32_a_iname
+[1187](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b0 __imp___p__environ
+[1188](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __data_start__
+[1189](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015e8 ___DTOR_LIST__
+[1190](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000088 __imp_timezone
+[1191](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d0 __imp_calloc
+[1192](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e8 __imp___p___argc
+[1193](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000090 __imp_tzname
+[1194](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014c0 _initialize_onexit_table
+[1195](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___tls_start__
+[1196](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000290 .refptr.__native_startup_state
+[1197](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000058 __imp_tzset
+[1198](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 __xl_a
+[1199](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015a0 GetLastError
+[1200](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000340 __imp__initialize_wide_environment
+[1201](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __rt_psrelocs_start
+[1202](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000160 __dll_characteristics__
+[1203](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_stack_commit__
+[1204](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000850 __lib64_libapi_ms_win_crt_time_l1_1_0_a_iname
+[1205](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __mingw_module_is_dll
+[1206](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000200000 __size_of_stack_reserve__
+[1207](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000005 __major_subsystem_version__
+[1208](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xl_start__
+[1209](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000250 __imp_DeleteCriticalSection
+[1210](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __xl_d
+[1211](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 _tls_end
+[1212](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001f0 .refptr.__CTOR_LIST__
+[1213](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001410 __tzname
+[1214](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001570 VirtualQuery
+[1215](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f0 __imp___p___argv
+[1216](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xi_start__
+[1217](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000068 __imp__amsg_exit
+[1218](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xi_end__
+[1219](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000260 .refptr.__mingw_module_is_dll
+[1220](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _tls_start
+[1221](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006fc __lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname
+[1222](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000220 .refptr.__RUNTIME_PSEUDO_RELOC_LIST__
+[1223](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 _CRT_MT
+[1224](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001580 TlsGetValue
+[1225](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __bss_start__
+[1226](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000398 __imp_putchar
+[1227](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 ___RUNTIME_PSEUDO_RELOC_LIST_END__
+[1228](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003d0 __imp___tzname
+[1229](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_heap_commit__
+[1230](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000370 __imp___stdio_common_vfprintf
+[1231](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000260 __imp_GetLastError
+[1232](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001448 kbhit
+[1233](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000330 __imp__initialize_narrow_environment
+[1234](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 __mingw_initltsdrot_force
+[1235](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d8 __imp_free
+[1236](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000308 __imp__configure_wide_argv
+[1237](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000b8 __imp_at_quick_exit
+[1238](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001510 __p__environ
+[1239](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000250 .refptr.__mingw_app_type
+[1240](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __mingw_initltssuo_force
+[1241](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001450 fflush
+[1242](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001578 VirtualProtect
+[1243](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 _head_lib64_libapi_ms_win_crt_environment_l1_1_0_a
+[1244](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003d8 __imp__tzset
+[1245](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_start__
+[1246](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000270 __imp_LeaveCriticalSection
+[1247](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014e0 abort
+[1248](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000210 .refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
+[1249](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __imp___ms_fwprintf
+[1250](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_end__
+[1251](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll__
+[1252](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_os_version__
+[1253](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001478 __p___argv
+[1254](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000081c __lib64_libapi_ms_win_crt_string_l1_1_0_a_iname
+[1255](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015a8 EnterCriticalSection
+[1256](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 _head_lib64_libapi_ms_win_crt_conio_l1_1_0_a
+[1257](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014f0 _set_new_mode
+[1258](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c0 .refptr.__xi_a
+[1259](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001e0 .refptr._CRT_MT
+[1260](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001520 getch
+[1261](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000328 __imp__exit
+[1262](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __section_alignment__
+[1263](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000024 __native_dllmain_reason
+[1264](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014f8 calloc
+[1265](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 _tls_used
+[1266](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003e8 __IAT_end__
+[1267](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000008c _head_lib64_libapi_ms_win_crt_time_l1_1_0_a
+[1268](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __RUNTIME_PSEUDO_RELOC_LIST__
+[1269](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001588 Sleep
+[1270](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000e0 __data_end__
+[1271](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000390 __imp_fwrite
+[1272](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015d0 __CTOR_LIST__
+[1273](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a0 __imp_getch
+[1274](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c8 __imp__set_new_mode
+[1275](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000003c _head_lib64_libapi_ms_win_crt_heap_l1_1_0_a
+[1276](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000078 __imp___getmainargs
+[1277](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _head_lib64_libkernel32_a
+[1278](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000110 __bss_end__
+[1279](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __xi_z
+[1280](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000018 pcinit
+[1281](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __native_vcclrit_reason
+[1282](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xc_end__
+[1283](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000280 .refptr.__native_startup_lock
+[1284](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000258 __imp_EnterCriticalSection
+[1285](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000004c _tls_index
+[1286](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001430 __acrt_iob_func
+[1287](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __native_startup_state
+[1288](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___crt_xc_start__
+[1289](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000380 __imp_kbhit
+[1290](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001428 strncmp
+[1291](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015d0 ___CTOR_LIST__
+[1292](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000230 .refptr.__dyn_tls_init_callback
+[1293](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000350 __imp__register_onexit_function
+[1294](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000078 _head_lib64_libapi_ms_win_crt_string_l1_1_0_a
+[1295](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __rt_psrelocs_size
+[1296](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014a8 _execute_onexit_table
+[1297](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 .refptr.__ImageBase
+[1298](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007b4 __lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname
+[1299](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f8 __imp___p___wargv
+[1300](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003a8 __imp_strlen
+[1301](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000070 __imp___wgetmainargs
+[1302](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003c0 __imp___daylight
+[1303](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 __file_alignment__
+[1304](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000268 __imp_InitializeCriticalSection
+[1305](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001518 __p__wenviron
+[1306](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014b8 _initialize_narrow_environment
+[1307](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001498 _crt_at_quick_exit
+[1308](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001598 InitializeCriticalSection
+[1309](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000064 _head_lib64_libapi_ms_win_crt_stdio_l1_1_0_a
+[1310](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __imp_vfprintf
+[1311](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000004 __major_os_version__
+[1312](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000250 __IAT_start__
+[1313](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __xl_z
+[1314](sec  0)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __end__
+[1315](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000378 __imp___stdio_common_vfwprintf
+[1316](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000c0 __imp__onexit
+[1317](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015e8 __DTOR_LIST__
+[1318](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000338 __imp__initialize_onexit_table
+[1319](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __xi_a
+[1320](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000278 __imp_Sleep
+[1321](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001590 LeaveCriticalSection
+[1322](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __xc_a
+[1323](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000100000 __size_of_heap_reserve__
+[1324](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_start__
+[1325](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000003 __subsystem__
+[1326](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000280 __imp_TlsGetValue
+[1327](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b8 __imp___p__wenviron
+[1328](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000320 __imp__execute_onexit_table
+[1329](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003c8 __imp___timezone
+[1330](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000d0 __imp_fprintf
+[1331](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001490 _configure_wide_argv
+[1332](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000318 __imp__crt_atexit
+[1333](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000724 __lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname
+[1334](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014d8 _register_onexit_function
+[1335](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001470 __p___argc
+[1336](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000288 __imp_VirtualProtect
+[1337](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __xl_c
+[1338](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___tls_end__
+[1339](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000240 .refptr.__imp__tzset
+[1340](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000290 __imp_VirtualQuery
+[1341](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000348 __imp__initterm
+[1342](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000044 __mingw_initltsdyn_force
+[1343](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007f4 __lib64_libapi_ms_win_crt_stdio_l1_1_0_a_iname
+[1344](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dyn_tls_init_callback
+[1345](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001408 __timezone
+[1346](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000758 __lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname
+[1347](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014d0 _initterm
+[1348](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001458 fwrite
+[1349](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003b0 __imp_strncmp
+[1350](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000368 __imp___acrt_iob_func
+[1351](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __major_image_version__
+[1352](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __loader_flags__
+[1353](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001160 ___chkstk_ms
+[1354](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __native_startup_lock
+[1355](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000270 .refptr.__native_dllmain_reason
+[1356](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __rt_psrelocs_end
+[1357](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000002 __minor_subsystem_version__
+[1358](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000388 __imp_fflush
+[1359](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_image_version__
+[1360](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000310 __imp__crt_at_quick_exit
+[1361](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014b0 _exit
+[1362](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a0 .refptr.__xc_a
+[1363](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001488 _configure_narrow_argv
+[1364](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001420 strlen
+[1365](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d0 .refptr.__xi_z
+[1366](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014a0 _crt_atexit
+[1367](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015b0 DeleteCriticalSection
+[1368](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014c8 _initialize_wide_environment
+[1369](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000300 __imp__configure_narrow_argv
+[1370](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 _head_lib64_libapi_ms_win_crt_runtime_l1_1_0_a
+[1371](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __RUNTIME_PSEUDO_RELOC_LIST_END__
+[1372](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b0 .refptr.__xc_z
+[1373](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000060 __imp__get_output_format
+[1374](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_end__
+[1375](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001438 __stdio_common_vfprintf
+[1376](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000080 __imp_daylight
+[1377](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001480 __p___wargv
+[1378](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001500 free
+[1379](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __mingw_app_type
 
 
 
 Disassembly of section .text:
 
 000000029a1b1000 <pre_c_init>:
 pre_c_init():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:64
    29a1b1000:	lea    0x5ff9(%rip),%rcx        # 29a1b7000 <__bss_start__>
-   29a1b1007:	jmp    29a1b2480 <_initialize_onexit_table>
+   29a1b1007:	jmp    29a1b24c0 <_initialize_onexit_table>
    29a1b100c:	nopl   0x0(%rax)
 
 000000029a1b1010 <_CRT_INIT>:
 _CRT_INIT():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:68
    29a1b1010:	push   %r13
    29a1b1012:	push   %r12
@@ -1971,15 +1982,15 @@
 C:\M\B\src\build-UCRT64/D:/a/msys64/ucrt64/include/psdk_inc/intrin-impl.h:1737
    29a1b103a:	xor    %ebp,%ebp
    29a1b103c:	mov    $0x1,%edi
 _CRT_INIT():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:72
    29a1b1041:	mov    %eax,0x5fd1(%rip)        # 29a1b7018 <__proc_attached>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:122
-   29a1b1047:	mov    0x8222(%rip),%r12        # 29a1b9270 <__imp_Sleep>
+   29a1b1047:	mov    0x822a(%rip),%r12        # 29a1b9278 <__imp_Sleep>
    29a1b104e:	jmp    29a1b1058 <_CRT_INIT+0x48>
    29a1b1050:	mov    $0x3e8,%ecx
    29a1b1055:	call   *%r12
 _InterlockedCompareExchangePointer():
 C:\M\B\src\build-UCRT64/D:/a/msys64/ucrt64/include/psdk_inc/intrin-impl.h:1737
    29a1b1058:	mov    %rbp,%rax
    29a1b105b:	lock cmpxchg %rdi,(%rbx)
@@ -1991,15 +2002,15 @@
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:124
    29a1b1068:	mov    0x3221(%rip),%rdi        # 29a1b4290 <.refptr.__native_startup_state>
    29a1b106f:	mov    (%rdi),%eax
    29a1b1071:	cmp    $0x2,%eax
    29a1b1074:	je     29a1b1140 <_CRT_INIT+0x130>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:126
    29a1b107a:	mov    $0x1f,%ecx
-   29a1b107f:	call   29a1b22e0 <_amsg_exit>
+   29a1b107f:	call   29a1b2310 <_amsg_exit>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:135
    29a1b1084:	mov    $0x1,%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:136
    29a1b1089:	mov    %edx,%eax
    29a1b108b:	add    $0x28,%rsp
    29a1b108f:	pop    %rbx
    29a1b1090:	pop    %rsi
@@ -2020,15 +2031,15 @@
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:79
    29a1b10b5:	mov    0x8(%rax),%rsi
 _InterlockedCompareExchangePointer():
 C:\M\B\src\build-UCRT64/D:/a/msys64/ucrt64/include/psdk_inc/intrin-impl.h:1737
    29a1b10b9:	xor    %ebp,%ebp
 _CRT_INIT():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:90
-   29a1b10bb:	mov    0x81ae(%rip),%r12        # 29a1b9270 <__imp_Sleep>
+   29a1b10bb:	mov    0x81b6(%rip),%r12        # 29a1b9278 <__imp_Sleep>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:82
    29a1b10c2:	jmp    29a1b10d9 <_CRT_INIT+0xc9>
    29a1b10c4:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:85
    29a1b10c8:	cmp    %rax,%rsi
    29a1b10cb:	je     29a1b1160 <_CRT_INIT+0x150>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:90
@@ -2073,15 +2084,15 @@
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:115
    29a1b112f:	addl   $0x1,0x5ee2(%rip)        # 29a1b7018 <__proc_attached>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:135
    29a1b1136:	mov    $0x1,%edx
    29a1b113b:	jmp    29a1b1089 <_CRT_INIT+0x79>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:130
    29a1b1140:	lea    0x5eb9(%rip),%rcx        # 29a1b7000 <__bss_start__>
-   29a1b1147:	call   29a1b2468 <_execute_onexit_table>
+   29a1b1147:	call   29a1b24a8 <_execute_onexit_table>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:131
    29a1b114c:	movl   $0x0,(%rdi)
 _InterlockedExchangePointer():
 C:\M\B\src\build-UCRT64/D:/a/msys64/ucrt64/include/psdk_inc/intrin-impl.h:1748
    29a1b1152:	xchg   %rsi,(%rbx)
    29a1b1155:	jmp    29a1b1084 <_CRT_INIT+0x74>
    29a1b115a:	nopw   0x0(%rax,%rax,1)
@@ -2099,28 +2110,28 @@
 _CRT_INIT():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:100
    29a1b1180:	mov    0x3149(%rip),%rdx        # 29a1b42d0 <.refptr.__xi_z>
    29a1b1187:	mov    0x3132(%rip),%rcx        # 29a1b42c0 <.refptr.__xi_a>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:98
    29a1b118e:	movl   $0x1,(%rsi)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:100
-   29a1b1194:	call   29a1b2490 <_initterm>
+   29a1b1194:	call   29a1b24d0 <_initterm>
    29a1b1199:	jmp    29a1b1104 <_CRT_INIT+0xf4>
    29a1b119e:	xchg   %ax,%ax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:104
    29a1b11a0:	mov    0x3109(%rip),%rdx        # 29a1b42b0 <.refptr.__xc_z>
    29a1b11a7:	mov    0x30f2(%rip),%rcx        # 29a1b42a0 <.refptr.__xc_a>
-   29a1b11ae:	call   29a1b2490 <_initterm>
+   29a1b11ae:	call   29a1b24d0 <_initterm>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:105
    29a1b11b3:	movl   $0x2,(%rsi)
    29a1b11b9:	jmp    29a1b110f <_CRT_INIT+0xff>
    29a1b11be:	xchg   %ax,%ax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:94
    29a1b11c0:	mov    $0x1f,%ecx
-   29a1b11c5:	call   29a1b22e0 <_amsg_exit>
+   29a1b11c5:	call   29a1b2310 <_amsg_exit>
    29a1b11ca:	jmp    29a1b1104 <_CRT_INIT+0xf4>
    29a1b11cf:	nop
 
 000000029a1b11d0 <__DllMainCRTStartup>:
 __DllMainCRTStartup():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:161
    29a1b11d0:	push   %r12
@@ -2141,25 +2152,25 @@
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:165
    29a1b11ec:	test   %edx,%edx
    29a1b11ee:	jne    29a1b1250 <__DllMainCRTStartup+0x80>
    29a1b11f0:	mov    0x5e22(%rip),%eax        # 29a1b7018 <__proc_attached>
    29a1b11f6:	test   %eax,%eax
    29a1b11f8:	je     29a1b1230 <__DllMainCRTStartup+0x60>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:170
-   29a1b11fa:	call   29a1b1750 <_pei386_runtime_relocator>
+   29a1b11fa:	call   29a1b1780 <_pei386_runtime_relocator>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:186
    29a1b11ff:	mov    %rdi,%r8
    29a1b1202:	xor    %edx,%edx
    29a1b1204:	mov    %rsi,%rcx
-   29a1b1207:	call   29a1b2180 <DllMain>
+   29a1b1207:	call   29a1b21b0 <DllMain>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:195
    29a1b120c:	mov    %rdi,%r8
    29a1b120f:	mov    %ebx,%edx
    29a1b1211:	mov    %rsi,%rcx
-   29a1b1214:	call   29a1b2170 <DllEntryPoint>
+   29a1b1214:	call   29a1b21a0 <DllEntryPoint>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:196
    29a1b1219:	mov    %rdi,%r8
    29a1b121c:	mov    %ebx,%edx
    29a1b121e:	mov    %rsi,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:195
    29a1b1221:	mov    %eax,%r12d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:196
@@ -2179,15 +2190,15 @@
    29a1b1242:	pop    %rsi
    29a1b1243:	pop    %rdi
    29a1b1244:	pop    %rbp
    29a1b1245:	pop    %r12
    29a1b1247:	ret
    29a1b1248:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:170
-   29a1b1250:	call   29a1b1750 <_pei386_runtime_relocator>
+   29a1b1250:	call   29a1b1780 <_pei386_runtime_relocator>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:171
    29a1b1255:	lea    -0x1(%rbx),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:173
    29a1b1258:	mov    %rdi,%r8
    29a1b125b:	mov    %ebx,%edx
    29a1b125d:	mov    %rsi,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:171
@@ -2198,32 +2209,32 @@
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:174
    29a1b126a:	test   %eax,%eax
    29a1b126c:	je     29a1b1230 <__DllMainCRTStartup+0x60>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:176
    29a1b126e:	mov    %rdi,%r8
    29a1b1271:	mov    %ebx,%edx
    29a1b1273:	mov    %rsi,%rcx
-   29a1b1276:	call   29a1b2170 <DllEntryPoint>
+   29a1b1276:	call   29a1b21a0 <DllEntryPoint>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:177
    29a1b127b:	test   %eax,%eax
    29a1b127d:	je     29a1b12b8 <__DllMainCRTStartup+0xe8>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:184
    29a1b127f:	cmp    $0x1,%ebx
    29a1b1282:	je     29a1b12d8 <__DllMainCRTStartup+0x108>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:186
    29a1b1284:	mov    %rdi,%r8
    29a1b1287:	mov    $0x2,%edx
    29a1b128c:	mov    %rsi,%rcx
-   29a1b128f:	call   29a1b2180 <DllMain>
+   29a1b128f:	call   29a1b21b0 <DllMain>
    29a1b1294:	mov    %eax,%r12d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:193
    29a1b1297:	jmp    29a1b1233 <__DllMainCRTStartup+0x63>
    29a1b1299:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:186
-   29a1b12a0:	call   29a1b2180 <DllMain>
+   29a1b12a0:	call   29a1b21b0 <DllMain>
    29a1b12a5:	mov    %eax,%r12d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:193
    29a1b12a8:	cmp    $0x3,%ebx
    29a1b12ab:	jne    29a1b1233 <__DllMainCRTStartup+0x63>
    29a1b12ad:	jmp    29a1b120c <__DllMainCRTStartup+0x3c>
    29a1b12b2:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:179
@@ -2233,34 +2244,34 @@
    29a1b12c1:	mov    %rdi,%r8
    29a1b12c4:	xor    %edx,%edx
    29a1b12c6:	mov    %rsi,%rcx
    29a1b12c9:	call   29a1b1010 <_CRT_INIT>
    29a1b12ce:	jmp    29a1b1230 <__DllMainCRTStartup+0x60>
    29a1b12d3:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:185
-   29a1b12d8:	call   29a1b1480 <__main>
+   29a1b12d8:	call   29a1b14b0 <__main>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:186
    29a1b12dd:	mov    %rdi,%r8
    29a1b12e0:	mov    $0x1,%edx
    29a1b12e5:	mov    %rsi,%rcx
-   29a1b12e8:	call   29a1b2180 <DllMain>
+   29a1b12e8:	call   29a1b21b0 <DllMain>
    29a1b12ed:	mov    %eax,%r12d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:187
    29a1b12f0:	test   %eax,%eax
    29a1b12f2:	jne    29a1b1233 <__DllMainCRTStartup+0x63>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:189
    29a1b12f8:	mov    %rdi,%r8
    29a1b12fb:	xor    %edx,%edx
    29a1b12fd:	mov    %rsi,%rcx
-   29a1b1300:	call   29a1b2180 <DllMain>
+   29a1b1300:	call   29a1b21b0 <DllMain>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:190
    29a1b1305:	mov    %rdi,%r8
    29a1b1308:	xor    %edx,%edx
    29a1b130a:	mov    %rsi,%rcx
-   29a1b130d:	call   29a1b2170 <DllEntryPoint>
+   29a1b130d:	call   29a1b21a0 <DllEntryPoint>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:191
    29a1b1312:	mov    %rdi,%r8
    29a1b1315:	xor    %edx,%edx
    29a1b1317:	mov    %rsi,%rcx
    29a1b131a:	call   29a1b1010 <_CRT_INIT>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:193
    29a1b131f:	jmp    29a1b1233 <__DllMainCRTStartup+0x63>
@@ -2279,15 +2290,15 @@
 
 000000029a1b1350 <atexit>:
 atexit():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:206
    29a1b1350:	mov    %rcx,%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:207
    29a1b1353:	lea    0x5ca6(%rip),%rcx        # 29a1b7000 <__bss_start__>
-   29a1b135a:	jmp    29a1b2498 <_register_onexit_function>
+   29a1b135a:	jmp    29a1b24d8 <_register_onexit_function>
    29a1b135f:	nop
 
 000000029a1b1360 <__gcc_register_frame>:
    29a1b1360:	lea    0x9(%rip),%rcx        # 29a1b1370 <__gcc_deregister_frame>
    29a1b1367:	jmp    29a1b1350 <atexit>
    29a1b136c:	nopl   0x0(%rax)
 
@@ -2308,2165 +2319,2185 @@
    29a1b137d:	nop
    29a1b137e:	nop
    29a1b137f:	nop
 
 000000029a1b1380 <init>:
    29a1b1380:	push   %rbp
    29a1b1381:	mov    %rsp,%rbp
-   29a1b1384:	nop
-   29a1b1385:	pop    %rbp
-   29a1b1386:	ret
-
-000000029a1b1387 <isInputReady>:
-   29a1b1387:	push   %rbp
-   29a1b1388:	mov    %rsp,%rbp
-   29a1b138b:	sub    $0x20,%rsp
-   29a1b138f:	call   29a1b2418 <kbhit>
-   29a1b1394:	add    $0x20,%rsp
-   29a1b1398:	pop    %rbp
-   29a1b1399:	ret
-
-000000029a1b139a <getCharacter>:
-   29a1b139a:	push   %rbp
-   29a1b139b:	mov    %rsp,%rbp
-   29a1b139e:	sub    $0x30,%rsp
-   29a1b13a2:	call   29a1b24e0 <getch>
-   29a1b13a7:	mov    %al,-0x1(%rbp)
-   29a1b13aa:	movsbl -0x1(%rbp),%eax
-   29a1b13ae:	mov    %eax,%ecx
-   29a1b13b0:	call   29a1b2428 <putchar>
-   29a1b13b5:	movzbl -0x1(%rbp),%eax
-   29a1b13b9:	add    $0x30,%rsp
-   29a1b13bd:	pop    %rbp
-   29a1b13be:	ret
-
-000000029a1b13bf <stop>:
-   29a1b13bf:	push   %rbp
-   29a1b13c0:	mov    %rsp,%rbp
-   29a1b13c3:	nop
-   29a1b13c4:	pop    %rbp
-   29a1b13c5:	ret
-   29a1b13c6:	nop
-   29a1b13c7:	nop
-   29a1b13c8:	nop
-   29a1b13c9:	nop
-   29a1b13ca:	nop
-   29a1b13cb:	nop
-   29a1b13cc:	nop
-   29a1b13cd:	nop
-   29a1b13ce:	nop
-   29a1b13cf:	nop
+   29a1b1384:	sub    $0x20,%rsp
+   29a1b1388:	mov    $0x0,%ecx
+   29a1b138d:	mov    0x7fd4(%rip),%rax        # 29a1b9368 <__imp___acrt_iob_func>
+   29a1b1394:	call   *%rax
+   29a1b1396:	mov    %rax,%rcx
+   29a1b1399:	call   29a1b2450 <fflush>
+   29a1b139e:	nop
+   29a1b139f:	add    $0x20,%rsp
+   29a1b13a3:	pop    %rbp
+   29a1b13a4:	ret
+
+000000029a1b13a5 <isInputReady>:
+   29a1b13a5:	push   %rbp
+   29a1b13a6:	mov    %rsp,%rbp
+   29a1b13a9:	sub    $0x20,%rsp
+   29a1b13ad:	call   29a1b2448 <kbhit>
+   29a1b13b2:	add    $0x20,%rsp
+   29a1b13b6:	pop    %rbp
+   29a1b13b7:	ret
+
+000000029a1b13b8 <getCharacter>:
+   29a1b13b8:	push   %rbp
+   29a1b13b9:	mov    %rsp,%rbp
+   29a1b13bc:	sub    $0x30,%rsp
+   29a1b13c0:	call   29a1b2520 <getch>
+   29a1b13c5:	mov    %eax,-0x4(%rbp)
+   29a1b13c8:	mov    -0x4(%rbp),%eax
+   29a1b13cb:	cmp    $0xd,%al
+   29a1b13cd:	jne    29a1b13d6 <getCharacter+0x1e>
+   29a1b13cf:	movl   $0xa,-0x4(%rbp)
+   29a1b13d6:	mov    -0x4(%rbp),%eax
+   29a1b13d9:	movsbl %al,%eax
+   29a1b13dc:	mov    %eax,%ecx
+   29a1b13de:	call   29a1b2460 <putchar>
+   29a1b13e3:	mov    -0x4(%rbp),%eax
+   29a1b13e6:	add    $0x30,%rsp
+   29a1b13ea:	pop    %rbp
+   29a1b13eb:	ret
+
+000000029a1b13ec <stop>:
+   29a1b13ec:	push   %rbp
+   29a1b13ed:	mov    %rsp,%rbp
+   29a1b13f0:	nop
+   29a1b13f1:	pop    %rbp
+   29a1b13f2:	ret
+   29a1b13f3:	nop
+   29a1b13f4:	nop
+   29a1b13f5:	nop
+   29a1b13f6:	nop
+   29a1b13f7:	nop
+   29a1b13f8:	nop
+   29a1b13f9:	nop
+   29a1b13fa:	nop
+   29a1b13fb:	nop
+   29a1b13fc:	nop
+   29a1b13fd:	nop
+   29a1b13fe:	nop
+   29a1b13ff:	nop
 
-000000029a1b13d0 <__do_global_dtors>:
+000000029a1b1400 <__do_global_dtors>:
 __do_global_dtors():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:21
-   29a1b13d0:	sub    $0x28,%rsp
+   29a1b1400:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:24
-   29a1b13d4:	mov    0x1c35(%rip),%rax        # 29a1b3010 <p.0>
-   29a1b13db:	mov    (%rax),%rax
-   29a1b13de:	test   %rax,%rax
-   29a1b13e1:	je     29a1b1405 <__do_global_dtors+0x35>
-   29a1b13e3:	nopl   0x0(%rax,%rax,1)
+   29a1b1404:	mov    0x1c05(%rip),%rax        # 29a1b3010 <p.0>
+   29a1b140b:	mov    (%rax),%rax
+   29a1b140e:	test   %rax,%rax
+   29a1b1411:	je     29a1b1435 <__do_global_dtors+0x35>
+   29a1b1413:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:26
-   29a1b13e8:	call   *%rax
+   29a1b1418:	call   *%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:27
-   29a1b13ea:	mov    0x1c1f(%rip),%rax        # 29a1b3010 <p.0>
-   29a1b13f1:	lea    0x8(%rax),%rdx
+   29a1b141a:	mov    0x1bef(%rip),%rax        # 29a1b3010 <p.0>
+   29a1b1421:	lea    0x8(%rax),%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:24
-   29a1b13f5:	mov    0x8(%rax),%rax
+   29a1b1425:	mov    0x8(%rax),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:27
-   29a1b13f9:	mov    %rdx,0x1c10(%rip)        # 29a1b3010 <p.0>
+   29a1b1429:	mov    %rdx,0x1be0(%rip)        # 29a1b3010 <p.0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:24
-   29a1b1400:	test   %rax,%rax
-   29a1b1403:	jne    29a1b13e8 <__do_global_dtors+0x18>
+   29a1b1430:	test   %rax,%rax
+   29a1b1433:	jne    29a1b1418 <__do_global_dtors+0x18>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:29
-   29a1b1405:	add    $0x28,%rsp
-   29a1b1409:	ret
-   29a1b140a:	nopw   0x0(%rax,%rax,1)
+   29a1b1435:	add    $0x28,%rsp
+   29a1b1439:	ret
+   29a1b143a:	nopw   0x0(%rax,%rax,1)
 
-000000029a1b1410 <__do_global_ctors>:
+000000029a1b1440 <__do_global_ctors>:
 __do_global_ctors():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:33
-   29a1b1410:	push   %rsi
-   29a1b1411:	push   %rbx
-   29a1b1412:	sub    $0x28,%rsp
+   29a1b1440:	push   %rsi
+   29a1b1441:	push   %rbx
+   29a1b1442:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:34
-   29a1b1416:	mov    0x2dd3(%rip),%rdx        # 29a1b41f0 <.refptr.__CTOR_LIST__>
-   29a1b141d:	mov    (%rdx),%rax
-   29a1b1420:	mov    %eax,%ecx
+   29a1b1446:	mov    0x2da3(%rip),%rdx        # 29a1b41f0 <.refptr.__CTOR_LIST__>
+   29a1b144d:	mov    (%rdx),%rax
+   29a1b1450:	mov    %eax,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:37
-   29a1b1422:	cmp    $0xffffffff,%eax
-   29a1b1425:	je     29a1b1460 <__do_global_ctors+0x50>
+   29a1b1452:	cmp    $0xffffffff,%eax
+   29a1b1455:	je     29a1b1490 <__do_global_ctors+0x50>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:42
-   29a1b1427:	test   %ecx,%ecx
-   29a1b1429:	je     29a1b144b <__do_global_ctors+0x3b>
-   29a1b142b:	mov    %ecx,%eax
-   29a1b142d:	sub    $0x1,%ecx
-   29a1b1430:	lea    (%rdx,%rax,8),%rbx
-   29a1b1434:	sub    %rcx,%rax
-   29a1b1437:	lea    -0x8(%rdx,%rax,8),%rsi
-   29a1b143c:	nopl   0x0(%rax)
+   29a1b1457:	test   %ecx,%ecx
+   29a1b1459:	je     29a1b147b <__do_global_ctors+0x3b>
+   29a1b145b:	mov    %ecx,%eax
+   29a1b145d:	sub    $0x1,%ecx
+   29a1b1460:	lea    (%rdx,%rax,8),%rbx
+   29a1b1464:	sub    %rcx,%rax
+   29a1b1467:	lea    -0x8(%rdx,%rax,8),%rsi
+   29a1b146c:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:44
-   29a1b1440:	call   *(%rbx)
+   29a1b1470:	call   *(%rbx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:42
-   29a1b1442:	sub    $0x8,%rbx
-   29a1b1446:	cmp    %rsi,%rbx
-   29a1b1449:	jne    29a1b1440 <__do_global_ctors+0x30>
+   29a1b1472:	sub    $0x8,%rbx
+   29a1b1476:	cmp    %rsi,%rbx
+   29a1b1479:	jne    29a1b1470 <__do_global_ctors+0x30>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:47
-   29a1b144b:	lea    -0x82(%rip),%rcx        # 29a1b13d0 <__do_global_dtors>
+   29a1b147b:	lea    -0x82(%rip),%rcx        # 29a1b1400 <__do_global_dtors>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:48
-   29a1b1452:	add    $0x28,%rsp
-   29a1b1456:	pop    %rbx
-   29a1b1457:	pop    %rsi
+   29a1b1482:	add    $0x28,%rsp
+   29a1b1486:	pop    %rbx
+   29a1b1487:	pop    %rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:47
-   29a1b1458:	jmp    29a1b1350 <atexit>
-   29a1b145d:	nopl   (%rax)
+   29a1b1488:	jmp    29a1b1350 <atexit>
+   29a1b148d:	nopl   (%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:39
-   29a1b1460:	xor    %eax,%eax
-   29a1b1462:	nopw   0x0(%rax,%rax,1)
-   29a1b1468:	lea    0x1(%rax),%r8d
-   29a1b146c:	mov    %eax,%ecx
-   29a1b146e:	cmpq   $0x0,(%rdx,%r8,8)
-   29a1b1473:	mov    %r8,%rax
-   29a1b1476:	jne    29a1b1468 <__do_global_ctors+0x58>
-   29a1b1478:	jmp    29a1b1427 <__do_global_ctors+0x17>
-   29a1b147a:	nopw   0x0(%rax,%rax,1)
+   29a1b1490:	xor    %eax,%eax
+   29a1b1492:	nopw   0x0(%rax,%rax,1)
+   29a1b1498:	lea    0x1(%rax),%r8d
+   29a1b149c:	mov    %eax,%ecx
+   29a1b149e:	cmpq   $0x0,(%rdx,%r8,8)
+   29a1b14a3:	mov    %r8,%rax
+   29a1b14a6:	jne    29a1b1498 <__do_global_ctors+0x58>
+   29a1b14a8:	jmp    29a1b1457 <__do_global_ctors+0x17>
+   29a1b14aa:	nopw   0x0(%rax,%rax,1)
 
-000000029a1b1480 <__main>:
+000000029a1b14b0 <__main>:
 __main():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:55
-   29a1b1480:	mov    0x5b9a(%rip),%eax        # 29a1b7020 <initialized>
-   29a1b1486:	test   %eax,%eax
-   29a1b1488:	je     29a1b1490 <__main+0x10>
+   29a1b14b0:	mov    0x5b6a(%rip),%eax        # 29a1b7020 <initialized>
+   29a1b14b6:	test   %eax,%eax
+   29a1b14b8:	je     29a1b14c0 <__main+0x10>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:60
-   29a1b148a:	ret
-   29a1b148b:	nopl   0x0(%rax,%rax,1)
+   29a1b14ba:	ret
+   29a1b14bb:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:57
-   29a1b1490:	movl   $0x1,0x5b86(%rip)        # 29a1b7020 <initialized>
+   29a1b14c0:	movl   $0x1,0x5b56(%rip)        # 29a1b7020 <initialized>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:58
-   29a1b149a:	jmp    29a1b1410 <__do_global_ctors>
-   29a1b149f:	nop
+   29a1b14ca:	jmp    29a1b1440 <__do_global_ctors>
+   29a1b14cf:	nop
 
-000000029a1b14a0 <__dyn_tls_dtor>:
+000000029a1b14d0 <__dyn_tls_dtor>:
 __dyn_tls_dtor():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:138
-   29a1b14a0:	sub    $0x28,%rsp
+   29a1b14d0:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:144
-   29a1b14a4:	cmp    $0x3,%edx
-   29a1b14a7:	je     29a1b14c0 <__dyn_tls_dtor+0x20>
-   29a1b14a9:	test   %edx,%edx
-   29a1b14ab:	je     29a1b14c0 <__dyn_tls_dtor+0x20>
+   29a1b14d4:	cmp    $0x3,%edx
+   29a1b14d7:	je     29a1b14f0 <__dyn_tls_dtor+0x20>
+   29a1b14d9:	test   %edx,%edx
+   29a1b14db:	je     29a1b14f0 <__dyn_tls_dtor+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:169
-   29a1b14ad:	mov    $0x1,%eax
-   29a1b14b2:	add    $0x28,%rsp
-   29a1b14b6:	ret
-   29a1b14b7:	nopw   0x0(%rax,%rax,1)
+   29a1b14dd:	mov    $0x1,%eax
+   29a1b14e2:	add    $0x28,%rsp
+   29a1b14e6:	ret
+   29a1b14e7:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:167
-   29a1b14c0:	call   29a1b1c20 <__mingw_TLScallback>
+   29a1b14f0:	call   29a1b1c50 <__mingw_TLScallback>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:169
-   29a1b14c5:	mov    $0x1,%eax
-   29a1b14ca:	add    $0x28,%rsp
-   29a1b14ce:	ret
-   29a1b14cf:	nop
+   29a1b14f5:	mov    $0x1,%eax
+   29a1b14fa:	add    $0x28,%rsp
+   29a1b14fe:	ret
+   29a1b14ff:	nop
 
-000000029a1b14d0 <__dyn_tls_init>:
+000000029a1b1500 <__dyn_tls_init>:
 __dyn_tls_init():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:78
-   29a1b14d0:	push   %rsi
-   29a1b14d1:	push   %rbx
-   29a1b14d2:	sub    $0x28,%rsp
+   29a1b1500:	push   %rsi
+   29a1b1501:	push   %rbx
+   29a1b1502:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:83
-   29a1b14d6:	mov    0x2d03(%rip),%rax        # 29a1b41e0 <.refptr._CRT_MT>
-   29a1b14dd:	cmpl   $0x2,(%rax)
-   29a1b14e0:	je     29a1b14e8 <__dyn_tls_init+0x18>
+   29a1b1506:	mov    0x2cd3(%rip),%rax        # 29a1b41e0 <.refptr._CRT_MT>
+   29a1b150d:	cmpl   $0x2,(%rax)
+   29a1b1510:	je     29a1b1518 <__dyn_tls_init+0x18>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:84
-   29a1b14e2:	movl   $0x2,(%rax)
+   29a1b1512:	movl   $0x2,(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:86
-   29a1b14e8:	cmp    $0x2,%edx
-   29a1b14eb:	je     29a1b1500 <__dyn_tls_init+0x30>
+   29a1b1518:	cmp    $0x2,%edx
+   29a1b151b:	je     29a1b1530 <__dyn_tls_init+0x30>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:88
-   29a1b14ed:	cmp    $0x1,%edx
-   29a1b14f0:	je     29a1b1540 <__dyn_tls_init+0x70>
+   29a1b151d:	cmp    $0x1,%edx
+   29a1b1520:	je     29a1b1570 <__dyn_tls_init+0x70>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:102
-   29a1b14f2:	mov    $0x1,%eax
-   29a1b14f7:	add    $0x28,%rsp
-   29a1b14fb:	pop    %rbx
-   29a1b14fc:	pop    %rsi
-   29a1b14fd:	ret
-   29a1b14fe:	xchg   %ax,%ax
+   29a1b1522:	mov    $0x1,%eax
+   29a1b1527:	add    $0x28,%rsp
+   29a1b152b:	pop    %rbx
+   29a1b152c:	pop    %rsi
+   29a1b152d:	ret
+   29a1b152e:	xchg   %ax,%ax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:94
-   29a1b1500:	lea    0x8b49(%rip),%rbx        # 29a1ba050 <__xd_z>
+   29a1b1530:	lea    0x8b19(%rip),%rbx        # 29a1ba050 <__xd_z>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:95
-   29a1b1507:	lea    0x8b42(%rip),%rsi        # 29a1ba050 <__xd_z>
-   29a1b150e:	cmp    %rsi,%rbx
-   29a1b1511:	je     29a1b14f2 <__dyn_tls_init+0x22>
-   29a1b1513:	nopl   0x0(%rax,%rax,1)
+   29a1b1537:	lea    0x8b12(%rip),%rsi        # 29a1ba050 <__xd_z>
+   29a1b153e:	cmp    %rsi,%rbx
+   29a1b1541:	je     29a1b1522 <__dyn_tls_init+0x22>
+   29a1b1543:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:98
-   29a1b1518:	mov    (%rbx),%rax
-   29a1b151b:	test   %rax,%rax
-   29a1b151e:	je     29a1b1522 <__dyn_tls_init+0x52>
+   29a1b1548:	mov    (%rbx),%rax
+   29a1b154b:	test   %rax,%rax
+   29a1b154e:	je     29a1b1552 <__dyn_tls_init+0x52>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:99
-   29a1b1520:	call   *%rax
+   29a1b1550:	call   *%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:95
-   29a1b1522:	add    $0x8,%rbx
-   29a1b1526:	cmp    %rsi,%rbx
-   29a1b1529:	jne    29a1b1518 <__dyn_tls_init+0x48>
+   29a1b1552:	add    $0x8,%rbx
+   29a1b1556:	cmp    %rsi,%rbx
+   29a1b1559:	jne    29a1b1548 <__dyn_tls_init+0x48>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:102
-   29a1b152b:	mov    $0x1,%eax
-   29a1b1530:	add    $0x28,%rsp
-   29a1b1534:	pop    %rbx
-   29a1b1535:	pop    %rsi
-   29a1b1536:	ret
-   29a1b1537:	nopw   0x0(%rax,%rax,1)
+   29a1b155b:	mov    $0x1,%eax
+   29a1b1560:	add    $0x28,%rsp
+   29a1b1564:	pop    %rbx
+   29a1b1565:	pop    %rsi
+   29a1b1566:	ret
+   29a1b1567:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:89
-   29a1b1540:	call   29a1b1c20 <__mingw_TLScallback>
+   29a1b1570:	call   29a1b1c50 <__mingw_TLScallback>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:102
-   29a1b1545:	mov    $0x1,%eax
-   29a1b154a:	add    $0x28,%rsp
-   29a1b154e:	pop    %rbx
-   29a1b154f:	pop    %rsi
-   29a1b1550:	ret
-   29a1b1551:	data16 cs nopw 0x0(%rax,%rax,1)
-   29a1b155c:	nopl   0x0(%rax)
+   29a1b1575:	mov    $0x1,%eax
+   29a1b157a:	add    $0x28,%rsp
+   29a1b157e:	pop    %rbx
+   29a1b157f:	pop    %rsi
+   29a1b1580:	ret
+   29a1b1581:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b158c:	nopl   0x0(%rax)
 
-000000029a1b1560 <__tlregdtor>:
+000000029a1b1590 <__tlregdtor>:
 __tlregdtor():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:134
-   29a1b1560:	xor    %eax,%eax
-   29a1b1562:	ret
-   29a1b1563:	nop
-   29a1b1564:	nop
-   29a1b1565:	nop
-   29a1b1566:	nop
-   29a1b1567:	nop
-   29a1b1568:	nop
-   29a1b1569:	nop
-   29a1b156a:	nop
-   29a1b156b:	nop
-   29a1b156c:	nop
-   29a1b156d:	nop
-   29a1b156e:	nop
-   29a1b156f:	nop
+   29a1b1590:	xor    %eax,%eax
+   29a1b1592:	ret
+   29a1b1593:	nop
+   29a1b1594:	nop
+   29a1b1595:	nop
+   29a1b1596:	nop
+   29a1b1597:	nop
+   29a1b1598:	nop
+   29a1b1599:	nop
+   29a1b159a:	nop
+   29a1b159b:	nop
+   29a1b159c:	nop
+   29a1b159d:	nop
+   29a1b159e:	nop
+   29a1b159f:	nop
 
-000000029a1b1570 <__report_error>:
+000000029a1b15a0 <__report_error>:
 __report_error():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:85
-   29a1b1570:	push   %rsi
-   29a1b1571:	push   %rbx
-   29a1b1572:	sub    $0x38,%rsp
-   29a1b1576:	mov    %rcx,%rbx
+   29a1b15a0:	push   %rsi
+   29a1b15a1:	push   %rbx
+   29a1b15a2:	sub    $0x38,%rsp
+   29a1b15a6:	mov    %rcx,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:148
-   29a1b1579:	lea    0x58(%rsp),%rax
+   29a1b15a9:	lea    0x58(%rsp),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:150
-   29a1b157e:	mov    $0x2,%ecx
+   29a1b15ae:	mov    $0x2,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:85
-   29a1b1583:	mov    %rdx,0x58(%rsp)
-   29a1b1588:	mov    %r8,0x60(%rsp)
-   29a1b158d:	mov    %r9,0x68(%rsp)
+   29a1b15b3:	mov    %rdx,0x58(%rsp)
+   29a1b15b8:	mov    %r8,0x60(%rsp)
+   29a1b15bd:	mov    %r9,0x68(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:148
-   29a1b1592:	mov    %rax,0x28(%rsp)
+   29a1b15c2:	mov    %rax,0x28(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:150
-   29a1b1597:	call   29a1b2400 <__acrt_iob_func>
-   29a1b159c:	mov    $0x1b,%r8d
-   29a1b15a2:	mov    $0x1,%edx
-   29a1b15a7:	lea    0x2ab2(%rip),%rcx        # 29a1b4060 <.rdata>
-   29a1b15ae:	mov    %rax,%r9
-   29a1b15b1:	call   29a1b2420 <fwrite>
+   29a1b15c7:	call   29a1b2430 <__acrt_iob_func>
+   29a1b15cc:	mov    $0x1b,%r8d
+   29a1b15d2:	mov    $0x1,%edx
+   29a1b15d7:	lea    0x2a82(%rip),%rcx        # 29a1b4060 <.rdata>
+   29a1b15de:	mov    %rax,%r9
+   29a1b15e1:	call   29a1b2458 <fwrite>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:151
-   29a1b15b6:	mov    0x28(%rsp),%rsi
-   29a1b15bb:	mov    $0x2,%ecx
-   29a1b15c0:	call   29a1b2400 <__acrt_iob_func>
-   29a1b15c5:	mov    %rbx,%rdx
-   29a1b15c8:	mov    %rax,%rcx
-   29a1b15cb:	mov    %rsi,%r8
-   29a1b15ce:	call   29a1b2190 <vfprintf>
+   29a1b15e6:	mov    0x28(%rsp),%rsi
+   29a1b15eb:	mov    $0x2,%ecx
+   29a1b15f0:	call   29a1b2430 <__acrt_iob_func>
+   29a1b15f5:	mov    %rbx,%rdx
+   29a1b15f8:	mov    %rax,%rcx
+   29a1b15fb:	mov    %rsi,%r8
+   29a1b15fe:	call   29a1b21c0 <vfprintf>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:157
-   29a1b15d3:	call   29a1b24a0 <abort>
-   29a1b15d8:	nop
-   29a1b15d9:	nopl   0x0(%rax)
+   29a1b1603:	call   29a1b24e0 <abort>
+   29a1b1608:	nop
+   29a1b1609:	nopl   0x0(%rax)
 
-000000029a1b15e0 <mark_section_writable>:
+000000029a1b1610 <mark_section_writable>:
 mark_section_writable():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:184
-   29a1b15e0:	push   %rdi
-   29a1b15e1:	push   %rsi
-   29a1b15e2:	push   %rbx
-   29a1b15e3:	sub    $0x50,%rsp
+   29a1b1610:	push   %rdi
+   29a1b1611:	push   %rsi
+   29a1b1612:	push   %rbx
+   29a1b1613:	sub    $0x50,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:189
-   29a1b15e7:	movslq 0x5a76(%rip),%rsi        # 29a1b7064 <maxSections>
+   29a1b1617:	movslq 0x5a46(%rip),%rsi        # 29a1b7064 <maxSections>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:184
-   29a1b15ee:	mov    %rcx,%rbx
+   29a1b161e:	mov    %rcx,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:189
-   29a1b15f1:	test   %esi,%esi
-   29a1b15f3:	jle    29a1b1710 <mark_section_writable+0x130>
-   29a1b15f9:	mov    0x5a68(%rip),%rax        # 29a1b7068 <the_secs>
-   29a1b1600:	xor    %r9d,%r9d
-   29a1b1603:	add    $0x18,%rax
-   29a1b1607:	nopw   0x0(%rax,%rax,1)
+   29a1b1621:	test   %esi,%esi
+   29a1b1623:	jle    29a1b1740 <mark_section_writable+0x130>
+   29a1b1629:	mov    0x5a38(%rip),%rax        # 29a1b7068 <the_secs>
+   29a1b1630:	xor    %r9d,%r9d
+   29a1b1633:	add    $0x18,%rax
+   29a1b1637:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:191
-   29a1b1610:	mov    (%rax),%r8
-   29a1b1613:	cmp    %r8,%rbx
-   29a1b1616:	jb     29a1b162b <mark_section_writable+0x4b>
+   29a1b1640:	mov    (%rax),%r8
+   29a1b1643:	cmp    %r8,%rbx
+   29a1b1646:	jb     29a1b165b <mark_section_writable+0x4b>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:192
-   29a1b1618:	mov    0x8(%rax),%rdx
-   29a1b161c:	mov    0x8(%rdx),%edx
-   29a1b161f:	add    %rdx,%r8
-   29a1b1622:	cmp    %r8,%rbx
-   29a1b1625:	jb     29a1b16b5 <mark_section_writable+0xd5>
+   29a1b1648:	mov    0x8(%rax),%rdx
+   29a1b164c:	mov    0x8(%rdx),%edx
+   29a1b164f:	add    %rdx,%r8
+   29a1b1652:	cmp    %r8,%rbx
+   29a1b1655:	jb     29a1b16e5 <mark_section_writable+0xd5>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:189
-   29a1b162b:	add    $0x1,%r9d
-   29a1b162f:	add    $0x28,%rax
-   29a1b1633:	cmp    %esi,%r9d
-   29a1b1636:	jne    29a1b1610 <mark_section_writable+0x30>
+   29a1b165b:	add    $0x1,%r9d
+   29a1b165f:	add    $0x28,%rax
+   29a1b1663:	cmp    %esi,%r9d
+   29a1b1666:	jne    29a1b1640 <mark_section_writable+0x30>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:195
-   29a1b1638:	mov    %rbx,%rcx
-   29a1b163b:	call   29a1b1e40 <__mingw_GetSectionForAddress>
-   29a1b1640:	mov    %rax,%rdi
+   29a1b1668:	mov    %rbx,%rcx
+   29a1b166b:	call   29a1b1e70 <__mingw_GetSectionForAddress>
+   29a1b1670:	mov    %rax,%rdi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:196
-   29a1b1643:	test   %rax,%rax
-   29a1b1646:	je     29a1b1732 <mark_section_writable+0x152>
+   29a1b1673:	test   %rax,%rax
+   29a1b1676:	je     29a1b1762 <mark_section_writable+0x152>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:201
-   29a1b164c:	mov    0x5a15(%rip),%rax        # 29a1b7068 <the_secs>
-   29a1b1653:	lea    (%rsi,%rsi,4),%rbx
-   29a1b1657:	shl    $0x3,%rbx
-   29a1b165b:	add    %rbx,%rax
-   29a1b165e:	mov    %rdi,0x20(%rax)
+   29a1b167c:	mov    0x59e5(%rip),%rax        # 29a1b7068 <the_secs>
+   29a1b1683:	lea    (%rsi,%rsi,4),%rbx
+   29a1b1687:	shl    $0x3,%rbx
+   29a1b168b:	add    %rbx,%rax
+   29a1b168e:	mov    %rdi,0x20(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:202
-   29a1b1662:	movl   $0x0,(%rax)
+   29a1b1692:	movl   $0x0,(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:203
-   29a1b1668:	call   29a1b1f80 <_GetPEImageBase>
-   29a1b166d:	mov    0xc(%rdi),%edx
+   29a1b1698:	call   29a1b1fb0 <_GetPEImageBase>
+   29a1b169d:	mov    0xc(%rdi),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:205
-   29a1b1670:	mov    $0x30,%r8d
+   29a1b16a0:	mov    $0x30,%r8d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:203
-   29a1b1676:	lea    (%rax,%rdx,1),%rcx
-   29a1b167a:	mov    0x59e7(%rip),%rax        # 29a1b7068 <the_secs>
+   29a1b16a6:	lea    (%rax,%rdx,1),%rcx
+   29a1b16aa:	mov    0x59b7(%rip),%rax        # 29a1b7068 <the_secs>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:205
-   29a1b1681:	lea    0x20(%rsp),%rdx
+   29a1b16b1:	lea    0x20(%rsp),%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:203
-   29a1b1686:	mov    %rcx,0x18(%rax,%rbx,1)
+   29a1b16b6:	mov    %rcx,0x18(%rax,%rbx,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:205
-   29a1b168b:	call   *0x7bf7(%rip)        # 29a1b9288 <__imp_VirtualQuery>
-   29a1b1691:	test   %rax,%rax
-   29a1b1694:	je     29a1b1717 <mark_section_writable+0x137>
+   29a1b16bb:	call   *0x7bcf(%rip)        # 29a1b9290 <__imp_VirtualQuery>
+   29a1b16c1:	test   %rax,%rax
+   29a1b16c4:	je     29a1b1747 <mark_section_writable+0x137>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:212
-   29a1b169a:	mov    0x44(%rsp),%eax
-   29a1b169e:	lea    -0x4(%rax),%edx
+   29a1b16ca:	mov    0x44(%rsp),%eax
+   29a1b16ce:	lea    -0x4(%rax),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:213
-   29a1b16a1:	and    $0xfffffffb,%edx
-   29a1b16a4:	je     29a1b16ae <mark_section_writable+0xce>
+   29a1b16d1:	and    $0xfffffffb,%edx
+   29a1b16d4:	je     29a1b16de <mark_section_writable+0xce>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:212
-   29a1b16a6:	lea    -0x40(%rax),%edx
+   29a1b16d6:	lea    -0x40(%rax),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:213
-   29a1b16a9:	and    $0xffffffbf,%edx
-   29a1b16ac:	jne    29a1b16c0 <mark_section_writable+0xe0>
+   29a1b16d9:	and    $0xffffffbf,%edx
+   29a1b16dc:	jne    29a1b16f0 <mark_section_writable+0xe0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:228
-   29a1b16ae:	addl   $0x1,0x59af(%rip)        # 29a1b7064 <maxSections>
+   29a1b16de:	addl   $0x1,0x597f(%rip)        # 29a1b7064 <maxSections>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:230
-   29a1b16b5:	add    $0x50,%rsp
-   29a1b16b9:	pop    %rbx
-   29a1b16ba:	pop    %rsi
-   29a1b16bb:	pop    %rdi
-   29a1b16bc:	ret
-   29a1b16bd:	nopl   (%rax)
+   29a1b16e5:	add    $0x50,%rsp
+   29a1b16e9:	pop    %rbx
+   29a1b16ea:	pop    %rsi
+   29a1b16eb:	pop    %rdi
+   29a1b16ec:	ret
+   29a1b16ed:	nopl   (%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:217
-   29a1b16c0:	cmp    $0x2,%eax
+   29a1b16f0:	cmp    $0x2,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:220
-   29a1b16c3:	mov    0x20(%rsp),%rcx
+   29a1b16f3:	mov    0x20(%rsp),%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:221
-   29a1b16c8:	mov    0x38(%rsp),%rdx
+   29a1b16f8:	mov    0x38(%rsp),%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:217
-   29a1b16cd:	mov    $0x40,%r8d
-   29a1b16d3:	mov    $0x4,%eax
-   29a1b16d8:	cmove  %eax,%r8d
+   29a1b16fd:	mov    $0x40,%r8d
+   29a1b1703:	mov    $0x4,%eax
+   29a1b1708:	cmove  %eax,%r8d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:220
-   29a1b16dc:	add    0x5985(%rip),%rbx        # 29a1b7068 <the_secs>
-   29a1b16e3:	mov    %rcx,0x8(%rbx)
-   29a1b16e7:	mov    %rbx,%r9
+   29a1b170c:	add    0x5955(%rip),%rbx        # 29a1b7068 <the_secs>
+   29a1b1713:	mov    %rcx,0x8(%rbx)
+   29a1b1717:	mov    %rbx,%r9
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:221
-   29a1b16ea:	mov    %rdx,0x10(%rbx)
+   29a1b171a:	mov    %rdx,0x10(%rbx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:222
-   29a1b16ee:	call   *0x7b8c(%rip)        # 29a1b9280 <__imp_VirtualProtect>
-   29a1b16f4:	test   %eax,%eax
-   29a1b16f6:	jne    29a1b16ae <mark_section_writable+0xce>
+   29a1b171e:	call   *0x7b64(%rip)        # 29a1b9288 <__imp_VirtualProtect>
+   29a1b1724:	test   %eax,%eax
+   29a1b1726:	jne    29a1b16de <mark_section_writable+0xce>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:226
-   29a1b16f8:	call   *0x7b5a(%rip)        # 29a1b9258 <__imp_GetLastError>
+   29a1b1728:	call   *0x7b32(%rip)        # 29a1b9260 <__imp_GetLastError>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:225
-   29a1b16fe:	lea    0x29d3(%rip),%rcx        # 29a1b40d8 <.rdata+0x78>
+   29a1b172e:	lea    0x29a3(%rip),%rcx        # 29a1b40d8 <.rdata+0x78>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:226
-   29a1b1705:	mov    %eax,%edx
+   29a1b1735:	mov    %eax,%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:225
-   29a1b1707:	call   29a1b1570 <__report_error>
-   29a1b170c:	nopl   0x0(%rax)
+   29a1b1737:	call   29a1b15a0 <__report_error>
+   29a1b173c:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:189
-   29a1b1710:	xor    %esi,%esi
-   29a1b1712:	jmp    29a1b1638 <mark_section_writable+0x58>
+   29a1b1740:	xor    %esi,%esi
+   29a1b1742:	jmp    29a1b1668 <mark_section_writable+0x58>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:207
-   29a1b1717:	mov    0x594a(%rip),%rax        # 29a1b7068 <the_secs>
-   29a1b171e:	mov    0x8(%rdi),%edx
-   29a1b1721:	lea    0x2978(%rip),%rcx        # 29a1b40a0 <.rdata+0x40>
-   29a1b1728:	mov    0x18(%rax,%rbx,1),%r8
-   29a1b172d:	call   29a1b1570 <__report_error>
+   29a1b1747:	mov    0x591a(%rip),%rax        # 29a1b7068 <the_secs>
+   29a1b174e:	mov    0x8(%rdi),%edx
+   29a1b1751:	lea    0x2948(%rip),%rcx        # 29a1b40a0 <.rdata+0x40>
+   29a1b1758:	mov    0x18(%rax,%rbx,1),%r8
+   29a1b175d:	call   29a1b15a0 <__report_error>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:198
-   29a1b1732:	mov    %rbx,%rdx
-   29a1b1735:	lea    0x2944(%rip),%rcx        # 29a1b4080 <.rdata+0x20>
-   29a1b173c:	call   29a1b1570 <__report_error>
-   29a1b1741:	nop
-   29a1b1742:	data16 cs nopw 0x0(%rax,%rax,1)
-   29a1b174d:	nopl   (%rax)
+   29a1b1762:	mov    %rbx,%rdx
+   29a1b1765:	lea    0x2914(%rip),%rcx        # 29a1b4080 <.rdata+0x20>
+   29a1b176c:	call   29a1b15a0 <__report_error>
+   29a1b1771:	nop
+   29a1b1772:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b177d:	nopl   (%rax)
 
-000000029a1b1750 <_pei386_runtime_relocator>:
+000000029a1b1780 <_pei386_runtime_relocator>:
 _pei386_runtime_relocator():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:486
-   29a1b1750:	push   %rbp
-   29a1b1751:	push   %r15
-   29a1b1753:	push   %r14
-   29a1b1755:	push   %r13
-   29a1b1757:	push   %r12
-   29a1b1759:	push   %rdi
-   29a1b175a:	push   %rsi
-   29a1b175b:	push   %rbx
-   29a1b175c:	sub    $0x48,%rsp
-   29a1b1760:	lea    0x40(%rsp),%rbp
+   29a1b1780:	push   %rbp
+   29a1b1781:	push   %r15
+   29a1b1783:	push   %r14
+   29a1b1785:	push   %r13
+   29a1b1787:	push   %r12
+   29a1b1789:	push   %rdi
+   29a1b178a:	push   %rsi
+   29a1b178b:	push   %rbx
+   29a1b178c:	sub    $0x48,%rsp
+   29a1b1790:	lea    0x40(%rsp),%rbp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:492
-   29a1b1765:	mov    0x58f4(%rip),%r12d        # 29a1b7060 <was_init.0>
-   29a1b176c:	test   %r12d,%r12d
-   29a1b176f:	je     29a1b1788 <_pei386_runtime_relocator+0x38>
+   29a1b1795:	mov    0x58c4(%rip),%r12d        # 29a1b7060 <was_init.0>
+   29a1b179c:	test   %r12d,%r12d
+   29a1b179f:	je     29a1b17b8 <_pei386_runtime_relocator+0x38>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:508
-   29a1b1771:	lea    0x8(%rbp),%rsp
-   29a1b1775:	pop    %rbx
-   29a1b1776:	pop    %rsi
-   29a1b1777:	pop    %rdi
-   29a1b1778:	pop    %r12
-   29a1b177a:	pop    %r13
-   29a1b177c:	pop    %r14
-   29a1b177e:	pop    %r15
-   29a1b1780:	pop    %rbp
-   29a1b1781:	ret
-   29a1b1782:	nopw   0x0(%rax,%rax,1)
+   29a1b17a1:	lea    0x8(%rbp),%rsp
+   29a1b17a5:	pop    %rbx
+   29a1b17a6:	pop    %rsi
+   29a1b17a7:	pop    %rdi
+   29a1b17a8:	pop    %r12
+   29a1b17aa:	pop    %r13
+   29a1b17ac:	pop    %r14
+   29a1b17ae:	pop    %r15
+   29a1b17b0:	pop    %rbp
+   29a1b17b1:	ret
+   29a1b17b2:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:494
-   29a1b1788:	movl   $0x1,0x58ce(%rip)        # 29a1b7060 <was_init.0>
+   29a1b17b8:	movl   $0x1,0x589e(%rip)        # 29a1b7060 <was_init.0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:496
-   29a1b1792:	call   29a1b1ec0 <__mingw_GetSectionCount>
+   29a1b17c2:	call   29a1b1ef0 <__mingw_GetSectionCount>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:497
-   29a1b1797:	cltq
-   29a1b1799:	lea    (%rax,%rax,4),%rax
-   29a1b179d:	lea    0xf(,%rax,8),%rax
-   29a1b17a5:	and    $0xfffffffffffffff0,%rax
-   29a1b17a9:	call   29a1b2130 <___chkstk_ms>
+   29a1b17c7:	cltq
+   29a1b17c9:	lea    (%rax,%rax,4),%rax
+   29a1b17cd:	lea    0xf(,%rax,8),%rax
+   29a1b17d5:	and    $0xfffffffffffffff0,%rax
+   29a1b17d9:	call   29a1b2160 <___chkstk_ms>
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:312
-   29a1b17ae:	mov    0x2a5b(%rip),%r13        # 29a1b4210 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
-   29a1b17b5:	mov    0x2a64(%rip),%rbx        # 29a1b4220 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
+   29a1b17de:	mov    0x2a2b(%rip),%r13        # 29a1b4210 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
+   29a1b17e5:	mov    0x2a34(%rip),%rbx        # 29a1b4220 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
 _pei386_runtime_relocator():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:498
-   29a1b17bc:	movl   $0x0,0x589e(%rip)        # 29a1b7064 <maxSections>
+   29a1b17ec:	movl   $0x0,0x586e(%rip)        # 29a1b7064 <maxSections>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:497
-   29a1b17c6:	sub    %rax,%rsp
-   29a1b17c9:	lea    0x30(%rsp),%rax
-   29a1b17ce:	mov    %rax,0x5893(%rip)        # 29a1b7068 <the_secs>
+   29a1b17f6:	sub    %rax,%rsp
+   29a1b17f9:	lea    0x30(%rsp),%rax
+   29a1b17fe:	mov    %rax,0x5863(%rip)        # 29a1b7068 <the_secs>
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:312
-   29a1b17d5:	mov    %r13,%rax
-   29a1b17d8:	sub    %rbx,%rax
+   29a1b1805:	mov    %r13,%rax
+   29a1b1808:	sub    %rbx,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:321
-   29a1b17db:	cmp    $0x7,%rax
-   29a1b17df:	jle    29a1b1771 <_pei386_runtime_relocator+0x21>
+   29a1b180b:	cmp    $0x7,%rax
+   29a1b180f:	jle    29a1b17a1 <_pei386_runtime_relocator+0x21>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:344
-   29a1b17e1:	mov    (%rbx),%edx
+   29a1b1811:	mov    (%rbx),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:343
-   29a1b17e3:	cmp    $0xb,%rax
-   29a1b17e7:	jg     29a1b18f0 <_pei386_runtime_relocator+0x1a0>
+   29a1b1813:	cmp    $0xb,%rax
+   29a1b1817:	jg     29a1b1920 <_pei386_runtime_relocator+0x1a0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:358
-   29a1b17ed:	mov    (%rbx),%eax
-   29a1b17ef:	test   %eax,%eax
-   29a1b17f1:	jne    29a1b1a60 <_pei386_runtime_relocator+0x310>
-   29a1b17f7:	mov    0x4(%rbx),%eax
-   29a1b17fa:	test   %eax,%eax
-   29a1b17fc:	jne    29a1b1a60 <_pei386_runtime_relocator+0x310>
+   29a1b181d:	mov    (%rbx),%eax
+   29a1b181f:	test   %eax,%eax
+   29a1b1821:	jne    29a1b1a90 <_pei386_runtime_relocator+0x310>
+   29a1b1827:	mov    0x4(%rbx),%eax
+   29a1b182a:	test   %eax,%eax
+   29a1b182c:	jne    29a1b1a90 <_pei386_runtime_relocator+0x310>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:379
-   29a1b1802:	mov    0x8(%rbx),%edx
-   29a1b1805:	cmp    $0x1,%edx
-   29a1b1808:	jne    29a1b1aa0 <_pei386_runtime_relocator+0x350>
+   29a1b1832:	mov    0x8(%rbx),%edx
+   29a1b1835:	cmp    $0x1,%edx
+   29a1b1838:	jne    29a1b1ad0 <_pei386_runtime_relocator+0x350>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:391
-   29a1b180e:	add    $0xc,%rbx
+   29a1b183e:	add    $0xc,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:393
-   29a1b1812:	cmp    %r13,%rbx
-   29a1b1815:	jae    29a1b1771 <_pei386_runtime_relocator+0x21>
+   29a1b1842:	cmp    %r13,%rbx
+   29a1b1845:	jae    29a1b17a1 <_pei386_runtime_relocator+0x21>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:396
-   29a1b181b:	mov    0x29de(%rip),%r14        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b184b:	mov    0x29ae(%rip),%r14        # 29a1b4200 <.refptr.__ImageBase>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:456
-   29a1b1822:	mov    $0xffffffff,%r15d
-   29a1b1828:	jmp    29a1b188f <_pei386_runtime_relocator+0x13f>
-   29a1b182a:	nopw   0x0(%rax,%rax,1)
+   29a1b1852:	mov    $0xffffffff,%r15d
+   29a1b1858:	jmp    29a1b18bf <_pei386_runtime_relocator+0x13f>
+   29a1b185a:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:410
-   29a1b1830:	cmp    $0x8,%ecx
-   29a1b1833:	je     29a1b1910 <_pei386_runtime_relocator+0x1c0>
-   29a1b1839:	cmp    $0x10,%ecx
-   29a1b183c:	jne    29a1b1a92 <_pei386_runtime_relocator+0x342>
+   29a1b1860:	cmp    $0x8,%ecx
+   29a1b1863:	je     29a1b1940 <_pei386_runtime_relocator+0x1c0>
+   29a1b1869:	cmp    $0x10,%ecx
+   29a1b186c:	jne    29a1b1ac2 <_pei386_runtime_relocator+0x342>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:418
-   29a1b1842:	movzwl (%rdi),%esi
+   29a1b1872:	movzwl (%rdi),%esi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:419
-   29a1b1845:	and    $0xc0,%edx
-   29a1b184b:	test   %si,%si
-   29a1b184e:	jns    29a1b1a20 <_pei386_runtime_relocator+0x2d0>
+   29a1b1875:	and    $0xc0,%edx
+   29a1b187b:	test   %si,%si
+   29a1b187e:	jns    29a1b1a50 <_pei386_runtime_relocator+0x2d0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:420
-   29a1b1854:	or     $0xffffffffffff0000,%rsi
+   29a1b1884:	or     $0xffffffffffff0000,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b185b:	sub    %rax,%rsi
+   29a1b188b:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b185e:	add    %r9,%rsi
+   29a1b188e:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b1861:	test   %edx,%edx
-   29a1b1863:	jne    29a1b1877 <_pei386_runtime_relocator+0x127>
+   29a1b1891:	test   %edx,%edx
+   29a1b1893:	jne    29a1b18a7 <_pei386_runtime_relocator+0x127>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:456
-   29a1b1865:	cmp    $0xffffffffffff8000,%rsi
-   29a1b186c:	jl     29a1b18d3 <_pei386_runtime_relocator+0x183>
-   29a1b186e:	cmp    $0xffff,%rsi
-   29a1b1875:	jg     29a1b18d3 <_pei386_runtime_relocator+0x183>
+   29a1b1895:	cmp    $0xffffffffffff8000,%rsi
+   29a1b189c:	jl     29a1b1903 <_pei386_runtime_relocator+0x183>
+   29a1b189e:	cmp    $0xffff,%rsi
+   29a1b18a5:	jg     29a1b1903 <_pei386_runtime_relocator+0x183>
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b1877:	mov    %rdi,%rcx
-   29a1b187a:	call   29a1b15e0 <mark_section_writable>
+   29a1b18a7:	mov    %rdi,%rcx
+   29a1b18aa:	call   29a1b1610 <mark_section_writable>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:294
-   29a1b187f:	mov    %si,(%rdi)
+   29a1b18af:	mov    %si,(%rdi)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:393
-   29a1b1882:	add    $0xc,%rbx
-   29a1b1886:	cmp    %r13,%rbx
-   29a1b1889:	jae    29a1b1960 <_pei386_runtime_relocator+0x210>
+   29a1b18b2:	add    $0xc,%rbx
+   29a1b18b6:	cmp    %r13,%rbx
+   29a1b18b9:	jae    29a1b1990 <_pei386_runtime_relocator+0x210>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:401
-   29a1b188f:	mov    (%rbx),%eax
+   29a1b18bf:	mov    (%rbx),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:410
-   29a1b1891:	mov    0x8(%rbx),%edx
+   29a1b18c1:	mov    0x8(%rbx),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:396
-   29a1b1894:	mov    0x4(%rbx),%edi
+   29a1b18c4:	mov    0x4(%rbx),%edi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:401
-   29a1b1897:	add    %r14,%rax
+   29a1b18c7:	add    %r14,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:410
-   29a1b189a:	movzbl %dl,%ecx
+   29a1b18ca:	movzbl %dl,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:402
-   29a1b189d:	mov    (%rax),%r9
+   29a1b18cd:	mov    (%rax),%r9
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:396
-   29a1b18a0:	add    %r14,%rdi
+   29a1b18d0:	add    %r14,%rdi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:410
-   29a1b18a3:	cmp    $0x20,%ecx
-   29a1b18a6:	je     29a1b19b8 <_pei386_runtime_relocator+0x268>
-   29a1b18ac:	jbe    29a1b1830 <_pei386_runtime_relocator+0xe0>
-   29a1b18ae:	cmp    $0x40,%ecx
-   29a1b18b1:	jne    29a1b1a92 <_pei386_runtime_relocator+0x342>
+   29a1b18d3:	cmp    $0x20,%ecx
+   29a1b18d6:	je     29a1b19e8 <_pei386_runtime_relocator+0x268>
+   29a1b18dc:	jbe    29a1b1860 <_pei386_runtime_relocator+0xe0>
+   29a1b18de:	cmp    $0x40,%ecx
+   29a1b18e1:	jne    29a1b1ac2 <_pei386_runtime_relocator+0x342>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b18b7:	mov    (%rdi),%rsi
+   29a1b18e7:	mov    (%rdi),%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b18ba:	mov    %edx,%ecx
+   29a1b18ea:	mov    %edx,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b18bc:	sub    %rax,%rsi
+   29a1b18ec:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b18bf:	add    %r9,%rsi
+   29a1b18ef:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b18c2:	and    $0xc0,%ecx
-   29a1b18c8:	jne    29a1b1a10 <_pei386_runtime_relocator+0x2c0>
+   29a1b18f2:	and    $0xc0,%ecx
+   29a1b18f8:	jne    29a1b1a40 <_pei386_runtime_relocator+0x2c0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:456
-   29a1b18ce:	test   %rsi,%rsi
-   29a1b18d1:	js     29a1b1882 <_pei386_runtime_relocator+0x132>
+   29a1b18fe:	test   %rsi,%rsi
+   29a1b1901:	js     29a1b18b2 <_pei386_runtime_relocator+0x132>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:457
-   29a1b18d3:	mov    %rsi,0x20(%rsp)
-   29a1b18d8:	mov    %ecx,%edx
-   29a1b18da:	mov    %rdi,%r8
-   29a1b18dd:	lea    0x2884(%rip),%rcx        # 29a1b4168 <.rdata+0x108>
-   29a1b18e4:	call   29a1b1570 <__report_error>
-   29a1b18e9:	nopl   0x0(%rax)
+   29a1b1903:	mov    %rsi,0x20(%rsp)
+   29a1b1908:	mov    %ecx,%edx
+   29a1b190a:	mov    %rdi,%r8
+   29a1b190d:	lea    0x2854(%rip),%rcx        # 29a1b4168 <.rdata+0x108>
+   29a1b1914:	call   29a1b15a0 <__report_error>
+   29a1b1919:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:344
-   29a1b18f0:	test   %edx,%edx
-   29a1b18f2:	jne    29a1b1a60 <_pei386_runtime_relocator+0x310>
-   29a1b18f8:	mov    0x4(%rbx),%eax
+   29a1b1920:	test   %edx,%edx
+   29a1b1922:	jne    29a1b1a90 <_pei386_runtime_relocator+0x310>
+   29a1b1928:	mov    0x4(%rbx),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:345
-   29a1b18fb:	mov    %eax,%edx
-   29a1b18fd:	or     0x8(%rbx),%edx
-   29a1b1900:	jne    29a1b17fa <_pei386_runtime_relocator+0xaa>
+   29a1b192b:	mov    %eax,%edx
+   29a1b192d:	or     0x8(%rbx),%edx
+   29a1b1930:	jne    29a1b182a <_pei386_runtime_relocator+0xaa>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:355
-   29a1b1906:	add    $0xc,%rbx
-   29a1b190a:	jmp    29a1b17ed <_pei386_runtime_relocator+0x9d>
-   29a1b190f:	nop
+   29a1b1936:	add    $0xc,%rbx
+   29a1b193a:	jmp    29a1b181d <_pei386_runtime_relocator+0x9d>
+   29a1b193f:	nop
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:413
-   29a1b1910:	movzbl (%rdi),%esi
+   29a1b1940:	movzbl (%rdi),%esi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:414
-   29a1b1913:	and    $0xc0,%edx
-   29a1b1919:	test   %sil,%sil
-   29a1b191c:	jns    29a1b1a48 <_pei386_runtime_relocator+0x2f8>
+   29a1b1943:	and    $0xc0,%edx
+   29a1b1949:	test   %sil,%sil
+   29a1b194c:	jns    29a1b1a78 <_pei386_runtime_relocator+0x2f8>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:415
-   29a1b1922:	or     $0xffffffffffffff00,%rsi
+   29a1b1952:	or     $0xffffffffffffff00,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b1929:	sub    %rax,%rsi
+   29a1b1959:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b192c:	add    %r9,%rsi
+   29a1b195c:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b192f:	test   %edx,%edx
-   29a1b1931:	jne    29a1b1942 <_pei386_runtime_relocator+0x1f2>
+   29a1b195f:	test   %edx,%edx
+   29a1b1961:	jne    29a1b1972 <_pei386_runtime_relocator+0x1f2>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:456
-   29a1b1933:	cmp    $0xff,%rsi
-   29a1b193a:	jg     29a1b18d3 <_pei386_runtime_relocator+0x183>
-   29a1b193c:	cmp    $0xffffffffffffff80,%rsi
-   29a1b1940:	jl     29a1b18d3 <_pei386_runtime_relocator+0x183>
+   29a1b1963:	cmp    $0xff,%rsi
+   29a1b196a:	jg     29a1b1903 <_pei386_runtime_relocator+0x183>
+   29a1b196c:	cmp    $0xffffffffffffff80,%rsi
+   29a1b1970:	jl     29a1b1903 <_pei386_runtime_relocator+0x183>
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b1942:	mov    %rdi,%rcx
+   29a1b1972:	mov    %rdi,%rcx
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:393
-   29a1b1945:	add    $0xc,%rbx
+   29a1b1975:	add    $0xc,%rbx
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b1949:	call   29a1b15e0 <mark_section_writable>
+   29a1b1979:	call   29a1b1610 <mark_section_writable>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:294
-   29a1b194e:	mov    %sil,(%rdi)
+   29a1b197e:	mov    %sil,(%rdi)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:393
-   29a1b1951:	cmp    %r13,%rbx
-   29a1b1954:	jb     29a1b188f <_pei386_runtime_relocator+0x13f>
-   29a1b195a:	nopw   0x0(%rax,%rax,1)
+   29a1b1981:	cmp    %r13,%rbx
+   29a1b1984:	jb     29a1b18bf <_pei386_runtime_relocator+0x13f>
+   29a1b198a:	nopw   0x0(%rax,%rax,1)
 restore_modified_sections():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:238
-   29a1b1960:	mov    0x56fe(%rip),%edx        # 29a1b7064 <maxSections>
-   29a1b1966:	test   %edx,%edx
-   29a1b1968:	jle    29a1b1771 <_pei386_runtime_relocator+0x21>
+   29a1b1990:	mov    0x56ce(%rip),%edx        # 29a1b7064 <maxSections>
+   29a1b1996:	test   %edx,%edx
+   29a1b1998:	jle    29a1b17a1 <_pei386_runtime_relocator+0x21>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:242
-   29a1b196e:	mov    0x790b(%rip),%rsi        # 29a1b9280 <__imp_VirtualProtect>
+   29a1b199e:	mov    0x78e3(%rip),%rsi        # 29a1b9288 <__imp_VirtualProtect>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:238
-   29a1b1975:	xor    %ebx,%ebx
+   29a1b19a5:	xor    %ebx,%ebx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:242
-   29a1b1977:	lea    -0x4(%rbp),%rdi
-   29a1b197b:	nopl   0x0(%rax,%rax,1)
+   29a1b19a7:	lea    -0x4(%rbp),%rdi
+   29a1b19ab:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:240
-   29a1b1980:	mov    0x56e1(%rip),%rax        # 29a1b7068 <the_secs>
-   29a1b1987:	add    %rbx,%rax
-   29a1b198a:	mov    (%rax),%r8d
-   29a1b198d:	test   %r8d,%r8d
-   29a1b1990:	je     29a1b199f <_pei386_runtime_relocator+0x24f>
+   29a1b19b0:	mov    0x56b1(%rip),%rax        # 29a1b7068 <the_secs>
+   29a1b19b7:	add    %rbx,%rax
+   29a1b19ba:	mov    (%rax),%r8d
+   29a1b19bd:	test   %r8d,%r8d
+   29a1b19c0:	je     29a1b19cf <_pei386_runtime_relocator+0x24f>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:242
-   29a1b1992:	mov    0x10(%rax),%rdx
-   29a1b1996:	mov    0x8(%rax),%rcx
-   29a1b199a:	mov    %rdi,%r9
-   29a1b199d:	call   *%rsi
+   29a1b19c2:	mov    0x10(%rax),%rdx
+   29a1b19c6:	mov    0x8(%rax),%rcx
+   29a1b19ca:	mov    %rdi,%r9
+   29a1b19cd:	call   *%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:238
-   29a1b199f:	add    $0x1,%r12d
-   29a1b19a3:	add    $0x28,%rbx
-   29a1b19a7:	cmp    0x56b6(%rip),%r12d        # 29a1b7064 <maxSections>
-   29a1b19ae:	jl     29a1b1980 <_pei386_runtime_relocator+0x230>
-   29a1b19b0:	jmp    29a1b1771 <_pei386_runtime_relocator+0x21>
-   29a1b19b5:	nopl   (%rax)
+   29a1b19cf:	add    $0x1,%r12d
+   29a1b19d3:	add    $0x28,%rbx
+   29a1b19d7:	cmp    0x5686(%rip),%r12d        # 29a1b7064 <maxSections>
+   29a1b19de:	jl     29a1b19b0 <_pei386_runtime_relocator+0x230>
+   29a1b19e0:	jmp    29a1b17a1 <_pei386_runtime_relocator+0x21>
+   29a1b19e5:	nopl   (%rax)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:423
-   29a1b19b8:	mov    (%rdi),%esi
+   29a1b19e8:	mov    (%rdi),%esi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:425
-   29a1b19ba:	and    $0xc0,%edx
-   29a1b19c0:	test   %esi,%esi
-   29a1b19c2:	jns    29a1b1a38 <_pei386_runtime_relocator+0x2e8>
+   29a1b19ea:	and    $0xc0,%edx
+   29a1b19f0:	test   %esi,%esi
+   29a1b19f2:	jns    29a1b1a68 <_pei386_runtime_relocator+0x2e8>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:426
-   29a1b19c4:	movabs $0xffffffff00000000,%r11
-   29a1b19ce:	or     %r11,%rsi
+   29a1b19f4:	movabs $0xffffffff00000000,%r11
+   29a1b19fe:	or     %r11,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b19d1:	sub    %rax,%rsi
+   29a1b1a01:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b19d4:	add    %r9,%rsi
+   29a1b1a04:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b19d7:	test   %edx,%edx
-   29a1b19d9:	jne    29a1b19f7 <_pei386_runtime_relocator+0x2a7>
+   29a1b1a07:	test   %edx,%edx
+   29a1b1a09:	jne    29a1b1a27 <_pei386_runtime_relocator+0x2a7>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:456
-   29a1b19db:	cmp    %r15,%rsi
-   29a1b19de:	jg     29a1b18d3 <_pei386_runtime_relocator+0x183>
-   29a1b19e4:	movabs $0xffffffff7fffffff,%rax
-   29a1b19ee:	cmp    %rax,%rsi
-   29a1b19f1:	jle    29a1b18d3 <_pei386_runtime_relocator+0x183>
+   29a1b1a0b:	cmp    %r15,%rsi
+   29a1b1a0e:	jg     29a1b1903 <_pei386_runtime_relocator+0x183>
+   29a1b1a14:	movabs $0xffffffff7fffffff,%rax
+   29a1b1a1e:	cmp    %rax,%rsi
+   29a1b1a21:	jle    29a1b1903 <_pei386_runtime_relocator+0x183>
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b19f7:	mov    %rdi,%rcx
-   29a1b19fa:	call   29a1b15e0 <mark_section_writable>
+   29a1b1a27:	mov    %rdi,%rcx
+   29a1b1a2a:	call   29a1b1610 <mark_section_writable>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:294
-   29a1b19ff:	mov    %esi,(%rdi)
+   29a1b1a2f:	mov    %esi,(%rdi)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:473
-   29a1b1a01:	jmp    29a1b1882 <_pei386_runtime_relocator+0x132>
-   29a1b1a06:	cs nopw 0x0(%rax,%rax,1)
+   29a1b1a31:	jmp    29a1b18b2 <_pei386_runtime_relocator+0x132>
+   29a1b1a36:	cs nopw 0x0(%rax,%rax,1)
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b1a10:	mov    %rdi,%rcx
-   29a1b1a13:	call   29a1b15e0 <mark_section_writable>
+   29a1b1a40:	mov    %rdi,%rcx
+   29a1b1a43:	call   29a1b1610 <mark_section_writable>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:294
-   29a1b1a18:	mov    %rsi,(%rdi)
+   29a1b1a48:	mov    %rsi,(%rdi)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:477
-   29a1b1a1b:	jmp    29a1b1882 <_pei386_runtime_relocator+0x132>
+   29a1b1a4b:	jmp    29a1b18b2 <_pei386_runtime_relocator+0x132>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b1a20:	sub    %rax,%rsi
+   29a1b1a50:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b1a23:	add    %r9,%rsi
+   29a1b1a53:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b1a26:	test   %edx,%edx
-   29a1b1a28:	je     29a1b1865 <_pei386_runtime_relocator+0x115>
-   29a1b1a2e:	jmp    29a1b1877 <_pei386_runtime_relocator+0x127>
-   29a1b1a33:	nopl   0x0(%rax,%rax,1)
+   29a1b1a56:	test   %edx,%edx
+   29a1b1a58:	je     29a1b1895 <_pei386_runtime_relocator+0x115>
+   29a1b1a5e:	jmp    29a1b18a7 <_pei386_runtime_relocator+0x127>
+   29a1b1a63:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b1a38:	sub    %rax,%rsi
+   29a1b1a68:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b1a3b:	add    %r9,%rsi
+   29a1b1a6b:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b1a3e:	test   %edx,%edx
-   29a1b1a40:	je     29a1b19db <_pei386_runtime_relocator+0x28b>
-   29a1b1a42:	jmp    29a1b19f7 <_pei386_runtime_relocator+0x2a7>
-   29a1b1a44:	nopl   0x0(%rax)
+   29a1b1a6e:	test   %edx,%edx
+   29a1b1a70:	je     29a1b1a0b <_pei386_runtime_relocator+0x28b>
+   29a1b1a72:	jmp    29a1b1a27 <_pei386_runtime_relocator+0x2a7>
+   29a1b1a74:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b1a48:	sub    %rax,%rsi
+   29a1b1a78:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b1a4b:	add    %r9,%rsi
+   29a1b1a7b:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b1a4e:	test   %edx,%edx
-   29a1b1a50:	je     29a1b1933 <_pei386_runtime_relocator+0x1e3>
-   29a1b1a56:	jmp    29a1b1942 <_pei386_runtime_relocator+0x1f2>
-   29a1b1a5b:	nopl   0x0(%rax,%rax,1)
+   29a1b1a7e:	test   %edx,%edx
+   29a1b1a80:	je     29a1b1963 <_pei386_runtime_relocator+0x1e3>
+   29a1b1a86:	jmp    29a1b1972 <_pei386_runtime_relocator+0x1f2>
+   29a1b1a8b:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:365
-   29a1b1a60:	cmp    %r13,%rbx
-   29a1b1a63:	jae    29a1b1771 <_pei386_runtime_relocator+0x21>
+   29a1b1a90:	cmp    %r13,%rbx
+   29a1b1a93:	jae    29a1b17a1 <_pei386_runtime_relocator+0x21>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:396
-   29a1b1a69:	mov    0x2790(%rip),%r14        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1a99:	mov    0x2760(%rip),%r14        # 29a1b4200 <.refptr.__ImageBase>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:369
-   29a1b1a70:	mov    0x4(%rbx),%esi
+   29a1b1aa0:	mov    0x4(%rbx),%esi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:370
-   29a1b1a73:	mov    (%rbx),%edi
+   29a1b1aa3:	mov    (%rbx),%edi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:366
-   29a1b1a75:	add    $0x8,%rbx
+   29a1b1aa5:	add    $0x8,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:369
-   29a1b1a79:	add    %r14,%rsi
+   29a1b1aa9:	add    %r14,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:370
-   29a1b1a7c:	add    (%rsi),%edi
+   29a1b1aac:	add    (%rsi),%edi
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b1a7e:	mov    %rsi,%rcx
-   29a1b1a81:	call   29a1b15e0 <mark_section_writable>
+   29a1b1aae:	mov    %rsi,%rcx
+   29a1b1ab1:	call   29a1b1610 <mark_section_writable>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:294
-   29a1b1a86:	mov    %edi,(%rsi)
+   29a1b1ab6:	mov    %edi,(%rsi)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:365
-   29a1b1a88:	cmp    %r13,%rbx
-   29a1b1a8b:	jb     29a1b1a70 <_pei386_runtime_relocator+0x320>
-   29a1b1a8d:	jmp    29a1b1960 <_pei386_runtime_relocator+0x210>
+   29a1b1ab8:	cmp    %r13,%rbx
+   29a1b1abb:	jb     29a1b1aa0 <_pei386_runtime_relocator+0x320>
+   29a1b1abd:	jmp    29a1b1990 <_pei386_runtime_relocator+0x210>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:436
-   29a1b1a92:	mov    %ecx,%edx
-   29a1b1a94:	lea    0x269d(%rip),%rcx        # 29a1b4138 <.rdata+0xd8>
-   29a1b1a9b:	call   29a1b1570 <__report_error>
+   29a1b1ac2:	mov    %ecx,%edx
+   29a1b1ac4:	lea    0x266d(%rip),%rcx        # 29a1b4138 <.rdata+0xd8>
+   29a1b1acb:	call   29a1b15a0 <__report_error>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:381
-   29a1b1aa0:	lea    0x2659(%rip),%rcx        # 29a1b4100 <.rdata+0xa0>
-   29a1b1aa7:	call   29a1b1570 <__report_error>
-   29a1b1aac:	nop
-   29a1b1aad:	nop
-   29a1b1aae:	nop
-   29a1b1aaf:	nop
+   29a1b1ad0:	lea    0x2629(%rip),%rcx        # 29a1b4100 <.rdata+0xa0>
+   29a1b1ad7:	call   29a1b15a0 <__report_error>
+   29a1b1adc:	nop
+   29a1b1add:	nop
+   29a1b1ade:	nop
+   29a1b1adf:	nop
 
-000000029a1b1ab0 <__mingwthr_run_key_dtors.part.0>:
+000000029a1b1ae0 <__mingwthr_run_key_dtors.part.0>:
 __mingwthr_run_key_dtors():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:99
-   29a1b1ab0:	push   %r12
-   29a1b1ab2:	push   %rbp
-   29a1b1ab3:	push   %rdi
-   29a1b1ab4:	push   %rsi
-   29a1b1ab5:	push   %rbx
-   29a1b1ab6:	sub    $0x20,%rsp
+   29a1b1ae0:	push   %r12
+   29a1b1ae2:	push   %rbp
+   29a1b1ae3:	push   %rdi
+   29a1b1ae4:	push   %rsi
+   29a1b1ae5:	push   %rbx
+   29a1b1ae6:	sub    $0x20,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:105
-   29a1b1aba:	lea    0x55df(%rip),%r12        # 29a1b70a0 <__mingwthr_cs>
-   29a1b1ac1:	mov    %r12,%rcx
-   29a1b1ac4:	call   *0x7786(%rip)        # 29a1b9250 <__imp_EnterCriticalSection>
+   29a1b1aea:	lea    0x55af(%rip),%r12        # 29a1b70a0 <__mingwthr_cs>
+   29a1b1af1:	mov    %r12,%rcx
+   29a1b1af4:	call   *0x775e(%rip)        # 29a1b9258 <__imp_EnterCriticalSection>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:107
-   29a1b1aca:	mov    0x55af(%rip),%rbx        # 29a1b7080 <key_dtor_list>
-   29a1b1ad1:	test   %rbx,%rbx
-   29a1b1ad4:	je     29a1b1b0c <__mingwthr_run_key_dtors.part.0+0x5c>
-   29a1b1ad6:	mov    0x779b(%rip),%rbp        # 29a1b9278 <__imp_TlsGetValue>
-   29a1b1add:	mov    0x7774(%rip),%rdi        # 29a1b9258 <__imp_GetLastError>
-   29a1b1ae4:	nopl   0x0(%rax)
+   29a1b1afa:	mov    0x557f(%rip),%rbx        # 29a1b7080 <key_dtor_list>
+   29a1b1b01:	test   %rbx,%rbx
+   29a1b1b04:	je     29a1b1b3c <__mingwthr_run_key_dtors.part.0+0x5c>
+   29a1b1b06:	mov    0x7773(%rip),%rbp        # 29a1b9280 <__imp_TlsGetValue>
+   29a1b1b0d:	mov    0x774c(%rip),%rdi        # 29a1b9260 <__imp_GetLastError>
+   29a1b1b14:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:109
-   29a1b1ae8:	mov    (%rbx),%ecx
-   29a1b1aea:	call   *%rbp
-   29a1b1aec:	mov    %rax,%rsi
+   29a1b1b18:	mov    (%rbx),%ecx
+   29a1b1b1a:	call   *%rbp
+   29a1b1b1c:	mov    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:110
-   29a1b1aef:	call   *%rdi
+   29a1b1b1f:	call   *%rdi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:112
-   29a1b1af1:	test   %rsi,%rsi
-   29a1b1af4:	je     29a1b1b03 <__mingwthr_run_key_dtors.part.0+0x53>
-   29a1b1af6:	test   %eax,%eax
-   29a1b1af8:	jne    29a1b1b03 <__mingwthr_run_key_dtors.part.0+0x53>
+   29a1b1b21:	test   %rsi,%rsi
+   29a1b1b24:	je     29a1b1b33 <__mingwthr_run_key_dtors.part.0+0x53>
+   29a1b1b26:	test   %eax,%eax
+   29a1b1b28:	jne    29a1b1b33 <__mingwthr_run_key_dtors.part.0+0x53>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:113
-   29a1b1afa:	mov    0x8(%rbx),%rax
-   29a1b1afe:	mov    %rsi,%rcx
-   29a1b1b01:	call   *%rax
+   29a1b1b2a:	mov    0x8(%rbx),%rax
+   29a1b1b2e:	mov    %rsi,%rcx
+   29a1b1b31:	call   *%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:115
-   29a1b1b03:	mov    0x10(%rbx),%rbx
+   29a1b1b33:	mov    0x10(%rbx),%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:107
-   29a1b1b07:	test   %rbx,%rbx
-   29a1b1b0a:	jne    29a1b1ae8 <__mingwthr_run_key_dtors.part.0+0x38>
+   29a1b1b37:	test   %rbx,%rbx
+   29a1b1b3a:	jne    29a1b1b18 <__mingwthr_run_key_dtors.part.0+0x38>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:118
-   29a1b1b0c:	mov    %r12,%rcx
+   29a1b1b3c:	mov    %r12,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:119
-   29a1b1b0f:	add    $0x20,%rsp
-   29a1b1b13:	pop    %rbx
-   29a1b1b14:	pop    %rsi
-   29a1b1b15:	pop    %rdi
-   29a1b1b16:	pop    %rbp
-   29a1b1b17:	pop    %r12
+   29a1b1b3f:	add    $0x20,%rsp
+   29a1b1b43:	pop    %rbx
+   29a1b1b44:	pop    %rsi
+   29a1b1b45:	pop    %rdi
+   29a1b1b46:	pop    %rbp
+   29a1b1b47:	pop    %r12
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:118
-   29a1b1b19:	rex.W jmp *0x7748(%rip)        # 29a1b9268 <__imp_LeaveCriticalSection>
+   29a1b1b49:	rex.W jmp *0x7720(%rip)        # 29a1b9270 <__imp_LeaveCriticalSection>
 
-000000029a1b1b20 <___w64_mingwthr_add_key_dtor>:
+000000029a1b1b50 <___w64_mingwthr_add_key_dtor>:
 ___w64_mingwthr_add_key_dtor():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:43
-   29a1b1b20:	push   %rdi
-   29a1b1b21:	push   %rsi
-   29a1b1b22:	push   %rbx
-   29a1b1b23:	sub    $0x20,%rsp
+   29a1b1b50:	push   %rdi
+   29a1b1b51:	push   %rsi
+   29a1b1b52:	push   %rbx
+   29a1b1b53:	sub    $0x20,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:46
-   29a1b1b27:	mov    0x555b(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1b57:	mov    0x552b(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:43
-   29a1b1b2d:	mov    %ecx,%edi
-   29a1b1b2f:	mov    %rdx,%rsi
+   29a1b1b5d:	mov    %ecx,%edi
+   29a1b1b5f:	mov    %rdx,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:46
-   29a1b1b32:	test   %eax,%eax
-   29a1b1b34:	jne    29a1b1b40 <___w64_mingwthr_add_key_dtor+0x20>
+   29a1b1b62:	test   %eax,%eax
+   29a1b1b64:	jne    29a1b1b70 <___w64_mingwthr_add_key_dtor+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:47
-   29a1b1b36:	xor    %eax,%eax
+   29a1b1b66:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:62
-   29a1b1b38:	add    $0x20,%rsp
-   29a1b1b3c:	pop    %rbx
-   29a1b1b3d:	pop    %rsi
-   29a1b1b3e:	pop    %rdi
-   29a1b1b3f:	ret
+   29a1b1b68:	add    $0x20,%rsp
+   29a1b1b6c:	pop    %rbx
+   29a1b1b6d:	pop    %rsi
+   29a1b1b6e:	pop    %rdi
+   29a1b1b6f:	ret
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:48
-   29a1b1b40:	mov    $0x18,%edx
-   29a1b1b45:	mov    $0x1,%ecx
-   29a1b1b4a:	call   29a1b24b8 <calloc>
-   29a1b1b4f:	mov    %rax,%rbx
+   29a1b1b70:	mov    $0x18,%edx
+   29a1b1b75:	mov    $0x1,%ecx
+   29a1b1b7a:	call   29a1b24f8 <calloc>
+   29a1b1b7f:	mov    %rax,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:49
-   29a1b1b52:	test   %rax,%rax
-   29a1b1b55:	je     29a1b1b8a <___w64_mingwthr_add_key_dtor+0x6a>
+   29a1b1b82:	test   %rax,%rax
+   29a1b1b85:	je     29a1b1bba <___w64_mingwthr_add_key_dtor+0x6a>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:53
-   29a1b1b57:	mov    %rsi,0x8(%rax)
+   29a1b1b87:	mov    %rsi,0x8(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:55
-   29a1b1b5b:	lea    0x553e(%rip),%rsi        # 29a1b70a0 <__mingwthr_cs>
+   29a1b1b8b:	lea    0x550e(%rip),%rsi        # 29a1b70a0 <__mingwthr_cs>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:52
-   29a1b1b62:	mov    %edi,(%rax)
+   29a1b1b92:	mov    %edi,(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:55
-   29a1b1b64:	mov    %rsi,%rcx
-   29a1b1b67:	call   *0x76e3(%rip)        # 29a1b9250 <__imp_EnterCriticalSection>
+   29a1b1b94:	mov    %rsi,%rcx
+   29a1b1b97:	call   *0x76bb(%rip)        # 29a1b9258 <__imp_EnterCriticalSection>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:57
-   29a1b1b6d:	mov    0x550c(%rip),%rax        # 29a1b7080 <key_dtor_list>
+   29a1b1b9d:	mov    0x54dc(%rip),%rax        # 29a1b7080 <key_dtor_list>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:60
-   29a1b1b74:	mov    %rsi,%rcx
+   29a1b1ba4:	mov    %rsi,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:58
-   29a1b1b77:	mov    %rbx,0x5502(%rip)        # 29a1b7080 <key_dtor_list>
+   29a1b1ba7:	mov    %rbx,0x54d2(%rip)        # 29a1b7080 <key_dtor_list>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:57
-   29a1b1b7e:	mov    %rax,0x10(%rbx)
+   29a1b1bae:	mov    %rax,0x10(%rbx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:60
-   29a1b1b82:	call   *0x76e0(%rip)        # 29a1b9268 <__imp_LeaveCriticalSection>
+   29a1b1bb2:	call   *0x76b8(%rip)        # 29a1b9270 <__imp_LeaveCriticalSection>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:61
-   29a1b1b88:	jmp    29a1b1b36 <___w64_mingwthr_add_key_dtor+0x16>
+   29a1b1bb8:	jmp    29a1b1b66 <___w64_mingwthr_add_key_dtor+0x16>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:50
-   29a1b1b8a:	or     $0xffffffff,%eax
-   29a1b1b8d:	jmp    29a1b1b38 <___w64_mingwthr_add_key_dtor+0x18>
-   29a1b1b8f:	nop
+   29a1b1bba:	or     $0xffffffff,%eax
+   29a1b1bbd:	jmp    29a1b1b68 <___w64_mingwthr_add_key_dtor+0x18>
+   29a1b1bbf:	nop
 
-000000029a1b1b90 <___w64_mingwthr_remove_key_dtor>:
+000000029a1b1bc0 <___w64_mingwthr_remove_key_dtor>:
 ___w64_mingwthr_remove_key_dtor():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:66
-   29a1b1b90:	push   %rsi
-   29a1b1b91:	push   %rbx
-   29a1b1b92:	sub    $0x28,%rsp
+   29a1b1bc0:	push   %rsi
+   29a1b1bc1:	push   %rbx
+   29a1b1bc2:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:70
-   29a1b1b96:	mov    0x54ec(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1bc6:	mov    0x54bc(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:66
-   29a1b1b9c:	mov    %ecx,%ebx
+   29a1b1bcc:	mov    %ecx,%ebx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:70
-   29a1b1b9e:	test   %eax,%eax
-   29a1b1ba0:	jne    29a1b1bb0 <___w64_mingwthr_remove_key_dtor+0x20>
+   29a1b1bce:	test   %eax,%eax
+   29a1b1bd0:	jne    29a1b1be0 <___w64_mingwthr_remove_key_dtor+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:96
-   29a1b1ba2:	xor    %eax,%eax
-   29a1b1ba4:	add    $0x28,%rsp
-   29a1b1ba8:	pop    %rbx
-   29a1b1ba9:	pop    %rsi
-   29a1b1baa:	ret
-   29a1b1bab:	nopl   0x0(%rax,%rax,1)
+   29a1b1bd2:	xor    %eax,%eax
+   29a1b1bd4:	add    $0x28,%rsp
+   29a1b1bd8:	pop    %rbx
+   29a1b1bd9:	pop    %rsi
+   29a1b1bda:	ret
+   29a1b1bdb:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:73
-   29a1b1bb0:	lea    0x54e9(%rip),%rsi        # 29a1b70a0 <__mingwthr_cs>
-   29a1b1bb7:	mov    %rsi,%rcx
-   29a1b1bba:	call   *0x7690(%rip)        # 29a1b9250 <__imp_EnterCriticalSection>
+   29a1b1be0:	lea    0x54b9(%rip),%rsi        # 29a1b70a0 <__mingwthr_cs>
+   29a1b1be7:	mov    %rsi,%rcx
+   29a1b1bea:	call   *0x7668(%rip)        # 29a1b9258 <__imp_EnterCriticalSection>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:76
-   29a1b1bc0:	mov    0x54b9(%rip),%rcx        # 29a1b7080 <key_dtor_list>
+   29a1b1bf0:	mov    0x5489(%rip),%rcx        # 29a1b7080 <key_dtor_list>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:78
-   29a1b1bc7:	test   %rcx,%rcx
-   29a1b1bca:	je     29a1b1bf3 <___w64_mingwthr_remove_key_dtor+0x63>
+   29a1b1bf7:	test   %rcx,%rcx
+   29a1b1bfa:	je     29a1b1c23 <___w64_mingwthr_remove_key_dtor+0x63>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:75
-   29a1b1bcc:	xor    %edx,%edx
-   29a1b1bce:	jmp    29a1b1bdb <___w64_mingwthr_remove_key_dtor+0x4b>
+   29a1b1bfc:	xor    %edx,%edx
+   29a1b1bfe:	jmp    29a1b1c0b <___w64_mingwthr_remove_key_dtor+0x4b>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:78
-   29a1b1bd0:	mov    %rcx,%rdx
-   29a1b1bd3:	test   %rax,%rax
-   29a1b1bd6:	je     29a1b1bf3 <___w64_mingwthr_remove_key_dtor+0x63>
-   29a1b1bd8:	mov    %rax,%rcx
+   29a1b1c00:	mov    %rcx,%rdx
+   29a1b1c03:	test   %rax,%rax
+   29a1b1c06:	je     29a1b1c23 <___w64_mingwthr_remove_key_dtor+0x63>
+   29a1b1c08:	mov    %rax,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:80
-   29a1b1bdb:	mov    (%rcx),%eax
-   29a1b1bdd:	cmp    %ebx,%eax
+   29a1b1c0b:	mov    (%rcx),%eax
+   29a1b1c0d:	cmp    %ebx,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:83
-   29a1b1bdf:	mov    0x10(%rcx),%rax
+   29a1b1c0f:	mov    0x10(%rcx),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:80
-   29a1b1be3:	jne    29a1b1bd0 <___w64_mingwthr_remove_key_dtor+0x40>
+   29a1b1c13:	jne    29a1b1c00 <___w64_mingwthr_remove_key_dtor+0x40>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:82
-   29a1b1be5:	test   %rdx,%rdx
-   29a1b1be8:	je     29a1b1c08 <___w64_mingwthr_remove_key_dtor+0x78>
+   29a1b1c15:	test   %rdx,%rdx
+   29a1b1c18:	je     29a1b1c38 <___w64_mingwthr_remove_key_dtor+0x78>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:85
-   29a1b1bea:	mov    %rax,0x10(%rdx)
+   29a1b1c1a:	mov    %rax,0x10(%rdx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:87
-   29a1b1bee:	call   29a1b24c0 <free>
+   29a1b1c1e:	call   29a1b2500 <free>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:94
-   29a1b1bf3:	mov    %rsi,%rcx
-   29a1b1bf6:	call   *0x766c(%rip)        # 29a1b9268 <__imp_LeaveCriticalSection>
+   29a1b1c23:	mov    %rsi,%rcx
+   29a1b1c26:	call   *0x7644(%rip)        # 29a1b9270 <__imp_LeaveCriticalSection>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:96
-   29a1b1bfc:	xor    %eax,%eax
-   29a1b1bfe:	add    $0x28,%rsp
-   29a1b1c02:	pop    %rbx
-   29a1b1c03:	pop    %rsi
-   29a1b1c04:	ret
-   29a1b1c05:	nopl   (%rax)
+   29a1b1c2c:	xor    %eax,%eax
+   29a1b1c2e:	add    $0x28,%rsp
+   29a1b1c32:	pop    %rbx
+   29a1b1c33:	pop    %rsi
+   29a1b1c34:	ret
+   29a1b1c35:	nopl   (%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:83
-   29a1b1c08:	mov    %rax,0x5471(%rip)        # 29a1b7080 <key_dtor_list>
-   29a1b1c0f:	jmp    29a1b1bee <___w64_mingwthr_remove_key_dtor+0x5e>
-   29a1b1c11:	data16 cs nopw 0x0(%rax,%rax,1)
-   29a1b1c1c:	nopl   0x0(%rax)
+   29a1b1c38:	mov    %rax,0x5441(%rip)        # 29a1b7080 <key_dtor_list>
+   29a1b1c3f:	jmp    29a1b1c1e <___w64_mingwthr_remove_key_dtor+0x5e>
+   29a1b1c41:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b1c4c:	nopl   0x0(%rax)
 
-000000029a1b1c20 <__mingw_TLScallback>:
+000000029a1b1c50 <__mingw_TLScallback>:
 __mingw_TLScallback():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:125
-   29a1b1c20:	push   %rbx
-   29a1b1c21:	sub    $0x20,%rsp
+   29a1b1c50:	push   %rbx
+   29a1b1c51:	sub    $0x20,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:126
-   29a1b1c25:	cmp    $0x2,%edx
-   29a1b1c28:	je     29a1b1ce0 <__mingw_TLScallback+0xc0>
-   29a1b1c2e:	ja     29a1b1c60 <__mingw_TLScallback+0x40>
-   29a1b1c30:	test   %edx,%edx
-   29a1b1c32:	je     29a1b1c80 <__mingw_TLScallback+0x60>
+   29a1b1c55:	cmp    $0x2,%edx
+   29a1b1c58:	je     29a1b1d10 <__mingw_TLScallback+0xc0>
+   29a1b1c5e:	ja     29a1b1c90 <__mingw_TLScallback+0x40>
+   29a1b1c60:	test   %edx,%edx
+   29a1b1c62:	je     29a1b1cb0 <__mingw_TLScallback+0x60>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:129
-   29a1b1c34:	mov    0x544e(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
-   29a1b1c3a:	test   %eax,%eax
-   29a1b1c3c:	je     29a1b1d00 <__mingw_TLScallback+0xe0>
+   29a1b1c64:	mov    0x541e(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1c6a:	test   %eax,%eax
+   29a1b1c6c:	je     29a1b1d30 <__mingw_TLScallback+0xe0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:131
-   29a1b1c42:	movl   $0x1,0x543c(%rip)        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1c72:	movl   $0x1,0x540c(%rip)        # 29a1b7088 <__mingwthr_cs_init>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:157
-   29a1b1c4c:	mov    $0x1,%eax
-   29a1b1c51:	add    $0x20,%rsp
-   29a1b1c55:	pop    %rbx
-   29a1b1c56:	ret
-   29a1b1c57:	nopw   0x0(%rax,%rax,1)
+   29a1b1c7c:	mov    $0x1,%eax
+   29a1b1c81:	add    $0x20,%rsp
+   29a1b1c85:	pop    %rbx
+   29a1b1c86:	ret
+   29a1b1c87:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:126
-   29a1b1c60:	cmp    $0x3,%edx
-   29a1b1c63:	jne    29a1b1c4c <__mingw_TLScallback+0x2c>
+   29a1b1c90:	cmp    $0x3,%edx
+   29a1b1c93:	jne    29a1b1c7c <__mingw_TLScallback+0x2c>
 __mingwthr_run_key_dtors():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:103
-   29a1b1c65:	mov    0x541d(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
-   29a1b1c6b:	test   %eax,%eax
-   29a1b1c6d:	je     29a1b1c4c <__mingw_TLScallback+0x2c>
-   29a1b1c6f:	call   29a1b1ab0 <__mingwthr_run_key_dtors.part.0>
-   29a1b1c74:	jmp    29a1b1c4c <__mingw_TLScallback+0x2c>
-   29a1b1c76:	cs nopw 0x0(%rax,%rax,1)
-   29a1b1c80:	mov    0x5402(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
-   29a1b1c86:	test   %eax,%eax
-   29a1b1c88:	jne    29a1b1cf0 <__mingw_TLScallback+0xd0>
+   29a1b1c95:	mov    0x53ed(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1c9b:	test   %eax,%eax
+   29a1b1c9d:	je     29a1b1c7c <__mingw_TLScallback+0x2c>
+   29a1b1c9f:	call   29a1b1ae0 <__mingwthr_run_key_dtors.part.0>
+   29a1b1ca4:	jmp    29a1b1c7c <__mingw_TLScallback+0x2c>
+   29a1b1ca6:	cs nopw 0x0(%rax,%rax,1)
+   29a1b1cb0:	mov    0x53d2(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1cb6:	test   %eax,%eax
+   29a1b1cb8:	jne    29a1b1d20 <__mingw_TLScallback+0xd0>
 __mingw_TLScallback():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:135
-   29a1b1c8a:	mov    0x53f8(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
-   29a1b1c90:	cmp    $0x1,%eax
-   29a1b1c93:	jne    29a1b1c4c <__mingw_TLScallback+0x2c>
+   29a1b1cba:	mov    0x53c8(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1cc0:	cmp    $0x1,%eax
+   29a1b1cc3:	jne    29a1b1c7c <__mingw_TLScallback+0x2c>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:138
-   29a1b1c95:	mov    0x53e4(%rip),%rbx        # 29a1b7080 <key_dtor_list>
-   29a1b1c9c:	test   %rbx,%rbx
-   29a1b1c9f:	je     29a1b1cb9 <__mingw_TLScallback+0x99>
-   29a1b1ca1:	nopl   0x0(%rax)
+   29a1b1cc5:	mov    0x53b4(%rip),%rbx        # 29a1b7080 <key_dtor_list>
+   29a1b1ccc:	test   %rbx,%rbx
+   29a1b1ccf:	je     29a1b1ce9 <__mingw_TLScallback+0x99>
+   29a1b1cd1:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:140
-   29a1b1ca8:	mov    %rbx,%rcx
-   29a1b1cab:	mov    0x10(%rbx),%rbx
+   29a1b1cd8:	mov    %rbx,%rcx
+   29a1b1cdb:	mov    0x10(%rbx),%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:141
-   29a1b1caf:	call   29a1b24c0 <free>
+   29a1b1cdf:	call   29a1b2500 <free>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:138
-   29a1b1cb4:	test   %rbx,%rbx
-   29a1b1cb7:	jne    29a1b1ca8 <__mingw_TLScallback+0x88>
+   29a1b1ce4:	test   %rbx,%rbx
+   29a1b1ce7:	jne    29a1b1cd8 <__mingw_TLScallback+0x88>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:146
-   29a1b1cb9:	lea    0x53e0(%rip),%rcx        # 29a1b70a0 <__mingwthr_cs>
+   29a1b1ce9:	lea    0x53b0(%rip),%rcx        # 29a1b70a0 <__mingwthr_cs>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:144
-   29a1b1cc0:	movq   $0x0,0x53b5(%rip)        # 29a1b7080 <key_dtor_list>
+   29a1b1cf0:	movq   $0x0,0x5385(%rip)        # 29a1b7080 <key_dtor_list>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:145
-   29a1b1ccb:	movl   $0x0,0x53b3(%rip)        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1cfb:	movl   $0x0,0x5383(%rip)        # 29a1b7088 <__mingwthr_cs_init>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:146
-   29a1b1cd5:	call   *0x756d(%rip)        # 29a1b9248 <__IAT_start__>
-   29a1b1cdb:	jmp    29a1b1c4c <__mingw_TLScallback+0x2c>
+   29a1b1d05:	call   *0x7545(%rip)        # 29a1b9250 <__IAT_start__>
+   29a1b1d0b:	jmp    29a1b1c7c <__mingw_TLScallback+0x2c>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:150
-   29a1b1ce0:	call   29a1b2120 <_fpreset>
+   29a1b1d10:	call   29a1b2150 <_fpreset>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:157
-   29a1b1ce5:	mov    $0x1,%eax
-   29a1b1cea:	add    $0x20,%rsp
-   29a1b1cee:	pop    %rbx
-   29a1b1cef:	ret
+   29a1b1d15:	mov    $0x1,%eax
+   29a1b1d1a:	add    $0x20,%rsp
+   29a1b1d1e:	pop    %rbx
+   29a1b1d1f:	ret
 __mingwthr_run_key_dtors():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:157
-   29a1b1cf0:	call   29a1b1ab0 <__mingwthr_run_key_dtors.part.0>
-   29a1b1cf5:	jmp    29a1b1c8a <__mingw_TLScallback+0x6a>
-   29a1b1cf7:	nopw   0x0(%rax,%rax,1)
+   29a1b1d20:	call   29a1b1ae0 <__mingwthr_run_key_dtors.part.0>
+   29a1b1d25:	jmp    29a1b1cba <__mingw_TLScallback+0x6a>
+   29a1b1d27:	nopw   0x0(%rax,%rax,1)
 __mingw_TLScallback():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:130
-   29a1b1d00:	lea    0x5399(%rip),%rcx        # 29a1b70a0 <__mingwthr_cs>
-   29a1b1d07:	call   *0x7553(%rip)        # 29a1b9260 <__imp_InitializeCriticalSection>
-   29a1b1d0d:	jmp    29a1b1c42 <__mingw_TLScallback+0x22>
-   29a1b1d12:	nop
-   29a1b1d13:	nop
-   29a1b1d14:	nop
-   29a1b1d15:	nop
-   29a1b1d16:	nop
-   29a1b1d17:	nop
-   29a1b1d18:	nop
-   29a1b1d19:	nop
-   29a1b1d1a:	nop
-   29a1b1d1b:	nop
-   29a1b1d1c:	nop
-   29a1b1d1d:	nop
-   29a1b1d1e:	nop
-   29a1b1d1f:	nop
+   29a1b1d30:	lea    0x5369(%rip),%rcx        # 29a1b70a0 <__mingwthr_cs>
+   29a1b1d37:	call   *0x752b(%rip)        # 29a1b9268 <__imp_InitializeCriticalSection>
+   29a1b1d3d:	jmp    29a1b1c72 <__mingw_TLScallback+0x22>
+   29a1b1d42:	nop
+   29a1b1d43:	nop
+   29a1b1d44:	nop
+   29a1b1d45:	nop
+   29a1b1d46:	nop
+   29a1b1d47:	nop
+   29a1b1d48:	nop
+   29a1b1d49:	nop
+   29a1b1d4a:	nop
+   29a1b1d4b:	nop
+   29a1b1d4c:	nop
+   29a1b1d4d:	nop
+   29a1b1d4e:	nop
+   29a1b1d4f:	nop
 
-000000029a1b1d20 <_ValidateImageBase>:
+000000029a1b1d50 <_ValidateImageBase>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:23
-   29a1b1d20:	xor    %eax,%eax
+   29a1b1d50:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1d22:	cmpw   $0x5a4d,(%rcx)
-   29a1b1d27:	jne    29a1b1d38 <_ValidateImageBase+0x18>
+   29a1b1d52:	cmpw   $0x5a4d,(%rcx)
+   29a1b1d57:	jne    29a1b1d68 <_ValidateImageBase+0x18>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1d29:	movslq 0x3c(%rcx),%rdx
-   29a1b1d2d:	add    %rdx,%rcx
+   29a1b1d59:	movslq 0x3c(%rcx),%rdx
+   29a1b1d5d:	add    %rdx,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1d30:	cmpl   $0x4550,(%rcx)
-   29a1b1d36:	je     29a1b1d40 <_ValidateImageBase+0x20>
+   29a1b1d60:	cmpl   $0x4550,(%rcx)
+   29a1b1d66:	je     29a1b1d70 <_ValidateImageBase+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:31
-   29a1b1d38:	ret
-   29a1b1d39:	nopl   0x0(%rax)
+   29a1b1d68:	ret
+   29a1b1d69:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b1d40:	xor    %eax,%eax
-   29a1b1d42:	cmpw   $0x20b,0x18(%rcx)
-   29a1b1d48:	sete   %al
+   29a1b1d70:	xor    %eax,%eax
+   29a1b1d72:	cmpw   $0x20b,0x18(%rcx)
+   29a1b1d78:	sete   %al
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:31
-   29a1b1d4b:	ret
-   29a1b1d4c:	nopl   0x0(%rax)
+   29a1b1d7b:	ret
+   29a1b1d7c:	nopl   0x0(%rax)
 
-000000029a1b1d50 <_FindPESection>:
+000000029a1b1d80 <_FindPESection>:
 _FindPESection():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:42
-   29a1b1d50:	movslq 0x3c(%rcx),%rax
-   29a1b1d54:	add    %rax,%rcx
+   29a1b1d80:	movslq 0x3c(%rcx),%rax
+   29a1b1d84:	add    %rax,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b1d57:	movzwl 0x14(%rcx),%eax
+   29a1b1d87:	movzwl 0x14(%rcx),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b1d5b:	movzwl 0x6(%rcx),%r8d
+   29a1b1d8b:	movzwl 0x6(%rcx),%r8d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b1d60:	lea    0x18(%rcx,%rax,1),%rax
+   29a1b1d90:	lea    0x18(%rcx,%rax,1),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b1d65:	test   %r8w,%r8w
-   29a1b1d69:	je     29a1b1d9d <_FindPESection+0x4d>
-   29a1b1d6b:	lea    -0x1(%r8),%ecx
-   29a1b1d6f:	lea    (%rcx,%rcx,4),%rcx
-   29a1b1d73:	lea    0x28(%rax,%rcx,8),%r9
-   29a1b1d78:	nopl   0x0(%rax,%rax,1)
+   29a1b1d95:	test   %r8w,%r8w
+   29a1b1d99:	je     29a1b1dcd <_FindPESection+0x4d>
+   29a1b1d9b:	lea    -0x1(%r8),%ecx
+   29a1b1d9f:	lea    (%rcx,%rcx,4),%rcx
+   29a1b1da3:	lea    0x28(%rax,%rcx,8),%r9
+   29a1b1da8:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:48
-   29a1b1d80:	mov    0xc(%rax),%r8d
-   29a1b1d84:	mov    %r8,%rcx
-   29a1b1d87:	cmp    %r8,%rdx
-   29a1b1d8a:	jb     29a1b1d94 <_FindPESection+0x44>
+   29a1b1db0:	mov    0xc(%rax),%r8d
+   29a1b1db4:	mov    %r8,%rcx
+   29a1b1db7:	cmp    %r8,%rdx
+   29a1b1dba:	jb     29a1b1dc4 <_FindPESection+0x44>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:49
-   29a1b1d8c:	add    0x8(%rax),%ecx
-   29a1b1d8f:	cmp    %rcx,%rdx
-   29a1b1d92:	jb     29a1b1d9f <_FindPESection+0x4f>
+   29a1b1dbc:	add    0x8(%rax),%ecx
+   29a1b1dbf:	cmp    %rcx,%rdx
+   29a1b1dc2:	jb     29a1b1dcf <_FindPESection+0x4f>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:46
-   29a1b1d94:	add    $0x28,%rax
+   29a1b1dc4:	add    $0x28,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b1d98:	cmp    %r9,%rax
-   29a1b1d9b:	jne    29a1b1d80 <_FindPESection+0x30>
+   29a1b1dc8:	cmp    %r9,%rax
+   29a1b1dcb:	jne    29a1b1db0 <_FindPESection+0x30>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:52
-   29a1b1d9d:	xor    %eax,%eax
+   29a1b1dcd:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:53
-   29a1b1d9f:	ret
+   29a1b1dcf:	ret
 
-000000029a1b1da0 <_FindPESectionByName>:
+000000029a1b1dd0 <_FindPESectionByName>:
 _FindPESectionByName():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:59
-   29a1b1da0:	push   %rdi
-   29a1b1da1:	push   %rsi
-   29a1b1da2:	push   %rbx
-   29a1b1da3:	sub    $0x20,%rsp
-   29a1b1da7:	mov    %rcx,%rsi
+   29a1b1dd0:	push   %rdi
+   29a1b1dd1:	push   %rsi
+   29a1b1dd2:	push   %rbx
+   29a1b1dd3:	sub    $0x20,%rsp
+   29a1b1dd7:	mov    %rcx,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:66
-   29a1b1daa:	call   29a1b23f0 <strlen>
-   29a1b1daf:	cmp    $0x8,%rax
-   29a1b1db3:	ja     29a1b1e30 <_FindPESectionByName+0x90>
+   29a1b1dda:	call   29a1b2420 <strlen>
+   29a1b1ddf:	cmp    $0x8,%rax
+   29a1b1de3:	ja     29a1b1e60 <_FindPESectionByName+0x90>
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1db5:	mov    0x2444(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1de5:	mov    0x2414(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
 _FindPESectionByName():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:67
-   29a1b1dbc:	xor    %ebx,%ebx
+   29a1b1dec:	xor    %ebx,%ebx
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1dbe:	cmpw   $0x5a4d,(%rdx)
-   29a1b1dc3:	jne    29a1b1e1e <_FindPESectionByName+0x7e>
+   29a1b1dee:	cmpw   $0x5a4d,(%rdx)
+   29a1b1df3:	jne    29a1b1e4e <_FindPESectionByName+0x7e>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1dc5:	movslq 0x3c(%rdx),%rax
-   29a1b1dc9:	add    %rdx,%rax
+   29a1b1df5:	movslq 0x3c(%rdx),%rax
+   29a1b1df9:	add    %rdx,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1dcc:	cmpl   $0x4550,(%rax)
-   29a1b1dd2:	jne    29a1b1e1e <_FindPESectionByName+0x7e>
+   29a1b1dfc:	cmpl   $0x4550,(%rax)
+   29a1b1e02:	jne    29a1b1e4e <_FindPESectionByName+0x7e>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b1dd4:	cmpw   $0x20b,0x18(%rax)
-   29a1b1dda:	jne    29a1b1e1e <_FindPESectionByName+0x7e>
+   29a1b1e04:	cmpw   $0x20b,0x18(%rax)
+   29a1b1e0a:	jne    29a1b1e4e <_FindPESectionByName+0x7e>
 _FindPESectionByName():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:75
-   29a1b1ddc:	movzwl 0x14(%rax),%edx
-   29a1b1de0:	lea    0x18(%rax,%rdx,1),%rbx
+   29a1b1e0c:	movzwl 0x14(%rax),%edx
+   29a1b1e10:	lea    0x18(%rax,%rdx,1),%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:76
-   29a1b1de5:	movzwl 0x6(%rax),%edx
-   29a1b1de9:	test   %dx,%dx
-   29a1b1dec:	je     29a1b1e30 <_FindPESectionByName+0x90>
-   29a1b1dee:	lea    -0x1(%rdx),%eax
-   29a1b1df1:	lea    (%rax,%rax,4),%rax
-   29a1b1df5:	lea    0x28(%rbx,%rax,8),%rdi
-   29a1b1dfa:	jmp    29a1b1e09 <_FindPESectionByName+0x69>
-   29a1b1dfc:	nopl   0x0(%rax)
+   29a1b1e15:	movzwl 0x6(%rax),%edx
+   29a1b1e19:	test   %dx,%dx
+   29a1b1e1c:	je     29a1b1e60 <_FindPESectionByName+0x90>
+   29a1b1e1e:	lea    -0x1(%rdx),%eax
+   29a1b1e21:	lea    (%rax,%rax,4),%rax
+   29a1b1e25:	lea    0x28(%rbx,%rax,8),%rdi
+   29a1b1e2a:	jmp    29a1b1e39 <_FindPESectionByName+0x69>
+   29a1b1e2c:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:77
-   29a1b1e00:	add    $0x28,%rbx
+   29a1b1e30:	add    $0x28,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:76
-   29a1b1e04:	cmp    %rdi,%rbx
-   29a1b1e07:	je     29a1b1e30 <_FindPESectionByName+0x90>
+   29a1b1e34:	cmp    %rdi,%rbx
+   29a1b1e37:	je     29a1b1e60 <_FindPESectionByName+0x90>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:79
-   29a1b1e09:	mov    $0x8,%r8d
-   29a1b1e0f:	mov    %rsi,%rdx
-   29a1b1e12:	mov    %rbx,%rcx
-   29a1b1e15:	call   29a1b23f8 <strncmp>
-   29a1b1e1a:	test   %eax,%eax
-   29a1b1e1c:	jne    29a1b1e00 <_FindPESectionByName+0x60>
+   29a1b1e39:	mov    $0x8,%r8d
+   29a1b1e3f:	mov    %rsi,%rdx
+   29a1b1e42:	mov    %rbx,%rcx
+   29a1b1e45:	call   29a1b2428 <strncmp>
+   29a1b1e4a:	test   %eax,%eax
+   29a1b1e4c:	jne    29a1b1e30 <_FindPESectionByName+0x60>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:83
-   29a1b1e1e:	mov    %rbx,%rax
-   29a1b1e21:	add    $0x20,%rsp
-   29a1b1e25:	pop    %rbx
-   29a1b1e26:	pop    %rsi
-   29a1b1e27:	pop    %rdi
-   29a1b1e28:	ret
-   29a1b1e29:	nopl   0x0(%rax)
+   29a1b1e4e:	mov    %rbx,%rax
+   29a1b1e51:	add    $0x20,%rsp
+   29a1b1e55:	pop    %rbx
+   29a1b1e56:	pop    %rsi
+   29a1b1e57:	pop    %rdi
+   29a1b1e58:	ret
+   29a1b1e59:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:67
-   29a1b1e30:	xor    %ebx,%ebx
+   29a1b1e60:	xor    %ebx,%ebx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:83
-   29a1b1e32:	mov    %rbx,%rax
-   29a1b1e35:	add    $0x20,%rsp
-   29a1b1e39:	pop    %rbx
-   29a1b1e3a:	pop    %rsi
-   29a1b1e3b:	pop    %rdi
-   29a1b1e3c:	ret
-   29a1b1e3d:	nopl   (%rax)
+   29a1b1e62:	mov    %rbx,%rax
+   29a1b1e65:	add    $0x20,%rsp
+   29a1b1e69:	pop    %rbx
+   29a1b1e6a:	pop    %rsi
+   29a1b1e6b:	pop    %rdi
+   29a1b1e6c:	ret
+   29a1b1e6d:	nopl   (%rax)
 
-000000029a1b1e40 <__mingw_GetSectionForAddress>:
+000000029a1b1e70 <__mingw_GetSectionForAddress>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1e40:	mov    0x23b9(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1e70:	mov    0x2389(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
 __mingw_GetSectionForAddress():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:96
-   29a1b1e47:	xor    %eax,%eax
+   29a1b1e77:	xor    %eax,%eax
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1e49:	cmpw   $0x5a4d,(%rdx)
-   29a1b1e4e:	jne    29a1b1e60 <__mingw_GetSectionForAddress+0x20>
+   29a1b1e79:	cmpw   $0x5a4d,(%rdx)
+   29a1b1e7e:	jne    29a1b1e90 <__mingw_GetSectionForAddress+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1e50:	movslq 0x3c(%rdx),%r8
-   29a1b1e54:	add    %rdx,%r8
+   29a1b1e80:	movslq 0x3c(%rdx),%r8
+   29a1b1e84:	add    %rdx,%r8
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1e57:	cmpl   $0x4550,(%r8)
-   29a1b1e5e:	je     29a1b1e68 <__mingw_GetSectionForAddress+0x28>
+   29a1b1e87:	cmpl   $0x4550,(%r8)
+   29a1b1e8e:	je     29a1b1e98 <__mingw_GetSectionForAddress+0x28>
 __mingw_GetSectionForAddress():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:100
-   29a1b1e60:	ret
-   29a1b1e61:	nopl   0x0(%rax)
+   29a1b1e90:	ret
+   29a1b1e91:	nopl   0x0(%rax)
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b1e68:	cmpw   $0x20b,0x18(%r8)
-   29a1b1e6f:	jne    29a1b1e60 <__mingw_GetSectionForAddress+0x20>
+   29a1b1e98:	cmpw   $0x20b,0x18(%r8)
+   29a1b1e9f:	jne    29a1b1e90 <__mingw_GetSectionForAddress+0x20>
 _FindPESection():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b1e71:	movzwl 0x14(%r8),%eax
+   29a1b1ea1:	movzwl 0x14(%r8),%eax
 __mingw_GetSectionForAddress():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:98
-   29a1b1e76:	sub    %rdx,%rcx
+   29a1b1ea6:	sub    %rdx,%rcx
 _FindPESection():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b1e79:	lea    0x18(%r8,%rax,1),%rax
+   29a1b1ea9:	lea    0x18(%r8,%rax,1),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b1e7e:	movzwl 0x6(%r8),%r8d
-   29a1b1e83:	test   %r8w,%r8w
-   29a1b1e87:	je     29a1b1ebd <__mingw_GetSectionForAddress+0x7d>
-   29a1b1e89:	lea    -0x1(%r8),%edx
-   29a1b1e8d:	lea    (%rdx,%rdx,4),%rdx
-   29a1b1e91:	lea    0x28(%rax,%rdx,8),%r9
-   29a1b1e96:	cs nopw 0x0(%rax,%rax,1)
+   29a1b1eae:	movzwl 0x6(%r8),%r8d
+   29a1b1eb3:	test   %r8w,%r8w
+   29a1b1eb7:	je     29a1b1eed <__mingw_GetSectionForAddress+0x7d>
+   29a1b1eb9:	lea    -0x1(%r8),%edx
+   29a1b1ebd:	lea    (%rdx,%rdx,4),%rdx
+   29a1b1ec1:	lea    0x28(%rax,%rdx,8),%r9
+   29a1b1ec6:	cs nopw 0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:48
-   29a1b1ea0:	mov    0xc(%rax),%r8d
-   29a1b1ea4:	mov    %r8,%rdx
-   29a1b1ea7:	cmp    %r8,%rcx
-   29a1b1eaa:	jb     29a1b1eb4 <__mingw_GetSectionForAddress+0x74>
+   29a1b1ed0:	mov    0xc(%rax),%r8d
+   29a1b1ed4:	mov    %r8,%rdx
+   29a1b1ed7:	cmp    %r8,%rcx
+   29a1b1eda:	jb     29a1b1ee4 <__mingw_GetSectionForAddress+0x74>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:49
-   29a1b1eac:	add    0x8(%rax),%edx
-   29a1b1eaf:	cmp    %rdx,%rcx
-   29a1b1eb2:	jb     29a1b1e60 <__mingw_GetSectionForAddress+0x20>
+   29a1b1edc:	add    0x8(%rax),%edx
+   29a1b1edf:	cmp    %rdx,%rcx
+   29a1b1ee2:	jb     29a1b1e90 <__mingw_GetSectionForAddress+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:46
-   29a1b1eb4:	add    $0x28,%rax
+   29a1b1ee4:	add    $0x28,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b1eb8:	cmp    %r9,%rax
-   29a1b1ebb:	jne    29a1b1ea0 <__mingw_GetSectionForAddress+0x60>
+   29a1b1ee8:	cmp    %r9,%rax
+   29a1b1eeb:	jne    29a1b1ed0 <__mingw_GetSectionForAddress+0x60>
 __mingw_GetSectionForAddress():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:96
-   29a1b1ebd:	xor    %eax,%eax
+   29a1b1eed:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:100
-   29a1b1ebf:	ret
+   29a1b1eef:	ret
 
-000000029a1b1ec0 <__mingw_GetSectionCount>:
+000000029a1b1ef0 <__mingw_GetSectionCount>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1ec0:	mov    0x2339(%rip),%rax        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1ef0:	mov    0x2309(%rip),%rax        # 29a1b4200 <.refptr.__ImageBase>
 __mingw_GetSectionCount():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:110
-   29a1b1ec7:	xor    %ecx,%ecx
+   29a1b1ef7:	xor    %ecx,%ecx
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1ec9:	cmpw   $0x5a4d,(%rax)
-   29a1b1ece:	jne    29a1b1edf <__mingw_GetSectionCount+0x1f>
+   29a1b1ef9:	cmpw   $0x5a4d,(%rax)
+   29a1b1efe:	jne    29a1b1f0f <__mingw_GetSectionCount+0x1f>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1ed0:	movslq 0x3c(%rax),%rdx
-   29a1b1ed4:	add    %rdx,%rax
+   29a1b1f00:	movslq 0x3c(%rax),%rdx
+   29a1b1f04:	add    %rdx,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1ed7:	cmpl   $0x4550,(%rax)
-   29a1b1edd:	je     29a1b1ee8 <__mingw_GetSectionCount+0x28>
+   29a1b1f07:	cmpl   $0x4550,(%rax)
+   29a1b1f0d:	je     29a1b1f18 <__mingw_GetSectionCount+0x28>
 __mingw_GetSectionCount():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:115
-   29a1b1edf:	mov    %ecx,%eax
-   29a1b1ee1:	ret
-   29a1b1ee2:	nopw   0x0(%rax,%rax,1)
+   29a1b1f0f:	mov    %ecx,%eax
+   29a1b1f11:	ret
+   29a1b1f12:	nopw   0x0(%rax,%rax,1)
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b1ee8:	cmpw   $0x20b,0x18(%rax)
-   29a1b1eee:	jne    29a1b1edf <__mingw_GetSectionCount+0x1f>
+   29a1b1f18:	cmpw   $0x20b,0x18(%rax)
+   29a1b1f1e:	jne    29a1b1f0f <__mingw_GetSectionCount+0x1f>
 __mingw_GetSectionCount():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:114
-   29a1b1ef0:	movzwl 0x6(%rax),%ecx
+   29a1b1f20:	movzwl 0x6(%rax),%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:115
-   29a1b1ef4:	mov    %ecx,%eax
-   29a1b1ef6:	ret
-   29a1b1ef7:	nopw   0x0(%rax,%rax,1)
+   29a1b1f24:	mov    %ecx,%eax
+   29a1b1f26:	ret
+   29a1b1f27:	nopw   0x0(%rax,%rax,1)
 
-000000029a1b1f00 <_FindPESectionExec>:
+000000029a1b1f30 <_FindPESectionExec>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1f00:	mov    0x22f9(%rip),%r8        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1f30:	mov    0x22c9(%rip),%r8        # 29a1b4200 <.refptr.__ImageBase>
 _FindPESectionExec():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:130
-   29a1b1f07:	xor    %eax,%eax
+   29a1b1f37:	xor    %eax,%eax
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1f09:	cmpw   $0x5a4d,(%r8)
-   29a1b1f0f:	jne    29a1b1f20 <_FindPESectionExec+0x20>
+   29a1b1f39:	cmpw   $0x5a4d,(%r8)
+   29a1b1f3f:	jne    29a1b1f50 <_FindPESectionExec+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1f11:	movslq 0x3c(%r8),%rdx
-   29a1b1f15:	add    %r8,%rdx
+   29a1b1f41:	movslq 0x3c(%r8),%rdx
+   29a1b1f45:	add    %r8,%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1f18:	cmpl   $0x4550,(%rdx)
-   29a1b1f1e:	je     29a1b1f28 <_FindPESectionExec+0x28>
+   29a1b1f48:	cmpl   $0x4550,(%rdx)
+   29a1b1f4e:	je     29a1b1f58 <_FindPESectionExec+0x28>
 _FindPESectionExec():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:146
-   29a1b1f20:	ret
-   29a1b1f21:	nopl   0x0(%rax)
+   29a1b1f50:	ret
+   29a1b1f51:	nopl   0x0(%rax)
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b1f28:	cmpw   $0x20b,0x18(%rdx)
-   29a1b1f2e:	jne    29a1b1f20 <_FindPESectionExec+0x20>
+   29a1b1f58:	cmpw   $0x20b,0x18(%rdx)
+   29a1b1f5e:	jne    29a1b1f50 <_FindPESectionExec+0x20>
 _FindPESectionExec():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:134
-   29a1b1f30:	movzwl 0x14(%rdx),%eax
+   29a1b1f60:	movzwl 0x14(%rdx),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:135
-   29a1b1f34:	movzwl 0x6(%rdx),%r8d
+   29a1b1f64:	movzwl 0x6(%rdx),%r8d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:134
-   29a1b1f39:	lea    0x18(%rdx,%rax,1),%rax
+   29a1b1f69:	lea    0x18(%rdx,%rax,1),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:135
-   29a1b1f3e:	test   %r8w,%r8w
-   29a1b1f42:	je     29a1b1f70 <_FindPESectionExec+0x70>
-   29a1b1f44:	lea    -0x1(%r8),%edx
-   29a1b1f48:	lea    (%rdx,%rdx,4),%rdx
-   29a1b1f4c:	lea    0x28(%rax,%rdx,8),%rdx
-   29a1b1f51:	nopl   0x0(%rax)
+   29a1b1f6e:	test   %r8w,%r8w
+   29a1b1f72:	je     29a1b1fa0 <_FindPESectionExec+0x70>
+   29a1b1f74:	lea    -0x1(%r8),%edx
+   29a1b1f78:	lea    (%rdx,%rdx,4),%rdx
+   29a1b1f7c:	lea    0x28(%rax,%rdx,8),%rdx
+   29a1b1f81:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:138
-   29a1b1f58:	testb  $0x20,0x27(%rax)
-   29a1b1f5c:	je     29a1b1f67 <_FindPESectionExec+0x67>
+   29a1b1f88:	testb  $0x20,0x27(%rax)
+   29a1b1f8c:	je     29a1b1f97 <_FindPESectionExec+0x67>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:140
-   29a1b1f5e:	test   %rcx,%rcx
-   29a1b1f61:	je     29a1b1f20 <_FindPESectionExec+0x20>
+   29a1b1f8e:	test   %rcx,%rcx
+   29a1b1f91:	je     29a1b1f50 <_FindPESectionExec+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:142
-   29a1b1f63:	sub    $0x1,%rcx
+   29a1b1f93:	sub    $0x1,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:136
-   29a1b1f67:	add    $0x28,%rax
+   29a1b1f97:	add    $0x28,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:135
-   29a1b1f6b:	cmp    %rax,%rdx
-   29a1b1f6e:	jne    29a1b1f58 <_FindPESectionExec+0x58>
+   29a1b1f9b:	cmp    %rax,%rdx
+   29a1b1f9e:	jne    29a1b1f88 <_FindPESectionExec+0x58>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:130
-   29a1b1f70:	xor    %eax,%eax
+   29a1b1fa0:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:146
-   29a1b1f72:	ret
-   29a1b1f73:	data16 cs nopw 0x0(%rax,%rax,1)
-   29a1b1f7e:	xchg   %ax,%ax
+   29a1b1fa2:	ret
+   29a1b1fa3:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b1fae:	xchg   %ax,%ax
 
-000000029a1b1f80 <_GetPEImageBase>:
+000000029a1b1fb0 <_GetPEImageBase>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1f80:	mov    0x2279(%rip),%rax        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1fb0:	mov    0x2249(%rip),%rax        # 29a1b4200 <.refptr.__ImageBase>
 _GetPEImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:156
-   29a1b1f87:	xor    %edx,%edx
+   29a1b1fb7:	xor    %edx,%edx
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1f89:	cmpw   $0x5a4d,(%rax)
-   29a1b1f8e:	jne    29a1b1f9f <_GetPEImageBase+0x1f>
+   29a1b1fb9:	cmpw   $0x5a4d,(%rax)
+   29a1b1fbe:	jne    29a1b1fcf <_GetPEImageBase+0x1f>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1f90:	movslq 0x3c(%rax),%rcx
-   29a1b1f94:	add    %rax,%rcx
+   29a1b1fc0:	movslq 0x3c(%rax),%rcx
+   29a1b1fc4:	add    %rax,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1f97:	cmpl   $0x4550,(%rcx)
-   29a1b1f9d:	je     29a1b1fa8 <_GetPEImageBase+0x28>
+   29a1b1fc7:	cmpl   $0x4550,(%rcx)
+   29a1b1fcd:	je     29a1b1fd8 <_GetPEImageBase+0x28>
 _GetPEImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:158
-   29a1b1f9f:	mov    %rdx,%rax
-   29a1b1fa2:	ret
-   29a1b1fa3:	nopl   0x0(%rax,%rax,1)
+   29a1b1fcf:	mov    %rdx,%rax
+   29a1b1fd2:	ret
+   29a1b1fd3:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:157
-   29a1b1fa8:	cmpw   $0x20b,0x18(%rcx)
-   29a1b1fae:	cmove  %rax,%rdx
+   29a1b1fd8:	cmpw   $0x20b,0x18(%rcx)
+   29a1b1fde:	cmove  %rax,%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:158
-   29a1b1fb2:	mov    %rdx,%rax
-   29a1b1fb5:	ret
-   29a1b1fb6:	cs nopw 0x0(%rax,%rax,1)
+   29a1b1fe2:	mov    %rdx,%rax
+   29a1b1fe5:	ret
+   29a1b1fe6:	cs nopw 0x0(%rax,%rax,1)
 
-000000029a1b1fc0 <_IsNonwritableInCurrentImage>:
+000000029a1b1ff0 <_IsNonwritableInCurrentImage>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1fc0:	mov    0x2239(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1ff0:	mov    0x2209(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
 _IsNonwritableInCurrentImage():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:171
-   29a1b1fc7:	xor    %eax,%eax
+   29a1b1ff7:	xor    %eax,%eax
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1fc9:	cmpw   $0x5a4d,(%rdx)
-   29a1b1fce:	jne    29a1b1fe0 <_IsNonwritableInCurrentImage+0x20>
+   29a1b1ff9:	cmpw   $0x5a4d,(%rdx)
+   29a1b1ffe:	jne    29a1b2010 <_IsNonwritableInCurrentImage+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1fd0:	movslq 0x3c(%rdx),%r8
-   29a1b1fd4:	add    %rdx,%r8
+   29a1b2000:	movslq 0x3c(%rdx),%r8
+   29a1b2004:	add    %rdx,%r8
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1fd7:	cmpl   $0x4550,(%r8)
-   29a1b1fde:	je     29a1b1fe8 <_IsNonwritableInCurrentImage+0x28>
+   29a1b2007:	cmpl   $0x4550,(%r8)
+   29a1b200e:	je     29a1b2018 <_IsNonwritableInCurrentImage+0x28>
 _IsNonwritableInCurrentImage():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:177
-   29a1b1fe0:	ret
-   29a1b1fe1:	nopl   0x0(%rax)
+   29a1b2010:	ret
+   29a1b2011:	nopl   0x0(%rax)
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b1fe8:	cmpw   $0x20b,0x18(%r8)
-   29a1b1fef:	jne    29a1b1fe0 <_IsNonwritableInCurrentImage+0x20>
+   29a1b2018:	cmpw   $0x20b,0x18(%r8)
+   29a1b201f:	jne    29a1b2010 <_IsNonwritableInCurrentImage+0x20>
 _IsNonwritableInCurrentImage():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:172
-   29a1b1ff1:	sub    %rdx,%rcx
+   29a1b2021:	sub    %rdx,%rcx
 _FindPESection():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b1ff4:	movzwl 0x6(%r8),%r9d
+   29a1b2024:	movzwl 0x6(%r8),%r9d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b1ff9:	movzwl 0x14(%r8),%edx
-   29a1b1ffe:	lea    0x18(%r8,%rdx,1),%rdx
+   29a1b2029:	movzwl 0x14(%r8),%edx
+   29a1b202e:	lea    0x18(%r8,%rdx,1),%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b2003:	test   %r9w,%r9w
-   29a1b2007:	je     29a1b1fe0 <_IsNonwritableInCurrentImage+0x20>
-   29a1b2009:	lea    -0x1(%r9),%eax
-   29a1b200d:	lea    (%rax,%rax,4),%rax
-   29a1b2011:	lea    0x28(%rdx,%rax,8),%r9
-   29a1b2016:	cs nopw 0x0(%rax,%rax,1)
+   29a1b2033:	test   %r9w,%r9w
+   29a1b2037:	je     29a1b2010 <_IsNonwritableInCurrentImage+0x20>
+   29a1b2039:	lea    -0x1(%r9),%eax
+   29a1b203d:	lea    (%rax,%rax,4),%rax
+   29a1b2041:	lea    0x28(%rdx,%rax,8),%r9
+   29a1b2046:	cs nopw 0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:48
-   29a1b2020:	mov    0xc(%rdx),%r8d
-   29a1b2024:	mov    %r8,%rax
-   29a1b2027:	cmp    %r8,%rcx
-   29a1b202a:	jb     29a1b2034 <_IsNonwritableInCurrentImage+0x74>
+   29a1b2050:	mov    0xc(%rdx),%r8d
+   29a1b2054:	mov    %r8,%rax
+   29a1b2057:	cmp    %r8,%rcx
+   29a1b205a:	jb     29a1b2064 <_IsNonwritableInCurrentImage+0x74>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:49
-   29a1b202c:	add    0x8(%rdx),%eax
-   29a1b202f:	cmp    %rax,%rcx
-   29a1b2032:	jb     29a1b2040 <_IsNonwritableInCurrentImage+0x80>
+   29a1b205c:	add    0x8(%rdx),%eax
+   29a1b205f:	cmp    %rax,%rcx
+   29a1b2062:	jb     29a1b2070 <_IsNonwritableInCurrentImage+0x80>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:46
-   29a1b2034:	add    $0x28,%rdx
+   29a1b2064:	add    $0x28,%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b2038:	cmp    %r9,%rdx
-   29a1b203b:	jne    29a1b2020 <_IsNonwritableInCurrentImage+0x60>
+   29a1b2068:	cmp    %r9,%rdx
+   29a1b206b:	jne    29a1b2050 <_IsNonwritableInCurrentImage+0x60>
 _IsNonwritableInCurrentImage():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:171
-   29a1b203d:	xor    %eax,%eax
+   29a1b206d:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:177
-   29a1b203f:	ret
+   29a1b206f:	ret
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:176
-   29a1b2040:	mov    0x24(%rdx),%eax
-   29a1b2043:	not    %eax
-   29a1b2045:	shr    $0x1f,%eax
+   29a1b2070:	mov    0x24(%rdx),%eax
+   29a1b2073:	not    %eax
+   29a1b2075:	shr    $0x1f,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:177
-   29a1b2048:	ret
-   29a1b2049:	nopl   0x0(%rax)
+   29a1b2078:	ret
+   29a1b2079:	nopl   0x0(%rax)
 
-000000029a1b2050 <__mingw_enum_import_library_names>:
+000000029a1b2080 <__mingw_enum_import_library_names>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b2050:	mov    0x21a9(%rip),%r11        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b2080:	mov    0x2179(%rip),%r11        # 29a1b4200 <.refptr.__ImageBase>
 __mingw_enum_import_library_names():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:193
-   29a1b2057:	xor    %r9d,%r9d
+   29a1b2087:	xor    %r9d,%r9d
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b205a:	cmpw   $0x5a4d,(%r11)
-   29a1b2060:	jne    29a1b2072 <__mingw_enum_import_library_names+0x22>
+   29a1b208a:	cmpw   $0x5a4d,(%r11)
+   29a1b2090:	jne    29a1b20a2 <__mingw_enum_import_library_names+0x22>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b2062:	movslq 0x3c(%r11),%r8
-   29a1b2066:	add    %r11,%r8
+   29a1b2092:	movslq 0x3c(%r11),%r8
+   29a1b2096:	add    %r11,%r8
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b2069:	cmpl   $0x4550,(%r8)
-   29a1b2070:	je     29a1b2080 <__mingw_enum_import_library_names+0x30>
+   29a1b2099:	cmpl   $0x4550,(%r8)
+   29a1b20a0:	je     29a1b20b0 <__mingw_enum_import_library_names+0x30>
 __mingw_enum_import_library_names():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:221
-   29a1b2072:	mov    %r9,%rax
-   29a1b2075:	ret
-   29a1b2076:	cs nopw 0x0(%rax,%rax,1)
+   29a1b20a2:	mov    %r9,%rax
+   29a1b20a5:	ret
+   29a1b20a6:	cs nopw 0x0(%rax,%rax,1)
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b2080:	cmpw   $0x20b,0x18(%r8)
-   29a1b2087:	jne    29a1b2072 <__mingw_enum_import_library_names+0x22>
+   29a1b20b0:	cmpw   $0x20b,0x18(%r8)
+   29a1b20b7:	jne    29a1b20a2 <__mingw_enum_import_library_names+0x22>
 __mingw_enum_import_library_names():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:197
-   29a1b2089:	mov    0x90(%r8),%eax
+   29a1b20b9:	mov    0x90(%r8),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:198
-   29a1b2090:	test   %eax,%eax
-   29a1b2092:	je     29a1b2072 <__mingw_enum_import_library_names+0x22>
+   29a1b20c0:	test   %eax,%eax
+   29a1b20c2:	je     29a1b20a2 <__mingw_enum_import_library_names+0x22>
 _FindPESection():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b2094:	movzwl 0x14(%r8),%edx
+   29a1b20c4:	movzwl 0x14(%r8),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b2099:	movzwl 0x6(%r8),%r10d
+   29a1b20c9:	movzwl 0x6(%r8),%r10d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b209e:	lea    0x18(%r8,%rdx,1),%rdx
+   29a1b20ce:	lea    0x18(%r8,%rdx,1),%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b20a3:	test   %r10w,%r10w
-   29a1b20a7:	je     29a1b2072 <__mingw_enum_import_library_names+0x22>
-   29a1b20a9:	lea    -0x1(%r10),%r8d
-   29a1b20ad:	lea    (%r8,%r8,4),%r8
-   29a1b20b1:	lea    0x28(%rdx,%r8,8),%r10
-   29a1b20b6:	cs nopw 0x0(%rax,%rax,1)
+   29a1b20d3:	test   %r10w,%r10w
+   29a1b20d7:	je     29a1b20a2 <__mingw_enum_import_library_names+0x22>
+   29a1b20d9:	lea    -0x1(%r10),%r8d
+   29a1b20dd:	lea    (%r8,%r8,4),%r8
+   29a1b20e1:	lea    0x28(%rdx,%r8,8),%r10
+   29a1b20e6:	cs nopw 0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:48
-   29a1b20c0:	mov    0xc(%rdx),%r9d
-   29a1b20c4:	mov    %r9,%r8
-   29a1b20c7:	cmp    %r9,%rax
-   29a1b20ca:	jb     29a1b20d5 <__mingw_enum_import_library_names+0x85>
+   29a1b20f0:	mov    0xc(%rdx),%r9d
+   29a1b20f4:	mov    %r9,%r8
+   29a1b20f7:	cmp    %r9,%rax
+   29a1b20fa:	jb     29a1b2105 <__mingw_enum_import_library_names+0x85>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:49
-   29a1b20cc:	add    0x8(%rdx),%r8d
-   29a1b20d0:	cmp    %r8,%rax
-   29a1b20d3:	jb     29a1b20e8 <__mingw_enum_import_library_names+0x98>
+   29a1b20fc:	add    0x8(%rdx),%r8d
+   29a1b2100:	cmp    %r8,%rax
+   29a1b2103:	jb     29a1b2118 <__mingw_enum_import_library_names+0x98>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:46
-   29a1b20d5:	add    $0x28,%rdx
+   29a1b2105:	add    $0x28,%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b20d9:	cmp    %rdx,%r10
-   29a1b20dc:	jne    29a1b20c0 <__mingw_enum_import_library_names+0x70>
+   29a1b2109:	cmp    %rdx,%r10
+   29a1b210c:	jne    29a1b20f0 <__mingw_enum_import_library_names+0x70>
 __mingw_enum_import_library_names():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:193
-   29a1b20de:	xor    %r9d,%r9d
+   29a1b210e:	xor    %r9d,%r9d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:221
-   29a1b20e1:	mov    %r9,%rax
-   29a1b20e4:	ret
-   29a1b20e5:	nopl   (%rax)
+   29a1b2111:	mov    %r9,%rax
+   29a1b2114:	ret
+   29a1b2115:	nopl   (%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:205
-   29a1b20e8:	add    %r11,%rax
+   29a1b2118:	add    %r11,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:206
-   29a1b20eb:	jmp    29a1b20f7 <__mingw_enum_import_library_names+0xa7>
-   29a1b20ed:	nopl   (%rax)
+   29a1b211b:	jmp    29a1b2127 <__mingw_enum_import_library_names+0xa7>
+   29a1b211d:	nopl   (%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:216
-   29a1b20f0:	sub    $0x1,%ecx
+   29a1b2120:	sub    $0x1,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:217
-   29a1b20f3:	add    $0x14,%rax
+   29a1b2123:	add    $0x14,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:211
-   29a1b20f7:	mov    0x4(%rax),%r8d
-   29a1b20fb:	test   %r8d,%r8d
-   29a1b20fe:	jne    29a1b2107 <__mingw_enum_import_library_names+0xb7>
-   29a1b2100:	mov    0xc(%rax),%edx
-   29a1b2103:	test   %edx,%edx
-   29a1b2105:	je     29a1b20de <__mingw_enum_import_library_names+0x8e>
+   29a1b2127:	mov    0x4(%rax),%r8d
+   29a1b212b:	test   %r8d,%r8d
+   29a1b212e:	jne    29a1b2137 <__mingw_enum_import_library_names+0xb7>
+   29a1b2130:	mov    0xc(%rax),%edx
+   29a1b2133:	test   %edx,%edx
+   29a1b2135:	je     29a1b210e <__mingw_enum_import_library_names+0x8e>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:214
-   29a1b2107:	test   %ecx,%ecx
-   29a1b2109:	jg     29a1b20f0 <__mingw_enum_import_library_names+0xa0>
+   29a1b2137:	test   %ecx,%ecx
+   29a1b2139:	jg     29a1b2120 <__mingw_enum_import_library_names+0xa0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:215
-   29a1b210b:	mov    0xc(%rax),%r9d
-   29a1b210f:	add    %r11,%r9
+   29a1b213b:	mov    0xc(%rax),%r9d
+   29a1b213f:	add    %r11,%r9
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:221
-   29a1b2112:	mov    %r9,%rax
-   29a1b2115:	ret
-   29a1b2116:	nop
-   29a1b2117:	nop
-   29a1b2118:	nop
-   29a1b2119:	nop
-   29a1b211a:	nop
-   29a1b211b:	nop
-   29a1b211c:	nop
-   29a1b211d:	nop
-   29a1b211e:	nop
-   29a1b211f:	nop
+   29a1b2142:	mov    %r9,%rax
+   29a1b2145:	ret
+   29a1b2146:	nop
+   29a1b2147:	nop
+   29a1b2148:	nop
+   29a1b2149:	nop
+   29a1b214a:	nop
+   29a1b214b:	nop
+   29a1b214c:	nop
+   29a1b214d:	nop
+   29a1b214e:	nop
+   29a1b214f:	nop
 
-000000029a1b2120 <_fpreset>:
+000000029a1b2150 <_fpreset>:
 _fpreset():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/CRT_fp10.c:19
-   29a1b2120:	fninit
+   29a1b2150:	fninit
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/CRT_fp10.c:24
-   29a1b2122:	ret
-   29a1b2123:	nop
-   29a1b2124:	nop
-   29a1b2125:	nop
-   29a1b2126:	nop
-   29a1b2127:	nop
-   29a1b2128:	nop
-   29a1b2129:	nop
-   29a1b212a:	nop
-   29a1b212b:	nop
-   29a1b212c:	nop
-   29a1b212d:	nop
-   29a1b212e:	nop
-   29a1b212f:	nop
-
-000000029a1b2130 <___chkstk_ms>:
-   29a1b2130:	push   %rcx
-   29a1b2131:	push   %rax
-   29a1b2132:	cmp    $0x1000,%rax
-   29a1b2138:	lea    0x18(%rsp),%rcx
-   29a1b213d:	jb     29a1b2158 <___chkstk_ms+0x28>
-   29a1b213f:	sub    $0x1000,%rcx
-   29a1b2146:	orq    $0x0,(%rcx)
-   29a1b214a:	sub    $0x1000,%rax
-   29a1b2150:	cmp    $0x1000,%rax
-   29a1b2156:	ja     29a1b213f <___chkstk_ms+0xf>
-   29a1b2158:	sub    %rax,%rcx
-   29a1b215b:	orq    $0x0,(%rcx)
-   29a1b215f:	pop    %rax
-   29a1b2160:	pop    %rcx
-   29a1b2161:	ret
-   29a1b2162:	nop
-   29a1b2163:	nop
-   29a1b2164:	nop
-   29a1b2165:	nop
-   29a1b2166:	nop
-   29a1b2167:	nop
-   29a1b2168:	nop
-   29a1b2169:	nop
-   29a1b216a:	nop
-   29a1b216b:	nop
-   29a1b216c:	nop
-   29a1b216d:	nop
-   29a1b216e:	nop
-   29a1b216f:	nop
+   29a1b2152:	ret
+   29a1b2153:	nop
+   29a1b2154:	nop
+   29a1b2155:	nop
+   29a1b2156:	nop
+   29a1b2157:	nop
+   29a1b2158:	nop
+   29a1b2159:	nop
+   29a1b215a:	nop
+   29a1b215b:	nop
+   29a1b215c:	nop
+   29a1b215d:	nop
+   29a1b215e:	nop
+   29a1b215f:	nop
+
+000000029a1b2160 <___chkstk_ms>:
+   29a1b2160:	push   %rcx
+   29a1b2161:	push   %rax
+   29a1b2162:	cmp    $0x1000,%rax
+   29a1b2168:	lea    0x18(%rsp),%rcx
+   29a1b216d:	jb     29a1b2188 <___chkstk_ms+0x28>
+   29a1b216f:	sub    $0x1000,%rcx
+   29a1b2176:	orq    $0x0,(%rcx)
+   29a1b217a:	sub    $0x1000,%rax
+   29a1b2180:	cmp    $0x1000,%rax
+   29a1b2186:	ja     29a1b216f <___chkstk_ms+0xf>
+   29a1b2188:	sub    %rax,%rcx
+   29a1b218b:	orq    $0x0,(%rcx)
+   29a1b218f:	pop    %rax
+   29a1b2190:	pop    %rcx
+   29a1b2191:	ret
+   29a1b2192:	nop
+   29a1b2193:	nop
+   29a1b2194:	nop
+   29a1b2195:	nop
+   29a1b2196:	nop
+   29a1b2197:	nop
+   29a1b2198:	nop
+   29a1b2199:	nop
+   29a1b219a:	nop
+   29a1b219b:	nop
+   29a1b219c:	nop
+   29a1b219d:	nop
+   29a1b219e:	nop
+   29a1b219f:	nop
 
-000000029a1b2170 <DllEntryPoint>:
+000000029a1b21a0 <DllEntryPoint>:
 DllEntryPoint():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/dllentry.c:18
-   29a1b2170:	mov    $0x1,%eax
-   29a1b2175:	ret
-   29a1b2176:	nop
-   29a1b2177:	nop
-   29a1b2178:	nop
-   29a1b2179:	nop
-   29a1b217a:	nop
-   29a1b217b:	nop
-   29a1b217c:	nop
-   29a1b217d:	nop
-   29a1b217e:	nop
-   29a1b217f:	nop
+   29a1b21a0:	mov    $0x1,%eax
+   29a1b21a5:	ret
+   29a1b21a6:	nop
+   29a1b21a7:	nop
+   29a1b21a8:	nop
+   29a1b21a9:	nop
+   29a1b21aa:	nop
+   29a1b21ab:	nop
+   29a1b21ac:	nop
+   29a1b21ad:	nop
+   29a1b21ae:	nop
+   29a1b21af:	nop
 
-000000029a1b2180 <DllMain>:
+000000029a1b21b0 <DllMain>:
 DllMain():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/dllmain.c:10
-   29a1b2180:	mov    $0x1,%eax
-   29a1b2185:	ret
-   29a1b2186:	nop
-   29a1b2187:	nop
-   29a1b2188:	nop
-   29a1b2189:	nop
-   29a1b218a:	nop
-   29a1b218b:	nop
-   29a1b218c:	nop
-   29a1b218d:	nop
-   29a1b218e:	nop
-   29a1b218f:	nop
+   29a1b21b0:	mov    $0x1,%eax
+   29a1b21b5:	ret
+   29a1b21b6:	nop
+   29a1b21b7:	nop
+   29a1b21b8:	nop
+   29a1b21b9:	nop
+   29a1b21ba:	nop
+   29a1b21bb:	nop
+   29a1b21bc:	nop
+   29a1b21bd:	nop
+   29a1b21be:	nop
+   29a1b21bf:	nop
 
-000000029a1b2190 <vfprintf>:
+000000029a1b21c0 <vfprintf>:
 vfprintf():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_vfprintf.c:12
-   29a1b2190:	sub    $0x38,%rsp
+   29a1b21c0:	sub    $0x38,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_vfprintf.c:13
-   29a1b2194:	xor    %r9d,%r9d
-   29a1b2197:	mov    %r8,0x20(%rsp)
-   29a1b219c:	mov    %rdx,%r8
-   29a1b219f:	mov    %rcx,%rdx
-   29a1b21a2:	xor    %ecx,%ecx
-   29a1b21a4:	call   29a1b2408 <__stdio_common_vfprintf>
+   29a1b21c4:	xor    %r9d,%r9d
+   29a1b21c7:	mov    %r8,0x20(%rsp)
+   29a1b21cc:	mov    %rdx,%r8
+   29a1b21cf:	mov    %rcx,%rdx
+   29a1b21d2:	xor    %ecx,%ecx
+   29a1b21d4:	call   29a1b2438 <__stdio_common_vfprintf>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_vfprintf.c:14
-   29a1b21a9:	add    $0x38,%rsp
-   29a1b21ad:	ret
-   29a1b21ae:	nop
-   29a1b21af:	nop
+   29a1b21d9:	add    $0x38,%rsp
+   29a1b21dd:	ret
+   29a1b21de:	nop
+   29a1b21df:	nop
 
-000000029a1b21b0 <_get_output_format>:
+000000029a1b21e0 <_get_output_format>:
 _get_output_format():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:113
-   29a1b21b0:	xor    %eax,%eax
-   29a1b21b2:	ret
-   29a1b21b3:	data16 cs nopw 0x0(%rax,%rax,1)
-   29a1b21be:	xchg   %ax,%ax
+   29a1b21e0:	xor    %eax,%eax
+   29a1b21e2:	ret
+   29a1b21e3:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b21ee:	xchg   %ax,%ax
 
-000000029a1b21c0 <__getmainargs>:
+000000029a1b21f0 <__getmainargs>:
 __getmainargs():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:63
-   29a1b21c0:	push   %r12
-   29a1b21c2:	push   %rbp
-   29a1b21c3:	push   %rdi
-   29a1b21c4:	push   %rsi
-   29a1b21c5:	push   %rbx
-   29a1b21c6:	sub    $0x20,%rsp
-   29a1b21ca:	mov    0x70(%rsp),%r12
-   29a1b21cf:	mov    %r9d,%ebp
-   29a1b21d2:	mov    %rdx,%rsi
-   29a1b21d5:	mov    %r8,%rbx
-   29a1b21d8:	mov    %rcx,%rdi
+   29a1b21f0:	push   %r12
+   29a1b21f2:	push   %rbp
+   29a1b21f3:	push   %rdi
+   29a1b21f4:	push   %rsi
+   29a1b21f5:	push   %rbx
+   29a1b21f6:	sub    $0x20,%rsp
+   29a1b21fa:	mov    0x70(%rsp),%r12
+   29a1b21ff:	mov    %r9d,%ebp
+   29a1b2202:	mov    %rdx,%rsi
+   29a1b2205:	mov    %r8,%rbx
+   29a1b2208:	mov    %rcx,%rdi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:64
-   29a1b21db:	call   29a1b2478 <_initialize_narrow_environment>
+   29a1b220b:	call   29a1b24b8 <_initialize_narrow_environment>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:65
-   29a1b21e0:	cmp    $0x1,%ebp
-   29a1b21e3:	mov    $0x1,%ecx
-   29a1b21e8:	sbb    $0xffffffff,%ecx
-   29a1b21eb:	call   29a1b2448 <_configure_narrow_argv>
+   29a1b2210:	cmp    $0x1,%ebp
+   29a1b2213:	mov    $0x1,%ecx
+   29a1b2218:	sbb    $0xffffffff,%ecx
+   29a1b221b:	call   29a1b2488 <_configure_narrow_argv>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:66
-   29a1b21f0:	call   29a1b2430 <__p___argc>
-   29a1b21f5:	mov    (%rax),%eax
-   29a1b21f7:	mov    %eax,(%rdi)
+   29a1b2220:	call   29a1b2470 <__p___argc>
+   29a1b2225:	mov    (%rax),%eax
+   29a1b2227:	mov    %eax,(%rdi)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:67
-   29a1b21f9:	call   29a1b2438 <__p___argv>
-   29a1b21fe:	mov    (%rax),%rax
-   29a1b2201:	mov    %rax,(%rsi)
+   29a1b2229:	call   29a1b2478 <__p___argv>
+   29a1b222e:	mov    (%rax),%rax
+   29a1b2231:	mov    %rax,(%rsi)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:68
-   29a1b2204:	call   29a1b24d0 <__p__environ>
-   29a1b2209:	mov    (%rax),%rax
-   29a1b220c:	mov    %rax,(%rbx)
+   29a1b2234:	call   29a1b2510 <__p__environ>
+   29a1b2239:	mov    (%rax),%rax
+   29a1b223c:	mov    %rax,(%rbx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:69
-   29a1b220f:	test   %r12,%r12
-   29a1b2212:	je     29a1b221d <__getmainargs+0x5d>
+   29a1b223f:	test   %r12,%r12
+   29a1b2242:	je     29a1b224d <__getmainargs+0x5d>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:70
-   29a1b2214:	mov    (%r12),%ecx
-   29a1b2218:	call   29a1b24b0 <_set_new_mode>
+   29a1b2244:	mov    (%r12),%ecx
+   29a1b2248:	call   29a1b24f0 <_set_new_mode>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:72
-   29a1b221d:	xor    %eax,%eax
-   29a1b221f:	add    $0x20,%rsp
-   29a1b2223:	pop    %rbx
-   29a1b2224:	pop    %rsi
-   29a1b2225:	pop    %rdi
-   29a1b2226:	pop    %rbp
-   29a1b2227:	pop    %r12
-   29a1b2229:	ret
-   29a1b222a:	nopw   0x0(%rax,%rax,1)
+   29a1b224d:	xor    %eax,%eax
+   29a1b224f:	add    $0x20,%rsp
+   29a1b2253:	pop    %rbx
+   29a1b2254:	pop    %rsi
+   29a1b2255:	pop    %rdi
+   29a1b2256:	pop    %rbp
+   29a1b2257:	pop    %r12
+   29a1b2259:	ret
+   29a1b225a:	nopw   0x0(%rax,%rax,1)
 
-000000029a1b2230 <__wgetmainargs>:
+000000029a1b2260 <__wgetmainargs>:
 __wgetmainargs():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:75
-   29a1b2230:	push   %r12
-   29a1b2232:	push   %rbp
-   29a1b2233:	push   %rdi
-   29a1b2234:	push   %rsi
-   29a1b2235:	push   %rbx
-   29a1b2236:	sub    $0x20,%rsp
-   29a1b223a:	mov    0x70(%rsp),%r12
-   29a1b223f:	mov    %r9d,%ebp
-   29a1b2242:	mov    %rdx,%rsi
-   29a1b2245:	mov    %r8,%rbx
-   29a1b2248:	mov    %rcx,%rdi
+   29a1b2260:	push   %r12
+   29a1b2262:	push   %rbp
+   29a1b2263:	push   %rdi
+   29a1b2264:	push   %rsi
+   29a1b2265:	push   %rbx
+   29a1b2266:	sub    $0x20,%rsp
+   29a1b226a:	mov    0x70(%rsp),%r12
+   29a1b226f:	mov    %r9d,%ebp
+   29a1b2272:	mov    %rdx,%rsi
+   29a1b2275:	mov    %r8,%rbx
+   29a1b2278:	mov    %rcx,%rdi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:76
-   29a1b224b:	call   29a1b2488 <_initialize_wide_environment>
+   29a1b227b:	call   29a1b24c8 <_initialize_wide_environment>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:77
-   29a1b2250:	cmp    $0x1,%ebp
-   29a1b2253:	mov    $0x1,%ecx
-   29a1b2258:	sbb    $0xffffffff,%ecx
-   29a1b225b:	call   29a1b2450 <_configure_wide_argv>
+   29a1b2280:	cmp    $0x1,%ebp
+   29a1b2283:	mov    $0x1,%ecx
+   29a1b2288:	sbb    $0xffffffff,%ecx
+   29a1b228b:	call   29a1b2490 <_configure_wide_argv>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:78
-   29a1b2260:	call   29a1b2430 <__p___argc>
-   29a1b2265:	mov    (%rax),%eax
-   29a1b2267:	mov    %eax,(%rdi)
+   29a1b2290:	call   29a1b2470 <__p___argc>
+   29a1b2295:	mov    (%rax),%eax
+   29a1b2297:	mov    %eax,(%rdi)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:79
-   29a1b2269:	call   29a1b2440 <__p___wargv>
-   29a1b226e:	mov    (%rax),%rax
-   29a1b2271:	mov    %rax,(%rsi)
+   29a1b2299:	call   29a1b2480 <__p___wargv>
+   29a1b229e:	mov    (%rax),%rax
+   29a1b22a1:	mov    %rax,(%rsi)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:80
-   29a1b2274:	call   29a1b24d8 <__p__wenviron>
-   29a1b2279:	mov    (%rax),%rax
-   29a1b227c:	mov    %rax,(%rbx)
+   29a1b22a4:	call   29a1b2518 <__p__wenviron>
+   29a1b22a9:	mov    (%rax),%rax
+   29a1b22ac:	mov    %rax,(%rbx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:81
-   29a1b227f:	test   %r12,%r12
-   29a1b2282:	je     29a1b228d <__wgetmainargs+0x5d>
+   29a1b22af:	test   %r12,%r12
+   29a1b22b2:	je     29a1b22bd <__wgetmainargs+0x5d>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:82
-   29a1b2284:	mov    (%r12),%ecx
-   29a1b2288:	call   29a1b24b0 <_set_new_mode>
+   29a1b22b4:	mov    (%r12),%ecx
+   29a1b22b8:	call   29a1b24f0 <_set_new_mode>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:84
-   29a1b228d:	xor    %eax,%eax
-   29a1b228f:	add    $0x20,%rsp
-   29a1b2293:	pop    %rbx
-   29a1b2294:	pop    %rsi
-   29a1b2295:	pop    %rdi
-   29a1b2296:	pop    %rbp
-   29a1b2297:	pop    %r12
-   29a1b2299:	ret
-   29a1b229a:	nopw   0x0(%rax,%rax,1)
+   29a1b22bd:	xor    %eax,%eax
+   29a1b22bf:	add    $0x20,%rsp
+   29a1b22c3:	pop    %rbx
+   29a1b22c4:	pop    %rsi
+   29a1b22c5:	pop    %rdi
+   29a1b22c6:	pop    %rbp
+   29a1b22c7:	pop    %r12
+   29a1b22c9:	ret
+   29a1b22ca:	nopw   0x0(%rax,%rax,1)
 
-000000029a1b22a0 <_onexit>:
+000000029a1b22d0 <_onexit>:
 _onexit():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:87
-   29a1b22a0:	push   %rbx
-   29a1b22a1:	sub    $0x20,%rsp
-   29a1b22a5:	mov    %rcx,%rbx
+   29a1b22d0:	push   %rbx
+   29a1b22d1:	sub    $0x20,%rsp
+   29a1b22d5:	mov    %rcx,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:88
-   29a1b22a8:	call   29a1b2460 <_crt_atexit>
-   29a1b22ad:	test   %eax,%eax
-   29a1b22af:	mov    $0x0,%eax
-   29a1b22b4:	cmove  %rbx,%rax
+   29a1b22d8:	call   29a1b24a0 <_crt_atexit>
+   29a1b22dd:	test   %eax,%eax
+   29a1b22df:	mov    $0x0,%eax
+   29a1b22e4:	cmove  %rbx,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:89
-   29a1b22b8:	add    $0x20,%rsp
-   29a1b22bc:	pop    %rbx
-   29a1b22bd:	ret
-   29a1b22be:	xchg   %ax,%ax
+   29a1b22e8:	add    $0x20,%rsp
+   29a1b22ec:	pop    %rbx
+   29a1b22ed:	ret
+   29a1b22ee:	xchg   %ax,%ax
 
-000000029a1b22c0 <at_quick_exit>:
+000000029a1b22f0 <at_quick_exit>:
 at_quick_exit():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:98
-   29a1b22c0:	mov    0x1f99(%rip),%rax        # 29a1b4260 <.refptr.__mingw_module_is_dll>
-   29a1b22c7:	cmpb   $0x0,(%rax)
-   29a1b22ca:	je     29a1b22d0 <at_quick_exit+0x10>
+   29a1b22f0:	mov    0x1f69(%rip),%rax        # 29a1b4260 <.refptr.__mingw_module_is_dll>
+   29a1b22f7:	cmpb   $0x0,(%rax)
+   29a1b22fa:	je     29a1b2300 <at_quick_exit+0x10>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:101
-   29a1b22cc:	xor    %eax,%eax
-   29a1b22ce:	ret
-   29a1b22cf:	nop
+   29a1b22fc:	xor    %eax,%eax
+   29a1b22fe:	ret
+   29a1b22ff:	nop
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:100
-   29a1b22d0:	jmp    29a1b2458 <_crt_at_quick_exit>
-   29a1b22d5:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b2300:	jmp    29a1b2498 <_crt_at_quick_exit>
+   29a1b2305:	data16 cs nopw 0x0(%rax,%rax,1)
 
-000000029a1b22e0 <_amsg_exit>:
+000000029a1b2310 <_amsg_exit>:
 _amsg_exit():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:105
-   29a1b22e0:	push   %rbx
-   29a1b22e1:	sub    $0x20,%rsp
-   29a1b22e5:	mov    %ecx,%ebx
+   29a1b2310:	push   %rbx
+   29a1b2311:	sub    $0x20,%rsp
+   29a1b2315:	mov    %ecx,%ebx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:106
-   29a1b22e7:	mov    $0x2,%ecx
-   29a1b22ec:	call   29a1b2400 <__acrt_iob_func>
-   29a1b22f1:	mov    %ebx,%r8d
-   29a1b22f4:	lea    0x1ec5(%rip),%rdx        # 29a1b41c0 <.rdata>
-   29a1b22fb:	mov    %rax,%rcx
-   29a1b22fe:	call   29a1b24f0 <fprintf>
+   29a1b2317:	mov    $0x2,%ecx
+   29a1b231c:	call   29a1b2430 <__acrt_iob_func>
+   29a1b2321:	mov    %ebx,%r8d
+   29a1b2324:	lea    0x1e95(%rip),%rdx        # 29a1b41c0 <.rdata>
+   29a1b232b:	mov    %rax,%rcx
+   29a1b232e:	call   29a1b2530 <fprintf>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:107
-   29a1b2303:	mov    $0xff,%ecx
-   29a1b2308:	call   29a1b2470 <_exit>
-   29a1b230d:	nop
-   29a1b230e:	xchg   %ax,%ax
+   29a1b2333:	mov    $0xff,%ecx
+   29a1b2338:	call   29a1b24b0 <_exit>
+   29a1b233d:	nop
+   29a1b233e:	xchg   %ax,%ax
 
-000000029a1b2310 <__ms_fwprintf>:
+000000029a1b2340 <__ms_fwprintf>:
 __ms_fwprintf():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:151
-   29a1b2310:	sub    $0x48,%rsp
+   29a1b2340:	sub    $0x48,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:154
-   29a1b2314:	lea    0x60(%rsp),%rax
+   29a1b2344:	lea    0x60(%rsp),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:151
-   29a1b2319:	mov    %r8,0x60(%rsp)
+   29a1b2349:	mov    %r8,0x60(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:155
-   29a1b231e:	mov    %rdx,%r8
-   29a1b2321:	mov    %rcx,%rdx
-   29a1b2324:	mov    %rax,0x20(%rsp)
-   29a1b2329:	mov    $0x4,%ecx
+   29a1b234e:	mov    %rdx,%r8
+   29a1b2351:	mov    %rcx,%rdx
+   29a1b2354:	mov    %rax,0x20(%rsp)
+   29a1b2359:	mov    $0x4,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:151
-   29a1b232e:	mov    %r9,0x68(%rsp)
+   29a1b235e:	mov    %r9,0x68(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:155
-   29a1b2333:	xor    %r9d,%r9d
+   29a1b2363:	xor    %r9d,%r9d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:154
-   29a1b2336:	mov    %rax,0x38(%rsp)
+   29a1b2366:	mov    %rax,0x38(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:155
-   29a1b233b:	call   29a1b2410 <__stdio_common_vfwprintf>
+   29a1b236b:	call   29a1b2440 <__stdio_common_vfwprintf>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:158
-   29a1b2340:	add    $0x48,%rsp
-   29a1b2344:	ret
-   29a1b2345:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b2370:	add    $0x48,%rsp
+   29a1b2374:	ret
+   29a1b2375:	data16 cs nopw 0x0(%rax,%rax,1)
 
-000000029a1b2350 <tzset>:
+000000029a1b2380 <tzset>:
 tzset():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:144
-   29a1b2350:	sub    $0x28,%rsp
+   29a1b2380:	sub    $0x28,%rsp
 _tzset():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:135
-   29a1b2354:	mov    0x1ee5(%rip),%rax        # 29a1b4240 <.refptr.__imp__tzset>
-   29a1b235b:	call   *(%rax)
+   29a1b2384:	mov    0x1eb5(%rip),%rax        # 29a1b4240 <.refptr.__imp__tzset>
+   29a1b238b:	call   *(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:138
-   29a1b235d:	call   29a1b23e0 <__tzname>
-   29a1b2362:	mov    %rax,0xd27(%rip)        # 29a1b3090 <__imp_tzname>
+   29a1b238d:	call   29a1b2410 <__tzname>
+   29a1b2392:	mov    %rax,0xcf7(%rip)        # 29a1b3090 <__imp_tzname>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:139
-   29a1b2369:	call   29a1b23d8 <__timezone>
-   29a1b236e:	mov    %rax,0xd13(%rip)        # 29a1b3088 <__imp_timezone>
+   29a1b2399:	call   29a1b2408 <__timezone>
+   29a1b239e:	mov    %rax,0xce3(%rip)        # 29a1b3088 <__imp_timezone>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:140
-   29a1b2375:	call   29a1b23d0 <__daylight>
-   29a1b237a:	mov    %rax,0xcff(%rip)        # 29a1b3080 <__imp_daylight>
+   29a1b23a5:	call   29a1b2400 <__daylight>
+   29a1b23aa:	mov    %rax,0xccf(%rip)        # 29a1b3080 <__imp_daylight>
 tzset():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:146
-   29a1b2381:	add    $0x28,%rsp
-   29a1b2385:	ret
-   29a1b2386:	cs nopw 0x0(%rax,%rax,1)
+   29a1b23b1:	add    $0x28,%rsp
+   29a1b23b5:	ret
+   29a1b23b6:	cs nopw 0x0(%rax,%rax,1)
 
-000000029a1b2390 <_tzset>:
+000000029a1b23c0 <_tzset>:
 _tzset():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:134
-   29a1b2390:	sub    $0x28,%rsp
+   29a1b23c0:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:135
-   29a1b2394:	mov    0x1ea5(%rip),%rax        # 29a1b4240 <.refptr.__imp__tzset>
-   29a1b239b:	call   *(%rax)
+   29a1b23c4:	mov    0x1e75(%rip),%rax        # 29a1b4240 <.refptr.__imp__tzset>
+   29a1b23cb:	call   *(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:138
-   29a1b239d:	call   29a1b23e0 <__tzname>
-   29a1b23a2:	mov    %rax,0xce7(%rip)        # 29a1b3090 <__imp_tzname>
+   29a1b23cd:	call   29a1b2410 <__tzname>
+   29a1b23d2:	mov    %rax,0xcb7(%rip)        # 29a1b3090 <__imp_tzname>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:139
-   29a1b23a9:	call   29a1b23d8 <__timezone>
-   29a1b23ae:	mov    %rax,0xcd3(%rip)        # 29a1b3088 <__imp_timezone>
+   29a1b23d9:	call   29a1b2408 <__timezone>
+   29a1b23de:	mov    %rax,0xca3(%rip)        # 29a1b3088 <__imp_timezone>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:140
-   29a1b23b5:	call   29a1b23d0 <__daylight>
-   29a1b23ba:	mov    %rax,0xcbf(%rip)        # 29a1b3080 <__imp_daylight>
+   29a1b23e5:	call   29a1b2400 <__daylight>
+   29a1b23ea:	mov    %rax,0xc8f(%rip)        # 29a1b3080 <__imp_daylight>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:141
-   29a1b23c1:	add    $0x28,%rsp
-   29a1b23c5:	ret
-   29a1b23c6:	nop
-   29a1b23c7:	nop
-   29a1b23c8:	nop
-   29a1b23c9:	nop
-   29a1b23ca:	nop
-   29a1b23cb:	nop
-   29a1b23cc:	nop
-   29a1b23cd:	nop
-   29a1b23ce:	nop
-   29a1b23cf:	nop
-
-000000029a1b23d0 <__daylight>:
-   29a1b23d0:	jmp    *0x6fda(%rip)        # 29a1b93b0 <__imp___daylight>
-   29a1b23d6:	nop
-   29a1b23d7:	nop
-
-000000029a1b23d8 <__timezone>:
-   29a1b23d8:	jmp    *0x6fda(%rip)        # 29a1b93b8 <__imp___timezone>
-   29a1b23de:	nop
-   29a1b23df:	nop
-
-000000029a1b23e0 <__tzname>:
-   29a1b23e0:	jmp    *0x6fda(%rip)        # 29a1b93c0 <__imp___tzname>
-   29a1b23e6:	nop
-   29a1b23e7:	nop
-
-000000029a1b23e8 <.text>:
-   29a1b23e8:	nopl   0x0(%rax,%rax,1)
-
-000000029a1b23f0 <strlen>:
-   29a1b23f0:	jmp    *0x6fa2(%rip)        # 29a1b9398 <__imp_strlen>
+   29a1b23f1:	add    $0x28,%rsp
+   29a1b23f5:	ret
    29a1b23f6:	nop
    29a1b23f7:	nop
-
-000000029a1b23f8 <strncmp>:
-   29a1b23f8:	jmp    *0x6fa2(%rip)        # 29a1b93a0 <__imp_strncmp>
+   29a1b23f8:	nop
+   29a1b23f9:	nop
+   29a1b23fa:	nop
+   29a1b23fb:	nop
+   29a1b23fc:	nop
+   29a1b23fd:	nop
    29a1b23fe:	nop
    29a1b23ff:	nop
 
-000000029a1b2400 <__acrt_iob_func>:
-   29a1b2400:	jmp    *0x6f5a(%rip)        # 29a1b9360 <__imp___acrt_iob_func>
+000000029a1b2400 <__daylight>:
+   29a1b2400:	jmp    *0x6fba(%rip)        # 29a1b93c0 <__imp___daylight>
    29a1b2406:	nop
    29a1b2407:	nop
 
-000000029a1b2408 <__stdio_common_vfprintf>:
-   29a1b2408:	jmp    *0x6f5a(%rip)        # 29a1b9368 <__imp___stdio_common_vfprintf>
+000000029a1b2408 <__timezone>:
+   29a1b2408:	jmp    *0x6fba(%rip)        # 29a1b93c8 <__imp___timezone>
    29a1b240e:	nop
    29a1b240f:	nop
 
-000000029a1b2410 <__stdio_common_vfwprintf>:
-   29a1b2410:	jmp    *0x6f5a(%rip)        # 29a1b9370 <__imp___stdio_common_vfwprintf>
+000000029a1b2410 <__tzname>:
+   29a1b2410:	jmp    *0x6fba(%rip)        # 29a1b93d0 <__imp___tzname>
    29a1b2416:	nop
    29a1b2417:	nop
 
-000000029a1b2418 <kbhit>:
-   29a1b2418:	jmp    *0x6f5a(%rip)        # 29a1b9378 <__imp_kbhit>
-   29a1b241e:	nop
-   29a1b241f:	nop
+000000029a1b2418 <.text>:
+   29a1b2418:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b2420 <fwrite>:
-   29a1b2420:	jmp    *0x6f5a(%rip)        # 29a1b9380 <__imp_fwrite>
+000000029a1b2420 <strlen>:
+   29a1b2420:	jmp    *0x6f82(%rip)        # 29a1b93a8 <__imp_strlen>
    29a1b2426:	nop
    29a1b2427:	nop
 
-000000029a1b2428 <putchar>:
-   29a1b2428:	jmp    *0x6f5a(%rip)        # 29a1b9388 <__imp_putchar>
+000000029a1b2428 <strncmp>:
+   29a1b2428:	jmp    *0x6f82(%rip)        # 29a1b93b0 <__imp_strncmp>
    29a1b242e:	nop
    29a1b242f:	nop
 
-000000029a1b2430 <__p___argc>:
-   29a1b2430:	jmp    *0x6eaa(%rip)        # 29a1b92e0 <__imp___p___argc>
+000000029a1b2430 <__acrt_iob_func>:
+   29a1b2430:	jmp    *0x6f32(%rip)        # 29a1b9368 <__imp___acrt_iob_func>
    29a1b2436:	nop
    29a1b2437:	nop
 
-000000029a1b2438 <__p___argv>:
-   29a1b2438:	jmp    *0x6eaa(%rip)        # 29a1b92e8 <__imp___p___argv>
+000000029a1b2438 <__stdio_common_vfprintf>:
+   29a1b2438:	jmp    *0x6f32(%rip)        # 29a1b9370 <__imp___stdio_common_vfprintf>
    29a1b243e:	nop
    29a1b243f:	nop
 
-000000029a1b2440 <__p___wargv>:
-   29a1b2440:	jmp    *0x6eaa(%rip)        # 29a1b92f0 <__imp___p___wargv>
+000000029a1b2440 <__stdio_common_vfwprintf>:
+   29a1b2440:	jmp    *0x6f32(%rip)        # 29a1b9378 <__imp___stdio_common_vfwprintf>
    29a1b2446:	nop
    29a1b2447:	nop
 
-000000029a1b2448 <_configure_narrow_argv>:
-   29a1b2448:	jmp    *0x6eaa(%rip)        # 29a1b92f8 <__imp__configure_narrow_argv>
+000000029a1b2448 <kbhit>:
+   29a1b2448:	jmp    *0x6f32(%rip)        # 29a1b9380 <__imp_kbhit>
    29a1b244e:	nop
    29a1b244f:	nop
 
-000000029a1b2450 <_configure_wide_argv>:
-   29a1b2450:	jmp    *0x6eaa(%rip)        # 29a1b9300 <__imp__configure_wide_argv>
+000000029a1b2450 <fflush>:
+   29a1b2450:	jmp    *0x6f32(%rip)        # 29a1b9388 <__imp_fflush>
    29a1b2456:	nop
    29a1b2457:	nop
 
-000000029a1b2458 <_crt_at_quick_exit>:
-   29a1b2458:	jmp    *0x6eaa(%rip)        # 29a1b9308 <__imp__crt_at_quick_exit>
+000000029a1b2458 <fwrite>:
+   29a1b2458:	jmp    *0x6f32(%rip)        # 29a1b9390 <__imp_fwrite>
    29a1b245e:	nop
    29a1b245f:	nop
 
-000000029a1b2460 <_crt_atexit>:
-   29a1b2460:	jmp    *0x6eaa(%rip)        # 29a1b9310 <__imp__crt_atexit>
+000000029a1b2460 <putchar>:
+   29a1b2460:	jmp    *0x6f32(%rip)        # 29a1b9398 <__imp_putchar>
    29a1b2466:	nop
    29a1b2467:	nop
+   29a1b2468:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b2468 <_execute_onexit_table>:
-   29a1b2468:	jmp    *0x6eaa(%rip)        # 29a1b9318 <__imp__execute_onexit_table>
-   29a1b246e:	nop
-   29a1b246f:	nop
-
-000000029a1b2470 <_exit>:
-   29a1b2470:	jmp    *0x6eaa(%rip)        # 29a1b9320 <__imp__exit>
+000000029a1b2470 <__p___argc>:
+   29a1b2470:	jmp    *0x6e72(%rip)        # 29a1b92e8 <__imp___p___argc>
    29a1b2476:	nop
    29a1b2477:	nop
 
-000000029a1b2478 <_initialize_narrow_environment>:
-   29a1b2478:	jmp    *0x6eaa(%rip)        # 29a1b9328 <__imp__initialize_narrow_environment>
+000000029a1b2478 <__p___argv>:
+   29a1b2478:	jmp    *0x6e72(%rip)        # 29a1b92f0 <__imp___p___argv>
    29a1b247e:	nop
    29a1b247f:	nop
 
-000000029a1b2480 <_initialize_onexit_table>:
-   29a1b2480:	jmp    *0x6eaa(%rip)        # 29a1b9330 <__imp__initialize_onexit_table>
+000000029a1b2480 <__p___wargv>:
+   29a1b2480:	jmp    *0x6e72(%rip)        # 29a1b92f8 <__imp___p___wargv>
    29a1b2486:	nop
    29a1b2487:	nop
 
-000000029a1b2488 <_initialize_wide_environment>:
-   29a1b2488:	jmp    *0x6eaa(%rip)        # 29a1b9338 <__imp__initialize_wide_environment>
+000000029a1b2488 <_configure_narrow_argv>:
+   29a1b2488:	jmp    *0x6e72(%rip)        # 29a1b9300 <__imp__configure_narrow_argv>
    29a1b248e:	nop
    29a1b248f:	nop
 
-000000029a1b2490 <_initterm>:
-   29a1b2490:	jmp    *0x6eaa(%rip)        # 29a1b9340 <__imp__initterm>
+000000029a1b2490 <_configure_wide_argv>:
+   29a1b2490:	jmp    *0x6e72(%rip)        # 29a1b9308 <__imp__configure_wide_argv>
    29a1b2496:	nop
    29a1b2497:	nop
 
-000000029a1b2498 <_register_onexit_function>:
-   29a1b2498:	jmp    *0x6eaa(%rip)        # 29a1b9348 <__imp__register_onexit_function>
+000000029a1b2498 <_crt_at_quick_exit>:
+   29a1b2498:	jmp    *0x6e72(%rip)        # 29a1b9310 <__imp__crt_at_quick_exit>
    29a1b249e:	nop
    29a1b249f:	nop
 
-000000029a1b24a0 <abort>:
-   29a1b24a0:	jmp    *0x6eaa(%rip)        # 29a1b9350 <__imp_abort>
+000000029a1b24a0 <_crt_atexit>:
+   29a1b24a0:	jmp    *0x6e72(%rip)        # 29a1b9318 <__imp__crt_atexit>
    29a1b24a6:	nop
    29a1b24a7:	nop
-   29a1b24a8:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b24b0 <_set_new_mode>:
-   29a1b24b0:	jmp    *0x6e0a(%rip)        # 29a1b92c0 <__imp__set_new_mode>
+000000029a1b24a8 <_execute_onexit_table>:
+   29a1b24a8:	jmp    *0x6e72(%rip)        # 29a1b9320 <__imp__execute_onexit_table>
+   29a1b24ae:	nop
+   29a1b24af:	nop
+
+000000029a1b24b0 <_exit>:
+   29a1b24b0:	jmp    *0x6e72(%rip)        # 29a1b9328 <__imp__exit>
    29a1b24b6:	nop
    29a1b24b7:	nop
 
-000000029a1b24b8 <calloc>:
-   29a1b24b8:	jmp    *0x6e0a(%rip)        # 29a1b92c8 <__imp_calloc>
+000000029a1b24b8 <_initialize_narrow_environment>:
+   29a1b24b8:	jmp    *0x6e72(%rip)        # 29a1b9330 <__imp__initialize_narrow_environment>
    29a1b24be:	nop
    29a1b24bf:	nop
 
-000000029a1b24c0 <free>:
-   29a1b24c0:	jmp    *0x6e0a(%rip)        # 29a1b92d0 <__imp_free>
+000000029a1b24c0 <_initialize_onexit_table>:
+   29a1b24c0:	jmp    *0x6e72(%rip)        # 29a1b9338 <__imp__initialize_onexit_table>
    29a1b24c6:	nop
    29a1b24c7:	nop
-   29a1b24c8:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b24d0 <__p__environ>:
-   29a1b24d0:	jmp    *0x6dd2(%rip)        # 29a1b92a8 <__imp___p__environ>
+000000029a1b24c8 <_initialize_wide_environment>:
+   29a1b24c8:	jmp    *0x6e72(%rip)        # 29a1b9340 <__imp__initialize_wide_environment>
+   29a1b24ce:	nop
+   29a1b24cf:	nop
+
+000000029a1b24d0 <_initterm>:
+   29a1b24d0:	jmp    *0x6e72(%rip)        # 29a1b9348 <__imp__initterm>
    29a1b24d6:	nop
    29a1b24d7:	nop
 
-000000029a1b24d8 <__p__wenviron>:
-   29a1b24d8:	jmp    *0x6dd2(%rip)        # 29a1b92b0 <__imp___p__wenviron>
+000000029a1b24d8 <_register_onexit_function>:
+   29a1b24d8:	jmp    *0x6e72(%rip)        # 29a1b9350 <__imp__register_onexit_function>
    29a1b24de:	nop
    29a1b24df:	nop
 
-000000029a1b24e0 <getch>:
-   29a1b24e0:	jmp    *0x6db2(%rip)        # 29a1b9298 <__imp_getch>
+000000029a1b24e0 <abort>:
+   29a1b24e0:	jmp    *0x6e72(%rip)        # 29a1b9358 <__imp_abort>
    29a1b24e6:	nop
    29a1b24e7:	nop
    29a1b24e8:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b24f0 <fprintf>:
+000000029a1b24f0 <_set_new_mode>:
+   29a1b24f0:	jmp    *0x6dd2(%rip)        # 29a1b92c8 <__imp__set_new_mode>
+   29a1b24f6:	nop
+   29a1b24f7:	nop
+
+000000029a1b24f8 <calloc>:
+   29a1b24f8:	jmp    *0x6dd2(%rip)        # 29a1b92d0 <__imp_calloc>
+   29a1b24fe:	nop
+   29a1b24ff:	nop
+
+000000029a1b2500 <free>:
+   29a1b2500:	jmp    *0x6dd2(%rip)        # 29a1b92d8 <__imp_free>
+   29a1b2506:	nop
+   29a1b2507:	nop
+   29a1b2508:	nopl   0x0(%rax,%rax,1)
+
+000000029a1b2510 <__p__environ>:
+   29a1b2510:	jmp    *0x6d9a(%rip)        # 29a1b92b0 <__imp___p__environ>
+   29a1b2516:	nop
+   29a1b2517:	nop
+
+000000029a1b2518 <__p__wenviron>:
+   29a1b2518:	jmp    *0x6d9a(%rip)        # 29a1b92b8 <__imp___p__wenviron>
+   29a1b251e:	nop
+   29a1b251f:	nop
+
+000000029a1b2520 <getch>:
+   29a1b2520:	jmp    *0x6d7a(%rip)        # 29a1b92a0 <__imp_getch>
+   29a1b2526:	nop
+   29a1b2527:	nop
+   29a1b2528:	nopl   0x0(%rax,%rax,1)
+
+000000029a1b2530 <fprintf>:
 fprintf():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:12
-   29a1b24f0:	sub    $0x48,%rsp
+   29a1b2530:	sub    $0x48,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:15
-   29a1b24f4:	lea    0x60(%rsp),%rax
+   29a1b2534:	lea    0x60(%rsp),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:12
-   29a1b24f9:	mov    %r8,0x60(%rsp)
+   29a1b2539:	mov    %r8,0x60(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:16
-   29a1b24fe:	mov    %rdx,%r8
-   29a1b2501:	mov    %rcx,%rdx
-   29a1b2504:	mov    %rax,0x20(%rsp)
-   29a1b2509:	xor    %ecx,%ecx
+   29a1b253e:	mov    %rdx,%r8
+   29a1b2541:	mov    %rcx,%rdx
+   29a1b2544:	mov    %rax,0x20(%rsp)
+   29a1b2549:	xor    %ecx,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:12
-   29a1b250b:	mov    %r9,0x68(%rsp)
+   29a1b254b:	mov    %r9,0x68(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:16
-   29a1b2510:	xor    %r9d,%r9d
+   29a1b2550:	xor    %r9d,%r9d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:15
-   29a1b2513:	mov    %rax,0x38(%rsp)
+   29a1b2553:	mov    %rax,0x38(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:16
-   29a1b2518:	call   29a1b2408 <__stdio_common_vfprintf>
+   29a1b2558:	call   29a1b2438 <__stdio_common_vfprintf>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:19
-   29a1b251d:	add    $0x48,%rsp
-   29a1b2521:	ret
-   29a1b2522:	nop
-   29a1b2523:	nop
-   29a1b2524:	nop
-   29a1b2525:	nop
-   29a1b2526:	nop
-   29a1b2527:	nop
-   29a1b2528:	nop
-   29a1b2529:	nop
-   29a1b252a:	nop
-   29a1b252b:	nop
-   29a1b252c:	nop
-   29a1b252d:	nop
-   29a1b252e:	nop
-   29a1b252f:	nop
-
-000000029a1b2530 <VirtualQuery>:
-   29a1b2530:	jmp    *0x6d52(%rip)        # 29a1b9288 <__imp_VirtualQuery>
-   29a1b2536:	nop
-   29a1b2537:	nop
-
-000000029a1b2538 <VirtualProtect>:
-   29a1b2538:	jmp    *0x6d42(%rip)        # 29a1b9280 <__imp_VirtualProtect>
-   29a1b253e:	nop
-   29a1b253f:	nop
-
-000000029a1b2540 <TlsGetValue>:
-   29a1b2540:	jmp    *0x6d32(%rip)        # 29a1b9278 <__imp_TlsGetValue>
-   29a1b2546:	nop
-   29a1b2547:	nop
-
-000000029a1b2548 <Sleep>:
-   29a1b2548:	jmp    *0x6d22(%rip)        # 29a1b9270 <__imp_Sleep>
-   29a1b254e:	nop
-   29a1b254f:	nop
-
-000000029a1b2550 <LeaveCriticalSection>:
-   29a1b2550:	jmp    *0x6d12(%rip)        # 29a1b9268 <__imp_LeaveCriticalSection>
-   29a1b2556:	nop
-   29a1b2557:	nop
-
-000000029a1b2558 <InitializeCriticalSection>:
-   29a1b2558:	jmp    *0x6d02(%rip)        # 29a1b9260 <__imp_InitializeCriticalSection>
-   29a1b255e:	nop
-   29a1b255f:	nop
-
-000000029a1b2560 <GetLastError>:
-   29a1b2560:	jmp    *0x6cf2(%rip)        # 29a1b9258 <__imp_GetLastError>
+   29a1b255d:	add    $0x48,%rsp
+   29a1b2561:	ret
+   29a1b2562:	nop
+   29a1b2563:	nop
+   29a1b2564:	nop
+   29a1b2565:	nop
    29a1b2566:	nop
    29a1b2567:	nop
-
-000000029a1b2568 <EnterCriticalSection>:
-   29a1b2568:	jmp    *0x6ce2(%rip)        # 29a1b9250 <__imp_EnterCriticalSection>
+   29a1b2568:	nop
+   29a1b2569:	nop
+   29a1b256a:	nop
+   29a1b256b:	nop
+   29a1b256c:	nop
+   29a1b256d:	nop
    29a1b256e:	nop
    29a1b256f:	nop
 
-000000029a1b2570 <DeleteCriticalSection>:
-   29a1b2570:	jmp    *0x6cd2(%rip)        # 29a1b9248 <__IAT_start__>
+000000029a1b2570 <VirtualQuery>:
+   29a1b2570:	jmp    *0x6d1a(%rip)        # 29a1b9290 <__imp_VirtualQuery>
    29a1b2576:	nop
    29a1b2577:	nop
-   29a1b2578:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b2580 <register_frame_ctor>:
-   29a1b2580:	jmp    29a1b1360 <__gcc_register_frame>
-   29a1b2585:	nop
+000000029a1b2578 <VirtualProtect>:
+   29a1b2578:	jmp    *0x6d0a(%rip)        # 29a1b9288 <__imp_VirtualProtect>
+   29a1b257e:	nop
+   29a1b257f:	nop
+
+000000029a1b2580 <TlsGetValue>:
+   29a1b2580:	jmp    *0x6cfa(%rip)        # 29a1b9280 <__imp_TlsGetValue>
    29a1b2586:	nop
    29a1b2587:	nop
-   29a1b2588:	nop
-   29a1b2589:	nop
-   29a1b258a:	nop
-   29a1b258b:	nop
-   29a1b258c:	nop
-   29a1b258d:	nop
+
+000000029a1b2588 <Sleep>:
+   29a1b2588:	jmp    *0x6cea(%rip)        # 29a1b9278 <__imp_Sleep>
    29a1b258e:	nop
    29a1b258f:	nop
 
-000000029a1b2590 <__CTOR_LIST__>:
-   29a1b2590:	(bad)
-   29a1b2591:	(bad)
-   29a1b2592:	(bad)
-   29a1b2593:	(bad)
-   29a1b2594:	(bad)
-   29a1b2595:	(bad)
-   29a1b2596:	(bad)
-   29a1b2597:	incl   0x29a1b25(%rax)
-
-000000029a1b2598 <.ctors.65535>:
-   29a1b2598:	andb   $0x0,0x29a1b(%rip)        # 29a1dbfba <.debug_rnglists+0xbf16>
-	...
-
-000000029a1b25a8 <__DTOR_LIST__>:
-   29a1b25a8:	(bad)
-   29a1b25a9:	(bad)
-   29a1b25aa:	(bad)
-   29a1b25ab:	(bad)
-   29a1b25ac:	(bad)
-   29a1b25ad:	(bad)
-   29a1b25ae:	(bad)
-   29a1b25af:	incl   (%rax)
-   29a1b25b1:	add    %al,(%rax)
-   29a1b25b3:	add    %al,(%rax)
-   29a1b25b5:	add    %al,(%rax)
+000000029a1b2590 <LeaveCriticalSection>:
+   29a1b2590:	jmp    *0x6cda(%rip)        # 29a1b9270 <__imp_LeaveCriticalSection>
+   29a1b2596:	nop
+   29a1b2597:	nop
+
+000000029a1b2598 <InitializeCriticalSection>:
+   29a1b2598:	jmp    *0x6cca(%rip)        # 29a1b9268 <__imp_InitializeCriticalSection>
+   29a1b259e:	nop
+   29a1b259f:	nop
+
+000000029a1b25a0 <GetLastError>:
+   29a1b25a0:	jmp    *0x6cba(%rip)        # 29a1b9260 <__imp_GetLastError>
+   29a1b25a6:	nop
+   29a1b25a7:	nop
+
+000000029a1b25a8 <EnterCriticalSection>:
+   29a1b25a8:	jmp    *0x6caa(%rip)        # 29a1b9258 <__imp_EnterCriticalSection>
+   29a1b25ae:	nop
+   29a1b25af:	nop
+
+000000029a1b25b0 <DeleteCriticalSection>:
+   29a1b25b0:	jmp    *0x6c9a(%rip)        # 29a1b9250 <__IAT_start__>
+   29a1b25b6:	nop
+   29a1b25b7:	nop
+   29a1b25b8:	nopl   0x0(%rax,%rax,1)
+
+000000029a1b25c0 <register_frame_ctor>:
+   29a1b25c0:	jmp    29a1b1360 <__gcc_register_frame>
+   29a1b25c5:	nop
+   29a1b25c6:	nop
+   29a1b25c7:	nop
+   29a1b25c8:	nop
+   29a1b25c9:	nop
+   29a1b25ca:	nop
+   29a1b25cb:	nop
+   29a1b25cc:	nop
+   29a1b25cd:	nop
+   29a1b25ce:	nop
+   29a1b25cf:	nop
+
+000000029a1b25d0 <__CTOR_LIST__>:
+   29a1b25d0:	(bad)
+   29a1b25d1:	(bad)
+   29a1b25d2:	(bad)
+   29a1b25d3:	(bad)
+   29a1b25d4:	(bad)
+   29a1b25d5:	(bad)
+   29a1b25d6:	(bad)
+   29a1b25d7:	inc    %eax
+
+000000029a1b25d8 <.ctors.65535>:
+   29a1b25d8:	shlb   $0x0,0x29a1b(%rip)        # 29a1dbffa <.debug_rnglists+0xbf56>
+	...
+
+000000029a1b25e8 <__DTOR_LIST__>:
+   29a1b25e8:	(bad)
+   29a1b25e9:	(bad)
+   29a1b25ea:	(bad)
+   29a1b25eb:	(bad)
+   29a1b25ec:	(bad)
+   29a1b25ed:	(bad)
+   29a1b25ee:	(bad)
+   29a1b25ef:	incl   (%rax)
+   29a1b25f1:	add    %al,(%rax)
+   29a1b25f3:	add    %al,(%rax)
+   29a1b25f5:	add    %al,(%rax)
 	...
 
 Disassembly of section .data:
 
 000000029a1b3000 <__data_start__>:
    29a1b3000:	add    %eax,(%rax)
 	...
 
 000000029a1b3010 <p.0>:
-   29a1b3010:	mov    $0x25,%al
-   29a1b3012:	sbb    0x2(%rdx),%ebx
+   29a1b3010:	lock and $0x29a1b,%eax
 	...
 
 000000029a1b3020 <__native_vcclrit_reason>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/natstart.c:12
    29a1b3020:	(bad)
    29a1b3021:	(bad)
    29a1b3022:	(bad)
@@ -4486,51 +4517,54 @@
 000000029a1b3030 <_CRT_MT>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsmcrt.c:12
    29a1b3030:	add    (%rax),%al
 	...
 
 000000029a1b3040 <__imp_vfprintf>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_vfprintf.c:15
-   29a1b3040:	nop
-   29a1b3041:	and    %ebx,(%rbx)
+   29a1b3040:	shlb   $0x1b,(%rcx)
    29a1b3043:	(bad)
    29a1b3044:	add    (%rax),%al
 	...
 
 000000029a1b3050 <__imp___ms_fwprintf>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:166
-   29a1b3050:	adc    %ah,(%rbx)
-   29a1b3052:	sbb    0x2(%rdx),%ebx
+   29a1b3050:	rex and (%rbx),%ebx
+   29a1b3053:	(bad)
+   29a1b3054:	add    (%rax),%al
+	...
 
 000000029a1b3058 <__imp_tzset>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:165
-   29a1b3058:	push   %rax
-   29a1b3059:	and    (%rbx),%ebx
+   29a1b3058:	andb   $0x1b,(%rbx)
    29a1b305b:	(bad)
    29a1b305c:	add    (%rax),%al
 	...
 
 000000029a1b3060 <__imp__get_output_format>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:164
-   29a1b3060:	mov    $0x21,%al
+   29a1b3060:	loopne 29a1b3083 <__imp_daylight+0x3>
    29a1b3062:	sbb    0x2(%rdx),%ebx
 
 000000029a1b3068 <__imp__amsg_exit>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:163
-   29a1b3068:	loopne 29a1b308c <__imp_timezone+0x4>
+   29a1b3068:	adc    %ah,(%rbx)
    29a1b306a:	sbb    0x2(%rdx),%ebx
 
 000000029a1b3070 <__imp___wgetmainargs>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:162
-   29a1b3070:	xor    %ah,(%rdx)
-   29a1b3072:	sbb    0x2(%rdx),%ebx
+   29a1b3070:	(bad)
+   29a1b3071:	and    (%rbx),%bl
+   29a1b3073:	(bad)
+   29a1b3074:	add    (%rax),%al
+	...
 
 000000029a1b3078 <__imp___getmainargs>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:161
-   29a1b3078:	shlb   $0x1b,(%rcx)
+   29a1b3078:	lock and %ebx,(%rbx)
    29a1b307b:	(bad)
    29a1b307c:	add    (%rax),%al
 	...
 
 000000029a1b3080 <__imp_daylight>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:131
    29a1b3080:	cwtl
@@ -4578,41 +4612,35 @@
    29a1b30b4:	push   %rax
    29a1b30b5:	push   %rbx
    29a1b30b6:	push   %rsp
 	...
 
 000000029a1b30b8 <__imp_at_quick_exit>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:103
-   29a1b30b8:	shlb   $0x1b,(%rdx)
+   29a1b30b8:	lock and (%rbx),%bl
    29a1b30bb:	(bad)
    29a1b30bc:	add    (%rax),%al
 	...
 
 000000029a1b30c0 <__imp__onexit>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:91
-   29a1b30c0:	movabs 0x29a1b22,%al
-   29a1b30c9:	add    %al,(%rax)
-   29a1b30cb:	add    %al,(%rax)
-   29a1b30cd:	add    %al,(%rax)
+   29a1b30c0:	shlb   $1,(%rdx)
+   29a1b30c2:	sbb    0x2(%rdx),%ebx
 	...
 
 000000029a1b30d0 <__imp_fprintf>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:20
-   29a1b30d0:	lock and $0x1b,%al
-   29a1b30d3:	(bad)
-   29a1b30d4:	add    (%rax),%al
+   29a1b30d0:	xor    %ah,0x29a1b(%rip)        # 29a1dcaf1 <.debug_rnglists+0xca4d>
 	...
 
 Disassembly of section .rdata:
 
 000000029a1b4000 <__dyn_tls_init_callback>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:104
-   29a1b4000:	rclb   $1,(%rbx,%rbx,1)
-   29a1b4003:	(bad)
-   29a1b4004:	add    (%rax),%al
+   29a1b4000:	add    %dl,0x29a1b(%rip)        # 29a1dda21 <.debug_rnglists+0xd97d>
 	...
 
 000000029a1b4020 <_tls_used>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:48
    29a1b4020:	add    %dh,0x29a1b(%rax)
    29a1b4026:	add    %al,(%rax)
    29a1b4028:	or     %dh,0x29a1b(%rax)
@@ -4761,16 +4789,15 @@
 
 000000029a1b41e0 <.refptr._CRT_MT>:
    29a1b41e0:	xor    %dh,(%rax)
    29a1b41e2:	sbb    0x2(%rdx),%ebx
 	...
 
 000000029a1b41f0 <.refptr.__CTOR_LIST__>:
-   29a1b41f0:	nop
-   29a1b41f1:	and    $0x29a1b,%eax
+   29a1b41f0:	shlb   $1,0x29a1b(%rip)        # 29a1ddc11 <.debug_rnglists+0xdb6d>
 	...
 
 000000029a1b4200 <.refptr.__ImageBase>:
    29a1b4200:	add    %al,(%rax)
    29a1b4202:	sbb    0x2(%rdx),%ebx
 	...
 
@@ -4789,16 +4816,15 @@
 000000029a1b4230 <.refptr.__dyn_tls_init_callback>:
    29a1b4230:	add    %al,0x1b(%rax)
    29a1b4233:	(bad)
    29a1b4234:	add    (%rax),%al
 	...
 
 000000029a1b4240 <.refptr.__imp__tzset>:
-   29a1b4240:	enter  $0x1b93,$0x9a
-   29a1b4244:	add    (%rax),%al
+   29a1b4240:	fcoms  0x29a1b(%rbx)
 	...
 
 000000029a1b4250 <.refptr.__mingw_app_type>:
    29a1b4250:	push   %rax
    29a1b4251:	jo     29a1b426e <.refptr.__mingw_module_is_dll+0xe>
    29a1b4253:	(bad)
    29a1b4254:	add    (%rax),%al
@@ -5410,241 +5436,232 @@
    29a1b504c:	jno    29a1b5061 <.pdata+0xd>
    29a1b504e:	add    %al,(%rax)
    29a1b5050:	xor    $0x60,%al
 	...
 
 000000029a1b5054 <.pdata>:
    29a1b5054:	adcb   $0x0,(%rbx)
-   29a1b5057:	add    %al,0x38000013(%rdi)
+   29a1b5057:	add    %ah,0x38000013(%rbp)
    29a1b505d:	(bad)
    29a1b505e:	add    %al,(%rax)
-   29a1b5060:	xchg   %edx,(%rbx)
-   29a1b5062:	add    %al,(%rax)
-   29a1b5064:	(bad)
-   29a1b5065:	adc    (%rax),%eax
-   29a1b5067:	add    %al,0x60(%rax)
+   29a1b5060:	movsl  %ds:(%rsi),%es:(%rdi)
+   29a1b5061:	adc    (%rax),%eax
+   29a1b5063:	add    %bh,0x44000013(%rax)
+   29a1b5069:	(bad)
    29a1b506a:	add    %al,(%rax)
-   29a1b506c:	(bad)
-   29a1b506d:	adc    (%rax),%eax
-   29a1b506f:	add    %bh,0x4c000013(%rdi)
-   29a1b5075:	(bad)
+   29a1b506c:	mov    $0xec000013,%eax
+   29a1b5071:	adc    (%rax),%eax
+   29a1b5073:	add    %dl,0x60(%rax)
    29a1b5076:	add    %al,(%rax)
-   29a1b5078:	mov    $0xc6000013,%edi
+   29a1b5078:	in     (%dx),%al
+   29a1b5079:	adc    (%rax),%eax
+   29a1b507b:	add    %dh,%bl
    29a1b507d:	adc    (%rax),%eax
-   29a1b507f:	add    %bl,0x60(%rax)
+   29a1b507f:	add    %bl,0x0(%rax,%riz,2)
 	...
 
 000000029a1b5084 <.pdata>:
-   29a1b5084:	rclb   $1,(%rbx)
-   29a1b5086:	add    %al,(%rax)
-   29a1b5088:	or     (%rax,%rax,1),%dl
-   29a1b508b:	add    %ah,0x60(%rax)
-   29a1b508e:	add    %al,(%rax)
-   29a1b5090:	adc    %dl,(%rax,%rax,1)
-   29a1b5093:	add    %bh,0x14(%rdx)
-   29a1b5096:	add    %al,(%rax)
-   29a1b5098:	push   $0xffffffff80000060
-   29a1b509d:	adc    $0x0,%al
-   29a1b509f:	add    %bl,0x74000014(%rdi)
-   29a1b50a5:	(bad)
+   29a1b5084:	add    %dl,(%rax,%rax,1)
+   29a1b5087:	add    %bh,(%rdx)
+   29a1b5089:	adc    $0x0,%al
+   29a1b508b:	add    %ah,0x0(%rax,%riz,2)
+   29a1b508f:	add    %al,0x14(%rax)
+   29a1b5092:	add    %al,(%rax)
+   29a1b5094:	stos   %al,%es:(%rdi)
+   29a1b5095:	adc    $0x0,%al
+   29a1b5097:	add    %ch,0x0(%rax,%riz,2)
+   29a1b509b:	add    %dh,-0x30ffffec(%rax)
+   29a1b50a1:	adc    $0x0,%al
+   29a1b50a3:	add    %bh,0x60(%rax)
 	...
 
 000000029a1b50a8 <.pdata>:
-   29a1b50a8:	movabs 0x78000014cf000014,%al
-   29a1b50b1:	(bad)
-   29a1b50b2:	add    %al,(%rax)
-   29a1b50b4:	rclb   $1,(%rax,%rax,1)
-   29a1b50b7:	add    %dl,0x15(%rcx)
+   29a1b50a8:	rclb   $1,(%rax,%rax,1)
+   29a1b50ab:	add    %bh,%bh
+   29a1b50ad:	adc    $0x0,%al
+   29a1b50af:	add    %bh,0x0(%rax,%riz,2)
+   29a1b50b3:	add    %al,(%rax)
+   29a1b50b5:	adc    $0x15810000,%eax
    29a1b50ba:	add    %al,(%rax)
-   29a1b50bc:	andb   $0x0,0x0(%rax)
-   29a1b50c0:	(bad)
-   29a1b50c1:	adc    $0x15630000,%eax
-   29a1b50c6:	add    %al,(%rax)
-   29a1b50c8:	mov    %fs,0x0(%rax)
+   29a1b50bc:	test   %ah,0x0(%rax)
+   29a1b50bf:	add    %dl,-0x6cffffeb(%rax)
+   29a1b50c5:	adc    $0x60900000,%eax
 	...
 
 000000029a1b50cc <.pdata>:
-   29a1b50cc:	jo     29a1b50e3 <.pdata+0x17>
-   29a1b50ce:	add    %al,(%rax)
-   29a1b50d0:	fsts   0x60900000(%rip)        # 2faab50d6 <.debug_rnglists+0x608e5032>
+   29a1b50cc:	movabs 0x9400001609000015,%al
+   29a1b50d5:	(bad)
    29a1b50d6:	add    %al,(%rax)
-   29a1b50d8:	loopne 29a1b50ef <.pdata+0x23>
+   29a1b50d8:	adc    %dl,(%rsi)
    29a1b50da:	add    %al,(%rax)
-   29a1b50dc:	rex.X (bad)
+   29a1b50dc:	jb     29a1b50f5 <.pdata+0x5>
    29a1b50de:	add    %al,(%rax)
-   29a1b50e0:	pushf
-   29a1b50e1:	(bad)
-   29a1b50e2:	add    %al,(%rax)
-   29a1b50e4:	push   %rax
-   29a1b50e5:	(bad)
-   29a1b50e6:	add    %al,(%rax)
-   29a1b50e8:	lods   %ds:(%rsi),%eax
+   29a1b50e0:	movabs 0xdd00001780000060,%al
    29a1b50e9:	sbb    (%rax),%al
-   29a1b50eb:	add    %ch,-0x4fffffa0(%rax)
+   29a1b50eb:	add    %ch,0x1ae00000(%rax,%riz,2)
 
 000000029a1b50f0 <.pdata>:
-   29a1b50f0:	mov    $0x1a,%al
+   29a1b50f0:	loopne 29a1b510c <.pdata+0x1c>
    29a1b50f2:	add    %al,(%rax)
-   29a1b50f4:	and    %bl,(%rbx)
-   29a1b50f6:	add    %al,(%rax)
-   29a1b50f8:	shlb   $0x0,0x0(%rax)
-   29a1b50fc:	and    %bl,(%rbx)
-   29a1b50fe:	add    %al,(%rax)
-   29a1b5100:	(bad)
-   29a1b5101:	sbb    (%rax),%eax
-   29a1b5103:	add    %dl,%al
+   29a1b50f4:	push   %rax
+   29a1b50f5:	sbb    (%rax),%eax
+   29a1b50f7:	add    %al,%ah
+   29a1b50f9:	(bad)
+   29a1b50fa:	add    %al,(%rax)
+   29a1b50fc:	push   %rax
+   29a1b50fd:	sbb    (%rax),%eax
+   29a1b50ff:	add    %bh,-0x2bffffe5(%rdi)
    29a1b5105:	(bad)
    29a1b5106:	add    %al,(%rax)
-   29a1b5108:	nop
-   29a1b5109:	sbb    (%rax),%eax
-   29a1b510b:	add    %dl,(%rcx)
-   29a1b510d:	sbb    $0x0,%al
-   29a1b510f:	add    %bl,%ah
-   29a1b5111:	(bad)
+   29a1b5108:	rcrb   $0x0,(%rbx)
+   29a1b510b:	add    %al,0x1c(%rcx)
+   29a1b510e:	add    %al,(%rax)
+   29a1b5110:	loopne 29a1b5172 <.pdata+0x52>
    29a1b5112:	add    %al,(%rax)
-   29a1b5114:	and    %bl,(%rax,%rax,1)
-   29a1b5117:	add    %dl,(%rdx)
-   29a1b5119:	sbb    $0x60e80000,%eax
+   29a1b5114:	push   %rax
+   29a1b5115:	sbb    $0x0,%al
+   29a1b5117:	add    %al,0x1d(%rdx)
+   29a1b511a:	add    %al,(%rax)
+   29a1b511c:	in     (%dx),%al
+   29a1b511d:	(bad)
 	...
 
 000000029a1b5120 <.pdata>:
-   29a1b5120:	and    %bl,0x1d4c0000(%rip)        # 2b7675126 <.debug_rnglists+0x1d4a5082>
+   29a1b5120:	push   %rax
+   29a1b5121:	sbb    $0x1d7c0000,%eax
    29a1b5126:	add    %al,(%rax)
-   29a1b5128:	lock (bad)
+   29a1b5128:	hlt
+   29a1b5129:	(bad)
    29a1b512a:	add    %al,(%rax)
-   29a1b512c:	push   %rax
-   29a1b512d:	sbb    $0x1da00000,%eax
-   29a1b5132:	add    %al,(%rax)
-   29a1b5134:	hlt
+   29a1b512c:	sbbb   $0x0,0x1dd00000(%rip)        # 2b7eb5133 <.debug_rnglists+0x1dce508f>
+   29a1b5133:	add    %bh,%al
    29a1b5135:	(bad)
    29a1b5136:	add    %al,(%rax)
-   29a1b5138:	movabs 0xf800001e3d00001d,%al
+   29a1b5138:	rcrb   $1,0x1e6d0000(%rip)        # 2b888513e <.debug_rnglists+0x1e6b509a>
+   29a1b513e:	add    %al,(%rax)
+   29a1b5140:	cld
    29a1b5141:	(bad)
    29a1b5142:	add    %al,(%rax)
-   29a1b5144:	rex (bad)
+   29a1b5144:	jo     29a1b5164 <.pdata+0x44>
    29a1b5146:	add    %al,(%rax)
-   29a1b5148:	rcrb   $0x0,(%rsi)
-   29a1b514b:	add    %al,(%rcx,%riz,2)
-   29a1b514e:	add    %al,(%rax)
-   29a1b5150:	rcrb   $0x0,(%rsi)
-   29a1b5153:	add    %dh,%bh
+   29a1b5148:	lock (bad)
+   29a1b514a:	add    %al,(%rax)
+   29a1b514c:	or     %ah,0x0(%rcx)
+   29a1b514f:	add    %dh,%al
+   29a1b5151:	(bad)
+   29a1b5152:	add    %al,(%rax)
+   29a1b5154:	(bad)
    29a1b5155:	(bad)
    29a1b5156:	add    %al,(%rax)
-   29a1b5158:	or     %ah,0x0(%rcx)
-   29a1b515b:	add    %al,(%rax)
-   29a1b515d:	(bad)
+   29a1b5158:	or     $0x61,%al
+   29a1b515a:	add    %al,(%rax)
+   29a1b515c:	xor    %bl,(%rdi)
    29a1b515e:	add    %al,(%rax)
-   29a1b5160:	jae    29a1b5181 <.pdata+0x61>
-   29a1b5162:	add    %al,(%rax)
-   29a1b5164:	or     $0x61,%al
-   29a1b5166:	add    %al,(%rax)
-   29a1b5168:	sbbb   $0x0,(%rdi)
-   29a1b516b:	add    %dh,0x1000001f(%rsi)
-   29a1b5171:	(bad)
+   29a1b5160:	movabs %eax,0xb00000611000001f
+   29a1b5169:	(bad)
+   29a1b516a:	add    %al,(%rax)
+   29a1b516c:	out    %al,$0x1f
+   29a1b516e:	add    %al,(%rax)
+   29a1b5170:	adc    $0x61,%al
    29a1b5172:	add    %al,(%rax)
-   29a1b5174:	rcrb   $0x0,(%rdi)
-   29a1b5177:	add    %cl,0x20(%rcx)
+   29a1b5174:	lock (bad)
+   29a1b5176:	add    %al,(%rax)
+   29a1b5178:	jns    29a1b519a <.pdata+0x2>
    29a1b517a:	add    %al,(%rax)
-   29a1b517c:	adc    $0x61,%al
-   29a1b517e:	add    %al,(%rax)
-   29a1b5180:	push   %rax
-   29a1b5181:	and    %al,(%rax)
-   29a1b5183:	add    %dl,(%rsi)
+   29a1b517c:	sbb    %ah,0x0(%rcx)
+   29a1b517f:	add    %al,0x46000020(%rax)
    29a1b5185:	and    %eax,(%rax)
-   29a1b5187:	add    %bl,(%rax)
-   29a1b5189:	(bad)
+   29a1b5187:	add    %bl,(%rcx,%riz,2)
 	...
 
 000000029a1b518c <.pdata>:
-   29a1b518c:	and    %ah,(%rcx)
-   29a1b518e:	add    %al,(%rax)
-   29a1b5190:	and    (%rcx),%esp
+   29a1b518c:	push   %rax
+   29a1b518d:	and    %eax,(%rax)
+   29a1b518f:	add    %dl,0x21(%rbx)
    29a1b5192:	add    %al,(%rax)
-   29a1b5194:	sbb    $0x61,%al
+   29a1b5194:	and    %ah,0x0(%rcx)
 	...
 
 000000029a1b5198 <.pdata>:
-   29a1b5198:	jo     29a1b51bb <.pdata+0xb>
-   29a1b519a:	add    %al,(%rax)
-   29a1b519c:	jbe    29a1b51bf <.pdata+0x3>
-   29a1b519e:	add    %al,(%rax)
-   29a1b51a0:	and    %ah,0x0(%rcx)
+   29a1b5198:	movabs 0x24000021a6000021,%al
+   29a1b51a1:	(bad)
 	...
 
 000000029a1b51a4 <.pdata>:
-   29a1b51a4:	andb   $0x0,(%rcx)
-   29a1b51a7:	add    %al,0x24000021(%rsi)
-   29a1b51ad:	(bad)
+   29a1b51a4:	mov    $0x21,%al
+   29a1b51a6:	add    %al,(%rax)
+   29a1b51a8:	mov    $0x21,%dh
+   29a1b51aa:	add    %al,(%rax)
+   29a1b51ac:	sub    %ah,0x0(%rcx)
 	...
 
 000000029a1b51b0 <.pdata>:
-   29a1b51b0:	nop
-   29a1b51b1:	and    %eax,(%rax)
-   29a1b51b3:	add    %ch,0x28000021(%rsi)
-   29a1b51b9:	(bad)
+   29a1b51b0:	shlb   $0x0,(%rcx)
+   29a1b51b3:	add    %bl,%dh
+   29a1b51b5:	and    %eax,(%rax)
+   29a1b51b7:	add    %ch,(%rcx,%riz,2)
 	...
 
 000000029a1b51bc <.pdata>:
-   29a1b51bc:	mov    $0x21,%al
+   29a1b51bc:	loopne 29a1b51df <.pdata+0x23>
    29a1b51be:	add    %al,(%rax)
-   29a1b51c0:	mov    $0x21,%bl
+   29a1b51c0:	jrcxz  29a1b51e3 <.pdata+0x27>
    29a1b51c2:	add    %al,(%rax)
-   29a1b51c4:	xor    %ah,0x0(%rcx)
-   29a1b51c7:	add    %al,%al
-   29a1b51c9:	and    %eax,(%rax)
-   29a1b51cb:	add    %ch,(%rdx)
-   29a1b51cd:	and    (%rax),%al
-   29a1b51cf:	add    %dh,(%rcx,%riz,2)
-   29a1b51d2:	add    %al,(%rax)
-   29a1b51d4:	xor    %ah,(%rdx)
+   29a1b51c4:	xor    $0x61,%al
+   29a1b51c6:	add    %al,(%rax)
+   29a1b51c8:	lock and %eax,(%rax)
+   29a1b51cb:	add    %bl,0x22(%rdx)
+   29a1b51ce:	add    %al,(%rax)
+   29a1b51d0:	cmp    %ah,0x0(%rcx)
+   29a1b51d3:	add    %ah,0x22(%rax)
    29a1b51d6:	add    %al,(%rax)
-   29a1b51d8:	(bad)
-   29a1b51d9:	and    (%rax),%al
-   29a1b51db:	add    %al,0x0(%rcx,%riz,2)
-   29a1b51df:	add    %ah,-0x41ffffde(%rax)
+   29a1b51d8:	lret   $0x22
+   29a1b51db:	add    %cl,0x61(%rax)
+   29a1b51de:	add    %al,(%rax)
+   29a1b51e0:	shlb   $1,(%rdx)
+   29a1b51e2:	add    %al,(%rax)
+   29a1b51e4:	out    %al,(%dx)
    29a1b51e5:	and    (%rax),%al
-   29a1b51e7:	add    %dl,0x0(%rcx,%riz,2)
-   29a1b51eb:	add    %al,%al
-   29a1b51ed:	and    (%rax),%al
-   29a1b51ef:	add    %dl,%ch
-   29a1b51f1:	and    (%rax),%al
-   29a1b51f3:	add    %bl,0x0(%rcx,%riz,2)
-   29a1b51f7:	add    %ah,%al
-   29a1b51f9:	and    (%rax),%al
-   29a1b51fb:	add    %cl,(%rsi)
-   29a1b51fd:	and    (%rax),%eax
-   29a1b51ff:	add    %ah,0x61(%rax)
-   29a1b5202:	add    %al,(%rax)
-   29a1b5204:	adc    %ah,(%rbx)
+   29a1b51e7:	add    %bl,0x61(%rax)
+   29a1b51ea:	add    %al,(%rax)
+   29a1b51ec:	lock and (%rax),%al
+   29a1b51ef:	add    %al,0x60000023(%rip)        # 2fa1b5218 <.debug_rnglists+0x5ffe5174>
+   29a1b51f5:	(bad)
+   29a1b51f6:	add    %al,(%rax)
+   29a1b51f8:	adc    %ah,(%rbx)
+   29a1b51fa:	add    %al,(%rax)
+   29a1b51fc:	ds and (%rax),%eax
+   29a1b51ff:	add    %ah,0x0(%rcx,%riz,2)
+   29a1b5203:	add    %al,0x23(%rax)
    29a1b5206:	add    %al,(%rax)
-   29a1b5208:	and    (%r8),%r8d
-   29a1b520b:	add    %ch,0x61(%rax)
+   29a1b5208:	jne    29a1b522d <.pdata+0x5>
+   29a1b520a:	add    %al,(%rax)
+   29a1b520c:	insb   (%dx),%es:(%rdi)
+   29a1b520d:	(bad)
    29a1b520e:	add    %al,(%rax)
-   29a1b5210:	push   %rax
-   29a1b5211:	and    (%rax),%eax
-   29a1b5213:	add    %al,0x70000023(%rsi)
+   29a1b5210:	andb   $0x0,(%rbx)
+   29a1b5213:	add    %dh,0x74000023(%rsi)
    29a1b5219:	(bad)
    29a1b521a:	add    %al,(%rax)
-   29a1b521c:	nop
-   29a1b521d:	and    (%rax),%eax
-   29a1b521f:	add    %al,%dh
+   29a1b521c:	shlb   $0x0,(%rbx)
+   29a1b521f:	add    %dh,%dh
    29a1b5221:	and    (%rax),%eax
-   29a1b5223:	add    %bh,0x61(%rax)
+   29a1b5223:	add    %bh,0x0(%rcx,%riz,2)
 	...
 
 000000029a1b5228 <.pdata>:
-   29a1b5228:	lock and $0x0,%al
-   29a1b522b:	add    %ah,(%rdx)
-   29a1b522d:	and    $0x61800000,%eax
+   29a1b5228:	xor    %ah,0x25620000(%rip)        # 2bf7d522e <.debug_rnglists+0x2560518a>
+   29a1b522e:	add    %al,(%rax)
+   29a1b5230:	test   %ah,0x0(%rcx)
 	...
 
 000000029a1b5234 <.pdata.startup>:
-   29a1b5234:	andb   $0x0,0x25850000(%rip)        # 2bfa0523b <.debug_rnglists+0x25835197>
+   29a1b5234:	shlb   $0x0,0x25c50000(%rip)        # 2bfe0523b <.debug_rnglists+0x25c35197>
    29a1b523b:	.byte 0
-   29a1b523c:	mov    %ah,0x0(%rcx)
+   29a1b523c:	mov    %fs,0x0(%rcx)
 	...
 
 Disassembly of section .xdata:
 
 000000029a1b6000 <.xdata>:
    29a1b6000:	add    %eax,(%rax)
    29a1b6002:	add    %al,(%rax)
@@ -5674,207 +5691,208 @@
 000000029a1b6030 <.xdata>:
    29a1b6030:	add    %eax,(%rax)
    29a1b6032:	add    %al,(%rax)
    29a1b6034:	add    %eax,(%rax)
 	...
 
 000000029a1b6038 <.xdata>:
-   29a1b6038:	add    %eax,(%rdx,%rax,1)
-   29a1b603b:	add    $0x50010304,%eax
-   29a1b6040:	add    %ecx,(%rax)
-   29a1b6042:	add    0x3043208(%rip),%eax        # 29d1f9250 <.debug_rnglists+0x30291ac>
-   29a1b6048:	add    %edx,0x0(%rax)
-   29a1b604b:	add    %al,(%rcx)
-   29a1b604d:	or     %al,(%rbx)
-   29a1b604f:	add    $0x3045208,%eax
-   29a1b6054:	add    %edx,0x0(%rax)
-   29a1b6057:	add    %al,(%rcx)
-   29a1b6059:	add    $0x2,%al
-   29a1b605b:	add    $0x50010304,%eax
-
-000000029a1b6060 <.xdata>:
-   29a1b6060:	add    %eax,(%rcx,%rax,1)
-   29a1b6063:	add    %al,(%rdx,%rax,2)
-   29a1b6066:	add    %al,(%rax)
-   29a1b6068:	add    %eax,(%rsi)
-   29a1b606a:	add    (%rax),%eax
-   29a1b606c:	(bad)
-   29a1b606d:	rex.X add (%rax),%sil
-   29a1b6070:	add    %esp,0x0(%rax)
-   29a1b6073:	add    %al,(%rcx)
-   29a1b6075:	add    %al,(%rax)
-	...
-
-000000029a1b6078 <.xdata>:
-   29a1b6078:	add    %eax,(%rcx,%rax,1)
-   29a1b607b:	add    %al,(%rdx,%rax,2)
-   29a1b607e:	add    %al,(%rax)
-   29a1b6080:	add    %eax,(%rsi)
-   29a1b6082:	add    (%rax),%eax
-   29a1b6084:	(bad)
-   29a1b6085:	rex.X add (%rax),%sil
-   29a1b6088:	add    %esp,0x0(%rax)
-   29a1b608b:	add    %al,(%rcx)
-   29a1b608d:	add    %al,(%rax)
-	...
-
-000000029a1b6090 <.xdata>:
-   29a1b6090:	add    %eax,(%rsi)
-   29a1b6092:	add    (%rax),%eax
-   29a1b6094:	(bad)
-   29a1b6095:	(bad)
-   29a1b609a:	add    %al,(%rax)
-   29a1b609c:	add    %eax,(%rdi)
-   29a1b609e:	add    $0x0,%al
-   29a1b60a0:	(bad)
-   29a1b60a1:	xchg   %eax,%edx
-   29a1b60a2:	add    (%rax),%esi
-   29a1b60a4:	add    0x1(%rax),%ah
-   29a1b60a7:	jo     29a1b60aa <.xdata+0x1a>
-   29a1b60a9:	adc    $0x315450a,%eax
-   29a1b60ae:	adc    %al,0x600b300c(%rdx)
-   29a1b60b4:	or     0x9(%rax),%dh
-   29a1b60b7:	rolb   $0xd0,(%rdi)
-   29a1b60ba:	add    $0x1f003e0,%eax
-   29a1b60bf:	push   %rax
-
-000000029a1b60c0 <.xdata>:
-   29a1b60c0:	add    %ecx,(%rdx)
-   29a1b60c2:	(bad)
-   29a1b60c3:	add    %cl,(%rdx)
-   29a1b60c5:	xor    (%rsi),%al
-   29a1b60c7:	xor    %al,0x3700460(%rip)        # 29d8b652d <.debug_rnglists+0x36e6489>
-   29a1b60cd:	push   %rax
-   29a1b60ce:	add    %al,%al
-   29a1b60d0:	add    %eax,(%rdi)
-   29a1b60d2:	add    $0x0,%al
-   29a1b60d4:	(bad)
-   29a1b60d5:	xor    (%rbx),%al
-   29a1b60d7:	xor    %al,(%rdx)
-   29a1b60d9:	(bad)
-   29a1b60da:	add    %esi,0x1(%rax)
+   29a1b6038:	add    %ecx,(%rax)
+   29a1b603a:	add    0x3043208(%rip),%eax        # 29d1f9248 <.debug_rnglists+0x30291a4>
+   29a1b6040:	add    %edx,0x0(%rax)
+   29a1b6043:	add    %al,(%rcx)
+   29a1b6045:	or     %al,(%rbx)
+   29a1b6047:	add    $0x3043208,%eax
+   29a1b604c:	add    %edx,0x0(%rax)
+   29a1b604f:	add    %al,(%rcx)
+   29a1b6051:	or     %al,(%rbx)
+   29a1b6053:	add    $0x3045208,%eax
+   29a1b6058:	add    %edx,0x0(%rax)
+   29a1b605b:	add    %al,(%rcx)
+   29a1b605d:	add    $0x2,%al
+   29a1b605f:	add    $0x50010304,%eax
+
+000000029a1b6064 <.xdata>:
+   29a1b6064:	add    %eax,(%rcx,%rax,1)
+   29a1b6067:	add    %al,(%rdx,%rax,2)
+   29a1b606a:	add    %al,(%rax)
+   29a1b606c:	add    %eax,(%rsi)
+   29a1b606e:	add    (%rax),%eax
+   29a1b6070:	(bad)
+   29a1b6071:	rex.X add (%rax),%sil
+   29a1b6074:	add    %esp,0x0(%rax)
+   29a1b6077:	add    %al,(%rcx)
+   29a1b6079:	add    %al,(%rax)
+	...
+
+000000029a1b607c <.xdata>:
+   29a1b607c:	add    %eax,(%rcx,%rax,1)
+   29a1b607f:	add    %al,(%rdx,%rax,2)
+   29a1b6082:	add    %al,(%rax)
+   29a1b6084:	add    %eax,(%rsi)
+   29a1b6086:	add    (%rax),%eax
+   29a1b6088:	(bad)
+   29a1b6089:	rex.X add (%rax),%sil
+   29a1b608c:	add    %esp,0x0(%rax)
+   29a1b608f:	add    %al,(%rcx)
+   29a1b6091:	add    %al,(%rax)
+	...
+
+000000029a1b6094 <.xdata>:
+   29a1b6094:	add    %eax,(%rsi)
+   29a1b6096:	add    (%rax),%eax
+   29a1b6098:	(bad)
+   29a1b6099:	(bad)
+   29a1b609e:	add    %al,(%rax)
+   29a1b60a0:	add    %eax,(%rdi)
+   29a1b60a2:	add    $0x0,%al
+   29a1b60a4:	(bad)
+   29a1b60a5:	xchg   %eax,%edx
+   29a1b60a6:	add    (%rax),%esi
+   29a1b60a8:	add    0x1(%rax),%ah
+   29a1b60ab:	jo     29a1b60ae <.xdata+0x1a>
+   29a1b60ad:	adc    $0x315450a,%eax
+   29a1b60b2:	adc    %al,0x600b300c(%rdx)
+   29a1b60b8:	or     0x9(%rax),%dh
+   29a1b60bb:	rolb   $0xd0,(%rdi)
+   29a1b60be:	add    $0x1f003e0,%eax
+   29a1b60c3:	push   %rax
+
+000000029a1b60c4 <.xdata>:
+   29a1b60c4:	add    %ecx,(%rdx)
+   29a1b60c6:	(bad)
+   29a1b60c7:	add    %cl,(%rdx)
+   29a1b60c9:	xor    (%rsi),%al
+   29a1b60cb:	xor    %al,0x3700460(%rip)        # 29d8b6531 <.debug_rnglists+0x36e648d>
+   29a1b60d1:	push   %rax
+   29a1b60d2:	add    %al,%al
+   29a1b60d4:	add    %eax,(%rdi)
+   29a1b60d6:	add    $0x0,%al
+   29a1b60d8:	(bad)
+   29a1b60d9:	xor    (%rbx),%al
+   29a1b60db:	xor    %al,(%rdx)
    29a1b60dd:	(bad)
-   29a1b60de:	add    (%rax),%eax
-   29a1b60e0:	(bad)
-   29a1b60e1:	rex.X add (%rax),%sil
-   29a1b60e4:	add    %esp,0x0(%rax)
-   29a1b60e7:	add    %al,(%rcx)
-   29a1b60e9:	add    $0x32050002,%eax
-   29a1b60ee:	add    %esi,(%rax)
-
-000000029a1b60f0 <.xdata>:
-   29a1b60f0:	add    %eax,(%rax)
-   29a1b60f2:	add    %al,(%rax)
+   29a1b60de:	add    %esi,0x1(%rax)
+   29a1b60e1:	(bad)
+   29a1b60e2:	add    (%rax),%eax
+   29a1b60e4:	(bad)
+   29a1b60e5:	rex.X add (%rax),%sil
+   29a1b60e8:	add    %esp,0x0(%rax)
+   29a1b60eb:	add    %al,(%rcx)
+   29a1b60ed:	add    $0x32050002,%eax
+   29a1b60f2:	add    %esi,(%rax)
+
+000000029a1b60f4 <.xdata>:
    29a1b60f4:	add    %eax,(%rax)
    29a1b60f6:	add    %al,(%rax)
-   29a1b60f8:	add    %eax,(%rdi)
-   29a1b60fa:	add    $0x0,%al
-   29a1b60fc:	(bad)
-   29a1b60fd:	xor    (%rbx),%al
-   29a1b60ff:	xor    %al,(%rdx)
-   29a1b6101:	(bad)
-   29a1b6102:	add    %esi,0x1(%rax)
-   29a1b6105:	add    %al,(%rax)
-   29a1b6107:	add    %al,(%rcx)
+   29a1b60f8:	add    %eax,(%rax)
+   29a1b60fa:	add    %al,(%rax)
+   29a1b60fc:	add    %eax,(%rdi)
+   29a1b60fe:	add    $0x0,%al
+   29a1b6100:	(bad)
+   29a1b6101:	xor    (%rbx),%al
+   29a1b6103:	xor    %al,(%rdx)
+   29a1b6105:	(bad)
+   29a1b6106:	add    %esi,0x1(%rax)
    29a1b6109:	add    %al,(%rax)
    29a1b610b:	add    %al,(%rcx)
    29a1b610d:	add    %al,(%rax)
    29a1b610f:	add    %al,(%rcx)
    29a1b6111:	add    %al,(%rax)
    29a1b6113:	add    %al,(%rcx)
    29a1b6115:	add    %al,(%rax)
    29a1b6117:	add    %al,(%rcx)
    29a1b6119:	add    %al,(%rax)
-	...
-
-000000029a1b611c <.xdata>:
-   29a1b611c:	add    %eax,(%rax)
+   29a1b611b:	add    %al,(%rcx)
+   29a1b611d:	add    %al,(%rax)
 	...
 
 000000029a1b6120 <.xdata>:
    29a1b6120:	add    %eax,(%rax)
 	...
 
 000000029a1b6124 <.xdata>:
    29a1b6124:	add    %eax,(%rax)
 	...
 
 000000029a1b6128 <.xdata>:
-   29a1b6128:	add    %eax,(%rcx,%rax,1)
-   29a1b612b:	add    %al,(%rdx,%riz,2)
+   29a1b6128:	add    %eax,(%rax)
 	...
 
-000000029a1b6130 <.xdata>:
-   29a1b6130:	add    %eax,(%rax)
-   29a1b6132:	add    %al,(%rax)
-   29a1b6134:	add    %ecx,(%rdx)
-   29a1b6136:	(bad)
-   29a1b6137:	add    %cl,(%rdx)
-   29a1b6139:	xor    (%rsi),%al
-   29a1b613b:	xor    %al,0x3700460(%rip)        # 29d8b65a1 <.debug_rnglists+0x36e64fd>
-   29a1b6141:	push   %rax
-   29a1b6142:	add    %al,%al
-   29a1b6144:	add    %ecx,(%rdx)
-   29a1b6146:	(bad)
-   29a1b6147:	add    %cl,(%rdx)
-   29a1b6149:	xor    (%rsi),%al
-   29a1b614b:	xor    %al,0x3700460(%rip)        # 29d8b65b1 <.debug_rnglists+0x36e650d>
-   29a1b6151:	push   %rax
-   29a1b6152:	add    %al,%al
-   29a1b6154:	add    %eax,0x32050002(%rip)        # 2cc20615c <.debug_rnglists+0x320360b8>
-   29a1b615a:	add    %esi,(%rax)
-   29a1b615c:	add    %eax,(%rax)
-   29a1b615e:	add    %al,(%rax)
-   29a1b6160:	add    %eax,0x32050002(%rip)        # 2cc206168 <.debug_rnglists+0x320360c4>
-   29a1b6166:	add    %esi,(%rax)
-   29a1b6168:	add    %eax,(%rcx,%rax,1)
-   29a1b616b:	add    %al,(%rdx,%rax,4)
-   29a1b616e:	add    %al,(%rax)
-   29a1b6170:	add    %eax,(%rcx,%rax,1)
-   29a1b6173:	add    %al,(%rdx,%rax,2)
-   29a1b6176:	add    %al,(%rax)
-   29a1b6178:	add    %eax,(%rcx,%rax,1)
-   29a1b617b:	add    %al,(%rdx,%rax,2)
-	...
-
-000000029a1b6180 <.xdata>:
-   29a1b6180:	add    %eax,(%rcx,%rax,1)
-   29a1b6183:	add    %al,(%rdx,%rax,4)
+000000029a1b612c <.xdata>:
+   29a1b612c:	add    %eax,(%rcx,%rax,1)
+   29a1b612f:	add    %al,(%rdx,%riz,2)
+	...
+
+000000029a1b6134 <.xdata>:
+   29a1b6134:	add    %eax,(%rax)
+   29a1b6136:	add    %al,(%rax)
+   29a1b6138:	add    %ecx,(%rdx)
+   29a1b613a:	(bad)
+   29a1b613b:	add    %cl,(%rdx)
+   29a1b613d:	xor    (%rsi),%al
+   29a1b613f:	xor    %al,0x3700460(%rip)        # 29d8b65a5 <.debug_rnglists+0x36e6501>
+   29a1b6145:	push   %rax
+   29a1b6146:	add    %al,%al
+   29a1b6148:	add    %ecx,(%rdx)
+   29a1b614a:	(bad)
+   29a1b614b:	add    %cl,(%rdx)
+   29a1b614d:	xor    (%rsi),%al
+   29a1b614f:	xor    %al,0x3700460(%rip)        # 29d8b65b5 <.debug_rnglists+0x36e6511>
+   29a1b6155:	push   %rax
+   29a1b6156:	add    %al,%al
+   29a1b6158:	add    %eax,0x32050002(%rip)        # 2cc206160 <.debug_rnglists+0x320360bc>
+   29a1b615e:	add    %esi,(%rax)
+   29a1b6160:	add    %eax,(%rax)
+   29a1b6162:	add    %al,(%rax)
+   29a1b6164:	add    %eax,0x32050002(%rip)        # 2cc20616c <.debug_rnglists+0x320360c8>
+   29a1b616a:	add    %esi,(%rax)
+   29a1b616c:	add    %eax,(%rcx,%rax,1)
+   29a1b616f:	add    %al,(%rdx,%rax,4)
+   29a1b6172:	add    %al,(%rax)
+   29a1b6174:	add    %eax,(%rcx,%rax,1)
+   29a1b6177:	add    %al,(%rdx,%rax,2)
+   29a1b617a:	add    %al,(%rax)
+   29a1b617c:	add    %eax,(%rcx,%rax,1)
+   29a1b617f:	add    %al,(%rdx,%rax,2)
+	...
+
+000000029a1b6184 <.xdata>:
+   29a1b6184:	add    %eax,(%rcx,%rax,1)
+   29a1b6187:	add    %al,(%rdx,%rax,4)
 	...
 
-000000029a1b6188 <.xdata.startup>:
-   29a1b6188:	add    %eax,(%rax)
+000000029a1b618c <.xdata.startup>:
+   29a1b618c:	add    %eax,(%rax)
 	...
 
 Disassembly of section .edata:
 
 000000029a1b8000 <.edata>:
    29a1b8000:	add    %al,(%rax)
    29a1b8002:	add    %al,(%rax)
-   29a1b8004:	xchg   %eax,%edx
-   29a1b8005:	lea    (%rax),%esi
-   29a1b8007:	data16 add %al,(%rax)
-   29a1b800a:	add    %al,(%rax)
-   29a1b800c:	push   %rax
-   29a1b800d:	addb   $0x0,(%rax)
+   29a1b8004:	adc    %ch,%ch
+   29a1b8006:	xor    %esp,0x0(%rsi)
+   29a1b8009:	add    %al,(%rax)
+   29a1b800b:	add    %dl,-0x80(%rax)
+   29a1b800e:	add    %al,(%rax)
    29a1b8010:	add    %eax,(%rax)
    29a1b8012:	add    %al,(%rax)
    29a1b8014:	add    $0x0,%al
    29a1b8016:	add    %al,(%rax)
    29a1b8018:	add    $0x0,%al
    29a1b801a:	add    %al,(%rax)
    29a1b801c:	sub    %al,-0x7fc80000(%rax)
    29a1b8022:	add    %al,(%rax)
    29a1b8024:	rex.W addb $0x0,(%rax)
-   29a1b8028:	(bad)
-   29a1b8029:	adc    (%rax),%eax
-   29a1b802b:	add    %al,-0x78ffffed(%rax)
-   29a1b8031:	adc    (%rax),%eax
-   29a1b8033:	add    %bh,0x63000013(%rdi)
-   29a1b8039:	addb   $0x0,(%rax)
+   29a1b8028:	mov    $0x80000013,%eax
+   29a1b802d:	adc    (%rax),%eax
+   29a1b802f:	add    %ah,-0x13ffffed(%rbp)
+   29a1b8035:	adc    (%rax),%eax
+   29a1b8037:	add    %ah,-0x80(%rbx)
+   29a1b803a:	add    %al,(%rax)
    29a1b803c:	jo     29a1b7fbe <__bss_end__+0xeae>
    29a1b803e:	add    %al,(%rax)
    29a1b8040:	jne    29a1b7fc2 <__bss_end__+0xeb2>
    29a1b8042:	add    %al,(%rax)
    29a1b8044:	(bad)
    29a1b8045:	addb   $0x0,(%rax)
    29a1b8048:	add    %al,(%rax)
@@ -5907,1158 +5925,1150 @@
 Disassembly of section .idata:
 
 000000029a1b9000 <_head_lib64_libkernel32_a>:
    29a1b9000:	mov    $0x90,%eax
    29a1b9005:	add    %al,(%rax)
    29a1b9007:	add    %al,(%rax)
    29a1b9009:	add    %al,(%rax)
-   29a1b900b:	add    %dl,%al
+   29a1b900b:	add    %ch,%al
    29a1b900d:	xchg   %eax,%esi
    29a1b900e:	add    %al,(%rax)
-   29a1b9010:	xchg   %rax,%rdx
+   29a1b9010:	push   %rax
+   29a1b9011:	xchg   %eax,%edx
 	...
 
 000000029a1b9014 <_head_lib64_libapi_ms_win_crt_conio_l1_1_0_a>:
    29a1b9014:	or     %dl,0x0(%rcx)
    29a1b901a:	add    %al,(%rax)
    29a1b901c:	add    %al,(%rax)
    29a1b901e:	add    %al,(%rax)
-   29a1b9020:	in     $0x96,%al
+   29a1b9020:	cld
+   29a1b9021:	xchg   %eax,%esi
    29a1b9022:	add    %al,(%rax)
-   29a1b9024:	cwtl
-   29a1b9025:	xchg   %eax,%edx
-	...
+   29a1b9024:	movabs 0x9118000092,%al
 
 000000029a1b9028 <_head_lib64_libapi_ms_win_crt_environment_l1_1_0_a>:
    29a1b9028:	sbb    %dl,0x0(%rcx)
    29a1b902e:	add    %al,(%rax)
    29a1b9030:	add    %al,(%rax)
    29a1b9032:	add    %al,(%rax)
-   29a1b9034:	or     $0x97,%al
+   29a1b9034:	and    $0x97,%al
    29a1b9036:	add    %al,(%rax)
-   29a1b9038:	test   $0x92,%al
+   29a1b9038:	mov    $0x92,%al
 	...
 
 000000029a1b903c <_head_lib64_libapi_ms_win_crt_heap_l1_1_0_a>:
    29a1b903c:	xor    %dl,0x0(%rcx)
    29a1b9042:	add    %al,(%rax)
    29a1b9044:	add    %al,(%rax)
    29a1b9046:	add    %al,(%rax)
-   29a1b9048:	rex xchg %eax,%edi
+   29a1b9048:	pop    %rax
+   29a1b9049:	xchg   %eax,%edi
    29a1b904a:	add    %al,(%rax)
-   29a1b904c:	rclb   $0x0,-0x6eb00000(%rdx)
+   29a1b904c:	enter  $0x92,$0x0
 
 000000029a1b9050 <_head_lib64_libapi_ms_win_crt_runtime_l1_1_0_a>:
    29a1b9050:	push   %rax
    29a1b9051:	xchg   %eax,%ecx
 	...
    29a1b905a:	add    %al,(%rax)
-   29a1b905c:	pushf
-   29a1b905d:	xchg   %eax,%edi
+   29a1b905c:	mov    $0x97,%ah
    29a1b905e:	add    %al,(%rax)
-   29a1b9060:	loopne 29a1b8ff4 <__bss_end__+0x1ee4>
-	...
+   29a1b9060:	call   26a1b90f7 <__size_of_stack_reserve__+0x269fb90f7>
 
 000000029a1b9064 <_head_lib64_libapi_ms_win_crt_stdio_l1_1_0_a>:
    29a1b9064:	rclb   $1,0x0(%rcx)
    29a1b906a:	add    %al,(%rax)
    29a1b906c:	add    %al,(%rax)
    29a1b906e:	add    %al,(%rax)
-   29a1b9070:	fcoms  -0x6ca00000(%rdi)
-	...
+   29a1b9070:	hlt
+   29a1b9071:	xchg   %eax,%edi
+   29a1b9072:	add    %al,(%rax)
+   29a1b9074:	push   $0x10000093
 
 000000029a1b9078 <_head_lib64_libapi_ms_win_crt_string_l1_1_0_a>:
-   29a1b9078:	or     %dl,0x0(%rdx)
+   29a1b9078:	adc    %dl,0x0(%rdx)
    29a1b907e:	add    %al,(%rax)
    29a1b9080:	add    %al,(%rax)
    29a1b9082:	add    %al,(%rax)
-   29a1b9084:	add    %bl,-0x6c680000(%rax)
+   29a1b9084:	sbb    $0x98,%al
+   29a1b9086:	add    %al,(%rax)
+   29a1b9088:	test   $0x93,%al
 	...
 
 000000029a1b908c <_head_lib64_libapi_ms_win_crt_time_l1_1_0_a>:
-   29a1b908c:	and    %dl,0x0(%rdx)
+   29a1b908c:	sub    %dl,0x0(%rdx)
    29a1b9092:	add    %al,(%rax)
    29a1b9094:	add    %al,(%rax)
    29a1b9096:	add    %al,(%rax)
-   29a1b9098:	xor    $0x98,%al
+   29a1b9098:	push   %rax
+   29a1b9099:	cwtl
    29a1b909a:	add    %al,(%rax)
-   29a1b909c:	mov    $0x93,%al
+   29a1b909c:	rclb   $0x0,0x0(%rbx)
 	...
 
 000000029a1b90b8 <hname>:
-   29a1b90b8:	fcoms  0x0(%rbx)
+   29a1b90b8:	call   29a1b9150 <hname>
+   29a1b90bd:	add    %al,(%rax)
 	...
 
 000000029a1b90c0 <.idata$4>:
-   29a1b90c0:	lock xchg %eax,%ebx
-   29a1b90c2:	add    %al,(%rax)
-   29a1b90c4:	add    %al,(%rax)
+   29a1b90c0:	add    %dl,0x0(%rax,%rax,1)
 	...
 
 000000029a1b90c8 <.idata$4>:
-   29a1b90c8:	or     %dl,0x0(%rax,%rax,1)
+   29a1b90c8:	sbb    %dl,0x0(%rax,%rax,1)
 	...
 
 000000029a1b90d0 <.idata$4>:
-   29a1b90d0:	sbb    %dl,0x0(%rax,%rax,1)
+   29a1b90d0:	sub    %dl,0x0(%rax,%rax,1)
 	...
 
 000000029a1b90d8 <.idata$4>:
-   29a1b90d8:	xor    $0x94,%al
+   29a1b90d8:	rex.R xchg %eax,%esp
    29a1b90da:	add    %al,(%rax)
    29a1b90dc:	add    %al,(%rax)
 	...
 
 000000029a1b90e0 <.idata$4>:
-   29a1b90e0:	rex.WR xchg %rax,%rsp
+   29a1b90e0:	pop    %rsp
+   29a1b90e1:	xchg   %eax,%esp
    29a1b90e2:	add    %al,(%rax)
    29a1b90e4:	add    %al,(%rax)
 	...
 
 000000029a1b90e8 <.idata$4>:
-   29a1b90e8:	push   %rsp
-   29a1b90e9:	xchg   %eax,%esp
+   29a1b90e8:	fs xchg %eax,%esp
    29a1b90ea:	add    %al,(%rax)
    29a1b90ec:	add    %al,(%rax)
 	...
 
 000000029a1b90f0 <.idata$4>:
-   29a1b90f0:	(bad)
-   29a1b90f3:	add    %al,(%rax)
-   29a1b90f5:	add    %al,(%rax)
+   29a1b90f0:	jb     29a1b9086 <_head_lib64_libapi_ms_win_crt_string_l1_1_0_a+0xe>
+   29a1b90f2:	add    %al,(%rax)
+   29a1b90f4:	add    %al,(%rax)
 	...
 
 000000029a1b90f8 <.idata$4>:
-   29a1b90f8:	je     29a1b908e <_head_lib64_libapi_ms_win_crt_time_l1_1_0_a+0x2>
-   29a1b90fa:	add    %al,(%rax)
-   29a1b90fc:	add    %al,(%rax)
+   29a1b90f8:	test   %dl,0x0(%rax,%rax,1)
 	...
 
 000000029a1b9100 <.idata$4>:
 	...
 
 000000029a1b9108 <hname>:
-   29a1b9108:	test   %dl,0x0(%rax,%rax,1)
+   29a1b9108:	xchg   %eax,%esp
+   29a1b9109:	xchg   %eax,%esp
+   29a1b910a:	add    %al,(%rax)
+   29a1b910c:	add    %al,(%rax)
 	...
 
 000000029a1b9110 <.idata$4>:
 	...
 
 000000029a1b9118 <hname>:
-   29a1b9118:	mov    0x0(%rax,%rax,1),%ss
+   29a1b9118:	sahf
+   29a1b9119:	xchg   %eax,%esp
+   29a1b911a:	add    %al,(%rax)
+   29a1b911c:	add    %al,(%rax)
 	...
 
 000000029a1b9120 <.idata$4>:
-   29a1b9120:	sahf
+   29a1b9120:	scas   %es:(%rdi),%al
    29a1b9121:	xchg   %eax,%esp
    29a1b9122:	add    %al,(%rax)
    29a1b9124:	add    %al,(%rax)
 	...
 
 000000029a1b9128 <.idata$4>:
 	...
 
 000000029a1b9130 <hname>:
-   29a1b9130:	scas   %es:(%rdi),%al
-   29a1b9131:	xchg   %eax,%esp
-   29a1b9132:	add    %al,(%rax)
-   29a1b9134:	add    %al,(%rax)
+   29a1b9130:	mov    $0x94,%esi
+   29a1b9135:	add    %al,(%rax)
 	...
 
 000000029a1b9138 <.idata$4>:
-   29a1b9138:	mov    $0x94,%esi
-   29a1b913d:	add    %al,(%rax)
+   29a1b9138:	(bad)
+   29a1b9139:	xchg   %eax,%esp
+   29a1b913a:	add    %al,(%rax)
+   29a1b913c:	add    %al,(%rax)
 	...
 
 000000029a1b9140 <.idata$4>:
-   29a1b9140:	enter  $0x94,$0x0
-   29a1b9144:	add    %al,(%rax)
+   29a1b9140:	fcoms  0x0(%rax,%rax,1)
 	...
 
 000000029a1b9148 <.idata$4>:
 	...
 
 000000029a1b9150 <hname>:
-   29a1b9150:	rclb   $1,0x0(%rax,%rax,1)
+   29a1b9150:	loopne 29a1b90e6 <.idata$4+0x6>
+   29a1b9152:	add    %al,(%rax)
+   29a1b9154:	add    %al,(%rax)
 	...
 
 000000029a1b9158 <.idata$4>:
-   29a1b9158:	ficoms 0x0(%rax,%rax,1)
+   29a1b9158:	out    %al,(%dx)
+   29a1b9159:	xchg   %eax,%esp
+   29a1b915a:	add    %al,(%rax)
+   29a1b915c:	add    %al,(%rax)
 	...
 
 000000029a1b9160 <.idata$4>:
-   29a1b9160:	in     (%dx),%al
+   29a1b9160:	cld
    29a1b9161:	xchg   %eax,%esp
    29a1b9162:	add    %al,(%rax)
    29a1b9164:	add    %al,(%rax)
 	...
 
 000000029a1b9168 <.idata$4>:
-   29a1b9168:	cli
-   29a1b9169:	xchg   %eax,%esp
-   29a1b916a:	add    %al,(%rax)
-   29a1b916c:	add    %al,(%rax)
+   29a1b9168:	or     0x0(%rbp),%dl
 	...
 
 000000029a1b9170 <.idata$4>:
-   29a1b9170:	adc    $0x95,%al
+   29a1b9170:	and    $0x95,%al
    29a1b9172:	add    %al,(%rax)
    29a1b9174:	add    %al,(%rax)
 	...
 
 000000029a1b9178 <.idata$4>:
-   29a1b9178:	sub    $0x95,%al
+   29a1b9178:	cmp    $0x95,%al
    29a1b917a:	add    %al,(%rax)
    29a1b917c:	add    %al,(%rax)
 	...
 
 000000029a1b9180 <.idata$4>:
-   29a1b9180:	rex.X xchg %eax,%ebp
+   29a1b9180:	push   %rdx
+   29a1b9181:	xchg   %eax,%ebp
    29a1b9182:	add    %al,(%rax)
    29a1b9184:	add    %al,(%rax)
 	...
 
 000000029a1b9188 <.idata$4>:
-   29a1b9188:	push   %rax
+   29a1b9188:	(bad)
    29a1b9189:	xchg   %eax,%ebp
    29a1b918a:	add    %al,(%rax)
    29a1b918c:	add    %al,(%rax)
 	...
 
 000000029a1b9190 <.idata$4>:
-   29a1b9190:	push   $0x95
-   29a1b9195:	add    %al,(%rax)
+   29a1b9190:	js     29a1b9127 <.idata$4+0x7>
+   29a1b9192:	add    %al,(%rax)
+   29a1b9194:	add    %al,(%rax)
 	...
 
 000000029a1b9198 <.idata$4>:
-   29a1b9198:	jo     29a1b912f <.idata$4+0x7>
-   29a1b919a:	add    %al,(%rax)
-   29a1b919c:	add    %al,(%rax)
+   29a1b9198:	adcb   $0x0,0x0(%rbp)
 	...
 
 000000029a1b91a0 <.idata$4>:
-   29a1b91a0:	xchg   %eax,%edx
-   29a1b91a1:	xchg   %eax,%ebp
-   29a1b91a2:	add    %al,(%rax)
-   29a1b91a4:	add    %al,(%rax)
-	...
+   29a1b91a0:	movabs %al,0xbe00000000000095
 
 000000029a1b91a8 <.idata$4>:
-   29a1b91a8:	scas   %es:(%rdi),%al
-   29a1b91a9:	xchg   %eax,%ebp
-   29a1b91aa:	add    %al,(%rax)
-   29a1b91ac:	add    %al,(%rax)
+   29a1b91a8:	mov    $0x95,%esi
+   29a1b91ad:	add    %al,(%rax)
 	...
 
 000000029a1b91b0 <.idata$4>:
-   29a1b91b0:	(bad)
-   29a1b91b1:	xchg   %eax,%ebp
-   29a1b91b2:	add    %al,(%rax)
-   29a1b91b4:	add    %al,(%rax)
+   29a1b91b0:	ficoms 0x0(%rbp)
 	...
 
 000000029a1b91b8 <.idata$4>:
-   29a1b91b8:	ficoml 0x0(%rbp)
+   29a1b91b8:	(bad)
+   29a1b91b9:	xchg   %eax,%ebp
+   29a1b91ba:	add    %al,(%rax)
+   29a1b91bc:	add    %al,(%rax)
 	...
 
 000000029a1b91c0 <.idata$4>:
-   29a1b91c0:	notb   0x0(%rbp)
+   29a1b91c0:	(bad)
+   29a1b91c1:	xchg   %eax,%esi
+   29a1b91c2:	add    %al,(%rax)
+   29a1b91c4:	add    %al,(%rax)
 	...
 
 000000029a1b91c8 <.idata$4>:
 	...
 
 000000029a1b91d0 <hname>:
    29a1b91d0:	(bad)
-   29a1b91d1:	xchg   %eax,%ebp
+   29a1b91d1:	xchg   %eax,%esi
    29a1b91d2:	add    %al,(%rax)
    29a1b91d4:	add    %al,(%rax)
 	...
 
 000000029a1b91d8 <.idata$4>:
-   29a1b91d8:	adc    %dl,0x0(%rsi)
+   29a1b91d8:	and    %dl,0x0(%rsi)
 	...
 
 000000029a1b91e0 <.idata$4>:
-   29a1b91e0:	sub    0x0(%rsi),%dl
+   29a1b91e0:	cmp    0x0(%rsi),%dl
 	...
 
 000000029a1b91e8 <.idata$4>:
-   29a1b91e8:	rex.RX xchg %eax,%esi
+   29a1b91e8:	push   %rsi
+   29a1b91e9:	xchg   %eax,%esi
    29a1b91ea:	add    %al,(%rax)
    29a1b91ec:	add    %al,(%rax)
 	...
 
 000000029a1b91f0 <.idata$4>:
-   29a1b91f0:	push   %rax
+   29a1b91f0:	(bad)
    29a1b91f1:	xchg   %eax,%esi
    29a1b91f2:	add    %al,(%rax)
    29a1b91f4:	add    %al,(%rax)
 	...
 
 000000029a1b91f8 <.idata$4>:
-   29a1b91f8:	pop    %rdx
-   29a1b91f9:	xchg   %eax,%esi
+   29a1b91f8:	push   $0xffffffffffffff96
    29a1b91fa:	add    %al,(%rax)
    29a1b91fc:	add    %al,(%rax)
 	...
 
 000000029a1b9200 <.idata$4>:
+   29a1b9200:	je     29a1b9198 <.idata$4>
+   29a1b9202:	add    %al,(%rax)
+   29a1b9204:	add    %al,(%rax)
 	...
 
-000000029a1b9208 <hname>:
-   29a1b9208:	fs xchg %eax,%esi
-   29a1b920a:	add    %al,(%rax)
-   29a1b920c:	add    %al,(%rax)
+000000029a1b9208 <.idata$4>:
 	...
 
-000000029a1b9210 <.idata$4>:
-   29a1b9210:	outsb  %ds:(%rsi),(%dx)
-   29a1b9211:	xchg   %eax,%esi
+000000029a1b9210 <hname>:
+   29a1b9210:	jle    29a1b91a8 <.idata$4>
    29a1b9212:	add    %al,(%rax)
    29a1b9214:	add    %al,(%rax)
 	...
 
 000000029a1b9218 <.idata$4>:
+   29a1b9218:	mov    %dl,0x0(%rsi)
 	...
 
-000000029a1b9220 <hname>:
-   29a1b9220:	js     29a1b91b8 <.idata$4>
-   29a1b9222:	add    %al,(%rax)
-   29a1b9224:	add    %al,(%rax)
+000000029a1b9220 <.idata$4>:
 	...
 
-000000029a1b9228 <.idata$4>:
-   29a1b9228:	xchg   %dl,0x0(%rsi)
+000000029a1b9228 <hname>:
+   29a1b9228:	xchg   %eax,%edx
+   29a1b9229:	xchg   %eax,%esi
+   29a1b922a:	add    %al,(%rax)
+   29a1b922c:	add    %al,(%rax)
 	...
 
 000000029a1b9230 <.idata$4>:
-   29a1b9230:	xchg   %eax,%esp
-   29a1b9231:	xchg   %eax,%esi
-   29a1b9232:	add    %al,(%rax)
-   29a1b9234:	add    %al,(%rax)
-	...
+   29a1b9230:	movabs 0xae00000000000096,%al
 
 000000029a1b9238 <.idata$4>:
-   29a1b9238:	movabs 0x96,%al
+   29a1b9238:	scas   %es:(%rdi),%al
+   29a1b9239:	xchg   %eax,%esi
+   29a1b923a:	add    %al,(%rax)
+   29a1b923c:	add    %al,(%rax)
+	...
 
 000000029a1b9240 <.idata$4>:
+   29a1b9240:	mov    $0x96,%edx
+   29a1b9245:	add    %al,(%rax)
 	...
 
-000000029a1b9248 <__IAT_start__>:
-   29a1b9248:	fcoms  0x0(%rbx)
+000000029a1b9248 <.idata$4>:
 	...
 
-000000029a1b9250 <__imp_EnterCriticalSection>:
-   29a1b9250:	lock xchg %eax,%ebx
-   29a1b9252:	add    %al,(%rax)
-   29a1b9254:	add    %al,(%rax)
+000000029a1b9250 <__IAT_start__>:
+   29a1b9250:	call   29a1b92e8 <__imp___p___argc>
+   29a1b9255:	add    %al,(%rax)
 	...
 
-000000029a1b9258 <__imp_GetLastError>:
-   29a1b9258:	or     %dl,0x0(%rax,%rax,1)
+000000029a1b9258 <__imp_EnterCriticalSection>:
+   29a1b9258:	add    %dl,0x0(%rax,%rax,1)
 	...
 
-000000029a1b9260 <__imp_InitializeCriticalSection>:
+000000029a1b9260 <__imp_GetLastError>:
    29a1b9260:	sbb    %dl,0x0(%rax,%rax,1)
 	...
 
-000000029a1b9268 <__imp_LeaveCriticalSection>:
-   29a1b9268:	xor    $0x94,%al
-   29a1b926a:	add    %al,(%rax)
-   29a1b926c:	add    %al,(%rax)
+000000029a1b9268 <__imp_InitializeCriticalSection>:
+   29a1b9268:	sub    %dl,0x0(%rax,%rax,1)
 	...
 
-000000029a1b9270 <__imp_Sleep>:
-   29a1b9270:	rex.WR xchg %rax,%rsp
+000000029a1b9270 <__imp_LeaveCriticalSection>:
+   29a1b9270:	rex.R xchg %eax,%esp
    29a1b9272:	add    %al,(%rax)
    29a1b9274:	add    %al,(%rax)
 	...
 
-000000029a1b9278 <__imp_TlsGetValue>:
-   29a1b9278:	push   %rsp
+000000029a1b9278 <__imp_Sleep>:
+   29a1b9278:	pop    %rsp
    29a1b9279:	xchg   %eax,%esp
    29a1b927a:	add    %al,(%rax)
    29a1b927c:	add    %al,(%rax)
 	...
 
-000000029a1b9280 <__imp_VirtualProtect>:
-   29a1b9280:	(bad)
-   29a1b9283:	add    %al,(%rax)
-   29a1b9285:	add    %al,(%rax)
+000000029a1b9280 <__imp_TlsGetValue>:
+   29a1b9280:	fs xchg %eax,%esp
+   29a1b9282:	add    %al,(%rax)
+   29a1b9284:	add    %al,(%rax)
 	...
 
-000000029a1b9288 <__imp_VirtualQuery>:
-   29a1b9288:	je     29a1b921e <.idata$4+0x6>
+000000029a1b9288 <__imp_VirtualProtect>:
+   29a1b9288:	jb     29a1b921e <.idata$4+0x6>
    29a1b928a:	add    %al,(%rax)
    29a1b928c:	add    %al,(%rax)
 	...
 
-000000029a1b9290 <.idata$5>:
+000000029a1b9290 <__imp_VirtualQuery>:
+   29a1b9290:	test   %dl,0x0(%rax,%rax,1)
 	...
 
-000000029a1b9298 <__imp_getch>:
-   29a1b9298:	test   %dl,0x0(%rax,%rax,1)
+000000029a1b9298 <.idata$5>:
 	...
 
-000000029a1b92a0 <.idata$5>:
+000000029a1b92a0 <__imp_getch>:
+   29a1b92a0:	xchg   %eax,%esp
+   29a1b92a1:	xchg   %eax,%esp
+   29a1b92a2:	add    %al,(%rax)
+   29a1b92a4:	add    %al,(%rax)
 	...
 
-000000029a1b92a8 <__imp___p__environ>:
-   29a1b92a8:	mov    0x0(%rax,%rax,1),%ss
+000000029a1b92a8 <.idata$5>:
 	...
 
-000000029a1b92b0 <__imp___p__wenviron>:
+000000029a1b92b0 <__imp___p__environ>:
    29a1b92b0:	sahf
    29a1b92b1:	xchg   %eax,%esp
    29a1b92b2:	add    %al,(%rax)
    29a1b92b4:	add    %al,(%rax)
 	...
 
-000000029a1b92b8 <.idata$5>:
+000000029a1b92b8 <__imp___p__wenviron>:
+   29a1b92b8:	scas   %es:(%rdi),%al
+   29a1b92b9:	xchg   %eax,%esp
+   29a1b92ba:	add    %al,(%rax)
+   29a1b92bc:	add    %al,(%rax)
 	...
 
-000000029a1b92c0 <__imp__set_new_mode>:
-   29a1b92c0:	scas   %es:(%rdi),%al
-   29a1b92c1:	xchg   %eax,%esp
-   29a1b92c2:	add    %al,(%rax)
-   29a1b92c4:	add    %al,(%rax)
+000000029a1b92c0 <.idata$5>:
 	...
 
-000000029a1b92c8 <__imp_calloc>:
+000000029a1b92c8 <__imp__set_new_mode>:
    29a1b92c8:	mov    $0x94,%esi
    29a1b92cd:	add    %al,(%rax)
 	...
 
-000000029a1b92d0 <__imp_free>:
-   29a1b92d0:	enter  $0x94,$0x0
+000000029a1b92d0 <__imp_calloc>:
+   29a1b92d0:	(bad)
+   29a1b92d1:	xchg   %eax,%esp
+   29a1b92d2:	add    %al,(%rax)
    29a1b92d4:	add    %al,(%rax)
 	...
 
-000000029a1b92d8 <.idata$5>:
+000000029a1b92d8 <__imp_free>:
+   29a1b92d8:	fcoms  0x0(%rax,%rax,1)
 	...
 
-000000029a1b92e0 <__imp___p___argc>:
-   29a1b92e0:	rclb   $1,0x0(%rax,%rax,1)
+000000029a1b92e0 <.idata$5>:
 	...
 
-000000029a1b92e8 <__imp___p___argv>:
-   29a1b92e8:	ficoms 0x0(%rax,%rax,1)
+000000029a1b92e8 <__imp___p___argc>:
+   29a1b92e8:	loopne 29a1b927e <__imp_Sleep+0x6>
+   29a1b92ea:	add    %al,(%rax)
+   29a1b92ec:	add    %al,(%rax)
 	...
 
-000000029a1b92f0 <__imp___p___wargv>:
-   29a1b92f0:	in     (%dx),%al
+000000029a1b92f0 <__imp___p___argv>:
+   29a1b92f0:	out    %al,(%dx)
    29a1b92f1:	xchg   %eax,%esp
    29a1b92f2:	add    %al,(%rax)
    29a1b92f4:	add    %al,(%rax)
 	...
 
-000000029a1b92f8 <__imp__configure_narrow_argv>:
-   29a1b92f8:	cli
+000000029a1b92f8 <__imp___p___wargv>:
+   29a1b92f8:	cld
    29a1b92f9:	xchg   %eax,%esp
    29a1b92fa:	add    %al,(%rax)
    29a1b92fc:	add    %al,(%rax)
 	...
 
-000000029a1b9300 <__imp__configure_wide_argv>:
-   29a1b9300:	adc    $0x95,%al
-   29a1b9302:	add    %al,(%rax)
-   29a1b9304:	add    %al,(%rax)
+000000029a1b9300 <__imp__configure_narrow_argv>:
+   29a1b9300:	or     0x0(%rbp),%dl
 	...
 
-000000029a1b9308 <__imp__crt_at_quick_exit>:
-   29a1b9308:	sub    $0x95,%al
+000000029a1b9308 <__imp__configure_wide_argv>:
+   29a1b9308:	and    $0x95,%al
    29a1b930a:	add    %al,(%rax)
    29a1b930c:	add    %al,(%rax)
 	...
 
-000000029a1b9310 <__imp__crt_atexit>:
-   29a1b9310:	rex.X xchg %eax,%ebp
+000000029a1b9310 <__imp__crt_at_quick_exit>:
+   29a1b9310:	cmp    $0x95,%al
    29a1b9312:	add    %al,(%rax)
    29a1b9314:	add    %al,(%rax)
 	...
 
-000000029a1b9318 <__imp__execute_onexit_table>:
-   29a1b9318:	push   %rax
+000000029a1b9318 <__imp__crt_atexit>:
+   29a1b9318:	push   %rdx
    29a1b9319:	xchg   %eax,%ebp
    29a1b931a:	add    %al,(%rax)
    29a1b931c:	add    %al,(%rax)
 	...
 
-000000029a1b9320 <__imp__exit>:
-   29a1b9320:	push   $0x95
-   29a1b9325:	add    %al,(%rax)
+000000029a1b9320 <__imp__execute_onexit_table>:
+   29a1b9320:	(bad)
+   29a1b9321:	xchg   %eax,%ebp
+   29a1b9322:	add    %al,(%rax)
+   29a1b9324:	add    %al,(%rax)
 	...
 
-000000029a1b9328 <__imp__initialize_narrow_environment>:
-   29a1b9328:	jo     29a1b92bf <.idata$5+0x7>
+000000029a1b9328 <__imp__exit>:
+   29a1b9328:	js     29a1b92bf <__imp___p__wenviron+0x7>
    29a1b932a:	add    %al,(%rax)
    29a1b932c:	add    %al,(%rax)
 	...
 
-000000029a1b9330 <__imp__initialize_onexit_table>:
-   29a1b9330:	xchg   %eax,%edx
-   29a1b9331:	xchg   %eax,%ebp
-   29a1b9332:	add    %al,(%rax)
-   29a1b9334:	add    %al,(%rax)
+000000029a1b9330 <__imp__initialize_narrow_environment>:
+   29a1b9330:	adcb   $0x0,0x0(%rbp)
 	...
 
-000000029a1b9338 <__imp__initialize_wide_environment>:
-   29a1b9338:	scas   %es:(%rdi),%al
-   29a1b9339:	xchg   %eax,%ebp
-   29a1b933a:	add    %al,(%rax)
-   29a1b933c:	add    %al,(%rax)
-	...
+000000029a1b9338 <__imp__initialize_onexit_table>:
+   29a1b9338:	movabs %al,0xbe00000000000095
 
-000000029a1b9340 <__imp__initterm>:
-   29a1b9340:	(bad)
-   29a1b9341:	xchg   %eax,%ebp
-   29a1b9342:	add    %al,(%rax)
-   29a1b9344:	add    %al,(%rax)
+000000029a1b9340 <__imp__initialize_wide_environment>:
+   29a1b9340:	mov    $0x95,%esi
+   29a1b9345:	add    %al,(%rax)
 	...
 
-000000029a1b9348 <__imp__register_onexit_function>:
-   29a1b9348:	ficoml 0x0(%rbp)
+000000029a1b9348 <__imp__initterm>:
+   29a1b9348:	ficoms 0x0(%rbp)
 	...
 
-000000029a1b9350 <__imp_abort>:
-   29a1b9350:	notb   0x0(%rbp)
+000000029a1b9350 <__imp__register_onexit_function>:
+   29a1b9350:	(bad)
+   29a1b9351:	xchg   %eax,%ebp
+   29a1b9352:	add    %al,(%rax)
+   29a1b9354:	add    %al,(%rax)
 	...
 
-000000029a1b9358 <.idata$5>:
+000000029a1b9358 <__imp_abort>:
+   29a1b9358:	(bad)
+   29a1b9359:	xchg   %eax,%esi
+   29a1b935a:	add    %al,(%rax)
+   29a1b935c:	add    %al,(%rax)
 	...
 
-000000029a1b9360 <__imp___acrt_iob_func>:
-   29a1b9360:	(bad)
-   29a1b9361:	xchg   %eax,%ebp
-   29a1b9362:	add    %al,(%rax)
-   29a1b9364:	add    %al,(%rax)
+000000029a1b9360 <.idata$5>:
 	...
 
-000000029a1b9368 <__imp___stdio_common_vfprintf>:
-   29a1b9368:	adc    %dl,0x0(%rsi)
+000000029a1b9368 <__imp___acrt_iob_func>:
+   29a1b9368:	(bad)
+   29a1b9369:	xchg   %eax,%esi
+   29a1b936a:	add    %al,(%rax)
+   29a1b936c:	add    %al,(%rax)
 	...
 
-000000029a1b9370 <__imp___stdio_common_vfwprintf>:
-   29a1b9370:	sub    0x0(%rsi),%dl
+000000029a1b9370 <__imp___stdio_common_vfprintf>:
+   29a1b9370:	and    %dl,0x0(%rsi)
 	...
 
-000000029a1b9378 <__imp_kbhit>:
-   29a1b9378:	rex.RX xchg %eax,%esi
-   29a1b937a:	add    %al,(%rax)
-   29a1b937c:	add    %al,(%rax)
+000000029a1b9378 <__imp___stdio_common_vfwprintf>:
+   29a1b9378:	cmp    0x0(%rsi),%dl
 	...
 
-000000029a1b9380 <__imp_fwrite>:
-   29a1b9380:	push   %rax
+000000029a1b9380 <__imp_kbhit>:
+   29a1b9380:	push   %rsi
    29a1b9381:	xchg   %eax,%esi
    29a1b9382:	add    %al,(%rax)
    29a1b9384:	add    %al,(%rax)
 	...
 
-000000029a1b9388 <__imp_putchar>:
-   29a1b9388:	pop    %rdx
+000000029a1b9388 <__imp_fflush>:
+   29a1b9388:	(bad)
    29a1b9389:	xchg   %eax,%esi
    29a1b938a:	add    %al,(%rax)
    29a1b938c:	add    %al,(%rax)
 	...
 
-000000029a1b9390 <.idata$5>:
+000000029a1b9390 <__imp_fwrite>:
+   29a1b9390:	push   $0xffffffffffffff96
+   29a1b9392:	add    %al,(%rax)
+   29a1b9394:	add    %al,(%rax)
 	...
 
-000000029a1b9398 <__imp_strlen>:
-   29a1b9398:	fs xchg %eax,%esi
+000000029a1b9398 <__imp_putchar>:
+   29a1b9398:	je     29a1b9330 <__imp__initialize_narrow_environment>
    29a1b939a:	add    %al,(%rax)
    29a1b939c:	add    %al,(%rax)
 	...
 
-000000029a1b93a0 <__imp_strncmp>:
-   29a1b93a0:	outsb  %ds:(%rsi),(%dx)
-   29a1b93a1:	xchg   %eax,%esi
-   29a1b93a2:	add    %al,(%rax)
-   29a1b93a4:	add    %al,(%rax)
+000000029a1b93a0 <.idata$5>:
 	...
 
-000000029a1b93a8 <.idata$5>:
+000000029a1b93a8 <__imp_strlen>:
+   29a1b93a8:	jle    29a1b9340 <__imp__initialize_wide_environment>
+   29a1b93aa:	add    %al,(%rax)
+   29a1b93ac:	add    %al,(%rax)
 	...
 
-000000029a1b93b0 <__imp___daylight>:
-   29a1b93b0:	js     29a1b9348 <__imp__register_onexit_function>
-   29a1b93b2:	add    %al,(%rax)
-   29a1b93b4:	add    %al,(%rax)
+000000029a1b93b0 <__imp_strncmp>:
+   29a1b93b0:	mov    %dl,0x0(%rsi)
 	...
 
-000000029a1b93b8 <__imp___timezone>:
-   29a1b93b8:	xchg   %dl,0x0(%rsi)
+000000029a1b93b8 <.idata$5>:
 	...
 
-000000029a1b93c0 <__imp___tzname>:
-   29a1b93c0:	xchg   %eax,%esp
+000000029a1b93c0 <__imp___daylight>:
+   29a1b93c0:	xchg   %eax,%edx
    29a1b93c1:	xchg   %eax,%esi
    29a1b93c2:	add    %al,(%rax)
    29a1b93c4:	add    %al,(%rax)
 	...
 
-000000029a1b93c8 <__imp__tzset>:
-   29a1b93c8:	movabs 0x96,%al
+000000029a1b93c8 <__imp___timezone>:
+   29a1b93c8:	movabs 0xae00000000000096,%al
 
-000000029a1b93d0 <.idata$5>:
-	...
-
-000000029a1b93d8 <__IAT_end__>:
-   29a1b93d8:	and    $0x6c654401,%eax
-   29a1b93dd:	gs je  29a1b9445 <.idata$6+0x11>
-   29a1b93e0:	rex.XB jb 29a1b944c <.idata$6>
-   29a1b93e3:	je     29a1b944e <.idata$6+0x2>
-   29a1b93e5:	movsxd 0x6c(%rcx),%esp
-   29a1b93e8:	push   %rbx
-   29a1b93e9:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   29a1b93ee:	outsb  %ds:(%rsi),(%dx)
-	...
-
-000000029a1b93f0 <.idata$6>:
-   29a1b93f0:	rex.WXB add %rax,0x6e(%r13)
-   29a1b93f4:	je     29a1b945b <.idata$6+0x7>
-   29a1b93f6:	jb     29a1b943b <.idata$6+0x7>
-   29a1b93f8:	jb     29a1b9463 <.idata$6+0x1>
-   29a1b93fa:	je     29a1b9465 <.idata$6+0x3>
-   29a1b93fc:	movsxd 0x6c(%rcx),%esp
-   29a1b93ff:	push   %rbx
-   29a1b9400:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   29a1b9405:	outsb  %ds:(%rsi),(%dx)
-	...
-
-000000029a1b9408 <.idata$6>:
-   29a1b9408:	test   %al,(%rdx)
-   29a1b940a:	rex.RXB
-   29a1b940b:	gs je  29a1b945a <.idata$6+0x6>
-   29a1b940e:	(bad)
-   29a1b940f:	jae    29a1b9485 <.idata$6+0x1>
-   29a1b9411:	rex.RB jb 29a1b9486 <.idata$6+0x2>
-   29a1b9414:	outsl  %ds:(%rsi),(%dx)
-   29a1b9415:	jb     29a1b9417 <.idata$6+0xf>
+000000029a1b93d0 <__imp___tzname>:
+   29a1b93d0:	scas   %es:(%rdi),%al
+   29a1b93d1:	xchg   %eax,%esi
+   29a1b93d2:	add    %al,(%rax)
+   29a1b93d4:	add    %al,(%rax)
+	...
+
+000000029a1b93d8 <__imp__tzset>:
+   29a1b93d8:	mov    $0x96,%edx
+   29a1b93dd:	add    %al,(%rax)
+	...
+
+000000029a1b93e0 <.idata$5>:
+	...
+
+000000029a1b93e8 <__IAT_end__>:
+   29a1b93e8:	and    $0x6c654401,%eax
+   29a1b93ed:	gs je  29a1b9455 <.idata$6+0x11>
+   29a1b93f0:	rex.XB jb 29a1b945c <.idata$6>
+   29a1b93f3:	je     29a1b945e <.idata$6+0x2>
+   29a1b93f5:	movsxd 0x6c(%rcx),%esp
+   29a1b93f8:	push   %rbx
+   29a1b93f9:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   29a1b93fe:	outsb  %ds:(%rsi),(%dx)
+	...
+
+000000029a1b9400 <.idata$6>:
+   29a1b9400:	rex.WXB add %rax,0x6e(%r13)
+   29a1b9404:	je     29a1b946b <.idata$6+0x7>
+   29a1b9406:	jb     29a1b944b <.idata$6+0x7>
+   29a1b9408:	jb     29a1b9473 <.idata$6+0x1>
+   29a1b940a:	je     29a1b9475 <.idata$6+0x3>
+   29a1b940c:	movsxd 0x6c(%rcx),%esp
+   29a1b940f:	push   %rbx
+   29a1b9410:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   29a1b9415:	outsb  %ds:(%rsi),(%dx)
 	...
 
 000000029a1b9418 <.idata$6>:
-   29a1b9418:	xchg   %eax,%edx
-   29a1b9419:	add    0x6e(%rcx),%ecx
-   29a1b941c:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
-   29a1b9424:	rex.XB jb 29a1b9490 <.idata$6+0x2>
-   29a1b9427:	je     29a1b9492 <.idata$6+0x4>
-   29a1b9429:	movsxd 0x6c(%rcx),%esp
-   29a1b942c:	push   %rbx
-   29a1b942d:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   29a1b9432:	outsb  %ds:(%rsi),(%dx)
-	...
-
-000000029a1b9434 <.idata$6>:
-   29a1b9434:	lock add 0x61(%rbp,%riz,2),%ecx
-   29a1b9439:	jbe    29a1b94a0 <.idata$6+0x2>
-   29a1b943b:	rex.XB jb 29a1b94a7 <.idata$6+0x9>
-   29a1b943e:	je     29a1b94a9 <.idata$6+0xb>
-   29a1b9440:	movsxd 0x6c(%rcx),%esp
-   29a1b9443:	push   %rbx
-   29a1b9444:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   29a1b9449:	outsb  %ds:(%rsi),(%dx)
-	...
-
-000000029a1b944c <.idata$6>:
-   29a1b944c:	movsb  %ds:(%rsi),%es:(%rdi)
-   29a1b944d:	add    $0x65656c53,%eax
-   29a1b9452:	jo     29a1b9454 <.idata$6>
-
-000000029a1b9454 <.idata$6>:
-   29a1b9454:	enter  $0x5405,$0x6c
-   29a1b9458:	jae    29a1b94a1 <.idata$6+0x3>
-   29a1b945a:	gs je  29a1b94b3 <.idata$6+0x5>
-   29a1b945d:	(bad)
-   29a1b945e:	insb   (%dx),%es:(%rdi)
-   29a1b945f:	jne    29a1b94c6 <.idata$6+0x8>
-	...
-
-000000029a1b9462 <.idata$6>:
-   29a1b9462:	testl  $0x506c6175,0x74726956(%rip)        # 30e8dfdc2 <.debug_rnglists+0x7470fd1e>
-   29a1b946c:	jb     29a1b94dd <.idata$6+0xd>
-   29a1b946e:	je     29a1b94d5 <.idata$6+0x5>
-   29a1b9470:	movsxd 0x0(%rax,%rax,1),%esi
-
-000000029a1b9474 <.idata$6>:
-   29a1b9474:	stc
-   29a1b9475:	add    $0x74726956,%eax
-   29a1b947a:	jne    29a1b94dd <.idata$6+0xd>
-   29a1b947c:	insb   (%dx),%es:(%rdi)
-   29a1b947d:	push   %rcx
-   29a1b947e:	jne    29a1b94e5 <.idata$6+0x7>
-   29a1b9480:	jb     29a1b94fb <.idata$6+0x1>
-	...
+   29a1b9418:	test   %al,(%rdx)
+   29a1b941a:	rex.RXB
+   29a1b941b:	gs je  29a1b946a <.idata$6+0x6>
+   29a1b941e:	(bad)
+   29a1b941f:	jae    29a1b9495 <.idata$6+0x1>
+   29a1b9421:	rex.RB jb 29a1b9496 <.idata$6+0x2>
+   29a1b9424:	outsl  %ds:(%rsi),(%dx)
+   29a1b9425:	jb     29a1b9427 <.idata$6+0xf>
+	...
+
+000000029a1b9428 <.idata$6>:
+   29a1b9428:	xchg   %eax,%edx
+   29a1b9429:	add    0x6e(%rcx),%ecx
+   29a1b942c:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   29a1b9434:	rex.XB jb 29a1b94a0 <.idata$6+0x2>
+   29a1b9437:	je     29a1b94a2 <.idata$6+0x4>
+   29a1b9439:	movsxd 0x6c(%rcx),%esp
+   29a1b943c:	push   %rbx
+   29a1b943d:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   29a1b9442:	outsb  %ds:(%rsi),(%dx)
+	...
+
+000000029a1b9444 <.idata$6>:
+   29a1b9444:	lock add 0x61(%rbp,%riz,2),%ecx
+   29a1b9449:	jbe    29a1b94b0 <.idata$6+0x2>
+   29a1b944b:	rex.XB jb 29a1b94b7 <.idata$6+0x9>
+   29a1b944e:	je     29a1b94b9 <.idata$6+0xb>
+   29a1b9450:	movsxd 0x6c(%rcx),%esp
+   29a1b9453:	push   %rbx
+   29a1b9454:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   29a1b9459:	outsb  %ds:(%rsi),(%dx)
+	...
+
+000000029a1b945c <.idata$6>:
+   29a1b945c:	movsb  %ds:(%rsi),%es:(%rdi)
+   29a1b945d:	add    $0x65656c53,%eax
+   29a1b9462:	jo     29a1b9464 <.idata$6>
+
+000000029a1b9464 <.idata$6>:
+   29a1b9464:	enter  $0x5405,$0x6c
+   29a1b9468:	jae    29a1b94b1 <.idata$6+0x3>
+   29a1b946a:	gs je  29a1b94c3 <.idata$6+0x5>
+   29a1b946d:	(bad)
+   29a1b946e:	insb   (%dx),%es:(%rdi)
+   29a1b946f:	jne    29a1b94d6 <.idata$6+0x8>
+	...
+
+000000029a1b9472 <.idata$6>:
+   29a1b9472:	testl  $0x506c6175,0x74726956(%rip)        # 30e8dfdd2 <.debug_rnglists+0x7470fd2e>
+   29a1b947c:	jb     29a1b94ed <.idata$6+0xd>
+   29a1b947e:	je     29a1b94e5 <.idata$6+0x5>
+   29a1b9480:	movsxd 0x0(%rax,%rax,1),%esi
 
 000000029a1b9484 <.idata$6>:
-   29a1b9484:	ltr    0x67(%rdi)
-   29a1b9488:	gs je  29a1b94ee <.idata$6+0x2>
-   29a1b948b:	push   $0x10000
-
-000000029a1b948e <.idata$6>:
-   29a1b948e:	add    %eax,(%rax)
-   29a1b9490:	pop    %rdi
-   29a1b9491:	pop    %rdi
-   29a1b9492:	jo     29a1b94f3 <.idata$6+0x7>
-   29a1b9494:	pop    %rdi
-   29a1b9495:	outsb  %gs:(%rsi),(%dx)
-   29a1b9497:	jbe    29a1b9502 <.idata$6+0x8>
-   29a1b9499:	jb     29a1b950a <.idata$6+0x10>
-   29a1b949b:	outsb  %ds:(%rsi),(%dx)
+   29a1b9484:	stc
+   29a1b9485:	add    $0x74726956,%eax
+   29a1b948a:	jne    29a1b94ed <.idata$6+0xd>
+   29a1b948c:	insb   (%dx),%es:(%rdi)
+   29a1b948d:	push   %rcx
+   29a1b948e:	jne    29a1b94f5 <.idata$6+0x7>
+   29a1b9490:	jb     29a1b950b <.idata$6+0x1>
 	...
 
+000000029a1b9494 <.idata$6>:
+   29a1b9494:	ltr    0x67(%rdi)
+   29a1b9498:	gs je  29a1b94fe <.idata$6+0x2>
+   29a1b949b:	push   $0x10000
+
 000000029a1b949e <.idata$6>:
-   29a1b949e:	add    (%rax),%al
+   29a1b949e:	add    %eax,(%rax)
    29a1b94a0:	pop    %rdi
    29a1b94a1:	pop    %rdi
-   29a1b94a2:	jo     29a1b9503 <.idata$6+0x9>
+   29a1b94a2:	jo     29a1b9503 <.idata$6+0x7>
    29a1b94a4:	pop    %rdi
-   29a1b94a5:	ja     29a1b950c <.idata$6+0x12>
-   29a1b94a7:	outsb  %ds:(%rsi),(%dx)
-   29a1b94a8:	jbe    29a1b9513 <.idata$6+0x19>
-   29a1b94aa:	jb     29a1b951b <.idata$6+0x7>
-   29a1b94ac:	outsb  %ds:(%rsi),(%dx)
+   29a1b94a5:	outsb  %gs:(%rsi),(%dx)
+   29a1b94a7:	jbe    29a1b9512 <.idata$6+0x8>
+   29a1b94a9:	jb     29a1b951a <.idata$6+0x10>
+   29a1b94ab:	outsb  %ds:(%rsi),(%dx)
 	...
 
 000000029a1b94ae <.idata$6>:
-   29a1b94ae:	sbb    %al,(%rax)
+   29a1b94ae:	add    (%rax),%al
    29a1b94b0:	pop    %rdi
-   29a1b94b1:	jae    29a1b9518 <.idata$6+0x4>
-   29a1b94b3:	je     29a1b9514 <.idata$6>
-   29a1b94b5:	outsb  %ds:(%rsi),(%dx)
-   29a1b94b6:	gs ja  29a1b9518 <.idata$6+0x4>
-   29a1b94b9:	insl   (%dx),%es:(%rdi)
-   29a1b94ba:	outsl  %ds:(%rsi),(%dx)
-   29a1b94bb:	fs add %bl,%gs:(%rcx)
+   29a1b94b1:	pop    %rdi
+   29a1b94b2:	jo     29a1b9513 <.idata$6+0x9>
+   29a1b94b4:	pop    %rdi
+   29a1b94b5:	ja     29a1b951c <.idata$6+0x12>
+   29a1b94b7:	outsb  %ds:(%rsi),(%dx)
+   29a1b94b8:	jbe    29a1b9523 <.idata$6+0x19>
+   29a1b94ba:	jb     29a1b952b <.idata$6+0x7>
+   29a1b94bc:	outsb  %ds:(%rsi),(%dx)
+	...
 
 000000029a1b94be <.idata$6>:
-   29a1b94be:	sbb    %eax,(%rax)
-   29a1b94c0:	movsxd 0x6c(%rcx),%esp
-   29a1b94c3:	insb   (%dx),%es:(%rdi)
-   29a1b94c4:	outsl  %ds:(%rsi),(%dx)
-   29a1b94c5:	movsxd (%rax),%eax
-	...
-
-000000029a1b94c8 <.idata$6>:
-   29a1b94c8:	sbb    (%rax),%al
-   29a1b94ca:	data16 jb 29a1b9532 <.idata$6+0x6>
-   29a1b94cd:	add    %al,%gs:(%rax)
-
-000000029a1b94d0 <.idata$6>:
-   29a1b94d0:	add    $0x705f5f00,%eax
-   29a1b94d5:	pop    %rdi
-   29a1b94d6:	pop    %rdi
-   29a1b94d7:	pop    %rdi
-   29a1b94d8:	(bad)
-   29a1b94d9:	jb     29a1b9542 <.idata$6>
-   29a1b94db:	movsxd (%rax),%eax
-	...
-
-000000029a1b94de <.idata$6>:
-   29a1b94de:	(bad)
-   29a1b94df:	add    %bl,0x5f(%rdi)
-   29a1b94e2:	jo     29a1b9543 <.idata$6+0x1>
-   29a1b94e4:	pop    %rdi
-   29a1b94e5:	pop    %rdi
-   29a1b94e6:	(bad)
-   29a1b94e7:	jb     29a1b9550 <.idata$6>
-   29a1b94e9:	jbe    29a1b94eb <.idata$6+0xd>
-	...
-
-000000029a1b94ec <.idata$6>:
-   29a1b94ec:	(bad)
-   29a1b94ed:	add    %bl,0x5f(%rdi)
-   29a1b94f0:	jo     29a1b9551 <.idata$6+0x1>
-   29a1b94f2:	pop    %rdi
-   29a1b94f3:	pop    %rdi
-   29a1b94f4:	ja     29a1b9557 <.idata$6+0x7>
-   29a1b94f6:	jb     29a1b955f <.idata$6+0xf>
-   29a1b94f8:	jbe    29a1b94fa <.idata$6>
-
-000000029a1b94fa <.idata$6>:
-   29a1b94fa:	sbb    %eax,(%rax)
-   29a1b94fc:	pop    %rdi
-   29a1b94fd:	movsxd 0x6e(%rdi),%ebp
-   29a1b9500:	imul   $0x6572,0x75(%rdi),%sp
-   29a1b9506:	pop    %rdi
-   29a1b9507:	outsb  %ds:(%rsi),(%dx)
-   29a1b9508:	(bad)
-   29a1b9509:	jb     29a1b957d <.idata$6+0xd>
-   29a1b950b:	outsl  %ds:(%rsi),(%dx)
-   29a1b950c:	ja     29a1b956d <.idata$6+0x5>
-   29a1b950e:	(bad)
-   29a1b950f:	jb     29a1b9578 <.idata$6+0x8>
-   29a1b9511:	jbe    29a1b9513 <.idata$6+0x19>
-	...
+   29a1b94be:	sbb    %al,(%rax)
+   29a1b94c0:	pop    %rdi
+   29a1b94c1:	jae    29a1b9528 <.idata$6+0x4>
+   29a1b94c3:	je     29a1b9524 <.idata$6>
+   29a1b94c5:	outsb  %ds:(%rsi),(%dx)
+   29a1b94c6:	gs ja  29a1b9528 <.idata$6+0x4>
+   29a1b94c9:	insl   (%dx),%es:(%rdi)
+   29a1b94ca:	outsl  %ds:(%rsi),(%dx)
+   29a1b94cb:	fs add %bl,%gs:(%rcx)
+
+000000029a1b94ce <.idata$6>:
+   29a1b94ce:	sbb    %eax,(%rax)
+   29a1b94d0:	movsxd 0x6c(%rcx),%esp
+   29a1b94d3:	insb   (%dx),%es:(%rdi)
+   29a1b94d4:	outsl  %ds:(%rsi),(%dx)
+   29a1b94d5:	movsxd (%rax),%eax
+	...
+
+000000029a1b94d8 <.idata$6>:
+   29a1b94d8:	sbb    (%rax),%al
+   29a1b94da:	data16 jb 29a1b9542 <.idata$6+0x6>
+   29a1b94dd:	add    %al,%gs:(%rax)
 
-000000029a1b9514 <.idata$6>:
-   29a1b9514:	sbb    (%rax),%al
+000000029a1b94e0 <.idata$6>:
+   29a1b94e0:	add    $0x705f5f00,%eax
+   29a1b94e5:	pop    %rdi
+   29a1b94e6:	pop    %rdi
+   29a1b94e7:	pop    %rdi
+   29a1b94e8:	(bad)
+   29a1b94e9:	jb     29a1b9552 <.idata$6>
+   29a1b94eb:	movsxd (%rax),%eax
+	...
+
+000000029a1b94ee <.idata$6>:
+   29a1b94ee:	(bad)
+   29a1b94ef:	add    %bl,0x5f(%rdi)
+   29a1b94f2:	jo     29a1b9553 <.idata$6+0x1>
+   29a1b94f4:	pop    %rdi
+   29a1b94f5:	pop    %rdi
+   29a1b94f6:	(bad)
+   29a1b94f7:	jb     29a1b9560 <.idata$6>
+   29a1b94f9:	jbe    29a1b94fb <.idata$6+0xd>
+	...
+
+000000029a1b94fc <.idata$6>:
+   29a1b94fc:	(bad)
+   29a1b94fd:	add    %bl,0x5f(%rdi)
+   29a1b9500:	jo     29a1b9561 <.idata$6+0x1>
+   29a1b9502:	pop    %rdi
+   29a1b9503:	pop    %rdi
+   29a1b9504:	ja     29a1b9567 <.idata$6+0x7>
+   29a1b9506:	jb     29a1b956f <.idata$6+0xf>
+   29a1b9508:	jbe    29a1b950a <.idata$6>
+
+000000029a1b950a <.idata$6>:
+   29a1b950a:	sbb    %eax,(%rax)
+   29a1b950c:	pop    %rdi
+   29a1b950d:	movsxd 0x6e(%rdi),%ebp
+   29a1b9510:	imul   $0x6572,0x75(%rdi),%sp
    29a1b9516:	pop    %rdi
-   29a1b9517:	movsxd 0x6e(%rdi),%ebp
-   29a1b951a:	imul   $0x6572,0x75(%rdi),%sp
-   29a1b9520:	pop    %rdi
-   29a1b9521:	ja     29a1b958c <.idata$6+0x1c>
-   29a1b9523:	fs gs pop %rdi
-   29a1b9526:	(bad)
-   29a1b9527:	jb     29a1b9590 <.idata$6+0x20>
-   29a1b9529:	jbe    29a1b952b <.idata$6+0x17>
-	...
-
-000000029a1b952c <.idata$6>:
-   29a1b952c:	(bad)
-   29a1b952d:	add    %bl,0x63(%rdi)
-   29a1b9530:	jb     29a1b95a6 <.idata$6+0x14>
-   29a1b9532:	pop    %rdi
-   29a1b9533:	(bad)
-   29a1b9534:	je     29a1b9595 <.idata$6+0x3>
-   29a1b9536:	jno    29a1b95ad <.idata$6+0x1b>
-   29a1b9538:	imul   $0x6978655f,0x6b(%rbx),%esp
-   29a1b953f:	je     29a1b9541 <.idata$6+0x15>
-	...
-
-000000029a1b9542 <.idata$6>:
-   29a1b9542:	(bad)
-   29a1b9543:	add    %bl,0x63(%rdi)
-   29a1b9546:	jb     29a1b95bc <.idata$6+0xe>
-   29a1b9548:	pop    %rdi
-   29a1b9549:	(bad)
-   29a1b954a:	je     29a1b95b1 <.idata$6+0x3>
-   29a1b954c:	js     29a1b95b7 <.idata$6+0x9>
-   29a1b954e:	je     29a1b9550 <.idata$6>
-
-000000029a1b9550 <.idata$6>:
-   29a1b9550:	and    $0x0,%al
-   29a1b9552:	pop    %rdi
-   29a1b9553:	gs js  29a1b95bb <.idata$6+0xd>
-   29a1b9556:	movsxd 0x74(%rbp),%esi
-   29a1b9559:	gs pop %rdi
-   29a1b955b:	outsl  %ds:(%rsi),(%dx)
-   29a1b955c:	outsb  %ds:(%rsi),(%dx)
-   29a1b955d:	gs js  29a1b95c9 <.idata$6+0x1b>
-   29a1b9560:	je     29a1b95c1 <.idata$6+0x13>
-   29a1b9562:	je     29a1b95c5 <.idata$6+0x17>
-   29a1b9564:	(bad)
-	...
-
-000000029a1b9568 <.idata$6>:
-   29a1b9568:	and    $0x78655f00,%eax
-   29a1b956d:	imul   $0x6e695f00,0x36(%rax,%rax,1),%esi
-
-000000029a1b9570 <.idata$6>:
-   29a1b9570:	ss add %bl,0x69(%rdi)
-   29a1b9574:	outsb  %ds:(%rsi),(%dx)
-   29a1b9575:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
-   29a1b957d:	pop    %rdi
-   29a1b957e:	outsb  %ds:(%rsi),(%dx)
-   29a1b957f:	(bad)
-   29a1b9580:	jb     29a1b95f4 <.idata$6+0x1a>
-   29a1b9582:	outsl  %ds:(%rsi),(%dx)
-   29a1b9583:	ja     29a1b95e4 <.idata$6+0xa>
-   29a1b9585:	outsb  %gs:(%rsi),(%dx)
-   29a1b9587:	jbe    29a1b95f2 <.idata$6+0x18>
-   29a1b9589:	jb     29a1b95fa <.idata$6+0x4>
-   29a1b958b:	outsb  %ds:(%rsi),(%dx)
-   29a1b958c:	insl   (%dx),%es:(%rdi)
-   29a1b958d:	outsb  %gs:(%rsi),(%dx)
-   29a1b958f:	je     29a1b9591 <.idata$6+0x21>
-	...
-
-000000029a1b9592 <.idata$6>:
-   29a1b9592:	(bad)
-   29a1b9593:	add    %bl,0x69(%rdi)
-   29a1b9596:	outsb  %ds:(%rsi),(%dx)
-   29a1b9597:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
-   29a1b959f:	pop    %rdi
-   29a1b95a0:	outsl  %ds:(%rsi),(%dx)
-   29a1b95a1:	outsb  %ds:(%rsi),(%dx)
-   29a1b95a2:	gs js  29a1b960e <.idata$6+0x10>
-   29a1b95a5:	je     29a1b9606 <.idata$6+0x8>
-   29a1b95a7:	je     29a1b960a <.idata$6+0xc>
-   29a1b95a9:	(bad)
-	...
-
-000000029a1b95ae <.idata$6>:
-   29a1b95ae:	cmp    %al,(%rax)
-   29a1b95b0:	pop    %rdi
-   29a1b95b1:	imul   $0x6c616974,0x69(%rsi),%ebp
-   29a1b95b8:	imul   $0x6469775f,0x65(%rdx),%edi
-   29a1b95bf:	gs pop %rdi
-   29a1b95c1:	outsb  %gs:(%rsi),(%dx)
-   29a1b95c3:	jbe    29a1b962e <.idata$6+0x4>
-   29a1b95c5:	jb     29a1b9636 <.idata$6+0xc>
-   29a1b95c7:	outsb  %ds:(%rsi),(%dx)
-   29a1b95c8:	insl   (%dx),%es:(%rdi)
-   29a1b95c9:	outsb  %gs:(%rsi),(%dx)
-   29a1b95cb:	je     29a1b95cd <.idata$6+0x1f>
-	...
-
-000000029a1b95ce <.idata$6>:
-   29a1b95ce:	cmp    %eax,(%rax)
-   29a1b95d0:	pop    %rdi
-   29a1b95d1:	imul   $0x72657474,0x69(%rsi),%ebp
+   29a1b9517:	outsb  %ds:(%rsi),(%dx)
+   29a1b9518:	(bad)
+   29a1b9519:	jb     29a1b958d <.idata$6+0xd>
+   29a1b951b:	outsl  %ds:(%rsi),(%dx)
+   29a1b951c:	ja     29a1b957d <.idata$6+0x5>
+   29a1b951e:	(bad)
+   29a1b951f:	jb     29a1b9588 <.idata$6+0x8>
+   29a1b9521:	jbe    29a1b9523 <.idata$6+0x19>
+	...
+
+000000029a1b9524 <.idata$6>:
+   29a1b9524:	sbb    (%rax),%al
+   29a1b9526:	pop    %rdi
+   29a1b9527:	movsxd 0x6e(%rdi),%ebp
+   29a1b952a:	imul   $0x6572,0x75(%rdi),%sp
+   29a1b9530:	pop    %rdi
+   29a1b9531:	ja     29a1b959c <.idata$6+0x1c>
+   29a1b9533:	fs gs pop %rdi
+   29a1b9536:	(bad)
+   29a1b9537:	jb     29a1b95a0 <.idata$6+0x20>
+   29a1b9539:	jbe    29a1b953b <.idata$6+0x17>
+	...
+
+000000029a1b953c <.idata$6>:
+   29a1b953c:	(bad)
+   29a1b953d:	add    %bl,0x63(%rdi)
+   29a1b9540:	jb     29a1b95b6 <.idata$6+0x14>
+   29a1b9542:	pop    %rdi
+   29a1b9543:	(bad)
+   29a1b9544:	je     29a1b95a5 <.idata$6+0x3>
+   29a1b9546:	jno    29a1b95bd <.idata$6+0x1b>
+   29a1b9548:	imul   $0x6978655f,0x6b(%rbx),%esp
+   29a1b954f:	je     29a1b9551 <.idata$6+0x15>
+	...
+
+000000029a1b9552 <.idata$6>:
+   29a1b9552:	(bad)
+   29a1b9553:	add    %bl,0x63(%rdi)
+   29a1b9556:	jb     29a1b95cc <.idata$6+0xe>
+   29a1b9558:	pop    %rdi
+   29a1b9559:	(bad)
+   29a1b955a:	je     29a1b95c1 <.idata$6+0x3>
+   29a1b955c:	js     29a1b95c7 <.idata$6+0x9>
+   29a1b955e:	je     29a1b9560 <.idata$6>
+
+000000029a1b9560 <.idata$6>:
+   29a1b9560:	and    $0x0,%al
+   29a1b9562:	pop    %rdi
+   29a1b9563:	gs js  29a1b95cb <.idata$6+0xd>
+   29a1b9566:	movsxd 0x74(%rbp),%esi
+   29a1b9569:	gs pop %rdi
+   29a1b956b:	outsl  %ds:(%rsi),(%dx)
+   29a1b956c:	outsb  %ds:(%rsi),(%dx)
+   29a1b956d:	gs js  29a1b95d9 <.idata$6+0x1b>
+   29a1b9570:	je     29a1b95d1 <.idata$6+0x13>
+   29a1b9572:	je     29a1b95d5 <.idata$6+0x17>
+   29a1b9574:	(bad)
+	...
+
+000000029a1b9578 <.idata$6>:
+   29a1b9578:	and    $0x78655f00,%eax
+   29a1b957d:	imul   $0x6e695f00,0x36(%rax,%rax,1),%esi
+
+000000029a1b9580 <.idata$6>:
+   29a1b9580:	ss add %bl,0x69(%rdi)
+   29a1b9584:	outsb  %ds:(%rsi),(%dx)
+   29a1b9585:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   29a1b958d:	pop    %rdi
+   29a1b958e:	outsb  %ds:(%rsi),(%dx)
+   29a1b958f:	(bad)
+   29a1b9590:	jb     29a1b9604 <.idata$6+0x1a>
+   29a1b9592:	outsl  %ds:(%rsi),(%dx)
+   29a1b9593:	ja     29a1b95f4 <.idata$6+0xa>
+   29a1b9595:	outsb  %gs:(%rsi),(%dx)
+   29a1b9597:	jbe    29a1b9602 <.idata$6+0x18>
+   29a1b9599:	jb     29a1b960a <.idata$6+0x4>
+   29a1b959b:	outsb  %ds:(%rsi),(%dx)
+   29a1b959c:	insl   (%dx),%es:(%rdi)
+   29a1b959d:	outsb  %gs:(%rsi),(%dx)
+   29a1b959f:	je     29a1b95a1 <.idata$6+0x21>
+	...
+
+000000029a1b95a2 <.idata$6>:
+   29a1b95a2:	(bad)
+   29a1b95a3:	add    %bl,0x69(%rdi)
+   29a1b95a6:	outsb  %ds:(%rsi),(%dx)
+   29a1b95a7:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   29a1b95af:	pop    %rdi
+   29a1b95b0:	outsl  %ds:(%rsi),(%dx)
+   29a1b95b1:	outsb  %ds:(%rsi),(%dx)
+   29a1b95b2:	gs js  29a1b961e <.idata$6+0x10>
+   29a1b95b5:	je     29a1b9616 <.idata$6+0x8>
+   29a1b95b7:	je     29a1b961a <.idata$6+0xc>
+   29a1b95b9:	(bad)
+	...
+
+000000029a1b95be <.idata$6>:
+   29a1b95be:	cmp    %al,(%rax)
+   29a1b95c0:	pop    %rdi
+   29a1b95c1:	imul   $0x6c616974,0x69(%rsi),%ebp
+   29a1b95c8:	imul   $0x6469775f,0x65(%rdx),%edi
+   29a1b95cf:	gs pop %rdi
+   29a1b95d1:	outsb  %gs:(%rsi),(%dx)
+   29a1b95d3:	jbe    29a1b963e <.idata$6+0x4>
+   29a1b95d5:	jb     29a1b9646 <.idata$6+0xc>
+   29a1b95d7:	outsb  %ds:(%rsi),(%dx)
    29a1b95d8:	insl   (%dx),%es:(%rdi)
+   29a1b95d9:	outsb  %gs:(%rsi),(%dx)
+   29a1b95db:	je     29a1b95dd <.idata$6+0x1f>
 	...
 
-000000029a1b95da <.idata$6>:
-   29a1b95da:	(bad)
-   29a1b95db:	add    %bl,0x72(%rdi)
-   29a1b95de:	imul   $0x6f5f7265,%gs:0x74(%ebx),%esi
-   29a1b95e7:	outsb  %ds:(%rsi),(%dx)
-   29a1b95e8:	gs js  29a1b9654 <.idata$6+0x4>
-   29a1b95eb:	je     29a1b964c <.idata$6+0x6>
-   29a1b95ed:	data16 jne 29a1b965e <.idata$6+0x4>
-   29a1b95f0:	movsxd 0x6f(%rcx,%rbp,2),%esi
-   29a1b95f4:	outsb  %ds:(%rsi),(%dx)
-	...
-
-000000029a1b95f6 <.idata$6>:
-   29a1b95f6:	pop    %rax
-   29a1b95f7:	add    %ah,0x62(%rcx)
-   29a1b95fa:	outsl  %ds:(%rsi),(%dx)
-   29a1b95fb:	jb     29a1b9671 <.idata$6+0x3>
-	...
-
-000000029a1b95fe <.idata$6>:
-   29a1b95fe:	add    %eax,(%rax)
-   29a1b9600:	pop    %rdi
-   29a1b9601:	pop    %rdi
-   29a1b9602:	(bad)
-   29a1b9603:	movsxd 0x74(%rdx),%esi
-   29a1b9606:	pop    %rdi
-   29a1b9607:	imul   $0x6e75665f,0x62(%rdi),%ebp
-   29a1b960e:	movsxd (%rax),%eax
-
-000000029a1b9610 <.idata$6>:
-   29a1b9610:	add    $0x0,%al
-   29a1b9612:	pop    %rdi
-   29a1b9613:	pop    %rdi
-   29a1b9614:	jae    29a1b968a <.idata$6+0x4>
-   29a1b9616:	imul   $0x6d6d6f63,%fs:0x5f(%rdi),%ebp
-   29a1b961e:	outsl  %ds:(%rsi),(%dx)
-   29a1b961f:	outsb  %ds:(%rsi),(%dx)
-   29a1b9620:	pop    %rdi
-   29a1b9621:	jbe    29a1b9689 <.idata$6+0x3>
-   29a1b9623:	jo     29a1b9697 <.idata$6+0x3>
-   29a1b9625:	imul   $0x80066,0x74(%rsi),%ebp
-
-000000029a1b962a <.idata$6>:
-   29a1b962a:	or     %al,(%rax)
-   29a1b962c:	pop    %rdi
-   29a1b962d:	pop    %rdi
-   29a1b962e:	jae    29a1b96a4 <.idata$6+0x4>
-   29a1b9630:	imul   $0x6d6d6f63,%fs:0x5f(%rdi),%ebp
-   29a1b9638:	outsl  %ds:(%rsi),(%dx)
-   29a1b9639:	outsb  %ds:(%rsi),(%dx)
-   29a1b963a:	pop    %rdi
-   29a1b963b:	jbe    29a1b96a3 <.idata$6+0x3>
-   29a1b963d:	ja     29a1b96af <.idata$7+0x3>
-   29a1b963f:	jb     29a1b96aa <.idata$6+0xa>
-   29a1b9641:	outsb  %ds:(%rsi),(%dx)
-   29a1b9642:	je     29a1b96aa <.idata$6+0xa>
-	...
-
-000000029a1b9646 <.idata$6>:
-   29a1b9646:	push   %rsp
-   29a1b9647:	add    %bl,0x6b(%rdi)
-   29a1b964a:	(bad)
-   29a1b964b:	push   $0x7469
-
-000000029a1b9650 <.idata$6>:
-   29a1b9650:	test   $0x72776600,%eax
-   29a1b9655:	imul   $0x7000b100,0x0(%rbp,%riz,2),%esi
-
-000000029a1b965a <.idata$6>:
-   29a1b965a:	mov    $0x0,%cl
-   29a1b965c:	jo     29a1b96d3 <__lib64_libkernel32_a_iname+0x3>
-   29a1b965e:	je     29a1b96c3 <.idata$7+0x3>
-   29a1b9660:	push   $0xffffffffa8007261
-
-000000029a1b9664 <.idata$6>:
-   29a1b9664:	test   $0x0,%al
-   29a1b9666:	jae    29a1b96dc <__lib64_libkernel32_a_iname+0xc>
-   29a1b9668:	jb     29a1b96d6 <__lib64_libkernel32_a_iname+0x6>
-   29a1b966a:	outsb  %gs:(%rsi),(%dx)
-	...
-
-000000029a1b966e <.idata$6>:
-   29a1b966e:	stos   %eax,%es:(%rdi)
-   29a1b966f:	add    %dh,0x74(%rbx)
-   29a1b9672:	jb     29a1b96e2 <.idata$7+0x2>
-   29a1b9674:	movsxd 0x70(%rbp),%ebp
-	...
-
-000000029a1b9678 <.idata$6>:
-   29a1b9678:	or     %eax,(%rax)
-   29a1b967a:	pop    %rdi
-   29a1b967b:	pop    %rdi
-   29a1b967c:	fs (bad)
-   29a1b967e:	jns    29a1b96ec <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0x8>
-   29a1b9680:	imul   $0xb000074,0x68(%rdi),%esp
-
-000000029a1b9686 <.idata$6>:
-   29a1b9686:	or     (%rax),%eax
-   29a1b9688:	pop    %rdi
-   29a1b9689:	pop    %rdi
-   29a1b968a:	je     29a1b96f5 <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0x11>
-   29a1b968c:	insl   (%dx),%es:(%rdi)
-   29a1b968d:	gs jp  29a1b96ff <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0x1b>
-   29a1b9690:	outsb  %ds:(%rsi),(%dx)
-   29a1b9691:	add    %al,%gs:(%rax)
-
-000000029a1b9694 <.idata$6>:
-   29a1b9694:	or     $0x0,%al
-   29a1b9696:	pop    %rdi
-   29a1b9697:	pop    %rdi
-   29a1b9698:	je     29a1b9714 <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname+0x8>
-   29a1b969a:	outsb  %ds:(%rsi),(%dx)
-   29a1b969b:	(bad)
-   29a1b969c:	insl   (%dx),%es:(%rdi)
-   29a1b969d:	add    %al,%gs:(%rax)
+000000029a1b95de <.idata$6>:
+   29a1b95de:	cmp    %eax,(%rax)
+   29a1b95e0:	pop    %rdi
+   29a1b95e1:	imul   $0x72657474,0x69(%rsi),%ebp
+   29a1b95e8:	insl   (%dx),%es:(%rdi)
+	...
+
+000000029a1b95ea <.idata$6>:
+   29a1b95ea:	(bad)
+   29a1b95eb:	add    %bl,0x72(%rdi)
+   29a1b95ee:	imul   $0x6f5f7265,%gs:0x74(%ebx),%esi
+   29a1b95f7:	outsb  %ds:(%rsi),(%dx)
+   29a1b95f8:	gs js  29a1b9664 <.idata$6+0x4>
+   29a1b95fb:	je     29a1b965c <.idata$6+0x6>
+   29a1b95fd:	data16 jne 29a1b966e <.idata$6+0x4>
+   29a1b9600:	movsxd 0x6f(%rcx,%rbp,2),%esi
+   29a1b9604:	outsb  %ds:(%rsi),(%dx)
+	...
+
+000000029a1b9606 <.idata$6>:
+   29a1b9606:	pop    %rax
+   29a1b9607:	add    %ah,0x62(%rcx)
+   29a1b960a:	outsl  %ds:(%rsi),(%dx)
+   29a1b960b:	jb     29a1b9681 <.idata$6+0x3>
+	...
+
+000000029a1b960e <.idata$6>:
+   29a1b960e:	add    %eax,(%rax)
+   29a1b9610:	pop    %rdi
+   29a1b9611:	pop    %rdi
+   29a1b9612:	(bad)
+   29a1b9613:	movsxd 0x74(%rdx),%esi
+   29a1b9616:	pop    %rdi
+   29a1b9617:	imul   $0x6e75665f,0x62(%rdi),%ebp
+   29a1b961e:	movsxd (%rax),%eax
+
+000000029a1b9620 <.idata$6>:
+   29a1b9620:	add    $0x0,%al
+   29a1b9622:	pop    %rdi
+   29a1b9623:	pop    %rdi
+   29a1b9624:	jae    29a1b969a <.idata$6+0x8>
+   29a1b9626:	imul   $0x6d6d6f63,%fs:0x5f(%rdi),%ebp
+   29a1b962e:	outsl  %ds:(%rsi),(%dx)
+   29a1b962f:	outsb  %ds:(%rsi),(%dx)
+   29a1b9630:	pop    %rdi
+   29a1b9631:	jbe    29a1b9699 <.idata$6+0x7>
+   29a1b9633:	jo     29a1b96a7 <.idata$6+0x7>
+   29a1b9635:	imul   $0x80066,0x74(%rsi),%ebp
+
+000000029a1b963a <.idata$6>:
+   29a1b963a:	or     %al,(%rax)
+   29a1b963c:	pop    %rdi
+   29a1b963d:	pop    %rdi
+   29a1b963e:	jae    29a1b96b4 <.idata$6+0x6>
+   29a1b9640:	imul   $0x6d6d6f63,%fs:0x5f(%rdi),%ebp
+   29a1b9648:	outsl  %ds:(%rsi),(%dx)
+   29a1b9649:	outsb  %ds:(%rsi),(%dx)
+   29a1b964a:	pop    %rdi
+   29a1b964b:	jbe    29a1b96b3 <.idata$6+0x5>
+   29a1b964d:	ja     29a1b96bf <.idata$6+0x5>
+   29a1b964f:	jb     29a1b96ba <.idata$6>
+   29a1b9651:	outsb  %ds:(%rsi),(%dx)
+   29a1b9652:	je     29a1b96ba <.idata$6>
+	...
+
+000000029a1b9656 <.idata$6>:
+   29a1b9656:	push   %rsp
+   29a1b9657:	add    %bl,0x6b(%rdi)
+   29a1b965a:	(bad)
+   29a1b965b:	push   $0x7469
+
+000000029a1b9660 <.idata$6>:
+   29a1b9660:	xchg   %eax,%esi
+   29a1b9661:	add    %ah,0x66(%rsi)
+   29a1b9664:	insb   (%dx),%es:(%rdi)
+   29a1b9665:	jne    29a1b96da <.idata$7+0x2>
+   29a1b9667:	push   $0xa90000
+
+000000029a1b966a <.idata$6>:
+   29a1b966a:	test   $0x72776600,%eax
+   29a1b966f:	imul   $0x7000b100,0x0(%rbp,%riz,2),%esi
+
+000000029a1b9674 <.idata$6>:
+   29a1b9674:	mov    $0x0,%cl
+   29a1b9676:	jo     29a1b96ed <__lib64_libkernel32_a_iname+0x5>
+   29a1b9678:	je     29a1b96dd <.idata$7+0x1>
+   29a1b967a:	push   $0xffffffffa8007261
+
+000000029a1b967e <.idata$6>:
+   29a1b967e:	test   $0x0,%al
+   29a1b9680:	jae    29a1b96f6 <__lib64_libkernel32_a_iname+0xe>
+   29a1b9682:	jb     29a1b96f0 <__lib64_libkernel32_a_iname+0x8>
+   29a1b9684:	outsb  %gs:(%rsi),(%dx)
+	...
+
+000000029a1b9688 <.idata$6>:
+   29a1b9688:	stos   %eax,%es:(%rdi)
+   29a1b9689:	add    %dh,0x74(%rbx)
+   29a1b968c:	jb     29a1b96fc <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname>
+   29a1b968e:	movsxd 0x70(%rbp),%ebp
+	...
+
+000000029a1b9692 <.idata$6>:
+   29a1b9692:	or     %eax,(%rax)
+   29a1b9694:	pop    %rdi
+   29a1b9695:	pop    %rdi
+   29a1b9696:	fs (bad)
+   29a1b9698:	jns    29a1b9706 <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0xa>
+   29a1b969a:	imul   $0xb000074,0x68(%rdi),%esp
 
 000000029a1b96a0 <.idata$6>:
-   29a1b96a0:	cmp    $0x0,%al
+   29a1b96a0:	or     (%rax),%eax
    29a1b96a2:	pop    %rdi
-   29a1b96a3:	je     29a1b971f <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname+0x13>
-   29a1b96a5:	jae    29a1b970c <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname>
-   29a1b96a7:	je     29a1b96a9 <.idata$6+0x9>
-   29a1b96a9:	add    %al,(%rax)
+   29a1b96a3:	pop    %rdi
+   29a1b96a4:	je     29a1b970f <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0x13>
+   29a1b96a6:	insl   (%dx),%es:(%rdi)
+   29a1b96a7:	gs jp  29a1b9719 <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0x1d>
+   29a1b96aa:	outsb  %ds:(%rsi),(%dx)
+   29a1b96ab:	add    %al,%gs:(%rax)
+
+000000029a1b96ae <.idata$6>:
+   29a1b96ae:	or     $0x0,%al
+   29a1b96b0:	pop    %rdi
+   29a1b96b1:	pop    %rdi
+   29a1b96b2:	je     29a1b972e <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname+0xa>
+   29a1b96b4:	outsb  %ds:(%rsi),(%dx)
+   29a1b96b5:	(bad)
+   29a1b96b6:	insl   (%dx),%es:(%rdi)
+   29a1b96b7:	add    %al,%gs:(%rax)
+
+000000029a1b96ba <.idata$6>:
+   29a1b96ba:	cmp    $0x0,%al
+   29a1b96bc:	pop    %rdi
+   29a1b96bd:	je     29a1b9739 <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname+0x15>
+   29a1b96bf:	jae    29a1b9726 <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname+0x2>
+   29a1b96c1:	je     29a1b96c3 <.idata$6+0x9>
 	...
 
-000000029a1b96ac <.idata$7>:
-   29a1b96ac:	add    %dl,-0x70000000(%rax)
-
-000000029a1b96b0 <.idata$7>:
-   29a1b96b0:	add    %dl,-0x70000000(%rax)
-
-000000029a1b96b4 <.idata$7>:
-   29a1b96b4:	add    %dl,-0x70000000(%rax)
-
-000000029a1b96b8 <.idata$7>:
-   29a1b96b8:	add    %dl,-0x70000000(%rax)
-
-000000029a1b96bc <.idata$7>:
-   29a1b96bc:	add    %dl,-0x70000000(%rax)
-
-000000029a1b96c0 <.idata$7>:
-   29a1b96c0:	add    %dl,-0x70000000(%rax)
-
 000000029a1b96c4 <.idata$7>:
    29a1b96c4:	add    %dl,-0x70000000(%rax)
 
 000000029a1b96c8 <.idata$7>:
    29a1b96c8:	add    %dl,-0x70000000(%rax)
 
 000000029a1b96cc <.idata$7>:
-   29a1b96cc:	add    %dl,0x454b0000(%rax)
-
-000000029a1b96d0 <__lib64_libkernel32_a_iname>:
-   29a1b96d0:	rex.WXB
-   29a1b96d1:	rex.RB push %r10
-   29a1b96d3:	rex.WRX
-   29a1b96d4:	rex.RB
-   29a1b96d5:	xor    (%rdx),%r14
-   29a1b96d8:	cs fs insb (%dx),%es:(%rdi)
-   29a1b96db:	insb   (%dx),%es:(%rdi)
-   29a1b96dc:	add    %al,(%rax)
-	...
-
-000000029a1b96e0 <.idata$7>:
-   29a1b96e0:	adc    $0x90,%al
-	...
-
-000000029a1b96e4 <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname>:
-   29a1b96e4:	(bad)
-   29a1b96e5:	jo     29a1b9750 <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname+0x10>
-   29a1b96e7:	sub    $0x772d736d,%eax
-   29a1b96ec:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b96f3:	movsxd 0x6e(%rdi),%ebp
-   29a1b96f6:	imul   $0x312d316c,0x2d(%rdi),%ebp
-   29a1b96fd:	sub    $0x6c642e30,%eax
-   29a1b9702:	insb   (%dx),%es:(%rdi)
-	...
-
-000000029a1b9704 <.idata$7>:
-   29a1b9704:	sub    %dl,-0x6fd80000(%rax)
-
-000000029a1b9708 <.idata$7>:
-   29a1b9708:	sub    %dl,0x70610000(%rax)
-
-000000029a1b970c <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname>:
-   29a1b970c:	(bad)
-   29a1b970d:	jo     29a1b9778 <.idata$7>
-   29a1b970f:	sub    $0x772d736d,%eax
-   29a1b9714:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b971b:	outsb  %gs:(%rsi),(%dx)
-   29a1b971d:	jbe    29a1b9788 <.idata$7>
-   29a1b971f:	jb     29a1b9790 <.idata$7>
-   29a1b9721:	outsb  %ds:(%rsi),(%dx)
-   29a1b9722:	insl   (%dx),%es:(%rdi)
-   29a1b9723:	outsb  %gs:(%rsi),(%dx)
-   29a1b9725:	je     29a1b9754 <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname+0x14>
-   29a1b9727:	insb   (%dx),%es:(%rdi)
-   29a1b9728:	xor    %ebp,0x2e302d31(%rip)        # 2c84bc45f <.debug_rnglists+0x2e2ec3bb>
-   29a1b972e:	fs insb (%dx),%es:(%rdi)
-   29a1b9730:	insb   (%dx),%es:(%rdi)
-   29a1b9731:	add    %al,(%rax)
-	...
+   29a1b96cc:	add    %dl,-0x70000000(%rax)
 
-000000029a1b9734 <.idata$7>:
-   29a1b9734:	cmp    $0x90,%al
-	...
+000000029a1b96d0 <.idata$7>:
+   29a1b96d0:	add    %dl,-0x70000000(%rax)
 
-000000029a1b9738 <.idata$7>:
-   29a1b9738:	cmp    $0x90,%al
-	...
+000000029a1b96d4 <.idata$7>:
+   29a1b96d4:	add    %dl,-0x70000000(%rax)
 
-000000029a1b973c <.idata$7>:
-   29a1b973c:	cmp    $0x90,%al
-	...
+000000029a1b96d8 <.idata$7>:
+   29a1b96d8:	add    %dl,-0x70000000(%rax)
 
-000000029a1b9740 <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname>:
-   29a1b9740:	(bad)
-   29a1b9741:	jo     29a1b97ac <__lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname+0x10>
-   29a1b9743:	sub    $0x772d736d,%eax
-   29a1b9748:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b974f:	push   $0x2d706165
-   29a1b9754:	insb   (%dx),%es:(%rdi)
-   29a1b9755:	xor    %ebp,0x2e302d31(%rip)        # 2c84bc48c <.debug_rnglists+0x2e2ec3e8>
-   29a1b975b:	fs insb (%dx),%es:(%rdi)
-   29a1b975d:	insb   (%dx),%es:(%rdi)
-	...
+000000029a1b96dc <.idata$7>:
+   29a1b96dc:	add    %dl,-0x70000000(%rax)
 
-000000029a1b9760 <.idata$7>:
-   29a1b9760:	push   %rax
-   29a1b9761:	nop
-	...
-
-000000029a1b9764 <.idata$7>:
-   29a1b9764:	push   %rax
-   29a1b9765:	nop
-	...
-
-000000029a1b9768 <.idata$7>:
-   29a1b9768:	push   %rax
-   29a1b9769:	nop
-	...
-
-000000029a1b976c <.idata$7>:
-   29a1b976c:	push   %rax
-   29a1b976d:	nop
-	...
+000000029a1b96e0 <.idata$7>:
+   29a1b96e0:	add    %dl,-0x70000000(%rax)
 
-000000029a1b9770 <.idata$7>:
-   29a1b9770:	push   %rax
-   29a1b9771:	nop
-	...
+000000029a1b96e4 <.idata$7>:
+   29a1b96e4:	add    %dl,0x454b0000(%rax)
 
-000000029a1b9774 <.idata$7>:
-   29a1b9774:	push   %rax
-   29a1b9775:	nop
+000000029a1b96e8 <__lib64_libkernel32_a_iname>:
+   29a1b96e8:	rex.WXB
+   29a1b96e9:	rex.RB push %r10
+   29a1b96eb:	rex.WRX
+   29a1b96ec:	rex.RB
+   29a1b96ed:	xor    (%rdx),%r14
+   29a1b96f0:	cs fs insb (%dx),%es:(%rdi)
+   29a1b96f3:	insb   (%dx),%es:(%rdi)
+   29a1b96f4:	add    %al,(%rax)
+	...
+
+000000029a1b96f8 <.idata$7>:
+   29a1b96f8:	adc    $0x90,%al
+	...
+
+000000029a1b96fc <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname>:
+   29a1b96fc:	(bad)
+   29a1b96fd:	jo     29a1b9768 <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname+0x10>
+   29a1b96ff:	sub    $0x772d736d,%eax
+   29a1b9704:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b970b:	movsxd 0x6e(%rdi),%ebp
+   29a1b970e:	imul   $0x312d316c,0x2d(%rdi),%ebp
+   29a1b9715:	sub    $0x6c642e30,%eax
+   29a1b971a:	insb   (%dx),%es:(%rdi)
+	...
+
+000000029a1b971c <.idata$7>:
+   29a1b971c:	sub    %dl,-0x6fd80000(%rax)
+
+000000029a1b9720 <.idata$7>:
+   29a1b9720:	sub    %dl,0x70610000(%rax)
+
+000000029a1b9724 <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname>:
+   29a1b9724:	(bad)
+   29a1b9725:	jo     29a1b9790 <.idata$7>
+   29a1b9727:	sub    $0x772d736d,%eax
+   29a1b972c:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b9733:	outsb  %gs:(%rsi),(%dx)
+   29a1b9735:	jbe    29a1b97a0 <.idata$7>
+   29a1b9737:	jb     29a1b97a8 <.idata$7>
+   29a1b9739:	outsb  %ds:(%rsi),(%dx)
+   29a1b973a:	insl   (%dx),%es:(%rdi)
+   29a1b973b:	outsb  %gs:(%rsi),(%dx)
+   29a1b973d:	je     29a1b976c <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname+0x14>
+   29a1b973f:	insb   (%dx),%es:(%rdi)
+   29a1b9740:	xor    %ebp,0x2e302d31(%rip)        # 2c84bc477 <.debug_rnglists+0x2e2ec3d3>
+   29a1b9746:	fs insb (%dx),%es:(%rdi)
+   29a1b9748:	insb   (%dx),%es:(%rdi)
+   29a1b9749:	add    %al,(%rax)
+	...
+
+000000029a1b974c <.idata$7>:
+   29a1b974c:	cmp    $0x90,%al
+	...
+
+000000029a1b9750 <.idata$7>:
+   29a1b9750:	cmp    $0x90,%al
+	...
+
+000000029a1b9754 <.idata$7>:
+   29a1b9754:	cmp    $0x90,%al
+	...
+
+000000029a1b9758 <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname>:
+   29a1b9758:	(bad)
+   29a1b9759:	jo     29a1b97c4 <__lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname+0x10>
+   29a1b975b:	sub    $0x772d736d,%eax
+   29a1b9760:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b9767:	push   $0x2d706165
+   29a1b976c:	insb   (%dx),%es:(%rdi)
+   29a1b976d:	xor    %ebp,0x2e302d31(%rip)        # 2c84bc4a4 <.debug_rnglists+0x2e2ec400>
+   29a1b9773:	fs insb (%dx),%es:(%rdi)
+   29a1b9775:	insb   (%dx),%es:(%rdi)
 	...
 
 000000029a1b9778 <.idata$7>:
    29a1b9778:	push   %rax
    29a1b9779:	nop
 	...
 
@@ -7098,108 +7108,142 @@
 	...
 
 000000029a1b9798 <.idata$7>:
    29a1b9798:	push   %rax
    29a1b9799:	nop
 	...
 
-000000029a1b979c <__lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname>:
-   29a1b979c:	(bad)
-   29a1b979d:	jo     29a1b9808 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x8>
-   29a1b979f:	sub    $0x772d736d,%eax
-   29a1b97a4:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b97ab:	jb     29a1b9822 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x22>
-   29a1b97ad:	outsb  %ds:(%rsi),(%dx)
-   29a1b97ae:	je     29a1b9819 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x19>
-   29a1b97b0:	insl   (%dx),%es:(%rdi)
-   29a1b97b1:	gs sub $0x312d316c,%eax
-   29a1b97b7:	sub    $0x6c642e30,%eax
-   29a1b97bc:	insb   (%dx),%es:(%rdi)
-   29a1b97bd:	add    %al,(%rax)
+000000029a1b979c <.idata$7>:
+   29a1b979c:	push   %rax
+   29a1b979d:	nop
 	...
 
-000000029a1b97c0 <.idata$7>:
-   29a1b97c0:	fs nop
+000000029a1b97a0 <.idata$7>:
+   29a1b97a0:	push   %rax
+   29a1b97a1:	nop
 	...
 
-000000029a1b97c4 <.idata$7>:
-   29a1b97c4:	fs nop
+000000029a1b97a4 <.idata$7>:
+   29a1b97a4:	push   %rax
+   29a1b97a5:	nop
 	...
 
-000000029a1b97c8 <.idata$7>:
-   29a1b97c8:	fs nop
+000000029a1b97a8 <.idata$7>:
+   29a1b97a8:	push   %rax
+   29a1b97a9:	nop
 	...
 
-000000029a1b97cc <.idata$7>:
-   29a1b97cc:	fs nop
+000000029a1b97ac <.idata$7>:
+   29a1b97ac:	push   %rax
+   29a1b97ad:	nop
 	...
 
-000000029a1b97d0 <.idata$7>:
-   29a1b97d0:	fs nop
+000000029a1b97b0 <.idata$7>:
+   29a1b97b0:	push   %rax
+   29a1b97b1:	nop
 	...
 
-000000029a1b97d4 <.idata$7>:
-   29a1b97d4:	fs nop
+000000029a1b97b4 <__lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname>:
+   29a1b97b4:	(bad)
+   29a1b97b5:	jo     29a1b9820 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x4>
+   29a1b97b7:	sub    $0x772d736d,%eax
+   29a1b97bc:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b97c3:	jb     29a1b983a <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x1e>
+   29a1b97c5:	outsb  %ds:(%rsi),(%dx)
+   29a1b97c6:	je     29a1b9831 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x15>
+   29a1b97c8:	insl   (%dx),%es:(%rdi)
+   29a1b97c9:	gs sub $0x312d316c,%eax
+   29a1b97cf:	sub    $0x6c642e30,%eax
+   29a1b97d4:	insb   (%dx),%es:(%rdi)
+   29a1b97d5:	add    %al,(%rax)
 	...
 
-000000029a1b97d8 <__lib64_libapi_ms_win_crt_stdio_l1_1_0_a_iname>:
-   29a1b97d8:	(bad)
-   29a1b97d9:	jo     29a1b9844 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x10>
-   29a1b97db:	sub    $0x772d736d,%eax
-   29a1b97e0:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b97e7:	jae    29a1b985d <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x29>
-   29a1b97e9:	imul   $0x312d316c,%fs:0x2d(%rdi),%ebp
-   29a1b97f1:	sub    $0x6c642e30,%eax
-   29a1b97f6:	insb   (%dx),%es:(%rdi)
+000000029a1b97d8 <.idata$7>:
+   29a1b97d8:	fs nop
 	...
 
-000000029a1b97f8 <.idata$7>:
-   29a1b97f8:	js     29a1b978a <.idata$7+0x2>
+000000029a1b97dc <.idata$7>:
+   29a1b97dc:	fs nop
 	...
 
-000000029a1b97fc <.idata$7>:
-   29a1b97fc:	js     29a1b978e <.idata$7+0x2>
+000000029a1b97e0 <.idata$7>:
+   29a1b97e0:	fs nop
 	...
 
-000000029a1b9800 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname>:
-   29a1b9800:	(bad)
-   29a1b9801:	jo     29a1b986c <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x38>
-   29a1b9803:	sub    $0x772d736d,%eax
-   29a1b9808:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b980f:	jae    29a1b9885 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x51>
-   29a1b9811:	jb     29a1b987c <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x48>
-   29a1b9813:	outsb  %ds:(%rsi),(%dx)
-   29a1b9814:	addr32 sub $0x312d316c,%eax
-   29a1b981a:	sub    $0x6c642e30,%eax
-   29a1b981f:	insb   (%dx),%es:(%rdi)
-   29a1b9820:	add    %al,(%rax)
+000000029a1b97e4 <.idata$7>:
+   29a1b97e4:	fs nop
 	...
 
-000000029a1b9824 <.idata$7>:
-   29a1b9824:	mov    %ss,-0x6f740000(%rax)
+000000029a1b97e8 <.idata$7>:
+   29a1b97e8:	fs nop
+	...
 
-000000029a1b9828 <.idata$7>:
-   29a1b9828:	mov    %ss,-0x6f740000(%rax)
+000000029a1b97ec <.idata$7>:
+   29a1b97ec:	fs nop
+	...
 
-000000029a1b982c <.idata$7>:
-   29a1b982c:	mov    %ss,-0x6f740000(%rax)
+000000029a1b97f0 <.idata$7>:
+   29a1b97f0:	fs nop
+	...
 
-000000029a1b9830 <.idata$7>:
-   29a1b9830:	mov    %ss,0x70610000(%rax)
+000000029a1b97f4 <__lib64_libapi_ms_win_crt_stdio_l1_1_0_a_iname>:
+   29a1b97f4:	(bad)
+   29a1b97f5:	jo     29a1b9860 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x10>
+   29a1b97f7:	sub    $0x772d736d,%eax
+   29a1b97fc:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b9803:	jae    29a1b9879 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x29>
+   29a1b9805:	imul   $0x312d316c,%fs:0x2d(%rdi),%ebp
+   29a1b980d:	sub    $0x6c642e30,%eax
+   29a1b9812:	insb   (%dx),%es:(%rdi)
+	...
 
-000000029a1b9834 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname>:
-   29a1b9834:	(bad)
-   29a1b9835:	jo     29a1b98a0 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x6c>
-   29a1b9837:	sub    $0x772d736d,%eax
-   29a1b983c:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b9843:	je     29a1b98ae <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x7a>
-   29a1b9845:	insl   (%dx),%es:(%rdi)
-   29a1b9846:	gs sub $0x312d316c,%eax
-   29a1b984c:	sub    $0x6c642e30,%eax
-   29a1b9851:	insb   (%dx),%es:(%rdi)
+000000029a1b9814 <.idata$7>:
+   29a1b9814:	js     29a1b97a6 <.idata$7+0x2>
+	...
+
+000000029a1b9818 <.idata$7>:
+   29a1b9818:	js     29a1b97aa <.idata$7+0x2>
+	...
+
+000000029a1b981c <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname>:
+   29a1b981c:	(bad)
+   29a1b981d:	jo     29a1b9888 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x38>
+   29a1b981f:	sub    $0x772d736d,%eax
+   29a1b9824:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b982b:	jae    29a1b98a1 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x51>
+   29a1b982d:	jb     29a1b9898 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x48>
+   29a1b982f:	outsb  %ds:(%rsi),(%dx)
+   29a1b9830:	addr32 sub $0x312d316c,%eax
+   29a1b9836:	sub    $0x6c642e30,%eax
+   29a1b983b:	insb   (%dx),%es:(%rdi)
+   29a1b983c:	add    %al,(%rax)
+	...
+
+000000029a1b9840 <.idata$7>:
+   29a1b9840:	mov    %ss,-0x6f740000(%rax)
+
+000000029a1b9844 <.idata$7>:
+   29a1b9844:	mov    %ss,-0x6f740000(%rax)
+
+000000029a1b9848 <.idata$7>:
+   29a1b9848:	mov    %ss,-0x6f740000(%rax)
+
+000000029a1b984c <.idata$7>:
+   29a1b984c:	mov    %ss,0x70610000(%rax)
+
+000000029a1b9850 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname>:
+   29a1b9850:	(bad)
+   29a1b9851:	jo     29a1b98bc <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x6c>
+   29a1b9853:	sub    $0x772d736d,%eax
+   29a1b9858:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b985f:	je     29a1b98ca <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x7a>
+   29a1b9861:	insl   (%dx),%es:(%rdi)
+   29a1b9862:	gs sub $0x312d316c,%eax
+   29a1b9868:	sub    $0x6c642e30,%eax
+   29a1b986d:	insb   (%dx),%es:(%rdi)
 	...
 
 Disassembly of section .CRT:
 
 000000029a1ba000 <___crt_xc_start__>:
 	...
 
@@ -7218,22 +7262,23 @@
 	...
 
 000000029a1ba028 <___crt_xi_end__>:
 	...
 
 000000029a1ba030 <__xl_c>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:105
-   29a1ba030:	rclb   $1,(%rbx,%rbx,1)
-   29a1ba033:	(bad)
-   29a1ba034:	add    (%rax),%al
+   29a1ba030:	add    %dl,0x29a1b(%rip)        # 29a1e3a51 <.debug_rnglists+0x139ad>
 	...
 
 000000029a1ba038 <__xl_d>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:171
-   29a1ba038:	movabs 0x29a1b14,%al
+   29a1ba038:	rclb   $1,(%rbx,%rbx,1)
+   29a1ba03b:	(bad)
+   29a1ba03c:	add    (%rax),%al
+	...
 
 000000029a1ba040 <__xl_z>:
 	...
 
 000000029a1ba048 <___crt_xp_end__>:
 	...
 
@@ -7251,18 +7296,15 @@
 Disassembly of section .reloc:
 
 000000029a1bc000 <.reloc>:
    29a1bc000:	add    %ah,(%rax)
    29a1bc002:	add    %al,(%rax)
    29a1bc004:	or     $0x0,%al
    29a1bc006:	add    %al,(%rax)
-   29a1bc008:	cwtl
-   29a1bc009:	movsl  %ds:(%rsi),%es:(%rdi)
-   29a1bc00a:	add    %al,(%rax)
-   29a1bc00c:	add    %dh,(%rax)
+   29a1bc008:	fsubs  0x30000000(%rbp)
    29a1bc00e:	add    %al,(%rax)
    29a1bc010:	sub    %al,(%rax)
    29a1bc012:	add    %al,(%rax)
    29a1bc014:	adc    %ah,-0x5faf5fc0(%rax)
    29a1bc01a:	pop    %rax
    29a1bc01b:	movabs 0xa078a070a068a060,%al
    29a1bc024:	andb   $0xa0,-0x5f6f5f78(%rax)
@@ -7304,16 +7346,18 @@
    29a1bd032:	add    %al,(%rax)
    29a1bd034:	add    (%rax),%al
    29a1bd036:	mov    $0x19,%ah
    29a1bd038:	add    %al,(%rax)
    29a1bd03a:	or     %al,(%rax)
    29a1bd03c:	add    %al,(%rax)
    29a1bd03e:	add    %al,(%rax)
-   29a1bd040:	rclb   $1,(%rbx)
-   29a1bd042:	sbb    0x2(%rdx),%ebx
+   29a1bd040:	add    %dl,(%rbx,%rbx,1)
+   29a1bd043:	(bad)
+   29a1bd044:	add    (%rax),%al
+   29a1bd046:	add    %al,(%rax)
    29a1bd048:	iret
 	...
 
 000000029a1bd060 <.debug_aranges>:
    29a1bd060:	sbb    $0x0,%al
    29a1bd062:	add    %al,(%rax)
    29a1bd064:	add    (%rax),%al
@@ -7325,15 +7369,19 @@
    29a1bd082:	add    %al,(%rax)
    29a1bd084:	add    (%rax),%al
    29a1bd086:	(bad)
    29a1bd087:	es add %al,(%rax)
    29a1bd08a:	or     %al,(%rax)
    29a1bd08c:	add    %al,(%rax)
    29a1bd08e:	add    %al,(%rax)
-   29a1bd090:	movabs 0xc3000000029a1b14,%al
+   29a1bd090:	rclb   $1,(%rbx,%rbx,1)
+   29a1bd093:	(bad)
+   29a1bd094:	add    (%rax),%al
+   29a1bd096:	add    %al,(%rax)
+   29a1bd098:	ret
 	...
 
 000000029a1bd0b0 <.debug_aranges>:
    29a1bd0b0:	sbb    $0x0,%al
    29a1bd0b2:	add    %al,(%rax)
    29a1bd0b4:	add    (%rax),%al
    29a1bd0b6:	fisubrs 0x80000(%rip)        # 29a23d0bc <.debug_rnglists+0x6d018>
@@ -7354,28 +7402,27 @@
    29a1bd0f2:	add    %al,(%rax)
    29a1bd0f4:	add    (%rax),%al
    29a1bd0f6:	jmp    29a1bd127 <.debug_aranges+0x7>
    29a1bd0f8:	add    %al,(%rax)
    29a1bd0fa:	or     %al,(%rax)
    29a1bd0fc:	add    %al,(%rax)
    29a1bd0fe:	add    %al,(%rax)
-   29a1bd100:	jo     29a1bd117 <.debug_aranges+0x27>
-   29a1bd102:	sbb    0x2(%rdx),%ebx
-   29a1bd108:	cmp    $0x5,%eax
+   29a1bd100:	movabs 0x3d000000029a1b15,%al
+   29a1bd109:	add    $0x0,%eax
 	...
 
 000000029a1bd120 <.debug_aranges>:
    29a1bd120:	sub    $0x0,%al
    29a1bd122:	add    %al,(%rax)
    29a1bd124:	add    (%rax),%al
    29a1bd126:	ss rex.RXB add %r8b,(%r8)
    29a1bd12a:	or     %al,(%rax)
    29a1bd12c:	add    %al,(%rax)
    29a1bd12e:	add    %al,(%rax)
-   29a1bd130:	mov    $0x1a,%al
+   29a1bd130:	loopne 29a1bd14c <.debug_aranges+0x2c>
    29a1bd132:	sbb    0x2(%rdx),%ebx
    29a1bd138:	(bad)
 	...
 
 000000029a1bd150 <.debug_aranges>:
    29a1bd150:	sbb    $0x0,%al
    29a1bd152:	add    %al,(%rax)
@@ -7397,97 +7444,101 @@
 000000029a1bd190 <.debug_aranges>:
    29a1bd190:	sub    $0x0,%al
    29a1bd192:	add    %al,(%rax)
    29a1bd194:	add    (%rax),%al
    29a1bd196:	(bad)
    29a1bd19b:	add    %al,(%rax)
    29a1bd19d:	add    %al,(%rax)
-   29a1bd19f:	add    %ah,(%rax)
-   29a1bd1a1:	sbb    $0x29a1b,%eax
-   29a1bd1a6:	add    %al,(%rax)
+   29a1bd19f:	add    %dl,0x1d(%rax)
+   29a1bd1a2:	sbb    0x2(%rdx),%ebx
    29a1bd1a8:	testb  $0x0,(%rbx)
 	...
 
 000000029a1bd1c0 <.debug_aranges>:
    29a1bd1c0:	sub    $0x0,%al
    29a1bd1c2:	add    %al,(%rax)
    29a1bd1c4:	add    (%rax),%al
    29a1bd1c6:	xor    $0x68,%al
    29a1bd1c8:	add    %al,(%rax)
    29a1bd1ca:	or     %al,(%rax)
    29a1bd1cc:	add    %al,(%rax)
    29a1bd1ce:	add    %al,(%rax)
-   29a1bd1d0:	and    %ah,(%rcx)
-   29a1bd1d2:	sbb    0x2(%rdx),%ebx
+   29a1bd1d0:	push   %rax
+   29a1bd1d1:	and    %ebx,(%rbx)
+   29a1bd1d3:	(bad)
+   29a1bd1d4:	add    (%rax),%al
+   29a1bd1d6:	add    %al,(%rax)
    29a1bd1d8:	add    (%rax),%eax
 	...
 
 000000029a1bd1f0 <.debug_aranges>:
    29a1bd1f0:	sub    $0x0,%al
    29a1bd1f2:	add    %al,(%rax)
    29a1bd1f4:	add    (%rax),%al
    29a1bd1f6:	lret
    29a1bd1f7:	push   $0x80000
    29a1bd1fc:	add    %al,(%rax)
    29a1bd1fe:	add    %al,(%rax)
-   29a1bd200:	jo     29a1bd223 <.debug_aranges+0x3>
-   29a1bd202:	sbb    0x2(%rdx),%ebx
-   29a1bd208:	(bad)
+   29a1bd200:	movabs 0x6000000029a1b21,%al
 	...
 
 000000029a1bd220 <.debug_aranges>:
    29a1bd220:	sub    $0x0,%al
    29a1bd222:	add    %al,(%rax)
    29a1bd224:	add    (%rax),%al
    29a1bd226:	(bad)
    29a1bd229:	add    %cl,(%rax)
    29a1bd22b:	add    %al,(%rax)
    29a1bd22d:	add    %al,(%rax)
-   29a1bd22f:	add    %al,0x29a1b21(%rax)
+   29a1bd22f:	add    %dh,0x29a1b21(%rax)
    29a1bd235:	add    %al,(%rax)
    29a1bd237:	add    %al,(%rsi)
 	...
 
 000000029a1bd250 <.debug_aranges>:
    29a1bd250:	sub    $0x0,%al
    29a1bd252:	add    %al,(%rax)
    29a1bd254:	add    (%rax),%al
    29a1bd256:	mov    $0x800006c,%ecx
    29a1bd25b:	add    %al,(%rax)
    29a1bd25d:	add    %al,(%rax)
-   29a1bd25f:	add    %dl,0x29a1b21(%rax)
-   29a1bd265:	add    %al,(%rax)
-   29a1bd267:	add    %bl,(%rsi)
+   29a1bd25f:	add    %al,%al
+   29a1bd261:	and    %ebx,(%rbx)
+   29a1bd263:	(bad)
+   29a1bd264:	add    (%rax),%al
+   29a1bd266:	add    %al,(%rax)
+   29a1bd268:	(bad)
 	...
 
 000000029a1bd280 <.debug_aranges>:
    29a1bd280:	sub    $0x0,%al
    29a1bd282:	add    %al,(%rax)
    29a1bd284:	add    (%rax),%al
    29a1bd286:	push   %rsi
    29a1bd287:	jo     29a1bd289 <.debug_aranges+0x9>
    29a1bd289:	add    %cl,(%rax)
    29a1bd28b:	add    %al,(%rax)
    29a1bd28d:	add    %al,(%rax)
-   29a1bd28f:	add    %dh,0x29a1b21(%rax)
-   29a1bd295:	add    %al,(%rax)
-   29a1bd297:	add    %dl,(%rsi)
+   29a1bd28f:	add    %ah,%al
+   29a1bd291:	and    %ebx,(%rbx)
+   29a1bd293:	(bad)
+   29a1bd294:	add    (%rax),%al
+   29a1bd296:	add    %al,(%rax)
+   29a1bd298:	(bad)
    29a1bd299:	add    (%rax),%al
 	...
 
 000000029a1bd2b0 <.debug_aranges>:
    29a1bd2b0:	sub    $0x0,%al
    29a1bd2b2:	add    %al,(%rax)
    29a1bd2b4:	add    (%rax),%al
    29a1bd2b6:	fildl  0x80000(%rcx)
    29a1bd2bc:	add    %al,(%rax)
    29a1bd2be:	add    %al,(%rax)
-   29a1bd2c0:	lock and $0x1b,%al
-   29a1bd2c3:	(bad)
-   29a1bd2c4:	add    (%rax),%al
+   29a1bd2c0:	xor    %ah,0x29a1b(%rip)        # 29a1e6ce1 <.debug_rnglists+0x16c3d>
    29a1bd2c6:	add    %al,(%rax)
    29a1bd2c8:	xor    (%rax),%al
 	...
 
 Disassembly of section .debug_info:
 
 000000029a1be000 <.debug_info>:
@@ -10484,16 +10535,16 @@
    29a1bfa01:	xor    (%rax),%ah
    29a1bfa03:	sub    $0x3d647473,%eax
    29a1bfa08:	outsb  %ds:(%esi),(%dx)
    29a1bfa0a:	jne    29a1bfa45 <.debug_info+0x91>
    29a1bfa0c:	cmp    %eax,(%rax)
    29a1bfa0e:	or     $0xa2,%al
    29a1bfa10:	add    %eax,(%rax)
-   29a1bfa12:	add    %cl,-0x2fffffff(%rdx)
-   29a1bfa18:	adc    (%rbx),%ebx
+   29a1bfa12:	add    %cl,0x1(%rdx)
+   29a1bfa18:	adc    $0x1b,%al
    29a1bfa1a:	(bad)
    29a1bfa1b:	add    (%rax),%al
    29a1bfa1d:	add    %al,(%rax)
    29a1bfa1f:	iret
    29a1bfa20:	add    %al,(%rax)
    29a1bfa22:	add    %al,(%rax)
    29a1bfa24:	add    %al,(%rax)
@@ -11236,40 +11287,46 @@
    29a1bff2c:	add    %al,(%rax)
    29a1bff2e:	test   %al,0x59110000(%rip)        # 2f32cff34 <.debug_rnglists+0x590ffe90>
    29a1bff34:	add    %eax,(%rax)
    29a1bff36:	add    %al,(%rax)
    29a1bff38:	adc    0x5f(%rdi),%bl
    29a1bff3b:	insl   (%dx),%es:(%rdi)
    29a1bff3c:	(bad)
-   29a1bff3d:	imul   $0x80013501,0x0(%rsi),%ebp
+   29a1bff3d:	imul   $0xb0013501,0x0(%rsi),%ebp
    29a1bff44:	adc    $0x1b,%al
    29a1bff46:	(bad)
    29a1bff47:	add    (%rax),%al
    29a1bff49:	add    %al,(%rax)
    29a1bff4b:	(bad)
    29a1bff4c:	add    %al,(%rax)
    29a1bff4e:	add    %al,(%rax)
    29a1bff50:	add    %al,(%rax)
    29a1bff52:	add    %al,(%rcx)
    29a1bff54:	pushf
    29a1bff55:	mov    $0x5,%bl
    29a1bff57:	add    %al,(%rax)
-   29a1bff59:	adc    0x29a1b14(%rdi),%ebx
-   29a1bff5f:	add    %al,(%rax)
-   29a1bff61:	add    %dh,0x5(%rbx)
-   29a1bff67:	or     %ebx,0x5f(%rdi)
+   29a1bff59:	adc    %edi,%ecx
+   29a1bff5b:	adc    $0x1b,%al
+   29a1bff5d:	(bad)
+   29a1bff5e:	add    (%rax),%al
+   29a1bff60:	add    %al,(%rax)
+   29a1bff62:	mov    $0x5,%bl
+   29a1bff64:	add    %al,(%rax)
+   29a1bff66:	add    %cl,(%rcx)
+   29a1bff68:	pop    %rdi
+   29a1bff69:	pop    %rdi
    29a1bff6a:	outsl  %fs:(%rsi),(%dx)
    29a1bff6c:	pop    %rdi
    29a1bff6d:	insb   (%dx),%es:(%edi)
    29a1bff6f:	outsl  %ds:(%rsi),(%dx)
    29a1bff70:	(bad)
    29a1bff75:	je     29a1bffe6 <.debug_info+0x632>
    29a1bff77:	jb     29a1bffec <.debug_info+0x638>
    29a1bff79:	add    %ah,(%rax)
-   29a1bff7b:	adc    %dl,(%rbx,%rbx,1)
+   29a1bff7b:	rex adc $0x1b,%al
    29a1bff7e:	(bad)
    29a1bff7f:	add    (%rax),%al
    29a1bff81:	add    %al,(%rax)
    29a1bff83:	push   $0x0
    29a1bff85:	add    %al,(%rax)
    29a1bff87:	add    %al,(%rax)
    29a1bff89:	add    %al,(%rax)
@@ -11285,32 +11342,34 @@
    29a1bffa1:	add    (%r8),%eax
    29a1bffa4:	add    %cl,(%rdx)
    29a1bffa6:	imul   $0xf523,(%rax),%eax
    29a1bffac:	add    %bl,0x3(%rdi)
    29a1bffaf:	add    %al,(%rax)
    29a1bffb1:	pop    %rbx
    29a1bffb2:	add    (%rax),%eax
-   29a1bffb4:	add    %dl,0x29a1b14(,%rbx,2)
+   29a1bffb4:	add    %dl,0x29a1b14(,%rcx,4)
    29a1bffbb:	add    %al,(%rax)
    29a1bffbd:	add    %ch,0x5(%rdx)
    29a1bffc0:	add    %al,(%rax)
    29a1bffc2:	adc    $0x3095201,%eax
-   29a1bffc7:	rclb   $1,(%rbx)
-   29a1bffc9:	sbb    0x2(%rdx),%ebx
+   29a1bffc7:	add    %dl,(%rbx,%rbx,1)
+   29a1bffca:	(bad)
+   29a1bffcb:	add    (%rax),%al
+   29a1bffcd:	add    %al,(%rax)
    29a1bffcf:	add    %al,(%rax)
    29a1bffd1:	or     %ebx,0x5f(%rdi)
    29a1bffd4:	outsl  %fs:(%rsi),(%dx)
    29a1bffd6:	pop    %rdi
    29a1bffd7:	insb   (%dx),%es:(%edi)
    29a1bffd9:	outsl  %ds:(%rsi),(%dx)
    29a1bffda:	(bad)
    29a1bffdf:	je     29a1c0050 <.debug_info+0x3b>
    29a1bffe1:	jb     29a1c0056 <.debug_info+0x41>
-   29a1bffe3:	add    %dl,(%rax,%rdx,8)
-   29a1bffe6:	adc    (%rbx),%ebx
+   29a1bffe3:	add    %dl,(%rax,%rax,1)
+   29a1bffe6:	adc    $0x1b,%al
    29a1bffe8:	(bad)
    29a1bffe9:	add    (%rax),%al
    29a1bffeb:	add    %al,(%rax)
    29a1bffed:	cmp    (%rax),%al
    29a1bffef:	add    %al,(%rax)
    29a1bfff1:	add    %al,(%rax)
    29a1bfff3:	add    %al,(%rax)
@@ -12196,15 +12255,15 @@
    29a1c0664:	xor    (%rax),%ah
    29a1c0666:	sub    $0x3d647473,%eax
    29a1c066b:	outsb  %ds:(%esi),(%dx)
    29a1c066d:	jne    29a1c06a8 <.debug_info+0x91>
    29a1c066f:	cmp    %eax,(%rax)
    29a1c0671:	or     $0x98,%al
    29a1c0673:	add    (%rax),%eax
-   29a1c0675:	add    %al,-0x5ffffffd(%rax)
+   29a1c0675:	add    %al,-0x2ffffffd(%rax)
    29a1c067b:	adc    $0x1b,%al
    29a1c067d:	(bad)
    29a1c067e:	add    (%rax),%al
    29a1c0680:	add    %al,(%rax)
    29a1c0682:	ret
    29a1c0683:	add    %al,(%rax)
    29a1c0685:	add    %al,(%rax)
@@ -12864,17 +12923,20 @@
    29a1c0c26:	fs jns 29a1c0c97 <.debug_info+0x680>
    29a1c0c29:	pop    %rdi
    29a1c0c2a:	je     29a1c0c98 <.debug_info+0x681>
    29a1c0c2c:	jae    29a1c0c8d <.debug_info+0x676>
    29a1c0c2e:	fs je  29a1c0ca0 <.debug_info+0x689>
    29a1c0c31:	jb     29a1c0c33 <.debug_info+0x61c>
    29a1c0c33:	add    %ecx,0x14001(%rcx)
-   29a1c0c39:	add    %ah,0x29a1b14(%rax)
-   29a1c0c3f:	add    %al,(%rax)
-   29a1c0c41:	add    %ch,(%rdi)
+   29a1c0c39:	add    %dl,%al
+   29a1c0c3b:	adc    $0x1b,%al
+   29a1c0c3d:	(bad)
+   29a1c0c3e:	add    (%rax),%al
+   29a1c0c40:	add    %al,(%rax)
+   29a1c0c42:	(bad)
    29a1c0c43:	add    %al,(%rax)
    29a1c0c45:	add    %al,(%rax)
    29a1c0c47:	add    %al,(%rax)
    29a1c0c49:	add    %al,(%rcx)
    29a1c0c4b:	pushf
    29a1c0c4c:	jge    29a1c0c54 <.debug_info+0x63d>
    29a1c0c4e:	add    %al,(%rax)
@@ -12894,29 +12956,30 @@
    29a1c0c72:	add    %al,(%rax)
    29a1c0c74:	or     0x0(%rax,%rax,1),%dh
    29a1c0c78:	add    %bh,(%rbx)
    29a1c0c7a:	add    %eax,%fs:(%rax)
    29a1c0c7d:	add    %bl,-0x65fffffd(%rsi)
    29a1c0c83:	add    (%rax),%eax
    29a1c0c85:	add    %cl,(%rsi)
-   29a1c0c87:	(bad)
+   29a1c0c87:	cmc
+   29a1c0c88:	adc    $0x1b,%al
    29a1c0c8a:	(bad)
    29a1c0c8b:	add    (%rax),%al
    29a1c0c8d:	add    %al,(%rax)
    29a1c0c8f:	faddl  0x1b000000(%rip)        # 2b51c0c95 <.debug_rnglists+0x1aff0bf1>
    29a1c0c95:	pop    %rdi
    29a1c0c96:	pop    %rdi
    29a1c0c97:	je     29a1c0d05 <.debug_info+0x6ee>
    29a1c0c99:	jb     29a1c0d00 <.debug_info+0x6e9>
    29a1c0c9b:	addr32 fs je 29a1c0d0e <.debug_info+0x6f7>
    29a1c0c9f:	jb     29a1c0ca1 <.debug_info+0x68a>
    29a1c0ca1:	add    %ebp,0x1(%rsi)
    29a1c0ca4:	rolb   %cl,(%rax)
    29a1c0ca6:	add    %al,(%rax)
-   29a1c0ca8:	(bad)
+   29a1c0ca8:	nop
    29a1c0ca9:	adc    $0x29a1b,%eax
    29a1c0cae:	add    %al,(%rax)
    29a1c0cb0:	add    (%rax),%eax
    29a1c0cb2:	add    %al,(%rax)
    29a1c0cb4:	add    %al,(%rax)
    29a1c0cb6:	add    %al,(%rax)
    29a1c0cb8:	add    %ebx,0x1c000006(%rdi,%rsi,4)
@@ -12955,17 +13018,15 @@
    29a1c0d0f:	rex.WRXB or (%r12,%r8,1),%r12b
    29a1c0d13:	add    %al,(%rax)
    29a1c0d15:	pshufw $0x50,0x0(%rbx),%mm6
    29a1c0d1a:	or     $0xaa,%eax
    29a1c0d1f:	add    %bl,(%rsi)
    29a1c0d21:	mov    $0x6,%bh
    29a1c0d23:	add    %al,(%rax)
-   29a1c0d25:	rclb   $1,(%rbx,%rbx,1)
-   29a1c0d28:	(bad)
-   29a1c0d29:	add    (%rax),%al
+   29a1c0d25:	add    %dl,0x29a1b(%rip)        # 29a1ea746 <.debug_rnglists+0x1a6a2>
    29a1c0d2b:	add    %al,(%rax)
    29a1c0d2d:	addl   $0x0,(%rax)
    29a1c0d33:	add    %al,(%rax)
    29a1c0d35:	add    %ebx,0x6d3(%rdi,%rax,1)
    29a1c0d3c:	mov    $0x3,%ah
    29a1c0d3e:	add    %al,(%rax)
    29a1c0d40:	lods   %ds:(%rsi),%al
@@ -12990,17 +13051,17 @@
    29a1c0d61:	add    %al,(%rax)
    29a1c0d63:	adc    %bh,%dh
    29a1c0d65:	(bad)
    29a1c0d66:	add    %al,(%rax)
    29a1c0d68:	(bad)
    29a1c0d69:	mov    $0x6,%bh
    29a1c0d6b:	add    %al,(%rax)
-   29a1c0d6d:	add    %dl,0x29a1b(%rip)        # 29a1ea78e <.debug_rnglists+0x1a6ea>
+   29a1c0d6d:	xor    %dl,0x29a1b(%rip)        # 29a1ea78e <.debug_rnglists+0x1a6ea>
    29a1c0d73:	add    %al,(%rax)
-   29a1c0d75:	add    %al,(%rax)
+   29a1c0d75:	add    %dh,(%rax)
    29a1c0d77:	adc    $0x29a1b,%eax
    29a1c0d7c:	add    %al,(%rax)
    29a1c0d7e:	sub    (%rax),%eax
    29a1c0d80:	add    %al,(%rax)
    29a1c0d82:	add    %al,(%rax)
    29a1c0d84:	add    %al,(%rax)
    29a1c0d86:	add    %ecx,0x1(%rbp)
@@ -13032,16 +13093,16 @@
    29a1c0dc2:	incb   (%rsi)
    29a1c0dc4:	add    %al,(%rax)
    29a1c0dc6:	insb   (%dx),%es:(%rdi)
    29a1c0dc7:	add    $0x0,%al
    29a1c0dc9:	add    %ch,0x4(%rax)
    29a1c0dcc:	add    %al,(%rax)
    29a1c0dce:	add    %cl,(%rsi)
-   29a1c0dd0:	rex.RB adc $0x29a1b,%eax
-   29a1c0dd6:	add    %al,(%rax)
+   29a1c0dd0:	jne    29a1c0de7 <.debug_info+0x9>
+   29a1c0dd2:	sbb    0x2(%rdx),%ebx
    29a1c0dd8:	faddl  0x0(%rip)        # 29a1c0dde <.debug_info>
 
 000000029a1c0dde <.debug_info>:
    29a1c0dde:	ja     29a1c0de1 <.debug_info+0x3>
    29a1c0de0:	add    %al,(%rax)
    29a1c0de2:	add    $0x9b080100,%eax
    29a1c0de7:	or     %al,(%rax)
@@ -13274,19 +13335,21 @@
    29a1c103a:	sub    $0x3d647473,%eax
    29a1c103f:	outsb  %ds:(%esi),(%dx)
    29a1c1041:	jne    29a1c107c <.debug_info+0x91>
    29a1c1043:	cmp    %eax,(%rax)
    29a1c1045:	or     $0xbb,%al
    29a1c1047:	add    $0x5f10000,%eax
    29a1c104c:	add    %al,(%rax)
-   29a1c104e:	jo     29a1c1065 <.debug_info+0x7a>
-   29a1c1050:	sbb    0x2(%rdx),%ebx
-   29a1c1056:	cmp    $0x5,%eax
-   29a1c105b:	add    %al,(%rax)
-   29a1c105d:	add    %al,0x5f060000(%rsi,%rax,1)
+   29a1c104e:	movabs 0x3d000000029a1b15,%al
+   29a1c1057:	add    $0x0,%eax
+   29a1c105c:	add    %al,(%rax)
+   29a1c105e:	test   %al,(%rsi)
+   29a1c1060:	add    %al,(%rax)
+   29a1c1062:	(bad)
+   29a1c1063:	pop    %rdi
    29a1c1064:	pop    %rdi
    29a1c1065:	outsb  %ds:(%esi),(%dx)
    29a1c1067:	jne    29a1c10cc <.debug_info+0xe1>
    29a1c1069:	pop    %rdi
    29a1c106a:	jbe    29a1c10cd <.debug_info+0xe2>
    29a1c106c:	pop    %rdi
    29a1c106d:	insb   (%dx),%es:(%rdi)
@@ -14982,17 +15045,18 @@
    29a1c1e5d:	insb   (%dx),%es:(%rdi)
    29a1c1e5e:	outsl  %ds:(%rsi),(%dx)
    29a1c1e5f:	movsxd 0x74(%rcx),%esp
    29a1c1e62:	outsl  %ds:(%rsi),(%dx)
    29a1c1e63:	jb     29a1c1e65 <.debug_info+0xe7a>
    29a1c1e65:	add    %esp,%ebp
    29a1c1e67:	add    %eax,(%rcx)
-   29a1c1e69:	push   %rax
-   29a1c1e6a:	(bad)
-   29a1c1e6b:	sbb    0x2(%rdx),%ebx
+   29a1c1e69:	adcb   $0x1b,(%rdi)
+   29a1c1e6c:	(bad)
+   29a1c1e6d:	add    (%rax),%al
+   29a1c1e6f:	add    %al,(%rax)
    29a1c1e71:	pop    %rbp
    29a1c1e72:	add    (%rax),%eax
    29a1c1e74:	add    %al,(%rax)
    29a1c1e76:	add    %al,(%rax)
    29a1c1e78:	add    %al,(%rcx)
    29a1c1e7a:	pushf
    29a1c1e7b:	mov    (%rbx),%dl
@@ -15010,18 +15074,19 @@
    29a1c1ea2:	add    %ebp,%ecx
    29a1c1ea4:	add    %eax,(%rdi)
    29a1c1ea6:	and    $0x8f000001,%eax
    29a1c1eab:	add    $0x0,%al
    29a1c1ead:	add    %cl,0x21000004(%rbp)
    29a1c1eb3:	mov    (%rbx),%dl
    29a1c1eb5:	add    %al,(%rax)
-   29a1c1eb7:	{rex2 0x17} sbb 0x2(%r26),%r11d
-   29a1c1ebf:	add    0x0(%rdx),%al
-   29a1c1ec2:	add    %al,(%rax)
-   29a1c1ec4:	cmc
+   29a1c1eb7:	add    $0x29a1b18,%eax
+   29a1c1ebc:	add    %al,(%rax)
+   29a1c1ebe:	add    %al,(%rdx)
+   29a1c1ec0:	rex.X add %al,(%rax)
+   29a1c1ec3:	add    %dh,%ch
    29a1c1ec5:	add    %eax,(%rbx)
    29a1c1ec7:	xor    $0x13,%al
    29a1c1ec9:	add    %al,(%rax)
    29a1c1ecb:	sbb    0x1b000013(%rcx),%esp
    29a1c1ed1:	scas   %es:(%rdi),%eax
    29a1c1ed2:	adc    (%rax),%eax
    29a1c1ed4:	add    %bl,(%rbx)
@@ -15073,16 +15138,16 @@
    29a1c1f45:	add    %al,(%rax)
    29a1c1f47:	or     0x14(%rbx),%bl
    29a1c1f4a:	add    %al,(%rax)
    29a1c1f4c:	xchg   %eax,(%rdi)
    29a1c1f4e:	add    %al,(%rax)
    29a1c1f50:	jg     29a1c1f59 <.debug_info+0xf6e>
    29a1c1f52:	add    %al,(%rax)
-   29a1c1f54:	or     %ecx,%ebp
-   29a1c1f56:	sbb    %bl,(%rbx)
+   29a1c1f54:	or     (%rcx),%ebx
+   29a1c1f56:	sbb    %ebx,(%rbx)
    29a1c1f58:	(bad)
    29a1c1f59:	add    (%rax),%al
    29a1c1f5b:	add    %al,(%rax)
    29a1c1f5d:	(bad)
    29a1c1f5e:	(bad)
    29a1c1f5f:	add    %al,(%rax)
    29a1c1f61:	add    $0x1,%al
@@ -15094,18 +15159,22 @@
    29a1c1f70:	pop    %rax
    29a1c1f71:	add    0x0(%rbp),%dh
    29a1c1f74:	add    $0x2,%al
    29a1c1f76:	ja     29a1c1f98 <.debug_info+0xfad>
    29a1c1f78:	add    0x0(%rax,%rax,1),%dh
    29a1c1f7c:	add    %bl,(%rdi,%rdi,2)
    29a1c1f7f:	adc    $0x0,%al
-   29a1c1f81:	add    %dh,0x18(%rdi)
-   29a1c1f84:	sbb    0x2(%rdx),%ebx
-   29a1c1f8a:	add    0x18(%rdi),%dh
-   29a1c1f8d:	sbb    0x2(%rdx),%ebx
+   29a1c1f81:	add    %ah,0x29a1b18(%rdi)
+   29a1c1f87:	add    %al,(%rax)
+   29a1c1f89:	add    %al,(%rdx)
+   29a1c1f8b:	cmpsl  %es:(%rdi),%ds:(%rsi)
+   29a1c1f8c:	sbb    %bl,(%rbx)
+   29a1c1f8e:	(bad)
+   29a1c1f8f:	add    (%rax),%al
+   29a1c1f91:	add    %al,(%rax)
    29a1c1f93:	or     (%rax),%eax
    29a1c1f95:	add    %al,(%rax)
    29a1c1f97:	add    %al,(%rax)
    29a1c1f99:	add    %al,(%rax)
    29a1c1f9b:	{rex2 0x1} cmp (%r8),%edx
    29a1c1f9f:	add    %al,(%rax)
    29a1c1fa1:	add    -0x47ffffec(%rsi),%ebp
@@ -15123,17 +15192,20 @@
    29a1c1fbf:	add    %dl,%dl
    29a1c1fc1:	(bad)
    29a1c1fc2:	add    %al,(%rax)
    29a1c1fc4:	rolb   $1,(%rdi)
    29a1c1fc6:	add    %al,(%rax)
    29a1c1fc8:	adc    0x14(%rdi),%bh
    29a1c1fcb:	add    %al,(%rax)
-   29a1c1fcd:	ja     29a1c1fe7 <.debug_info+0xffc>
-   29a1c1fcf:	sbb    0x2(%rdx),%ebx
-   29a1c1fd5:	add    $0x77,%al
+   29a1c1fcd:	cmpsl  %es:(%rdi),%ds:(%rsi)
+   29a1c1fce:	sbb    %bl,(%rbx)
+   29a1c1fd0:	(bad)
+   29a1c1fd1:	add    (%rax),%al
+   29a1c1fd3:	add    %al,(%rax)
+   29a1c1fd5:	add    $0xa7,%al
    29a1c1fd7:	sbb    %bl,(%rbx)
    29a1c1fd9:	(bad)
    29a1c1fda:	add    (%rax),%al
    29a1c1fdc:	add    %al,(%rax)
    29a1c1fde:	or     (%rax),%eax
    29a1c1fe0:	add    %al,(%rax)
    29a1c1fe2:	add    %al,(%rax)
@@ -15152,28 +15224,27 @@
    29a1c2001:	add    %al,(%rax)
    29a1c2003:	add    -0x9ffffec(%rbp),%edx
    29a1c2009:	(bad)
    29a1c200a:	add    %al,(%rax)
    29a1c200c:	hlt
    29a1c200d:	(bad)
    29a1c200e:	add    %al,(%rax)
-   29a1c2010:	or     0x18(%rdi),%edi
-   29a1c2013:	sbb    0x2(%rdx),%ebx
-   29a1c2019:	notl   (%rax,%rax,1)
+   29a1c2010:	or     0x29a1b18(%rdi),%ebp
+   29a1c2016:	add    %al,(%rax)
+   29a1c2018:	add    %dh,%bh
+   29a1c201a:	adc    $0x0,%al
    29a1c201c:	add    %al,(%rcx,%rax,1)
    29a1c201f:	push   %rdx
    29a1c2020:	add    0x0(%rbp),%dh
    29a1c2023:	add    %al,(%rax)
    29a1c2025:	add    %ah,(%rcx)
    29a1c2027:	jg     29a1c203d <.debug_info+0x1052>
    29a1c2029:	add    %al,(%rax)
-   29a1c202b:	rex.X sbb %ebx,(%rbx)
-   29a1c202e:	(bad)
-   29a1c202f:	add    (%rax),%al
-   29a1c2031:	add    %al,(%rax)
+   29a1c202b:	jb     29a1c2046 <.debug_info+0x105b>
+   29a1c202d:	sbb    0x2(%rdx),%ebx
    29a1c2033:	add    0x0(%rax,%rax,1),%ch
    29a1c2037:	add    %dl,%dl
    29a1c2039:	add    %ecx,(%rsi,%rcx,8)
    29a1c203c:	adc    %al,(%rax)
    29a1c203e:	add    %al,(%rbx)
    29a1c2040:	scas   %es:(%rdi),%al
    29a1c2041:	adc    $0x0,%al
@@ -15192,18 +15263,16 @@
    29a1c205d:	add    %bl,(%rdx)
    29a1c205f:	or     %al,(%rax)
    29a1c2061:	add    %bl,(%rax)
    29a1c2063:	or     %al,(%rax)
    29a1c2065:	add    %dh,(%rdi)
    29a1c2067:	jg     29a1c207d <.debug_info+0x1092>
    29a1c2069:	add    %al,(%rax)
-   29a1c206b:	rex.X sbb %ebx,(%rbx)
-   29a1c206e:	(bad)
-   29a1c206f:	add    (%rax),%al
-   29a1c2071:	add    %al,(%rax)
+   29a1c206b:	jb     29a1c2086 <.debug_info+0x109b>
+   29a1c206d:	sbb    0x2(%rdx),%ebx
    29a1c2073:	add    $0x6c,%al
    29a1c2075:	add    %al,(%rax)
    29a1c2077:	add    %al,(%rcx)
    29a1c2079:	(bad)
    29a1c207a:	add    %eax,(%rcx)
    29a1c207c:	add    0x24000014(%rsi),%ebp
    29a1c2082:	or     %al,(%rax)
@@ -15215,30 +15284,30 @@
    29a1c2095:	add    %al,(%rbx)
    29a1c2097:	xchg   %eax,%ebp
    29a1c2098:	adc    $0x0,%al
    29a1c209a:	add    %bh,(%rsi)
    29a1c209c:	or     %al,(%rax)
    29a1c209e:	add    %bh,(%rax,%rcx,1)
    29a1c20a1:	add    %al,(%rax)
-   29a1c20a3:	or     0x19(%rsi),%ecx
+   29a1c20a3:	or     0x19(%rsi),%edi
    29a1c20a6:	sbb    0x2(%rdx),%ebx
    29a1c20ac:	notl   (%rax,%rax,1)
    29a1c20af:	add    %al,(%rcx,%rax,1)
    29a1c20b2:	push   %rdx
    29a1c20b3:	add    0x0(%rbp),%dh
    29a1c20b6:	add    %al,(%rax)
    29a1c20b8:	add    %bl,(%rdi,%rdi,2)
    29a1c20bb:	adc    $0x0,%al
-   29a1c20bd:	add    %dh,%bh
-   29a1c20bf:	sbb    %ebx,(%rbx)
+   29a1c20bd:	add    %ah,(%rdi)
+   29a1c20bf:	sbb    (%rbx),%bl
    29a1c20c1:	(bad)
    29a1c20c2:	add    (%rax),%al
    29a1c20c4:	add    %al,(%rax)
-   29a1c20c6:	add    %bh,%dh
-   29a1c20c8:	sbb    %ebx,(%rbx)
+   29a1c20c6:	add    (%rdi),%ah
+   29a1c20c8:	sbb    (%rbx),%bl
    29a1c20ca:	(bad)
    29a1c20cb:	add    (%rax),%al
    29a1c20cd:	add    %al,(%rax)
    29a1c20cf:	or     (%rax),%al
    29a1c20d1:	add    %al,(%rax)
    29a1c20d3:	add    %al,(%rax)
    29a1c20d5:	add    %al,(%rax)
@@ -15255,18 +15324,21 @@
    29a1c20f5:	add    %al,(%rax)
    29a1c20f7:	add    0x62000014(%rbp),%edx
    29a1c20fd:	or     %al,(%rax)
    29a1c20ff:	add    %ah,0x8(%rax)
    29a1c2102:	add    %al,(%rax)
    29a1c2104:	adc    0x14(%rdi),%bh
    29a1c2107:	add    %al,(%rax)
-   29a1c2109:	negl   (%rcx)
-   29a1c210b:	sbb    0x2(%rdx),%ebx
-   29a1c2111:	add    $0xf7,%al
-   29a1c2113:	sbb    %ebx,(%rbx)
+   29a1c2109:	(bad)
+   29a1c210a:	sbb    (%rbx),%bl
+   29a1c210c:	(bad)
+   29a1c210d:	add    (%rax),%al
+   29a1c210f:	add    %al,(%rax)
+   29a1c2111:	add    $0x27,%al
+   29a1c2113:	sbb    (%rbx),%bl
    29a1c2115:	(bad)
    29a1c2116:	add    (%rax),%al
    29a1c2118:	add    %al,(%rax)
    29a1c211a:	or     (%rax),%al
    29a1c211c:	add    %al,(%rax)
    29a1c211e:	add    %al,(%rax)
    29a1c2120:	add    %al,(%rax)
@@ -15278,36 +15350,30 @@
    29a1c2130:	add    %al,(%rax)
    29a1c2132:	add    0x77000014(%rdx),%esp
    29a1c2138:	or     %al,(%rax)
    29a1c213a:	add    %dh,0x8(%rbp)
    29a1c213d:	add    %al,(%rax)
    29a1c213f:	add    -0x79ffffec(%rbp),%edx
    29a1c2145:	or     %al,(%rax)
-   29a1c2147:	add    %al,-0xf50000(%rax,%rcx,1)
-   29a1c214e:	sbb    %ebx,(%rbx)
+   29a1c2147:	add    %al,0x2f0b0000(%rax,%rcx,1)
+   29a1c214e:	sbb    (%rbx),%bl
    29a1c2150:	(bad)
    29a1c2151:	add    (%rax),%al
    29a1c2153:	add    %al,(%rax)
    29a1c2155:	notl   (%rax,%rax,1)
    29a1c2158:	add    %al,(%rcx,%rax,1)
    29a1c215b:	push   %rdx
    29a1c215c:	add    0x0(%rbp),%dh
    29a1c215f:	add    %al,(%rax)
    29a1c2161:	add    %bl,(%rdi,%rdi,2)
    29a1c2164:	adc    $0x0,%al
-   29a1c2166:	add    %dl,(%rax)
-   29a1c2168:	sbb    (%rbx),%bl
-   29a1c216a:	(bad)
-   29a1c216b:	add    (%rax),%al
-   29a1c216d:	add    %al,(%rax)
-   29a1c216f:	add    %edx,(%rax)
-   29a1c2171:	sbb    (%rbx),%bl
-   29a1c2173:	(bad)
-   29a1c2174:	add    (%rax),%al
-   29a1c2176:	add    %al,(%rax)
+   29a1c2166:	add    %al,0x1a(%rax)
+   29a1c2169:	sbb    0x2(%rdx),%ebx
+   29a1c216f:	add    %eax,0x1a(%rax)
+   29a1c2172:	sbb    0x2(%rdx),%ebx
    29a1c2178:	or     (%rax),%eax
    29a1c217a:	add    %al,(%rax)
    29a1c217c:	add    %al,(%rax)
    29a1c217e:	add    %al,(%rax)
    29a1c2180:	faddl  (%rcx)
    29a1c2182:	and    %dl,(%rdx)
    29a1c2184:	add    %al,(%rax)
@@ -15320,21 +15386,20 @@
    29a1c21a1:	xchg   %eax,%ebp
    29a1c21a2:	adc    $0x0,%al
    29a1c21a4:	add    %ch,-0x57fffff8(%rdx)
    29a1c21aa:	or     %al,(%rax)
    29a1c21ac:	add    %dl,(%rdx)
    29a1c21ae:	jg     29a1c21c4 <.debug_info+0x11d9>
    29a1c21b0:	add    %al,(%rax)
-   29a1c21b2:	adc    %bl,(%rdx)
-   29a1c21b4:	sbb    0x2(%rdx),%ebx
-   29a1c21ba:	add    (%rax),%edx
-   29a1c21bc:	sbb    (%rbx),%bl
-   29a1c21be:	(bad)
-   29a1c21bf:	add    (%rax),%al
-   29a1c21c1:	add    %al,(%rax)
+   29a1c21b2:	rex sbb (%rbx),%bl
+   29a1c21b5:	(bad)
+   29a1c21b6:	add    (%rax),%al
+   29a1c21b8:	add    %al,(%rax)
+   29a1c21ba:	add    0x1a(%rax),%eax
+   29a1c21bd:	sbb    0x2(%rdx),%ebx
    29a1c21c3:	or     (%rax),%eax
    29a1c21c5:	add    %al,(%rax)
    29a1c21c7:	add    %al,(%rax)
    29a1c21c9:	add    %al,(%rax)
    29a1c21cb:	(bad)
    29a1c21cc:	add    %eax,(%rcx)
    29a1c21ce:	add    -0x4bffffec(%rsi),%ebp
@@ -15346,16 +15411,18 @@
    29a1c21e9:	xchg   %eax,%ebp
    29a1c21ea:	adc    $0x0,%al
    29a1c21ec:	add    %cl,%dh
    29a1c21ee:	or     %al,(%rax)
    29a1c21f0:	add    %cl,%ah
    29a1c21f2:	or     %al,(%rax)
    29a1c21f4:	add    %cl,(%rbx)
-   29a1c21f6:	sbb    %bl,(%rdx)
-   29a1c21f8:	sbb    0x2(%rdx),%ebx
+   29a1c21f6:	rex.W sbb (%rbx),%bl
+   29a1c21f9:	(bad)
+   29a1c21fa:	add    (%rax),%al
+   29a1c21fc:	add    %al,(%rax)
    29a1c21fe:	notl   (%rax,%rax,1)
    29a1c2201:	add    %al,(%rcx,%rax,1)
    29a1c2204:	push   %rdx
    29a1c2205:	add    0x0(%rbp),%dh
    29a1c2208:	add    %al,(%rax)
    29a1c220a:	add    %ah,(%rdx)
    29a1c220c:	and    $0x14,%al
@@ -15377,23 +15444,26 @@
    29a1c2231:	add    %al,(%rax)
    29a1c2233:	testb  $0x0,(%rax)
    29a1c2236:	add    %dh,%ah
    29a1c2238:	or     %al,(%rax)
    29a1c223a:	add    %dl,(%rdx)
    29a1c223c:	jg     29a1c2252 <.debug_info+0x1267>
    29a1c223e:	add    %al,(%rax)
-   29a1c2240:	jle    29a1c225c <.debug_info+0x1271>
-   29a1c2242:	sbb    0x2(%rdx),%ebx
-   29a1c2248:	add    %edi,0x1a(%rsi)
-   29a1c224b:	sbb    0x2(%rdx),%ebx
-   29a1c2251:	or     (%rax),%al
-   29a1c2253:	add    %al,(%rax)
-   29a1c2255:	add    %al,(%rax)
-   29a1c2257:	add    %al,(%rax)
-   29a1c2259:	jae    29a1c225c <.debug_info+0x1271>
+   29a1c2240:	scas   %es:(%rdi),%al
+   29a1c2241:	sbb    (%rbx),%bl
+   29a1c2243:	(bad)
+   29a1c2244:	add    (%rax),%al
+   29a1c2246:	add    %al,(%rax)
+   29a1c2248:	add    %ebp,0x29a1b1a(%rsi)
+   29a1c224e:	add    %al,(%rax)
+   29a1c2250:	add    %cl,(%rdx)
+   29a1c2252:	add    %al,(%rax)
+   29a1c2254:	add    %al,(%rax)
+   29a1c2256:	add    %al,(%rax)
+   29a1c2258:	add    %dh,0x1(%rbx)
    29a1c225b:	add    $0x3,%al
    29a1c225d:	scas   %es:(%rdi),%al
    29a1c225e:	adc    $0x0,%al
    29a1c2260:	add    %al,(%rax)
    29a1c2262:	or     %eax,(%rax)
    29a1c2264:	add    %bh,%dh
    29a1c2266:	or     %al,(%rax)
@@ -15406,23 +15476,26 @@
    29a1c227a:	add    %bl,(%rdx)
    29a1c227c:	or     %eax,(%rax)
    29a1c227e:	add    %bl,(%rax)
    29a1c2280:	or     %eax,(%rax)
    29a1c2282:	add    %dl,(%rdx)
    29a1c2284:	jg     29a1c229a <.debug_info+0x12af>
    29a1c2286:	add    %al,(%rax)
-   29a1c2288:	jle    29a1c22a4 <.debug_info+0x12b9>
-   29a1c228a:	sbb    0x2(%rdx),%ebx
-   29a1c2290:	add    0x1a(%rsi),%edi
-   29a1c2293:	sbb    0x2(%rdx),%ebx
-   29a1c2299:	or     (%rax),%al
-   29a1c229b:	add    %al,(%rax)
-   29a1c229d:	add    %al,(%rax)
-   29a1c229f:	add    %al,(%rax)
-   29a1c22a1:	(bad)
+   29a1c2288:	scas   %es:(%rdi),%al
+   29a1c2289:	sbb    (%rbx),%bl
+   29a1c228b:	(bad)
+   29a1c228c:	add    (%rax),%al
+   29a1c228e:	add    %al,(%rax)
+   29a1c2290:	add    0x29a1b1a(%rsi),%ebp
+   29a1c2296:	add    %al,(%rax)
+   29a1c2298:	add    %cl,(%rdx)
+   29a1c229a:	add    %al,(%rax)
+   29a1c229c:	add    %al,(%rax)
+   29a1c229e:	add    %al,(%rax)
+   29a1c22a0:	add    %al,(%rdi)
    29a1c22a2:	add    %eax,(%rcx)
    29a1c22a4:	add    0x24000014(%rsi),%ebp
    29a1c22aa:	or     %eax,(%rax)
    29a1c22ac:	add    %ah,(%rdx)
    29a1c22ae:	or     %eax,(%rax)
    29a1c22b0:	add    %al,(%rbx)
    29a1c22b2:	movabs %al,0x2d0000092f000014
@@ -15430,24 +15503,24 @@
    29a1c22bd:	add    %al,(%rbx)
    29a1c22bf:	xchg   %eax,%ebp
    29a1c22c0:	adc    $0x0,%al
    29a1c22c2:	add    %bh,(%rsi)
    29a1c22c4:	or     %eax,(%rax)
    29a1c22c6:	add    %bh,(%rcx,%rcx,1)
    29a1c22c9:	add    %al,(%rax)
-   29a1c22cb:	or     0x29a1b1a(%rsi),%eax
+   29a1c22cb:	or     0x29a1b1a(%rsi),%esi
    29a1c22d1:	add    %al,(%rax)
    29a1c22d3:	add    %dh,%bh
    29a1c22d5:	adc    $0x0,%al
    29a1c22d7:	add    %al,(%rcx,%rax,1)
    29a1c22da:	push   %rdx
    29a1c22db:	add    0x0(%rax,%rax,1),%dh
    29a1c22df:	add    %al,(%rax)
    29a1c22e1:	add    %al,(%rax)
-   29a1c22e3:	or     $0x9a1b1aa0,%eax
+   29a1c22e3:	or     $0x9a1b1ad0,%eax
    29a1c22e8:	add    (%rax),%al
    29a1c22ea:	add    %al,(%rax)
    29a1c22ec:	(bad)
    29a1c22ed:	(bad)
    29a1c22ee:	add    %al,(%rax)
    29a1c22f0:	(bad)
    29a1c22f1:	adc    (%rax),%eax
@@ -15455,32 +15528,29 @@
    29a1c22f6:	push   %rdx
    29a1c22f7:	or     %eax,(%rbx)
    29a1c22f9:	cmp    %al,0x1b(%rcx)
    29a1c22fc:	(bad)
    29a1c22fd:	add    (%rax),%al
    29a1c22ff:	add    %al,(%rax)
    29a1c2301:	add    %cl,(%rbx)
-   29a1c2303:	lods   %ds:(%rsi),%eax
-   29a1c2304:	sbb    (%rbx),%bl
-   29a1c2306:	(bad)
-   29a1c2307:	add    (%rax),%al
-   29a1c2309:	add    %al,(%rax)
+   29a1c2303:	fstpl  (%rdx)
+   29a1c2305:	sbb    0x2(%rdx),%ebx
    29a1c230b:	(bad)
    29a1c230c:	(bad)
    29a1c230d:	add    %al,(%rax)
    29a1c230f:	add    $0x1,%al
    29a1c2311:	push   %rdx
    29a1c2312:	or     %eax,(%rbx)
    29a1c2314:	add    %al,0x1b(%rcx)
    29a1c2317:	(bad)
    29a1c2318:	add    (%rax),%al
    29a1c231a:	add    %al,(%rax)
    29a1c231c:	add    %al,(%rax)
    29a1c231e:	add    %bh,(%rcx)
-   29a1c2320:	mov    $0x60000014,%ebx
+   29a1c2320:	mov    $0x90000014,%ebx
    29a1c2325:	sbb    %ebx,(%rbx)
    29a1c2327:	(bad)
    29a1c2328:	add    (%rax),%al
    29a1c232a:	add    %al,(%rax)
    29a1c232c:	pop    %rax
    29a1c232d:	add    %al,(%rax)
    29a1c232f:	add    %al,(%rax)
@@ -15494,24 +15564,24 @@
    29a1c233e:	adc    $0x0,%al
    29a1c2340:	add    %cl,0x9(%rdx)
    29a1c2343:	add    %al,(%rax)
    29a1c2345:	rex.RX or %r8d,(%rax)
    29a1c2348:	add    %bh,(%rdx)
    29a1c234a:	out    %eax,$0x14
    29a1c234c:	add    %al,(%rax)
-   29a1c234e:	add    -0x60f48054(%rcx),%edx
+   29a1c234e:	add    -0x30f48054(%rcx),%edx
    29a1c2354:	sbb    %ebx,(%rbx)
    29a1c2356:	(bad)
    29a1c2357:	add    (%rax),%al
    29a1c2359:	add    %al,(%rax)
    29a1c235b:	adc    $0x400000d,%eax
    29a1c2360:	add    %ebx,0x2(%rcx)
    29a1c2363:	jne    29a1c2365 <.debug_info+0x137a>
    29a1c2365:	add    %al,(%rax)
-   29a1c2367:	adc    $0x97,%al
+   29a1c2367:	adc    $0xc7,%al
    29a1c2369:	(bad)
    29a1c236a:	sbb    0x2(%rdx),%ebx
    29a1c2370:	(bad)
    29a1c2371:	(bad)
    29a1c2372:	add    %al,(%rax)
    29a1c2374:	add    %ah,(%rbx)
    29a1c2376:	outsl  %fs:(%rsi),(%dx)
@@ -15658,15 +15728,15 @@
    29a1c24e8:	jae    29a1c254f <.debug_info+0x1564>
    29a1c24ea:	movsxd 0x6f(%rcx,%rbp,2),%esi
    29a1c24ee:	outsb  %ds:(%rsi),(%dx)
    29a1c24ef:	pop    %rdi
    29a1c24f0:	ja     29a1c2564 <.debug_info+0x1579>
    29a1c24f2:	imul   $0x100656c,0x62(%rcx,%riz,2),%esi
    29a1c24fa:	mov    $0x1,%bh
-   29a1c24fc:	loopne 29a1c2513 <.debug_info+0x1528>
+   29a1c24fc:	adc    %dl,(%rsi)
    29a1c24fe:	sbb    0x2(%rdx),%ebx
    29a1c2504:	(bad)
    29a1c2509:	add    %al,(%rax)
    29a1c250b:	add    %al,(%rcx)
    29a1c250d:	pushf
    29a1c250e:	(bad)
    29a1c250f:	(bad)
@@ -15692,18 +15762,16 @@
    29a1c253c:	movabs %al,0x1d00000996000009
    29a1c2545:	imul   $0x12507bb,(%rax),%eax
    29a1c254b:	add    %al,(%rax)
    29a1c254d:	rorl   %cl,(%rcx)
    29a1c254f:	add    %al,(%rax)
    29a1c2551:	int    $0x9
    29a1c2553:	add    %al,(%rax)
-   29a1c2555:	ds rclb $0x1b,(%rsi)
-   29a1c2559:	(bad)
-   29a1c255a:	add    (%rax),%al
-   29a1c255c:	add    %al,(%rax)
+   29a1c2555:	ds lock (bad)
+   29a1c2558:	sbb    0x2(%rdx),%ebx
    29a1c255e:	push   %rax
    29a1c255f:	add    %al,(%rax)
    29a1c2561:	add    %al,(%rax)
    29a1c2563:	add    %al,(%rax)
    29a1c2565:	add    %bl,%bl
    29a1c2567:	adc    $0x6e1d0000,%eax
    29a1c256c:	gs ja  29a1c25ce <.debug_info+0x15e3>
@@ -15712,74 +15780,74 @@
    29a1c2572:	je     29a1c25d9 <.debug_info+0x15ee>
    29a1c2574:	movsxd -0x29(%rax,%rax,1),%esi
    29a1c2578:	or     $0x175,%eax
    29a1c257d:	in     (%dx),%al
    29a1c257e:	or     %eax,(%rax)
    29a1c2580:	add    %ch,%dl
    29a1c2582:	or     %eax,(%rax)
-   29a1c2584:	add    %cl,-0x65e4e90c(%rip)        # 234373c7e <__size_of_stack_reserve__+0x234173c7e>
+   29a1c2584:	add    %cl,-0x65e4e8dc(%rip)        # 234373cae <__size_of_stack_reserve__+0x234173cae>
    29a1c258a:	add    (%rax),%al
    29a1c258c:	add    %al,(%rax)
    29a1c258e:	adc    $0xb200000d,%eax
    29a1c2593:	adc    $0x1040000,%eax
    29a1c2598:	pop    %rcx
    29a1c2599:	add    0x0(%rbx),%dh
-   29a1c259c:	add    %dl,(%rsi,%rdi,8)
+   29a1c259c:	add    %dl,(%rsi,%rbp,1)
    29a1c259f:	(bad)
    29a1c25a0:	sbb    0x2(%rdx),%ebx
-   29a1c25a6:	add    %cl,0xc0b0000(%rip)        # 2a62725ac <.debug_rnglists+0xc0a2508>
+   29a1c25a6:	add    %cl,0x3c0b0000(%rip)        # 2d62725ac <.debug_rnglists+0x3c0a2508>
    29a1c25ac:	(bad)
    29a1c25ad:	sbb    0x2(%rdx),%ebx
    29a1c25b3:	(bad)
    29a1c25b4:	(bad)
    29a1c25b5:	add    %al,(%rax)
    29a1c25b7:	add    $0x1,%al
    29a1c25b9:	push   %rdx
    29a1c25ba:	or     %eax,(%rbx)
    29a1c25bc:	fadds  0x1b(%rax)
    29a1c25bf:	(bad)
    29a1c25c0:	add    (%rax),%al
    29a1c25c2:	add    %al,(%rax)
    29a1c25c4:	add    %al,(%rax)
-   29a1c25c6:	or     $0x9a1b1640,%eax
+   29a1c25c6:	or     $0x9a1b1670,%eax
    29a1c25cb:	add    (%rax),%al
    29a1c25cd:	add    %al,(%rax)
    29a1c25cf:	xchg   %cl,0x15f30000(%rip)        # 2b00f25d5 <.debug_rnglists+0x15f22531>
    29a1c25d5:	add    %al,(%rax)
    29a1c25d7:	add    $0x1,%al
    29a1c25d9:	push   %rdx
    29a1c25da:	add    0x0(%rbx),%dh
-   29a1c25dd:	add    %dl,0x29a1b16(,%rbp,2)
+   29a1c25dd:	add    %dl,0x29a1b16(,%rbx,4)
    29a1c25e4:	add    %al,(%rax)
    29a1c25e6:	add    %ch,0xd(%rsi)
    29a1c25e9:	add    %al,(%rax)
-   29a1c25eb:	or     $0x9a1b1691,%eax
+   29a1c25eb:	or     $0x9a1b16c1,%eax
    29a1c25f0:	add    (%rax),%al
    29a1c25f2:	add    %al,(%rax)
    29a1c25f4:	rex.RB or $0x161f0000,%eax
    29a1c25fa:	add    %al,(%rax)
    29a1c25fc:	add    $0x1,%al
    29a1c25fe:	push   %rcx
    29a1c25ff:	add    0x1047fb0(%rcx),%edx
    29a1c2605:	pop    %rax
    29a1c2606:	add    (%rax),%cl
    29a1c2608:	xor    %al,(%rax)
-   29a1c260a:	or     $0x9a1b1732,%eax
+   29a1c260a:	or     $0x9a1b1762,%eax
    29a1c260f:	add    (%rax),%al
    29a1c2611:	add    %al,(%rax)
    29a1c2613:	(bad)
    29a1c2614:	(bad)
    29a1c2615:	add    %al,(%rax)
    29a1c2617:	ds (bad)
    29a1c2619:	add    %al,(%rax)
    29a1c261b:	add    $0x1,%al
    29a1c261d:	push   %rdx
    29a1c261e:	or     %eax,(%rbx)
    29a1c2620:	movabs 0x29a1b40,%al
-   29a1c2629:	or     0x17(%rdx),%eax
+   29a1c2629:	or     0x17(%rdx),%esi
    29a1c262c:	sbb    0x2(%rdx),%ebx
    29a1c2632:	(bad)
    29a1c2633:	(bad)
    29a1c2634:	add    %al,(%rax)
    29a1c2636:	add    $0x1,%al
    29a1c2638:	push   %rdx
    29a1c2639:	or     %eax,(%rbx)
@@ -15796,15 +15864,15 @@
    29a1c264e:	jb     29a1c26b5 <.debug_info+0x16ca>
    29a1c2650:	jo     29a1c26c1 <.debug_info+0x16d6>
    29a1c2652:	jb     29a1c26c8 <.debug_info+0x16dd>
    29a1c2654:	pop    %rdi
    29a1c2655:	gs jb  29a1c26ca <.debug_info+0x16df>
    29a1c2658:	outsl  %ds:(%rsi),(%dx)
    29a1c2659:	jb     29a1c265b <.debug_info+0x1670>
-   29a1c265b:	add    %edx,0x70(%rcx,%rax,1)
+   29a1c265b:	add    %edx,-0x60(%rcx,%rax,1)
    29a1c265f:	adc    $0x29a1b,%eax
    29a1c2664:	add    %al,(%rax)
    29a1c2666:	imul   $0x0,(%rax),%eax
    29a1c266c:	add    %al,(%rax)
    29a1c266e:	add    %ebx,0x26000017(%rdi,%rbp,1)
    29a1c2675:	insl   (%dx),%es:(%rdi)
    29a1c2676:	jae    29a1c26df <.debug_info+0x16f4>
@@ -15819,24 +15887,24 @@
    29a1c2689:	(bad)
    29a1c268a:	jb     29a1c26f3 <.debug_info+0x1708>
    29a1c268c:	jo     29a1c268e <.debug_info+0x16a3>
    29a1c268e:	xchg   %eax,%ebx
    29a1c268f:	or     0x2000000(%rbx),%esi
    29a1c2695:	xchg   %eax,%ecx
    29a1c2696:	pop    %rax
-   29a1c2697:	or     $0x9a1b159c,%eax
+   29a1c2697:	or     $0x9a1b15cc,%eax
    29a1c269c:	add    (%rax),%al
    29a1c269e:	add    %al,(%rax)
    29a1c26a0:	sbb    $0xc300000e,%eax
    29a1c26a5:	(bad)
    29a1c26a6:	add    %al,(%rax)
    29a1c26a8:	add    $0x1,%al
    29a1c26aa:	push   %rdx
    29a1c26ab:	add    %esi,(%rdx)
-   29a1c26ad:	add    %cl,-0x65e4ea4a(%rip)        # 234373c69 <__size_of_stack_reserve__+0x234173c69>
+   29a1c26ad:	add    %cl,-0x65e4ea1a(%rip)        # 234373c99 <__size_of_stack_reserve__+0x234173c99>
    29a1c26b3:	add    (%rax),%al
    29a1c26b5:	add    %al,(%rax)
    29a1c26b7:	(bad)
    29a1c26b8:	(bad)
    29a1c26b9:	add    %al,(%rax)
    29a1c26bb:	in     (%dx),%al
    29a1c26bc:	(bad)
@@ -15848,39 +15916,39 @@
    29a1c26c5:	rex sbb 0x2(%rdx),%ebx
    29a1c26cc:	add    $0x1,%al
    29a1c26ce:	push   %rcx
    29a1c26cf:	add    %esi,(%rcx)
    29a1c26d1:	add    $0x1,%al
    29a1c26d3:	pop    %rax
    29a1c26d4:	add    %ecx,0x0(%rbx)
-   29a1c26d7:	or     $0x9a1b15c5,%eax
+   29a1c26d7:	or     $0x9a1b15f5,%eax
    29a1c26dc:	add    (%rax),%al
    29a1c26de:	add    %al,(%rax)
    29a1c26e0:	sbb    $0x300000e,%eax
    29a1c26e5:	(bad)
    29a1c26e6:	add    %al,(%rax)
    29a1c26e8:	add    $0x1,%al
    29a1c26ea:	push   %rdx
    29a1c26eb:	add    %esi,(%rdx)
-   29a1c26ed:	add    %cl,-0x65e4ea2d(%rip)        # 234373cc6 <__size_of_stack_reserve__+0x234173cc6>
+   29a1c26ed:	add    %cl,-0x65e4e9fd(%rip)        # 234373cf6 <__size_of_stack_reserve__+0x234173cf6>
    29a1c26f3:	add    (%rax),%al
    29a1c26f5:	add    %al,(%rax)
    29a1c26f7:	jrcxz  29a1c2706 <.debug_info+0x171b>
    29a1c26f9:	add    %al,(%rax)
    29a1c26fb:	and    %edx,(%rdi)
    29a1c26fd:	add    %al,(%rax)
    29a1c26ff:	add    $0x1,%al
    29a1c2701:	push   %rcx
    29a1c2702:	add    0x0(%rbx),%dh
    29a1c2705:	add    $0x1,%al
    29a1c2707:	pop    %rax
    29a1c2708:	add    0x0(%rax,%rax,1),%dh
-   29a1c270c:	adc    $0xd9,%al
-   29a1c270e:	adc    $0x29a1b,%eax
-   29a1c2713:	add    %al,(%rax)
+   29a1c270c:	adc    $0x9,%al
+   29a1c270e:	(bad)
+   29a1c270f:	sbb    0x2(%rdx),%ebx
    29a1c2715:	fmuls  0x41000000(%rip)        # 2db1c271b <.debug_rnglists+0x40ff2677>
    29a1c271b:	data16 ja 29a1c2790 <.debug_info+0x5a>
    29a1c271e:	imul   $0x75625f5f,0x0(%rbp,%riz,2),%esi
    29a1c2726:	imul   $0x77665f6e,0x69(%rsp,%rsi,2),%ebp
    29a1c272e:	jb     29a1c2799 <.debug_info+0x63>
    29a1c2730:	je     29a1c2797 <.debug_info+0x61>
    29a1c2732:	add    %cl,(%rsi)
@@ -15916,15 +15984,15 @@
    29a1c278c:	jne    29a1c27c7 <.debug_info+0x91>
    29a1c278e:	cmp    %eax,(%rax)
    29a1c2790:	or     $0x22,%al
    29a1c2792:	(bad)
    29a1c2793:	add    %al,(%rax)
    29a1c2795:	or     (%rdi),%al
    29a1c2797:	add    %al,(%rax)
-   29a1c2799:	mov    $0x1a,%al
+   29a1c2799:	loopne 29a1c27b5 <.debug_info+0x7f>
    29a1c279b:	sbb    0x2(%rdx),%ebx
    29a1c27a1:	(bad)
    29a1c27a6:	add    %al,(%rax)
    29a1c27a8:	add    %al,(%rsp,%rcx,1)
    29a1c27ab:	add    %al,(%rax)
    29a1c27ad:	add    (%rcx),%al
    29a1c27af:	(bad)
@@ -16712,19 +16780,16 @@
    29a1c2e3a:	imul   $0x4c545f77,0x67(%rsi),%ebp
    29a1c2e41:	push   %rbx
    29a1c2e42:	movsxd 0x6c(%rcx),%esp
    29a1c2e45:	insb   (%dx),%es:(%rdi)
    29a1c2e46:	(bad)
    29a1c2e4b:	jp     29a1c2e6c <.debug_info+0x736>
    29a1c2e4d:	add    %eax,(%rax)
-   29a1c2e4f:	add    %ah,(%rax)
-   29a1c2e51:	sbb    $0x1b,%al
-   29a1c2e53:	(bad)
-   29a1c2e54:	add    (%rax),%al
-   29a1c2e56:	add    %al,(%rax)
+   29a1c2e4f:	add    %dl,0x1c(%rax)
+   29a1c2e52:	sbb    0x2(%rdx),%ebx
    29a1c2e58:	repnz add %al,(%rax)
    29a1c2e5b:	add    %al,(%rax)
    29a1c2e5d:	add    %al,(%rax)
    29a1c2e5f:	add    %al,(%rcx)
    29a1c2e61:	pushf
    29a1c2e62:	outsb  %ds:(%rsi),(%dx)
    29a1c2e63:	or     %al,(%rax)
@@ -16755,16 +16820,15 @@
    29a1c2e99:	jae    29a1c2f00 <.debug_info+0x7ca>
    29a1c2e9b:	jb     29a1c2f13 <.debug_info+0x7dd>
    29a1c2e9d:	gs add %bh,%fs:0x53(%rdi,%rcx,1)
    29a1c2ea3:	add    %eax,(%rax)
    29a1c2ea5:	add    %ah,0xd00000b(%rip)        # 2a71c2eb6 <.debug_rnglists+0xcff2e12>
    29a1c2eab:	or     (%rax),%eax
    29a1c2ead:	add    %ah,(%rax)
-   29a1c2eaf:	xchg   %eax,%ebp
-   29a1c2eb0:	sbb    $0x1b,%al
+   29a1c2eaf:	(bad)
    29a1c2eb2:	(bad)
    29a1c2eb3:	add    (%rax),%al
    29a1c2eb5:	add    %al,(%rax)
    29a1c2eb7:	rex.WXB add %al,(%r8)
    29a1c2eba:	add    %al,(%rax)
    29a1c2ebc:	add    %al,(%rax)
    29a1c2ebe:	add    %bl,%bl
@@ -16777,75 +16841,80 @@
    29a1c2ed4:	or     (%rax),%eax
    29a1c2ed6:	add    %cl,(%rdx)
    29a1c2ed8:	je     29a1c2eda <.debug_info+0x7a4>
    29a1c2eda:	mov    %ebp,0x5de(%rip)        # 29a1c34be <.debug_info+0x15c>
    29a1c2ee0:	stos   %al,%es:(%rdi)
    29a1c2ee1:	or     (%rax),%eax
    29a1c2ee3:	add    %ch,0x600000b(%rax)
-   29a1c2ee9:	mov    $0x1c,%ah
+   29a1c2ee9:	in     $0x1c,%al
    29a1c2eeb:	sbb    0x2(%rdx),%ebx
    29a1c2ef1:	mov    (%rsi),%eax
    29a1c2ef3:	add    %al,(%rax)
-   29a1c2ef5:	or     $0x9a1b1cdb,%eax
+   29a1c2ef5:	or     $0x9a1b1d0b,%eax
    29a1c2efa:	add    (%rax),%al
    29a1c2efc:	add    %al,(%rax)
    29a1c2efe:	rex.XB (bad)
    29a1c2f00:	add    %al,(%rax)
    29a1c2f02:	add    (%rcx),%eax
    29a1c2f04:	push   %rdx
    29a1c2f05:	or     %eax,(%rbx)
    29a1c2f07:	movabs 0x29a1b70,%al
    29a1c2f10:	add    %ah,(%rcx)
    29a1c2f12:	outsb  %ds:(%rsi),(%dx)
    29a1c2f13:	or     %al,(%rax)
-   29a1c2f15:	add    %ah,0x1c(%rbp)
-   29a1c2f18:	sbb    0x2(%rdx),%ebx
-   29a1c2f1e:	add    %esp,0x1c(%rbp)
-   29a1c2f21:	sbb    0x2(%rdx),%ebx
+   29a1c2f15:	add    %dl,0x29a1b1c(%rbp)
+   29a1c2f1b:	add    %al,(%rax)
+   29a1c2f1d:	add    %al,(%rcx)
+   29a1c2f1f:	xchg   %eax,%ebp
+   29a1c2f20:	sbb    $0x1b,%al
+   29a1c2f22:	(bad)
+   29a1c2f23:	add    (%rax),%al
+   29a1c2f25:	add    %al,(%rax)
    29a1c2f27:	sbb    (%rax),%eax
    29a1c2f29:	add    %al,(%rax)
    29a1c2f2b:	add    %al,(%rax)
    29a1c2f2d:	add    %al,(%rax)
    29a1c2f2f:	add    %ebx,0x81307(%rcx)
    29a1c2f35:	add    %dl,0x890(%rip)        # 29a1c37cb <.debug_info+0x469>
    29a1c2f3b:	(bad)
-   29a1c2f3c:	je     29a1c2f5a <.debug_info+0x824>
-   29a1c2f3e:	sbb    0x2(%rdx),%ebx
+   29a1c2f3c:	movsb  %ds:(%rsi),%es:(%rdi)
+   29a1c2f3d:	sbb    $0x1b,%al
+   29a1c2f3f:	(bad)
+   29a1c2f40:	add    (%rax),%al
+   29a1c2f42:	add    %al,(%rax)
    29a1c2f44:	sub    %ecx,(%rdx)
    29a1c2f46:	add    %al,(%rax)
    29a1c2f48:	add    %ah,(%rdx)
    29a1c2f4a:	outsb  %ds:(%rsi),(%dx)
    29a1c2f4b:	or     %al,(%rax)
-   29a1c2f4d:	add    %al,0x29a1b1c(%rax)
+   29a1c2f4d:	add    %dh,0x29a1b1c(%rax)
    29a1c2f53:	add    %al,(%rax)
    29a1c2f55:	add    %al,(%rdx)
    29a1c2f57:	cltd
    29a1c2f58:	add    %al,(%rax)
    29a1c2f5a:	add    %al,(%rcx)
    29a1c2f5c:	xchg   %al,(%rdi)
    29a1c2f5e:	or     %r8b,(%r8)
    29a1c2f61:	add    %ah,(%rbx)
    29a1c2f63:	cltd
    29a1c2f64:	add    %al,(%rax)
    29a1c2f66:	add    %dl,0x890(%rip)        # 29a1c37fc <.debug_info+0x49a>
    29a1c2f6c:	(bad)
-   29a1c2f6d:	cmc
-   29a1c2f6e:	sbb    $0x1b,%al
-   29a1c2f70:	(bad)
-   29a1c2f71:	add    (%rax),%al
-   29a1c2f73:	add    %al,(%rax)
-   29a1c2f75:	sub    %ecx,(%rdx)
-   29a1c2f77:	add    %al,(%rax)
-   29a1c2f79:	add    %al,(%rax)
-   29a1c2f7b:	(bad)
-   29a1c2f7c:	in     $0x1c,%eax
-   29a1c2f7e:	sbb    0x2(%rdx),%ebx
-   29a1c2f84:	ss (bad)
+   29a1c2f6d:	and    $0x29a1b1d,%eax
+   29a1c2f72:	add    %al,(%rax)
+   29a1c2f74:	add    %ch,(%rcx)
+   29a1c2f76:	or     (%rax),%al
+   29a1c2f78:	add    %al,(%rax)
+   29a1c2f7a:	add    %al,(%rsi)
+   29a1c2f7c:	adc    $0x29a1b1d,%eax
+   29a1c2f81:	add    %al,(%rax)
+   29a1c2f83:	add    %dh,(%rsi)
+   29a1c2f85:	(bad)
    29a1c2f86:	add    %al,(%rax)
-   29a1c2f88:	or     $0x9a1b1d0d,%eax
+   29a1c2f88:	or     $0x9a1b1d3d,%eax
    29a1c2f8d:	add    (%rax),%al
    29a1c2f8f:	add    %al,(%rax)
    29a1c2f91:	gs (bad)
    29a1c2f93:	add    %al,(%rax)
    29a1c2f95:	add    (%rcx),%eax
    29a1c2f97:	push   %rdx
    29a1c2f98:	or     %eax,(%rbx)
@@ -16889,22 +16958,22 @@
    29a1c2ff7:	jbe    29a1c305e <.debug_info+0x928>
    29a1c2ff9:	pop    %rdi
    29a1c2ffa:	imul   $0x5f,0x79(%rbp),%esp
    29a1c2ffe:	fs je  29a1c3070 <.debug_info+0x93a>
    29a1c3001:	jb     29a1c3003 <.debug_info+0x8cd>
    29a1c3003:	rex.B iret
    29a1c3005:	add    %al,(%rax)
-   29a1c3007:	add    %dl,0x29a1b1b(%rax)
-   29a1c300d:	add    %al,(%rax)
-   29a1c300f:	add    %al,0x0(%rcx)
-   29a1c3015:	add    %al,(%rax)
-   29a1c3017:	add    %al,(%rcx)
-   29a1c3019:	pushf
-   29a1c301a:	or     %eax,%fs:(%rax)
-   29a1c301d:	add    %cl,(%rcx)
+   29a1c3007:	add    %al,%al
+   29a1c3009:	sbb    (%rbx),%ebx
+   29a1c300b:	(bad)
+   29a1c300c:	add    (%rax),%al
+   29a1c300e:	add    %al,(%rax)
+   29a1c3010:	addl   $0x0,(%rax)
+   29a1c3016:	add    %al,(%rax)
+   29a1c3018:	add    %ebx,0x9000009(%rsp,%riz,2)
    29a1c301f:	imul   $0x0,0x79(%rbp),%esp
    29a1c3023:	sub    %dil,(%r9,%rax,1)
    29a1c3027:	add    %al,(%rax)
    29a1c3029:	mov    $0xb200000b,%edx
    29a1c302e:	or     (%rax),%eax
    29a1c3030:	add    %cl,(%rdx)
    29a1c3032:	jo     29a1c30a6 <.debug_info+0x970>
@@ -16917,33 +16986,33 @@
    29a1c3047:	add    %al,(%rax)
    29a1c3049:	or     0x75(%rbx),%ah
    29a1c304c:	jb     29a1c30ad <.debug_info+0x977>
    29a1c304e:	imul   $0x0,0x79(%rbp),%esp
    29a1c3052:	rex.R (bad)
    29a1c3054:	fiadds 0xbff0000(%rip)        # 2a61b305a <.debug_rnglists+0xbfe2fb6>
    29a1c305a:	add    %al,(%rax)
-   29a1c305c:	testl  $0xc00e0000,(%rbx)
+   29a1c305c:	testl  $0xf00e0000,(%rbx)
    29a1c3062:	sbb    (%rbx),%ebx
    29a1c3064:	(bad)
    29a1c3065:	add    (%rax),%al
    29a1c3067:	add    %al,(%rax)
    29a1c3069:	rolb   $0x0,(%rsi)
    29a1c306c:	add    %al,0x9(%rdx)
    29a1c306f:	add    %al,(%rax)
    29a1c3071:	add    (%rcx),%eax
    29a1c3073:	push   %rdx
    29a1c3074:	add    0x0(%rax,%rax,1),%dh
    29a1c3078:	(bad)
-   29a1c3079:	repz sbb (%rbx),%ebx
+   29a1c3079:	and    (%rbx,%rbx,1),%ebx
    29a1c307c:	(bad)
    29a1c307d:	add    (%rax),%al
    29a1c307f:	add    %al,(%rax)
    29a1c3081:	mov    (%rsi),%eax
    29a1c3083:	add    %al,(%rax)
-   29a1c3085:	or     $0x9a1b1bfc,%eax
+   29a1c3085:	or     $0x9a1b1c2c,%eax
    29a1c308a:	add    (%rax),%al
    29a1c308c:	add    %al,(%rax)
    29a1c308e:	lahf
    29a1c308f:	(bad)
    29a1c3090:	add    %al,(%rax)
    29a1c3092:	add    (%rcx),%eax
    29a1c3094:	push   %rdx
@@ -16960,19 +17029,16 @@
    29a1c30ab:	(bad)
    29a1c30ac:	fs fs pop %rdi
    29a1c30af:	imul   $0x5f,0x79(%rbp),%esp
    29a1c30b3:	fs je  29a1c3125 <.debug_info+0x9ef>
    29a1c30b6:	jb     29a1c30b8 <.debug_info+0x982>
    29a1c30b8:	sub    %bh,%cl
    29a1c30ba:	add    %al,(%rax)
-   29a1c30bc:	add    %ah,(%rax)
-   29a1c30be:	sbb    (%rbx),%ebx
-   29a1c30c0:	(bad)
-   29a1c30c1:	add    (%rax),%al
-   29a1c30c3:	add    %al,(%rax)
+   29a1c30bc:	add    %dl,0x1b(%rax)
+   29a1c30bf:	sbb    0x2(%rdx),%ebx
    29a1c30c5:	outsl  %ds:(%rsi),(%dx)
    29a1c30c6:	add    %al,(%rax)
    29a1c30c8:	add    %al,(%rax)
    29a1c30ca:	add    %al,(%rax)
    29a1c30cc:	add    %al,(%rcx)
    29a1c30ce:	pushf
    29a1c30cf:	and    $0xa,%al
@@ -16995,114 +17061,110 @@
    29a1c30ff:	imul   $0x0,0x79(%rbp),%esp
    29a1c3103:	sub    $0x15,%al
    29a1c3105:	and    $0xa,%al
    29a1c3107:	add    %al,(%rax)
    29a1c3109:	(bad)
    29a1c310a:	or     $0x0,%al
    29a1c310c:	add    %dl,0xe00000c(%rdx)
-   29a1c3112:	rex.WRXB sbb (%r11),%r11
-   29a1c3115:	(bad)
-   29a1c3116:	add    (%rax),%al
-   29a1c3118:	add    %al,(%rax)
+   29a1c3112:	jg     29a1c312f <.debug_info+0x9f9>
+   29a1c3114:	sbb    0x2(%rdx),%ebx
    29a1c311a:	loope  29a1c3122 <.debug_info+0x9ec>
    29a1c311c:	add    %al,(%rax)
    29a1c311e:	testl  $0x1030000,(%rcx)
    29a1c3124:	push   %rdx
    29a1c3125:	add    %esi,(%rcx)
    29a1c3127:	add    (%rcx),%eax
    29a1c3129:	push   %rcx
    29a1c312a:	add    %ecx,0x0(%rax)
    29a1c312d:	(bad)
-   29a1c312e:	insl   (%dx),%es:(%rdi)
+   29a1c312e:	popf
    29a1c312f:	sbb    (%rbx),%ebx
    29a1c3131:	(bad)
    29a1c3132:	add    (%rax),%al
    29a1c3134:	add    %al,(%rax)
    29a1c3136:	rolb   $0x0,(%rsi)
    29a1c3139:	add    %cl,(%rdi)
    29a1c313b:	or     (%rax),%al
    29a1c313d:	add    %al,(%rbx)
    29a1c313f:	add    %edx,0x2(%rdx)
    29a1c3142:	je     29a1c3144 <.debug_info+0xa0e>
-   29a1c3144:	add    %cl,-0x65e4e478(%rip)        # 234374cd2 <__size_of_stack_reserve__+0x234174cd2>
+   29a1c3144:	add    %cl,-0x65e4e448(%rip)        # 234374d02 <__size_of_stack_reserve__+0x234174d02>
    29a1c314a:	add    (%rax),%al
    29a1c314c:	add    %al,(%rax)
    29a1c314e:	lahf
    29a1c314f:	(bad)
    29a1c3150:	add    %al,(%rax)
    29a1c3152:	add    (%rcx),%eax
    29a1c3154:	push   %rdx
    29a1c3155:	add    0x0(%rax,%rax,1),%dh
    29a1c3159:	add    %cl,(%rax)
-   29a1c315b:	addl   $0xb0000008,0x6e260000(%rip)        # 308423165 <.debug_rnglists+0x6e2530c1>
+   29a1c315b:	addl   $0xe0000008,0x6e260000(%rip)        # 308423165 <.debug_rnglists+0x6e2530c1>
    29a1c3165:	sbb    (%rbx),%bl
    29a1c3167:	(bad)
    29a1c3168:	add    (%rax),%al
    29a1c316a:	add    %al,(%rax)
    29a1c316c:	jo     29a1c316e <.debug_info+0xa38>
    29a1c316e:	add    %al,(%rax)
    29a1c3170:	add    %al,(%rax)
    29a1c3172:	add    %al,(%rax)
    29a1c3174:	add    %ebx,0x890(%rdi,%rdx,1)
    29a1c317b:	mov    $0xb700000c,%ecx
    29a1c3180:	or     $0x0,%al
    29a1c3182:	add    %ah,(%rdi)
    29a1c3184:	pushf
    29a1c3185:	or     %al,(%rax)
-   29a1c3187:	add    %ch,%al
-   29a1c3189:	sbb    (%rbx),%bl
+   29a1c3187:	add    %bl,(%rax)
+   29a1c3189:	sbb    (%rbx),%ebx
    29a1c318b:	(bad)
    29a1c318c:	add    (%rax),%al
    29a1c318e:	add    %al,(%rax)
    29a1c3190:	(bad)
    29a1c3191:	add    %al,(%rax)
    29a1c3193:	add    %al,(%rax)
    29a1c3195:	add    %al,(%rax)
    29a1c3197:	add    %bl,0x1700000a(%rsi)
    29a1c319d:	popf
    29a1c319e:	or     %al,(%rax)
    29a1c31a0:	add    %al,%bl
    29a1c31a2:	or     $0x0,%al
    29a1c31a4:	add    %bh,0x600000c(%rdi)
-   29a1c31aa:	in     (%dx),%al
-   29a1c31ab:	sbb    (%rbx),%bl
-   29a1c31ad:	(bad)
-   29a1c31ae:	add    (%rax),%al
-   29a1c31b0:	add    %al,(%rax)
+   29a1c31aa:	sbb    $0x1b,%al
+   29a1c31ac:	sbb    0x2(%rdx),%ebx
    29a1c31b2:	(bad)
    29a1c31b3:	(bad)
    29a1c31b4:	add    %al,(%rax)
    29a1c31b6:	(bad)
-   29a1c31b7:	int1
-   29a1c31b8:	sbb    (%rbx),%bl
-   29a1c31ba:	(bad)
-   29a1c31bb:	add    (%rax),%al
-   29a1c31bd:	add    %al,(%rax)
+   29a1c31b7:	and    %ebx,(%rbx)
+   29a1c31b9:	sbb    0x2(%rdx),%ebx
    29a1c31bf:	add    (%rsi),%al
    29a1c31c1:	add    %al,(%rax)
-   29a1c31c3:	sub    %al,(%rbx)
+   29a1c31c3:	sub    %dh,(%rbx)
    29a1c31c5:	sbb    (%rbx),%ebx
    29a1c31c7:	(bad)
    29a1c31c8:	add    (%rax),%al
    29a1c31ca:	add    %al,(%rax)
    29a1c31cc:	add    (%rcx),%eax
    29a1c31ce:	push   %rdx
    29a1c31cf:	add    0x0(%rax,%rax,1),%dh
    29a1c31d3:	add    %cl,(%rsi)
-   29a1c31d5:	lret   $0x1b1a
+   29a1c31d5:	cli
+   29a1c31d6:	sbb    (%rbx),%bl
    29a1c31d8:	(bad)
    29a1c31d9:	add    (%rax),%al
    29a1c31db:	add    %al,(%rax)
    29a1c31dd:	rolb   $0x0,(%rsi)
    29a1c31e0:	add    %dh,0x300000a(%rsi)
    29a1c31e6:	add    %edx,0x2(%rdx)
    29a1c31e9:	jl     29a1c31eb <.debug_info+0xab5>
    29a1c31eb:	add    %ch,(%rcx)
-   29a1c31ed:	and    %bl,(%rbx)
-   29a1c31ef:	sbb    0x2(%rdx),%ebx
+   29a1c31ed:	push   %rax
+   29a1c31ee:	sbb    (%rbx),%ebx
+   29a1c31f0:	(bad)
+   29a1c31f1:	add    (%rax),%al
+   29a1c31f3:	add    %al,(%rax)
    29a1c31f5:	lahf
    29a1c31f6:	(bad)
    29a1c31f7:	add    %al,(%rax)
    29a1c31f9:	add    (%rcx),%eax
    29a1c31fb:	push   %rdx
    29a1c31fc:	or     %eax,(%rbx)
    29a1c31fe:	movabs 0x29a1b70,%al
@@ -17293,15 +17355,15 @@
    29a1c33af:	xor    (%rax),%ah
    29a1c33b1:	sub    $0x3d647473,%eax
    29a1c33b6:	outsb  %ds:(%esi),(%dx)
    29a1c33b8:	jne    29a1c33f3 <.debug_info+0x91>
    29a1c33ba:	cmp    %eax,(%rax)
    29a1c33bc:	or     $0x9d,%al
    29a1c33be:	or     %eax,(%rax)
-   29a1c33c0:	add    %al,0x20000009(%rbp)
+   29a1c33c0:	add    %al,0x50000009(%rbp)
    29a1c33c6:	sbb    $0x29a1b,%eax
    29a1c33cb:	add    %al,(%rax)
    29a1c33cd:	testb  $0x0,(%rbx)
    29a1c33d0:	add    %al,(%rax)
    29a1c33d2:	add    %al,(%rax)
    29a1c33d4:	add    %dh,%al
    29a1c33d6:	(bad)
@@ -18583,17 +18645,18 @@
    29a1c3f32:	imul   $0x5f797261,0x72(%rdx),%esp
    29a1c3f39:	outsb  %ds:(%rsi),(%dx)
    29a1c3f3a:	(bad)
    29a1c3f3b:	insl   (%dx),%es:(%rdi)
    29a1c3f3c:	gs jae 29a1c3f3f <.debug_info+0xbdd>
    29a1c3f3f:	mov    $0x9d,%bh
    29a1c3f41:	or     (%rax),%eax
-   29a1c3f43:	add    %dl,0x20(%rax)
-   29a1c3f46:	sbb    0x2(%rdx),%ebx
-   29a1c3f4c:	movb   $0x0,(%rax)
+   29a1c3f43:	add    %al,0x29a1b20(%rax)
+   29a1c3f49:	add    %al,(%rax)
+   29a1c3f4b:	add    %al,%dh
+   29a1c3f4d:	add    %al,(%rax)
    29a1c3f4f:	add    %al,(%rax)
    29a1c3f51:	add    %al,(%rax)
    29a1c3f53:	add    %al,(%rcx)
    29a1c3f55:	pushf
    29a1c3f56:	(bad)
    29a1c3f57:	or     $0x69110000,%eax
    29a1c3f5c:	add    %dh,0xd428(%rdi)
@@ -18633,17 +18696,19 @@
    29a1c3fbd:	add    %dil,0x14909(%r13)
    29a1c3fc4:	add    %bl,(%rdi)
    29a1c3fc6:	or     $0xd170000,%eax
    29a1c3fcb:	add    %al,(%rax)
    29a1c3fcd:	(bad)
    29a1c3fce:	lahf
    29a1c3fcf:	adc    (%rax),%eax
-   29a1c3fd1:	add    %dl,0x20(%rax)
-   29a1c3fd4:	sbb    0x2(%rdx),%ebx
-   29a1c3fda:	or     %edx,0x0(%rcx,%rax,1)
+   29a1c3fd1:	add    %al,0x29a1b20(%rax)
+   29a1c3fd7:	add    %al,(%rax)
+   29a1c3fd9:	add    %cl,(%rcx)
+   29a1c3fdb:	push   %rsp
+   29a1c3fdc:	add    %eax,(%rax)
    29a1c3fde:	add    %al,%al
    29a1c3fe0:	fmull  (%rax,%rax,1)
    29a1c3fe3:	add    %al,(%rsp,%rdi,4)
    29a1c3fe6:	adc    (%rax),%eax
    29a1c3fe8:	add    %al,(%rsi)
    29a1c3fea:	push   %rsp
    29a1c3feb:	add    %eax,(%rax)
@@ -18654,17 +18719,18 @@
    29a1c3ff4:	fsts   (%rbx)
    29a1c3ff6:	add    %al,(%rax)
    29a1c3ff8:	add    %ah,%ah
    29a1c3ffa:	adc    (%rax),%eax
    29a1c3ffc:	add    %cl,(%rcx)
    29a1c3ffe:	lahf
    29a1c3fff:	adc    (%rax),%eax
-   29a1c4001:	add    %ah,0x20(%rdx)
-   29a1c4004:	sbb    0x2(%rdx),%ebx
-   29a1c400a:	add    %ah,0x0(%rcx,%rax,1)
+   29a1c4001:	add    %dl,0x29a1b20(%rdx)
+   29a1c4007:	add    %al,(%rax)
+   29a1c4009:	add    %al,(%rax)
+   29a1c400b:	add    %eax,%fs:(%rax)
    29a1c400e:	add    %cl,(%rdi)
    29a1c4010:	add    %eax,(%rsp,%rdi,4)
    29a1c4013:	adc    (%rax),%eax
    29a1c4015:	add    %al,(%rsi)
    29a1c4017:	add    %eax,%fs:(%rax)
    29a1c401a:	add    %al,(%rdx)
    29a1c401c:	(bad)
@@ -18680,20 +18746,23 @@
    29a1c4031:	add    %ch,0xd(%rdi)
    29a1c4034:	add    %al,(%rax)
    29a1c4036:	insl   (%dx),%es:(%rdi)
    29a1c4037:	or     $0x0,%eax
    29a1c403c:	add    %al,(%rax)
    29a1c403e:	sbb    %ecx,0x13(%rbp)
    29a1c4041:	add    %al,(%rax)
-   29a1c4043:	xchg   %eax,%esp
+   29a1c4043:	(bad)
    29a1c4044:	and    %bl,(%rbx)
    29a1c4046:	(bad)
    29a1c4047:	add    (%rax),%al
    29a1c4049:	add    %al,(%rax)
-   29a1c404b:	add    %edx,0x29a1b(%rax,%riz,1)
+   29a1c404b:	add    %eax,%esp
+   29a1c404d:	and    %bl,(%rbx)
+   29a1c404f:	(bad)
+   29a1c4050:	add    (%rax),%al
    29a1c4052:	add    %al,(%rax)
    29a1c4054:	rex.WX add %al,(%rax)
    29a1c4057:	add    %al,(%rax)
    29a1c4059:	add    %al,(%rax)
    29a1c405b:	add    %cl,%cl
    29a1c405d:	(bad)
    29a1c405e:	adc    %dh,0x13(%rcx)
@@ -18724,18 +18793,16 @@
    29a1c40aa:	rex.XB jne 29a1c411f <.debug_info+0xdbd>
    29a1c40ad:	jb     29a1c4114 <.debug_info+0xdb2>
    29a1c40af:	outsb  %ds:(%rsi),(%dx)
    29a1c40b0:	je     29a1c40fb <.debug_info+0xd99>
    29a1c40b2:	insl   (%dx),%es:(%rdi)
    29a1c40b3:	(bad)
    29a1c40b4:	add    %ah,%gs:0x11f(%ebx)
-   29a1c40bc:	rcrb   $0x1b,(%rdi)
-   29a1c40bf:	(bad)
-   29a1c40c0:	add    (%rax),%al
-   29a1c40c2:	add    %al,(%rax)
+   29a1c40bc:	lock (bad)
+   29a1c40be:	sbb    0x2(%rdx),%ebx
    29a1c40c4:	mov    %eax,(%rax)
    29a1c40c6:	add    %al,(%rax)
    29a1c40c8:	add    %al,(%rax)
    29a1c40ca:	add    %al,(%rax)
    29a1c40cc:	add    %ebx,0x1100000e(%rdx,%rcx,4)
    29a1c40d3:	jo     29a1c4129 <.debug_info+0xdc7>
    29a1c40d5:	(bad)
@@ -18761,15 +18828,15 @@
    29a1c4118:	add    (%rsi),%ecx
    29a1c411a:	add    %al,(%rax)
    29a1c411c:	add    %ecx,(%rsi)
    29a1c411e:	add    %al,(%rax)
    29a1c4120:	(bad)
    29a1c4121:	lahf
    29a1c4122:	adc    (%rax),%eax
-   29a1c4124:	add    %al,%al
+   29a1c4124:	add    %dh,%al
    29a1c4126:	(bad)
    29a1c4127:	sbb    0x2(%rdx),%ebx
    29a1c412d:	(bad)
    29a1c412e:	cmp    %eax,(%rcx)
    29a1c4130:	add    %al,(%rax)
    29a1c4132:	stos   %al,%es:(%rdi)
    29a1c4133:	(bad)
@@ -18786,17 +18853,19 @@
    29a1c4147:	fsts   (%rbx)
    29a1c4149:	add    %al,(%rax)
    29a1c414b:	add    %ah,%ah
    29a1c414d:	adc    (%rax),%eax
    29a1c414f:	add    %cl,(%rcx)
    29a1c4151:	lahf
    29a1c4152:	adc    (%rax),%eax
-   29a1c4154:	add    %dl,%al
-   29a1c4156:	(bad)
-   29a1c4157:	sbb    0x2(%rdx),%ebx
+   29a1c4154:	add    %al,(%rax)
+   29a1c4156:	and    %bl,(%rbx)
+   29a1c4158:	(bad)
+   29a1c4159:	add    (%rax),%al
+   29a1c415b:	add    %al,(%rax)
    29a1c415d:	add    %cl,0x1(%rcx)
    29a1c4160:	add    %al,(%rax)
    29a1c4162:	sgdt   (%rsp,%rdi,4)
    29a1c4166:	adc    (%rax),%eax
    29a1c4168:	add    %al,(%rsi)
    29a1c416a:	add    %rax,(%r8)
    29a1c416d:	add    %al,(%rdx)
@@ -18817,19 +18886,17 @@
    29a1c4189:	(bad)
    29a1c418a:	(bad)
    29a1c418b:	add    %al,(%rax)
    29a1c418d:	add    %al,(%rax)
    29a1c418f:	add    %al,(%rax)
    29a1c4191:	sbb    %ecx,0x13(%rbp)
    29a1c4194:	add    %al,(%rax)
-   29a1c4196:	hlt
-   29a1c4197:	(bad)
+   29a1c4196:	and    $0x20,%al
    29a1c4198:	sbb    0x2(%rdx),%ebx
-   29a1c419e:	add    %esi,%esp
-   29a1c41a0:	(bad)
+   29a1c419e:	add    %esp,(%rax,%riz,1)
    29a1c41a1:	sbb    0x2(%rdx),%ebx
    29a1c41a7:	rex.WB add %al,(%r8)
    29a1c41aa:	add    %al,(%rax)
    29a1c41ac:	add    %al,(%rax)
    29a1c41ae:	add    %ch,0x1371100e(%rbp)
    29a1c41b4:	add    %al,(%rax)
    29a1c41b6:	sub    $0xe,%al
@@ -18860,32 +18927,30 @@
    29a1c41f1:	push   %rax
    29a1c41f2:	rex.RB
    29a1c41f3:	rex.WB insl (%dx),%es:(%rdi)
    29a1c41f5:	(bad)
    29a1c41f6:	addr32 gs rex.X (bad)
    29a1c41fa:	jae    29a1c4261 <.debug_info+0xeff>
    29a1c41fc:	add    %dl,0x160(%rdi)
-   29a1c4202:	sbbb   $0x1b,(%rdi)
-   29a1c4205:	(bad)
-   29a1c4206:	add    (%rax),%al
-   29a1c4208:	add    %al,(%rax)
+   29a1c4202:	mov    $0x1f,%al
+   29a1c4204:	sbb    0x2(%rdx),%ebx
    29a1c420a:	ss add %al,(%rax)
    29a1c420d:	add    %al,(%rax)
    29a1c420f:	add    %al,(%rax)
    29a1c4211:	add    %al,(%rcx)
    29a1c4213:	pushf
    29a1c4214:	xor    %cl,(%rdi)
    29a1c4216:	add    %al,(%rax)
    29a1c4218:	or     %al,%dl
    29a1c421a:	add    %al,(%rax)
    29a1c421c:	add    %bl,0x16009(%rcx)
    29a1c4222:	add    %cl,(%rcx)
    29a1c4224:	lahf
    29a1c4225:	adc    (%rax),%eax
-   29a1c4227:	add    %al,0x29a1b1f(%rax)
+   29a1c4227:	add    %dh,0x29a1b1f(%rax)
    29a1c422d:	add    %al,(%rax)
    29a1c422f:	add    %al,(%rsi,%rbx,1)
    29a1c4232:	add    %eax,(%rax)
    29a1c4234:	add    %bl,0x13bc0409(%rbx)
    29a1c423a:	add    %al,(%rax)
    29a1c423c:	(bad)
    29a1c423d:	(bad)
@@ -18897,18 +18962,19 @@
    29a1c4247:	fsts   (%rbx)
    29a1c4249:	add    %al,(%rax)
    29a1c424b:	add    %ah,%ah
    29a1c424d:	adc    (%rax),%eax
    29a1c424f:	add    %cl,(%rcx)
    29a1c4251:	lahf
    29a1c4252:	adc    (%rax),%eax
-   29a1c4254:	add    %dl,0x29a1b1f(%rax)
-   29a1c425a:	add    %al,(%rax)
-   29a1c425c:	add    %al,(%rax)
-   29a1c425e:	cs add %eax,(%rax)
+   29a1c4254:	add    %al,%al
+   29a1c4256:	(bad)
+   29a1c4257:	sbb    0x2(%rdx),%ebx
+   29a1c425d:	add    %ch,(%rsi)
+   29a1c425f:	add    %eax,(%rax)
    29a1c4261:	add    %cl,(%rdi)
    29a1c4263:	add    %eax,(%rsp,%rdi,4)
    29a1c4266:	adc    (%rax),%eax
    29a1c4268:	add    %al,(%rsi)
    29a1c426a:	cs add %eax,(%rax)
    29a1c426d:	add    %al,(%rdx)
    29a1c426f:	(bad)
@@ -18935,15 +19001,15 @@
    29a1c4299:	rex.RB push %r11
    29a1c429b:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
    29a1c42a0:	outsb  %ds:(%rsi),(%dx)
    29a1c42a1:	rex.RB js 29a1c4309 <.debug_info+0xfa7>
    29a1c42a4:	movsxd (%rax),%eax
    29a1c42a6:	jns    29a1c4306 <.debug_info+0xfa4>
    29a1c42a8:	or     (%rax),%al
-   29a1c42aa:	add    %al,(%rax)
+   29a1c42aa:	add    %dh,(%rax)
    29a1c42ac:	(bad)
    29a1c42ad:	sbb    0x2(%rdx),%ebx
    29a1c42b3:	jae    29a1c42b5 <.debug_info+0xf53>
    29a1c42b5:	add    %al,(%rax)
    29a1c42b7:	add    %al,(%rax)
    29a1c42b9:	add    %al,(%rax)
    29a1c42bb:	add    %ebx,0x11000010(%rbp,%riz,1)
@@ -18985,15 +19051,15 @@
    29a1c430e:	add    %al,(%rax)
    29a1c4310:	fwait
    29a1c4311:	(bad)
    29a1c4312:	add    %al,(%rax)
    29a1c4314:	cltd
    29a1c4315:	(bad)
    29a1c4316:	add    %al,(%rax)
-   29a1c4318:	or     %ebx,0x13(%rdi)
+   29a1c4318:	or     %ebx,0x30000013(%rdi)
    29a1c431e:	(bad)
    29a1c431f:	sbb    0x2(%rdx),%ebx
    29a1c4325:	or     %al,(%rbx)
    29a1c4327:	add    %eax,(%rax)
    29a1c4329:	add    %al,0x13bc0409(%rcx)
    29a1c432f:	add    %al,(%rax)
    29a1c4331:	(bad)
@@ -19005,16 +19071,15 @@
    29a1c433c:	fsts   (%rbx)
    29a1c433e:	add    %al,(%rax)
    29a1c4340:	add    %ah,%ah
    29a1c4342:	adc    (%rax),%eax
    29a1c4344:	add    %cl,(%rcx)
    29a1c4346:	lahf
    29a1c4347:	adc    (%rax),%eax
-   29a1c4349:	add    %dl,(%rcx)
-   29a1c434b:	(bad)
+   29a1c4349:	add    %al,0x1f(%rcx)
    29a1c434c:	sbb    0x2(%rdx),%ebx
    29a1c4352:	add    %dl,(%rbx)
    29a1c4354:	add    %eax,(%rax)
    29a1c4356:	add    %cl,(%rdi)
    29a1c4358:	add    %eax,(%rsp,%rdi,4)
    29a1c435b:	adc    (%rax),%eax
    29a1c435d:	add    %al,(%rsi)
@@ -19045,15 +19110,15 @@
    29a1c4394:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
    29a1c4399:	outsb  %ds:(%rsi),(%dx)
    29a1c439a:	rex.XB outsl %ds:(%rsi),(%dx)
    29a1c439c:	jne    29a1c440c <.debug_info+0x10aa>
    29a1c439e:	je     29a1c43a0 <.debug_info+0x103e>
    29a1c43a0:	addr32 (bad)
    29a1c43a2:	add    %al,(%rax)
-   29a1c43a4:	add    %al,%al
+   29a1c43a4:	add    %dh,%al
    29a1c43a6:	(bad)
    29a1c43a7:	sbb    0x2(%rdx),%ebx
    29a1c43ad:	(bad)
    29a1c43ae:	add    %al,(%rax)
    29a1c43b0:	add    %al,(%rax)
    29a1c43b2:	add    %al,(%rax)
    29a1c43b4:	add    %al,(%rcx)
@@ -19071,15 +19136,15 @@
    29a1c43cb:	push   $0x15
    29a1c43cd:	adc    $0xc5000009,%eax
    29a1c43d2:	(bad)
    29a1c43d3:	add    %al,(%rax)
    29a1c43d5:	ret
    29a1c43d6:	(bad)
    29a1c43d7:	add    %al,(%rax)
-   29a1c43d9:	or     %ebx,-0x3fffffed(%rdi)
+   29a1c43d9:	or     %ebx,-0xfffffed(%rdi)
    29a1c43df:	(bad)
    29a1c43e0:	sbb    0x2(%rdx),%ebx
    29a1c43e6:	add    $0xe8,%eax
    29a1c43eb:	insl   (%dx),%es:(%rdi)
    29a1c43ec:	or     %eax,(%rsp,%rdi,4)
    29a1c43ef:	adc    (%rax),%eax
    29a1c43f1:	add    %al,(%rsi)
@@ -19090,15 +19155,15 @@
    29a1c43fd:	fsts   (%rbx)
    29a1c43ff:	add    %al,(%rax)
    29a1c4401:	add    %ah,%ah
    29a1c4403:	adc    (%rax),%eax
    29a1c4405:	add    %cl,(%rcx)
    29a1c4407:	lahf
    29a1c4408:	adc    (%rax),%eax
-   29a1c440a:	add    %dl,%al
+   29a1c440a:	add    %al,(%rax)
    29a1c440c:	(bad)
    29a1c440d:	sbb    0x2(%rdx),%ebx
    29a1c4413:	add    %bh,%al
    29a1c4415:	add    %al,(%rax)
    29a1c4417:	add    %cl,(%rdi)
    29a1c4419:	add    %eax,(%rsp,%rdi,4)
    29a1c441c:	adc    (%rax),%eax
@@ -19133,15 +19198,15 @@
    29a1c445a:	outsb  %ds:(%rsi),(%dx)
    29a1c445b:	rex.RX outsl %ds:(%rsi),(%dx)
    29a1c445d:	jb     29a1c44a0 <.debug_info+0x113e>
    29a1c445f:	fs fs jb 29a1c44c8 <.debug_info+0x1166>
    29a1c4463:	jae    29a1c44d8 <.debug_info+0x1176>
    29a1c4465:	add    %bl,0x5e(%rcx)
    29a1c4468:	or     (%rax),%al
-   29a1c446a:	add    %al,0x1e(%rax)
+   29a1c446a:	add    %dh,0x1e(%rax)
    29a1c446d:	sbb    0x2(%rdx),%ebx
    29a1c4473:	addb   $0x0,(%rax)
    29a1c4476:	add    %al,(%rax)
    29a1c4478:	add    %al,(%rax)
    29a1c447a:	add    %al,(%rcx)
    29a1c447c:	pushf
    29a1c447d:	adc    $0x12,%al
@@ -19167,15 +19232,15 @@
    29a1c44a8:	sbb    %ecx,(%rdi)
    29a1c44aa:	add    %al,(%rax)
    29a1c44ac:	(bad)
    29a1c44ad:	sldt   (%rax)
    29a1c44b0:	(bad)
    29a1c44b1:	lahf
    29a1c44b2:	adc    (%rax),%eax
-   29a1c44b4:	add    %al,0x1e(%rax)
+   29a1c44b4:	add    %dh,0x1e(%rax)
    29a1c44b7:	sbb    0x2(%rdx),%ebx
    29a1c44bd:	(bad)
    29a1c44be:	ret    $0x0
    29a1c44c1:	add    %bl,-0x41(%rdi)
    29a1c44c4:	adc    %eax,(%rax)
    29a1c44c6:	add    %al,(%rsp,%rdi,4)
    29a1c44c9:	adc    (%rax),%eax
@@ -19188,20 +19253,20 @@
    29a1c44d7:	fsts   (%rbx)
    29a1c44d9:	add    %al,(%rax)
    29a1c44db:	add    %ah,%ah
    29a1c44dd:	adc    (%rax),%eax
    29a1c44df:	add    %cl,(%rcx)
    29a1c44e1:	lahf
    29a1c44e2:	adc    (%rax),%eax
-   29a1c44e4:	add    %dl,0x1e(%rax)
-   29a1c44e7:	sbb    0x2(%rdx),%ebx
-   29a1c44ed:	add    %dl,%dl
-   29a1c44ef:	add    %al,(%rax)
-   29a1c44f1:	add    %cl,(%rdi)
-   29a1c44f3:	add    %eax,(%rsp,%rdi,4)
+   29a1c44e4:	add    %al,0x29a1b1e(%rax)
+   29a1c44ea:	add    %al,(%rax)
+   29a1c44ec:	add    %al,(%rax)
+   29a1c44ee:	rolb   %cl,(%rax)
+   29a1c44f0:	add    %al,(%rax)
+   29a1c44f2:	sgdt   (%rsp,%rdi,4)
    29a1c44f6:	adc    (%rax),%eax
    29a1c44f8:	add    %al,(%rsi)
    29a1c44fa:	rolb   %cl,(%rax)
    29a1c44fc:	add    %al,(%rax)
    29a1c44fe:	add    %bh,%al
    29a1c4500:	adc    (%rax),%eax
    29a1c4502:	add    %al,(%rbx)
@@ -19215,19 +19280,20 @@
    29a1c4516:	sldt   (%rax)
    29a1c4519:	xor    $0xf,%al
    29a1c451b:	add    %al,(%rax)
    29a1c451d:	add    %al,(%rax)
    29a1c451f:	add    %al,(%rax)
    29a1c4521:	or     %ecx,0x13(%rbp)
    29a1c4524:	add    %al,(%rax)
-   29a1c4526:	jns    29a1c4546 <.debug_info+0x11e4>
-   29a1c4528:	sbb    0x2(%rdx),%ebx
-   29a1c452e:	add    %ebx,%ebp
-   29a1c4530:	add    %al,(%rax)
-   29a1c4532:	add    %ah,0xa(%rbx)
+   29a1c4526:	test   $0x29a1b1e,%eax
+   29a1c452b:	add    %al,(%rax)
+   29a1c452d:	add    %al,(%rcx)
+   29a1c452f:	fldl   (%rax)
+   29a1c4531:	add    %al,(%rax)
+   29a1c4533:	movsxd (%rdx),%ecx
    29a1c4535:	adc    %dh,0x13(%rcx)
    29a1c4538:	add    %al,(%rax)
    29a1c453a:	rex.X sldt (%rax)
    29a1c453e:	rex sldt (%rax)
    29a1c4542:	add    $0x66,%al
    29a1c4544:	adc    (%rax),%eax
    29a1c4546:	add    %al,(%rsi)
@@ -19253,17 +19319,20 @@
    29a1c4584:	outsb  %ds:(%rsi),(%dx)
    29a1c4585:	rex.X jns 29a1c45d6 <.debug_info+0x1274>
    29a1c4588:	(bad)
    29a1c4589:	insl   (%dx),%es:(%rdi)
    29a1c458a:	add    %bh,%gs:(%rdx)
    29a1c458d:	pop    %rsi
    29a1c458e:	or     (%rax),%al
-   29a1c4590:	add    %ah,0x29a1b1d(%rax)
-   29a1c4596:	add    %al,(%rax)
-   29a1c4598:	add    %bl,0x0(%rbp)
+   29a1c4590:	add    %dl,%al
+   29a1c4592:	sbb    $0x29a1b,%eax
+   29a1c4597:	add    %al,(%rax)
+   29a1c4599:	popf
+   29a1c459a:	add    %al,(%rax)
+   29a1c459c:	add    %al,(%rax)
    29a1c459e:	add    %al,(%rax)
    29a1c45a0:	add    %al,(%rcx)
    29a1c45a2:	pushf
    29a1c45a3:	adc    (%r8),%r8
    29a1c45a6:	add    %dl,(%rcx)
    29a1c45a8:	jo     29a1c45f8 <.debug_info+0x1296>
    29a1c45aa:	(bad)
@@ -19297,37 +19366,36 @@
    29a1c45f7:	add    %cl,%cl
    29a1c45f9:	sldt   (%rax)
    29a1c45fc:	(bad)
    29a1c45fd:	sldt   (%rax)
    29a1c4600:	(bad)
    29a1c4601:	lahf
    29a1c4602:	adc    (%rax),%eax
-   29a1c4604:	add    %dh,0x29a1b1d(%rbp)
-   29a1c460a:	add    %al,(%rax)
-   29a1c460c:	add    %al,(%rdx)
-   29a1c460e:	mov    $0x0,%bh
-   29a1c4610:	add    %al,(%rax)
-   29a1c4612:	rex.RX adc $0x4000013,%eax
+   29a1c4604:	add    %ah,%ch
+   29a1c4606:	sbb    $0x29a1b,%eax
+   29a1c460b:	add    %al,(%rax)
+   29a1c460d:	add    0x46000000(%rdi),%dh
+   29a1c4613:	adc    $0x4000013,%eax
    29a1c4618:	mov    $0x6000013,%esp
    29a1c461d:	mov    $0x0,%bh
    29a1c461f:	add    %al,(%rax)
    29a1c4621:	add    %bh,%al
    29a1c4623:	adc    (%rax),%eax
    29a1c4625:	add    %al,(%rdx)
    29a1c4627:	fsts   (%rbx)
    29a1c4629:	add    %al,(%rax)
    29a1c462b:	add    %ah,%ah
    29a1c462d:	adc    (%rax),%eax
    29a1c462f:	add    %bl,(%rcx)
    29a1c4631:	lahf
    29a1c4632:	adc    (%rax),%eax
-   29a1c4634:	add    %al,%ch
+   29a1c4634:	add    %dh,%ch
    29a1c4636:	sbb    $0x29a1b,%eax
    29a1c463b:	add    %al,(%rax)
-   29a1c463d:	add    %al,%ch
+   29a1c463d:	add    %dh,%ch
    29a1c463f:	sbb    $0x29a1b,%eax
    29a1c4644:	add    %al,(%rax)
    29a1c4646:	(bad)
    29a1c4647:	add    %al,(%rax)
    29a1c4649:	add    %al,(%rax)
    29a1c464b:	add    %al,(%rax)
    29a1c464d:	add    %cl,(%rdi)
@@ -19347,22 +19415,21 @@
    29a1c4669:	adc    (%rax),%eax
    29a1c466b:	add    %bl,%dh
    29a1c466d:	sldt   (%rax)
    29a1c4670:	fmull  (%rdi)
    29a1c4672:	add    %al,(%rax)
    29a1c4674:	add    %al,(%rax)
    29a1c4676:	add    %ah,(%rsi)
-   29a1c4678:	scas   %es:(%rdi),%eax
-   29a1c4679:	sbb    $0x29a1b,%eax
+   29a1c4678:	fistps 0x29a1b(%rip)        # 29a1ee099 <.debug_rnglists+0x1dff5>
    29a1c467e:	add    %al,(%rax)
    29a1c4680:	movabs %al,0x170000132d00000b
    29a1c4689:	add    %edx,0x2(%rdx)
    29a1c468c:	je     29a1c468e <.debug_info+0x132c>
    29a1c468e:	add    %ah,(%rdi)
-   29a1c4690:	sbb    (%rsi),%bl
+   29a1c4690:	rex.WX (bad)
    29a1c4692:	sbb    0x2(%rdx),%ebx
    29a1c4698:	jp     29a1c46a5 <.debug_info+0x1343>
    29a1c469a:	add    %al,(%rax)
    29a1c469c:	(bad)
    29a1c469d:	add    %edx,0x2(%rdx)
    29a1c46a0:	jae    29a1c46a2 <.debug_info+0x1340>
    29a1c46a2:	(bad)
@@ -19432,17 +19499,16 @@
    29a1c474e:	fs gs jb 29a1c4752 <.debug_info+0x13f0>
    29a1c4752:	adc    (%rdx),%ebx
    29a1c4754:	jbe    29a1c475e <.debug_info+0x13fc>
    29a1c4756:	add    %al,(%rax)
    29a1c4758:	add    %ch,(%rcx)
    29a1c475a:	lahf
    29a1c475b:	adc    (%rax),%eax
-   29a1c475d:	add    %ah,(%rax)
-   29a1c475f:	sbb    $0x29a1b,%eax
-   29a1c4764:	add    %al,(%rax)
+   29a1c475d:	add    %dl,0x1d(%rax)
+   29a1c4760:	sbb    0x2(%rdx),%ebx
    29a1c4766:	sub    $0x0,%al
    29a1c4768:	add    %al,(%rax)
    29a1c476a:	add    %al,(%rax)
    29a1c476c:	add    %al,(%rax)
    29a1c476e:	add    %ebx,0x10000014(%rsi,%rdi,2)
    29a1c4775:	mov    $0xec000013,%esp
    29a1c477a:	sldt   (%rax)
@@ -19454,15 +19520,15 @@
    29a1c478a:	cli
    29a1c478b:	sldt   (%rax)
    29a1c478e:	add    %cl,%bl
    29a1c4790:	adc    (%rax),%eax
    29a1c4792:	add    %al,(%rdx)
    29a1c4794:	in     $0x13,%al
    29a1c4796:	add    %al,(%rax)
-   29a1c4798:	or     %ebx,0x29000013(%rdi)
+   29a1c4798:	or     %ebx,0x59000013(%rdi)
    29a1c479e:	sbb    $0x29a1b,%eax
    29a1c47a3:	add    %al,(%rax)
    29a1c47a5:	add    %dh,0xf000000(%rax)
    29a1c47ab:	add    %edx,(%rax)
    29a1c47ad:	mov    $0x12000013,%esp
    29a1c47b2:	adc    %al,(%rax)
    29a1c47b4:	add    %cl,(%rax,%rdx,1)
@@ -19485,25 +19551,20 @@
    29a1c47d6:	adc    %al,(%rax)
    29a1c47d8:	add    %dh,(%rdi)
    29a1c47da:	adc    %al,(%rax)
    29a1c47dc:	add    %al,(%rax)
    29a1c47de:	add    %al,(%rax)
    29a1c47e0:	sub    0x13(%rbp),%cl
    29a1c47e3:	add    %al,(%rax)
-   29a1c47e5:	push   %rax
-   29a1c47e6:	sbb    $0x29a1b,%eax
-   29a1c47eb:	add    %al,(%rax)
-   29a1c47ed:	push   %rax
-   29a1c47ee:	add    %al,(%rax)
-   29a1c47f0:	add    %al,(%rax)
-   29a1c47f2:	add    %al,(%rax)
-   29a1c47f4:	add    %al,(%rcx)
-   29a1c47f6:	pushf
-   29a1c47f7:	adc    %ah,0x13(%rsi)
-   29a1c47fa:	add    %al,(%rax)
+   29a1c47e5:	sbbb   $0x0,0x29a1b(%rip)        # 29a1ee207 <.debug_rnglists+0x1e163>
+   29a1c47ec:	add    %dl,0x0(%rax)
+   29a1c47ef:	add    %al,(%rax)
+   29a1c47f1:	add    %al,(%rax)
+   29a1c47f3:	add    %al,(%rax)
+   29a1c47f5:	add    %ebx,0x1366(%rax,%rdx,1)
    29a1c47fc:	adc    %r8b,(%r8)
    29a1c47ff:	add    %al,0x10(%rcx)
    29a1c4802:	add    %al,(%rax)
    29a1c4804:	sub    0x13(%rcx),%esi
    29a1c4807:	add    %al,(%rax)
    29a1c4809:	add    %edx,0x3(%rcx)
    29a1c480c:	jge    29a1c4821 <.debug_info+0x14bf>
@@ -19555,30 +19616,36 @@
    29a1c4888:	outsb  %ds:(%esi),(%dx)
    29a1c488a:	jne    29a1c48c5 <.debug_info+0x91>
    29a1c488c:	cmp    %eax,(%rax)
    29a1c488e:	or     $0x82,%al
    29a1c4890:	or     (%rax),%al
    29a1c4892:	add    %ch,0xa(%rdx)
    29a1c4895:	add    %al,(%rax)
-   29a1c4897:	and    %ah,(%rcx)
-   29a1c4899:	sbb    0x2(%rdx),%ebx
+   29a1c4897:	push   %rax
+   29a1c4898:	and    %ebx,(%rbx)
+   29a1c489a:	(bad)
+   29a1c489b:	add    (%rax),%al
+   29a1c489d:	add    %al,(%rax)
    29a1c489f:	add    (%rax),%eax
    29a1c48a1:	add    %al,(%rax)
    29a1c48a3:	add    %al,(%rax)
    29a1c48a5:	add    %al,(%rax)
    29a1c48a7:	cmp    (%rax,%rax,1),%edx
    29a1c48aa:	add    %al,(%rdx)
    29a1c48ac:	pop    %rdi
    29a1c48ad:	data16 jo 29a1c4922 <.debug_info+0x57>
    29a1c48b0:	gs jae 29a1c4918 <.debug_info+0x4d>
    29a1c48b3:	je     29a1c48b5 <.debug_info+0x81>
    29a1c48b5:	add    %ecx,(%rcx)
    29a1c48b7:	(bad)
-   29a1c48b8:	and    %ah,(%rcx)
-   29a1c48ba:	sbb    0x2(%rdx),%ebx
+   29a1c48b8:	push   %rax
+   29a1c48b9:	and    %ebx,(%rbx)
+   29a1c48bb:	(bad)
+   29a1c48bc:	add    (%rax),%al
+   29a1c48be:	add    %al,(%rax)
    29a1c48c0:	add    (%rax),%eax
    29a1c48c2:	add    %al,(%rax)
    29a1c48c4:	add    %al,(%rax)
    29a1c48c6:	add    %al,(%rax)
    29a1c48c8:	add    %ebx,0x1f6(%rax,%rax,1)
 
 000000029a1c48cb <.debug_info>:
@@ -19610,17 +19677,17 @@
    29a1c491f:	outsb  %ds:(%esi),(%dx)
    29a1c4921:	jne    29a1c495c <.debug_info+0x91>
    29a1c4923:	cmp    %eax,(%rax)
    29a1c4925:	or     $0x9,%al
    29a1c4927:	or     (%rax),%eax
    29a1c4929:	add    %bh,(%rbx)
    29a1c492b:	or     (%rax),%eax
-   29a1c492d:	add    %dh,0x21(%rax)
-   29a1c4930:	sbb    0x2(%rdx),%ebx
-   29a1c4936:	(bad)
+   29a1c492d:	add    %ah,0x29a1b21(%rax)
+   29a1c4933:	add    %al,(%rax)
+   29a1c4935:	add    %al,(%rsi)
    29a1c4937:	add    %al,(%rax)
    29a1c4939:	add    %al,(%rax)
    29a1c493b:	add    %al,(%rax)
    29a1c493d:	add    %dl,0x1000014(%rbx)
    29a1c4943:	add    %eax,(%rsi)
    29a1c4945:	movsxd 0x61(%rax),%ebp
    29a1c4948:	jb     29a1c494a <.debug_info+0x7f>
@@ -19739,17 +19806,15 @@
    29a1c4a65:	rex.RB outsb %ds:(%rsi),(%dx)
    29a1c4a67:	je     29a1c4adb <.debug_info+0x16>
    29a1c4a69:	jns    29a1c4abb <.debug_info+0x1f0>
    29a1c4a6b:	outsl  %ds:(%rsi),(%dx)
    29a1c4a6c:	imul   $0xd0d0100,0x74(%rsi),%ebp
    29a1c4a73:	or     (%rcx),%eax
    29a1c4a75:	add    %al,(%rax)
-   29a1c4a77:	jo     29a1c4a9a <.debug_info+0x1cf>
-   29a1c4a79:	sbb    0x2(%rdx),%ebx
-   29a1c4a7f:	(bad)
+   29a1c4a77:	movabs 0x6000000029a1b21,%al
    29a1c4a80:	add    %al,(%rax)
    29a1c4a82:	add    %al,(%rax)
    29a1c4a84:	add    %al,(%rax)
    29a1c4a86:	add    %al,(%rcx)
    29a1c4a88:	pushf
    29a1c4a89:	add    0x44(%rax),%ebp
    29a1c4a8c:	insb   (%dx),%es:(%rdi)
@@ -19808,15 +19873,15 @@
    29a1c4b19:	outsb  %ds:(%esi),(%dx)
    29a1c4b1b:	jne    29a1c4b56 <.debug_info+0x91>
    29a1c4b1d:	cmp    %eax,(%rax)
    29a1c4b1f:	or     $0xef,%al
    29a1c4b21:	or     (%rax),%eax
    29a1c4b23:	add    %dl,%bh
    29a1c4b25:	or     (%rax),%eax
-   29a1c4b27:	add    %al,0x29a1b21(%rax)
+   29a1c4b27:	add    %dh,0x29a1b21(%rax)
    29a1c4b2d:	add    %al,(%rax)
    29a1c4b2f:	add    %al,(%rsi)
    29a1c4b31:	add    %al,(%rax)
    29a1c4b33:	add    %al,(%rax)
    29a1c4b35:	add    %al,(%rax)
    29a1c4b37:	add    %bh,%dl
    29a1c4b39:	adc    $0x0,%al
@@ -19935,15 +20000,15 @@
    29a1c4c56:	(bad)
    29a1c4c5b:	(bad)
    29a1c4c5c:	rex.R insb (%dx),%es:(%rdi)
    29a1c4c5e:	insb   (%dx),%es:(%rdi)
    29a1c4c5f:	rex.WRB (bad)
    29a1c4c61:	imul   $0xb128804,0x0(%rsi),%ebp
    29a1c4c68:	add    %eax,(%rax)
-   29a1c4c6a:	add    %al,0x29a1b21(%rax)
+   29a1c4c6a:	add    %dh,0x29a1b21(%rax)
    29a1c4c70:	add    %al,(%rax)
    29a1c4c72:	add    %al,(%rsi)
    29a1c4c74:	add    %al,(%rax)
    29a1c4c76:	add    %al,(%rax)
    29a1c4c78:	add    %al,(%rax)
    29a1c4c7a:	add    %al,(%rcx)
    29a1c4c7c:	pushf
@@ -20002,15 +20067,15 @@
    29a1c4d06:	xor    (%rax),%ah
    29a1c4d08:	sub    $0x3d647473,%eax
    29a1c4d0d:	outsb  %ds:(%esi),(%dx)
    29a1c4d0f:	jne    29a1c4d4a <.debug_info+0x91>
    29a1c4d11:	cmp    %eax,(%rax)
    29a1c4d13:	or     $0xc4,%al
    29a1c4d15:	or     $0x0,%al
-   29a1c4d17:	add    %ch,0x21900000(%rsp,%rcx,1)
+   29a1c4d17:	add    %ch,0x21c00000(%rsp,%rcx,1)
    29a1c4d1e:	sbb    0x2(%rdx),%ebx
    29a1c4d24:	(bad)
    29a1c4d25:	add    %al,(%rax)
    29a1c4d27:	add    %al,(%rax)
    29a1c4d29:	add    %al,(%rax)
    29a1c4d2b:	add    %ah,0x0(%rbp,%rdx,1)
    29a1c4d2f:	add    %al,(%rsi)
@@ -20291,16 +20356,15 @@
    29a1c4fbc:	mov    $0x0,%bl
    29a1c4fbe:	add    %al,(%rax)
    29a1c4fc0:	add    %dl,0x72706676(%rip)        # 30c8cb63c <.debug_rnglists+0x726fb598>
    29a1c4fc6:	imul   $0x6040066,0x74(%rsi),%ebp
    29a1c4fcd:	add    (%rdi),%cl
    29a1c4fcf:	or     %eax,(%rcx)
    29a1c4fd1:	add    %al,(%rax)
-   29a1c4fd3:	nop
-   29a1c4fd4:	and    %ebx,(%rbx)
+   29a1c4fd3:	shlb   $0x1b,(%rcx)
    29a1c4fd6:	(bad)
    29a1c4fd7:	add    (%rax),%al
    29a1c4fd9:	add    %al,(%rax)
    29a1c4fdb:	(bad)
    29a1c4fdc:	add    %al,(%rax)
    29a1c4fde:	add    %al,(%rax)
    29a1c4fe0:	add    %al,(%rax)
@@ -20330,18 +20394,17 @@
    29a1c5014:	imul   $0xb35a00,0x74(%rbx),%r14
    29a1c501c:	add    %al,(%rax)
    29a1c501e:	or     (%rcx),%dl
    29a1c5020:	add    %al,(%rax)
    29a1c5022:	add    $0x11,%al
    29a1c5024:	add    %al,(%rax)
    29a1c5026:	(bad)
-   29a1c5027:	test   $0x29a1b21,%eax
-   29a1c502c:	add    %al,(%rax)
-   29a1c502e:	add    %cl,%dl
-   29a1c5030:	add    (%rax),%al
+   29a1c5027:	fldenv (%rcx)
+   29a1c5029:	sbb    0x2(%rdx),%ebx
+   29a1c502f:	lret   $0x2
    29a1c5032:	add    %al,0x30015201(%rip)        # 2ca1da239 <.debug_rnglists+0x3000a195>
    29a1c5038:	add    $0xa3035101,%eax
    29a1c503d:	add    %edx,0x5(%rdx)
    29a1c5040:	add    %ebx,0x3(%rax)
    29a1c5043:	movabs %eax,0x530015901055101
    29a1c504c:	add    0x20(%rdi),%dh
    29a1c504f:	add    0x5801(%rbx),%esp
@@ -20377,15 +20440,15 @@
    29a1c50a5:	sub    $0x3d647473,%eax
    29a1c50aa:	outsb  %ds:(%esi),(%dx)
    29a1c50ac:	jne    29a1c50e7 <.debug_info+0x91>
    29a1c50ae:	cmp    %eax,(%rax)
    29a1c50b0:	or     $0xac,%al
    29a1c50b2:	or     $0xd940000,%eax
    29a1c50b7:	add    %al,(%rax)
-   29a1c50b9:	mov    $0x21,%al
+   29a1c50b9:	loopne 29a1c50dc <.debug_info+0x86>
    29a1c50bb:	sbb    0x2(%rdx),%ebx
    29a1c50c1:	(bad)
    29a1c50c2:	add    (%rax),%al
    29a1c50c4:	add    %al,(%rax)
    29a1c50c6:	add    %al,(%rax)
    29a1c50c8:	add    %dl,%dh
    29a1c50ca:	adc    $0x5f0b0000,%eax
@@ -21906,19 +21969,16 @@
    29a1c5d5f:	jb     29a1c5dca <.debug_info+0xd74>
    29a1c5d61:	outsb  %ds:(%rsi),(%dx)
    29a1c5d62:	je     29a1c5dca <.debug_info+0xd74>
    29a1c5d64:	add    %cl,(%rbx)
    29a1c5d66:	and    (%rdi,%rcx,1),%eax
    29a1c5d69:	(bad)
    29a1c5d6a:	add    %eax,(%rax)
-   29a1c5d6c:	add    %dl,(%rax)
-   29a1c5d6e:	and    (%rbx),%ebx
-   29a1c5d70:	(bad)
-   29a1c5d71:	add    (%rax),%al
-   29a1c5d73:	add    %al,(%rax)
+   29a1c5d6c:	add    %al,0x23(%rax)
+   29a1c5d6f:	sbb    0x2(%rdx),%ebx
    29a1c5d75:	xor    $0x0,%eax
    29a1c5d7a:	add    %al,(%rax)
    29a1c5d7c:	add    %al,(%rcx)
    29a1c5d7e:	pushf
    29a1c5d7f:	movsb  %ds:(%rsi),%es:(%rdi)
    29a1c5d80:	or     $0x66080000,%eax
    29a1c5d85:	imul   $0xa932196,0x0(%rbp,%riz,2),%ebp
@@ -21943,18 +22003,16 @@
    29a1c5dbe:	cltd
    29a1c5dbf:	(bad)
    29a1c5dc0:	(bad)
    29a1c5dc1:	add    %eax,(%rax)
    29a1c5dc3:	add    %ch,0x11(%rdx)
    29a1c5dc6:	add    %al,(%rax)
    29a1c5dc8:	push   $0x16000011
-   29a1c5dcd:	rex and (%rbx),%ebx
-   29a1c5dd0:	(bad)
-   29a1c5dd1:	add    (%rax),%al
-   29a1c5dd3:	add    %al,(%rax)
+   29a1c5dcd:	jo     29a1c5df2 <.debug_info+0xd9c>
+   29a1c5dcf:	sbb    0x2(%rdx),%ebx
    29a1c5dd5:	(bad)
    29a1c5dd6:	or     (%rax),%al
    29a1c5dd8:	add    %al,(%rsi)
    29a1c5dda:	add    %edx,0x1(%rdx)
    29a1c5ddd:	xor    $0x6,%al
    29a1c5ddf:	add    %edx,0x3(%rcx)
    29a1c5de2:	movabs %eax,0x1a3035801065201
@@ -21965,51 +22023,45 @@
    29a1c5df2:	add    0x20(%rdi),%dh
    29a1c5df5:	add    0x2c000010(%rcx),%dl
    29a1c5dfb:	je     29a1c5e77 <.debug_info+0xe21>
    29a1c5dfd:	jae    29a1c5e64 <.debug_info+0xe0e>
    29a1c5dff:	je     29a1c5e01 <.debug_info+0xdab>
    29a1c5e01:	add    (%rdx),%ah
    29a1c5e03:	add    %edx,(%rax)
-   29a1c5e05:	push   %rax
-   29a1c5e06:	and    (%rbx),%ebx
+   29a1c5e05:	andb   $0x1b,(%rbx)
    29a1c5e08:	(bad)
    29a1c5e09:	add    (%rax),%al
    29a1c5e0b:	add    %al,(%rax)
    29a1c5e0d:	ss add %al,(%rax)
    29a1c5e10:	add    %al,(%rax)
    29a1c5e12:	add    %al,(%rax)
    29a1c5e14:	add    %al,(%rcx)
    29a1c5e16:	pushf
    29a1c5e17:	femms
    29a1c5e19:	add    %al,(%rax)
    29a1c5e1b:	sub    $0xe0f,%eax
-   29a1c5e20:	push   %rsp
-   29a1c5e21:	and    (%rbx),%ebx
-   29a1c5e23:	(bad)
-   29a1c5e24:	add    (%rax),%al
-   29a1c5e26:	add    %al,(%rax)
-   29a1c5e28:	add    %edx,0x1b(%rbx,%riz,1)
-   29a1c5e2c:	(bad)
-   29a1c5e2d:	add    (%rax),%al
+   29a1c5e20:	test   %ah,(%rbx)
+   29a1c5e22:	sbb    0x2(%rdx),%ebx
+   29a1c5e28:	add    %eax,0x29a1b(%rbx,%riz,1)
    29a1c5e2f:	add    %al,(%rax)
    29a1c5e31:	sub    $0x0,%eax
    29a1c5e36:	add    %al,(%rax)
    29a1c5e38:	add    %al,(%rcx)
    29a1c5e3a:	xchg   %eax,%ecx
-   29a1c5e3b:	add    -0x65e4dc9e(%rip),%eax        # 2343781a3 <__size_of_stack_reserve__+0x2341781a3>
+   29a1c5e3b:	add    -0x65e4dc6e(%rip),%eax        # 2343781d3 <__size_of_stack_reserve__+0x2341781d3>
    29a1c5e41:	add    (%rax),%al
    29a1c5e43:	add    %al,(%rax)
    29a1c5e45:	sub    (%rbx),%ecx
    29a1c5e47:	add    %al,(%rax)
-   29a1c5e49:	add    $0x9a1b236e,%eax
+   29a1c5e49:	add    $0x9a1b239e,%eax
    29a1c5e4e:	add    (%rax),%al
    29a1c5e50:	add    %al,(%rax)
    29a1c5e52:	sbb    %cl,(%rbx)
    29a1c5e54:	add    %al,(%rax)
-   29a1c5e56:	add    $0x9a1b237a,%eax
+   29a1c5e56:	add    $0x9a1b23aa,%eax
    29a1c5e5b:	add    (%rax),%al
    29a1c5e5d:	add    %al,(%rax)
    29a1c5e5f:	add    $0xb,%eax
    29a1c5e64:	add    %ch,(%rsi)
    29a1c5e66:	pop    %rdi
    29a1c5e67:	je     29a1c5ee3 <.debug_info+0xe8d>
    29a1c5e69:	jae    29a1c5ed0 <.debug_info+0xe7a>
@@ -22022,57 +22074,56 @@
    29a1c5e7c:	je     29a1c5edd <.debug_info+0xe87>
    29a1c5e7e:	outsw  %ds:(%rsi),(%dx)
    29a1c5e80:	jb     29a1c5eef <.debug_info+0xe99>
    29a1c5e82:	(bad)
    29a1c5e83:	je     29a1c5e85 <.debug_info+0xe2f>
    29a1c5e85:	add    %ebp,0x16(%rsi)
    29a1c5e88:	rex.RX add (%rax),%r8b
-   29a1c5e8b:	add    %dh,0x29a1b21(%rax)
-   29a1c5e91:	add    %al,(%rax)
-   29a1c5e93:	add    %al,(%rbx)
-   29a1c5e95:	add    %al,(%rax)
-   29a1c5e97:	add    %al,(%rax)
-   29a1c5e99:	add    %al,(%rax)
-   29a1c5e9b:	add    %al,(%rcx)
-   29a1c5e9d:	pushf
-   29a1c5e9e:	xor    %bl,0x61(%rdi)
-   29a1c5ea1:	insl   (%dx),%es:(%rdi)
-   29a1c5ea2:	jae    29a1c5f0b <.debug_info+0xeb5>
-   29a1c5ea4:	pop    %rdi
+   29a1c5e8b:	add    %ah,%al
+   29a1c5e8d:	and    %ebx,(%rbx)
+   29a1c5e8f:	(bad)
+   29a1c5e90:	add    (%rax),%al
+   29a1c5e92:	add    %al,(%rax)
+   29a1c5e94:	add    (%rax),%eax
+   29a1c5e96:	add    %al,(%rax)
+   29a1c5e98:	add    %al,(%rax)
+   29a1c5e9a:	add    %al,(%rax)
+   29a1c5e9c:	add    %ebx,0x736d615f(%rax,%rsi,1)
+   29a1c5ea3:	addr32 pop %rdi
    29a1c5ea5:	gs js  29a1c5f11 <.debug_info+0xebb>
    29a1c5ea8:	je     29a1c5eaa <.debug_info+0xe54>
    29a1c5eaa:	add    %ebp,0x26(%rcx)
-   29a1c5ead:	loopne 29a1c5ed1 <.debug_info+0xe7b>
+   29a1c5ead:	adc    %ah,(%rbx)
    29a1c5eaf:	sbb    0x2(%rdx),%ebx
    29a1c5eb5:	cs add %al,(%rax)
    29a1c5eb8:	add    %al,(%rax)
    29a1c5eba:	add    %al,(%rax)
    29a1c5ebc:	add    %al,(%rcx)
    29a1c5ebe:	pushf
    29a1c5ebf:	rorl   $1,(%rsi)
    29a1c5ec1:	add    %al,(%rax)
    29a1c5ec3:	or     %dh,0x65(%rdx)
    29a1c5ec6:	je     29a1c5ec8 <.debug_info+0xe72>
    29a1c5ec8:	imul   $0x1176,0x11e(%rip),%esi        # 29a1c5ff0 <.debug_info+0xf9a>
    29a1c5ed2:	jb     29a1c5ee5 <.debug_info+0xe8f>
    29a1c5ed4:	add    %al,(%rax)
-   29a1c5ed6:	adc    %esi,%ecx
-   29a1c5ed8:	and    (%rbx),%bl
+   29a1c5ed6:	adc    %esp,(%rcx)
+   29a1c5ed8:	and    (%rbx),%ebx
    29a1c5eda:	(bad)
    29a1c5edb:	add    (%rax),%al
    29a1c5edd:	add    %al,(%rax)
    29a1c5edf:	jp     29a1c5eec <.debug_info+0xe96>
    29a1c5ee1:	add    %al,(%rax)
    29a1c5ee3:	xchg   %eax,%edi
    29a1c5ee4:	(bad)
    29a1c5ee5:	add    %al,(%rax)
    29a1c5ee7:	(bad)
    29a1c5ee8:	add    %edx,0x1(%rdx)
    29a1c5eeb:	xor    (%rax),%al
-   29a1c5eed:	adc    %eax,(%rbx)
+   29a1c5eed:	adc    %esi,(%rbx)
    29a1c5eef:	and    (%rbx),%ebx
    29a1c5ef1:	(bad)
    29a1c5ef2:	add    (%rax),%al
    29a1c5ef4:	add    %al,(%rax)
    29a1c5ef6:	push   %rcx
    29a1c5ef7:	or     (%rax),%eax
    29a1c5ef9:	add    %bh,0x1060000(%rsi,%rcx,1)
@@ -22081,16 +22132,15 @@
    29a1c5f03:	rolb   $0x9a,0x1b(%rcx)
    29a1c5f07:	add    (%rax),%al
    29a1c5f09:	add    %al,(%rax)
    29a1c5f0b:	(bad)
    29a1c5f0c:	add    %ebx,0x2(%rax)
    29a1c5f0f:	jae    29a1c5f11 <.debug_info+0xebb>
    29a1c5f11:	add    %dl,(%rsi)
-   29a1c5f13:	(bad)
-   29a1c5f14:	and    (%rbx),%ebx
+   29a1c5f13:	ds and (%rbx),%ebx
    29a1c5f16:	(bad)
    29a1c5f17:	add    (%rax),%al
    29a1c5f19:	add    %al,(%rax)
    29a1c5f1b:	cmp    $0xb,%al
    29a1c5f1d:	add    %al,(%rax)
    29a1c5f1f:	(bad)
    29a1c5f20:	add    %edx,0x2(%rdx)
@@ -22099,15 +22149,15 @@
    29a1c5f27:	adc    $0x715f7461,%eax
    29a1c5f2c:	jne    29a1c5f97 <.debug_info+0xf41>
    29a1c5f2e:	movsxd 0x5f(%rbx),%ebp
    29a1c5f31:	gs js  29a1c5f9d <.debug_info+0xf47>
    29a1c5f34:	je     29a1c5f36 <.debug_info+0xee0>
    29a1c5f36:	add    $0x1e0f01ab,%eax
    29a1c5f3b:	add    %eax,(%rax)
-   29a1c5f3d:	add    %al,%al
+   29a1c5f3d:	add    %dh,%al
    29a1c5f3f:	and    (%rbx),%bl
    29a1c5f41:	(bad)
    29a1c5f42:	add    (%rax),%al
    29a1c5f44:	add    %al,(%rax)
    29a1c5f46:	adc    $0x0,%eax
    29a1c5f4b:	add    %al,(%rax)
    29a1c5f4d:	add    %al,(%rcx)
@@ -22119,63 +22169,61 @@
    29a1c5f58:	movsxd (%rax),%eax
    29a1c5f5a:	pop    %rbp
    29a1c5f5b:	sub    %ch,%dh
    29a1c5f5d:	add    (%rax),%al
    29a1c5f5f:	add    %cl,-0x7affffef(%rcx)
    29a1c5f65:	adc    %eax,(%rax)
    29a1c5f67:	add    %dh,(%rcx)
-   29a1c5f69:	{rex2 0x22} sbb 0x2(%rdx),%ebx
-   29a1c5f71:	pushf
-   29a1c5f72:	or     (%rax),%eax
-   29a1c5f74:	add    %al,(%rax)
-   29a1c5f76:	adc    $0x656e6f5f,%eax
-   29a1c5f7b:	js     29a1c5fe6 <.debug_info+0xf90>
+   29a1c5f69:	add    $0x29a1b23,%eax
+   29a1c5f6e:	add    %al,(%rax)
+   29a1c5f70:	add    %bl,0x15000000(%rbx,%rcx,1)
+   29a1c5f77:	pop    %rdi
+   29a1c5f78:	outsl  %ds:(%rsi),(%dx)
+   29a1c5f79:	outsb  %ds:(%rsi),(%dx)
+   29a1c5f7a:	gs js  29a1c5fe6 <.debug_info+0xf90>
    29a1c5f7d:	je     29a1c5f7f <.debug_info+0xf29>
    29a1c5f7f:	add    $0xc0150287,%eax
    29a1c5f84:	add    (%rax),%al
-   29a1c5f86:	add    %ah,0x29a1b22(%rax)
-   29a1c5f8c:	add    %al,(%rax)
-   29a1c5f8e:	add    %bl,(%rsi)
+   29a1c5f86:	add    %dl,%al
+   29a1c5f88:	and    (%rbx),%bl
+   29a1c5f8a:	(bad)
+   29a1c5f8b:	add    (%rax),%al
+   29a1c5f8d:	add    %al,(%rax)
+   29a1c5f8f:	(bad)
    29a1c5f90:	add    %al,(%rax)
    29a1c5f92:	add    %al,(%rax)
    29a1c5f94:	add    %al,(%rax)
    29a1c5f96:	add    %al,(%rcx)
    29a1c5f98:	pushf
    29a1c5f99:	jo     29a1c5faa <.debug_info+0xf54>
    29a1c5f9b:	add    %al,(%rax)
    29a1c5f9d:	or     %ah,0x75(%rsi)
    29a1c5fa0:	outsb  %ds:(%rsi),(%dx)
    29a1c5fa1:	movsxd (%rax),%eax
    29a1c5fa3:	push   %rsi
    29a1c5fa4:	and    $0x2c0,%eax
    29a1c5fa9:	movabs 0x160000119b000011,%eax
-   29a1c5fb2:	lods   %ds:(%rsi),%eax
-   29a1c5fb3:	and    (%rbx),%bl
-   29a1c5fb5:	(bad)
-   29a1c5fb6:	add    (%rax),%al
-   29a1c5fb8:	add    %al,(%rax)
+   29a1c5fb2:	frstor (%rdx)
+   29a1c5fb4:	sbb    0x2(%rdx),%ebx
    29a1c5fba:	rorl   $0x0,(%rbx)
    29a1c5fbd:	add    %al,(%rsi)
    29a1c5fbf:	add    %edx,0x2(%rdx)
    29a1c5fc2:	jae    29a1c5fc4 <.debug_info+0xf6e>
    29a1c5fc4:	add    %al,(%rax)
    29a1c5fc6:	(bad)
    29a1c5fc7:	pop    %rdi
    29a1c5fc8:	pop    %rdi
    29a1c5fc9:	ja     29a1c6032 <.debug_info+0xfdc>
    29a1c5fcb:	gs je  29a1c603b <.debug_info+0xfe5>
    29a1c5fce:	(bad)
    29a1c5fcf:	imul   $0x736772,0x61(%rsi),%ebp
    29a1c5fd6:	rex.WX (bad)
    29a1c5fd8:	add    %eax,(%rax)
-   29a1c5fda:	add    %dh,(%rax)
-   29a1c5fdc:	and    (%rbx),%bl
-   29a1c5fde:	(bad)
-   29a1c5fdf:	add    (%rax),%al
-   29a1c5fe1:	add    %al,(%rax)
+   29a1c5fda:	add    %ah,0x22(%rax)
+   29a1c5fdd:	sbb    0x2(%rdx),%ebx
    29a1c5fe3:	push   $0x0
    29a1c5fe5:	add    %al,(%rax)
    29a1c5fe7:	add    %al,(%rax)
    29a1c5fe9:	add    %al,(%rax)
    29a1c5feb:	add    %ebx,0x8000010(%rbx,%rbx,2)
    29a1c5ff2:	pop    %rdi
    29a1c5ff3:	rex.B jb 29a1c605d <.debug_info+0x1007>
@@ -22212,62 +22260,62 @@
    29a1c603f:	adc    (%rax),%al
    29a1c6041:	add    %ah,(%rcx)
    29a1c6043:	int1
    29a1c6044:	add    %al,(%rax)
    29a1c6046:	add    %cl,0x6c(%rdx)
    29a1c6049:	mov    (%rcx),%cs
    29a1c604b:	add    %al,(%rax)
-   29a1c604d:	add    0x22500520(%rcx),%dl
+   29a1c604d:	add    0x22800520(%rcx),%dl
    29a1c6053:	sbb    0x2(%rdx),%ebx
    29a1c6059:	xor    %cl,(%rax,%rax,1)
    29a1c605c:	add    %dl,(%rcx)
-   29a1c605e:	(bad)
+   29a1c605e:	nop
    29a1c605f:	and    (%rbx),%bl
    29a1c6061:	(bad)
    29a1c6062:	add    (%rax),%al
    29a1c6064:	add    %al,(%rax)
    29a1c6066:	or     %ecx,(%rax,%rax,1)
    29a1c6069:	add    %ah,(%rsi)
    29a1c606b:	adc    %al,(%rax)
    29a1c606d:	add    %al,(%rsi)
    29a1c606f:	add    %edx,0x9(%rdx)
    29a1c6072:	jbe    29a1c6074 <.debug_info+0x101e>
    29a1c6074:	or     %ah,(%rax)
    29a1c6076:	and    $0x30,%al
    29a1c6078:	cs and (%rcx),%eax
-   29a1c607b:	add    %al,-0x65e4dd9b(%rip)        # 2343782e6 <__size_of_stack_reserve__+0x2341782e6>
+   29a1c607b:	add    %al,-0x65e4dd6b(%rip)        # 234378316 <__size_of_stack_reserve__+0x234178316>
    29a1c6081:	add    (%rax),%al
    29a1c6083:	add    %al,(%rax)
    29a1c6085:	popf
    29a1c6086:	or     $0x0,%al
-   29a1c6088:	add    %al,-0x65e4dd92(%rip)        # 2343782fc <__size_of_stack_reserve__+0x2341782fc>
+   29a1c6088:	add    %al,-0x65e4dd62(%rip)        # 23437832c <__size_of_stack_reserve__+0x23417832c>
    29a1c608e:	add    (%rax),%al
    29a1c6090:	add    %al,(%rax)
    29a1c6092:	cmc
    29a1c6093:	or     (%rax),%eax
-   29a1c6095:	add    %al,-0x65e4dd87(%rip)        # 234378314 <__size_of_stack_reserve__+0x234178314>
+   29a1c6095:	add    %al,-0x65e4dd57(%rip)        # 234378344 <__size_of_stack_reserve__+0x234178344>
    29a1c609b:	add    (%rax),%al
    29a1c609d:	add    %al,(%rax)
    29a1c609f:	fisttps (%rbx)
    29a1c60a1:	add    %al,(%rax)
-   29a1c60a3:	add    $0x9a1b228d,%eax
+   29a1c60a3:	add    $0x9a1b22bd,%eax
    29a1c60a8:	add    (%rax),%al
    29a1c60aa:	add    %al,(%rax)
    29a1c60ac:	push   %rbp
    29a1c60ad:	or     $0x0,%al
    29a1c60af:	add    %al,(%rax)
    29a1c60b1:	(bad)
    29a1c60b2:	pop    %rdi
    29a1c60b3:	pop    %rdi
    29a1c60b4:	addr32 gs je 29a1c6125 <.debug_info+0x10cf>
    29a1c60b8:	(bad)
    29a1c60b9:	imul   $0x736772,0x61(%rsi),%ebp
    29a1c60c0:	ds (bad)
    29a1c60c2:	add    %eax,(%rax)
-   29a1c60c4:	add    %al,%al
+   29a1c60c4:	add    %dh,%al
    29a1c60c6:	and    %ebx,(%rbx)
    29a1c60c8:	(bad)
    29a1c60c9:	add    (%rax),%al
    29a1c60cb:	add    %al,(%rax)
    29a1c60cd:	push   $0x0
    29a1c60cf:	add    %al,(%rax)
    29a1c60d1:	add    %al,(%rax)
@@ -22309,76 +22357,73 @@
    29a1c6129:	adc    (%rax),%al
    29a1c612b:	add    %ah,(%rcx)
    29a1c612d:	int1
    29a1c612e:	add    %al,(%rax)
    29a1c6130:	add    %bh,(%rsi)
    29a1c6132:	mov    %gs:(%rcx),%cs
    29a1c6135:	add    %al,(%rax)
-   29a1c6137:	add    0x21e00520(%rcx),%dl
+   29a1c6137:	add    0x22100520(%rcx),%dl
    29a1c613d:	sbb    0x2(%rdx),%ebx
    29a1c6143:	(bad)  (%rax,%rax,1)
    29a1c6146:	add    %dl,(%rcx)
-   29a1c6148:	lock and %ebx,(%rbx)
-   29a1c614b:	(bad)
-   29a1c614c:	add    (%rax),%al
-   29a1c614e:	add    %al,(%rax)
+   29a1c6148:	and    %ah,(%rdx)
+   29a1c614a:	sbb    0x2(%rdx),%ebx
    29a1c6150:	mov    $0xc,%al
    29a1c6152:	add    %al,(%rax)
    29a1c6154:	adc    %dl,(%rcx)
    29a1c6156:	add    %al,(%rax)
    29a1c6158:	(bad)
    29a1c6159:	add    %edx,0x9(%rdx)
    29a1c615c:	jbe    29a1c615e <.debug_info+0x1108>
    29a1c615e:	or     %ah,(%rax)
    29a1c6160:	and    $0x30,%al
    29a1c6162:	cs and (%rcx),%eax
-   29a1c6165:	add    %al,-0x65e4de0b(%rip)        # 234378360 <__size_of_stack_reserve__+0x234178360>
+   29a1c6165:	add    %al,-0x65e4dddb(%rip)        # 234378390 <__size_of_stack_reserve__+0x234178390>
    29a1c616b:	add    (%rax),%al
    29a1c616d:	add    %al,(%rax)
    29a1c616f:	popf
    29a1c6170:	or     $0x0,%al
-   29a1c6172:	add    %al,-0x65e4de02(%rip)        # 234378376 <__size_of_stack_reserve__+0x234178376>
+   29a1c6172:	add    %al,-0x65e4ddd2(%rip)        # 2343783a6 <__size_of_stack_reserve__+0x2341783a6>
    29a1c6178:	add    (%rax),%al
    29a1c617a:	add    %al,(%rax)
    29a1c617c:	mov    (%rax,%rax,1),%cl
-   29a1c617f:	add    %al,-0x65e4ddf7(%rip)        # 23437838e <__size_of_stack_reserve__+0x23417838e>
+   29a1c617f:	add    %al,-0x65e4ddc7(%rip)        # 2343783be <__size_of_stack_reserve__+0x2341783be>
    29a1c6185:	add    (%rax),%al
    29a1c6187:	add    %al,(%rax)
    29a1c6189:	jne    29a1c6197 <.debug_info+0x1141>
    29a1c618b:	add    %al,(%rax)
-   29a1c618d:	add    $0x9a1b221d,%eax
+   29a1c618d:	add    $0x9a1b224d,%eax
    29a1c6192:	add    (%rax),%al
    29a1c6194:	add    %al,(%rax)
    29a1c6196:	push   %rbp
    29a1c6197:	or     $0x0,%al
    29a1c6199:	add    %al,(%rax)
    29a1c619b:	xor    (%rdi),%cl
    29a1c619d:	(bad)
    29a1c619e:	add    %al,(%rax)
-   29a1c61a0:	nop
-   29a1c61a1:	and    (%rbx),%ebx
+   29a1c61a0:	shlb   $0x1b,(%rbx)
    29a1c61a3:	(bad)
    29a1c61a4:	add    (%rax),%al
    29a1c61a6:	add    %al,(%rax)
    29a1c61a8:	ss add %al,(%rax)
    29a1c61ab:	add    %al,(%rax)
    29a1c61ad:	add    %al,(%rax)
    29a1c61af:	add    %al,(%rcx)
    29a1c61b1:	pushf
-   29a1c61b2:	add    $0x9a1b23a2,%eax
+   29a1c61b2:	add    $0x9a1b23d2,%eax
    29a1c61b7:	add    (%rax),%al
    29a1c61b9:	add    %al,(%rax)
    29a1c61bb:	sub    (%rbx),%ecx
    29a1c61bd:	add    %al,(%rax)
-   29a1c61bf:	add    $0x9a1b23ae,%eax
+   29a1c61bf:	add    $0x9a1b23de,%eax
    29a1c61c4:	add    (%rax),%al
    29a1c61c6:	add    %al,(%rax)
    29a1c61c8:	sbb    %cl,(%rbx)
    29a1c61ca:	add    %al,(%rax)
-   29a1c61cc:	add    $0x9a1b23ba,%eax
+   29a1c61cc:	add    $0x9a1b23ea,%eax
    29a1c61d1:	add    (%rax),%al
    29a1c61d3:	add    %al,(%rax)
    29a1c61d5:	add    $0xb,%eax
 	...
 
 000000029a1c61db <.debug_info>:
    29a1c61db:	sahf
@@ -22411,17 +22456,15 @@
    29a1c6231:	jne    29a1c626c <.debug_info+0x91>
    29a1c6233:	cmp    %eax,(%rax)
    29a1c6235:	or     $0xc,%al
    29a1c6237:	sldt   (%rax)
    29a1c623a:	hlt
    29a1c623b:	(bad)
    29a1c623c:	add    %al,(%rax)
-   29a1c623e:	lock and $0x1b,%al
-   29a1c6241:	(bad)
-   29a1c6242:	add    (%rax),%al
+   29a1c623e:	xor    %ah,0x29a1b(%rip)        # 29a1efc5f <.debug_rnglists+0x1fbbb>
    29a1c6244:	add    %al,(%rax)
    29a1c6246:	xor    (%rax),%al
    29a1c6248:	add    %al,(%rax)
    29a1c624a:	add    %al,(%rax)
    29a1c624c:	add    %al,(%rax)
    29a1c624e:	push   %rsi
    29a1c624f:	sbb    %al,(%rax)
@@ -22686,17 +22729,15 @@
    29a1c64db:	add    %al,(%rax)
    29a1c64dd:	add    %dl,(%rsi)
    29a1c64df:	data16 jo 29a1c6554 <.debug_info+0x379>
    29a1c64e2:	imul   $0xff040066,0x74(%rsi),%ebp
    29a1c64e9:	add    %ecx,(%rdi)
    29a1c64eb:	or     %eax,(%rcx)
    29a1c64ed:	add    %al,(%rax)
-   29a1c64ef:	lock and $0x1b,%al
-   29a1c64f2:	(bad)
-   29a1c64f3:	add    (%rax),%al
+   29a1c64ef:	xor    %ah,0x29a1b(%rip)        # 29a1eff10 <.debug_rnglists+0x1fe6c>
    29a1c64f5:	add    %al,(%rax)
    29a1c64f7:	xor    (%rax),%al
    29a1c64f9:	add    %al,(%rax)
    29a1c64fb:	add    %al,(%rax)
    29a1c64fd:	add    %al,(%rax)
    29a1c64ff:	add    %ebx,0x6c69465f(%rsp,%rcx,1)
    29a1c6506:	add    %ch,%gs:(%rcx)
@@ -22727,18 +22768,17 @@
    29a1c6541:	(bad)
    29a1c6542:	or     %eax,(%rcx)
    29a1c6544:	add    %al,(%rax)
    29a1c6546:	ficoml (%rdx)
    29a1c6548:	add    %al,(%rax)
    29a1c654a:	fcoms  (%rdx)
    29a1c654c:	add    %al,(%rax)
-   29a1c654e:	sbb    %ebx,0x29a1b25(%rip)        # 29cb68079 <.debug_rnglists+0x2997fd5>
-   29a1c6554:	add    %al,(%rax)
-   29a1c6556:	add    %al,%ch
-   29a1c6558:	add    (%rax),%al
+   29a1c654e:	sbb    %ebx,0x25(%rbp)
+   29a1c6551:	sbb    0x2(%rdx),%ebx
+   29a1c6557:	(bad)
    29a1c655a:	add    %al,0x30015201(%rip)        # 2ca1db761 <.debug_rnglists+0x3000b6bd>
    29a1c6560:	add    $0xa3035101,%eax
    29a1c6565:	add    %edx,0x5(%rdx)
    29a1c6568:	add    %ebx,0x3(%rax)
    29a1c656b:	movabs %eax,0x530015901055101
    29a1c6574:	add    0x20(%rdi),%dh
    29a1c6577:	add    0x10(%rcx),%dl
@@ -25777,16 +25817,18 @@
    29a1c93c8:	add    %al,(%rdx)
    29a1c93ca:	pop    %rdi
    29a1c93cb:	add    (%rax),%al
    29a1c93cd:	add    %al,(%rdx)
    29a1c93cf:	imul   $0x5020000,(%rdx),%eax
    29a1c93d5:	add    %eax,(%rax)
    29a1c93d7:	or     %eax,(%rdx)
-   29a1c93d9:	rclb   $1,(%rbx)
-   29a1c93db:	sbb    0x2(%rdx),%ebx
+   29a1c93d9:	add    %dl,(%rbx,%rbx,1)
+   29a1c93dc:	(bad)
+   29a1c93dd:	add    (%rax),%al
+   29a1c93df:	add    %al,(%rax)
    29a1c93e1:	add    (%rcx,%rax,1),%edx
    29a1c93e4:	add    $0x5144b03,%eax
    29a1c93e9:	or     (%rcx),%al
    29a1c93eb:	add    $0x53e0807,%eax
    29a1c93f0:	or     %al,(%rsi)
    29a1c93f2:	add    %eax,0x52f0607(%rip)        # 29f4b99ff <.debug_rnglists+0x52e995b>
    29a1c93f8:	or     %al,(%rsi)
@@ -25938,18 +25980,20 @@
    29a1c9547:	push   %rsp
    29a1c9548:	add    $0x0,%al
    29a1c954a:	add    %al,(%rdx)
    29a1c954c:	pop    %rsp
    29a1c954d:	add    $0x0,%al
    29a1c954f:	add    %al,(%rdx)
    29a1c9551:	add    $0x2090001,%eax
-   29a1c9556:	movabs 0x3000000029a1b14,%al
-   29a1c955f:	mov    %eax,(%rcx)
-   29a1c9561:	add    %eax,(%rsi)
-   29a1c9563:	add    %eax,0x5500603(%rip)        # 29f6c9b6c <.debug_rnglists+0x54f9ac8>
+   29a1c9556:	rclb   $1,(%rbx,%rbx,1)
+   29a1c9559:	(bad)
+   29a1c955a:	add    (%rax),%al
+   29a1c955c:	add    %al,(%rax)
+   29a1c955e:	add    0x1060101(%rcx),%ecx
+   29a1c9564:	add    $0x5500603,%eax
    29a1c9569:	(bad)
    29a1c956a:	(bad)
    29a1c956b:	add    %eax,-0x6fe6fcff(%rip)        # 22a359872 <__size_of_stack_reserve__+0x22a159872>
    29a1c9571:	add    $0x2c080603,%eax
    29a1c9576:	pop    %rcx
    29a1c9577:	add    $0x6130601,%eax
    29a1c957c:	add    0x106ac7f(%rbp),%esp
@@ -26101,17 +26145,16 @@
    29a1c96f8:	add    %dh,%dh
    29a1c96fa:	(bad)
    29a1c96fb:	add    %al,(%rax)
    29a1c96fd:	add    %bh,%bh
    29a1c96ff:	(bad)
    29a1c9700:	add    %al,(%rax)
    29a1c9702:	add    %al,0x2090001(%rip)        # 29c259709 <.debug_rnglists+0x2089665>
-   29a1c9708:	jo     29a1c971f <.debug_line+0x9b>
-   29a1c970a:	sbb    0x2(%rdx),%ebx
-   29a1c9710:	add    %esp,%edx
+   29a1c9708:	movabs 0x3000000029a1b15,%al
+   29a1c9711:	(bad)
    29a1c9712:	add    %al,(%rcx)
    29a1c9714:	(bad)
    29a1c9715:	add    %eax,0x3e030603(%rip)        # 2d81f9d1e <.debug_rnglists+0x3e029c7a>
    29a1c971b:	adc    0x41030601(%rip),%ax        # 2db1f9d23 <.debug_rnglists+0x41029c7f>
    29a1c9722:	add    %eax,0x3c3f0303(%rip)        # 2d65b9a2b <.debug_rnglists+0x3c3e9987>
    29a1c9728:	pop    %rdx
    29a1c9729:	add    $0x7fbf0301,%eax
@@ -26218,27 +26261,26 @@
    29a1c986d:	pop    %rsp
    29a1c986e:	add    %eax,0x12030607(%rip)        # 2ac1f9e7b <.debug_rnglists+0x12029dd7>
    29a1c9874:	je     29a1c9879 <.debug_line+0x1f5>
    29a1c9876:	ja     29a1c9880 <.debug_line+0x1fc>
    29a1c9878:	sahf
    29a1c9879:	(bad)
    29a1c987a:	repnz add $0x9000601,%eax
-   29a1c9880:	add    0x17(%rax),%dl
-   29a1c9883:	sbb    0x2(%rdx),%ebx
-   29a1c9889:	add    0x3050102(%rax),%esp
-   29a1c988f:	or     %cl,0x14(%rbx)
-   29a1c9892:	adc    $0x1060705,%eax
-   29a1c9897:	add    $0x1057406,%eax
-   29a1c989c:	add    (%rax),%edx
-   29a1c989e:	pop    %rax
-   29a1c989f:	add    $0x72030603,%eax
-   29a1c98a4:	or     %ah,-0x60(%rsi)
-   29a1c98a7:	add    $0x501060b,%eax
-   29a1c98ac:	add    (%rsi),%eax
-   29a1c98ae:	pop    %rcx
+   29a1c9880:	add    0x29a1b17(%rax),%al
+   29a1c9886:	add    %al,(%rax)
+   29a1c9888:	add    %al,(%rbx)
+   29a1c988a:	movabs 0x15144b0803050102,%al
+   29a1c9893:	add    $0x5010607,%eax
+   29a1c9898:	(bad)
+   29a1c9899:	je     29a1c98a0 <.debug_line+0x21c>
+   29a1c989b:	add    %eax,(%rbx)
+   29a1c989d:	adc    %bl,0x5(%rax)
+   29a1c98a0:	add    (%rsi),%eax
+   29a1c98a2:	add    0x8(%rdx),%esi
+   29a1c98a5:	data16 movabs 0x5906030501060b05,%al
    29a1c98af:	add    $0x2e01061b,%eax
    29a1c98b4:	rex.WX add $0x7ec7030d,%rax
    29a1c98ba:	or     %dl,(%rdx)
    29a1c98bc:	add    $0x1ba030f,%eax
    29a1c98c1:	(bad)
    29a1c98c2:	add    $0xc059d1b,%eax
    29a1c98c7:	add    %al,(%rdx)
@@ -26536,15 +26578,15 @@
    29a1c9c63:	add    %al,(%rdx)
    29a1c9c65:	or     (%rax),%cl
    29a1c9c67:	add    %al,(%rax)
    29a1c9c69:	add    (%rsi),%bl
    29a1c9c6b:	or     %al,(%rax)
    29a1c9c6d:	add    %al,(%rdx)
    29a1c9c6f:	add    $0x2090001,%eax
-   29a1c9c74:	mov    $0x1a,%al
+   29a1c9c74:	loopne 29a1c9c90 <.debug_line+0x8c>
    29a1c9c76:	sbb    0x2(%rdx),%ebx
    29a1c9c7c:	add    %edx,%esp
    29a1c9c7e:	add    %al,(%rcx)
    29a1c9c80:	add    $0x5f4a403,%eax
    29a1c9c85:	or     $0x1e050106,%eax
    29a1c9c8a:	add    %al,(%rdx)
    29a1c9c8c:	add    $0x1,%al
@@ -26802,15 +26844,16 @@
    29a1c9f3d:	pop    %rcx
    29a1c9f3e:	or     (%rax),%al
    29a1c9f40:	add    %al,(%rdx)
    29a1c9f42:	(bad)
    29a1c9f43:	or     (%rax),%al
    29a1c9f45:	add    %al,(%rdx)
    29a1c9f47:	add    $0x2090001,%eax
-   29a1c9f4c:	and    %bl,0x29a1b(%rip)        # 29a1f396d <.debug_rnglists+0x238c9>
+   29a1c9f4c:	push   %rax
+   29a1c9f4d:	sbb    $0x29a1b,%eax
    29a1c9f52:	add    %al,(%rax)
    29a1c9f54:	add    (%rdi),%ecx
    29a1c9f56:	add    %eax,(%rsi)
    29a1c9f58:	add    %eax,0x13130603(%rip)        # 2ad2fa561 <.debug_rnglists+0x1312a4bd>
    29a1c9f5e:	adc    (%rbx,%rdx,1),%edx
    29a1c9f61:	add    $0x513060c,%eax
    29a1c9f66:	(bad)
@@ -27189,16 +27232,19 @@
    29a1ca468:	add    (%rdi),%cl
    29a1ca46a:	add    %bl,%dh
    29a1ca46c:	or     (%rax),%al
    29a1ca46e:	add    %al,(%rcx)
    29a1ca470:	decb   (%rdx)
    29a1ca472:	add    %al,(%rax)
    29a1ca474:	add    %eax,0x2090001(%rip)        # 29c25a47b <.debug_rnglists+0x208a3d7>
-   29a1ca47a:	and    %ah,(%rcx)
-   29a1ca47c:	sbb    0x2(%rdx),%ebx
+   29a1ca47a:	push   %rax
+   29a1ca47b:	and    %ebx,(%rbx)
+   29a1ca47d:	(bad)
+   29a1ca47e:	add    (%rax),%al
+   29a1ca480:	add    %al,(%rax)
    29a1ca482:	add    (%rcx),%ecx
    29a1ca484:	add    %eax,0x1090303(%rip)        # 29b25a78d <.debug_rnglists+0x108a6e9>
    29a1ca48a:	add    $0x2330601,%eax
    29a1ca48f:	add    %eax,(%rax)
    29a1ca491:	add    %eax,(%rcx)
 
 000000029a1ca493 <.debug_line>:
@@ -27230,18 +27276,16 @@
    29a1ca4d1:	ret
    29a1ca4d2:	or     (%rax),%eax
    29a1ca4d4:	add    %al,(%rdx)
    29a1ca4d6:	iret
    29a1ca4d7:	or     (%rax),%eax
    29a1ca4d9:	add    %al,(%rdx)
    29a1ca4db:	add    $0x2090001,%eax
-   29a1ca4e0:	jo     29a1ca503 <.debug_line+0x9>
-   29a1ca4e2:	sbb    0x2(%rdx),%ebx
-   29a1ca4e8:	add    (%rdi),%ecx
-   29a1ca4ea:	add    %eax,(%rsi)
+   29a1ca4e0:	movabs 0x3000000029a1b21,%al
+   29a1ca4e9:	sgdt   (%rsi)
    29a1ca4ec:	add    %eax,0x5130603(%rip)        # 29f2faaf5 <.debug_rnglists+0x512aa51>
    29a1ca4f2:	add    %eax,(%rsi)
    29a1ca4f4:	adc    (%rdx),%eax
    29a1ca4f6:	(bad)
    29a1ca4f7:	add    %al,(%rcx)
    29a1ca4f9:	add    %esp,0x0(%rsi)
 
@@ -27273,15 +27317,15 @@
    29a1ca532:	add    %eax,-0x71ff0000(%rsp,%rcx,1)
    29a1ca539:	or     $0x0,%al
    29a1ca53b:	add    %al,(%rdx)
    29a1ca53d:	(bad)
    29a1ca53e:	or     $0x0,%al
    29a1ca540:	add    %al,(%rdx)
    29a1ca542:	movabs %al,0x90001050200000c
-   29a1ca54b:	add    0x29a1b21(%rax),%al
+   29a1ca54b:	add    0x29a1b21(%rax),%dh
    29a1ca551:	add    %al,(%rax)
    29a1ca553:	add    %bl,(%rcx)
    29a1ca555:	(bad)
    29a1ca556:	add    %eax,0x5130603(%rip)        # 29f2fab5f <.debug_rnglists+0x512aabb>
    29a1ca55c:	add    %eax,(%rsi)
    29a1ca55e:	adc    (%rdx),%eax
    29a1ca560:	(bad)
@@ -27315,16 +27359,15 @@
    29a1ca59f:	add    %al,(%rax)
    29a1ca5a1:	add    %edi,0xd(%rcx)
    29a1ca5a4:	add    %al,(%rax)
    29a1ca5a6:	add    0x200000d(%rdx),%al
    29a1ca5ac:	mov    %cs,0x5020000(%rip)        # 29f1ea5b2 <.debug_rnglists+0x501a50e>
    29a1ca5b2:	add    %eax,(%rax)
    29a1ca5b4:	or     %eax,(%rdx)
-   29a1ca5b6:	nop
-   29a1ca5b7:	and    %ebx,(%rbx)
+   29a1ca5b6:	shlb   $0x1b,(%rcx)
    29a1ca5b9:	(bad)
    29a1ca5ba:	add    (%rax),%al
    29a1ca5bc:	add    %al,(%rax)
    29a1ca5be:	add    (%rbx),%ecx
    29a1ca5c0:	add    %eax,(%rsi)
    29a1ca5c2:	add    %eax,0x54b0603(%rip)        # 29f67abcb <.debug_rnglists+0x54aab27>
    29a1ca5c8:	or     (%rsi),%al
@@ -27382,15 +27425,15 @@
    29a1ca63f:	add    %edx,%ebx
    29a1ca641:	(bad)
    29a1ca642:	add    %al,(%rax)
    29a1ca644:	add    %ah,%ch
    29a1ca646:	(bad)
    29a1ca647:	add    %al,(%rax)
    29a1ca649:	add    0x2090001(%rip),%al        # 29c25a650 <.debug_rnglists+0x208a5ac>
-   29a1ca64f:	mov    $0x21,%al
+   29a1ca64f:	loopne 29a1ca672 <.debug_line+0x9c>
    29a1ca651:	sbb    0x2(%rdx),%ebx
    29a1ca657:	add    %esi,%ebp
    29a1ca659:	add    %al,(%rcx)
    29a1ca65b:	add    $0x1051303,%eax
    29a1ca660:	(bad)
    29a1ca661:	adc    (%rsi),%eax
    29a1ca663:	add    -0xe(%rsi),%ecx
@@ -27489,16 +27532,16 @@
    29a1ca771:	add    %eax,0x1057406(%rip)        # 29b221b7d <.debug_rnglists+0x1051ad9>
    29a1ca777:	pop    %rbx
    29a1ca778:	add    $0x5490603,%eax
    29a1ca77d:	add    %eax,(%rsi)
    29a1ca77f:	adc    0x558110a(%rip),%eax        # 29f74b88f <.debug_rnglists+0x557b7eb>
    29a1ca785:	cmp    (%rsi),%al
    29a1ca787:	add    %cl,(%rcx)
-   29a1ca789:	add    %al,%ah
-   29a1ca78b:	and    (%rbx),%bl
+   29a1ca789:	add    (%rax),%dl
+   29a1ca78b:	and    (%rbx),%ebx
    29a1ca78d:	(bad)
    29a1ca78e:	add    (%rax),%al
    29a1ca790:	add    %al,(%rax)
    29a1ca792:	(bad)
    29a1ca793:	(bad)
    29a1ca794:	add    %eax,0x5590603(%rip)        # 29f75ad9d <.debug_rnglists+0x558acf9>
    29a1ca79a:	cmp    (%rsi),%al
@@ -27588,17 +27631,15 @@
    29a1ca88e:	add    %ebp,0x100000f(%rdi)
    29a1ca894:	mov    $0x200000f,%esi
    29a1ca899:	(bad)
    29a1ca89a:	sldt   (%rax)
    29a1ca89d:	add    %cl,%dl
    29a1ca89f:	sldt   (%rax)
    29a1ca8a2:	add    0x2090001(%rip),%al        # 29c25a8a9 <.debug_rnglists+0x208a805>
-   29a1ca8a8:	lock and $0x1b,%al
-   29a1ca8ab:	(bad)
-   29a1ca8ac:	add    (%rax),%al
+   29a1ca8a8:	xor    %ah,0x29a1b(%rip)        # 29a1f42c9 <.debug_rnglists+0x24225>
    29a1ca8ae:	add    %al,(%rax)
    29a1ca8b0:	add    (%rbx),%ecx
    29a1ca8b2:	add    %eax,(%rsi)
    29a1ca8b4:	add    %eax,0x134b0603(%rip)        # 2ad67aebd <.debug_rnglists+0x134aae19>
    29a1ca8ba:	adc    0x5550601(%rip),%eax        # 29f71aec1 <.debug_rnglists+0x554ae1d>
    29a1ca8c0:	or     %ebx,0x5(%rsi,%riz,2)
    29a1ca8c4:	add    %esi,0x5(%rax)
@@ -27741,28 +27782,30 @@
    29a1cb115:	or     $0x7,%al
    29a1cb117:	or     %ah,0x1(%rax)
    29a1cb11d:	add    %al,(%rax)
    29a1cb11f:	add    %bl,(%rax,%rax,1)
    29a1cb122:	add    %al,(%rax)
    29a1cb124:	or     %al,(%rcx)
    29a1cb126:	add    %al,(%rax)
-   29a1cb128:	rclb   $1,(%rbx)
-   29a1cb12a:	sbb    0x2(%rdx),%ebx
+   29a1cb128:	add    %dl,(%rbx,%rbx,1)
+   29a1cb12b:	(bad)
+   29a1cb12c:	add    (%rax),%al
+   29a1cb12e:	add    %al,(%rax)
    29a1cb130:	cmp    (%rax),%al
    29a1cb132:	add    %al,(%rax)
    29a1cb134:	add    %al,(%rax)
    29a1cb136:	add    %al,(%rax)
    29a1cb138:	rex.R (bad)
    29a1cb13a:	xor    %dh,0xe(%rbp)
    29a1cb13d:	or     %al,(%rax)
    29a1cb13f:	add    %dh,(%rax,%rax,1)
    29a1cb142:	add    %al,(%rax)
    29a1cb144:	or     %al,(%rcx)
    29a1cb146:	add    %al,(%rax)
-   29a1cb148:	adc    %dl,(%rbx,%rbx,1)
+   29a1cb148:	rex adc $0x1b,%al
    29a1cb14b:	(bad)
    29a1cb14c:	add    (%rax),%al
    29a1cb14e:	add    %al,(%rax)
    29a1cb150:	push   $0x0
    29a1cb152:	add    %al,(%rax)
    29a1cb154:	add    %al,(%rax)
    29a1cb156:	add    %al,(%rax)
@@ -27778,17 +27821,16 @@
    29a1cb171:	or     %cl,0xb(%rax)
    29a1cb174:	add    %al,(%rax)
    29a1cb176:	add    %al,(%rax)
    29a1cb178:	adc    $0x0,%al
    29a1cb17a:	add    %al,(%rax)
    29a1cb17c:	or     %al,(%rcx)
    29a1cb17e:	add    %al,(%rax)
-   29a1cb180:	adcb   $0x9a,(%rbx,%rbx,1)
-   29a1cb184:	add    (%rax),%al
-   29a1cb186:	add    %al,(%rax)
+   29a1cb180:	mov    $0x14,%al
+   29a1cb182:	sbb    0x2(%rdx),%ebx
    29a1cb188:	(bad)
    29a1cb189:	add    %al,(%rax)
    29a1cb18b:	add    %al,(%rax)
    29a1cb18d:	add    %al,(%rax)
 	...
 
 000000029a1cb190 <.debug_frame>:
@@ -27803,32 +27845,33 @@
    29a1cb19d:	or     $0x7,%al
    29a1cb19f:	or     %ah,0x1(%rax)
    29a1cb1a5:	add    %al,(%rax)
    29a1cb1a7:	add    %ah,(%rax,%rax,1)
    29a1cb1aa:	add    %al,(%rax)
    29a1cb1ac:	nop
    29a1cb1ad:	add    %eax,(%rax)
-   29a1cb1af:	add    %ah,0x29a1b14(%rax)
-   29a1cb1b5:	add    %al,(%rax)
-   29a1cb1b7:	add    %ch,(%rdi)
+   29a1cb1af:	add    %dl,%al
+   29a1cb1b1:	adc    $0x1b,%al
+   29a1cb1b3:	(bad)
+   29a1cb1b4:	add    (%rax),%al
+   29a1cb1b6:	add    %al,(%rax)
+   29a1cb1b8:	(bad)
    29a1cb1b9:	add    %al,(%rax)
    29a1cb1bb:	add    %al,(%rax)
    29a1cb1bd:	add    %al,(%rax)
    29a1cb1bf:	add    %al,0x30(%rsi,%rcx,1)
    29a1cb1c3:	push   %rdx
    29a1cb1c4:	or     (%rsi),%cl
    29a1cb1c6:	or     %cl,0xb(%rdx)
    29a1cb1c9:	rex.WRX (bad)
    29a1cb1cb:	or     %al,(%rax)
    29a1cb1cd:	add    %al,(%rax)
    29a1cb1cf:	add    %cl,0x0(%rax,%rax,1)
-   29a1cb1d3:	add    %dl,-0x2fffffff(%rax)
-   29a1cb1d9:	adc    $0x1b,%al
-   29a1cb1db:	(bad)
-   29a1cb1dc:	add    (%rax),%al
+   29a1cb1d3:	add    %dl,0x1(%rax)
+   29a1cb1d9:	adc    $0x29a1b,%eax
    29a1cb1de:	add    %al,(%rax)
    29a1cb1e0:	addl   $0x0,(%rax)
    29a1cb1e6:	add    %al,(%rax)
    29a1cb1e8:	rex.B (bad)
    29a1cb1ea:	adc    %al,-0x7ce7f1bf(%rdx,%rax,1)
    29a1cb1f1:	add    0x40(%rsi,%rcx,1),%eax
    29a1cb1f5:	or     %gs:(%rsi),%cl
@@ -27851,19 +27894,20 @@
    29a1cb21a:	(bad)
    29a1cb21b:	or     %al,(%rax)
    29a1cb21d:	add    %al,(%rax)
    29a1cb21f:	add    %dl,(%rax,%rax,1)
    29a1cb222:	add    %al,(%rax)
    29a1cb224:	nop
    29a1cb225:	add    %eax,(%rax)
-   29a1cb227:	add    %ah,0x15(%rax)
-   29a1cb22a:	sbb    0x2(%rdx),%ebx
-   29a1cb230:	add    (%rax),%eax
-   29a1cb232:	add    %al,(%rax)
-   29a1cb234:	add    %al,(%rax)
+   29a1cb227:	add    %dl,0x29a1b15(%rax)
+   29a1cb22d:	add    %al,(%rax)
+   29a1cb22f:	add    %al,(%rbx)
+   29a1cb231:	add    %al,(%rax)
+   29a1cb233:	add    %al,(%rax)
+   29a1cb235:	add    %al,(%rax)
 	...
 
 000000029a1cb238 <.debug_frame>:
    29a1cb238:	adc    $0x0,%al
    29a1cb23a:	add    %al,(%rax)
    29a1cb23c:	(bad)
    29a1cb23d:	(bad)
@@ -27874,27 +27918,27 @@
    29a1cb245:	or     $0x7,%al
    29a1cb247:	or     %ah,0x1(%rax)
    29a1cb24d:	add    %al,(%rax)
    29a1cb24f:	add    %ah,(%rax,%rax,1)
    29a1cb252:	add    %al,(%rax)
    29a1cb254:	cmp    %al,(%rdx)
    29a1cb256:	add    %al,(%rax)
-   29a1cb258:	jo     29a1cb26f <.debug_frame+0x37>
-   29a1cb25a:	sbb    0x2(%rdx),%ebx
-   29a1cb260:	imul   $0x0,(%rax),%eax
-   29a1cb266:	add    %al,(%rax)
-   29a1cb268:	rex.B (bad)
+   29a1cb258:	movabs 0x69000000029a1b15,%al
+   29a1cb261:	add    %al,(%rax)
+   29a1cb263:	add    %al,(%rax)
+   29a1cb265:	add    %al,(%rax)
+   29a1cb267:	add    %al,0xe(%rcx)
    29a1cb26a:	adc    %al,-0x7ce7f1bf(%rdx,%rax,1)
    29a1cb271:	add    0x50(%rsi,%rcx,1),%eax
    29a1cb275:	add    %al,(%rax)
    29a1cb277:	add    %bh,(%rax,%rax,1)
    29a1cb27a:	add    %al,(%rax)
    29a1cb27c:	cmp    %al,(%rdx)
    29a1cb27e:	add    %al,(%rax)
-   29a1cb280:	loopne 29a1cb297 <.debug_frame+0x5f>
+   29a1cb280:	adc    %dl,(%rsi)
    29a1cb282:	sbb    0x2(%rdx),%ebx
    29a1cb288:	(bad)
    29a1cb28d:	add    %al,(%rax)
    29a1cb28f:	add    %al,0xe(%rcx)
    29a1cb292:	adc    %al,0x180e4102(%rbp)
    29a1cb298:	test   %al,(%rbx)
    29a1cb29a:	rex.B (bad)
@@ -27909,21 +27953,21 @@
    29a1cb2b1:	(bad)
    29a1cb2b2:	or     %al,0x0(%rbx,%rcx,1)
    29a1cb2b6:	add    %al,(%rax)
    29a1cb2b8:	pop    %rsp
    29a1cb2b9:	add    %al,(%rax)
    29a1cb2bb:	add    %bh,(%rax)
    29a1cb2bd:	add    (%rax),%al
-   29a1cb2bf:	add    %dl,0x17(%rax)
-   29a1cb2c2:	sbb    0x2(%rdx),%ebx
-   29a1cb2c8:	pop    %rbp
-   29a1cb2c9:	add    (%rax),%eax
-   29a1cb2cb:	add    %al,(%rax)
-   29a1cb2cd:	add    %al,(%rax)
-   29a1cb2cf:	add    %al,0xe(%rcx)
+   29a1cb2bf:	add    %al,0x29a1b17(%rax)
+   29a1cb2c5:	add    %al,(%rax)
+   29a1cb2c7:	add    %bl,0x3(%rbp)
+   29a1cb2ca:	add    %al,(%rax)
+   29a1cb2cc:	add    %al,(%rax)
+   29a1cb2ce:	add    %al,(%rax)
+   29a1cb2d0:	rex.B (bad)
    29a1cb2d2:	adc    %al,0x180e4202(%rsi)
    29a1cb2d8:	pop    (%rbx)
    29a1cb2da:	rex.X (bad)
    29a1cb2dc:	and    %cl,0x280e4204(%rsi)
    29a1cb2e2:	lea    -0x73cff1be(%rip),%eax        # 2264cc12a <__size_of_stack_reserve__+0x2262cc12a>
    29a1cb2e8:	(bad)
    29a1cb2e9:	rex.B (bad)
@@ -27958,17 +28002,20 @@
    29a1cb323:	js     29a1cb345 <.debug_frame+0x2d>
    29a1cb325:	or     $0x7,%al
    29a1cb327:	or     %ah,0x1(%rax)
    29a1cb32d:	add    %al,(%rax)
    29a1cb32f:	add    %cl,0x0(%rax,%rax,1)
    29a1cb333:	add    %bl,(%rax)
    29a1cb335:	add    (%rax),%eax
-   29a1cb337:	add    %dh,0x29a1b1a(%rax)
-   29a1cb33d:	add    %al,(%rax)
-   29a1cb33f:	add    %dh,0x0(%rax)
+   29a1cb337:	add    %ah,%al
+   29a1cb339:	sbb    (%rbx),%bl
+   29a1cb33b:	(bad)
+   29a1cb33c:	add    (%rax),%al
+   29a1cb33e:	add    %al,(%rax)
+   29a1cb340:	jo     29a1cb342 <.debug_frame+0x2a>
    29a1cb342:	add    %al,(%rax)
    29a1cb344:	add    %al,(%rax)
    29a1cb346:	add    %al,(%rax)
    29a1cb348:	rex.X (bad)
    29a1cb34a:	adc    %cl,-0x79e7f1bf(%rdx,%rax,1)
    29a1cb351:	add    0xe(%rcx),%eax
    29a1cb354:	and    %al,0x280e4104(%rbp)
@@ -27989,16 +28036,19 @@
    29a1cb37a:	(bad)
    29a1cb37b:	or     %al,(%rax)
    29a1cb37d:	add    %al,(%rax)
    29a1cb37f:	add    %bh,(%rax,%rax,1)
    29a1cb382:	add    %al,(%rax)
    29a1cb384:	sbb    %al,(%rbx)
    29a1cb386:	add    %al,(%rax)
-   29a1cb388:	and    %bl,(%rbx)
-   29a1cb38a:	sbb    0x2(%rdx),%ebx
+   29a1cb388:	push   %rax
+   29a1cb389:	sbb    (%rbx),%ebx
+   29a1cb38b:	(bad)
+   29a1cb38c:	add    (%rax),%al
+   29a1cb38e:	add    %al,(%rax)
    29a1cb390:	outsl  %ds:(%rsi),(%dx)
    29a1cb391:	add    %al,(%rax)
    29a1cb393:	add    %al,(%rax)
    29a1cb395:	add    %al,(%rax)
    29a1cb397:	add    %al,0xe(%rcx)
    29a1cb39a:	adc    %al,0x180e4102(%rbp)
    29a1cb3a0:	test   %al,(%rbx)
@@ -28014,19 +28064,22 @@
    29a1cb3b8:	(bad)
    29a1cb3b9:	or     %al,0xb(%rcx)
    29a1cb3bc:	add    %al,(%rax)
    29a1cb3be:	add    %al,(%rax)
    29a1cb3c0:	add    %r8b,(%rax)
    29a1cb3c3:	add    %bl,(%rax)
    29a1cb3c5:	add    (%rax),%eax
-   29a1cb3c7:	add    %dl,0x29a1b1b(%rax)
-   29a1cb3cd:	add    %al,(%rax)
-   29a1cb3cf:	add    %al,0x0(%rcx)
-   29a1cb3d5:	add    %al,(%rax)
-   29a1cb3d7:	add    %al,0xe(%rcx)
+   29a1cb3c7:	add    %al,%al
+   29a1cb3c9:	sbb    (%rbx),%ebx
+   29a1cb3cb:	(bad)
+   29a1cb3cc:	add    (%rax),%al
+   29a1cb3ce:	add    %al,(%rax)
+   29a1cb3d0:	addl   $0x0,(%rax)
+   29a1cb3d6:	add    %al,(%rax)
+   29a1cb3d8:	rex.B (bad)
    29a1cb3da:	adc    %al,-0x7ce7f1bf(%rdx,%rax,1)
    29a1cb3e1:	add    0x40(%rsi,%rcx,1),%eax
    29a1cb3e5:	push   %rdx
    29a1cb3e6:	or     (%rsi),%cl
    29a1cb3e8:	sbb    %al,-0x3d(%rcx)
    29a1cb3eb:	(bad)
    29a1cb3ec:	adc    %al,-0x3c(%rcx)
@@ -28041,15 +28094,16 @@
    29a1cb3ff:	or     %al,0x0(%rbx,%rcx,1)
    29a1cb403:	add    %al,(%rax)
    29a1cb405:	add    %al,(%rax)
    29a1cb407:	add    %dh,(%rax,%rax,1)
    29a1cb40a:	add    %al,(%rax)
    29a1cb40c:	sbb    %al,(%rbx)
    29a1cb40e:	add    %al,(%rax)
-   29a1cb410:	and    %bl,(%rbx,%rbx,1)
+   29a1cb410:	push   %rax
+   29a1cb411:	sbb    $0x1b,%al
    29a1cb413:	(bad)
    29a1cb414:	add    (%rax),%al
    29a1cb416:	add    %al,(%rax)
    29a1cb418:	repnz add %al,(%rax)
    29a1cb41b:	add    %al,(%rax)
    29a1cb41d:	add    %al,(%rax)
    29a1cb41f:	add    %al,0xe(%rcx)
@@ -28077,34 +28131,35 @@
    29a1cb44b:	js     29a1cb46d <.debug_frame+0x2d>
    29a1cb44d:	or     $0x7,%al
    29a1cb44f:	or     %ah,0x1(%rax)
    29a1cb455:	add    %al,(%rax)
    29a1cb457:	add    %dl,(%rax,%rax,1)
    29a1cb45a:	add    %al,(%rax)
    29a1cb45c:	rex add $0x0,%al
-   29a1cb45f:	add    %ah,(%rax)
-   29a1cb461:	sbb    $0x29a1b,%eax
-   29a1cb466:	add    %al,(%rax)
+   29a1cb45f:	add    %dl,0x1d(%rax)
+   29a1cb462:	sbb    0x2(%rdx),%ebx
    29a1cb468:	sub    $0x0,%al
    29a1cb46a:	add    %al,(%rax)
    29a1cb46c:	add    %al,(%rax)
    29a1cb46e:	add    %al,(%rax)
    29a1cb470:	adc    $0x0,%al
    29a1cb472:	add    %al,(%rax)
    29a1cb474:	rex add $0x0,%al
-   29a1cb477:	add    %dl,0x1d(%rax)
-   29a1cb47a:	sbb    0x2(%rdx),%ebx
-   29a1cb480:	push   %rax
-   29a1cb481:	add    %al,(%rax)
-   29a1cb483:	add    %al,(%rax)
-   29a1cb485:	add    %al,(%rax)
-   29a1cb487:	add    %cl,0x0(%rax,%rax,1)
+   29a1cb477:	add    %al,0x29a1b1d(%rax)
+   29a1cb47d:	add    %al,(%rax)
+   29a1cb47f:	add    %dl,0x0(%rax)
+   29a1cb482:	add    %al,(%rax)
+   29a1cb484:	add    %al,(%rax)
+   29a1cb486:	add    %al,(%rax)
+   29a1cb488:	rex.WR add %r8b,(%rax)
    29a1cb48b:	add    %al,0x4(%rax)
    29a1cb48e:	add    %al,(%rax)
-   29a1cb490:	movabs 0x9d000000029a1b1d,%al
+   29a1cb490:	rcrb   $1,0x29a1b(%rip)        # 29a1f4eb1 <.debug_rnglists+0x24e0d>
+   29a1cb496:	add    %al,(%rax)
+   29a1cb498:	popf
    29a1cb499:	add    %al,(%rax)
    29a1cb49b:	add    %al,(%rax)
    29a1cb49d:	add    %al,(%rax)
    29a1cb49f:	add    %al,0xe(%rcx)
    29a1cb4a2:	adc    %al,0x180e4102(%rbp)
    29a1cb4a8:	test   %al,(%rbx)
    29a1cb4aa:	rex.B (bad)
@@ -28126,64 +28181,65 @@
    29a1cb4cf:	adc    %al,-0x3b(%rcx)
    29a1cb4d2:	(bad)
    29a1cb4d3:	or     %al,(%rax)
    29a1cb4d5:	add    %al,(%rax)
    29a1cb4d7:	add    %dl,(%rax,%rax,1)
    29a1cb4da:	add    %al,(%rax)
    29a1cb4dc:	rex add $0x0,%al
-   29a1cb4df:	add    %al,0x1e(%rax)
+   29a1cb4df:	add    %dh,0x1e(%rax)
    29a1cb4e2:	sbb    0x2(%rdx),%ebx
    29a1cb4e8:	addb   $0x0,(%rax)
    29a1cb4eb:	add    %al,(%rax)
    29a1cb4ed:	add    %al,(%rax)
    29a1cb4ef:	add    %dl,(%rax,%rax,1)
    29a1cb4f2:	add    %al,(%rax)
    29a1cb4f4:	rex add $0x0,%al
-   29a1cb4f7:	add    %al,%al
+   29a1cb4f7:	add    %dh,%al
    29a1cb4f9:	(bad)
    29a1cb4fa:	sbb    0x2(%rdx),%ebx
    29a1cb500:	(bad)
    29a1cb501:	add    %al,(%rax)
    29a1cb503:	add    %al,(%rax)
    29a1cb505:	add    %al,(%rax)
    29a1cb507:	add    %dl,(%rax,%rax,1)
    29a1cb50a:	add    %al,(%rax)
    29a1cb50c:	rex add $0x0,%al
-   29a1cb50f:	add    %al,(%rax)
+   29a1cb50f:	add    %dh,(%rax)
    29a1cb511:	(bad)
    29a1cb512:	sbb    0x2(%rdx),%ebx
    29a1cb518:	jae    29a1cb51a <.debug_frame+0xda>
    29a1cb51a:	add    %al,(%rax)
    29a1cb51c:	add    %al,(%rax)
    29a1cb51e:	add    %al,(%rax)
    29a1cb520:	adc    $0x0,%al
    29a1cb522:	add    %al,(%rax)
    29a1cb524:	rex add $0x0,%al
-   29a1cb527:	add    %al,0x29a1b1f(%rax)
+   29a1cb527:	add    %dh,0x29a1b1f(%rax)
    29a1cb52d:	add    %al,(%rax)
    29a1cb52f:	add    %dh,(%rsi)
    29a1cb531:	add    %al,(%rax)
    29a1cb533:	add    %al,(%rax)
    29a1cb535:	add    %al,(%rax)
    29a1cb537:	add    %dl,(%rax,%rax,1)
    29a1cb53a:	add    %al,(%rax)
    29a1cb53c:	rex add $0x0,%al
-   29a1cb53f:	add    %al,%al
+   29a1cb53f:	add    %dh,%al
    29a1cb541:	(bad)
    29a1cb542:	sbb    0x2(%rdx),%ebx
    29a1cb548:	mov    %eax,(%rax)
    29a1cb54a:	add    %al,(%rax)
    29a1cb54c:	add    %al,(%rax)
    29a1cb54e:	add    %al,(%rax)
    29a1cb550:	adc    $0x0,%al
    29a1cb552:	add    %al,(%rax)
    29a1cb554:	rex add $0x0,%al
-   29a1cb557:	add    %dl,0x20(%rax)
-   29a1cb55a:	sbb    0x2(%rdx),%ebx
-   29a1cb560:	movb   $0x0,(%rax)
+   29a1cb557:	add    %al,0x29a1b20(%rax)
+   29a1cb55d:	add    %al,(%rax)
+   29a1cb55f:	add    %al,%dh
+   29a1cb561:	add    %al,(%rax)
    29a1cb563:	add    %al,(%rax)
    29a1cb565:	add    %al,(%rax)
 	...
 
 000000029a1cb568 <.debug_frame>:
    29a1cb568:	adc    $0x0,%al
    29a1cb56a:	add    %al,(%rax)
@@ -28194,15 +28250,15 @@
    29a1cb571:	add    %al,(%rcx)
    29a1cb573:	js     29a1cb595 <.debug_frame+0x2d>
    29a1cb575:	or     $0x7,%al
    29a1cb577:	or     %ah,0x1(%rax)
    29a1cb57d:	add    %al,(%rax)
    29a1cb57f:	add    %dl,(%rax,%rax,1)
    29a1cb582:	add    %al,(%rax)
-   29a1cb584:	push   $0x20000005
+   29a1cb584:	push   $0x50000005
    29a1cb589:	and    %ebx,(%rbx)
    29a1cb58b:	(bad)
    29a1cb58c:	add    (%rax),%al
    29a1cb58e:	add    %al,(%rax)
    29a1cb590:	add    (%rax),%eax
    29a1cb592:	add    %al,(%rax)
    29a1cb594:	add    %al,(%rax)
@@ -28219,15 +28275,15 @@
    29a1cb5a3:	js     29a1cb5c5 <.debug_frame+0x2d>
    29a1cb5a5:	or     $0x7,%al
    29a1cb5a7:	or     %ah,0x1(%rax)
    29a1cb5ad:	add    %al,(%rax)
    29a1cb5af:	add    %dl,(%rax,%rax,1)
    29a1cb5b2:	add    %al,(%rax)
    29a1cb5b4:	cwtl
-   29a1cb5b5:	add    $0x21700000,%eax
+   29a1cb5b5:	add    $0x21a00000,%eax
    29a1cb5ba:	sbb    0x2(%rdx),%ebx
    29a1cb5c0:	(bad)
    29a1cb5c1:	add    %al,(%rax)
    29a1cb5c3:	add    %al,(%rax)
    29a1cb5c5:	add    %al,(%rax)
 	...
 
@@ -28242,18 +28298,16 @@
    29a1cb5d3:	js     29a1cb5f5 <.debug_frame+0x2d>
    29a1cb5d5:	or     $0x7,%al
    29a1cb5d7:	or     %ah,0x1(%rax)
    29a1cb5dd:	add    %al,(%rax)
    29a1cb5df:	add    %dl,(%rax,%rax,1)
    29a1cb5e2:	add    %al,(%rax)
    29a1cb5e4:	enter  $0x5,$0x0
-   29a1cb5e8:	andb   $0x1b,(%rcx)
-   29a1cb5eb:	(bad)
-   29a1cb5ec:	add    (%rax),%al
-   29a1cb5ee:	add    %al,(%rax)
+   29a1cb5e8:	mov    $0x21,%al
+   29a1cb5ea:	sbb    0x2(%rdx),%ebx
    29a1cb5f0:	(bad)
    29a1cb5f1:	add    %al,(%rax)
    29a1cb5f3:	add    %al,(%rax)
    29a1cb5f5:	add    %al,(%rax)
 	...
 
 000000029a1cb5f8 <.debug_frame>:
@@ -28267,15 +28321,15 @@
    29a1cb603:	js     29a1cb625 <.debug_frame+0x2d>
    29a1cb605:	or     $0x7,%al
    29a1cb607:	or     %ah,0x1(%rax)
    29a1cb60d:	add    %al,(%rax)
    29a1cb60f:	add    %bl,(%rax,%rax,1)
    29a1cb612:	add    %al,(%rax)
    29a1cb614:	clc
-   29a1cb615:	add    $0x21900000,%eax
+   29a1cb615:	add    $0x21c00000,%eax
    29a1cb61a:	sbb    0x2(%rdx),%ebx
    29a1cb620:	(bad)
    29a1cb621:	add    %al,(%rax)
    29a1cb623:	add    %al,(%rax)
    29a1cb625:	add    %al,(%rax)
    29a1cb627:	add    %al,0x40(%rsi,%rcx,1)
    29a1cb62b:	pop    %rcx
@@ -28295,25 +28349,25 @@
    29a1cb63d:	or     $0x7,%al
    29a1cb63f:	or     %ah,0x1(%rax)
    29a1cb645:	add    %al,(%rax)
    29a1cb647:	add    %dl,(%rax,%rax,1)
    29a1cb64a:	add    %al,(%rax)
    29a1cb64c:	xor    %al,(%rsi)
    29a1cb64e:	add    %al,(%rax)
-   29a1cb650:	mov    $0x21,%al
+   29a1cb650:	loopne 29a1cb673 <.debug_frame+0x43>
    29a1cb652:	sbb    0x2(%rdx),%ebx
    29a1cb658:	add    (%rax),%eax
    29a1cb65a:	add    %al,(%rax)
    29a1cb65c:	add    %al,(%rax)
    29a1cb65e:	add    %al,(%rax)
    29a1cb660:	rex.WR add %r8b,(%rax)
    29a1cb663:	add    %dh,(%rax)
    29a1cb665:	(bad)
    29a1cb666:	add    %al,(%rax)
-   29a1cb668:	shlb   $0x1b,(%rcx)
+   29a1cb668:	lock and %ebx,(%rbx)
    29a1cb66b:	(bad)
    29a1cb66c:	add    (%rax),%al
    29a1cb66e:	add    %al,(%rax)
    29a1cb670:	push   $0x0
    29a1cb672:	add    %al,(%rax)
    29a1cb674:	add    %al,(%rax)
    29a1cb676:	add    %al,(%rax)
@@ -28338,16 +28392,19 @@
    29a1cb6aa:	(bad)
    29a1cb6ab:	or     %al,(%rax)
    29a1cb6ad:	add    %al,(%rax)
    29a1cb6af:	add    %cl,0x0(%rax,%rax,1)
    29a1cb6b3:	add    %dh,(%rax)
    29a1cb6b5:	(bad)
    29a1cb6b6:	add    %al,(%rax)
-   29a1cb6b8:	xor    %ah,(%rdx)
-   29a1cb6ba:	sbb    0x2(%rdx),%ebx
+   29a1cb6b8:	(bad)
+   29a1cb6b9:	and    (%rbx),%bl
+   29a1cb6bb:	(bad)
+   29a1cb6bc:	add    (%rax),%al
+   29a1cb6be:	add    %al,(%rax)
    29a1cb6c0:	push   $0x0
    29a1cb6c2:	add    %al,(%rax)
    29a1cb6c4:	add    %al,(%rax)
    29a1cb6c6:	add    %al,(%rax)
    29a1cb6c8:	rex.X (bad)
    29a1cb6ca:	adc    %cl,-0x79e7f1bf(%rdx,%rax,1)
    29a1cb6d1:	add    0xe(%rcx),%eax
@@ -28369,78 +28426,80 @@
    29a1cb6fa:	(bad)
    29a1cb6fb:	or     %al,(%rax)
    29a1cb6fd:	add    %al,(%rax)
    29a1cb6ff:	add    %ah,(%rax,%rax,1)
    29a1cb702:	add    %al,(%rax)
    29a1cb704:	xor    %al,(%rsi)
    29a1cb706:	add    %al,(%rax)
-   29a1cb708:	movabs 0x1e000000029a1b22,%al
+   29a1cb708:	shlb   $1,(%rdx)
+   29a1cb70a:	sbb    0x2(%rdx),%ebx
+   29a1cb710:	(bad)
    29a1cb711:	add    %al,(%rax)
    29a1cb713:	add    %al,(%rax)
    29a1cb715:	add    %al,(%rax)
    29a1cb717:	add    %al,0xe(%rcx)
    29a1cb71a:	adc    %al,0x300e4402(%rbx)
    29a1cb720:	push   %rdi
    29a1cb721:	(bad)
    29a1cb722:	adc    %al,-0x3d(%rcx)
    29a1cb725:	(bad)
    29a1cb726:	or     %al,(%rax)
    29a1cb728:	adc    $0x0,%al
    29a1cb72a:	add    %al,(%rax)
    29a1cb72c:	xor    %al,(%rsi)
    29a1cb72e:	add    %al,(%rax)
-   29a1cb730:	shlb   $0x1b,(%rdx)
+   29a1cb730:	lock and (%rbx),%bl
    29a1cb733:	(bad)
    29a1cb734:	add    (%rax),%al
    29a1cb736:	add    %al,(%rax)
    29a1cb738:	adc    $0x0,%eax
    29a1cb73d:	add    %al,(%rax)
    29a1cb73f:	add    %bl,(%rax,%rax,1)
    29a1cb742:	add    %al,(%rax)
    29a1cb744:	xor    %al,(%rsi)
    29a1cb746:	add    %al,(%rax)
-   29a1cb748:	loopne 29a1cb76c <.debug_frame+0x13c>
+   29a1cb748:	adc    %ah,(%rbx)
    29a1cb74a:	sbb    0x2(%rdx),%ebx
    29a1cb750:	cs add %al,(%rax)
    29a1cb753:	add    %al,(%rax)
    29a1cb755:	add    %al,(%rax)
    29a1cb757:	add    %al,0xe(%rcx)
    29a1cb75a:	adc    %al,0x300e4402(%rbx)
    29a1cb760:	sbb    $0x0,%al
    29a1cb762:	add    %al,(%rax)
    29a1cb764:	xor    %al,(%rsi)
    29a1cb766:	add    %al,(%rax)
-   29a1cb768:	adc    %ah,(%rbx)
-   29a1cb76a:	sbb    0x2(%rdx),%ebx
+   29a1cb768:	rex and (%rbx),%ebx
+   29a1cb76b:	(bad)
+   29a1cb76c:	add    (%rax),%al
+   29a1cb76e:	add    %al,(%rax)
    29a1cb770:	xor    $0x0,%eax
    29a1cb775:	add    %al,(%rax)
    29a1cb777:	add    %al,0x50(%rsi,%rcx,1)
    29a1cb77b:	jo     29a1cb78b <.debug_frame+0x15b>
    29a1cb77d:	or     %al,(%rax)
    29a1cb77f:	add    %bl,(%rax,%rax,1)
    29a1cb782:	add    %al,(%rax)
    29a1cb784:	xor    %al,(%rsi)
    29a1cb786:	add    %al,(%rax)
-   29a1cb788:	push   %rax
-   29a1cb789:	and    (%rbx),%ebx
+   29a1cb788:	andb   $0x1b,(%rbx)
    29a1cb78b:	(bad)
    29a1cb78c:	add    (%rax),%al
    29a1cb78e:	add    %al,(%rax)
    29a1cb790:	ss add %al,(%rax)
    29a1cb793:	add    %al,(%rax)
    29a1cb795:	add    %al,(%rax)
    29a1cb797:	add    %al,0x30(%rsi,%rcx,1)
    29a1cb79b:	jno    29a1cb7ab <.debug_frame+0x17b>
    29a1cb79d:	or     %al,(%rax)
    29a1cb79f:	add    %bl,(%rax,%rax,1)
    29a1cb7a2:	add    %al,(%rax)
    29a1cb7a4:	xor    %al,(%rsi)
    29a1cb7a6:	add    %al,(%rax)
-   29a1cb7a8:	nop
-   29a1cb7a9:	and    (%rbx),%ebx
+   29a1cb7a8:	shlb   $0x1b,(%rbx)
    29a1cb7ab:	(bad)
    29a1cb7ac:	add    (%rax),%al
    29a1cb7ae:	add    %al,(%rax)
    29a1cb7b0:	ss add %al,(%rax)
    29a1cb7b3:	add    %al,(%rax)
    29a1cb7b5:	add    %al,(%rax)
    29a1cb7b7:	add    %al,0x30(%rsi,%rcx,1)
@@ -28459,18 +28518,16 @@
    29a1cb7cb:	js     29a1cb7ed <.debug_frame+0x2d>
    29a1cb7cd:	or     $0x7,%al
    29a1cb7cf:	or     %ah,0x1(%rax)
    29a1cb7d5:	add    %al,(%rax)
    29a1cb7d7:	add    %bl,(%rax,%rax,1)
    29a1cb7da:	add    %al,(%rax)
    29a1cb7dc:	rolb   $0x0,(%rdi)
-   29a1cb7df:	add    %dh,%al
-   29a1cb7e1:	and    $0x1b,%al
-   29a1cb7e3:	(bad)
-   29a1cb7e4:	add    (%rax),%al
+   29a1cb7df:	add    %dh,(%rax)
+   29a1cb7e1:	and    $0x29a1b,%eax
    29a1cb7e6:	add    %al,(%rax)
    29a1cb7e8:	xor    (%rax),%al
    29a1cb7ea:	add    %al,(%rax)
    29a1cb7ec:	add    %al,(%rax)
    29a1cb7ee:	add    %al,(%rax)
    29a1cb7f0:	rex.R (bad)
    29a1cb7f2:	push   %rax
```

### Comparing `advanced_input-0.1.3/advanced_input.egg-info/PKG-INFO` & `advanced_input-0.2.0/advanced_input.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: advanced_input
-Version: 0.1.3
+Version: 0.2.0
 Summary: IO Extention
 Home-page: https://github.com/NightKey/advanced-input
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/advanced-input/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freeware
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Advanced Input
 
 Advanced input for python, where you can read in just one character or have inputs priority ordered.
```

