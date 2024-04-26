# Comparing `tmp/KratosCSharpWrapperApplication-9.4.6-cp39-cp39-win_amd64.whl.zip` & `tmp/KratosCSharpWrapperApplication-9.5-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,249 +1,492 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    495446 (0000000000078F56h)
-  Actual end-cent-dir record offset:        495424 (0000000000078F40h)
-  Expected end-cent-dir record offset:      495424 (0000000000078F40h)
+  Zip archive file size:                   9104039 (00000000008AEAA7h)
+  Actual end-cent-dir record offset:       9104017 (00000000008AEA91h)
+  Expected end-cent-dir record offset:     9104017 (00000000008AEA91h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 8 entries.
-  The central directory is 806 (0000000000000326h) bytes long,
+  central directory contains 13 entries.
+  The central directory is 1587 (0000000000000633h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 494618 (0000000000078C1Ah).
+  is 9102430 (00000000008AE45Eh).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosCSharpWrapperApplication.pyd
+  KratosCSharpWrapperApplication-9.5.dist-info/
 
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
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:32
-  32-bit CRC value (hex):                         b65f6a22
-  compressed size:                                155066 bytes
-  uncompressed size:                              436224 bytes
-  length of filename:                             59 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:44
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:44 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:44 UTC
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
 
-  KratosMultiphysics/.libs/KratosCSharpWrapperCore.dll
+  KratosCSharpWrapperApplication-9.5.dist-info/METADATA
 
-  offset of local header from start of archive:   155155
-                                                  (0000000000025E13h) bytes
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
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:32
-  32-bit CRC value (hex):                         a1e09b29
-  compressed size:                                333714 bytes
-  uncompressed size:                              1086976 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 UTC
+  32-bit CRC value (hex):                         8ecd918f
+  compressed size:                                550 bytes
+  uncompressed size:                              1353 bytes
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
 
-  KratosMultiphysics/.libs/KratosCSharpWrapperCore.lib
+  KratosCSharpWrapperApplication-9.5.dist-info/WHEEL
 
-  offset of local header from start of archive:   488951
-                                                  (00000000000775F7h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   764
+                                                  (00000000000002FCh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:32
-  32-bit CRC value (hex):                         50c06088
-  compressed size:                                3911 bytes
-  uncompressed size:                              25736 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 UTC
+  32-bit CRC value (hex):                         a9cd4497
+  compressed size:                                117 bytes
+  uncompressed size:                              152 bytes
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
 
-  KratosMultiphysics/CSharpWrapperApplication/__init__.py
+  KratosCSharpWrapperApplication-9.5.dist-info/top_level.txt
+
+  offset of local header from start of archive:   989
+                                                  (00000000000003DDh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 UTC
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
+  KratosCSharpWrapperApplication-9.5.dist-info/RECORD
 
-  offset of local header from start of archive:   492944
-                                                  (0000000000078590h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1124
+                                                  (0000000000000464h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:40
-  32-bit CRC value (hex):                         0cb24ba6
-  compressed size:                                135 bytes
-  uncompressed size:                              309 bytes
-  length of filename:                             55 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:44
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:44 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:44 UTC
+  32-bit CRC value (hex):                         8202397c
+  compressed size:                                543 bytes
+  uncompressed size:                              1039 bytes
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
 
-  KratosCSharpWrapperApplication-9.4.6.dist-info/METADATA
+  KratosCSharpWrapperApplication.libs/
 
-  offset of local header from start of archive:   493164
-                                                  (000000000007866Ch) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1776
+                                                  (00000000000006F0h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:44
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:44 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:44 UTC
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
+  KratosCSharpWrapperApplication.libs/libKratosStructuralMechanicsCore-d06c43d3.so
+
+  offset of local header from start of archive:   1870
+                                                  (000000000000074Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:32
-  32-bit CRC value (hex):                         9f5d1fa0
-  compressed size:                                562 bytes
-  uncompressed size:                              1385 bytes
-  length of filename:                             55 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 UTC
+  32-bit CRC value (hex):                         5595483d
+  compressed size:                                7316396 bytes
+  uncompressed size:                              25336065 bytes
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
 
-Central directory entry #6:
+Central directory entry #8:
 ---------------------------
 
-  KratosCSharpWrapperApplication-9.4.6.dist-info/WHEEL
+  KratosCSharpWrapperApplication.libs/libKratosCSharpWrapperCore-ad3cc3cd.so
 
-  offset of local header from start of archive:   493811
-                                                  (00000000000788F3h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   7318404
+                                                  (00000000006FAB84h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:32
-  32-bit CRC value (hex):                         86fb6b41
-  compressed size:                                96 bytes
-  uncompressed size:                              100 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 UTC
+  32-bit CRC value (hex):                         6c5a6b7f
+  compressed size:                                1257014 bytes
+  uncompressed size:                              5981969 bytes
+  length of filename:                             74 characters
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
+Central directory entry #9:
+---------------------------
+
+  KratosMultiphysics/
+
+  offset of local header from start of archive:   8575550
+                                                  (000000000082DA3Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 UTC
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
+Central directory entry #10:
+---------------------------
+
+  KratosMultiphysics/.libs/
+
+  offset of local header from start of archive:   8575627
+                                                  (000000000082DA8Bh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:44
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:44 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:44 UTC
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
+Central directory entry #11:
 ---------------------------
 
-  KratosCSharpWrapperApplication-9.4.6.dist-info/top_level.txt
+  KratosMultiphysics/.libs/KratosCSharpWrapperApplication.cpython-310-x86_64-linux-gnu.so
 
-  offset of local header from start of archive:   493989
-                                                  (00000000000789A5h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   8575710
+                                                  (000000000082DADEh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:32
-  32-bit CRC value (hex):                         f32d789f
-  compressed size:                                21 bytes
-  uncompressed size:                              19 bytes
-  length of filename:                             60 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 UTC
+  32-bit CRC value (hex):                         ea5ce8fa
+  compressed size:                                526229 bytes
+  uncompressed size:                              1542697 bytes
+  length of filename:                             87 characters
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
 
-Central directory entry #8:
+Central directory entry #12:
 ---------------------------
 
-  KratosCSharpWrapperApplication-9.4.6.dist-info/RECORD
+  KratosMultiphysics/CSharpWrapperApplication/
 
-  offset of local header from start of archive:   494100
-                                                  (0000000000078A14h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   9102084
+                                                  (00000000008AE304h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 UTC
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
+Central directory entry #13:
+---------------------------
+
+  KratosMultiphysics/CSharpWrapperApplication/__init__.py
+
+  offset of local header from start of archive:   9102186
+                                                  (00000000008AE36Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:32
-  32-bit CRC value (hex):                         5b007ff5
-  compressed size:                                435 bytes
-  uncompressed size:                              842 bytes
-  length of filename:                             53 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:09:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:09:36 UTC
+  32-bit CRC value (hex):                         f3e7c911
+  compressed size:                                131 bytes
+  uncompressed size:                              302 bytes
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
@@ -1,25 +1,40 @@
-Filename: KratosMultiphysics/.libs/KratosCSharpWrapperApplication.pyd
+Filename: KratosCSharpWrapperApplication-9.5.dist-info/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosCSharpWrapperCore.dll
+Filename: KratosCSharpWrapperApplication-9.5.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosCSharpWrapperCore.lib
+Filename: KratosCSharpWrapperApplication-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics/CSharpWrapperApplication/__init__.py
+Filename: KratosCSharpWrapperApplication-9.5.dist-info/top_level.txt
+Comment: 
+
+Filename: KratosCSharpWrapperApplication-9.5.dist-info/RECORD
+Comment: 
+
+Filename: KratosCSharpWrapperApplication.libs/
+Comment: 
+
+Filename: KratosCSharpWrapperApplication.libs/libKratosStructuralMechanicsCore-d06c43d3.so
+Comment: 
+
+Filename: KratosCSharpWrapperApplication.libs/libKratosCSharpWrapperCore-ad3cc3cd.so
 Comment: 
 
-Filename: KratosCSharpWrapperApplication-9.4.6.dist-info/METADATA
+Filename: KratosMultiphysics/
 Comment: 
 
-Filename: KratosCSharpWrapperApplication-9.4.6.dist-info/WHEEL
+Filename: KratosMultiphysics/.libs/
 Comment: 
 
-Filename: KratosCSharpWrapperApplication-9.4.6.dist-info/top_level.txt
+Filename: KratosMultiphysics/.libs/KratosCSharpWrapperApplication.cpython-310-x86_64-linux-gnu.so
 Comment: 
 
-Filename: KratosCSharpWrapperApplication-9.4.6.dist-info/RECORD
+Filename: KratosMultiphysics/CSharpWrapperApplication/
+Comment: 
+
+Filename: KratosMultiphysics/CSharpWrapperApplication/__init__.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## KratosMultiphysics/CSharpWrapperApplication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-from KratosMultiphysics import _ImportApplication
-import KratosMultiphysics.StructuralMechanicsApplication
-from KratosCSharpWrapperApplication import *
-application = KratosCSharpWrapperApplication()
-application_name = "KratosCSharpWrapperApplication"
-
-_ImportApplication(application, application_name)
+from KratosMultiphysics import _ImportApplication
+import KratosMultiphysics.StructuralMechanicsApplication
+from KratosCSharpWrapperApplication import *
+application = KratosCSharpWrapperApplication()
+application_name = "KratosCSharpWrapperApplication"
+
+_ImportApplication(application, application_name)
```

## Comparing `KratosCSharpWrapperApplication-9.4.6.dist-info/METADATA` & `KratosCSharpWrapperApplication-9.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1
-Name: KratosCSharpWrapperApplication
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
+Metadata-Version: 2.1
+Name: KratosCSharpWrapperApplication
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
```

## Comparing `KratosCSharpWrapperApplication-9.4.6.dist-info/RECORD` & `KratosCSharpWrapperApplication-9.5.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-KratosMultiphysics/.libs/KratosCSharpWrapperApplication.pyd,sha256=B18EHb2x5lxpshcwq0cP3QA1MTnYZaD-DJ6Dzs5ZEic,436224
-KratosMultiphysics/.libs/KratosCSharpWrapperCore.dll,sha256=V-YDJHcK1Qs6mnXHvS4o6RkP-6JhGVM24Tcpi73yTMg,1086976
-KratosMultiphysics/.libs/KratosCSharpWrapperCore.lib,sha256=A8FJyWFNVympwH7rSIew_4WLs7FODR9PeWtDMWR9N60,25736
-KratosMultiphysics/CSharpWrapperApplication/__init__.py,sha256=5qwQ4UhZEL6wzXSh-1z6_6vXP8-aCIhDCNYTd9CVw2w,309
-KratosCSharpWrapperApplication-9.4.6.dist-info/METADATA,sha256=yPLwja9442Tja-iKo0bkxfHnuwE-dxt0TCx7xxjtMus,1385
-KratosCSharpWrapperApplication-9.4.6.dist-info/WHEEL,sha256=GZFS91_ufm4WrNPBaFVPB9MvOXR6bMZQhPcZRRTN5YM,100
-KratosCSharpWrapperApplication-9.4.6.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
-KratosCSharpWrapperApplication-9.4.6.dist-info/RECORD,,
+KratosCSharpWrapperApplication-9.5.dist-info/METADATA,sha256=Jhk3QlVendsqCln7e1F6JcHmWvzh_NmyPfNLibG0eUU,1353
+KratosCSharpWrapperApplication-9.5.dist-info/WHEEL,sha256=CzQQWV-lNyM92gr3iaBk8dvO35YDHRxgzkZ-dxumUIM,152
+KratosCSharpWrapperApplication-9.5.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
+KratosCSharpWrapperApplication-9.5.dist-info/RECORD,,
+KratosMultiphysics/.libs/KratosCSharpWrapperApplication.cpython-310-x86_64-linux-gnu.so,sha256=JUJ_Cpq6vHrm7CGU1bb_xZm5fklosDoCXLTABp6A0vk,1542697
+KratosMultiphysics/.libs/libKratosCSharpWrapperCore.so,sha256=ZhM8axQIQ_M27X0dhh3Unx92ErGRazjkP97RTzuR9Kk,5478817
+KratosMultiphysics/CSharpWrapperApplication/__init__.py,sha256=IHJ_xbWBRdO8NqQshij80YDJwYavnGUzqi7Db3IBcks,302
+KratosCSharpWrapperApplication.libs/libKratosStructuralMechanicsCore-d06c43d3.so,sha256=kNNiTF23PiVxUu9fFewusHGA6gRiSZAAuDgtvIThy0U,25336065
+KratosCSharpWrapperApplication.libs/libKratosCSharpWrapperCore-ad3cc3cd.so,sha256=Lzv-Frernbc3ARbWpJ10Qz_aFHLIs2PhEasXOWmb9Dk,5981969
```

