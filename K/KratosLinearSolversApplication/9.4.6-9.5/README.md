# Comparing `tmp/KratosLinearSolversApplication-9.4.6-cp39-cp39-win_amd64.whl.zip` & `tmp/KratosLinearSolversApplication-9.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,278 +1,529 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    885145 (00000000000D8199h)
-  Actual end-cent-dir record offset:        885123 (00000000000D8183h)
-  Expected end-cent-dir record offset:      885123 (00000000000D8183h)
+  Zip archive file size:                   2565116 (00000000002723FCh)
+  Actual end-cent-dir record offset:       2565094 (00000000002723E6h)
+  Expected end-cent-dir record offset:     2565094 (00000000002723E6h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 9 entries.
-  The central directory is 926 (000000000000039Eh) bytes long,
+  central directory contains 14 entries.
+  The central directory is 1706 (00000000000006AAh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 884197 (00000000000D7DE5h).
+  is 2563388 (0000000000271D3Ch).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosLinearSolversApplication.pyd
+  KratosLinearSolversApplication-9.5.dist-info/
 
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
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:36
-  32-bit CRC value (hex):                         7eb107fe
-  compressed size:                                540511 bytes
-  uncompressed size:                              1513472 bytes
-  length of filename:                             59 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:02 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             45 characters
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
 
-  KratosMultiphysics/.libs/KratosLinearSolversCore.lib
+  KratosLinearSolversApplication-9.5.dist-info/METADATA
 
-  offset of local header from start of archive:   540600
-                                                  (0000000000083FB8h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   103
+                                                  (0000000000000067h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:36
-  32-bit CRC value (hex):                         1a0bb10e
-  compressed size:                                10205 bytes
-  uncompressed size:                              425234 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:56
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 UTC
+  32-bit CRC value (hex):                         52fee0d2
+  compressed size:                                2836 bytes
+  uncompressed size:                              8974 bytes
+  length of filename:                             53 characters
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
 
 Central directory entry #3:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosLinearSolversCore.pyd
+  KratosLinearSolversApplication-9.5.dist-info/WHEEL
 
-  offset of local header from start of archive:   550887
-                                                  (00000000000867E7h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3050
+                                                  (0000000000000BEAh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:36
-  32-bit CRC value (hex):                         1db2b2d8
-  compressed size:                                328467 bytes
-  uncompressed size:                              1041408 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:56
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 UTC
+  32-bit CRC value (hex):                         90d34e0d
+  compressed size:                                116 bytes
+  uncompressed size:                              148 bytes
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
 
 Central directory entry #4:
 ---------------------------
 
-  KratosMultiphysics/LinearSolversApplication/__init__.py
+  KratosLinearSolversApplication-9.5.dist-info/top_level.txt
+
+  offset of local header from start of archive:   3274
+                                                  (0000000000000CCAh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:56
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 UTC
+  32-bit CRC value (hex):                         f32d789f
+  compressed size:                                19 bytes
+  uncompressed size:                              19 bytes
+  length of filename:                             58 characters
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
+  KratosLinearSolversApplication-9.5.dist-info/RECORD
 
-  offset of local header from start of archive:   879436
-                                                  (00000000000D6B4Ch) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3409
+                                                  (0000000000000D51h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         da54b5e3
-  compressed size:                                291 bytes
-  uncompressed size:                              692 bytes
-  length of filename:                             55 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:02 UTC
+  32-bit CRC value (hex):                         9f048a9d
+  compressed size:                                574 bytes
+  uncompressed size:                              1142 bytes
+  length of filename:                             51 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  apparent file type:                             text
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
   There is no file comment.
 
-Central directory entry #5:
+Central directory entry #6:
 ---------------------------
 
-  KratosMultiphysics/LinearSolversApplication/dense_linear_solver_factory.py
+  KratosLinearSolversApplication.libs/
 
-  offset of local header from start of archive:   879812
-                                                  (00000000000D6CC4h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   4092
+                                                  (0000000000000FFCh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:02 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             36 characters
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
+Central directory entry #7:
+---------------------------
+
+  KratosLinearSolversApplication.libs/libKratosLinearSolversCore-946bfc3a.so
+
+  offset of local header from start of archive:   4186
+                                                  (000000000000105Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         4c768912
-  compressed size:                                462 bytes
-  uncompressed size:                              1254 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:56
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 UTC
+  32-bit CRC value (hex):                         bce5d88c
+  compressed size:                                1056666 bytes
+  uncompressed size:                              4673617 bytes
   length of filename:                             74 characters
-  length of extra field:                          0 bytes
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
+Central directory entry #8:
+---------------------------
+
+  KratosMultiphysics/
+
+  offset of local header from start of archive:   1060984
+                                                  (0000000000103078h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:56
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 UTC
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
+Central directory entry #9:
 ---------------------------
 
-  KratosLinearSolversApplication-9.4.6.dist-info/METADATA
+  KratosMultiphysics/.libs/
 
-  offset of local header from start of archive:   880378
-                                                  (00000000000D6EFAh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1061061
+                                                  (00000000001030C5h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:02
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:02 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:02 UTC
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
+Central directory entry #10:
+---------------------------
+
+  KratosMultiphysics/.libs/KratosLinearSolversApplication.cpython-39-x86_64-linux-gnu.so
+
+  offset of local header from start of archive:   1061144
+                                                  (0000000000103118h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:36
-  32-bit CRC value (hex):                         afc16f3c
-  compressed size:                                2867 bytes
-  uncompressed size:                              9211 bytes
-  length of filename:                             55 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:56
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 UTC
+  32-bit CRC value (hex):                         10605789
+  compressed size:                                1500187 bytes
+  uncompressed size:                              3847457 bytes
+  length of filename:                             86 characters
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
+Central directory entry #11:
+---------------------------
+
+  KratosMultiphysics/LinearSolversApplication/
+
+  offset of local header from start of archive:   2561475
+                                                  (00000000002715C3h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:56
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             44 characters
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
+Central directory entry #12:
 ---------------------------
 
-  KratosLinearSolversApplication-9.4.6.dist-info/WHEEL
+  KratosMultiphysics/LinearSolversApplication/dense_linear_solver_factory.py
 
-  offset of local header from start of archive:   883330
-                                                  (00000000000D7A82h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   2561577
+                                                  (0000000000271629h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:36
-  32-bit CRC value (hex):                         86fb6b41
-  compressed size:                                96 bytes
-  uncompressed size:                              100 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:56
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 UTC
+  32-bit CRC value (hex):                         4fe764dc
+  compressed size:                                453 bytes
+  uncompressed size:                              1231 bytes
+  length of filename:                             74 characters
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
+Central directory entry #13:
 ---------------------------
 
-  KratosLinearSolversApplication-9.4.6.dist-info/top_level.txt
+  KratosMultiphysics/LinearSolversApplication/__init__.pyi
 
-  offset of local header from start of archive:   883508
-                                                  (00000000000D7B34h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   2562162
+                                                  (0000000000271872h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:36
-  32-bit CRC value (hex):                         f32d789f
-  compressed size:                                21 bytes
-  uncompressed size:                              19 bytes
-  length of filename:                             60 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:56
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 UTC
+  32-bit CRC value (hex):                         3e6e4654
+  compressed size:                                714 bytes
+  uncompressed size:                              6675 bytes
+  length of filename:                             56 characters
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
+Central directory entry #14:
 ---------------------------
 
-  KratosLinearSolversApplication-9.4.6.dist-info/RECORD
+  KratosMultiphysics/LinearSolversApplication/__init__.py
 
-  offset of local header from start of archive:   883619
-                                                  (00000000000D7BA3h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   2562990
+                                                  (0000000000271BAEh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         68166296
-  compressed size:                                495 bytes
-  uncompressed size:                              975 bytes
-  length of filename:                             53 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:56
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:56 UTC
+  32-bit CRC value (hex):                         5c0d4788
+  compressed size:                                285 bytes
+  uncompressed size:                              676 bytes
+  length of filename:                             55 characters
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
@@ -1,28 +1,43 @@
-Filename: KratosMultiphysics/.libs/KratosLinearSolversApplication.pyd
+Filename: KratosLinearSolversApplication-9.5.dist-info/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosLinearSolversCore.lib
+Filename: KratosLinearSolversApplication-9.5.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosLinearSolversCore.pyd
+Filename: KratosLinearSolversApplication-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics/LinearSolversApplication/__init__.py
+Filename: KratosLinearSolversApplication-9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosMultiphysics/LinearSolversApplication/dense_linear_solver_factory.py
+Filename: KratosLinearSolversApplication-9.5.dist-info/RECORD
+Comment: 
+
+Filename: KratosLinearSolversApplication.libs/
+Comment: 
+
+Filename: KratosLinearSolversApplication.libs/libKratosLinearSolversCore-946bfc3a.so
+Comment: 
+
+Filename: KratosMultiphysics/
+Comment: 
+
+Filename: KratosMultiphysics/.libs/
 Comment: 
 
-Filename: KratosLinearSolversApplication-9.4.6.dist-info/METADATA
+Filename: KratosMultiphysics/.libs/KratosLinearSolversApplication.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: KratosLinearSolversApplication-9.4.6.dist-info/WHEEL
+Filename: KratosMultiphysics/LinearSolversApplication/
 Comment: 
 
-Filename: KratosLinearSolversApplication-9.4.6.dist-info/top_level.txt
+Filename: KratosMultiphysics/LinearSolversApplication/dense_linear_solver_factory.py
 Comment: 
 
-Filename: KratosLinearSolversApplication-9.4.6.dist-info/RECORD
+Filename: KratosMultiphysics/LinearSolversApplication/__init__.pyi
+Comment: 
+
+Filename: KratosMultiphysics/LinearSolversApplication/__init__.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## KratosMultiphysics/LinearSolversApplication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,16 +1,16 @@
-# KRATOS  _     _                       ____        _
-#        | |   (_)_ __   ___  __ _ _ __/ ___|  ___ | |_   _____ _ __ ___
-#        | |   | | '_ \ / _ \/ _` | '__\___ \ / _ \| \ \ / / _ \ '__/ __|
-#        | |___| | | | |  __/ (_| | |   ___) | (_) | |\ V /  __/ |  \__ |
-#        |_____|_|_| |_|\___|\__,_|_|  |____/ \___/|_| \_/ \___|_|  |___/ Application
-#
-#   Author: Thomas Oberbichler
-#
-
-# Application dependent names and paths
-from KratosMultiphysics import _ImportApplication
-from KratosLinearSolversApplication import *
-application = KratosLinearSolversApplication()
-application_name = "LinearSolversApplication"
-
-_ImportApplication(application, application_name)
+# KRATOS  _     _                       ____        _
+#        | |   (_)_ __   ___  __ _ _ __/ ___|  ___ | |_   _____ _ __ ___
+#        | |   | | '_ \ / _ \/ _` | '__\___ \ / _ \| \ \ / / _ \ '__/ __|
+#        | |___| | | | |  __/ (_| | |   ___) | (_) | |\ V /  __/ |  \__ |
+#        |_____|_|_| |_|\___|\__,_|_|  |____/ \___/|_| \_/ \___|_|  |___/ Application
+#
+#   Author: Thomas Oberbichler
+#
+
+# Application dependent names and paths
+from KratosMultiphysics import _ImportApplication
+from KratosLinearSolversApplication import *
+application = KratosLinearSolversApplication()
+application_name = "LinearSolversApplication"
+
+_ImportApplication(application, application_name)
```

## KratosMultiphysics/LinearSolversApplication/dense_linear_solver_factory.py

```diff
@@ -1,79 +1,77 @@
-00000000: 0d0a 696d 706f 7274 204b 7261 746f 734d  ..import KratosM
-00000010: 756c 7469 7068 7973 6963 7320 6173 204b  ultiphysics as K
-00000020: 4d0d 0a69 6d70 6f72 7420 4b72 6174 6f73  M..import Kratos
-00000030: 4d75 6c74 6970 6879 7369 6373 2e4c 696e  Multiphysics.Lin
-00000040: 6561 7253 6f6c 7665 7273 4170 706c 6963  earSolversApplic
-00000050: 6174 696f 6e20 6173 204b 7261 746f 7353  ation as KratosS
-00000060: 6f6c 7665 7273 0d0a 6672 6f6d 204b 7261  olvers..from Kra
-00000070: 746f 734d 756c 7469 7068 7973 6963 7320  tosMultiphysics 
-00000080: 696d 706f 7274 2070 7974 686f 6e5f 6c69  import python_li
-00000090: 6e65 6172 5f73 6f6c 7665 725f 6661 6374  near_solver_fact
-000000a0: 6f72 790d 0a0d 0a64 6566 2043 6f6e 7374  ory....def Const
-000000b0: 7275 6374 536f 6c76 6572 2863 6f6e 6669  ructSolver(confi
-000000c0: 6775 7261 7469 6f6e 293a 0d0a 2020 2020  guration):..    
-000000d0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-000000e0: 6528 636f 6e66 6967 7572 6174 696f 6e2c  e(configuration,
-000000f0: 204b 4d2e 5061 7261 6d65 7465 7273 293a   KM.Parameters):
-00000100: 0d0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
-00000110: 4578 6365 7074 696f 6e28 2269 6e70 7574  Exception("input
-00000120: 2069 7320 6578 7065 6374 6564 2074 6f20   is expected to 
-00000130: 6265 2070 726f 7669 6465 6420 6173 2061  be provided as a
-00000140: 204b 7261 746f 7320 5061 7261 6d65 7465   Kratos Paramete
-00000150: 7273 206f 626a 6563 7422 290d 0a0d 0a20  rs object").... 
-00000160: 2020 2073 6f6c 7665 725f 7479 7065 203d     solver_type =
-00000170: 2063 6f6e 6669 6775 7261 7469 6f6e 5b22   configuration["
-00000180: 736f 6c76 6572 5f74 7970 6522 5d2e 4765  solver_type"].Ge
-00000190: 7453 7472 696e 6728 290d 0a20 2020 2069  tString()..    i
-000001a0: 6620 2241 7070 6c69 6361 7469 6f6e 2e22  f "Application."
-000001b0: 2069 6e20 736f 6c76 6572 5f74 7970 653a   in solver_type:
-000001c0: 2023 2074 6865 206d 6f64 756c 6520 696e   # the module in
-000001d0: 2077 6869 6368 2074 6865 2073 6f6c 7665   which the solve
-000001e0: 7220 6973 2069 6d70 6c65 6d65 6e74 6564  r is implemented
-000001f0: 2077 6173 2073 7065 6369 6669 6564 0d0a   was specified..
-00000200: 2020 2020 2020 2020 7370 6c69 745f 6e61          split_na
-00000210: 6d65 203d 2073 6f6c 7665 725f 7479 7065  me = solver_type
-00000220: 2e73 706c 6974 2822 2e22 290d 0a20 2020  .split(".")..   
-00000230: 2020 2020 2073 6f6c 7665 725f 7479 7065       solver_type
-00000240: 203d 2073 706c 6974 5f6e 616d 655b 315d   = split_name[1]
-00000250: 0d0a 0d0a 2020 2020 6966 204b 7261 746f  ....    if Krato
-00000260: 7353 6f6c 7665 7273 2e44 656e 7365 4c69  sSolvers.DenseLi
-00000270: 6e65 6172 536f 6c76 6572 4661 6374 6f72  nearSolverFactor
-00000280: 7928 292e 4861 7328 736f 6c76 6572 5f74  y().Has(solver_t
-00000290: 7970 6529 3a0d 0a20 2020 2020 2020 204b  ype):..        K
-000002a0: 4d2e 4c6f 6767 6572 2e50 7269 6e74 496e  M.Logger.PrintIn
-000002b0: 666f 2822 4569 6765 6e2d 4c69 6e65 6172  fo("Eigen-Linear
-000002c0: 2d53 6f6c 7665 722d 4661 6374 6f72 7922  -Solver-Factory"
-000002d0: 2c20 2243 6f6e 7374 7275 6374 696e 6720  , "Constructing 
-000002e0: 6120 6465 6e73 6520 6c69 6e65 6172 2d73  a dense linear-s
-000002f0: 6f6c 7665 7222 290d 0a20 2020 2020 2020  olver")..       
-00000300: 2072 6574 7572 6e20 4b72 6174 6f73 536f   return KratosSo
-00000310: 6c76 6572 732e 4465 6e73 654c 696e 6561  lvers.DenseLinea
-00000320: 7253 6f6c 7665 7246 6163 746f 7279 2829  rSolverFactory()
-00000330: 2e43 7265 6174 6528 636f 6e66 6967 7572  .Create(configur
-00000340: 6174 696f 6e29 0d0a 2020 2020 656c 6966  ation)..    elif
-00000350: 204b 7261 746f 7353 6f6c 7665 7273 2e43   KratosSolvers.C
-00000360: 6f6d 706c 6578 4465 6e73 654c 696e 6561  omplexDenseLinea
-00000370: 7253 6f6c 7665 7246 6163 746f 7279 2829  rSolverFactory()
-00000380: 2e48 6173 2873 6f6c 7665 725f 7479 7065  .Has(solver_type
-00000390: 293a 0d0a 2020 2020 2020 2020 4b4d 2e4c  ):..        KM.L
-000003a0: 6f67 6765 722e 5072 696e 7449 6e66 6f28  ogger.PrintInfo(
-000003b0: 2245 6967 656e 2d4c 696e 6561 722d 536f  "Eigen-Linear-So
-000003c0: 6c76 6572 2d46 6163 746f 7279 222c 2022  lver-Factory", "
-000003d0: 436f 6e73 7472 7563 7469 6e67 2061 2063  Constructing a c
-000003e0: 6f6d 706c 6578 2064 656e 7365 206c 696e  omplex dense lin
-000003f0: 6561 722d 736f 6c76 6572 2229 0d0a 2020  ear-solver")..  
-00000400: 2020 2020 2020 7265 7475 726e 204b 7261        return Kra
-00000410: 746f 7353 6f6c 7665 7273 2e43 6f6d 706c  tosSolvers.Compl
-00000420: 6578 4465 6e73 654c 696e 6561 7253 6f6c  exDenseLinearSol
-00000430: 7665 7246 6163 746f 7279 2829 2e43 7265  verFactory().Cre
-00000440: 6174 6528 636f 6e66 6967 7572 6174 696f  ate(configuratio
-00000450: 6e29 0d0a 2020 2020 656c 7365 3a0d 0a20  n)..    else:.. 
-00000460: 2020 2020 2020 2023 2066 616c 6c20 6261         # fall ba
-00000470: 636b 2074 6f20 7468 6520 7374 616e 6461  ck to the standa
-00000480: 7264 206c 696e 6561 7220 736f 6c76 6572  rd linear solver
-00000490: 2066 6163 746f 7279 0d0a 2020 2020 2020   factory..      
-000004a0: 2020 7265 7475 726e 2070 7974 686f 6e5f    return python_
-000004b0: 6c69 6e65 6172 5f73 6f6c 7665 725f 6661  linear_solver_fa
-000004c0: 6374 6f72 792e 436f 6e73 7472 7563 7453  ctory.ConstructS
-000004d0: 6f6c 7665 7228 636f 6e66 6967 7572 6174  olver(configurat
-000004e0: 696f 6e29 0d0a                           ion)..
+00000000: 0a69 6d70 6f72 7420 4b72 6174 6f73 4d75  .import KratosMu
+00000010: 6c74 6970 6879 7369 6373 2061 7320 4b4d  ltiphysics as KM
+00000020: 0a69 6d70 6f72 7420 4b72 6174 6f73 4d75  .import KratosMu
+00000030: 6c74 6970 6879 7369 6373 2e4c 696e 6561  ltiphysics.Linea
+00000040: 7253 6f6c 7665 7273 4170 706c 6963 6174  rSolversApplicat
+00000050: 696f 6e20 6173 204b 7261 746f 7353 6f6c  ion as KratosSol
+00000060: 7665 7273 0a66 726f 6d20 4b72 6174 6f73  vers.from Kratos
+00000070: 4d75 6c74 6970 6879 7369 6373 2069 6d70  Multiphysics imp
+00000080: 6f72 7420 7079 7468 6f6e 5f6c 696e 6561  ort python_linea
+00000090: 725f 736f 6c76 6572 5f66 6163 746f 7279  r_solver_factory
+000000a0: 0a0a 6465 6620 436f 6e73 7472 7563 7453  ..def ConstructS
+000000b0: 6f6c 7665 7228 636f 6e66 6967 7572 6174  olver(configurat
+000000c0: 696f 6e29 3a0a 2020 2020 6966 206e 6f74  ion):.    if not
+000000d0: 2069 7369 6e73 7461 6e63 6528 636f 6e66   isinstance(conf
+000000e0: 6967 7572 6174 696f 6e2c 204b 4d2e 5061  iguration, KM.Pa
+000000f0: 7261 6d65 7465 7273 293a 0a20 2020 2020  rameters):.     
+00000100: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+00000110: 6f6e 2822 696e 7075 7420 6973 2065 7870  on("input is exp
+00000120: 6563 7465 6420 746f 2062 6520 7072 6f76  ected to be prov
+00000130: 6964 6564 2061 7320 6120 4b72 6174 6f73  ided as a Kratos
+00000140: 2050 6172 616d 6574 6572 7320 6f62 6a65   Parameters obje
+00000150: 6374 2229 0a0a 2020 2020 736f 6c76 6572  ct")..    solver
+00000160: 5f74 7970 6520 3d20 636f 6e66 6967 7572  _type = configur
+00000170: 6174 696f 6e5b 2273 6f6c 7665 725f 7479  ation["solver_ty
+00000180: 7065 225d 2e47 6574 5374 7269 6e67 2829  pe"].GetString()
+00000190: 0a20 2020 2069 6620 2241 7070 6c69 6361  .    if "Applica
+000001a0: 7469 6f6e 2e22 2069 6e20 736f 6c76 6572  tion." in solver
+000001b0: 5f74 7970 653a 2023 2074 6865 206d 6f64  _type: # the mod
+000001c0: 756c 6520 696e 2077 6869 6368 2074 6865  ule in which the
+000001d0: 2073 6f6c 7665 7220 6973 2069 6d70 6c65   solver is imple
+000001e0: 6d65 6e74 6564 2077 6173 2073 7065 6369  mented was speci
+000001f0: 6669 6564 0a20 2020 2020 2020 2073 706c  fied.        spl
+00000200: 6974 5f6e 616d 6520 3d20 736f 6c76 6572  it_name = solver
+00000210: 5f74 7970 652e 7370 6c69 7428 222e 2229  _type.split(".")
+00000220: 0a20 2020 2020 2020 2073 6f6c 7665 725f  .        solver_
+00000230: 7479 7065 203d 2073 706c 6974 5f6e 616d  type = split_nam
+00000240: 655b 315d 0a0a 2020 2020 6966 204b 7261  e[1]..    if Kra
+00000250: 746f 7353 6f6c 7665 7273 2e44 656e 7365  tosSolvers.Dense
+00000260: 4c69 6e65 6172 536f 6c76 6572 4661 6374  LinearSolverFact
+00000270: 6f72 7928 292e 4861 7328 736f 6c76 6572  ory().Has(solver
+00000280: 5f74 7970 6529 3a0a 2020 2020 2020 2020  _type):.        
+00000290: 4b4d 2e4c 6f67 6765 722e 5072 696e 7449  KM.Logger.PrintI
+000002a0: 6e66 6f28 2245 6967 656e 2d4c 696e 6561  nfo("Eigen-Linea
+000002b0: 722d 536f 6c76 6572 2d46 6163 746f 7279  r-Solver-Factory
+000002c0: 222c 2022 436f 6e73 7472 7563 7469 6e67  ", "Constructing
+000002d0: 2061 2064 656e 7365 206c 696e 6561 722d   a dense linear-
+000002e0: 736f 6c76 6572 2229 0a20 2020 2020 2020  solver").       
+000002f0: 2072 6574 7572 6e20 4b72 6174 6f73 536f   return KratosSo
+00000300: 6c76 6572 732e 4465 6e73 654c 696e 6561  lvers.DenseLinea
+00000310: 7253 6f6c 7665 7246 6163 746f 7279 2829  rSolverFactory()
+00000320: 2e43 7265 6174 6528 636f 6e66 6967 7572  .Create(configur
+00000330: 6174 696f 6e29 0a20 2020 2065 6c69 6620  ation).    elif 
+00000340: 4b72 6174 6f73 536f 6c76 6572 732e 436f  KratosSolvers.Co
+00000350: 6d70 6c65 7844 656e 7365 4c69 6e65 6172  mplexDenseLinear
+00000360: 536f 6c76 6572 4661 6374 6f72 7928 292e  SolverFactory().
+00000370: 4861 7328 736f 6c76 6572 5f74 7970 6529  Has(solver_type)
+00000380: 3a0a 2020 2020 2020 2020 4b4d 2e4c 6f67  :.        KM.Log
+00000390: 6765 722e 5072 696e 7449 6e66 6f28 2245  ger.PrintInfo("E
+000003a0: 6967 656e 2d4c 696e 6561 722d 536f 6c76  igen-Linear-Solv
+000003b0: 6572 2d46 6163 746f 7279 222c 2022 436f  er-Factory", "Co
+000003c0: 6e73 7472 7563 7469 6e67 2061 2063 6f6d  nstructing a com
+000003d0: 706c 6578 2064 656e 7365 206c 696e 6561  plex dense linea
+000003e0: 722d 736f 6c76 6572 2229 0a20 2020 2020  r-solver").     
+000003f0: 2020 2072 6574 7572 6e20 4b72 6174 6f73     return Kratos
+00000400: 536f 6c76 6572 732e 436f 6d70 6c65 7844  Solvers.ComplexD
+00000410: 656e 7365 4c69 6e65 6172 536f 6c76 6572  enseLinearSolver
+00000420: 4661 6374 6f72 7928 292e 4372 6561 7465  Factory().Create
+00000430: 2863 6f6e 6669 6775 7261 7469 6f6e 290a  (configuration).
+00000440: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00000450: 2020 2320 6661 6c6c 2062 6163 6b20 746f    # fall back to
+00000460: 2074 6865 2073 7461 6e64 6172 6420 6c69   the standard li
+00000470: 6e65 6172 2073 6f6c 7665 7220 6661 6374  near solver fact
+00000480: 6f72 790a 2020 2020 2020 2020 7265 7475  ory.        retu
+00000490: 726e 2070 7974 686f 6e5f 6c69 6e65 6172  rn python_linear
+000004a0: 5f73 6f6c 7665 725f 6661 6374 6f72 792e  _solver_factory.
+000004b0: 436f 6e73 7472 7563 7453 6f6c 7665 7228  ConstructSolver(
+000004c0: 636f 6e66 6967 7572 6174 696f 6e29 0a    configuration).
```

## Comparing `KratosLinearSolversApplication-9.4.6.dist-info/METADATA` & `KratosLinearSolversApplication-9.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,233 +1,233 @@
-Metadata-Version: 2.1
-Name: KratosLinearSolversApplication
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
-# LinearSolversApplication
-
-The *LinearSolversApplication* is a thin wrapper for the [Eigen linear algebra library](http://eigen.tuxfamily.org/index.php?title=Main_Page).
-
-## Direct sparse solvers
-
-The application provides the following direct sparse solvers:
-
-| Python class             | solver_type            | Matrix kind | Domain   | Dependencies |
-|--------------------------|------------------------|:-----------:|:--------:|:------------:|
-| SparseLUSolver           | `sparse_lu`            | Square      | Real     | None         |
-| SparseQRSolver           | `sparse_qr`            | Rectangular | Real     | None         |
-| SparseCGSolver           | `sparse_cg`            | SPD*        | Real     | None         |
-| PardisoLLTSolver         | `pardiso_llt`          | SPD*        | Real     | Intel® MKL   |
-| PardisoLDLTSolver        | `pardiso_ldlt`         | SPD*        | Real     | Intel® MKL   |
-| PardisoLUSolver          | `pardiso_lu`           | Square      | Real     | Intel® MKL   |
-| ComplexSparseLUSolver    | `sparse_lu_complex`    | Square      | Complex  | None         |
-| ComplexPardisoLLTSolver  | `pardiso_llt_complex`  | SPD*        | Complex  | Intel® MKL   |
-| ComplexPardisoLDLTSolver | `pardiso_ldlt_complex` | SPD*        | Complex  | Intel® MKL   |
-| ComplexPardisoLUSolver   | `pardiso_lu_complex`   | Square      | Complex  | Intel® MKL   |
-
-*SPD = Symmetric Positive Definite
-
-**Example**:
-
-```json
-{
-    "solver_type": "eigen_sparse_lu"
-}
-```
-
-## Direct dense solvers
-
-The application provides the following direct solvers for dense systems of equations:
-
-| Python class                            | solver_type                            | Matrix requirements | Domain  | Dependencies |
-| --------------------------------------- | -------------------------------------- | :-----------------: | :-----: | :----------: |
-| DenseColPivHouseholderQRSolver**        | `dense_col_piv_householder_qr`         |        None         |  Real   |     None     |
-| DenseHouseholderQRSolver**              | `dense_householder_qr`                 |        None         |  Real   |     None     |
-| DenseLLTSolver**                        | `dense_llt`                            |        SPD*         |  Real   |     None     |
-| DensePartialPivLUSolver**               | `dense_partial_piv_lu`                 |     Invertible      |  Real   |     None     |
-| ComplexDenseColPivHouseholderQRSolver   | `complex_dense_col_piv_householder_qr` |        None         | Complex |     None     |
-| ComplexDenseHouseholderQRSolver         | `complex_dense_householder_qr`         |        None         | Complex |     None     |
-| ComplexDensePartialPivLUSolver          | `complex_dense_partial_piv_lu`         |     Invertible      | Complex |     None     |
-
-*SPD = Symmetric Positive Definite
-
-**Can also be used to solve equation systems with multiple right hand sides.
-
-## Generalized eigensystem solvers
-
-The application provides the following generalized eigensystem `Ax=λBx` solver for sparse matrices.
-
-| Python class                           | solver_type                | Matrix kind A | Matrix kind B | Domain   | Dependencies |
-|----------------------------------------|----------------------------|:-------------:|:-------------:|:--------:|:------------:|
-| EigensystemSolver                      | `eigen_eigensystem`        | Symmetric     | SPD*          | Real     | None         |
-| SpectraSymGEigsShiftSolver             | `spectra_sym_g_eigs_shift` | Symmetric     | SPD*          | Real     | None         |
-| FEASTGeneralEigensystemSolver**        | `feast`                    | General       | General       | Real     | Intel® MKL   |
-| ComplexFEASTGeneralEigensystemSolver** | `feast_complex`            | General       | General       | Complex  | Intel® MKL   |
-
-*SPD = Symmetric Positive Definite
-**A special version for symmetric matrices can be triggered in the solver settings.
-
-`EigensystemSolver` and `SpectraSymGEigsShiftSolver` compute the smallest eigenvalues and corresponding eigenvectors of the system. MKL routines are used automatically if they are available.
-
-`SpectraSymGEigsShiftSolver` interfaces a solver from the [Spectra library](https://spectralib.org/), and has a shift mode that can be used to compute the smallest eigenvalues > `shift`.
-
-**Example:**
-
-```json
-{
-    "solver_type": "spectra_sym_g_eigs_shift",
-    "number_of_eigenvalues": 3,
-    "max_iteration": 1000,
-    "echo_level": 1
-}
-
-```
-If the application is compiled with MKL, [FEAST 4.0](http://www.ecs.umass.edu/~polizzi/feast/) can be used to solve the generalized eigenvalue problem for real and complex systems (symmetric or unsymmetric). The cmake switch `USE_EIGEN_FEAST` must be set to `ON` with
-```batch
--DUSE_EIGEN_FEAST=ON \
-```
-
-**Example:**
-```json
-{
-    "solver_type": "feast",
-    "symmetric": true,
-    "number_of_eigenvalues": 3,
-    "search_lowest_eigenvalues": true,
-    "e_min" : 0.0,
-    "e_max" : 0.2
-}
-```
-
-## Build instructions
-
-1. Set the required definitions for cmake
-
-    As any other app:
-
-    **Windows:** in `configure.bat`
-
-    ```batch
-    set KRATOS_APPLICATIONS=%KRATOS_APPLICATIONS%%KRATOS_APP_DIR%\LinearSolversApplication;
-    ```
-
-    **Linux:** in `configure.sh`
-
-    ```console
-    add_app ${KRATOS_APP_DIR}/LinearSolversApplication
-    ```
-
-2. Build Kratos
-
-3. Setup the `ProjectParameters.json`
-
-    ```json
-    "linear_solver_settings": {
-        "solver_type" : "LinearSolversApplication.sparse_lu"
-    }
-    ```
-
-4. Run the simulation
-
-## Enable MKL (optional)
-
-In case you have installed [MKL](https://software.intel.com/en-us/mkl) (see below), you can also use the Pardiso solvers.
-
-1. Run the MKL setup script before building Kratos:
-
-    **Windows:**
-
-    ```batch
-    call "C:\Program Files (x86)\Intel\oneAPI\mkl\latest\env\vars.bat" intel64 lp64
-    ```
-
-    **Linux:**
-
-    ```console
-    source /opt/intel/oneapi/setvars.sh intel64
-    ```
-
-2. Add the following flag to CMake to your configure script:
-
-    **Windows:**
-
-    ```batch
-    -DUSE_EIGEN_MKL=ON ^
-    ```
-
-    **Linux:**
-
-    ```console
-    -DUSE_EIGEN_MKL=ON \
-    ```
-
-3. Build Kratos
-
-4. Usage:
-
-    **Windows:**
-
-    ```batch
-    call "C:\Program Files (x86)\Intel\oneAPI\mkl\latest\env\vars.bat" intel64 lp64
-    ```
-
-    **Linux:**
-
-    Set the environment before using MKL
-
-    ```console
-    source /opt/intel/oneapi/setvars.sh intel64
-    ```
-
-## Install MKL on Ubuntu with apt
-
-Intel MKL can be installed with apt on Ubuntu. A guide can be found in [here](https://neelravi.com/post/intel-oneapi-install/).
-For example to install the MKL 2022 version
-
-```console
-sudo bash
-# <type your user password when prompted.  this will put you in a root shell>
-# If they are not installed, you can install using the following command:
-sudo apt update
-sudo apt -y install cmake pkg-config build-essential
-# use wget to fetch the Intel repository public key
-wget https://apt.repos.intel.com/intel-gpg-keys/GPG-PUB-KEY-INTEL-SW-PRODUCTS.PUB
-# add to your apt sources keyring so that archives signed with this key will be trusted.
-sudo apt-key add GPG-PUB-KEY-INTEL-SW-PRODUCTS.PUB
-# remove the public key
-rm GPG-PUB-KEY-INTEL-SW-PRODUCTS.PUB
-# Configure apt client to use Intel repository
-sudo add-apt-repository "deb https://apt.repos.intel.com/oneapi all main"
-# Install all MKL related dependencies. You can install full HPC with: sudo apt install intel-hpckit
-sudo apt install intel-oneapi-mkl-devel
-# Exit
-exit
-```
-
-To enable the MKL environment (needs to be done before build/run) use
-
-```console
-source /opt/intel/oneapi/setvars.sh intel64
-```
+Metadata-Version: 2.1
+Name: KratosLinearSolversApplication
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
+# LinearSolversApplication
+
+The *LinearSolversApplication* is a thin wrapper for the [Eigen linear algebra library](http://eigen.tuxfamily.org/index.php?title=Main_Page).
+
+## Direct sparse solvers
+
+The application provides the following direct sparse solvers:
+
+| Python class             | solver_type            | Matrix kind | Domain   | Dependencies |
+|--------------------------|------------------------|:-----------:|:--------:|:------------:|
+| SparseLUSolver           | `sparse_lu`            | Square      | Real     | None         |
+| SparseQRSolver           | `sparse_qr`            | Rectangular | Real     | None         |
+| SparseCGSolver           | `sparse_cg`            | SPD*        | Real     | None         |
+| PardisoLLTSolver         | `pardiso_llt`          | SPD*        | Real     | Intel® MKL   |
+| PardisoLDLTSolver        | `pardiso_ldlt`         | SPD*        | Real     | Intel® MKL   |
+| PardisoLUSolver          | `pardiso_lu`           | Square      | Real     | Intel® MKL   |
+| ComplexSparseLUSolver    | `sparse_lu_complex`    | Square      | Complex  | None         |
+| ComplexPardisoLLTSolver  | `pardiso_llt_complex`  | SPD*        | Complex  | Intel® MKL   |
+| ComplexPardisoLDLTSolver | `pardiso_ldlt_complex` | SPD*        | Complex  | Intel® MKL   |
+| ComplexPardisoLUSolver   | `pardiso_lu_complex`   | Square      | Complex  | Intel® MKL   |
+
+*SPD = Symmetric Positive Definite
+
+**Example**:
+
+```json
+{
+    "solver_type": "eigen_sparse_lu"
+}
+```
+
+## Direct dense solvers
+
+The application provides the following direct solvers for dense systems of equations:
+
+| Python class                            | solver_type                            | Matrix requirements | Domain  | Dependencies |
+| --------------------------------------- | -------------------------------------- | :-----------------: | :-----: | :----------: |
+| DenseColPivHouseholderQRSolver**        | `dense_col_piv_householder_qr`         |        None         |  Real   |     None     |
+| DenseHouseholderQRSolver**              | `dense_householder_qr`                 |        None         |  Real   |     None     |
+| DenseLLTSolver**                        | `dense_llt`                            |        SPD*         |  Real   |     None     |
+| DensePartialPivLUSolver**               | `dense_partial_piv_lu`                 |     Invertible      |  Real   |     None     |
+| ComplexDenseColPivHouseholderQRSolver   | `complex_dense_col_piv_householder_qr` |        None         | Complex |     None     |
+| ComplexDenseHouseholderQRSolver         | `complex_dense_householder_qr`         |        None         | Complex |     None     |
+| ComplexDensePartialPivLUSolver          | `complex_dense_partial_piv_lu`         |     Invertible      | Complex |     None     |
+
+*SPD = Symmetric Positive Definite
+
+**Can also be used to solve equation systems with multiple right hand sides.
+
+## Generalized eigensystem solvers
+
+The application provides the following generalized eigensystem `Ax=λBx` solver for sparse matrices.
+
+| Python class                           | solver_type                | Matrix kind A | Matrix kind B | Domain   | Dependencies |
+|----------------------------------------|----------------------------|:-------------:|:-------------:|:--------:|:------------:|
+| EigensystemSolver                      | `eigen_eigensystem`        | Symmetric     | SPD*          | Real     | None         |
+| SpectraSymGEigsShiftSolver             | `spectra_sym_g_eigs_shift` | Symmetric     | SPD*          | Real     | None         |
+| FEASTGeneralEigensystemSolver**        | `feast`                    | General       | General       | Real     | Intel® MKL   |
+| ComplexFEASTGeneralEigensystemSolver** | `feast_complex`            | General       | General       | Complex  | Intel® MKL   |
+
+*SPD = Symmetric Positive Definite
+**A special version for symmetric matrices can be triggered in the solver settings.
+
+`EigensystemSolver` and `SpectraSymGEigsShiftSolver` compute the smallest eigenvalues and corresponding eigenvectors of the system. MKL routines are used automatically if they are available.
+
+`SpectraSymGEigsShiftSolver` interfaces a solver from the [Spectra library](https://spectralib.org/), and has a shift mode that can be used to compute the smallest eigenvalues > `shift`.
+
+**Example:**
+
+```json
+{
+    "solver_type": "spectra_sym_g_eigs_shift",
+    "number_of_eigenvalues": 3,
+    "max_iteration": 1000,
+    "echo_level": 1
+}
+
+```
+If the application is compiled with MKL, [FEAST 4.0](http://www.ecs.umass.edu/~polizzi/feast/) can be used to solve the generalized eigenvalue problem for real and complex systems (symmetric or unsymmetric). The cmake switch `USE_EIGEN_FEAST` must be set to `ON` with
+```batch
+-DUSE_EIGEN_FEAST=ON \
+```
+
+**Example:**
+```json
+{
+    "solver_type": "feast",
+    "symmetric": true,
+    "number_of_eigenvalues": 3,
+    "search_lowest_eigenvalues": true,
+    "e_min" : 0.0,
+    "e_max" : 0.2
+}
+```
+
+## Build instructions
+
+1. Set the required definitions for cmake
+
+    As any other app:
+
+    **Windows:** in `configure.bat`
+
+    ```batch
+    set KRATOS_APPLICATIONS=%KRATOS_APPLICATIONS%%KRATOS_APP_DIR%\LinearSolversApplication;
+    ```
+
+    **Linux:** in `configure.sh`
+
+    ```console
+    add_app ${KRATOS_APP_DIR}/LinearSolversApplication
+    ```
+
+2. Build Kratos
+
+3. Setup the `ProjectParameters.json`
+
+    ```json
+    "linear_solver_settings": {
+        "solver_type" : "LinearSolversApplication.sparse_lu"
+    }
+    ```
+
+4. Run the simulation
+
+## Enable MKL (optional)
+
+In case you have installed [MKL](https://software.intel.com/en-us/mkl) (see below), you can also use the Pardiso solvers.
+
+1. Run the MKL setup script before building Kratos:
+
+    **Windows:**
+
+    ```batch
+    call "C:\Program Files (x86)\Intel\oneAPI\mkl\latest\env\vars.bat" intel64 lp64
+    ```
+
+    **Linux:**
+
+    ```console
+    source /opt/intel/oneapi/setvars.sh intel64
+    ```
+
+2. Add the following flag to CMake to your configure script:
+
+    **Windows:**
+
+    ```batch
+    -DUSE_EIGEN_MKL=ON ^
+    ```
+
+    **Linux:**
+
+    ```console
+    -DUSE_EIGEN_MKL=ON \
+    ```
+
+3. Build Kratos
+
+4. Usage:
+
+    **Windows:**
+
+    ```batch
+    call "C:\Program Files (x86)\Intel\oneAPI\mkl\latest\env\vars.bat" intel64 lp64
+    ```
+
+    **Linux:**
+
+    Set the environment before using MKL
+
+    ```console
+    source /opt/intel/oneapi/setvars.sh intel64
+    ```
+
+## Install MKL on Ubuntu with apt
+
+Intel MKL can be installed with apt on Ubuntu. A guide can be found in [here](https://neelravi.com/post/intel-oneapi-install/).
+For example to install the MKL 2022 version
+
+```console
+sudo bash
+# <type your user password when prompted.  this will put you in a root shell>
+# If they are not installed, you can install using the following command:
+sudo apt update
+sudo apt -y install cmake pkg-config build-essential
+# use wget to fetch the Intel repository public key
+wget https://apt.repos.intel.com/intel-gpg-keys/GPG-PUB-KEY-INTEL-SW-PRODUCTS.PUB
+# add to your apt sources keyring so that archives signed with this key will be trusted.
+sudo apt-key add GPG-PUB-KEY-INTEL-SW-PRODUCTS.PUB
+# remove the public key
+rm GPG-PUB-KEY-INTEL-SW-PRODUCTS.PUB
+# Configure apt client to use Intel repository
+sudo add-apt-repository "deb https://apt.repos.intel.com/oneapi all main"
+# Install all MKL related dependencies. You can install full HPC with: sudo apt install intel-hpckit
+sudo apt install intel-oneapi-mkl-devel
+# Exit
+exit
+```
+
+To enable the MKL environment (needs to be done before build/run) use
+
+```console
+source /opt/intel/oneapi/setvars.sh intel64
+```
```

