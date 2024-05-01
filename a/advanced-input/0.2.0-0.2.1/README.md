# Comparing `tmp/advanced_input-0.2.0.tar.gz` & `tmp/advanced_input-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advanced_input-0.2.0.tar", last modified: Wed May  1 07:24:48 2024, max compression
+gzip compressed data, was "advanced_input-0.2.1.tar", last modified: Wed May  1 09:14:21 2024, max compression
```

## Comparing `advanced_input-0.2.0.tar` & `advanced_input-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 07:24:48.874633 advanced_input-0.2.0/
--rw-rw-rw-   0        0        0     1235 2020-07-21 09:29:29.000000 advanced_input-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1685 2024-05-01 07:24:48.873631 advanced_input-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2024-04-26 06:22:56.000000 advanced_input-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 07:24:48.859021 advanced_input-0.2.0/advanced_input/
--rw-rw-rw-   0        0        0      564 2024-05-01 07:02:14.000000 advanced_input-0.2.0/advanced_input/__init__.py
--rw-rw-rw-   0        0        0      316 2024-04-25 10:42:38.000000 advanced_input-0.2.0/advanced_input/constants.py
--rw-rw-rw-   0        0        0     3168 2024-05-01 07:18:53.000000 advanced_input-0.2.0/advanced_input/input.py
--rw-rw-rw-   0        0        0     1245 2024-05-01 07:19:39.000000 advanced_input-0.2.0/advanced_input/inputExtention.c
--rw-rw-rw-   0        0        0   107263 2024-05-01 07:19:44.000000 advanced_input-0.2.0/advanced_input/inputExtention.dll
--rw-rw-rw-   0        0        0    16096 2024-05-01 07:22:41.000000 advanced_input-0.2.0/advanced_input/inputExtention.so
-drwxrwxrwx   0        0        0        0 2024-05-01 07:24:48.873631 advanced_input-0.2.0/advanced_input.egg-info/
--rw-rw-rw-   0        0        0     1685 2024-05-01 07:24:48.000000 advanced_input-0.2.0/advanced_input.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-05-01 07:24:48.000000 advanced_input-0.2.0/advanced_input.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 07:24:48.000000 advanced_input-0.2.0/advanced_input.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-01 07:24:48.000000 advanced_input-0.2.0/advanced_input.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-12-08 11:06:28.000000 advanced_input-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      653 2024-05-01 07:24:48.875629 advanced_input-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 09:14:21.417767 advanced_input-0.2.1/
+-rw-rw-rw-   0        0        0     1235 2020-07-21 09:29:29.000000 advanced_input-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2053 2024-05-01 09:14:21.417767 advanced_input-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1512 2024-05-01 09:05:26.000000 advanced_input-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 09:14:21.404816 advanced_input-0.2.1/advanced_input/
+-rw-rw-rw-   0        0        0      633 2024-05-01 07:41:25.000000 advanced_input-0.2.1/advanced_input/__init__.py
+-rw-rw-rw-   0        0        0      316 2024-04-25 10:42:38.000000 advanced_input-0.2.1/advanced_input/constants.py
+-rw-rw-rw-   0        0        0     3213 2024-05-01 07:59:15.000000 advanced_input-0.2.1/advanced_input/input.py
+-rw-rw-rw-   0        0        0     1225 2024-05-01 08:03:10.000000 advanced_input-0.2.1/advanced_input/inputExtention.c
+-rw-rw-rw-   0        0        0   107088 2024-05-01 09:14:06.000000 advanced_input-0.2.1/advanced_input/inputExtention.dll
+-rw-rw-rw-   0        0        0    16000 2024-05-01 09:14:09.000000 advanced_input-0.2.1/advanced_input/inputExtention.so
+drwxrwxrwx   0        0        0        0 2024-05-01 09:14:21.416736 advanced_input-0.2.1/advanced_input.egg-info/
+-rw-rw-rw-   0        0        0     2053 2024-05-01 09:14:21.000000 advanced_input-0.2.1/advanced_input.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-05-01 09:14:21.000000 advanced_input-0.2.1/advanced_input.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 09:14:21.000000 advanced_input-0.2.1/advanced_input.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-01 09:14:21.000000 advanced_input-0.2.1/advanced_input.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-12-08 11:06:28.000000 advanced_input-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      653 2024-05-01 09:14:21.419325 advanced_input-0.2.1/setup.cfg
```

### Comparing `advanced_input-0.2.0/LICENSE` & `advanced_input-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `advanced_input-0.2.0/PKG-INFO` & `advanced_input-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advanced_input
-Version: 0.2.0
+Version: 0.2.1
 Summary: IO Extention
 Home-page: https://github.com/NightKey/advanced-input
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/advanced-input/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -38,7 +38,12 @@
     input_handler.read("Press any character to exit...", PriorityOrder.Low)
     input_handler.stop()
 ```
 
 This will result in a user input for `thread_one` being created before the `main` function's exit will be available. Normally, this would result in the program exiting, before accepting the user input of `thread_one`. With this, thread one will be in a higher priority than `main`, and that will be the first to be served the user's input. Additionally, `Read()` returns when one character is pressed.
 
 If there are multiple inputs with the same priority, it will return them in a first come last serve method.
+
+## Windows quirks
+
+Due to how Windows works with new line (\r\n), on Windows it is not possible to read the "Carriage Return" (\r) character. It will always return "Line Feed" (\n) instead.
+Due to how Windows console works, the default (utf-8) encoding input will not work with some special character. For it to work, please specify the encoding of your system.
```

### Comparing `advanced_input-0.2.0/advanced_input/__init__.py` & `advanced_input-0.2.1/advanced_input/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from .input import AdvancedInput, is_input_ready, get_character_from_input
 from .constants import PriorityOrder, EventType, EventWithType
 from platform import system
+import atexit
 current_input_extender: AdvancedInput = None
 
 def get_advanced_input(encoding: str = None):
     global current_input_extender
     if encoding is None:
         encoding = "cp850" if system() == "Windows" else "utf-8"
     if current_input_extender is None:
         current_input_extender = AdvancedInput(encoding)
         current_input_extender.start()
+        atexit.register(current_input_extender.stop)
     return current_input_extender
```

### Comparing `advanced_input-0.2.0/advanced_input/input.py` & `advanced_input-0.2.1/advanced_input/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     def start(self) -> None:
         self.stop_event.clear()
         self.main_thread = Thread(target=self.__loop)
         self.main_thread.name = "Advanced Input Reader Thread"
         self.main_thread.start()
 
     def stop(self) -> None:
+        if self.main_thread is None: return
         self.stop_event.set()
         self.main_thread.join()
         self.main_thread = None
         inputExtentionStop()
 
     def input(self, prompt: str = None, priority: PriorityOrder = PriorityOrder.Normal) -> str:
         input_event = EventWithType(EventType.LINE)
```

### Comparing `advanced_input-0.2.0/advanced_input/inputExtention.c` & `advanced_input-0.2.1/advanced_input/inputExtention.c`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 void init() {
     #ifdef LINUX
     tcgetattr( STDIN_FILENO, &oldt);
     newt = oldt;
     newt.c_lflag &= ~(ICANON | ECHO);
     tcsetattr( STDIN_FILENO, TCSANOW, &newt);
     #endif
-    fflush(stdin);
     return;
 }
 
 int isInputReady() {
     return kbhit();
 }
```

### Comparing `advanced_input-0.2.0/advanced_input/inputExtention.dll` & `advanced_input-0.2.1/advanced_input/inputExtention.dll`

 * *Files 2% similar despite different names*

#### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Wed May  1 07:19:44 2024
+Time/Date		Wed May  1 09:14:06 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	41
 SizeOfCode		0000000000001600
 SizeOfInitializedData	0000000000003800
 SizeOfUninitializedData	0000000000000200
 AddressOfEntryPoint	0000000000001330
@@ -26,157 +26,156 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00021000
 SizeOfHeaders		00000600
-CheckSum		00021edf
+CheckSum		00025db8
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
-Entry 1 0000000000009000 00000870 Import Directory [parts of .idata]
+Entry 1 0000000000009000 00000854 Import Directory [parts of .idata]
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
-Entry c 0000000000009250 00000198 Import Address Table Directory
+Entry c 0000000000009248 00000190 Import Address Table Directory
 Entry d 0000000000000000 00000000 Delay Import Directory
 Entry e 0000000000000000 00000000 CLR Runtime Header
 Entry f 0000000000000000 00000000 Reserved
 
 There is an import table in .idata at 0x29a1b9000
 
 The Import Tables (interpreted .idata section contents)
  vma:            Hint    Time      Forward  DLL       First
                  Table   Stamp     Chain    Name      Thunk
- 00009000	000090b8 00000000 00000000 000096e8 00009250
+ 00009000	000090b8 00000000 00000000 000096d0 00009248
 
 	DLL Name: KERNEL32.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	93e8	  293  DeleteCriticalSection
-	9400	  331  EnterCriticalSection
-	9418	  644  GetLastError
-	9428	  914  InitializeCriticalSection
-	9444	 1008  LeaveCriticalSection
-	945c	 1444  Sleep
-	9464	 1480  TlsGetValue
-	9472	 1527  VirtualProtect
-	9484	 1529  VirtualQuery
+	93d8	  293  DeleteCriticalSection
+	93f0	  331  EnterCriticalSection
+	9408	  644  GetLastError
+	9418	  914  InitializeCriticalSection
+	9434	 1008  LeaveCriticalSection
+	944c	 1444  Sleep
+	9454	 1480  TlsGetValue
+	9462	 1527  VirtualProtect
+	9474	 1529  VirtualQuery
 
- 00009014	00009108 00000000 00000000 000096fc 000092a0
+ 00009014	00009108 00000000 00000000 000096e4 00009298
 
 	DLL Name: api-ms-win-crt-conio-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	9494	   15  _getch
+	9484	   15  _getch
 
- 00009028	00009118 00000000 00000000 00009724 000092b0
+ 00009028	00009118 00000000 00000000 0000970c 000092a8
 
 	DLL Name: api-ms-win-crt-environment-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	949e	    1  __p__environ
-	94ae	    2  __p__wenviron
+	948e	    1  __p__environ
+	949e	    2  __p__wenviron
 
- 0000903c	00009130 00000000 00000000 00009758 000092c8
+ 0000903c	00009130 00000000 00000000 00009740 000092c0
 
 	DLL Name: api-ms-win-crt-heap-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	94be	   24  _set_new_mode
-	94ce	   25  calloc
-	94d8	   26  free
+	94ae	   24  _set_new_mode
+	94be	   25  calloc
+	94c8	   26  free
 
- 00009050	00009150 00000000 00000000 000097b4 000092e8
+ 00009050	00009150 00000000 00000000 0000979c 000092e0
 
 	DLL Name: api-ms-win-crt-runtime-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	94e0	    5  __p___argc
-	94ee	    6  __p___argv
-	94fc	    7  __p___wargv
-	950a	   25  _configure_narrow_argv
-	9524	   26  _configure_wide_argv
-	953c	   30  _crt_at_quick_exit
-	9552	   31  _crt_atexit
-	9560	   36  _execute_onexit_table
-	9578	   37  _exit
-	9580	   54  _initialize_narrow_environment
-	95a2	   55  _initialize_onexit_table
-	95be	   56  _initialize_wide_environment
-	95de	   57  _initterm
-	95ea	   63  _register_onexit_function
-	9606	   88  abort
+	94d0	    5  __p___argc
+	94de	    6  __p___argv
+	94ec	    7  __p___wargv
+	94fa	   25  _configure_narrow_argv
+	9514	   26  _configure_wide_argv
+	952c	   30  _crt_at_quick_exit
+	9542	   31  _crt_atexit
+	9550	   36  _execute_onexit_table
+	9568	   37  _exit
+	9570	   54  _initialize_narrow_environment
+	9592	   55  _initialize_onexit_table
+	95ae	   56  _initialize_wide_environment
+	95ce	   57  _initterm
+	95da	   63  _register_onexit_function
+	95f6	   88  abort
 
- 00009064	000091d0 00000000 00000000 000097f4 00009368
+ 00009064	000091d0 00000000 00000000 000097d8 00009360
 
 	DLL Name: api-ms-win-crt-stdio-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	960e	    1  __acrt_iob_func
-	9620	    4  __stdio_common_vfprintf
-	963a	    8  __stdio_common_vfwprintf
-	9656	   84  _kbhit
-	9660	  150  fflush
-	966a	  169  fwrite
-	9674	  177  putchar
+	95fe	    1  __acrt_iob_func
+	9610	    4  __stdio_common_vfprintf
+	962a	    8  __stdio_common_vfwprintf
+	9646	   84  _kbhit
+	9650	  169  fwrite
+	965a	  177  putchar
 
- 00009078	00009210 00000000 00000000 0000981c 000093a8
+ 00009078	00009208 00000000 00000000 00009800 00009398
 
 	DLL Name: api-ms-win-crt-string-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	967e	  168  strlen
-	9688	  171  strncmp
+	9664	  168  strlen
+	966e	  171  strncmp
 
- 0000908c	00009228 00000000 00000000 00009850 000093c0
+ 0000908c	00009220 00000000 00000000 00009834 000093b0
 
 	DLL Name: api-ms-win-crt-time-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	9692	    9  __daylight
-	96a0	   11  __timezone
-	96ae	   12  __tzname
-	96ba	   60  _tzset
+	9678	    9  __daylight
+	9686	   11  __timezone
+	9694	   12  __tzname
+	96a0	   60  _tzset
 
  000090a0	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x29a1b8000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		6631ed10
+Time/Date stamp 		663207de
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
-	[   0] +base[   1] 13b8 Export RVA
+	[   0] +base[   1] 139a Export RVA
 	[   1] +base[   2] 1380 Export RVA
-	[   2] +base[   3] 13a5 Export RVA
-	[   3] +base[   4] 13ec Export RVA
+	[   2] +base[   3] 1387 Export RVA
+	[   3] +base[   4] 13ce Export RVA
 
 [Ordinal/Name Pointer] Table
 	[   0] getCharacter
 	[   1] init
 	[   2] isInputReady
 	[   3] stop
 
@@ -185,55 +184,55 @@
  000000029a1b5000:	000000029a1b1000 000000029a1b100c 000000029a1b6000
  000000029a1b500c:	000000029a1b1010 000000029a1b11cf 000000029a1b6004
  000000029a1b5018:	000000029a1b11d0 000000029a1b1324 000000029a1b6018
  000000029a1b5024:	000000029a1b1330 000000029a1b1342 000000029a1b6028
  000000029a1b5030:	000000029a1b1350 000000029a1b135f 000000029a1b602c
  000000029a1b503c:	000000029a1b1360 000000029a1b136c 000000029a1b6030
  000000029a1b5048:	000000029a1b1370 000000029a1b1371 000000029a1b6034
- 000000029a1b5054:	000000029a1b1380 000000029a1b13a5 000000029a1b6038
- 000000029a1b5060:	000000029a1b13a5 000000029a1b13b8 000000029a1b6044
- 000000029a1b506c:	000000029a1b13b8 000000029a1b13ec 000000029a1b6050
- 000000029a1b5078:	000000029a1b13ec 000000029a1b13f3 000000029a1b605c
- 000000029a1b5084:	000000029a1b1400 000000029a1b143a 000000029a1b6064
- 000000029a1b5090:	000000029a1b1440 000000029a1b14aa 000000029a1b606c
- 000000029a1b509c:	000000029a1b14b0 000000029a1b14cf 000000029a1b6078
- 000000029a1b50a8:	000000029a1b14d0 000000029a1b14ff 000000029a1b607c
- 000000029a1b50b4:	000000029a1b1500 000000029a1b1581 000000029a1b6084
- 000000029a1b50c0:	000000029a1b1590 000000029a1b1593 000000029a1b6090
- 000000029a1b50cc:	000000029a1b15a0 000000029a1b1609 000000029a1b6094
- 000000029a1b50d8:	000000029a1b1610 000000029a1b1772 000000029a1b60a0
- 000000029a1b50e4:	000000029a1b1780 000000029a1b1add 000000029a1b60ac
- 000000029a1b50f0:	000000029a1b1ae0 000000029a1b1b50 000000029a1b60c4
- 000000029a1b50fc:	000000029a1b1b50 000000029a1b1bbf 000000029a1b60d4
- 000000029a1b5108:	000000029a1b1bc0 000000029a1b1c41 000000029a1b60e0
- 000000029a1b5114:	000000029a1b1c50 000000029a1b1d42 000000029a1b60ec
- 000000029a1b5120:	000000029a1b1d50 000000029a1b1d7c 000000029a1b60f4
- 000000029a1b512c:	000000029a1b1d80 000000029a1b1dd0 000000029a1b60f8
- 000000029a1b5138:	000000029a1b1dd0 000000029a1b1e6d 000000029a1b60fc
- 000000029a1b5144:	000000029a1b1e70 000000029a1b1ef0 000000029a1b6108
- 000000029a1b5150:	000000029a1b1ef0 000000029a1b1f27 000000029a1b610c
- 000000029a1b515c:	000000029a1b1f30 000000029a1b1fa3 000000029a1b6110
- 000000029a1b5168:	000000029a1b1fb0 000000029a1b1fe6 000000029a1b6114
- 000000029a1b5174:	000000029a1b1ff0 000000029a1b2079 000000029a1b6118
- 000000029a1b5180:	000000029a1b2080 000000029a1b2146 000000029a1b611c
- 000000029a1b518c:	000000029a1b2150 000000029a1b2153 000000029a1b6120
- 000000029a1b5198:	000000029a1b21a0 000000029a1b21a6 000000029a1b6124
- 000000029a1b51a4:	000000029a1b21b0 000000029a1b21b6 000000029a1b6128
- 000000029a1b51b0:	000000029a1b21c0 000000029a1b21de 000000029a1b612c
- 000000029a1b51bc:	000000029a1b21e0 000000029a1b21e3 000000029a1b6134
- 000000029a1b51c8:	000000029a1b21f0 000000029a1b225a 000000029a1b6138
- 000000029a1b51d4:	000000029a1b2260 000000029a1b22ca 000000029a1b6148
- 000000029a1b51e0:	000000029a1b22d0 000000029a1b22ee 000000029a1b6158
- 000000029a1b51ec:	000000029a1b22f0 000000029a1b2305 000000029a1b6160
- 000000029a1b51f8:	000000029a1b2310 000000029a1b233e 000000029a1b6164
- 000000029a1b5204:	000000029a1b2340 000000029a1b2375 000000029a1b616c
- 000000029a1b5210:	000000029a1b2380 000000029a1b23b6 000000029a1b6174
- 000000029a1b521c:	000000029a1b23c0 000000029a1b23f6 000000029a1b617c
- 000000029a1b5228:	000000029a1b2530 000000029a1b2562 000000029a1b6184
- 000000029a1b5234:	000000029a1b25c0 000000029a1b25c5 000000029a1b618c
+ 000000029a1b5054:	000000029a1b1380 000000029a1b1387 000000029a1b6038
+ 000000029a1b5060:	000000029a1b1387 000000029a1b139a 000000029a1b6040
+ 000000029a1b506c:	000000029a1b139a 000000029a1b13ce 000000029a1b604c
+ 000000029a1b5078:	000000029a1b13ce 000000029a1b13d5 000000029a1b6058
+ 000000029a1b5084:	000000029a1b13e0 000000029a1b141a 000000029a1b6060
+ 000000029a1b5090:	000000029a1b1420 000000029a1b148a 000000029a1b6068
+ 000000029a1b509c:	000000029a1b1490 000000029a1b14af 000000029a1b6074
+ 000000029a1b50a8:	000000029a1b14b0 000000029a1b14df 000000029a1b6078
+ 000000029a1b50b4:	000000029a1b14e0 000000029a1b1561 000000029a1b6080
+ 000000029a1b50c0:	000000029a1b1570 000000029a1b1573 000000029a1b608c
+ 000000029a1b50cc:	000000029a1b1580 000000029a1b15e9 000000029a1b6090
+ 000000029a1b50d8:	000000029a1b15f0 000000029a1b1752 000000029a1b609c
+ 000000029a1b50e4:	000000029a1b1760 000000029a1b1abd 000000029a1b60a8
+ 000000029a1b50f0:	000000029a1b1ac0 000000029a1b1b30 000000029a1b60c0
+ 000000029a1b50fc:	000000029a1b1b30 000000029a1b1b9f 000000029a1b60d0
+ 000000029a1b5108:	000000029a1b1ba0 000000029a1b1c21 000000029a1b60dc
+ 000000029a1b5114:	000000029a1b1c30 000000029a1b1d22 000000029a1b60e8
+ 000000029a1b5120:	000000029a1b1d30 000000029a1b1d5c 000000029a1b60f0
+ 000000029a1b512c:	000000029a1b1d60 000000029a1b1db0 000000029a1b60f4
+ 000000029a1b5138:	000000029a1b1db0 000000029a1b1e4d 000000029a1b60f8
+ 000000029a1b5144:	000000029a1b1e50 000000029a1b1ed0 000000029a1b6104
+ 000000029a1b5150:	000000029a1b1ed0 000000029a1b1f07 000000029a1b6108
+ 000000029a1b515c:	000000029a1b1f10 000000029a1b1f83 000000029a1b610c
+ 000000029a1b5168:	000000029a1b1f90 000000029a1b1fc6 000000029a1b6110
+ 000000029a1b5174:	000000029a1b1fd0 000000029a1b2059 000000029a1b6114
+ 000000029a1b5180:	000000029a1b2060 000000029a1b2126 000000029a1b6118
+ 000000029a1b518c:	000000029a1b2130 000000029a1b2133 000000029a1b611c
+ 000000029a1b5198:	000000029a1b2180 000000029a1b2186 000000029a1b6120
+ 000000029a1b51a4:	000000029a1b2190 000000029a1b2196 000000029a1b6124
+ 000000029a1b51b0:	000000029a1b21a0 000000029a1b21be 000000029a1b6128
+ 000000029a1b51bc:	000000029a1b21c0 000000029a1b21c3 000000029a1b6130
+ 000000029a1b51c8:	000000029a1b21d0 000000029a1b223a 000000029a1b6134
+ 000000029a1b51d4:	000000029a1b2240 000000029a1b22aa 000000029a1b6144
+ 000000029a1b51e0:	000000029a1b22b0 000000029a1b22ce 000000029a1b6154
+ 000000029a1b51ec:	000000029a1b22d0 000000029a1b22e5 000000029a1b615c
+ 000000029a1b51f8:	000000029a1b22f0 000000029a1b231e 000000029a1b6160
+ 000000029a1b5204:	000000029a1b2320 000000029a1b2355 000000029a1b6168
+ 000000029a1b5210:	000000029a1b2360 000000029a1b2396 000000029a1b6170
+ 000000029a1b521c:	000000029a1b23a0 000000029a1b23d6 000000029a1b6178
+ 000000029a1b5228:	000000029a1b2500 000000029a1b2532 000000029a1b6180
+ 000000029a1b5234:	000000029a1b2590 000000029a1b2595 000000029a1b6188
 
 Dump of .xdata
  000000029a1b6000 (rva: 00006000): 000000029a1b1000 - 000000029a1b100c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  000000029a1b6004 (rva: 00006004): 000000029a1b1010 - 000000029a1b11cf
 	Version: 1, Flags: none
@@ -262,219 +261,218 @@
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  000000029a1b6030 (rva: 00006030): 000000029a1b1360 - 000000029a1b136c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  000000029a1b6034 (rva: 00006034): 000000029a1b1370 - 000000029a1b1371
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6038 (rva: 00006038): 000000029a1b1380 - 000000029a1b13a5
+ 000000029a1b6038 (rva: 00006038): 000000029a1b1380 - 000000029a1b1387
 	Version: 1, Flags: none
-	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
-	  pc+0x08: alloc small area: rsp = rsp - 0x20
+	Nbr codes: 2, Prologue size: 0x04, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 000000029a1b6044 (rva: 00006044): 000000029a1b13a5 - 000000029a1b13b8
+ 000000029a1b6040 (rva: 00006040): 000000029a1b1387 - 000000029a1b139a
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 000000029a1b6050 (rva: 00006050): 000000029a1b13b8 - 000000029a1b13ec
+ 000000029a1b604c (rva: 0000604c): 000000029a1b139a - 000000029a1b13ce
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 000000029a1b605c (rva: 0000605c): 000000029a1b13ec - 000000029a1b13f3
+ 000000029a1b6058 (rva: 00006058): 000000029a1b13ce - 000000029a1b13d5
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x04, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 000000029a1b6064 (rva: 00006064): 000000029a1b1400 - 000000029a1b143a
+ 000000029a1b6060 (rva: 00006060): 000000029a1b13e0 - 000000029a1b141a
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000029a1b606c (rva: 0000606c): 000000029a1b1440 - 000000029a1b14aa
+ 000000029a1b6068 (rva: 00006068): 000000029a1b1420 - 000000029a1b148a
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 000000029a1b6078 (rva: 00006078): 000000029a1b14b0 - 000000029a1b14cf
+ 000000029a1b6074 (rva: 00006074): 000000029a1b1490 - 000000029a1b14af
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b607c (rva: 0000607c): 000000029a1b14d0 - 000000029a1b14ff
+ 000000029a1b6078 (rva: 00006078): 000000029a1b14b0 - 000000029a1b14df
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000029a1b6084 (rva: 00006084): 000000029a1b1500 - 000000029a1b1581
+ 000000029a1b6080 (rva: 00006080): 000000029a1b14e0 - 000000029a1b1561
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 000000029a1b6090 (rva: 00006090): 000000029a1b1590 - 000000029a1b1593
+ 000000029a1b608c (rva: 0000608c): 000000029a1b1570 - 000000029a1b1573
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6094 (rva: 00006094): 000000029a1b15a0 - 000000029a1b1609
+ 000000029a1b6090 (rva: 00006090): 000000029a1b1580 - 000000029a1b15e9
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 000000029a1b60a0 (rva: 000060a0): 000000029a1b1610 - 000000029a1b1772
+ 000000029a1b609c (rva: 0000609c): 000000029a1b15f0 - 000000029a1b1752
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x50
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 000000029a1b60ac (rva: 000060ac): 000000029a1b1780 - 000000029a1b1add
+ 000000029a1b60a8 (rva: 000060a8): 000000029a1b1760 - 000000029a1b1abd
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
- 000000029a1b60c4 (rva: 000060c4): 000000029a1b1ae0 - 000000029a1b1b50
+ 000000029a1b60c0 (rva: 000060c0): 000000029a1b1ac0 - 000000029a1b1b30
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 000000029a1b60d4 (rva: 000060d4): 000000029a1b1b50 - 000000029a1b1bbf
+ 000000029a1b60d0 (rva: 000060d0): 000000029a1b1b30 - 000000029a1b1b9f
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 000000029a1b60e0 (rva: 000060e0): 000000029a1b1bc0 - 000000029a1b1c41
+ 000000029a1b60dc (rva: 000060dc): 000000029a1b1ba0 - 000000029a1b1c21
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 000000029a1b60ec (rva: 000060ec): 000000029a1b1c50 - 000000029a1b1d42
+ 000000029a1b60e8 (rva: 000060e8): 000000029a1b1c30 - 000000029a1b1d22
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 000000029a1b60f4 (rva: 000060f4): 000000029a1b1d50 - 000000029a1b1d7c
+ 000000029a1b60f0 (rva: 000060f0): 000000029a1b1d30 - 000000029a1b1d5c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b60f8 (rva: 000060f8): 000000029a1b1d80 - 000000029a1b1dd0
+ 000000029a1b60f4 (rva: 000060f4): 000000029a1b1d60 - 000000029a1b1db0
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b60fc (rva: 000060fc): 000000029a1b1dd0 - 000000029a1b1e6d
+ 000000029a1b60f8 (rva: 000060f8): 000000029a1b1db0 - 000000029a1b1e4d
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 000000029a1b6108 (rva: 00006108): 000000029a1b1e70 - 000000029a1b1ef0
+ 000000029a1b6104 (rva: 00006104): 000000029a1b1e50 - 000000029a1b1ed0
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b610c (rva: 0000610c): 000000029a1b1ef0 - 000000029a1b1f27
+ 000000029a1b6108 (rva: 00006108): 000000029a1b1ed0 - 000000029a1b1f07
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6110 (rva: 00006110): 000000029a1b1f30 - 000000029a1b1fa3
+ 000000029a1b610c (rva: 0000610c): 000000029a1b1f10 - 000000029a1b1f83
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6114 (rva: 00006114): 000000029a1b1fb0 - 000000029a1b1fe6
+ 000000029a1b6110 (rva: 00006110): 000000029a1b1f90 - 000000029a1b1fc6
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6118 (rva: 00006118): 000000029a1b1ff0 - 000000029a1b2079
+ 000000029a1b6114 (rva: 00006114): 000000029a1b1fd0 - 000000029a1b2059
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b611c (rva: 0000611c): 000000029a1b2080 - 000000029a1b2146
+ 000000029a1b6118 (rva: 00006118): 000000029a1b2060 - 000000029a1b2126
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6120 (rva: 00006120): 000000029a1b2150 - 000000029a1b2153
+ 000000029a1b611c (rva: 0000611c): 000000029a1b2130 - 000000029a1b2133
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6124 (rva: 00006124): 000000029a1b21a0 - 000000029a1b21a6
+ 000000029a1b6120 (rva: 00006120): 000000029a1b2180 - 000000029a1b2186
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6128 (rva: 00006128): 000000029a1b21b0 - 000000029a1b21b6
+ 000000029a1b6124 (rva: 00006124): 000000029a1b2190 - 000000029a1b2196
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b612c (rva: 0000612c): 000000029a1b21c0 - 000000029a1b21de
+ 000000029a1b6128 (rva: 00006128): 000000029a1b21a0 - 000000029a1b21be
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x38
- 000000029a1b6134 (rva: 00006134): 000000029a1b21e0 - 000000029a1b21e3
+ 000000029a1b6130 (rva: 00006130): 000000029a1b21c0 - 000000029a1b21c3
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6138 (rva: 00006138): 000000029a1b21f0 - 000000029a1b225a
+ 000000029a1b6134 (rva: 00006134): 000000029a1b21d0 - 000000029a1b223a
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 000000029a1b6148 (rva: 00006148): 000000029a1b2260 - 000000029a1b22ca
+ 000000029a1b6144 (rva: 00006144): 000000029a1b2240 - 000000029a1b22aa
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 000000029a1b6158 (rva: 00006158): 000000029a1b22d0 - 000000029a1b22ee
+ 000000029a1b6154 (rva: 00006154): 000000029a1b22b0 - 000000029a1b22ce
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 000000029a1b6160 (rva: 00006160): 000000029a1b22f0 - 000000029a1b2305
+ 000000029a1b615c (rva: 0000615c): 000000029a1b22d0 - 000000029a1b22e5
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000029a1b6164 (rva: 00006164): 000000029a1b2310 - 000000029a1b233e
+ 000000029a1b6160 (rva: 00006160): 000000029a1b22f0 - 000000029a1b231e
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 000000029a1b616c (rva: 0000616c): 000000029a1b2340 - 000000029a1b2375
+ 000000029a1b6168 (rva: 00006168): 000000029a1b2320 - 000000029a1b2355
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x48
- 000000029a1b6174 (rva: 00006174): 000000029a1b2380 - 000000029a1b23b6
+ 000000029a1b6170 (rva: 00006170): 000000029a1b2360 - 000000029a1b2396
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000029a1b617c (rva: 0000617c): 000000029a1b23c0 - 000000029a1b23f6
+ 000000029a1b6178 (rva: 00006178): 000000029a1b23a0 - 000000029a1b23d6
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000029a1b6184 (rva: 00006184): 000000029a1b2530 - 000000029a1b2562
+ 000000029a1b6180 (rva: 00006180): 000000029a1b2500 - 000000029a1b2532
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x48
- 000000029a1b618c (rva: 0000618c): 000000029a1b25c0 - 000000029a1b25c5
+ 000000029a1b6188 (rva: 00006188): 000000029a1b2590 - 000000029a1b2595
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 
 
 PE File Base Relocations (interpreted .reloc section contents)
 
 Virtual Address: 00002000 Chunk size 12 (0xc) Number of fixups 2
-	reloc    0 offset  5d8 [25d8] DIR64
+	reloc    0 offset  5a8 [25a8] DIR64
 	reloc    1 offset    0 [2000] ABSOLUTE
 
 Virtual Address: 00003000 Chunk size 40 (0x28) Number of fixups 16
 	reloc    0 offset   10 [3010] DIR64
 	reloc    1 offset   40 [3040] DIR64
 	reloc    2 offset   50 [3050] DIR64
 	reloc    3 offset   58 [3058] DIR64
@@ -519,29 +517,29 @@
 	reloc    0 offset   18 [a018] DIR64
 	reloc    1 offset   30 [a030] DIR64
 	reloc    2 offset   38 [a038] DIR64
 	reloc    3 offset    0 [a000] ABSOLUTE
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
-  0 .text         000015f8  000000029a1b1000  000000029a1b1000  00000600  2**4
+  0 .text         000015c8  000000029a1b1000  000000029a1b1000  00000600  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE, DATA
   1 .data         000000e0  000000029a1b3000  000000029a1b3000  00001c00  2**4
                   CONTENTS, ALLOC, LOAD, DATA
   2 .rdata        000006d0  000000029a1b4000  000000029a1b4000  00001e00  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   3 .pdata        00000240  000000029a1b5000  000000029a1b5000  00002600  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  4 .xdata        00000190  000000029a1b6000  000000029a1b6000  00002a00  2**2
+  4 .xdata        0000018c  000000029a1b6000  000000029a1b6000  00002a00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   5 .bss          00000110  000000029a1b7000  000000029a1b7000  00000000  2**4
                   ALLOC
   6 .edata        00000087  000000029a1b8000  000000029a1b8000  00002c00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  7 .idata        00000870  000000029a1b9000  000000029a1b9000  00002e00  2**2
+  7 .idata        00000854  000000029a1b9000  000000029a1b9000  00002e00  2**2
                   CONTENTS, ALLOC, LOAD, DATA
   8 .CRT          00000058  000000029a1ba000  000000029a1ba000  00003800  2**2
                   CONTENTS, ALLOC, LOAD, DATA
   9 .tls          00000010  000000029a1bb000  000000029a1bb000  00003a00  2**2
                   CONTENTS, ALLOC, LOAD, DATA
  10 .reloc        00000078  000000029a1bc000  000000029a1bc000  00003c00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
@@ -641,46 +639,46 @@
 AUX scnlen 0x18 nreloc 6 nlnno 0
 [ 75](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000310 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [ 77](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000060 inputExtention
 File 
 [ 79](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000000380 init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[ 81](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000003a5 isInputReady
-[ 82](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000003b8 getCharacter
-[ 83](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000003ec stop
+[ 81](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000387 isInputReady
+[ 82](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000039a getCharacter
+[ 83](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000003ce stop
 [ 84](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000380 .text
-AUX scnlen 0x73 nreloc 5 nlnno 0
+AUX scnlen 0x55 nreloc 3 nlnno 0
 [ 86](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [ 88](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [ 90](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000038 .xdata
-AUX scnlen 0x2c nreloc 0 nlnno 0
+AUX scnlen 0x28 nreloc 0 nlnno 0
 [ 92](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000054 .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
 [ 94](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000340 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [ 96](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000084 gccmain.c
 File 
-[ 98](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000000400 __do_global_dtors
+[ 98](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000003e0 __do_global_dtors
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [100](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000010 p.0
-[101](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000440 __do_global_ctors
+[101](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000420 __do_global_ctors
 [102](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001f0 .rdata$.refptr.__CTOR_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[104](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000004b0 __main
+[104](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000490 __main
 [105](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000020 initialized
-[106](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000400 .text
+[106](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003e0 .text
 AUX scnlen 0xcf nreloc 7 nlnno 0
 [108](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [110](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[112](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000064 .xdata
+[112](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000060 .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
 [114](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000084 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [116](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000019b4 .debug_info
 AUX scnlen 0x661 nreloc 17 nlnno 0
 [118](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004bf .debug_abbrev
 AUX scnlen 0x13f nreloc 0 nlnno 0
@@ -694,15 +692,15 @@
 AUX scnlen 0xe8 nreloc 0 nlnno 0
 [128](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000370 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [130](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000108 .debug_frame
 AUX scnlen 0x88 nreloc 6 nlnno 0
 [132](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000009a natstart.c
 File 
-[134](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d0 .text
+[134](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004b0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [136](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [138](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .bss
 AUX scnlen 0xc nreloc 0 nlnno 0
 [140](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002015 .debug_info
 AUX scnlen 0x602 nreloc 10 nlnno 0
@@ -716,29 +714,29 @@
 AUX scnlen 0x18 nreloc 0 nlnno 0
 [150](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000272 .debug_line_str
 AUX scnlen 0x10e nreloc 0 nlnno 0
 [152](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [154](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000d2 tlssup.c
 File 
-[156](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000004d0 __dyn_tls_dtor
+[156](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000004b0 __dyn_tls_dtor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[158](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000500 __dyn_tls_init
+[158](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000004e0 __dyn_tls_init
 [159](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001e0 .rdata$.refptr._CRT_MT
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [161](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000048 __xd_a
 [162](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 __xd_z
-[163](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000590 __tlregdtor
-[164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d0 .text
+[163](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000570 __tlregdtor
+[164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004b0 .text
 AUX scnlen 0xc3 nreloc 5 nlnno 0
 [166](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [168](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[170](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000007c .xdata
+[170](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000078 .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
 [172](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000a8 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [174](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000038 .CRT$XLD
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [176](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .CRT$XLC
 AUX scnlen 0x8 nreloc 1 nlnno 0
@@ -772,15 +770,15 @@
 AUX scnlen 0xee nreloc 0 nlnno 0
 [206](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003d0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [208](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000190 .debug_frame
 AUX scnlen 0xa8 nreloc 6 nlnno 0
 [210](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000ee cinitexe.c
 File 
-[212](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005a0 .text
+[212](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000580 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [214](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [216](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [218](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .CRT$XCZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
@@ -800,15 +798,15 @@
 AUX scnlen 0x3a nreloc 4 nlnno 0
 [234](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000046e .debug_line_str
 AUX scnlen 0x9f nreloc 0 nlnno 0
 [236](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000400 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [238](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000102 mingw_helpers.
 File 
-[240](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005a0 .text
+[240](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000580 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [242](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [244](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [246](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002f59 .debug_info
 AUX scnlen 0x92 nreloc 5 nlnno 0
@@ -820,36 +818,36 @@
 AUX scnlen 0x3a nreloc 4 nlnno 0
 [254](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000050d .debug_line_str
 AUX scnlen 0xae nreloc 0 nlnno 0
 [256](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000430 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [258](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000131 pseudo-reloc.c
 File 
-[260](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000005a0 __report_error
+[260](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000000580 __report_error
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[262](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000000610 mark_section_writable
+[262](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x00000000000005f0 mark_section_writable
 [263](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000064 maxSections
 [264](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000068 the_secs
-[265](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000780 _pei386_runtime_relocator
+[265](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000760 _pei386_runtime_relocator
 [266](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000060 was_init.0
 [267](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000210 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [269](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000220 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [271](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000200 .rdata$.refptr.__ImageBase
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[273](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005a0 .text
+[273](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000580 .text
 AUX scnlen 0x53d nreloc 38 nlnno 0
 [275](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [277](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000060 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
 [279](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000060 .rdata
 AUX scnlen 0x15b nreloc 0 nlnno 0
-[281](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000094 .xdata
+[281](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000090 .xdata
 AUX scnlen 0x30 nreloc 0 nlnno 0
 [283](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000cc .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [285](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002feb .debug_info
 AUX scnlen 0x174b nreloc 165 nlnno 0
 [287](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000092a .debug_abbrev
 AUX scnlen 0x3d8 nreloc 0 nlnno 0
@@ -867,29 +865,29 @@
 AUX scnlen 0x14f nreloc 0 nlnno 0
 [301](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000460 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [303](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000238 .debug_frame
 AUX scnlen 0xe0 nreloc 6 nlnno 0
 [305](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000157 tlsthrd.c
 File 
-[307](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000000ae0 __mingwthr_run_key_dtors.part.0
+[307](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000000ac0 __mingwthr_run_key_dtors.part.0
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [309](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000a0 __mingwthr_cs
 [310](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 key_dtor_list
-[311](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000b50 ___w64_mingwthr_add_key_dtor
+[311](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000b30 ___w64_mingwthr_add_key_dtor
 [312](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000088 __mingwthr_cs_init
-[313](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000bc0 ___w64_mingwthr_remove_key_dtor
-[314](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000c50 __mingw_TLScallback
-[315](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000ae0 .text
+[313](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000ba0 ___w64_mingwthr_remove_key_dtor
+[314](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000c30 __mingw_TLScallback
+[315](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000ac0 .text
 AUX scnlen 0x262 nreloc 34 nlnno 0
 [317](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [319](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .bss
 AUX scnlen 0x48 nreloc 0 nlnno 0
-[321](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000c4 .xdata
+[321](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000c0 .xdata
 AUX scnlen 0x30 nreloc 0 nlnno 0
 [323](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
 [325](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004736 .debug_info
 AUX scnlen 0xad3 nreloc 65 nlnno 0
 [327](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d02 .debug_abbrev
 AUX scnlen 0x261 nreloc 0 nlnno 0
@@ -905,15 +903,15 @@
 AUX scnlen 0x125 nreloc 0 nlnno 0
 [339](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000490 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [341](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000318 .debug_frame
 AUX scnlen 0x128 nreloc 8 nlnno 0
 [343](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000016b tlsmcrt.c
 File 
-[345](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d50 .text
+[345](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d30 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [347](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [349](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [351](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005209 .debug_info
 AUX scnlen 0x89 nreloc 5 nlnno 0
@@ -925,15 +923,15 @@
 AUX scnlen 0x3a nreloc 4 nlnno 0
 [359](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000082f .debug_line_str
 AUX scnlen 0x9c nreloc 0 nlnno 0
 [361](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [363](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000017f pseudo-reloc-list.c
 File 
-[365](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d50 .text
+[365](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d30 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [367](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [369](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .bss
 AUX scnlen 0x2 nreloc 0 nlnno 0
 [371](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005292 .debug_info
 AUX scnlen 0xd0 nreloc 6 nlnno 0
@@ -945,31 +943,31 @@
 AUX scnlen 0x3a nreloc 4 nlnno 0
 [379](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000008cb .debug_line_str
 AUX scnlen 0xba nreloc 0 nlnno 0
 [381](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004f0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [383](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001a9 pesect.c
 File 
-[385](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000000d50 _ValidateImageBase
+[385](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000000d30 _ValidateImageBase
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[387](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000d80 _FindPESection
-[388](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000dd0 _FindPESectionByName
-[389](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000e70 __mingw_GetSectionForAddress
-[390](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000ef0 __mingw_GetSectionCount
-[391](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000f30 _FindPESectionExec
-[392](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000fb0 _GetPEImageBase
-[393](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000ff0 _IsNonwritableInCurrentImage
-[394](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001080 __mingw_enum_import_library_names
-[395](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d50 .text
+[387](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000d60 _FindPESection
+[388](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000db0 _FindPESectionByName
+[389](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000e50 __mingw_GetSectionForAddress
+[390](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000ed0 __mingw_GetSectionCount
+[391](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000f10 _FindPESectionExec
+[392](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000f90 _GetPEImageBase
+[393](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000fd0 _IsNonwritableInCurrentImage
+[394](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001060 __mingw_enum_import_library_names
+[395](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d30 .text
 AUX scnlen 0x3f6 nreloc 9 nlnno 0
 [397](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [399](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[401](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f4 .xdata
+[401](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .xdata
 AUX scnlen 0x2c nreloc 0 nlnno 0
 [403](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000120 .pdata
 AUX scnlen 0x6c nreloc 27 nlnno 0
 [405](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005362 .debug_info
 AUX scnlen 0x14d2 nreloc 203 nlnno 0
 [407](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000fc1 .debug_abbrev
 AUX scnlen 0x28a nreloc 0 nlnno 0
@@ -987,24 +985,24 @@
 AUX scnlen 0xe5 nreloc 0 nlnno 0
 [421](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000520 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [423](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000440 .debug_frame
 AUX scnlen 0x128 nreloc 18 nlnno 0
 [425](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001d4 CRT_fp10.c
 File 
-[427](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001150 _fpreset
+[427](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001130 _fpreset
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[429](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001150 fpreset
-[430](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001150 .text
+[429](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001130 fpreset
+[430](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001130 .text
 AUX scnlen 0x3 nreloc 0 nlnno 0
 [432](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [434](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[436](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000120 .xdata
+[436](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000011c .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [438](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000018c .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [440](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006834 .debug_info
 AUX scnlen 0x97 nreloc 6 nlnno 0
 [442](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000124b .debug_abbrev
 AUX scnlen 0x2d nreloc 0 nlnno 0
@@ -1014,39 +1012,39 @@
 AUX scnlen 0x58 nreloc 5 nlnno 0
 [448](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000a6a .debug_line_str
 AUX scnlen 0x9f nreloc 0 nlnno 0
 [450](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000550 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [452](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000568 .debug_frame
 AUX scnlen 0x30 nreloc 2 nlnno 0
-[454](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001160 .text
+[454](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001140 .text
 AUX scnlen 0x32 nreloc 0 nlnno 0
 [456](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [458](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[460](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011a0 .text
+[460](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001180 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [462](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [464](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000f0 .bss
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [466](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000580 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [468](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001f0 dllentry.c
 File 
-[470](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000011a0 DllEntryPoint
+[470](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001180 DllEntryPoint
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[472](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011a0 .text
+[472](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001180 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
 [474](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [476](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[478](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000124 .xdata
+[478](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000120 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [480](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000198 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [482](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000068cb .debug_info
 AUX scnlen 0x1fa nreloc 6 nlnno 0
 [484](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001278 .debug_abbrev
 AUX scnlen 0x72 nreloc 0 nlnno 0
@@ -1058,23 +1056,23 @@
 AUX scnlen 0xce nreloc 0 nlnno 0
 [492](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005b0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [494](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000598 .debug_frame
 AUX scnlen 0x30 nreloc 2 nlnno 0
 [496](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000020c dllmain.c
 File 
-[498](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000011b0 DllMain
+[498](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001190 DllMain
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[500](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011b0 .text
+[500](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001190 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
 [502](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [504](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[506](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000128 .xdata
+[506](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000124 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [508](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001a4 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [510](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ac5 .debug_info
 AUX scnlen 0x1f4 nreloc 6 nlnno 0
 [512](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000012ea .debug_abbrev
 AUX scnlen 0x72 nreloc 0 nlnno 0
@@ -1086,23 +1084,23 @@
 AUX scnlen 0xd5 nreloc 0 nlnno 0
 [520](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005e0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [522](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005c8 .debug_frame
 AUX scnlen 0x30 nreloc 2 nlnno 0
 [524](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000022a ucrt_vfprintf.
 File 
-[526](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000011c0 vfprintf
+[526](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000011a0 vfprintf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[528](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011c0 .text
+[528](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011a0 .text
 AUX scnlen 0x1e nreloc 1 nlnno 0
 [530](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [532](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[534](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000012c .xdata
+[534](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000128 .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [536](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001b0 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [538](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006cb9 .debug_info
 AUX scnlen 0x39d nreloc 14 nlnno 0
 [540](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000135c .debug_abbrev
 AUX scnlen 0x138 nreloc 0 nlnno 0
@@ -1116,40 +1114,40 @@
 AUX scnlen 0xe8 nreloc 0 nlnno 0
 [550](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000610 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [552](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005f8 .debug_frame
 AUX scnlen 0x38 nreloc 2 nlnno 0
 [554](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000279 ucrtbase_compa
 File 
-[556](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000011e0 _get_output_format
+[556](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000011c0 _get_output_format
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[558](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000011f0 __getmainargs
-[559](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001260 __wgetmainargs
-[560](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000012d0 _onexit
-[561](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000012f0 at_quick_exit
+[558](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000011d0 __getmainargs
+[559](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001240 __wgetmainargs
+[560](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000012b0 _onexit
+[561](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000012d0 at_quick_exit
 [562](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000260 .rdata$.refptr.__mingw_module_is_dll
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[564](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001310 _amsg_exit
-[565](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001340 __ms_fwprintf
-[566](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001380 tzset
+[564](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000012f0 _amsg_exit
+[565](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001320 __ms_fwprintf
+[566](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001360 tzset
 [567](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000240 .rdata$.refptr.__imp__tzset
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[569](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013c0 _tzset
+[569](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013a0 _tzset
 [570](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000098 initial_daylight
 [571](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000009c initial_timezone
 [572](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000a0 initial_tznames
 [573](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b4 initial_tzname0
 [574](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b0 initial_tzname1
-[575](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011e0 .text
+[575](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000011c0 .text
 AUX scnlen 0x216 nreloc 34 nlnno 0
 [577](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x78 nreloc 13 nlnno 0
 [579](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[581](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000134 .xdata
+[581](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000130 .xdata
 AUX scnlen 0x50 nreloc 0 nlnno 0
 [583](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001bc .pdata
 AUX scnlen 0x6c nreloc 27 nlnno 0
 [585](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c0 .rdata
 AUX scnlen 0x12 nreloc 0 nlnno 0
 [587](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000007056 .debug_info
 AUX scnlen 0x1185 nreloc 89 nlnno 0
@@ -1165,799 +1163,790 @@
 AUX scnlen 0x17 nreloc 0 nlnno 0
 [599](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000d94 .debug_line_str
 AUX scnlen 0x160 nreloc 0 nlnno 0
 [601](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000640 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
 [603](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000630 .debug_frame
 AUX scnlen 0x190 nreloc 18 nlnno 0
-[605](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001400 .text
+[605](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000013e0 .text
 [606](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [607](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[608](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000840 .idata$7
-[609](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c0 .idata$5
-[610](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000228 .idata$4
-[611](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000692 .idata$6
-[612](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001408 .text
+[608](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000824 .idata$7
+[609](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b0 .idata$5
+[610](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000220 .idata$4
+[611](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000678 .idata$6
+[612](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000013e8 .text
 [613](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [614](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[615](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000844 .idata$7
-[616](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c8 .idata$5
-[617](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000230 .idata$4
-[618](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006a0 .idata$6
-[619](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001410 .text
+[615](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000828 .idata$7
+[616](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b8 .idata$5
+[617](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000228 .idata$4
+[618](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000686 .idata$6
+[619](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000013f0 .text
 [620](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [621](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[622](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000848 .idata$7
-[623](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003d0 .idata$5
-[624](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000238 .idata$4
-[625](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ae .idata$6
-[626](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001418 .text
+[622](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000082c .idata$7
+[623](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c0 .idata$5
+[624](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000230 .idata$4
+[625](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000694 .idata$6
+[626](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000013f8 .text
 [627](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [628](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[629](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000084c .idata$7
-[630](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003d8 .idata$5
-[631](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000240 .idata$4
-[632](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ba .idata$6
+[629](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000830 .idata$7
+[630](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c8 .idata$5
+[631](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000238 .idata$4
+[632](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006a0 .idata$6
 [633](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000287 fake
 File 
-[635](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000228 hname
-[636](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c0 fthunk
-[637](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001420 .text
+[635](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000220 hname
+[636](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b0 fthunk
+[637](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001400 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [639](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [641](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [643](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000008c .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[645](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000228 .idata$4
-[646](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003c0 .idata$5
+[645](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000220 .idata$4
+[646](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b0 .idata$5
 [647](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002a3 fake
 File 
-[649](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001420 .text
+[649](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001400 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [651](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [653](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[655](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000248 .idata$4
+[655](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000240 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[657](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003e0 .idata$5
+[657](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003d0 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[659](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000850 .idata$7
+[659](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000834 .idata$7
 AUX scnlen 0x1f nreloc 0 nlnno 0
-[661](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001420 .text
+[661](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001400 .text
 [662](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [663](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[664](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000814 .idata$7
-[665](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a8 .idata$5
-[666](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000210 .idata$4
-[667](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000067e .idata$6
-[668](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001428 .text
+[664](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007f8 .idata$7
+[665](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000398 .idata$5
+[666](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000208 .idata$4
+[667](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000664 .idata$6
+[668](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001408 .text
 [669](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [670](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[671](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000818 .idata$7
-[672](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b0 .idata$5
-[673](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000218 .idata$4
-[674](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000688 .idata$6
+[671](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007fc .idata$7
+[672](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a0 .idata$5
+[673](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000210 .idata$4
+[674](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000066e .idata$6
 [675](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002b1 fake
 File 
-[677](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000210 hname
-[678](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a8 fthunk
-[679](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001430 .text
+[677](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000208 hname
+[678](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000398 fthunk
+[679](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001410 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [681](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [683](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [685](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000078 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[687](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000210 .idata$4
-[688](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a8 .idata$5
-[689](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002f0 fake
+[687](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000208 .idata$4
+[688](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000398 .idata$5
+[689](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002e9 fake
 File 
-[691](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001430 .text
+[691](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001410 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [693](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [695](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[697](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000220 .idata$4
+[697](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000218 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[699](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003b8 .idata$5
+[699](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a8 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[701](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000081c .idata$7
+[701](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000800 .idata$7
 AUX scnlen 0x21 nreloc 0 nlnno 0
-[703](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001430 .text
+[703](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001410 .text
 [704](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [705](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[706](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007d8 .idata$7
-[707](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000368 .idata$5
+[706](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007c0 .idata$7
+[707](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000360 .idata$5
 [708](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 .idata$4
-[709](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000060e .idata$6
-[710](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001438 .text
+[709](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005fe .idata$6
+[710](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001418 .text
 [711](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [712](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[713](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007dc .idata$7
-[714](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000370 .idata$5
+[713](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007c4 .idata$7
+[714](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000368 .idata$5
 [715](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d8 .idata$4
-[716](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000620 .idata$6
-[717](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001440 .text
+[716](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000610 .idata$6
+[717](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001420 .text
 [718](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [719](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[720](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007e0 .idata$7
-[721](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000378 .idata$5
+[720](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007c8 .idata$7
+[721](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000370 .idata$5
 [722](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e0 .idata$4
-[723](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000063a .idata$6
-[724](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001448 .text
+[723](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000062a .idata$6
+[724](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001428 .text
 [725](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [726](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[727](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007e4 .idata$7
-[728](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000380 .idata$5
+[727](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007cc .idata$7
+[728](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000378 .idata$5
 [729](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e8 .idata$4
-[730](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000656 .idata$6
-[731](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001450 .text
+[730](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000646 .idata$6
+[731](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001430 .text
 [732](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [733](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[734](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007e8 .idata$7
-[735](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000388 .idata$5
+[734](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007d0 .idata$7
+[735](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000380 .idata$5
 [736](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f0 .idata$4
-[737](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000660 .idata$6
-[738](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001458 .text
+[737](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000650 .idata$6
+[738](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001438 .text
 [739](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [740](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[741](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007ec .idata$7
-[742](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000390 .idata$5
+[741](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007d4 .idata$7
+[742](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000388 .idata$5
 [743](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f8 .idata$4
-[744](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000066a .idata$6
-[745](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001460 .text
-[746](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
-[747](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[748](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007f0 .idata$7
-[749](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000398 .idata$5
-[750](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000200 .idata$4
-[751](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000674 .idata$6
-[752](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002fe fake
+[744](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000065a .idata$6
+[745](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002f7 fake
 File 
-[754](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 hname
-[755](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000368 fthunk
-[756](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001470 .text
+[747](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 hname
+[748](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000360 fthunk
+[749](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001440 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[758](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[751](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[760](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[753](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[762](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000064 .idata$2
+[755](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000064 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[764](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 .idata$4
-[765](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000368 .idata$5
-[766](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000375 fake
+[757](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 .idata$4
+[758](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000360 .idata$5
+[759](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000036e fake
 File 
-[768](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001470 .text
+[761](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001440 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[770](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[763](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[772](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[765](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[774](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000208 .idata$4
+[767](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000200 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[776](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a0 .idata$5
+[769](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000390 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[778](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007f4 .idata$7
+[771](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007d8 .idata$7
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[780](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001470 .text
+[773](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001440 .text
+[774](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
+[775](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
+[776](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000760 .idata$7
+[777](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e0 .idata$5
+[778](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 .idata$4
+[779](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004d0 .idata$6
+[780](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001448 .text
 [781](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [782](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[783](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000778 .idata$7
+[783](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000764 .idata$7
 [784](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e8 .idata$5
-[785](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 .idata$4
-[786](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004e0 .idata$6
-[787](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001478 .text
+[785](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000158 .idata$4
+[786](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004de .idata$6
+[787](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001450 .text
 [788](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [789](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[790](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000077c .idata$7
+[790](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000768 .idata$7
 [791](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002f0 .idata$5
-[792](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000158 .idata$4
-[793](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ee .idata$6
-[794](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001480 .text
+[792](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000160 .idata$4
+[793](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ec .idata$6
+[794](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001458 .text
 [795](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [796](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[797](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000780 .idata$7
+[797](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000076c .idata$7
 [798](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002f8 .idata$5
-[799](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000160 .idata$4
-[800](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004fc .idata$6
-[801](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001488 .text
+[799](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000168 .idata$4
+[800](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004fa .idata$6
+[801](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001460 .text
 [802](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [803](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[804](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000784 .idata$7
+[804](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000770 .idata$7
 [805](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000300 .idata$5
-[806](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000168 .idata$4
-[807](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000050a .idata$6
-[808](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001490 .text
+[806](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000170 .idata$4
+[807](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000514 .idata$6
+[808](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001468 .text
 [809](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [810](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[811](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000788 .idata$7
+[811](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000774 .idata$7
 [812](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000308 .idata$5
-[813](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000170 .idata$4
-[814](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000524 .idata$6
-[815](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001498 .text
+[813](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000178 .idata$4
+[814](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000052c .idata$6
+[815](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001470 .text
 [816](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [817](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[818](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000078c .idata$7
+[818](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000778 .idata$7
 [819](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000310 .idata$5
-[820](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000178 .idata$4
-[821](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000053c .idata$6
-[822](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014a0 .text
+[820](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000180 .idata$4
+[821](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000542 .idata$6
+[822](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001478 .text
 [823](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [824](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[825](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000790 .idata$7
+[825](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000077c .idata$7
 [826](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000318 .idata$5
-[827](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000180 .idata$4
-[828](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000552 .idata$6
-[829](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014a8 .text
+[827](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000188 .idata$4
+[828](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000550 .idata$6
+[829](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001480 .text
 [830](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [831](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[832](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000794 .idata$7
+[832](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000780 .idata$7
 [833](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000320 .idata$5
-[834](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000188 .idata$4
-[835](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000560 .idata$6
-[836](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014b0 .text
+[834](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000190 .idata$4
+[835](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000568 .idata$6
+[836](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001488 .text
 [837](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [838](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[839](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000798 .idata$7
+[839](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000784 .idata$7
 [840](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000328 .idata$5
-[841](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000190 .idata$4
-[842](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000578 .idata$6
-[843](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014b8 .text
+[841](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000198 .idata$4
+[842](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000570 .idata$6
+[843](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001490 .text
 [844](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [845](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[846](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000079c .idata$7
+[846](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000788 .idata$7
 [847](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000330 .idata$5
-[848](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000198 .idata$4
-[849](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000580 .idata$6
-[850](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014c0 .text
+[848](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a0 .idata$4
+[849](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000592 .idata$6
+[850](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001498 .text
 [851](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [852](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[853](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007a0 .idata$7
+[853](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000078c .idata$7
 [854](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000338 .idata$5
-[855](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a0 .idata$4
-[856](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005a2 .idata$6
-[857](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014c8 .text
+[855](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a8 .idata$4
+[856](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ae .idata$6
+[857](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014a0 .text
 [858](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [859](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[860](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007a4 .idata$7
+[860](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000790 .idata$7
 [861](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000340 .idata$5
-[862](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a8 .idata$4
-[863](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005be .idata$6
-[864](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014d0 .text
+[862](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b0 .idata$4
+[863](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ce .idata$6
+[864](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014a8 .text
 [865](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [866](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[867](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007a8 .idata$7
+[867](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000794 .idata$7
 [868](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000348 .idata$5
-[869](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b0 .idata$4
-[870](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005de .idata$6
-[871](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014d8 .text
+[869](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b8 .idata$4
+[870](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005da .idata$6
+[871](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014b0 .text
 [872](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [873](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[874](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007ac .idata$7
+[874](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000798 .idata$7
 [875](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000350 .idata$5
-[876](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b8 .idata$4
-[877](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ea .idata$6
-[878](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014e0 .text
-[879](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
-[880](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[881](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007b0 .idata$7
-[882](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000358 .idata$5
-[883](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001c0 .idata$4
-[884](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000606 .idata$6
-[885](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000383 fake
+[876](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001c0 .idata$4
+[877](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005f6 .idata$6
+[878](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000037c fake
 File 
-[887](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 hname
-[888](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e8 fthunk
-[889](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014f0 .text
+[880](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 hname
+[881](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e0 fthunk
+[882](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014c0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[891](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[884](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[893](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[886](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[895](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .idata$2
+[888](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[897](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 .idata$4
-[898](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e8 .idata$5
-[899](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003a6 fake
+[890](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 .idata$4
+[891](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e0 .idata$5
+[892](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000039f fake
 File 
-[901](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014f0 .text
+[894](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014c0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[903](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[896](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[905](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[898](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[907](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c8 .idata$4
+[900](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c8 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[909](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000360 .idata$5
+[902](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000358 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[911](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007b4 .idata$7
+[904](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000079c .idata$7
 AUX scnlen 0x22 nreloc 0 nlnno 0
-[913](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014f0 .text
+[906](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014c0 .text
+[907](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
+[908](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
+[909](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000734 .idata$7
+[910](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c0 .idata$5
+[911](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 .idata$4
+[912](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ae .idata$6
+[913](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014c8 .text
 [914](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [915](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[916](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000074c .idata$7
+[916](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000738 .idata$7
 [917](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c8 .idata$5
-[918](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 .idata$4
+[918](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000138 .idata$4
 [919](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004be .idata$6
-[920](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014f8 .text
+[920](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014d0 .text
 [921](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [922](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[923](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000750 .idata$7
+[923](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000073c .idata$7
 [924](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002d0 .idata$5
-[925](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000138 .idata$4
-[926](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ce .idata$6
-[927](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001500 .text
-[928](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
-[929](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[930](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000754 .idata$7
-[931](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002d8 .idata$5
-[932](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000140 .idata$4
-[933](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004d8 .idata$6
-[934](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003b4 fake
+[925](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000140 .idata$4
+[926](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004c8 .idata$6
+[927](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003ad fake
 File 
-[936](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 hname
-[937](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c8 fthunk
-[938](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001510 .text
+[929](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 hname
+[930](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c0 fthunk
+[931](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014e0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[940](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[933](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[942](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[935](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[944](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000003c .idata$2
+[937](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000003c .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[946](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 .idata$4
-[947](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c8 .idata$5
-[948](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003d0 fake
+[939](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 .idata$4
+[940](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c0 .idata$5
+[941](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003c9 fake
 File 
-[950](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001510 .text
+[943](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014e0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[952](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[945](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[954](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[947](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[956](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000148 .idata$4
+[949](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000148 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[958](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002e0 .idata$5
+[951](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002d8 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[960](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000758 .idata$7
+[953](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000740 .idata$7
 AUX scnlen 0x1f nreloc 0 nlnno 0
-[962](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001510 .text
+[955](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014e0 .text
+[956](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
+[957](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
+[958](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000704 .idata$7
+[959](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a8 .idata$5
+[960](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 .idata$4
+[961](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000048e .idata$6
+[962](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014e8 .text
 [963](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
 [964](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[965](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000071c .idata$7
+[965](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000708 .idata$7
 [966](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b0 .idata$5
-[967](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 .idata$4
+[967](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000120 .idata$4
 [968](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000049e .idata$6
-[969](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001518 .text
-[970](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
-[971](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[972](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000720 .idata$7
-[973](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b8 .idata$5
-[974](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000120 .idata$4
-[975](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ae .idata$6
-[976](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003de fake
+[969](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003d7 fake
 File 
-[978](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 hname
-[979](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b0 fthunk
-[980](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001520 .text
+[971](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 hname
+[972](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a8 fthunk
+[973](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014f0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[982](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[975](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[984](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[977](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[986](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000028 .idata$2
+[979](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000028 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[988](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 .idata$4
-[989](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b0 .idata$5
-[990](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003f3 fake
+[981](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 .idata$4
+[982](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a8 .idata$5
+[983](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003ec fake
 File 
-[992](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001520 .text
+[985](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000014f0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[994](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[987](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[996](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[989](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[998](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000128 .idata$4
+[991](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000128 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1000](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002c0 .idata$5
+[993](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002b8 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1002](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000724 .idata$7
+[995](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000070c .idata$7
 AUX scnlen 0x26 nreloc 0 nlnno 0
-[1004](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001520 .text
-[1005](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
-[1006](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1007](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f8 .idata$7
-[1008](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a0 .idata$5
-[1009](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 .idata$4
-[1010](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000494 .idata$6
-[1011](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000401 fake
+[997](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000014f0 .text
+[998](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .data
+[999](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
+[1000](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e0 .idata$7
+[1001](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000298 .idata$5
+[1002](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 .idata$4
+[1003](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000484 .idata$6
+[1004](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003fa fake
 File 
-[1013](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 hname
-[1014](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a0 fthunk
-[1015](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001530 .text
+[1006](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 hname
+[1007](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000298 fthunk
+[1008](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001500 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1017](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[1010](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1019](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1012](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1021](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .idata$2
+[1014](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[1023](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 .idata$4
-[1024](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a0 .idata$5
-[1025](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000040f fake
+[1016](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000108 .idata$4
+[1017](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000298 .idata$5
+[1018](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000408 fake
 File 
-[1027](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001530 .text
+[1020](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001500 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1029](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[1022](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1031](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1024](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1033](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .idata$4
+[1026](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1035](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002a8 .idata$5
+[1028](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002a0 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1037](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006fc .idata$7
+[1030](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006e4 .idata$7
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[1039](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000046c ucrt_fprintf.c
+[1032](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000465 ucrt_fprintf.c
 File 
-[1041](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001530 fprintf
+[1034](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001500 fprintf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1043](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001530 .text
+[1036](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001500 .text
 AUX scnlen 0x32 nreloc 1 nlnno 0
-[1045](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
+[1038](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000d0 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[1047](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1040](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1049](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000184 .xdata
+[1042](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000180 .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1051](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000228 .pdata
+[1044](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000228 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[1053](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000081db .debug_info
+[1046](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000081db .debug_info
 AUX scnlen 0x3a2 nreloc 14 nlnno 0
-[1055](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000017b7 .debug_abbrev
+[1048](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000017b7 .debug_abbrev
 AUX scnlen 0x162 nreloc 0 nlnno 0
-[1057](sec 19)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000129a .debug_loclists
+[1050](sec 19)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000129a .debug_loclists
 AUX scnlen 0x46 nreloc 0 nlnno 0
-[1059](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002b0 .debug_aranges
+[1052](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002b0 .debug_aranges
 AUX scnlen 0x30 nreloc 2 nlnno 0
-[1061](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001856 .debug_line
+[1054](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001856 .debug_line
 AUX scnlen 0x8a nreloc 9 nlnno 0
-[1063](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000ef4 .debug_line_str
+[1056](sec 18)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000ef4 .debug_line_str
 AUX scnlen 0xe5 nreloc 0 nlnno 0
-[1065](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000670 .rdata$zzz
+[1058](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000670 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
-[1067](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007c0 .debug_frame
+[1060](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007c0 .debug_frame
 AUX scnlen 0x38 nreloc 2 nlnno 0
-[1069](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001570 .text
+[1062](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001540 .text
+[1063](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
+[1064](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
+[1065](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006cc .idata$7
+[1066](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000288 .idata$5
+[1067](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f8 .idata$4
+[1068](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000474 .idata$6
+[1069](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001548 .text
 [1070](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1071](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1072](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e4 .idata$7
-[1073](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000290 .idata$5
-[1074](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f8 .idata$4
-[1075](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000484 .idata$6
-[1076](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001578 .text
+[1072](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c8 .idata$7
+[1073](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 .idata$5
+[1074](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f0 .idata$4
+[1075](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000462 .idata$6
+[1076](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001550 .text
 [1077](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1078](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1079](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e0 .idata$7
-[1080](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000288 .idata$5
-[1081](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f0 .idata$4
-[1082](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000472 .idata$6
-[1083](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001580 .text
+[1079](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c4 .idata$7
+[1080](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000278 .idata$5
+[1081](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e8 .idata$4
+[1082](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000454 .idata$6
+[1083](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001558 .text
 [1084](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1085](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1086](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006dc .idata$7
-[1087](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 .idata$5
-[1088](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e8 .idata$4
-[1089](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000464 .idata$6
-[1090](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001588 .text
+[1086](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c0 .idata$7
+[1087](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000270 .idata$5
+[1088](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .idata$4
+[1089](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000044c .idata$6
+[1090](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001560 .text
 [1091](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1092](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1093](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d8 .idata$7
-[1094](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000278 .idata$5
-[1095](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .idata$4
-[1096](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000045c .idata$6
-[1097](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001590 .text
+[1093](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006bc .idata$7
+[1094](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000268 .idata$5
+[1095](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d8 .idata$4
+[1096](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000434 .idata$6
+[1097](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001568 .text
 [1098](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1099](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1100](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d4 .idata$7
-[1101](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000270 .idata$5
-[1102](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d8 .idata$4
-[1103](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000444 .idata$6
-[1104](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001598 .text
+[1100](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b8 .idata$7
+[1101](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000260 .idata$5
+[1102](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .idata$4
+[1103](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000418 .idata$6
+[1104](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001570 .text
 [1105](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1106](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1107](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d0 .idata$7
-[1108](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000268 .idata$5
-[1109](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 .idata$4
-[1110](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000428 .idata$6
-[1111](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000015a0 .text
+[1107](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b4 .idata$7
+[1108](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000258 .idata$5
+[1109](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c8 .idata$4
+[1110](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000408 .idata$6
+[1111](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001578 .text
 [1112](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1113](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1114](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006cc .idata$7
-[1115](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000260 .idata$5
-[1116](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c8 .idata$4
-[1117](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000418 .idata$6
-[1118](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000015a8 .text
+[1114](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b0 .idata$7
+[1115](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000250 .idata$5
+[1116](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c0 .idata$4
+[1117](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003f0 .idata$6
+[1118](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000001580 .text
 [1119](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
 [1120](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1121](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c8 .idata$7
-[1122](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000258 .idata$5
-[1123](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c0 .idata$4
-[1124](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000400 .idata$6
-[1125](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000015b0 .text
-[1126](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 .data
-[1127](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 .bss
-[1128](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c4 .idata$7
-[1129](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000250 .idata$5
-[1130](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 .idata$4
-[1131](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003e8 .idata$6
-[1132](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000047a fake
+[1121](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ac .idata$7
+[1122](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000248 .idata$5
+[1123](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 .idata$4
+[1124](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003d8 .idata$6
+[1125](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000473 fake
 File 
-[1134](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 hname
-[1135](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000250 fthunk
-[1136](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000015c0 .text
+[1127](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 hname
+[1128](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000248 fthunk
+[1129](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001590 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1138](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
+[1131](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1140](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1133](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1142](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .idata$2
+[1135](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[1144](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 .idata$4
-[1145](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000250 .idata$5
-[1146](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000488 fake
+[1137](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b8 .idata$4
+[1138](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000248 .idata$5
+[1139](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000481 fake
 File 
-[1148](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000015c0 .text
+[1141](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001590 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1150](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
+[1143](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1152](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1145](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1154](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000100 .idata$4
+[1147](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000100 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1156](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000298 .idata$5
+[1149](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000290 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1158](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006e8 .idata$7
+[1151](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006d0 .idata$7
 AUX scnlen 0xd nreloc 0 nlnno 0
-[1160](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000049c cygming-crtend
+[1153](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000495 cygming-crtend
 File 
-[1162](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000015c0 register_frame_ctor
+[1155](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000001590 register_frame_ctor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000015c0 .text
+[1157](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001590 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1166](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
+[1159](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000e0 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1168](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
+[1161](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000110 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1170](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000015c0 .text.startup
+[1163](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001590 .text.startup
 AUX scnlen 0x5 nreloc 1 nlnno 0
-[1172](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000018c .xdata.startup
+[1165](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000188 .xdata.startup
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[1174](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000234 .pdata.startup
+[1167](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000234 .pdata.startup
 AUX scnlen 0xc nreloc 3 nlnno 0
-[1176](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000015d8 .ctors.65535
+[1169](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000015a8 .ctors.65535
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[1178](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006a0 .rdata$zzz
+[1171](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006a0 .rdata$zzz
 AUX scnlen 0x2b nreloc 0 nlnno 0
-[1180](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 __xc_z
-[1181](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001460 putchar
-[1182](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 ___RUNTIME_PSEUDO_RELOC_LIST__
-[1183](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001400 __daylight
-[1184](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001440 __stdio_common_vfwprintf
-[1185](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000358 __imp_abort
-[1186](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006e8 __lib64_libkernel32_a_iname
-[1187](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b0 __imp___p__environ
-[1188](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __data_start__
-[1189](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015e8 ___DTOR_LIST__
-[1190](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000088 __imp_timezone
-[1191](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d0 __imp_calloc
-[1192](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e8 __imp___p___argc
-[1193](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000090 __imp_tzname
-[1194](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014c0 _initialize_onexit_table
-[1195](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___tls_start__
-[1196](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000290 .refptr.__native_startup_state
-[1197](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000058 __imp_tzset
-[1198](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 __xl_a
-[1199](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015a0 GetLastError
-[1200](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000340 __imp__initialize_wide_environment
-[1201](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __rt_psrelocs_start
-[1202](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000160 __dll_characteristics__
-[1203](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_stack_commit__
-[1204](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000850 __lib64_libapi_ms_win_crt_time_l1_1_0_a_iname
-[1205](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __mingw_module_is_dll
-[1206](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000200000 __size_of_stack_reserve__
-[1207](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000005 __major_subsystem_version__
-[1208](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xl_start__
-[1209](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000250 __imp_DeleteCriticalSection
-[1210](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __xl_d
-[1211](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 _tls_end
-[1212](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001f0 .refptr.__CTOR_LIST__
-[1213](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001410 __tzname
-[1214](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001570 VirtualQuery
-[1215](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f0 __imp___p___argv
-[1216](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xi_start__
-[1217](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000068 __imp__amsg_exit
-[1218](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xi_end__
-[1219](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000260 .refptr.__mingw_module_is_dll
-[1220](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _tls_start
-[1221](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006fc __lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname
-[1222](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000220 .refptr.__RUNTIME_PSEUDO_RELOC_LIST__
-[1223](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 _CRT_MT
-[1224](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001580 TlsGetValue
-[1225](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __bss_start__
-[1226](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000398 __imp_putchar
-[1227](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 ___RUNTIME_PSEUDO_RELOC_LIST_END__
-[1228](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003d0 __imp___tzname
-[1229](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_heap_commit__
-[1230](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000370 __imp___stdio_common_vfprintf
-[1231](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000260 __imp_GetLastError
-[1232](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001448 kbhit
-[1233](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000330 __imp__initialize_narrow_environment
-[1234](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 __mingw_initltsdrot_force
-[1235](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d8 __imp_free
-[1236](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000308 __imp__configure_wide_argv
-[1237](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000b8 __imp_at_quick_exit
-[1238](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001510 __p__environ
-[1239](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000250 .refptr.__mingw_app_type
-[1240](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __mingw_initltssuo_force
-[1241](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001450 fflush
-[1242](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001578 VirtualProtect
-[1243](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 _head_lib64_libapi_ms_win_crt_environment_l1_1_0_a
-[1244](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003d8 __imp__tzset
-[1245](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_start__
-[1246](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000270 __imp_LeaveCriticalSection
-[1247](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014e0 abort
-[1248](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000210 .refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
-[1249](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __imp___ms_fwprintf
-[1250](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_end__
-[1251](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll__
-[1252](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_os_version__
-[1253](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001478 __p___argv
-[1254](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000081c __lib64_libapi_ms_win_crt_string_l1_1_0_a_iname
-[1255](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015a8 EnterCriticalSection
-[1256](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 _head_lib64_libapi_ms_win_crt_conio_l1_1_0_a
-[1257](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014f0 _set_new_mode
-[1258](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c0 .refptr.__xi_a
-[1259](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001e0 .refptr._CRT_MT
-[1260](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001520 getch
-[1261](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000328 __imp__exit
-[1262](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __section_alignment__
-[1263](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000024 __native_dllmain_reason
-[1264](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014f8 calloc
-[1265](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 _tls_used
-[1266](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003e8 __IAT_end__
-[1267](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000008c _head_lib64_libapi_ms_win_crt_time_l1_1_0_a
-[1268](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __RUNTIME_PSEUDO_RELOC_LIST__
-[1269](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001588 Sleep
-[1270](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000e0 __data_end__
-[1271](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000390 __imp_fwrite
-[1272](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015d0 __CTOR_LIST__
-[1273](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a0 __imp_getch
-[1274](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c8 __imp__set_new_mode
-[1275](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000003c _head_lib64_libapi_ms_win_crt_heap_l1_1_0_a
-[1276](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000078 __imp___getmainargs
-[1277](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _head_lib64_libkernel32_a
-[1278](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000110 __bss_end__
-[1279](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __xi_z
-[1280](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000018 pcinit
-[1281](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __native_vcclrit_reason
-[1282](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xc_end__
-[1283](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000280 .refptr.__native_startup_lock
-[1284](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000258 __imp_EnterCriticalSection
-[1285](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000004c _tls_index
-[1286](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001430 __acrt_iob_func
-[1287](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __native_startup_state
-[1288](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___crt_xc_start__
-[1289](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000380 __imp_kbhit
-[1290](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001428 strncmp
-[1291](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015d0 ___CTOR_LIST__
-[1292](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000230 .refptr.__dyn_tls_init_callback
-[1293](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000350 __imp__register_onexit_function
-[1294](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000078 _head_lib64_libapi_ms_win_crt_string_l1_1_0_a
-[1295](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __rt_psrelocs_size
-[1296](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014a8 _execute_onexit_table
-[1297](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 .refptr.__ImageBase
-[1298](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007b4 __lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname
-[1299](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f8 __imp___p___wargv
-[1300](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003a8 __imp_strlen
-[1301](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000070 __imp___wgetmainargs
-[1302](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003c0 __imp___daylight
-[1303](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 __file_alignment__
-[1304](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000268 __imp_InitializeCriticalSection
-[1305](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001518 __p__wenviron
-[1306](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014b8 _initialize_narrow_environment
-[1307](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001498 _crt_at_quick_exit
-[1308](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001598 InitializeCriticalSection
-[1309](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000064 _head_lib64_libapi_ms_win_crt_stdio_l1_1_0_a
-[1310](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __imp_vfprintf
-[1311](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000004 __major_os_version__
-[1312](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000250 __IAT_start__
-[1313](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __xl_z
-[1314](sec  0)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __end__
-[1315](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000378 __imp___stdio_common_vfwprintf
-[1316](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000c0 __imp__onexit
-[1317](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015e8 __DTOR_LIST__
-[1318](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000338 __imp__initialize_onexit_table
-[1319](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __xi_a
-[1320](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000278 __imp_Sleep
-[1321](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001590 LeaveCriticalSection
-[1322](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __xc_a
-[1323](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000100000 __size_of_heap_reserve__
-[1324](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_start__
-[1325](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000003 __subsystem__
-[1326](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000280 __imp_TlsGetValue
-[1327](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b8 __imp___p__wenviron
-[1328](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000320 __imp__execute_onexit_table
-[1329](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003c8 __imp___timezone
-[1330](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000d0 __imp_fprintf
-[1331](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001490 _configure_wide_argv
-[1332](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000318 __imp__crt_atexit
-[1333](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000724 __lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname
-[1334](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014d8 _register_onexit_function
-[1335](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001470 __p___argc
-[1336](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000288 __imp_VirtualProtect
-[1337](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __xl_c
-[1338](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___tls_end__
-[1339](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000240 .refptr.__imp__tzset
-[1340](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000290 __imp_VirtualQuery
-[1341](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000348 __imp__initterm
-[1342](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000044 __mingw_initltsdyn_force
-[1343](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007f4 __lib64_libapi_ms_win_crt_stdio_l1_1_0_a_iname
-[1344](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dyn_tls_init_callback
-[1345](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001408 __timezone
-[1346](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000758 __lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname
-[1347](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014d0 _initterm
-[1348](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001458 fwrite
-[1349](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003b0 __imp_strncmp
-[1350](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000368 __imp___acrt_iob_func
-[1351](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __major_image_version__
-[1352](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __loader_flags__
-[1353](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001160 ___chkstk_ms
-[1354](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __native_startup_lock
-[1355](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000270 .refptr.__native_dllmain_reason
-[1356](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __rt_psrelocs_end
-[1357](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000002 __minor_subsystem_version__
-[1358](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000388 __imp_fflush
-[1359](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_image_version__
-[1360](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000310 __imp__crt_at_quick_exit
-[1361](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014b0 _exit
-[1362](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a0 .refptr.__xc_a
-[1363](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001488 _configure_narrow_argv
-[1364](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001420 strlen
-[1365](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d0 .refptr.__xi_z
-[1366](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014a0 _crt_atexit
-[1367](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015b0 DeleteCriticalSection
-[1368](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014c8 _initialize_wide_environment
-[1369](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000300 __imp__configure_narrow_argv
-[1370](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 _head_lib64_libapi_ms_win_crt_runtime_l1_1_0_a
-[1371](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __RUNTIME_PSEUDO_RELOC_LIST_END__
-[1372](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b0 .refptr.__xc_z
-[1373](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000060 __imp__get_output_format
-[1374](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_end__
-[1375](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001438 __stdio_common_vfprintf
-[1376](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000080 __imp_daylight
-[1377](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001480 __p___wargv
-[1378](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001500 free
-[1379](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __mingw_app_type
+[1173](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 __xc_z
+[1174](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001438 putchar
+[1175](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 ___RUNTIME_PSEUDO_RELOC_LIST__
+[1176](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013e0 __daylight
+[1177](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001420 __stdio_common_vfwprintf
+[1178](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000350 __imp_abort
+[1179](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __lib64_libkernel32_a_iname
+[1180](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a8 __imp___p__environ
+[1181](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __data_start__
+[1182](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015b8 ___DTOR_LIST__
+[1183](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000088 __imp_timezone
+[1184](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c8 __imp_calloc
+[1185](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e0 __imp___p___argc
+[1186](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000090 __imp_tzname
+[1187](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001490 _initialize_onexit_table
+[1188](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___tls_start__
+[1189](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000290 .refptr.__native_startup_state
+[1190](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000058 __imp_tzset
+[1191](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 __xl_a
+[1192](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001570 GetLastError
+[1193](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000338 __imp__initialize_wide_environment
+[1194](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __rt_psrelocs_start
+[1195](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000160 __dll_characteristics__
+[1196](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_stack_commit__
+[1197](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000834 __lib64_libapi_ms_win_crt_time_l1_1_0_a_iname
+[1198](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __mingw_module_is_dll
+[1199](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000200000 __size_of_stack_reserve__
+[1200](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000005 __major_subsystem_version__
+[1201](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xl_start__
+[1202](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000248 __imp_DeleteCriticalSection
+[1203](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __xl_d
+[1204](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 _tls_end
+[1205](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001f0 .refptr.__CTOR_LIST__
+[1206](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013f0 __tzname
+[1207](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001540 VirtualQuery
+[1208](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e8 __imp___p___argv
+[1209](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xi_start__
+[1210](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000068 __imp__amsg_exit
+[1211](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xi_end__
+[1212](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000260 .refptr.__mingw_module_is_dll
+[1213](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _tls_start
+[1214](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006e4 __lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname
+[1215](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000220 .refptr.__RUNTIME_PSEUDO_RELOC_LIST__
+[1216](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 _CRT_MT
+[1217](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001550 TlsGetValue
+[1218](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __bss_start__
+[1219](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000388 __imp_putchar
+[1220](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 ___RUNTIME_PSEUDO_RELOC_LIST_END__
+[1221](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003c0 __imp___tzname
+[1222](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_heap_commit__
+[1223](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000368 __imp___stdio_common_vfprintf
+[1224](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000258 __imp_GetLastError
+[1225](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001428 kbhit
+[1226](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000328 __imp__initialize_narrow_environment
+[1227](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 __mingw_initltsdrot_force
+[1228](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d0 __imp_free
+[1229](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000300 __imp__configure_wide_argv
+[1230](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000b8 __imp_at_quick_exit
+[1231](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014e0 __p__environ
+[1232](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000250 .refptr.__mingw_app_type
+[1233](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __mingw_initltssuo_force
+[1234](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001548 VirtualProtect
+[1235](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 _head_lib64_libapi_ms_win_crt_environment_l1_1_0_a
+[1236](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003c8 __imp__tzset
+[1237](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_start__
+[1238](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000268 __imp_LeaveCriticalSection
+[1239](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014b0 abort
+[1240](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000210 .refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
+[1241](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __imp___ms_fwprintf
+[1242](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_end__
+[1243](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll__
+[1244](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_os_version__
+[1245](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001448 __p___argv
+[1246](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000800 __lib64_libapi_ms_win_crt_string_l1_1_0_a_iname
+[1247](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001578 EnterCriticalSection
+[1248](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 _head_lib64_libapi_ms_win_crt_conio_l1_1_0_a
+[1249](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014c0 _set_new_mode
+[1250](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c0 .refptr.__xi_a
+[1251](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001e0 .refptr._CRT_MT
+[1252](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014f0 getch
+[1253](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000320 __imp__exit
+[1254](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __section_alignment__
+[1255](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000024 __native_dllmain_reason
+[1256](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014c8 calloc
+[1257](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 _tls_used
+[1258](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003d8 __IAT_end__
+[1259](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000008c _head_lib64_libapi_ms_win_crt_time_l1_1_0_a
+[1260](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __RUNTIME_PSEUDO_RELOC_LIST__
+[1261](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001558 Sleep
+[1262](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000e0 __data_end__
+[1263](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000380 __imp_fwrite
+[1264](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015a0 __CTOR_LIST__
+[1265](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000298 __imp_getch
+[1266](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c0 __imp__set_new_mode
+[1267](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000003c _head_lib64_libapi_ms_win_crt_heap_l1_1_0_a
+[1268](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000078 __imp___getmainargs
+[1269](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _head_lib64_libkernel32_a
+[1270](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000110 __bss_end__
+[1271](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __xi_z
+[1272](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000018 pcinit
+[1273](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __native_vcclrit_reason
+[1274](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xc_end__
+[1275](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000280 .refptr.__native_startup_lock
+[1276](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000250 __imp_EnterCriticalSection
+[1277](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000004c _tls_index
+[1278](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001410 __acrt_iob_func
+[1279](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __native_startup_state
+[1280](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___crt_xc_start__
+[1281](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000378 __imp_kbhit
+[1282](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001408 strncmp
+[1283](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015a0 ___CTOR_LIST__
+[1284](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000230 .refptr.__dyn_tls_init_callback
+[1285](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000348 __imp__register_onexit_function
+[1286](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000078 _head_lib64_libapi_ms_win_crt_string_l1_1_0_a
+[1287](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __rt_psrelocs_size
+[1288](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001478 _execute_onexit_table
+[1289](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 .refptr.__ImageBase
+[1290](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000079c __lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname
+[1291](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f0 __imp___p___wargv
+[1292](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000398 __imp_strlen
+[1293](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000070 __imp___wgetmainargs
+[1294](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003b0 __imp___daylight
+[1295](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 __file_alignment__
+[1296](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000260 __imp_InitializeCriticalSection
+[1297](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014e8 __p__wenviron
+[1298](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001488 _initialize_narrow_environment
+[1299](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001468 _crt_at_quick_exit
+[1300](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001568 InitializeCriticalSection
+[1301](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000064 _head_lib64_libapi_ms_win_crt_stdio_l1_1_0_a
+[1302](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __imp_vfprintf
+[1303](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000004 __major_os_version__
+[1304](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000248 __IAT_start__
+[1305](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __xl_z
+[1306](sec  0)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __end__
+[1307](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000370 __imp___stdio_common_vfwprintf
+[1308](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000c0 __imp__onexit
+[1309](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000015b8 __DTOR_LIST__
+[1310](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000330 __imp__initialize_onexit_table
+[1311](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __xi_a
+[1312](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000270 __imp_Sleep
+[1313](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001560 LeaveCriticalSection
+[1314](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __xc_a
+[1315](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000100000 __size_of_heap_reserve__
+[1316](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_start__
+[1317](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000003 __subsystem__
+[1318](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000278 __imp_TlsGetValue
+[1319](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b0 __imp___p__wenviron
+[1320](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000318 __imp__execute_onexit_table
+[1321](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003b8 __imp___timezone
+[1322](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000d0 __imp_fprintf
+[1323](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001460 _configure_wide_argv
+[1324](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000310 __imp__crt_atexit
+[1325](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000070c __lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname
+[1326](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014a8 _register_onexit_function
+[1327](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001440 __p___argc
+[1328](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000280 __imp_VirtualProtect
+[1329](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __xl_c
+[1330](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___tls_end__
+[1331](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000240 .refptr.__imp__tzset
+[1332](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000288 __imp_VirtualQuery
+[1333](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000340 __imp__initterm
+[1334](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000044 __mingw_initltsdyn_force
+[1335](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007d8 __lib64_libapi_ms_win_crt_stdio_l1_1_0_a_iname
+[1336](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dyn_tls_init_callback
+[1337](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013e8 __timezone
+[1338](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000740 __lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname
+[1339](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014a0 _initterm
+[1340](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001430 fwrite
+[1341](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000003a0 __imp_strncmp
+[1342](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000360 __imp___acrt_iob_func
+[1343](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __major_image_version__
+[1344](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __loader_flags__
+[1345](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001140 ___chkstk_ms
+[1346](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __native_startup_lock
+[1347](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000270 .refptr.__native_dllmain_reason
+[1348](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __rt_psrelocs_end
+[1349](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000002 __minor_subsystem_version__
+[1350](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_image_version__
+[1351](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000308 __imp__crt_at_quick_exit
+[1352](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001480 _exit
+[1353](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a0 .refptr.__xc_a
+[1354](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001458 _configure_narrow_argv
+[1355](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001400 strlen
+[1356](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d0 .refptr.__xi_z
+[1357](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001470 _crt_atexit
+[1358](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001580 DeleteCriticalSection
+[1359](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001498 _initialize_wide_environment
+[1360](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f8 __imp__configure_narrow_argv
+[1361](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 _head_lib64_libapi_ms_win_crt_runtime_l1_1_0_a
+[1362](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 __RUNTIME_PSEUDO_RELOC_LIST_END__
+[1363](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b0 .refptr.__xc_z
+[1364](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000060 __imp__get_output_format
+[1365](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_end__
+[1366](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001418 __stdio_common_vfprintf
+[1367](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000080 __imp_daylight
+[1368](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001450 __p___wargv
+[1369](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000014d0 free
+[1370](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __mingw_app_type
 
 
 
 Disassembly of section .text:
 
 000000029a1b1000 <pre_c_init>:
 pre_c_init():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:64
    29a1b1000:	lea    0x5ff9(%rip),%rcx        # 29a1b7000 <__bss_start__>
-   29a1b1007:	jmp    29a1b24c0 <_initialize_onexit_table>
+   29a1b1007:	jmp    29a1b2490 <_initialize_onexit_table>
    29a1b100c:	nopl   0x0(%rax)
 
 000000029a1b1010 <_CRT_INIT>:
 _CRT_INIT():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:68
    29a1b1010:	push   %r13
    29a1b1012:	push   %r12
@@ -1982,15 +1971,15 @@
 C:\M\B\src\build-UCRT64/D:/a/msys64/ucrt64/include/psdk_inc/intrin-impl.h:1737
    29a1b103a:	xor    %ebp,%ebp
    29a1b103c:	mov    $0x1,%edi
 _CRT_INIT():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:72
    29a1b1041:	mov    %eax,0x5fd1(%rip)        # 29a1b7018 <__proc_attached>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:122
-   29a1b1047:	mov    0x822a(%rip),%r12        # 29a1b9278 <__imp_Sleep>
+   29a1b1047:	mov    0x8222(%rip),%r12        # 29a1b9270 <__imp_Sleep>
    29a1b104e:	jmp    29a1b1058 <_CRT_INIT+0x48>
    29a1b1050:	mov    $0x3e8,%ecx
    29a1b1055:	call   *%r12
 _InterlockedCompareExchangePointer():
 C:\M\B\src\build-UCRT64/D:/a/msys64/ucrt64/include/psdk_inc/intrin-impl.h:1737
    29a1b1058:	mov    %rbp,%rax
    29a1b105b:	lock cmpxchg %rdi,(%rbx)
@@ -2002,15 +1991,15 @@
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:124
    29a1b1068:	mov    0x3221(%rip),%rdi        # 29a1b4290 <.refptr.__native_startup_state>
    29a1b106f:	mov    (%rdi),%eax
    29a1b1071:	cmp    $0x2,%eax
    29a1b1074:	je     29a1b1140 <_CRT_INIT+0x130>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:126
    29a1b107a:	mov    $0x1f,%ecx
-   29a1b107f:	call   29a1b2310 <_amsg_exit>
+   29a1b107f:	call   29a1b22f0 <_amsg_exit>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:135
    29a1b1084:	mov    $0x1,%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:136
    29a1b1089:	mov    %edx,%eax
    29a1b108b:	add    $0x28,%rsp
    29a1b108f:	pop    %rbx
    29a1b1090:	pop    %rsi
@@ -2031,15 +2020,15 @@
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:79
    29a1b10b5:	mov    0x8(%rax),%rsi
 _InterlockedCompareExchangePointer():
 C:\M\B\src\build-UCRT64/D:/a/msys64/ucrt64/include/psdk_inc/intrin-impl.h:1737
    29a1b10b9:	xor    %ebp,%ebp
 _CRT_INIT():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:90
-   29a1b10bb:	mov    0x81b6(%rip),%r12        # 29a1b9278 <__imp_Sleep>
+   29a1b10bb:	mov    0x81ae(%rip),%r12        # 29a1b9270 <__imp_Sleep>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:82
    29a1b10c2:	jmp    29a1b10d9 <_CRT_INIT+0xc9>
    29a1b10c4:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:85
    29a1b10c8:	cmp    %rax,%rsi
    29a1b10cb:	je     29a1b1160 <_CRT_INIT+0x150>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:90
@@ -2084,15 +2073,15 @@
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:115
    29a1b112f:	addl   $0x1,0x5ee2(%rip)        # 29a1b7018 <__proc_attached>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:135
    29a1b1136:	mov    $0x1,%edx
    29a1b113b:	jmp    29a1b1089 <_CRT_INIT+0x79>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:130
    29a1b1140:	lea    0x5eb9(%rip),%rcx        # 29a1b7000 <__bss_start__>
-   29a1b1147:	call   29a1b24a8 <_execute_onexit_table>
+   29a1b1147:	call   29a1b2478 <_execute_onexit_table>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:131
    29a1b114c:	movl   $0x0,(%rdi)
 _InterlockedExchangePointer():
 C:\M\B\src\build-UCRT64/D:/a/msys64/ucrt64/include/psdk_inc/intrin-impl.h:1748
    29a1b1152:	xchg   %rsi,(%rbx)
    29a1b1155:	jmp    29a1b1084 <_CRT_INIT+0x74>
    29a1b115a:	nopw   0x0(%rax,%rax,1)
@@ -2110,28 +2099,28 @@
 _CRT_INIT():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:100
    29a1b1180:	mov    0x3149(%rip),%rdx        # 29a1b42d0 <.refptr.__xi_z>
    29a1b1187:	mov    0x3132(%rip),%rcx        # 29a1b42c0 <.refptr.__xi_a>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:98
    29a1b118e:	movl   $0x1,(%rsi)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:100
-   29a1b1194:	call   29a1b24d0 <_initterm>
+   29a1b1194:	call   29a1b24a0 <_initterm>
    29a1b1199:	jmp    29a1b1104 <_CRT_INIT+0xf4>
    29a1b119e:	xchg   %ax,%ax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:104
    29a1b11a0:	mov    0x3109(%rip),%rdx        # 29a1b42b0 <.refptr.__xc_z>
    29a1b11a7:	mov    0x30f2(%rip),%rcx        # 29a1b42a0 <.refptr.__xc_a>
-   29a1b11ae:	call   29a1b24d0 <_initterm>
+   29a1b11ae:	call   29a1b24a0 <_initterm>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:105
    29a1b11b3:	movl   $0x2,(%rsi)
    29a1b11b9:	jmp    29a1b110f <_CRT_INIT+0xff>
    29a1b11be:	xchg   %ax,%ax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:94
    29a1b11c0:	mov    $0x1f,%ecx
-   29a1b11c5:	call   29a1b2310 <_amsg_exit>
+   29a1b11c5:	call   29a1b22f0 <_amsg_exit>
    29a1b11ca:	jmp    29a1b1104 <_CRT_INIT+0xf4>
    29a1b11cf:	nop
 
 000000029a1b11d0 <__DllMainCRTStartup>:
 __DllMainCRTStartup():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:161
    29a1b11d0:	push   %r12
@@ -2152,25 +2141,25 @@
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:165
    29a1b11ec:	test   %edx,%edx
    29a1b11ee:	jne    29a1b1250 <__DllMainCRTStartup+0x80>
    29a1b11f0:	mov    0x5e22(%rip),%eax        # 29a1b7018 <__proc_attached>
    29a1b11f6:	test   %eax,%eax
    29a1b11f8:	je     29a1b1230 <__DllMainCRTStartup+0x60>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:170
-   29a1b11fa:	call   29a1b1780 <_pei386_runtime_relocator>
+   29a1b11fa:	call   29a1b1760 <_pei386_runtime_relocator>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:186
    29a1b11ff:	mov    %rdi,%r8
    29a1b1202:	xor    %edx,%edx
    29a1b1204:	mov    %rsi,%rcx
-   29a1b1207:	call   29a1b21b0 <DllMain>
+   29a1b1207:	call   29a1b2190 <DllMain>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:195
    29a1b120c:	mov    %rdi,%r8
    29a1b120f:	mov    %ebx,%edx
    29a1b1211:	mov    %rsi,%rcx
-   29a1b1214:	call   29a1b21a0 <DllEntryPoint>
+   29a1b1214:	call   29a1b2180 <DllEntryPoint>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:196
    29a1b1219:	mov    %rdi,%r8
    29a1b121c:	mov    %ebx,%edx
    29a1b121e:	mov    %rsi,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:195
    29a1b1221:	mov    %eax,%r12d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:196
@@ -2190,15 +2179,15 @@
    29a1b1242:	pop    %rsi
    29a1b1243:	pop    %rdi
    29a1b1244:	pop    %rbp
    29a1b1245:	pop    %r12
    29a1b1247:	ret
    29a1b1248:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:170
-   29a1b1250:	call   29a1b1780 <_pei386_runtime_relocator>
+   29a1b1250:	call   29a1b1760 <_pei386_runtime_relocator>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:171
    29a1b1255:	lea    -0x1(%rbx),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:173
    29a1b1258:	mov    %rdi,%r8
    29a1b125b:	mov    %ebx,%edx
    29a1b125d:	mov    %rsi,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:171
@@ -2209,32 +2198,32 @@
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:174
    29a1b126a:	test   %eax,%eax
    29a1b126c:	je     29a1b1230 <__DllMainCRTStartup+0x60>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:176
    29a1b126e:	mov    %rdi,%r8
    29a1b1271:	mov    %ebx,%edx
    29a1b1273:	mov    %rsi,%rcx
-   29a1b1276:	call   29a1b21a0 <DllEntryPoint>
+   29a1b1276:	call   29a1b2180 <DllEntryPoint>
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
-   29a1b128f:	call   29a1b21b0 <DllMain>
+   29a1b128f:	call   29a1b2190 <DllMain>
    29a1b1294:	mov    %eax,%r12d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:193
    29a1b1297:	jmp    29a1b1233 <__DllMainCRTStartup+0x63>
    29a1b1299:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:186
-   29a1b12a0:	call   29a1b21b0 <DllMain>
+   29a1b12a0:	call   29a1b2190 <DllMain>
    29a1b12a5:	mov    %eax,%r12d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:193
    29a1b12a8:	cmp    $0x3,%ebx
    29a1b12ab:	jne    29a1b1233 <__DllMainCRTStartup+0x63>
    29a1b12ad:	jmp    29a1b120c <__DllMainCRTStartup+0x3c>
    29a1b12b2:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:179
@@ -2244,34 +2233,34 @@
    29a1b12c1:	mov    %rdi,%r8
    29a1b12c4:	xor    %edx,%edx
    29a1b12c6:	mov    %rsi,%rcx
    29a1b12c9:	call   29a1b1010 <_CRT_INIT>
    29a1b12ce:	jmp    29a1b1230 <__DllMainCRTStartup+0x60>
    29a1b12d3:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:185
-   29a1b12d8:	call   29a1b14b0 <__main>
+   29a1b12d8:	call   29a1b1490 <__main>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:186
    29a1b12dd:	mov    %rdi,%r8
    29a1b12e0:	mov    $0x1,%edx
    29a1b12e5:	mov    %rsi,%rcx
-   29a1b12e8:	call   29a1b21b0 <DllMain>
+   29a1b12e8:	call   29a1b2190 <DllMain>
    29a1b12ed:	mov    %eax,%r12d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:187
    29a1b12f0:	test   %eax,%eax
    29a1b12f2:	jne    29a1b1233 <__DllMainCRTStartup+0x63>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:189
    29a1b12f8:	mov    %rdi,%r8
    29a1b12fb:	xor    %edx,%edx
    29a1b12fd:	mov    %rsi,%rcx
-   29a1b1300:	call   29a1b21b0 <DllMain>
+   29a1b1300:	call   29a1b2190 <DllMain>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:190
    29a1b1305:	mov    %rdi,%r8
    29a1b1308:	xor    %edx,%edx
    29a1b130a:	mov    %rsi,%rcx
-   29a1b130d:	call   29a1b21a0 <DllEntryPoint>
+   29a1b130d:	call   29a1b2180 <DllEntryPoint>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:191
    29a1b1312:	mov    %rdi,%r8
    29a1b1315:	xor    %edx,%edx
    29a1b1317:	mov    %rsi,%rcx
    29a1b131a:	call   29a1b1010 <_CRT_INIT>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:193
    29a1b131f:	jmp    29a1b1233 <__DllMainCRTStartup+0x63>
@@ -2290,15 +2279,15 @@
 
 000000029a1b1350 <atexit>:
 atexit():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:206
    29a1b1350:	mov    %rcx,%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/crtdll.c:207
    29a1b1353:	lea    0x5ca6(%rip),%rcx        # 29a1b7000 <__bss_start__>
-   29a1b135a:	jmp    29a1b24d8 <_register_onexit_function>
+   29a1b135a:	jmp    29a1b24a8 <_register_onexit_function>
    29a1b135f:	nop
 
 000000029a1b1360 <__gcc_register_frame>:
    29a1b1360:	lea    0x9(%rip),%rcx        # 29a1b1370 <__gcc_deregister_frame>
    29a1b1367:	jmp    29a1b1350 <atexit>
    29a1b136c:	nopl   0x0(%rax)
 
@@ -2319,2185 +2308,2171 @@
    29a1b137d:	nop
    29a1b137e:	nop
    29a1b137f:	nop
 
 000000029a1b1380 <init>:
    29a1b1380:	push   %rbp
    29a1b1381:	mov    %rsp,%rbp
-   29a1b1384:	sub    $0x20,%rsp
-   29a1b1388:	mov    $0x0,%ecx
-   29a1b138d:	mov    0x7fd4(%rip),%rax        # 29a1b9368 <__imp___acrt_iob_func>
-   29a1b1394:	call   *%rax
-   29a1b1396:	mov    %rax,%rcx
-   29a1b1399:	call   29a1b2450 <fflush>
-   29a1b139e:	nop
-   29a1b139f:	add    $0x20,%rsp
-   29a1b13a3:	pop    %rbp
-   29a1b13a4:	ret
-
-000000029a1b13a5 <isInputReady>:
-   29a1b13a5:	push   %rbp
-   29a1b13a6:	mov    %rsp,%rbp
-   29a1b13a9:	sub    $0x20,%rsp
-   29a1b13ad:	call   29a1b2448 <kbhit>
-   29a1b13b2:	add    $0x20,%rsp
-   29a1b13b6:	pop    %rbp
-   29a1b13b7:	ret
-
-000000029a1b13b8 <getCharacter>:
-   29a1b13b8:	push   %rbp
-   29a1b13b9:	mov    %rsp,%rbp
-   29a1b13bc:	sub    $0x30,%rsp
-   29a1b13c0:	call   29a1b2520 <getch>
-   29a1b13c5:	mov    %eax,-0x4(%rbp)
-   29a1b13c8:	mov    -0x4(%rbp),%eax
-   29a1b13cb:	cmp    $0xd,%al
-   29a1b13cd:	jne    29a1b13d6 <getCharacter+0x1e>
-   29a1b13cf:	movl   $0xa,-0x4(%rbp)
-   29a1b13d6:	mov    -0x4(%rbp),%eax
-   29a1b13d9:	movsbl %al,%eax
-   29a1b13dc:	mov    %eax,%ecx
-   29a1b13de:	call   29a1b2460 <putchar>
-   29a1b13e3:	mov    -0x4(%rbp),%eax
-   29a1b13e6:	add    $0x30,%rsp
-   29a1b13ea:	pop    %rbp
-   29a1b13eb:	ret
-
-000000029a1b13ec <stop>:
-   29a1b13ec:	push   %rbp
-   29a1b13ed:	mov    %rsp,%rbp
-   29a1b13f0:	nop
-   29a1b13f1:	pop    %rbp
-   29a1b13f2:	ret
-   29a1b13f3:	nop
-   29a1b13f4:	nop
-   29a1b13f5:	nop
-   29a1b13f6:	nop
-   29a1b13f7:	nop
-   29a1b13f8:	nop
-   29a1b13f9:	nop
-   29a1b13fa:	nop
-   29a1b13fb:	nop
-   29a1b13fc:	nop
-   29a1b13fd:	nop
-   29a1b13fe:	nop
-   29a1b13ff:	nop
+   29a1b1384:	nop
+   29a1b1385:	pop    %rbp
+   29a1b1386:	ret
+
+000000029a1b1387 <isInputReady>:
+   29a1b1387:	push   %rbp
+   29a1b1388:	mov    %rsp,%rbp
+   29a1b138b:	sub    $0x20,%rsp
+   29a1b138f:	call   29a1b2428 <kbhit>
+   29a1b1394:	add    $0x20,%rsp
+   29a1b1398:	pop    %rbp
+   29a1b1399:	ret
+
+000000029a1b139a <getCharacter>:
+   29a1b139a:	push   %rbp
+   29a1b139b:	mov    %rsp,%rbp
+   29a1b139e:	sub    $0x30,%rsp
+   29a1b13a2:	call   29a1b24f0 <getch>
+   29a1b13a7:	mov    %eax,-0x4(%rbp)
+   29a1b13aa:	mov    -0x4(%rbp),%eax
+   29a1b13ad:	cmp    $0xd,%al
+   29a1b13af:	jne    29a1b13b8 <getCharacter+0x1e>
+   29a1b13b1:	movl   $0xa,-0x4(%rbp)
+   29a1b13b8:	mov    -0x4(%rbp),%eax
+   29a1b13bb:	movsbl %al,%eax
+   29a1b13be:	mov    %eax,%ecx
+   29a1b13c0:	call   29a1b2438 <putchar>
+   29a1b13c5:	mov    -0x4(%rbp),%eax
+   29a1b13c8:	add    $0x30,%rsp
+   29a1b13cc:	pop    %rbp
+   29a1b13cd:	ret
+
+000000029a1b13ce <stop>:
+   29a1b13ce:	push   %rbp
+   29a1b13cf:	mov    %rsp,%rbp
+   29a1b13d2:	nop
+   29a1b13d3:	pop    %rbp
+   29a1b13d4:	ret
+   29a1b13d5:	nop
+   29a1b13d6:	nop
+   29a1b13d7:	nop
+   29a1b13d8:	nop
+   29a1b13d9:	nop
+   29a1b13da:	nop
+   29a1b13db:	nop
+   29a1b13dc:	nop
+   29a1b13dd:	nop
+   29a1b13de:	nop
+   29a1b13df:	nop
 
-000000029a1b1400 <__do_global_dtors>:
+000000029a1b13e0 <__do_global_dtors>:
 __do_global_dtors():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:21
-   29a1b1400:	sub    $0x28,%rsp
+   29a1b13e0:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:24
-   29a1b1404:	mov    0x1c05(%rip),%rax        # 29a1b3010 <p.0>
-   29a1b140b:	mov    (%rax),%rax
-   29a1b140e:	test   %rax,%rax
-   29a1b1411:	je     29a1b1435 <__do_global_dtors+0x35>
-   29a1b1413:	nopl   0x0(%rax,%rax,1)
+   29a1b13e4:	mov    0x1c25(%rip),%rax        # 29a1b3010 <p.0>
+   29a1b13eb:	mov    (%rax),%rax
+   29a1b13ee:	test   %rax,%rax
+   29a1b13f1:	je     29a1b1415 <__do_global_dtors+0x35>
+   29a1b13f3:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:26
-   29a1b1418:	call   *%rax
+   29a1b13f8:	call   *%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:27
-   29a1b141a:	mov    0x1bef(%rip),%rax        # 29a1b3010 <p.0>
-   29a1b1421:	lea    0x8(%rax),%rdx
+   29a1b13fa:	mov    0x1c0f(%rip),%rax        # 29a1b3010 <p.0>
+   29a1b1401:	lea    0x8(%rax),%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:24
-   29a1b1425:	mov    0x8(%rax),%rax
+   29a1b1405:	mov    0x8(%rax),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:27
-   29a1b1429:	mov    %rdx,0x1be0(%rip)        # 29a1b3010 <p.0>
+   29a1b1409:	mov    %rdx,0x1c00(%rip)        # 29a1b3010 <p.0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:24
-   29a1b1430:	test   %rax,%rax
-   29a1b1433:	jne    29a1b1418 <__do_global_dtors+0x18>
+   29a1b1410:	test   %rax,%rax
+   29a1b1413:	jne    29a1b13f8 <__do_global_dtors+0x18>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:29
-   29a1b1435:	add    $0x28,%rsp
-   29a1b1439:	ret
-   29a1b143a:	nopw   0x0(%rax,%rax,1)
+   29a1b1415:	add    $0x28,%rsp
+   29a1b1419:	ret
+   29a1b141a:	nopw   0x0(%rax,%rax,1)
 
-000000029a1b1440 <__do_global_ctors>:
+000000029a1b1420 <__do_global_ctors>:
 __do_global_ctors():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:33
-   29a1b1440:	push   %rsi
-   29a1b1441:	push   %rbx
-   29a1b1442:	sub    $0x28,%rsp
+   29a1b1420:	push   %rsi
+   29a1b1421:	push   %rbx
+   29a1b1422:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:34
-   29a1b1446:	mov    0x2da3(%rip),%rdx        # 29a1b41f0 <.refptr.__CTOR_LIST__>
-   29a1b144d:	mov    (%rdx),%rax
-   29a1b1450:	mov    %eax,%ecx
+   29a1b1426:	mov    0x2dc3(%rip),%rdx        # 29a1b41f0 <.refptr.__CTOR_LIST__>
+   29a1b142d:	mov    (%rdx),%rax
+   29a1b1430:	mov    %eax,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:37
-   29a1b1452:	cmp    $0xffffffff,%eax
-   29a1b1455:	je     29a1b1490 <__do_global_ctors+0x50>
+   29a1b1432:	cmp    $0xffffffff,%eax
+   29a1b1435:	je     29a1b1470 <__do_global_ctors+0x50>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:42
-   29a1b1457:	test   %ecx,%ecx
-   29a1b1459:	je     29a1b147b <__do_global_ctors+0x3b>
-   29a1b145b:	mov    %ecx,%eax
-   29a1b145d:	sub    $0x1,%ecx
-   29a1b1460:	lea    (%rdx,%rax,8),%rbx
-   29a1b1464:	sub    %rcx,%rax
-   29a1b1467:	lea    -0x8(%rdx,%rax,8),%rsi
-   29a1b146c:	nopl   0x0(%rax)
+   29a1b1437:	test   %ecx,%ecx
+   29a1b1439:	je     29a1b145b <__do_global_ctors+0x3b>
+   29a1b143b:	mov    %ecx,%eax
+   29a1b143d:	sub    $0x1,%ecx
+   29a1b1440:	lea    (%rdx,%rax,8),%rbx
+   29a1b1444:	sub    %rcx,%rax
+   29a1b1447:	lea    -0x8(%rdx,%rax,8),%rsi
+   29a1b144c:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:44
-   29a1b1470:	call   *(%rbx)
+   29a1b1450:	call   *(%rbx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:42
-   29a1b1472:	sub    $0x8,%rbx
-   29a1b1476:	cmp    %rsi,%rbx
-   29a1b1479:	jne    29a1b1470 <__do_global_ctors+0x30>
+   29a1b1452:	sub    $0x8,%rbx
+   29a1b1456:	cmp    %rsi,%rbx
+   29a1b1459:	jne    29a1b1450 <__do_global_ctors+0x30>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:47
-   29a1b147b:	lea    -0x82(%rip),%rcx        # 29a1b1400 <__do_global_dtors>
+   29a1b145b:	lea    -0x82(%rip),%rcx        # 29a1b13e0 <__do_global_dtors>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:48
-   29a1b1482:	add    $0x28,%rsp
-   29a1b1486:	pop    %rbx
-   29a1b1487:	pop    %rsi
+   29a1b1462:	add    $0x28,%rsp
+   29a1b1466:	pop    %rbx
+   29a1b1467:	pop    %rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:47
-   29a1b1488:	jmp    29a1b1350 <atexit>
-   29a1b148d:	nopl   (%rax)
+   29a1b1468:	jmp    29a1b1350 <atexit>
+   29a1b146d:	nopl   (%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:39
-   29a1b1490:	xor    %eax,%eax
-   29a1b1492:	nopw   0x0(%rax,%rax,1)
-   29a1b1498:	lea    0x1(%rax),%r8d
-   29a1b149c:	mov    %eax,%ecx
-   29a1b149e:	cmpq   $0x0,(%rdx,%r8,8)
-   29a1b14a3:	mov    %r8,%rax
-   29a1b14a6:	jne    29a1b1498 <__do_global_ctors+0x58>
-   29a1b14a8:	jmp    29a1b1457 <__do_global_ctors+0x17>
-   29a1b14aa:	nopw   0x0(%rax,%rax,1)
+   29a1b1470:	xor    %eax,%eax
+   29a1b1472:	nopw   0x0(%rax,%rax,1)
+   29a1b1478:	lea    0x1(%rax),%r8d
+   29a1b147c:	mov    %eax,%ecx
+   29a1b147e:	cmpq   $0x0,(%rdx,%r8,8)
+   29a1b1483:	mov    %r8,%rax
+   29a1b1486:	jne    29a1b1478 <__do_global_ctors+0x58>
+   29a1b1488:	jmp    29a1b1437 <__do_global_ctors+0x17>
+   29a1b148a:	nopw   0x0(%rax,%rax,1)
 
-000000029a1b14b0 <__main>:
+000000029a1b1490 <__main>:
 __main():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:55
-   29a1b14b0:	mov    0x5b6a(%rip),%eax        # 29a1b7020 <initialized>
-   29a1b14b6:	test   %eax,%eax
-   29a1b14b8:	je     29a1b14c0 <__main+0x10>
+   29a1b1490:	mov    0x5b8a(%rip),%eax        # 29a1b7020 <initialized>
+   29a1b1496:	test   %eax,%eax
+   29a1b1498:	je     29a1b14a0 <__main+0x10>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:60
-   29a1b14ba:	ret
-   29a1b14bb:	nopl   0x0(%rax,%rax,1)
+   29a1b149a:	ret
+   29a1b149b:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:57
-   29a1b14c0:	movl   $0x1,0x5b56(%rip)        # 29a1b7020 <initialized>
+   29a1b14a0:	movl   $0x1,0x5b76(%rip)        # 29a1b7020 <initialized>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/gccmain.c:58
-   29a1b14ca:	jmp    29a1b1440 <__do_global_ctors>
-   29a1b14cf:	nop
+   29a1b14aa:	jmp    29a1b1420 <__do_global_ctors>
+   29a1b14af:	nop
 
-000000029a1b14d0 <__dyn_tls_dtor>:
+000000029a1b14b0 <__dyn_tls_dtor>:
 __dyn_tls_dtor():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:138
-   29a1b14d0:	sub    $0x28,%rsp
+   29a1b14b0:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:144
-   29a1b14d4:	cmp    $0x3,%edx
-   29a1b14d7:	je     29a1b14f0 <__dyn_tls_dtor+0x20>
-   29a1b14d9:	test   %edx,%edx
-   29a1b14db:	je     29a1b14f0 <__dyn_tls_dtor+0x20>
+   29a1b14b4:	cmp    $0x3,%edx
+   29a1b14b7:	je     29a1b14d0 <__dyn_tls_dtor+0x20>
+   29a1b14b9:	test   %edx,%edx
+   29a1b14bb:	je     29a1b14d0 <__dyn_tls_dtor+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:169
-   29a1b14dd:	mov    $0x1,%eax
-   29a1b14e2:	add    $0x28,%rsp
-   29a1b14e6:	ret
-   29a1b14e7:	nopw   0x0(%rax,%rax,1)
+   29a1b14bd:	mov    $0x1,%eax
+   29a1b14c2:	add    $0x28,%rsp
+   29a1b14c6:	ret
+   29a1b14c7:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:167
-   29a1b14f0:	call   29a1b1c50 <__mingw_TLScallback>
+   29a1b14d0:	call   29a1b1c30 <__mingw_TLScallback>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:169
-   29a1b14f5:	mov    $0x1,%eax
-   29a1b14fa:	add    $0x28,%rsp
-   29a1b14fe:	ret
-   29a1b14ff:	nop
+   29a1b14d5:	mov    $0x1,%eax
+   29a1b14da:	add    $0x28,%rsp
+   29a1b14de:	ret
+   29a1b14df:	nop
 
-000000029a1b1500 <__dyn_tls_init>:
+000000029a1b14e0 <__dyn_tls_init>:
 __dyn_tls_init():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:78
-   29a1b1500:	push   %rsi
-   29a1b1501:	push   %rbx
-   29a1b1502:	sub    $0x28,%rsp
+   29a1b14e0:	push   %rsi
+   29a1b14e1:	push   %rbx
+   29a1b14e2:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:83
-   29a1b1506:	mov    0x2cd3(%rip),%rax        # 29a1b41e0 <.refptr._CRT_MT>
-   29a1b150d:	cmpl   $0x2,(%rax)
-   29a1b1510:	je     29a1b1518 <__dyn_tls_init+0x18>
+   29a1b14e6:	mov    0x2cf3(%rip),%rax        # 29a1b41e0 <.refptr._CRT_MT>
+   29a1b14ed:	cmpl   $0x2,(%rax)
+   29a1b14f0:	je     29a1b14f8 <__dyn_tls_init+0x18>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:84
-   29a1b1512:	movl   $0x2,(%rax)
+   29a1b14f2:	movl   $0x2,(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:86
-   29a1b1518:	cmp    $0x2,%edx
-   29a1b151b:	je     29a1b1530 <__dyn_tls_init+0x30>
+   29a1b14f8:	cmp    $0x2,%edx
+   29a1b14fb:	je     29a1b1510 <__dyn_tls_init+0x30>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:88
-   29a1b151d:	cmp    $0x1,%edx
-   29a1b1520:	je     29a1b1570 <__dyn_tls_init+0x70>
+   29a1b14fd:	cmp    $0x1,%edx
+   29a1b1500:	je     29a1b1550 <__dyn_tls_init+0x70>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:102
-   29a1b1522:	mov    $0x1,%eax
-   29a1b1527:	add    $0x28,%rsp
-   29a1b152b:	pop    %rbx
-   29a1b152c:	pop    %rsi
-   29a1b152d:	ret
-   29a1b152e:	xchg   %ax,%ax
+   29a1b1502:	mov    $0x1,%eax
+   29a1b1507:	add    $0x28,%rsp
+   29a1b150b:	pop    %rbx
+   29a1b150c:	pop    %rsi
+   29a1b150d:	ret
+   29a1b150e:	xchg   %ax,%ax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:94
-   29a1b1530:	lea    0x8b19(%rip),%rbx        # 29a1ba050 <__xd_z>
+   29a1b1510:	lea    0x8b39(%rip),%rbx        # 29a1ba050 <__xd_z>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:95
-   29a1b1537:	lea    0x8b12(%rip),%rsi        # 29a1ba050 <__xd_z>
-   29a1b153e:	cmp    %rsi,%rbx
-   29a1b1541:	je     29a1b1522 <__dyn_tls_init+0x22>
-   29a1b1543:	nopl   0x0(%rax,%rax,1)
+   29a1b1517:	lea    0x8b32(%rip),%rsi        # 29a1ba050 <__xd_z>
+   29a1b151e:	cmp    %rsi,%rbx
+   29a1b1521:	je     29a1b1502 <__dyn_tls_init+0x22>
+   29a1b1523:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:98
-   29a1b1548:	mov    (%rbx),%rax
-   29a1b154b:	test   %rax,%rax
-   29a1b154e:	je     29a1b1552 <__dyn_tls_init+0x52>
+   29a1b1528:	mov    (%rbx),%rax
+   29a1b152b:	test   %rax,%rax
+   29a1b152e:	je     29a1b1532 <__dyn_tls_init+0x52>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:99
-   29a1b1550:	call   *%rax
+   29a1b1530:	call   *%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:95
-   29a1b1552:	add    $0x8,%rbx
-   29a1b1556:	cmp    %rsi,%rbx
-   29a1b1559:	jne    29a1b1548 <__dyn_tls_init+0x48>
+   29a1b1532:	add    $0x8,%rbx
+   29a1b1536:	cmp    %rsi,%rbx
+   29a1b1539:	jne    29a1b1528 <__dyn_tls_init+0x48>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:102
-   29a1b155b:	mov    $0x1,%eax
-   29a1b1560:	add    $0x28,%rsp
-   29a1b1564:	pop    %rbx
-   29a1b1565:	pop    %rsi
-   29a1b1566:	ret
-   29a1b1567:	nopw   0x0(%rax,%rax,1)
+   29a1b153b:	mov    $0x1,%eax
+   29a1b1540:	add    $0x28,%rsp
+   29a1b1544:	pop    %rbx
+   29a1b1545:	pop    %rsi
+   29a1b1546:	ret
+   29a1b1547:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:89
-   29a1b1570:	call   29a1b1c50 <__mingw_TLScallback>
+   29a1b1550:	call   29a1b1c30 <__mingw_TLScallback>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:102
-   29a1b1575:	mov    $0x1,%eax
-   29a1b157a:	add    $0x28,%rsp
-   29a1b157e:	pop    %rbx
-   29a1b157f:	pop    %rsi
-   29a1b1580:	ret
-   29a1b1581:	data16 cs nopw 0x0(%rax,%rax,1)
-   29a1b158c:	nopl   0x0(%rax)
+   29a1b1555:	mov    $0x1,%eax
+   29a1b155a:	add    $0x28,%rsp
+   29a1b155e:	pop    %rbx
+   29a1b155f:	pop    %rsi
+   29a1b1560:	ret
+   29a1b1561:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b156c:	nopl   0x0(%rax)
 
-000000029a1b1590 <__tlregdtor>:
+000000029a1b1570 <__tlregdtor>:
 __tlregdtor():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:134
-   29a1b1590:	xor    %eax,%eax
-   29a1b1592:	ret
-   29a1b1593:	nop
-   29a1b1594:	nop
-   29a1b1595:	nop
-   29a1b1596:	nop
-   29a1b1597:	nop
-   29a1b1598:	nop
-   29a1b1599:	nop
-   29a1b159a:	nop
-   29a1b159b:	nop
-   29a1b159c:	nop
-   29a1b159d:	nop
-   29a1b159e:	nop
-   29a1b159f:	nop
+   29a1b1570:	xor    %eax,%eax
+   29a1b1572:	ret
+   29a1b1573:	nop
+   29a1b1574:	nop
+   29a1b1575:	nop
+   29a1b1576:	nop
+   29a1b1577:	nop
+   29a1b1578:	nop
+   29a1b1579:	nop
+   29a1b157a:	nop
+   29a1b157b:	nop
+   29a1b157c:	nop
+   29a1b157d:	nop
+   29a1b157e:	nop
+   29a1b157f:	nop
 
-000000029a1b15a0 <__report_error>:
+000000029a1b1580 <__report_error>:
 __report_error():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:85
-   29a1b15a0:	push   %rsi
-   29a1b15a1:	push   %rbx
-   29a1b15a2:	sub    $0x38,%rsp
-   29a1b15a6:	mov    %rcx,%rbx
+   29a1b1580:	push   %rsi
+   29a1b1581:	push   %rbx
+   29a1b1582:	sub    $0x38,%rsp
+   29a1b1586:	mov    %rcx,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:148
-   29a1b15a9:	lea    0x58(%rsp),%rax
+   29a1b1589:	lea    0x58(%rsp),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:150
-   29a1b15ae:	mov    $0x2,%ecx
+   29a1b158e:	mov    $0x2,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:85
-   29a1b15b3:	mov    %rdx,0x58(%rsp)
-   29a1b15b8:	mov    %r8,0x60(%rsp)
-   29a1b15bd:	mov    %r9,0x68(%rsp)
+   29a1b1593:	mov    %rdx,0x58(%rsp)
+   29a1b1598:	mov    %r8,0x60(%rsp)
+   29a1b159d:	mov    %r9,0x68(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:148
-   29a1b15c2:	mov    %rax,0x28(%rsp)
+   29a1b15a2:	mov    %rax,0x28(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:150
-   29a1b15c7:	call   29a1b2430 <__acrt_iob_func>
-   29a1b15cc:	mov    $0x1b,%r8d
-   29a1b15d2:	mov    $0x1,%edx
-   29a1b15d7:	lea    0x2a82(%rip),%rcx        # 29a1b4060 <.rdata>
-   29a1b15de:	mov    %rax,%r9
-   29a1b15e1:	call   29a1b2458 <fwrite>
+   29a1b15a7:	call   29a1b2410 <__acrt_iob_func>
+   29a1b15ac:	mov    $0x1b,%r8d
+   29a1b15b2:	mov    $0x1,%edx
+   29a1b15b7:	lea    0x2aa2(%rip),%rcx        # 29a1b4060 <.rdata>
+   29a1b15be:	mov    %rax,%r9
+   29a1b15c1:	call   29a1b2430 <fwrite>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:151
-   29a1b15e6:	mov    0x28(%rsp),%rsi
-   29a1b15eb:	mov    $0x2,%ecx
-   29a1b15f0:	call   29a1b2430 <__acrt_iob_func>
-   29a1b15f5:	mov    %rbx,%rdx
-   29a1b15f8:	mov    %rax,%rcx
-   29a1b15fb:	mov    %rsi,%r8
-   29a1b15fe:	call   29a1b21c0 <vfprintf>
+   29a1b15c6:	mov    0x28(%rsp),%rsi
+   29a1b15cb:	mov    $0x2,%ecx
+   29a1b15d0:	call   29a1b2410 <__acrt_iob_func>
+   29a1b15d5:	mov    %rbx,%rdx
+   29a1b15d8:	mov    %rax,%rcx
+   29a1b15db:	mov    %rsi,%r8
+   29a1b15de:	call   29a1b21a0 <vfprintf>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:157
-   29a1b1603:	call   29a1b24e0 <abort>
-   29a1b1608:	nop
-   29a1b1609:	nopl   0x0(%rax)
+   29a1b15e3:	call   29a1b24b0 <abort>
+   29a1b15e8:	nop
+   29a1b15e9:	nopl   0x0(%rax)
 
-000000029a1b1610 <mark_section_writable>:
+000000029a1b15f0 <mark_section_writable>:
 mark_section_writable():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:184
-   29a1b1610:	push   %rdi
-   29a1b1611:	push   %rsi
-   29a1b1612:	push   %rbx
-   29a1b1613:	sub    $0x50,%rsp
+   29a1b15f0:	push   %rdi
+   29a1b15f1:	push   %rsi
+   29a1b15f2:	push   %rbx
+   29a1b15f3:	sub    $0x50,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:189
-   29a1b1617:	movslq 0x5a46(%rip),%rsi        # 29a1b7064 <maxSections>
+   29a1b15f7:	movslq 0x5a66(%rip),%rsi        # 29a1b7064 <maxSections>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:184
-   29a1b161e:	mov    %rcx,%rbx
+   29a1b15fe:	mov    %rcx,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:189
-   29a1b1621:	test   %esi,%esi
-   29a1b1623:	jle    29a1b1740 <mark_section_writable+0x130>
-   29a1b1629:	mov    0x5a38(%rip),%rax        # 29a1b7068 <the_secs>
-   29a1b1630:	xor    %r9d,%r9d
-   29a1b1633:	add    $0x18,%rax
-   29a1b1637:	nopw   0x0(%rax,%rax,1)
+   29a1b1601:	test   %esi,%esi
+   29a1b1603:	jle    29a1b1720 <mark_section_writable+0x130>
+   29a1b1609:	mov    0x5a58(%rip),%rax        # 29a1b7068 <the_secs>
+   29a1b1610:	xor    %r9d,%r9d
+   29a1b1613:	add    $0x18,%rax
+   29a1b1617:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:191
-   29a1b1640:	mov    (%rax),%r8
-   29a1b1643:	cmp    %r8,%rbx
-   29a1b1646:	jb     29a1b165b <mark_section_writable+0x4b>
+   29a1b1620:	mov    (%rax),%r8
+   29a1b1623:	cmp    %r8,%rbx
+   29a1b1626:	jb     29a1b163b <mark_section_writable+0x4b>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:192
-   29a1b1648:	mov    0x8(%rax),%rdx
-   29a1b164c:	mov    0x8(%rdx),%edx
-   29a1b164f:	add    %rdx,%r8
-   29a1b1652:	cmp    %r8,%rbx
-   29a1b1655:	jb     29a1b16e5 <mark_section_writable+0xd5>
+   29a1b1628:	mov    0x8(%rax),%rdx
+   29a1b162c:	mov    0x8(%rdx),%edx
+   29a1b162f:	add    %rdx,%r8
+   29a1b1632:	cmp    %r8,%rbx
+   29a1b1635:	jb     29a1b16c5 <mark_section_writable+0xd5>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:189
-   29a1b165b:	add    $0x1,%r9d
-   29a1b165f:	add    $0x28,%rax
-   29a1b1663:	cmp    %esi,%r9d
-   29a1b1666:	jne    29a1b1640 <mark_section_writable+0x30>
+   29a1b163b:	add    $0x1,%r9d
+   29a1b163f:	add    $0x28,%rax
+   29a1b1643:	cmp    %esi,%r9d
+   29a1b1646:	jne    29a1b1620 <mark_section_writable+0x30>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:195
-   29a1b1668:	mov    %rbx,%rcx
-   29a1b166b:	call   29a1b1e70 <__mingw_GetSectionForAddress>
-   29a1b1670:	mov    %rax,%rdi
+   29a1b1648:	mov    %rbx,%rcx
+   29a1b164b:	call   29a1b1e50 <__mingw_GetSectionForAddress>
+   29a1b1650:	mov    %rax,%rdi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:196
-   29a1b1673:	test   %rax,%rax
-   29a1b1676:	je     29a1b1762 <mark_section_writable+0x152>
+   29a1b1653:	test   %rax,%rax
+   29a1b1656:	je     29a1b1742 <mark_section_writable+0x152>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:201
-   29a1b167c:	mov    0x59e5(%rip),%rax        # 29a1b7068 <the_secs>
-   29a1b1683:	lea    (%rsi,%rsi,4),%rbx
-   29a1b1687:	shl    $0x3,%rbx
-   29a1b168b:	add    %rbx,%rax
-   29a1b168e:	mov    %rdi,0x20(%rax)
+   29a1b165c:	mov    0x5a05(%rip),%rax        # 29a1b7068 <the_secs>
+   29a1b1663:	lea    (%rsi,%rsi,4),%rbx
+   29a1b1667:	shl    $0x3,%rbx
+   29a1b166b:	add    %rbx,%rax
+   29a1b166e:	mov    %rdi,0x20(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:202
-   29a1b1692:	movl   $0x0,(%rax)
+   29a1b1672:	movl   $0x0,(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:203
-   29a1b1698:	call   29a1b1fb0 <_GetPEImageBase>
-   29a1b169d:	mov    0xc(%rdi),%edx
+   29a1b1678:	call   29a1b1f90 <_GetPEImageBase>
+   29a1b167d:	mov    0xc(%rdi),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:205
-   29a1b16a0:	mov    $0x30,%r8d
+   29a1b1680:	mov    $0x30,%r8d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:203
-   29a1b16a6:	lea    (%rax,%rdx,1),%rcx
-   29a1b16aa:	mov    0x59b7(%rip),%rax        # 29a1b7068 <the_secs>
+   29a1b1686:	lea    (%rax,%rdx,1),%rcx
+   29a1b168a:	mov    0x59d7(%rip),%rax        # 29a1b7068 <the_secs>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:205
-   29a1b16b1:	lea    0x20(%rsp),%rdx
+   29a1b1691:	lea    0x20(%rsp),%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:203
-   29a1b16b6:	mov    %rcx,0x18(%rax,%rbx,1)
+   29a1b1696:	mov    %rcx,0x18(%rax,%rbx,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:205
-   29a1b16bb:	call   *0x7bcf(%rip)        # 29a1b9290 <__imp_VirtualQuery>
-   29a1b16c1:	test   %rax,%rax
-   29a1b16c4:	je     29a1b1747 <mark_section_writable+0x137>
+   29a1b169b:	call   *0x7be7(%rip)        # 29a1b9288 <__imp_VirtualQuery>
+   29a1b16a1:	test   %rax,%rax
+   29a1b16a4:	je     29a1b1727 <mark_section_writable+0x137>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:212
-   29a1b16ca:	mov    0x44(%rsp),%eax
-   29a1b16ce:	lea    -0x4(%rax),%edx
+   29a1b16aa:	mov    0x44(%rsp),%eax
+   29a1b16ae:	lea    -0x4(%rax),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:213
-   29a1b16d1:	and    $0xfffffffb,%edx
-   29a1b16d4:	je     29a1b16de <mark_section_writable+0xce>
+   29a1b16b1:	and    $0xfffffffb,%edx
+   29a1b16b4:	je     29a1b16be <mark_section_writable+0xce>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:212
-   29a1b16d6:	lea    -0x40(%rax),%edx
+   29a1b16b6:	lea    -0x40(%rax),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:213
-   29a1b16d9:	and    $0xffffffbf,%edx
-   29a1b16dc:	jne    29a1b16f0 <mark_section_writable+0xe0>
+   29a1b16b9:	and    $0xffffffbf,%edx
+   29a1b16bc:	jne    29a1b16d0 <mark_section_writable+0xe0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:228
-   29a1b16de:	addl   $0x1,0x597f(%rip)        # 29a1b7064 <maxSections>
+   29a1b16be:	addl   $0x1,0x599f(%rip)        # 29a1b7064 <maxSections>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:230
-   29a1b16e5:	add    $0x50,%rsp
-   29a1b16e9:	pop    %rbx
-   29a1b16ea:	pop    %rsi
-   29a1b16eb:	pop    %rdi
-   29a1b16ec:	ret
-   29a1b16ed:	nopl   (%rax)
+   29a1b16c5:	add    $0x50,%rsp
+   29a1b16c9:	pop    %rbx
+   29a1b16ca:	pop    %rsi
+   29a1b16cb:	pop    %rdi
+   29a1b16cc:	ret
+   29a1b16cd:	nopl   (%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:217
-   29a1b16f0:	cmp    $0x2,%eax
+   29a1b16d0:	cmp    $0x2,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:220
-   29a1b16f3:	mov    0x20(%rsp),%rcx
+   29a1b16d3:	mov    0x20(%rsp),%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:221
-   29a1b16f8:	mov    0x38(%rsp),%rdx
+   29a1b16d8:	mov    0x38(%rsp),%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:217
-   29a1b16fd:	mov    $0x40,%r8d
-   29a1b1703:	mov    $0x4,%eax
-   29a1b1708:	cmove  %eax,%r8d
+   29a1b16dd:	mov    $0x40,%r8d
+   29a1b16e3:	mov    $0x4,%eax
+   29a1b16e8:	cmove  %eax,%r8d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:220
-   29a1b170c:	add    0x5955(%rip),%rbx        # 29a1b7068 <the_secs>
-   29a1b1713:	mov    %rcx,0x8(%rbx)
-   29a1b1717:	mov    %rbx,%r9
+   29a1b16ec:	add    0x5975(%rip),%rbx        # 29a1b7068 <the_secs>
+   29a1b16f3:	mov    %rcx,0x8(%rbx)
+   29a1b16f7:	mov    %rbx,%r9
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:221
-   29a1b171a:	mov    %rdx,0x10(%rbx)
+   29a1b16fa:	mov    %rdx,0x10(%rbx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:222
-   29a1b171e:	call   *0x7b64(%rip)        # 29a1b9288 <__imp_VirtualProtect>
-   29a1b1724:	test   %eax,%eax
-   29a1b1726:	jne    29a1b16de <mark_section_writable+0xce>
+   29a1b16fe:	call   *0x7b7c(%rip)        # 29a1b9280 <__imp_VirtualProtect>
+   29a1b1704:	test   %eax,%eax
+   29a1b1706:	jne    29a1b16be <mark_section_writable+0xce>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:226
-   29a1b1728:	call   *0x7b32(%rip)        # 29a1b9260 <__imp_GetLastError>
+   29a1b1708:	call   *0x7b4a(%rip)        # 29a1b9258 <__imp_GetLastError>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:225
-   29a1b172e:	lea    0x29a3(%rip),%rcx        # 29a1b40d8 <.rdata+0x78>
+   29a1b170e:	lea    0x29c3(%rip),%rcx        # 29a1b40d8 <.rdata+0x78>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:226
-   29a1b1735:	mov    %eax,%edx
+   29a1b1715:	mov    %eax,%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:225
-   29a1b1737:	call   29a1b15a0 <__report_error>
-   29a1b173c:	nopl   0x0(%rax)
+   29a1b1717:	call   29a1b1580 <__report_error>
+   29a1b171c:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:189
-   29a1b1740:	xor    %esi,%esi
-   29a1b1742:	jmp    29a1b1668 <mark_section_writable+0x58>
+   29a1b1720:	xor    %esi,%esi
+   29a1b1722:	jmp    29a1b1648 <mark_section_writable+0x58>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:207
-   29a1b1747:	mov    0x591a(%rip),%rax        # 29a1b7068 <the_secs>
-   29a1b174e:	mov    0x8(%rdi),%edx
-   29a1b1751:	lea    0x2948(%rip),%rcx        # 29a1b40a0 <.rdata+0x40>
-   29a1b1758:	mov    0x18(%rax,%rbx,1),%r8
-   29a1b175d:	call   29a1b15a0 <__report_error>
+   29a1b1727:	mov    0x593a(%rip),%rax        # 29a1b7068 <the_secs>
+   29a1b172e:	mov    0x8(%rdi),%edx
+   29a1b1731:	lea    0x2968(%rip),%rcx        # 29a1b40a0 <.rdata+0x40>
+   29a1b1738:	mov    0x18(%rax,%rbx,1),%r8
+   29a1b173d:	call   29a1b1580 <__report_error>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:198
-   29a1b1762:	mov    %rbx,%rdx
-   29a1b1765:	lea    0x2914(%rip),%rcx        # 29a1b4080 <.rdata+0x20>
-   29a1b176c:	call   29a1b15a0 <__report_error>
-   29a1b1771:	nop
-   29a1b1772:	data16 cs nopw 0x0(%rax,%rax,1)
-   29a1b177d:	nopl   (%rax)
+   29a1b1742:	mov    %rbx,%rdx
+   29a1b1745:	lea    0x2934(%rip),%rcx        # 29a1b4080 <.rdata+0x20>
+   29a1b174c:	call   29a1b1580 <__report_error>
+   29a1b1751:	nop
+   29a1b1752:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b175d:	nopl   (%rax)
 
-000000029a1b1780 <_pei386_runtime_relocator>:
+000000029a1b1760 <_pei386_runtime_relocator>:
 _pei386_runtime_relocator():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:486
-   29a1b1780:	push   %rbp
-   29a1b1781:	push   %r15
-   29a1b1783:	push   %r14
-   29a1b1785:	push   %r13
-   29a1b1787:	push   %r12
-   29a1b1789:	push   %rdi
-   29a1b178a:	push   %rsi
-   29a1b178b:	push   %rbx
-   29a1b178c:	sub    $0x48,%rsp
-   29a1b1790:	lea    0x40(%rsp),%rbp
+   29a1b1760:	push   %rbp
+   29a1b1761:	push   %r15
+   29a1b1763:	push   %r14
+   29a1b1765:	push   %r13
+   29a1b1767:	push   %r12
+   29a1b1769:	push   %rdi
+   29a1b176a:	push   %rsi
+   29a1b176b:	push   %rbx
+   29a1b176c:	sub    $0x48,%rsp
+   29a1b1770:	lea    0x40(%rsp),%rbp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:492
-   29a1b1795:	mov    0x58c4(%rip),%r12d        # 29a1b7060 <was_init.0>
-   29a1b179c:	test   %r12d,%r12d
-   29a1b179f:	je     29a1b17b8 <_pei386_runtime_relocator+0x38>
+   29a1b1775:	mov    0x58e4(%rip),%r12d        # 29a1b7060 <was_init.0>
+   29a1b177c:	test   %r12d,%r12d
+   29a1b177f:	je     29a1b1798 <_pei386_runtime_relocator+0x38>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:508
-   29a1b17a1:	lea    0x8(%rbp),%rsp
-   29a1b17a5:	pop    %rbx
-   29a1b17a6:	pop    %rsi
-   29a1b17a7:	pop    %rdi
-   29a1b17a8:	pop    %r12
-   29a1b17aa:	pop    %r13
-   29a1b17ac:	pop    %r14
-   29a1b17ae:	pop    %r15
-   29a1b17b0:	pop    %rbp
-   29a1b17b1:	ret
-   29a1b17b2:	nopw   0x0(%rax,%rax,1)
+   29a1b1781:	lea    0x8(%rbp),%rsp
+   29a1b1785:	pop    %rbx
+   29a1b1786:	pop    %rsi
+   29a1b1787:	pop    %rdi
+   29a1b1788:	pop    %r12
+   29a1b178a:	pop    %r13
+   29a1b178c:	pop    %r14
+   29a1b178e:	pop    %r15
+   29a1b1790:	pop    %rbp
+   29a1b1791:	ret
+   29a1b1792:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:494
-   29a1b17b8:	movl   $0x1,0x589e(%rip)        # 29a1b7060 <was_init.0>
+   29a1b1798:	movl   $0x1,0x58be(%rip)        # 29a1b7060 <was_init.0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:496
-   29a1b17c2:	call   29a1b1ef0 <__mingw_GetSectionCount>
+   29a1b17a2:	call   29a1b1ed0 <__mingw_GetSectionCount>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:497
-   29a1b17c7:	cltq
-   29a1b17c9:	lea    (%rax,%rax,4),%rax
-   29a1b17cd:	lea    0xf(,%rax,8),%rax
-   29a1b17d5:	and    $0xfffffffffffffff0,%rax
-   29a1b17d9:	call   29a1b2160 <___chkstk_ms>
+   29a1b17a7:	cltq
+   29a1b17a9:	lea    (%rax,%rax,4),%rax
+   29a1b17ad:	lea    0xf(,%rax,8),%rax
+   29a1b17b5:	and    $0xfffffffffffffff0,%rax
+   29a1b17b9:	call   29a1b2140 <___chkstk_ms>
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:312
-   29a1b17de:	mov    0x2a2b(%rip),%r13        # 29a1b4210 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
-   29a1b17e5:	mov    0x2a34(%rip),%rbx        # 29a1b4220 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
+   29a1b17be:	mov    0x2a4b(%rip),%r13        # 29a1b4210 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
+   29a1b17c5:	mov    0x2a54(%rip),%rbx        # 29a1b4220 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
 _pei386_runtime_relocator():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:498
-   29a1b17ec:	movl   $0x0,0x586e(%rip)        # 29a1b7064 <maxSections>
+   29a1b17cc:	movl   $0x0,0x588e(%rip)        # 29a1b7064 <maxSections>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:497
-   29a1b17f6:	sub    %rax,%rsp
-   29a1b17f9:	lea    0x30(%rsp),%rax
-   29a1b17fe:	mov    %rax,0x5863(%rip)        # 29a1b7068 <the_secs>
+   29a1b17d6:	sub    %rax,%rsp
+   29a1b17d9:	lea    0x30(%rsp),%rax
+   29a1b17de:	mov    %rax,0x5883(%rip)        # 29a1b7068 <the_secs>
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:312
-   29a1b1805:	mov    %r13,%rax
-   29a1b1808:	sub    %rbx,%rax
+   29a1b17e5:	mov    %r13,%rax
+   29a1b17e8:	sub    %rbx,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:321
-   29a1b180b:	cmp    $0x7,%rax
-   29a1b180f:	jle    29a1b17a1 <_pei386_runtime_relocator+0x21>
+   29a1b17eb:	cmp    $0x7,%rax
+   29a1b17ef:	jle    29a1b1781 <_pei386_runtime_relocator+0x21>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:344
-   29a1b1811:	mov    (%rbx),%edx
+   29a1b17f1:	mov    (%rbx),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:343
-   29a1b1813:	cmp    $0xb,%rax
-   29a1b1817:	jg     29a1b1920 <_pei386_runtime_relocator+0x1a0>
+   29a1b17f3:	cmp    $0xb,%rax
+   29a1b17f7:	jg     29a1b1900 <_pei386_runtime_relocator+0x1a0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:358
-   29a1b181d:	mov    (%rbx),%eax
-   29a1b181f:	test   %eax,%eax
-   29a1b1821:	jne    29a1b1a90 <_pei386_runtime_relocator+0x310>
-   29a1b1827:	mov    0x4(%rbx),%eax
-   29a1b182a:	test   %eax,%eax
-   29a1b182c:	jne    29a1b1a90 <_pei386_runtime_relocator+0x310>
+   29a1b17fd:	mov    (%rbx),%eax
+   29a1b17ff:	test   %eax,%eax
+   29a1b1801:	jne    29a1b1a70 <_pei386_runtime_relocator+0x310>
+   29a1b1807:	mov    0x4(%rbx),%eax
+   29a1b180a:	test   %eax,%eax
+   29a1b180c:	jne    29a1b1a70 <_pei386_runtime_relocator+0x310>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:379
-   29a1b1832:	mov    0x8(%rbx),%edx
-   29a1b1835:	cmp    $0x1,%edx
-   29a1b1838:	jne    29a1b1ad0 <_pei386_runtime_relocator+0x350>
+   29a1b1812:	mov    0x8(%rbx),%edx
+   29a1b1815:	cmp    $0x1,%edx
+   29a1b1818:	jne    29a1b1ab0 <_pei386_runtime_relocator+0x350>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:391
-   29a1b183e:	add    $0xc,%rbx
+   29a1b181e:	add    $0xc,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:393
-   29a1b1842:	cmp    %r13,%rbx
-   29a1b1845:	jae    29a1b17a1 <_pei386_runtime_relocator+0x21>
+   29a1b1822:	cmp    %r13,%rbx
+   29a1b1825:	jae    29a1b1781 <_pei386_runtime_relocator+0x21>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:396
-   29a1b184b:	mov    0x29ae(%rip),%r14        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b182b:	mov    0x29ce(%rip),%r14        # 29a1b4200 <.refptr.__ImageBase>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:456
-   29a1b1852:	mov    $0xffffffff,%r15d
-   29a1b1858:	jmp    29a1b18bf <_pei386_runtime_relocator+0x13f>
-   29a1b185a:	nopw   0x0(%rax,%rax,1)
+   29a1b1832:	mov    $0xffffffff,%r15d
+   29a1b1838:	jmp    29a1b189f <_pei386_runtime_relocator+0x13f>
+   29a1b183a:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:410
-   29a1b1860:	cmp    $0x8,%ecx
-   29a1b1863:	je     29a1b1940 <_pei386_runtime_relocator+0x1c0>
-   29a1b1869:	cmp    $0x10,%ecx
-   29a1b186c:	jne    29a1b1ac2 <_pei386_runtime_relocator+0x342>
+   29a1b1840:	cmp    $0x8,%ecx
+   29a1b1843:	je     29a1b1920 <_pei386_runtime_relocator+0x1c0>
+   29a1b1849:	cmp    $0x10,%ecx
+   29a1b184c:	jne    29a1b1aa2 <_pei386_runtime_relocator+0x342>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:418
-   29a1b1872:	movzwl (%rdi),%esi
+   29a1b1852:	movzwl (%rdi),%esi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:419
-   29a1b1875:	and    $0xc0,%edx
-   29a1b187b:	test   %si,%si
-   29a1b187e:	jns    29a1b1a50 <_pei386_runtime_relocator+0x2d0>
+   29a1b1855:	and    $0xc0,%edx
+   29a1b185b:	test   %si,%si
+   29a1b185e:	jns    29a1b1a30 <_pei386_runtime_relocator+0x2d0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:420
-   29a1b1884:	or     $0xffffffffffff0000,%rsi
+   29a1b1864:	or     $0xffffffffffff0000,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b188b:	sub    %rax,%rsi
+   29a1b186b:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b188e:	add    %r9,%rsi
+   29a1b186e:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b1891:	test   %edx,%edx
-   29a1b1893:	jne    29a1b18a7 <_pei386_runtime_relocator+0x127>
+   29a1b1871:	test   %edx,%edx
+   29a1b1873:	jne    29a1b1887 <_pei386_runtime_relocator+0x127>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:456
-   29a1b1895:	cmp    $0xffffffffffff8000,%rsi
-   29a1b189c:	jl     29a1b1903 <_pei386_runtime_relocator+0x183>
-   29a1b189e:	cmp    $0xffff,%rsi
-   29a1b18a5:	jg     29a1b1903 <_pei386_runtime_relocator+0x183>
+   29a1b1875:	cmp    $0xffffffffffff8000,%rsi
+   29a1b187c:	jl     29a1b18e3 <_pei386_runtime_relocator+0x183>
+   29a1b187e:	cmp    $0xffff,%rsi
+   29a1b1885:	jg     29a1b18e3 <_pei386_runtime_relocator+0x183>
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b18a7:	mov    %rdi,%rcx
-   29a1b18aa:	call   29a1b1610 <mark_section_writable>
+   29a1b1887:	mov    %rdi,%rcx
+   29a1b188a:	call   29a1b15f0 <mark_section_writable>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:294
-   29a1b18af:	mov    %si,(%rdi)
+   29a1b188f:	mov    %si,(%rdi)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:393
-   29a1b18b2:	add    $0xc,%rbx
-   29a1b18b6:	cmp    %r13,%rbx
-   29a1b18b9:	jae    29a1b1990 <_pei386_runtime_relocator+0x210>
+   29a1b1892:	add    $0xc,%rbx
+   29a1b1896:	cmp    %r13,%rbx
+   29a1b1899:	jae    29a1b1970 <_pei386_runtime_relocator+0x210>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:401
-   29a1b18bf:	mov    (%rbx),%eax
+   29a1b189f:	mov    (%rbx),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:410
-   29a1b18c1:	mov    0x8(%rbx),%edx
+   29a1b18a1:	mov    0x8(%rbx),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:396
-   29a1b18c4:	mov    0x4(%rbx),%edi
+   29a1b18a4:	mov    0x4(%rbx),%edi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:401
-   29a1b18c7:	add    %r14,%rax
+   29a1b18a7:	add    %r14,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:410
-   29a1b18ca:	movzbl %dl,%ecx
+   29a1b18aa:	movzbl %dl,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:402
-   29a1b18cd:	mov    (%rax),%r9
+   29a1b18ad:	mov    (%rax),%r9
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:396
-   29a1b18d0:	add    %r14,%rdi
+   29a1b18b0:	add    %r14,%rdi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:410
-   29a1b18d3:	cmp    $0x20,%ecx
-   29a1b18d6:	je     29a1b19e8 <_pei386_runtime_relocator+0x268>
-   29a1b18dc:	jbe    29a1b1860 <_pei386_runtime_relocator+0xe0>
-   29a1b18de:	cmp    $0x40,%ecx
-   29a1b18e1:	jne    29a1b1ac2 <_pei386_runtime_relocator+0x342>
+   29a1b18b3:	cmp    $0x20,%ecx
+   29a1b18b6:	je     29a1b19c8 <_pei386_runtime_relocator+0x268>
+   29a1b18bc:	jbe    29a1b1840 <_pei386_runtime_relocator+0xe0>
+   29a1b18be:	cmp    $0x40,%ecx
+   29a1b18c1:	jne    29a1b1aa2 <_pei386_runtime_relocator+0x342>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b18e7:	mov    (%rdi),%rsi
+   29a1b18c7:	mov    (%rdi),%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b18ea:	mov    %edx,%ecx
+   29a1b18ca:	mov    %edx,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b18ec:	sub    %rax,%rsi
+   29a1b18cc:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b18ef:	add    %r9,%rsi
+   29a1b18cf:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b18f2:	and    $0xc0,%ecx
-   29a1b18f8:	jne    29a1b1a40 <_pei386_runtime_relocator+0x2c0>
+   29a1b18d2:	and    $0xc0,%ecx
+   29a1b18d8:	jne    29a1b1a20 <_pei386_runtime_relocator+0x2c0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:456
-   29a1b18fe:	test   %rsi,%rsi
-   29a1b1901:	js     29a1b18b2 <_pei386_runtime_relocator+0x132>
+   29a1b18de:	test   %rsi,%rsi
+   29a1b18e1:	js     29a1b1892 <_pei386_runtime_relocator+0x132>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:457
-   29a1b1903:	mov    %rsi,0x20(%rsp)
-   29a1b1908:	mov    %ecx,%edx
-   29a1b190a:	mov    %rdi,%r8
-   29a1b190d:	lea    0x2854(%rip),%rcx        # 29a1b4168 <.rdata+0x108>
-   29a1b1914:	call   29a1b15a0 <__report_error>
-   29a1b1919:	nopl   0x0(%rax)
+   29a1b18e3:	mov    %rsi,0x20(%rsp)
+   29a1b18e8:	mov    %ecx,%edx
+   29a1b18ea:	mov    %rdi,%r8
+   29a1b18ed:	lea    0x2874(%rip),%rcx        # 29a1b4168 <.rdata+0x108>
+   29a1b18f4:	call   29a1b1580 <__report_error>
+   29a1b18f9:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:344
-   29a1b1920:	test   %edx,%edx
-   29a1b1922:	jne    29a1b1a90 <_pei386_runtime_relocator+0x310>
-   29a1b1928:	mov    0x4(%rbx),%eax
+   29a1b1900:	test   %edx,%edx
+   29a1b1902:	jne    29a1b1a70 <_pei386_runtime_relocator+0x310>
+   29a1b1908:	mov    0x4(%rbx),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:345
-   29a1b192b:	mov    %eax,%edx
-   29a1b192d:	or     0x8(%rbx),%edx
-   29a1b1930:	jne    29a1b182a <_pei386_runtime_relocator+0xaa>
+   29a1b190b:	mov    %eax,%edx
+   29a1b190d:	or     0x8(%rbx),%edx
+   29a1b1910:	jne    29a1b180a <_pei386_runtime_relocator+0xaa>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:355
-   29a1b1936:	add    $0xc,%rbx
-   29a1b193a:	jmp    29a1b181d <_pei386_runtime_relocator+0x9d>
-   29a1b193f:	nop
+   29a1b1916:	add    $0xc,%rbx
+   29a1b191a:	jmp    29a1b17fd <_pei386_runtime_relocator+0x9d>
+   29a1b191f:	nop
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:413
-   29a1b1940:	movzbl (%rdi),%esi
+   29a1b1920:	movzbl (%rdi),%esi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:414
-   29a1b1943:	and    $0xc0,%edx
-   29a1b1949:	test   %sil,%sil
-   29a1b194c:	jns    29a1b1a78 <_pei386_runtime_relocator+0x2f8>
+   29a1b1923:	and    $0xc0,%edx
+   29a1b1929:	test   %sil,%sil
+   29a1b192c:	jns    29a1b1a58 <_pei386_runtime_relocator+0x2f8>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:415
-   29a1b1952:	or     $0xffffffffffffff00,%rsi
+   29a1b1932:	or     $0xffffffffffffff00,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b1959:	sub    %rax,%rsi
+   29a1b1939:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b195c:	add    %r9,%rsi
+   29a1b193c:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b195f:	test   %edx,%edx
-   29a1b1961:	jne    29a1b1972 <_pei386_runtime_relocator+0x1f2>
+   29a1b193f:	test   %edx,%edx
+   29a1b1941:	jne    29a1b1952 <_pei386_runtime_relocator+0x1f2>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:456
-   29a1b1963:	cmp    $0xff,%rsi
-   29a1b196a:	jg     29a1b1903 <_pei386_runtime_relocator+0x183>
-   29a1b196c:	cmp    $0xffffffffffffff80,%rsi
-   29a1b1970:	jl     29a1b1903 <_pei386_runtime_relocator+0x183>
+   29a1b1943:	cmp    $0xff,%rsi
+   29a1b194a:	jg     29a1b18e3 <_pei386_runtime_relocator+0x183>
+   29a1b194c:	cmp    $0xffffffffffffff80,%rsi
+   29a1b1950:	jl     29a1b18e3 <_pei386_runtime_relocator+0x183>
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b1972:	mov    %rdi,%rcx
+   29a1b1952:	mov    %rdi,%rcx
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:393
-   29a1b1975:	add    $0xc,%rbx
+   29a1b1955:	add    $0xc,%rbx
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b1979:	call   29a1b1610 <mark_section_writable>
+   29a1b1959:	call   29a1b15f0 <mark_section_writable>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:294
-   29a1b197e:	mov    %sil,(%rdi)
+   29a1b195e:	mov    %sil,(%rdi)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:393
-   29a1b1981:	cmp    %r13,%rbx
-   29a1b1984:	jb     29a1b18bf <_pei386_runtime_relocator+0x13f>
-   29a1b198a:	nopw   0x0(%rax,%rax,1)
+   29a1b1961:	cmp    %r13,%rbx
+   29a1b1964:	jb     29a1b189f <_pei386_runtime_relocator+0x13f>
+   29a1b196a:	nopw   0x0(%rax,%rax,1)
 restore_modified_sections():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:238
-   29a1b1990:	mov    0x56ce(%rip),%edx        # 29a1b7064 <maxSections>
-   29a1b1996:	test   %edx,%edx
-   29a1b1998:	jle    29a1b17a1 <_pei386_runtime_relocator+0x21>
+   29a1b1970:	mov    0x56ee(%rip),%edx        # 29a1b7064 <maxSections>
+   29a1b1976:	test   %edx,%edx
+   29a1b1978:	jle    29a1b1781 <_pei386_runtime_relocator+0x21>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:242
-   29a1b199e:	mov    0x78e3(%rip),%rsi        # 29a1b9288 <__imp_VirtualProtect>
+   29a1b197e:	mov    0x78fb(%rip),%rsi        # 29a1b9280 <__imp_VirtualProtect>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:238
-   29a1b19a5:	xor    %ebx,%ebx
+   29a1b1985:	xor    %ebx,%ebx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:242
-   29a1b19a7:	lea    -0x4(%rbp),%rdi
-   29a1b19ab:	nopl   0x0(%rax,%rax,1)
+   29a1b1987:	lea    -0x4(%rbp),%rdi
+   29a1b198b:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:240
-   29a1b19b0:	mov    0x56b1(%rip),%rax        # 29a1b7068 <the_secs>
-   29a1b19b7:	add    %rbx,%rax
-   29a1b19ba:	mov    (%rax),%r8d
-   29a1b19bd:	test   %r8d,%r8d
-   29a1b19c0:	je     29a1b19cf <_pei386_runtime_relocator+0x24f>
+   29a1b1990:	mov    0x56d1(%rip),%rax        # 29a1b7068 <the_secs>
+   29a1b1997:	add    %rbx,%rax
+   29a1b199a:	mov    (%rax),%r8d
+   29a1b199d:	test   %r8d,%r8d
+   29a1b19a0:	je     29a1b19af <_pei386_runtime_relocator+0x24f>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:242
-   29a1b19c2:	mov    0x10(%rax),%rdx
-   29a1b19c6:	mov    0x8(%rax),%rcx
-   29a1b19ca:	mov    %rdi,%r9
-   29a1b19cd:	call   *%rsi
+   29a1b19a2:	mov    0x10(%rax),%rdx
+   29a1b19a6:	mov    0x8(%rax),%rcx
+   29a1b19aa:	mov    %rdi,%r9
+   29a1b19ad:	call   *%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:238
-   29a1b19cf:	add    $0x1,%r12d
-   29a1b19d3:	add    $0x28,%rbx
-   29a1b19d7:	cmp    0x5686(%rip),%r12d        # 29a1b7064 <maxSections>
-   29a1b19de:	jl     29a1b19b0 <_pei386_runtime_relocator+0x230>
-   29a1b19e0:	jmp    29a1b17a1 <_pei386_runtime_relocator+0x21>
-   29a1b19e5:	nopl   (%rax)
+   29a1b19af:	add    $0x1,%r12d
+   29a1b19b3:	add    $0x28,%rbx
+   29a1b19b7:	cmp    0x56a6(%rip),%r12d        # 29a1b7064 <maxSections>
+   29a1b19be:	jl     29a1b1990 <_pei386_runtime_relocator+0x230>
+   29a1b19c0:	jmp    29a1b1781 <_pei386_runtime_relocator+0x21>
+   29a1b19c5:	nopl   (%rax)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:423
-   29a1b19e8:	mov    (%rdi),%esi
+   29a1b19c8:	mov    (%rdi),%esi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:425
-   29a1b19ea:	and    $0xc0,%edx
-   29a1b19f0:	test   %esi,%esi
-   29a1b19f2:	jns    29a1b1a68 <_pei386_runtime_relocator+0x2e8>
+   29a1b19ca:	and    $0xc0,%edx
+   29a1b19d0:	test   %esi,%esi
+   29a1b19d2:	jns    29a1b1a48 <_pei386_runtime_relocator+0x2e8>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:426
-   29a1b19f4:	movabs $0xffffffff00000000,%r11
-   29a1b19fe:	or     %r11,%rsi
+   29a1b19d4:	movabs $0xffffffff00000000,%r11
+   29a1b19de:	or     %r11,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b1a01:	sub    %rax,%rsi
+   29a1b19e1:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b1a04:	add    %r9,%rsi
+   29a1b19e4:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b1a07:	test   %edx,%edx
-   29a1b1a09:	jne    29a1b1a27 <_pei386_runtime_relocator+0x2a7>
+   29a1b19e7:	test   %edx,%edx
+   29a1b19e9:	jne    29a1b1a07 <_pei386_runtime_relocator+0x2a7>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:456
-   29a1b1a0b:	cmp    %r15,%rsi
-   29a1b1a0e:	jg     29a1b1903 <_pei386_runtime_relocator+0x183>
-   29a1b1a14:	movabs $0xffffffff7fffffff,%rax
-   29a1b1a1e:	cmp    %rax,%rsi
-   29a1b1a21:	jle    29a1b1903 <_pei386_runtime_relocator+0x183>
+   29a1b19eb:	cmp    %r15,%rsi
+   29a1b19ee:	jg     29a1b18e3 <_pei386_runtime_relocator+0x183>
+   29a1b19f4:	movabs $0xffffffff7fffffff,%rax
+   29a1b19fe:	cmp    %rax,%rsi
+   29a1b1a01:	jle    29a1b18e3 <_pei386_runtime_relocator+0x183>
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b1a27:	mov    %rdi,%rcx
-   29a1b1a2a:	call   29a1b1610 <mark_section_writable>
+   29a1b1a07:	mov    %rdi,%rcx
+   29a1b1a0a:	call   29a1b15f0 <mark_section_writable>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:294
-   29a1b1a2f:	mov    %esi,(%rdi)
+   29a1b1a0f:	mov    %esi,(%rdi)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:473
-   29a1b1a31:	jmp    29a1b18b2 <_pei386_runtime_relocator+0x132>
-   29a1b1a36:	cs nopw 0x0(%rax,%rax,1)
+   29a1b1a11:	jmp    29a1b1892 <_pei386_runtime_relocator+0x132>
+   29a1b1a16:	cs nopw 0x0(%rax,%rax,1)
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b1a40:	mov    %rdi,%rcx
-   29a1b1a43:	call   29a1b1610 <mark_section_writable>
+   29a1b1a20:	mov    %rdi,%rcx
+   29a1b1a23:	call   29a1b15f0 <mark_section_writable>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:294
-   29a1b1a48:	mov    %rsi,(%rdi)
+   29a1b1a28:	mov    %rsi,(%rdi)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:477
-   29a1b1a4b:	jmp    29a1b18b2 <_pei386_runtime_relocator+0x132>
+   29a1b1a2b:	jmp    29a1b1892 <_pei386_runtime_relocator+0x132>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b1a50:	sub    %rax,%rsi
+   29a1b1a30:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b1a53:	add    %r9,%rsi
+   29a1b1a33:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b1a56:	test   %edx,%edx
-   29a1b1a58:	je     29a1b1895 <_pei386_runtime_relocator+0x115>
-   29a1b1a5e:	jmp    29a1b18a7 <_pei386_runtime_relocator+0x127>
-   29a1b1a63:	nopl   0x0(%rax,%rax,1)
+   29a1b1a36:	test   %edx,%edx
+   29a1b1a38:	je     29a1b1875 <_pei386_runtime_relocator+0x115>
+   29a1b1a3e:	jmp    29a1b1887 <_pei386_runtime_relocator+0x127>
+   29a1b1a43:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b1a68:	sub    %rax,%rsi
+   29a1b1a48:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b1a6b:	add    %r9,%rsi
+   29a1b1a4b:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b1a6e:	test   %edx,%edx
-   29a1b1a70:	je     29a1b1a0b <_pei386_runtime_relocator+0x28b>
-   29a1b1a72:	jmp    29a1b1a27 <_pei386_runtime_relocator+0x2a7>
-   29a1b1a74:	nopl   0x0(%rax)
+   29a1b1a4e:	test   %edx,%edx
+   29a1b1a50:	je     29a1b19eb <_pei386_runtime_relocator+0x28b>
+   29a1b1a52:	jmp    29a1b1a07 <_pei386_runtime_relocator+0x2a7>
+   29a1b1a54:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:442
-   29a1b1a78:	sub    %rax,%rsi
+   29a1b1a58:	sub    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:443
-   29a1b1a7b:	add    %r9,%rsi
+   29a1b1a5b:	add    %r9,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:446
-   29a1b1a7e:	test   %edx,%edx
-   29a1b1a80:	je     29a1b1963 <_pei386_runtime_relocator+0x1e3>
-   29a1b1a86:	jmp    29a1b1972 <_pei386_runtime_relocator+0x1f2>
-   29a1b1a8b:	nopl   0x0(%rax,%rax,1)
+   29a1b1a5e:	test   %edx,%edx
+   29a1b1a60:	je     29a1b1943 <_pei386_runtime_relocator+0x1e3>
+   29a1b1a66:	jmp    29a1b1952 <_pei386_runtime_relocator+0x1f2>
+   29a1b1a6b:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:365
-   29a1b1a90:	cmp    %r13,%rbx
-   29a1b1a93:	jae    29a1b17a1 <_pei386_runtime_relocator+0x21>
+   29a1b1a70:	cmp    %r13,%rbx
+   29a1b1a73:	jae    29a1b1781 <_pei386_runtime_relocator+0x21>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:396
-   29a1b1a99:	mov    0x2760(%rip),%r14        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1a79:	mov    0x2780(%rip),%r14        # 29a1b4200 <.refptr.__ImageBase>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:369
-   29a1b1aa0:	mov    0x4(%rbx),%esi
+   29a1b1a80:	mov    0x4(%rbx),%esi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:370
-   29a1b1aa3:	mov    (%rbx),%edi
+   29a1b1a83:	mov    (%rbx),%edi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:366
-   29a1b1aa5:	add    $0x8,%rbx
+   29a1b1a85:	add    $0x8,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:369
-   29a1b1aa9:	add    %r14,%rsi
+   29a1b1a89:	add    %r14,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:370
-   29a1b1aac:	add    (%rsi),%edi
+   29a1b1a8c:	add    (%rsi),%edi
 __write_memory():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:271
-   29a1b1aae:	mov    %rsi,%rcx
-   29a1b1ab1:	call   29a1b1610 <mark_section_writable>
+   29a1b1a8e:	mov    %rsi,%rcx
+   29a1b1a91:	call   29a1b15f0 <mark_section_writable>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:294
-   29a1b1ab6:	mov    %edi,(%rsi)
+   29a1b1a96:	mov    %edi,(%rsi)
 do_pseudo_reloc():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:365
-   29a1b1ab8:	cmp    %r13,%rbx
-   29a1b1abb:	jb     29a1b1aa0 <_pei386_runtime_relocator+0x320>
-   29a1b1abd:	jmp    29a1b1990 <_pei386_runtime_relocator+0x210>
+   29a1b1a98:	cmp    %r13,%rbx
+   29a1b1a9b:	jb     29a1b1a80 <_pei386_runtime_relocator+0x320>
+   29a1b1a9d:	jmp    29a1b1970 <_pei386_runtime_relocator+0x210>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:436
-   29a1b1ac2:	mov    %ecx,%edx
-   29a1b1ac4:	lea    0x266d(%rip),%rcx        # 29a1b4138 <.rdata+0xd8>
-   29a1b1acb:	call   29a1b15a0 <__report_error>
+   29a1b1aa2:	mov    %ecx,%edx
+   29a1b1aa4:	lea    0x268d(%rip),%rcx        # 29a1b4138 <.rdata+0xd8>
+   29a1b1aab:	call   29a1b1580 <__report_error>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pseudo-reloc.c:381
-   29a1b1ad0:	lea    0x2629(%rip),%rcx        # 29a1b4100 <.rdata+0xa0>
-   29a1b1ad7:	call   29a1b15a0 <__report_error>
-   29a1b1adc:	nop
-   29a1b1add:	nop
-   29a1b1ade:	nop
-   29a1b1adf:	nop
+   29a1b1ab0:	lea    0x2649(%rip),%rcx        # 29a1b4100 <.rdata+0xa0>
+   29a1b1ab7:	call   29a1b1580 <__report_error>
+   29a1b1abc:	nop
+   29a1b1abd:	nop
+   29a1b1abe:	nop
+   29a1b1abf:	nop
 
-000000029a1b1ae0 <__mingwthr_run_key_dtors.part.0>:
+000000029a1b1ac0 <__mingwthr_run_key_dtors.part.0>:
 __mingwthr_run_key_dtors():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:99
-   29a1b1ae0:	push   %r12
-   29a1b1ae2:	push   %rbp
-   29a1b1ae3:	push   %rdi
-   29a1b1ae4:	push   %rsi
-   29a1b1ae5:	push   %rbx
-   29a1b1ae6:	sub    $0x20,%rsp
+   29a1b1ac0:	push   %r12
+   29a1b1ac2:	push   %rbp
+   29a1b1ac3:	push   %rdi
+   29a1b1ac4:	push   %rsi
+   29a1b1ac5:	push   %rbx
+   29a1b1ac6:	sub    $0x20,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:105
-   29a1b1aea:	lea    0x55af(%rip),%r12        # 29a1b70a0 <__mingwthr_cs>
-   29a1b1af1:	mov    %r12,%rcx
-   29a1b1af4:	call   *0x775e(%rip)        # 29a1b9258 <__imp_EnterCriticalSection>
+   29a1b1aca:	lea    0x55cf(%rip),%r12        # 29a1b70a0 <__mingwthr_cs>
+   29a1b1ad1:	mov    %r12,%rcx
+   29a1b1ad4:	call   *0x7776(%rip)        # 29a1b9250 <__imp_EnterCriticalSection>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:107
-   29a1b1afa:	mov    0x557f(%rip),%rbx        # 29a1b7080 <key_dtor_list>
-   29a1b1b01:	test   %rbx,%rbx
-   29a1b1b04:	je     29a1b1b3c <__mingwthr_run_key_dtors.part.0+0x5c>
-   29a1b1b06:	mov    0x7773(%rip),%rbp        # 29a1b9280 <__imp_TlsGetValue>
-   29a1b1b0d:	mov    0x774c(%rip),%rdi        # 29a1b9260 <__imp_GetLastError>
-   29a1b1b14:	nopl   0x0(%rax)
+   29a1b1ada:	mov    0x559f(%rip),%rbx        # 29a1b7080 <key_dtor_list>
+   29a1b1ae1:	test   %rbx,%rbx
+   29a1b1ae4:	je     29a1b1b1c <__mingwthr_run_key_dtors.part.0+0x5c>
+   29a1b1ae6:	mov    0x778b(%rip),%rbp        # 29a1b9278 <__imp_TlsGetValue>
+   29a1b1aed:	mov    0x7764(%rip),%rdi        # 29a1b9258 <__imp_GetLastError>
+   29a1b1af4:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:109
-   29a1b1b18:	mov    (%rbx),%ecx
-   29a1b1b1a:	call   *%rbp
-   29a1b1b1c:	mov    %rax,%rsi
+   29a1b1af8:	mov    (%rbx),%ecx
+   29a1b1afa:	call   *%rbp
+   29a1b1afc:	mov    %rax,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:110
-   29a1b1b1f:	call   *%rdi
+   29a1b1aff:	call   *%rdi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:112
-   29a1b1b21:	test   %rsi,%rsi
-   29a1b1b24:	je     29a1b1b33 <__mingwthr_run_key_dtors.part.0+0x53>
-   29a1b1b26:	test   %eax,%eax
-   29a1b1b28:	jne    29a1b1b33 <__mingwthr_run_key_dtors.part.0+0x53>
+   29a1b1b01:	test   %rsi,%rsi
+   29a1b1b04:	je     29a1b1b13 <__mingwthr_run_key_dtors.part.0+0x53>
+   29a1b1b06:	test   %eax,%eax
+   29a1b1b08:	jne    29a1b1b13 <__mingwthr_run_key_dtors.part.0+0x53>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:113
-   29a1b1b2a:	mov    0x8(%rbx),%rax
-   29a1b1b2e:	mov    %rsi,%rcx
-   29a1b1b31:	call   *%rax
+   29a1b1b0a:	mov    0x8(%rbx),%rax
+   29a1b1b0e:	mov    %rsi,%rcx
+   29a1b1b11:	call   *%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:115
-   29a1b1b33:	mov    0x10(%rbx),%rbx
+   29a1b1b13:	mov    0x10(%rbx),%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:107
-   29a1b1b37:	test   %rbx,%rbx
-   29a1b1b3a:	jne    29a1b1b18 <__mingwthr_run_key_dtors.part.0+0x38>
+   29a1b1b17:	test   %rbx,%rbx
+   29a1b1b1a:	jne    29a1b1af8 <__mingwthr_run_key_dtors.part.0+0x38>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:118
-   29a1b1b3c:	mov    %r12,%rcx
+   29a1b1b1c:	mov    %r12,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:119
-   29a1b1b3f:	add    $0x20,%rsp
-   29a1b1b43:	pop    %rbx
-   29a1b1b44:	pop    %rsi
-   29a1b1b45:	pop    %rdi
-   29a1b1b46:	pop    %rbp
-   29a1b1b47:	pop    %r12
+   29a1b1b1f:	add    $0x20,%rsp
+   29a1b1b23:	pop    %rbx
+   29a1b1b24:	pop    %rsi
+   29a1b1b25:	pop    %rdi
+   29a1b1b26:	pop    %rbp
+   29a1b1b27:	pop    %r12
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:118
-   29a1b1b49:	rex.W jmp *0x7720(%rip)        # 29a1b9270 <__imp_LeaveCriticalSection>
+   29a1b1b29:	rex.W jmp *0x7738(%rip)        # 29a1b9268 <__imp_LeaveCriticalSection>
 
-000000029a1b1b50 <___w64_mingwthr_add_key_dtor>:
+000000029a1b1b30 <___w64_mingwthr_add_key_dtor>:
 ___w64_mingwthr_add_key_dtor():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:43
-   29a1b1b50:	push   %rdi
-   29a1b1b51:	push   %rsi
-   29a1b1b52:	push   %rbx
-   29a1b1b53:	sub    $0x20,%rsp
+   29a1b1b30:	push   %rdi
+   29a1b1b31:	push   %rsi
+   29a1b1b32:	push   %rbx
+   29a1b1b33:	sub    $0x20,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:46
-   29a1b1b57:	mov    0x552b(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1b37:	mov    0x554b(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:43
-   29a1b1b5d:	mov    %ecx,%edi
-   29a1b1b5f:	mov    %rdx,%rsi
+   29a1b1b3d:	mov    %ecx,%edi
+   29a1b1b3f:	mov    %rdx,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:46
-   29a1b1b62:	test   %eax,%eax
-   29a1b1b64:	jne    29a1b1b70 <___w64_mingwthr_add_key_dtor+0x20>
+   29a1b1b42:	test   %eax,%eax
+   29a1b1b44:	jne    29a1b1b50 <___w64_mingwthr_add_key_dtor+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:47
-   29a1b1b66:	xor    %eax,%eax
+   29a1b1b46:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:62
-   29a1b1b68:	add    $0x20,%rsp
-   29a1b1b6c:	pop    %rbx
-   29a1b1b6d:	pop    %rsi
-   29a1b1b6e:	pop    %rdi
-   29a1b1b6f:	ret
+   29a1b1b48:	add    $0x20,%rsp
+   29a1b1b4c:	pop    %rbx
+   29a1b1b4d:	pop    %rsi
+   29a1b1b4e:	pop    %rdi
+   29a1b1b4f:	ret
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:48
-   29a1b1b70:	mov    $0x18,%edx
-   29a1b1b75:	mov    $0x1,%ecx
-   29a1b1b7a:	call   29a1b24f8 <calloc>
-   29a1b1b7f:	mov    %rax,%rbx
+   29a1b1b50:	mov    $0x18,%edx
+   29a1b1b55:	mov    $0x1,%ecx
+   29a1b1b5a:	call   29a1b24c8 <calloc>
+   29a1b1b5f:	mov    %rax,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:49
-   29a1b1b82:	test   %rax,%rax
-   29a1b1b85:	je     29a1b1bba <___w64_mingwthr_add_key_dtor+0x6a>
+   29a1b1b62:	test   %rax,%rax
+   29a1b1b65:	je     29a1b1b9a <___w64_mingwthr_add_key_dtor+0x6a>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:53
-   29a1b1b87:	mov    %rsi,0x8(%rax)
+   29a1b1b67:	mov    %rsi,0x8(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:55
-   29a1b1b8b:	lea    0x550e(%rip),%rsi        # 29a1b70a0 <__mingwthr_cs>
+   29a1b1b6b:	lea    0x552e(%rip),%rsi        # 29a1b70a0 <__mingwthr_cs>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:52
-   29a1b1b92:	mov    %edi,(%rax)
+   29a1b1b72:	mov    %edi,(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:55
-   29a1b1b94:	mov    %rsi,%rcx
-   29a1b1b97:	call   *0x76bb(%rip)        # 29a1b9258 <__imp_EnterCriticalSection>
+   29a1b1b74:	mov    %rsi,%rcx
+   29a1b1b77:	call   *0x76d3(%rip)        # 29a1b9250 <__imp_EnterCriticalSection>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:57
-   29a1b1b9d:	mov    0x54dc(%rip),%rax        # 29a1b7080 <key_dtor_list>
+   29a1b1b7d:	mov    0x54fc(%rip),%rax        # 29a1b7080 <key_dtor_list>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:60
-   29a1b1ba4:	mov    %rsi,%rcx
+   29a1b1b84:	mov    %rsi,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:58
-   29a1b1ba7:	mov    %rbx,0x54d2(%rip)        # 29a1b7080 <key_dtor_list>
+   29a1b1b87:	mov    %rbx,0x54f2(%rip)        # 29a1b7080 <key_dtor_list>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:57
-   29a1b1bae:	mov    %rax,0x10(%rbx)
+   29a1b1b8e:	mov    %rax,0x10(%rbx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:60
-   29a1b1bb2:	call   *0x76b8(%rip)        # 29a1b9270 <__imp_LeaveCriticalSection>
+   29a1b1b92:	call   *0x76d0(%rip)        # 29a1b9268 <__imp_LeaveCriticalSection>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:61
-   29a1b1bb8:	jmp    29a1b1b66 <___w64_mingwthr_add_key_dtor+0x16>
+   29a1b1b98:	jmp    29a1b1b46 <___w64_mingwthr_add_key_dtor+0x16>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:50
-   29a1b1bba:	or     $0xffffffff,%eax
-   29a1b1bbd:	jmp    29a1b1b68 <___w64_mingwthr_add_key_dtor+0x18>
-   29a1b1bbf:	nop
+   29a1b1b9a:	or     $0xffffffff,%eax
+   29a1b1b9d:	jmp    29a1b1b48 <___w64_mingwthr_add_key_dtor+0x18>
+   29a1b1b9f:	nop
 
-000000029a1b1bc0 <___w64_mingwthr_remove_key_dtor>:
+000000029a1b1ba0 <___w64_mingwthr_remove_key_dtor>:
 ___w64_mingwthr_remove_key_dtor():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:66
-   29a1b1bc0:	push   %rsi
-   29a1b1bc1:	push   %rbx
-   29a1b1bc2:	sub    $0x28,%rsp
+   29a1b1ba0:	push   %rsi
+   29a1b1ba1:	push   %rbx
+   29a1b1ba2:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:70
-   29a1b1bc6:	mov    0x54bc(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1ba6:	mov    0x54dc(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:66
-   29a1b1bcc:	mov    %ecx,%ebx
+   29a1b1bac:	mov    %ecx,%ebx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:70
-   29a1b1bce:	test   %eax,%eax
-   29a1b1bd0:	jne    29a1b1be0 <___w64_mingwthr_remove_key_dtor+0x20>
+   29a1b1bae:	test   %eax,%eax
+   29a1b1bb0:	jne    29a1b1bc0 <___w64_mingwthr_remove_key_dtor+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:96
-   29a1b1bd2:	xor    %eax,%eax
-   29a1b1bd4:	add    $0x28,%rsp
-   29a1b1bd8:	pop    %rbx
-   29a1b1bd9:	pop    %rsi
-   29a1b1bda:	ret
-   29a1b1bdb:	nopl   0x0(%rax,%rax,1)
+   29a1b1bb2:	xor    %eax,%eax
+   29a1b1bb4:	add    $0x28,%rsp
+   29a1b1bb8:	pop    %rbx
+   29a1b1bb9:	pop    %rsi
+   29a1b1bba:	ret
+   29a1b1bbb:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:73
-   29a1b1be0:	lea    0x54b9(%rip),%rsi        # 29a1b70a0 <__mingwthr_cs>
-   29a1b1be7:	mov    %rsi,%rcx
-   29a1b1bea:	call   *0x7668(%rip)        # 29a1b9258 <__imp_EnterCriticalSection>
+   29a1b1bc0:	lea    0x54d9(%rip),%rsi        # 29a1b70a0 <__mingwthr_cs>
+   29a1b1bc7:	mov    %rsi,%rcx
+   29a1b1bca:	call   *0x7680(%rip)        # 29a1b9250 <__imp_EnterCriticalSection>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:76
-   29a1b1bf0:	mov    0x5489(%rip),%rcx        # 29a1b7080 <key_dtor_list>
+   29a1b1bd0:	mov    0x54a9(%rip),%rcx        # 29a1b7080 <key_dtor_list>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:78
-   29a1b1bf7:	test   %rcx,%rcx
-   29a1b1bfa:	je     29a1b1c23 <___w64_mingwthr_remove_key_dtor+0x63>
+   29a1b1bd7:	test   %rcx,%rcx
+   29a1b1bda:	je     29a1b1c03 <___w64_mingwthr_remove_key_dtor+0x63>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:75
-   29a1b1bfc:	xor    %edx,%edx
-   29a1b1bfe:	jmp    29a1b1c0b <___w64_mingwthr_remove_key_dtor+0x4b>
+   29a1b1bdc:	xor    %edx,%edx
+   29a1b1bde:	jmp    29a1b1beb <___w64_mingwthr_remove_key_dtor+0x4b>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:78
-   29a1b1c00:	mov    %rcx,%rdx
-   29a1b1c03:	test   %rax,%rax
-   29a1b1c06:	je     29a1b1c23 <___w64_mingwthr_remove_key_dtor+0x63>
-   29a1b1c08:	mov    %rax,%rcx
+   29a1b1be0:	mov    %rcx,%rdx
+   29a1b1be3:	test   %rax,%rax
+   29a1b1be6:	je     29a1b1c03 <___w64_mingwthr_remove_key_dtor+0x63>
+   29a1b1be8:	mov    %rax,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:80
-   29a1b1c0b:	mov    (%rcx),%eax
-   29a1b1c0d:	cmp    %ebx,%eax
+   29a1b1beb:	mov    (%rcx),%eax
+   29a1b1bed:	cmp    %ebx,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:83
-   29a1b1c0f:	mov    0x10(%rcx),%rax
+   29a1b1bef:	mov    0x10(%rcx),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:80
-   29a1b1c13:	jne    29a1b1c00 <___w64_mingwthr_remove_key_dtor+0x40>
+   29a1b1bf3:	jne    29a1b1be0 <___w64_mingwthr_remove_key_dtor+0x40>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:82
-   29a1b1c15:	test   %rdx,%rdx
-   29a1b1c18:	je     29a1b1c38 <___w64_mingwthr_remove_key_dtor+0x78>
+   29a1b1bf5:	test   %rdx,%rdx
+   29a1b1bf8:	je     29a1b1c18 <___w64_mingwthr_remove_key_dtor+0x78>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:85
-   29a1b1c1a:	mov    %rax,0x10(%rdx)
+   29a1b1bfa:	mov    %rax,0x10(%rdx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:87
-   29a1b1c1e:	call   29a1b2500 <free>
+   29a1b1bfe:	call   29a1b24d0 <free>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:94
-   29a1b1c23:	mov    %rsi,%rcx
-   29a1b1c26:	call   *0x7644(%rip)        # 29a1b9270 <__imp_LeaveCriticalSection>
+   29a1b1c03:	mov    %rsi,%rcx
+   29a1b1c06:	call   *0x765c(%rip)        # 29a1b9268 <__imp_LeaveCriticalSection>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:96
-   29a1b1c2c:	xor    %eax,%eax
-   29a1b1c2e:	add    $0x28,%rsp
-   29a1b1c32:	pop    %rbx
-   29a1b1c33:	pop    %rsi
-   29a1b1c34:	ret
-   29a1b1c35:	nopl   (%rax)
+   29a1b1c0c:	xor    %eax,%eax
+   29a1b1c0e:	add    $0x28,%rsp
+   29a1b1c12:	pop    %rbx
+   29a1b1c13:	pop    %rsi
+   29a1b1c14:	ret
+   29a1b1c15:	nopl   (%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:83
-   29a1b1c38:	mov    %rax,0x5441(%rip)        # 29a1b7080 <key_dtor_list>
-   29a1b1c3f:	jmp    29a1b1c1e <___w64_mingwthr_remove_key_dtor+0x5e>
-   29a1b1c41:	data16 cs nopw 0x0(%rax,%rax,1)
-   29a1b1c4c:	nopl   0x0(%rax)
+   29a1b1c18:	mov    %rax,0x5461(%rip)        # 29a1b7080 <key_dtor_list>
+   29a1b1c1f:	jmp    29a1b1bfe <___w64_mingwthr_remove_key_dtor+0x5e>
+   29a1b1c21:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b1c2c:	nopl   0x0(%rax)
 
-000000029a1b1c50 <__mingw_TLScallback>:
+000000029a1b1c30 <__mingw_TLScallback>:
 __mingw_TLScallback():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:125
-   29a1b1c50:	push   %rbx
-   29a1b1c51:	sub    $0x20,%rsp
+   29a1b1c30:	push   %rbx
+   29a1b1c31:	sub    $0x20,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:126
-   29a1b1c55:	cmp    $0x2,%edx
-   29a1b1c58:	je     29a1b1d10 <__mingw_TLScallback+0xc0>
-   29a1b1c5e:	ja     29a1b1c90 <__mingw_TLScallback+0x40>
-   29a1b1c60:	test   %edx,%edx
-   29a1b1c62:	je     29a1b1cb0 <__mingw_TLScallback+0x60>
+   29a1b1c35:	cmp    $0x2,%edx
+   29a1b1c38:	je     29a1b1cf0 <__mingw_TLScallback+0xc0>
+   29a1b1c3e:	ja     29a1b1c70 <__mingw_TLScallback+0x40>
+   29a1b1c40:	test   %edx,%edx
+   29a1b1c42:	je     29a1b1c90 <__mingw_TLScallback+0x60>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:129
-   29a1b1c64:	mov    0x541e(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
-   29a1b1c6a:	test   %eax,%eax
-   29a1b1c6c:	je     29a1b1d30 <__mingw_TLScallback+0xe0>
+   29a1b1c44:	mov    0x543e(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1c4a:	test   %eax,%eax
+   29a1b1c4c:	je     29a1b1d10 <__mingw_TLScallback+0xe0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:131
-   29a1b1c72:	movl   $0x1,0x540c(%rip)        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1c52:	movl   $0x1,0x542c(%rip)        # 29a1b7088 <__mingwthr_cs_init>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:157
-   29a1b1c7c:	mov    $0x1,%eax
-   29a1b1c81:	add    $0x20,%rsp
-   29a1b1c85:	pop    %rbx
-   29a1b1c86:	ret
-   29a1b1c87:	nopw   0x0(%rax,%rax,1)
+   29a1b1c5c:	mov    $0x1,%eax
+   29a1b1c61:	add    $0x20,%rsp
+   29a1b1c65:	pop    %rbx
+   29a1b1c66:	ret
+   29a1b1c67:	nopw   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:126
-   29a1b1c90:	cmp    $0x3,%edx
-   29a1b1c93:	jne    29a1b1c7c <__mingw_TLScallback+0x2c>
+   29a1b1c70:	cmp    $0x3,%edx
+   29a1b1c73:	jne    29a1b1c5c <__mingw_TLScallback+0x2c>
 __mingwthr_run_key_dtors():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:103
-   29a1b1c95:	mov    0x53ed(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
-   29a1b1c9b:	test   %eax,%eax
-   29a1b1c9d:	je     29a1b1c7c <__mingw_TLScallback+0x2c>
-   29a1b1c9f:	call   29a1b1ae0 <__mingwthr_run_key_dtors.part.0>
-   29a1b1ca4:	jmp    29a1b1c7c <__mingw_TLScallback+0x2c>
-   29a1b1ca6:	cs nopw 0x0(%rax,%rax,1)
-   29a1b1cb0:	mov    0x53d2(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
-   29a1b1cb6:	test   %eax,%eax
-   29a1b1cb8:	jne    29a1b1d20 <__mingw_TLScallback+0xd0>
+   29a1b1c75:	mov    0x540d(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1c7b:	test   %eax,%eax
+   29a1b1c7d:	je     29a1b1c5c <__mingw_TLScallback+0x2c>
+   29a1b1c7f:	call   29a1b1ac0 <__mingwthr_run_key_dtors.part.0>
+   29a1b1c84:	jmp    29a1b1c5c <__mingw_TLScallback+0x2c>
+   29a1b1c86:	cs nopw 0x0(%rax,%rax,1)
+   29a1b1c90:	mov    0x53f2(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1c96:	test   %eax,%eax
+   29a1b1c98:	jne    29a1b1d00 <__mingw_TLScallback+0xd0>
 __mingw_TLScallback():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:135
-   29a1b1cba:	mov    0x53c8(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
-   29a1b1cc0:	cmp    $0x1,%eax
-   29a1b1cc3:	jne    29a1b1c7c <__mingw_TLScallback+0x2c>
+   29a1b1c9a:	mov    0x53e8(%rip),%eax        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1ca0:	cmp    $0x1,%eax
+   29a1b1ca3:	jne    29a1b1c5c <__mingw_TLScallback+0x2c>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:138
-   29a1b1cc5:	mov    0x53b4(%rip),%rbx        # 29a1b7080 <key_dtor_list>
-   29a1b1ccc:	test   %rbx,%rbx
-   29a1b1ccf:	je     29a1b1ce9 <__mingw_TLScallback+0x99>
-   29a1b1cd1:	nopl   0x0(%rax)
+   29a1b1ca5:	mov    0x53d4(%rip),%rbx        # 29a1b7080 <key_dtor_list>
+   29a1b1cac:	test   %rbx,%rbx
+   29a1b1caf:	je     29a1b1cc9 <__mingw_TLScallback+0x99>
+   29a1b1cb1:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:140
-   29a1b1cd8:	mov    %rbx,%rcx
-   29a1b1cdb:	mov    0x10(%rbx),%rbx
+   29a1b1cb8:	mov    %rbx,%rcx
+   29a1b1cbb:	mov    0x10(%rbx),%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:141
-   29a1b1cdf:	call   29a1b2500 <free>
+   29a1b1cbf:	call   29a1b24d0 <free>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:138
-   29a1b1ce4:	test   %rbx,%rbx
-   29a1b1ce7:	jne    29a1b1cd8 <__mingw_TLScallback+0x88>
+   29a1b1cc4:	test   %rbx,%rbx
+   29a1b1cc7:	jne    29a1b1cb8 <__mingw_TLScallback+0x88>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:146
-   29a1b1ce9:	lea    0x53b0(%rip),%rcx        # 29a1b70a0 <__mingwthr_cs>
+   29a1b1cc9:	lea    0x53d0(%rip),%rcx        # 29a1b70a0 <__mingwthr_cs>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:144
-   29a1b1cf0:	movq   $0x0,0x5385(%rip)        # 29a1b7080 <key_dtor_list>
+   29a1b1cd0:	movq   $0x0,0x53a5(%rip)        # 29a1b7080 <key_dtor_list>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:145
-   29a1b1cfb:	movl   $0x0,0x5383(%rip)        # 29a1b7088 <__mingwthr_cs_init>
+   29a1b1cdb:	movl   $0x0,0x53a3(%rip)        # 29a1b7088 <__mingwthr_cs_init>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:146
-   29a1b1d05:	call   *0x7545(%rip)        # 29a1b9250 <__IAT_start__>
-   29a1b1d0b:	jmp    29a1b1c7c <__mingw_TLScallback+0x2c>
+   29a1b1ce5:	call   *0x755d(%rip)        # 29a1b9248 <__IAT_start__>
+   29a1b1ceb:	jmp    29a1b1c5c <__mingw_TLScallback+0x2c>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:150
-   29a1b1d10:	call   29a1b2150 <_fpreset>
+   29a1b1cf0:	call   29a1b2130 <_fpreset>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:157
-   29a1b1d15:	mov    $0x1,%eax
-   29a1b1d1a:	add    $0x20,%rsp
-   29a1b1d1e:	pop    %rbx
-   29a1b1d1f:	ret
+   29a1b1cf5:	mov    $0x1,%eax
+   29a1b1cfa:	add    $0x20,%rsp
+   29a1b1cfe:	pop    %rbx
+   29a1b1cff:	ret
 __mingwthr_run_key_dtors():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:157
-   29a1b1d20:	call   29a1b1ae0 <__mingwthr_run_key_dtors.part.0>
-   29a1b1d25:	jmp    29a1b1cba <__mingw_TLScallback+0x6a>
-   29a1b1d27:	nopw   0x0(%rax,%rax,1)
+   29a1b1d00:	call   29a1b1ac0 <__mingwthr_run_key_dtors.part.0>
+   29a1b1d05:	jmp    29a1b1c9a <__mingw_TLScallback+0x6a>
+   29a1b1d07:	nopw   0x0(%rax,%rax,1)
 __mingw_TLScallback():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsthrd.c:130
-   29a1b1d30:	lea    0x5369(%rip),%rcx        # 29a1b70a0 <__mingwthr_cs>
-   29a1b1d37:	call   *0x752b(%rip)        # 29a1b9268 <__imp_InitializeCriticalSection>
-   29a1b1d3d:	jmp    29a1b1c72 <__mingw_TLScallback+0x22>
-   29a1b1d42:	nop
-   29a1b1d43:	nop
-   29a1b1d44:	nop
-   29a1b1d45:	nop
-   29a1b1d46:	nop
-   29a1b1d47:	nop
-   29a1b1d48:	nop
-   29a1b1d49:	nop
-   29a1b1d4a:	nop
-   29a1b1d4b:	nop
-   29a1b1d4c:	nop
-   29a1b1d4d:	nop
-   29a1b1d4e:	nop
-   29a1b1d4f:	nop
+   29a1b1d10:	lea    0x5389(%rip),%rcx        # 29a1b70a0 <__mingwthr_cs>
+   29a1b1d17:	call   *0x7543(%rip)        # 29a1b9260 <__imp_InitializeCriticalSection>
+   29a1b1d1d:	jmp    29a1b1c52 <__mingw_TLScallback+0x22>
+   29a1b1d22:	nop
+   29a1b1d23:	nop
+   29a1b1d24:	nop
+   29a1b1d25:	nop
+   29a1b1d26:	nop
+   29a1b1d27:	nop
+   29a1b1d28:	nop
+   29a1b1d29:	nop
+   29a1b1d2a:	nop
+   29a1b1d2b:	nop
+   29a1b1d2c:	nop
+   29a1b1d2d:	nop
+   29a1b1d2e:	nop
+   29a1b1d2f:	nop
 
-000000029a1b1d50 <_ValidateImageBase>:
+000000029a1b1d30 <_ValidateImageBase>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:23
-   29a1b1d50:	xor    %eax,%eax
+   29a1b1d30:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1d52:	cmpw   $0x5a4d,(%rcx)
-   29a1b1d57:	jne    29a1b1d68 <_ValidateImageBase+0x18>
+   29a1b1d32:	cmpw   $0x5a4d,(%rcx)
+   29a1b1d37:	jne    29a1b1d48 <_ValidateImageBase+0x18>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1d59:	movslq 0x3c(%rcx),%rdx
-   29a1b1d5d:	add    %rdx,%rcx
+   29a1b1d39:	movslq 0x3c(%rcx),%rdx
+   29a1b1d3d:	add    %rdx,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1d60:	cmpl   $0x4550,(%rcx)
-   29a1b1d66:	je     29a1b1d70 <_ValidateImageBase+0x20>
+   29a1b1d40:	cmpl   $0x4550,(%rcx)
+   29a1b1d46:	je     29a1b1d50 <_ValidateImageBase+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:31
-   29a1b1d68:	ret
-   29a1b1d69:	nopl   0x0(%rax)
+   29a1b1d48:	ret
+   29a1b1d49:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b1d70:	xor    %eax,%eax
-   29a1b1d72:	cmpw   $0x20b,0x18(%rcx)
-   29a1b1d78:	sete   %al
+   29a1b1d50:	xor    %eax,%eax
+   29a1b1d52:	cmpw   $0x20b,0x18(%rcx)
+   29a1b1d58:	sete   %al
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:31
-   29a1b1d7b:	ret
-   29a1b1d7c:	nopl   0x0(%rax)
+   29a1b1d5b:	ret
+   29a1b1d5c:	nopl   0x0(%rax)
 
-000000029a1b1d80 <_FindPESection>:
+000000029a1b1d60 <_FindPESection>:
 _FindPESection():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:42
-   29a1b1d80:	movslq 0x3c(%rcx),%rax
-   29a1b1d84:	add    %rax,%rcx
+   29a1b1d60:	movslq 0x3c(%rcx),%rax
+   29a1b1d64:	add    %rax,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b1d87:	movzwl 0x14(%rcx),%eax
+   29a1b1d67:	movzwl 0x14(%rcx),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b1d8b:	movzwl 0x6(%rcx),%r8d
+   29a1b1d6b:	movzwl 0x6(%rcx),%r8d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b1d90:	lea    0x18(%rcx,%rax,1),%rax
+   29a1b1d70:	lea    0x18(%rcx,%rax,1),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b1d95:	test   %r8w,%r8w
-   29a1b1d99:	je     29a1b1dcd <_FindPESection+0x4d>
-   29a1b1d9b:	lea    -0x1(%r8),%ecx
-   29a1b1d9f:	lea    (%rcx,%rcx,4),%rcx
-   29a1b1da3:	lea    0x28(%rax,%rcx,8),%r9
-   29a1b1da8:	nopl   0x0(%rax,%rax,1)
+   29a1b1d75:	test   %r8w,%r8w
+   29a1b1d79:	je     29a1b1dad <_FindPESection+0x4d>
+   29a1b1d7b:	lea    -0x1(%r8),%ecx
+   29a1b1d7f:	lea    (%rcx,%rcx,4),%rcx
+   29a1b1d83:	lea    0x28(%rax,%rcx,8),%r9
+   29a1b1d88:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:48
-   29a1b1db0:	mov    0xc(%rax),%r8d
-   29a1b1db4:	mov    %r8,%rcx
-   29a1b1db7:	cmp    %r8,%rdx
-   29a1b1dba:	jb     29a1b1dc4 <_FindPESection+0x44>
+   29a1b1d90:	mov    0xc(%rax),%r8d
+   29a1b1d94:	mov    %r8,%rcx
+   29a1b1d97:	cmp    %r8,%rdx
+   29a1b1d9a:	jb     29a1b1da4 <_FindPESection+0x44>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:49
-   29a1b1dbc:	add    0x8(%rax),%ecx
-   29a1b1dbf:	cmp    %rcx,%rdx
-   29a1b1dc2:	jb     29a1b1dcf <_FindPESection+0x4f>
+   29a1b1d9c:	add    0x8(%rax),%ecx
+   29a1b1d9f:	cmp    %rcx,%rdx
+   29a1b1da2:	jb     29a1b1daf <_FindPESection+0x4f>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:46
-   29a1b1dc4:	add    $0x28,%rax
+   29a1b1da4:	add    $0x28,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b1dc8:	cmp    %r9,%rax
-   29a1b1dcb:	jne    29a1b1db0 <_FindPESection+0x30>
+   29a1b1da8:	cmp    %r9,%rax
+   29a1b1dab:	jne    29a1b1d90 <_FindPESection+0x30>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:52
-   29a1b1dcd:	xor    %eax,%eax
+   29a1b1dad:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:53
-   29a1b1dcf:	ret
+   29a1b1daf:	ret
 
-000000029a1b1dd0 <_FindPESectionByName>:
+000000029a1b1db0 <_FindPESectionByName>:
 _FindPESectionByName():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:59
-   29a1b1dd0:	push   %rdi
-   29a1b1dd1:	push   %rsi
-   29a1b1dd2:	push   %rbx
-   29a1b1dd3:	sub    $0x20,%rsp
-   29a1b1dd7:	mov    %rcx,%rsi
+   29a1b1db0:	push   %rdi
+   29a1b1db1:	push   %rsi
+   29a1b1db2:	push   %rbx
+   29a1b1db3:	sub    $0x20,%rsp
+   29a1b1db7:	mov    %rcx,%rsi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:66
-   29a1b1dda:	call   29a1b2420 <strlen>
-   29a1b1ddf:	cmp    $0x8,%rax
-   29a1b1de3:	ja     29a1b1e60 <_FindPESectionByName+0x90>
+   29a1b1dba:	call   29a1b2400 <strlen>
+   29a1b1dbf:	cmp    $0x8,%rax
+   29a1b1dc3:	ja     29a1b1e40 <_FindPESectionByName+0x90>
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1de5:	mov    0x2414(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1dc5:	mov    0x2434(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
 _FindPESectionByName():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:67
-   29a1b1dec:	xor    %ebx,%ebx
+   29a1b1dcc:	xor    %ebx,%ebx
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1dee:	cmpw   $0x5a4d,(%rdx)
-   29a1b1df3:	jne    29a1b1e4e <_FindPESectionByName+0x7e>
+   29a1b1dce:	cmpw   $0x5a4d,(%rdx)
+   29a1b1dd3:	jne    29a1b1e2e <_FindPESectionByName+0x7e>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1df5:	movslq 0x3c(%rdx),%rax
-   29a1b1df9:	add    %rdx,%rax
+   29a1b1dd5:	movslq 0x3c(%rdx),%rax
+   29a1b1dd9:	add    %rdx,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1dfc:	cmpl   $0x4550,(%rax)
-   29a1b1e02:	jne    29a1b1e4e <_FindPESectionByName+0x7e>
+   29a1b1ddc:	cmpl   $0x4550,(%rax)
+   29a1b1de2:	jne    29a1b1e2e <_FindPESectionByName+0x7e>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b1e04:	cmpw   $0x20b,0x18(%rax)
-   29a1b1e0a:	jne    29a1b1e4e <_FindPESectionByName+0x7e>
+   29a1b1de4:	cmpw   $0x20b,0x18(%rax)
+   29a1b1dea:	jne    29a1b1e2e <_FindPESectionByName+0x7e>
 _FindPESectionByName():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:75
-   29a1b1e0c:	movzwl 0x14(%rax),%edx
-   29a1b1e10:	lea    0x18(%rax,%rdx,1),%rbx
+   29a1b1dec:	movzwl 0x14(%rax),%edx
+   29a1b1df0:	lea    0x18(%rax,%rdx,1),%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:76
-   29a1b1e15:	movzwl 0x6(%rax),%edx
-   29a1b1e19:	test   %dx,%dx
-   29a1b1e1c:	je     29a1b1e60 <_FindPESectionByName+0x90>
-   29a1b1e1e:	lea    -0x1(%rdx),%eax
-   29a1b1e21:	lea    (%rax,%rax,4),%rax
-   29a1b1e25:	lea    0x28(%rbx,%rax,8),%rdi
-   29a1b1e2a:	jmp    29a1b1e39 <_FindPESectionByName+0x69>
-   29a1b1e2c:	nopl   0x0(%rax)
+   29a1b1df5:	movzwl 0x6(%rax),%edx
+   29a1b1df9:	test   %dx,%dx
+   29a1b1dfc:	je     29a1b1e40 <_FindPESectionByName+0x90>
+   29a1b1dfe:	lea    -0x1(%rdx),%eax
+   29a1b1e01:	lea    (%rax,%rax,4),%rax
+   29a1b1e05:	lea    0x28(%rbx,%rax,8),%rdi
+   29a1b1e0a:	jmp    29a1b1e19 <_FindPESectionByName+0x69>
+   29a1b1e0c:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:77
-   29a1b1e30:	add    $0x28,%rbx
+   29a1b1e10:	add    $0x28,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:76
-   29a1b1e34:	cmp    %rdi,%rbx
-   29a1b1e37:	je     29a1b1e60 <_FindPESectionByName+0x90>
+   29a1b1e14:	cmp    %rdi,%rbx
+   29a1b1e17:	je     29a1b1e40 <_FindPESectionByName+0x90>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:79
-   29a1b1e39:	mov    $0x8,%r8d
-   29a1b1e3f:	mov    %rsi,%rdx
-   29a1b1e42:	mov    %rbx,%rcx
-   29a1b1e45:	call   29a1b2428 <strncmp>
-   29a1b1e4a:	test   %eax,%eax
-   29a1b1e4c:	jne    29a1b1e30 <_FindPESectionByName+0x60>
+   29a1b1e19:	mov    $0x8,%r8d
+   29a1b1e1f:	mov    %rsi,%rdx
+   29a1b1e22:	mov    %rbx,%rcx
+   29a1b1e25:	call   29a1b2408 <strncmp>
+   29a1b1e2a:	test   %eax,%eax
+   29a1b1e2c:	jne    29a1b1e10 <_FindPESectionByName+0x60>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:83
-   29a1b1e4e:	mov    %rbx,%rax
-   29a1b1e51:	add    $0x20,%rsp
-   29a1b1e55:	pop    %rbx
-   29a1b1e56:	pop    %rsi
-   29a1b1e57:	pop    %rdi
-   29a1b1e58:	ret
-   29a1b1e59:	nopl   0x0(%rax)
+   29a1b1e2e:	mov    %rbx,%rax
+   29a1b1e31:	add    $0x20,%rsp
+   29a1b1e35:	pop    %rbx
+   29a1b1e36:	pop    %rsi
+   29a1b1e37:	pop    %rdi
+   29a1b1e38:	ret
+   29a1b1e39:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:67
-   29a1b1e60:	xor    %ebx,%ebx
+   29a1b1e40:	xor    %ebx,%ebx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:83
-   29a1b1e62:	mov    %rbx,%rax
-   29a1b1e65:	add    $0x20,%rsp
-   29a1b1e69:	pop    %rbx
-   29a1b1e6a:	pop    %rsi
-   29a1b1e6b:	pop    %rdi
-   29a1b1e6c:	ret
-   29a1b1e6d:	nopl   (%rax)
+   29a1b1e42:	mov    %rbx,%rax
+   29a1b1e45:	add    $0x20,%rsp
+   29a1b1e49:	pop    %rbx
+   29a1b1e4a:	pop    %rsi
+   29a1b1e4b:	pop    %rdi
+   29a1b1e4c:	ret
+   29a1b1e4d:	nopl   (%rax)
 
-000000029a1b1e70 <__mingw_GetSectionForAddress>:
+000000029a1b1e50 <__mingw_GetSectionForAddress>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1e70:	mov    0x2389(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1e50:	mov    0x23a9(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
 __mingw_GetSectionForAddress():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:96
-   29a1b1e77:	xor    %eax,%eax
+   29a1b1e57:	xor    %eax,%eax
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1e79:	cmpw   $0x5a4d,(%rdx)
-   29a1b1e7e:	jne    29a1b1e90 <__mingw_GetSectionForAddress+0x20>
+   29a1b1e59:	cmpw   $0x5a4d,(%rdx)
+   29a1b1e5e:	jne    29a1b1e70 <__mingw_GetSectionForAddress+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1e80:	movslq 0x3c(%rdx),%r8
-   29a1b1e84:	add    %rdx,%r8
+   29a1b1e60:	movslq 0x3c(%rdx),%r8
+   29a1b1e64:	add    %rdx,%r8
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1e87:	cmpl   $0x4550,(%r8)
-   29a1b1e8e:	je     29a1b1e98 <__mingw_GetSectionForAddress+0x28>
+   29a1b1e67:	cmpl   $0x4550,(%r8)
+   29a1b1e6e:	je     29a1b1e78 <__mingw_GetSectionForAddress+0x28>
 __mingw_GetSectionForAddress():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:100
-   29a1b1e90:	ret
-   29a1b1e91:	nopl   0x0(%rax)
+   29a1b1e70:	ret
+   29a1b1e71:	nopl   0x0(%rax)
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b1e98:	cmpw   $0x20b,0x18(%r8)
-   29a1b1e9f:	jne    29a1b1e90 <__mingw_GetSectionForAddress+0x20>
+   29a1b1e78:	cmpw   $0x20b,0x18(%r8)
+   29a1b1e7f:	jne    29a1b1e70 <__mingw_GetSectionForAddress+0x20>
 _FindPESection():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b1ea1:	movzwl 0x14(%r8),%eax
+   29a1b1e81:	movzwl 0x14(%r8),%eax
 __mingw_GetSectionForAddress():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:98
-   29a1b1ea6:	sub    %rdx,%rcx
+   29a1b1e86:	sub    %rdx,%rcx
 _FindPESection():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b1ea9:	lea    0x18(%r8,%rax,1),%rax
+   29a1b1e89:	lea    0x18(%r8,%rax,1),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b1eae:	movzwl 0x6(%r8),%r8d
-   29a1b1eb3:	test   %r8w,%r8w
-   29a1b1eb7:	je     29a1b1eed <__mingw_GetSectionForAddress+0x7d>
-   29a1b1eb9:	lea    -0x1(%r8),%edx
-   29a1b1ebd:	lea    (%rdx,%rdx,4),%rdx
-   29a1b1ec1:	lea    0x28(%rax,%rdx,8),%r9
-   29a1b1ec6:	cs nopw 0x0(%rax,%rax,1)
+   29a1b1e8e:	movzwl 0x6(%r8),%r8d
+   29a1b1e93:	test   %r8w,%r8w
+   29a1b1e97:	je     29a1b1ecd <__mingw_GetSectionForAddress+0x7d>
+   29a1b1e99:	lea    -0x1(%r8),%edx
+   29a1b1e9d:	lea    (%rdx,%rdx,4),%rdx
+   29a1b1ea1:	lea    0x28(%rax,%rdx,8),%r9
+   29a1b1ea6:	cs nopw 0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:48
-   29a1b1ed0:	mov    0xc(%rax),%r8d
-   29a1b1ed4:	mov    %r8,%rdx
-   29a1b1ed7:	cmp    %r8,%rcx
-   29a1b1eda:	jb     29a1b1ee4 <__mingw_GetSectionForAddress+0x74>
+   29a1b1eb0:	mov    0xc(%rax),%r8d
+   29a1b1eb4:	mov    %r8,%rdx
+   29a1b1eb7:	cmp    %r8,%rcx
+   29a1b1eba:	jb     29a1b1ec4 <__mingw_GetSectionForAddress+0x74>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:49
-   29a1b1edc:	add    0x8(%rax),%edx
-   29a1b1edf:	cmp    %rdx,%rcx
-   29a1b1ee2:	jb     29a1b1e90 <__mingw_GetSectionForAddress+0x20>
+   29a1b1ebc:	add    0x8(%rax),%edx
+   29a1b1ebf:	cmp    %rdx,%rcx
+   29a1b1ec2:	jb     29a1b1e70 <__mingw_GetSectionForAddress+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:46
-   29a1b1ee4:	add    $0x28,%rax
+   29a1b1ec4:	add    $0x28,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b1ee8:	cmp    %r9,%rax
-   29a1b1eeb:	jne    29a1b1ed0 <__mingw_GetSectionForAddress+0x60>
+   29a1b1ec8:	cmp    %r9,%rax
+   29a1b1ecb:	jne    29a1b1eb0 <__mingw_GetSectionForAddress+0x60>
 __mingw_GetSectionForAddress():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:96
-   29a1b1eed:	xor    %eax,%eax
+   29a1b1ecd:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:100
-   29a1b1eef:	ret
+   29a1b1ecf:	ret
 
-000000029a1b1ef0 <__mingw_GetSectionCount>:
+000000029a1b1ed0 <__mingw_GetSectionCount>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1ef0:	mov    0x2309(%rip),%rax        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1ed0:	mov    0x2329(%rip),%rax        # 29a1b4200 <.refptr.__ImageBase>
 __mingw_GetSectionCount():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:110
-   29a1b1ef7:	xor    %ecx,%ecx
+   29a1b1ed7:	xor    %ecx,%ecx
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1ef9:	cmpw   $0x5a4d,(%rax)
-   29a1b1efe:	jne    29a1b1f0f <__mingw_GetSectionCount+0x1f>
+   29a1b1ed9:	cmpw   $0x5a4d,(%rax)
+   29a1b1ede:	jne    29a1b1eef <__mingw_GetSectionCount+0x1f>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1f00:	movslq 0x3c(%rax),%rdx
-   29a1b1f04:	add    %rdx,%rax
+   29a1b1ee0:	movslq 0x3c(%rax),%rdx
+   29a1b1ee4:	add    %rdx,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1f07:	cmpl   $0x4550,(%rax)
-   29a1b1f0d:	je     29a1b1f18 <__mingw_GetSectionCount+0x28>
+   29a1b1ee7:	cmpl   $0x4550,(%rax)
+   29a1b1eed:	je     29a1b1ef8 <__mingw_GetSectionCount+0x28>
 __mingw_GetSectionCount():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:115
-   29a1b1f0f:	mov    %ecx,%eax
-   29a1b1f11:	ret
-   29a1b1f12:	nopw   0x0(%rax,%rax,1)
+   29a1b1eef:	mov    %ecx,%eax
+   29a1b1ef1:	ret
+   29a1b1ef2:	nopw   0x0(%rax,%rax,1)
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b1f18:	cmpw   $0x20b,0x18(%rax)
-   29a1b1f1e:	jne    29a1b1f0f <__mingw_GetSectionCount+0x1f>
+   29a1b1ef8:	cmpw   $0x20b,0x18(%rax)
+   29a1b1efe:	jne    29a1b1eef <__mingw_GetSectionCount+0x1f>
 __mingw_GetSectionCount():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:114
-   29a1b1f20:	movzwl 0x6(%rax),%ecx
+   29a1b1f00:	movzwl 0x6(%rax),%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:115
-   29a1b1f24:	mov    %ecx,%eax
-   29a1b1f26:	ret
-   29a1b1f27:	nopw   0x0(%rax,%rax,1)
+   29a1b1f04:	mov    %ecx,%eax
+   29a1b1f06:	ret
+   29a1b1f07:	nopw   0x0(%rax,%rax,1)
 
-000000029a1b1f30 <_FindPESectionExec>:
+000000029a1b1f10 <_FindPESectionExec>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1f30:	mov    0x22c9(%rip),%r8        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1f10:	mov    0x22e9(%rip),%r8        # 29a1b4200 <.refptr.__ImageBase>
 _FindPESectionExec():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:130
-   29a1b1f37:	xor    %eax,%eax
+   29a1b1f17:	xor    %eax,%eax
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1f39:	cmpw   $0x5a4d,(%r8)
-   29a1b1f3f:	jne    29a1b1f50 <_FindPESectionExec+0x20>
+   29a1b1f19:	cmpw   $0x5a4d,(%r8)
+   29a1b1f1f:	jne    29a1b1f30 <_FindPESectionExec+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1f41:	movslq 0x3c(%r8),%rdx
-   29a1b1f45:	add    %r8,%rdx
+   29a1b1f21:	movslq 0x3c(%r8),%rdx
+   29a1b1f25:	add    %r8,%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1f48:	cmpl   $0x4550,(%rdx)
-   29a1b1f4e:	je     29a1b1f58 <_FindPESectionExec+0x28>
+   29a1b1f28:	cmpl   $0x4550,(%rdx)
+   29a1b1f2e:	je     29a1b1f38 <_FindPESectionExec+0x28>
 _FindPESectionExec():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:146
-   29a1b1f50:	ret
-   29a1b1f51:	nopl   0x0(%rax)
+   29a1b1f30:	ret
+   29a1b1f31:	nopl   0x0(%rax)
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b1f58:	cmpw   $0x20b,0x18(%rdx)
-   29a1b1f5e:	jne    29a1b1f50 <_FindPESectionExec+0x20>
+   29a1b1f38:	cmpw   $0x20b,0x18(%rdx)
+   29a1b1f3e:	jne    29a1b1f30 <_FindPESectionExec+0x20>
 _FindPESectionExec():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:134
-   29a1b1f60:	movzwl 0x14(%rdx),%eax
+   29a1b1f40:	movzwl 0x14(%rdx),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:135
-   29a1b1f64:	movzwl 0x6(%rdx),%r8d
+   29a1b1f44:	movzwl 0x6(%rdx),%r8d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:134
-   29a1b1f69:	lea    0x18(%rdx,%rax,1),%rax
+   29a1b1f49:	lea    0x18(%rdx,%rax,1),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:135
-   29a1b1f6e:	test   %r8w,%r8w
-   29a1b1f72:	je     29a1b1fa0 <_FindPESectionExec+0x70>
-   29a1b1f74:	lea    -0x1(%r8),%edx
-   29a1b1f78:	lea    (%rdx,%rdx,4),%rdx
-   29a1b1f7c:	lea    0x28(%rax,%rdx,8),%rdx
-   29a1b1f81:	nopl   0x0(%rax)
+   29a1b1f4e:	test   %r8w,%r8w
+   29a1b1f52:	je     29a1b1f80 <_FindPESectionExec+0x70>
+   29a1b1f54:	lea    -0x1(%r8),%edx
+   29a1b1f58:	lea    (%rdx,%rdx,4),%rdx
+   29a1b1f5c:	lea    0x28(%rax,%rdx,8),%rdx
+   29a1b1f61:	nopl   0x0(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:138
-   29a1b1f88:	testb  $0x20,0x27(%rax)
-   29a1b1f8c:	je     29a1b1f97 <_FindPESectionExec+0x67>
+   29a1b1f68:	testb  $0x20,0x27(%rax)
+   29a1b1f6c:	je     29a1b1f77 <_FindPESectionExec+0x67>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:140
-   29a1b1f8e:	test   %rcx,%rcx
-   29a1b1f91:	je     29a1b1f50 <_FindPESectionExec+0x20>
+   29a1b1f6e:	test   %rcx,%rcx
+   29a1b1f71:	je     29a1b1f30 <_FindPESectionExec+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:142
-   29a1b1f93:	sub    $0x1,%rcx
+   29a1b1f73:	sub    $0x1,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:136
-   29a1b1f97:	add    $0x28,%rax
+   29a1b1f77:	add    $0x28,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:135
-   29a1b1f9b:	cmp    %rax,%rdx
-   29a1b1f9e:	jne    29a1b1f88 <_FindPESectionExec+0x58>
+   29a1b1f7b:	cmp    %rax,%rdx
+   29a1b1f7e:	jne    29a1b1f68 <_FindPESectionExec+0x58>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:130
-   29a1b1fa0:	xor    %eax,%eax
+   29a1b1f80:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:146
-   29a1b1fa2:	ret
-   29a1b1fa3:	data16 cs nopw 0x0(%rax,%rax,1)
-   29a1b1fae:	xchg   %ax,%ax
+   29a1b1f82:	ret
+   29a1b1f83:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b1f8e:	xchg   %ax,%ax
 
-000000029a1b1fb0 <_GetPEImageBase>:
+000000029a1b1f90 <_GetPEImageBase>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1fb0:	mov    0x2249(%rip),%rax        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1f90:	mov    0x2269(%rip),%rax        # 29a1b4200 <.refptr.__ImageBase>
 _GetPEImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:156
-   29a1b1fb7:	xor    %edx,%edx
+   29a1b1f97:	xor    %edx,%edx
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1fb9:	cmpw   $0x5a4d,(%rax)
-   29a1b1fbe:	jne    29a1b1fcf <_GetPEImageBase+0x1f>
+   29a1b1f99:	cmpw   $0x5a4d,(%rax)
+   29a1b1f9e:	jne    29a1b1faf <_GetPEImageBase+0x1f>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b1fc0:	movslq 0x3c(%rax),%rcx
-   29a1b1fc4:	add    %rax,%rcx
+   29a1b1fa0:	movslq 0x3c(%rax),%rcx
+   29a1b1fa4:	add    %rax,%rcx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b1fc7:	cmpl   $0x4550,(%rcx)
-   29a1b1fcd:	je     29a1b1fd8 <_GetPEImageBase+0x28>
+   29a1b1fa7:	cmpl   $0x4550,(%rcx)
+   29a1b1fad:	je     29a1b1fb8 <_GetPEImageBase+0x28>
 _GetPEImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:158
-   29a1b1fcf:	mov    %rdx,%rax
-   29a1b1fd2:	ret
-   29a1b1fd3:	nopl   0x0(%rax,%rax,1)
+   29a1b1faf:	mov    %rdx,%rax
+   29a1b1fb2:	ret
+   29a1b1fb3:	nopl   0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:157
-   29a1b1fd8:	cmpw   $0x20b,0x18(%rcx)
-   29a1b1fde:	cmove  %rax,%rdx
+   29a1b1fb8:	cmpw   $0x20b,0x18(%rcx)
+   29a1b1fbe:	cmove  %rax,%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:158
-   29a1b1fe2:	mov    %rdx,%rax
-   29a1b1fe5:	ret
-   29a1b1fe6:	cs nopw 0x0(%rax,%rax,1)
+   29a1b1fc2:	mov    %rdx,%rax
+   29a1b1fc5:	ret
+   29a1b1fc6:	cs nopw 0x0(%rax,%rax,1)
 
-000000029a1b1ff0 <_IsNonwritableInCurrentImage>:
+000000029a1b1fd0 <_IsNonwritableInCurrentImage>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1ff0:	mov    0x2209(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b1fd0:	mov    0x2229(%rip),%rdx        # 29a1b4200 <.refptr.__ImageBase>
 _IsNonwritableInCurrentImage():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:171
-   29a1b1ff7:	xor    %eax,%eax
+   29a1b1fd7:	xor    %eax,%eax
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b1ff9:	cmpw   $0x5a4d,(%rdx)
-   29a1b1ffe:	jne    29a1b2010 <_IsNonwritableInCurrentImage+0x20>
+   29a1b1fd9:	cmpw   $0x5a4d,(%rdx)
+   29a1b1fde:	jne    29a1b1ff0 <_IsNonwritableInCurrentImage+0x20>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b2000:	movslq 0x3c(%rdx),%r8
-   29a1b2004:	add    %rdx,%r8
+   29a1b1fe0:	movslq 0x3c(%rdx),%r8
+   29a1b1fe4:	add    %rdx,%r8
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b2007:	cmpl   $0x4550,(%r8)
-   29a1b200e:	je     29a1b2018 <_IsNonwritableInCurrentImage+0x28>
+   29a1b1fe7:	cmpl   $0x4550,(%r8)
+   29a1b1fee:	je     29a1b1ff8 <_IsNonwritableInCurrentImage+0x28>
 _IsNonwritableInCurrentImage():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:177
-   29a1b2010:	ret
-   29a1b2011:	nopl   0x0(%rax)
+   29a1b1ff0:	ret
+   29a1b1ff1:	nopl   0x0(%rax)
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b2018:	cmpw   $0x20b,0x18(%r8)
-   29a1b201f:	jne    29a1b2010 <_IsNonwritableInCurrentImage+0x20>
+   29a1b1ff8:	cmpw   $0x20b,0x18(%r8)
+   29a1b1fff:	jne    29a1b1ff0 <_IsNonwritableInCurrentImage+0x20>
 _IsNonwritableInCurrentImage():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:172
-   29a1b2021:	sub    %rdx,%rcx
+   29a1b2001:	sub    %rdx,%rcx
 _FindPESection():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b2024:	movzwl 0x6(%r8),%r9d
+   29a1b2004:	movzwl 0x6(%r8),%r9d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b2029:	movzwl 0x14(%r8),%edx
-   29a1b202e:	lea    0x18(%r8,%rdx,1),%rdx
+   29a1b2009:	movzwl 0x14(%r8),%edx
+   29a1b200e:	lea    0x18(%r8,%rdx,1),%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b2033:	test   %r9w,%r9w
-   29a1b2037:	je     29a1b2010 <_IsNonwritableInCurrentImage+0x20>
-   29a1b2039:	lea    -0x1(%r9),%eax
-   29a1b203d:	lea    (%rax,%rax,4),%rax
-   29a1b2041:	lea    0x28(%rdx,%rax,8),%r9
-   29a1b2046:	cs nopw 0x0(%rax,%rax,1)
+   29a1b2013:	test   %r9w,%r9w
+   29a1b2017:	je     29a1b1ff0 <_IsNonwritableInCurrentImage+0x20>
+   29a1b2019:	lea    -0x1(%r9),%eax
+   29a1b201d:	lea    (%rax,%rax,4),%rax
+   29a1b2021:	lea    0x28(%rdx,%rax,8),%r9
+   29a1b2026:	cs nopw 0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:48
-   29a1b2050:	mov    0xc(%rdx),%r8d
-   29a1b2054:	mov    %r8,%rax
-   29a1b2057:	cmp    %r8,%rcx
-   29a1b205a:	jb     29a1b2064 <_IsNonwritableInCurrentImage+0x74>
+   29a1b2030:	mov    0xc(%rdx),%r8d
+   29a1b2034:	mov    %r8,%rax
+   29a1b2037:	cmp    %r8,%rcx
+   29a1b203a:	jb     29a1b2044 <_IsNonwritableInCurrentImage+0x74>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:49
-   29a1b205c:	add    0x8(%rdx),%eax
-   29a1b205f:	cmp    %rax,%rcx
-   29a1b2062:	jb     29a1b2070 <_IsNonwritableInCurrentImage+0x80>
+   29a1b203c:	add    0x8(%rdx),%eax
+   29a1b203f:	cmp    %rax,%rcx
+   29a1b2042:	jb     29a1b2050 <_IsNonwritableInCurrentImage+0x80>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:46
-   29a1b2064:	add    $0x28,%rdx
+   29a1b2044:	add    $0x28,%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b2068:	cmp    %r9,%rdx
-   29a1b206b:	jne    29a1b2050 <_IsNonwritableInCurrentImage+0x60>
+   29a1b2048:	cmp    %r9,%rdx
+   29a1b204b:	jne    29a1b2030 <_IsNonwritableInCurrentImage+0x60>
 _IsNonwritableInCurrentImage():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:171
-   29a1b206d:	xor    %eax,%eax
+   29a1b204d:	xor    %eax,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:177
-   29a1b206f:	ret
+   29a1b204f:	ret
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:176
-   29a1b2070:	mov    0x24(%rdx),%eax
-   29a1b2073:	not    %eax
-   29a1b2075:	shr    $0x1f,%eax
+   29a1b2050:	mov    0x24(%rdx),%eax
+   29a1b2053:	not    %eax
+   29a1b2055:	shr    $0x1f,%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:177
-   29a1b2078:	ret
-   29a1b2079:	nopl   0x0(%rax)
+   29a1b2058:	ret
+   29a1b2059:	nopl   0x0(%rax)
 
-000000029a1b2080 <__mingw_enum_import_library_names>:
+000000029a1b2060 <__mingw_enum_import_library_names>:
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b2080:	mov    0x2179(%rip),%r11        # 29a1b4200 <.refptr.__ImageBase>
+   29a1b2060:	mov    0x2199(%rip),%r11        # 29a1b4200 <.refptr.__ImageBase>
 __mingw_enum_import_library_names():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:193
-   29a1b2087:	xor    %r9d,%r9d
+   29a1b2067:	xor    %r9d,%r9d
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:22
-   29a1b208a:	cmpw   $0x5a4d,(%r11)
-   29a1b2090:	jne    29a1b20a2 <__mingw_enum_import_library_names+0x22>
+   29a1b206a:	cmpw   $0x5a4d,(%r11)
+   29a1b2070:	jne    29a1b2082 <__mingw_enum_import_library_names+0x22>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:24
-   29a1b2092:	movslq 0x3c(%r11),%r8
-   29a1b2096:	add    %r11,%r8
+   29a1b2072:	movslq 0x3c(%r11),%r8
+   29a1b2076:	add    %r11,%r8
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:25
-   29a1b2099:	cmpl   $0x4550,(%r8)
-   29a1b20a0:	je     29a1b20b0 <__mingw_enum_import_library_names+0x30>
+   29a1b2079:	cmpl   $0x4550,(%r8)
+   29a1b2080:	je     29a1b2090 <__mingw_enum_import_library_names+0x30>
 __mingw_enum_import_library_names():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:221
-   29a1b20a2:	mov    %r9,%rax
-   29a1b20a5:	ret
-   29a1b20a6:	cs nopw 0x0(%rax,%rax,1)
+   29a1b2082:	mov    %r9,%rax
+   29a1b2085:	ret
+   29a1b2086:	cs nopw 0x0(%rax,%rax,1)
 _ValidateImageBase():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:28
-   29a1b20b0:	cmpw   $0x20b,0x18(%r8)
-   29a1b20b7:	jne    29a1b20a2 <__mingw_enum_import_library_names+0x22>
+   29a1b2090:	cmpw   $0x20b,0x18(%r8)
+   29a1b2097:	jne    29a1b2082 <__mingw_enum_import_library_names+0x22>
 __mingw_enum_import_library_names():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:197
-   29a1b20b9:	mov    0x90(%r8),%eax
+   29a1b2099:	mov    0x90(%r8),%eax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:198
-   29a1b20c0:	test   %eax,%eax
-   29a1b20c2:	je     29a1b20a2 <__mingw_enum_import_library_names+0x22>
+   29a1b20a0:	test   %eax,%eax
+   29a1b20a2:	je     29a1b2082 <__mingw_enum_import_library_names+0x22>
 _FindPESection():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b20c4:	movzwl 0x14(%r8),%edx
+   29a1b20a4:	movzwl 0x14(%r8),%edx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b20c9:	movzwl 0x6(%r8),%r10d
+   29a1b20a9:	movzwl 0x6(%r8),%r10d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:44
-   29a1b20ce:	lea    0x18(%r8,%rdx,1),%rdx
+   29a1b20ae:	lea    0x18(%r8,%rdx,1),%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b20d3:	test   %r10w,%r10w
-   29a1b20d7:	je     29a1b20a2 <__mingw_enum_import_library_names+0x22>
-   29a1b20d9:	lea    -0x1(%r10),%r8d
-   29a1b20dd:	lea    (%r8,%r8,4),%r8
-   29a1b20e1:	lea    0x28(%rdx,%r8,8),%r10
-   29a1b20e6:	cs nopw 0x0(%rax,%rax,1)
+   29a1b20b3:	test   %r10w,%r10w
+   29a1b20b7:	je     29a1b2082 <__mingw_enum_import_library_names+0x22>
+   29a1b20b9:	lea    -0x1(%r10),%r8d
+   29a1b20bd:	lea    (%r8,%r8,4),%r8
+   29a1b20c1:	lea    0x28(%rdx,%r8,8),%r10
+   29a1b20c6:	cs nopw 0x0(%rax,%rax,1)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:48
-   29a1b20f0:	mov    0xc(%rdx),%r9d
-   29a1b20f4:	mov    %r9,%r8
-   29a1b20f7:	cmp    %r9,%rax
-   29a1b20fa:	jb     29a1b2105 <__mingw_enum_import_library_names+0x85>
+   29a1b20d0:	mov    0xc(%rdx),%r9d
+   29a1b20d4:	mov    %r9,%r8
+   29a1b20d7:	cmp    %r9,%rax
+   29a1b20da:	jb     29a1b20e5 <__mingw_enum_import_library_names+0x85>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:49
-   29a1b20fc:	add    0x8(%rdx),%r8d
-   29a1b2100:	cmp    %r8,%rax
-   29a1b2103:	jb     29a1b2118 <__mingw_enum_import_library_names+0x98>
+   29a1b20dc:	add    0x8(%rdx),%r8d
+   29a1b20e0:	cmp    %r8,%rax
+   29a1b20e3:	jb     29a1b20f8 <__mingw_enum_import_library_names+0x98>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:46
-   29a1b2105:	add    $0x28,%rdx
+   29a1b20e5:	add    $0x28,%rdx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:45
-   29a1b2109:	cmp    %rdx,%r10
-   29a1b210c:	jne    29a1b20f0 <__mingw_enum_import_library_names+0x70>
+   29a1b20e9:	cmp    %rdx,%r10
+   29a1b20ec:	jne    29a1b20d0 <__mingw_enum_import_library_names+0x70>
 __mingw_enum_import_library_names():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:193
-   29a1b210e:	xor    %r9d,%r9d
+   29a1b20ee:	xor    %r9d,%r9d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:221
-   29a1b2111:	mov    %r9,%rax
-   29a1b2114:	ret
-   29a1b2115:	nopl   (%rax)
+   29a1b20f1:	mov    %r9,%rax
+   29a1b20f4:	ret
+   29a1b20f5:	nopl   (%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:205
-   29a1b2118:	add    %r11,%rax
+   29a1b20f8:	add    %r11,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:206
-   29a1b211b:	jmp    29a1b2127 <__mingw_enum_import_library_names+0xa7>
-   29a1b211d:	nopl   (%rax)
+   29a1b20fb:	jmp    29a1b2107 <__mingw_enum_import_library_names+0xa7>
+   29a1b20fd:	nopl   (%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:216
-   29a1b2120:	sub    $0x1,%ecx
+   29a1b2100:	sub    $0x1,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:217
-   29a1b2123:	add    $0x14,%rax
+   29a1b2103:	add    $0x14,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:211
-   29a1b2127:	mov    0x4(%rax),%r8d
-   29a1b212b:	test   %r8d,%r8d
-   29a1b212e:	jne    29a1b2137 <__mingw_enum_import_library_names+0xb7>
-   29a1b2130:	mov    0xc(%rax),%edx
-   29a1b2133:	test   %edx,%edx
-   29a1b2135:	je     29a1b210e <__mingw_enum_import_library_names+0x8e>
+   29a1b2107:	mov    0x4(%rax),%r8d
+   29a1b210b:	test   %r8d,%r8d
+   29a1b210e:	jne    29a1b2117 <__mingw_enum_import_library_names+0xb7>
+   29a1b2110:	mov    0xc(%rax),%edx
+   29a1b2113:	test   %edx,%edx
+   29a1b2115:	je     29a1b20ee <__mingw_enum_import_library_names+0x8e>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:214
-   29a1b2137:	test   %ecx,%ecx
-   29a1b2139:	jg     29a1b2120 <__mingw_enum_import_library_names+0xa0>
+   29a1b2117:	test   %ecx,%ecx
+   29a1b2119:	jg     29a1b2100 <__mingw_enum_import_library_names+0xa0>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:215
-   29a1b213b:	mov    0xc(%rax),%r9d
-   29a1b213f:	add    %r11,%r9
+   29a1b211b:	mov    0xc(%rax),%r9d
+   29a1b211f:	add    %r11,%r9
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/pesect.c:221
-   29a1b2142:	mov    %r9,%rax
-   29a1b2145:	ret
-   29a1b2146:	nop
-   29a1b2147:	nop
-   29a1b2148:	nop
-   29a1b2149:	nop
-   29a1b214a:	nop
-   29a1b214b:	nop
-   29a1b214c:	nop
-   29a1b214d:	nop
-   29a1b214e:	nop
-   29a1b214f:	nop
+   29a1b2122:	mov    %r9,%rax
+   29a1b2125:	ret
+   29a1b2126:	nop
+   29a1b2127:	nop
+   29a1b2128:	nop
+   29a1b2129:	nop
+   29a1b212a:	nop
+   29a1b212b:	nop
+   29a1b212c:	nop
+   29a1b212d:	nop
+   29a1b212e:	nop
+   29a1b212f:	nop
 
-000000029a1b2150 <_fpreset>:
+000000029a1b2130 <_fpreset>:
 _fpreset():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/CRT_fp10.c:19
-   29a1b2150:	fninit
+   29a1b2130:	fninit
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/CRT_fp10.c:24
-   29a1b2152:	ret
-   29a1b2153:	nop
-   29a1b2154:	nop
-   29a1b2155:	nop
-   29a1b2156:	nop
-   29a1b2157:	nop
-   29a1b2158:	nop
-   29a1b2159:	nop
-   29a1b215a:	nop
-   29a1b215b:	nop
-   29a1b215c:	nop
-   29a1b215d:	nop
-   29a1b215e:	nop
-   29a1b215f:	nop
-
-000000029a1b2160 <___chkstk_ms>:
-   29a1b2160:	push   %rcx
-   29a1b2161:	push   %rax
-   29a1b2162:	cmp    $0x1000,%rax
-   29a1b2168:	lea    0x18(%rsp),%rcx
-   29a1b216d:	jb     29a1b2188 <___chkstk_ms+0x28>
-   29a1b216f:	sub    $0x1000,%rcx
-   29a1b2176:	orq    $0x0,(%rcx)
-   29a1b217a:	sub    $0x1000,%rax
-   29a1b2180:	cmp    $0x1000,%rax
-   29a1b2186:	ja     29a1b216f <___chkstk_ms+0xf>
-   29a1b2188:	sub    %rax,%rcx
-   29a1b218b:	orq    $0x0,(%rcx)
-   29a1b218f:	pop    %rax
-   29a1b2190:	pop    %rcx
-   29a1b2191:	ret
-   29a1b2192:	nop
-   29a1b2193:	nop
-   29a1b2194:	nop
-   29a1b2195:	nop
+   29a1b2132:	ret
+   29a1b2133:	nop
+   29a1b2134:	nop
+   29a1b2135:	nop
+   29a1b2136:	nop
+   29a1b2137:	nop
+   29a1b2138:	nop
+   29a1b2139:	nop
+   29a1b213a:	nop
+   29a1b213b:	nop
+   29a1b213c:	nop
+   29a1b213d:	nop
+   29a1b213e:	nop
+   29a1b213f:	nop
+
+000000029a1b2140 <___chkstk_ms>:
+   29a1b2140:	push   %rcx
+   29a1b2141:	push   %rax
+   29a1b2142:	cmp    $0x1000,%rax
+   29a1b2148:	lea    0x18(%rsp),%rcx
+   29a1b214d:	jb     29a1b2168 <___chkstk_ms+0x28>
+   29a1b214f:	sub    $0x1000,%rcx
+   29a1b2156:	orq    $0x0,(%rcx)
+   29a1b215a:	sub    $0x1000,%rax
+   29a1b2160:	cmp    $0x1000,%rax
+   29a1b2166:	ja     29a1b214f <___chkstk_ms+0xf>
+   29a1b2168:	sub    %rax,%rcx
+   29a1b216b:	orq    $0x0,(%rcx)
+   29a1b216f:	pop    %rax
+   29a1b2170:	pop    %rcx
+   29a1b2171:	ret
+   29a1b2172:	nop
+   29a1b2173:	nop
+   29a1b2174:	nop
+   29a1b2175:	nop
+   29a1b2176:	nop
+   29a1b2177:	nop
+   29a1b2178:	nop
+   29a1b2179:	nop
+   29a1b217a:	nop
+   29a1b217b:	nop
+   29a1b217c:	nop
+   29a1b217d:	nop
+   29a1b217e:	nop
+   29a1b217f:	nop
+
+000000029a1b2180 <DllEntryPoint>:
+DllEntryPoint():
+C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/dllentry.c:18
+   29a1b2180:	mov    $0x1,%eax
+   29a1b2185:	ret
+   29a1b2186:	nop
+   29a1b2187:	nop
+   29a1b2188:	nop
+   29a1b2189:	nop
+   29a1b218a:	nop
+   29a1b218b:	nop
+   29a1b218c:	nop
+   29a1b218d:	nop
+   29a1b218e:	nop
+   29a1b218f:	nop
+
+000000029a1b2190 <DllMain>:
+DllMain():
+C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/dllmain.c:10
+   29a1b2190:	mov    $0x1,%eax
+   29a1b2195:	ret
    29a1b2196:	nop
    29a1b2197:	nop
    29a1b2198:	nop
    29a1b2199:	nop
    29a1b219a:	nop
    29a1b219b:	nop
    29a1b219c:	nop
    29a1b219d:	nop
    29a1b219e:	nop
    29a1b219f:	nop
 
-000000029a1b21a0 <DllEntryPoint>:
-DllEntryPoint():
-C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/dllentry.c:18
-   29a1b21a0:	mov    $0x1,%eax
-   29a1b21a5:	ret
-   29a1b21a6:	nop
-   29a1b21a7:	nop
-   29a1b21a8:	nop
-   29a1b21a9:	nop
-   29a1b21aa:	nop
-   29a1b21ab:	nop
-   29a1b21ac:	nop
-   29a1b21ad:	nop
-   29a1b21ae:	nop
-   29a1b21af:	nop
-
-000000029a1b21b0 <DllMain>:
-DllMain():
-C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/dllmain.c:10
-   29a1b21b0:	mov    $0x1,%eax
-   29a1b21b5:	ret
-   29a1b21b6:	nop
-   29a1b21b7:	nop
-   29a1b21b8:	nop
-   29a1b21b9:	nop
-   29a1b21ba:	nop
-   29a1b21bb:	nop
-   29a1b21bc:	nop
-   29a1b21bd:	nop
-   29a1b21be:	nop
-   29a1b21bf:	nop
-
-000000029a1b21c0 <vfprintf>:
+000000029a1b21a0 <vfprintf>:
 vfprintf():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_vfprintf.c:12
-   29a1b21c0:	sub    $0x38,%rsp
+   29a1b21a0:	sub    $0x38,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_vfprintf.c:13
-   29a1b21c4:	xor    %r9d,%r9d
-   29a1b21c7:	mov    %r8,0x20(%rsp)
-   29a1b21cc:	mov    %rdx,%r8
-   29a1b21cf:	mov    %rcx,%rdx
-   29a1b21d2:	xor    %ecx,%ecx
-   29a1b21d4:	call   29a1b2438 <__stdio_common_vfprintf>
+   29a1b21a4:	xor    %r9d,%r9d
+   29a1b21a7:	mov    %r8,0x20(%rsp)
+   29a1b21ac:	mov    %rdx,%r8
+   29a1b21af:	mov    %rcx,%rdx
+   29a1b21b2:	xor    %ecx,%ecx
+   29a1b21b4:	call   29a1b2418 <__stdio_common_vfprintf>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_vfprintf.c:14
-   29a1b21d9:	add    $0x38,%rsp
-   29a1b21dd:	ret
-   29a1b21de:	nop
-   29a1b21df:	nop
+   29a1b21b9:	add    $0x38,%rsp
+   29a1b21bd:	ret
+   29a1b21be:	nop
+   29a1b21bf:	nop
 
-000000029a1b21e0 <_get_output_format>:
+000000029a1b21c0 <_get_output_format>:
 _get_output_format():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:113
-   29a1b21e0:	xor    %eax,%eax
-   29a1b21e2:	ret
-   29a1b21e3:	data16 cs nopw 0x0(%rax,%rax,1)
-   29a1b21ee:	xchg   %ax,%ax
+   29a1b21c0:	xor    %eax,%eax
+   29a1b21c2:	ret
+   29a1b21c3:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b21ce:	xchg   %ax,%ax
 
-000000029a1b21f0 <__getmainargs>:
+000000029a1b21d0 <__getmainargs>:
 __getmainargs():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:63
-   29a1b21f0:	push   %r12
-   29a1b21f2:	push   %rbp
-   29a1b21f3:	push   %rdi
-   29a1b21f4:	push   %rsi
-   29a1b21f5:	push   %rbx
-   29a1b21f6:	sub    $0x20,%rsp
-   29a1b21fa:	mov    0x70(%rsp),%r12
-   29a1b21ff:	mov    %r9d,%ebp
-   29a1b2202:	mov    %rdx,%rsi
-   29a1b2205:	mov    %r8,%rbx
-   29a1b2208:	mov    %rcx,%rdi
+   29a1b21d0:	push   %r12
+   29a1b21d2:	push   %rbp
+   29a1b21d3:	push   %rdi
+   29a1b21d4:	push   %rsi
+   29a1b21d5:	push   %rbx
+   29a1b21d6:	sub    $0x20,%rsp
+   29a1b21da:	mov    0x70(%rsp),%r12
+   29a1b21df:	mov    %r9d,%ebp
+   29a1b21e2:	mov    %rdx,%rsi
+   29a1b21e5:	mov    %r8,%rbx
+   29a1b21e8:	mov    %rcx,%rdi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:64
-   29a1b220b:	call   29a1b24b8 <_initialize_narrow_environment>
+   29a1b21eb:	call   29a1b2488 <_initialize_narrow_environment>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:65
-   29a1b2210:	cmp    $0x1,%ebp
-   29a1b2213:	mov    $0x1,%ecx
-   29a1b2218:	sbb    $0xffffffff,%ecx
-   29a1b221b:	call   29a1b2488 <_configure_narrow_argv>
+   29a1b21f0:	cmp    $0x1,%ebp
+   29a1b21f3:	mov    $0x1,%ecx
+   29a1b21f8:	sbb    $0xffffffff,%ecx
+   29a1b21fb:	call   29a1b2458 <_configure_narrow_argv>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:66
-   29a1b2220:	call   29a1b2470 <__p___argc>
-   29a1b2225:	mov    (%rax),%eax
-   29a1b2227:	mov    %eax,(%rdi)
+   29a1b2200:	call   29a1b2440 <__p___argc>
+   29a1b2205:	mov    (%rax),%eax
+   29a1b2207:	mov    %eax,(%rdi)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:67
-   29a1b2229:	call   29a1b2478 <__p___argv>
-   29a1b222e:	mov    (%rax),%rax
-   29a1b2231:	mov    %rax,(%rsi)
+   29a1b2209:	call   29a1b2448 <__p___argv>
+   29a1b220e:	mov    (%rax),%rax
+   29a1b2211:	mov    %rax,(%rsi)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:68
-   29a1b2234:	call   29a1b2510 <__p__environ>
-   29a1b2239:	mov    (%rax),%rax
-   29a1b223c:	mov    %rax,(%rbx)
+   29a1b2214:	call   29a1b24e0 <__p__environ>
+   29a1b2219:	mov    (%rax),%rax
+   29a1b221c:	mov    %rax,(%rbx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:69
-   29a1b223f:	test   %r12,%r12
-   29a1b2242:	je     29a1b224d <__getmainargs+0x5d>
+   29a1b221f:	test   %r12,%r12
+   29a1b2222:	je     29a1b222d <__getmainargs+0x5d>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:70
-   29a1b2244:	mov    (%r12),%ecx
-   29a1b2248:	call   29a1b24f0 <_set_new_mode>
+   29a1b2224:	mov    (%r12),%ecx
+   29a1b2228:	call   29a1b24c0 <_set_new_mode>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:72
-   29a1b224d:	xor    %eax,%eax
-   29a1b224f:	add    $0x20,%rsp
-   29a1b2253:	pop    %rbx
-   29a1b2254:	pop    %rsi
-   29a1b2255:	pop    %rdi
-   29a1b2256:	pop    %rbp
-   29a1b2257:	pop    %r12
-   29a1b2259:	ret
-   29a1b225a:	nopw   0x0(%rax,%rax,1)
+   29a1b222d:	xor    %eax,%eax
+   29a1b222f:	add    $0x20,%rsp
+   29a1b2233:	pop    %rbx
+   29a1b2234:	pop    %rsi
+   29a1b2235:	pop    %rdi
+   29a1b2236:	pop    %rbp
+   29a1b2237:	pop    %r12
+   29a1b2239:	ret
+   29a1b223a:	nopw   0x0(%rax,%rax,1)
 
-000000029a1b2260 <__wgetmainargs>:
+000000029a1b2240 <__wgetmainargs>:
 __wgetmainargs():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:75
-   29a1b2260:	push   %r12
-   29a1b2262:	push   %rbp
-   29a1b2263:	push   %rdi
-   29a1b2264:	push   %rsi
-   29a1b2265:	push   %rbx
-   29a1b2266:	sub    $0x20,%rsp
-   29a1b226a:	mov    0x70(%rsp),%r12
-   29a1b226f:	mov    %r9d,%ebp
-   29a1b2272:	mov    %rdx,%rsi
-   29a1b2275:	mov    %r8,%rbx
-   29a1b2278:	mov    %rcx,%rdi
+   29a1b2240:	push   %r12
+   29a1b2242:	push   %rbp
+   29a1b2243:	push   %rdi
+   29a1b2244:	push   %rsi
+   29a1b2245:	push   %rbx
+   29a1b2246:	sub    $0x20,%rsp
+   29a1b224a:	mov    0x70(%rsp),%r12
+   29a1b224f:	mov    %r9d,%ebp
+   29a1b2252:	mov    %rdx,%rsi
+   29a1b2255:	mov    %r8,%rbx
+   29a1b2258:	mov    %rcx,%rdi
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:76
-   29a1b227b:	call   29a1b24c8 <_initialize_wide_environment>
+   29a1b225b:	call   29a1b2498 <_initialize_wide_environment>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:77
-   29a1b2280:	cmp    $0x1,%ebp
-   29a1b2283:	mov    $0x1,%ecx
-   29a1b2288:	sbb    $0xffffffff,%ecx
-   29a1b228b:	call   29a1b2490 <_configure_wide_argv>
+   29a1b2260:	cmp    $0x1,%ebp
+   29a1b2263:	mov    $0x1,%ecx
+   29a1b2268:	sbb    $0xffffffff,%ecx
+   29a1b226b:	call   29a1b2460 <_configure_wide_argv>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:78
-   29a1b2290:	call   29a1b2470 <__p___argc>
-   29a1b2295:	mov    (%rax),%eax
-   29a1b2297:	mov    %eax,(%rdi)
+   29a1b2270:	call   29a1b2440 <__p___argc>
+   29a1b2275:	mov    (%rax),%eax
+   29a1b2277:	mov    %eax,(%rdi)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:79
-   29a1b2299:	call   29a1b2480 <__p___wargv>
-   29a1b229e:	mov    (%rax),%rax
-   29a1b22a1:	mov    %rax,(%rsi)
+   29a1b2279:	call   29a1b2450 <__p___wargv>
+   29a1b227e:	mov    (%rax),%rax
+   29a1b2281:	mov    %rax,(%rsi)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:80
-   29a1b22a4:	call   29a1b2518 <__p__wenviron>
-   29a1b22a9:	mov    (%rax),%rax
-   29a1b22ac:	mov    %rax,(%rbx)
+   29a1b2284:	call   29a1b24e8 <__p__wenviron>
+   29a1b2289:	mov    (%rax),%rax
+   29a1b228c:	mov    %rax,(%rbx)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:81
-   29a1b22af:	test   %r12,%r12
-   29a1b22b2:	je     29a1b22bd <__wgetmainargs+0x5d>
+   29a1b228f:	test   %r12,%r12
+   29a1b2292:	je     29a1b229d <__wgetmainargs+0x5d>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:82
-   29a1b22b4:	mov    (%r12),%ecx
-   29a1b22b8:	call   29a1b24f0 <_set_new_mode>
+   29a1b2294:	mov    (%r12),%ecx
+   29a1b2298:	call   29a1b24c0 <_set_new_mode>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:84
-   29a1b22bd:	xor    %eax,%eax
-   29a1b22bf:	add    $0x20,%rsp
-   29a1b22c3:	pop    %rbx
-   29a1b22c4:	pop    %rsi
-   29a1b22c5:	pop    %rdi
-   29a1b22c6:	pop    %rbp
-   29a1b22c7:	pop    %r12
-   29a1b22c9:	ret
-   29a1b22ca:	nopw   0x0(%rax,%rax,1)
+   29a1b229d:	xor    %eax,%eax
+   29a1b229f:	add    $0x20,%rsp
+   29a1b22a3:	pop    %rbx
+   29a1b22a4:	pop    %rsi
+   29a1b22a5:	pop    %rdi
+   29a1b22a6:	pop    %rbp
+   29a1b22a7:	pop    %r12
+   29a1b22a9:	ret
+   29a1b22aa:	nopw   0x0(%rax,%rax,1)
 
-000000029a1b22d0 <_onexit>:
+000000029a1b22b0 <_onexit>:
 _onexit():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:87
-   29a1b22d0:	push   %rbx
-   29a1b22d1:	sub    $0x20,%rsp
-   29a1b22d5:	mov    %rcx,%rbx
+   29a1b22b0:	push   %rbx
+   29a1b22b1:	sub    $0x20,%rsp
+   29a1b22b5:	mov    %rcx,%rbx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:88
-   29a1b22d8:	call   29a1b24a0 <_crt_atexit>
-   29a1b22dd:	test   %eax,%eax
-   29a1b22df:	mov    $0x0,%eax
-   29a1b22e4:	cmove  %rbx,%rax
+   29a1b22b8:	call   29a1b2470 <_crt_atexit>
+   29a1b22bd:	test   %eax,%eax
+   29a1b22bf:	mov    $0x0,%eax
+   29a1b22c4:	cmove  %rbx,%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:89
-   29a1b22e8:	add    $0x20,%rsp
-   29a1b22ec:	pop    %rbx
-   29a1b22ed:	ret
-   29a1b22ee:	xchg   %ax,%ax
+   29a1b22c8:	add    $0x20,%rsp
+   29a1b22cc:	pop    %rbx
+   29a1b22cd:	ret
+   29a1b22ce:	xchg   %ax,%ax
 
-000000029a1b22f0 <at_quick_exit>:
+000000029a1b22d0 <at_quick_exit>:
 at_quick_exit():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:98
-   29a1b22f0:	mov    0x1f69(%rip),%rax        # 29a1b4260 <.refptr.__mingw_module_is_dll>
-   29a1b22f7:	cmpb   $0x0,(%rax)
-   29a1b22fa:	je     29a1b2300 <at_quick_exit+0x10>
+   29a1b22d0:	mov    0x1f89(%rip),%rax        # 29a1b4260 <.refptr.__mingw_module_is_dll>
+   29a1b22d7:	cmpb   $0x0,(%rax)
+   29a1b22da:	je     29a1b22e0 <at_quick_exit+0x10>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:101
-   29a1b22fc:	xor    %eax,%eax
-   29a1b22fe:	ret
-   29a1b22ff:	nop
+   29a1b22dc:	xor    %eax,%eax
+   29a1b22de:	ret
+   29a1b22df:	nop
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:100
-   29a1b2300:	jmp    29a1b2498 <_crt_at_quick_exit>
-   29a1b2305:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b22e0:	jmp    29a1b2468 <_crt_at_quick_exit>
+   29a1b22e5:	data16 cs nopw 0x0(%rax,%rax,1)
 
-000000029a1b2310 <_amsg_exit>:
+000000029a1b22f0 <_amsg_exit>:
 _amsg_exit():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:105
-   29a1b2310:	push   %rbx
-   29a1b2311:	sub    $0x20,%rsp
-   29a1b2315:	mov    %ecx,%ebx
+   29a1b22f0:	push   %rbx
+   29a1b22f1:	sub    $0x20,%rsp
+   29a1b22f5:	mov    %ecx,%ebx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:106
-   29a1b2317:	mov    $0x2,%ecx
-   29a1b231c:	call   29a1b2430 <__acrt_iob_func>
-   29a1b2321:	mov    %ebx,%r8d
-   29a1b2324:	lea    0x1e95(%rip),%rdx        # 29a1b41c0 <.rdata>
-   29a1b232b:	mov    %rax,%rcx
-   29a1b232e:	call   29a1b2530 <fprintf>
+   29a1b22f7:	mov    $0x2,%ecx
+   29a1b22fc:	call   29a1b2410 <__acrt_iob_func>
+   29a1b2301:	mov    %ebx,%r8d
+   29a1b2304:	lea    0x1eb5(%rip),%rdx        # 29a1b41c0 <.rdata>
+   29a1b230b:	mov    %rax,%rcx
+   29a1b230e:	call   29a1b2500 <fprintf>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:107
-   29a1b2333:	mov    $0xff,%ecx
-   29a1b2338:	call   29a1b24b0 <_exit>
-   29a1b233d:	nop
-   29a1b233e:	xchg   %ax,%ax
+   29a1b2313:	mov    $0xff,%ecx
+   29a1b2318:	call   29a1b2480 <_exit>
+   29a1b231d:	nop
+   29a1b231e:	xchg   %ax,%ax
 
-000000029a1b2340 <__ms_fwprintf>:
+000000029a1b2320 <__ms_fwprintf>:
 __ms_fwprintf():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:151
-   29a1b2340:	sub    $0x48,%rsp
+   29a1b2320:	sub    $0x48,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:154
-   29a1b2344:	lea    0x60(%rsp),%rax
+   29a1b2324:	lea    0x60(%rsp),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:151
-   29a1b2349:	mov    %r8,0x60(%rsp)
+   29a1b2329:	mov    %r8,0x60(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:155
-   29a1b234e:	mov    %rdx,%r8
-   29a1b2351:	mov    %rcx,%rdx
-   29a1b2354:	mov    %rax,0x20(%rsp)
-   29a1b2359:	mov    $0x4,%ecx
+   29a1b232e:	mov    %rdx,%r8
+   29a1b2331:	mov    %rcx,%rdx
+   29a1b2334:	mov    %rax,0x20(%rsp)
+   29a1b2339:	mov    $0x4,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:151
-   29a1b235e:	mov    %r9,0x68(%rsp)
+   29a1b233e:	mov    %r9,0x68(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:155
-   29a1b2363:	xor    %r9d,%r9d
+   29a1b2343:	xor    %r9d,%r9d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:154
-   29a1b2366:	mov    %rax,0x38(%rsp)
+   29a1b2346:	mov    %rax,0x38(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:155
-   29a1b236b:	call   29a1b2440 <__stdio_common_vfwprintf>
+   29a1b234b:	call   29a1b2420 <__stdio_common_vfwprintf>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:158
-   29a1b2370:	add    $0x48,%rsp
-   29a1b2374:	ret
-   29a1b2375:	data16 cs nopw 0x0(%rax,%rax,1)
+   29a1b2350:	add    $0x48,%rsp
+   29a1b2354:	ret
+   29a1b2355:	data16 cs nopw 0x0(%rax,%rax,1)
 
-000000029a1b2380 <tzset>:
+000000029a1b2360 <tzset>:
 tzset():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:144
-   29a1b2380:	sub    $0x28,%rsp
+   29a1b2360:	sub    $0x28,%rsp
 _tzset():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:135
-   29a1b2384:	mov    0x1eb5(%rip),%rax        # 29a1b4240 <.refptr.__imp__tzset>
-   29a1b238b:	call   *(%rax)
+   29a1b2364:	mov    0x1ed5(%rip),%rax        # 29a1b4240 <.refptr.__imp__tzset>
+   29a1b236b:	call   *(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:138
-   29a1b238d:	call   29a1b2410 <__tzname>
-   29a1b2392:	mov    %rax,0xcf7(%rip)        # 29a1b3090 <__imp_tzname>
+   29a1b236d:	call   29a1b23f0 <__tzname>
+   29a1b2372:	mov    %rax,0xd17(%rip)        # 29a1b3090 <__imp_tzname>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:139
-   29a1b2399:	call   29a1b2408 <__timezone>
-   29a1b239e:	mov    %rax,0xce3(%rip)        # 29a1b3088 <__imp_timezone>
+   29a1b2379:	call   29a1b23e8 <__timezone>
+   29a1b237e:	mov    %rax,0xd03(%rip)        # 29a1b3088 <__imp_timezone>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:140
-   29a1b23a5:	call   29a1b2400 <__daylight>
-   29a1b23aa:	mov    %rax,0xccf(%rip)        # 29a1b3080 <__imp_daylight>
+   29a1b2385:	call   29a1b23e0 <__daylight>
+   29a1b238a:	mov    %rax,0xcef(%rip)        # 29a1b3080 <__imp_daylight>
 tzset():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:146
-   29a1b23b1:	add    $0x28,%rsp
-   29a1b23b5:	ret
-   29a1b23b6:	cs nopw 0x0(%rax,%rax,1)
+   29a1b2391:	add    $0x28,%rsp
+   29a1b2395:	ret
+   29a1b2396:	cs nopw 0x0(%rax,%rax,1)
 
-000000029a1b23c0 <_tzset>:
+000000029a1b23a0 <_tzset>:
 _tzset():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:134
-   29a1b23c0:	sub    $0x28,%rsp
+   29a1b23a0:	sub    $0x28,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:135
-   29a1b23c4:	mov    0x1e75(%rip),%rax        # 29a1b4240 <.refptr.__imp__tzset>
-   29a1b23cb:	call   *(%rax)
+   29a1b23a4:	mov    0x1e95(%rip),%rax        # 29a1b4240 <.refptr.__imp__tzset>
+   29a1b23ab:	call   *(%rax)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:138
-   29a1b23cd:	call   29a1b2410 <__tzname>
-   29a1b23d2:	mov    %rax,0xcb7(%rip)        # 29a1b3090 <__imp_tzname>
+   29a1b23ad:	call   29a1b23f0 <__tzname>
+   29a1b23b2:	mov    %rax,0xcd7(%rip)        # 29a1b3090 <__imp_tzname>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:139
-   29a1b23d9:	call   29a1b2408 <__timezone>
-   29a1b23de:	mov    %rax,0xca3(%rip)        # 29a1b3088 <__imp_timezone>
+   29a1b23b9:	call   29a1b23e8 <__timezone>
+   29a1b23be:	mov    %rax,0xcc3(%rip)        # 29a1b3088 <__imp_timezone>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:140
-   29a1b23e5:	call   29a1b2400 <__daylight>
-   29a1b23ea:	mov    %rax,0xc8f(%rip)        # 29a1b3080 <__imp_daylight>
+   29a1b23c5:	call   29a1b23e0 <__daylight>
+   29a1b23ca:	mov    %rax,0xcaf(%rip)        # 29a1b3080 <__imp_daylight>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:141
-   29a1b23f1:	add    $0x28,%rsp
-   29a1b23f5:	ret
+   29a1b23d1:	add    $0x28,%rsp
+   29a1b23d5:	ret
+   29a1b23d6:	nop
+   29a1b23d7:	nop
+   29a1b23d8:	nop
+   29a1b23d9:	nop
+   29a1b23da:	nop
+   29a1b23db:	nop
+   29a1b23dc:	nop
+   29a1b23dd:	nop
+   29a1b23de:	nop
+   29a1b23df:	nop
+
+000000029a1b23e0 <__daylight>:
+   29a1b23e0:	jmp    *0x6fca(%rip)        # 29a1b93b0 <__imp___daylight>
+   29a1b23e6:	nop
+   29a1b23e7:	nop
+
+000000029a1b23e8 <__timezone>:
+   29a1b23e8:	jmp    *0x6fca(%rip)        # 29a1b93b8 <__imp___timezone>
+   29a1b23ee:	nop
+   29a1b23ef:	nop
+
+000000029a1b23f0 <__tzname>:
+   29a1b23f0:	jmp    *0x6fca(%rip)        # 29a1b93c0 <__imp___tzname>
    29a1b23f6:	nop
    29a1b23f7:	nop
-   29a1b23f8:	nop
-   29a1b23f9:	nop
-   29a1b23fa:	nop
-   29a1b23fb:	nop
-   29a1b23fc:	nop
-   29a1b23fd:	nop
-   29a1b23fe:	nop
-   29a1b23ff:	nop
 
-000000029a1b2400 <__daylight>:
-   29a1b2400:	jmp    *0x6fba(%rip)        # 29a1b93c0 <__imp___daylight>
+000000029a1b23f8 <.text>:
+   29a1b23f8:	nopl   0x0(%rax,%rax,1)
+
+000000029a1b2400 <strlen>:
+   29a1b2400:	jmp    *0x6f92(%rip)        # 29a1b9398 <__imp_strlen>
    29a1b2406:	nop
    29a1b2407:	nop
 
-000000029a1b2408 <__timezone>:
-   29a1b2408:	jmp    *0x6fba(%rip)        # 29a1b93c8 <__imp___timezone>
+000000029a1b2408 <strncmp>:
+   29a1b2408:	jmp    *0x6f92(%rip)        # 29a1b93a0 <__imp_strncmp>
    29a1b240e:	nop
    29a1b240f:	nop
 
-000000029a1b2410 <__tzname>:
-   29a1b2410:	jmp    *0x6fba(%rip)        # 29a1b93d0 <__imp___tzname>
+000000029a1b2410 <__acrt_iob_func>:
+   29a1b2410:	jmp    *0x6f4a(%rip)        # 29a1b9360 <__imp___acrt_iob_func>
    29a1b2416:	nop
    29a1b2417:	nop
 
-000000029a1b2418 <.text>:
-   29a1b2418:	nopl   0x0(%rax,%rax,1)
+000000029a1b2418 <__stdio_common_vfprintf>:
+   29a1b2418:	jmp    *0x6f4a(%rip)        # 29a1b9368 <__imp___stdio_common_vfprintf>
+   29a1b241e:	nop
+   29a1b241f:	nop
 
-000000029a1b2420 <strlen>:
-   29a1b2420:	jmp    *0x6f82(%rip)        # 29a1b93a8 <__imp_strlen>
+000000029a1b2420 <__stdio_common_vfwprintf>:
+   29a1b2420:	jmp    *0x6f4a(%rip)        # 29a1b9370 <__imp___stdio_common_vfwprintf>
    29a1b2426:	nop
    29a1b2427:	nop
 
-000000029a1b2428 <strncmp>:
-   29a1b2428:	jmp    *0x6f82(%rip)        # 29a1b93b0 <__imp_strncmp>
+000000029a1b2428 <kbhit>:
+   29a1b2428:	jmp    *0x6f4a(%rip)        # 29a1b9378 <__imp_kbhit>
    29a1b242e:	nop
    29a1b242f:	nop
 
-000000029a1b2430 <__acrt_iob_func>:
-   29a1b2430:	jmp    *0x6f32(%rip)        # 29a1b9368 <__imp___acrt_iob_func>
+000000029a1b2430 <fwrite>:
+   29a1b2430:	jmp    *0x6f4a(%rip)        # 29a1b9380 <__imp_fwrite>
    29a1b2436:	nop
    29a1b2437:	nop
 
-000000029a1b2438 <__stdio_common_vfprintf>:
-   29a1b2438:	jmp    *0x6f32(%rip)        # 29a1b9370 <__imp___stdio_common_vfprintf>
+000000029a1b2438 <putchar>:
+   29a1b2438:	jmp    *0x6f4a(%rip)        # 29a1b9388 <__imp_putchar>
    29a1b243e:	nop
    29a1b243f:	nop
 
-000000029a1b2440 <__stdio_common_vfwprintf>:
-   29a1b2440:	jmp    *0x6f32(%rip)        # 29a1b9378 <__imp___stdio_common_vfwprintf>
+000000029a1b2440 <__p___argc>:
+   29a1b2440:	jmp    *0x6e9a(%rip)        # 29a1b92e0 <__imp___p___argc>
    29a1b2446:	nop
    29a1b2447:	nop
 
-000000029a1b2448 <kbhit>:
-   29a1b2448:	jmp    *0x6f32(%rip)        # 29a1b9380 <__imp_kbhit>
+000000029a1b2448 <__p___argv>:
+   29a1b2448:	jmp    *0x6e9a(%rip)        # 29a1b92e8 <__imp___p___argv>
    29a1b244e:	nop
    29a1b244f:	nop
 
-000000029a1b2450 <fflush>:
-   29a1b2450:	jmp    *0x6f32(%rip)        # 29a1b9388 <__imp_fflush>
+000000029a1b2450 <__p___wargv>:
+   29a1b2450:	jmp    *0x6e9a(%rip)        # 29a1b92f0 <__imp___p___wargv>
    29a1b2456:	nop
    29a1b2457:	nop
 
-000000029a1b2458 <fwrite>:
-   29a1b2458:	jmp    *0x6f32(%rip)        # 29a1b9390 <__imp_fwrite>
+000000029a1b2458 <_configure_narrow_argv>:
+   29a1b2458:	jmp    *0x6e9a(%rip)        # 29a1b92f8 <__imp__configure_narrow_argv>
    29a1b245e:	nop
    29a1b245f:	nop
 
-000000029a1b2460 <putchar>:
-   29a1b2460:	jmp    *0x6f32(%rip)        # 29a1b9398 <__imp_putchar>
+000000029a1b2460 <_configure_wide_argv>:
+   29a1b2460:	jmp    *0x6e9a(%rip)        # 29a1b9300 <__imp__configure_wide_argv>
    29a1b2466:	nop
    29a1b2467:	nop
-   29a1b2468:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b2470 <__p___argc>:
-   29a1b2470:	jmp    *0x6e72(%rip)        # 29a1b92e8 <__imp___p___argc>
+000000029a1b2468 <_crt_at_quick_exit>:
+   29a1b2468:	jmp    *0x6e9a(%rip)        # 29a1b9308 <__imp__crt_at_quick_exit>
+   29a1b246e:	nop
+   29a1b246f:	nop
+
+000000029a1b2470 <_crt_atexit>:
+   29a1b2470:	jmp    *0x6e9a(%rip)        # 29a1b9310 <__imp__crt_atexit>
    29a1b2476:	nop
    29a1b2477:	nop
 
-000000029a1b2478 <__p___argv>:
-   29a1b2478:	jmp    *0x6e72(%rip)        # 29a1b92f0 <__imp___p___argv>
+000000029a1b2478 <_execute_onexit_table>:
+   29a1b2478:	jmp    *0x6e9a(%rip)        # 29a1b9318 <__imp__execute_onexit_table>
    29a1b247e:	nop
    29a1b247f:	nop
 
-000000029a1b2480 <__p___wargv>:
-   29a1b2480:	jmp    *0x6e72(%rip)        # 29a1b92f8 <__imp___p___wargv>
+000000029a1b2480 <_exit>:
+   29a1b2480:	jmp    *0x6e9a(%rip)        # 29a1b9320 <__imp__exit>
    29a1b2486:	nop
    29a1b2487:	nop
 
-000000029a1b2488 <_configure_narrow_argv>:
-   29a1b2488:	jmp    *0x6e72(%rip)        # 29a1b9300 <__imp__configure_narrow_argv>
+000000029a1b2488 <_initialize_narrow_environment>:
+   29a1b2488:	jmp    *0x6e9a(%rip)        # 29a1b9328 <__imp__initialize_narrow_environment>
    29a1b248e:	nop
    29a1b248f:	nop
 
-000000029a1b2490 <_configure_wide_argv>:
-   29a1b2490:	jmp    *0x6e72(%rip)        # 29a1b9308 <__imp__configure_wide_argv>
+000000029a1b2490 <_initialize_onexit_table>:
+   29a1b2490:	jmp    *0x6e9a(%rip)        # 29a1b9330 <__imp__initialize_onexit_table>
    29a1b2496:	nop
    29a1b2497:	nop
 
-000000029a1b2498 <_crt_at_quick_exit>:
-   29a1b2498:	jmp    *0x6e72(%rip)        # 29a1b9310 <__imp__crt_at_quick_exit>
+000000029a1b2498 <_initialize_wide_environment>:
+   29a1b2498:	jmp    *0x6e9a(%rip)        # 29a1b9338 <__imp__initialize_wide_environment>
    29a1b249e:	nop
    29a1b249f:	nop
 
-000000029a1b24a0 <_crt_atexit>:
-   29a1b24a0:	jmp    *0x6e72(%rip)        # 29a1b9318 <__imp__crt_atexit>
+000000029a1b24a0 <_initterm>:
+   29a1b24a0:	jmp    *0x6e9a(%rip)        # 29a1b9340 <__imp__initterm>
    29a1b24a6:	nop
    29a1b24a7:	nop
 
-000000029a1b24a8 <_execute_onexit_table>:
-   29a1b24a8:	jmp    *0x6e72(%rip)        # 29a1b9320 <__imp__execute_onexit_table>
+000000029a1b24a8 <_register_onexit_function>:
+   29a1b24a8:	jmp    *0x6e9a(%rip)        # 29a1b9348 <__imp__register_onexit_function>
    29a1b24ae:	nop
    29a1b24af:	nop
 
-000000029a1b24b0 <_exit>:
-   29a1b24b0:	jmp    *0x6e72(%rip)        # 29a1b9328 <__imp__exit>
+000000029a1b24b0 <abort>:
+   29a1b24b0:	jmp    *0x6e9a(%rip)        # 29a1b9350 <__imp_abort>
    29a1b24b6:	nop
    29a1b24b7:	nop
+   29a1b24b8:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b24b8 <_initialize_narrow_environment>:
-   29a1b24b8:	jmp    *0x6e72(%rip)        # 29a1b9330 <__imp__initialize_narrow_environment>
-   29a1b24be:	nop
-   29a1b24bf:	nop
-
-000000029a1b24c0 <_initialize_onexit_table>:
-   29a1b24c0:	jmp    *0x6e72(%rip)        # 29a1b9338 <__imp__initialize_onexit_table>
+000000029a1b24c0 <_set_new_mode>:
+   29a1b24c0:	jmp    *0x6dfa(%rip)        # 29a1b92c0 <__imp__set_new_mode>
    29a1b24c6:	nop
    29a1b24c7:	nop
 
-000000029a1b24c8 <_initialize_wide_environment>:
-   29a1b24c8:	jmp    *0x6e72(%rip)        # 29a1b9340 <__imp__initialize_wide_environment>
+000000029a1b24c8 <calloc>:
+   29a1b24c8:	jmp    *0x6dfa(%rip)        # 29a1b92c8 <__imp_calloc>
    29a1b24ce:	nop
    29a1b24cf:	nop
 
-000000029a1b24d0 <_initterm>:
-   29a1b24d0:	jmp    *0x6e72(%rip)        # 29a1b9348 <__imp__initterm>
+000000029a1b24d0 <free>:
+   29a1b24d0:	jmp    *0x6dfa(%rip)        # 29a1b92d0 <__imp_free>
    29a1b24d6:	nop
    29a1b24d7:	nop
+   29a1b24d8:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b24d8 <_register_onexit_function>:
-   29a1b24d8:	jmp    *0x6e72(%rip)        # 29a1b9350 <__imp__register_onexit_function>
-   29a1b24de:	nop
-   29a1b24df:	nop
-
-000000029a1b24e0 <abort>:
-   29a1b24e0:	jmp    *0x6e72(%rip)        # 29a1b9358 <__imp_abort>
+000000029a1b24e0 <__p__environ>:
+   29a1b24e0:	jmp    *0x6dc2(%rip)        # 29a1b92a8 <__imp___p__environ>
    29a1b24e6:	nop
    29a1b24e7:	nop
-   29a1b24e8:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b24f0 <_set_new_mode>:
-   29a1b24f0:	jmp    *0x6dd2(%rip)        # 29a1b92c8 <__imp__set_new_mode>
+000000029a1b24e8 <__p__wenviron>:
+   29a1b24e8:	jmp    *0x6dc2(%rip)        # 29a1b92b0 <__imp___p__wenviron>
+   29a1b24ee:	nop
+   29a1b24ef:	nop
+
+000000029a1b24f0 <getch>:
+   29a1b24f0:	jmp    *0x6da2(%rip)        # 29a1b9298 <__imp_getch>
    29a1b24f6:	nop
    29a1b24f7:	nop
+   29a1b24f8:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b24f8 <calloc>:
-   29a1b24f8:	jmp    *0x6dd2(%rip)        # 29a1b92d0 <__imp_calloc>
-   29a1b24fe:	nop
-   29a1b24ff:	nop
-
-000000029a1b2500 <free>:
-   29a1b2500:	jmp    *0x6dd2(%rip)        # 29a1b92d8 <__imp_free>
-   29a1b2506:	nop
-   29a1b2507:	nop
-   29a1b2508:	nopl   0x0(%rax,%rax,1)
-
-000000029a1b2510 <__p__environ>:
-   29a1b2510:	jmp    *0x6d9a(%rip)        # 29a1b92b0 <__imp___p__environ>
-   29a1b2516:	nop
-   29a1b2517:	nop
-
-000000029a1b2518 <__p__wenviron>:
-   29a1b2518:	jmp    *0x6d9a(%rip)        # 29a1b92b8 <__imp___p__wenviron>
-   29a1b251e:	nop
-   29a1b251f:	nop
-
-000000029a1b2520 <getch>:
-   29a1b2520:	jmp    *0x6d7a(%rip)        # 29a1b92a0 <__imp_getch>
-   29a1b2526:	nop
-   29a1b2527:	nop
-   29a1b2528:	nopl   0x0(%rax,%rax,1)
-
-000000029a1b2530 <fprintf>:
+000000029a1b2500 <fprintf>:
 fprintf():
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:12
-   29a1b2530:	sub    $0x48,%rsp
+   29a1b2500:	sub    $0x48,%rsp
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:15
-   29a1b2534:	lea    0x60(%rsp),%rax
+   29a1b2504:	lea    0x60(%rsp),%rax
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:12
-   29a1b2539:	mov    %r8,0x60(%rsp)
+   29a1b2509:	mov    %r8,0x60(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:16
-   29a1b253e:	mov    %rdx,%r8
-   29a1b2541:	mov    %rcx,%rdx
-   29a1b2544:	mov    %rax,0x20(%rsp)
-   29a1b2549:	xor    %ecx,%ecx
+   29a1b250e:	mov    %rdx,%r8
+   29a1b2511:	mov    %rcx,%rdx
+   29a1b2514:	mov    %rax,0x20(%rsp)
+   29a1b2519:	xor    %ecx,%ecx
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:12
-   29a1b254b:	mov    %r9,0x68(%rsp)
+   29a1b251b:	mov    %r9,0x68(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:16
-   29a1b2550:	xor    %r9d,%r9d
+   29a1b2520:	xor    %r9d,%r9d
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:15
-   29a1b2553:	mov    %rax,0x38(%rsp)
+   29a1b2523:	mov    %rax,0x38(%rsp)
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:16
-   29a1b2558:	call   29a1b2438 <__stdio_common_vfprintf>
+   29a1b2528:	call   29a1b2418 <__stdio_common_vfprintf>
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:19
-   29a1b255d:	add    $0x48,%rsp
-   29a1b2561:	ret
-   29a1b2562:	nop
-   29a1b2563:	nop
-   29a1b2564:	nop
-   29a1b2565:	nop
+   29a1b252d:	add    $0x48,%rsp
+   29a1b2531:	ret
+   29a1b2532:	nop
+   29a1b2533:	nop
+   29a1b2534:	nop
+   29a1b2535:	nop
+   29a1b2536:	nop
+   29a1b2537:	nop
+   29a1b2538:	nop
+   29a1b2539:	nop
+   29a1b253a:	nop
+   29a1b253b:	nop
+   29a1b253c:	nop
+   29a1b253d:	nop
+   29a1b253e:	nop
+   29a1b253f:	nop
+
+000000029a1b2540 <VirtualQuery>:
+   29a1b2540:	jmp    *0x6d42(%rip)        # 29a1b9288 <__imp_VirtualQuery>
+   29a1b2546:	nop
+   29a1b2547:	nop
+
+000000029a1b2548 <VirtualProtect>:
+   29a1b2548:	jmp    *0x6d32(%rip)        # 29a1b9280 <__imp_VirtualProtect>
+   29a1b254e:	nop
+   29a1b254f:	nop
+
+000000029a1b2550 <TlsGetValue>:
+   29a1b2550:	jmp    *0x6d22(%rip)        # 29a1b9278 <__imp_TlsGetValue>
+   29a1b2556:	nop
+   29a1b2557:	nop
+
+000000029a1b2558 <Sleep>:
+   29a1b2558:	jmp    *0x6d12(%rip)        # 29a1b9270 <__imp_Sleep>
+   29a1b255e:	nop
+   29a1b255f:	nop
+
+000000029a1b2560 <LeaveCriticalSection>:
+   29a1b2560:	jmp    *0x6d02(%rip)        # 29a1b9268 <__imp_LeaveCriticalSection>
    29a1b2566:	nop
    29a1b2567:	nop
-   29a1b2568:	nop
-   29a1b2569:	nop
-   29a1b256a:	nop
-   29a1b256b:	nop
-   29a1b256c:	nop
-   29a1b256d:	nop
+
+000000029a1b2568 <InitializeCriticalSection>:
+   29a1b2568:	jmp    *0x6cf2(%rip)        # 29a1b9260 <__imp_InitializeCriticalSection>
    29a1b256e:	nop
    29a1b256f:	nop
 
-000000029a1b2570 <VirtualQuery>:
-   29a1b2570:	jmp    *0x6d1a(%rip)        # 29a1b9290 <__imp_VirtualQuery>
+000000029a1b2570 <GetLastError>:
+   29a1b2570:	jmp    *0x6ce2(%rip)        # 29a1b9258 <__imp_GetLastError>
    29a1b2576:	nop
    29a1b2577:	nop
 
-000000029a1b2578 <VirtualProtect>:
-   29a1b2578:	jmp    *0x6d0a(%rip)        # 29a1b9288 <__imp_VirtualProtect>
+000000029a1b2578 <EnterCriticalSection>:
+   29a1b2578:	jmp    *0x6cd2(%rip)        # 29a1b9250 <__imp_EnterCriticalSection>
    29a1b257e:	nop
    29a1b257f:	nop
 
-000000029a1b2580 <TlsGetValue>:
-   29a1b2580:	jmp    *0x6cfa(%rip)        # 29a1b9280 <__imp_TlsGetValue>
+000000029a1b2580 <DeleteCriticalSection>:
+   29a1b2580:	jmp    *0x6cc2(%rip)        # 29a1b9248 <__IAT_start__>
    29a1b2586:	nop
    29a1b2587:	nop
+   29a1b2588:	nopl   0x0(%rax,%rax,1)
 
-000000029a1b2588 <Sleep>:
-   29a1b2588:	jmp    *0x6cea(%rip)        # 29a1b9278 <__imp_Sleep>
-   29a1b258e:	nop
-   29a1b258f:	nop
-
-000000029a1b2590 <LeaveCriticalSection>:
-   29a1b2590:	jmp    *0x6cda(%rip)        # 29a1b9270 <__imp_LeaveCriticalSection>
+000000029a1b2590 <register_frame_ctor>:
+   29a1b2590:	jmp    29a1b1360 <__gcc_register_frame>
+   29a1b2595:	nop
    29a1b2596:	nop
    29a1b2597:	nop
-
-000000029a1b2598 <InitializeCriticalSection>:
-   29a1b2598:	jmp    *0x6cca(%rip)        # 29a1b9268 <__imp_InitializeCriticalSection>
+   29a1b2598:	nop
+   29a1b2599:	nop
+   29a1b259a:	nop
+   29a1b259b:	nop
+   29a1b259c:	nop
+   29a1b259d:	nop
    29a1b259e:	nop
    29a1b259f:	nop
 
-000000029a1b25a0 <GetLastError>:
-   29a1b25a0:	jmp    *0x6cba(%rip)        # 29a1b9260 <__imp_GetLastError>
-   29a1b25a6:	nop
-   29a1b25a7:	nop
-
-000000029a1b25a8 <EnterCriticalSection>:
-   29a1b25a8:	jmp    *0x6caa(%rip)        # 29a1b9258 <__imp_EnterCriticalSection>
-   29a1b25ae:	nop
-   29a1b25af:	nop
-
-000000029a1b25b0 <DeleteCriticalSection>:
-   29a1b25b0:	jmp    *0x6c9a(%rip)        # 29a1b9250 <__IAT_start__>
-   29a1b25b6:	nop
-   29a1b25b7:	nop
-   29a1b25b8:	nopl   0x0(%rax,%rax,1)
-
-000000029a1b25c0 <register_frame_ctor>:
-   29a1b25c0:	jmp    29a1b1360 <__gcc_register_frame>
-   29a1b25c5:	nop
-   29a1b25c6:	nop
-   29a1b25c7:	nop
-   29a1b25c8:	nop
-   29a1b25c9:	nop
-   29a1b25ca:	nop
-   29a1b25cb:	nop
-   29a1b25cc:	nop
-   29a1b25cd:	nop
-   29a1b25ce:	nop
-   29a1b25cf:	nop
-
-000000029a1b25d0 <__CTOR_LIST__>:
-   29a1b25d0:	(bad)
-   29a1b25d1:	(bad)
-   29a1b25d2:	(bad)
-   29a1b25d3:	(bad)
-   29a1b25d4:	(bad)
-   29a1b25d5:	(bad)
-   29a1b25d6:	(bad)
-   29a1b25d7:	inc    %eax
-
-000000029a1b25d8 <.ctors.65535>:
-   29a1b25d8:	shlb   $0x0,0x29a1b(%rip)        # 29a1dbffa <.debug_rnglists+0xbf56>
-	...
-
-000000029a1b25e8 <__DTOR_LIST__>:
-   29a1b25e8:	(bad)
-   29a1b25e9:	(bad)
-   29a1b25ea:	(bad)
-   29a1b25eb:	(bad)
-   29a1b25ec:	(bad)
-   29a1b25ed:	(bad)
-   29a1b25ee:	(bad)
-   29a1b25ef:	incl   (%rax)
-   29a1b25f1:	add    %al,(%rax)
-   29a1b25f3:	add    %al,(%rax)
-   29a1b25f5:	add    %al,(%rax)
+000000029a1b25a0 <__CTOR_LIST__>:
+   29a1b25a0:	(bad)
+   29a1b25a1:	(bad)
+   29a1b25a2:	(bad)
+   29a1b25a3:	(bad)
+   29a1b25a4:	(bad)
+   29a1b25a5:	(bad)
+   29a1b25a6:	(bad)
+   29a1b25a7:	call   *0x29a1b25(%rax)
+
+000000029a1b25a8 <.ctors.65535>:
+   29a1b25a8:	nop
+   29a1b25a9:	and    $0x29a1b,%eax
+	...
+
+000000029a1b25b8 <__DTOR_LIST__>:
+   29a1b25b8:	(bad)
+   29a1b25b9:	(bad)
+   29a1b25ba:	(bad)
+   29a1b25bb:	(bad)
+   29a1b25bc:	(bad)
+   29a1b25bd:	(bad)
+   29a1b25be:	(bad)
+   29a1b25bf:	incl   (%rax)
+   29a1b25c1:	add    %al,(%rax)
+   29a1b25c3:	add    %al,(%rax)
+   29a1b25c5:	add    %al,(%rax)
 	...
 
 Disassembly of section .data:
 
 000000029a1b3000 <__data_start__>:
    29a1b3000:	add    %eax,(%rax)
 	...
 
 000000029a1b3010 <p.0>:
-   29a1b3010:	lock and $0x29a1b,%eax
+   29a1b3010:	shlb   $0x0,0x29a1b(%rip)        # 29a1dca32 <.debug_rnglists+0xc98e>
 	...
 
 000000029a1b3020 <__native_vcclrit_reason>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/natstart.c:12
    29a1b3020:	(bad)
    29a1b3021:	(bad)
    29a1b3022:	(bad)
@@ -4517,57 +4492,58 @@
 000000029a1b3030 <_CRT_MT>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlsmcrt.c:12
    29a1b3030:	add    (%rax),%al
 	...
 
 000000029a1b3040 <__imp_vfprintf>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_vfprintf.c:15
-   29a1b3040:	shlb   $0x1b,(%rcx)
-   29a1b3043:	(bad)
-   29a1b3044:	add    (%rax),%al
+   29a1b3040:	movabs 0x29a1b21,%al
+   29a1b3049:	add    %al,(%rax)
+   29a1b304b:	add    %al,(%rax)
+   29a1b304d:	add    %al,(%rax)
 	...
 
 000000029a1b3050 <__imp___ms_fwprintf>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:166
-   29a1b3050:	rex and (%rbx),%ebx
-   29a1b3053:	(bad)
-   29a1b3054:	add    (%rax),%al
-	...
+   29a1b3050:	and    %ah,(%rbx)
+   29a1b3052:	sbb    0x2(%rdx),%ebx
 
 000000029a1b3058 <__imp_tzset>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:165
-   29a1b3058:	andb   $0x1b,(%rbx)
+   29a1b3058:	(bad)
+   29a1b3059:	and    (%rbx),%ebx
    29a1b305b:	(bad)
    29a1b305c:	add    (%rax),%al
 	...
 
 000000029a1b3060 <__imp__get_output_format>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:164
-   29a1b3060:	loopne 29a1b3083 <__imp_daylight+0x3>
-   29a1b3062:	sbb    0x2(%rdx),%ebx
+   29a1b3060:	shlb   $0x1b,(%rcx)
+   29a1b3063:	(bad)
+   29a1b3064:	add    (%rax),%al
+	...
 
 000000029a1b3068 <__imp__amsg_exit>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:163
-   29a1b3068:	adc    %ah,(%rbx)
-   29a1b306a:	sbb    0x2(%rdx),%ebx
+   29a1b3068:	lock and (%rbx),%bl
+   29a1b306b:	(bad)
+   29a1b306c:	add    (%rax),%al
+	...
 
 000000029a1b3070 <__imp___wgetmainargs>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:162
-   29a1b3070:	(bad)
-   29a1b3071:	and    (%rbx),%bl
+   29a1b3070:	rex and (%rbx),%bl
    29a1b3073:	(bad)
    29a1b3074:	add    (%rax),%al
 	...
 
 000000029a1b3078 <__imp___getmainargs>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:161
-   29a1b3078:	lock and %ebx,(%rbx)
-   29a1b307b:	(bad)
-   29a1b307c:	add    (%rax),%al
-	...
+   29a1b3078:	shlb   $1,(%rcx)
+   29a1b307a:	sbb    0x2(%rdx),%ebx
 
 000000029a1b3080 <__imp_daylight>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:131
    29a1b3080:	cwtl
    29a1b3081:	xor    %bl,(%rbx)
    29a1b3083:	(bad)
    29a1b3084:	add    (%rax),%al
@@ -4612,35 +4588,34 @@
    29a1b30b4:	push   %rax
    29a1b30b5:	push   %rbx
    29a1b30b6:	push   %rsp
 	...
 
 000000029a1b30b8 <__imp_at_quick_exit>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:103
-   29a1b30b8:	lock and (%rbx),%bl
-   29a1b30bb:	(bad)
-   29a1b30bc:	add    (%rax),%al
-	...
+   29a1b30b8:	shlb   $1,(%rdx)
+   29a1b30ba:	sbb    0x2(%rdx),%ebx
 
 000000029a1b30c0 <__imp__onexit>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/ucrtbase_compat.c:91
-   29a1b30c0:	shlb   $1,(%rdx)
+   29a1b30c0:	mov    $0x22,%al
    29a1b30c2:	sbb    0x2(%rdx),%ebx
 	...
 
 000000029a1b30d0 <__imp_fprintf>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/stdio/ucrt_fprintf.c:20
-   29a1b30d0:	xor    %ah,0x29a1b(%rip)        # 29a1dcaf1 <.debug_rnglists+0xca4d>
+   29a1b30d0:	add    %ah,0x29a1b(%rip)        # 29a1dcaf1 <.debug_rnglists+0xca4d>
 	...
 
 Disassembly of section .rdata:
 
 000000029a1b4000 <__dyn_tls_init_callback>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:104
-   29a1b4000:	add    %dl,0x29a1b(%rip)        # 29a1dda21 <.debug_rnglists+0xd97d>
+   29a1b4000:	loopne 29a1b4016 <__dyn_tls_init_callback+0x16>
+   29a1b4002:	sbb    0x2(%rdx),%ebx
 	...
 
 000000029a1b4020 <_tls_used>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:48
    29a1b4020:	add    %dh,0x29a1b(%rax)
    29a1b4026:	add    %al,(%rax)
    29a1b4028:	or     %dh,0x29a1b(%rax)
@@ -4789,15 +4764,18 @@
 
 000000029a1b41e0 <.refptr._CRT_MT>:
    29a1b41e0:	xor    %dh,(%rax)
    29a1b41e2:	sbb    0x2(%rdx),%ebx
 	...
 
 000000029a1b41f0 <.refptr.__CTOR_LIST__>:
-   29a1b41f0:	shlb   $1,0x29a1b(%rip)        # 29a1ddc11 <.debug_rnglists+0xdb6d>
+   29a1b41f0:	movabs 0x29a1b25,%al
+   29a1b41f9:	add    %al,(%rax)
+   29a1b41fb:	add    %al,(%rax)
+   29a1b41fd:	add    %al,(%rax)
 	...
 
 000000029a1b4200 <.refptr.__ImageBase>:
    29a1b4200:	add    %al,(%rax)
    29a1b4202:	sbb    0x2(%rdx),%ebx
 	...
 
@@ -4816,15 +4794,16 @@
 000000029a1b4230 <.refptr.__dyn_tls_init_callback>:
    29a1b4230:	add    %al,0x1b(%rax)
    29a1b4233:	(bad)
    29a1b4234:	add    (%rax),%al
 	...
 
 000000029a1b4240 <.refptr.__imp__tzset>:
-   29a1b4240:	fcoms  0x29a1b(%rbx)
+   29a1b4240:	enter  $0x1b93,$0x9a
+   29a1b4244:	add    (%rax),%al
 	...
 
 000000029a1b4250 <.refptr.__mingw_app_type>:
    29a1b4250:	push   %rax
    29a1b4251:	jo     29a1b426e <.refptr.__mingw_module_is_dll+0xe>
    29a1b4253:	(bad)
    29a1b4254:	add    (%rax),%al
@@ -5436,232 +5415,249 @@
    29a1b504c:	jno    29a1b5061 <.pdata+0xd>
    29a1b504e:	add    %al,(%rax)
    29a1b5050:	xor    $0x60,%al
 	...
 
 000000029a1b5054 <.pdata>:
    29a1b5054:	adcb   $0x0,(%rbx)
-   29a1b5057:	add    %ah,0x38000013(%rbp)
+   29a1b5057:	add    %al,0x38000013(%rdi)
    29a1b505d:	(bad)
    29a1b505e:	add    %al,(%rax)
-   29a1b5060:	movsl  %ds:(%rsi),%es:(%rdi)
-   29a1b5061:	adc    (%rax),%eax
-   29a1b5063:	add    %bh,0x44000013(%rax)
-   29a1b5069:	(bad)
+   29a1b5060:	xchg   %edx,(%rbx)
+   29a1b5062:	add    %al,(%rax)
+   29a1b5064:	(bad)
+   29a1b5065:	adc    (%rax),%eax
+   29a1b5067:	add    %al,0x60(%rax)
    29a1b506a:	add    %al,(%rax)
-   29a1b506c:	mov    $0xec000013,%eax
+   29a1b506c:	(bad)
+   29a1b506d:	adc    (%rax),%eax
+   29a1b506f:	add    %cl,%dh
    29a1b5071:	adc    (%rax),%eax
-   29a1b5073:	add    %dl,0x60(%rax)
-   29a1b5076:	add    %al,(%rax)
-   29a1b5078:	in     (%dx),%al
+   29a1b5073:	add    %cl,0x0(%rax,%riz,2)
+   29a1b5077:	add    %cl,%dh
    29a1b5079:	adc    (%rax),%eax
-   29a1b507b:	add    %dh,%bl
+   29a1b507b:	add    %dl,%ch
    29a1b507d:	adc    (%rax),%eax
-   29a1b507f:	add    %bl,0x0(%rax,%riz,2)
+   29a1b507f:	add    %bl,0x60(%rax)
 	...
 
 000000029a1b5084 <.pdata>:
-   29a1b5084:	add    %dl,(%rax,%rax,1)
-   29a1b5087:	add    %bh,(%rdx)
-   29a1b5089:	adc    $0x0,%al
-   29a1b508b:	add    %ah,0x0(%rax,%riz,2)
-   29a1b508f:	add    %al,0x14(%rax)
-   29a1b5092:	add    %al,(%rax)
-   29a1b5094:	stos   %al,%es:(%rdi)
-   29a1b5095:	adc    $0x0,%al
-   29a1b5097:	add    %ch,0x0(%rax,%riz,2)
-   29a1b509b:	add    %dh,-0x30ffffec(%rax)
-   29a1b50a1:	adc    $0x0,%al
-   29a1b50a3:	add    %bh,0x60(%rax)
+   29a1b5084:	loopne 29a1b5099 <.pdata+0x15>
+   29a1b5086:	add    %al,(%rax)
+   29a1b5088:	sbb    (%rax,%rax,1),%dl
+   29a1b508b:	add    %ah,0x60(%rax)
+   29a1b508e:	add    %al,(%rax)
+   29a1b5090:	and    %dl,(%rax,%rax,1)
+   29a1b5093:	add    %cl,0x68000014(%rdx)
+   29a1b5099:	(bad)
+   29a1b509a:	add    %al,(%rax)
+   29a1b509c:	nop
+   29a1b509d:	adc    $0x0,%al
+   29a1b509f:	add    %ch,0x74000014(%rdi)
+   29a1b50a5:	(bad)
 	...
 
 000000029a1b50a8 <.pdata>:
-   29a1b50a8:	rclb   $1,(%rax,%rax,1)
-   29a1b50ab:	add    %bh,%bh
-   29a1b50ad:	adc    $0x0,%al
-   29a1b50af:	add    %bh,0x0(%rax,%riz,2)
-   29a1b50b3:	add    %al,(%rax)
-   29a1b50b5:	adc    $0x15810000,%eax
-   29a1b50ba:	add    %al,(%rax)
-   29a1b50bc:	test   %ah,0x0(%rax)
-   29a1b50bf:	add    %dl,-0x6cffffeb(%rax)
-   29a1b50c5:	adc    $0x60900000,%eax
+   29a1b50a8:	mov    $0x14,%al
+   29a1b50aa:	add    %al,(%rax)
+   29a1b50ac:	fists  (%rax,%rax,1)
+   29a1b50af:	add    %bh,0x60(%rax)
+   29a1b50b2:	add    %al,(%rax)
+   29a1b50b4:	loopne 29a1b50ca <.pdata+0x22>
+   29a1b50b6:	add    %al,(%rax)
+   29a1b50b8:	(bad)
+   29a1b50b9:	adc    $0x60800000,%eax
+   29a1b50be:	add    %al,(%rax)
+   29a1b50c0:	jo     29a1b50d7 <.pdata+0xb>
+   29a1b50c2:	add    %al,(%rax)
+   29a1b50c4:	jae    29a1b50db <.pdata+0xf>
+   29a1b50c6:	add    %al,(%rax)
+   29a1b50c8:	mov    %fs,0x0(%rax)
 	...
 
 000000029a1b50cc <.pdata>:
-   29a1b50cc:	movabs 0x9400001609000015,%al
-   29a1b50d5:	(bad)
-   29a1b50d6:	add    %al,(%rax)
-   29a1b50d8:	adc    %dl,(%rsi)
-   29a1b50da:	add    %al,(%rax)
-   29a1b50dc:	jb     29a1b50f5 <.pdata+0x5>
+   29a1b50cc:	adcb   $0x0,0x15e90000(%rip)        # 2b00450d3 <.debug_rnglists+0x15e7502f>
+   29a1b50d3:	add    %dl,-0xfffffa0(%rax)
+   29a1b50d9:	adc    $0x17520000,%eax
    29a1b50de:	add    %al,(%rax)
-   29a1b50e0:	movabs 0xdd00001780000060,%al
-   29a1b50e9:	sbb    (%rax),%al
-   29a1b50eb:	add    %ch,0x1ae00000(%rax,%riz,2)
+   29a1b50e0:	pushf
+   29a1b50e1:	(bad)
+   29a1b50e2:	add    %al,(%rax)
+   29a1b50e4:	(bad)
+   29a1b50e5:	(bad)
+   29a1b50e6:	add    %al,(%rax)
+   29a1b50e8:	mov    $0xa800001a,%ebp
+   29a1b50ed:	(bad)
+	...
 
 000000029a1b50f0 <.pdata>:
-   29a1b50f0:	loopne 29a1b510c <.pdata+0x1c>
-   29a1b50f2:	add    %al,(%rax)
-   29a1b50f4:	push   %rax
+   29a1b50f0:	rcrb   $0x0,(%rdx)
+   29a1b50f3:	add    %dh,(%rax)
    29a1b50f5:	sbb    (%rax),%eax
-   29a1b50f7:	add    %al,%ah
+   29a1b50f7:	add    %al,%al
    29a1b50f9:	(bad)
    29a1b50fa:	add    %al,(%rax)
-   29a1b50fc:	push   %rax
-   29a1b50fd:	sbb    (%rax),%eax
-   29a1b50ff:	add    %bh,-0x2bffffe5(%rdi)
+   29a1b50fc:	xor    %bl,(%rbx)
+   29a1b50fe:	add    %al,(%rax)
+   29a1b5100:	lahf
+   29a1b5101:	sbb    (%rax),%eax
+   29a1b5103:	add    %dl,%al
    29a1b5105:	(bad)
    29a1b5106:	add    %al,(%rax)
-   29a1b5108:	rcrb   $0x0,(%rbx)
-   29a1b510b:	add    %al,0x1c(%rcx)
-   29a1b510e:	add    %al,(%rax)
-   29a1b5110:	loopne 29a1b5172 <.pdata+0x52>
+   29a1b5108:	movabs 0xdc00001c2100001b,%al
+   29a1b5111:	(bad)
    29a1b5112:	add    %al,(%rax)
-   29a1b5114:	push   %rax
-   29a1b5115:	sbb    $0x0,%al
-   29a1b5117:	add    %al,0x1d(%rdx)
-   29a1b511a:	add    %al,(%rax)
-   29a1b511c:	in     (%dx),%al
-   29a1b511d:	(bad)
+   29a1b5114:	xor    %bl,(%rax,%rax,1)
+   29a1b5117:	add    %ah,(%rdx)
+   29a1b5119:	sbb    $0x60e80000,%eax
 	...
 
 000000029a1b5120 <.pdata>:
-   29a1b5120:	push   %rax
-   29a1b5121:	sbb    $0x1d7c0000,%eax
+   29a1b5120:	xor    %bl,0x1d5c0000(%rip)        # 2b7775126 <.debug_rnglists+0x1d5a5082>
    29a1b5126:	add    %al,(%rax)
-   29a1b5128:	hlt
-   29a1b5129:	(bad)
+   29a1b5128:	lock (bad)
    29a1b512a:	add    %al,(%rax)
-   29a1b512c:	sbbb   $0x0,0x1dd00000(%rip)        # 2b7eb5133 <.debug_rnglists+0x1dce508f>
-   29a1b5133:	add    %bh,%al
+   29a1b512c:	(bad)
+   29a1b512d:	sbb    $0x1db00000,%eax
+   29a1b5132:	add    %al,(%rax)
+   29a1b5134:	hlt
    29a1b5135:	(bad)
    29a1b5136:	add    %al,(%rax)
-   29a1b5138:	rcrb   $1,0x1e6d0000(%rip)        # 2b888513e <.debug_rnglists+0x1e6b509a>
+   29a1b5138:	mov    $0x1d,%al
+   29a1b513a:	add    %al,(%rax)
+   29a1b513c:	rex.WRB (bad)
    29a1b513e:	add    %al,(%rax)
-   29a1b5140:	cld
+   29a1b5140:	clc
    29a1b5141:	(bad)
    29a1b5142:	add    %al,(%rax)
-   29a1b5144:	jo     29a1b5164 <.pdata+0x44>
+   29a1b5144:	push   %rax
+   29a1b5145:	(bad)
    29a1b5146:	add    %al,(%rax)
-   29a1b5148:	lock (bad)
+   29a1b5148:	rcrb   $1,(%rsi)
    29a1b514a:	add    %al,(%rax)
-   29a1b514c:	or     %ah,0x0(%rcx)
-   29a1b514f:	add    %dh,%al
-   29a1b5151:	(bad)
+   29a1b514c:	add    $0x61,%al
+   29a1b514e:	add    %al,(%rax)
+   29a1b5150:	rcrb   $1,(%rsi)
    29a1b5152:	add    %al,(%rax)
    29a1b5154:	(bad)
    29a1b5155:	(bad)
    29a1b5156:	add    %al,(%rax)
-   29a1b5158:	or     $0x61,%al
-   29a1b515a:	add    %al,(%rax)
-   29a1b515c:	xor    %bl,(%rdi)
+   29a1b5158:	or     %ah,0x0(%rcx)
+   29a1b515b:	add    %dl,(%rax)
+   29a1b515d:	(bad)
    29a1b515e:	add    %al,(%rax)
-   29a1b5160:	movabs %eax,0xb00000611000001f
+   29a1b5160:	sbbl   $0x0,(%rdi)
+   29a1b5163:	add    %cl,(%rcx,%riz,2)
+   29a1b5166:	add    %al,(%rax)
+   29a1b5168:	nop
    29a1b5169:	(bad)
    29a1b516a:	add    %al,(%rax)
-   29a1b516c:	out    %al,$0x1f
+   29a1b516c:	(bad)
+   29a1b516d:	(bad)
    29a1b516e:	add    %al,(%rax)
-   29a1b5170:	adc    $0x61,%al
-   29a1b5172:	add    %al,(%rax)
-   29a1b5174:	lock (bad)
+   29a1b5170:	adc    %ah,0x0(%rcx)
+   29a1b5173:	add    %dl,%al
+   29a1b5175:	(bad)
    29a1b5176:	add    %al,(%rax)
-   29a1b5178:	jns    29a1b519a <.pdata+0x2>
-   29a1b517a:	add    %al,(%rax)
-   29a1b517c:	sbb    %ah,0x0(%rcx)
-   29a1b517f:	add    %al,0x46000020(%rax)
+   29a1b5178:	pop    %rcx
+   29a1b5179:	and    %al,(%rax)
+   29a1b517b:	add    %dl,(%rcx,%riz,2)
+   29a1b517e:	add    %al,(%rax)
+   29a1b5180:	(bad)
+   29a1b5181:	and    %al,(%rax)
+   29a1b5183:	add    %ah,(%rsi)
    29a1b5185:	and    %eax,(%rax)
-   29a1b5187:	add    %bl,(%rcx,%riz,2)
+   29a1b5187:	add    %bl,(%rax)
+   29a1b5189:	(bad)
 	...
 
 000000029a1b518c <.pdata>:
-   29a1b518c:	push   %rax
-   29a1b518d:	and    %eax,(%rax)
-   29a1b518f:	add    %dl,0x21(%rbx)
+   29a1b518c:	xor    %ah,(%rcx)
+   29a1b518e:	add    %al,(%rax)
+   29a1b5190:	xor    (%rcx),%esp
    29a1b5192:	add    %al,(%rax)
-   29a1b5194:	and    %ah,0x0(%rcx)
+   29a1b5194:	sbb    $0x61,%al
 	...
 
 000000029a1b5198 <.pdata>:
-   29a1b5198:	movabs 0x24000021a6000021,%al
+   29a1b5198:	andb   $0x0,(%rcx)
+   29a1b519b:	add    %al,0x20000021(%rsi)
    29a1b51a1:	(bad)
 	...
 
 000000029a1b51a4 <.pdata>:
-   29a1b51a4:	mov    $0x21,%al
-   29a1b51a6:	add    %al,(%rax)
-   29a1b51a8:	mov    $0x21,%dh
-   29a1b51aa:	add    %al,(%rax)
-   29a1b51ac:	sub    %ah,0x0(%rcx)
+   29a1b51a4:	nop
+   29a1b51a5:	and    %eax,(%rax)
+   29a1b51a7:	add    %dl,0x24000021(%rsi)
+   29a1b51ad:	(bad)
 	...
 
 000000029a1b51b0 <.pdata>:
-   29a1b51b0:	shlb   $0x0,(%rcx)
-   29a1b51b3:	add    %bl,%dh
-   29a1b51b5:	and    %eax,(%rax)
-   29a1b51b7:	add    %ch,(%rcx,%riz,2)
+   29a1b51b0:	movabs 0x28000021be000021,%al
+   29a1b51b9:	(bad)
 	...
 
 000000029a1b51bc <.pdata>:
-   29a1b51bc:	loopne 29a1b51df <.pdata+0x23>
-   29a1b51be:	add    %al,(%rax)
-   29a1b51c0:	jrcxz  29a1b51e3 <.pdata+0x27>
-   29a1b51c2:	add    %al,(%rax)
-   29a1b51c4:	xor    $0x61,%al
+   29a1b51bc:	shlb   $0x0,(%rcx)
+   29a1b51bf:	add    %al,%bl
+   29a1b51c1:	and    %eax,(%rax)
+   29a1b51c3:	add    %dh,(%rax)
+   29a1b51c5:	(bad)
    29a1b51c6:	add    %al,(%rax)
-   29a1b51c8:	lock and %eax,(%rax)
-   29a1b51cb:	add    %bl,0x22(%rdx)
+   29a1b51c8:	shlb   $1,(%rcx)
+   29a1b51ca:	add    %al,(%rax)
+   29a1b51cc:	cmp    (%rdx),%ah
    29a1b51ce:	add    %al,(%rax)
-   29a1b51d0:	cmp    %ah,0x0(%rcx)
-   29a1b51d3:	add    %ah,0x22(%rax)
-   29a1b51d6:	add    %al,(%rax)
-   29a1b51d8:	lret   $0x22
-   29a1b51db:	add    %cl,0x61(%rax)
+   29a1b51d0:	xor    $0x61,%al
+   29a1b51d2:	add    %al,(%rax)
+   29a1b51d4:	rex and (%rax),%al
+   29a1b51d7:	add    %ch,0x44000022(%rdx)
+   29a1b51dd:	(bad)
    29a1b51de:	add    %al,(%rax)
-   29a1b51e0:	shlb   $1,(%rdx)
+   29a1b51e0:	mov    $0x22,%al
    29a1b51e2:	add    %al,(%rax)
-   29a1b51e4:	out    %al,(%dx)
+   29a1b51e4:	(bad)
    29a1b51e5:	and    (%rax),%al
-   29a1b51e7:	add    %bl,0x61(%rax)
-   29a1b51ea:	add    %al,(%rax)
-   29a1b51ec:	lock and (%rax),%al
-   29a1b51ef:	add    %al,0x60000023(%rip)        # 2fa1b5218 <.debug_rnglists+0x5ffe5174>
-   29a1b51f5:	(bad)
-   29a1b51f6:	add    %al,(%rax)
-   29a1b51f8:	adc    %ah,(%rbx)
-   29a1b51fa:	add    %al,(%rax)
-   29a1b51fc:	ds and (%rax),%eax
-   29a1b51ff:	add    %ah,0x0(%rcx,%riz,2)
-   29a1b5203:	add    %al,0x23(%rax)
+   29a1b51e7:	add    %dl,0x0(%rcx,%riz,2)
+   29a1b51eb:	add    %dl,%al
+   29a1b51ed:	and    (%rax),%al
+   29a1b51ef:	add    %ah,%ch
+   29a1b51f1:	and    (%rax),%al
+   29a1b51f3:	add    %bl,0x0(%rcx,%riz,2)
+   29a1b51f7:	add    %dh,%al
+   29a1b51f9:	and    (%rax),%al
+   29a1b51fb:	add    %bl,(%rsi)
+   29a1b51fd:	and    (%rax),%eax
+   29a1b51ff:	add    %ah,0x61(%rax)
+   29a1b5202:	add    %al,(%rax)
+   29a1b5204:	and    %ah,(%rbx)
    29a1b5206:	add    %al,(%rax)
-   29a1b5208:	jne    29a1b522d <.pdata+0x5>
-   29a1b520a:	add    %al,(%rax)
-   29a1b520c:	insb   (%dx),%es:(%rdi)
-   29a1b520d:	(bad)
+   29a1b5208:	push   %rbp
+   29a1b5209:	and    (%rax),%eax
+   29a1b520b:	add    %ch,0x61(%rax)
    29a1b520e:	add    %al,(%rax)
-   29a1b5210:	andb   $0x0,(%rbx)
-   29a1b5213:	add    %dh,0x74000023(%rsi)
+   29a1b5210:	(bad)
+   29a1b5211:	and    (%rax),%eax
+   29a1b5213:	add    %dl,0x70000023(%rsi)
    29a1b5219:	(bad)
    29a1b521a:	add    %al,(%rax)
-   29a1b521c:	shlb   $0x0,(%rbx)
-   29a1b521f:	add    %dh,%dh
-   29a1b5221:	and    (%rax),%eax
-   29a1b5223:	add    %bh,0x0(%rcx,%riz,2)
+   29a1b521c:	movabs 0x78000023d6000023,%al
+   29a1b5225:	(bad)
 	...
 
 000000029a1b5228 <.pdata>:
-   29a1b5228:	xor    %ah,0x25620000(%rip)        # 2bf7d522e <.debug_rnglists+0x2560518a>
+   29a1b5228:	add    %ah,0x25320000(%rip)        # 2bf4d522e <.debug_rnglists+0x2530518a>
    29a1b522e:	add    %al,(%rax)
-   29a1b5230:	test   %ah,0x0(%rcx)
-	...
+   29a1b5230:	andb   $0x0,0x0(%rcx)
 
 000000029a1b5234 <.pdata.startup>:
-   29a1b5234:	shlb   $0x0,0x25c50000(%rip)        # 2bfe0523b <.debug_rnglists+0x25c35197>
-   29a1b523b:	.byte 0
-   29a1b523c:	mov    %fs,0x0(%rcx)
+   29a1b5234:	nop
+   29a1b5235:	and    $0x25950000,%eax
+   29a1b523a:	add    %al,(%rax)
+   29a1b523c:	mov    %ah,0x0(%rcx)
 	...
 
 Disassembly of section .xdata:
 
 000000029a1b6000 <.xdata>:
    29a1b6000:	add    %eax,(%rax)
    29a1b6002:	add    %al,(%rax)
@@ -5691,205 +5687,205 @@
 000000029a1b6030 <.xdata>:
    29a1b6030:	add    %eax,(%rax)
    29a1b6032:	add    %al,(%rax)
    29a1b6034:	add    %eax,(%rax)
 	...
 
 000000029a1b6038 <.xdata>:
-   29a1b6038:	add    %ecx,(%rax)
-   29a1b603a:	add    0x3043208(%rip),%eax        # 29d1f9248 <.debug_rnglists+0x30291a4>
-   29a1b6040:	add    %edx,0x0(%rax)
-   29a1b6043:	add    %al,(%rcx)
-   29a1b6045:	or     %al,(%rbx)
-   29a1b6047:	add    $0x3043208,%eax
-   29a1b604c:	add    %edx,0x0(%rax)
-   29a1b604f:	add    %al,(%rcx)
-   29a1b6051:	or     %al,(%rbx)
-   29a1b6053:	add    $0x3045208,%eax
-   29a1b6058:	add    %edx,0x0(%rax)
-   29a1b605b:	add    %al,(%rcx)
-   29a1b605d:	add    $0x2,%al
-   29a1b605f:	add    $0x50010304,%eax
-
-000000029a1b6064 <.xdata>:
-   29a1b6064:	add    %eax,(%rcx,%rax,1)
-   29a1b6067:	add    %al,(%rdx,%rax,2)
-   29a1b606a:	add    %al,(%rax)
-   29a1b606c:	add    %eax,(%rsi)
-   29a1b606e:	add    (%rax),%eax
-   29a1b6070:	(bad)
-   29a1b6071:	rex.X add (%rax),%sil
-   29a1b6074:	add    %esp,0x0(%rax)
-   29a1b6077:	add    %al,(%rcx)
-   29a1b6079:	add    %al,(%rax)
-	...
-
-000000029a1b607c <.xdata>:
-   29a1b607c:	add    %eax,(%rcx,%rax,1)
-   29a1b607f:	add    %al,(%rdx,%rax,2)
-   29a1b6082:	add    %al,(%rax)
-   29a1b6084:	add    %eax,(%rsi)
-   29a1b6086:	add    (%rax),%eax
-   29a1b6088:	(bad)
-   29a1b6089:	rex.X add (%rax),%sil
-   29a1b608c:	add    %esp,0x0(%rax)
-   29a1b608f:	add    %al,(%rcx)
-   29a1b6091:	add    %al,(%rax)
-	...
-
-000000029a1b6094 <.xdata>:
-   29a1b6094:	add    %eax,(%rsi)
-   29a1b6096:	add    (%rax),%eax
-   29a1b6098:	(bad)
-   29a1b6099:	(bad)
-   29a1b609e:	add    %al,(%rax)
-   29a1b60a0:	add    %eax,(%rdi)
-   29a1b60a2:	add    $0x0,%al
-   29a1b60a4:	(bad)
-   29a1b60a5:	xchg   %eax,%edx
-   29a1b60a6:	add    (%rax),%esi
-   29a1b60a8:	add    0x1(%rax),%ah
-   29a1b60ab:	jo     29a1b60ae <.xdata+0x1a>
-   29a1b60ad:	adc    $0x315450a,%eax
-   29a1b60b2:	adc    %al,0x600b300c(%rdx)
-   29a1b60b8:	or     0x9(%rax),%dh
-   29a1b60bb:	rolb   $0xd0,(%rdi)
-   29a1b60be:	add    $0x1f003e0,%eax
-   29a1b60c3:	push   %rax
-
-000000029a1b60c4 <.xdata>:
-   29a1b60c4:	add    %ecx,(%rdx)
-   29a1b60c6:	(bad)
-   29a1b60c7:	add    %cl,(%rdx)
-   29a1b60c9:	xor    (%rsi),%al
-   29a1b60cb:	xor    %al,0x3700460(%rip)        # 29d8b6531 <.debug_rnglists+0x36e648d>
-   29a1b60d1:	push   %rax
-   29a1b60d2:	add    %al,%al
-   29a1b60d4:	add    %eax,(%rdi)
-   29a1b60d6:	add    $0x0,%al
-   29a1b60d8:	(bad)
-   29a1b60d9:	xor    (%rbx),%al
-   29a1b60db:	xor    %al,(%rdx)
+   29a1b6038:	add    %eax,(%rdx,%rax,1)
+   29a1b603b:	add    $0x50010304,%eax
+   29a1b6040:	add    %ecx,(%rax)
+   29a1b6042:	add    0x3043208(%rip),%eax        # 29d1f9250 <.debug_rnglists+0x30291ac>
+   29a1b6048:	add    %edx,0x0(%rax)
+   29a1b604b:	add    %al,(%rcx)
+   29a1b604d:	or     %al,(%rbx)
+   29a1b604f:	add    $0x3045208,%eax
+   29a1b6054:	add    %edx,0x0(%rax)
+   29a1b6057:	add    %al,(%rcx)
+   29a1b6059:	add    $0x2,%al
+   29a1b605b:	add    $0x50010304,%eax
+
+000000029a1b6060 <.xdata>:
+   29a1b6060:	add    %eax,(%rcx,%rax,1)
+   29a1b6063:	add    %al,(%rdx,%rax,2)
+   29a1b6066:	add    %al,(%rax)
+   29a1b6068:	add    %eax,(%rsi)
+   29a1b606a:	add    (%rax),%eax
+   29a1b606c:	(bad)
+   29a1b606d:	rex.X add (%rax),%sil
+   29a1b6070:	add    %esp,0x0(%rax)
+   29a1b6073:	add    %al,(%rcx)
+   29a1b6075:	add    %al,(%rax)
+	...
+
+000000029a1b6078 <.xdata>:
+   29a1b6078:	add    %eax,(%rcx,%rax,1)
+   29a1b607b:	add    %al,(%rdx,%rax,2)
+   29a1b607e:	add    %al,(%rax)
+   29a1b6080:	add    %eax,(%rsi)
+   29a1b6082:	add    (%rax),%eax
+   29a1b6084:	(bad)
+   29a1b6085:	rex.X add (%rax),%sil
+   29a1b6088:	add    %esp,0x0(%rax)
+   29a1b608b:	add    %al,(%rcx)
+   29a1b608d:	add    %al,(%rax)
+	...
+
+000000029a1b6090 <.xdata>:
+   29a1b6090:	add    %eax,(%rsi)
+   29a1b6092:	add    (%rax),%eax
+   29a1b6094:	(bad)
+   29a1b6095:	(bad)
+   29a1b609a:	add    %al,(%rax)
+   29a1b609c:	add    %eax,(%rdi)
+   29a1b609e:	add    $0x0,%al
+   29a1b60a0:	(bad)
+   29a1b60a1:	xchg   %eax,%edx
+   29a1b60a2:	add    (%rax),%esi
+   29a1b60a4:	add    0x1(%rax),%ah
+   29a1b60a7:	jo     29a1b60aa <.xdata+0x1a>
+   29a1b60a9:	adc    $0x315450a,%eax
+   29a1b60ae:	adc    %al,0x600b300c(%rdx)
+   29a1b60b4:	or     0x9(%rax),%dh
+   29a1b60b7:	rolb   $0xd0,(%rdi)
+   29a1b60ba:	add    $0x1f003e0,%eax
+   29a1b60bf:	push   %rax
+
+000000029a1b60c0 <.xdata>:
+   29a1b60c0:	add    %ecx,(%rdx)
+   29a1b60c2:	(bad)
+   29a1b60c3:	add    %cl,(%rdx)
+   29a1b60c5:	xor    (%rsi),%al
+   29a1b60c7:	xor    %al,0x3700460(%rip)        # 29d8b652d <.debug_rnglists+0x36e6489>
+   29a1b60cd:	push   %rax
+   29a1b60ce:	add    %al,%al
+   29a1b60d0:	add    %eax,(%rdi)
+   29a1b60d2:	add    $0x0,%al
+   29a1b60d4:	(bad)
+   29a1b60d5:	xor    (%rbx),%al
+   29a1b60d7:	xor    %al,(%rdx)
+   29a1b60d9:	(bad)
+   29a1b60da:	add    %esi,0x1(%rax)
    29a1b60dd:	(bad)
-   29a1b60de:	add    %esi,0x1(%rax)
-   29a1b60e1:	(bad)
-   29a1b60e2:	add    (%rax),%eax
-   29a1b60e4:	(bad)
-   29a1b60e5:	rex.X add (%rax),%sil
-   29a1b60e8:	add    %esp,0x0(%rax)
-   29a1b60eb:	add    %al,(%rcx)
-   29a1b60ed:	add    $0x32050002,%eax
-   29a1b60f2:	add    %esi,(%rax)
-
-000000029a1b60f4 <.xdata>:
+   29a1b60de:	add    (%rax),%eax
+   29a1b60e0:	(bad)
+   29a1b60e1:	rex.X add (%rax),%sil
+   29a1b60e4:	add    %esp,0x0(%rax)
+   29a1b60e7:	add    %al,(%rcx)
+   29a1b60e9:	add    $0x32050002,%eax
+   29a1b60ee:	add    %esi,(%rax)
+
+000000029a1b60f0 <.xdata>:
+   29a1b60f0:	add    %eax,(%rax)
+   29a1b60f2:	add    %al,(%rax)
    29a1b60f4:	add    %eax,(%rax)
    29a1b60f6:	add    %al,(%rax)
-   29a1b60f8:	add    %eax,(%rax)
-   29a1b60fa:	add    %al,(%rax)
-   29a1b60fc:	add    %eax,(%rdi)
-   29a1b60fe:	add    $0x0,%al
-   29a1b6100:	(bad)
-   29a1b6101:	xor    (%rbx),%al
-   29a1b6103:	xor    %al,(%rdx)
-   29a1b6105:	(bad)
-   29a1b6106:	add    %esi,0x1(%rax)
+   29a1b60f8:	add    %eax,(%rdi)
+   29a1b60fa:	add    $0x0,%al
+   29a1b60fc:	(bad)
+   29a1b60fd:	xor    (%rbx),%al
+   29a1b60ff:	xor    %al,(%rdx)
+   29a1b6101:	(bad)
+   29a1b6102:	add    %esi,0x1(%rax)
+   29a1b6105:	add    %al,(%rax)
+   29a1b6107:	add    %al,(%rcx)
    29a1b6109:	add    %al,(%rax)
    29a1b610b:	add    %al,(%rcx)
    29a1b610d:	add    %al,(%rax)
    29a1b610f:	add    %al,(%rcx)
    29a1b6111:	add    %al,(%rax)
    29a1b6113:	add    %al,(%rcx)
    29a1b6115:	add    %al,(%rax)
    29a1b6117:	add    %al,(%rcx)
    29a1b6119:	add    %al,(%rax)
-   29a1b611b:	add    %al,(%rcx)
-   29a1b611d:	add    %al,(%rax)
+	...
+
+000000029a1b611c <.xdata>:
+   29a1b611c:	add    %eax,(%rax)
 	...
 
 000000029a1b6120 <.xdata>:
    29a1b6120:	add    %eax,(%rax)
 	...
 
 000000029a1b6124 <.xdata>:
    29a1b6124:	add    %eax,(%rax)
 	...
 
 000000029a1b6128 <.xdata>:
-   29a1b6128:	add    %eax,(%rax)
+   29a1b6128:	add    %eax,(%rcx,%rax,1)
+   29a1b612b:	add    %al,(%rdx,%riz,2)
 	...
 
-000000029a1b612c <.xdata>:
-   29a1b612c:	add    %eax,(%rcx,%rax,1)
-   29a1b612f:	add    %al,(%rdx,%riz,2)
-	...
-
-000000029a1b6134 <.xdata>:
-   29a1b6134:	add    %eax,(%rax)
-   29a1b6136:	add    %al,(%rax)
-   29a1b6138:	add    %ecx,(%rdx)
-   29a1b613a:	(bad)
-   29a1b613b:	add    %cl,(%rdx)
-   29a1b613d:	xor    (%rsi),%al
-   29a1b613f:	xor    %al,0x3700460(%rip)        # 29d8b65a5 <.debug_rnglists+0x36e6501>
-   29a1b6145:	push   %rax
-   29a1b6146:	add    %al,%al
-   29a1b6148:	add    %ecx,(%rdx)
-   29a1b614a:	(bad)
-   29a1b614b:	add    %cl,(%rdx)
-   29a1b614d:	xor    (%rsi),%al
-   29a1b614f:	xor    %al,0x3700460(%rip)        # 29d8b65b5 <.debug_rnglists+0x36e6511>
-   29a1b6155:	push   %rax
-   29a1b6156:	add    %al,%al
-   29a1b6158:	add    %eax,0x32050002(%rip)        # 2cc206160 <.debug_rnglists+0x320360bc>
-   29a1b615e:	add    %esi,(%rax)
-   29a1b6160:	add    %eax,(%rax)
-   29a1b6162:	add    %al,(%rax)
-   29a1b6164:	add    %eax,0x32050002(%rip)        # 2cc20616c <.debug_rnglists+0x320360c8>
-   29a1b616a:	add    %esi,(%rax)
-   29a1b616c:	add    %eax,(%rcx,%rax,1)
-   29a1b616f:	add    %al,(%rdx,%rax,4)
-   29a1b6172:	add    %al,(%rax)
-   29a1b6174:	add    %eax,(%rcx,%rax,1)
-   29a1b6177:	add    %al,(%rdx,%rax,2)
-   29a1b617a:	add    %al,(%rax)
-   29a1b617c:	add    %eax,(%rcx,%rax,1)
-   29a1b617f:	add    %al,(%rdx,%rax,2)
-	...
-
-000000029a1b6184 <.xdata>:
-   29a1b6184:	add    %eax,(%rcx,%rax,1)
-   29a1b6187:	add    %al,(%rdx,%rax,4)
+000000029a1b6130 <.xdata>:
+   29a1b6130:	add    %eax,(%rax)
+   29a1b6132:	add    %al,(%rax)
+   29a1b6134:	add    %ecx,(%rdx)
+   29a1b6136:	(bad)
+   29a1b6137:	add    %cl,(%rdx)
+   29a1b6139:	xor    (%rsi),%al
+   29a1b613b:	xor    %al,0x3700460(%rip)        # 29d8b65a1 <.debug_rnglists+0x36e64fd>
+   29a1b6141:	push   %rax
+   29a1b6142:	add    %al,%al
+   29a1b6144:	add    %ecx,(%rdx)
+   29a1b6146:	(bad)
+   29a1b6147:	add    %cl,(%rdx)
+   29a1b6149:	xor    (%rsi),%al
+   29a1b614b:	xor    %al,0x3700460(%rip)        # 29d8b65b1 <.debug_rnglists+0x36e650d>
+   29a1b6151:	push   %rax
+   29a1b6152:	add    %al,%al
+   29a1b6154:	add    %eax,0x32050002(%rip)        # 2cc20615c <.debug_rnglists+0x320360b8>
+   29a1b615a:	add    %esi,(%rax)
+   29a1b615c:	add    %eax,(%rax)
+   29a1b615e:	add    %al,(%rax)
+   29a1b6160:	add    %eax,0x32050002(%rip)        # 2cc206168 <.debug_rnglists+0x320360c4>
+   29a1b6166:	add    %esi,(%rax)
+   29a1b6168:	add    %eax,(%rcx,%rax,1)
+   29a1b616b:	add    %al,(%rdx,%rax,4)
+   29a1b616e:	add    %al,(%rax)
+   29a1b6170:	add    %eax,(%rcx,%rax,1)
+   29a1b6173:	add    %al,(%rdx,%rax,2)
+   29a1b6176:	add    %al,(%rax)
+   29a1b6178:	add    %eax,(%rcx,%rax,1)
+   29a1b617b:	add    %al,(%rdx,%rax,2)
+	...
+
+000000029a1b6180 <.xdata>:
+   29a1b6180:	add    %eax,(%rcx,%rax,1)
+   29a1b6183:	add    %al,(%rdx,%rax,4)
 	...
 
-000000029a1b618c <.xdata.startup>:
-   29a1b618c:	add    %eax,(%rax)
+000000029a1b6188 <.xdata.startup>:
+   29a1b6188:	add    %eax,(%rax)
 	...
 
 Disassembly of section .edata:
 
 000000029a1b8000 <.edata>:
    29a1b8000:	add    %al,(%rax)
    29a1b8002:	add    %al,(%rax)
-   29a1b8004:	adc    %ch,%ch
-   29a1b8006:	xor    %esp,0x0(%rsi)
+   29a1b8004:	fiadds (%rdi)
+   29a1b8006:	xor    0x0(%rsi),%ah
    29a1b8009:	add    %al,(%rax)
    29a1b800b:	add    %dl,-0x80(%rax)
    29a1b800e:	add    %al,(%rax)
    29a1b8010:	add    %eax,(%rax)
    29a1b8012:	add    %al,(%rax)
    29a1b8014:	add    $0x0,%al
    29a1b8016:	add    %al,(%rax)
    29a1b8018:	add    $0x0,%al
    29a1b801a:	add    %al,(%rax)
    29a1b801c:	sub    %al,-0x7fc80000(%rax)
    29a1b8022:	add    %al,(%rax)
    29a1b8024:	rex.W addb $0x0,(%rax)
-   29a1b8028:	mov    $0x80000013,%eax
-   29a1b802d:	adc    (%rax),%eax
-   29a1b802f:	add    %ah,-0x13ffffed(%rbp)
+   29a1b8028:	(bad)
+   29a1b8029:	adc    (%rax),%eax
+   29a1b802b:	add    %al,-0x78ffffed(%rax)
+   29a1b8031:	adc    (%rax),%eax
+   29a1b8033:	add    %cl,%dh
    29a1b8035:	adc    (%rax),%eax
    29a1b8037:	add    %ah,-0x80(%rbx)
    29a1b803a:	add    %al,(%rax)
    29a1b803c:	jo     29a1b7fbe <__bss_end__+0xeae>
    29a1b803e:	add    %al,(%rax)
    29a1b8040:	jne    29a1b7fc2 <__bss_end__+0xeb2>
    29a1b8042:	add    %al,(%rax)
@@ -5925,1150 +5921,1158 @@
 Disassembly of section .idata:
 
 000000029a1b9000 <_head_lib64_libkernel32_a>:
    29a1b9000:	mov    $0x90,%eax
    29a1b9005:	add    %al,(%rax)
    29a1b9007:	add    %al,(%rax)
    29a1b9009:	add    %al,(%rax)
-   29a1b900b:	add    %ch,%al
+   29a1b900b:	add    %dl,%al
    29a1b900d:	xchg   %eax,%esi
    29a1b900e:	add    %al,(%rax)
-   29a1b9010:	push   %rax
-   29a1b9011:	xchg   %eax,%edx
+   29a1b9010:	xchg   %rax,%rdx
 	...
 
 000000029a1b9014 <_head_lib64_libapi_ms_win_crt_conio_l1_1_0_a>:
    29a1b9014:	or     %dl,0x0(%rcx)
    29a1b901a:	add    %al,(%rax)
    29a1b901c:	add    %al,(%rax)
    29a1b901e:	add    %al,(%rax)
-   29a1b9020:	cld
-   29a1b9021:	xchg   %eax,%esi
+   29a1b9020:	in     $0x96,%al
    29a1b9022:	add    %al,(%rax)
-   29a1b9024:	movabs 0x9118000092,%al
+   29a1b9024:	cwtl
+   29a1b9025:	xchg   %eax,%edx
+	...
 
 000000029a1b9028 <_head_lib64_libapi_ms_win_crt_environment_l1_1_0_a>:
    29a1b9028:	sbb    %dl,0x0(%rcx)
    29a1b902e:	add    %al,(%rax)
    29a1b9030:	add    %al,(%rax)
    29a1b9032:	add    %al,(%rax)
-   29a1b9034:	and    $0x97,%al
+   29a1b9034:	or     $0x97,%al
    29a1b9036:	add    %al,(%rax)
-   29a1b9038:	mov    $0x92,%al
+   29a1b9038:	test   $0x92,%al
 	...
 
 000000029a1b903c <_head_lib64_libapi_ms_win_crt_heap_l1_1_0_a>:
    29a1b903c:	xor    %dl,0x0(%rcx)
    29a1b9042:	add    %al,(%rax)
    29a1b9044:	add    %al,(%rax)
    29a1b9046:	add    %al,(%rax)
-   29a1b9048:	pop    %rax
-   29a1b9049:	xchg   %eax,%edi
+   29a1b9048:	rex xchg %eax,%edi
    29a1b904a:	add    %al,(%rax)
-   29a1b904c:	enter  $0x92,$0x0
+   29a1b904c:	rclb   $0x0,-0x6eb00000(%rdx)
 
 000000029a1b9050 <_head_lib64_libapi_ms_win_crt_runtime_l1_1_0_a>:
    29a1b9050:	push   %rax
    29a1b9051:	xchg   %eax,%ecx
 	...
    29a1b905a:	add    %al,(%rax)
-   29a1b905c:	mov    $0x97,%ah
+   29a1b905c:	pushf
+   29a1b905d:	xchg   %eax,%edi
    29a1b905e:	add    %al,(%rax)
-   29a1b9060:	call   26a1b90f7 <__size_of_stack_reserve__+0x269fb90f7>
+   29a1b9060:	loopne 29a1b8ff4 <__bss_end__+0x1ee4>
+	...
 
 000000029a1b9064 <_head_lib64_libapi_ms_win_crt_stdio_l1_1_0_a>:
    29a1b9064:	rclb   $1,0x0(%rcx)
    29a1b906a:	add    %al,(%rax)
    29a1b906c:	add    %al,(%rax)
    29a1b906e:	add    %al,(%rax)
-   29a1b9070:	hlt
-   29a1b9071:	xchg   %eax,%edi
-   29a1b9072:	add    %al,(%rax)
-   29a1b9074:	push   $0x10000093
+   29a1b9070:	fcoms  -0x6ca00000(%rdi)
+	...
 
 000000029a1b9078 <_head_lib64_libapi_ms_win_crt_string_l1_1_0_a>:
-   29a1b9078:	adc    %dl,0x0(%rdx)
+   29a1b9078:	or     %dl,0x0(%rdx)
    29a1b907e:	add    %al,(%rax)
    29a1b9080:	add    %al,(%rax)
    29a1b9082:	add    %al,(%rax)
-   29a1b9084:	sbb    $0x98,%al
-   29a1b9086:	add    %al,(%rax)
-   29a1b9088:	test   $0x93,%al
+   29a1b9084:	add    %bl,-0x6c680000(%rax)
 	...
 
 000000029a1b908c <_head_lib64_libapi_ms_win_crt_time_l1_1_0_a>:
-   29a1b908c:	sub    %dl,0x0(%rdx)
+   29a1b908c:	and    %dl,0x0(%rdx)
    29a1b9092:	add    %al,(%rax)
    29a1b9094:	add    %al,(%rax)
    29a1b9096:	add    %al,(%rax)
-   29a1b9098:	push   %rax
-   29a1b9099:	cwtl
+   29a1b9098:	xor    $0x98,%al
    29a1b909a:	add    %al,(%rax)
-   29a1b909c:	rclb   $0x0,0x0(%rbx)
+   29a1b909c:	mov    $0x93,%al
 	...
 
 000000029a1b90b8 <hname>:
-   29a1b90b8:	call   29a1b9150 <hname>
-   29a1b90bd:	add    %al,(%rax)
+   29a1b90b8:	fcoms  0x0(%rbx)
 	...
 
 000000029a1b90c0 <.idata$4>:
-   29a1b90c0:	add    %dl,0x0(%rax,%rax,1)
+   29a1b90c0:	lock xchg %eax,%ebx
+   29a1b90c2:	add    %al,(%rax)
+   29a1b90c4:	add    %al,(%rax)
 	...
 
 000000029a1b90c8 <.idata$4>:
-   29a1b90c8:	sbb    %dl,0x0(%rax,%rax,1)
+   29a1b90c8:	or     %dl,0x0(%rax,%rax,1)
 	...
 
 000000029a1b90d0 <.idata$4>:
-   29a1b90d0:	sub    %dl,0x0(%rax,%rax,1)
+   29a1b90d0:	sbb    %dl,0x0(%rax,%rax,1)
 	...
 
 000000029a1b90d8 <.idata$4>:
-   29a1b90d8:	rex.R xchg %eax,%esp
+   29a1b90d8:	xor    $0x94,%al
    29a1b90da:	add    %al,(%rax)
    29a1b90dc:	add    %al,(%rax)
 	...
 
 000000029a1b90e0 <.idata$4>:
-   29a1b90e0:	pop    %rsp
-   29a1b90e1:	xchg   %eax,%esp
+   29a1b90e0:	rex.WR xchg %rax,%rsp
    29a1b90e2:	add    %al,(%rax)
    29a1b90e4:	add    %al,(%rax)
 	...
 
 000000029a1b90e8 <.idata$4>:
-   29a1b90e8:	fs xchg %eax,%esp
+   29a1b90e8:	push   %rsp
+   29a1b90e9:	xchg   %eax,%esp
    29a1b90ea:	add    %al,(%rax)
    29a1b90ec:	add    %al,(%rax)
 	...
 
 000000029a1b90f0 <.idata$4>:
-   29a1b90f0:	jb     29a1b9086 <_head_lib64_libapi_ms_win_crt_string_l1_1_0_a+0xe>
-   29a1b90f2:	add    %al,(%rax)
-   29a1b90f4:	add    %al,(%rax)
+   29a1b90f0:	(bad)
+   29a1b90f3:	add    %al,(%rax)
+   29a1b90f5:	add    %al,(%rax)
 	...
 
 000000029a1b90f8 <.idata$4>:
-   29a1b90f8:	test   %dl,0x0(%rax,%rax,1)
+   29a1b90f8:	je     29a1b908e <_head_lib64_libapi_ms_win_crt_time_l1_1_0_a+0x2>
+   29a1b90fa:	add    %al,(%rax)
+   29a1b90fc:	add    %al,(%rax)
 	...
 
 000000029a1b9100 <.idata$4>:
 	...
 
 000000029a1b9108 <hname>:
-   29a1b9108:	xchg   %eax,%esp
-   29a1b9109:	xchg   %eax,%esp
-   29a1b910a:	add    %al,(%rax)
-   29a1b910c:	add    %al,(%rax)
+   29a1b9108:	test   %dl,0x0(%rax,%rax,1)
 	...
 
 000000029a1b9110 <.idata$4>:
 	...
 
 000000029a1b9118 <hname>:
-   29a1b9118:	sahf
-   29a1b9119:	xchg   %eax,%esp
-   29a1b911a:	add    %al,(%rax)
-   29a1b911c:	add    %al,(%rax)
+   29a1b9118:	mov    0x0(%rax,%rax,1),%ss
 	...
 
 000000029a1b9120 <.idata$4>:
-   29a1b9120:	scas   %es:(%rdi),%al
+   29a1b9120:	sahf
    29a1b9121:	xchg   %eax,%esp
    29a1b9122:	add    %al,(%rax)
    29a1b9124:	add    %al,(%rax)
 	...
 
 000000029a1b9128 <.idata$4>:
 	...
 
 000000029a1b9130 <hname>:
-   29a1b9130:	mov    $0x94,%esi
-   29a1b9135:	add    %al,(%rax)
+   29a1b9130:	scas   %es:(%rdi),%al
+   29a1b9131:	xchg   %eax,%esp
+   29a1b9132:	add    %al,(%rax)
+   29a1b9134:	add    %al,(%rax)
 	...
 
 000000029a1b9138 <.idata$4>:
-   29a1b9138:	(bad)
-   29a1b9139:	xchg   %eax,%esp
-   29a1b913a:	add    %al,(%rax)
-   29a1b913c:	add    %al,(%rax)
+   29a1b9138:	mov    $0x94,%esi
+   29a1b913d:	add    %al,(%rax)
 	...
 
 000000029a1b9140 <.idata$4>:
-   29a1b9140:	fcoms  0x0(%rax,%rax,1)
+   29a1b9140:	enter  $0x94,$0x0
+   29a1b9144:	add    %al,(%rax)
 	...
 
 000000029a1b9148 <.idata$4>:
 	...
 
 000000029a1b9150 <hname>:
-   29a1b9150:	loopne 29a1b90e6 <.idata$4+0x6>
-   29a1b9152:	add    %al,(%rax)
-   29a1b9154:	add    %al,(%rax)
+   29a1b9150:	rclb   $1,0x0(%rax,%rax,1)
 	...
 
 000000029a1b9158 <.idata$4>:
-   29a1b9158:	out    %al,(%dx)
-   29a1b9159:	xchg   %eax,%esp
-   29a1b915a:	add    %al,(%rax)
-   29a1b915c:	add    %al,(%rax)
+   29a1b9158:	ficoms 0x0(%rax,%rax,1)
 	...
 
 000000029a1b9160 <.idata$4>:
-   29a1b9160:	cld
+   29a1b9160:	in     (%dx),%al
    29a1b9161:	xchg   %eax,%esp
    29a1b9162:	add    %al,(%rax)
    29a1b9164:	add    %al,(%rax)
 	...
 
 000000029a1b9168 <.idata$4>:
-   29a1b9168:	or     0x0(%rbp),%dl
+   29a1b9168:	cli
+   29a1b9169:	xchg   %eax,%esp
+   29a1b916a:	add    %al,(%rax)
+   29a1b916c:	add    %al,(%rax)
 	...
 
 000000029a1b9170 <.idata$4>:
-   29a1b9170:	and    $0x95,%al
+   29a1b9170:	adc    $0x95,%al
    29a1b9172:	add    %al,(%rax)
    29a1b9174:	add    %al,(%rax)
 	...
 
 000000029a1b9178 <.idata$4>:
-   29a1b9178:	cmp    $0x95,%al
+   29a1b9178:	sub    $0x95,%al
    29a1b917a:	add    %al,(%rax)
    29a1b917c:	add    %al,(%rax)
 	...
 
 000000029a1b9180 <.idata$4>:
-   29a1b9180:	push   %rdx
-   29a1b9181:	xchg   %eax,%ebp
+   29a1b9180:	rex.X xchg %eax,%ebp
    29a1b9182:	add    %al,(%rax)
    29a1b9184:	add    %al,(%rax)
 	...
 
 000000029a1b9188 <.idata$4>:
-   29a1b9188:	(bad)
+   29a1b9188:	push   %rax
    29a1b9189:	xchg   %eax,%ebp
    29a1b918a:	add    %al,(%rax)
    29a1b918c:	add    %al,(%rax)
 	...
 
 000000029a1b9190 <.idata$4>:
-   29a1b9190:	js     29a1b9127 <.idata$4+0x7>
-   29a1b9192:	add    %al,(%rax)
-   29a1b9194:	add    %al,(%rax)
+   29a1b9190:	push   $0x95
+   29a1b9195:	add    %al,(%rax)
 	...
 
 000000029a1b9198 <.idata$4>:
-   29a1b9198:	adcb   $0x0,0x0(%rbp)
+   29a1b9198:	jo     29a1b912f <.idata$4+0x7>
+   29a1b919a:	add    %al,(%rax)
+   29a1b919c:	add    %al,(%rax)
 	...
 
 000000029a1b91a0 <.idata$4>:
-   29a1b91a0:	movabs %al,0xbe00000000000095
+   29a1b91a0:	xchg   %eax,%edx
+   29a1b91a1:	xchg   %eax,%ebp
+   29a1b91a2:	add    %al,(%rax)
+   29a1b91a4:	add    %al,(%rax)
+	...
 
 000000029a1b91a8 <.idata$4>:
-   29a1b91a8:	mov    $0x95,%esi
-   29a1b91ad:	add    %al,(%rax)
+   29a1b91a8:	scas   %es:(%rdi),%al
+   29a1b91a9:	xchg   %eax,%ebp
+   29a1b91aa:	add    %al,(%rax)
+   29a1b91ac:	add    %al,(%rax)
 	...
 
 000000029a1b91b0 <.idata$4>:
-   29a1b91b0:	ficoms 0x0(%rbp)
+   29a1b91b0:	(bad)
+   29a1b91b1:	xchg   %eax,%ebp
+   29a1b91b2:	add    %al,(%rax)
+   29a1b91b4:	add    %al,(%rax)
 	...
 
 000000029a1b91b8 <.idata$4>:
-   29a1b91b8:	(bad)
-   29a1b91b9:	xchg   %eax,%ebp
-   29a1b91ba:	add    %al,(%rax)
-   29a1b91bc:	add    %al,(%rax)
+   29a1b91b8:	ficoml 0x0(%rbp)
 	...
 
 000000029a1b91c0 <.idata$4>:
-   29a1b91c0:	(bad)
-   29a1b91c1:	xchg   %eax,%esi
-   29a1b91c2:	add    %al,(%rax)
-   29a1b91c4:	add    %al,(%rax)
+   29a1b91c0:	notb   0x0(%rbp)
 	...
 
 000000029a1b91c8 <.idata$4>:
 	...
 
 000000029a1b91d0 <hname>:
    29a1b91d0:	(bad)
-   29a1b91d1:	xchg   %eax,%esi
+   29a1b91d1:	xchg   %eax,%ebp
    29a1b91d2:	add    %al,(%rax)
    29a1b91d4:	add    %al,(%rax)
 	...
 
 000000029a1b91d8 <.idata$4>:
-   29a1b91d8:	and    %dl,0x0(%rsi)
+   29a1b91d8:	adc    %dl,0x0(%rsi)
 	...
 
 000000029a1b91e0 <.idata$4>:
-   29a1b91e0:	cmp    0x0(%rsi),%dl
+   29a1b91e0:	sub    0x0(%rsi),%dl
 	...
 
 000000029a1b91e8 <.idata$4>:
-   29a1b91e8:	push   %rsi
-   29a1b91e9:	xchg   %eax,%esi
+   29a1b91e8:	rex.RX xchg %eax,%esi
    29a1b91ea:	add    %al,(%rax)
    29a1b91ec:	add    %al,(%rax)
 	...
 
 000000029a1b91f0 <.idata$4>:
-   29a1b91f0:	(bad)
+   29a1b91f0:	push   %rax
    29a1b91f1:	xchg   %eax,%esi
    29a1b91f2:	add    %al,(%rax)
    29a1b91f4:	add    %al,(%rax)
 	...
 
 000000029a1b91f8 <.idata$4>:
-   29a1b91f8:	push   $0xffffffffffffff96
+   29a1b91f8:	pop    %rdx
+   29a1b91f9:	xchg   %eax,%esi
    29a1b91fa:	add    %al,(%rax)
    29a1b91fc:	add    %al,(%rax)
 	...
 
 000000029a1b9200 <.idata$4>:
-   29a1b9200:	je     29a1b9198 <.idata$4>
-   29a1b9202:	add    %al,(%rax)
-   29a1b9204:	add    %al,(%rax)
 	...
 
-000000029a1b9208 <.idata$4>:
+000000029a1b9208 <hname>:
+   29a1b9208:	fs xchg %eax,%esi
+   29a1b920a:	add    %al,(%rax)
+   29a1b920c:	add    %al,(%rax)
 	...
 
-000000029a1b9210 <hname>:
-   29a1b9210:	jle    29a1b91a8 <.idata$4>
+000000029a1b9210 <.idata$4>:
+   29a1b9210:	outsb  %ds:(%rsi),(%dx)
+   29a1b9211:	xchg   %eax,%esi
    29a1b9212:	add    %al,(%rax)
    29a1b9214:	add    %al,(%rax)
 	...
 
 000000029a1b9218 <.idata$4>:
-   29a1b9218:	mov    %dl,0x0(%rsi)
 	...
 
-000000029a1b9220 <.idata$4>:
+000000029a1b9220 <hname>:
+   29a1b9220:	js     29a1b91b8 <.idata$4>
+   29a1b9222:	add    %al,(%rax)
+   29a1b9224:	add    %al,(%rax)
 	...
 
-000000029a1b9228 <hname>:
-   29a1b9228:	xchg   %eax,%edx
-   29a1b9229:	xchg   %eax,%esi
-   29a1b922a:	add    %al,(%rax)
-   29a1b922c:	add    %al,(%rax)
+000000029a1b9228 <.idata$4>:
+   29a1b9228:	xchg   %dl,0x0(%rsi)
 	...
 
 000000029a1b9230 <.idata$4>:
-   29a1b9230:	movabs 0xae00000000000096,%al
+   29a1b9230:	xchg   %eax,%esp
+   29a1b9231:	xchg   %eax,%esi
+   29a1b9232:	add    %al,(%rax)
+   29a1b9234:	add    %al,(%rax)
+	...
 
 000000029a1b9238 <.idata$4>:
-   29a1b9238:	scas   %es:(%rdi),%al
-   29a1b9239:	xchg   %eax,%esi
-   29a1b923a:	add    %al,(%rax)
-   29a1b923c:	add    %al,(%rax)
-	...
+   29a1b9238:	movabs 0x96,%al
 
 000000029a1b9240 <.idata$4>:
-   29a1b9240:	mov    $0x96,%edx
-   29a1b9245:	add    %al,(%rax)
 	...
 
-000000029a1b9248 <.idata$4>:
+000000029a1b9248 <__IAT_start__>:
+   29a1b9248:	fcoms  0x0(%rbx)
 	...
 
-000000029a1b9250 <__IAT_start__>:
-   29a1b9250:	call   29a1b92e8 <__imp___p___argc>
-   29a1b9255:	add    %al,(%rax)
+000000029a1b9250 <__imp_EnterCriticalSection>:
+   29a1b9250:	lock xchg %eax,%ebx
+   29a1b9252:	add    %al,(%rax)
+   29a1b9254:	add    %al,(%rax)
 	...
 
-000000029a1b9258 <__imp_EnterCriticalSection>:
-   29a1b9258:	add    %dl,0x0(%rax,%rax,1)
+000000029a1b9258 <__imp_GetLastError>:
+   29a1b9258:	or     %dl,0x0(%rax,%rax,1)
 	...
 
-000000029a1b9260 <__imp_GetLastError>:
+000000029a1b9260 <__imp_InitializeCriticalSection>:
    29a1b9260:	sbb    %dl,0x0(%rax,%rax,1)
 	...
 
-000000029a1b9268 <__imp_InitializeCriticalSection>:
-   29a1b9268:	sub    %dl,0x0(%rax,%rax,1)
+000000029a1b9268 <__imp_LeaveCriticalSection>:
+   29a1b9268:	xor    $0x94,%al
+   29a1b926a:	add    %al,(%rax)
+   29a1b926c:	add    %al,(%rax)
 	...
 
-000000029a1b9270 <__imp_LeaveCriticalSection>:
-   29a1b9270:	rex.R xchg %eax,%esp
+000000029a1b9270 <__imp_Sleep>:
+   29a1b9270:	rex.WR xchg %rax,%rsp
    29a1b9272:	add    %al,(%rax)
    29a1b9274:	add    %al,(%rax)
 	...
 
-000000029a1b9278 <__imp_Sleep>:
-   29a1b9278:	pop    %rsp
+000000029a1b9278 <__imp_TlsGetValue>:
+   29a1b9278:	push   %rsp
    29a1b9279:	xchg   %eax,%esp
    29a1b927a:	add    %al,(%rax)
    29a1b927c:	add    %al,(%rax)
 	...
 
-000000029a1b9280 <__imp_TlsGetValue>:
-   29a1b9280:	fs xchg %eax,%esp
-   29a1b9282:	add    %al,(%rax)
-   29a1b9284:	add    %al,(%rax)
+000000029a1b9280 <__imp_VirtualProtect>:
+   29a1b9280:	(bad)
+   29a1b9283:	add    %al,(%rax)
+   29a1b9285:	add    %al,(%rax)
 	...
 
-000000029a1b9288 <__imp_VirtualProtect>:
-   29a1b9288:	jb     29a1b921e <.idata$4+0x6>
+000000029a1b9288 <__imp_VirtualQuery>:
+   29a1b9288:	je     29a1b921e <.idata$4+0x6>
    29a1b928a:	add    %al,(%rax)
    29a1b928c:	add    %al,(%rax)
 	...
 
-000000029a1b9290 <__imp_VirtualQuery>:
-   29a1b9290:	test   %dl,0x0(%rax,%rax,1)
+000000029a1b9290 <.idata$5>:
 	...
 
-000000029a1b9298 <.idata$5>:
+000000029a1b9298 <__imp_getch>:
+   29a1b9298:	test   %dl,0x0(%rax,%rax,1)
 	...
 
-000000029a1b92a0 <__imp_getch>:
-   29a1b92a0:	xchg   %eax,%esp
-   29a1b92a1:	xchg   %eax,%esp
-   29a1b92a2:	add    %al,(%rax)
-   29a1b92a4:	add    %al,(%rax)
+000000029a1b92a0 <.idata$5>:
 	...
 
-000000029a1b92a8 <.idata$5>:
+000000029a1b92a8 <__imp___p__environ>:
+   29a1b92a8:	mov    0x0(%rax,%rax,1),%ss
 	...
 
-000000029a1b92b0 <__imp___p__environ>:
+000000029a1b92b0 <__imp___p__wenviron>:
    29a1b92b0:	sahf
    29a1b92b1:	xchg   %eax,%esp
    29a1b92b2:	add    %al,(%rax)
    29a1b92b4:	add    %al,(%rax)
 	...
 
-000000029a1b92b8 <__imp___p__wenviron>:
-   29a1b92b8:	scas   %es:(%rdi),%al
-   29a1b92b9:	xchg   %eax,%esp
-   29a1b92ba:	add    %al,(%rax)
-   29a1b92bc:	add    %al,(%rax)
+000000029a1b92b8 <.idata$5>:
 	...
 
-000000029a1b92c0 <.idata$5>:
+000000029a1b92c0 <__imp__set_new_mode>:
+   29a1b92c0:	scas   %es:(%rdi),%al
+   29a1b92c1:	xchg   %eax,%esp
+   29a1b92c2:	add    %al,(%rax)
+   29a1b92c4:	add    %al,(%rax)
 	...
 
-000000029a1b92c8 <__imp__set_new_mode>:
+000000029a1b92c8 <__imp_calloc>:
    29a1b92c8:	mov    $0x94,%esi
    29a1b92cd:	add    %al,(%rax)
 	...
 
-000000029a1b92d0 <__imp_calloc>:
-   29a1b92d0:	(bad)
-   29a1b92d1:	xchg   %eax,%esp
-   29a1b92d2:	add    %al,(%rax)
+000000029a1b92d0 <__imp_free>:
+   29a1b92d0:	enter  $0x94,$0x0
    29a1b92d4:	add    %al,(%rax)
 	...
 
-000000029a1b92d8 <__imp_free>:
-   29a1b92d8:	fcoms  0x0(%rax,%rax,1)
+000000029a1b92d8 <.idata$5>:
 	...
 
-000000029a1b92e0 <.idata$5>:
+000000029a1b92e0 <__imp___p___argc>:
+   29a1b92e0:	rclb   $1,0x0(%rax,%rax,1)
 	...
 
-000000029a1b92e8 <__imp___p___argc>:
-   29a1b92e8:	loopne 29a1b927e <__imp_Sleep+0x6>
-   29a1b92ea:	add    %al,(%rax)
-   29a1b92ec:	add    %al,(%rax)
+000000029a1b92e8 <__imp___p___argv>:
+   29a1b92e8:	ficoms 0x0(%rax,%rax,1)
 	...
 
-000000029a1b92f0 <__imp___p___argv>:
-   29a1b92f0:	out    %al,(%dx)
+000000029a1b92f0 <__imp___p___wargv>:
+   29a1b92f0:	in     (%dx),%al
    29a1b92f1:	xchg   %eax,%esp
    29a1b92f2:	add    %al,(%rax)
    29a1b92f4:	add    %al,(%rax)
 	...
 
-000000029a1b92f8 <__imp___p___wargv>:
-   29a1b92f8:	cld
+000000029a1b92f8 <__imp__configure_narrow_argv>:
+   29a1b92f8:	cli
    29a1b92f9:	xchg   %eax,%esp
    29a1b92fa:	add    %al,(%rax)
    29a1b92fc:	add    %al,(%rax)
 	...
 
-000000029a1b9300 <__imp__configure_narrow_argv>:
-   29a1b9300:	or     0x0(%rbp),%dl
+000000029a1b9300 <__imp__configure_wide_argv>:
+   29a1b9300:	adc    $0x95,%al
+   29a1b9302:	add    %al,(%rax)
+   29a1b9304:	add    %al,(%rax)
 	...
 
-000000029a1b9308 <__imp__configure_wide_argv>:
-   29a1b9308:	and    $0x95,%al
+000000029a1b9308 <__imp__crt_at_quick_exit>:
+   29a1b9308:	sub    $0x95,%al
    29a1b930a:	add    %al,(%rax)
    29a1b930c:	add    %al,(%rax)
 	...
 
-000000029a1b9310 <__imp__crt_at_quick_exit>:
-   29a1b9310:	cmp    $0x95,%al
+000000029a1b9310 <__imp__crt_atexit>:
+   29a1b9310:	rex.X xchg %eax,%ebp
    29a1b9312:	add    %al,(%rax)
    29a1b9314:	add    %al,(%rax)
 	...
 
-000000029a1b9318 <__imp__crt_atexit>:
-   29a1b9318:	push   %rdx
+000000029a1b9318 <__imp__execute_onexit_table>:
+   29a1b9318:	push   %rax
    29a1b9319:	xchg   %eax,%ebp
    29a1b931a:	add    %al,(%rax)
    29a1b931c:	add    %al,(%rax)
 	...
 
-000000029a1b9320 <__imp__execute_onexit_table>:
-   29a1b9320:	(bad)
-   29a1b9321:	xchg   %eax,%ebp
-   29a1b9322:	add    %al,(%rax)
-   29a1b9324:	add    %al,(%rax)
+000000029a1b9320 <__imp__exit>:
+   29a1b9320:	push   $0x95
+   29a1b9325:	add    %al,(%rax)
 	...
 
-000000029a1b9328 <__imp__exit>:
-   29a1b9328:	js     29a1b92bf <__imp___p__wenviron+0x7>
+000000029a1b9328 <__imp__initialize_narrow_environment>:
+   29a1b9328:	jo     29a1b92bf <.idata$5+0x7>
    29a1b932a:	add    %al,(%rax)
    29a1b932c:	add    %al,(%rax)
 	...
 
-000000029a1b9330 <__imp__initialize_narrow_environment>:
-   29a1b9330:	adcb   $0x0,0x0(%rbp)
+000000029a1b9330 <__imp__initialize_onexit_table>:
+   29a1b9330:	xchg   %eax,%edx
+   29a1b9331:	xchg   %eax,%ebp
+   29a1b9332:	add    %al,(%rax)
+   29a1b9334:	add    %al,(%rax)
 	...
 
-000000029a1b9338 <__imp__initialize_onexit_table>:
-   29a1b9338:	movabs %al,0xbe00000000000095
+000000029a1b9338 <__imp__initialize_wide_environment>:
+   29a1b9338:	scas   %es:(%rdi),%al
+   29a1b9339:	xchg   %eax,%ebp
+   29a1b933a:	add    %al,(%rax)
+   29a1b933c:	add    %al,(%rax)
+	...
 
-000000029a1b9340 <__imp__initialize_wide_environment>:
-   29a1b9340:	mov    $0x95,%esi
-   29a1b9345:	add    %al,(%rax)
+000000029a1b9340 <__imp__initterm>:
+   29a1b9340:	(bad)
+   29a1b9341:	xchg   %eax,%ebp
+   29a1b9342:	add    %al,(%rax)
+   29a1b9344:	add    %al,(%rax)
 	...
 
-000000029a1b9348 <__imp__initterm>:
-   29a1b9348:	ficoms 0x0(%rbp)
+000000029a1b9348 <__imp__register_onexit_function>:
+   29a1b9348:	ficoml 0x0(%rbp)
 	...
 
-000000029a1b9350 <__imp__register_onexit_function>:
-   29a1b9350:	(bad)
-   29a1b9351:	xchg   %eax,%ebp
-   29a1b9352:	add    %al,(%rax)
-   29a1b9354:	add    %al,(%rax)
+000000029a1b9350 <__imp_abort>:
+   29a1b9350:	notb   0x0(%rbp)
 	...
 
-000000029a1b9358 <__imp_abort>:
-   29a1b9358:	(bad)
-   29a1b9359:	xchg   %eax,%esi
-   29a1b935a:	add    %al,(%rax)
-   29a1b935c:	add    %al,(%rax)
+000000029a1b9358 <.idata$5>:
 	...
 
-000000029a1b9360 <.idata$5>:
+000000029a1b9360 <__imp___acrt_iob_func>:
+   29a1b9360:	(bad)
+   29a1b9361:	xchg   %eax,%ebp
+   29a1b9362:	add    %al,(%rax)
+   29a1b9364:	add    %al,(%rax)
 	...
 
-000000029a1b9368 <__imp___acrt_iob_func>:
-   29a1b9368:	(bad)
-   29a1b9369:	xchg   %eax,%esi
-   29a1b936a:	add    %al,(%rax)
-   29a1b936c:	add    %al,(%rax)
+000000029a1b9368 <__imp___stdio_common_vfprintf>:
+   29a1b9368:	adc    %dl,0x0(%rsi)
 	...
 
-000000029a1b9370 <__imp___stdio_common_vfprintf>:
-   29a1b9370:	and    %dl,0x0(%rsi)
+000000029a1b9370 <__imp___stdio_common_vfwprintf>:
+   29a1b9370:	sub    0x0(%rsi),%dl
 	...
 
-000000029a1b9378 <__imp___stdio_common_vfwprintf>:
-   29a1b9378:	cmp    0x0(%rsi),%dl
+000000029a1b9378 <__imp_kbhit>:
+   29a1b9378:	rex.RX xchg %eax,%esi
+   29a1b937a:	add    %al,(%rax)
+   29a1b937c:	add    %al,(%rax)
 	...
 
-000000029a1b9380 <__imp_kbhit>:
-   29a1b9380:	push   %rsi
+000000029a1b9380 <__imp_fwrite>:
+   29a1b9380:	push   %rax
    29a1b9381:	xchg   %eax,%esi
    29a1b9382:	add    %al,(%rax)
    29a1b9384:	add    %al,(%rax)
 	...
 
-000000029a1b9388 <__imp_fflush>:
-   29a1b9388:	(bad)
+000000029a1b9388 <__imp_putchar>:
+   29a1b9388:	pop    %rdx
    29a1b9389:	xchg   %eax,%esi
    29a1b938a:	add    %al,(%rax)
    29a1b938c:	add    %al,(%rax)
 	...
 
-000000029a1b9390 <__imp_fwrite>:
-   29a1b9390:	push   $0xffffffffffffff96
-   29a1b9392:	add    %al,(%rax)
-   29a1b9394:	add    %al,(%rax)
+000000029a1b9390 <.idata$5>:
 	...
 
-000000029a1b9398 <__imp_putchar>:
-   29a1b9398:	je     29a1b9330 <__imp__initialize_narrow_environment>
+000000029a1b9398 <__imp_strlen>:
+   29a1b9398:	fs xchg %eax,%esi
    29a1b939a:	add    %al,(%rax)
    29a1b939c:	add    %al,(%rax)
 	...
 
-000000029a1b93a0 <.idata$5>:
+000000029a1b93a0 <__imp_strncmp>:
+   29a1b93a0:	outsb  %ds:(%rsi),(%dx)
+   29a1b93a1:	xchg   %eax,%esi
+   29a1b93a2:	add    %al,(%rax)
+   29a1b93a4:	add    %al,(%rax)
 	...
 
-000000029a1b93a8 <__imp_strlen>:
-   29a1b93a8:	jle    29a1b9340 <__imp__initialize_wide_environment>
-   29a1b93aa:	add    %al,(%rax)
-   29a1b93ac:	add    %al,(%rax)
+000000029a1b93a8 <.idata$5>:
 	...
 
-000000029a1b93b0 <__imp_strncmp>:
-   29a1b93b0:	mov    %dl,0x0(%rsi)
+000000029a1b93b0 <__imp___daylight>:
+   29a1b93b0:	js     29a1b9348 <__imp__register_onexit_function>
+   29a1b93b2:	add    %al,(%rax)
+   29a1b93b4:	add    %al,(%rax)
 	...
 
-000000029a1b93b8 <.idata$5>:
+000000029a1b93b8 <__imp___timezone>:
+   29a1b93b8:	xchg   %dl,0x0(%rsi)
 	...
 
-000000029a1b93c0 <__imp___daylight>:
-   29a1b93c0:	xchg   %eax,%edx
+000000029a1b93c0 <__imp___tzname>:
+   29a1b93c0:	xchg   %eax,%esp
    29a1b93c1:	xchg   %eax,%esi
    29a1b93c2:	add    %al,(%rax)
    29a1b93c4:	add    %al,(%rax)
 	...
 
-000000029a1b93c8 <__imp___timezone>:
-   29a1b93c8:	movabs 0xae00000000000096,%al
+000000029a1b93c8 <__imp__tzset>:
+   29a1b93c8:	movabs 0x96,%al
+
+000000029a1b93d0 <.idata$5>:
+	...
 
-000000029a1b93d0 <__imp___tzname>:
-   29a1b93d0:	scas   %es:(%rdi),%al
-   29a1b93d1:	xchg   %eax,%esi
-   29a1b93d2:	add    %al,(%rax)
-   29a1b93d4:	add    %al,(%rax)
-	...
-
-000000029a1b93d8 <__imp__tzset>:
-   29a1b93d8:	mov    $0x96,%edx
-   29a1b93dd:	add    %al,(%rax)
-	...
-
-000000029a1b93e0 <.idata$5>:
-	...
-
-000000029a1b93e8 <__IAT_end__>:
-   29a1b93e8:	and    $0x6c654401,%eax
-   29a1b93ed:	gs je  29a1b9455 <.idata$6+0x11>
-   29a1b93f0:	rex.XB jb 29a1b945c <.idata$6>
-   29a1b93f3:	je     29a1b945e <.idata$6+0x2>
-   29a1b93f5:	movsxd 0x6c(%rcx),%esp
-   29a1b93f8:	push   %rbx
-   29a1b93f9:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   29a1b93fe:	outsb  %ds:(%rsi),(%dx)
-	...
-
-000000029a1b9400 <.idata$6>:
-   29a1b9400:	rex.WXB add %rax,0x6e(%r13)
-   29a1b9404:	je     29a1b946b <.idata$6+0x7>
-   29a1b9406:	jb     29a1b944b <.idata$6+0x7>
-   29a1b9408:	jb     29a1b9473 <.idata$6+0x1>
-   29a1b940a:	je     29a1b9475 <.idata$6+0x3>
-   29a1b940c:	movsxd 0x6c(%rcx),%esp
-   29a1b940f:	push   %rbx
-   29a1b9410:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   29a1b9415:	outsb  %ds:(%rsi),(%dx)
+000000029a1b93d8 <__IAT_end__>:
+   29a1b93d8:	and    $0x6c654401,%eax
+   29a1b93dd:	gs je  29a1b9445 <.idata$6+0x11>
+   29a1b93e0:	rex.XB jb 29a1b944c <.idata$6>
+   29a1b93e3:	je     29a1b944e <.idata$6+0x2>
+   29a1b93e5:	movsxd 0x6c(%rcx),%esp
+   29a1b93e8:	push   %rbx
+   29a1b93e9:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   29a1b93ee:	outsb  %ds:(%rsi),(%dx)
+	...
+
+000000029a1b93f0 <.idata$6>:
+   29a1b93f0:	rex.WXB add %rax,0x6e(%r13)
+   29a1b93f4:	je     29a1b945b <.idata$6+0x7>
+   29a1b93f6:	jb     29a1b943b <.idata$6+0x7>
+   29a1b93f8:	jb     29a1b9463 <.idata$6+0x1>
+   29a1b93fa:	je     29a1b9465 <.idata$6+0x3>
+   29a1b93fc:	movsxd 0x6c(%rcx),%esp
+   29a1b93ff:	push   %rbx
+   29a1b9400:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   29a1b9405:	outsb  %ds:(%rsi),(%dx)
+	...
+
+000000029a1b9408 <.idata$6>:
+   29a1b9408:	test   %al,(%rdx)
+   29a1b940a:	rex.RXB
+   29a1b940b:	gs je  29a1b945a <.idata$6+0x6>
+   29a1b940e:	(bad)
+   29a1b940f:	jae    29a1b9485 <.idata$6+0x1>
+   29a1b9411:	rex.RB jb 29a1b9486 <.idata$6+0x2>
+   29a1b9414:	outsl  %ds:(%rsi),(%dx)
+   29a1b9415:	jb     29a1b9417 <.idata$6+0xf>
 	...
 
 000000029a1b9418 <.idata$6>:
-   29a1b9418:	test   %al,(%rdx)
-   29a1b941a:	rex.RXB
-   29a1b941b:	gs je  29a1b946a <.idata$6+0x6>
-   29a1b941e:	(bad)
-   29a1b941f:	jae    29a1b9495 <.idata$6+0x1>
-   29a1b9421:	rex.RB jb 29a1b9496 <.idata$6+0x2>
-   29a1b9424:	outsl  %ds:(%rsi),(%dx)
-   29a1b9425:	jb     29a1b9427 <.idata$6+0xf>
-	...
-
-000000029a1b9428 <.idata$6>:
-   29a1b9428:	xchg   %eax,%edx
-   29a1b9429:	add    0x6e(%rcx),%ecx
-   29a1b942c:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
-   29a1b9434:	rex.XB jb 29a1b94a0 <.idata$6+0x2>
-   29a1b9437:	je     29a1b94a2 <.idata$6+0x4>
-   29a1b9439:	movsxd 0x6c(%rcx),%esp
-   29a1b943c:	push   %rbx
-   29a1b943d:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   29a1b9442:	outsb  %ds:(%rsi),(%dx)
-	...
-
-000000029a1b9444 <.idata$6>:
-   29a1b9444:	lock add 0x61(%rbp,%riz,2),%ecx
-   29a1b9449:	jbe    29a1b94b0 <.idata$6+0x2>
-   29a1b944b:	rex.XB jb 29a1b94b7 <.idata$6+0x9>
-   29a1b944e:	je     29a1b94b9 <.idata$6+0xb>
-   29a1b9450:	movsxd 0x6c(%rcx),%esp
-   29a1b9453:	push   %rbx
-   29a1b9454:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
-   29a1b9459:	outsb  %ds:(%rsi),(%dx)
-	...
-
-000000029a1b945c <.idata$6>:
-   29a1b945c:	movsb  %ds:(%rsi),%es:(%rdi)
-   29a1b945d:	add    $0x65656c53,%eax
-   29a1b9462:	jo     29a1b9464 <.idata$6>
-
-000000029a1b9464 <.idata$6>:
-   29a1b9464:	enter  $0x5405,$0x6c
-   29a1b9468:	jae    29a1b94b1 <.idata$6+0x3>
-   29a1b946a:	gs je  29a1b94c3 <.idata$6+0x5>
-   29a1b946d:	(bad)
-   29a1b946e:	insb   (%dx),%es:(%rdi)
-   29a1b946f:	jne    29a1b94d6 <.idata$6+0x8>
-	...
-
-000000029a1b9472 <.idata$6>:
-   29a1b9472:	testl  $0x506c6175,0x74726956(%rip)        # 30e8dfdd2 <.debug_rnglists+0x7470fd2e>
-   29a1b947c:	jb     29a1b94ed <.idata$6+0xd>
-   29a1b947e:	je     29a1b94e5 <.idata$6+0x5>
-   29a1b9480:	movsxd 0x0(%rax,%rax,1),%esi
+   29a1b9418:	xchg   %eax,%edx
+   29a1b9419:	add    0x6e(%rcx),%ecx
+   29a1b941c:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   29a1b9424:	rex.XB jb 29a1b9490 <.idata$6+0x2>
+   29a1b9427:	je     29a1b9492 <.idata$6+0x4>
+   29a1b9429:	movsxd 0x6c(%rcx),%esp
+   29a1b942c:	push   %rbx
+   29a1b942d:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   29a1b9432:	outsb  %ds:(%rsi),(%dx)
+	...
+
+000000029a1b9434 <.idata$6>:
+   29a1b9434:	lock add 0x61(%rbp,%riz,2),%ecx
+   29a1b9439:	jbe    29a1b94a0 <.idata$6+0x2>
+   29a1b943b:	rex.XB jb 29a1b94a7 <.idata$6+0x9>
+   29a1b943e:	je     29a1b94a9 <.idata$6+0xb>
+   29a1b9440:	movsxd 0x6c(%rcx),%esp
+   29a1b9443:	push   %rbx
+   29a1b9444:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
+   29a1b9449:	outsb  %ds:(%rsi),(%dx)
+	...
+
+000000029a1b944c <.idata$6>:
+   29a1b944c:	movsb  %ds:(%rsi),%es:(%rdi)
+   29a1b944d:	add    $0x65656c53,%eax
+   29a1b9452:	jo     29a1b9454 <.idata$6>
+
+000000029a1b9454 <.idata$6>:
+   29a1b9454:	enter  $0x5405,$0x6c
+   29a1b9458:	jae    29a1b94a1 <.idata$6+0x3>
+   29a1b945a:	gs je  29a1b94b3 <.idata$6+0x5>
+   29a1b945d:	(bad)
+   29a1b945e:	insb   (%dx),%es:(%rdi)
+   29a1b945f:	jne    29a1b94c6 <.idata$6+0x8>
+	...
+
+000000029a1b9462 <.idata$6>:
+   29a1b9462:	testl  $0x506c6175,0x74726956(%rip)        # 30e8dfdc2 <.debug_rnglists+0x7470fd1e>
+   29a1b946c:	jb     29a1b94dd <.idata$6+0xd>
+   29a1b946e:	je     29a1b94d5 <.idata$6+0x5>
+   29a1b9470:	movsxd 0x0(%rax,%rax,1),%esi
+
+000000029a1b9474 <.idata$6>:
+   29a1b9474:	stc
+   29a1b9475:	add    $0x74726956,%eax
+   29a1b947a:	jne    29a1b94dd <.idata$6+0xd>
+   29a1b947c:	insb   (%dx),%es:(%rdi)
+   29a1b947d:	push   %rcx
+   29a1b947e:	jne    29a1b94e5 <.idata$6+0x7>
+   29a1b9480:	jb     29a1b94fb <.idata$6+0x1>
+	...
 
 000000029a1b9484 <.idata$6>:
-   29a1b9484:	stc
-   29a1b9485:	add    $0x74726956,%eax
-   29a1b948a:	jne    29a1b94ed <.idata$6+0xd>
-   29a1b948c:	insb   (%dx),%es:(%rdi)
-   29a1b948d:	push   %rcx
-   29a1b948e:	jne    29a1b94f5 <.idata$6+0x7>
-   29a1b9490:	jb     29a1b950b <.idata$6+0x1>
+   29a1b9484:	ltr    0x67(%rdi)
+   29a1b9488:	gs je  29a1b94ee <.idata$6+0x2>
+   29a1b948b:	push   $0x10000
+
+000000029a1b948e <.idata$6>:
+   29a1b948e:	add    %eax,(%rax)
+   29a1b9490:	pop    %rdi
+   29a1b9491:	pop    %rdi
+   29a1b9492:	jo     29a1b94f3 <.idata$6+0x7>
+   29a1b9494:	pop    %rdi
+   29a1b9495:	outsb  %gs:(%rsi),(%dx)
+   29a1b9497:	jbe    29a1b9502 <.idata$6+0x8>
+   29a1b9499:	jb     29a1b950a <.idata$6+0x10>
+   29a1b949b:	outsb  %ds:(%rsi),(%dx)
 	...
 
-000000029a1b9494 <.idata$6>:
-   29a1b9494:	ltr    0x67(%rdi)
-   29a1b9498:	gs je  29a1b94fe <.idata$6+0x2>
-   29a1b949b:	push   $0x10000
-
 000000029a1b949e <.idata$6>:
-   29a1b949e:	add    %eax,(%rax)
+   29a1b949e:	add    (%rax),%al
    29a1b94a0:	pop    %rdi
    29a1b94a1:	pop    %rdi
-   29a1b94a2:	jo     29a1b9503 <.idata$6+0x7>
+   29a1b94a2:	jo     29a1b9503 <.idata$6+0x9>
    29a1b94a4:	pop    %rdi
-   29a1b94a5:	outsb  %gs:(%rsi),(%dx)
-   29a1b94a7:	jbe    29a1b9512 <.idata$6+0x8>
-   29a1b94a9:	jb     29a1b951a <.idata$6+0x10>
-   29a1b94ab:	outsb  %ds:(%rsi),(%dx)
+   29a1b94a5:	ja     29a1b950c <.idata$6+0x12>
+   29a1b94a7:	outsb  %ds:(%rsi),(%dx)
+   29a1b94a8:	jbe    29a1b9513 <.idata$6+0x19>
+   29a1b94aa:	jb     29a1b951b <.idata$6+0x7>
+   29a1b94ac:	outsb  %ds:(%rsi),(%dx)
 	...
 
 000000029a1b94ae <.idata$6>:
-   29a1b94ae:	add    (%rax),%al
+   29a1b94ae:	sbb    %al,(%rax)
    29a1b94b0:	pop    %rdi
-   29a1b94b1:	pop    %rdi
-   29a1b94b2:	jo     29a1b9513 <.idata$6+0x9>
-   29a1b94b4:	pop    %rdi
-   29a1b94b5:	ja     29a1b951c <.idata$6+0x12>
-   29a1b94b7:	outsb  %ds:(%rsi),(%dx)
-   29a1b94b8:	jbe    29a1b9523 <.idata$6+0x19>
-   29a1b94ba:	jb     29a1b952b <.idata$6+0x7>
-   29a1b94bc:	outsb  %ds:(%rsi),(%dx)
-	...
+   29a1b94b1:	jae    29a1b9518 <.idata$6+0x4>
+   29a1b94b3:	je     29a1b9514 <.idata$6>
+   29a1b94b5:	outsb  %ds:(%rsi),(%dx)
+   29a1b94b6:	gs ja  29a1b9518 <.idata$6+0x4>
+   29a1b94b9:	insl   (%dx),%es:(%rdi)
+   29a1b94ba:	outsl  %ds:(%rsi),(%dx)
+   29a1b94bb:	fs add %bl,%gs:(%rcx)
 
 000000029a1b94be <.idata$6>:
-   29a1b94be:	sbb    %al,(%rax)
-   29a1b94c0:	pop    %rdi
-   29a1b94c1:	jae    29a1b9528 <.idata$6+0x4>
-   29a1b94c3:	je     29a1b9524 <.idata$6>
-   29a1b94c5:	outsb  %ds:(%rsi),(%dx)
-   29a1b94c6:	gs ja  29a1b9528 <.idata$6+0x4>
-   29a1b94c9:	insl   (%dx),%es:(%rdi)
-   29a1b94ca:	outsl  %ds:(%rsi),(%dx)
-   29a1b94cb:	fs add %bl,%gs:(%rcx)
-
-000000029a1b94ce <.idata$6>:
-   29a1b94ce:	sbb    %eax,(%rax)
-   29a1b94d0:	movsxd 0x6c(%rcx),%esp
-   29a1b94d3:	insb   (%dx),%es:(%rdi)
-   29a1b94d4:	outsl  %ds:(%rsi),(%dx)
-   29a1b94d5:	movsxd (%rax),%eax
-	...
-
-000000029a1b94d8 <.idata$6>:
-   29a1b94d8:	sbb    (%rax),%al
-   29a1b94da:	data16 jb 29a1b9542 <.idata$6+0x6>
-   29a1b94dd:	add    %al,%gs:(%rax)
-
-000000029a1b94e0 <.idata$6>:
-   29a1b94e0:	add    $0x705f5f00,%eax
+   29a1b94be:	sbb    %eax,(%rax)
+   29a1b94c0:	movsxd 0x6c(%rcx),%esp
+   29a1b94c3:	insb   (%dx),%es:(%rdi)
+   29a1b94c4:	outsl  %ds:(%rsi),(%dx)
+   29a1b94c5:	movsxd (%rax),%eax
+	...
+
+000000029a1b94c8 <.idata$6>:
+   29a1b94c8:	sbb    (%rax),%al
+   29a1b94ca:	data16 jb 29a1b9532 <.idata$6+0x6>
+   29a1b94cd:	add    %al,%gs:(%rax)
+
+000000029a1b94d0 <.idata$6>:
+   29a1b94d0:	add    $0x705f5f00,%eax
+   29a1b94d5:	pop    %rdi
+   29a1b94d6:	pop    %rdi
+   29a1b94d7:	pop    %rdi
+   29a1b94d8:	(bad)
+   29a1b94d9:	jb     29a1b9542 <.idata$6>
+   29a1b94db:	movsxd (%rax),%eax
+	...
+
+000000029a1b94de <.idata$6>:
+   29a1b94de:	(bad)
+   29a1b94df:	add    %bl,0x5f(%rdi)
+   29a1b94e2:	jo     29a1b9543 <.idata$6+0x1>
+   29a1b94e4:	pop    %rdi
    29a1b94e5:	pop    %rdi
-   29a1b94e6:	pop    %rdi
-   29a1b94e7:	pop    %rdi
-   29a1b94e8:	(bad)
-   29a1b94e9:	jb     29a1b9552 <.idata$6>
-   29a1b94eb:	movsxd (%rax),%eax
-	...
-
-000000029a1b94ee <.idata$6>:
-   29a1b94ee:	(bad)
-   29a1b94ef:	add    %bl,0x5f(%rdi)
-   29a1b94f2:	jo     29a1b9553 <.idata$6+0x1>
-   29a1b94f4:	pop    %rdi
-   29a1b94f5:	pop    %rdi
-   29a1b94f6:	(bad)
-   29a1b94f7:	jb     29a1b9560 <.idata$6>
-   29a1b94f9:	jbe    29a1b94fb <.idata$6+0xd>
-	...
-
-000000029a1b94fc <.idata$6>:
-   29a1b94fc:	(bad)
-   29a1b94fd:	add    %bl,0x5f(%rdi)
-   29a1b9500:	jo     29a1b9561 <.idata$6+0x1>
-   29a1b9502:	pop    %rdi
-   29a1b9503:	pop    %rdi
-   29a1b9504:	ja     29a1b9567 <.idata$6+0x7>
-   29a1b9506:	jb     29a1b956f <.idata$6+0xf>
-   29a1b9508:	jbe    29a1b950a <.idata$6>
-
-000000029a1b950a <.idata$6>:
-   29a1b950a:	sbb    %eax,(%rax)
-   29a1b950c:	pop    %rdi
-   29a1b950d:	movsxd 0x6e(%rdi),%ebp
-   29a1b9510:	imul   $0x6572,0x75(%rdi),%sp
+   29a1b94e6:	(bad)
+   29a1b94e7:	jb     29a1b9550 <.idata$6>
+   29a1b94e9:	jbe    29a1b94eb <.idata$6+0xd>
+	...
+
+000000029a1b94ec <.idata$6>:
+   29a1b94ec:	(bad)
+   29a1b94ed:	add    %bl,0x5f(%rdi)
+   29a1b94f0:	jo     29a1b9551 <.idata$6+0x1>
+   29a1b94f2:	pop    %rdi
+   29a1b94f3:	pop    %rdi
+   29a1b94f4:	ja     29a1b9557 <.idata$6+0x7>
+   29a1b94f6:	jb     29a1b955f <.idata$6+0xf>
+   29a1b94f8:	jbe    29a1b94fa <.idata$6>
+
+000000029a1b94fa <.idata$6>:
+   29a1b94fa:	sbb    %eax,(%rax)
+   29a1b94fc:	pop    %rdi
+   29a1b94fd:	movsxd 0x6e(%rdi),%ebp
+   29a1b9500:	imul   $0x6572,0x75(%rdi),%sp
+   29a1b9506:	pop    %rdi
+   29a1b9507:	outsb  %ds:(%rsi),(%dx)
+   29a1b9508:	(bad)
+   29a1b9509:	jb     29a1b957d <.idata$6+0xd>
+   29a1b950b:	outsl  %ds:(%rsi),(%dx)
+   29a1b950c:	ja     29a1b956d <.idata$6+0x5>
+   29a1b950e:	(bad)
+   29a1b950f:	jb     29a1b9578 <.idata$6+0x8>
+   29a1b9511:	jbe    29a1b9513 <.idata$6+0x19>
+	...
+
+000000029a1b9514 <.idata$6>:
+   29a1b9514:	sbb    (%rax),%al
    29a1b9516:	pop    %rdi
-   29a1b9517:	outsb  %ds:(%rsi),(%dx)
-   29a1b9518:	(bad)
-   29a1b9519:	jb     29a1b958d <.idata$6+0xd>
-   29a1b951b:	outsl  %ds:(%rsi),(%dx)
-   29a1b951c:	ja     29a1b957d <.idata$6+0x5>
-   29a1b951e:	(bad)
-   29a1b951f:	jb     29a1b9588 <.idata$6+0x8>
-   29a1b9521:	jbe    29a1b9523 <.idata$6+0x19>
-	...
-
-000000029a1b9524 <.idata$6>:
-   29a1b9524:	sbb    (%rax),%al
-   29a1b9526:	pop    %rdi
-   29a1b9527:	movsxd 0x6e(%rdi),%ebp
-   29a1b952a:	imul   $0x6572,0x75(%rdi),%sp
-   29a1b9530:	pop    %rdi
-   29a1b9531:	ja     29a1b959c <.idata$6+0x1c>
-   29a1b9533:	fs gs pop %rdi
-   29a1b9536:	(bad)
-   29a1b9537:	jb     29a1b95a0 <.idata$6+0x20>
-   29a1b9539:	jbe    29a1b953b <.idata$6+0x17>
-	...
-
-000000029a1b953c <.idata$6>:
-   29a1b953c:	(bad)
-   29a1b953d:	add    %bl,0x63(%rdi)
-   29a1b9540:	jb     29a1b95b6 <.idata$6+0x14>
-   29a1b9542:	pop    %rdi
-   29a1b9543:	(bad)
-   29a1b9544:	je     29a1b95a5 <.idata$6+0x3>
-   29a1b9546:	jno    29a1b95bd <.idata$6+0x1b>
-   29a1b9548:	imul   $0x6978655f,0x6b(%rbx),%esp
-   29a1b954f:	je     29a1b9551 <.idata$6+0x15>
-	...
-
-000000029a1b9552 <.idata$6>:
-   29a1b9552:	(bad)
-   29a1b9553:	add    %bl,0x63(%rdi)
-   29a1b9556:	jb     29a1b95cc <.idata$6+0xe>
-   29a1b9558:	pop    %rdi
-   29a1b9559:	(bad)
-   29a1b955a:	je     29a1b95c1 <.idata$6+0x3>
-   29a1b955c:	js     29a1b95c7 <.idata$6+0x9>
-   29a1b955e:	je     29a1b9560 <.idata$6>
-
-000000029a1b9560 <.idata$6>:
-   29a1b9560:	and    $0x0,%al
-   29a1b9562:	pop    %rdi
-   29a1b9563:	gs js  29a1b95cb <.idata$6+0xd>
-   29a1b9566:	movsxd 0x74(%rbp),%esi
-   29a1b9569:	gs pop %rdi
-   29a1b956b:	outsl  %ds:(%rsi),(%dx)
-   29a1b956c:	outsb  %ds:(%rsi),(%dx)
-   29a1b956d:	gs js  29a1b95d9 <.idata$6+0x1b>
-   29a1b9570:	je     29a1b95d1 <.idata$6+0x13>
-   29a1b9572:	je     29a1b95d5 <.idata$6+0x17>
-   29a1b9574:	(bad)
-	...
-
-000000029a1b9578 <.idata$6>:
-   29a1b9578:	and    $0x78655f00,%eax
-   29a1b957d:	imul   $0x6e695f00,0x36(%rax,%rax,1),%esi
-
-000000029a1b9580 <.idata$6>:
-   29a1b9580:	ss add %bl,0x69(%rdi)
-   29a1b9584:	outsb  %ds:(%rsi),(%dx)
-   29a1b9585:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
-   29a1b958d:	pop    %rdi
-   29a1b958e:	outsb  %ds:(%rsi),(%dx)
-   29a1b958f:	(bad)
-   29a1b9590:	jb     29a1b9604 <.idata$6+0x1a>
-   29a1b9592:	outsl  %ds:(%rsi),(%dx)
-   29a1b9593:	ja     29a1b95f4 <.idata$6+0xa>
-   29a1b9595:	outsb  %gs:(%rsi),(%dx)
-   29a1b9597:	jbe    29a1b9602 <.idata$6+0x18>
-   29a1b9599:	jb     29a1b960a <.idata$6+0x4>
-   29a1b959b:	outsb  %ds:(%rsi),(%dx)
-   29a1b959c:	insl   (%dx),%es:(%rdi)
-   29a1b959d:	outsb  %gs:(%rsi),(%dx)
-   29a1b959f:	je     29a1b95a1 <.idata$6+0x21>
-	...
-
-000000029a1b95a2 <.idata$6>:
-   29a1b95a2:	(bad)
-   29a1b95a3:	add    %bl,0x69(%rdi)
-   29a1b95a6:	outsb  %ds:(%rsi),(%dx)
-   29a1b95a7:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
-   29a1b95af:	pop    %rdi
-   29a1b95b0:	outsl  %ds:(%rsi),(%dx)
-   29a1b95b1:	outsb  %ds:(%rsi),(%dx)
-   29a1b95b2:	gs js  29a1b961e <.idata$6+0x10>
-   29a1b95b5:	je     29a1b9616 <.idata$6+0x8>
-   29a1b95b7:	je     29a1b961a <.idata$6+0xc>
-   29a1b95b9:	(bad)
-	...
-
-000000029a1b95be <.idata$6>:
-   29a1b95be:	cmp    %al,(%rax)
-   29a1b95c0:	pop    %rdi
-   29a1b95c1:	imul   $0x6c616974,0x69(%rsi),%ebp
-   29a1b95c8:	imul   $0x6469775f,0x65(%rdx),%edi
-   29a1b95cf:	gs pop %rdi
-   29a1b95d1:	outsb  %gs:(%rsi),(%dx)
-   29a1b95d3:	jbe    29a1b963e <.idata$6+0x4>
-   29a1b95d5:	jb     29a1b9646 <.idata$6+0xc>
-   29a1b95d7:	outsb  %ds:(%rsi),(%dx)
+   29a1b9517:	movsxd 0x6e(%rdi),%ebp
+   29a1b951a:	imul   $0x6572,0x75(%rdi),%sp
+   29a1b9520:	pop    %rdi
+   29a1b9521:	ja     29a1b958c <.idata$6+0x1c>
+   29a1b9523:	fs gs pop %rdi
+   29a1b9526:	(bad)
+   29a1b9527:	jb     29a1b9590 <.idata$6+0x20>
+   29a1b9529:	jbe    29a1b952b <.idata$6+0x17>
+	...
+
+000000029a1b952c <.idata$6>:
+   29a1b952c:	(bad)
+   29a1b952d:	add    %bl,0x63(%rdi)
+   29a1b9530:	jb     29a1b95a6 <.idata$6+0x14>
+   29a1b9532:	pop    %rdi
+   29a1b9533:	(bad)
+   29a1b9534:	je     29a1b9595 <.idata$6+0x3>
+   29a1b9536:	jno    29a1b95ad <.idata$6+0x1b>
+   29a1b9538:	imul   $0x6978655f,0x6b(%rbx),%esp
+   29a1b953f:	je     29a1b9541 <.idata$6+0x15>
+	...
+
+000000029a1b9542 <.idata$6>:
+   29a1b9542:	(bad)
+   29a1b9543:	add    %bl,0x63(%rdi)
+   29a1b9546:	jb     29a1b95bc <.idata$6+0xe>
+   29a1b9548:	pop    %rdi
+   29a1b9549:	(bad)
+   29a1b954a:	je     29a1b95b1 <.idata$6+0x3>
+   29a1b954c:	js     29a1b95b7 <.idata$6+0x9>
+   29a1b954e:	je     29a1b9550 <.idata$6>
+
+000000029a1b9550 <.idata$6>:
+   29a1b9550:	and    $0x0,%al
+   29a1b9552:	pop    %rdi
+   29a1b9553:	gs js  29a1b95bb <.idata$6+0xd>
+   29a1b9556:	movsxd 0x74(%rbp),%esi
+   29a1b9559:	gs pop %rdi
+   29a1b955b:	outsl  %ds:(%rsi),(%dx)
+   29a1b955c:	outsb  %ds:(%rsi),(%dx)
+   29a1b955d:	gs js  29a1b95c9 <.idata$6+0x1b>
+   29a1b9560:	je     29a1b95c1 <.idata$6+0x13>
+   29a1b9562:	je     29a1b95c5 <.idata$6+0x17>
+   29a1b9564:	(bad)
+	...
+
+000000029a1b9568 <.idata$6>:
+   29a1b9568:	and    $0x78655f00,%eax
+   29a1b956d:	imul   $0x6e695f00,0x36(%rax,%rax,1),%esi
+
+000000029a1b9570 <.idata$6>:
+   29a1b9570:	ss add %bl,0x69(%rdi)
+   29a1b9574:	outsb  %ds:(%rsi),(%dx)
+   29a1b9575:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   29a1b957d:	pop    %rdi
+   29a1b957e:	outsb  %ds:(%rsi),(%dx)
+   29a1b957f:	(bad)
+   29a1b9580:	jb     29a1b95f4 <.idata$6+0x1a>
+   29a1b9582:	outsl  %ds:(%rsi),(%dx)
+   29a1b9583:	ja     29a1b95e4 <.idata$6+0xa>
+   29a1b9585:	outsb  %gs:(%rsi),(%dx)
+   29a1b9587:	jbe    29a1b95f2 <.idata$6+0x18>
+   29a1b9589:	jb     29a1b95fa <.idata$6+0x4>
+   29a1b958b:	outsb  %ds:(%rsi),(%dx)
+   29a1b958c:	insl   (%dx),%es:(%rdi)
+   29a1b958d:	outsb  %gs:(%rsi),(%dx)
+   29a1b958f:	je     29a1b9591 <.idata$6+0x21>
+	...
+
+000000029a1b9592 <.idata$6>:
+   29a1b9592:	(bad)
+   29a1b9593:	add    %bl,0x69(%rdi)
+   29a1b9596:	outsb  %ds:(%rsi),(%dx)
+   29a1b9597:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   29a1b959f:	pop    %rdi
+   29a1b95a0:	outsl  %ds:(%rsi),(%dx)
+   29a1b95a1:	outsb  %ds:(%rsi),(%dx)
+   29a1b95a2:	gs js  29a1b960e <.idata$6+0x10>
+   29a1b95a5:	je     29a1b9606 <.idata$6+0x8>
+   29a1b95a7:	je     29a1b960a <.idata$6+0xc>
+   29a1b95a9:	(bad)
+	...
+
+000000029a1b95ae <.idata$6>:
+   29a1b95ae:	cmp    %al,(%rax)
+   29a1b95b0:	pop    %rdi
+   29a1b95b1:	imul   $0x6c616974,0x69(%rsi),%ebp
+   29a1b95b8:	imul   $0x6469775f,0x65(%rdx),%edi
+   29a1b95bf:	gs pop %rdi
+   29a1b95c1:	outsb  %gs:(%rsi),(%dx)
+   29a1b95c3:	jbe    29a1b962e <.idata$6+0x4>
+   29a1b95c5:	jb     29a1b9636 <.idata$6+0xc>
+   29a1b95c7:	outsb  %ds:(%rsi),(%dx)
+   29a1b95c8:	insl   (%dx),%es:(%rdi)
+   29a1b95c9:	outsb  %gs:(%rsi),(%dx)
+   29a1b95cb:	je     29a1b95cd <.idata$6+0x1f>
+	...
+
+000000029a1b95ce <.idata$6>:
+   29a1b95ce:	cmp    %eax,(%rax)
+   29a1b95d0:	pop    %rdi
+   29a1b95d1:	imul   $0x72657474,0x69(%rsi),%ebp
    29a1b95d8:	insl   (%dx),%es:(%rdi)
-   29a1b95d9:	outsb  %gs:(%rsi),(%dx)
-   29a1b95db:	je     29a1b95dd <.idata$6+0x1f>
 	...
 
-000000029a1b95de <.idata$6>:
-   29a1b95de:	cmp    %eax,(%rax)
-   29a1b95e0:	pop    %rdi
-   29a1b95e1:	imul   $0x72657474,0x69(%rsi),%ebp
-   29a1b95e8:	insl   (%dx),%es:(%rdi)
-	...
-
-000000029a1b95ea <.idata$6>:
-   29a1b95ea:	(bad)
-   29a1b95eb:	add    %bl,0x72(%rdi)
-   29a1b95ee:	imul   $0x6f5f7265,%gs:0x74(%ebx),%esi
-   29a1b95f7:	outsb  %ds:(%rsi),(%dx)
-   29a1b95f8:	gs js  29a1b9664 <.idata$6+0x4>
-   29a1b95fb:	je     29a1b965c <.idata$6+0x6>
-   29a1b95fd:	data16 jne 29a1b966e <.idata$6+0x4>
-   29a1b9600:	movsxd 0x6f(%rcx,%rbp,2),%esi
-   29a1b9604:	outsb  %ds:(%rsi),(%dx)
-	...
-
-000000029a1b9606 <.idata$6>:
-   29a1b9606:	pop    %rax
-   29a1b9607:	add    %ah,0x62(%rcx)
-   29a1b960a:	outsl  %ds:(%rsi),(%dx)
-   29a1b960b:	jb     29a1b9681 <.idata$6+0x3>
-	...
-
-000000029a1b960e <.idata$6>:
-   29a1b960e:	add    %eax,(%rax)
-   29a1b9610:	pop    %rdi
-   29a1b9611:	pop    %rdi
-   29a1b9612:	(bad)
-   29a1b9613:	movsxd 0x74(%rdx),%esi
-   29a1b9616:	pop    %rdi
-   29a1b9617:	imul   $0x6e75665f,0x62(%rdi),%ebp
-   29a1b961e:	movsxd (%rax),%eax
-
-000000029a1b9620 <.idata$6>:
-   29a1b9620:	add    $0x0,%al
-   29a1b9622:	pop    %rdi
-   29a1b9623:	pop    %rdi
-   29a1b9624:	jae    29a1b969a <.idata$6+0x8>
-   29a1b9626:	imul   $0x6d6d6f63,%fs:0x5f(%rdi),%ebp
-   29a1b962e:	outsl  %ds:(%rsi),(%dx)
-   29a1b962f:	outsb  %ds:(%rsi),(%dx)
-   29a1b9630:	pop    %rdi
-   29a1b9631:	jbe    29a1b9699 <.idata$6+0x7>
-   29a1b9633:	jo     29a1b96a7 <.idata$6+0x7>
-   29a1b9635:	imul   $0x80066,0x74(%rsi),%ebp
-
-000000029a1b963a <.idata$6>:
-   29a1b963a:	or     %al,(%rax)
-   29a1b963c:	pop    %rdi
-   29a1b963d:	pop    %rdi
-   29a1b963e:	jae    29a1b96b4 <.idata$6+0x6>
-   29a1b9640:	imul   $0x6d6d6f63,%fs:0x5f(%rdi),%ebp
-   29a1b9648:	outsl  %ds:(%rsi),(%dx)
-   29a1b9649:	outsb  %ds:(%rsi),(%dx)
-   29a1b964a:	pop    %rdi
-   29a1b964b:	jbe    29a1b96b3 <.idata$6+0x5>
-   29a1b964d:	ja     29a1b96bf <.idata$6+0x5>
-   29a1b964f:	jb     29a1b96ba <.idata$6>
-   29a1b9651:	outsb  %ds:(%rsi),(%dx)
-   29a1b9652:	je     29a1b96ba <.idata$6>
-	...
-
-000000029a1b9656 <.idata$6>:
-   29a1b9656:	push   %rsp
-   29a1b9657:	add    %bl,0x6b(%rdi)
-   29a1b965a:	(bad)
-   29a1b965b:	push   $0x7469
-
-000000029a1b9660 <.idata$6>:
-   29a1b9660:	xchg   %eax,%esi
-   29a1b9661:	add    %ah,0x66(%rsi)
-   29a1b9664:	insb   (%dx),%es:(%rdi)
-   29a1b9665:	jne    29a1b96da <.idata$7+0x2>
-   29a1b9667:	push   $0xa90000
-
-000000029a1b966a <.idata$6>:
-   29a1b966a:	test   $0x72776600,%eax
-   29a1b966f:	imul   $0x7000b100,0x0(%rbp,%riz,2),%esi
-
-000000029a1b9674 <.idata$6>:
-   29a1b9674:	mov    $0x0,%cl
-   29a1b9676:	jo     29a1b96ed <__lib64_libkernel32_a_iname+0x5>
-   29a1b9678:	je     29a1b96dd <.idata$7+0x1>
-   29a1b967a:	push   $0xffffffffa8007261
-
-000000029a1b967e <.idata$6>:
-   29a1b967e:	test   $0x0,%al
-   29a1b9680:	jae    29a1b96f6 <__lib64_libkernel32_a_iname+0xe>
-   29a1b9682:	jb     29a1b96f0 <__lib64_libkernel32_a_iname+0x8>
-   29a1b9684:	outsb  %gs:(%rsi),(%dx)
-	...
-
-000000029a1b9688 <.idata$6>:
-   29a1b9688:	stos   %eax,%es:(%rdi)
-   29a1b9689:	add    %dh,0x74(%rbx)
-   29a1b968c:	jb     29a1b96fc <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname>
-   29a1b968e:	movsxd 0x70(%rbp),%ebp
-	...
-
-000000029a1b9692 <.idata$6>:
-   29a1b9692:	or     %eax,(%rax)
-   29a1b9694:	pop    %rdi
-   29a1b9695:	pop    %rdi
-   29a1b9696:	fs (bad)
-   29a1b9698:	jns    29a1b9706 <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0xa>
-   29a1b969a:	imul   $0xb000074,0x68(%rdi),%esp
+000000029a1b95da <.idata$6>:
+   29a1b95da:	(bad)
+   29a1b95db:	add    %bl,0x72(%rdi)
+   29a1b95de:	imul   $0x6f5f7265,%gs:0x74(%ebx),%esi
+   29a1b95e7:	outsb  %ds:(%rsi),(%dx)
+   29a1b95e8:	gs js  29a1b9654 <.idata$6+0x4>
+   29a1b95eb:	je     29a1b964c <.idata$6+0x6>
+   29a1b95ed:	data16 jne 29a1b965e <.idata$6+0x4>
+   29a1b95f0:	movsxd 0x6f(%rcx,%rbp,2),%esi
+   29a1b95f4:	outsb  %ds:(%rsi),(%dx)
+	...
+
+000000029a1b95f6 <.idata$6>:
+   29a1b95f6:	pop    %rax
+   29a1b95f7:	add    %ah,0x62(%rcx)
+   29a1b95fa:	outsl  %ds:(%rsi),(%dx)
+   29a1b95fb:	jb     29a1b9671 <.idata$6+0x3>
+	...
+
+000000029a1b95fe <.idata$6>:
+   29a1b95fe:	add    %eax,(%rax)
+   29a1b9600:	pop    %rdi
+   29a1b9601:	pop    %rdi
+   29a1b9602:	(bad)
+   29a1b9603:	movsxd 0x74(%rdx),%esi
+   29a1b9606:	pop    %rdi
+   29a1b9607:	imul   $0x6e75665f,0x62(%rdi),%ebp
+   29a1b960e:	movsxd (%rax),%eax
+
+000000029a1b9610 <.idata$6>:
+   29a1b9610:	add    $0x0,%al
+   29a1b9612:	pop    %rdi
+   29a1b9613:	pop    %rdi
+   29a1b9614:	jae    29a1b968a <.idata$6+0x4>
+   29a1b9616:	imul   $0x6d6d6f63,%fs:0x5f(%rdi),%ebp
+   29a1b961e:	outsl  %ds:(%rsi),(%dx)
+   29a1b961f:	outsb  %ds:(%rsi),(%dx)
+   29a1b9620:	pop    %rdi
+   29a1b9621:	jbe    29a1b9689 <.idata$6+0x3>
+   29a1b9623:	jo     29a1b9697 <.idata$6+0x3>
+   29a1b9625:	imul   $0x80066,0x74(%rsi),%ebp
+
+000000029a1b962a <.idata$6>:
+   29a1b962a:	or     %al,(%rax)
+   29a1b962c:	pop    %rdi
+   29a1b962d:	pop    %rdi
+   29a1b962e:	jae    29a1b96a4 <.idata$6+0x4>
+   29a1b9630:	imul   $0x6d6d6f63,%fs:0x5f(%rdi),%ebp
+   29a1b9638:	outsl  %ds:(%rsi),(%dx)
+   29a1b9639:	outsb  %ds:(%rsi),(%dx)
+   29a1b963a:	pop    %rdi
+   29a1b963b:	jbe    29a1b96a3 <.idata$6+0x3>
+   29a1b963d:	ja     29a1b96af <.idata$7+0x3>
+   29a1b963f:	jb     29a1b96aa <.idata$6+0xa>
+   29a1b9641:	outsb  %ds:(%rsi),(%dx)
+   29a1b9642:	je     29a1b96aa <.idata$6+0xa>
+	...
+
+000000029a1b9646 <.idata$6>:
+   29a1b9646:	push   %rsp
+   29a1b9647:	add    %bl,0x6b(%rdi)
+   29a1b964a:	(bad)
+   29a1b964b:	push   $0x7469
+
+000000029a1b9650 <.idata$6>:
+   29a1b9650:	test   $0x72776600,%eax
+   29a1b9655:	imul   $0x7000b100,0x0(%rbp,%riz,2),%esi
+
+000000029a1b965a <.idata$6>:
+   29a1b965a:	mov    $0x0,%cl
+   29a1b965c:	jo     29a1b96d3 <__lib64_libkernel32_a_iname+0x3>
+   29a1b965e:	je     29a1b96c3 <.idata$7+0x3>
+   29a1b9660:	push   $0xffffffffa8007261
+
+000000029a1b9664 <.idata$6>:
+   29a1b9664:	test   $0x0,%al
+   29a1b9666:	jae    29a1b96dc <__lib64_libkernel32_a_iname+0xc>
+   29a1b9668:	jb     29a1b96d6 <__lib64_libkernel32_a_iname+0x6>
+   29a1b966a:	outsb  %gs:(%rsi),(%dx)
+	...
+
+000000029a1b966e <.idata$6>:
+   29a1b966e:	stos   %eax,%es:(%rdi)
+   29a1b966f:	add    %dh,0x74(%rbx)
+   29a1b9672:	jb     29a1b96e2 <.idata$7+0x2>
+   29a1b9674:	movsxd 0x70(%rbp),%ebp
+	...
+
+000000029a1b9678 <.idata$6>:
+   29a1b9678:	or     %eax,(%rax)
+   29a1b967a:	pop    %rdi
+   29a1b967b:	pop    %rdi
+   29a1b967c:	fs (bad)
+   29a1b967e:	jns    29a1b96ec <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0x8>
+   29a1b9680:	imul   $0xb000074,0x68(%rdi),%esp
+
+000000029a1b9686 <.idata$6>:
+   29a1b9686:	or     (%rax),%eax
+   29a1b9688:	pop    %rdi
+   29a1b9689:	pop    %rdi
+   29a1b968a:	je     29a1b96f5 <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0x11>
+   29a1b968c:	insl   (%dx),%es:(%rdi)
+   29a1b968d:	gs jp  29a1b96ff <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0x1b>
+   29a1b9690:	outsb  %ds:(%rsi),(%dx)
+   29a1b9691:	add    %al,%gs:(%rax)
+
+000000029a1b9694 <.idata$6>:
+   29a1b9694:	or     $0x0,%al
+   29a1b9696:	pop    %rdi
+   29a1b9697:	pop    %rdi
+   29a1b9698:	je     29a1b9714 <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname+0x8>
+   29a1b969a:	outsb  %ds:(%rsi),(%dx)
+   29a1b969b:	(bad)
+   29a1b969c:	insl   (%dx),%es:(%rdi)
+   29a1b969d:	add    %al,%gs:(%rax)
 
 000000029a1b96a0 <.idata$6>:
-   29a1b96a0:	or     (%rax),%eax
+   29a1b96a0:	cmp    $0x0,%al
    29a1b96a2:	pop    %rdi
-   29a1b96a3:	pop    %rdi
-   29a1b96a4:	je     29a1b970f <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0x13>
-   29a1b96a6:	insl   (%dx),%es:(%rdi)
-   29a1b96a7:	gs jp  29a1b9719 <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname+0x1d>
-   29a1b96aa:	outsb  %ds:(%rsi),(%dx)
-   29a1b96ab:	add    %al,%gs:(%rax)
-
-000000029a1b96ae <.idata$6>:
-   29a1b96ae:	or     $0x0,%al
-   29a1b96b0:	pop    %rdi
-   29a1b96b1:	pop    %rdi
-   29a1b96b2:	je     29a1b972e <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname+0xa>
-   29a1b96b4:	outsb  %ds:(%rsi),(%dx)
-   29a1b96b5:	(bad)
-   29a1b96b6:	insl   (%dx),%es:(%rdi)
-   29a1b96b7:	add    %al,%gs:(%rax)
-
-000000029a1b96ba <.idata$6>:
-   29a1b96ba:	cmp    $0x0,%al
-   29a1b96bc:	pop    %rdi
-   29a1b96bd:	je     29a1b9739 <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname+0x15>
-   29a1b96bf:	jae    29a1b9726 <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname+0x2>
-   29a1b96c1:	je     29a1b96c3 <.idata$6+0x9>
+   29a1b96a3:	je     29a1b971f <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname+0x13>
+   29a1b96a5:	jae    29a1b970c <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname>
+   29a1b96a7:	je     29a1b96a9 <.idata$6+0x9>
+   29a1b96a9:	add    %al,(%rax)
 	...
 
+000000029a1b96ac <.idata$7>:
+   29a1b96ac:	add    %dl,-0x70000000(%rax)
+
+000000029a1b96b0 <.idata$7>:
+   29a1b96b0:	add    %dl,-0x70000000(%rax)
+
+000000029a1b96b4 <.idata$7>:
+   29a1b96b4:	add    %dl,-0x70000000(%rax)
+
+000000029a1b96b8 <.idata$7>:
+   29a1b96b8:	add    %dl,-0x70000000(%rax)
+
+000000029a1b96bc <.idata$7>:
+   29a1b96bc:	add    %dl,-0x70000000(%rax)
+
+000000029a1b96c0 <.idata$7>:
+   29a1b96c0:	add    %dl,-0x70000000(%rax)
+
 000000029a1b96c4 <.idata$7>:
    29a1b96c4:	add    %dl,-0x70000000(%rax)
 
 000000029a1b96c8 <.idata$7>:
    29a1b96c8:	add    %dl,-0x70000000(%rax)
 
 000000029a1b96cc <.idata$7>:
-   29a1b96cc:	add    %dl,-0x70000000(%rax)
+   29a1b96cc:	add    %dl,0x454b0000(%rax)
+
+000000029a1b96d0 <__lib64_libkernel32_a_iname>:
+   29a1b96d0:	rex.WXB
+   29a1b96d1:	rex.RB push %r10
+   29a1b96d3:	rex.WRX
+   29a1b96d4:	rex.RB
+   29a1b96d5:	xor    (%rdx),%r14
+   29a1b96d8:	cs fs insb (%dx),%es:(%rdi)
+   29a1b96db:	insb   (%dx),%es:(%rdi)
+   29a1b96dc:	add    %al,(%rax)
+	...
 
-000000029a1b96d0 <.idata$7>:
-   29a1b96d0:	add    %dl,-0x70000000(%rax)
+000000029a1b96e0 <.idata$7>:
+   29a1b96e0:	adc    $0x90,%al
+	...
 
-000000029a1b96d4 <.idata$7>:
-   29a1b96d4:	add    %dl,-0x70000000(%rax)
+000000029a1b96e4 <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname>:
+   29a1b96e4:	(bad)
+   29a1b96e5:	jo     29a1b9750 <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname+0x10>
+   29a1b96e7:	sub    $0x772d736d,%eax
+   29a1b96ec:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b96f3:	movsxd 0x6e(%rdi),%ebp
+   29a1b96f6:	imul   $0x312d316c,0x2d(%rdi),%ebp
+   29a1b96fd:	sub    $0x6c642e30,%eax
+   29a1b9702:	insb   (%dx),%es:(%rdi)
+	...
 
-000000029a1b96d8 <.idata$7>:
-   29a1b96d8:	add    %dl,-0x70000000(%rax)
+000000029a1b9704 <.idata$7>:
+   29a1b9704:	sub    %dl,-0x6fd80000(%rax)
 
-000000029a1b96dc <.idata$7>:
-   29a1b96dc:	add    %dl,-0x70000000(%rax)
+000000029a1b9708 <.idata$7>:
+   29a1b9708:	sub    %dl,0x70610000(%rax)
 
-000000029a1b96e0 <.idata$7>:
-   29a1b96e0:	add    %dl,-0x70000000(%rax)
+000000029a1b970c <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname>:
+   29a1b970c:	(bad)
+   29a1b970d:	jo     29a1b9778 <.idata$7>
+   29a1b970f:	sub    $0x772d736d,%eax
+   29a1b9714:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b971b:	outsb  %gs:(%rsi),(%dx)
+   29a1b971d:	jbe    29a1b9788 <.idata$7>
+   29a1b971f:	jb     29a1b9790 <.idata$7>
+   29a1b9721:	outsb  %ds:(%rsi),(%dx)
+   29a1b9722:	insl   (%dx),%es:(%rdi)
+   29a1b9723:	outsb  %gs:(%rsi),(%dx)
+   29a1b9725:	je     29a1b9754 <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname+0x14>
+   29a1b9727:	insb   (%dx),%es:(%rdi)
+   29a1b9728:	xor    %ebp,0x2e302d31(%rip)        # 2c84bc45f <.debug_rnglists+0x2e2ec3bb>
+   29a1b972e:	fs insb (%dx),%es:(%rdi)
+   29a1b9730:	insb   (%dx),%es:(%rdi)
+   29a1b9731:	add    %al,(%rax)
+	...
+
+000000029a1b9734 <.idata$7>:
+   29a1b9734:	cmp    $0x90,%al
+	...
+
+000000029a1b9738 <.idata$7>:
+   29a1b9738:	cmp    $0x90,%al
+	...
+
+000000029a1b973c <.idata$7>:
+   29a1b973c:	cmp    $0x90,%al
+	...
+
+000000029a1b9740 <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname>:
+   29a1b9740:	(bad)
+   29a1b9741:	jo     29a1b97ac <__lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname+0x10>
+   29a1b9743:	sub    $0x772d736d,%eax
+   29a1b9748:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b974f:	push   $0x2d706165
+   29a1b9754:	insb   (%dx),%es:(%rdi)
+   29a1b9755:	xor    %ebp,0x2e302d31(%rip)        # 2c84bc48c <.debug_rnglists+0x2e2ec3e8>
+   29a1b975b:	fs insb (%dx),%es:(%rdi)
+   29a1b975d:	insb   (%dx),%es:(%rdi)
+	...
+
+000000029a1b9760 <.idata$7>:
+   29a1b9760:	push   %rax
+   29a1b9761:	nop
+	...
 
-000000029a1b96e4 <.idata$7>:
-   29a1b96e4:	add    %dl,0x454b0000(%rax)
+000000029a1b9764 <.idata$7>:
+   29a1b9764:	push   %rax
+   29a1b9765:	nop
+	...
 
-000000029a1b96e8 <__lib64_libkernel32_a_iname>:
-   29a1b96e8:	rex.WXB
-   29a1b96e9:	rex.RB push %r10
-   29a1b96eb:	rex.WRX
-   29a1b96ec:	rex.RB
-   29a1b96ed:	xor    (%rdx),%r14
-   29a1b96f0:	cs fs insb (%dx),%es:(%rdi)
-   29a1b96f3:	insb   (%dx),%es:(%rdi)
-   29a1b96f4:	add    %al,(%rax)
-	...
-
-000000029a1b96f8 <.idata$7>:
-   29a1b96f8:	adc    $0x90,%al
-	...
-
-000000029a1b96fc <__lib64_libapi_ms_win_crt_conio_l1_1_0_a_iname>:
-   29a1b96fc:	(bad)
-   29a1b96fd:	jo     29a1b9768 <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname+0x10>
-   29a1b96ff:	sub    $0x772d736d,%eax
-   29a1b9704:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b970b:	movsxd 0x6e(%rdi),%ebp
-   29a1b970e:	imul   $0x312d316c,0x2d(%rdi),%ebp
-   29a1b9715:	sub    $0x6c642e30,%eax
-   29a1b971a:	insb   (%dx),%es:(%rdi)
-	...
-
-000000029a1b971c <.idata$7>:
-   29a1b971c:	sub    %dl,-0x6fd80000(%rax)
-
-000000029a1b9720 <.idata$7>:
-   29a1b9720:	sub    %dl,0x70610000(%rax)
-
-000000029a1b9724 <__lib64_libapi_ms_win_crt_environment_l1_1_0_a_iname>:
-   29a1b9724:	(bad)
-   29a1b9725:	jo     29a1b9790 <.idata$7>
-   29a1b9727:	sub    $0x772d736d,%eax
-   29a1b972c:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b9733:	outsb  %gs:(%rsi),(%dx)
-   29a1b9735:	jbe    29a1b97a0 <.idata$7>
-   29a1b9737:	jb     29a1b97a8 <.idata$7>
-   29a1b9739:	outsb  %ds:(%rsi),(%dx)
-   29a1b973a:	insl   (%dx),%es:(%rdi)
-   29a1b973b:	outsb  %gs:(%rsi),(%dx)
-   29a1b973d:	je     29a1b976c <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname+0x14>
-   29a1b973f:	insb   (%dx),%es:(%rdi)
-   29a1b9740:	xor    %ebp,0x2e302d31(%rip)        # 2c84bc477 <.debug_rnglists+0x2e2ec3d3>
-   29a1b9746:	fs insb (%dx),%es:(%rdi)
-   29a1b9748:	insb   (%dx),%es:(%rdi)
-   29a1b9749:	add    %al,(%rax)
-	...
-
-000000029a1b974c <.idata$7>:
-   29a1b974c:	cmp    $0x90,%al
-	...
-
-000000029a1b9750 <.idata$7>:
-   29a1b9750:	cmp    $0x90,%al
-	...
-
-000000029a1b9754 <.idata$7>:
-   29a1b9754:	cmp    $0x90,%al
-	...
-
-000000029a1b9758 <__lib64_libapi_ms_win_crt_heap_l1_1_0_a_iname>:
-   29a1b9758:	(bad)
-   29a1b9759:	jo     29a1b97c4 <__lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname+0x10>
-   29a1b975b:	sub    $0x772d736d,%eax
-   29a1b9760:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b9767:	push   $0x2d706165
-   29a1b976c:	insb   (%dx),%es:(%rdi)
-   29a1b976d:	xor    %ebp,0x2e302d31(%rip)        # 2c84bc4a4 <.debug_rnglists+0x2e2ec400>
-   29a1b9773:	fs insb (%dx),%es:(%rdi)
-   29a1b9775:	insb   (%dx),%es:(%rdi)
+000000029a1b9768 <.idata$7>:
+   29a1b9768:	push   %rax
+   29a1b9769:	nop
+	...
+
+000000029a1b976c <.idata$7>:
+   29a1b976c:	push   %rax
+   29a1b976d:	nop
+	...
+
+000000029a1b9770 <.idata$7>:
+   29a1b9770:	push   %rax
+   29a1b9771:	nop
+	...
+
+000000029a1b9774 <.idata$7>:
+   29a1b9774:	push   %rax
+   29a1b9775:	nop
 	...
 
 000000029a1b9778 <.idata$7>:
    29a1b9778:	push   %rax
    29a1b9779:	nop
 	...
 
@@ -7108,142 +7112,108 @@
 	...
 
 000000029a1b9798 <.idata$7>:
    29a1b9798:	push   %rax
    29a1b9799:	nop
 	...
 
-000000029a1b979c <.idata$7>:
-   29a1b979c:	push   %rax
-   29a1b979d:	nop
-	...
-
-000000029a1b97a0 <.idata$7>:
-   29a1b97a0:	push   %rax
-   29a1b97a1:	nop
-	...
-
-000000029a1b97a4 <.idata$7>:
-   29a1b97a4:	push   %rax
-   29a1b97a5:	nop
+000000029a1b979c <__lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname>:
+   29a1b979c:	(bad)
+   29a1b979d:	jo     29a1b9808 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x8>
+   29a1b979f:	sub    $0x772d736d,%eax
+   29a1b97a4:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b97ab:	jb     29a1b9822 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x22>
+   29a1b97ad:	outsb  %ds:(%rsi),(%dx)
+   29a1b97ae:	je     29a1b9819 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x19>
+   29a1b97b0:	insl   (%dx),%es:(%rdi)
+   29a1b97b1:	gs sub $0x312d316c,%eax
+   29a1b97b7:	sub    $0x6c642e30,%eax
+   29a1b97bc:	insb   (%dx),%es:(%rdi)
+   29a1b97bd:	add    %al,(%rax)
 	...
 
-000000029a1b97a8 <.idata$7>:
-   29a1b97a8:	push   %rax
-   29a1b97a9:	nop
+000000029a1b97c0 <.idata$7>:
+   29a1b97c0:	fs nop
 	...
 
-000000029a1b97ac <.idata$7>:
-   29a1b97ac:	push   %rax
-   29a1b97ad:	nop
+000000029a1b97c4 <.idata$7>:
+   29a1b97c4:	fs nop
 	...
 
-000000029a1b97b0 <.idata$7>:
-   29a1b97b0:	push   %rax
-   29a1b97b1:	nop
+000000029a1b97c8 <.idata$7>:
+   29a1b97c8:	fs nop
 	...
 
-000000029a1b97b4 <__lib64_libapi_ms_win_crt_runtime_l1_1_0_a_iname>:
-   29a1b97b4:	(bad)
-   29a1b97b5:	jo     29a1b9820 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x4>
-   29a1b97b7:	sub    $0x772d736d,%eax
-   29a1b97bc:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b97c3:	jb     29a1b983a <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x1e>
-   29a1b97c5:	outsb  %ds:(%rsi),(%dx)
-   29a1b97c6:	je     29a1b9831 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname+0x15>
-   29a1b97c8:	insl   (%dx),%es:(%rdi)
-   29a1b97c9:	gs sub $0x312d316c,%eax
-   29a1b97cf:	sub    $0x6c642e30,%eax
-   29a1b97d4:	insb   (%dx),%es:(%rdi)
-   29a1b97d5:	add    %al,(%rax)
+000000029a1b97cc <.idata$7>:
+   29a1b97cc:	fs nop
 	...
 
-000000029a1b97d8 <.idata$7>:
-   29a1b97d8:	fs nop
+000000029a1b97d0 <.idata$7>:
+   29a1b97d0:	fs nop
 	...
 
-000000029a1b97dc <.idata$7>:
-   29a1b97dc:	fs nop
+000000029a1b97d4 <.idata$7>:
+   29a1b97d4:	fs nop
 	...
 
-000000029a1b97e0 <.idata$7>:
-   29a1b97e0:	fs nop
+000000029a1b97d8 <__lib64_libapi_ms_win_crt_stdio_l1_1_0_a_iname>:
+   29a1b97d8:	(bad)
+   29a1b97d9:	jo     29a1b9844 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x10>
+   29a1b97db:	sub    $0x772d736d,%eax
+   29a1b97e0:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b97e7:	jae    29a1b985d <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x29>
+   29a1b97e9:	imul   $0x312d316c,%fs:0x2d(%rdi),%ebp
+   29a1b97f1:	sub    $0x6c642e30,%eax
+   29a1b97f6:	insb   (%dx),%es:(%rdi)
 	...
 
-000000029a1b97e4 <.idata$7>:
-   29a1b97e4:	fs nop
+000000029a1b97f8 <.idata$7>:
+   29a1b97f8:	js     29a1b978a <.idata$7+0x2>
 	...
 
-000000029a1b97e8 <.idata$7>:
-   29a1b97e8:	fs nop
+000000029a1b97fc <.idata$7>:
+   29a1b97fc:	js     29a1b978e <.idata$7+0x2>
 	...
 
-000000029a1b97ec <.idata$7>:
-   29a1b97ec:	fs nop
+000000029a1b9800 <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname>:
+   29a1b9800:	(bad)
+   29a1b9801:	jo     29a1b986c <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x38>
+   29a1b9803:	sub    $0x772d736d,%eax
+   29a1b9808:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b980f:	jae    29a1b9885 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x51>
+   29a1b9811:	jb     29a1b987c <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x48>
+   29a1b9813:	outsb  %ds:(%rsi),(%dx)
+   29a1b9814:	addr32 sub $0x312d316c,%eax
+   29a1b981a:	sub    $0x6c642e30,%eax
+   29a1b981f:	insb   (%dx),%es:(%rdi)
+   29a1b9820:	add    %al,(%rax)
 	...
 
-000000029a1b97f0 <.idata$7>:
-   29a1b97f0:	fs nop
-	...
+000000029a1b9824 <.idata$7>:
+   29a1b9824:	mov    %ss,-0x6f740000(%rax)
 
-000000029a1b97f4 <__lib64_libapi_ms_win_crt_stdio_l1_1_0_a_iname>:
-   29a1b97f4:	(bad)
-   29a1b97f5:	jo     29a1b9860 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x10>
-   29a1b97f7:	sub    $0x772d736d,%eax
-   29a1b97fc:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b9803:	jae    29a1b9879 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x29>
-   29a1b9805:	imul   $0x312d316c,%fs:0x2d(%rdi),%ebp
-   29a1b980d:	sub    $0x6c642e30,%eax
-   29a1b9812:	insb   (%dx),%es:(%rdi)
-	...
+000000029a1b9828 <.idata$7>:
+   29a1b9828:	mov    %ss,-0x6f740000(%rax)
 
-000000029a1b9814 <.idata$7>:
-   29a1b9814:	js     29a1b97a6 <.idata$7+0x2>
-	...
+000000029a1b982c <.idata$7>:
+   29a1b982c:	mov    %ss,-0x6f740000(%rax)
 
-000000029a1b9818 <.idata$7>:
-   29a1b9818:	js     29a1b97aa <.idata$7+0x2>
-	...
+000000029a1b9830 <.idata$7>:
+   29a1b9830:	mov    %ss,0x70610000(%rax)
 
-000000029a1b981c <__lib64_libapi_ms_win_crt_string_l1_1_0_a_iname>:
-   29a1b981c:	(bad)
-   29a1b981d:	jo     29a1b9888 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x38>
-   29a1b981f:	sub    $0x772d736d,%eax
-   29a1b9824:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b982b:	jae    29a1b98a1 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x51>
-   29a1b982d:	jb     29a1b9898 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x48>
-   29a1b982f:	outsb  %ds:(%rsi),(%dx)
-   29a1b9830:	addr32 sub $0x312d316c,%eax
-   29a1b9836:	sub    $0x6c642e30,%eax
-   29a1b983b:	insb   (%dx),%es:(%rdi)
-   29a1b983c:	add    %al,(%rax)
-	...
-
-000000029a1b9840 <.idata$7>:
-   29a1b9840:	mov    %ss,-0x6f740000(%rax)
-
-000000029a1b9844 <.idata$7>:
-   29a1b9844:	mov    %ss,-0x6f740000(%rax)
-
-000000029a1b9848 <.idata$7>:
-   29a1b9848:	mov    %ss,-0x6f740000(%rax)
-
-000000029a1b984c <.idata$7>:
-   29a1b984c:	mov    %ss,0x70610000(%rax)
-
-000000029a1b9850 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname>:
-   29a1b9850:	(bad)
-   29a1b9851:	jo     29a1b98bc <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x6c>
-   29a1b9853:	sub    $0x772d736d,%eax
-   29a1b9858:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   29a1b985f:	je     29a1b98ca <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x7a>
-   29a1b9861:	insl   (%dx),%es:(%rdi)
-   29a1b9862:	gs sub $0x312d316c,%eax
-   29a1b9868:	sub    $0x6c642e30,%eax
-   29a1b986d:	insb   (%dx),%es:(%rdi)
+000000029a1b9834 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname>:
+   29a1b9834:	(bad)
+   29a1b9835:	jo     29a1b98a0 <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x6c>
+   29a1b9837:	sub    $0x772d736d,%eax
+   29a1b983c:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   29a1b9843:	je     29a1b98ae <__lib64_libapi_ms_win_crt_time_l1_1_0_a_iname+0x7a>
+   29a1b9845:	insl   (%dx),%es:(%rdi)
+   29a1b9846:	gs sub $0x312d316c,%eax
+   29a1b984c:	sub    $0x6c642e30,%eax
+   29a1b9851:	insb   (%dx),%es:(%rdi)
 	...
 
 Disassembly of section .CRT:
 
 000000029a1ba000 <___crt_xc_start__>:
 	...
 
@@ -7262,23 +7232,21 @@
 	...
 
 000000029a1ba028 <___crt_xi_end__>:
 	...
 
 000000029a1ba030 <__xl_c>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:105
-   29a1ba030:	add    %dl,0x29a1b(%rip)        # 29a1e3a51 <.debug_rnglists+0x139ad>
-	...
+   29a1ba030:	loopne 29a1ba046 <__xl_z+0x6>
+   29a1ba032:	sbb    0x2(%rdx),%ebx
 
 000000029a1ba038 <__xl_d>:
 C:\M\B\src\build-UCRT64/C:/M/B/src/mingw-w64/mingw-w64-crt/crt/tlssup.c:171
-   29a1ba038:	rclb   $1,(%rbx,%rbx,1)
-   29a1ba03b:	(bad)
-   29a1ba03c:	add    (%rax),%al
-	...
+   29a1ba038:	mov    $0x14,%al
+   29a1ba03a:	sbb    0x2(%rdx),%ebx
 
 000000029a1ba040 <__xl_z>:
 	...
 
 000000029a1ba048 <___crt_xp_end__>:
 	...
 
@@ -7296,15 +7264,17 @@
 Disassembly of section .reloc:
 
 000000029a1bc000 <.reloc>:
    29a1bc000:	add    %ah,(%rax)
    29a1bc002:	add    %al,(%rax)
    29a1bc004:	or     $0x0,%al
    29a1bc006:	add    %al,(%rax)
-   29a1bc008:	fsubs  0x30000000(%rbp)
+   29a1bc008:	test   $0xa5,%al
+   29a1bc00a:	add    %al,(%rax)
+   29a1bc00c:	add    %dh,(%rax)
    29a1bc00e:	add    %al,(%rax)
    29a1bc010:	sub    %al,(%rax)
    29a1bc012:	add    %al,(%rax)
    29a1bc014:	adc    %ah,-0x5faf5fc0(%rax)
    29a1bc01a:	pop    %rax
    29a1bc01b:	movabs 0xa078a070a068a060,%al
    29a1bc024:	andb   $0xa0,-0x5f6f5f78(%rax)
@@ -7346,18 +7316,16 @@
    29a1bd032:	add    %al,(%rax)
    29a1bd034:	add    (%rax),%al
    29a1bd036:	mov    $0x19,%ah
    29a1bd038:	add    %al,(%rax)
    29a1bd03a:	or     %al,(%rax)
    29a1bd03c:	add    %al,(%rax)
    29a1bd03e:	add    %al,(%rax)
-   29a1bd040:	add    %dl,(%rbx,%rbx,1)
-   29a1bd043:	(bad)
-   29a1bd044:	add    (%rax),%al
-   29a1bd046:	add    %al,(%rax)
+   29a1bd040:	loopne 29a1bd055 <.debug_aranges+0x25>
+   29a1bd042:	sbb    0x2(%rdx),%ebx
    29a1bd048:	iret
 	...
 
 000000029a1bd060 <.debug_aranges>:
    29a1bd060:	sbb    $0x0,%al
    29a1bd062:	add    %al,(%rax)
    29a1bd064:	add    (%rax),%al
@@ -7369,18 +7337,16 @@
    29a1bd082:	add    %al,(%rax)
    29a1bd084:	add    (%rax),%al
    29a1bd086:	(bad)
    29a1bd087:	es add %al,(%rax)
    29a1bd08a:	or     %al,(%rax)
    29a1bd08c:	add    %al,(%rax)
    29a1bd08e:	add    %al,(%rax)
-   29a1bd090:	rclb   $1,(%rbx,%rbx,1)
-   29a1bd093:	(bad)
-   29a1bd094:	add    (%rax),%al
-   29a1bd096:	add    %al,(%rax)
+   29a1bd090:	mov    $0x14,%al
+   29a1bd092:	sbb    0x2(%rdx),%ebx
    29a1bd098:	ret
 	...
 
 000000029a1bd0b0 <.debug_aranges>:
    29a1bd0b0:	sbb    $0x0,%al
    29a1bd0b2:	add    %al,(%rax)
    29a1bd0b4:	add    (%rax),%al
@@ -7402,28 +7368,30 @@
    29a1bd0f2:	add    %al,(%rax)
    29a1bd0f4:	add    (%rax),%al
    29a1bd0f6:	jmp    29a1bd127 <.debug_aranges+0x7>
    29a1bd0f8:	add    %al,(%rax)
    29a1bd0fa:	or     %al,(%rax)
    29a1bd0fc:	add    %al,(%rax)
    29a1bd0fe:	add    %al,(%rax)
-   29a1bd100:	movabs 0x3d000000029a1b15,%al
-   29a1bd109:	add    $0x0,%eax
+   29a1bd100:	adcb   $0x0,0x29a1b(%rip)        # 29a1e6b22 <.debug_rnglists+0x16a7e>
+   29a1bd107:	add    %bh,0x5(%rip)        # 29a1bd112 <.debug_aranges+0x22>
 	...
 
 000000029a1bd120 <.debug_aranges>:
    29a1bd120:	sub    $0x0,%al
    29a1bd122:	add    %al,(%rax)
    29a1bd124:	add    (%rax),%al
    29a1bd126:	ss rex.RXB add %r8b,(%r8)
    29a1bd12a:	or     %al,(%rax)
    29a1bd12c:	add    %al,(%rax)
    29a1bd12e:	add    %al,(%rax)
-   29a1bd130:	loopne 29a1bd14c <.debug_aranges+0x2c>
-   29a1bd132:	sbb    0x2(%rdx),%ebx
+   29a1bd130:	rcrb   $0x1b,(%rdx)
+   29a1bd133:	(bad)
+   29a1bd134:	add    (%rax),%al
+   29a1bd136:	add    %al,(%rax)
    29a1bd138:	(bad)
 	...
 
 000000029a1bd150 <.debug_aranges>:
    29a1bd150:	sbb    $0x0,%al
    29a1bd152:	add    %al,(%rax)
    29a1bd154:	add    (%rax),%al
@@ -7444,85 +7412,84 @@
 000000029a1bd190 <.debug_aranges>:
    29a1bd190:	sub    $0x0,%al
    29a1bd192:	add    %al,(%rax)
    29a1bd194:	add    (%rax),%al
    29a1bd196:	(bad)
    29a1bd19b:	add    %al,(%rax)
    29a1bd19d:	add    %al,(%rax)
-   29a1bd19f:	add    %dl,0x1d(%rax)
-   29a1bd1a2:	sbb    0x2(%rdx),%ebx
+   29a1bd19f:	add    %dh,(%rax)
+   29a1bd1a1:	sbb    $0x29a1b,%eax
+   29a1bd1a6:	add    %al,(%rax)
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
-   29a1bd1d0:	push   %rax
-   29a1bd1d1:	and    %ebx,(%rbx)
-   29a1bd1d3:	(bad)
-   29a1bd1d4:	add    (%rax),%al
-   29a1bd1d6:	add    %al,(%rax)
+   29a1bd1d0:	xor    %ah,(%rcx)
+   29a1bd1d2:	sbb    0x2(%rdx),%ebx
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
-   29a1bd200:	movabs 0x6000000029a1b21,%al
+   29a1bd200:	andb   $0x1b,(%rcx)
+   29a1bd203:	(bad)
+   29a1bd204:	add    (%rax),%al
+   29a1bd206:	add    %al,(%rax)
+   29a1bd208:	(bad)
 	...
 
 000000029a1bd220 <.debug_aranges>:
    29a1bd220:	sub    $0x0,%al
    29a1bd222:	add    %al,(%rax)
    29a1bd224:	add    (%rax),%al
    29a1bd226:	(bad)
    29a1bd229:	add    %cl,(%rax)
    29a1bd22b:	add    %al,(%rax)
    29a1bd22d:	add    %al,(%rax)
-   29a1bd22f:	add    %dh,0x29a1b21(%rax)
+   29a1bd22f:	add    %dl,0x29a1b21(%rax)
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
-   29a1bd25f:	add    %al,%al
-   29a1bd261:	and    %ebx,(%rbx)
-   29a1bd263:	(bad)
-   29a1bd264:	add    (%rax),%al
-   29a1bd266:	add    %al,(%rax)
-   29a1bd268:	(bad)
+   29a1bd25f:	add    %ah,0x29a1b21(%rax)
+   29a1bd265:	add    %al,(%rax)
+   29a1bd267:	add    %bl,(%rsi)
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
-   29a1bd28f:	add    %ah,%al
+   29a1bd28f:	add    %al,%al
    29a1bd291:	and    %ebx,(%rbx)
    29a1bd293:	(bad)
    29a1bd294:	add    (%rax),%al
    29a1bd296:	add    %al,(%rax)
    29a1bd298:	(bad)
    29a1bd299:	add    (%rax),%al
 	...
@@ -7530,15 +7497,15 @@
 000000029a1bd2b0 <.debug_aranges>:
    29a1bd2b0:	sub    $0x0,%al
    29a1bd2b2:	add    %al,(%rax)
    29a1bd2b4:	add    (%rax),%al
    29a1bd2b6:	fildl  0x80000(%rcx)
    29a1bd2bc:	add    %al,(%rax)
    29a1bd2be:	add    %al,(%rax)
-   29a1bd2c0:	xor    %ah,0x29a1b(%rip)        # 29a1e6ce1 <.debug_rnglists+0x16c3d>
+   29a1bd2c0:	add    %ah,0x29a1b(%rip)        # 29a1e6ce1 <.debug_rnglists+0x16c3d>
    29a1bd2c6:	add    %al,(%rax)
    29a1bd2c8:	xor    (%rax),%al
 	...
 
 Disassembly of section .debug_info:
 
 000000029a1be000 <.debug_info>:
@@ -10535,16 +10502,16 @@
    29a1bfa01:	xor    (%rax),%ah
    29a1bfa03:	sub    $0x3d647473,%eax
    29a1bfa08:	outsb  %ds:(%esi),(%dx)
    29a1bfa0a:	jne    29a1bfa45 <.debug_info+0x91>
    29a1bfa0c:	cmp    %eax,(%rax)
    29a1bfa0e:	or     $0xa2,%al
    29a1bfa10:	add    %eax,(%rax)
-   29a1bfa12:	add    %cl,0x1(%rdx)
-   29a1bfa18:	adc    $0x1b,%al
+   29a1bfa12:	add    %cl,-0x1fffffff(%rdx)
+   29a1bfa18:	adc    (%rbx),%ebx
    29a1bfa1a:	(bad)
    29a1bfa1b:	add    (%rax),%al
    29a1bfa1d:	add    %al,(%rax)
    29a1bfa1f:	iret
    29a1bfa20:	add    %al,(%rax)
    29a1bfa22:	add    %al,(%rax)
    29a1bfa24:	add    %al,(%rax)
@@ -11287,46 +11254,40 @@
    29a1bff2c:	add    %al,(%rax)
    29a1bff2e:	test   %al,0x59110000(%rip)        # 2f32cff34 <.debug_rnglists+0x590ffe90>
    29a1bff34:	add    %eax,(%rax)
    29a1bff36:	add    %al,(%rax)
    29a1bff38:	adc    0x5f(%rdi),%bl
    29a1bff3b:	insl   (%dx),%es:(%rdi)
    29a1bff3c:	(bad)
-   29a1bff3d:	imul   $0xb0013501,0x0(%rsi),%ebp
+   29a1bff3d:	imul   $0x90013501,0x0(%rsi),%ebp
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
-   29a1bff59:	adc    %edi,%ecx
-   29a1bff5b:	adc    $0x1b,%al
-   29a1bff5d:	(bad)
-   29a1bff5e:	add    (%rax),%al
-   29a1bff60:	add    %al,(%rax)
-   29a1bff62:	mov    $0x5,%bl
-   29a1bff64:	add    %al,(%rax)
-   29a1bff66:	add    %cl,(%rcx)
-   29a1bff68:	pop    %rdi
-   29a1bff69:	pop    %rdi
+   29a1bff59:	adc    0x29a1b14(%rdi),%ebp
+   29a1bff5f:	add    %al,(%rax)
+   29a1bff61:	add    %dh,0x5(%rbx)
+   29a1bff67:	or     %ebx,0x5f(%rdi)
    29a1bff6a:	outsl  %fs:(%rsi),(%dx)
    29a1bff6c:	pop    %rdi
    29a1bff6d:	insb   (%dx),%es:(%edi)
    29a1bff6f:	outsl  %ds:(%rsi),(%dx)
    29a1bff70:	(bad)
    29a1bff75:	je     29a1bffe6 <.debug_info+0x632>
    29a1bff77:	jb     29a1bffec <.debug_info+0x638>
    29a1bff79:	add    %ah,(%rax)
-   29a1bff7b:	rex adc $0x1b,%al
+   29a1bff7b:	and    %dl,(%rbx,%rbx,1)
    29a1bff7e:	(bad)
    29a1bff7f:	add    (%rax),%al
    29a1bff81:	add    %al,(%rax)
    29a1bff83:	push   $0x0
    29a1bff85:	add    %al,(%rax)
    29a1bff87:	add    %al,(%rax)
    29a1bff89:	add    %al,(%rax)
@@ -11342,34 +11303,32 @@
    29a1bffa1:	add    (%r8),%eax
    29a1bffa4:	add    %cl,(%rdx)
    29a1bffa6:	imul   $0xf523,(%rax),%eax
    29a1bffac:	add    %bl,0x3(%rdi)
    29a1bffaf:	add    %al,(%rax)
    29a1bffb1:	pop    %rbx
    29a1bffb2:	add    (%rax),%eax
-   29a1bffb4:	add    %dl,0x29a1b14(,%rcx,4)
+   29a1bffb4:	add    %dl,0x29a1b14(,%rbp,2)
    29a1bffbb:	add    %al,(%rax)
    29a1bffbd:	add    %ch,0x5(%rdx)
    29a1bffc0:	add    %al,(%rax)
    29a1bffc2:	adc    $0x3095201,%eax
-   29a1bffc7:	add    %dl,(%rbx,%rbx,1)
-   29a1bffca:	(bad)
-   29a1bffcb:	add    (%rax),%al
-   29a1bffcd:	add    %al,(%rax)
+   29a1bffc7:	loopne 29a1bffdc <.debug_info+0x628>
+   29a1bffc9:	sbb    0x2(%rdx),%ebx
    29a1bffcf:	add    %al,(%rax)
    29a1bffd1:	or     %ebx,0x5f(%rdi)
    29a1bffd4:	outsl  %fs:(%rsi),(%dx)
    29a1bffd6:	pop    %rdi
    29a1bffd7:	insb   (%dx),%es:(%edi)
    29a1bffd9:	outsl  %ds:(%rsi),(%dx)
    29a1bffda:	(bad)
    29a1bffdf:	je     29a1c0050 <.debug_info+0x3b>
    29a1bffe1:	jb     29a1c0056 <.debug_info+0x41>
-   29a1bffe3:	add    %dl,(%rax,%rax,1)
-   29a1bffe6:	adc    $0x1b,%al
+   29a1bffe3:	add    %dl,(%rax,%riz,8)
+   29a1bffe6:	adc    (%rbx),%ebx
    29a1bffe8:	(bad)
    29a1bffe9:	add    (%rax),%al
    29a1bffeb:	add    %al,(%rax)
    29a1bffed:	cmp    (%rax),%al
    29a1bffef:	add    %al,(%rax)
    29a1bfff1:	add    %al,(%rax)
    29a1bfff3:	add    %al,(%rax)
@@ -12255,15 +12214,15 @@
    29a1c0664:	xor    (%rax),%ah
    29a1c0666:	sub    $0x3d647473,%eax
    29a1c066b:	outsb  %ds:(%esi),(%dx)
    29a1c066d:	jne    29a1c06a8 <.debug_info+0x91>
    29a1c066f:	cmp    %eax,(%rax)
    29a1c0671:	or     $0x98,%al
    29a1c0673:	add    (%rax),%eax
-   29a1c0675:	add    %al,-0x2ffffffd(%rax)
+   29a1c0675:	add    %al,-0x4ffffffd(%rax)
    29a1c067b:	adc    $0x1b,%al
    29a1c067d:	(bad)
    29a1c067e:	add    (%rax),%al
    29a1c0680:	add    %al,(%rax)
    29a1c0682:	ret
    29a1c0683:	add    %al,(%rax)
    29a1c0685:	add    %al,(%rax)
@@ -12923,20 +12882,17 @@
    29a1c0c26:	fs jns 29a1c0c97 <.debug_info+0x680>
    29a1c0c29:	pop    %rdi
    29a1c0c2a:	je     29a1c0c98 <.debug_info+0x681>
    29a1c0c2c:	jae    29a1c0c8d <.debug_info+0x676>
    29a1c0c2e:	fs je  29a1c0ca0 <.debug_info+0x689>
    29a1c0c31:	jb     29a1c0c33 <.debug_info+0x61c>
    29a1c0c33:	add    %ecx,0x14001(%rcx)
-   29a1c0c39:	add    %dl,%al
-   29a1c0c3b:	adc    $0x1b,%al
-   29a1c0c3d:	(bad)
-   29a1c0c3e:	add    (%rax),%al
-   29a1c0c40:	add    %al,(%rax)
-   29a1c0c42:	(bad)
+   29a1c0c39:	add    %dh,0x29a1b14(%rax)
+   29a1c0c3f:	add    %al,(%rax)
+   29a1c0c41:	add    %ch,(%rdi)
    29a1c0c43:	add    %al,(%rax)
    29a1c0c45:	add    %al,(%rax)
    29a1c0c47:	add    %al,(%rax)
    29a1c0c49:	add    %al,(%rcx)
    29a1c0c4b:	pushf
    29a1c0c4c:	jge    29a1c0c54 <.debug_info+0x63d>
    29a1c0c4e:	add    %al,(%rax)
@@ -12956,32 +12912,27 @@
    29a1c0c72:	add    %al,(%rax)
    29a1c0c74:	or     0x0(%rax,%rax,1),%dh
    29a1c0c78:	add    %bh,(%rbx)
    29a1c0c7a:	add    %eax,%fs:(%rax)
    29a1c0c7d:	add    %bl,-0x65fffffd(%rsi)
    29a1c0c83:	add    (%rax),%eax
    29a1c0c85:	add    %cl,(%rsi)
-   29a1c0c87:	cmc
-   29a1c0c88:	adc    $0x1b,%al
-   29a1c0c8a:	(bad)
-   29a1c0c8b:	add    (%rax),%al
-   29a1c0c8d:	add    %al,(%rax)
+   29a1c0c87:	sbb    0x2(%r18),%r11d
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
-   29a1c0ca8:	nop
-   29a1c0ca9:	adc    $0x29a1b,%eax
-   29a1c0cae:	add    %al,(%rax)
+   29a1c0ca8:	jo     29a1c0cbf <.debug_info+0x6a8>
+   29a1c0caa:	sbb    0x2(%rdx),%ebx
    29a1c0cb0:	add    (%rax),%eax
    29a1c0cb2:	add    %al,(%rax)
    29a1c0cb4:	add    %al,(%rax)
    29a1c0cb6:	add    %al,(%rax)
    29a1c0cb8:	add    %ebx,0x1c000006(%rdi,%rsi,4)
    29a1c0cbf:	data16 jne 29a1c0d30 <.debug_info+0x719>
    29a1c0cc2:	movsxd (%rax),%eax
@@ -13018,16 +12969,16 @@
    29a1c0d0f:	rex.WRXB or (%r12,%r8,1),%r12b
    29a1c0d13:	add    %al,(%rax)
    29a1c0d15:	pshufw $0x50,0x0(%rbx),%mm6
    29a1c0d1a:	or     $0xaa,%eax
    29a1c0d1f:	add    %bl,(%rsi)
    29a1c0d21:	mov    $0x6,%bh
    29a1c0d23:	add    %al,(%rax)
-   29a1c0d25:	add    %dl,0x29a1b(%rip)        # 29a1ea746 <.debug_rnglists+0x1a6a2>
-   29a1c0d2b:	add    %al,(%rax)
+   29a1c0d25:	loopne 29a1c0d3b <.debug_info+0x724>
+   29a1c0d27:	sbb    0x2(%rdx),%ebx
    29a1c0d2d:	addl   $0x0,(%rax)
    29a1c0d33:	add    %al,(%rax)
    29a1c0d35:	add    %ebx,0x6d3(%rdi,%rax,1)
    29a1c0d3c:	mov    $0x3,%ah
    29a1c0d3e:	add    %al,(%rax)
    29a1c0d40:	lods   %ds:(%rsi),%al
    29a1c0d41:	add    (%rax),%eax
@@ -13051,17 +13002,17 @@
    29a1c0d61:	add    %al,(%rax)
    29a1c0d63:	adc    %bh,%dh
    29a1c0d65:	(bad)
    29a1c0d66:	add    %al,(%rax)
    29a1c0d68:	(bad)
    29a1c0d69:	mov    $0x6,%bh
    29a1c0d6b:	add    %al,(%rax)
-   29a1c0d6d:	xor    %dl,0x29a1b(%rip)        # 29a1ea78e <.debug_rnglists+0x1a6ea>
+   29a1c0d6d:	adc    %dl,0x29a1b(%rip)        # 29a1ea78e <.debug_rnglists+0x1a6ea>
    29a1c0d73:	add    %al,(%rax)
-   29a1c0d75:	add    %dh,(%rax)
+   29a1c0d75:	add    %dl,(%rax)
    29a1c0d77:	adc    $0x29a1b,%eax
    29a1c0d7c:	add    %al,(%rax)
    29a1c0d7e:	sub    (%rax),%eax
    29a1c0d80:	add    %al,(%rax)
    29a1c0d82:	add    %al,(%rax)
    29a1c0d84:	add    %al,(%rax)
    29a1c0d86:	add    %ecx,0x1(%rbp)
@@ -13093,16 +13044,17 @@
    29a1c0dc2:	incb   (%rsi)
    29a1c0dc4:	add    %al,(%rax)
    29a1c0dc6:	insb   (%dx),%es:(%rdi)
    29a1c0dc7:	add    $0x0,%al
    29a1c0dc9:	add    %ch,0x4(%rax)
    29a1c0dcc:	add    %al,(%rax)
    29a1c0dce:	add    %cl,(%rsi)
-   29a1c0dd0:	jne    29a1c0de7 <.debug_info+0x9>
-   29a1c0dd2:	sbb    0x2(%rdx),%ebx
+   29a1c0dd0:	push   %rbp
+   29a1c0dd1:	adc    $0x29a1b,%eax
+   29a1c0dd6:	add    %al,(%rax)
    29a1c0dd8:	faddl  0x0(%rip)        # 29a1c0dde <.debug_info>
 
 000000029a1c0dde <.debug_info>:
    29a1c0dde:	ja     29a1c0de1 <.debug_info+0x3>
    29a1c0de0:	add    %al,(%rax)
    29a1c0de2:	add    $0x9b080100,%eax
    29a1c0de7:	or     %al,(%rax)
@@ -13335,21 +13287,18 @@
    29a1c103a:	sub    $0x3d647473,%eax
    29a1c103f:	outsb  %ds:(%esi),(%dx)
    29a1c1041:	jne    29a1c107c <.debug_info+0x91>
    29a1c1043:	cmp    %eax,(%rax)
    29a1c1045:	or     $0xbb,%al
    29a1c1047:	add    $0x5f10000,%eax
    29a1c104c:	add    %al,(%rax)
-   29a1c104e:	movabs 0x3d000000029a1b15,%al
-   29a1c1057:	add    $0x0,%eax
-   29a1c105c:	add    %al,(%rax)
-   29a1c105e:	test   %al,(%rsi)
-   29a1c1060:	add    %al,(%rax)
-   29a1c1062:	(bad)
-   29a1c1063:	pop    %rdi
+   29a1c104e:	adcb   $0x0,0x29a1b(%rip)        # 29a1eaa70 <.debug_rnglists+0x1a9cc>
+   29a1c1055:	add    %bh,0x5(%rip)        # 29a1c1060 <.debug_info+0x75>
+   29a1c105b:	add    %al,(%rax)
+   29a1c105d:	add    %al,0x5f060000(%rsi,%rax,1)
    29a1c1064:	pop    %rdi
    29a1c1065:	outsb  %ds:(%esi),(%dx)
    29a1c1067:	jne    29a1c10cc <.debug_info+0xe1>
    29a1c1069:	pop    %rdi
    29a1c106a:	jbe    29a1c10cd <.debug_info+0xe2>
    29a1c106c:	pop    %rdi
    29a1c106d:	insb   (%dx),%es:(%rdi)
@@ -15045,18 +14994,17 @@
    29a1c1e5d:	insb   (%dx),%es:(%rdi)
    29a1c1e5e:	outsl  %ds:(%rsi),(%dx)
    29a1c1e5f:	movsxd 0x74(%rcx),%esp
    29a1c1e62:	outsl  %ds:(%rsi),(%dx)
    29a1c1e63:	jb     29a1c1e65 <.debug_info+0xe7a>
    29a1c1e65:	add    %esp,%ebp
    29a1c1e67:	add    %eax,(%rcx)
-   29a1c1e69:	adcb   $0x1b,(%rdi)
-   29a1c1e6c:	(bad)
-   29a1c1e6d:	add    (%rax),%al
-   29a1c1e6f:	add    %al,(%rax)
+   29a1c1e69:	(bad)
+   29a1c1e6a:	(bad)
+   29a1c1e6b:	sbb    0x2(%rdx),%ebx
    29a1c1e71:	pop    %rbp
    29a1c1e72:	add    (%rax),%eax
    29a1c1e74:	add    %al,(%rax)
    29a1c1e76:	add    %al,(%rax)
    29a1c1e78:	add    %al,(%rcx)
    29a1c1e7a:	pushf
    29a1c1e7b:	mov    (%rbx),%dl
@@ -15074,19 +15022,19 @@
    29a1c1ea2:	add    %ebp,%ecx
    29a1c1ea4:	add    %eax,(%rdi)
    29a1c1ea6:	and    $0x8f000001,%eax
    29a1c1eab:	add    $0x0,%al
    29a1c1ead:	add    %cl,0x21000004(%rbp)
    29a1c1eb3:	mov    (%rbx),%dl
    29a1c1eb5:	add    %al,(%rax)
-   29a1c1eb7:	add    $0x29a1b18,%eax
-   29a1c1ebc:	add    %al,(%rax)
-   29a1c1ebe:	add    %al,(%rdx)
-   29a1c1ec0:	rex.X add %al,(%rax)
-   29a1c1ec3:	add    %dh,%ch
+   29a1c1eb7:	in     $0x17,%eax
+   29a1c1eb9:	sbb    0x2(%rdx),%ebx
+   29a1c1ebf:	add    0x0(%rdx),%al
+   29a1c1ec2:	add    %al,(%rax)
+   29a1c1ec4:	cmc
    29a1c1ec5:	add    %eax,(%rbx)
    29a1c1ec7:	xor    $0x13,%al
    29a1c1ec9:	add    %al,(%rax)
    29a1c1ecb:	sbb    0x1b000013(%rcx),%esp
    29a1c1ed1:	scas   %es:(%rdi),%eax
    29a1c1ed2:	adc    (%rax),%eax
    29a1c1ed4:	add    %bl,(%rbx)
@@ -15138,16 +15086,16 @@
    29a1c1f45:	add    %al,(%rax)
    29a1c1f47:	or     0x14(%rbx),%bl
    29a1c1f4a:	add    %al,(%rax)
    29a1c1f4c:	xchg   %eax,(%rdi)
    29a1c1f4e:	add    %al,(%rax)
    29a1c1f50:	jg     29a1c1f59 <.debug_info+0xf6e>
    29a1c1f52:	add    %al,(%rax)
-   29a1c1f54:	or     (%rcx),%ebx
-   29a1c1f56:	sbb    %ebx,(%rbx)
+   29a1c1f54:	or     %ecx,%edi
+   29a1c1f56:	sbb    %bl,(%rbx)
    29a1c1f58:	(bad)
    29a1c1f59:	add    (%rax),%al
    29a1c1f5b:	add    %al,(%rax)
    29a1c1f5d:	(bad)
    29a1c1f5e:	(bad)
    29a1c1f5f:	add    %al,(%rax)
    29a1c1f61:	add    $0x1,%al
@@ -15159,22 +15107,19 @@
    29a1c1f70:	pop    %rax
    29a1c1f71:	add    0x0(%rbp),%dh
    29a1c1f74:	add    $0x2,%al
    29a1c1f76:	ja     29a1c1f98 <.debug_info+0xfad>
    29a1c1f78:	add    0x0(%rax,%rax,1),%dh
    29a1c1f7c:	add    %bl,(%rdi,%rdi,2)
    29a1c1f7f:	adc    $0x0,%al
-   29a1c1f81:	add    %ah,0x29a1b18(%rdi)
+   29a1c1f81:	add    %al,0x29a1b18(%rdi)
    29a1c1f87:	add    %al,(%rax)
    29a1c1f89:	add    %al,(%rdx)
-   29a1c1f8b:	cmpsl  %es:(%rdi),%ds:(%rsi)
-   29a1c1f8c:	sbb    %bl,(%rbx)
-   29a1c1f8e:	(bad)
-   29a1c1f8f:	add    (%rax),%al
-   29a1c1f91:	add    %al,(%rax)
+   29a1c1f8b:	xchg   %ebx,(%rax)
+   29a1c1f8d:	sbb    0x2(%rdx),%ebx
    29a1c1f93:	or     (%rax),%eax
    29a1c1f95:	add    %al,(%rax)
    29a1c1f97:	add    %al,(%rax)
    29a1c1f99:	add    %al,(%rax)
    29a1c1f9b:	{rex2 0x1} cmp (%r8),%edx
    29a1c1f9f:	add    %al,(%rax)
    29a1c1fa1:	add    -0x47ffffec(%rsi),%ebp
@@ -15192,20 +15137,17 @@
    29a1c1fbf:	add    %dl,%dl
    29a1c1fc1:	(bad)
    29a1c1fc2:	add    %al,(%rax)
    29a1c1fc4:	rolb   $1,(%rdi)
    29a1c1fc6:	add    %al,(%rax)
    29a1c1fc8:	adc    0x14(%rdi),%bh
    29a1c1fcb:	add    %al,(%rax)
-   29a1c1fcd:	cmpsl  %es:(%rdi),%ds:(%rsi)
-   29a1c1fce:	sbb    %bl,(%rbx)
-   29a1c1fd0:	(bad)
-   29a1c1fd1:	add    (%rax),%al
-   29a1c1fd3:	add    %al,(%rax)
-   29a1c1fd5:	add    $0xa7,%al
+   29a1c1fcd:	xchg   %ebx,(%rax)
+   29a1c1fcf:	sbb    0x2(%rdx),%ebx
+   29a1c1fd5:	add    $0x87,%al
    29a1c1fd7:	sbb    %bl,(%rbx)
    29a1c1fd9:	(bad)
    29a1c1fda:	add    (%rax),%al
    29a1c1fdc:	add    %al,(%rax)
    29a1c1fde:	or     (%rax),%eax
    29a1c1fe0:	add    %al,(%rax)
    29a1c1fe2:	add    %al,(%rax)
@@ -15224,27 +15166,30 @@
    29a1c2001:	add    %al,(%rax)
    29a1c2003:	add    -0x9ffffec(%rbp),%edx
    29a1c2009:	(bad)
    29a1c200a:	add    %al,(%rax)
    29a1c200c:	hlt
    29a1c200d:	(bad)
    29a1c200e:	add    %al,(%rax)
-   29a1c2010:	or     0x29a1b18(%rdi),%ebp
+   29a1c2010:	or     0x29a1b18(%rdi),%ecx
    29a1c2016:	add    %al,(%rax)
    29a1c2018:	add    %dh,%bh
    29a1c201a:	adc    $0x0,%al
    29a1c201c:	add    %al,(%rcx,%rax,1)
    29a1c201f:	push   %rdx
    29a1c2020:	add    0x0(%rbp),%dh
    29a1c2023:	add    %al,(%rax)
    29a1c2025:	add    %ah,(%rcx)
    29a1c2027:	jg     29a1c203d <.debug_info+0x1052>
    29a1c2029:	add    %al,(%rax)
-   29a1c202b:	jb     29a1c2046 <.debug_info+0x105b>
-   29a1c202d:	sbb    0x2(%rdx),%ebx
+   29a1c202b:	push   %rdx
+   29a1c202c:	sbb    %ebx,(%rbx)
+   29a1c202e:	(bad)
+   29a1c202f:	add    (%rax),%al
+   29a1c2031:	add    %al,(%rax)
    29a1c2033:	add    0x0(%rax,%rax,1),%ch
    29a1c2037:	add    %dl,%dl
    29a1c2039:	add    %ecx,(%rsi,%rcx,8)
    29a1c203c:	adc    %al,(%rax)
    29a1c203e:	add    %al,(%rbx)
    29a1c2040:	scas   %es:(%rdi),%al
    29a1c2041:	adc    $0x0,%al
@@ -15263,16 +15208,19 @@
    29a1c205d:	add    %bl,(%rdx)
    29a1c205f:	or     %al,(%rax)
    29a1c2061:	add    %bl,(%rax)
    29a1c2063:	or     %al,(%rax)
    29a1c2065:	add    %dh,(%rdi)
    29a1c2067:	jg     29a1c207d <.debug_info+0x1092>
    29a1c2069:	add    %al,(%rax)
-   29a1c206b:	jb     29a1c2086 <.debug_info+0x109b>
-   29a1c206d:	sbb    0x2(%rdx),%ebx
+   29a1c206b:	push   %rdx
+   29a1c206c:	sbb    %ebx,(%rbx)
+   29a1c206e:	(bad)
+   29a1c206f:	add    (%rax),%al
+   29a1c2071:	add    %al,(%rax)
    29a1c2073:	add    $0x6c,%al
    29a1c2075:	add    %al,(%rax)
    29a1c2077:	add    %al,(%rcx)
    29a1c2079:	(bad)
    29a1c207a:	add    %eax,(%rcx)
    29a1c207c:	add    0x24000014(%rsi),%ebp
    29a1c2082:	or     %al,(%rax)
@@ -15284,29 +15232,29 @@
    29a1c2095:	add    %al,(%rbx)
    29a1c2097:	xchg   %eax,%ebp
    29a1c2098:	adc    $0x0,%al
    29a1c209a:	add    %bh,(%rsi)
    29a1c209c:	or     %al,(%rax)
    29a1c209e:	add    %bh,(%rax,%rcx,1)
    29a1c20a1:	add    %al,(%rax)
-   29a1c20a3:	or     0x19(%rsi),%edi
+   29a1c20a3:	or     0x19(%rsi),%ebx
    29a1c20a6:	sbb    0x2(%rdx),%ebx
    29a1c20ac:	notl   (%rax,%rax,1)
    29a1c20af:	add    %al,(%rcx,%rax,1)
    29a1c20b2:	push   %rdx
    29a1c20b3:	add    0x0(%rbp),%dh
    29a1c20b6:	add    %al,(%rax)
    29a1c20b8:	add    %bl,(%rdi,%rdi,2)
    29a1c20bb:	adc    $0x0,%al
-   29a1c20bd:	add    %ah,(%rdi)
+   29a1c20bd:	add    %al,(%rdi)
    29a1c20bf:	sbb    (%rbx),%bl
    29a1c20c1:	(bad)
    29a1c20c2:	add    (%rax),%al
    29a1c20c4:	add    %al,(%rax)
-   29a1c20c6:	add    (%rdi),%ah
+   29a1c20c6:	add    (%rdi),%al
    29a1c20c8:	sbb    (%rbx),%bl
    29a1c20ca:	(bad)
    29a1c20cb:	add    (%rax),%al
    29a1c20cd:	add    %al,(%rax)
    29a1c20cf:	or     (%rax),%al
    29a1c20d1:	add    %al,(%rax)
    29a1c20d3:	add    %al,(%rax)
@@ -15329,15 +15277,15 @@
    29a1c2104:	adc    0x14(%rdi),%bh
    29a1c2107:	add    %al,(%rax)
    29a1c2109:	(bad)
    29a1c210a:	sbb    (%rbx),%bl
    29a1c210c:	(bad)
    29a1c210d:	add    (%rax),%al
    29a1c210f:	add    %al,(%rax)
-   29a1c2111:	add    $0x27,%al
+   29a1c2111:	add    $0x7,%al
    29a1c2113:	sbb    (%rbx),%bl
    29a1c2115:	(bad)
    29a1c2116:	add    (%rax),%al
    29a1c2118:	add    %al,(%rax)
    29a1c211a:	or     (%rax),%al
    29a1c211c:	add    %al,(%rax)
    29a1c211e:	add    %al,(%rax)
@@ -15350,30 +15298,36 @@
    29a1c2130:	add    %al,(%rax)
    29a1c2132:	add    0x77000014(%rdx),%esp
    29a1c2138:	or     %al,(%rax)
    29a1c213a:	add    %dh,0x8(%rbp)
    29a1c213d:	add    %al,(%rax)
    29a1c213f:	add    -0x79ffffec(%rbp),%edx
    29a1c2145:	or     %al,(%rax)
-   29a1c2147:	add    %al,0x2f0b0000(%rax,%rcx,1)
+   29a1c2147:	add    %al,0xf0b0000(%rax,%rcx,1)
    29a1c214e:	sbb    (%rbx),%bl
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
-   29a1c2166:	add    %al,0x1a(%rax)
-   29a1c2169:	sbb    0x2(%rdx),%ebx
-   29a1c216f:	add    %eax,0x1a(%rax)
-   29a1c2172:	sbb    0x2(%rdx),%ebx
+   29a1c2166:	add    %ah,(%rax)
+   29a1c2168:	sbb    (%rbx),%bl
+   29a1c216a:	(bad)
+   29a1c216b:	add    (%rax),%al
+   29a1c216d:	add    %al,(%rax)
+   29a1c216f:	add    %esp,(%rax)
+   29a1c2171:	sbb    (%rbx),%bl
+   29a1c2173:	(bad)
+   29a1c2174:	add    (%rax),%al
+   29a1c2176:	add    %al,(%rax)
    29a1c2178:	or     (%rax),%eax
    29a1c217a:	add    %al,(%rax)
    29a1c217c:	add    %al,(%rax)
    29a1c217e:	add    %al,(%rax)
    29a1c2180:	faddl  (%rcx)
    29a1c2182:	and    %dl,(%rdx)
    29a1c2184:	add    %al,(%rax)
@@ -15386,20 +15340,21 @@
    29a1c21a1:	xchg   %eax,%ebp
    29a1c21a2:	adc    $0x0,%al
    29a1c21a4:	add    %ch,-0x57fffff8(%rdx)
    29a1c21aa:	or     %al,(%rax)
    29a1c21ac:	add    %dl,(%rdx)
    29a1c21ae:	jg     29a1c21c4 <.debug_info+0x11d9>
    29a1c21b0:	add    %al,(%rax)
-   29a1c21b2:	rex sbb (%rbx),%bl
-   29a1c21b5:	(bad)
-   29a1c21b6:	add    (%rax),%al
-   29a1c21b8:	add    %al,(%rax)
-   29a1c21ba:	add    0x1a(%rax),%eax
-   29a1c21bd:	sbb    0x2(%rdx),%ebx
+   29a1c21b2:	and    %bl,(%rdx)
+   29a1c21b4:	sbb    0x2(%rdx),%ebx
+   29a1c21ba:	add    (%rax),%esp
+   29a1c21bc:	sbb    (%rbx),%bl
+   29a1c21be:	(bad)
+   29a1c21bf:	add    (%rax),%al
+   29a1c21c1:	add    %al,(%rax)
    29a1c21c3:	or     (%rax),%eax
    29a1c21c5:	add    %al,(%rax)
    29a1c21c7:	add    %al,(%rax)
    29a1c21c9:	add    %al,(%rax)
    29a1c21cb:	(bad)
    29a1c21cc:	add    %eax,(%rcx)
    29a1c21ce:	add    -0x4bffffec(%rsi),%ebp
@@ -15411,18 +15366,16 @@
    29a1c21e9:	xchg   %eax,%ebp
    29a1c21ea:	adc    $0x0,%al
    29a1c21ec:	add    %cl,%dh
    29a1c21ee:	or     %al,(%rax)
    29a1c21f0:	add    %cl,%ah
    29a1c21f2:	or     %al,(%rax)
    29a1c21f4:	add    %cl,(%rbx)
-   29a1c21f6:	rex.W sbb (%rbx),%bl
-   29a1c21f9:	(bad)
-   29a1c21fa:	add    (%rax),%al
-   29a1c21fc:	add    %al,(%rax)
+   29a1c21f6:	sub    %bl,(%rdx)
+   29a1c21f8:	sbb    0x2(%rdx),%ebx
    29a1c21fe:	notl   (%rax,%rax,1)
    29a1c2201:	add    %al,(%rcx,%rax,1)
    29a1c2204:	push   %rdx
    29a1c2205:	add    0x0(%rbp),%dh
    29a1c2208:	add    %al,(%rax)
    29a1c220a:	add    %ah,(%rdx)
    29a1c220c:	and    $0x14,%al
@@ -15444,20 +15397,17 @@
    29a1c2231:	add    %al,(%rax)
    29a1c2233:	testb  $0x0,(%rax)
    29a1c2236:	add    %dh,%ah
    29a1c2238:	or     %al,(%rax)
    29a1c223a:	add    %dl,(%rdx)
    29a1c223c:	jg     29a1c2252 <.debug_info+0x1267>
    29a1c223e:	add    %al,(%rax)
-   29a1c2240:	scas   %es:(%rdi),%al
-   29a1c2241:	sbb    (%rbx),%bl
-   29a1c2243:	(bad)
-   29a1c2244:	add    (%rax),%al
-   29a1c2246:	add    %al,(%rax)
-   29a1c2248:	add    %ebp,0x29a1b1a(%rsi)
+   29a1c2240:	mov    (%rdx),%ds
+   29a1c2242:	sbb    0x2(%rdx),%ebx
+   29a1c2248:	add    %ecx,0x29a1b1a(%rsi)
    29a1c224e:	add    %al,(%rax)
    29a1c2250:	add    %cl,(%rdx)
    29a1c2252:	add    %al,(%rax)
    29a1c2254:	add    %al,(%rax)
    29a1c2256:	add    %al,(%rax)
    29a1c2258:	add    %dh,0x1(%rbx)
    29a1c225b:	add    $0x3,%al
@@ -15476,20 +15426,17 @@
    29a1c227a:	add    %bl,(%rdx)
    29a1c227c:	or     %eax,(%rax)
    29a1c227e:	add    %bl,(%rax)
    29a1c2280:	or     %eax,(%rax)
    29a1c2282:	add    %dl,(%rdx)
    29a1c2284:	jg     29a1c229a <.debug_info+0x12af>
    29a1c2286:	add    %al,(%rax)
-   29a1c2288:	scas   %es:(%rdi),%al
-   29a1c2289:	sbb    (%rbx),%bl
-   29a1c228b:	(bad)
-   29a1c228c:	add    (%rax),%al
-   29a1c228e:	add    %al,(%rax)
-   29a1c2290:	add    0x29a1b1a(%rsi),%ebp
+   29a1c2288:	mov    (%rdx),%ds
+   29a1c228a:	sbb    0x2(%rdx),%ebx
+   29a1c2290:	add    0x29a1b1a(%rsi),%ecx
    29a1c2296:	add    %al,(%rax)
    29a1c2298:	add    %cl,(%rdx)
    29a1c229a:	add    %al,(%rax)
    29a1c229c:	add    %al,(%rax)
    29a1c229e:	add    %al,(%rax)
    29a1c22a0:	add    %al,(%rdi)
    29a1c22a2:	add    %eax,(%rcx)
@@ -15503,24 +15450,24 @@
    29a1c22bd:	add    %al,(%rbx)
    29a1c22bf:	xchg   %eax,%ebp
    29a1c22c0:	adc    $0x0,%al
    29a1c22c2:	add    %bh,(%rsi)
    29a1c22c4:	or     %eax,(%rax)
    29a1c22c6:	add    %bh,(%rcx,%rcx,1)
    29a1c22c9:	add    %al,(%rax)
-   29a1c22cb:	or     0x29a1b1a(%rsi),%esi
+   29a1c22cb:	or     0x29a1b1a(%rsi),%edx
    29a1c22d1:	add    %al,(%rax)
    29a1c22d3:	add    %dh,%bh
    29a1c22d5:	adc    $0x0,%al
    29a1c22d7:	add    %al,(%rcx,%rax,1)
    29a1c22da:	push   %rdx
    29a1c22db:	add    0x0(%rax,%rax,1),%dh
    29a1c22df:	add    %al,(%rax)
    29a1c22e1:	add    %al,(%rax)
-   29a1c22e3:	or     $0x9a1b1ad0,%eax
+   29a1c22e3:	or     $0x9a1b1ab0,%eax
    29a1c22e8:	add    (%rax),%al
    29a1c22ea:	add    %al,(%rax)
    29a1c22ec:	(bad)
    29a1c22ed:	(bad)
    29a1c22ee:	add    %al,(%rax)
    29a1c22f0:	(bad)
    29a1c22f1:	adc    (%rax),%eax
@@ -15528,29 +15475,28 @@
    29a1c22f6:	push   %rdx
    29a1c22f7:	or     %eax,(%rbx)
    29a1c22f9:	cmp    %al,0x1b(%rcx)
    29a1c22fc:	(bad)
    29a1c22fd:	add    (%rax),%al
    29a1c22ff:	add    %al,(%rax)
    29a1c2301:	add    %cl,(%rbx)
-   29a1c2303:	fstpl  (%rdx)
-   29a1c2305:	sbb    0x2(%rdx),%ebx
-   29a1c230b:	(bad)
-   29a1c230c:	(bad)
+   29a1c2303:	mov    $0x29a1b1a,%ebp
+   29a1c2308:	add    %al,(%rax)
+   29a1c230a:	add    %ah,0x16(%rax)
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
-   29a1c2320:	mov    $0x90000014,%ebx
+   29a1c2320:	mov    $0x70000014,%ebx
    29a1c2325:	sbb    %ebx,(%rbx)
    29a1c2327:	(bad)
    29a1c2328:	add    (%rax),%al
    29a1c232a:	add    %al,(%rax)
    29a1c232c:	pop    %rax
    29a1c232d:	add    %al,(%rax)
    29a1c232f:	add    %al,(%rax)
@@ -15564,24 +15510,24 @@
    29a1c233e:	adc    $0x0,%al
    29a1c2340:	add    %cl,0x9(%rdx)
    29a1c2343:	add    %al,(%rax)
    29a1c2345:	rex.RX or %r8d,(%rax)
    29a1c2348:	add    %bh,(%rdx)
    29a1c234a:	out    %eax,$0x14
    29a1c234c:	add    %al,(%rax)
-   29a1c234e:	add    -0x30f48054(%rcx),%edx
+   29a1c234e:	add    -0x50f48054(%rcx),%edx
    29a1c2354:	sbb    %ebx,(%rbx)
    29a1c2356:	(bad)
    29a1c2357:	add    (%rax),%al
    29a1c2359:	add    %al,(%rax)
    29a1c235b:	adc    $0x400000d,%eax
    29a1c2360:	add    %ebx,0x2(%rcx)
    29a1c2363:	jne    29a1c2365 <.debug_info+0x137a>
    29a1c2365:	add    %al,(%rax)
-   29a1c2367:	adc    $0xc7,%al
+   29a1c2367:	adc    $0xa7,%al
    29a1c2369:	(bad)
    29a1c236a:	sbb    0x2(%rdx),%ebx
    29a1c2370:	(bad)
    29a1c2371:	(bad)
    29a1c2372:	add    %al,(%rax)
    29a1c2374:	add    %ah,(%rbx)
    29a1c2376:	outsl  %fs:(%rsi),(%dx)
@@ -15728,16 +15674,16 @@
    29a1c24e8:	jae    29a1c254f <.debug_info+0x1564>
    29a1c24ea:	movsxd 0x6f(%rcx,%rbp,2),%esi
    29a1c24ee:	outsb  %ds:(%rsi),(%dx)
    29a1c24ef:	pop    %rdi
    29a1c24f0:	ja     29a1c2564 <.debug_info+0x1579>
    29a1c24f2:	imul   $0x100656c,0x62(%rcx,%riz,2),%esi
    29a1c24fa:	mov    $0x1,%bh
-   29a1c24fc:	adc    %dl,(%rsi)
-   29a1c24fe:	sbb    0x2(%rdx),%ebx
+   29a1c24fc:	lock adc $0x29a1b,%eax
+   29a1c2502:	add    %al,(%rax)
    29a1c2504:	(bad)
    29a1c2509:	add    %al,(%rax)
    29a1c250b:	add    %al,(%rcx)
    29a1c250d:	pushf
    29a1c250e:	(bad)
    29a1c250f:	(bad)
    29a1c2510:	add    %al,(%rax)
@@ -15762,15 +15708,15 @@
    29a1c253c:	movabs %al,0x1d00000996000009
    29a1c2545:	imul   $0x12507bb,(%rax),%eax
    29a1c254b:	add    %al,(%rax)
    29a1c254d:	rorl   %cl,(%rcx)
    29a1c254f:	add    %al,(%rax)
    29a1c2551:	int    $0x9
    29a1c2553:	add    %al,(%rax)
-   29a1c2555:	ds lock (bad)
+   29a1c2555:	ds rclb $1,(%rsi)
    29a1c2558:	sbb    0x2(%rdx),%ebx
    29a1c255e:	push   %rax
    29a1c255f:	add    %al,(%rax)
    29a1c2561:	add    %al,(%rax)
    29a1c2563:	add    %al,(%rax)
    29a1c2565:	add    %bl,%bl
    29a1c2567:	adc    $0x6e1d0000,%eax
@@ -15780,74 +15726,74 @@
    29a1c2572:	je     29a1c25d9 <.debug_info+0x15ee>
    29a1c2574:	movsxd -0x29(%rax,%rax,1),%esi
    29a1c2578:	or     $0x175,%eax
    29a1c257d:	in     (%dx),%al
    29a1c257e:	or     %eax,(%rax)
    29a1c2580:	add    %ch,%dl
    29a1c2582:	or     %eax,(%rax)
-   29a1c2584:	add    %cl,-0x65e4e8dc(%rip)        # 234373cae <__size_of_stack_reserve__+0x234173cae>
+   29a1c2584:	add    %cl,-0x65e4e8fc(%rip)        # 234373c8e <__size_of_stack_reserve__+0x234173c8e>
    29a1c258a:	add    (%rax),%al
    29a1c258c:	add    %al,(%rax)
    29a1c258e:	adc    $0xb200000d,%eax
    29a1c2593:	adc    $0x1040000,%eax
    29a1c2598:	pop    %rcx
    29a1c2599:	add    0x0(%rbx),%dh
-   29a1c259c:	add    %dl,(%rsi,%rbp,1)
+   29a1c259c:	add    %dl,(%rsi,%rcx,1)
    29a1c259f:	(bad)
    29a1c25a0:	sbb    0x2(%rdx),%ebx
-   29a1c25a6:	add    %cl,0x3c0b0000(%rip)        # 2d62725ac <.debug_rnglists+0x3c0a2508>
+   29a1c25a6:	add    %cl,0x1c0b0000(%rip)        # 2b62725ac <.debug_rnglists+0x1c0a2508>
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
-   29a1c25c6:	or     $0x9a1b1670,%eax
+   29a1c25c6:	or     $0x9a1b1650,%eax
    29a1c25cb:	add    (%rax),%al
    29a1c25cd:	add    %al,(%rax)
    29a1c25cf:	xchg   %cl,0x15f30000(%rip)        # 2b00f25d5 <.debug_rnglists+0x15f22531>
    29a1c25d5:	add    %al,(%rax)
    29a1c25d7:	add    $0x1,%al
    29a1c25d9:	push   %rdx
    29a1c25da:	add    0x0(%rbx),%dh
-   29a1c25dd:	add    %dl,0x29a1b16(,%rbx,4)
+   29a1c25dd:	add    %dl,0x29a1b16(,%rdi,2)
    29a1c25e4:	add    %al,(%rax)
    29a1c25e6:	add    %ch,0xd(%rsi)
    29a1c25e9:	add    %al,(%rax)
-   29a1c25eb:	or     $0x9a1b16c1,%eax
+   29a1c25eb:	or     $0x9a1b16a1,%eax
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
-   29a1c260a:	or     $0x9a1b1762,%eax
+   29a1c260a:	or     $0x9a1b1742,%eax
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
-   29a1c2629:	or     0x17(%rdx),%esi
+   29a1c2629:	or     0x17(%rdx),%edx
    29a1c262c:	sbb    0x2(%rdx),%ebx
    29a1c2632:	(bad)
    29a1c2633:	(bad)
    29a1c2634:	add    %al,(%rax)
    29a1c2636:	add    $0x1,%al
    29a1c2638:	push   %rdx
    29a1c2639:	or     %eax,(%rbx)
@@ -15864,15 +15810,15 @@
    29a1c264e:	jb     29a1c26b5 <.debug_info+0x16ca>
    29a1c2650:	jo     29a1c26c1 <.debug_info+0x16d6>
    29a1c2652:	jb     29a1c26c8 <.debug_info+0x16dd>
    29a1c2654:	pop    %rdi
    29a1c2655:	gs jb  29a1c26ca <.debug_info+0x16df>
    29a1c2658:	outsl  %ds:(%rsi),(%dx)
    29a1c2659:	jb     29a1c265b <.debug_info+0x1670>
-   29a1c265b:	add    %edx,-0x60(%rcx,%rax,1)
+   29a1c265b:	add    %edx,-0x80(%rcx,%rax,1)
    29a1c265f:	adc    $0x29a1b,%eax
    29a1c2664:	add    %al,(%rax)
    29a1c2666:	imul   $0x0,(%rax),%eax
    29a1c266c:	add    %al,(%rax)
    29a1c266e:	add    %ebx,0x26000017(%rdi,%rbp,1)
    29a1c2675:	insl   (%dx),%es:(%rdi)
    29a1c2676:	jae    29a1c26df <.debug_info+0x16f4>
@@ -15887,24 +15833,24 @@
    29a1c2689:	(bad)
    29a1c268a:	jb     29a1c26f3 <.debug_info+0x1708>
    29a1c268c:	jo     29a1c268e <.debug_info+0x16a3>
    29a1c268e:	xchg   %eax,%ebx
    29a1c268f:	or     0x2000000(%rbx),%esi
    29a1c2695:	xchg   %eax,%ecx
    29a1c2696:	pop    %rax
-   29a1c2697:	or     $0x9a1b15cc,%eax
+   29a1c2697:	or     $0x9a1b15ac,%eax
    29a1c269c:	add    (%rax),%al
    29a1c269e:	add    %al,(%rax)
    29a1c26a0:	sbb    $0xc300000e,%eax
    29a1c26a5:	(bad)
    29a1c26a6:	add    %al,(%rax)
    29a1c26a8:	add    $0x1,%al
    29a1c26aa:	push   %rdx
    29a1c26ab:	add    %esi,(%rdx)
-   29a1c26ad:	add    %cl,-0x65e4ea1a(%rip)        # 234373c99 <__size_of_stack_reserve__+0x234173c99>
+   29a1c26ad:	add    %cl,-0x65e4ea3a(%rip)        # 234373c79 <__size_of_stack_reserve__+0x234173c79>
    29a1c26b3:	add    (%rax),%al
    29a1c26b5:	add    %al,(%rax)
    29a1c26b7:	(bad)
    29a1c26b8:	(bad)
    29a1c26b9:	add    %al,(%rax)
    29a1c26bb:	in     (%dx),%al
    29a1c26bc:	(bad)
@@ -15916,39 +15862,39 @@
    29a1c26c5:	rex sbb 0x2(%rdx),%ebx
    29a1c26cc:	add    $0x1,%al
    29a1c26ce:	push   %rcx
    29a1c26cf:	add    %esi,(%rcx)
    29a1c26d1:	add    $0x1,%al
    29a1c26d3:	pop    %rax
    29a1c26d4:	add    %ecx,0x0(%rbx)
-   29a1c26d7:	or     $0x9a1b15f5,%eax
+   29a1c26d7:	or     $0x9a1b15d5,%eax
    29a1c26dc:	add    (%rax),%al
    29a1c26de:	add    %al,(%rax)
    29a1c26e0:	sbb    $0x300000e,%eax
    29a1c26e5:	(bad)
    29a1c26e6:	add    %al,(%rax)
    29a1c26e8:	add    $0x1,%al
    29a1c26ea:	push   %rdx
    29a1c26eb:	add    %esi,(%rdx)
-   29a1c26ed:	add    %cl,-0x65e4e9fd(%rip)        # 234373cf6 <__size_of_stack_reserve__+0x234173cf6>
+   29a1c26ed:	add    %cl,-0x65e4ea1d(%rip)        # 234373cd6 <__size_of_stack_reserve__+0x234173cd6>
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
-   29a1c270c:	adc    $0x9,%al
-   29a1c270e:	(bad)
-   29a1c270f:	sbb    0x2(%rdx),%ebx
+   29a1c270c:	adc    $0xe9,%al
+   29a1c270e:	adc    $0x29a1b,%eax
+   29a1c2713:	add    %al,(%rax)
    29a1c2715:	fmuls  0x41000000(%rip)        # 2db1c271b <.debug_rnglists+0x40ff2677>
    29a1c271b:	data16 ja 29a1c2790 <.debug_info+0x5a>
    29a1c271e:	imul   $0x75625f5f,0x0(%rbp,%riz,2),%esi
    29a1c2726:	imul   $0x77665f6e,0x69(%rsp,%rsi,2),%ebp
    29a1c272e:	jb     29a1c2799 <.debug_info+0x63>
    29a1c2730:	je     29a1c2797 <.debug_info+0x61>
    29a1c2732:	add    %cl,(%rsi)
@@ -15984,16 +15930,18 @@
    29a1c278c:	jne    29a1c27c7 <.debug_info+0x91>
    29a1c278e:	cmp    %eax,(%rax)
    29a1c2790:	or     $0x22,%al
    29a1c2792:	(bad)
    29a1c2793:	add    %al,(%rax)
    29a1c2795:	or     (%rdi),%al
    29a1c2797:	add    %al,(%rax)
-   29a1c2799:	loopne 29a1c27b5 <.debug_info+0x7f>
-   29a1c279b:	sbb    0x2(%rdx),%ebx
+   29a1c2799:	rcrb   $0x1b,(%rdx)
+   29a1c279c:	(bad)
+   29a1c279d:	add    (%rax),%al
+   29a1c279f:	add    %al,(%rax)
    29a1c27a1:	(bad)
    29a1c27a6:	add    %al,(%rax)
    29a1c27a8:	add    %al,(%rsp,%rcx,1)
    29a1c27ab:	add    %al,(%rax)
    29a1c27ad:	add    (%rcx),%al
    29a1c27af:	(bad)
    29a1c27b0:	movsxd 0x61(%rax),%ebp
@@ -16780,16 +16728,19 @@
    29a1c2e3a:	imul   $0x4c545f77,0x67(%rsi),%ebp
    29a1c2e41:	push   %rbx
    29a1c2e42:	movsxd 0x6c(%rcx),%esp
    29a1c2e45:	insb   (%dx),%es:(%rdi)
    29a1c2e46:	(bad)
    29a1c2e4b:	jp     29a1c2e6c <.debug_info+0x736>
    29a1c2e4d:	add    %eax,(%rax)
-   29a1c2e4f:	add    %dl,0x1c(%rax)
-   29a1c2e52:	sbb    0x2(%rdx),%ebx
+   29a1c2e4f:	add    %dh,(%rax)
+   29a1c2e51:	sbb    $0x1b,%al
+   29a1c2e53:	(bad)
+   29a1c2e54:	add    (%rax),%al
+   29a1c2e56:	add    %al,(%rax)
    29a1c2e58:	repnz add %al,(%rax)
    29a1c2e5b:	add    %al,(%rax)
    29a1c2e5d:	add    %al,(%rax)
    29a1c2e5f:	add    %al,(%rcx)
    29a1c2e61:	pushf
    29a1c2e62:	outsb  %ds:(%rsi),(%dx)
    29a1c2e63:	or     %al,(%rax)
@@ -16820,15 +16771,16 @@
    29a1c2e99:	jae    29a1c2f00 <.debug_info+0x7ca>
    29a1c2e9b:	jb     29a1c2f13 <.debug_info+0x7dd>
    29a1c2e9d:	gs add %bh,%fs:0x53(%rdi,%rcx,1)
    29a1c2ea3:	add    %eax,(%rax)
    29a1c2ea5:	add    %ah,0xd00000b(%rip)        # 2a71c2eb6 <.debug_rnglists+0xcff2e12>
    29a1c2eab:	or     (%rax),%eax
    29a1c2ead:	add    %ah,(%rax)
-   29a1c2eaf:	(bad)
+   29a1c2eaf:	movsl  %ds:(%rsi),%es:(%rdi)
+   29a1c2eb0:	sbb    $0x1b,%al
    29a1c2eb2:	(bad)
    29a1c2eb3:	add    (%rax),%al
    29a1c2eb5:	add    %al,(%rax)
    29a1c2eb7:	rex.WXB add %al,(%r8)
    29a1c2eba:	add    %al,(%rax)
    29a1c2ebc:	add    %al,(%rax)
    29a1c2ebe:	add    %bl,%bl
@@ -16841,80 +16793,80 @@
    29a1c2ed4:	or     (%rax),%eax
    29a1c2ed6:	add    %cl,(%rdx)
    29a1c2ed8:	je     29a1c2eda <.debug_info+0x7a4>
    29a1c2eda:	mov    %ebp,0x5de(%rip)        # 29a1c34be <.debug_info+0x15c>
    29a1c2ee0:	stos   %al,%es:(%rdi)
    29a1c2ee1:	or     (%rax),%eax
    29a1c2ee3:	add    %ch,0x600000b(%rax)
-   29a1c2ee9:	in     $0x1c,%al
-   29a1c2eeb:	sbb    0x2(%rdx),%ebx
+   29a1c2ee9:	(bad)
+   29a1c2eea:	sbb    $0x1b,%al
+   29a1c2eec:	(bad)
+   29a1c2eed:	add    (%rax),%al
+   29a1c2eef:	add    %al,(%rax)
    29a1c2ef1:	mov    (%rsi),%eax
    29a1c2ef3:	add    %al,(%rax)
-   29a1c2ef5:	or     $0x9a1b1d0b,%eax
+   29a1c2ef5:	or     $0x9a1b1ceb,%eax
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
-   29a1c2f15:	add    %dl,0x29a1b1c(%rbp)
-   29a1c2f1b:	add    %al,(%rax)
-   29a1c2f1d:	add    %al,(%rcx)
-   29a1c2f1f:	xchg   %eax,%ebp
-   29a1c2f20:	sbb    $0x1b,%al
-   29a1c2f22:	(bad)
-   29a1c2f23:	add    (%rax),%al
-   29a1c2f25:	add    %al,(%rax)
+   29a1c2f15:	add    %dh,0x1c(%rbp)
+   29a1c2f18:	sbb    0x2(%rdx),%ebx
+   29a1c2f1e:	add    %esi,0x1c(%rbp)
+   29a1c2f21:	sbb    0x2(%rdx),%ebx
    29a1c2f27:	sbb    (%rax),%eax
    29a1c2f29:	add    %al,(%rax)
    29a1c2f2b:	add    %al,(%rax)
    29a1c2f2d:	add    %al,(%rax)
    29a1c2f2f:	add    %ebx,0x81307(%rcx)
    29a1c2f35:	add    %dl,0x890(%rip)        # 29a1c37cb <.debug_info+0x469>
    29a1c2f3b:	(bad)
-   29a1c2f3c:	movsb  %ds:(%rsi),%es:(%rdi)
-   29a1c2f3d:	sbb    $0x1b,%al
+   29a1c2f3c:	test   %bl,(%rbx,%rbx,1)
    29a1c2f3f:	(bad)
    29a1c2f40:	add    (%rax),%al
    29a1c2f42:	add    %al,(%rax)
    29a1c2f44:	sub    %ecx,(%rdx)
    29a1c2f46:	add    %al,(%rax)
    29a1c2f48:	add    %ah,(%rdx)
    29a1c2f4a:	outsb  %ds:(%rsi),(%dx)
    29a1c2f4b:	or     %al,(%rax)
-   29a1c2f4d:	add    %dh,0x29a1b1c(%rax)
+   29a1c2f4d:	add    %dl,0x29a1b1c(%rax)
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
-   29a1c2f6d:	and    $0x29a1b1d,%eax
+   29a1c2f6d:	add    $0x29a1b1d,%eax
    29a1c2f72:	add    %al,(%rax)
    29a1c2f74:	add    %ch,(%rcx)
    29a1c2f76:	or     (%rax),%al
    29a1c2f78:	add    %al,(%rax)
    29a1c2f7a:	add    %al,(%rsi)
-   29a1c2f7c:	adc    $0x29a1b1d,%eax
-   29a1c2f81:	add    %al,(%rax)
-   29a1c2f83:	add    %dh,(%rsi)
-   29a1c2f85:	(bad)
+   29a1c2f7c:	cmc
+   29a1c2f7d:	sbb    $0x1b,%al
+   29a1c2f7f:	(bad)
+   29a1c2f80:	add    (%rax),%al
+   29a1c2f82:	add    %al,(%rax)
+   29a1c2f84:	ss (bad)
    29a1c2f86:	add    %al,(%rax)
-   29a1c2f88:	or     $0x9a1b1d3d,%eax
+   29a1c2f88:	or     $0x9a1b1d1d,%eax
    29a1c2f8d:	add    (%rax),%al
    29a1c2f8f:	add    %al,(%rax)
    29a1c2f91:	gs (bad)
    29a1c2f93:	add    %al,(%rax)
    29a1c2f95:	add    (%rcx),%eax
    29a1c2f97:	push   %rdx
    29a1c2f98:	or     %eax,(%rbx)
@@ -16958,22 +16910,22 @@
    29a1c2ff7:	jbe    29a1c305e <.debug_info+0x928>
    29a1c2ff9:	pop    %rdi
    29a1c2ffa:	imul   $0x5f,0x79(%rbp),%esp
    29a1c2ffe:	fs je  29a1c3070 <.debug_info+0x93a>
    29a1c3001:	jb     29a1c3003 <.debug_info+0x8cd>
    29a1c3003:	rex.B iret
    29a1c3005:	add    %al,(%rax)
-   29a1c3007:	add    %al,%al
-   29a1c3009:	sbb    (%rbx),%ebx
-   29a1c300b:	(bad)
-   29a1c300c:	add    (%rax),%al
-   29a1c300e:	add    %al,(%rax)
-   29a1c3010:	addl   $0x0,(%rax)
-   29a1c3016:	add    %al,(%rax)
-   29a1c3018:	add    %ebx,0x9000009(%rsp,%riz,2)
+   29a1c3007:	add    %ah,0x29a1b1b(%rax)
+   29a1c300d:	add    %al,(%rax)
+   29a1c300f:	add    %al,0x0(%rcx)
+   29a1c3015:	add    %al,(%rax)
+   29a1c3017:	add    %al,(%rcx)
+   29a1c3019:	pushf
+   29a1c301a:	or     %eax,%fs:(%rax)
+   29a1c301d:	add    %cl,(%rcx)
    29a1c301f:	imul   $0x0,0x79(%rbp),%esp
    29a1c3023:	sub    %dil,(%r9,%rax,1)
    29a1c3027:	add    %al,(%rax)
    29a1c3029:	mov    $0xb200000b,%edx
    29a1c302e:	or     (%rax),%eax
    29a1c3030:	add    %cl,(%rdx)
    29a1c3032:	jo     29a1c30a6 <.debug_info+0x970>
@@ -16986,33 +16938,33 @@
    29a1c3047:	add    %al,(%rax)
    29a1c3049:	or     0x75(%rbx),%ah
    29a1c304c:	jb     29a1c30ad <.debug_info+0x977>
    29a1c304e:	imul   $0x0,0x79(%rbp),%esp
    29a1c3052:	rex.R (bad)
    29a1c3054:	fiadds 0xbff0000(%rip)        # 2a61b305a <.debug_rnglists+0xbfe2fb6>
    29a1c305a:	add    %al,(%rax)
-   29a1c305c:	testl  $0xf00e0000,(%rbx)
+   29a1c305c:	testl  $0xd00e0000,(%rbx)
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
-   29a1c3079:	and    (%rbx,%rbx,1),%ebx
+   29a1c3079:	add    (%rbx,%rbx,1),%ebx
    29a1c307c:	(bad)
    29a1c307d:	add    (%rax),%al
    29a1c307f:	add    %al,(%rax)
    29a1c3081:	mov    (%rsi),%eax
    29a1c3083:	add    %al,(%rax)
-   29a1c3085:	or     $0x9a1b1c2c,%eax
+   29a1c3085:	or     $0x9a1b1c0c,%eax
    29a1c308a:	add    (%rax),%al
    29a1c308c:	add    %al,(%rax)
    29a1c308e:	lahf
    29a1c308f:	(bad)
    29a1c3090:	add    %al,(%rax)
    29a1c3092:	add    (%rcx),%eax
    29a1c3094:	push   %rdx
@@ -17029,16 +16981,19 @@
    29a1c30ab:	(bad)
    29a1c30ac:	fs fs pop %rdi
    29a1c30af:	imul   $0x5f,0x79(%rbp),%esp
    29a1c30b3:	fs je  29a1c3125 <.debug_info+0x9ef>
    29a1c30b6:	jb     29a1c30b8 <.debug_info+0x982>
    29a1c30b8:	sub    %bh,%cl
    29a1c30ba:	add    %al,(%rax)
-   29a1c30bc:	add    %dl,0x1b(%rax)
-   29a1c30bf:	sbb    0x2(%rdx),%ebx
+   29a1c30bc:	add    %dh,(%rax)
+   29a1c30be:	sbb    (%rbx),%ebx
+   29a1c30c0:	(bad)
+   29a1c30c1:	add    (%rax),%al
+   29a1c30c3:	add    %al,(%rax)
    29a1c30c5:	outsl  %ds:(%rsi),(%dx)
    29a1c30c6:	add    %al,(%rax)
    29a1c30c8:	add    %al,(%rax)
    29a1c30ca:	add    %al,(%rax)
    29a1c30cc:	add    %al,(%rcx)
    29a1c30ce:	pushf
    29a1c30cf:	and    $0xa,%al
@@ -17061,110 +17016,107 @@
    29a1c30ff:	imul   $0x0,0x79(%rbp),%esp
    29a1c3103:	sub    $0x15,%al
    29a1c3105:	and    $0xa,%al
    29a1c3107:	add    %al,(%rax)
    29a1c3109:	(bad)
    29a1c310a:	or     $0x0,%al
    29a1c310c:	add    %dl,0xe00000c(%rdx)
-   29a1c3112:	jg     29a1c312f <.debug_info+0x9f9>
-   29a1c3114:	sbb    0x2(%rdx),%ebx
+   29a1c3112:	pop    %rdi
+   29a1c3113:	sbb    (%rbx),%ebx
+   29a1c3115:	(bad)
+   29a1c3116:	add    (%rax),%al
+   29a1c3118:	add    %al,(%rax)
    29a1c311a:	loope  29a1c3122 <.debug_info+0x9ec>
    29a1c311c:	add    %al,(%rax)
    29a1c311e:	testl  $0x1030000,(%rcx)
    29a1c3124:	push   %rdx
    29a1c3125:	add    %esi,(%rcx)
    29a1c3127:	add    (%rcx),%eax
    29a1c3129:	push   %rcx
    29a1c312a:	add    %ecx,0x0(%rax)
    29a1c312d:	(bad)
-   29a1c312e:	popf
-   29a1c312f:	sbb    (%rbx),%ebx
-   29a1c3131:	(bad)
-   29a1c3132:	add    (%rax),%al
-   29a1c3134:	add    %al,(%rax)
+   29a1c312e:	jge    29a1c314b <.debug_info+0xa15>
+   29a1c3130:	sbb    0x2(%rdx),%ebx
    29a1c3136:	rolb   $0x0,(%rsi)
    29a1c3139:	add    %cl,(%rdi)
    29a1c313b:	or     (%rax),%al
    29a1c313d:	add    %al,(%rbx)
    29a1c313f:	add    %edx,0x2(%rdx)
    29a1c3142:	je     29a1c3144 <.debug_info+0xa0e>
-   29a1c3144:	add    %cl,-0x65e4e448(%rip)        # 234374d02 <__size_of_stack_reserve__+0x234174d02>
+   29a1c3144:	add    %cl,-0x65e4e468(%rip)        # 234374ce2 <__size_of_stack_reserve__+0x234174ce2>
    29a1c314a:	add    (%rax),%al
    29a1c314c:	add    %al,(%rax)
    29a1c314e:	lahf
    29a1c314f:	(bad)
    29a1c3150:	add    %al,(%rax)
    29a1c3152:	add    (%rcx),%eax
    29a1c3154:	push   %rdx
    29a1c3155:	add    0x0(%rax,%rax,1),%dh
    29a1c3159:	add    %cl,(%rax)
-   29a1c315b:	addl   $0xe0000008,0x6e260000(%rip)        # 308423165 <.debug_rnglists+0x6e2530c1>
+   29a1c315b:	addl   $0xc0000008,0x6e260000(%rip)        # 308423165 <.debug_rnglists+0x6e2530c1>
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
-   29a1c3187:	add    %bl,(%rax)
-   29a1c3189:	sbb    (%rbx),%ebx
+   29a1c3187:	add    %bh,%al
+   29a1c3189:	sbb    (%rbx),%bl
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
-   29a1c31aa:	sbb    $0x1b,%al
-   29a1c31ac:	sbb    0x2(%rdx),%ebx
+   29a1c31aa:	cld
+   29a1c31ab:	sbb    (%rbx),%bl
+   29a1c31ad:	(bad)
+   29a1c31ae:	add    (%rax),%al
+   29a1c31b0:	add    %al,(%rax)
    29a1c31b2:	(bad)
    29a1c31b3:	(bad)
    29a1c31b4:	add    %al,(%rax)
    29a1c31b6:	(bad)
-   29a1c31b7:	and    %ebx,(%rbx)
+   29a1c31b7:	add    %ebx,(%rbx)
    29a1c31b9:	sbb    0x2(%rdx),%ebx
    29a1c31bf:	add    (%rsi),%al
    29a1c31c1:	add    %al,(%rax)
-   29a1c31c3:	sub    %dh,(%rbx)
+   29a1c31c3:	sub    %dl,(%rbx)
    29a1c31c5:	sbb    (%rbx),%ebx
    29a1c31c7:	(bad)
    29a1c31c8:	add    (%rax),%al
    29a1c31ca:	add    %al,(%rax)
    29a1c31cc:	add    (%rcx),%eax
    29a1c31ce:	push   %rdx
    29a1c31cf:	add    0x0(%rax,%rax,1),%dh
    29a1c31d3:	add    %cl,(%rsi)
-   29a1c31d5:	cli
-   29a1c31d6:	sbb    (%rbx),%bl
-   29a1c31d8:	(bad)
-   29a1c31d9:	add    (%rax),%al
-   29a1c31db:	add    %al,(%rax)
+   29a1c31d5:	ficompl (%rdx)
+   29a1c31d7:	sbb    0x2(%rdx),%ebx
    29a1c31dd:	rolb   $0x0,(%rsi)
    29a1c31e0:	add    %dh,0x300000a(%rsi)
    29a1c31e6:	add    %edx,0x2(%rdx)
    29a1c31e9:	jl     29a1c31eb <.debug_info+0xab5>
    29a1c31eb:	add    %ch,(%rcx)
-   29a1c31ed:	push   %rax
-   29a1c31ee:	sbb    (%rbx),%ebx
-   29a1c31f0:	(bad)
-   29a1c31f1:	add    (%rax),%al
-   29a1c31f3:	add    %al,(%rax)
+   29a1c31ed:	xor    %bl,(%rbx)
+   29a1c31ef:	sbb    0x2(%rdx),%ebx
    29a1c31f5:	lahf
    29a1c31f6:	(bad)
    29a1c31f7:	add    %al,(%rax)
    29a1c31f9:	add    (%rcx),%eax
    29a1c31fb:	push   %rdx
    29a1c31fc:	or     %eax,(%rbx)
    29a1c31fe:	movabs 0x29a1b70,%al
@@ -17355,15 +17307,15 @@
    29a1c33af:	xor    (%rax),%ah
    29a1c33b1:	sub    $0x3d647473,%eax
    29a1c33b6:	outsb  %ds:(%esi),(%dx)
    29a1c33b8:	jne    29a1c33f3 <.debug_info+0x91>
    29a1c33ba:	cmp    %eax,(%rax)
    29a1c33bc:	or     $0x9d,%al
    29a1c33be:	or     %eax,(%rax)
-   29a1c33c0:	add    %al,0x50000009(%rbp)
+   29a1c33c0:	add    %al,0x30000009(%rbp)
    29a1c33c6:	sbb    $0x29a1b,%eax
    29a1c33cb:	add    %al,(%rax)
    29a1c33cd:	testb  $0x0,(%rbx)
    29a1c33d0:	add    %al,(%rax)
    29a1c33d2:	add    %al,(%rax)
    29a1c33d4:	add    %dh,%al
    29a1c33d6:	(bad)
@@ -18645,18 +18597,17 @@
    29a1c3f32:	imul   $0x5f797261,0x72(%rdx),%esp
    29a1c3f39:	outsb  %ds:(%rsi),(%dx)
    29a1c3f3a:	(bad)
    29a1c3f3b:	insl   (%dx),%es:(%rdi)
    29a1c3f3c:	gs jae 29a1c3f3f <.debug_info+0xbdd>
    29a1c3f3f:	mov    $0x9d,%bh
    29a1c3f41:	or     (%rax),%eax
-   29a1c3f43:	add    %al,0x29a1b20(%rax)
-   29a1c3f49:	add    %al,(%rax)
-   29a1c3f4b:	add    %al,%dh
-   29a1c3f4d:	add    %al,(%rax)
+   29a1c3f43:	add    %ah,0x20(%rax)
+   29a1c3f46:	sbb    0x2(%rdx),%ebx
+   29a1c3f4c:	movb   $0x0,(%rax)
    29a1c3f4f:	add    %al,(%rax)
    29a1c3f51:	add    %al,(%rax)
    29a1c3f53:	add    %al,(%rcx)
    29a1c3f55:	pushf
    29a1c3f56:	(bad)
    29a1c3f57:	or     $0x69110000,%eax
    29a1c3f5c:	add    %dh,0xd428(%rdi)
@@ -18696,19 +18647,17 @@
    29a1c3fbd:	add    %dil,0x14909(%r13)
    29a1c3fc4:	add    %bl,(%rdi)
    29a1c3fc6:	or     $0xd170000,%eax
    29a1c3fcb:	add    %al,(%rax)
    29a1c3fcd:	(bad)
    29a1c3fce:	lahf
    29a1c3fcf:	adc    (%rax),%eax
-   29a1c3fd1:	add    %al,0x29a1b20(%rax)
-   29a1c3fd7:	add    %al,(%rax)
-   29a1c3fd9:	add    %cl,(%rcx)
-   29a1c3fdb:	push   %rsp
-   29a1c3fdc:	add    %eax,(%rax)
+   29a1c3fd1:	add    %ah,0x20(%rax)
+   29a1c3fd4:	sbb    0x2(%rdx),%ebx
+   29a1c3fda:	or     %edx,0x0(%rcx,%rax,1)
    29a1c3fde:	add    %al,%al
    29a1c3fe0:	fmull  (%rax,%rax,1)
    29a1c3fe3:	add    %al,(%rsp,%rdi,4)
    29a1c3fe6:	adc    (%rax),%eax
    29a1c3fe8:	add    %al,(%rsi)
    29a1c3fea:	push   %rsp
    29a1c3feb:	add    %eax,(%rax)
@@ -18719,18 +18668,17 @@
    29a1c3ff4:	fsts   (%rbx)
    29a1c3ff6:	add    %al,(%rax)
    29a1c3ff8:	add    %ah,%ah
    29a1c3ffa:	adc    (%rax),%eax
    29a1c3ffc:	add    %cl,(%rcx)
    29a1c3ffe:	lahf
    29a1c3fff:	adc    (%rax),%eax
-   29a1c4001:	add    %dl,0x29a1b20(%rdx)
-   29a1c4007:	add    %al,(%rax)
-   29a1c4009:	add    %al,(%rax)
-   29a1c400b:	add    %eax,%fs:(%rax)
+   29a1c4001:	add    %dh,0x20(%rdx)
+   29a1c4004:	sbb    0x2(%rdx),%ebx
+   29a1c400a:	add    %ah,0x0(%rcx,%rax,1)
    29a1c400e:	add    %cl,(%rdi)
    29a1c4010:	add    %eax,(%rsp,%rdi,4)
    29a1c4013:	adc    (%rax),%eax
    29a1c4015:	add    %al,(%rsi)
    29a1c4017:	add    %eax,%fs:(%rax)
    29a1c401a:	add    %al,(%rdx)
    29a1c401c:	(bad)
@@ -18746,23 +18694,20 @@
    29a1c4031:	add    %ch,0xd(%rdi)
    29a1c4034:	add    %al,(%rax)
    29a1c4036:	insl   (%dx),%es:(%rdi)
    29a1c4037:	or     $0x0,%eax
    29a1c403c:	add    %al,(%rax)
    29a1c403e:	sbb    %ecx,0x13(%rbp)
    29a1c4041:	add    %al,(%rax)
-   29a1c4043:	(bad)
+   29a1c4043:	movsb  %ds:(%rsi),%es:(%rdi)
    29a1c4044:	and    %bl,(%rbx)
    29a1c4046:	(bad)
    29a1c4047:	add    (%rax),%al
    29a1c4049:	add    %al,(%rax)
-   29a1c404b:	add    %eax,%esp
-   29a1c404d:	and    %bl,(%rbx)
-   29a1c404f:	(bad)
-   29a1c4050:	add    (%rax),%al
+   29a1c404b:	add    %esp,0x29a1b(%rax,%riz,1)
    29a1c4052:	add    %al,(%rax)
    29a1c4054:	rex.WX add %al,(%rax)
    29a1c4057:	add    %al,(%rax)
    29a1c4059:	add    %al,(%rax)
    29a1c405b:	add    %cl,%cl
    29a1c405d:	(bad)
    29a1c405e:	adc    %dh,0x13(%rcx)
@@ -18793,15 +18738,15 @@
    29a1c40aa:	rex.XB jne 29a1c411f <.debug_info+0xdbd>
    29a1c40ad:	jb     29a1c4114 <.debug_info+0xdb2>
    29a1c40af:	outsb  %ds:(%rsi),(%dx)
    29a1c40b0:	je     29a1c40fb <.debug_info+0xd99>
    29a1c40b2:	insl   (%dx),%es:(%rdi)
    29a1c40b3:	(bad)
    29a1c40b4:	add    %ah,%gs:0x11f(%ebx)
-   29a1c40bc:	lock (bad)
+   29a1c40bc:	rcrb   $1,(%rdi)
    29a1c40be:	sbb    0x2(%rdx),%ebx
    29a1c40c4:	mov    %eax,(%rax)
    29a1c40c6:	add    %al,(%rax)
    29a1c40c8:	add    %al,(%rax)
    29a1c40ca:	add    %al,(%rax)
    29a1c40cc:	add    %ebx,0x1100000e(%rdx,%rcx,4)
    29a1c40d3:	jo     29a1c4129 <.debug_info+0xdc7>
@@ -18828,15 +18773,15 @@
    29a1c4118:	add    (%rsi),%ecx
    29a1c411a:	add    %al,(%rax)
    29a1c411c:	add    %ecx,(%rsi)
    29a1c411e:	add    %al,(%rax)
    29a1c4120:	(bad)
    29a1c4121:	lahf
    29a1c4122:	adc    (%rax),%eax
-   29a1c4124:	add    %dh,%al
+   29a1c4124:	add    %dl,%al
    29a1c4126:	(bad)
    29a1c4127:	sbb    0x2(%rdx),%ebx
    29a1c412d:	(bad)
    29a1c412e:	cmp    %eax,(%rcx)
    29a1c4130:	add    %al,(%rax)
    29a1c4132:	stos   %al,%es:(%rdi)
    29a1c4133:	(bad)
@@ -18853,19 +18798,17 @@
    29a1c4147:	fsts   (%rbx)
    29a1c4149:	add    %al,(%rax)
    29a1c414b:	add    %ah,%ah
    29a1c414d:	adc    (%rax),%eax
    29a1c414f:	add    %cl,(%rcx)
    29a1c4151:	lahf
    29a1c4152:	adc    (%rax),%eax
-   29a1c4154:	add    %al,(%rax)
-   29a1c4156:	and    %bl,(%rbx)
-   29a1c4158:	(bad)
-   29a1c4159:	add    (%rax),%al
-   29a1c415b:	add    %al,(%rax)
+   29a1c4154:	add    %ah,%al
+   29a1c4156:	(bad)
+   29a1c4157:	sbb    0x2(%rdx),%ebx
    29a1c415d:	add    %cl,0x1(%rcx)
    29a1c4160:	add    %al,(%rax)
    29a1c4162:	sgdt   (%rsp,%rdi,4)
    29a1c4166:	adc    (%rax),%eax
    29a1c4168:	add    %al,(%rsi)
    29a1c416a:	add    %rax,(%r8)
    29a1c416d:	add    %al,(%rdx)
@@ -18886,17 +18829,17 @@
    29a1c4189:	(bad)
    29a1c418a:	(bad)
    29a1c418b:	add    %al,(%rax)
    29a1c418d:	add    %al,(%rax)
    29a1c418f:	add    %al,(%rax)
    29a1c4191:	sbb    %ecx,0x13(%rbp)
    29a1c4194:	add    %al,(%rax)
-   29a1c4196:	and    $0x20,%al
+   29a1c4196:	add    $0x20,%al
    29a1c4198:	sbb    0x2(%rdx),%ebx
-   29a1c419e:	add    %esp,(%rax,%riz,1)
+   29a1c419e:	add    %eax,(%rax,%riz,1)
    29a1c41a1:	sbb    0x2(%rdx),%ebx
    29a1c41a7:	rex.WB add %al,(%r8)
    29a1c41aa:	add    %al,(%rax)
    29a1c41ac:	add    %al,(%rax)
    29a1c41ae:	add    %ch,0x1371100e(%rbp)
    29a1c41b4:	add    %al,(%rax)
    29a1c41b6:	sub    $0xe,%al
@@ -18927,30 +18870,31 @@
    29a1c41f1:	push   %rax
    29a1c41f2:	rex.RB
    29a1c41f3:	rex.WB insl (%dx),%es:(%rdi)
    29a1c41f5:	(bad)
    29a1c41f6:	addr32 gs rex.X (bad)
    29a1c41fa:	jae    29a1c4261 <.debug_info+0xeff>
    29a1c41fc:	add    %dl,0x160(%rdi)
-   29a1c4202:	mov    $0x1f,%al
+   29a1c4202:	nop
+   29a1c4203:	(bad)
    29a1c4204:	sbb    0x2(%rdx),%ebx
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
-   29a1c4227:	add    %dh,0x29a1b1f(%rax)
+   29a1c4227:	add    %dl,0x29a1b1f(%rax)
    29a1c422d:	add    %al,(%rax)
    29a1c422f:	add    %al,(%rsi,%rbx,1)
    29a1c4232:	add    %eax,(%rax)
    29a1c4234:	add    %bl,0x13bc0409(%rbx)
    29a1c423a:	add    %al,(%rax)
    29a1c423c:	(bad)
    29a1c423d:	(bad)
@@ -18962,19 +18906,18 @@
    29a1c4247:	fsts   (%rbx)
    29a1c4249:	add    %al,(%rax)
    29a1c424b:	add    %ah,%ah
    29a1c424d:	adc    (%rax),%eax
    29a1c424f:	add    %cl,(%rcx)
    29a1c4251:	lahf
    29a1c4252:	adc    (%rax),%eax
-   29a1c4254:	add    %al,%al
-   29a1c4256:	(bad)
-   29a1c4257:	sbb    0x2(%rdx),%ebx
-   29a1c425d:	add    %ch,(%rsi)
-   29a1c425f:	add    %eax,(%rax)
+   29a1c4254:	add    %ah,0x29a1b1f(%rax)
+   29a1c425a:	add    %al,(%rax)
+   29a1c425c:	add    %al,(%rax)
+   29a1c425e:	cs add %eax,(%rax)
    29a1c4261:	add    %cl,(%rdi)
    29a1c4263:	add    %eax,(%rsp,%rdi,4)
    29a1c4266:	adc    (%rax),%eax
    29a1c4268:	add    %al,(%rsi)
    29a1c426a:	cs add %eax,(%rax)
    29a1c426d:	add    %al,(%rdx)
    29a1c426f:	(bad)
@@ -19001,15 +18944,15 @@
    29a1c4299:	rex.RB push %r11
    29a1c429b:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
    29a1c42a0:	outsb  %ds:(%rsi),(%dx)
    29a1c42a1:	rex.RB js 29a1c4309 <.debug_info+0xfa7>
    29a1c42a4:	movsxd (%rax),%eax
    29a1c42a6:	jns    29a1c4306 <.debug_info+0xfa4>
    29a1c42a8:	or     (%rax),%al
-   29a1c42aa:	add    %dh,(%rax)
+   29a1c42aa:	add    %dl,(%rax)
    29a1c42ac:	(bad)
    29a1c42ad:	sbb    0x2(%rdx),%ebx
    29a1c42b3:	jae    29a1c42b5 <.debug_info+0xf53>
    29a1c42b5:	add    %al,(%rax)
    29a1c42b7:	add    %al,(%rax)
    29a1c42b9:	add    %al,(%rax)
    29a1c42bb:	add    %ebx,0x11000010(%rbp,%riz,1)
@@ -19051,15 +18994,15 @@
    29a1c430e:	add    %al,(%rax)
    29a1c4310:	fwait
    29a1c4311:	(bad)
    29a1c4312:	add    %al,(%rax)
    29a1c4314:	cltd
    29a1c4315:	(bad)
    29a1c4316:	add    %al,(%rax)
-   29a1c4318:	or     %ebx,0x30000013(%rdi)
+   29a1c4318:	or     %ebx,0x10000013(%rdi)
    29a1c431e:	(bad)
    29a1c431f:	sbb    0x2(%rdx),%ebx
    29a1c4325:	or     %al,(%rbx)
    29a1c4327:	add    %eax,(%rax)
    29a1c4329:	add    %al,0x13bc0409(%rcx)
    29a1c432f:	add    %al,(%rax)
    29a1c4331:	(bad)
@@ -19071,15 +19014,16 @@
    29a1c433c:	fsts   (%rbx)
    29a1c433e:	add    %al,(%rax)
    29a1c4340:	add    %ah,%ah
    29a1c4342:	adc    (%rax),%eax
    29a1c4344:	add    %cl,(%rcx)
    29a1c4346:	lahf
    29a1c4347:	adc    (%rax),%eax
-   29a1c4349:	add    %al,0x1f(%rcx)
+   29a1c4349:	add    %ah,(%rcx)
+   29a1c434b:	(bad)
    29a1c434c:	sbb    0x2(%rdx),%ebx
    29a1c4352:	add    %dl,(%rbx)
    29a1c4354:	add    %eax,(%rax)
    29a1c4356:	add    %cl,(%rdi)
    29a1c4358:	add    %eax,(%rsp,%rdi,4)
    29a1c435b:	adc    (%rax),%eax
    29a1c435d:	add    %al,(%rsi)
@@ -19110,15 +19054,15 @@
    29a1c4394:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
    29a1c4399:	outsb  %ds:(%rsi),(%dx)
    29a1c439a:	rex.XB outsl %ds:(%rsi),(%dx)
    29a1c439c:	jne    29a1c440c <.debug_info+0x10aa>
    29a1c439e:	je     29a1c43a0 <.debug_info+0x103e>
    29a1c43a0:	addr32 (bad)
    29a1c43a2:	add    %al,(%rax)
-   29a1c43a4:	add    %dh,%al
+   29a1c43a4:	add    %dl,%al
    29a1c43a6:	(bad)
    29a1c43a7:	sbb    0x2(%rdx),%ebx
    29a1c43ad:	(bad)
    29a1c43ae:	add    %al,(%rax)
    29a1c43b0:	add    %al,(%rax)
    29a1c43b2:	add    %al,(%rax)
    29a1c43b4:	add    %al,(%rcx)
@@ -19136,15 +19080,15 @@
    29a1c43cb:	push   $0x15
    29a1c43cd:	adc    $0xc5000009,%eax
    29a1c43d2:	(bad)
    29a1c43d3:	add    %al,(%rax)
    29a1c43d5:	ret
    29a1c43d6:	(bad)
    29a1c43d7:	add    %al,(%rax)
-   29a1c43d9:	or     %ebx,-0xfffffed(%rdi)
+   29a1c43d9:	or     %ebx,-0x2fffffed(%rdi)
    29a1c43df:	(bad)
    29a1c43e0:	sbb    0x2(%rdx),%ebx
    29a1c43e6:	add    $0xe8,%eax
    29a1c43eb:	insl   (%dx),%es:(%rdi)
    29a1c43ec:	or     %eax,(%rsp,%rdi,4)
    29a1c43ef:	adc    (%rax),%eax
    29a1c43f1:	add    %al,(%rsi)
@@ -19155,15 +19099,15 @@
    29a1c43fd:	fsts   (%rbx)
    29a1c43ff:	add    %al,(%rax)
    29a1c4401:	add    %ah,%ah
    29a1c4403:	adc    (%rax),%eax
    29a1c4405:	add    %cl,(%rcx)
    29a1c4407:	lahf
    29a1c4408:	adc    (%rax),%eax
-   29a1c440a:	add    %al,(%rax)
+   29a1c440a:	add    %ah,%al
    29a1c440c:	(bad)
    29a1c440d:	sbb    0x2(%rdx),%ebx
    29a1c4413:	add    %bh,%al
    29a1c4415:	add    %al,(%rax)
    29a1c4417:	add    %cl,(%rdi)
    29a1c4419:	add    %eax,(%rsp,%rdi,4)
    29a1c441c:	adc    (%rax),%eax
@@ -19198,15 +19142,15 @@
    29a1c445a:	outsb  %ds:(%rsi),(%dx)
    29a1c445b:	rex.RX outsl %ds:(%rsi),(%dx)
    29a1c445d:	jb     29a1c44a0 <.debug_info+0x113e>
    29a1c445f:	fs fs jb 29a1c44c8 <.debug_info+0x1166>
    29a1c4463:	jae    29a1c44d8 <.debug_info+0x1176>
    29a1c4465:	add    %bl,0x5e(%rcx)
    29a1c4468:	or     (%rax),%al
-   29a1c446a:	add    %dh,0x1e(%rax)
+   29a1c446a:	add    %dl,0x1e(%rax)
    29a1c446d:	sbb    0x2(%rdx),%ebx
    29a1c4473:	addb   $0x0,(%rax)
    29a1c4476:	add    %al,(%rax)
    29a1c4478:	add    %al,(%rax)
    29a1c447a:	add    %al,(%rcx)
    29a1c447c:	pushf
    29a1c447d:	adc    $0x12,%al
@@ -19232,15 +19176,15 @@
    29a1c44a8:	sbb    %ecx,(%rdi)
    29a1c44aa:	add    %al,(%rax)
    29a1c44ac:	(bad)
    29a1c44ad:	sldt   (%rax)
    29a1c44b0:	(bad)
    29a1c44b1:	lahf
    29a1c44b2:	adc    (%rax),%eax
-   29a1c44b4:	add    %dh,0x1e(%rax)
+   29a1c44b4:	add    %dl,0x1e(%rax)
    29a1c44b7:	sbb    0x2(%rdx),%ebx
    29a1c44bd:	(bad)
    29a1c44be:	ret    $0x0
    29a1c44c1:	add    %bl,-0x41(%rdi)
    29a1c44c4:	adc    %eax,(%rax)
    29a1c44c6:	add    %al,(%rsp,%rdi,4)
    29a1c44c9:	adc    (%rax),%eax
@@ -19253,20 +19197,20 @@
    29a1c44d7:	fsts   (%rbx)
    29a1c44d9:	add    %al,(%rax)
    29a1c44db:	add    %ah,%ah
    29a1c44dd:	adc    (%rax),%eax
    29a1c44df:	add    %cl,(%rcx)
    29a1c44e1:	lahf
    29a1c44e2:	adc    (%rax),%eax
-   29a1c44e4:	add    %al,0x29a1b1e(%rax)
-   29a1c44ea:	add    %al,(%rax)
-   29a1c44ec:	add    %al,(%rax)
-   29a1c44ee:	rolb   %cl,(%rax)
-   29a1c44f0:	add    %al,(%rax)
-   29a1c44f2:	sgdt   (%rsp,%rdi,4)
+   29a1c44e4:	add    %ah,0x1e(%rax)
+   29a1c44e7:	sbb    0x2(%rdx),%ebx
+   29a1c44ed:	add    %dl,%dl
+   29a1c44ef:	add    %al,(%rax)
+   29a1c44f1:	add    %cl,(%rdi)
+   29a1c44f3:	add    %eax,(%rsp,%rdi,4)
    29a1c44f6:	adc    (%rax),%eax
    29a1c44f8:	add    %al,(%rsi)
    29a1c44fa:	rolb   %cl,(%rax)
    29a1c44fc:	add    %al,(%rax)
    29a1c44fe:	add    %bh,%al
    29a1c4500:	adc    (%rax),%eax
    29a1c4502:	add    %al,(%rbx)
@@ -19280,20 +19224,19 @@
    29a1c4516:	sldt   (%rax)
    29a1c4519:	xor    $0xf,%al
    29a1c451b:	add    %al,(%rax)
    29a1c451d:	add    %al,(%rax)
    29a1c451f:	add    %al,(%rax)
    29a1c4521:	or     %ecx,0x13(%rbp)
    29a1c4524:	add    %al,(%rax)
-   29a1c4526:	test   $0x29a1b1e,%eax
-   29a1c452b:	add    %al,(%rax)
-   29a1c452d:	add    %al,(%rcx)
-   29a1c452f:	fldl   (%rax)
-   29a1c4531:	add    %al,(%rax)
-   29a1c4533:	movsxd (%rdx),%ecx
+   29a1c4526:	mov    %ebx,(%rsi)
+   29a1c4528:	sbb    0x2(%rdx),%ebx
+   29a1c452e:	add    %ebx,%ebp
+   29a1c4530:	add    %al,(%rax)
+   29a1c4532:	add    %ah,0xa(%rbx)
    29a1c4535:	adc    %dh,0x13(%rcx)
    29a1c4538:	add    %al,(%rax)
    29a1c453a:	rex.X sldt (%rax)
    29a1c453e:	rex sldt (%rax)
    29a1c4542:	add    $0x66,%al
    29a1c4544:	adc    (%rax),%eax
    29a1c4546:	add    %al,(%rsi)
@@ -19319,20 +19262,17 @@
    29a1c4584:	outsb  %ds:(%rsi),(%dx)
    29a1c4585:	rex.X jns 29a1c45d6 <.debug_info+0x1274>
    29a1c4588:	(bad)
    29a1c4589:	insl   (%dx),%es:(%rdi)
    29a1c458a:	add    %bh,%gs:(%rdx)
    29a1c458d:	pop    %rsi
    29a1c458e:	or     (%rax),%al
-   29a1c4590:	add    %dl,%al
-   29a1c4592:	sbb    $0x29a1b,%eax
-   29a1c4597:	add    %al,(%rax)
-   29a1c4599:	popf
-   29a1c459a:	add    %al,(%rax)
-   29a1c459c:	add    %al,(%rax)
+   29a1c4590:	add    %dh,0x29a1b1d(%rax)
+   29a1c4596:	add    %al,(%rax)
+   29a1c4598:	add    %bl,0x0(%rbp)
    29a1c459e:	add    %al,(%rax)
    29a1c45a0:	add    %al,(%rcx)
    29a1c45a2:	pushf
    29a1c45a3:	adc    (%r8),%r8
    29a1c45a6:	add    %dl,(%rcx)
    29a1c45a8:	jo     29a1c45f8 <.debug_info+0x1296>
    29a1c45aa:	(bad)
@@ -19366,15 +19306,15 @@
    29a1c45f7:	add    %cl,%cl
    29a1c45f9:	sldt   (%rax)
    29a1c45fc:	(bad)
    29a1c45fd:	sldt   (%rax)
    29a1c4600:	(bad)
    29a1c4601:	lahf
    29a1c4602:	adc    (%rax),%eax
-   29a1c4604:	add    %ah,%ch
+   29a1c4604:	add    %al,%ch
    29a1c4606:	sbb    $0x29a1b,%eax
    29a1c460b:	add    %al,(%rax)
    29a1c460d:	add    0x46000000(%rdi),%dh
    29a1c4613:	adc    $0x4000013,%eax
    29a1c4618:	mov    $0x6000013,%esp
    29a1c461d:	mov    $0x0,%bh
    29a1c461f:	add    %al,(%rax)
@@ -19384,18 +19324,18 @@
    29a1c4627:	fsts   (%rbx)
    29a1c4629:	add    %al,(%rax)
    29a1c462b:	add    %ah,%ah
    29a1c462d:	adc    (%rax),%eax
    29a1c462f:	add    %bl,(%rcx)
    29a1c4631:	lahf
    29a1c4632:	adc    (%rax),%eax
-   29a1c4634:	add    %dh,%ch
+   29a1c4634:	add    %dl,%ch
    29a1c4636:	sbb    $0x29a1b,%eax
    29a1c463b:	add    %al,(%rax)
-   29a1c463d:	add    %dh,%ch
+   29a1c463d:	add    %dl,%ch
    29a1c463f:	sbb    $0x29a1b,%eax
    29a1c4644:	add    %al,(%rax)
    29a1c4646:	(bad)
    29a1c4647:	add    %al,(%rax)
    29a1c4649:	add    %al,(%rax)
    29a1c464b:	add    %al,(%rax)
    29a1c464d:	add    %cl,(%rdi)
@@ -19415,21 +19355,23 @@
    29a1c4669:	adc    (%rax),%eax
    29a1c466b:	add    %bl,%dh
    29a1c466d:	sldt   (%rax)
    29a1c4670:	fmull  (%rdi)
    29a1c4672:	add    %al,(%rax)
    29a1c4674:	add    %al,(%rax)
    29a1c4676:	add    %ah,(%rsi)
-   29a1c4678:	fistps 0x29a1b(%rip)        # 29a1ee099 <.debug_rnglists+0x1dff5>
-   29a1c467e:	add    %al,(%rax)
-   29a1c4680:	movabs %al,0x170000132d00000b
+   29a1c4678:	mov    $0x29a1b1d,%edi
+   29a1c467d:	add    %al,(%rax)
+   29a1c467f:	add    %ah,0x2d00000b(%rdx)
+   29a1c4685:	adc    (%rax),%eax
+   29a1c4687:	add    %dl,(%rdi)
    29a1c4689:	add    %edx,0x2(%rdx)
    29a1c468c:	je     29a1c468e <.debug_info+0x132c>
    29a1c468e:	add    %ah,(%rdi)
-   29a1c4690:	rex.WX (bad)
+   29a1c4690:	sub    (%rsi),%bl
    29a1c4692:	sbb    0x2(%rdx),%ebx
    29a1c4698:	jp     29a1c46a5 <.debug_info+0x1343>
    29a1c469a:	add    %al,(%rax)
    29a1c469c:	(bad)
    29a1c469d:	add    %edx,0x2(%rdx)
    29a1c46a0:	jae    29a1c46a2 <.debug_info+0x1340>
    29a1c46a2:	(bad)
@@ -19499,16 +19441,17 @@
    29a1c474e:	fs gs jb 29a1c4752 <.debug_info+0x13f0>
    29a1c4752:	adc    (%rdx),%ebx
    29a1c4754:	jbe    29a1c475e <.debug_info+0x13fc>
    29a1c4756:	add    %al,(%rax)
    29a1c4758:	add    %ch,(%rcx)
    29a1c475a:	lahf
    29a1c475b:	adc    (%rax),%eax
-   29a1c475d:	add    %dl,0x1d(%rax)
-   29a1c4760:	sbb    0x2(%rdx),%ebx
+   29a1c475d:	add    %dh,(%rax)
+   29a1c475f:	sbb    $0x29a1b,%eax
+   29a1c4764:	add    %al,(%rax)
    29a1c4766:	sub    $0x0,%al
    29a1c4768:	add    %al,(%rax)
    29a1c476a:	add    %al,(%rax)
    29a1c476c:	add    %al,(%rax)
    29a1c476e:	add    %ebx,0x10000014(%rsi,%rdi,2)
    29a1c4775:	mov    $0xec000013,%esp
    29a1c477a:	sldt   (%rax)
@@ -19520,15 +19463,15 @@
    29a1c478a:	cli
    29a1c478b:	sldt   (%rax)
    29a1c478e:	add    %cl,%bl
    29a1c4790:	adc    (%rax),%eax
    29a1c4792:	add    %al,(%rdx)
    29a1c4794:	in     $0x13,%al
    29a1c4796:	add    %al,(%rax)
-   29a1c4798:	or     %ebx,0x59000013(%rdi)
+   29a1c4798:	or     %ebx,0x39000013(%rdi)
    29a1c479e:	sbb    $0x29a1b,%eax
    29a1c47a3:	add    %al,(%rax)
    29a1c47a5:	add    %dh,0xf000000(%rax)
    29a1c47ab:	add    %edx,(%rax)
    29a1c47ad:	mov    $0x12000013,%esp
    29a1c47b2:	adc    %al,(%rax)
    29a1c47b4:	add    %cl,(%rax,%rdx,1)
@@ -19551,20 +19494,25 @@
    29a1c47d6:	adc    %al,(%rax)
    29a1c47d8:	add    %dh,(%rdi)
    29a1c47da:	adc    %al,(%rax)
    29a1c47dc:	add    %al,(%rax)
    29a1c47de:	add    %al,(%rax)
    29a1c47e0:	sub    0x13(%rbp),%cl
    29a1c47e3:	add    %al,(%rax)
-   29a1c47e5:	sbbb   $0x0,0x29a1b(%rip)        # 29a1ee207 <.debug_rnglists+0x1e163>
-   29a1c47ec:	add    %dl,0x0(%rax)
-   29a1c47ef:	add    %al,(%rax)
-   29a1c47f1:	add    %al,(%rax)
-   29a1c47f3:	add    %al,(%rax)
-   29a1c47f5:	add    %ebx,0x1366(%rax,%rdx,1)
+   29a1c47e5:	(bad)
+   29a1c47e6:	sbb    $0x29a1b,%eax
+   29a1c47eb:	add    %al,(%rax)
+   29a1c47ed:	push   %rax
+   29a1c47ee:	add    %al,(%rax)
+   29a1c47f0:	add    %al,(%rax)
+   29a1c47f2:	add    %al,(%rax)
+   29a1c47f4:	add    %al,(%rcx)
+   29a1c47f6:	pushf
+   29a1c47f7:	adc    %ah,0x13(%rsi)
+   29a1c47fa:	add    %al,(%rax)
    29a1c47fc:	adc    %r8b,(%r8)
    29a1c47ff:	add    %al,0x10(%rcx)
    29a1c4802:	add    %al,(%rax)
    29a1c4804:	sub    0x13(%rcx),%esi
    29a1c4807:	add    %al,(%rax)
    29a1c4809:	add    %edx,0x3(%rcx)
    29a1c480c:	jge    29a1c4821 <.debug_info+0x14bf>
@@ -19616,36 +19564,30 @@
    29a1c4888:	outsb  %ds:(%esi),(%dx)
    29a1c488a:	jne    29a1c48c5 <.debug_info+0x91>
    29a1c488c:	cmp    %eax,(%rax)
    29a1c488e:	or     $0x82,%al
    29a1c4890:	or     (%rax),%al
    29a1c4892:	add    %ch,0xa(%rdx)
    29a1c4895:	add    %al,(%rax)
-   29a1c4897:	push   %rax
-   29a1c4898:	and    %ebx,(%rbx)
-   29a1c489a:	(bad)
-   29a1c489b:	add    (%rax),%al
-   29a1c489d:	add    %al,(%rax)
+   29a1c4897:	xor    %ah,(%rcx)
+   29a1c4899:	sbb    0x2(%rdx),%ebx
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
-   29a1c48b8:	push   %rax
-   29a1c48b9:	and    %ebx,(%rbx)
-   29a1c48bb:	(bad)
-   29a1c48bc:	add    (%rax),%al
-   29a1c48be:	add    %al,(%rax)
+   29a1c48b8:	xor    %ah,(%rcx)
+   29a1c48ba:	sbb    0x2(%rdx),%ebx
    29a1c48c0:	add    (%rax),%eax
    29a1c48c2:	add    %al,(%rax)
    29a1c48c4:	add    %al,(%rax)
    29a1c48c6:	add    %al,(%rax)
    29a1c48c8:	add    %ebx,0x1f6(%rax,%rax,1)
 
 000000029a1c48cb <.debug_info>:
@@ -19677,15 +19619,15 @@
    29a1c491f:	outsb  %ds:(%esi),(%dx)
    29a1c4921:	jne    29a1c495c <.debug_info+0x91>
    29a1c4923:	cmp    %eax,(%rax)
    29a1c4925:	or     $0x9,%al
    29a1c4927:	or     (%rax),%eax
    29a1c4929:	add    %bh,(%rbx)
    29a1c492b:	or     (%rax),%eax
-   29a1c492d:	add    %ah,0x29a1b21(%rax)
+   29a1c492d:	add    %al,0x29a1b21(%rax)
    29a1c4933:	add    %al,(%rax)
    29a1c4935:	add    %al,(%rsi)
    29a1c4937:	add    %al,(%rax)
    29a1c4939:	add    %al,(%rax)
    29a1c493b:	add    %al,(%rax)
    29a1c493d:	add    %dl,0x1000014(%rbx)
    29a1c4943:	add    %eax,(%rsi)
@@ -19806,15 +19748,19 @@
    29a1c4a65:	rex.RB outsb %ds:(%rsi),(%dx)
    29a1c4a67:	je     29a1c4adb <.debug_info+0x16>
    29a1c4a69:	jns    29a1c4abb <.debug_info+0x1f0>
    29a1c4a6b:	outsl  %ds:(%rsi),(%dx)
    29a1c4a6c:	imul   $0xd0d0100,0x74(%rsi),%ebp
    29a1c4a73:	or     (%rcx),%eax
    29a1c4a75:	add    %al,(%rax)
-   29a1c4a77:	movabs 0x6000000029a1b21,%al
+   29a1c4a77:	andb   $0x1b,(%rcx)
+   29a1c4a7a:	(bad)
+   29a1c4a7b:	add    (%rax),%al
+   29a1c4a7d:	add    %al,(%rax)
+   29a1c4a7f:	(bad)
    29a1c4a80:	add    %al,(%rax)
    29a1c4a82:	add    %al,(%rax)
    29a1c4a84:	add    %al,(%rax)
    29a1c4a86:	add    %al,(%rcx)
    29a1c4a88:	pushf
    29a1c4a89:	add    0x44(%rax),%ebp
    29a1c4a8c:	insb   (%dx),%es:(%rdi)
@@ -19873,15 +19819,15 @@
    29a1c4b19:	outsb  %ds:(%esi),(%dx)
    29a1c4b1b:	jne    29a1c4b56 <.debug_info+0x91>
    29a1c4b1d:	cmp    %eax,(%rax)
    29a1c4b1f:	or     $0xef,%al
    29a1c4b21:	or     (%rax),%eax
    29a1c4b23:	add    %dl,%bh
    29a1c4b25:	or     (%rax),%eax
-   29a1c4b27:	add    %dh,0x29a1b21(%rax)
+   29a1c4b27:	add    %dl,0x29a1b21(%rax)
    29a1c4b2d:	add    %al,(%rax)
    29a1c4b2f:	add    %al,(%rsi)
    29a1c4b31:	add    %al,(%rax)
    29a1c4b33:	add    %al,(%rax)
    29a1c4b35:	add    %al,(%rax)
    29a1c4b37:	add    %bh,%dl
    29a1c4b39:	adc    $0x0,%al
@@ -20000,15 +19946,15 @@
    29a1c4c56:	(bad)
    29a1c4c5b:	(bad)
    29a1c4c5c:	rex.R insb (%dx),%es:(%rdi)
    29a1c4c5e:	insb   (%dx),%es:(%rdi)
    29a1c4c5f:	rex.WRB (bad)
    29a1c4c61:	imul   $0xb128804,0x0(%rsi),%ebp
    29a1c4c68:	add    %eax,(%rax)
-   29a1c4c6a:	add    %dh,0x29a1b21(%rax)
+   29a1c4c6a:	add    %dl,0x29a1b21(%rax)
    29a1c4c70:	add    %al,(%rax)
    29a1c4c72:	add    %al,(%rsi)
    29a1c4c74:	add    %al,(%rax)
    29a1c4c76:	add    %al,(%rax)
    29a1c4c78:	add    %al,(%rax)
    29a1c4c7a:	add    %al,(%rcx)
    29a1c4c7c:	pushf
@@ -20067,15 +20013,15 @@
    29a1c4d06:	xor    (%rax),%ah
    29a1c4d08:	sub    $0x3d647473,%eax
    29a1c4d0d:	outsb  %ds:(%esi),(%dx)
    29a1c4d0f:	jne    29a1c4d4a <.debug_info+0x91>
    29a1c4d11:	cmp    %eax,(%rax)
    29a1c4d13:	or     $0xc4,%al
    29a1c4d15:	or     $0x0,%al
-   29a1c4d17:	add    %ch,0x21c00000(%rsp,%rcx,1)
+   29a1c4d17:	add    %ch,0x21a00000(%rsp,%rcx,1)
    29a1c4d1e:	sbb    0x2(%rdx),%ebx
    29a1c4d24:	(bad)
    29a1c4d25:	add    %al,(%rax)
    29a1c4d27:	add    %al,(%rax)
    29a1c4d29:	add    %al,(%rax)
    29a1c4d2b:	add    %ah,0x0(%rbp,%rdx,1)
    29a1c4d2f:	add    %al,(%rsi)
@@ -20356,19 +20302,15 @@
    29a1c4fbc:	mov    $0x0,%bl
    29a1c4fbe:	add    %al,(%rax)
    29a1c4fc0:	add    %dl,0x72706676(%rip)        # 30c8cb63c <.debug_rnglists+0x726fb598>
    29a1c4fc6:	imul   $0x6040066,0x74(%rsi),%ebp
    29a1c4fcd:	add    (%rdi),%cl
    29a1c4fcf:	or     %eax,(%rcx)
    29a1c4fd1:	add    %al,(%rax)
-   29a1c4fd3:	shlb   $0x1b,(%rcx)
-   29a1c4fd6:	(bad)
-   29a1c4fd7:	add    (%rax),%al
-   29a1c4fd9:	add    %al,(%rax)
-   29a1c4fdb:	(bad)
+   29a1c4fd3:	movabs 0x1e000000029a1b21,%al
    29a1c4fdc:	add    %al,(%rax)
    29a1c4fde:	add    %al,(%rax)
    29a1c4fe0:	add    %al,(%rax)
    29a1c4fe2:	add    %al,(%rcx)
    29a1c4fe4:	pushf
    29a1c4fe5:	or     %bl,0x46(%rdi)
    29a1c4fe8:	imul   $0x2952a,0x0(%rbp,%riz,2),%ebp
@@ -20394,17 +20336,18 @@
    29a1c5014:	imul   $0xb35a00,0x74(%rbx),%r14
    29a1c501c:	add    %al,(%rax)
    29a1c501e:	or     (%rcx),%dl
    29a1c5020:	add    %al,(%rax)
    29a1c5022:	add    $0x11,%al
    29a1c5024:	add    %al,(%rax)
    29a1c5026:	(bad)
-   29a1c5027:	fldenv (%rcx)
-   29a1c5029:	sbb    0x2(%rdx),%ebx
-   29a1c502f:	lret   $0x2
+   29a1c5027:	mov    $0x29a1b21,%ecx
+   29a1c502c:	add    %al,(%rax)
+   29a1c502e:	add    %cl,%dl
+   29a1c5030:	add    (%rax),%al
    29a1c5032:	add    %al,0x30015201(%rip)        # 2ca1da239 <.debug_rnglists+0x3000a195>
    29a1c5038:	add    $0xa3035101,%eax
    29a1c503d:	add    %edx,0x5(%rdx)
    29a1c5040:	add    %ebx,0x3(%rax)
    29a1c5043:	movabs %eax,0x530015901055101
    29a1c504c:	add    0x20(%rdi),%dh
    29a1c504f:	add    0x5801(%rbx),%esp
@@ -20440,16 +20383,18 @@
    29a1c50a5:	sub    $0x3d647473,%eax
    29a1c50aa:	outsb  %ds:(%esi),(%dx)
    29a1c50ac:	jne    29a1c50e7 <.debug_info+0x91>
    29a1c50ae:	cmp    %eax,(%rax)
    29a1c50b0:	or     $0xac,%al
    29a1c50b2:	or     $0xd940000,%eax
    29a1c50b7:	add    %al,(%rax)
-   29a1c50b9:	loopne 29a1c50dc <.debug_info+0x86>
-   29a1c50bb:	sbb    0x2(%rdx),%ebx
+   29a1c50b9:	shlb   $0x1b,(%rcx)
+   29a1c50bc:	(bad)
+   29a1c50bd:	add    (%rax),%al
+   29a1c50bf:	add    %al,(%rax)
    29a1c50c1:	(bad)
    29a1c50c2:	add    (%rax),%al
    29a1c50c4:	add    %al,(%rax)
    29a1c50c6:	add    %al,(%rax)
    29a1c50c8:	add    %dl,%dh
    29a1c50ca:	adc    $0x5f0b0000,%eax
    29a1c50cf:	pop    %rdi
@@ -21969,16 +21914,19 @@
    29a1c5d5f:	jb     29a1c5dca <.debug_info+0xd74>
    29a1c5d61:	outsb  %ds:(%rsi),(%dx)
    29a1c5d62:	je     29a1c5dca <.debug_info+0xd74>
    29a1c5d64:	add    %cl,(%rbx)
    29a1c5d66:	and    (%rdi,%rcx,1),%eax
    29a1c5d69:	(bad)
    29a1c5d6a:	add    %eax,(%rax)
-   29a1c5d6c:	add    %al,0x23(%rax)
-   29a1c5d6f:	sbb    0x2(%rdx),%ebx
+   29a1c5d6c:	add    %ah,(%rax)
+   29a1c5d6e:	and    (%rbx),%ebx
+   29a1c5d70:	(bad)
+   29a1c5d71:	add    (%rax),%al
+   29a1c5d73:	add    %al,(%rax)
    29a1c5d75:	xor    $0x0,%eax
    29a1c5d7a:	add    %al,(%rax)
    29a1c5d7c:	add    %al,(%rcx)
    29a1c5d7e:	pushf
    29a1c5d7f:	movsb  %ds:(%rsi),%es:(%rdi)
    29a1c5d80:	or     $0x66080000,%eax
    29a1c5d85:	imul   $0xa932196,0x0(%rbp,%riz,2),%ebp
@@ -22003,16 +21951,19 @@
    29a1c5dbe:	cltd
    29a1c5dbf:	(bad)
    29a1c5dc0:	(bad)
    29a1c5dc1:	add    %eax,(%rax)
    29a1c5dc3:	add    %ch,0x11(%rdx)
    29a1c5dc6:	add    %al,(%rax)
    29a1c5dc8:	push   $0x16000011
-   29a1c5dcd:	jo     29a1c5df2 <.debug_info+0xd9c>
-   29a1c5dcf:	sbb    0x2(%rdx),%ebx
+   29a1c5dcd:	push   %rax
+   29a1c5dce:	and    (%rbx),%ebx
+   29a1c5dd0:	(bad)
+   29a1c5dd1:	add    (%rax),%al
+   29a1c5dd3:	add    %al,(%rax)
    29a1c5dd5:	(bad)
    29a1c5dd6:	or     (%rax),%al
    29a1c5dd8:	add    %al,(%rsi)
    29a1c5dda:	add    %edx,0x1(%rdx)
    29a1c5ddd:	xor    $0x6,%al
    29a1c5ddf:	add    %edx,0x3(%rcx)
    29a1c5de2:	movabs %eax,0x1a3035801065201
@@ -22023,45 +21974,50 @@
    29a1c5df2:	add    0x20(%rdi),%dh
    29a1c5df5:	add    0x2c000010(%rcx),%dl
    29a1c5dfb:	je     29a1c5e77 <.debug_info+0xe21>
    29a1c5dfd:	jae    29a1c5e64 <.debug_info+0xe0e>
    29a1c5dff:	je     29a1c5e01 <.debug_info+0xdab>
    29a1c5e01:	add    (%rdx),%ah
    29a1c5e03:	add    %edx,(%rax)
-   29a1c5e05:	andb   $0x1b,(%rbx)
+   29a1c5e05:	(bad)
+   29a1c5e06:	and    (%rbx),%ebx
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
-   29a1c5e20:	test   %ah,(%rbx)
-   29a1c5e22:	sbb    0x2(%rdx),%ebx
-   29a1c5e28:	add    %eax,0x29a1b(%rbx,%riz,1)
+   29a1c5e20:	and    %fs:(%rbx),%ebx
+   29a1c5e23:	(bad)
+   29a1c5e24:	add    (%rax),%al
+   29a1c5e26:	add    %al,(%rax)
+   29a1c5e28:	add    %esp,0x1b(%rbx,%riz,1)
+   29a1c5e2c:	(bad)
+   29a1c5e2d:	add    (%rax),%al
    29a1c5e2f:	add    %al,(%rax)
    29a1c5e31:	sub    $0x0,%eax
    29a1c5e36:	add    %al,(%rax)
    29a1c5e38:	add    %al,(%rcx)
    29a1c5e3a:	xchg   %eax,%ecx
-   29a1c5e3b:	add    -0x65e4dc6e(%rip),%eax        # 2343781d3 <__size_of_stack_reserve__+0x2341781d3>
+   29a1c5e3b:	add    -0x65e4dc8e(%rip),%eax        # 2343781b3 <__size_of_stack_reserve__+0x2341781b3>
    29a1c5e41:	add    (%rax),%al
    29a1c5e43:	add    %al,(%rax)
    29a1c5e45:	sub    (%rbx),%ecx
    29a1c5e47:	add    %al,(%rax)
-   29a1c5e49:	add    $0x9a1b239e,%eax
+   29a1c5e49:	add    $0x9a1b237e,%eax
    29a1c5e4e:	add    (%rax),%al
    29a1c5e50:	add    %al,(%rax)
    29a1c5e52:	sbb    %cl,(%rbx)
    29a1c5e54:	add    %al,(%rax)
-   29a1c5e56:	add    $0x9a1b23aa,%eax
+   29a1c5e56:	add    $0x9a1b238a,%eax
    29a1c5e5b:	add    (%rax),%al
    29a1c5e5d:	add    %al,(%rax)
    29a1c5e5f:	add    $0xb,%eax
    29a1c5e64:	add    %ch,(%rsi)
    29a1c5e66:	pop    %rdi
    29a1c5e67:	je     29a1c5ee3 <.debug_info+0xe8d>
    29a1c5e69:	jae    29a1c5ed0 <.debug_info+0xe7a>
@@ -22074,56 +22030,58 @@
    29a1c5e7c:	je     29a1c5edd <.debug_info+0xe87>
    29a1c5e7e:	outsw  %ds:(%rsi),(%dx)
    29a1c5e80:	jb     29a1c5eef <.debug_info+0xe99>
    29a1c5e82:	(bad)
    29a1c5e83:	je     29a1c5e85 <.debug_info+0xe2f>
    29a1c5e85:	add    %ebp,0x16(%rsi)
    29a1c5e88:	rex.RX add (%rax),%r8b
-   29a1c5e8b:	add    %ah,%al
+   29a1c5e8b:	add    %al,%al
    29a1c5e8d:	and    %ebx,(%rbx)
    29a1c5e8f:	(bad)
    29a1c5e90:	add    (%rax),%al
    29a1c5e92:	add    %al,(%rax)
    29a1c5e94:	add    (%rax),%eax
    29a1c5e96:	add    %al,(%rax)
    29a1c5e98:	add    %al,(%rax)
    29a1c5e9a:	add    %al,(%rax)
    29a1c5e9c:	add    %ebx,0x736d615f(%rax,%rsi,1)
    29a1c5ea3:	addr32 pop %rdi
    29a1c5ea5:	gs js  29a1c5f11 <.debug_info+0xebb>
    29a1c5ea8:	je     29a1c5eaa <.debug_info+0xe54>
    29a1c5eaa:	add    %ebp,0x26(%rcx)
-   29a1c5ead:	adc    %ah,(%rbx)
-   29a1c5eaf:	sbb    0x2(%rdx),%ebx
+   29a1c5ead:	lock and (%rbx),%bl
+   29a1c5eb0:	(bad)
+   29a1c5eb1:	add    (%rax),%al
+   29a1c5eb3:	add    %al,(%rax)
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
-   29a1c5ed6:	adc    %esp,(%rcx)
+   29a1c5ed6:	adc    %eax,(%rcx)
    29a1c5ed8:	and    (%rbx),%ebx
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
-   29a1c5eed:	adc    %esi,(%rbx)
+   29a1c5eed:	adc    %edx,(%rbx)
    29a1c5eef:	and    (%rbx),%ebx
    29a1c5ef1:	(bad)
    29a1c5ef2:	add    (%rax),%al
    29a1c5ef4:	add    %al,(%rax)
    29a1c5ef6:	push   %rcx
    29a1c5ef7:	or     (%rax),%eax
    29a1c5ef9:	add    %bh,0x1060000(%rsi,%rcx,1)
@@ -22132,15 +22090,16 @@
    29a1c5f03:	rolb   $0x9a,0x1b(%rcx)
    29a1c5f07:	add    (%rax),%al
    29a1c5f09:	add    %al,(%rax)
    29a1c5f0b:	(bad)
    29a1c5f0c:	add    %ebx,0x2(%rax)
    29a1c5f0f:	jae    29a1c5f11 <.debug_info+0xebb>
    29a1c5f11:	add    %dl,(%rsi)
-   29a1c5f13:	ds and (%rbx),%ebx
+   29a1c5f13:	(bad)
+   29a1c5f14:	and    (%rbx),%ebx
    29a1c5f16:	(bad)
    29a1c5f17:	add    (%rax),%al
    29a1c5f19:	add    %al,(%rax)
    29a1c5f1b:	cmp    $0xb,%al
    29a1c5f1d:	add    %al,(%rax)
    29a1c5f1f:	(bad)
    29a1c5f20:	add    %edx,0x2(%rdx)
@@ -22149,15 +22108,15 @@
    29a1c5f27:	adc    $0x715f7461,%eax
    29a1c5f2c:	jne    29a1c5f97 <.debug_info+0xf41>
    29a1c5f2e:	movsxd 0x5f(%rbx),%ebp
    29a1c5f31:	gs js  29a1c5f9d <.debug_info+0xf47>
    29a1c5f34:	je     29a1c5f36 <.debug_info+0xee0>
    29a1c5f36:	add    $0x1e0f01ab,%eax
    29a1c5f3b:	add    %eax,(%rax)
-   29a1c5f3d:	add    %dh,%al
+   29a1c5f3d:	add    %dl,%al
    29a1c5f3f:	and    (%rbx),%bl
    29a1c5f41:	(bad)
    29a1c5f42:	add    (%rax),%al
    29a1c5f44:	add    %al,(%rax)
    29a1c5f46:	adc    $0x0,%eax
    29a1c5f4b:	add    %al,(%rax)
    29a1c5f4d:	add    %al,(%rcx)
@@ -22169,60 +22128,58 @@
    29a1c5f58:	movsxd (%rax),%eax
    29a1c5f5a:	pop    %rbp
    29a1c5f5b:	sub    %ch,%dh
    29a1c5f5d:	add    (%rax),%al
    29a1c5f5f:	add    %cl,-0x7affffef(%rcx)
    29a1c5f65:	adc    %eax,(%rax)
    29a1c5f67:	add    %dh,(%rcx)
-   29a1c5f69:	add    $0x29a1b23,%eax
-   29a1c5f6e:	add    %al,(%rax)
-   29a1c5f70:	add    %bl,0x15000000(%rbx,%rcx,1)
-   29a1c5f77:	pop    %rdi
-   29a1c5f78:	outsl  %ds:(%rsi),(%dx)
-   29a1c5f79:	outsb  %ds:(%rsi),(%dx)
-   29a1c5f7a:	gs js  29a1c5fe6 <.debug_info+0xf90>
+   29a1c5f69:	in     $0x22,%eax
+   29a1c5f6b:	sbb    0x2(%rdx),%ebx
+   29a1c5f71:	pushf
+   29a1c5f72:	or     (%rax),%eax
+   29a1c5f74:	add    %al,(%rax)
+   29a1c5f76:	adc    $0x656e6f5f,%eax
+   29a1c5f7b:	js     29a1c5fe6 <.debug_info+0xf90>
    29a1c5f7d:	je     29a1c5f7f <.debug_info+0xf29>
    29a1c5f7f:	add    $0xc0150287,%eax
    29a1c5f84:	add    (%rax),%al
-   29a1c5f86:	add    %dl,%al
-   29a1c5f88:	and    (%rbx),%bl
-   29a1c5f8a:	(bad)
-   29a1c5f8b:	add    (%rax),%al
-   29a1c5f8d:	add    %al,(%rax)
-   29a1c5f8f:	(bad)
+   29a1c5f86:	add    %dh,0x29a1b22(%rax)
+   29a1c5f8c:	add    %al,(%rax)
+   29a1c5f8e:	add    %bl,(%rsi)
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
-   29a1c5fb2:	frstor (%rdx)
-   29a1c5fb4:	sbb    0x2(%rdx),%ebx
-   29a1c5fba:	rorl   $0x0,(%rbx)
+   29a1c5fb2:	mov    $0x29a1b22,%ebp
+   29a1c5fb7:	add    %al,(%rax)
+   29a1c5fb9:	add    %al,%cl
+   29a1c5fbb:	or     (%rax),%eax
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
-   29a1c5fda:	add    %ah,0x22(%rax)
+   29a1c5fda:	add    %al,0x22(%rax)
    29a1c5fdd:	sbb    0x2(%rdx),%ebx
    29a1c5fe3:	push   $0x0
    29a1c5fe5:	add    %al,(%rax)
    29a1c5fe7:	add    %al,(%rax)
    29a1c5fe9:	add    %al,(%rax)
    29a1c5feb:	add    %ebx,0x8000010(%rbx,%rbx,2)
    29a1c5ff2:	pop    %rdi
@@ -22260,62 +22217,59 @@
    29a1c603f:	adc    (%rax),%al
    29a1c6041:	add    %ah,(%rcx)
    29a1c6043:	int1
    29a1c6044:	add    %al,(%rax)
    29a1c6046:	add    %cl,0x6c(%rdx)
    29a1c6049:	mov    (%rcx),%cs
    29a1c604b:	add    %al,(%rax)
-   29a1c604d:	add    0x22800520(%rcx),%dl
+   29a1c604d:	add    0x22600520(%rcx),%dl
    29a1c6053:	sbb    0x2(%rdx),%ebx
    29a1c6059:	xor    %cl,(%rax,%rax,1)
    29a1c605c:	add    %dl,(%rcx)
-   29a1c605e:	nop
-   29a1c605f:	and    (%rbx),%bl
-   29a1c6061:	(bad)
-   29a1c6062:	add    (%rax),%al
-   29a1c6064:	add    %al,(%rax)
+   29a1c605e:	jo     29a1c6082 <.debug_info+0x102c>
+   29a1c6060:	sbb    0x2(%rdx),%ebx
    29a1c6066:	or     %ecx,(%rax,%rax,1)
    29a1c6069:	add    %ah,(%rsi)
    29a1c606b:	adc    %al,(%rax)
    29a1c606d:	add    %al,(%rsi)
    29a1c606f:	add    %edx,0x9(%rdx)
    29a1c6072:	jbe    29a1c6074 <.debug_info+0x101e>
    29a1c6074:	or     %ah,(%rax)
    29a1c6076:	and    $0x30,%al
    29a1c6078:	cs and (%rcx),%eax
-   29a1c607b:	add    %al,-0x65e4dd6b(%rip)        # 234378316 <__size_of_stack_reserve__+0x234178316>
+   29a1c607b:	add    %al,-0x65e4dd8b(%rip)        # 2343782f6 <__size_of_stack_reserve__+0x2341782f6>
    29a1c6081:	add    (%rax),%al
    29a1c6083:	add    %al,(%rax)
    29a1c6085:	popf
    29a1c6086:	or     $0x0,%al
-   29a1c6088:	add    %al,-0x65e4dd62(%rip)        # 23437832c <__size_of_stack_reserve__+0x23417832c>
+   29a1c6088:	add    %al,-0x65e4dd82(%rip)        # 23437830c <__size_of_stack_reserve__+0x23417830c>
    29a1c608e:	add    (%rax),%al
    29a1c6090:	add    %al,(%rax)
    29a1c6092:	cmc
    29a1c6093:	or     (%rax),%eax
-   29a1c6095:	add    %al,-0x65e4dd57(%rip)        # 234378344 <__size_of_stack_reserve__+0x234178344>
+   29a1c6095:	add    %al,-0x65e4dd77(%rip)        # 234378324 <__size_of_stack_reserve__+0x234178324>
    29a1c609b:	add    (%rax),%al
    29a1c609d:	add    %al,(%rax)
    29a1c609f:	fisttps (%rbx)
    29a1c60a1:	add    %al,(%rax)
-   29a1c60a3:	add    $0x9a1b22bd,%eax
+   29a1c60a3:	add    $0x9a1b229d,%eax
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
-   29a1c60c4:	add    %dh,%al
+   29a1c60c4:	add    %dl,%al
    29a1c60c6:	and    %ebx,(%rbx)
    29a1c60c8:	(bad)
    29a1c60c9:	add    (%rax),%al
    29a1c60cb:	add    %al,(%rax)
    29a1c60cd:	push   $0x0
    29a1c60cf:	add    %al,(%rax)
    29a1c60d1:	add    %al,(%rax)
@@ -22357,73 +22311,70 @@
    29a1c6129:	adc    (%rax),%al
    29a1c612b:	add    %ah,(%rcx)
    29a1c612d:	int1
    29a1c612e:	add    %al,(%rax)
    29a1c6130:	add    %bh,(%rsi)
    29a1c6132:	mov    %gs:(%rcx),%cs
    29a1c6135:	add    %al,(%rax)
-   29a1c6137:	add    0x22100520(%rcx),%dl
+   29a1c6137:	add    0x21f00520(%rcx),%dl
    29a1c613d:	sbb    0x2(%rdx),%ebx
    29a1c6143:	(bad)  (%rax,%rax,1)
    29a1c6146:	add    %dl,(%rcx)
-   29a1c6148:	and    %ah,(%rdx)
+   29a1c6148:	add    %ah,(%rdx)
    29a1c614a:	sbb    0x2(%rdx),%ebx
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
-   29a1c6165:	add    %al,-0x65e4dddb(%rip)        # 234378390 <__size_of_stack_reserve__+0x234178390>
+   29a1c6165:	add    %al,-0x65e4ddfb(%rip)        # 234378370 <__size_of_stack_reserve__+0x234178370>
    29a1c616b:	add    (%rax),%al
    29a1c616d:	add    %al,(%rax)
    29a1c616f:	popf
    29a1c6170:	or     $0x0,%al
-   29a1c6172:	add    %al,-0x65e4ddd2(%rip)        # 2343783a6 <__size_of_stack_reserve__+0x2341783a6>
+   29a1c6172:	add    %al,-0x65e4ddf2(%rip)        # 234378386 <__size_of_stack_reserve__+0x234178386>
    29a1c6178:	add    (%rax),%al
    29a1c617a:	add    %al,(%rax)
    29a1c617c:	mov    (%rax,%rax,1),%cl
-   29a1c617f:	add    %al,-0x65e4ddc7(%rip)        # 2343783be <__size_of_stack_reserve__+0x2341783be>
+   29a1c617f:	add    %al,-0x65e4dde7(%rip)        # 23437839e <__size_of_stack_reserve__+0x23417839e>
    29a1c6185:	add    (%rax),%al
    29a1c6187:	add    %al,(%rax)
    29a1c6189:	jne    29a1c6197 <.debug_info+0x1141>
    29a1c618b:	add    %al,(%rax)
-   29a1c618d:	add    $0x9a1b224d,%eax
+   29a1c618d:	add    $0x9a1b222d,%eax
    29a1c6192:	add    (%rax),%al
    29a1c6194:	add    %al,(%rax)
    29a1c6196:	push   %rbp
    29a1c6197:	or     $0x0,%al
    29a1c6199:	add    %al,(%rax)
    29a1c619b:	xor    (%rdi),%cl
    29a1c619d:	(bad)
    29a1c619e:	add    %al,(%rax)
-   29a1c61a0:	shlb   $0x1b,(%rbx)
-   29a1c61a3:	(bad)
-   29a1c61a4:	add    (%rax),%al
-   29a1c61a6:	add    %al,(%rax)
-   29a1c61a8:	ss add %al,(%rax)
+   29a1c61a0:	movabs 0x36000000029a1b23,%al
+   29a1c61a9:	add    %al,(%rax)
    29a1c61ab:	add    %al,(%rax)
    29a1c61ad:	add    %al,(%rax)
    29a1c61af:	add    %al,(%rcx)
    29a1c61b1:	pushf
-   29a1c61b2:	add    $0x9a1b23d2,%eax
+   29a1c61b2:	add    $0x9a1b23b2,%eax
    29a1c61b7:	add    (%rax),%al
    29a1c61b9:	add    %al,(%rax)
    29a1c61bb:	sub    (%rbx),%ecx
    29a1c61bd:	add    %al,(%rax)
-   29a1c61bf:	add    $0x9a1b23de,%eax
+   29a1c61bf:	add    $0x9a1b23be,%eax
    29a1c61c4:	add    (%rax),%al
    29a1c61c6:	add    %al,(%rax)
    29a1c61c8:	sbb    %cl,(%rbx)
    29a1c61ca:	add    %al,(%rax)
-   29a1c61cc:	add    $0x9a1b23ea,%eax
+   29a1c61cc:	add    $0x9a1b23ca,%eax
    29a1c61d1:	add    (%rax),%al
    29a1c61d3:	add    %al,(%rax)
    29a1c61d5:	add    $0xb,%eax
 	...
 
 000000029a1c61db <.debug_info>:
    29a1c61db:	sahf
@@ -22456,15 +22407,15 @@
    29a1c6231:	jne    29a1c626c <.debug_info+0x91>
    29a1c6233:	cmp    %eax,(%rax)
    29a1c6235:	or     $0xc,%al
    29a1c6237:	sldt   (%rax)
    29a1c623a:	hlt
    29a1c623b:	(bad)
    29a1c623c:	add    %al,(%rax)
-   29a1c623e:	xor    %ah,0x29a1b(%rip)        # 29a1efc5f <.debug_rnglists+0x1fbbb>
+   29a1c623e:	add    %ah,0x29a1b(%rip)        # 29a1efc5f <.debug_rnglists+0x1fbbb>
    29a1c6244:	add    %al,(%rax)
    29a1c6246:	xor    (%rax),%al
    29a1c6248:	add    %al,(%rax)
    29a1c624a:	add    %al,(%rax)
    29a1c624c:	add    %al,(%rax)
    29a1c624e:	push   %rsi
    29a1c624f:	sbb    %al,(%rax)
@@ -22729,15 +22680,15 @@
    29a1c64db:	add    %al,(%rax)
    29a1c64dd:	add    %dl,(%rsi)
    29a1c64df:	data16 jo 29a1c6554 <.debug_info+0x379>
    29a1c64e2:	imul   $0xff040066,0x74(%rsi),%ebp
    29a1c64e9:	add    %ecx,(%rdi)
    29a1c64eb:	or     %eax,(%rcx)
    29a1c64ed:	add    %al,(%rax)
-   29a1c64ef:	xor    %ah,0x29a1b(%rip)        # 29a1eff10 <.debug_rnglists+0x1fe6c>
+   29a1c64ef:	add    %ah,0x29a1b(%rip)        # 29a1eff10 <.debug_rnglists+0x1fe6c>
    29a1c64f5:	add    %al,(%rax)
    29a1c64f7:	xor    (%rax),%al
    29a1c64f9:	add    %al,(%rax)
    29a1c64fb:	add    %al,(%rax)
    29a1c64fd:	add    %al,(%rax)
    29a1c64ff:	add    %ebx,0x6c69465f(%rsp,%rcx,1)
    29a1c6506:	add    %ch,%gs:(%rcx)
@@ -22768,17 +22719,18 @@
    29a1c6541:	(bad)
    29a1c6542:	or     %eax,(%rcx)
    29a1c6544:	add    %al,(%rax)
    29a1c6546:	ficoml (%rdx)
    29a1c6548:	add    %al,(%rax)
    29a1c654a:	fcoms  (%rdx)
    29a1c654c:	add    %al,(%rax)
-   29a1c654e:	sbb    %ebx,0x25(%rbp)
-   29a1c6551:	sbb    0x2(%rdx),%ebx
-   29a1c6557:	(bad)
+   29a1c654e:	sbb    %ebp,0x29a1b25(%rip)        # 29cb68079 <.debug_rnglists+0x2997fd5>
+   29a1c6554:	add    %al,(%rax)
+   29a1c6556:	add    %al,%ch
+   29a1c6558:	add    (%rax),%al
    29a1c655a:	add    %al,0x30015201(%rip)        # 2ca1db761 <.debug_rnglists+0x3000b6bd>
    29a1c6560:	add    $0xa3035101,%eax
    29a1c6565:	add    %edx,0x5(%rdx)
    29a1c6568:	add    %ebx,0x3(%rax)
    29a1c656b:	movabs %eax,0x530015901055101
    29a1c6574:	add    0x20(%rdi),%dh
    29a1c6577:	add    0x10(%rcx),%dl
@@ -25817,18 +25769,16 @@
    29a1c93c8:	add    %al,(%rdx)
    29a1c93ca:	pop    %rdi
    29a1c93cb:	add    (%rax),%al
    29a1c93cd:	add    %al,(%rdx)
    29a1c93cf:	imul   $0x5020000,(%rdx),%eax
    29a1c93d5:	add    %eax,(%rax)
    29a1c93d7:	or     %eax,(%rdx)
-   29a1c93d9:	add    %dl,(%rbx,%rbx,1)
-   29a1c93dc:	(bad)
-   29a1c93dd:	add    (%rax),%al
-   29a1c93df:	add    %al,(%rax)
+   29a1c93d9:	loopne 29a1c93ee <.debug_line+0x71>
+   29a1c93db:	sbb    0x2(%rdx),%ebx
    29a1c93e1:	add    (%rcx,%rax,1),%edx
    29a1c93e4:	add    $0x5144b03,%eax
    29a1c93e9:	or     (%rcx),%al
    29a1c93eb:	add    $0x53e0807,%eax
    29a1c93f0:	or     %al,(%rsi)
    29a1c93f2:	add    %eax,0x52f0607(%rip)        # 29f4b99ff <.debug_rnglists+0x52e995b>
    29a1c93f8:	or     %al,(%rsi)
@@ -25980,18 +25930,16 @@
    29a1c9547:	push   %rsp
    29a1c9548:	add    $0x0,%al
    29a1c954a:	add    %al,(%rdx)
    29a1c954c:	pop    %rsp
    29a1c954d:	add    $0x0,%al
    29a1c954f:	add    %al,(%rdx)
    29a1c9551:	add    $0x2090001,%eax
-   29a1c9556:	rclb   $1,(%rbx,%rbx,1)
-   29a1c9559:	(bad)
-   29a1c955a:	add    (%rax),%al
-   29a1c955c:	add    %al,(%rax)
+   29a1c9556:	mov    $0x14,%al
+   29a1c9558:	sbb    0x2(%rdx),%ebx
    29a1c955e:	add    0x1060101(%rcx),%ecx
    29a1c9564:	add    $0x5500603,%eax
    29a1c9569:	(bad)
    29a1c956a:	(bad)
    29a1c956b:	add    %eax,-0x6fe6fcff(%rip)        # 22a359872 <__size_of_stack_reserve__+0x22a159872>
    29a1c9571:	add    $0x2c080603,%eax
    29a1c9576:	pop    %rcx
@@ -26145,15 +26093,16 @@
    29a1c96f8:	add    %dh,%dh
    29a1c96fa:	(bad)
    29a1c96fb:	add    %al,(%rax)
    29a1c96fd:	add    %bh,%bh
    29a1c96ff:	(bad)
    29a1c9700:	add    %al,(%rax)
    29a1c9702:	add    %al,0x2090001(%rip)        # 29c259709 <.debug_rnglists+0x2089665>
-   29a1c9708:	movabs 0x3000000029a1b15,%al
+   29a1c9708:	adcb   $0x0,0x29a1b(%rip)        # 29a1f312a <.debug_rnglists+0x23086>
+   29a1c970f:	add    %al,(%rbx)
    29a1c9711:	(bad)
    29a1c9712:	add    %al,(%rcx)
    29a1c9714:	(bad)
    29a1c9715:	add    %eax,0x3e030603(%rip)        # 2d81f9d1e <.debug_rnglists+0x3e029c7a>
    29a1c971b:	adc    0x41030601(%rip),%ax        # 2db1f9d23 <.debug_rnglists+0x41029c7f>
    29a1c9722:	add    %eax,0x3c3f0303(%rip)        # 2d65b9a2b <.debug_rnglists+0x3c3e9987>
    29a1c9728:	pop    %rdx
@@ -26261,26 +26210,27 @@
    29a1c986d:	pop    %rsp
    29a1c986e:	add    %eax,0x12030607(%rip)        # 2ac1f9e7b <.debug_rnglists+0x12029dd7>
    29a1c9874:	je     29a1c9879 <.debug_line+0x1f5>
    29a1c9876:	ja     29a1c9880 <.debug_line+0x1fc>
    29a1c9878:	sahf
    29a1c9879:	(bad)
    29a1c987a:	repnz add $0x9000601,%eax
-   29a1c9880:	add    0x29a1b17(%rax),%al
-   29a1c9886:	add    %al,(%rax)
-   29a1c9888:	add    %al,(%rbx)
-   29a1c988a:	movabs 0x15144b0803050102,%al
-   29a1c9893:	add    $0x5010607,%eax
-   29a1c9898:	(bad)
-   29a1c9899:	je     29a1c98a0 <.debug_line+0x21c>
-   29a1c989b:	add    %eax,(%rbx)
-   29a1c989d:	adc    %bl,0x5(%rax)
-   29a1c98a0:	add    (%rsi),%eax
-   29a1c98a2:	add    0x8(%rdx),%esi
-   29a1c98a5:	data16 movabs 0x5906030501060b05,%al
+   29a1c9880:	add    0x17(%rax),%ah
+   29a1c9883:	sbb    0x2(%rdx),%ebx
+   29a1c9889:	add    0x3050102(%rax),%esp
+   29a1c988f:	or     %cl,0x14(%rbx)
+   29a1c9892:	adc    $0x1060705,%eax
+   29a1c9897:	add    $0x1057406,%eax
+   29a1c989c:	add    (%rax),%edx
+   29a1c989e:	pop    %rax
+   29a1c989f:	add    $0x72030603,%eax
+   29a1c98a4:	or     %ah,-0x60(%rsi)
+   29a1c98a7:	add    $0x501060b,%eax
+   29a1c98ac:	add    (%rsi),%eax
+   29a1c98ae:	pop    %rcx
    29a1c98af:	add    $0x2e01061b,%eax
    29a1c98b4:	rex.WX add $0x7ec7030d,%rax
    29a1c98ba:	or     %dl,(%rdx)
    29a1c98bc:	add    $0x1ba030f,%eax
    29a1c98c1:	(bad)
    29a1c98c2:	add    $0xc059d1b,%eax
    29a1c98c7:	add    %al,(%rdx)
@@ -26578,16 +26528,18 @@
    29a1c9c63:	add    %al,(%rdx)
    29a1c9c65:	or     (%rax),%cl
    29a1c9c67:	add    %al,(%rax)
    29a1c9c69:	add    (%rsi),%bl
    29a1c9c6b:	or     %al,(%rax)
    29a1c9c6d:	add    %al,(%rdx)
    29a1c9c6f:	add    $0x2090001,%eax
-   29a1c9c74:	loopne 29a1c9c90 <.debug_line+0x8c>
-   29a1c9c76:	sbb    0x2(%rdx),%ebx
+   29a1c9c74:	rcrb   $0x1b,(%rdx)
+   29a1c9c77:	(bad)
+   29a1c9c78:	add    (%rax),%al
+   29a1c9c7a:	add    %al,(%rax)
    29a1c9c7c:	add    %edx,%esp
    29a1c9c7e:	add    %al,(%rcx)
    29a1c9c80:	add    $0x5f4a403,%eax
    29a1c9c85:	or     $0x1e050106,%eax
    29a1c9c8a:	add    %al,(%rdx)
    29a1c9c8c:	add    $0x1,%al
    29a1c9c8e:	(bad)
@@ -26844,16 +26796,15 @@
    29a1c9f3d:	pop    %rcx
    29a1c9f3e:	or     (%rax),%al
    29a1c9f40:	add    %al,(%rdx)
    29a1c9f42:	(bad)
    29a1c9f43:	or     (%rax),%al
    29a1c9f45:	add    %al,(%rdx)
    29a1c9f47:	add    $0x2090001,%eax
-   29a1c9f4c:	push   %rax
-   29a1c9f4d:	sbb    $0x29a1b,%eax
+   29a1c9f4c:	xor    %bl,0x29a1b(%rip)        # 29a1f396d <.debug_rnglists+0x238c9>
    29a1c9f52:	add    %al,(%rax)
    29a1c9f54:	add    (%rdi),%ecx
    29a1c9f56:	add    %eax,(%rsi)
    29a1c9f58:	add    %eax,0x13130603(%rip)        # 2ad2fa561 <.debug_rnglists+0x1312a4bd>
    29a1c9f5e:	adc    (%rbx,%rdx,1),%edx
    29a1c9f61:	add    $0x513060c,%eax
    29a1c9f66:	(bad)
@@ -27232,19 +27183,16 @@
    29a1ca468:	add    (%rdi),%cl
    29a1ca46a:	add    %bl,%dh
    29a1ca46c:	or     (%rax),%al
    29a1ca46e:	add    %al,(%rcx)
    29a1ca470:	decb   (%rdx)
    29a1ca472:	add    %al,(%rax)
    29a1ca474:	add    %eax,0x2090001(%rip)        # 29c25a47b <.debug_rnglists+0x208a3d7>
-   29a1ca47a:	push   %rax
-   29a1ca47b:	and    %ebx,(%rbx)
-   29a1ca47d:	(bad)
-   29a1ca47e:	add    (%rax),%al
-   29a1ca480:	add    %al,(%rax)
+   29a1ca47a:	xor    %ah,(%rcx)
+   29a1ca47c:	sbb    0x2(%rdx),%ebx
    29a1ca482:	add    (%rcx),%ecx
    29a1ca484:	add    %eax,0x1090303(%rip)        # 29b25a78d <.debug_rnglists+0x108a6e9>
    29a1ca48a:	add    $0x2330601,%eax
    29a1ca48f:	add    %eax,(%rax)
    29a1ca491:	add    %eax,(%rcx)
 
 000000029a1ca493 <.debug_line>:
@@ -27276,16 +27224,20 @@
    29a1ca4d1:	ret
    29a1ca4d2:	or     (%rax),%eax
    29a1ca4d4:	add    %al,(%rdx)
    29a1ca4d6:	iret
    29a1ca4d7:	or     (%rax),%eax
    29a1ca4d9:	add    %al,(%rdx)
    29a1ca4db:	add    $0x2090001,%eax
-   29a1ca4e0:	movabs 0x3000000029a1b21,%al
-   29a1ca4e9:	sgdt   (%rsi)
+   29a1ca4e0:	andb   $0x1b,(%rcx)
+   29a1ca4e3:	(bad)
+   29a1ca4e4:	add    (%rax),%al
+   29a1ca4e6:	add    %al,(%rax)
+   29a1ca4e8:	add    (%rdi),%ecx
+   29a1ca4ea:	add    %eax,(%rsi)
    29a1ca4ec:	add    %eax,0x5130603(%rip)        # 29f2faaf5 <.debug_rnglists+0x512aa51>
    29a1ca4f2:	add    %eax,(%rsi)
    29a1ca4f4:	adc    (%rdx),%eax
    29a1ca4f6:	(bad)
    29a1ca4f7:	add    %al,(%rcx)
    29a1ca4f9:	add    %esp,0x0(%rsi)
 
@@ -27317,15 +27269,15 @@
    29a1ca532:	add    %eax,-0x71ff0000(%rsp,%rcx,1)
    29a1ca539:	or     $0x0,%al
    29a1ca53b:	add    %al,(%rdx)
    29a1ca53d:	(bad)
    29a1ca53e:	or     $0x0,%al
    29a1ca540:	add    %al,(%rdx)
    29a1ca542:	movabs %al,0x90001050200000c
-   29a1ca54b:	add    0x29a1b21(%rax),%dh
+   29a1ca54b:	add    0x29a1b21(%rax),%dl
    29a1ca551:	add    %al,(%rax)
    29a1ca553:	add    %bl,(%rcx)
    29a1ca555:	(bad)
    29a1ca556:	add    %eax,0x5130603(%rip)        # 29f2fab5f <.debug_rnglists+0x512aabb>
    29a1ca55c:	add    %eax,(%rsi)
    29a1ca55e:	adc    (%rdx),%eax
    29a1ca560:	(bad)
@@ -27359,20 +27311,17 @@
    29a1ca59f:	add    %al,(%rax)
    29a1ca5a1:	add    %edi,0xd(%rcx)
    29a1ca5a4:	add    %al,(%rax)
    29a1ca5a6:	add    0x200000d(%rdx),%al
    29a1ca5ac:	mov    %cs,0x5020000(%rip)        # 29f1ea5b2 <.debug_rnglists+0x501a50e>
    29a1ca5b2:	add    %eax,(%rax)
    29a1ca5b4:	or     %eax,(%rdx)
-   29a1ca5b6:	shlb   $0x1b,(%rcx)
-   29a1ca5b9:	(bad)
-   29a1ca5ba:	add    (%rax),%al
-   29a1ca5bc:	add    %al,(%rax)
-   29a1ca5be:	add    (%rbx),%ecx
-   29a1ca5c0:	add    %eax,(%rsi)
+   29a1ca5b6:	movabs 0x3000000029a1b21,%al
+   29a1ca5bf:	or     (%rcx),%eax
+   29a1ca5c1:	(bad)
    29a1ca5c2:	add    %eax,0x54b0603(%rip)        # 29f67abcb <.debug_rnglists+0x54aab27>
    29a1ca5c8:	or     (%rsi),%al
    29a1ca5ca:	add    %ebp,0x5901052e(%rsp,%rdi,1)
    29a1ca5d1:	add    0x7c010100(%rip),%al        # 3161da6d7 <.debug_rnglists+0x7c00a633>
 
 000000029a1ca5d6 <.debug_line>:
    29a1ca5d6:	jl     29a1ca5da <.debug_line+0x4>
@@ -27425,16 +27374,18 @@
    29a1ca63f:	add    %edx,%ebx
    29a1ca641:	(bad)
    29a1ca642:	add    %al,(%rax)
    29a1ca644:	add    %ah,%ch
    29a1ca646:	(bad)
    29a1ca647:	add    %al,(%rax)
    29a1ca649:	add    0x2090001(%rip),%al        # 29c25a650 <.debug_rnglists+0x208a5ac>
-   29a1ca64f:	loopne 29a1ca672 <.debug_line+0x9c>
-   29a1ca651:	sbb    0x2(%rdx),%ebx
+   29a1ca64f:	shlb   $0x1b,(%rcx)
+   29a1ca652:	(bad)
+   29a1ca653:	add    (%rax),%al
+   29a1ca655:	add    %al,(%rax)
    29a1ca657:	add    %esi,%ebp
    29a1ca659:	add    %al,(%rcx)
    29a1ca65b:	add    $0x1051303,%eax
    29a1ca660:	(bad)
    29a1ca661:	adc    (%rsi),%eax
    29a1ca663:	add    -0xe(%rsi),%ecx
    29a1ca666:	(bad)
@@ -27532,16 +27483,16 @@
    29a1ca771:	add    %eax,0x1057406(%rip)        # 29b221b7d <.debug_rnglists+0x1051ad9>
    29a1ca777:	pop    %rbx
    29a1ca778:	add    $0x5490603,%eax
    29a1ca77d:	add    %eax,(%rsi)
    29a1ca77f:	adc    0x558110a(%rip),%eax        # 29f74b88f <.debug_rnglists+0x557b7eb>
    29a1ca785:	cmp    (%rsi),%al
    29a1ca787:	add    %cl,(%rcx)
-   29a1ca789:	add    (%rax),%dl
-   29a1ca78b:	and    (%rbx),%ebx
+   29a1ca789:	add    %al,%dh
+   29a1ca78b:	and    (%rbx),%bl
    29a1ca78d:	(bad)
    29a1ca78e:	add    (%rax),%al
    29a1ca790:	add    %al,(%rax)
    29a1ca792:	(bad)
    29a1ca793:	(bad)
    29a1ca794:	add    %eax,0x5590603(%rip)        # 29f75ad9d <.debug_rnglists+0x558acf9>
    29a1ca79a:	cmp    (%rsi),%al
@@ -27631,15 +27582,15 @@
    29a1ca88e:	add    %ebp,0x100000f(%rdi)
    29a1ca894:	mov    $0x200000f,%esi
    29a1ca899:	(bad)
    29a1ca89a:	sldt   (%rax)
    29a1ca89d:	add    %cl,%dl
    29a1ca89f:	sldt   (%rax)
    29a1ca8a2:	add    0x2090001(%rip),%al        # 29c25a8a9 <.debug_rnglists+0x208a805>
-   29a1ca8a8:	xor    %ah,0x29a1b(%rip)        # 29a1f42c9 <.debug_rnglists+0x24225>
+   29a1ca8a8:	add    %ah,0x29a1b(%rip)        # 29a1f42c9 <.debug_rnglists+0x24225>
    29a1ca8ae:	add    %al,(%rax)
    29a1ca8b0:	add    (%rbx),%ecx
    29a1ca8b2:	add    %eax,(%rsi)
    29a1ca8b4:	add    %eax,0x134b0603(%rip)        # 2ad67aebd <.debug_rnglists+0x134aae19>
    29a1ca8ba:	adc    0x5550601(%rip),%eax        # 29f71aec1 <.debug_rnglists+0x554ae1d>
    29a1ca8c0:	or     %ebx,0x5(%rsi,%riz,2)
    29a1ca8c4:	add    %esi,0x5(%rax)
@@ -27782,30 +27733,28 @@
    29a1cb115:	or     $0x7,%al
    29a1cb117:	or     %ah,0x1(%rax)
    29a1cb11d:	add    %al,(%rax)
    29a1cb11f:	add    %bl,(%rax,%rax,1)
    29a1cb122:	add    %al,(%rax)
    29a1cb124:	or     %al,(%rcx)
    29a1cb126:	add    %al,(%rax)
-   29a1cb128:	add    %dl,(%rbx,%rbx,1)
-   29a1cb12b:	(bad)
-   29a1cb12c:	add    (%rax),%al
-   29a1cb12e:	add    %al,(%rax)
+   29a1cb128:	loopne 29a1cb13d <.debug_frame+0x35>
+   29a1cb12a:	sbb    0x2(%rdx),%ebx
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
-   29a1cb148:	rex adc $0x1b,%al
+   29a1cb148:	and    %dl,(%rbx,%rbx,1)
    29a1cb14b:	(bad)
    29a1cb14c:	add    (%rax),%al
    29a1cb14e:	add    %al,(%rax)
    29a1cb150:	push   $0x0
    29a1cb152:	add    %al,(%rax)
    29a1cb154:	add    %al,(%rax)
    29a1cb156:	add    %al,(%rax)
@@ -27821,16 +27770,19 @@
    29a1cb171:	or     %cl,0xb(%rax)
    29a1cb174:	add    %al,(%rax)
    29a1cb176:	add    %al,(%rax)
    29a1cb178:	adc    $0x0,%al
    29a1cb17a:	add    %al,(%rax)
    29a1cb17c:	or     %al,(%rcx)
    29a1cb17e:	add    %al,(%rax)
-   29a1cb180:	mov    $0x14,%al
-   29a1cb182:	sbb    0x2(%rdx),%ebx
+   29a1cb180:	nop
+   29a1cb181:	adc    $0x1b,%al
+   29a1cb183:	(bad)
+   29a1cb184:	add    (%rax),%al
+   29a1cb186:	add    %al,(%rax)
    29a1cb188:	(bad)
    29a1cb189:	add    %al,(%rax)
    29a1cb18b:	add    %al,(%rax)
    29a1cb18d:	add    %al,(%rax)
 	...
 
 000000029a1cb190 <.debug_frame>:
@@ -27845,33 +27797,32 @@
    29a1cb19d:	or     $0x7,%al
    29a1cb19f:	or     %ah,0x1(%rax)
    29a1cb1a5:	add    %al,(%rax)
    29a1cb1a7:	add    %ah,(%rax,%rax,1)
    29a1cb1aa:	add    %al,(%rax)
    29a1cb1ac:	nop
    29a1cb1ad:	add    %eax,(%rax)
-   29a1cb1af:	add    %dl,%al
-   29a1cb1b1:	adc    $0x1b,%al
-   29a1cb1b3:	(bad)
-   29a1cb1b4:	add    (%rax),%al
-   29a1cb1b6:	add    %al,(%rax)
-   29a1cb1b8:	(bad)
+   29a1cb1af:	add    %dh,0x29a1b14(%rax)
+   29a1cb1b5:	add    %al,(%rax)
+   29a1cb1b7:	add    %ch,(%rdi)
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
-   29a1cb1d3:	add    %dl,0x1(%rax)
-   29a1cb1d9:	adc    $0x29a1b,%eax
+   29a1cb1d3:	add    %dl,-0x1fffffff(%rax)
+   29a1cb1d9:	adc    $0x1b,%al
+   29a1cb1db:	(bad)
+   29a1cb1dc:	add    (%rax),%al
    29a1cb1de:	add    %al,(%rax)
    29a1cb1e0:	addl   $0x0,(%rax)
    29a1cb1e6:	add    %al,(%rax)
    29a1cb1e8:	rex.B (bad)
    29a1cb1ea:	adc    %al,-0x7ce7f1bf(%rdx,%rax,1)
    29a1cb1f1:	add    0x40(%rsi,%rcx,1),%eax
    29a1cb1f5:	or     %gs:(%rsi),%cl
@@ -27894,20 +27845,19 @@
    29a1cb21a:	(bad)
    29a1cb21b:	or     %al,(%rax)
    29a1cb21d:	add    %al,(%rax)
    29a1cb21f:	add    %dl,(%rax,%rax,1)
    29a1cb222:	add    %al,(%rax)
    29a1cb224:	nop
    29a1cb225:	add    %eax,(%rax)
-   29a1cb227:	add    %dl,0x29a1b15(%rax)
-   29a1cb22d:	add    %al,(%rax)
-   29a1cb22f:	add    %al,(%rbx)
-   29a1cb231:	add    %al,(%rax)
-   29a1cb233:	add    %al,(%rax)
-   29a1cb235:	add    %al,(%rax)
+   29a1cb227:	add    %dh,0x15(%rax)
+   29a1cb22a:	sbb    0x2(%rdx),%ebx
+   29a1cb230:	add    (%rax),%eax
+   29a1cb232:	add    %al,(%rax)
+   29a1cb234:	add    %al,(%rax)
 	...
 
 000000029a1cb238 <.debug_frame>:
    29a1cb238:	adc    $0x0,%al
    29a1cb23a:	add    %al,(%rax)
    29a1cb23c:	(bad)
    29a1cb23d:	(bad)
@@ -27918,28 +27868,29 @@
    29a1cb245:	or     $0x7,%al
    29a1cb247:	or     %ah,0x1(%rax)
    29a1cb24d:	add    %al,(%rax)
    29a1cb24f:	add    %ah,(%rax,%rax,1)
    29a1cb252:	add    %al,(%rax)
    29a1cb254:	cmp    %al,(%rdx)
    29a1cb256:	add    %al,(%rax)
-   29a1cb258:	movabs 0x69000000029a1b15,%al
-   29a1cb261:	add    %al,(%rax)
-   29a1cb263:	add    %al,(%rax)
-   29a1cb265:	add    %al,(%rax)
-   29a1cb267:	add    %al,0xe(%rcx)
+   29a1cb258:	adcb   $0x0,0x29a1b(%rip)        # 29a1f4c7a <.debug_rnglists+0x24bd6>
+   29a1cb25f:	add    %ch,0x0(%rcx)
+   29a1cb262:	add    %al,(%rax)
+   29a1cb264:	add    %al,(%rax)
+   29a1cb266:	add    %al,(%rax)
+   29a1cb268:	rex.B (bad)
    29a1cb26a:	adc    %al,-0x7ce7f1bf(%rdx,%rax,1)
    29a1cb271:	add    0x50(%rsi,%rcx,1),%eax
    29a1cb275:	add    %al,(%rax)
    29a1cb277:	add    %bh,(%rax,%rax,1)
    29a1cb27a:	add    %al,(%rax)
    29a1cb27c:	cmp    %al,(%rdx)
    29a1cb27e:	add    %al,(%rax)
-   29a1cb280:	adc    %dl,(%rsi)
-   29a1cb282:	sbb    0x2(%rdx),%ebx
+   29a1cb280:	lock adc $0x29a1b,%eax
+   29a1cb286:	add    %al,(%rax)
    29a1cb288:	(bad)
    29a1cb28d:	add    %al,(%rax)
    29a1cb28f:	add    %al,0xe(%rcx)
    29a1cb292:	adc    %al,0x180e4102(%rbp)
    29a1cb298:	test   %al,(%rbx)
    29a1cb29a:	rex.B (bad)
    29a1cb29c:	and    %al,0x700e4404(%rbx)
@@ -27953,21 +27904,21 @@
    29a1cb2b1:	(bad)
    29a1cb2b2:	or     %al,0x0(%rbx,%rcx,1)
    29a1cb2b6:	add    %al,(%rax)
    29a1cb2b8:	pop    %rsp
    29a1cb2b9:	add    %al,(%rax)
    29a1cb2bb:	add    %bh,(%rax)
    29a1cb2bd:	add    (%rax),%al
-   29a1cb2bf:	add    %al,0x29a1b17(%rax)
-   29a1cb2c5:	add    %al,(%rax)
-   29a1cb2c7:	add    %bl,0x3(%rbp)
-   29a1cb2ca:	add    %al,(%rax)
-   29a1cb2cc:	add    %al,(%rax)
-   29a1cb2ce:	add    %al,(%rax)
-   29a1cb2d0:	rex.B (bad)
+   29a1cb2bf:	add    %ah,0x17(%rax)
+   29a1cb2c2:	sbb    0x2(%rdx),%ebx
+   29a1cb2c8:	pop    %rbp
+   29a1cb2c9:	add    (%rax),%eax
+   29a1cb2cb:	add    %al,(%rax)
+   29a1cb2cd:	add    %al,(%rax)
+   29a1cb2cf:	add    %al,0xe(%rcx)
    29a1cb2d2:	adc    %al,0x180e4202(%rsi)
    29a1cb2d8:	pop    (%rbx)
    29a1cb2da:	rex.X (bad)
    29a1cb2dc:	and    %cl,0x280e4204(%rsi)
    29a1cb2e2:	lea    -0x73cff1be(%rip),%eax        # 2264cc12a <__size_of_stack_reserve__+0x2262cc12a>
    29a1cb2e8:	(bad)
    29a1cb2e9:	rex.B (bad)
@@ -28002,15 +27953,15 @@
    29a1cb323:	js     29a1cb345 <.debug_frame+0x2d>
    29a1cb325:	or     $0x7,%al
    29a1cb327:	or     %ah,0x1(%rax)
    29a1cb32d:	add    %al,(%rax)
    29a1cb32f:	add    %cl,0x0(%rax,%rax,1)
    29a1cb333:	add    %bl,(%rax)
    29a1cb335:	add    (%rax),%eax
-   29a1cb337:	add    %ah,%al
+   29a1cb337:	add    %al,%al
    29a1cb339:	sbb    (%rbx),%bl
    29a1cb33b:	(bad)
    29a1cb33c:	add    (%rax),%al
    29a1cb33e:	add    %al,(%rax)
    29a1cb340:	jo     29a1cb342 <.debug_frame+0x2a>
    29a1cb342:	add    %al,(%rax)
    29a1cb344:	add    %al,(%rax)
@@ -28036,19 +27987,16 @@
    29a1cb37a:	(bad)
    29a1cb37b:	or     %al,(%rax)
    29a1cb37d:	add    %al,(%rax)
    29a1cb37f:	add    %bh,(%rax,%rax,1)
    29a1cb382:	add    %al,(%rax)
    29a1cb384:	sbb    %al,(%rbx)
    29a1cb386:	add    %al,(%rax)
-   29a1cb388:	push   %rax
-   29a1cb389:	sbb    (%rbx),%ebx
-   29a1cb38b:	(bad)
-   29a1cb38c:	add    (%rax),%al
-   29a1cb38e:	add    %al,(%rax)
+   29a1cb388:	xor    %bl,(%rbx)
+   29a1cb38a:	sbb    0x2(%rdx),%ebx
    29a1cb390:	outsl  %ds:(%rsi),(%dx)
    29a1cb391:	add    %al,(%rax)
    29a1cb393:	add    %al,(%rax)
    29a1cb395:	add    %al,(%rax)
    29a1cb397:	add    %al,0xe(%rcx)
    29a1cb39a:	adc    %al,0x180e4102(%rbp)
    29a1cb3a0:	test   %al,(%rbx)
@@ -28064,22 +28012,19 @@
    29a1cb3b8:	(bad)
    29a1cb3b9:	or     %al,0xb(%rcx)
    29a1cb3bc:	add    %al,(%rax)
    29a1cb3be:	add    %al,(%rax)
    29a1cb3c0:	add    %r8b,(%rax)
    29a1cb3c3:	add    %bl,(%rax)
    29a1cb3c5:	add    (%rax),%eax
-   29a1cb3c7:	add    %al,%al
-   29a1cb3c9:	sbb    (%rbx),%ebx
-   29a1cb3cb:	(bad)
-   29a1cb3cc:	add    (%rax),%al
-   29a1cb3ce:	add    %al,(%rax)
-   29a1cb3d0:	addl   $0x0,(%rax)
-   29a1cb3d6:	add    %al,(%rax)
-   29a1cb3d8:	rex.B (bad)
+   29a1cb3c7:	add    %ah,0x29a1b1b(%rax)
+   29a1cb3cd:	add    %al,(%rax)
+   29a1cb3cf:	add    %al,0x0(%rcx)
+   29a1cb3d5:	add    %al,(%rax)
+   29a1cb3d7:	add    %al,0xe(%rcx)
    29a1cb3da:	adc    %al,-0x7ce7f1bf(%rdx,%rax,1)
    29a1cb3e1:	add    0x40(%rsi,%rcx,1),%eax
    29a1cb3e5:	push   %rdx
    29a1cb3e6:	or     (%rsi),%cl
    29a1cb3e8:	sbb    %al,-0x3d(%rcx)
    29a1cb3eb:	(bad)
    29a1cb3ec:	adc    %al,-0x3c(%rcx)
@@ -28094,16 +28039,15 @@
    29a1cb3ff:	or     %al,0x0(%rbx,%rcx,1)
    29a1cb403:	add    %al,(%rax)
    29a1cb405:	add    %al,(%rax)
    29a1cb407:	add    %dh,(%rax,%rax,1)
    29a1cb40a:	add    %al,(%rax)
    29a1cb40c:	sbb    %al,(%rbx)
    29a1cb40e:	add    %al,(%rax)
-   29a1cb410:	push   %rax
-   29a1cb411:	sbb    $0x1b,%al
+   29a1cb410:	xor    %bl,(%rbx,%rbx,1)
    29a1cb413:	(bad)
    29a1cb414:	add    (%rax),%al
    29a1cb416:	add    %al,(%rax)
    29a1cb418:	repnz add %al,(%rax)
    29a1cb41b:	add    %al,(%rax)
    29a1cb41d:	add    %al,(%rax)
    29a1cb41f:	add    %al,0xe(%rcx)
@@ -28131,34 +28075,35 @@
    29a1cb44b:	js     29a1cb46d <.debug_frame+0x2d>
    29a1cb44d:	or     $0x7,%al
    29a1cb44f:	or     %ah,0x1(%rax)
    29a1cb455:	add    %al,(%rax)
    29a1cb457:	add    %dl,(%rax,%rax,1)
    29a1cb45a:	add    %al,(%rax)
    29a1cb45c:	rex add $0x0,%al
-   29a1cb45f:	add    %dl,0x1d(%rax)
-   29a1cb462:	sbb    0x2(%rdx),%ebx
+   29a1cb45f:	add    %dh,(%rax)
+   29a1cb461:	sbb    $0x29a1b,%eax
+   29a1cb466:	add    %al,(%rax)
    29a1cb468:	sub    $0x0,%al
    29a1cb46a:	add    %al,(%rax)
    29a1cb46c:	add    %al,(%rax)
    29a1cb46e:	add    %al,(%rax)
    29a1cb470:	adc    $0x0,%al
    29a1cb472:	add    %al,(%rax)
    29a1cb474:	rex add $0x0,%al
-   29a1cb477:	add    %al,0x29a1b1d(%rax)
-   29a1cb47d:	add    %al,(%rax)
-   29a1cb47f:	add    %dl,0x0(%rax)
-   29a1cb482:	add    %al,(%rax)
-   29a1cb484:	add    %al,(%rax)
-   29a1cb486:	add    %al,(%rax)
-   29a1cb488:	rex.WR add %r8b,(%rax)
+   29a1cb477:	add    %ah,0x1d(%rax)
+   29a1cb47a:	sbb    0x2(%rdx),%ebx
+   29a1cb480:	push   %rax
+   29a1cb481:	add    %al,(%rax)
+   29a1cb483:	add    %al,(%rax)
+   29a1cb485:	add    %al,(%rax)
+   29a1cb487:	add    %cl,0x0(%rax,%rax,1)
    29a1cb48b:	add    %al,0x4(%rax)
    29a1cb48e:	add    %al,(%rax)
-   29a1cb490:	rcrb   $1,0x29a1b(%rip)        # 29a1f4eb1 <.debug_rnglists+0x24e0d>
-   29a1cb496:	add    %al,(%rax)
+   29a1cb490:	mov    $0x1d,%al
+   29a1cb492:	sbb    0x2(%rdx),%ebx
    29a1cb498:	popf
    29a1cb499:	add    %al,(%rax)
    29a1cb49b:	add    %al,(%rax)
    29a1cb49d:	add    %al,(%rax)
    29a1cb49f:	add    %al,0xe(%rcx)
    29a1cb4a2:	adc    %al,0x180e4102(%rbp)
    29a1cb4a8:	test   %al,(%rbx)
@@ -28181,65 +28126,64 @@
    29a1cb4cf:	adc    %al,-0x3b(%rcx)
    29a1cb4d2:	(bad)
    29a1cb4d3:	or     %al,(%rax)
    29a1cb4d5:	add    %al,(%rax)
    29a1cb4d7:	add    %dl,(%rax,%rax,1)
    29a1cb4da:	add    %al,(%rax)
    29a1cb4dc:	rex add $0x0,%al
-   29a1cb4df:	add    %dh,0x1e(%rax)
+   29a1cb4df:	add    %dl,0x1e(%rax)
    29a1cb4e2:	sbb    0x2(%rdx),%ebx
    29a1cb4e8:	addb   $0x0,(%rax)
    29a1cb4eb:	add    %al,(%rax)
    29a1cb4ed:	add    %al,(%rax)
    29a1cb4ef:	add    %dl,(%rax,%rax,1)
    29a1cb4f2:	add    %al,(%rax)
    29a1cb4f4:	rex add $0x0,%al
-   29a1cb4f7:	add    %dh,%al
+   29a1cb4f7:	add    %dl,%al
    29a1cb4f9:	(bad)
    29a1cb4fa:	sbb    0x2(%rdx),%ebx
    29a1cb500:	(bad)
    29a1cb501:	add    %al,(%rax)
    29a1cb503:	add    %al,(%rax)
    29a1cb505:	add    %al,(%rax)
    29a1cb507:	add    %dl,(%rax,%rax,1)
    29a1cb50a:	add    %al,(%rax)
    29a1cb50c:	rex add $0x0,%al
-   29a1cb50f:	add    %dh,(%rax)
+   29a1cb50f:	add    %dl,(%rax)
    29a1cb511:	(bad)
    29a1cb512:	sbb    0x2(%rdx),%ebx
    29a1cb518:	jae    29a1cb51a <.debug_frame+0xda>
    29a1cb51a:	add    %al,(%rax)
    29a1cb51c:	add    %al,(%rax)
    29a1cb51e:	add    %al,(%rax)
    29a1cb520:	adc    $0x0,%al
    29a1cb522:	add    %al,(%rax)
    29a1cb524:	rex add $0x0,%al
-   29a1cb527:	add    %dh,0x29a1b1f(%rax)
+   29a1cb527:	add    %dl,0x29a1b1f(%rax)
    29a1cb52d:	add    %al,(%rax)
    29a1cb52f:	add    %dh,(%rsi)
    29a1cb531:	add    %al,(%rax)
    29a1cb533:	add    %al,(%rax)
    29a1cb535:	add    %al,(%rax)
    29a1cb537:	add    %dl,(%rax,%rax,1)
    29a1cb53a:	add    %al,(%rax)
    29a1cb53c:	rex add $0x0,%al
-   29a1cb53f:	add    %dh,%al
+   29a1cb53f:	add    %dl,%al
    29a1cb541:	(bad)
    29a1cb542:	sbb    0x2(%rdx),%ebx
    29a1cb548:	mov    %eax,(%rax)
    29a1cb54a:	add    %al,(%rax)
    29a1cb54c:	add    %al,(%rax)
    29a1cb54e:	add    %al,(%rax)
    29a1cb550:	adc    $0x0,%al
    29a1cb552:	add    %al,(%rax)
    29a1cb554:	rex add $0x0,%al
-   29a1cb557:	add    %al,0x29a1b20(%rax)
-   29a1cb55d:	add    %al,(%rax)
-   29a1cb55f:	add    %al,%dh
-   29a1cb561:	add    %al,(%rax)
+   29a1cb557:	add    %ah,0x20(%rax)
+   29a1cb55a:	sbb    0x2(%rdx),%ebx
+   29a1cb560:	movb   $0x0,(%rax)
    29a1cb563:	add    %al,(%rax)
    29a1cb565:	add    %al,(%rax)
 	...
 
 000000029a1cb568 <.debug_frame>:
    29a1cb568:	adc    $0x0,%al
    29a1cb56a:	add    %al,(%rax)
@@ -28250,15 +28194,15 @@
    29a1cb571:	add    %al,(%rcx)
    29a1cb573:	js     29a1cb595 <.debug_frame+0x2d>
    29a1cb575:	or     $0x7,%al
    29a1cb577:	or     %ah,0x1(%rax)
    29a1cb57d:	add    %al,(%rax)
    29a1cb57f:	add    %dl,(%rax,%rax,1)
    29a1cb582:	add    %al,(%rax)
-   29a1cb584:	push   $0x50000005
+   29a1cb584:	push   $0x30000005
    29a1cb589:	and    %ebx,(%rbx)
    29a1cb58b:	(bad)
    29a1cb58c:	add    (%rax),%al
    29a1cb58e:	add    %al,(%rax)
    29a1cb590:	add    (%rax),%eax
    29a1cb592:	add    %al,(%rax)
    29a1cb594:	add    %al,(%rax)
@@ -28275,15 +28219,15 @@
    29a1cb5a3:	js     29a1cb5c5 <.debug_frame+0x2d>
    29a1cb5a5:	or     $0x7,%al
    29a1cb5a7:	or     %ah,0x1(%rax)
    29a1cb5ad:	add    %al,(%rax)
    29a1cb5af:	add    %dl,(%rax,%rax,1)
    29a1cb5b2:	add    %al,(%rax)
    29a1cb5b4:	cwtl
-   29a1cb5b5:	add    $0x21a00000,%eax
+   29a1cb5b5:	add    $0x21800000,%eax
    29a1cb5ba:	sbb    0x2(%rdx),%ebx
    29a1cb5c0:	(bad)
    29a1cb5c1:	add    %al,(%rax)
    29a1cb5c3:	add    %al,(%rax)
    29a1cb5c5:	add    %al,(%rax)
 	...
 
@@ -28298,16 +28242,19 @@
    29a1cb5d3:	js     29a1cb5f5 <.debug_frame+0x2d>
    29a1cb5d5:	or     $0x7,%al
    29a1cb5d7:	or     %ah,0x1(%rax)
    29a1cb5dd:	add    %al,(%rax)
    29a1cb5df:	add    %dl,(%rax,%rax,1)
    29a1cb5e2:	add    %al,(%rax)
    29a1cb5e4:	enter  $0x5,$0x0
-   29a1cb5e8:	mov    $0x21,%al
-   29a1cb5ea:	sbb    0x2(%rdx),%ebx
+   29a1cb5e8:	nop
+   29a1cb5e9:	and    %ebx,(%rbx)
+   29a1cb5eb:	(bad)
+   29a1cb5ec:	add    (%rax),%al
+   29a1cb5ee:	add    %al,(%rax)
    29a1cb5f0:	(bad)
    29a1cb5f1:	add    %al,(%rax)
    29a1cb5f3:	add    %al,(%rax)
    29a1cb5f5:	add    %al,(%rax)
 	...
 
 000000029a1cb5f8 <.debug_frame>:
@@ -28321,15 +28268,15 @@
    29a1cb603:	js     29a1cb625 <.debug_frame+0x2d>
    29a1cb605:	or     $0x7,%al
    29a1cb607:	or     %ah,0x1(%rax)
    29a1cb60d:	add    %al,(%rax)
    29a1cb60f:	add    %bl,(%rax,%rax,1)
    29a1cb612:	add    %al,(%rax)
    29a1cb614:	clc
-   29a1cb615:	add    $0x21c00000,%eax
+   29a1cb615:	add    $0x21a00000,%eax
    29a1cb61a:	sbb    0x2(%rdx),%ebx
    29a1cb620:	(bad)
    29a1cb621:	add    %al,(%rax)
    29a1cb623:	add    %al,(%rax)
    29a1cb625:	add    %al,(%rax)
    29a1cb627:	add    %al,0x40(%rsi,%rcx,1)
    29a1cb62b:	pop    %rcx
@@ -28349,28 +28296,28 @@
    29a1cb63d:	or     $0x7,%al
    29a1cb63f:	or     %ah,0x1(%rax)
    29a1cb645:	add    %al,(%rax)
    29a1cb647:	add    %dl,(%rax,%rax,1)
    29a1cb64a:	add    %al,(%rax)
    29a1cb64c:	xor    %al,(%rsi)
    29a1cb64e:	add    %al,(%rax)
-   29a1cb650:	loopne 29a1cb673 <.debug_frame+0x43>
-   29a1cb652:	sbb    0x2(%rdx),%ebx
+   29a1cb650:	shlb   $0x1b,(%rcx)
+   29a1cb653:	(bad)
+   29a1cb654:	add    (%rax),%al
+   29a1cb656:	add    %al,(%rax)
    29a1cb658:	add    (%rax),%eax
    29a1cb65a:	add    %al,(%rax)
    29a1cb65c:	add    %al,(%rax)
    29a1cb65e:	add    %al,(%rax)
    29a1cb660:	rex.WR add %r8b,(%rax)
    29a1cb663:	add    %dh,(%rax)
    29a1cb665:	(bad)
    29a1cb666:	add    %al,(%rax)
-   29a1cb668:	lock and %ebx,(%rbx)
-   29a1cb66b:	(bad)
-   29a1cb66c:	add    (%rax),%al
-   29a1cb66e:	add    %al,(%rax)
+   29a1cb668:	shlb   $1,(%rcx)
+   29a1cb66a:	sbb    0x2(%rdx),%ebx
    29a1cb670:	push   $0x0
    29a1cb672:	add    %al,(%rax)
    29a1cb674:	add    %al,(%rax)
    29a1cb676:	add    %al,(%rax)
    29a1cb678:	rex.X (bad)
    29a1cb67a:	adc    %cl,-0x79e7f1bf(%rdx,%rax,1)
    29a1cb681:	add    0xe(%rcx),%eax
@@ -28392,16 +28339,15 @@
    29a1cb6aa:	(bad)
    29a1cb6ab:	or     %al,(%rax)
    29a1cb6ad:	add    %al,(%rax)
    29a1cb6af:	add    %cl,0x0(%rax,%rax,1)
    29a1cb6b3:	add    %dh,(%rax)
    29a1cb6b5:	(bad)
    29a1cb6b6:	add    %al,(%rax)
-   29a1cb6b8:	(bad)
-   29a1cb6b9:	and    (%rbx),%bl
+   29a1cb6b8:	rex and (%rbx),%bl
    29a1cb6bb:	(bad)
    29a1cb6bc:	add    (%rax),%al
    29a1cb6be:	add    %al,(%rax)
    29a1cb6c0:	push   $0x0
    29a1cb6c2:	add    %al,(%rax)
    29a1cb6c4:	add    %al,(%rax)
    29a1cb6c6:	add    %al,(%rax)
@@ -28426,15 +28372,15 @@
    29a1cb6fa:	(bad)
    29a1cb6fb:	or     %al,(%rax)
    29a1cb6fd:	add    %al,(%rax)
    29a1cb6ff:	add    %ah,(%rax,%rax,1)
    29a1cb702:	add    %al,(%rax)
    29a1cb704:	xor    %al,(%rsi)
    29a1cb706:	add    %al,(%rax)
-   29a1cb708:	shlb   $1,(%rdx)
+   29a1cb708:	mov    $0x22,%al
    29a1cb70a:	sbb    0x2(%rdx),%ebx
    29a1cb710:	(bad)
    29a1cb711:	add    %al,(%rax)
    29a1cb713:	add    %al,(%rax)
    29a1cb715:	add    %al,(%rax)
    29a1cb717:	add    %al,0xe(%rcx)
    29a1cb71a:	adc    %al,0x300e4402(%rbx)
@@ -28443,67 +28389,63 @@
    29a1cb722:	adc    %al,-0x3d(%rcx)
    29a1cb725:	(bad)
    29a1cb726:	or     %al,(%rax)
    29a1cb728:	adc    $0x0,%al
    29a1cb72a:	add    %al,(%rax)
    29a1cb72c:	xor    %al,(%rsi)
    29a1cb72e:	add    %al,(%rax)
-   29a1cb730:	lock and (%rbx),%bl
-   29a1cb733:	(bad)
-   29a1cb734:	add    (%rax),%al
-   29a1cb736:	add    %al,(%rax)
+   29a1cb730:	shlb   $1,(%rdx)
+   29a1cb732:	sbb    0x2(%rdx),%ebx
    29a1cb738:	adc    $0x0,%eax
    29a1cb73d:	add    %al,(%rax)
    29a1cb73f:	add    %bl,(%rax,%rax,1)
    29a1cb742:	add    %al,(%rax)
    29a1cb744:	xor    %al,(%rsi)
    29a1cb746:	add    %al,(%rax)
-   29a1cb748:	adc    %ah,(%rbx)
-   29a1cb74a:	sbb    0x2(%rdx),%ebx
+   29a1cb748:	lock and (%rbx),%bl
+   29a1cb74b:	(bad)
+   29a1cb74c:	add    (%rax),%al
+   29a1cb74e:	add    %al,(%rax)
    29a1cb750:	cs add %al,(%rax)
    29a1cb753:	add    %al,(%rax)
    29a1cb755:	add    %al,(%rax)
    29a1cb757:	add    %al,0xe(%rcx)
    29a1cb75a:	adc    %al,0x300e4402(%rbx)
    29a1cb760:	sbb    $0x0,%al
    29a1cb762:	add    %al,(%rax)
    29a1cb764:	xor    %al,(%rsi)
    29a1cb766:	add    %al,(%rax)
-   29a1cb768:	rex and (%rbx),%ebx
-   29a1cb76b:	(bad)
-   29a1cb76c:	add    (%rax),%al
-   29a1cb76e:	add    %al,(%rax)
+   29a1cb768:	and    %ah,(%rbx)
+   29a1cb76a:	sbb    0x2(%rdx),%ebx
    29a1cb770:	xor    $0x0,%eax
    29a1cb775:	add    %al,(%rax)
    29a1cb777:	add    %al,0x50(%rsi,%rcx,1)
    29a1cb77b:	jo     29a1cb78b <.debug_frame+0x15b>
    29a1cb77d:	or     %al,(%rax)
    29a1cb77f:	add    %bl,(%rax,%rax,1)
    29a1cb782:	add    %al,(%rax)
    29a1cb784:	xor    %al,(%rsi)
    29a1cb786:	add    %al,(%rax)
-   29a1cb788:	andb   $0x1b,(%rbx)
+   29a1cb788:	(bad)
+   29a1cb789:	and    (%rbx),%ebx
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
-   29a1cb7a8:	shlb   $0x1b,(%rbx)
-   29a1cb7ab:	(bad)
-   29a1cb7ac:	add    (%rax),%al
-   29a1cb7ae:	add    %al,(%rax)
-   29a1cb7b0:	ss add %al,(%rax)
+   29a1cb7a8:	movabs 0x36000000029a1b23,%al
+   29a1cb7b1:	add    %al,(%rax)
    29a1cb7b3:	add    %al,(%rax)
    29a1cb7b5:	add    %al,(%rax)
    29a1cb7b7:	add    %al,0x30(%rsi,%rcx,1)
    29a1cb7bb:	jno    29a1cb7cb <.debug_frame+0xb>
    29a1cb7bd:	or     %al,(%rax)
 	...
 
@@ -28518,15 +28460,15 @@
    29a1cb7cb:	js     29a1cb7ed <.debug_frame+0x2d>
    29a1cb7cd:	or     $0x7,%al
    29a1cb7cf:	or     %ah,0x1(%rax)
    29a1cb7d5:	add    %al,(%rax)
    29a1cb7d7:	add    %bl,(%rax,%rax,1)
    29a1cb7da:	add    %al,(%rax)
    29a1cb7dc:	rolb   $0x0,(%rdi)
-   29a1cb7df:	add    %dh,(%rax)
+   29a1cb7df:	add    %al,(%rax)
    29a1cb7e1:	and    $0x29a1b,%eax
    29a1cb7e6:	add    %al,(%rax)
    29a1cb7e8:	xor    (%rax),%al
    29a1cb7ea:	add    %al,(%rax)
    29a1cb7ec:	add    %al,(%rax)
    29a1cb7ee:	add    %al,(%rax)
    29a1cb7f0:	rex.R (bad)
```

### Comparing `advanced_input-0.2.0/advanced_input/inputExtention.so` & `advanced_input-0.2.1/advanced_input/inputExtention.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 14% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          14240 (bytes into file)
+  Start of section headers:          14144 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         11
   Size of section headers:           64 (bytes)
   Number of section headers:         29
   Section header string table index: 28
```

#### readelf --wide --program-header {}

```diff
@@ -1,25 +1,25 @@
 
 Elf file type is DYN (Shared object file)
 Entry point 0x0
 There are 11 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x0007e8 0x0007e8 R   0x1000
-  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000485 0x000485 R E 0x1000
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000778 0x000778 R   0x1000
+  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000451 0x000451 R E 0x1000
   LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x0001b4 0x0001b4 R   0x1000
-  LOAD           0x002e08 0x0000000000003e08 0x0000000000003e08 0x000268 0x000318 RW  0x1000
-  DYNAMIC        0x002e18 0x0000000000003e18 0x0000000000003e18 0x0001c0 0x0001c0 RW  0x8
+  LOAD           0x002e10 0x0000000000003e10 0x0000000000003e10 0x000258 0x000310 RW  0x1000
+  DYNAMIC        0x002e20 0x0000000000003e20 0x0000000000003e20 0x0001c0 0x0001c0 RW  0x8
   NOTE           0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   NOTE           0x0002c8 0x00000000000002c8 0x00000000000002c8 0x000024 0x000024 R   0x4
   GNU_PROPERTY   0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   GNU_EH_FRAME   0x002000 0x0000000000002000 0x0000000000002000 0x00005c 0x00005c R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
-  GNU_RELRO      0x002e08 0x0000000000003e08 0x0000000000003e08 0x0001f8 0x0001f8 R   0x1
+  GNU_RELRO      0x002e10 0x0000000000003e10 0x0000000000003e10 0x0001f0 0x0001f0 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     .note.gnu.property .note.gnu.build-id .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt 
    01     .init .plt .plt.got .plt.sec .text .fini 
    02     .eh_frame_hdr .eh_frame 
    03     .init_array .fini_array .dynamic .got .got.plt .data .bss
```

#### readelf --wide --sections {}

```diff
@@ -1,38 +1,38 @@
-There are 29 section headers, starting at offset 0x37a0:
+There are 29 section headers, starting at offset 0x3740:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.property NOTE            00000000000002a8 0002a8 000020 00   A  0   0  8
   [ 2] .note.gnu.build-id NOTE            00000000000002c8 0002c8 000024 00   A  0   0  4
   [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 000040 00   A  4   0  8
-  [ 4] .dynsym           DYNSYM          0000000000000330 000330 0001c8 18   A  5   1  8
-  [ 5] .dynstr           STRTAB          00000000000004f8 0004f8 0000e9 00   A  0   0  1
-  [ 6] .gnu.version      VERSYM          00000000000005e2 0005e2 000026 02   A  4   0  2
-  [ 7] .gnu.version_r    VERNEED         0000000000000608 000608 000030 00   A  5   1  8
-  [ 8] .rela.dyn         RELA            0000000000000638 000638 0000c0 18   A  4   0  8
-  [ 9] .rela.plt         RELA            00000000000006f8 0006f8 0000f0 18  AI  4  22  8
+  [ 4] .dynsym           DYNSYM          0000000000000330 000330 000198 18   A  5   1  8
+  [ 5] .dynstr           STRTAB          00000000000004c8 0004c8 0000dc 00   A  0   0  1
+  [ 6] .gnu.version      VERSYM          00000000000005a4 0005a4 000022 02   A  4   0  2
+  [ 7] .gnu.version_r    VERNEED         00000000000005c8 0005c8 000030 00   A  5   1  8
+  [ 8] .rela.dyn         RELA            00000000000005f8 0005f8 0000a8 18   A  4   0  8
+  [ 9] .rela.plt         RELA            00000000000006a0 0006a0 0000d8 18  AI  4  22  8
   [10] .init             PROGBITS        0000000000001000 001000 00001b 00  AX  0   0  4
-  [11] .plt              PROGBITS        0000000000001020 001020 0000b0 10  AX  0   0 16
-  [12] .plt.got          PROGBITS        00000000000010d0 0010d0 000010 10  AX  0   0 16
-  [13] .plt.sec          PROGBITS        00000000000010e0 0010e0 0000a0 10  AX  0   0 16
-  [14] .text             PROGBITS        0000000000001180 001180 0002f5 00  AX  0   0 16
-  [15] .fini             PROGBITS        0000000000001478 001478 00000d 00  AX  0   0  4
+  [11] .plt              PROGBITS        0000000000001020 001020 0000a0 10  AX  0   0 16
+  [12] .plt.got          PROGBITS        00000000000010c0 0010c0 000010 10  AX  0   0 16
+  [13] .plt.sec          PROGBITS        00000000000010d0 0010d0 000090 10  AX  0   0 16
+  [14] .text             PROGBITS        0000000000001160 001160 0002e3 00  AX  0   0 16
+  [15] .fini             PROGBITS        0000000000001444 001444 00000d 00  AX  0   0  4
   [16] .eh_frame_hdr     PROGBITS        0000000000002000 002000 00005c 00   A  0   0  4
   [17] .eh_frame         PROGBITS        0000000000002060 002060 000154 00   A  0   0  8
-  [18] .init_array       INIT_ARRAY      0000000000003e08 002e08 000008 08  WA  0   0  8
-  [19] .fini_array       FINI_ARRAY      0000000000003e10 002e10 000008 08  WA  0   0  8
-  [20] .dynamic          DYNAMIC         0000000000003e18 002e18 0001c0 10  WA  5   0  8
-  [21] .got              PROGBITS        0000000000003fd8 002fd8 000028 08  WA  0   0  8
-  [22] .got.plt          PROGBITS        0000000000004000 003000 000068 08  WA  0   0  8
-  [23] .data             PROGBITS        0000000000004068 003068 000008 00  WA  0   0  8
-  [24] .bss              NOBITS          0000000000004080 003070 0000a0 00  WA  0   0 32
-  [25] .comment          PROGBITS        0000000000000000 003070 00002b 01  MS  0   0  1
-  [26] .symtab           SYMTAB          0000000000000000 0030a0 0003c0 18     27  22  8
-  [27] .strtab           STRTAB          0000000000000000 003460 000236 00      0   0  1
-  [28] .shstrtab         STRTAB          0000000000000000 003696 000105 00      0   0  1
+  [18] .init_array       INIT_ARRAY      0000000000003e10 002e10 000008 08  WA  0   0  8
+  [19] .fini_array       FINI_ARRAY      0000000000003e18 002e18 000008 08  WA  0   0  8
+  [20] .dynamic          DYNAMIC         0000000000003e20 002e20 0001c0 10  WA  5   0  8
+  [21] .got              PROGBITS        0000000000003fe0 002fe0 000020 08  WA  0   0  8
+  [22] .got.plt          PROGBITS        0000000000004000 003000 000060 08  WA  0   0  8
+  [23] .data             PROGBITS        0000000000004060 003060 000008 00  WA  0   0  8
+  [24] .bss              NOBITS          0000000000004080 003068 0000a0 00  WA  0   0 32
+  [25] .comment          PROGBITS        0000000000000000 003068 00002b 01  MS  0   0  1
+  [26] .symtab           SYMTAB          0000000000000000 003098 000390 18     27  22  8
+  [27] .strtab           STRTAB          0000000000000000 003428 000211 00      0   0  1
+  [28] .shstrtab         STRTAB          0000000000000000 003639 000105 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -1,65 +1,61 @@
 
-Symbol table '.dynsym' contains 19 entries:
+Symbol table '.dynsym' contains 17 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-     2: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND stdin@GLIBC_2.2.5 (2)
-     3: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4 (3)
-     4: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND ioctl@GLIBC_2.2.5 (2)
-     5: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND read@GLIBC_2.2.5 (2)
-     6: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-     7: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fflush@GLIBC_2.2.5 (2)
-     8: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND tcgetattr@GLIBC_2.2.5 (2)
-     9: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND tcsetattr@GLIBC_2.2.5 (2)
-    10: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-    11: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (2)
-    12: 000000000000141f    20 FUNC    GLOBAL DEFAULT   14 isInputReady
-    13: 0000000000001451    36 FUNC    GLOBAL DEFAULT   14 stop
-    14: 0000000000001239    36 FUNC    GLOBAL DEFAULT   14 resume
-    15: 000000000000125d   107 FUNC    GLOBAL DEFAULT   14 kbhit
-    16: 0000000000001358   199 FUNC    GLOBAL DEFAULT   14 init
-    17: 00000000000012c8   144 FUNC    GLOBAL DEFAULT   14 getch
-    18: 0000000000001433    30 FUNC    GLOBAL DEFAULT   14 getCharacter
+     2: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4 (2)
+     3: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND ioctl@GLIBC_2.2.5 (3)
+     4: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND read@GLIBC_2.2.5 (3)
+     5: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+     6: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND tcgetattr@GLIBC_2.2.5 (3)
+     7: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND tcsetattr@GLIBC_2.2.5 (3)
+     8: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+     9: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (3)
+    10: 00000000000013ed    20 FUNC    GLOBAL DEFAULT   14 isInputReady
+    11: 000000000000141f    36 FUNC    GLOBAL DEFAULT   14 stop
+    12: 0000000000001219    36 FUNC    GLOBAL DEFAULT   14 resume
+    13: 000000000000123d   107 FUNC    GLOBAL DEFAULT   14 kbhit
+    14: 0000000000001338   181 FUNC    GLOBAL DEFAULT   14 init
+    15: 00000000000012a8   144 FUNC    GLOBAL DEFAULT   14 getch
+    16: 0000000000001401    30 FUNC    GLOBAL DEFAULT   14 getCharacter
 
-Symbol table '.symtab' contains 40 entries:
+Symbol table '.symtab' contains 38 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-     2: 0000000000001180     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
-     3: 00000000000011b0     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
-     4: 00000000000011f0     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
+     2: 0000000000001160     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
+     3: 0000000000001190     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
+     4: 00000000000011d0     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
      5: 0000000000004080     1 OBJECT  LOCAL  DEFAULT   24 completed.0
-     6: 0000000000003e10     0 OBJECT  LOCAL  DEFAULT   19 __do_global_dtors_aux_fini_array_entry
-     7: 0000000000001230     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
-     8: 0000000000003e08     0 OBJECT  LOCAL  DEFAULT   18 __frame_dummy_init_array_entry
+     6: 0000000000003e18     0 OBJECT  LOCAL  DEFAULT   19 __do_global_dtors_aux_fini_array_entry
+     7: 0000000000001210     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
+     8: 0000000000003e10     0 OBJECT  LOCAL  DEFAULT   18 __frame_dummy_init_array_entry
      9: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS inputExtention.c
     10: 00000000000040a0    60 OBJECT  LOCAL  DEFAULT   24 oldt
     11: 00000000000040e0    60 OBJECT  LOCAL  DEFAULT   24 newt
     12: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
     13: 00000000000021b0     0 OBJECT  LOCAL  DEFAULT   17 __FRAME_END__
     14: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
-    15: 0000000000001478     0 FUNC    LOCAL  DEFAULT   15 _fini
-    16: 0000000000004068     0 OBJECT  LOCAL  DEFAULT   23 __dso_handle
-    17: 0000000000003e18     0 OBJECT  LOCAL  DEFAULT   20 _DYNAMIC
+    15: 0000000000001444     0 FUNC    LOCAL  DEFAULT   15 _fini
+    16: 0000000000004060     0 OBJECT  LOCAL  DEFAULT   23 __dso_handle
+    17: 0000000000003e20     0 OBJECT  LOCAL  DEFAULT   20 _DYNAMIC
     18: 0000000000002000     0 NOTYPE  LOCAL  DEFAULT   16 __GNU_EH_FRAME_HDR
-    19: 0000000000004070     0 OBJECT  LOCAL  DEFAULT   23 __TMC_END__
+    19: 0000000000004068     0 OBJECT  LOCAL  DEFAULT   23 __TMC_END__
     20: 0000000000004000     0 OBJECT  LOCAL  DEFAULT   22 _GLOBAL_OFFSET_TABLE_
     21: 0000000000001000     0 FUNC    LOCAL  DEFAULT   10 _init
     22: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-    23: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND stdin@GLIBC_2.2.5
-    24: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4
-    25: 000000000000141f    20 FUNC    GLOBAL DEFAULT   14 isInputReady
-    26: 000000000000125d   107 FUNC    GLOBAL DEFAULT   14 kbhit
-    27: 0000000000001451    36 FUNC    GLOBAL DEFAULT   14 stop
-    28: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND ioctl@GLIBC_2.2.5
-    29: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND read@GLIBC_2.2.5
-    30: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-    31: 0000000000001239    36 FUNC    GLOBAL DEFAULT   14 resume
-    32: 0000000000001358   199 FUNC    GLOBAL DEFAULT   14 init
-    33: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fflush@GLIBC_2.2.5
-    34: 00000000000012c8   144 FUNC    GLOBAL DEFAULT   14 getch
-    35: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND tcgetattr@GLIBC_2.2.5
-    36: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND tcsetattr@GLIBC_2.2.5
-    37: 0000000000001433    30 FUNC    GLOBAL DEFAULT   14 getCharacter
-    38: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-    39: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
+    23: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4
+    24: 00000000000013ed    20 FUNC    GLOBAL DEFAULT   14 isInputReady
+    25: 000000000000123d   107 FUNC    GLOBAL DEFAULT   14 kbhit
+    26: 000000000000141f    36 FUNC    GLOBAL DEFAULT   14 stop
+    27: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND ioctl@GLIBC_2.2.5
+    28: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND read@GLIBC_2.2.5
+    29: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+    30: 0000000000001219    36 FUNC    GLOBAL DEFAULT   14 resume
+    31: 0000000000001338   181 FUNC    GLOBAL DEFAULT   14 init
+    32: 00000000000012a8   144 FUNC    GLOBAL DEFAULT   14 getch
+    33: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND tcgetattr@GLIBC_2.2.5
+    34: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND tcsetattr@GLIBC_2.2.5
+    35: 0000000000001401    30 FUNC    GLOBAL DEFAULT   14 getCharacter
+    36: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+    37: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
```

#### readelf --wide --relocs {}

```diff
@@ -1,24 +1,22 @@
 
-Relocation section '.rela.dyn' at offset 0x638 contains 8 entries:
+Relocation section '.rela.dyn' at offset 0x5f8 contains 7 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000003e08  0000000000000008 R_X86_64_RELATIVE                         1230
-0000000000003e10  0000000000000008 R_X86_64_RELATIVE                         11f0
-0000000000004068  0000000000000008 R_X86_64_RELATIVE                         4068
-0000000000003fd8  0000000100000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
-0000000000003fe0  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 stdin@GLIBC_2.2.5 + 0
-0000000000003fe8  0000000600000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
-0000000000003ff0  0000000a00000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
-0000000000003ff8  0000000b00000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
+0000000000003e10  0000000000000008 R_X86_64_RELATIVE                         1210
+0000000000003e18  0000000000000008 R_X86_64_RELATIVE                         11d0
+0000000000004060  0000000000000008 R_X86_64_RELATIVE                         4060
+0000000000003fe0  0000000100000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
+0000000000003fe8  0000000500000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
+0000000000003ff0  0000000800000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+0000000000003ff8  0000000900000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
 
-Relocation section '.rela.plt' at offset 0x6f8 contains 10 entries:
+Relocation section '.rela.plt' at offset 0x6a0 contains 9 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000004018  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 __stack_chk_fail@GLIBC_2.4 + 0
-0000000000004020  0000000f00000007 R_X86_64_JUMP_SLOT     000000000000125d kbhit + 0
-0000000000004028  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000001451 stop + 0
-0000000000004030  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 ioctl@GLIBC_2.2.5 + 0
-0000000000004038  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 read@GLIBC_2.2.5 + 0
-0000000000004040  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000001239 resume + 0
-0000000000004048  0000000700000007 R_X86_64_JUMP_SLOT     0000000000000000 fflush@GLIBC_2.2.5 + 0
-0000000000004050  0000001100000007 R_X86_64_JUMP_SLOT     00000000000012c8 getch + 0
-0000000000004058  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 tcgetattr@GLIBC_2.2.5 + 0
-0000000000004060  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 tcsetattr@GLIBC_2.2.5 + 0
+0000000000004018  0000000200000007 R_X86_64_JUMP_SLOT     0000000000000000 __stack_chk_fail@GLIBC_2.4 + 0
+0000000000004020  0000000d00000007 R_X86_64_JUMP_SLOT     000000000000123d kbhit + 0
+0000000000004028  0000000b00000007 R_X86_64_JUMP_SLOT     000000000000141f stop + 0
+0000000000004030  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 ioctl@GLIBC_2.2.5 + 0
+0000000000004038  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 read@GLIBC_2.2.5 + 0
+0000000000004040  0000000c00000007 R_X86_64_JUMP_SLOT     0000000000001219 resume + 0
+0000000000004048  0000000f00000007 R_X86_64_JUMP_SLOT     00000000000012a8 getch + 0
+0000000000004050  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 tcgetattr@GLIBC_2.2.5 + 0
+0000000000004058  0000000700000007 R_X86_64_JUMP_SLOT     0000000000000000 tcsetattr@GLIBC_2.2.5 + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -1,27 +1,27 @@
 
-Dynamic section at offset 0x2e18 contains 24 entries:
+Dynamic section at offset 0x2e20 contains 24 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000c (INIT)               0x1000
- 0x000000000000000d (FINI)               0x1478
- 0x0000000000000019 (INIT_ARRAY)         0x3e08
+ 0x000000000000000d (FINI)               0x1444
+ 0x0000000000000019 (INIT_ARRAY)         0x3e10
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
- 0x000000000000001a (FINI_ARRAY)         0x3e10
+ 0x000000000000001a (FINI_ARRAY)         0x3e18
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x2f0
- 0x0000000000000005 (STRTAB)             0x4f8
+ 0x0000000000000005 (STRTAB)             0x4c8
  0x0000000000000006 (SYMTAB)             0x330
- 0x000000000000000a (STRSZ)              233 (bytes)
+ 0x000000000000000a (STRSZ)              220 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
  0x0000000000000003 (PLTGOT)             0x4000
- 0x0000000000000002 (PLTRELSZ)           240 (bytes)
+ 0x0000000000000002 (PLTRELSZ)           216 (bytes)
  0x0000000000000014 (PLTREL)             RELA
- 0x0000000000000017 (JMPREL)             0x6f8
- 0x0000000000000007 (RELA)               0x638
- 0x0000000000000008 (RELASZ)             192 (bytes)
+ 0x0000000000000017 (JMPREL)             0x6a0
+ 0x0000000000000007 (RELA)               0x5f8
+ 0x0000000000000008 (RELASZ)             168 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
- 0x000000006ffffffe (VERNEED)            0x608
+ 0x000000006ffffffe (VERNEED)            0x5c8
  0x000000006fffffff (VERNEEDNUM)         1
- 0x000000006ffffff0 (VERSYM)             0x5e2
+ 0x000000006ffffff0 (VERSYM)             0x5a4
  0x000000006ffffff9 (RELACOUNT)          3
  0x0000000000000000 (NULL)               0x0
```

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 391f25a822d1a6d3a5f540b0b12394f2063724e7
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: f99d4d9b1f35083fbb5f4c688483b0a978211b17
```

#### readelf --wide --version-info {}

```diff
@@ -1,14 +1,14 @@
 
-Version symbols section '.gnu.version' contains 19 entries:
- Addr: 0x00000000000005e2  Offset: 0x000005e2  Link: 4 (.dynsym)
-  000:   0 (*local*)       1 (*global*)      2 (GLIBC_2.2.5)   3 (GLIBC_2.4)  
-  004:   2 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)   1 (*global*)      2 (GLIBC_2.2.5)
-  008:   2 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)   1 (*global*)      2 (GLIBC_2.2.5)
+Version symbols section '.gnu.version' contains 17 entries:
+ Addr: 0x00000000000005a4  Offset: 0x000005a4  Link: 4 (.dynsym)
+  000:   0 (*local*)       1 (*global*)      2 (GLIBC_2.4)     3 (GLIBC_2.2.5)
+  004:   3 (GLIBC_2.2.5)   1 (*global*)      3 (GLIBC_2.2.5)   3 (GLIBC_2.2.5)
+  008:   1 (*global*)      3 (GLIBC_2.2.5)   1 (*global*)      1 (*global*)   
   00c:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
-  010:   1 (*global*)      1 (*global*)      1 (*global*)   
+  010:   1 (*global*)   
 
 Version needs section '.gnu.version_r' contains 1 entry:
- Addr: 0x0000000000000608  Offset: 0x00000608  Link: 5 (.dynstr)
+ Addr: 0x00000000000005c8  Offset: 0x000005c8  Link: 5 (.dynstr)
   000000: Version: 1  File: libc.so.6  Cnt: 2
-  0x0010:   Name: GLIBC_2.4  Flags: none  Version: 3
-  0x0020:   Name: GLIBC_2.2.5  Flags: none  Version: 2
+  0x0010:   Name: GLIBC_2.2.5  Flags: none  Version: 3
+  0x0020:   Name: GLIBC_2.4  Flags: none  Version: 2
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -9,119 +9,119 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000001020..00000000000010d0
+00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000001020..00000000000010c0
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 6 to 0000000000001026
   DW_CFA_def_cfa_offset: 24
   DW_CFA_advance_loc: 10 to 0000000000001030
   DW_CFA_def_cfa_expression (DW_OP_breg7 (rsp): 8; DW_OP_breg16 (rip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit10; DW_OP_ge; DW_OP_lit3; DW_OP_shl; DW_OP_plus)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000040 0000000000000014 00000044 FDE cie=00000000 pc=00000000000010d0..00000000000010e0
+00000040 0000000000000014 00000044 FDE cie=00000000 pc=00000000000010c0..00000000000010d0
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000058 0000000000000014 0000005c FDE cie=00000000 pc=00000000000010e0..0000000000001180
+00000058 0000000000000014 0000005c FDE cie=00000000 pc=00000000000010d0..0000000000001160
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000070 000000000000001c 00000074 FDE cie=00000000 pc=0000000000001239..000000000000125d
-  DW_CFA_advance_loc: 5 to 000000000000123e
+00000070 000000000000001c 00000074 FDE cie=00000000 pc=0000000000001219..000000000000123d
+  DW_CFA_advance_loc: 5 to 000000000000121e
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000001241
+  DW_CFA_advance_loc: 3 to 0000000000001221
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 27 to 000000000000125c
+  DW_CFA_advance_loc: 27 to 000000000000123c
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000090 000000000000001c 00000094 FDE cie=00000000 pc=000000000000125d..00000000000012c8
-  DW_CFA_advance_loc: 5 to 0000000000001262
+00000090 000000000000001c 00000094 FDE cie=00000000 pc=000000000000123d..00000000000012a8
+  DW_CFA_advance_loc: 5 to 0000000000001242
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000001265
+  DW_CFA_advance_loc: 3 to 0000000000001245
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 98 to 00000000000012c7
+  DW_CFA_advance_loc1: 98 to 00000000000012a7
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000000b0 000000000000001c 000000b4 FDE cie=00000000 pc=00000000000012c8..0000000000001358
-  DW_CFA_advance_loc: 5 to 00000000000012cd
+000000b0 000000000000001c 000000b4 FDE cie=00000000 pc=00000000000012a8..0000000000001338
+  DW_CFA_advance_loc: 5 to 00000000000012ad
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000012d0
+  DW_CFA_advance_loc: 3 to 00000000000012b0
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 135 to 0000000000001357
+  DW_CFA_advance_loc1: 135 to 0000000000001337
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000000d0 000000000000001c 000000d4 FDE cie=00000000 pc=0000000000001358..000000000000141f
-  DW_CFA_advance_loc: 5 to 000000000000135d
+000000d0 000000000000001c 000000d4 FDE cie=00000000 pc=0000000000001338..00000000000013ed
+  DW_CFA_advance_loc: 5 to 000000000000133d
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000001360
+  DW_CFA_advance_loc: 3 to 0000000000001340
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 190 to 000000000000141e
+  DW_CFA_advance_loc1: 172 to 00000000000013ec
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000000f0 000000000000001c 000000f4 FDE cie=00000000 pc=000000000000141f..0000000000001433
-  DW_CFA_advance_loc: 5 to 0000000000001424
+000000f0 000000000000001c 000000f4 FDE cie=00000000 pc=00000000000013ed..0000000000001401
+  DW_CFA_advance_loc: 5 to 00000000000013f2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000001427
+  DW_CFA_advance_loc: 3 to 00000000000013f5
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 11 to 0000000000001432
+  DW_CFA_advance_loc: 11 to 0000000000001400
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000110 000000000000001c 00000114 FDE cie=00000000 pc=0000000000001433..0000000000001451
-  DW_CFA_advance_loc: 5 to 0000000000001438
+00000110 000000000000001c 00000114 FDE cie=00000000 pc=0000000000001401..000000000000141f
+  DW_CFA_advance_loc: 5 to 0000000000001406
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 000000000000143b
+  DW_CFA_advance_loc: 3 to 0000000000001409
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 21 to 0000000000001450
+  DW_CFA_advance_loc: 21 to 000000000000141e
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000130 000000000000001c 00000134 FDE cie=00000000 pc=0000000000001451..0000000000001475
-  DW_CFA_advance_loc: 5 to 0000000000001456
+00000130 000000000000001c 00000134 FDE cie=00000000 pc=000000000000141f..0000000000001443
+  DW_CFA_advance_loc: 5 to 0000000000001424
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000001459
+  DW_CFA_advance_loc: 3 to 0000000000001427
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 27 to 0000000000001474
+  DW_CFA_advance_loc: 27 to 0000000000001442
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
 00000150 ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -4,16 +4,16 @@
 __cxa_finalize
 tcsetattr
 __stack_chk_fail
 tcgetattr
 isInputReady
 getCharacter
 libc.so.6
-GLIBC_2.4
 GLIBC_2.2.5
+GLIBC_2.4
 GCC: (Ubuntu 11.4.0-1ubuntu1~22.04) 11.4.0
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.0
 __do_global_dtors_aux_fini_array_entry
 frame_dummy
@@ -22,21 +22,19 @@
 __FRAME_END__
 __dso_handle
 _DYNAMIC
 __GNU_EH_FRAME_HDR
 __TMC_END__
 _GLOBAL_OFFSET_TABLE_
 _ITM_deregisterTMCloneTable
-stdin@GLIBC_2.2.5
 __stack_chk_fail@GLIBC_2.4
 isInputReady
 ioctl@GLIBC_2.2.5
 read@GLIBC_2.2.5
 __gmon_start__
-fflush@GLIBC_2.2.5
 tcgetattr@GLIBC_2.2.5
 tcsetattr@GLIBC_2.2.5
 getCharacter
 _ITM_registerTMCloneTable
 __cxa_finalize@GLIBC_2.2.5
 .shstrtab
 .note.gnu.property
```

#### readelf --wide --decompress --hex-dump=.gnu.hash {}

```diff
@@ -1,7 +1,7 @@
 
 Hex dump of section '.gnu.hash':
-  0x000002f0 03000000 0c000000 01000000 06000000 ................
-  0x00000300 4048d810 08200502 0c000000 0f000000 @H... ..........
+  0x000002f0 03000000 0a000000 01000000 06000000 ................
+  0x00000300 4048d810 08200502 0a000000 0d000000 @H... ..........
   0x00000310 00000000 86a35b29 4a1b9e7c 17d72f19 ......[)J..|../.
   0x00000320 96c3c60f 3885987c f038800f f3540b30 ....8..|.8...T.0
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1,18 +1,17 @@
 
 Hex dump of section '.dynstr':
-  0x000004f8 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
-  0x00000508 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
-  0x00000518 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
-  0x00000528 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
-  0x00000538 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
-  0x00000548 6c697a65 00726573 756d6500 74637365 lize.resume.tcse
-  0x00000558 74617474 72006b62 68697400 696f6374 tattr.kbhit.ioct
-  0x00000568 6c007374 6f70005f 5f737461 636b5f63 l.stop.__stack_c
-  0x00000578 686b5f66 61696c00 67657463 68007265 hk_fail.getch.re
-  0x00000588 61640069 6e697400 74636765 74617474 ad.init.tcgetatt
-  0x00000598 72007374 64696e00 66666c75 73680069 r.stdin.fflush.i
-  0x000005a8 73496e70 75745265 61647900 67657443 sInputReady.getC
-  0x000005b8 68617261 63746572 006c6962 632e736f haracter.libc.so
-  0x000005c8 2e360047 4c494243 5f322e34 00474c49 .6.GLIBC_2.4.GLI
-  0x000005d8 42435f32 2e322e35 00                BC_2.2.5.
+  0x000004c8 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
+  0x000004d8 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
+  0x000004e8 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
+  0x000004f8 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
+  0x00000508 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
+  0x00000518 6c697a65 00726573 756d6500 74637365 lize.resume.tcse
+  0x00000528 74617474 72006b62 68697400 696f6374 tattr.kbhit.ioct
+  0x00000538 6c007374 6f70005f 5f737461 636b5f63 l.stop.__stack_c
+  0x00000548 686b5f66 61696c00 67657463 68007265 hk_fail.getch.re
+  0x00000558 61640069 6e697400 74636765 74617474 ad.init.tcgetatt
+  0x00000568 72006973 496e7075 74526561 64790067 r.isInputReady.g
+  0x00000578 65744368 61726163 74657200 6c696263 etCharacter.libc
+  0x00000588 2e736f2e 3600474c 4942435f 322e322e .so.6.GLIBC_2.2.
+  0x00000598 3500474c 4942435f 322e3400          5.GLIBC_2.4.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -39,11 +39,7 @@
 	push   $0x7
 	bnd jmp 1020 <_init+0x20>
 	nop
 	endbr64
 	push   $0x8
 	bnd jmp 1020 <_init+0x20>
 	nop
-	endbr64
-	push   $0x9
-	bnd jmp 1020 <_init+0x20>
-	nop
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.got {}

```diff
@@ -1,9 +1,9 @@
 
 
 
 Disassembly of section .plt.got:
 
-00000000000010d0 <__cxa_finalize@plt>:
+00000000000010c0 <__cxa_finalize@plt>:
 	endbr64
-	bnd jmp *0x2f1d(%rip)        
+	bnd jmp *0x2f2d(%rip)        
 	nopl   0x0(%rax,%rax,1)
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.sec {}

```diff
@@ -1,54 +1,49 @@
 
 
 
 Disassembly of section .plt.sec:
 
-00000000000010e0 <__stack_chk_fail@plt>:
+00000000000010d0 <__stack_chk_fail@plt>:
+	endbr64
+	bnd jmp *0x2f3d(%rip)        
+	nopl   0x0(%rax,%rax,1)
+
+00000000000010e0 <kbhit@plt>:
+	endbr64
+	bnd jmp *0x2f35(%rip)        
+	nopl   0x0(%rax,%rax,1)
+
+00000000000010f0 <stop@plt>:
 	endbr64
 	bnd jmp *0x2f2d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000010f0 <kbhit@plt>:
+0000000000001100 <ioctl@plt>:
 	endbr64
 	bnd jmp *0x2f25(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000001100 <stop@plt>:
+0000000000001110 <read@plt>:
 	endbr64
 	bnd jmp *0x2f1d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000001110 <ioctl@plt>:
+0000000000001120 <resume@plt>:
 	endbr64
 	bnd jmp *0x2f15(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000001120 <read@plt>:
+0000000000001130 <getch@plt>:
 	endbr64
 	bnd jmp *0x2f0d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000001130 <resume@plt>:
+0000000000001140 <tcgetattr@plt>:
 	endbr64
 	bnd jmp *0x2f05(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000001140 <fflush@plt>:
+0000000000001150 <tcsetattr@plt>:
 	endbr64
 	bnd jmp *0x2efd(%rip)        
 	nopl   0x0(%rax,%rax,1)
-
-0000000000001150 <getch@plt>:
-	endbr64
-	bnd jmp *0x2ef5(%rip)        
-	nopl   0x0(%rax,%rax,1)
-
-0000000000001160 <tcgetattr@plt>:
-	endbr64
-	bnd jmp *0x2eed(%rip)        
-	nopl   0x0(%rax,%rax,1)
-
-0000000000001170 <tcsetattr@plt>:
-	endbr64
-	bnd jmp *0x2ee5(%rip)        
-	nopl   0x0(%rax,%rax,1)
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,221 +1,217 @@
 
 
 
 Disassembly of section .text:
 
-0000000000001180 <deregister_tm_clones>:
+0000000000001160 <deregister_tm_clones>:
 deregister_tm_clones():
-	lea    0x2ee9(%rip),%rdi        
-	lea    0x2ee2(%rip),%rax        
+	lea    0x2f01(%rip),%rdi        
+	lea    0x2efa(%rip),%rax        
 	cmp    %rdi,%rax
-	je     11a8 <deregister_tm_clones+0x28>
-	mov    0x2e3e(%rip),%rax        
+	je     1188 <deregister_tm_clones+0x28>
+	mov    0x2e66(%rip),%rax        
 	test   %rax,%rax
-	je     11a8 <deregister_tm_clones+0x28>
+	je     1188 <deregister_tm_clones+0x28>
 	jmp    *%rax
 	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
 
-00000000000011b0 <register_tm_clones>:
+0000000000001190 <register_tm_clones>:
 register_tm_clones():
-	lea    0x2eb9(%rip),%rdi        
-	lea    0x2eb2(%rip),%rsi        
+	lea    0x2ed1(%rip),%rdi        
+	lea    0x2eca(%rip),%rsi        
 	sub    %rdi,%rsi
 	mov    %rsi,%rax
 	shr    $0x3f,%rsi
 	sar    $0x3,%rax
 	add    %rax,%rsi
 	sar    $1,%rsi
-	je     11e8 <register_tm_clones+0x38>
-	mov    0x2e15(%rip),%rax        
+	je     11c8 <register_tm_clones+0x38>
+	mov    0x2e35(%rip),%rax        
 	test   %rax,%rax
-	je     11e8 <register_tm_clones+0x38>
+	je     11c8 <register_tm_clones+0x38>
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 	ret
 	nopl   0x0(%rax)
 
-00000000000011f0 <__do_global_dtors_aux>:
+00000000000011d0 <__do_global_dtors_aux>:
 __do_global_dtors_aux():
 	endbr64
-	cmpb   $0x0,0x2e85(%rip)        
-	jne    1228 <__do_global_dtors_aux+0x38>
+	cmpb   $0x0,0x2ea5(%rip)        
+	jne    1208 <__do_global_dtors_aux+0x38>
 	push   %rbp
-	cmpq   $0x0,0x2df2(%rip)        
+	cmpq   $0x0,0x2e12(%rip)        
 	mov    %rsp,%rbp
-	je     1217 <__do_global_dtors_aux+0x27>
-	mov    0x2e56(%rip),%rdi        
-	call   10d0 <__cxa_finalize@plt>
-	call   1180 <deregister_tm_clones>
-	movb   $0x1,0x2e5d(%rip)        
+	je     11f7 <__do_global_dtors_aux+0x27>
+	mov    0x2e6e(%rip),%rdi        
+	call   10c0 <__cxa_finalize@plt>
+	call   1160 <deregister_tm_clones>
+	movb   $0x1,0x2e7d(%rip)        
 	pop    %rbp
 	ret
 	nopl   (%rax)
 	ret
 	nopl   0x0(%rax)
 
-0000000000001230 <frame_dummy>:
+0000000000001210 <frame_dummy>:
 frame_dummy():
 	endbr64
-	jmp    11b0 <register_tm_clones>
+	jmp    1190 <register_tm_clones>
 
-0000000000001239 <resume>:
+0000000000001219 <resume>:
 resume():
 	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
-	lea    0x2e98(%rip),%rax        
+	lea    0x2eb8(%rip),%rax        
 	mov    %rax,%rdx
 	mov    $0x0,%esi
 	mov    $0x0,%edi
-	call   1170 <tcsetattr@plt>
+	call   1150 <tcsetattr@plt>
 	nop
 	pop    %rbp
 	ret
 
-000000000000125d <kbhit>:
+000000000000123d <kbhit>:
 kbhit():
 	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %fs:0x28,%rax
 	mov    %rax,-0x8(%rbp)
 	xor    %eax,%eax
 	mov    $0x0,%eax
-	call   1130 <resume@plt>
+	call   1120 <resume@plt>
 	lea    -0xc(%rbp),%rax
 	mov    %rax,%rdx
 	mov    $0x541b,%esi
 	mov    $0x0,%edi
 	mov    $0x0,%eax
-	call   1110 <ioctl@plt>
+	call   1100 <ioctl@plt>
 	mov    $0x0,%eax
-	call   1100 <stop@plt>
+	call   10f0 <stop@plt>
 	mov    -0xc(%rbp),%eax
 	test   %eax,%eax
 	setg   %al
 	movzbl %al,%eax
 	mov    -0x8(%rbp),%rdx
 	sub    %fs:0x28,%rdx
-	je     12c6 <kbhit+0x69>
-	call   10e0 <__stack_chk_fail@plt>
+	je     12a6 <kbhit+0x69>
+	call   10d0 <__stack_chk_fail@plt>
 	leave
 	ret
 
-00000000000012c8 <getch>:
+00000000000012a8 <getch>:
 getch():
 	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %fs:0x28,%rax
 	mov    %rax,-0x8(%rbp)
 	xor    %eax,%eax
 	mov    $0x0,%eax
-	call   1130 <resume@plt>
+	call   1120 <resume@plt>
 	lea    -0x10(%rbp),%rax
 	mov    %rax,%rdx
 	mov    $0x541b,%esi
 	mov    $0x0,%edi
 	mov    $0x0,%eax
-	call   1110 <ioctl@plt>
+	call   1100 <ioctl@plt>
 	mov    -0x10(%rbp),%eax
 	cmp    $0x4,%eax
-	jle    1317 <getch+0x4f>
+	jle    12f7 <getch+0x4f>
 	movl   $0x4,-0x10(%rbp)
 	movl   $0x0,-0xc(%rbp)
 	mov    -0x10(%rbp),%eax
 	movslq %eax,%rdx
 	lea    -0xc(%rbp),%rax
 	mov    %rax,%rsi
 	mov    $0x0,%edi
-	call   1120 <read@plt>
+	call   1110 <read@plt>
 	mov    $0x0,%eax
-	call   1100 <stop@plt>
+	call   10f0 <stop@plt>
 	mov    -0xc(%rbp),%eax
 	mov    -0x8(%rbp),%rdx
 	sub    %fs:0x28,%rdx
-	je     1356 <getch+0x8e>
-	call   10e0 <__stack_chk_fail@plt>
+	je     1336 <getch+0x8e>
+	call   10d0 <__stack_chk_fail@plt>
 	leave
 	ret
 
-0000000000001358 <init>:
+0000000000001338 <init>:
 init():
 	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
-	lea    0x2d39(%rip),%rax        
+	lea    0x2d59(%rip),%rax        
 	mov    %rax,%rsi
 	mov    $0x0,%edi
-	call   1160 <tcgetattr@plt>
-	mov    0x2d25(%rip),%rax        
-	mov    0x2d26(%rip),%rdx        
-	mov    %rax,0x2d57(%rip)        
-	mov    %rdx,0x2d58(%rip)        
-	mov    0x2d19(%rip),%rax        
-	mov    0x2d1a(%rip),%rdx        
-	mov    %rax,0x2d4b(%rip)        
-	mov    %rdx,0x2d4c(%rip)        
-	mov    0x2d0d(%rip),%rax        
-	mov    0x2d0e(%rip),%rdx        
-	mov    %rax,0x2d3f(%rip)        
-	mov    %rdx,0x2d40(%rip)        
-	mov    0x2d01(%rip),%rax        
-	mov    %rax,0x2d3a(%rip)        
-	mov    0x2cfc(%rip),%eax        
-	mov    %eax,0x2d36(%rip)        
-	mov    0x2d04(%rip),%eax        
+	call   1140 <tcgetattr@plt>
+	mov    0x2d45(%rip),%rax        
+	mov    0x2d46(%rip),%rdx        
+	mov    %rax,0x2d77(%rip)        
+	mov    %rdx,0x2d78(%rip)        
+	mov    0x2d39(%rip),%rax        
+	mov    0x2d3a(%rip),%rdx        
+	mov    %rax,0x2d6b(%rip)        
+	mov    %rdx,0x2d6c(%rip)        
+	mov    0x2d2d(%rip),%rax        
+	mov    0x2d2e(%rip),%rdx        
+	mov    %rax,0x2d5f(%rip)        
+	mov    %rdx,0x2d60(%rip)        
+	mov    0x2d21(%rip),%rax        
+	mov    %rax,0x2d5a(%rip)        
+	mov    0x2d1c(%rip),%eax        
+	mov    %eax,0x2d56(%rip)        
+	mov    0x2d24(%rip),%eax        
 	and    $0xfffffff5,%eax
-	mov    %eax,0x2cfb(%rip)        
-	lea    0x2ce8(%rip),%rax        
+	mov    %eax,0x2d1b(%rip)        
+	lea    0x2d08(%rip),%rax        
 	mov    %rax,%rdx
 	mov    $0x0,%esi
 	mov    $0x0,%edi
-	call   1170 <tcsetattr@plt>
-	mov    0x2bcf(%rip),%rax        
-	mov    (%rax),%rax
-	mov    %rax,%rdi
-	call   1140 <fflush@plt>
+	call   1150 <tcsetattr@plt>
 	nop
 	pop    %rbp
 	ret
 
-000000000000141f <isInputReady>:
+00000000000013ed <isInputReady>:
 isInputReady():
 	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    $0x0,%eax
-	call   10f0 <kbhit@plt>
+	call   10e0 <kbhit@plt>
 	pop    %rbp
 	ret
 
-0000000000001433 <getCharacter>:
+0000000000001401 <getCharacter>:
 getCharacter():
 	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    $0x0,%eax
-	call   1150 <getch@plt>
+	call   1130 <getch@plt>
 	mov    %eax,-0x4(%rbp)
 	mov    -0x4(%rbp),%eax
 	leave
 	ret
 
-0000000000001451 <stop>:
+000000000000141f <stop>:
 stop():
 	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
-	lea    0x2c40(%rip),%rax        
+	lea    0x2c72(%rip),%rax        
 	mov    %rax,%rdx
 	mov    $0x0,%esi
 	mov    $0x0,%edi
-	call   1170 <tcsetattr@plt>
+	call   1150 <tcsetattr@plt>
 	nop
 	pop    %rbp
 	ret
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,11 +1,11 @@
 
 
 
 Disassembly of section .fini:
 
-0000000000001478 <_fini>:
+0000000000001444 <_fini>:
 _fini():
 	endbr64
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,9 +1,9 @@
 
 Hex dump of section '.eh_frame_hdr':
   0x00002000 011b033b 5c000000 0a000000 20f0ffff ...;\....... ...
-  0x00002010 78000000 d0f0ffff a0000000 e0f0ffff x...............
-  0x00002020 b8000000 39f2ffff d0000000 5df2ffff ....9.......]...
-  0x00002030 f0000000 c8f2ffff 10010000 58f3ffff ............X...
-  0x00002040 30010000 1ff4ffff 50010000 33f4ffff 0.......P...3...
-  0x00002050 70010000 51f4ffff 90010000          p...Q.......
+  0x00002010 78000000 c0f0ffff a0000000 d0f0ffff x...............
+  0x00002020 b8000000 19f2ffff d0000000 3df2ffff ............=...
+  0x00002030 f0000000 a8f2ffff 10010000 38f3ffff ............8...
+  0x00002040 30010000 edf3ffff 50010000 01f4ffff 0.......P.......
+  0x00002050 70010000 1ff4ffff 90010000          p...........
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,25 +1,25 @@
 
 Hex dump of section '.eh_frame':
   0x00002060 14000000 00000000 017a5200 01781001 .........zR..x..
   0x00002070 1b0c0708 90010000 24000000 1c000000 ........$.......
-  0x00002080 a0efffff b0000000 000e1046 0e184a0f ...........F..J.
+  0x00002080 a0efffff a0000000 000e1046 0e184a0f ...........F..J.
   0x00002090 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
-  0x000020a0 14000000 44000000 28f0ffff 10000000 ....D...(.......
+  0x000020a0 14000000 44000000 18f0ffff 10000000 ....D...........
   0x000020b0 00000000 00000000 14000000 5c000000 ............\...
-  0x000020c0 20f0ffff a0000000 00000000 00000000  ...............
-  0x000020d0 1c000000 74000000 61f1ffff 24000000 ....t...a...$...
+  0x000020c0 10f0ffff 90000000 00000000 00000000 ................
+  0x000020d0 1c000000 74000000 41f1ffff 24000000 ....t...A...$...
   0x000020e0 00450e10 8602430d 065b0c07 08000000 .E....C..[......
-  0x000020f0 1c000000 94000000 65f1ffff 6b000000 ........e...k...
+  0x000020f0 1c000000 94000000 45f1ffff 6b000000 ........E...k...
   0x00002100 00450e10 8602430d 0602620c 07080000 .E....C...b.....
-  0x00002110 1c000000 b4000000 b0f1ffff 90000000 ................
+  0x00002110 1c000000 b4000000 90f1ffff 90000000 ................
   0x00002120 00450e10 8602430d 0602870c 07080000 .E....C.........
-  0x00002130 1c000000 d4000000 20f2ffff c7000000 ........ .......
-  0x00002140 00450e10 8602430d 0602be0c 07080000 .E....C.........
-  0x00002150 1c000000 f4000000 c7f2ffff 14000000 ................
+  0x00002130 1c000000 d4000000 00f2ffff b5000000 ................
+  0x00002140 00450e10 8602430d 0602ac0c 07080000 .E....C.........
+  0x00002150 1c000000 f4000000 95f2ffff 14000000 ................
   0x00002160 00450e10 8602430d 064b0c07 08000000 .E....C..K......
-  0x00002170 1c000000 14010000 bbf2ffff 1e000000 ................
+  0x00002170 1c000000 14010000 89f2ffff 1e000000 ................
   0x00002180 00450e10 8602430d 06550c07 08000000 .E....C..U......
-  0x00002190 1c000000 34010000 b9f2ffff 24000000 ....4.......$...
+  0x00002190 1c000000 34010000 87f2ffff 24000000 ....4.......$...
   0x000021a0 00450e10 8602430d 065b0c07 08000000 .E....C..[......
   0x000021b0 00000000                            ....
```

#### readelf --wide --decompress --hex-dump=.init_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.init_array':
-  0x00003e08 30120000 00000000                   0.......
+  0x00003e10 10120000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.fini_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.fini_array':
-  0x00003e10 f0110000 00000000                   ........
+  0x00003e18 d0110000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.got {}

```diff
@@ -1,6 +1,5 @@
 
 Hex dump of section '.got':
-  0x00003fd8 00000000 00000000 00000000 00000000 ................
-  0x00003fe8 00000000 00000000 00000000 00000000 ................
-  0x00003ff8 00000000 00000000                   ........
+  0x00003fe0 00000000 00000000 00000000 00000000 ................
+  0x00003ff0 00000000 00000000 00000000 00000000 ................
```

#### readelf --wide --decompress --hex-dump=.got.plt {}

```diff
@@ -1,11 +1,10 @@
 
 Hex dump of section '.got.plt':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
-  0x00004000 183e0000 00000000 00000000 00000000 .>..............
+  0x00004000 203e0000 00000000 00000000 00000000  >..............
   0x00004010 00000000 00000000 30100000 00000000 ........0.......
   0x00004020 40100000 00000000 50100000 00000000 @.......P.......
   0x00004030 60100000 00000000 70100000 00000000 `.......p.......
   0x00004040 80100000 00000000 90100000 00000000 ................
   0x00004050 a0100000 00000000 b0100000 00000000 ................
-  0x00004060 c0100000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.data':
-  0x00004068 68400000 00000000                   h@......
+  0x00004060 60400000 00000000                   `@......
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -15,25 +15,23 @@
   0x000000c0 696e6900 5f5f6473 6f5f6861 6e646c65 ini.__dso_handle
   0x000000d0 005f4459 4e414d49 43005f5f 474e555f ._DYNAMIC.__GNU_
   0x000000e0 45485f46 52414d45 5f484452 005f5f54 EH_FRAME_HDR.__T
   0x000000f0 4d435f45 4e445f5f 005f474c 4f42414c MC_END__._GLOBAL
   0x00000100 5f4f4646 5345545f 5441424c 455f005f _OFFSET_TABLE_._
   0x00000110 696e6974 005f4954 4d5f6465 72656769 init._ITM_deregi
   0x00000120 73746572 544d436c 6f6e6554 61626c65 sterTMCloneTable
-  0x00000130 00737464 696e4047 4c494243 5f322e32 .stdin@GLIBC_2.2
-  0x00000140 2e35005f 5f737461 636b5f63 686b5f66 .5.__stack_chk_f
-  0x00000150 61696c40 474c4942 435f322e 34006973 ail@GLIBC_2.4.is
-  0x00000160 496e7075 74526561 6479006b 62686974 InputReady.kbhit
-  0x00000170 0073746f 7000696f 63746c40 474c4942 .stop.ioctl@GLIB
-  0x00000180 435f322e 322e3500 72656164 40474c49 C_2.2.5.read@GLI
-  0x00000190 42435f32 2e322e35 005f5f67 6d6f6e5f BC_2.2.5.__gmon_
-  0x000001a0 73746172 745f5f00 72657375 6d650066 start__.resume.f
-  0x000001b0 666c7573 6840474c 4942435f 322e322e flush@GLIBC_2.2.
-  0x000001c0 35006765 74636800 74636765 74617474 5.getch.tcgetatt
-  0x000001d0 7240474c 4942435f 322e322e 35007463 r@GLIBC_2.2.5.tc
-  0x000001e0 73657461 74747240 474c4942 435f322e setattr@GLIBC_2.
-  0x000001f0 322e3500 67657443 68617261 63746572 2.5.getCharacter
-  0x00000200 005f4954 4d5f7265 67697374 6572544d ._ITM_registerTM
-  0x00000210 436c6f6e 65546162 6c65005f 5f637861 CloneTable.__cxa
-  0x00000220 5f66696e 616c697a 6540474c 4942435f _finalize@GLIBC_
-  0x00000230 322e322e 3500                       2.2.5.
+  0x00000130 005f5f73 7461636b 5f63686b 5f666169 .__stack_chk_fai
+  0x00000140 6c40474c 4942435f 322e3400 6973496e l@GLIBC_2.4.isIn
+  0x00000150 70757452 65616479 006b6268 69740073 putReady.kbhit.s
+  0x00000160 746f7000 696f6374 6c40474c 4942435f top.ioctl@GLIBC_
+  0x00000170 322e322e 35007265 61644047 4c494243 2.2.5.read@GLIBC
+  0x00000180 5f322e32 2e35005f 5f676d6f 6e5f7374 _2.2.5.__gmon_st
+  0x00000190 6172745f 5f007265 73756d65 00676574 art__.resume.get
+  0x000001a0 63680074 63676574 61747472 40474c49 ch.tcgetattr@GLI
+  0x000001b0 42435f32 2e322e35 00746373 65746174 BC_2.2.5.tcsetat
+  0x000001c0 74724047 4c494243 5f322e32 2e350067 tr@GLIBC_2.2.5.g
+  0x000001d0 65744368 61726163 74657200 5f49544d etCharacter._ITM
+  0x000001e0 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
+  0x000001f0 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
+  0x00000200 6c697a65 40474c49 42435f32 2e322e35 lize@GLIBC_2.2.5
+  0x00000210 00                                  .
```

### Comparing `advanced_input-0.2.0/advanced_input.egg-info/PKG-INFO` & `advanced_input-0.2.1/advanced_input.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advanced_input
-Version: 0.2.0
+Version: 0.2.1
 Summary: IO Extention
 Home-page: https://github.com/NightKey/advanced-input
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/advanced-input/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -38,7 +38,12 @@
     input_handler.read("Press any character to exit...", PriorityOrder.Low)
     input_handler.stop()
 ```
 
 This will result in a user input for `thread_one` being created before the `main` function's exit will be available. Normally, this would result in the program exiting, before accepting the user input of `thread_one`. With this, thread one will be in a higher priority than `main`, and that will be the first to be served the user's input. Additionally, `Read()` returns when one character is pressed.
 
 If there are multiple inputs with the same priority, it will return them in a first come last serve method.
+
+## Windows quirks
+
+Due to how Windows works with new line (\r\n), on Windows it is not possible to read the "Carriage Return" (\r) character. It will always return "Line Feed" (\n) instead.
+Due to how Windows console works, the default (utf-8) encoding input will not work with some special character. For it to work, please specify the encoding of your system.
```

### Comparing `advanced_input-0.2.0/setup.cfg` & `advanced_input-0.2.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6476 616e 6365 645f 696e 7075   = advanced_inpu
 00000020: 740d 0a76 6572 7369 6f6e 203d 2030 2e32  t..version = 0.2
-00000030: 2e30 0d0a 6175 7468 6f72 203d 204a 616e  .0..author = Jan
+00000030: 2e31 0d0a 6175 7468 6f72 203d 204a 616e  .1..author = Jan
 00000040: 7468 c3b3 2044 c3a1 7669 640d 0a61 7574  th.. D..vid..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6461 7669  hor_email = davi
 00000060: 646a 616e 7468 6f40 676d 6169 6c2e 636f  djantho@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2049 4f20 4578 7465 6e74 696f 6e0d 0a6c   IO Extention..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 000000a0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
```

