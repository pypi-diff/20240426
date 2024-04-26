# Comparing `tmp/KratosFSIApplication-9.4.6-cp39-cp39-win_amd64.whl.zip` & `tmp/KratosFSIApplication-9.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,481 +1,751 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    641153 (000000000009C881h)
-  Actual end-cent-dir record offset:        641131 (000000000009C86Bh)
-  Expected end-cent-dir record offset:      641131 (000000000009C86Bh)
+  Zip archive file size:                   1793131 (00000000001B5C6Bh)
+  Actual end-cent-dir record offset:       1793109 (00000000001B5C55h)
+  Expected end-cent-dir record offset:     1793109 (00000000001B5C55h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 16 entries.
-  The central directory is 1601 (0000000000000641h) bytes long,
+  central directory contains 20 entries.
+  The central directory is 2393 (0000000000000959h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 639530 (000000000009C22Ah).
+  is 1790716 (00000000001B52FCh).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosFSIApplication.pyd
+  KratosFSIApplication-9.5.dist-info/
 
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
-  32-bit CRC value (hex):                         7cb18ec4
-  compressed size:                                325146 bytes
-  uncompressed size:                              999424 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:22
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:21 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:21 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             35 characters
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
 
-  KratosMultiphysics/.libs/KratosFSICore.dll
+  KratosFSIApplication-9.5.dist-info/METADATA
 
-  offset of local header from start of archive:   325225
-                                                  (000000000004F669h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   93
+                                                  (000000000000005Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:36
-  32-bit CRC value (hex):                         f0082827
-  compressed size:                                289102 bytes
-  uncompressed size:                              834048 bytes
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         78acffb8
+  compressed size:                                764 bytes
+  uncompressed size:                              1999 bytes
+  length of filename:                             43 characters
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
 
-  KratosMultiphysics/.libs/KratosFSICore.lib
+  KratosFSIApplication-9.5.dist-info/WHEEL
 
-  offset of local header from start of archive:   614399
-                                                  (0000000000095FFFh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   958
+                                                  (00000000000003BEh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:36
-  32-bit CRC value (hex):                         b7464076
-  compressed size:                                891 bytes
-  uncompressed size:                              4808 bytes
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         90d34e0d
+  compressed size:                                116 bytes
+  uncompressed size:                              148 bytes
+  length of filename:                             40 characters
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
 
-  KratosMultiphysics/FSIApplication/Conformant_OneSideMap.py
+  KratosFSIApplication-9.5.dist-info/top_level.txt
 
-  offset of local header from start of archive:   615362
-                                                  (00000000000963C2h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1172
+                                                  (0000000000000494h) bytes
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
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         d42cf054
-  compressed size:                                436 bytes
-  uncompressed size:                              1710 bytes
-  length of filename:                             58 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         f32d789f
+  compressed size:                                19 bytes
+  uncompressed size:                              19 bytes
+  length of filename:                             48 characters
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
 
 Central directory entry #5:
 ---------------------------
 
-  KratosMultiphysics/FSIApplication/__init__.py
+  KratosFSIApplication-9.5.dist-info/RECORD
 
-  offset of local header from start of archive:   615886
-                                                  (00000000000965CEh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1297
+                                                  (0000000000000511h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         07b0c9f5
-  compressed size:                                100 bytes
-  uncompressed size:                              221 bytes
-  length of filename:                             45 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:22
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:21 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:21 UTC
+  32-bit CRC value (hex):                         ce495eaa
+  compressed size:                                897 bytes
+  uncompressed size:                              1780 bytes
+  length of filename:                             41 characters
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
 
 Central directory entry #6:
 ---------------------------
 
-  KratosMultiphysics/FSIApplication/convergence_accelerator_factory.py
+  KratosFSIApplication.libs/
 
-  offset of local header from start of archive:   616061
-                                                  (000000000009667Dh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   2293
+                                                  (00000000000008F5h) bytes
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
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         ebf1121f
-  compressed size:                                863 bytes
-  uncompressed size:                              4108 bytes
-  length of filename:                             68 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:22
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:21 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:21 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             26 characters
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
 
 Central directory entry #7:
 ---------------------------
 
-  KratosMultiphysics/FSIApplication/fsi_analysis.py
+  KratosFSIApplication.libs/libKratosFSICore-f59bd74f.so
 
-  offset of local header from start of archive:   617022
-                                                  (0000000000096A3Eh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   2377
+                                                  (0000000000000949h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         a771932d
-  compressed size:                                2192 bytes
-  uncompressed size:                              9079 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         3ddc0517
+  compressed size:                                829457 bytes
+  uncompressed size:                              3564969 bytes
+  length of filename:                             54 characters
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
 
 Central directory entry #8:
 ---------------------------
 
-  KratosMultiphysics/FSIApplication/fsi_coupling_interface.py
+  KratosMultiphysics/
 
-  offset of local header from start of archive:   619293
-                                                  (000000000009731Dh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   831946
+                                                  (00000000000CB1CAh) bytes
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
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         5de53895
-  compressed size:                                3152 bytes
-  uncompressed size:                              20363 bytes
-  length of filename:                             59 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
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
 
 Central directory entry #9:
 ---------------------------
 
-  KratosMultiphysics/FSIApplication/partitioned_embedded_fsi_base_solver.py
+  KratosMultiphysics/FSIApplication/
 
-  offset of local header from start of archive:   622534
-                                                  (0000000000097FC6h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   832023
+                                                  (00000000000CB217h) bytes
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
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         a74ef35c
-  compressed size:                                4631 bytes
-  uncompressed size:                              28117 bytes
-  length of filename:                             73 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             34 characters
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
 
 Central directory entry #10:
 ---------------------------
 
-  KratosMultiphysics/FSIApplication/partitioned_fsi_base_solver.py
+  KratosMultiphysics/FSIApplication/trilinos_partitioned_fsi_base_solver.py
 
-  offset of local header from start of archive:   627268
-                                                  (0000000000099244h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   832115
+                                                  (00000000000CB273h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         a2f17e20
-  compressed size:                                8021 bytes
-  uncompressed size:                              45501 bytes
-  length of filename:                             64 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         20296d77
+  compressed size:                                1269 bytes
+  uncompressed size:                              4797 bytes
+  length of filename:                             73 characters
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
 
-  KratosMultiphysics/FSIApplication/python_solvers_wrapper_fsi.py
+  KratosMultiphysics/FSIApplication/Conformant_OneSideMap.py
 
-  offset of local header from start of archive:   635383
-                                                  (000000000009B1F7h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   833515
+                                                  (00000000000CB7EBh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         1efbc9fc
-  compressed size:                                604 bytes
-  uncompressed size:                              3073 bytes
-  length of filename:                             63 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         d4ab453d
+  compressed size:                                428 bytes
+  uncompressed size:                              1674 bytes
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
 
 Central directory entry #12:
 ---------------------------
 
-  KratosMultiphysics/FSIApplication/trilinos_partitioned_fsi_base_solver.py
+  KratosMultiphysics/FSIApplication/python_solvers_wrapper_fsi.py
 
-  offset of local header from start of archive:   636080
-                                                  (000000000009B4B0h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   834059
+                                                  (00000000000CBA0Bh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         840836f7
-  compressed size:                                1283 bytes
-  uncompressed size:                              4898 bytes
-  length of filename:                             73 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         86c455ab
+  compressed size:                                599 bytes
+  uncompressed size:                              3010 bytes
+  length of filename:                             63 characters
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
 
 Central directory entry #13:
 ---------------------------
 
-  KratosFSIApplication-9.4.6.dist-info/METADATA
+  KratosMultiphysics/FSIApplication/convergence_accelerator_factory.py
 
-  offset of local header from start of archive:   637466
-                                                  (000000000009BA1Ah) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   834779
+                                                  (00000000000CBCDBh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:36
-  32-bit CRC value (hex):                         c9118c95
-  compressed size:                                780 bytes
-  uncompressed size:                              2056 bytes
-  length of filename:                             45 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         213301bb
+  compressed size:                                854 bytes
+  uncompressed size:                              4025 bytes
+  length of filename:                             68 characters
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
 
 Central directory entry #14:
 ---------------------------
 
-  KratosFSIApplication-9.4.6.dist-info/WHEEL
+  KratosMultiphysics/FSIApplication/fsi_coupling_interface.py
 
-  offset of local header from start of archive:   638321
-                                                  (000000000009BD71h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   835759
+                                                  (00000000000CC0AFh) bytes
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
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         46a4867a
+  compressed size:                                3133 bytes
+  uncompressed size:                              19993 bytes
+  length of filename:                             59 characters
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
 
 Central directory entry #15:
 ---------------------------
 
-  KratosFSIApplication-9.4.6.dist-info/top_level.txt
+  KratosMultiphysics/FSIApplication/partitioned_fsi_base_solver.py
 
-  offset of local header from start of archive:   638489
-                                                  (000000000009BE19h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   839009
+                                                  (00000000000CCD61h) bytes
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
-  length of filename:                             50 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         1b118358
+  compressed size:                                7990 bytes
+  uncompressed size:                              44681 bytes
+  length of filename:                             64 characters
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
 
 Central directory entry #16:
 ---------------------------
 
-  KratosFSIApplication-9.4.6.dist-info/RECORD
+  KratosMultiphysics/FSIApplication/partitioned_embedded_fsi_base_solver.py
 
-  offset of local header from start of archive:   638590
-                                                  (000000000009BE7Eh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   847121
+                                                  (00000000000CED11h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:36
-  32-bit CRC value (hex):                         a3622727
-  compressed size:                                867 bytes
-  uncompressed size:                              1726 bytes
-  length of filename:                             43 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         7e4104dc
+  compressed size:                                4602 bytes
+  uncompressed size:                              27593 bytes
+  length of filename:                             73 characters
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
+Central directory entry #17:
+---------------------------
+
+  KratosMultiphysics/FSIApplication/__init__.py
+
+  offset of local header from start of archive:   851854
+                                                  (00000000000CFF8Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         b1924fd1
+  compressed size:                                96 bytes
+  uncompressed size:                              215 bytes
+  length of filename:                             45 characters
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
+Central directory entry #18:
+---------------------------
+
+  KratosMultiphysics/FSIApplication/fsi_analysis.py
+
+  offset of local header from start of archive:   852053
+                                                  (00000000000D0055h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         91eb8b6f
+  compressed size:                                2177 bytes
+  uncompressed size:                              8884 bytes
+  length of filename:                             49 characters
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
+  KratosMultiphysics/.libs/
+
+  offset of local header from start of archive:   854337
+                                                  (00000000000D0941h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:22
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:21 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:21 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             25 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B400 hex
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
+  KratosMultiphysics/.libs/KratosFSIApplication.cpython-39-x86_64-linux-gnu.so
+
+  offset of local header from start of archive:   854420
+                                                  (00000000000D0994h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:59:16
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:16 UTC
+  32-bit CRC value (hex):                         5d4b688e
+  compressed size:                                936162 bytes
+  uncompressed size:                              2677841 bytes
+  length of filename:                             76 characters
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
@@ -1,49 +1,61 @@
-Filename: KratosMultiphysics/.libs/KratosFSIApplication.pyd
+Filename: KratosFSIApplication-9.5.dist-info/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosFSICore.dll
+Filename: KratosFSIApplication-9.5.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosFSICore.lib
+Filename: KratosFSIApplication-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics/FSIApplication/Conformant_OneSideMap.py
+Filename: KratosFSIApplication-9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosMultiphysics/FSIApplication/__init__.py
+Filename: KratosFSIApplication-9.5.dist-info/RECORD
 Comment: 
 
-Filename: KratosMultiphysics/FSIApplication/convergence_accelerator_factory.py
+Filename: KratosFSIApplication.libs/
 Comment: 
 
-Filename: KratosMultiphysics/FSIApplication/fsi_analysis.py
+Filename: KratosFSIApplication.libs/libKratosFSICore-f59bd74f.so
 Comment: 
 
-Filename: KratosMultiphysics/FSIApplication/fsi_coupling_interface.py
+Filename: KratosMultiphysics/
 Comment: 
 
-Filename: KratosMultiphysics/FSIApplication/partitioned_embedded_fsi_base_solver.py
+Filename: KratosMultiphysics/FSIApplication/
 Comment: 
 
-Filename: KratosMultiphysics/FSIApplication/partitioned_fsi_base_solver.py
+Filename: KratosMultiphysics/FSIApplication/trilinos_partitioned_fsi_base_solver.py
+Comment: 
+
+Filename: KratosMultiphysics/FSIApplication/Conformant_OneSideMap.py
 Comment: 
 
 Filename: KratosMultiphysics/FSIApplication/python_solvers_wrapper_fsi.py
 Comment: 
 
-Filename: KratosMultiphysics/FSIApplication/trilinos_partitioned_fsi_base_solver.py
+Filename: KratosMultiphysics/FSIApplication/convergence_accelerator_factory.py
+Comment: 
+
+Filename: KratosMultiphysics/FSIApplication/fsi_coupling_interface.py
+Comment: 
+
+Filename: KratosMultiphysics/FSIApplication/partitioned_fsi_base_solver.py
+Comment: 
+
+Filename: KratosMultiphysics/FSIApplication/partitioned_embedded_fsi_base_solver.py
 Comment: 
 
-Filename: KratosFSIApplication-9.4.6.dist-info/METADATA
+Filename: KratosMultiphysics/FSIApplication/__init__.py
 Comment: 
 
-Filename: KratosFSIApplication-9.4.6.dist-info/WHEEL
+Filename: KratosMultiphysics/FSIApplication/fsi_analysis.py
 Comment: 
 
-Filename: KratosFSIApplication-9.4.6.dist-info/top_level.txt
+Filename: KratosMultiphysics/.libs/
 Comment: 
 
-Filename: KratosFSIApplication-9.4.6.dist-info/RECORD
+Filename: KratosMultiphysics/.libs/KratosFSIApplication.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## KratosMultiphysics/FSIApplication/Conformant_OneSideMap.py

 * *Ordering differences only*

```diff
@@ -1,36 +1,36 @@
-
-# Importing the Kratos Library
-from KratosMultiphysics import *
-
-# Import applications
-from KratosMultiphysics.FSIApplication import *
-
-def AddVariables(fluid_model_part, structure_model_part):
-    fluid_model_part.AddNodalSolutionStepVariable(PRESSURE)
-    fluid_model_part.AddNodalSolutionStepVariable(DISPLACEMENT)
-    fluid_model_part.AddNodalSolutionStepVariable(IS_INTERFACE)
-
-    structure_model_part.AddNodalSolutionStepVariable(PRESSURE)
-    structure_model_part.AddNodalSolutionStepVariable(DISPLACEMENT)
-    structure_model_part.AddNodalSolutionStepVariable(IS_INTERFACE)
-
-    print("variables for the mesh solver added correctly")
-
-
-class Conformant_OneSideMap:
-
-    def __init__(self, fluid_model_part_nodes, structure_model_part_nodes):
-        self.FluidToStructureMapper = SharedPointsMapper(fluid_model_part_nodes, structure_model_part_nodes, 1e-9)
-        self.StructureToFluidMapper = SharedPointsMapper(structure_model_part_nodes, fluid_model_part_nodes, 1e-9)
-
-    def StructureToFluid_VectorMap(self, VectorVar_Origin, VectorVar_Destination):
-        (self.StructureToFluidMapper).VectorMap(VectorVar_Origin, VectorVar_Destination)
-
-    def StructureToFluid_ScalarMap(self, ScalarVar_Origin, ScalarVar_Destination):
-        (self.StructureToFluidMapper).ScalarMap(ScalarVar_Origin, ScalarVar_Destination)
-
-    def FluidToStructure_VectorMap(self, VectorVar_Origin, VectorVar_Destination):
-        (self.FluidToStructureMapper).VectorMap(VectorVar_Origin, VectorVar_Destination)
-
-    def FluidToStructure_ScalarMap(self, ScalarVar_Origin, ScalarVar_Destination):
-        (self.FluidToStructureMapper).ScalarMap(ScalarVar_Origin, ScalarVar_Destination)
+
+# Importing the Kratos Library
+from KratosMultiphysics import *
+
+# Import applications
+from KratosMultiphysics.FSIApplication import *
+
+def AddVariables(fluid_model_part, structure_model_part):
+    fluid_model_part.AddNodalSolutionStepVariable(PRESSURE)
+    fluid_model_part.AddNodalSolutionStepVariable(DISPLACEMENT)
+    fluid_model_part.AddNodalSolutionStepVariable(IS_INTERFACE)
+
+    structure_model_part.AddNodalSolutionStepVariable(PRESSURE)
+    structure_model_part.AddNodalSolutionStepVariable(DISPLACEMENT)
+    structure_model_part.AddNodalSolutionStepVariable(IS_INTERFACE)
+
+    print("variables for the mesh solver added correctly")
+
+
+class Conformant_OneSideMap:
+
+    def __init__(self, fluid_model_part_nodes, structure_model_part_nodes):
+        self.FluidToStructureMapper = SharedPointsMapper(fluid_model_part_nodes, structure_model_part_nodes, 1e-9)
+        self.StructureToFluidMapper = SharedPointsMapper(structure_model_part_nodes, fluid_model_part_nodes, 1e-9)
+
+    def StructureToFluid_VectorMap(self, VectorVar_Origin, VectorVar_Destination):
+        (self.StructureToFluidMapper).VectorMap(VectorVar_Origin, VectorVar_Destination)
+
+    def StructureToFluid_ScalarMap(self, ScalarVar_Origin, ScalarVar_Destination):
+        (self.StructureToFluidMapper).ScalarMap(ScalarVar_Origin, ScalarVar_Destination)
+
+    def FluidToStructure_VectorMap(self, VectorVar_Origin, VectorVar_Destination):
+        (self.FluidToStructureMapper).VectorMap(VectorVar_Origin, VectorVar_Destination)
+
+    def FluidToStructure_ScalarMap(self, ScalarVar_Origin, ScalarVar_Destination):
+        (self.FluidToStructureMapper).ScalarMap(ScalarVar_Origin, ScalarVar_Destination)
```

## KratosMultiphysics/FSIApplication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-from KratosMultiphysics import _ImportApplication
-from KratosFSIApplication import *
-application = KratosFSIApplication()
-application_name = "KratosFSIApplication"
-
-_ImportApplication(application, application_name)
+from KratosMultiphysics import _ImportApplication
+from KratosFSIApplication import *
+application = KratosFSIApplication()
+application_name = "KratosFSIApplication"
+
+_ImportApplication(application, application_name)
```

## KratosMultiphysics/FSIApplication/convergence_accelerator_factory.py

 * *Ordering differences only*

```diff
@@ -1,83 +1,83 @@
-
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications
-import KratosMultiphysics.FSIApplication as KratosFSI
-
-import KratosMultiphysics.kratos_utilities as KratosUtilities
-have_trilinos = KratosUtilities.CheckIfApplicationsAvailable("TrilinosApplication")
-is_distributed = KratosMultiphysics.DataCommunicator.GetDefault().IsDistributed()
-if have_trilinos and is_distributed:
-    try:
-        import KratosMultiphysics.TrilinosApplication as KratosTrilinos
-    except Exception as e:
-        raise Exception("Trying to create a Trilinos convergence accelerator, but TrilinosApplication could not be found.")
-
-have_linear_solvers = KratosUtilities.CheckIfApplicationsAvailable("LinearSolversApplication")
-if have_linear_solvers:
-    import KratosMultiphysics.LinearSolversApplication as KratosLinearSolvers
-
-def CreateConvergenceAccelerator(configuration):
-
-    if(type(configuration) != KratosMultiphysics.Parameters):
-        raise Exception("Input is expected to be provided as a Kratos Parameters object.")
-
-    convergence_accelerator_type = configuration["solver_type"].GetString()
-
-    if(convergence_accelerator_type == "constant_relaxation"):
-        return KratosFSI.ConstantRelaxationConvergenceAccelerator(configuration)
-
-    elif(convergence_accelerator_type == "Relaxation"):
-        return KratosFSI.AitkenConvergenceAccelerator(configuration)
-
-    elif(convergence_accelerator_type == "MVQN"):
-        return KratosFSI.MVQNFullJacobianConvergenceAccelerator(configuration)
-
-    elif(convergence_accelerator_type == "MVQN_randomized_SVD"):
-        if not have_linear_solvers:
-            err_msg = "MVQN with randomized SVD Jacobian requires the \'LinearSolversApplication\'."
-            raise Exception(err_msg)
-        bdc_svd = KratosLinearSolvers.EigenDenseBDCSVD()
-        col_piv_qr = KratosLinearSolvers.EigenDenseColumnPivotingHouseholderQRDecomposition()
-        return KratosFSI.MVQNRandomizedSVDConvergenceAccelerator(col_piv_qr, bdc_svd, configuration)
-
-    elif(convergence_accelerator_type == "MVQN_recursive"):
-        return KratosFSI.MVQNRecursiveJacobianConvergenceAccelerator(configuration)
-
-    elif(convergence_accelerator_type == "IBQN_MVQN"):
-        return KratosFSI.IBQNMVQNConvergenceAccelerator(configuration)
-
-    elif(convergence_accelerator_type == "IBQN_MVQN_randomized_SVD"):
-        if not have_linear_solvers:
-            err_msg = "MVQN with randomized SVD Jacobian requires the \'LinearSolversApplication\'."
-            raise Exception(err_msg)
-        bdc_svd = KratosLinearSolvers.EigenDenseBDCSVD()
-        col_piv_qr = KratosLinearSolvers.EigenDenseColumnPivotingHouseholderQRDecomposition()
-        return KratosFSI.IBQNMVQNRandomizedSVDConvergenceAccelerator(col_piv_qr, bdc_svd, configuration)
-
-    else:
-        raise Exception("Convergence accelerator not found. Asking for : " + convergence_accelerator_type)
-
-    return convergence_accelerator
-
-def CreateTrilinosConvergenceAccelerator(interface_model_part, epetra_communicator, configuration):
-
-    if (type(interface_model_part) != KratosMultiphysics.ModelPart):
-        raise Exception("First input in Trilinos convergence accelerator factory is expceted to be provided as a Kratos ModelPart object.")
-
-    if(type(configuration) != KratosMultiphysics.Parameters):
-        raise Exception("Third input in Trilinos convergence accelerator factory is expected to be provided as a Kratos Parameters object.")
-
-    convergence_accelerator_type = configuration["solver_type"].GetString()
-
-    if(convergence_accelerator_type == "Relaxation"):
-        return KratosTrilinos.TrilinosAitkenConvergenceAccelerator(configuration)
-
-    elif(convergence_accelerator_type == "MVQN_recursive"):
-        return KratosTrilinos.TrilinosMVQNRecursiveJacobianConvergenceAccelerator(interface_model_part, epetra_communicator, configuration)
-
-    else:
-        raise Exception("Trilinos convergence accelerator not found. Asking for : " + convergence_accelerator_type)
-
-    return convergence_accelerator
+
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications
+import KratosMultiphysics.FSIApplication as KratosFSI
+
+import KratosMultiphysics.kratos_utilities as KratosUtilities
+have_trilinos = KratosUtilities.CheckIfApplicationsAvailable("TrilinosApplication")
+is_distributed = KratosMultiphysics.DataCommunicator.GetDefault().IsDistributed()
+if have_trilinos and is_distributed:
+    try:
+        import KratosMultiphysics.TrilinosApplication as KratosTrilinos
+    except Exception as e:
+        raise Exception("Trying to create a Trilinos convergence accelerator, but TrilinosApplication could not be found.")
+
+have_linear_solvers = KratosUtilities.CheckIfApplicationsAvailable("LinearSolversApplication")
+if have_linear_solvers:
+    import KratosMultiphysics.LinearSolversApplication as KratosLinearSolvers
+
+def CreateConvergenceAccelerator(configuration):
+
+    if(type(configuration) != KratosMultiphysics.Parameters):
+        raise Exception("Input is expected to be provided as a Kratos Parameters object.")
+
+    convergence_accelerator_type = configuration["solver_type"].GetString()
+
+    if(convergence_accelerator_type == "constant_relaxation"):
+        return KratosFSI.ConstantRelaxationConvergenceAccelerator(configuration)
+
+    elif(convergence_accelerator_type == "Relaxation"):
+        return KratosFSI.AitkenConvergenceAccelerator(configuration)
+
+    elif(convergence_accelerator_type == "MVQN"):
+        return KratosFSI.MVQNFullJacobianConvergenceAccelerator(configuration)
+
+    elif(convergence_accelerator_type == "MVQN_randomized_SVD"):
+        if not have_linear_solvers:
+            err_msg = "MVQN with randomized SVD Jacobian requires the \'LinearSolversApplication\'."
+            raise Exception(err_msg)
+        bdc_svd = KratosLinearSolvers.EigenDenseBDCSVD()
+        col_piv_qr = KratosLinearSolvers.EigenDenseColumnPivotingHouseholderQRDecomposition()
+        return KratosFSI.MVQNRandomizedSVDConvergenceAccelerator(col_piv_qr, bdc_svd, configuration)
+
+    elif(convergence_accelerator_type == "MVQN_recursive"):
+        return KratosFSI.MVQNRecursiveJacobianConvergenceAccelerator(configuration)
+
+    elif(convergence_accelerator_type == "IBQN_MVQN"):
+        return KratosFSI.IBQNMVQNConvergenceAccelerator(configuration)
+
+    elif(convergence_accelerator_type == "IBQN_MVQN_randomized_SVD"):
+        if not have_linear_solvers:
+            err_msg = "MVQN with randomized SVD Jacobian requires the \'LinearSolversApplication\'."
+            raise Exception(err_msg)
+        bdc_svd = KratosLinearSolvers.EigenDenseBDCSVD()
+        col_piv_qr = KratosLinearSolvers.EigenDenseColumnPivotingHouseholderQRDecomposition()
+        return KratosFSI.IBQNMVQNRandomizedSVDConvergenceAccelerator(col_piv_qr, bdc_svd, configuration)
+
+    else:
+        raise Exception("Convergence accelerator not found. Asking for : " + convergence_accelerator_type)
+
+    return convergence_accelerator
+
+def CreateTrilinosConvergenceAccelerator(interface_model_part, epetra_communicator, configuration):
+
+    if (type(interface_model_part) != KratosMultiphysics.ModelPart):
+        raise Exception("First input in Trilinos convergence accelerator factory is expceted to be provided as a Kratos ModelPart object.")
+
+    if(type(configuration) != KratosMultiphysics.Parameters):
+        raise Exception("Third input in Trilinos convergence accelerator factory is expected to be provided as a Kratos Parameters object.")
+
+    convergence_accelerator_type = configuration["solver_type"].GetString()
+
+    if(convergence_accelerator_type == "Relaxation"):
+        return KratosTrilinos.TrilinosAitkenConvergenceAccelerator(configuration)
+
+    elif(convergence_accelerator_type == "MVQN_recursive"):
+        return KratosTrilinos.TrilinosMVQNRecursiveJacobianConvergenceAccelerator(interface_model_part, epetra_communicator, configuration)
+
+    else:
+        raise Exception("Trilinos convergence accelerator not found. Asking for : " + convergence_accelerator_type)
+
+    return convergence_accelerator
```

## KratosMultiphysics/FSIApplication/fsi_analysis.py

 * *Ordering differences only*

```diff
@@ -1,195 +1,195 @@
-
-import KratosMultiphysics as Kratos
-from KratosMultiphysics.analysis_stage import AnalysisStage
-from KratosMultiphysics.FSIApplication import python_solvers_wrapper_fsi
-
-class FsiAnalysis(AnalysisStage):
-    '''Main script for FSI simulations using the FSI family of python solvers.'''
-
-    def Initialize(self):
-        '''
-        Construct and initialize all classes and tools used in the simulation loop.
-        '''
-        self._SetUpRestart()
-
-        if self.load_restart:
-            fluid_restart_utility = self._GetFluidRestartUtility()
-            structure_restart_utility = self._GetStructureRestartUtility()
-            fluid_restart_utility.LoadRestart()
-            structure_restart_utility.LoadRestart()
-        else:
-            self._GetSolver().ImportModelPart()
-            self._GetSolver().PrepareModelPart()
-            self._GetSolver().AddDofs()
-            self.fluid_main_model_part = self.model.GetModelPart(
-                self.project_parameters["solver_settings"]["fluid_solver_settings"]["model_part_name"].GetString())
-            self.structure_main_model_part = self.model.GetModelPart(
-                self.project_parameters["solver_settings"]["structure_solver_settings"]["model_part_name"].GetString())
-
-        # This should let eventual derived stages modify the model after reading.
-        self.ModifyInitialProperties()
-        self.ModifyInitialGeometry()
-
-        # Initialize the user-provided processes
-        self._AnalysisStage__CreateListOfProcesses() # Why name mangling?
-        for process in self._GetListOfProcesses():
-            process.ExecuteInitialize()
-
-        self._GetSolver().Initialize()
-        self.Check()
-
-        self.ModifyAfterSolverInitialize()
-
-        for process in self._GetListOfProcesses():
-            process.ExecuteBeforeSolutionLoop()
-
-        ## Stepping and time settings
-        self.end_time = self.project_parameters["problem_data"]["end_time"].GetDouble()
-
-        fluid_is_restarted = self.fluid_main_model_part.ProcessInfo[Kratos.IS_RESTARTED]
-        structure_is_restarted = self.structure_main_model_part.ProcessInfo[Kratos.IS_RESTARTED]
-        is_restarted = fluid_is_restarted and structure_is_restarted
-
-        if is_restarted:
-            fluid_time = self.fluid_main_model_part.ProcessInfo[Kratos.TIME]
-            structure_time = self.structure_main_model_part.ProcessInfo[Kratos.TIME]
-            if (abs(fluid_time - structure_time) > 1.0e-12):
-                err_msg = 'Fluid restarting time is:' + str(fluid_time) + '\n'
-                err_msg += 'Structure restarting time is:' + \
-                    str(structure_time) + '\n'
-                err_msg += 'Restarting time must coincide between subdomains.\n'
-                raise Exception(err_msg)
-            self.time = fluid_time
-        else:
-            self.time = self.project_parameters["problem_data"]["start_time"].GetDouble()
-
-        ## If the echo level is high enough, print the complete list of settings used to run the simulation
-        if self.echo_level > 1:
-            with open("ProjectParametersOutput.json", 'w') as parameter_output_file:
-                parameter_output_file.write(self.project_parameters.PrettyPrintJsonString())
-
-        Kratos.Logger.PrintInfo(self._GetSimulationName(), "Analysis -START-")
-
-    def InitializeSolutionStep(self):
-
-        # Since no substepping is implemented yet, structure and fluid step/time must match
-        step_fluid = self.fluid_main_model_part.ProcessInfo[Kratos.STEP]
-        step_structure = self.structure_main_model_part.ProcessInfo[Kratos.STEP]
-        if step_fluid != step_structure:
-            err_msg =  'Fluid step: '+ str(step_fluid) + '\n'
-            err_msg += 'Structure step: '+ str(step_structure) + '\n'
-            err_msg += 'No substepping has been implemented yet. Fluid and structure step must match.'
-            raise Exception(err_msg)
-
-        Kratos.Logger.PrintInfo(self._GetSimulationName(),"STEP = ", step_fluid)
-        Kratos.Logger.PrintInfo(self._GetSimulationName(),"TIME = ", self.time)
-
-        self.ApplyBoundaryConditions() #here the processes are called
-        self.ChangeMaterialProperties() #this is normally empty
-        self._GetSolver().InitializeSolutionStep()
-
-    def OutputSolutionStep(self):
-        super().OutputSolutionStep()
-
-        if self.save_restart:
-            fluid_restart_utility = self._GetFluidRestartUtility()
-            structure_restart_utility = self._GetStructureRestartUtility()
-            fluid_restart_utility.SaveRestart()
-            structure_restart_utility.SaveRestart()
-
-    def _CreateSolver(self):
-        return python_solvers_wrapper_fsi.CreateSolver(self.model, self.project_parameters)
-
-    def _GetSimulationName(self):
-        return self.project_parameters["problem_data"]["problem_name"].GetString()
-
-    def _GetOrderOfProcessesInitialization(self):
-        return ["structure_constraints_process_list",
-                "structure_contact_process_list",
-                "structure_loads_process_list",
-                "fluid_gravity",
-                "fluid_initial_conditions_process_list",
-                "fluid_boundary_conditions_process_list",
-                "fluid_auxiliar_process_list"]
-
-    def _GetOrderOfOutputProcessesInitialization(self):
-        return ["gid_output"]
-
-    def _SetUpRestart(self):
-        """Initialize self.restart_utility as a RestartUtility instance and check if we need to initialize the problem from a restart file."""
-        has_restart = self.project_parameters.Has("restart_settings")
-
-        if has_restart:
-            raise Exception("FSI restart not implemented yet.")
-        else:
-
-            self.load_restart = False
-            self.save_restart = False
-
-    def _GetFluidRestartUtility(self):
-
-        if self.__fluid_restart_utility is not None:
-            return self.__fluid_restart_utility
-        else:
-            if self.parallel_type == "OpenMP":
-                from restart_utility import RestartUtility as Restart
-            elif self.parallel_type == "MPI":
-                from KratosMultiphysics.mpi.distributed_restart_utility import DistributedRestartUtility as Restart
-            model_part_name = self.project_parameters["fluid_solver_settings"]["solver_settings"]["model_part_name"].GetString()
-            if self.model.HasModelPart(model_part_name):
-                model_part = self.model.GetModelPart(model_part_name)
-            else:
-                model_part = self.model.CreateModelPart(model_part_name)
-
-            self.__fluid_restart_utility = Restart(
-                model_part,
-                self.project_parameters["fluid_solver_settings"]["restart_settings"])
-
-    def _GetStructureRestartUtility(self):
-
-        if self.__structure_restart_utility is not None:
-            return self.__structure_restart_utility
-        else:
-            if self.parallel_type == "OpenMP":
-                from restart_utility import RestartUtility as Restart
-            elif self.parallel_type == "MPI":
-                from KratosMultiphysics.mpi.distributed_restart_utility import DistributedRestartUtility as Restart
-
-            model_part_name = self.project_parameters["structure_solver_settings"]["solver_settings"]["model_part_name"].GetString()
-            if self.model.HasModelPart(model_part_name):
-                model_part = self.model.GetModelPart(model_part_name)
-            else:
-                model_part = self.model.CreateModelPart(model_part_name)
-
-            self.__structure_restart_utility = Restart(
-                model_part,
-                self.project_parameters["structure_solver_settings"]["restart_settings"])
-
-#TODO: Remove this when the backwards compatibility period is over
-class FSIAnalysis(FsiAnalysis):
-    def __init__(self, model, project_parameters):
-        Kratos.Logger.PrintWarning("FSIAnalysis", "\'FSIAnalysis\' is deprecated. Use the \'FsiAnalysis\' one instead.")
-
-if __name__ == '__main__':
-    from sys import argv
-
-    if len(argv) > 2:
-        err_msg =  'Too many input arguments!\n'
-        err_msg += 'Use this script in the following way:\n'
-        err_msg += '- With default parameter file (assumed to be called "ProjectParameters.json"):\n'
-        err_msg += '    "python fsi_analysis.py"\n'
-        err_msg += '- With custom parameter file:\n'
-        err_msg += '    "python fsi_analysis.py <my-parameter-file>.json"\n'
-        raise Exception(err_msg)
-
-    if len(argv) == 2: # ProjectParameters is being passed from outside
-        parameter_file_name = argv[1]
-    else: # using default name
-        parameter_file_name = "ProjectParameters.json"
-
-    with open(parameter_file_name,'r') as parameter_file:
-        parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-    model = KratosMultiphysics.Model()
-    simulation = FSIAnalysis(model, parameters)
-    simulation.Run()
+
+import KratosMultiphysics as Kratos
+from KratosMultiphysics.analysis_stage import AnalysisStage
+from KratosMultiphysics.FSIApplication import python_solvers_wrapper_fsi
+
+class FsiAnalysis(AnalysisStage):
+    '''Main script for FSI simulations using the FSI family of python solvers.'''
+
+    def Initialize(self):
+        '''
+        Construct and initialize all classes and tools used in the simulation loop.
+        '''
+        self._SetUpRestart()
+
+        if self.load_restart:
+            fluid_restart_utility = self._GetFluidRestartUtility()
+            structure_restart_utility = self._GetStructureRestartUtility()
+            fluid_restart_utility.LoadRestart()
+            structure_restart_utility.LoadRestart()
+        else:
+            self._GetSolver().ImportModelPart()
+            self._GetSolver().PrepareModelPart()
+            self._GetSolver().AddDofs()
+            self.fluid_main_model_part = self.model.GetModelPart(
+                self.project_parameters["solver_settings"]["fluid_solver_settings"]["model_part_name"].GetString())
+            self.structure_main_model_part = self.model.GetModelPart(
+                self.project_parameters["solver_settings"]["structure_solver_settings"]["model_part_name"].GetString())
+
+        # This should let eventual derived stages modify the model after reading.
+        self.ModifyInitialProperties()
+        self.ModifyInitialGeometry()
+
+        # Initialize the user-provided processes
+        self._AnalysisStage__CreateListOfProcesses() # Why name mangling?
+        for process in self._GetListOfProcesses():
+            process.ExecuteInitialize()
+
+        self._GetSolver().Initialize()
+        self.Check()
+
+        self.ModifyAfterSolverInitialize()
+
+        for process in self._GetListOfProcesses():
+            process.ExecuteBeforeSolutionLoop()
+
+        ## Stepping and time settings
+        self.end_time = self.project_parameters["problem_data"]["end_time"].GetDouble()
+
+        fluid_is_restarted = self.fluid_main_model_part.ProcessInfo[Kratos.IS_RESTARTED]
+        structure_is_restarted = self.structure_main_model_part.ProcessInfo[Kratos.IS_RESTARTED]
+        is_restarted = fluid_is_restarted and structure_is_restarted
+
+        if is_restarted:
+            fluid_time = self.fluid_main_model_part.ProcessInfo[Kratos.TIME]
+            structure_time = self.structure_main_model_part.ProcessInfo[Kratos.TIME]
+            if (abs(fluid_time - structure_time) > 1.0e-12):
+                err_msg = 'Fluid restarting time is:' + str(fluid_time) + '\n'
+                err_msg += 'Structure restarting time is:' + \
+                    str(structure_time) + '\n'
+                err_msg += 'Restarting time must coincide between subdomains.\n'
+                raise Exception(err_msg)
+            self.time = fluid_time
+        else:
+            self.time = self.project_parameters["problem_data"]["start_time"].GetDouble()
+
+        ## If the echo level is high enough, print the complete list of settings used to run the simulation
+        if self.echo_level > 1:
+            with open("ProjectParametersOutput.json", 'w') as parameter_output_file:
+                parameter_output_file.write(self.project_parameters.PrettyPrintJsonString())
+
+        Kratos.Logger.PrintInfo(self._GetSimulationName(), "Analysis -START-")
+
+    def InitializeSolutionStep(self):
+
+        # Since no substepping is implemented yet, structure and fluid step/time must match
+        step_fluid = self.fluid_main_model_part.ProcessInfo[Kratos.STEP]
+        step_structure = self.structure_main_model_part.ProcessInfo[Kratos.STEP]
+        if step_fluid != step_structure:
+            err_msg =  'Fluid step: '+ str(step_fluid) + '\n'
+            err_msg += 'Structure step: '+ str(step_structure) + '\n'
+            err_msg += 'No substepping has been implemented yet. Fluid and structure step must match.'
+            raise Exception(err_msg)
+
+        Kratos.Logger.PrintInfo(self._GetSimulationName(),"STEP = ", step_fluid)
+        Kratos.Logger.PrintInfo(self._GetSimulationName(),"TIME = ", self.time)
+
+        self.ApplyBoundaryConditions() #here the processes are called
+        self.ChangeMaterialProperties() #this is normally empty
+        self._GetSolver().InitializeSolutionStep()
+
+    def OutputSolutionStep(self):
+        super().OutputSolutionStep()
+
+        if self.save_restart:
+            fluid_restart_utility = self._GetFluidRestartUtility()
+            structure_restart_utility = self._GetStructureRestartUtility()
+            fluid_restart_utility.SaveRestart()
+            structure_restart_utility.SaveRestart()
+
+    def _CreateSolver(self):
+        return python_solvers_wrapper_fsi.CreateSolver(self.model, self.project_parameters)
+
+    def _GetSimulationName(self):
+        return self.project_parameters["problem_data"]["problem_name"].GetString()
+
+    def _GetOrderOfProcessesInitialization(self):
+        return ["structure_constraints_process_list",
+                "structure_contact_process_list",
+                "structure_loads_process_list",
+                "fluid_gravity",
+                "fluid_initial_conditions_process_list",
+                "fluid_boundary_conditions_process_list",
+                "fluid_auxiliar_process_list"]
+
+    def _GetOrderOfOutputProcessesInitialization(self):
+        return ["gid_output"]
+
+    def _SetUpRestart(self):
+        """Initialize self.restart_utility as a RestartUtility instance and check if we need to initialize the problem from a restart file."""
+        has_restart = self.project_parameters.Has("restart_settings")
+
+        if has_restart:
+            raise Exception("FSI restart not implemented yet.")
+        else:
+
+            self.load_restart = False
+            self.save_restart = False
+
+    def _GetFluidRestartUtility(self):
+
+        if self.__fluid_restart_utility is not None:
+            return self.__fluid_restart_utility
+        else:
+            if self.parallel_type == "OpenMP":
+                from restart_utility import RestartUtility as Restart
+            elif self.parallel_type == "MPI":
+                from KratosMultiphysics.mpi.distributed_restart_utility import DistributedRestartUtility as Restart
+            model_part_name = self.project_parameters["fluid_solver_settings"]["solver_settings"]["model_part_name"].GetString()
+            if self.model.HasModelPart(model_part_name):
+                model_part = self.model.GetModelPart(model_part_name)
+            else:
+                model_part = self.model.CreateModelPart(model_part_name)
+
+            self.__fluid_restart_utility = Restart(
+                model_part,
+                self.project_parameters["fluid_solver_settings"]["restart_settings"])
+
+    def _GetStructureRestartUtility(self):
+
+        if self.__structure_restart_utility is not None:
+            return self.__structure_restart_utility
+        else:
+            if self.parallel_type == "OpenMP":
+                from restart_utility import RestartUtility as Restart
+            elif self.parallel_type == "MPI":
+                from KratosMultiphysics.mpi.distributed_restart_utility import DistributedRestartUtility as Restart
+
+            model_part_name = self.project_parameters["structure_solver_settings"]["solver_settings"]["model_part_name"].GetString()
+            if self.model.HasModelPart(model_part_name):
+                model_part = self.model.GetModelPart(model_part_name)
+            else:
+                model_part = self.model.CreateModelPart(model_part_name)
+
+            self.__structure_restart_utility = Restart(
+                model_part,
+                self.project_parameters["structure_solver_settings"]["restart_settings"])
+
+#TODO: Remove this when the backwards compatibility period is over
+class FSIAnalysis(FsiAnalysis):
+    def __init__(self, model, project_parameters):
+        Kratos.Logger.PrintWarning("FSIAnalysis", "\'FSIAnalysis\' is deprecated. Use the \'FsiAnalysis\' one instead.")
+
+if __name__ == '__main__':
+    from sys import argv
+
+    if len(argv) > 2:
+        err_msg =  'Too many input arguments!\n'
+        err_msg += 'Use this script in the following way:\n'
+        err_msg += '- With default parameter file (assumed to be called "ProjectParameters.json"):\n'
+        err_msg += '    "python fsi_analysis.py"\n'
+        err_msg += '- With custom parameter file:\n'
+        err_msg += '    "python fsi_analysis.py <my-parameter-file>.json"\n'
+        raise Exception(err_msg)
+
+    if len(argv) == 2: # ProjectParameters is being passed from outside
+        parameter_file_name = argv[1]
+    else: # using default name
+        parameter_file_name = "ProjectParameters.json"
+
+    with open(parameter_file_name,'r') as parameter_file:
+        parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+    model = KratosMultiphysics.Model()
+    simulation = FSIAnalysis(model, parameters)
+    simulation.Run()
```

## KratosMultiphysics/FSIApplication/fsi_coupling_interface.py

 * *Ordering differences only*

```diff
@@ -1,370 +1,370 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications
-import KratosMultiphysics.FSIApplication as KratosFSI
-if KratosMultiphysics.ParallelEnvironment.GetDefaultDataCommunicator().IsDistributed():
-    import KratosMultiphysics.TrilinosApplication as KratosTrilinos
-
-class FSICouplingInterface:
-
-    def __ValidateSettings(self, settings):
-        default_settings = KratosMultiphysics.Parameters("""
-        {
-            "model_part_name": "",
-            "parent_model_part_name": "",
-            "input_variable_list": [],
-            "output_variable_list": [],
-            "auxiliary_variable_list": []
-        }""")
-
-        settings.ValidateAndAssignDefaults(default_settings)
-
-        if settings["model_part_name"].GetString() == "":
-            raise Exception("Provided \'model_part_name\' is empty.")
-        if settings["parent_model_part_name"].GetString() == "":
-            raise Exception("Provided \'parent_model_part_name\' is empty.")
-        if settings["input_variable_list"].size() == 0:
-            raise Exception("Provided \'input_variable_list\' is empty.")
-        if settings["output_variable_list"].size() == 0:
-            raise Exception("Provided \'output_variable_list\' is empty.")
-
-        return settings
-
-    def __init__(self, model, settings, convergence_accelerator = None):
-        # Validate settings
-        settings = self.__ValidateSettings(settings)
-
-        # Set required member variables
-        self.model = model
-        self.convergence_accelerator = convergence_accelerator
-        self.model_part_name = settings["model_part_name"].GetString()
-        self.parent_model_part_name = settings["parent_model_part_name"].GetString()
-        self.input_variable_list = settings["input_variable_list"]
-        self.output_variable_list = settings["output_variable_list"]
-        self.auxiliary_variable_list = settings["auxiliary_variable_list"]
-
-        # Check the variables list sizes
-        n_input_vars = self.input_variable_list.size()
-        if n_input_vars != 1:
-            err_msg = "\'input_variable_list\' size is {0}. Expected 1.".format(n_input_vars)
-            raise Exception(err_msg)
-        n_output_vars = self.output_variable_list.size()
-        if (n_output_vars == 0) or (n_output_vars > 2):
-            err_msg = "\'output_variable_list\' size is {0}. Expected 1 or 2.".format(n_output_vars)
-            raise Exception(err_msg)
-
-        # Check and get the output variable(s) data type
-        aux_list = []
-        for variable in self.output_variable_list.values():
-            if KratosMultiphysics.KratosGlobals.Kernel.HasDoubleVariable(variable.GetString()):
-                aux_list.append(True)
-            elif KratosMultiphysics.KratosGlobals.Kernel.HasArrayVariable(variable.GetString()):
-                aux_list.append(False)
-            else:
-                aux_list.append(None)
-                break
-
-        if aux_list.count(None) != 0:
-            err_msg = "Non-expected variable type in \'output_variable_list\'. Only scalar and array variables are supported."
-            raise Exception(err_msg)
-
-        self.scalar_output = None
-        if aux_list.count(True) == n_output_vars:
-            self.scalar_output = True
-        elif aux_list.count(False) == n_output_vars:
-            self.scalar_output = False
-        else:
-            err_msg = "Scalar and array variable types are mixed in the \'output_variable_list\'."
-            raise Exception(err_msg)
-
-    def SetConvergenceAccelerator(self, convergence_accelerator):
-        """Set the provided convergence accelerator to the current FSI coupling interface
-
-        This function sets the convergence accelerator of the current FSI coupling interface
-        This auxiliary method is understood to set the convergence accelerator in those situations
-        in which its constructor requires the FSI coupling interface model part to be set (e.g. MPI)
-        """
-        self.convergence_accelerator = convergence_accelerator
-
-    def GetInterfaceModelPart(self):
-        if not hasattr(self, '_fsi_interface_model_part'):
-            self._fsi_interface_model_part = self._create_fsi_interface_model_part()
-        return self._fsi_interface_model_part
-
-    def GetFatherModelPart(self):
-        return self.model.GetModelPart(self.parent_model_part_name)
-
-    def ComputeResidualVector(self):
-        # Check that the output variable that defines the residual is unique and get it
-        if (self.output_variable_list.size() == 1):
-            output_variable_name = self.output_variable_list[0].GetString()
-            output_variable = KratosMultiphysics.KratosGlobals.GetVariable(output_variable_name)
-        else:
-            err_msg = "ComputeResidualVector() can only be performed with a unique output variable.\n"
-            err_msg += "Number of variables in \'output_variable_list\' is " + int(self.output_variable_list.size())
-            raise Exception(err_msg)
-
-        # Get the output variable from the father model part
-        # Note that these are the current non-linear iteration unrelaxed values (\tilde{u}^{k+1})
-        # These values will be used below to calculate the interface residual vector
-        self.GetValuesFromFatherModelPart(output_variable)
-
-        # Save the previously existent RELAXED_DISPLACEMENT in OLD_RELAXED_DISPLACEMENT before doing the update
-        # These values will be used below to calculate the interface residual vector (u^{k})
-        KratosMultiphysics.VariableUtils().CopyVariable(
-            self._relaxed_variable,
-            self._old_relaxed_variable,
-            self.GetInterfaceModelPart().Nodes)
-
-        # Compute the current non-linear iteration interface residual using the output variable
-        # Note that the residual is computed as r^{k+1} = \tilde{u}^{k+1} - u^{k}
-        self._output_variable_residual_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
-        self._get_partitioned_fsi_utilities().ComputeInterfaceResidualVector(
-            self.GetInterfaceModelPart(),
-            self._old_relaxed_variable,
-            output_variable,
-            self._residual_variable,
-            self._output_variable_residual_vector,
-            "nodal",
-            KratosMultiphysics.FSI_INTERFACE_RESIDUAL_NORM)
-
-        # Return the current interface residual norm
-        return self.GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.FSI_INTERFACE_RESIDUAL_NORM]
-
-    def Update(self):
-        # Set and fill the iteration value vector with the previous non-linear iteration relaxed values (u^{k})
-        iteration_value_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
-        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
-            self.GetInterfaceModelPart(),
-            self._old_relaxed_variable,
-            iteration_value_vector)
-
-        # Compute the convergence accelerator correction
-        self._get_convergence_accelerator().UpdateSolution(self._output_variable_residual_vector, iteration_value_vector)
-
-        # Apply the corrected solution to the FSI coupling interface nodes
-        self._get_partitioned_fsi_utilities().UpdateInterfaceValues(
-            self.GetInterfaceModelPart(),
-            self._relaxed_variable,
-            iteration_value_vector)
-
-    def UpdateDisplacement(self):
-        # Set and fill the iteration value vector with the previous non-linear iteration relaxed values (u^{k})
-        iteration_value_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
-        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
-            self.GetInterfaceModelPart(),
-            self._relaxed_variable,
-            iteration_value_vector)
-
-        # Check that the output variable that defines the residual is unique and get it (i.e. DISPLACEMENT)
-        if (self.output_variable_list.size() == 1):
-            output_variable_name = self.output_variable_list[0].GetString()
-            output_variable = KratosMultiphysics.KratosGlobals.GetVariable(output_variable_name)
-        else:
-            err_msg = "ComputeResidualVector() can only be performed with a unique output variable.\n"
-            err_msg += "Number of variables in \'output_variable_list\' is " + int(self.output_variable_list.size())
-            raise Exception(err_msg)
-
-        # Get the output variable from the father model part
-        # Note that these are the current non-linear iteration unrelaxed values (\tilde{u}^{k+1})
-        self.GetValuesFromFatherModelPart(output_variable)
-
-        # Set and fill the displacement value vector with the current non-linear iteration values (\tilde{u}^{k+1})
-        # Note that these are the current uncorrected displacement obtained with the previously corrected load
-        iteration_value_u_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
-        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
-            self.GetInterfaceModelPart(),
-            output_variable,
-            iteration_value_u_vector)
-
-        # Set and fill the traction value vector with the current non-linear iteration values (f^{k+1})
-        # Note that these are the values that were employed to obtain the current displacements
-        iteration_value_f_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
-        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
-            self.GetInterfaceModelPart(),
-            self._traction_relaxed_variable,
-            iteration_value_f_vector)
-
-        # Compute the convergence accelerator correction
-        self._get_convergence_accelerator().UpdateSolutionRight(
-            iteration_value_f_vector,
-            iteration_value_u_vector,
-            iteration_value_vector)
-
-        # Apply the corrected solution to the FSI coupling interface nodes
-        self._get_partitioned_fsi_utilities().UpdateInterfaceValues(
-            self.GetInterfaceModelPart(),
-            self._relaxed_variable,
-            iteration_value_vector)
-
-    def UpdateTraction(self):
-        # Set and fill the iteration value vector with the previous non-linear iteration relaxed values (f^{k})
-        iteration_value_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
-        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
-            self.GetInterfaceModelPart(),
-            self._traction_relaxed_variable,
-            iteration_value_vector)
-
-        # Set and fill the displacement value vector with the current non-linear iteration values (\tilde{f}^{k+1})
-        if self.input_variable_list.size() == 1:
-            input_variable_name = self.input_variable_list[0].GetString()
-            input_variable = KratosMultiphysics.KratosGlobals.GetVariable(input_variable_name)
-        else:
-            err_msg = "Input variable list has more than one variable. One is expected for the IBQN update."
-            raise Exception(err_msg)
-
-        iteration_value_f_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
-        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
-            self.GetInterfaceModelPart(),
-            input_variable,
-            iteration_value_f_vector)
-
-        # Set and fill the traction value vector with the current non-linear iteration values (u^{k+1})
-        # Note that these are the values that were employed to obtain the current tractions
-        iteration_value_u_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
-        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
-            self.GetInterfaceModelPart(),
-            self._relaxed_variable,
-            iteration_value_u_vector)
-
-        # Compute the convergence accelerator correction
-        self._get_convergence_accelerator().UpdateSolutionLeft(
-            iteration_value_u_vector,
-            iteration_value_f_vector,
-            iteration_value_vector)
-
-        # Apply the corrected solution to the FSI coupling interface nodes
-        self._get_partitioned_fsi_utilities().UpdateInterfaceValues(
-            self.GetInterfaceModelPart(),
-            self._traction_relaxed_variable,
-            iteration_value_vector)
-
-    def UpdatePosition(self, update_variable = KratosMultiphysics.DISPLACEMENT):
-        KratosMultiphysics.VariableUtils().UpdateCurrentPosition(
-            self.GetInterfaceModelPart().Nodes,
-            update_variable)
-
-    def GetValuesFromFatherModelPart(self, variable):
-        buffer_step = 0
-        KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
-            variable,
-            self.GetFatherModelPart(),
-            self.GetInterfaceModelPart(),
-            buffer_step)
-        #TODO: Remove as soon as the CopyModelPartNodalVar synchronizes internally
-        self.GetInterfaceModelPart().GetCommunicator().SynchronizeVariable(variable)
-
-    def TransferValuesToFatherModelPart(self, variable):
-        buffer_step = 0
-        KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
-            variable,
-            self.GetInterfaceModelPart(),
-            self.GetFatherModelPart(),
-            buffer_step)
-        #TODO: Remove as soon as the CopyModelPartNodalVar synchronizes internally
-        self.GetFatherModelPart().GetCommunicator().SynchronizeVariable(variable)
-
-    def _create_fsi_interface_model_part(self):
-        # Add the FSI coupling interface to the model
-        self._fsi_interface_model_part = self.model.CreateModelPart(self.model_part_name)
-
-        # Set required ProcessInfo data
-        domain_size = self.GetFatherModelPart().ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
-        self._fsi_interface_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE] = domain_size
-
-        # Add the required variables to the FSI coupling interface model part
-        for variable_name in self.input_variable_list.values():
-            input_variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name.GetString())
-            self._fsi_interface_model_part.AddNodalSolutionStepVariable(input_variable)
-        for variable_name in self.output_variable_list.values():
-            output_variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name.GetString())
-            self._fsi_interface_model_part.AddNodalSolutionStepVariable(output_variable)
-        for variable_name in self.auxiliary_variable_list.values():
-            auxiliary_variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name.GetString())
-            self._fsi_interface_model_part.AddNodalSolutionStepVariable(auxiliary_variable)
-
-        # Add the variables required for the residual minimization
-        if self._get_convergence_accelerator() is not None:
-            # Get the required variables
-            if self.scalar_output:
-                self._relaxed_variable = KratosMultiphysics.RELAXED_SCALAR
-                self._old_relaxed_variable = KratosMultiphysics.OLD_RELAXED_SCALAR
-                self._residual_variable = KratosMultiphysics.SCALAR_INTERFACE_RESIDUAL
-                if self._get_convergence_accelerator().IsBlockNewton():
-                    self._traction_relaxed_variable = KratosMultiphysics.RELAXED_SCALAR_TRACTION
-                    self._old_traction_relaxed_variable = KratosMultiphysics.OLD_RELAXED_SCALAR_TRACTION
-                    self._traction_residual_variable = KratosMultiphysics.SCALAR_TRACTION_INTERFACE_RESIDUAL
-            else:
-                self._relaxed_variable = KratosMultiphysics.RELAXED_DISPLACEMENT
-                self._old_relaxed_variable = KratosMultiphysics.OLD_RELAXED_DISPLACEMENT
-                self._residual_variable = KratosMultiphysics.FSI_INTERFACE_RESIDUAL
-                if self._get_convergence_accelerator().IsBlockNewton():
-                    self._traction_relaxed_variable = KratosMultiphysics.RELAXED_TRACTION
-                    self._old_traction_relaxed_variable = KratosMultiphysics.OLD_RELAXED_TRACTION
-                    self._traction_residual_variable = KratosMultiphysics.TRACTION_INTERFACE_RESIDUAL
-
-            # Add the required variables to the nodal database
-            self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._relaxed_variable)
-            self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._old_relaxed_variable)
-            self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._residual_variable)
-            if self._get_convergence_accelerator().IsBlockNewton():
-                self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._traction_relaxed_variable)
-                self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._old_traction_relaxed_variable)
-                self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._traction_residual_variable)
-
-        # If parallel, add the PARTITION_INDEX variable
-        if self.GetFatherModelPart().IsDistributed():
-            self._fsi_interface_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PARTITION_INDEX)
-
-        # Set the FSI coupling interface entities (nodes and elements)
-        self._get_partitioned_fsi_utilities().CreateCouplingSkin(
-            self.GetFatherModelPart(),
-            self._fsi_interface_model_part)
-
-        # Create the communication plan for the current coupling interface
-        # Note that we retrieve the fill communicator from the ParallelEnvironment so nothing would be done if non MPI
-        fill_communicator = KratosMultiphysics.ParallelEnvironment.CreateFillCommunicatorFromGlobalParallelism(
-            self._fsi_interface_model_part,
-            self._fsi_interface_model_part.GetCommunicator().GetDataCommunicator())
-        fill_communicator.Execute()
-
-        return self._fsi_interface_model_part
-
-    def _get_convergence_accelerator(self):
-        return self.convergence_accelerator
-
-    def _get_partitioned_fsi_utilities(self):
-        if not hasattr(self, '_partitioned_fsi_utilities'):
-            self._partitioned_fsi_utilities = self._create_partitioned_fsi_utilities()
-        return self._partitioned_fsi_utilities
-
-    def _create_partitioned_fsi_utilities(self):
-        domain_size = self.GetFatherModelPart().ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
-        if not self.GetFatherModelPart().IsDistributed():
-            if domain_size == 2:
-                if self.scalar_output:
-                    return KratosFSI.PartitionedFSIUtilitiesDouble2D()
-                else:
-                    return KratosFSI.PartitionedFSIUtilitiesArray2D()
-            elif domain_size == 3:
-                if self.scalar_output:
-                    return KratosFSI.PartitionedFSIUtilitiesDouble3D()
-                else:
-                    return KratosFSI.PartitionedFSIUtilitiesArray3D()
-            else:
-                raise Exception("Domain size expected to be 2 or 3. Got " + str(self.domain_size))
-        else:
-            self._epetra_communicator = KratosTrilinos.CreateCommunicator()
-            if domain_size == 2:
-                if self.scalar_output:
-                    return KratosTrilinos.TrilinosPartitionedFSIUtilitiesDouble2D(self._epetra_communicator)
-                else:
-                    return KratosTrilinos.TrilinosPartitionedFSIUtilitiesArray2D(self._epetra_communicator)
-            elif domain_size == 3:
-                if self.scalar_output:
-                    return KratosTrilinos.TrilinosPartitionedFSIUtilitiesDouble3D(self._epetra_communicator)
-                else:
-                    return KratosTrilinos.TrilinosPartitionedFSIUtilitiesArray3D(self._epetra_communicator)
-            else:
-                raise Exception("Domain size expected to be 2 or 3. Got " + str(self.domain_size))
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications
+import KratosMultiphysics.FSIApplication as KratosFSI
+if KratosMultiphysics.ParallelEnvironment.GetDefaultDataCommunicator().IsDistributed():
+    import KratosMultiphysics.TrilinosApplication as KratosTrilinos
+
+class FSICouplingInterface:
+
+    def __ValidateSettings(self, settings):
+        default_settings = KratosMultiphysics.Parameters("""
+        {
+            "model_part_name": "",
+            "parent_model_part_name": "",
+            "input_variable_list": [],
+            "output_variable_list": [],
+            "auxiliary_variable_list": []
+        }""")
+
+        settings.ValidateAndAssignDefaults(default_settings)
+
+        if settings["model_part_name"].GetString() == "":
+            raise Exception("Provided \'model_part_name\' is empty.")
+        if settings["parent_model_part_name"].GetString() == "":
+            raise Exception("Provided \'parent_model_part_name\' is empty.")
+        if settings["input_variable_list"].size() == 0:
+            raise Exception("Provided \'input_variable_list\' is empty.")
+        if settings["output_variable_list"].size() == 0:
+            raise Exception("Provided \'output_variable_list\' is empty.")
+
+        return settings
+
+    def __init__(self, model, settings, convergence_accelerator = None):
+        # Validate settings
+        settings = self.__ValidateSettings(settings)
+
+        # Set required member variables
+        self.model = model
+        self.convergence_accelerator = convergence_accelerator
+        self.model_part_name = settings["model_part_name"].GetString()
+        self.parent_model_part_name = settings["parent_model_part_name"].GetString()
+        self.input_variable_list = settings["input_variable_list"]
+        self.output_variable_list = settings["output_variable_list"]
+        self.auxiliary_variable_list = settings["auxiliary_variable_list"]
+
+        # Check the variables list sizes
+        n_input_vars = self.input_variable_list.size()
+        if n_input_vars != 1:
+            err_msg = "\'input_variable_list\' size is {0}. Expected 1.".format(n_input_vars)
+            raise Exception(err_msg)
+        n_output_vars = self.output_variable_list.size()
+        if (n_output_vars == 0) or (n_output_vars > 2):
+            err_msg = "\'output_variable_list\' size is {0}. Expected 1 or 2.".format(n_output_vars)
+            raise Exception(err_msg)
+
+        # Check and get the output variable(s) data type
+        aux_list = []
+        for variable in self.output_variable_list.values():
+            if KratosMultiphysics.KratosGlobals.Kernel.HasDoubleVariable(variable.GetString()):
+                aux_list.append(True)
+            elif KratosMultiphysics.KratosGlobals.Kernel.HasArrayVariable(variable.GetString()):
+                aux_list.append(False)
+            else:
+                aux_list.append(None)
+                break
+
+        if aux_list.count(None) != 0:
+            err_msg = "Non-expected variable type in \'output_variable_list\'. Only scalar and array variables are supported."
+            raise Exception(err_msg)
+
+        self.scalar_output = None
+        if aux_list.count(True) == n_output_vars:
+            self.scalar_output = True
+        elif aux_list.count(False) == n_output_vars:
+            self.scalar_output = False
+        else:
+            err_msg = "Scalar and array variable types are mixed in the \'output_variable_list\'."
+            raise Exception(err_msg)
+
+    def SetConvergenceAccelerator(self, convergence_accelerator):
+        """Set the provided convergence accelerator to the current FSI coupling interface
+
+        This function sets the convergence accelerator of the current FSI coupling interface
+        This auxiliary method is understood to set the convergence accelerator in those situations
+        in which its constructor requires the FSI coupling interface model part to be set (e.g. MPI)
+        """
+        self.convergence_accelerator = convergence_accelerator
+
+    def GetInterfaceModelPart(self):
+        if not hasattr(self, '_fsi_interface_model_part'):
+            self._fsi_interface_model_part = self._create_fsi_interface_model_part()
+        return self._fsi_interface_model_part
+
+    def GetFatherModelPart(self):
+        return self.model.GetModelPart(self.parent_model_part_name)
+
+    def ComputeResidualVector(self):
+        # Check that the output variable that defines the residual is unique and get it
+        if (self.output_variable_list.size() == 1):
+            output_variable_name = self.output_variable_list[0].GetString()
+            output_variable = KratosMultiphysics.KratosGlobals.GetVariable(output_variable_name)
+        else:
+            err_msg = "ComputeResidualVector() can only be performed with a unique output variable.\n"
+            err_msg += "Number of variables in \'output_variable_list\' is " + int(self.output_variable_list.size())
+            raise Exception(err_msg)
+
+        # Get the output variable from the father model part
+        # Note that these are the current non-linear iteration unrelaxed values (\tilde{u}^{k+1})
+        # These values will be used below to calculate the interface residual vector
+        self.GetValuesFromFatherModelPart(output_variable)
+
+        # Save the previously existent RELAXED_DISPLACEMENT in OLD_RELAXED_DISPLACEMENT before doing the update
+        # These values will be used below to calculate the interface residual vector (u^{k})
+        KratosMultiphysics.VariableUtils().CopyVariable(
+            self._relaxed_variable,
+            self._old_relaxed_variable,
+            self.GetInterfaceModelPart().Nodes)
+
+        # Compute the current non-linear iteration interface residual using the output variable
+        # Note that the residual is computed as r^{k+1} = \tilde{u}^{k+1} - u^{k}
+        self._output_variable_residual_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
+        self._get_partitioned_fsi_utilities().ComputeInterfaceResidualVector(
+            self.GetInterfaceModelPart(),
+            self._old_relaxed_variable,
+            output_variable,
+            self._residual_variable,
+            self._output_variable_residual_vector,
+            "nodal",
+            KratosMultiphysics.FSI_INTERFACE_RESIDUAL_NORM)
+
+        # Return the current interface residual norm
+        return self.GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.FSI_INTERFACE_RESIDUAL_NORM]
+
+    def Update(self):
+        # Set and fill the iteration value vector with the previous non-linear iteration relaxed values (u^{k})
+        iteration_value_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
+        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
+            self.GetInterfaceModelPart(),
+            self._old_relaxed_variable,
+            iteration_value_vector)
+
+        # Compute the convergence accelerator correction
+        self._get_convergence_accelerator().UpdateSolution(self._output_variable_residual_vector, iteration_value_vector)
+
+        # Apply the corrected solution to the FSI coupling interface nodes
+        self._get_partitioned_fsi_utilities().UpdateInterfaceValues(
+            self.GetInterfaceModelPart(),
+            self._relaxed_variable,
+            iteration_value_vector)
+
+    def UpdateDisplacement(self):
+        # Set and fill the iteration value vector with the previous non-linear iteration relaxed values (u^{k})
+        iteration_value_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
+        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
+            self.GetInterfaceModelPart(),
+            self._relaxed_variable,
+            iteration_value_vector)
+
+        # Check that the output variable that defines the residual is unique and get it (i.e. DISPLACEMENT)
+        if (self.output_variable_list.size() == 1):
+            output_variable_name = self.output_variable_list[0].GetString()
+            output_variable = KratosMultiphysics.KratosGlobals.GetVariable(output_variable_name)
+        else:
+            err_msg = "ComputeResidualVector() can only be performed with a unique output variable.\n"
+            err_msg += "Number of variables in \'output_variable_list\' is " + int(self.output_variable_list.size())
+            raise Exception(err_msg)
+
+        # Get the output variable from the father model part
+        # Note that these are the current non-linear iteration unrelaxed values (\tilde{u}^{k+1})
+        self.GetValuesFromFatherModelPart(output_variable)
+
+        # Set and fill the displacement value vector with the current non-linear iteration values (\tilde{u}^{k+1})
+        # Note that these are the current uncorrected displacement obtained with the previously corrected load
+        iteration_value_u_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
+        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
+            self.GetInterfaceModelPart(),
+            output_variable,
+            iteration_value_u_vector)
+
+        # Set and fill the traction value vector with the current non-linear iteration values (f^{k+1})
+        # Note that these are the values that were employed to obtain the current displacements
+        iteration_value_f_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
+        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
+            self.GetInterfaceModelPart(),
+            self._traction_relaxed_variable,
+            iteration_value_f_vector)
+
+        # Compute the convergence accelerator correction
+        self._get_convergence_accelerator().UpdateSolutionRight(
+            iteration_value_f_vector,
+            iteration_value_u_vector,
+            iteration_value_vector)
+
+        # Apply the corrected solution to the FSI coupling interface nodes
+        self._get_partitioned_fsi_utilities().UpdateInterfaceValues(
+            self.GetInterfaceModelPart(),
+            self._relaxed_variable,
+            iteration_value_vector)
+
+    def UpdateTraction(self):
+        # Set and fill the iteration value vector with the previous non-linear iteration relaxed values (f^{k})
+        iteration_value_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
+        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
+            self.GetInterfaceModelPart(),
+            self._traction_relaxed_variable,
+            iteration_value_vector)
+
+        # Set and fill the displacement value vector with the current non-linear iteration values (\tilde{f}^{k+1})
+        if self.input_variable_list.size() == 1:
+            input_variable_name = self.input_variable_list[0].GetString()
+            input_variable = KratosMultiphysics.KratosGlobals.GetVariable(input_variable_name)
+        else:
+            err_msg = "Input variable list has more than one variable. One is expected for the IBQN update."
+            raise Exception(err_msg)
+
+        iteration_value_f_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
+        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
+            self.GetInterfaceModelPart(),
+            input_variable,
+            iteration_value_f_vector)
+
+        # Set and fill the traction value vector with the current non-linear iteration values (u^{k+1})
+        # Note that these are the values that were employed to obtain the current tractions
+        iteration_value_u_vector = self._get_partitioned_fsi_utilities().SetUpInterfaceVector(self.GetInterfaceModelPart())
+        self._get_partitioned_fsi_utilities().InitializeInterfaceVector(
+            self.GetInterfaceModelPart(),
+            self._relaxed_variable,
+            iteration_value_u_vector)
+
+        # Compute the convergence accelerator correction
+        self._get_convergence_accelerator().UpdateSolutionLeft(
+            iteration_value_u_vector,
+            iteration_value_f_vector,
+            iteration_value_vector)
+
+        # Apply the corrected solution to the FSI coupling interface nodes
+        self._get_partitioned_fsi_utilities().UpdateInterfaceValues(
+            self.GetInterfaceModelPart(),
+            self._traction_relaxed_variable,
+            iteration_value_vector)
+
+    def UpdatePosition(self, update_variable = KratosMultiphysics.DISPLACEMENT):
+        KratosMultiphysics.VariableUtils().UpdateCurrentPosition(
+            self.GetInterfaceModelPart().Nodes,
+            update_variable)
+
+    def GetValuesFromFatherModelPart(self, variable):
+        buffer_step = 0
+        KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
+            variable,
+            self.GetFatherModelPart(),
+            self.GetInterfaceModelPart(),
+            buffer_step)
+        #TODO: Remove as soon as the CopyModelPartNodalVar synchronizes internally
+        self.GetInterfaceModelPart().GetCommunicator().SynchronizeVariable(variable)
+
+    def TransferValuesToFatherModelPart(self, variable):
+        buffer_step = 0
+        KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
+            variable,
+            self.GetInterfaceModelPart(),
+            self.GetFatherModelPart(),
+            buffer_step)
+        #TODO: Remove as soon as the CopyModelPartNodalVar synchronizes internally
+        self.GetFatherModelPart().GetCommunicator().SynchronizeVariable(variable)
+
+    def _create_fsi_interface_model_part(self):
+        # Add the FSI coupling interface to the model
+        self._fsi_interface_model_part = self.model.CreateModelPart(self.model_part_name)
+
+        # Set required ProcessInfo data
+        domain_size = self.GetFatherModelPart().ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
+        self._fsi_interface_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE] = domain_size
+
+        # Add the required variables to the FSI coupling interface model part
+        for variable_name in self.input_variable_list.values():
+            input_variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name.GetString())
+            self._fsi_interface_model_part.AddNodalSolutionStepVariable(input_variable)
+        for variable_name in self.output_variable_list.values():
+            output_variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name.GetString())
+            self._fsi_interface_model_part.AddNodalSolutionStepVariable(output_variable)
+        for variable_name in self.auxiliary_variable_list.values():
+            auxiliary_variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name.GetString())
+            self._fsi_interface_model_part.AddNodalSolutionStepVariable(auxiliary_variable)
+
+        # Add the variables required for the residual minimization
+        if self._get_convergence_accelerator() is not None:
+            # Get the required variables
+            if self.scalar_output:
+                self._relaxed_variable = KratosMultiphysics.RELAXED_SCALAR
+                self._old_relaxed_variable = KratosMultiphysics.OLD_RELAXED_SCALAR
+                self._residual_variable = KratosMultiphysics.SCALAR_INTERFACE_RESIDUAL
+                if self._get_convergence_accelerator().IsBlockNewton():
+                    self._traction_relaxed_variable = KratosMultiphysics.RELAXED_SCALAR_TRACTION
+                    self._old_traction_relaxed_variable = KratosMultiphysics.OLD_RELAXED_SCALAR_TRACTION
+                    self._traction_residual_variable = KratosMultiphysics.SCALAR_TRACTION_INTERFACE_RESIDUAL
+            else:
+                self._relaxed_variable = KratosMultiphysics.RELAXED_DISPLACEMENT
+                self._old_relaxed_variable = KratosMultiphysics.OLD_RELAXED_DISPLACEMENT
+                self._residual_variable = KratosMultiphysics.FSI_INTERFACE_RESIDUAL
+                if self._get_convergence_accelerator().IsBlockNewton():
+                    self._traction_relaxed_variable = KratosMultiphysics.RELAXED_TRACTION
+                    self._old_traction_relaxed_variable = KratosMultiphysics.OLD_RELAXED_TRACTION
+                    self._traction_residual_variable = KratosMultiphysics.TRACTION_INTERFACE_RESIDUAL
+
+            # Add the required variables to the nodal database
+            self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._relaxed_variable)
+            self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._old_relaxed_variable)
+            self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._residual_variable)
+            if self._get_convergence_accelerator().IsBlockNewton():
+                self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._traction_relaxed_variable)
+                self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._old_traction_relaxed_variable)
+                self._fsi_interface_model_part.AddNodalSolutionStepVariable(self._traction_residual_variable)
+
+        # If parallel, add the PARTITION_INDEX variable
+        if self.GetFatherModelPart().IsDistributed():
+            self._fsi_interface_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PARTITION_INDEX)
+
+        # Set the FSI coupling interface entities (nodes and elements)
+        self._get_partitioned_fsi_utilities().CreateCouplingSkin(
+            self.GetFatherModelPart(),
+            self._fsi_interface_model_part)
+
+        # Create the communication plan for the current coupling interface
+        # Note that we retrieve the fill communicator from the ParallelEnvironment so nothing would be done if non MPI
+        fill_communicator = KratosMultiphysics.ParallelEnvironment.CreateFillCommunicatorFromGlobalParallelism(
+            self._fsi_interface_model_part,
+            self._fsi_interface_model_part.GetCommunicator().GetDataCommunicator())
+        fill_communicator.Execute()
+
+        return self._fsi_interface_model_part
+
+    def _get_convergence_accelerator(self):
+        return self.convergence_accelerator
+
+    def _get_partitioned_fsi_utilities(self):
+        if not hasattr(self, '_partitioned_fsi_utilities'):
+            self._partitioned_fsi_utilities = self._create_partitioned_fsi_utilities()
+        return self._partitioned_fsi_utilities
+
+    def _create_partitioned_fsi_utilities(self):
+        domain_size = self.GetFatherModelPart().ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
+        if not self.GetFatherModelPart().IsDistributed():
+            if domain_size == 2:
+                if self.scalar_output:
+                    return KratosFSI.PartitionedFSIUtilitiesDouble2D()
+                else:
+                    return KratosFSI.PartitionedFSIUtilitiesArray2D()
+            elif domain_size == 3:
+                if self.scalar_output:
+                    return KratosFSI.PartitionedFSIUtilitiesDouble3D()
+                else:
+                    return KratosFSI.PartitionedFSIUtilitiesArray3D()
+            else:
+                raise Exception("Domain size expected to be 2 or 3. Got " + str(self.domain_size))
+        else:
+            self._epetra_communicator = KratosTrilinos.CreateCommunicator()
+            if domain_size == 2:
+                if self.scalar_output:
+                    return KratosTrilinos.TrilinosPartitionedFSIUtilitiesDouble2D(self._epetra_communicator)
+                else:
+                    return KratosTrilinos.TrilinosPartitionedFSIUtilitiesArray2D(self._epetra_communicator)
+            elif domain_size == 3:
+                if self.scalar_output:
+                    return KratosTrilinos.TrilinosPartitionedFSIUtilitiesDouble3D(self._epetra_communicator)
+                else:
+                    return KratosTrilinos.TrilinosPartitionedFSIUtilitiesArray3D(self._epetra_communicator)
+            else:
+                raise Exception("Domain size expected to be 2 or 3. Got " + str(self.domain_size))
```

## KratosMultiphysics/FSIApplication/partitioned_embedded_fsi_base_solver.py

 * *Ordering differences only*

```diff
@@ -1,524 +1,524 @@
-from math import sqrt   # Import the square root from python library
-
-# Import utilities
-from KratosMultiphysics.FluidDynamicsApplication import python_solvers_wrapper_fluid            # Import the fluid Python solvers wrapper
-from KratosMultiphysics.StructuralMechanicsApplication import python_solvers_wrapper_structural # Import the structure Python solvers wrapper
-from KratosMultiphysics.FSIApplication import fsi_coupling_interface                            # Import the FSI coupling interface utility
-from KratosMultiphysics.FSIApplication import convergence_accelerator_factory                   # Import the FSI convergence accelerator factory
-
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications
-import KratosMultiphysics.FSIApplication as KratosFSI
-import KratosMultiphysics.MappingApplication as KratosMapping
-import KratosMultiphysics.FluidDynamicsApplication as KratosFluid
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-
-# Import base class
-from KratosMultiphysics.FSIApplication.partitioned_fsi_base_solver import PartitionedFSIBaseSolver
-
-def CreateSolver(model, project_parameters):
-    return PartitionedEmbeddedFSIBaseSolver(model, project_parameters)
-
-class PartitionedEmbeddedFSIBaseSolver(PartitionedFSIBaseSolver):
-
-    def __init__(self, model, project_parameters):
-        # Call the base solver constructor
-        super().__init__(model, project_parameters)
-
-        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Partitioned embedded FSI base solver construction finished')
-
-    @classmethod
-    def GetDefaultParameters(cls):
-
-        # Note that only the coupling settings are validated
-        # The subdomain solver settings will be validated while instantiating these
-        default_settings = KratosMultiphysics.Parameters("""
-        {
-            "echo_level": 0,
-            "parallel_type": "OpenMP",
-            "solver_type": "partitioned_embedded",
-            "coupling_scheme": "dirichlet_neumann",
-            "structure_solver_settings": {
-            },
-            "fluid_solver_settings":{
-            },
-            "coupling_settings":{
-                "coupling_strategy_settings": {
-                    "abs_cut_off_tol": 1e-06,
-                    "solver_type": "MVQN",
-                    "w_0": 0.5
-                },
-                "nl_max_it": 30,
-                "nl_tol": 1e-07,
-                "structure_interfaces_list": []
-            }
-        }""")
-
-        default_settings.AddMissingParameters(super().GetDefaultParameters())
-        return default_settings
-
-    #TODO: Use the base solver one once we use the fluid ALE solver
-    def AddVariables(self):
-        # Fluid and structure solvers variables addition
-        self.fluid_solver.AddVariables()
-        self.structure_solver.AddVariables()
-
-    #TODO: Use the base solver one once we use the fluid ALE solver
-    def ImportModelPart(self):
-        # Fluid and structure solvers ImportModelPart() call
-        self.fluid_solver.ImportModelPart()
-        self.structure_solver.ImportModelPart()
-
-    #TODO: Use the base solver one once we use the fluid ALE solver
-    def PrepareModelPart(self):
-        # Fluid and structure solvers PrepareModelPart() call
-        self.fluid_solver.PrepareModelPart()
-        self.structure_solver.PrepareModelPart()
-
-        # Perform all the operations required to set up the coupling interfaces
-        self._InitializeCouplingInterfaces()
-
-    #TODO: Use the base solver one once we use the fluid ALE solver
-    def AddDofs(self):
-        # Add DOFs structure
-        self.structure_solver.AddDofs()
-        # Add DOFs fluid
-        self.fluid_solver.AddDofs()
-
-    def Initialize(self):
-        # Coupling utility initialization
-        # The _GetConvergenceAccelerator is supposed to construct the convergence accelerator in here
-        self._GetConvergenceAccelerator().Initialize()
-
-        # Python structure solver initialization
-        self.structure_solver.Initialize()
-
-        # Python fluid solver initialization
-        self.fluid_solver.Initialize()
-
-        # Compute the fluid domain NODAL_AREA values
-        # Required by the parallel distance calculator if the distance has to be extended
-        if (self.level_set_type == "continuous"):
-            KratosMultiphysics.CalculateNodalAreaProcess(self.GetFluidComputingModelPart(), self._GetDomainSize()).Execute()
-
-        # Initialize the distance field
-        update_distance_process = True
-        self.__GetDistanceToSkinProcess(update_distance_process).Execute()
-        if (self.level_set_type == "continuous"):
-            self.__ExtendLevelSet()
-
-        # Initialize the embedded skin utility
-        self.__GetEmbeddedSkinUtility()
-
-        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', "Finished initialization.")
-
-    #TODO: Use the base one once the body fitted uses the fluid ALE solver
-    def InitializeSolutionStep(self):
-        # Initialize solution step of fluid, structure and coupling solvers
-        self.fluid_solver.InitializeSolutionStep()
-        self.structure_solver.InitializeSolutionStep()
-        self._GetConvergenceAccelerator().InitializeSolutionStep()
-
-    def Predict(self):
-        # Structure solver prediction. It is important to firstly perform the structure
-        # prediction to update the current buffer position before the FM-ALE operations.
-        # Otherwise position 0 and 1 of the buffer coincide since the advance in time
-        # has been already performed but no update has been done yet. Besides, this will
-        # give a better approximation of the level-set position at the end of step.
-        self.structure_solver.Predict()
-
-        # Update the level set position with the structure prediction
-        self.__UpdateLevelSet()
-
-        # Fluid solver prediction
-        self.fluid_solver.Predict()
-
-    #TODO: Use the base solver one once we use the fluid ALE solver for the fluid
-    def FinalizeSolutionStep(self):
-        # Finalize solution step
-        self.fluid_solver.FinalizeSolutionStep()
-        self.structure_solver.FinalizeSolutionStep()
-        self._GetConvergenceAccelerator().FinalizeSolutionStep()
-
-    #TODO: Use the base solver one once we use the fluid ALE solver for the fluid
-    def Finalize(self):
-        self.fluid_solver.Finalize()
-        self.structure_solver.Finalize()
-        self._GetConvergenceAccelerator().Finalize()
-
-    #######################################################################
-    ##############          PRIVATE METHODS SECTION          ##############
-    #######################################################################
-
-    def _AuxiliaryInitOperations(self):
-        # Auxiliar variables
-        self.parallel_type = self.settings["parallel_type"].GetString()
-        coupling_settings = self.settings["coupling_settings"]
-        self.max_nl_it = coupling_settings["nl_max_it"].GetInt()
-        self.nl_tol = coupling_settings["nl_tol"].GetDouble()
-        self.structure_interface_submodelpart_name = coupling_settings["structure_interfaces_list"][0].GetString()
-
-        # Construct the structure solver
-        self.structure_solver = python_solvers_wrapper_structural.CreateSolverByParameters(self.model, self.settings["structure_solver_settings"], self.parallel_type)
-        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Structure solver construction finished')
-
-        # Construct the fluid solver
-        self.fluid_solver = python_solvers_wrapper_fluid.CreateSolverByParameters(self.model, self.settings["fluid_solver_settings"], self.parallel_type)
-        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Fluid solver construction finished')
-        self.level_set_type = self.settings["fluid_solver_settings"]["formulation"]["level_set_type"].GetString()
-
-        # First call to create the embedded intersections model part
-        self.__GetEmbedddedSkinUtilityModelPart()
-
-    def _AdvanceInTimeCouplingInterfaces(self, new_time):
-        # Even though these are auxiliary model parts, this is mandatory to be done to properly set up the database
-        # Note that if this operations are removed, some auxiliary utils (e.g. FM-ALE algorithm in embedded) will perform wrong
-        self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart().GetRootModelPart().CloneTimeStep(new_time)
-        self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.STEP] = self._GetFSICouplingInterfaceFluid().GetFatherModelPart().ProcessInfo[KratosMultiphysics.STEP]
-        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart().GetRootModelPart().CloneTimeStep(new_time)
-        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.STEP] = self._GetFSICouplingInterfaceStructure().GetFatherModelPart().ProcessInfo[KratosMultiphysics.STEP]
-
-    def _InitializeCouplingInterfaces(self):
-        # FSI interface coupling interfaces initialization
-        # The getter methods are to construct the FSI coupling structure interface in here
-        self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart()
-        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart()
-
-        # Set the INTERFACE flag to the structure skin
-        KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self._GetStructureInterfaceSubmodelPart().Nodes)
-
-    def __GetDistanceToSkinProcess(self, update_distance_process = False):
-        if update_distance_process:
-            self._distance_to_skin_process = self.__CreateDistanceToSkinProcess()
-        return self._distance_to_skin_process
-
-    def __CreateDistanceToSkinProcess(self):
-        # Set the distance computation process
-        if (self.level_set_type == "continuous"):
-            raycasting_relative_tolerance = 1.0e-10
-            if self._GetDomainSize() == 2:
-                return KratosMultiphysics.CalculateDistanceToSkinProcess2D(
-                    self.GetFluidComputingModelPart(),
-                    self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
-                    raycasting_relative_tolerance)
-            elif self._GetDomainSize() == 3:
-                return KratosMultiphysics.CalculateDistanceToSkinProcess3D(
-                    self.GetFluidComputingModelPart(),
-                    self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
-                    raycasting_relative_tolerance)
-            else:
-                raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
-        elif (self.level_set_type == "discontinuous"):
-            discontinuous_distance_settings = KratosMultiphysics.Parameters("""{
-                "calculate_elemental_edge_distances" : true,
-                "calculate_elemental_edge_distances_extrapolated" : true
-            }""")
-            if self._GetDomainSize() == 2:
-                return KratosMultiphysics.CalculateDiscontinuousDistanceToSkinProcess2D(
-                    self.GetFluidComputingModelPart(),
-                    self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
-                    discontinuous_distance_settings)
-            elif self._GetDomainSize() == 3:
-                return KratosMultiphysics.CalculateDiscontinuousDistanceToSkinProcess3D(
-                    self.GetFluidComputingModelPart(),
-                    self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
-                    discontinuous_distance_settings)
-            else:
-                raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
-        else:
-            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
-            raise Exception(err_msg)
-
-    def __GetParallelDistanceCalculator(self):
-        if not hasattr(self, '_parallel_distance_calculator'):
-            self._parallel_distance_calculator = self.__CreateParallelDistanceCalculator()
-        return self._parallel_distance_calculator
-
-    def __CreateParallelDistanceCalculator(self):
-        parallel_redistance_settings = KratosMultiphysics.Parameters("""{
-            "max_levels" : 2,
-            "max_distance": 1e12
-        }""")
-        if self._GetDomainSize() == 2:
-            return KratosMultiphysics.ParallelDistanceCalculationProcess2D(
-                self.GetFluidComputingModelPart(),
-                parallel_redistance_settings)
-        elif self._GetDomainSize() == 3:
-            return KratosMultiphysics.ParallelDistanceCalculationProcess3D(
-                self.GetFluidComputingModelPart(),
-                parallel_redistance_settings)
-        else:
-            raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
-
-    def __GetEmbeddedSkinUtility(self):
-        if not hasattr(self, '_embedded_skin_utility'):
-            self._embedded_skin_utility = self.__CreateEmbeddedSkinUtility()
-        return self._embedded_skin_utility
-
-    def __CreateEmbeddedSkinUtility(self):
-        if self._GetDomainSize() == 2:
-            return KratosMultiphysics.EmbeddedSkinUtility2D(
-                self.GetFluidComputingModelPart(),
-                self.__GetEmbedddedSkinUtilityModelPart(),
-                self.level_set_type)
-        elif self._GetDomainSize() == 3:
-            return KratosMultiphysics.EmbeddedSkinUtility3D(
-                self.GetFluidComputingModelPart(),
-                self.__GetEmbedddedSkinUtilityModelPart(),
-                self.level_set_type)
-        else:
-            raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
-
-    def __GetEmbedddedSkinUtilityModelPart(self):
-        if not hasattr(self, '_embedded_skin_utility_model_part'):
-            self._embedded_skin_utility_model_part = self.__CreateEmbeddedSkinUtilityModelPart()
-        return self._embedded_skin_utility_model_part
-
-    def __CreateEmbeddedSkinUtilityModelPart(self):
-        embedded_skin_utility_skin_model_part_name = "EmbeddedSkinUtilityModelPart"
-        embedded_skin_utility_skin_model_part =self.model.CreateModelPart(embedded_skin_utility_skin_model_part_name)
-        embedded_skin_utility_skin_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NORMAL)
-        if (self.level_set_type == "continuous"):
-            embedded_skin_utility_skin_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PRESSURE)
-        elif (self.level_set_type == "discontinuous"):
-            embedded_skin_utility_skin_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_FACE_PRESSURE)
-            embedded_skin_utility_skin_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NEGATIVE_FACE_PRESSURE)
-        else:
-            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
-            raise Exception(err_msg)
-        return embedded_skin_utility_skin_model_part
-
-    def __UpdateLevelSet(self):
-        # Recompute the distance field with the obtained solution
-        self.__GetDistanceToSkinProcess().Execute()
-
-        # Extend the level set to the first layer of non-intersected elements
-        # This is required in case the distance modification process moves the level set
-        # to a non-intersected element to prevent almost empty fluid elements.
-        # Note that non-intersected elements have a large default distance value, which might
-        # alter the zero isosurface when the distance modification avoids almost empty elements.
-        if (self.level_set_type == "continuous"):
-            self.__ExtendLevelSet()
-
-    def __ExtendLevelSet(self):
-        self.__GetParallelDistanceCalculator().Execute()
-
-    def _MapStructureInterfaceDisplacement(self):
-        # Map the RELAXED_DISP from the structure FSI coupling interface to fluid FSI coupling interface
-        # Note that we take advance of the fact that the coupling interfaces coincide in the embedded case
-        # Then update the fluid FSI coupling interface position
-        KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
-            KratosMultiphysics.RELAXED_DISPLACEMENT,
-            KratosMultiphysics.DISPLACEMENT,
-            self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-            self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
-            0)
-        self._GetFSICouplingInterfaceFluid().UpdatePosition(KratosMultiphysics.DISPLACEMENT)
-
-    def _SolveFluid(self):
-        # Update the current iteration level-set position
-        self.__UpdateLevelSet()
-
-        # Solve fluid problem
-        self.fluid_solver.SolveSolutionStep() # This contains the FM-ALE operations and the level set correction
-
-    def _CalculateFluidInterfaceTraction(self):
-        if (self.level_set_type == "continuous"):
-            # Interpolate the pressure to the fluid FSI coupling interface
-            self._GetPartitionedFSIUtilities().EmbeddedPressureToPositiveFacePressureInterpolator(
-                self.GetFluidComputingModelPart(),
-                self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart())
-
-        elif (self.level_set_type == "discontinuous"):
-            # Generate the intersections skin to map from
-            self.__GetEmbeddedSkinUtility().GenerateSkin()
-
-            # Interpolate POSITIVE_FACE_PRESSURE and NEGATIVE_FACE_PRESSURE from the background mesh
-            self.__GetEmbeddedSkinUtility().InterpolateDiscontinuousMeshVariableToSkin(
-                KratosMultiphysics.PRESSURE, KratosMultiphysics.POSITIVE_FACE_PRESSURE, "positive")
-            self.__GetEmbeddedSkinUtility().InterpolateDiscontinuousMeshVariableToSkin(
-                KratosMultiphysics.PRESSURE, KratosMultiphysics.NEGATIVE_FACE_PRESSURE, "negative")
-
-        else:
-            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
-            raise Exception(err_msg)
-
-    def _MapFluidInterfaceTraction(self):
-        if (self.level_set_type == "continuous"):
-            # Map PRESSURE from fluid FSI coupling interface to structure FSI coupling interface
-            # Note that in here we take advantage of the fact that the coupling interfaces coincide in the embedded case
-            KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
-                KratosMultiphysics.POSITIVE_FACE_PRESSURE,
-                KratosMultiphysics.POSITIVE_FACE_PRESSURE,
-                self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
-                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-                0)
-
-            # Convert the pressure scalar load to a traction vector one
-            # This is required in the IBQN case as the structure and fluid interface residual sizes must match
-            if self._GetConvergenceAccelerator().IsBlockNewton():
-                swap_traction_sign = True
-                self._GetPartitionedFSIUtilities().CalculateTractionFromPressureValues(
-                    self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-                    KratosMultiphysics.POSITIVE_FACE_PRESSURE,
-                    self._GetTractionVariable(),
-                    swap_traction_sign)
-
-        elif (self.level_set_type == "discontinuous"):
-            # Map the POSITIVE_FACE_PRESSURE and NEGATIVE_FACE_PRESSURE from the auxiliary embedded skin model part,
-            # which is created from the elemental level set intersections, to the fluid FSI coupling interface
-            # Note that the mapper instance is created each time as the embedded skin mesh potentially changes at each iteration
-            mapper_params = KratosMultiphysics.Parameters("""{
-                "mapper_type": "nearest_element",
-                "echo_level" : 0
-            }""")
-            mapper = KratosMultiphysics.MapperFactory.CreateMapper(
-                self.__GetEmbedddedSkinUtilityModelPart(),
-                self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
-                mapper_params)
-            mapper.Map(KratosMultiphysics.POSITIVE_FACE_PRESSURE, KratosMultiphysics.POSITIVE_FACE_PRESSURE)
-            mapper.Map(KratosMultiphysics.NEGATIVE_FACE_PRESSURE, KratosMultiphysics.NEGATIVE_FACE_PRESSURE)
-
-            # Transfer POSITIVE_FACE_PRESSURE and NEGATIVE_FACE_PRESSURE from the fluid coupling interface to the structure one
-            # Note that in here we take advantage of the fact that the coupling interfaces coincide in the embedded case
-            KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
-                KratosMultiphysics.POSITIVE_FACE_PRESSURE,
-                self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
-                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-                0)
-            KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
-                KratosMultiphysics.NEGATIVE_FACE_PRESSURE,
-                self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
-                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-                0)
-
-            # Convert the pressure scalar load to a traction vector one
-            swap_traction_sign = True
-            self._GetPartitionedFSIUtilities().CalculateTractionFromPressureValues(
-                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-                KratosMultiphysics.POSITIVE_FACE_PRESSURE,
-                KratosMultiphysics.NEGATIVE_FACE_PRESSURE,
-                self._GetTractionVariable(),
-                swap_traction_sign)
-
-        else:
-            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
-            raise Exception(err_msg)
-
-    #TODO: Use the base solver one once the body-fitted does not require to do the traction to point load conversion
-    def _SolveStructure(self):
-        # Solve the structure problem
-        self.structure_solver.SolveSolutionStep()
-
-    def _CreateFSICouplingInterfaceStructure(self):
-        # Set auxiliary settings
-        if (self.level_set_type == "continuous"):
-            aux_settings = KratosMultiphysics.Parameters(
-            """{
-                "model_part_name": "FSICouplingInterfaceStructure",
-                "parent_model_part_name": "",
-                "input_variable_list": [],
-                "output_variable_list": ["DISPLACEMENT"],
-                "auxiliary_variable_list": ["POSITIVE_FACE_PRESSURE","NORMAL"]
-            }""")
-        elif (self.level_set_type == "discontinuous"):
-            aux_settings = KratosMultiphysics.Parameters(
-            """{
-                "model_part_name": "FSICouplingInterfaceStructure",
-                "parent_model_part_name": "",
-                "input_variable_list": [],
-                "output_variable_list": ["DISPLACEMENT"],
-                "auxiliary_variable_list": ["POSITIVE_FACE_PRESSURE","NEGATIVE_FACE_PRESSURE","NORMAL"]
-            }""")
-        else:
-            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
-            raise Exception(err_msg)
-
-        aux_settings["parent_model_part_name"].SetString(self.structure_interface_submodelpart_name)
-        aux_settings["input_variable_list"].Append(self._GetTractionVariable().Name())
-
-        # Construct the FSI coupling interface
-        fsi_coupling_interface_structure = fsi_coupling_interface.FSICouplingInterface(
-            self.model,
-            aux_settings,
-            self._GetConvergenceAccelerator())
-
-        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Structure FSI coupling interface created')
-
-        return fsi_coupling_interface_structure
-
-    def _GetFSICouplingInterfaceFluid(self):
-        if not hasattr(self, '_fsi_coupling_interface_fluid'):
-            self._fsi_coupling_interface_fluid = self.__CreateFSICouplingInterfaceFluid()
-        return self._fsi_coupling_interface_fluid
-
-    def __CreateFSICouplingInterfaceFluid(self):
-        # Set auxiliary settings
-        # Note that in the embedded case, the fluid interface is identical to the structure one
-        # This is intentionally done, since this copy will be used in the level set computation
-        if (self.level_set_type == "continuous"):
-            aux_settings = KratosMultiphysics.Parameters(
-            """{
-                "model_part_name": "FSICouplingInterfaceFluid",
-                "parent_model_part_name": "",
-                "input_variable_list": ["DISPLACEMENT"],
-                "output_variable_list": ["POSITIVE_FACE_PRESSURE"]
-            }""")
-        elif (self.level_set_type == "discontinuous"):
-            aux_settings = KratosMultiphysics.Parameters(
-            """{
-                "model_part_name": "FSICouplingInterfaceFluid",
-                "parent_model_part_name": "",
-                "input_variable_list": ["DISPLACEMENT"],
-                "output_variable_list": ["POSITIVE_FACE_PRESSURE","NEGATIVE_FACE_PRESSURE"]
-            }""")
-        else:
-            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
-            raise Exception(err_msg)
-
-        aux_settings["parent_model_part_name"].SetString(self.structure_interface_submodelpart_name)
-
-        # Construct the FSI coupling interface
-        fsi_coupling_interface_fluid = fsi_coupling_interface.FSICouplingInterface(
-            self.model,
-            aux_settings)
-
-        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Fluid FSI coupling interface created')
-
-        return fsi_coupling_interface_fluid
-
-    @classmethod
-    def _GetFSICouplingInterfaceFluidPositive(self):
-        err_msg = 'Embedded partitioned FSI solver does not implement the \'_GetFSICouplingInterfaceFluidPositive\' method.\n'
-        err_msg += 'Use \'_GetFSICouplingInterfaceFluid\' method as the fluid coupling interface is unique.'
-        raise Exception(err_msg)
-
-    @classmethod
-    def _GetFSICouplingInterfaceFluidNegative(self):
-        err_msg = 'Embedded partitioned FSI solver does not implement the \'_GetFSICouplingInterfaceFluidNegative\' method.\n'
-        err_msg += 'Use \'_GetFSICouplingInterfaceFluid\' method as the fluid coupling interface is unique.'
-        raise Exception(err_msg)
-
-    def _GetTractionVariable(self):
-        if self._GetConvergenceAccelerator().IsBlockNewton():
-            if self._GetDomainSize() == 2:
-                return KratosStructural.LINE_LOAD
-            elif self._GetDomainSize() == 3:
-                return KratosStructural.SURFACE_LOAD
-            else:
-                raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
-        else:
-            if self.level_set_type == "continuous":
-                return KratosMultiphysics.POSITIVE_FACE_PRESSURE
-            elif self.level_set_type == "discontinuous":
-                if self._GetDomainSize() == 2:
-                    return KratosStructural.LINE_LOAD
-                elif self._GetDomainSize() == 3:
-                    return KratosStructural.SURFACE_LOAD
-                else:
-                    raise Exception(
-                        "Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
-            else:
-                raise Exception("Wrong level set type '{}'".format(self.level_set_type))
+from math import sqrt   # Import the square root from python library
+
+# Import utilities
+from KratosMultiphysics.FluidDynamicsApplication import python_solvers_wrapper_fluid            # Import the fluid Python solvers wrapper
+from KratosMultiphysics.StructuralMechanicsApplication import python_solvers_wrapper_structural # Import the structure Python solvers wrapper
+from KratosMultiphysics.FSIApplication import fsi_coupling_interface                            # Import the FSI coupling interface utility
+from KratosMultiphysics.FSIApplication import convergence_accelerator_factory                   # Import the FSI convergence accelerator factory
+
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications
+import KratosMultiphysics.FSIApplication as KratosFSI
+import KratosMultiphysics.MappingApplication as KratosMapping
+import KratosMultiphysics.FluidDynamicsApplication as KratosFluid
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+
+# Import base class
+from KratosMultiphysics.FSIApplication.partitioned_fsi_base_solver import PartitionedFSIBaseSolver
+
+def CreateSolver(model, project_parameters):
+    return PartitionedEmbeddedFSIBaseSolver(model, project_parameters)
+
+class PartitionedEmbeddedFSIBaseSolver(PartitionedFSIBaseSolver):
+
+    def __init__(self, model, project_parameters):
+        # Call the base solver constructor
+        super().__init__(model, project_parameters)
+
+        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Partitioned embedded FSI base solver construction finished')
+
+    @classmethod
+    def GetDefaultParameters(cls):
+
+        # Note that only the coupling settings are validated
+        # The subdomain solver settings will be validated while instantiating these
+        default_settings = KratosMultiphysics.Parameters("""
+        {
+            "echo_level": 0,
+            "parallel_type": "OpenMP",
+            "solver_type": "partitioned_embedded",
+            "coupling_scheme": "dirichlet_neumann",
+            "structure_solver_settings": {
+            },
+            "fluid_solver_settings":{
+            },
+            "coupling_settings":{
+                "coupling_strategy_settings": {
+                    "abs_cut_off_tol": 1e-06,
+                    "solver_type": "MVQN",
+                    "w_0": 0.5
+                },
+                "nl_max_it": 30,
+                "nl_tol": 1e-07,
+                "structure_interfaces_list": []
+            }
+        }""")
+
+        default_settings.AddMissingParameters(super().GetDefaultParameters())
+        return default_settings
+
+    #TODO: Use the base solver one once we use the fluid ALE solver
+    def AddVariables(self):
+        # Fluid and structure solvers variables addition
+        self.fluid_solver.AddVariables()
+        self.structure_solver.AddVariables()
+
+    #TODO: Use the base solver one once we use the fluid ALE solver
+    def ImportModelPart(self):
+        # Fluid and structure solvers ImportModelPart() call
+        self.fluid_solver.ImportModelPart()
+        self.structure_solver.ImportModelPart()
+
+    #TODO: Use the base solver one once we use the fluid ALE solver
+    def PrepareModelPart(self):
+        # Fluid and structure solvers PrepareModelPart() call
+        self.fluid_solver.PrepareModelPart()
+        self.structure_solver.PrepareModelPart()
+
+        # Perform all the operations required to set up the coupling interfaces
+        self._InitializeCouplingInterfaces()
+
+    #TODO: Use the base solver one once we use the fluid ALE solver
+    def AddDofs(self):
+        # Add DOFs structure
+        self.structure_solver.AddDofs()
+        # Add DOFs fluid
+        self.fluid_solver.AddDofs()
+
+    def Initialize(self):
+        # Coupling utility initialization
+        # The _GetConvergenceAccelerator is supposed to construct the convergence accelerator in here
+        self._GetConvergenceAccelerator().Initialize()
+
+        # Python structure solver initialization
+        self.structure_solver.Initialize()
+
+        # Python fluid solver initialization
+        self.fluid_solver.Initialize()
+
+        # Compute the fluid domain NODAL_AREA values
+        # Required by the parallel distance calculator if the distance has to be extended
+        if (self.level_set_type == "continuous"):
+            KratosMultiphysics.CalculateNodalAreaProcess(self.GetFluidComputingModelPart(), self._GetDomainSize()).Execute()
+
+        # Initialize the distance field
+        update_distance_process = True
+        self.__GetDistanceToSkinProcess(update_distance_process).Execute()
+        if (self.level_set_type == "continuous"):
+            self.__ExtendLevelSet()
+
+        # Initialize the embedded skin utility
+        self.__GetEmbeddedSkinUtility()
+
+        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', "Finished initialization.")
+
+    #TODO: Use the base one once the body fitted uses the fluid ALE solver
+    def InitializeSolutionStep(self):
+        # Initialize solution step of fluid, structure and coupling solvers
+        self.fluid_solver.InitializeSolutionStep()
+        self.structure_solver.InitializeSolutionStep()
+        self._GetConvergenceAccelerator().InitializeSolutionStep()
+
+    def Predict(self):
+        # Structure solver prediction. It is important to firstly perform the structure
+        # prediction to update the current buffer position before the FM-ALE operations.
+        # Otherwise position 0 and 1 of the buffer coincide since the advance in time
+        # has been already performed but no update has been done yet. Besides, this will
+        # give a better approximation of the level-set position at the end of step.
+        self.structure_solver.Predict()
+
+        # Update the level set position with the structure prediction
+        self.__UpdateLevelSet()
+
+        # Fluid solver prediction
+        self.fluid_solver.Predict()
+
+    #TODO: Use the base solver one once we use the fluid ALE solver for the fluid
+    def FinalizeSolutionStep(self):
+        # Finalize solution step
+        self.fluid_solver.FinalizeSolutionStep()
+        self.structure_solver.FinalizeSolutionStep()
+        self._GetConvergenceAccelerator().FinalizeSolutionStep()
+
+    #TODO: Use the base solver one once we use the fluid ALE solver for the fluid
+    def Finalize(self):
+        self.fluid_solver.Finalize()
+        self.structure_solver.Finalize()
+        self._GetConvergenceAccelerator().Finalize()
+
+    #######################################################################
+    ##############          PRIVATE METHODS SECTION          ##############
+    #######################################################################
+
+    def _AuxiliaryInitOperations(self):
+        # Auxiliar variables
+        self.parallel_type = self.settings["parallel_type"].GetString()
+        coupling_settings = self.settings["coupling_settings"]
+        self.max_nl_it = coupling_settings["nl_max_it"].GetInt()
+        self.nl_tol = coupling_settings["nl_tol"].GetDouble()
+        self.structure_interface_submodelpart_name = coupling_settings["structure_interfaces_list"][0].GetString()
+
+        # Construct the structure solver
+        self.structure_solver = python_solvers_wrapper_structural.CreateSolverByParameters(self.model, self.settings["structure_solver_settings"], self.parallel_type)
+        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Structure solver construction finished')
+
+        # Construct the fluid solver
+        self.fluid_solver = python_solvers_wrapper_fluid.CreateSolverByParameters(self.model, self.settings["fluid_solver_settings"], self.parallel_type)
+        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Fluid solver construction finished')
+        self.level_set_type = self.settings["fluid_solver_settings"]["formulation"]["level_set_type"].GetString()
+
+        # First call to create the embedded intersections model part
+        self.__GetEmbedddedSkinUtilityModelPart()
+
+    def _AdvanceInTimeCouplingInterfaces(self, new_time):
+        # Even though these are auxiliary model parts, this is mandatory to be done to properly set up the database
+        # Note that if this operations are removed, some auxiliary utils (e.g. FM-ALE algorithm in embedded) will perform wrong
+        self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart().GetRootModelPart().CloneTimeStep(new_time)
+        self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.STEP] = self._GetFSICouplingInterfaceFluid().GetFatherModelPart().ProcessInfo[KratosMultiphysics.STEP]
+        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart().GetRootModelPart().CloneTimeStep(new_time)
+        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.STEP] = self._GetFSICouplingInterfaceStructure().GetFatherModelPart().ProcessInfo[KratosMultiphysics.STEP]
+
+    def _InitializeCouplingInterfaces(self):
+        # FSI interface coupling interfaces initialization
+        # The getter methods are to construct the FSI coupling structure interface in here
+        self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart()
+        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart()
+
+        # Set the INTERFACE flag to the structure skin
+        KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self._GetStructureInterfaceSubmodelPart().Nodes)
+
+    def __GetDistanceToSkinProcess(self, update_distance_process = False):
+        if update_distance_process:
+            self._distance_to_skin_process = self.__CreateDistanceToSkinProcess()
+        return self._distance_to_skin_process
+
+    def __CreateDistanceToSkinProcess(self):
+        # Set the distance computation process
+        if (self.level_set_type == "continuous"):
+            raycasting_relative_tolerance = 1.0e-10
+            if self._GetDomainSize() == 2:
+                return KratosMultiphysics.CalculateDistanceToSkinProcess2D(
+                    self.GetFluidComputingModelPart(),
+                    self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
+                    raycasting_relative_tolerance)
+            elif self._GetDomainSize() == 3:
+                return KratosMultiphysics.CalculateDistanceToSkinProcess3D(
+                    self.GetFluidComputingModelPart(),
+                    self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
+                    raycasting_relative_tolerance)
+            else:
+                raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
+        elif (self.level_set_type == "discontinuous"):
+            discontinuous_distance_settings = KratosMultiphysics.Parameters("""{
+                "calculate_elemental_edge_distances" : true,
+                "calculate_elemental_edge_distances_extrapolated" : true
+            }""")
+            if self._GetDomainSize() == 2:
+                return KratosMultiphysics.CalculateDiscontinuousDistanceToSkinProcess2D(
+                    self.GetFluidComputingModelPart(),
+                    self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
+                    discontinuous_distance_settings)
+            elif self._GetDomainSize() == 3:
+                return KratosMultiphysics.CalculateDiscontinuousDistanceToSkinProcess3D(
+                    self.GetFluidComputingModelPart(),
+                    self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
+                    discontinuous_distance_settings)
+            else:
+                raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
+        else:
+            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
+            raise Exception(err_msg)
+
+    def __GetParallelDistanceCalculator(self):
+        if not hasattr(self, '_parallel_distance_calculator'):
+            self._parallel_distance_calculator = self.__CreateParallelDistanceCalculator()
+        return self._parallel_distance_calculator
+
+    def __CreateParallelDistanceCalculator(self):
+        parallel_redistance_settings = KratosMultiphysics.Parameters("""{
+            "max_levels" : 2,
+            "max_distance": 1e12
+        }""")
+        if self._GetDomainSize() == 2:
+            return KratosMultiphysics.ParallelDistanceCalculationProcess2D(
+                self.GetFluidComputingModelPart(),
+                parallel_redistance_settings)
+        elif self._GetDomainSize() == 3:
+            return KratosMultiphysics.ParallelDistanceCalculationProcess3D(
+                self.GetFluidComputingModelPart(),
+                parallel_redistance_settings)
+        else:
+            raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
+
+    def __GetEmbeddedSkinUtility(self):
+        if not hasattr(self, '_embedded_skin_utility'):
+            self._embedded_skin_utility = self.__CreateEmbeddedSkinUtility()
+        return self._embedded_skin_utility
+
+    def __CreateEmbeddedSkinUtility(self):
+        if self._GetDomainSize() == 2:
+            return KratosMultiphysics.EmbeddedSkinUtility2D(
+                self.GetFluidComputingModelPart(),
+                self.__GetEmbedddedSkinUtilityModelPart(),
+                self.level_set_type)
+        elif self._GetDomainSize() == 3:
+            return KratosMultiphysics.EmbeddedSkinUtility3D(
+                self.GetFluidComputingModelPart(),
+                self.__GetEmbedddedSkinUtilityModelPart(),
+                self.level_set_type)
+        else:
+            raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
+
+    def __GetEmbedddedSkinUtilityModelPart(self):
+        if not hasattr(self, '_embedded_skin_utility_model_part'):
+            self._embedded_skin_utility_model_part = self.__CreateEmbeddedSkinUtilityModelPart()
+        return self._embedded_skin_utility_model_part
+
+    def __CreateEmbeddedSkinUtilityModelPart(self):
+        embedded_skin_utility_skin_model_part_name = "EmbeddedSkinUtilityModelPart"
+        embedded_skin_utility_skin_model_part =self.model.CreateModelPart(embedded_skin_utility_skin_model_part_name)
+        embedded_skin_utility_skin_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NORMAL)
+        if (self.level_set_type == "continuous"):
+            embedded_skin_utility_skin_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PRESSURE)
+        elif (self.level_set_type == "discontinuous"):
+            embedded_skin_utility_skin_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_FACE_PRESSURE)
+            embedded_skin_utility_skin_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NEGATIVE_FACE_PRESSURE)
+        else:
+            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
+            raise Exception(err_msg)
+        return embedded_skin_utility_skin_model_part
+
+    def __UpdateLevelSet(self):
+        # Recompute the distance field with the obtained solution
+        self.__GetDistanceToSkinProcess().Execute()
+
+        # Extend the level set to the first layer of non-intersected elements
+        # This is required in case the distance modification process moves the level set
+        # to a non-intersected element to prevent almost empty fluid elements.
+        # Note that non-intersected elements have a large default distance value, which might
+        # alter the zero isosurface when the distance modification avoids almost empty elements.
+        if (self.level_set_type == "continuous"):
+            self.__ExtendLevelSet()
+
+    def __ExtendLevelSet(self):
+        self.__GetParallelDistanceCalculator().Execute()
+
+    def _MapStructureInterfaceDisplacement(self):
+        # Map the RELAXED_DISP from the structure FSI coupling interface to fluid FSI coupling interface
+        # Note that we take advance of the fact that the coupling interfaces coincide in the embedded case
+        # Then update the fluid FSI coupling interface position
+        KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
+            KratosMultiphysics.RELAXED_DISPLACEMENT,
+            KratosMultiphysics.DISPLACEMENT,
+            self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+            self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
+            0)
+        self._GetFSICouplingInterfaceFluid().UpdatePosition(KratosMultiphysics.DISPLACEMENT)
+
+    def _SolveFluid(self):
+        # Update the current iteration level-set position
+        self.__UpdateLevelSet()
+
+        # Solve fluid problem
+        self.fluid_solver.SolveSolutionStep() # This contains the FM-ALE operations and the level set correction
+
+    def _CalculateFluidInterfaceTraction(self):
+        if (self.level_set_type == "continuous"):
+            # Interpolate the pressure to the fluid FSI coupling interface
+            self._GetPartitionedFSIUtilities().EmbeddedPressureToPositiveFacePressureInterpolator(
+                self.GetFluidComputingModelPart(),
+                self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart())
+
+        elif (self.level_set_type == "discontinuous"):
+            # Generate the intersections skin to map from
+            self.__GetEmbeddedSkinUtility().GenerateSkin()
+
+            # Interpolate POSITIVE_FACE_PRESSURE and NEGATIVE_FACE_PRESSURE from the background mesh
+            self.__GetEmbeddedSkinUtility().InterpolateDiscontinuousMeshVariableToSkin(
+                KratosMultiphysics.PRESSURE, KratosMultiphysics.POSITIVE_FACE_PRESSURE, "positive")
+            self.__GetEmbeddedSkinUtility().InterpolateDiscontinuousMeshVariableToSkin(
+                KratosMultiphysics.PRESSURE, KratosMultiphysics.NEGATIVE_FACE_PRESSURE, "negative")
+
+        else:
+            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
+            raise Exception(err_msg)
+
+    def _MapFluidInterfaceTraction(self):
+        if (self.level_set_type == "continuous"):
+            # Map PRESSURE from fluid FSI coupling interface to structure FSI coupling interface
+            # Note that in here we take advantage of the fact that the coupling interfaces coincide in the embedded case
+            KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
+                KratosMultiphysics.POSITIVE_FACE_PRESSURE,
+                KratosMultiphysics.POSITIVE_FACE_PRESSURE,
+                self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
+                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+                0)
+
+            # Convert the pressure scalar load to a traction vector one
+            # This is required in the IBQN case as the structure and fluid interface residual sizes must match
+            if self._GetConvergenceAccelerator().IsBlockNewton():
+                swap_traction_sign = True
+                self._GetPartitionedFSIUtilities().CalculateTractionFromPressureValues(
+                    self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+                    KratosMultiphysics.POSITIVE_FACE_PRESSURE,
+                    self._GetTractionVariable(),
+                    swap_traction_sign)
+
+        elif (self.level_set_type == "discontinuous"):
+            # Map the POSITIVE_FACE_PRESSURE and NEGATIVE_FACE_PRESSURE from the auxiliary embedded skin model part,
+            # which is created from the elemental level set intersections, to the fluid FSI coupling interface
+            # Note that the mapper instance is created each time as the embedded skin mesh potentially changes at each iteration
+            mapper_params = KratosMultiphysics.Parameters("""{
+                "mapper_type": "nearest_element",
+                "echo_level" : 0
+            }""")
+            mapper = KratosMultiphysics.MapperFactory.CreateMapper(
+                self.__GetEmbedddedSkinUtilityModelPart(),
+                self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
+                mapper_params)
+            mapper.Map(KratosMultiphysics.POSITIVE_FACE_PRESSURE, KratosMultiphysics.POSITIVE_FACE_PRESSURE)
+            mapper.Map(KratosMultiphysics.NEGATIVE_FACE_PRESSURE, KratosMultiphysics.NEGATIVE_FACE_PRESSURE)
+
+            # Transfer POSITIVE_FACE_PRESSURE and NEGATIVE_FACE_PRESSURE from the fluid coupling interface to the structure one
+            # Note that in here we take advantage of the fact that the coupling interfaces coincide in the embedded case
+            KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
+                KratosMultiphysics.POSITIVE_FACE_PRESSURE,
+                self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
+                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+                0)
+            KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
+                KratosMultiphysics.NEGATIVE_FACE_PRESSURE,
+                self._GetFSICouplingInterfaceFluid().GetInterfaceModelPart(),
+                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+                0)
+
+            # Convert the pressure scalar load to a traction vector one
+            swap_traction_sign = True
+            self._GetPartitionedFSIUtilities().CalculateTractionFromPressureValues(
+                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+                KratosMultiphysics.POSITIVE_FACE_PRESSURE,
+                KratosMultiphysics.NEGATIVE_FACE_PRESSURE,
+                self._GetTractionVariable(),
+                swap_traction_sign)
+
+        else:
+            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
+            raise Exception(err_msg)
+
+    #TODO: Use the base solver one once the body-fitted does not require to do the traction to point load conversion
+    def _SolveStructure(self):
+        # Solve the structure problem
+        self.structure_solver.SolveSolutionStep()
+
+    def _CreateFSICouplingInterfaceStructure(self):
+        # Set auxiliary settings
+        if (self.level_set_type == "continuous"):
+            aux_settings = KratosMultiphysics.Parameters(
+            """{
+                "model_part_name": "FSICouplingInterfaceStructure",
+                "parent_model_part_name": "",
+                "input_variable_list": [],
+                "output_variable_list": ["DISPLACEMENT"],
+                "auxiliary_variable_list": ["POSITIVE_FACE_PRESSURE","NORMAL"]
+            }""")
+        elif (self.level_set_type == "discontinuous"):
+            aux_settings = KratosMultiphysics.Parameters(
+            """{
+                "model_part_name": "FSICouplingInterfaceStructure",
+                "parent_model_part_name": "",
+                "input_variable_list": [],
+                "output_variable_list": ["DISPLACEMENT"],
+                "auxiliary_variable_list": ["POSITIVE_FACE_PRESSURE","NEGATIVE_FACE_PRESSURE","NORMAL"]
+            }""")
+        else:
+            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
+            raise Exception(err_msg)
+
+        aux_settings["parent_model_part_name"].SetString(self.structure_interface_submodelpart_name)
+        aux_settings["input_variable_list"].Append(self._GetTractionVariable().Name())
+
+        # Construct the FSI coupling interface
+        fsi_coupling_interface_structure = fsi_coupling_interface.FSICouplingInterface(
+            self.model,
+            aux_settings,
+            self._GetConvergenceAccelerator())
+
+        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Structure FSI coupling interface created')
+
+        return fsi_coupling_interface_structure
+
+    def _GetFSICouplingInterfaceFluid(self):
+        if not hasattr(self, '_fsi_coupling_interface_fluid'):
+            self._fsi_coupling_interface_fluid = self.__CreateFSICouplingInterfaceFluid()
+        return self._fsi_coupling_interface_fluid
+
+    def __CreateFSICouplingInterfaceFluid(self):
+        # Set auxiliary settings
+        # Note that in the embedded case, the fluid interface is identical to the structure one
+        # This is intentionally done, since this copy will be used in the level set computation
+        if (self.level_set_type == "continuous"):
+            aux_settings = KratosMultiphysics.Parameters(
+            """{
+                "model_part_name": "FSICouplingInterfaceFluid",
+                "parent_model_part_name": "",
+                "input_variable_list": ["DISPLACEMENT"],
+                "output_variable_list": ["POSITIVE_FACE_PRESSURE"]
+            }""")
+        elif (self.level_set_type == "discontinuous"):
+            aux_settings = KratosMultiphysics.Parameters(
+            """{
+                "model_part_name": "FSICouplingInterfaceFluid",
+                "parent_model_part_name": "",
+                "input_variable_list": ["DISPLACEMENT"],
+                "output_variable_list": ["POSITIVE_FACE_PRESSURE","NEGATIVE_FACE_PRESSURE"]
+            }""")
+        else:
+            err_msg = 'Level set type is: \'' + self.level_set_type + '\'. Expected \'continuous\' or \'discontinuous\'.'
+            raise Exception(err_msg)
+
+        aux_settings["parent_model_part_name"].SetString(self.structure_interface_submodelpart_name)
+
+        # Construct the FSI coupling interface
+        fsi_coupling_interface_fluid = fsi_coupling_interface.FSICouplingInterface(
+            self.model,
+            aux_settings)
+
+        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Fluid FSI coupling interface created')
+
+        return fsi_coupling_interface_fluid
+
+    @classmethod
+    def _GetFSICouplingInterfaceFluidPositive(self):
+        err_msg = 'Embedded partitioned FSI solver does not implement the \'_GetFSICouplingInterfaceFluidPositive\' method.\n'
+        err_msg += 'Use \'_GetFSICouplingInterfaceFluid\' method as the fluid coupling interface is unique.'
+        raise Exception(err_msg)
+
+    @classmethod
+    def _GetFSICouplingInterfaceFluidNegative(self):
+        err_msg = 'Embedded partitioned FSI solver does not implement the \'_GetFSICouplingInterfaceFluidNegative\' method.\n'
+        err_msg += 'Use \'_GetFSICouplingInterfaceFluid\' method as the fluid coupling interface is unique.'
+        raise Exception(err_msg)
+
+    def _GetTractionVariable(self):
+        if self._GetConvergenceAccelerator().IsBlockNewton():
+            if self._GetDomainSize() == 2:
+                return KratosStructural.LINE_LOAD
+            elif self._GetDomainSize() == 3:
+                return KratosStructural.SURFACE_LOAD
+            else:
+                raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
+        else:
+            if self.level_set_type == "continuous":
+                return KratosMultiphysics.POSITIVE_FACE_PRESSURE
+            elif self.level_set_type == "discontinuous":
+                if self._GetDomainSize() == 2:
+                    return KratosStructural.LINE_LOAD
+                elif self._GetDomainSize() == 3:
+                    return KratosStructural.SURFACE_LOAD
+                else:
+                    raise Exception(
+                        "Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
+            else:
+                raise Exception("Wrong level set type '{}'".format(self.level_set_type))
```

## KratosMultiphysics/FSIApplication/partitioned_fsi_base_solver.py

 * *Ordering differences only*

```diff
@@ -1,820 +1,820 @@
-from math import sqrt   # Import the square root from python library
-
-# Import utilities
-from KratosMultiphysics.FluidDynamicsApplication import python_solvers_wrapper_fluid            # Import the fluid Python solvers wrapper
-from KratosMultiphysics.StructuralMechanicsApplication import python_solvers_wrapper_structural       # Import the structure Python solvers wrapper
-from KratosMultiphysics.MeshMovingApplication import python_solvers_wrapper_mesh_motion      # Import the mesh motion Python solvers wrapper
-from KratosMultiphysics.FSIApplication import fsi_coupling_interface                            # Import the FSI coupling interface utility
-from KratosMultiphysics.FSIApplication import convergence_accelerator_factory         # Import the FSI convergence accelerator factory
-
-# Importing the Kratos Library
-import KratosMultiphysics
-from KratosMultiphysics.python_solver import PythonSolver
-
-# Import applications
-import KratosMultiphysics.FSIApplication as KratosFSI
-import KratosMultiphysics.MappingApplication as KratosMapping
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-
-def CreateSolver(model, project_parameters):
-    return PartitionedFSIBaseSolver(model, project_parameters)
-
-class PartitionedFSIBaseSolver(PythonSolver):
-    def __init__(self, model, project_parameters):
-        # TODO: Remove this as soon as the MPCs are implemented in MPI
-        # This has to be done prior to the defaults check to avoid the structural solver to throw an error in MPI
-        if not project_parameters["structure_solver_settings"].Has("multi_point_constraints_used"):
-            project_parameters["structure_solver_settings"].AddEmptyValue("multi_point_constraints_used")
-            project_parameters["structure_solver_settings"]["multi_point_constraints_used"].SetBool(False)
-
-        # Call the base Python solver constructor
-        # Note that default settings in GetDefaultParameters() are validated in here
-        super().__init__(model, project_parameters)
-
-        # This method encapsulates all the operations required to be done in the constructor
-        # It is intended to be overwritten in the derived classes
-        self._AuxiliaryInitOperations()
-
-        KratosMultiphysics.Logger.PrintInfo("PartitionedFSIBaseSolver", "Partitioned FSI base solver construction finished.")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-
-        # Note that only the coupling settings are validated
-        # The subdomain solver settings will be validated while instantiating these
-        this_defaults = KratosMultiphysics.Parameters("""{
-            "echo_level": 0,
-            "parallel_type": "OpenMP",
-            "solver_type": "partitioned",
-            "coupling_scheme": "dirichlet_neumann",
-            "structure_solver_settings": {
-            },
-            "fluid_solver_settings":{
-            },
-            "mesh_solver_settings":{
-            },
-            "coupling_settings":{
-                "coupling_strategy_settings": {
-                    "solver_type": "MVQN",
-                    "w_0": 0.825
-                },
-                "mapper_settings": [{
-                    "fluid_interface_submodelpart_name": "",
-                    "mapper_face": "unique",
-                    "structure_interface_submodelpart_name": ""
-                }],
-                "nl_max_it": 25,
-                "nl_tol": 1e-8,
-                "solve_mesh_at_each_iteration": true,
-                "fluid_interfaces_list": [],
-                "structure_interfaces_list": []
-            }
-        }""")
-
-        this_defaults.AddMissingParameters(super().GetDefaultParameters())
-        return this_defaults
-
-    def ValidateSettings(self):
-        default_settings = self.GetDefaultParameters()
-
-        ## Base class settings validation
-        super().ValidateSettings()
-
-        ## Validate coupling settings
-        self.settings["coupling_settings"].ValidateAndAssignDefaults(default_settings["coupling_settings"])
-
-    def GetMinimumBufferSize(self):
-        # Get structure buffer size
-        buffer_structure = self.structure_solver.GetMinimumBufferSize()
-        # Get fluid buffer size
-        buffer_fluid = self.fluid_solver.GetMinimumBufferSize()
-
-        return max(buffer_structure,buffer_fluid)
-
-    def AddVariables(self):
-        ## Structure variables addition
-        # Standard CSM variables addition
-        self.structure_solver.AddVariables()
-
-        ## Fluid variables addition
-        # Standard CFD variables addition
-        self.fluid_solver.AddVariables()
-        # Mesh solver variables addition
-        self.mesh_solver.AddVariables()
-
-        ## Fluid traction variables addition
-        # These are required for the reaction variable redistribution in the fluid model part skin
-        self.fluid_solver.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_MAPPED_VECTOR_VARIABLE)
-        self.fluid_solver.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NEGATIVE_MAPPED_VECTOR_VARIABLE)
-
-    def ImportModelPart(self):
-        # Fluid and structure solvers ImportModelPart() call
-        self.fluid_solver.ImportModelPart()
-        self.structure_solver.ImportModelPart()
-        self.mesh_solver.ImportModelPart()
-
-    def PrepareModelPart(self):
-        # Fluid and structure solvers PrepareModelPart() call
-        self.structure_solver.PrepareModelPart()
-        self.fluid_solver.PrepareModelPart()
-        self.mesh_solver.PrepareModelPart()
-
-        # FSI interface coupling interfaces initialization
-        # The getter methods are to construct the FSI coupling interfaces in here
-        self._GetFSICouplingInterfaceFluidPositive().GetInterfaceModelPart()
-        if self.double_faced_structure:
-            self._GetFSICouplingInterfaceFluidNegative().GetInterfaceModelPart()
-        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart()
-
-    def AddDofs(self):
-        # Add DOFs structure
-        self.structure_solver.AddDofs()
-
-        # Add DOFs fluid
-        self.fluid_solver.AddDofs()
-        self.mesh_solver.AddDofs()
-
-    def Initialize(self):
-        # Create the required mappers
-        self._GetStructureToFluidPositiveInterfaceMapper()
-        if self.double_faced_structure:
-            self._GetStructureToFluidNegativeInterfaceMapper()
-
-        # Coupling utility initialization
-        # The _GetConvergenceAccelerator is supposed to construct the convergence accelerator in here
-        self._GetConvergenceAccelerator().Initialize()
-
-        # Python structure solver initialization
-        self.structure_solver.Initialize()
-
-        # Ensure that the fluid reaction fluxes are computed before initializing the fluid strategy
-        if self.fluid_solver.settings["compute_reactions"].GetBool() == False:
-            self.fluid_solver.settings["compute_reactions"].SetBool(True)
-
-        # Python fluid solver initialization
-        self.fluid_solver.Initialize()
-
-        # Python mesh solver initialization
-        self.mesh_solver.Initialize()
-
-        # Perform all the operations required to set up the coupling interfaces
-        self._InitializeCouplingInterfaces()
-
-    def AdvanceInTime(self, current_time):
-        # Subdomains time advance
-        fluid_new_time = self.fluid_solver.AdvanceInTime(current_time)
-        structure_new_time = self.structure_solver.AdvanceInTime(current_time)
-
-        if abs(fluid_new_time - structure_new_time) > 1e-12:
-            err_msg =  'Fluid new time is: ' + str(fluid_new_time) + '\n'
-            err_msg += 'Structure new time is: ' + str(structure_new_time) + '\n'
-            err_msg += 'No substepping has been implemented yet. Fluid and structure time must coincide.'
-            raise Exception(err_msg)
-
-        # Update the auxiliary coupling interface model parts database in case these are to be output
-        # Note that there are also situations (e.g. embedded) in which this is mandatory for the proper performance of the solver
-        self._AdvanceInTimeCouplingInterfaces(fluid_new_time)
-
-        return fluid_new_time
-
-    def InitializeSolutionStep(self):
-        # Initialize solution step of fluid, structure and coupling solvers
-        self.structure_solver.InitializeSolutionStep()
-        self.fluid_solver.InitializeSolutionStep()
-        self.mesh_solver.InitializeSolutionStep()
-        self._GetConvergenceAccelerator().InitializeSolutionStep()
-
-    def Predict(self):
-        # Perform fluid and structure solvers predictions
-        self.structure_solver.Predict()
-        self.fluid_solver.Predict()
-        self.mesh_solver.Predict()
-
-    def GetComputingModelPart(self):
-        err_msg =  'Calling GetComputingModelPart() method in a partitioned solver.\n'
-        err_msg += 'Specify the domain of interest by calling:\n'
-        err_msg += '\t- GetFluidComputingModelPart()\n'
-        err_msg += '\t- GetStructureComputingModelPart()\n'
-        raise Exception(err_msg)
-
-    def GetFluidComputingModelPart(self):
-        return self.fluid_solver.GetComputingModelPart()
-
-    def GetStructureComputingModelPart(self):
-        return self.structure_solver.GetComputingModelPart()
-
-    def GetOutputVariables(self):
-        pass
-
-    def SaveRestart(self):
-        pass
-
-    def SolveSolutionStep(self):
-        ## Initialize residual
-        dis_residual_norm = self._ComputeInitialResidual()
-
-        ## FSI nonlinear iteration loop
-        nl_it = 1
-        is_converged = False
-        while (nl_it < self.max_nl_it):
-            # Check convergence
-            if self._CheckFSIConvergence(nl_it, dis_residual_norm):
-                KratosMultiphysics.Logger.PrintInfo('PartitionedFSIBaseSolver', 'FSI non-linear iteration convergence achieved in {0} iterations.'.format(nl_it))
-                is_converged = True
-                break
-            else:
-                nl_it += 1
-
-            # Perform the displacement convergence accelerator update
-            self._GetConvergenceAccelerator().InitializeNonLinearIteration()
-            if not self._GetConvergenceAccelerator().IsBlockNewton():
-                self._GetFSICouplingInterfaceStructure().Update()
-            else:
-                self._GetFSICouplingInterfaceStructure().UpdateDisplacement()
-
-            # Update the structure interface position
-            self._GetFSICouplingInterfaceStructure().UpdatePosition(KratosMultiphysics.RELAXED_DISPLACEMENT)
-
-            # Map the relaxed displacement from the structure coupling interface to the fluid one
-            self._MapStructureInterfaceDisplacement()
-
-            # Solve the mesh and fluid problem
-            self._SolveFluid()
-
-            # Calculate the fluid interface traction from the interface reaction
-            #TODO: THINK ABOUT COMPUTING THE SUM OF NEGATIVE AND POSITIVE DISTRIBUTED LOAD AND TRANSFER THIS TO THE STRUCTURE (INSTEAD OF PASSING POSITIVE AND NEGATIVE)
-            self._CalculateFluidInterfaceTraction()
-
-            # Transfer the fluid traction to the structure interface
-            self._MapFluidInterfaceTraction()
-
-            # Compute the current iteration traction
-            if not self._GetConvergenceAccelerator().IsBlockNewton():
-                # Directly send the map load from the structure FSI coupling interface to the parent one
-                self._GetFSICouplingInterfaceStructure().TransferValuesToFatherModelPart(self._GetTractionVariable())
-            else:
-                # Perform the traction convergence accelerator update
-                self._GetFSICouplingInterfaceStructure().UpdateTraction()
-                KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
-                    KratosMultiphysics.RELAXED_TRACTION,
-                    self._GetTractionVariable(),
-                    self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-                    self._GetFSICouplingInterfaceStructure().GetFatherModelPart(),
-                    0)
-
-            self._GetConvergenceAccelerator().FinalizeNonLinearIteration()
-
-            # Solve the structure problem
-            self._SolveStructure()
-
-            # Compute the residual vector
-            dis_residual_norm = self._GetFSICouplingInterfaceStructure().ComputeResidualVector()
-
-            # Check if maximum iterations are reached
-            if nl_it == self.max_nl_it:
-                KratosMultiphysics.Logger.PrintWarning('PartitionedFSIBaseSolver', 'FSI non-linear maximum iterations {0} reached'.format(self.max_nl_it))
-
-        return is_converged
-
-    def FinalizeSolutionStep(self):
-        self.structure_solver.FinalizeSolutionStep()
-        self.fluid_solver.FinalizeSolutionStep()
-        self.mesh_solver.FinalizeSolutionStep()
-        self._GetConvergenceAccelerator().FinalizeSolutionStep()
-
-    def Finalize(self):
-        self.structure_solver.Finalize()
-        self.fluid_solver.Finalize()
-        self.mesh_solver.Finalize()
-        self._GetConvergenceAccelerator().Finalize()
-
-    def SetEchoLevel(self, structure_echo_level, fluid_echo_level):
-        self.structure_solver.SetEchoLevel(self, structure_echo_level)
-        self.fluid_solver.SetEchoLevel(self, fluid_echo_level)
-
-    def Clear(self):
-        self.fluid_solver.Clear()
-        self.structure_solver.Clear()
-
-    def Check(self):
-        self.fluid_solver.Check()
-        self.structure_solver.Check()
-
-    #######################################################################
-    ##############          PRIVATE METHODS SECTION          ##############
-    #######################################################################
-
-    def _AuxiliaryInitOperations(self):
-        # Auxiliar variables
-        self.parallel_type = self.settings["parallel_type"].GetString()
-        coupling_settings = self.settings["coupling_settings"]
-        self.max_nl_it = coupling_settings["nl_max_it"].GetInt()
-        self.nl_tol = coupling_settings["nl_tol"].GetDouble()
-        self.solve_mesh_at_each_iteration = coupling_settings["solve_mesh_at_each_iteration"].GetBool()
-
-        ## Save the FSI interfaces information in a dictionary
-        mappers_settings = self.settings["coupling_settings"]["mapper_settings"]
-        self.interfaces_dict = {}
-        self.interfaces_dict['structure'] = coupling_settings["structure_interfaces_list"][0].GetString()
-        if mappers_settings.size() == 1:
-            self.double_faced_structure = False
-            self.interfaces_dict['fluid_positive'] = mappers_settings[0]["fluid_interface_submodelpart_name"].GetString()
-            self.interfaces_dict['fluid_negative'] = None
-        elif mappers_settings.size() == 2:
-            self.double_faced_structure = True
-            for mapper_id in range(2):
-                if (mappers_settings[mapper_id]["mapper_face"].GetString() == "Positive"):
-                    self.interfaces_dict['fluid_positive'] = mappers_settings[mapper_id]["fluid_interface_submodelpart_name"].GetString()
-                elif (mappers_settings[mapper_id]["mapper_face"].GetString() == "Negative"):
-                    self.interfaces_dict['fluid_negative'] = mappers_settings[mapper_id]["fluid_interface_submodelpart_name"].GetString()
-                else:
-                    err_msg = "The mapper face is not \'Positve\' nor \'Negative\'."
-                    raise Exception(err_msg)
-        else:
-            err_msg = "Case with more than 2 mappers has not been implemented yet.\n"
-            err_msg += "Please, in case you are using single faced immersed bodies, set the skin entities in a unique submodelpart.\n"
-            err_msg += "In case you are considering double faced immersed bodies (shells or membranes), set all the positive faces in a unique submodelpart and all the negative ones in another submodelpart."
-            raise Exception(err_msg)
-
-        ## Construct the structure solver
-        self.structure_solver = python_solvers_wrapper_structural.CreateSolverByParameters(self.model, self.settings["structure_solver_settings"], self.parallel_type)
-        KratosMultiphysics.Logger.PrintInfo("PartitionedFSIBaseSolver", "Structure solver construction finished.")
-
-        ## Construct the fluid solver
-        self.fluid_solver = python_solvers_wrapper_fluid.CreateSolverByParameters(self.model, self.settings["fluid_solver_settings"], self.parallel_type)
-        KratosMultiphysics.Logger.PrintInfo("PartitionedFSIBaseSolver", "Fluid solver construction finished.")
-
-        ## Check the ALE settings before the mesh solver construction
-        mesh_solver_settings = self.settings["mesh_solver_settings"]
-        fluid_solver_settings = self.settings["fluid_solver_settings"]
-
-        # Check that the ALE and the fluid are the same model part
-        fluid_model_part_name =  fluid_solver_settings["model_part_name"].GetString()
-        if mesh_solver_settings.Has("model_part_name"):
-            if not fluid_model_part_name == mesh_solver_settings["model_part_name"].GetString():
-                err_msg =  'Fluid and mesh solver have to use the same MainModelPart ("model_part_name")!\n'
-                raise Exception(err_msg)
-        else:
-            mesh_solver_settings.AddValue("model_part_name", fluid_solver_settings["model_part_name"])
-
-        # Ensure that the fluid domain is not imported twice
-        if mesh_solver_settings.Has("model_import_settings"):
-            if mesh_solver_settings["model_import_settings"].Has("input_type"):
-                if not mesh_solver_settings["model_import_settings"]["input_type"].GetString() == "use_input_model_part":
-                    mesh_solver_settings["model_import_settings"]["input_type"].SetString("use_input_model_part")
-            else:
-                mesh_solver_settings["model_import_settings"].AddEmptyValue("input_type").SetString("use_input_model_part")
-        else:
-            mesh_solver_settings.AddEmptyValue("model_import_settings").AddEmptyValue("input_type").SetString("use_input_model_part")
-
-        # Check that the ALE and the fluid have the sime time scheme
-        if fluid_solver_settings.Has("time_scheme"):
-            fluid_time_scheme =  fluid_solver_settings["time_scheme"].GetString()
-            if mesh_solver_settings.Has("mesh_velocity_calculation"):
-                if mesh_solver_settings["mesh_velocity_calculation"].Has("time_scheme"):
-                    if not fluid_time_scheme == mesh_solver_settings["mesh_velocity_calculation"]["time_scheme"].GetString():
-                        err_msg = 'Fluid and mesh solver require to use the same time scheme ("time_scheme") for consistency!\n'
-                        raise Exception(err_msg)
-                else:
-                    mesh_solver_settings["mesh_velocity_calculation"].AddValue("time_scheme", fluid_solver_settings["time_scheme"])
-            else:
-                mesh_solver_settings.AddEmptyValue("mesh_velocity_calculation")
-                mesh_solver_settings["mesh_velocity_calculation"].AddValue("time_scheme", fluid_solver_settings["time_scheme"])
-
-        # Check domain size
-        fluid_domain_size = fluid_solver_settings["domain_size"].GetInt()
-        if mesh_solver_settings.Has("domain_size"):
-            if not fluid_domain_size == mesh_solver_settings["domain_size"].GetInt():
-                raise Exception('Fluid and mesh solver have different "domain_size"!')
-        else:
-            mesh_solver_settings.AddValue("domain_size", fluid_solver_settings["domain_size"])
-
-        # Ensure that the MESH_VELOCITY is computed
-        if mesh_solver_settings.Has("calculate_mesh_velocity"):
-            if not mesh_solver_settings["calculate_mesh_velocity"].GetBool():
-                mesh_solver_settings.SetValue("calculate_mesh_velocity", True)
-                KratosMultiphysics.Logger.PrintWarning("","Mesh velocity calculation was deactivated. Switching \"calculate_mesh_velocity\" on")
-        else:
-            mesh_solver_settings.AddEmptyValue("calculate_mesh_velocity").SetBool(True)
-
-        ## Construct the ALE mesh solver
-        self.mesh_solver = python_solvers_wrapper_mesh_motion.CreateSolverByParameters(self.model, self.settings["mesh_solver_settings"], self.parallel_type)
-        KratosMultiphysics.Logger.PrintInfo("PartitionedFSIBaseSolver", "ALE mesh solver construction finished.")
-
-    def _AdvanceInTimeCouplingInterfaces(self, new_time):
-        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart().CloneTimeStep(new_time)
-        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.STEP] = self._GetFSICouplingInterfaceStructure().GetFatherModelPart().ProcessInfo[KratosMultiphysics.STEP]
-        self._GetFSICouplingInterfaceFluidPositive().GetInterfaceModelPart().CloneTimeStep(new_time)
-        self._GetFSICouplingInterfaceFluidPositive().GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.STEP] = self._GetFSICouplingInterfaceFluidPositive().GetFatherModelPart().ProcessInfo[KratosMultiphysics.STEP]
-        if self.double_faced_structure:
-            self._GetFSICouplingInterfaceFluidNegative().GetInterfaceModelPart().CloneTimeStep(new_time)
-            self._GetFSICouplingInterfaceFluidNegative().GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.STEP] = self._GetFSICouplingInterfaceFluidNegative().GetFatherModelPart().ProcessInfo[KratosMultiphysics.STEP]
-
-    # This method finds the maximum buffer size between mesh,
-    # fluid and structure solvers and sets it to all the solvers.
-    def _GetAndSetMinimumBufferSize(self):
-        fluid_buffer_size = self.fluid_solver.min_buffer_size
-        mesh_buffer_size = self.mesh_solver.settings["buffer_size"].GetInt()
-        str_buffer_size = self.structure_solver.settings["buffer_size"].GetInt()
-
-        buffer_size = max(fluid_buffer_size, mesh_buffer_size)
-        buffer_size = max(buffer_size, str_buffer_size)
-
-        self.fluid_solver.min_buffer_size = buffer_size
-        self.mesh_solver.settings["buffer_size"].SetInt(buffer_size)
-        self.structure_solver.settings["buffer_size"].SetInt(buffer_size)
-
-    #TODO: SHOULDN'T BE NEEDED AS WE ALWAYS USE THE POSITIVE ONE
-    # def _GetFluidInterfaceSubmodelPart(self):
-    #     # Returns the fluid interface submodelpart that will be used in the residual minimization
-    #     return self.fluid_solver.main_model_part.GetSubModelPart(self.fluid_interface_submodelpart_name)
-
-    def _InitializeCouplingInterfaces(self):
-        # Prepare the Dirichlet fluid interfaces
-        self.__SetFluidInterfaceFixity(self._GetFluidPositiveInterfaceSubmodelPart())
-        KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self._GetFluidPositiveInterfaceSubmodelPart().Nodes)
-        if self.double_faced_structure:
-            self.__SetFluidInterfaceFixity(self._GetFluidNegativeInterfaceSubmodelPart())
-            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self._GetFluidNegativeInterfaceSubmodelPart().Nodes)
-
-        # Prepare the Neumann structure interface
-        self._SetStructureNeumannCondition()
-        KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self._GetStructureInterfaceSubmodelPart().Nodes)
-
-    def __SetFluidInterfaceFixity(self, fluid_interface_submodelpart):
-        # Fix the VELOCITY, MESH_DISPLACEMENT and MESH_VELOCITY variables in all the fluid interface submodelparts
-        KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.VELOCITY_X, True, fluid_interface_submodelpart.Nodes)
-        KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.VELOCITY_Y, True, fluid_interface_submodelpart.Nodes)
-        KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.MESH_DISPLACEMENT_X, True, fluid_interface_submodelpart.Nodes)
-        KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.MESH_DISPLACEMENT_Y, True, fluid_interface_submodelpart.Nodes)
-        if self._GetDomainSize() == 3:
-            KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.VELOCITY_Z, True, fluid_interface_submodelpart.Nodes)
-            KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.MESH_DISPLACEMENT_Z, True, fluid_interface_submodelpart.Nodes)
-
-    def _GetFluidPositiveInterfaceSubmodelPart(self):
-        # Returns the fluid positive interface submodelpart
-        positive_interface_name = self.interfaces_dict['fluid_positive']
-        return self.model.GetModelPart(positive_interface_name)
-
-    def _GetFluidNegativeInterfaceSubmodelPart(self):
-        negative_interface_name = self.interfaces_dict['fluid_negative']
-        return self.model.GetModelPart(negative_interface_name)
-
-    def _GetStructureInterfaceSubmodelPart(self):
-        # Returns the structure interface submodelpart that will be used in the residual minimization
-        return self.model.GetModelPart(self.__GetStructureInterfaceModelPartName())
-
-    def __GetStructureInterfaceModelPartName(self):
-        if not hasattr(self, '_structure_interface_submodelpart_name'):
-            str_int_list = self.settings["coupling_settings"]["structure_interfaces_list"]
-            if (str_int_list.size() != 1):
-                raise Exception("FSI structure skin must be contained in a unique model part")
-            self._structure_interface_submodelpart_name = str_int_list[0].GetString()
-        return self._structure_interface_submodelpart_name
-
-    def _GetDomainSize(self):
-        if not hasattr(self, '_domain_size'):
-            fluid_domain_size = self.fluid_solver.main_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
-            structure_domain_size = self.structure_solver.main_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
-            if fluid_domain_size !=structure_domain_size:
-                raise("ERROR: Solid domain size and fluid domain size are not equal!")
-            self._domain_size = fluid_domain_size
-        return self._domain_size
-
-    def  _ComputeDeltaTime(self):
-        fluid_time_step = self.fluid_solver._ComputeDeltaTime()
-        structure_time_step = self.structure_solver.ComputeDeltaTime()
-
-        if abs(fluid_time_step - structure_time_step) > 1e-12:
-            err_msg =  'Fluid time step is: ' + str(fluid_time_step) + '\n'
-            err_msg += 'Structure time step is: ' + str(structure_time_step) + '\n'
-            err_msg += 'No substepping has been implemented yet. Fluid and structure time step must coincide.'
-            raise Exception(err_msg)
-
-        return fluid_time_step
-
-    #TODO: THIS MUST BE DONE IN C++ (FSIPartitionedUtils)
-    #TODO: THINK ABOUT ASSUMING THESE TO BE ALREADY IN THE MPDA (AS THE EMBEDDED DOES) OR TO ALWAYS CREATE THEM (ALSO IN THE EMBEDDED)
-    def _SetStructureNeumannCondition(self):
-
-        structure_computational_submodelpart = self.structure_solver.GetComputingModelPart()
-
-        # Get the maximum condition id
-        max_cond_id = 0
-        for condition in self.structure_solver.main_model_part.Conditions:
-            max_cond_id = max(max_cond_id, condition.Id)
-
-        max_cond_id = self.structure_solver.main_model_part.GetCommunicator().GetDataCommunicator().MaxAll(max_cond_id)
-
-        # Set up the point load condition in the structure interface
-        structure_interfaces_list = self.settings["coupling_settings"]["structure_interfaces_list"]
-        for i in range(structure_interfaces_list.size()):
-            interface_submodelpart_name = structure_interfaces_list[i].GetString()
-            interface_submodelpart_i = self.model.GetModelPart(interface_submodelpart_name)
-
-            # Get the number of conditions to be set in each processor
-            local_nodes_number_accumulated = -1
-            local_nodes_number = len(interface_submodelpart_i.GetCommunicator().LocalMesh().Nodes)
-            local_nodes_number_accumulated = interface_submodelpart_i.GetCommunicator().GetDataCommunicator().ScanSum(local_nodes_number)
-
-            # Create the point load condition
-            aux_count = max_cond_id + local_nodes_number_accumulated
-            if self._GetDomainSize() == 2:
-                for node in interface_submodelpart_i.GetCommunicator().LocalMesh().Nodes:
-                    aux_count+=1
-                    structure_computational_submodelpart.CreateNewCondition("PointLoadCondition2D1N",
-                                                                            int(aux_count),
-                                                                            [node.Id],
-                                                                            self.structure_solver.main_model_part.Properties[0])
-            elif self._GetDomainSize() == 3:
-                for node in interface_submodelpart_i.GetCommunicator().LocalMesh().Nodes:
-                    aux_count+=1
-                    structure_computational_submodelpart.CreateNewCondition("PointLoadCondition3D1N",
-                                                                            int(aux_count),
-                                                                            [node.Id],
-                                                                            self.structure_solver.main_model_part.Properties[0])
-
-    def _GetStructureToFluidPositiveInterfaceMapper(self):
-        if not hasattr(self, '_structure_to_fluid_positive_interface_mapper'):
-            self._structure_to_fluid_positive_interface_mapper = self._CreateStructureToFluidInterfaceMapper(
-                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-                self._GetFSICouplingInterfaceFluidPositive().GetInterfaceModelPart())
-        return self._structure_to_fluid_positive_interface_mapper
-
-    def _GetStructureToFluidNegativeInterfaceMapper(self):
-        if not hasattr(self, '_structure_to_fluid_negative_interface_mapper'):
-            self._structure_to_fluid_negative_interface_mapper = self._CreateStructureToFluidInterfaceMapper(
-                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-                self._GetFSICouplingInterfaceFluidNegative().GetInterfaceModelPart())
-        return self._structure_to_fluid_negative_interface_mapper
-
-    @classmethod
-    def _CreateStructureToFluidInterfaceMapper(self, structure_interface, fluid_interface):
-        mapper_params = KratosMultiphysics.Parameters("""{
-            "mapper_type": "nearest_element",
-            "echo_level" : 0
-        }""")
-        structure_to_fluid_interface_mapper = KratosMapping.MapperFactory.CreateMapper(
-            structure_interface,
-            fluid_interface,
-            mapper_params)
-
-        return structure_to_fluid_interface_mapper
-
-    def _GetFSICouplingInterfaceStructure(self):
-        if not hasattr(self, '_fsi_coupling_interface_structure'):
-            self._fsi_coupling_interface_structure = self._CreateFSICouplingInterfaceStructure()
-        return self._fsi_coupling_interface_structure
-
-    def _CreateFSICouplingInterfaceStructure(self):
-        # Set auxiliary settings
-        aux_settings = KratosMultiphysics.Parameters(
-        """{
-            "model_part_name": "FSICouplingInterfaceStructure",
-            "parent_model_part_name": "",
-            "input_variable_list": ["SURFACE_LOAD"],
-            "output_variable_list": ["DISPLACEMENT"]
-        }""")
-        aux_settings["parent_model_part_name"].SetString(self.interfaces_dict['structure'])
-
-        # Get the convergence accelerator instance (note that it is created in this call)
-        convergence_accelerator = self._GetConvergenceAccelerator()
-
-        # Construct the FSI coupling interface
-        fsi_coupling_interface_structure = fsi_coupling_interface.FSICouplingInterface(
-            self.model,
-            aux_settings,
-            convergence_accelerator)
-
-        KratosMultiphysics.Logger.PrintInfo('PartitionedFSIBaseSolver', 'Structure FSI coupling interface created')
-
-        return fsi_coupling_interface_structure
-
-    @classmethod
-    def _GetFSICouplingInterfaceFluid(self):
-        err_msg = 'Body-fitted partitioned FSI solver does not implement the \'_GetFSICouplingInterfaceFluid\' method.\n'
-        err_msg += 'Use \'_GetFSICouplingInterfaceFluidPositive\' as well as \'_GetFSICouplingInterfaceFluidNegative\' if the structure is thin-walled.'
-        raise Exception(err_msg)
-
-    def _GetFSICouplingInterfaceFluidPositive(self):
-        if not hasattr(self, '_fsi_coupling_interface_fluid_positive'):
-            fluid_interface_side = 'fluid_positive'
-            self._fsi_coupling_interface_fluid_positive = self.__CreateFSICouplingInterfaceFluid(fluid_interface_side)
-        return self._fsi_coupling_interface_fluid_positive
-
-    def _GetFSICouplingInterfaceFluidNegative(self):
-        if not hasattr(self, '_fsi_coupling_interface_fluid_negative'):
-            fluid_interface_side = 'fluid_negative'
-            self._fsi_coupling_interface_fluid_negative = self.__CreateFSICouplingInterfaceFluid(fluid_interface_side)
-        return self._fsi_coupling_interface_fluid_negative
-
-    def __CreateFSICouplingInterfaceFluid(self, fluid_interface_side):
-        # Set auxiliary settings
-        aux_settings = KratosMultiphysics.Parameters(
-        """{
-            "model_part_name": "",
-            "parent_model_part_name": "",
-            "input_variable_list": ["MESH_DISPLACEMENT"],
-            "output_variable_list": []
-        }""")
-        aux_settings["model_part_name"].SetString("FSICouplingInterface{}".format(fluid_interface_side.capitalize()))
-        aux_settings["parent_model_part_name"].SetString(self.interfaces_dict[fluid_interface_side])
-        aux_settings["output_variable_list"].Append("{}_MAPPED_VECTOR_VARIABLE".format("POSITIVE" if fluid_interface_side == 'fluid_positive' else "NEGATIVE"))
-
-        # Construct the FSI coupling interface
-        # Note that no convergence accelerator is created in the fluid side
-        fsi_coupling_interface_fluid = fsi_coupling_interface.FSICouplingInterface(
-            self.model,
-            aux_settings)
-
-        KratosMultiphysics.Logger.PrintInfo('PartitionedFSIBaseSolver', 'Fluid {} FSI coupling interface created'.format(fluid_interface_side))
-
-        return fsi_coupling_interface_fluid
-
-    # This method returns the convergence accelerator.
-    # If it is not created yet, it calls the _CreateConvergenceAccelerator first
-    def _GetConvergenceAccelerator(self):
-        if not hasattr(self, '_convergence_accelerator'):
-            self._convergence_accelerator = self._CreateConvergenceAccelerator()
-        return self._convergence_accelerator
-
-    # This method constructs the convergence accelerator coupling utility
-    def _CreateConvergenceAccelerator(self):
-        convergence_accelerator = convergence_accelerator_factory.CreateConvergenceAccelerator(self.settings["coupling_settings"]["coupling_strategy_settings"])
-        KratosMultiphysics.Logger.PrintInfo('PartitionedFSIBaseSolver', 'Coupling strategy construction finished')
-        return convergence_accelerator
-
-    def _MapStructureInterfaceDisplacement(self):
-        # Map the RELAXED_DISPLACEMENT from the structure FSI coupling interface to fluid FSI coupling interface
-        self._GetStructureToFluidPositiveInterfaceMapper().Map(
-            KratosMultiphysics.RELAXED_DISPLACEMENT,
-            KratosMultiphysics.MESH_DISPLACEMENT)
-
-        # In case the structure is double faced, we take advantage of the equal positive and negative sides meshes
-        if self.double_faced_structure:
-            KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
-                KratosMultiphysics.MESH_DISPLACEMENT,
-                KratosMultiphysics.MESH_DISPLACEMENT,
-                self._GetFSICouplingInterfaceFluidPositive.GetInterfaceModelPart(),
-                self._GetFSICouplingInterfaceFluidNegative.GetInterfaceModelPart())
-
-        # Update the fluid interface position
-        self._GetFSICouplingInterfaceFluidPositive().UpdatePosition(KratosMultiphysics.MESH_DISPLACEMENT)
-        if self.double_faced_structure:
-            self._GetFSICouplingInterfaceFluidNegative().UpdatePosition(KratosMultiphysics.MESH_DISPLACEMENT)
-
-    def _SolveFluid(self):
-        # Transfer values from fluid FSI coupling interface to fluid skin
-        self._GetFSICouplingInterfaceFluidPositive().TransferValuesToFatherModelPart(KratosMultiphysics.MESH_DISPLACEMENT)
-        if self.double_faced_structure:
-            self._GetFSICouplingInterfaceFluidNegative().TransferValuesToFatherModelPart(KratosMultiphysics.MESH_DISPLACEMENT)
-
-        # Solve the mesh problem (or moves the interface nodes)
-        if self.solve_mesh_at_each_iteration:
-            self.mesh_solver.SolveSolutionStep()
-        else:
-            self.mesh_solver.MoveMesh()
-
-        # Impose the structure MESH_VELOCITY in the fluid interface VELOCITY (Lagrangian interface)
-        KratosMultiphysics.VariableUtils().CopyVariable(
-                KratosMultiphysics.MESH_VELOCITY,
-                KratosMultiphysics.VELOCITY,
-                self._GetFluidPositiveInterfaceSubmodelPart().GetCommunicator().LocalMesh().Nodes)
-        self._GetFluidPositiveInterfaceSubmodelPart().GetCommunicator().SynchronizeVariable(KratosMultiphysics.VELOCITY)
-        if self.double_faced_structure:
-            KratosMultiphysics.VariableUtils().CopyVariable(
-                    KratosMultiphysics.MESH_VELOCITY,
-                    KratosMultiphysics.VELOCITY,
-                    self._GetFluidNegativeInterfaceSubmodelPart().GetCommunicator().LocalMesh().Nodes)
-            self._GetFluidNegativeInterfaceSubmodelPart().GetCommunicator().SynchronizeVariable(KratosMultiphysics.VELOCITY)
-
-        # Solve fluid problem
-        self.fluid_solver.SolveSolutionStep()
-
-    def _CalculateFluidInterfaceTraction(self):
-        # Distribute the REACTION point load
-        distribution_tolerance = 1.0e-12
-        distribution_max_iterations = 500
-
-        KratosMultiphysics.VariableRedistributionUtility.DistributePointValues(
-            self._GetFluidPositiveInterfaceSubmodelPart(),
-            self._GetFluidPositiveInterfaceSubmodelPart().Conditions,
-            KratosMultiphysics.REACTION,
-            KratosMultiphysics.POSITIVE_MAPPED_VECTOR_VARIABLE,
-            distribution_tolerance,
-            distribution_max_iterations)
-        if self.double_faced_structure:
-            KratosMultiphysics.VariableRedistributionUtility.DistributePointValues(
-                self._GetFluidNegativeInterfaceSubmodelPart(),
-                self._GetFluidNegativeInterfaceSubmodelPart().Conditions,
-                KratosMultiphysics.REACTION,
-                KratosMultiphysics.NEGATIVE_MAPPED_VECTOR_VARIABLE,
-                distribution_tolerance,
-                distribution_max_iterations)
-
-        # Transfer traction values from fluid interface to fluid FSI coupling interface
-        # NOTE: POSITIVE_MAPPED_VECTOR_VARIABLE is the positive side traction
-        # NOTE: NEGATIVE_MAPPED_VECTOR_VARIABLE is the negative side traction
-        self._GetFSICouplingInterfaceFluidPositive().GetValuesFromFatherModelPart(KratosMultiphysics.POSITIVE_MAPPED_VECTOR_VARIABLE)
-        if self.double_faced_structure:
-            self._GetFSICouplingInterfaceFluidNegative().GetValuesFromFatherModelPart(KratosMultiphysics.NEGATIVE_MAPPED_VECTOR_VARIABLE)
-
-    def _MapFluidInterfaceTraction(self):
-        # Map the distributed REACTION from the fluid FSI coupling interface to structure FSI coupling interface
-        self._GetStructureToFluidPositiveInterfaceMapper().InverseMap(
-            self._GetTractionVariable(),
-            KratosMultiphysics.POSITIVE_MAPPED_VECTOR_VARIABLE,
-            KratosMultiphysics.Mapper.SWAP_SIGN)
-        if self.double_faced_structure:
-            self._GetStructureToFluidNegativeInterfaceMapper().InverseMap(
-                self._GetTractionVariable(),
-                KratosMultiphysics.NEGATIVE_MAPPED_VECTOR_VARIABLE,
-                KratosMultiphysics.Mapper.ADD_VALUES | KratosMultiphysics.Mapper.SWAP_SIGN)
-
-        # Send the mapped load from the structure FSI coupling interface to the parent one
-        self._GetFSICouplingInterfaceStructure().TransferValuesToFatherModelPart(self._GetTractionVariable())
-
-    def _SolveStructure(self):
-        #TODO: Once we use the distributed (relaxed) traction in the body fitted we can remove this as well as the _SolveStructure in the embedded solver
-        # Convert distributed traction to point values
-        KratosMultiphysics.VariableRedistributionUtility.ConvertDistributedValuesToPoint(
-            self._GetStructureInterfaceSubmodelPart(),
-            self._GetStructureInterfaceSubmodelPart().Conditions,
-            self._GetTractionVariable(),
-            KratosStructural.POINT_LOAD)
-
-        # Solve the structure problem
-        self.structure_solver.SolveSolutionStep()
-
-    def _ComputeInitialResidual(self):
-        # Save as RELAXED_DISPLACEMENT the DISPLACEMENT coming from the structure Predict()
-        # Note that this would be required in order to set the first observation matrices
-        KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
-            KratosMultiphysics.DISPLACEMENT,
-            KratosMultiphysics.RELAXED_DISPLACEMENT,
-            self._GetStructureInterfaceSubmodelPart(),
-            self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-            0)
-
-        # Update the structure interface position with the DISPLACEMENT values from the predict
-        self._GetFSICouplingInterfaceStructure().UpdatePosition(KratosMultiphysics.RELAXED_DISPLACEMENT)
-
-        # Map the relaxed displacement from the structure coupling interface to the fluid one
-        self._MapStructureInterfaceDisplacement()
-
-        # Solve the mesh and fluid problem
-        self._SolveFluid()
-
-        # Calculate the fluid interface traction from the interface reaction
-        #TODO: THINK ABOUT COMPUTING THE SUM OF NEGATIVE AND POSITIVE DISTRIBUTED LOAD AND TRANSFER THIS TO THE STRUCTURE (INSTEAD OF PASSING POSITIVE AND NEGATIVE)
-        self._CalculateFluidInterfaceTraction()
-
-        # Transfer the fluid traction to the structure interface
-        self._MapFluidInterfaceTraction()
-
-        # Save as RELAXED_TRATION the TRACTION coming from the fluid
-        # Note that this would be required in order to set the first observation matrices
-        if self._GetConvergenceAccelerator().IsBlockNewton():
-            KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
-                self._GetTractionVariable(),
-                KratosMultiphysics.RELAXED_TRACTION,
-                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-                0)
-
-        # Directly send the map load from the structure FSI coupling interface to the parent one
-        self._GetFSICouplingInterfaceStructure().TransferValuesToFatherModelPart(self._GetTractionVariable())
-
-        # Solve the structure problem
-        self._SolveStructure()
-
-        # Compute the residual vector
-        dis_residual_norm = self._GetFSICouplingInterfaceStructure().ComputeResidualVector()
-
-        return dis_residual_norm
-
-    def _CheckFSIConvergence(self, nl_it, residual_norm):
-        interface_dofs = self._GetPartitionedFSIUtilities().GetInterfaceResidualSize(self._GetStructureInterfaceSubmodelPart())
-        normalised_residual = residual_norm/sqrt(interface_dofs)
-        KratosMultiphysics.Logger.PrintInfo('PartitionedFSIBaseSolver', 'FSI non-linear iteration = {0} |res|/sqrt(nDOFS) = {1}'.format(nl_it, normalised_residual))
-        return normalised_residual < self.nl_tol
-
-    def _GetPartitionedFSIUtilities(self):
-        if not hasattr(self, '_partitioned_fsi_utilities'):
-            self._partitioned_fsi_utilities = self._CreatePartitionedFSIUtilities()
-        return self._partitioned_fsi_utilities
-
-    def _CreatePartitionedFSIUtilities(self):
-        if self._GetDomainSize() == 2:
-            return KratosFSI.PartitionedFSIUtilitiesArray2D()
-        elif self._GetDomainSize() == 3:
-            return KratosFSI.PartitionedFSIUtilitiesArray3D()
-        else:
-            raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
-
-    @classmethod
-    def _GetTractionVariable(self):
-        #NOTE: No distinction is made between LINE_LOAD and SURFACE_LOAD as this is only used for the redistribution
-        #NOTE: Hence, this has only an auxiliary use as the traction will be converted to point load prior to the structure solve
-        #TODO: Use LINE_LOAD in 2D and SURFACE_LOAD in 3D when using distributed loads conditions
-        return KratosStructural.SURFACE_LOAD
+from math import sqrt   # Import the square root from python library
+
+# Import utilities
+from KratosMultiphysics.FluidDynamicsApplication import python_solvers_wrapper_fluid            # Import the fluid Python solvers wrapper
+from KratosMultiphysics.StructuralMechanicsApplication import python_solvers_wrapper_structural       # Import the structure Python solvers wrapper
+from KratosMultiphysics.MeshMovingApplication import python_solvers_wrapper_mesh_motion      # Import the mesh motion Python solvers wrapper
+from KratosMultiphysics.FSIApplication import fsi_coupling_interface                            # Import the FSI coupling interface utility
+from KratosMultiphysics.FSIApplication import convergence_accelerator_factory         # Import the FSI convergence accelerator factory
+
+# Importing the Kratos Library
+import KratosMultiphysics
+from KratosMultiphysics.python_solver import PythonSolver
+
+# Import applications
+import KratosMultiphysics.FSIApplication as KratosFSI
+import KratosMultiphysics.MappingApplication as KratosMapping
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+
+def CreateSolver(model, project_parameters):
+    return PartitionedFSIBaseSolver(model, project_parameters)
+
+class PartitionedFSIBaseSolver(PythonSolver):
+    def __init__(self, model, project_parameters):
+        # TODO: Remove this as soon as the MPCs are implemented in MPI
+        # This has to be done prior to the defaults check to avoid the structural solver to throw an error in MPI
+        if not project_parameters["structure_solver_settings"].Has("multi_point_constraints_used"):
+            project_parameters["structure_solver_settings"].AddEmptyValue("multi_point_constraints_used")
+            project_parameters["structure_solver_settings"]["multi_point_constraints_used"].SetBool(False)
+
+        # Call the base Python solver constructor
+        # Note that default settings in GetDefaultParameters() are validated in here
+        super().__init__(model, project_parameters)
+
+        # This method encapsulates all the operations required to be done in the constructor
+        # It is intended to be overwritten in the derived classes
+        self._AuxiliaryInitOperations()
+
+        KratosMultiphysics.Logger.PrintInfo("PartitionedFSIBaseSolver", "Partitioned FSI base solver construction finished.")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+
+        # Note that only the coupling settings are validated
+        # The subdomain solver settings will be validated while instantiating these
+        this_defaults = KratosMultiphysics.Parameters("""{
+            "echo_level": 0,
+            "parallel_type": "OpenMP",
+            "solver_type": "partitioned",
+            "coupling_scheme": "dirichlet_neumann",
+            "structure_solver_settings": {
+            },
+            "fluid_solver_settings":{
+            },
+            "mesh_solver_settings":{
+            },
+            "coupling_settings":{
+                "coupling_strategy_settings": {
+                    "solver_type": "MVQN",
+                    "w_0": 0.825
+                },
+                "mapper_settings": [{
+                    "fluid_interface_submodelpart_name": "",
+                    "mapper_face": "unique",
+                    "structure_interface_submodelpart_name": ""
+                }],
+                "nl_max_it": 25,
+                "nl_tol": 1e-8,
+                "solve_mesh_at_each_iteration": true,
+                "fluid_interfaces_list": [],
+                "structure_interfaces_list": []
+            }
+        }""")
+
+        this_defaults.AddMissingParameters(super().GetDefaultParameters())
+        return this_defaults
+
+    def ValidateSettings(self):
+        default_settings = self.GetDefaultParameters()
+
+        ## Base class settings validation
+        super().ValidateSettings()
+
+        ## Validate coupling settings
+        self.settings["coupling_settings"].ValidateAndAssignDefaults(default_settings["coupling_settings"])
+
+    def GetMinimumBufferSize(self):
+        # Get structure buffer size
+        buffer_structure = self.structure_solver.GetMinimumBufferSize()
+        # Get fluid buffer size
+        buffer_fluid = self.fluid_solver.GetMinimumBufferSize()
+
+        return max(buffer_structure,buffer_fluid)
+
+    def AddVariables(self):
+        ## Structure variables addition
+        # Standard CSM variables addition
+        self.structure_solver.AddVariables()
+
+        ## Fluid variables addition
+        # Standard CFD variables addition
+        self.fluid_solver.AddVariables()
+        # Mesh solver variables addition
+        self.mesh_solver.AddVariables()
+
+        ## Fluid traction variables addition
+        # These are required for the reaction variable redistribution in the fluid model part skin
+        self.fluid_solver.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_MAPPED_VECTOR_VARIABLE)
+        self.fluid_solver.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NEGATIVE_MAPPED_VECTOR_VARIABLE)
+
+    def ImportModelPart(self):
+        # Fluid and structure solvers ImportModelPart() call
+        self.fluid_solver.ImportModelPart()
+        self.structure_solver.ImportModelPart()
+        self.mesh_solver.ImportModelPart()
+
+    def PrepareModelPart(self):
+        # Fluid and structure solvers PrepareModelPart() call
+        self.structure_solver.PrepareModelPart()
+        self.fluid_solver.PrepareModelPart()
+        self.mesh_solver.PrepareModelPart()
+
+        # FSI interface coupling interfaces initialization
+        # The getter methods are to construct the FSI coupling interfaces in here
+        self._GetFSICouplingInterfaceFluidPositive().GetInterfaceModelPart()
+        if self.double_faced_structure:
+            self._GetFSICouplingInterfaceFluidNegative().GetInterfaceModelPart()
+        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart()
+
+    def AddDofs(self):
+        # Add DOFs structure
+        self.structure_solver.AddDofs()
+
+        # Add DOFs fluid
+        self.fluid_solver.AddDofs()
+        self.mesh_solver.AddDofs()
+
+    def Initialize(self):
+        # Create the required mappers
+        self._GetStructureToFluidPositiveInterfaceMapper()
+        if self.double_faced_structure:
+            self._GetStructureToFluidNegativeInterfaceMapper()
+
+        # Coupling utility initialization
+        # The _GetConvergenceAccelerator is supposed to construct the convergence accelerator in here
+        self._GetConvergenceAccelerator().Initialize()
+
+        # Python structure solver initialization
+        self.structure_solver.Initialize()
+
+        # Ensure that the fluid reaction fluxes are computed before initializing the fluid strategy
+        if self.fluid_solver.settings["compute_reactions"].GetBool() == False:
+            self.fluid_solver.settings["compute_reactions"].SetBool(True)
+
+        # Python fluid solver initialization
+        self.fluid_solver.Initialize()
+
+        # Python mesh solver initialization
+        self.mesh_solver.Initialize()
+
+        # Perform all the operations required to set up the coupling interfaces
+        self._InitializeCouplingInterfaces()
+
+    def AdvanceInTime(self, current_time):
+        # Subdomains time advance
+        fluid_new_time = self.fluid_solver.AdvanceInTime(current_time)
+        structure_new_time = self.structure_solver.AdvanceInTime(current_time)
+
+        if abs(fluid_new_time - structure_new_time) > 1e-12:
+            err_msg =  'Fluid new time is: ' + str(fluid_new_time) + '\n'
+            err_msg += 'Structure new time is: ' + str(structure_new_time) + '\n'
+            err_msg += 'No substepping has been implemented yet. Fluid and structure time must coincide.'
+            raise Exception(err_msg)
+
+        # Update the auxiliary coupling interface model parts database in case these are to be output
+        # Note that there are also situations (e.g. embedded) in which this is mandatory for the proper performance of the solver
+        self._AdvanceInTimeCouplingInterfaces(fluid_new_time)
+
+        return fluid_new_time
+
+    def InitializeSolutionStep(self):
+        # Initialize solution step of fluid, structure and coupling solvers
+        self.structure_solver.InitializeSolutionStep()
+        self.fluid_solver.InitializeSolutionStep()
+        self.mesh_solver.InitializeSolutionStep()
+        self._GetConvergenceAccelerator().InitializeSolutionStep()
+
+    def Predict(self):
+        # Perform fluid and structure solvers predictions
+        self.structure_solver.Predict()
+        self.fluid_solver.Predict()
+        self.mesh_solver.Predict()
+
+    def GetComputingModelPart(self):
+        err_msg =  'Calling GetComputingModelPart() method in a partitioned solver.\n'
+        err_msg += 'Specify the domain of interest by calling:\n'
+        err_msg += '\t- GetFluidComputingModelPart()\n'
+        err_msg += '\t- GetStructureComputingModelPart()\n'
+        raise Exception(err_msg)
+
+    def GetFluidComputingModelPart(self):
+        return self.fluid_solver.GetComputingModelPart()
+
+    def GetStructureComputingModelPart(self):
+        return self.structure_solver.GetComputingModelPart()
+
+    def GetOutputVariables(self):
+        pass
+
+    def SaveRestart(self):
+        pass
+
+    def SolveSolutionStep(self):
+        ## Initialize residual
+        dis_residual_norm = self._ComputeInitialResidual()
+
+        ## FSI nonlinear iteration loop
+        nl_it = 1
+        is_converged = False
+        while (nl_it < self.max_nl_it):
+            # Check convergence
+            if self._CheckFSIConvergence(nl_it, dis_residual_norm):
+                KratosMultiphysics.Logger.PrintInfo('PartitionedFSIBaseSolver', 'FSI non-linear iteration convergence achieved in {0} iterations.'.format(nl_it))
+                is_converged = True
+                break
+            else:
+                nl_it += 1
+
+            # Perform the displacement convergence accelerator update
+            self._GetConvergenceAccelerator().InitializeNonLinearIteration()
+            if not self._GetConvergenceAccelerator().IsBlockNewton():
+                self._GetFSICouplingInterfaceStructure().Update()
+            else:
+                self._GetFSICouplingInterfaceStructure().UpdateDisplacement()
+
+            # Update the structure interface position
+            self._GetFSICouplingInterfaceStructure().UpdatePosition(KratosMultiphysics.RELAXED_DISPLACEMENT)
+
+            # Map the relaxed displacement from the structure coupling interface to the fluid one
+            self._MapStructureInterfaceDisplacement()
+
+            # Solve the mesh and fluid problem
+            self._SolveFluid()
+
+            # Calculate the fluid interface traction from the interface reaction
+            #TODO: THINK ABOUT COMPUTING THE SUM OF NEGATIVE AND POSITIVE DISTRIBUTED LOAD AND TRANSFER THIS TO THE STRUCTURE (INSTEAD OF PASSING POSITIVE AND NEGATIVE)
+            self._CalculateFluidInterfaceTraction()
+
+            # Transfer the fluid traction to the structure interface
+            self._MapFluidInterfaceTraction()
+
+            # Compute the current iteration traction
+            if not self._GetConvergenceAccelerator().IsBlockNewton():
+                # Directly send the map load from the structure FSI coupling interface to the parent one
+                self._GetFSICouplingInterfaceStructure().TransferValuesToFatherModelPart(self._GetTractionVariable())
+            else:
+                # Perform the traction convergence accelerator update
+                self._GetFSICouplingInterfaceStructure().UpdateTraction()
+                KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
+                    KratosMultiphysics.RELAXED_TRACTION,
+                    self._GetTractionVariable(),
+                    self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+                    self._GetFSICouplingInterfaceStructure().GetFatherModelPart(),
+                    0)
+
+            self._GetConvergenceAccelerator().FinalizeNonLinearIteration()
+
+            # Solve the structure problem
+            self._SolveStructure()
+
+            # Compute the residual vector
+            dis_residual_norm = self._GetFSICouplingInterfaceStructure().ComputeResidualVector()
+
+            # Check if maximum iterations are reached
+            if nl_it == self.max_nl_it:
+                KratosMultiphysics.Logger.PrintWarning('PartitionedFSIBaseSolver', 'FSI non-linear maximum iterations {0} reached'.format(self.max_nl_it))
+
+        return is_converged
+
+    def FinalizeSolutionStep(self):
+        self.structure_solver.FinalizeSolutionStep()
+        self.fluid_solver.FinalizeSolutionStep()
+        self.mesh_solver.FinalizeSolutionStep()
+        self._GetConvergenceAccelerator().FinalizeSolutionStep()
+
+    def Finalize(self):
+        self.structure_solver.Finalize()
+        self.fluid_solver.Finalize()
+        self.mesh_solver.Finalize()
+        self._GetConvergenceAccelerator().Finalize()
+
+    def SetEchoLevel(self, structure_echo_level, fluid_echo_level):
+        self.structure_solver.SetEchoLevel(self, structure_echo_level)
+        self.fluid_solver.SetEchoLevel(self, fluid_echo_level)
+
+    def Clear(self):
+        self.fluid_solver.Clear()
+        self.structure_solver.Clear()
+
+    def Check(self):
+        self.fluid_solver.Check()
+        self.structure_solver.Check()
+
+    #######################################################################
+    ##############          PRIVATE METHODS SECTION          ##############
+    #######################################################################
+
+    def _AuxiliaryInitOperations(self):
+        # Auxiliar variables
+        self.parallel_type = self.settings["parallel_type"].GetString()
+        coupling_settings = self.settings["coupling_settings"]
+        self.max_nl_it = coupling_settings["nl_max_it"].GetInt()
+        self.nl_tol = coupling_settings["nl_tol"].GetDouble()
+        self.solve_mesh_at_each_iteration = coupling_settings["solve_mesh_at_each_iteration"].GetBool()
+
+        ## Save the FSI interfaces information in a dictionary
+        mappers_settings = self.settings["coupling_settings"]["mapper_settings"]
+        self.interfaces_dict = {}
+        self.interfaces_dict['structure'] = coupling_settings["structure_interfaces_list"][0].GetString()
+        if mappers_settings.size() == 1:
+            self.double_faced_structure = False
+            self.interfaces_dict['fluid_positive'] = mappers_settings[0]["fluid_interface_submodelpart_name"].GetString()
+            self.interfaces_dict['fluid_negative'] = None
+        elif mappers_settings.size() == 2:
+            self.double_faced_structure = True
+            for mapper_id in range(2):
+                if (mappers_settings[mapper_id]["mapper_face"].GetString() == "Positive"):
+                    self.interfaces_dict['fluid_positive'] = mappers_settings[mapper_id]["fluid_interface_submodelpart_name"].GetString()
+                elif (mappers_settings[mapper_id]["mapper_face"].GetString() == "Negative"):
+                    self.interfaces_dict['fluid_negative'] = mappers_settings[mapper_id]["fluid_interface_submodelpart_name"].GetString()
+                else:
+                    err_msg = "The mapper face is not \'Positve\' nor \'Negative\'."
+                    raise Exception(err_msg)
+        else:
+            err_msg = "Case with more than 2 mappers has not been implemented yet.\n"
+            err_msg += "Please, in case you are using single faced immersed bodies, set the skin entities in a unique submodelpart.\n"
+            err_msg += "In case you are considering double faced immersed bodies (shells or membranes), set all the positive faces in a unique submodelpart and all the negative ones in another submodelpart."
+            raise Exception(err_msg)
+
+        ## Construct the structure solver
+        self.structure_solver = python_solvers_wrapper_structural.CreateSolverByParameters(self.model, self.settings["structure_solver_settings"], self.parallel_type)
+        KratosMultiphysics.Logger.PrintInfo("PartitionedFSIBaseSolver", "Structure solver construction finished.")
+
+        ## Construct the fluid solver
+        self.fluid_solver = python_solvers_wrapper_fluid.CreateSolverByParameters(self.model, self.settings["fluid_solver_settings"], self.parallel_type)
+        KratosMultiphysics.Logger.PrintInfo("PartitionedFSIBaseSolver", "Fluid solver construction finished.")
+
+        ## Check the ALE settings before the mesh solver construction
+        mesh_solver_settings = self.settings["mesh_solver_settings"]
+        fluid_solver_settings = self.settings["fluid_solver_settings"]
+
+        # Check that the ALE and the fluid are the same model part
+        fluid_model_part_name =  fluid_solver_settings["model_part_name"].GetString()
+        if mesh_solver_settings.Has("model_part_name"):
+            if not fluid_model_part_name == mesh_solver_settings["model_part_name"].GetString():
+                err_msg =  'Fluid and mesh solver have to use the same MainModelPart ("model_part_name")!\n'
+                raise Exception(err_msg)
+        else:
+            mesh_solver_settings.AddValue("model_part_name", fluid_solver_settings["model_part_name"])
+
+        # Ensure that the fluid domain is not imported twice
+        if mesh_solver_settings.Has("model_import_settings"):
+            if mesh_solver_settings["model_import_settings"].Has("input_type"):
+                if not mesh_solver_settings["model_import_settings"]["input_type"].GetString() == "use_input_model_part":
+                    mesh_solver_settings["model_import_settings"]["input_type"].SetString("use_input_model_part")
+            else:
+                mesh_solver_settings["model_import_settings"].AddEmptyValue("input_type").SetString("use_input_model_part")
+        else:
+            mesh_solver_settings.AddEmptyValue("model_import_settings").AddEmptyValue("input_type").SetString("use_input_model_part")
+
+        # Check that the ALE and the fluid have the sime time scheme
+        if fluid_solver_settings.Has("time_scheme"):
+            fluid_time_scheme =  fluid_solver_settings["time_scheme"].GetString()
+            if mesh_solver_settings.Has("mesh_velocity_calculation"):
+                if mesh_solver_settings["mesh_velocity_calculation"].Has("time_scheme"):
+                    if not fluid_time_scheme == mesh_solver_settings["mesh_velocity_calculation"]["time_scheme"].GetString():
+                        err_msg = 'Fluid and mesh solver require to use the same time scheme ("time_scheme") for consistency!\n'
+                        raise Exception(err_msg)
+                else:
+                    mesh_solver_settings["mesh_velocity_calculation"].AddValue("time_scheme", fluid_solver_settings["time_scheme"])
+            else:
+                mesh_solver_settings.AddEmptyValue("mesh_velocity_calculation")
+                mesh_solver_settings["mesh_velocity_calculation"].AddValue("time_scheme", fluid_solver_settings["time_scheme"])
+
+        # Check domain size
+        fluid_domain_size = fluid_solver_settings["domain_size"].GetInt()
+        if mesh_solver_settings.Has("domain_size"):
+            if not fluid_domain_size == mesh_solver_settings["domain_size"].GetInt():
+                raise Exception('Fluid and mesh solver have different "domain_size"!')
+        else:
+            mesh_solver_settings.AddValue("domain_size", fluid_solver_settings["domain_size"])
+
+        # Ensure that the MESH_VELOCITY is computed
+        if mesh_solver_settings.Has("calculate_mesh_velocity"):
+            if not mesh_solver_settings["calculate_mesh_velocity"].GetBool():
+                mesh_solver_settings.SetValue("calculate_mesh_velocity", True)
+                KratosMultiphysics.Logger.PrintWarning("","Mesh velocity calculation was deactivated. Switching \"calculate_mesh_velocity\" on")
+        else:
+            mesh_solver_settings.AddEmptyValue("calculate_mesh_velocity").SetBool(True)
+
+        ## Construct the ALE mesh solver
+        self.mesh_solver = python_solvers_wrapper_mesh_motion.CreateSolverByParameters(self.model, self.settings["mesh_solver_settings"], self.parallel_type)
+        KratosMultiphysics.Logger.PrintInfo("PartitionedFSIBaseSolver", "ALE mesh solver construction finished.")
+
+    def _AdvanceInTimeCouplingInterfaces(self, new_time):
+        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart().CloneTimeStep(new_time)
+        self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.STEP] = self._GetFSICouplingInterfaceStructure().GetFatherModelPart().ProcessInfo[KratosMultiphysics.STEP]
+        self._GetFSICouplingInterfaceFluidPositive().GetInterfaceModelPart().CloneTimeStep(new_time)
+        self._GetFSICouplingInterfaceFluidPositive().GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.STEP] = self._GetFSICouplingInterfaceFluidPositive().GetFatherModelPart().ProcessInfo[KratosMultiphysics.STEP]
+        if self.double_faced_structure:
+            self._GetFSICouplingInterfaceFluidNegative().GetInterfaceModelPart().CloneTimeStep(new_time)
+            self._GetFSICouplingInterfaceFluidNegative().GetInterfaceModelPart().ProcessInfo[KratosMultiphysics.STEP] = self._GetFSICouplingInterfaceFluidNegative().GetFatherModelPart().ProcessInfo[KratosMultiphysics.STEP]
+
+    # This method finds the maximum buffer size between mesh,
+    # fluid and structure solvers and sets it to all the solvers.
+    def _GetAndSetMinimumBufferSize(self):
+        fluid_buffer_size = self.fluid_solver.min_buffer_size
+        mesh_buffer_size = self.mesh_solver.settings["buffer_size"].GetInt()
+        str_buffer_size = self.structure_solver.settings["buffer_size"].GetInt()
+
+        buffer_size = max(fluid_buffer_size, mesh_buffer_size)
+        buffer_size = max(buffer_size, str_buffer_size)
+
+        self.fluid_solver.min_buffer_size = buffer_size
+        self.mesh_solver.settings["buffer_size"].SetInt(buffer_size)
+        self.structure_solver.settings["buffer_size"].SetInt(buffer_size)
+
+    #TODO: SHOULDN'T BE NEEDED AS WE ALWAYS USE THE POSITIVE ONE
+    # def _GetFluidInterfaceSubmodelPart(self):
+    #     # Returns the fluid interface submodelpart that will be used in the residual minimization
+    #     return self.fluid_solver.main_model_part.GetSubModelPart(self.fluid_interface_submodelpart_name)
+
+    def _InitializeCouplingInterfaces(self):
+        # Prepare the Dirichlet fluid interfaces
+        self.__SetFluidInterfaceFixity(self._GetFluidPositiveInterfaceSubmodelPart())
+        KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self._GetFluidPositiveInterfaceSubmodelPart().Nodes)
+        if self.double_faced_structure:
+            self.__SetFluidInterfaceFixity(self._GetFluidNegativeInterfaceSubmodelPart())
+            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self._GetFluidNegativeInterfaceSubmodelPart().Nodes)
+
+        # Prepare the Neumann structure interface
+        self._SetStructureNeumannCondition()
+        KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self._GetStructureInterfaceSubmodelPart().Nodes)
+
+    def __SetFluidInterfaceFixity(self, fluid_interface_submodelpart):
+        # Fix the VELOCITY, MESH_DISPLACEMENT and MESH_VELOCITY variables in all the fluid interface submodelparts
+        KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.VELOCITY_X, True, fluid_interface_submodelpart.Nodes)
+        KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.VELOCITY_Y, True, fluid_interface_submodelpart.Nodes)
+        KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.MESH_DISPLACEMENT_X, True, fluid_interface_submodelpart.Nodes)
+        KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.MESH_DISPLACEMENT_Y, True, fluid_interface_submodelpart.Nodes)
+        if self._GetDomainSize() == 3:
+            KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.VELOCITY_Z, True, fluid_interface_submodelpart.Nodes)
+            KratosMultiphysics.VariableUtils().ApplyFixity(KratosMultiphysics.MESH_DISPLACEMENT_Z, True, fluid_interface_submodelpart.Nodes)
+
+    def _GetFluidPositiveInterfaceSubmodelPart(self):
+        # Returns the fluid positive interface submodelpart
+        positive_interface_name = self.interfaces_dict['fluid_positive']
+        return self.model.GetModelPart(positive_interface_name)
+
+    def _GetFluidNegativeInterfaceSubmodelPart(self):
+        negative_interface_name = self.interfaces_dict['fluid_negative']
+        return self.model.GetModelPart(negative_interface_name)
+
+    def _GetStructureInterfaceSubmodelPart(self):
+        # Returns the structure interface submodelpart that will be used in the residual minimization
+        return self.model.GetModelPart(self.__GetStructureInterfaceModelPartName())
+
+    def __GetStructureInterfaceModelPartName(self):
+        if not hasattr(self, '_structure_interface_submodelpart_name'):
+            str_int_list = self.settings["coupling_settings"]["structure_interfaces_list"]
+            if (str_int_list.size() != 1):
+                raise Exception("FSI structure skin must be contained in a unique model part")
+            self._structure_interface_submodelpart_name = str_int_list[0].GetString()
+        return self._structure_interface_submodelpart_name
+
+    def _GetDomainSize(self):
+        if not hasattr(self, '_domain_size'):
+            fluid_domain_size = self.fluid_solver.main_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
+            structure_domain_size = self.structure_solver.main_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
+            if fluid_domain_size !=structure_domain_size:
+                raise("ERROR: Solid domain size and fluid domain size are not equal!")
+            self._domain_size = fluid_domain_size
+        return self._domain_size
+
+    def  _ComputeDeltaTime(self):
+        fluid_time_step = self.fluid_solver._ComputeDeltaTime()
+        structure_time_step = self.structure_solver.ComputeDeltaTime()
+
+        if abs(fluid_time_step - structure_time_step) > 1e-12:
+            err_msg =  'Fluid time step is: ' + str(fluid_time_step) + '\n'
+            err_msg += 'Structure time step is: ' + str(structure_time_step) + '\n'
+            err_msg += 'No substepping has been implemented yet. Fluid and structure time step must coincide.'
+            raise Exception(err_msg)
+
+        return fluid_time_step
+
+    #TODO: THIS MUST BE DONE IN C++ (FSIPartitionedUtils)
+    #TODO: THINK ABOUT ASSUMING THESE TO BE ALREADY IN THE MPDA (AS THE EMBEDDED DOES) OR TO ALWAYS CREATE THEM (ALSO IN THE EMBEDDED)
+    def _SetStructureNeumannCondition(self):
+
+        structure_computational_submodelpart = self.structure_solver.GetComputingModelPart()
+
+        # Get the maximum condition id
+        max_cond_id = 0
+        for condition in self.structure_solver.main_model_part.Conditions:
+            max_cond_id = max(max_cond_id, condition.Id)
+
+        max_cond_id = self.structure_solver.main_model_part.GetCommunicator().GetDataCommunicator().MaxAll(max_cond_id)
+
+        # Set up the point load condition in the structure interface
+        structure_interfaces_list = self.settings["coupling_settings"]["structure_interfaces_list"]
+        for i in range(structure_interfaces_list.size()):
+            interface_submodelpart_name = structure_interfaces_list[i].GetString()
+            interface_submodelpart_i = self.model.GetModelPart(interface_submodelpart_name)
+
+            # Get the number of conditions to be set in each processor
+            local_nodes_number_accumulated = -1
+            local_nodes_number = len(interface_submodelpart_i.GetCommunicator().LocalMesh().Nodes)
+            local_nodes_number_accumulated = interface_submodelpart_i.GetCommunicator().GetDataCommunicator().ScanSum(local_nodes_number)
+
+            # Create the point load condition
+            aux_count = max_cond_id + local_nodes_number_accumulated
+            if self._GetDomainSize() == 2:
+                for node in interface_submodelpart_i.GetCommunicator().LocalMesh().Nodes:
+                    aux_count+=1
+                    structure_computational_submodelpart.CreateNewCondition("PointLoadCondition2D1N",
+                                                                            int(aux_count),
+                                                                            [node.Id],
+                                                                            self.structure_solver.main_model_part.Properties[0])
+            elif self._GetDomainSize() == 3:
+                for node in interface_submodelpart_i.GetCommunicator().LocalMesh().Nodes:
+                    aux_count+=1
+                    structure_computational_submodelpart.CreateNewCondition("PointLoadCondition3D1N",
+                                                                            int(aux_count),
+                                                                            [node.Id],
+                                                                            self.structure_solver.main_model_part.Properties[0])
+
+    def _GetStructureToFluidPositiveInterfaceMapper(self):
+        if not hasattr(self, '_structure_to_fluid_positive_interface_mapper'):
+            self._structure_to_fluid_positive_interface_mapper = self._CreateStructureToFluidInterfaceMapper(
+                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+                self._GetFSICouplingInterfaceFluidPositive().GetInterfaceModelPart())
+        return self._structure_to_fluid_positive_interface_mapper
+
+    def _GetStructureToFluidNegativeInterfaceMapper(self):
+        if not hasattr(self, '_structure_to_fluid_negative_interface_mapper'):
+            self._structure_to_fluid_negative_interface_mapper = self._CreateStructureToFluidInterfaceMapper(
+                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+                self._GetFSICouplingInterfaceFluidNegative().GetInterfaceModelPart())
+        return self._structure_to_fluid_negative_interface_mapper
+
+    @classmethod
+    def _CreateStructureToFluidInterfaceMapper(self, structure_interface, fluid_interface):
+        mapper_params = KratosMultiphysics.Parameters("""{
+            "mapper_type": "nearest_element",
+            "echo_level" : 0
+        }""")
+        structure_to_fluid_interface_mapper = KratosMapping.MapperFactory.CreateMapper(
+            structure_interface,
+            fluid_interface,
+            mapper_params)
+
+        return structure_to_fluid_interface_mapper
+
+    def _GetFSICouplingInterfaceStructure(self):
+        if not hasattr(self, '_fsi_coupling_interface_structure'):
+            self._fsi_coupling_interface_structure = self._CreateFSICouplingInterfaceStructure()
+        return self._fsi_coupling_interface_structure
+
+    def _CreateFSICouplingInterfaceStructure(self):
+        # Set auxiliary settings
+        aux_settings = KratosMultiphysics.Parameters(
+        """{
+            "model_part_name": "FSICouplingInterfaceStructure",
+            "parent_model_part_name": "",
+            "input_variable_list": ["SURFACE_LOAD"],
+            "output_variable_list": ["DISPLACEMENT"]
+        }""")
+        aux_settings["parent_model_part_name"].SetString(self.interfaces_dict['structure'])
+
+        # Get the convergence accelerator instance (note that it is created in this call)
+        convergence_accelerator = self._GetConvergenceAccelerator()
+
+        # Construct the FSI coupling interface
+        fsi_coupling_interface_structure = fsi_coupling_interface.FSICouplingInterface(
+            self.model,
+            aux_settings,
+            convergence_accelerator)
+
+        KratosMultiphysics.Logger.PrintInfo('PartitionedFSIBaseSolver', 'Structure FSI coupling interface created')
+
+        return fsi_coupling_interface_structure
+
+    @classmethod
+    def _GetFSICouplingInterfaceFluid(self):
+        err_msg = 'Body-fitted partitioned FSI solver does not implement the \'_GetFSICouplingInterfaceFluid\' method.\n'
+        err_msg += 'Use \'_GetFSICouplingInterfaceFluidPositive\' as well as \'_GetFSICouplingInterfaceFluidNegative\' if the structure is thin-walled.'
+        raise Exception(err_msg)
+
+    def _GetFSICouplingInterfaceFluidPositive(self):
+        if not hasattr(self, '_fsi_coupling_interface_fluid_positive'):
+            fluid_interface_side = 'fluid_positive'
+            self._fsi_coupling_interface_fluid_positive = self.__CreateFSICouplingInterfaceFluid(fluid_interface_side)
+        return self._fsi_coupling_interface_fluid_positive
+
+    def _GetFSICouplingInterfaceFluidNegative(self):
+        if not hasattr(self, '_fsi_coupling_interface_fluid_negative'):
+            fluid_interface_side = 'fluid_negative'
+            self._fsi_coupling_interface_fluid_negative = self.__CreateFSICouplingInterfaceFluid(fluid_interface_side)
+        return self._fsi_coupling_interface_fluid_negative
+
+    def __CreateFSICouplingInterfaceFluid(self, fluid_interface_side):
+        # Set auxiliary settings
+        aux_settings = KratosMultiphysics.Parameters(
+        """{
+            "model_part_name": "",
+            "parent_model_part_name": "",
+            "input_variable_list": ["MESH_DISPLACEMENT"],
+            "output_variable_list": []
+        }""")
+        aux_settings["model_part_name"].SetString("FSICouplingInterface{}".format(fluid_interface_side.capitalize()))
+        aux_settings["parent_model_part_name"].SetString(self.interfaces_dict[fluid_interface_side])
+        aux_settings["output_variable_list"].Append("{}_MAPPED_VECTOR_VARIABLE".format("POSITIVE" if fluid_interface_side == 'fluid_positive' else "NEGATIVE"))
+
+        # Construct the FSI coupling interface
+        # Note that no convergence accelerator is created in the fluid side
+        fsi_coupling_interface_fluid = fsi_coupling_interface.FSICouplingInterface(
+            self.model,
+            aux_settings)
+
+        KratosMultiphysics.Logger.PrintInfo('PartitionedFSIBaseSolver', 'Fluid {} FSI coupling interface created'.format(fluid_interface_side))
+
+        return fsi_coupling_interface_fluid
+
+    # This method returns the convergence accelerator.
+    # If it is not created yet, it calls the _CreateConvergenceAccelerator first
+    def _GetConvergenceAccelerator(self):
+        if not hasattr(self, '_convergence_accelerator'):
+            self._convergence_accelerator = self._CreateConvergenceAccelerator()
+        return self._convergence_accelerator
+
+    # This method constructs the convergence accelerator coupling utility
+    def _CreateConvergenceAccelerator(self):
+        convergence_accelerator = convergence_accelerator_factory.CreateConvergenceAccelerator(self.settings["coupling_settings"]["coupling_strategy_settings"])
+        KratosMultiphysics.Logger.PrintInfo('PartitionedFSIBaseSolver', 'Coupling strategy construction finished')
+        return convergence_accelerator
+
+    def _MapStructureInterfaceDisplacement(self):
+        # Map the RELAXED_DISPLACEMENT from the structure FSI coupling interface to fluid FSI coupling interface
+        self._GetStructureToFluidPositiveInterfaceMapper().Map(
+            KratosMultiphysics.RELAXED_DISPLACEMENT,
+            KratosMultiphysics.MESH_DISPLACEMENT)
+
+        # In case the structure is double faced, we take advantage of the equal positive and negative sides meshes
+        if self.double_faced_structure:
+            KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
+                KratosMultiphysics.MESH_DISPLACEMENT,
+                KratosMultiphysics.MESH_DISPLACEMENT,
+                self._GetFSICouplingInterfaceFluidPositive.GetInterfaceModelPart(),
+                self._GetFSICouplingInterfaceFluidNegative.GetInterfaceModelPart())
+
+        # Update the fluid interface position
+        self._GetFSICouplingInterfaceFluidPositive().UpdatePosition(KratosMultiphysics.MESH_DISPLACEMENT)
+        if self.double_faced_structure:
+            self._GetFSICouplingInterfaceFluidNegative().UpdatePosition(KratosMultiphysics.MESH_DISPLACEMENT)
+
+    def _SolveFluid(self):
+        # Transfer values from fluid FSI coupling interface to fluid skin
+        self._GetFSICouplingInterfaceFluidPositive().TransferValuesToFatherModelPart(KratosMultiphysics.MESH_DISPLACEMENT)
+        if self.double_faced_structure:
+            self._GetFSICouplingInterfaceFluidNegative().TransferValuesToFatherModelPart(KratosMultiphysics.MESH_DISPLACEMENT)
+
+        # Solve the mesh problem (or moves the interface nodes)
+        if self.solve_mesh_at_each_iteration:
+            self.mesh_solver.SolveSolutionStep()
+        else:
+            self.mesh_solver.MoveMesh()
+
+        # Impose the structure MESH_VELOCITY in the fluid interface VELOCITY (Lagrangian interface)
+        KratosMultiphysics.VariableUtils().CopyVariable(
+                KratosMultiphysics.MESH_VELOCITY,
+                KratosMultiphysics.VELOCITY,
+                self._GetFluidPositiveInterfaceSubmodelPart().GetCommunicator().LocalMesh().Nodes)
+        self._GetFluidPositiveInterfaceSubmodelPart().GetCommunicator().SynchronizeVariable(KratosMultiphysics.VELOCITY)
+        if self.double_faced_structure:
+            KratosMultiphysics.VariableUtils().CopyVariable(
+                    KratosMultiphysics.MESH_VELOCITY,
+                    KratosMultiphysics.VELOCITY,
+                    self._GetFluidNegativeInterfaceSubmodelPart().GetCommunicator().LocalMesh().Nodes)
+            self._GetFluidNegativeInterfaceSubmodelPart().GetCommunicator().SynchronizeVariable(KratosMultiphysics.VELOCITY)
+
+        # Solve fluid problem
+        self.fluid_solver.SolveSolutionStep()
+
+    def _CalculateFluidInterfaceTraction(self):
+        # Distribute the REACTION point load
+        distribution_tolerance = 1.0e-12
+        distribution_max_iterations = 500
+
+        KratosMultiphysics.VariableRedistributionUtility.DistributePointValues(
+            self._GetFluidPositiveInterfaceSubmodelPart(),
+            self._GetFluidPositiveInterfaceSubmodelPart().Conditions,
+            KratosMultiphysics.REACTION,
+            KratosMultiphysics.POSITIVE_MAPPED_VECTOR_VARIABLE,
+            distribution_tolerance,
+            distribution_max_iterations)
+        if self.double_faced_structure:
+            KratosMultiphysics.VariableRedistributionUtility.DistributePointValues(
+                self._GetFluidNegativeInterfaceSubmodelPart(),
+                self._GetFluidNegativeInterfaceSubmodelPart().Conditions,
+                KratosMultiphysics.REACTION,
+                KratosMultiphysics.NEGATIVE_MAPPED_VECTOR_VARIABLE,
+                distribution_tolerance,
+                distribution_max_iterations)
+
+        # Transfer traction values from fluid interface to fluid FSI coupling interface
+        # NOTE: POSITIVE_MAPPED_VECTOR_VARIABLE is the positive side traction
+        # NOTE: NEGATIVE_MAPPED_VECTOR_VARIABLE is the negative side traction
+        self._GetFSICouplingInterfaceFluidPositive().GetValuesFromFatherModelPart(KratosMultiphysics.POSITIVE_MAPPED_VECTOR_VARIABLE)
+        if self.double_faced_structure:
+            self._GetFSICouplingInterfaceFluidNegative().GetValuesFromFatherModelPart(KratosMultiphysics.NEGATIVE_MAPPED_VECTOR_VARIABLE)
+
+    def _MapFluidInterfaceTraction(self):
+        # Map the distributed REACTION from the fluid FSI coupling interface to structure FSI coupling interface
+        self._GetStructureToFluidPositiveInterfaceMapper().InverseMap(
+            self._GetTractionVariable(),
+            KratosMultiphysics.POSITIVE_MAPPED_VECTOR_VARIABLE,
+            KratosMultiphysics.Mapper.SWAP_SIGN)
+        if self.double_faced_structure:
+            self._GetStructureToFluidNegativeInterfaceMapper().InverseMap(
+                self._GetTractionVariable(),
+                KratosMultiphysics.NEGATIVE_MAPPED_VECTOR_VARIABLE,
+                KratosMultiphysics.Mapper.ADD_VALUES | KratosMultiphysics.Mapper.SWAP_SIGN)
+
+        # Send the mapped load from the structure FSI coupling interface to the parent one
+        self._GetFSICouplingInterfaceStructure().TransferValuesToFatherModelPart(self._GetTractionVariable())
+
+    def _SolveStructure(self):
+        #TODO: Once we use the distributed (relaxed) traction in the body fitted we can remove this as well as the _SolveStructure in the embedded solver
+        # Convert distributed traction to point values
+        KratosMultiphysics.VariableRedistributionUtility.ConvertDistributedValuesToPoint(
+            self._GetStructureInterfaceSubmodelPart(),
+            self._GetStructureInterfaceSubmodelPart().Conditions,
+            self._GetTractionVariable(),
+            KratosStructural.POINT_LOAD)
+
+        # Solve the structure problem
+        self.structure_solver.SolveSolutionStep()
+
+    def _ComputeInitialResidual(self):
+        # Save as RELAXED_DISPLACEMENT the DISPLACEMENT coming from the structure Predict()
+        # Note that this would be required in order to set the first observation matrices
+        KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
+            KratosMultiphysics.DISPLACEMENT,
+            KratosMultiphysics.RELAXED_DISPLACEMENT,
+            self._GetStructureInterfaceSubmodelPart(),
+            self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+            0)
+
+        # Update the structure interface position with the DISPLACEMENT values from the predict
+        self._GetFSICouplingInterfaceStructure().UpdatePosition(KratosMultiphysics.RELAXED_DISPLACEMENT)
+
+        # Map the relaxed displacement from the structure coupling interface to the fluid one
+        self._MapStructureInterfaceDisplacement()
+
+        # Solve the mesh and fluid problem
+        self._SolveFluid()
+
+        # Calculate the fluid interface traction from the interface reaction
+        #TODO: THINK ABOUT COMPUTING THE SUM OF NEGATIVE AND POSITIVE DISTRIBUTED LOAD AND TRANSFER THIS TO THE STRUCTURE (INSTEAD OF PASSING POSITIVE AND NEGATIVE)
+        self._CalculateFluidInterfaceTraction()
+
+        # Transfer the fluid traction to the structure interface
+        self._MapFluidInterfaceTraction()
+
+        # Save as RELAXED_TRATION the TRACTION coming from the fluid
+        # Note that this would be required in order to set the first observation matrices
+        if self._GetConvergenceAccelerator().IsBlockNewton():
+            KratosMultiphysics.VariableUtils().CopyModelPartNodalVar(
+                self._GetTractionVariable(),
+                KratosMultiphysics.RELAXED_TRACTION,
+                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+                self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+                0)
+
+        # Directly send the map load from the structure FSI coupling interface to the parent one
+        self._GetFSICouplingInterfaceStructure().TransferValuesToFatherModelPart(self._GetTractionVariable())
+
+        # Solve the structure problem
+        self._SolveStructure()
+
+        # Compute the residual vector
+        dis_residual_norm = self._GetFSICouplingInterfaceStructure().ComputeResidualVector()
+
+        return dis_residual_norm
+
+    def _CheckFSIConvergence(self, nl_it, residual_norm):
+        interface_dofs = self._GetPartitionedFSIUtilities().GetInterfaceResidualSize(self._GetStructureInterfaceSubmodelPart())
+        normalised_residual = residual_norm/sqrt(interface_dofs)
+        KratosMultiphysics.Logger.PrintInfo('PartitionedFSIBaseSolver', 'FSI non-linear iteration = {0} |res|/sqrt(nDOFS) = {1}'.format(nl_it, normalised_residual))
+        return normalised_residual < self.nl_tol
+
+    def _GetPartitionedFSIUtilities(self):
+        if not hasattr(self, '_partitioned_fsi_utilities'):
+            self._partitioned_fsi_utilities = self._CreatePartitionedFSIUtilities()
+        return self._partitioned_fsi_utilities
+
+    def _CreatePartitionedFSIUtilities(self):
+        if self._GetDomainSize() == 2:
+            return KratosFSI.PartitionedFSIUtilitiesArray2D()
+        elif self._GetDomainSize() == 3:
+            return KratosFSI.PartitionedFSIUtilitiesArray3D()
+        else:
+            raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
+
+    @classmethod
+    def _GetTractionVariable(self):
+        #NOTE: No distinction is made between LINE_LOAD and SURFACE_LOAD as this is only used for the redistribution
+        #NOTE: Hence, this has only an auxiliary use as the traction will be converted to point load prior to the structure solve
+        #TODO: Use LINE_LOAD in 2D and SURFACE_LOAD in 3D when using distributed loads conditions
+        return KratosStructural.SURFACE_LOAD
```

## KratosMultiphysics/FSIApplication/python_solvers_wrapper_fsi.py

 * *Ordering differences only*

```diff
@@ -1,64 +1,64 @@
-
-import KratosMultiphysics
-from importlib import import_module
-
-def CreateSolverByParameters(model, solver_settings, parallelism):
-
-    if (type(model) != KratosMultiphysics.Model):
-        raise Exception("input is expected to be provided as a Kratos Model object")
-
-    if (type(solver_settings) != KratosMultiphysics.Parameters):
-        raise Exception("input is expected to be provided as a Kratos Parameters object")
-
-    solver_type = solver_settings["solver_type"].GetString()
-    coupling_scheme = solver_settings["coupling_scheme"].GetString()
-
-    # Solvers for OpenMP parallelism
-    if (parallelism == "OpenMP"):
-        if (solver_type == "Partitioned" or solver_type == "partitioned"):
-            if (coupling_scheme == "DirichletNeumann" or coupling_scheme == "dirichlet_neumann"):
-                solver_module_name = "partitioned_fsi_base_solver"
-            else:
-                err_msg = 'Requested coupling_scheme: ' + coupling_scheme + ' is not available.'
-                raise Exception(err_msg)
-        elif (solver_type == "PartitionedEmbedded" or solver_type == "partitioned_embedded"):
-            if (coupling_scheme == "DirichletNeumann" or coupling_scheme == "dirichlet_neumann"):
-                solver_module_name = "partitioned_embedded_fsi_base_solver"
-            else:
-                err_msg = 'Requested coupling_scheme: ' + coupling_scheme + ' is not available.'
-                raise Exception(err_msg)
-        else:
-            err_msg = 'Requested solver_type: ' + solver_type + ' is not available.'
-            raise Exception(err_msg)
-    # Solvers for MPI parallelism
-    elif (parallelism == "MPI"):
-        if (solver_type == "Partitioned" or solver_type == "partitioned"):
-            if (coupling_scheme == "DirichletNeumann" or coupling_scheme == "dirichlet_neumann"):
-                solver_module_name = "trilinos_partitioned_fsi_base_solver"
-            else:
-                err_msg = 'Requested coupling_scheme: ' + coupling_scheme + ' is not available.'
-                raise Exception(err_msg)
-        else:
-            err_msg = 'Requested solver_type: ' + solver_type + ' is not available.'
-            raise Exception(err_msg)
-    else:
-        err_msg = "Parallelism is neither OpenMP nor MPI."
-        raise Exception(err_msg)
-
-    module_full = 'KratosMultiphysics.FSIApplication.' + solver_module_name
-    solver = import_module(module_full).CreateSolver(model, solver_settings)
-
-    return solver
-
-def CreateSolver(model, custom_settings):
-
-    if (type(model) != KratosMultiphysics.Model):
-        raise Exception("input is expected to be provided as a Kratos Model object")
-
-    if (type(custom_settings) != KratosMultiphysics.Parameters):
-        raise Exception("input is expected to be provided as a Kratos Parameters object")
-
-    parallelism = custom_settings["problem_data"]["parallel_type"].GetString()
-    solver_settings = custom_settings["solver_settings"]
-
+
+import KratosMultiphysics
+from importlib import import_module
+
+def CreateSolverByParameters(model, solver_settings, parallelism):
+
+    if (type(model) != KratosMultiphysics.Model):
+        raise Exception("input is expected to be provided as a Kratos Model object")
+
+    if (type(solver_settings) != KratosMultiphysics.Parameters):
+        raise Exception("input is expected to be provided as a Kratos Parameters object")
+
+    solver_type = solver_settings["solver_type"].GetString()
+    coupling_scheme = solver_settings["coupling_scheme"].GetString()
+
+    # Solvers for OpenMP parallelism
+    if (parallelism == "OpenMP"):
+        if (solver_type == "Partitioned" or solver_type == "partitioned"):
+            if (coupling_scheme == "DirichletNeumann" or coupling_scheme == "dirichlet_neumann"):
+                solver_module_name = "partitioned_fsi_base_solver"
+            else:
+                err_msg = 'Requested coupling_scheme: ' + coupling_scheme + ' is not available.'
+                raise Exception(err_msg)
+        elif (solver_type == "PartitionedEmbedded" or solver_type == "partitioned_embedded"):
+            if (coupling_scheme == "DirichletNeumann" or coupling_scheme == "dirichlet_neumann"):
+                solver_module_name = "partitioned_embedded_fsi_base_solver"
+            else:
+                err_msg = 'Requested coupling_scheme: ' + coupling_scheme + ' is not available.'
+                raise Exception(err_msg)
+        else:
+            err_msg = 'Requested solver_type: ' + solver_type + ' is not available.'
+            raise Exception(err_msg)
+    # Solvers for MPI parallelism
+    elif (parallelism == "MPI"):
+        if (solver_type == "Partitioned" or solver_type == "partitioned"):
+            if (coupling_scheme == "DirichletNeumann" or coupling_scheme == "dirichlet_neumann"):
+                solver_module_name = "trilinos_partitioned_fsi_base_solver"
+            else:
+                err_msg = 'Requested coupling_scheme: ' + coupling_scheme + ' is not available.'
+                raise Exception(err_msg)
+        else:
+            err_msg = 'Requested solver_type: ' + solver_type + ' is not available.'
+            raise Exception(err_msg)
+    else:
+        err_msg = "Parallelism is neither OpenMP nor MPI."
+        raise Exception(err_msg)
+
+    module_full = 'KratosMultiphysics.FSIApplication.' + solver_module_name
+    solver = import_module(module_full).CreateSolver(model, solver_settings)
+
+    return solver
+
+def CreateSolver(model, custom_settings):
+
+    if (type(model) != KratosMultiphysics.Model):
+        raise Exception("input is expected to be provided as a Kratos Model object")
+
+    if (type(custom_settings) != KratosMultiphysics.Parameters):
+        raise Exception("input is expected to be provided as a Kratos Parameters object")
+
+    parallelism = custom_settings["problem_data"]["parallel_type"].GetString()
+    solver_settings = custom_settings["solver_settings"]
+
     return CreateSolverByParameters(model, solver_settings, parallelism)
