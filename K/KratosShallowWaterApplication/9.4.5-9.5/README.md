# Comparing `tmp/KratosShallowWaterApplication-9.4.5-cp39-cp39-win_amd64.whl.zip` & `tmp/KratosShallowWaterApplication-9.5-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,1496 +1,2262 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   1080786 (0000000000107DD2h)
-  Actual end-cent-dir record offset:       1080764 (0000000000107DBCh)
-  Expected end-cent-dir record offset:     1080764 (0000000000107DBCh)
+  Zip archive file size:                   2896542 (00000000002C329Eh)
+  Actual end-cent-dir record offset:       2896520 (00000000002C3288h)
+  Expected end-cent-dir record offset:     2896520 (00000000002C3288h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 51 entries.
-  The central directory is 6138 (00000000000017FAh) bytes long,
+  central directory contains 61 entries.
+  The central directory is 8534 (0000000000002156h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 1074626 (00000000001065C2h).
+  is 2887986 (00000000002C1132h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosShallowWaterApplication.pyd
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
-  32-bit CRC value (hex):                         f2785a69
-  compressed size:                                361130 bytes
-  uncompressed size:                              1090560 bytes
-  length of filename:                             58 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
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
 
-  KratosMultiphysics/.libs/KratosShallowWaterCore.dll
+  KratosMultiphysics/ShallowWaterApplication/
 
-  offset of local header from start of archive:   361218
-                                                  (0000000000058302h) bytes
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
-  32-bit CRC value (hex):                         1c7e8fe5
-  compressed size:                                632622 bytes
-  uncompressed size:                              1899008 bytes
-  length of filename:                             51 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             43 characters
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
 
-  KratosMultiphysics/.libs/KratosShallowWaterCore.lib
+  KratosMultiphysics/ShallowWaterApplication/stabilized_shallow_water_solver.py
 
-  offset of local header from start of archive:   993921
-                                                  (00000000000F2A81h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   178
+                                                  (00000000000000B2h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         4fc39baa
-  compressed size:                                16845 bytes
-  uncompressed size:                              159124 bytes
-  length of filename:                             51 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         04e7c177
+  compressed size:                                1553 bytes
+  uncompressed size:                              5625 bytes
+  length of filename:                             77 characters
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
 
-  KratosMultiphysics/ShallowWaterApplication/__init__.py
+  KratosMultiphysics/ShallowWaterApplication/boussinesq_solver.py
 
-  offset of local header from start of archive:   1010847
-                                                  (00000000000F6C9Fh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1866
+                                                  (000000000000074Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         46821af3
-  compressed size:                                135 bytes
-  uncompressed size:                              289 bytes
-  length of filename:                             54 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         7642c6d3
+  compressed size:                                1182 bytes
+  uncompressed size:                              3817 bytes
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
 
 Central directory entry #5:
 ---------------------------
 
   KratosMultiphysics/ShallowWaterApplication/apply_absorbing_boundary_process.py
 
-  offset of local header from start of archive:   1011066
-                                                  (00000000000F6D7Ah) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3169
+                                                  (0000000000000C61h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         095836f6
-  compressed size:                                1020 bytes
-  uncompressed size:                              2957 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         0bc98c8e
+  compressed size:                                1007 bytes
+  uncompressed size:                              2894 bytes
   length of filename:                             78 characters
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
 
-  KratosMultiphysics/ShallowWaterApplication/apply_slip_process.py
+  KratosMultiphysics/ShallowWaterApplication/coupling/
 
-  offset of local header from start of archive:   1012194
-                                                  (00000000000F71E2h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         f1d4e598
-  compressed size:                                670 bytes
-  uncompressed size:                              1550 bytes
-  length of filename:                             64 characters
-  length of extra field:                          0 bytes
+  offset of local header from start of archive:   4312
+                                                  (00000000000010D8h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             52 characters
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
 
-  KratosMultiphysics/ShallowWaterApplication/automatic_dirichlet_conditions_process.py
+  KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_output_process.py
 
-  offset of local header from start of archive:   1012958
-                                                  (00000000000F74DEh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   4422
+                                                  (0000000000001146h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         d4cb9c3f
-  compressed size:                                1621 bytes
-  uncompressed size:                              6228 bytes
-  length of filename:                             84 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         ce2a2bf0
+  compressed size:                                1619 bytes
+  uncompressed size:                              6960 bytes
+  length of filename:                             87 characters
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
 
-  KratosMultiphysics/ShallowWaterApplication/boussinesq_solver.py
+  KratosMultiphysics/ShallowWaterApplication/coupling/write_from_sw_at_interface_process.py
 
-  offset of local header from start of archive:   1014693
-                                                  (00000000000F7BA5h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   6186
+                                                  (000000000000182Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         3f32fe85
-  compressed size:                                1193 bytes
-  uncompressed size:                              3886 bytes
-  length of filename:                             63 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         6bb3d360
+  compressed size:                                1218 bytes
+  uncompressed size:                              4253 bytes
+  length of filename:                             89 characters
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
 
-  KratosMultiphysics/ShallowWaterApplication/derivatives_recovery_process.py
+  KratosMultiphysics/ShallowWaterApplication/coupling/compute_boundary_force_process.py
 
-  offset of local header from start of archive:   1015979
-                                                  (00000000000F80ABh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   7551
+                                                  (0000000000001D7Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         19078257
-  compressed size:                                1381 bytes
-  uncompressed size:                              6332 bytes
-  length of filename:                             74 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         41d13499
+  compressed size:                                1622 bytes
+  uncompressed size:                              5350 bytes
+  length of filename:                             85 characters
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
 
-  KratosMultiphysics/ShallowWaterApplication/lagrangian_shallow_water_solver.py
+  KratosMultiphysics/ShallowWaterApplication/coupling/read_from_sw_interface_process.py
 
-  offset of local header from start of archive:   1017464
-                                                  (00000000000F8678h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   9316
+                                                  (0000000000002464h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         a8992880
-  compressed size:                                816 bytes
-  uncompressed size:                              2948 bytes
-  length of filename:                             77 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         89c0b6e3
+  compressed size:                                3435 bytes
+  uncompressed size:                              16112 bytes
+  length of filename:                             85 characters
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
 
-  KratosMultiphysics/ShallowWaterApplication/primitive_solver.py
+  KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_input_process.py
 
-  offset of local header from start of archive:   1018387
-                                                  (00000000000F8A13h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   12894
+                                                  (000000000000325Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         aa7c9569
-  compressed size:                                305 bytes
-  uncompressed size:                              654 bytes
-  length of filename:                             62 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         eb1b9382
+  compressed size:                                2705 bytes
+  uncompressed size:                              11460 bytes
+  length of filename:                             86 characters
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
 
-  KratosMultiphysics/ShallowWaterApplication/set_initial_perturbation_process.py
+  KratosMultiphysics/ShallowWaterApplication/wave_solver.py
 
-  offset of local header from start of archive:   1018784
-                                                  (00000000000F8BA0h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   15743
+                                                  (0000000000003D7Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         5b72adf6
-  compressed size:                                1032 bytes
-  uncompressed size:                              3403 bytes
-  length of filename:                             78 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         123e09ab
+  compressed size:                                1003 bytes
+  uncompressed size:                              3145 bytes
+  length of filename:                             57 characters
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
 
-  KratosMultiphysics/ShallowWaterApplication/set_initial_water_level_process.py
+  KratosMultiphysics/ShallowWaterApplication/shallow_water_base_solver.py
 
-  offset of local header from start of archive:   1019924
-                                                  (00000000000F9014h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   16861
+                                                  (00000000000041DDh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         4348ef19
-  compressed size:                                794 bytes
-  uncompressed size:                              2408 bytes
-  length of filename:                             77 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         c65808ce
+  compressed size:                                3195 bytes
+  uncompressed size:                              13397 bytes
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
 
 Central directory entry #14:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/set_topography_process.py
+  KratosMultiphysics/ShallowWaterApplication/automatic_dirichlet_conditions_process.py
 
-  offset of local header from start of archive:   1020825
-                                                  (00000000000F9399h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   20185
+                                                  (0000000000004ED9h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         26469dbc
-  compressed size:                                808 bytes
-  uncompressed size:                              2341 bytes
-  length of filename:                             68 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         9d51f165
+  compressed size:                                1607 bytes
+  uncompressed size:                              6111 bytes
+  length of filename:                             84 characters
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
 
-  KratosMultiphysics/ShallowWaterApplication/shallow_water_analysis.py
+  KratosMultiphysics/ShallowWaterApplication/utilities/
 
-  offset of local header from start of archive:   1021731
-                                                  (00000000000F9723h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   21934
+                                                  (00000000000055AEh) bytes
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
-  32-bit CRC value (hex):                         e03cb88d
-  compressed size:                                561 bytes
-  uncompressed size:                              1427 bytes
-  length of filename:                             68 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             53 characters
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
 
 Central directory entry #16:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/shallow_water_base_solver.py
+  KratosMultiphysics/ShallowWaterApplication/utilities/solitary_wave_utilities.py
 
-  offset of local header from start of archive:   1022390
-                                                  (00000000000F99B6h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   22045
+                                                  (000000000000561Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         52cf3b97
-  compressed size:                                3216 bytes
-  uncompressed size:                              13691 bytes
-  length of filename:                             71 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         ae312453
+  compressed size:                                1131 bytes
+  uncompressed size:                              4240 bytes
+  length of filename:                             79 characters
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
 
 Central directory entry #17:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/stabilized_shallow_water_solver.py
+  KratosMultiphysics/ShallowWaterApplication/utilities/wave_factory.py
 
-  offset of local header from start of archive:   1025707
-                                                  (00000000000FA6ABh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   23313
+                                                  (0000000000005B11h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         fe294023
-  compressed size:                                1563 bytes
-  uncompressed size:                              5736 bytes
-  length of filename:                             77 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         ac06c71d
+  compressed size:                                681 bytes
+  uncompressed size:                              2633 bytes
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
 
 Central directory entry #18:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/wave_generator_process.py
+  KratosMultiphysics/ShallowWaterApplication/utilities/wave_theory_utilities.py
 
-  offset of local header from start of archive:   1027377
-                                                  (00000000000FAD31h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   24120
+                                                  (0000000000005E38h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         e0353033
-  compressed size:                                1574 bytes
-  uncompressed size:                              5314 bytes
-  length of filename:                             68 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         d7216a13
+  compressed size:                                1040 bytes
+  uncompressed size:                              4580 bytes
+  length of filename:                             77 characters
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
 
 Central directory entry #19:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/wave_solver.py
+  KratosMultiphysics/ShallowWaterApplication/utilities/benchmarking_utilities.py
 
-  offset of local header from start of archive:   1029049
-                                                  (00000000000FB3B9h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   25295
+                                                  (00000000000062CFh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         c097d502
-  compressed size:                                1012 bytes
-  uncompressed size:                              3213 bytes
-  length of filename:                             57 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         62ab011b
+  compressed size:                                291 bytes
+  uncompressed size:                              855 bytes
+  length of filename:                             78 characters
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
 
 Central directory entry #20:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/benchmarks/base_benchmark_process.py
+  KratosMultiphysics/ShallowWaterApplication/postprocess/
 
-  offset of local header from start of archive:   1030148
-                                                  (00000000000FB804h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   25722
+                                                  (000000000000647Ah) bytes
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
-  32-bit CRC value (hex):                         db580899
-  compressed size:                                1404 bytes
-  uncompressed size:                              5492 bytes
-  length of filename:                             79 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             55 characters
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
 
 Central directory entry #21:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/benchmarks/dam_break_benchmark.py
+  KratosMultiphysics/ShallowWaterApplication/postprocess/offset_ids_process.py
 
-  offset of local header from start of archive:   1031661
-                                                  (00000000000FBDEDh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   25835
+                                                  (00000000000064EBh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         35b07874
-  compressed size:                                1345 bytes
-  uncompressed size:                              4131 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         bf72f1bb
+  compressed size:                                814 bytes
+  uncompressed size:                              2592 bytes
   length of filename:                             76 characters
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
 
 Central directory entry #22:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_shock_benchmark.py
+  KratosMultiphysics/ShallowWaterApplication/postprocess/generate_gid_list_file.py
 
-  offset of local header from start of archive:   1033112
-                                                  (00000000000FC398h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   26783
+                                                  (000000000000689Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         73fa8f74
-  compressed size:                                2400 bytes
-  uncompressed size:                              7983 bytes
-  length of filename:                             83 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         ddc6637e
+  compressed size:                                569 bytes
+  uncompressed size:                              1346 bytes
+  length of filename:                             80 characters
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
 
 Central directory entry #23:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_transition_benchmark.py
+  KratosMultiphysics/ShallowWaterApplication/postprocess/compute_froude_process.py
 
-  offset of local header from start of archive:   1035625
-                                                  (00000000000FCD69h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   27490
+                                                  (0000000000006B62h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         5bfe365b
-  compressed size:                                1254 bytes
-  uncompressed size:                              3137 bytes
-  length of filename:                             88 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         7c01b918
+  compressed size:                                589 bytes
+  uncompressed size:                              1501 bytes
+  length of filename:                             80 characters
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
 
 Central directory entry #24:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/benchmarks/planar_surface_in_parabola_benchmark.py
+  KratosMultiphysics/ShallowWaterApplication/postprocess/convergence_output_process.py
 
-  offset of local header from start of archive:   1036997
-                                                  (00000000000FD2C5h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   28217
+                                                  (0000000000006E39h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         9c80fd42
-  compressed size:                                1409 bytes
-  uncompressed size:                              4158 bytes
-  length of filename:                             93 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         c362416e
+  compressed size:                                1734 bytes
+  uncompressed size:                              6114 bytes
+  length of filename:                             84 characters
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
 
 Central directory entry #25:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/benchmarks/solitary_wave_benchmark.py
+  KratosMultiphysics/ShallowWaterApplication/postprocess/visualization_mesh_process.py
 
-  offset of local header from start of archive:   1038529
-                                                  (00000000000FD8C1h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   30093
+                                                  (000000000000758Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         107e719c
-  compressed size:                                1060 bytes
-  uncompressed size:                              3685 bytes
-  length of filename:                             80 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         e8ee5dd4
+  compressed size:                                2167 bytes
+  uncompressed size:                              9536 bytes
+  length of filename:                             84 characters
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
 
 Central directory entry #26:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/coupling/compute_boundary_force_process.py
+  KratosMultiphysics/ShallowWaterApplication/postprocess/line_envelope_output_process.py
 
-  offset of local header from start of archive:   1039699
-                                                  (00000000000FDD53h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   32402
+                                                  (0000000000007E92h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         41d13499
-  compressed size:                                1622 bytes
-  uncompressed size:                              5350 bytes
-  length of filename:                             85 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         5c4a8915
+  compressed size:                                948 bytes
+  uncompressed size:                              2608 bytes
+  length of filename:                             86 characters
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
 
 Central directory entry #27:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_input_process.py
+  KratosMultiphysics/ShallowWaterApplication/postprocess/auxiliary_nodes_visualization_process.py
 
-  offset of local header from start of archive:   1041436
-                                                  (00000000000FE41Ch) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   33494
+                                                  (00000000000082D6h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         a969a034
-  compressed size:                                2722 bytes
-  uncompressed size:                              11705 bytes
-  length of filename:                             86 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         c871d4e5
+  compressed size:                                1305 bytes
+  uncompressed size:                              4071 bytes
+  length of filename:                             95 characters
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
 
 Central directory entry #28:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_output_process.py
+  KratosMultiphysics/ShallowWaterApplication/postprocess/swap_coordinates_process.py
 
-  offset of local header from start of archive:   1044274
-                                                  (00000000000FEF32h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   34952
+                                                  (0000000000008888h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         9346753d
-  compressed size:                                1634 bytes
-  uncompressed size:                              7112 bytes
-  length of filename:                             87 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         686f0496
+  compressed size:                                682 bytes
+  uncompressed size:                              1864 bytes
+  length of filename:                             82 characters
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
 
 Central directory entry #29:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/coupling/read_from_sw_interface_process.py
+  KratosMultiphysics/ShallowWaterApplication/postprocess/line_graph_output_process.py
 
-  offset of local header from start of archive:   1046025
-                                                  (00000000000FF609h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   35774
+                                                  (0000000000008BBEh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         4a85d386
-  compressed size:                                3462 bytes
-  uncompressed size:                              16456 bytes
-  length of filename:                             85 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         0b5b5f37
+  compressed size:                                3308 bytes
+  uncompressed size:                              13473 bytes
+  length of filename:                             83 characters
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
 
 Central directory entry #30:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/coupling/write_from_sw_at_interface_process.py
+  KratosMultiphysics/ShallowWaterApplication/primitive_solver.py
 
-  offset of local header from start of archive:   1049602
-                                                  (0000000000100402h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   39223
+                                                  (0000000000009937h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         fe3371c0
-  compressed size:                                1227 bytes
-  uncompressed size:                              4329 bytes
-  length of filename:                             89 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         57ca07e6
+  compressed size:                                294 bytes
+  uncompressed size:                              636 bytes
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
 
 Central directory entry #31:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/modelers/dam_break_modeler.py
+  KratosMultiphysics/ShallowWaterApplication/testing/
 
-  offset of local header from start of archive:   1050948
-                                                  (0000000000100944h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         1f65f9ca
-  compressed size:                                275 bytes
-  uncompressed size:                              570 bytes
-  length of filename:                             72 characters
-  length of extra field:                          0 bytes
+  offset of local header from start of archive:   39637
+                                                  (0000000000009AD5h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             51 characters
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
 
 Central directory entry #32:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/modelers/planar_surface_in_parabola_modeler.py
+  KratosMultiphysics/ShallowWaterApplication/testing/empty_output_process.py
 
-  offset of local header from start of archive:   1051325
-                                                  (0000000000100ABDh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   39746
+                                                  (0000000000009B42h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         06476896
-  compressed size:                                292 bytes
-  uncompressed size:                              647 bytes
-  length of filename:                             89 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         1b56020f
+  compressed size:                                328 bytes
+  uncompressed size:                              640 bytes
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
 
 Central directory entry #33:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/postprocess/auxiliary_nodes_visualization_process.py
+  KratosMultiphysics/ShallowWaterApplication/testing/empty_solver_for_testing.py
 
-  offset of local header from start of archive:   1051736
-                                                  (0000000000100C58h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   40206
+                                                  (0000000000009D0Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         25151e48
-  compressed size:                                1316 bytes
-  uncompressed size:                              4164 bytes
-  length of filename:                             95 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         1d51fcb4
+  compressed size:                                985 bytes
+  uncompressed size:                              3585 bytes
+  length of filename:                             78 characters
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
 
 Central directory entry #34:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/postprocess/compute_froude_process.py
+  KratosMultiphysics/ShallowWaterApplication/wave_generator_process.py
 
-  offset of local header from start of archive:   1053177
-                                                  (00000000001011F9h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   41327
+                                                  (000000000000A16Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         a45edb33
-  compressed size:                                596 bytes
-  uncompressed size:                              1537 bytes
-  length of filename:                             80 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         16e6c3c6
+  compressed size:                                1561 bytes
+  uncompressed size:                              5195 bytes
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
 
 Central directory entry #35:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/postprocess/convergence_output_process.py
+  KratosMultiphysics/ShallowWaterApplication/benchmarks/
 
-  offset of local header from start of archive:   1053883
-                                                  (00000000001014BBh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         38100c0b
-  compressed size:                                1747 bytes
-  uncompressed size:                              6266 bytes
-  length of filename:                             84 characters
-  length of extra field:                          0 bytes
+  offset of local header from start of archive:   43014
+                                                  (000000000000A806h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             54 characters
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
 
 Central directory entry #36:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/postprocess/generate_gid_list_file.py
+  KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_shock_benchmark.py
 
-  offset of local header from start of archive:   1055744
-                                                  (0000000000101C00h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   43126
+                                                  (000000000000A876h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         a976a6d9
-  compressed size:                                576 bytes
-  uncompressed size:                              1384 bytes
-  length of filename:                             80 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         395cac19
+  compressed size:                                2382 bytes
+  uncompressed size:                              7773 bytes
+  length of filename:                             83 characters
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
 
 Central directory entry #37:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/postprocess/line_envelope_output_process.py
+  KratosMultiphysics/ShallowWaterApplication/benchmarks/base_benchmark_process.py
 
-  offset of local header from start of archive:   1056430
-                                                  (0000000000101EAEh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   45649
+                                                  (000000000000B251h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         f4d73d2a
-  compressed size:                                958 bytes
-  uncompressed size:                              2669 bytes
-  length of filename:                             86 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         95c43ea3
+  compressed size:                                1386 bytes
+  uncompressed size:                              5373 bytes
+  length of filename:                             79 characters
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
 
 Central directory entry #38:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/postprocess/line_graph_output_process.py
+  KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_transition_benchmark.py
 
-  offset of local header from start of archive:   1057504
-                                                  (00000000001022E0h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   47172
+                                                  (000000000000B844h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         060b49bc
-  compressed size:                                3322 bytes
-  uncompressed size:                              13777 bytes
-  length of filename:                             83 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         62dc12d8
+  compressed size:                                1242 bytes
+  uncompressed size:                              3058 bytes
+  length of filename:                             88 characters
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
 
 Central directory entry #39:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/postprocess/offset_ids_process.py
+  KratosMultiphysics/ShallowWaterApplication/benchmarks/dam_break_benchmark.py
 
-  offset of local header from start of archive:   1060939
-                                                  (000000000010304Bh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   48560
+                                                  (000000000000BDB0h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         4bcea161
-  compressed size:                                822 bytes
-  uncompressed size:                              2658 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         246e8fc5
+  compressed size:                                1332 bytes
+  uncompressed size:                              4003 bytes
   length of filename:                             76 characters
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
 
 Central directory entry #40:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/postprocess/swap_coordinates_process.py
+  KratosMultiphysics/ShallowWaterApplication/benchmarks/solitary_wave_benchmark.py
 
-  offset of local header from start of archive:   1061867
-                                                  (00000000001033EBh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   50026
+                                                  (000000000000C36Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         fd8254f6
-  compressed size:                                690 bytes
-  uncompressed size:                              1919 bytes
-  length of filename:                             82 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         eab82357
+  compressed size:                                1047 bytes
+  uncompressed size:                              3601 bytes
+  length of filename:                             80 characters
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
 
 Central directory entry #41:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/postprocess/visualization_mesh_process.py
+  KratosMultiphysics/ShallowWaterApplication/benchmarks/planar_surface_in_parabola_benchmark.py
 
-  offset of local header from start of archive:   1062669
-                                                  (000000000010370Dh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   51211
+                                                  (000000000000C80Bh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         b9928df7
-  compressed size:                                2183 bytes
-  uncompressed size:                              9747 bytes
-  length of filename:                             84 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         34633df2
+  compressed size:                                1396 bytes
+  uncompressed size:                              4042 bytes
+  length of filename:                             93 characters
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
 
 Central directory entry #42:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/testing/empty_output_process.py
+  KratosMultiphysics/ShallowWaterApplication/lagrangian_shallow_water_solver.py
 
-  offset of local header from start of archive:   1064966
-                                                  (0000000000104006h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   52758
+                                                  (000000000000CE16h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         eda7ed97
-  compressed size:                                335 bytes
-  uncompressed size:                              657 bytes
-  length of filename:                             74 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         bac62948
+  compressed size:                                804 bytes
+  uncompressed size:                              2864 bytes
+  length of filename:                             77 characters
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
 
 Central directory entry #43:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/testing/empty_solver_for_testing.py
+  KratosMultiphysics/ShallowWaterApplication/apply_slip_process.py
 
-  offset of local header from start of archive:   1065405
-                                                  (00000000001041BDh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   53697
+                                                  (000000000000D1C1h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         fb54f086
-  compressed size:                                997 bytes
-  uncompressed size:                              3663 bytes
-  length of filename:                             78 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         8f9eefa2
+  compressed size:                                663 bytes
+  uncompressed size:                              1510 bytes
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
 
 Central directory entry #44:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/utilities/benchmarking_utilities.py
+  KratosMultiphysics/ShallowWaterApplication/set_topography_process.py
 
-  offset of local header from start of archive:   1066510
-                                                  (000000000010460Eh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   54482
+                                                  (000000000000D4D2h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         115f223d
-  compressed size:                                296 bytes
-  uncompressed size:                              876 bytes
-  length of filename:                             78 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         c9ac0b54
+  compressed size:                                800 bytes
+  uncompressed size:                              2288 bytes
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
 
 Central directory entry #45:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/utilities/solitary_wave_utilities.py
+  KratosMultiphysics/ShallowWaterApplication/shallow_water_analysis.py
 
-  offset of local header from start of archive:   1066914
-                                                  (00000000001047A2h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   55408
+                                                  (000000000000D870h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         0ea2db75
-  compressed size:                                1141 bytes
-  uncompressed size:                              4364 bytes
-  length of filename:                             79 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         9b823de9
+  compressed size:                                552 bytes
+  uncompressed size:                              1390 bytes
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
 
 Central directory entry #46:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/utilities/wave_factory.py
+  KratosMultiphysics/ShallowWaterApplication/derivatives_recovery_process.py
 
-  offset of local header from start of archive:   1068164
-                                                  (0000000000104C84h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   56086
+                                                  (000000000000DB16h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         31fbbd44
-  compressed size:                                687 bytes
-  uncompressed size:                              2698 bytes
-  length of filename:                             68 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         4a938c61
+  compressed size:                                1372 bytes
+  uncompressed size:                              6190 bytes
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
 
 Central directory entry #47:
 ---------------------------
 
-  KratosMultiphysics/ShallowWaterApplication/utilities/wave_theory_utilities.py
+  KratosMultiphysics/ShallowWaterApplication/modelers/
+
+  offset of local header from start of archive:   57590
+                                                  (000000000000E0F6h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             52 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
-  offset of local header from start of archive:   1068949
-                                                  (0000000000104F95h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #48:
+---------------------------
+
+  KratosMultiphysics/ShallowWaterApplication/modelers/planar_surface_in_parabola_modeler.py
+
+  offset of local header from start of archive:   57700
+                                                  (000000000000E164h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         95ee3be9
-  compressed size:                                1051 bytes
-  uncompressed size:                              4716 bytes
-  length of filename:                             77 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         eaa0c984
+  compressed size:                                285 bytes
+  uncompressed size:                              630 bytes
+  length of filename:                             89 characters
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
 
-Central directory entry #48:
+Central directory entry #49:
+---------------------------
+
+  KratosMultiphysics/ShallowWaterApplication/modelers/dam_break_modeler.py
+
+  offset of local header from start of archive:   58132
+                                                  (000000000000E314h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         f602b508
+  compressed size:                                267 bytes
+  uncompressed size:                              553 bytes
+  length of filename:                             72 characters
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
+Central directory entry #50:
 ---------------------------
 
-  KratosShallowWaterApplication-9.4.5.dist-info/METADATA
+  KratosMultiphysics/ShallowWaterApplication/__init__.py
 
-  offset of local header from start of archive:   1070107
-                                                  (000000000010541Bh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   58529
+                                                  (000000000000E4A1h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         bf8d7a80
-  compressed size:                                1358 bytes
-  uncompressed size:                              3308 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         6eb78ecd
+  compressed size:                                131 bytes
+  uncompressed size:                              282 bytes
   length of filename:                             54 characters
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
 
-Central directory entry #49:
+Central directory entry #51:
 ---------------------------
 
-  KratosShallowWaterApplication-9.4.5.dist-info/WHEEL
+  KratosMultiphysics/ShallowWaterApplication/set_initial_perturbation_process.py
 
-  offset of local header from start of archive:   1071549
-                                                  (00000000001059BDh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   58772
+                                                  (000000000000E594h) bytes
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
-  length of filename:                             51 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         191f43fe
+  compressed size:                                1022 bytes
+  uncompressed size:                              3339 bytes
+  length of filename:                             78 characters
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
+Central directory entry #52:
+---------------------------
+
+  KratosMultiphysics/ShallowWaterApplication/set_initial_water_level_process.py
+
+  offset of local header from start of archive:   59930
+                                                  (000000000000EA1Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         9146084f
+  compressed size:                                786 bytes
+  uncompressed size:                              2355 bytes
+  length of filename:                             77 characters
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
+Central directory entry #53:
+---------------------------
+
+  KratosMultiphysics/.libs/
+
+  offset of local header from start of archive:   60851
+                                                  (000000000000EDB3h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:26
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:26 UTC
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
+Central directory entry #54:
+---------------------------
+
+  KratosMultiphysics/.libs/KratosShallowWaterApplication.cpython-38-x86_64-linux-gnu.so
+
+  offset of local header from start of archive:   60934
+                                                  (000000000000EE06h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         1cdcf954
+  compressed size:                                981764 bytes
+  uncompressed size:                              2877833 bytes
+  length of filename:                             85 characters
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
 
-Central directory entry #50:
+Central directory entry #55:
+---------------------------
+
+  KratosShallowWaterApplication-9.5.dist-info/
+
+  offset of local header from start of archive:   1042841
+                                                  (00000000000FE999h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:26
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:26 UTC
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
+Central directory entry #56:
+---------------------------
+
+  KratosShallowWaterApplication-9.5.dist-info/METADATA
+
+  offset of local header from start of archive:   1042943
+                                                  (00000000000FE9FFh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         ea110fe7
+  compressed size:                                1339 bytes
+  uncompressed size:                              3244 bytes
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
+Central directory entry #57:
 ---------------------------
 
-  KratosShallowWaterApplication-9.4.5.dist-info/top_level.txt
+  KratosShallowWaterApplication-9.5.dist-info/WHEEL
 
-  offset of local header from start of archive:   1071726
-                                                  (0000000000105A6Eh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1044392
+                                                  (00000000000FEFA8h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         46d5122e
+  compressed size:                                116 bytes
+  uncompressed size:                              148 bytes
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
+Central directory entry #58:
+---------------------------
+
+  KratosShallowWaterApplication-9.5.dist-info/top_level.txt
+
+  offset of local header from start of archive:   1044615
+                                                  (00000000000FF087h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
   32-bit CRC value (hex):                         f32d789f
-  compressed size:                                21 bytes
+  compressed size:                                19 bytes
   uncompressed size:                              19 bytes
-  length of filename:                             59 characters
-  length of extra field:                          0 bytes
+  length of filename:                             57 characters
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
 
-Central directory entry #51:
+Central directory entry #59:
 ---------------------------
 
-  KratosShallowWaterApplication-9.4.5.dist-info/RECORD
+  KratosShallowWaterApplication-9.5.dist-info/RECORD
 
-  offset of local header from start of archive:   1071836
-                                                  (0000000000105ADCh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1044749
+                                                  (00000000000FF10Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         e46426db
-  compressed size:                                2708 bytes
-  uncompressed size:                              6648 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:26
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:26 UTC
+  32-bit CRC value (hex):                         72806b5d
+  compressed size:                                2724 bytes
+  uncompressed size:                              6742 bytes
+  length of filename:                             50 characters
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
+Central directory entry #60:
+---------------------------
+
+  KratosShallowWaterApplication.libs/
+
+  offset of local header from start of archive:   1047581
+                                                  (00000000000FFC1Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:26
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             35 characters
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
+Central directory entry #61:
+---------------------------
+
+  KratosShallowWaterApplication.libs/libKratosShallowWaterCore-ed139967.so
+
+  offset of local header from start of archive:   1047674
+                                                  (00000000000FFC7Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:38:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:38:20 UTC
+  32-bit CRC value (hex):                         a710f265
+  compressed size:                                1840182 bytes
+  uncompressed size:                              7584961 bytes
+  length of filename:                             72 characters
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
@@ -1,154 +1,184 @@
-Filename: KratosMultiphysics/.libs/KratosShallowWaterApplication.pyd
+Filename: KratosMultiphysics/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosShallowWaterCore.dll
+Filename: KratosMultiphysics/ShallowWaterApplication/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosShallowWaterCore.lib
+Filename: KratosMultiphysics/ShallowWaterApplication/stabilized_shallow_water_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/__init__.py
+Filename: KratosMultiphysics/ShallowWaterApplication/boussinesq_solver.py
 Comment: 
 
 Filename: KratosMultiphysics/ShallowWaterApplication/apply_absorbing_boundary_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/apply_slip_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/coupling/
+Comment: 
+
+Filename: KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_output_process.py
+Comment: 
+
+Filename: KratosMultiphysics/ShallowWaterApplication/coupling/write_from_sw_at_interface_process.py
+Comment: 
+
+Filename: KratosMultiphysics/ShallowWaterApplication/coupling/compute_boundary_force_process.py
+Comment: 
+
+Filename: KratosMultiphysics/ShallowWaterApplication/coupling/read_from_sw_interface_process.py
+Comment: 
+
+Filename: KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_input_process.py
+Comment: 
+
+Filename: KratosMultiphysics/ShallowWaterApplication/wave_solver.py
+Comment: 
+
+Filename: KratosMultiphysics/ShallowWaterApplication/shallow_water_base_solver.py
 Comment: 
 
 Filename: KratosMultiphysics/ShallowWaterApplication/automatic_dirichlet_conditions_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/boussinesq_solver.py
+Filename: KratosMultiphysics/ShallowWaterApplication/utilities/
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/derivatives_recovery_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/utilities/solitary_wave_utilities.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/lagrangian_shallow_water_solver.py
+Filename: KratosMultiphysics/ShallowWaterApplication/utilities/wave_factory.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/primitive_solver.py
+Filename: KratosMultiphysics/ShallowWaterApplication/utilities/wave_theory_utilities.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/set_initial_perturbation_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/utilities/benchmarking_utilities.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/set_initial_water_level_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/set_topography_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/offset_ids_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/shallow_water_analysis.py
+Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/generate_gid_list_file.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/shallow_water_base_solver.py
+Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/compute_froude_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/stabilized_shallow_water_solver.py
+Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/convergence_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/wave_generator_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/visualization_mesh_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/wave_solver.py
+Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/line_envelope_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/base_benchmark_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/auxiliary_nodes_visualization_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/dam_break_benchmark.py
+Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/swap_coordinates_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_shock_benchmark.py
+Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/line_graph_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_transition_benchmark.py
+Filename: KratosMultiphysics/ShallowWaterApplication/primitive_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/planar_surface_in_parabola_benchmark.py
+Filename: KratosMultiphysics/ShallowWaterApplication/testing/
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/solitary_wave_benchmark.py
+Filename: KratosMultiphysics/ShallowWaterApplication/testing/empty_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/coupling/compute_boundary_force_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/testing/empty_solver_for_testing.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_input_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/wave_generator_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_output_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/coupling/read_from_sw_interface_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_shock_benchmark.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/coupling/write_from_sw_at_interface_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/base_benchmark_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/modelers/dam_break_modeler.py
+Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_transition_benchmark.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/modelers/planar_surface_in_parabola_modeler.py
+Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/dam_break_benchmark.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/auxiliary_nodes_visualization_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/solitary_wave_benchmark.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/compute_froude_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/benchmarks/planar_surface_in_parabola_benchmark.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/convergence_output_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/lagrangian_shallow_water_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/generate_gid_list_file.py
+Filename: KratosMultiphysics/ShallowWaterApplication/apply_slip_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/line_envelope_output_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/set_topography_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/line_graph_output_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/shallow_water_analysis.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/offset_ids_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/derivatives_recovery_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/swap_coordinates_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/modelers/
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/postprocess/visualization_mesh_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/modelers/planar_surface_in_parabola_modeler.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/testing/empty_output_process.py
+Filename: KratosMultiphysics/ShallowWaterApplication/modelers/dam_break_modeler.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/testing/empty_solver_for_testing.py
+Filename: KratosMultiphysics/ShallowWaterApplication/__init__.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/utilities/benchmarking_utilities.py
+Filename: KratosMultiphysics/ShallowWaterApplication/set_initial_perturbation_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/utilities/solitary_wave_utilities.py
+Filename: KratosMultiphysics/ShallowWaterApplication/set_initial_water_level_process.py
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/utilities/wave_factory.py
+Filename: KratosMultiphysics/.libs/
 Comment: 
 
-Filename: KratosMultiphysics/ShallowWaterApplication/utilities/wave_theory_utilities.py
+Filename: KratosMultiphysics/.libs/KratosShallowWaterApplication.cpython-38-x86_64-linux-gnu.so
+Comment: 
+
+Filename: KratosShallowWaterApplication-9.5.dist-info/
+Comment: 
+
+Filename: KratosShallowWaterApplication-9.5.dist-info/METADATA
+Comment: 
+
+Filename: KratosShallowWaterApplication-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosShallowWaterApplication-9.4.5.dist-info/METADATA
+Filename: KratosShallowWaterApplication-9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosShallowWaterApplication-9.4.5.dist-info/WHEEL
+Filename: KratosShallowWaterApplication-9.5.dist-info/RECORD
 Comment: 
 
-Filename: KratosShallowWaterApplication-9.4.5.dist-info/top_level.txt
+Filename: KratosShallowWaterApplication.libs/
 Comment: 
 
-Filename: KratosShallowWaterApplication-9.4.5.dist-info/RECORD
+Filename: KratosShallowWaterApplication.libs/libKratosShallowWaterCore-ed139967.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## KratosMultiphysics/ShallowWaterApplication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-# Application dependent names and paths
-from KratosMultiphysics import _ImportApplication
-from KratosShallowWaterApplication import *
-application = KratosShallowWaterApplication()
-application_name = "KratosShallowWaterApplication"
-
-_ImportApplication(application, application_name)
+# Application dependent names and paths
+from KratosMultiphysics import _ImportApplication
+from KratosShallowWaterApplication import *
+application = KratosShallowWaterApplication()
+application_name = "KratosShallowWaterApplication"
+
+_ImportApplication(application, application_name)
```

## KratosMultiphysics/ShallowWaterApplication/apply_absorbing_boundary_process.py

 * *Ordering differences only*

```diff
@@ -1,63 +1,63 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-from KratosMultiphysics.ShallowWaterApplication.utilities.wave_factory import WaveTheoryFactory
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ApplyAbsorbingBoundaryProcess(model, settings["Parameters"])
-
-class ApplyAbsorbingBoundaryProcess(KM.Process):
-    """ApplyAbsorbingBoundaryProcess
-
-    This process sets the DISTANCE variable from every
-    node to the nearest boundary condition
-    """
-
-    @staticmethod
-    def GetDefaultParameters():
-        return KM.Parameters("""{
-            "computing_model_part_name" : "",
-            "absorbing_boundary_name"   : "",
-            "r_squared_threshold"       : 0.99,
-            "relative_distance"         : 2.0,
-            "relative_damping"          : 2.0,
-            "wave_specifications"       : {}
-        }""")
-
-    def __init__(self, model, settings):
-        """The constructor of the ApplyAbsorbingBoundaryProcess"""
-
-        KM.Process.__init__(self)
-
-        self.settings = settings
-        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
-
-        self.model_part = model.GetModelPart(self.settings["computing_model_part_name"].GetString())
-        self.boundary_part = model.GetModelPart(self.settings["absorbing_boundary_name"].GetString())
-        self.distance_process = SW.CalculateDistanceToBoundaryProcess(self.model_part, self.boundary_part, self.settings["r_squared_threshold"].GetDouble())
-
-        variables_names = KM.SpecificationsUtilities.GetDofsListFromConditionsSpecifications(self.boundary_part)
-        self.variables_to_fix = []
-        for variable_name in variables_names:
-            if variable_name.startswith("VELOCITY") or variable_name.startswith("MOMENTUM"):
-                variable = KM.KratosGlobals.GetVariable(variable_name)
-                self.variables_to_fix.append(variable)
-
-    def Check(self):
-        """Check the correctness of the input."""
-        self.distance_process.Check()
-
-    def ExecuteBeforeSolutionLoop(self):
-        """Calculate the distances and the damping parameters."""
-        self.distance_process.ExecuteBeforeSolutionLoop()
-
-        wave = WaveTheoryFactory(self.boundary_part, self.settings["wave_specifications"])
-        absorbing_distance = wave.wavelength * self.settings["relative_distance"].GetDouble()
-        dissipation_factor = wave.frequency * self.settings["relative_damping"].GetDouble()
-
-        self.model_part.ProcessInfo.SetValue(SW.ABSORBING_DISTANCE, absorbing_distance)
-        self.model_part.ProcessInfo.SetValue(SW.DISSIPATION, dissipation_factor)
-
-        for variable in self.variables_to_fix:
-            KM.VariableUtils().ApplyFixity(variable, True, self.boundary_part.Nodes)
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+from KratosMultiphysics.ShallowWaterApplication.utilities.wave_factory import WaveTheoryFactory
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ApplyAbsorbingBoundaryProcess(model, settings["Parameters"])
+
+class ApplyAbsorbingBoundaryProcess(KM.Process):
+    """ApplyAbsorbingBoundaryProcess
+
+    This process sets the DISTANCE variable from every
+    node to the nearest boundary condition
+    """
+
+    @staticmethod
+    def GetDefaultParameters():
+        return KM.Parameters("""{
+            "computing_model_part_name" : "",
+            "absorbing_boundary_name"   : "",
+            "r_squared_threshold"       : 0.99,
+            "relative_distance"         : 2.0,
+            "relative_damping"          : 2.0,
+            "wave_specifications"       : {}
+        }""")
+
+    def __init__(self, model, settings):
+        """The constructor of the ApplyAbsorbingBoundaryProcess"""
+
+        KM.Process.__init__(self)
+
+        self.settings = settings
+        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
+
+        self.model_part = model.GetModelPart(self.settings["computing_model_part_name"].GetString())
+        self.boundary_part = model.GetModelPart(self.settings["absorbing_boundary_name"].GetString())
+        self.distance_process = SW.CalculateDistanceToBoundaryProcess(self.model_part, self.boundary_part, self.settings["r_squared_threshold"].GetDouble())
+
+        variables_names = KM.SpecificationsUtilities.GetDofsListFromConditionsSpecifications(self.boundary_part)
+        self.variables_to_fix = []
+        for variable_name in variables_names:
+            if variable_name.startswith("VELOCITY") or variable_name.startswith("MOMENTUM"):
+                variable = KM.KratosGlobals.GetVariable(variable_name)
+                self.variables_to_fix.append(variable)
+
+    def Check(self):
+        """Check the correctness of the input."""
+        self.distance_process.Check()
+
+    def ExecuteBeforeSolutionLoop(self):
+        """Calculate the distances and the damping parameters."""
+        self.distance_process.ExecuteBeforeSolutionLoop()
+
+        wave = WaveTheoryFactory(self.boundary_part, self.settings["wave_specifications"])
+        absorbing_distance = wave.wavelength * self.settings["relative_distance"].GetDouble()
+        dissipation_factor = wave.frequency * self.settings["relative_damping"].GetDouble()
+
+        self.model_part.ProcessInfo.SetValue(SW.ABSORBING_DISTANCE, absorbing_distance)
+        self.model_part.ProcessInfo.SetValue(SW.DISSIPATION, dissipation_factor)
+
+        for variable in self.variables_to_fix:
+            KM.VariableUtils().ApplyFixity(variable, True, self.boundary_part.Nodes)
```

## KratosMultiphysics/ShallowWaterApplication/apply_slip_process.py

 * *Ordering differences only*

```diff
@@ -1,40 +1,40 @@
-import KratosMultiphysics as KM
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ApplySlipProcess(model, settings["Parameters"])
-
-class ApplySlipProcess(KM.Process):
-    """ApplySlipProcess
-
-    This process sets the SLIP flag and computes the
-    NORMAL variable on the selected model part
-    """
-    def __init__(self, model, settings):
-        """The constructor of the ApplySlipProcess
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        model -- The model to be used
-        settings -- The ProjectParameters used
-        """
-        KM.Process.__init__(self)
-
-        default_parameters = KM.Parameters("""{
-                "model_part_name" : "PLEASE_CHOOSE_MODEL_PART_NAME",
-                "recompute_normals" : false
-            }""")
-        settings.ValidateAndAssignDefaults(default_parameters)
-
-        self.model_part = model[settings["model_part_name"].GetString()]
-        self.recompute_normals = settings["recompute_normals"].GetBool()
-
-    def ExecuteInitialize(self):
-        domain_size = self.model_part.ProcessInfo[KM.DOMAIN_SIZE]
-        KM.NormalCalculationUtils().CalculateOnSimplex(self.model_part, domain_size)
-        KM.VariableUtils().SetFlag(KM.SLIP, True, self.model_part.Nodes)
-
-    def ExecuteInitializeSolutionStep(self):
-        if self.recompute_normals:
-            self.ExecuteInitialize()
+import KratosMultiphysics as KM
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ApplySlipProcess(model, settings["Parameters"])
+
+class ApplySlipProcess(KM.Process):
+    """ApplySlipProcess
+
+    This process sets the SLIP flag and computes the
+    NORMAL variable on the selected model part
+    """
+    def __init__(self, model, settings):
+        """The constructor of the ApplySlipProcess
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        model -- The model to be used
+        settings -- The ProjectParameters used
+        """
+        KM.Process.__init__(self)
+
+        default_parameters = KM.Parameters("""{
+                "model_part_name" : "PLEASE_CHOOSE_MODEL_PART_NAME",
+                "recompute_normals" : false
+            }""")
+        settings.ValidateAndAssignDefaults(default_parameters)
+
+        self.model_part = model[settings["model_part_name"].GetString()]
+        self.recompute_normals = settings["recompute_normals"].GetBool()
+
+    def ExecuteInitialize(self):
+        domain_size = self.model_part.ProcessInfo[KM.DOMAIN_SIZE]
+        KM.NormalCalculationUtils().CalculateOnSimplex(self.model_part, domain_size)
+        KM.VariableUtils().SetFlag(KM.SLIP, True, self.model_part.Nodes)
+
+    def ExecuteInitializeSolutionStep(self):
+        if self.recompute_normals:
+            self.ExecuteInitialize()
```

## KratosMultiphysics/ShallowWaterApplication/automatic_dirichlet_conditions_process.py

 * *Ordering differences only*

```diff
@@ -1,117 +1,117 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return AutomaticDirichletConditionsProcess(model, settings["Parameters"])
-
-## This process fix the variables at the skin
-class AutomaticDirichletConditionsProcess(KM.Process):
-
-    def __init__(self, model, settings):
-
-        KM.Process.__init__(self)
-
-        default_settings = KM.Parameters("""
-            {
-                "model_part_name"             : "main_model_part",
-                "scalar_variables_list"       : [],
-                "scalar_value"                : 0.0,
-                "scalar_constraint"           : true,
-                "vector_variables_list"       : [],
-                "vector_value"                : [0.0, 0.0, 0.0],
-                "vector_constraint"           : [true, true, true],
-                "auxiliary_model_part_name"   : "skin_model_part",
-                "auxiliary_condition_name"    : "Condition",
-                "skin_parts_to_exclude"       : [],
-                "allow_outwards_flow_on_land" : true,
-                "sea_water_level"             : 0.0
-            }
-            """
-            )
-        settings.ValidateAndAssignDefaults(default_settings)
-        self.settings = settings
-        self.model = model
-
-        self._CheckIfParameterIsRelativeSubModelPartName(self.settings["auxiliary_model_part_name"])
-        for item in self.settings["skin_parts_to_exclude"]:
-            self._CheckIfParameterIsRelativeSubModelPartName(item)
-
-    def ExecuteInitialize(self):
-        model_part_name = self.settings["model_part_name"].GetString()
-        model_part = self.model[model_part_name]
-
-        skin_detection_settings = KM.Parameters()
-        skin_detection_settings.AddValue("name_auxiliar_model_part", self.settings["auxiliary_model_part_name"])
-        skin_detection_settings.AddValue("name_auxiliar_condition", self.settings["auxiliary_condition_name"])
-        skin_detection_settings.AddValue("list_model_parts_to_assign_conditions", self.settings["skin_parts_to_exclude"])
-        KM.SkinDetectionProcess2D(model_part, skin_detection_settings).Execute()
-
-        skin_model_part_name = model_part_name + '.' + self.settings["auxiliary_model_part_name"].GetString()
-        skin_model_part = self.model[skin_model_part_name]
-
-        # We remove the new interface condition from the bondaries with other conditions
-        for name in self.settings["skin_parts_to_exclude"].GetStringArray():
-            skin_to_exclude = model_part_name + '.' + name
-            self.model[skin_to_exclude].RemoveConditionsFromAllLevels(KM.INTERFACE)
-            KM.VariableUtils().SetFlag(KM.INTERFACE, False, self.model[skin_to_exclude].Nodes)
-        skin_model_part.RemoveNodes((KM.INTERFACE).AsFalse())
-
-        # Here we exclude the interface which will has an outward flow
-        if self.settings["allow_outwards_flow_on_land"].GetBool():
-            dimension = 2
-            KM.NormalCalculationUtils().CalculateOnSimplex(skin_model_part, dimension)
-            KM.ComputeNonHistoricalNodalGradientProcess(model_part, SW.TOPOGRAPHY, SW.TOPOGRAPHY_GRADIENT, KM.NODAL_AREA).Execute()
-            SW.ShallowWaterUtilities().IdentifySolidBoundary(skin_model_part, self.settings["sea_water_level"].GetDouble(), KM.SOLID)
-            skin_model_part.RemoveNodes((KM.SOLID).AsFalse())
-            skin_model_part.RemoveConditionsFromAllLevels((KM.SOLID).AsFalse())
-        else:
-            KM.VariableUtils().SetFlag(KM.SOLID, True, skin_model_part.Nodes)
-            KM.VariableUtils().SetFlag(KM.SOLID, True, skin_model_part.Conditions)
-
-        self.processes = []
-
-        from KratosMultiphysics.assign_scalar_variable_process import AssignScalarVariableProcess
-        for variable in self.settings["scalar_variables_list"].GetStringArray():
-            scalar_settings = KM.Parameters()
-            scalar_settings.AddEmptyValue("model_part_name").SetString(skin_model_part_name)
-            scalar_settings.AddEmptyValue("variable_name").SetString(variable)
-            scalar_settings.AddValue("value", self.settings["scalar_value"])
-            scalar_settings.AddValue("constrained", self.settings["scalar_constraint"])
-            self.processes.append(AssignScalarVariableProcess(self.model, scalar_settings))
-
-        from KratosMultiphysics.assign_vector_variable_process import AssignVectorVariableProcess
-        for variable in self.settings["vector_variables_list"].GetStringArray():
-            vector_settings = KM.Parameters()
-            vector_settings.AddEmptyValue("model_part_name").SetString(skin_model_part_name)
-            vector_settings.AddEmptyValue("variable_name").SetString(variable)
-            vector_settings.AddValue("value", self.settings["vector_value"])
-            vector_settings.AddValue("constrained", self.settings["vector_constraint"])
-            self.processes.append(AssignVectorVariableProcess(self.model, vector_settings))
-
-    def ExecuteBeforeSolutionLoop(self):
-        for process in self.processes:
-            process.ExecuteBeforeSolutionLoop()
-
-    def ExecuteInitializeSolutionStep(self):
-        for process in self.processes:
-            process.ExecuteInitializeSolutionStep()
-
-    def ExecuteFinalizeSolutionStep(self):
-        for process in self.processes:
-            process.ExecuteFinalizeSolutionStep()
-
-    @staticmethod
-    def _CheckIfParameterIsRelativeSubModelPartName(param):
-        name = param.GetString()
-        search = name.find('.')
-        if search != -1:
-            items = name.split('.')
-            msg = "AutomaticDirichletConditionsProcess"
-            msg += 'Please, specify the sub model part with the relative name\n'
-            msg += '\tWrite : \"' + items[-1] + '\"\n'
-            msg += '\tinstead of : \"' +  name + '\"\n'
-            param.SetString(name)
-            # The parameters are passed by value, we shall throw an error
-            raise Exception(msg)
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return AutomaticDirichletConditionsProcess(model, settings["Parameters"])
+
+## This process fix the variables at the skin
+class AutomaticDirichletConditionsProcess(KM.Process):
+
+    def __init__(self, model, settings):
+
+        KM.Process.__init__(self)
+
+        default_settings = KM.Parameters("""
+            {
+                "model_part_name"             : "main_model_part",
+                "scalar_variables_list"       : [],
+                "scalar_value"                : 0.0,
+                "scalar_constraint"           : true,
+                "vector_variables_list"       : [],
+                "vector_value"                : [0.0, 0.0, 0.0],
+                "vector_constraint"           : [true, true, true],
+                "auxiliary_model_part_name"   : "skin_model_part",
+                "auxiliary_condition_name"    : "Condition",
+                "skin_parts_to_exclude"       : [],
+                "allow_outwards_flow_on_land" : true,
+                "sea_water_level"             : 0.0
+            }
+            """
+            )
+        settings.ValidateAndAssignDefaults(default_settings)
+        self.settings = settings
+        self.model = model
+
+        self._CheckIfParameterIsRelativeSubModelPartName(self.settings["auxiliary_model_part_name"])
+        for item in self.settings["skin_parts_to_exclude"]:
+            self._CheckIfParameterIsRelativeSubModelPartName(item)
+
+    def ExecuteInitialize(self):
+        model_part_name = self.settings["model_part_name"].GetString()
+        model_part = self.model[model_part_name]
+
+        skin_detection_settings = KM.Parameters()
+        skin_detection_settings.AddValue("name_auxiliar_model_part", self.settings["auxiliary_model_part_name"])
+        skin_detection_settings.AddValue("name_auxiliar_condition", self.settings["auxiliary_condition_name"])
+        skin_detection_settings.AddValue("list_model_parts_to_assign_conditions", self.settings["skin_parts_to_exclude"])
+        KM.SkinDetectionProcess2D(model_part, skin_detection_settings).Execute()
+
+        skin_model_part_name = model_part_name + '.' + self.settings["auxiliary_model_part_name"].GetString()
+        skin_model_part = self.model[skin_model_part_name]
+
+        # We remove the new interface condition from the bondaries with other conditions
+        for name in self.settings["skin_parts_to_exclude"].GetStringArray():
+            skin_to_exclude = model_part_name + '.' + name
+            self.model[skin_to_exclude].RemoveConditionsFromAllLevels(KM.INTERFACE)
+            KM.VariableUtils().SetFlag(KM.INTERFACE, False, self.model[skin_to_exclude].Nodes)
+        skin_model_part.RemoveNodes((KM.INTERFACE).AsFalse())
+
+        # Here we exclude the interface which will has an outward flow
+        if self.settings["allow_outwards_flow_on_land"].GetBool():
+            dimension = 2
+            KM.NormalCalculationUtils().CalculateOnSimplex(skin_model_part, dimension)
+            KM.ComputeNonHistoricalNodalGradientProcess(model_part, SW.TOPOGRAPHY, SW.TOPOGRAPHY_GRADIENT, KM.NODAL_AREA).Execute()
+            SW.ShallowWaterUtilities().IdentifySolidBoundary(skin_model_part, self.settings["sea_water_level"].GetDouble(), KM.SOLID)
+            skin_model_part.RemoveNodes((KM.SOLID).AsFalse())
+            skin_model_part.RemoveConditionsFromAllLevels((KM.SOLID).AsFalse())
+        else:
+            KM.VariableUtils().SetFlag(KM.SOLID, True, skin_model_part.Nodes)
+            KM.VariableUtils().SetFlag(KM.SOLID, True, skin_model_part.Conditions)
+
+        self.processes = []
+
+        from KratosMultiphysics.assign_scalar_variable_process import AssignScalarVariableProcess
+        for variable in self.settings["scalar_variables_list"].GetStringArray():
+            scalar_settings = KM.Parameters()
+            scalar_settings.AddEmptyValue("model_part_name").SetString(skin_model_part_name)
+            scalar_settings.AddEmptyValue("variable_name").SetString(variable)
+            scalar_settings.AddValue("value", self.settings["scalar_value"])
+            scalar_settings.AddValue("constrained", self.settings["scalar_constraint"])
+            self.processes.append(AssignScalarVariableProcess(self.model, scalar_settings))
+
+        from KratosMultiphysics.assign_vector_variable_process import AssignVectorVariableProcess
+        for variable in self.settings["vector_variables_list"].GetStringArray():
+            vector_settings = KM.Parameters()
+            vector_settings.AddEmptyValue("model_part_name").SetString(skin_model_part_name)
+            vector_settings.AddEmptyValue("variable_name").SetString(variable)
+            vector_settings.AddValue("value", self.settings["vector_value"])
+            vector_settings.AddValue("constrained", self.settings["vector_constraint"])
+            self.processes.append(AssignVectorVariableProcess(self.model, vector_settings))
+
+    def ExecuteBeforeSolutionLoop(self):
+        for process in self.processes:
+            process.ExecuteBeforeSolutionLoop()
+
+    def ExecuteInitializeSolutionStep(self):
+        for process in self.processes:
+            process.ExecuteInitializeSolutionStep()
+
+    def ExecuteFinalizeSolutionStep(self):
+        for process in self.processes:
+            process.ExecuteFinalizeSolutionStep()
+
+    @staticmethod
+    def _CheckIfParameterIsRelativeSubModelPartName(param):
+        name = param.GetString()
+        search = name.find('.')
+        if search != -1:
+            items = name.split('.')
+            msg = "AutomaticDirichletConditionsProcess"
+            msg += 'Please, specify the sub model part with the relative name\n'
+            msg += '\tWrite : \"' + items[-1] + '\"\n'
+            msg += '\tinstead of : \"' +  name + '\"\n'
+            param.SetString(name)
+            # The parameters are passed by value, we shall throw an error
+            raise Exception(msg)
```

## KratosMultiphysics/ShallowWaterApplication/boussinesq_solver.py

 * *Ordering differences only*

```diff
@@ -1,69 +1,69 @@
-# importing the Kratos Library
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-## Import base class file
-from KratosMultiphysics.ShallowWaterApplication.shallow_water_base_solver import ShallowWaterBaseSolver
-
-def CreateSolver(model, custom_settings):
-    return BoussinesqSolver(model, custom_settings)
-
-class BoussinesqSolver(ShallowWaterBaseSolver):
-    def __init__(self, model, settings):
-        super().__init__(model, settings)
-        self.element_name = "BoussinesqElement"
-        self.condition_name = "BoussinesqCondition"
-        if self.settings["time_integration_scheme"].GetString().lower() == "bdf":
-            self.min_buffer_size = self.settings["time_integration_order"].GetInt() + 1
-        else:
-            self.min_buffer_size = 4
-            if self.settings["time_integration_order"].GetInt() != 4:
-                msg = "The order considered for the Adams-Moulton scheme is 4. The user provided order is {}"
-                KM.Logger.PrintWarning(self.__class__.__name__, msg.format(self.settings["time_integration_order"].GetInt()))
-
-    def AddDofs(self):
-        KM.VariableUtils().AddDof(KM.VELOCITY_X, self.main_model_part)
-        KM.VariableUtils().AddDof(KM.VELOCITY_Y, self.main_model_part)
-        KM.VariableUtils().AddDof(SW.HEIGHT, self.main_model_part)
-        KM.Logger.PrintInfo(self.__class__.__name__, "Boussinesq equations DOFs added correctly.")
-
-    def AddVariables(self):
-        super().AddVariables()
-        self.main_model_part.AddNodalSolutionStepVariable(SW.DISPERSION_H)      # Intermediate field
-        self.main_model_part.AddNodalSolutionStepVariable(SW.DISPERSION_V)      # Intermediate field
-        self.main_model_part.AddNodalSolutionStepVariable(KM.RHS)               # This is used by the predictor in ABM scheme
-        self.main_model_part.AddNodalSolutionStepVariable(KM.NODAL_AREA)        # This is used to assemble the RHS by the predictor and the dispersive fields
-
-    def FinalizeSolutionStep(self):
-        super().FinalizeSolutionStep()
-        SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.main_model_part)
-
-    def _SetProcessInfo(self):
-        super()._SetProcessInfo()
-        self.main_model_part.ProcessInfo.SetValue(SW.RELATIVE_DRY_HEIGHT, self.settings["relative_dry_height"].GetDouble())
-        self.main_model_part.ProcessInfo.SetValue(KM.STABILIZATION_FACTOR, self.settings["stabilization_factor"].GetDouble())
-        self.main_model_part.ProcessInfo.SetValue(SW.SHOCK_STABILIZATION_FACTOR, self.settings["shock_capturing_factor"].GetDouble())
-
-    def _CreateScheme(self):
-        if self.settings["time_integration_scheme"].GetString().lower() == "bdf":
-            scheme_settings = KM.Parameters()
-            scheme_settings.AddStringArray("solution_variables", ["VELOCITY","HEIGHT"])
-            scheme_settings.AddValue("integration_order", self.settings["time_integration_order"])
-            scheme_settings.AddBool("project_dispersive_field", True)
-            return SW.ShallowWaterResidualBasedBDFScheme(scheme_settings)
-        elif self.settings["time_integration_scheme"].GetString().lower() == "adams-moulton":
-            return SW.ResidualBasedAdamsMoultonScheme()
-        else:
-            raise Exception("Unknown time scheme, possible options are 'Adams-Moulton' or 'BDF'")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        default_settings = KM.Parameters("""{
-            "relative_dry_height"        : 0.1,
-            "stabilization_factor"       : 0.01,
-            "shock_capturing_factor"     : 0.0,
-            "time_integration_scheme"    : "Adams-Moulton",
-            "time_integration_order"     : 4
-        }""")
-        default_settings.AddMissingParameters(super().GetDefaultParameters())
-        return default_settings
+# importing the Kratos Library
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+## Import base class file
+from KratosMultiphysics.ShallowWaterApplication.shallow_water_base_solver import ShallowWaterBaseSolver
+
+def CreateSolver(model, custom_settings):
+    return BoussinesqSolver(model, custom_settings)
+
+class BoussinesqSolver(ShallowWaterBaseSolver):
+    def __init__(self, model, settings):
+        super().__init__(model, settings)
+        self.element_name = "BoussinesqElement"
+        self.condition_name = "BoussinesqCondition"
+        if self.settings["time_integration_scheme"].GetString().lower() == "bdf":
+            self.min_buffer_size = self.settings["time_integration_order"].GetInt() + 1
+        else:
+            self.min_buffer_size = 4
+            if self.settings["time_integration_order"].GetInt() != 4:
+                msg = "The order considered for the Adams-Moulton scheme is 4. The user provided order is {}"
+                KM.Logger.PrintWarning(self.__class__.__name__, msg.format(self.settings["time_integration_order"].GetInt()))
+
+    def AddDofs(self):
+        KM.VariableUtils().AddDof(KM.VELOCITY_X, self.main_model_part)
+        KM.VariableUtils().AddDof(KM.VELOCITY_Y, self.main_model_part)
+        KM.VariableUtils().AddDof(SW.HEIGHT, self.main_model_part)
+        KM.Logger.PrintInfo(self.__class__.__name__, "Boussinesq equations DOFs added correctly.")
+
+    def AddVariables(self):
+        super().AddVariables()
+        self.main_model_part.AddNodalSolutionStepVariable(SW.DISPERSION_H)      # Intermediate field
+        self.main_model_part.AddNodalSolutionStepVariable(SW.DISPERSION_V)      # Intermediate field
+        self.main_model_part.AddNodalSolutionStepVariable(KM.RHS)               # This is used by the predictor in ABM scheme
+        self.main_model_part.AddNodalSolutionStepVariable(KM.NODAL_AREA)        # This is used to assemble the RHS by the predictor and the dispersive fields
+
+    def FinalizeSolutionStep(self):
+        super().FinalizeSolutionStep()
+        SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.main_model_part)
+
+    def _SetProcessInfo(self):
+        super()._SetProcessInfo()
+        self.main_model_part.ProcessInfo.SetValue(SW.RELATIVE_DRY_HEIGHT, self.settings["relative_dry_height"].GetDouble())
+        self.main_model_part.ProcessInfo.SetValue(KM.STABILIZATION_FACTOR, self.settings["stabilization_factor"].GetDouble())
+        self.main_model_part.ProcessInfo.SetValue(SW.SHOCK_STABILIZATION_FACTOR, self.settings["shock_capturing_factor"].GetDouble())
+
+    def _CreateScheme(self):
+        if self.settings["time_integration_scheme"].GetString().lower() == "bdf":
+            scheme_settings = KM.Parameters()
+            scheme_settings.AddStringArray("solution_variables", ["VELOCITY","HEIGHT"])
+            scheme_settings.AddValue("integration_order", self.settings["time_integration_order"])
+            scheme_settings.AddBool("project_dispersive_field", True)
+            return SW.ShallowWaterResidualBasedBDFScheme(scheme_settings)
+        elif self.settings["time_integration_scheme"].GetString().lower() == "adams-moulton":
+            return SW.ResidualBasedAdamsMoultonScheme()
+        else:
+            raise Exception("Unknown time scheme, possible options are 'Adams-Moulton' or 'BDF'")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        default_settings = KM.Parameters("""{
+            "relative_dry_height"        : 0.1,
+            "stabilization_factor"       : 0.01,
+            "shock_capturing_factor"     : 0.0,
+            "time_integration_scheme"    : "Adams-Moulton",
+            "time_integration_order"     : 4
+        }""")
+        default_settings.AddMissingParameters(super().GetDefaultParameters())
+        return default_settings
```

## KratosMultiphysics/ShallowWaterApplication/derivatives_recovery_process.py

 * *Ordering differences only*

```diff
@@ -1,142 +1,142 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-
-def Factory(settings, Model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return DerivativesRecoveryProcess(Model, settings["Parameters"])
-
-
-class DerivativesRecoveryProcess(KM.Process):
-
-    @staticmethod
-    def GetDefaultParameters():
-        return KM.Parameters("""
-        {
-            "model_part_name"          : "model_part",
-            "list_of_operations"       : [],
-            "compute_neighbors"        : true,
-            "update_mesh_topology"     : false
-        }
-        """)
-
-    class DifferentialOperator(KM.Process):
-        '''Auxiliary class to execute the derivatives recovery.'''
-
-        @staticmethod
-        def GetDefaultParameters():
-            return KM.Parameters("""
-            {
-                "operation"           : "gradient",
-                "primitive_variable"  : "",
-                "derivative_variable" : "",
-                "buffer_step"         : 0,
-                "process_step"        : "ExecuteFinalizeSolutionStep"
-            }
-            """)
-
-        __operations = {
-            "gradient"   : "RecoverGradient",
-            "divergence" : "RecoverDivergence",
-            "laplacian"  : "RecoverLaplacian"
-        }
-
-        def __init__(self, settings, recovery_tool, model_part):
-            KM.Process.__init__(self)
-            settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
-            self.operation = self.__operations[settings["operation"].GetString()]
-            self.primitive_variable = KM.KratosGlobals.GetVariable(settings["primitive_variable"].GetString())
-            self.derivative_variable = KM.KratosGlobals.GetVariable(settings["derivative_variable"].GetString())
-            self.buffer_step = settings["buffer_step"].GetInt()
-            self.process_step = settings["process_step"].GetString()
-            self.model_part = model_part
-            self.differentiation = getattr(recovery_tool, self.operation)
-            setattr(self, self.process_step, self.ExecuteDifferentiation)
-
-        def ExecuteDifferentiation(self):
-            self.differentiation(self.model_part, self.primitive_variable, self.derivative_variable, self.buffer_step)
-
-        def Check(self):
-            if self.operation == "RecoverGradient":
-                if not isinstance(self.primitive_variable, KM.DoubleVariable):
-                    raise Exception("The primitive variable of a gradient should be a scalar")
-                if not isinstance(self.derivative_variable, KM.Array1DVariable3):
-                    raise Exception("The derivative variable of a gradient should be a vector")
-            if self.operation == "RecoverDivergence":
-                if not isinstance(self.primitive_variable, KM.Array1DVariable3):
-                    raise Exception("The primitive variable of a divergence should be a vector")
-                if not isinstance(self.derivative_variable, KM.DoubleVariable):
-                    raise Exception("The derivative variable of a divergence should be a scalar")
-            if self.operation == "RecoverLaplacian":
-                is_scalar = isinstance(self.primitive_variable, KM.DoubleVariable)
-                is_vector = isinstance(self.primitive_variable, KM.Array1DVariable3)
-                if is_scalar:
-                    if not isinstance(self.derivative_variable, KM.DoubleVariable):
-                        raise Exception("The derivative variable of a scalar laplacian should be a scalar")
-                elif is_vector:
-                    if not isinstance(self.primitive_variable, KM.Array1DVariable3):
-                        raise Exception("The derivative variable of a vector laplacian should be a vector")
-                else:
-                    raise Exception("The primitive and derivative variables of a laplacian must be scalar or vector")
-
-
-    def __init__(self, model, settings ):
-        """Construct the DerivativesRecoveryProcess."""
-
-        KM.Process.__init__(self)
-
-        settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
-        self.settings = settings
-        self.model_part = model.GetModelPart(self.settings["model_part_name"].GetString())
-
-        domain_size = self.model_part.ProcessInfo.GetValue(KM.DOMAIN_SIZE)
-        if domain_size == 2:
-            self.recovery_tool = SW.DerivativesRecoveryUtility2D
-        else:
-            self.recovery_tool = SW.DerivativesRecoveryUtility3D
-
-        self.operations = []
-        for operation_settings in self.settings["list_of_operations"].values():
-            operation = self.DifferentialOperator(operation_settings, self.recovery_tool, self.model_part)
-            self.operations.append(operation)
-
-    def Check(self):
-        self.recovery_tool.Check(self.model_part)
-        for operation in self.operations:
-            operation.Check()
-
-    def ExecuteInitialize(self):
-        if self.settings["compute_neighbors"].GetBool():
-            KM.FindGlobalNodalNeighboursProcess(self.model_part).Execute()
-        self.recovery_tool.CalculatePolynomialWeights(self.model_part)
-
-        for operation in self.operations:
-            operation.ExecuteInitialize()
-
-    def ExecuteBeforeSolutionLoop(self):
-        for operation in self.operations:
-            operation.ExecuteBeforeSolutionLoop()
-
-    def ExecuteInitializeSolutionStep(self):
-        if self.settings["update_mesh_topology"].GetBool():
-            self.ExecuteInitialize()
-
-        for operation in self.operations:
-            operation.ExecuteInitializeSolutionStep()
-
-    def ExecuteFinalizeSolutionStep(self):
-        for operation in self.operations:
-            operation.ExecuteFinalizeSolutionStep()
-
-    def ExecuteBeforeOutputStep(self):
-        for operation in self.operations:
-            operation.ExecuteBeforeOutputStep()
-
-    def ExecuteAfterOutputStep(self):
-        for operation in self.operations:
-            operation.ExecuteAfterOutputStep()
-
-    def ExecuteFinalize(self):
-        for operation in self.operations:
-            operation.ExecuteFinalize()
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+
+def Factory(settings, Model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return DerivativesRecoveryProcess(Model, settings["Parameters"])
+
+
+class DerivativesRecoveryProcess(KM.Process):
+
+    @staticmethod
+    def GetDefaultParameters():
+        return KM.Parameters("""
+        {
+            "model_part_name"          : "model_part",
+            "list_of_operations"       : [],
+            "compute_neighbors"        : true,
+            "update_mesh_topology"     : false
+        }
+        """)
+
+    class DifferentialOperator(KM.Process):
+        '''Auxiliary class to execute the derivatives recovery.'''
+
+        @staticmethod
+        def GetDefaultParameters():
+            return KM.Parameters("""
+            {
+                "operation"           : "gradient",
+                "primitive_variable"  : "",
+                "derivative_variable" : "",
+                "buffer_step"         : 0,
+                "process_step"        : "ExecuteFinalizeSolutionStep"
+            }
+            """)
+
+        __operations = {
+            "gradient"   : "RecoverGradient",
+            "divergence" : "RecoverDivergence",
+            "laplacian"  : "RecoverLaplacian"
+        }
+
+        def __init__(self, settings, recovery_tool, model_part):
+            KM.Process.__init__(self)
+            settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
+            self.operation = self.__operations[settings["operation"].GetString()]
+            self.primitive_variable = KM.KratosGlobals.GetVariable(settings["primitive_variable"].GetString())
+            self.derivative_variable = KM.KratosGlobals.GetVariable(settings["derivative_variable"].GetString())
+            self.buffer_step = settings["buffer_step"].GetInt()
+            self.process_step = settings["process_step"].GetString()
+            self.model_part = model_part
+            self.differentiation = getattr(recovery_tool, self.operation)
+            setattr(self, self.process_step, self.ExecuteDifferentiation)
+
+        def ExecuteDifferentiation(self):
+            self.differentiation(self.model_part, self.primitive_variable, self.derivative_variable, self.buffer_step)
+
+        def Check(self):
+            if self.operation == "RecoverGradient":
+                if not isinstance(self.primitive_variable, KM.DoubleVariable):
+                    raise Exception("The primitive variable of a gradient should be a scalar")
+                if not isinstance(self.derivative_variable, KM.Array1DVariable3):
+                    raise Exception("The derivative variable of a gradient should be a vector")
+            if self.operation == "RecoverDivergence":
+                if not isinstance(self.primitive_variable, KM.Array1DVariable3):
+                    raise Exception("The primitive variable of a divergence should be a vector")
+                if not isinstance(self.derivative_variable, KM.DoubleVariable):
+                    raise Exception("The derivative variable of a divergence should be a scalar")
+            if self.operation == "RecoverLaplacian":
+                is_scalar = isinstance(self.primitive_variable, KM.DoubleVariable)
+                is_vector = isinstance(self.primitive_variable, KM.Array1DVariable3)
+                if is_scalar:
+                    if not isinstance(self.derivative_variable, KM.DoubleVariable):
+                        raise Exception("The derivative variable of a scalar laplacian should be a scalar")
+                elif is_vector:
+                    if not isinstance(self.primitive_variable, KM.Array1DVariable3):
+                        raise Exception("The derivative variable of a vector laplacian should be a vector")
+                else:
+                    raise Exception("The primitive and derivative variables of a laplacian must be scalar or vector")
+
+
+    def __init__(self, model, settings ):
+        """Construct the DerivativesRecoveryProcess."""
+
+        KM.Process.__init__(self)
+
+        settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
+        self.settings = settings
+        self.model_part = model.GetModelPart(self.settings["model_part_name"].GetString())
+
+        domain_size = self.model_part.ProcessInfo.GetValue(KM.DOMAIN_SIZE)
+        if domain_size == 2:
+            self.recovery_tool = SW.DerivativesRecoveryUtility2D
+        else:
+            self.recovery_tool = SW.DerivativesRecoveryUtility3D
+
+        self.operations = []
+        for operation_settings in self.settings["list_of_operations"].values():
+            operation = self.DifferentialOperator(operation_settings, self.recovery_tool, self.model_part)
+            self.operations.append(operation)
+
+    def Check(self):
+        self.recovery_tool.Check(self.model_part)
+        for operation in self.operations:
+            operation.Check()
+
+    def ExecuteInitialize(self):
+        if self.settings["compute_neighbors"].GetBool():
+            KM.FindGlobalNodalNeighboursProcess(self.model_part).Execute()
+        self.recovery_tool.CalculatePolynomialWeights(self.model_part)
+
+        for operation in self.operations:
+            operation.ExecuteInitialize()
+
+    def ExecuteBeforeSolutionLoop(self):
+        for operation in self.operations:
+            operation.ExecuteBeforeSolutionLoop()
+
+    def ExecuteInitializeSolutionStep(self):
+        if self.settings["update_mesh_topology"].GetBool():
+            self.ExecuteInitialize()
+
+        for operation in self.operations:
+            operation.ExecuteInitializeSolutionStep()
+
+    def ExecuteFinalizeSolutionStep(self):
+        for operation in self.operations:
+            operation.ExecuteFinalizeSolutionStep()
+
+    def ExecuteBeforeOutputStep(self):
+        for operation in self.operations:
+            operation.ExecuteBeforeOutputStep()
+
+    def ExecuteAfterOutputStep(self):
+        for operation in self.operations:
+            operation.ExecuteAfterOutputStep()
+
+    def ExecuteFinalize(self):
+        for operation in self.operations:
+            operation.ExecuteFinalize()
```

## KratosMultiphysics/ShallowWaterApplication/lagrangian_shallow_water_solver.py

 * *Ordering differences only*

```diff
@@ -1,84 +1,84 @@
-# importing the Kratos Library
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-## Import base class file
-from KratosMultiphysics.python_solver import PythonSolver
-from KratosMultiphysics.ShallowWaterApplication.wave_solver import WaveSolver
-
-def CreateSolver(model, custom_settings):
-    return LagrangianShallowWaterSolver(model, custom_settings)
-
-class LagrangianShallowWaterSolver(PythonSolver):
-    def __init__(self, model, settings):
-        super().__init__(model, settings)
-
-        self.mesh_solver = WaveSolver(self.model, self.settings["mesh_solver_settings"])
-
-        # Either retrieve the model part from the model or create a new one
-        self.main_model_part = self.model.CreateModelPart(self.settings["model_part_name"].GetString())
-
-        eulerian_model_part = self.main_model_part
-        lagrangian_model_part = self.mesh_solver.main_model_part
-        self.mesh_moving = SW.MoveShallowMeshUtility(lagrangian_model_part, eulerian_model_part, self.settings["mesh_moving_settings"])
-
-    def AddVariables(self):
-        self.mesh_solver.AddVariables()
-        self.mesh_solver.main_model_part.AddNodalSolutionStepVariable(KM.DISPLACEMENT)
-        KM.MergeVariableListsUtility().Merge(self.mesh_solver.main_model_part, self.main_model_part)
-
-    def ImportModelPart(self):
-        pass
-
-    def PrepareModelPart(self):
-        self.mesh_solver.PrepareModelPart()
-
-    def AddDofs(self):
-        self.mesh_solver.AddDofs()
-
-    def AdvanceInTime(self, current_time):
-        return self.mesh_solver.AdvanceInTime(current_time)
-
-    def GetComputingModelPart(self):
-        return self.mesh_solver.GetComputingModelPart()
-
-    def Initialize(self):
-        self.mesh_moving.Initialize()
-        self.mesh_solver.Initialize()
-
-    def InitializeSolutionStep(self):
-        self.mesh_moving.MoveMesh()
-        self.mesh_solver.InitializeSolutionStep()
-
-    def Predict(self):
-        self.mesh_solver.Predict()
-
-    def SolveSolutionStep(self):
-        return self.mesh_solver.SolveSolutionStep()
-
-    def FinalizeSolutionStep(self):
-        self.mesh_solver.FinalizeSolutionStep()
-        self.mesh_moving.MapResults()
-        SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.main_model_part)
-
-    def Finalize(self):
-        self.mesh_solver.Finalize()
-
-    def Check(self):
-        self.mesh_solver.Check()
-        self.mesh_moving.Check()
-
-    def Clear(self):
-        self.mesh_solver.Clear()
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        default_settings = KM.Parameters("""
-        {
-            "solver_type"              : "",
-            "model_part_name"          : "eulerian_model_part",
-            "echo_level"               : 0,
-            "mesh_solver_settings"     : {},
-            "mesh_moving_settings"     : {}
-        }""")
-        return default_settings
+# importing the Kratos Library
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+## Import base class file
+from KratosMultiphysics.python_solver import PythonSolver
+from KratosMultiphysics.ShallowWaterApplication.wave_solver import WaveSolver
+
+def CreateSolver(model, custom_settings):
+    return LagrangianShallowWaterSolver(model, custom_settings)
+
+class LagrangianShallowWaterSolver(PythonSolver):
+    def __init__(self, model, settings):
+        super().__init__(model, settings)
+
+        self.mesh_solver = WaveSolver(self.model, self.settings["mesh_solver_settings"])
+
+        # Either retrieve the model part from the model or create a new one
+        self.main_model_part = self.model.CreateModelPart(self.settings["model_part_name"].GetString())
+
+        eulerian_model_part = self.main_model_part
+        lagrangian_model_part = self.mesh_solver.main_model_part
+        self.mesh_moving = SW.MoveShallowMeshUtility(lagrangian_model_part, eulerian_model_part, self.settings["mesh_moving_settings"])
+
+    def AddVariables(self):
+        self.mesh_solver.AddVariables()
+        self.mesh_solver.main_model_part.AddNodalSolutionStepVariable(KM.DISPLACEMENT)
+        KM.MergeVariableListsUtility().Merge(self.mesh_solver.main_model_part, self.main_model_part)
+
+    def ImportModelPart(self):
+        pass
+
+    def PrepareModelPart(self):
+        self.mesh_solver.PrepareModelPart()
+
+    def AddDofs(self):
+        self.mesh_solver.AddDofs()
+
+    def AdvanceInTime(self, current_time):
+        return self.mesh_solver.AdvanceInTime(current_time)
+
+    def GetComputingModelPart(self):
+        return self.mesh_solver.GetComputingModelPart()
+
+    def Initialize(self):
+        self.mesh_moving.Initialize()
+        self.mesh_solver.Initialize()
+
+    def InitializeSolutionStep(self):
+        self.mesh_moving.MoveMesh()
+        self.mesh_solver.InitializeSolutionStep()
+
+    def Predict(self):
+        self.mesh_solver.Predict()
+
+    def SolveSolutionStep(self):
+        return self.mesh_solver.SolveSolutionStep()
+
+    def FinalizeSolutionStep(self):
+        self.mesh_solver.FinalizeSolutionStep()
+        self.mesh_moving.MapResults()
+        SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.main_model_part)
+
+    def Finalize(self):
+        self.mesh_solver.Finalize()
+
+    def Check(self):
+        self.mesh_solver.Check()
+        self.mesh_moving.Check()
+
+    def Clear(self):
+        self.mesh_solver.Clear()
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        default_settings = KM.Parameters("""
+        {
+            "solver_type"              : "",
+            "model_part_name"          : "eulerian_model_part",
+            "echo_level"               : 0,
+            "mesh_solver_settings"     : {},
+            "mesh_moving_settings"     : {}
+        }""")
+        return default_settings
```

## KratosMultiphysics/ShallowWaterApplication/primitive_solver.py

 * *Ordering differences only*

```diff
@@ -1,18 +1,18 @@
-# importing the Kratos Library
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-## Import base class file
-from KratosMultiphysics.ShallowWaterApplication.wave_solver import WaveSolver
-
-def CreateSolver(model, custom_settings):
-    return PrimitiveSolver(model, custom_settings)
-
-class PrimitiveSolver(WaveSolver):
-
-    def _GetFormulationSettings(self):
-        order = self.settings["time_integration_order"].GetInt()
-        element_name = "PrimitiveElement"
-        condition_name = "PrimitiveCondition"
-        buffer_size = order + 1
-        return element_name, condition_name, buffer_size
+# importing the Kratos Library
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+## Import base class file
+from KratosMultiphysics.ShallowWaterApplication.wave_solver import WaveSolver
+
+def CreateSolver(model, custom_settings):
+    return PrimitiveSolver(model, custom_settings)
+
+class PrimitiveSolver(WaveSolver):
+
+    def _GetFormulationSettings(self):
+        order = self.settings["time_integration_order"].GetInt()
+        element_name = "PrimitiveElement"
+        condition_name = "PrimitiveCondition"
+        buffer_size = order + 1
+        return element_name, condition_name, buffer_size
```

## KratosMultiphysics/ShallowWaterApplication/set_initial_perturbation_process.py

 * *Ordering differences only*

```diff
@@ -1,64 +1,64 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-def Factory(settings, Model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return InitialPerturbationProcess(Model, settings["Parameters"])
-
-## This process sets the value of a scalar variable using the AssignScalarVariableProcess.
-class InitialPerturbationProcess(KM.Process):
-
-    def __init__(self, Model, settings):
-
-        KM.Process.__init__(self)
-
-        default_settings = KM.Parameters("""
-            {
-                "model_part_name"            : "main_model_part",
-                "interval"                   : [0.0, 0.0],
-                "source_type"                : "coordinates or model_part",
-                "source_coordinates"         : [0.0, 0.0, 0.0],
-                "source_model_part_name"     : "main_model_part.sub_model_part",
-                "variable_name"              : "FREE_SURFACE_ELEVATION",
-                "default_value"              : 0.0,
-                "distance_of_influence"      : 1.0,
-                "maximum_perturbation_value" : 1.0
-            }
-            """
-            )
-        settings.ValidateAndAssignDefaults(default_settings)
-
-        self.variable_name = settings["variable_name"].GetString()
-        self.model_part = Model[settings["model_part_name"].GetString()]
-        variable = KM.KratosGlobals.GetVariable(self.variable_name)
-
-        # Creation of the parameters for the c++ process
-        cpp_parameters = KM.Parameters("""{}""")
-        cpp_parameters.AddValue("default_value", settings["default_value"])
-        cpp_parameters.AddValue("distance_of_influence", settings["distance_of_influence"])
-        cpp_parameters.AddValue("maximum_perturbation_value", settings["maximum_perturbation_value"])
-
-        if settings["source_type"].GetString() == "coordinates":
-            # retrieving the position of the source
-            source_coordinates = settings["source_coordinates"].GetVector()
-            if (source_coordinates.Size() != 3):
-                raise Exception('The source_coordinates has to be provided with 3 coordinates! It has ', source_coordinates.Size())
-            node = KM.Node(1, source_coordinates[0], source_coordinates[1], source_coordinates[2])
-            # Construction of the process with one node
-            self.perturbation_process = SW.ApplyPerturbationFunctionToScalar(self.model_part, node, variable, cpp_parameters)
-
-        elif settings["source_type"].GetString() == "model_part":
-            # Construction of the process with a sub model part
-            source_model_part = Model[settings["source_model_part_name"].GetString()]
-            self.perturbation_process = SW.ApplyPerturbationFunctionToScalar(self.model_part, source_model_part.Nodes, variable, cpp_parameters)
-
-        else:
-            raise Exception("InitialPerturbationProcess: unknown source type")
-
-    def ExecuteInitialize(self):
-        self.perturbation_process.Execute()
-        if self.variable_name == "HEIGHT":
-            SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.model_part)
-        elif self.variable_name == "FREE_SURFACE_ELEVATION":
-            SW.ShallowWaterUtilities().ComputeHeightFromFreeSurface(self.model_part)
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+def Factory(settings, Model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return InitialPerturbationProcess(Model, settings["Parameters"])
+
+## This process sets the value of a scalar variable using the AssignScalarVariableProcess.
+class InitialPerturbationProcess(KM.Process):
+
+    def __init__(self, Model, settings):
+
+        KM.Process.__init__(self)
+
+        default_settings = KM.Parameters("""
+            {
+                "model_part_name"            : "main_model_part",
+                "interval"                   : [0.0, 0.0],
+                "source_type"                : "coordinates or model_part",
+                "source_coordinates"         : [0.0, 0.0, 0.0],
+                "source_model_part_name"     : "main_model_part.sub_model_part",
+                "variable_name"              : "FREE_SURFACE_ELEVATION",
+                "default_value"              : 0.0,
+                "distance_of_influence"      : 1.0,
+                "maximum_perturbation_value" : 1.0
+            }
+            """
+            )
+        settings.ValidateAndAssignDefaults(default_settings)
+
+        self.variable_name = settings["variable_name"].GetString()
+        self.model_part = Model[settings["model_part_name"].GetString()]
+        variable = KM.KratosGlobals.GetVariable(self.variable_name)
+
+        # Creation of the parameters for the c++ process
+        cpp_parameters = KM.Parameters("""{}""")
+        cpp_parameters.AddValue("default_value", settings["default_value"])
+        cpp_parameters.AddValue("distance_of_influence", settings["distance_of_influence"])
+        cpp_parameters.AddValue("maximum_perturbation_value", settings["maximum_perturbation_value"])
+
+        if settings["source_type"].GetString() == "coordinates":
+            # retrieving the position of the source
+            source_coordinates = settings["source_coordinates"].GetVector()
+            if (source_coordinates.Size() != 3):
+                raise Exception('The source_coordinates has to be provided with 3 coordinates! It has ', source_coordinates.Size())
+            node = KM.Node(1, source_coordinates[0], source_coordinates[1], source_coordinates[2])
+            # Construction of the process with one node
+            self.perturbation_process = SW.ApplyPerturbationFunctionToScalar(self.model_part, node, variable, cpp_parameters)
+
+        elif settings["source_type"].GetString() == "model_part":
+            # Construction of the process with a sub model part
+            source_model_part = Model[settings["source_model_part_name"].GetString()]
+            self.perturbation_process = SW.ApplyPerturbationFunctionToScalar(self.model_part, source_model_part.Nodes, variable, cpp_parameters)
+
+        else:
+            raise Exception("InitialPerturbationProcess: unknown source type")
+
+    def ExecuteInitialize(self):
+        self.perturbation_process.Execute()
+        if self.variable_name == "HEIGHT":
+            SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.model_part)
+        elif self.variable_name == "FREE_SURFACE_ELEVATION":
+            SW.ShallowWaterUtilities().ComputeHeightFromFreeSurface(self.model_part)
```

## KratosMultiphysics/ShallowWaterApplication/set_initial_water_level_process.py

 * *Ordering differences only*

```diff
@@ -1,53 +1,53 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-def Factory(settings, Model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return SetInitialWaterLevelProcess(Model, settings["Parameters"])
-
-## This process sets the value of a scalar variable using the AssignScalarVariableProcess.
-class SetInitialWaterLevelProcess(KM.Process):
-
-    def __init__(self, Model, settings):
-
-        KM.Process.__init__(self)
-
-        default_settings = KM.Parameters("""
-            {
-                "model_part_name"      : "please_specify_model_part_name",
-                "variable_name"        : "HEIGHT",
-                "constrained"          : false,
-                "interval"             : [0.0, 0.0],
-                "value"                : 1.0,
-                "set_minimum_height"   : true,
-                "minimum_height_value" : 1e-4
-            }
-            """
-            )
-        if settings.Has("value"):
-            if settings["value"].IsString():
-                default_settings["value"].SetString("1.0")
-        settings.ValidateAndAssignDefaults(default_settings)
-
-        self.variable = settings["variable_name"].GetString()
-        self.model_part = Model[settings["model_part_name"].GetString()]
-
-        self.set_minimum_height = settings["set_minimum_height"].GetBool()
-        self.minimum_height = settings["minimum_height_value"].GetDouble()
-        settings.RemoveValue("set_minimum_height")
-        settings.RemoveValue("minimum_height_value")
-
-        from KratosMultiphysics.assign_scalar_variable_process import AssignScalarVariableProcess
-        self.process = AssignScalarVariableProcess(Model, settings)
-
-    def ExecuteInitialize(self):
-        self.process.ExecuteInitializeSolutionStep()
-        if self.variable == "HEIGHT":
-            SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.model_part)
-        elif self.variable == "FREE_SURFACE_ELEVATION":
-            SW.ShallowWaterUtilities().ComputeHeightFromFreeSurface(self.model_part)
-
-        if self.set_minimum_height:
-            SW.ShallowWaterUtilities().SetMinimumValue(self.model_part, SW.HEIGHT, self.minimum_height)
-            SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.model_part)
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+def Factory(settings, Model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return SetInitialWaterLevelProcess(Model, settings["Parameters"])
+
+## This process sets the value of a scalar variable using the AssignScalarVariableProcess.
+class SetInitialWaterLevelProcess(KM.Process):
+
+    def __init__(self, Model, settings):
+
+        KM.Process.__init__(self)
+
+        default_settings = KM.Parameters("""
+            {
+                "model_part_name"      : "please_specify_model_part_name",
+                "variable_name"        : "HEIGHT",
+                "constrained"          : false,
+                "interval"             : [0.0, 0.0],
+                "value"                : 1.0,
+                "set_minimum_height"   : true,
+                "minimum_height_value" : 1e-4
+            }
+            """
+            )
+        if settings.Has("value"):
+            if settings["value"].IsString():
+                default_settings["value"].SetString("1.0")
+        settings.ValidateAndAssignDefaults(default_settings)
+
+        self.variable = settings["variable_name"].GetString()
+        self.model_part = Model[settings["model_part_name"].GetString()]
+
+        self.set_minimum_height = settings["set_minimum_height"].GetBool()
+        self.minimum_height = settings["minimum_height_value"].GetDouble()
+        settings.RemoveValue("set_minimum_height")
+        settings.RemoveValue("minimum_height_value")
+
+        from KratosMultiphysics.assign_scalar_variable_process import AssignScalarVariableProcess
+        self.process = AssignScalarVariableProcess(Model, settings)
+
+    def ExecuteInitialize(self):
+        self.process.ExecuteInitializeSolutionStep()
+        if self.variable == "HEIGHT":
+            SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.model_part)
+        elif self.variable == "FREE_SURFACE_ELEVATION":
+            SW.ShallowWaterUtilities().ComputeHeightFromFreeSurface(self.model_part)
+
+        if self.set_minimum_height:
+            SW.ShallowWaterUtilities().SetMinimumValue(self.model_part, SW.HEIGHT, self.minimum_height)
+            SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.model_part)
```

## KratosMultiphysics/ShallowWaterApplication/set_topography_process.py

 * *Ordering differences only*

```diff
@@ -1,53 +1,53 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-def Factory(settings, Model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return SetTopographyProcess(Model, settings["Parameters"])
-
-## This process sets the value of a scalar variable using the AssignScalarVariableProcess.
-class SetTopographyProcess(KM.Process):
-
-    def __init__(self, Model, settings):
-
-        KM.Process.__init__(self)
-
-        default_settings = KM.Parameters("""
-            {
-                "model_part_name"      : "please_specify_model_part_name",
-                "interval"             : [0.0, 1e30],
-                "constrained"          : false,
-                "value"                : 0.0,
-                "set_mesh_z_to_zero"   : true
-            }
-            """
-            )
-        if settings.Has("value"):
-            if settings["value"].IsString():
-                default_settings["value"].SetString("z")
-        settings.ValidateAndAssignDefaults(default_settings)
-        settings.AddEmptyValue("variable_name").SetString("TOPOGRAPHY")
-
-        self.model_part = Model[settings["model_part_name"].GetString()]
-        if settings["value"].IsString():
-            self.depends_on_time = settings["value"].GetString().find('t') != -1
-        else:
-            self.depends_on_time = False
-        self.set_mesh_z_to_zero = settings["set_mesh_z_to_zero"].GetBool()
-        process_settings = settings.Clone()
-        process_settings.RemoveValue("set_mesh_z_to_zero")
-
-        from KratosMultiphysics.assign_scalar_variable_process import AssignScalarVariableProcess
-        self.process = AssignScalarVariableProcess(Model, process_settings)
-
-    def ExecuteInitialize(self):
-        self.process.ExecuteInitializeSolutionStep()
-        SW.ShallowWaterUtilities().FlipScalarVariable(SW.TOPOGRAPHY, SW.BATHYMETRY, self.model_part)
-        if self.set_mesh_z_to_zero:
-            SW.ShallowWaterUtilities().SetMeshZCoordinateToZero(self.model_part)
-            SW.ShallowWaterUtilities().SetMeshZ0CoordinateToZero(self.model_part)
-
-    def ExecuteInitializeSolutionStep(self):
-        if self.depends_on_time:
-            self.ExecuteInitialize()
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+def Factory(settings, Model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return SetTopographyProcess(Model, settings["Parameters"])
+
+## This process sets the value of a scalar variable using the AssignScalarVariableProcess.
+class SetTopographyProcess(KM.Process):
+
+    def __init__(self, Model, settings):
+
+        KM.Process.__init__(self)
+
+        default_settings = KM.Parameters("""
+            {
+                "model_part_name"      : "please_specify_model_part_name",
+                "interval"             : [0.0, 1e30],
+                "constrained"          : false,
+                "value"                : 0.0,
+                "set_mesh_z_to_zero"   : true
+            }
+            """
+            )
+        if settings.Has("value"):
+            if settings["value"].IsString():
+                default_settings["value"].SetString("z")
+        settings.ValidateAndAssignDefaults(default_settings)
+        settings.AddEmptyValue("variable_name").SetString("TOPOGRAPHY")
+
+        self.model_part = Model[settings["model_part_name"].GetString()]
+        if settings["value"].IsString():
+            self.depends_on_time = settings["value"].GetString().find('t') != -1
+        else:
+            self.depends_on_time = False
+        self.set_mesh_z_to_zero = settings["set_mesh_z_to_zero"].GetBool()
+        process_settings = settings.Clone()
+        process_settings.RemoveValue("set_mesh_z_to_zero")
+
+        from KratosMultiphysics.assign_scalar_variable_process import AssignScalarVariableProcess
+        self.process = AssignScalarVariableProcess(Model, process_settings)
+
+    def ExecuteInitialize(self):
+        self.process.ExecuteInitializeSolutionStep()
+        SW.ShallowWaterUtilities().FlipScalarVariable(SW.TOPOGRAPHY, SW.BATHYMETRY, self.model_part)
+        if self.set_mesh_z_to_zero:
+            SW.ShallowWaterUtilities().SetMeshZCoordinateToZero(self.model_part)
+            SW.ShallowWaterUtilities().SetMeshZ0CoordinateToZero(self.model_part)
+
+    def ExecuteInitializeSolutionStep(self):
+        if self.depends_on_time:
+            self.ExecuteInitialize()
```

## KratosMultiphysics/ShallowWaterApplication/shallow_water_analysis.py

 * *Ordering differences only*

```diff
@@ -1,37 +1,37 @@
-# Importing Kratos
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-from KratosMultiphysics.analysis_stage import AnalysisStage
-
-from importlib import import_module
-
-class ShallowWaterAnalysis(AnalysisStage):
-    ''' Main script for shallow water simulations '''
-
-    def _CreateSolver(self):
-        python_module_name = "KratosMultiphysics.ShallowWaterApplication"
-        full_module_name = python_module_name + "." + self.project_parameters["solver_settings"]["solver_type"].GetString()
-        solver_module = import_module(full_module_name)
-        solver = solver_module.CreateSolver(self.model, self.project_parameters["solver_settings"])
-        return solver
-
-    def _GetOrderOfProcessesInitialization(self):
-        return ["topography_process_list",
-                "initial_conditions_process_list",
-                "boundary_conditions_process_list"]
-
-    def _GetSimulationName(self):
-        return "Shallow Water Analysis"
-
-if __name__ == "__main__":
-    import argparse
-    parser = argparse.ArgumentParser()
-    parser.add_argument("parameters_file_name", nargs="?", default="ProjectParameters.json")
-    args = parser.parse_args()
-
-    with open(args.parameters_file_name, 'r') as parameter_file:
-        parameters = KM.Parameters(parameter_file.read())
-
-    model = KM.Model()
-    ShallowWaterAnalysis(model, parameters).Run()
+# Importing Kratos
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+from KratosMultiphysics.analysis_stage import AnalysisStage
+
+from importlib import import_module
+
+class ShallowWaterAnalysis(AnalysisStage):
+    ''' Main script for shallow water simulations '''
+
+    def _CreateSolver(self):
+        python_module_name = "KratosMultiphysics.ShallowWaterApplication"
+        full_module_name = python_module_name + "." + self.project_parameters["solver_settings"]["solver_type"].GetString()
+        solver_module = import_module(full_module_name)
+        solver = solver_module.CreateSolver(self.model, self.project_parameters["solver_settings"])
+        return solver
+
+    def _GetOrderOfProcessesInitialization(self):
+        return ["topography_process_list",
+                "initial_conditions_process_list",
+                "boundary_conditions_process_list"]
+
+    def _GetSimulationName(self):
+        return "Shallow Water Analysis"
+
+if __name__ == "__main__":
+    import argparse
+    parser = argparse.ArgumentParser()
+    parser.add_argument("parameters_file_name", nargs="?", default="ProjectParameters.json")
+    args = parser.parse_args()
+
+    with open(args.parameters_file_name, 'r') as parameter_file:
+        parameters = KM.Parameters(parameter_file.read())
+
+    model = KM.Model()
+    ShallowWaterAnalysis(model, parameters).Run()
```

## KratosMultiphysics/ShallowWaterApplication/shallow_water_base_solver.py

 * *Ordering differences only*

```diff
@@ -1,294 +1,294 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KM
-from KratosMultiphysics.python_solver import PythonSolver
-import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
-
-# Import applications
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-def CreateSolver(model, custom_settings):
-    return ShallowWaterBaseSolver(model, custom_settings)
-
-class ShallowWaterBaseSolver(PythonSolver):
-    def __init__(self, model, settings):
-        super().__init__(model, settings)
-
-        ## Set the element and condition names for the replace settings
-        ## These should be defined in derived classes
-        self.element_name = None
-        self.condition_name = None
-        self.min_buffer_size = 2
-
-        # Either retrieve the model part from the model or create a new one
-        model_part_name = self.settings["model_part_name"].GetString()
-        self.main_model_part = self.model.CreateModelPart(model_part_name)
-
-        self._SetProcessInfo()
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        default_settings = KM.Parameters("""
-        {
-            "solver_type"              : "shallow_water_base_solver",
-            "model_part_name"          : "main_model_part",
-            "domain_size"              : 2,
-            "gravity"                  : 9.81,
-            "density"                  : 1000,
-            "model_import_settings"    : {
-                "input_type"               : "use_input_model_part"
-            },
-            "material_import_settings" :{
-                "materials_filename": ""
-            },
-            "echo_level"               : 0,
-            "convergence_criterion"    : "displacement",
-            "relative_tolerance"       : 1e-6,
-            "absolute_tolerance"       : 1e-9,
-            "maximum_iterations"       : 20,
-            "compute_reactions"        : false,
-            "reform_dofs_at_each_step" : false,
-            "move_mesh_flag"           : false,
-            "integrate_by_parts"       : false,
-            "linear_solver_settings"   : {
-                "solver_type"              : "amgcl"
-            },
-            "time_stepping"            : {
-                "automatic_time_step"      : false,
-                "time_step"                : 0.01
-            }
-        }""")
-        default_settings.AddMissingParameters(super().GetDefaultParameters())
-        return default_settings
-
-    def AddVariables(self):
-        self.main_model_part.AddNodalSolutionStepVariable(SW.HEIGHT)
-        self.main_model_part.AddNodalSolutionStepVariable(KM.MOMENTUM)
-        self.main_model_part.AddNodalSolutionStepVariable(KM.VELOCITY)
-        self.main_model_part.AddNodalSolutionStepVariable(KM.ACCELERATION)
-        self.main_model_part.AddNodalSolutionStepVariable(SW.VERTICAL_VELOCITY)
-        self.main_model_part.AddNodalSolutionStepVariable(SW.FREE_SURFACE_ELEVATION)
-        self.main_model_part.AddNodalSolutionStepVariable(SW.BATHYMETRY)
-        self.main_model_part.AddNodalSolutionStepVariable(SW.TOPOGRAPHY)
-        self.main_model_part.AddNodalSolutionStepVariable(SW.MANNING)
-        self.main_model_part.AddNodalSolutionStepVariable(SW.RAIN)
-        self.main_model_part.AddNodalSolutionStepVariable(KM.NORMAL)
-        self.main_model_part.AddNodalSolutionStepVariable(KM.DISTANCE)
-
-    def AddDofs(self):
-        raise Exception("Calling the base class instead of the derived one")
-
-    def ImportModelPart(self):
-        # we can use the default implementation in the base class
-        self._ImportModelPart(self.main_model_part,self.settings["model_import_settings"])
-
-    def PrepareModelPart(self):
-        if not self.main_model_part.ProcessInfo[KM.IS_RESTARTED]:
-            # Import material properties
-            materials_imported = self._ImportMaterials()
-            if materials_imported:
-                KM.Logger.PrintInfo(self.__class__.__name__, "Materials were successfully imported.")
-            else:
-                KM.Logger.PrintInfo(self.__class__.__name__, "Materials were not imported.")
-
-            ## Replace default elements and conditions
-            self._ReplaceElementsAndConditions()
-            ## Execute the check and prepare model process
-            self._ExecuteCheckAndPrepare()
-            ## Set buffer size
-            self.main_model_part.SetBufferSize(self.GetMinimumBufferSize())
-
-    def GetMinimumBufferSize(self):
-        return self.min_buffer_size
-
-    def GetComputingModelPart(self):
-        return self.main_model_part
-
-    def Initialize(self):
-        self._GetSolutionStrategy().Initialize()
-        KM.Logger.PrintInfo(self.__class__.__name__, "Initialization finished")
-
-    def AdvanceInTime(self, current_time):
-        current_time += self._GetEstimateDeltaTimeUtility().Execute()
-        self.main_model_part.CloneTimeStep(current_time)
-        self.main_model_part.ProcessInfo[KM.STEP] += 1
-        return current_time
-
-    def InitializeSolutionStep(self):
-        if self._TimeBufferIsInitialized():
-            self._GetSolutionStrategy().InitializeSolutionStep()
-
-    def Predict(self):
-        if self._TimeBufferIsInitialized():
-            self._GetSolutionStrategy().Predict()
-
-    def SolveSolutionStep(self):
-        if self._TimeBufferIsInitialized():
-            is_converged = self._GetSolutionStrategy().SolveSolutionStep()
-            if not is_converged:
-                KM.Logger.PrintInfo(self.__class__.__name__, "The solver did not converge")
-            return is_converged
-        else:
-            return True
-
-    def FinalizeSolutionStep(self):
-        if self._TimeBufferIsInitialized():
-            self._GetSolutionStrategy().FinalizeSolutionStep()
-
-    def Check(self):
-        self._GetSolutionStrategy().Check()
-
-    def Clear(self):
-        self._GetSolutionStrategy().Clear()
-
-    #### Specific internal functions ####
-
-    def _TimeBufferIsInitialized(self):
-        # We always have one extra old step (step 0, read from input)
-        return self.main_model_part.ProcessInfo[KM.STEP] + 1 >= self.GetMinimumBufferSize()
-
-    def _GetEstimateDeltaTimeUtility(self):
-        if not hasattr(self, '_delta_time_utility'):
-            self._delta_time_utility = self._CreateEstimateDeltaTimeUtility()
-        return self._delta_time_utility
-
-    def _CreateEstimateDeltaTimeUtility(self):
-        # The c++ utility manages all the time step settings
-        return SW.EstimateTimeStepUtility(self.GetComputingModelPart(), self.settings["time_stepping"])
-
-    def _SetProcessInfo(self):
-        self.main_model_part.ProcessInfo.SetValue(KM.STEP, 0)
-        self.main_model_part.ProcessInfo.SetValue(KM.DOMAIN_SIZE, self.settings["domain_size"].GetInt())
-        self.main_model_part.ProcessInfo.SetValue(KM.GRAVITY_Z, self.settings["gravity"].GetDouble())
-        self.main_model_part.ProcessInfo.SetValue(SW.INTEGRATE_BY_PARTS, self.settings["integrate_by_parts"].GetBool())
-
-    def _ImportMaterials(self):
-        # Add the properties from json file to model parts.
-        materials_filename = self.settings["material_import_settings"]["materials_filename"].GetString()
-        if (materials_filename != ""):
-            material_settings = KM.Parameters("""{"Parameters": {} }""")
-            material_settings["Parameters"].AddString("materials_filename", materials_filename)
-            KM.ReadMaterialsUtility(material_settings, self.model)
-            materials_imported = True
-        else:
-            materials_imported = False
-        return materials_imported
-
-    def _ReplaceElementsAndConditions(self):
-        ## Get number of nodes and domain size
-        elem_num_nodes = self.__get_geometry_num_nodes(self.GetComputingModelPart().Elements)
-        cond_num_nodes = self.__get_geometry_num_nodes(self.GetComputingModelPart().Conditions)
-        domain_size = self.main_model_part.ProcessInfo[KM.DOMAIN_SIZE]
-
-        ## Get the full names
-        new_elem_name = self.__append_geometry_name(self.element_name, domain_size, elem_num_nodes)
-        new_cond_name = self.__append_geometry_name(self.condition_name, domain_size, cond_num_nodes)
-
-        ## Set the element and condition names in the Json parameters
-        self.settings.AddValue("element_replace_settings", KM.Parameters("""{}"""))
-        self.settings["element_replace_settings"].AddEmptyValue("element_name").SetString(new_elem_name)
-        self.settings["element_replace_settings"].AddEmptyValue("condition_name").SetString(new_cond_name)
-
-        ## Call the replace elements and conditions process
-        KM.ReplaceElementsAndConditionsProcess(self.main_model_part, self.settings["element_replace_settings"]).Execute()
-
-    def _ExecuteCheckAndPrepare(self):
-        #verify the orientation of the skin in case of triangles mesh
-        elem_num_nodes = self.__get_geometry_num_nodes(self.GetComputingModelPart().Elements)
-        if elem_num_nodes == 3:
-            mesh_orientation = KM.TetrahedralMeshOrientationCheck
-            throw_errors = False
-            flags  = mesh_orientation.COMPUTE_NODAL_NORMALS.AsFalse()
-            flags |= mesh_orientation.COMPUTE_CONDITION_NORMALS.AsFalse()
-            flags |= mesh_orientation.ASSIGN_NEIGHBOUR_ELEMENTS_TO_CONDITIONS
-            KM.TetrahedralMeshOrientationCheck(self.GetComputingModelPart(), throw_errors, flags).Execute()
-        else:
-            KM.Logger.PrintWarning(self.__class__.__name__, "Orientation check not performed for quadrilateral or higher order geometries.")
-
-    def __get_geometry_num_nodes(self, container):
-        if len(container) != 0:
-            geometry_num_nodes = len(container.__iter__().__next__().GetNodes())
-        else:
-            geometry_num_nodes = 0
-        geometry_num_nodes = self.main_model_part.GetCommunicator().GetDataCommunicator().MaxAll(geometry_num_nodes)
-        return geometry_num_nodes
-
-    @staticmethod
-    def __append_geometry_name(base_name, domain_size, num_nodes):
-        if (base_name is not None):
-            return base_name + str(int(domain_size)) + "D" + str(int(num_nodes)) + "N"
-        else:
-            raise Exception("There is no element/condition name. Define the string variables in your derived solver.")
-
-    def _GetLinearSolver(self):
-        if not hasattr(self, '_linear_solver'):
-            self._linear_solver = self._CreateLinearSolver()
-        return self._linear_solver
-
-    def _GetBuilderAndSolver(self):
-        if not hasattr(self, '_builder_and_solver'):
-            self._builder_and_solver = self._CreateBuilderAndSolver()
-        return self._builder_and_solver
-
-    def _GetConvergenceCriterion(self):
-        if not hasattr(self, '_convergence_criterion'):
-            self._convergence_criterion = self._CreateConvergenceCriterion()
-        return self._convergence_criterion
-
-    def _GetScheme(self):
-        if not hasattr(self, '_scheme'):
-            self._scheme = self._CreateScheme()
-        return self._scheme
-
-    def _GetSolutionStrategy(self):
-        if not hasattr(self, '_solution_strategy'):
-            self._solution_strategy = self._CreateSolutionStrategy()
-        return self._solution_strategy
-
-    def _CreateLinearSolver(self):
-        linear_solver_configuration = self.settings["linear_solver_settings"]
-        return linear_solver_factory.ConstructSolver(linear_solver_configuration)
-
-    def _CreateBuilderAndSolver(self):
-        linear_solver = self._GetLinearSolver()
-        builder_and_solver = KM.ResidualBasedBlockBuilderAndSolver(linear_solver)
-        return builder_and_solver
-
-    def _CreateConvergenceCriterion(self):
-        convergence_criterion_type = self.settings["convergence_criterion"].GetString()
-        if convergence_criterion_type == "displacement":
-            convergence_criterion = KM.DisplacementCriteria(
-                self.settings["relative_tolerance"].GetDouble(),
-                self.settings["absolute_tolerance"].GetDouble())
-        elif convergence_criterion_type == "residual":
-            convergence_criterion = KM.ResidualCriteria(
-                self.settings["relative_tolerance"].GetDouble(),
-                self.settings["absolute_tolerance"].GetDouble())
-        else:
-            msg = "The displacement criterion specified is '{}'\n".format(convergence_criterion_type)
-            msg += "The following options are available:\n"
-            msg += "    - 'displacement'"
-            msg += "    - 'residual'"
-            raise Exception(msg)
-        convergence_criterion.SetEchoLevel(self.echo_level)
-        return convergence_criterion
-
-    def _CreateScheme(self):
-        time_scheme = KM.ResidualBasedIncrementalUpdateStaticScheme()
-        return time_scheme
-
-    def _CreateSolutionStrategy(self):
-        computing_model_part = self.GetComputingModelPart()
-        scheme = self._GetScheme()
-        convergence_criterion = self._GetConvergenceCriterion()
-        builder_and_solver = self._GetBuilderAndSolver()
-        strategy = KM.ResidualBasedNewtonRaphsonStrategy(
-            computing_model_part,
-            scheme,
-            convergence_criterion,
-            builder_and_solver,
-            self.settings["maximum_iterations"].GetInt(),
-            self.settings["compute_reactions"].GetBool(),
-            self.settings["reform_dofs_at_each_step"].GetBool(),
-            self.settings["move_mesh_flag"].GetBool())
-        strategy.SetEchoLevel(max(0, self.echo_level-1))
-        return strategy
+# Importing the Kratos Library
+import KratosMultiphysics as KM
+from KratosMultiphysics.python_solver import PythonSolver
+import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
+
+# Import applications
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+def CreateSolver(model, custom_settings):
+    return ShallowWaterBaseSolver(model, custom_settings)
+
+class ShallowWaterBaseSolver(PythonSolver):
+    def __init__(self, model, settings):
+        super().__init__(model, settings)
+
+        ## Set the element and condition names for the replace settings
+        ## These should be defined in derived classes
+        self.element_name = None
+        self.condition_name = None
+        self.min_buffer_size = 2
+
+        # Either retrieve the model part from the model or create a new one
+        model_part_name = self.settings["model_part_name"].GetString()
+        self.main_model_part = self.model.CreateModelPart(model_part_name)
+
+        self._SetProcessInfo()
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        default_settings = KM.Parameters("""
+        {
+            "solver_type"              : "shallow_water_base_solver",
+            "model_part_name"          : "main_model_part",
+            "domain_size"              : 2,
+            "gravity"                  : 9.81,
+            "density"                  : 1000,
+            "model_import_settings"    : {
+                "input_type"               : "use_input_model_part"
+            },
+            "material_import_settings" :{
+                "materials_filename": ""
+            },
+            "echo_level"               : 0,
+            "convergence_criterion"    : "displacement",
+            "relative_tolerance"       : 1e-6,
+            "absolute_tolerance"       : 1e-9,
+            "maximum_iterations"       : 20,
+            "compute_reactions"        : false,
+            "reform_dofs_at_each_step" : false,
+            "move_mesh_flag"           : false,
+            "integrate_by_parts"       : false,
+            "linear_solver_settings"   : {
+                "solver_type"              : "amgcl"
+            },
+            "time_stepping"            : {
+                "automatic_time_step"      : false,
+                "time_step"                : 0.01
+            }
+        }""")
+        default_settings.AddMissingParameters(super().GetDefaultParameters())
+        return default_settings
+
+    def AddVariables(self):
+        self.main_model_part.AddNodalSolutionStepVariable(SW.HEIGHT)
+        self.main_model_part.AddNodalSolutionStepVariable(KM.MOMENTUM)
+        self.main_model_part.AddNodalSolutionStepVariable(KM.VELOCITY)
+        self.main_model_part.AddNodalSolutionStepVariable(KM.ACCELERATION)
+        self.main_model_part.AddNodalSolutionStepVariable(SW.VERTICAL_VELOCITY)
+        self.main_model_part.AddNodalSolutionStepVariable(SW.FREE_SURFACE_ELEVATION)
+        self.main_model_part.AddNodalSolutionStepVariable(SW.BATHYMETRY)
+        self.main_model_part.AddNodalSolutionStepVariable(SW.TOPOGRAPHY)
+        self.main_model_part.AddNodalSolutionStepVariable(SW.MANNING)
+        self.main_model_part.AddNodalSolutionStepVariable(SW.RAIN)
+        self.main_model_part.AddNodalSolutionStepVariable(KM.NORMAL)
+        self.main_model_part.AddNodalSolutionStepVariable(KM.DISTANCE)
+
+    def AddDofs(self):
+        raise Exception("Calling the base class instead of the derived one")
+
+    def ImportModelPart(self):
+        # we can use the default implementation in the base class
+        self._ImportModelPart(self.main_model_part,self.settings["model_import_settings"])
+
+    def PrepareModelPart(self):
+        if not self.main_model_part.ProcessInfo[KM.IS_RESTARTED]:
+            # Import material properties
+            materials_imported = self._ImportMaterials()
+            if materials_imported:
+                KM.Logger.PrintInfo(self.__class__.__name__, "Materials were successfully imported.")
+            else:
+                KM.Logger.PrintInfo(self.__class__.__name__, "Materials were not imported.")
+
+            ## Replace default elements and conditions
+            self._ReplaceElementsAndConditions()
+            ## Execute the check and prepare model process
+            self._ExecuteCheckAndPrepare()
+            ## Set buffer size
+            self.main_model_part.SetBufferSize(self.GetMinimumBufferSize())
+
+    def GetMinimumBufferSize(self):
+        return self.min_buffer_size
+
+    def GetComputingModelPart(self):
+        return self.main_model_part
+
+    def Initialize(self):
+        self._GetSolutionStrategy().Initialize()
+        KM.Logger.PrintInfo(self.__class__.__name__, "Initialization finished")
+
+    def AdvanceInTime(self, current_time):
+        current_time += self._GetEstimateDeltaTimeUtility().Execute()
+        self.main_model_part.CloneTimeStep(current_time)
+        self.main_model_part.ProcessInfo[KM.STEP] += 1
+        return current_time
+
+    def InitializeSolutionStep(self):
+        if self._TimeBufferIsInitialized():
+            self._GetSolutionStrategy().InitializeSolutionStep()
+
+    def Predict(self):
+        if self._TimeBufferIsInitialized():
+            self._GetSolutionStrategy().Predict()
+
+    def SolveSolutionStep(self):
+        if self._TimeBufferIsInitialized():
+            is_converged = self._GetSolutionStrategy().SolveSolutionStep()
+            if not is_converged:
+                KM.Logger.PrintInfo(self.__class__.__name__, "The solver did not converge")
+            return is_converged
+        else:
+            return True
+
+    def FinalizeSolutionStep(self):
+        if self._TimeBufferIsInitialized():
+            self._GetSolutionStrategy().FinalizeSolutionStep()
+
+    def Check(self):
+        self._GetSolutionStrategy().Check()
+
+    def Clear(self):
+        self._GetSolutionStrategy().Clear()
+
+    #### Specific internal functions ####
+
+    def _TimeBufferIsInitialized(self):
+        # We always have one extra old step (step 0, read from input)
+        return self.main_model_part.ProcessInfo[KM.STEP] + 1 >= self.GetMinimumBufferSize()
+
+    def _GetEstimateDeltaTimeUtility(self):
+        if not hasattr(self, '_delta_time_utility'):
+            self._delta_time_utility = self._CreateEstimateDeltaTimeUtility()
+        return self._delta_time_utility
+
+    def _CreateEstimateDeltaTimeUtility(self):
+        # The c++ utility manages all the time step settings
+        return SW.EstimateTimeStepUtility(self.GetComputingModelPart(), self.settings["time_stepping"])
+
+    def _SetProcessInfo(self):
+        self.main_model_part.ProcessInfo.SetValue(KM.STEP, 0)
+        self.main_model_part.ProcessInfo.SetValue(KM.DOMAIN_SIZE, self.settings["domain_size"].GetInt())
+        self.main_model_part.ProcessInfo.SetValue(KM.GRAVITY_Z, self.settings["gravity"].GetDouble())
+        self.main_model_part.ProcessInfo.SetValue(SW.INTEGRATE_BY_PARTS, self.settings["integrate_by_parts"].GetBool())
+
+    def _ImportMaterials(self):
+        # Add the properties from json file to model parts.
+        materials_filename = self.settings["material_import_settings"]["materials_filename"].GetString()
+        if (materials_filename != ""):
+            material_settings = KM.Parameters("""{"Parameters": {} }""")
+            material_settings["Parameters"].AddString("materials_filename", materials_filename)
+            KM.ReadMaterialsUtility(material_settings, self.model)
+            materials_imported = True
+        else:
+            materials_imported = False
+        return materials_imported
+
+    def _ReplaceElementsAndConditions(self):
+        ## Get number of nodes and domain size
+        elem_num_nodes = self.__get_geometry_num_nodes(self.GetComputingModelPart().Elements)
+        cond_num_nodes = self.__get_geometry_num_nodes(self.GetComputingModelPart().Conditions)
+        domain_size = self.main_model_part.ProcessInfo[KM.DOMAIN_SIZE]
+
+        ## Get the full names
+        new_elem_name = self.__append_geometry_name(self.element_name, domain_size, elem_num_nodes)
+        new_cond_name = self.__append_geometry_name(self.condition_name, domain_size, cond_num_nodes)
+
+        ## Set the element and condition names in the Json parameters
+        self.settings.AddValue("element_replace_settings", KM.Parameters("""{}"""))
+        self.settings["element_replace_settings"].AddEmptyValue("element_name").SetString(new_elem_name)
+        self.settings["element_replace_settings"].AddEmptyValue("condition_name").SetString(new_cond_name)
+
+        ## Call the replace elements and conditions process
+        KM.ReplaceElementsAndConditionsProcess(self.main_model_part, self.settings["element_replace_settings"]).Execute()
+
+    def _ExecuteCheckAndPrepare(self):
+        #verify the orientation of the skin in case of triangles mesh
+        elem_num_nodes = self.__get_geometry_num_nodes(self.GetComputingModelPart().Elements)
+        if elem_num_nodes == 3:
+            mesh_orientation = KM.TetrahedralMeshOrientationCheck
+            throw_errors = False
+            flags  = mesh_orientation.COMPUTE_NODAL_NORMALS.AsFalse()
+            flags |= mesh_orientation.COMPUTE_CONDITION_NORMALS.AsFalse()
+            flags |= mesh_orientation.ASSIGN_NEIGHBOUR_ELEMENTS_TO_CONDITIONS
+            KM.TetrahedralMeshOrientationCheck(self.GetComputingModelPart(), throw_errors, flags).Execute()
+        else:
+            KM.Logger.PrintWarning(self.__class__.__name__, "Orientation check not performed for quadrilateral or higher order geometries.")
+
+    def __get_geometry_num_nodes(self, container):
+        if len(container) != 0:
+            geometry_num_nodes = len(container.__iter__().__next__().GetNodes())
+        else:
+            geometry_num_nodes = 0
+        geometry_num_nodes = self.main_model_part.GetCommunicator().GetDataCommunicator().MaxAll(geometry_num_nodes)
+        return geometry_num_nodes
+
+    @staticmethod
+    def __append_geometry_name(base_name, domain_size, num_nodes):
+        if (base_name is not None):
+            return base_name + str(int(domain_size)) + "D" + str(int(num_nodes)) + "N"
+        else:
+            raise Exception("There is no element/condition name. Define the string variables in your derived solver.")
+
+    def _GetLinearSolver(self):
+        if not hasattr(self, '_linear_solver'):
+            self._linear_solver = self._CreateLinearSolver()
+        return self._linear_solver
+
+    def _GetBuilderAndSolver(self):
+        if not hasattr(self, '_builder_and_solver'):
+            self._builder_and_solver = self._CreateBuilderAndSolver()
+        return self._builder_and_solver
+
+    def _GetConvergenceCriterion(self):
+        if not hasattr(self, '_convergence_criterion'):
+            self._convergence_criterion = self._CreateConvergenceCriterion()
+        return self._convergence_criterion
+
+    def _GetScheme(self):
+        if not hasattr(self, '_scheme'):
+            self._scheme = self._CreateScheme()
+        return self._scheme
+
+    def _GetSolutionStrategy(self):
+        if not hasattr(self, '_solution_strategy'):
+            self._solution_strategy = self._CreateSolutionStrategy()
+        return self._solution_strategy
+
+    def _CreateLinearSolver(self):
+        linear_solver_configuration = self.settings["linear_solver_settings"]
+        return linear_solver_factory.ConstructSolver(linear_solver_configuration)
+
+    def _CreateBuilderAndSolver(self):
+        linear_solver = self._GetLinearSolver()
+        builder_and_solver = KM.ResidualBasedBlockBuilderAndSolver(linear_solver)
+        return builder_and_solver
+
+    def _CreateConvergenceCriterion(self):
+        convergence_criterion_type = self.settings["convergence_criterion"].GetString()
+        if convergence_criterion_type == "displacement":
+            convergence_criterion = KM.DisplacementCriteria(
+                self.settings["relative_tolerance"].GetDouble(),
+                self.settings["absolute_tolerance"].GetDouble())
+        elif convergence_criterion_type == "residual":
+            convergence_criterion = KM.ResidualCriteria(
+                self.settings["relative_tolerance"].GetDouble(),
+                self.settings["absolute_tolerance"].GetDouble())
+        else:
+            msg = "The displacement criterion specified is '{}'\n".format(convergence_criterion_type)
+            msg += "The following options are available:\n"
+            msg += "    - 'displacement'"
+            msg += "    - 'residual'"
+            raise Exception(msg)
+        convergence_criterion.SetEchoLevel(self.echo_level)
+        return convergence_criterion
+
+    def _CreateScheme(self):
+        time_scheme = KM.ResidualBasedIncrementalUpdateStaticScheme()
+        return time_scheme
+
+    def _CreateSolutionStrategy(self):
+        computing_model_part = self.GetComputingModelPart()
+        scheme = self._GetScheme()
+        convergence_criterion = self._GetConvergenceCriterion()
+        builder_and_solver = self._GetBuilderAndSolver()
+        strategy = KM.ResidualBasedNewtonRaphsonStrategy(
+            computing_model_part,
+            scheme,
+            convergence_criterion,
+            builder_and_solver,
+            self.settings["maximum_iterations"].GetInt(),
+            self.settings["compute_reactions"].GetBool(),
+            self.settings["reform_dofs_at_each_step"].GetBool(),
+            self.settings["move_mesh_flag"].GetBool())
+        strategy.SetEchoLevel(max(0, self.echo_level-1))
+        return strategy
```

## KratosMultiphysics/ShallowWaterApplication/stabilized_shallow_water_solver.py

 * *Ordering differences only*

```diff
@@ -1,111 +1,111 @@
-# importing the Kratos Library
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-## Import base class file
-from KratosMultiphysics.ShallowWaterApplication.shallow_water_base_solver import ShallowWaterBaseSolver
-
-def CreateSolver(model, custom_settings):
-    return StabilizedShallowWaterSolver(model, custom_settings)
-
-class StabilizedShallowWaterSolver(ShallowWaterBaseSolver):
-    def __init__(self, model, settings):
-        super().__init__(model, settings)
-
-        self._SetUpFormulation()
-        self.min_buffer_size = self.settings["time_integration_order"].GetInt() + 1
-
-    def AddVariables(self):
-        super().AddVariables()
-        self.main_model_part.AddNodalSolutionStepVariable(SW.ATMOSPHERIC_PRESSURE)
-        self.main_model_part.AddNodalSolutionStepVariable(KM.MESH_ACCELERATION)
-        self.main_model_part.AddNodalSolutionStepVariable(SW.WIND)
-
-    def AddDofs(self):
-        KM.VariableUtils().AddDof(KM.MOMENTUM_X, self.main_model_part)
-        KM.VariableUtils().AddDof(KM.MOMENTUM_Y, self.main_model_part)
-        KM.VariableUtils().AddDof(SW.HEIGHT, self.main_model_part)
-        KM.Logger.PrintInfo(self.__class__.__name__, "Shallow water solver DOFs added correctly.")
-
-    def Initialize(self):
-        super().Initialize()
-        self.main_model_part.ProcessInfo.SetValue(SW.RELATIVE_DRY_HEIGHT, self.settings["relative_dry_height"].GetDouble())
-        self.main_model_part.ProcessInfo.SetValue(KM.STABILIZATION_FACTOR, self.settings["stabilization_factor"].GetDouble())
-        self.main_model_part.ProcessInfo.SetValue(SW.SHOCK_STABILIZATION_FACTOR, self.settings["shock_capturing_factor"].GetDouble())
-        self.main_model_part.ProcessInfo.SetValue(KM.DENSITY_AIR, 1e0)
-        self.main_model_part.ProcessInfo.SetValue(KM.DENSITY, 1e3)
-        self.main_model_part.ProcessInfo.SetValue(SW.INTEGRATE_BY_PARTS, False)
-        if self.compute_neighbours:
-            KM.GenericFindElementalNeighboursProcess(self.main_model_part).Execute()
-
-    def FinalizeSolutionStep(self):
-        super().FinalizeSolutionStep()
-        SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.main_model_part)
-        SW.ShallowWaterUtilities().ComputeVelocity(self.main_model_part, True)
-        self._CheckWaterLoss()
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        default_settings = KM.Parameters("""
-        {
-        "time_integration_order"     : 2,
-        "relative_dry_height"        : 0.1,
-        "stabilization_factor"       : 0.01,
-        "shock_capturing_factor"     : 1.0,
-        "shock_capturing_type"       : "residual_viscosity"
-        }
-        """)
-        default_settings.AddMissingParameters(super().GetDefaultParameters())
-        return default_settings
-
-    def _CreateScheme(self):
-        if self.add_flux_correction:
-            scheme_settings = KM.Parameters()
-            scheme_settings.AddStringArray("limiting_variables", ["FREE_SURFACE_ELEVATION","MOMENTUM"])
-            scheme_settings.AddValue("order", self.settings["time_integration_order"])
-            time_scheme = SW.FluxCorrectedShallowWaterScheme(scheme_settings)
-            if self.settings["shock_capturing_factor"].GetDouble() > 0.0:
-                KM.Logger.PrintInfo(self.__class__.__name__, "Detected a non-zero shock capturing factor and flux correction. The shock capturing factor will be ignored.")
-        else:
-            time_scheme = SW.ShallowWaterResidualBasedBDFScheme(self.settings["time_integration_order"].GetInt())
-        return time_scheme
-
-    def _InitializeWaterLoss(self):
-        self.initial_water = KM.VariableUtils().SumHistoricalNodeScalarVariable(SW.HEIGHT, self.main_model_part,0)
-        self.initial_water /= self.main_model_part.NumberOfNodes()
-
-    def _CheckWaterLoss(self):
-        if not hasattr(self, 'initial_water'):
-            self._InitializeWaterLoss()
-        total_water = KM.VariableUtils().SumHistoricalNodeScalarVariable(SW.HEIGHT, self.main_model_part,0)
-        total_water /= self.main_model_part.NumberOfNodes()
-        water_loss = (total_water - self.initial_water) / self.initial_water
-        if abs(water_loss) > 1e-3 and self.echo_level > 1:
-            msg = "Water loss : {} %"
-            KM.Logger.PrintWarning(self.__class__.__name__, msg.format(water_loss*100))
-
-    def _SetUpFormulation(self):
-        shock_capturing_type = self.settings["shock_capturing_type"].GetString()
-        if  shock_capturing_type == "residual_viscosity":
-            self.element_name = "ConservativeElementRV"
-            self.condition_name = "ConservativeCondition"
-            self.compute_neighbours = False
-            self.add_flux_correction = False
-        elif shock_capturing_type == "flux_correction":
-            self.element_name = "ConservativeElementFC"
-            self.condition_name = "ConservativeCondition"
-            self.compute_neighbours = False
-            self.add_flux_correction = True
-        elif shock_capturing_type == "gradient_jump":
-            self.element_name = "ConservativeElementGJ"
-            self.condition_name = "ConservativeCondition"
-            self.compute_neighbours = True
-            self.add_flux_correction = False
-        else:
-            msg  = "StabilizedShallowWaterSolver._SetUpFormulation:\n"
-            msg += "The specified 'shock_capturing_type' : '{}' is not available.\n".format(shock_capturing_type)
-            msg += "The possible options are:\n"
-            msg += "\t- 'residual_viscosity'\n"
-            msg += "\t- 'flux_correction'\n"
-            msg += "\t- 'gradient_jump'\n"
-            raise Exception(msg)
+# importing the Kratos Library
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+## Import base class file
+from KratosMultiphysics.ShallowWaterApplication.shallow_water_base_solver import ShallowWaterBaseSolver
+
+def CreateSolver(model, custom_settings):
+    return StabilizedShallowWaterSolver(model, custom_settings)
+
+class StabilizedShallowWaterSolver(ShallowWaterBaseSolver):
+    def __init__(self, model, settings):
+        super().__init__(model, settings)
+
+        self._SetUpFormulation()
+        self.min_buffer_size = self.settings["time_integration_order"].GetInt() + 1
+
+    def AddVariables(self):
+        super().AddVariables()
+        self.main_model_part.AddNodalSolutionStepVariable(SW.ATMOSPHERIC_PRESSURE)
+        self.main_model_part.AddNodalSolutionStepVariable(KM.MESH_ACCELERATION)
+        self.main_model_part.AddNodalSolutionStepVariable(SW.WIND)
+
+    def AddDofs(self):
+        KM.VariableUtils().AddDof(KM.MOMENTUM_X, self.main_model_part)
+        KM.VariableUtils().AddDof(KM.MOMENTUM_Y, self.main_model_part)
+        KM.VariableUtils().AddDof(SW.HEIGHT, self.main_model_part)
+        KM.Logger.PrintInfo(self.__class__.__name__, "Shallow water solver DOFs added correctly.")
+
+    def Initialize(self):
+        super().Initialize()
+        self.main_model_part.ProcessInfo.SetValue(SW.RELATIVE_DRY_HEIGHT, self.settings["relative_dry_height"].GetDouble())
+        self.main_model_part.ProcessInfo.SetValue(KM.STABILIZATION_FACTOR, self.settings["stabilization_factor"].GetDouble())
+        self.main_model_part.ProcessInfo.SetValue(SW.SHOCK_STABILIZATION_FACTOR, self.settings["shock_capturing_factor"].GetDouble())
+        self.main_model_part.ProcessInfo.SetValue(KM.DENSITY_AIR, 1e0)
+        self.main_model_part.ProcessInfo.SetValue(KM.DENSITY, 1e3)
+        self.main_model_part.ProcessInfo.SetValue(SW.INTEGRATE_BY_PARTS, False)
+        if self.compute_neighbours:
+            KM.GenericFindElementalNeighboursProcess(self.main_model_part).Execute()
+
+    def FinalizeSolutionStep(self):
+        super().FinalizeSolutionStep()
+        SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.main_model_part)
+        SW.ShallowWaterUtilities().ComputeVelocity(self.main_model_part, True)
+        self._CheckWaterLoss()
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        default_settings = KM.Parameters("""
+        {
+        "time_integration_order"     : 2,
+        "relative_dry_height"        : 0.1,
+        "stabilization_factor"       : 0.01,
+        "shock_capturing_factor"     : 1.0,
+        "shock_capturing_type"       : "residual_viscosity"
+        }
+        """)
+        default_settings.AddMissingParameters(super().GetDefaultParameters())
+        return default_settings
+
+    def _CreateScheme(self):
+        if self.add_flux_correction:
+            scheme_settings = KM.Parameters()
+            scheme_settings.AddStringArray("limiting_variables", ["FREE_SURFACE_ELEVATION","MOMENTUM"])
+            scheme_settings.AddValue("order", self.settings["time_integration_order"])
+            time_scheme = SW.FluxCorrectedShallowWaterScheme(scheme_settings)
+            if self.settings["shock_capturing_factor"].GetDouble() > 0.0:
+                KM.Logger.PrintInfo(self.__class__.__name__, "Detected a non-zero shock capturing factor and flux correction. The shock capturing factor will be ignored.")
+        else:
+            time_scheme = SW.ShallowWaterResidualBasedBDFScheme(self.settings["time_integration_order"].GetInt())
+        return time_scheme
+
+    def _InitializeWaterLoss(self):
+        self.initial_water = KM.VariableUtils().SumHistoricalNodeScalarVariable(SW.HEIGHT, self.main_model_part,0)
+        self.initial_water /= self.main_model_part.NumberOfNodes()
+
+    def _CheckWaterLoss(self):
+        if not hasattr(self, 'initial_water'):
+            self._InitializeWaterLoss()
+        total_water = KM.VariableUtils().SumHistoricalNodeScalarVariable(SW.HEIGHT, self.main_model_part,0)
+        total_water /= self.main_model_part.NumberOfNodes()
+        water_loss = (total_water - self.initial_water) / self.initial_water
+        if abs(water_loss) > 1e-3 and self.echo_level > 1:
+            msg = "Water loss : {} %"
+            KM.Logger.PrintWarning(self.__class__.__name__, msg.format(water_loss*100))
+
+    def _SetUpFormulation(self):
+        shock_capturing_type = self.settings["shock_capturing_type"].GetString()
+        if  shock_capturing_type == "residual_viscosity":
+            self.element_name = "ConservativeElementRV"
+            self.condition_name = "ConservativeCondition"
+            self.compute_neighbours = False
+            self.add_flux_correction = False
+        elif shock_capturing_type == "flux_correction":
+            self.element_name = "ConservativeElementFC"
+            self.condition_name = "ConservativeCondition"
+            self.compute_neighbours = False
+            self.add_flux_correction = True
+        elif shock_capturing_type == "gradient_jump":
+            self.element_name = "ConservativeElementGJ"
+            self.condition_name = "ConservativeCondition"
+            self.compute_neighbours = True
+            self.add_flux_correction = False
+        else:
+            msg  = "StabilizedShallowWaterSolver._SetUpFormulation:\n"
+            msg += "The specified 'shock_capturing_type' : '{}' is not available.\n".format(shock_capturing_type)
+            msg += "The possible options are:\n"
+            msg += "\t- 'residual_viscosity'\n"
+            msg += "\t- 'flux_correction'\n"
+            msg += "\t- 'gradient_jump'\n"
+            raise Exception(msg)
```

## KratosMultiphysics/ShallowWaterApplication/wave_generator_process.py

 * *Ordering differences only*

```diff
@@ -1,119 +1,119 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-from KratosMultiphysics.ShallowWaterApplication.utilities.wave_factory import WaveTheoryFactory
-
-
-def Factory(settings, Model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return WaveGeneratorProcess(Model, settings["Parameters"])
-
-
-class WaveGeneratorProcess(KM.Process):
-
-    @staticmethod
-    def GetDefaultParameters():
-        """Default parameters for wave generator process.
-
-        A zero value in the wave specifications will be ignored.
-        The direction can be specified with a vector or the 'normal' keyword. If the direction is missing,
-        it will be taken as the normal to the boundary.
-        """
-        return KM.Parameters("""{
-            "model_part_name"          : "model_part",
-            "interval"                 : [0.0, "End"],
-            "direction"                : [0.0, 0.0, 0.0],
-            "normal_positive_outwards" : true,
-            "smooth_time"              : 0.0,
-            "wave_specifications"      : {
-                "wave_theory"               : "boussinesq",
-                "period"                    : 0.0,
-                "wavelength"                : 0.0,
-                "amplitude"                 : 0.0,
-                "get_depth_from_model_part" : true
-            }
-        }""")
-
-
-    def __init__(self, model, settings ):
-        """"""
-        KM.Process.__init__(self)
-
-        # Check if the direction is specified by 'normal'
-        self.settings = settings
-        self.direction_by_normal = False
-        if self.settings.Has("direction"):
-            if self.settings["direction"].IsString():
-                if self.settings["direction"].GetString() == "normal":
-                    self.settings["direction"].SetVector(KM.Vector(3))
-                    self.direction_by_normal = True
-        else:
-            self.direction_by_normal = True
-
-        # Overwrite the default settings with user-provided parameters
-        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
-
-        # Get the custom settings
-        self.model_part = model[self.settings["model_part_name"].GetString()]
-        self.interval = KM.IntervalUtility(self.settings)
-        variables_names_list = KM.SpecificationsUtilities.GetDofsListFromConditionsSpecifications(self.model_part)
-        self.variables_to_fix = []
-        self.compute_momentum = False
-        for variable_name in variables_names_list:
-            if variable_name.startswith("VELOCITY") or variable_name.startswith("MOMENTUM"):
-                variable = KM.KratosGlobals.GetVariable(variable_name)
-                self.variables_to_fix.append(variable)
-            if variable_name.startswith("MOMENTUM"):
-                self.compute_momentum = True
-
-
-    def ExecuteInitialize(self):
-        """Initialize the wave theory and the periodic function."""
-
-        # Check the direction
-        if self.direction_by_normal:
-            direction = self._CalculateUnitNormal()
-            if self.settings["normal_positive_outwards"].GetBool():
-                direction *= -1
-            self.settings["direction"].SetVector(direction)
-
-        # Setup the wave theory
-        wave_settings = self.settings["wave_specifications"]
-        wave_theory = WaveTheoryFactory(self.model_part, wave_settings)
-
-        # Creation of the parameters for the c++ process
-        velocity_parameters = KM.Parameters("""{}""")
-        velocity_parameters.AddDouble("amplitude", wave_theory.horizontal_velocity)
-        velocity_parameters.AddDouble("wavelength", wave_theory.wavelength)
-        velocity_parameters.AddDouble("period", wave_theory.period)
-        velocity_parameters.AddValue("phase", self.settings["wave_specifications"]["t_shift"])
-        velocity_parameters.AddValue("shift", self.settings["wave_specifications"]["x_shift"])
-        velocity_parameters.AddValue("direction", self.settings["direction"])
-        velocity_parameters.AddValue("smooth_time", self.settings["smooth_time"])
-        velocity_parameters.AddValue("smooth_time_centers", self.settings["interval"])
-        self.velocity_process = SW.ApplySinusoidalFunctionToVector(self.model_part, KM.VELOCITY, velocity_parameters)
-
-
-    def Check(self):
-        self.velocity_process.Check()
-
-
-    def ExecuteInitializeSolutionStep(self):
-        if self._IsInInterval():
-            self.velocity_process.ExecuteInitializeSolutionStep()
-            if self.compute_momentum:
-                SW.ShallowWaterUtilities().ComputeMomentum(self.model_part)
-            for variable in self.variables_to_fix:
-                KM.VariableUtils().ApplyFixity(variable, True, self.model_part.Nodes)
-
-
-    def _IsInInterval(self):
-        """Returns if we are inside the time interval or not."""
-        current_time = self.model_part.ProcessInfo[KM.TIME]
-        return self.interval.IsInInterval(current_time)
-
-
-    def _CalculateUnitNormal(self):
-        geometry = self.model_part.Conditions.__iter__().__next__().GetGeometry()
-        normal = geometry.UnitNormal()
-        return normal
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+from KratosMultiphysics.ShallowWaterApplication.utilities.wave_factory import WaveTheoryFactory
+
+
+def Factory(settings, Model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return WaveGeneratorProcess(Model, settings["Parameters"])
+
+
+class WaveGeneratorProcess(KM.Process):
+
+    @staticmethod
+    def GetDefaultParameters():
+        """Default parameters for wave generator process.
+
+        A zero value in the wave specifications will be ignored.
+        The direction can be specified with a vector or the 'normal' keyword. If the direction is missing,
+        it will be taken as the normal to the boundary.
+        """
+        return KM.Parameters("""{
+            "model_part_name"          : "model_part",
+            "interval"                 : [0.0, "End"],
+            "direction"                : [0.0, 0.0, 0.0],
+            "normal_positive_outwards" : true,
+            "smooth_time"              : 0.0,
+            "wave_specifications"      : {
+                "wave_theory"               : "boussinesq",
+                "period"                    : 0.0,
+                "wavelength"                : 0.0,
+                "amplitude"                 : 0.0,
+                "get_depth_from_model_part" : true
+            }
+        }""")
+
+
+    def __init__(self, model, settings ):
+        """"""
+        KM.Process.__init__(self)
+
+        # Check if the direction is specified by 'normal'
+        self.settings = settings
+        self.direction_by_normal = False
+        if self.settings.Has("direction"):
+            if self.settings["direction"].IsString():
+                if self.settings["direction"].GetString() == "normal":
+                    self.settings["direction"].SetVector(KM.Vector(3))
+                    self.direction_by_normal = True
+        else:
+            self.direction_by_normal = True
+
+        # Overwrite the default settings with user-provided parameters
+        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
+
+        # Get the custom settings
+        self.model_part = model[self.settings["model_part_name"].GetString()]
+        self.interval = KM.IntervalUtility(self.settings)
+        variables_names_list = KM.SpecificationsUtilities.GetDofsListFromConditionsSpecifications(self.model_part)
+        self.variables_to_fix = []
+        self.compute_momentum = False
+        for variable_name in variables_names_list:
+            if variable_name.startswith("VELOCITY") or variable_name.startswith("MOMENTUM"):
+                variable = KM.KratosGlobals.GetVariable(variable_name)
+                self.variables_to_fix.append(variable)
+            if variable_name.startswith("MOMENTUM"):
+                self.compute_momentum = True
+
+
+    def ExecuteInitialize(self):
+        """Initialize the wave theory and the periodic function."""
+
+        # Check the direction
+        if self.direction_by_normal:
+            direction = self._CalculateUnitNormal()
+            if self.settings["normal_positive_outwards"].GetBool():
+                direction *= -1
+            self.settings["direction"].SetVector(direction)
+
+        # Setup the wave theory
+        wave_settings = self.settings["wave_specifications"]
+        wave_theory = WaveTheoryFactory(self.model_part, wave_settings)
+
+        # Creation of the parameters for the c++ process
+        velocity_parameters = KM.Parameters("""{}""")
+        velocity_parameters.AddDouble("amplitude", wave_theory.horizontal_velocity)
+        velocity_parameters.AddDouble("wavelength", wave_theory.wavelength)
+        velocity_parameters.AddDouble("period", wave_theory.period)
+        velocity_parameters.AddValue("phase", self.settings["wave_specifications"]["t_shift"])
+        velocity_parameters.AddValue("shift", self.settings["wave_specifications"]["x_shift"])
+        velocity_parameters.AddValue("direction", self.settings["direction"])
+        velocity_parameters.AddValue("smooth_time", self.settings["smooth_time"])
+        velocity_parameters.AddValue("smooth_time_centers", self.settings["interval"])
+        self.velocity_process = SW.ApplySinusoidalFunctionToVector(self.model_part, KM.VELOCITY, velocity_parameters)
+
+
+    def Check(self):
+        self.velocity_process.Check()
+
+
+    def ExecuteInitializeSolutionStep(self):
+        if self._IsInInterval():
+            self.velocity_process.ExecuteInitializeSolutionStep()
+            if self.compute_momentum:
+                SW.ShallowWaterUtilities().ComputeMomentum(self.model_part)
+            for variable in self.variables_to_fix:
+                KM.VariableUtils().ApplyFixity(variable, True, self.model_part.Nodes)
+
+
+    def _IsInInterval(self):
+        """Returns if we are inside the time interval or not."""
+        current_time = self.model_part.ProcessInfo[KM.TIME]
+        return self.interval.IsInInterval(current_time)
+
+
+    def _CalculateUnitNormal(self):
+        geometry = self.model_part.Conditions.__iter__().__next__().GetGeometry()
+        normal = geometry.UnitNormal()
+        return normal
```

## KratosMultiphysics/ShallowWaterApplication/wave_solver.py

 * *Ordering differences only*

```diff
@@ -1,68 +1,68 @@
-# importing the Kratos Library
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-## Import base class file
-from KratosMultiphysics.ShallowWaterApplication.shallow_water_base_solver import ShallowWaterBaseSolver
-
-def CreateSolver(model, custom_settings):
-    return WaveSolver(model, custom_settings)
-
-class WaveSolver(ShallowWaterBaseSolver):
-    def __init__(self, model, settings):
-        super().__init__(model, settings)
-        self.element_name, self.condition_name, self.min_buffer_size = self._GetFormulationSettings()
-
-    def AddDofs(self):
-        KM.VariableUtils().AddDof(KM.VELOCITY_X, self.main_model_part)
-        KM.VariableUtils().AddDof(KM.VELOCITY_Y, self.main_model_part)
-        KM.VariableUtils().AddDof(SW.HEIGHT, self.main_model_part)
-        KM.Logger.PrintInfo(self.__class__.__name__, "Shallow water primitive DOFs added correctly.")
-
-    def FinalizeSolutionStep(self):
-        super().FinalizeSolutionStep()
-        SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.main_model_part)
-
-    def _SetProcessInfo(self):
-        super()._SetProcessInfo()
-        self.main_model_part.ProcessInfo.SetValue(KM.STABILIZATION_FACTOR, self.settings["stabilization_factor"].GetDouble())
-        self.main_model_part.ProcessInfo.SetValue(SW.RELATIVE_DRY_HEIGHT, self.settings["relative_dry_height"].GetDouble())
-
-    def _GetFormulationSettings(self):
-        scheme = self.settings["time_integration_scheme"].GetString()
-        order = self.settings["time_integration_order"].GetInt()
-        if scheme == "bdf":
-            element_name = "WaveElement"
-            condition_name = "WaveCondition"
-            buffer_size = order + 1
-        elif scheme == "crank_nicolson":
-            element_name = "CrankNicolsonWaveElement"
-            condition_name = "WaveCondition"
-            buffer_size = 2
-            if not order == 2:
-                KM.Logger.PrintWarning('WaveSolver', 'Setting the "time_integration_order" to 2')
-        else:
-            raise Exception('The possible "time_integration_scheme" are "bdf" and "crank_nicolson"')
-        return element_name, condition_name, buffer_size
-
-    def _CreateScheme(self):
-        scheme = self.settings["time_integration_scheme"].GetString()
-        if scheme == "bdf":
-            scheme_settings = KM.Parameters()
-            scheme_settings.AddStringArray("solution_variables", ["VELOCITY","HEIGHT"])
-            scheme_settings.AddValue("integration_order", self.settings["time_integration_order"])
-            time_scheme = SW.ShallowWaterResidualBasedBDFScheme(scheme_settings)
-        else:
-            time_scheme = KM.ResidualBasedIncrementalUpdateStaticScheme()
-        return time_scheme
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        default_settings = KM.Parameters("""{
-            "time_integration_scheme"    : "bdf",
-            "time_integration_order"     : 2,
-            "relative_dry_height"        : 0.1,
-            "stabilization_factor"       : 0.01
-        }""")
-        default_settings.AddMissingParameters(super().GetDefaultParameters())
-        return default_settings
+# importing the Kratos Library
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+## Import base class file
+from KratosMultiphysics.ShallowWaterApplication.shallow_water_base_solver import ShallowWaterBaseSolver
+
+def CreateSolver(model, custom_settings):
+    return WaveSolver(model, custom_settings)
+
+class WaveSolver(ShallowWaterBaseSolver):
+    def __init__(self, model, settings):
+        super().__init__(model, settings)
+        self.element_name, self.condition_name, self.min_buffer_size = self._GetFormulationSettings()
+
+    def AddDofs(self):
+        KM.VariableUtils().AddDof(KM.VELOCITY_X, self.main_model_part)
+        KM.VariableUtils().AddDof(KM.VELOCITY_Y, self.main_model_part)
+        KM.VariableUtils().AddDof(SW.HEIGHT, self.main_model_part)
+        KM.Logger.PrintInfo(self.__class__.__name__, "Shallow water primitive DOFs added correctly.")
+
+    def FinalizeSolutionStep(self):
+        super().FinalizeSolutionStep()
+        SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.main_model_part)
+
+    def _SetProcessInfo(self):
+        super()._SetProcessInfo()
+        self.main_model_part.ProcessInfo.SetValue(KM.STABILIZATION_FACTOR, self.settings["stabilization_factor"].GetDouble())
+        self.main_model_part.ProcessInfo.SetValue(SW.RELATIVE_DRY_HEIGHT, self.settings["relative_dry_height"].GetDouble())
+
+    def _GetFormulationSettings(self):
+        scheme = self.settings["time_integration_scheme"].GetString()
+        order = self.settings["time_integration_order"].GetInt()
+        if scheme == "bdf":
+            element_name = "WaveElement"
+            condition_name = "WaveCondition"
+            buffer_size = order + 1
+        elif scheme == "crank_nicolson":
+            element_name = "CrankNicolsonWaveElement"
+            condition_name = "WaveCondition"
+            buffer_size = 2
+            if not order == 2:
+                KM.Logger.PrintWarning('WaveSolver', 'Setting the "time_integration_order" to 2')
+        else:
+            raise Exception('The possible "time_integration_scheme" are "bdf" and "crank_nicolson"')
+        return element_name, condition_name, buffer_size
+
+    def _CreateScheme(self):
+        scheme = self.settings["time_integration_scheme"].GetString()
+        if scheme == "bdf":
+            scheme_settings = KM.Parameters()
+            scheme_settings.AddStringArray("solution_variables", ["VELOCITY","HEIGHT"])
+            scheme_settings.AddValue("integration_order", self.settings["time_integration_order"])
+            time_scheme = SW.ShallowWaterResidualBasedBDFScheme(scheme_settings)
+        else:
+            time_scheme = KM.ResidualBasedIncrementalUpdateStaticScheme()
+        return time_scheme
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        default_settings = KM.Parameters("""{
+            "time_integration_scheme"    : "bdf",
+            "time_integration_order"     : 2,
+            "relative_dry_height"        : 0.1,
+            "stabilization_factor"       : 0.01
+        }""")
+        default_settings.AddMissingParameters(super().GetDefaultParameters())
+        return default_settings
```

## KratosMultiphysics/ShallowWaterApplication/benchmarks/base_benchmark_process.py

 * *Ordering differences only*

```diff
@@ -1,119 +1,119 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return BaseBenchmarkProcess(model, settings["Parameters"])
-
-class BaseBenchmarkProcess(KM.Process):
-    """The base class for the benchmarks."""
-
-    def __init__(self, model, settings ):
-        """The constructor of the BaseBenchmarkProcess.
-
-        It is intended to be called from the constructor of deriving classes.
-        """
-
-        super().__init__()
-
-        self.model = model
-        self.settings = settings
-
-        default_settings = KM.Parameters("""
-            {
-                "model_part_name"      : "model_part",
-                "variables_list"       : [],
-                "exact_variables_list" : [],
-                "error_variables_list" : [],
-                "benchmark_settings"   : {}
-            }
-            """
-            )
-        default_settings["benchmark_settings"] = self._GetBenchmarkDefaultSettings()
-        self.settings.RecursivelyValidateAndAssignDefaults(default_settings)
-
-        self.model_part = self.model[self.settings["model_part_name"].GetString()]
-        self.variables = GenerateVariableListFromInput(self.settings["variables_list"])
-        self.exact_variables = GenerateVariableListFromInput(self.settings["exact_variables_list"])
-        self.error_variables = GenerateVariableListFromInput(self.settings["error_variables_list"])
-
-
-    def ExecuteInitialize(self):
-        """Set the topography and the initial conditions."""
-        KM.Timer.Start("Benchmark/Initial state")
-        time = self.model_part.ProcessInfo[KM.TIME]
-        for node in self.model_part.Nodes:
-            if self._Topography(node):
-                node.SetSolutionStepValue(SW.TOPOGRAPHY, self._Topography(node))
-            node.SetSolutionStepValue(SW.HEIGHT, self._Height(node, time))
-            node.SetSolutionStepValue(KM.VELOCITY, self._Velocity(node, time))
-            node.SetSolutionStepValue(KM.MOMENTUM, self._Momentum(node, time))
-            node.SetSolutionStepValue(SW.FREE_SURFACE_ELEVATION, self._FreeSurfaceElevation(node, time))
-        KM.Timer.Stop("Benchmark/Initial state")
-
-
-    def ExecuteBeforeOutputStep(self):
-        """Compute the exact values of the benchmark and the error of the simulation."""
-        KM.Timer.Start("Benchmark/Exact values")
-        time = self.model_part.ProcessInfo[KM.TIME]
-        for (variable, exact_variable, error_variable) in zip(self.variables, self.exact_variables, self.error_variables):
-
-            if variable == SW.HEIGHT:
-                exact_value_function = self._Height
-            elif variable == KM.VELOCITY:
-                exact_value_function = self._Velocity
-            elif variable == KM.MOMENTUM:
-                exact_value_function = self._Momentum
-            elif variable == SW.FREE_SURFACE_ELEVATION:
-                exact_value_function = self._FreeSurfaceElevation
-
-            for node in self.model_part.Nodes:
-                exact_value = exact_value_function(node, time)
-                fem_value = node.GetSolutionStepValue(variable)
-
-                node.SetValue(exact_variable, exact_value)
-                node.SetValue(error_variable, fem_value - exact_value)
-        KM.Timer.Stop("Benchmark/Exact values")
-
-
-    def Check(self):
-        """Check if the input values have physical sense."""
-
-        if len(self.variables) != len(self.exact_variables):
-            raise Exception("The input variables list does not match the input exact variables list")
-
-        if len(self.variables) != len(self.error_variables):
-            raise Exception("The input variables list does not match the input error variables list")
-
-        for (var, exact, error) in zip(self.variables, self.exact_variables, self.error_variables):
-            if KM.KratosGlobals.GetVariableType(var.Name()) != KM.KratosGlobals.GetVariableType(exact.Name()):
-                msg = var.Name() + " variable type does not match the " + exact.Name() + " variable type"
-                raise Exception(msg)
-
-            if KM.KratosGlobals.GetVariableType(var.Name()) != KM.KratosGlobals.GetVariableType(error.Name()):
-                msg = var.Name() + " variable type does not match the " + error.Name() + " variable type"
-                raise Exception(msg)
-
-
-    @classmethod
-    def _GetBenchmarkDefaultSettings(cls):
-        raise Exception("Calling the base class of the benchmark. Please, implement the custom benchmark settings")
-
-    def _Topography(self, coordinates):
-        return 0
-
-    def _Height(self, coordinates, time):
-        raise Exception("Calling the base class of the benchmark. Please, implement the custom benchmark")
-
-    def _Velocity(self, coordinates, time):
-        raise Exception("Calling the base class of the benchmark. Please, implement the custom benchmark")
-
-    def _Momentum(self, coordinates, time):
-        return [self._Height(coordinates, time)*v for v in self._Velocity(coordinates, time)]
-
-    def _FreeSurfaceElevation(self, coordinates, time):
-        return self._Topography(coordinates) + self._Height(coordinates, time)
+# Importing the Kratos Library
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return BaseBenchmarkProcess(model, settings["Parameters"])
+
+class BaseBenchmarkProcess(KM.Process):
+    """The base class for the benchmarks."""
+
+    def __init__(self, model, settings ):
+        """The constructor of the BaseBenchmarkProcess.
+
+        It is intended to be called from the constructor of deriving classes.
+        """
+
+        super().__init__()
+
+        self.model = model
+        self.settings = settings
+
+        default_settings = KM.Parameters("""
+            {
+                "model_part_name"      : "model_part",
+                "variables_list"       : [],
+                "exact_variables_list" : [],
+                "error_variables_list" : [],
+                "benchmark_settings"   : {}
+            }
+            """
+            )
+        default_settings["benchmark_settings"] = self._GetBenchmarkDefaultSettings()
+        self.settings.RecursivelyValidateAndAssignDefaults(default_settings)
+
+        self.model_part = self.model[self.settings["model_part_name"].GetString()]
+        self.variables = GenerateVariableListFromInput(self.settings["variables_list"])
+        self.exact_variables = GenerateVariableListFromInput(self.settings["exact_variables_list"])
+        self.error_variables = GenerateVariableListFromInput(self.settings["error_variables_list"])
+
+
+    def ExecuteInitialize(self):
+        """Set the topography and the initial conditions."""
+        KM.Timer.Start("Benchmark/Initial state")
+        time = self.model_part.ProcessInfo[KM.TIME]
+        for node in self.model_part.Nodes:
+            if self._Topography(node):
+                node.SetSolutionStepValue(SW.TOPOGRAPHY, self._Topography(node))
+            node.SetSolutionStepValue(SW.HEIGHT, self._Height(node, time))
+            node.SetSolutionStepValue(KM.VELOCITY, self._Velocity(node, time))
+            node.SetSolutionStepValue(KM.MOMENTUM, self._Momentum(node, time))
+            node.SetSolutionStepValue(SW.FREE_SURFACE_ELEVATION, self._FreeSurfaceElevation(node, time))
+        KM.Timer.Stop("Benchmark/Initial state")
+
+
+    def ExecuteBeforeOutputStep(self):
+        """Compute the exact values of the benchmark and the error of the simulation."""
+        KM.Timer.Start("Benchmark/Exact values")
+        time = self.model_part.ProcessInfo[KM.TIME]
+        for (variable, exact_variable, error_variable) in zip(self.variables, self.exact_variables, self.error_variables):
+
+            if variable == SW.HEIGHT:
+                exact_value_function = self._Height
+            elif variable == KM.VELOCITY:
+                exact_value_function = self._Velocity
+            elif variable == KM.MOMENTUM:
+                exact_value_function = self._Momentum
+            elif variable == SW.FREE_SURFACE_ELEVATION:
+                exact_value_function = self._FreeSurfaceElevation
+
+            for node in self.model_part.Nodes:
+                exact_value = exact_value_function(node, time)
+                fem_value = node.GetSolutionStepValue(variable)
+
+                node.SetValue(exact_variable, exact_value)
+                node.SetValue(error_variable, fem_value - exact_value)
+        KM.Timer.Stop("Benchmark/Exact values")
+
+
+    def Check(self):
+        """Check if the input values have physical sense."""
+
+        if len(self.variables) != len(self.exact_variables):
+            raise Exception("The input variables list does not match the input exact variables list")
+
+        if len(self.variables) != len(self.error_variables):
+            raise Exception("The input variables list does not match the input error variables list")
+
+        for (var, exact, error) in zip(self.variables, self.exact_variables, self.error_variables):
+            if KM.KratosGlobals.GetVariableType(var.Name()) != KM.KratosGlobals.GetVariableType(exact.Name()):
+                msg = var.Name() + " variable type does not match the " + exact.Name() + " variable type"
+                raise Exception(msg)
+
+            if KM.KratosGlobals.GetVariableType(var.Name()) != KM.KratosGlobals.GetVariableType(error.Name()):
+                msg = var.Name() + " variable type does not match the " + error.Name() + " variable type"
+                raise Exception(msg)
+
+
+    @classmethod
+    def _GetBenchmarkDefaultSettings(cls):
+        raise Exception("Calling the base class of the benchmark. Please, implement the custom benchmark settings")
+
+    def _Topography(self, coordinates):
+        return 0
+
+    def _Height(self, coordinates, time):
+        raise Exception("Calling the base class of the benchmark. Please, implement the custom benchmark")
+
+    def _Velocity(self, coordinates, time):
+        raise Exception("Calling the base class of the benchmark. Please, implement the custom benchmark")
+
+    def _Momentum(self, coordinates, time):
+        return [self._Height(coordinates, time)*v for v in self._Velocity(coordinates, time)]
+
+    def _FreeSurfaceElevation(self, coordinates, time):
+        return self._Topography(coordinates) + self._Height(coordinates, time)
```

## KratosMultiphysics/ShallowWaterApplication/benchmarks/dam_break_benchmark.py

 * *Ordering differences only*

```diff
@@ -1,128 +1,128 @@
-import KratosMultiphysics as KM
-
-from KratosMultiphysics.ShallowWaterApplication.benchmarks.base_benchmark_process import BaseBenchmarkProcess
-
-# Other imports
-from math import sqrt
-import scipy.optimize as opt
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return DamBreakBenchmark(model, settings["Parameters"])
-
-class DamBreakBenchmark(BaseBenchmarkProcess):
-    """Dam break benchark.
-
-    O. Delestre, C. Lucas, P.-A. Ksinant, F. Darboux, C. Laguerre, T.N.T. Vo, F. James, S. Cordier
-    SWASHES: a compilation of Shallow Water Analytic Solutions for Hydraulic and Environmental Studies
-    International Journal for Numerical Methods in Fluids, Wiley, 2013, 72 (3), pp.269-300
-    """
-
-    def __init__(self, model, settings ):
-        """Constructor of the benchmark.
-
-        The base class validates the settings and sets the model_part, the variables and the benchmark_settings
-        """
-
-        super().__init__(model, settings)
-
-        self.dam = self.settings["benchmark_settings"]["dam_position"].GetDouble()
-        self.hl = self.settings["benchmark_settings"]["left_height"].GetDouble()
-        self.hr = self.settings["benchmark_settings"]["right_height"].GetDouble()
-        self.g = self.model_part.ProcessInfo[KM.GRAVITY_Z]
-
-        self.cm = self.__cm()
-
-
-    def Check(self):
-        """This method checks if the input values have physical sense."""
-
-        super().Check()
-        label = "DamBreakBenchmark. "
-        if self.g <= 0:
-            msg = label + "Gravity must be a positive value. Please, check the definition of GRAVITY_Z component in the ProcessInfo."
-            raise Exception(msg)
-        elif self.hr < 0:
-            msg = label + "Right height must be non-negative. Please, check the Parameters."
-            raise Exception(msg)
-        elif self.hl < 0:
-            msg = label + "Left height must be non-negative. Please, check the Parameters."
-            raise Exception(msg)
-
-
-    @classmethod
-    def _GetBenchmarkDefaultSettings(cls):
-        return KM.Parameters("""
-            {
-                "dam_position"  : 5.0,
-                "left_height"   : 2.0,
-                "right_height"  : 1.0
-            }
-            """
-            )
-
-
-    def _Height(self, coordinates, time):
-        x = coordinates.X
-
-        xa = self.__xa(time)
-        xb = self.__xb(time)
-        xc = self.__xc(time)
-
-        if x < xa:
-            return self.hl
-        elif x < xb:
-            return 4 / 9 / self.g * (sqrt(self.g * self.hl) - 0.5*(x - self.dam) / time)**2
-        elif x < xc:
-            return self.cm**2 / self.g
-        else:
-            return self.hr
-
-
-    def _Velocity(self, coordinates, time):
-        x = coordinates.X
-
-        xa = self.__xa(time)
-        xb = self.__xb(time)
-        xc = self.__xc(time)
-
-        if x < xa:
-            return [0.0, 0.0, 0.0]
-        elif x < xb:
-            return [2 / 3 * ((x - self.dam) / time + sqrt(self.g * self.hl)), 0.0, 0.0]
-        elif x < xc:
-            return [2 * (sqrt(self.g * self.hl) - self.cm), 0.0, 0.0]
-        else:
-            return [0.0, 0.0, 0.0]
-
-
-    def __xa(self, t):
-        return self.dam - t * sqrt(self.g * self.hl)
-
-
-    def __xb(self, t):
-        return self.dam + t * (2*sqrt(self.g * self.hl) - 3 * self.cm)
-
-
-    def __xc(self, t):
-        if self.hr > 0:
-            return self.dam + t * 2 * self.cm**2 * (sqrt(self.g*self.hl) - self.cm) / (self.cm**2 - self.g * self.hr)
-        else:
-            return self.__xb(t)
-
-
-    def __cm(self):
-        if self.hr > 0:
-            cm0 = sqrt(self.g * 0.5 * (self.hl + self.hr))
-            cm = opt.newton(self.__cm_residual, cm0)
-            return cm
-        else:
-            return 0.0
-
-
-    def __cm_residual(self,cm):
-        hl = self.hl
-        hr = self.hr
-        g  = self.g
-        return -8*g*hr*cm**2*(sqrt(g*hl)-cm)**2 + (cm**2-g*hr)**2 * (cm**2+g*hr)
+import KratosMultiphysics as KM
+
+from KratosMultiphysics.ShallowWaterApplication.benchmarks.base_benchmark_process import BaseBenchmarkProcess
+
+# Other imports
+from math import sqrt
+import scipy.optimize as opt
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return DamBreakBenchmark(model, settings["Parameters"])
+
+class DamBreakBenchmark(BaseBenchmarkProcess):
+    """Dam break benchark.
+
+    O. Delestre, C. Lucas, P.-A. Ksinant, F. Darboux, C. Laguerre, T.N.T. Vo, F. James, S. Cordier
+    SWASHES: a compilation of Shallow Water Analytic Solutions for Hydraulic and Environmental Studies
+    International Journal for Numerical Methods in Fluids, Wiley, 2013, 72 (3), pp.269-300
+    """
+
+    def __init__(self, model, settings ):
+        """Constructor of the benchmark.
+
+        The base class validates the settings and sets the model_part, the variables and the benchmark_settings
+        """
+
+        super().__init__(model, settings)
+
+        self.dam = self.settings["benchmark_settings"]["dam_position"].GetDouble()
+        self.hl = self.settings["benchmark_settings"]["left_height"].GetDouble()
+        self.hr = self.settings["benchmark_settings"]["right_height"].GetDouble()
+        self.g = self.model_part.ProcessInfo[KM.GRAVITY_Z]
+
+        self.cm = self.__cm()
+
+
+    def Check(self):
+        """This method checks if the input values have physical sense."""
+
+        super().Check()
+        label = "DamBreakBenchmark. "
+        if self.g <= 0:
+            msg = label + "Gravity must be a positive value. Please, check the definition of GRAVITY_Z component in the ProcessInfo."
+            raise Exception(msg)
+        elif self.hr < 0:
+            msg = label + "Right height must be non-negative. Please, check the Parameters."
+            raise Exception(msg)
+        elif self.hl < 0:
+            msg = label + "Left height must be non-negative. Please, check the Parameters."
+            raise Exception(msg)
+
+
+    @classmethod
+    def _GetBenchmarkDefaultSettings(cls):
+        return KM.Parameters("""
+            {
+                "dam_position"  : 5.0,
+                "left_height"   : 2.0,
+                "right_height"  : 1.0
+            }
+            """
+            )
+
+
+    def _Height(self, coordinates, time):
+        x = coordinates.X
+
+        xa = self.__xa(time)
+        xb = self.__xb(time)
+        xc = self.__xc(time)
+
+        if x < xa:
+            return self.hl
+        elif x < xb:
+            return 4 / 9 / self.g * (sqrt(self.g * self.hl) - 0.5*(x - self.dam) / time)**2
+        elif x < xc:
+            return self.cm**2 / self.g
+        else:
+            return self.hr
+
+
+    def _Velocity(self, coordinates, time):
+        x = coordinates.X
+
+        xa = self.__xa(time)
+        xb = self.__xb(time)
+        xc = self.__xc(time)
+
+        if x < xa:
+            return [0.0, 0.0, 0.0]
+        elif x < xb:
+            return [2 / 3 * ((x - self.dam) / time + sqrt(self.g * self.hl)), 0.0, 0.0]
+        elif x < xc:
+            return [2 * (sqrt(self.g * self.hl) - self.cm), 0.0, 0.0]
+        else:
+            return [0.0, 0.0, 0.0]
+
+
+    def __xa(self, t):
+        return self.dam - t * sqrt(self.g * self.hl)
+
+
+    def __xb(self, t):
+        return self.dam + t * (2*sqrt(self.g * self.hl) - 3 * self.cm)
+
+
+    def __xc(self, t):
+        if self.hr > 0:
+            return self.dam + t * 2 * self.cm**2 * (sqrt(self.g*self.hl) - self.cm) / (self.cm**2 - self.g * self.hr)
+        else:
+            return self.__xb(t)
+
+
+    def __cm(self):
+        if self.hr > 0:
+            cm0 = sqrt(self.g * 0.5 * (self.hl + self.hr))
+            cm = opt.newton(self.__cm_residual, cm0)
+            return cm
+        else:
+            return 0.0
+
+
+    def __cm_residual(self,cm):
+        hl = self.hl
+        hr = self.hr
+        g  = self.g
+        return -8*g*hr*cm**2*(sqrt(g*hl)-cm)**2 + (cm**2-g*hr)**2 * (cm**2+g*hr)
```

## KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_shock_benchmark.py

 * *Ordering differences only*

```diff
@@ -1,210 +1,210 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-from KratosMultiphysics.ShallowWaterApplication.benchmarks.base_benchmark_process import BaseBenchmarkProcess
-from KratosMultiphysics.process_factory import Factory as ProcessFactory
-
-# Other imports
-import numpy as np
-from scipy.integrate import odeint
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return MacDonaldShockBenchmark(model, settings["Parameters"])
-
-class MacDonaldShockBenchmark(BaseBenchmarkProcess):
-    """Mac Donald's shock benchmark.
-
-    This is a Mac Donald's type solution with a smooth transition and a shock in a
-    short domain, with Manning's friction coefficient.
-
-    The length of the channel is 100m and the discharge at steady state is q=2m^2/s. The flow
-    is fluvial both upstream and downstream, the boundary conditions are fixed as follows:
-        - upstream: q=2m^2/s
-        - downstream: h=h_ex(100)
-
-    This process sets the upstream and downstream boundary conditions.
-
-    O. Delestre, C. Lucas, P.-A. Ksinant, F. Darboux, C. Laguerre, T.N.T. Vo, F. James, S. Cordier
-    SWASHES: a compilation of Shallow Water Analytic Solutions for Hydraulic and Environmental Studies
-    International Journal for Numerical Methods in Fluids, Wiley, 2013, 72 (3), pp.269-300.
-    """
-
-    def __init__(self, model, settings):
-        """Constructor of the benchmark.
-
-        The base class validates the settings and sets the model_part, the variables and the benchmark_settings
-        """
-
-        super().__init__(model, settings)
-
-        self.n = self.settings["benchmark_settings"]["manning"].GetDouble()
-        self.q = self.settings["benchmark_settings"]["discharge"].GetDouble()
-        self.g = self.model_part.ProcessInfo[KM.GRAVITY_Z]
-        self.x0 = 0
-        self.x100 = 100
-        self.h0 = self._H(self.x0)
-        self.h100 = self._H(self.x100)
-
-        self.__PreComputeTopography()
-
-    @staticmethod
-    def _GetBenchmarkDefaultSettings():
-        return KM.Parameters("""
-            {
-                "discharge"             : 2,
-                "manning"               : 0.0328,
-                "upstream_model_part"   : "model_part.upstream",
-                "downstream_model_part" : "model_part.downstream"
-            }
-            """
-            )
-
-    def _Topography(self, coordinates):
-        x = coordinates.X
-        return self._Z(x)
-
-    def _Height(self, coordinates, time):
-        x = coordinates.X
-        if time > 0:
-            return self._H(x)
-        else:
-            return self._InitialH(x)
-
-    def _Momentum(self, coordinates, time):
-        if time > 0:
-            return [self.q, 0.0, 0.0]
-        else:
-            return [0.0, 0.0, 0.0]
-
-    def _Velocity(self, coordinates, time):
-        return [q / self._Height(coordinates, time) for q in self._Momentum(coordinates, time)]
-
-    def Check(self):
-        """This method checks if the input values have physical sense."""
-
-        super().Check()
-        label = self.__class__.__name__
-        if self.g <= 0:
-            msg = label + "Gravity must be a positive value. Please, check the definition of GRAVITY_Z component in the ProcessInfo."
-            raise Exception(msg)
-        elif self.n < 0:
-            msg = label + "The manning coefficient must be a positive value. Please, check the Parameters."
-            raise Exception(msg)
-        elif self.q <= 0:
-            msg = label + "The discharge must be a positive value. Please, check the Parameters."
-            raise Exception(msg)
-        self._CheckDomain()
-
-    def ExecuteInitialize(self):
-        """This method sets the topography, the initial conditions and the upstream/downstream boundary conditions"""
-
-        super().ExecuteInitialize()
-        for process in self._GetListOfBoundaryConditionsProcesses():
-            process.ExecuteInitialize()
-        KM.VariableUtils().SetVariable(SW.MANNING, self.n, self.model_part.Nodes)
-
-    def _CheckDomain(self):
-        x_min = 1.0
-        x_max = -1.0
-        for node in self.model_part.Nodes:
-            x_min = min(x_min, node.X)
-            x_max = max(x_max, node.X)
-
-        tolerance = 1e-6
-        if abs(x_min - self.x0) > tolerance:
-            KM.Logger.PrintWarning(self.__class__.__name__, "This benchmark expects an x-aligned model part starting at x=0")
-
-        if abs(x_max - self.x100) > tolerance:
-            KM.Logger.PrintWarning(self.__class__.__name__, "This benchmark expects an x-aligned model part ending at x=100")
-
-    def __PreComputeTopography(self):
-        X = np.linspace(self.x100, 0)
-        z100 = 0
-        Z = odeint(self._dZ, z100, X)
-        Z = np.ndarray.flatten(Z)
-        self.__X = X[::-1]
-        self.__Z = Z[::-1]
-
-    def _Z(self, x):
-        return np.interp(x, self.__X, self.__Z)
-
-    def _H1(self, x):
-        g = self.g
-        return (4/g)**(1/3) * (4/3 - x/100) - 9*x/1000 * (x/100 - 2/3)
-
-    def _H2(self, x):
-        g = self.g
-        a1 = 0.674202
-        a2 = 21.7112
-        a3 = 14.492
-        a4 = 1.4305
-        return (4/g)**(1/3) * (a1*(x/100 - 2/3)**4 + a1*(x/100 - 2/3)**3 - a2*(x/100 - 2/3)**2 + a3*(x/100 - 2/3) + a4)
-
-    def _dH1(self, x):
-        g = self.g
-        return -9*x/50000 - (4/g)**(1/3)/100 + 0.006
-
-    def _dH2(self, x):
-        g = self.g
-        return (4/g)**(1/3)*(-0.00434224*x + 0.02696808*(x/100 - 0.666666666666667)**3 + 0.02022606*(x/100 - 0.666666666666667)**2 + 0.434402666666667)
-
-    def _H(self, x):
-        if x < 200/3:
-            return self._H1(x)
-        else:
-            return self._H2(x)
-
-    def _dH(self, x):
-        if x < 200/3:
-            return self._dH1(x)
-        else:
-            return self._dH2(x)
-
-    def _Sf(self, h):
-        return self.n**2 * self.q**2 / h**(10/3)
-
-    def _dZ(self, z, x):
-        q = self.q
-        g = self.g
-        return (q**2 / (g * self._H(x)**3) - 1) * self._dH(x) - self._Sf(self._H(x))
-
-    def _InitialH(self, x):
-        return np.maximum(self.h100 - self._Z(x), self.h0)
-
-    def _GetListOfBoundaryConditionsProcesses(self):
-        if not hasattr(self, 'list_of_bc_processes'):
-            self.list_of_bc_processes = self._CreateListOfBoundaryConditionsProcesses()
-        return self.list_of_bc_processes
-
-    def _CreateListOfBoundaryConditionsProcesses(self):
-        benchmark_settings = self.settings["benchmark_settings"]
-
-        self.upstream_settings = KM.Parameters("""{
-            "process_name" : "ApplyConstantVectorValueProcess",
-            "Parameters"   : {
-                "variable_name"   : "MOMENTUM",
-                "is_fixed_x"      : true,
-                "is_fixed_y"      : true,
-                "direction"       : [1.0, 0.0, 0.0]}
-        }""")
-        self.upstream_settings["Parameters"].AddValue("model_part_name", benchmark_settings["upstream_model_part"])
-        self.upstream_settings["Parameters"].AddDouble("modulus", self.q)
-
-        self.downstream_settings = KM.Parameters("""{
-            "process_name" : "ApplyConstantScalarValueProcess",
-            "Parameters"   : {
-                "variable_name"   : "HEIGHT",
-                "is_fixed"        : true
-            }
-        }""")
-        self.downstream_settings["Parameters"].AddValue("model_part_name", benchmark_settings["downstream_model_part"])
-        self.downstream_settings["Parameters"].AddDouble("value", self.h100)
-
-        list_of_bc_processes = []
-        list_of_bc_processes.append(ProcessFactory(self.upstream_settings, self.model))
-        list_of_bc_processes.append(ProcessFactory(self.downstream_settings, self.model))
-
-        return list_of_bc_processes
+# Importing the Kratos Library
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+from KratosMultiphysics.ShallowWaterApplication.benchmarks.base_benchmark_process import BaseBenchmarkProcess
+from KratosMultiphysics.process_factory import Factory as ProcessFactory
+
+# Other imports
+import numpy as np
+from scipy.integrate import odeint
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return MacDonaldShockBenchmark(model, settings["Parameters"])
+
+class MacDonaldShockBenchmark(BaseBenchmarkProcess):
+    """Mac Donald's shock benchmark.
+
+    This is a Mac Donald's type solution with a smooth transition and a shock in a
+    short domain, with Manning's friction coefficient.
+
+    The length of the channel is 100m and the discharge at steady state is q=2m^2/s. The flow
+    is fluvial both upstream and downstream, the boundary conditions are fixed as follows:
+        - upstream: q=2m^2/s
+        - downstream: h=h_ex(100)
+
+    This process sets the upstream and downstream boundary conditions.
+
+    O. Delestre, C. Lucas, P.-A. Ksinant, F. Darboux, C. Laguerre, T.N.T. Vo, F. James, S. Cordier
+    SWASHES: a compilation of Shallow Water Analytic Solutions for Hydraulic and Environmental Studies
+    International Journal for Numerical Methods in Fluids, Wiley, 2013, 72 (3), pp.269-300.
+    """
+
+    def __init__(self, model, settings):
+        """Constructor of the benchmark.
+
+        The base class validates the settings and sets the model_part, the variables and the benchmark_settings
+        """
+
+        super().__init__(model, settings)
+
+        self.n = self.settings["benchmark_settings"]["manning"].GetDouble()
+        self.q = self.settings["benchmark_settings"]["discharge"].GetDouble()
+        self.g = self.model_part.ProcessInfo[KM.GRAVITY_Z]
+        self.x0 = 0
+        self.x100 = 100
+        self.h0 = self._H(self.x0)
+        self.h100 = self._H(self.x100)
+
+        self.__PreComputeTopography()
+
+    @staticmethod
+    def _GetBenchmarkDefaultSettings():
+        return KM.Parameters("""
+            {
+                "discharge"             : 2,
+                "manning"               : 0.0328,
+                "upstream_model_part"   : "model_part.upstream",
+                "downstream_model_part" : "model_part.downstream"
+            }
+            """
+            )
+
+    def _Topography(self, coordinates):
+        x = coordinates.X
+        return self._Z(x)
+
+    def _Height(self, coordinates, time):
+        x = coordinates.X
+        if time > 0:
+            return self._H(x)
+        else:
+            return self._InitialH(x)
+
+    def _Momentum(self, coordinates, time):
+        if time > 0:
+            return [self.q, 0.0, 0.0]
+        else:
+            return [0.0, 0.0, 0.0]
+
+    def _Velocity(self, coordinates, time):
+        return [q / self._Height(coordinates, time) for q in self._Momentum(coordinates, time)]
+
+    def Check(self):
+        """This method checks if the input values have physical sense."""
+
+        super().Check()
+        label = self.__class__.__name__
+        if self.g <= 0:
+            msg = label + "Gravity must be a positive value. Please, check the definition of GRAVITY_Z component in the ProcessInfo."
+            raise Exception(msg)
+        elif self.n < 0:
+            msg = label + "The manning coefficient must be a positive value. Please, check the Parameters."
+            raise Exception(msg)
+        elif self.q <= 0:
+            msg = label + "The discharge must be a positive value. Please, check the Parameters."
+            raise Exception(msg)
+        self._CheckDomain()
+
+    def ExecuteInitialize(self):
+        """This method sets the topography, the initial conditions and the upstream/downstream boundary conditions"""
+
+        super().ExecuteInitialize()
+        for process in self._GetListOfBoundaryConditionsProcesses():
+            process.ExecuteInitialize()
+        KM.VariableUtils().SetVariable(SW.MANNING, self.n, self.model_part.Nodes)
+
+    def _CheckDomain(self):
+        x_min = 1.0
+        x_max = -1.0
+        for node in self.model_part.Nodes:
+            x_min = min(x_min, node.X)
+            x_max = max(x_max, node.X)
+
+        tolerance = 1e-6
+        if abs(x_min - self.x0) > tolerance:
+            KM.Logger.PrintWarning(self.__class__.__name__, "This benchmark expects an x-aligned model part starting at x=0")
+
+        if abs(x_max - self.x100) > tolerance:
+            KM.Logger.PrintWarning(self.__class__.__name__, "This benchmark expects an x-aligned model part ending at x=100")
+
+    def __PreComputeTopography(self):
+        X = np.linspace(self.x100, 0)
+        z100 = 0
+        Z = odeint(self._dZ, z100, X)
+        Z = np.ndarray.flatten(Z)
+        self.__X = X[::-1]
+        self.__Z = Z[::-1]
+
+    def _Z(self, x):
+        return np.interp(x, self.__X, self.__Z)
+
+    def _H1(self, x):
+        g = self.g
+        return (4/g)**(1/3) * (4/3 - x/100) - 9*x/1000 * (x/100 - 2/3)
+
+    def _H2(self, x):
+        g = self.g
+        a1 = 0.674202
+        a2 = 21.7112
+        a3 = 14.492
+        a4 = 1.4305
+        return (4/g)**(1/3) * (a1*(x/100 - 2/3)**4 + a1*(x/100 - 2/3)**3 - a2*(x/100 - 2/3)**2 + a3*(x/100 - 2/3) + a4)
+
+    def _dH1(self, x):
+        g = self.g
+        return -9*x/50000 - (4/g)**(1/3)/100 + 0.006
+
+    def _dH2(self, x):
+        g = self.g
+        return (4/g)**(1/3)*(-0.00434224*x + 0.02696808*(x/100 - 0.666666666666667)**3 + 0.02022606*(x/100 - 0.666666666666667)**2 + 0.434402666666667)
+
+    def _H(self, x):
+        if x < 200/3:
+            return self._H1(x)
+        else:
+            return self._H2(x)
+
+    def _dH(self, x):
+        if x < 200/3:
+            return self._dH1(x)
+        else:
+            return self._dH2(x)
+
+    def _Sf(self, h):
+        return self.n**2 * self.q**2 / h**(10/3)
+
+    def _dZ(self, z, x):
+        q = self.q
+        g = self.g
+        return (q**2 / (g * self._H(x)**3) - 1) * self._dH(x) - self._Sf(self._H(x))
+
+    def _InitialH(self, x):
+        return np.maximum(self.h100 - self._Z(x), self.h0)
+
+    def _GetListOfBoundaryConditionsProcesses(self):
+        if not hasattr(self, 'list_of_bc_processes'):
+            self.list_of_bc_processes = self._CreateListOfBoundaryConditionsProcesses()
+        return self.list_of_bc_processes
+
+    def _CreateListOfBoundaryConditionsProcesses(self):
+        benchmark_settings = self.settings["benchmark_settings"]
+
+        self.upstream_settings = KM.Parameters("""{
+            "process_name" : "ApplyConstantVectorValueProcess",
+            "Parameters"   : {
+                "variable_name"   : "MOMENTUM",
+                "is_fixed_x"      : true,
+                "is_fixed_y"      : true,
+                "direction"       : [1.0, 0.0, 0.0]}
+        }""")
+        self.upstream_settings["Parameters"].AddValue("model_part_name", benchmark_settings["upstream_model_part"])
+        self.upstream_settings["Parameters"].AddDouble("modulus", self.q)
+
+        self.downstream_settings = KM.Parameters("""{
+            "process_name" : "ApplyConstantScalarValueProcess",
+            "Parameters"   : {
+                "variable_name"   : "HEIGHT",
+                "is_fixed"        : true
+            }
+        }""")
+        self.downstream_settings["Parameters"].AddValue("model_part_name", benchmark_settings["downstream_model_part"])
+        self.downstream_settings["Parameters"].AddDouble("value", self.h100)
+
+        list_of_bc_processes = []
+        list_of_bc_processes.append(ProcessFactory(self.upstream_settings, self.model))
+        list_of_bc_processes.append(ProcessFactory(self.downstream_settings, self.model))
+
+        return list_of_bc_processes
```

## KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_transition_benchmark.py

 * *Ordering differences only*

```diff
@@ -1,79 +1,79 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KM
-
-from KratosMultiphysics.ShallowWaterApplication.benchmarks.mac_donald_shock_benchmark import MacDonaldShockBenchmark
-from KratosMultiphysics.process_factory import Factory as ProcessFactory
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return MacDonaldTransitionBenchmark(model, settings["Parameters"])
-
-class MacDonaldTransitionBenchmark(MacDonaldShockBenchmark):
-    """Mac Donald's transcritical flow.
-
-    This is a Mac Donald's type solution with a smooth transition to supercritical flow in a
-    short domain, with Manning's friction coefficient.
-
-    The length of the channel is 100m and the discharge at steady state is q=2m^2/s. The flow
-    is fluvial upstream and torrential downstream, the boundary conditions are fixed as follows:
-        - upstream: q=2m^2/s
-        - downstream: free
-
-    This process sets the upstream and downstream boundary conditions.
-
-    O. Delestre, C. Lucas, P.-A. Ksinant, F. Darboux, C. Laguerre, T.N.T. Vo, F. James, S. Cordier
-    SWASHES: a compilation of Shallow Water Analytic Solutions for Hydraulic and Environmental Studies
-    International Journal for Numerical Methods in Fluids, Wiley, 2013, 72 (3), pp.269-300.
-    """
-
-    def __init__(self, model, settings):
-        """Constructor of the benchmark.
-
-        The base class validates the settings and sets the model_part, the variables and the benchmark_settings
-        """
-
-        super().__init__(model, settings)
-
-    @staticmethod
-    def _GetBenchmarkDefaultSettings():
-        return KM.Parameters("""
-            {
-                "discharge"             : 2,
-                "manning"               : 0.0328,
-                "upstream_model_part"   : "model_part.upstream"
-            }
-            """)
-
-    def _H(self, x):
-        g = self.g
-        return (4/g)**(1/3) * (1 - (x-50)/200 + (x-50)**2/30000)
-
-    def _dH(self, x):
-        g = self.g
-        return (4/g)**(1/3) * (x/15000 - 5/600)
-
-    def _InitialH(self, x):
-        if x > self.x0:
-            return 1e-6
-        else:
-            return self.h0
-
-    def _CreateListOfBoundaryConditionsProcesses(self):
-        benchmark_settings = self.settings["benchmark_settings"]
-
-        self.upstream_settings = KM.Parameters("""{
-            "process_name" : "ApplyConstantVectorValueProcess",
-            "Parameters"   : {
-                "variable_name"   : "MOMENTUM",
-                "is_fixed_x"      : true,
-                "is_fixed_y"      : true,
-                "direction"       : [1.0, 0.0, 0.0]}
-        }""")
-        self.upstream_settings["Parameters"].AddValue("model_part_name", benchmark_settings["upstream_model_part"])
-        self.upstream_settings["Parameters"].AddDouble("modulus", self.q)
-
-        list_of_bc_processes = []
-        list_of_bc_processes.append(ProcessFactory(self.upstream_settings, self.model))
-
-        return list_of_bc_processes
+# Importing the Kratos Library
+import KratosMultiphysics as KM
+
+from KratosMultiphysics.ShallowWaterApplication.benchmarks.mac_donald_shock_benchmark import MacDonaldShockBenchmark
+from KratosMultiphysics.process_factory import Factory as ProcessFactory
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return MacDonaldTransitionBenchmark(model, settings["Parameters"])
+
+class MacDonaldTransitionBenchmark(MacDonaldShockBenchmark):
+    """Mac Donald's transcritical flow.
+
+    This is a Mac Donald's type solution with a smooth transition to supercritical flow in a
+    short domain, with Manning's friction coefficient.
+
+    The length of the channel is 100m and the discharge at steady state is q=2m^2/s. The flow
+    is fluvial upstream and torrential downstream, the boundary conditions are fixed as follows:
+        - upstream: q=2m^2/s
+        - downstream: free
+
+    This process sets the upstream and downstream boundary conditions.
+
+    O. Delestre, C. Lucas, P.-A. Ksinant, F. Darboux, C. Laguerre, T.N.T. Vo, F. James, S. Cordier
+    SWASHES: a compilation of Shallow Water Analytic Solutions for Hydraulic and Environmental Studies
+    International Journal for Numerical Methods in Fluids, Wiley, 2013, 72 (3), pp.269-300.
+    """
+
+    def __init__(self, model, settings):
+        """Constructor of the benchmark.
+
+        The base class validates the settings and sets the model_part, the variables and the benchmark_settings
+        """
+
+        super().__init__(model, settings)
+
+    @staticmethod
+    def _GetBenchmarkDefaultSettings():
+        return KM.Parameters("""
+            {
+                "discharge"             : 2,
+                "manning"               : 0.0328,
+                "upstream_model_part"   : "model_part.upstream"
+            }
+            """)
+
+    def _H(self, x):
+        g = self.g
+        return (4/g)**(1/3) * (1 - (x-50)/200 + (x-50)**2/30000)
+
+    def _dH(self, x):
+        g = self.g
+        return (4/g)**(1/3) * (x/15000 - 5/600)
+
+    def _InitialH(self, x):
+        if x > self.x0:
+            return 1e-6
+        else:
+            return self.h0
+
+    def _CreateListOfBoundaryConditionsProcesses(self):
+        benchmark_settings = self.settings["benchmark_settings"]
+
+        self.upstream_settings = KM.Parameters("""{
+            "process_name" : "ApplyConstantVectorValueProcess",
+            "Parameters"   : {
+                "variable_name"   : "MOMENTUM",
+                "is_fixed_x"      : true,
+                "is_fixed_y"      : true,
+                "direction"       : [1.0, 0.0, 0.0]}
+        }""")
+        self.upstream_settings["Parameters"].AddValue("model_part_name", benchmark_settings["upstream_model_part"])
+        self.upstream_settings["Parameters"].AddDouble("modulus", self.q)
+
+        list_of_bc_processes = []
+        list_of_bc_processes.append(ProcessFactory(self.upstream_settings, self.model))
+
+        return list_of_bc_processes
```

## KratosMultiphysics/ShallowWaterApplication/benchmarks/planar_surface_in_parabola_benchmark.py

 * *Ordering differences only*

```diff
@@ -1,116 +1,116 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KM
-
-from KratosMultiphysics.ShallowWaterApplication.benchmarks.base_benchmark_process import BaseBenchmarkProcess
-
-# Other imports
-from math import sqrt, sin, cos
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return PlanarSurfaceInParabolaBenchmark(model, settings["Parameters"])
-
-class PlanarSurfaceInParabolaBenchmark(BaseBenchmarkProcess):
-    """Planar surface in parabola benchark.
-
-    O. Delestre, C. Lucas, P.-A. Ksinant, F. Darboux, C. Laguerre, T.N.T. Vo, F. James, S. Cordier
-    SWASHES: a compilation of Shallow Water Analytic Solutions for Hydraulic and Environmental Studies
-    International Journal for Numerical Methods in Fluids, Wiley, 2013, 72 (3), pp.269-300
-    """
-
-    def __init__(self, model, settings):
-        """Constructor of the benchmark.
-
-        The base class validates the settings and sets the model_part, the variables and the benchmark_settings
-        """
-
-        super().__init__(model, settings)
-
-        self.h0 = self.settings["benchmark_settings"]["depth"].GetDouble()
-        self.a = self.settings["benchmark_settings"]["amplitude"].GetDouble()
-    
-    def ExecuteInitialize(self):
-        self.g = self.model_part.ProcessInfo[KM.GRAVITY_Z]
-        self.B = self.__B()
-        self.C = self.__C()
-        self.L = self.__L()
-        super().ExecuteInitialize()
-
-    @classmethod
-    def _GetBenchmarkDefaultSettings(cls):
-        return KM.Parameters("""
-            {
-                "depth"     : 1.0,
-                "amplitude" : 1.0
-            }
-            """
-            )
-
-    def _Topography(self, coordinates):
-        x = coordinates.X
-        return self.h0 * (1/self.a**2 * (x - 0.5*self.L)**2 - 1.0)
-
-    def _Height(self, coordinates, time):
-        x = coordinates.X
-        x0 = self.__x0(time)
-        x1 = self.__x1(time)
-        if x0 < x < x1:
-            return -self.h0*(((x - 0.5*self.L)/self.a + 0.5/self.a*cos(self.C*time/self.a))**2 - 1)
-        else:
-            return 0.0
-
-    def _Velocity(self, coordinates, time):
-        x = coordinates.X
-        x0 = self.__x0(time)
-        x1 = self.__x1(time)
-        if x0 < x < x1:
-            return [self.B * sin(self.C*time/self.a), 0.0, 0.0]
-        else:
-            return [0.0, 0.0, 0.0]
-
-    def Check(self):
-        """This method checks if the input values have physical sense."""
-
-        super().Check()
-        label = self.__class__.__name__
-        if self.g <= 0:
-            msg = label + "Gravity must be a positive value. Please, check the definition of GRAVITY_Z component in the ProcessInfo."
-            raise Exception(msg)
-        elif self.L <= 0:
-            msg = label + "The length must be a positive value. Please, check the Parameters."
-            raise Exception(msg)
-        elif self.h0 <= 0:
-            msg = label + "The depth must be a positive value. Please, check the Parameters."
-            raise Exception(msg)
-        elif self.a <= 0:
-            msg = label + "The amplitude must be a positive value. Please, check the Parameters."
-            raise Exception(msg)
-
-    def __B(self):
-        return self.__C() / 2.0 / self.a
-
-    def __C(self):
-        return sqrt(2*self.g*self.h0)
-
-    def __L(self):
-        x0 = 1.0
-        x1 = -1.0
-        for node in self.model_part.Nodes:
-            x0 = min(x0, node.X)
-            x1 = max(x1, node.X)
-
-        tolerance = 1e-6
-        if abs(x0) > tolerance:
-            KM.Logger.PrintWarning(self.__class__.__name__, "This benchmark expects an x-aligned model part starting at x=0")
-
-        if x1 <= 0.0:
-            KM.Logger.PrintWarning(self.__class__.__name__, "This benchmark expects a model part with x>0")
-
-        return x1 - x0
-
-    def __x0(self, time):
-        return -0.5*cos(self.C/self.a*time) - self.a + 0.5*self.L
-
-    def __x1(self, time):
-        return -0.5*cos(self.C/self.a*time) + self.a + 0.5*self.L
+# Importing the Kratos Library
+import KratosMultiphysics as KM
+
+from KratosMultiphysics.ShallowWaterApplication.benchmarks.base_benchmark_process import BaseBenchmarkProcess
+
+# Other imports
+from math import sqrt, sin, cos
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return PlanarSurfaceInParabolaBenchmark(model, settings["Parameters"])
+
+class PlanarSurfaceInParabolaBenchmark(BaseBenchmarkProcess):
+    """Planar surface in parabola benchark.
+
+    O. Delestre, C. Lucas, P.-A. Ksinant, F. Darboux, C. Laguerre, T.N.T. Vo, F. James, S. Cordier
+    SWASHES: a compilation of Shallow Water Analytic Solutions for Hydraulic and Environmental Studies
+    International Journal for Numerical Methods in Fluids, Wiley, 2013, 72 (3), pp.269-300
+    """
+
+    def __init__(self, model, settings):
+        """Constructor of the benchmark.
+
+        The base class validates the settings and sets the model_part, the variables and the benchmark_settings
+        """
+
+        super().__init__(model, settings)
+
+        self.h0 = self.settings["benchmark_settings"]["depth"].GetDouble()
+        self.a = self.settings["benchmark_settings"]["amplitude"].GetDouble()
+    
+    def ExecuteInitialize(self):
+        self.g = self.model_part.ProcessInfo[KM.GRAVITY_Z]
+        self.B = self.__B()
+        self.C = self.__C()
+        self.L = self.__L()
+        super().ExecuteInitialize()
+
+    @classmethod
+    def _GetBenchmarkDefaultSettings(cls):
+        return KM.Parameters("""
+            {
+                "depth"     : 1.0,
+                "amplitude" : 1.0
+            }
+            """
+            )
+
+    def _Topography(self, coordinates):
+        x = coordinates.X
+        return self.h0 * (1/self.a**2 * (x - 0.5*self.L)**2 - 1.0)
+
+    def _Height(self, coordinates, time):
+        x = coordinates.X
+        x0 = self.__x0(time)
+        x1 = self.__x1(time)
+        if x0 < x < x1:
+            return -self.h0*(((x - 0.5*self.L)/self.a + 0.5/self.a*cos(self.C*time/self.a))**2 - 1)
+        else:
+            return 0.0
+
+    def _Velocity(self, coordinates, time):
+        x = coordinates.X
+        x0 = self.__x0(time)
+        x1 = self.__x1(time)
+        if x0 < x < x1:
+            return [self.B * sin(self.C*time/self.a), 0.0, 0.0]
+        else:
+            return [0.0, 0.0, 0.0]
+
+    def Check(self):
+        """This method checks if the input values have physical sense."""
+
+        super().Check()
+        label = self.__class__.__name__
+        if self.g <= 0:
+            msg = label + "Gravity must be a positive value. Please, check the definition of GRAVITY_Z component in the ProcessInfo."
+            raise Exception(msg)
+        elif self.L <= 0:
+            msg = label + "The length must be a positive value. Please, check the Parameters."
+            raise Exception(msg)
+        elif self.h0 <= 0:
+            msg = label + "The depth must be a positive value. Please, check the Parameters."
+            raise Exception(msg)
+        elif self.a <= 0:
+            msg = label + "The amplitude must be a positive value. Please, check the Parameters."
+            raise Exception(msg)
+
+    def __B(self):
+        return self.__C() / 2.0 / self.a
+
+    def __C(self):
+        return sqrt(2*self.g*self.h0)
+
+    def __L(self):
+        x0 = 1.0
+        x1 = -1.0
+        for node in self.model_part.Nodes:
+            x0 = min(x0, node.X)
+            x1 = max(x1, node.X)
+
+        tolerance = 1e-6
+        if abs(x0) > tolerance:
+            KM.Logger.PrintWarning(self.__class__.__name__, "This benchmark expects an x-aligned model part starting at x=0")
+
+        if x1 <= 0.0:
+            KM.Logger.PrintWarning(self.__class__.__name__, "This benchmark expects a model part with x>0")
+
+        return x1 - x0
+
+    def __x0(self, time):
+        return -0.5*cos(self.C/self.a*time) - self.a + 0.5*self.L
+
+    def __x1(self, time):
+        return -0.5*cos(self.C/self.a*time) + self.a + 0.5*self.L
```

## KratosMultiphysics/ShallowWaterApplication/benchmarks/solitary_wave_benchmark.py

 * *Ordering differences only*

```diff
@@ -1,84 +1,84 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-from KratosMultiphysics.ShallowWaterApplication.benchmarks.base_benchmark_process import BaseBenchmarkProcess
-from KratosMultiphysics.ShallowWaterApplication.utilities.wave_factory import SolitaryWaveFactory
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return SolitaryWaveBenchmark(model, settings["Parameters"])
-
-class SolitaryWaveBenchmark(BaseBenchmarkProcess):
-    """Solitary wave benchmark.
-
-    Propagation of a solitary wave along the x axis.
-    """
-
-    def ExecuteInitialize(self):
-        # Construction of the wave settings
-        benchmark_settings = self.settings["benchmark_settings"]
-        self.boundary_model_part = self.model.GetModelPart(benchmark_settings["boundary_model_part_name"].GetString())
-        self.wave = SolitaryWaveFactory(self.boundary_model_part, benchmark_settings["wave_specifications"])
-        self.x_shift = benchmark_settings["wave_specifications"]["x_shift"].GetDouble()
-        self.t_shift = benchmark_settings["wave_specifications"]["t_shift"].GetDouble()
-        self.get_depth_from_model_part = benchmark_settings["wave_specifications"]["get_depth_from_model_part"].GetBool()
-
-        # Here the base class sets the topography and initial conditions
-        super().ExecuteInitialize()
-
-
-    @classmethod
-    def _GetBenchmarkDefaultSettings(cls):
-        return KM.Parameters("""{
-            "boundary_model_part_name"  : "",
-            "wave_specifications"       : {
-                "wave_theory"               : "boussinesq",
-                "amplitude"                 : 1.0,
-                "depth"                     : 1.0,
-                "get_depth_from_model_part" : false,
-                "x_shift"                   : 0.0,
-                "t_shift"                   : 0.0
-            }
-        }""")
-
-
-    def _Topography(self, coordinates):
-        if self.get_depth_from_model_part:
-            return 0
-        else:
-            return -self.wave.depth
-
-
-    def _FreeSurfaceElevation(self, coordinates, time):
-        x = coordinates.X
-        return self.wave.eta(x - self.x_shift, time - self.t_shift)
-
-
-    def _Height(self, coordinates, time):
-        return self._FreeSurfaceElevation(coordinates, time) + self.wave.depth
-
-
-    def _Velocity(self, coordinates, time):
-        x = coordinates.X
-        u_x = self.wave.u(x - self.x_shift, time - self.t_shift)
-        return [u_x, 0.0, 0.0]
-
-
-    def ExecuteBeforeSolutionLoop(self):
-        SW.ShallowWaterUtilities().ComputeHeightFromFreeSurface(self.model_part)
-        SW.ShallowWaterUtilities().SetMinimumValue(self.model_part, SW.HEIGHT, 0.0)
-        SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.model_part)
-
-
-    def ExecuteInitializeSolutionStep(self):
-        time = self.boundary_model_part.ProcessInfo[KM.TIME]
-        for node in self.boundary_model_part.Nodes:
-            node.SetSolutionStepValue(KM.VELOCITY, self._Velocity(node, time))
-            node.SetSolutionStepValue(SW.HEIGHT, self._Height(node, time))
-        KM.VariableUtils().ApplyFixity(KM.VELOCITY_X, True, self.boundary_model_part.Nodes)
-        KM.VariableUtils().ApplyFixity(SW.HEIGHT, True, self.boundary_model_part.Nodes)
-
-
-    def ExecuteFinalizeSolutionStep(self):
-        KM.VariableUtils().ApplyFixity(KM.VELOCITY_X, True, self.boundary_model_part.Nodes)
-        KM.VariableUtils().ApplyFixity(SW.HEIGHT, False, self.boundary_model_part.Nodes)
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+from KratosMultiphysics.ShallowWaterApplication.benchmarks.base_benchmark_process import BaseBenchmarkProcess
+from KratosMultiphysics.ShallowWaterApplication.utilities.wave_factory import SolitaryWaveFactory
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return SolitaryWaveBenchmark(model, settings["Parameters"])
+
+class SolitaryWaveBenchmark(BaseBenchmarkProcess):
+    """Solitary wave benchmark.
+
+    Propagation of a solitary wave along the x axis.
+    """
+
+    def ExecuteInitialize(self):
+        # Construction of the wave settings
+        benchmark_settings = self.settings["benchmark_settings"]
+        self.boundary_model_part = self.model.GetModelPart(benchmark_settings["boundary_model_part_name"].GetString())
+        self.wave = SolitaryWaveFactory(self.boundary_model_part, benchmark_settings["wave_specifications"])
+        self.x_shift = benchmark_settings["wave_specifications"]["x_shift"].GetDouble()
+        self.t_shift = benchmark_settings["wave_specifications"]["t_shift"].GetDouble()
+        self.get_depth_from_model_part = benchmark_settings["wave_specifications"]["get_depth_from_model_part"].GetBool()
+
+        # Here the base class sets the topography and initial conditions
+        super().ExecuteInitialize()
+
+
+    @classmethod
+    def _GetBenchmarkDefaultSettings(cls):
+        return KM.Parameters("""{
+            "boundary_model_part_name"  : "",
+            "wave_specifications"       : {
+                "wave_theory"               : "boussinesq",
+                "amplitude"                 : 1.0,
+                "depth"                     : 1.0,
+                "get_depth_from_model_part" : false,
+                "x_shift"                   : 0.0,
+                "t_shift"                   : 0.0
+            }
+        }""")
+
+
+    def _Topography(self, coordinates):
+        if self.get_depth_from_model_part:
+            return 0
+        else:
+            return -self.wave.depth
+
+
+    def _FreeSurfaceElevation(self, coordinates, time):
+        x = coordinates.X
+        return self.wave.eta(x - self.x_shift, time - self.t_shift)
+
+
+    def _Height(self, coordinates, time):
+        return self._FreeSurfaceElevation(coordinates, time) + self.wave.depth
+
+
+    def _Velocity(self, coordinates, time):
+        x = coordinates.X
+        u_x = self.wave.u(x - self.x_shift, time - self.t_shift)
+        return [u_x, 0.0, 0.0]
+
+
+    def ExecuteBeforeSolutionLoop(self):
+        SW.ShallowWaterUtilities().ComputeHeightFromFreeSurface(self.model_part)
+        SW.ShallowWaterUtilities().SetMinimumValue(self.model_part, SW.HEIGHT, 0.0)
+        SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.model_part)
+
+
+    def ExecuteInitializeSolutionStep(self):
+        time = self.boundary_model_part.ProcessInfo[KM.TIME]
+        for node in self.boundary_model_part.Nodes:
+            node.SetSolutionStepValue(KM.VELOCITY, self._Velocity(node, time))
+            node.SetSolutionStepValue(SW.HEIGHT, self._Height(node, time))
+        KM.VariableUtils().ApplyFixity(KM.VELOCITY_X, True, self.boundary_model_part.Nodes)
+        KM.VariableUtils().ApplyFixity(SW.HEIGHT, True, self.boundary_model_part.Nodes)
+
+
+    def ExecuteFinalizeSolutionStep(self):
+        KM.VariableUtils().ApplyFixity(KM.VELOCITY_X, True, self.boundary_model_part.Nodes)
+        KM.VariableUtils().ApplyFixity(SW.HEIGHT, False, self.boundary_model_part.Nodes)
```

## KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_input_process.py

 * *Ordering differences only*

```diff
@@ -1,245 +1,245 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-import KratosMultiphysics.MappingApplication as Mapping
-from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
-from KratosMultiphysics.HDF5Application import import_model_part_from_hdf5_process
-from KratosMultiphysics.HDF5Application import single_mesh_temporal_input_process
-from os.path import commonprefix
-from pathlib import Path
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return DepthIntegrationInputProcess(model, settings["Parameters"])
-
-class DepthIntegrationInputProcess(KM.Process):
-    """DepthIntegrationInputProcess
-
-    Read the depth integrated values from an HDF5 file and set them as boundary conditions.
-    """
-
-    def GetDefaultParameters(self):
-        default_parameters = KM.Parameters("""{
-            "interface_model_part_name"   : "",
-            "input_model_part_name"       : "input_model_part",
-            "read_historical_database"    : false,
-            "interval"                    : [0.0,"End"],
-            "list_of_variables"           : ["MOMENTUM"],
-            "list_of_variables_to_fix"    : ["MOMENTUM_X","MOMENTUM_Y"],
-            "default_time_after_interval" : null,
-            "semi_period_after_interval"  : 1.0,
-            "swap_yz_axis"                : false,
-            "ignore_vertical_component"   : true,
-            "file_settings"               : {}
-        }""")
-        if self.settings.Has("default_time_after_interval"):
-            if self.settings["default_time_after_interval"].IsDouble():
-                default_parameters["default_time_after_interval"].SetDouble(0.0)
-        return default_parameters
-
-    def __init__(self, model, settings):
-        """The constructor of the DepthIntegrationInputProcess."""
-
-        KM.Process.__init__(self)
-        self.settings = settings
-        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
-
-        self.interface_model_part = model[self.settings["interface_model_part_name"].GetString()]
-        self.input_model_part = model.CreateModelPart(self.settings["input_model_part_name"].GetString())
-        self.interval = KM.IntervalUtility(self.settings)
-        self.variables = GenerateVariableListFromInput(self.settings["list_of_variables"])
-        self.variables_to_fix = GenerateVariableListFromInput(self.settings["list_of_variables_to_fix"])
-
-        self.hdf5_import = import_model_part_from_hdf5_process.Factory(self._CreateHDF5Parameters(), model)
-        self.hdf5_process = single_mesh_temporal_input_process.Factory(self._CreateHDF5Parameters(), model)
-        self._GetInputTimes(self.settings['file_settings'])
-
-
-    def Check(self):
-        '''Check the processes.'''
-        self.hdf5_import.Check()
-        self.hdf5_process.Check()
-        free_surface_is_present = False
-        height_is_present = False
-        for variable in self.variables:
-            if variable == SW.FREE_SURFACE_ELEVATION:
-                free_surface_is_present = True
-            if variable == SW.HEIGHT:
-                height_is_present = True
-        if free_surface_is_present and not height_is_present:
-            self.variables.append(SW.HEIGHT)
-
-
-    def ExecuteInitialize(self):
-        '''Read the input_model_part and set the variables.'''
-        self.hdf5_import.ExecuteInitialize()
-        self._CheckInputCoordinates()
-        self._CheckInputVariables()
-        self._CreateMapper()
-        self._MapToBoundaryCondition()
-
-
-    def ExecuteInitializeSolutionStep(self):
-        '''Set the variables in the input_model_part at the current time.'''
-        current_time = self.interface_model_part.ProcessInfo.GetValue(KM.TIME)
-        if self.interval.IsInInterval(current_time):
-            self._SetCurrentTime()
-            self.hdf5_process.ExecuteInitializeSolutionStep()
-            self._CheckInputVariables()
-            self._MapToBoundaryCondition()
-        else:
-            if self.settings["default_time_after_interval"] is not None:
-                self._SetDefaultTime()
-                self.hdf5_process.ExecuteInitializeSolutionStep()
-                self._CheckInputVariables()
-                self._MapToBoundaryCondition()
-                self._SmoothDefaultValue()
-
-
-    def _GetInputTimes(self, file_settings):
-        # Get all the file names
-        file = Path(file_settings["file_name"].GetString())
-        directory = file.parent
-        file_names = [str(f) for f in directory.glob("*.h5")]
-        if len(file_names) == 0:
-            msg = self.__class__.__name__ + ": The specified path is empty or does not exist: '{}'"
-            raise Exception(msg.format(directory))
-
-        # Find the common parts (prefix and suffix) of the found names and the file pattern
-        # The different part is the time, we need to store all the available times
-        file_pattern = str(file).replace('<model_part_name>', self.input_model_part.Name)
-        prefix = commonprefix([file_pattern, file_names[0]])
-        suffix = commonprefix([''.join(reversed(file_pattern)), ''.join(reversed(file_names[0]))])
-        suffix = ''.join(reversed(suffix))
-
-        # Store the times
-        self.times = []
-        for f in file_names:
-            f = f.replace(prefix, '')
-            f = f.replace(suffix, '')
-            try:
-                self.times.append(float(f))
-            except ValueError:
-                msg = self.__class__.__name__
-                msg += ": Trying to extract the time stamp from the input file name:\n"
-                msg += "\tExpected pattern: {}\n"
-                msg += "\tFound pattern:    {}<{}>{}"
-                KM.Logger.PrintInfo(msg.format(file_pattern, prefix, f, suffix))
-                raise
-        self.times.sort()
-
-
-    def _SetCurrentTime(self):
-        current_time = self.interface_model_part.ProcessInfo.GetValue(KM.TIME)
-        if current_time > self.times[-1]:
-            msg = self.__class__.__name__
-            msg += ": Looking for an input file at time {}. However, the input files end at time {}."
-            raise Exception(msg.format(current_time, self.times[-1]))
-        closest_time = next(filter(lambda x: x>current_time, self.times))
-        self.input_model_part.ProcessInfo.SetValue(KM.TIME, closest_time)
-
-
-    def _SetDefaultTime(self):
-        default_time = self.settings["default_time_after_interval"].GetDouble()
-        self.input_model_part.ProcessInfo.SetValue(KM.TIME, default_time)
-
-
-    def _CheckInputCoordinates(self):
-        if self.settings["swap_yz_axis"].GetBool():
-            SW.ShallowWaterUtilities().SwapYZCoordinates(self.input_model_part)
-            SW.ShallowWaterUtilities().SwapY0Z0Coordinates(self.input_model_part)
-        if self.settings["ignore_vertical_component"].GetBool():
-            SW.ShallowWaterUtilities().SetMeshZCoordinateToZero(self.input_model_part)
-            SW.ShallowWaterUtilities().SetMeshZ0CoordinateToZero(self.input_model_part)
-
-
-    def _CheckInputVariables(self):
-        if self.settings["swap_yz_axis"].GetBool():
-            if self.settings["read_historical_database"].GetBool():
-                SW.ShallowWaterUtilities().SwapYZComponents(KM.MOMENTUM, self.input_model_part.Nodes)
-                SW.ShallowWaterUtilities().SwapYZComponents(KM.VELOCITY, self.input_model_part.Nodes)
-            else:
-                SW.ShallowWaterUtilities().SwapYZComponentsNonHistorical(KM.MOMENTUM, self.input_model_part.Nodes)
-                SW.ShallowWaterUtilities().SwapYZComponentsNonHistorical(KM.VELOCITY, self.input_model_part.Nodes)
-        if self.settings["ignore_vertical_component"].GetBool():
-            if self.settings["read_historical_database"].GetBool():
-                KM.VariableUtils().SetVariableToZero(KM.MOMENTUM_Z, self.input_model_part.Nodes)
-                KM.VariableUtils().SetVariableToZero(KM.VELOCITY_Z, self.input_model_part.Nodes)
-            else:
-                KM.VariableUtils().SetNonHistoricalVariableToZero(KM.MOMENTUM_Z, self.input_model_part.Nodes)
-                KM.VariableUtils().SetNonHistoricalVariableToZero(KM.VELOCITY_Z, self.input_model_part.Nodes)
-
-
-    def _MapToBoundaryCondition(self):
-        for variable in self.variables:
-            if variable == SW.FREE_SURFACE_ELEVATION:
-                pass
-            else:
-                if self.settings["read_historical_database"].GetBool():
-                    self.mapper.Map(variable, variable)
-                else:
-                    self.mapper.Map(variable, variable, KM.Mapper.FROM_NON_HISTORICAL)
-
-        for variable in self.variables:
-            if variable == SW.FREE_SURFACE_ELEVATION:
-                SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.interface_model_part)
-            else:
-                pass
-
-        for variable in self.variables_to_fix:
-            KM.VariableUtils().ApplyFixity(variable, True, self.interface_model_part.Nodes)
-
-
-    def _CreateMapper(self):
-        domain_size = self.input_model_part.ProcessInfo[KM.DOMAIN_SIZE]
-        if domain_size == 2:
-            mapper_settings = KM.Parameters("""{
-                "mapper_type": "nearest_neighbor",
-                "echo_level" : 0,
-                "search_settings" : {
-                    "search_radius" : 0.0
-                }
-            }""")
-            min_point, max_point = KM.BoundingBox(self.interface_model_part.Nodes).GetPoints()
-            search_radius = 1.05 * (max_point - min_point).norm_2()
-            mapper_settings.AddEmptyValue("search_settings")
-            mapper_settings["search_settings"]["search_radius"].SetDouble(search_radius)
-        elif domain_size == 3:
-            mapper_settings = KM.Parameters("""{
-                "mapper_type": "nearest_neighbor",
-                "echo_level" : 0
-            }""")
-        else:
-            msg = self.__class__.__name__
-            msg += "._CreateMapper: The domain size of the input_model_part is: {}"
-            raise Exception(msg.format(domain_size))
-
-        self.mapper = KM.MapperFactory.CreateMapper(
-            self.input_model_part,
-            self.interface_model_part,
-            mapper_settings)
-
-
-    def _CreateHDF5Parameters(self):
-        hdf5_settings = KM.Parameters()
-        hdf5_settings.AddValue("model_part_name", self.settings["input_model_part_name"])
-        hdf5_settings.AddValue("file_settings", self.settings["file_settings"])
-        data_settings = KM.Parameters("""{"list_of_variables" : ["MOMENTUM","VELOCITY","HEIGHT"]}""")
-        if self.settings["read_historical_database"].GetBool():
-            hdf5_settings.AddValue("nodal_solution_step_data_settings", data_settings)
-        else:
-            hdf5_settings.AddValue("nodal_data_value_settings", data_settings)
-        hdf5_process_settings = KM.Parameters()
-        hdf5_process_settings.AddValue("Parameters", hdf5_settings)
-        return hdf5_process_settings
-
-
-    def _SmoothDefaultValue(self):
-        elapsed_time = self.interface_model_part.ProcessInfo.GetValue(KM.DELTA_TIME)
-        semi_period = self.settings["semi_period_after_interval"].GetDouble()
-        for variable in self.variables:
-            SW.ShallowWaterUtilities().SmoothHistoricalVariable(
-                variable,
-                self.interface_model_part.Nodes,
-                elapsed_time,
-                semi_period)
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+import KratosMultiphysics.MappingApplication as Mapping
+from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
+from KratosMultiphysics.HDF5Application import import_model_part_from_hdf5_process
+from KratosMultiphysics.HDF5Application import single_mesh_temporal_input_process
+from os.path import commonprefix
+from pathlib import Path
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return DepthIntegrationInputProcess(model, settings["Parameters"])
+
+class DepthIntegrationInputProcess(KM.Process):
+    """DepthIntegrationInputProcess
+
+    Read the depth integrated values from an HDF5 file and set them as boundary conditions.
+    """
+
+    def GetDefaultParameters(self):
+        default_parameters = KM.Parameters("""{
+            "interface_model_part_name"   : "",
+            "input_model_part_name"       : "input_model_part",
+            "read_historical_database"    : false,
+            "interval"                    : [0.0,"End"],
+            "list_of_variables"           : ["MOMENTUM"],
+            "list_of_variables_to_fix"    : ["MOMENTUM_X","MOMENTUM_Y"],
+            "default_time_after_interval" : null,
+            "semi_period_after_interval"  : 1.0,
+            "swap_yz_axis"                : false,
+            "ignore_vertical_component"   : true,
+            "file_settings"               : {}
+        }""")
+        if self.settings.Has("default_time_after_interval"):
+            if self.settings["default_time_after_interval"].IsDouble():
+                default_parameters["default_time_after_interval"].SetDouble(0.0)
+        return default_parameters
+
+    def __init__(self, model, settings):
+        """The constructor of the DepthIntegrationInputProcess."""
+
+        KM.Process.__init__(self)
+        self.settings = settings
+        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
+
+        self.interface_model_part = model[self.settings["interface_model_part_name"].GetString()]
+        self.input_model_part = model.CreateModelPart(self.settings["input_model_part_name"].GetString())
+        self.interval = KM.IntervalUtility(self.settings)
+        self.variables = GenerateVariableListFromInput(self.settings["list_of_variables"])
+        self.variables_to_fix = GenerateVariableListFromInput(self.settings["list_of_variables_to_fix"])
+
+        self.hdf5_import = import_model_part_from_hdf5_process.Factory(self._CreateHDF5Parameters(), model)
+        self.hdf5_process = single_mesh_temporal_input_process.Factory(self._CreateHDF5Parameters(), model)
+        self._GetInputTimes(self.settings['file_settings'])
+
+
+    def Check(self):
+        '''Check the processes.'''
+        self.hdf5_import.Check()
+        self.hdf5_process.Check()
+        free_surface_is_present = False
+        height_is_present = False
+        for variable in self.variables:
+            if variable == SW.FREE_SURFACE_ELEVATION:
+                free_surface_is_present = True
+            if variable == SW.HEIGHT:
+                height_is_present = True
+        if free_surface_is_present and not height_is_present:
+            self.variables.append(SW.HEIGHT)
+
+
+    def ExecuteInitialize(self):
+        '''Read the input_model_part and set the variables.'''
+        self.hdf5_import.ExecuteInitialize()
+        self._CheckInputCoordinates()
+        self._CheckInputVariables()
+        self._CreateMapper()
+        self._MapToBoundaryCondition()
+
+
+    def ExecuteInitializeSolutionStep(self):
+        '''Set the variables in the input_model_part at the current time.'''
+        current_time = self.interface_model_part.ProcessInfo.GetValue(KM.TIME)
+        if self.interval.IsInInterval(current_time):
+            self._SetCurrentTime()
+            self.hdf5_process.ExecuteInitializeSolutionStep()
+            self._CheckInputVariables()
+            self._MapToBoundaryCondition()
+        else:
+            if self.settings["default_time_after_interval"] is not None:
+                self._SetDefaultTime()
+                self.hdf5_process.ExecuteInitializeSolutionStep()
+                self._CheckInputVariables()
+                self._MapToBoundaryCondition()
+                self._SmoothDefaultValue()
+
+
+    def _GetInputTimes(self, file_settings):
+        # Get all the file names
+        file = Path(file_settings["file_name"].GetString())
+        directory = file.parent
+        file_names = [str(f) for f in directory.glob("*.h5")]
+        if len(file_names) == 0:
+            msg = self.__class__.__name__ + ": The specified path is empty or does not exist: '{}'"
+            raise Exception(msg.format(directory))
+
+        # Find the common parts (prefix and suffix) of the found names and the file pattern
+        # The different part is the time, we need to store all the available times
+        file_pattern = str(file).replace('<model_part_name>', self.input_model_part.Name)
+        prefix = commonprefix([file_pattern, file_names[0]])
+        suffix = commonprefix([''.join(reversed(file_pattern)), ''.join(reversed(file_names[0]))])
+        suffix = ''.join(reversed(suffix))
+
+        # Store the times
+        self.times = []
+        for f in file_names:
+            f = f.replace(prefix, '')
+            f = f.replace(suffix, '')
+            try:
+                self.times.append(float(f))
+            except ValueError:
+                msg = self.__class__.__name__
+                msg += ": Trying to extract the time stamp from the input file name:\n"
+                msg += "\tExpected pattern: {}\n"
+                msg += "\tFound pattern:    {}<{}>{}"
+                KM.Logger.PrintInfo(msg.format(file_pattern, prefix, f, suffix))
+                raise
+        self.times.sort()
+
+
+    def _SetCurrentTime(self):
+        current_time = self.interface_model_part.ProcessInfo.GetValue(KM.TIME)
+        if current_time > self.times[-1]:
+            msg = self.__class__.__name__
+            msg += ": Looking for an input file at time {}. However, the input files end at time {}."
+            raise Exception(msg.format(current_time, self.times[-1]))
+        closest_time = next(filter(lambda x: x>current_time, self.times))
+        self.input_model_part.ProcessInfo.SetValue(KM.TIME, closest_time)
+
+
+    def _SetDefaultTime(self):
+        default_time = self.settings["default_time_after_interval"].GetDouble()
+        self.input_model_part.ProcessInfo.SetValue(KM.TIME, default_time)
+
+
+    def _CheckInputCoordinates(self):
+        if self.settings["swap_yz_axis"].GetBool():
+            SW.ShallowWaterUtilities().SwapYZCoordinates(self.input_model_part)
+            SW.ShallowWaterUtilities().SwapY0Z0Coordinates(self.input_model_part)
+        if self.settings["ignore_vertical_component"].GetBool():
+            SW.ShallowWaterUtilities().SetMeshZCoordinateToZero(self.input_model_part)
+            SW.ShallowWaterUtilities().SetMeshZ0CoordinateToZero(self.input_model_part)
+
+
+    def _CheckInputVariables(self):
+        if self.settings["swap_yz_axis"].GetBool():
+            if self.settings["read_historical_database"].GetBool():
+                SW.ShallowWaterUtilities().SwapYZComponents(KM.MOMENTUM, self.input_model_part.Nodes)
+                SW.ShallowWaterUtilities().SwapYZComponents(KM.VELOCITY, self.input_model_part.Nodes)
+            else:
+                SW.ShallowWaterUtilities().SwapYZComponentsNonHistorical(KM.MOMENTUM, self.input_model_part.Nodes)
+                SW.ShallowWaterUtilities().SwapYZComponentsNonHistorical(KM.VELOCITY, self.input_model_part.Nodes)
+        if self.settings["ignore_vertical_component"].GetBool():
+            if self.settings["read_historical_database"].GetBool():
+                KM.VariableUtils().SetVariableToZero(KM.MOMENTUM_Z, self.input_model_part.Nodes)
+                KM.VariableUtils().SetVariableToZero(KM.VELOCITY_Z, self.input_model_part.Nodes)
+            else:
+                KM.VariableUtils().SetNonHistoricalVariableToZero(KM.MOMENTUM_Z, self.input_model_part.Nodes)
+                KM.VariableUtils().SetNonHistoricalVariableToZero(KM.VELOCITY_Z, self.input_model_part.Nodes)
+
+
+    def _MapToBoundaryCondition(self):
+        for variable in self.variables:
+            if variable == SW.FREE_SURFACE_ELEVATION:
+                pass
+            else:
+                if self.settings["read_historical_database"].GetBool():
+                    self.mapper.Map(variable, variable)
+                else:
+                    self.mapper.Map(variable, variable, KM.Mapper.FROM_NON_HISTORICAL)
+
+        for variable in self.variables:
+            if variable == SW.FREE_SURFACE_ELEVATION:
+                SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.interface_model_part)
+            else:
+                pass
+
+        for variable in self.variables_to_fix:
+            KM.VariableUtils().ApplyFixity(variable, True, self.interface_model_part.Nodes)
+
+
+    def _CreateMapper(self):
+        domain_size = self.input_model_part.ProcessInfo[KM.DOMAIN_SIZE]
+        if domain_size == 2:
+            mapper_settings = KM.Parameters("""{
+                "mapper_type": "nearest_neighbor",
+                "echo_level" : 0,
+                "search_settings" : {
+                    "search_radius" : 0.0
+                }
+            }""")
+            min_point, max_point = KM.BoundingBox(self.interface_model_part.Nodes).GetPoints()
+            search_radius = 1.05 * (max_point - min_point).norm_2()
+            mapper_settings.AddEmptyValue("search_settings")
+            mapper_settings["search_settings"]["search_radius"].SetDouble(search_radius)
+        elif domain_size == 3:
+            mapper_settings = KM.Parameters("""{
+                "mapper_type": "nearest_neighbor",
+                "echo_level" : 0
+            }""")
+        else:
+            msg = self.__class__.__name__
+            msg += "._CreateMapper: The domain size of the input_model_part is: {}"
+            raise Exception(msg.format(domain_size))
+
+        self.mapper = KM.MapperFactory.CreateMapper(
+            self.input_model_part,
+            self.interface_model_part,
+            mapper_settings)
+
+
+    def _CreateHDF5Parameters(self):
+        hdf5_settings = KM.Parameters()
+        hdf5_settings.AddValue("model_part_name", self.settings["input_model_part_name"])
+        hdf5_settings.AddValue("file_settings", self.settings["file_settings"])
+        data_settings = KM.Parameters("""{"list_of_variables" : ["MOMENTUM","VELOCITY","HEIGHT"]}""")
+        if self.settings["read_historical_database"].GetBool():
+            hdf5_settings.AddValue("nodal_solution_step_data_settings", data_settings)
+        else:
+            hdf5_settings.AddValue("nodal_data_value_settings", data_settings)
+        hdf5_process_settings = KM.Parameters()
+        hdf5_process_settings.AddValue("Parameters", hdf5_settings)
+        return hdf5_process_settings
+
+
+    def _SmoothDefaultValue(self):
+        elapsed_time = self.interface_model_part.ProcessInfo.GetValue(KM.DELTA_TIME)
+        semi_period = self.settings["semi_period_after_interval"].GetDouble()
+        for variable in self.variables:
+            SW.ShallowWaterUtilities().SmoothHistoricalVariable(
+                variable,
+                self.interface_model_part.Nodes,
+                elapsed_time,
+                semi_period)
```

## KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_output_process.py

 * *Ordering differences only*

```diff
@@ -1,152 +1,152 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-from KratosMultiphysics.HDF5Application import single_mesh_temporal_output_process
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return DepthIntegrationOutputProcess(model, settings["Parameters"])
-
-class DepthIntegrationOutputProcess(KM.OutputProcess):
-    """DepthIntegrationOutputProcess
-
-    This process performs a depth integration from a Navier-Stokes domain to a shallow water domain.
-    The depth integration values are stored in the nodes of the shallow water domain and
-    printed in HDF5 format.
-    """
-
-    @staticmethod
-    def GetDefaultParameters():
-        return KM.Parameters("""{
-            "volume_model_part_name"    : "",
-            "interface_model_part_name" : "",
-            "output_model_part_name"    : "",
-            "store_historical_database" : false,
-            "extrapolate_boundaries"    : false,
-            "print_velocity_profile"    : false,
-            "interval"                  : [0.0,"End"],
-            "file_settings"             : {},
-            "output_time_settings"      : {}
-        }""")
-
-    def __init__(self, model, settings):
-        """The constructor of the DepthIntegrationOutputProcess"""
-
-        KM.OutputProcess.__init__(self)
-        self.settings = settings
-        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
-
-        self.volume_model_part = model[self.settings["volume_model_part_name"].GetString()]
-        self.interface_model_part = model[self.settings["interface_model_part_name"].GetString()]
-        self.output_model_part = model.CreateModelPart(self.settings["output_model_part_name"].GetString())
-        self.interval = KM.IntervalUtility(self.settings)
-        self.variables = [KM.VELOCITY, KM.MOMENTUM, SW.HEIGHT]
-
-        if self.volume_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 2:
-            self.integration_process = SW.DepthIntegrationProcess2D(model, self._CreateIntegrationParameters())
-        else:
-            self.integration_process = SW.DepthIntegrationProcess3D(model, self._CreateIntegrationParameters())
-        self.hdf5_process = single_mesh_temporal_output_process.Factory(self._CreateHDF5Parameters(), model)
-
-
-    def Check(self):
-        '''Check the processes.'''
-        self.integration_process.Check()
-        self.hdf5_process.Check()
-
-
-    def ExecuteInitialize(self):
-        '''Initialize the output model part.'''
-        self._InitializeOutputModelPart()
-        self._SetOutputProcessInfo()
-        if not self.settings["store_historical_database"].GetBool():
-            for var in self.variables:
-                KM.VariableUtils().SetNonHistoricalVariableToZero(var, self.interface_model_part.Nodes)
-                KM.VariableUtils().SetNonHistoricalVariableToZero(var, self.output_model_part.Nodes)
-
-
-    def ExecuteBeforeSolutionLoop(self):
-        '''Write the interface model part in HDF5 format.'''
-        self.integration_process.Execute()
-        self._MapToOutputModelPart()
-        self.hdf5_process.ExecuteBeforeSolutionLoop()
-
-
-    def ExecuteInitializeSolutionStep(self):
-        '''Synchronize the ProcessInfo of the output and interface model part.'''
-        self._SetOutputProcessInfo()
-
-
-    def IsOutputStep(self):
-        '''IsOutputStep.'''
-        # return self.hdf5_process.IsOutputstep()
-        return True
-
-
-    def PrintOutput(self):
-        '''Perform the depth integration over the interface model part.'''
-        self.integration_process.Execute()
-        self._MapToOutputModelPart()
-        self.hdf5_process.ExecuteFinalizeSolutionStep()
-
-
-    def _InitializeOutputModelPart(self):
-        if self.settings["store_historical_database"].GetBool():
-            self.output_model_part.AddNodalSolutionStepVariable(SW.HEIGHT)
-            self.output_model_part.AddNodalSolutionStepVariable(KM.MOMENTUM)
-            self.output_model_part.AddNodalSolutionStepVariable(KM.VELOCITY)
-        domain_size = self.volume_model_part.ProcessInfo[KM.DOMAIN_SIZE]
-        element_name = "Element{}D2N".format(domain_size)
-        condition_name = "LineCondition{}D2N".format(domain_size)
-        KM.DuplicateMeshModeler(self.interface_model_part).GenerateMesh(
-            self.output_model_part, element_name, condition_name)
-        self.output_model_part.ProcessInfo[KM.DOMAIN_SIZE] = domain_size
-
-
-    def _MapToOutputModelPart(self):
-        if self.settings["store_historical_database"].GetBool():
-            for variable in self.variables:
-                KM.VariableUtils().CopyModelPartNodalVar(
-                    variable,
-                    self.interface_model_part,
-                    self.output_model_part,
-                    0)
-        else:
-            for variable in self.variables:
-                KM.VariableUtils().CopyModelPartFlaggedNodalNonHistoricalVarToNonHistoricalVar(
-                    variable, variable,
-                    self.interface_model_part,
-                    self.output_model_part,
-                    KM.Flags(), False)
-
-
-    def _SetOutputProcessInfo(self):
-        time = self.interface_model_part.ProcessInfo[KM.TIME]
-        step = self.interface_model_part.ProcessInfo[KM.STEP]
-        self.output_model_part.ProcessInfo[KM.TIME] = time
-        self.output_model_part.ProcessInfo[KM.STEP] = step
-
-
-    def _CreateIntegrationParameters(self):
-        integration_settings = KM.Parameters()
-        integration_settings.AddValue("volume_model_part_name", self.settings["volume_model_part_name"])
-        integration_settings.AddValue("interface_model_part_name", self.settings["interface_model_part_name"])
-        integration_settings.AddValue("store_historical_database", self.settings["store_historical_database"])
-        integration_settings.AddValue("extrapolate_boundaries", self.settings["extrapolate_boundaries"])
-        integration_settings.AddValue("print_velocity_profile", self.settings["print_velocity_profile"])
-        return integration_settings
-
-
-    def _CreateHDF5Parameters(self):
-        hdf5_settings = KM.Parameters()
-        hdf5_settings.AddValue("model_part_name", self.settings["output_model_part_name"])
-        hdf5_settings.AddValue("file_settings", self.settings["file_settings"])
-        hdf5_settings.AddValue("output_time_settings", self.settings["output_time_settings"])
-        data_settings = KM.Parameters("""{"list_of_variables" : ["MOMENTUM","VELOCITY","HEIGHT"]}""")
-        if self.settings["store_historical_database"].GetBool():
-            hdf5_settings.AddValue("nodal_solution_step_data_settings", data_settings)
-        else:
-            hdf5_settings.AddValue("nodal_data_value_settings", data_settings)
-        hdf5_process_settings = KM.Parameters()
-        hdf5_process_settings.AddValue("Parameters", hdf5_settings)
-        return hdf5_process_settings
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+from KratosMultiphysics.HDF5Application import single_mesh_temporal_output_process
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return DepthIntegrationOutputProcess(model, settings["Parameters"])
+
+class DepthIntegrationOutputProcess(KM.OutputProcess):
+    """DepthIntegrationOutputProcess
+
+    This process performs a depth integration from a Navier-Stokes domain to a shallow water domain.
+    The depth integration values are stored in the nodes of the shallow water domain and
+    printed in HDF5 format.
+    """
+
+    @staticmethod
+    def GetDefaultParameters():
+        return KM.Parameters("""{
+            "volume_model_part_name"    : "",
+            "interface_model_part_name" : "",
+            "output_model_part_name"    : "",
+            "store_historical_database" : false,
+            "extrapolate_boundaries"    : false,
+            "print_velocity_profile"    : false,
+            "interval"                  : [0.0,"End"],
+            "file_settings"             : {},
+            "output_time_settings"      : {}
+        }""")
+
+    def __init__(self, model, settings):
+        """The constructor of the DepthIntegrationOutputProcess"""
+
+        KM.OutputProcess.__init__(self)
+        self.settings = settings
+        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
+
+        self.volume_model_part = model[self.settings["volume_model_part_name"].GetString()]
+        self.interface_model_part = model[self.settings["interface_model_part_name"].GetString()]
+        self.output_model_part = model.CreateModelPart(self.settings["output_model_part_name"].GetString())
+        self.interval = KM.IntervalUtility(self.settings)
+        self.variables = [KM.VELOCITY, KM.MOMENTUM, SW.HEIGHT]
+
+        if self.volume_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 2:
+            self.integration_process = SW.DepthIntegrationProcess2D(model, self._CreateIntegrationParameters())
+        else:
+            self.integration_process = SW.DepthIntegrationProcess3D(model, self._CreateIntegrationParameters())
+        self.hdf5_process = single_mesh_temporal_output_process.Factory(self._CreateHDF5Parameters(), model)
+
+
+    def Check(self):
+        '''Check the processes.'''
+        self.integration_process.Check()
+        self.hdf5_process.Check()
+
+
+    def ExecuteInitialize(self):
+        '''Initialize the output model part.'''
+        self._InitializeOutputModelPart()
+        self._SetOutputProcessInfo()
+        if not self.settings["store_historical_database"].GetBool():
+            for var in self.variables:
+                KM.VariableUtils().SetNonHistoricalVariableToZero(var, self.interface_model_part.Nodes)
+                KM.VariableUtils().SetNonHistoricalVariableToZero(var, self.output_model_part.Nodes)
+
+
+    def ExecuteBeforeSolutionLoop(self):
+        '''Write the interface model part in HDF5 format.'''
+        self.integration_process.Execute()
+        self._MapToOutputModelPart()
+        self.hdf5_process.ExecuteBeforeSolutionLoop()
+
+
+    def ExecuteInitializeSolutionStep(self):
+        '''Synchronize the ProcessInfo of the output and interface model part.'''
+        self._SetOutputProcessInfo()
+
+
+    def IsOutputStep(self):
+        '''IsOutputStep.'''
+        # return self.hdf5_process.IsOutputstep()
+        return True
+
+
+    def PrintOutput(self):
+        '''Perform the depth integration over the interface model part.'''
+        self.integration_process.Execute()
+        self._MapToOutputModelPart()
+        self.hdf5_process.ExecuteFinalizeSolutionStep()
+
+
+    def _InitializeOutputModelPart(self):
+        if self.settings["store_historical_database"].GetBool():
+            self.output_model_part.AddNodalSolutionStepVariable(SW.HEIGHT)
+            self.output_model_part.AddNodalSolutionStepVariable(KM.MOMENTUM)
+            self.output_model_part.AddNodalSolutionStepVariable(KM.VELOCITY)
+        domain_size = self.volume_model_part.ProcessInfo[KM.DOMAIN_SIZE]
+        element_name = "Element{}D2N".format(domain_size)
+        condition_name = "LineCondition{}D2N".format(domain_size)
+        KM.DuplicateMeshModeler(self.interface_model_part).GenerateMesh(
+            self.output_model_part, element_name, condition_name)
+        self.output_model_part.ProcessInfo[KM.DOMAIN_SIZE] = domain_size
+
+
+    def _MapToOutputModelPart(self):
+        if self.settings["store_historical_database"].GetBool():
+            for variable in self.variables:
+                KM.VariableUtils().CopyModelPartNodalVar(
+                    variable,
+                    self.interface_model_part,
+                    self.output_model_part,
+                    0)
+        else:
+            for variable in self.variables:
+                KM.VariableUtils().CopyModelPartFlaggedNodalNonHistoricalVarToNonHistoricalVar(
+                    variable, variable,
+                    self.interface_model_part,
+                    self.output_model_part,
+                    KM.Flags(), False)
+
+
+    def _SetOutputProcessInfo(self):
+        time = self.interface_model_part.ProcessInfo[KM.TIME]
+        step = self.interface_model_part.ProcessInfo[KM.STEP]
+        self.output_model_part.ProcessInfo[KM.TIME] = time
+        self.output_model_part.ProcessInfo[KM.STEP] = step
+
+
+    def _CreateIntegrationParameters(self):
+        integration_settings = KM.Parameters()
+        integration_settings.AddValue("volume_model_part_name", self.settings["volume_model_part_name"])
+        integration_settings.AddValue("interface_model_part_name", self.settings["interface_model_part_name"])
+        integration_settings.AddValue("store_historical_database", self.settings["store_historical_database"])
+        integration_settings.AddValue("extrapolate_boundaries", self.settings["extrapolate_boundaries"])
+        integration_settings.AddValue("print_velocity_profile", self.settings["print_velocity_profile"])
+        return integration_settings
+
+
+    def _CreateHDF5Parameters(self):
+        hdf5_settings = KM.Parameters()
+        hdf5_settings.AddValue("model_part_name", self.settings["output_model_part_name"])
+        hdf5_settings.AddValue("file_settings", self.settings["file_settings"])
+        hdf5_settings.AddValue("output_time_settings", self.settings["output_time_settings"])
+        data_settings = KM.Parameters("""{"list_of_variables" : ["MOMENTUM","VELOCITY","HEIGHT"]}""")
+        if self.settings["store_historical_database"].GetBool():
+            hdf5_settings.AddValue("nodal_solution_step_data_settings", data_settings)
+        else:
+            hdf5_settings.AddValue("nodal_data_value_settings", data_settings)
+        hdf5_process_settings = KM.Parameters()
+        hdf5_process_settings.AddValue("Parameters", hdf5_settings)
+        return hdf5_process_settings
```

## KratosMultiphysics/ShallowWaterApplication/coupling/read_from_sw_interface_process.py

 * *Ordering differences only*

```diff
@@ -1,344 +1,344 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-import KratosMultiphysics.MappingApplication as Mapping
-from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
-from KratosMultiphysics.HDF5Application import import_model_part_from_hdf5_process
-from KratosMultiphysics.HDF5Application import single_mesh_temporal_input_process
-from os.path import commonprefix
-from pathlib import Path
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ReadFromSwInterfaceProcess(model, settings["Parameters"])
-
-class ReadFromSwInterfaceProcess(KM.Process):
-    """ReadFromSwInterfaceProcess
-
-    Read the depth integrated values from an HDF5 file and set them as boundary conditions.
-    """
-
-    def GetDefaultParameters(self):
-        default_parameters = KM.Parameters("""{
-            "interface_model_part_name"   : "",
-            "input_model_part_name"       : "input_model_part",
-            "read_historical_database"    : false,
-            "interval"                    : [0.0,"End"],
-            "list_of_variables"           : ["MOMENTUM"],
-            "list_of_variables_to_fix"    : ["MOMENTUM_X","MOMENTUM_Y"],
-            "default_time_after_interval" : null,
-            "semi_period_after_interval"  : 1.0,
-            "swap_yz_axis"                : false,
-            "ignore_vertical_component"   : true,
-            "file_settings"               : {}
-        }""")
-        if self.settings.Has("default_time_after_interval"):
-            if self.settings["default_time_after_interval"].IsDouble():
-                default_parameters["default_time_after_interval"].SetDouble(0.0)
-        return default_parameters
-
-    def __init__(self, model, settings):
-        """The constructor of the ReadFromSwInterfaceProcess."""
-
-        KM.Process.__init__(self)
-        self.settings = settings
-        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
-
-        self.interface_model_part = model[self.settings["interface_model_part_name"].GetString()]
-        self.input_model_part = model.CreateModelPart(self.settings["input_model_part_name"].GetString())
-
-        self.interpolate_sw_to_pfem_utility = SW.InterpolateSwToPfemUtility()
-        
-        self.interval = KM.IntervalUtility(self.settings)
-        self.variables = GenerateVariableListFromInput(self.settings["list_of_variables"])
-        self.variables_to_fix = GenerateVariableListFromInput(self.settings["list_of_variables_to_fix"])
-        
-        self.hdf5_import = import_model_part_from_hdf5_process.Factory(self._CreateHDF5Parameters(), model)
-        
-        self.hdf5_process = single_mesh_temporal_input_process.Factory(self._CreateHDF5Parameters(), model)
-        self._GetInputTimes(self.settings['file_settings'])
-
-
-    def Check(self):
-        '''Check the processes.'''
-        self.hdf5_import.Check()
-        self.hdf5_process.Check()
-        free_surface_is_present = False
-        height_is_present = False
-        for variable in self.variables:
-            if variable == SW.FREE_SURFACE_ELEVATION:
-                free_surface_is_present = True
-            if variable == SW.HEIGHT:
-                height_is_present = True
-        if free_surface_is_present and not height_is_present:
-            self.variables.append(SW.HEIGHT)
-
-
-    def ExecuteInitialize(self):
-        '''Read the input_model_part and set the variables.'''
-        self.hdf5_import.ExecuteInitialize()
-        self._CheckInputCoordinates()
-        self.FindPfemHeight() 
-        self._CheckInputVariables()
-        
-
-    def ExecuteInitializeSolutionStep(self):
-        '''Set the variables in the input_model_part at the current time.'''
-        current_time = self.interface_model_part.ProcessInfo.GetValue(KM.TIME)
-        if self.interval.IsInInterval(current_time):
-            self._SetCurrentTime()
-            self.hdf5_process.ExecuteInitializeSolutionStep()
-            self.ComputeAverageValues()
-            self._CheckInputVariables()
-            self.DistributeVelocityToPfem()
-        else:
-            if self.settings["default_time_after_interval"] is not None:
-                self._SetDefaultTime()
-                self.hdf5_process.ExecuteInitializeSolutionStep()
-                self.ComputeAverageValues()
-                self._CheckInputVariables()
-                self.DistributeVelocityToPfem()
-                self._SmoothDefaultValue()
-
-    def ComputeAverageValues(self):
-        if self.interface_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 2:
-            avg_vel_x = 0.0
-            avg_h = 0.0
-            avg_vel_z = 0.0
-            n = 0
-            for node in self.input_model_part.Nodes:
-                n = n+1
-                avg_h         = avg_h      + node.GetValue(SW.HEIGHT) 
-                avg_vel_x     = avg_vel_x  + node.GetValue(KM.VELOCITY_X) 
-                avg_vel_z     = avg_vel_z  + node.GetValue(SW.VERTICAL_VELOCITY) 
-            self.avg_h = avg_h/n
-            self.avg_vel_x = avg_vel_x/n
-            self.avg_vel_z = avg_vel_z/n
-
-    def FindPfemHeight(self):
-        if self.interface_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 2:
-            ymin =  1e32
-            ymax = -1e32
-            for node in self.interface_model_part.Nodes:
-                if node.Y < ymin:
-                    ymin = node.Y 
-                if node.Y > ymax:
-                    ymax = node.Y
-            self.h_pfem = ymax - ymin
-            self.y_bottom = ymin
-        if self.interface_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 3:
-            zmax = -1e32
-            for node in self.interface_model_part.Nodes:
-                if node.Z > zmax:
-                    zmax = node.Z
-            self.z_top = zmax
-            
-            
-    def DistributeVelocityToPfem(self):
-        if self.interface_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 2:
-            self.Moving_v()
-
-        if self.interface_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 3:
-            self.interpolate_sw_to_pfem_utility.InterpolateVariables(self.interface_model_part,self.input_model_part)
-            for node in self.interface_model_part.Nodes:
-                
-                node_topography = node.GetValue(SW.TOPOGRAPHY)
-                self.h_pfem     = -node_topography
-                self.z_bottom   = self.z_top + node_topography
-                self.height   = node.GetValue(SW.HEIGHT)
-               
-                node.Z = (node.Z0 - self.z_bottom)*self.height/self.h_pfem + self.z_bottom
-                displacement = node.Z - node.Z0
-                node.SetSolutionStepValue(KM.DISPLACEMENT_Z, displacement)
-                
-                self.vel_z = node.GetValue(SW.VERTICAL_VELOCITY) 
-                vel_z_var  = (node.Z - self.z_bottom)/self.height*self.vel_z
-                vel_x      = node.GetValue(KM.VELOCITY_X)
-                vel_y      = node.GetValue(KM.VELOCITY_Y)
-                node.SetSolutionStepValue(KM.VELOCITY_X, vel_x)
-                node.SetSolutionStepValue(KM.VELOCITY_Y, vel_y)
-                node.SetSolutionStepValue(KM.VELOCITY_Z, vel_z_var)
-                
-
-    def Fixed_v0(self):
-        self.avg_vel_z = 0.0
-        self.vel_pfem   = self.avg_vel_x*self.avg_h/self.h_pfem
-        self.vel_pfem_z = self.avg_vel_z*self.avg_h/self.h_pfem
-        for node in self.interface_model_part.Nodes:
-            vel_z_var = self.vel_pfem_z*(node.Y - self.y_bottom)/self.h_pfem
-            node.SetSolutionStepValue(KM.VELOCITY_X, self.vel_pfem) 
-            node.SetSolutionStepValue(KM.VELOCITY_Y, vel_z_var)
-
-    def Fixed_v(self):
-        self.vel_pfem   = self.avg_vel_x*self.avg_h/self.h_pfem
-        self.vel_pfem_z = self.avg_vel_z*self.avg_h/self.h_pfem
-        for node in self.interface_model_part.Nodes:
-            vel_z_var = self.vel_pfem_z*(node.Y - self.y_bottom)/self.h_pfem
-            node.SetSolutionStepValue(KM.VELOCITY_X, self.vel_pfem) 
-            node.SetSolutionStepValue(KM.VELOCITY_Y, vel_z_var)
-
-    def Moving_v0(self):
-        for node in self.interface_model_part.Nodes:
-            node.Y = (node.Y0 - self.y_bottom)*self.avg_h/self.h_pfem + self.y_bottom
-            displacement = node.Y - node.Y0
-            node.SetSolutionStepValue(KM.DISPLACEMENT_Y, displacement)
-            vel_z_var = 0.0
-            node.SetSolutionStepValue(KM.VELOCITY_X, self.avg_vel_x)
-            node.SetSolutionStepValue(KM.VELOCITY_Y, vel_z_var) 
-
-    def Moving_v(self):
-        for node in self.interface_model_part.Nodes:
-            node.Y = (node.Y0 - self.y_bottom)*self.avg_h/self.h_pfem + self.y_bottom
-            displacement = node.Y - node.Y0
-            node.SetSolutionStepValue(KM.DISPLACEMENT_Y, displacement)
-            vel_z_var = self.avg_vel_z*(node.Y - self.y_bottom)/self.avg_h
-            node.SetSolutionStepValue(KM.VELOCITY_X, self.avg_vel_x)
-            node.SetSolutionStepValue(KM.VELOCITY_Y, vel_z_var) 
-
-    def _GetInputTimes(self, file_settings):
-        # Get all the file names
-        file = Path(file_settings["file_name"].GetString())
-        directory = file.parent
-        file_names = [str(f) for f in directory.glob("*.h5")]
-        if len(file_names) == 0:
-            msg = self.__class__.__name__ + ": The specified path is empty or does not exist: '{}'"
-            raise Exception(msg.format(directory))
-
-        # Find the common parts (prefix and suffix) of the found names and the file pattern
-        # The different part is the time, we need to store all the available times
-        file_pattern = str(file).replace('<model_part_name>', self.input_model_part.Name)
-        prefix = commonprefix([file_pattern, file_names[0]])
-        suffix = commonprefix([''.join(reversed(file_pattern)), ''.join(reversed(file_names[0]))])
-        suffix = ''.join(reversed(suffix))
-
-        # Store the times
-        self.times = []
-        for f in file_names:
-            f = f.replace(prefix, '')
-            f = f.replace(suffix, '')
-            try:
-                self.times.append(float(f))
-            except ValueError:
-                msg = self.__class__.__name__
-                msg += ": Trying to extract the time stamp from the input file name:\n"
-                msg += "\tExpected pattern: {}\n"
-                msg += "\tFound pattern:    {}<{}>{}"
-                KM.Logger.PrintInfo(msg.format(file_pattern, prefix, f, suffix))
-                raise
-        self.times.sort()
-
-
-    def _SetCurrentTime(self):
-        current_time = self.interface_model_part.ProcessInfo.GetValue(KM.TIME)
-        if current_time > self.times[-1]:
-            msg = self.__class__.__name__
-            msg += ": Looking for an input file at time {}. However, the input files end at time {}."
-            raise Exception(msg.format(current_time, self.times[-1]))
-        closest_time = next(filter(lambda x: x>current_time, self.times))
-        self.input_model_part.ProcessInfo.SetValue(KM.TIME, closest_time)
-
-
-    def _SetDefaultTime(self):
-        default_time = self.settings["default_time_after_interval"].GetDouble()
-        self.input_model_part.ProcessInfo.SetValue(KM.TIME, default_time)
-
-
-    def _CheckInputCoordinates(self):
-        if self.settings["swap_yz_axis"].GetBool():
-            SW.ShallowWaterUtilities().SwapYZCoordinates(self.input_model_part)
-            SW.ShallowWaterUtilities().SwapY0Z0Coordinates(self.input_model_part)
-        if self.settings["ignore_vertical_component"].GetBool():
-            SW.ShallowWaterUtilities().SetMeshZCoordinateToZero(self.input_model_part)
-            SW.ShallowWaterUtilities().SetMeshZ0CoordinateToZero(self.input_model_part)
-
-
-    def _CheckInputVariables(self):
-        if self.settings["swap_yz_axis"].GetBool():
-            if self.settings["read_historical_database"].GetBool():
-                SW.ShallowWaterUtilities().SwapYZComponents(KM.MOMENTUM, self.input_model_part.Nodes)
-                SW.ShallowWaterUtilities().SwapYZComponents(KM.VELOCITY, self.input_model_part.Nodes)
-            else:
-                SW.ShallowWaterUtilities().SwapYZComponentsNonHistorical(KM.MOMENTUM, self.input_model_part.Nodes)
-                SW.ShallowWaterUtilities().SwapYZComponentsNonHistorical(KM.VELOCITY, self.input_model_part.Nodes)
-        if self.settings["ignore_vertical_component"].GetBool():
-            if self.settings["read_historical_database"].GetBool():
-                KM.VariableUtils().SetVariableToZero(KM.MOMENTUM_Z, self.input_model_part.Nodes)
-                KM.VariableUtils().SetVariableToZero(KM.VELOCITY_Z, self.input_model_part.Nodes)
-            else:
-                KM.VariableUtils().SetNonHistoricalVariableToZero(KM.MOMENTUM_Z, self.input_model_part.Nodes)
-                KM.VariableUtils().SetNonHistoricalVariableToZero(KM.VELOCITY_Z, self.input_model_part.Nodes)
-
-
-    def _MapToBoundaryCondition(self):
-        for variable in self.variables:
-            if variable == SW.FREE_SURFACE_ELEVATION:
-                pass
-            else:
-                if self.settings["read_historical_database"].GetBool():
-                    self.mapper.Map(variable, variable)
-                else:
-                    self.mapper.Map(variable, variable, KM.Mapper.FROM_NON_HISTORICAL)
-
-        for variable in self.variables:
-            if variable == SW.FREE_SURFACE_ELEVATION:
-                SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.interface_model_part)
-            else:
-                pass
-
-        for variable in self.variables_to_fix:
-            KM.VariableUtils().ApplyFixity(variable, True, self.interface_model_part.Nodes)
-
-
-    def _CreateMapper(self):
-        domain_size = self.input_model_part.ProcessInfo[KM.DOMAIN_SIZE]
-        if domain_size == 2:
-            mapper_settings = KM.Parameters("""{
-                "mapper_type": "nearest_neighbor",
-                "echo_level" : 0,
-                "search_settings" : {
-                    "search_radius" : 0.0
-                }
-            }""")
-            min_point, max_point = KM.BoundingBox(self.interface_model_part.Nodes).GetPoints()
-            search_radius = 1.05 * (max_point - min_point).norm_2()
-            mapper_settings.AddEmptyValue("search_settings")
-            mapper_settings["search_settings"]["search_radius"].SetDouble(search_radius)
-        elif domain_size == 3:
-            mapper_settings = KM.Parameters("""{
-                "mapper_type": "nearest_neighbor",
-                "echo_level" : 0
-            }""")
-        else:
-            msg = self.__class__.__name__
-            msg += "._CreateMapper: The domain size of the input_model_part is: {}"
-            raise Exception(msg.format(domain_size))
-
-        self.mapper = KM.MapperFactory.CreateMapper(
-            self.input_model_part,
-            self.interface_model_part,
-            mapper_settings)
-
-
-    def _CreateHDF5Parameters(self):
-        hdf5_settings = KM.Parameters()
-        hdf5_settings.AddValue("model_part_name", self.settings["input_model_part_name"])
-        hdf5_settings.AddValue("file_settings", self.settings["file_settings"])
-        data_settings = KM.Parameters("""{"list_of_variables" : ["MOMENTUM","VELOCITY","HEIGHT","VERTICAL_VELOCITY","TOPOGRAPHY"]}""")
-        if self.settings["read_historical_database"].GetBool():
-            hdf5_settings.AddValue("nodal_solution_step_data_settings", data_settings)
-        else:
-            hdf5_settings.AddValue("nodal_data_value_settings", data_settings)
-        hdf5_process_settings = KM.Parameters()
-        hdf5_process_settings.AddValue("Parameters", hdf5_settings)
-        return hdf5_process_settings
-
-
-    def _SmoothDefaultValue(self):
-        elapsed_time = self.interface_model_part.ProcessInfo.GetValue(KM.DELTA_TIME)
-        semi_period = self.settings["semi_period_after_interval"].GetDouble()
-        for variable in self.variables:
-            SW.ShallowWaterUtilities().SmoothHistoricalVariable(
-                variable,
-                self.interface_model_part.Nodes,
-                elapsed_time,
-                semi_period)
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+import KratosMultiphysics.MappingApplication as Mapping
+from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
+from KratosMultiphysics.HDF5Application import import_model_part_from_hdf5_process
+from KratosMultiphysics.HDF5Application import single_mesh_temporal_input_process
+from os.path import commonprefix
+from pathlib import Path
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ReadFromSwInterfaceProcess(model, settings["Parameters"])
+
+class ReadFromSwInterfaceProcess(KM.Process):
+    """ReadFromSwInterfaceProcess
+
+    Read the depth integrated values from an HDF5 file and set them as boundary conditions.
+    """
+
+    def GetDefaultParameters(self):
+        default_parameters = KM.Parameters("""{
+            "interface_model_part_name"   : "",
+            "input_model_part_name"       : "input_model_part",
+            "read_historical_database"    : false,
+            "interval"                    : [0.0,"End"],
+            "list_of_variables"           : ["MOMENTUM"],
+            "list_of_variables_to_fix"    : ["MOMENTUM_X","MOMENTUM_Y"],
+            "default_time_after_interval" : null,
+            "semi_period_after_interval"  : 1.0,
+            "swap_yz_axis"                : false,
+            "ignore_vertical_component"   : true,
+            "file_settings"               : {}
+        }""")
+        if self.settings.Has("default_time_after_interval"):
+            if self.settings["default_time_after_interval"].IsDouble():
+                default_parameters["default_time_after_interval"].SetDouble(0.0)
+        return default_parameters
+
+    def __init__(self, model, settings):
+        """The constructor of the ReadFromSwInterfaceProcess."""
+
+        KM.Process.__init__(self)
+        self.settings = settings
+        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
+
+        self.interface_model_part = model[self.settings["interface_model_part_name"].GetString()]
+        self.input_model_part = model.CreateModelPart(self.settings["input_model_part_name"].GetString())
+
+        self.interpolate_sw_to_pfem_utility = SW.InterpolateSwToPfemUtility()
+        
+        self.interval = KM.IntervalUtility(self.settings)
+        self.variables = GenerateVariableListFromInput(self.settings["list_of_variables"])
+        self.variables_to_fix = GenerateVariableListFromInput(self.settings["list_of_variables_to_fix"])
+        
+        self.hdf5_import = import_model_part_from_hdf5_process.Factory(self._CreateHDF5Parameters(), model)
+        
+        self.hdf5_process = single_mesh_temporal_input_process.Factory(self._CreateHDF5Parameters(), model)
+        self._GetInputTimes(self.settings['file_settings'])
+
+
+    def Check(self):
+        '''Check the processes.'''
+        self.hdf5_import.Check()
+        self.hdf5_process.Check()
+        free_surface_is_present = False
+        height_is_present = False
+        for variable in self.variables:
+            if variable == SW.FREE_SURFACE_ELEVATION:
+                free_surface_is_present = True
+            if variable == SW.HEIGHT:
+                height_is_present = True
+        if free_surface_is_present and not height_is_present:
+            self.variables.append(SW.HEIGHT)
+
+
+    def ExecuteInitialize(self):
+        '''Read the input_model_part and set the variables.'''
+        self.hdf5_import.ExecuteInitialize()
+        self._CheckInputCoordinates()
+        self.FindPfemHeight() 
+        self._CheckInputVariables()
+        
+
+    def ExecuteInitializeSolutionStep(self):
+        '''Set the variables in the input_model_part at the current time.'''
+        current_time = self.interface_model_part.ProcessInfo.GetValue(KM.TIME)
+        if self.interval.IsInInterval(current_time):
+            self._SetCurrentTime()
+            self.hdf5_process.ExecuteInitializeSolutionStep()
+            self.ComputeAverageValues()
+            self._CheckInputVariables()
+            self.DistributeVelocityToPfem()
+        else:
+            if self.settings["default_time_after_interval"] is not None:
+                self._SetDefaultTime()
+                self.hdf5_process.ExecuteInitializeSolutionStep()
+                self.ComputeAverageValues()
+                self._CheckInputVariables()
+                self.DistributeVelocityToPfem()
+                self._SmoothDefaultValue()
+
+    def ComputeAverageValues(self):
+        if self.interface_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 2:
+            avg_vel_x = 0.0
+            avg_h = 0.0
+            avg_vel_z = 0.0
+            n = 0
+            for node in self.input_model_part.Nodes:
+                n = n+1
+                avg_h         = avg_h      + node.GetValue(SW.HEIGHT) 
+                avg_vel_x     = avg_vel_x  + node.GetValue(KM.VELOCITY_X) 
+                avg_vel_z     = avg_vel_z  + node.GetValue(SW.VERTICAL_VELOCITY) 
+            self.avg_h = avg_h/n
+            self.avg_vel_x = avg_vel_x/n
+            self.avg_vel_z = avg_vel_z/n
+
+    def FindPfemHeight(self):
+        if self.interface_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 2:
+            ymin =  1e32
+            ymax = -1e32
+            for node in self.interface_model_part.Nodes:
+                if node.Y < ymin:
+                    ymin = node.Y 
+                if node.Y > ymax:
+                    ymax = node.Y
+            self.h_pfem = ymax - ymin
+            self.y_bottom = ymin
+        if self.interface_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 3:
+            zmax = -1e32
+            for node in self.interface_model_part.Nodes:
+                if node.Z > zmax:
+                    zmax = node.Z
+            self.z_top = zmax
+            
+            
+    def DistributeVelocityToPfem(self):
+        if self.interface_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 2:
+            self.Moving_v()
+
+        if self.interface_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 3:
+            self.interpolate_sw_to_pfem_utility.InterpolateVariables(self.interface_model_part,self.input_model_part)
+            for node in self.interface_model_part.Nodes:
+                
+                node_topography = node.GetValue(SW.TOPOGRAPHY)
+                self.h_pfem     = -node_topography
+                self.z_bottom   = self.z_top + node_topography
+                self.height   = node.GetValue(SW.HEIGHT)
+               
+                node.Z = (node.Z0 - self.z_bottom)*self.height/self.h_pfem + self.z_bottom
+                displacement = node.Z - node.Z0
+                node.SetSolutionStepValue(KM.DISPLACEMENT_Z, displacement)
+                
+                self.vel_z = node.GetValue(SW.VERTICAL_VELOCITY) 
+                vel_z_var  = (node.Z - self.z_bottom)/self.height*self.vel_z
+                vel_x      = node.GetValue(KM.VELOCITY_X)
+                vel_y      = node.GetValue(KM.VELOCITY_Y)
+                node.SetSolutionStepValue(KM.VELOCITY_X, vel_x)
+                node.SetSolutionStepValue(KM.VELOCITY_Y, vel_y)
+                node.SetSolutionStepValue(KM.VELOCITY_Z, vel_z_var)
+                
+
+    def Fixed_v0(self):
+        self.avg_vel_z = 0.0
+        self.vel_pfem   = self.avg_vel_x*self.avg_h/self.h_pfem
+        self.vel_pfem_z = self.avg_vel_z*self.avg_h/self.h_pfem
+        for node in self.interface_model_part.Nodes:
+            vel_z_var = self.vel_pfem_z*(node.Y - self.y_bottom)/self.h_pfem
+            node.SetSolutionStepValue(KM.VELOCITY_X, self.vel_pfem) 
+            node.SetSolutionStepValue(KM.VELOCITY_Y, vel_z_var)
+
+    def Fixed_v(self):
+        self.vel_pfem   = self.avg_vel_x*self.avg_h/self.h_pfem
+        self.vel_pfem_z = self.avg_vel_z*self.avg_h/self.h_pfem
+        for node in self.interface_model_part.Nodes:
+            vel_z_var = self.vel_pfem_z*(node.Y - self.y_bottom)/self.h_pfem
+            node.SetSolutionStepValue(KM.VELOCITY_X, self.vel_pfem) 
+            node.SetSolutionStepValue(KM.VELOCITY_Y, vel_z_var)
+
+    def Moving_v0(self):
+        for node in self.interface_model_part.Nodes:
+            node.Y = (node.Y0 - self.y_bottom)*self.avg_h/self.h_pfem + self.y_bottom
+            displacement = node.Y - node.Y0
+            node.SetSolutionStepValue(KM.DISPLACEMENT_Y, displacement)
+            vel_z_var = 0.0
+            node.SetSolutionStepValue(KM.VELOCITY_X, self.avg_vel_x)
+            node.SetSolutionStepValue(KM.VELOCITY_Y, vel_z_var) 
+
+    def Moving_v(self):
+        for node in self.interface_model_part.Nodes:
+            node.Y = (node.Y0 - self.y_bottom)*self.avg_h/self.h_pfem + self.y_bottom
+            displacement = node.Y - node.Y0
+            node.SetSolutionStepValue(KM.DISPLACEMENT_Y, displacement)
+            vel_z_var = self.avg_vel_z*(node.Y - self.y_bottom)/self.avg_h
+            node.SetSolutionStepValue(KM.VELOCITY_X, self.avg_vel_x)
+            node.SetSolutionStepValue(KM.VELOCITY_Y, vel_z_var) 
+
+    def _GetInputTimes(self, file_settings):
+        # Get all the file names
+        file = Path(file_settings["file_name"].GetString())
+        directory = file.parent
+        file_names = [str(f) for f in directory.glob("*.h5")]
+        if len(file_names) == 0:
+            msg = self.__class__.__name__ + ": The specified path is empty or does not exist: '{}'"
+            raise Exception(msg.format(directory))
+
+        # Find the common parts (prefix and suffix) of the found names and the file pattern
+        # The different part is the time, we need to store all the available times
+        file_pattern = str(file).replace('<model_part_name>', self.input_model_part.Name)
+        prefix = commonprefix([file_pattern, file_names[0]])
+        suffix = commonprefix([''.join(reversed(file_pattern)), ''.join(reversed(file_names[0]))])
+        suffix = ''.join(reversed(suffix))
+
+        # Store the times
+        self.times = []
+        for f in file_names:
+            f = f.replace(prefix, '')
+            f = f.replace(suffix, '')
+            try:
+                self.times.append(float(f))
+            except ValueError:
+                msg = self.__class__.__name__
+                msg += ": Trying to extract the time stamp from the input file name:\n"
+                msg += "\tExpected pattern: {}\n"
+                msg += "\tFound pattern:    {}<{}>{}"
+                KM.Logger.PrintInfo(msg.format(file_pattern, prefix, f, suffix))
+                raise
+        self.times.sort()
+
+
+    def _SetCurrentTime(self):
+        current_time = self.interface_model_part.ProcessInfo.GetValue(KM.TIME)
+        if current_time > self.times[-1]:
+            msg = self.__class__.__name__
+            msg += ": Looking for an input file at time {}. However, the input files end at time {}."
+            raise Exception(msg.format(current_time, self.times[-1]))
+        closest_time = next(filter(lambda x: x>current_time, self.times))
+        self.input_model_part.ProcessInfo.SetValue(KM.TIME, closest_time)
+
+
+    def _SetDefaultTime(self):
+        default_time = self.settings["default_time_after_interval"].GetDouble()
+        self.input_model_part.ProcessInfo.SetValue(KM.TIME, default_time)
+
+
+    def _CheckInputCoordinates(self):
+        if self.settings["swap_yz_axis"].GetBool():
+            SW.ShallowWaterUtilities().SwapYZCoordinates(self.input_model_part)
+            SW.ShallowWaterUtilities().SwapY0Z0Coordinates(self.input_model_part)
+        if self.settings["ignore_vertical_component"].GetBool():
+            SW.ShallowWaterUtilities().SetMeshZCoordinateToZero(self.input_model_part)
+            SW.ShallowWaterUtilities().SetMeshZ0CoordinateToZero(self.input_model_part)
+
+
+    def _CheckInputVariables(self):
+        if self.settings["swap_yz_axis"].GetBool():
+            if self.settings["read_historical_database"].GetBool():
+                SW.ShallowWaterUtilities().SwapYZComponents(KM.MOMENTUM, self.input_model_part.Nodes)
+                SW.ShallowWaterUtilities().SwapYZComponents(KM.VELOCITY, self.input_model_part.Nodes)
+            else:
+                SW.ShallowWaterUtilities().SwapYZComponentsNonHistorical(KM.MOMENTUM, self.input_model_part.Nodes)
+                SW.ShallowWaterUtilities().SwapYZComponentsNonHistorical(KM.VELOCITY, self.input_model_part.Nodes)
+        if self.settings["ignore_vertical_component"].GetBool():
+            if self.settings["read_historical_database"].GetBool():
+                KM.VariableUtils().SetVariableToZero(KM.MOMENTUM_Z, self.input_model_part.Nodes)
+                KM.VariableUtils().SetVariableToZero(KM.VELOCITY_Z, self.input_model_part.Nodes)
+            else:
+                KM.VariableUtils().SetNonHistoricalVariableToZero(KM.MOMENTUM_Z, self.input_model_part.Nodes)
+                KM.VariableUtils().SetNonHistoricalVariableToZero(KM.VELOCITY_Z, self.input_model_part.Nodes)
+
+
+    def _MapToBoundaryCondition(self):
+        for variable in self.variables:
+            if variable == SW.FREE_SURFACE_ELEVATION:
+                pass
+            else:
+                if self.settings["read_historical_database"].GetBool():
+                    self.mapper.Map(variable, variable)
+                else:
+                    self.mapper.Map(variable, variable, KM.Mapper.FROM_NON_HISTORICAL)
+
+        for variable in self.variables:
+            if variable == SW.FREE_SURFACE_ELEVATION:
+                SW.ShallowWaterUtilities().ComputeFreeSurfaceElevation(self.interface_model_part)
+            else:
+                pass
+
+        for variable in self.variables_to_fix:
+            KM.VariableUtils().ApplyFixity(variable, True, self.interface_model_part.Nodes)
+
+
+    def _CreateMapper(self):
+        domain_size = self.input_model_part.ProcessInfo[KM.DOMAIN_SIZE]
+        if domain_size == 2:
+            mapper_settings = KM.Parameters("""{
+                "mapper_type": "nearest_neighbor",
+                "echo_level" : 0,
+                "search_settings" : {
+                    "search_radius" : 0.0
+                }
+            }""")
+            min_point, max_point = KM.BoundingBox(self.interface_model_part.Nodes).GetPoints()
+            search_radius = 1.05 * (max_point - min_point).norm_2()
+            mapper_settings.AddEmptyValue("search_settings")
+            mapper_settings["search_settings"]["search_radius"].SetDouble(search_radius)
+        elif domain_size == 3:
+            mapper_settings = KM.Parameters("""{
+                "mapper_type": "nearest_neighbor",
+                "echo_level" : 0
+            }""")
+        else:
+            msg = self.__class__.__name__
+            msg += "._CreateMapper: The domain size of the input_model_part is: {}"
+            raise Exception(msg.format(domain_size))
+
+        self.mapper = KM.MapperFactory.CreateMapper(
+            self.input_model_part,
+            self.interface_model_part,
+            mapper_settings)
+
+
+    def _CreateHDF5Parameters(self):
+        hdf5_settings = KM.Parameters()
+        hdf5_settings.AddValue("model_part_name", self.settings["input_model_part_name"])
+        hdf5_settings.AddValue("file_settings", self.settings["file_settings"])
+        data_settings = KM.Parameters("""{"list_of_variables" : ["MOMENTUM","VELOCITY","HEIGHT","VERTICAL_VELOCITY","TOPOGRAPHY"]}""")
+        if self.settings["read_historical_database"].GetBool():
+            hdf5_settings.AddValue("nodal_solution_step_data_settings", data_settings)
+        else:
+            hdf5_settings.AddValue("nodal_data_value_settings", data_settings)
+        hdf5_process_settings = KM.Parameters()
+        hdf5_process_settings.AddValue("Parameters", hdf5_settings)
+        return hdf5_process_settings
+
+
+    def _SmoothDefaultValue(self):
+        elapsed_time = self.interface_model_part.ProcessInfo.GetValue(KM.DELTA_TIME)
+        semi_period = self.settings["semi_period_after_interval"].GetDouble()
+        for variable in self.variables:
+            SW.ShallowWaterUtilities().SmoothHistoricalVariable(
+                variable,
+                self.interface_model_part.Nodes,
+                elapsed_time,
+                semi_period)
```

## KratosMultiphysics/ShallowWaterApplication/coupling/write_from_sw_at_interface_process.py

 * *Ordering differences only*

```diff
@@ -1,77 +1,77 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-from KratosMultiphysics.HDF5Application import single_mesh_temporal_output_process
-from KratosMultiphysics.ShallowWaterApplication.coupling import depth_integration_output_process as BaseProcess
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return WriteFromSwAtInterfaceProcess(model, settings["Parameters"])
-
-class WriteFromSwAtInterfaceProcess(BaseProcess.DepthIntegrationOutputProcess):
-    """WriteFromSwAtInterfaceProcess
-
-    This process stores the varialbes of a SW simulation into specific nodes, 
-    used as interface, and printed in HDF5 format.
-    """
-
-    @staticmethod
-    def GetDefaultParameters():
-        return KM.Parameters("""{
-            "volume_model_part_name"    : "",
-            "interface_model_part_name" : "",
-            "output_model_part_name"    : "",
-            "store_historical_database" : false,
-            "extrapolate_boundaries"    : false,
-            "print_velocity_profile"    : false,
-            "interval"                  : [0.0,"End"],
-            "file_settings"             : {},
-            "output_time_settings"      : {}
-        }""")
-
-    def __init__(self, model, settings):
-        """The constructor of the WriteFromSwAtInterfaceProcess"""
-
-        KM.OutputProcess.__init__(self)
-        self.settings = settings
-        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
-
-        self.volume_model_part = model[self.settings["volume_model_part_name"].GetString()]
-        self.interface_model_part = model[self.settings["interface_model_part_name"].GetString()]
-        self.output_model_part = model.CreateModelPart(self.settings["output_model_part_name"].GetString())
-        self.interval = KM.IntervalUtility(self.settings)
-        self.variables = [KM.VELOCITY, KM.MOMENTUM, SW.HEIGHT, SW.VERTICAL_VELOCITY, SW.TOPOGRAPHY]
-
-        if self.volume_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 2:
-            self.integration_process = SW.WriteFromSwAtInterfaceProcess2D(model, self._CreateIntegrationParameters())
-        else:
-            self.integration_process = SW.WriteFromSwAtInterfaceProcess3D(model, self._CreateIntegrationParameters())
-        self.hdf5_process = single_mesh_temporal_output_process.Factory(self._CreateHDF5Parameters(), model)
-
-    def _InitializeOutputModelPart(self):
-        if self.settings["store_historical_database"].GetBool():
-            self.output_model_part.AddNodalSolutionStepVariable(SW.HEIGHT)
-            self.output_model_part.AddNodalSolutionStepVariable(KM.MOMENTUM)
-            self.output_model_part.AddNodalSolutionStepVariable(KM.VELOCITY)
-            self.output_model_part.AddNodalSolutionStepVariable(SW.VERTICAL_VELOCITY)
-            self.output_model_part.AddNodalSolutionStepVariable(SW.TOPOGRAPHY)
-        domain_size = self.volume_model_part.ProcessInfo[KM.DOMAIN_SIZE]
-        element_name = "Element{}D2N".format(domain_size)
-        condition_name = "LineCondition{}D2N".format(domain_size)
-        KM.DuplicateMeshModeler(self.interface_model_part).GenerateMesh(
-            self.output_model_part, element_name, condition_name)
-        self.output_model_part.ProcessInfo[KM.DOMAIN_SIZE] = domain_size
-
-    def _CreateHDF5Parameters(self):
-        hdf5_settings = KM.Parameters()
-        hdf5_settings.AddValue("model_part_name", self.settings["output_model_part_name"])
-        hdf5_settings.AddValue("file_settings", self.settings["file_settings"])
-        hdf5_settings.AddValue("output_time_settings", self.settings["output_time_settings"])
-        data_settings = KM.Parameters("""{"list_of_variables" : ["MOMENTUM","VELOCITY","HEIGHT", "VERTICAL_VELOCITY","TOPOGRAPHY"]}""")
-        if self.settings["store_historical_database"].GetBool():
-            hdf5_settings.AddValue("nodal_solution_step_data_settings", data_settings)
-        else:
-            hdf5_settings.AddValue("nodal_data_value_settings", data_settings)
-        hdf5_process_settings = KM.Parameters()
-        hdf5_process_settings.AddValue("Parameters", hdf5_settings)
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+from KratosMultiphysics.HDF5Application import single_mesh_temporal_output_process
+from KratosMultiphysics.ShallowWaterApplication.coupling import depth_integration_output_process as BaseProcess
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return WriteFromSwAtInterfaceProcess(model, settings["Parameters"])
+
+class WriteFromSwAtInterfaceProcess(BaseProcess.DepthIntegrationOutputProcess):
+    """WriteFromSwAtInterfaceProcess
+
+    This process stores the varialbes of a SW simulation into specific nodes, 
+    used as interface, and printed in HDF5 format.
+    """
+
+    @staticmethod
+    def GetDefaultParameters():
+        return KM.Parameters("""{
+            "volume_model_part_name"    : "",
+            "interface_model_part_name" : "",
+            "output_model_part_name"    : "",
+            "store_historical_database" : false,
+            "extrapolate_boundaries"    : false,
+            "print_velocity_profile"    : false,
+            "interval"                  : [0.0,"End"],
+            "file_settings"             : {},
+            "output_time_settings"      : {}
+        }""")
+
+    def __init__(self, model, settings):
+        """The constructor of the WriteFromSwAtInterfaceProcess"""
+
+        KM.OutputProcess.__init__(self)
+        self.settings = settings
+        self.settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
+
+        self.volume_model_part = model[self.settings["volume_model_part_name"].GetString()]
+        self.interface_model_part = model[self.settings["interface_model_part_name"].GetString()]
+        self.output_model_part = model.CreateModelPart(self.settings["output_model_part_name"].GetString())
+        self.interval = KM.IntervalUtility(self.settings)
+        self.variables = [KM.VELOCITY, KM.MOMENTUM, SW.HEIGHT, SW.VERTICAL_VELOCITY, SW.TOPOGRAPHY]
+
+        if self.volume_model_part.ProcessInfo[KM.DOMAIN_SIZE] == 2:
+            self.integration_process = SW.WriteFromSwAtInterfaceProcess2D(model, self._CreateIntegrationParameters())
+        else:
+            self.integration_process = SW.WriteFromSwAtInterfaceProcess3D(model, self._CreateIntegrationParameters())
+        self.hdf5_process = single_mesh_temporal_output_process.Factory(self._CreateHDF5Parameters(), model)
+
+    def _InitializeOutputModelPart(self):
+        if self.settings["store_historical_database"].GetBool():
+            self.output_model_part.AddNodalSolutionStepVariable(SW.HEIGHT)
+            self.output_model_part.AddNodalSolutionStepVariable(KM.MOMENTUM)
+            self.output_model_part.AddNodalSolutionStepVariable(KM.VELOCITY)
+            self.output_model_part.AddNodalSolutionStepVariable(SW.VERTICAL_VELOCITY)
+            self.output_model_part.AddNodalSolutionStepVariable(SW.TOPOGRAPHY)
+        domain_size = self.volume_model_part.ProcessInfo[KM.DOMAIN_SIZE]
+        element_name = "Element{}D2N".format(domain_size)
+        condition_name = "LineCondition{}D2N".format(domain_size)
+        KM.DuplicateMeshModeler(self.interface_model_part).GenerateMesh(
+            self.output_model_part, element_name, condition_name)
+        self.output_model_part.ProcessInfo[KM.DOMAIN_SIZE] = domain_size
+
+    def _CreateHDF5Parameters(self):
+        hdf5_settings = KM.Parameters()
+        hdf5_settings.AddValue("model_part_name", self.settings["output_model_part_name"])
+        hdf5_settings.AddValue("file_settings", self.settings["file_settings"])
+        hdf5_settings.AddValue("output_time_settings", self.settings["output_time_settings"])
+        data_settings = KM.Parameters("""{"list_of_variables" : ["MOMENTUM","VELOCITY","HEIGHT", "VERTICAL_VELOCITY","TOPOGRAPHY"]}""")
+        if self.settings["store_historical_database"].GetBool():
+            hdf5_settings.AddValue("nodal_solution_step_data_settings", data_settings)
+        else:
+            hdf5_settings.AddValue("nodal_data_value_settings", data_settings)
+        hdf5_process_settings = KM.Parameters()
+        hdf5_process_settings.AddValue("Parameters", hdf5_settings)
         return hdf5_process_settings
```

## KratosMultiphysics/ShallowWaterApplication/modelers/dam_break_modeler.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-# importing the Kratos Library
-import KratosMultiphysics as KM
-
-## Import base class file
-from KratosMultiphysics.ShallowWaterApplication.benchmarks.dam_break_benchmark import DamBreakBenchmark
-
-def Factory(model, settings):
-    return DamBreakModeler(model, settings)
-
-class DamBreakModeler(KM.Modeler):
-    def __init__(self, model, settings):
-        super().__init__(model, settings)
-        self.process = DamBreakBenchmark(model, settings)
-
-    def PrepareGeometryModel(self):
-        self.process.ExecuteInitialize()
-        self.process.Check()
+# importing the Kratos Library
+import KratosMultiphysics as KM
+
+## Import base class file
+from KratosMultiphysics.ShallowWaterApplication.benchmarks.dam_break_benchmark import DamBreakBenchmark
+
+def Factory(model, settings):
+    return DamBreakModeler(model, settings)
+
+class DamBreakModeler(KM.Modeler):
+    def __init__(self, model, settings):
+        super().__init__(model, settings)
+        self.process = DamBreakBenchmark(model, settings)
+
+    def PrepareGeometryModel(self):
+        self.process.ExecuteInitialize()
+        self.process.Check()
```

## KratosMultiphysics/ShallowWaterApplication/modelers/planar_surface_in_parabola_modeler.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-# importing the Kratos Library
-import KratosMultiphysics as KM
-
-## Import base class file
-from KratosMultiphysics.ShallowWaterApplication.benchmarks.planar_surface_in_parabola_benchmark import PlanarSurfaceInParabolaBenchmark
-
-def Factory(model, settings):
-    return PlanarSurfaceInParabolaModeler(model, settings)
-
-class PlanarSurfaceInParabolaModeler(KM.Modeler):
-    def __init__(self, model, settings):
-        super().__init__(model, settings)
-        self.process = PlanarSurfaceInParabolaBenchmark(model, settings)
-
-    def PrepareGeometryModel(self):
-        self.process.ExecuteInitialize()
-        self.process.Check()
+# importing the Kratos Library
+import KratosMultiphysics as KM
+
+## Import base class file
+from KratosMultiphysics.ShallowWaterApplication.benchmarks.planar_surface_in_parabola_benchmark import PlanarSurfaceInParabolaBenchmark
+
+def Factory(model, settings):
+    return PlanarSurfaceInParabolaModeler(model, settings)
+
+class PlanarSurfaceInParabolaModeler(KM.Modeler):
+    def __init__(self, model, settings):
+        super().__init__(model, settings)
+        self.process = PlanarSurfaceInParabolaBenchmark(model, settings)
+
+    def PrepareGeometryModel(self):
+        self.process.ExecuteInitialize()
+        self.process.Check()
```

## KratosMultiphysics/ShallowWaterApplication/postprocess/auxiliary_nodes_visualization_process.py

 * *Ordering differences only*

```diff
@@ -1,93 +1,93 @@
-import KratosMultiphysics as KM
-from KratosMultiphysics.point_output_process import Interpolate
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return AuxiliaryNodesVisualizationProcess(model, settings["Parameters"])
-
-class AuxiliaryNodesVisualizationProcess(KM.Process):
-    """This class creates some auxiliary nodes.
-
-    If a reference model part is is specified, a mapping structure is created in
-    order to update the solution step data from the reference the auxiliary nodes.
-    The reference model part can be a specified by name or as the root model part.
-    """
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        return KM.Parameters('''{
-            "model_part_name"           : "",
-            "reference_model_part_name" : "",
-            "nodes_coordinates"         : [],
-            "search_configuration"      : "initial",
-            "search_tolerance"          : 1e-6
-        }''')
-
-    _search_configurations = {
-        "initial" : KM.Configuration.Initial,
-        "current" : KM.Configuration.Current
-    }
-
-    def __init__(self, model, settings):
-        """Constructor of the process."""
-        super().__init__()
-
-        # Validate settings
-        settings.AddMissingParameters(self.GetDefaultParameters())
-        self.settings = settings
-
-        # Retrieve the model part
-        self.model_part = model.CreateModelPart(self.settings["model_part_name"].GetString())
-        self.reference_model_part = None
-        if self.settings["reference_model_part_name"].GetString():
-            self.reference_model_part = model.CreateModelPart(self.settings["reference_model_part_name"].GetString())
-            self.model_part.ProcessInfo = self.reference_model_part.ProcessInfo
-            KM.MergeVariableListsUtility().Merge(self.reference_model_part, self.model_part)
-        elif self.model_part.IsSubModelPart():
-            self.reference_model_part = self.model_part.GetRootModelPart()
-
-    def ExecuteInitialize(self):
-        """Create the auxiliary nodes and set up the mapping structure."""
-        # Initialize the variables
-        if self.reference_model_part is not None:
-            self.node_id = self.reference_model_part.NumberOfNodes()
-            variables_names = self.model_part.GetHistoricalVariablesNames()
-            self.variables = [KM.KratosGlobals.GetVariable(name) for name in variables_names]
-        else:
-            self.node_id = 0
-
-        # Create the auxiliary geometries
-        for coord in self.settings["nodes_coordinates"]:
-            self._AddNode(coord)
-
-        # Initialize the mapping
-        if self.reference_model_part is not None:
-            self._SearchNodes()
-
-    def ExecuteBeforeOutputStep(self):
-        for node, entity, area_coords in zip(self.found_positions, self.entities, self.area_coords):
-            for variable in self.variables:
-                value = Interpolate(variable, entity, area_coords, historical_value=True)
-                node.SetSolutionStepValue(variable, value)
-
-    def _AddNode(self, params):
-        self.node_id += 1
-        coordinates = params.GetVector()
-        self.model_part.CreateNewNode(self.node_id, coordinates[0], coordinates[1], coordinates[2])
-
-    def _SearchNodes(self):
-        search_configuration = self._search_configurations[self.settings["search_configuration"].GetString()]
-        search_tolerance = self.settings["search_tolerance"].GetDouble()
-
-        self.entities = []
-        self.area_coords = []
-        self.found_positions = []
-
-        for node in self.model_part.Nodes:
-            sf_values = KM.Vector()
-            found_id = KM.BruteForcePointLocator(self.reference_model_part).FindElement(node, sf_values, search_configuration, search_tolerance)
-            if found_id > -1:
-                self.entities.append(self.reference_model_part.Elements[found_id])
-                self.area_coords.append(sf_values)
-                self.found_positions.append(node)
+import KratosMultiphysics as KM
+from KratosMultiphysics.point_output_process import Interpolate
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return AuxiliaryNodesVisualizationProcess(model, settings["Parameters"])
+
+class AuxiliaryNodesVisualizationProcess(KM.Process):
+    """This class creates some auxiliary nodes.
+
+    If a reference model part is is specified, a mapping structure is created in
+    order to update the solution step data from the reference the auxiliary nodes.
+    The reference model part can be a specified by name or as the root model part.
+    """
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        return KM.Parameters('''{
+            "model_part_name"           : "",
+            "reference_model_part_name" : "",
+            "nodes_coordinates"         : [],
+            "search_configuration"      : "initial",
+            "search_tolerance"          : 1e-6
+        }''')
+
+    _search_configurations = {
+        "initial" : KM.Configuration.Initial,
+        "current" : KM.Configuration.Current
+    }
+
+    def __init__(self, model, settings):
+        """Constructor of the process."""
+        super().__init__()
+
+        # Validate settings
+        settings.AddMissingParameters(self.GetDefaultParameters())
+        self.settings = settings
+
+        # Retrieve the model part
+        self.model_part = model.CreateModelPart(self.settings["model_part_name"].GetString())
+        self.reference_model_part = None
+        if self.settings["reference_model_part_name"].GetString():
+            self.reference_model_part = model.CreateModelPart(self.settings["reference_model_part_name"].GetString())
+            self.model_part.ProcessInfo = self.reference_model_part.ProcessInfo
+            KM.MergeVariableListsUtility().Merge(self.reference_model_part, self.model_part)
+        elif self.model_part.IsSubModelPart():
+            self.reference_model_part = self.model_part.GetRootModelPart()
+
+    def ExecuteInitialize(self):
+        """Create the auxiliary nodes and set up the mapping structure."""
+        # Initialize the variables
+        if self.reference_model_part is not None:
+            self.node_id = self.reference_model_part.NumberOfNodes()
+            variables_names = self.model_part.GetHistoricalVariablesNames()
+            self.variables = [KM.KratosGlobals.GetVariable(name) for name in variables_names]
+        else:
+            self.node_id = 0
+
+        # Create the auxiliary geometries
+        for coord in self.settings["nodes_coordinates"]:
+            self._AddNode(coord)
+
+        # Initialize the mapping
+        if self.reference_model_part is not None:
+            self._SearchNodes()
+
+    def ExecuteBeforeOutputStep(self):
+        for node, entity, area_coords in zip(self.found_positions, self.entities, self.area_coords):
+            for variable in self.variables:
+                value = Interpolate(variable, entity, area_coords, historical_value=True)
+                node.SetSolutionStepValue(variable, value)
+
+    def _AddNode(self, params):
+        self.node_id += 1
+        coordinates = params.GetVector()
+        self.model_part.CreateNewNode(self.node_id, coordinates[0], coordinates[1], coordinates[2])
+
+    def _SearchNodes(self):
+        search_configuration = self._search_configurations[self.settings["search_configuration"].GetString()]
+        search_tolerance = self.settings["search_tolerance"].GetDouble()
+
+        self.entities = []
+        self.area_coords = []
+        self.found_positions = []
+
+        for node in self.model_part.Nodes:
+            sf_values = KM.Vector()
+            found_id = KM.BruteForcePointLocator(self.reference_model_part).FindElement(node, sf_values, search_configuration, search_tolerance)
+            if found_id > -1:
+                self.entities.append(self.reference_model_part.Elements[found_id])
+                self.area_coords.append(sf_values)
+                self.found_positions.append(node)
```

## KratosMultiphysics/ShallowWaterApplication/postprocess/compute_froude_process.py

 * *Ordering differences only*

```diff
@@ -1,36 +1,36 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-def Factory(settings, Model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ComputeFroudeProcess(Model, settings["Parameters"])
-
-class ComputeFroudeProcess(KM.Process):
-    """Compute the Froude number before the output step."""
-
-    def __init__(self, Model, settings):
-
-        KM.Process.__init__(self)
-
-        default_settings = KM.Parameters("""
-        {
-            "model_part_name"      : "please_specify_model_part_name",
-            "save_as_historical"   : false,
-            "dry_height_threshold" : 1e-3
-        }
-        """)
-        settings.ValidateAndAssignDefaults(default_settings)
-        self.model_part = Model[settings["model_part_name"].GetString()]
-        self.save_as_historical = settings["save_as_historical"].GetBool()
-        self.dry_height_threshold = settings["dry_height_threshold"].GetDouble()
-
-    def ExecuteInitialize(self):
-        if not self.save_as_historical:
-            KM.VariableUtils().SetNonHistoricalVariableToZero(SW.FROUDE, self.model_part.Nodes)
-
-    def ExecuteBeforeOutputStep(self):
-        if self.save_as_historical:
-            SW.ShallowWaterUtilities().ComputeFroude(self.model_part, self.dry_height_threshold)
-        else:
-            SW.ShallowWaterUtilities().ComputeFroudeNonHistorical(self.model_part, self.dry_height_threshold)
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+def Factory(settings, Model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ComputeFroudeProcess(Model, settings["Parameters"])
+
+class ComputeFroudeProcess(KM.Process):
+    """Compute the Froude number before the output step."""
+
+    def __init__(self, Model, settings):
+
+        KM.Process.__init__(self)
+
+        default_settings = KM.Parameters("""
+        {
+            "model_part_name"      : "please_specify_model_part_name",
+            "save_as_historical"   : false,
+            "dry_height_threshold" : 1e-3
+        }
+        """)
+        settings.ValidateAndAssignDefaults(default_settings)
+        self.model_part = Model[settings["model_part_name"].GetString()]
+        self.save_as_historical = settings["save_as_historical"].GetBool()
+        self.dry_height_threshold = settings["dry_height_threshold"].GetDouble()
+
+    def ExecuteInitialize(self):
+        if not self.save_as_historical:
+            KM.VariableUtils().SetNonHistoricalVariableToZero(SW.FROUDE, self.model_part.Nodes)
+
+    def ExecuteBeforeOutputStep(self):
+        if self.save_as_historical:
+            SW.ShallowWaterUtilities().ComputeFroude(self.model_part, self.dry_height_threshold)
+        else:
+            SW.ShallowWaterUtilities().ComputeFroudeNonHistorical(self.model_part, self.dry_height_threshold)
```

## KratosMultiphysics/ShallowWaterApplication/postprocess/convergence_output_process.py

 * *Ordering differences only*

```diff
@@ -1,152 +1,152 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
-
-# Other imports
-import time
-from pathlib import Path
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ConvergenceOutputProcess(model, settings["Parameters"])
-
-class ConvergenceOutputProcess(KM.Process):
-
-    def __init__(self, model, settings):
-        super().__init__()
-
-        default_settings = KM.Parameters("""{
-                "model_part_name"       : "model_part",
-                "file_name"             : "output_file",
-                "printing_times"        : [],
-                "analysis_label"        : "label",
-                "convergence_variables" : [],
-                "low_corner"            : [],
-                "high_corner"           : []
-            }""")
-
-        self.settings = settings
-        self.settings.ValidateAndAssignDefaults(default_settings)
-
-        self.model_part = model[self.settings["model_part_name"].GetString()]
-        self.variables = GenerateVariableListFromInput(self.settings["convergence_variables"])
-
-        # Initialize output control variables
-        self.printing_times = self.settings["printing_times"].GetVector()
-        self.is_printed = [False] * len(self.printing_times)
-
-        if self.settings["low_corner"].GetVector().Size() == 0:
-            self.integrate_over_all_the_domain = True
-        else:
-            self.integrate_over_all_the_domain = False
-
-        self._InitializeOutputFile()
-
-
-    def ExecuteInitialize(self):
-        """Initialize the non historical variables and the measuring of computational time."""
-        for variable in self.variables:
-            KM.VariableUtils().SetNonHistoricalVariableToZero(variable, self.model_part.Nodes)
-        self.start_time = time.time()
-
-
-    def IsOutputStep(self):
-        """Check if the current time step is near enough to the specified printing times."""
-        time = self.model_part.ProcessInfo.GetValue(KM.TIME)
-        for i in range(len(self.printing_times)):
-            if time >= self.printing_times[i] and not self.is_printed[i]:
-                self.is_printed[i] = True
-                return True
-        return False
-
-
-    def PrintOutput(self):
-        """Write the values into the file."""
-        self._WriteAverageError()
-
-
-    def Check(self):
-        """Check the correctness of the input parameters."""
-        for variable in self.variables:
-            if not isinstance(variable, KM.DoubleVariable):
-                raise Exception("This process is expecting only double or component variables")
-        
-        low_corner = self.settings["low_corner"].GetVector()
-        high_corner = self.settings["high_corner"].GetVector()
-        if not low_corner.Size() == high_corner.Size():
-            raise Exception("The low and high corners do not have the same dimension")
-
-        if low_corner.Size() == 0:
-            pass
-        elif low_corner.Size() == 2:
-            self.settings["low_corner"].Append(0.0)
-            self.settings["high_corner"].Append(0.0)
-        elif low_corner.Size() == 3:
-            pass
-        else:
-            raise Exception("The corners must be specified with 2 or 3 coordinates")
-
-
-    def _InitializeOutputFile(self):
-        file_path = Path(self.settings["file_name"].GetString()).with_suffix('.dat')
-        file_path.touch(exist_ok=True)
-        header = self._GetHeader()
-        if file_path.stat().st_size == 0:
-            with open(file_path, 'w') as file:
-                file.write(header)
-        else:
-            existing_header = ''
-            with open(file_path, 'r') as file:
-                for i in range(2):
-                    existing_header += file.readline()
-            if existing_header != header:
-                msg = self.__class__.__name__ + ": "
-                msg += "The specified fields mismatch\n"
-                msg += "Existing header:\n"
-                msg += existing_header
-                msg += "Specified header:\n"
-                msg += header
-                raise Exception(msg)
-
-
-    def _GetHeader(self):
-        header = "# RMS for model part '{}' ".format(self.model_part.Name)
-        if self.integrate_over_all_the_domain:
-            header += "over all the domain\n"
-        else:
-            low_corner = KM.Point(self.settings["low_corner"].GetVector())
-            high_corner = KM.Point(self.settings["high_corner"].GetVector())
-            header += "over rectangle {} x {}\n".format(list(low_corner), list(high_corner))
-
-        header += "label num_nodes num_elems time_step time computational_time"
-        for variable in self.variables:
-            header += ' ' + variable.Name()
-        header += '\n'
-        return header
-
-
-    def _WriteAverageError(self):
-        data  = self.settings["analysis_label"].GetString() + ' '
-        data += str(self.model_part.NumberOfNodes()) + ' '
-        data += str(self.model_part.NumberOfElements()) + ' '
-        data += str(self.model_part.ProcessInfo[KM.DELTA_TIME]) + ' '
-        data += str(self.model_part.ProcessInfo[KM.TIME]) + ' '
-        data += str(time.time() - self.start_time)
-
-        if not self.integrate_over_all_the_domain:
-            low_corner = KM.Point(self.settings["low_corner"].GetVector())
-            high_corner = KM.Point(self.settings["high_corner"].GetVector())
-
-        for variable in self.variables:
-            if self.integrate_over_all_the_domain:
-                value = SW.ShallowWaterUtilities().ComputeL2NormNonHistorical(self.model_part, variable)
-            else:
-                value = SW.ShallowWaterUtilities().ComputeL2NormNonHistorical(self.model_part, variable, low_corner, high_corner)
-            data += ' {}'.format(value)
-        data += '\n'
-
-        file_path = Path(self.settings["file_name"].GetString()).with_suffix('.dat')
-        with open(file_path, 'a') as file:
-            file.write(data)
+# Importing the Kratos Library
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
+
+# Other imports
+import time
+from pathlib import Path
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ConvergenceOutputProcess(model, settings["Parameters"])
+
+class ConvergenceOutputProcess(KM.Process):
+
+    def __init__(self, model, settings):
+        super().__init__()
+
+        default_settings = KM.Parameters("""{
+                "model_part_name"       : "model_part",
+                "file_name"             : "output_file",
+                "printing_times"        : [],
+                "analysis_label"        : "label",
+                "convergence_variables" : [],
+                "low_corner"            : [],
+                "high_corner"           : []
+            }""")
+
+        self.settings = settings
+        self.settings.ValidateAndAssignDefaults(default_settings)
+
+        self.model_part = model[self.settings["model_part_name"].GetString()]
+        self.variables = GenerateVariableListFromInput(self.settings["convergence_variables"])
+
+        # Initialize output control variables
+        self.printing_times = self.settings["printing_times"].GetVector()
+        self.is_printed = [False] * len(self.printing_times)
+
+        if self.settings["low_corner"].GetVector().Size() == 0:
+            self.integrate_over_all_the_domain = True
+        else:
+            self.integrate_over_all_the_domain = False
+
+        self._InitializeOutputFile()
+
+
+    def ExecuteInitialize(self):
+        """Initialize the non historical variables and the measuring of computational time."""
+        for variable in self.variables:
+            KM.VariableUtils().SetNonHistoricalVariableToZero(variable, self.model_part.Nodes)
+        self.start_time = time.time()
+
+
+    def IsOutputStep(self):
+        """Check if the current time step is near enough to the specified printing times."""
+        time = self.model_part.ProcessInfo.GetValue(KM.TIME)
+        for i in range(len(self.printing_times)):
+            if time >= self.printing_times[i] and not self.is_printed[i]:
+                self.is_printed[i] = True
+                return True
+        return False
+
+
+    def PrintOutput(self):
+        """Write the values into the file."""
+        self._WriteAverageError()
+
+
+    def Check(self):
+        """Check the correctness of the input parameters."""
+        for variable in self.variables:
+            if not isinstance(variable, KM.DoubleVariable):
+                raise Exception("This process is expecting only double or component variables")
+        
+        low_corner = self.settings["low_corner"].GetVector()
+        high_corner = self.settings["high_corner"].GetVector()
+        if not low_corner.Size() == high_corner.Size():
+            raise Exception("The low and high corners do not have the same dimension")
+
+        if low_corner.Size() == 0:
+            pass
+        elif low_corner.Size() == 2:
+            self.settings["low_corner"].Append(0.0)
+            self.settings["high_corner"].Append(0.0)
+        elif low_corner.Size() == 3:
+            pass
+        else:
+            raise Exception("The corners must be specified with 2 or 3 coordinates")
+
+
+    def _InitializeOutputFile(self):
+        file_path = Path(self.settings["file_name"].GetString()).with_suffix('.dat')
+        file_path.touch(exist_ok=True)
+        header = self._GetHeader()
+        if file_path.stat().st_size == 0:
+            with open(file_path, 'w') as file:
+                file.write(header)
+        else:
+            existing_header = ''
+            with open(file_path, 'r') as file:
+                for i in range(2):
+                    existing_header += file.readline()
+            if existing_header != header:
+                msg = self.__class__.__name__ + ": "
+                msg += "The specified fields mismatch\n"
+                msg += "Existing header:\n"
+                msg += existing_header
+                msg += "Specified header:\n"
+                msg += header
+                raise Exception(msg)
+
+
+    def _GetHeader(self):
+        header = "# RMS for model part '{}' ".format(self.model_part.Name)
+        if self.integrate_over_all_the_domain:
+            header += "over all the domain\n"
+        else:
+            low_corner = KM.Point(self.settings["low_corner"].GetVector())
+            high_corner = KM.Point(self.settings["high_corner"].GetVector())
+            header += "over rectangle {} x {}\n".format(list(low_corner), list(high_corner))
+
+        header += "label num_nodes num_elems time_step time computational_time"
+        for variable in self.variables:
+            header += ' ' + variable.Name()
+        header += '\n'
+        return header
+
+
+    def _WriteAverageError(self):
+        data  = self.settings["analysis_label"].GetString() + ' '
+        data += str(self.model_part.NumberOfNodes()) + ' '
+        data += str(self.model_part.NumberOfElements()) + ' '
+        data += str(self.model_part.ProcessInfo[KM.DELTA_TIME]) + ' '
+        data += str(self.model_part.ProcessInfo[KM.TIME]) + ' '
+        data += str(time.time() - self.start_time)
+
+        if not self.integrate_over_all_the_domain:
+            low_corner = KM.Point(self.settings["low_corner"].GetVector())
+            high_corner = KM.Point(self.settings["high_corner"].GetVector())
+
+        for variable in self.variables:
+            if self.integrate_over_all_the_domain:
+                value = SW.ShallowWaterUtilities().ComputeL2NormNonHistorical(self.model_part, variable)
+            else:
+                value = SW.ShallowWaterUtilities().ComputeL2NormNonHistorical(self.model_part, variable, low_corner, high_corner)
+            data += ' {}'.format(value)
+        data += '\n'
+
+        file_path = Path(self.settings["file_name"].GetString()).with_suffix('.dat')
+        with open(file_path, 'a') as file:
+            file.write(data)
```

## KratosMultiphysics/ShallowWaterApplication/postprocess/generate_gid_list_file.py

 * *Ordering differences only*

```diff
@@ -1,38 +1,38 @@
-from pathlib import Path
-
-
-def GenerateGiDListFile(directories = [], file_name = ""):
-    files = []
-    for dir in directories:
-        files += _GetPostFilesList(Path(dir))
-    files.sort()
-    file_name = _ValidateFileName(file_name)
-    _WriteListFile(files, file_name)
-
-
-def _GetPostFilesList(directory):
-    files = list(directory.glob("*.post.bin"))
-    files.extend(list(directory.glob("*.post.res")))
-    return files
-
-
-def _ValidateFileName(file_name):
-    if not file_name:
-        file_name = Path.cwd().name
-    return Path(file_name).with_suffix("").with_suffix(".post.lst")
-
-
-def _WriteListFile(file_list, file_name):
-    with open(file_name, "w") as file:
-        file.write("Merge\n")
-        for output_file in file_list:
-            file.write("{}\n".format(output_file))
-
-
-if __name__ == "__main__":
-    import argparse
-    parser = argparse.ArgumentParser(description="Generate a GiD .post.lst file to merge the results from several simulations.")
-    parser.add_argument("directory", nargs="*", type=str, default=["."], help="where the post files are located. By default, the first location is the current directory")
-    parser.add_argument("-n", "--name", type=str, help="name of the output file. By default it is the current folder name")
-    args = parser.parse_args()
-    GenerateGiDListFile(args.directory, args.name)
+from pathlib import Path
+
+
+def GenerateGiDListFile(directories = [], file_name = ""):
+    files = []
+    for dir in directories:
+        files += _GetPostFilesList(Path(dir))
+    files.sort()
+    file_name = _ValidateFileName(file_name)
+    _WriteListFile(files, file_name)
+
+
+def _GetPostFilesList(directory):
+    files = list(directory.glob("*.post.bin"))
+    files.extend(list(directory.glob("*.post.res")))
+    return files
+
+
+def _ValidateFileName(file_name):
+    if not file_name:
+        file_name = Path.cwd().name
+    return Path(file_name).with_suffix("").with_suffix(".post.lst")
+
+
+def _WriteListFile(file_list, file_name):
+    with open(file_name, "w") as file:
+        file.write("Merge\n")
+        for output_file in file_list:
+            file.write("{}\n".format(output_file))
+
+
+if __name__ == "__main__":
+    import argparse
+    parser = argparse.ArgumentParser(description="Generate a GiD .post.lst file to merge the results from several simulations.")
+    parser.add_argument("directory", nargs="*", type=str, default=["."], help="where the post files are located. By default, the first location is the current directory")
+    parser.add_argument("-n", "--name", type=str, help="name of the output file. By default it is the current folder name")
+    args = parser.parse_args()
+    GenerateGiDListFile(args.directory, args.name)
```

## KratosMultiphysics/ShallowWaterApplication/postprocess/line_envelope_output_process.py

 * *Ordering differences only*

```diff
@@ -1,61 +1,61 @@
-import KratosMultiphysics as KM
-from KratosMultiphysics.time_based_ascii_file_writer_utility import TimeBasedAsciiFileWriterUtility
-from KratosMultiphysics.ShallowWaterApplication.postprocess.line_graph_output_process import LineGraphOutputProcess
-from KratosMultiphysics.point_output_process import Interpolate
-
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object")
-    return LineEnvelopeOutputProcess(model, settings["Parameters"])
-
-
-class LineEnvelopeOutputProcess(LineGraphOutputProcess):
-    """This process writes the maximum results along a line to generate a graph."""
-
-    def ExecuteBeforeSolutionLoop(self):
-        """Initialize the list of maximum values."""
-        super().ExecuteBeforeSolutionLoop()
-        num_of_vaviables = len(self.variables) + len(self.nonhistorical_variables)
-        self.values = [[-1e6] * num_of_vaviables for _ in self.found_positions]
-
-
-    def ExecuteFinalizeSolutionStep(self):
-        """Look for the maximum value."""
-        i = 0
-        for entity, area_coords in zip(self.entities, self.area_coords):
-            for v, var in enumerate(self.variables):
-                value = Interpolate(var, entity, area_coords, historical_value=True)
-                self.values[i][v] = max(self.values[i][v], value)
-            for v, var in enumerate(self.nonhistorical_variables):
-                value = Interpolate(var, entity, area_coords, historical_value=False)
-                self.values[i][v] = max(self.values[i][v], value)
-            i += 1
-
-
-    def PrintOutput(self):
-        """The output file is created, filled and closed.
-
-        The previous output files are overwitten. If the simulation
-        does not reach the end, an envelope will be kept.
-        """
-        self.file_settings["file_name"].SetString(self.file_name)
-        file = TimeBasedAsciiFileWriterUtility(self.model_part, self.file_settings, self._GetHeader()).file
-        for point, var_values in zip(self.found_positions, self.values):
-            file.write(self._DataToString(point, var_values))
-        file.close()
-
-
-    def _DataToString(self, node, values):
-        data = self.print_format.format(node.X)
-        data += " " + self.print_format.format(node.Y)
-        data += " " + self.print_format.format(node.Z)
-        for value in values:
-            data += " " + self.print_format.format(value)
-        return data + "\n"
-
-
-    def _GetHeader(self):
-        header = super()._GetHeader()
-        header = header.replace("Results", "Envelope")
-        return header
+import KratosMultiphysics as KM
+from KratosMultiphysics.time_based_ascii_file_writer_utility import TimeBasedAsciiFileWriterUtility
+from KratosMultiphysics.ShallowWaterApplication.postprocess.line_graph_output_process import LineGraphOutputProcess
+from KratosMultiphysics.point_output_process import Interpolate
+
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object")
+    return LineEnvelopeOutputProcess(model, settings["Parameters"])
+
+
+class LineEnvelopeOutputProcess(LineGraphOutputProcess):
+    """This process writes the maximum results along a line to generate a graph."""
+
+    def ExecuteBeforeSolutionLoop(self):
+        """Initialize the list of maximum values."""
+        super().ExecuteBeforeSolutionLoop()
+        num_of_vaviables = len(self.variables) + len(self.nonhistorical_variables)
+        self.values = [[-1e6] * num_of_vaviables for _ in self.found_positions]
+
+
+    def ExecuteFinalizeSolutionStep(self):
+        """Look for the maximum value."""
+        i = 0
+        for entity, area_coords in zip(self.entities, self.area_coords):
+            for v, var in enumerate(self.variables):
+                value = Interpolate(var, entity, area_coords, historical_value=True)
+                self.values[i][v] = max(self.values[i][v], value)
+            for v, var in enumerate(self.nonhistorical_variables):
+                value = Interpolate(var, entity, area_coords, historical_value=False)
+                self.values[i][v] = max(self.values[i][v], value)
+            i += 1
+
+
+    def PrintOutput(self):
+        """The output file is created, filled and closed.
+
+        The previous output files are overwitten. If the simulation
+        does not reach the end, an envelope will be kept.
+        """
+        self.file_settings["file_name"].SetString(self.file_name)
+        file = TimeBasedAsciiFileWriterUtility(self.model_part, self.file_settings, self._GetHeader()).file
+        for point, var_values in zip(self.found_positions, self.values):
+            file.write(self._DataToString(point, var_values))
+        file.close()
+
+
+    def _DataToString(self, node, values):
+        data = self.print_format.format(node.X)
+        data += " " + self.print_format.format(node.Y)
+        data += " " + self.print_format.format(node.Z)
+        for value in values:
+            data += " " + self.print_format.format(value)
+        return data + "\n"
+
+
+    def _GetHeader(self):
+        header = super()._GetHeader()
+        header = header.replace("Results", "Envelope")
+        return header
```

## KratosMultiphysics/ShallowWaterApplication/postprocess/line_graph_output_process.py

 * *Ordering differences only*

```diff
@@ -1,304 +1,304 @@
-import KratosMultiphysics as KM
-from KratosMultiphysics.time_based_ascii_file_writer_utility import TimeBasedAsciiFileWriterUtility
-from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput, DeleteFileIfExisting
-from KratosMultiphysics.point_output_process import Interpolate
-from pathlib import Path
-from numpy import linspace
-
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object")
-    return LineGraphOutputProcess(model, settings["Parameters"])
-
-
-class LineGraphOutputProcess(KM.OutputProcess):
-    """This process writes results along a line to generate a graph.
-    Every output step, an output file will be generated containing the graph data.
-    At the moment, MPI is not supported.
-    """
-
-    def GetDefaultParameters(self):
-        return KM.Parameters("""
-        {
-            "help"                    : "This process writes results from a geometrical object (line) in the model to a file. It first searches the entities containing the requested output location and then interpolates the requested variable(s). The output can be requested for elements, conditions and nodes. For nodes no geometrical interpolation is performed, the exact coordinates have to be specified.",
-            "model_part_name"         : "",
-            "entity_type"             : "element",
-            "interval"                : [0.0,"End"],
-            "start_point"             : [0, 0, 0],
-            "end_point"               : [0, 0, 0],
-            "sampling_points"         : 100,
-            "output_variables"        : [],
-            "nonhistorical_variables" : [],
-            "search_configuration"    : "initial",
-            "search_tolerance"        : 1e-6,
-            "print_format"            : "{:.6f}",
-            "time_format"             : "{:.3f}",
-            "output_file_settings"    : {
-                "file_name"               : "<model_part>",
-                "output_path"             : ""
-            },
-            "output_control_settings" : {
-                "output_control_type"     : "time",
-                "time_frequency"          : 1.0
-            }
-        }""")
-
-    def __init__(self, model, settings):
-        """Constructor of the class."""
-        super().__init__()
-
-        settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
-        self.model_part = model[settings["model_part_name"].GetString()]
-        self.interval = KM.IntervalUtility(settings)
-
-        # Retrieving the positions defining the line entity
-        start_point_position = settings["start_point"].GetVector()
-        if start_point_position.Size() != 3:
-            raise Exception('The start point position has to be provided with 3 coordinates!')
-        end_point_position = settings["end_point"].GetVector()
-        if end_point_position.Size() != 3:
-            raise Exception('The end point position has to be provided with 3 coordinates!')
-
-        # Get the number of points defining the line entity
-        number_of_sampling_points = settings["sampling_points"].GetInt()
-        if number_of_sampling_points <= 2:
-            raise Exception('The number of sampling points has to be larger than 2!')
-        parametrized_distances = linspace(0, 1, number_of_sampling_points)
-        increment = end_point_position - start_point_position
-        self.positions = [KM.Point(start_point_position + float(d)*increment) for d in parametrized_distances]
-
-        # Check the entity type
-        self.entity_type = settings["entity_type"].GetString()
-        if not (self.entity_type == "node" or self.entity_type == "element" or self.entity_type == "condition"):
-            raise Exception("Invalid 'entity_type' : {} (Expecting 'node', 'element' or 'condition')".format(self.entity_type))
-
-        # Retrieve the variables list
-        self.variables = self._GenerateVariablesList(settings["output_variables"], historical_value=True)
-        self.nonhistorical_variables = self._GenerateVariablesList(settings["nonhistorical_variables"], historical_value=False)
-
-        # Search settings
-        if settings["search_configuration"].GetString() == "initial":
-            self.search_configuration = KM.Configuration.Initial
-        elif settings["search_configuration"].GetString() == "current":
-            self.search_configuration = KM.Configuration.Current
-        else:
-            raise Exception("Invalid configuration: {} (Expecting 'initial' or 'current')".format(self.search_configuration))
-        self.search_tolerance = settings["search_tolerance"].GetDouble()
-
-        # Printing settings
-        self.print_format = settings["print_format"].GetString()
-        self.time_format = settings["time_format"].GetString()
-        self.file_settings = settings["output_file_settings"].Clone()
-
-        # Initialize output control
-        self.output_control = OutputControlFactory(self.model_part, settings["output_control_settings"])
-
-
-    def Check(self):
-        """Check the file settings."""
-
-        # Generate a dummy file to validate the parameters
-        file = TimeBasedAsciiFileWriterUtility(self.model_part, self.file_settings, "").file
-        file.close()
-        DeleteFileIfExisting(file.name)
-
-
-    def ExecuteBeforeSolutionLoop(self):
-        """Search the points and delete the existing files after the current time."""
-
-        # Get the file base name and check if there is a replacement
-        self.file_name = self.file_settings["file_name"].GetString()
-        self.file_name = self.file_name.replace("<model_part>", self.model_part.Name)
-
-        # Delete the previous files
-        time = self.model_part.ProcessInfo[KM.TIME]
-        self._DeleteExistingFiles(time)
-
-        # Perform the search
-        self._SearchPoints()
-
-
-    def IsOutputStep(self):
-        """Return if the current step is an output step."""
-
-        time = self.model_part.ProcessInfo[KM.TIME]
-        return self.interval.IsInInterval(time) and self.output_control.IsOutputStep()
-
-
-    def PrintOutput(self):
-        """The output file is created, filled and closed.
-        There will be one file for each printing step with the time as label.
-        """
-
-        time = self.model_part.ProcessInfo.GetValue(KM.TIME)
-        dummy_extension = ".z" #NOTE: the dummy extension will be replaced by the file utility. It is used to keep the decimals.
-        self.file_settings["file_name"].SetString(self.file_name + '_' + self.time_format.format(time) + dummy_extension)
-        file = TimeBasedAsciiFileWriterUtility(self.model_part, self.file_settings, self._GetHeader()).file
-        for point, entity, area_coords in zip(self.found_positions, self.entities, self.area_coords):
-            file.write(self._GetPointData(point, entity, area_coords))
-        file.close()
-
-
-    def _GenerateVariablesList(self, parameters, historical_value):
-        all_variables_list = GenerateVariableListFromInput(parameters)
-        variables = []
-        # Validate the types of variables
-        for var in all_variables_list:
-            if historical_value:
-                if not self.model_part.HasNodalSolutionStepVariable(var):
-                    raise Exception("ModelPart '{}' does not have {} as SolutionStepVariable".format(self.model_part.Name, var.Name()))
-            if isinstance(var, KM.DoubleVariable):
-                variables.append(var)
-            elif isinstance(var, KM.Array1DVariable3):
-                variables.append(KM.KratosGlobals.GetVariable(var.Name() + "_X"))
-                variables.append(KM.KratosGlobals.GetVariable(var.Name() + "_Y"))
-                variables.append(KM.KratosGlobals.GetVariable(var.Name() + "_Z"))
-            else:
-                raise Exception("The variable {} is not valid. It can only be double, component or array_3d".format(var.Name()))
-        return variables
-
-
-    def _SearchPoints(self):
-        self.entities = []
-        self.area_coords = []
-        self.found_positions = []
-        if self.entity_type == "node":
-            for point in self.positions:
-                found_id = KM.BruteForcePointLocator(self.model_part).FindNode(point, self.search_configuration, self.search_tolerance)
-                if found_id > -1:
-                    self.entities.append(self.model_part.Nodes[found_id])
-                    self.area_coords.append("dummy") # needed for looping later
-                    self.found_positions.append(point)
-        elif self.entity_type == "element":
-            for point in self.positions:
-                self.sf_values = KM.Vector()
-                found_id = KM.BruteForcePointLocator(self.model_part).FindElement(point, self.sf_values, self.search_configuration, self.search_tolerance)
-                if found_id > -1:
-                    self.entities.append(self.model_part.Elements[found_id])
-                    self.area_coords.append(self.sf_values)
-                    self.found_positions.append(point)
-        elif self.entity_type == "condition":
-            for point in self.positions:
-                self.sf_values = KM.Vector()
-                found_id = KM.BruteForcePointLocator(self.model_part).FindCondition(point, self.sf_values, self.search_configuration, self.search_tolerance)
-                if found_id > -1:
-                    self.entities.append(self.model_part.Conditions[found_id])
-                    self.area_coords.append(self.sf_values)
-                    self.found_positions.append(point)
-
-
-    def _GetHeader(self):
-        if len(self.found_positions) > 1:
-            start = list(self.found_positions[0])
-            end = list(self.found_positions[-1])
-        else:
-            start = "'NOT FOUND'"
-            end = "'NOT FOUND'"
-        time = self.model_part.ProcessInfo[KM.TIME]
-        header = "# Results for '{}s' over line {}-{} at time {}\n#".format(self.entity_type, start, end, time)
-        coordinates = ["X", "Y", "Z"]
-        for c in coordinates:
-            header += " " + c
-        for var in self.variables:
-            header += " " + var.Name()
-        for var in self.nonhistorical_variables:
-            header += " " + var.Name()
-        return header + "\n"
-
-
-    def _GetPointData(self, node, entity, area_coords):
-        data = self.print_format.format(node.X)
-        data += " " + self.print_format.format(node.Y)
-        data += " " + self.print_format.format(node.Z)
-        for var in self.variables:
-            data += " " + self.print_format.format(Interpolate(var, entity, area_coords, historical_value=True))
-        for var in self.nonhistorical_variables:
-            data += " " + self.print_format.format(Interpolate(var, entity, area_coords, historical_value=False))
-        return data + "\n"
-
-
-    def _DeleteExistingFiles(self, time):
-        output_path = self.file_settings["output_path"].GetString()
-        file_extension = self.file_settings["file_extension"].GetString()
-        for dir in Path(output_path).glob(self.file_name + "*." + file_extension):
-            file_time = dir.stem.split("-")[-1]
-            try:
-                file_time = float(file_time)
-                if file_time >= time:
-                    DeleteFileIfExisting(dir)
-            except ValueError:
-                pass
-
-
-
-
-# TODO: move this to a common place
-
-def OutputControlFactory(model_part, parameters):
-    if not parameters.Has("output_control_type"):
-        raise Exception ("OutputControlFactory. There is no 'output_control_settings' key in the parameters.")
-    output_control_type = parameters["output_control_type"].GetString()
-
-    output_control_types = {
-        "time" : TimeOutputControl,
-        "step" : StepOutputControl
-    }
-    module = output_control_types[output_control_type]
-    return module(model_part, parameters)
-
-class OutputControl():
-
-    @staticmethod
-    def IsOutputStep():
-        return True
-
-    @staticmethod
-    def GetDefaultParameters():
-        return KM.Parameters()
-
-class TimeOutputControl(OutputControl):
-
-    @staticmethod
-    def GetDefaultParameters():
-        return KM.Parameters("""{
-            "output_control_type"     : "time",
-            "time_frequency"          : 1.0
-        }""")
-
-    def __init__(self, model_part, parameters):
-        parameters.ValidateAndAssignDefaults(self.GetDefaultParameters())
-        self.time_frequency = parameters["time_frequency"].GetDouble()
-        self.model_part = model_part
-        self.next_output = 0.0
-
-    def IsOutputStep(self):
-        time = self.model_part.ProcessInfo[KM.TIME]
-        if time >= self.next_output:
-            while time >= self.next_output:
-                self.next_output += self.time_frequency
-            return True
-        return False
-
-class StepOutputControl(OutputControl):
-
-    @staticmethod
-    def GetDefaultParameters():
-        return KM.Parameters("""{
-            "output_control_type"     : "step",
-            "step_frequency"          : 1
-        }""")
-
-    def __init__(self, model_part, parameters):
-        parameters.ValidateAndAssignDefaults(self.GetDefaultParameters())
-        self.step_frequency = parameters["step_frequency"].GetDouble()
-        self.model_part = model_part
-        self.next_output = 0
-
-    def IsOutputStep(self):
-        step = self.model_part.ProcessInfo[KM.STEP]
-        if step >= self.next_output:
-            while step >= self.next_output:
-                self.next_output += self.step_frequency
-            return True
-        return False
+import KratosMultiphysics as KM
+from KratosMultiphysics.time_based_ascii_file_writer_utility import TimeBasedAsciiFileWriterUtility
+from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput, DeleteFileIfExisting
+from KratosMultiphysics.point_output_process import Interpolate
+from pathlib import Path
+from numpy import linspace
+
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object")
+    return LineGraphOutputProcess(model, settings["Parameters"])
+
+
+class LineGraphOutputProcess(KM.OutputProcess):
+    """This process writes results along a line to generate a graph.
+    Every output step, an output file will be generated containing the graph data.
+    At the moment, MPI is not supported.
+    """
+
+    def GetDefaultParameters(self):
+        return KM.Parameters("""
+        {
+            "help"                    : "This process writes results from a geometrical object (line) in the model to a file. It first searches the entities containing the requested output location and then interpolates the requested variable(s). The output can be requested for elements, conditions and nodes. For nodes no geometrical interpolation is performed, the exact coordinates have to be specified.",
+            "model_part_name"         : "",
+            "entity_type"             : "element",
+            "interval"                : [0.0,"End"],
+            "start_point"             : [0, 0, 0],
+            "end_point"               : [0, 0, 0],
+            "sampling_points"         : 100,
+            "output_variables"        : [],
+            "nonhistorical_variables" : [],
+            "search_configuration"    : "initial",
+            "search_tolerance"        : 1e-6,
+            "print_format"            : "{:.6f}",
+            "time_format"             : "{:.3f}",
+            "output_file_settings"    : {
+                "file_name"               : "<model_part>",
+                "output_path"             : ""
+            },
+            "output_control_settings" : {
+                "output_control_type"     : "time",
+                "time_frequency"          : 1.0
+            }
+        }""")
+
+    def __init__(self, model, settings):
+        """Constructor of the class."""
+        super().__init__()
+
+        settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
+        self.model_part = model[settings["model_part_name"].GetString()]
+        self.interval = KM.IntervalUtility(settings)
+
+        # Retrieving the positions defining the line entity
+        start_point_position = settings["start_point"].GetVector()
+        if start_point_position.Size() != 3:
+            raise Exception('The start point position has to be provided with 3 coordinates!')
+        end_point_position = settings["end_point"].GetVector()
+        if end_point_position.Size() != 3:
+            raise Exception('The end point position has to be provided with 3 coordinates!')
+
+        # Get the number of points defining the line entity
+        number_of_sampling_points = settings["sampling_points"].GetInt()
+        if number_of_sampling_points <= 2:
+            raise Exception('The number of sampling points has to be larger than 2!')
+        parametrized_distances = linspace(0, 1, number_of_sampling_points)
+        increment = end_point_position - start_point_position
+        self.positions = [KM.Point(start_point_position + float(d)*increment) for d in parametrized_distances]
+
+        # Check the entity type
+        self.entity_type = settings["entity_type"].GetString()
+        if not (self.entity_type == "node" or self.entity_type == "element" or self.entity_type == "condition"):
+            raise Exception("Invalid 'entity_type' : {} (Expecting 'node', 'element' or 'condition')".format(self.entity_type))
+
+        # Retrieve the variables list
+        self.variables = self._GenerateVariablesList(settings["output_variables"], historical_value=True)
+        self.nonhistorical_variables = self._GenerateVariablesList(settings["nonhistorical_variables"], historical_value=False)
+
+        # Search settings
+        if settings["search_configuration"].GetString() == "initial":
+            self.search_configuration = KM.Configuration.Initial
+        elif settings["search_configuration"].GetString() == "current":
+            self.search_configuration = KM.Configuration.Current
+        else:
+            raise Exception("Invalid configuration: {} (Expecting 'initial' or 'current')".format(self.search_configuration))
+        self.search_tolerance = settings["search_tolerance"].GetDouble()
+
+        # Printing settings
+        self.print_format = settings["print_format"].GetString()
+        self.time_format = settings["time_format"].GetString()
+        self.file_settings = settings["output_file_settings"].Clone()
+
+        # Initialize output control
+        self.output_control = OutputControlFactory(self.model_part, settings["output_control_settings"])
+
+
+    def Check(self):
+        """Check the file settings."""
+
+        # Generate a dummy file to validate the parameters
+        file = TimeBasedAsciiFileWriterUtility(self.model_part, self.file_settings, "").file
+        file.close()
+        DeleteFileIfExisting(file.name)
+
+
+    def ExecuteBeforeSolutionLoop(self):
+        """Search the points and delete the existing files after the current time."""
+
+        # Get the file base name and check if there is a replacement
+        self.file_name = self.file_settings["file_name"].GetString()
+        self.file_name = self.file_name.replace("<model_part>", self.model_part.Name)
+
+        # Delete the previous files
+        time = self.model_part.ProcessInfo[KM.TIME]
+        self._DeleteExistingFiles(time)
+
+        # Perform the search
+        self._SearchPoints()
+
+
+    def IsOutputStep(self):
+        """Return if the current step is an output step."""
+
+        time = self.model_part.ProcessInfo[KM.TIME]
+        return self.interval.IsInInterval(time) and self.output_control.IsOutputStep()
+
+
+    def PrintOutput(self):
+        """The output file is created, filled and closed.
+        There will be one file for each printing step with the time as label.
+        """
+
+        time = self.model_part.ProcessInfo.GetValue(KM.TIME)
+        dummy_extension = ".z" #NOTE: the dummy extension will be replaced by the file utility. It is used to keep the decimals.
+        self.file_settings["file_name"].SetString(self.file_name + '_' + self.time_format.format(time) + dummy_extension)
+        file = TimeBasedAsciiFileWriterUtility(self.model_part, self.file_settings, self._GetHeader()).file
+        for point, entity, area_coords in zip(self.found_positions, self.entities, self.area_coords):
+            file.write(self._GetPointData(point, entity, area_coords))
+        file.close()
+
+
+    def _GenerateVariablesList(self, parameters, historical_value):
+        all_variables_list = GenerateVariableListFromInput(parameters)
+        variables = []
+        # Validate the types of variables
+        for var in all_variables_list:
+            if historical_value:
+                if not self.model_part.HasNodalSolutionStepVariable(var):
+                    raise Exception("ModelPart '{}' does not have {} as SolutionStepVariable".format(self.model_part.Name, var.Name()))
+            if isinstance(var, KM.DoubleVariable):
+                variables.append(var)
+            elif isinstance(var, KM.Array1DVariable3):
+                variables.append(KM.KratosGlobals.GetVariable(var.Name() + "_X"))
+                variables.append(KM.KratosGlobals.GetVariable(var.Name() + "_Y"))
+                variables.append(KM.KratosGlobals.GetVariable(var.Name() + "_Z"))
+            else:
+                raise Exception("The variable {} is not valid. It can only be double, component or array_3d".format(var.Name()))
+        return variables
+
+
+    def _SearchPoints(self):
+        self.entities = []
+        self.area_coords = []
+        self.found_positions = []
+        if self.entity_type == "node":
+            for point in self.positions:
+                found_id = KM.BruteForcePointLocator(self.model_part).FindNode(point, self.search_configuration, self.search_tolerance)
+                if found_id > -1:
+                    self.entities.append(self.model_part.Nodes[found_id])
+                    self.area_coords.append("dummy") # needed for looping later
+                    self.found_positions.append(point)
+        elif self.entity_type == "element":
+            for point in self.positions:
+                self.sf_values = KM.Vector()
+                found_id = KM.BruteForcePointLocator(self.model_part).FindElement(point, self.sf_values, self.search_configuration, self.search_tolerance)
+                if found_id > -1:
+                    self.entities.append(self.model_part.Elements[found_id])
+                    self.area_coords.append(self.sf_values)
+                    self.found_positions.append(point)
+        elif self.entity_type == "condition":
+            for point in self.positions:
+                self.sf_values = KM.Vector()
+                found_id = KM.BruteForcePointLocator(self.model_part).FindCondition(point, self.sf_values, self.search_configuration, self.search_tolerance)
+                if found_id > -1:
+                    self.entities.append(self.model_part.Conditions[found_id])
+                    self.area_coords.append(self.sf_values)
+                    self.found_positions.append(point)
+
+
+    def _GetHeader(self):
+        if len(self.found_positions) > 1:
+            start = list(self.found_positions[0])
+            end = list(self.found_positions[-1])
+        else:
+            start = "'NOT FOUND'"
+            end = "'NOT FOUND'"
+        time = self.model_part.ProcessInfo[KM.TIME]
+        header = "# Results for '{}s' over line {}-{} at time {}\n#".format(self.entity_type, start, end, time)
+        coordinates = ["X", "Y", "Z"]
+        for c in coordinates:
+            header += " " + c
+        for var in self.variables:
+            header += " " + var.Name()
+        for var in self.nonhistorical_variables:
+            header += " " + var.Name()
+        return header + "\n"
+
+
+    def _GetPointData(self, node, entity, area_coords):
+        data = self.print_format.format(node.X)
+        data += " " + self.print_format.format(node.Y)
+        data += " " + self.print_format.format(node.Z)
+        for var in self.variables:
+            data += " " + self.print_format.format(Interpolate(var, entity, area_coords, historical_value=True))
+        for var in self.nonhistorical_variables:
+            data += " " + self.print_format.format(Interpolate(var, entity, area_coords, historical_value=False))
+        return data + "\n"
+
+
+    def _DeleteExistingFiles(self, time):
+        output_path = self.file_settings["output_path"].GetString()
+        file_extension = self.file_settings["file_extension"].GetString()
+        for dir in Path(output_path).glob(self.file_name + "*." + file_extension):
+            file_time = dir.stem.split("-")[-1]
+            try:
+                file_time = float(file_time)
+                if file_time >= time:
+                    DeleteFileIfExisting(dir)
+            except ValueError:
+                pass
+
+
+
+
+# TODO: move this to a common place
+
+def OutputControlFactory(model_part, parameters):
+    if not parameters.Has("output_control_type"):
+        raise Exception ("OutputControlFactory. There is no 'output_control_settings' key in the parameters.")
+    output_control_type = parameters["output_control_type"].GetString()
+
+    output_control_types = {
+        "time" : TimeOutputControl,
+        "step" : StepOutputControl
+    }
+    module = output_control_types[output_control_type]
+    return module(model_part, parameters)
+
+class OutputControl():
+
+    @staticmethod
+    def IsOutputStep():
+        return True
+
+    @staticmethod
+    def GetDefaultParameters():
+        return KM.Parameters()
+
+class TimeOutputControl(OutputControl):
+
+    @staticmethod
+    def GetDefaultParameters():
+        return KM.Parameters("""{
+            "output_control_type"     : "time",
+            "time_frequency"          : 1.0
+        }""")
+
+    def __init__(self, model_part, parameters):
+        parameters.ValidateAndAssignDefaults(self.GetDefaultParameters())
+        self.time_frequency = parameters["time_frequency"].GetDouble()
+        self.model_part = model_part
+        self.next_output = 0.0
+
+    def IsOutputStep(self):
+        time = self.model_part.ProcessInfo[KM.TIME]
+        if time >= self.next_output:
+            while time >= self.next_output:
+                self.next_output += self.time_frequency
+            return True
+        return False
+
+class StepOutputControl(OutputControl):
+
+    @staticmethod
+    def GetDefaultParameters():
+        return KM.Parameters("""{
+            "output_control_type"     : "step",
+            "step_frequency"          : 1
+        }""")
+
+    def __init__(self, model_part, parameters):
+        parameters.ValidateAndAssignDefaults(self.GetDefaultParameters())
+        self.step_frequency = parameters["step_frequency"].GetDouble()
+        self.model_part = model_part
+        self.next_output = 0
+
+    def IsOutputStep(self):
+        step = self.model_part.ProcessInfo[KM.STEP]
+        if step >= self.next_output:
+            while step >= self.next_output:
+                self.next_output += self.step_frequency
+            return True
+        return False
```

## KratosMultiphysics/ShallowWaterApplication/postprocess/offset_ids_process.py

 * *Ordering differences only*

```diff
@@ -1,66 +1,66 @@
-# Importing Kratos library
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return OffsetIdsProcess(model, settings["Parameters"])
-
-class OffsetIdsProcess(KM.Process):
-
-    """ SwapCoordinatesAndOffsetIdsProcess.
-
-    This process offsets the ids in order to differentiate several model parts
-    at post-processing level.
-    """
-
-    def __init__(self, model, settings):
-        """Constructor of the class."""
-        KM.Process.__init__(self)
-
-        default_settings = KM.Parameters("""{
-                "model_part_name"        : "model_part_name",
-                "nodes_ids_offset"       : 0,
-                "elements_ids_offset"    : 0,
-                "conditions_ids_offset"  : 0,
-                "properties_ids_offset"  : 0
-            }""")
-        settings.ValidateAndAssignDefaults(default_settings)
-
-        self.model_part = model[settings["model_part_name"].GetString()]
-        self.nodes_ids_offset = settings["nodes_ids_offset"].GetInt()
-        self.elements_ids_offset = settings["elements_ids_offset"].GetInt()
-        self.conditions_ids_offset = settings["conditions_ids_offset"].GetInt()
-        self.properties_ids_offset = settings["properties_ids_offset"].GetInt()
-
-        self.execute_initialize_solution_step_is_called = False
-
-
-    def ExecuteBeforeSolutionLoop(self):
-        """Perform the transformation before printing the initial mesh."""
-        self.ExecuteBeforeOutputStep()
-
-
-    def ExecuteInitializeSolutionStep(self):
-        """Undo the transformation after the initial mesh is printed."""
-        if not self.execute_initialize_solution_step_is_called:
-            self.ExecuteAfterOutputStep()
-            self.execute_initialize_solution_step_is_called = True
-
-
-    def ExecuteBeforeOutputStep(self):
-        """Offset the Ids."""
-        self._OffsetIds()
-
-
-    def ExecuteAfterOutputStep(self):
-        """Restore the Ids offset."""
-        self._OffsetIds(-1)
-
-
-    def _OffsetIds(self, sign=1):
-        SW.ShallowWaterUtilities().OffsetIds(self.model_part.Nodes, sign * self.nodes_ids_offset)
-        SW.ShallowWaterUtilities().OffsetIds(self.model_part.Elements, sign * self.elements_ids_offset)
-        SW.ShallowWaterUtilities().OffsetIds(self.model_part.Conditions, sign * self.conditions_ids_offset)
-        SW.ShallowWaterUtilities().OffsetIds(self.model_part.Properties, sign * self.properties_ids_offset)
+# Importing Kratos library
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return OffsetIdsProcess(model, settings["Parameters"])
+
+class OffsetIdsProcess(KM.Process):
+
+    """ SwapCoordinatesAndOffsetIdsProcess.
+
+    This process offsets the ids in order to differentiate several model parts
+    at post-processing level.
+    """
+
+    def __init__(self, model, settings):
+        """Constructor of the class."""
+        KM.Process.__init__(self)
+
+        default_settings = KM.Parameters("""{
+                "model_part_name"        : "model_part_name",
+                "nodes_ids_offset"       : 0,
+                "elements_ids_offset"    : 0,
+                "conditions_ids_offset"  : 0,
+                "properties_ids_offset"  : 0
+            }""")
+        settings.ValidateAndAssignDefaults(default_settings)
+
+        self.model_part = model[settings["model_part_name"].GetString()]
+        self.nodes_ids_offset = settings["nodes_ids_offset"].GetInt()
+        self.elements_ids_offset = settings["elements_ids_offset"].GetInt()
+        self.conditions_ids_offset = settings["conditions_ids_offset"].GetInt()
+        self.properties_ids_offset = settings["properties_ids_offset"].GetInt()
+
+        self.execute_initialize_solution_step_is_called = False
+
+
+    def ExecuteBeforeSolutionLoop(self):
+        """Perform the transformation before printing the initial mesh."""
+        self.ExecuteBeforeOutputStep()
+
+
+    def ExecuteInitializeSolutionStep(self):
+        """Undo the transformation after the initial mesh is printed."""
+        if not self.execute_initialize_solution_step_is_called:
+            self.ExecuteAfterOutputStep()
+            self.execute_initialize_solution_step_is_called = True
+
+
+    def ExecuteBeforeOutputStep(self):
+        """Offset the Ids."""
+        self._OffsetIds()
+
+
+    def ExecuteAfterOutputStep(self):
+        """Restore the Ids offset."""
+        self._OffsetIds(-1)
+
+
+    def _OffsetIds(self, sign=1):
+        SW.ShallowWaterUtilities().OffsetIds(self.model_part.Nodes, sign * self.nodes_ids_offset)
+        SW.ShallowWaterUtilities().OffsetIds(self.model_part.Elements, sign * self.elements_ids_offset)
+        SW.ShallowWaterUtilities().OffsetIds(self.model_part.Conditions, sign * self.conditions_ids_offset)
+        SW.ShallowWaterUtilities().OffsetIds(self.model_part.Properties, sign * self.properties_ids_offset)
```

## KratosMultiphysics/ShallowWaterApplication/postprocess/swap_coordinates_process.py

 * *Ordering differences only*

```diff
@@ -1,55 +1,55 @@
-# Importing Kratos library
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return SwapCoordinatesProcess(model, settings["Parameters"])
-
-class SwapCoordinatesProcess(KM.Process):
-
-    """ SwapCoordinatesProcess.
-
-    This process swaps the YZ coordinates of a model part in order to merge several
-    2D simulations for post-processing purpose.
-    """
-
-    def __init__(self, model, settings):
-        """Constructor of the class."""
-        KM.Process.__init__(self)
-
-        default_settings = KM.Parameters("""{
-                "model_part_name"        : "model_part_name"
-            }""")
-
-        settings.ValidateAndAssignDefaults(default_settings)
-        self.model_part = model[settings["model_part_name"].GetString()]
-        self.execute_initialize_solution_step_is_called = False
-
-
-    def ExecuteBeforeSolutionLoop(self):
-        """Perform the transformation before printing the initial mesh."""
-        self.ExecuteBeforeOutputStep()
-
-
-    def ExecuteInitializeSolutionStep(self):
-        """Undo the transformation after the initial mesh is printed."""
-        if not self.execute_initialize_solution_step_is_called:
-            self.ExecuteAfterOutputStep()
-            self.execute_initialize_solution_step_is_called = True
-
-
-    def ExecuteBeforeOutputStep(self):
-        """Swap the mesh."""
-        self._SwapYZCoordinates()
-
-
-    def ExecuteAfterOutputStep(self):
-        """Restore the mesh swapping."""
-        self._SwapYZCoordinates()
-
-
-    def _SwapYZCoordinates(self):
-        SW.ShallowWaterUtilities().SwapYZCoordinates(self.model_part)
-        SW.ShallowWaterUtilities().SwapY0Z0Coordinates(self.model_part)
+# Importing Kratos library
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return SwapCoordinatesProcess(model, settings["Parameters"])
+
+class SwapCoordinatesProcess(KM.Process):
+
+    """ SwapCoordinatesProcess.
+
+    This process swaps the YZ coordinates of a model part in order to merge several
+    2D simulations for post-processing purpose.
+    """
+
+    def __init__(self, model, settings):
+        """Constructor of the class."""
+        KM.Process.__init__(self)
+
+        default_settings = KM.Parameters("""{
+                "model_part_name"        : "model_part_name"
+            }""")
+
+        settings.ValidateAndAssignDefaults(default_settings)
+        self.model_part = model[settings["model_part_name"].GetString()]
+        self.execute_initialize_solution_step_is_called = False
+
+
+    def ExecuteBeforeSolutionLoop(self):
+        """Perform the transformation before printing the initial mesh."""
+        self.ExecuteBeforeOutputStep()
+
+
+    def ExecuteInitializeSolutionStep(self):
+        """Undo the transformation after the initial mesh is printed."""
+        if not self.execute_initialize_solution_step_is_called:
+            self.ExecuteAfterOutputStep()
+            self.execute_initialize_solution_step_is_called = True
+
+
+    def ExecuteBeforeOutputStep(self):
+        """Swap the mesh."""
+        self._SwapYZCoordinates()
+
+
+    def ExecuteAfterOutputStep(self):
+        """Restore the mesh swapping."""
+        self._SwapYZCoordinates()
+
+
+    def _SwapYZCoordinates(self):
+        SW.ShallowWaterUtilities().SwapYZCoordinates(self.model_part)
+        SW.ShallowWaterUtilities().SwapY0Z0Coordinates(self.model_part)
```

## KratosMultiphysics/ShallowWaterApplication/postprocess/visualization_mesh_process.py

 * *Ordering differences only*

```diff
@@ -1,211 +1,211 @@
-# Importing Kratos library
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-# Importing useful utilities
-from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return VisualizationMeshProcess(model, settings["Parameters"])
-
-class VisualizationMeshProcess(KM.Process):
-    """ VisualizationMeshProcess.
-
-    This process provides several tools for post-processing.
-    - Generation of an auxiliary model part for the topography visualization as a separate file.
-    - Setting the TOPOGRAPHY and FREE_SURFACE_ELEVATION into DISPLACEMENT_Z or Z-coordinate in order to view the mesh deformation.
-    - Saving the HEIGHT and FREE_SURFACE_ELEVATION as non-historical only on wet nodes. Dry nodes are set with the no-data value of GiD.
-    """
-
-    @staticmethod
-    def GetDefaultParameters():
-        return KM.Parameters("""
-            {
-                "model_part_name"                : "model_part_name",
-                "topographic_model_part_name"    : "",
-                "free_surface_deformation_mode"  : "nodal_displacement",
-                "topography_deformation_mode"    : "z_coordinate",
-                "nodal_historical_displacement"  : false,
-                "mean_water_level"               : 0.0,
-                "nodal_variables_to_transfer"    : [],
-                "nonhistorical_variables_to_transfer" : []
-            }
-            """)
-
-    _mesh_deformation_modes = {
-        "z_coordinate"       : True,
-        "nodal_displacement" : False
-    }
-
-    def __init__(self, model, settings):
-        """Constructor with Model and Parameters."""
-
-        KM.Process.__init__(self)
-        self.model = model
-        settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
-
-        self.computing_model_part = self.model[settings["model_part_name"].GetString()]
-
-        # Get the deformation mode options
-        self.deform_free_surface = self._GetDeformMeshFlag(settings["free_surface_deformation_mode"])
-        self.deform_topography = self._GetDeformMeshFlag(settings["topography_deformation_mode"])
-        self.nodal_historical_displacement = settings["nodal_historical_displacement"].GetBool()
-        self.mean_water_level = settings["mean_water_level"].GetDouble()
-
-        # Creating the topographic model part if specified
-        self.topographic_model_part = None
-        self.duplicate_model_part = False
-        topographic_model_part_name = settings["topographic_model_part_name"].GetString()
-        if topographic_model_part_name:
-            self.topographic_model_part = self.model.CreateModelPart(topographic_model_part_name)
-            if self._IsEmpty(self.topographic_model_part):
-                self.duplicate_model_part = True
-
-                # Creating the variables list if the topographic model part has to be duplicated
-                self.nodal_variables = GenerateVariableListFromInput(settings["nodal_variables_to_transfer"])
-                self.nonhistorical_variables = GenerateVariableListFromInput(settings["nonhistorical_variables_to_transfer"])
-
-
-    def ExecuteInitialize(self):
-        """Generate the topographic model part if specified or it already exists."""
-        if self.topographic_model_part is not None:
-            if self.duplicate_model_part:
-                self._DuplicateModelPart()
-
-
-    def ExecuteBeforeSolutionLoop(self):
-        """Initialize the visualization operations."""
-
-        # Deform the mesh according to the input options
-        if not self.deform_free_surface:
-            self._FlattenMeshCoordinates(self.computing_model_part)
-            self._InitializeDisplacement(self.computing_model_part)
-
-        # Deform the topography and transfer the nodal variables
-        if self.topographic_model_part is not None:
-            if not self.deform_topography:
-                self._FlattenMeshCoordinates(self.topographic_model_part)
-                self._InitializeDisplacement(self.topographic_model_part)
-
-        self.ExecuteBeforeOutputStep()
-
-
-    def ExecuteBeforeOutputStep(self):
-        """Perform the visualization operations."""
-        # Set the results only over the wet domain as non-historical
-        self._StoreNonHistoricalVariablesGiDNoDataIfDry()
-
-        # Deform the mesh according to the input options
-        if self.deform_free_surface:
-            self._DeformMesh(self.computing_model_part, SW.FREE_SURFACE_ELEVATION)
-        else:
-            self._UpdateDisplacement(self.computing_model_part, SW.FREE_SURFACE_ELEVATION)
-
-        # Deform the topography and transfer the nodal variables
-        if self.topographic_model_part is not None:
-            if self.duplicate_model_part:
-                self._TransferVariables()
-
-            if self.deform_topography:
-                self._DeformMesh(self.topographic_model_part, SW.TOPOGRAPHY)
-            else:
-                self._UpdateDisplacement(self.topographic_model_part, SW.TOPOGRAPHY)
-
-
-    def ExecuteAfterOutputStep(self):
-        """Restore the mesh deformation."""
-        if self.deform_free_surface:
-            self._RestoreMesh(self.computing_model_part)
-        
-        if self.topographic_model_part is not None:
-            if self.deform_topography:
-                self._RestoreMesh(self.topographic_model_part)
-
-
-    def _StoreNonHistoricalVariablesGiDNoDataIfDry(self):
-        SW.ShallowWaterUtilities().StoreNonHistoricalGiDNoDataIfDry(self.computing_model_part, SW.HEIGHT)
-        SW.ShallowWaterUtilities().StoreNonHistoricalGiDNoDataIfDry(self.computing_model_part, SW.FREE_SURFACE_ELEVATION)
-
-
-    @staticmethod
-    def _IsEmpty(model_part):
-        if model_part.NumberOfNodes() > 0:
-            return False
-        if model_part.NumberOfElements() > 0:
-            return False
-        if model_part.NumberOfConditions() > 0:
-            return False
-        return True
-
-
-    def _DuplicateModelPart(self):
-        KM.MergeVariableListsUtility().Merge(self.computing_model_part, self.topographic_model_part)
-        self.topographic_model_part.ProcessInfo = self.computing_model_part.ProcessInfo
-        element_num_nodes = len(self.computing_model_part.Elements.__iter__().__next__().GetNodes())
-        condition_num_nodes = len(self.computing_model_part.Conditions.__iter__().__next__().GetNodes())
-        reference_element = "Element2D{}N".format(element_num_nodes)
-        reference_condition = "LineCondition2D{}N".format(condition_num_nodes)
-        KM.DuplicateMeshModeler(self.computing_model_part).GenerateMesh(
-            self.topographic_model_part, reference_element, reference_condition)
-        KM.CopyPropertiesModeler(self.computing_model_part, self.topographic_model_part).SetupModelPart()
-        SW.ShallowWaterUtilities().OffsetIds(self.topographic_model_part.Nodes)
-        SW.ShallowWaterUtilities().OffsetIds(self.topographic_model_part.Elements)
-        SW.ShallowWaterUtilities().OffsetIds(self.topographic_model_part.Conditions)
-        SW.ShallowWaterUtilities().OffsetIds(self.topographic_model_part.Properties)
-
-
-    def _TransferVariables(self):
-        for variable in self.nodal_variables:
-            KM.VariableUtils().CopyModelPartNodalVar(
-                variable,
-                self.computing_model_part,
-                self.topographic_model_part,
-                0)
-        for variable in self.nonhistorical_variables:
-            KM.VariableUtils().CopyModelPartFlaggedNodalNonHistoricalVarToNonHistoricalVar(
-                variable, variable,
-                self.computing_model_part,
-                self.topographic_model_part,
-                KM.Flags(), False)
-
-
-    def _FlattenMeshCoordinates(self, model_part):
-        SW.ShallowWaterUtilities().SetMeshZCoordinateToZero(model_part)
-        SW.ShallowWaterUtilities().SetMeshZ0CoordinateToZero(model_part)
-        SW.ShallowWaterUtilities().OffsetMeshZCoordinate(model_part, self.mean_water_level)
-
-
-    def _DeformMesh(self, model_part, variable):
-        SW.ShallowWaterUtilities().SetMeshZCoordinate(model_part, variable)
-        SW.ShallowWaterUtilities().OffsetMeshZCoordinate(model_part, self.mean_water_level)
-
-
-    def _RestoreMesh(self, model_part):
-        SW.ShallowWaterUtilities().SetMeshZCoordinateToZero(model_part)
-
-
-    @staticmethod
-    def _InitializeDisplacement(model_part):
-        KM.VariableUtils().SetNonHistoricalVariableToZero(KM.DISPLACEMENT, model_part.Nodes)
-
-
-    def _UpdateDisplacement(self, model_part, variable):
-        if self.nodal_historical_displacement:
-            KM.VariableUtils().CopyModelPartNodalVar(variable, KM.DISPLACEMENT_Z,
-                                                     model_part, model_part, 0)
-        else:
-            KM.VariableUtils().CopyModelPartNodalVarToNonHistoricalVar(variable, KM.DISPLACEMENT_Z,
-                                                                       model_part, model_part, 0)
-
-
-    def _GetDeformMeshFlag(self, mesh_deformation_mode):
-        try:
-            value = self._mesh_deformation_modes[mesh_deformation_mode.GetString()]
-        except KeyError:
-            msg = "VisualizationMeshProcess. Unknown deformation mode '{}'. The possible options are: \n".format(mesh_deformation_mode.GetString())
-            for key in self._mesh_deformation_modes.keys():
-                msg += " - {}\n".format(key)
-            raise Exception(msg)
-        return value
+# Importing Kratos library
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+# Importing useful utilities
+from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return VisualizationMeshProcess(model, settings["Parameters"])
+
+class VisualizationMeshProcess(KM.Process):
+    """ VisualizationMeshProcess.
+
+    This process provides several tools for post-processing.
+    - Generation of an auxiliary model part for the topography visualization as a separate file.
+    - Setting the TOPOGRAPHY and FREE_SURFACE_ELEVATION into DISPLACEMENT_Z or Z-coordinate in order to view the mesh deformation.
+    - Saving the HEIGHT and FREE_SURFACE_ELEVATION as non-historical only on wet nodes. Dry nodes are set with the no-data value of GiD.
+    """
+
+    @staticmethod
+    def GetDefaultParameters():
+        return KM.Parameters("""
+            {
+                "model_part_name"                : "model_part_name",
+                "topographic_model_part_name"    : "",
+                "free_surface_deformation_mode"  : "nodal_displacement",
+                "topography_deformation_mode"    : "z_coordinate",
+                "nodal_historical_displacement"  : false,
+                "mean_water_level"               : 0.0,
+                "nodal_variables_to_transfer"    : [],
+                "nonhistorical_variables_to_transfer" : []
+            }
+            """)
+
+    _mesh_deformation_modes = {
+        "z_coordinate"       : True,
+        "nodal_displacement" : False
+    }
+
+    def __init__(self, model, settings):
+        """Constructor with Model and Parameters."""
+
+        KM.Process.__init__(self)
+        self.model = model
+        settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
+
+        self.computing_model_part = self.model[settings["model_part_name"].GetString()]
+
+        # Get the deformation mode options
+        self.deform_free_surface = self._GetDeformMeshFlag(settings["free_surface_deformation_mode"])
+        self.deform_topography = self._GetDeformMeshFlag(settings["topography_deformation_mode"])
+        self.nodal_historical_displacement = settings["nodal_historical_displacement"].GetBool()
+        self.mean_water_level = settings["mean_water_level"].GetDouble()
+
+        # Creating the topographic model part if specified
+        self.topographic_model_part = None
+        self.duplicate_model_part = False
+        topographic_model_part_name = settings["topographic_model_part_name"].GetString()
+        if topographic_model_part_name:
+            self.topographic_model_part = self.model.CreateModelPart(topographic_model_part_name)
+            if self._IsEmpty(self.topographic_model_part):
+                self.duplicate_model_part = True
+
+                # Creating the variables list if the topographic model part has to be duplicated
+                self.nodal_variables = GenerateVariableListFromInput(settings["nodal_variables_to_transfer"])
+                self.nonhistorical_variables = GenerateVariableListFromInput(settings["nonhistorical_variables_to_transfer"])
+
+
+    def ExecuteInitialize(self):
+        """Generate the topographic model part if specified or it already exists."""
+        if self.topographic_model_part is not None:
+            if self.duplicate_model_part:
+                self._DuplicateModelPart()
+
+
+    def ExecuteBeforeSolutionLoop(self):
+        """Initialize the visualization operations."""
+
+        # Deform the mesh according to the input options
+        if not self.deform_free_surface:
+            self._FlattenMeshCoordinates(self.computing_model_part)
+            self._InitializeDisplacement(self.computing_model_part)
+
+        # Deform the topography and transfer the nodal variables
+        if self.topographic_model_part is not None:
+            if not self.deform_topography:
+                self._FlattenMeshCoordinates(self.topographic_model_part)
+                self._InitializeDisplacement(self.topographic_model_part)
+
+        self.ExecuteBeforeOutputStep()
+
+
+    def ExecuteBeforeOutputStep(self):
+        """Perform the visualization operations."""
+        # Set the results only over the wet domain as non-historical
+        self._StoreNonHistoricalVariablesGiDNoDataIfDry()
+
+        # Deform the mesh according to the input options
+        if self.deform_free_surface:
+            self._DeformMesh(self.computing_model_part, SW.FREE_SURFACE_ELEVATION)
+        else:
+            self._UpdateDisplacement(self.computing_model_part, SW.FREE_SURFACE_ELEVATION)
+
+        # Deform the topography and transfer the nodal variables
+        if self.topographic_model_part is not None:
+            if self.duplicate_model_part:
+                self._TransferVariables()
+
+            if self.deform_topography:
+                self._DeformMesh(self.topographic_model_part, SW.TOPOGRAPHY)
+            else:
+                self._UpdateDisplacement(self.topographic_model_part, SW.TOPOGRAPHY)
+
+
+    def ExecuteAfterOutputStep(self):
+        """Restore the mesh deformation."""
+        if self.deform_free_surface:
+            self._RestoreMesh(self.computing_model_part)
+        
+        if self.topographic_model_part is not None:
+            if self.deform_topography:
+                self._RestoreMesh(self.topographic_model_part)
+
+
+    def _StoreNonHistoricalVariablesGiDNoDataIfDry(self):
+        SW.ShallowWaterUtilities().StoreNonHistoricalGiDNoDataIfDry(self.computing_model_part, SW.HEIGHT)
+        SW.ShallowWaterUtilities().StoreNonHistoricalGiDNoDataIfDry(self.computing_model_part, SW.FREE_SURFACE_ELEVATION)
+
+
+    @staticmethod
+    def _IsEmpty(model_part):
+        if model_part.NumberOfNodes() > 0:
+            return False
+        if model_part.NumberOfElements() > 0:
+            return False
+        if model_part.NumberOfConditions() > 0:
+            return False
+        return True
+
+
+    def _DuplicateModelPart(self):
+        KM.MergeVariableListsUtility().Merge(self.computing_model_part, self.topographic_model_part)
+        self.topographic_model_part.ProcessInfo = self.computing_model_part.ProcessInfo
+        element_num_nodes = len(self.computing_model_part.Elements.__iter__().__next__().GetNodes())
+        condition_num_nodes = len(self.computing_model_part.Conditions.__iter__().__next__().GetNodes())
+        reference_element = "Element2D{}N".format(element_num_nodes)
+        reference_condition = "LineCondition2D{}N".format(condition_num_nodes)
+        KM.DuplicateMeshModeler(self.computing_model_part).GenerateMesh(
+            self.topographic_model_part, reference_element, reference_condition)
+        KM.CopyPropertiesModeler(self.computing_model_part, self.topographic_model_part).SetupModelPart()
+        SW.ShallowWaterUtilities().OffsetIds(self.topographic_model_part.Nodes)
+        SW.ShallowWaterUtilities().OffsetIds(self.topographic_model_part.Elements)
+        SW.ShallowWaterUtilities().OffsetIds(self.topographic_model_part.Conditions)
+        SW.ShallowWaterUtilities().OffsetIds(self.topographic_model_part.Properties)
+
+
+    def _TransferVariables(self):
+        for variable in self.nodal_variables:
+            KM.VariableUtils().CopyModelPartNodalVar(
+                variable,
+                self.computing_model_part,
+                self.topographic_model_part,
+                0)
+        for variable in self.nonhistorical_variables:
+            KM.VariableUtils().CopyModelPartFlaggedNodalNonHistoricalVarToNonHistoricalVar(
+                variable, variable,
+                self.computing_model_part,
+                self.topographic_model_part,
+                KM.Flags(), False)
+
+
+    def _FlattenMeshCoordinates(self, model_part):
+        SW.ShallowWaterUtilities().SetMeshZCoordinateToZero(model_part)
+        SW.ShallowWaterUtilities().SetMeshZ0CoordinateToZero(model_part)
+        SW.ShallowWaterUtilities().OffsetMeshZCoordinate(model_part, self.mean_water_level)
+
+
+    def _DeformMesh(self, model_part, variable):
+        SW.ShallowWaterUtilities().SetMeshZCoordinate(model_part, variable)
+        SW.ShallowWaterUtilities().OffsetMeshZCoordinate(model_part, self.mean_water_level)
+
+
+    def _RestoreMesh(self, model_part):
+        SW.ShallowWaterUtilities().SetMeshZCoordinateToZero(model_part)
+
+
+    @staticmethod
+    def _InitializeDisplacement(model_part):
+        KM.VariableUtils().SetNonHistoricalVariableToZero(KM.DISPLACEMENT, model_part.Nodes)
+
+
+    def _UpdateDisplacement(self, model_part, variable):
+        if self.nodal_historical_displacement:
+            KM.VariableUtils().CopyModelPartNodalVar(variable, KM.DISPLACEMENT_Z,
+                                                     model_part, model_part, 0)
+        else:
+            KM.VariableUtils().CopyModelPartNodalVarToNonHistoricalVar(variable, KM.DISPLACEMENT_Z,
+                                                                       model_part, model_part, 0)
+
+
+    def _GetDeformMeshFlag(self, mesh_deformation_mode):
+        try:
+            value = self._mesh_deformation_modes[mesh_deformation_mode.GetString()]
+        except KeyError:
+            msg = "VisualizationMeshProcess. Unknown deformation mode '{}'. The possible options are: \n".format(mesh_deformation_mode.GetString())
+            for key in self._mesh_deformation_modes.keys():
+                msg += " - {}\n".format(key)
+            raise Exception(msg)
+        return value
```

## KratosMultiphysics/ShallowWaterApplication/testing/empty_output_process.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-# Importing the KratosMultiphysics library
-import KratosMultiphysics as KM
-
-def Factory(settings, Model):
-    return EmptyOutputProcess(Model, settings["Parameters"])
-
-class EmptyOutputProcess(KM.OutputProcess):
-    def __init__(self, model, parameters):
-        ''' EmptyOutputProcess constructor.
-
-        This is a temporal file and it must be deleted once there is an output_process base class in the core.
-        The main reason of existing is the need to test VisualizationMeshProcess with JsonOutputProcess and FromJsonCheckResultProcess.
-        '''
-        KM.OutputProcess.__init__(self)
-
-    def PrintOutput(self):
-        pass
+# Importing the KratosMultiphysics library
+import KratosMultiphysics as KM
+
+def Factory(settings, Model):
+    return EmptyOutputProcess(Model, settings["Parameters"])
+
+class EmptyOutputProcess(KM.OutputProcess):
+    def __init__(self, model, parameters):
+        ''' EmptyOutputProcess constructor.
+
+        This is a temporal file and it must be deleted once there is an output_process base class in the core.
+        The main reason of existing is the need to test VisualizationMeshProcess with JsonOutputProcess and FromJsonCheckResultProcess.
+        '''
+        KM.OutputProcess.__init__(self)
+
+    def PrintOutput(self):
+        pass
```

## KratosMultiphysics/ShallowWaterApplication/testing/empty_solver_for_testing.py

 * *Ordering differences only*

```diff
@@ -1,78 +1,78 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KM
-from KratosMultiphysics.python_solver import PythonSolver
-
-# Import applications
-import KratosMultiphysics.ShallowWaterApplication as SW
-
-def CreateSolver(model, custom_settings):
-    return EmptySolverForTesting(model, custom_settings)
-
-class EmptySolverForTesting(PythonSolver):
-    def __init__(self, model, settings):
-        """A solver with the minimal methods to run an analysis."""
-        super().__init__(model, settings)
-        self.model_part = self.model.CreateModelPart(self.settings["model_part_name"].GetString())
-        self.model_part.ProcessInfo.SetValue(KM.DOMAIN_SIZE, self.settings["domain_size"].GetInt())
-        self.model_part.ProcessInfo.SetValue(KM.GRAVITY_Z, self.settings["gravity"].GetDouble())
-        self.EstimateDeltaTimeUtility = SW.EstimateTimeStepUtility(self.GetComputingModelPart(), self.settings["time_stepping"])
-
-    def ImportModelPart(self):
-        self._ImportModelPart(self.model_part,self.settings["model_import_settings"])
-
-    def AddVariables(self):
-        self.model_part.AddNodalSolutionStepVariable(SW.HEIGHT)
-        self.model_part.AddNodalSolutionStepVariable(SW.FREE_SURFACE_ELEVATION)
-        self.model_part.AddNodalSolutionStepVariable(KM.MOMENTUM)
-        self.model_part.AddNodalSolutionStepVariable(KM.VELOCITY)
-        self.model_part.AddNodalSolutionStepVariable(SW.TOPOGRAPHY)
-        self.model_part.AddNodalSolutionStepVariable(SW.BATHYMETRY)
-        self.model_part.AddNodalSolutionStepVariable(SW.MANNING)
-
-    def AddDofs(self):
-        formulation_variables = self.settings["formulation_variables"].GetString()
-        if formulation_variables == "conservative":
-            KM.VariableUtils().AddDof(KM.MOMENTUM_X, self.model_part)
-            KM.VariableUtils().AddDof(KM.MOMENTUM_Y, self.model_part)
-            KM.VariableUtils().AddDof(SW.HEIGHT, self.model_part)
-        elif formulation_variables == "primitive":
-            KM.VariableUtils().AddDof(KM.VELOCITY_X, self.model_part)
-            KM.VariableUtils().AddDof(KM.VELOCITY_Y, self.model_part)
-            KM.VariableUtils().AddDof(SW.HEIGHT, self.model_part)
-        elif formulation_variables == "boussinesq":
-            KM.VariableUtils().AddDof(KM.VELOCITY_X, self.model_part)
-            KM.VariableUtils().AddDof(KM.VELOCITY_Y, self.model_part)
-            KM.VariableUtils().AddDof(SW.HEIGHT, self.model_part)
-
-    def GetMinimumBufferSize(self):
-        return 2
-
-    def GetComputingModelPart(self):
-        return self.model_part
-
-    def AdvanceInTime(self, current_time):
-        new_time = current_time + self.EstimateDeltaTimeUtility.Execute()
-        self.model_part.CloneTimeStep(new_time)
-        self.model_part.ProcessInfo[KM.STEP] += 1
-        return new_time
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        default_settings = KM.Parameters("""
-        {
-            "solver_type"              : "empty_solver_for_testing",
-            "model_part_name"          : "model_part",
-            "domain_size"              : 2,
-            "gravity"                  : 9.81,
-            "formulation_variables"    : "conservative",
-            "model_import_settings"    : {
-                "input_type"               : "use_input_model_part"
-            },
-            "time_stepping"            : {
-                "automatic_time_step"      : false,
-                "time_step"                : 0.01
-            }
-        }
-        """)
-        default_settings.AddMissingParameters(super().GetDefaultParameters())
-        return default_settings
+# Importing the Kratos Library
+import KratosMultiphysics as KM
+from KratosMultiphysics.python_solver import PythonSolver
+
+# Import applications
+import KratosMultiphysics.ShallowWaterApplication as SW
+
+def CreateSolver(model, custom_settings):
+    return EmptySolverForTesting(model, custom_settings)
+
+class EmptySolverForTesting(PythonSolver):
+    def __init__(self, model, settings):
+        """A solver with the minimal methods to run an analysis."""
+        super().__init__(model, settings)
+        self.model_part = self.model.CreateModelPart(self.settings["model_part_name"].GetString())
+        self.model_part.ProcessInfo.SetValue(KM.DOMAIN_SIZE, self.settings["domain_size"].GetInt())
+        self.model_part.ProcessInfo.SetValue(KM.GRAVITY_Z, self.settings["gravity"].GetDouble())
+        self.EstimateDeltaTimeUtility = SW.EstimateTimeStepUtility(self.GetComputingModelPart(), self.settings["time_stepping"])
+
+    def ImportModelPart(self):
+        self._ImportModelPart(self.model_part,self.settings["model_import_settings"])
+
+    def AddVariables(self):
+        self.model_part.AddNodalSolutionStepVariable(SW.HEIGHT)
+        self.model_part.AddNodalSolutionStepVariable(SW.FREE_SURFACE_ELEVATION)
+        self.model_part.AddNodalSolutionStepVariable(KM.MOMENTUM)
+        self.model_part.AddNodalSolutionStepVariable(KM.VELOCITY)
+        self.model_part.AddNodalSolutionStepVariable(SW.TOPOGRAPHY)
+        self.model_part.AddNodalSolutionStepVariable(SW.BATHYMETRY)
+        self.model_part.AddNodalSolutionStepVariable(SW.MANNING)
+
+    def AddDofs(self):
+        formulation_variables = self.settings["formulation_variables"].GetString()
+        if formulation_variables == "conservative":
+            KM.VariableUtils().AddDof(KM.MOMENTUM_X, self.model_part)
+            KM.VariableUtils().AddDof(KM.MOMENTUM_Y, self.model_part)
+            KM.VariableUtils().AddDof(SW.HEIGHT, self.model_part)
+        elif formulation_variables == "primitive":
+            KM.VariableUtils().AddDof(KM.VELOCITY_X, self.model_part)
+            KM.VariableUtils().AddDof(KM.VELOCITY_Y, self.model_part)
+            KM.VariableUtils().AddDof(SW.HEIGHT, self.model_part)
+        elif formulation_variables == "boussinesq":
+            KM.VariableUtils().AddDof(KM.VELOCITY_X, self.model_part)
+            KM.VariableUtils().AddDof(KM.VELOCITY_Y, self.model_part)
+            KM.VariableUtils().AddDof(SW.HEIGHT, self.model_part)
+
+    def GetMinimumBufferSize(self):
+        return 2
+
+    def GetComputingModelPart(self):
+        return self.model_part
+
+    def AdvanceInTime(self, current_time):
+        new_time = current_time + self.EstimateDeltaTimeUtility.Execute()
+        self.model_part.CloneTimeStep(new_time)
+        self.model_part.ProcessInfo[KM.STEP] += 1
+        return new_time
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        default_settings = KM.Parameters("""
+        {
+            "solver_type"              : "empty_solver_for_testing",
+            "model_part_name"          : "model_part",
+            "domain_size"              : 2,
+            "gravity"                  : 9.81,
+            "formulation_variables"    : "conservative",
+            "model_import_settings"    : {
+                "input_type"               : "use_input_model_part"
+            },
+            "time_stepping"            : {
+                "automatic_time_step"      : false,
+                "time_step"                : 0.01
+            }
+        }
+        """)
+        default_settings.AddMissingParameters(super().GetDefaultParameters())
+        return default_settings
```

## KratosMultiphysics/ShallowWaterApplication/utilities/benchmarking_utilities.py

 * *Ordering differences only*

```diff
@@ -1,21 +1,21 @@
-
-def GetProcessParameters(list_of_processes, name):
-    for processes in list_of_processes.values():
-        for process in processes:
-            if process['python_module'].GetString() == name:
-                return process['Parameters']
-
-def GetModelerParameters(list_of_modelers, name):
-    for modeler in list_of_modelers:
-        if modeler['modeler_name'].GetString() == name:
-            return modeler['Parameters']
-
-def KeepOnlyThisProcess(list_of_processes, module):
-    for list_name, proc_list in list_of_processes.items():
-        for proc in proc_list:
-            if proc['python_module'].GetString() == module:
-                keep_proc = proc.Clone()
-                keep_list = list_name
-        list_of_processes.RemoveValue(list_name)
-    list_of_processes.AddEmptyArray(keep_list)
-    list_of_processes[keep_list].Append(keep_proc)
+
+def GetProcessParameters(list_of_processes, name):
+    for processes in list_of_processes.values():
+        for process in processes:
+            if process['python_module'].GetString() == name:
+                return process['Parameters']
+
+def GetModelerParameters(list_of_modelers, name):
+    for modeler in list_of_modelers:
+        if modeler['modeler_name'].GetString() == name:
+            return modeler['Parameters']
+
+def KeepOnlyThisProcess(list_of_processes, module):
+    for list_name, proc_list in list_of_processes.items():
+        for proc in proc_list:
+            if proc['python_module'].GetString() == module:
+                keep_proc = proc.Clone()
+                keep_list = list_name
+        list_of_processes.RemoveValue(list_name)
+    list_of_processes.AddEmptyArray(keep_list)
+    list_of_processes[keep_list].Append(keep_proc)
```

## KratosMultiphysics/ShallowWaterApplication/utilities/solitary_wave_utilities.py

 * *Ordering differences only*

```diff
@@ -1,124 +1,124 @@
-from numpy import roots, cosh, errstate
-from math import pi, sqrt, tanh
-
-@errstate(over='ignore')
-def sech(x):
-    return 1/cosh(x)
-
-class SolitaryWaveSolution:
-    """Base class for analytical solutions of a solitary wave."""
-
-    def __init__(self, depth, gravity=9.81, *, amplitude):
-        self.depth = depth
-        self.gravity = gravity
-        self.amplitude = amplitude
-        self.amplitude1 = amplitude
-        self.amplitude2 = 0
-
-    def eta(self, x, t):
-        phase = self.wavenumber * (self.phase_speed * t - x)
-        return self.amplitude1 * sech(phase)**2 + self.amplitude2 * sech(phase)**4
-
-    def u(self, x, t):
-        eta = self.eta(x, t)
-        return self.phase_speed * eta / (self.depth + eta)
-
-    @property
-    def wavenumber(self):
-        raise Exception("SolitaryWaveSolution. The wavenumber is not defined in the base class.")
-
-    @property
-    def phase_speed(self):
-        return sqrt(self.gravity * (self.amplitude + self.depth))
-
-    @property
-    def frequency(self):
-        return self.wavenumber * self.phase_speed
-
-    @property
-    def wavelength(self):
-        return 2 * pi / self.wavenumber
-
-    @property
-    def period(self):
-        return 2 * pi / self.frequency
-
-
-class GoringSolution(SolitaryWaveSolution):
-    """Goring analytical solution.
-
-    K. Guizien and E. Barthelemy, Accuracy of solitary wave generation by a piston wave maker.
-    Journal of Hydraulic Research, February 2010
-    """
-
-    @property
-    def wavenumber(self):
-        return sqrt(3 / 4 * self.amplitude / self.depth**3)
-
-
-class RayleighSolution(SolitaryWaveSolution):
-    """Goring analytical solution.
-
-    K. Guizien and E. Barthelemy, Accuracy of solitary wave generation by a piston wave maker.
-    Journal of Hydraulic Research, February 2010
-    """
-
-    @property
-    def wavenumber(self):
-        return sqrt(3 * self.amplitude / 4 / self.depth**2 / (self.depth + self.amplitude))
-
-
-class BoussinesqSolution(SolitaryWaveSolution):
-    """Analytical solution for a solitary wave with the modified Boussinesq equations.
-
-    G. Wei and J. T. Kirby, Time-dependent numerical Code for extended Boussinesq equations.
-    Journal of Waterway, Port, Coastal and Ocean Engineering, September 1995
-
-    O. Nwogu, Alternative form of Boussinesq for nearshore wave propagation.
-    Journal of Waterway, Port, Coastal and Ocean Engineering, 1993
-    """
-
-    def __init__(self, depth, gravity=9.81, *, amplitude):
-        super().__init__(depth, gravity, amplitude=amplitude)
-        self.beta = -0.531
-        self.alpha = 0.5 * self.beta**2 + self.beta
-        self.delta = self.amplitude / self.depth
-
-        coefficients = [
-            2*self.alpha,                                     # C^6
-            -3*self.alpha - 1 / 3 - 2*self.alpha*self.delta,  # C^4
-            2*self.delta*(self.alpha + 1 / 3),                # C^2
-            self.alpha + 1 / 3]                               # 1
-        c_roots = roots(coefficients)
-        self.c_dimless = sqrt(c_roots[0])
-
-        gh = self.gravity * self.depth
-        c2 = gh * self.c_dimless**2
-        gha3 = gh * (self.alpha + 1 / 3)
-        self.amplitude1 = (c2 - gh) / 3 / (gha3 - self.alpha * c2) * self.depth
-        self.amplitude2 = -(c2 - gh)**2 / 2 / gh / c2 * (gha3 + 2 * self.alpha * c2) / (gha3 - self.alpha * c2) * self.depth
-
-    @property
-    def phase_speed(self):
-        return sqrt(self.gravity * self.depth) * self.c_dimless
-
-    @property
-    def wavenumber(self):
-        gh = self.gravity * self.depth
-        c2 = self.phase_speed**2
-        gha3 = gh * (self.alpha + 1 / 3)
-        return sqrt((c2 - gh) / 4 / (gha3 - self.alpha * c2)) / self.depth
-
-    def u(self, x, t):
-        gh = self.gravity * self.depth
-        c2 = self.phase_speed**2
-        horizontal_velocity = (c2 - gh) / self.phase_speed
-        phase = self.wavenumber * (self.phase_speed * t - x)
-        return horizontal_velocity * sech(phase)**2
-
-    def a(self, x, t):
-        gh = self.gravity * self.depth
-        c2 = self.phase_speed**2
-        horizontal_velocity = (c2 - gh) / self.phase_speed
-        phase = self.wavenumber * (self.phase_speed * t - x)
-        return -2 * self.frequency * horizontal_velocity * tanh(phase) * sech(phase)**2
+from numpy import roots, cosh, errstate
+from math import pi, sqrt, tanh
+
+@errstate(over='ignore')
+def sech(x):
+    return 1/cosh(x)
+
+class SolitaryWaveSolution:
+    """Base class for analytical solutions of a solitary wave."""
+
+    def __init__(self, depth, gravity=9.81, *, amplitude):
+        self.depth = depth
+        self.gravity = gravity
+        self.amplitude = amplitude
+        self.amplitude1 = amplitude
+        self.amplitude2 = 0
+
+    def eta(self, x, t):
+        phase = self.wavenumber * (self.phase_speed * t - x)
+        return self.amplitude1 * sech(phase)**2 + self.amplitude2 * sech(phase)**4
+
+    def u(self, x, t):
+        eta = self.eta(x, t)
+        return self.phase_speed * eta / (self.depth + eta)
+
+    @property
+    def wavenumber(self):
+        raise Exception("SolitaryWaveSolution. The wavenumber is not defined in the base class.")
+
+    @property
+    def phase_speed(self):
+        return sqrt(self.gravity * (self.amplitude + self.depth))
+
+    @property
+    def frequency(self):
+        return self.wavenumber * self.phase_speed
+
+    @property
+    def wavelength(self):
+        return 2 * pi / self.wavenumber
+
+    @property
+    def period(self):
+        return 2 * pi / self.frequency
+
+
+class GoringSolution(SolitaryWaveSolution):
+    """Goring analytical solution.
+
+    K. Guizien and E. Barthelemy, Accuracy of solitary wave generation by a piston wave maker.
+    Journal of Hydraulic Research, February 2010
+    """
+
+    @property
+    def wavenumber(self):
+        return sqrt(3 / 4 * self.amplitude / self.depth**3)
+
+
+class RayleighSolution(SolitaryWaveSolution):
+    """Goring analytical solution.
+
+    K. Guizien and E. Barthelemy, Accuracy of solitary wave generation by a piston wave maker.
+    Journal of Hydraulic Research, February 2010
+    """
+
+    @property
+    def wavenumber(self):
+        return sqrt(3 * self.amplitude / 4 / self.depth**2 / (self.depth + self.amplitude))
+
+
+class BoussinesqSolution(SolitaryWaveSolution):
+    """Analytical solution for a solitary wave with the modified Boussinesq equations.
+
+    G. Wei and J. T. Kirby, Time-dependent numerical Code for extended Boussinesq equations.
+    Journal of Waterway, Port, Coastal and Ocean Engineering, September 1995
+
+    O. Nwogu, Alternative form of Boussinesq for nearshore wave propagation.
+    Journal of Waterway, Port, Coastal and Ocean Engineering, 1993
+    """
+
+    def __init__(self, depth, gravity=9.81, *, amplitude):
+        super().__init__(depth, gravity, amplitude=amplitude)
+        self.beta = -0.531
+        self.alpha = 0.5 * self.beta**2 + self.beta
+        self.delta = self.amplitude / self.depth
+
+        coefficients = [
+            2*self.alpha,                                     # C^6
+            -3*self.alpha - 1 / 3 - 2*self.alpha*self.delta,  # C^4
+            2*self.delta*(self.alpha + 1 / 3),                # C^2
+            self.alpha + 1 / 3]                               # 1
+        c_roots = roots(coefficients)
+        self.c_dimless = sqrt(c_roots[0])
+
+        gh = self.gravity * self.depth
+        c2 = gh * self.c_dimless**2
+        gha3 = gh * (self.alpha + 1 / 3)
+        self.amplitude1 = (c2 - gh) / 3 / (gha3 - self.alpha * c2) * self.depth
+        self.amplitude2 = -(c2 - gh)**2 / 2 / gh / c2 * (gha3 + 2 * self.alpha * c2) / (gha3 - self.alpha * c2) * self.depth
+
+    @property
+    def phase_speed(self):
+        return sqrt(self.gravity * self.depth) * self.c_dimless
+
+    @property
+    def wavenumber(self):
+        gh = self.gravity * self.depth
+        c2 = self.phase_speed**2
+        gha3 = gh * (self.alpha + 1 / 3)
+        return sqrt((c2 - gh) / 4 / (gha3 - self.alpha * c2)) / self.depth
+
+    def u(self, x, t):
+        gh = self.gravity * self.depth
+        c2 = self.phase_speed**2
+        horizontal_velocity = (c2 - gh) / self.phase_speed
+        phase = self.wavenumber * (self.phase_speed * t - x)
+        return horizontal_velocity * sech(phase)**2
+
+    def a(self, x, t):
+        gh = self.gravity * self.depth
+        c2 = self.phase_speed**2
+        horizontal_velocity = (c2 - gh) / self.phase_speed
+        phase = self.wavenumber * (self.phase_speed * t - x)
+        return -2 * self.frequency * horizontal_velocity * tanh(phase) * sech(phase)**2
```

## KratosMultiphysics/ShallowWaterApplication/utilities/wave_factory.py

 * *Ordering differences only*

```diff
@@ -1,65 +1,65 @@
-import KratosMultiphysics as KM
-import KratosMultiphysics.ShallowWaterApplication as SW
-import KratosMultiphysics.ShallowWaterApplication.utilities.wave_theory_utilities as wave_theory
-import KratosMultiphysics.ShallowWaterApplication.utilities.solitary_wave_utilities as solitary_wave
-
-
-def WaveTheoryFactory(model_part, settings):
-    default_settings = KM.Parameters("""{
-        "wave_theory"               : "boussinesq",
-        "period"                    : 0.0,
-        "wavelength"                : 0.0,
-        "amplitude"                 : 0.0,
-        "depth"                     : 0.0,
-        "get_depth_from_model_part" : true,
-        "x_shift"                   : 0.0,
-        "t_shift"                   : 0.0
-    }""")
-    settings.ValidateAndAssignDefaults(default_settings)
-
-    wave_modules = {
-        "boussinesq"      : wave_theory.BoussinesqTheory,
-        "linear_theory"   : wave_theory.LinearTheory,
-        "shallow_theory"  : wave_theory.ShallowTheory,
-    }
-    wave_module = wave_modules[settings["wave_theory"].GetString()]
-    gravity = model_part.ProcessInfo[KM.GRAVITY_Z]
-    depth = _GetDepth(settings, model_part)
-    period = settings["period"].GetDouble()
-    wavelength = settings["wavelength"].GetDouble()
-    amplitude = settings["amplitude"].GetDouble()
-
-    return wave_module(depth, gravity, period=period, wavelength=wavelength, amplitude=amplitude)
-
-
-def SolitaryWaveFactory(model_part, settings):
-    default_settings = KM.Parameters("""{
-        "wave_theory"               : "boussinesq",
-        "amplitude"                 : 0.0,
-        "depth"                     : 0.0,
-        "get_depth_from_model_part" : true,
-        "x_shift"                   : 0.0,
-        "t_shift"                   : 0.0
-    }""")
-    settings.ValidateAndAssignDefaults(default_settings)
-
-    wave_modules = {
-        "goring"      : solitary_wave.GoringSolution,
-        "rayleigh"    : solitary_wave.RayleighSolution,
-        "boussinesq"  : solitary_wave.BoussinesqSolution,
-    }
-    wave_module = wave_modules[settings["wave_theory"].GetString()]
-    gravity = model_part.ProcessInfo[KM.GRAVITY_Z]
-    depth = _GetDepth(settings, model_part)
-    amplitude = settings["amplitude"].GetDouble()
-
-    return wave_module(depth, gravity, amplitude=amplitude)
-
-
-def _GetDepth(settings, model_part):
-    if settings["get_depth_from_model_part"].GetBool():
-        sum_depths = -KM.VariableUtils().SumHistoricalNodeScalarVariable(SW.TOPOGRAPHY, model_part, 0)
-        mean_depth = sum_depths / model_part.NumberOfNodes()
-        return mean_depth
-    else:
-        return settings["depth"].GetDouble()
+import KratosMultiphysics as KM
+import KratosMultiphysics.ShallowWaterApplication as SW
+import KratosMultiphysics.ShallowWaterApplication.utilities.wave_theory_utilities as wave_theory
+import KratosMultiphysics.ShallowWaterApplication.utilities.solitary_wave_utilities as solitary_wave
+
+
+def WaveTheoryFactory(model_part, settings):
+    default_settings = KM.Parameters("""{
+        "wave_theory"               : "boussinesq",
+        "period"                    : 0.0,
+        "wavelength"                : 0.0,
+        "amplitude"                 : 0.0,
+        "depth"                     : 0.0,
+        "get_depth_from_model_part" : true,
+        "x_shift"                   : 0.0,
+        "t_shift"                   : 0.0
+    }""")
+    settings.ValidateAndAssignDefaults(default_settings)
+
+    wave_modules = {
+        "boussinesq"      : wave_theory.BoussinesqTheory,
+        "linear_theory"   : wave_theory.LinearTheory,
+        "shallow_theory"  : wave_theory.ShallowTheory,
+    }
+    wave_module = wave_modules[settings["wave_theory"].GetString()]
+    gravity = model_part.ProcessInfo[KM.GRAVITY_Z]
+    depth = _GetDepth(settings, model_part)
+    period = settings["period"].GetDouble()
+    wavelength = settings["wavelength"].GetDouble()
+    amplitude = settings["amplitude"].GetDouble()
+
+    return wave_module(depth, gravity, period=period, wavelength=wavelength, amplitude=amplitude)
+
+
+def SolitaryWaveFactory(model_part, settings):
+    default_settings = KM.Parameters("""{
+        "wave_theory"               : "boussinesq",
+        "amplitude"                 : 0.0,
+        "depth"                     : 0.0,
+        "get_depth_from_model_part" : true,
+        "x_shift"                   : 0.0,
+        "t_shift"                   : 0.0
+    }""")
+    settings.ValidateAndAssignDefaults(default_settings)
+
+    wave_modules = {
+        "goring"      : solitary_wave.GoringSolution,
+        "rayleigh"    : solitary_wave.RayleighSolution,
+        "boussinesq"  : solitary_wave.BoussinesqSolution,
+    }
+    wave_module = wave_modules[settings["wave_theory"].GetString()]
+    gravity = model_part.ProcessInfo[KM.GRAVITY_Z]
+    depth = _GetDepth(settings, model_part)
+    amplitude = settings["amplitude"].GetDouble()
+
+    return wave_module(depth, gravity, amplitude=amplitude)
+
+
+def _GetDepth(settings, model_part):
+    if settings["get_depth_from_model_part"].GetBool():
+        sum_depths = -KM.VariableUtils().SumHistoricalNodeScalarVariable(SW.TOPOGRAPHY, model_part, 0)
+        mean_depth = sum_depths / model_part.NumberOfNodes()
+        return mean_depth
+    else:
+        return settings["depth"].GetDouble()
```

## KratosMultiphysics/ShallowWaterApplication/utilities/wave_theory_utilities.py

 * *Ordering differences only*

```diff
@@ -1,136 +1,136 @@
-from math import pi, sqrt, tanh
-from scipy.optimize import root
-
-
-class WaveTheory:
-    '''Base class for waves calculations.'''
-
-    def __init__(self, depth, gravity=9.81, *, period=0, wavelength=0, amplitude=0):
-        self.gravity = gravity
-        self.depth = depth
-        if self.depth <= 0:
-            raise Exception('WaveTheory. The water depth must be greather than 0.')
-        if self.gravity <= 0:
-            raise Exception('WaveTheory. The gravity must be greather than 0.')
-        if wavelength > 0 and period > 0:
-            raise Exception('WaveTheory. Specify only the wavelength or the period.')
-        if period > 0:
-            self.SetPeriod(period)
-        if wavelength > 0:
-            self.SetWavelength(wavelength)
-        if amplitude > 0:
-            self.SetAmplitude(amplitude)
-
-    def SetPeriod(self, period):
-        self.period = period
-        self.wavelength = self._CalculateWavelength(period)
-
-    def SetWavelength(self, wavelength):
-        self.wavelength = wavelength
-        self.period = self._CalculatePeriod(wavelength)
-
-    def SetAmplitude(self, amplitude):
-        self.amplitude = amplitude
-
-    @property
-    def horizontal_velocity(self):
-        return self._HorizontalVelocity(self.amplitude, self.frequency, self.wavenumber)
-
-    @property
-    def phase_speed(self):
-        return self._PhaseSpeed(self.wavenumber)
-
-    @property
-    def wavenumber(self):
-        return 2 * pi / self.wavelength
-
-    @property
-    def frequency(self):
-        return 2 * pi / self.period
-
-    def _DispersionRelation(self, wavenumber):
-        raise Exception('WaveTheory base class: it is not possible to calculate the disperison relation.')
-
-    def _HorizontalVelocity(self, amplitude, frequency, wavenumber):
-        raise Exception('WaveTheory base class: it is not possible to calculate the horizontal velocity.')
-
-    def _PhaseSpeed(self, wavenumber):
-        raise Exception('WaveTheory base class: it is not possible to calculate the phase speed.')
-
-    def _CalculateFrequency(self, wavenumber):
-        return sqrt(self._DispersionRelation(wavenumber))
-
-    def _CalculatePeriod(self, wavelength):
-        wavenumber = 2 * pi / wavelength
-        frequency = self._CalculateFrequency(wavenumber)
-        return 2 * pi / frequency
-
-    def _CalculateWavenumber(self, frequency):
-        k0 = frequency / sqrt(self.gravity * self.depth)
-        func = lambda k: self._CalculateFrequency(k) - frequency
-        result = root(func, k0)
-        if len(result.x) == 1:
-            return result.x[0]
-        else:
-            return result.x
-
-    def _CalculateWavelength(self, period):
-        frequency = 2*pi / period
-        wavenumber = self._CalculateWavenumber(frequency)
-        return 2 * pi / wavenumber
-
-
-class BoussinesqTheory(WaveTheory):
-    '''Boussinesq theory for dispersive waves.'''
-
-    beta = -0.531
-    alpha = 0.5 * beta**2 + beta
-
-    def _DispersionRelation(self, wavenumber):
-        g = self.gravity
-        kh = wavenumber * self.depth
-        return g * kh * wavenumber * (1 -(self.alpha + 1/3) * kh**2) / (1 -self.alpha * kh**2)
-
-    def _HorizontalVelocity(self, amplitude, frequency, wavenumber):
-        kh = wavenumber * self.depth
-        return frequency * amplitude / kh / (1 -(self.alpha + 1/3) * kh**2)
-
-    def _PhaseSpeed(self, wavenumber):
-        kh = wavenumber * self.depth
-        gh = self.gravity * self.depth
-        return sqrt(max(0, gh * (1 -(self.alpha + 1/3) * kh**2) / (1 -self.alpha * kh**2)))
-
-
-class LinearTheory(WaveTheory):
-    '''Linear theory for intermediate water.'''
-
-    def _DispersionRelation(self, wavenumber):
-        g = self.gravity
-        kh = wavenumber * self.depth
-        return g * wavenumber * tanh(kh)
-
-    def _HorizontalVelocity(self, amplitude, frequency, wavenumber):
-        kh = wavenumber * self.depth
-        return frequency * amplitude / kh # Note: 1/h * int{cosh(k*(z+h)) dz}_{-h}^{0} = sinh(kh) / kh
-
-    def _PhaseSpeed(self, wavenumber):
-        kh = wavenumber * self.depth
-        gh = self.gravity * self.depth
-        return sqrt(gh * tanh(kh) / kh)
-
-
-class ShallowTheory(WaveTheory):
-    '''Linear theory for shallow water.'''
-
-    def _DispersionRelation(self, wavenumber):
-        g = self.gravity
-        kh = wavenumber * self.depth
-        return g * wavenumber * kh
-
-    def _HorizontalVelocity(self, amplitude, frequency, wavenumber):
-        kh = wavenumber * self.depth
-        return frequency * amplitude / kh
-
-    def _PhaseSpeed(self, wavenumber):
-        gh = self.gravity * self.depth
-        return sqrt(gh)
+from math import pi, sqrt, tanh
+from scipy.optimize import root
+
+
+class WaveTheory:
+    '''Base class for waves calculations.'''
+
+    def __init__(self, depth, gravity=9.81, *, period=0, wavelength=0, amplitude=0):
+        self.gravity = gravity
+        self.depth = depth
+        if self.depth <= 0:
+            raise Exception('WaveTheory. The water depth must be greather than 0.')
+        if self.gravity <= 0:
+            raise Exception('WaveTheory. The gravity must be greather than 0.')
+        if wavelength > 0 and period > 0:
+            raise Exception('WaveTheory. Specify only the wavelength or the period.')
+        if period > 0:
+            self.SetPeriod(period)
+        if wavelength > 0:
+            self.SetWavelength(wavelength)
+        if amplitude > 0:
+            self.SetAmplitude(amplitude)
+
+    def SetPeriod(self, period):
+        self.period = period
+        self.wavelength = self._CalculateWavelength(period)
+
+    def SetWavelength(self, wavelength):
+        self.wavelength = wavelength
+        self.period = self._CalculatePeriod(wavelength)
+
+    def SetAmplitude(self, amplitude):
+        self.amplitude = amplitude
+
+    @property
+    def horizontal_velocity(self):
+        return self._HorizontalVelocity(self.amplitude, self.frequency, self.wavenumber)
+
+    @property
+    def phase_speed(self):
+        return self._PhaseSpeed(self.wavenumber)
+
+    @property
+    def wavenumber(self):
+        return 2 * pi / self.wavelength
+
+    @property
+    def frequency(self):
+        return 2 * pi / self.period
+
+    def _DispersionRelation(self, wavenumber):
+        raise Exception('WaveTheory base class: it is not possible to calculate the disperison relation.')
+
+    def _HorizontalVelocity(self, amplitude, frequency, wavenumber):
+        raise Exception('WaveTheory base class: it is not possible to calculate the horizontal velocity.')
+
+    def _PhaseSpeed(self, wavenumber):
+        raise Exception('WaveTheory base class: it is not possible to calculate the phase speed.')
+
+    def _CalculateFrequency(self, wavenumber):
+        return sqrt(self._DispersionRelation(wavenumber))
+
+    def _CalculatePeriod(self, wavelength):
+        wavenumber = 2 * pi / wavelength
+        frequency = self._CalculateFrequency(wavenumber)
+        return 2 * pi / frequency
+
+    def _CalculateWavenumber(self, frequency):
+        k0 = frequency / sqrt(self.gravity * self.depth)
+        func = lambda k: self._CalculateFrequency(k) - frequency
+        result = root(func, k0)
+        if len(result.x) == 1:
+            return result.x[0]
+        else:
+            return result.x
+
+    def _CalculateWavelength(self, period):
+        frequency = 2*pi / period
+        wavenumber = self._CalculateWavenumber(frequency)
+        return 2 * pi / wavenumber
+
+
+class BoussinesqTheory(WaveTheory):
+    '''Boussinesq theory for dispersive waves.'''
+
+    beta = -0.531
+    alpha = 0.5 * beta**2 + beta
+
+    def _DispersionRelation(self, wavenumber):
+        g = self.gravity
+        kh = wavenumber * self.depth
+        return g * kh * wavenumber * (1 -(self.alpha + 1/3) * kh**2) / (1 -self.alpha * kh**2)
+
+    def _HorizontalVelocity(self, amplitude, frequency, wavenumber):
+        kh = wavenumber * self.depth
+        return frequency * amplitude / kh / (1 -(self.alpha + 1/3) * kh**2)
+
+    def _PhaseSpeed(self, wavenumber):
+        kh = wavenumber * self.depth
+        gh = self.gravity * self.depth
+        return sqrt(max(0, gh * (1 -(self.alpha + 1/3) * kh**2) / (1 -self.alpha * kh**2)))
+
+
+class LinearTheory(WaveTheory):
+    '''Linear theory for intermediate water.'''
+
+    def _DispersionRelation(self, wavenumber):
+        g = self.gravity
+        kh = wavenumber * self.depth
+        return g * wavenumber * tanh(kh)
+
+    def _HorizontalVelocity(self, amplitude, frequency, wavenumber):
+        kh = wavenumber * self.depth
+        return frequency * amplitude / kh # Note: 1/h * int{cosh(k*(z+h)) dz}_{-h}^{0} = sinh(kh) / kh
+
+    def _PhaseSpeed(self, wavenumber):
+        kh = wavenumber * self.depth
+        gh = self.gravity * self.depth
+        return sqrt(gh * tanh(kh) / kh)
+
+
+class ShallowTheory(WaveTheory):
+    '''Linear theory for shallow water.'''
+
+    def _DispersionRelation(self, wavenumber):
+        g = self.gravity
+        kh = wavenumber * self.depth
+        return g * wavenumber * kh
+
+    def _HorizontalVelocity(self, amplitude, frequency, wavenumber):
+        kh = wavenumber * self.depth
+        return frequency * amplitude / kh
+
+    def _PhaseSpeed(self, wavenumber):
+        gh = self.gravity * self.depth
+        return sqrt(gh)
```

## Comparing `KratosShallowWaterApplication-9.4.5.dist-info/METADATA` & `KratosShallowWaterApplication-9.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-Metadata-Version: 2.1
-Name: KratosShallowWaterApplication
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
-# Shallow water application
-
-This is a research application that provides a set of tools for oceanographic and hydrographic simulations over shallow domains. The background of the stabilization method is explained in [^1].
-
-## Overview
-
-|               | BDF                | Crank-Nicolson     | Adams-Moulton      |
-|---------------|:------------------:|:------------------:|:------------------:|
-| Gravity waves | :heavy_check_mark: | :heavy_check_mark: |                    |
-| Saint-Venant  | :heavy_check_mark: |                    |                    |
-| Boussinesq    | :heavy_check_mark: |                    | :heavy_check_mark: |
-
-## Dependencies
-
-This application does not have other application dependencies at compile time. The following Python libraries may be required:
-
-- `scipy` is used by the wave generator and by the benchmarks
-- `numpy` is used to generate solitary waves and analytical solutions by the benchmarks
-
-If the coupling with the Navier-Stokes equations is required [^2], add the following applications to compilation:
-
-- [HDF5Application](../HDF5Application/README.md)
-- [MappingApplication](../MappingApplication/README.md)
-- [PfemFluidDynamicsApplication](../PfemFluidDynamicsApplication/README.md)
-
-## References
-
-[^1]: M. Masó, I. De-Pouplana, E. Oñate. A FIC-FEM stabilized formulation for the shallow water equations over partially dry domains. Computer Methods in Applied Mechanics and Engineering, 389C (2022) 114362 [10.1016/j.cma.2021.114362](https://doi.org/10.1016/j.cma.2021.114362)
-
-[^2]: M. Masó, A. Franci, I. de-Pouplana, A. Cornejo and E. Oñate, A Lagrangian-Eulerian procedure for the coupled solution of the Navier-Stokes and shallow water equations for landslide-generated waves. Advanced Modelling and Simulation in Engineering Sciences, (2022) [10.21203/rs.3.rs-1457837/v1](https://doi.org/10.21203/rs.3.rs-1457837/v1) (in press)
+Metadata-Version: 2.1
+Name: KratosShallowWaterApplication
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
+# Shallow water application
+
+This is a research application that provides a set of tools for oceanographic and hydrographic simulations over shallow domains. The background of the stabilization method is explained in [^1].
+
+## Overview
+
+|               | BDF                | Crank-Nicolson     | Adams-Moulton      |
+|---------------|:------------------:|:------------------:|:------------------:|
+| Gravity waves | :heavy_check_mark: | :heavy_check_mark: |                    |
+| Saint-Venant  | :heavy_check_mark: |                    |                    |
+| Boussinesq    | :heavy_check_mark: |                    | :heavy_check_mark: |
+
+## Dependencies
+
+This application does not have other application dependencies at compile time. The following Python libraries may be required:
+
+- `scipy` is used by the wave generator and by the benchmarks
+- `numpy` is used to generate solitary waves and analytical solutions by the benchmarks
+
+If the coupling with the Navier-Stokes equations is required [^2], add the following applications to compilation:
+
+- [HDF5Application](../HDF5Application/README.md)
+- [MappingApplication](../MappingApplication/README.md)
+- [PfemFluidDynamicsApplication](../PfemFluidDynamicsApplication/README.md)
+
+## References
+
+[^1]: M. Masó, I. De-Pouplana, E. Oñate. A FIC-FEM stabilized formulation for the shallow water equations over partially dry domains. Computer Methods in Applied Mechanics and Engineering, 389C (2022) 114362 [10.1016/j.cma.2021.114362](https://doi.org/10.1016/j.cma.2021.114362)
+
+[^2]: M. Masó, A. Franci, I. de-Pouplana, A. Cornejo and E. Oñate, A Lagrangian-Eulerian procedure for the coupled solution of the Navier-Stokes and shallow water equations for landslide-generated waves. Advanced Modelling and Simulation in Engineering Sciences, (2022) [10.21203/rs.3.rs-1457837/v1](https://doi.org/10.21203/rs.3.rs-1457837/v1) (in press)
```

## Comparing `KratosShallowWaterApplication-9.4.5.dist-info/RECORD` & `KratosShallowWaterApplication-9.5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-KratosMultiphysics/.libs/KratosShallowWaterApplication.pyd,sha256=WgUxak8SPFLxLYvrMrenHHbs1X6tNyDReBByF6eDJ7s,1090560
-KratosMultiphysics/.libs/KratosShallowWaterCore.dll,sha256=VPD9ST-LlLn1mKIr-q67zgxrrwEAgO5ZpYkyweYmztA,1899008
-KratosMultiphysics/.libs/KratosShallowWaterCore.lib,sha256=jdt0ogCjSoNSSLoCv38-ciDckzNf3P4LqdVWgMVkweQ,159124
-KratosMultiphysics/ShallowWaterApplication/__init__.py,sha256=nqOzO3ywy27_N0ULuF-mvhVPattkHBDf3XkVErr8NaQ,289
-KratosMultiphysics/ShallowWaterApplication/apply_absorbing_boundary_process.py,sha256=tnm-vWnEC4aLuqQaE8oGDbfqJYUlJfIGwFZGhegxU7c,2957
-KratosMultiphysics/ShallowWaterApplication/apply_slip_process.py,sha256=WviPDRt_XlXqIl5H0jJtSv9YMGHWm7jb8tF-V7rfbDk,1550
-KratosMultiphysics/ShallowWaterApplication/automatic_dirichlet_conditions_process.py,sha256=gHauJ0ZU-dj5qHLNi-zF0QSkYB0cHPIXlrjTN54Ld4g,6228
-KratosMultiphysics/ShallowWaterApplication/boussinesq_solver.py,sha256=cVkKLMtLr4xmn-lf_FNCik2NgzalxQ7egJNftvuSYhw,3886
-KratosMultiphysics/ShallowWaterApplication/derivatives_recovery_process.py,sha256=HLdog3ImPSuWT4ePE6UgHGyfti-tHz-sy8Obc-f6Gak,6332
-KratosMultiphysics/ShallowWaterApplication/lagrangian_shallow_water_solver.py,sha256=Nh9gD_4H8oKPDzBqbxhmU8u44B27XUgJ5NS4sAUaHn8,2948
-KratosMultiphysics/ShallowWaterApplication/primitive_solver.py,sha256=0nZb_HqAkFVy3wVjqkZ0zQcL_lVMj8KRwPtW0fgzfSo,654
-KratosMultiphysics/ShallowWaterApplication/set_initial_perturbation_process.py,sha256=AF0g-aZicwQvld6-GY2i8IeMMnXZU6UfgZh2t4ZrByg,3403
-KratosMultiphysics/ShallowWaterApplication/set_initial_water_level_process.py,sha256=31ebwb8Dl4ze02oWBYz8pm9w7kS-OG4-7L2n2njweUU,2408
-KratosMultiphysics/ShallowWaterApplication/set_topography_process.py,sha256=zalKtMnLDR4n7mRy35BbNq8KDy4RKdrIgPa9_4VbvyE,2341
-KratosMultiphysics/ShallowWaterApplication/shallow_water_analysis.py,sha256=M0nKmilZX-xBvtKSQPa5yEgd8xpu0ZTIQxwshyIoU5o,1427
-KratosMultiphysics/ShallowWaterApplication/shallow_water_base_solver.py,sha256=RCRI48GNYovHrcTNwKv_-j1Wzv42PSgUaZiz_1lRuS4,13691
-KratosMultiphysics/ShallowWaterApplication/stabilized_shallow_water_solver.py,sha256=jZos1ZrP7KTGeXFzUNz3AZZ0_1KGXRxrhg9Ao0muAPo,5736
-KratosMultiphysics/ShallowWaterApplication/wave_generator_process.py,sha256=CqnnMAzIIp0KqBMv8DUb5ygYiQZQFu3IaD5XPac7gbs,5314
-KratosMultiphysics/ShallowWaterApplication/wave_solver.py,sha256=sTPfa1xYbr5O_PekCkaqvsg3j7tzOpkTXZ-WrefK59M,3213
-KratosMultiphysics/ShallowWaterApplication/benchmarks/base_benchmark_process.py,sha256=ilK2Be8KFcc_dUhtDmM29Z0hLukcly9XXdlL-bjXeLw,5492
-KratosMultiphysics/ShallowWaterApplication/benchmarks/dam_break_benchmark.py,sha256=ow0NeJ6lWfWPNajYLQ1itAsYa2sY8Tg86ATqENiPdnE,4131
-KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_shock_benchmark.py,sha256=Cmm_Dd9PzzxsooSIz54v7LzH9h65sv16bDXNBwgdpI4,7983
-KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_transition_benchmark.py,sha256=RYWyFIT955ALhl6WIjzexv5mA7JmDm30SSiIEPz93Q0,3137
-KratosMultiphysics/ShallowWaterApplication/benchmarks/planar_surface_in_parabola_benchmark.py,sha256=YCRyj7vbYvwNpb3gd9TMPHNmW7xYkugNdTLEJcDOjr0,4158
-KratosMultiphysics/ShallowWaterApplication/benchmarks/solitary_wave_benchmark.py,sha256=WLHYKAI1NGJrBbPnc7ENouG7jAaFAujsaZMO1fdFDio,3685
-KratosMultiphysics/ShallowWaterApplication/coupling/compute_boundary_force_process.py,sha256=D0sCmNKGaquWz0tEEnMpK5ns0hgB3EtuSTlLzh74zGA,5350
-KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_input_process.py,sha256=qZaluUHXeCUoTjAOAhj-Jy3rg8HvGZmijudbbCvNaU4,11705
-KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_output_process.py,sha256=WIBCeZosaIkLNGNoe9CdA7rP8LPDATcqbYdjJeRWrO0,7112
-KratosMultiphysics/ShallowWaterApplication/coupling/read_from_sw_interface_process.py,sha256=jBYp8RXNG6hWSEE16Kccv1QaHjmd4udnQuUPQi7Xjfs,16456
-KratosMultiphysics/ShallowWaterApplication/coupling/write_from_sw_at_interface_process.py,sha256=rzOwiet9qOand3hJThRVtkOIGnAVpLaNdauEd-5zdyQ,4329
-KratosMultiphysics/ShallowWaterApplication/modelers/dam_break_modeler.py,sha256=VAgHD2Jgaj0804dIHHzuSwjAdoHPSPO6MqUC7kA-FJk,570
-KratosMultiphysics/ShallowWaterApplication/modelers/planar_surface_in_parabola_modeler.py,sha256=lgKpMxWLS4ZOTMeEASkfhksQtxfMpygADjGlf85mZIQ,647
-KratosMultiphysics/ShallowWaterApplication/postprocess/auxiliary_nodes_visualization_process.py,sha256=5FMAm8BsGryY6u0CUEcd1YbDLJIaHnlJMvTFBpjVVRg,4164
-KratosMultiphysics/ShallowWaterApplication/postprocess/compute_froude_process.py,sha256=VZEtaJQZHOGXOXvM8vE_VrQOJPI0k_wCXrUVnwKYuXk,1537
-KratosMultiphysics/ShallowWaterApplication/postprocess/convergence_output_process.py,sha256=wIdDPfY8MzAzZBpUJ4yZt8xYWuus8IULEThYjmmTqNY,6266
-KratosMultiphysics/ShallowWaterApplication/postprocess/generate_gid_list_file.py,sha256=PmUCPF2LkDbjFeKTN3vrGW_d5tB4bpoADMTX8BcLs50,1384
-KratosMultiphysics/ShallowWaterApplication/postprocess/line_envelope_output_process.py,sha256=Y1uAUiagABDOLZ8mID3i3kKfL47bk7sqdEjwHE1OFdA,2669
-KratosMultiphysics/ShallowWaterApplication/postprocess/line_graph_output_process.py,sha256=CgIaPbROqiObuYEj_ie6l5RVoSwsyvV1kB-jDtcA_e8,13777
-KratosMultiphysics/ShallowWaterApplication/postprocess/offset_ids_process.py,sha256=N1xc8bE4An4ODMAhEqCaTanAywHYtXQSMcctN-7Xok0,2658
-KratosMultiphysics/ShallowWaterApplication/postprocess/swap_coordinates_process.py,sha256=TubFe4hrTrPKqLLxG8D2t9PQPJldt73Esq-XU0rgw90,1919
-KratosMultiphysics/ShallowWaterApplication/postprocess/visualization_mesh_process.py,sha256=YLqjGouSABdhfZWx57Daxs7DtNZ03GP9fZT95Mu58L0,9747
-KratosMultiphysics/ShallowWaterApplication/testing/empty_output_process.py,sha256=Uov5tGGmNOzINCktOLiDXEDSQ71A7VJVw2iwm5tpNfA,657
-KratosMultiphysics/ShallowWaterApplication/testing/empty_solver_for_testing.py,sha256=Ilh-fqA8HABQyUuOiKvYh7LCMJgm9e6yh3IVWfQ_xkE,3663
-KratosMultiphysics/ShallowWaterApplication/utilities/benchmarking_utilities.py,sha256=RWi9yRlBsk8KrupRUkpeMfCrCn_Uxm541v6d5lt_AHM,876
-KratosMultiphysics/ShallowWaterApplication/utilities/solitary_wave_utilities.py,sha256=MSaN4X6AoACGrJ5NRB_-hbgw1S5fHm0vS8Su9FHT1cE,4364
-KratosMultiphysics/ShallowWaterApplication/utilities/wave_factory.py,sha256=EFzlj-6zPJATiiDu3tjGcOQmmo6CW3Di9WSTSZ8N7V8,2698
-KratosMultiphysics/ShallowWaterApplication/utilities/wave_theory_utilities.py,sha256=QKpLPLK6flhK1wOM2HJByq0b3yLChGPvtmurImKdTsI,4716
-KratosShallowWaterApplication-9.4.5.dist-info/METADATA,sha256=v85v_YFVasqakYqwkBS3Pz5a_u9oi2dUW3zxDzVoqCk,3308
-KratosShallowWaterApplication-9.4.5.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
-KratosShallowWaterApplication-9.4.5.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
-KratosShallowWaterApplication-9.4.5.dist-info/RECORD,,
+KratosShallowWaterApplication.libs/libKratosShallowWaterCore-ed139967.so,sha256=intBaPF3edOfTcqkU3gsmKHrewoGaJCvTLsxODct9Ds,7584961
+KratosShallowWaterApplication-9.5.dist-info/METADATA,sha256=oRezw3p9ND_tfRXopAImTSLv5q3Zk4zfWu7ibDfuIks,3244
+KratosShallowWaterApplication-9.5.dist-info/WHEEL,sha256=L0ABBnxO_xKRR_wTzM7WWWX8RRfdKRK-fZ5a3ZEhDqQ,148
+KratosShallowWaterApplication-9.5.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
+KratosShallowWaterApplication-9.5.dist-info/RECORD,,
+KratosMultiphysics/ShallowWaterApplication/stabilized_shallow_water_solver.py,sha256=J6LC8NFYK9Fwx9tMbfyqw4k7A1stUnUhpV2ivQeEhbE,5625
+KratosMultiphysics/ShallowWaterApplication/boussinesq_solver.py,sha256=uB3648uA5eAg3Dib-9U2G1cOc_XRWPxhjGReXiAh9h0,3817
+KratosMultiphysics/ShallowWaterApplication/apply_absorbing_boundary_process.py,sha256=4lsRYSfBQQEUm2Q-vC487ZD91MwHuG5rHJvWywXS3qc,2894
+KratosMultiphysics/ShallowWaterApplication/wave_solver.py,sha256=ORZ2pbPvD8Nlrm35qLlSpqnVzMNNILuTLhMUcSQbuNA,3145
+KratosMultiphysics/ShallowWaterApplication/shallow_water_base_solver.py,sha256=i325CinLdlh8mk1QdbLeyFKRFVsHGylSzzGVeJJ1Jh8,13397
+KratosMultiphysics/ShallowWaterApplication/automatic_dirichlet_conditions_process.py,sha256=bjqTg_eRozj3neqJ5mYEdGuuBatJBMHYMtvPYcbV4tk,6111
+KratosMultiphysics/ShallowWaterApplication/primitive_solver.py,sha256=HrIKYzzNgEVn8pHq8J5EM0wj7ZnifLjKL7wlWK4tFc4,636
+KratosMultiphysics/ShallowWaterApplication/wave_generator_process.py,sha256=Dk2J7zRrhlqj6b6TYA3VEyhFEXdHlZh7B3Drgw5BM-k,5195
+KratosMultiphysics/ShallowWaterApplication/lagrangian_shallow_water_solver.py,sha256=ESWbdF3jcOhDoiMoRGTxYXDUcBILIxixceNDiQNSY5s,2864
+KratosMultiphysics/ShallowWaterApplication/apply_slip_process.py,sha256=HUMemVpcSwCwnVCHV0h8Pex4ySPAMSehhImIAu00Yfg,1510
+KratosMultiphysics/ShallowWaterApplication/set_topography_process.py,sha256=HoYVhh6_gdAdmdHMuAPladzPdeK0jGs--qPrc2LEmEQ,2288
+KratosMultiphysics/ShallowWaterApplication/shallow_water_analysis.py,sha256=299GK0cAq6DmtGhHZ4btp5ui4XbhdtWTw-MrWBp33m4,1390
+KratosMultiphysics/ShallowWaterApplication/derivatives_recovery_process.py,sha256=UKhqHVjAi6j4je9ybRkLoGqyO0lGiNFzOUG2DcBR8zc,6190
+KratosMultiphysics/ShallowWaterApplication/__init__.py,sha256=YIgb0E1pt8ieJYu-gst26EfXAn29GIvwHMxtgyTg7s0,282
+KratosMultiphysics/ShallowWaterApplication/set_initial_perturbation_process.py,sha256=TK-ZcGaV3oC6WIUcYIshz7CueOHAXpTvXSfakOlFh4E,3339
+KratosMultiphysics/ShallowWaterApplication/set_initial_water_level_process.py,sha256=iTj1Lq5MZjpuQYb_xqwl16vrgdeh5sdGWUjB2E2gxso,2355
+KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_output_process.py,sha256=aFdtE2kV5ma5WOrJUa_0kQXjsjFQHUmApIXlgcwBeVU,6960
+KratosMultiphysics/ShallowWaterApplication/coupling/write_from_sw_at_interface_process.py,sha256=WU1qyXHEzGh6B_Du6PpCs-5M3YQmLaJVtrrHuT3nQyI,4253
+KratosMultiphysics/ShallowWaterApplication/coupling/compute_boundary_force_process.py,sha256=D0sCmNKGaquWz0tEEnMpK5ns0hgB3EtuSTlLzh74zGA,5350
+KratosMultiphysics/ShallowWaterApplication/coupling/read_from_sw_interface_process.py,sha256=8em5daGN_HDSdo64a1glDehpp9wcc_5FJo7nkxGVQi8,16112
+KratosMultiphysics/ShallowWaterApplication/coupling/depth_integration_input_process.py,sha256=qEQSYkrqeb-irnSN8fQtpqU0G9nIF5s4VV66M7M3YQ0,11460
+KratosMultiphysics/ShallowWaterApplication/utilities/solitary_wave_utilities.py,sha256=305sodZ8uqICYWy1KeeMFkzGNqr7KySfQnEzn1VwIyQ,4240
+KratosMultiphysics/ShallowWaterApplication/utilities/wave_factory.py,sha256=jjOoapxzqv3CdxDhcM8t5BPUR2pX-Hz-YhyvJrgtoFU,2633
+KratosMultiphysics/ShallowWaterApplication/utilities/wave_theory_utilities.py,sha256=FPA-Kc-JoZ5PB-XmfORL5Hvst0kXpZqKL7vkIrCIi0I,4580
+KratosMultiphysics/ShallowWaterApplication/utilities/benchmarking_utilities.py,sha256=8dLVnxstygX7wM04Dv0f4owOFKUmiCpPkY65tBPGxYA,855
+KratosMultiphysics/ShallowWaterApplication/postprocess/offset_ids_process.py,sha256=9PV1Z-yyjF8IRWyasdkrbBM4Bpio6tdTvuN0tOSdb88,2592
+KratosMultiphysics/ShallowWaterApplication/postprocess/generate_gid_list_file.py,sha256=h4psbty8uapPzXdk4Trrh9sDwMxepeVJOUtY9_9Wmbw,1346
+KratosMultiphysics/ShallowWaterApplication/postprocess/compute_froude_process.py,sha256=tfj0xx9OyXzhsZlYxgdDtqAOzCAPdQuUTQmFxMU6QR8,1501
+KratosMultiphysics/ShallowWaterApplication/postprocess/convergence_output_process.py,sha256=lvrupzK4zY7hYfGyMlKfGH4K8Pl27QCqPPF6mgIn81Y,6114
+KratosMultiphysics/ShallowWaterApplication/postprocess/visualization_mesh_process.py,sha256=8516vCJbs_i6Bwx46Dby4R_zJbnzIX6cZ5hr8eFQtBE,9536
+KratosMultiphysics/ShallowWaterApplication/postprocess/line_envelope_output_process.py,sha256=W_1D0NMCS5jyaK4YkIWiFqL45-B5Snf43NDKBGJH6EY,2608
+KratosMultiphysics/ShallowWaterApplication/postprocess/auxiliary_nodes_visualization_process.py,sha256=sVY2-q_6tpU4fNIwXp7anfr6xfBidsCYF8zUwApXXzE,4071
+KratosMultiphysics/ShallowWaterApplication/postprocess/swap_coordinates_process.py,sha256=7lLKTVmfV0fDd6zU-WbpeMfvZawgGdNBqZsUzOmjKLc,1864
+KratosMultiphysics/ShallowWaterApplication/postprocess/line_graph_output_process.py,sha256=FlFj38jFZic_4YVapxttdGyy_1oOkC_jLhlTjzZ5540,13473
+KratosMultiphysics/ShallowWaterApplication/testing/empty_output_process.py,sha256=b_KBBmPmpGICzzf1yZOqR5VwdZie_EQ7XZKdI6-TxiA,640
+KratosMultiphysics/ShallowWaterApplication/testing/empty_solver_for_testing.py,sha256=dA4BkoUC8YQfnkbTr5LeZKgg_X5AG-2RRtayfWOP5fY,3585
+KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_shock_benchmark.py,sha256=zV4JWhb_c7sRI6gaFy7ehQQe-xpdHkKwn_Mbmq7GibY,7773
+KratosMultiphysics/ShallowWaterApplication/benchmarks/base_benchmark_process.py,sha256=fReuYnSm7R5omCrt508foapUymh0H5A74mJEU76Ebtg,5373
+KratosMultiphysics/ShallowWaterApplication/benchmarks/mac_donald_transition_benchmark.py,sha256=WNQiQvgUJwUZ5eChiusogznlVKBjl3ukgOXoixZqPcw,3058
+KratosMultiphysics/ShallowWaterApplication/benchmarks/dam_break_benchmark.py,sha256=CgSfQMrv7JrMLef2C9Lt3HXDBqPUMgfqIn8o0DW3WgY,4003
+KratosMultiphysics/ShallowWaterApplication/benchmarks/solitary_wave_benchmark.py,sha256=WE6XY39vr4Q9akdRSU7gfPOYvCI5A89zmqaq6r5v_VI,3601
+KratosMultiphysics/ShallowWaterApplication/benchmarks/planar_surface_in_parabola_benchmark.py,sha256=4i8uj2oqlZwoLqjiroccB56R-KbaB3xiRfFmbjV9Xtg,4042
+KratosMultiphysics/ShallowWaterApplication/modelers/planar_surface_in_parabola_modeler.py,sha256=gezu-34L1ndf7XDWrBRf1LYyEEyEHcsERlgbGAjvPCs,630
+KratosMultiphysics/ShallowWaterApplication/modelers/dam_break_modeler.py,sha256=mSWEWzI4sczaFB81PGfh6PP-gGkRAT_I-oLxLhl6YeM,553
+KratosMultiphysics/.libs/libKratosShallowWaterCore.so,sha256=BDK8MdHLzrQno0zjuzRlChM2kadxLha5ZEgzR9rVqUU,7094081
+KratosMultiphysics/.libs/KratosShallowWaterApplication.cpython-38-x86_64-linux-gnu.so,sha256=Sx7nvhkLBAa8kEq_GZIFaej_3Nf53MXWnres4cO4hto,2877833
```

