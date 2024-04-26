# Comparing `tmp/KratosStatisticsApplication-9.4.5-cp39-cp39-win_amd64.whl.zip` & `tmp/KratosStatisticsApplication-9.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,423 +1,677 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    832424 (00000000000CB3A8h)
-  Actual end-cent-dir record offset:        832402 (00000000000CB392h)
-  Expected end-cent-dir record offset:      832402 (00000000000CB392h)
+  Zip archive file size:                   2248967 (0000000000225107h)
+  Actual end-cent-dir record offset:       2248945 (00000000002250F1h)
+  Expected end-cent-dir record offset:     2248945 (00000000002250F1h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 14 entries.
-  The central directory is 1440 (00000000000005A0h) bytes long,
+  central directory contains 18 entries.
+  The central directory is 2205 (000000000000089Dh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 830962 (00000000000CADF2h).
+  is 2246740 (0000000000224854h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosStatisticsApplication.pyd
+  KratosMultiphysics/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         586fe233
-  compressed size:                                647307 bytes
-  uncompressed size:                              3240448 bytes
-  length of filename:                             56 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             19 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosStatisticsCore.dll
+  KratosMultiphysics/.libs/
 
-  offset of local header from start of archive:   647393
-                                                  (000000000009E0E1h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   77
+                                                  (000000000000004Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         188b8d72
-  compressed size:                                157575 bytes
-  uncompressed size:                              493568 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:08
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:08 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:08 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             25 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosStatisticsCore.lib
+  KratosMultiphysics/.libs/KratosStatisticsApplication.cpython-39-x86_64-linux-gnu.so
 
-  offset of local header from start of archive:   805047
-                                                  (00000000000C48B7h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   160
+                                                  (00000000000000A0h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         62e8e91a
-  compressed size:                                4734 bytes
-  uncompressed size:                              81868 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         16106552
+  compressed size:                                1554084 bytes
+  uncompressed size:                              6628217 bytes
+  length of filename:                             83 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  KratosMultiphysics/StatisticsApplication/__init__.py
+  KratosMultiphysics/StatisticsApplication/
 
-  offset of local header from start of archive:   809860
-                                                  (00000000000C5B84h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1554385
+                                                  (000000000017B7D1h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         d001c605
-  compressed size:                                132 bytes
-  uncompressed size:                              283 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             41 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
   KratosMultiphysics/StatisticsApplication/method_utilities.py
 
-  offset of local header from start of archive:   810074
-                                                  (00000000000C5C5Ah) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1554484
+                                                  (000000000017B834h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         e7b4e429
-  compressed size:                                400 bytes
-  uncompressed size:                              1184 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         076aa88d
+  compressed size:                                397 bytes
+  uncompressed size:                              1156 bytes
   length of filename:                             60 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
-  KratosMultiphysics/StatisticsApplication/spatial_statistics_process.py
+  KratosMultiphysics/StatisticsApplication/test_utilities.py
 
-  offset of local header from start of archive:   810564
-                                                  (00000000000C5E44h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1554999
+                                                  (000000000017BA37h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         ccbdcbab
-  compressed size:                                3727 bytes
-  uncompressed size:                              17616 bytes
-  length of filename:                             70 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         9d21a7b6
+  compressed size:                                1404 bytes
+  uncompressed size:                              7101 bytes
+  length of filename:                             58 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
 Central directory entry #7:
 ---------------------------
 
-  KratosMultiphysics/StatisticsApplication/spatial_utilities.py
+  KratosMultiphysics/StatisticsApplication/temporal_statistics_process.py
 
-  offset of local header from start of archive:   814391
-                                                  (00000000000C6D37h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1556519
+                                                  (000000000017C027h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         0a4ac522
-  compressed size:                                1895 bytes
-  uncompressed size:                              10543 bytes
-  length of filename:                             61 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         c902105d
+  compressed size:                                1555 bytes
+  uncompressed size:                              5943 bytes
+  length of filename:                             71 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
 Central directory entry #8:
 ---------------------------
 
-  KratosMultiphysics/StatisticsApplication/temporal_statistics_process.py
+  KratosMultiphysics/StatisticsApplication/temporal_utilities.py
 
-  offset of local header from start of archive:   816377
-                                                  (00000000000C74F9h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1558203
+                                                  (000000000017C6BBh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         9c7b9523
-  compressed size:                                1564 bytes
-  uncompressed size:                              6063 bytes
-  length of filename:                             71 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         ccd8564d
+  compressed size:                                567 bytes
+  uncompressed size:                              2254 bytes
+  length of filename:                             62 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
 Central directory entry #9:
 ---------------------------
 
-  KratosMultiphysics/StatisticsApplication/temporal_utilities.py
+  KratosMultiphysics/StatisticsApplication/spatial_utilities.py
 
-  offset of local header from start of archive:   818042
-                                                  (00000000000C7B7Ah) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1558890
+                                                  (000000000017C96Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         03e2634a
-  compressed size:                                574 bytes
-  uncompressed size:                              2316 bytes
-  length of filename:                             62 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         b4e945ae
+  compressed size:                                1877 bytes
+  uncompressed size:                              10317 bytes
+  length of filename:                             61 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
 Central directory entry #10:
 ---------------------------
 
-  KratosMultiphysics/StatisticsApplication/test_utilities.py
+  KratosMultiphysics/StatisticsApplication/spatial_statistics_process.py
 
-  offset of local header from start of archive:   818708
-                                                  (00000000000C7E14h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1560886
+                                                  (000000000017D136h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         edd4b5d7
-  compressed size:                                1414 bytes
-  uncompressed size:                              7265 bytes
-  length of filename:                             58 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         60727a91
+  compressed size:                                3712 bytes
+  uncompressed size:                              17296 bytes
+  length of filename:                             70 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
 Central directory entry #11:
 ---------------------------
 
-  KratosStatisticsApplication-9.4.5.dist-info/METADATA
+  KratosMultiphysics/StatisticsApplication/__init__.py
 
-  offset of local header from start of archive:   820210
-                                                  (00000000000C83F2h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1564726
+                                                  (000000000017E036h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         b37c9f70
-  compressed size:                                9591 bytes
-  uncompressed size:                              63056 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         7b04f726
+  compressed size:                                127 bytes
+  uncompressed size:                              276 bytes
   length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
 Central directory entry #12:
 ---------------------------
 
-  KratosStatisticsApplication-9.4.5.dist-info/WHEEL
+  KratosStatisticsApplication-9.5.dist-info/
 
-  offset of local header from start of archive:   829883
-                                                  (00000000000CA9BBh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1564963
+                                                  (000000000017E123h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:08
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:08 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:08 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             42 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #13:
+---------------------------
+
+  KratosStatisticsApplication-9.5.dist-info/METADATA
+
+  offset of local header from start of archive:   1565063
+                                                  (000000000017E187h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         1ad59a98
-  compressed size:                                96 bytes
-  uncompressed size:                              100 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         b29c5024
+  compressed size:                                9551 bytes
+  uncompressed size:                              62229 bytes
+  length of filename:                             50 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
-Central directory entry #13:
+Central directory entry #14:
 ---------------------------
 
-  KratosStatisticsApplication-9.4.5.dist-info/top_level.txt
+  KratosStatisticsApplication-9.5.dist-info/WHEEL
 
-  offset of local header from start of archive:   830058
-                                                  (00000000000CAA6Ah) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1574722
+                                                  (0000000000180742h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         90d34e0d
+  compressed size:                                116 bytes
+  uncompressed size:                              148 bytes
+  length of filename:                             47 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #15:
+---------------------------
+
+  KratosStatisticsApplication-9.5.dist-info/top_level.txt
+
+  offset of local header from start of archive:   1574943
+                                                  (000000000018081Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
   32-bit CRC value (hex):                         f32d789f
-  compressed size:                                21 bytes
+  compressed size:                                19 bytes
   uncompressed size:                              19 bytes
-  length of filename:                             57 characters
-  length of extra field:                          0 bytes
+  length of filename:                             55 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
-Central directory entry #14:
+Central directory entry #16:
 ---------------------------
 
-  KratosStatisticsApplication-9.4.5.dist-info/RECORD
+  KratosStatisticsApplication-9.5.dist-info/RECORD
 
-  offset of local header from start of archive:   830166
-                                                  (00000000000CAAD6h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1575075
+                                                  (00000000001808A3h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:34
-  32-bit CRC value (hex):                         b6d7ff3f
-  compressed size:                                716 bytes
-  uncompressed size:                              1545 bytes
-  length of filename:                             50 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:08
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:08 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:08 UTC
+  32-bit CRC value (hex):                         e7b064b9
+  compressed size:                                757 bytes
+  uncompressed size:                              1602 bytes
+  length of filename:                             48 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100664 octal):            -rw-rw-r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #17:
+---------------------------
+
+  KratosStatisticsApplication.libs/
+
+  offset of local header from start of archive:   1575938
+                                                  (0000000000180C02h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:08
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:08 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:08 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             33 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             01B400 hex
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #18:
+---------------------------
+
+  KratosStatisticsApplication.libs/libKratosStatisticsCore-e894e91a.so
+
+  offset of local header from start of archive:   1576029
+                                                  (0000000000180C5Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:02:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:02:02 UTC
+  32-bit CRC value (hex):                         4ec42b56
+  compressed size:                                670585 bytes
+  uncompressed size:                              2844569 bytes
+  length of filename:                             68 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,43 +1,55 @@
-Filename: KratosMultiphysics/.libs/KratosStatisticsApplication.pyd
+Filename: KratosMultiphysics/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosStatisticsCore.dll
+Filename: KratosMultiphysics/.libs/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosStatisticsCore.lib
+Filename: KratosMultiphysics/.libs/KratosStatisticsApplication.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: KratosMultiphysics/StatisticsApplication/__init__.py
+Filename: KratosMultiphysics/StatisticsApplication/
 Comment: 
 
 Filename: KratosMultiphysics/StatisticsApplication/method_utilities.py
 Comment: 
 
-Filename: KratosMultiphysics/StatisticsApplication/spatial_statistics_process.py
+Filename: KratosMultiphysics/StatisticsApplication/test_utilities.py
+Comment: 
+
+Filename: KratosMultiphysics/StatisticsApplication/temporal_statistics_process.py
+Comment: 
+
+Filename: KratosMultiphysics/StatisticsApplication/temporal_utilities.py
 Comment: 
 
 Filename: KratosMultiphysics/StatisticsApplication/spatial_utilities.py
 Comment: 
 
-Filename: KratosMultiphysics/StatisticsApplication/temporal_statistics_process.py
+Filename: KratosMultiphysics/StatisticsApplication/spatial_statistics_process.py
 Comment: 
 
-Filename: KratosMultiphysics/StatisticsApplication/temporal_utilities.py
+Filename: KratosMultiphysics/StatisticsApplication/__init__.py
 Comment: 
 
-Filename: KratosMultiphysics/StatisticsApplication/test_utilities.py
+Filename: KratosStatisticsApplication-9.5.dist-info/
+Comment: 
+
+Filename: KratosStatisticsApplication-9.5.dist-info/METADATA
+Comment: 
+
+Filename: KratosStatisticsApplication-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosStatisticsApplication-9.4.5.dist-info/METADATA
+Filename: KratosStatisticsApplication-9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosStatisticsApplication-9.4.5.dist-info/WHEEL
+Filename: KratosStatisticsApplication-9.5.dist-info/RECORD
 Comment: 
 
-Filename: KratosStatisticsApplication-9.4.5.dist-info/top_level.txt
+Filename: KratosStatisticsApplication.libs/
 Comment: 
 
-Filename: KratosStatisticsApplication-9.4.5.dist-info/RECORD
+Filename: KratosStatisticsApplication.libs/libKratosStatisticsCore-e894e91a.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## KratosMultiphysics/StatisticsApplication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-# Application dependent names and paths
-from KratosMultiphysics import _ImportApplication
-from KratosStatisticsApplication import *
-application = KratosStatisticsApplication()
-application_name = "KratosStatisticsApplication"
-
-_ImportApplication(application, application_name)
+# Application dependent names and paths
+from KratosMultiphysics import _ImportApplication
+from KratosStatisticsApplication import *
+application = KratosStatisticsApplication()
+application_name = "KratosStatisticsApplication"
+
+_ImportApplication(application, application_name)
```

## KratosMultiphysics/StatisticsApplication/method_utilities.py

 * *Ordering differences only*

```diff
@@ -1,28 +1,28 @@
-def GetNormTypeContainer(item_container, norm_type):
-    if (norm_type == "none"):
-        return item_container.ValueMethods
-    else:
-        return item_container.NormMethods
-
-def GetAvailableMethods(item_norm_container):
-    method_info_list = []
-    for method in dir(item_norm_container):
-        if (not method.startswith("__")):
-            method_info_list.append([method.lower(), method])
-
-    method_names_list = [method_info[0] for method_info in method_info_list]
-    method_list = [method_info[1] for method_info in method_info_list]
-
-    return method_names_list, method_list
-
-def GetMethod(item_norm_container, method_name):
-    method_names_list, method_list = GetAvailableMethods(item_norm_container)
-
-    if method_name not in method_names_list:
-        msg = "Unknown method name requested for the container " + str(item_norm_container) + ". [ \"method_name\" = \"" + method_name + "\" ]\n"
-        msg += "Allowed method names are:\n    "
-        msg += "\n    ".join(sorted(method_names_list))
-        raise Exception(msg)
-
-    return getattr(item_norm_container,
-                   method_list[method_names_list.index(method_name)])
+def GetNormTypeContainer(item_container, norm_type):
+    if (norm_type == "none"):
+        return item_container.ValueMethods
+    else:
+        return item_container.NormMethods
+
+def GetAvailableMethods(item_norm_container):
+    method_info_list = []
+    for method in dir(item_norm_container):
+        if (not method.startswith("__")):
+            method_info_list.append([method.lower(), method])
+
+    method_names_list = [method_info[0] for method_info in method_info_list]
+    method_list = [method_info[1] for method_info in method_info_list]
+
+    return method_names_list, method_list
+
+def GetMethod(item_norm_container, method_name):
+    method_names_list, method_list = GetAvailableMethods(item_norm_container)
+
+    if method_name not in method_names_list:
+        msg = "Unknown method name requested for the container " + str(item_norm_container) + ". [ \"method_name\" = \"" + method_name + "\" ]\n"
+        msg += "Allowed method names are:\n    "
+        msg += "\n    ".join(sorted(method_names_list))
+        raise Exception(msg)
+
+    return getattr(item_norm_container,
+                   method_list[method_names_list.index(method_name)])
```

## KratosMultiphysics/StatisticsApplication/spatial_statistics_process.py

 * *Ordering differences only*

```diff
@@ -1,320 +1,320 @@
-import KratosMultiphysics as Kratos
-from KratosMultiphysics.process_factory import KratosProcessFactory
-
-from KratosMultiphysics.StatisticsApplication.method_utilities import GetAvailableMethods
-from KratosMultiphysics.StatisticsApplication.method_utilities import GetNormTypeContainer
-from KratosMultiphysics.StatisticsApplication.spatial_utilities import GetItemContainer
-from KratosMultiphysics.StatisticsApplication.spatial_utilities import GetFormattedValue
-from KratosMultiphysics.time_based_ascii_file_writer_utility import TimeBasedAsciiFileWriterUtility
-
-import KratosMultiphysics.StatisticsApplication.spatial_utilities as SpatialUtilities
-
-from datetime import datetime
-
-
-def Factory(settings, model):
-    if (not isinstance(model, Kratos.Model)):
-        raise Exception(
-            "expected input shall be a Model object, encapsulating a json string"
-        )
-    if (not isinstance(settings, Kratos.Parameters)):
-        raise Exception(
-            "expected input shall be a Parameters object, encapsulating a json string"
-        )
-    return SpatialStatisticsProcess(model, settings["Parameters"])
-
-
-class SpatialStatisticsProcess(Kratos.Process):
-    """A process to calculate spatial statistics on Kratos containers
-
-    This process calculates spatial statistics for given variables in a given container.
-
-    This process is compatible with OpenMP and MPI with restart
-
-    Args:
-        model (Kratos.Model): Model used in problem
-        settings (Kratos.Parameters): Kratos parameter settings for process
-    """
-    def __init__(self, model, settings):
-        Kratos.Process.__init__(self)
-
-        default_parameters = Kratos.Parameters("""
-        {
-            "model_part_name"         : "PLEASE_SPECIFY_MODEL_PART_NAME",
-            "echo_level"              : 0,
-            "computation_processes"   : [],
-            "computation_points"      : [
-                "ExecuteInitialize",
-                "ExecuteInitializeSolutionStep",
-                "Execute",
-                "ExecuteFinalizeSolutionStep"
-            ],
-            "input_variable_settings" : [
-                {
-                    "variable_names" : [],
-                    "norm_type"      : "none",
-                    "container"      : "nodal_historical"
-                }
-            ],
-            "statistics_methods": [
-                {
-                    "method_name"    : "",
-                    "method_settings": {}
-                }
-            ],
-            "output_settings" : {
-                "interval"               : [0.0, "End"],
-                "output_control_variable": "STEP",
-                "output_time_interval"   : 1,
-                "write_kratos_version"   : false,
-                "write_time_stamp"       : false,
-                "output_value_precision" : 5,
-                "output_value_length"    : 14,
-                "output_file_settings"   : {
-                    "file_name"  : "<model_part_name>.dat",
-                    "output_path": "spatial_statistics_output",
-                    "write_buffer_size" : -1
-                }
-            }
-        }  """)
-
-        self.model = model
-        self.settings = settings
-        self.settings.ValidateAndAssignDefaults(default_parameters)
-        self.variables_settings_list = self.settings["input_variable_settings"]
-
-        self.echo_level = self.settings["echo_level"].GetInt()
-
-        self.output_settings = self.settings["output_settings"]
-        self.output_settings["output_file_settings"].ValidateAndAssignDefaults(default_parameters["output_settings"]["output_file_settings"])
-        self.output_settings.RecursivelyValidateAndAssignDefaults(default_parameters["output_settings"])
-
-        self.model_part_name = self.settings["model_part_name"].GetString()
-
-        ## set the input variavle x methods operations list
-        self.list_of_operations = []
-
-        spatial_output_method_info = []
-        for spatial_method_output in dir(SpatialUtilities):
-            if (spatial_method_output.startswith("Spatial") and spatial_method_output.endswith("Output")):
-                spatial_output_method_info.append([spatial_method_output.lower()[7:-6], spatial_method_output])
-
-        spatial_method_output_names_ = [method_info[0] for method_info in spatial_output_method_info]
-        spatial_method_output = [method_info[1] for method_info in spatial_output_method_info]
-
-        for variable_settings in self.settings["input_variable_settings"].values():
-            variable_settings.ValidateAndAssignDefaults(default_parameters["input_variable_settings"][0])
-
-            container_type = variable_settings["container"].GetString()
-            norm_type = variable_settings["norm_type"].GetString()
-
-            container = GetItemContainer(container_type)
-            norm_container = GetNormTypeContainer(container, norm_type)
-            available_methods, _ = GetAvailableMethods(norm_container)
-
-            for variable_name in variable_settings["variable_names"].GetStringArray():
-                if (not Kratos.KratosGlobals.HasVariable(variable_name)):
-                    raise RuntimeError("Variable not found. [ variable_name = " + variable_name + " ]")
-
-                for method_settings in self.settings["statistics_methods"].values():
-                    method_settings.ValidateAndAssignDefaults(default_parameters["statistics_methods"][0])
-
-                    method_name = method_settings["method_name"].GetString()
-                    if method_name == "":
-                        raise RuntimeError("Found an empty method name. {:s}".format(method_settings))
-
-                    if method_name not in spatial_method_output_names_:
-                        msg = "Unknown method name [ \"method_name\" = \"" + method_name + "\" ]\n"
-                        msg += "Allowed method names are:\n    "
-                        msg += "\n    ".join(sorted(spatial_method_output_names_))
-                        raise RuntimeError(msg)
-
-
-                    if not method_name in available_methods:
-                        Kratos.Logger.PrintInfo(self.__class__.__name__, "Skipping statistics output for {:s} method for {:s} in {:s} because {:s} norm type does not support it.".format(method_name, variable_name, container_type, norm_type))
-                    else:
-                        operation_type = getattr(SpatialUtilities, spatial_method_output[spatial_method_output_names_.index(method_name)])
-                        self.list_of_operations.append(operation_type(container_type, norm_type, variable_name, method_settings["method_settings"]))
-
-        ## set the output controller settings
-        self.interval_utility = Kratos.IntervalUtility(self.output_settings)
-        output_control_variable_name = self.output_settings["output_control_variable"].GetString()
-        if (not Kratos.KratosGlobals.HasVariable(output_control_variable_name)):
-            raise RuntimeError("Unknown output control variable. [ \"output_control_variable\" = \"" + output_control_variable_name + "\" ]")
-        output_control_variable_type = Kratos.KratosGlobals.GetVariableType(output_control_variable_name)
-        if (output_control_variable_type not in ["Integer", "Double"]):
-            raise RuntimeError("Unsupported output control variable type for " + output_control_variable_name + " of " + output_control_variable_type + " type. Supported types are Integer and Double only")
-        self.output_control_variable = Kratos.KratosGlobals.GetVariable(output_control_variable_name)
-        self.output_interval = self.output_settings["output_time_interval"].GetDouble()
-        self.output_value_precision = self.output_settings["output_value_precision"].GetInt()
-        self.output_value_length = self.output_settings["output_value_length"].GetInt()
-
-        ## set the execution process
-        self.computation_points = self.settings["computation_points"].GetStringArray()
-        if self.settings["computation_processes"].size() == 0 or len(self.computation_points) == 0:
-            self.statistics_computation_processeses = None
-        else:
-            self.statistics_computation_processeses = KratosProcessFactory(self.model).ConstructListOfProcesses(self.settings["computation_processes"])
-            Kratos.Logger.PrintInfo(self.__class__.__name__, "Created statistics computation processes with following parameters: \n{:s}".format(self.settings["computation_processes"].PrettyPrintJsonString()))
-
-        self.is_headers_written = False
-
-        Kratos.Logger.PrintInfo("SpatialStatisticsProcess", "Initialized statistics process.")
-
-    def Check(self):
-        if (not self.model.HasModelPart(self.model_part_name)):
-            raise RuntimeError(self.model_part_name + " not found.")
-
-        for variable_settings in self.variables_settings_list.values():
-            variable_names_list = variable_settings["variable_names"].GetStringArray()
-
-            container = variable_settings["container"].GetString()
-            if (container == "nodal_historical"):
-                for variable_name in variable_names_list:
-                    variable = Kratos.KratosGlobals.GetVariable(variable_name)
-                    if (not self.__get_model_part().HasNodalSolutionStepVariable(variable)):
-                        raise RuntimeError("Variable " + variable_name + " not found in nodal solution step data of " + self.__get_model_part().Name)
-
-        if self.statistics_computation_processeses is not None:
-            for process in self.statistics_computation_processeses:
-                process.Check()
-
-    def ExecuteInitialize(self):
-        ## set output file path
-        self.output_settings["output_file_settings"]["file_name"].SetString(self.output_settings["output_file_settings"]["file_name"].GetString().replace("<model_part_name>", self.__get_model_part().FullName()))
-        self.output_settings["output_file_settings"]["output_path"].SetString(self.output_settings["output_file_settings"]["output_path"].GetString().replace("<model_part_name>", self.__get_model_part().FullName()))
-
-        self.__write_headers()
-
-        if self.echo_level > 0:
-            Kratos.Logger.PrintInfo(self.__class__.__name__, "List of output operations:\n\t" + "\n\t".join([str(operation) for operation in self.list_of_operations]))
-
-        self.previous_process_info_value = self.__get_model_part().ProcessInfo[self.output_control_variable]
-
-    def ExecuteFinalizeSolutionStep(self):
-        output_control_counter = self.__get_model_part().ProcessInfo[self.output_control_variable]
-
-        if self.interval_utility.IsInInterval(output_control_counter):
-            if (output_control_counter - self.previous_process_info_value) >= self.output_interval:
-
-                # execute the statistics computation process
-                if self.statistics_computation_processeses is not None:
-                    for process in self.statistics_computation_processeses:
-                        for computation_point in self.computation_points:
-                            getattr(process, computation_point)()
-
-                for operation in self.list_of_operations:
-                    operation.Evaluate(self.model_part)
-
-                self.__write_values()
-
-                if self.echo_level > 1:
-                    Kratos.Logger.PrintInfo(self.__class__.__name__, "Calculated statistics on {:s}.".format(self.__get_model_part().FullName()))
-
-                self.previous_process_info_value = output_control_counter
-
-    def ExecuteFinalize(self):
-        if (self.__is_writing_process()):
-            self.output_file.file.write("# End of file.")
-            self.output_file.file.close()
-
-    def __write_headers(self):
-        if (self.__is_writing_process()):
-            kratos_version = "not_given"
-            if (self.output_settings["write_kratos_version"].GetBool()):
-                kratos_version = str(Kratos.KratosGlobals.Kernel.Version())
-
-            time_stamp = "not_specified"
-            if (self.output_settings["write_time_stamp"].GetBool()):
-                time_stamp = str(datetime.now())
-
-            method_name = ""
-            variable_info = ""
-            for operation in self.list_of_operations:
-                if operation.method_name not in method_name:
-                    method_name += operation.method_name + ", "
-                current_variable_info = "{:s}[{:s}, {:s}], ".format(operation.variable_name, operation.norm_type, operation.container_type)
-                if current_variable_info not in variable_info:
-                    variable_info += current_variable_info
-
-            self.headers, self.header_lengths = self.__get_headers()
-
-            msg_header = ""
-            msg_header += "# Spatial statistics process output\n"
-            msg_header += "# Kratos version               : " + kratos_version + "\n"
-            msg_header += "# Timestamp                    : " + time_stamp + "\n"
-            msg_header += "# Method name(s)               : " + method_name[:-2] + "\n"
-            msg_header += "# Variable info(s)             : " + variable_info[:-2] + "\n"
-            msg_header += "# Modelpart name               : " + self.model_part_name + "\n"
-            msg_header += "# Output control variable name : " + self.output_control_variable.Name() + "\n"
-            msg_header += "# ----------------------------------------------------------------------\n"
-            msg_header += "# Headers:\n"
-            msg_header += "#" + " ".join([("{:>" + str(header_length) + "s}").format(header) for header, header_length in zip(self.headers, self.header_lengths)]) + "\n"
-
-            self.output_file = TimeBasedAsciiFileWriterUtility(self.__get_model_part(), self.output_settings["output_file_settings"], msg_header)
-
-            self.is_headers_written = True
-
-    def __get_headers(self):
-        # check whether only one variable with one
-        variable_info = ""
-        for operation in self.list_of_operations:
-            current_variable_info = "{:s}[{:s}, {:s}], ".format(operation.variable_name, operation.norm_type, operation.container_type)
-            if current_variable_info not in variable_info:
-                variable_info += current_variable_info
-
-        headers = ["\"TIME\""]
-        header_lengths = [max(6, self.output_value_length)]
-        if self.output_control_variable != Kratos.TIME:
-            headers.append("\"" + self.output_control_variable.Name() + "\"")
-            header_lengths.append(max(len(self.output_control_variable.Name()) + 2, self.output_value_length))
-
-        # found only one variable type info
-        if variable_info.count(",") == 2:
-            header_formatting_string = "\"<HEADER_NAME><COMPONENT>\""
-        else:
-            header_formatting_string = "\"<VARIABLE_NAME><COMPONENT> [ <NORM_TYPE> | <CONTAINER_TYPE> ] <HEADER_NAME>\""
-
-        variable_components = {
-            "Double": [""],
-            "Array" : ["_X", "_Y", "_Z"]
-        }
-
-        for operation in self.list_of_operations:
-            if operation.norm_type == "none":
-                comps_list = variable_components[Kratos.KratosGlobals.GetVariableType(operation.variable.Name())]
-            else:
-                comps_list = variable_components["Double"]
-
-            for current_header, current_header_length in zip(operation.GetHeaders(), operation.GetValueLengths(self.output_value_length)):
-                for comp in comps_list:
-                    current_header_name = str(header_formatting_string)
-
-                    current_header_name = current_header_name.replace("<HEADER_NAME>", current_header)
-                    current_header_name = current_header_name.replace("<VARIABLE_NAME>", operation.variable.Name())
-                    current_header_name = current_header_name.replace("<COMPONENT>", comp)
-                    current_header_name = current_header_name.replace("<NORM_TYPE>", operation.norm_type)
-                    current_header_name = current_header_name.replace("<CONTAINER_TYPE>", operation.container_type)
-
-                    headers.append(current_header_name)
-                    header_lengths.append(max(len(current_header_name), current_header_length))
-
-        return headers, header_lengths
-
-    def __write_values(self):
-        if (self.__is_writing_process()):
-            values = [GetFormattedValue(self.__get_model_part().ProcessInfo[Kratos.TIME], self.output_value_length, self.output_value_precision)[0]]
-            if self.output_control_variable != Kratos.TIME:
-                values.append(GetFormattedValue(self.__get_model_part().ProcessInfo[self.output_control_variable], self.output_value_length, self.output_value_precision)[0])
-            for operation in self.list_of_operations:
-                values.extend(operation.GetValues(self.output_value_length, self.output_value_precision))
-            self.output_file.file.write(" " + " ".join([("{:>" + str(header_length) + "s}").format(value) for value, header_length in zip(values, self.header_lengths)]) + "\n")
-
-    def __get_model_part(self):
-        if (not hasattr(self, "model_part")):
-            self.model_part = self.model[self.model_part_name]
-
-        return self.model_part
-
-    def __is_writing_process(self):
-        return (self.__get_model_part().GetCommunicator().MyPID() == 0)
+import KratosMultiphysics as Kratos
+from KratosMultiphysics.process_factory import KratosProcessFactory
+
+from KratosMultiphysics.StatisticsApplication.method_utilities import GetAvailableMethods
+from KratosMultiphysics.StatisticsApplication.method_utilities import GetNormTypeContainer
+from KratosMultiphysics.StatisticsApplication.spatial_utilities import GetItemContainer
+from KratosMultiphysics.StatisticsApplication.spatial_utilities import GetFormattedValue
+from KratosMultiphysics.time_based_ascii_file_writer_utility import TimeBasedAsciiFileWriterUtility
+
+import KratosMultiphysics.StatisticsApplication.spatial_utilities as SpatialUtilities
+
+from datetime import datetime
+
+
+def Factory(settings, model):
+    if (not isinstance(model, Kratos.Model)):
+        raise Exception(
+            "expected input shall be a Model object, encapsulating a json string"
+        )
+    if (not isinstance(settings, Kratos.Parameters)):
+        raise Exception(
+            "expected input shall be a Parameters object, encapsulating a json string"
+        )
+    return SpatialStatisticsProcess(model, settings["Parameters"])
+
+
+class SpatialStatisticsProcess(Kratos.Process):
+    """A process to calculate spatial statistics on Kratos containers
+
+    This process calculates spatial statistics for given variables in a given container.
+
+    This process is compatible with OpenMP and MPI with restart
+
+    Args:
+        model (Kratos.Model): Model used in problem
+        settings (Kratos.Parameters): Kratos parameter settings for process
+    """
+    def __init__(self, model, settings):
+        Kratos.Process.__init__(self)
+
+        default_parameters = Kratos.Parameters("""
+        {
+            "model_part_name"         : "PLEASE_SPECIFY_MODEL_PART_NAME",
+            "echo_level"              : 0,
+            "computation_processes"   : [],
+            "computation_points"      : [
+                "ExecuteInitialize",
+                "ExecuteInitializeSolutionStep",
+                "Execute",
+                "ExecuteFinalizeSolutionStep"
+            ],
+            "input_variable_settings" : [
+                {
+                    "variable_names" : [],
+                    "norm_type"      : "none",
+                    "container"      : "nodal_historical"
+                }
+            ],
+            "statistics_methods": [
+                {
+                    "method_name"    : "",
+                    "method_settings": {}
+                }
+            ],
+            "output_settings" : {
+                "interval"               : [0.0, "End"],
+                "output_control_variable": "STEP",
+                "output_time_interval"   : 1,
+                "write_kratos_version"   : false,
+                "write_time_stamp"       : false,
+                "output_value_precision" : 5,
+                "output_value_length"    : 14,
+                "output_file_settings"   : {
+                    "file_name"  : "<model_part_name>.dat",
+                    "output_path": "spatial_statistics_output",
+                    "write_buffer_size" : -1
+                }
+            }
+        }  """)
+
+        self.model = model
+        self.settings = settings
+        self.settings.ValidateAndAssignDefaults(default_parameters)
+        self.variables_settings_list = self.settings["input_variable_settings"]
+
+        self.echo_level = self.settings["echo_level"].GetInt()
+
+        self.output_settings = self.settings["output_settings"]
+        self.output_settings["output_file_settings"].ValidateAndAssignDefaults(default_parameters["output_settings"]["output_file_settings"])
+        self.output_settings.RecursivelyValidateAndAssignDefaults(default_parameters["output_settings"])
+
+        self.model_part_name = self.settings["model_part_name"].GetString()
+
+        ## set the input variavle x methods operations list
+        self.list_of_operations = []
+
+        spatial_output_method_info = []
+        for spatial_method_output in dir(SpatialUtilities):
+            if (spatial_method_output.startswith("Spatial") and spatial_method_output.endswith("Output")):
+                spatial_output_method_info.append([spatial_method_output.lower()[7:-6], spatial_method_output])
+
+        spatial_method_output_names_ = [method_info[0] for method_info in spatial_output_method_info]
+        spatial_method_output = [method_info[1] for method_info in spatial_output_method_info]
+
+        for variable_settings in self.settings["input_variable_settings"].values():
+            variable_settings.ValidateAndAssignDefaults(default_parameters["input_variable_settings"][0])
+
+            container_type = variable_settings["container"].GetString()
+            norm_type = variable_settings["norm_type"].GetString()
+
+            container = GetItemContainer(container_type)
+            norm_container = GetNormTypeContainer(container, norm_type)
+            available_methods, _ = GetAvailableMethods(norm_container)
+
+            for variable_name in variable_settings["variable_names"].GetStringArray():
+                if (not Kratos.KratosGlobals.HasVariable(variable_name)):
+                    raise RuntimeError("Variable not found. [ variable_name = " + variable_name + " ]")
+
+                for method_settings in self.settings["statistics_methods"].values():
+                    method_settings.ValidateAndAssignDefaults(default_parameters["statistics_methods"][0])
+
+                    method_name = method_settings["method_name"].GetString()
+                    if method_name == "":
+                        raise RuntimeError("Found an empty method name. {:s}".format(method_settings))
+
+                    if method_name not in spatial_method_output_names_:
+                        msg = "Unknown method name [ \"method_name\" = \"" + method_name + "\" ]\n"
+                        msg += "Allowed method names are:\n    "
+                        msg += "\n    ".join(sorted(spatial_method_output_names_))
+                        raise RuntimeError(msg)
+
+
+                    if not method_name in available_methods:
+                        Kratos.Logger.PrintInfo(self.__class__.__name__, "Skipping statistics output for {:s} method for {:s} in {:s} because {:s} norm type does not support it.".format(method_name, variable_name, container_type, norm_type))
+                    else:
+                        operation_type = getattr(SpatialUtilities, spatial_method_output[spatial_method_output_names_.index(method_name)])
+                        self.list_of_operations.append(operation_type(container_type, norm_type, variable_name, method_settings["method_settings"]))
+
+        ## set the output controller settings
+        self.interval_utility = Kratos.IntervalUtility(self.output_settings)
+        output_control_variable_name = self.output_settings["output_control_variable"].GetString()
+        if (not Kratos.KratosGlobals.HasVariable(output_control_variable_name)):
+            raise RuntimeError("Unknown output control variable. [ \"output_control_variable\" = \"" + output_control_variable_name + "\" ]")
+        output_control_variable_type = Kratos.KratosGlobals.GetVariableType(output_control_variable_name)
+        if (output_control_variable_type not in ["Integer", "Double"]):
+            raise RuntimeError("Unsupported output control variable type for " + output_control_variable_name + " of " + output_control_variable_type + " type. Supported types are Integer and Double only")
+        self.output_control_variable = Kratos.KratosGlobals.GetVariable(output_control_variable_name)
+        self.output_interval = self.output_settings["output_time_interval"].GetDouble()
+        self.output_value_precision = self.output_settings["output_value_precision"].GetInt()
+        self.output_value_length = self.output_settings["output_value_length"].GetInt()
+
+        ## set the execution process
+        self.computation_points = self.settings["computation_points"].GetStringArray()
+        if self.settings["computation_processes"].size() == 0 or len(self.computation_points) == 0:
+            self.statistics_computation_processeses = None
+        else:
+            self.statistics_computation_processeses = KratosProcessFactory(self.model).ConstructListOfProcesses(self.settings["computation_processes"])
+            Kratos.Logger.PrintInfo(self.__class__.__name__, "Created statistics computation processes with following parameters: \n{:s}".format(self.settings["computation_processes"].PrettyPrintJsonString()))
+
+        self.is_headers_written = False
+
+        Kratos.Logger.PrintInfo("SpatialStatisticsProcess", "Initialized statistics process.")
+
+    def Check(self):
+        if (not self.model.HasModelPart(self.model_part_name)):
+            raise RuntimeError(self.model_part_name + " not found.")
+
+        for variable_settings in self.variables_settings_list.values():
+            variable_names_list = variable_settings["variable_names"].GetStringArray()
+
+            container = variable_settings["container"].GetString()
+            if (container == "nodal_historical"):
+                for variable_name in variable_names_list:
+                    variable = Kratos.KratosGlobals.GetVariable(variable_name)
+                    if (not self.__get_model_part().HasNodalSolutionStepVariable(variable)):
+                        raise RuntimeError("Variable " + variable_name + " not found in nodal solution step data of " + self.__get_model_part().Name)
+
+        if self.statistics_computation_processeses is not None:
+            for process in self.statistics_computation_processeses:
+                process.Check()
+
+    def ExecuteInitialize(self):
+        ## set output file path
+        self.output_settings["output_file_settings"]["file_name"].SetString(self.output_settings["output_file_settings"]["file_name"].GetString().replace("<model_part_name>", self.__get_model_part().FullName()))
+        self.output_settings["output_file_settings"]["output_path"].SetString(self.output_settings["output_file_settings"]["output_path"].GetString().replace("<model_part_name>", self.__get_model_part().FullName()))
+
+        self.__write_headers()
+
+        if self.echo_level > 0:
+            Kratos.Logger.PrintInfo(self.__class__.__name__, "List of output operations:\n\t" + "\n\t".join([str(operation) for operation in self.list_of_operations]))
+
+        self.previous_process_info_value = self.__get_model_part().ProcessInfo[self.output_control_variable]
+
+    def ExecuteFinalizeSolutionStep(self):
+        output_control_counter = self.__get_model_part().ProcessInfo[self.output_control_variable]
+
+        if self.interval_utility.IsInInterval(output_control_counter):
+            if (output_control_counter - self.previous_process_info_value) >= self.output_interval:
+
+                # execute the statistics computation process
+                if self.statistics_computation_processeses is not None:
+                    for process in self.statistics_computation_processeses:
+                        for computation_point in self.computation_points:
+                            getattr(process, computation_point)()
+
+                for operation in self.list_of_operations:
+                    operation.Evaluate(self.model_part)
+
+                self.__write_values()
+
+                if self.echo_level > 1:
+                    Kratos.Logger.PrintInfo(self.__class__.__name__, "Calculated statistics on {:s}.".format(self.__get_model_part().FullName()))
+
+                self.previous_process_info_value = output_control_counter
+
+    def ExecuteFinalize(self):
+        if (self.__is_writing_process()):
+            self.output_file.file.write("# End of file.")
+            self.output_file.file.close()
+
+    def __write_headers(self):
+        if (self.__is_writing_process()):
+            kratos_version = "not_given"
+            if (self.output_settings["write_kratos_version"].GetBool()):
+                kratos_version = str(Kratos.KratosGlobals.Kernel.Version())
+
+            time_stamp = "not_specified"
+            if (self.output_settings["write_time_stamp"].GetBool()):
+                time_stamp = str(datetime.now())
+
+            method_name = ""
+            variable_info = ""
+            for operation in self.list_of_operations:
+                if operation.method_name not in method_name:
+                    method_name += operation.method_name + ", "
+                current_variable_info = "{:s}[{:s}, {:s}], ".format(operation.variable_name, operation.norm_type, operation.container_type)
+                if current_variable_info not in variable_info:
+                    variable_info += current_variable_info
+
+            self.headers, self.header_lengths = self.__get_headers()
+
+            msg_header = ""
+            msg_header += "# Spatial statistics process output\n"
+            msg_header += "# Kratos version               : " + kratos_version + "\n"
+            msg_header += "# Timestamp                    : " + time_stamp + "\n"
+            msg_header += "# Method name(s)               : " + method_name[:-2] + "\n"
+            msg_header += "# Variable info(s)             : " + variable_info[:-2] + "\n"
+            msg_header += "# Modelpart name               : " + self.model_part_name + "\n"
+            msg_header += "# Output control variable name : " + self.output_control_variable.Name() + "\n"
+            msg_header += "# ----------------------------------------------------------------------\n"
+            msg_header += "# Headers:\n"
+            msg_header += "#" + " ".join([("{:>" + str(header_length) + "s}").format(header) for header, header_length in zip(self.headers, self.header_lengths)]) + "\n"
+
+            self.output_file = TimeBasedAsciiFileWriterUtility(self.__get_model_part(), self.output_settings["output_file_settings"], msg_header)
+
+            self.is_headers_written = True
+
+    def __get_headers(self):
+        # check whether only one variable with one
+        variable_info = ""
+        for operation in self.list_of_operations:
+            current_variable_info = "{:s}[{:s}, {:s}], ".format(operation.variable_name, operation.norm_type, operation.container_type)
+            if current_variable_info not in variable_info:
+                variable_info += current_variable_info
+
+        headers = ["\"TIME\""]
+        header_lengths = [max(6, self.output_value_length)]
+        if self.output_control_variable != Kratos.TIME:
+            headers.append("\"" + self.output_control_variable.Name() + "\"")
+            header_lengths.append(max(len(self.output_control_variable.Name()) + 2, self.output_value_length))
+
+        # found only one variable type info
+        if variable_info.count(",") == 2:
+            header_formatting_string = "\"<HEADER_NAME><COMPONENT>\""
+        else:
+            header_formatting_string = "\"<VARIABLE_NAME><COMPONENT> [ <NORM_TYPE> | <CONTAINER_TYPE> ] <HEADER_NAME>\""
+
+        variable_components = {
+            "Double": [""],
+            "Array" : ["_X", "_Y", "_Z"]
+        }
+
+        for operation in self.list_of_operations:
+            if operation.norm_type == "none":
+                comps_list = variable_components[Kratos.KratosGlobals.GetVariableType(operation.variable.Name())]
+            else:
+                comps_list = variable_components["Double"]
+
+            for current_header, current_header_length in zip(operation.GetHeaders(), operation.GetValueLengths(self.output_value_length)):
+                for comp in comps_list:
+                    current_header_name = str(header_formatting_string)
+
+                    current_header_name = current_header_name.replace("<HEADER_NAME>", current_header)
+                    current_header_name = current_header_name.replace("<VARIABLE_NAME>", operation.variable.Name())
+                    current_header_name = current_header_name.replace("<COMPONENT>", comp)
+                    current_header_name = current_header_name.replace("<NORM_TYPE>", operation.norm_type)
+                    current_header_name = current_header_name.replace("<CONTAINER_TYPE>", operation.container_type)
+
+                    headers.append(current_header_name)
+                    header_lengths.append(max(len(current_header_name), current_header_length))
+
+        return headers, header_lengths
+
+    def __write_values(self):
+        if (self.__is_writing_process()):
+            values = [GetFormattedValue(self.__get_model_part().ProcessInfo[Kratos.TIME], self.output_value_length, self.output_value_precision)[0]]
+            if self.output_control_variable != Kratos.TIME:
+                values.append(GetFormattedValue(self.__get_model_part().ProcessInfo[self.output_control_variable], self.output_value_length, self.output_value_precision)[0])
+            for operation in self.list_of_operations:
+                values.extend(operation.GetValues(self.output_value_length, self.output_value_precision))
+            self.output_file.file.write(" " + " ".join([("{:>" + str(header_length) + "s}").format(value) for value, header_length in zip(values, self.header_lengths)]) + "\n")
+
+    def __get_model_part(self):
+        if (not hasattr(self, "model_part")):
+            self.model_part = self.model[self.model_part_name]
+
+        return self.model_part
+
+    def __is_writing_process(self):
+        return (self.__get_model_part().GetCommunicator().MyPID() == 0)
```

## KratosMultiphysics/StatisticsApplication/spatial_utilities.py

 * *Ordering differences only*

```diff
@@ -1,226 +1,226 @@
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as Statistics
-
-from KratosMultiphysics.StatisticsApplication.method_utilities import GetNormTypeContainer
-from KratosMultiphysics.StatisticsApplication.method_utilities import GetMethod
-
-def GetFormattedValue(value, length: int, precision: int) -> str:
-    if isinstance(value, int):
-        fixed_format = ("{: " + str(length) + ".0f}").format(value)
-        if len(fixed_format) <= length:
-            return [fixed_format]
-        else:
-            return [("{: " + str(length) + "." + str(precision) + "e}").format(value)]
-    elif isinstance(value, float):
-        fixed_format = ("{: " + str(length) + "." + str(precision) + "f}").format(value)
-        if len(fixed_format) <= length:
-            return [fixed_format]
-        else:
-            return [("{: " + str(length) + "." + str(precision) + "e}").format(value)]
-
-    elif isinstance(value, Kratos.Array3):
-        return [GetFormattedValue(value[0], length, precision)[0], GetFormattedValue(value[1], length, precision)[0], GetFormattedValue(value[2], length, precision)[0]]
-
-def GetItemContainer(item_container_name):
-    item_container_types = [
-        ["nodal_historical", Statistics.SpatialMethods.Historical],
-        ["nodal_non_historical", Statistics.SpatialMethods.NonHistorical.Nodes],
-        ["element_non_historical", Statistics.SpatialMethods.NonHistorical.Elements],
-        ["condition_non_historical", Statistics.SpatialMethods.NonHistorical.Conditions],
-    ]
-
-    item_container_names_list = [item_container_types[i][0] for i in range(len(item_container_types))]
-    item_container_types_list = [item_container_types[i][1] for i in range(len(item_container_types))]
-
-    if (item_container_name not in item_container_names_list):
-        msg = "Unknown container [ \"container\" = \"" + item_container_name + "\" ]\n"
-        msg += "Allowed containers are:\n    "
-        msg += "\n    ".join(sorted(item_container_names_list))
-        raise Exception(msg)
-
-    return item_container_types_list[item_container_names_list.index(item_container_name)]
-
-
-def GetVariableHeaders(norm_type, variable_name):
-    if (norm_type == "none"):
-        variable_type = Kratos.KratosGlobals.GetVariableType(variable_name)
-        if (variable_type == "Double"):
-            return [variable_name]
-        elif (variable_type == "Array" and Kratos.KratosGlobals.GetVariableType(variable_name + "_X") == "Double"):
-            return [variable_name + "_X", variable_name + "_Y", variable_name + "_Z"]
-        else:
-            raise Exception("Unsupported variable type " + variable_type)
-    else:
-        return [variable_name]
-
-class SpatialMethodOutput:
-    def __init__(self, method_name, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
-        self.method_name = method_name
-        self.container_type = container_type
-        self.norm_type = norm_type
-        self.variable_name = variable_name
-        self.method_settings = method_settings
-        self.variable = Kratos.KratosGlobals.GetVariable(self.variable_name)
-
-        self.container = GetItemContainer(self.container_type)
-        self.norm_type_container = GetNormTypeContainer(self.container, norm_type)
-        method = GetMethod(self.norm_type_container, self.method_name)
-
-        if method_settings.IsEquivalentTo(Kratos.Parameters("""{}""")):
-            if norm_type == "none":
-                self.norm_type_container = self.container.ValueMethods
-                self.method = lambda model_part: method(model_part, self.variable)
-            else:
-                self.norm_type_container = self.container.NormMethods
-                self.method = lambda model_part: method(model_part, self.variable, norm_type)
-        else:
-            if norm_type == "none":
-                self.norm_type_container = self.container.ValueMethods
-                self.method = lambda model_part: method(model_part, self.variable, method_settings)
-            else:
-                self.norm_type_container = self.container.NormMethods
-                self.method = lambda model_part: method(model_part, self.variable, norm_type, method_settings)
-
-    def Evaluate(self, model_part):
-        self.data = self.method(model_part)
-
-    def GetValues(self, length, precision):
-        if isinstance(self.data, float):
-            return GetFormattedValue(self.data, length, precision)
-        else:
-            values = []
-            for v in self.data:
-                values.extend(GetFormattedValue(v, length, precision))
-            return values
-
-    def GetValueLengths(self, value_length):
-        return [value_length]
-
-    def __str__(self):
-        return self.__class__.__name__ + "(container: {:s}, norm_type: {:s}, variable: {:s})".format(self.container_type, self.norm_type, self.variable_name)
-
-
-class SpatialSumOutput(SpatialMethodOutput):
-    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
-        super().__init__("sum", container_type, norm_type, variable_name)
-
-    def GetHeaders(self):
-        return ["sum"]
-
-
-class SpatialMeanOutput(SpatialMethodOutput):
-    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
-        super().__init__("mean", container_type, norm_type, variable_name)
-
-    def GetHeaders(self):
-        return ["mean"]
-
-
-class SpatialRootMeanSquareOutput(SpatialMethodOutput):
-    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
-        super().__init__("rootmeansquare", container_type, norm_type, variable_name)
-
-    def GetHeaders(self):
-        return ["rootmeansquare"]
-
-
-class SpatialMinOutput(SpatialMethodOutput):
-    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
-        super().__init__("min", container_type, norm_type, variable_name)
-
-    def GetHeaders(self):
-        return ["min_value", "min_id"]
-
-    def GetValueLengths(self, value_length):
-        return [value_length, value_length]
-
-
-class SpatialMaxOutput(SpatialMethodOutput):
-    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
-        super().__init__("max", container_type, norm_type, variable_name)
-
-    def GetHeaders(self):
-        return ["max_value", "max_id"]
-
-    def GetValueLengths(self, value_length):
-        return [value_length, value_length]
-
-
-class SpatialMedianOutput(SpatialMethodOutput):
-    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
-        super().__init__("median", container_type, norm_type, variable_name)
-
-    def GetHeaders(self):
-        return ["median"]
-
-
-class SpatialVarianceOutput(SpatialMethodOutput):
-    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
-        super().__init__("variance", container_type, norm_type, variable_name)
-
-    def GetHeaders(self):
-        return ["mean", "variance"]
-
-    def GetValueLengths(self, value_length):
-        return [value_length, value_length]
-
-
-class SpatialDistributionOutput(SpatialMethodOutput):
-    def __init__(self, container_type, norm_type, variable_name, method_settings):
-        super().__init__("distribution", container_type, norm_type, variable_name, method_settings)
-        default_parameters = Kratos.Parameters("""{ "number_of_value_groups": 10 }""")
-        self.method_settings.AddMissingParameters(default_parameters)
-
-        self.write_min_value = True
-        if self.method_settings.Has("min_value") and self.method_settings["min_value"].IsDouble():
-            self.write_min_value = False
-
-        self.write_max_value = True
-        if self.method_settings.Has("max_value") and self.method_settings["max_value"].IsDouble():
-            self.write_max_value = False
-
-    def Evaluate(self, *args):
-        super().Evaluate(*args)
-        (self.min_value, self.max_value, self.group_upper_values, self.group_histogram, self.group_percentage_distribution, self.group_means, self.group_variances) = self.data
-
-    def GetHeaders(self):
-        number_of_groups = self.method_settings["number_of_value_groups"].GetInt()
-        headers = []
-        if self.write_min_value:
-            headers.append("min")
-        if self.write_max_value:
-            headers.append("max")
-
-        headers.append("group_below_min {mean|variance}")
-        headers.extend(["group_{:d}".format(i+1) + " {mean|variance}" for i in range(number_of_groups)])
-        headers.append("group_above_max {mean|variance}")
-        return headers
-
-    def GetValues(self, length, precision):
-        values = []
-        if self.write_min_value:
-            values.append(GetFormattedValue(self.min_value, length, precision)[0])
-        if self.write_max_value:
-            values.append(GetFormattedValue(self.max_value, length, precision)[0])
-
-        def get_formatted_group_value(hist_v, percentage_v, upper_v, mean_v, variance_v):
-            s = "{:s} [#] = {:s} [%] < {:s}".format(GetFormattedValue(hist_v, length, precision)[0], GetFormattedValue(percentage_v * 100.0, length, precision)[0], GetFormattedValue(upper_v, length, precision)[0])
-            s += " { " + GetFormattedValue(mean_v, length, precision)[0] + " | " + GetFormattedValue(variance_v, length, precision)[0] + " }"
-            return s
-        values.extend([get_formatted_group_value(hist_v, percentage_v, upper_v, mean_v, variance_v) for hist_v, percentage_v, upper_v, mean_v, variance_v in zip(self.group_histogram, self.group_percentage_distribution, self.group_upper_values, self.group_means, self.group_variances)])
-        values[-1] = values[-1].replace(" <", ">=")
-        return values
-
-    def GetValueLengths(self, value_length):
-        values_per_header = []
-        if self.write_min_value:
-            values_per_header.append(value_length)
-        if self.write_max_value:
-            values_per_header.append(value_length)
-
-        number_of_groups = self.method_settings["number_of_value_groups"].GetInt()
-        for _ in range(number_of_groups + 2):
-            values_per_header.append(22 + value_length * 5)
-        return values_per_header
-
-
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as Statistics
+
+from KratosMultiphysics.StatisticsApplication.method_utilities import GetNormTypeContainer
+from KratosMultiphysics.StatisticsApplication.method_utilities import GetMethod
+
+def GetFormattedValue(value, length: int, precision: int) -> str:
+    if isinstance(value, int):
+        fixed_format = ("{: " + str(length) + ".0f}").format(value)
+        if len(fixed_format) <= length:
+            return [fixed_format]
+        else:
+            return [("{: " + str(length) + "." + str(precision) + "e}").format(value)]
+    elif isinstance(value, float):
+        fixed_format = ("{: " + str(length) + "." + str(precision) + "f}").format(value)
+        if len(fixed_format) <= length:
+            return [fixed_format]
+        else:
+            return [("{: " + str(length) + "." + str(precision) + "e}").format(value)]
+
+    elif isinstance(value, Kratos.Array3):
+        return [GetFormattedValue(value[0], length, precision)[0], GetFormattedValue(value[1], length, precision)[0], GetFormattedValue(value[2], length, precision)[0]]
+
+def GetItemContainer(item_container_name):
+    item_container_types = [
+        ["nodal_historical", Statistics.SpatialMethods.Historical],
+        ["nodal_non_historical", Statistics.SpatialMethods.NonHistorical.Nodes],
+        ["element_non_historical", Statistics.SpatialMethods.NonHistorical.Elements],
+        ["condition_non_historical", Statistics.SpatialMethods.NonHistorical.Conditions],
+    ]
+
+    item_container_names_list = [item_container_types[i][0] for i in range(len(item_container_types))]
+    item_container_types_list = [item_container_types[i][1] for i in range(len(item_container_types))]
+
+    if (item_container_name not in item_container_names_list):
+        msg = "Unknown container [ \"container\" = \"" + item_container_name + "\" ]\n"
+        msg += "Allowed containers are:\n    "
+        msg += "\n    ".join(sorted(item_container_names_list))
+        raise Exception(msg)
+
+    return item_container_types_list[item_container_names_list.index(item_container_name)]
+
+
+def GetVariableHeaders(norm_type, variable_name):
+    if (norm_type == "none"):
+        variable_type = Kratos.KratosGlobals.GetVariableType(variable_name)
+        if (variable_type == "Double"):
+            return [variable_name]
+        elif (variable_type == "Array" and Kratos.KratosGlobals.GetVariableType(variable_name + "_X") == "Double"):
+            return [variable_name + "_X", variable_name + "_Y", variable_name + "_Z"]
+        else:
+            raise Exception("Unsupported variable type " + variable_type)
+    else:
+        return [variable_name]
+
+class SpatialMethodOutput:
+    def __init__(self, method_name, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
+        self.method_name = method_name
+        self.container_type = container_type
+        self.norm_type = norm_type
+        self.variable_name = variable_name
+        self.method_settings = method_settings
+        self.variable = Kratos.KratosGlobals.GetVariable(self.variable_name)
+
+        self.container = GetItemContainer(self.container_type)
+        self.norm_type_container = GetNormTypeContainer(self.container, norm_type)
+        method = GetMethod(self.norm_type_container, self.method_name)
+
+        if method_settings.IsEquivalentTo(Kratos.Parameters("""{}""")):
+            if norm_type == "none":
+                self.norm_type_container = self.container.ValueMethods
+                self.method = lambda model_part: method(model_part, self.variable)
+            else:
+                self.norm_type_container = self.container.NormMethods
+                self.method = lambda model_part: method(model_part, self.variable, norm_type)
+        else:
+            if norm_type == "none":
+                self.norm_type_container = self.container.ValueMethods
+                self.method = lambda model_part: method(model_part, self.variable, method_settings)
+            else:
+                self.norm_type_container = self.container.NormMethods
+                self.method = lambda model_part: method(model_part, self.variable, norm_type, method_settings)
+
+    def Evaluate(self, model_part):
+        self.data = self.method(model_part)
+
+    def GetValues(self, length, precision):
+        if isinstance(self.data, float):
+            return GetFormattedValue(self.data, length, precision)
+        else:
+            values = []
+            for v in self.data:
+                values.extend(GetFormattedValue(v, length, precision))
+            return values
+
+    def GetValueLengths(self, value_length):
+        return [value_length]
+
+    def __str__(self):
+        return self.__class__.__name__ + "(container: {:s}, norm_type: {:s}, variable: {:s})".format(self.container_type, self.norm_type, self.variable_name)
+
+
+class SpatialSumOutput(SpatialMethodOutput):
+    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
+        super().__init__("sum", container_type, norm_type, variable_name)
+
+    def GetHeaders(self):
+        return ["sum"]
+
+
+class SpatialMeanOutput(SpatialMethodOutput):
+    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
+        super().__init__("mean", container_type, norm_type, variable_name)
+
+    def GetHeaders(self):
+        return ["mean"]
+
+
+class SpatialRootMeanSquareOutput(SpatialMethodOutput):
+    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
+        super().__init__("rootmeansquare", container_type, norm_type, variable_name)
+
+    def GetHeaders(self):
+        return ["rootmeansquare"]
+
+
+class SpatialMinOutput(SpatialMethodOutput):
+    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
+        super().__init__("min", container_type, norm_type, variable_name)
+
+    def GetHeaders(self):
+        return ["min_value", "min_id"]
+
+    def GetValueLengths(self, value_length):
+        return [value_length, value_length]
+
+
+class SpatialMaxOutput(SpatialMethodOutput):
+    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
+        super().__init__("max", container_type, norm_type, variable_name)
+
+    def GetHeaders(self):
+        return ["max_value", "max_id"]
+
+    def GetValueLengths(self, value_length):
+        return [value_length, value_length]
+
+
+class SpatialMedianOutput(SpatialMethodOutput):
+    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
+        super().__init__("median", container_type, norm_type, variable_name)
+
+    def GetHeaders(self):
+        return ["median"]
+
+
+class SpatialVarianceOutput(SpatialMethodOutput):
+    def __init__(self, container_type, norm_type, variable_name, method_settings = Kratos.Parameters("""{}""")):
+        super().__init__("variance", container_type, norm_type, variable_name)
+
+    def GetHeaders(self):
+        return ["mean", "variance"]
+
+    def GetValueLengths(self, value_length):
+        return [value_length, value_length]
+
+
+class SpatialDistributionOutput(SpatialMethodOutput):
+    def __init__(self, container_type, norm_type, variable_name, method_settings):
+        super().__init__("distribution", container_type, norm_type, variable_name, method_settings)
+        default_parameters = Kratos.Parameters("""{ "number_of_value_groups": 10 }""")
+        self.method_settings.AddMissingParameters(default_parameters)
+
+        self.write_min_value = True
+        if self.method_settings.Has("min_value") and self.method_settings["min_value"].IsDouble():
+            self.write_min_value = False
+
+        self.write_max_value = True
+        if self.method_settings.Has("max_value") and self.method_settings["max_value"].IsDouble():
+            self.write_max_value = False
+
+    def Evaluate(self, *args):
+        super().Evaluate(*args)
+        (self.min_value, self.max_value, self.group_upper_values, self.group_histogram, self.group_percentage_distribution, self.group_means, self.group_variances) = self.data
+
+    def GetHeaders(self):
+        number_of_groups = self.method_settings["number_of_value_groups"].GetInt()
+        headers = []
+        if self.write_min_value:
+            headers.append("min")
+        if self.write_max_value:
+            headers.append("max")
+
+        headers.append("group_below_min {mean|variance}")
+        headers.extend(["group_{:d}".format(i+1) + " {mean|variance}" for i in range(number_of_groups)])
+        headers.append("group_above_max {mean|variance}")
+        return headers
+
+    def GetValues(self, length, precision):
+        values = []
+        if self.write_min_value:
+            values.append(GetFormattedValue(self.min_value, length, precision)[0])
+        if self.write_max_value:
+            values.append(GetFormattedValue(self.max_value, length, precision)[0])
+
+        def get_formatted_group_value(hist_v, percentage_v, upper_v, mean_v, variance_v):
+            s = "{:s} [#] = {:s} [%] < {:s}".format(GetFormattedValue(hist_v, length, precision)[0], GetFormattedValue(percentage_v * 100.0, length, precision)[0], GetFormattedValue(upper_v, length, precision)[0])
+            s += " { " + GetFormattedValue(mean_v, length, precision)[0] + " | " + GetFormattedValue(variance_v, length, precision)[0] + " }"
+            return s
+        values.extend([get_formatted_group_value(hist_v, percentage_v, upper_v, mean_v, variance_v) for hist_v, percentage_v, upper_v, mean_v, variance_v in zip(self.group_histogram, self.group_percentage_distribution, self.group_upper_values, self.group_means, self.group_variances)])
+        values[-1] = values[-1].replace(" <", ">=")
+        return values
+
+    def GetValueLengths(self, value_length):
+        values_per_header = []
+        if self.write_min_value:
+            values_per_header.append(value_length)
+        if self.write_max_value:
+            values_per_header.append(value_length)
+
+        number_of_groups = self.method_settings["number_of_value_groups"].GetInt()
+        for _ in range(number_of_groups + 2):
+            values_per_header.append(22 + value_length * 5)
+        return values_per_header
+
+
```

## KratosMultiphysics/StatisticsApplication/temporal_statistics_process.py

 * *Ordering differences only*

```diff
@@ -1,121 +1,121 @@
-import KratosMultiphysics as Kratos
-
-from KratosMultiphysics.StatisticsApplication.method_utilities import GetNormTypeContainer
-from KratosMultiphysics.StatisticsApplication.method_utilities import GetMethod
-from KratosMultiphysics.StatisticsApplication.temporal_utilities import GetItemContainer
-
-def Factory(settings, model):
-    if (not isinstance(model, Kratos.Model)):
-        raise Exception(
-            "expected input shall be a Model object, encapsulating a json string"
-        )
-    if (not isinstance(settings, Kratos.Parameters)):
-        raise Exception(
-            "expected input shall be a Parameters object, encapsulating a json string"
-        )
-    return TemporalStatisticsProcess(model, settings["Parameters"])
-
-class TemporalStatisticsProcess(Kratos.Process):
-    """A process to use temporal statistics for Kratos containers
-
-    This process calculates temporal statistics for given input variables in given container, and outputs to chosen variables
-    and chosen container.
-
-    This is compatible in OpenMP and MPI with restart
-
-    Note: When this process is used with restarting, please don't use restarting start timestep and "statistics_start_point_control_value" time step
-          same. This will have an error in averaging, once simulation is restarted.
-
-    Args:
-        model (Kratos.Model): Model used in problem
-        settings (Kratos.Parameters): Kratos parameter settings for process
-    """
-    def __init__(self, model, settings):
-        Kratos.Process.__init__(self)
-
-        default_parameters = Kratos.Parameters("""
-        {
-            "model_part_name" : "PLEASE_SPECIFY_MODEL_PART_NAME",
-            "input_variable_settings" : [
-                {
-                    "method_name"     : "sum",
-                    "norm_type"       : "none",
-                    "container"       : "nodal_historical_non_historical",
-                    "echo_level"      : 0,
-                    "method_settings" : {}
-                }
-            ],
-            "echo_level" : 0,
-            "statistics_start_point_control_variable_name" : "TIME",
-            "statistics_start_point_control_value"         : 0.0
-        }  """)
-
-        self.model = model
-        self.settings = settings
-        self.settings.ValidateAndAssignDefaults(default_parameters)
-        self.echo_level = self.settings["echo_level"].GetInt()
-        self.variables_settings_list = self.settings["input_variable_settings"]
-
-        for variable_settings in self.variables_settings_list.values():
-            variable_settings.ValidateAndAssignDefaults(default_parameters["input_variable_settings"][0])
-            container_name = variable_settings["container"].GetString()
-            norm_type = variable_settings["norm_type"].GetString()
-
-            item_container = GetItemContainer(container_name)
-            _ = GetNormTypeContainer(item_container, norm_type)
-
-        self.model_part_name = self.settings["model_part_name"].GetString()
-
-        statistics_control_variable_name = self.settings["statistics_start_point_control_variable_name"].GetString()
-        if (not Kratos.KratosGlobals.HasVariable(statistics_control_variable_name)):
-            raise Exception("Unknown statistics control variable. [ \"statistics_control_variable_name\" = \"" + statistics_control_variable_name + "\" ]")
-
-        ## this is required to support restarting capabilities. If STEP is used, there need to be a way to retrieve
-        ## initial starting time for integration in the case of restarting.
-        if (statistics_control_variable_name != "TIME"):
-            raise Exception("Only \"TIME\" is supported as statistics_start_point_control_variable_name.")
-
-        self.statistics_control_variable = Kratos.KratosGlobals.GetVariable(statistics_control_variable_name)
-        statistics_control_variable_type = Kratos.KratosGlobals.GetVariableType(statistics_control_variable_name)
-        if (statistics_control_variable_type == "Integer"):
-            self.statistics_control_value = self.settings["statistics_start_point_control_value"].GetInt()
-        elif (statistics_control_variable_type == "Double"):
-            self.statistics_control_value = self.settings["statistics_start_point_control_value"].GetDouble()
-        else:
-            raise Exception("Unsupported statistics control variable type. Only supports Integer, and Double.")
-
-        if (self.echo_level > 0):
-            Kratos.Logger.PrintInfo("TemporalStatisticsProcess", "Initialized statistics process.")
-
-    def Check(self):
-        if (not self.model.HasModelPart(self.model_part_name)):
-            raise Exception(self.model_part_name + " not found.")
-
-    def ExecuteInitialize(self):
-        self.method_list = []
-        for variable_settings in self.variables_settings_list.values():
-            container_name = variable_settings["container"].GetString()
-            norm_type = variable_settings["norm_type"].GetString()
-            method_name = variable_settings["method_name"].GetString()
-            echo_level = variable_settings["echo_level"].GetInt()
-
-            item_container = GetItemContainer(container_name)
-            method = GetMethod(item_container, method_name)
-            method_objects = method(self.__get_model_part(), norm_type, echo_level, variable_settings["method_settings"])
-
-            self.method_list.extend(method_objects)
-
-        for method in self.method_list:
-            method.InitializeStatisticsMethod(self.statistics_control_value)
-
-    def ExecuteFinalizeSolutionStep(self):
-        current_value = self.model_part.ProcessInfo[self.statistics_control_variable]
-        if (current_value >= self.statistics_control_value):
-            for method in self.method_list:
-                method.CalculateStatistics()
-
-    def __get_model_part(self):
-        if (not hasattr(self, "model_part")):
-            self.model_part = self.model[self.model_part_name]
-
+import KratosMultiphysics as Kratos
+
+from KratosMultiphysics.StatisticsApplication.method_utilities import GetNormTypeContainer
+from KratosMultiphysics.StatisticsApplication.method_utilities import GetMethod
+from KratosMultiphysics.StatisticsApplication.temporal_utilities import GetItemContainer
+
+def Factory(settings, model):
+    if (not isinstance(model, Kratos.Model)):
+        raise Exception(
+            "expected input shall be a Model object, encapsulating a json string"
+        )
+    if (not isinstance(settings, Kratos.Parameters)):
+        raise Exception(
+            "expected input shall be a Parameters object, encapsulating a json string"
+        )
+    return TemporalStatisticsProcess(model, settings["Parameters"])
+
+class TemporalStatisticsProcess(Kratos.Process):
+    """A process to use temporal statistics for Kratos containers
+
+    This process calculates temporal statistics for given input variables in given container, and outputs to chosen variables
+    and chosen container.
+
+    This is compatible in OpenMP and MPI with restart
+
+    Note: When this process is used with restarting, please don't use restarting start timestep and "statistics_start_point_control_value" time step
+          same. This will have an error in averaging, once simulation is restarted.
+
+    Args:
+        model (Kratos.Model): Model used in problem
+        settings (Kratos.Parameters): Kratos parameter settings for process
+    """
+    def __init__(self, model, settings):
+        Kratos.Process.__init__(self)
+
+        default_parameters = Kratos.Parameters("""
+        {
+            "model_part_name" : "PLEASE_SPECIFY_MODEL_PART_NAME",
+            "input_variable_settings" : [
+                {
+                    "method_name"     : "sum",
+                    "norm_type"       : "none",
+                    "container"       : "nodal_historical_non_historical",
+                    "echo_level"      : 0,
+                    "method_settings" : {}
+                }
+            ],
+            "echo_level" : 0,
+            "statistics_start_point_control_variable_name" : "TIME",
+            "statistics_start_point_control_value"         : 0.0
+        }  """)
+
+        self.model = model
+        self.settings = settings
+        self.settings.ValidateAndAssignDefaults(default_parameters)
+        self.echo_level = self.settings["echo_level"].GetInt()
+        self.variables_settings_list = self.settings["input_variable_settings"]
+
+        for variable_settings in self.variables_settings_list.values():
+            variable_settings.ValidateAndAssignDefaults(default_parameters["input_variable_settings"][0])
+            container_name = variable_settings["container"].GetString()
+            norm_type = variable_settings["norm_type"].GetString()
+
+            item_container = GetItemContainer(container_name)
+            _ = GetNormTypeContainer(item_container, norm_type)
+
+        self.model_part_name = self.settings["model_part_name"].GetString()
+
+        statistics_control_variable_name = self.settings["statistics_start_point_control_variable_name"].GetString()
+        if (not Kratos.KratosGlobals.HasVariable(statistics_control_variable_name)):
+            raise Exception("Unknown statistics control variable. [ \"statistics_control_variable_name\" = \"" + statistics_control_variable_name + "\" ]")
+
+        ## this is required to support restarting capabilities. If STEP is used, there need to be a way to retrieve
+        ## initial starting time for integration in the case of restarting.
+        if (statistics_control_variable_name != "TIME"):
+            raise Exception("Only \"TIME\" is supported as statistics_start_point_control_variable_name.")
+
+        self.statistics_control_variable = Kratos.KratosGlobals.GetVariable(statistics_control_variable_name)
+        statistics_control_variable_type = Kratos.KratosGlobals.GetVariableType(statistics_control_variable_name)
+        if (statistics_control_variable_type == "Integer"):
+            self.statistics_control_value = self.settings["statistics_start_point_control_value"].GetInt()
+        elif (statistics_control_variable_type == "Double"):
+            self.statistics_control_value = self.settings["statistics_start_point_control_value"].GetDouble()
+        else:
+            raise Exception("Unsupported statistics control variable type. Only supports Integer, and Double.")
+
+        if (self.echo_level > 0):
+            Kratos.Logger.PrintInfo("TemporalStatisticsProcess", "Initialized statistics process.")
+
+    def Check(self):
+        if (not self.model.HasModelPart(self.model_part_name)):
+            raise Exception(self.model_part_name + " not found.")
+
+    def ExecuteInitialize(self):
+        self.method_list = []
+        for variable_settings in self.variables_settings_list.values():
+            container_name = variable_settings["container"].GetString()
+            norm_type = variable_settings["norm_type"].GetString()
+            method_name = variable_settings["method_name"].GetString()
+            echo_level = variable_settings["echo_level"].GetInt()
+
+            item_container = GetItemContainer(container_name)
+            method = GetMethod(item_container, method_name)
+            method_objects = method(self.__get_model_part(), norm_type, echo_level, variable_settings["method_settings"])
+
+            self.method_list.extend(method_objects)
+
+        for method in self.method_list:
+            method.InitializeStatisticsMethod(self.statistics_control_value)
+
+    def ExecuteFinalizeSolutionStep(self):
+        current_value = self.model_part.ProcessInfo[self.statistics_control_variable]
+        if (current_value >= self.statistics_control_value):
+            for method in self.method_list:
+                method.CalculateStatistics()
+
+    def __get_model_part(self):
+        if (not hasattr(self, "model_part")):
+            self.model_part = self.model[self.model_part_name]
+
         return self.model_part
```

## KratosMultiphysics/StatisticsApplication/temporal_utilities.py

 * *Ordering differences only*

```diff
@@ -1,62 +1,62 @@
-import KratosMultiphysics.StatisticsApplication as Statistics
-
-def GetItemContainer(item_container_name):
-    item_container_types = [
-        [
-            "nodal_historical_historical",
-            Statistics.TemporalMethods.Historical.HistoricalOutput
-        ],
-        [
-            "nodal_historical_non_historical",
-            Statistics.TemporalMethods.Historical.NonHistoricalOutput
-        ],
-        [
-            "nodal_non_historical",
-            Statistics.TemporalMethods.NonHistorical.Nodes
-        ],
-        [
-            "element_non_historical",
-            Statistics.TemporalMethods.NonHistorical.Elements
-        ],
-        [
-            "condition_non_historical",
-            Statistics.TemporalMethods.NonHistorical.Conditions
-        ],
-    ]
-
-    item_container_names_list = [
-        item_container_types[i][0] for i in range(len(item_container_types))
-    ]
-    item_container_types_list = [
-        item_container_types[i][1] for i in range(len(item_container_types))
-    ]
-
-    if (item_container_name not in item_container_names_list):
-        msg = "Unknown container [ \"container\" = \"" + item_container_name + "\" ]\n"
-        msg += "Allowed containers are:\n    "
-        msg += "\n    ".join(sorted(item_container_names_list))
-        raise Exception(msg)
-
-    return item_container_types_list[item_container_names_list.index(
-        item_container_name)]
-
-
-def GetMethodClass(item_norm_method_container, variable_type):
-    method_class_info_list = []
-    for method in dir(item_norm_method_container):
-        if (not method.startswith("__")):
-            method_class_info_list.append([method.lower(), method])
-
-    variable_types_list = [method_class_info_list[i][0] for i in range(len(method_class_info_list))]
-    method_type_class_list = [method_class_info_list[i][1] for i in range(len(method_class_info_list))]
-
-    if (variable_type not in variable_types_list):
-        msg = "Unknown variable type. [ variable_type = " + variable_type + " ]\n"
-        msg += "Allowed variable types are:\n    "
-        msg += "\n    ".join(sorted(variable_types_list))
-        raise Exception(msg)
-
-    return getattr(item_norm_method_container, method_type_class_list[variable_types_list.index(variable_type)])
-
-
-
+import KratosMultiphysics.StatisticsApplication as Statistics
+
+def GetItemContainer(item_container_name):
+    item_container_types = [
+        [
+            "nodal_historical_historical",
+            Statistics.TemporalMethods.Historical.HistoricalOutput
+        ],
+        [
+            "nodal_historical_non_historical",
+            Statistics.TemporalMethods.Historical.NonHistoricalOutput
+        ],
+        [
+            "nodal_non_historical",
+            Statistics.TemporalMethods.NonHistorical.Nodes
+        ],
+        [
+            "element_non_historical",
+            Statistics.TemporalMethods.NonHistorical.Elements
+        ],
+        [
+            "condition_non_historical",
+            Statistics.TemporalMethods.NonHistorical.Conditions
+        ],
+    ]
+
+    item_container_names_list = [
+        item_container_types[i][0] for i in range(len(item_container_types))
+    ]
+    item_container_types_list = [
+        item_container_types[i][1] for i in range(len(item_container_types))
+    ]
+
+    if (item_container_name not in item_container_names_list):
+        msg = "Unknown container [ \"container\" = \"" + item_container_name + "\" ]\n"
+        msg += "Allowed containers are:\n    "
+        msg += "\n    ".join(sorted(item_container_names_list))
+        raise Exception(msg)
+
+    return item_container_types_list[item_container_names_list.index(
+        item_container_name)]
+
+
+def GetMethodClass(item_norm_method_container, variable_type):
+    method_class_info_list = []
+    for method in dir(item_norm_method_container):
+        if (not method.startswith("__")):
+            method_class_info_list.append([method.lower(), method])
+
+    variable_types_list = [method_class_info_list[i][0] for i in range(len(method_class_info_list))]
+    method_type_class_list = [method_class_info_list[i][1] for i in range(len(method_class_info_list))]
+
+    if (variable_type not in variable_types_list):
+        msg = "Unknown variable type. [ variable_type = " + variable_type + " ]\n"
+        msg += "Allowed variable types are:\n    "
+        msg += "\n    ".join(sorted(variable_types_list))
+        raise Exception(msg)
+
+    return getattr(item_norm_method_container, method_type_class_list[variable_types_list.index(variable_type)])
+
+
+
```

## KratosMultiphysics/StatisticsApplication/test_utilities.py

 * *Ordering differences only*

```diff
@@ -1,164 +1,164 @@
-import KratosMultiphysics as Kratos
-from random import uniform
-
-
-def GetRandomValue(min_value=-10.0, max_value=10.0):
-    return uniform(min_value, max_value)
-
-
-def GetRandomVector(vector_size=3, min_value=-10.0, max_value=10.0):
-    v = Kratos.Vector(vector_size)
-
-    for i in range(vector_size):
-        v[i] = GetRandomValue(min_value, max_value)
-
-    return v
-
-
-def GetRandomMatrix(size_1=5, size_2=5, min_value=-10.0, max_value=10.0):
-    m = Kratos.Matrix(size_1, size_2)
-
-    for i in range(size_1):
-        for j in range(size_1):
-            m[i, j] = GetRandomValue(min_value, max_value)
-
-    return m
-
-def HistoricalRetrievalMethod(item, variable):
-    return item.GetSolutionStepValue(variable)
-
-def NonHistoricalRetrievalMethod(item, variable):
-    return item.GetValue(variable)
-
-def InitializeContainerArrays(container):
-    scalar_list = []
-    vector_3d_list = []
-    vector_list = []
-    matrix_list = []
-    for _ in container:
-        scalar_list.append([])
-        vector_3d_list.append([])
-        vector_list.append([])
-        matrix_list.append([])
-
-    return scalar_list, vector_3d_list, vector_list, matrix_list
-
-def CheckValues(test_unit, value_a, value_b, tolerance):
-    if (isinstance(value_a, tuple)):
-        for i, v_a in enumerate(value_a):
-            CheckValues(test_unit, v_a, value_b[i], tolerance)
-    else:
-        if (isinstance(value_a, Kratos.Matrix)):
-            test_unit.assertMatrixAlmostEqual(value_a, value_b, tolerance)
-        elif (isinstance(value_a, Kratos.Vector)):
-            test_unit.assertVectorAlmostEqual(value_a, value_b, tolerance)
-        elif (isinstance(value_a, list)):
-            for i, v_a in enumerate(value_a):
-                test_unit.assertAlmostEqual(v_a, value_b[i], tolerance)
-        else:
-            test_unit.assertAlmostEqual(value_a, value_b, tolerance)
-
-def CreateModelPart(model_part):
-    model_part.CreateNewNode(1, 0.0, 0.0, 0.0)
-    model_part.CreateNewNode(2, 1.0, 0.0, 0.0)
-    model_part.CreateNewNode(3, 2.0, 0.0, 0.0)
-    model_part.CreateNewNode(4, 2.0, 1.0, 0.0)
-    model_part.CreateNewNode(5, 1.5, 1.0, 0.0)
-    model_part.CreateNewNode(6, 0.5, 1.0, 0.0)
-    model_part.CreateNewNode(7, 0.0, 1.0, 0.0)
-
-    prop = model_part.GetProperties()[0]
-
-    model_part.CreateNewElement("Element2D3N", 1, [1, 6, 7], prop)
-    model_part.CreateNewElement("Element2D3N", 2, [1, 2, 6], prop)
-    model_part.CreateNewElement("Element2D3N", 3, [6, 2, 5], prop)
-    model_part.CreateNewElement("Element2D3N", 4, [2, 3, 5], prop)
-    model_part.CreateNewElement("Element2D3N", 5, [5, 3, 4], prop)
-
-    model_part.CreateNewCondition("LineCondition2D2N", 1, [1, 2], prop)
-    model_part.CreateNewCondition("LineCondition2D2N", 2, [2, 3], prop)
-    model_part.CreateNewCondition("LineCondition2D2N", 3, [3, 4], prop)
-    model_part.CreateNewCondition("LineCondition2D2N", 4, [4, 5], prop)
-    model_part.CreateNewCondition("LineCondition2D2N", 5, [5, 6], prop)
-    model_part.CreateNewCondition("LineCondition2D2N", 6, [6, 7], prop)
-    model_part.CreateNewCondition("LineCondition2D2N", 7, [7, 1], prop)
-
-def InitializeModelPartVariables(model_part, is_random = True):
-    if is_random:
-        scalar_method = lambda item : GetRandomValue()
-        array_3d_method = lambda item : GetRandomVector()
-        vector_method = lambda item : GetRandomVector(5)
-        matrix_method = lambda item : GetRandomMatrix()
-    else:
-        t = model_part.ProcessInfo[Kratos.STEP]
-        scalar_method = lambda item : GetInitialVariableValue(Kratos.PRESSURE, "none", (t+1) * (item.Id+1))
-        array_3d_method = lambda item : GetInitialVariableValue(Kratos.VELOCITY, "none", (t+1) * (item.Id +1) * 2.0)
-        vector_method = lambda item : GetInitialVariableValue(Kratos.LOAD_MESHES, "none", (t+1) * (item.Id + 2.0))
-        matrix_method = lambda item : GetInitialVariableValue(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, "none", (t+1) * (item.Id+3)* 2.0)
-
-    communicator = model_part.GetCommunicator()
-    container = communicator.LocalMesh()
-
-    for node in container.Nodes:
-        node.SetValue(Kratos.PRESSURE, scalar_method(node))
-        node.SetValue(Kratos.VELOCITY, array_3d_method(node))
-        node.SetValue(Kratos.LOAD_MESHES, vector_method(node))
-        node.SetValue(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, matrix_method(node))
-
-        node.SetSolutionStepValue(Kratos.PRESSURE, 0, scalar_method(node))
-        node.SetSolutionStepValue(Kratos.VELOCITY, 0, array_3d_method(node))
-        node.SetSolutionStepValue(Kratos.LOAD_MESHES, 0, vector_method(node))
-        node.SetSolutionStepValue(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, 0, matrix_method(node))
-
-    communicator.GetDataCommunicator().Barrier()
-    model_part.GetCommunicator().SynchronizeVariable(Kratos.PRESSURE)
-    model_part.GetCommunicator().SynchronizeVariable(Kratos.VELOCITY)
-    model_part.GetCommunicator().SynchronizeVariable(Kratos.LOAD_MESHES)
-    model_part.GetCommunicator().SynchronizeVariable(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR)
-    model_part.GetCommunicator().SynchronizeNonHistoricalVariable(Kratos.PRESSURE)
-    model_part.GetCommunicator().SynchronizeNonHistoricalVariable(Kratos.VELOCITY)
-    model_part.GetCommunicator().SynchronizeNonHistoricalVariable(Kratos.LOAD_MESHES)
-    model_part.GetCommunicator().SynchronizeNonHistoricalVariable(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR)
-
-    for condition in container.Conditions:
-        condition.SetValue(Kratos.PRESSURE, scalar_method(condition))
-        condition.SetValue(Kratos.VELOCITY, array_3d_method(condition))
-        condition.SetValue(Kratos.LOAD_MESHES, vector_method(condition))
-        condition.SetValue(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, matrix_method(condition))
-
-    for element in container.Elements:
-        element.SetValue(Kratos.PRESSURE, scalar_method(element))
-        element.SetValue(Kratos.VELOCITY, array_3d_method(element))
-        element.SetValue(Kratos.LOAD_MESHES, vector_method(element))
-        element.SetValue(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, matrix_method(element))
-
-    communicator.GetDataCommunicator().Barrier()
-
-def GetInitialVariableValue(variable, norm_type, value = 0.0):
-    if (norm_type == "none"):
-        if (variable == Kratos.PRESSURE):
-            return value
-        elif (variable == Kratos.VELOCITY):
-            return Kratos.Vector(3, value)
-        elif (variable == Kratos.LOAD_MESHES):
-            return Kratos.Vector(5, value)
-        elif (variable == Kratos.GREEN_LAGRANGE_STRAIN_TENSOR):
-            return Kratos.Matrix(5, 5, value)
-    else:
-        return 0.0
-
-def InitializeProcesses(test):
-    communicator = test.model_part.GetCommunicator().GetDataCommunicator()
-    for process in test.process_list:
-        communicator.Barrier()
-        process.Check()
-
-    for process in test.process_list:
-        communicator.Barrier()
-        process.ExecuteInitialize()
-
-def ExecuteProcessFinalizeSolutionStep(test):
-    communicator = test.model_part.GetCommunicator().GetDataCommunicator()
-    for process in test.process_list:
-        communicator.Barrier()
-        process.ExecuteFinalizeSolutionStep()
+import KratosMultiphysics as Kratos
+from random import uniform
+
+
+def GetRandomValue(min_value=-10.0, max_value=10.0):
+    return uniform(min_value, max_value)
+
+
+def GetRandomVector(vector_size=3, min_value=-10.0, max_value=10.0):
+    v = Kratos.Vector(vector_size)
+
+    for i in range(vector_size):
+        v[i] = GetRandomValue(min_value, max_value)
+
+    return v
+
+
+def GetRandomMatrix(size_1=5, size_2=5, min_value=-10.0, max_value=10.0):
+    m = Kratos.Matrix(size_1, size_2)
+
+    for i in range(size_1):
+        for j in range(size_1):
+            m[i, j] = GetRandomValue(min_value, max_value)
+
+    return m
+
+def HistoricalRetrievalMethod(item, variable):
+    return item.GetSolutionStepValue(variable)
+
+def NonHistoricalRetrievalMethod(item, variable):
+    return item.GetValue(variable)
+
+def InitializeContainerArrays(container):
+    scalar_list = []
+    vector_3d_list = []
+    vector_list = []
+    matrix_list = []
+    for _ in container:
+        scalar_list.append([])
+        vector_3d_list.append([])
+        vector_list.append([])
+        matrix_list.append([])
+
+    return scalar_list, vector_3d_list, vector_list, matrix_list
+
+def CheckValues(test_unit, value_a, value_b, tolerance):
+    if (isinstance(value_a, tuple)):
+        for i, v_a in enumerate(value_a):
+            CheckValues(test_unit, v_a, value_b[i], tolerance)
+    else:
+        if (isinstance(value_a, Kratos.Matrix)):
+            test_unit.assertMatrixAlmostEqual(value_a, value_b, tolerance)
+        elif (isinstance(value_a, Kratos.Vector)):
+            test_unit.assertVectorAlmostEqual(value_a, value_b, tolerance)
+        elif (isinstance(value_a, list)):
+            for i, v_a in enumerate(value_a):
+                test_unit.assertAlmostEqual(v_a, value_b[i], tolerance)
+        else:
+            test_unit.assertAlmostEqual(value_a, value_b, tolerance)
+
+def CreateModelPart(model_part):
+    model_part.CreateNewNode(1, 0.0, 0.0, 0.0)
+    model_part.CreateNewNode(2, 1.0, 0.0, 0.0)
+    model_part.CreateNewNode(3, 2.0, 0.0, 0.0)
+    model_part.CreateNewNode(4, 2.0, 1.0, 0.0)
+    model_part.CreateNewNode(5, 1.5, 1.0, 0.0)
+    model_part.CreateNewNode(6, 0.5, 1.0, 0.0)
+    model_part.CreateNewNode(7, 0.0, 1.0, 0.0)
+
+    prop = model_part.GetProperties()[0]
+
+    model_part.CreateNewElement("Element2D3N", 1, [1, 6, 7], prop)
+    model_part.CreateNewElement("Element2D3N", 2, [1, 2, 6], prop)
+    model_part.CreateNewElement("Element2D3N", 3, [6, 2, 5], prop)
+    model_part.CreateNewElement("Element2D3N", 4, [2, 3, 5], prop)
+    model_part.CreateNewElement("Element2D3N", 5, [5, 3, 4], prop)
+
+    model_part.CreateNewCondition("LineCondition2D2N", 1, [1, 2], prop)
+    model_part.CreateNewCondition("LineCondition2D2N", 2, [2, 3], prop)
+    model_part.CreateNewCondition("LineCondition2D2N", 3, [3, 4], prop)
+    model_part.CreateNewCondition("LineCondition2D2N", 4, [4, 5], prop)
+    model_part.CreateNewCondition("LineCondition2D2N", 5, [5, 6], prop)
+    model_part.CreateNewCondition("LineCondition2D2N", 6, [6, 7], prop)
+    model_part.CreateNewCondition("LineCondition2D2N", 7, [7, 1], prop)
+
+def InitializeModelPartVariables(model_part, is_random = True):
+    if is_random:
+        scalar_method = lambda item : GetRandomValue()
+        array_3d_method = lambda item : GetRandomVector()
+        vector_method = lambda item : GetRandomVector(5)
+        matrix_method = lambda item : GetRandomMatrix()
+    else:
+        t = model_part.ProcessInfo[Kratos.STEP]
+        scalar_method = lambda item : GetInitialVariableValue(Kratos.PRESSURE, "none", (t+1) * (item.Id+1))
+        array_3d_method = lambda item : GetInitialVariableValue(Kratos.VELOCITY, "none", (t+1) * (item.Id +1) * 2.0)
+        vector_method = lambda item : GetInitialVariableValue(Kratos.LOAD_MESHES, "none", (t+1) * (item.Id + 2.0))
+        matrix_method = lambda item : GetInitialVariableValue(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, "none", (t+1) * (item.Id+3)* 2.0)
+
+    communicator = model_part.GetCommunicator()
+    container = communicator.LocalMesh()
+
+    for node in container.Nodes:
+        node.SetValue(Kratos.PRESSURE, scalar_method(node))
+        node.SetValue(Kratos.VELOCITY, array_3d_method(node))
+        node.SetValue(Kratos.LOAD_MESHES, vector_method(node))
+        node.SetValue(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, matrix_method(node))
+
+        node.SetSolutionStepValue(Kratos.PRESSURE, 0, scalar_method(node))
+        node.SetSolutionStepValue(Kratos.VELOCITY, 0, array_3d_method(node))
+        node.SetSolutionStepValue(Kratos.LOAD_MESHES, 0, vector_method(node))
+        node.SetSolutionStepValue(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, 0, matrix_method(node))
+
+    communicator.GetDataCommunicator().Barrier()
+    model_part.GetCommunicator().SynchronizeVariable(Kratos.PRESSURE)
+    model_part.GetCommunicator().SynchronizeVariable(Kratos.VELOCITY)
+    model_part.GetCommunicator().SynchronizeVariable(Kratos.LOAD_MESHES)
+    model_part.GetCommunicator().SynchronizeVariable(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR)
+    model_part.GetCommunicator().SynchronizeNonHistoricalVariable(Kratos.PRESSURE)
+    model_part.GetCommunicator().SynchronizeNonHistoricalVariable(Kratos.VELOCITY)
+    model_part.GetCommunicator().SynchronizeNonHistoricalVariable(Kratos.LOAD_MESHES)
+    model_part.GetCommunicator().SynchronizeNonHistoricalVariable(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR)
+
+    for condition in container.Conditions:
+        condition.SetValue(Kratos.PRESSURE, scalar_method(condition))
+        condition.SetValue(Kratos.VELOCITY, array_3d_method(condition))
+        condition.SetValue(Kratos.LOAD_MESHES, vector_method(condition))
+        condition.SetValue(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, matrix_method(condition))
+
+    for element in container.Elements:
+        element.SetValue(Kratos.PRESSURE, scalar_method(element))
+        element.SetValue(Kratos.VELOCITY, array_3d_method(element))
+        element.SetValue(Kratos.LOAD_MESHES, vector_method(element))
+        element.SetValue(Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, matrix_method(element))
+
+    communicator.GetDataCommunicator().Barrier()
+
+def GetInitialVariableValue(variable, norm_type, value = 0.0):
+    if (norm_type == "none"):
+        if (variable == Kratos.PRESSURE):
+            return value
+        elif (variable == Kratos.VELOCITY):
+            return Kratos.Vector(3, value)
+        elif (variable == Kratos.LOAD_MESHES):
+            return Kratos.Vector(5, value)
+        elif (variable == Kratos.GREEN_LAGRANGE_STRAIN_TENSOR):
+            return Kratos.Matrix(5, 5, value)
+    else:
+        return 0.0
+
+def InitializeProcesses(test):
+    communicator = test.model_part.GetCommunicator().GetDataCommunicator()
+    for process in test.process_list:
+        communicator.Barrier()
+        process.Check()
+
+    for process in test.process_list:
+        communicator.Barrier()
+        process.ExecuteInitialize()
+
+def ExecuteProcessFinalizeSolutionStep(test):
+    communicator = test.model_part.GetCommunicator().GetDataCommunicator()
+    for process in test.process_list:
+        communicator.Barrier()
+        process.ExecuteFinalizeSolutionStep()
```

## Comparing `KratosStatisticsApplication-9.4.5.dist-info/METADATA` & `KratosStatisticsApplication-9.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,821 +1,821 @@
-Metadata-Version: 2.1
-Name: KratosStatisticsApplication
-Version: 9.4.5
-Summary: KRATOS Multiphysics ("Kratos") is a framework for building parallel, multi-disciplinary simulation software, aiming at modularity, extensibility, and high performance. Kratos is written in C++, and counts with an extensive Python interface.
-Home-page: https://github.com/KratosMultiphysics/
-Author: Kratos Team
-Author-email: kratos@listas.cimne.upc.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Other Audience
-Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: KratosMultiphysics (==9.4.5)
-
-# Statistics Application
-
-Statistics application consist of widely used methods to calculate statistics in various containers of KratosMultiphysics. There are mainly two groups of statistical methods namely **Spatial** and **Temporal**. **Spatial** methods calculate statistics on spatial containers and output the values whenever they are called. **Temporal** methods calculate statistics on the fly in a transient simulation. All the temporal methods gurantee that, the resultant statistics will be same as the ones if one calculates accumulating all the data upto that time instance and calculate the same statistics. All of these methods in each group is `OpenMP` and `MPI` compatible, and tested.
-
-Following table summarize capabilities of Statistics Application.
-
-| Statistical Methods                   | Norm Types              | Spatial Domain                                                | Temporal Domain                                                              | Data types |
-|---------------------------------------|-------------------------|---------------------------------------------------------------|------------------------------------------------------------------------------|------------|
-| [Sum](#sum)                           | [Value](#value)         | [Spatial methods](#spatial-methods)                           | [Temporal methods](#temporal-methods)                                        | Double     |
-| [Mean](#mean)                         | [Magnitude](#magnitude) | [Spatial containers](#spatial-containers)                     | [Temporal containers](#temporal-containers)                                  | Array 3D   |
-| [Root mean square](#root-mean-square) | [Euclidean](#euclidean) | [nodal_historical](#spatial-nodal-historical)                 | [nodal_historical_historical](#temporal-nodal-historical-historical)         | Vector     |
-| [Variance](#variance)                 | [Infinity](#infinity)   | [nodal_non_historical](#spatial-nodal-non-historical)         | [nodal_historical_non_historical](#temporal-nodal-historical-non-historical) | Matrix     |
-| [Min](#min)                           | [P-Norm](#p-norm)       | [condition_non_historical](#spatial-condition-non-historical) | [nodal_non_historical](#temporal-nodal-non-historical)                       |            |
-| [Max](#max)                           | [Lpq-Norm](#lpq-norm)   | [element_non_historical](#spatial-element-non-historical)     | [element_non_historical](#temporal-element-non-historical)                   |            |
-| [Median](#median)                     | [Frobenius](#frobenius) | [Spatial statistics process](#spatial-statistics-process)     | [condition_non_historical](#temporal-condition-non-historical)               |            |
-| [Distribution](#distribution)         | [Trace](#trace)         |                                                               | [Temporal statistics process](#temporal-statistics-process)                  |            |
-| [Norm methods](#norm-methods)         | [Index](#index-based)         |                                                               |                                                                              |            |
-|                                       | [Component](#component-based) |                                                               |                                                                              |            |
-
-## JSON Examples
-
-If you prefer to use statistics of a simulation using StatisticsApplication, there is `spatial_statistics_process` for spatial statistics calculations and `temporal_statistics_process` for temporal statistics. These processes can be included via JSON settings under `auxiliary_processes`.
-
-### Spatial statistics process examples
-
-Following example illustrates different methods used in different containers with different norms. `input_variable_settings` holds an array of methods for specified containers, specified norm and specified variables. They can be customized for your requirement. `output_settings` holds information about how the output should be handled.
-
-```json
-{
-                "kratos_module" : "KratosMultiphysics.StatisticsApplication",
-                "python_module" : "spatial_statistics_process",
-                "Parameters" : {
-                    "model_part_name" : "test_model_part",
-                    "input_variable_settings" : [
-                        {
-                            "method_name"    : "sum",
-                            "norm_type"      : "none",
-                            "container"      : "nodal_historical",
-                            "variable_names" : ["PRESSURE", "VELOCITY"],
-                            "method_settings": {}
-                        },
-                        {
-                            "method_name"    : "mean",
-                            "norm_type"      : "none",
-                            "container"      : "nodal_non_historical",
-                            "variable_names" : ["PRESSURE", "VELOCITY"],
-                            "method_settings": {}
-                        },
-                        {
-                            "method_name"    : "variance",
-                            "norm_type"      : "none",
-                            "container"      : "element_non_historical",
-                            "variable_names" : ["PRESSURE", "VELOCITY"],
-                            "method_settings": {}
-                        },
-                        {
-                            "method_name"    : "rootmeansquare",
-                            "norm_type"      : "none",
-                            "container"      : "condition_non_historical",
-                            "variable_names" : ["PRESSURE", "VELOCITY"],
-                            "method_settings": {}
-                        },
-                        {
-                            "method_name"    : "sum",
-                            "norm_type"      : "magnitude",
-                            "container"      : "nodal_historical",
-                            "variable_names" : ["PRESSURE", "VELOCITY", "LOAD_MESHES", "GREEN_LAGRANGE_STRAIN_TENSOR"],
-                            "method_settings": {}
-                        },
-                        {
-                            "method_name"    : "mean",
-                            "norm_type"      : "pnorm_2.5",
-                            "container"      : "nodal_non_historical",
-                            "variable_names" : ["VELOCITY", "LOAD_MESHES", "GREEN_LAGRANGE_STRAIN_TENSOR"],
-                            "method_settings": {}
-                        },
-                        {
-                            "method_name"    : "variance",
-                            "norm_type"      : "component_x",
-                            "container"      : "condition_non_historical",
-                            "variable_names" : ["VELOCITY"],
-                            "method_settings": {}
-                        },
-                        {
-                            "method_name"    : "rootmeansquare",
-                            "norm_type"      : "index_3",
-                            "container"      : "nodal_non_historical",
-                            "variable_names" : ["LOAD_MESHES"],
-                            "method_settings": {}
-                        },
-                        {
-                            "method_name"    : "min",
-                            "norm_type"      : "frobenius",
-                            "container"      : "nodal_non_historical",
-                            "variable_names" : ["GREEN_LAGRANGE_STRAIN_TENSOR"],
-                            "method_settings": {}
-                        }
-                    ],
-                    "output_settings" : {
-                        "output_control_variable": "STEP",
-                        "output_time_interval"   : 1,
-                        "write_kratos_version"   : false,
-                        "write_time_stamp"       : false,
-                        "output_file_settings"   : {
-                            "file_name"  : "<model_part_name>_<container>_<norm_type>_<method_name>.dat",
-                            "output_path": "spatial_statistics_process",
-                            "write_buffer_size" : -1
-                        }
-                    }
-                }
-            }
-```
-
-### Temporal statistics process example
-
-Following is an example on how to use `temporal_statistics_process` in json. The output variables data type should be matched with the input variables order and the data type for `"norm_type" = "none"`. If `"norm_type" != "none"`, then output variables should be `scalars`. If `"container" = "nodal_historical_historical"` is used as the container type, then output variables should be added to `NodalSolutionStepVariables` list in Kratos since this container type outputs temporal statistics variables to nodal historical container. This json settings also can be added to `auxiliary_processes` list.
-
-For details about all the available statistical methods, norm_types, etc, please refer to rest of the `README.md` file.
-
-```json
-        {
-            "kratos_module": "KratosMultiphysics.StatisticsApplication",
-            "python_module": "temporal_statistics_process",
-            "Parameters": {
-                "model_part_name": "FluidModelPart.fluid_computational_model_part",
-                "input_variable_settings": [
-                    {
-                        "method_name": "variance",
-                        "norm_type": "none",
-                        "container": "nodal_historical_non_historical",
-                        "echo_level": 1,
-                        "method_settings": {
-                            "input_variables": [
-                                "VELOCITY",
-                                "PRESSURE"
-                            ],
-                            "output_mean_variables": [
-                                "VECTOR_3D_MEAN",
-                                "SCALAR_MEAN"
-                            ],
-                            "output_variance_variables": [
-                                "VECTOR_3D_VARIANCE",
-                                "SCALAR_VARIANCE"
-                            ]
-                        }
-                    }
-                ],
-                "statistics_start_point_control_variable_name": "TIME",
-                "statistics_start_point_control_value": 2.5
-            }
-        }
-```
-
-## Method definitions
-
-There are two types of methods under each **Spatial** and **Temporal** method groups. They are namely **Value** and **Norm** methods. In these methods, `i` index refers to spatial domain element index, and `k` index refers to time step.
-
-### Value methods
-
-#### Sum
-
-In the case of spatial domain, it adds up all the variable values for a given container and returns summed up value as shown in following equation. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{r}&space;=&space;\sum_{i=1}^N{\underline{x}_i}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{r}&space;=&space;\sum_{i=1}^N{\underline{x}_i}}" title="\color{Black}{\underline{r} = \sum_{i=1}^N{\underline{x}_i}}" /></a>
-
-Following is an example of summation of non historical `VELOCITY` over the whole model part's nodes
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Sum(model_part, Kratos.VELOCITY)
-```
-
-In the case of temporal domain, **Sum** methods is the time integrated quantity for a specific variable. It will be stored each element under user specified variable and a user specified container. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{r}&space;=&space;\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}&space;\quad&space;where&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{r}&space;=&space;\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}&space;\quad&space;where&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" title="\color{Black}{\underline{r} = \sum_{k=1}^{P}{\underline{x}_k\Delta t_k} \quad where \quad \Delta t_k = T_{k} - T_{k-1} \quad \forall T_k \in \left\lbrace T_{initial}, ..., T_{end} \right\rbrace}" /></a>
-
-Following is an example of integration calculation of non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable is same containers `DISPLACEMENT` where integrated value will be stored for each node. The `0` represents echo level for this method object. Blank "" indicates that value method is used.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
-integration_starting_time = 2.0
-sum_method.InitializeStatisticsMethod(integration_starting_time)
-for t in range(3, 6):
-    sum_method.CalculateStatistics()
-```
-
-#### Mean
-
-In the case of spatial domain, it calculates mean of a given variable for a given container and returns it as shown in following equation. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user. (If it has higher dimension than a scalar, mean of each dimension will be calculated seperately resulting with a mean having same dimension as the input dimension)
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{r}&space;=&space;\frac{1}{N}\sum_{i=1}^{N}\underline{x}_i}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{r}&space;=&space;\frac{1}{N}\sum_{i=1}^{N}\underline{x}_i}" title="\color{Black}{\underline{r} = \frac{1}{N}\sum_{i=1}^{N}\underline{x}_i}" /></a>
-
-Following is an example of mean calculation of non historical `VELOCITY` over the whole model part's nodes
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-mean = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Mean(model_part, Kratos.VELOCITY)
-```
-
-In the case of temporal domain, **Mean** methods is the time integrated quantity's mean for a specific variable. It will be stored each element under user specified variable and a user specified container. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user preserving the dimensionality as in the spatial case.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}&space;\quad&space;where&space;\quad&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}&space;\quad&space;where&space;\quad&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" title="\color{Black}{\underline{\bar{x}} = \frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta t_k} \quad where \quad T_{total} = T_{end} - T_{initial} \quad and \quad \Delta t_k = T_{k} - T_{k-1} \quad \forall T_k \in \left\lbrace T_{initial}, ..., T_{end} \right\rbrace}" /></a>
-
-Following is an example of mean calculation of non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable is same containers `VECTOR_3D_MEAN` where mean will be stored for each node. The `0` represents echo level for this method object. Blank "" indicates that value method is used.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-mean_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Mean.Array(model_part, "", Kratos.VELOCITY, 0, KratosStats.VECTOR_3D_MEAN)
-integration_starting_time = 2.0
-mean_method.InitializeStatisticsMethod(integration_starting_time)
-for t in range(3, 6):
-    mean_method.CalculateStatistics()
-```
-
-#### Root mean square
-
-In the case of spatial domain, it calculates root mean square of a given variable for a given container and returns it as shown in following equation. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user. (If it has higher dimension than a scalar, root mean square of each dimension will be calculated seperately resulting with a mean having same dimension as the input dimension)
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{r}&space;=&space;\sqrt{\frac{1}{N}\sum_{i=1}^{N}{\underline{x}^2_i}&space;}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{r}&space;=&space;\sqrt{\frac{1}{N}\sum_{i=1}^{N}{\underline{x}^2_i}&space;}}" title="\color{Black}{\underline{r} = \sqrt{\frac{1}{N}\sum_{i=1}^{N}{\underline{x}^2_i} }}" /></a>
-
-Following is an example of root mean square calculation of non historical `VELOCITY` over the whole model part's nodes
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-rms = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.RootMeanSquare(model_part, Kratos.VELOCITY)
-```
-
-In the case of temporal domain, **Root Mean Square** methods is the time integrated quantity's root mean square for a specific variable. It will be stored each element under user specified variable and a user specified container. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user preserving the dimensionality as in the spatial case.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{r}&space;=&space;\sqrt{\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k^2\Delta&space;t_k}}&space;\quad&space;where&space;\quad&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{r}&space;=&space;\sqrt{\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k^2\Delta&space;t_k}}&space;\quad&space;where&space;\quad&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" title="\color{Black}{\underline{r} = \sqrt{\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k^2\Delta t_k}} \quad where \quad T_{total} = T_{end} - T_{initial} \quad and \quad \Delta t_k = T_{k} - T_{k-1} \quad \forall T_k \in \left\lbrace T_{initial}, ..., T_{end} \right\rbrace}" /></a>
-
-Following is an example of root mean square calculation of non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable is same containers `VECTOR_3D_MEAN` where root mean square value will be stored for each node. The `0` represents echo level for this method object. Blank "" indicates that value method is used.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-rms_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.RootMeanSquare.Array(model_part, "", Kratos.VELOCITY, 0, KratosStats.VECTOR_3D_MEAN)
-integration_starting_time = 2.0
-rms_method.InitializeStatisticsMethod(integration_starting_time)
-for t in range(3, 6):
-    rms_method.CalculateStatistics()
-```
-
-#### Variance
-
-In the case of spatial domain, it calculates variance of a given variable for a given container and returns mean and variance as shown in following equations. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Results will have the same type as the type of the variable specified by the user. (If it has higher dimension than a scalar, mean of each dimension will be calculated seperately resulting with a mean having same dimension as the input dimension)
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{N}\sum_{i=1}^N{\underline{x}_i}}&space;\\&space;\color{Black}{\underline{v}&space;=&space;\frac{1}{N}\sum_{i=1}^N{\left(\underline{x}_i&space;-&space;\underline{\bar{x}}&space;\right&space;)^2}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{N}\sum_{i=1}^N{\underline{x}_i}}&space;\\&space;\color{Black}{\underline{v}&space;=&space;\frac{1}{N}\sum_{i=1}^N{\left(\underline{x}_i&space;-&space;\underline{\bar{x}}&space;\right&space;)^2}}" title="\color{Black}{\underline{\bar{x}} = \frac{1}{N}\sum_{i=1}^N{\underline{x}_i}} \\ \color{Black}{\underline{v} = \frac{1}{N}\sum_{i=1}^N{\left(\underline{x}_i - \underline{\bar{x}} \right )^2}}" /></a>
-
-Following is an example of variance calculation of non historical `VELOCITY` over the whole model part's nodes
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-mean, variance = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Variance(model_part, Kratos.VELOCITY)
-```
-
-In the case of temporal domain, **Variance** method is the time integrated quantity's variance for a specific variable. Mean and variance will be stored each element under user specified variables and a user specified container. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Results will have the same type as the type of the variable specified by the user preserving the dimensionality as in the spatial case.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}}&space;\\&space;\color{Black}{Var\left(\underline{x}&space;\right&space;)&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\left(\underline{x}_k&space;-&space;\underline{\bar{x}}&space;\right&space;)^2\Delta&space;t_k}}&space;\\&space;\\&space;\color{Black}{&space;\quad&space;where}&space;\\&space;\\&space;\color{Black}{&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}}&space;\\&space;\color{Black}{Var\left(\underline{x}&space;\right&space;)&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\left(\underline{x}_k&space;-&space;\underline{\bar{x}}&space;\right&space;)^2\Delta&space;t_k}}&space;\\&space;\\&space;\color{Black}{&space;\quad&space;where}&space;\\&space;\\&space;\color{Black}{&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" title="\color{Black}{\underline{\bar{x}} = \frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta t_k}} \\ \color{Black}{Var\left(\underline{x} \right ) = \frac{1}{T_{total}}\sum_{k=1}^{P}{\left(\underline{x}_k - \underline{\bar{x}} \right )^2\Delta t_k}} \\ \\ \color{Black}{ \quad where} \\ \\ \color{Black}{ T_{total} = T_{end} - T_{initial} \quad and \quad \Delta t_k = T_{k} - T_{k-1} \quad \forall T_k \in \left\lbrace T_{initial}, ..., T_{end} \right\rbrace}" /></a>
-
-Following is an example of root mean square calculation of non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable `VECTOR_3D_MEAN` will store mean and `VECTOR_3D_VARIANCE` will store variance in same container for each node. The `0` represents echo level for this method object. Blank "" indicates that value method is used.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-variance_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Variance.Array(model_part, "", Kratos.VELOCITY, 0, KratosStats.VECTOR_3D_MEAN, KratosStats.VECTOR_3D_VARIANCE)
-integration_starting_time = 2.0
-variance_method.InitializeStatisticsMethod(integration_starting_time)
-for t in range(3, 6):
-    variance_method.CalculateStatistics()
-```
-
-#### Min
-
-In the case of spatial domain, it returns minimum of a given variable's norm for a given container, and the corresponding items id. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Results will be double and integer, irrespective of the input type, since higher dimensional variable types will be reduced to scalars by the use of norms.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{v&space;=&space;\min_{\underline{x}_i&space;\in&space;\mathbf{T}}&space;|\underline{x}_i|}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{v&space;=&space;\min_{\underline{x}_i&space;\in&space;\mathbf{T}}&space;|\underline{x}_i|}" title="\color{Black}{v = \min_{\underline{x}_i \in \mathbf{T}} |\underline{x}_i|}" /></a>
-
-Following is an example of min method of non historical `VELOCITY`'s magnitude over the whole model part's nodes. It returns a tuple, first argument being the minimum, and the second argument being the id of the node where the minimum is found.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-min_value, min_id = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Min(model_part, Kratos.VELOCITY, "magnitude")
-```
-
-In the case of temporal domain, **Min** method returns minimum value in the temporal domain, and the time minimum is found. Minimum and its occurring time will be stored each element under user specified variables and a user specified container. x<sub>k</sub> is the k<sup>th</sup> time step element's variable value of the corresponding container. Results will have the same type as the type of the variable specified by the user preserving the dimensionality as in the spatial case.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{v&space;=&space;\min_{\underline{x}_k&space;\in&space;\mathbf{T}}&space;|\underline{x}_k|}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{v&space;=&space;\min_{\underline{x}_k&space;\in&space;\mathbf{T}}&space;|\underline{x}_k|}" title="\color{Black}{v = \min_{\underline{x}_k \in \mathbf{T}} |\underline{x}_k|}" /></a>
-
-Following is an example of min method in non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable `VECTOR_3D_NORM` will store minimum and `TIME` will store the time minimum occured for each node. The `0` represents echo level for this method object. "magnitude" indicates that magnitude norm is used.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-min_method = KratosStats.TemporalMethods.NonHistorical.Nodes.NormMethods.Min.Array(model_part, "magnitude", Kratos.VELOCITY, 0, KratosStats.VECTOR_3D_NORM, Kratos.TIME)
-integration_starting_time = 2.0
-min_method.InitializeStatisticsMethod(integration_starting_time)
-for t in range(3, 6):
-    min_method.CalculateStatistics()
-```
-
-#### Max
-
-In the case of spatial domain, it returns maximum of a given variable's norm for a given container, and the corresponding items id. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Results will be double and integer, irrespective of the input type, since higher dimensional variable types will be reduced to scalars by the use of norms.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{v&space;=&space;\max_{\underline{x}_i&space;\in&space;\Omega}&space;|\underline{x}_i|}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{v&space;=&space;\max_{\underline{x}_i&space;\in&space;\Omega}&space;|\underline{x}_i|}" title="\color{Black}{v = \max_{\underline{x}_i \in \Omega} |\underline{x}_i|}" /></a>
-
-Following is an example of max method of non historical `VELOCITY`'s magnitude over the whole model part's nodes. It returns a tuple, first argument being the maximum, and the second argument being the id of the node where the maximum is found.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-max_value, max_id = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Max(model_part, Kratos.VELOCITY, "magnitude")
-```
-
-In the case of temporal domain, **Max** method returns maximum value in the temporal domain, and the time maximum is found. Maximum and its occurring time will be stored each element under user specified variables and a user specified container. x<sub>k</sub> is the k<sup>th</sup> time step element's variable value of the corresponding container. Results will have the same type as the type of the variable specified by the user preserving the dimensionality as in the spatial case.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{v&space;=&space;\max_{\underline{x}_k&space;\in&space;\mathbf{T}}&space;|\underline{x}_k|}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{v&space;=&space;\max_{\underline{x}_k&space;\in&space;\mathbf{T}}&space;|\underline{x}_k|}" title="\color{Black}{v = \max_{\underline{x}_k \in \mathbf{T}} |\underline{x}_k|}" /></a>
-
-Following is an example of max method in non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable `VECTOR_3D_NORM` will store maximum and `TIME` will store the time maximum occured for each node. The `0` represents echo level for this method object. "magnitude" indicates that magnitude norm is used.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-max_method = KratosStats.TemporalMethods.NonHistorical.Nodes.NormMethods.Max.Array(model_part, "magnitude", Kratos.VELOCITY, 0, KratosStats.VECTOR_3D_NORM, Kratos.TIME)
-integration_starting_time = 2.0
-max_method.InitializeStatisticsMethod(integration_starting_time)
-for t in range(3, 6):
-    max_method.CalculateStatistics()
-```
-
-#### Median
-
-Median returns the median value in spatial domain of a given variable's norm for a given container. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Results will be double value type, irrespective of the input type, since higher dimensional variable types will be reduced to scalars by the use of norms.
-
-Following is an example of median method of non historical `VELOCITY`'s magnitude over the whole model part's nodes. It returns a double which is the median.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-median_value = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Median(model_part, Kratos.VELOCITY, "magnitude")
-```
-
-#### Distribution
-
-Distribution methods calculates distribution of a given variable with respect to given norm in a given container in spatial domain. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will be a tuple with followings in the same order:
-
-1. min in the domain or user specified min value
-2. max in the domain or user specified min value
-3. group limits of the distribution (only upper limit) (double array)
-4. number of occurences of items within each group (int array)
-5. percentage distribution of number of occurences of items within each group (double array)
-6. Each group's seperate means
-7. Eash group's seperate variances
-
-This method requires followings as the parameters as a object of Kratos.Parameters, if nothing is provided, then followings are assumed as defaults.
-
-```json
-{
-    "number_of_value_groups" : 10,
-    "min_value"              : "min",
-    "max_value"              : "max"
-}
-```
-
-In here, `"min_value"` can either be `"min"` or a `double` value. In the case of a double, it will be used as the minimum when creating groups to identify distribution. `"max_value"` also can either be `"max"` of `double` value, which will determine the maximum value when creating the groups. This will create 2 additional groups to represent values below the specified `"min_value"` and `"max_value"` apart from the `"number_of_value_groups"` specified by the user.
-
-Following is an example of median method of non historical `VELOCITY`'s magnitude over the whole model part's nodes.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-min_value, max_value, group_upper_values, group_histogram, group_percentage_distribution, group_means, group_variances = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Distribution(model_part, Kratos.VELOCITY, "magnitude")
-```
-
-### Norm methods
-
-All of the value methods mentioned before supports norm version of it, in these methods, higher dimensional values are transformed in to scalar values by a use specified norm, and then statistics are calculated based on the chosen method. Supported norm types may differ based on the variable data type being used. There are few methods, which only supports norm methods. Following table summarize availability of value and norm methods.
-
-| Statistical Methods                   | Value Method | Norm Method |
-|---------------------------------------|--------------|-------------|
-| [Sum](#sum)                           | [x]          | [x]         |
-| [Mean](#mean)                         | [x]          | [x]         |
-| [Root mean square](#root-mean-square) | [x]          | [x]         |
-| [Variance](#variance)                 | [x]          | [x]         |
-| [Min](#min)                           |              | [x]         |
-| [Max](#max)                           |              | [x]         |
-| [Median](#median)                     |              | [x]         |
-| [Distribution](#distribution)         |              | [x]         |
-
-Following example shows variance method, under **value** category and **norm** category for nodal non historical velocity. Norm method uses `"magnitude"` as the norm to reduce `VELOCITY` to a scalar value. `value_mean` and `value_variance` will be of `Array 3D` type, whereas `norm_mean` and `norm_variance` will be of `Double` type.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-value_mean, value_variance = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Variance(model_part, Kratos.VELOCITY)
-norm_mean, norm_variance = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Variance(model_part, Kratos.VELOCITY, "magnitude")
-```
-
-## Norm definitions
-
-Few different norms are predefined in this application. Following table summarize
-
-|                               | Double | Array 3D | Vector | Matrix |
-|-------------------------------|--------|----------|--------|--------|
-| [Value](#value)               | [x]    |          |        |        |
-| [Magnitude](#magnitude)       | [x]    | [x]      | [x]    | [x]    |
-| [Euclidean](#euclidean)       |        | [x]      | [x]    |        |
-| [Infinity](#infinity)         |        | [x]      | [x]    | [x]    |
-| [P-Norm](#p-norm)             |        | [x]      | [x]    | [x]    |
-| [Lpq-Norm](#lpq-norm)         |        |          |        | [x]    |
-| [Frobenius](#frobenius)       |        |          |        | [x]    |
-| [Trace](#trace)               |        |          |        | [x]    |
-| [Index](#index-based)         |        |          | [x]    | [x]    |
-| [Component](#component-based) |        | [x]      |        |        |
-
-### Value
-
-This returns the exact value. Only available for `Double` type variables.
-
-### Magnitude
-
-This returns the second norm of the variable.
-
-1. For a `Double` type, it returns the absolute value.
-2. For a `Array 3D` type, it returns the magnitude of the 3D vector.
-3. For a `Vector` type, it returns root square sum of the vector.
-4. For a `Matrix` type, it returns the [frobenius](#frobenius) norm.
-
-### Euclidean
-
-This again returns the second norm of the variable for following variable types.
-
-1. For a `Array 3D` type, it returns the magnitude of the 3D vector.
-2. For a `Vector` type, it returns root square sum of the vector.
-
-### Frobenius
-
-This is only available for `Matrix` data type variables only. Following equation illustrates the norm, where `A` is the matrix and a<sub>ij</sub> is the i<sup>th</sup> row, j<sup>th</sup> column value.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||A||_F&space;=&space;\sqrt{\sum_i&space;{\sum_j{||a_{ij}||^2}}}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||A||_F&space;=&space;\sqrt{\sum_i&space;{\sum_j{||a_{ij}||^2}}}}" title="{\color{Black} ||A||_F = \sqrt{\sum_i {\sum_j{||a_{ij}||^2}}}}" /></a>
-
-### Infinity
-
-This is infinity (i.e. max norm) which is available for `Array 3D`, `Vector` and `Matrix` type.
-For an `Array 3D` variable following equation is used.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{V}||_\infty&space;=&space;\max\left&space;\lbrace&space;{|V_X|,&space;|V_Y|,&space;|V_Z|}\right&space;\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{V}||_\infty&space;=&space;\max\left&space;\lbrace&space;{|V_X|,&space;|V_Y|,&space;|V_Z|}\right&space;\rbrace}" title="{\color{Black} ||\underline{V}||_\infty = \max\left \lbrace {|V_X|, |V_Y|, |V_Z|}\right \rbrace}" /></a>
-
-For a `Vector` variable following equation is used.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{V}||_\infty&space;=&space;\max\left&space;\lbrace&space;{|V_0|,&space;|V_1|,&space;|V_2|,...,{V_{n-1}}}\right&space;\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{V}||_\infty&space;=&space;\max\left&space;\lbrace&space;{|V_0|,&space;|V_1|,&space;|V_2|,...,{V_{n-1}}}\right&space;\rbrace}" title="{\color{Black} ||\underline{V}||_\infty = \max\left \lbrace {|V_0|, |V_1|, |V_2|,...,{V_{n-1}}}\right \rbrace}" /></a>
-
-For a `Matrix` variable following equation is used.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{A}||_\infty&space;=&space;\max_{0&space;\leq&space;i&space;<&space;n}\left(&space;\sum_{j=0}^{n-1}&space;|a_{ij}|\right&space;)}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{A}||_\infty&space;=&space;\max_{0&space;\leq&space;i&space;<&space;n}\left(&space;\sum_{j=0}^{n-1}&space;|a_{ij}|\right&space;)}" title="{\color{Black} ||\underline{A}||_\infty = \max_{0 \leq i < n}\left( \sum_{j=0}^{n-1} |a_{ij}|\right )}" /></a>
-
-### Trace
-
-Trace is only for `Matrix` type variables. If the given matrix is not squre, an error is thrown.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{A}||_{trace}&space;=&space;\sum_{i=0}^{n-1}a_{ij}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{A}||_{trace}&space;=&space;\sum_{i=0}^{n-1}a_{ij}}" title="{\color{Black} ||\underline{A}||_{trace} = \sum_{i=0}^{n-1}a_{ij}}" /></a>
-
-### P norm
-
-P norm is applicable for `Array 3D`, `Vector` and `Matrix` variables. The p-norm is used as `pnorm_p` where, `p` represents the value to be used as `p` in the p-norm equation given below. `p` should be greater than or equal to 1.0.
-
-For `Array 3D` and `Vector`:
-
-<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{V}||_{p}&space;=&space;\left(\sum_{i=0}^{n-1}|v_{i}|^p&space;\right&space;)^{1/p}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{V}||_{p}&space;=&space;\left(\sum_{i=0}^{n-1}|v_{i}|^p&space;\right&space;)^{1/p}}" title="{\color{Black} ||\underline{V}||_{p} = \left(\sum_{i=0}^{n-1}|v_{i}|^p \right )^{1/p}}" /></a>
-
-For `Matrix`:
-
-<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{A}||_{p}&space;=&space;\left(\sum_{i=0}^{n-1}\sum_{j=0}^{n-1}|a_{ij}|^p&space;\right&space;)^{1/p}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{A}||_{p}&space;=&space;\left(\sum_{i=0}^{n-1}\sum_{j=0}^{n-1}|a_{ij}|^p&space;\right&space;)^{1/p}}" title="{\color{Black} ||\underline{A}||_{p} = \left(\sum_{i=0}^{n-1}\sum_{j=0}^{n-1}|a_{ij}|^p \right )^{1/p}}" /></a>
-
-### Lpq norm
-
-This norm is only applicable to `Matrix` type variables.
-
-<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{A}||_{lpq}&space;=&space;\left(\sum_{j=0}^{n-1}\left(\sum_{i=0}^{n-1}|a_{ij}|^p&space;\right&space;)^{q/p}&space;\right&space;)^{1/q}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{A}||_{lpq}&space;=&space;\left(\sum_{j=0}^{n-1}\left(\sum_{i=0}^{n-1}|a_{ij}|^p&space;\right&space;)^{q/p}&space;\right&space;)^{1/q}}" title="{\color{Black} ||\underline{A}||_{lpq} = \left(\sum_{j=0}^{n-1}\left(\sum_{i=0}^{n-1}|a_{ij}|^p \right )^{q/p} \right )^{1/q}}" /></a>
-
-### Index based
-
-Index based norms are available for both `Vector` and `Matrix` based variable types. `index_i` is used for `Vector` variables, where `i` represents the index of the vector to be used as the scalar representing a corresponding vector. `index_(i,j)` is used for `Matrix` variables, where `i` represents the row index and `j` represents the column index of the matrix value which to be used as the scalar representation of the given matrix.
-
-### Component based
-
-Component based norms are available only for `Array 3D` type variables. `component_x` represents the `x` component of 3D variable, `component_y` represents `y` component, `component_z` represents the `z` component.
-
-
-## Spatial methods
-
-All the spatial statistical methods can be found in the `SpatialMethods` submodule. `ValueMethods` container will contain all available spatial value methods, and `NormMethods` container will contain all available norm methods.
-
-Following example illustrates all the available value methods executed on nodal non historical variable velocity.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_value = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Sum(model_part, Kratos.VELOCITY)
-mean_value = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Mean(model_part, Kratos.VELOCITY)
-rms_value = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.RootMeanSquare(model_part, Kratos.VELOCITY)
-mean_value, variance_value = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Variance(model_part, Kratos.VELOCITY)
-```
-
-Following example illustrates all the available norm methods executed on nodal non historical variable velocity's magnitude.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_norm = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Sum(model_part, Kratos.VELOCITY, "magnitude")
-mean_norm = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Mean(model_part, Kratos.VELOCITY, "magnitude")
-rms_norm = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.RootMeanSquare(model_part, Kratos.VELOCITY, "magnitude")
-mean_norm, variance_norm = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Variance(model_part, Kratos.VELOCITY, "magnitude")
-min_norm, min_norm_id = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Min(model_part, Kratos.VELOCITY, "magnitude")
-max_norm, max_norm_id = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Max(model_part, Kratos.VELOCITY, "magnitude")
-min_norm, max_norm, group_upper_norms, group_histogram, group_percentage_distribution = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Distribution(model_part, Kratos.VELOCITY, "magnitude")
-```
-
-### Spatial containers
-
-Four different types of containers are supported for spatial methods.
-
-1. [nodal_historical](#spatial-nodal-historical)
-2. [nodal_non_historical](#spatial-nodal-non-historical)
-3. [condition_non_historical](#spatial-condition-non-historical)
-4. [element_non_historical](#spatial-element-non-historical)
-
-#### Spatial nodal historical
-
-Nodal historical containers methods can be accessed through `Historical` submodule in `SpatialMethods`. This calculates chosen statistics of the variable in the nodal historical data. Following example illustrates use of value and norm methods.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-model_part.AddNodalSolutionStepVariable(Kratos.VELOCITY)
-sum_value = KratosStats.SpatialMethods.Historical.ValueMethods.Sum(model_part, Kratos.VELOCITY)
-sum_norm = KratosStats.SpatialMethods.Historical.NormMethods.Sum(model_part, Kratos.VELOCITY, "magnitude")
-```
-
-#### Spatial nodal non historical
-
-Nodal non historical containers methods can be accessed through `NonHistorical.Nodes` submodule in `SpatialMethods`. This calculates chosen statistics of the variable in the nodal non historical data. Following example illustrates use of value and norm methods.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_value = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Sum(model_part, Kratos.VELOCITY)
-sum_norm = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Sum(model_part, Kratos.VELOCITY, "magnitude")
-```
-
-#### Spatial condition non historical
-
-Condition non historical containers methods can be accessed through `NonHistorical.Conditions` submodule in `SpatialMethods`. This calculates chosen statistics of the variable in the condition non historical data. Following example illustrates use of value and norm methods.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_value = KratosStats.SpatialMethods.NonHistorical.Conditions.ValueMethods.Sum(model_part, Kratos.VELOCITY)
-sum_norm = KratosStats.SpatialMethods.NonHistorical.Conditions.NormMethods.Sum(model_part, Kratos.VELOCITY, "magnitude")
-```
-
-#### Spatial element non historical
-
-Element non historical containers methods can be accessed through `NonHistorical.Elements` submodule in `SpatialMethods`. This calculates chosen statistics of the variable in the element non historical data. Following example illustrates use of value and norm methods.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_value = KratosStats.SpatialMethods.NonHistorical.Elements.ValueMethods.Sum(model_part, Kratos.VELOCITY)
-sum_norm = KratosStats.SpatialMethods.NonHistorical.Elements.NormMethods.Sum(model_part, Kratos.VELOCITY, "magnitude")
-```
-
-### Spatial statistics process
-
-This is a seperate process, which can be included in the json file as an auxiliary process. Followings are the defaults used in this process.
-
-```json
-{
-    "model_part_name" : "PLEASE_SPECIFY_MODEL_PART_NAME",
-    "input_variable_settings" : [
-        {
-            "method_name"    : "sum",
-            "norm_type"      : "none",
-            "container"      : "nodal_historical",
-            "variable_names" : [],
-            "method_settings": {}
-        }
-    ],
-    "output_settings" : {
-        "output_control_variable": "STEP",
-        "output_time_interval"   : 1,
-        "write_kratos_version"   : true,
-        "write_time_stamp"       : true,
-        "output_file_settings"   : {
-            "file_name"  : "<model_part_name>_<container>_<norm_type>_<method_name>.dat",
-            "output_path": "spatial_statistics_output",
-            "write_buffer_size" : -1
-        }
-    }
-}
-```
-
-`model_part_name` indicates which model part to be operated on for statistics calculation. `input_variable_settings` contains list of statistics and/or norm methods along with their acting containers of the model part. `method_name` is the statistics method name (always everything is in lower case). `norm_type` is the applied norm, `none` means, value methods are used, otherwise specified norm is used. `container` is the [container](#spatial-method-containers) to be specified for statistical value calculation. `method_settings` is used to pass additional information required by statistics method such as in [Distribution](#distribution) method. Output is written to a file in the format given at `file_name`, under the folder `folder_name`. This process can be used, if someone prefers not to modify their python scripts to calculate statistics as mentioned in the previous sections
-
-## Temporal methods
-
-All the temporal methods are available through `TemporalMethods` submodule under `StatisticsApplication`. In the case of temporal methods, seperate objects needs to be created for each input variable for different type of variables as shown in following example for nodal non historical data container value methods.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_double_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Double(model_part, "", Kratos.PRESSURE, 0, Kratos.DENSITY)
-sum_array_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
-sum_vector_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Vector(model_part, "", Kratos.LOAD_MESHES, 0, Kratos.MATERIAL_PARAMETERS)
-sum_matrix_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Matrix(model_part, "", Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, 0, Kratos.CAUCHY_STRESS_TENSOR)
-```
-
-In order to remove the hassle of using different names (such as `Double`, `Array`...), one can get the advantage of common methods available in each of the containers. Following example will create the same objects as in the previous example in one go using simplified sum method.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-params = Kratos.Parameters(r"""
-{
-    "input_variables" : ["PRESSURE", "VELOCITY", "LOAD_MESHES", "GREEN_LAGRANGE_STRAIN_TENSOR"],
-    "output_variables" : ["DENSITY", "DISPLACEMENT", "MATERIAL_PARAMETERS", "CAUCHY_STRESS_TENSOR"]
-}""")
-sum_methods = KratosStats.TemporalMethods.NonHistorical.Nodes.Sum(model_part, "none", 0, params)
-```
-
-For **Sum**, **Mean**, **RootMeanSquare** methods, above `Kratos.Parameters` object keys will remain the same. But for **Variance** method following `json` parameters are used.
-
-```json
-{
-    "input_variables"           : [],
-    "output_mean_variables"     : [],
-    "output_variance_variables" : []
-}
-```
-
-When using these simplified, one needs to take care of compatibility of input and output variables depending on the method and norm type, otherwise runtime errors will be thrown.
-
-### Temporal containers
-
-In the temporal domain, there are five different containers available for user to calculate temporal statistics. They are,
-
-1. [nodal_historical_historical](#temporal-nodal-historical-historical)
-2. [nodal_historical_non_historical](#temporal-nodal-historical-non-historical)
-3. [nodal_non_historical](#temporal-nodal-non-historical)
-4. [condition_non_historical](#temporal-condition-non-historical)
-5. [element_non_historical](#temporal-element-non-historical)
-
-#### Temporal nodal historical historical
-
-In this container, statistics are calculated on user specified variables in the nodal historical container and, output is also written to the nodal historical container. Example is given below.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_value = KratosStats.TemporalMethods.Historical.HistoricalOutput.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
-sum_norm = KratosStats.TemporalMethods.Historical.HistoricalOutput.NormMethods.Sum.Array(model_part, "magnitude", Kratos.VELOCITY, 0, Kratos.DENSITY)
-```
-
-#### Temporal nodal historical non historical
-
-In this container, statistics are calculated on user specified variables in the nodal historical container and, output is also written to the nodal non historical container. Example is given below.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_value = KratosStats.TemporalMethods.Historical.NonHistoricalOutput.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
-sum_norm = KratosStats.TemporalMethods.Historical.NonHistoricalOutput.NormMethods.Sum.Array(model_part, "magnitude", Kratos.VELOCITY, 0, Kratos.DENSITY)
-```
-
-#### Temporal nodal non historical
-
-In this container, statistics are calculated on user specified variables in the nodal non historical container and, output is also written to the nodal non historical container. Example is given below.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_value = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
-sum_norm = KratosStats.TemporalMethods.NonHistorical.Nodes.NormMethods.Sum.Array(model_part, "magnitude", Kratos.VELOCITY, 0, Kratos.DENSITY)
-```
-
-#### Temporal condition non historical
-
-In this container, statistics are calculated on user specified variables in the condition non historical container and, output is also written to the condition non historical container. Example is given below.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_value = KratosStats.TemporalMethods.NonHistorical.Conditions.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
-sum_norm = KratosStats.TemporalMethods.NonHistorical.Conditions.NormMethods.Sum.Array(model_part, "magnitude", Kratos.VELOCITY, 0, Kratos.DENSITY)
-```
-
-#### Temporal element non historical
-
-In this container, statistics are calculated on user specified variables in the element non historical container and, output is also written to the element non historical container. Example is given below.
-
-```python
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.StatisticsApplication as KratosStats
-model = Kratos.Model()
-model_part = model.CreateModelPart("test_model_part")
-sum_value = KratosStats.TemporalMethods.NonHistorical.Elements.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
-sum_norm = KratosStats.TemporalMethods.NonHistorical.Elements.NormMethods.Sum.Array(model_part, "magnitude", Kratos.VELOCITY, 0, Kratos.DENSITY)
-```
-
-### Temporal statistics process
-
-This is a seperate process, which can be included in the json file as an auxiliary process. Followings are the defaults used in this process.
-
-```json
-    "model_part_name" : "PLEASE_SPECIFY_MODEL_PART_NAME",
-    "input_variable_settings" : [
-        {
-            "method_name"     : "sum",
-            "norm_type"       : "none",
-            "container"       : "nodal_historical_non_historical",
-            "echo_level"      : 0,
-            "method_settings" : {}
-        }
-    ],
-    "echo_level" : 0,
-    "statistics_start_point_control_variable_name" : "TIME",
-    "statistics_start_point_control_value"         : 0.0
-```
-
-`model_part_name` is the model part which all of the mentioned statistics will be calculated. `input_variable_settings` contains list of statistical methods, their norms and container combinations where statistics will be calculated. under each `input_variable_settings_block`, `method_name` is the statistics method, `norm_type` is the norm type (`"none"` for value methods, other wise norms are used), `container` to tell from which container to read/write, `method_settings` to specifiy input/output variables for the method. Apart from that, there are few global settings. `statistics_start_point_control_variable_name` is the temporal statistics calculation start control variable name. This variable should be present in the model_part specified in order to calculate temporal statistics. Statistics calculation will start when this variable's value passes user specified value in `statistics_start_point_control_value`.
+Metadata-Version: 2.1
+Name: KratosStatisticsApplication
+Version: 9.5
+Summary: KRATOS Multiphysics ("Kratos") is a framework for building parallel, multi-disciplinary simulation software, aiming at modularity, extensibility, and high performance. Kratos is written in C++, and counts with an extensive Python interface.
+Home-page: https://github.com/KratosMultiphysics/
+Author: Kratos Team
+Author-email: kratos@listas.cimne.upc.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Other Audience
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: KratosMultiphysics ==9.5
+
+# Statistics Application
+
+Statistics application consist of widely used methods to calculate statistics in various containers of KratosMultiphysics. There are mainly two groups of statistical methods namely **Spatial** and **Temporal**. **Spatial** methods calculate statistics on spatial containers and output the values whenever they are called. **Temporal** methods calculate statistics on the fly in a transient simulation. All the temporal methods gurantee that, the resultant statistics will be same as the ones if one calculates accumulating all the data upto that time instance and calculate the same statistics. All of these methods in each group is `OpenMP` and `MPI` compatible, and tested.
+
+Following table summarize capabilities of Statistics Application.
+
+| Statistical Methods                   | Norm Types              | Spatial Domain                                                | Temporal Domain                                                              | Data types |
+|---------------------------------------|-------------------------|---------------------------------------------------------------|------------------------------------------------------------------------------|------------|
+| [Sum](#sum)                           | [Value](#value)         | [Spatial methods](#spatial-methods)                           | [Temporal methods](#temporal-methods)                                        | Double     |
+| [Mean](#mean)                         | [Magnitude](#magnitude) | [Spatial containers](#spatial-containers)                     | [Temporal containers](#temporal-containers)                                  | Array 3D   |
+| [Root mean square](#root-mean-square) | [Euclidean](#euclidean) | [nodal_historical](#spatial-nodal-historical)                 | [nodal_historical_historical](#temporal-nodal-historical-historical)         | Vector     |
+| [Variance](#variance)                 | [Infinity](#infinity)   | [nodal_non_historical](#spatial-nodal-non-historical)         | [nodal_historical_non_historical](#temporal-nodal-historical-non-historical) | Matrix     |
+| [Min](#min)                           | [P-Norm](#p-norm)       | [condition_non_historical](#spatial-condition-non-historical) | [nodal_non_historical](#temporal-nodal-non-historical)                       |            |
+| [Max](#max)                           | [Lpq-Norm](#lpq-norm)   | [element_non_historical](#spatial-element-non-historical)     | [element_non_historical](#temporal-element-non-historical)                   |            |
+| [Median](#median)                     | [Frobenius](#frobenius) | [Spatial statistics process](#spatial-statistics-process)     | [condition_non_historical](#temporal-condition-non-historical)               |            |
+| [Distribution](#distribution)         | [Trace](#trace)         |                                                               | [Temporal statistics process](#temporal-statistics-process)                  |            |
+| [Norm methods](#norm-methods)         | [Index](#index-based)         |                                                               |                                                                              |            |
+|                                       | [Component](#component-based) |                                                               |                                                                              |            |
+
+## JSON Examples
+
+If you prefer to use statistics of a simulation using StatisticsApplication, there is `spatial_statistics_process` for spatial statistics calculations and `temporal_statistics_process` for temporal statistics. These processes can be included via JSON settings under `auxiliary_processes`.
+
+### Spatial statistics process examples
+
+Following example illustrates different methods used in different containers with different norms. `input_variable_settings` holds an array of methods for specified containers, specified norm and specified variables. They can be customized for your requirement. `output_settings` holds information about how the output should be handled.
+
+```json
+{
+                "kratos_module" : "KratosMultiphysics.StatisticsApplication",
+                "python_module" : "spatial_statistics_process",
+                "Parameters" : {
+                    "model_part_name" : "test_model_part",
+                    "input_variable_settings" : [
+                        {
+                            "method_name"    : "sum",
+                            "norm_type"      : "none",
+                            "container"      : "nodal_historical",
+                            "variable_names" : ["PRESSURE", "VELOCITY"],
+                            "method_settings": {}
+                        },
+                        {
+                            "method_name"    : "mean",
+                            "norm_type"      : "none",
+                            "container"      : "nodal_non_historical",
+                            "variable_names" : ["PRESSURE", "VELOCITY"],
+                            "method_settings": {}
+                        },
+                        {
+                            "method_name"    : "variance",
+                            "norm_type"      : "none",
+                            "container"      : "element_non_historical",
+                            "variable_names" : ["PRESSURE", "VELOCITY"],
+                            "method_settings": {}
+                        },
+                        {
+                            "method_name"    : "rootmeansquare",
+                            "norm_type"      : "none",
+                            "container"      : "condition_non_historical",
+                            "variable_names" : ["PRESSURE", "VELOCITY"],
+                            "method_settings": {}
+                        },
+                        {
+                            "method_name"    : "sum",
+                            "norm_type"      : "magnitude",
+                            "container"      : "nodal_historical",
+                            "variable_names" : ["PRESSURE", "VELOCITY", "LOAD_MESHES", "GREEN_LAGRANGE_STRAIN_TENSOR"],
+                            "method_settings": {}
+                        },
+                        {
+                            "method_name"    : "mean",
+                            "norm_type"      : "pnorm_2.5",
+                            "container"      : "nodal_non_historical",
+                            "variable_names" : ["VELOCITY", "LOAD_MESHES", "GREEN_LAGRANGE_STRAIN_TENSOR"],
+                            "method_settings": {}
+                        },
+                        {
+                            "method_name"    : "variance",
+                            "norm_type"      : "component_x",
+                            "container"      : "condition_non_historical",
+                            "variable_names" : ["VELOCITY"],
+                            "method_settings": {}
+                        },
+                        {
+                            "method_name"    : "rootmeansquare",
+                            "norm_type"      : "index_3",
+                            "container"      : "nodal_non_historical",
+                            "variable_names" : ["LOAD_MESHES"],
+                            "method_settings": {}
+                        },
+                        {
+                            "method_name"    : "min",
+                            "norm_type"      : "frobenius",
+                            "container"      : "nodal_non_historical",
+                            "variable_names" : ["GREEN_LAGRANGE_STRAIN_TENSOR"],
+                            "method_settings": {}
+                        }
+                    ],
+                    "output_settings" : {
+                        "output_control_variable": "STEP",
+                        "output_time_interval"   : 1,
+                        "write_kratos_version"   : false,
+                        "write_time_stamp"       : false,
+                        "output_file_settings"   : {
+                            "file_name"  : "<model_part_name>_<container>_<norm_type>_<method_name>.dat",
+                            "output_path": "spatial_statistics_process",
+                            "write_buffer_size" : -1
+                        }
+                    }
+                }
+            }
+```
+
+### Temporal statistics process example
+
+Following is an example on how to use `temporal_statistics_process` in json. The output variables data type should be matched with the input variables order and the data type for `"norm_type" = "none"`. If `"norm_type" != "none"`, then output variables should be `scalars`. If `"container" = "nodal_historical_historical"` is used as the container type, then output variables should be added to `NodalSolutionStepVariables` list in Kratos since this container type outputs temporal statistics variables to nodal historical container. This json settings also can be added to `auxiliary_processes` list.
+
+For details about all the available statistical methods, norm_types, etc, please refer to rest of the `README.md` file.
+
+```json
+        {
+            "kratos_module": "KratosMultiphysics.StatisticsApplication",
+            "python_module": "temporal_statistics_process",
+            "Parameters": {
+                "model_part_name": "FluidModelPart.fluid_computational_model_part",
+                "input_variable_settings": [
+                    {
+                        "method_name": "variance",
+                        "norm_type": "none",
+                        "container": "nodal_historical_non_historical",
+                        "echo_level": 1,
+                        "method_settings": {
+                            "input_variables": [
+                                "VELOCITY",
+                                "PRESSURE"
+                            ],
+                            "output_mean_variables": [
+                                "VECTOR_3D_MEAN",
+                                "SCALAR_MEAN"
+                            ],
+                            "output_variance_variables": [
+                                "VECTOR_3D_VARIANCE",
+                                "SCALAR_VARIANCE"
+                            ]
+                        }
+                    }
+                ],
+                "statistics_start_point_control_variable_name": "TIME",
+                "statistics_start_point_control_value": 2.5
+            }
+        }
+```
+
+## Method definitions
+
+There are two types of methods under each **Spatial** and **Temporal** method groups. They are namely **Value** and **Norm** methods. In these methods, `i` index refers to spatial domain element index, and `k` index refers to time step.
+
+### Value methods
+
+#### Sum
+
+In the case of spatial domain, it adds up all the variable values for a given container and returns summed up value as shown in following equation. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{r}&space;=&space;\sum_{i=1}^N{\underline{x}_i}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{r}&space;=&space;\sum_{i=1}^N{\underline{x}_i}}" title="\color{Black}{\underline{r} = \sum_{i=1}^N{\underline{x}_i}}" /></a>
+
+Following is an example of summation of non historical `VELOCITY` over the whole model part's nodes
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Sum(model_part, Kratos.VELOCITY)
+```
+
+In the case of temporal domain, **Sum** methods is the time integrated quantity for a specific variable. It will be stored each element under user specified variable and a user specified container. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{r}&space;=&space;\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}&space;\quad&space;where&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{r}&space;=&space;\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}&space;\quad&space;where&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" title="\color{Black}{\underline{r} = \sum_{k=1}^{P}{\underline{x}_k\Delta t_k} \quad where \quad \Delta t_k = T_{k} - T_{k-1} \quad \forall T_k \in \left\lbrace T_{initial}, ..., T_{end} \right\rbrace}" /></a>
+
+Following is an example of integration calculation of non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable is same containers `DISPLACEMENT` where integrated value will be stored for each node. The `0` represents echo level for this method object. Blank "" indicates that value method is used.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
+integration_starting_time = 2.0
+sum_method.InitializeStatisticsMethod(integration_starting_time)
+for t in range(3, 6):
+    sum_method.CalculateStatistics()
+```
+
+#### Mean
+
+In the case of spatial domain, it calculates mean of a given variable for a given container and returns it as shown in following equation. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user. (If it has higher dimension than a scalar, mean of each dimension will be calculated seperately resulting with a mean having same dimension as the input dimension)
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{r}&space;=&space;\frac{1}{N}\sum_{i=1}^{N}\underline{x}_i}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{r}&space;=&space;\frac{1}{N}\sum_{i=1}^{N}\underline{x}_i}" title="\color{Black}{\underline{r} = \frac{1}{N}\sum_{i=1}^{N}\underline{x}_i}" /></a>
+
+Following is an example of mean calculation of non historical `VELOCITY` over the whole model part's nodes
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+mean = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Mean(model_part, Kratos.VELOCITY)
+```
+
+In the case of temporal domain, **Mean** methods is the time integrated quantity's mean for a specific variable. It will be stored each element under user specified variable and a user specified container. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user preserving the dimensionality as in the spatial case.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}&space;\quad&space;where&space;\quad&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}&space;\quad&space;where&space;\quad&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" title="\color{Black}{\underline{\bar{x}} = \frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta t_k} \quad where \quad T_{total} = T_{end} - T_{initial} \quad and \quad \Delta t_k = T_{k} - T_{k-1} \quad \forall T_k \in \left\lbrace T_{initial}, ..., T_{end} \right\rbrace}" /></a>
+
+Following is an example of mean calculation of non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable is same containers `VECTOR_3D_MEAN` where mean will be stored for each node. The `0` represents echo level for this method object. Blank "" indicates that value method is used.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+mean_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Mean.Array(model_part, "", Kratos.VELOCITY, 0, KratosStats.VECTOR_3D_MEAN)
+integration_starting_time = 2.0
+mean_method.InitializeStatisticsMethod(integration_starting_time)
+for t in range(3, 6):
+    mean_method.CalculateStatistics()
+```
+
+#### Root mean square
+
+In the case of spatial domain, it calculates root mean square of a given variable for a given container and returns it as shown in following equation. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user. (If it has higher dimension than a scalar, root mean square of each dimension will be calculated seperately resulting with a mean having same dimension as the input dimension)
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{r}&space;=&space;\sqrt{\frac{1}{N}\sum_{i=1}^{N}{\underline{x}^2_i}&space;}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{r}&space;=&space;\sqrt{\frac{1}{N}\sum_{i=1}^{N}{\underline{x}^2_i}&space;}}" title="\color{Black}{\underline{r} = \sqrt{\frac{1}{N}\sum_{i=1}^{N}{\underline{x}^2_i} }}" /></a>
+
+Following is an example of root mean square calculation of non historical `VELOCITY` over the whole model part's nodes
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+rms = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.RootMeanSquare(model_part, Kratos.VELOCITY)
+```
+
+In the case of temporal domain, **Root Mean Square** methods is the time integrated quantity's root mean square for a specific variable. It will be stored each element under user specified variable and a user specified container. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will have the same type as the type of the variable specified by the user preserving the dimensionality as in the spatial case.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{r}&space;=&space;\sqrt{\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k^2\Delta&space;t_k}}&space;\quad&space;where&space;\quad&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{r}&space;=&space;\sqrt{\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k^2\Delta&space;t_k}}&space;\quad&space;where&space;\quad&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" title="\color{Black}{\underline{r} = \sqrt{\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k^2\Delta t_k}} \quad where \quad T_{total} = T_{end} - T_{initial} \quad and \quad \Delta t_k = T_{k} - T_{k-1} \quad \forall T_k \in \left\lbrace T_{initial}, ..., T_{end} \right\rbrace}" /></a>
+
+Following is an example of root mean square calculation of non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable is same containers `VECTOR_3D_MEAN` where root mean square value will be stored for each node. The `0` represents echo level for this method object. Blank "" indicates that value method is used.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+rms_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.RootMeanSquare.Array(model_part, "", Kratos.VELOCITY, 0, KratosStats.VECTOR_3D_MEAN)
+integration_starting_time = 2.0
+rms_method.InitializeStatisticsMethod(integration_starting_time)
+for t in range(3, 6):
+    rms_method.CalculateStatistics()
+```
+
+#### Variance
+
+In the case of spatial domain, it calculates variance of a given variable for a given container and returns mean and variance as shown in following equations. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Results will have the same type as the type of the variable specified by the user. (If it has higher dimension than a scalar, mean of each dimension will be calculated seperately resulting with a mean having same dimension as the input dimension)
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{N}\sum_{i=1}^N{\underline{x}_i}}&space;\\&space;\color{Black}{\underline{v}&space;=&space;\frac{1}{N}\sum_{i=1}^N{\left(\underline{x}_i&space;-&space;\underline{\bar{x}}&space;\right&space;)^2}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{N}\sum_{i=1}^N{\underline{x}_i}}&space;\\&space;\color{Black}{\underline{v}&space;=&space;\frac{1}{N}\sum_{i=1}^N{\left(\underline{x}_i&space;-&space;\underline{\bar{x}}&space;\right&space;)^2}}" title="\color{Black}{\underline{\bar{x}} = \frac{1}{N}\sum_{i=1}^N{\underline{x}_i}} \\ \color{Black}{\underline{v} = \frac{1}{N}\sum_{i=1}^N{\left(\underline{x}_i - \underline{\bar{x}} \right )^2}}" /></a>
+
+Following is an example of variance calculation of non historical `VELOCITY` over the whole model part's nodes
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+mean, variance = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Variance(model_part, Kratos.VELOCITY)
+```
+
+In the case of temporal domain, **Variance** method is the time integrated quantity's variance for a specific variable. Mean and variance will be stored each element under user specified variables and a user specified container. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Results will have the same type as the type of the variable specified by the user preserving the dimensionality as in the spatial case.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}}&space;\\&space;\color{Black}{Var\left(\underline{x}&space;\right&space;)&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\left(\underline{x}_k&space;-&space;\underline{\bar{x}}&space;\right&space;)^2\Delta&space;t_k}}&space;\\&space;\\&space;\color{Black}{&space;\quad&space;where}&space;\\&space;\\&space;\color{Black}{&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{\underline{\bar{x}}&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta&space;t_k}}&space;\\&space;\color{Black}{Var\left(\underline{x}&space;\right&space;)&space;=&space;\frac{1}{T_{total}}\sum_{k=1}^{P}{\left(\underline{x}_k&space;-&space;\underline{\bar{x}}&space;\right&space;)^2\Delta&space;t_k}}&space;\\&space;\\&space;\color{Black}{&space;\quad&space;where}&space;\\&space;\\&space;\color{Black}{&space;T_{total}&space;=&space;T_{end}&space;-&space;T_{initial}&space;\quad&space;and&space;\quad&space;\Delta&space;t_k&space;=&space;T_{k}&space;-&space;T_{k-1}&space;\quad&space;\forall&space;T_k&space;\in&space;\left\lbrace&space;T_{initial},&space;...,&space;T_{end}&space;\right\rbrace}" title="\color{Black}{\underline{\bar{x}} = \frac{1}{T_{total}}\sum_{k=1}^{P}{\underline{x}_k\Delta t_k}} \\ \color{Black}{Var\left(\underline{x} \right ) = \frac{1}{T_{total}}\sum_{k=1}^{P}{\left(\underline{x}_k - \underline{\bar{x}} \right )^2\Delta t_k}} \\ \\ \color{Black}{ \quad where} \\ \\ \color{Black}{ T_{total} = T_{end} - T_{initial} \quad and \quad \Delta t_k = T_{k} - T_{k-1} \quad \forall T_k \in \left\lbrace T_{initial}, ..., T_{end} \right\rbrace}" /></a>
+
+Following is an example of root mean square calculation of non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable `VECTOR_3D_MEAN` will store mean and `VECTOR_3D_VARIANCE` will store variance in same container for each node. The `0` represents echo level for this method object. Blank "" indicates that value method is used.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+variance_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Variance.Array(model_part, "", Kratos.VELOCITY, 0, KratosStats.VECTOR_3D_MEAN, KratosStats.VECTOR_3D_VARIANCE)
+integration_starting_time = 2.0
+variance_method.InitializeStatisticsMethod(integration_starting_time)
+for t in range(3, 6):
+    variance_method.CalculateStatistics()
+```
+
+#### Min
+
+In the case of spatial domain, it returns minimum of a given variable's norm for a given container, and the corresponding items id. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Results will be double and integer, irrespective of the input type, since higher dimensional variable types will be reduced to scalars by the use of norms.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{v&space;=&space;\min_{\underline{x}_i&space;\in&space;\mathbf{T}}&space;|\underline{x}_i|}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{v&space;=&space;\min_{\underline{x}_i&space;\in&space;\mathbf{T}}&space;|\underline{x}_i|}" title="\color{Black}{v = \min_{\underline{x}_i \in \mathbf{T}} |\underline{x}_i|}" /></a>
+
+Following is an example of min method of non historical `VELOCITY`'s magnitude over the whole model part's nodes. It returns a tuple, first argument being the minimum, and the second argument being the id of the node where the minimum is found.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+min_value, min_id = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Min(model_part, Kratos.VELOCITY, "magnitude")
+```
+
+In the case of temporal domain, **Min** method returns minimum value in the temporal domain, and the time minimum is found. Minimum and its occurring time will be stored each element under user specified variables and a user specified container. x<sub>k</sub> is the k<sup>th</sup> time step element's variable value of the corresponding container. Results will have the same type as the type of the variable specified by the user preserving the dimensionality as in the spatial case.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{v&space;=&space;\min_{\underline{x}_k&space;\in&space;\mathbf{T}}&space;|\underline{x}_k|}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{v&space;=&space;\min_{\underline{x}_k&space;\in&space;\mathbf{T}}&space;|\underline{x}_k|}" title="\color{Black}{v = \min_{\underline{x}_k \in \mathbf{T}} |\underline{x}_k|}" /></a>
+
+Following is an example of min method in non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable `VECTOR_3D_NORM` will store minimum and `TIME` will store the time minimum occured for each node. The `0` represents echo level for this method object. "magnitude" indicates that magnitude norm is used.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+min_method = KratosStats.TemporalMethods.NonHistorical.Nodes.NormMethods.Min.Array(model_part, "magnitude", Kratos.VELOCITY, 0, KratosStats.VECTOR_3D_NORM, Kratos.TIME)
+integration_starting_time = 2.0
+min_method.InitializeStatisticsMethod(integration_starting_time)
+for t in range(3, 6):
+    min_method.CalculateStatistics()
+```
+
+#### Max
+
+In the case of spatial domain, it returns maximum of a given variable's norm for a given container, and the corresponding items id. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Results will be double and integer, irrespective of the input type, since higher dimensional variable types will be reduced to scalars by the use of norms.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{v&space;=&space;\max_{\underline{x}_i&space;\in&space;\Omega}&space;|\underline{x}_i|}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{v&space;=&space;\max_{\underline{x}_i&space;\in&space;\Omega}&space;|\underline{x}_i|}" title="\color{Black}{v = \max_{\underline{x}_i \in \Omega} |\underline{x}_i|}" /></a>
+
+Following is an example of max method of non historical `VELOCITY`'s magnitude over the whole model part's nodes. It returns a tuple, first argument being the maximum, and the second argument being the id of the node where the maximum is found.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+max_value, max_id = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Max(model_part, Kratos.VELOCITY, "magnitude")
+```
+
+In the case of temporal domain, **Max** method returns maximum value in the temporal domain, and the time maximum is found. Maximum and its occurring time will be stored each element under user specified variables and a user specified container. x<sub>k</sub> is the k<sup>th</sup> time step element's variable value of the corresponding container. Results will have the same type as the type of the variable specified by the user preserving the dimensionality as in the spatial case.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex=\color{Black}{v&space;=&space;\max_{\underline{x}_k&space;\in&space;\mathbf{T}}&space;|\underline{x}_k|}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?\color{Black}{v&space;=&space;\max_{\underline{x}_k&space;\in&space;\mathbf{T}}&space;|\underline{x}_k|}" title="\color{Black}{v = \max_{\underline{x}_k \in \mathbf{T}} |\underline{x}_k|}" /></a>
+
+Following is an example of max method in non historical velocity. Input variable is node's non-historical container's `VELOCITY` and output variable `VECTOR_3D_NORM` will store maximum and `TIME` will store the time maximum occured for each node. The `0` represents echo level for this method object. "magnitude" indicates that magnitude norm is used.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+max_method = KratosStats.TemporalMethods.NonHistorical.Nodes.NormMethods.Max.Array(model_part, "magnitude", Kratos.VELOCITY, 0, KratosStats.VECTOR_3D_NORM, Kratos.TIME)
+integration_starting_time = 2.0
+max_method.InitializeStatisticsMethod(integration_starting_time)
+for t in range(3, 6):
+    max_method.CalculateStatistics()
+```
+
+#### Median
+
+Median returns the median value in spatial domain of a given variable's norm for a given container. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Results will be double value type, irrespective of the input type, since higher dimensional variable types will be reduced to scalars by the use of norms.
+
+Following is an example of median method of non historical `VELOCITY`'s magnitude over the whole model part's nodes. It returns a double which is the median.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+median_value = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Median(model_part, Kratos.VELOCITY, "magnitude")
+```
+
+#### Distribution
+
+Distribution methods calculates distribution of a given variable with respect to given norm in a given container in spatial domain. x<sub>i</sub> is the i<sup>th</sup> element's variable value of the corresponding container. Result will be a tuple with followings in the same order:
+
+1. min in the domain or user specified min value
+2. max in the domain or user specified min value
+3. group limits of the distribution (only upper limit) (double array)
+4. number of occurences of items within each group (int array)
+5. percentage distribution of number of occurences of items within each group (double array)
+6. Each group's seperate means
+7. Eash group's seperate variances
+
+This method requires followings as the parameters as a object of Kratos.Parameters, if nothing is provided, then followings are assumed as defaults.
+
+```json
+{
+    "number_of_value_groups" : 10,
+    "min_value"              : "min",
+    "max_value"              : "max"
+}
+```
+
+In here, `"min_value"` can either be `"min"` or a `double` value. In the case of a double, it will be used as the minimum when creating groups to identify distribution. `"max_value"` also can either be `"max"` of `double` value, which will determine the maximum value when creating the groups. This will create 2 additional groups to represent values below the specified `"min_value"` and `"max_value"` apart from the `"number_of_value_groups"` specified by the user.
+
+Following is an example of median method of non historical `VELOCITY`'s magnitude over the whole model part's nodes.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+min_value, max_value, group_upper_values, group_histogram, group_percentage_distribution, group_means, group_variances = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Distribution(model_part, Kratos.VELOCITY, "magnitude")
+```
+
+### Norm methods
+
+All of the value methods mentioned before supports norm version of it, in these methods, higher dimensional values are transformed in to scalar values by a use specified norm, and then statistics are calculated based on the chosen method. Supported norm types may differ based on the variable data type being used. There are few methods, which only supports norm methods. Following table summarize availability of value and norm methods.
+
+| Statistical Methods                   | Value Method | Norm Method |
+|---------------------------------------|--------------|-------------|
+| [Sum](#sum)                           | [x]          | [x]         |
+| [Mean](#mean)                         | [x]          | [x]         |
+| [Root mean square](#root-mean-square) | [x]          | [x]         |
+| [Variance](#variance)                 | [x]          | [x]         |
+| [Min](#min)                           |              | [x]         |
+| [Max](#max)                           |              | [x]         |
+| [Median](#median)                     |              | [x]         |
+| [Distribution](#distribution)         |              | [x]         |
+
+Following example shows variance method, under **value** category and **norm** category for nodal non historical velocity. Norm method uses `"magnitude"` as the norm to reduce `VELOCITY` to a scalar value. `value_mean` and `value_variance` will be of `Array 3D` type, whereas `norm_mean` and `norm_variance` will be of `Double` type.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+value_mean, value_variance = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Variance(model_part, Kratos.VELOCITY)
+norm_mean, norm_variance = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Variance(model_part, Kratos.VELOCITY, "magnitude")
+```
+
+## Norm definitions
+
+Few different norms are predefined in this application. Following table summarize
+
+|                               | Double | Array 3D | Vector | Matrix |
+|-------------------------------|--------|----------|--------|--------|
+| [Value](#value)               | [x]    |          |        |        |
+| [Magnitude](#magnitude)       | [x]    | [x]      | [x]    | [x]    |
+| [Euclidean](#euclidean)       |        | [x]      | [x]    |        |
+| [Infinity](#infinity)         |        | [x]      | [x]    | [x]    |
+| [P-Norm](#p-norm)             |        | [x]      | [x]    | [x]    |
+| [Lpq-Norm](#lpq-norm)         |        |          |        | [x]    |
+| [Frobenius](#frobenius)       |        |          |        | [x]    |
+| [Trace](#trace)               |        |          |        | [x]    |
+| [Index](#index-based)         |        |          | [x]    | [x]    |
+| [Component](#component-based) |        | [x]      |        |        |
+
+### Value
+
+This returns the exact value. Only available for `Double` type variables.
+
+### Magnitude
+
+This returns the second norm of the variable.
+
+1. For a `Double` type, it returns the absolute value.
+2. For a `Array 3D` type, it returns the magnitude of the 3D vector.
+3. For a `Vector` type, it returns root square sum of the vector.
+4. For a `Matrix` type, it returns the [frobenius](#frobenius) norm.
+
+### Euclidean
+
+This again returns the second norm of the variable for following variable types.
+
+1. For a `Array 3D` type, it returns the magnitude of the 3D vector.
+2. For a `Vector` type, it returns root square sum of the vector.
+
+### Frobenius
+
+This is only available for `Matrix` data type variables only. Following equation illustrates the norm, where `A` is the matrix and a<sub>ij</sub> is the i<sup>th</sup> row, j<sup>th</sup> column value.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||A||_F&space;=&space;\sqrt{\sum_i&space;{\sum_j{||a_{ij}||^2}}}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||A||_F&space;=&space;\sqrt{\sum_i&space;{\sum_j{||a_{ij}||^2}}}}" title="{\color{Black} ||A||_F = \sqrt{\sum_i {\sum_j{||a_{ij}||^2}}}}" /></a>
+
+### Infinity
+
+This is infinity (i.e. max norm) which is available for `Array 3D`, `Vector` and `Matrix` type.
+For an `Array 3D` variable following equation is used.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{V}||_\infty&space;=&space;\max\left&space;\lbrace&space;{|V_X|,&space;|V_Y|,&space;|V_Z|}\right&space;\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{V}||_\infty&space;=&space;\max\left&space;\lbrace&space;{|V_X|,&space;|V_Y|,&space;|V_Z|}\right&space;\rbrace}" title="{\color{Black} ||\underline{V}||_\infty = \max\left \lbrace {|V_X|, |V_Y|, |V_Z|}\right \rbrace}" /></a>
+
+For a `Vector` variable following equation is used.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{V}||_\infty&space;=&space;\max\left&space;\lbrace&space;{|V_0|,&space;|V_1|,&space;|V_2|,...,{V_{n-1}}}\right&space;\rbrace}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{V}||_\infty&space;=&space;\max\left&space;\lbrace&space;{|V_0|,&space;|V_1|,&space;|V_2|,...,{V_{n-1}}}\right&space;\rbrace}" title="{\color{Black} ||\underline{V}||_\infty = \max\left \lbrace {|V_0|, |V_1|, |V_2|,...,{V_{n-1}}}\right \rbrace}" /></a>
+
+For a `Matrix` variable following equation is used.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{A}||_\infty&space;=&space;\max_{0&space;\leq&space;i&space;<&space;n}\left(&space;\sum_{j=0}^{n-1}&space;|a_{ij}|\right&space;)}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{A}||_\infty&space;=&space;\max_{0&space;\leq&space;i&space;<&space;n}\left(&space;\sum_{j=0}^{n-1}&space;|a_{ij}|\right&space;)}" title="{\color{Black} ||\underline{A}||_\infty = \max_{0 \leq i < n}\left( \sum_{j=0}^{n-1} |a_{ij}|\right )}" /></a>
+
+### Trace
+
+Trace is only for `Matrix` type variables. If the given matrix is not squre, an error is thrown.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{A}||_{trace}&space;=&space;\sum_{i=0}^{n-1}a_{ij}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{A}||_{trace}&space;=&space;\sum_{i=0}^{n-1}a_{ij}}" title="{\color{Black} ||\underline{A}||_{trace} = \sum_{i=0}^{n-1}a_{ij}}" /></a>
+
+### P norm
+
+P norm is applicable for `Array 3D`, `Vector` and `Matrix` variables. The p-norm is used as `pnorm_p` where, `p` represents the value to be used as `p` in the p-norm equation given below. `p` should be greater than or equal to 1.0.
+
+For `Array 3D` and `Vector`:
+
+<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{V}||_{p}&space;=&space;\left(\sum_{i=0}^{n-1}|v_{i}|^p&space;\right&space;)^{1/p}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{V}||_{p}&space;=&space;\left(\sum_{i=0}^{n-1}|v_{i}|^p&space;\right&space;)^{1/p}}" title="{\color{Black} ||\underline{V}||_{p} = \left(\sum_{i=0}^{n-1}|v_{i}|^p \right )^{1/p}}" /></a>
+
+For `Matrix`:
+
+<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{A}||_{p}&space;=&space;\left(\sum_{i=0}^{n-1}\sum_{j=0}^{n-1}|a_{ij}|^p&space;\right&space;)^{1/p}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{A}||_{p}&space;=&space;\left(\sum_{i=0}^{n-1}\sum_{j=0}^{n-1}|a_{ij}|^p&space;\right&space;)^{1/p}}" title="{\color{Black} ||\underline{A}||_{p} = \left(\sum_{i=0}^{n-1}\sum_{j=0}^{n-1}|a_{ij}|^p \right )^{1/p}}" /></a>
+
+### Lpq norm
+
+This norm is only applicable to `Matrix` type variables.
+
+<a href="https://www.codecogs.com/eqnedit.php?latex={\color{Black}&space;||\underline{A}||_{lpq}&space;=&space;\left(\sum_{j=0}^{n-1}\left(\sum_{i=0}^{n-1}|a_{ij}|^p&space;\right&space;)^{q/p}&space;\right&space;)^{1/q}}" target="_blank"><img src="https://latex.codecogs.com/svg.latex?{\color{Black}&space;||\underline{A}||_{lpq}&space;=&space;\left(\sum_{j=0}^{n-1}\left(\sum_{i=0}^{n-1}|a_{ij}|^p&space;\right&space;)^{q/p}&space;\right&space;)^{1/q}}" title="{\color{Black} ||\underline{A}||_{lpq} = \left(\sum_{j=0}^{n-1}\left(\sum_{i=0}^{n-1}|a_{ij}|^p \right )^{q/p} \right )^{1/q}}" /></a>
+
+### Index based
+
+Index based norms are available for both `Vector` and `Matrix` based variable types. `index_i` is used for `Vector` variables, where `i` represents the index of the vector to be used as the scalar representing a corresponding vector. `index_(i,j)` is used for `Matrix` variables, where `i` represents the row index and `j` represents the column index of the matrix value which to be used as the scalar representation of the given matrix.
+
+### Component based
+
+Component based norms are available only for `Array 3D` type variables. `component_x` represents the `x` component of 3D variable, `component_y` represents `y` component, `component_z` represents the `z` component.
+
+
+## Spatial methods
+
+All the spatial statistical methods can be found in the `SpatialMethods` submodule. `ValueMethods` container will contain all available spatial value methods, and `NormMethods` container will contain all available norm methods.
+
+Following example illustrates all the available value methods executed on nodal non historical variable velocity.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_value = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Sum(model_part, Kratos.VELOCITY)
+mean_value = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Mean(model_part, Kratos.VELOCITY)
+rms_value = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.RootMeanSquare(model_part, Kratos.VELOCITY)
+mean_value, variance_value = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Variance(model_part, Kratos.VELOCITY)
+```
+
+Following example illustrates all the available norm methods executed on nodal non historical variable velocity's magnitude.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_norm = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Sum(model_part, Kratos.VELOCITY, "magnitude")
+mean_norm = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Mean(model_part, Kratos.VELOCITY, "magnitude")
+rms_norm = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.RootMeanSquare(model_part, Kratos.VELOCITY, "magnitude")
+mean_norm, variance_norm = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Variance(model_part, Kratos.VELOCITY, "magnitude")
+min_norm, min_norm_id = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Min(model_part, Kratos.VELOCITY, "magnitude")
+max_norm, max_norm_id = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Max(model_part, Kratos.VELOCITY, "magnitude")
+min_norm, max_norm, group_upper_norms, group_histogram, group_percentage_distribution = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Distribution(model_part, Kratos.VELOCITY, "magnitude")
+```
+
+### Spatial containers
+
+Four different types of containers are supported for spatial methods.
+
+1. [nodal_historical](#spatial-nodal-historical)
+2. [nodal_non_historical](#spatial-nodal-non-historical)
+3. [condition_non_historical](#spatial-condition-non-historical)
+4. [element_non_historical](#spatial-element-non-historical)
+
+#### Spatial nodal historical
+
+Nodal historical containers methods can be accessed through `Historical` submodule in `SpatialMethods`. This calculates chosen statistics of the variable in the nodal historical data. Following example illustrates use of value and norm methods.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+model_part.AddNodalSolutionStepVariable(Kratos.VELOCITY)
+sum_value = KratosStats.SpatialMethods.Historical.ValueMethods.Sum(model_part, Kratos.VELOCITY)
+sum_norm = KratosStats.SpatialMethods.Historical.NormMethods.Sum(model_part, Kratos.VELOCITY, "magnitude")
+```
+
+#### Spatial nodal non historical
+
+Nodal non historical containers methods can be accessed through `NonHistorical.Nodes` submodule in `SpatialMethods`. This calculates chosen statistics of the variable in the nodal non historical data. Following example illustrates use of value and norm methods.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_value = KratosStats.SpatialMethods.NonHistorical.Nodes.ValueMethods.Sum(model_part, Kratos.VELOCITY)
+sum_norm = KratosStats.SpatialMethods.NonHistorical.Nodes.NormMethods.Sum(model_part, Kratos.VELOCITY, "magnitude")
+```
+
+#### Spatial condition non historical
+
+Condition non historical containers methods can be accessed through `NonHistorical.Conditions` submodule in `SpatialMethods`. This calculates chosen statistics of the variable in the condition non historical data. Following example illustrates use of value and norm methods.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_value = KratosStats.SpatialMethods.NonHistorical.Conditions.ValueMethods.Sum(model_part, Kratos.VELOCITY)
+sum_norm = KratosStats.SpatialMethods.NonHistorical.Conditions.NormMethods.Sum(model_part, Kratos.VELOCITY, "magnitude")
+```
+
+#### Spatial element non historical
+
+Element non historical containers methods can be accessed through `NonHistorical.Elements` submodule in `SpatialMethods`. This calculates chosen statistics of the variable in the element non historical data. Following example illustrates use of value and norm methods.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_value = KratosStats.SpatialMethods.NonHistorical.Elements.ValueMethods.Sum(model_part, Kratos.VELOCITY)
+sum_norm = KratosStats.SpatialMethods.NonHistorical.Elements.NormMethods.Sum(model_part, Kratos.VELOCITY, "magnitude")
+```
+
+### Spatial statistics process
+
+This is a seperate process, which can be included in the json file as an auxiliary process. Followings are the defaults used in this process.
+
+```json
+{
+    "model_part_name" : "PLEASE_SPECIFY_MODEL_PART_NAME",
+    "input_variable_settings" : [
+        {
+            "method_name"    : "sum",
+            "norm_type"      : "none",
+            "container"      : "nodal_historical",
+            "variable_names" : [],
+            "method_settings": {}
+        }
+    ],
+    "output_settings" : {
+        "output_control_variable": "STEP",
+        "output_time_interval"   : 1,
+        "write_kratos_version"   : true,
+        "write_time_stamp"       : true,
+        "output_file_settings"   : {
+            "file_name"  : "<model_part_name>_<container>_<norm_type>_<method_name>.dat",
+            "output_path": "spatial_statistics_output",
+            "write_buffer_size" : -1
+        }
+    }
+}
+```
+
+`model_part_name` indicates which model part to be operated on for statistics calculation. `input_variable_settings` contains list of statistics and/or norm methods along with their acting containers of the model part. `method_name` is the statistics method name (always everything is in lower case). `norm_type` is the applied norm, `none` means, value methods are used, otherwise specified norm is used. `container` is the [container](#spatial-method-containers) to be specified for statistical value calculation. `method_settings` is used to pass additional information required by statistics method such as in [Distribution](#distribution) method. Output is written to a file in the format given at `file_name`, under the folder `folder_name`. This process can be used, if someone prefers not to modify their python scripts to calculate statistics as mentioned in the previous sections
+
+## Temporal methods
+
+All the temporal methods are available through `TemporalMethods` submodule under `StatisticsApplication`. In the case of temporal methods, seperate objects needs to be created for each input variable for different type of variables as shown in following example for nodal non historical data container value methods.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_double_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Double(model_part, "", Kratos.PRESSURE, 0, Kratos.DENSITY)
+sum_array_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
+sum_vector_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Vector(model_part, "", Kratos.LOAD_MESHES, 0, Kratos.MATERIAL_PARAMETERS)
+sum_matrix_method = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Matrix(model_part, "", Kratos.GREEN_LAGRANGE_STRAIN_TENSOR, 0, Kratos.CAUCHY_STRESS_TENSOR)
+```
+
+In order to remove the hassle of using different names (such as `Double`, `Array`...), one can get the advantage of common methods available in each of the containers. Following example will create the same objects as in the previous example in one go using simplified sum method.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+params = Kratos.Parameters(r"""
+{
+    "input_variables" : ["PRESSURE", "VELOCITY", "LOAD_MESHES", "GREEN_LAGRANGE_STRAIN_TENSOR"],
+    "output_variables" : ["DENSITY", "DISPLACEMENT", "MATERIAL_PARAMETERS", "CAUCHY_STRESS_TENSOR"]
+}""")
+sum_methods = KratosStats.TemporalMethods.NonHistorical.Nodes.Sum(model_part, "none", 0, params)
+```
+
+For **Sum**, **Mean**, **RootMeanSquare** methods, above `Kratos.Parameters` object keys will remain the same. But for **Variance** method following `json` parameters are used.
+
+```json
+{
+    "input_variables"           : [],
+    "output_mean_variables"     : [],
+    "output_variance_variables" : []
+}
+```
+
+When using these simplified, one needs to take care of compatibility of input and output variables depending on the method and norm type, otherwise runtime errors will be thrown.
+
+### Temporal containers
+
+In the temporal domain, there are five different containers available for user to calculate temporal statistics. They are,
+
+1. [nodal_historical_historical](#temporal-nodal-historical-historical)
+2. [nodal_historical_non_historical](#temporal-nodal-historical-non-historical)
+3. [nodal_non_historical](#temporal-nodal-non-historical)
+4. [condition_non_historical](#temporal-condition-non-historical)
+5. [element_non_historical](#temporal-element-non-historical)
+
+#### Temporal nodal historical historical
+
+In this container, statistics are calculated on user specified variables in the nodal historical container and, output is also written to the nodal historical container. Example is given below.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_value = KratosStats.TemporalMethods.Historical.HistoricalOutput.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
+sum_norm = KratosStats.TemporalMethods.Historical.HistoricalOutput.NormMethods.Sum.Array(model_part, "magnitude", Kratos.VELOCITY, 0, Kratos.DENSITY)
+```
+
+#### Temporal nodal historical non historical
+
+In this container, statistics are calculated on user specified variables in the nodal historical container and, output is also written to the nodal non historical container. Example is given below.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_value = KratosStats.TemporalMethods.Historical.NonHistoricalOutput.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
+sum_norm = KratosStats.TemporalMethods.Historical.NonHistoricalOutput.NormMethods.Sum.Array(model_part, "magnitude", Kratos.VELOCITY, 0, Kratos.DENSITY)
+```
+
+#### Temporal nodal non historical
+
+In this container, statistics are calculated on user specified variables in the nodal non historical container and, output is also written to the nodal non historical container. Example is given below.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_value = KratosStats.TemporalMethods.NonHistorical.Nodes.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
+sum_norm = KratosStats.TemporalMethods.NonHistorical.Nodes.NormMethods.Sum.Array(model_part, "magnitude", Kratos.VELOCITY, 0, Kratos.DENSITY)
+```
+
+#### Temporal condition non historical
+
+In this container, statistics are calculated on user specified variables in the condition non historical container and, output is also written to the condition non historical container. Example is given below.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_value = KratosStats.TemporalMethods.NonHistorical.Conditions.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
+sum_norm = KratosStats.TemporalMethods.NonHistorical.Conditions.NormMethods.Sum.Array(model_part, "magnitude", Kratos.VELOCITY, 0, Kratos.DENSITY)
+```
+
+#### Temporal element non historical
+
+In this container, statistics are calculated on user specified variables in the element non historical container and, output is also written to the element non historical container. Example is given below.
+
+```python
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.StatisticsApplication as KratosStats
+model = Kratos.Model()
+model_part = model.CreateModelPart("test_model_part")
+sum_value = KratosStats.TemporalMethods.NonHistorical.Elements.ValueMethods.Sum.Array(model_part, "", Kratos.VELOCITY, 0, Kratos.DISPLACEMENT)
+sum_norm = KratosStats.TemporalMethods.NonHistorical.Elements.NormMethods.Sum.Array(model_part, "magnitude", Kratos.VELOCITY, 0, Kratos.DENSITY)
+```
+
+### Temporal statistics process
+
+This is a seperate process, which can be included in the json file as an auxiliary process. Followings are the defaults used in this process.
+
+```json
+    "model_part_name" : "PLEASE_SPECIFY_MODEL_PART_NAME",
+    "input_variable_settings" : [
+        {
+            "method_name"     : "sum",
+            "norm_type"       : "none",
+            "container"       : "nodal_historical_non_historical",
+            "echo_level"      : 0,
+            "method_settings" : {}
+        }
+    ],
+    "echo_level" : 0,
+    "statistics_start_point_control_variable_name" : "TIME",
+    "statistics_start_point_control_value"         : 0.0
+```
+
+`model_part_name` is the model part which all of the mentioned statistics will be calculated. `input_variable_settings` contains list of statistical methods, their norms and container combinations where statistics will be calculated. under each `input_variable_settings_block`, `method_name` is the statistics method, `norm_type` is the norm type (`"none"` for value methods, other wise norms are used), `container` to tell from which container to read/write, `method_settings` to specifiy input/output variables for the method. Apart from that, there are few global settings. `statistics_start_point_control_variable_name` is the temporal statistics calculation start control variable name. This variable should be present in the model_part specified in order to calculate temporal statistics. Statistics calculation will start when this variable's value passes user specified value in `statistics_start_point_control_value`.
```

## Comparing `KratosStatisticsApplication-9.4.5.dist-info/RECORD` & `KratosStatisticsApplication-9.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-KratosMultiphysics/.libs/KratosStatisticsApplication.pyd,sha256=1gBckEZtvX0H1rEspDh4suEv-6qebyec3-sH62NVdZY,3240448
-KratosMultiphysics/.libs/KratosStatisticsCore.dll,sha256=hPQxS-agcmgjxJqANYKHxwQD_HNNsXVRAa6SEohAj_Y,493568
-KratosMultiphysics/.libs/KratosStatisticsCore.lib,sha256=qGhR10HoEOEMwhIk-uEaLeP0XHQH3e7zIxJbrRspSJ4,81868
-KratosMultiphysics/StatisticsApplication/__init__.py,sha256=Ui40SBLib0u0X-O1D7_sgjx7ibVhH7gF0GhGTK1h26M,283
-KratosMultiphysics/StatisticsApplication/method_utilities.py,sha256=l2l60DbZ5un0YOYr1k06BjUNDtS9uHRowzekmyOLK6c,1184
-KratosMultiphysics/StatisticsApplication/spatial_statistics_process.py,sha256=t84V9DXiPfoCpgUdOZ0X__RhcHgPUEv3chUhDwYOeBw,17616
-KratosMultiphysics/StatisticsApplication/spatial_utilities.py,sha256=gUDIx5udOJxCGjxkNBHPSg0NlhSkCbJjI6TWBk-Nlcw,10543
-KratosMultiphysics/StatisticsApplication/temporal_statistics_process.py,sha256=AwP06w4wltgLe8k79vOv2t0f6h1OGjWDcROUtJ6InZo,6063
-KratosMultiphysics/StatisticsApplication/temporal_utilities.py,sha256=jQOshULSIEg9AFPlTm7-lJx0wRCmmbojaqdsm6YAETA,2316
-KratosMultiphysics/StatisticsApplication/test_utilities.py,sha256=00qsmDj7JdqEqG7yZ_5rVdZ3MNcwOYbvrQ-qv82VsYg,7265
-KratosStatisticsApplication-9.4.5.dist-info/METADATA,sha256=NjNTASb0_0hs8U2qo-8Q1VO-zku5Gh26NZEjE8lYrko,63056
-KratosStatisticsApplication-9.4.5.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
-KratosStatisticsApplication-9.4.5.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
-KratosStatisticsApplication-9.4.5.dist-info/RECORD,,
+KratosStatisticsApplication.libs/libKratosStatisticsCore-e894e91a.so,sha256=EuSL_nOk0aJZ9AgiMBWknFC8otkuhpFQv4TustPStFE,2844569
+KratosMultiphysics/.libs/libKratosStatisticsCore.so,sha256=O4bbDnvC4iyDwAdNgRjsFqyHZrg_VVfgCKmCNCfqV7Y,2636313
+KratosMultiphysics/.libs/KratosStatisticsApplication.cpython-39-x86_64-linux-gnu.so,sha256=gyp2fYKT3ByACV9wjmczdE8uBZD3MjGwgU9SzYnm6Zo,6628217
+KratosMultiphysics/StatisticsApplication/method_utilities.py,sha256=ZWXBjY4A4fZuT7F4la4X_FPZdnt9tBhiqWQl4ZVyEiQ,1156
+KratosMultiphysics/StatisticsApplication/test_utilities.py,sha256=vZOwU7x-vsT8pf5hQNAejJl3zezl5TTBnxsAy82C2C0,7101
+KratosMultiphysics/StatisticsApplication/temporal_statistics_process.py,sha256=B0i6Ox_G7aMXgknenEHrrwdGdFPyRU--KtNq9apj66k,5943
+KratosMultiphysics/StatisticsApplication/temporal_utilities.py,sha256=aHZ_j4MUste1iO06oFQzgj8cQTDVKFMoYJj2WTutrVw,2254
+KratosMultiphysics/StatisticsApplication/spatial_utilities.py,sha256=LKhMVlaXB6TyOjWOr8RWWPIoocjohhCXRHyCd7YtaD8,10317
+KratosMultiphysics/StatisticsApplication/spatial_statistics_process.py,sha256=I_xjwEBdjx6dIiAZZNzUUWCToyx3FWG1QkZ_fa__81Q,17296
+KratosMultiphysics/StatisticsApplication/__init__.py,sha256=RIbWPazF8jYx_knfD19yCW8tBUwhQ5o9MhKKhjD-q80,276
+KratosStatisticsApplication-9.5.dist-info/METADATA,sha256=1cqV7_bfTGrv4gGyP-k0ovTewXFE5EiZgHCFUVZYP-g,62229
+KratosStatisticsApplication-9.5.dist-info/WHEEL,sha256=rY0Y6THYM7EImsHfF-zs67o8pQciAsMw9_YuSvftjrQ,148
+KratosStatisticsApplication-9.5.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
+KratosStatisticsApplication-9.5.dist-info/RECORD,,
```