```

## KratosMultiphysics/FSIApplication/trilinos_partitioned_fsi_base_solver.py

 * *Ordering differences only*

```diff
@@ -1,101 +1,101 @@
-
-# Import utilities
-from KratosMultiphysics.FSIApplication import convergence_accelerator_factory         # Import the FSI convergence accelerator factory
-from KratosMultiphysics.FSIApplication import fsi_coupling_interface
-
-# Importing the Kratos Library
-import KratosMultiphysics
-import KratosMultiphysics.mpi as KratosMPI
-
-# Import applications
-import KratosMultiphysics.TrilinosApplication as KratosTrilinos
-import KratosMultiphysics.MappingApplication as KratosMapping
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-
-# Import base class file
-from KratosMultiphysics.FSIApplication import partitioned_fsi_base_solver
-
-def CreateSolver(model, project_parameters):
-    return TrilinosPartitionedFSIBaseSolver(model, project_parameters)
-
-class TrilinosPartitionedFSIBaseSolver(partitioned_fsi_base_solver.PartitionedFSIBaseSolver):
-    def __init__(self, model, project_parameters):
-        super(TrilinosPartitionedFSIBaseSolver, self).__init__(model, project_parameters)
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        """This function returns the default-settings used by this class
-        """
-        this_defaults = KratosMultiphysics.Parameters("""{
-            "parallel_type": "MPI"
-        }""")
-        this_defaults.AddMissingParameters(super().GetDefaultParameters())
-        return this_defaults
-
-    def _GetEpetraCommunicator(self):
-        if not hasattr(self, '_epetra_communicator'):
-            self._epetra_communicator = self._CreateEpetraCommunicator()
-        return self._epetra_communicator
-
-    def _CreateEpetraCommunicator(self):
-        return KratosTrilinos.CreateCommunicator()
-
-    def _CreateConvergenceAccelerator(self):
-        """ Create the MPI parallel convergence accelerator and assign it to the structure FSI coupling interface"""
-        # Create the MPI parallel convergence accelerator
-        convergence_accelerator = convergence_accelerator_factory.CreateTrilinosConvergenceAccelerator(
-            self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
-            self._GetEpetraCommunicator(),
-            self.settings["coupling_settings"]["coupling_strategy_settings"])
-        # Assign the new convergence accelerator to the structure FSI coupling interface
-        self._GetFSICouplingInterfaceStructure().SetConvergenceAccelerator(convergence_accelerator)
-        KratosMultiphysics.Logger.PrintInfo('TrilinosPartitionedFSIBaseSolver', 'Coupling strategy construction finished.')
-        return convergence_accelerator
-
-    def _CreateFSICouplingInterfaceStructure(self):
-        """Create the structure FSI coupling interface
-
-        Create the structure FSI coupling interface with a default MPI convergence accelerator
-        The final convergence accelerator will be assigned to the structure FSI coupling interface in the _CreateConvergenceAccelerator
-        This is required since the MPI parallel convergence accelerators require the residual minimization model part to be instantiated
-        """
-        # Set auxiliary settings
-        aux_settings = KratosMultiphysics.Parameters(
-        """{
-            "model_part_name": "FSICouplingInterfaceStructure",
-            "parent_model_part_name": "",
-            "input_variable_list": ["SURFACE_LOAD"],
-            "output_variable_list": ["DISPLACEMENT"]
-        }""")
-        aux_settings["parent_model_part_name"].SetString(self.interfaces_dict['structure'])
-
-        # Construct the FSI coupling interface
-        fsi_coupling_interface_structure = fsi_coupling_interface.FSICouplingInterface(
-            self.model,
-            aux_settings,
-            KratosTrilinos.TrilinosConvergenceAccelerator())
-
-        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Structure FSI coupling interface created')
-
-        return fsi_coupling_interface_structure
-
-    def _CreatePartitionedFSIUtilities(self):
-        if self._GetDomainSize() == 2:
-            return KratosTrilinos.TrilinosPartitionedFSIUtilitiesArray2D(self._GetEpetraCommunicator())
-        elif self._GetDomainSize() == 3:
-            return KratosTrilinos.TrilinosPartitionedFSIUtilitiesArray3D(self._GetEpetraCommunicator())
-        else:
-            raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
-
-    @classmethod
-    def _CreateStructureToFluidInterfaceMapper(self, structure_interface, fluid_interface):
-        mapper_params = KratosMultiphysics.Parameters("""{
-            "mapper_type": "nearest_element",
-            "echo_level" : 0
-        }""")
-        structure_to_fluid_interface_mapper = KratosMapping.MapperFactory.CreateMPIMapper(
-            structure_interface,
-            fluid_interface,
-            mapper_params)
-
-        return structure_to_fluid_interface_mapper
+
+# Import utilities
+from KratosMultiphysics.FSIApplication import convergence_accelerator_factory         # Import the FSI convergence accelerator factory
+from KratosMultiphysics.FSIApplication import fsi_coupling_interface
+
+# Importing the Kratos Library
+import KratosMultiphysics
+import KratosMultiphysics.mpi as KratosMPI
+
+# Import applications
+import KratosMultiphysics.TrilinosApplication as KratosTrilinos
+import KratosMultiphysics.MappingApplication as KratosMapping
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+
+# Import base class file
+from KratosMultiphysics.FSIApplication import partitioned_fsi_base_solver
+
+def CreateSolver(model, project_parameters):
+    return TrilinosPartitionedFSIBaseSolver(model, project_parameters)
+
+class TrilinosPartitionedFSIBaseSolver(partitioned_fsi_base_solver.PartitionedFSIBaseSolver):
+    def __init__(self, model, project_parameters):
+        super(TrilinosPartitionedFSIBaseSolver, self).__init__(model, project_parameters)
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        """This function returns the default-settings used by this class
+        """
+        this_defaults = KratosMultiphysics.Parameters("""{
+            "parallel_type": "MPI"
+        }""")
+        this_defaults.AddMissingParameters(super().GetDefaultParameters())
+        return this_defaults
+
+    def _GetEpetraCommunicator(self):
+        if not hasattr(self, '_epetra_communicator'):
+            self._epetra_communicator = self._CreateEpetraCommunicator()
+        return self._epetra_communicator
+
+    def _CreateEpetraCommunicator(self):
+        return KratosTrilinos.CreateCommunicator()
+
+    def _CreateConvergenceAccelerator(self):
+        """ Create the MPI parallel convergence accelerator and assign it to the structure FSI coupling interface"""
+        # Create the MPI parallel convergence accelerator
+        convergence_accelerator = convergence_accelerator_factory.CreateTrilinosConvergenceAccelerator(
+            self._GetFSICouplingInterfaceStructure().GetInterfaceModelPart(),
+            self._GetEpetraCommunicator(),
+            self.settings["coupling_settings"]["coupling_strategy_settings"])
+        # Assign the new convergence accelerator to the structure FSI coupling interface
+        self._GetFSICouplingInterfaceStructure().SetConvergenceAccelerator(convergence_accelerator)
+        KratosMultiphysics.Logger.PrintInfo('TrilinosPartitionedFSIBaseSolver', 'Coupling strategy construction finished.')
+        return convergence_accelerator
+
+    def _CreateFSICouplingInterfaceStructure(self):
+        """Create the structure FSI coupling interface
+
+        Create the structure FSI coupling interface with a default MPI convergence accelerator
+        The final convergence accelerator will be assigned to the structure FSI coupling interface in the _CreateConvergenceAccelerator
+        This is required since the MPI parallel convergence accelerators require the residual minimization model part to be instantiated
+        """
+        # Set auxiliary settings
+        aux_settings = KratosMultiphysics.Parameters(
+        """{
+            "model_part_name": "FSICouplingInterfaceStructure",
+            "parent_model_part_name": "",
+            "input_variable_list": ["SURFACE_LOAD"],
+            "output_variable_list": ["DISPLACEMENT"]
+        }""")
+        aux_settings["parent_model_part_name"].SetString(self.interfaces_dict['structure'])
+
+        # Construct the FSI coupling interface
+        fsi_coupling_interface_structure = fsi_coupling_interface.FSICouplingInterface(
+            self.model,
+            aux_settings,
+            KratosTrilinos.TrilinosConvergenceAccelerator())
+
+        KratosMultiphysics.Logger.PrintInfo('PartitionedEmbeddedFSIBaseSolver', 'Structure FSI coupling interface created')
+
+        return fsi_coupling_interface_structure
+
+    def _CreatePartitionedFSIUtilities(self):
+        if self._GetDomainSize() == 2:
+            return KratosTrilinos.TrilinosPartitionedFSIUtilitiesArray2D(self._GetEpetraCommunicator())
+        elif self._GetDomainSize() == 3:
+            return KratosTrilinos.TrilinosPartitionedFSIUtilitiesArray3D(self._GetEpetraCommunicator())
+        else:
+            raise Exception("Domain size expected to be 2 or 3. Got " + str(self._GetDomainSize()))
+
+    @classmethod
+    def _CreateStructureToFluidInterfaceMapper(self, structure_interface, fluid_interface):
+        mapper_params = KratosMultiphysics.Parameters("""{
+            "mapper_type": "nearest_element",
+            "echo_level" : 0
+        }""")
+        structure_to_fluid_interface_mapper = KratosMapping.MapperFactory.CreateMPIMapper(
+            structure_interface,
+            fluid_interface,
+            mapper_params)
+
+        return structure_to_fluid_interface_mapper
```

## Comparing `KratosFSIApplication-9.4.6.dist-info/METADATA` & `KratosFSIApplication-9.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: KratosFSIApplication
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
-Requires-Dist: KratosStructuralMechanicsApplication ==9.4.6
-Requires-Dist: KratosFluidDynamicsApplication ==9.4.6
-Requires-Dist: KratosMeshMovingApplication ==9.4.6
-Requires-Dist: KratosMappingApplication ==9.4.6
-
-## Fluid-Structure Interaction Application
-
-The Fluid-Structure Interaction Application contains the core developments in Fluid-Structure Interaction (FSI) within Kratos Multiphysics.
-
-### Features:
-
-- Partitioned relaxation and Quasi-Newton coupling schemes.
-
-- Support for MPI parallelization (with Trilinos Application).
-
-- Non-matching meshes support (see MappingApplication).
-
-- Laplacian and structural mesh solvers (see MeshMovingApplication).
+Metadata-Version: 2.1
+Name: KratosFSIApplication
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
+Requires-Dist: KratosStructuralMechanicsApplication ==9.5
+Requires-Dist: KratosFluidDynamicsApplication ==9.5
+Requires-Dist: KratosMeshMovingApplication ==9.5
+Requires-Dist: KratosMappingApplication ==9.5
+
+## Fluid-Structure Interaction Application
+
+The Fluid-Structure Interaction Application contains the core developments in Fluid-Structure Interaction (FSI) within Kratos Multiphysics.
+
+### Features:
+
+- Partitioned relaxation and Quasi-Newton coupling schemes.
+
+- Support for MPI parallelization (with Trilinos Application).
+
+- Non-matching meshes support (see MappingApplication).
+
+- Laplacian and structural mesh solvers (see MeshMovingApplication).
```

