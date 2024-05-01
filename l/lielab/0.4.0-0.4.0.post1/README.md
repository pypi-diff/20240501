# Comparing `tmp/lielab-0.4.0-cp39-none-win_amd64.whl.zip` & `tmp/lielab-0.4.0post1-cp311-none-manylinux1_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,539 +1,545 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    673945 (00000000000A4899h)
-  Actual end-cent-dir record offset:        673923 (00000000000A4883h)
-  Expected end-cent-dir record offset:      673923 (00000000000A4883h)
+  Zip archive file size:                    751811 (00000000000B78C3h)
+  Actual end-cent-dir record offset:        751789 (00000000000B78ADh)
+  Expected end-cent-dir record offset:      751789 (00000000000B78ADh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
   central directory contains 18 entries.
-  The central directory is 1308 (000000000000051Ch) bytes long,
+  The central directory is 1377 (0000000000000561h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 672615 (00000000000A4367h).
+  is 750412 (00000000000B734Ch).
 
 
 Central directory entry #1:
 ---------------------------
 
-  lielab/__init__.py
+  lielab-0.4.0post1.dist-info/METADATA
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 30 20:01:48
-  32-bit CRC value (hex):                         4adc5346
-  compressed size:                                134 bytes
-  uncompressed size:                              280 bytes
-  length of filename:                             18 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 May 1 08:43:38
+  32-bit CRC value (hex):                         fd233fcb
+  compressed size:                                252 bytes
+  uncompressed size:                              417 bytes
+  length of filename:                             36 characters
+  length of extra field:                          36 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
-  MS-DOS file attributes (00 hex):                none
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 ba 29 e8 f2 d5 9b da 01 ba 29 e8 f2.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  lielab/cppLielab.cp39-win_amd64.pyd
+  There are an extra -36 bytes preceding this file.
 
-  offset of local header from start of archive:   182
-                                                  (00000000000000B6h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  lielab-0.4.0post1.dist-info/RECORD
+
+  offset of local header from start of archive:   318
+                                                  (000000000000013Eh) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 May 1 02:37:12
-  32-bit CRC value (hex):                         acbc924b
-  compressed size:                                666992 bytes
-  uncompressed size:                              2073600 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          2024 Apr 30 23:55:58
+  32-bit CRC value (hex):                         635000c2
+  compressed size:                                853 bytes
+  uncompressed size:                              1444 bytes
+  length of filename:                             34 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  lielab/domain/__init__.py
+  lielab-0.4.0post1.dist-info/top_level.txt
 
-  offset of local header from start of archive:   667239
-                                                  (00000000000A2E67h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   1235
+                                                  (00000000000004D3h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 29 19:07:18
-  32-bit CRC value (hex):                         67acb6bd
-  compressed size:                                58 bytes
-  uncompressed size:                              69 bytes
-  length of filename:                             25 characters
+  file last modified on (DOS date/time):          2024 Apr 30 23:55:58
+  32-bit CRC value (hex):                         20a856d7
+  compressed size:                                9 bytes
+  uncompressed size:                              7 bytes
+  length of filename:                             41 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  lielab/domain/domain.py
+  lielab-0.4.0post1.dist-info/WHEEL
 
-  offset of local header from start of archive:   667352
-                                                  (00000000000A2ED8h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   1315
+                                                  (0000000000000523h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 29 14:50:22
-  32-bit CRC value (hex):                         64f4bcb7
-  compressed size:                                8 bytes
-  uncompressed size:                              6 bytes
-  length of filename:                             23 characters
+  file last modified on (DOS date/time):          2024 Apr 30 23:55:58
+  32-bit CRC value (hex):                         f84b88ab
+  compressed size:                                106 bytes
+  uncompressed size:                              108 bytes
+  length of filename:                             33 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  lielab/dynamics/__init__.py
+  lielab/cppLielab.cpython-311-x86_64-linux-gnu.so
 
-  offset of local header from start of archive:   667413
-                                                  (00000000000A2F15h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   1484
+                                                  (00000000000005CCh) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 29 19:07:26
-  32-bit CRC value (hex):                         cdb1ea41
-  compressed size:                                38 bytes
-  uncompressed size:                              36 bytes
-  length of filename:                             27 characters
+  file last modified on (DOS date/time):          2024 Apr 30 23:55:56
+  32-bit CRC value (hex):                         36747ae3
+  compressed size:                                744804 bytes
+  uncompressed size:                              2346944 bytes
+  length of filename:                             48 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
-  lielab/functions/__init__.py
+  lielab/domain/domain.py
 
-  offset of local header from start of archive:   667508
-                                                  (00000000000A2F74h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   746366
+                                                  (00000000000B637Eh) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 29 19:07:42
-  32-bit CRC value (hex):                         385a8f09
-  compressed size:                                39 bytes
-  uncompressed size:                              37 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2024 Apr 30 17:04:22
+  32-bit CRC value (hex):                         0e1a9296
+  compressed size:                                7 bytes
+  uncompressed size:                              5 bytes
+  length of filename:                             23 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #7:
 ---------------------------
 
-  lielab/kinematics/__init__.py
+  lielab/domain/__init__.py
 
-  offset of local header from start of archive:   667605
-                                                  (00000000000A2FD5h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   746426
+                                                  (00000000000B63BAh) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 29 19:07:50
-  32-bit CRC value (hex):                         9e7cd960
-  compressed size:                                50 bytes
-  uncompressed size:                              53 bytes
-  length of filename:                             29 characters
+  file last modified on (DOS date/time):          2024 Apr 30 17:04:22
+  32-bit CRC value (hex):                         0a2b3a74
+  compressed size:                                55 bytes
+  uncompressed size:                              65 bytes
+  length of filename:                             25 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #8:
 ---------------------------
 
-  lielab/optim/__init__.py
+  lielab/dynamics/__init__.py
 
-  offset of local header from start of archive:   667714
-                                                  (00000000000A3042h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   746536
+                                                  (00000000000B6428h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 29 14:50:22
-  32-bit CRC value (hex):                         cb876b31
-  compressed size:                                40 bytes
-  uncompressed size:                              40 bytes
-  length of filename:                             24 characters
+  file last modified on (DOS date/time):          2024 Apr 30 17:04:22
+  32-bit CRC value (hex):                         f7e2377a
+  compressed size:                                37 bytes
+  uncompressed size:                              35 bytes
+  length of filename:                             27 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #9:
 ---------------------------
 
-  lielab/optim/optim.py
+  lielab/functions/__init__.py
 
-  offset of local header from start of archive:   667808
-                                                  (00000000000A30A0h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   746630
+                                                  (00000000000B6486h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 29 19:08:00
-  32-bit CRC value (hex):                         f81e567e
-  compressed size:                                409 bytes
-  uncompressed size:                              1493 bytes
-  length of filename:                             21 characters
+  file last modified on (DOS date/time):          2024 Apr 30 17:04:22
+  32-bit CRC value (hex):                         1343282d
+  compressed size:                                38 bytes
+  uncompressed size:                              36 bytes
+  length of filename:                             28 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #10:
 ---------------------------
 
-  lielab/testing/__init__.py
+  lielab/kinematics/__init__.py
 
-  offset of local header from start of archive:   668268
-                                                  (00000000000A326Ch) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   746726
+                                                  (00000000000B64E6h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 29 14:50:22
-  32-bit CRC value (hex):                         6f992dc0
-  compressed size:                                28 bytes
-  uncompressed size:                              26 bytes
-  length of filename:                             26 characters
+  file last modified on (DOS date/time):          2024 Apr 30 17:04:22
+  32-bit CRC value (hex):                         37593294
+  compressed size:                                48 bytes
+  uncompressed size:                              51 bytes
+  length of filename:                             29 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #11:
 ---------------------------
 
-  lielab/testing/test_main.py
+  lielab/optim/optim.py
 
-  offset of local header from start of archive:   668352
-                                                  (00000000000A32C0h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   746833
+                                                  (00000000000B6551h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 May 1 02:26:18
-  32-bit CRC value (hex):                         183d58b5
-  compressed size:                                396 bytes
-  uncompressed size:                              1069 bytes
-  length of filename:                             27 characters
+  file last modified on (DOS date/time):          2024 Apr 30 17:04:22
+  32-bit CRC value (hex):                         5ac083f4
+  compressed size:                                401 bytes
+  uncompressed size:                              1438 bytes
+  length of filename:                             21 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #12:
 ---------------------------
 
-  lielab/topos/__init__.py
+  lielab/optim/__init__.py
 
-  offset of local header from start of archive:   668805
-                                                  (00000000000A3485h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   747285
+                                                  (00000000000B6715h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 29 19:08:18
-  32-bit CRC value (hex):                         e061bc8b
-  compressed size:                                172 bytes
-  uncompressed size:                              299 bytes
+  file last modified on (DOS date/time):          2024 Apr 30 17:04:22
+  32-bit CRC value (hex):                         77d6583f
+  compressed size:                                39 bytes
+  uncompressed size:                              39 bytes
   length of filename:                             24 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #13:
 ---------------------------
 
-  lielab/topos/topos.py
+  lielab/testing/test_main.py
 
-  offset of local header from start of archive:   669031
-                                                  (00000000000A3567h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   747378
+                                                  (00000000000B6772h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 30 20:01:48
-  32-bit CRC value (hex):                         76a3613e
-  compressed size:                                1974 bytes
-  uncompressed size:                              7311 bytes
-  length of filename:                             21 characters
+  file last modified on (DOS date/time):          2024 Apr 30 23:34:32
+  32-bit CRC value (hex):                         df76a100
+  compressed size:                                388 bytes
+  uncompressed size:                              1023 bytes
+  length of filename:                             27 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #14:
 ---------------------------
 
-  lielab/transform/__init__.py
+  lielab/testing/__init__.py
 
-  offset of local header from start of archive:   671056
-                                                  (00000000000A3D50h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   747823
+                                                  (00000000000B692Fh) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 29 19:08:38
-  32-bit CRC value (hex):                         2a88a22c
-  compressed size:                                49 bytes
-  uncompressed size:                              52 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2024 Apr 30 17:04:22
+  32-bit CRC value (hex):                         b854c459
+  compressed size:                                27 bytes
+  uncompressed size:                              25 bytes
+  length of filename:                             26 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #15:
 ---------------------------
 
-  lielab-0.4.0.dist-info/METADATA
+  lielab/topos/topos.py
 
-  offset of local header from start of archive:   671163
-                                                  (00000000000A3DBBh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   747906
+                                                  (00000000000B6982h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 May 1 02:37:22
-  32-bit CRC value (hex):                         249a0307
-  compressed size:                                257 bytes
-  uncompressed size:                              426 bytes
-  length of filename:                             31 characters
+  file last modified on (DOS date/time):          2024 Apr 30 22:10:28
+  32-bit CRC value (hex):                         21970299
+  compressed size:                                1950 bytes
+  uncompressed size:                              7092 bytes
+  length of filename:                             21 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #16:
 ---------------------------
 
-  lielab-0.4.0.dist-info/WHEEL
+  lielab/topos/__init__.py
 
-  offset of local header from start of archive:   671481
-                                                  (00000000000A3EF9h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   749907
+                                                  (00000000000B7153h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 May 1 02:37:22
-  32-bit CRC value (hex):                         ea925743
-  compressed size:                                99 bytes
-  uncompressed size:                              99 bytes
-  length of filename:                             28 characters
+  file last modified on (DOS date/time):          2024 Apr 30 17:04:22
+  32-bit CRC value (hex):                         0e95ce21
+  compressed size:                                168 bytes
+  uncompressed size:                              290 bytes
+  length of filename:                             24 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #17:
 ---------------------------
 
-  lielab-0.4.0.dist-info/top_level.txt
+  lielab/transform/__init__.py
 
-  offset of local header from start of archive:   671638
-                                                  (00000000000A3F96h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   750129
+                                                  (00000000000B7231h) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 May 1 02:37:22
-  32-bit CRC value (hex):                         20a856d7
-  compressed size:                                9 bytes
-  uncompressed size:                              7 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          2024 Apr 30 17:04:22
+  32-bit CRC value (hex):                         66835106
+  compressed size:                                47 bytes
+  uncompressed size:                              50 bytes
+  length of filename:                             28 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #18:
 ---------------------------
 
-  lielab-0.4.0.dist-info/RECORD
+  lielab/__init__.py
 
-  offset of local header from start of archive:   671713
-                                                  (00000000000A3FE1h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  offset of local header from start of archive:   750234
+                                                  (00000000000B729Ah) bytes
+  file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 May 1 02:37:22
-  32-bit CRC value (hex):                         383670bd
-  compressed size:                                843 bytes
-  uncompressed size:                              1430 bytes
-  length of filename:                             29 characters
+  file last modified on (DOS date/time):          2024 Apr 30 22:10:28
+  32-bit CRC value (hex):                         9880e0a0
+  compressed size:                                130 bytes
+  uncompressed size:                              268 bytes
+  length of filename:                             18 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B400 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,55 +1,55 @@
-Filename: lielab/__init__.py
+Filename: lielab-0.4.0post1.dist-info/METADATA
 Comment: 
 
-Filename: lielab/cppLielab.cp39-win_amd64.pyd
+Filename: lielab-0.4.0post1.dist-info/RECORD
 Comment: 
 
-Filename: lielab/domain/__init__.py
+Filename: lielab-0.4.0post1.dist-info/top_level.txt
+Comment: 
+
+Filename: lielab-0.4.0post1.dist-info/WHEEL
+Comment: 
+
+Filename: lielab/cppLielab.cpython-311-x86_64-linux-gnu.so
 Comment: 
 
 Filename: lielab/domain/domain.py
 Comment: 
 
+Filename: lielab/domain/__init__.py
+Comment: 
+
 Filename: lielab/dynamics/__init__.py
 Comment: 
 
 Filename: lielab/functions/__init__.py
 Comment: 
 
 Filename: lielab/kinematics/__init__.py
 Comment: 
 
-Filename: lielab/optim/__init__.py
-Comment: 
-
 Filename: lielab/optim/optim.py
 Comment: 
 
-Filename: lielab/testing/__init__.py
+Filename: lielab/optim/__init__.py
 Comment: 
 
 Filename: lielab/testing/test_main.py
 Comment: 
 
-Filename: lielab/topos/__init__.py
+Filename: lielab/testing/__init__.py
 Comment: 
 
 Filename: lielab/topos/topos.py
 Comment: 
 
-Filename: lielab/transform/__init__.py
-Comment: 
-
-Filename: lielab-0.4.0.dist-info/METADATA
-Comment: 
-
-Filename: lielab-0.4.0.dist-info/WHEEL
+Filename: lielab/topos/__init__.py
 Comment: 
 
-Filename: lielab-0.4.0.dist-info/top_level.txt
+Filename: lielab/transform/__init__.py
 Comment: 
 
-Filename: lielab-0.4.0.dist-info/RECORD
+Filename: lielab/__init__.py
 Comment: 
 
 Zip file comment:
```

## lielab/__init__.py

 * *Ordering differences only*

```diff
@@ -1,12 +1,12 @@
-from .cppLielab import ALGO_STATUS
-
-from .cppLielab import __author__, __contact__, __location__, __version__
-
-from . import testing
-
-from . import domain
-from . import functions
-from . import kinematics
-from . import optim
-from . import topos
-from . import transform
+from .cppLielab import ALGO_STATUS
+
+from .cppLielab import __author__, __contact__, __location__, __version__
+
+from . import testing
+
+from . import domain
+from . import functions
+from . import kinematics
+from . import optim
+from . import topos
+from . import transform
```

## lielab/domain/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-# C++ imports
-from ..cppLielab.domain import *
-
-# Python imports
+# C++ imports
+from ..cppLielab.domain import *
+
+# Python imports
```

## lielab/domain/domain.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-pass
+pass
```

## lielab/dynamics/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from ..cppLielab.dynamics import *
+from ..cppLielab.dynamics import *
```

## lielab/functions/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from ..cppLielab.functions import *
+from ..cppLielab.functions import *
```

## lielab/kinematics/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-# C++ imports
-from ..cppLielab.kinematics import *
+# C++ imports
+from ..cppLielab.kinematics import *
```

## lielab/optim/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from .optim import opt_golden, hnewton
+from .optim import opt_golden, hnewton
```

## lielab/optim/optim.py

 * *Ordering differences only*

```diff
@@ -1,55 +1,55 @@
-from ..cppLielab.optim import opt_golden as _opt_golden
-from ..cppLielab.optim import hnewton as _hnewton
-from lielab import ALGO_STATUS
-import numpy as np
-
-class opt_golden(_opt_golden):
-    def __call__(self, function):
-        self.init()
-
-        while (self.algo_status == ALGO_STATUS.OK):
-            self._f1 = function(self._X1)
-            self.num_objective_evals += 1
-
-            self._f2 = function(self._X2)
-            self.num_objective_evals += 1
-            self.step()
-        
-        self._f1 = function(self._X1)
-        self.num_objective_evals += 1
-
-        self._f2 = function(self._X2)
-        self.num_objective_evals += 1
-
-        if (self._f1 < self._f2):
-            self.val_objective = self._f1
-            self._X = self._X1
-        else:
-            self.val_objective = self._f2
-            self._X = self._X2
-
-        return self._X
-
-class hnewton(_hnewton):
-    def __call__(self, fun, m0):
-        self.init(m0, fun(m0))
-
-        while (self.algo_status == ALGO_STATUS.OK):
-            self.step0()
-            self.fnext = fun(self.mnext)
-            self.step1()
-            self.fnext = fun(self.mnext)
-
-        self.m = self.mnext
-
-        return self.m
-
-# class search_linearx(_search_linearx):
-#     def __call__(self, function, x0):
-#         self.init(x0)
-#         x = x0
-
-#         while (self.algo_status == ALGO_STATUS.OK):
-#             x = self.step(x, function(x))
-
-#         return x
+from ..cppLielab.optim import opt_golden as _opt_golden
+from ..cppLielab.optim import hnewton as _hnewton
+from lielab import ALGO_STATUS
+import numpy as np
+
+class opt_golden(_opt_golden):
+    def __call__(self, function):
+        self.init()
+
+        while (self.algo_status == ALGO_STATUS.OK):
+            self._f1 = function(self._X1)
+            self.num_objective_evals += 1
+
+            self._f2 = function(self._X2)
+            self.num_objective_evals += 1
+            self.step()
+        
+        self._f1 = function(self._X1)
+        self.num_objective_evals += 1
+
+        self._f2 = function(self._X2)
+        self.num_objective_evals += 1
+
+        if (self._f1 < self._f2):
+            self.val_objective = self._f1
+            self._X = self._X1
+        else:
+            self.val_objective = self._f2
+            self._X = self._X2
+
+        return self._X
+
+class hnewton(_hnewton):
+    def __call__(self, fun, m0):
+        self.init(m0, fun(m0))
+
+        while (self.algo_status == ALGO_STATUS.OK):
+            self.step0()
+            self.fnext = fun(self.mnext)
+            self.step1()
+            self.fnext = fun(self.mnext)
+
+        self.m = self.mnext
+
+        return self.m
+
+# class search_linearx(_search_linearx):
+#     def __call__(self, function, x0):
+#         self.init(x0)
+#         x = x0
+
+#         while (self.algo_status == ALGO_STATUS.OK):
+#             x = self.step(x, function(x))
+
+#         return x
```

## lielab/testing/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from .test_main import *
+from .test_main import *
```

## lielab/testing/test_main.py

 * *Ordering differences only*

```diff
@@ -1,46 +1,46 @@
-import numpy as np
-
-TOL_FINE = 1e-6
-TOL_COARSE = 1e-3
-
-an_int = int(2)
-a_double = float(2)
-an_imag_int = 2j # TODO: I think this is actually just a double
-an_imag_double = 2.0j
-
-def assert_matrix(mat1: np.ndarray, mat2: np.ndarray) -> None:
-    if isinstance(mat1, np.ndarray):
-        pass
-    else:
-        mat1 = mat1.get_matrix()
-
-    r1 = mat1.shape[0]
-    if len(mat1.shape) == 1:
-        c1 = 0
-    else:
-        c1 = mat1.shape[1]
-    
-    if isinstance(mat2, np.ndarray):
-        pass
-    else:
-        mat2 = mat2.get_matrix()
-    
-    r2 = mat2.shape[0]
-    if len(mat2.shape) == 1:
-        c2 = 0
-    else:
-        c2 = mat2.shape[1]
-    
-    assert r1 == r2
-    assert c1 == c2
-
-    if (c1 != 0 and c2 != 0):
-        for ii in range(r1):
-            for jj in range(c1):
-                assert abs(mat1[ii,jj] - mat2[ii,jj]) < TOL_FINE
-    else:
-        for ii in range(r1):
-            assert abs(mat1[ii] - mat2[ii]) < TOL_FINE
-
-def assert_domain(d1, d2):
-    assert_matrix(d1.get_matrix(), d2.get_matrix())
+import numpy as np
+
+TOL_FINE = 1e-6
+TOL_COARSE = 1e-3
+
+an_int = int(2)
+a_double = float(2)
+an_imag_int = 2j # TODO: I think this is actually just a double
+an_imag_double = 2.0j
+
+def assert_matrix(mat1: np.ndarray, mat2: np.ndarray) -> None:
+    if isinstance(mat1, np.ndarray):
+        pass
+    else:
+        mat1 = mat1.get_matrix()
+
+    r1 = mat1.shape[0]
+    if len(mat1.shape) == 1:
+        c1 = 0
+    else:
+        c1 = mat1.shape[1]
+    
+    if isinstance(mat2, np.ndarray):
+        pass
+    else:
+        mat2 = mat2.get_matrix()
+    
+    r2 = mat2.shape[0]
+    if len(mat2.shape) == 1:
+        c2 = 0
+    else:
+        c2 = mat2.shape[1]
+    
+    assert r1 == r2
+    assert c1 == c2
+
+    if (c1 != 0 and c2 != 0):
+        for ii in range(r1):
+            for jj in range(c1):
+                assert abs(mat1[ii,jj] - mat2[ii,jj]) < TOL_FINE
+    else:
+        for ii in range(r1):
+            assert abs(mat1[ii] - mat2[ii]) < TOL_FINE
+
+def assert_domain(d1, d2):
+    assert_matrix(d1.get_matrix(), d2.get_matrix())
```

## lielab/topos/__init__.py

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-# Need to list every function and class to prevent collisions
-# C++ Imports
-from ..cppLielab.topos import Ad, dexp, dexpinv, exp, log
-from ..cppLielab.topos import RKMETHOD
-from ..cppLielab.topos import IntegralCurve
-
-# Python imports
-from .topos import MuntheKaas, Flow, CustomMuntheKaas
-
+# Need to list every function and class to prevent collisions
+# C++ Imports
+from ..cppLielab.topos import Ad, dexp, dexpinv, exp, log
+from ..cppLielab.topos import RKMETHOD
+from ..cppLielab.topos import IntegralCurve
+
+# Python imports
+from .topos import MuntheKaas, Flow, CustomMuntheKaas
+
```

## lielab/topos/topos.py

 * *Ordering differences only*

```diff
@@ -1,219 +1,219 @@
-from lielab import ALGO_STATUS
-from lielab.domain import CompositeAlgebra, CompositeManifold
-from lielab.topos import IntegralCurve
-from lielab.cppLielab.topos import Flow as _Flow
-from lielab.cppLielab.topos import MuntheKaas as _MuntheKaas
-from lielab.cppLielab.topos import TimeStepper as _TimeStepper
-from lielab.cppLielab.topos import TSOutput
-import numpy as np
-
-# Import hnewton as a python object
-from lielab.optim import hnewton
-
-class MuntheKaas(_MuntheKaas):
-    """
-    MuntheKaas integrator that maximizes time spent in C++
-    for performance.
-    """
-    
-    def __call__(self, vectorfield, y0, t0, dt):
-        self.init(t0, y0, dt, vectorfield(t0, y0))
-
-        while (self.algo_status == ALGO_STATUS.OK):
-            self.step_0()
-            self.set_dy(vectorfield(self.next_t, self.next_y))
-            self.step_1()
-
-        return self.postprocess()
-
-
-class CustomMuntheKaas(_TimeStepper):
-    """
-    MuntheKaas integrator with customizable actions.
-    """
-
-    def __init__(self, *args, **kwargs):
-        """
-        Instantiates a new MuntheKaas object.
-        """
-
-        super(CustomMuntheKaas, self).__init__(*args, **kwargs)
-
-        from lielab.functions import left_product
-        from lielab.topos import exp, dexpinv
-        # self.RKT = RKTYPE::RKTYPE_EXPLICIT; # TODO:
-
-        self.action = left_product
-        self.phi = exp
-        self.dphiinv = dexpinv
-
-        self._t0 = None
-        self._y0 = None
-        self._dt = None
-
-        self.next_t = None
-        self.next_y = None
-
-        self._dy = None
-        self._U = None
-        self._KK = None
-
-    def init(self, t0, y0, dt, dy0):
-        """
-        Initializes the MuntheKaas process.
-        """
-        
-        super(CustomMuntheKaas, self).init()
-
-        self._t0 = t0
-        self._y0 = y0
-        self._dt = dt
-        self._KK = [CompositeAlgebra()]*self.n
-        self._KK[0] = dy0
-        self._dy = dy0
-        self._U = 0*dy0
-
-        if (self.iterations >= self.n - 1):
-            self.algo_status = ALGO_STATUS.FINISHED
-        
-    def step_0(self):
-        """
-        Advances the solution to current iteration and returns pair
-        (next_t, next_y) to be evaluated by the vectorfield.
-        """
-
-        self._U *= 0
-
-        for jj in range(self.iterations + 1):
-            self._U += self._dt*self.A[self.iterations+1, jj]*self._KK[jj]
-        
-        self.next_y = self.action(self.phi(self._U), self._y0)
-        self.next_t = self._t0 + self._dt*self.C[self.iterations + 1]
-    
-    def set_dy(self, dy):
-        """
-        Sets the current vectorfield value. Do this after step_0()
-        and before step_1().
-        """
-
-        self._dy = dy
-
-    def step_1(self):
-        """
-        Evaluates the $ d phi^{-1} u ( xi(s,y)) $ map.
-        """
-
-        self._KK[self.iterations + 1] = self.dphiinv(self._U, self._dy, self.n - 1)
-
-        super(CustomMuntheKaas, self).step()
-
-        if (self.iterations == self.n - 1):
-            self.algo_status = ALGO_STATUS.FINISHED
-    
-    def postprocess(self):
-        Ulow = 0*self._KK[0]
-        Uhigh = 0*self._KK[0]
-
-        for ii in range(self.n):
-            Ulow += self._dt*self.B[ii]*self._KK[ii]
-
-        low = self.action(self.phi(Ulow), self._y0)
-
-        if self.variable_step:
-            for ii in range(self.n):
-                Uhigh += self._dt*self.Bhat[ii]*self._KK[ii]
-            
-            high = self.action(self.phi(Uhigh), self._y0)
-            error = np.linalg.norm(Uhigh.get_vector() - Ulow.get_vector())
-            return TSOutput(low, high, error)
-        
-        return TSOutput(low)
-    
-    def __call__(self, vectorfield, y0, t0, dt):
-        self.init(t0, y0, dt, vectorfield(t0, y0))
-
-        while (self.algo_status == ALGO_STATUS.OK):
-            self.step_0()
-            self.set_dy(vectorfield(self.next_t, self.next_y))
-            self.step_1()
-        
-        return self.postprocess()
-
-
-class Flow(_Flow):
-    search = hnewton()
-    stepper = MuntheKaas()
-
-    def __call__(self, vectorfield, tspan, y0, *args):
-        from lielab.domain import rn, RN, CompositeAlgebra, CompositeManifold
-
-        # Check if the solution we're running has an event
-        has_event = False
-        if len(args) > 0:
-            has_event = True
-            event = args[0]
-        
-        # Check the type of inputs
-        dy0 = vectorfield(tspan[0], y0)
-
-        if isinstance(dy0, np.ndarray) or isinstance(dy0, list):
-            # NumPy and list type inputs, we need to wrap these in
-            # sophus objects
-            _y0 = CompositeManifold([RN(y0)])
-            def _vectorfield(_t, M):
-                _RN = M.space[0]
-                _states = _RN.serialize()
-                gradient = vectorfield(_t, _states)
-                dx = rn(gradient)
-                return CompositeAlgebra([dx])
-            
-            if has_event:
-                def _event(_t, M):
-                    _RN = M.space[0]
-                    _states = _RN.serialize()
-                    return event(_t, _states)
-        else:
-            # Assume these are sophus type inputs and
-            # don't need to be wrapped
-            _y0 = y0
-            _vectorfield = vectorfield
-            if has_event:
-                _event = event
-        
-        # Initialize the Flow object
-        self.init(tspan, _y0)
-
-        # Main loop. Run until algorithm says it's done
-        while (self.algo_status == ALGO_STATUS.OK):
-            accepted = False
-
-            # This is the RK loop. It's the error control loop that will
-            # change step size until we have an acceptable step
-            while (not accepted):
-                next = self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], self._dt)
-                if has_event:
-                    if _event(self._out.t[self.iterations], self._ynext) > 0 and _event(self._out.t[self.iterations] + self._dt, next.high) <= 0:
-                        self.search.lower = CompositeAlgebra([rn([self.tol])])
-                        self.search.upper = CompositeAlgebra([rn([self._dt])])
-
-                        def sfun(sdt):
-                            _sdt = sdt.space[0](0)
-                            return _event(self._out.t[self.iterations] + _sdt, self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], _sdt).high)
-
-                        temp_dt = self.search(sfun, CompositeAlgebra([rn([self._dt/2])]))
-                        self._dt = temp_dt.space[0](0)
-                        next = self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], self._dt)
-
-                accepted = self.step0(next)
-            
-            # We have an acceptable step at this point. Step the solution forward by one
-            self.step()
-
-            # If there's an event, check to see if conditions are met
-            # This will stop integration if an event returns <= 0
-            if has_event:
-                self.stepE(_event(self._out.t[self.iterations], self._ynext))
-        
-        self.postprocess()
-        
-        return IntegralCurve(self._out)
+from lielab import ALGO_STATUS
+from lielab.domain import CompositeAlgebra, CompositeManifold
+from lielab.topos import IntegralCurve
+from lielab.cppLielab.topos import Flow as _Flow
+from lielab.cppLielab.topos import MuntheKaas as _MuntheKaas
+from lielab.cppLielab.topos import TimeStepper as _TimeStepper
+from lielab.cppLielab.topos import TSOutput
+import numpy as np
+
+# Import hnewton as a python object
+from lielab.optim import hnewton
+
+class MuntheKaas(_MuntheKaas):
+    """
+    MuntheKaas integrator that maximizes time spent in C++
+    for performance.
+    """
+    
+    def __call__(self, vectorfield, y0, t0, dt):
+        self.init(t0, y0, dt, vectorfield(t0, y0))
+
+        while (self.algo_status == ALGO_STATUS.OK):
+            self.step_0()
+            self.set_dy(vectorfield(self.next_t, self.next_y))
+            self.step_1()
+
+        return self.postprocess()
+
+
+class CustomMuntheKaas(_TimeStepper):
+    """
+    MuntheKaas integrator with customizable actions.
+    """
+
+    def __init__(self, *args, **kwargs):
+        """
+        Instantiates a new MuntheKaas object.
+        """
+
+        super(CustomMuntheKaas, self).__init__(*args, **kwargs)
+
+        from lielab.functions import left_product
+        from lielab.topos import exp, dexpinv
+        # self.RKT = RKTYPE::RKTYPE_EXPLICIT; # TODO:
+
+        self.action = left_product
+        self.phi = exp
+        self.dphiinv = dexpinv
+
+        self._t0 = None
+        self._y0 = None
+        self._dt = None
+
+        self.next_t = None
+        self.next_y = None
+
+        self._dy = None
+        self._U = None
+        self._KK = None
+
+    def init(self, t0, y0, dt, dy0):
+        """
+        Initializes the MuntheKaas process.
+        """
+        
+        super(CustomMuntheKaas, self).init()
+
+        self._t0 = t0
+        self._y0 = y0
+        self._dt = dt
+        self._KK = [CompositeAlgebra()]*self.n
+        self._KK[0] = dy0
+        self._dy = dy0
+        self._U = 0*dy0
+
+        if (self.iterations >= self.n - 1):
+            self.algo_status = ALGO_STATUS.FINISHED
+        
+    def step_0(self):
+        """
+        Advances the solution to current iteration and returns pair
+        (next_t, next_y) to be evaluated by the vectorfield.
+        """
+
+        self._U *= 0
+
+        for jj in range(self.iterations + 1):
+            self._U += self._dt*self.A[self.iterations+1, jj]*self._KK[jj]
+        
+        self.next_y = self.action(self.phi(self._U), self._y0)
+        self.next_t = self._t0 + self._dt*self.C[self.iterations + 1]
+    
+    def set_dy(self, dy):
+        """
+        Sets the current vectorfield value. Do this after step_0()
+        and before step_1().
+        """
+
+        self._dy = dy
+
+    def step_1(self):
+        """
+        Evaluates the $ d phi^{-1} u ( xi(s,y)) $ map.
+        """
+
+        self._KK[self.iterations + 1] = self.dphiinv(self._U, self._dy, self.n - 1)
+
+        super(CustomMuntheKaas, self).step()
+
+        if (self.iterations == self.n - 1):
+            self.algo_status = ALGO_STATUS.FINISHED
+    
+    def postprocess(self):
+        Ulow = 0*self._KK[0]
+        Uhigh = 0*self._KK[0]
+
+        for ii in range(self.n):
+            Ulow += self._dt*self.B[ii]*self._KK[ii]
+
+        low = self.action(self.phi(Ulow), self._y0)
+
+        if self.variable_step:
+            for ii in range(self.n):
+                Uhigh += self._dt*self.Bhat[ii]*self._KK[ii]
+            
+            high = self.action(self.phi(Uhigh), self._y0)
+            error = np.linalg.norm(Uhigh.get_vector() - Ulow.get_vector())
+            return TSOutput(low, high, error)
+        
+        return TSOutput(low)
+    
+    def __call__(self, vectorfield, y0, t0, dt):
+        self.init(t0, y0, dt, vectorfield(t0, y0))
+
+        while (self.algo_status == ALGO_STATUS.OK):
+            self.step_0()
+            self.set_dy(vectorfield(self.next_t, self.next_y))
+            self.step_1()
+        
+        return self.postprocess()
+
+
+class Flow(_Flow):
+    search = hnewton()
+    stepper = MuntheKaas()
+
+    def __call__(self, vectorfield, tspan, y0, *args):
+        from lielab.domain import rn, RN, CompositeAlgebra, CompositeManifold
+
+        # Check if the solution we're running has an event
+        has_event = False
+        if len(args) > 0:
+            has_event = True
+            event = args[0]
+        
+        # Check the type of inputs
+        dy0 = vectorfield(tspan[0], y0)
+
+        if isinstance(dy0, np.ndarray) or isinstance(dy0, list):
+            # NumPy and list type inputs, we need to wrap these in
+            # sophus objects
+            _y0 = CompositeManifold([RN(y0)])
+            def _vectorfield(_t, M):
+                _RN = M.space[0]
+                _states = _RN.serialize()
+                gradient = vectorfield(_t, _states)
+                dx = rn(gradient)
+                return CompositeAlgebra([dx])
+            
+            if has_event:
+                def _event(_t, M):
+                    _RN = M.space[0]
+                    _states = _RN.serialize()
+                    return event(_t, _states)
+        else:
+            # Assume these are sophus type inputs and
+            # don't need to be wrapped
+            _y0 = y0
+            _vectorfield = vectorfield
+            if has_event:
+                _event = event
+        
+        # Initialize the Flow object
+        self.init(tspan, _y0)
+
+        # Main loop. Run until algorithm says it's done
+        while (self.algo_status == ALGO_STATUS.OK):
+            accepted = False
+
+            # This is the RK loop. It's the error control loop that will
+            # change step size until we have an acceptable step
+            while (not accepted):
+                next = self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], self._dt)
+                if has_event:
+                    if _event(self._out.t[self.iterations], self._ynext) > 0 and _event(self._out.t[self.iterations] + self._dt, next.high) <= 0:
+                        self.search.lower = CompositeAlgebra([rn([self.tol])])
+                        self.search.upper = CompositeAlgebra([rn([self._dt])])
+
+                        def sfun(sdt):
+                            _sdt = sdt.space[0](0)
+                            return _event(self._out.t[self.iterations] + _sdt, self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], _sdt).high)
+
+                        temp_dt = self.search(sfun, CompositeAlgebra([rn([self._dt/2])]))
+                        self._dt = temp_dt.space[0](0)
+                        next = self.stepper(_vectorfield, self._ynext, self._out.t[self.iterations], self._dt)
+
+                accepted = self.step0(next)
+            
+            # We have an acceptable step at this point. Step the solution forward by one
+            self.step()
+
+            # If there's an event, check to see if conditions are met
+            # This will stop integration if an event returns <= 0
+            if has_event:
+                self.stepE(_event(self._out.t[self.iterations], self._ynext))
+        
+        self.postprocess()
+        
+        return IntegralCurve(self._out)
```

## lielab/transform/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-# C++ imports
-from ..cppLielab.transform import *
+# C++ imports
+from ..cppLielab.transform import *
```

