# Comparing `tmp/KratosMeshingApplication-9.4.6-cp39-cp39-win_amd64.whl.zip` & `tmp/KratosMeshingApplication-9.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,336 +1,824 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   1243346 (000000000012F8D2h)
-  Actual end-cent-dir record offset:       1243324 (000000000012F8BCh)
-  Expected end-cent-dir record offset:     1243324 (000000000012F8BCh)
+  Zip archive file size:                   6215473 (00000000005ED731h)
+  Actual end-cent-dir record offset:       6215451 (00000000005ED71Bh)
+  Expected end-cent-dir record offset:     6215451 (00000000005ED71Bh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 11 entries.
-  The central directory is 1095 (0000000000000447h) bytes long,
+  central directory contains 22 entries.
+  The central directory is 2695 (0000000000000A87h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 1242229 (000000000012F475h).
+  is 6212756 (00000000005ECC94h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosMeshingApplication.pyd
+  KratosMeshingApplication-9.5.dist-info/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:22
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:21 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:21 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             39 characters
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
+Central directory entry #2:
+---------------------------
+
+  KratosMeshingApplication-9.5.dist-info/METADATA
+
+  offset of local header from start of archive:   97
+                                                  (0000000000000061h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         e41fe821
+  compressed size:                                2283 bytes
+  uncompressed size:                              6024 bytes
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
+Central directory entry #3:
+---------------------------
+
+  KratosMeshingApplication-9.5.dist-info/WHEEL
+
+  offset of local header from start of archive:   2485
+                                                  (00000000000009B5h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         90d34e0d
+  compressed size:                                116 bytes
+  uncompressed size:                              148 bytes
+  length of filename:                             44 characters
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
+Central directory entry #4:
+---------------------------
+
+  KratosMeshingApplication-9.5.dist-info/top_level.txt
+
+  offset of local header from start of archive:   2703
+                                                  (0000000000000A8Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         f32d789f
+  compressed size:                                19 bytes
+  uncompressed size:                              19 bytes
+  length of filename:                             52 characters
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
+Central directory entry #5:
+---------------------------
+
+  KratosMeshingApplication-9.5.dist-info/RECORD
+
+  offset of local header from start of archive:   2832
+                                                  (0000000000000B10h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         b7d60006
-  compressed size:                                613795 bytes
-  uncompressed size:                              1717760 bytes
-  length of filename:                             53 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:22
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:21 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:21 UTC
+  32-bit CRC value (hex):                         fd981e9a
+  compressed size:                                974 bytes
+  uncompressed size:                              1954 bytes
+  length of filename:                             45 characters
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
+Central directory entry #6:
+---------------------------
+
+  KratosMeshingApplication.libs/
+
+  offset of local header from start of archive:   3909
+                                                  (0000000000000F45h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:22
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:21 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:21 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             30 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
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
+Central directory entry #7:
+---------------------------
+
+  KratosMeshingApplication.libs/libmmg-ef3d646f.so.5.5.1
+
+  offset of local header from start of archive:   3997
+                                                  (0000000000000F9Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         c8bd79bc
+  compressed size:                                813702 bytes
+  uncompressed size:                              1923617 bytes
+  length of filename:                             54 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
-Central directory entry #2:
+Central directory entry #8:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosMeshingCore.dll
+  KratosMeshingApplication.libs/libmmgs-a9c9f31a.so.5.5.1
 
-  offset of local header from start of archive:   613878
-                                                  (0000000000095DF6h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   817811
+                                                  (00000000000C7A93h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         c201ab19
-  compressed size:                                598012 bytes
-  uncompressed size:                              1657344 bytes
-  length of filename:                             46 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         bb008911
+  compressed size:                                237204 bytes
+  uncompressed size:                              578073 bytes
+  length of filename:                             55 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
-Central directory entry #3:
+Central directory entry #9:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosMeshingCore.lib
+  KratosMeshingApplication.libs/libmmg2d-808e00cf.so.5.5.1
 
-  offset of local header from start of archive:   1211966
-                                                  (0000000000127E3Eh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1055128
+                                                  (0000000000101998h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         63da36f3
-  compressed size:                                13984 bytes
-  uncompressed size:                              138008 bytes
-  length of filename:                             46 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         2397621a
+  compressed size:                                261506 bytes
+  uncompressed size:                              634793 bytes
+  length of filename:                             56 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
-Central directory entry #4:
+Central directory entry #10:
 ---------------------------
 
-  KratosMultiphysics/MeshingApplication/__init__.py
+  KratosMeshingApplication.libs/libmmg3d-48d89c48.so.5.5.1
 
-  offset of local header from start of archive:   1226026
-                                                  (000000000012B52Ah) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1316748
+                                                  (000000000014178Ch) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         a1095b4a
-  compressed size:                                179 bytes
-  uncompressed size:                              407 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         1f885012
+  compressed size:                                514481 bytes
+  uncompressed size:                              1187849 bytes
+  length of filename:                             56 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
-Central directory entry #5:
+Central directory entry #11:
 ---------------------------
 
-  KratosMultiphysics/MeshingApplication/gradual_variable_interpolation_process.py
+  KratosMeshingApplication.libs/libKratosMeshingCore-00c820f7.so
 
-  offset of local header from start of archive:   1226284
-                                                  (000000000012B62Ch) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1831343
+                                                  (00000000001BF1AFh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         ca25fbe6
-  compressed size:                                1322 bytes
-  uncompressed size:                              4870 bytes
-  length of filename:                             79 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         13d90448
+  compressed size:                                2957842 bytes
+  uncompressed size:                              10551313 bytes
+  length of filename:                             62 characters
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
 
-Central directory entry #6:
+Central directory entry #12:
 ---------------------------
 
-  KratosMultiphysics/MeshingApplication/mmg_process.py
+  KratosMultiphysics/
 
-  offset of local header from start of archive:   1227715
-                                                  (000000000012BBC3h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   4789305
+                                                  (0000000000491439h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             19 characters
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
+  KratosMultiphysics/.libs/
+
+  offset of local header from start of archive:   4789382
+                                                  (0000000000491486h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:22
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:21 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:21 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             25 characters
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
+Central directory entry #14:
+---------------------------
+
+  KratosMultiphysics/.libs/KratosMeshingApplication.cpython-39-x86_64-linux-gnu.so
+
+  offset of local header from start of archive:   4789465
+                                                  (00000000004914D9h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         bf157bfa
-  compressed size:                                8933 bytes
-  uncompressed size:                              51951 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         3b3a3920
+  compressed size:                                1408349 bytes
+  uncompressed size:                              3886409 bytes
+  length of filename:                             80 characters
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
 
-Central directory entry #7:
+Central directory entry #15:
+---------------------------
+
+  KratosMultiphysics/MeshingApplication/
+
+  offset of local header from start of archive:   6197952
+                                                  (00000000005E92C0h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             38 characters
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
+Central directory entry #16:
 ---------------------------
 
   KratosMultiphysics/MeshingApplication/multiscale_refining_process.py
 
-  offset of local header from start of archive:   1236730
-                                                  (000000000012DEFAh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   6198048
+                                                  (00000000005E9320h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         737e04e2
-  compressed size:                                2055 bytes
-  uncompressed size:                              9563 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         ab1e4110
+  compressed size:                                2040 bytes
+  uncompressed size:                              9371 bytes
   length of filename:                             68 characters
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
 
-Central directory entry #8:
+Central directory entry #17:
 ---------------------------
 
-  KratosMeshingApplication-9.4.6.dist-info/METADATA
+  KratosMultiphysics/MeshingApplication/mmg_process.py
 
-  offset of local header from start of archive:   1238883
-                                                  (000000000012E763h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   6200214
+                                                  (00000000005E9B96h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         41b23806
-  compressed size:                                2310 bytes
-  uncompressed size:                              6202 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         aeec27e6
+  compressed size:                                8897 bytes
+  uncompressed size:                              50998 bytes
+  length of filename:                             52 characters
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
 
-Central directory entry #9:
+Central directory entry #18:
 ---------------------------
 
-  KratosMeshingApplication-9.4.6.dist-info/WHEEL
+  KratosMultiphysics/MeshingApplication/gradual_variable_interpolation_process.py
 
-  offset of local header from start of archive:   1241272
-                                                  (000000000012F0B8h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   6209221
+                                                  (00000000005EBEC5h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         86fb6b41
-  compressed size:                                96 bytes
-  uncompressed size:                              100 bytes
-  length of filename:                             46 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         7e9effda
+  compressed size:                                1315 bytes
+  uncompressed size:                              4792 bytes
+  length of filename:                             79 characters
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
+Central directory entry #19:
+---------------------------
+
+  KratosMultiphysics/MeshingApplication/modelers/
+
+  offset of local header from start of archive:   6210673
+                                                  (00000000005EC471h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             47 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
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
+Central directory entry #20:
+---------------------------
+
+  KratosMultiphysics/MeshingApplication/modelers/convert_linear_tetrahedra_to_quadratic_modeler.py
+
+  offset of local header from start of archive:   6210778
+                                                  (00000000005EC4DAh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         186778b0
+  compressed size:                                1235 bytes
+  uncompressed size:                              4267 bytes
+  length of filename:                             96 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
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
 
-Central directory entry #10:
+Central directory entry #21:
 ---------------------------
 
-  KratosMeshingApplication-9.4.6.dist-info/top_level.txt
+  KratosMultiphysics/MeshingApplication/__init__.py
 
-  offset of local header from start of archive:   1241444
-                                                  (000000000012F164h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   6212167
+                                                  (00000000005ECA47h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         f32d789f
-  compressed size:                                21 bytes
-  uncompressed size:                              19 bytes
-  length of filename:                             54 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         d504a9ce
+  compressed size:                                220 bytes
+  uncompressed size:                              592 bytes
+  length of filename:                             49 characters
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
 
-Central directory entry #11:
+Central directory entry #22:
 ---------------------------
 
-  KratosMeshingApplication-9.4.6.dist-info/RECORD
+  KratosMultiphysics/MeshingApplication/python_registry_lists.py
 
-  offset of local header from start of archive:   1241549
-                                                  (000000000012F1CDh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   6212494
+                                                  (00000000005ECB8Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         71f3ead1
-  compressed size:                                603 bytes
-  uncompressed size:                              1167 bytes
-  length of filename:                             47 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:14
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:14 UTC
+  32-bit CRC value (hex):                         d5c08402
+  compressed size:                                142 bytes
+  uncompressed size:                              305 bytes
+  length of filename:                             62 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B400 hex
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
```

## zipnote {}

```diff
@@ -1,34 +1,67 @@
-Filename: KratosMultiphysics/.libs/KratosMeshingApplication.pyd
+Filename: KratosMeshingApplication-9.5.dist-info/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosMeshingCore.dll
+Filename: KratosMeshingApplication-9.5.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosMeshingCore.lib
+Filename: KratosMeshingApplication-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics/MeshingApplication/__init__.py
+Filename: KratosMeshingApplication-9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosMultiphysics/MeshingApplication/gradual_variable_interpolation_process.py
+Filename: KratosMeshingApplication-9.5.dist-info/RECORD
 Comment: 
 
-Filename: KratosMultiphysics/MeshingApplication/mmg_process.py
+Filename: KratosMeshingApplication.libs/
+Comment: 
+
+Filename: KratosMeshingApplication.libs/libmmg-ef3d646f.so.5.5.1
+Comment: 
+
+Filename: KratosMeshingApplication.libs/libmmgs-a9c9f31a.so.5.5.1
+Comment: 
+
+Filename: KratosMeshingApplication.libs/libmmg2d-808e00cf.so.5.5.1
+Comment: 
+
+Filename: KratosMeshingApplication.libs/libmmg3d-48d89c48.so.5.5.1
+Comment: 
+
+Filename: KratosMeshingApplication.libs/libKratosMeshingCore-00c820f7.so
+Comment: 
+
+Filename: KratosMultiphysics/
+Comment: 
+
+Filename: KratosMultiphysics/.libs/
+Comment: 
+
+Filename: KratosMultiphysics/.libs/KratosMeshingApplication.cpython-39-x86_64-linux-gnu.so
+Comment: 
+
+Filename: KratosMultiphysics/MeshingApplication/
 Comment: 
 
 Filename: KratosMultiphysics/MeshingApplication/multiscale_refining_process.py
 Comment: 
 
-Filename: KratosMeshingApplication-9.4.6.dist-info/METADATA
+Filename: KratosMultiphysics/MeshingApplication/mmg_process.py
+Comment: 
+
+Filename: KratosMultiphysics/MeshingApplication/gradual_variable_interpolation_process.py
 Comment: 
 
-Filename: KratosMeshingApplication-9.4.6.dist-info/WHEEL
+Filename: KratosMultiphysics/MeshingApplication/modelers/
 Comment: 
 
-Filename: KratosMeshingApplication-9.4.6.dist-info/top_level.txt
+Filename: KratosMultiphysics/MeshingApplication/modelers/convert_linear_tetrahedra_to_quadratic_modeler.py
+Comment: 
+
+Filename: KratosMultiphysics/MeshingApplication/__init__.py
 Comment: 
 
-Filename: KratosMeshingApplication-9.4.6.dist-info/RECORD
+Filename: KratosMultiphysics/MeshingApplication/python_registry_lists.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## KratosMultiphysics/MeshingApplication/__init__.py

```diff
@@ -1,10 +1,14 @@
-# Application dependent names and paths
-from KratosMultiphysics import _ImportApplication
-from KratosMultiphysics import IsDistributedRun
-if IsDistributedRun():
-    import KratosMultiphysics.mpi # importing the MPI-Core
-from KratosMeshingApplication import *
-application = KratosMeshingApplication()
-application_name = "KratosMeshingApplication"
-
-_ImportApplication(application, application_name)
+# Application dependent names and paths
+from KratosMultiphysics import _ImportApplication
+from KratosMultiphysics import IsDistributedRun
+if IsDistributedRun():
+    import KratosMultiphysics.mpi # importing the MPI-Core
+from KratosMeshingApplication import *
+application = KratosMeshingApplication()
+application_name = "KratosMeshingApplication"
+
+_ImportApplication(application, application_name)
+
+from KratosMultiphysics import python_registry_utilities
+from . import python_registry_lists
+python_registry_utilities.RegisterAll("KratosMultiphysics.MeshingApplication", python_registry_lists)
```

## KratosMultiphysics/MeshingApplication/gradual_variable_interpolation_process.py

 * *Ordering differences only*

```diff
@@ -1,79 +1,79 @@
-import KratosMultiphysics
-import KratosMultiphysics.MeshingApplication as KratosMA
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return GradualVariableInterpolationProcess(model, settings["Parameters"])
-
-class GradualVariableInterpolationProcess(KratosMultiphysics.Process):
-    """This class defines a process for gradually interpolating nodal values from one 
-    model part to another, called the origin and destination model parts respectively. 
-    The rate of interpolation can be controlled through an increment parameter 'alpha_rampup_increment' 
-    or by specifying the total number of steps for the full interpolation 'steps_for_rampup'. 
-    The list of variables to be interpolated is also user-definable."""
-    def __init__(self, model, settings):
-        KratosMultiphysics.Process.__init__(self)
-
-        default_settings = KratosMultiphysics.Parameters("""{
-            "origin_model_part_file_name" : "NameOfMDPAfile",
-            "destination_model_part_name" : "ModelPartName",
-            "interpolation_variables_list": [],
-            "constrain_variables": false,
-            "alpha_rampup_increment": 0.0,
-            "steps_for_rampup": 0.0
-        }""")
-
-        settings.ValidateAndAssignDefaults(default_settings)
-
-        self.model = model
-        self.settings = settings
-        self.constrain_variables = self.settings["constrain_variables"].GetBool()
-        self.alpha_rampup_increment = self.settings["alpha_rampup_increment"].GetDouble()
-        self.steps_for_rampup = self.settings["steps_for_rampup"].GetInt()
-
-        if not self.alpha_rampup_increment and not self.steps_for_rampup:
-            KratosMultiphysics.Logger.PrintWarning('GradualVariableInterpolationProcess', 'Neither alpha_rampup_increment nor steps_for_rampup was specified; defaulting to alpha_rampup_increment = 1.0')
-            self.alpha_rampup_increment = 1.0
-        elif self.alpha_rampup_increment and self.steps_for_rampup:
-            KratosMultiphysics.Logger.PrintWarning('GradualVariableInterpolationProcess', 'Both alpha_rampup_increment and steps_for_rampup were specified; using alpha_rampup_increment and ignoring steps_for_rampup')
-        elif self.alpha_rampup_increment:
-            if self.alpha_rampup_increment < 0 or self.alpha_rampup_increment > 1:
-                raise Exception("'alpha_rampup_increment' must be in the interval (0, 1].")
-        elif self.steps_for_rampup:
-            if self.steps_for_rampup <= 0:
-                raise Exception("'steps_for_rampup' must be a positive integer.")
-            else:
-                self.alpha_rampup_increment = 1.0 / self.steps_for_rampup
-
-        self.alpha = 0.0
-        self.expected_alpha = 1.0
-        self.interpolation_variables_list = self.settings["interpolation_variables_list"].GetStringArray()
-
-    def ExecuteInitialize(self):
-        origin_model_part_file_name = self.settings["origin_model_part_file_name"].GetString()
-        destination_model_part_name = self.settings["destination_model_part_name"].GetString()
-        self.destination_model_part = self.model.GetModelPart(destination_model_part_name)
-        
-        # Import Origin Model Part 
-        self.origin_model_part = self.model.CreateModelPart("OriginModelPart")
-        for variable in self.destination_model_part.GetHistoricalVariablesNames():
-            if KratosMultiphysics.KratosGlobals.HasVariable(variable):
-                self.origin_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.KratosGlobals.GetVariable(variable))
-            else:
-                raise Exception(f"Variable '{variable}' does not exist or is not valid in KratosMultiphysics.")
-                
-        model_part_io = KratosMultiphysics.ModelPartIO(origin_model_part_file_name)
-        model_part_io.ReadModelPart(self.origin_model_part)
-
-        self.domain_size = self.destination_model_part.ProcessInfo.GetValue(KratosMultiphysics.DOMAIN_SIZE)
-
-        KratosMA.GradualVariableInterpolationUtility.InitializeInterpolationAndConstraints(self.origin_model_part, self.destination_model_part, self.interpolation_variables_list, self.alpha_rampup_increment, self.domain_size, self.constrain_variables)
-
-    def ExecuteInitializeSolutionStep(self):
-        self.old_alpha = self.alpha
-        if self.old_alpha == 0.0:
-            self.old_alpha = self.alpha_rampup_increment
-        self.alpha += self.alpha_rampup_increment
-        if self.alpha <= self.expected_alpha:
+import KratosMultiphysics
+import KratosMultiphysics.MeshingApplication as KratosMA
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return GradualVariableInterpolationProcess(model, settings["Parameters"])
+
+class GradualVariableInterpolationProcess(KratosMultiphysics.Process):
+    """This class defines a process for gradually interpolating nodal values from one 
+    model part to another, called the origin and destination model parts respectively. 
+    The rate of interpolation can be controlled through an increment parameter 'alpha_rampup_increment' 
+    or by specifying the total number of steps for the full interpolation 'steps_for_rampup'. 
+    The list of variables to be interpolated is also user-definable."""
+    def __init__(self, model, settings):
+        KratosMultiphysics.Process.__init__(self)
+
+        default_settings = KratosMultiphysics.Parameters("""{
+            "origin_model_part_file_name" : "NameOfMDPAfile",
+            "destination_model_part_name" : "ModelPartName",
+            "interpolation_variables_list": [],
+            "constrain_variables": false,
+            "alpha_rampup_increment": 0.0,
+            "steps_for_rampup": 0.0
+        }""")
+
+        settings.ValidateAndAssignDefaults(default_settings)
+
+        self.model = model
+        self.settings = settings
+        self.constrain_variables = self.settings["constrain_variables"].GetBool()
+        self.alpha_rampup_increment = self.settings["alpha_rampup_increment"].GetDouble()
+        self.steps_for_rampup = self.settings["steps_for_rampup"].GetInt()
+
+        if not self.alpha_rampup_increment and not self.steps_for_rampup:
+            KratosMultiphysics.Logger.PrintWarning('GradualVariableInterpolationProcess', 'Neither alpha_rampup_increment nor steps_for_rampup was specified; defaulting to alpha_rampup_increment = 1.0')
+            self.alpha_rampup_increment = 1.0
+        elif self.alpha_rampup_increment and self.steps_for_rampup:
+            KratosMultiphysics.Logger.PrintWarning('GradualVariableInterpolationProcess', 'Both alpha_rampup_increment and steps_for_rampup were specified; using alpha_rampup_increment and ignoring steps_for_rampup')
+        elif self.alpha_rampup_increment:
+            if self.alpha_rampup_increment < 0 or self.alpha_rampup_increment > 1:
+                raise Exception("'alpha_rampup_increment' must be in the interval (0, 1].")
+        elif self.steps_for_rampup:
+            if self.steps_for_rampup <= 0:
+                raise Exception("'steps_for_rampup' must be a positive integer.")
+            else:
+                self.alpha_rampup_increment = 1.0 / self.steps_for_rampup
+
+        self.alpha = 0.0
+        self.expected_alpha = 1.0
+        self.interpolation_variables_list = self.settings["interpolation_variables_list"].GetStringArray()
+
+    def ExecuteInitialize(self):
+        origin_model_part_file_name = self.settings["origin_model_part_file_name"].GetString()
+        destination_model_part_name = self.settings["destination_model_part_name"].GetString()
+        self.destination_model_part = self.model.GetModelPart(destination_model_part_name)
+        
+        # Import Origin Model Part 
+        self.origin_model_part = self.model.CreateModelPart("OriginModelPart")
+        for variable in self.destination_model_part.GetHistoricalVariablesNames():
+            if KratosMultiphysics.KratosGlobals.HasVariable(variable):
+                self.origin_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.KratosGlobals.GetVariable(variable))
+            else:
+                raise Exception(f"Variable '{variable}' does not exist or is not valid in KratosMultiphysics.")
+                
+        model_part_io = KratosMultiphysics.ModelPartIO(origin_model_part_file_name)
+        model_part_io.ReadModelPart(self.origin_model_part)
+
+        self.domain_size = self.destination_model_part.ProcessInfo.GetValue(KratosMultiphysics.DOMAIN_SIZE)
+
+        KratosMA.GradualVariableInterpolationUtility.InitializeInterpolationAndConstraints(self.origin_model_part, self.destination_model_part, self.interpolation_variables_list, self.alpha_rampup_increment, self.domain_size, self.constrain_variables)
+
+    def ExecuteInitializeSolutionStep(self):
+        self.old_alpha = self.alpha
+        if self.old_alpha == 0.0:
+            self.old_alpha = self.alpha_rampup_increment
+        self.alpha += self.alpha_rampup_increment
+        if self.alpha <= self.expected_alpha:
             KratosMA.GradualVariableInterpolationUtility.UpdateSolutionStepVariables(self.destination_model_part, self.interpolation_variables_list, self.alpha, self.old_alpha, self.constrain_variables)
```

## KratosMultiphysics/MeshingApplication/mmg_process.py

 * *Ordering differences only*

```diff
@@ -1,954 +1,954 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KratosMultiphysics
-import KratosMultiphysics.MeshingApplication as MeshingApplication
-
-try:
-    import KratosMultiphysics.StructuralMechanicsApplication as StructuralMechanicsApplication
-    structural_dependencies = True
-except ImportError as e:
-    structural_dependencies = False
-
-# Some Kratos dependencies
-from KratosMultiphysics import kratos_utilities
-from KratosMultiphysics import json_utilities
-
-# Some python dependencies
-import os
-import statistics as stat
-
-def Factory(settings, Model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return MmgProcess(Model, settings["Parameters"])
-
-class MmgProcess(KratosMultiphysics.Process):
-    """This process remeshes using MMG library. This process uses different utilities and processes
-
-    Only the member variables listed below should be accessed directly.
-
-    Public member variables:
-    Model -- the container of the different model parts.
-    settings -- Kratos parameters containing solver settings.
-    """
-
-    def __init__(self, Model, settings ):
-        """ The default constructor of the class
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        Model -- the container of the different model parts.
-        settings -- Kratos parameters containing solver settings.
-        """
-
-        KratosMultiphysics.Process.__init__(self)
-
-        ## Settings string in json format
-        default_parameters = KratosMultiphysics.Parameters("""
-        {
-            "help"                             : "This process remeshes using MMG library. This process uses different utilities and processes",
-            "mesh_id"                          : 0,
-            "filename"                         : "out",
-            "model_part_name"                  : "PLEASE_SPECIFY_MODEL_PART_NAME",
-            "blocking_threshold_size"          : false,
-            "threshold_sizes"                  : {
-                "minimal_size"                     : 0.1,
-                "maximal_size"                     : 10.0
-            },
-            "strategy"                         : "levelset",
-            "level_set_strategy_parameters"    : {
-                "scalar_variable"                  : "DISTANCE",
-                "gradient_variable"                : "DISTANCE_GRADIENT"
-            },
-            "error_strategy_parameters"        : {
-                "compute_error_extra_parameters"     : {
-                    "stress_vector_variable"              : "CAUCHY_STRESS_VECTOR",
-                    "penalty_normal"                      : 1.0e4,
-                    "penalty_tangential"                  : 1.0e4
-                },
-                "error_metric_parameters"            : {
-                    "error_threshold"                       : 1.0e-4,
-                    "interpolation_error"                   : 0.04
-                },
-                "set_target_number_of_elements"       : false,
-                "target_number_of_elements"           : 1000,
-                "perform_nodal_h_averaging"           : false
-            },
-            "discretization_type"                  : "Standard",
-            "isosurface_parameters"                : {
-                "isosurface_variable"              : "DISTANCE",
-                "invert_value"                     : false,
-                "nonhistorical_variable"           : false,
-                "use_metric_field"                 : false,
-                "remove_internal_regions"          : false
-            },
-            "framework"                            : "Eulerian",
-            "internal_variables_parameters"        : {
-                "allocation_size"                      : 1000,
-                "bucket_size"                          : 4,
-                "search_factor"                        : 2,
-                "interpolation_type"                   : "LST",
-                "internal_variable_interpolation_list" :[]
-            },
-            "hessian_strategy_parameters"              :{
-                "metric_variable"                  : ["DISTANCE"],
-                "non_historical_metric_variable"   : [false],
-                "normalization_factor"             : [1.0],
-                "normalization_alpha"              : [0.0],
-                "normalization_method"             : ["constant"],
-                "estimate_interpolation_error"     : false,
-                "interpolation_error"              : 0.04,
-                "mesh_dependent_constant"          : 0.28125
-            },
-            "enforce_current"                  : true,
-            "remesh_control_type"              : "step",
-            "initial_step"                     : 1,
-            "step_frequency"                   : 0,
-            "interval"                         : [0.0, 1e30],
-            "time_stepping"                    : {},
-            "automatic_remesh"                 : true,
-            "automatic_remesh_parameters"      : {
-                "automatic_remesh_type"            : "Ratio",
-                "min_size_ratio"                   : 1.0,
-                "max_size_ratio"                   : 3.0,
-                "refer_type"                       : "Mean",
-                "min_size_current_percentage"      : 50.0,
-                "max_size_current_percentage"      : 98.0
-            },
-            "initial_remeshing"                : false,
-            "fix_contour_model_parts"          : [],
-            "fix_conditions_model_parts"       : [],
-            "fix_elements_model_parts"         : [],
-            "force_min"                        : false,
-            "minimal_size"                     : 0.1,
-            "force_max"                        : false,
-            "maximal_size"                     : 10.0,
-            "sizing_parameters"                : {
-                "reference_variable_name"          : "DISTANCE",
-                "boundary_layer_max_distance"      : 1.0,
-                "interpolation"                    : "constant"
-            },
-            "advanced_parameters"                  : {
-                "force_hausdorff_value"            : false,
-                "hausdorff_value"                  : 0.0001,
-                "no_move_mesh"                     : false,
-                "no_surf_mesh"                     : false,
-                "no_insert_mesh"                   : false,
-                "no_swap_mesh"                     : false,
-                "normal_regularization_mesh"       : false,
-                "deactivate_detect_angle"          : false,
-                "force_angle_detection_value"      : false,
-                "angle_detection_value"            : 45.0,
-                "force_gradation_value"            : false,
-                "mesh_optimization_only"           : false,
-                "gradation_value"                  : 1.3,
-                "local_entity_parameters_list"     : []
-            },
-            "anisotropy_remeshing"                 : true,
-            "enforce_anisotropy_relative_variable" : false,
-            "anisotropy_parameters":{
-                "reference_variable_name"          : "DISTANCE",
-                "hmin_over_hmax_anisotropic_ratio" : 0.01,
-                "boundary_layer_max_distance"      : 1.0,
-                "boundary_layer_min_size_ratio"    : 2.0,
-                "interpolation"                    : "Linear"
-            },
-            "collapse_prisms_elements"         : false,
-            "save_external_files"              : false,
-            "save_colors_files"                : false,
-            "save_mdpa_file"                   : false,
-            "remesh_at_finalize"               : false,
-            "output_final_mesh"                : false,
-            "sub_model_part_names_to_remove"   : [],
-            "output_mesh_file_name"            : "final_refined_mesh",
-            "max_number_of_searchs"            : 1000,
-            "preserve_flags"                   : true,
-            "interpolate_nodal_values"         : true,
-            "interpolate_non_historical"       : true,
-            "use_mapper_if_available"          : false,
-            "mapping_parameters"               : {
-                "mapper_type"                      : "nearest_element",
-                "echo_level"                       : 0,
-                "search_settings" : {
-                    "max_num_search_iterations"    : 8,
-                    "echo_level"                   : 0
-                }
-            }, 
-            "extrapolate_contour_values"       : true,
-            "surface_elements"                 : false,
-            "search_parameters"                : {
-                "allocation_size"                  : 1000,
-                "bucket_size"                      : 4,
-                "search_factor"                    : 2.0
-            },
-            "debug_mode"                       : "",
-            "debug_result_mesh"                : false,
-            "initialize_entities"              : true,
-            "echo_level"                       : 3
-        }
-        """)
-
-        # Identify the dimension first
-        if not settings.Has("model_part_name"):
-            settings.AddValue("model_part_name", default_parameters["model_part_name"])
-
-        # Getting model part and working dimension
-        self.main_model_part = Model[settings["model_part_name"].GetString()]
-        self.domain_size = self.main_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
-        self.is_surface = False
-        if self.domain_size == 3:
-            for elem in self.main_model_part.Elements:
-                geom = elem.GetGeometry()
-                if geom.WorkingSpaceDimension() != geom.LocalSpaceDimension():
-                    self.is_surface = True
-                break
-
-        # The mesh dependent constant depends on dimension
-        if self.domain_size == 2:
-            default_parameters["hessian_strategy_parameters"]["mesh_dependent_constant"].SetDouble(2.0/9.0)
-        else:
-            default_parameters["hessian_strategy_parameters"]["mesh_dependent_constant"].SetDouble(9.0/32.0)
-
-        # Assign this here since it will change the "interval" prior to validation
-        self.interval = KratosMultiphysics.IntervalUtility(settings)
-
-        # Time stepping
-        if not hasattr(self, 'time_stepping'):
-            self.time_stepping = KratosMultiphysics.Parameters("""{}""")
-            if settings.Has("time_stepping"):
-                self.time_stepping = settings["time_stepping"].Clone()
-                settings.RemoveValue("time_stepping")
-
-        # Overwrite the default settings with user-provided parameters
-        self.settings = settings
-        self.settings.RecursivelyValidateAndAssignDefaults(default_parameters)
-
-        # Getting some settings
-        self.strategy = _check_strategy(self.settings["strategy"].GetString())
-        self.enforce_current = self.settings["enforce_current"].GetBool()
-        self.initial_remeshing = self.settings["initial_remeshing"].GetBool()
-        self.remesh_control_type = self.settings["remesh_control_type"].GetString()
-        self.initial_step = self.settings["initial_step"].GetInt()
-        self.step_frequency = self.settings["step_frequency"].GetInt()
-        self.settings["surface_elements"].SetBool(self.is_surface)
-
-        # Setting initial_step_done here
-        self.initial_step_done = False
-
-        # Initialize flag
-        self.remesh_executed = False
-
-    def ExecuteInitialize(self):
-        """ This method is executed at the begining to initialize the process
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-
-        # Calculate NODAL_H
-        KratosMultiphysics.VariableUtils().SetNonHistoricalVariable(KratosMultiphysics.NODAL_H, 0.0, self.main_model_part.Nodes)
-        KratosMultiphysics.VariableUtils().SetNonHistoricalVariable(KratosMultiphysics.NODAL_AREA, 0.0, self.main_model_part.Nodes)
-        self.find_nodal_h = KratosMultiphysics.FindNodalHNonHistoricalProcess(self.main_model_part)
-        self.find_nodal_h.Execute()
-
-        # Calculate the parameters of automatic remeshing
-        if self.settings["automatic_remesh"].GetBool():
-            nodal_h_values = []
-            for node in self.main_model_part.Nodes:
-                nodal_h_values.append(node.GetValue(KratosMultiphysics.NODAL_H))
-
-            # Calculate the minimum size
-            if self.settings["automatic_remesh_parameters"]["automatic_remesh_type"].GetString() == "Ratio":
-                # NOTE: For mode: https://docs.python.org/3/library/statistics.html
-                if self.settings["automatic_remesh_parameters"]["refer_type"].GetString() == "Mean":
-                    ref = stat.mean(nodal_h_values)
-                elif self.settings["automatic_remesh_parameters"]["refer_type"].GetString() == "Median":
-                    ref = stat.median(nodal_h_values)
-
-                self.settings["minimal_size"].SetDouble(ref * (self.settings["automatic_remesh_parameters"]["min_size_ratio"].GetDouble()))
-                self.settings["maximal_size"].SetDouble(ref * (self.settings["automatic_remesh_parameters"]["max_size_ratio"].GetDouble()))
-            elif self.settings["automatic_remesh_parameters"]["automatic_remesh_type"].GetString() == "Percentage":
-                mean = stat.mean(nodal_h_values)
-                stdev = stat.stdev(nodal_h_values)
-                prob = (self.settings["automatic_remesh_parameters"]["min_size_current_percentage"].GetDouble())/100
-                self.settings["minimal_size"].SetDouble(_normvalf(prob, mean, stdev)) # Using normal normal distribution to get the minimal size as a stadistical meaninful value
-
-                prob = (self.settings["automatic_remesh_parameters"]["max_size_current_percentage"].GetDouble())/100
-                self.settings["maximal_size"].SetDouble(_normvalf(prob, mean, stdev)) # Using normal normal distribution to get the maximal size as a stadistical meaninful value
-
-            # We deactivate, so it doesn't recalculate each initialization
-            self.settings["automatic_remesh"].SetBool(False)
-
-        ## We print the parameters considered
-        KratosMultiphysics.Logger.PrintInfo("MINIMAL SIZE: ", "{:.2e}".format(self.settings["minimal_size"].GetDouble()))
-        KratosMultiphysics.Logger.PrintInfo("MAXIMAL SIZE: ", "{:.2e}".format(self.settings["maximal_size"].GetDouble()))
-
-        # Anisotropic remeshing parameters
-        self.anisotropy_remeshing = self.settings["anisotropy_remeshing"].GetBool()
-        if self.anisotropy_remeshing:
-            if self.settings["automatic_remesh"].GetBool():
-                self.settings["anisotropy_parameters"]["boundary_layer_max_distance"].SetDouble(self.settings["minimal_size"].GetDouble() * self.settings["anisotropy_parameters"]["boundary_layer_min_size_ratio"].GetDouble())
-
-        # Select the remeshing strategy
-        if self.strategy == "levelset":
-            self.scalar_variable = KratosMultiphysics.KratosGlobals.GetVariable( self.settings["level_set_strategy_parameters"]["scalar_variable"].GetString() )
-            self.gradient_variable = KratosMultiphysics.KratosGlobals.GetVariable( self.settings["level_set_strategy_parameters"]["gradient_variable"].GetString() )
-        elif self.strategy == "hessian":
-            self.metric_variables, variable_types = self.__generate_variable_list_from_input(self.settings["hessian_strategy_parameters"]["metric_variable"])
-            self.non_historical_metric_variable = self.__generate_boolean_list_from_input(self.settings["hessian_strategy_parameters"]["non_historical_metric_variable"])
-            self.non_historical_metric_variable = self.__list_extender(self.non_historical_metric_variable, variable_types)
-            self.normalization_factor = self.__generate_double_list_from_input(self.settings["hessian_strategy_parameters"]["normalization_factor"])
-            self.normalization_factor = self.__list_extender(self.normalization_factor, variable_types)
-            self.normalization_alpha = self.__generate_double_list_from_input(self.settings["hessian_strategy_parameters"]["normalization_alpha"])
-            self.normalization_alpha = self.__list_extender(self.normalization_alpha, variable_types)
-            self.normalization_method = self.__generate_string_list_from_input(self.settings["hessian_strategy_parameters"]["normalization_method"])
-            self.normalization_method = self.__list_extender(self.normalization_method, variable_types)
-            len_metric_variables = len(self.metric_variables)
-            len_non_historical_metric_variable = len(self.non_historical_metric_variable)
-            if len_metric_variables > len_non_historical_metric_variable:
-                for i in range(len_non_historical_metric_variable, len_metric_variables):
-                    self.non_historical_metric_variable.append(False)
-            len_normalization_factor = len(self.normalization_factor)
-            if len_metric_variables > len_normalization_factor:
-                for i in range(len_normalization_factor, len_metric_variables):
-                    self.normalization_factor.append(1.0)
-            len_normalization_alpha = len(self.normalization_alpha)
-            if len_metric_variables > len_normalization_alpha:
-                for i in range(len_normalization_alpha, len_metric_variables):
-                    self.normalization_alpha.append(0.0)
-            len_normalization_method = len(self.normalization_method)
-            if len_metric_variables > len_normalization_method:
-                for i in range(len_normalization_method, len_metric_variables):
-                    self.normalization_method.append("constant")
-            mesh_dependent_constant = self.settings["hessian_strategy_parameters"]["mesh_dependent_constant"].GetDouble()
-            if mesh_dependent_constant == 0.0:
-                self.settings["hessian_strategy_parameters"]["mesh_dependent_constant"].SetDouble(0.5 * (self.domain_size/(self.domain_size + 1))**2.0)
-        elif self.strategy == "superconvergent_patch_recovery" or self.strategy == "spr":
-            self.error_threshold = self.settings["error_strategy_parameters"]["error_metric_parameters"]["error_threshold"].GetDouble()
-            self.error_ratio = 0
-
-        self.internal_variable_interpolation_list = kratos_utilities.GenerateVariableListFromInput(self.settings["internal_variables_parameters"]["internal_variable_interpolation_list"])
-
-        # Model parts to fix the nodes
-        fix_contour_model_parts = self.__generate_submodelparts_list_from_input(self.settings["fix_contour_model_parts"])
-
-        # Setting flag BLOCKED to the non nodes
-        for submodelpart in fix_contour_model_parts:
-            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.BLOCKED, True, submodelpart.Nodes)
-
-        # Model parts to fix the conditions
-        fix_conditions_model_parts = self.__generate_submodelparts_list_from_input(self.settings["fix_conditions_model_parts"])
-
-        # Setting flag BLOCKED to the non conditions
-        for submodelpart in fix_conditions_model_parts:
-            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.BLOCKED, True, submodelpart.Conditions)
-
-        # Model parts to fix the nodes
-        fix_elements_model_parts = self.__generate_submodelparts_list_from_input(self.settings["fix_elements_model_parts"])
-
-        # Setting flag BLOCKED to the non elements
-        for submodelpart in fix_elements_model_parts:
-            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.BLOCKED, True, submodelpart.Elements)
-
-        if self.strategy == "levelset":
-            self._CreateGradientProcess()
-
-        if self.domain_size == 2:
-            self.initialize_metric = MeshingApplication.MetricFastInit2D(self.main_model_part)
-        else:
-            self.initialize_metric = MeshingApplication.MetricFastInit3D(self.main_model_part)
-
-        self.initialize_metric.Execute()
-
-        self._CreateMetricsProcess()
-
-        mmg_parameters = KratosMultiphysics.Parameters("""{"force_sizes":{}}""")
-        mmg_parameters.AddValue("filename",self.settings["filename"])
-        mmg_parameters.AddValue("framework",self.settings["framework"])
-        mmg_parameters.AddValue("discretization_type",self.settings["discretization_type"])
-        mmg_parameters.AddValue("isosurface_parameters",self.settings["isosurface_parameters"])
-        mmg_parameters.AddValue("internal_variables_parameters",self.settings["internal_variables_parameters"])
-        mmg_parameters.AddValue("collapse_prisms_elements",self.settings["collapse_prisms_elements"])
-        mmg_parameters.AddValue("save_external_files",self.settings["save_external_files"])
-        mmg_parameters.AddValue("save_colors_files",self.settings["save_colors_files"])
-        mmg_parameters.AddValue("save_mdpa_file",self.settings["save_mdpa_file"])
-        mmg_parameters.AddValue("max_number_of_searchs",self.settings["max_number_of_searchs"])
-        mmg_parameters.AddValue("preserve_flags",self.settings["preserve_flags"])
-        mmg_parameters.AddValue("interpolate_nodal_values",self.settings["interpolate_nodal_values"])
-        mmg_parameters.AddValue("interpolate_non_historical",self.settings["interpolate_non_historical"])
-        mmg_parameters.AddValue("extrapolate_contour_values",self.settings["extrapolate_contour_values"])
-        mmg_parameters.AddValue("search_parameters",self.settings["search_parameters"])
-        mmg_parameters["force_sizes"].AddValue("force_min",self.settings["force_min"])
-        mmg_parameters["force_sizes"].AddValue("minimal_size",self.settings["minimal_size"])
-        mmg_parameters["force_sizes"].AddValue("force_max",self.settings["force_max"])
-        mmg_parameters["force_sizes"].AddValue("maximal_size",self.settings["maximal_size"])
-        mmg_parameters.AddValue("advanced_parameters",self.settings["advanced_parameters"])
-        mmg_parameters.AddValue("debug_result_mesh",self.settings["debug_result_mesh"])
-        mmg_parameters.AddValue("initialize_entities",self.settings["initialize_entities"])
-        mmg_parameters.AddValue("echo_level",self.settings["echo_level"])
-        if self.strategy == "optimization":
-            mmg_parameters["advanced_parameters"]["mesh_optimization_only"].SetBool(True)
-
-        if self.domain_size == 2:
-            self.mmg_process = MeshingApplication.MmgProcess2D(self.main_model_part, mmg_parameters)
-        else:
-            # Differentiate between 3D volumes and 3D surfaces
-            if self.is_surface:
-                self.mmg_process = MeshingApplication.MmgProcess3DSurfaces(self.main_model_part, mmg_parameters)
-            else:
-                self.mmg_process = MeshingApplication.MmgProcess3D(self.main_model_part, mmg_parameters)
-
-        # We reset the step and time
-        self.step = 0
-        self.time = 0.0
-
-        # We compute initial remeshing is desired
-        if self.initial_remeshing:
-            if not self.main_model_part.Is(KratosMultiphysics.MODIFIED):
-                self._ExecuteRefinement()
-            else:
-                self.main_model_part.Set(KratosMultiphysics.MODIFIED, False)
-
-    def ExecuteInitializeSolutionStep(self):
-        """ This method is executed in order to initialize the current step
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-
-        # If not previous remesh
-        if not self.remesh_executed:
-            if not self.initial_remeshing:
-                # We need to check if the model part has been modified recently
-                if self.main_model_part.Is(KratosMultiphysics.MODIFIED):
-                    self.main_model_part.Set(KratosMultiphysics.MODIFIED, False)
-                    self.step = 0  # Reset (just to be sure)
-                    self.time = 0.0  # Reset (just to be sure)
-                else:
-                    current_time = self.main_model_part.ProcessInfo[KratosMultiphysics.TIME]
-                    if self.interval.IsInInterval(current_time):
-                        # We remesh if needed
-                        if self.__execute_remesh():
-                            if self.strategy in ["hessian", "levelset", "optimization"]:
-                                if self.settings["blocking_threshold_size"].GetBool():
-                                    MeshingApplication.BlockThresholdSizeElements(self.main_model_part, self.settings["threshold_sizes"])
-                                self._ExecuteRefinement()
-                                self.initial_step_done = True
-                                self.step = 0  # Reset
-                                self.time = 0.0  # Reset
-
-    def ExecuteFinalize(self):
-        """ This method is executed in order to finalize the simulation and save the refined mesh in a new .mdpa file
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        remesh_at_finalize = self.settings["remesh_at_finalize"].GetBool()
-        output_final_mesh = self.settings["output_final_mesh"].GetBool()
-        output_mesh_file_name = self.settings["output_mesh_file_name"].GetString()
-        sub_model_part_names_to_remove = self.settings["sub_model_part_names_to_remove"].GetStringArray()
-        if remesh_at_finalize:
-            for sub_model_part_name in sub_model_part_names_to_remove:
-                if self.main_model_part.HasSubModelPart(sub_model_part_name):
-                    self.main_model_part.RemoveSubModelPart(sub_model_part_name)
-            self._ExecuteRefinement()
-        if output_final_mesh:
-            KratosMultiphysics.ModelPartIO(output_mesh_file_name, KratosMultiphysics.IO.WRITE | KratosMultiphysics.IO.MESH_ONLY).WriteModelPart(self.main_model_part)
-
-    def ExecuteFinalizeSolutionStep(self):
-        """ This method is executed in order to finalize the current step
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        if self.strategy == "superconvergent_patch_recovery" or self.strategy == "spr":
-            current_time = self.main_model_part.ProcessInfo[KratosMultiphysics.TIME]
-            if self.interval.IsInInterval(current_time):
-                if self.__execute_remesh():
-                    self._ErrorCalculation()
-
-                    if self.error_ratio > self.error_threshold:
-                        self._ExecuteRefinement()
-                        self.step = 0  # Reset
-                        self.time = 0.0  # Reset
-
-        # Reset flag
-        self.remesh_executed = False
-
-    def ExecuteBeforeOutputStep(self):
-        """ This method is executed right before the ouput process computation
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        if self.strategy == "superconvergent_patch_recovery" or self.strategy == "spr":
-            current_time = self.main_model_part.ProcessInfo[KratosMultiphysics.TIME]
-            if self.interval.IsInInterval(current_time):
-                self._ErrorCalculation()
-
-    def ExecuteAfterOutputStep(self):
-        """ This method is executed right after the ouput process computation
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        pass
-
-    def _CreateMetricsProcess(self):
-        """ This method is responsible to create the metrics of the process
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        self.metric_processes = []
-        if self.strategy == "levelset":
-            level_set_parameters = KratosMultiphysics.Parameters("""{}""")
-            level_set_parameters.AddValue("minimal_size",self.settings["minimal_size"])
-            level_set_parameters.AddValue("maximal_size",self.settings["maximal_size"])
-            level_set_parameters.AddValue("sizing_parameters",self.settings["sizing_parameters"])
-            level_set_parameters.AddValue("enforce_current",self.settings["enforce_current"])
-            level_set_parameters.AddValue("anisotropy_remeshing",self.settings["anisotropy_remeshing"])
-            level_set_parameters.AddValue("anisotropy_parameters",self.settings["anisotropy_parameters"])
-            level_set_parameters["anisotropy_parameters"].RemoveValue("boundary_layer_min_size_ratio")
-            if self.domain_size == 2:
-                self.metric_processes.append(MeshingApplication.ComputeLevelSetSolMetricProcess2D(self.main_model_part, self.gradient_variable, level_set_parameters))
-            else:
-                self.metric_processes.append(MeshingApplication.ComputeLevelSetSolMetricProcess3D(self.main_model_part, self.gradient_variable, level_set_parameters))
-
-        elif self.strategy == "hessian":
-            hessian_parameters = KratosMultiphysics.Parameters("""{}""")
-            hessian_parameters.AddValue("minimal_size",self.settings["minimal_size"])
-            hessian_parameters.AddValue("maximal_size",self.settings["maximal_size"])
-            hessian_parameters.AddValue("enforce_current",self.settings["enforce_current"])
-            hessian_parameters.AddValue("hessian_strategy_parameters",self.settings["hessian_strategy_parameters"])
-            hessian_parameters["hessian_strategy_parameters"].RemoveValue("metric_variable")
-            hessian_parameters["hessian_strategy_parameters"].RemoveValue("non_historical_metric_variable")
-            hessian_parameters["hessian_strategy_parameters"].AddEmptyValue("non_historical_metric_variable")
-            hessian_parameters["hessian_strategy_parameters"].RemoveValue("normalization_factor")
-            hessian_parameters["hessian_strategy_parameters"].AddEmptyValue("normalization_factor")
-            hessian_parameters["hessian_strategy_parameters"].RemoveValue("normalization_alpha")
-            hessian_parameters["hessian_strategy_parameters"].AddEmptyValue("normalization_alpha")
-            hessian_parameters["hessian_strategy_parameters"].RemoveValue("normalization_method")
-            hessian_parameters["hessian_strategy_parameters"].AddEmptyValue("normalization_method")
-            hessian_parameters.AddValue("anisotropy_remeshing",self.settings["anisotropy_remeshing"])
-            hessian_parameters.AddValue("enforce_anisotropy_relative_variable",self.settings["enforce_anisotropy_relative_variable"])
-            hessian_parameters.AddValue("enforced_anisotropy_parameters",self.settings["anisotropy_parameters"])
-            hessian_parameters["enforced_anisotropy_parameters"].RemoveValue("boundary_layer_min_size_ratio")
-            for current_metric_variable, non_historical_metric_variable, normalization_factor, normalization_alpha, normalization_method in zip(self.metric_variables, self.non_historical_metric_variable, self.normalization_factor, self.normalization_alpha, self.normalization_method):
-                hessian_parameters["hessian_strategy_parameters"]["non_historical_metric_variable"].SetBool(non_historical_metric_variable)
-                hessian_parameters["hessian_strategy_parameters"]["normalization_factor"].SetDouble(normalization_factor)
-                hessian_parameters["hessian_strategy_parameters"]["normalization_alpha"].SetDouble(normalization_alpha)
-                hessian_parameters["hessian_strategy_parameters"]["normalization_method"].SetString(normalization_method)
-                self.metric_processes.append(MeshingApplication.ComputeHessianSolMetricProcess(self.main_model_part, current_metric_variable, hessian_parameters))
-        elif self.strategy == "superconvergent_patch_recovery" or self.strategy == "spr":
-            # Generate SPR process
-            self.error_compute = self._GenerateErrorProcess()
-
-            # Now we compute the metric
-            error_metric_parameters = KratosMultiphysics.Parameters("""{"error_strategy_parameters":{}}""")
-            error_metric_parameters.AddValue("minimal_size",self.settings["minimal_size"])
-            error_metric_parameters.AddValue("maximal_size",self.settings["maximal_size"])
-            error_metric_parameters["error_strategy_parameters"].AddValue("target_error",self.settings["error_strategy_parameters"]["error_metric_parameters"]["interpolation_error"])
-            error_metric_parameters["error_strategy_parameters"].AddValue("set_target_number_of_elements", self.settings["error_strategy_parameters"]["set_target_number_of_elements"])
-            error_metric_parameters["error_strategy_parameters"].AddValue("target_number_of_elements", self.settings["error_strategy_parameters"]["target_number_of_elements"])
-            error_metric_parameters["error_strategy_parameters"].AddValue("perform_nodal_h_averaging", self.settings["error_strategy_parameters"]["perform_nodal_h_averaging"])
-            error_metric_parameters.AddValue("echo_level", self.settings["echo_level"])
-
-            if self.domain_size == 2:
-                self.metric_process = MeshingApplication.MetricErrorProcess2D(self.main_model_part, error_metric_parameters)
-            else:
-                self.metric_process = MeshingApplication.MetricErrorProcess3D(self.main_model_part, error_metric_parameters)
-
-    def _CreateGradientProcess(self):
-        """ This method is responsible of create the gradients for the level-set process
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        # We compute the scalar value gradient
-        if self.domain_size == 2:
-            self.local_gradient = KratosMultiphysics.ComputeNodalGradientProcess2D(self.main_model_part, self.scalar_variable, self.gradient_variable, KratosMultiphysics.NODAL_AREA)
-        else:
-            self.local_gradient = KratosMultiphysics.ComputeNodalGradientProcess3D(self.main_model_part, self.scalar_variable, self.gradient_variable, KratosMultiphysics.NODAL_AREA)
-
-    def _ExecuteRefinement(self):
-        """ This method is the one responsible to execute the remeshing
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        if self.strategy == "levelset":
-            # Calculate the gradient
-            self.local_gradient.Execute()
-
-        # Recalculate NODAL_H
-        self.find_nodal_h.Execute()
-
-        # Initialize metric
-        if self.strategy == "hessian" or self.strategy == "levelset":
-            self.initialize_metric.Execute()
-
-        KratosMultiphysics.Logger.PrintInfo("MMG Remeshing Process", "Calculating the metrics")
-        # Execute metric computation
-        for metric_process in self.metric_processes:
-            metric_process.Execute()
-
-        # Debug before remesh
-        if self.settings["debug_mode"].GetString() == "GiD": # GiD
-            self._debug_output_gid(self.main_model_part.ProcessInfo[KratosMultiphysics.STEP], "", "BEFORE_")
-        elif self.settings["debug_mode"].GetString() == "VTK": # VTK
-            self._debug_output_vtk(self.main_model_part.ProcessInfo[KratosMultiphysics.STEP], "", "BEFORE_")
-
-        # Execute before remesh
-        self._AuxiliarCallsBeforeRemesh()
-
-        # Actually remesh
-        KratosMultiphysics.Logger.PrintInfo("MMG Remeshing Process", "Remeshing")
-        self.mmg_process.Execute()
-
-        # Execute after remesh
-        self._AuxiliarCallsAfterRemesh()
-
-        # Debug after remesh
-        if self.settings["debug_mode"].GetString() == "GiD": # GiD
-            self._debug_output_gid(self.main_model_part.ProcessInfo[KratosMultiphysics.STEP], "", "AFTER_")
-        elif self.settings["debug_mode"].GetString() == "VTK": # VTK
-            self._debug_output_vtk(self.main_model_part.ProcessInfo[KratosMultiphysics.STEP], "", "AFTER_")
-
-        if self.strategy == "levelset":
-            self.local_gradient.Execute() # Recalculate gradient after remeshing
-
-        # Recalculate NODAL_H
-        self.find_nodal_h.Execute()
-
-        # We need to set that the model part has been modified (later on we will act in consequence)
-        self.main_model_part.Set(KratosMultiphysics.MODIFIED, True)
-
-        # Deactivate to avoid remesh again
-        self.remesh_executed = True
-
-        KratosMultiphysics.Logger.PrintInfo("MMG Remeshing Process", "Remesh finished")
-
-    def _ErrorCalculation(self):
-        """ This method calculates the error in case an error estimation procedure is chosen
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-
-        # Initialize metric
-        self.initialize_metric.Execute()
-
-        KratosMultiphysics.Logger.PrintInfo("MMG Remeshing Process", "Calculating the metrics")
-        # Execute error computation
-        self.error_compute.Execute()
-        # Execute metric computation
-        self.metric_process.Execute()
-        self.error_ratio = self.main_model_part.ProcessInfo[KratosMultiphysics.ERROR_RATIO]
-
-    def _AuxiliarCallsBeforeRemesh(self):
-        """ This method is executed right before execute the remesh
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        pass
-
-    def _AuxiliarCallsAfterRemesh(self):
-        """ This method is executed right after execute the remesh
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        pass
-
-    def _GenerateErrorProcess(self):
-        """ This method creates an erro process to compute the metric
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        # Check dependencies
-        if not structural_dependencies:
-            raise Exception("You need to compile the StructuralMechanicsApplication in order to use this criteria")
-
-        # We compute the error
-        error_compute_parameters = KratosMultiphysics.Parameters("""{}""")
-        error_compute_parameters.AddValue("stress_vector_variable", self.settings["error_strategy_parameters"]["compute_error_extra_parameters"]["stress_vector_variable"])
-        error_compute_parameters.AddValue("echo_level", self.settings["echo_level"])
-        if self.domain_size == 2:
-            return StructuralMechanicsApplication.SPRErrorProcess2D(self.main_model_part, error_compute_parameters)
-        else:
-            return StructuralMechanicsApplication.SPRErrorProcess3D(self.main_model_part, error_compute_parameters)
-
-    def __execute_remesh(self):
-        """ This method returns if we need to execute the remeshing
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        execute_remesh = False
-        if self.remesh_control_type == "step":
-            self.step += 1
-            if self.step_frequency > 0:
-                if self.main_model_part.ProcessInfo[KratosMultiphysics.STEP] >= self.initial_step:
-                    if not self.initial_step_done:
-                        execute_remesh = True
-                    else:
-                        if self.step >= self.step_frequency:
-                            execute_remesh = True
-        elif self.remesh_control_type == "time":
-            delta_time = self.main_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
-            self.time += delta_time
-            remesh_delta_time = self.__get_delta_time()
-            if remesh_delta_time > 0:
-                if not self.initial_step_done:
-                    execute_remesh = True
-                else:
-                    if self.time >= remesh_delta_time:
-                        execute_remesh = True
-        else:
-            raise Exception("{0} Error: remesh_control_type is unreadable".format(self.remesh_control_type))
-
-        return execute_remesh
-
-    def __get_delta_time(self):
-        """ This method returns the delta time for time managed remeshing
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        if self.time_stepping.Has("time_step"):
-            delta_time = self.time_stepping["time_step"].GetDouble()
-            return delta_time
-        elif self.time_stepping.Has("time_step_intervals"):
-            current_time = self.main_model_part.ProcessInfo[KratosMultiphysics.TIME]
-            for key in self.time_stepping["time_step_intervals"].keys():
-                interval_settings = self.time_stepping["time_step_intervals"][key]
-                interval = KratosMultiphysics.IntervalUtility(interval_settings)
-
-                # Getting the time step of the interval
-                if interval.IsInInterval(current_time):
-                    return interval_settings["time_step"].GetDouble()
-            # If we arrive here we raise an error because the intervals are not well defined
-            raise Exception("::[MmgProcess]:: Time stepping not well defined!")
-        else:
-            raise Exception("::[MmgProcess]:: Time stepping not defined!")
-
-    def __generate_boolean_list_from_input(self,param):
-      '''Parse a list of booleans from input.'''
-      # At least verify that the input is an array
-      if not param.IsArray():
-          raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
-
-      # Retrieve the boolean from the arrays
-      boolean_list = []
-
-      for i in range( 0,param.size()):
-          boolean_list.append(param[i].GetBool())
-
-      return boolean_list
-
-    def __generate_double_list_from_input(self,param):
-      '''Parse a list of doubles from input.'''
-      # At least verify that the input is an array
-      if not param.IsArray():
-          raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
-
-      # Retrieve the boolean from the arrays
-      double_list = []
-
-      for i in range( 0,param.size()):
-          double_list.append(param[i].GetDouble())
-
-      return double_list
-
-    def __generate_string_list_from_input(self,param):
-      '''Parse a list of strings from input.'''
-      # At least verify that the input is an array
-      if not param.IsArray():
-          raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
-
-      # Retrieve the boolean from the arrays
-      string_list = []
-
-      for i in range( 0,param.size()):
-          string_list.append(param[i].GetString())
-
-      return string_list
-
-    def __generate_submodelparts_list_from_input(self,param):
-        '''Parse a list of variables from input.'''
-        # At least verify that the input is a string
-        if not param.IsArray():
-            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
-
-        # Retrieve submodelparts name from input (a string) and request the corresponding C++ object to the kernel
-        return [self.main_model_part.GetSubModelPart(sub_model_part_name) for sub_model_part_name in param.GetStringArray()]
-
-    def __generate_variable_list_from_input(self,param):
-        '''Parse a list of variables from input.'''
-        # At least verify that the input is a string
-        if not param.IsArray():
-            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
-
-        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
-        variable_list = []
-        variable_types = []
-        param_names = param.GetStringArray()
-        for variable_name in param_names:
-            varriable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
-            if varriable_type == "Double" or varriable_type == "Component":
-                variable_list.append(KratosMultiphysics.KratosGlobals.GetVariable(variable_name))
-                variable_types.append(1)
-            else:
-                variable_list.append( KratosMultiphysics.KratosGlobals.GetVariable( variable_name + "_X" ))
-                variable_list.append( KratosMultiphysics.KratosGlobals.GetVariable( variable_name + "_Y" ))
-                if self.domain_size == 3:
-                    variable_list.append( KratosMultiphysics.KratosGlobals.GetVariable( variable_name + "_Z" ))
-                    variable_types.append(3)
-                else:
-                    variable_types.append(2)
-
-        return variable_list, variable_types
-
-    def __list_extender(self, values, repetition_list):
-        '''Extends the list depending of a repetition parameter'''
-
-        aux_list = []
-        for value, repetition in zip(values, repetition_list):
-            for i in range(repetition):
-                aux_list.append(value)
-
-        return aux_list
-
-    def _debug_output_gid(self, label, name, prefix):
-        '''Debug postprocess with GiD.'''
-        gid_mode = KratosMultiphysics.GiDPostMode.GiD_PostBinary
-        singlefile = KratosMultiphysics.MultiFileFlag.SingleFile
-        deformed_mesh_flag = KratosMultiphysics.WriteDeformedMeshFlag.WriteUndeformed
-        write_conditions = KratosMultiphysics.WriteConditionsFlag.WriteConditions
-        gid_io = KratosMultiphysics.GidIO(prefix + "REMESHING_" + name + "_STEP_" + str(label), gid_mode, singlefile, deformed_mesh_flag, write_conditions)
-
-        gid_io.InitializeMesh(label)
-        gid_io.WriteMesh(self.main_model_part.GetMesh())
-        gid_io.FinalizeMesh()
-        gid_io.InitializeResults(label, self.main_model_part.GetMesh())
-        if self.settings["framework"].GetString() ==  "Lagrangian":
-            gid_io.WriteNodalResults(KratosMultiphysics.DISPLACEMENT, self.main_model_part.Nodes, label, 0)
-            for var in self.internal_variable_interpolation_list:
-                gid_io.PrintOnGaussPoints(var, self.main_model_part, label)
-        else:
-            gid_io.WriteNodalResults(KratosMultiphysics.VELOCITY, self.main_model_part.Nodes, label, 0)
-
-        if self.strategy == "levelset":
-            gid_io.WriteNodalResults(self.scalar_variable, self.main_model_part.Nodes, label, 0)
-            gid_io.WriteNodalResults(self.gradation_value, self.main_model_part.Nodes, label, 0)
-        elif self.strategy == "hessian":
-            variables = self.settings["hessian_strategy_parameters"]["metric_variable"].GetStringArray()
-            for i in range(len(variables)):
-                aux_var = KratosMultiphysics.KratosGlobals.GetVariable( variables[i] )
-                if self.settings["hessian_strategy_parameters"]["non_historical_metric_variable"][i].GetBool():
-                    gid_io.WriteNodalResultsNonHistorical(aux_var, self.main_model_part.Nodes, label)
-                else:
-                    gid_io.WriteNodalResults(aux_var, self.main_model_part.Nodes, label, 0)
-
-        gid_io.FinalizeResults()
-
-        #raise NameError("DEBUG")
-
-    def _debug_output_vtk(self, label, name, prefix):
-        '''Debug postprocess with VTK.'''
-        vtk_settings = KratosMultiphysics.Parameters("""{
-            "model_part_name"                    : "PLEASE_SPECIFY_MODEL_PART_NAME",
-            "file_format"                        : "ascii",
-            "output_precision"                   : 7,
-            "output_control_type"                : "step",
-            "output_frequency"                   : 1.0,
-            "output_sub_model_parts"             : false,
-            "custom_name_prefix"                 : "",
-            "save_output_files_in_folder"        : false,
-            "nodal_solution_step_data_variables" : [],
-            "nodal_data_value_variables"         : [],
-            "element_data_value_variables"       : [],
-            "condition_data_value_variables"     : [],
-            "gauss_point_variables"              : []
-        }""")
-
-        vtk_settings["custom_name_prefix"].SetString(prefix + "REMESHING_" + name + "_STEP_" + str(label) + "_")
-        if self.settings["framework"].GetString() ==  "Lagrangian":
-            vtk_settings["nodal_solution_step_data_variables"].Append("DISPLACEMENT")
-            for var in self.internal_variable_interpolation_list:
-                vtk_settings["gauss_point_variables"].Append(var.Name())
-        else:
-            vtk_settings["nodal_solution_step_data_variables"].Append("VELOCITY")
-
-        if self.strategy == "levelset":
-            vtk_settings["nodal_solution_step_data_variables"].Append(self.scalar_variable.Name())
-            vtk_settings["nodal_solution_step_data_variables"].Append(self.gradation_value.Name())
-        elif self.strategy == "hessian":
-            variables = self.settings["hessian_strategy_parameters"]["metric_variable"].GetStringArray()
-            for i in range(len(variables)):
-                aux_var = KratosMultiphysics.KratosGlobals.GetVariable( variables[i] )
-                if self.settings["hessian_strategy_parameters"]["non_historical_metric_variable"][i].GetBool():
-                    vtk_settings["nodal_data_value_variables"].Append(variables[i])
-                else:
-                    vtk_settings["nodal_solution_step_data_variables"].Append(variables[i])
-
-        vtk_io = KratosMultiphysics.VtkOutput(self.main_model_part, vtk_settings)
-        vtk_io.PrintOutput()
-
-        #raise NameError("DEBUG")
-
-def _linear_interpolation(x, x_list, y_list):
-    tb = KratosMultiphysics.PiecewiseLinearTable()
-    for x,y in zip(x_list, y_list):
-        tb.AddRow(x, y)
-
-    return tb.GetNearestValue(x)
-
-def _normpdf(x, mean, sd):
-    dir_path = os.path.dirname(os.path.realpath(__file__))
-    data = json_utilities.read_external_json(dir_path+"/normal_distribution.json")
-    z = (x-mean)/sd
-    z_list = data["Z"]
-    prob_list = data["Prob"]
-    if (z > 0):
-        prob = _linear_interpolation(z, z_list, prob_list)
-    else:
-        prob = 1.0 - _linear_interpolation(-z, z_list, prob_list)
-    return prob
-
-
-def _normvalf(prob, mean, sd):
-    dir_path = os.path.dirname(os.path.realpath(__file__))
-    data = json_utilities.read_external_json(dir_path+"/normal_distribution.json")
-    z_list = data["Z"]
-    prob_list = data["Prob"]
-    if (prob >= 0.5):
-        z = _linear_interpolation(prob, prob_list, z_list)
-    else:
-        z = - _linear_interpolation(1.0 - prob, prob_list, z_list)
-    x = z * sd + mean
-    return x
-
-def _check_strategy(strategy):
-    strategies_list = [
-        "hessian",
-        "levelset",
-        "optimization",
-        "superconvergent_patch_recovery",
-        "spr"
-    ]
-    if strategy in strategies_list:
-        return strategy
-    elif strategy.lower() in strategies_list:
-        depr_msg  = 'The input strategy string is not in lower case letters. '
-        depr_msg += 'Please change it from "' + strategy + '" to "' +  strategy.lower() + '"'
-        KratosMultiphysics.Logger.PrintWarning('DEPRECATION-WARNING', depr_msg)
-        return strategy.lower()
-    else:
-        err_msg  = 'The input strategy "' + strategy + '" does not exit. The available options are:\n'
-        err_msg  += 'Available strategies: '
-        for avail_strategy in strategies_list:
-            err_msg += '"'+avail_strategy+'" '
+# Importing the Kratos Library
+import KratosMultiphysics as KratosMultiphysics
+import KratosMultiphysics.MeshingApplication as MeshingApplication
+
+try:
+    import KratosMultiphysics.StructuralMechanicsApplication as StructuralMechanicsApplication
+    structural_dependencies = True
+except ImportError as e:
+    structural_dependencies = False
+
+# Some Kratos dependencies
+from KratosMultiphysics import kratos_utilities
+from KratosMultiphysics import json_utilities
+
+# Some python dependencies
+import os
+import statistics as stat
+
+def Factory(settings, Model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return MmgProcess(Model, settings["Parameters"])
+
+class MmgProcess(KratosMultiphysics.Process):
+    """This process remeshes using MMG library. This process uses different utilities and processes
+
+    Only the member variables listed below should be accessed directly.
+
+    Public member variables:
+    Model -- the container of the different model parts.
+    settings -- Kratos parameters containing solver settings.
+    """
+
+    def __init__(self, Model, settings ):
+        """ The default constructor of the class
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        Model -- the container of the different model parts.
+        settings -- Kratos parameters containing solver settings.
+        """
+
+        KratosMultiphysics.Process.__init__(self)
+
+        ## Settings string in json format
+        default_parameters = KratosMultiphysics.Parameters("""
+        {
+            "help"                             : "This process remeshes using MMG library. This process uses different utilities and processes",
+            "mesh_id"                          : 0,
+            "filename"                         : "out",
+            "model_part_name"                  : "PLEASE_SPECIFY_MODEL_PART_NAME",
+            "blocking_threshold_size"          : false,
+            "threshold_sizes"                  : {
+                "minimal_size"                     : 0.1,
+                "maximal_size"                     : 10.0
+            },
+            "strategy"                         : "levelset",
+            "level_set_strategy_parameters"    : {
+                "scalar_variable"                  : "DISTANCE",
+                "gradient_variable"                : "DISTANCE_GRADIENT"
+            },
+            "error_strategy_parameters"        : {
+                "compute_error_extra_parameters"     : {
+                    "stress_vector_variable"              : "CAUCHY_STRESS_VECTOR",
+                    "penalty_normal"                      : 1.0e4,
+                    "penalty_tangential"                  : 1.0e4
+                },
+                "error_metric_parameters"            : {
+                    "error_threshold"                       : 1.0e-4,
+                    "interpolation_error"                   : 0.04
+                },
+                "set_target_number_of_elements"       : false,
+                "target_number_of_elements"           : 1000,
+                "perform_nodal_h_averaging"           : false
+            },
+            "discretization_type"                  : "Standard",
+            "isosurface_parameters"                : {
+                "isosurface_variable"              : "DISTANCE",
+                "invert_value"                     : false,
+                "nonhistorical_variable"           : false,
+                "use_metric_field"                 : false,
+                "remove_internal_regions"          : false
+            },
+            "framework"                            : "Eulerian",
+            "internal_variables_parameters"        : {
+                "allocation_size"                      : 1000,
+                "bucket_size"                          : 4,
+                "search_factor"                        : 2,
+                "interpolation_type"                   : "LST",
+                "internal_variable_interpolation_list" :[]
+            },
+            "hessian_strategy_parameters"              :{
+                "metric_variable"                  : ["DISTANCE"],
+                "non_historical_metric_variable"   : [false],
+                "normalization_factor"             : [1.0],
+                "normalization_alpha"              : [0.0],
+                "normalization_method"             : ["constant"],
+                "estimate_interpolation_error"     : false,
+                "interpolation_error"              : 0.04,
+                "mesh_dependent_constant"          : 0.28125
+            },
+            "enforce_current"                  : true,
+            "remesh_control_type"              : "step",
+            "initial_step"                     : 1,
+            "step_frequency"                   : 0,
+            "interval"                         : [0.0, 1e30],
+            "time_stepping"                    : {},
+            "automatic_remesh"                 : true,
+            "automatic_remesh_parameters"      : {
+                "automatic_remesh_type"            : "Ratio",
+                "min_size_ratio"                   : 1.0,
+                "max_size_ratio"                   : 3.0,
+                "refer_type"                       : "Mean",
+                "min_size_current_percentage"      : 50.0,
+                "max_size_current_percentage"      : 98.0
+            },
+            "initial_remeshing"                : false,
+            "fix_contour_model_parts"          : [],
+            "fix_conditions_model_parts"       : [],
+            "fix_elements_model_parts"         : [],
+            "force_min"                        : false,
+            "minimal_size"                     : 0.1,
+            "force_max"                        : false,
+            "maximal_size"                     : 10.0,
+            "sizing_parameters"                : {
+                "reference_variable_name"          : "DISTANCE",
+                "boundary_layer_max_distance"      : 1.0,
+                "interpolation"                    : "constant"
+            },
+            "advanced_parameters"                  : {
+                "force_hausdorff_value"            : false,
+                "hausdorff_value"                  : 0.0001,
+                "no_move_mesh"                     : false,
+                "no_surf_mesh"                     : false,
+                "no_insert_mesh"                   : false,
+                "no_swap_mesh"                     : false,
+                "normal_regularization_mesh"       : false,
+                "deactivate_detect_angle"          : false,
+                "force_angle_detection_value"      : false,
+                "angle_detection_value"            : 45.0,
+                "force_gradation_value"            : false,
+                "mesh_optimization_only"           : false,
+                "gradation_value"                  : 1.3,
+                "local_entity_parameters_list"     : []
+            },
+            "anisotropy_remeshing"                 : true,
+            "enforce_anisotropy_relative_variable" : false,
+            "anisotropy_parameters":{
+                "reference_variable_name"          : "DISTANCE",
+                "hmin_over_hmax_anisotropic_ratio" : 0.01,
+                "boundary_layer_max_distance"      : 1.0,
+                "boundary_layer_min_size_ratio"    : 2.0,
+                "interpolation"                    : "Linear"
+            },
+            "collapse_prisms_elements"         : false,
+            "save_external_files"              : false,
+            "save_colors_files"                : false,
+            "save_mdpa_file"                   : false,
+            "remesh_at_finalize"               : false,
+            "output_final_mesh"                : false,
+            "sub_model_part_names_to_remove"   : [],
+            "output_mesh_file_name"            : "final_refined_mesh",
+            "max_number_of_searchs"            : 1000,
+            "preserve_flags"                   : true,
+            "interpolate_nodal_values"         : true,
+            "interpolate_non_historical"       : true,
+            "use_mapper_if_available"          : false,
+            "mapping_parameters"               : {
+                "mapper_type"                      : "nearest_element",
+                "echo_level"                       : 0,
+                "search_settings" : {
+                    "max_num_search_iterations"    : 8,
+                    "echo_level"                   : 0
+                }
+            }, 
+            "extrapolate_contour_values"       : true,
+            "surface_elements"                 : false,
+            "search_parameters"                : {
+                "allocation_size"                  : 1000,
+                "bucket_size"                      : 4,
+                "search_factor"                    : 2.0
+            },
+            "debug_mode"                       : "",
+            "debug_result_mesh"                : false,
+            "initialize_entities"              : true,
+            "echo_level"                       : 3
+        }
+        """)
+
+        # Identify the dimension first
+        if not settings.Has("model_part_name"):
+            settings.AddValue("model_part_name", default_parameters["model_part_name"])
+
+        # Getting model part and working dimension
+        self.main_model_part = Model[settings["model_part_name"].GetString()]
+        self.domain_size = self.main_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
+        self.is_surface = False
+        if self.domain_size == 3:
+            for elem in self.main_model_part.Elements:
+                geom = elem.GetGeometry()
+                if geom.WorkingSpaceDimension() != geom.LocalSpaceDimension():
+                    self.is_surface = True
+                break
+
+        # The mesh dependent constant depends on dimension
+        if self.domain_size == 2:
+            default_parameters["hessian_strategy_parameters"]["mesh_dependent_constant"].SetDouble(2.0/9.0)
+        else:
+            default_parameters["hessian_strategy_parameters"]["mesh_dependent_constant"].SetDouble(9.0/32.0)
+
+        # Assign this here since it will change the "interval" prior to validation
+        self.interval = KratosMultiphysics.IntervalUtility(settings)
+
+        # Time stepping
+        if not hasattr(self, 'time_stepping'):
+            self.time_stepping = KratosMultiphysics.Parameters("""{}""")
+            if settings.Has("time_stepping"):
+                self.time_stepping = settings["time_stepping"].Clone()
+                settings.RemoveValue("time_stepping")
+
+        # Overwrite the default settings with user-provided parameters
+        self.settings = settings
+        self.settings.RecursivelyValidateAndAssignDefaults(default_parameters)
+
+        # Getting some settings
+        self.strategy = _check_strategy(self.settings["strategy"].GetString())
+        self.enforce_current = self.settings["enforce_current"].GetBool()
+        self.initial_remeshing = self.settings["initial_remeshing"].GetBool()
+        self.remesh_control_type = self.settings["remesh_control_type"].GetString()
+        self.initial_step = self.settings["initial_step"].GetInt()
+        self.step_frequency = self.settings["step_frequency"].GetInt()
+        self.settings["surface_elements"].SetBool(self.is_surface)
+
+        # Setting initial_step_done here
+        self.initial_step_done = False
+
+        # Initialize flag
+        self.remesh_executed = False
+
+    def ExecuteInitialize(self):
+        """ This method is executed at the begining to initialize the process
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+
+        # Calculate NODAL_H
+        KratosMultiphysics.VariableUtils().SetNonHistoricalVariable(KratosMultiphysics.NODAL_H, 0.0, self.main_model_part.Nodes)
+        KratosMultiphysics.VariableUtils().SetNonHistoricalVariable(KratosMultiphysics.NODAL_AREA, 0.0, self.main_model_part.Nodes)
+        self.find_nodal_h = KratosMultiphysics.FindNodalHNonHistoricalProcess(self.main_model_part)
+        self.find_nodal_h.Execute()
+
+        # Calculate the parameters of automatic remeshing
+        if self.settings["automatic_remesh"].GetBool():
+            nodal_h_values = []
+            for node in self.main_model_part.Nodes:
+                nodal_h_values.append(node.GetValue(KratosMultiphysics.NODAL_H))
+
+            # Calculate the minimum size
+            if self.settings["automatic_remesh_parameters"]["automatic_remesh_type"].GetString() == "Ratio":
+                # NOTE: For mode: https://docs.python.org/3/library/statistics.html
+                if self.settings["automatic_remesh_parameters"]["refer_type"].GetString() == "Mean":
+                    ref = stat.mean(nodal_h_values)
+                elif self.settings["automatic_remesh_parameters"]["refer_type"].GetString() == "Median":
+                    ref = stat.median(nodal_h_values)
+
+                self.settings["minimal_size"].SetDouble(ref * (self.settings["automatic_remesh_parameters"]["min_size_ratio"].GetDouble()))
+                self.settings["maximal_size"].SetDouble(ref * (self.settings["automatic_remesh_parameters"]["max_size_ratio"].GetDouble()))
+            elif self.settings["automatic_remesh_parameters"]["automatic_remesh_type"].GetString() == "Percentage":
+                mean = stat.mean(nodal_h_values)
+                stdev = stat.stdev(nodal_h_values)
+                prob = (self.settings["automatic_remesh_parameters"]["min_size_current_percentage"].GetDouble())/100
+                self.settings["minimal_size"].SetDouble(_normvalf(prob, mean, stdev)) # Using normal normal distribution to get the minimal size as a stadistical meaninful value
+
+                prob = (self.settings["automatic_remesh_parameters"]["max_size_current_percentage"].GetDouble())/100
+                self.settings["maximal_size"].SetDouble(_normvalf(prob, mean, stdev)) # Using normal normal distribution to get the maximal size as a stadistical meaninful value
+
+            # We deactivate, so it doesn't recalculate each initialization
+            self.settings["automatic_remesh"].SetBool(False)
+
+        ## We print the parameters considered
+        KratosMultiphysics.Logger.PrintInfo("MINIMAL SIZE: ", "{:.2e}".format(self.settings["minimal_size"].GetDouble()))
+        KratosMultiphysics.Logger.PrintInfo("MAXIMAL SIZE: ", "{:.2e}".format(self.settings["maximal_size"].GetDouble()))
+
+        # Anisotropic remeshing parameters
+        self.anisotropy_remeshing = self.settings["anisotropy_remeshing"].GetBool()
+        if self.anisotropy_remeshing:
+            if self.settings["automatic_remesh"].GetBool():
+                self.settings["anisotropy_parameters"]["boundary_layer_max_distance"].SetDouble(self.settings["minimal_size"].GetDouble() * self.settings["anisotropy_parameters"]["boundary_layer_min_size_ratio"].GetDouble())
+
+        # Select the remeshing strategy
+        if self.strategy == "levelset":
+            self.scalar_variable = KratosMultiphysics.KratosGlobals.GetVariable( self.settings["level_set_strategy_parameters"]["scalar_variable"].GetString() )
+            self.gradient_variable = KratosMultiphysics.KratosGlobals.GetVariable( self.settings["level_set_strategy_parameters"]["gradient_variable"].GetString() )
+        elif self.strategy == "hessian":
+            self.metric_variables, variable_types = self.__generate_variable_list_from_input(self.settings["hessian_strategy_parameters"]["metric_variable"])
+            self.non_historical_metric_variable = self.__generate_boolean_list_from_input(self.settings["hessian_strategy_parameters"]["non_historical_metric_variable"])
+            self.non_historical_metric_variable = self.__list_extender(self.non_historical_metric_variable, variable_types)
+            self.normalization_factor = self.__generate_double_list_from_input(self.settings["hessian_strategy_parameters"]["normalization_factor"])
+            self.normalization_factor = self.__list_extender(self.normalization_factor, variable_types)
+            self.normalization_alpha = self.__generate_double_list_from_input(self.settings["hessian_strategy_parameters"]["normalization_alpha"])
+            self.normalization_alpha = self.__list_extender(self.normalization_alpha, variable_types)
+            self.normalization_method = self.__generate_string_list_from_input(self.settings["hessian_strategy_parameters"]["normalization_method"])
+            self.normalization_method = self.__list_extender(self.normalization_method, variable_types)
+            len_metric_variables = len(self.metric_variables)
+            len_non_historical_metric_variable = len(self.non_historical_metric_variable)
+            if len_metric_variables > len_non_historical_metric_variable:
+                for i in range(len_non_historical_metric_variable, len_metric_variables):
+                    self.non_historical_metric_variable.append(False)
+            len_normalization_factor = len(self.normalization_factor)
+            if len_metric_variables > len_normalization_factor:
+                for i in range(len_normalization_factor, len_metric_variables):
+                    self.normalization_factor.append(1.0)
+            len_normalization_alpha = len(self.normalization_alpha)
+            if len_metric_variables > len_normalization_alpha:
+                for i in range(len_normalization_alpha, len_metric_variables):
+                    self.normalization_alpha.append(0.0)
+            len_normalization_method = len(self.normalization_method)
+            if len_metric_variables > len_normalization_method:
+                for i in range(len_normalization_method, len_metric_variables):
+                    self.normalization_method.append("constant")
+            mesh_dependent_constant = self.settings["hessian_strategy_parameters"]["mesh_dependent_constant"].GetDouble()
+            if mesh_dependent_constant == 0.0:
+                self.settings["hessian_strategy_parameters"]["mesh_dependent_constant"].SetDouble(0.5 * (self.domain_size/(self.domain_size + 1))**2.0)
+        elif self.strategy == "superconvergent_patch_recovery" or self.strategy == "spr":
+            self.error_threshold = self.settings["error_strategy_parameters"]["error_metric_parameters"]["error_threshold"].GetDouble()
+            self.error_ratio = 0
+
+        self.internal_variable_interpolation_list = kratos_utilities.GenerateVariableListFromInput(self.settings["internal_variables_parameters"]["internal_variable_interpolation_list"])
+
+        # Model parts to fix the nodes
+        fix_contour_model_parts = self.__generate_submodelparts_list_from_input(self.settings["fix_contour_model_parts"])
+
+        # Setting flag BLOCKED to the non nodes
+        for submodelpart in fix_contour_model_parts:
+            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.BLOCKED, True, submodelpart.Nodes)
+
+        # Model parts to fix the conditions
+        fix_conditions_model_parts = self.__generate_submodelparts_list_from_input(self.settings["fix_conditions_model_parts"])
+
+        # Setting flag BLOCKED to the non conditions
+        for submodelpart in fix_conditions_model_parts:
+            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.BLOCKED, True, submodelpart.Conditions)
+
+        # Model parts to fix the nodes
+        fix_elements_model_parts = self.__generate_submodelparts_list_from_input(self.settings["fix_elements_model_parts"])
+
+        # Setting flag BLOCKED to the non elements
+        for submodelpart in fix_elements_model_parts:
+            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.BLOCKED, True, submodelpart.Elements)
+
+        if self.strategy == "levelset":
+            self._CreateGradientProcess()
+
+        if self.domain_size == 2:
+            self.initialize_metric = MeshingApplication.MetricFastInit2D(self.main_model_part)
+        else:
+            self.initialize_metric = MeshingApplication.MetricFastInit3D(self.main_model_part)
+
+        self.initialize_metric.Execute()
+
+        self._CreateMetricsProcess()
+
+        mmg_parameters = KratosMultiphysics.Parameters("""{"force_sizes":{}}""")
+        mmg_parameters.AddValue("filename",self.settings["filename"])
+        mmg_parameters.AddValue("framework",self.settings["framework"])
+        mmg_parameters.AddValue("discretization_type",self.settings["discretization_type"])
+        mmg_parameters.AddValue("isosurface_parameters",self.settings["isosurface_parameters"])
+        mmg_parameters.AddValue("internal_variables_parameters",self.settings["internal_variables_parameters"])
+        mmg_parameters.AddValue("collapse_prisms_elements",self.settings["collapse_prisms_elements"])
+        mmg_parameters.AddValue("save_external_files",self.settings["save_external_files"])
+        mmg_parameters.AddValue("save_colors_files",self.settings["save_colors_files"])
+        mmg_parameters.AddValue("save_mdpa_file",self.settings["save_mdpa_file"])
+        mmg_parameters.AddValue("max_number_of_searchs",self.settings["max_number_of_searchs"])
+        mmg_parameters.AddValue("preserve_flags",self.settings["preserve_flags"])
+        mmg_parameters.AddValue("interpolate_nodal_values",self.settings["interpolate_nodal_values"])
+        mmg_parameters.AddValue("interpolate_non_historical",self.settings["interpolate_non_historical"])
+        mmg_parameters.AddValue("extrapolate_contour_values",self.settings["extrapolate_contour_values"])
+        mmg_parameters.AddValue("search_parameters",self.settings["search_parameters"])
+        mmg_parameters["force_sizes"].AddValue("force_min",self.settings["force_min"])
+        mmg_parameters["force_sizes"].AddValue("minimal_size",self.settings["minimal_size"])
+        mmg_parameters["force_sizes"].AddValue("force_max",self.settings["force_max"])
+        mmg_parameters["force_sizes"].AddValue("maximal_size",self.settings["maximal_size"])
+        mmg_parameters.AddValue("advanced_parameters",self.settings["advanced_parameters"])
+        mmg_parameters.AddValue("debug_result_mesh",self.settings["debug_result_mesh"])
+        mmg_parameters.AddValue("initialize_entities",self.settings["initialize_entities"])
+        mmg_parameters.AddValue("echo_level",self.settings["echo_level"])
+        if self.strategy == "optimization":
+            mmg_parameters["advanced_parameters"]["mesh_optimization_only"].SetBool(True)
+
+        if self.domain_size == 2:
+            self.mmg_process = MeshingApplication.MmgProcess2D(self.main_model_part, mmg_parameters)
+        else:
+            # Differentiate between 3D volumes and 3D surfaces
+            if self.is_surface:
+                self.mmg_process = MeshingApplication.MmgProcess3DSurfaces(self.main_model_part, mmg_parameters)
+            else:
+                self.mmg_process = MeshingApplication.MmgProcess3D(self.main_model_part, mmg_parameters)
+
+        # We reset the step and time
+        self.step = 0
+        self.time = 0.0
+
+        # We compute initial remeshing is desired
+        if self.initial_remeshing:
+            if not self.main_model_part.Is(KratosMultiphysics.MODIFIED):
+                self._ExecuteRefinement()
+            else:
+                self.main_model_part.Set(KratosMultiphysics.MODIFIED, False)
+
+    def ExecuteInitializeSolutionStep(self):
+        """ This method is executed in order to initialize the current step
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+
+        # If not previous remesh
+        if not self.remesh_executed:
+            if not self.initial_remeshing:
+                # We need to check if the model part has been modified recently
+                if self.main_model_part.Is(KratosMultiphysics.MODIFIED):
+                    self.main_model_part.Set(KratosMultiphysics.MODIFIED, False)
+                    self.step = 0  # Reset (just to be sure)
+                    self.time = 0.0  # Reset (just to be sure)
+                else:
+                    current_time = self.main_model_part.ProcessInfo[KratosMultiphysics.TIME]
+                    if self.interval.IsInInterval(current_time):
+                        # We remesh if needed
+                        if self.__execute_remesh():
+                            if self.strategy in ["hessian", "levelset", "optimization"]:
+                                if self.settings["blocking_threshold_size"].GetBool():
+                                    MeshingApplication.BlockThresholdSizeElements(self.main_model_part, self.settings["threshold_sizes"])
+                                self._ExecuteRefinement()
+                                self.initial_step_done = True
+                                self.step = 0  # Reset
+                                self.time = 0.0  # Reset
+
+    def ExecuteFinalize(self):
+        """ This method is executed in order to finalize the simulation and save the refined mesh in a new .mdpa file
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        remesh_at_finalize = self.settings["remesh_at_finalize"].GetBool()
+        output_final_mesh = self.settings["output_final_mesh"].GetBool()
+        output_mesh_file_name = self.settings["output_mesh_file_name"].GetString()
+        sub_model_part_names_to_remove = self.settings["sub_model_part_names_to_remove"].GetStringArray()
+        if remesh_at_finalize:
+            for sub_model_part_name in sub_model_part_names_to_remove:
+                if self.main_model_part.HasSubModelPart(sub_model_part_name):
+                    self.main_model_part.RemoveSubModelPart(sub_model_part_name)
+            self._ExecuteRefinement()
+        if output_final_mesh:
+            KratosMultiphysics.ModelPartIO(output_mesh_file_name, KratosMultiphysics.IO.WRITE | KratosMultiphysics.IO.MESH_ONLY).WriteModelPart(self.main_model_part)
+
+    def ExecuteFinalizeSolutionStep(self):
+        """ This method is executed in order to finalize the current step
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        if self.strategy == "superconvergent_patch_recovery" or self.strategy == "spr":
+            current_time = self.main_model_part.ProcessInfo[KratosMultiphysics.TIME]
+            if self.interval.IsInInterval(current_time):
+                if self.__execute_remesh():
+                    self._ErrorCalculation()
+
+                    if self.error_ratio > self.error_threshold:
+                        self._ExecuteRefinement()
+                        self.step = 0  # Reset
+                        self.time = 0.0  # Reset
+
+        # Reset flag
+        self.remesh_executed = False
+
+    def ExecuteBeforeOutputStep(self):
+        """ This method is executed right before the ouput process computation
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        if self.strategy == "superconvergent_patch_recovery" or self.strategy == "spr":
+            current_time = self.main_model_part.ProcessInfo[KratosMultiphysics.TIME]
+            if self.interval.IsInInterval(current_time):
+                self._ErrorCalculation()
+
+    def ExecuteAfterOutputStep(self):
+        """ This method is executed right after the ouput process computation
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        pass
+
+    def _CreateMetricsProcess(self):
+        """ This method is responsible to create the metrics of the process
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        self.metric_processes = []
+        if self.strategy == "levelset":
+            level_set_parameters = KratosMultiphysics.Parameters("""{}""")
+            level_set_parameters.AddValue("minimal_size",self.settings["minimal_size"])
+            level_set_parameters.AddValue("maximal_size",self.settings["maximal_size"])
+            level_set_parameters.AddValue("sizing_parameters",self.settings["sizing_parameters"])
+            level_set_parameters.AddValue("enforce_current",self.settings["enforce_current"])
+            level_set_parameters.AddValue("anisotropy_remeshing",self.settings["anisotropy_remeshing"])
+            level_set_parameters.AddValue("anisotropy_parameters",self.settings["anisotropy_parameters"])
+            level_set_parameters["anisotropy_parameters"].RemoveValue("boundary_layer_min_size_ratio")
+            if self.domain_size == 2:
+                self.metric_processes.append(MeshingApplication.ComputeLevelSetSolMetricProcess2D(self.main_model_part, self.gradient_variable, level_set_parameters))
+            else:
+                self.metric_processes.append(MeshingApplication.ComputeLevelSetSolMetricProcess3D(self.main_model_part, self.gradient_variable, level_set_parameters))
+
+        elif self.strategy == "hessian":
+            hessian_parameters = KratosMultiphysics.Parameters("""{}""")
+            hessian_parameters.AddValue("minimal_size",self.settings["minimal_size"])
+            hessian_parameters.AddValue("maximal_size",self.settings["maximal_size"])
+            hessian_parameters.AddValue("enforce_current",self.settings["enforce_current"])
+            hessian_parameters.AddValue("hessian_strategy_parameters",self.settings["hessian_strategy_parameters"])
+            hessian_parameters["hessian_strategy_parameters"].RemoveValue("metric_variable")
+            hessian_parameters["hessian_strategy_parameters"].RemoveValue("non_historical_metric_variable")
+            hessian_parameters["hessian_strategy_parameters"].AddEmptyValue("non_historical_metric_variable")
+            hessian_parameters["hessian_strategy_parameters"].RemoveValue("normalization_factor")
+            hessian_parameters["hessian_strategy_parameters"].AddEmptyValue("normalization_factor")
+            hessian_parameters["hessian_strategy_parameters"].RemoveValue("normalization_alpha")
+            hessian_parameters["hessian_strategy_parameters"].AddEmptyValue("normalization_alpha")
+            hessian_parameters["hessian_strategy_parameters"].RemoveValue("normalization_method")
+            hessian_parameters["hessian_strategy_parameters"].AddEmptyValue("normalization_method")
+            hessian_parameters.AddValue("anisotropy_remeshing",self.settings["anisotropy_remeshing"])
+            hessian_parameters.AddValue("enforce_anisotropy_relative_variable",self.settings["enforce_anisotropy_relative_variable"])
+            hessian_parameters.AddValue("enforced_anisotropy_parameters",self.settings["anisotropy_parameters"])
+            hessian_parameters["enforced_anisotropy_parameters"].RemoveValue("boundary_layer_min_size_ratio")
+            for current_metric_variable, non_historical_metric_variable, normalization_factor, normalization_alpha, normalization_method in zip(self.metric_variables, self.non_historical_metric_variable, self.normalization_factor, self.normalization_alpha, self.normalization_method):
+                hessian_parameters["hessian_strategy_parameters"]["non_historical_metric_variable"].SetBool(non_historical_metric_variable)
+                hessian_parameters["hessian_strategy_parameters"]["normalization_factor"].SetDouble(normalization_factor)
+                hessian_parameters["hessian_strategy_parameters"]["normalization_alpha"].SetDouble(normalization_alpha)
+                hessian_parameters["hessian_strategy_parameters"]["normalization_method"].SetString(normalization_method)
+                self.metric_processes.append(MeshingApplication.ComputeHessianSolMetricProcess(self.main_model_part, current_metric_variable, hessian_parameters))
+        elif self.strategy == "superconvergent_patch_recovery" or self.strategy == "spr":
+            # Generate SPR process
+            self.error_compute = self._GenerateErrorProcess()
+
+            # Now we compute the metric
+            error_metric_parameters = KratosMultiphysics.Parameters("""{"error_strategy_parameters":{}}""")
+            error_metric_parameters.AddValue("minimal_size",self.settings["minimal_size"])
+            error_metric_parameters.AddValue("maximal_size",self.settings["maximal_size"])
+            error_metric_parameters["error_strategy_parameters"].AddValue("target_error",self.settings["error_strategy_parameters"]["error_metric_parameters"]["interpolation_error"])
+            error_metric_parameters["error_strategy_parameters"].AddValue("set_target_number_of_elements", self.settings["error_strategy_parameters"]["set_target_number_of_elements"])
+            error_metric_parameters["error_strategy_parameters"].AddValue("target_number_of_elements", self.settings["error_strategy_parameters"]["target_number_of_elements"])
+            error_metric_parameters["error_strategy_parameters"].AddValue("perform_nodal_h_averaging", self.settings["error_strategy_parameters"]["perform_nodal_h_averaging"])
+            error_metric_parameters.AddValue("echo_level", self.settings["echo_level"])
+
+            if self.domain_size == 2:
+                self.metric_process = MeshingApplication.MetricErrorProcess2D(self.main_model_part, error_metric_parameters)
+            else:
+                self.metric_process = MeshingApplication.MetricErrorProcess3D(self.main_model_part, error_metric_parameters)
+
+    def _CreateGradientProcess(self):
+        """ This method is responsible of create the gradients for the level-set process
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        # We compute the scalar value gradient
+        if self.domain_size == 2:
+            self.local_gradient = KratosMultiphysics.ComputeNodalGradientProcess2D(self.main_model_part, self.scalar_variable, self.gradient_variable, KratosMultiphysics.NODAL_AREA)
+        else:
+            self.local_gradient = KratosMultiphysics.ComputeNodalGradientProcess3D(self.main_model_part, self.scalar_variable, self.gradient_variable, KratosMultiphysics.NODAL_AREA)
+
+    def _ExecuteRefinement(self):
+        """ This method is the one responsible to execute the remeshing
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        if self.strategy == "levelset":
+            # Calculate the gradient
+            self.local_gradient.Execute()
+
+        # Recalculate NODAL_H
+        self.find_nodal_h.Execute()
+
+        # Initialize metric
+        if self.strategy == "hessian" or self.strategy == "levelset":
+            self.initialize_metric.Execute()
+
+        KratosMultiphysics.Logger.PrintInfo("MMG Remeshing Process", "Calculating the metrics")
+        # Execute metric computation
+        for metric_process in self.metric_processes:
+            metric_process.Execute()
+
+        # Debug before remesh
+        if self.settings["debug_mode"].GetString() == "GiD": # GiD
+            self._debug_output_gid(self.main_model_part.ProcessInfo[KratosMultiphysics.STEP], "", "BEFORE_")
+        elif self.settings["debug_mode"].GetString() == "VTK": # VTK
+            self._debug_output_vtk(self.main_model_part.ProcessInfo[KratosMultiphysics.STEP], "", "BEFORE_")
+
+        # Execute before remesh
+        self._AuxiliarCallsBeforeRemesh()
+
+        # Actually remesh
+        KratosMultiphysics.Logger.PrintInfo("MMG Remeshing Process", "Remeshing")
+        self.mmg_process.Execute()
+
+        # Execute after remesh
+        self._AuxiliarCallsAfterRemesh()
+
+        # Debug after remesh
+        if self.settings["debug_mode"].GetString() == "GiD": # GiD
+            self._debug_output_gid(self.main_model_part.ProcessInfo[KratosMultiphysics.STEP], "", "AFTER_")
+        elif self.settings["debug_mode"].GetString() == "VTK": # VTK
+            self._debug_output_vtk(self.main_model_part.ProcessInfo[KratosMultiphysics.STEP], "", "AFTER_")
+
+        if self.strategy == "levelset":
+            self.local_gradient.Execute() # Recalculate gradient after remeshing
+
+        # Recalculate NODAL_H
+        self.find_nodal_h.Execute()
+
+        # We need to set that the model part has been modified (later on we will act in consequence)
+        self.main_model_part.Set(KratosMultiphysics.MODIFIED, True)
+
+        # Deactivate to avoid remesh again
+        self.remesh_executed = True
+
+        KratosMultiphysics.Logger.PrintInfo("MMG Remeshing Process", "Remesh finished")
+
+    def _ErrorCalculation(self):
+        """ This method calculates the error in case an error estimation procedure is chosen
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+
+        # Initialize metric
+        self.initialize_metric.Execute()
+
+        KratosMultiphysics.Logger.PrintInfo("MMG Remeshing Process", "Calculating the metrics")
+        # Execute error computation
+        self.error_compute.Execute()
+        # Execute metric computation
+        self.metric_process.Execute()
+        self.error_ratio = self.main_model_part.ProcessInfo[KratosMultiphysics.ERROR_RATIO]
+
+    def _AuxiliarCallsBeforeRemesh(self):
+        """ This method is executed right before execute the remesh
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        pass
+
+    def _AuxiliarCallsAfterRemesh(self):
+        """ This method is executed right after execute the remesh
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        pass
+
+    def _GenerateErrorProcess(self):
+        """ This method creates an erro process to compute the metric
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        # Check dependencies
+        if not structural_dependencies:
+            raise Exception("You need to compile the StructuralMechanicsApplication in order to use this criteria")
+
+        # We compute the error
+        error_compute_parameters = KratosMultiphysics.Parameters("""{}""")
+        error_compute_parameters.AddValue("stress_vector_variable", self.settings["error_strategy_parameters"]["compute_error_extra_parameters"]["stress_vector_variable"])
+        error_compute_parameters.AddValue("echo_level", self.settings["echo_level"])
+        if self.domain_size == 2:
+            return StructuralMechanicsApplication.SPRErrorProcess2D(self.main_model_part, error_compute_parameters)
+        else:
+            return StructuralMechanicsApplication.SPRErrorProcess3D(self.main_model_part, error_compute_parameters)
+
+    def __execute_remesh(self):
+        """ This method returns if we need to execute the remeshing
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        execute_remesh = False
+        if self.remesh_control_type == "step":
+            self.step += 1
+            if self.step_frequency > 0:
+                if self.main_model_part.ProcessInfo[KratosMultiphysics.STEP] >= self.initial_step:
+                    if not self.initial_step_done:
+                        execute_remesh = True
+                    else:
+                        if self.step >= self.step_frequency:
+                            execute_remesh = True
+        elif self.remesh_control_type == "time":
+            delta_time = self.main_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
+            self.time += delta_time
+            remesh_delta_time = self.__get_delta_time()
+            if remesh_delta_time > 0:
+                if not self.initial_step_done:
+                    execute_remesh = True
+                else:
+                    if self.time >= remesh_delta_time:
+                        execute_remesh = True
+        else:
+            raise Exception("{0} Error: remesh_control_type is unreadable".format(self.remesh_control_type))
+
+        return execute_remesh
+
+    def __get_delta_time(self):
+        """ This method returns the delta time for time managed remeshing
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        if self.time_stepping.Has("time_step"):
+            delta_time = self.time_stepping["time_step"].GetDouble()
+            return delta_time
+        elif self.time_stepping.Has("time_step_intervals"):
+            current_time = self.main_model_part.ProcessInfo[KratosMultiphysics.TIME]
+            for key in self.time_stepping["time_step_intervals"].keys():
+                interval_settings = self.time_stepping["time_step_intervals"][key]
+                interval = KratosMultiphysics.IntervalUtility(interval_settings)
+
+                # Getting the time step of the interval
+                if interval.IsInInterval(current_time):
+                    return interval_settings["time_step"].GetDouble()
+            # If we arrive here we raise an error because the intervals are not well defined
+            raise Exception("::[MmgProcess]:: Time stepping not well defined!")
+        else:
+            raise Exception("::[MmgProcess]:: Time stepping not defined!")
+
+    def __generate_boolean_list_from_input(self,param):
+      '''Parse a list of booleans from input.'''
+      # At least verify that the input is an array
+      if not param.IsArray():
+          raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
+
+      # Retrieve the boolean from the arrays
+      boolean_list = []
+
+      for i in range( 0,param.size()):
+          boolean_list.append(param[i].GetBool())
+
+      return boolean_list
+
+    def __generate_double_list_from_input(self,param):
+      '''Parse a list of doubles from input.'''
+      # At least verify that the input is an array
+      if not param.IsArray():
+          raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
+
+      # Retrieve the boolean from the arrays
+      double_list = []
+
+      for i in range( 0,param.size()):
+          double_list.append(param[i].GetDouble())
+
+      return double_list
+
+    def __generate_string_list_from_input(self,param):
+      '''Parse a list of strings from input.'''
+      # At least verify that the input is an array
+      if not param.IsArray():
+          raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
+
+      # Retrieve the boolean from the arrays
+      string_list = []
+
+      for i in range( 0,param.size()):
+          string_list.append(param[i].GetString())
+
+      return string_list
+
+    def __generate_submodelparts_list_from_input(self,param):
+        '''Parse a list of variables from input.'''
+        # At least verify that the input is a string
+        if not param.IsArray():
+            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
+
+        # Retrieve submodelparts name from input (a string) and request the corresponding C++ object to the kernel
+        return [self.main_model_part.GetSubModelPart(sub_model_part_name) for sub_model_part_name in param.GetStringArray()]
+
+    def __generate_variable_list_from_input(self,param):
+        '''Parse a list of variables from input.'''
+        # At least verify that the input is a string
+        if not param.IsArray():
+            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
+
+        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
+        variable_list = []
+        variable_types = []
+        param_names = param.GetStringArray()
+        for variable_name in param_names:
+            varriable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
+            if varriable_type == "Double" or varriable_type == "Component":
+                variable_list.append(KratosMultiphysics.KratosGlobals.GetVariable(variable_name))
+                variable_types.append(1)
+            else:
+                variable_list.append( KratosMultiphysics.KratosGlobals.GetVariable( variable_name + "_X" ))
+                variable_list.append( KratosMultiphysics.KratosGlobals.GetVariable( variable_name + "_Y" ))
+                if self.domain_size == 3:
+                    variable_list.append( KratosMultiphysics.KratosGlobals.GetVariable( variable_name + "_Z" ))
+                    variable_types.append(3)
+                else:
+                    variable_types.append(2)
+
+        return variable_list, variable_types
+
+    def __list_extender(self, values, repetition_list):
+        '''Extends the list depending of a repetition parameter'''
+
+        aux_list = []
+        for value, repetition in zip(values, repetition_list):
+            for i in range(repetition):
+                aux_list.append(value)
+
+        return aux_list
+
+    def _debug_output_gid(self, label, name, prefix):
+        '''Debug postprocess with GiD.'''
+        gid_mode = KratosMultiphysics.GiDPostMode.GiD_PostBinary
+        singlefile = KratosMultiphysics.MultiFileFlag.SingleFile
+        deformed_mesh_flag = KratosMultiphysics.WriteDeformedMeshFlag.WriteUndeformed
+        write_conditions = KratosMultiphysics.WriteConditionsFlag.WriteConditions
+        gid_io = KratosMultiphysics.GidIO(prefix + "REMESHING_" + name + "_STEP_" + str(label), gid_mode, singlefile, deformed_mesh_flag, write_conditions)
+
+        gid_io.InitializeMesh(label)
+        gid_io.WriteMesh(self.main_model_part.GetMesh())
+        gid_io.FinalizeMesh()
+        gid_io.InitializeResults(label, self.main_model_part.GetMesh())
+        if self.settings["framework"].GetString() ==  "Lagrangian":
+            gid_io.WriteNodalResults(KratosMultiphysics.DISPLACEMENT, self.main_model_part.Nodes, label, 0)
+            for var in self.internal_variable_interpolation_list:
+                gid_io.PrintOnGaussPoints(var, self.main_model_part, label)
+        else:
+            gid_io.WriteNodalResults(KratosMultiphysics.VELOCITY, self.main_model_part.Nodes, label, 0)
+
+        if self.strategy == "levelset":
+            gid_io.WriteNodalResults(self.scalar_variable, self.main_model_part.Nodes, label, 0)
+            gid_io.WriteNodalResults(self.gradation_value, self.main_model_part.Nodes, label, 0)
+        elif self.strategy == "hessian":
+            variables = self.settings["hessian_strategy_parameters"]["metric_variable"].GetStringArray()
+            for i in range(len(variables)):
+                aux_var = KratosMultiphysics.KratosGlobals.GetVariable( variables[i] )
+                if self.settings["hessian_strategy_parameters"]["non_historical_metric_variable"][i].GetBool():
+                    gid_io.WriteNodalResultsNonHistorical(aux_var, self.main_model_part.Nodes, label)
+                else:
+                    gid_io.WriteNodalResults(aux_var, self.main_model_part.Nodes, label, 0)
+
+        gid_io.FinalizeResults()
+
+        #raise NameError("DEBUG")
+
+    def _debug_output_vtk(self, label, name, prefix):
+        '''Debug postprocess with VTK.'''
+        vtk_settings = KratosMultiphysics.Parameters("""{
+            "model_part_name"                    : "PLEASE_SPECIFY_MODEL_PART_NAME",
+            "file_format"                        : "ascii",
+            "output_precision"                   : 7,
+            "output_control_type"                : "step",
+            "output_frequency"                   : 1.0,
+            "output_sub_model_parts"             : false,
+            "custom_name_prefix"                 : "",
+            "save_output_files_in_folder"        : false,
+            "nodal_solution_step_data_variables" : [],
+            "nodal_data_value_variables"         : [],
+            "element_data_value_variables"       : [],
+            "condition_data_value_variables"     : [],
+            "gauss_point_variables"              : []
+        }""")
+
+        vtk_settings["custom_name_prefix"].SetString(prefix + "REMESHING_" + name + "_STEP_" + str(label) + "_")
+        if self.settings["framework"].GetString() ==  "Lagrangian":
+            vtk_settings["nodal_solution_step_data_variables"].Append("DISPLACEMENT")
+            for var in self.internal_variable_interpolation_list:
+                vtk_settings["gauss_point_variables"].Append(var.Name())
+        else:
+            vtk_settings["nodal_solution_step_data_variables"].Append("VELOCITY")
+
+        if self.strategy == "levelset":
+            vtk_settings["nodal_solution_step_data_variables"].Append(self.scalar_variable.Name())
+            vtk_settings["nodal_solution_step_data_variables"].Append(self.gradation_value.Name())
+        elif self.strategy == "hessian":
+            variables = self.settings["hessian_strategy_parameters"]["metric_variable"].GetStringArray()
+            for i in range(len(variables)):
+                aux_var = KratosMultiphysics.KratosGlobals.GetVariable( variables[i] )
+                if self.settings["hessian_strategy_parameters"]["non_historical_metric_variable"][i].GetBool():
+                    vtk_settings["nodal_data_value_variables"].Append(variables[i])
+                else:
+                    vtk_settings["nodal_solution_step_data_variables"].Append(variables[i])
+
+        vtk_io = KratosMultiphysics.VtkOutput(self.main_model_part, vtk_settings)
+        vtk_io.PrintOutput()
+
+        #raise NameError("DEBUG")
+
+def _linear_interpolation(x, x_list, y_list):
+    tb = KratosMultiphysics.PiecewiseLinearTable()
+    for x,y in zip(x_list, y_list):
+        tb.AddRow(x, y)
+
+    return tb.GetNearestValue(x)
+
+def _normpdf(x, mean, sd):
+    dir_path = os.path.dirname(os.path.realpath(__file__))
+    data = json_utilities.read_external_json(dir_path+"/normal_distribution.json")
+    z = (x-mean)/sd
+    z_list = data["Z"]
+    prob_list = data["Prob"]
+    if (z > 0):
+        prob = _linear_interpolation(z, z_list, prob_list)
+    else:
+        prob = 1.0 - _linear_interpolation(-z, z_list, prob_list)
+    return prob
+
+
+def _normvalf(prob, mean, sd):
+    dir_path = os.path.dirname(os.path.realpath(__file__))
+    data = json_utilities.read_external_json(dir_path+"/normal_distribution.json")
+    z_list = data["Z"]
+    prob_list = data["Prob"]
+    if (prob >= 0.5):
+        z = _linear_interpolation(prob, prob_list, z_list)
+    else:
+        z = - _linear_interpolation(1.0 - prob, prob_list, z_list)
+    x = z * sd + mean
+    return x
+
+def _check_strategy(strategy):
+    strategies_list = [
+        "hessian",
+        "levelset",
+        "optimization",
+        "superconvergent_patch_recovery",
+        "spr"
+    ]
+    if strategy in strategies_list:
+        return strategy
+    elif strategy.lower() in strategies_list:
+        depr_msg  = 'The input strategy string is not in lower case letters. '
+        depr_msg += 'Please change it from "' + strategy + '" to "' +  strategy.lower() + '"'
+        KratosMultiphysics.Logger.PrintWarning('DEPRECATION-WARNING', depr_msg)
+        return strategy.lower()
+    else:
+        err_msg  = 'The input strategy "' + strategy + '" does not exit. The available options are:\n'
+        err_msg  += 'Available strategies: '
+        for avail_strategy in strategies_list:
+            err_msg += '"'+avail_strategy+'" '
         raise Exception(err_msg)
```

## KratosMultiphysics/MeshingApplication/multiscale_refining_process.py

 * *Ordering differences only*

```diff
@@ -1,192 +1,192 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KratosMultiphysics
-import KratosMultiphysics.MeshingApplication as MeshingApplication
-
-def Factory(settings, Model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return MultiscaleRefiningProcess(Model, settings["Parameters"])
-
-class MultiscaleRefiningProcess(KratosMultiphysics.Process):
-    def __init__(self, Model, settings ):
-
-        ## Settings string in json format
-        default_parameters = KratosMultiphysics.Parameters("""
-        {
-            "main_model_part_name"            : "MainModelPart",
-            "visualization_model_part_name"   : "VisualizationModelPart",
-            "current_subscale"                : 0,
-            "maximum_number_of_subscales"     : 4,
-            "echo_level"                      : 0,
-            "refining_condition_parameters"   : {
-                "kratos_module"                   : "KratosMultiphysics.ShallowWaterApplication",
-                "python_module"                   : "residual_based_refining_condition_process",
-                "Parameters"                      : {
-                    "model_part_name"                 : "model_part",
-                    "error_variable"                  : "RESIDUAL_NORM",
-                    "variable_threshold"              : 1e-3,
-                    "increase_threshold"              : true,
-                    "only_refine_wet_domain"          : true
-                }
-            },
-            "variables_to_apply_fixity"       : [],
-            "variables_to_set_at_interface"   : [],
-            "variables_to_update_at_coarse"   : [],
-            "advanced_configuration"          : {
-                "echo_level"                      : 0,
-                "number_of_divisions_at_subscale" : 2,
-                "subscale_interface_base_name"    : "refined_interface",
-                "subscale_boundary_condition"     : "LineCondition2D2N"
-            }
-        }
-        """)
-
-        # Overwrite the default settings with user-provided parameters
-        self.settings = settings
-        self.settings.RecursivelyValidateAndAssignDefaults(default_parameters)
-
-        self.model = Model
-
-        self.echo_level = self.settings['echo_level'].GetInt()
-        self.current_subscale = self.settings['current_subscale'].GetInt()
-        self.maximum_number_of_subscales = self.settings['maximum_number_of_subscales'].GetInt()
-        self.number_of_divisions_at_subscale = self.settings['advanced_configuration']['number_of_divisions_at_subscale'].GetInt()
-        self.number_of_substeps = 2**self.settings['advanced_configuration']['number_of_divisions_at_subscale'].GetInt()
-
-        # Get the coarse and refined model part names
-        self.coarse_model_part_name = self.settings['main_model_part_name'].GetString()
-        self.refined_model_part_name = self.coarse_model_part_name
-        if (self.current_subscale == 0):
-            self.coarse_model_part_name += '_0'
-            self.refined_model_part_name += '_0'
-        else:
-            self.coarse_model_part_name += '_' + str(self.current_subscale - 1)
-            self.refined_model_part_name += '_' + str(self.current_subscale)
-
-        # Get the model parts
-        if (self.current_subscale == 0):
-            self.coarse_model_part = self.model.CreateModelPart(self.coarse_model_part_name)
-            self.visualization_model_part = self.model.CreateModelPart(self.settings['visualization_model_part_name'].GetString())
-            self.refined_model_part = self.coarse_model_part
-        else:
-            self.coarse_model_part = self.model[self.coarse_model_part_name]
-            self.visualization_model_part = self.model[self.settings['visualization_model_part_name'].GetString()]
-            self.refined_model_part = self.model.CreateModelPart(self.refined_model_part_name)
-            self.refined_model_part.ProcessInfo[MeshingApplication.SUBSCALE_INDEX] = self.current_subscale
-
-        self.variables_to_apply_fixity = self._GenerateVariableListFromInput(self.settings["variables_to_apply_fixity"])
-        self.variables_to_set_at_interface = self._GenerateVariableListFromInput(self.settings["variables_to_set_at_interface"])
-        self.variables_to_update_at_coarse = self._GenerateVariableListFromInput(self.settings["variables_to_update_at_coarse"])
-
-        kratos_module_name = self.settings["refining_condition_parameters"]["kratos_module"].GetString()
-        python_module_name = self.settings["refining_condition_parameters"]["python_module"].GetString()
-        full_module_name = kratos_module_name + "." + python_module_name
-        python_module = __import__(full_module_name, fromlist=[python_module_name])
-        self.settings["refining_condition_parameters"]["Parameters"]["model_part_name"].SetString(self.coarse_model_part_name)
-        self.refining_condition_process = python_module.Factory(self.settings["refining_condition_parameters"], self.model)
-
-    def PrepareModelPart(self):
-        # Initialize the corresponding model part
-        if self.current_subscale == 0:
-            self._InitializeVisualizationModelPart()
-        else:
-            self._InitializeRefinedModelPart()
-            self.subscales_utility = MeshingApplication.MultiscaleRefiningProcess(
-                self.coarse_model_part,
-                self.refined_model_part,
-                self.visualization_model_part,
-                self.settings["advanced_configuration"])
-
-            if self.echo_level > 0:
-                print('The multiscale process is initialized')
-
-            if self.echo_level > 1:
-                print(self.model[self.coarse_model_part_name])
-                print(self.model[self.refined_model_part_name])
-
-    def ExecuteInitialize(self):
-        # This is equivalent to the ExecuteBeforeSolutionLoop
-        self.ExecuteBeforeSolutionLoop()
-
-    def ExecuteBeforeSolutionLoop(self):
-        if self.current_subscale > 0:
-            self._EvaluateCondition()
-            self._ExecuteRefinement()
-            self._ExecuteCoarsening()
-            self._ApplyFixityAtInterface(True)
-
-    def ExecuteInitializeSolutionStep(self):
-        if self.current_subscale == 0:
-            time = self.coarse_model_part.ProcessInfo[KratosMultiphysics.TIME]
-            step = self.coarse_model_part.ProcessInfo[KratosMultiphysics.STEP]
-            self.visualization_model_part.ProcessInfo[KratosMultiphysics.TIME] = time
-            self.visualization_model_part.ProcessInfo[KratosMultiphysics.STEP] = step
-        else:
-            self._TransferSubstepToRefinedInterface()
-
-    def ExecuteFinalizeSolutionStep(self):
-        pass
-
-    def ExecuteBeforeOutputStep(self):
-        pass
-
-    def ExecuteAfterOutputStep(self):
-        pass
-
-    def ExecuteFinalize(self):
-        if self.current_subscale > 0:
-            self._ApplyFixityAtInterface(False)
-            self._UpdateVariablesAtCoarseModelPart()
-
-    def Clear(self):
-        pass
-
-    def GetCoarseModelPart(self):
-        return self.coarse_model_part
-
-    def GetRefinedModelPart(self):
-        return self.refined_model_part
-
-    def GetVisualizationModelPart(self):
-        return self.visualization_model_part
-
-    def _InitializeVisualizationModelPart(self):
-        buffer_size = self.coarse_model_part.GetBufferSize()
-        self.visualization_model_part.SetBufferSize(buffer_size)
-        MeshingApplication.MultiscaleRefiningProcess.InitializeVisualizationModelPart(self.coarse_model_part, self.visualization_model_part)
-
-    def _InitializeRefinedModelPart(self):
-        buffer_size = self.coarse_model_part.GetBufferSize()
-        self.refined_model_part.SetBufferSize(buffer_size)
-        MeshingApplication.MultiscaleRefiningProcess.InitializeRefinedModelPart(self.coarse_model_part, self.refined_model_part)
-
-    def _ExecuteRefinement(self):
-        self.subscales_utility.ExecuteRefinement()
-
-    def _ExecuteCoarsening(self):
-        self.subscales_utility.ExecuteCoarsening()
-
-    def _EvaluateCondition(self):
-        self.refining_condition_process.Execute()
-
-    def _ApplyFixityAtInterface(self, state):
-        for variable in self.variables_to_apply_fixity:
-            self.subscales_utility.FixRefinedInterface(variable, state)
-
-    def _TransferSubstepToRefinedInterface(self):
-        substep_fraction = self.refined_model_part.ProcessInfo[KratosMultiphysics.STEP] / self.number_of_substeps
-        for variable in self.variables_to_set_at_interface:
-            self.subscales_utility.TransferSubstepToRefinedInterface(variable, substep_fraction)
-
-    def _UpdateVariablesAtCoarseModelPart(self):
-        for variable in self.variables_to_update_at_coarse:
-            self.subscales_utility.TransferLastStepToCoarseModelPart(variable)
-
-    def _GenerateVariableListFromInput(self,param):
-        '''Parse a list of variables from input.'''
-        # At least verify that the input is a string
-        if not param.IsArray():
-            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
-
-        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
-        return [ KratosMultiphysics.KratosGlobals.GetVariable( param[i].GetString() ) for i in range( 0,param.size() ) ]
+# Importing the Kratos Library
+import KratosMultiphysics as KratosMultiphysics
+import KratosMultiphysics.MeshingApplication as MeshingApplication
+
+def Factory(settings, Model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return MultiscaleRefiningProcess(Model, settings["Parameters"])
+
+class MultiscaleRefiningProcess(KratosMultiphysics.Process):
+    def __init__(self, Model, settings ):
+
+        ## Settings string in json format
+        default_parameters = KratosMultiphysics.Parameters("""
+        {
+            "main_model_part_name"            : "MainModelPart",
+            "visualization_model_part_name"   : "VisualizationModelPart",
+            "current_subscale"                : 0,
+            "maximum_number_of_subscales"     : 4,
+            "echo_level"                      : 0,
+            "refining_condition_parameters"   : {
+                "kratos_module"                   : "KratosMultiphysics.ShallowWaterApplication",
+                "python_module"                   : "residual_based_refining_condition_process",
+                "Parameters"                      : {
+                    "model_part_name"                 : "model_part",
+                    "error_variable"                  : "RESIDUAL_NORM",
+                    "variable_threshold"              : 1e-3,
+                    "increase_threshold"              : true,
+                    "only_refine_wet_domain"          : true
+                }
+            },
+            "variables_to_apply_fixity"       : [],
+            "variables_to_set_at_interface"   : [],
+            "variables_to_update_at_coarse"   : [],
+            "advanced_configuration"          : {
+                "echo_level"                      : 0,
+                "number_of_divisions_at_subscale" : 2,
+                "subscale_interface_base_name"    : "refined_interface",
+                "subscale_boundary_condition"     : "LineCondition2D2N"
+            }
+        }
+        """)
+
+        # Overwrite the default settings with user-provided parameters
+        self.settings = settings
+        self.settings.RecursivelyValidateAndAssignDefaults(default_parameters)
+
+        self.model = Model
+
+        self.echo_level = self.settings['echo_level'].GetInt()
+        self.current_subscale = self.settings['current_subscale'].GetInt()
+        self.maximum_number_of_subscales = self.settings['maximum_number_of_subscales'].GetInt()
+        self.number_of_divisions_at_subscale = self.settings['advanced_configuration']['number_of_divisions_at_subscale'].GetInt()
+        self.number_of_substeps = 2**self.settings['advanced_configuration']['number_of_divisions_at_subscale'].GetInt()
+
+        # Get the coarse and refined model part names
+        self.coarse_model_part_name = self.settings['main_model_part_name'].GetString()
+        self.refined_model_part_name = self.coarse_model_part_name
+        if (self.current_subscale == 0):
+            self.coarse_model_part_name += '_0'
+            self.refined_model_part_name += '_0'
+        else:
+            self.coarse_model_part_name += '_' + str(self.current_subscale - 1)
+            self.refined_model_part_name += '_' + str(self.current_subscale)
+
+        # Get the model parts
+        if (self.current_subscale == 0):
+            self.coarse_model_part = self.model.CreateModelPart(self.coarse_model_part_name)
+            self.visualization_model_part = self.model.CreateModelPart(self.settings['visualization_model_part_name'].GetString())
+            self.refined_model_part = self.coarse_model_part
+        else:
+            self.coarse_model_part = self.model[self.coarse_model_part_name]
+            self.visualization_model_part = self.model[self.settings['visualization_model_part_name'].GetString()]
+            self.refined_model_part = self.model.CreateModelPart(self.refined_model_part_name)
+            self.refined_model_part.ProcessInfo[MeshingApplication.SUBSCALE_INDEX] = self.current_subscale
+
+        self.variables_to_apply_fixity = self._GenerateVariableListFromInput(self.settings["variables_to_apply_fixity"])
+        self.variables_to_set_at_interface = self._GenerateVariableListFromInput(self.settings["variables_to_set_at_interface"])
+        self.variables_to_update_at_coarse = self._GenerateVariableListFromInput(self.settings["variables_to_update_at_coarse"])
+
+        kratos_module_name = self.settings["refining_condition_parameters"]["kratos_module"].GetString()
+        python_module_name = self.settings["refining_condition_parameters"]["python_module"].GetString()
+        full_module_name = kratos_module_name + "." + python_module_name
+        python_module = __import__(full_module_name, fromlist=[python_module_name])
+        self.settings["refining_condition_parameters"]["Parameters"]["model_part_name"].SetString(self.coarse_model_part_name)
+        self.refining_condition_process = python_module.Factory(self.settings["refining_condition_parameters"], self.model)
+
+    def PrepareModelPart(self):
+        # Initialize the corresponding model part
+        if self.current_subscale == 0:
+            self._InitializeVisualizationModelPart()
+        else:
+            self._InitializeRefinedModelPart()
+            self.subscales_utility = MeshingApplication.MultiscaleRefiningProcess(
+                self.coarse_model_part,
+                self.refined_model_part,
+                self.visualization_model_part,
+                self.settings["advanced_configuration"])
+
+            if self.echo_level > 0:
+                print('The multiscale process is initialized')
+
+            if self.echo_level > 1:
+                print(self.model[self.coarse_model_part_name])
+                print(self.model[self.refined_model_part_name])
+
+    def ExecuteInitialize(self):
+        # This is equivalent to the ExecuteBeforeSolutionLoop
+        self.ExecuteBeforeSolutionLoop()
+
+    def ExecuteBeforeSolutionLoop(self):
+        if self.current_subscale > 0:
+            self._EvaluateCondition()
+            self._ExecuteRefinement()
+            self._ExecuteCoarsening()
+            self._ApplyFixityAtInterface(True)
+
+    def ExecuteInitializeSolutionStep(self):
+        if self.current_subscale == 0:
+            time = self.coarse_model_part.ProcessInfo[KratosMultiphysics.TIME]
+            step = self.coarse_model_part.ProcessInfo[KratosMultiphysics.STEP]
+            self.visualization_model_part.ProcessInfo[KratosMultiphysics.TIME] = time
+            self.visualization_model_part.ProcessInfo[KratosMultiphysics.STEP] = step
+        else:
+            self._TransferSubstepToRefinedInterface()
+
+    def ExecuteFinalizeSolutionStep(self):
+        pass
+
+    def ExecuteBeforeOutputStep(self):
+        pass
+
+    def ExecuteAfterOutputStep(self):
+        pass
+
+    def ExecuteFinalize(self):
+        if self.current_subscale > 0:
+            self._ApplyFixityAtInterface(False)
+            self._UpdateVariablesAtCoarseModelPart()
+
+    def Clear(self):
+        pass
+
+    def GetCoarseModelPart(self):
+        return self.coarse_model_part
+
+    def GetRefinedModelPart(self):
+        return self.refined_model_part
+
+    def GetVisualizationModelPart(self):
+        return self.visualization_model_part
+
+    def _InitializeVisualizationModelPart(self):
+        buffer_size = self.coarse_model_part.GetBufferSize()
+        self.visualization_model_part.SetBufferSize(buffer_size)
+        MeshingApplication.MultiscaleRefiningProcess.InitializeVisualizationModelPart(self.coarse_model_part, self.visualization_model_part)
+
+    def _InitializeRefinedModelPart(self):
+        buffer_size = self.coarse_model_part.GetBufferSize()
+        self.refined_model_part.SetBufferSize(buffer_size)
+        MeshingApplication.MultiscaleRefiningProcess.InitializeRefinedModelPart(self.coarse_model_part, self.refined_model_part)
+
+    def _ExecuteRefinement(self):
+        self.subscales_utility.ExecuteRefinement()
+
+    def _ExecuteCoarsening(self):
+        self.subscales_utility.ExecuteCoarsening()
+
+    def _EvaluateCondition(self):
+        self.refining_condition_process.Execute()
+
+    def _ApplyFixityAtInterface(self, state):
+        for variable in self.variables_to_apply_fixity:
+            self.subscales_utility.FixRefinedInterface(variable, state)
+
+    def _TransferSubstepToRefinedInterface(self):
+        substep_fraction = self.refined_model_part.ProcessInfo[KratosMultiphysics.STEP] / self.number_of_substeps
+        for variable in self.variables_to_set_at_interface:
+            self.subscales_utility.TransferSubstepToRefinedInterface(variable, substep_fraction)
+
+    def _UpdateVariablesAtCoarseModelPart(self):
+        for variable in self.variables_to_update_at_coarse:
+            self.subscales_utility.TransferLastStepToCoarseModelPart(variable)
+
+    def _GenerateVariableListFromInput(self,param):
+        '''Parse a list of variables from input.'''
+        # At least verify that the input is a string
+        if not param.IsArray():
+            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
+
+        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
+        return [ KratosMultiphysics.KratosGlobals.GetVariable( param[i].GetString() ) for i in range( 0,param.size() ) ]
```

## Comparing `KratosMeshingApplication-9.4.6.dist-info/METADATA` & `KratosMeshingApplication-9.5.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-Metadata-Version: 2.1
-Name: KratosMeshingApplication
-Version: 9.4.6
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
-Requires-Dist: KratosMultiphysics ==9.4.6
-
-# Meshing Application
-
-![](https://raw.githubusercontent.com/KratosMultiphysics/Examples/master/mmg_remeshing_examples/use_cases/channel_sphere2D/data/channel.png)
-
-Meshing Application provides several tools to create, manipulate and interact with meshes. It containts several interfaces to both Kratos
-thrid party libraries (Triangle, TetGen, MMG)
-
-The application offers the functionalities listed below. If there is an Object without methds it means it can be called using the __Execute()__ function.
-
-- [Interface](#interface)
-  * [Custom IO](#custom-io)
-  * [Utilities](#utilities)
-  * [Meshers](#meshers)
-  * [Processes](#processes)
-    + [Metrics](#metrics)
-    + [LevelSet](#levelset)
-    + [Hessian](#hessian)
-    + [Error](#error)
-- [External Libraries](#external-libraries)
-  * [TetGen](#tetgen)
-  * [MMG](#mmg)
-  
-## Interface
-
-### Custom IO
-* __PFEMGidIO__: A specialized instance of GiDIO for the PFEM Application. It redefines several IO methods:
-  * _WriteMesh_
-  * _WriteNodeMesh_
-  * _InitializeMesh_
-  * _FinalizeMesh_
-  * _InitializeResults_
-  * _FinalizeResults_
-  * _WriteNodalResults_
-  * _PrintOnGaussPoints_
-  * _Flush_
-  * _CloseResultFile_
-  
-### Utilities
-* __MeshTransfer2D__
-* __MeshTransfer3D__:
-  * _DirectModelPartInterpolation_
-  * _DirectScalarVarInterpolation_
-  * _DirectVectorialVarInterpolation_
-
-* __BinBasedMeshTransfer2D__
-* __BinBasedMeshTransfer3D__: Alternative implementation of the __MeshTransfer__ utility based on bins. Inherits the procedures from __MeshTransfer__ and also adds:
-  * _MappingFromMovingMesh_ScalarVar_
-  * _MappingFromMovingMesh_VectorialVar_
-  * _MappingFromMovingMesh_VariableMeshes_ScalarVar_
-  * _MappingFromMovingMesh_VariableMeshes_VectorialVar_
-
-* __LocalRefineTriangleMesh__: Refines a Trianglular Mesh.
-* __LocalRefinePrismMesh__: Refines a Prism Mesh.
-* __LocalRefineSPrismMesh__: Refines a SPrism Mesh.
-* __LocalRefineTetrahedraMesh__: Refines a Tetrahedra Mesh.
-
-* __Cutting_Isosurface_Application__:
-  * _GenerateScalarVarCut_
-  * _GenerateVectorialComponentVarCut_
-  * _GenerateVectorialVarCut_
-  * _AddModelPartElements_
-  * _AddSkinConditions_
-  * _UpdateCutData_
-  * _DeleteCutData_
-
-### Meshers
-* __TriGenPFEMModeler__:
-  * _ReGenerateMesh_
-  
-* __TriGenGLASSModeler__:
-  * _ReGenerateMeshGlass_
-  
-* __TriGenPFEMModelerVMS__:
-  * _ReGenerateMesh_
-  
-* __TriGenPFEMSegment__:
-  * _ReGenerateMesh_
-
-### Processes
-* __InternalVariablesInterpolationProcess__: Inerpolates Nodal v
-
-#### Metrics
-* __MetricFastInit2D__:
-* __MetricFastInit3D__:
-
-#### LevelSet
-* __ComputeLevelSetSolMetricProcess2D__:
-* __ComputeLevelSetSolMetricProcess3D__:
-        
-#### Hessian
-* __ComputeHessianSolMetricProcess2D__: For double values.
-* __ComputeHessianSolMetricProcess3D__: For double values.
-* __ComputeHessianSolMetricProcessComp2D__: For components.
-* __ComputeHessianSolMetricProcessComp3D__: For components.
-        
-#### Error
-* __ComputeErrorSolMetricProcess2D__:
-* __ComputeErrorSolMetricProcess3D__:
-
-## External Libraries
-
-Meshing application can make use of several third party libs as an alternative (or sometimes unique) way to implementd the
-interface shown. You can find information about these libs in their respective pages which are listed below:
-
-### TetGen
-[TetGen](http://wias-berlin.de/software/index.jsp?id=TetGen&lang=1) is a program to generate tetrahedral meshes of any 3D polyhedral domains. 
-Please note that __Tetgen license is not compatible__ with Kratos, and hence it is not included as part of Kratos. You must indicate in compile time where it can find a tetgen already in your system.
-
-Tetgen enables to use the following __utilities__:
-
-* __TetgenVolumeMesher__:
-  * _AddHole_
-  * _GenerateMesh_
-    
-* __TetrahedraReconnectUtility__:
-  * _EvaluateQuality_
-  * _TestRemovingElements_
-  * _OptimizeQuality_
-  * _FinalizeOptimization_
-  * _updateNodesPositions_
-  * _setMaxNumThreads_
-  * _setBlockSize_
-  * _isaValidMesh_
-  
-Tetgen also enable to use the following __meshers__:
-
-* __TetGenPfemModeler__:
-  * _ReGenerateMesh_
-
-* __TetGenPfemRefineFace__:
-  * _ReGenerateMesh_
-
-* __TetGenPfemContact__:
-  * _ReGenerateMesh_
-    
-* __TetGenCDT__:
-  * _GenerateCDT_
-
-* __TetGenPfemModelerVms__:
-  * _ReGenerateMesh_
-  
-### MMG
-[MMG](https://www.mmgtools.org/) is an open source software for simplicial remeshing. It provides 3 applications and 4 libraries. In Kratos it provides the following additioanl __procedures__:
-
-* __MmgProcess__: This class is a remesher which uses the MMG library. The class uses a class for the 2D and 3D cases (solid and surfaces). The remesher keeps the previous submodelparts and interpolates the nodal values between the old and new mesh
-        
+Metadata-Version: 2.1
+Name: KratosMeshingApplication
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
+# Meshing Application
+
+![](https://raw.githubusercontent.com/KratosMultiphysics/Examples/master/mmg_remeshing_examples/use_cases/channel_sphere2D/data/channel.png)
+
+Meshing Application provides several tools to create, manipulate and interact with meshes. It containts several interfaces to both Kratos
+thrid party libraries (Triangle, TetGen, MMG)
+
+The application offers the functionalities listed below. If there is an Object without methds it means it can be called using the __Execute()__ function.
+
+- [Interface](#interface)
+  * [Custom IO](#custom-io)
+  * [Utilities](#utilities)
+  * [Meshers](#meshers)
+  * [Processes](#processes)
+    + [Metrics](#metrics)
+    + [LevelSet](#levelset)
+    + [Hessian](#hessian)
+    + [Error](#error)
+- [External Libraries](#external-libraries)
+  * [TetGen](#tetgen)
+  * [MMG](#mmg)
+  
+## Interface
+
+### Custom IO
+* __PFEMGidIO__: A specialized instance of GiDIO for the PFEM Application. It redefines several IO methods:
+  * _WriteMesh_
+  * _WriteNodeMesh_
+  * _InitializeMesh_
+  * _FinalizeMesh_
+  * _InitializeResults_
+  * _FinalizeResults_
+  * _WriteNodalResults_
+  * _PrintOnGaussPoints_
+  * _Flush_
+  * _CloseResultFile_
+  
+### Utilities
+* __MeshTransfer2D__
+* __MeshTransfer3D__:
+  * _DirectModelPartInterpolation_
+  * _DirectScalarVarInterpolation_
+  * _DirectVectorialVarInterpolation_
+
+* __BinBasedMeshTransfer2D__
+* __BinBasedMeshTransfer3D__: Alternative implementation of the __MeshTransfer__ utility based on bins. Inherits the procedures from __MeshTransfer__ and also adds:
+  * _MappingFromMovingMesh_ScalarVar_
+  * _MappingFromMovingMesh_VectorialVar_
+  * _MappingFromMovingMesh_VariableMeshes_ScalarVar_
+  * _MappingFromMovingMesh_VariableMeshes_VectorialVar_
+
+* __LocalRefineTriangleMesh__: Refines a Trianglular Mesh.
+* __LocalRefinePrismMesh__: Refines a Prism Mesh.
+* __LocalRefineSPrismMesh__: Refines a SPrism Mesh.
+* __LocalRefineTetrahedraMesh__: Refines a Tetrahedra Mesh.
+
+* __Cutting_Isosurface_Application__:
+  * _GenerateScalarVarCut_
+  * _GenerateVectorialComponentVarCut_
+  * _GenerateVectorialVarCut_
+  * _AddModelPartElements_
+  * _AddSkinConditions_
+  * _UpdateCutData_
+  * _DeleteCutData_
+
+### Meshers
+* __TriGenPFEMModeler__:
+  * _ReGenerateMesh_
+  
+* __TriGenGLASSModeler__:
+  * _ReGenerateMeshGlass_
+  
+* __TriGenPFEMModelerVMS__:
+  * _ReGenerateMesh_
+  
+* __TriGenPFEMSegment__:
+  * _ReGenerateMesh_
+
+### Processes
+* __InternalVariablesInterpolationProcess__: Inerpolates Nodal v
+
+#### Metrics
+* __MetricFastInit2D__:
+* __MetricFastInit3D__:
+
+#### LevelSet
+* __ComputeLevelSetSolMetricProcess2D__:
+* __ComputeLevelSetSolMetricProcess3D__:
+        
+#### Hessian
+* __ComputeHessianSolMetricProcess2D__: For double values.
+* __ComputeHessianSolMetricProcess3D__: For double values.
+* __ComputeHessianSolMetricProcessComp2D__: For components.
+* __ComputeHessianSolMetricProcessComp3D__: For components.
+        
+#### Error
+* __ComputeErrorSolMetricProcess2D__:
+* __ComputeErrorSolMetricProcess3D__:
+
+## External Libraries
+
+Meshing application can make use of several third party libs as an alternative (or sometimes unique) way to implementd the
+interface shown. You can find information about these libs in their respective pages which are listed below:
+
+### TetGen
+[TetGen](http://wias-berlin.de/software/index.jsp?id=TetGen&lang=1) is a program to generate tetrahedral meshes of any 3D polyhedral domains. 
+Please note that __Tetgen license is not compatible__ with Kratos, and hence it is not included as part of Kratos. You must indicate in compile time where it can find a tetgen already in your system.
+
+Tetgen enables to use the following __utilities__:
+
+* __TetgenVolumeMesher__:
+  * _AddHole_
+  * _GenerateMesh_
+    
+* __TetrahedraReconnectUtility__:
+  * _EvaluateQuality_
+  * _TestRemovingElements_
+  * _OptimizeQuality_
+  * _FinalizeOptimization_
+  * _updateNodesPositions_
+  * _setMaxNumThreads_
+  * _setBlockSize_
+  * _isaValidMesh_
+  
+Tetgen also enable to use the following __meshers__:
+
+* __TetGenPfemModeler__:
+  * _ReGenerateMesh_
+
+* __TetGenPfemRefineFace__:
+  * _ReGenerateMesh_
+
+* __TetGenPfemContact__:
+  * _ReGenerateMesh_
+    
+* __TetGenCDT__:
+  * _GenerateCDT_
+
+* __TetGenPfemModelerVms__:
+  * _ReGenerateMesh_
+  
+### MMG
+[MMG](https://www.mmgtools.org/) is an open source software for simplicial remeshing. It provides 3 applications and 4 libraries. In Kratos it provides the following additioanl __procedures__:
+
+* __MmgProcess__: This class is a remesher which uses the MMG library. The class uses a class for the 2D and 3D cases (solid and surfaces). The remesher keeps the previous submodelparts and interpolates the nodal values between the old and new mesh
+
```

