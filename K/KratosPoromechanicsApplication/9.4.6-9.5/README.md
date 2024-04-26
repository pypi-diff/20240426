# Comparing `tmp/KratosPoromechanicsApplication-9.4.6-cp39-cp39-win_amd64.whl.zip` & `tmp/KratosPoromechanicsApplication-9.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,597 +1,899 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   1727583 (00000000001A5C5Fh)
-  Actual end-cent-dir record offset:       1727561 (00000000001A5C49h)
-  Expected end-cent-dir record offset:     1727561 (00000000001A5C49h)
+  Zip archive file size:                   6549713 (000000000063F0D1h)
+  Actual end-cent-dir record offset:       6549691 (000000000063F0BBh)
+  Expected end-cent-dir record offset:     6549691 (000000000063F0BBh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 20 entries.
-  The central directory is 2343 (0000000000000927h) bytes long,
+  central directory contains 24 entries.
+  The central directory is 3261 (0000000000000CBDh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 1725218 (00000000001A5322h).
+  is 6546430 (000000000063E3FEh).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosPoromechanicsApplication.pyd
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
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:40
-  32-bit CRC value (hex):                         455f45d1
-  compressed size:                                519143 bytes
-  uncompressed size:                              1818624 bytes
-  length of filename:                             59 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
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
 
-  KratosMultiphysics/.libs/KratosPoromechanicsCore.dll
+  KratosMultiphysics/PoromechanicsApplication/
 
-  offset of local header from start of archive:   519232
-                                                  (000000000007EC40h) bytes
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
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:40
-  32-bit CRC value (hex):                         315351ac
-  compressed size:                                1071237 bytes
-  uncompressed size:                              3814912 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             44 characters
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
 
-  KratosMultiphysics/.libs/KratosPoromechanicsCore.lib
+  KratosMultiphysics/PoromechanicsApplication/poromechanics_cleaning_utility.py
 
-  offset of local header from start of archive:   1590551
-                                                  (0000000000184517h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   179
+                                                  (00000000000000B3h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:40
-  32-bit CRC value (hex):                         1fbdc43a
-  compressed size:                                113011 bytes
-  uncompressed size:                              1697748 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         f96926e5
+  compressed size:                                171 bytes
+  uncompressed size:                              629 bytes
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
 
-  KratosMultiphysics/PoromechanicsApplication/__init__.py
+  KratosMultiphysics/PoromechanicsApplication/apply_scalar_constraint_table_process.py
 
-  offset of local header from start of archive:   1703644
-                                                  (000000000019FEDCh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   485
+                                                  (00000000000001E5h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         13d73fc0
-  compressed size:                                134 bytes
-  uncompressed size:                              292 bytes
-  length of filename:                             55 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         33df3e26
+  compressed size:                                671 bytes
+  uncompressed size:                              2780 bytes
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
 
 Central directory entry #5:
 ---------------------------
 
-  KratosMultiphysics/PoromechanicsApplication/apply_normal_load_table_process.py
+  KratosMultiphysics/PoromechanicsApplication/poromechanics_analysis.py
 
-  offset of local header from start of archive:   1703863
-                                                  (000000000019FFB7h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1298
+                                                  (0000000000000512h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         c6c72ac7
-  compressed size:                                797 bytes
-  uncompressed size:                              3440 bytes
-  length of filename:                             78 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         bef9e63a
+  compressed size:                                1431 bytes
+  uncompressed size:                              5514 bytes
+  length of filename:                             69 characters
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
 
-  KratosMultiphysics/PoromechanicsApplication/apply_scalar_constraint_table_process.py
+  KratosMultiphysics/PoromechanicsApplication/poromechanics_face_load_control_module_process.py
 
-  offset of local header from start of archive:   1704768
-                                                  (00000000001A0340h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   2856
+                                                  (0000000000000B28h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         33df3e26
-  compressed size:                                671 bytes
-  uncompressed size:                              2780 bytes
-  length of filename:                             84 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         d3a5dd27
+  compressed size:                                787 bytes
+  uncompressed size:                              3388 bytes
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
 
 Central directory entry #7:
 ---------------------------
 
-  KratosMultiphysics/PoromechanicsApplication/apply_vector_constraint_table_process.py
+  KratosMultiphysics/PoromechanicsApplication/check_and_prepare_model_process_poro.py
 
-  offset of local header from start of archive:   1705553
-                                                  (00000000001A0651h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3794
+                                                  (0000000000000ED2h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         6250e508
-  compressed size:                                739 bytes
-  uncompressed size:                              3703 bytes
-  length of filename:                             84 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         64f80c30
+  compressed size:                                879 bytes
+  uncompressed size:                              4480 bytes
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
 
 Central directory entry #8:
 ---------------------------
 
-  KratosMultiphysics/PoromechanicsApplication/check_and_prepare_model_process_poro.py
+  KratosMultiphysics/PoromechanicsApplication/poromechanics_fracture_propagation_utility.py
 
-  offset of local header from start of archive:   1706406
-                                                  (00000000001A09A6h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   4814
+                                                  (00000000000012CEh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         8615ccc8
-  compressed size:                                887 bytes
-  uncompressed size:                              4558 bytes
-  length of filename:                             83 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         cf22ed63
+  compressed size:                                2733 bytes
+  uncompressed size:                              16333 bytes
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
 
-  KratosMultiphysics/PoromechanicsApplication/periodic_interface_activation_process.py
+  KratosMultiphysics/PoromechanicsApplication/apply_vector_constraint_table_process.py
 
-  offset of local header from start of archive:   1707406
-                                                  (00000000001A0D8Eh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   7694
+                                                  (0000000000001E0Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         f574b11f
-  compressed size:                                515 bytes
-  uncompressed size:                              1520 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         6250e508
+  compressed size:                                739 bytes
+  uncompressed size:                              3703 bytes
   length of filename:                             84 characters
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
 
 Central directory entry #10:
 ---------------------------
 
-  KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pw_explicit_dynamic_solver.py
+  KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pl_solver.py
 
-  offset of local header from start of archive:   1708035
-                                                  (00000000001A1003h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   8575
+                                                  (000000000000217Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         0ea6a21b
-  compressed size:                                2535 bytes
-  uncompressed size:                              11791 bytes
-  length of filename:                             89 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         9ec47dc2
+  compressed size:                                5348 bytes
+  uncompressed size:                              30765 bytes
+  length of filename:                             72 characters
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
 
-  KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pw_solver.py
+  KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pl_explicit_dynamic_solver.py
 
-  offset of local header from start of archive:   1710689
-                                                  (00000000001A1A61h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   14053
+                                                  (00000000000036E5h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         8b99452c
-  compressed size:                                5391 bytes
-  uncompressed size:                              31444 bytes
-  length of filename:                             72 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         34b8256c
+  compressed size:                                2533 bytes
+  uncompressed size:                              11681 bytes
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
 
 Central directory entry #12:
 ---------------------------
 
-  KratosMultiphysics/PoromechanicsApplication/poromechanics_analysis.py
+  KratosMultiphysics/PoromechanicsApplication/apply_normal_load_table_process.py
 
-  offset of local header from start of archive:   1716182
-                                                  (00000000001A2FD6h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   16733
+                                                  (000000000000415Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         06a31c1a
-  compressed size:                                1443 bytes
-  uncompressed size:                              5631 bytes
-  length of filename:                             69 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         c6c72ac7
+  compressed size:                                797 bytes
+  uncompressed size:                              3440 bytes
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
 
 Central directory entry #13:
 ---------------------------
 
-  KratosMultiphysics/PoromechanicsApplication/poromechanics_cleaning_utility.py
+  KratosMultiphysics/PoromechanicsApplication/__init__.py
 
-  offset of local header from start of archive:   1717724
-                                                  (00000000001A35DCh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   17666
+                                                  (0000000000004502h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         d3aa7370
-  compressed size:                                175 bytes
-  uncompressed size:                              651 bytes
-  length of filename:                             77 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         80a7c9d0
+  compressed size:                                129 bytes
+  uncompressed size:                              285 bytes
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
 
 Central directory entry #14:
 ---------------------------
 
-  KratosMultiphysics/PoromechanicsApplication/poromechanics_face_load_control_module_process.py
+  KratosMultiphysics/PoromechanicsApplication/periodic_interface_activation_process.py
 
-  offset of local header from start of archive:   1718006
-                                                  (00000000001A36F6h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   17908
+                                                  (00000000000045F4h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         d3a5dd27
-  compressed size:                                787 bytes
-  uncompressed size:                              3388 bytes
-  length of filename:                             93 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         6427b0a7
+  compressed size:                                508 bytes
+  uncompressed size:                              1483 bytes
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
 
-  KratosMultiphysics/PoromechanicsApplication/poromechanics_fracture_propagation_utility.py
+  KratosMultiphysics/PoromechanicsApplication/poromechanics_initial_stress_utility.py
 
-  offset of local header from start of archive:   1718916
-                                                  (00000000001A3A84h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   18558
+                                                  (000000000000487Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         cf22ed63
-  compressed size:                                2733 bytes
-  uncompressed size:                              16333 bytes
-  length of filename:                             89 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         a5791941
+  compressed size:                                805 bytes
+  uncompressed size:                              2845 bytes
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
 
 Central directory entry #16:
 ---------------------------
 
-  KratosMultiphysics/PoromechanicsApplication/poromechanics_initial_stress_utility.py
+  KratosMultiphysics/.libs/
 
-  offset of local header from start of archive:   1721768
-                                                  (00000000001A45A8h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   19504
+                                                  (0000000000004C30h) bytes
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
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:44
-  32-bit CRC value (hex):                         77a0e0e6
-  compressed size:                                812 bytes
-  uncompressed size:                              2906 bytes
-  length of filename:                             83 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:19 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:19 UTC
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
 
 Central directory entry #17:
 ---------------------------
 
-  KratosPoromechanicsApplication-9.4.6.dist-info/METADATA
+  KratosMultiphysics/.libs/KratosPoromechanicsApplication.cpython-39-x86_64-linux-gnu.so
 
-  offset of local header from start of archive:   1722693
-                                                  (00000000001A4945h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   19587
+                                                  (0000000000004C83h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:40
-  32-bit CRC value (hex):                         b515d18c
-  compressed size:                                956 bytes
-  uncompressed size:                              2493 bytes
-  length of filename:                             55 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         80a2cf87
+  compressed size:                                1474300 bytes
+  uncompressed size:                              4593257 bytes
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
 
 Central directory entry #18:
 ---------------------------
 
-  KratosPoromechanicsApplication-9.4.6.dist-info/WHEEL
+  KratosPoromechanicsApplication-9.5.dist-info/
 
-  offset of local header from start of archive:   1723734
-                                                  (00000000001A4D56h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1494031
+                                                  (000000000016CC0Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:19 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:19 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             45 characters
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
+Central directory entry #19:
+---------------------------
+
+  KratosPoromechanicsApplication-9.5.dist-info/METADATA
+
+  offset of local header from start of archive:   1494134
+                                                  (000000000016CC76h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:40
-  32-bit CRC value (hex):                         86fb6b41
-  compressed size:                                96 bytes
-  uncompressed size:                              100 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         112d644e
+  compressed size:                                934 bytes
+  uncompressed size:                              2427 bytes
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
 
-Central directory entry #19:
+Central directory entry #20:
 ---------------------------
 
-  KratosPoromechanicsApplication-9.4.6.dist-info/top_level.txt
+  KratosPoromechanicsApplication-9.5.dist-info/WHEEL
 
-  offset of local header from start of archive:   1723912
-                                                  (00000000001A4E08h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1495179
+                                                  (000000000016D08Bh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:40
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         90d34e0d
+  compressed size:                                116 bytes
+  uncompressed size:                              148 bytes
+  length of filename:                             50 characters
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
+Central directory entry #21:
+---------------------------
+
+  KratosPoromechanicsApplication-9.5.dist-info/top_level.txt
+
+  offset of local header from start of archive:   1495403
+                                                  (000000000016D16Bh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
   32-bit CRC value (hex):                         f32d789f
-  compressed size:                                21 bytes
+  compressed size:                                19 bytes
   uncompressed size:                              19 bytes
-  length of filename:                             60 characters
-  length of extra field:                          0 bytes
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
 
-Central directory entry #20:
+Central directory entry #22:
 ---------------------------
 
-  KratosPoromechanicsApplication-9.4.6.dist-info/RECORD
+  KratosPoromechanicsApplication-9.5.dist-info/RECORD
 
-  offset of local header from start of archive:   1724023
-                                                  (00000000001A4E77h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1495538
+                                                  (000000000016D1F2h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:40
-  32-bit CRC value (hex):                         01f987f8
-  compressed size:                                1112 bytes
-  uncompressed size:                              2516 bytes
-  length of filename:                             53 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:19 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:19 UTC
+  32-bit CRC value (hex):                         e7280235
+  compressed size:                                1139 bytes
+  uncompressed size:                              2581 bytes
+  length of filename:                             51 characters
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
+Central directory entry #23:
+---------------------------
+
+  KratosPoromechanicsApplication.libs/
+
+  offset of local header from start of archive:   1496786
+                                                  (000000000016D6D2h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:20
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:19 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:19 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             36 characters
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
+Central directory entry #24:
+---------------------------
+
+  KratosPoromechanicsApplication.libs/libKratosPoromechanicsCore-2e59df2b.so
+
+  offset of local header from start of archive:   1496880
+                                                  (000000000016D730h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:10 UTC
+  32-bit CRC value (hex):                         095304fd
+  compressed size:                                5049418 bytes
+  uncompressed size:                              18688153 bytes
+  length of filename:                             74 characters
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
@@ -1,61 +1,73 @@
-Filename: KratosMultiphysics/.libs/KratosPoromechanicsApplication.pyd
+Filename: KratosMultiphysics/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosPoromechanicsCore.dll
+Filename: KratosMultiphysics/PoromechanicsApplication/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosPoromechanicsCore.lib
+Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_cleaning_utility.py
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/__init__.py
+Filename: KratosMultiphysics/PoromechanicsApplication/apply_scalar_constraint_table_process.py
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/apply_normal_load_table_process.py
+Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_analysis.py
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/apply_scalar_constraint_table_process.py
+Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_face_load_control_module_process.py
+Comment: 
+
+Filename: KratosMultiphysics/PoromechanicsApplication/check_and_prepare_model_process_poro.py
+Comment: 
+
+Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_fracture_propagation_utility.py
 Comment: 
 
 Filename: KratosMultiphysics/PoromechanicsApplication/apply_vector_constraint_table_process.py
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/check_and_prepare_model_process_poro.py
+Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pl_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/periodic_interface_activation_process.py
+Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pl_explicit_dynamic_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pw_explicit_dynamic_solver.py
+Filename: KratosMultiphysics/PoromechanicsApplication/apply_normal_load_table_process.py
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pw_solver.py
+Filename: KratosMultiphysics/PoromechanicsApplication/__init__.py
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_analysis.py
+Filename: KratosMultiphysics/PoromechanicsApplication/periodic_interface_activation_process.py
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_cleaning_utility.py
+Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_initial_stress_utility.py
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_face_load_control_module_process.py
+Filename: KratosMultiphysics/.libs/
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_fracture_propagation_utility.py
+Filename: KratosMultiphysics/.libs/KratosPoromechanicsApplication.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: KratosMultiphysics/PoromechanicsApplication/poromechanics_initial_stress_utility.py
+Filename: KratosPoromechanicsApplication-9.5.dist-info/
+Comment: 
+
+Filename: KratosPoromechanicsApplication-9.5.dist-info/METADATA
+Comment: 
+
+Filename: KratosPoromechanicsApplication-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosPoromechanicsApplication-9.4.6.dist-info/METADATA
+Filename: KratosPoromechanicsApplication-9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosPoromechanicsApplication-9.4.6.dist-info/WHEEL
+Filename: KratosPoromechanicsApplication-9.5.dist-info/RECORD
 Comment: 
 
-Filename: KratosPoromechanicsApplication-9.4.6.dist-info/top_level.txt
+Filename: KratosPoromechanicsApplication.libs/
 Comment: 
 
-Filename: KratosPoromechanicsApplication-9.4.6.dist-info/RECORD
+Filename: KratosPoromechanicsApplication.libs/libKratosPoromechanicsCore-2e59df2b.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## KratosMultiphysics/PoromechanicsApplication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,8 +1,8 @@
-
-# Application dependent names and paths
-from KratosMultiphysics import _ImportApplication
-from KratosPoromechanicsApplication import *
-application = KratosPoromechanicsApplication()
-application_name = "KratosPoromechanicsApplication"
-
+
+# Application dependent names and paths
+from KratosMultiphysics import _ImportApplication
+from KratosPoromechanicsApplication import *
+application = KratosPoromechanicsApplication()
+application_name = "KratosPoromechanicsApplication"
+
 _ImportApplication(application, application_name)
```

## KratosMultiphysics/PoromechanicsApplication/check_and_prepare_model_process_poro.py

 * *Ordering differences only*

```diff
@@ -1,78 +1,78 @@
-import KratosMultiphysics
-import KratosMultiphysics.PoromechanicsApplication
-
-def Factory(settings, Model):
-    if(type(settings) != KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return CheckAndPrepareModelProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class CheckAndPrepareModelProcess(KratosMultiphysics.Process):
-    def __init__(self, main_model_part, Parameters ):
-        KratosMultiphysics.Process.__init__(self)
-        self.main_model_part = main_model_part
-
-        self.computing_model_part_name  = Parameters["computing_model_part_name"].GetString()
-        self.problem_domain_sub_model_part_list = Parameters["problem_domain_sub_model_part_list"]
-        self.processes_sub_model_part_list = Parameters["processes_sub_model_part_list"]
-        self.body_domain_sub_model_part_list = Parameters["body_domain_sub_model_part_list"]
-        self.body_domain_sub_sub_model_part_list = Parameters["body_domain_sub_sub_model_part_list"]
-        self.loads_sub_model_part_list = Parameters["loads_sub_model_part_list"]
-        self.loads_sub_sub_model_part_list = Parameters["loads_sub_sub_model_part_list"]
-
-    def Execute(self):
-        # Construct the computing model part: a model part which contains the mesh to compute
-        self.main_model_part.CreateSubModelPart(self.computing_model_part_name)
-        computing_model_part = self.main_model_part.GetSubModelPart(self.computing_model_part_name)
-        computing_model_part.ProcessInfo = self.main_model_part.ProcessInfo
-        computing_model_part.Properties = self.main_model_part.Properties
-        computing_model_part.Set(KratosMultiphysics.ACTIVE)
-
-        domain_parts = []
-        for i in range(self.problem_domain_sub_model_part_list.size()):
-            domain_parts.append(self.main_model_part.GetSubModelPart(self.problem_domain_sub_model_part_list[i].GetString()))
-        # Adding Nodes to Computing Model Part
-        list_of_ids = set()
-        for part in domain_parts:
-            for node in part.Nodes:
-                list_of_ids.add(node.Id)
-        computing_model_part.AddNodes(list(list_of_ids))
-        # Adding Elements to Computing Model Part
-        list_of_ids = set()
-        for part in domain_parts:
-            for elem in part.Elements:
-                list_of_ids.add(elem.Id)
-        computing_model_part.AddElements(list(list_of_ids))
-        # Adding Conditions to Computing Model Part
-        domain_conditions = []
-        for i in range(self.processes_sub_model_part_list.size()):
-            domain_conditions.append(self.main_model_part.GetSubModelPart(self.processes_sub_model_part_list[i].GetString()))
-        list_of_ids = set()
-        for part in domain_conditions:
-            for cond in part.Conditions:
-                list_of_ids.add(cond.Id)
-        computing_model_part.AddConditions(list(list_of_ids))
-
-        # Adding Computing Sub Sub Model Parts
-        # Body - Joints
-        for i in range(self.body_domain_sub_model_part_list.size()):
-            body_sub_model_part = self.main_model_part.GetSubModelPart(self.body_domain_sub_model_part_list[i].GetString())
-            computing_model_part.CreateSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
-            body_sub_sub_model_part = computing_model_part.GetSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
-            list_of_ids = set()
-            for node in body_sub_model_part.Nodes:
-                list_of_ids.add(node.Id)
-            body_sub_sub_model_part.AddNodes(list(list_of_ids))
-            list_of_ids = set()
-            for elem in body_sub_model_part.Elements:
-                list_of_ids.add(elem.Id)
-            body_sub_sub_model_part.AddElements(list(list_of_ids))
-        # Arc-Length
-        for i in range(self.loads_sub_model_part_list.size()):
-            load_sub_model_part = self.main_model_part.GetSubModelPart(self.loads_sub_model_part_list[i].GetString())
-            computing_model_part.CreateSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
-            load_sub_sub_model_part = computing_model_part.GetSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
-            list_of_ids = set()
-            for node in load_sub_model_part.Nodes:
-                list_of_ids.add(node.Id)
-            load_sub_sub_model_part.AddNodes(list(list_of_ids))
+import KratosMultiphysics
+import KratosMultiphysics.PoromechanicsApplication
+
+def Factory(settings, Model):
+    if(type(settings) != KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return CheckAndPrepareModelProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class CheckAndPrepareModelProcess(KratosMultiphysics.Process):
+    def __init__(self, main_model_part, Parameters ):
+        KratosMultiphysics.Process.__init__(self)
+        self.main_model_part = main_model_part
+
+        self.computing_model_part_name  = Parameters["computing_model_part_name"].GetString()
+        self.problem_domain_sub_model_part_list = Parameters["problem_domain_sub_model_part_list"]
+        self.processes_sub_model_part_list = Parameters["processes_sub_model_part_list"]
+        self.body_domain_sub_model_part_list = Parameters["body_domain_sub_model_part_list"]
+        self.body_domain_sub_sub_model_part_list = Parameters["body_domain_sub_sub_model_part_list"]
+        self.loads_sub_model_part_list = Parameters["loads_sub_model_part_list"]
+        self.loads_sub_sub_model_part_list = Parameters["loads_sub_sub_model_part_list"]
+
+    def Execute(self):
+        # Construct the computing model part: a model part which contains the mesh to compute
+        self.main_model_part.CreateSubModelPart(self.computing_model_part_name)
+        computing_model_part = self.main_model_part.GetSubModelPart(self.computing_model_part_name)
+        computing_model_part.ProcessInfo = self.main_model_part.ProcessInfo
+        computing_model_part.Properties = self.main_model_part.Properties
+        computing_model_part.Set(KratosMultiphysics.ACTIVE)
+
+        domain_parts = []
+        for i in range(self.problem_domain_sub_model_part_list.size()):
+            domain_parts.append(self.main_model_part.GetSubModelPart(self.problem_domain_sub_model_part_list[i].GetString()))
+        # Adding Nodes to Computing Model Part
+        list_of_ids = set()
+        for part in domain_parts:
+            for node in part.Nodes:
+                list_of_ids.add(node.Id)
+        computing_model_part.AddNodes(list(list_of_ids))
+        # Adding Elements to Computing Model Part
+        list_of_ids = set()
+        for part in domain_parts:
+            for elem in part.Elements:
+                list_of_ids.add(elem.Id)
+        computing_model_part.AddElements(list(list_of_ids))
+        # Adding Conditions to Computing Model Part
+        domain_conditions = []
+        for i in range(self.processes_sub_model_part_list.size()):
+            domain_conditions.append(self.main_model_part.GetSubModelPart(self.processes_sub_model_part_list[i].GetString()))
+        list_of_ids = set()
+        for part in domain_conditions:
+            for cond in part.Conditions:
+                list_of_ids.add(cond.Id)
+        computing_model_part.AddConditions(list(list_of_ids))
+
+        # Adding Computing Sub Sub Model Parts
+        # Body - Joints
+        for i in range(self.body_domain_sub_model_part_list.size()):
+            body_sub_model_part = self.main_model_part.GetSubModelPart(self.body_domain_sub_model_part_list[i].GetString())
+            computing_model_part.CreateSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
+            body_sub_sub_model_part = computing_model_part.GetSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
+            list_of_ids = set()
+            for node in body_sub_model_part.Nodes:
+                list_of_ids.add(node.Id)
+            body_sub_sub_model_part.AddNodes(list(list_of_ids))
+            list_of_ids = set()
+            for elem in body_sub_model_part.Elements:
+                list_of_ids.add(elem.Id)
+            body_sub_sub_model_part.AddElements(list(list_of_ids))
+        # Arc-Length
+        for i in range(self.loads_sub_model_part_list.size()):
+            load_sub_model_part = self.main_model_part.GetSubModelPart(self.loads_sub_model_part_list[i].GetString())
+            computing_model_part.CreateSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
+            load_sub_sub_model_part = computing_model_part.GetSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
+            list_of_ids = set()
+            for node in load_sub_model_part.Nodes:
+                list_of_ids.add(node.Id)
+            load_sub_sub_model_part.AddNodes(list(list_of_ids))
```

## KratosMultiphysics/PoromechanicsApplication/periodic_interface_activation_process.py

 * *Ordering differences only*

```diff
@@ -1,37 +1,37 @@
-import KratosMultiphysics
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-
-def Factory(settings, Model):
-    if(type(settings) != KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return PeriodicInterfaceActivationProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-
-class PeriodicInterfaceActivationProcess(KratosMultiphysics.Process):
-    def __init__(self, Model, settings ):
-        KratosMultiphysics.Process.__init__(self)
-
-        self.model_part = Model[settings["model_part_name"].GetString()]
-
-        self.params = KratosMultiphysics.Parameters("{}")
-        self.params.AddValue("model_part_name",settings["model_part_name"])
-        self.params.AddValue("dimension",settings["dimension"])
-        self.params.AddValue("stress_limit",settings["stress_limit"])
-
-        self.process = KratosPoro.PeriodicInterfaceProcess(self.model_part, self.params)
-
-        if(settings["dimension"].GetInt() == 2):
-            self.FindNodalNeigh = KratosMultiphysics.FindNodalNeighboursProcess(self.model_part)
-        else:
-            self.FindNodalNeigh = KratosMultiphysics.FindNodalNeighboursProcess(self.model_part)
-
-    def ExecuteInitialize(self):
-
-        self.FindNodalNeigh.Execute()
-
-        self.process.ExecuteInitialize()
-
-    def ExecuteFinalizeSolutionStep(self):
-
-        self.process.ExecuteFinalizeSolutionStep()
+import KratosMultiphysics
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+
+def Factory(settings, Model):
+    if(type(settings) != KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return PeriodicInterfaceActivationProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+
+class PeriodicInterfaceActivationProcess(KratosMultiphysics.Process):
+    def __init__(self, Model, settings ):
+        KratosMultiphysics.Process.__init__(self)
+
+        self.model_part = Model[settings["model_part_name"].GetString()]
+
+        self.params = KratosMultiphysics.Parameters("{}")
+        self.params.AddValue("model_part_name",settings["model_part_name"])
+        self.params.AddValue("dimension",settings["dimension"])
+        self.params.AddValue("stress_limit",settings["stress_limit"])
+
+        self.process = KratosPoro.PeriodicInterfaceProcess(self.model_part, self.params)
+
+        if(settings["dimension"].GetInt() == 2):
+            self.FindNodalNeigh = KratosMultiphysics.FindNodalNeighboursProcess(self.model_part)
+        else:
+            self.FindNodalNeigh = KratosMultiphysics.FindNodalNeighboursProcess(self.model_part)
+
+    def ExecuteInitialize(self):
+
+        self.FindNodalNeigh.Execute()
+
+        self.process.ExecuteInitialize()
+
+    def ExecuteFinalizeSolutionStep(self):
+
+        self.process.ExecuteFinalizeSolutionStep()
```

## KratosMultiphysics/PoromechanicsApplication/poromechanics_analysis.py

 * *Ordering differences only*

```diff
@@ -1,117 +1,117 @@
-
-import time as timer
-import os
-
-import KratosMultiphysics as Kratos
-import KratosMultiphysics.LinearSolversApplication
-import KratosMultiphysics.FluidDynamicsApplication
-import KratosMultiphysics.StructuralMechanicsApplication
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-
-from KratosMultiphysics.analysis_stage import AnalysisStage
-
-from importlib import import_module
-
-class PoromechanicsAnalysis(AnalysisStage):
-    '''Main script for poromechanics simulations.'''
-
-    def __init__(self,model,parameters):
-        # Time monitoring
-        KratosMultiphysics.Logger.PrintInfo(self._GetSimulationName(),timer.ctime())
-        self.initial_time = timer.perf_counter()
-
-        ## Import parallel modules if needed
-        from KratosMultiphysics.PoromechanicsApplication import poromechanics_cleaning_utility
-        poromechanics_cleaning_utility.CleanPreviousFiles(os.getcwd()) # Clean previous post files
-        KratosMultiphysics.Logger.PrintInfo(self._GetSimulationName(),"OpenMP parallel configuration.")
-
-        # Initialize Fracture Propagation Utility if necessary
-        if parameters["problem_data"]["fracture_utility"].GetBool():
-            from KratosMultiphysics.PoromechanicsApplication.poromechanics_fracture_propagation_utility import FracturePropagationUtility
-            self.fracture_utility = FracturePropagationUtility(model,
-                                                                self._GetOrderOfProcessesInitialization())
-            parameters = self.fracture_utility.Initialize(parameters)
-
-        # Creating solver and model part and adding variables
-        super(PoromechanicsAnalysis,self).__init__(model,parameters)
-
-        self.initial_stress_mode = 'external' # Not from a Poromechanics solution
-        if parameters["problem_data"].Has("initial_stress_utility_settings"):
-            self.initial_stress_mode = parameters["problem_data"]["initial_stress_utility_settings"]["mode"].GetString()
-        if (self.initial_stress_mode == 'load' or self.initial_stress_mode == 'save'):
-            from KratosMultiphysics.PoromechanicsApplication.poromechanics_initial_stress_utility import InitialStressUtility
-            self.initial_stress_utility = InitialStressUtility(model,parameters)
-
-    def Initialize(self):
-        super(PoromechanicsAnalysis,self).Initialize()
-
-        if (self.initial_stress_mode == 'load'):
-            self.initial_stress_utility.Load()
-
-    def OutputSolutionStep(self):
-        super(PoromechanicsAnalysis,self).OutputSolutionStep()
-
-        # Check Fracture Propagation Utility
-        if self.project_parameters["problem_data"]["fracture_utility"].GetBool():
-            if self.fracture_utility.IsPropagationStep():
-                self._solver,self._list_of_processes,self._list_of_output_processes = self.fracture_utility.CheckPropagation(self._solver,
-                                                                                                                            self._list_of_processes,
-                                                                                                                            self._list_of_output_processes)
-
-    def Finalize(self):
-        super(PoromechanicsAnalysis,self).Finalize()
-
-        # Finalize Fracture Propagation Utility
-        if self.project_parameters["problem_data"]["fracture_utility"].GetBool():
-            self.fracture_utility.Finalize()
-
-        if (self.initial_stress_mode == 'save'):
-            self.initial_stress_utility.Save()
-
-        # Finalizing strategy
-        if self.parallel_type == "OpenMP":
-            self._GetSolver().Clear()
-
-        # Time control
-        KratosMultiphysics.Logger.PrintInfo(self._GetSimulationName(),"Analysis Completed. Elapsed Time = %.3f" % (timer.perf_counter() - self.initial_time)," seconds.")
-        KratosMultiphysics.Logger.PrintInfo(self._GetSimulationName(),timer.ctime())
-
-    def _CreateSolver(self):
-        python_module_name = "KratosMultiphysics.PoromechanicsApplication"
-        full_module_name = python_module_name + "." + self.project_parameters["solver_settings"]["solver_type"].GetString()
-        solver_module = import_module(full_module_name)
-        solver = solver_module.CreateSolver(self.model, self.project_parameters["solver_settings"])
-        return solver
-
-    def _GetOrderOfProcessesInitialization(self):
-        return ["constraints_process_list",
-                "loads_process_list",
-                "auxiliar_process_list"]
-
-    def _GetSimulationName(self):
-        return "Poromechanics Analysis"
-
-
-if __name__ == '__main__':
-    from sys import argv
-
-    if len(argv) > 2:
-        err_msg =  'Too many input arguments!\n'
-        err_msg += 'Use this script in the following way:\n'
-        err_msg += '- With default parameter file (assumed to be called "ProjectParameters.json"):\n'
-        err_msg += '    "python poromechanics_analysis.py"\n'
-        err_msg += '- With custom parameter file:\n'
-        err_msg += '    "python poromechanics_analysis.py <my-parameter-file>.json"\n'
-        raise Exception(err_msg)
-
-    if len(argv) == 2: # ProjectParameters is being passed from outside
-        parameter_file_name = argv[1]
-    else: # using default name
-        parameter_file_name = "ProjectParameters.json"
-
-    with open(parameter_file_name,'r') as parameter_file:
-        parameters = Kratos.Parameters(parameter_file.read())
-
-    model = Kratos.Model()
-    simulation = PoromechanicsAnalysis(model,parameters)
-    simulation.Run()
+
+import time as timer
+import os
+
+import KratosMultiphysics as Kratos
+import KratosMultiphysics.LinearSolversApplication
+import KratosMultiphysics.FluidDynamicsApplication
+import KratosMultiphysics.StructuralMechanicsApplication
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+
+from KratosMultiphysics.analysis_stage import AnalysisStage
+
+from importlib import import_module
+
+class PoromechanicsAnalysis(AnalysisStage):
+    '''Main script for poromechanics simulations.'''
+
+    def __init__(self,model,parameters):
+        # Time monitoring
+        KratosMultiphysics.Logger.PrintInfo(self._GetSimulationName(),timer.ctime())
+        self.initial_time = timer.perf_counter()
+
+        ## Import parallel modules if needed
+        from KratosMultiphysics.PoromechanicsApplication import poromechanics_cleaning_utility
+        poromechanics_cleaning_utility.CleanPreviousFiles(os.getcwd()) # Clean previous post files
+        KratosMultiphysics.Logger.PrintInfo(self._GetSimulationName(),"OpenMP parallel configuration.")
+
+        # Initialize Fracture Propagation Utility if necessary
+        if parameters["problem_data"]["fracture_utility"].GetBool():
+            from KratosMultiphysics.PoromechanicsApplication.poromechanics_fracture_propagation_utility import FracturePropagationUtility
+            self.fracture_utility = FracturePropagationUtility(model,
+                                                                self._GetOrderOfProcessesInitialization())
+            parameters = self.fracture_utility.Initialize(parameters)
+
+        # Creating solver and model part and adding variables
+        super(PoromechanicsAnalysis,self).__init__(model,parameters)
+
+        self.initial_stress_mode = 'external' # Not from a Poromechanics solution
+        if parameters["problem_data"].Has("initial_stress_utility_settings"):
+            self.initial_stress_mode = parameters["problem_data"]["initial_stress_utility_settings"]["mode"].GetString()
+        if (self.initial_stress_mode == 'load' or self.initial_stress_mode == 'save'):
+            from KratosMultiphysics.PoromechanicsApplication.poromechanics_initial_stress_utility import InitialStressUtility
+            self.initial_stress_utility = InitialStressUtility(model,parameters)
+
+    def Initialize(self):
+        super(PoromechanicsAnalysis,self).Initialize()
+
+        if (self.initial_stress_mode == 'load'):
+            self.initial_stress_utility.Load()
+
+    def OutputSolutionStep(self):
+        super(PoromechanicsAnalysis,self).OutputSolutionStep()
+
+        # Check Fracture Propagation Utility
+        if self.project_parameters["problem_data"]["fracture_utility"].GetBool():
+            if self.fracture_utility.IsPropagationStep():
+                self._solver,self._list_of_processes,self._list_of_output_processes = self.fracture_utility.CheckPropagation(self._solver,
+                                                                                                                            self._list_of_processes,
+                                                                                                                            self._list_of_output_processes)
+
+    def Finalize(self):
+        super(PoromechanicsAnalysis,self).Finalize()
+
+        # Finalize Fracture Propagation Utility
+        if self.project_parameters["problem_data"]["fracture_utility"].GetBool():
+            self.fracture_utility.Finalize()
+
+        if (self.initial_stress_mode == 'save'):
+            self.initial_stress_utility.Save()
+
+        # Finalizing strategy
+        if self.parallel_type == "OpenMP":
+            self._GetSolver().Clear()
+
+        # Time control
+        KratosMultiphysics.Logger.PrintInfo(self._GetSimulationName(),"Analysis Completed. Elapsed Time = %.3f" % (timer.perf_counter() - self.initial_time)," seconds.")
+        KratosMultiphysics.Logger.PrintInfo(self._GetSimulationName(),timer.ctime())
+
+    def _CreateSolver(self):
+        python_module_name = "KratosMultiphysics.PoromechanicsApplication"
+        full_module_name = python_module_name + "." + self.project_parameters["solver_settings"]["solver_type"].GetString()
+        solver_module = import_module(full_module_name)
+        solver = solver_module.CreateSolver(self.model, self.project_parameters["solver_settings"])
+        return solver
+
+    def _GetOrderOfProcessesInitialization(self):
+        return ["constraints_process_list",
+                "loads_process_list",
+                "auxiliar_process_list"]
+
+    def _GetSimulationName(self):
+        return "Poromechanics Analysis"
+
+
+if __name__ == '__main__':
+    from sys import argv
+
+    if len(argv) > 2:
+        err_msg =  'Too many input arguments!\n'
+        err_msg += 'Use this script in the following way:\n'
+        err_msg += '- With default parameter file (assumed to be called "ProjectParameters.json"):\n'
+        err_msg += '    "python poromechanics_analysis.py"\n'
+        err_msg += '- With custom parameter file:\n'
+        err_msg += '    "python poromechanics_analysis.py <my-parameter-file>.json"\n'
+        raise Exception(err_msg)
+
+    if len(argv) == 2: # ProjectParameters is being passed from outside
+        parameter_file_name = argv[1]
+    else: # using default name
+        parameter_file_name = "ProjectParameters.json"
+
+    with open(parameter_file_name,'r') as parameter_file:
+        parameters = Kratos.Parameters(parameter_file.read())
+
+    model = Kratos.Model()
+    simulation = PoromechanicsAnalysis(model,parameters)
+    simulation.Run()
```

## KratosMultiphysics/PoromechanicsApplication/poromechanics_cleaning_utility.py

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-import os
-
-def CleanPreviousFiles(problem_path):
-
-	file_ending_type = ".post.bin"
-	CleanPreviousFileType(file_ending_type,problem_path)
-
-	file_ending_type = ".post.res"
-	CleanPreviousFileType(file_ending_type,problem_path)
-
-	file_ending_type = ".post.msh"
-	CleanPreviousFileType(file_ending_type,problem_path)
-
-	file_ending_type = ".post.lst"
-	CleanPreviousFileType(file_ending_type,problem_path)
-
-	file_ending_type = "info.time"
-	CleanPreviousFileType(file_ending_type,problem_path)
-
-
-def CleanPreviousFileType(file_ending_type,problem_path):
-
+import os
+
+def CleanPreviousFiles(problem_path):
+
+	file_ending_type = ".post.bin"
+	CleanPreviousFileType(file_ending_type,problem_path)
+
+	file_ending_type = ".post.res"
+	CleanPreviousFileType(file_ending_type,problem_path)
+
+	file_ending_type = ".post.msh"
+	CleanPreviousFileType(file_ending_type,problem_path)
+
+	file_ending_type = ".post.lst"
+	CleanPreviousFileType(file_ending_type,problem_path)
+
+	file_ending_type = "info.time"
+	CleanPreviousFileType(file_ending_type,problem_path)
+
+
+def CleanPreviousFileType(file_ending_type,problem_path):
+
     [os.remove(f) for f in os.listdir(problem_path) if f.endswith(file_ending_type)]
```

## KratosMultiphysics/PoromechanicsApplication/poromechanics_initial_stress_utility.py

 * *Ordering differences only*

```diff
@@ -1,61 +1,61 @@
-
-# Import kratos core and applications
-import KratosMultiphysics
-import KratosMultiphysics.LinearSolversApplication
-import KratosMultiphysics.FluidDynamicsApplication
-import KratosMultiphysics.StructuralMechanicsApplication
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-
-from importlib import import_module
-
-class InitialStressUtility(object):
-
-    def __init__(self, model, parameters):
-
-        self.model = model
-        self.parameters = parameters
-
-        domain_size = self.parameters["solver_settings"]["domain_size"].GetInt()
-        if domain_size == 2:
-            self.initial_stress_utility = KratosPoro.InitialStress2DUtilities()
-        else:
-            self.initial_stress_utility = KratosPoro.InitialStress3DUtilities()
-
-        self.current_model_part = self.model.GetModelPart(self.parameters["solver_settings"]["model_part_name"].GetString())
-
-    def Load(self):
-        # Read the initial model part with initial stresses and perform a mapping to transfer them to the current model part
-
-        initial_model_part_name = 'InitialPorousModelPart'
-
-        # Create initial solver (and initial_model_part)
-        initial_solver_settings = self.parameters["solver_settings"]
-        initial_solver_settings["model_part_name"].SetString(initial_model_part_name)
-        initial_solver_settings["model_import_settings"]["input_filename"].SetString(self.parameters["problem_data"]["initial_stress_utility_settings"]["initial_input_filename"].GetString())
-        python_module_name = "KratosMultiphysics.PoromechanicsApplication"
-        full_module_name = python_module_name + "." + initial_solver_settings["solver_type"].GetString()
-        solver_module = import_module(full_module_name)
-        initial_solver = solver_module.CreateSolver(self.model, initial_solver_settings)
-
-        initial_solver.AddVariables()
-        initial_solver.ImportModelPart()
-        # initial_solver.PrepareModelPart()
-        initial_solver.AddDofs()
-
-        # Mapping between initial and current model parts
-        initial_model_part = self.model.GetModelPart(initial_model_part_name)
-
-        self.initial_stress_utility.TransferInitialStresses(initial_model_part,self.current_model_part)
-
-        # Delete initial_model_part
-        self.model.DeleteModelPart(initial_model_part_name)
-
-    def Save(self):
-        # Write an mdpa file containing the initial stress tensor as NodalData
-
-        initial_stress_parameters = KratosMultiphysics.Parameters("{}")
-        initial_stress_parameters.AddValue("initial_input_filename",self.parameters["problem_data"]["initial_stress_utility_settings"]["initial_input_filename"])
-
-        self.current_model_part.ProcessInfo.SetValue(KratosPoro.NODAL_SMOOTHING, True)
-
-        self.initial_stress_utility.SaveInitialStresses(initial_stress_parameters,self.current_model_part)
+
+# Import kratos core and applications
+import KratosMultiphysics
+import KratosMultiphysics.LinearSolversApplication
+import KratosMultiphysics.FluidDynamicsApplication
+import KratosMultiphysics.StructuralMechanicsApplication
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+
+from importlib import import_module
+
+class InitialStressUtility(object):
+
+    def __init__(self, model, parameters):
+
+        self.model = model
+        self.parameters = parameters
+
+        domain_size = self.parameters["solver_settings"]["domain_size"].GetInt()
+        if domain_size == 2:
+            self.initial_stress_utility = KratosPoro.InitialStress2DUtilities()
+        else:
+            self.initial_stress_utility = KratosPoro.InitialStress3DUtilities()
+
+        self.current_model_part = self.model.GetModelPart(self.parameters["solver_settings"]["model_part_name"].GetString())
+
+    def Load(self):
+        # Read the initial model part with initial stresses and perform a mapping to transfer them to the current model part
+
+        initial_model_part_name = 'InitialPorousModelPart'
+
+        # Create initial solver (and initial_model_part)
+        initial_solver_settings = self.parameters["solver_settings"]
+        initial_solver_settings["model_part_name"].SetString(initial_model_part_name)
+        initial_solver_settings["model_import_settings"]["input_filename"].SetString(self.parameters["problem_data"]["initial_stress_utility_settings"]["initial_input_filename"].GetString())
+        python_module_name = "KratosMultiphysics.PoromechanicsApplication"
+        full_module_name = python_module_name + "." + initial_solver_settings["solver_type"].GetString()
+        solver_module = import_module(full_module_name)
+        initial_solver = solver_module.CreateSolver(self.model, initial_solver_settings)
+
+        initial_solver.AddVariables()
+        initial_solver.ImportModelPart()
+        # initial_solver.PrepareModelPart()
+        initial_solver.AddDofs()
+
+        # Mapping between initial and current model parts
+        initial_model_part = self.model.GetModelPart(initial_model_part_name)
+
+        self.initial_stress_utility.TransferInitialStresses(initial_model_part,self.current_model_part)
+
+        # Delete initial_model_part
+        self.model.DeleteModelPart(initial_model_part_name)
+
+    def Save(self):
+        # Write an mdpa file containing the initial stress tensor as NodalData
+
+        initial_stress_parameters = KratosMultiphysics.Parameters("{}")
+        initial_stress_parameters.AddValue("initial_input_filename",self.parameters["problem_data"]["initial_stress_utility_settings"]["initial_input_filename"])
+
+        self.current_model_part.ProcessInfo.SetValue(KratosPoro.NODAL_SMOOTHING, True)
+
+        self.initial_stress_utility.SaveInitialStresses(initial_stress_parameters,self.current_model_part)
```

## Comparing `KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pw_explicit_dynamic_solver.py` & `KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pl_explicit_dynamic_solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications
-import KratosMultiphysics.FluidDynamicsApplication as KratosCFD
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-import KratosMultiphysics.StructuralMechanicsApplication as StructuralMechanicsApplication
-
-# Import base class file
-from KratosMultiphysics.PoromechanicsApplication.poromechanics_U_Pw_solver import UPwSolver
-
-def CreateSolver(model, custom_settings):
-    return ExplicitUPwSolver(model, custom_settings)
-
-class ExplicitUPwSolver(UPwSolver):
-    """The Poromechanics explicit U (displacement) dynamic solver.
-
-    This class creates the mechanical solvers for explicit dynamic analysis.
-    """
-    def __init__(self, model, custom_settings):
-        # Construct the base solver.
-        super().__init__(model, custom_settings)
-
-        self.min_buffer_size = 2           
-
-        # Lumped mass-matrix is necessary for explicit analysis
-        self.main_model_part.ProcessInfo[KratosMultiphysics.COMPUTE_LUMPED_MASS_MATRIX] = True
-        KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: Construction finished")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        this_defaults = KratosMultiphysics.Parameters("""{
-            "scheme_type"                : "Explicit_Central_Differences",
-            "rebuild_level"              : 0,
-            "theta_factor"               : 1.0,
-            "g_factor"                   : 0.0,
-            "calculate_xi"               : false,
-            "xi_1_factor"                : 1.0
-        }""")
-        this_defaults.AddMissingParameters(super().GetDefaultParameters())
-        return this_defaults
-
-    def AddVariables(self):
-        super().AddVariables()
-
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.DISPLACEMENT_OLD)
-        # self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.DISPLACEMENT_OLDER)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.INTERNAL_FORCE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.EXTERNAL_FORCE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FORCE_RESIDUAL)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.FLUX_RESIDUAL)
-
-        scheme_type = self.settings["scheme_type"].GetString()
-        if(scheme_type == "Explicit_Velocity_Verlet"):
-            self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.DAMPING_FORCE)
-        
-        # self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_MASS)
-        # self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.RESIDUAL_VECTOR)
-
-        KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: Variables ADDED")
-
-    def AddDofs(self):
-        # super().AddDofs()
-        ## Solid dofs
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_X, KratosMultiphysics.REACTION_X,self.main_model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Y, KratosMultiphysics.REACTION_Y,self.main_model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Z, KratosMultiphysics.REACTION_Z,self.main_model_part)
-
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.VELOCITY_X,self.main_model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.VELOCITY_Y,self.main_model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.VELOCITY_Z,self.main_model_part)
-
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.ACCELERATION_X,self.main_model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.ACCELERATION_Y,self.main_model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.ACCELERATION_Z,self.main_model_part)
-
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.WATER_PRESSURE, KratosMultiphysics.REACTION_WATER_PRESSURE,self.main_model_part)
-
-        KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: DOF's ADDED")
-
-    def Initialize(self):
-        # Using the base Initialize
-        # super().Initialize()
-        """Perform initialization after adding nodal variables and dofs to the main model part. """
-
-        self.computing_model_part = self.GetComputingModelPart()
-
-        # Fill the previous steps of the buffer with the initial conditions
-        self._FillBuffer()
-
-        # Solution scheme creation
-        self.scheme = self._ConstructScheme(self.settings["scheme_type"].GetString())
-
-        # Solver creation
-        self.solver = self._ConstructSolver(self.settings["strategy_type"].GetString())
-
-        # Set echo_level
-        self.SetEchoLevel(self.settings["echo_level"].GetInt())
-
-        # Initialize Strategy
-        if self.settings["clear_storage"].GetBool():
-            self.Clear()
-
-        self.solver.Initialize()
-
-        # Check if everything is assigned correctly
-        self.Check()
-
-        # Check and construct gp_to_nodal_variable process
-        self._CheckAndConstructGPtoNodalVariableExtrapolationProcess()
-
-    #### Specific internal functions ####
-    def _ConstructScheme(self, scheme_type):
-        scheme_type = self.settings["scheme_type"].GetString()
-
-        # Setting the Rayleigh damping parameters
-        process_info = self.main_model_part.ProcessInfo
-        g_factor = self.settings["g_factor"].GetDouble()
-        theta_factor = self.settings["theta_factor"].GetDouble()
-        g_coeff = 0.0
-        Dt = self.settings["time_step"].GetDouble()
-        omega_1 = self.settings["omega_1"].GetDouble()
-        omega_n = self.settings["omega_n"].GetDouble()
-        rayleigh_alpha = self.settings["rayleigh_alpha"].GetDouble()
-        rayleigh_beta = self.settings["rayleigh_beta"].GetDouble()
-        if (scheme_type == "Explicit_Central_Differences" and g_factor >= 1.0):
-            theta_factor = 0.5
-            g_coeff = Dt*omega_n*omega_n*0.25*g_factor
-        if self.settings["calculate_alpha_beta"].GetBool():
-            xi_1 = self.settings["xi_1"].GetDouble()
-            xi_n = self.settings["xi_n"].GetDouble()
-            if (scheme_type == "Explicit_Central_Differences" and self.settings["calculate_xi"].GetBool()==True):
-                xi_1_factor = self.settings["xi_1_factor"].GetDouble()                
-                import numpy as np
-                xi_1 = (np.sqrt(1+g_coeff*Dt)-theta_factor*omega_1*Dt*0.5)*xi_1_factor
-                xi_n = (np.sqrt(1+g_coeff*Dt)-theta_factor*omega_n*Dt*0.5)
-            rayleigh_beta = 2.0*(xi_n*omega_n-xi_1*omega_1)/(omega_n*omega_n-omega_1*omega_1)
-            rayleigh_alpha = 2.0*xi_1*omega_1-rayleigh_beta*omega_1*omega_1
-            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: Scheme Information")
-            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: dt: ",Dt)
-            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: g_coeff: ",g_coeff)
-            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: omega_1: ",omega_1)
-            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: omega_n: ",omega_n)
-            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: xi_1: ",xi_1)
-            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: xi_n: ",xi_n)
-            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: Alpha and Beta output")
-            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: rayleigh_alpha: ",rayleigh_alpha)
-            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPwSolver]:: rayleigh_beta: ",rayleigh_beta)
-        
-        process_info.SetValue(StructuralMechanicsApplication.RAYLEIGH_ALPHA, rayleigh_alpha)
-        process_info.SetValue(StructuralMechanicsApplication.RAYLEIGH_BETA, rayleigh_beta)
-        process_info.SetValue(KratosPoro.G_COEFFICIENT, g_coeff)
-        process_info.SetValue(KratosPoro.THETA_FACTOR, theta_factor)
-
-        # Setting the time integration schemes
-        if(scheme_type == "Explicit_Central_Differences"):
-            scheme = KratosPoro.PoroExplicitCDScheme()
-        elif(scheme_type == "Explicit_Velocity_Verlet"):
-            scheme = KratosPoro.PoroExplicitVVScheme()
-        else:
-            err_msg =  "The requested scheme type \"" + scheme_type + "\" is not available!\n"
-            err_msg += "Available options are: \"Explicit_Central_Differences\", \"Explicit_Velocity_Verlet\" "
-            raise Exception(err_msg)
-        return scheme
-
-    def _ConstructSolver(self, strategy_type):
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.ERROR_RATIO, self.settings["displacement_relative_tolerance"].GetDouble())
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.ERROR_INTEGRATION_POINT, self.settings["displacement_absolute_tolerance"].GetDouble())
-        self.main_model_part.ProcessInfo.SetValue(KratosPoro.IS_CONVERGED, True)
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.NL_ITERATION_NUMBER, 1)
-
-        nonlocal_damage = self.settings["nonlocal_damage"].GetBool()
-        compute_reactions = self.settings["compute_reactions"].GetBool()
-        reform_step_dofs = self.settings["reform_dofs_at_each_step"].GetBool()
-        move_mesh_flag = self.settings["move_mesh_flag"].GetBool()
-
-        self.strategy_params = KratosMultiphysics.Parameters("{}")
-        self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
-        self.strategy_params.AddValue("loads_variable_list",self.settings["loads_variable_list"])
-        # NOTE: A rebuild level of 0 means that the nodal mass is calculated only once at the beginning (Initialize)
-        #       A rebuild level higher than 0 means that the nodal mass can be updated at the beginning of each step (InitializeSolutionStep)
-        self.strategy_params.AddValue("rebuild_level",self.settings["rebuild_level"])
-
-        if nonlocal_damage:
-            self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
-            self.strategy_params.AddValue("characteristic_length",self.settings["characteristic_length"])
-            self.strategy_params.AddValue("search_neighbours_step",self.settings["search_neighbours_step"])
-            solving_strategy = KratosPoro.PoromechanicsExplicitNonlocalStrategy(self.computing_model_part,
-                                                                            self.scheme,
-                                                                            self.strategy_params,
-                                                                            compute_reactions,
-                                                                            reform_step_dofs,
-                                                                            move_mesh_flag)
-        else:
-            solving_strategy = KratosPoro.PoromechanicsExplicitStrategy(self.computing_model_part,
-                                                                            self.scheme,
-                                                                            self.strategy_params,
-                                                                            compute_reactions,
-                                                                            reform_step_dofs,
-                                                                            move_mesh_flag)
-
-        return solving_strategy
-
-    #### Private functions ####
-
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications
+import KratosMultiphysics.FluidDynamicsApplication as KratosCFD
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+import KratosMultiphysics.StructuralMechanicsApplication as StructuralMechanicsApplication
+
+# Import base class file
+from KratosMultiphysics.PoromechanicsApplication.poromechanics_U_Pl_solver import UPlSolver
+
+def CreateSolver(model, custom_settings):
+    return ExplicitUPlSolver(model, custom_settings)
+
+class ExplicitUPlSolver(UPlSolver):
+    """The Poromechanics explicit U (displacement) dynamic solver.
+
+    This class creates the mechanical solvers for explicit dynamic analysis.
+    """
+    def __init__(self, model, custom_settings):
+        # Construct the base solver.
+        super(ExplicitUPlSolver,self).__init__(model, custom_settings)
+
+        self.min_buffer_size = 2           
+
+        # Lumped mass-matrix is necessary for explicit analysis
+        self.main_model_part.ProcessInfo[KratosMultiphysics.COMPUTE_LUMPED_MASS_MATRIX] = True
+        KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: Construction finished")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        this_defaults = KratosMultiphysics.Parameters("""{
+            "scheme_type"                : "Explicit_Central_Differences",
+            "rebuild_level"              : 0,
+            "theta_factor"               : 1.0,
+            "g_factor"                   : 0.0,
+            "calculate_xi"               : false,
+            "xi_1_factor"                : 1.0
+        }""")
+        this_defaults.AddMissingParameters(super(ExplicitUPlSolver,cls).GetDefaultParameters())
+        return this_defaults
+
+    def AddVariables(self):
+        super(ExplicitUPlSolver,self).AddVariables()
+
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.DISPLACEMENT_OLD)
+        # self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.DISPLACEMENT_OLDER)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.INTERNAL_FORCE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.EXTERNAL_FORCE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FORCE_RESIDUAL)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.FLUX_RESIDUAL)
+
+        scheme_type = self.settings["scheme_type"].GetString()
+        if(scheme_type == "Explicit_Velocity_Verlet"):
+            self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.DAMPING_FORCE)
+        
+        # self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_MASS)
+        # self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.RESIDUAL_VECTOR)
+
+        KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: Variables ADDED")
+
+    def AddDofs(self):
+        # super(ExplicitUPlSolver,self).AddDofs()
+        ## Solid dofs
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_X, KratosMultiphysics.REACTION_X,self.main_model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Y, KratosMultiphysics.REACTION_Y,self.main_model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Z, KratosMultiphysics.REACTION_Z,self.main_model_part)
+
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.VELOCITY_X,self.main_model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.VELOCITY_Y,self.main_model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.VELOCITY_Z,self.main_model_part)
+
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.ACCELERATION_X,self.main_model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.ACCELERATION_Y,self.main_model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.ACCELERATION_Z,self.main_model_part)
+
+        KratosMultiphysics.VariableUtils().AddDof(KratosPoro.LIQUID_PRESSURE, KratosPoro.REACTION_LIQUID_PRESSURE,self.main_model_part)
+
+        KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: DOF's ADDED")
+
+    def Initialize(self):
+        # Using the base Initialize
+        # super(ExplicitUPlSolver,self).Initialize()
+        """Perform initialization after adding nodal variables and dofs to the main model part. """
+
+        self.computing_model_part = self.GetComputingModelPart()
+
+        # Fill the previous steps of the buffer with the initial conditions
+        self._FillBuffer()
+
+        # Solution scheme creation
+        self.scheme = self._ConstructScheme(self.settings["scheme_type"].GetString())
+
+        # Solver creation
+        self.solver = self._ConstructSolver(self.settings["strategy_type"].GetString())
+
+        # Set echo_level
+        self.SetEchoLevel(self.settings["echo_level"].GetInt())
+
+        # Initialize Strategy
+        if self.settings["clear_storage"].GetBool():
+            self.Clear()
+
+        self.solver.Initialize()
+
+        # Check if everything is assigned correctly
+        self.Check()
+
+        # Check and construct gp_to_nodal_variable process
+        self._CheckAndConstructGPtoNodalVariableExtrapolationProcess()
+
+    #### Specific internal functions ####
+    def _ConstructScheme(self, scheme_type):
+        scheme_type = self.settings["scheme_type"].GetString()
+
+        # Setting the Rayleigh damping parameters
+        process_info = self.main_model_part.ProcessInfo
+        g_factor = self.settings["g_factor"].GetDouble()
+        theta_factor = self.settings["theta_factor"].GetDouble()
+        g_coeff = 0.0
+        Dt = self.settings["time_step"].GetDouble()
+        omega_1 = self.settings["omega_1"].GetDouble()
+        omega_n = self.settings["omega_n"].GetDouble()
+        rayleigh_alpha = self.settings["rayleigh_alpha"].GetDouble()
+        rayleigh_beta = self.settings["rayleigh_beta"].GetDouble()
+        if (scheme_type == "Explicit_Central_Differences" and g_factor >= 1.0):
+            theta_factor = 0.5
+            g_coeff = Dt*omega_n*omega_n*0.25*g_factor
+        if self.settings["calculate_alpha_beta"].GetBool():
+            xi_1 = self.settings["xi_1"].GetDouble()
+            xi_n = self.settings["xi_n"].GetDouble()
+            if (scheme_type == "Explicit_Central_Differences" and self.settings["calculate_xi"].GetBool()==True):
+                xi_1_factor = self.settings["xi_1_factor"].GetDouble()                
+                import numpy as np
+                xi_1 = (np.sqrt(1+g_coeff*Dt)-theta_factor*omega_1*Dt*0.5)*xi_1_factor
+                xi_n = (np.sqrt(1+g_coeff*Dt)-theta_factor*omega_n*Dt*0.5)
+            rayleigh_beta = 2.0*(xi_n*omega_n-xi_1*omega_1)/(omega_n*omega_n-omega_1*omega_1)
+            rayleigh_alpha = 2.0*xi_1*omega_1-rayleigh_beta*omega_1*omega_1
+            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: Scheme Information")
+            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: dt: ",Dt)
+            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: g_coeff: ",g_coeff)
+            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: omega_1: ",omega_1)
+            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: omega_n: ",omega_n)
+            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: xi_1: ",xi_1)
+            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: xi_n: ",xi_n)
+            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: Alpha and Beta output")
+            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: rayleigh_alpha: ",rayleigh_alpha)
+            KratosMultiphysics.Logger.PrintInfo("::[ExplicitUPlSolver]:: rayleigh_beta: ",rayleigh_beta)
+        
+        process_info.SetValue(StructuralMechanicsApplication.RAYLEIGH_ALPHA, rayleigh_alpha)
+        process_info.SetValue(StructuralMechanicsApplication.RAYLEIGH_BETA, rayleigh_beta)
+        process_info.SetValue(KratosPoro.G_COEFFICIENT, g_coeff)
+        process_info.SetValue(KratosPoro.THETA_FACTOR, theta_factor)
+
+        # Setting the time integration schemes
+        if(scheme_type == "Explicit_Central_Differences"):
+            scheme = KratosPoro.PoroExplicitCDScheme()
+        elif(scheme_type == "Explicit_Velocity_Verlet"):
+            scheme = KratosPoro.PoroExplicitVVScheme()
+        else:
+            err_msg =  "The requested scheme type \"" + scheme_type + "\" is not available!\n"
+            err_msg += "Available options are: \"Explicit_Central_Differences\", \"Explicit_Velocity_Verlet\" "
+            raise Exception(err_msg)
+        return scheme
+
+    def _ConstructSolver(self, strategy_type):
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.ERROR_RATIO, self.settings["displacement_relative_tolerance"].GetDouble())
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.ERROR_INTEGRATION_POINT, self.settings["displacement_absolute_tolerance"].GetDouble())
+        self.main_model_part.ProcessInfo.SetValue(KratosPoro.IS_CONVERGED, True)
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.NL_ITERATION_NUMBER, 1)
+
+        nonlocal_damage = self.settings["nonlocal_damage"].GetBool()
+        compute_reactions = self.settings["compute_reactions"].GetBool()
+        reform_step_dofs = self.settings["reform_dofs_at_each_step"].GetBool()
+        move_mesh_flag = self.settings["move_mesh_flag"].GetBool()
+
+        self.strategy_params = KratosMultiphysics.Parameters("{}")
+        self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
+        self.strategy_params.AddValue("loads_variable_list",self.settings["loads_variable_list"])
+        # NOTE: A rebuild level of 0 means that the nodal mass is calculated only once at the beginning (Initialize)
+        #       A rebuild level higher than 0 means that the nodal mass can be updated at the beginning of each step (InitializeSolutionStep)
+        self.strategy_params.AddValue("rebuild_level",self.settings["rebuild_level"])
+
+        if nonlocal_damage:
+            self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
+            self.strategy_params.AddValue("characteristic_length",self.settings["characteristic_length"])
+            self.strategy_params.AddValue("search_neighbours_step",self.settings["search_neighbours_step"])
+            solving_strategy = KratosPoro.PoromechanicsExplicitNonlocalStrategy(self.computing_model_part,
+                                                                            self.scheme,
+                                                                            self.strategy_params,
+                                                                            compute_reactions,
+                                                                            reform_step_dofs,
+                                                                            move_mesh_flag)
+        else:
+            solving_strategy = KratosPoro.PoromechanicsExplicitStrategy(self.computing_model_part,
+                                                                            self.scheme,
+                                                                            self.strategy_params,
+                                                                            compute_reactions,
+                                                                            reform_step_dofs,
+                                                                            move_mesh_flag)
+
+        return solving_strategy
+
+    #### Private functions ####
+
```

## Comparing `KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pw_solver.py` & `KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pl_solver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,580 +1,579 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-from KratosMultiphysics.python_solver import PythonSolver
-
-# Import applications
-import KratosMultiphysics.FluidDynamicsApplication as KratosCFD
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-
-def CreateSolver(model, custom_settings):
-    return UPwSolver(model, custom_settings)
-
-class UPwSolver(PythonSolver):
-    '''Solver for the solution of displacement-pore pressure coupled problems.'''
-
-    def __init__(self, model, custom_settings):
-
-        self._validate_settings_in_baseclass=True # To be removed eventually
-
-        super(UPwSolver,self).__init__(model, custom_settings)
-
-        self.min_buffer_size = 2
-
-        # Either retrieve the model part from the model or create a new one
-        model_part_name = self.settings["model_part_name"].GetString()
-
-        if model_part_name == "":
-            raise Exception('Please specify a model_part name!')
-
-        if self.model.HasModelPart(model_part_name):
-            self.main_model_part = self.model.GetModelPart(model_part_name)
-        else:
-            self.main_model_part = self.model.CreateModelPart(model_part_name,self.min_buffer_size)
-
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE,
-                                                  self.settings["domain_size"].GetInt())
-
-        KratosMultiphysics.Logger.PrintInfo("UPwSolver", "Construction of UPwSolver finished.")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        this_defaults = KratosMultiphysics.Parameters("""{
-            "solver_type": "poromechanics_U_Pw_solver",
-            "model_part_name": "PorousModelPart",
-            "domain_size": 2,
-            "start_time": 0.0,
-            "time_step": 0.1,
-            "model_import_settings":{
-                "input_type": "mdpa",
-                "input_filename": "unknown_name"
-            },
-            "material_import_settings" :{
-                "materials_filename": ""
-            },
-            "buffer_size": 2,
-            "echo_level": 0,
-            "reform_dofs_at_each_step": false,
-            "clear_storage": false,
-            "compute_reactions": false,
-            "move_mesh_flag": false,
-            "nodal_smoothing": false,
-            "gp_to_nodal_variable_list": [],
-            "gp_to_nodal_variable_extrapolate_non_historical": false,
-            "periodic_interface_conditions": false,
-            "solution_type": "implicit_quasi_static",
-            "scheme_type": "Newmark",
-            "newmark_beta": 0.25,
-            "newmark_gamma": 0.5,
-            "newmark_theta": 0.5,
-            "calculate_alpha_beta"       : false,
-            "omega_1"                    : 1.0,
-            "omega_n"                    : 10.0,
-            "xi_1"                       : 1.0,
-            "xi_n"                       : 0.05,
-            "rayleigh_alpha": 0.0,
-            "rayleigh_beta": 0.0,
-            "strategy_type": "newton_raphson",
-            "convergence_criterion": "Displacement_criterion",
-            "displacement_relative_tolerance": 1.0e-4,
-            "displacement_absolute_tolerance": 1.0e-9,
-            "residual_relative_tolerance": 1.0e-4,
-            "residual_absolute_tolerance": 1.0e-9,
-            "max_iteration": 15,
-            "desired_iterations": 4,
-            "max_radius_factor": 20.0,
-            "min_radius_factor": 0.5,
-            "block_builder": true,
-            "nonlocal_damage": false,
-            "characteristic_length": 0.05,
-            "search_neighbours_step": false,
-            "linear_solver_settings":{
-                "solver_type": "amgcl",
-                "tolerance": 1.0e-6,
-                "max_iteration": 100,
-                "scaling": false,
-                "verbosity": 0,
-                "preconditioner_type": "ilu0",
-                "smoother_type": "ilu0",
-                "krylov_type": "gmres",
-                "coarsening_type": "aggregation"
-            },
-            "problem_domain_sub_model_part_list": [""],
-            "processes_sub_model_part_list": [""],
-            "body_domain_sub_model_part_list": [""],
-            "loads_sub_model_part_list": [],
-            "loads_variable_list": []
-        }""")
-
-        this_defaults.AddMissingParameters(super(UPwSolver, cls).GetDefaultParameters())
-        return this_defaults
-
-    def AddVariables(self):
-
-        ## Solid Variables
-        # Add displacements
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
-        # Add reactions for the displacements
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
-        # Add dynamic variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
-        # Add variables for the solid conditions
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FORCE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FACE_LOAD)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NORMAL_CONTACT_STRESS)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.TANGENTIAL_CONTACT_STRESS)
-        ## Fluid Variables
-        # Add water pressure
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.WATER_PRESSURE)
-        # Add reactions for the water pressure
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION_WATER_PRESSURE)
-        # Add dynamic variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.DT_WATER_PRESSURE)
-        # Add variables for the water conditions
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NORMAL_FLUID_FLUX)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.DISCHARGE)
-        ## Other variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VOLUME_ACCELERATION)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PERIODIC_PAIR_INDEX)
-
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_DAMAGE_VARIABLE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_AREA)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_WIDTH)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_DAMAGE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_AREA)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_EFFECTIVE_STRESS_TENSOR)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_WATER_PRESSURE_GRADIENT)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.INITIAL_STRESS_TENSOR)
-
-        # Add variables from gp to nodal variable list
-        if self.settings["gp_to_nodal_variable_extrapolate_non_historical"].GetBool()==False:
-            for i in range(self.settings["gp_to_nodal_variable_list"].size()):
-                variable_name = self.settings["gp_to_nodal_variable_list"][i].GetString()
-                variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name)
-                self.main_model_part.AddNodalSolutionStepVariable(variable)
-
-        KratosMultiphysics.Logger.PrintInfo("UPwSolver", "Variables added correctly.")
-
-    def ImportModelPart(self):
-        # we can use the default implementation in the base class
-        self._ImportModelPart(self.main_model_part,self.settings["model_import_settings"])
-
-    def PrepareModelPart(self):
-
-        # Set ProcessInfo variables
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME,
-                                                  self.settings["start_time"].GetDouble())
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME,
-                                                  self.settings["time_step"].GetDouble())
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.STEP, 0)
-        self.main_model_part.ProcessInfo.SetValue(KratosPoro.TIME_UNIT_CONVERTER, 1.0)
-        if(self.settings["nodal_smoothing"].GetBool() == True):
-            self.main_model_part.ProcessInfo.SetValue(KratosPoro.NODAL_SMOOTHING, True)
-        else:
-            self.main_model_part.ProcessInfo.SetValue(KratosPoro.NODAL_SMOOTHING, False)
-
-        if not self.main_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
-            ## Executes the check and prepare model process (Create computing_model_part and set constitutive law)
-            self._ExecuteCheckAndPrepare()
-            ## Set buffer size
-            self._SetBufferSize()
-
-        KratosMultiphysics.Logger.PrintInfo("UPwSolver", "Model reading finished.")
-
-    def AddDofs(self):
-        ## Solid dofs
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_X, KratosMultiphysics.REACTION_X,self.main_model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Y, KratosMultiphysics.REACTION_Y,self.main_model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Z, KratosMultiphysics.REACTION_Z,self.main_model_part)
-        ## Fluid dofs
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.WATER_PRESSURE, KratosMultiphysics.REACTION_WATER_PRESSURE,self.main_model_part)
-
-        if(self.settings["solution_type"].GetString() == "implicit_dynamic"):
-            for node in self.main_model_part.Nodes:
-                # adding VELOCITY as dofs
-                node.AddDof(KratosMultiphysics.VELOCITY_X)
-                node.AddDof(KratosMultiphysics.VELOCITY_Y)
-                node.AddDof(KratosMultiphysics.VELOCITY_Z)
-                # adding ACCELERATION as dofs
-                node.AddDof(KratosMultiphysics.ACCELERATION_X)
-                node.AddDof(KratosMultiphysics.ACCELERATION_Y)
-                node.AddDof(KratosMultiphysics.ACCELERATION_Z)
-
-        KratosMultiphysics.Logger.PrintInfo("UPwSolver", "DOFs added correctly.")
-
-    def GetMinimumBufferSize(self):
-        return self.min_buffer_size
-
-    def Initialize(self):
-        self.computing_model_part = self.GetComputingModelPart()
-
-        # Fill the previous steps of the buffer with the initial conditions
-        self._FillBuffer()
-
-        # Construct the linear solver
-        self.linear_solver = self._ConstructLinearSolver()
-
-        # Builder and solver creation
-        builder_and_solver = self._ConstructBuilderAndSolver(self.settings["block_builder"].GetBool())
-
-        # Solution scheme creation
-        self.scheme = self._ConstructScheme(self.settings["scheme_type"].GetString(),
-                                         self.settings["solution_type"].GetString())
-
-        # Get the convergence criterion
-        self.convergence_criterion = self._ConstructConvergenceCriterion(self.settings["convergence_criterion"].GetString())
-
-        # Solver creation
-        self.solver = self._ConstructSolver(builder_and_solver,
-                                            self.settings["strategy_type"].GetString())
-
-        # Set echo_level
-        self.SetEchoLevel(self.settings["echo_level"].GetInt())
-
-        # Initialize Strategy
-        if self.settings["clear_storage"].GetBool():
-            self.Clear()
-
-        self.solver.Initialize()
-
-        # Check if everything is assigned correctly
-        self.Check()
-
-        # Check and construct gp_to_nodal_variable process
-        self._CheckAndConstructGPtoNodalVariableExtrapolationProcess()
-
-        KratosMultiphysics.Logger.PrintInfo("UPwSolver", "Solver initialization finished.")
-
-    def GetComputingModelPart(self):
-        return self.main_model_part.GetSubModelPart(self.computing_model_part_name)
-
-    def ComputeDeltaTime(self):
-        return self.main_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
-
-    def Clear(self):
-        self.solver.Clear()
-
-    def Check(self):
-        self.solver.Check()
-
-    def SetEchoLevel(self, level):
-        self.solver.SetEchoLevel(level)
-
-    def AdvanceInTime(self, current_time):
-        dt = self.ComputeDeltaTime()
-        new_time = current_time + dt
-
-        self.main_model_part.CloneTimeStep(new_time)
-        self.main_model_part.ProcessInfo[KratosMultiphysics.STEP] += 1
-
-        return new_time
-
-    def InitializeSolutionStep(self):
-        self.solver.InitializeSolutionStep()
-
-    def Predict(self):
-        self.solver.Predict()
-
-    def SolveSolutionStep(self):
-        is_converged = self.solver.SolveSolutionStep()
-        return is_converged
-
-    def FinalizeSolutionStep(self):
-        self.solver.FinalizeSolutionStep()
-
-        if self.gp_to_nodal_variable:
-            self.integration_values_extrapolation_to_nodes_process.ExecuteBeforeSolutionLoop()
-            self.integration_values_extrapolation_to_nodes_process.ExecuteFinalizeSolutionStep()
-
-    def Finalize(self):
-        if self.gp_to_nodal_variable:
-            self.integration_values_extrapolation_to_nodes_process.ExecuteFinalize()
-
-    def Solve(self):
-        message = "".join([
-            "Calling UPwSolver.Solve() method, which is deprecated\n",
-            "Please call the individual methods instead:\n",
-            "solver.InitializeSolutionStep()\n",
-            "solver.Predict()\n",
-            "solver.SolveSolutionStep()\n",
-            "solver.FinalizeSolutionStep()\n"]
-        )
-        KratosMultiphysics.Logger.PrintWarning("UPwSolver",message)
-
-        if self.settings["clear_storage"].GetBool():
-            self.Clear()
-
-        self.InitializeSolutionStep()
-        self.Predict()
-        self.SolveSolutionStep()
-        self.FinalizeSolutionStep()
-
-    #### Specific internal functions ####
-
-    def _ExecuteCheckAndPrepare(self):
-
-        self.computing_model_part_name = "porous_computational_model_part"
-
-        # Create list of sub sub model parts (it is a copy of the standard lists with a different name)
-        import json
-
-        self.body_domain_sub_sub_model_part_list = []
-        for i in range(self.settings["body_domain_sub_model_part_list"].size()):
-            self.body_domain_sub_sub_model_part_list.append("sub_"+self.settings["body_domain_sub_model_part_list"][i].GetString())
-        self.body_domain_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.body_domain_sub_sub_model_part_list))
-
-        self.loads_sub_sub_model_part_list = []
-        for i in range(self.settings["loads_sub_model_part_list"].size()):
-            self.loads_sub_sub_model_part_list.append("sub_"+self.settings["loads_sub_model_part_list"][i].GetString())
-        self.loads_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.loads_sub_sub_model_part_list))
-
-        # Auxiliary parameters object for the CheckAndPepareModelProcess
-        params = KratosMultiphysics.Parameters("{}")
-        params.AddEmptyValue("computing_model_part_name").SetString(self.computing_model_part_name)
-        params.AddValue("problem_domain_sub_model_part_list",self.settings["problem_domain_sub_model_part_list"])
-        params.AddValue("processes_sub_model_part_list",self.settings["processes_sub_model_part_list"])
-        params.AddValue("body_domain_sub_model_part_list",self.settings["body_domain_sub_model_part_list"])
-        params.AddValue("body_domain_sub_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
-        params.AddValue("loads_sub_model_part_list",self.settings["loads_sub_model_part_list"])
-        params.AddValue("loads_sub_sub_model_part_list",self.loads_sub_sub_model_part_list)
-        # CheckAndPrepareModelProcess creates the porous_computational_model_part
-        from KratosMultiphysics.PoromechanicsApplication import check_and_prepare_model_process_poro
-        check_and_prepare_model_process_poro.CheckAndPrepareModelProcess(self.main_model_part, params).Execute()
-
-        # Constitutive law import
-        materials_imported = self.import_constitutive_laws()
-        if materials_imported:
-            KratosMultiphysics.Logger.PrintInfo("UPwSolver", "Constitutive law was successfully imported via json.")
-        else:
-            KratosMultiphysics.Logger.PrintInfo("UPwSolver", "Constitutive law was not successfully imported.")
-
-    def import_constitutive_laws(self):
-        materials_filename = self.settings["material_import_settings"]["materials_filename"].GetString()
-        if (materials_filename != ""):
-            # Add constitutive laws and material properties from json file to model parts.
-            material_settings = KratosMultiphysics.Parameters("""{"Parameters": {"materials_filename": ""}} """)
-            material_settings["Parameters"]["materials_filename"].SetString(materials_filename)
-            KratosMultiphysics.ReadMaterialsUtility(material_settings, self.model)
-            materials_imported = True
-        else:
-            materials_imported = False
-        return materials_imported
-
-    def _SetBufferSize(self):
-        required_buffer_size = self.settings["buffer_size"].GetInt()
-        if required_buffer_size < self.GetMinimumBufferSize():
-            required_buffer_size = self.GetMinimumBufferSize()
-        current_buffer_size = self.main_model_part.GetBufferSize()
-        buffer_size = max(current_buffer_size, required_buffer_size)
-        self.main_model_part.SetBufferSize(buffer_size)
-
-    def _FillBuffer(self):
-        buffer_size = self.main_model_part.GetBufferSize()
-        time = self.main_model_part.ProcessInfo[KratosMultiphysics.TIME]
-        delta_time = self.main_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
-        step = self.main_model_part.ProcessInfo[KratosMultiphysics.STEP]
-
-        step = step - (buffer_size-1)*1
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.STEP, step)
-        time = time - (buffer_size-1)*delta_time
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, time)
-        for i in range(buffer_size-1):
-            step = step + 1
-            self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.STEP, step)
-            time = time + delta_time
-            self.main_model_part.CloneTimeStep(time)
-
-    def _ConstructLinearSolver(self):
-        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
-        return linear_solver_factory.ConstructSolver(self.settings["linear_solver_settings"])
-
-    def _ConstructBuilderAndSolver(self, block_builder):
-
-        # Creating the builder and solver
-        if(self.settings["periodic_interface_conditions"].GetBool() == True):
-            builder_and_solver = KratosCFD.ResidualBasedBlockBuilderAndSolverPeriodic(self.linear_solver,KratosMultiphysics.PERIODIC_PAIR_INDEX)
-        else:
-            if(block_builder):
-                builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(self.linear_solver)
-            else:
-                builder_and_solver = KratosMultiphysics.ResidualBasedEliminationBuilderAndSolver(self.linear_solver)
-
-        return builder_and_solver
-
-    def _ConstructScheme(self, scheme_type, solution_type):
-
-        self.main_model_part.ProcessInfo.SetValue(KratosPoro.VELOCITY_COEFFICIENT, 1.0)
-        self.main_model_part.ProcessInfo.SetValue(KratosPoro.DT_PRESSURE_COEFFICIENT, 1.0)
-
-        if(scheme_type == "Newmark"):
-            beta = self.settings["newmark_beta"].GetDouble()
-            gamma = self.settings["newmark_gamma"].GetDouble()
-            theta = self.settings["newmark_theta"].GetDouble()
-            rayleigh_alpha = self.settings["rayleigh_alpha"].GetDouble()
-            rayleigh_beta = self.settings["rayleigh_beta"].GetDouble()
-            if self.settings["calculate_alpha_beta"].GetBool():
-                omega_1 = self.settings["omega_1"].GetDouble()
-                omega_n = self.settings["omega_n"].GetDouble()
-                xi_1 = self.settings["xi_1"].GetDouble()
-                xi_n = self.settings["xi_n"].GetDouble()
-                rayleigh_beta = 2.0*(xi_n*omega_n-xi_1*omega_1)/(omega_n*omega_n-omega_1*omega_1)
-                rayleigh_alpha = 2.0*xi_1*omega_1-rayleigh_beta*omega_1*omega_1
-                KratosMultiphysics.Logger.PrintInfo("::[UPwSolver]:: Scheme Information")
-                KratosMultiphysics.Logger.PrintInfo("::[UPwSolver]:: omega_1: ",omega_1)
-                KratosMultiphysics.Logger.PrintInfo("::[UPwSolver]:: omega_n: ",omega_n)
-                KratosMultiphysics.Logger.PrintInfo("::[UPwSolver]:: xi_1: ",xi_1)
-                KratosMultiphysics.Logger.PrintInfo("::[UPwSolver]:: xi_n: ",xi_n)
-                KratosMultiphysics.Logger.PrintInfo("::[UPwSolver]:: Alpha and Beta output")
-                KratosMultiphysics.Logger.PrintInfo("::[UPwSolver]:: rayleigh_alpha: ",rayleigh_alpha)
-                KratosMultiphysics.Logger.PrintInfo("::[UPwSolver]:: rayleigh_beta: ",rayleigh_beta)
-            
-            self.main_model_part.ProcessInfo.SetValue(KratosStructural.RAYLEIGH_ALPHA,rayleigh_alpha)
-            self.main_model_part.ProcessInfo.SetValue(KratosStructural.RAYLEIGH_BETA,rayleigh_beta)
-            if(solution_type == "implicit_quasi_static"):
-                if(rayleigh_alpha<1.0e-20 and rayleigh_beta<1.0e-20):
-                    scheme = KratosPoro.PoroNewmarkQuasistaticUPwScheme(beta,gamma,theta)
-                else:
-                    scheme = KratosPoro.PoroNewmarkQuasistaticDampedUPwScheme(beta,gamma,theta)
-            else:
-                scheme = KratosPoro.PoroNewmarkDynamicUPwScheme(beta,gamma,theta)
-        else:
-            raise Exception("Apart from Newmark, other scheme_type are not available.")
-
-        return scheme
-
-    def _ConstructConvergenceCriterion(self, convergence_criterion):
-
-        D_RT = self.settings["displacement_relative_tolerance"].GetDouble()
-        D_AT = self.settings["displacement_absolute_tolerance"].GetDouble()
-        R_RT = self.settings["residual_relative_tolerance"].GetDouble()
-        R_AT = self.settings["residual_absolute_tolerance"].GetDouble()
-        echo_level = self.settings["echo_level"].GetInt()
-
-        if(convergence_criterion == "Displacement_criterion"):
-            convergence_criterion = KratosMultiphysics.DisplacementCriteria(D_RT, D_AT)
-            convergence_criterion.SetEchoLevel(echo_level)
-        elif(convergence_criterion == "Residual_criterion"):
-            convergence_criterion = KratosMultiphysics.ResidualCriteria(R_RT, R_AT)
-            convergence_criterion.SetEchoLevel(echo_level)
-        elif(convergence_criterion == "And_criterion"):
-            Displacement = KratosMultiphysics.DisplacementCriteria(D_RT, D_AT)
-            Displacement.SetEchoLevel(echo_level)
-            Residual = KratosMultiphysics.ResidualCriteria(R_RT, R_AT)
-            Residual.SetEchoLevel(echo_level)
-            convergence_criterion = KratosMultiphysics.AndCriteria(Residual, Displacement)
-        elif(convergence_criterion == "Or_criterion"):
-            Displacement = KratosMultiphysics.DisplacementCriteria(D_RT, D_AT)
-            Displacement.SetEchoLevel(echo_level)
-            Residual = KratosMultiphysics.ResidualCriteria(R_RT, R_AT)
-            Residual.SetEchoLevel(echo_level)
-            convergence_criterion = KratosMultiphysics.OrCriteria(Residual, Displacement)
-
-        return convergence_criterion
-
-    def _ConstructSolver(self, builder_and_solver, strategy_type):
-
-        self.main_model_part.ProcessInfo.SetValue(KratosPoro.IS_CONVERGED, True)
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.NL_ITERATION_NUMBER, 1)
-
-        nonlocal_damage = self.settings["nonlocal_damage"].GetBool()
-        max_iters = self.settings["max_iteration"].GetInt()
-        compute_reactions = self.settings["compute_reactions"].GetBool()
-        reform_step_dofs = self.settings["reform_dofs_at_each_step"].GetBool()
-        move_mesh_flag = self.settings["move_mesh_flag"].GetBool()
-
-        self.strategy_params = KratosMultiphysics.Parameters("{}")
-        self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
-        self.strategy_params.AddValue("loads_variable_list",self.settings["loads_variable_list"])
-
-        if strategy_type == "newton_raphson":
-            if nonlocal_damage:
-                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
-                self.strategy_params.AddValue("characteristic_length",self.settings["characteristic_length"])
-                self.strategy_params.AddValue("search_neighbours_step",self.settings["search_neighbours_step"])
-                solving_strategy = KratosPoro.PoromechanicsNewtonRaphsonNonlocalStrategy(self.computing_model_part,
-                                                                               self.scheme,
-                                                                               self.convergence_criterion,
-                                                                               builder_and_solver,
-                                                                               self.strategy_params,
-                                                                               max_iters,
-                                                                               compute_reactions,
-                                                                               reform_step_dofs,
-                                                                               move_mesh_flag)
-            else:
-                solving_strategy = KratosPoro.PoromechanicsNewtonRaphsonStrategy(self.computing_model_part,
-                                                                       self.scheme,
-                                                                       self.convergence_criterion,
-                                                                       builder_and_solver,
-                                                                       self.strategy_params,
-                                                                       max_iters,
-                                                                       compute_reactions,
-                                                                       reform_step_dofs,
-                                                                       move_mesh_flag)
-        else:
-            # Arc-Length strategy
-            self.main_model_part.ProcessInfo.SetValue(KratosPoro.ARC_LENGTH_LAMBDA,1.0)
-            self.main_model_part.ProcessInfo.SetValue(KratosPoro.ARC_LENGTH_RADIUS_FACTOR,1.0)
-
-            self.strategy_params.AddValue("desired_iterations",self.settings["desired_iterations"])
-            self.strategy_params.AddValue("max_radius_factor",self.settings["max_radius_factor"])
-            self.strategy_params.AddValue("min_radius_factor",self.settings["min_radius_factor"])
-            if nonlocal_damage:
-                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
-                self.strategy_params.AddValue("characteristic_length",self.settings["characteristic_length"])
-                self.strategy_params.AddValue("search_neighbours_step",self.settings["search_neighbours_step"])
-                solving_strategy = KratosPoro.PoromechanicsRammArcLengthNonlocalStrategy(self.computing_model_part,
-                                                                               self.scheme,
-                                                                               self.convergence_criterion,
-                                                                               builder_and_solver,
-                                                                               self.strategy_params,
-                                                                               max_iters,
-                                                                               compute_reactions,
-                                                                               reform_step_dofs,
-                                                                               move_mesh_flag)
-            else:
-                solving_strategy = KratosPoro.PoromechanicsRammArcLengthStrategy(self.computing_model_part,
-                                                                       self.scheme,
-                                                                       self.convergence_criterion,
-                                                                       builder_and_solver,
-                                                                       self.strategy_params,
-                                                                       max_iters,
-                                                                       compute_reactions,
-                                                                       reform_step_dofs,
-                                                                       move_mesh_flag)
-
-        return solving_strategy
-
-    def _CheckConvergence(self):
-
-        IsConverged = self.solver.IsConverged()
-
-        return IsConverged
-
-    def _UpdateLoads(self):
-
-        self.solver.UpdateLoads()
-
-    def _CheckAndConstructGPtoNodalVariableExtrapolationProcess(self):
-        if self.settings["gp_to_nodal_variable_list"].size() > 0:
-            self.gp_to_nodal_variable = True
-            # Create extrapolation process
-            extrapolation_parameters = KratosMultiphysics.Parameters("""
-            {
-                "model_part_name"            : "",
-                "echo_level"                 : 0,
-                "average_variable"           : "NODAL_AREA",
-                "area_average"               : true,
-                "list_of_variables"          : [],
-                "extrapolate_non_historical" : false
-            }
-            """)
-            for i in range(self.settings["gp_to_nodal_variable_list"].size()):
-                var_name = self.settings["gp_to_nodal_variable_list"][i].GetString()
-                extrapolation_parameters["list_of_variables"].Append(var_name)
-            extrapolation_parameters["model_part_name"].SetString(self.settings["model_part_name"].GetString())
-            extrapolation_parameters["extrapolate_non_historical"].SetBool(self.settings["gp_to_nodal_variable_extrapolate_non_historical"].GetBool())
-            self.integration_values_extrapolation_to_nodes_process = KratosMultiphysics.IntegrationValuesExtrapolationToNodesProcess(self.main_model_part, extrapolation_parameters)
-        else:
-            self.gp_to_nodal_variable = False
+# Importing the Kratos Library
+import KratosMultiphysics
+from KratosMultiphysics.python_solver import PythonSolver
+
+# Import applications
+import KratosMultiphysics.FluidDynamicsApplication as KratosCFD
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+
+def CreateSolver(model, custom_settings):
+    return UPlSolver(model, custom_settings)
+
+class UPlSolver(PythonSolver):
+    '''Solver for the solution of displacement-pore pressure coupled problems
+    for one-phase flow in porous media.'''
+
+    def __init__(self, model, custom_settings):
+
+        super(UPlSolver,self).__init__(model, custom_settings)
+
+        self.min_buffer_size = 2
+
+        # Either retrieve the model part from the model or create a new one
+        model_part_name = self.settings["model_part_name"].GetString()
+
+        if model_part_name == "":
+            raise Exception('Please specify a model_part name!')
+
+        if self.model.HasModelPart(model_part_name):
+            self.main_model_part = self.model.GetModelPart(model_part_name)
+        else:
+            self.main_model_part = self.model.CreateModelPart(model_part_name,self.min_buffer_size)
+
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE,
+                                                  self.settings["domain_size"].GetInt())
+
+        KratosMultiphysics.Logger.PrintInfo("UPlSolver", "Construction of UPlSolver finished.")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        this_defaults = KratosMultiphysics.Parameters("""{
+            "solver_type": "poromechanics_U_Pl_solver",
+            "model_part_name": "PorousModelPart",
+            "domain_size": 2,
+            "start_time": 0.0,
+            "time_step": 0.1,
+            "model_import_settings":{
+                "input_type": "mdpa",
+                "input_filename": "unknown_name"
+            },
+            "material_import_settings" :{
+                "materials_filename": ""
+            },
+            "buffer_size": 2,
+            "echo_level": 0,
+            "reform_dofs_at_each_step": false,
+            "clear_storage": false,
+            "compute_reactions": false,
+            "move_mesh_flag": false,
+            "nodal_smoothing": false,
+            "gp_to_nodal_variable_list": [],
+            "gp_to_nodal_variable_extrapolate_non_historical": false,
+            "periodic_interface_conditions": false,
+            "solution_type": "implicit_quasi_static",
+            "scheme_type": "Newmark",
+            "newmark_beta": 0.25,
+            "newmark_gamma": 0.5,
+            "newmark_theta_u": 0.5,
+            "newmark_theta_p": 0.5,
+            "calculate_alpha_beta"       : false,
+            "omega_1"                    : 1.0,
+            "omega_n"                    : 10.0,
+            "xi_1"                       : 1.0,
+            "xi_n"                       : 0.05,
+            "rayleigh_alpha": 0.0,
+            "rayleigh_beta": 0.0,
+            "strategy_type": "newton_raphson",
+            "convergence_criterion": "Displacement_criterion",
+            "displacement_relative_tolerance": 1.0e-4,
+            "displacement_absolute_tolerance": 1.0e-9,
+            "residual_relative_tolerance": 1.0e-4,
+            "residual_absolute_tolerance": 1.0e-9,
+            "max_iteration": 15,
+            "desired_iterations": 4,
+            "max_radius_factor": 20.0,
+            "min_radius_factor": 0.5,
+            "block_builder": true,
+            "nonlocal_damage": false,
+            "characteristic_length": 0.05,
+            "search_neighbours_step": false,
+            "linear_solver_settings":{
+                "solver_type": "amgcl",
+                "tolerance": 1.0e-6,
+                "max_iteration": 100,
+                "scaling": false,
+                "verbosity": 0,
+                "preconditioner_type": "ilu0",
+                "smoother_type": "ilu0",
+                "krylov_type": "gmres",
+                "coarsening_type": "aggregation"
+            },
+            "problem_domain_sub_model_part_list": [""],
+            "processes_sub_model_part_list": [""],
+            "body_domain_sub_model_part_list": [""],
+            "loads_sub_model_part_list": [],
+            "loads_variable_list": []
+        }""")
+
+        this_defaults.AddMissingParameters(super(UPlSolver, cls).GetDefaultParameters())
+        return this_defaults
+
+    def AddVariables(self):
+
+        ## Solid Variables
+        # Add displacements
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
+        # Add reactions for the displacements
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
+        # Add dynamic variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
+        # Add variables for the solid conditions
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FORCE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FACE_LOAD)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NORMAL_CONTACT_STRESS)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.TANGENTIAL_CONTACT_STRESS)
+        ## Fluid Variables
+        # Add liquid pressure
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.LIQUID_PRESSURE)
+        # Add reactions for the liquid pressure
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.REACTION_LIQUID_PRESSURE)
+        # Add dynamic variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.DT_LIQUID_PRESSURE)
+        # Add variables for the liquid conditions
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NORMAL_LIQUID_FLUX)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.LIQUID_DISCHARGE)
+        ## Other variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VOLUME_ACCELERATION)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PERIODIC_PAIR_INDEX)
+
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_AREA)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_WIDTH)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_DAMAGE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_AREA)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_EFFECTIVE_STRESS_TENSOR)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.INITIAL_STRESS_TENSOR)
+
+        # Add variables from gp to nodal variable list
+        if self.settings["gp_to_nodal_variable_extrapolate_non_historical"].GetBool()==False:
+            for i in range(self.settings["gp_to_nodal_variable_list"].size()):
+                variable_name = self.settings["gp_to_nodal_variable_list"][i].GetString()
+                variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name)
+                self.main_model_part.AddNodalSolutionStepVariable(variable)
+
+        KratosMultiphysics.Logger.PrintInfo("UPlSolver", "Variables added correctly.")
+
+    def ImportModelPart(self):
+        # we can use the default implementation in the base class
+        self._ImportModelPart(self.main_model_part,self.settings["model_import_settings"])
+
+    def PrepareModelPart(self):
+
+        # Set ProcessInfo variables
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME,
+                                                  self.settings["start_time"].GetDouble())
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME,
+                                                  self.settings["time_step"].GetDouble())
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.STEP, 0)
+        self.main_model_part.ProcessInfo.SetValue(KratosPoro.TIME_UNIT_CONVERTER, 1.0)
+        if(self.settings["nodal_smoothing"].GetBool() == True):
+            self.main_model_part.ProcessInfo.SetValue(KratosPoro.NODAL_SMOOTHING, True)
+        else:
+            self.main_model_part.ProcessInfo.SetValue(KratosPoro.NODAL_SMOOTHING, False)
+
+        if not self.main_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
+            ## Executes the check and prepare model process (Create computing_model_part and set constitutive law)
+            self._ExecuteCheckAndPrepare()
+            ## Set buffer size
+            self._SetBufferSize()
+
+        KratosMultiphysics.Logger.PrintInfo("UPlSolver", "Model reading finished.")
+
+    def AddDofs(self):
+        ## Solid dofs
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_X, KratosMultiphysics.REACTION_X,self.main_model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Y, KratosMultiphysics.REACTION_Y,self.main_model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Z, KratosMultiphysics.REACTION_Z,self.main_model_part)
+        ## Liquid dofs
+        KratosMultiphysics.VariableUtils().AddDof(KratosPoro.LIQUID_PRESSURE, KratosPoro.REACTION_LIQUID_PRESSURE,self.main_model_part)
+
+        if(self.settings["solution_type"].GetString() == "implicit_dynamic"):
+            for node in self.main_model_part.Nodes:
+                # adding VELOCITY as dofs
+                node.AddDof(KratosMultiphysics.VELOCITY_X)
+                node.AddDof(KratosMultiphysics.VELOCITY_Y)
+                node.AddDof(KratosMultiphysics.VELOCITY_Z)
+                # adding ACCELERATION as dofs
+                node.AddDof(KratosMultiphysics.ACCELERATION_X)
+                node.AddDof(KratosMultiphysics.ACCELERATION_Y)
+                node.AddDof(KratosMultiphysics.ACCELERATION_Z)
+
+        KratosMultiphysics.Logger.PrintInfo("UPlSolver", "DOFs added correctly.")
+
+    def GetMinimumBufferSize(self):
+        return self.min_buffer_size
+
+    def Initialize(self):
+        self.computing_model_part = self.GetComputingModelPart()
+
+        # Fill the previous steps of the buffer with the initial conditions
+        self._FillBuffer()
+
+        # Construct the linear solver
+        self.linear_solver = self._ConstructLinearSolver()
+
+        # Builder and solver creation
+        builder_and_solver = self._ConstructBuilderAndSolver(self.settings["block_builder"].GetBool())
+
+        # Solution scheme creation
+        self.scheme = self._ConstructScheme(self.settings["scheme_type"].GetString(),
+                                         self.settings["solution_type"].GetString())
+
+        # Get the convergence criterion
+        self.convergence_criterion = self._ConstructConvergenceCriterion(self.settings["convergence_criterion"].GetString())
+
+        # Solver creation
+        self.solver = self._ConstructSolver(builder_and_solver,
+                                            self.settings["strategy_type"].GetString())
+
+        # Set echo_level
+        self.SetEchoLevel(self.settings["echo_level"].GetInt())
+
+        # Initialize Strategy
+        if self.settings["clear_storage"].GetBool():
+            self.Clear()
+
+        self.solver.Initialize()
+
+        # Check if everything is assigned correctly
+        self.Check()
+
+        # Check and construct gp_to_nodal_variable process
+        self._CheckAndConstructGPtoNodalVariableExtrapolationProcess()
+
+        KratosMultiphysics.Logger.PrintInfo("UPlSolver", "Solver initialization finished.")
+
+    def GetComputingModelPart(self):
+        return self.main_model_part.GetSubModelPart(self.computing_model_part_name)
+
+    def ComputeDeltaTime(self):
+        return self.main_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
+
+    def Clear(self):
+        self.solver.Clear()
+
+    def Check(self):
+        self.solver.Check()
+
+    def SetEchoLevel(self, level):
+        self.solver.SetEchoLevel(level)
+
+    def AdvanceInTime(self, current_time):
+        dt = self.ComputeDeltaTime()
+        new_time = current_time + dt
+
+        self.main_model_part.CloneTimeStep(new_time)
+        self.main_model_part.ProcessInfo[KratosMultiphysics.STEP] += 1
+
+        return new_time
+
+    def InitializeSolutionStep(self):
+        self.solver.InitializeSolutionStep()
+
+    def Predict(self):
+        self.solver.Predict()
+
+    def SolveSolutionStep(self):
+        is_converged = self.solver.SolveSolutionStep()
+        return is_converged
+
+    def FinalizeSolutionStep(self):
+        self.solver.FinalizeSolutionStep()
+
+        if self.gp_to_nodal_variable:
+            self.integration_values_extrapolation_to_nodes_process.ExecuteBeforeSolutionLoop()
+            self.integration_values_extrapolation_to_nodes_process.ExecuteFinalizeSolutionStep()
+
+    def Finalize(self):
+        if self.gp_to_nodal_variable:
+            self.integration_values_extrapolation_to_nodes_process.ExecuteFinalize()
+
+    def Solve(self):
+        message = "".join([
+            "Calling UPlSolver.Solve() method, which is deprecated\n",
+            "Please call the individual methods instead:\n",
+            "solver.InitializeSolutionStep()\n",
+            "solver.Predict()\n",
+            "solver.SolveSolutionStep()\n",
+            "solver.FinalizeSolutionStep()\n"]
+        )
+        KratosMultiphysics.Logger.PrintWarning("UPlSolver",message)
+
+        if self.settings["clear_storage"].GetBool():
+            self.Clear()
+
+        self.InitializeSolutionStep()
+        self.Predict()
+        self.SolveSolutionStep()
+        self.FinalizeSolutionStep()
+
+    #### Specific internal functions ####
+
+    def _ExecuteCheckAndPrepare(self):
+
+        self.computing_model_part_name = "porous_computational_model_part"
+
+        # Create list of sub sub model parts (it is a copy of the standard lists with a different name)
+        import json
+
+        self.body_domain_sub_sub_model_part_list = []
+        for i in range(self.settings["body_domain_sub_model_part_list"].size()):
+            self.body_domain_sub_sub_model_part_list.append("sub_"+self.settings["body_domain_sub_model_part_list"][i].GetString())
+        self.body_domain_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.body_domain_sub_sub_model_part_list))
+
+        self.loads_sub_sub_model_part_list = []
+        for i in range(self.settings["loads_sub_model_part_list"].size()):
+            self.loads_sub_sub_model_part_list.append("sub_"+self.settings["loads_sub_model_part_list"][i].GetString())
+        self.loads_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.loads_sub_sub_model_part_list))
+
+        # Auxiliary parameters object for the CheckAndPepareModelProcess
+        params = KratosMultiphysics.Parameters("{}")
+        params.AddEmptyValue("computing_model_part_name").SetString(self.computing_model_part_name)
+        params.AddValue("problem_domain_sub_model_part_list",self.settings["problem_domain_sub_model_part_list"])
+        params.AddValue("processes_sub_model_part_list",self.settings["processes_sub_model_part_list"])
+        params.AddValue("body_domain_sub_model_part_list",self.settings["body_domain_sub_model_part_list"])
+        params.AddValue("body_domain_sub_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
+        params.AddValue("loads_sub_model_part_list",self.settings["loads_sub_model_part_list"])
+        params.AddValue("loads_sub_sub_model_part_list",self.loads_sub_sub_model_part_list)
+        # CheckAndPrepareModelProcess creates the porous_computational_model_part
+        from KratosMultiphysics.PoromechanicsApplication import check_and_prepare_model_process_poro
+        check_and_prepare_model_process_poro.CheckAndPrepareModelProcess(self.main_model_part, params).Execute()
+
+        # Constitutive law import
+        materials_imported = self.import_constitutive_laws()
+        if materials_imported:
+            KratosMultiphysics.Logger.PrintInfo("UPlSolver", "Constitutive law was successfully imported via json.")
+        else:
+            KratosMultiphysics.Logger.PrintInfo("UPlSolver", "Constitutive law was not successfully imported.")
+
+    def import_constitutive_laws(self):
+        materials_filename = self.settings["material_import_settings"]["materials_filename"].GetString()
+        if (materials_filename != ""):
+            # Add constitutive laws and material properties from json file to model parts.
+            material_settings = KratosMultiphysics.Parameters("""{"Parameters": {"materials_filename": ""}} """)
+            material_settings["Parameters"]["materials_filename"].SetString(materials_filename)
+            KratosMultiphysics.ReadMaterialsUtility(material_settings, self.model)
+            materials_imported = True
+        else:
+            materials_imported = False
+        return materials_imported
+
+    def _SetBufferSize(self):
+        required_buffer_size = self.settings["buffer_size"].GetInt()
+        if required_buffer_size < self.GetMinimumBufferSize():
+            required_buffer_size = self.GetMinimumBufferSize()
+        current_buffer_size = self.main_model_part.GetBufferSize()
+        buffer_size = max(current_buffer_size, required_buffer_size)
+        self.main_model_part.SetBufferSize(buffer_size)
+
+    def _FillBuffer(self):
+        buffer_size = self.main_model_part.GetBufferSize()
+        time = self.main_model_part.ProcessInfo[KratosMultiphysics.TIME]
+        delta_time = self.main_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
+        step = self.main_model_part.ProcessInfo[KratosMultiphysics.STEP]
+
+        step = step - (buffer_size-1)*1
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.STEP, step)
+        time = time - (buffer_size-1)*delta_time
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, time)
+        for i in range(buffer_size-1):
+            step = step + 1
+            self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.STEP, step)
+            time = time + delta_time
+            self.main_model_part.CloneTimeStep(time)
+
+    def _ConstructLinearSolver(self):
+        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
+        return linear_solver_factory.ConstructSolver(self.settings["linear_solver_settings"])
+
+    def _ConstructBuilderAndSolver(self, block_builder):
+
+        # Creating the builder and solver
+        if(self.settings["periodic_interface_conditions"].GetBool() == True):
+            builder_and_solver = KratosCFD.ResidualBasedBlockBuilderAndSolverPeriodic(self.linear_solver,KratosMultiphysics.PERIODIC_PAIR_INDEX)
+        else:
+            if(block_builder):
+                builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(self.linear_solver)
+            else:
+                builder_and_solver = KratosMultiphysics.ResidualBasedEliminationBuilderAndSolver(self.linear_solver)
+
+        return builder_and_solver
+
+    def _ConstructScheme(self, scheme_type, solution_type):
+
+        self.main_model_part.ProcessInfo.SetValue(KratosPoro.VELOCITY_COEFFICIENT, 1.0)
+        self.main_model_part.ProcessInfo.SetValue(KratosPoro.DT_LIQUID_PRESSURE_COEFFICIENT, 1.0)
+
+        if(scheme_type == "Newmark"):
+            beta = self.settings["newmark_beta"].GetDouble()
+            gamma = self.settings["newmark_gamma"].GetDouble()
+            theta_u = self.settings["newmark_theta_u"].GetDouble()
+            theta_p = self.settings["newmark_theta_p"].GetDouble()
+            rayleigh_alpha = self.settings["rayleigh_alpha"].GetDouble()
+            rayleigh_beta = self.settings["rayleigh_beta"].GetDouble()
+            if self.settings["calculate_alpha_beta"].GetBool():
+                omega_1 = self.settings["omega_1"].GetDouble()
+                omega_n = self.settings["omega_n"].GetDouble()
+                xi_1 = self.settings["xi_1"].GetDouble()
+                xi_n = self.settings["xi_n"].GetDouble()
+                rayleigh_beta = 2.0*(xi_n*omega_n-xi_1*omega_1)/(omega_n*omega_n-omega_1*omega_1)
+                rayleigh_alpha = 2.0*xi_1*omega_1-rayleigh_beta*omega_1*omega_1
+                KratosMultiphysics.Logger.PrintInfo("::[UPlSolver]:: Scheme Information")
+                KratosMultiphysics.Logger.PrintInfo("::[UPlSolver]:: omega_1: ",omega_1)
+                KratosMultiphysics.Logger.PrintInfo("::[UPlSolver]:: omega_n: ",omega_n)
+                KratosMultiphysics.Logger.PrintInfo("::[UPlSolver]:: xi_1: ",xi_1)
+                KratosMultiphysics.Logger.PrintInfo("::[UPlSolver]:: xi_n: ",xi_n)
+                KratosMultiphysics.Logger.PrintInfo("::[UPlSolver]:: Alpha and Beta output")
+                KratosMultiphysics.Logger.PrintInfo("::[UPlSolver]:: rayleigh_alpha: ",rayleigh_alpha)
+                KratosMultiphysics.Logger.PrintInfo("::[UPlSolver]:: rayleigh_beta: ",rayleigh_beta)
+            
+            self.main_model_part.ProcessInfo.SetValue(KratosStructural.RAYLEIGH_ALPHA,rayleigh_alpha)
+            self.main_model_part.ProcessInfo.SetValue(KratosStructural.RAYLEIGH_BETA,rayleigh_beta)
+            if(solution_type == "implicit_quasi_static"):
+                if(rayleigh_alpha<1.0e-20 and rayleigh_beta<1.0e-20):
+                    scheme = KratosPoro.PoroNewmarkQuasistaticUPlScheme(theta_u,theta_p,beta,gamma)
+                else:
+                    scheme = KratosPoro.PoroNewmarkQuasistaticDampedUPlScheme(theta_u,theta_p,beta,gamma)
+            else:
+                scheme = KratosPoro.PoroNewmarkDynamicUPlScheme(theta_u,theta_p,beta,gamma)
+        else:
+            raise Exception("Apart from Newmark, other scheme_type are not available.")
+
+        return scheme
+
+    def _ConstructConvergenceCriterion(self, convergence_criterion):
+
+        D_RT = self.settings["displacement_relative_tolerance"].GetDouble()
+        D_AT = self.settings["displacement_absolute_tolerance"].GetDouble()
+        R_RT = self.settings["residual_relative_tolerance"].GetDouble()
+        R_AT = self.settings["residual_absolute_tolerance"].GetDouble()
+        echo_level = self.settings["echo_level"].GetInt()
+
+        if(convergence_criterion == "Displacement_criterion"):
+            convergence_criterion = KratosMultiphysics.DisplacementCriteria(D_RT, D_AT)
+            convergence_criterion.SetEchoLevel(echo_level)
+        elif(convergence_criterion == "Residual_criterion"):
+            convergence_criterion = KratosMultiphysics.ResidualCriteria(R_RT, R_AT)
+            convergence_criterion.SetEchoLevel(echo_level)
+        elif(convergence_criterion == "And_criterion"):
+            Displacement = KratosMultiphysics.DisplacementCriteria(D_RT, D_AT)
+            Displacement.SetEchoLevel(echo_level)
+            Residual = KratosMultiphysics.ResidualCriteria(R_RT, R_AT)
+            Residual.SetEchoLevel(echo_level)
+            convergence_criterion = KratosMultiphysics.AndCriteria(Residual, Displacement)
+        elif(convergence_criterion == "Or_criterion"):
+            Displacement = KratosMultiphysics.DisplacementCriteria(D_RT, D_AT)
+            Displacement.SetEchoLevel(echo_level)
+            Residual = KratosMultiphysics.ResidualCriteria(R_RT, R_AT)
+            Residual.SetEchoLevel(echo_level)
+            convergence_criterion = KratosMultiphysics.OrCriteria(Residual, Displacement)
+
+        return convergence_criterion
+
+    def _ConstructSolver(self, builder_and_solver, strategy_type):
+
+        self.main_model_part.ProcessInfo.SetValue(KratosPoro.IS_CONVERGED, True)
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.NL_ITERATION_NUMBER, 1)
+
+        nonlocal_damage = self.settings["nonlocal_damage"].GetBool()
+        max_iters = self.settings["max_iteration"].GetInt()
+        compute_reactions = self.settings["compute_reactions"].GetBool()
+        reform_step_dofs = self.settings["reform_dofs_at_each_step"].GetBool()
+        move_mesh_flag = self.settings["move_mesh_flag"].GetBool()
+
+        self.strategy_params = KratosMultiphysics.Parameters("{}")
+        self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
+        self.strategy_params.AddValue("loads_variable_list",self.settings["loads_variable_list"])
+
+        if strategy_type == "newton_raphson":
+            if nonlocal_damage:
+                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
+                self.strategy_params.AddValue("characteristic_length",self.settings["characteristic_length"])
+                self.strategy_params.AddValue("search_neighbours_step",self.settings["search_neighbours_step"])
+                solving_strategy = KratosPoro.PoromechanicsNewtonRaphsonNonlocalStrategy(self.computing_model_part,
+                                                                               self.scheme,
+                                                                               self.convergence_criterion,
+                                                                               builder_and_solver,
+                                                                               self.strategy_params,
+                                                                               max_iters,
+                                                                               compute_reactions,
+                                                                               reform_step_dofs,
+                                                                               move_mesh_flag)
+            else:
+                solving_strategy = KratosPoro.PoromechanicsNewtonRaphsonStrategy(self.computing_model_part,
+                                                                       self.scheme,
+                                                                       self.convergence_criterion,
+                                                                       builder_and_solver,
+                                                                       self.strategy_params,
+                                                                       max_iters,
+                                                                       compute_reactions,
+                                                                       reform_step_dofs,
+                                                                       move_mesh_flag)
+        else:
+            # Arc-Length strategy
+            self.main_model_part.ProcessInfo.SetValue(KratosPoro.ARC_LENGTH_LAMBDA,1.0)
+            self.main_model_part.ProcessInfo.SetValue(KratosPoro.ARC_LENGTH_RADIUS_FACTOR,1.0)
+
+            self.strategy_params.AddValue("desired_iterations",self.settings["desired_iterations"])
+            self.strategy_params.AddValue("max_radius_factor",self.settings["max_radius_factor"])
+            self.strategy_params.AddValue("min_radius_factor",self.settings["min_radius_factor"])
+            if nonlocal_damage:
+                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
+                self.strategy_params.AddValue("characteristic_length",self.settings["characteristic_length"])
+                self.strategy_params.AddValue("search_neighbours_step",self.settings["search_neighbours_step"])
+                solving_strategy = KratosPoro.PoromechanicsRammArcLengthNonlocalStrategy(self.computing_model_part,
+                                                                               self.scheme,
+                                                                               self.convergence_criterion,
+                                                                               builder_and_solver,
+                                                                               self.strategy_params,
+                                                                               max_iters,
+                                                                               compute_reactions,
+                                                                               reform_step_dofs,
+                                                                               move_mesh_flag)
+            else:
+                solving_strategy = KratosPoro.PoromechanicsRammArcLengthStrategy(self.computing_model_part,
+                                                                       self.scheme,
+                                                                       self.convergence_criterion,
+                                                                       builder_and_solver,
+                                                                       self.strategy_params,
+                                                                       max_iters,
+                                                                       compute_reactions,
+                                                                       reform_step_dofs,
+                                                                       move_mesh_flag)
+
+        return solving_strategy
+
+    def _CheckConvergence(self):
+
+        IsConverged = self.solver.IsConverged()
+
+        return IsConverged
+
+    def _UpdateLoads(self):
+
+        self.solver.UpdateLoads()
+
+    def _CheckAndConstructGPtoNodalVariableExtrapolationProcess(self):
+        if self.settings["gp_to_nodal_variable_list"].size() > 0:
+            self.gp_to_nodal_variable = True
+            # Create extrapolation process
+            extrapolation_parameters = KratosMultiphysics.Parameters("""
+            {
+                "model_part_name"            : "",
+                "echo_level"                 : 0,
+                "average_variable"           : "NODAL_AREA",
+                "area_average"               : true,
+                "list_of_variables"          : [],
+                "extrapolate_non_historical" : false
+            }
+            """)
+            for i in range(self.settings["gp_to_nodal_variable_list"].size()):
+                var_name = self.settings["gp_to_nodal_variable_list"][i].GetString()
+                extrapolation_parameters["list_of_variables"].Append(var_name)
+            extrapolation_parameters["model_part_name"].SetString(self.settings["model_part_name"].GetString())
+            extrapolation_parameters["extrapolate_non_historical"].SetBool(self.settings["gp_to_nodal_variable_extrapolate_non_historical"].GetBool())
+            self.integration_values_extrapolation_to_nodes_process = KratosMultiphysics.IntegrationValuesExtrapolationToNodesProcess(self.main_model_part, extrapolation_parameters)
+        else:
+            self.gp_to_nodal_variable = False
             self.integration_values_extrapolation_to_nodes_process = KratosMultiphysics.Process()
```

## Comparing `KratosPoromechanicsApplication-9.4.6.dist-info/METADATA` & `KratosPoromechanicsApplication-9.5.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-Metadata-Version: 2.1
-Name: KratosPoromechanicsApplication
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
-
-## Poromechanics Application
-
-The Poromechanics Application contains developments in coupled solid-pore fluid interaction problems within Kratos Multiphysics.
-
-### Features:
-
-- UPw small displacement element for saturated porous media (with
-equal order interpolation, unstable under incompressible-undrained
-conditions)
-
-- Stable UPw small displacement element for saturated porous media
-(with higher order interpolation for displacements)
-
-- FIC-Stabilized UPw small displacement element for saturated porous media
-(with equal order interpolation for displacements)
-
-- UPw Quasi-zero-thickness interface elements for defining cracks and
-joints
-
-- Local linear elastic damage model (Simo-Ju and modified Von Mises)
-
-- Non-local linear elastic damage model (Simo-Ju and modified Von
-Mises)
-
-- Bilinear cohesive fracture model (for quasi-zero-thickness interface elements)
-
-- Fracture propagation utility based on the combination of the
-damage model with the insertion of interface elements after remeshing
-with GiD
-
-
+Metadata-Version: 2.1
+Name: KratosPoromechanicsApplication
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
+
+## Poromechanics Application
+
+The Poromechanics Application contains developments in coupled solid-pore fluid interaction problems within Kratos Multiphysics.
+
+### Features:
+
+- UPl small displacement element for saturated porous media (with
+equal order interpolation, unstable under incompressible-undrained
+conditions)
+
+- Stable UPl small displacement element for saturated porous media
+(with higher order interpolation for displacements)
+
+- FIC-Stabilized UPl small displacement element for saturated porous media
+(with equal order interpolation for displacements)
+
+- UPl Quasi-zero-thickness interface elements for defining cracks and
+joints
+
+- Local linear elastic damage model (Simo-Ju and modified Von Mises)
+
+- Non-local linear elastic damage model (Simo-Ju and modified Von
+Mises)
+
+- Bilinear cohesive fracture model (for quasi-zero-thickness interface elements)
+
+- Fracture propagation utility based on the combination of the
+damage model with the insertion of interface elements after remeshing
+with GiD
+
+
```

## Comparing `KratosPoromechanicsApplication-9.4.6.dist-info/RECORD` & `KratosPoromechanicsApplication-9.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-KratosMultiphysics/.libs/KratosPoromechanicsApplication.pyd,sha256=LvHWQFaCFyXMQQnW5rMbQpiqIzUcu5iuKs9ru4y0l4U,1818624
-KratosMultiphysics/.libs/KratosPoromechanicsCore.dll,sha256=cbhJRSPJyXwcnhI0XaZtCV7w7utPcUeqLGJw_8utwiA,3814912
-KratosMultiphysics/.libs/KratosPoromechanicsCore.lib,sha256=4bfUnTWuNL0PJcwRO-SdbNP0k8bGi9M_HQOymUsUzCA,1697748
-KratosMultiphysics/PoromechanicsApplication/__init__.py,sha256=ntdM3m0WXHQ5aTjWx0zLRVidlw1ivh7Vgmy8w54eQTw,292
-KratosMultiphysics/PoromechanicsApplication/apply_normal_load_table_process.py,sha256=Tkuqnq3lBDi5NKaDt8--gJ6fqfsWBtp7KPc2VJxx994,3440
-KratosMultiphysics/PoromechanicsApplication/apply_scalar_constraint_table_process.py,sha256=W49QOrH_5lYLyxkIOxTQAlPjNyDdOJB1BA7cdX_lp9I,2780
-KratosMultiphysics/PoromechanicsApplication/apply_vector_constraint_table_process.py,sha256=6361O6OACWW5SO6kGKzUOwtfIMMaoB0sZ5NWDqrJWmg,3703
-KratosMultiphysics/PoromechanicsApplication/check_and_prepare_model_process_poro.py,sha256=zHARQ2IEyo8SMAqzHYnZx2U91jSYLSVQuidM1bjjfw4,4558
-KratosMultiphysics/PoromechanicsApplication/periodic_interface_activation_process.py,sha256=DkRWwFLWaTehUhRyPHnconi4pQsdwbdlNCJ7vKDFDuE,1520
-KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pw_explicit_dynamic_solver.py,sha256=WbFjAvQDYu3VmaTjVqqbbJqQkoPT04PPfp8fkrKM4ek,11791
-KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pw_solver.py,sha256=vZYADYypAsRrV0GxVYeY7OPd-0gFM5-xifSPNu60eNs,31444
-KratosMultiphysics/PoromechanicsApplication/poromechanics_analysis.py,sha256=oB2fAmrImqwalAy8YJvxl9VBGTT8qwP3DApicor4dLw,5631
-KratosMultiphysics/PoromechanicsApplication/poromechanics_cleaning_utility.py,sha256=XCg2c8LBVfqKWouoBr06V4RGiVfd_aa_BtOy2TmHEdM,651
-KratosMultiphysics/PoromechanicsApplication/poromechanics_face_load_control_module_process.py,sha256=isOifaXajCQ2kz9itwM_5jUA2L_aBvEjaXycF0SL9Nk,3388
-KratosMultiphysics/PoromechanicsApplication/poromechanics_fracture_propagation_utility.py,sha256=r5tOokrD26AMQpKJ59AVQ8SoyRKl4CANhzpAKn7iO9I,16333
-KratosMultiphysics/PoromechanicsApplication/poromechanics_initial_stress_utility.py,sha256=BRgfI-mzhOeE4rdZC8h_hZPnVfAKY3LWptXm47FMMxs,2906
-KratosPoromechanicsApplication-9.4.6.dist-info/METADATA,sha256=ErXsaKEorMPS3g-cndxbKi7fTFt8nW_HMZYO1XfOEEU,2493
-KratosPoromechanicsApplication-9.4.6.dist-info/WHEEL,sha256=GZFS91_ufm4WrNPBaFVPB9MvOXR6bMZQhPcZRRTN5YM,100
-KratosPoromechanicsApplication-9.4.6.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
-KratosPoromechanicsApplication-9.4.6.dist-info/RECORD,,
+KratosPoromechanicsApplication.libs/libKratosPoromechanicsCore-2e59df2b.so,sha256=XJq4jVLDKEFRcsofb3O27CO727oEDv4dPAJFIkD5cVw,18688153
+KratosMultiphysics/PoromechanicsApplication/poromechanics_cleaning_utility.py,sha256=ZvNLuXgJwbX16zabOSYfc1idcQCf9HVjr_mDEhmE4mk,629
+KratosMultiphysics/PoromechanicsApplication/apply_scalar_constraint_table_process.py,sha256=W49QOrH_5lYLyxkIOxTQAlPjNyDdOJB1BA7cdX_lp9I,2780
+KratosMultiphysics/PoromechanicsApplication/poromechanics_analysis.py,sha256=kuPpwCN-i4CfzX0D-Bk1ni6ePJSpulOOKHiTxySu6m8,5514
+KratosMultiphysics/PoromechanicsApplication/poromechanics_face_load_control_module_process.py,sha256=isOifaXajCQ2kz9itwM_5jUA2L_aBvEjaXycF0SL9Nk,3388
+KratosMultiphysics/PoromechanicsApplication/check_and_prepare_model_process_poro.py,sha256=d4KIUPr9o32WtvoTG0594SvVo8lDDvxshC7vDEZ0C7g,4480
+KratosMultiphysics/PoromechanicsApplication/poromechanics_fracture_propagation_utility.py,sha256=r5tOokrD26AMQpKJ59AVQ8SoyRKl4CANhzpAKn7iO9I,16333
+KratosMultiphysics/PoromechanicsApplication/apply_vector_constraint_table_process.py,sha256=6361O6OACWW5SO6kGKzUOwtfIMMaoB0sZ5NWDqrJWmg,3703
+KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pl_solver.py,sha256=k_cWaCTU8qneIwxjlKT_hN9FCYCro5mx5uEVqqEElus,30765
+KratosMultiphysics/PoromechanicsApplication/poromechanics_U_Pl_explicit_dynamic_solver.py,sha256=jRSc9hE6TtuOLGfkCo-keQlLW-5gTyJv10S54QHxRVI,11681
+KratosMultiphysics/PoromechanicsApplication/apply_normal_load_table_process.py,sha256=Tkuqnq3lBDi5NKaDt8--gJ6fqfsWBtp7KPc2VJxx994,3440
+KratosMultiphysics/PoromechanicsApplication/__init__.py,sha256=Hq4qYqU-mg_8UxAlkA-ZW2vAElTDlMnWGMfUMTosoHI,285
+KratosMultiphysics/PoromechanicsApplication/periodic_interface_activation_process.py,sha256=Pzxp8pkRmkTf_d616RZ5JCy3ECo59C7u-sY5mSK23Qs,1483
+KratosMultiphysics/PoromechanicsApplication/poromechanics_initial_stress_utility.py,sha256=h0xg2Ao-Z-vxhaV2PTT8N7f5-DceKE0L4cMIFOyWHRk,2845
+KratosMultiphysics/.libs/libKratosPoromechanicsCore.so,sha256=In4Nd7ZB8ljp7VAX5jbHx4Q_f1WlDUdGG15VhFDFYfM,17988393
+KratosMultiphysics/.libs/KratosPoromechanicsApplication.cpython-39-x86_64-linux-gnu.so,sha256=Kqv26lOuZcQxyaNaoUjUoz1JdmJJNEXa6UkmsoUv_NU,4593257
+KratosPoromechanicsApplication-9.5.dist-info/METADATA,sha256=66Ry6XGnFN3_4Kbnd55cNW6fni9_veJz2jSJFjR9a_E,2427
+KratosPoromechanicsApplication-9.5.dist-info/WHEEL,sha256=rY0Y6THYM7EImsHfF-zs67o8pQciAsMw9_YuSvftjrQ,148
+KratosPoromechanicsApplication-9.5.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
+KratosPoromechanicsApplication-9.5.dist-info/RECORD,,
```

