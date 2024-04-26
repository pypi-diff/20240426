# Comparing `tmp/KratosDamApplication-9.4.6-cp39-cp39-win_amd64.whl.zip` & `tmp/KratosDamApplication-9.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,1351 +1,1861 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   1311454 (00000000001402DEh)
-  Actual end-cent-dir record offset:       1311432 (00000000001402C8h)
-  Expected end-cent-dir record offset:     1311432 (00000000001402C8h)
+  Zip archive file size:                   4481712 (00000000004462B0h)
+  Actual end-cent-dir record offset:       4481690 (000000000044629Ah)
+  Expected end-cent-dir record offset:     4481690 (000000000044629Ah)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 46 entries.
-  The central directory is 5075 (00000000000013D3h) bytes long,
+  central directory contains 50 entries.
+  The central directory is 6587 (00000000000019BBh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 1306357 (000000000013EEF5h).
+  is 4475103 (00000000004448DFh).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosDamApplication.pyd
+  KratosDamApplication-9.5.dist-info/
 
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
-  32-bit CRC value (hex):                         cca1b4a3
-  compressed size:                                489859 bytes
-  uncompressed size:                              1624064 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:58:08
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:58:07 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:58:07 UTC
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
 
-  KratosMultiphysics/.libs/KratosDamCore.dll
+  KratosDamApplication-9.5.dist-info/METADATA
 
-  offset of local header from start of archive:   489938
-                                                  (00000000000779D2h) bytes
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
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:32
-  32-bit CRC value (hex):                         2b320392
-  compressed size:                                736533 bytes
-  uncompressed size:                              2483200 bytes
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         36198e08
+  compressed size:                                1058 bytes
+  uncompressed size:                              2898 bytes
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
 
-  KratosMultiphysics/.libs/KratosDamCore.lib
+  KratosDamApplication-9.5.dist-info/WHEEL
 
-  offset of local header from start of archive:   1226543
-                                                  (000000000012B72Fh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1252
+                                                  (00000000000004E4h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:32
-  32-bit CRC value (hex):                         52078e61
-  compressed size:                                24076 bytes
-  uncompressed size:                              266260 bytes
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
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
 
-  KratosMultiphysics/DamApplication/__init__.py
+  KratosDamApplication-9.5.dist-info/top_level.txt
 
-  offset of local header from start of archive:   1250691
-                                                  (0000000000131583h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1466
+                                                  (00000000000005BAh) bytes
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
-  32-bit CRC value (hex):                         d5ebec2e
-  compressed size:                                158 bytes
-  uncompressed size:                              373 bytes
-  length of filename:                             45 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
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
 
-  KratosMultiphysics/DamApplication/apply_constraint_vector_dam_table_process.py
+  KratosDamApplication-9.5.dist-info/RECORD
 
-  offset of local header from start of archive:   1250924
-                                                  (000000000013166Ch) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1591
+                                                  (0000000000000637h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         9aadba6d
-  compressed size:                                669 bytes
-  uncompressed size:                              2977 bytes
-  length of filename:                             78 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:58:08
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:58:07 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:58:07 UTC
+  32-bit CRC value (hex):                         47eee5a6
+  compressed size:                                2370 bytes
+  uncompressed size:                              5503 bytes
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
 
-  KratosMultiphysics/DamApplication/apply_load_vector_dam_process.py
+  KratosDamApplication.libs/
 
-  offset of local header from start of archive:   1251701
-                                                  (0000000000131975h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   4060
+                                                  (0000000000000FDCh) bytes
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
-  32-bit CRC value (hex):                         46da110f
-  compressed size:                                664 bytes
-  uncompressed size:                              2558 bytes
-  length of filename:                             66 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:58:08
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:58:07 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:58:07 UTC
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
 
-  KratosMultiphysics/DamApplication/apply_load_vector_dam_table_process.py
+  KratosDamApplication.libs/libKratosDamCore-90b98398.so
 
-  offset of local header from start of archive:   1252461
-                                                  (0000000000131C6Dh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   4144
+                                                  (0000000000001030h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         bc1c1504
-  compressed size:                                733 bytes
-  uncompressed size:                              3288 bytes
-  length of filename:                             72 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         e7cf7475
+  compressed size:                                3116452 bytes
+  uncompressed size:                              11791673 bytes
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
 
-  KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_mechanical.py
+  KratosMultiphysics/
 
-  offset of local header from start of archive:   1253296
-                                                  (0000000000131FB0h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3120708
+                                                  (00000000002F9E44h) bytes
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
-  32-bit CRC value (hex):                         b9a269ad
-  compressed size:                                954 bytes
-  uncompressed size:                              4848 bytes
-  length of filename:                             83 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
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
 
-  KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_thermal.py
+  KratosMultiphysics/DamApplication/
 
-  offset of local header from start of archive:   1254363
-                                                  (00000000001323DBh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3120785
+                                                  (00000000002F9E91h) bytes
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
-  32-bit CRC value (hex):                         b8d955e6
-  compressed size:                                1255 bytes
-  uncompressed size:                              9244 bytes
-  length of filename:                             80 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
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
 
-  KratosMultiphysics/DamApplication/check_and_prepare_selfweight_model_process_dam.py
+  KratosMultiphysics/DamApplication/impose_input_table_nodal_young_modulus_process.py
 
-  offset of local header from start of archive:   1255728
-                                                  (0000000000132930h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3120877
+                                                  (00000000002F9EEDh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         6e5d16fa
-  compressed size:                                960 bytes
-  uncompressed size:                              4956 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         a1a07372
+  compressed size:                                680 bytes
+  uncompressed size:                              1879 bytes
   length of filename:                             83 characters
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
 
 Central directory entry #11:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_P_solver.py
+  KratosMultiphysics/DamApplication/impose_grouting_reference_temperature_process.py
 
-  offset of local header from start of archive:   1256801
-                                                  (0000000000132D61h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3121698
+                                                  (00000000002FA222h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         f9305778
-  compressed size:                                1851 bytes
-  uncompressed size:                              6973 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         4ad21653
+  compressed size:                                352 bytes
+  uncompressed size:                              857 bytes
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
 
 Central directory entry #12:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_UP_mechanical_solver.py
+  KratosMultiphysics/DamApplication/apply_load_vector_dam_table_process.py
 
-  offset of local header from start of archive:   1258731
-                                                  (00000000001334EBh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3122190
+                                                  (00000000002FA40Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         32c449a8
-  compressed size:                                1446 bytes
-  uncompressed size:                              5397 bytes
-  length of filename:                             61 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         d5b92df3
+  compressed size:                                727 bytes
+  uncompressed size:                              3223 bytes
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
 
 Central directory entry #13:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_UP_thermo_mechanic_solver.py
+  KratosMultiphysics/DamApplication/impose_thermal_parameters_scalar_value_process.py
 
-  offset of local header from start of archive:   1260268
-                                                  (0000000000133AECh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3123047
+                                                  (00000000002FA767h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         ee07ca58
-  compressed size:                                1563 bytes
-  uncompressed size:                              6731 bytes
-  length of filename:                             66 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         f6cfceb3
+  compressed size:                                698 bytes
+  uncompressed size:                              2423 bytes
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
 
 Central directory entry #14:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_analysis.py
+  KratosMultiphysics/DamApplication/dam_eigen_solver.py
 
-  offset of local header from start of archive:   1261927
-                                                  (0000000000134167h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3123886
+                                                  (00000000002FAAAEh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         afab174f
-  compressed size:                                4173 bytes
-  uncompressed size:                              26347 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         d8bd22f7
+  compressed size:                                1727 bytes
+  uncompressed size:                              6374 bytes
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
 
 Central directory entry #15:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_cleaning_utility.py
+  KratosMultiphysics/DamApplication/dam_thermo_mechanic_solver.py
 
-  offset of local header from start of archive:   1266179
-                                                  (0000000000135203h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3125724
+                                                  (00000000002FB1DCh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         94d86f01
-  compressed size:                                177 bytes
-  uncompressed size:                              675 bytes
-  length of filename:                             57 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         91645e0d
+  compressed size:                                4429 bytes
+  uncompressed size:                              29449 bytes
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
 
 Central directory entry #16:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_constitutive_law_utility.py
+  KratosMultiphysics/DamApplication/streamlines_output_utility.py
 
-  offset of local header from start of archive:   1266443
-                                                  (000000000013530Bh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3130274
+                                                  (00000000002FC3A2h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         f5f5181b
-  compressed size:                                327 bytes
-  uncompressed size:                              793 bytes
-  length of filename:                             65 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         f51cbdc0
+  compressed size:                                282 bytes
+  uncompressed size:                              702 bytes
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
 
 Central directory entry #17:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_construction_utility.py
+  KratosMultiphysics/DamApplication/impose_2d_random_fields_variable_process.py
 
-  offset of local header from start of archive:   1266865
-                                                  (00000000001354B1h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3130677
+                                                  (00000000002FC535h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         ca8ed42e
-  compressed size:                                1765 bytes
-  uncompressed size:                              9313 bytes
-  length of filename:                             61 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         dc3b224a
+  compressed size:                                830 bytes
+  uncompressed size:                              2360 bytes
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
 
 Central directory entry #18:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_eigen_solver.py
+  KratosMultiphysics/DamApplication/check_and_prepare_selfweight_model_process_dam.py
 
-  offset of local header from start of archive:   1268721
-                                                  (0000000000135BF1h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3131642
+                                                  (00000000002FC8FAh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         0530a44b
-  compressed size:                                1752 bytes
-  uncompressed size:                              6604 bytes
-  length of filename:                             53 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         d8f1487f
+  compressed size:                                952 bytes
+  uncompressed size:                              4871 bytes
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
 
 Central directory entry #19:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_mapping_variables_utility.py
+  KratosMultiphysics/DamApplication/gid_dam_output_process.py
 
-  offset of local header from start of archive:   1270556
-                                                  (000000000013631Ch) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3132735
+                                                  (00000000002FCD3Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         d32462bd
-  compressed size:                                416 bytes
-  uncompressed size:                              2196 bytes
-  length of filename:                             66 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         d77e4e07
+  compressed size:                                6611 bytes
+  uncompressed size:                              34676 bytes
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
 
 Central directory entry #20:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_mechanical_solver.py
+  KratosMultiphysics/DamApplication/impose_chemo_mechanical_aging_process.py
 
-  offset of local header from start of archive:   1271068
-                                                  (000000000013651Ch) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3139463
+                                                  (00000000002FE787h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         81e7c6fb
-  compressed size:                                3659 bytes
-  uncompressed size:                              22475 bytes
-  length of filename:                             58 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         4ec1a44a
+  compressed size:                                381 bytes
+  uncompressed size:                              841 bytes
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
 
 Central directory entry #21:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_selfweight_solver.py
+  KratosMultiphysics/DamApplication/impose_heat_source_process.py
 
-  offset of local header from start of archive:   1274815
-                                                  (00000000001373BFh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3139976
+                                                  (00000000002FE988h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         2312a54a
-  compressed size:                                4011 bytes
-  uncompressed size:                              24523 bytes
-  length of filename:                             58 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         007dbd51
+  compressed size:                                483 bytes
+  uncompressed size:                              1428 bytes
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
 
 Central directory entry #22:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/dam_thermo_mechanic_solver.py
+  KratosMultiphysics/DamApplication/dam_selfweight_solver.py
 
-  offset of local header from start of archive:   1278914
-                                                  (00000000001383C2h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3140580
+                                                  (00000000002FEBE4h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         9b127304
-  compressed size:                                4450 bytes
-  uncompressed size:                              29961 bytes
-  length of filename:                             63 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         9f188c96
+  compressed size:                                3986 bytes
+  uncompressed size:                              24082 bytes
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
 
 Central directory entry #23:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/gid_dam_output_process.py
+  KratosMultiphysics/DamApplication/impose_nodal_reference_temperature_process.py
 
-  offset of local header from start of archive:   1283457
-                                                  (0000000000139581h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3144682
+                                                  (00000000002FFBEAh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         3b44a987
-  compressed size:                                6640 bytes
-  uncompressed size:                              35439 bytes
-  length of filename:                             59 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         659035af
+  compressed size:                                679 bytes
+  uncompressed size:                              1810 bytes
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
 
 Central directory entry #24:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/global_joint_stress_utility.py
+  KratosMultiphysics/DamApplication/dam_construction_utility.py
 
-  offset of local header from start of archive:   1290186
-                                                  (000000000013AFCAh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3145498
+                                                  (00000000002FFF1Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         498b8a68
-  compressed size:                                362 bytes
-  uncompressed size:                              1114 bytes
-  length of filename:                             64 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         d9779879
+  compressed size:                                1757 bytes
+  uncompressed size:                              9151 bytes
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
 
 Central directory entry #25:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_2d_random_fields_variable_process.py
+  KratosMultiphysics/DamApplication/impose_uniform_temperature_process.py
 
-  offset of local header from start of archive:   1290642
-                                                  (000000000013B192h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3147374
+                                                  (000000000030066Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         e0e47287
-  compressed size:                                842 bytes
-  uncompressed size:                              2431 bytes
-  length of filename:                             77 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         4276e570
+  compressed size:                                579 bytes
+  uncompressed size:                              1663 bytes
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
 
 Central directory entry #26:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_3d_random_fields_variable_process.py
+  KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_thermal.py
 
-  offset of local header from start of archive:   1291591
-                                                  (000000000013B547h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3148082
+                                                  (0000000000300932h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         0f574137
-  compressed size:                                855 bytes
-  uncompressed size:                              2482 bytes
-  length of filename:                             77 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         35c2e3d6
+  compressed size:                                1242 bytes
+  uncompressed size:                              9089 bytes
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
 
 Central directory entry #27:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_chemo_mechanical_aging_process.py
+  KratosMultiphysics/DamApplication/dam_cleaning_utility.py
 
-  offset of local header from start of archive:   1292553
-                                                  (000000000013B909h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3149462
+                                                  (0000000000300E96h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         2f4dcd08
-  compressed size:                                385 bytes
-  uncompressed size:                              864 bytes
-  length of filename:                             74 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         cb033975
+  compressed size:                                173 bytes
+  uncompressed size:                              650 bytes
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
 
 Central directory entry #28:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_face_heat_flux_process.py
+  KratosMultiphysics/DamApplication/impose_nodal_young_modulus_process.py
 
-  offset of local header from start of archive:   1293042
-                                                  (000000000013BAF2h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3149750
+                                                  (0000000000300FB6h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         c4f8dfca
-  compressed size:                                853 bytes
-  uncompressed size:                              3212 bytes
-  length of filename:                             66 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         c4c86304
+  compressed size:                                409 bytes
+  uncompressed size:                              888 bytes
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
 
 Central directory entry #29:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_grouting_reference_temperature_process.py
+  KratosMultiphysics/DamApplication/dam_UP_mechanical_solver.py
 
-  offset of local header from start of archive:   1293991
-                                                  (000000000013BEA7h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3150288
+                                                  (00000000003011D0h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         a8ca2e1e
-  compressed size:                                355 bytes
-  uncompressed size:                              882 bytes
-  length of filename:                             82 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         922e0700
+  compressed size:                                1435 bytes
+  uncompressed size:                              5269 bytes
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
 
 Central directory entry #30:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_heat_source_process.py
+  KratosMultiphysics/DamApplication/transfer_selfweight_stress_utility.py
 
-  offset of local header from start of archive:   1294458
-                                                  (000000000013C07Ah) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3151842
+                                                  (00000000003017E2h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         7220ee91
-  compressed size:                                490 bytes
-  uncompressed size:                              1462 bytes
-  length of filename:                             63 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         0da43822
+  compressed size:                                250 bytes
+  uncompressed size:                              679 bytes
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
 
 Central directory entry #31:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_input_table_nodal_young_modulus_process.py
+  KratosMultiphysics/DamApplication/impose_reservoir_temperature_condition_process.py
 
-  offset of local header from start of archive:   1295041
-                                                  (000000000013C2C1h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3152221
+                                                  (000000000030195Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         f0d187e0
-  compressed size:                                686 bytes
-  uncompressed size:                              1924 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         53299a4e
+  compressed size:                                581 bytes
+  uncompressed size:                              1823 bytes
   length of filename:                             83 characters
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
 
 Central directory entry #32:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_nodal_reference_temperature_process.py
+  KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_mechanical.py
 
-  offset of local header from start of archive:   1295840
-                                                  (000000000013C5E0h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3152943
+                                                  (0000000000301C2Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         59e2fadf
-  compressed size:                                689 bytes
-  uncompressed size:                              1856 bytes
-  length of filename:                             79 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         dd0614a1
+  compressed size:                                946 bytes
+  uncompressed size:                              4765 bytes
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
 
 Central directory entry #33:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_nodal_young_modulus_process.py
+  KratosMultiphysics/DamApplication/apply_load_vector_dam_process.py
 
-  offset of local header from start of archive:   1296638
-                                                  (000000000013C8FEh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3154030
+                                                  (000000000030206Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         5d128829
-  compressed size:                                413 bytes
-  uncompressed size:                              916 bytes
-  length of filename:                             71 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         52a150b3
+  compressed size:                                657 bytes
+  uncompressed size:                              2505 bytes
+  length of filename:                             66 characters
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
 
-  KratosMultiphysics/DamApplication/impose_reservoir_temperature_condition_process.py
+  KratosMultiphysics/DamApplication/impose_temperature_by_device_process.py
 
-  offset of local header from start of archive:   1297152
-                                                  (000000000013CB00h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3154811
+                                                  (000000000030237Bh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         7bc54bb0
-  compressed size:                                587 bytes
-  uncompressed size:                              1868 bytes
-  length of filename:                             83 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         f1a36791
+  compressed size:                                326 bytes
+  uncompressed size:                              702 bytes
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
 
 Central directory entry #35:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_temperature_by_device_process.py
+  KratosMultiphysics/DamApplication/global_joint_stress_utility.py
 
-  offset of local header from start of archive:   1297852
-                                                  (000000000013CDBCh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3155268
+                                                  (0000000000302544h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         ed154ee9
-  compressed size:                                332 bytes
-  uncompressed size:                              723 bytes
-  length of filename:                             73 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         b35338df
+  compressed size:                                357 bytes
+  uncompressed size:                              1087 bytes
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
 
 Central directory entry #36:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_thermal_parameters_scalar_value_process.py
+  KratosMultiphysics/DamApplication/dam_constitutive_law_utility.py
 
-  offset of local header from start of archive:   1298287
-                                                  (000000000013CF6Fh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3155747
+                                                  (0000000000302723h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         bea82889
-  compressed size:                                706 bytes
-  uncompressed size:                              2480 bytes
-  length of filename:                             83 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         6d0f8728
+  compressed size:                                323 bytes
+  uncompressed size:                              775 bytes
+  length of filename:                             65 characters
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
 
-  KratosMultiphysics/DamApplication/impose_uniform_temperature_process.py
+  KratosMultiphysics/DamApplication/dam_mechanical_solver.py
 
-  offset of local header from start of archive:   1299106
-                                                  (000000000013D2A2h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3156193
+                                                  (00000000003028E1h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         e2bf4373
-  compressed size:                                586 bytes
-  uncompressed size:                              1702 bytes
-  length of filename:                             71 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         48600536
+  compressed size:                                3639 bytes
+  uncompressed size:                              22066 bytes
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
 
 Central directory entry #38:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/impose_water_loads_condition_process.py
+  KratosMultiphysics/DamApplication/dam_UP_thermo_mechanic_solver.py
 
-  offset of local header from start of archive:   1299793
-                                                  (000000000013D551h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3159948
+                                                  (000000000030378Ch) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         1175743b
-  compressed size:                                611 bytes
-  uncompressed size:                              2354 bytes
-  length of filename:                             73 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         fc95ca71
+  compressed size:                                1550 bytes
+  uncompressed size:                              6575 bytes
+  length of filename:                             66 characters
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
 
-  KratosMultiphysics/DamApplication/save_variables_utility.py
+  KratosMultiphysics/DamApplication/special_condition_process.py
 
-  offset of local header from start of archive:   1300507
-                                                  (000000000013D81Bh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3161622
+                                                  (0000000000303E16h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         771dc3b4
-  compressed size:                                713 bytes
-  uncompressed size:                              6056 bytes
-  length of filename:                             59 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         f6534ca9
+  compressed size:                                343 bytes
+  uncompressed size:                              683 bytes
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
 
 Central directory entry #40:
 ---------------------------
 
-  KratosMultiphysics/DamApplication/special_condition_process.py
+  KratosMultiphysics/DamApplication/impose_face_heat_flux_process.py
 
-  offset of local header from start of archive:   1301309
-                                                  (000000000013DB3Dh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3162085
+                                                  (0000000000303FE5h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         be094c8d
-  compressed size:                                349 bytes
-  uncompressed size:                              701 bytes
-  length of filename:                             62 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         24d063d4
+  compressed size:                                845 bytes
+  uncompressed size:                              3156 bytes
+  length of filename:                             66 characters
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
 
-  KratosMultiphysics/DamApplication/streamlines_output_utility.py
+  KratosMultiphysics/DamApplication/dam_mapping_variables_utility.py
 
-  offset of local header from start of archive:   1301750
-                                                  (000000000013DCF6h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3163054
+                                                  (00000000003043AEh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         67f90a4b
-  compressed size:                                287 bytes
-  uncompressed size:                              724 bytes
-  length of filename:                             63 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         d32462bd
+  compressed size:                                416 bytes
+  uncompressed size:                              2196 bytes
+  length of filename:                             66 characters
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
 
-  KratosMultiphysics/DamApplication/transfer_selfweight_stress_utility.py
+  KratosMultiphysics/DamApplication/dam_P_solver.py
 
-  offset of local header from start of archive:   1302130
-                                                  (000000000013DE72h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3163594
+                                                  (00000000003045CAh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         e6a439f9
-  compressed size:                                253 bytes
-  uncompressed size:                              699 bytes
-  length of filename:                             71 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         0b865c12
+  compressed size:                                1839 bytes
+  uncompressed size:                              6809 bytes
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
 
 Central directory entry #43:
 ---------------------------
 
-  KratosDamApplication-9.4.6.dist-info/METADATA
+  KratosMultiphysics/DamApplication/save_variables_utility.py
 
-  offset of local header from start of archive:   1302484
-                                                  (000000000013DFD4h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3165540
+                                                  (0000000000304D64h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:32
-  32-bit CRC value (hex):                         6f60220d
-  compressed size:                                1076 bytes
-  uncompressed size:                              2961 bytes
-  length of filename:                             45 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         51473ed7
+  compressed size:                                708 bytes
+  uncompressed size:                              5924 bytes
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
 
 Central directory entry #44:
 ---------------------------
 
-  KratosDamApplication-9.4.6.dist-info/WHEEL
+  KratosMultiphysics/DamApplication/__init__.py
 
-  offset of local header from start of archive:   1303635
-                                                  (000000000013E453h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3166365
+                                                  (000000000030509Dh) bytes
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
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         303d5681
+  compressed size:                                153 bytes
+  uncompressed size:                              363 bytes
+  length of filename:                             45 characters
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
 
-  KratosDamApplication-9.4.6.dist-info/top_level.txt
+  KratosMultiphysics/DamApplication/apply_constraint_vector_dam_table_process.py
 
-  offset of local header from start of archive:   1303803
-                                                  (000000000013E4FBh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3166621
+                                                  (000000000030519Dh) bytes
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
-  length of filename:                             50 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         0fc658d1
+  compressed size:                                662 bytes
+  uncompressed size:                              2916 bytes
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
 
 Central directory entry #46:
 ---------------------------
 
-  KratosDamApplication-9.4.6.dist-info/RECORD
+  KratosMultiphysics/DamApplication/impose_3d_random_fields_variable_process.py
 
-  offset of local header from start of archive:   1303904
-                                                  (000000000013E560h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   3167419
+                                                  (00000000003054BBh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:32
-  32-bit CRC value (hex):                         df8fe544
-  compressed size:                                2380 bytes
-  uncompressed size:                              5527 bytes
-  length of filename:                             43 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         ddf8b6bc
+  compressed size:                                843 bytes
+  uncompressed size:                              2408 bytes
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
+Central directory entry #47:
+---------------------------
+
+  KratosMultiphysics/DamApplication/impose_water_loads_condition_process.py
+
+  offset of local header from start of archive:   3168397
+                                                  (000000000030588Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         3801089c
+  compressed size:                                602 bytes
+  uncompressed size:                              2306 bytes
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
+Central directory entry #48:
+---------------------------
+
+  KratosMultiphysics/DamApplication/dam_analysis.py
+
+  offset of local header from start of archive:   3169130
+                                                  (0000000000305B6Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         8c595a60
+  compressed size:                                4149 bytes
+  uncompressed size:                              25883 bytes
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
+Central directory entry #49:
+---------------------------
+
+  KratosMultiphysics/.libs/
+
+  offset of local header from start of archive:   3173386
+                                                  (0000000000306C0Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
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
+Central directory entry #50:
+---------------------------
+
+  KratosMultiphysics/.libs/KratosDamApplication.cpython-39-x86_64-linux-gnu.so
+
+  offset of local header from start of archive:   3173469
+                                                  (0000000000306C5Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 15:57:58
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 15:57:58 UTC
+  32-bit CRC value (hex):                         f92beb75
+  compressed size:                                1301500 bytes
+  uncompressed size:                              3827505 bytes
+  length of filename:                             76 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B400 hex
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
@@ -1,139 +1,151 @@
-Filename: KratosMultiphysics/.libs/KratosDamApplication.pyd
+Filename: KratosDamApplication-9.5.dist-info/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosDamCore.dll
+Filename: KratosDamApplication-9.5.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosDamCore.lib
+Filename: KratosDamApplication-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/__init__.py
+Filename: KratosDamApplication-9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/apply_constraint_vector_dam_table_process.py
+Filename: KratosDamApplication-9.5.dist-info/RECORD
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/apply_load_vector_dam_process.py
+Filename: KratosDamApplication.libs/
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/apply_load_vector_dam_table_process.py
+Filename: KratosDamApplication.libs/libKratosDamCore-90b98398.so
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_mechanical.py
+Filename: KratosMultiphysics/
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_thermal.py
+Filename: KratosMultiphysics/DamApplication/
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/check_and_prepare_selfweight_model_process_dam.py
+Filename: KratosMultiphysics/DamApplication/impose_input_table_nodal_young_modulus_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/dam_P_solver.py
+Filename: KratosMultiphysics/DamApplication/impose_grouting_reference_temperature_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/dam_UP_mechanical_solver.py
+Filename: KratosMultiphysics/DamApplication/apply_load_vector_dam_table_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/dam_UP_thermo_mechanic_solver.py
+Filename: KratosMultiphysics/DamApplication/impose_thermal_parameters_scalar_value_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/dam_analysis.py
+Filename: KratosMultiphysics/DamApplication/dam_eigen_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/dam_cleaning_utility.py
+Filename: KratosMultiphysics/DamApplication/dam_thermo_mechanic_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/dam_constitutive_law_utility.py
+Filename: KratosMultiphysics/DamApplication/streamlines_output_utility.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/dam_construction_utility.py
+Filename: KratosMultiphysics/DamApplication/impose_2d_random_fields_variable_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/dam_eigen_solver.py
+Filename: KratosMultiphysics/DamApplication/check_and_prepare_selfweight_model_process_dam.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/dam_mapping_variables_utility.py
+Filename: KratosMultiphysics/DamApplication/gid_dam_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/dam_mechanical_solver.py
+Filename: KratosMultiphysics/DamApplication/impose_chemo_mechanical_aging_process.py
+Comment: 
+
+Filename: KratosMultiphysics/DamApplication/impose_heat_source_process.py
 Comment: 
 
 Filename: KratosMultiphysics/DamApplication/dam_selfweight_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/dam_thermo_mechanic_solver.py
+Filename: KratosMultiphysics/DamApplication/impose_nodal_reference_temperature_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/gid_dam_output_process.py
+Filename: KratosMultiphysics/DamApplication/dam_construction_utility.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/global_joint_stress_utility.py
+Filename: KratosMultiphysics/DamApplication/impose_uniform_temperature_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_2d_random_fields_variable_process.py
+Filename: KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_thermal.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_3d_random_fields_variable_process.py
+Filename: KratosMultiphysics/DamApplication/dam_cleaning_utility.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_chemo_mechanical_aging_process.py
+Filename: KratosMultiphysics/DamApplication/impose_nodal_young_modulus_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_face_heat_flux_process.py
+Filename: KratosMultiphysics/DamApplication/dam_UP_mechanical_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_grouting_reference_temperature_process.py
+Filename: KratosMultiphysics/DamApplication/transfer_selfweight_stress_utility.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_heat_source_process.py
+Filename: KratosMultiphysics/DamApplication/impose_reservoir_temperature_condition_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_input_table_nodal_young_modulus_process.py
+Filename: KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_mechanical.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_nodal_reference_temperature_process.py
+Filename: KratosMultiphysics/DamApplication/apply_load_vector_dam_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_nodal_young_modulus_process.py
+Filename: KratosMultiphysics/DamApplication/impose_temperature_by_device_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_reservoir_temperature_condition_process.py
+Filename: KratosMultiphysics/DamApplication/global_joint_stress_utility.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_temperature_by_device_process.py
+Filename: KratosMultiphysics/DamApplication/dam_constitutive_law_utility.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_thermal_parameters_scalar_value_process.py
+Filename: KratosMultiphysics/DamApplication/dam_mechanical_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_uniform_temperature_process.py
+Filename: KratosMultiphysics/DamApplication/dam_UP_thermo_mechanic_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/impose_water_loads_condition_process.py
+Filename: KratosMultiphysics/DamApplication/special_condition_process.py
+Comment: 
+
+Filename: KratosMultiphysics/DamApplication/impose_face_heat_flux_process.py
+Comment: 
+
+Filename: KratosMultiphysics/DamApplication/dam_mapping_variables_utility.py
+Comment: 
+
+Filename: KratosMultiphysics/DamApplication/dam_P_solver.py
 Comment: 
 
 Filename: KratosMultiphysics/DamApplication/save_variables_utility.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/special_condition_process.py
+Filename: KratosMultiphysics/DamApplication/__init__.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/streamlines_output_utility.py
+Filename: KratosMultiphysics/DamApplication/apply_constraint_vector_dam_table_process.py
 Comment: 
 
-Filename: KratosMultiphysics/DamApplication/transfer_selfweight_stress_utility.py
+Filename: KratosMultiphysics/DamApplication/impose_3d_random_fields_variable_process.py
 Comment: 
 
-Filename: KratosDamApplication-9.4.6.dist-info/METADATA
+Filename: KratosMultiphysics/DamApplication/impose_water_loads_condition_process.py
 Comment: 
 
-Filename: KratosDamApplication-9.4.6.dist-info/WHEEL
+Filename: KratosMultiphysics/DamApplication/dam_analysis.py
 Comment: 
 
-Filename: KratosDamApplication-9.4.6.dist-info/top_level.txt
+Filename: KratosMultiphysics/.libs/
 Comment: 
 
-Filename: KratosDamApplication-9.4.6.dist-info/RECORD
+Filename: KratosMultiphysics/.libs/KratosDamApplication.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## KratosMultiphysics/DamApplication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,10 +1,10 @@
-
-# Application dependent names and paths
-from KratosMultiphysics import _ImportApplication
-import KratosMultiphysics.StructuralMechanicsApplication
-import KratosMultiphysics.PoromechanicsApplication
-from KratosDamApplication import *
-application = KratosDamApplication()
-application_name = "KratosDamApplication"
-
-_ImportApplication(application,application_name)
+
+# Application dependent names and paths
+from KratosMultiphysics import _ImportApplication
+import KratosMultiphysics.StructuralMechanicsApplication
+import KratosMultiphysics.PoromechanicsApplication
+from KratosDamApplication import *
+application = KratosDamApplication()
+application_name = "KratosDamApplication"
+
+_ImportApplication(application,application_name)
```

## KratosMultiphysics/DamApplication/apply_constraint_vector_dam_table_process.py

 * *Ordering differences only*

```diff
@@ -1,61 +1,61 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ApplyConstraintVectorDamTableProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-
-class ApplyConstraintVectorDamTableProcess(Process):
-    def __init__(self, Model, settings ):
-        Process.__init__(self)
-
-        model_part = Model[settings["model_part_name"].GetString()]
-        variable_name = settings["variable_name"].GetString()
-
-        self.components_process_list = []
-
-        x_params = Parameters("{}")
-        x_params.AddValue("model_part_name",settings["model_part_name"])
-        x_params.AddValue("is_fixed",settings["is_fixed"][0])
-        x_params.AddValue("value",settings["value"][0])
-        x_params.AddEmptyValue("variable_name").SetString(variable_name+"_X")
-        if settings["Value_Table"][0].GetInt() == 0:
-            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, x_params))
-        else:
-            x_params.AddValue("table",settings["Value_Table"][0])
-            self.components_process_list.append(ApplyComponentTableProcessDam(model_part, x_params))
-
-        y_params = Parameters("{}")
-        y_params.AddValue("model_part_name",settings["model_part_name"])
-        y_params.AddValue("is_fixed",settings["is_fixed"][1])
-        y_params.AddValue("value",settings["value"][1])
-        y_params.AddEmptyValue("variable_name").SetString(variable_name+"_Y")
-        if settings["Value_Table"][1].GetInt() == 0:
-            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, y_params))
-        else:
-            y_params.AddValue("table",settings["Value_Table"][1])
-            self.components_process_list.append(ApplyComponentTableProcessDam(model_part, y_params))
-
-        z_params = Parameters("{}")
-        z_params.AddValue("model_part_name",settings["model_part_name"])
-        z_params.AddValue("is_fixed",settings["is_fixed"][2])
-        z_params.AddValue("value",settings["value"][2])
-        z_params.AddEmptyValue("variable_name").SetString(variable_name+"_Z")
-        if settings["Value_Table"][2].GetInt() == 0:
-            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, z_params))
-        else:
-            z_params.AddValue("table",settings["Value_Table"][2])
-            self.components_process_list.append(ApplyComponentTableProcessDam(model_part, z_params))
-
-    def ExecuteInitialize(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitializeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ApplyConstraintVectorDamTableProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+
+class ApplyConstraintVectorDamTableProcess(Process):
+    def __init__(self, Model, settings ):
+        Process.__init__(self)
+
+        model_part = Model[settings["model_part_name"].GetString()]
+        variable_name = settings["variable_name"].GetString()
+
+        self.components_process_list = []
+
+        x_params = Parameters("{}")
+        x_params.AddValue("model_part_name",settings["model_part_name"])
+        x_params.AddValue("is_fixed",settings["is_fixed"][0])
+        x_params.AddValue("value",settings["value"][0])
+        x_params.AddEmptyValue("variable_name").SetString(variable_name+"_X")
+        if settings["Value_Table"][0].GetInt() == 0:
+            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, x_params))
+        else:
+            x_params.AddValue("table",settings["Value_Table"][0])
+            self.components_process_list.append(ApplyComponentTableProcessDam(model_part, x_params))
+
+        y_params = Parameters("{}")
+        y_params.AddValue("model_part_name",settings["model_part_name"])
+        y_params.AddValue("is_fixed",settings["is_fixed"][1])
+        y_params.AddValue("value",settings["value"][1])
+        y_params.AddEmptyValue("variable_name").SetString(variable_name+"_Y")
+        if settings["Value_Table"][1].GetInt() == 0:
+            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, y_params))
+        else:
+            y_params.AddValue("table",settings["Value_Table"][1])
+            self.components_process_list.append(ApplyComponentTableProcessDam(model_part, y_params))
+
+        z_params = Parameters("{}")
+        z_params.AddValue("model_part_name",settings["model_part_name"])
+        z_params.AddValue("is_fixed",settings["is_fixed"][2])
+        z_params.AddValue("value",settings["value"][2])
+        z_params.AddEmptyValue("variable_name").SetString(variable_name+"_Z")
+        if settings["Value_Table"][2].GetInt() == 0:
+            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, z_params))
+        else:
+            z_params.AddValue("table",settings["Value_Table"][2])
+            self.components_process_list.append(ApplyComponentTableProcessDam(model_part, z_params))
+
+    def ExecuteInitialize(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/apply_load_vector_dam_process.py

 * *Ordering differences only*

```diff
@@ -1,53 +1,53 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ApplyLoadVectorDamProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-
-class ApplyLoadVectorDamProcess(Process):
-    def __init__(self, Model, settings ):
-        Process.__init__(self)
-
-        model_part = Model[settings["model_part_name"].GetString()]
-        variable_name = settings["variable_name"].GetString()
-
-        self.components_process_list = []
-
-        self.factor = settings["modulus"].GetDouble();
-        self.direction = [settings["direction"][0].GetDouble(),settings["direction"][1].GetDouble(),settings["direction"][2].GetDouble()]
-        self.value = [self.direction[0]*self.factor,self.direction[1]*self.factor,self.direction[2]*self.factor]
-
-        if abs(self.value[0])>1.0e-15:
-            x_params = Parameters("{}")
-            x_params.AddValue("model_part_name",settings["model_part_name"])
-            x_params.AddEmptyValue("value").SetDouble(self.value[0])
-            x_params.AddEmptyValue("variable_name").SetString(variable_name+"_X")
-            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, x_params))
-
-        if abs(self.value[1])>1.0e-15:
-            y_params = Parameters("{}")
-            y_params.AddValue("model_part_name",settings["model_part_name"])
-            y_params.AddEmptyValue("value").SetDouble(self.value[1])
-            y_params.AddEmptyValue("variable_name").SetString(variable_name+"_Y")
-            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, y_params))
-
-        if abs(self.value[2])>1.0e-15:
-            z_params = Parameters("{}")
-            z_params.AddValue("model_part_name",settings["model_part_name"])
-            z_params.AddEmptyValue("value").SetDouble(self.value[2])
-            z_params.AddEmptyValue("variable_name").SetString(variable_name+"_Z")
-            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, z_params))
-
-    def ExecuteInitialize(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitializeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ApplyLoadVectorDamProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+
+class ApplyLoadVectorDamProcess(Process):
+    def __init__(self, Model, settings ):
+        Process.__init__(self)
+
+        model_part = Model[settings["model_part_name"].GetString()]
+        variable_name = settings["variable_name"].GetString()
+
+        self.components_process_list = []
+
+        self.factor = settings["modulus"].GetDouble();
+        self.direction = [settings["direction"][0].GetDouble(),settings["direction"][1].GetDouble(),settings["direction"][2].GetDouble()]
+        self.value = [self.direction[0]*self.factor,self.direction[1]*self.factor,self.direction[2]*self.factor]
+
+        if abs(self.value[0])>1.0e-15:
+            x_params = Parameters("{}")
+            x_params.AddValue("model_part_name",settings["model_part_name"])
+            x_params.AddEmptyValue("value").SetDouble(self.value[0])
+            x_params.AddEmptyValue("variable_name").SetString(variable_name+"_X")
+            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, x_params))
+
+        if abs(self.value[1])>1.0e-15:
+            y_params = Parameters("{}")
+            y_params.AddValue("model_part_name",settings["model_part_name"])
+            y_params.AddEmptyValue("value").SetDouble(self.value[1])
+            y_params.AddEmptyValue("variable_name").SetString(variable_name+"_Y")
+            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, y_params))
+
+        if abs(self.value[2])>1.0e-15:
+            z_params = Parameters("{}")
+            z_params.AddValue("model_part_name",settings["model_part_name"])
+            z_params.AddEmptyValue("value").SetDouble(self.value[2])
+            z_params.AddEmptyValue("variable_name").SetString(variable_name+"_Z")
+            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, z_params))
+
+    def ExecuteInitialize(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/apply_load_vector_dam_table_process.py

 * *Ordering differences only*

```diff
@@ -1,65 +1,65 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ApplyLoadVectorDamTableProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-
-class ApplyLoadVectorDamTableProcess(Process):
-    def __init__(self, Model, settings ):
-        Process.__init__(self)
-
-        model_part = Model[settings["model_part_name"].GetString()]
-        variable_name = settings["variable_name"].GetString()
-
-        self.components_process_list = []
-
-        self.factor = settings["modulus"].GetDouble();
-        self.direction = [settings["direction"][0].GetDouble(),settings["direction"][1].GetDouble(),settings["direction"][2].GetDouble()]
-        self.value = [self.direction[0]*self.factor,self.direction[1]*self.factor,self.direction[2]*self.factor]
-
-        if abs(self.value[0])>1.0e-15:
-            x_params = Parameters("{}")
-            x_params.AddValue("model_part_name",settings["model_part_name"])
-            x_params.AddEmptyValue("value").SetDouble(self.value[0])
-            x_params.AddEmptyValue("variable_name").SetString(variable_name+"_X")
-            if settings["table"].GetInt() == 0:
-                self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, x_params))
-            else:
-                x_params.AddValue("table",settings["table"])
-                self.components_process_list.append(ApplyComponentTableProcessDam(model_part, x_params))
-
-        if abs(self.value[1])>1.0e-15:
-            y_params = Parameters("{}")
-            y_params.AddValue("model_part_name",settings["model_part_name"])
-            y_params.AddEmptyValue("value").SetDouble(self.value[1])
-            y_params.AddEmptyValue("variable_name").SetString(variable_name+"_Y")
-            if settings["table"].GetInt() == 0:
-                self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, y_params))
-            else:
-                y_params.AddValue("table",settings["table"])
-                self.components_process_list.append(ApplyComponentTableProcessDam(model_part, y_params))
-
-        if abs(self.value[2])>1.0e-15:
-            z_params = Parameters("{}")
-            z_params.AddValue("model_part_name",settings["model_part_name"])
-            z_params.AddEmptyValue("value").SetDouble(self.value[2])
-            z_params.AddEmptyValue("variable_name").SetString(variable_name+"_Z")
-            if settings["table"].GetInt() == 0:
-                self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, z_params))
-            else:
-                z_params.AddValue("table",settings["table"])
-                self.components_process_list.append(ApplyComponentTableProcessDam(model_part, z_params))
-
-    def ExecuteInitialize(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitializeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ApplyLoadVectorDamTableProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+
+class ApplyLoadVectorDamTableProcess(Process):
+    def __init__(self, Model, settings ):
+        Process.__init__(self)
+
+        model_part = Model[settings["model_part_name"].GetString()]
+        variable_name = settings["variable_name"].GetString()
+
+        self.components_process_list = []
+
+        self.factor = settings["modulus"].GetDouble();
+        self.direction = [settings["direction"][0].GetDouble(),settings["direction"][1].GetDouble(),settings["direction"][2].GetDouble()]
+        self.value = [self.direction[0]*self.factor,self.direction[1]*self.factor,self.direction[2]*self.factor]
+
+        if abs(self.value[0])>1.0e-15:
+            x_params = Parameters("{}")
+            x_params.AddValue("model_part_name",settings["model_part_name"])
+            x_params.AddEmptyValue("value").SetDouble(self.value[0])
+            x_params.AddEmptyValue("variable_name").SetString(variable_name+"_X")
+            if settings["table"].GetInt() == 0:
+                self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, x_params))
+            else:
+                x_params.AddValue("table",settings["table"])
+                self.components_process_list.append(ApplyComponentTableProcessDam(model_part, x_params))
+
+        if abs(self.value[1])>1.0e-15:
+            y_params = Parameters("{}")
+            y_params.AddValue("model_part_name",settings["model_part_name"])
+            y_params.AddEmptyValue("value").SetDouble(self.value[1])
+            y_params.AddEmptyValue("variable_name").SetString(variable_name+"_Y")
+            if settings["table"].GetInt() == 0:
+                self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, y_params))
+            else:
+                y_params.AddValue("table",settings["table"])
+                self.components_process_list.append(ApplyComponentTableProcessDam(model_part, y_params))
+
+        if abs(self.value[2])>1.0e-15:
+            z_params = Parameters("{}")
+            z_params.AddValue("model_part_name",settings["model_part_name"])
+            z_params.AddEmptyValue("value").SetDouble(self.value[2])
+            z_params.AddEmptyValue("variable_name").SetString(variable_name+"_Z")
+            if settings["table"].GetInt() == 0:
+                self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, z_params))
+            else:
+                z_params.AddValue("table",settings["table"])
+                self.components_process_list.append(ApplyComponentTableProcessDam(model_part, z_params))
+
+    def ExecuteInitialize(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_mechanical.py

 * *Ordering differences only*

```diff
@@ -1,83 +1,83 @@
-import KratosMultiphysics
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return CheckAndPrepareModelProcessDamMechanical(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class CheckAndPrepareModelProcessDamMechanical(KratosMultiphysics.Process):
-    """Prepare the computing model part.
-
-    The computing model part is created if it does not exist. Nodes and elements
-    from the domain sub model parts are added to the computing model part.
-    Conditions are added from the processes sub model parts.
-    """
-    def __init__(self, main_model_part, Parameters ):
-        KratosMultiphysics.Process.__init__(self)
-        self.main_model_part = main_model_part
-
-        self.mechanical_model_part_name  = Parameters["mechanical_model_part_name"].GetString()
-        self.mechanical_domain_sub_model_part_list = Parameters["mechanical_domain_sub_model_part_list"]
-        self.mechanical_loads_sub_model_part_list = Parameters["mechanical_loads_sub_model_part_list"]
-        self.body_domain_sub_model_part_list = Parameters["body_domain_sub_model_part_list"]
-        self.body_domain_sub_sub_model_part_list = Parameters["body_domain_sub_sub_model_part_list"]
-        self.loads_sub_model_part_list = Parameters["loads_sub_model_part_list"]
-        self.loads_sub_sub_model_part_list = Parameters["loads_sub_sub_model_part_list"]
-
-    def Execute(self):
-        # Construct the computing model part: a model part which contains the mesh to compute
-        self.main_model_part.CreateSubModelPart(self.mechanical_model_part_name)
-        mechanical_model_part = self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
-        mechanical_model_part.ProcessInfo = self.main_model_part.ProcessInfo
-        mechanical_model_part.Properties = self.main_model_part.Properties
-        mechanical_model_part.Set(KratosMultiphysics.ACTIVE)
-
-        domain_parts = []
-        for i in range(self.mechanical_domain_sub_model_part_list.size()):
-            domain_parts.append(self.main_model_part.GetSubModelPart(self.mechanical_domain_sub_model_part_list[i].GetString()))
-        # Adding Nodes to Computing Model Part
-        list_of_ids = set()
-        for part in domain_parts:
-            for node in part.Nodes:
-                list_of_ids.add(node.Id)
-        mechanical_model_part.AddNodes(list(list_of_ids))
-        # Adding Elements to Computing Model Part
-        list_of_ids = set()
-        for part in domain_parts:
-            for elem in part.Elements:
-                list_of_ids.add(elem.Id)
-        mechanical_model_part.AddElements(list(list_of_ids))
-        # Adding Conditions to Computing Model Part
-        domain_conditions = []
-        for i in range(self.mechanical_loads_sub_model_part_list.size()):
-            domain_conditions.append(self.main_model_part.GetSubModelPart(self.mechanical_loads_sub_model_part_list[i].GetString()))
-        list_of_ids = set()
-        for part in domain_conditions:
-            for cond in part.Conditions:
-                list_of_ids.add(cond.Id)
-        mechanical_model_part.AddConditions(list(list_of_ids))
-
-        # Adding Computing Sub Sub Model Parts
-        # Body - Joints
-        for i in range(self.body_domain_sub_model_part_list.size()):
-            body_sub_model_part = self.main_model_part.GetSubModelPart(self.body_domain_sub_model_part_list[i].GetString())
-            mechanical_model_part.CreateSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
-            body_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
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
-            mechanical_model_part.CreateSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
-            load_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
-            list_of_ids = set()
-            for node in load_sub_model_part.Nodes:
-                list_of_ids.add(node.Id)
-            load_sub_sub_model_part.AddNodes(list(list_of_ids))
+import KratosMultiphysics
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return CheckAndPrepareModelProcessDamMechanical(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class CheckAndPrepareModelProcessDamMechanical(KratosMultiphysics.Process):
+    """Prepare the computing model part.
+
+    The computing model part is created if it does not exist. Nodes and elements
+    from the domain sub model parts are added to the computing model part.
+    Conditions are added from the processes sub model parts.
+    """
+    def __init__(self, main_model_part, Parameters ):
+        KratosMultiphysics.Process.__init__(self)
+        self.main_model_part = main_model_part
+
+        self.mechanical_model_part_name  = Parameters["mechanical_model_part_name"].GetString()
+        self.mechanical_domain_sub_model_part_list = Parameters["mechanical_domain_sub_model_part_list"]
+        self.mechanical_loads_sub_model_part_list = Parameters["mechanical_loads_sub_model_part_list"]
+        self.body_domain_sub_model_part_list = Parameters["body_domain_sub_model_part_list"]
+        self.body_domain_sub_sub_model_part_list = Parameters["body_domain_sub_sub_model_part_list"]
+        self.loads_sub_model_part_list = Parameters["loads_sub_model_part_list"]
+        self.loads_sub_sub_model_part_list = Parameters["loads_sub_sub_model_part_list"]
+
+    def Execute(self):
+        # Construct the computing model part: a model part which contains the mesh to compute
+        self.main_model_part.CreateSubModelPart(self.mechanical_model_part_name)
+        mechanical_model_part = self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
+        mechanical_model_part.ProcessInfo = self.main_model_part.ProcessInfo
+        mechanical_model_part.Properties = self.main_model_part.Properties
+        mechanical_model_part.Set(KratosMultiphysics.ACTIVE)
+
+        domain_parts = []
+        for i in range(self.mechanical_domain_sub_model_part_list.size()):
+            domain_parts.append(self.main_model_part.GetSubModelPart(self.mechanical_domain_sub_model_part_list[i].GetString()))
+        # Adding Nodes to Computing Model Part
+        list_of_ids = set()
+        for part in domain_parts:
+            for node in part.Nodes:
+                list_of_ids.add(node.Id)
+        mechanical_model_part.AddNodes(list(list_of_ids))
+        # Adding Elements to Computing Model Part
+        list_of_ids = set()
+        for part in domain_parts:
+            for elem in part.Elements:
+                list_of_ids.add(elem.Id)
+        mechanical_model_part.AddElements(list(list_of_ids))
+        # Adding Conditions to Computing Model Part
+        domain_conditions = []
+        for i in range(self.mechanical_loads_sub_model_part_list.size()):
+            domain_conditions.append(self.main_model_part.GetSubModelPart(self.mechanical_loads_sub_model_part_list[i].GetString()))
+        list_of_ids = set()
+        for part in domain_conditions:
+            for cond in part.Conditions:
+                list_of_ids.add(cond.Id)
+        mechanical_model_part.AddConditions(list(list_of_ids))
+
+        # Adding Computing Sub Sub Model Parts
+        # Body - Joints
+        for i in range(self.body_domain_sub_model_part_list.size()):
+            body_sub_model_part = self.main_model_part.GetSubModelPart(self.body_domain_sub_model_part_list[i].GetString())
+            mechanical_model_part.CreateSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
+            body_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
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
+            mechanical_model_part.CreateSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
+            load_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
+            list_of_ids = set()
+            for node in load_sub_model_part.Nodes:
+                list_of_ids.add(node.Id)
+            load_sub_sub_model_part.AddNodes(list(list_of_ids))
```

## KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_thermal.py

 * *Ordering differences only*

```diff
@@ -1,155 +1,155 @@
-import KratosMultiphysics
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return CheckAndPrepareModelProcessDamThermal(Model, settings["Parameters"])
-
-
-## All the processes python should be derived from "Process"
-class CheckAndPrepareModelProcessDamThermal(KratosMultiphysics.Process):
-    """Prepare the computing model part.
-
-    The computing model part is created if it does not exist. Nodes and elements
-    from the domain sub model parts are added to the computing model part.
-    Conditions are added from the processes sub model parts.
-    """
-    def __init__(self, main_model_part, Parameters ):
-        KratosMultiphysics.Process.__init__(self)
-        self.main_model_part = main_model_part
-
-        self.thermal_model_part_name  = Parameters["thermal_model_part_name"].GetString()
-        self.thermal_domain_sub_model_part_list = Parameters["thermal_domain_sub_model_part_list"]
-        self.thermal_loads_sub_model_part_list = Parameters["thermal_loads_sub_model_part_list"]
-        self.thermal_domain_sub_sub_model_part_list = Parameters["thermal_domain_sub_sub_model_part_list"]
-        self.thermal_loads_sub_sub_model_part_list = Parameters["thermal_loads_sub_sub_model_part_list"]
-
-        self.mechanical_model_part_name  = Parameters["mechanical_model_part_name"].GetString()
-        self.mechanical_domain_sub_model_part_list = Parameters["mechanical_domain_sub_model_part_list"]
-        self.mechanical_loads_sub_model_part_list = Parameters["mechanical_loads_sub_model_part_list"]
-        self.body_domain_sub_model_part_list = Parameters["body_domain_sub_model_part_list"]
-        self.body_domain_sub_sub_model_part_list = Parameters["body_domain_sub_sub_model_part_list"]
-        self.loads_sub_model_part_list = Parameters["loads_sub_model_part_list"]
-        self.loads_sub_sub_model_part_list = Parameters["loads_sub_sub_model_part_list"]
-
-    def Execute(self):
-
-        ## Construct the thermal model part:
-        thermal_parts = []
-        for i in range(self.thermal_domain_sub_model_part_list.size()):
-            thermal_parts.append(self.main_model_part.GetSubModelPart(self.thermal_domain_sub_model_part_list[i].GetString()))
-        self.main_model_part.CreateSubModelPart(self.thermal_model_part_name)
-        thermal_model_part = self.main_model_part.GetSubModelPart(self.thermal_model_part_name)
-        thermal_model_part.ProcessInfo = self.main_model_part.ProcessInfo
-        thermal_model_part.Properties = self.main_model_part.Properties
-        thermal_model_part.Set(KratosMultiphysics.ACTIVE)
-        print("Adding Nodes to Thermal Model Part")
-        list_of_ids = set()
-        for part in thermal_parts:
-            for node in part.Nodes:
-                list_of_ids.add(node.Id)
-        thermal_model_part.AddNodes(list(list_of_ids))
-        print("Adding Elements to Thermal Model Part")
-        list_of_ids = set()
-        for part in thermal_parts:
-            for elem in part.Elements:
-                list_of_ids.add(elem.Id)
-        thermal_model_part.AddElements(list(list_of_ids))
-        # Thermal Conditions
-        print("Adding Thermal Conditions to Thermal Model Part")
-        thermal_conditions = []
-        for i in range(self.thermal_loads_sub_model_part_list.size()):
-            thermal_conditions.append(self.main_model_part.GetSubModelPart(self.thermal_loads_sub_model_part_list[i].GetString()))
-        list_of_ids = set()
-        for part in thermal_conditions:
-            for cond in part.Conditions:
-                list_of_ids.add(cond.Id)
-        thermal_model_part.AddConditions(list(list_of_ids))
-        # Sub sub model parts
-        # Construction process
-        print("Adding Thermal Sub Sub Model Parts")
-        for i in range(self.thermal_domain_sub_model_part_list.size()):
-            thermal_sub_model_part = self.main_model_part.GetSubModelPart(self.thermal_domain_sub_model_part_list[i].GetString())
-            thermal_model_part.CreateSubModelPart(self.thermal_domain_sub_sub_model_part_list[i].GetString())
-            thermal_sub_sub_model_part = thermal_model_part.GetSubModelPart(self.thermal_domain_sub_sub_model_part_list[i].GetString())
-            list_of_ids = set()
-            for elem in thermal_sub_model_part.Elements:
-                list_of_ids.add(elem.Id)
-            thermal_sub_sub_model_part.AddElements(list(list_of_ids))
-            list_of_ids = set()
-            for node in thermal_sub_model_part.Nodes:
-                list_of_ids.add(node.Id)
-            thermal_sub_sub_model_part.AddNodes(list(list_of_ids))
-        for i in range(self.thermal_loads_sub_model_part_list.size()):
-            thermal_load_sub_model_part = self.main_model_part.GetSubModelPart(self.thermal_loads_sub_model_part_list[i].GetString())
-            thermal_model_part.CreateSubModelPart(self.thermal_loads_sub_sub_model_part_list[i].GetString())
-            thermal_load_sub_sub_model_part = thermal_model_part.GetSubModelPart(self.thermal_loads_sub_sub_model_part_list[i].GetString())
-            list_of_ids = set()
-            for node in thermal_load_sub_model_part.Nodes:
-                list_of_ids.add(node.Id)
-            thermal_load_sub_sub_model_part.AddNodes(list(list_of_ids))
-            list_of_ids = set()
-            for cond in thermal_load_sub_model_part.Conditions:
-                list_of_ids.add(cond.Id)
-            thermal_load_sub_sub_model_part.AddConditions(list(list_of_ids))
-        print(thermal_model_part)
-
-        ## Construct the mechanical model part:
-        mechanical_parts = []
-        for i in range(self.mechanical_domain_sub_model_part_list.size()):
-            mechanical_parts.append(self.main_model_part.GetSubModelPart(self.mechanical_domain_sub_model_part_list[i].GetString()))
-        self.main_model_part.CreateSubModelPart(self.mechanical_model_part_name)
-        mechanical_model_part = self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
-        mechanical_model_part.ProcessInfo = self.main_model_part.ProcessInfo
-        mechanical_model_part.Properties = self.main_model_part.Properties
-        mechanical_model_part.Set(KratosMultiphysics.ACTIVE)
-        print("Adding Nodes to Mechanical Model Part")
-        list_of_ids = set()
-        for part in mechanical_parts:
-            for node in part.Nodes:
-                list_of_ids.add(node.Id)
-        mechanical_model_part.AddNodes(list(list_of_ids))
-        print("Adding Elements to Mechanical Model Part")
-        list_of_ids = set()
-        for part in mechanical_parts:
-            for elem in part.Elements:
-                list_of_ids.add(elem.Id)
-        mechanical_model_part.AddElements(list(list_of_ids))
-        # Mechanical Conditions
-        print("Adding Conditions to Mechanical Model Part")
-        mechanical_conditions = []
-        for i in range(self.mechanical_loads_sub_model_part_list.size()):
-            mechanical_conditions.append(self.main_model_part.GetSubModelPart(self.mechanical_loads_sub_model_part_list[i].GetString()))
-        list_of_ids = set()
-        for part in mechanical_conditions:
-            for cond in part.Conditions:
-                list_of_ids.add(cond.Id)
-        mechanical_model_part.AddConditions(list(list_of_ids))
-        print("Adding Mechanical Sub Sub Model Parts")
-        # Sub sub model parts
-        # Body - Joints
-        for i in range(self.body_domain_sub_model_part_list.size()):
-            body_sub_model_part = self.main_model_part.GetSubModelPart(self.body_domain_sub_model_part_list[i].GetString())
-            mechanical_model_part.CreateSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
-            body_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
-            list_of_ids = set()
-            for node in body_sub_model_part.Nodes:
-                list_of_ids.add(node.Id)
-            body_sub_sub_model_part.AddNodes(list(list_of_ids))
-            list_of_ids = set()
-            for elem in body_sub_model_part.Elements:
-                list_of_ids.add(elem.Id)
-            body_sub_sub_model_part.AddElements(list(list_of_ids))
-        # Arc-length
-        for i in range(self.loads_sub_model_part_list.size()):
-            load_sub_model_part = self.main_model_part.GetSubModelPart(self.loads_sub_model_part_list[i].GetString())
-            mechanical_model_part.CreateSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
-            load_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
-            list_of_ids = set()
-            for node in load_sub_model_part.Nodes:
-                list_of_ids.add(node.Id)
-            load_sub_sub_model_part.AddNodes(list(list_of_ids))
-            for cond in load_sub_model_part.Conditions:
-                list_of_ids.add(cond.Id)
-            load_sub_sub_model_part.AddConditions(list(list_of_ids))
-        print(mechanical_model_part)
+import KratosMultiphysics
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return CheckAndPrepareModelProcessDamThermal(Model, settings["Parameters"])
+
+
+## All the processes python should be derived from "Process"
+class CheckAndPrepareModelProcessDamThermal(KratosMultiphysics.Process):
+    """Prepare the computing model part.
+
+    The computing model part is created if it does not exist. Nodes and elements
+    from the domain sub model parts are added to the computing model part.
+    Conditions are added from the processes sub model parts.
+    """
+    def __init__(self, main_model_part, Parameters ):
+        KratosMultiphysics.Process.__init__(self)
+        self.main_model_part = main_model_part
+
+        self.thermal_model_part_name  = Parameters["thermal_model_part_name"].GetString()
+        self.thermal_domain_sub_model_part_list = Parameters["thermal_domain_sub_model_part_list"]
+        self.thermal_loads_sub_model_part_list = Parameters["thermal_loads_sub_model_part_list"]
+        self.thermal_domain_sub_sub_model_part_list = Parameters["thermal_domain_sub_sub_model_part_list"]
+        self.thermal_loads_sub_sub_model_part_list = Parameters["thermal_loads_sub_sub_model_part_list"]
+
+        self.mechanical_model_part_name  = Parameters["mechanical_model_part_name"].GetString()
+        self.mechanical_domain_sub_model_part_list = Parameters["mechanical_domain_sub_model_part_list"]
+        self.mechanical_loads_sub_model_part_list = Parameters["mechanical_loads_sub_model_part_list"]
+        self.body_domain_sub_model_part_list = Parameters["body_domain_sub_model_part_list"]
+        self.body_domain_sub_sub_model_part_list = Parameters["body_domain_sub_sub_model_part_list"]
+        self.loads_sub_model_part_list = Parameters["loads_sub_model_part_list"]
+        self.loads_sub_sub_model_part_list = Parameters["loads_sub_sub_model_part_list"]
+
+    def Execute(self):
+
+        ## Construct the thermal model part:
+        thermal_parts = []
+        for i in range(self.thermal_domain_sub_model_part_list.size()):
+            thermal_parts.append(self.main_model_part.GetSubModelPart(self.thermal_domain_sub_model_part_list[i].GetString()))
+        self.main_model_part.CreateSubModelPart(self.thermal_model_part_name)
+        thermal_model_part = self.main_model_part.GetSubModelPart(self.thermal_model_part_name)
+        thermal_model_part.ProcessInfo = self.main_model_part.ProcessInfo
+        thermal_model_part.Properties = self.main_model_part.Properties
+        thermal_model_part.Set(KratosMultiphysics.ACTIVE)
+        print("Adding Nodes to Thermal Model Part")
+        list_of_ids = set()
+        for part in thermal_parts:
+            for node in part.Nodes:
+                list_of_ids.add(node.Id)
+        thermal_model_part.AddNodes(list(list_of_ids))
+        print("Adding Elements to Thermal Model Part")
+        list_of_ids = set()
+        for part in thermal_parts:
+            for elem in part.Elements:
+                list_of_ids.add(elem.Id)
+        thermal_model_part.AddElements(list(list_of_ids))
+        # Thermal Conditions
+        print("Adding Thermal Conditions to Thermal Model Part")
+        thermal_conditions = []
+        for i in range(self.thermal_loads_sub_model_part_list.size()):
+            thermal_conditions.append(self.main_model_part.GetSubModelPart(self.thermal_loads_sub_model_part_list[i].GetString()))
+        list_of_ids = set()
+        for part in thermal_conditions:
+            for cond in part.Conditions:
+                list_of_ids.add(cond.Id)
+        thermal_model_part.AddConditions(list(list_of_ids))
+        # Sub sub model parts
+        # Construction process
+        print("Adding Thermal Sub Sub Model Parts")
+        for i in range(self.thermal_domain_sub_model_part_list.size()):
+            thermal_sub_model_part = self.main_model_part.GetSubModelPart(self.thermal_domain_sub_model_part_list[i].GetString())
+            thermal_model_part.CreateSubModelPart(self.thermal_domain_sub_sub_model_part_list[i].GetString())
+            thermal_sub_sub_model_part = thermal_model_part.GetSubModelPart(self.thermal_domain_sub_sub_model_part_list[i].GetString())
+            list_of_ids = set()
+            for elem in thermal_sub_model_part.Elements:
+                list_of_ids.add(elem.Id)
+            thermal_sub_sub_model_part.AddElements(list(list_of_ids))
+            list_of_ids = set()
+            for node in thermal_sub_model_part.Nodes:
+                list_of_ids.add(node.Id)
+            thermal_sub_sub_model_part.AddNodes(list(list_of_ids))
+        for i in range(self.thermal_loads_sub_model_part_list.size()):
+            thermal_load_sub_model_part = self.main_model_part.GetSubModelPart(self.thermal_loads_sub_model_part_list[i].GetString())
+            thermal_model_part.CreateSubModelPart(self.thermal_loads_sub_sub_model_part_list[i].GetString())
+            thermal_load_sub_sub_model_part = thermal_model_part.GetSubModelPart(self.thermal_loads_sub_sub_model_part_list[i].GetString())
+            list_of_ids = set()
+            for node in thermal_load_sub_model_part.Nodes:
+                list_of_ids.add(node.Id)
+            thermal_load_sub_sub_model_part.AddNodes(list(list_of_ids))
+            list_of_ids = set()
+            for cond in thermal_load_sub_model_part.Conditions:
+                list_of_ids.add(cond.Id)
+            thermal_load_sub_sub_model_part.AddConditions(list(list_of_ids))
+        print(thermal_model_part)
+
+        ## Construct the mechanical model part:
+        mechanical_parts = []
+        for i in range(self.mechanical_domain_sub_model_part_list.size()):
+            mechanical_parts.append(self.main_model_part.GetSubModelPart(self.mechanical_domain_sub_model_part_list[i].GetString()))
+        self.main_model_part.CreateSubModelPart(self.mechanical_model_part_name)
+        mechanical_model_part = self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
+        mechanical_model_part.ProcessInfo = self.main_model_part.ProcessInfo
+        mechanical_model_part.Properties = self.main_model_part.Properties
+        mechanical_model_part.Set(KratosMultiphysics.ACTIVE)
+        print("Adding Nodes to Mechanical Model Part")
+        list_of_ids = set()
+        for part in mechanical_parts:
+            for node in part.Nodes:
+                list_of_ids.add(node.Id)
+        mechanical_model_part.AddNodes(list(list_of_ids))
+        print("Adding Elements to Mechanical Model Part")
+        list_of_ids = set()
+        for part in mechanical_parts:
+            for elem in part.Elements:
+                list_of_ids.add(elem.Id)
+        mechanical_model_part.AddElements(list(list_of_ids))
+        # Mechanical Conditions
+        print("Adding Conditions to Mechanical Model Part")
+        mechanical_conditions = []
+        for i in range(self.mechanical_loads_sub_model_part_list.size()):
+            mechanical_conditions.append(self.main_model_part.GetSubModelPart(self.mechanical_loads_sub_model_part_list[i].GetString()))
+        list_of_ids = set()
+        for part in mechanical_conditions:
+            for cond in part.Conditions:
+                list_of_ids.add(cond.Id)
+        mechanical_model_part.AddConditions(list(list_of_ids))
+        print("Adding Mechanical Sub Sub Model Parts")
+        # Sub sub model parts
+        # Body - Joints
+        for i in range(self.body_domain_sub_model_part_list.size()):
+            body_sub_model_part = self.main_model_part.GetSubModelPart(self.body_domain_sub_model_part_list[i].GetString())
+            mechanical_model_part.CreateSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
+            body_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
+            list_of_ids = set()
+            for node in body_sub_model_part.Nodes:
+                list_of_ids.add(node.Id)
+            body_sub_sub_model_part.AddNodes(list(list_of_ids))
+            list_of_ids = set()
+            for elem in body_sub_model_part.Elements:
+                list_of_ids.add(elem.Id)
+            body_sub_sub_model_part.AddElements(list(list_of_ids))
+        # Arc-length
+        for i in range(self.loads_sub_model_part_list.size()):
+            load_sub_model_part = self.main_model_part.GetSubModelPart(self.loads_sub_model_part_list[i].GetString())
+            mechanical_model_part.CreateSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
+            load_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
+            list_of_ids = set()
+            for node in load_sub_model_part.Nodes:
+                list_of_ids.add(node.Id)
+            load_sub_sub_model_part.AddNodes(list(list_of_ids))
+            for cond in load_sub_model_part.Conditions:
+                list_of_ids.add(cond.Id)
+            load_sub_sub_model_part.AddConditions(list(list_of_ids))
+        print(mechanical_model_part)
```

## KratosMultiphysics/DamApplication/check_and_prepare_selfweight_model_process_dam.py

 * *Ordering differences only*

```diff
@@ -1,85 +1,85 @@
-import KratosMultiphysics
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return CheckAndPrepareSelfweightModelProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class CheckAndPrepareSelfweightModelProcess(KratosMultiphysics.Process):
-    """Prepare the computing model part.
-
-    The computing model part is created if it does not exist. Nodes and elements
-    from the domain sub model parts are added to the computing model part.
-    Conditions are added from the processes sub model parts.
-    """
-    def __init__(self, main_model_part, Parameters ):
-        KratosMultiphysics.Process.__init__(self)
-        self.main_model_part = main_model_part
-
-        self.mechanical_model_part_name  = Parameters["mechanical_model_part_name"].GetString()
-        self.mechanical_domain_sub_model_part_list = Parameters["mechanical_domain_sub_model_part_list"]
-        self.mechanical_loads_sub_model_part_list = Parameters["mechanical_loads_sub_model_part_list"]
-        self.body_domain_sub_model_part_list = Parameters["body_domain_sub_model_part_list"]
-        self.body_domain_sub_sub_model_part_list = Parameters["body_domain_sub_sub_model_part_list"]
-        self.loads_sub_model_part_list = Parameters["loads_sub_model_part_list"]
-        self.loads_sub_sub_model_part_list = Parameters["loads_sub_sub_model_part_list"]
-
-    def Execute(self):
-
-        ## Construct the mechanical model part:
-        mechanical_parts = []
-        for i in range(self.mechanical_domain_sub_model_part_list.size()):
-            mechanical_parts.append(self.main_model_part.GetSubModelPart(self.mechanical_domain_sub_model_part_list[i].GetString()))
-        self.main_model_part.CreateSubModelPart(self.mechanical_model_part_name)
-        mechanical_model_part = self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
-        mechanical_model_part.ProcessInfo = self.main_model_part.ProcessInfo
-        mechanical_model_part.Properties = self.main_model_part.Properties
-        mechanical_model_part.Set(KratosMultiphysics.ACTIVE)
-        print("Adding Nodes to Mechanical Model Part")
-        list_of_ids = set()
-        for part in mechanical_parts:
-            for node in part.Nodes:
-                list_of_ids.add(node.Id)
-        mechanical_model_part.AddNodes(list(list_of_ids))
-        print("Adding Elements to Mechanical Model Part")
-        list_of_ids = set()
-        for part in mechanical_parts:
-            for elem in part.Elements:
-                list_of_ids.add(elem.Id)
-        mechanical_model_part.AddElements(list(list_of_ids))
-        # Mechanical Conditions
-        print("Adding Conditions to Mechanical Model Part")
-        mechanical_conditions = []
-        for i in range(self.mechanical_loads_sub_model_part_list.size()):
-            mechanical_conditions.append(self.main_model_part.GetSubModelPart(self.mechanical_loads_sub_model_part_list[i].GetString()))
-        list_of_ids = set()
-        for part in mechanical_conditions:
-            for cond in part.Conditions:
-                list_of_ids.add(cond.Id)
-        mechanical_model_part.AddConditions(list(list_of_ids))
-        print("Adding Mechanical Sub Sub Model Parts")
-        # Sub sub model parts
-        # Body - Joints
-        for i in range(self.body_domain_sub_model_part_list.size()):
-            body_sub_model_part = self.main_model_part.GetSubModelPart(self.body_domain_sub_model_part_list[i].GetString())
-            mechanical_model_part.CreateSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
-            body_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
-            list_of_ids = set()
-            for node in body_sub_model_part.Nodes:
-                list_of_ids.add(node.Id)
-            body_sub_sub_model_part.AddNodes(list(list_of_ids))
-            list_of_ids = set()
-            for elem in body_sub_model_part.Elements:
-                list_of_ids.add(elem.Id)
-            body_sub_sub_model_part.AddElements(list(list_of_ids))
-        # Arc-length
-        for i in range(self.loads_sub_model_part_list.size()):
-            load_sub_model_part = self.main_model_part.GetSubModelPart(self.loads_sub_model_part_list[i].GetString())
-            mechanical_model_part.CreateSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
-            load_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
-            list_of_ids = set()
-            for node in load_sub_model_part.Nodes:
-                list_of_ids.add(node.Id)
-            load_sub_sub_model_part.AddNodes(list(list_of_ids))
-        print(mechanical_model_part)
+import KratosMultiphysics
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return CheckAndPrepareSelfweightModelProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class CheckAndPrepareSelfweightModelProcess(KratosMultiphysics.Process):
+    """Prepare the computing model part.
+
+    The computing model part is created if it does not exist. Nodes and elements
+    from the domain sub model parts are added to the computing model part.
+    Conditions are added from the processes sub model parts.
+    """
+    def __init__(self, main_model_part, Parameters ):
+        KratosMultiphysics.Process.__init__(self)
+        self.main_model_part = main_model_part
+
+        self.mechanical_model_part_name  = Parameters["mechanical_model_part_name"].GetString()
+        self.mechanical_domain_sub_model_part_list = Parameters["mechanical_domain_sub_model_part_list"]
+        self.mechanical_loads_sub_model_part_list = Parameters["mechanical_loads_sub_model_part_list"]
+        self.body_domain_sub_model_part_list = Parameters["body_domain_sub_model_part_list"]
+        self.body_domain_sub_sub_model_part_list = Parameters["body_domain_sub_sub_model_part_list"]
+        self.loads_sub_model_part_list = Parameters["loads_sub_model_part_list"]
+        self.loads_sub_sub_model_part_list = Parameters["loads_sub_sub_model_part_list"]
+
+    def Execute(self):
+
+        ## Construct the mechanical model part:
+        mechanical_parts = []
+        for i in range(self.mechanical_domain_sub_model_part_list.size()):
+            mechanical_parts.append(self.main_model_part.GetSubModelPart(self.mechanical_domain_sub_model_part_list[i].GetString()))
+        self.main_model_part.CreateSubModelPart(self.mechanical_model_part_name)
+        mechanical_model_part = self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
+        mechanical_model_part.ProcessInfo = self.main_model_part.ProcessInfo
+        mechanical_model_part.Properties = self.main_model_part.Properties
+        mechanical_model_part.Set(KratosMultiphysics.ACTIVE)
+        print("Adding Nodes to Mechanical Model Part")
+        list_of_ids = set()
+        for part in mechanical_parts:
+            for node in part.Nodes:
+                list_of_ids.add(node.Id)
+        mechanical_model_part.AddNodes(list(list_of_ids))
+        print("Adding Elements to Mechanical Model Part")
+        list_of_ids = set()
+        for part in mechanical_parts:
+            for elem in part.Elements:
+                list_of_ids.add(elem.Id)
+        mechanical_model_part.AddElements(list(list_of_ids))
+        # Mechanical Conditions
+        print("Adding Conditions to Mechanical Model Part")
+        mechanical_conditions = []
+        for i in range(self.mechanical_loads_sub_model_part_list.size()):
+            mechanical_conditions.append(self.main_model_part.GetSubModelPart(self.mechanical_loads_sub_model_part_list[i].GetString()))
+        list_of_ids = set()
+        for part in mechanical_conditions:
+            for cond in part.Conditions:
+                list_of_ids.add(cond.Id)
+        mechanical_model_part.AddConditions(list(list_of_ids))
+        print("Adding Mechanical Sub Sub Model Parts")
+        # Sub sub model parts
+        # Body - Joints
+        for i in range(self.body_domain_sub_model_part_list.size()):
+            body_sub_model_part = self.main_model_part.GetSubModelPart(self.body_domain_sub_model_part_list[i].GetString())
+            mechanical_model_part.CreateSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
+            body_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.body_domain_sub_sub_model_part_list[i].GetString())
+            list_of_ids = set()
+            for node in body_sub_model_part.Nodes:
+                list_of_ids.add(node.Id)
+            body_sub_sub_model_part.AddNodes(list(list_of_ids))
+            list_of_ids = set()
+            for elem in body_sub_model_part.Elements:
+                list_of_ids.add(elem.Id)
+            body_sub_sub_model_part.AddElements(list(list_of_ids))
+        # Arc-length
+        for i in range(self.loads_sub_model_part_list.size()):
+            load_sub_model_part = self.main_model_part.GetSubModelPart(self.loads_sub_model_part_list[i].GetString())
+            mechanical_model_part.CreateSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
+            load_sub_sub_model_part = mechanical_model_part.GetSubModelPart(self.loads_sub_sub_model_part_list[i].GetString())
+            list_of_ids = set()
+            for node in load_sub_model_part.Nodes:
+                list_of_ids.add(node.Id)
+            load_sub_sub_model_part.AddNodes(list(list_of_ids))
+        print(mechanical_model_part)
```

## KratosMultiphysics/DamApplication/dam_P_solver.py

 * *Ordering differences only*

```diff
@@ -1,164 +1,164 @@
-# importing the Kratos Library
-import KratosMultiphysics
-# import KratosMultiphysics.ExternalSolversApplication as KratosExternal
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-import KratosMultiphysics.DamApplication as KratosDam
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-
-def CreateSolver(main_model_part, custom_settings):
-    return DamUPSolver(main_model_part, custom_settings)
-
-class DamUPSolver:
-    def __init__(self, model_part, custom_settings):
-
-        self.main_model_part = model_part
-
-        ##settings string in json format
-        default_settings = KratosMultiphysics.Parameters("""
-        {
-            "solver_type"                   : "dam_P_solver",
-            "model_import_settings"         : {
-                "input_type"       : "mdpa",
-                "input_filename"   : "unknown_name",
-                "input_file_label" : 0
-            },
-            "echo_level"                    : 1,
-            "buffer_size"                   : 2,
-            "processes_sub_model_part_list" : [""],
-            "acoustic_solver_settings"      : {
-                "strategy_type"               : "Newton-Raphson",
-                "scheme_type"                 : "Newmark",
-                "convergence_criterion"       : "Residual_criterion",
-                "residual_relative_tolerance" : 0.0001,
-                "residual_absolute_tolerance" : 1e-9,
-                "max_iteration"               : 10,
-                "move_mesh_flag"              : false,
-                "echo_level"                  : 0,
-                "linear_solver_settings"      : {
-                    "solver_type"   : "amgcl",
-                    "max_iteration" : 200,
-                    "tolerance"     : 1e-7,
-                    "verbosity"     : 0,
-                    "GMRES_size"    : 50
-                    }
-            }
-         }""")
-
-        ##overwrite the default settings with user-provided parameters
-        self.settings = custom_settings
-        self.settings.ValidateAndAssignDefaults(default_settings)
-
-        ## Definition of the linear solver
-        amgcl_smoother = KratosMultiphysics.AMGCLSmoother.ILU0
-        amgcl_krylov_type = KratosMultiphysics.AMGCLIterativeSolverType.BICGSTAB
-        tolerance = self.settings["acoustic_solver_settings"]["linear_solver_settings"]["tolerance"].GetDouble()
-        max_iterations = self.settings["acoustic_solver_settings"]["linear_solver_settings"]["max_iteration"].GetInt()
-        verbosity = self.settings["acoustic_solver_settings"]["linear_solver_settings"]["verbosity"].GetInt()
-        gmres_size = self.settings["acoustic_solver_settings"]["linear_solver_settings"]["GMRES_size"].GetInt()
-
-        self.linear_solver =  KratosMultiphysics.AMGCLSolver(amgcl_smoother,amgcl_krylov_type,tolerance,max_iterations,verbosity,gmres_size)
-
-
-    def AddVariables(self):
-        ## Add pressure
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PRESSURE)
-        ## Add Dynamic pressure Variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt_PRESSURE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt2_PRESSURE)
-
-        print("Variables correctly added")
-
-
-    def AddDofs(self):
-        for node in self.main_model_part.Nodes:
-            # adding dofs
-            node.AddDof(KratosMultiphysics.PRESSURE)
-
-        print("P DOFs correctly added")
-
-    def Initialize(self):
-
-        if (self.settings["acoustic_solver_settings"]["scheme_type"].GetString() == "Newmark"):
-            beta=0.25
-            gamma=0.5
-        else:
-            raise Exception("Please use the Newmark Scheme, it is the only one available")
-
-        move_mesh_flag = self.settings["acoustic_solver_settings"]["move_mesh_flag"].GetBool()
-        max_iterations = self.settings["acoustic_solver_settings"]["max_iteration"].GetInt()
-        res_rel_tol = self.settings["acoustic_solver_settings"]["residual_relative_tolerance"].GetDouble()
-        res_abs_tol = self.settings["acoustic_solver_settings"]["residual_absolute_tolerance"].GetDouble()
-
-        time_scheme = KratosDam.DamPScheme(beta,gamma)
-        conv_criteria = KratosMultiphysics.ResidualCriteria(res_rel_tol,res_abs_tol)
-
-        self.solver = KratosMultiphysics.ResidualBasedNewtonRaphsonStrategy(
-            self.main_model_part,
-            time_scheme,
-            self.linear_solver,
-            conv_criteria,
-            max_iterations,
-            False,
-            False,
-            move_mesh_flag)
-
-
-        (self.solver).SetEchoLevel(self.settings["acoustic_solver_settings"]["echo_level"].GetInt())
-
-        print ("Initialization Solver finished")
-
-    def ImportModelPart(self):
-
-        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
-
-            # Here it would be the place to import restart data if required
-            KratosMultiphysics.ModelPartIO(self.settings["model_import_settings"]["input_filename"].GetString()).ReadModelPart(self.main_model_part)
-
-            # Create computing_model_part, set constitutive law and buffer size
-            self._ExecuteAfterReading()
-
-        else:
-            raise Exception("other input options are not yet implemented")
-
-        print ("model reading finished")
-
-
-    def GetMinimumBufferSize(self):
-        return 2;
-
-    def GetComputingModelPart(self):
-        return self.main_model_part
-
-    def Solve(self):
-        (self.solver).Solve()
-
-    def SetEchoLevel(self, level):
-        (self.solver).SetEchoLevel(level)
-
-    def Clear(self):
-        (self.solver).Clear()
-
-
-    #### Specific internal functions ####
-
-    def _ExecuteAfterReading(self):
-
-        self.computing_model_part_name = "acoustic_computing_domain"
-
-        # Auxiliary Kratos parameters object to be called by the CheckAndPepareModelProcess
-        aux_params = KratosMultiphysics.Parameters("{}")
-        aux_params.AddEmptyValue("computing_model_part_name").SetString(self.computing_model_part_name)
-
-        # CheckAndPrepareModelProcess creates the solid_computational_model_part
-        from KratosMultiphysics.PoromechanicsApplication import check_and_prepare_model_process_poro
-        check_and_prepare_model_process_poro.CheckAndPrepareModelProcess(self.main_model_part, aux_params).Execute()
-
-        # Constitutive law import
-        from KratosMultiphysics.DamApplication import dam_constitutive_law_utility
-        dam_constitutive_law_utility.SetConstitutiveLaw(self.main_model_part)
-
-        self.main_model_part.SetBufferSize( self.settings["buffer_size"].GetInt() )
-        minimum_buffer_size = self.GetMinimumBufferSize()
-        if(minimum_buffer_size > self.main_model_part.GetBufferSize()):
-            self.main_model_part.SetBufferSize( minimum_buffer_size )
-
+# importing the Kratos Library
+import KratosMultiphysics
+# import KratosMultiphysics.ExternalSolversApplication as KratosExternal
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+import KratosMultiphysics.DamApplication as KratosDam
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+
+def CreateSolver(main_model_part, custom_settings):
+    return DamUPSolver(main_model_part, custom_settings)
+
+class DamUPSolver:
+    def __init__(self, model_part, custom_settings):
+
+        self.main_model_part = model_part
+
+        ##settings string in json format
+        default_settings = KratosMultiphysics.Parameters("""
+        {
+            "solver_type"                   : "dam_P_solver",
+            "model_import_settings"         : {
+                "input_type"       : "mdpa",
+                "input_filename"   : "unknown_name",
+                "input_file_label" : 0
+            },
+            "echo_level"                    : 1,
+            "buffer_size"                   : 2,
+            "processes_sub_model_part_list" : [""],
+            "acoustic_solver_settings"      : {
+                "strategy_type"               : "Newton-Raphson",
+                "scheme_type"                 : "Newmark",
+                "convergence_criterion"       : "Residual_criterion",
+                "residual_relative_tolerance" : 0.0001,
+                "residual_absolute_tolerance" : 1e-9,
+                "max_iteration"               : 10,
+                "move_mesh_flag"              : false,
+                "echo_level"                  : 0,
+                "linear_solver_settings"      : {
+                    "solver_type"   : "amgcl",
+                    "max_iteration" : 200,
+                    "tolerance"     : 1e-7,
+                    "verbosity"     : 0,
+                    "GMRES_size"    : 50
+                    }
+            }
+         }""")
+
+        ##overwrite the default settings with user-provided parameters
+        self.settings = custom_settings
+        self.settings.ValidateAndAssignDefaults(default_settings)
+
+        ## Definition of the linear solver
+        amgcl_smoother = KratosMultiphysics.AMGCLSmoother.ILU0
+        amgcl_krylov_type = KratosMultiphysics.AMGCLIterativeSolverType.BICGSTAB
+        tolerance = self.settings["acoustic_solver_settings"]["linear_solver_settings"]["tolerance"].GetDouble()
+        max_iterations = self.settings["acoustic_solver_settings"]["linear_solver_settings"]["max_iteration"].GetInt()
+        verbosity = self.settings["acoustic_solver_settings"]["linear_solver_settings"]["verbosity"].GetInt()
+        gmres_size = self.settings["acoustic_solver_settings"]["linear_solver_settings"]["GMRES_size"].GetInt()
+
+        self.linear_solver =  KratosMultiphysics.AMGCLSolver(amgcl_smoother,amgcl_krylov_type,tolerance,max_iterations,verbosity,gmres_size)
+
+
+    def AddVariables(self):
+        ## Add pressure
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PRESSURE)
+        ## Add Dynamic pressure Variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt_PRESSURE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt2_PRESSURE)
+
+        print("Variables correctly added")
+
+
+    def AddDofs(self):
+        for node in self.main_model_part.Nodes:
+            # adding dofs
+            node.AddDof(KratosMultiphysics.PRESSURE)
+
+        print("P DOFs correctly added")
+
+    def Initialize(self):
+
+        if (self.settings["acoustic_solver_settings"]["scheme_type"].GetString() == "Newmark"):
+            beta=0.25
+            gamma=0.5
+        else:
+            raise Exception("Please use the Newmark Scheme, it is the only one available")
+
+        move_mesh_flag = self.settings["acoustic_solver_settings"]["move_mesh_flag"].GetBool()
+        max_iterations = self.settings["acoustic_solver_settings"]["max_iteration"].GetInt()
+        res_rel_tol = self.settings["acoustic_solver_settings"]["residual_relative_tolerance"].GetDouble()
+        res_abs_tol = self.settings["acoustic_solver_settings"]["residual_absolute_tolerance"].GetDouble()
+
+        time_scheme = KratosDam.DamPScheme(beta,gamma)
+        conv_criteria = KratosMultiphysics.ResidualCriteria(res_rel_tol,res_abs_tol)
+
+        self.solver = KratosMultiphysics.ResidualBasedNewtonRaphsonStrategy(
+            self.main_model_part,
+            time_scheme,
+            self.linear_solver,
+            conv_criteria,
+            max_iterations,
+            False,
+            False,
+            move_mesh_flag)
+
+
+        (self.solver).SetEchoLevel(self.settings["acoustic_solver_settings"]["echo_level"].GetInt())
+
+        print ("Initialization Solver finished")
+
+    def ImportModelPart(self):
+
+        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
+
+            # Here it would be the place to import restart data if required
+            KratosMultiphysics.ModelPartIO(self.settings["model_import_settings"]["input_filename"].GetString()).ReadModelPart(self.main_model_part)
+
+            # Create computing_model_part, set constitutive law and buffer size
+            self._ExecuteAfterReading()
+
+        else:
+            raise Exception("other input options are not yet implemented")
+
+        print ("model reading finished")
+
+
+    def GetMinimumBufferSize(self):
+        return 2;
+
+    def GetComputingModelPart(self):
+        return self.main_model_part
+
+    def Solve(self):
+        (self.solver).Solve()
+
+    def SetEchoLevel(self, level):
+        (self.solver).SetEchoLevel(level)
+
+    def Clear(self):
+        (self.solver).Clear()
+
+
+    #### Specific internal functions ####
+
+    def _ExecuteAfterReading(self):
+
+        self.computing_model_part_name = "acoustic_computing_domain"
+
+        # Auxiliary Kratos parameters object to be called by the CheckAndPepareModelProcess
+        aux_params = KratosMultiphysics.Parameters("{}")
+        aux_params.AddEmptyValue("computing_model_part_name").SetString(self.computing_model_part_name)
+
+        # CheckAndPrepareModelProcess creates the solid_computational_model_part
+        from KratosMultiphysics.PoromechanicsApplication import check_and_prepare_model_process_poro
+        check_and_prepare_model_process_poro.CheckAndPrepareModelProcess(self.main_model_part, aux_params).Execute()
+
+        # Constitutive law import
+        from KratosMultiphysics.DamApplication import dam_constitutive_law_utility
+        dam_constitutive_law_utility.SetConstitutiveLaw(self.main_model_part)
+
+        self.main_model_part.SetBufferSize( self.settings["buffer_size"].GetInt() )
+        minimum_buffer_size = self.GetMinimumBufferSize()
+        if(minimum_buffer_size > self.main_model_part.GetBufferSize()):
+            self.main_model_part.SetBufferSize( minimum_buffer_size )
+
```

## KratosMultiphysics/DamApplication/dam_UP_mechanical_solver.py

 * *Ordering differences only*

```diff
@@ -1,128 +1,128 @@
-#import kratos core and applications
-import KratosMultiphysics
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-import KratosMultiphysics.DamApplication as KratosDam
-
-from KratosMultiphysics.DamApplication import dam_mechanical_solver
-
-
-def CreateSolver(main_model_part, custom_settings):
-
-    return DamUPMechanicalSolver(main_model_part, custom_settings)
-
-
-class DamUPMechanicalSolver(dam_mechanical_solver.DamMechanicalSolver):
-
-    def __init__(self, main_model_part, custom_settings):
-
-        #TODO: shall obtain the computing_model_part from the MODEL once the object is implemented
-        self.main_model_part = main_model_part
-
-        ##settings string in json format
-        default_settings = KratosMultiphysics.Parameters("""
-        {
-            "solver_type": "dam_UP_mechanical_solver",
-            "model_import_settings":{
-                "input_type": "mdpa",
-                "input_filename": "unknown_name",
-                "input_file_label": 0
-            },
-            "buffer_size": 2,
-            "echo_level": 0,
-            "processes_sub_model_part_list": [""],
-            "mechanical_solver_settings":{
-                "echo_level": 0,
-                "reform_dofs_at_each_step": false,
-                "clear_storage": false,
-                "compute_reactions": false,
-                "move_mesh_flag": true,
-                "solution_type": "Quasi-Static",
-                "scheme_type": "Newmark",
-                "rayleigh_m": 0.0,
-                "rayleigh_k": 0.0,
-                "strategy_type": "Newton-Raphson",
-                "convergence_criterion": "Displacement_criterion",
-                "displacement_relative_tolerance": 1.0e-4,
-                "displacement_absolute_tolerance": 1.0e-9,
-                "residual_relative_tolerance": 1.0e-4,
-                "residual_absolute_tolerance": 1.0e-9,
-                "max_iteration": 15,
-                "desired_iterations": 4,
-                "max_radius_factor": 20.0,
-                "min_radius_factor": 0.5,
-                "block_builder": true,
-                "nonlocal_damage": false,
-                "characteristic_length": 0.05,
-                "search_neighbours_step": false,
-                "linear_solver_settings":{
-                    "solver_type": "amgcl",
-                    "tolerance": 1.0e-6,
-                    "max_iteration": 100,
-                    "scaling": false,
-                    "verbosity": 0,
-                    "preconditioner_type": "ilu0",
-                    "smoother_type": "ilu0",
-                    "krylov_type": "gmres",
-                    "coarsening_type": "aggregation"
-                },
-                "problem_domain_sub_model_part_list": [""],
-                "body_domain_sub_model_part_list": [],
-                "mechanical_loads_sub_model_part_list": [],
-                "loads_sub_model_part_list": [],
-                "loads_variable_list": []
-            }
-        }
-        """)
-
-        # Overwrite the default settings with user-provided parameters
-        self.settings = custom_settings
-        self.settings.ValidateAndAssignDefaults(default_settings)
-
-        # Construct the linear solver
-        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
-        self.linear_solver = linear_solver_factory.ConstructSolver(self.settings["mechanical_solver_settings"]["linear_solver_settings"])
-
-        print("Construction of DamUPMechanicalSolver finished")
-
-    def AddVariables(self):
-
-        super(DamUPMechanicalSolver, self).AddVariables()
-
-        ## Fluid variables
-        # Add pressure
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PRESSURE)
-        # Add Dynamic pressure variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt_PRESSURE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt2_PRESSURE)
-
-    def AddDofs(self):
-
-        for node in self.main_model_part.Nodes:
-            ## Solid dofs
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_X,KratosMultiphysics.REACTION_X)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y,KratosMultiphysics.REACTION_Y)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z,KratosMultiphysics.REACTION_Z)
-            ## Fluid dofs
-            node.AddDof(KratosMultiphysics.PRESSURE)
-            # adding VELOCITY as dofs
-            node.AddDof(KratosMultiphysics.VELOCITY_X)
-            node.AddDof(KratosMultiphysics.VELOCITY_Y)
-            node.AddDof(KratosMultiphysics.VELOCITY_Z)
-            # adding ACCELERATION as dofs
-            node.AddDof(KratosMultiphysics.ACCELERATION_X)
-            node.AddDof(KratosMultiphysics.ACCELERATION_Y)
-            node.AddDof(KratosMultiphysics.ACCELERATION_Z)
-
-    #### Specific internal functions ####
-
-    def _ConstructScheme(self, scheme_type, solution_type):
-
-        rayleigh_m = self.settings["mechanical_solver_settings"]["rayleigh_m"].GetDouble()
-        rayleigh_k = self.settings["mechanical_solver_settings"]["rayleigh_k"].GetDouble()
-
-        beta=0.25
-        gamma=0.5
-        scheme = KratosDam.DamUPScheme(beta,gamma,rayleigh_m,rayleigh_k)
-
-        return scheme
+#import kratos core and applications
+import KratosMultiphysics
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+import KratosMultiphysics.DamApplication as KratosDam
+
+from KratosMultiphysics.DamApplication import dam_mechanical_solver
+
+
+def CreateSolver(main_model_part, custom_settings):
+
+    return DamUPMechanicalSolver(main_model_part, custom_settings)
+
+
+class DamUPMechanicalSolver(dam_mechanical_solver.DamMechanicalSolver):
+
+    def __init__(self, main_model_part, custom_settings):
+
+        #TODO: shall obtain the computing_model_part from the MODEL once the object is implemented
+        self.main_model_part = main_model_part
+
+        ##settings string in json format
+        default_settings = KratosMultiphysics.Parameters("""
+        {
+            "solver_type": "dam_UP_mechanical_solver",
+            "model_import_settings":{
+                "input_type": "mdpa",
+                "input_filename": "unknown_name",
+                "input_file_label": 0
+            },
+            "buffer_size": 2,
+            "echo_level": 0,
+            "processes_sub_model_part_list": [""],
+            "mechanical_solver_settings":{
+                "echo_level": 0,
+                "reform_dofs_at_each_step": false,
+                "clear_storage": false,
+                "compute_reactions": false,
+                "move_mesh_flag": true,
+                "solution_type": "Quasi-Static",
+                "scheme_type": "Newmark",
+                "rayleigh_m": 0.0,
+                "rayleigh_k": 0.0,
+                "strategy_type": "Newton-Raphson",
+                "convergence_criterion": "Displacement_criterion",
+                "displacement_relative_tolerance": 1.0e-4,
+                "displacement_absolute_tolerance": 1.0e-9,
+                "residual_relative_tolerance": 1.0e-4,
+                "residual_absolute_tolerance": 1.0e-9,
+                "max_iteration": 15,
+                "desired_iterations": 4,
+                "max_radius_factor": 20.0,
+                "min_radius_factor": 0.5,
+                "block_builder": true,
+                "nonlocal_damage": false,
+                "characteristic_length": 0.05,
+                "search_neighbours_step": false,
+                "linear_solver_settings":{
+                    "solver_type": "amgcl",
+                    "tolerance": 1.0e-6,
+                    "max_iteration": 100,
+                    "scaling": false,
+                    "verbosity": 0,
+                    "preconditioner_type": "ilu0",
+                    "smoother_type": "ilu0",
+                    "krylov_type": "gmres",
+                    "coarsening_type": "aggregation"
+                },
+                "problem_domain_sub_model_part_list": [""],
+                "body_domain_sub_model_part_list": [],
+                "mechanical_loads_sub_model_part_list": [],
+                "loads_sub_model_part_list": [],
+                "loads_variable_list": []
+            }
+        }
+        """)
+
+        # Overwrite the default settings with user-provided parameters
+        self.settings = custom_settings
+        self.settings.ValidateAndAssignDefaults(default_settings)
+
+        # Construct the linear solver
+        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
+        self.linear_solver = linear_solver_factory.ConstructSolver(self.settings["mechanical_solver_settings"]["linear_solver_settings"])
+
+        print("Construction of DamUPMechanicalSolver finished")
+
+    def AddVariables(self):
+
+        super(DamUPMechanicalSolver, self).AddVariables()
+
+        ## Fluid variables
+        # Add pressure
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PRESSURE)
+        # Add Dynamic pressure variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt_PRESSURE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt2_PRESSURE)
+
+    def AddDofs(self):
+
+        for node in self.main_model_part.Nodes:
+            ## Solid dofs
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_X,KratosMultiphysics.REACTION_X)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y,KratosMultiphysics.REACTION_Y)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z,KratosMultiphysics.REACTION_Z)
+            ## Fluid dofs
+            node.AddDof(KratosMultiphysics.PRESSURE)
+            # adding VELOCITY as dofs
+            node.AddDof(KratosMultiphysics.VELOCITY_X)
+            node.AddDof(KratosMultiphysics.VELOCITY_Y)
+            node.AddDof(KratosMultiphysics.VELOCITY_Z)
+            # adding ACCELERATION as dofs
+            node.AddDof(KratosMultiphysics.ACCELERATION_X)
+            node.AddDof(KratosMultiphysics.ACCELERATION_Y)
+            node.AddDof(KratosMultiphysics.ACCELERATION_Z)
+
+    #### Specific internal functions ####
+
+    def _ConstructScheme(self, scheme_type, solution_type):
+
+        rayleigh_m = self.settings["mechanical_solver_settings"]["rayleigh_m"].GetDouble()
+        rayleigh_k = self.settings["mechanical_solver_settings"]["rayleigh_k"].GetDouble()
+
+        beta=0.25
+        gamma=0.5
+        scheme = KratosDam.DamUPScheme(beta,gamma,rayleigh_m,rayleigh_k)
+
+        return scheme
```

## KratosMultiphysics/DamApplication/dam_UP_thermo_mechanic_solver.py

 * *Ordering differences only*

```diff
@@ -1,156 +1,156 @@
-#import kratos core and applications
-import KratosMultiphysics
-import KratosMultiphysics.ConvectionDiffusionApplication as KratosConvDiff
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-import KratosMultiphysics.DamApplication as KratosDam
-
-import dam_thermo_mechanic_solver
-
-
-def CreateSolver(main_model_part, custom_settings):
-
-    return DamUPThermoMechanicSolver(main_model_part, custom_settings)
-
-
-class DamUPThermoMechanicSolver(dam_thermo_mechanic_solver.DamThermoMechanicSolver):
-
-    def __init__(self, main_model_part, custom_settings):
-
-        #TODO: shall obtain the computing_model_part from the MODEL once the object is implemented
-        self.main_model_part = main_model_part
-
-        ##settings string in json format
-        default_settings = KratosMultiphysics.Parameters("""
-        {
-            "solver_type": "dam_UP_thermo_mechanic_solver",
-            "model_import_settings":{
-                "input_type": "mdpa",
-                "input_filename": "unknown_name",
-                "input_file_label": 0
-            },
-            "echo_level": 0,
-            "buffer_size": 2,
-            "reference_temperature" : 10.0,
-            "processes_sub_model_part_list": [""],
-            "thermal_solver_settings":{
-                "echo_level": 0,
-                "reform_dofs_at_each_step": false,
-                "clear_storage": false,
-                "compute_reactions": false,
-                "move_mesh_flag": true,
-                "compute_norm_dx_flag": false,
-                "theta_scheme": 1.0,
-                "block_builder": true,
-                "linear_solver_settings":{
-                    "solver_type": "amgcl",
-                    "tolerance": 1.0e-6,
-                    "max_iteration": 100,
-                    "scaling": false,
-                    "verbosity": 0,
-                    "preconditioner_type": "ilu0",
-                    "smoother_type": "ilu0",
-                    "krylov_type": "gmres",
-                    "coarsening_type": "aggregation"
-                },
-                "problem_domain_sub_model_part_list": [""],
-                "thermal_loads_sub_model_part_list": []
-            },
-            "mechanical_solver_settings":{
-                "echo_level": 0,
-                "reform_dofs_at_each_step": false,
-                "clear_storage": false,
-                "compute_reactions": false,
-                "move_mesh_flag": true,
-                "solution_type": "Dynamic",
-                "scheme_type": "Newmark",
-                "rayleigh_m": 0.0,
-                "rayleigh_k": 0.0,
-                "strategy_type": "Newton-Raphson",
-                "convergence_criterion": "Displacement_criterion",
-                "displacement_relative_tolerance": 1.0e-4,
-                "displacement_absolute_tolerance": 1.0e-9,
-                "residual_relative_tolerance": 1.0e-4,
-                "residual_absolute_tolerance": 1.0e-9,
-                "max_iteration": 15,
-                "desired_iterations": 4,
-                "max_radius_factor": 20.0,
-                "min_radius_factor": 0.5,
-                "block_builder": true,
-                "nonlocal_damage": false,
-                "characteristic_length": 0.05,
-                "search_neighbours_step": false,
-                "linear_solver_settings":{
-                    "solver_type": "amgcl",
-                    "tolerance": 1.0e-6,
-                    "max_iteration": 100,
-                    "scaling": false,
-                    "verbosity": 0,
-                    "preconditioner_type": "ilu0",
-                    "smoother_type": "ilu0",
-                    "krylov_type": "gmres",
-                    "coarsening_type": "aggregation"
-                },
-                "problem_domain_sub_model_part_list": [""],
-                "body_domain_sub_model_part_list": [],
-                "mechanical_loads_sub_model_part_list": [],
-                "loads_sub_model_part_list": [],
-                "loads_variable_list": []
-            }
-        }
-        """)
-
-        # Overwrite the default settings with user-provided parameters
-        self.settings = custom_settings
-        self.settings.ValidateAndAssignDefaults(default_settings)
-
-        # Construct the linear solver
-        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
-        self.thermal_linear_solver = linear_solver_factory.ConstructSolver(self.settings["thermal_solver_settings"]["linear_solver_settings"])
-        self.mechanical_linear_solver = linear_solver_factory.ConstructSolver(self.settings["mechanical_solver_settings"]["linear_solver_settings"])
-
-        print("Construction of DamUPThermoMechanicSolver finished")
-
-    def AddVariables(self):
-
-        super(DamUPThermoMechanicSolver, self).AddVariables()
-
-        ## Fluid variables
-        # Add pressure
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PRESSURE)
-        # Add Dynamic pressure variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt_PRESSURE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt2_PRESSURE)
-
-    def AddDofs(self):
-
-        for node in self.main_model_part.Nodes:
-            ## Solid dofs
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_X,KratosMultiphysics.REACTION_X)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y,KratosMultiphysics.REACTION_Y)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z,KratosMultiphysics.REACTION_Z)
-            ## Fluid dofs
-            node.AddDof(KratosMultiphysics.PRESSURE)
-            ## Thermal dofs
-            node.AddDof(KratosMultiphysics.TEMPERATURE)
-            # adding VELOCITY as dofs
-            node.AddDof(KratosMultiphysics.VELOCITY_X)
-            node.AddDof(KratosMultiphysics.VELOCITY_Y)
-            node.AddDof(KratosMultiphysics.VELOCITY_Z)
-            # adding ACCELERATION as dofs
-            node.AddDof(KratosMultiphysics.ACCELERATION_X)
-            node.AddDof(KratosMultiphysics.ACCELERATION_Y)
-            node.AddDof(KratosMultiphysics.ACCELERATION_Z)
-
-    #### Specific internal functions ####
-
-    def _ConstructScheme(self, scheme_type, solution_type):
-
-        rayleigh_m = self.settings["mechanical_solver_settings"]["rayleigh_m"].GetDouble()
-        rayleigh_k = self.settings["mechanical_solver_settings"]["rayleigh_k"].GetDouble()
-
-        beta=0.25
-        gamma=0.5
-        scheme = KratosDam.DamUPScheme(beta,gamma,rayleigh_m,rayleigh_k)
-
-        return scheme
+#import kratos core and applications
+import KratosMultiphysics
+import KratosMultiphysics.ConvectionDiffusionApplication as KratosConvDiff
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+import KratosMultiphysics.DamApplication as KratosDam
+
+import dam_thermo_mechanic_solver
+
+
+def CreateSolver(main_model_part, custom_settings):
+
+    return DamUPThermoMechanicSolver(main_model_part, custom_settings)
+
+
+class DamUPThermoMechanicSolver(dam_thermo_mechanic_solver.DamThermoMechanicSolver):
+
+    def __init__(self, main_model_part, custom_settings):
+
+        #TODO: shall obtain the computing_model_part from the MODEL once the object is implemented
+        self.main_model_part = main_model_part
+
+        ##settings string in json format
+        default_settings = KratosMultiphysics.Parameters("""
+        {
+            "solver_type": "dam_UP_thermo_mechanic_solver",
+            "model_import_settings":{
+                "input_type": "mdpa",
+                "input_filename": "unknown_name",
+                "input_file_label": 0
+            },
+            "echo_level": 0,
+            "buffer_size": 2,
+            "reference_temperature" : 10.0,
+            "processes_sub_model_part_list": [""],
+            "thermal_solver_settings":{
+                "echo_level": 0,
+                "reform_dofs_at_each_step": false,
+                "clear_storage": false,
+                "compute_reactions": false,
+                "move_mesh_flag": true,
+                "compute_norm_dx_flag": false,
+                "theta_scheme": 1.0,
+                "block_builder": true,
+                "linear_solver_settings":{
+                    "solver_type": "amgcl",
+                    "tolerance": 1.0e-6,
+                    "max_iteration": 100,
+                    "scaling": false,
+                    "verbosity": 0,
+                    "preconditioner_type": "ilu0",
+                    "smoother_type": "ilu0",
+                    "krylov_type": "gmres",
+                    "coarsening_type": "aggregation"
+                },
+                "problem_domain_sub_model_part_list": [""],
+                "thermal_loads_sub_model_part_list": []
+            },
+            "mechanical_solver_settings":{
+                "echo_level": 0,
+                "reform_dofs_at_each_step": false,
+                "clear_storage": false,
+                "compute_reactions": false,
+                "move_mesh_flag": true,
+                "solution_type": "Dynamic",
+                "scheme_type": "Newmark",
+                "rayleigh_m": 0.0,
+                "rayleigh_k": 0.0,
+                "strategy_type": "Newton-Raphson",
+                "convergence_criterion": "Displacement_criterion",
+                "displacement_relative_tolerance": 1.0e-4,
+                "displacement_absolute_tolerance": 1.0e-9,
+                "residual_relative_tolerance": 1.0e-4,
+                "residual_absolute_tolerance": 1.0e-9,
+                "max_iteration": 15,
+                "desired_iterations": 4,
+                "max_radius_factor": 20.0,
+                "min_radius_factor": 0.5,
+                "block_builder": true,
+                "nonlocal_damage": false,
+                "characteristic_length": 0.05,
+                "search_neighbours_step": false,
+                "linear_solver_settings":{
+                    "solver_type": "amgcl",
+                    "tolerance": 1.0e-6,
+                    "max_iteration": 100,
+                    "scaling": false,
+                    "verbosity": 0,
+                    "preconditioner_type": "ilu0",
+                    "smoother_type": "ilu0",
+                    "krylov_type": "gmres",
+                    "coarsening_type": "aggregation"
+                },
+                "problem_domain_sub_model_part_list": [""],
+                "body_domain_sub_model_part_list": [],
+                "mechanical_loads_sub_model_part_list": [],
+                "loads_sub_model_part_list": [],
+                "loads_variable_list": []
+            }
+        }
+        """)
+
+        # Overwrite the default settings with user-provided parameters
+        self.settings = custom_settings
+        self.settings.ValidateAndAssignDefaults(default_settings)
+
+        # Construct the linear solver
+        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
+        self.thermal_linear_solver = linear_solver_factory.ConstructSolver(self.settings["thermal_solver_settings"]["linear_solver_settings"])
+        self.mechanical_linear_solver = linear_solver_factory.ConstructSolver(self.settings["mechanical_solver_settings"]["linear_solver_settings"])
+
+        print("Construction of DamUPThermoMechanicSolver finished")
+
+    def AddVariables(self):
+
+        super(DamUPThermoMechanicSolver, self).AddVariables()
+
+        ## Fluid variables
+        # Add pressure
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PRESSURE)
+        # Add Dynamic pressure variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt_PRESSURE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Dt2_PRESSURE)
+
+    def AddDofs(self):
+
+        for node in self.main_model_part.Nodes:
+            ## Solid dofs
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_X,KratosMultiphysics.REACTION_X)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y,KratosMultiphysics.REACTION_Y)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z,KratosMultiphysics.REACTION_Z)
+            ## Fluid dofs
+            node.AddDof(KratosMultiphysics.PRESSURE)
+            ## Thermal dofs
+            node.AddDof(KratosMultiphysics.TEMPERATURE)
+            # adding VELOCITY as dofs
+            node.AddDof(KratosMultiphysics.VELOCITY_X)
+            node.AddDof(KratosMultiphysics.VELOCITY_Y)
+            node.AddDof(KratosMultiphysics.VELOCITY_Z)
+            # adding ACCELERATION as dofs
+            node.AddDof(KratosMultiphysics.ACCELERATION_X)
+            node.AddDof(KratosMultiphysics.ACCELERATION_Y)
+            node.AddDof(KratosMultiphysics.ACCELERATION_Z)
+
+    #### Specific internal functions ####
+
+    def _ConstructScheme(self, scheme_type, solution_type):
+
+        rayleigh_m = self.settings["mechanical_solver_settings"]["rayleigh_m"].GetDouble()
+        rayleigh_k = self.settings["mechanical_solver_settings"]["rayleigh_k"].GetDouble()
+
+        beta=0.25
+        gamma=0.5
+        scheme = KratosDam.DamUPScheme(beta,gamma,rayleigh_m,rayleigh_k)
+
+        return scheme
```

## KratosMultiphysics/DamApplication/dam_analysis.py

 * *Ordering differences only*

```diff
@@ -1,464 +1,464 @@
-# Time monitoring
-import time as timer
-print(timer.ctime())
-initial_time = timer.perf_counter()
-
-import os
-
-# Importing Kratos Core, Applications and Dependencies
-import KratosMultiphysics
-import KratosMultiphysics.ConvectionDiffusionApplication as KratosConvDiff
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-import KratosMultiphysics.DamApplication as KratosDam
-
-# Importing the base class
-from KratosMultiphysics.analysis_stage import AnalysisStage
-
-from importlib import import_module
-
-class DamAnalysis(AnalysisStage):
-    """Main-script of the DamApplication put in a class."""
-    def __init__(self, model, project_parameters):
-        """DamApplication analysis."""
-        self.model = model
-        self.project_parameters = project_parameters
-        self.DefineParallelType()
-        self.DefineVariables()
-
-        if self.consider_selfweight:
-           self.model_selfweight = KratosMultiphysics.Model()
-           self.PreviousSelfweightProblem()
-
-        self.CreateModelPart()
-
-        if self.add_previous_results:
-            if self.type_of_results == "Mechanical":
-                self.model_mechanical = KratosMultiphysics.Model()
-                self.CreatePostModelPartMechanical()
-            elif self.type_of_results == "Thermal":
-                self.model_thermal = KratosMultiphysics.Model()
-                self.CreatePostModelPartThermal()
-            else:
-                self.model_mechanical = KratosMultiphysics.Model()
-                self.model_thermal = KratosMultiphysics.Model()
-                self.CreatePostModelPartMechanical()
-                self.CreatePostModelPartThermal()
-
-        self.SetSolver()
-
-    def DefineParallelType(self):
-        KratosMultiphysics.ParallelUtilities.SetNumThreads(self.project_parameters["problem_data"]["number_of_threads"].GetInt())
-        print("OpenMP parallel configuration. OMP_NUM_THREADS =",KratosMultiphysics.ParallelUtilities.GetNumThreads())
-
-    def DefineVariables(self):
-        self.domain_size = self.project_parameters["problem_data"]["domain_size"].GetInt()
-        self.problem_name = self.project_parameters["problem_data"]["problem_name"].GetString()
-        self.problem_path = os.getcwd()
-        self.echo_level = self.project_parameters["solver_settings"]["echo_level"].GetInt()
-        self.buffer_size = self.project_parameters["solver_settings"]["buffer_size"].GetInt()
-        self.consider_selfweight = self.project_parameters["problem_data"]["consider_selfweight"].GetBool()
-        self.consider_construction = self.project_parameters["problem_data"]["consider_construction"].GetBool()
-        self.use_streamline_utility = self.project_parameters["problem_data"]["streamlines_utility"].GetBool()
-        self.delta_time = self.project_parameters["problem_data"]["time_step"].GetDouble()
-        self.end_time = self.project_parameters["problem_data"]["end_time"].GetDouble()
-        self.time = self.project_parameters["problem_data"]["start_time"].GetDouble()
-        self.tol = self.delta_time*1.0e-10
-        self.time_scale = self.project_parameters["problem_data"]["time_scale"].GetString()
-        self.save_intermediate_mechanical_variables = self.project_parameters["transfer_results_process"]["save_intermediate_mechanical_variables"].GetBool()
-        self.save_intermediate_thermal_variables = self.project_parameters["transfer_results_process"]["save_intermediate_thermal_variables"].GetBool()
-        self.save_intermediate_variables_step = self.project_parameters["transfer_results_process"]["save_intermediate_variables_step"].GetInt()
-        self.save_final_mechanical_variables = self.project_parameters["transfer_results_process"]["save_final_mechanical_variables"].GetBool()
-        self.save_final_thermal_variables = self.project_parameters["transfer_results_process"]["save_final_thermal_variables"].GetBool()
-        self.add_previous_results = self.project_parameters["transfer_results_process"]["add_previous_results"].GetBool()
-        self.type_of_results = self.project_parameters["transfer_results_process"]["type_of_results"].GetString()
-        self.add_displacement = self.project_parameters["transfer_results_process"]["add_displacement"].GetBool()
-        self.add_stress = self.project_parameters["transfer_results_process"]["add_stress"].GetBool()
-        self.add_temperature = self.project_parameters["transfer_results_process"]["add_temperature"].GetBool()
-        self.add_reference_temperature = self.project_parameters["transfer_results_process"]["add_reference_temperature"].GetBool()
-
-
-        # Time Units Converter
-        if(self.time_scale=="Weeks"):               # Factor to pass from weeks to seconds
-            self.time_unit_converter = 604800.0
-        elif(self.time_scale=="Days"):               # Factor to pass from days to seconds
-            self.time_unit_converter = 86400.0
-        elif(self.time_scale=="Hours"):              # Factor to pass from hours to seconds
-            self.time_unit_converter = 3600.0
-        else:                                       # No changes
-            self.time_unit_converter = 1.0
-
-        # Update time variables
-        self.start_time = self.time
-        self.delta_time = self.delta_time * self.time_unit_converter
-        self.end_time = self.end_time * self.time_unit_converter
-        self.time = self.time * self.time_unit_converter
-        self.tol = self.tol * self.time_unit_converter
-
-    def CreateModelPart(self):
-        self.main_model_part = self.model.CreateModelPart(self.project_parameters["problem_data"]["model_part_name"].GetString())
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, self.domain_size)
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
-        self.main_model_part.ProcessInfo.SetValue(KratosDam.TIME_UNIT_CONVERTER, self.time_unit_converter)
-
-    def CreatePostModelPartMechanical(self):
-        self.file_name_mechanical = self.project_parameters["transfer_results_process"]["file_name_mechanical"].GetString()
-        self.post_model_part_mechanical = self.model_mechanical.CreateModelPart(self.file_name_mechanical)
-        self.post_model_part_mechanical.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, self.domain_size)
-        self.post_model_part_mechanical.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
-        self.post_model_part_mechanical.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
-        self.post_model_part_mechanical.ProcessInfo.SetValue(KratosDam.TIME_UNIT_CONVERTER, self.time_unit_converter)
-
-    def CreatePostModelPartThermal(self):
-        self.file_name_thermal = self.project_parameters["transfer_results_process"]["file_name_thermal"].GetString()
-        self.post_model_part_thermal = self.model_thermal.CreateModelPart(self.file_name_thermal)
-        self.post_model_part_thermal.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, self.domain_size)
-        self.post_model_part_thermal.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
-        self.post_model_part_thermal.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
-        self.post_model_part_thermal.ProcessInfo.SetValue(KratosDam.TIME_UNIT_CONVERTER, self.time_unit_converter)
-
-    def SetSolver(self):
-        python_module_name = "KratosMultiphysics.DamApplication"
-        full_module_name = python_module_name + "." + self.project_parameters["solver_settings"]["solver_type"].GetString()
-        solver_module = import_module(full_module_name)
-        self.solver = solver_module.CreateSolver(self.main_model_part, self.project_parameters["solver_settings"])
-
-    def PreviousSelfweightProblem(self):
-        # Parsing parmeters of Selfweight Problem
-        self_parameter_file = open("ProjectParametersSelfWeight.json",'r')
-        SelfWeightProjectParameters = KratosMultiphysics.Parameters( self_parameter_file.read())
-
-        ## Creating Selfweight model part --------------------------------------------------------------
-        self.self_weight_model_part = self.model_selfweight.CreateModelPart("SelfWeight")
-        self.self_weight_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, self.domain_size)
-        self.self_weight_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
-        self.self_weight_model_part.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
-        self.self_weight_model_part.ProcessInfo.SetValue(KratosDam.TIME_UNIT_CONVERTER, self.time_unit_converter)
-
-        ## Construct the solver for selfweight problem -------------------------------------------------
-        selfweight_solver_module = __import__(SelfWeightProjectParameters["solver_settings"]["solver_type"].GetString())
-        selfweight_solver = selfweight_solver_module.CreateSolver(self.self_weight_model_part, SelfWeightProjectParameters["solver_settings"])
-        selfweight_solver.AddVariables()
-        selfweight_solver.ImportModelPart()
-        selfweight_solver.AddDofs()
-
-        ## Kratos Selfweight Model ---------------------------------------------------------------------
-        #DamSelfWeightModel = KratosMultiphysics.Model()
-        #DamSelfWeightModel.AddModelPart(self.self_weight_model_part)
-
-        ## Initialize ----------------------------------------------------------------------------------
-
-        # Construct processes to be applied
-        import KratosMultiphysics.process_factory
-        self_list_of_processes = process_factory.KratosProcessFactory(DamSelfWeightModel).ConstructListOfProcesses( SelfWeightProjectParameters["constraints_process_list"] )
-        self_list_of_processes += process_factory.KratosProcessFactory(DamSelfWeightModel).ConstructListOfProcesses( SelfWeightProjectParameters["loads_process_list"] )
-
-        # Initialize processes
-        for process in self_list_of_processes:
-            process.ExecuteInitialize()
-
-        # Set TIME and DELTA_TIME and fill the previous steps of the buffer with the initial conditions
-        self_time = self.time - (self.buffer_size-1) * self.delta_time
-        self.self_weight_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
-        for step in range(self.buffer_size-1):
-            self_time = self_time + self.delta_time
-            self.self_weight_model_part.CloneTimeStep(self_time)
-
-        # Initialize the solver
-        selfweight_solver.Initialize()
-
-        # ExecuteBeforeSolutionLoop
-        for process in self_list_of_processes:
-            process.ExecuteBeforeSolutionLoop()
-
-        # Solving selfweight problem
-        selfweight_solver.Solve()
-
-        # Cleaning selfweight solver
-        selfweight_solver.Clear()
-
-        # Initialize transfer_selfweight_stress_utility
-        from KratosMultiphysics.DamApplication import transfer_selfweight_stress_utility
-        self.transfer_utility = transfer_selfweight_stress_utility.TransferSelfweightStressToMainModelPartUtility()
-
-    def Run(self):
-        self.Initialize()
-
-        self.RunMainTemporalLoop()
-
-        self.Finalize()
-
-    def Initialize(self):
-
-        self.solver.AddVariables() # Add problem variables
-        self.solver.ImportModelPart() # Read model_part (note: the buffer_size is set here)
-        self.solver.AddDofs() # Add degrees of freedom
-
-        #DamModel = KratosMultiphysics.Model() # Creation of Kratos model
-        #DamModel.AddModelPart(self.main_model_part)
-
-        # Print model_part and properties
-        if(self.echo_level > 1):
-            print(self.main_model_part)
-            for self.properties in self.main_model_part.Properties:
-                print(self.properties)
-
-        # Initialize GiD I/O
-        computing_model_part = self.solver.GetComputingModelPart()
-
-        ## Initialize Construction Utility
-        if self.consider_construction:
-            thermal_computing_model_part = self.solver.GetComputingThermalModelPart()
-            from KratosMultiphysics.DamApplication import dam_construction_utility
-            self.construction_utilities = dam_construction_utility.DamConstructionUtility(computing_model_part, thermal_computing_model_part, self.project_parameters["construction_process"])
-            self.construction_utilities.Initialize()
-
-        # Construct processes to be applied
-        import KratosMultiphysics.process_factory
-        self.list_of_processes = KratosMultiphysics.process_factory.KratosProcessFactory(self.model).ConstructListOfProcesses( self.project_parameters["constraints_process_list"] )
-        self.list_of_processes += KratosMultiphysics.process_factory.KratosProcessFactory(self.model).ConstructListOfProcesses( self.project_parameters["loads_process_list"] )
-        self.list_of_processes += KratosMultiphysics.process_factory.KratosProcessFactory(self.model).ConstructListOfProcesses( self.project_parameters["temperature_by_device_list"] )
-
-        self.list_of_output_processes = KratosMultiphysics.process_factory.KratosProcessFactory(self.model).ConstructListOfProcesses( self.project_parameters["output_device_list"] )
-
-        # Print list of constructed processes
-        if(self.echo_level>1):
-            for self.process in self.list_of_processes:
-                print(self.process)
-
-            for self.output_process in self.list_of_output_processes:
-                print(self.output_process)
-
-        # Initialize processes
-        for self.process in self.list_of_processes:
-            self.process.ExecuteInitialize()
-
-        for self.output_process in self.list_of_output_processes:
-            self.output_process.ExecuteInitialize()
-
-        # Set TIME and DELTA_TIME and fill the previous steps of the buffer with the initial conditions
-        self.time = self.time - (self.buffer_size-1)*self.delta_time
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
-        for step in range(self.buffer_size-1):
-            self.time = self.time + self.delta_time
-            self.main_model_part.CloneTimeStep(self.time)
-
-
-        ## Initialize Mapping Variables Utility
-        if self.add_previous_results:
-
-            from KratosMultiphysics.DamApplication import dam_mapping_variables_utility
-            dam_mapping_variables_utility = dam_mapping_variables_utility.MappingVariablesUtility(self.domain_size)
-
-            if self.type_of_results == "Mechanical":
-                self.post_model_part_mechanical.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
-                self.post_model_part_mechanical.AddNodalSolutionStepVariable(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)
-                self.aux_file_name_mechanical = self.file_name_mechanical.replace('.mdpa','')
-                KratosMultiphysics.ModelPartIO(self.aux_file_name_mechanical).ReadModelPart(self.post_model_part_mechanical)
-
-                dam_mapping_variables_utility.AddPreviousModelPartMechanical(self.main_model_part,self.post_model_part_mechanical,self.add_displacement,self.add_stress)
-
-            if self.type_of_results == "Thermal":
-                self.post_model_part_thermal.AddNodalSolutionStepVariable(KratosMultiphysics.TEMPERATURE)
-                self.post_model_part_thermal.AddNodalSolutionStepVariable(KratosDam.NODAL_REFERENCE_TEMPERATURE)
-                self.aux_file_name_thermal = self.file_name_thermal.replace('.mdpa','')
-                KratosMultiphysics.ModelPartIO(self.aux_file_name_thermal).ReadModelPart(self.post_model_part_thermal)
-
-                dam_mapping_variables_utility.AddPreviousModelPartThermal(self.main_model_part,self.post_model_part_thermal,self.add_temperature,self.add_reference_temperature)
-
-            if self.type_of_results == "Thermo-Mechanical":
-                self.post_model_part_mechanical.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
-                self.post_model_part_mechanical.AddNodalSolutionStepVariable(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)
-                self.aux_file_name_mechanical = self.file_name_mechanical.replace('.mdpa','')
-                KratosMultiphysics.ModelPartIO(self.aux_file_name_mechanical).ReadModelPart(self.post_model_part_mechanical)
-
-                self.post_model_part_thermal.AddNodalSolutionStepVariable(KratosMultiphysics.TEMPERATURE)
-                self.post_model_part_thermal.AddNodalSolutionStepVariable(KratosDam.NODAL_REFERENCE_TEMPERATURE)
-                self.aux_file_name_thermal = self.file_name_thermal.replace('.mdpa','')
-                KratosMultiphysics.ModelPartIO(self.aux_file_name_thermal).ReadModelPart(self.post_model_part_thermal)
-
-                dam_mapping_variables_utility.AddPreviousModelPartThermoMechanical(self.main_model_part,self.post_model_part_mechanical,self.post_model_part_thermal,self.add_displacement,self.add_stress,self.add_temperature,self.add_reference_temperature)
-
-        output_settings = self.project_parameters["output_configuration"]
-        #if self.parallel_type == "OpenMP":
-        from KratosMultiphysics.DamApplication import dam_cleaning_utility
-        dam_cleaning_utility.CleanPreviousFiles(self.problem_path) # Clean previous post files
-        from KratosMultiphysics.DamApplication.gid_dam_output_process import GiDDamOutputProcess
-        self.gid_output = GiDDamOutputProcess(computing_model_part,
-                                              self.problem_name,
-                                              self.start_time,
-                                              output_settings)
-        #else:
-            #from gid_output_process_mpi import GiDOutputProcessMPI
-            #self.gid_output = GiDOutputProcessMPI(computing_model_part,
-                                                  #self.problem_name,
-                                                  #self.start_time,
-                                                  #output_settings)
-        self.gid_output.ExecuteInitialize()
-
-        self.solver.Initialize() # Initialize the solver
-
-        if self.consider_construction:
-            # Execute initialize solution
-            self.construction_utilities.BeforeSolutionLoop()
-
-        # ExecuteBeforeSolutionLoop
-        for self.process in self.list_of_processes:
-            self.process.ExecuteBeforeSolutionLoop()
-
-        for self.output_process in self.list_of_output_processes:
-            self.output_process.ExecuteBeforeSolutionLoop()
-
-        self.gid_output.ExecuteBeforeSolutionLoop() # Set results when they are written in a single file
-
-        # Initialize streamlines_output_utility
-        self.UseStreamlineUtility = False
-        if self.use_streamline_utility and self.domain_size==3:
-            self.UseStreamlineUtility = True
-            from KratosMultiphysics.DamApplication import streamlines_output_utility
-            self.streamline_utility = streamlines_output_utility.StreamlinesOutputUtility(self.domain_size)
-
-        if (self.echo_level > 1):
-            f = open("ProjectParametersOutput.json", 'w')
-            f.write(self.project_parameters.PrettyPrintJsonString())
-            f.close()
-
-    def RunMainTemporalLoop(self):
-
-        while( (self.time+self.tol) <= self.end_time ):
-
-            # Update temporal variables
-            self.time = self.time + self.delta_time
-            self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
-            self.main_model_part.CloneTimeStep(self.time)
-
-            if self.add_previous_results:
-                if self.type_of_results == "Mechanical":
-                    self.post_model_part_mechanical.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
-                if self.type_of_results == "Thermal":
-                    self.post_model_part_thermal.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
-                if self.type_of_results == "Thermo-Mechanical":
-                    self.post_model_part_mechanical.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
-                    self.post_model_part_thermal.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
-
-            if self.consider_construction:
-                # Execute initialize solution
-                self.construction_utilities.InitializeSolutionStep()
-
-            # Update imposed conditions
-            for self.process in self.list_of_processes:
-                self.process.ExecuteInitializeSolutionStep()
-
-            for self.output_process in self.list_of_output_processes:
-                self.output_process.ExecuteInitializeSolutionStep()
-
-            # ExecuteInitializeSolutionStep
-            self.gid_output.ExecuteInitializeSolutionStep()
-            self.solver.Solve() # Solve step
-
-            # streamlines_output_utility
-            if self.UseStreamlineUtility:
-                self.streamline_utility.ComputeOutputStep(self.main_model_part, self.domain_size)
-            self.gid_output.ExecuteFinalizeSolutionStep()
-
-            for self.process in self.list_of_processes:
-                self.process.ExecuteFinalizeSolutionStep()
-
-            for self.output_process in self.list_of_output_processes:
-                self.output_process.ExecuteFinalizeSolutionStep()
-
-            for self.process in self.list_of_processes:
-                self.process.ExecuteBeforeOutputStep()
-
-            for self.output_process in self.list_of_output_processes:
-                self.output_process.ExecuteBeforeOutputStep()
-
-            # selfweight utility
-            if self.consider_selfweight:
-                self.transfer_utility.Transfer(self.self_weight_model_part, self.main_model_part, self.domain_size)
-
-            # add previous results utility
-            if self.add_previous_results and self.add_stress:
-                if self.type_of_results == "Mechanical" or self.type_of_results == "Thermo-Mechanical":
-                    from KratosMultiphysics.DamApplication import transfer_selfweight_stress_utility
-                    self.transfer_utility = transfer_selfweight_stress_utility.TransferSelfweightStressToMainModelPartUtility()
-                    self.transfer_utility.TransferInitialStress(self.main_model_part, self.domain_size)
-
-            # Write GiD results
-            if self.gid_output.IsOutputStep():
-                self.PrintOutput()
-
-            for self.process in self.list_of_processes:
-                self.process.ExecuteAfterOutputStep()
-
-            for self.output_process in self.list_of_output_processes:
-                self.output_process.ExecuteAfterOutputStep()
-                if self.output_process.IsOutputStep():
-                    self.output_process.PrintOutput()
-
-            if self.consider_construction:
-                #  After initialize solution
-                self.construction_utilities.AfterOutputStep()
-
-            # Save results at any time in an auxiliary .mdpa
-            if self.time == (self.save_intermediate_variables_step*self.time_unit_converter):
-                from KratosMultiphysics.DamApplication import save_variables_utility
-                self.save_utility = save_variables_utility.SaveVariablesUtility
-                if self.save_intermediate_mechanical_variables:
-                    self.save_utility.SaveMechanicalVariables(self.problem_name, self.project_parameters, self.main_model_part, self.save_intermediate_variables_step)
-                if self.save_intermediate_thermal_variables:
-                    self.save_utility.SaveThermalVariables(self.problem_name, self.project_parameters, self.main_model_part, self.save_intermediate_variables_step)
-
-    def PrintOutput(self):
-        self.gid_output.PrintOutput()
-
-    def Finalize(self):
-        # Save final results in an auxiliary .mdpa
-        from KratosMultiphysics.DamApplication import save_variables_utility
-        self.save_utility = save_variables_utility.SaveVariablesUtility
-        if self.save_final_mechanical_variables:
-            self.save_utility.SaveFinalMechanicalVariables(self.problem_name, self.project_parameters, self.main_model_part)
-
-        if self.save_final_thermal_variables:
-            self.save_utility.SaveFinalThermalVariables(self.problem_name, self.project_parameters, self.main_model_part)
-
-        self.gid_output.ExecuteFinalize() # Finalizing output files
-
-        for self.process in self.list_of_processes:
-            self.process.ExecuteFinalize()
-
-        for self.output_process in self.list_of_output_processes:
-            self.output_process.ExecuteFinalize()
-
-        # Finalizing strategy
-        #if self.parallel_type == "OpenMP":
-        self.solver.Clear()
-
-        # Time control
-        print("Analysis Completed. Elapsed Time = %.3f" % (timer.perf_counter() - initial_time)," seconds.")
-        print(timer.ctime())
-
-if __name__ == "__main__":
-    from sys import argv
-
-    if len(argv) > 2:
-        err_msg =  'Too many input arguments!\n'
-        err_msg += 'Use this script in the following way:\n'
-        err_msg += '- With default ProjectParameters (read from "ProjectParameters.json"):\n'
-        err_msg += '    "python3 dam_analysis.py"\n'
-        err_msg += '- With custom ProjectParameters:\n'
-        err_msg += '    "python3 dam_analysis.py CustomProjectParameters.json"\n'
-        raise Exception(err_msg)
-
-    if len(argv) == 2: # ProjectParameters is being passed from outside
-        project_parameters_file_name = argv[1]
-    else: # using default name
-        project_parameters_file_name = "ProjectParameters.json"
-
-    with open(project_parameters_file_name,'r') as parameter_file:
-        parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-    model = KratosMultiphysics.Model()
-    simulation = DamAnalysis(model, parameters)
-    simulation.Run()
+# Time monitoring
+import time as timer
+print(timer.ctime())
+initial_time = timer.perf_counter()
+
+import os
+
+# Importing Kratos Core, Applications and Dependencies
+import KratosMultiphysics
+import KratosMultiphysics.ConvectionDiffusionApplication as KratosConvDiff
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+import KratosMultiphysics.DamApplication as KratosDam
+
+# Importing the base class
+from KratosMultiphysics.analysis_stage import AnalysisStage
+
+from importlib import import_module
+
+class DamAnalysis(AnalysisStage):
+    """Main-script of the DamApplication put in a class."""
+    def __init__(self, model, project_parameters):
+        """DamApplication analysis."""
+        self.model = model
+        self.project_parameters = project_parameters
+        self.DefineParallelType()
+        self.DefineVariables()
+
+        if self.consider_selfweight:
+           self.model_selfweight = KratosMultiphysics.Model()
+           self.PreviousSelfweightProblem()
+
+        self.CreateModelPart()
+
+        if self.add_previous_results:
+            if self.type_of_results == "Mechanical":
+                self.model_mechanical = KratosMultiphysics.Model()
+                self.CreatePostModelPartMechanical()
+            elif self.type_of_results == "Thermal":
+                self.model_thermal = KratosMultiphysics.Model()
+                self.CreatePostModelPartThermal()
+            else:
+                self.model_mechanical = KratosMultiphysics.Model()
+                self.model_thermal = KratosMultiphysics.Model()
+                self.CreatePostModelPartMechanical()
+                self.CreatePostModelPartThermal()
+
+        self.SetSolver()
+
+    def DefineParallelType(self):
+        KratosMultiphysics.ParallelUtilities.SetNumThreads(self.project_parameters["problem_data"]["number_of_threads"].GetInt())
+        print("OpenMP parallel configuration. OMP_NUM_THREADS =",KratosMultiphysics.ParallelUtilities.GetNumThreads())
+
+    def DefineVariables(self):
+        self.domain_size = self.project_parameters["problem_data"]["domain_size"].GetInt()
+        self.problem_name = self.project_parameters["problem_data"]["problem_name"].GetString()
+        self.problem_path = os.getcwd()
+        self.echo_level = self.project_parameters["solver_settings"]["echo_level"].GetInt()
+        self.buffer_size = self.project_parameters["solver_settings"]["buffer_size"].GetInt()
+        self.consider_selfweight = self.project_parameters["problem_data"]["consider_selfweight"].GetBool()
+        self.consider_construction = self.project_parameters["problem_data"]["consider_construction"].GetBool()
+        self.use_streamline_utility = self.project_parameters["problem_data"]["streamlines_utility"].GetBool()
+        self.delta_time = self.project_parameters["problem_data"]["time_step"].GetDouble()
+        self.end_time = self.project_parameters["problem_data"]["end_time"].GetDouble()
+        self.time = self.project_parameters["problem_data"]["start_time"].GetDouble()
+        self.tol = self.delta_time*1.0e-10
+        self.time_scale = self.project_parameters["problem_data"]["time_scale"].GetString()
+        self.save_intermediate_mechanical_variables = self.project_parameters["transfer_results_process"]["save_intermediate_mechanical_variables"].GetBool()
+        self.save_intermediate_thermal_variables = self.project_parameters["transfer_results_process"]["save_intermediate_thermal_variables"].GetBool()
+        self.save_intermediate_variables_step = self.project_parameters["transfer_results_process"]["save_intermediate_variables_step"].GetInt()
+        self.save_final_mechanical_variables = self.project_parameters["transfer_results_process"]["save_final_mechanical_variables"].GetBool()
+        self.save_final_thermal_variables = self.project_parameters["transfer_results_process"]["save_final_thermal_variables"].GetBool()
+        self.add_previous_results = self.project_parameters["transfer_results_process"]["add_previous_results"].GetBool()
+        self.type_of_results = self.project_parameters["transfer_results_process"]["type_of_results"].GetString()
+        self.add_displacement = self.project_parameters["transfer_results_process"]["add_displacement"].GetBool()
+        self.add_stress = self.project_parameters["transfer_results_process"]["add_stress"].GetBool()
+        self.add_temperature = self.project_parameters["transfer_results_process"]["add_temperature"].GetBool()
+        self.add_reference_temperature = self.project_parameters["transfer_results_process"]["add_reference_temperature"].GetBool()
+
+
+        # Time Units Converter
+        if(self.time_scale=="Weeks"):               # Factor to pass from weeks to seconds
+            self.time_unit_converter = 604800.0
+        elif(self.time_scale=="Days"):               # Factor to pass from days to seconds
+            self.time_unit_converter = 86400.0
+        elif(self.time_scale=="Hours"):              # Factor to pass from hours to seconds
+            self.time_unit_converter = 3600.0
+        else:                                       # No changes
+            self.time_unit_converter = 1.0
+
+        # Update time variables
+        self.start_time = self.time
+        self.delta_time = self.delta_time * self.time_unit_converter
+        self.end_time = self.end_time * self.time_unit_converter
+        self.time = self.time * self.time_unit_converter
+        self.tol = self.tol * self.time_unit_converter
+
+    def CreateModelPart(self):
+        self.main_model_part = self.model.CreateModelPart(self.project_parameters["problem_data"]["model_part_name"].GetString())
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, self.domain_size)
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
+        self.main_model_part.ProcessInfo.SetValue(KratosDam.TIME_UNIT_CONVERTER, self.time_unit_converter)
+
+    def CreatePostModelPartMechanical(self):
+        self.file_name_mechanical = self.project_parameters["transfer_results_process"]["file_name_mechanical"].GetString()
+        self.post_model_part_mechanical = self.model_mechanical.CreateModelPart(self.file_name_mechanical)
+        self.post_model_part_mechanical.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, self.domain_size)
+        self.post_model_part_mechanical.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
+        self.post_model_part_mechanical.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
+        self.post_model_part_mechanical.ProcessInfo.SetValue(KratosDam.TIME_UNIT_CONVERTER, self.time_unit_converter)
+
+    def CreatePostModelPartThermal(self):
+        self.file_name_thermal = self.project_parameters["transfer_results_process"]["file_name_thermal"].GetString()
+        self.post_model_part_thermal = self.model_thermal.CreateModelPart(self.file_name_thermal)
+        self.post_model_part_thermal.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, self.domain_size)
+        self.post_model_part_thermal.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
+        self.post_model_part_thermal.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
+        self.post_model_part_thermal.ProcessInfo.SetValue(KratosDam.TIME_UNIT_CONVERTER, self.time_unit_converter)
+
+    def SetSolver(self):
+        python_module_name = "KratosMultiphysics.DamApplication"
+        full_module_name = python_module_name + "." + self.project_parameters["solver_settings"]["solver_type"].GetString()
+        solver_module = import_module(full_module_name)
+        self.solver = solver_module.CreateSolver(self.main_model_part, self.project_parameters["solver_settings"])
+
+    def PreviousSelfweightProblem(self):
+        # Parsing parmeters of Selfweight Problem
+        self_parameter_file = open("ProjectParametersSelfWeight.json",'r')
+        SelfWeightProjectParameters = KratosMultiphysics.Parameters( self_parameter_file.read())
+
+        ## Creating Selfweight model part --------------------------------------------------------------
+        self.self_weight_model_part = self.model_selfweight.CreateModelPart("SelfWeight")
+        self.self_weight_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, self.domain_size)
+        self.self_weight_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
+        self.self_weight_model_part.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
+        self.self_weight_model_part.ProcessInfo.SetValue(KratosDam.TIME_UNIT_CONVERTER, self.time_unit_converter)
+
+        ## Construct the solver for selfweight problem -------------------------------------------------
+        selfweight_solver_module = __import__(SelfWeightProjectParameters["solver_settings"]["solver_type"].GetString())
+        selfweight_solver = selfweight_solver_module.CreateSolver(self.self_weight_model_part, SelfWeightProjectParameters["solver_settings"])
+        selfweight_solver.AddVariables()
+        selfweight_solver.ImportModelPart()
+        selfweight_solver.AddDofs()
+
+        ## Kratos Selfweight Model ---------------------------------------------------------------------
+        #DamSelfWeightModel = KratosMultiphysics.Model()
+        #DamSelfWeightModel.AddModelPart(self.self_weight_model_part)
+
+        ## Initialize ----------------------------------------------------------------------------------
+
+        # Construct processes to be applied
+        import KratosMultiphysics.process_factory
+        self_list_of_processes = process_factory.KratosProcessFactory(DamSelfWeightModel).ConstructListOfProcesses( SelfWeightProjectParameters["constraints_process_list"] )
+        self_list_of_processes += process_factory.KratosProcessFactory(DamSelfWeightModel).ConstructListOfProcesses( SelfWeightProjectParameters["loads_process_list"] )
+
+        # Initialize processes
+        for process in self_list_of_processes:
+            process.ExecuteInitialize()
+
+        # Set TIME and DELTA_TIME and fill the previous steps of the buffer with the initial conditions
+        self_time = self.time - (self.buffer_size-1) * self.delta_time
+        self.self_weight_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
+        for step in range(self.buffer_size-1):
+            self_time = self_time + self.delta_time
+            self.self_weight_model_part.CloneTimeStep(self_time)
+
+        # Initialize the solver
+        selfweight_solver.Initialize()
+
+        # ExecuteBeforeSolutionLoop
+        for process in self_list_of_processes:
+            process.ExecuteBeforeSolutionLoop()
+
+        # Solving selfweight problem
+        selfweight_solver.Solve()
+
+        # Cleaning selfweight solver
+        selfweight_solver.Clear()
+
+        # Initialize transfer_selfweight_stress_utility
+        from KratosMultiphysics.DamApplication import transfer_selfweight_stress_utility
+        self.transfer_utility = transfer_selfweight_stress_utility.TransferSelfweightStressToMainModelPartUtility()
+
+    def Run(self):
+        self.Initialize()
+
+        self.RunMainTemporalLoop()
+
+        self.Finalize()
+
+    def Initialize(self):
+
+        self.solver.AddVariables() # Add problem variables
+        self.solver.ImportModelPart() # Read model_part (note: the buffer_size is set here)
+        self.solver.AddDofs() # Add degrees of freedom
+
+        #DamModel = KratosMultiphysics.Model() # Creation of Kratos model
+        #DamModel.AddModelPart(self.main_model_part)
+
+        # Print model_part and properties
+        if(self.echo_level > 1):
+            print(self.main_model_part)
+            for self.properties in self.main_model_part.Properties:
+                print(self.properties)
+
+        # Initialize GiD I/O
+        computing_model_part = self.solver.GetComputingModelPart()
+
+        ## Initialize Construction Utility
+        if self.consider_construction:
+            thermal_computing_model_part = self.solver.GetComputingThermalModelPart()
+            from KratosMultiphysics.DamApplication import dam_construction_utility
+            self.construction_utilities = dam_construction_utility.DamConstructionUtility(computing_model_part, thermal_computing_model_part, self.project_parameters["construction_process"])
+            self.construction_utilities.Initialize()
+
+        # Construct processes to be applied
+        import KratosMultiphysics.process_factory
+        self.list_of_processes = KratosMultiphysics.process_factory.KratosProcessFactory(self.model).ConstructListOfProcesses( self.project_parameters["constraints_process_list"] )
+        self.list_of_processes += KratosMultiphysics.process_factory.KratosProcessFactory(self.model).ConstructListOfProcesses( self.project_parameters["loads_process_list"] )
+        self.list_of_processes += KratosMultiphysics.process_factory.KratosProcessFactory(self.model).ConstructListOfProcesses( self.project_parameters["temperature_by_device_list"] )
+
+        self.list_of_output_processes = KratosMultiphysics.process_factory.KratosProcessFactory(self.model).ConstructListOfProcesses( self.project_parameters["output_device_list"] )
+
+        # Print list of constructed processes
+        if(self.echo_level>1):
+            for self.process in self.list_of_processes:
+                print(self.process)
+
+            for self.output_process in self.list_of_output_processes:
+                print(self.output_process)
+
+        # Initialize processes
+        for self.process in self.list_of_processes:
+            self.process.ExecuteInitialize()
+
+        for self.output_process in self.list_of_output_processes:
+            self.output_process.ExecuteInitialize()
+
+        # Set TIME and DELTA_TIME and fill the previous steps of the buffer with the initial conditions
+        self.time = self.time - (self.buffer_size-1)*self.delta_time
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, self.time)
+        for step in range(self.buffer_size-1):
+            self.time = self.time + self.delta_time
+            self.main_model_part.CloneTimeStep(self.time)
+
+
+        ## Initialize Mapping Variables Utility
+        if self.add_previous_results:
+
+            from KratosMultiphysics.DamApplication import dam_mapping_variables_utility
+            dam_mapping_variables_utility = dam_mapping_variables_utility.MappingVariablesUtility(self.domain_size)
+
+            if self.type_of_results == "Mechanical":
+                self.post_model_part_mechanical.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
+                self.post_model_part_mechanical.AddNodalSolutionStepVariable(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)
+                self.aux_file_name_mechanical = self.file_name_mechanical.replace('.mdpa','')
+                KratosMultiphysics.ModelPartIO(self.aux_file_name_mechanical).ReadModelPart(self.post_model_part_mechanical)
+
+                dam_mapping_variables_utility.AddPreviousModelPartMechanical(self.main_model_part,self.post_model_part_mechanical,self.add_displacement,self.add_stress)
+
+            if self.type_of_results == "Thermal":
+                self.post_model_part_thermal.AddNodalSolutionStepVariable(KratosMultiphysics.TEMPERATURE)
+                self.post_model_part_thermal.AddNodalSolutionStepVariable(KratosDam.NODAL_REFERENCE_TEMPERATURE)
+                self.aux_file_name_thermal = self.file_name_thermal.replace('.mdpa','')
+                KratosMultiphysics.ModelPartIO(self.aux_file_name_thermal).ReadModelPart(self.post_model_part_thermal)
+
+                dam_mapping_variables_utility.AddPreviousModelPartThermal(self.main_model_part,self.post_model_part_thermal,self.add_temperature,self.add_reference_temperature)
+
+            if self.type_of_results == "Thermo-Mechanical":
+                self.post_model_part_mechanical.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
+                self.post_model_part_mechanical.AddNodalSolutionStepVariable(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)
+                self.aux_file_name_mechanical = self.file_name_mechanical.replace('.mdpa','')
+                KratosMultiphysics.ModelPartIO(self.aux_file_name_mechanical).ReadModelPart(self.post_model_part_mechanical)
+
+                self.post_model_part_thermal.AddNodalSolutionStepVariable(KratosMultiphysics.TEMPERATURE)
+                self.post_model_part_thermal.AddNodalSolutionStepVariable(KratosDam.NODAL_REFERENCE_TEMPERATURE)
+                self.aux_file_name_thermal = self.file_name_thermal.replace('.mdpa','')
+                KratosMultiphysics.ModelPartIO(self.aux_file_name_thermal).ReadModelPart(self.post_model_part_thermal)
+
+                dam_mapping_variables_utility.AddPreviousModelPartThermoMechanical(self.main_model_part,self.post_model_part_mechanical,self.post_model_part_thermal,self.add_displacement,self.add_stress,self.add_temperature,self.add_reference_temperature)
+
+        output_settings = self.project_parameters["output_configuration"]
+        #if self.parallel_type == "OpenMP":
+        from KratosMultiphysics.DamApplication import dam_cleaning_utility
+        dam_cleaning_utility.CleanPreviousFiles(self.problem_path) # Clean previous post files
+        from KratosMultiphysics.DamApplication.gid_dam_output_process import GiDDamOutputProcess
+        self.gid_output = GiDDamOutputProcess(computing_model_part,
+                                              self.problem_name,
+                                              self.start_time,
+                                              output_settings)
+        #else:
+            #from gid_output_process_mpi import GiDOutputProcessMPI
+            #self.gid_output = GiDOutputProcessMPI(computing_model_part,
+                                                  #self.problem_name,
+                                                  #self.start_time,
+                                                  #output_settings)
+        self.gid_output.ExecuteInitialize()
+
+        self.solver.Initialize() # Initialize the solver
+
+        if self.consider_construction:
+            # Execute initialize solution
+            self.construction_utilities.BeforeSolutionLoop()
+
+        # ExecuteBeforeSolutionLoop
+        for self.process in self.list_of_processes:
+            self.process.ExecuteBeforeSolutionLoop()
+
+        for self.output_process in self.list_of_output_processes:
+            self.output_process.ExecuteBeforeSolutionLoop()
+
+        self.gid_output.ExecuteBeforeSolutionLoop() # Set results when they are written in a single file
+
+        # Initialize streamlines_output_utility
+        self.UseStreamlineUtility = False
+        if self.use_streamline_utility and self.domain_size==3:
+            self.UseStreamlineUtility = True
+            from KratosMultiphysics.DamApplication import streamlines_output_utility
+            self.streamline_utility = streamlines_output_utility.StreamlinesOutputUtility(self.domain_size)
+
+        if (self.echo_level > 1):
+            f = open("ProjectParametersOutput.json", 'w')
+            f.write(self.project_parameters.PrettyPrintJsonString())
+            f.close()
+
+    def RunMainTemporalLoop(self):
+
+        while( (self.time+self.tol) <= self.end_time ):
+
+            # Update temporal variables
+            self.time = self.time + self.delta_time
+            self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
+            self.main_model_part.CloneTimeStep(self.time)
+
+            if self.add_previous_results:
+                if self.type_of_results == "Mechanical":
+                    self.post_model_part_mechanical.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
+                if self.type_of_results == "Thermal":
+                    self.post_model_part_thermal.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
+                if self.type_of_results == "Thermo-Mechanical":
+                    self.post_model_part_mechanical.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
+                    self.post_model_part_thermal.ProcessInfo.SetValue(KratosMultiphysics.DELTA_TIME, self.delta_time)
+
+            if self.consider_construction:
+                # Execute initialize solution
+                self.construction_utilities.InitializeSolutionStep()
+
+            # Update imposed conditions
+            for self.process in self.list_of_processes:
+                self.process.ExecuteInitializeSolutionStep()
+
+            for self.output_process in self.list_of_output_processes:
+                self.output_process.ExecuteInitializeSolutionStep()
+
+            # ExecuteInitializeSolutionStep
+            self.gid_output.ExecuteInitializeSolutionStep()
+            self.solver.Solve() # Solve step
+
+            # streamlines_output_utility
+            if self.UseStreamlineUtility:
+                self.streamline_utility.ComputeOutputStep(self.main_model_part, self.domain_size)
+            self.gid_output.ExecuteFinalizeSolutionStep()
+
+            for self.process in self.list_of_processes:
+                self.process.ExecuteFinalizeSolutionStep()
+
+            for self.output_process in self.list_of_output_processes:
+                self.output_process.ExecuteFinalizeSolutionStep()
+
+            for self.process in self.list_of_processes:
+                self.process.ExecuteBeforeOutputStep()
+
+            for self.output_process in self.list_of_output_processes:
+                self.output_process.ExecuteBeforeOutputStep()
+
+            # selfweight utility
+            if self.consider_selfweight:
+                self.transfer_utility.Transfer(self.self_weight_model_part, self.main_model_part, self.domain_size)
+
+            # add previous results utility
+            if self.add_previous_results and self.add_stress:
+                if self.type_of_results == "Mechanical" or self.type_of_results == "Thermo-Mechanical":
+                    from KratosMultiphysics.DamApplication import transfer_selfweight_stress_utility
+                    self.transfer_utility = transfer_selfweight_stress_utility.TransferSelfweightStressToMainModelPartUtility()
+                    self.transfer_utility.TransferInitialStress(self.main_model_part, self.domain_size)
+
+            # Write GiD results
+            if self.gid_output.IsOutputStep():
+                self.PrintOutput()
+
+            for self.process in self.list_of_processes:
+                self.process.ExecuteAfterOutputStep()
+
+            for self.output_process in self.list_of_output_processes:
+                self.output_process.ExecuteAfterOutputStep()
+                if self.output_process.IsOutputStep():
+                    self.output_process.PrintOutput()
+
+            if self.consider_construction:
+                #  After initialize solution
+                self.construction_utilities.AfterOutputStep()
+
+            # Save results at any time in an auxiliary .mdpa
+            if self.time == (self.save_intermediate_variables_step*self.time_unit_converter):
+                from KratosMultiphysics.DamApplication import save_variables_utility
+                self.save_utility = save_variables_utility.SaveVariablesUtility
+                if self.save_intermediate_mechanical_variables:
+                    self.save_utility.SaveMechanicalVariables(self.problem_name, self.project_parameters, self.main_model_part, self.save_intermediate_variables_step)
+                if self.save_intermediate_thermal_variables:
+                    self.save_utility.SaveThermalVariables(self.problem_name, self.project_parameters, self.main_model_part, self.save_intermediate_variables_step)
+
+    def PrintOutput(self):
+        self.gid_output.PrintOutput()
+
+    def Finalize(self):
+        # Save final results in an auxiliary .mdpa
+        from KratosMultiphysics.DamApplication import save_variables_utility
+        self.save_utility = save_variables_utility.SaveVariablesUtility
+        if self.save_final_mechanical_variables:
+            self.save_utility.SaveFinalMechanicalVariables(self.problem_name, self.project_parameters, self.main_model_part)
+
+        if self.save_final_thermal_variables:
+            self.save_utility.SaveFinalThermalVariables(self.problem_name, self.project_parameters, self.main_model_part)
+
+        self.gid_output.ExecuteFinalize() # Finalizing output files
+
+        for self.process in self.list_of_processes:
+            self.process.ExecuteFinalize()
+
+        for self.output_process in self.list_of_output_processes:
+            self.output_process.ExecuteFinalize()
+
+        # Finalizing strategy
+        #if self.parallel_type == "OpenMP":
+        self.solver.Clear()
+
+        # Time control
+        print("Analysis Completed. Elapsed Time = %.3f" % (timer.perf_counter() - initial_time)," seconds.")
+        print(timer.ctime())
+
+if __name__ == "__main__":
+    from sys import argv
+
+    if len(argv) > 2:
+        err_msg =  'Too many input arguments!\n'
+        err_msg += 'Use this script in the following way:\n'
+        err_msg += '- With default ProjectParameters (read from "ProjectParameters.json"):\n'
+        err_msg += '    "python3 dam_analysis.py"\n'
+        err_msg += '- With custom ProjectParameters:\n'
+        err_msg += '    "python3 dam_analysis.py CustomProjectParameters.json"\n'
+        raise Exception(err_msg)
+
+    if len(argv) == 2: # ProjectParameters is being passed from outside
+        project_parameters_file_name = argv[1]
+    else: # using default name
+        project_parameters_file_name = "ProjectParameters.json"
+
+    with open(project_parameters_file_name,'r') as parameter_file:
+        parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+    model = KratosMultiphysics.Model()
+    simulation = DamAnalysis(model, parameters)
+    simulation.Run()
```

## KratosMultiphysics/DamApplication/dam_cleaning_utility.py

 * *Ordering differences only*

```diff
@@ -1,25 +1,25 @@
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
-    for f in os.listdir(problem_path):
-        if f.endswith(file_ending_type):
-            os.remove(f)
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
+    for f in os.listdir(problem_path):
+        if f.endswith(file_ending_type):
+            os.remove(f)
```

## KratosMultiphysics/DamApplication/dam_constitutive_law_utility.py

 * *Ordering differences only*

```diff
@@ -1,18 +1,18 @@
-#importing the Kratos Library
-from KratosMultiphysics import *
-from KratosMultiphysics.StructuralMechanicsApplication import *
-from KratosMultiphysics.PoromechanicsApplication import *
-from KratosMultiphysics.DamApplication import *
-
-def SetConstitutiveLaw(model_part):
-
-    for prop in model_part.Properties:
-        if prop.Has(CONSTITUTIVE_LAW_NAME):
-            ConstitutiveLawName=prop.GetValue(CONSTITUTIVE_LAW_NAME)
-            if (ConstitutiveLawName=="Newtonian"):
-                print("Newtonian Law is not used, we just need its parameters")
-            else:
-                mat = globals().get(ConstitutiveLawName)()
-                prop.SetValue(CONSTITUTIVE_LAW, mat.Clone())
-        else:
-            print("Property",prop.Id,"has no CONSTITUTIVE_LAW_NAME")
+#importing the Kratos Library
+from KratosMultiphysics import *
+from KratosMultiphysics.StructuralMechanicsApplication import *
+from KratosMultiphysics.PoromechanicsApplication import *
+from KratosMultiphysics.DamApplication import *
+
+def SetConstitutiveLaw(model_part):
+
+    for prop in model_part.Properties:
+        if prop.Has(CONSTITUTIVE_LAW_NAME):
+            ConstitutiveLawName=prop.GetValue(CONSTITUTIVE_LAW_NAME)
+            if (ConstitutiveLawName=="Newtonian"):
+                print("Newtonian Law is not used, we just need its parameters")
+            else:
+                mat = globals().get(ConstitutiveLawName)()
+                prop.SetValue(CONSTITUTIVE_LAW, mat.Clone())
+        else:
+            print("Property",prop.Id,"has no CONSTITUTIVE_LAW_NAME")
```

## KratosMultiphysics/DamApplication/dam_construction_utility.py

 * *Ordering differences only*

```diff
@@ -1,162 +1,162 @@
-#importing the Kratos Library
-from KratosMultiphysics import *
-from KratosMultiphysics.StructuralMechanicsApplication import *
-# from KratosMultiphysics.ExternalSolversApplication import *
-from KratosMultiphysics.DamApplication import *
-
-class DamConstructionUtility:
-
-    def __init__(self,mechanical_model_part, thermal_model_part, parameters):
-
-        self.mechanical_model_part = mechanical_model_part
-        self.thermal_model_part = thermal_model_part
-
-        # Getting neccessary files from constructive phase
-        ambient_input_file_name = parameters["ambient_input_file_name"].GetString()
-        self.construction_input_file_name = parameters["construction_input_file_name"].GetString()
-
-        self.check_temperature_parameters = Parameters("{}")
-        self.activate_check_temperature = parameters["activate_check_temperature"].GetBool()
-        if (self.activate_check_temperature):
-            self.check_temperature_parameters.AddValue("maximum_temperature_increment",parameters["maximum_temperature_increment"])
-            self.check_temperature_parameters.AddValue("maximum_temperature",parameters["maximum_temperature"])
-            self.check_temperature_parameters.AddValue("minimum_temperature",parameters["minimum_temperature"])
-
-        self.heat_source_parameters = Parameters("{}")
-        if (parameters["source_type"].GetString() == "Adiabatic"):
-            self.heat_source_type = "Noorzai"
-            self.heat_source_parameters.AddValue("density",parameters["density"])
-            self.heat_source_parameters.AddValue("specific_heat",parameters["specific_heat"])
-            self.heat_source_parameters.AddValue("alpha",parameters["alpha"])
-            self.heat_source_parameters.AddValue("t_max",parameters["tmax"])
-
-        if (parameters["source_type"].GetString() == "NonAdiabatic"):
-            self.heat_source_type = "Azenha"
-            self.heat_source_parameters.AddValue("activation_energy",parameters["activation_energy"])
-            self.heat_source_parameters.AddValue("gas_constant",parameters["gas_constant"])
-            self.heat_source_parameters.AddValue("constant_rate",parameters["constant_rate"])
-            self.heat_source_parameters.AddValue("alpha_initial",parameters["alpha_initial"])
-            self.heat_source_parameters.AddValue("q_total",parameters["q_total"])
-            self.heat_source_parameters.AddValue("A",parameters["A"])
-            self.heat_source_parameters.AddValue("B",parameters["B"])
-            self.heat_source_parameters.AddValue("C",parameters["C"])
-            self.heat_source_parameters.AddValue("D",parameters["D"])
-
-        # If there are parts alreadey existent (actived from the beginning of the model) getting these parts for its activation in the initialize. This parts can correspond to either the soil or the already built part of the dam.
-        if (parameters["activate_soil_part"].GetBool()):
-            name_soil_part = parameters["name_soil_part"].GetString()
-            parameters.RemoveValue("name_soil_part")
-            parameters.AddEmptyValue("mechanical_soil_part").SetString("sub_Parts_"+name_soil_part)
-            parameters.AddEmptyValue("thermal_soil_part").SetString("sub_Thermal_"+name_soil_part)
-
-        if (parameters["activate_existing_part"].GetBool()):
-            name_existing_part = parameters["name_existing_part"].GetString()
-            parameters.RemoveValue("name_existing_part")
-            parameters.AddEmptyValue("mechanical_existing_part").SetString("sub_Parts_"+name_existing_part)
-            parameters.AddEmptyValue("thermal_existing_part").SetString("sub_Thermal_"+name_existing_part)
-
-        self.table_ambient = PiecewiseLinearTable()
-        with open(ambient_input_file_name,'r') as file_name1:
-            for j, line in enumerate(file_name1):
-                file_1= line.split(" ")
-                if (len(file_1)) > 1:
-                    self.table_ambient.AddRow(float(file_1[0]), float(file_1[1]))
-
-        # Construct the utility
-        self.Construction = ConstructionUtility(self.mechanical_model_part,self.thermal_model_part, self.table_ambient, parameters)
-
-    def Initialize(self):
-        self.Construction.Initialize()
-
-        # The function recieves the mame of submodel Part, the number of phase and the activation time
-        print("Assigning time activation for each node")
-        with open(self.construction_input_file_name,'r') as file_name2:
-            for j, line in enumerate(file_name2):
-                file_2 = line.split(" ")
-                if (len(file_2)) > 1:
-                    self.name_sub_thermal_part = "sub_Thermal_" + file_2[1]
-                    self.Construction.AssignTimeActivation(self.name_sub_thermal_part,int(file_2[2]),float(file_2[0]), float(file_2[3]))
-
-    def BeforeSolutionLoop(self):
-
-        time = self.mechanical_model_part.ProcessInfo[TIME]
-        tol = self.mechanical_model_part.ProcessInfo[DELTA_TIME]*1e-10
-        time_unit_converter = self.mechanical_model_part.ProcessInfo[TIME_UNIT_CONVERTER]
-
-        # Activation according the input file
-        with open(self.construction_input_file_name,'r') as file_name3:
-            for j, line in enumerate(file_name3):
-                file_3 = line.split(" ")
-                if ((len(file_3)) > 1 and (time >=(float(file_3[0])*time_unit_converter-tol))):
-                    print("New phase has been activated...")
-                    self.name_sub_thermal_part = "sub_Thermal_" + file_3[1]
-                    self.name_sub_mechanical_part = "sub_Parts_" + file_3[1]
-                    self.name_sub_heat_flux = "sub_TAmbientFlux3D_T_Ambient_Heat_Flux_" + file_3[1]
-                    self.name_sub_hydro_press = "sub_HydroSurfacePressure3D_Hydrostatic_Pressure_" + file_3[1]
-
-                    thermal_conditions = True
-                    mechanical_conditions = True
-                    try:
-                        self.thermal_model_part.GetSubModelPart(self.name_sub_heat_flux)
-                    except:
-                        thermal_conditions = False
-                    try:
-                        self.mechanical_model_part.GetSubModelPart(self.name_sub_hydro_press)
-                    except:
-                        mechanical_conditions = False
-
-                    self.Construction.InitializeSolutionStep(self.name_sub_thermal_part,self.name_sub_mechanical_part,self.name_sub_heat_flux,self.name_sub_hydro_press,thermal_conditions,mechanical_conditions,int(file_3[2]))
-
-    def InitializeSolutionStep(self):
-
-        time = self.mechanical_model_part.ProcessInfo[TIME]
-        tol = self.mechanical_model_part.ProcessInfo[DELTA_TIME]*1e-10
-        time_unit_converter = self.mechanical_model_part.ProcessInfo[TIME_UNIT_CONVERTER]
-
-        # Activation according the input file
-        with open(self.construction_input_file_name,'r') as file_name3:
-            for j, line in enumerate(file_name3):
-                file_3 = line.split(" ")
-                if ((len(file_3)) > 1 and ((time <=(float(file_3[0])*time_unit_converter+tol)) and (time >=(float(file_3[0])*time_unit_converter-tol)))):
-                    print("New phase has been activated...")
-                    self.name_sub_thermal_part = "sub_Thermal_" + file_3[1]
-                    self.name_sub_mechanical_part = "sub_Parts_" + file_3[1]
-                    self.name_sub_heat_flux = "sub_TAmbientFlux3D_T_Ambient_Heat_Flux_" + file_3[1]
-                    self.name_sub_hydro_press = "sub_HydroSurfacePressure3D_Hydrostatic_Pressure_" + file_3[1]
-
-                    thermal_conditions = True
-                    mechanical_conditions = True
-                    try:
-                        self.thermal_model_part.GetSubModelPart(self.name_sub_heat_flux)
-                    except:
-                        thermal_conditions = False
-                    try:
-                        self.mechanical_model_part.GetSubModelPart(self.name_sub_hydro_press)
-                    except:
-                        mechanical_conditions = False
-
-                    self.Construction.InitializeSolutionStep(self.name_sub_thermal_part,self.name_sub_mechanical_part,self.name_sub_heat_flux,self.name_sub_hydro_press,thermal_conditions,mechanical_conditions,int(file_3[2]))
-
-        # Check if the temperature of every nodes is in the range (it must be done each step)
-        if (self.activate_check_temperature):
-            print("Checking temperatures...")
-            self.Construction.CheckTemperature(self.check_temperature_parameters)
-
-        # Detection of fluxes (it must be done each step)
-        print("Searching free surfaces...")
-        self.Construction.SearchingFluxes()
-
-        # Contribution of heat source (it must be done each step)
-        print("Assigning heat source...")
-        if (self.heat_source_type == 'Noorzai'):
-            self.Construction.ActiveHeatFluxNoorzai(self.heat_source_parameters)
-
-        elif (self.heat_source_type == 'Azenha'):
-            self.Construction.ActiveHeatFluxAzenha(self.heat_source_parameters)
-
-
-    def AfterOutputStep(self):
-        self.Construction.AfterOutputStep()
-
-    def ExecuteFinalize(self):
-        pass
+#importing the Kratos Library
+from KratosMultiphysics import *
+from KratosMultiphysics.StructuralMechanicsApplication import *
+# from KratosMultiphysics.ExternalSolversApplication import *
+from KratosMultiphysics.DamApplication import *
+
+class DamConstructionUtility:
+
+    def __init__(self,mechanical_model_part, thermal_model_part, parameters):
+
+        self.mechanical_model_part = mechanical_model_part
+        self.thermal_model_part = thermal_model_part
+
+        # Getting neccessary files from constructive phase
+        ambient_input_file_name = parameters["ambient_input_file_name"].GetString()
+        self.construction_input_file_name = parameters["construction_input_file_name"].GetString()
+
+        self.check_temperature_parameters = Parameters("{}")
+        self.activate_check_temperature = parameters["activate_check_temperature"].GetBool()
+        if (self.activate_check_temperature):
+            self.check_temperature_parameters.AddValue("maximum_temperature_increment",parameters["maximum_temperature_increment"])
+            self.check_temperature_parameters.AddValue("maximum_temperature",parameters["maximum_temperature"])
+            self.check_temperature_parameters.AddValue("minimum_temperature",parameters["minimum_temperature"])
+
+        self.heat_source_parameters = Parameters("{}")
+        if (parameters["source_type"].GetString() == "Adiabatic"):
+            self.heat_source_type = "Noorzai"
+            self.heat_source_parameters.AddValue("density",parameters["density"])
+            self.heat_source_parameters.AddValue("specific_heat",parameters["specific_heat"])
+            self.heat_source_parameters.AddValue("alpha",parameters["alpha"])
+            self.heat_source_parameters.AddValue("t_max",parameters["tmax"])
+
+        if (parameters["source_type"].GetString() == "NonAdiabatic"):
+            self.heat_source_type = "Azenha"
+            self.heat_source_parameters.AddValue("activation_energy",parameters["activation_energy"])
+            self.heat_source_parameters.AddValue("gas_constant",parameters["gas_constant"])
+            self.heat_source_parameters.AddValue("constant_rate",parameters["constant_rate"])
+            self.heat_source_parameters.AddValue("alpha_initial",parameters["alpha_initial"])
+            self.heat_source_parameters.AddValue("q_total",parameters["q_total"])
+            self.heat_source_parameters.AddValue("A",parameters["A"])
+            self.heat_source_parameters.AddValue("B",parameters["B"])
+            self.heat_source_parameters.AddValue("C",parameters["C"])
+            self.heat_source_parameters.AddValue("D",parameters["D"])
+
+        # If there are parts alreadey existent (actived from the beginning of the model) getting these parts for its activation in the initialize. This parts can correspond to either the soil or the already built part of the dam.
+        if (parameters["activate_soil_part"].GetBool()):
+            name_soil_part = parameters["name_soil_part"].GetString()
+            parameters.RemoveValue("name_soil_part")
+            parameters.AddEmptyValue("mechanical_soil_part").SetString("sub_Parts_"+name_soil_part)
+            parameters.AddEmptyValue("thermal_soil_part").SetString("sub_Thermal_"+name_soil_part)
+
+        if (parameters["activate_existing_part"].GetBool()):
+            name_existing_part = parameters["name_existing_part"].GetString()
+            parameters.RemoveValue("name_existing_part")
+            parameters.AddEmptyValue("mechanical_existing_part").SetString("sub_Parts_"+name_existing_part)
+            parameters.AddEmptyValue("thermal_existing_part").SetString("sub_Thermal_"+name_existing_part)
+
+        self.table_ambient = PiecewiseLinearTable()
+        with open(ambient_input_file_name,'r') as file_name1:
+            for j, line in enumerate(file_name1):
+                file_1= line.split(" ")
+                if (len(file_1)) > 1:
+                    self.table_ambient.AddRow(float(file_1[0]), float(file_1[1]))
+
+        # Construct the utility
+        self.Construction = ConstructionUtility(self.mechanical_model_part,self.thermal_model_part, self.table_ambient, parameters)
+
+    def Initialize(self):
+        self.Construction.Initialize()
+
+        # The function recieves the mame of submodel Part, the number of phase and the activation time
+        print("Assigning time activation for each node")
+        with open(self.construction_input_file_name,'r') as file_name2:
+            for j, line in enumerate(file_name2):
+                file_2 = line.split(" ")
+                if (len(file_2)) > 1:
+                    self.name_sub_thermal_part = "sub_Thermal_" + file_2[1]
+                    self.Construction.AssignTimeActivation(self.name_sub_thermal_part,int(file_2[2]),float(file_2[0]), float(file_2[3]))
+
+    def BeforeSolutionLoop(self):
+
+        time = self.mechanical_model_part.ProcessInfo[TIME]
+        tol = self.mechanical_model_part.ProcessInfo[DELTA_TIME]*1e-10
+        time_unit_converter = self.mechanical_model_part.ProcessInfo[TIME_UNIT_CONVERTER]
+
+        # Activation according the input file
+        with open(self.construction_input_file_name,'r') as file_name3:
+            for j, line in enumerate(file_name3):
+                file_3 = line.split(" ")
+                if ((len(file_3)) > 1 and (time >=(float(file_3[0])*time_unit_converter-tol))):
+                    print("New phase has been activated...")
+                    self.name_sub_thermal_part = "sub_Thermal_" + file_3[1]
+                    self.name_sub_mechanical_part = "sub_Parts_" + file_3[1]
+                    self.name_sub_heat_flux = "sub_TAmbientFlux3D_T_Ambient_Heat_Flux_" + file_3[1]
+                    self.name_sub_hydro_press = "sub_HydroSurfacePressure3D_Hydrostatic_Pressure_" + file_3[1]
+
+                    thermal_conditions = True
+                    mechanical_conditions = True
+                    try:
+                        self.thermal_model_part.GetSubModelPart(self.name_sub_heat_flux)
+                    except:
+                        thermal_conditions = False
+                    try:
+                        self.mechanical_model_part.GetSubModelPart(self.name_sub_hydro_press)
+                    except:
+                        mechanical_conditions = False
+
+                    self.Construction.InitializeSolutionStep(self.name_sub_thermal_part,self.name_sub_mechanical_part,self.name_sub_heat_flux,self.name_sub_hydro_press,thermal_conditions,mechanical_conditions,int(file_3[2]))
+
+    def InitializeSolutionStep(self):
+
+        time = self.mechanical_model_part.ProcessInfo[TIME]
+        tol = self.mechanical_model_part.ProcessInfo[DELTA_TIME]*1e-10
+        time_unit_converter = self.mechanical_model_part.ProcessInfo[TIME_UNIT_CONVERTER]
+
+        # Activation according the input file
+        with open(self.construction_input_file_name,'r') as file_name3:
+            for j, line in enumerate(file_name3):
+                file_3 = line.split(" ")
+                if ((len(file_3)) > 1 and ((time <=(float(file_3[0])*time_unit_converter+tol)) and (time >=(float(file_3[0])*time_unit_converter-tol)))):
+                    print("New phase has been activated...")
+                    self.name_sub_thermal_part = "sub_Thermal_" + file_3[1]
+                    self.name_sub_mechanical_part = "sub_Parts_" + file_3[1]
+                    self.name_sub_heat_flux = "sub_TAmbientFlux3D_T_Ambient_Heat_Flux_" + file_3[1]
+                    self.name_sub_hydro_press = "sub_HydroSurfacePressure3D_Hydrostatic_Pressure_" + file_3[1]
+
+                    thermal_conditions = True
+                    mechanical_conditions = True
+                    try:
+                        self.thermal_model_part.GetSubModelPart(self.name_sub_heat_flux)
+                    except:
+                        thermal_conditions = False
+                    try:
+                        self.mechanical_model_part.GetSubModelPart(self.name_sub_hydro_press)
+                    except:
+                        mechanical_conditions = False
+
+                    self.Construction.InitializeSolutionStep(self.name_sub_thermal_part,self.name_sub_mechanical_part,self.name_sub_heat_flux,self.name_sub_hydro_press,thermal_conditions,mechanical_conditions,int(file_3[2]))
+
+        # Check if the temperature of every nodes is in the range (it must be done each step)
+        if (self.activate_check_temperature):
+            print("Checking temperatures...")
+            self.Construction.CheckTemperature(self.check_temperature_parameters)
+
+        # Detection of fluxes (it must be done each step)
+        print("Searching free surfaces...")
+        self.Construction.SearchingFluxes()
+
+        # Contribution of heat source (it must be done each step)
+        print("Assigning heat source...")
+        if (self.heat_source_type == 'Noorzai'):
+            self.Construction.ActiveHeatFluxNoorzai(self.heat_source_parameters)
+
+        elif (self.heat_source_type == 'Azenha'):
+            self.Construction.ActiveHeatFluxAzenha(self.heat_source_parameters)
+
+
+    def AfterOutputStep(self):
+        self.Construction.AfterOutputStep()
+
+    def ExecuteFinalize(self):
+        pass
```

## KratosMultiphysics/DamApplication/dam_eigen_solver.py

```diff
@@ -1,164 +1,163 @@
-#import kratos core and applications
-import KratosMultiphysics
-import KratosMultiphysics.EigenSolversApplication as KratosEigen
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-import KratosMultiphysics.DamApplication as KratosDam
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-
-def CreateSolver(main_model_part, custom_settings):
-    return DamEigenSolver(main_model_part, custom_settings)
-
-class DamEigenSolver():
-
-    def __init__(self, main_model_part, custom_settings):
-
-        self.main_model_part = main_model_part
-
-        ##settings string in json format
-        default_settings = KratosMultiphysics.Parameters("""
-        {
-            "solver_type": "dam_eigen_solver",
-            "echo_level": 0,
-            "buffer_size": 1,
-            "solution_type": "Dynamic",
-            "analysis_type": "Linear",
-            "model_import_settings": {
-                "input_type": "mdpa",
-                "input_filename": "unknown_name",
-                "input_file_label": 0
-            },
-            "eigensolver_settings":{
-                "solver_type": "feast",
-                "echo_level" : 0,
-                "symmetric" : true,
-                "search_lowest_eigenvalues" : false,
-                "search_highest_eigenvalues" : false,
-                "compute_modal_contribution"  : false,
-                "e_min" : 0.0,
-                "e_max" : 500.0,
-                "subspace_size" : 4,
-                "number_of_eigenvalues" : 0
-            },
-            "problem_domain_sub_model_part_list": ["solid_model_part"],
-            "processes_sub_model_part_list": [""]
-        }
-        """)
-
-        ##overwrite the default settings with user-provided parameters
-        self.settings = custom_settings
-        self.settings.ValidateAndAssignDefaults(default_settings)
-
-        self.compute_modal_contribution = self.settings["eigensolver_settings"]["compute_modal_contribution"].GetBool()
-        self.settings["eigensolver_settings"].RemoveValue("compute_modal_contribution")
-
-        # eigensolver_settings are validated/assigned in the linear_solver
-        print("Construction of Dam Eigensolver finished")
-
-
-    def AddVariables(self):
-
-        # Add displacements
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
-        # Add dynamic variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
-        # Add reactions for the displacements
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
-
-        print("::[Dam EigenSolver]:: Variables ADDED")
-
-
-    def GetMinimumBufferSize(self):
-        return 2;
-
-
-    def AddDofs(self):
-
-        for node in self.main_model_part.Nodes:
-            # adding dofs
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_X, KratosMultiphysics.REACTION_X)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y, KratosMultiphysics.REACTION_Y)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z, KratosMultiphysics.REACTION_Z)
-
-        print("::[Dam EigenSolver]:: DOF's ADDED")
-
-
-    def ImportModelPart(self):
-
-        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
-
-            # Read ModelPart
-            KratosMultiphysics.ModelPartIO(self.settings["model_import_settings"]["input_filename"].GetString()).ReadModelPart(self.main_model_part)
-
-            # Create computing_model_part, set constitutive law and buffer size
-            self._ExecuteAfterReading()
-
-        else:
-            raise Exception("Other input options are not yet implemented.")
-
-        print ("Model reading finished")
-
-
-    def Initialize(self):
-
-        self.eigensolver_settings = self.settings["eigensolver_settings"]
-        solver_type = self.eigensolver_settings["solver_type"].GetString()
-        solution_type = self.settings["solution_type"].GetString()
-
-        if solver_type == "FEAST" or solver_type == "feast":
-            from KratosMultiphysics import eigen_solver_factory
-            self.linear_solver = eigen_solver_factory.ConstructSolver(self.eigensolver_settings)
-            mass_matrix_diagonal_value = 1.0
-            stiffness_matrix_diagonal_value = -1.0
-        else:
-            raise Exception("solver_type is not yet implemented.")
-
-        if solution_type == "Dynamic":
-            self.scheme = KratosStructural.EigensolverDynamicScheme()
-        else:
-            raise Exception("solution_type is not yet implemented.")
-
-        self.builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(self.linear_solver)
-
-        self.solver = KratosStructural.EigensolverStrategy(
-            self.main_model_part,
-            self.scheme,
-            self.builder_and_solver,
-            mass_matrix_diagonal_value,
-            stiffness_matrix_diagonal_value,
-            self.compute_modal_contribution)
-
-
-    def GetComputingModelPart(self):
-        return self.main_model_part.GetSubModelPart(self.computing_model_part_name)
-
-
-    def Solve(self):
-        self.solver.Solve()
-
-
-    def SetEchoLevel(self, level):
-        self.solver.SetEchoLevel(level)
-
-        #### Specific internal functions ####
-
-    def _ExecuteAfterReading(self):
-
-        self.computing_model_part_name = "mechanical_computing_domain"
-
-        # Auxiliary Kratos parameters object to be called by the CheckAndPepareModelProcess
-        aux_params = KratosMultiphysics.Parameters("{}")
-        aux_params.AddEmptyValue("computing_model_part_name").SetString(self.computing_model_part_name)
-
-        # CheckAndPrepareModelProcess creates the solid_computational_model_part
-        from KratosMultiphysics.PoromechanicsApplication import check_and_prepare_model_process_poro
-        check_and_prepare_model_process_poro.CheckAndPrepareModelProcess(self.main_model_part, aux_params).Execute()
-
-        # Constitutive law import
-        from KratosMultiphysics.DamApplication import dam_constitutive_law_utility
-        dam_constitutive_law_utility.SetConstitutiveLaw(self.main_model_part)
-
-        self.main_model_part.SetBufferSize( self.settings["buffer_size"].GetInt() )
-        minimum_buffer_size = self.GetMinimumBufferSize()
-        if(minimum_buffer_size > self.main_model_part.GetBufferSize()):
-            self.main_model_part.SetBufferSize( minimum_buffer_size )
+#import kratos core and applications
+import KratosMultiphysics
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+import KratosMultiphysics.DamApplication as KratosDam
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+
+def CreateSolver(main_model_part, custom_settings):
+    return DamEigenSolver(main_model_part, custom_settings)
+
+class DamEigenSolver():
+
+    def __init__(self, main_model_part, custom_settings):
+
+        self.main_model_part = main_model_part
+
+        ##settings string in json format
+        default_settings = KratosMultiphysics.Parameters("""
+        {
+            "solver_type": "dam_eigen_solver",
+            "echo_level": 0,
+            "buffer_size": 1,
+            "solution_type": "Dynamic",
+            "analysis_type": "Linear",
+            "model_import_settings": {
+                "input_type": "mdpa",
+                "input_filename": "unknown_name",
+                "input_file_label": 0
+            },
+            "eigensolver_settings":{
+                "solver_type": "feast",
+                "echo_level" : 0,
+                "symmetric" : true,
+                "search_lowest_eigenvalues" : false,
+                "search_highest_eigenvalues" : false,
+                "compute_modal_contribution"  : false,
+                "e_min" : 0.0,
+                "e_max" : 500.0,
+                "subspace_size" : 4,
+                "number_of_eigenvalues" : 0
+            },
+            "problem_domain_sub_model_part_list": ["solid_model_part"],
+            "processes_sub_model_part_list": [""]
+        }
+        """)
+
+        ##overwrite the default settings with user-provided parameters
+        self.settings = custom_settings
+        self.settings.ValidateAndAssignDefaults(default_settings)
+
+        self.compute_modal_contribution = self.settings["eigensolver_settings"]["compute_modal_contribution"].GetBool()
+        self.settings["eigensolver_settings"].RemoveValue("compute_modal_contribution")
+
+        # eigensolver_settings are validated/assigned in the linear_solver
+        print("Construction of Dam Eigensolver finished")
+
+
+    def AddVariables(self):
+
+        # Add displacements
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
+        # Add dynamic variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
+        # Add reactions for the displacements
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
+
+        print("::[Dam EigenSolver]:: Variables ADDED")
+
+
+    def GetMinimumBufferSize(self):
+        return 2
+
+
+    def AddDofs(self):
+
+        for node in self.main_model_part.Nodes:
+            # adding dofs
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_X, KratosMultiphysics.REACTION_X)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y, KratosMultiphysics.REACTION_Y)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z, KratosMultiphysics.REACTION_Z)
+
+        print("::[Dam EigenSolver]:: DOF's ADDED")
+
+
+    def ImportModelPart(self):
+
+        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
+
+            # Read ModelPart
+            KratosMultiphysics.ModelPartIO(self.settings["model_import_settings"]["input_filename"].GetString()).ReadModelPart(self.main_model_part)
+
+            # Create computing_model_part, set constitutive law and buffer size
+            self._ExecuteAfterReading()
+
+        else:
+            raise Exception("Other input options are not yet implemented.")
+
+        print ("Model reading finished")
+
+
+    def Initialize(self):
+
+        self.eigensolver_settings = self.settings["eigensolver_settings"]
+        solver_type = self.eigensolver_settings["solver_type"].GetString()
+        solution_type = self.settings["solution_type"].GetString()
+
+        if solver_type == "FEAST" or solver_type == "feast":
+            from KratosMultiphysics import eigen_solver_factory
+            self.linear_solver = eigen_solver_factory.ConstructSolver(self.eigensolver_settings)
+            mass_matrix_diagonal_value = 1.0
+            stiffness_matrix_diagonal_value = -1.0
+        else:
+            raise Exception("solver_type is not yet implemented.")
+
+        if solution_type == "Dynamic":
+            self.scheme = KratosStructural.EigensolverDynamicScheme()
+        else:
+            raise Exception("solution_type is not yet implemented.")
+
+        self.builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(self.linear_solver)
+
+        self.solver = KratosStructural.EigensolverStrategy(
+            self.main_model_part,
+            self.scheme,
+            self.builder_and_solver,
+            mass_matrix_diagonal_value,
+            stiffness_matrix_diagonal_value,
+            self.compute_modal_contribution)
+
+
+    def GetComputingModelPart(self):
+        return self.main_model_part.GetSubModelPart(self.computing_model_part_name)
+
+
+    def Solve(self):
+        self.solver.Solve()
+
+
+    def SetEchoLevel(self, level):
+        self.solver.SetEchoLevel(level)
+
+        #### Specific internal functions ####
+
+    def _ExecuteAfterReading(self):
+
+        self.computing_model_part_name = "mechanical_computing_domain"
+
+        # Auxiliary Kratos parameters object to be called by the CheckAndPepareModelProcess
+        aux_params = KratosMultiphysics.Parameters("{}")
+        aux_params.AddEmptyValue("computing_model_part_name").SetString(self.computing_model_part_name)
+
+        # CheckAndPrepareModelProcess creates the solid_computational_model_part
+        from KratosMultiphysics.PoromechanicsApplication import check_and_prepare_model_process_poro
+        check_and_prepare_model_process_poro.CheckAndPrepareModelProcess(self.main_model_part, aux_params).Execute()
+
+        # Constitutive law import
+        from KratosMultiphysics.DamApplication import dam_constitutive_law_utility
+        dam_constitutive_law_utility.SetConstitutiveLaw(self.main_model_part)
+
+        self.main_model_part.SetBufferSize( self.settings["buffer_size"].GetInt() )
+        minimum_buffer_size = self.GetMinimumBufferSize()
+        if(minimum_buffer_size > self.main_model_part.GetBufferSize()):
+            self.main_model_part.SetBufferSize( minimum_buffer_size )
```

## KratosMultiphysics/DamApplication/dam_mechanical_solver.py

 * *Ordering differences only*

```diff
@@ -1,409 +1,409 @@
-#import kratos core and applications
-import KratosMultiphysics
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-import KratosMultiphysics.DamApplication as KratosDam
-import json
-
-def CreateSolver(main_model_part, custom_settings):
-
-    return DamMechanicalSolver(main_model_part, custom_settings)
-
-
-class DamMechanicalSolver(object):
-
-    ##constructor. the constructor shall only take care of storing the settings
-    ##and the pointer to the main_model part. This is needed since at the point of constructing the
-    ##model part is still not filled and the variables are not yet allocated
-    ##
-    ##real construction shall be delayed to the function "Initialize" which
-    ##will be called once the model is already filled
-    def __init__(self, main_model_part, custom_settings):
-
-        #TODO: shall obtain the computing_model_part from the MODEL once the object is implemented
-        self.main_model_part = main_model_part
-
-        ##settings string in json format
-        default_settings = KratosMultiphysics.Parameters("""
-        {
-            "solver_type": "dam_mechanical_solver",
-            "model_import_settings":{
-                "input_type": "mdpa",
-                "input_filename": "unknown_name",
-                "input_file_label": 0
-            },
-            "buffer_size": 2,
-            "echo_level": 0,
-            "processes_sub_model_part_list": [""],
-            "mechanical_solver_settings":{
-                "echo_level": 0,
-                "reform_dofs_at_each_step": false,
-                "clear_storage": false,
-                "compute_reactions": false,
-                "move_mesh_flag": true,
-                "solution_type": "Quasi-Static",
-                "scheme_type": "Newmark",
-                "rayleigh_m": 0.0,
-                "rayleigh_k": 0.0,
-                "strategy_type": "Newton-Raphson",
-                "convergence_criterion": "Displacement_criterion",
-                "displacement_relative_tolerance": 1.0e-4,
-                "displacement_absolute_tolerance": 1.0e-9,
-                "residual_relative_tolerance": 1.0e-4,
-                "residual_absolute_tolerance": 1.0e-9,
-                "max_iteration": 15,
-                "desired_iterations": 4,
-                "max_radius_factor": 20.0,
-                "min_radius_factor": 0.5,
-                "block_builder": true,
-                "nonlocal_damage": false,
-                "characteristic_length": 0.05,
-                "search_neighbours_step": false,
-                "linear_solver_settings":{
-                    "solver_type": "amgcl",
-                    "tolerance": 1.0e-6,
-                    "max_iteration": 100,
-                    "scaling": false,
-                    "verbosity": 0,
-                    "preconditioner_type": "ilu0",
-                    "smoother_type": "ilu0",
-                    "krylov_type": "gmres",
-                    "coarsening_type": "aggregation"
-                },
-                "problem_domain_sub_model_part_list": [""],
-                "body_domain_sub_model_part_list": [],
-                "mechanical_loads_sub_model_part_list": [],
-                "loads_sub_model_part_list": [],
-                "loads_variable_list": []
-            }
-        }
-        """)
-
-        # Overwrite the default settings with user-provided parameters
-        self.settings = custom_settings
-        self.settings.ValidateAndAssignDefaults(default_settings)
-
-        # Construct the linear solver
-        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
-        self.linear_solver = linear_solver_factory.ConstructSolver(self.settings["mechanical_solver_settings"]["linear_solver_settings"])
-
-        print("Construction of DamMechanicalSolver finished")
-
-    def AddVariables(self):
-
-        ## Mechanical Variables
-        # Add displacements
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
-        # Add reactions for the displacements
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
-        # Add dynamic variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
-        # Add variables for the solid conditions
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_FACE_PRESSURE)
-        # Add volume acceleration
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VOLUME_ACCELERATION)
-        # Add variables for post-processing
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_AREA)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.INITIAL_NODAL_CAUCHY_STRESS_TENSOR)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Vi_POSITIVE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Viii_POSITIVE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_WIDTH)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_AREA)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.NODAL_YOUNG_MODULUS)
-
-        print("Variables correctly added")
-
-    def GetMinimumBufferSize(self):
-        return 2
-
-    def AddDofs(self):
-
-        for node in self.main_model_part.Nodes:
-            ## Solid dofs
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_X,KratosMultiphysics.REACTION_X)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y,KratosMultiphysics.REACTION_Y)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z,KratosMultiphysics.REACTION_Z)
-
-        if(self.settings["mechanical_solver_settings"]["solution_type"].GetString() == "Dynamic"):
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
-        print("DOFs correctly added")
-
-    def ImportModelPart(self):
-
-        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
-
-            # Read ModelPart
-            KratosMultiphysics.ModelPartIO(self.settings["model_import_settings"]["input_filename"].GetString()).ReadModelPart(self.main_model_part)
-
-            # Create computing_model_part, set constitutive law and buffer size
-            self._ExecuteAfterReading()
-
-        else:
-            raise Exception("Other input options are not yet implemented.")
-
-        print ("Model reading finished")
-
-    def Initialize(self):
-
-        # Builder and solver creation
-        builder_and_solver = self._ConstructBuilderAndSolver(self.settings["mechanical_solver_settings"]["block_builder"].GetBool())
-
-        # Solution scheme creation
-        scheme = self._ConstructScheme(self.settings["mechanical_solver_settings"]["scheme_type"].GetString(),
-                                         self.settings["mechanical_solver_settings"]["solution_type"].GetString())
-
-        # Get the convergence criterion
-        convergence_criterion = self._ConstructConvergenceCriterion(self.settings["mechanical_solver_settings"]["convergence_criterion"].GetString())
-
-        # Solver creation
-        self.Solver = self._ConstructSolver(builder_and_solver,
-                                            scheme,
-                                            convergence_criterion,
-                                            self.settings["mechanical_solver_settings"]["strategy_type"].GetString())
-
-        # Set echo_level
-        self.Solver.SetEchoLevel(self.settings["mechanical_solver_settings"]["echo_level"].GetInt())
-
-        # Check if everything is assigned correctly
-        self.Solver.Check()
-
-        print ("Initialization of DamMechanicalSolver finished")
-
-    def GetComputingModelPart(self):
-        return self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
-
-    def GetOutputVariables(self):
-        pass
-
-    def ComputeDeltaTime(self):
-        pass
-
-    def SaveRestart(self):
-        pass #one should write the restart file here
-
-    def Solve(self):
-        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
-            self.Clear()
-
-        self.Solver.Solve()
-
-    # solve :: sequencial calls
-
-    def InitializeStrategy(self):
-        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
-            self.Clear()
-
-        self.Solver.Initialize()
-
-    def InitializeSolutionStep(self):
-        self.Solver.InitializeSolutionStep()
-
-    def Predict(self):
-        self.Solver.Predict()
-
-    def SolveSolutionStep(self):
-        self.Solver.SolveSolutionStep()
-
-    def FinalizeSolutionStep(self):
-        self.Solver.FinalizeSolutionStep()
-
-    # solve :: sequencial calls
-
-    def SetEchoLevel(self, level):
-        self.Solver.SetEchoLevel(level)
-
-    def Clear(self):
-        self.Solver.Clear()
-
-    def Check(self):
-        self.Solver.Check()
-
-    #### Specific internal functions ####
-
-    def _ExecuteAfterReading(self):
-
-        self.mechanical_model_part_name = "mechanical_computing_domain"
-
-        # Create list of sub sub model parts (it is a copy of the standard lists with a different name)
-        self.body_domain_sub_sub_model_part_list = []
-        for i in range(self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"].size()):
-            self.body_domain_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"][i].GetString())
-        self.body_domain_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.body_domain_sub_sub_model_part_list))
-
-        self.loads_sub_sub_model_part_list = []
-        for i in range(self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"].size()):
-            self.loads_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"][i].GetString())
-        self.loads_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.loads_sub_sub_model_part_list))
-
-        # Auxiliary Kratos parameters object to be called by the CheckAndPepareModelProcess
-        aux_params = KratosMultiphysics.Parameters("{}")
-        aux_params.AddEmptyValue("mechanical_model_part_name").SetString(self.mechanical_model_part_name)
-        aux_params.AddValue("mechanical_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["problem_domain_sub_model_part_list"])
-        aux_params.AddValue("mechanical_loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["mechanical_loads_sub_model_part_list"])
-        aux_params.AddValue("body_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"])
-        aux_params.AddValue("body_domain_sub_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
-        aux_params.AddValue("loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"])
-        aux_params.AddValue("loads_sub_sub_model_part_list",self.loads_sub_sub_model_part_list)
-
-        # CheckAndPrepareModelProcess creates the solid_computational_model_part
-        from KratosMultiphysics.DamApplication import check_and_prepare_model_process_dam_mechanical
-        check_and_prepare_model_process_dam_mechanical.CheckAndPrepareModelProcessDamMechanical(self.main_model_part, aux_params).Execute()
-
-        # Constitutive law import
-        from KratosMultiphysics.DamApplication import dam_constitutive_law_utility
-        dam_constitutive_law_utility.SetConstitutiveLaw(self.main_model_part)
-
-        self.main_model_part.SetBufferSize( self.settings["buffer_size"].GetInt() )
-        minimum_buffer_size = self.GetMinimumBufferSize()
-        if(minimum_buffer_size > self.main_model_part.GetBufferSize()):
-            self.main_model_part.SetBufferSize( minimum_buffer_size )
-
-    def _ConstructBuilderAndSolver(self, block_builder):
-
-        # Creating the builder and solver
-        if(block_builder):
-            builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(self.linear_solver)
-        else:
-            builder_and_solver = KratosMultiphysics.ResidualBasedEliminationBuilderAndSolver(self.linear_solver)
-
-        return builder_and_solver
-
-    def _ConstructScheme(self, scheme_type, solution_type):
-
-        rayleigh_m = self.settings["mechanical_solver_settings"]["rayleigh_m"].GetDouble()
-        rayleigh_k = self.settings["mechanical_solver_settings"]["rayleigh_k"].GetDouble()
-
-        if(solution_type == "Quasi-Static"):
-            if(rayleigh_m<1.0e-15 and rayleigh_k<1.0e-15):
-                scheme =  KratosDam.IncrementalUpdateStaticSmoothingScheme()
-            else:
-                scheme =  KratosDam.IncrementalUpdateStaticDampedSmoothingScheme(rayleigh_m,rayleigh_k)
-        else:
-            if(scheme_type == "Newmark"):
-                damp_factor_m = 0.0
-            else:
-                damp_factor_m = -0.01
-            scheme = KratosDam.BossakDisplacementSmoothingScheme(damp_factor_m,rayleigh_m,rayleigh_k)
-
-        return scheme
-
-    def _ConstructConvergenceCriterion(self, convergence_criterion):
-
-        D_RT = self.settings["mechanical_solver_settings"]["displacement_relative_tolerance"].GetDouble()
-        D_AT = self.settings["mechanical_solver_settings"]["displacement_absolute_tolerance"].GetDouble()
-        R_RT = self.settings["mechanical_solver_settings"]["residual_relative_tolerance"].GetDouble()
-        R_AT = self.settings["mechanical_solver_settings"]["residual_absolute_tolerance"].GetDouble()
-        echo_level = self.settings["mechanical_solver_settings"]["echo_level"].GetInt()
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
-    def _ConstructSolver(self, builder_and_solver, scheme, convergence_criterion, strategy_type):
-
-        nonlocal_damage = self.settings["mechanical_solver_settings"]["nonlocal_damage"].GetBool()
-        max_iters = self.settings["mechanical_solver_settings"]["max_iteration"].GetInt()
-        compute_reactions = self.settings["mechanical_solver_settings"]["compute_reactions"].GetBool()
-        reform_step_dofs = self.settings["mechanical_solver_settings"]["reform_dofs_at_each_step"].GetBool()
-        move_mesh_flag = self.settings["mechanical_solver_settings"]["move_mesh_flag"].GetBool()
-
-        if strategy_type == "Newton-Raphson":
-            if nonlocal_damage:
-                self.strategy_params = KratosMultiphysics.Parameters("{}")
-                self.strategy_params.AddValue("loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"])
-                self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
-                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"])
-                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
-                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
-                solver = KratosPoro.PoromechanicsNewtonRaphsonNonlocalStrategy(self.main_model_part,
-                                                                               scheme,
-                                                                               convergence_criterion,
-                                                                               builder_and_solver,
-                                                                               self.strategy_params,
-                                                                               max_iters,
-                                                                               compute_reactions,
-                                                                               reform_step_dofs,
-                                                                               move_mesh_flag)
-            else:
-                self.main_model_part.ProcessInfo.SetValue(KratosPoro.IS_CONVERGED, True)
-                solver = KratosMultiphysics.ResidualBasedNewtonRaphsonStrategy(self.main_model_part,
-                                                                               scheme,
-                                                                               convergence_criterion,
-                                                                               builder_and_solver,
-                                                                               max_iters,
-                                                                               compute_reactions,
-                                                                               reform_step_dofs,
-                                                                               move_mesh_flag)
-        else:
-            # Arc-Length strategy
-            self.strategy_params = KratosMultiphysics.Parameters("{}")
-            self.strategy_params.AddValue("desired_iterations",self.settings["mechanical_solver_settings"]["desired_iterations"])
-            self.strategy_params.AddValue("max_radius_factor",self.settings["mechanical_solver_settings"]["max_radius_factor"])
-            self.strategy_params.AddValue("min_radius_factor",self.settings["mechanical_solver_settings"]["min_radius_factor"])
-            self.strategy_params.AddValue("loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"])
-            self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
-            if nonlocal_damage:
-                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"])
-                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
-                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
-                solver = KratosPoro.PoromechanicsRammArcLengthNonlocalStrategy(self.main_model_part,
-                                                                               scheme,
-                                                                               self.linear_solver,
-                                                                               convergence_criterion,
-                                                                               builder_and_solver,
-                                                                               self.strategy_params,
-                                                                               max_iters,
-                                                                               compute_reactions,
-                                                                               reform_step_dofs,
-                                                                               move_mesh_flag)
-            else:
-                solver = KratosPoro.PoromechanicsRammArcLengthStrategy(self.main_model_part,
-                                                                       scheme,
-                                                                       self.linear_solver,
-                                                                       convergence_criterion,
-                                                                       builder_and_solver,
-                                                                       self.strategy_params,
-                                                                       max_iters,
-                                                                       compute_reactions,
-                                                                       reform_step_dofs,
-                                                                       move_mesh_flag)
-
-        return solver
-
-    def _CheckConvergence(self):
-
-        IsConverged = self.Solver.IsConverged()
-
-        return IsConverged
-
-    def _UpdateLoads(self):
-
-        self.Solver.UpdateLoads()
+#import kratos core and applications
+import KratosMultiphysics
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+import KratosMultiphysics.DamApplication as KratosDam
+import json
+
+def CreateSolver(main_model_part, custom_settings):
+
+    return DamMechanicalSolver(main_model_part, custom_settings)
+
+
+class DamMechanicalSolver(object):
+
+    ##constructor. the constructor shall only take care of storing the settings
+    ##and the pointer to the main_model part. This is needed since at the point of constructing the
+    ##model part is still not filled and the variables are not yet allocated
+    ##
+    ##real construction shall be delayed to the function "Initialize" which
+    ##will be called once the model is already filled
+    def __init__(self, main_model_part, custom_settings):
+
+        #TODO: shall obtain the computing_model_part from the MODEL once the object is implemented
+        self.main_model_part = main_model_part
+
+        ##settings string in json format
+        default_settings = KratosMultiphysics.Parameters("""
+        {
+            "solver_type": "dam_mechanical_solver",
+            "model_import_settings":{
+                "input_type": "mdpa",
+                "input_filename": "unknown_name",
+                "input_file_label": 0
+            },
+            "buffer_size": 2,
+            "echo_level": 0,
+            "processes_sub_model_part_list": [""],
+            "mechanical_solver_settings":{
+                "echo_level": 0,
+                "reform_dofs_at_each_step": false,
+                "clear_storage": false,
+                "compute_reactions": false,
+                "move_mesh_flag": true,
+                "solution_type": "Quasi-Static",
+                "scheme_type": "Newmark",
+                "rayleigh_m": 0.0,
+                "rayleigh_k": 0.0,
+                "strategy_type": "Newton-Raphson",
+                "convergence_criterion": "Displacement_criterion",
+                "displacement_relative_tolerance": 1.0e-4,
+                "displacement_absolute_tolerance": 1.0e-9,
+                "residual_relative_tolerance": 1.0e-4,
+                "residual_absolute_tolerance": 1.0e-9,
+                "max_iteration": 15,
+                "desired_iterations": 4,
+                "max_radius_factor": 20.0,
+                "min_radius_factor": 0.5,
+                "block_builder": true,
+                "nonlocal_damage": false,
+                "characteristic_length": 0.05,
+                "search_neighbours_step": false,
+                "linear_solver_settings":{
+                    "solver_type": "amgcl",
+                    "tolerance": 1.0e-6,
+                    "max_iteration": 100,
+                    "scaling": false,
+                    "verbosity": 0,
+                    "preconditioner_type": "ilu0",
+                    "smoother_type": "ilu0",
+                    "krylov_type": "gmres",
+                    "coarsening_type": "aggregation"
+                },
+                "problem_domain_sub_model_part_list": [""],
+                "body_domain_sub_model_part_list": [],
+                "mechanical_loads_sub_model_part_list": [],
+                "loads_sub_model_part_list": [],
+                "loads_variable_list": []
+            }
+        }
+        """)
+
+        # Overwrite the default settings with user-provided parameters
+        self.settings = custom_settings
+        self.settings.ValidateAndAssignDefaults(default_settings)
+
+        # Construct the linear solver
+        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
+        self.linear_solver = linear_solver_factory.ConstructSolver(self.settings["mechanical_solver_settings"]["linear_solver_settings"])
+
+        print("Construction of DamMechanicalSolver finished")
+
+    def AddVariables(self):
+
+        ## Mechanical Variables
+        # Add displacements
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
+        # Add reactions for the displacements
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
+        # Add dynamic variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
+        # Add variables for the solid conditions
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_FACE_PRESSURE)
+        # Add volume acceleration
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VOLUME_ACCELERATION)
+        # Add variables for post-processing
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_AREA)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.INITIAL_NODAL_CAUCHY_STRESS_TENSOR)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Vi_POSITIVE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Viii_POSITIVE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_WIDTH)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_AREA)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.NODAL_YOUNG_MODULUS)
+
+        print("Variables correctly added")
+
+    def GetMinimumBufferSize(self):
+        return 2
+
+    def AddDofs(self):
+
+        for node in self.main_model_part.Nodes:
+            ## Solid dofs
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_X,KratosMultiphysics.REACTION_X)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y,KratosMultiphysics.REACTION_Y)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z,KratosMultiphysics.REACTION_Z)
+
+        if(self.settings["mechanical_solver_settings"]["solution_type"].GetString() == "Dynamic"):
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
+        print("DOFs correctly added")
+
+    def ImportModelPart(self):
+
+        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
+
+            # Read ModelPart
+            KratosMultiphysics.ModelPartIO(self.settings["model_import_settings"]["input_filename"].GetString()).ReadModelPart(self.main_model_part)
+
+            # Create computing_model_part, set constitutive law and buffer size
+            self._ExecuteAfterReading()
+
+        else:
+            raise Exception("Other input options are not yet implemented.")
+
+        print ("Model reading finished")
+
+    def Initialize(self):
+
+        # Builder and solver creation
+        builder_and_solver = self._ConstructBuilderAndSolver(self.settings["mechanical_solver_settings"]["block_builder"].GetBool())
+
+        # Solution scheme creation
+        scheme = self._ConstructScheme(self.settings["mechanical_solver_settings"]["scheme_type"].GetString(),
+                                         self.settings["mechanical_solver_settings"]["solution_type"].GetString())
+
+        # Get the convergence criterion
+        convergence_criterion = self._ConstructConvergenceCriterion(self.settings["mechanical_solver_settings"]["convergence_criterion"].GetString())
+
+        # Solver creation
+        self.Solver = self._ConstructSolver(builder_and_solver,
+                                            scheme,
+                                            convergence_criterion,
+                                            self.settings["mechanical_solver_settings"]["strategy_type"].GetString())
+
+        # Set echo_level
+        self.Solver.SetEchoLevel(self.settings["mechanical_solver_settings"]["echo_level"].GetInt())
+
+        # Check if everything is assigned correctly
+        self.Solver.Check()
+
+        print ("Initialization of DamMechanicalSolver finished")
+
+    def GetComputingModelPart(self):
+        return self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
+
+    def GetOutputVariables(self):
+        pass
+
+    def ComputeDeltaTime(self):
+        pass
+
+    def SaveRestart(self):
+        pass #one should write the restart file here
+
+    def Solve(self):
+        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
+            self.Clear()
+
+        self.Solver.Solve()
+
+    # solve :: sequencial calls
+
+    def InitializeStrategy(self):
+        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
+            self.Clear()
+
+        self.Solver.Initialize()
+
+    def InitializeSolutionStep(self):
+        self.Solver.InitializeSolutionStep()
+
+    def Predict(self):
+        self.Solver.Predict()
+
+    def SolveSolutionStep(self):
+        self.Solver.SolveSolutionStep()
+
+    def FinalizeSolutionStep(self):
+        self.Solver.FinalizeSolutionStep()
+
+    # solve :: sequencial calls
+
+    def SetEchoLevel(self, level):
+        self.Solver.SetEchoLevel(level)
+
+    def Clear(self):
+        self.Solver.Clear()
+
+    def Check(self):
+        self.Solver.Check()
+
+    #### Specific internal functions ####
+
+    def _ExecuteAfterReading(self):
+
+        self.mechanical_model_part_name = "mechanical_computing_domain"
+
+        # Create list of sub sub model parts (it is a copy of the standard lists with a different name)
+        self.body_domain_sub_sub_model_part_list = []
+        for i in range(self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"].size()):
+            self.body_domain_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"][i].GetString())
+        self.body_domain_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.body_domain_sub_sub_model_part_list))
+
+        self.loads_sub_sub_model_part_list = []
+        for i in range(self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"].size()):
+            self.loads_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"][i].GetString())
+        self.loads_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.loads_sub_sub_model_part_list))
+
+        # Auxiliary Kratos parameters object to be called by the CheckAndPepareModelProcess
+        aux_params = KratosMultiphysics.Parameters("{}")
+        aux_params.AddEmptyValue("mechanical_model_part_name").SetString(self.mechanical_model_part_name)
+        aux_params.AddValue("mechanical_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["problem_domain_sub_model_part_list"])
+        aux_params.AddValue("mechanical_loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["mechanical_loads_sub_model_part_list"])
+        aux_params.AddValue("body_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"])
+        aux_params.AddValue("body_domain_sub_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
+        aux_params.AddValue("loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"])
+        aux_params.AddValue("loads_sub_sub_model_part_list",self.loads_sub_sub_model_part_list)
+
+        # CheckAndPrepareModelProcess creates the solid_computational_model_part
+        from KratosMultiphysics.DamApplication import check_and_prepare_model_process_dam_mechanical
+        check_and_prepare_model_process_dam_mechanical.CheckAndPrepareModelProcessDamMechanical(self.main_model_part, aux_params).Execute()
+
+        # Constitutive law import
+        from KratosMultiphysics.DamApplication import dam_constitutive_law_utility
+        dam_constitutive_law_utility.SetConstitutiveLaw(self.main_model_part)
+
+        self.main_model_part.SetBufferSize( self.settings["buffer_size"].GetInt() )
+        minimum_buffer_size = self.GetMinimumBufferSize()
+        if(minimum_buffer_size > self.main_model_part.GetBufferSize()):
+            self.main_model_part.SetBufferSize( minimum_buffer_size )
+
+    def _ConstructBuilderAndSolver(self, block_builder):
+
+        # Creating the builder and solver
+        if(block_builder):
+            builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(self.linear_solver)
+        else:
+            builder_and_solver = KratosMultiphysics.ResidualBasedEliminationBuilderAndSolver(self.linear_solver)
+
+        return builder_and_solver
+
+    def _ConstructScheme(self, scheme_type, solution_type):
+
+        rayleigh_m = self.settings["mechanical_solver_settings"]["rayleigh_m"].GetDouble()
+        rayleigh_k = self.settings["mechanical_solver_settings"]["rayleigh_k"].GetDouble()
+
+        if(solution_type == "Quasi-Static"):
+            if(rayleigh_m<1.0e-15 and rayleigh_k<1.0e-15):
+                scheme =  KratosDam.IncrementalUpdateStaticSmoothingScheme()
+            else:
+                scheme =  KratosDam.IncrementalUpdateStaticDampedSmoothingScheme(rayleigh_m,rayleigh_k)
+        else:
+            if(scheme_type == "Newmark"):
+                damp_factor_m = 0.0
+            else:
+                damp_factor_m = -0.01
+            scheme = KratosDam.BossakDisplacementSmoothingScheme(damp_factor_m,rayleigh_m,rayleigh_k)
+
+        return scheme
+
+    def _ConstructConvergenceCriterion(self, convergence_criterion):
+
+        D_RT = self.settings["mechanical_solver_settings"]["displacement_relative_tolerance"].GetDouble()
+        D_AT = self.settings["mechanical_solver_settings"]["displacement_absolute_tolerance"].GetDouble()
+        R_RT = self.settings["mechanical_solver_settings"]["residual_relative_tolerance"].GetDouble()
+        R_AT = self.settings["mechanical_solver_settings"]["residual_absolute_tolerance"].GetDouble()
+        echo_level = self.settings["mechanical_solver_settings"]["echo_level"].GetInt()
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
+    def _ConstructSolver(self, builder_and_solver, scheme, convergence_criterion, strategy_type):
+
+        nonlocal_damage = self.settings["mechanical_solver_settings"]["nonlocal_damage"].GetBool()
+        max_iters = self.settings["mechanical_solver_settings"]["max_iteration"].GetInt()
+        compute_reactions = self.settings["mechanical_solver_settings"]["compute_reactions"].GetBool()
+        reform_step_dofs = self.settings["mechanical_solver_settings"]["reform_dofs_at_each_step"].GetBool()
+        move_mesh_flag = self.settings["mechanical_solver_settings"]["move_mesh_flag"].GetBool()
+
+        if strategy_type == "Newton-Raphson":
+            if nonlocal_damage:
+                self.strategy_params = KratosMultiphysics.Parameters("{}")
+                self.strategy_params.AddValue("loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"])
+                self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
+                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"])
+                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
+                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
+                solver = KratosPoro.PoromechanicsNewtonRaphsonNonlocalStrategy(self.main_model_part,
+                                                                               scheme,
+                                                                               convergence_criterion,
+                                                                               builder_and_solver,
+                                                                               self.strategy_params,
+                                                                               max_iters,
+                                                                               compute_reactions,
+                                                                               reform_step_dofs,
+                                                                               move_mesh_flag)
+            else:
+                self.main_model_part.ProcessInfo.SetValue(KratosPoro.IS_CONVERGED, True)
+                solver = KratosMultiphysics.ResidualBasedNewtonRaphsonStrategy(self.main_model_part,
+                                                                               scheme,
+                                                                               convergence_criterion,
+                                                                               builder_and_solver,
+                                                                               max_iters,
+                                                                               compute_reactions,
+                                                                               reform_step_dofs,
+                                                                               move_mesh_flag)
+        else:
+            # Arc-Length strategy
+            self.strategy_params = KratosMultiphysics.Parameters("{}")
+            self.strategy_params.AddValue("desired_iterations",self.settings["mechanical_solver_settings"]["desired_iterations"])
+            self.strategy_params.AddValue("max_radius_factor",self.settings["mechanical_solver_settings"]["max_radius_factor"])
+            self.strategy_params.AddValue("min_radius_factor",self.settings["mechanical_solver_settings"]["min_radius_factor"])
+            self.strategy_params.AddValue("loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"])
+            self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
+            if nonlocal_damage:
+                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"])
+                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
+                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
+                solver = KratosPoro.PoromechanicsRammArcLengthNonlocalStrategy(self.main_model_part,
+                                                                               scheme,
+                                                                               self.linear_solver,
+                                                                               convergence_criterion,
+                                                                               builder_and_solver,
+                                                                               self.strategy_params,
+                                                                               max_iters,
+                                                                               compute_reactions,
+                                                                               reform_step_dofs,
+                                                                               move_mesh_flag)
+            else:
+                solver = KratosPoro.PoromechanicsRammArcLengthStrategy(self.main_model_part,
+                                                                       scheme,
+                                                                       self.linear_solver,
+                                                                       convergence_criterion,
+                                                                       builder_and_solver,
+                                                                       self.strategy_params,
+                                                                       max_iters,
+                                                                       compute_reactions,
+                                                                       reform_step_dofs,
+                                                                       move_mesh_flag)
+
+        return solver
+
+    def _CheckConvergence(self):
+
+        IsConverged = self.Solver.IsConverged()
+
+        return IsConverged
+
+    def _UpdateLoads(self):
+
+        self.Solver.UpdateLoads()
```

## KratosMultiphysics/DamApplication/dam_selfweight_solver.py

 * *Ordering differences only*

```diff
@@ -1,441 +1,441 @@
-#import kratos core and applications
-import KratosMultiphysics
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-import KratosMultiphysics.DamApplication as KratosDam
-import json
-
-def CreateSolver(main_model_part, custom_settings):
-
-    return DamSelfweightSolver(main_model_part, custom_settings)
-
-
-class DamSelfweightSolver(object):
-
-    ##constructor. the constructor shall only take care of storing the settings
-    ##and the pointer to the main_model part. This is needed since at the point of constructing the
-    ##model part is still not filled and the variables are not yet allocated
-    ##
-    ##real construction shall be delayed to the function "Initialize" which
-    ##will be called once the model is already filled
-    def __init__(self, main_model_part, custom_settings):
-
-        #TODO: shall obtain the computing_model_part from the MODEL once the object is implemented
-        self.main_model_part = main_model_part
-
-        ##settings string in json format
-        default_settings = KratosMultiphysics.Parameters("""
-        {
-            "solver_type": "dam_selfweight_solver",
-            "model_import_settings":{
-                "input_type": "mdpa",
-                "input_filename": "unknown_name",
-                "input_file_label": 0
-            },
-            "echo_level": 0,
-            "buffer_size": 2,
-            "processes_sub_model_part_list": [""],
-            "mechanical_solver_settings":{
-                "echo_level": 0,
-                "reform_dofs_at_each_step": false,
-                "clear_storage": false,
-                "compute_reactions": false,
-                "move_mesh_flag": true,
-                "solution_type": "Quasi-Static",
-                "scheme_type": "Newmark",
-                "rayleigh_m": 0.0,
-                "rayleigh_k": 0.0,
-                "strategy_type": "Newton-Raphson",
-                "convergence_criterion": "Displacement_criterion",
-                "displacement_relative_tolerance": 1.0e-4,
-                "displacement_absolute_tolerance": 1.0e-9,
-                "residual_relative_tolerance": 1.0e-4,
-                "residual_absolute_tolerance": 1.0e-9,
-                "max_iteration": 15,
-                "desired_iterations": 4,
-                "max_radius_factor": 20.0,
-                "min_radius_factor": 0.5,
-                "block_builder": true,
-                "nonlocal_damage": false,
-                "characteristic_length": 0.05,
-                "search_neighbours_step": false,
-                "linear_solver_settings":{
-                    "solver_type": "amgcl",
-                    "tolerance": 1.0e-6,
-                    "max_iteration": 100,
-                    "scaling": false,
-                    "verbosity": 0,
-                    "preconditioner_type": "ilu0",
-                    "smoother_type": "ilu0",
-                    "krylov_type": "gmres",
-                    "coarsening_type": "aggregation"
-                },
-                "problem_domain_sub_model_part_list": [""],
-                "body_domain_sub_model_part_list": [],
-                "mechanical_loads_sub_model_part_list": [],
-                "loads_sub_model_part_list": [],
-                "loads_variable_list": []
-            }
-        }
-        """)
-
-        # Overwrite the default settings with user-provided parameters
-        self.settings = custom_settings
-        self.settings.ValidateAndAssignDefaults(default_settings)
-
-        # Construct the linear solver
-        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
-        self.mechanical_linear_solver = linear_solver_factory.ConstructSolver(self.settings["mechanical_solver_settings"]["linear_solver_settings"])
-
-        print("Construction of DamSelfweightSolver finished")
-
-    def AddVariables(self):
-
-        ## Mechanical Variables
-        # Add displacements
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
-        # Add reactions for the displacements
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
-        # Add dynamic variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
-        # Add variables for the solid conditions
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_FACE_PRESSURE)
-        # Add volume acceleration
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VOLUME_ACCELERATION)
-        # Add variables for post-processing
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_AREA)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.INITIAL_NODAL_CAUCHY_STRESS_TENSOR)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Vi_POSITIVE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Viii_POSITIVE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_WIDTH)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_AREA)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.NODAL_YOUNG_MODULUS)
-
-        ## Thermal variables
-        thermal_settings = KratosMultiphysics.ConvectionDiffusionSettings()
-        thermal_settings.SetDiffusionVariable(KratosMultiphysics.CONDUCTIVITY)
-        thermal_settings.SetUnknownVariable(KratosMultiphysics.TEMPERATURE)
-        thermal_settings.SetSpecificHeatVariable(KratosMultiphysics.SPECIFIC_HEAT)
-        thermal_settings.SetDensityVariable(KratosMultiphysics.DENSITY)
-        thermal_settings.SetVolumeSourceVariable(KratosMultiphysics.HEAT_FLUX)
-        thermal_settings.SetSurfaceSourceVariable(KratosMultiphysics.FACE_HEAT_FLUX)
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.CONVECTION_DIFFUSION_SETTINGS, thermal_settings)
-
-        # Add thermal variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.CONDUCTIVITY)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.TEMPERATURE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.SPECIFIC_HEAT)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DENSITY)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.HEAT_FLUX)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FACE_HEAT_FLUX)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.NODAL_REFERENCE_TEMPERATURE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.PLACEMENT_TEMPERATURE)
-
-        # This Variable is used for computing heat source according Azenha Formulation
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.ALPHA_HEAT_SOURCE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.TIME_ACTIVATION)
-
-        print("Variables correctly added")
-
-    @classmethod
-    def GetMinimumBufferSize(self):
-        return 2
-
-    def AddDofs(self):
-
-        for node in self.main_model_part.Nodes:
-            ## Solid dofs
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_X,KratosMultiphysics.REACTION_X)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y,KratosMultiphysics.REACTION_Y)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z,KratosMultiphysics.REACTION_Z)
-
-        if(self.settings["mechanical_solver_settings"]["solution_type"].GetString() == "Dynamic"):
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
-        print("DOFs correctly added")
-
-    def ImportModelPart(self):
-
-        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
-
-            # Read ModelPart
-            KratosMultiphysics.ModelPartIO(self.settings["model_import_settings"]["input_filename"].GetString()).ReadModelPart(self.main_model_part)
-
-            # Create computing_model_part, set constitutive law and buffer size
-            self._ExecuteAfterReading()
-
-        else:
-            raise Exception("Other input options are not yet implemented.")
-
-        print ("Model reading finished")
-
-    def Initialize(self):
-
-
-        # Get the computing model parts
-        self.mechanical_computing_model_part = self.GetComputingModelPart()
-
-        # Builder and solver creation
-        mechanical_builder_and_solver = self._ConstructBuilderAndSolver(self.settings["mechanical_solver_settings"]["block_builder"].GetBool(),self.mechanical_linear_solver)
-
-        # Solution scheme creation
-        mechanical_scheme = self._ConstructScheme(self.settings["mechanical_solver_settings"]["scheme_type"].GetString(),
-                                         self.settings["mechanical_solver_settings"]["solution_type"].GetString())
-
-        # Get the convergence criterion
-        convergence_criterion = self._ConstructConvergenceCriterion(self.settings["mechanical_solver_settings"]["convergence_criterion"].GetString())
-
-        # Solver creation
-        self.Selfweight_Solver = self._ConstructSolver(mechanical_builder_and_solver,
-                                            mechanical_scheme,
-                                            convergence_criterion,
-                                            self.settings["mechanical_solver_settings"]["strategy_type"].GetString())
-
-        # Set echo_level
-        self.Selfweight_Solver.SetEchoLevel(self.settings["mechanical_solver_settings"]["echo_level"].GetInt())
-
-        # Check if everything is assigned correctly
-        self.Selfweight_Solver.Check()
-
-        print ("Initialization of DamSelfweightSolver finished")
-
-    def GetComputingModelPart(self):
-        return self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
-
-    def GetOutputVariables(self):
-        pass
-
-    def ComputeDeltaTime(self):
-        pass
-
-    def SaveRestart(self):
-        pass #one should write the restart file here
-
-    def Solve(self):
-        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
-            self.Selfweight_Solver.Clear()
-
-        self.Selfweight_Solver.Solve()
-
-    # solve :: sequencial calls
-
-    def InitializeStrategy(self):
-        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
-            self.Selfweight_Solver.Clear()
-
-        self.Selfweight_Solver.Initialize()
-
-    def InitializeSolutionStep(self):
-        self.Selfweight_Solver.InitializeSolutionStep()
-
-    def Predict(self):
-        self.Selfweight_Solver.Predict()
-
-    def SolveSolutionStep(self):
-        self.Selfweight_Solver.SolveSolutionStep()
-
-    def FinalizeSolutionStep(self):
-        self.Selfweight_Solver.FinalizeSolutionStep()
-
-    # solve :: sequencial calls
-
-    def SetEchoLevel(self, level):
-
-        self.Selfweight_Solver.SetEchoLevel(level)
-
-    def Clear(self):
-
-        self.Selfweight_Solver.Clear()
-
-    def Check(self):
-
-        self.Selfweight_Solver.Check()
-
-    #### Specific internal functions ####
-
-    def _ExecuteAfterReading(self):
-
-        self.mechanical_model_part_name = "mechanical_computing_domain"
-
-        self.body_domain_sub_sub_model_part_list = []
-        for i in range(self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"].size()):
-            self.body_domain_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"][i].GetString())
-        self.body_domain_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.body_domain_sub_sub_model_part_list))
-
-        self.loads_sub_sub_model_part_list = []
-        for i in range(self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"].size()):
-            self.loads_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"][i].GetString())
-        self.loads_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.loads_sub_sub_model_part_list))
-
-        # Auxiliary Kratos parameters object to be called by the CheckAndPepareModelProcess
-        aux_params = KratosMultiphysics.Parameters("{}")
-        aux_params.AddEmptyValue("mechanical_model_part_name").SetString(self.mechanical_model_part_name)
-        aux_params.AddValue("mechanical_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["problem_domain_sub_model_part_list"])
-        aux_params.AddValue("mechanical_loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["mechanical_loads_sub_model_part_list"])
-        aux_params.AddValue("body_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"])
-        aux_params.AddValue("body_domain_sub_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
-        aux_params.AddValue("loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"])
-        aux_params.AddValue("loads_sub_sub_model_part_list",self.loads_sub_sub_model_part_list)
-
-        # CheckAndPrepareModelProcess creates the solid_computational_model_part
-        from KratosMultiphysics.DamApplication import check_and_prepare_selfweight_model_process_dam
-        check_and_prepare_selfweight_model_process_dam.CheckAndPrepareSelfweightModelProcess(self.main_model_part, aux_params).Execute()
-
-        # Constitutive law import
-        from KratosMultiphysics.DamApplication import dam_constitutive_law_utility
-        dam_constitutive_law_utility.SetConstitutiveLaw(self.main_model_part)
-
-        self.main_model_part.SetBufferSize( self.settings["buffer_size"].GetInt() )
-        minimum_buffer_size = self.GetMinimumBufferSize()
-        if(minimum_buffer_size > self.main_model_part.GetBufferSize()):
-            self.main_model_part.SetBufferSize( minimum_buffer_size )
-
-    @classmethod
-    def _ConstructBuilderAndSolver(self, block_builder, linear_solver):
-
-        # Creating the builder and solver
-        if(block_builder):
-            builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(linear_solver)
-        else:
-            builder_and_solver = KratosMultiphysics.ResidualBasedEliminationBuilderAndSolver(linear_solver)
-
-        return builder_and_solver
-
-    def _ConstructScheme(self, scheme_type, solution_type):
-
-        rayleigh_m = self.settings["mechanical_solver_settings"]["rayleigh_m"].GetDouble()
-        rayleigh_k = self.settings["mechanical_solver_settings"]["rayleigh_k"].GetDouble()
-
-        if(solution_type == "Quasi-Static"):
-            if(rayleigh_m<1.0e-15 and rayleigh_k<1.0e-15):
-                scheme =  KratosDam.IncrementalUpdateStaticSmoothingScheme()
-            else:
-                scheme =  KratosDam.IncrementalUpdateStaticDampedSmoothingScheme(rayleigh_m,rayleigh_k)
-        else:
-            if(scheme_type == "Newmark"):
-                damp_factor_m = 0.0
-            else:
-                damp_factor_m = -0.01
-            scheme = KratosDam.BossakDisplacementSmoothingScheme(damp_factor_m,rayleigh_m,rayleigh_k)
-
-        return scheme
-
-    def _ConstructConvergenceCriterion(self, convergence_criterion):
-
-        D_RT = self.settings["mechanical_solver_settings"]["displacement_relative_tolerance"].GetDouble()
-        D_AT = self.settings["mechanical_solver_settings"]["displacement_absolute_tolerance"].GetDouble()
-        R_RT = self.settings["mechanical_solver_settings"]["residual_relative_tolerance"].GetDouble()
-        R_AT = self.settings["mechanical_solver_settings"]["residual_absolute_tolerance"].GetDouble()
-        echo_level = self.settings["mechanical_solver_settings"]["echo_level"].GetInt()
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
-    def _ConstructSolver(self, builder_and_solver, scheme, convergence_criterion, strategy_type):
-
-        nonlocal_damage = self.settings["mechanical_solver_settings"]["nonlocal_damage"].GetBool()
-        max_iters = self.settings["mechanical_solver_settings"]["max_iteration"].GetInt()
-        compute_reactions = self.settings["mechanical_solver_settings"]["compute_reactions"].GetBool()
-        reform_step_dofs = self.settings["mechanical_solver_settings"]["reform_dofs_at_each_step"].GetBool()
-        move_mesh_flag = self.settings["mechanical_solver_settings"]["move_mesh_flag"].GetBool()
-
-        if strategy_type == "Newton-Raphson":
-            if nonlocal_damage:
-                self.strategy_params = KratosMultiphysics.Parameters("{}")
-                self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
-                self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
-                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
-                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
-                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
-                solver = KratosPoro.PoromechanicsNewtonRaphsonNonlocalStrategy(self.mechanical_computing_model_part,
-                                                                               scheme,
-                                                                               convergence_criterion,
-                                                                               builder_and_solver,
-                                                                               self.strategy_params,
-                                                                               max_iters,
-                                                                               compute_reactions,
-                                                                               reform_step_dofs,
-                                                                               move_mesh_flag)
-            else:
-                self.main_model_part.ProcessInfo.SetValue(KratosPoro.IS_CONVERGED, True)
-                solver = KratosMultiphysics.ResidualBasedNewtonRaphsonStrategy(self.mechanical_computing_model_part,
-                                                                                    scheme,
-                                                                                    convergence_criterion,
-                                                                                    builder_and_solver,
-                                                                                    max_iters,
-                                                                                    compute_reactions,
-                                                                                    reform_step_dofs,
-                                                                                    move_mesh_flag)
-        else:
-            # Arc-Length strategy
-            self.strategy_params = KratosMultiphysics.Parameters("{}")
-            self.strategy_params.AddValue("desired_iterations",self.settings["mechanical_solver_settings"]["desired_iterations"])
-            self.strategy_params.AddValue("max_radius_factor",self.settings["mechanical_solver_settings"]["max_radius_factor"])
-            self.strategy_params.AddValue("min_radius_factor",self.settings["mechanical_solver_settings"]["min_radius_factor"])
-            self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
-            self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
-            if nonlocal_damage:
-                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
-                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
-                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
-                solver = KratosPoro.PoromechanicsRammArcLengthNonlocalStrategy(self.mechanical_computing_model_part,
-                                                                               scheme,
-                                                                               self.mechanical_linear_solver,
-                                                                               convergence_criterion,
-                                                                               builder_and_solver,
-                                                                               self.strategy_params,
-                                                                               max_iters,
-                                                                               compute_reactions,
-                                                                               reform_step_dofs,
-                                                                               move_mesh_flag)
-            else:
-                solver = KratosPoro.PoromechanicsRammArcLengthStrategy(self.mechanical_computing_model_part,
-                                                                       scheme,
-                                                                       self.mechanical_linear_solver,
-                                                                       convergence_criterion,
-                                                                       builder_and_solver,
-                                                                       self.strategy_params,
-                                                                       max_iters,
-                                                                       compute_reactions,
-                                                                       reform_step_dofs,
-                                                                       move_mesh_flag)
-
-        return solver
-
-    def _CheckConvergence(self):
-
-        IsConverged = self.Selfweight_Solver.IsConverged()
-
-        return IsConverged
-
-    def _UpdateLoads(self):
-
-        self.Selfweight_Solver.UpdateLoads()
+#import kratos core and applications
+import KratosMultiphysics
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+import KratosMultiphysics.DamApplication as KratosDam
+import json
+
+def CreateSolver(main_model_part, custom_settings):
+
+    return DamSelfweightSolver(main_model_part, custom_settings)
+
+
+class DamSelfweightSolver(object):
+
+    ##constructor. the constructor shall only take care of storing the settings
+    ##and the pointer to the main_model part. This is needed since at the point of constructing the
+    ##model part is still not filled and the variables are not yet allocated
+    ##
+    ##real construction shall be delayed to the function "Initialize" which
+    ##will be called once the model is already filled
+    def __init__(self, main_model_part, custom_settings):
+
+        #TODO: shall obtain the computing_model_part from the MODEL once the object is implemented
+        self.main_model_part = main_model_part
+
+        ##settings string in json format
+        default_settings = KratosMultiphysics.Parameters("""
+        {
+            "solver_type": "dam_selfweight_solver",
+            "model_import_settings":{
+                "input_type": "mdpa",
+                "input_filename": "unknown_name",
+                "input_file_label": 0
+            },
+            "echo_level": 0,
+            "buffer_size": 2,
+            "processes_sub_model_part_list": [""],
+            "mechanical_solver_settings":{
+                "echo_level": 0,
+                "reform_dofs_at_each_step": false,
+                "clear_storage": false,
+                "compute_reactions": false,
+                "move_mesh_flag": true,
+                "solution_type": "Quasi-Static",
+                "scheme_type": "Newmark",
+                "rayleigh_m": 0.0,
+                "rayleigh_k": 0.0,
+                "strategy_type": "Newton-Raphson",
+                "convergence_criterion": "Displacement_criterion",
+                "displacement_relative_tolerance": 1.0e-4,
+                "displacement_absolute_tolerance": 1.0e-9,
+                "residual_relative_tolerance": 1.0e-4,
+                "residual_absolute_tolerance": 1.0e-9,
+                "max_iteration": 15,
+                "desired_iterations": 4,
+                "max_radius_factor": 20.0,
+                "min_radius_factor": 0.5,
+                "block_builder": true,
+                "nonlocal_damage": false,
+                "characteristic_length": 0.05,
+                "search_neighbours_step": false,
+                "linear_solver_settings":{
+                    "solver_type": "amgcl",
+                    "tolerance": 1.0e-6,
+                    "max_iteration": 100,
+                    "scaling": false,
+                    "verbosity": 0,
+                    "preconditioner_type": "ilu0",
+                    "smoother_type": "ilu0",
+                    "krylov_type": "gmres",
+                    "coarsening_type": "aggregation"
+                },
+                "problem_domain_sub_model_part_list": [""],
+                "body_domain_sub_model_part_list": [],
+                "mechanical_loads_sub_model_part_list": [],
+                "loads_sub_model_part_list": [],
+                "loads_variable_list": []
+            }
+        }
+        """)
+
+        # Overwrite the default settings with user-provided parameters
+        self.settings = custom_settings
+        self.settings.ValidateAndAssignDefaults(default_settings)
+
+        # Construct the linear solver
+        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
+        self.mechanical_linear_solver = linear_solver_factory.ConstructSolver(self.settings["mechanical_solver_settings"]["linear_solver_settings"])
+
+        print("Construction of DamSelfweightSolver finished")
+
+    def AddVariables(self):
+
+        ## Mechanical Variables
+        # Add displacements
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
+        # Add reactions for the displacements
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
+        # Add dynamic variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
+        # Add variables for the solid conditions
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_FACE_PRESSURE)
+        # Add volume acceleration
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VOLUME_ACCELERATION)
+        # Add variables for post-processing
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_AREA)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.INITIAL_NODAL_CAUCHY_STRESS_TENSOR)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Vi_POSITIVE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Viii_POSITIVE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_WIDTH)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_AREA)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.NODAL_YOUNG_MODULUS)
+
+        ## Thermal variables
+        thermal_settings = KratosMultiphysics.ConvectionDiffusionSettings()
+        thermal_settings.SetDiffusionVariable(KratosMultiphysics.CONDUCTIVITY)
+        thermal_settings.SetUnknownVariable(KratosMultiphysics.TEMPERATURE)
+        thermal_settings.SetSpecificHeatVariable(KratosMultiphysics.SPECIFIC_HEAT)
+        thermal_settings.SetDensityVariable(KratosMultiphysics.DENSITY)
+        thermal_settings.SetVolumeSourceVariable(KratosMultiphysics.HEAT_FLUX)
+        thermal_settings.SetSurfaceSourceVariable(KratosMultiphysics.FACE_HEAT_FLUX)
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.CONVECTION_DIFFUSION_SETTINGS, thermal_settings)
+
+        # Add thermal variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.CONDUCTIVITY)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.TEMPERATURE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.SPECIFIC_HEAT)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DENSITY)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.HEAT_FLUX)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FACE_HEAT_FLUX)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.NODAL_REFERENCE_TEMPERATURE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.PLACEMENT_TEMPERATURE)
+
+        # This Variable is used for computing heat source according Azenha Formulation
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.ALPHA_HEAT_SOURCE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.TIME_ACTIVATION)
+
+        print("Variables correctly added")
+
+    @classmethod
+    def GetMinimumBufferSize(self):
+        return 2
+
+    def AddDofs(self):
+
+        for node in self.main_model_part.Nodes:
+            ## Solid dofs
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_X,KratosMultiphysics.REACTION_X)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y,KratosMultiphysics.REACTION_Y)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z,KratosMultiphysics.REACTION_Z)
+
+        if(self.settings["mechanical_solver_settings"]["solution_type"].GetString() == "Dynamic"):
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
+        print("DOFs correctly added")
+
+    def ImportModelPart(self):
+
+        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
+
+            # Read ModelPart
+            KratosMultiphysics.ModelPartIO(self.settings["model_import_settings"]["input_filename"].GetString()).ReadModelPart(self.main_model_part)
+
+            # Create computing_model_part, set constitutive law and buffer size
+            self._ExecuteAfterReading()
+
+        else:
+            raise Exception("Other input options are not yet implemented.")
+
+        print ("Model reading finished")
+
+    def Initialize(self):
+
+
+        # Get the computing model parts
+        self.mechanical_computing_model_part = self.GetComputingModelPart()
+
+        # Builder and solver creation
+        mechanical_builder_and_solver = self._ConstructBuilderAndSolver(self.settings["mechanical_solver_settings"]["block_builder"].GetBool(),self.mechanical_linear_solver)
+
+        # Solution scheme creation
+        mechanical_scheme = self._ConstructScheme(self.settings["mechanical_solver_settings"]["scheme_type"].GetString(),
+                                         self.settings["mechanical_solver_settings"]["solution_type"].GetString())
+
+        # Get the convergence criterion
+        convergence_criterion = self._ConstructConvergenceCriterion(self.settings["mechanical_solver_settings"]["convergence_criterion"].GetString())
+
+        # Solver creation
+        self.Selfweight_Solver = self._ConstructSolver(mechanical_builder_and_solver,
+                                            mechanical_scheme,
+                                            convergence_criterion,
+                                            self.settings["mechanical_solver_settings"]["strategy_type"].GetString())
+
+        # Set echo_level
+        self.Selfweight_Solver.SetEchoLevel(self.settings["mechanical_solver_settings"]["echo_level"].GetInt())
+
+        # Check if everything is assigned correctly
+        self.Selfweight_Solver.Check()
+
+        print ("Initialization of DamSelfweightSolver finished")
+
+    def GetComputingModelPart(self):
+        return self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
+
+    def GetOutputVariables(self):
+        pass
+
+    def ComputeDeltaTime(self):
+        pass
+
+    def SaveRestart(self):
+        pass #one should write the restart file here
+
+    def Solve(self):
+        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
+            self.Selfweight_Solver.Clear()
+
+        self.Selfweight_Solver.Solve()
+
+    # solve :: sequencial calls
+
+    def InitializeStrategy(self):
+        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
+            self.Selfweight_Solver.Clear()
+
+        self.Selfweight_Solver.Initialize()
+
+    def InitializeSolutionStep(self):
+        self.Selfweight_Solver.InitializeSolutionStep()
+
+    def Predict(self):
+        self.Selfweight_Solver.Predict()
+
+    def SolveSolutionStep(self):
+        self.Selfweight_Solver.SolveSolutionStep()
+
+    def FinalizeSolutionStep(self):
+        self.Selfweight_Solver.FinalizeSolutionStep()
+
+    # solve :: sequencial calls
+
+    def SetEchoLevel(self, level):
+
+        self.Selfweight_Solver.SetEchoLevel(level)
+
+    def Clear(self):
+
+        self.Selfweight_Solver.Clear()
+
+    def Check(self):
+
+        self.Selfweight_Solver.Check()
+
+    #### Specific internal functions ####
+
+    def _ExecuteAfterReading(self):
+
+        self.mechanical_model_part_name = "mechanical_computing_domain"
+
+        self.body_domain_sub_sub_model_part_list = []
+        for i in range(self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"].size()):
+            self.body_domain_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"][i].GetString())
+        self.body_domain_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.body_domain_sub_sub_model_part_list))
+
+        self.loads_sub_sub_model_part_list = []
+        for i in range(self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"].size()):
+            self.loads_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"][i].GetString())
+        self.loads_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.loads_sub_sub_model_part_list))
+
+        # Auxiliary Kratos parameters object to be called by the CheckAndPepareModelProcess
+        aux_params = KratosMultiphysics.Parameters("{}")
+        aux_params.AddEmptyValue("mechanical_model_part_name").SetString(self.mechanical_model_part_name)
+        aux_params.AddValue("mechanical_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["problem_domain_sub_model_part_list"])
+        aux_params.AddValue("mechanical_loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["mechanical_loads_sub_model_part_list"])
+        aux_params.AddValue("body_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"])
+        aux_params.AddValue("body_domain_sub_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
+        aux_params.AddValue("loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"])
+        aux_params.AddValue("loads_sub_sub_model_part_list",self.loads_sub_sub_model_part_list)
+
+        # CheckAndPrepareModelProcess creates the solid_computational_model_part
+        from KratosMultiphysics.DamApplication import check_and_prepare_selfweight_model_process_dam
+        check_and_prepare_selfweight_model_process_dam.CheckAndPrepareSelfweightModelProcess(self.main_model_part, aux_params).Execute()
+
+        # Constitutive law import
+        from KratosMultiphysics.DamApplication import dam_constitutive_law_utility
+        dam_constitutive_law_utility.SetConstitutiveLaw(self.main_model_part)
+
+        self.main_model_part.SetBufferSize( self.settings["buffer_size"].GetInt() )
+        minimum_buffer_size = self.GetMinimumBufferSize()
+        if(minimum_buffer_size > self.main_model_part.GetBufferSize()):
+            self.main_model_part.SetBufferSize( minimum_buffer_size )
+
+    @classmethod
+    def _ConstructBuilderAndSolver(self, block_builder, linear_solver):
+
+        # Creating the builder and solver
+        if(block_builder):
+            builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(linear_solver)
+        else:
+            builder_and_solver = KratosMultiphysics.ResidualBasedEliminationBuilderAndSolver(linear_solver)
+
+        return builder_and_solver
+
+    def _ConstructScheme(self, scheme_type, solution_type):
+
+        rayleigh_m = self.settings["mechanical_solver_settings"]["rayleigh_m"].GetDouble()
+        rayleigh_k = self.settings["mechanical_solver_settings"]["rayleigh_k"].GetDouble()
+
+        if(solution_type == "Quasi-Static"):
+            if(rayleigh_m<1.0e-15 and rayleigh_k<1.0e-15):
+                scheme =  KratosDam.IncrementalUpdateStaticSmoothingScheme()
+            else:
+                scheme =  KratosDam.IncrementalUpdateStaticDampedSmoothingScheme(rayleigh_m,rayleigh_k)
+        else:
+            if(scheme_type == "Newmark"):
+                damp_factor_m = 0.0
+            else:
+                damp_factor_m = -0.01
+            scheme = KratosDam.BossakDisplacementSmoothingScheme(damp_factor_m,rayleigh_m,rayleigh_k)
+
+        return scheme
+
+    def _ConstructConvergenceCriterion(self, convergence_criterion):
+
+        D_RT = self.settings["mechanical_solver_settings"]["displacement_relative_tolerance"].GetDouble()
+        D_AT = self.settings["mechanical_solver_settings"]["displacement_absolute_tolerance"].GetDouble()
+        R_RT = self.settings["mechanical_solver_settings"]["residual_relative_tolerance"].GetDouble()
+        R_AT = self.settings["mechanical_solver_settings"]["residual_absolute_tolerance"].GetDouble()
+        echo_level = self.settings["mechanical_solver_settings"]["echo_level"].GetInt()
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
+    def _ConstructSolver(self, builder_and_solver, scheme, convergence_criterion, strategy_type):
+
+        nonlocal_damage = self.settings["mechanical_solver_settings"]["nonlocal_damage"].GetBool()
+        max_iters = self.settings["mechanical_solver_settings"]["max_iteration"].GetInt()
+        compute_reactions = self.settings["mechanical_solver_settings"]["compute_reactions"].GetBool()
+        reform_step_dofs = self.settings["mechanical_solver_settings"]["reform_dofs_at_each_step"].GetBool()
+        move_mesh_flag = self.settings["mechanical_solver_settings"]["move_mesh_flag"].GetBool()
+
+        if strategy_type == "Newton-Raphson":
+            if nonlocal_damage:
+                self.strategy_params = KratosMultiphysics.Parameters("{}")
+                self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
+                self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
+                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
+                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
+                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
+                solver = KratosPoro.PoromechanicsNewtonRaphsonNonlocalStrategy(self.mechanical_computing_model_part,
+                                                                               scheme,
+                                                                               convergence_criterion,
+                                                                               builder_and_solver,
+                                                                               self.strategy_params,
+                                                                               max_iters,
+                                                                               compute_reactions,
+                                                                               reform_step_dofs,
+                                                                               move_mesh_flag)
+            else:
+                self.main_model_part.ProcessInfo.SetValue(KratosPoro.IS_CONVERGED, True)
+                solver = KratosMultiphysics.ResidualBasedNewtonRaphsonStrategy(self.mechanical_computing_model_part,
+                                                                                    scheme,
+                                                                                    convergence_criterion,
+                                                                                    builder_and_solver,
+                                                                                    max_iters,
+                                                                                    compute_reactions,
+                                                                                    reform_step_dofs,
+                                                                                    move_mesh_flag)
+        else:
+            # Arc-Length strategy
+            self.strategy_params = KratosMultiphysics.Parameters("{}")
+            self.strategy_params.AddValue("desired_iterations",self.settings["mechanical_solver_settings"]["desired_iterations"])
+            self.strategy_params.AddValue("max_radius_factor",self.settings["mechanical_solver_settings"]["max_radius_factor"])
+            self.strategy_params.AddValue("min_radius_factor",self.settings["mechanical_solver_settings"]["min_radius_factor"])
+            self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
+            self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
+            if nonlocal_damage:
+                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
+                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
+                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
+                solver = KratosPoro.PoromechanicsRammArcLengthNonlocalStrategy(self.mechanical_computing_model_part,
+                                                                               scheme,
+                                                                               self.mechanical_linear_solver,
+                                                                               convergence_criterion,
+                                                                               builder_and_solver,
+                                                                               self.strategy_params,
+                                                                               max_iters,
+                                                                               compute_reactions,
+                                                                               reform_step_dofs,
+                                                                               move_mesh_flag)
+            else:
+                solver = KratosPoro.PoromechanicsRammArcLengthStrategy(self.mechanical_computing_model_part,
+                                                                       scheme,
+                                                                       self.mechanical_linear_solver,
+                                                                       convergence_criterion,
+                                                                       builder_and_solver,
+                                                                       self.strategy_params,
+                                                                       max_iters,
+                                                                       compute_reactions,
+                                                                       reform_step_dofs,
+                                                                       move_mesh_flag)
+
+        return solver
+
+    def _CheckConvergence(self):
+
+        IsConverged = self.Selfweight_Solver.IsConverged()
+
+        return IsConverged
+
+    def _UpdateLoads(self):
+
+        self.Selfweight_Solver.UpdateLoads()
```

## KratosMultiphysics/DamApplication/dam_thermo_mechanic_solver.py

 * *Ordering differences only*

```diff
@@ -1,512 +1,512 @@
-#import kratos core and applications
-import KratosMultiphysics
-import KratosMultiphysics.ConvectionDiffusionApplication as KratosConvDiff
-import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-import KratosMultiphysics.DamApplication as KratosDam
-import json
-
-def CreateSolver(main_model_part, custom_settings):
-
-    return DamThermoMechanicSolver(main_model_part, custom_settings)
-
-
-class DamThermoMechanicSolver(object):
-
-    ##constructor. the constructor shall only take care of storing the settings
-    ##and the pointer to the main_model part. This is needed since at the point of constructing the
-    ##model part is still not filled and the variables are not yet allocated
-    ##
-    ##real construction shall be delayed to the function "Initialize" which
-    ##will be called once the model is already filled
-    def __init__(self, main_model_part, custom_settings):
-
-        #TODO: shall obtain the computing_model_part from the MODEL once the object is implemented
-        self.main_model_part = main_model_part
-
-        ##settings string in json format
-        default_settings = KratosMultiphysics.Parameters("""
-        {
-            "solver_type": "dam_thermo_mechanic_solver",
-            "model_import_settings":{
-                "input_type": "mdpa",
-                "input_filename": "unknown_name",
-                "input_file_label": 0
-            },
-            "echo_level": 0,
-            "buffer_size": 2,
-            "processes_sub_model_part_list": [""],
-            "thermal_solver_settings":{
-                "echo_level": 0,
-                "reform_dofs_at_each_step": false,
-                "clear_storage": false,
-                "compute_reactions": false,
-                "move_mesh_flag": true,
-                "compute_norm_dx_flag": false,
-                "theta_scheme": 1.0,
-                "block_builder": true,
-                "linear_solver_settings":{
-                    "solver_type": "amgcl",
-                    "tolerance": 1.0e-6,
-                    "max_iteration": 100,
-                    "scaling": false,
-                    "verbosity": 0,
-                    "preconditioner_type": "ilu0",
-                    "smoother_type": "ilu0",
-                    "krylov_type": "gmres",
-                    "coarsening_type": "aggregation"
-                },
-                "problem_domain_sub_model_part_list": [""],
-                "thermal_loads_sub_model_part_list": []
-            },
-            "mechanical_solver_settings":{
-                "echo_level": 0,
-                "reform_dofs_at_each_step": false,
-                "clear_storage": false,
-                "compute_reactions": false,
-                "move_mesh_flag": true,
-                "solution_type": "Quasi-Static",
-                "scheme_type": "Newmark",
-                "rayleigh_m": 0.0,
-                "rayleigh_k": 0.0,
-                "strategy_type": "Newton-Raphson",
-                "convergence_criterion": "Displacement_criterion",
-                "displacement_relative_tolerance": 1.0e-4,
-                "displacement_absolute_tolerance": 1.0e-9,
-                "residual_relative_tolerance": 1.0e-4,
-                "residual_absolute_tolerance": 1.0e-9,
-                "max_iteration": 15,
-                "desired_iterations": 4,
-                "max_radius_factor": 20.0,
-                "min_radius_factor": 0.5,
-                "block_builder": true,
-                "nonlocal_damage": false,
-                "characteristic_length": 0.05,
-                "search_neighbours_step": false,
-                "linear_solver_settings":{
-                    "solver_type": "amgcl",
-                    "tolerance": 1.0e-6,
-                    "max_iteration": 100,
-                    "scaling": false,
-                    "verbosity": 0,
-                    "preconditioner_type": "ilu0",
-                    "smoother_type": "ilu0",
-                    "krylov_type": "gmres",
-                    "coarsening_type": "aggregation"
-                },
-                "problem_domain_sub_model_part_list": [""],
-                "body_domain_sub_model_part_list": [],
-                "mechanical_loads_sub_model_part_list": [],
-                "loads_sub_model_part_list": [],
-                "loads_variable_list": []
-            }
-        }
-        """)
-
-        # Overwrite the default settings with user-provided parameters
-        self.settings = custom_settings
-        self.settings.ValidateAndAssignDefaults(default_settings)
-
-        # Construct the linear solver
-        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
-        self.thermal_linear_solver = linear_solver_factory.ConstructSolver(self.settings["thermal_solver_settings"]["linear_solver_settings"])
-        self.mechanical_linear_solver = linear_solver_factory.ConstructSolver(self.settings["mechanical_solver_settings"]["linear_solver_settings"])
-
-        print("Construction of DamThermoMechanicSolver finished")
-
-    def AddVariables(self):
-
-        ## Mechanical Variables
-        # Add displacements
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
-        # Add reactions for the displacements
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
-        # Add dynamic variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
-        # Add variables for the solid conditions
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_FACE_PRESSURE)
-        # Add volume acceleration
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VOLUME_ACCELERATION)
-        # Add variables for post-processing
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_AREA)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.INITIAL_NODAL_CAUCHY_STRESS_TENSOR)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Vi_POSITIVE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Viii_POSITIVE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_WIDTH)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_AREA)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.NODAL_YOUNG_MODULUS)
-
-        ## Thermal variables
-        thermal_settings = KratosMultiphysics.ConvectionDiffusionSettings()
-        thermal_settings.SetDiffusionVariable(KratosMultiphysics.CONDUCTIVITY)
-        thermal_settings.SetUnknownVariable(KratosMultiphysics.TEMPERATURE)
-        thermal_settings.SetSpecificHeatVariable(KratosMultiphysics.SPECIFIC_HEAT)
-        thermal_settings.SetDensityVariable(KratosMultiphysics.DENSITY)
-        thermal_settings.SetVolumeSourceVariable(KratosMultiphysics.HEAT_FLUX)
-        thermal_settings.SetSurfaceSourceVariable(KratosMultiphysics.FACE_HEAT_FLUX)
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.CONVECTION_DIFFUSION_SETTINGS, thermal_settings)
-
-        # Add thermal variables
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.CONDUCTIVITY)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.TEMPERATURE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.SPECIFIC_HEAT)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DENSITY)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.HEAT_FLUX)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FACE_HEAT_FLUX)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.NODAL_REFERENCE_TEMPERATURE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.PLACEMENT_TEMPERATURE)
-
-        # This Variable is used for computing heat source according Azenha Formulation
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.ALPHA_HEAT_SOURCE)
-        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.TIME_ACTIVATION)
-
-
-        print("Variables correctly added")
-
-    def GetMinimumBufferSize(self):
-        return 2
-
-    def AddDofs(self):
-
-        for node in self.main_model_part.Nodes:
-            ## Solid dofs
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_X,KratosMultiphysics.REACTION_X)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y,KratosMultiphysics.REACTION_Y)
-            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z,KratosMultiphysics.REACTION_Z)
-            ## Thermal dofs
-            node.AddDof(KratosMultiphysics.TEMPERATURE)
-
-        if(self.settings["mechanical_solver_settings"]["solution_type"].GetString() == "Dynamic"):
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
-        print("DOFs correctly added")
-
-    def ImportModelPart(self):
-
-        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
-
-            # Read ModelPart
-            KratosMultiphysics.ModelPartIO(self.settings["model_import_settings"]["input_filename"].GetString()).ReadModelPart(self.main_model_part)
-
-            # Create computing_model_part, set constitutive law and buffer size
-            self._ExecuteAfterReading()
-
-        else:
-            raise Exception("Other input options are not yet implemented.")
-
-        print ("Model reading finished")
-
-    def Initialize(self):
-
-        # Set ProcessInfo variables
-        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME_INTEGRATION_THETA, self.settings["thermal_solver_settings"]["theta_scheme"].GetDouble())
-
-        # Get the computing model parts
-        self.thermal_computing_model_part = self.GetComputingThermalModelPart()
-        self.mechanical_computing_model_part = self.GetComputingModelPart()
-
-        # Builder and solver creation
-        thermal_builder_and_solver = self._ConstructBuilderAndSolver(self.settings["thermal_solver_settings"]["block_builder"].GetBool(),self.thermal_linear_solver)
-        mechanical_builder_and_solver = self._ConstructBuilderAndSolver(self.settings["mechanical_solver_settings"]["block_builder"].GetBool(),self.mechanical_linear_solver)
-
-        # Solution scheme creation
-        thermal_scheme = KratosMultiphysics.ResidualBasedIncrementalUpdateStaticScheme()
-        mechanical_scheme = self._ConstructScheme(self.settings["mechanical_solver_settings"]["scheme_type"].GetString(),
-                                         self.settings["mechanical_solver_settings"]["solution_type"].GetString())
-
-        # Get the convergence criterion
-        convergence_criterion = self._ConstructConvergenceCriterion(self.settings["mechanical_solver_settings"]["convergence_criterion"].GetString())
-
-        # Solver creation
-        self.Thermal_Solver = KratosMultiphysics.ResidualBasedLinearStrategy(self.thermal_computing_model_part,
-                                                                             thermal_scheme,
-                                                                             thermal_builder_and_solver,
-                                                                             self.settings["thermal_solver_settings"]["compute_reactions"].GetBool(),
-                                                                             self.settings["thermal_solver_settings"]["reform_dofs_at_each_step"].GetBool(),
-                                                                             self.settings["thermal_solver_settings"]["compute_norm_dx_flag"].GetBool(),
-                                                                             self.settings["thermal_solver_settings"]["move_mesh_flag"].GetBool())
-        self.Mechanical_Solver = self._ConstructSolver(mechanical_builder_and_solver,
-                                                       mechanical_scheme,
-                                                       convergence_criterion,
-                                                       self.settings["mechanical_solver_settings"]["strategy_type"].GetString())
-
-        # Set echo_level
-        self.Thermal_Solver.SetEchoLevel(self.settings["thermal_solver_settings"]["echo_level"].GetInt())
-        self.Mechanical_Solver.SetEchoLevel(self.settings["mechanical_solver_settings"]["echo_level"].GetInt())
-
-        # Check if everything is assigned correctly
-        self.Thermal_Solver.Check()
-        self.Mechanical_Solver.Check()
-
-        print ("Initialization DamThermoMechanicSolver finished")
-
-    def GetComputingModelPart(self):
-        return self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
-
-    def GetComputingThermalModelPart(self):
-        return self.main_model_part.GetSubModelPart(self.thermal_model_part_name)
-
-    def GetOutputVariables(self):
-        pass
-
-    def ComputeDeltaTime(self):
-        pass
-
-    def SaveRestart(self):
-        pass #one should write the restart file here
-
-    def Solve(self):
-        if self.settings["thermal_solver_settings"]["clear_storage"].GetBool():
-            self.Thermal_Solver.Clear()
-        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
-            self.Mechanical_Solver.Clear()
-
-        self.Thermal_Solver.Solve()
-        self.Mechanical_Solver.Solve()
-
-    # solve :: sequencial calls
-
-    def InitializeStrategy(self):
-        if self.settings["thermal_solver_settings"]["clear_storage"].GetBool():
-            self.Thermal_Solver.Clear()
-        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
-            self.Mechanical_Solver.Clear()
-
-        self.Thermal_Solver.Initialize()
-        self.Mechanical_Solver.Initialize()
-
-    def InitializeSolutionStep(self):
-        self.Thermal_Solver.InitializeSolutionStep()
-        self.Mechanical_Solver.InitializeSolutionStep()
-
-    def Predict(self):
-        self.Thermal_Solver.Predict()
-        self.Mechanical_Solver.Predict()
-
-    def SolveSolutionStep(self):
-        self.Thermal_Solver.SolveSolutionStep()
-        self.Mechanical_Solver.SolveSolutionStep()
-
-    def FinalizeSolutionStep(self):
-        self.Thermal_Solver.FinalizeSolutionStep()
-        self.Mechanical_Solver.FinalizeSolutionStep()
-
-    # solve :: sequencial calls
-
-    def SetEchoLevel(self, level):
-        self.Thermal_Solver.SetEchoLevel(level)
-        self.Mechanical_Solver.SetEchoLevel(level)
-
-    def Clear(self):
-        self.Thermal_Solver.Clear()
-        self.Mechanical_Solver.Clear()
-
-    def Check(self):
-        self.Thermal_Solver.Check()
-        self.Mechanical_Solver.Check()
-
-    #### Specific internal functions ####
-
-    def _ExecuteAfterReading(self):
-
-        self.thermal_model_part_name = "thermal_computing_domain"
-        self.mechanical_model_part_name = "mechanical_computing_domain"
-
-        # Create list of sub sub model parts (it is a copy of the standard lists with a different name)
-        self.thermal_domain_sub_sub_model_part_list = []
-        for i in range(self.settings["thermal_solver_settings"]["problem_domain_sub_model_part_list"].size()):
-            self.thermal_domain_sub_sub_model_part_list.append("sub_"+self.settings["thermal_solver_settings"]["problem_domain_sub_model_part_list"][i].GetString())
-        self.thermal_domain_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.thermal_domain_sub_sub_model_part_list))
-
-        self.thermal_loads_sub_sub_model_part_list = []
-        for i in range(self.settings["thermal_solver_settings"]["thermal_loads_sub_model_part_list"].size()):
-            self.thermal_loads_sub_sub_model_part_list.append("sub_"+self.settings["thermal_solver_settings"]["thermal_loads_sub_model_part_list"][i].GetString())
-        self.thermal_loads_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.thermal_loads_sub_sub_model_part_list))
-
-        self.body_domain_sub_sub_model_part_list = []
-        for i in range(self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"].size()):
-            self.body_domain_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"][i].GetString())
-        self.body_domain_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.body_domain_sub_sub_model_part_list))
-
-        self.loads_sub_sub_model_part_list = []
-        for i in range(self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"].size()):
-            self.loads_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"][i].GetString())
-        self.loads_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.loads_sub_sub_model_part_list))
-
-        # Auxiliary Kratos parameters object to be called by the CheckAndPepareModelProcessDamThermal
-        aux_params = KratosMultiphysics.Parameters("{}")
-        aux_params.AddEmptyValue("thermal_model_part_name").SetString(self.thermal_model_part_name)
-        aux_params.AddValue("thermal_domain_sub_model_part_list",self.settings["thermal_solver_settings"]["problem_domain_sub_model_part_list"])
-        aux_params.AddValue("thermal_domain_sub_sub_model_part_list",self.thermal_domain_sub_sub_model_part_list)
-        aux_params.AddValue("thermal_loads_sub_model_part_list",self.settings["thermal_solver_settings"]["thermal_loads_sub_model_part_list"])
-        aux_params.AddValue("thermal_loads_sub_sub_model_part_list",self.thermal_loads_sub_sub_model_part_list)
-
-        aux_params.AddEmptyValue("mechanical_model_part_name").SetString(self.mechanical_model_part_name)
-        aux_params.AddValue("mechanical_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["problem_domain_sub_model_part_list"])
-        aux_params.AddValue("mechanical_loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["mechanical_loads_sub_model_part_list"])
-        aux_params.AddValue("body_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"])
-        aux_params.AddValue("body_domain_sub_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
-        aux_params.AddValue("loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"])
-        aux_params.AddValue("loads_sub_sub_model_part_list",self.loads_sub_sub_model_part_list)
-
-        # CheckAndPrepareModelProcessDamMechanical creates the solid_computational_model_part
-        from KratosMultiphysics.DamApplication import check_and_prepare_model_process_dam_thermal
-        check_and_prepare_model_process_dam_thermal.CheckAndPrepareModelProcessDamThermal(self.main_model_part, aux_params).Execute()
-
-        # Constitutive law import
-        from KratosMultiphysics.DamApplication import dam_constitutive_law_utility
-        dam_constitutive_law_utility.SetConstitutiveLaw(self.main_model_part)
-
-        self.main_model_part.SetBufferSize( self.settings["buffer_size"].GetInt() )
-        minimum_buffer_size = self.GetMinimumBufferSize()
-        if(minimum_buffer_size > self.main_model_part.GetBufferSize()):
-            self.main_model_part.SetBufferSize( minimum_buffer_size )
-
-    def _ConstructBuilderAndSolver(self, block_builder, linear_solver):
-
-        # Creating the builder and solver
-        if(block_builder):
-            builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(linear_solver)
-        else:
-            builder_and_solver = KratosMultiphysics.ResidualBasedEliminationBuilderAndSolver(linear_solver)
-
-        return builder_and_solver
-
-    def _ConstructScheme(self, scheme_type, solution_type):
-
-        rayleigh_m = self.settings["mechanical_solver_settings"]["rayleigh_m"].GetDouble()
-        rayleigh_k = self.settings["mechanical_solver_settings"]["rayleigh_k"].GetDouble()
-
-        if(solution_type == "Quasi-Static"):
-            if(rayleigh_m<1.0e-15 and rayleigh_k<1.0e-15):
-                scheme =  KratosDam.IncrementalUpdateStaticSmoothingScheme()
-            else:
-                scheme =  KratosDam.IncrementalUpdateStaticDampedSmoothingScheme(rayleigh_m,rayleigh_k)
-        else:
-            if(scheme_type == "Newmark"):
-                damp_factor_m = 0.0
-            else:
-                damp_factor_m = -0.01
-            scheme = KratosDam.BossakDisplacementSmoothingScheme(damp_factor_m,rayleigh_m,rayleigh_k)
-
-        return scheme
-
-    def _ConstructConvergenceCriterion(self, convergence_criterion):
-
-        D_RT = self.settings["mechanical_solver_settings"]["displacement_relative_tolerance"].GetDouble()
-        D_AT = self.settings["mechanical_solver_settings"]["displacement_absolute_tolerance"].GetDouble()
-        R_RT = self.settings["mechanical_solver_settings"]["residual_relative_tolerance"].GetDouble()
-        R_AT = self.settings["mechanical_solver_settings"]["residual_absolute_tolerance"].GetDouble()
-        echo_level = self.settings["mechanical_solver_settings"]["echo_level"].GetInt()
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
-    def _ConstructSolver(self, builder_and_solver, scheme, convergence_criterion, strategy_type):
-
-        nonlocal_damage = self.settings["mechanical_solver_settings"]["nonlocal_damage"].GetBool()
-        max_iters = self.settings["mechanical_solver_settings"]["max_iteration"].GetInt()
-        compute_reactions = self.settings["mechanical_solver_settings"]["compute_reactions"].GetBool()
-        reform_step_dofs = self.settings["mechanical_solver_settings"]["reform_dofs_at_each_step"].GetBool()
-        move_mesh_flag = self.settings["mechanical_solver_settings"]["move_mesh_flag"].GetBool()
-
-        if strategy_type == "Newton-Raphson":
-            if nonlocal_damage:
-                self.strategy_params = KratosMultiphysics.Parameters("{}")
-                self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
-                self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
-                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
-                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
-                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
-                solver = KratosPoro.PoromechanicsNewtonRaphsonNonlocalStrategy(self.mechanical_computing_model_part,
-                                                                               scheme,
-                                                                               convergence_criterion,
-                                                                               builder_and_solver,
-                                                                               self.strategy_params,
-                                                                               max_iters,
-                                                                               compute_reactions,
-                                                                               reform_step_dofs,
-                                                                               move_mesh_flag)
-            else:
-                self.main_model_part.ProcessInfo.SetValue(KratosPoro.IS_CONVERGED, True)
-                solver = KratosMultiphysics.ResidualBasedNewtonRaphsonStrategy(self.mechanical_computing_model_part,
-                                                                                    scheme,
-                                                                                    convergence_criterion,
-                                                                                    builder_and_solver,
-                                                                                    max_iters,
-                                                                                    compute_reactions,
-                                                                                    reform_step_dofs,
-                                                                                    move_mesh_flag)
-        else:
-            # Arc-Length strategy
-            self.strategy_params = KratosMultiphysics.Parameters("{}")
-            self.strategy_params.AddValue("desired_iterations",self.settings["mechanical_solver_settings"]["desired_iterations"])
-            self.strategy_params.AddValue("max_radius_factor",self.settings["mechanical_solver_settings"]["max_radius_factor"])
-            self.strategy_params.AddValue("min_radius_factor",self.settings["mechanical_solver_settings"]["min_radius_factor"])
-            self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
-            self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
-            if nonlocal_damage:
-                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
-                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
-                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
-                solver = KratosPoro.PoromechanicsRammArcLengthNonlocalStrategy(self.mechanical_computing_model_part,
-                                                                               scheme,
-                                                                               self.mechanical_linear_solver,
-                                                                               convergence_criterion,
-                                                                               builder_and_solver,
-                                                                               self.strategy_params,
-                                                                               max_iters,
-                                                                               compute_reactions,
-                                                                               reform_step_dofs,
-                                                                               move_mesh_flag)
-            else:
-                solver = KratosPoro.PoromechanicsRammArcLengthStrategy(self.mechanical_computing_model_part,
-                                                                       scheme,
-                                                                       self.mechanical_linear_solver,
-                                                                       convergence_criterion,
-                                                                       builder_and_solver,
-                                                                       self.strategy_params,
-                                                                       max_iters,
-                                                                       compute_reactions,
-                                                                       reform_step_dofs,
-                                                                       move_mesh_flag)
-
-        return solver
-
-    def _CheckConvergence(self):
-
-        IsConverged = self.Mechanical_Solver.IsConverged()
-
-        return IsConverged
-
-    def _UpdateLoads(self):
-
-        self.Mechanical_Solver.UpdateLoads()
+#import kratos core and applications
+import KratosMultiphysics
+import KratosMultiphysics.ConvectionDiffusionApplication as KratosConvDiff
+import KratosMultiphysics.StructuralMechanicsApplication as KratosStructural
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+import KratosMultiphysics.DamApplication as KratosDam
+import json
+
+def CreateSolver(main_model_part, custom_settings):
+
+    return DamThermoMechanicSolver(main_model_part, custom_settings)
+
+
+class DamThermoMechanicSolver(object):
+
+    ##constructor. the constructor shall only take care of storing the settings
+    ##and the pointer to the main_model part. This is needed since at the point of constructing the
+    ##model part is still not filled and the variables are not yet allocated
+    ##
+    ##real construction shall be delayed to the function "Initialize" which
+    ##will be called once the model is already filled
+    def __init__(self, main_model_part, custom_settings):
+
+        #TODO: shall obtain the computing_model_part from the MODEL once the object is implemented
+        self.main_model_part = main_model_part
+
+        ##settings string in json format
+        default_settings = KratosMultiphysics.Parameters("""
+        {
+            "solver_type": "dam_thermo_mechanic_solver",
+            "model_import_settings":{
+                "input_type": "mdpa",
+                "input_filename": "unknown_name",
+                "input_file_label": 0
+            },
+            "echo_level": 0,
+            "buffer_size": 2,
+            "processes_sub_model_part_list": [""],
+            "thermal_solver_settings":{
+                "echo_level": 0,
+                "reform_dofs_at_each_step": false,
+                "clear_storage": false,
+                "compute_reactions": false,
+                "move_mesh_flag": true,
+                "compute_norm_dx_flag": false,
+                "theta_scheme": 1.0,
+                "block_builder": true,
+                "linear_solver_settings":{
+                    "solver_type": "amgcl",
+                    "tolerance": 1.0e-6,
+                    "max_iteration": 100,
+                    "scaling": false,
+                    "verbosity": 0,
+                    "preconditioner_type": "ilu0",
+                    "smoother_type": "ilu0",
+                    "krylov_type": "gmres",
+                    "coarsening_type": "aggregation"
+                },
+                "problem_domain_sub_model_part_list": [""],
+                "thermal_loads_sub_model_part_list": []
+            },
+            "mechanical_solver_settings":{
+                "echo_level": 0,
+                "reform_dofs_at_each_step": false,
+                "clear_storage": false,
+                "compute_reactions": false,
+                "move_mesh_flag": true,
+                "solution_type": "Quasi-Static",
+                "scheme_type": "Newmark",
+                "rayleigh_m": 0.0,
+                "rayleigh_k": 0.0,
+                "strategy_type": "Newton-Raphson",
+                "convergence_criterion": "Displacement_criterion",
+                "displacement_relative_tolerance": 1.0e-4,
+                "displacement_absolute_tolerance": 1.0e-9,
+                "residual_relative_tolerance": 1.0e-4,
+                "residual_absolute_tolerance": 1.0e-9,
+                "max_iteration": 15,
+                "desired_iterations": 4,
+                "max_radius_factor": 20.0,
+                "min_radius_factor": 0.5,
+                "block_builder": true,
+                "nonlocal_damage": false,
+                "characteristic_length": 0.05,
+                "search_neighbours_step": false,
+                "linear_solver_settings":{
+                    "solver_type": "amgcl",
+                    "tolerance": 1.0e-6,
+                    "max_iteration": 100,
+                    "scaling": false,
+                    "verbosity": 0,
+                    "preconditioner_type": "ilu0",
+                    "smoother_type": "ilu0",
+                    "krylov_type": "gmres",
+                    "coarsening_type": "aggregation"
+                },
+                "problem_domain_sub_model_part_list": [""],
+                "body_domain_sub_model_part_list": [],
+                "mechanical_loads_sub_model_part_list": [],
+                "loads_sub_model_part_list": [],
+                "loads_variable_list": []
+            }
+        }
+        """)
+
+        # Overwrite the default settings with user-provided parameters
+        self.settings = custom_settings
+        self.settings.ValidateAndAssignDefaults(default_settings)
+
+        # Construct the linear solver
+        import KratosMultiphysics.python_linear_solver_factory as linear_solver_factory
+        self.thermal_linear_solver = linear_solver_factory.ConstructSolver(self.settings["thermal_solver_settings"]["linear_solver_settings"])
+        self.mechanical_linear_solver = linear_solver_factory.ConstructSolver(self.settings["mechanical_solver_settings"]["linear_solver_settings"])
+
+        print("Construction of DamThermoMechanicSolver finished")
+
+    def AddVariables(self):
+
+        ## Mechanical Variables
+        # Add displacements
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
+        # Add reactions for the displacements
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
+        # Add dynamic variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
+        # Add variables for the solid conditions
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_FACE_PRESSURE)
+        # Add volume acceleration
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VOLUME_ACCELERATION)
+        # Add variables for post-processing
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_AREA)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.INITIAL_NODAL_CAUCHY_STRESS_TENSOR)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Vi_POSITIVE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.Viii_POSITIVE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_WIDTH)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosPoro.NODAL_JOINT_AREA)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.NODAL_YOUNG_MODULUS)
+
+        ## Thermal variables
+        thermal_settings = KratosMultiphysics.ConvectionDiffusionSettings()
+        thermal_settings.SetDiffusionVariable(KratosMultiphysics.CONDUCTIVITY)
+        thermal_settings.SetUnknownVariable(KratosMultiphysics.TEMPERATURE)
+        thermal_settings.SetSpecificHeatVariable(KratosMultiphysics.SPECIFIC_HEAT)
+        thermal_settings.SetDensityVariable(KratosMultiphysics.DENSITY)
+        thermal_settings.SetVolumeSourceVariable(KratosMultiphysics.HEAT_FLUX)
+        thermal_settings.SetSurfaceSourceVariable(KratosMultiphysics.FACE_HEAT_FLUX)
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.CONVECTION_DIFFUSION_SETTINGS, thermal_settings)
+
+        # Add thermal variables
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.CONDUCTIVITY)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.TEMPERATURE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.SPECIFIC_HEAT)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DENSITY)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.HEAT_FLUX)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FACE_HEAT_FLUX)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.NODAL_REFERENCE_TEMPERATURE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.PLACEMENT_TEMPERATURE)
+
+        # This Variable is used for computing heat source according Azenha Formulation
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.ALPHA_HEAT_SOURCE)
+        self.main_model_part.AddNodalSolutionStepVariable(KratosDam.TIME_ACTIVATION)
+
+
+        print("Variables correctly added")
+
+    def GetMinimumBufferSize(self):
+        return 2
+
+    def AddDofs(self):
+
+        for node in self.main_model_part.Nodes:
+            ## Solid dofs
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_X,KratosMultiphysics.REACTION_X)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Y,KratosMultiphysics.REACTION_Y)
+            node.AddDof(KratosMultiphysics.DISPLACEMENT_Z,KratosMultiphysics.REACTION_Z)
+            ## Thermal dofs
+            node.AddDof(KratosMultiphysics.TEMPERATURE)
+
+        if(self.settings["mechanical_solver_settings"]["solution_type"].GetString() == "Dynamic"):
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
+        print("DOFs correctly added")
+
+    def ImportModelPart(self):
+
+        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
+
+            # Read ModelPart
+            KratosMultiphysics.ModelPartIO(self.settings["model_import_settings"]["input_filename"].GetString()).ReadModelPart(self.main_model_part)
+
+            # Create computing_model_part, set constitutive law and buffer size
+            self._ExecuteAfterReading()
+
+        else:
+            raise Exception("Other input options are not yet implemented.")
+
+        print ("Model reading finished")
+
+    def Initialize(self):
+
+        # Set ProcessInfo variables
+        self.main_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME_INTEGRATION_THETA, self.settings["thermal_solver_settings"]["theta_scheme"].GetDouble())
+
+        # Get the computing model parts
+        self.thermal_computing_model_part = self.GetComputingThermalModelPart()
+        self.mechanical_computing_model_part = self.GetComputingModelPart()
+
+        # Builder and solver creation
+        thermal_builder_and_solver = self._ConstructBuilderAndSolver(self.settings["thermal_solver_settings"]["block_builder"].GetBool(),self.thermal_linear_solver)
+        mechanical_builder_and_solver = self._ConstructBuilderAndSolver(self.settings["mechanical_solver_settings"]["block_builder"].GetBool(),self.mechanical_linear_solver)
+
+        # Solution scheme creation
+        thermal_scheme = KratosMultiphysics.ResidualBasedIncrementalUpdateStaticScheme()
+        mechanical_scheme = self._ConstructScheme(self.settings["mechanical_solver_settings"]["scheme_type"].GetString(),
+                                         self.settings["mechanical_solver_settings"]["solution_type"].GetString())
+
+        # Get the convergence criterion
+        convergence_criterion = self._ConstructConvergenceCriterion(self.settings["mechanical_solver_settings"]["convergence_criterion"].GetString())
+
+        # Solver creation
+        self.Thermal_Solver = KratosMultiphysics.ResidualBasedLinearStrategy(self.thermal_computing_model_part,
+                                                                             thermal_scheme,
+                                                                             thermal_builder_and_solver,
+                                                                             self.settings["thermal_solver_settings"]["compute_reactions"].GetBool(),
+                                                                             self.settings["thermal_solver_settings"]["reform_dofs_at_each_step"].GetBool(),
+                                                                             self.settings["thermal_solver_settings"]["compute_norm_dx_flag"].GetBool(),
+                                                                             self.settings["thermal_solver_settings"]["move_mesh_flag"].GetBool())
+        self.Mechanical_Solver = self._ConstructSolver(mechanical_builder_and_solver,
+                                                       mechanical_scheme,
+                                                       convergence_criterion,
+                                                       self.settings["mechanical_solver_settings"]["strategy_type"].GetString())
+
+        # Set echo_level
+        self.Thermal_Solver.SetEchoLevel(self.settings["thermal_solver_settings"]["echo_level"].GetInt())
+        self.Mechanical_Solver.SetEchoLevel(self.settings["mechanical_solver_settings"]["echo_level"].GetInt())
+
+        # Check if everything is assigned correctly
+        self.Thermal_Solver.Check()
+        self.Mechanical_Solver.Check()
+
+        print ("Initialization DamThermoMechanicSolver finished")
+
+    def GetComputingModelPart(self):
+        return self.main_model_part.GetSubModelPart(self.mechanical_model_part_name)
+
+    def GetComputingThermalModelPart(self):
+        return self.main_model_part.GetSubModelPart(self.thermal_model_part_name)
+
+    def GetOutputVariables(self):
+        pass
+
+    def ComputeDeltaTime(self):
+        pass
+
+    def SaveRestart(self):
+        pass #one should write the restart file here
+
+    def Solve(self):
+        if self.settings["thermal_solver_settings"]["clear_storage"].GetBool():
+            self.Thermal_Solver.Clear()
+        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
+            self.Mechanical_Solver.Clear()
+
+        self.Thermal_Solver.Solve()
+        self.Mechanical_Solver.Solve()
+
+    # solve :: sequencial calls
+
+    def InitializeStrategy(self):
+        if self.settings["thermal_solver_settings"]["clear_storage"].GetBool():
+            self.Thermal_Solver.Clear()
+        if self.settings["mechanical_solver_settings"]["clear_storage"].GetBool():
+            self.Mechanical_Solver.Clear()
+
+        self.Thermal_Solver.Initialize()
+        self.Mechanical_Solver.Initialize()
+
+    def InitializeSolutionStep(self):
+        self.Thermal_Solver.InitializeSolutionStep()
+        self.Mechanical_Solver.InitializeSolutionStep()
+
+    def Predict(self):
+        self.Thermal_Solver.Predict()
+        self.Mechanical_Solver.Predict()
+
+    def SolveSolutionStep(self):
+        self.Thermal_Solver.SolveSolutionStep()
+        self.Mechanical_Solver.SolveSolutionStep()
+
+    def FinalizeSolutionStep(self):
+        self.Thermal_Solver.FinalizeSolutionStep()
+        self.Mechanical_Solver.FinalizeSolutionStep()
+
+    # solve :: sequencial calls
+
+    def SetEchoLevel(self, level):
+        self.Thermal_Solver.SetEchoLevel(level)
+        self.Mechanical_Solver.SetEchoLevel(level)
+
+    def Clear(self):
+        self.Thermal_Solver.Clear()
+        self.Mechanical_Solver.Clear()
+
+    def Check(self):
+        self.Thermal_Solver.Check()
+        self.Mechanical_Solver.Check()
+
+    #### Specific internal functions ####
+
+    def _ExecuteAfterReading(self):
+
+        self.thermal_model_part_name = "thermal_computing_domain"
+        self.mechanical_model_part_name = "mechanical_computing_domain"
+
+        # Create list of sub sub model parts (it is a copy of the standard lists with a different name)
+        self.thermal_domain_sub_sub_model_part_list = []
+        for i in range(self.settings["thermal_solver_settings"]["problem_domain_sub_model_part_list"].size()):
+            self.thermal_domain_sub_sub_model_part_list.append("sub_"+self.settings["thermal_solver_settings"]["problem_domain_sub_model_part_list"][i].GetString())
+        self.thermal_domain_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.thermal_domain_sub_sub_model_part_list))
+
+        self.thermal_loads_sub_sub_model_part_list = []
+        for i in range(self.settings["thermal_solver_settings"]["thermal_loads_sub_model_part_list"].size()):
+            self.thermal_loads_sub_sub_model_part_list.append("sub_"+self.settings["thermal_solver_settings"]["thermal_loads_sub_model_part_list"][i].GetString())
+        self.thermal_loads_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.thermal_loads_sub_sub_model_part_list))
+
+        self.body_domain_sub_sub_model_part_list = []
+        for i in range(self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"].size()):
+            self.body_domain_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"][i].GetString())
+        self.body_domain_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.body_domain_sub_sub_model_part_list))
+
+        self.loads_sub_sub_model_part_list = []
+        for i in range(self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"].size()):
+            self.loads_sub_sub_model_part_list.append("sub_"+self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"][i].GetString())
+        self.loads_sub_sub_model_part_list = KratosMultiphysics.Parameters(json.dumps(self.loads_sub_sub_model_part_list))
+
+        # Auxiliary Kratos parameters object to be called by the CheckAndPepareModelProcessDamThermal
+        aux_params = KratosMultiphysics.Parameters("{}")
+        aux_params.AddEmptyValue("thermal_model_part_name").SetString(self.thermal_model_part_name)
+        aux_params.AddValue("thermal_domain_sub_model_part_list",self.settings["thermal_solver_settings"]["problem_domain_sub_model_part_list"])
+        aux_params.AddValue("thermal_domain_sub_sub_model_part_list",self.thermal_domain_sub_sub_model_part_list)
+        aux_params.AddValue("thermal_loads_sub_model_part_list",self.settings["thermal_solver_settings"]["thermal_loads_sub_model_part_list"])
+        aux_params.AddValue("thermal_loads_sub_sub_model_part_list",self.thermal_loads_sub_sub_model_part_list)
+
+        aux_params.AddEmptyValue("mechanical_model_part_name").SetString(self.mechanical_model_part_name)
+        aux_params.AddValue("mechanical_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["problem_domain_sub_model_part_list"])
+        aux_params.AddValue("mechanical_loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["mechanical_loads_sub_model_part_list"])
+        aux_params.AddValue("body_domain_sub_model_part_list",self.settings["mechanical_solver_settings"]["body_domain_sub_model_part_list"])
+        aux_params.AddValue("body_domain_sub_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
+        aux_params.AddValue("loads_sub_model_part_list",self.settings["mechanical_solver_settings"]["loads_sub_model_part_list"])
+        aux_params.AddValue("loads_sub_sub_model_part_list",self.loads_sub_sub_model_part_list)
+
+        # CheckAndPrepareModelProcessDamMechanical creates the solid_computational_model_part
+        from KratosMultiphysics.DamApplication import check_and_prepare_model_process_dam_thermal
+        check_and_prepare_model_process_dam_thermal.CheckAndPrepareModelProcessDamThermal(self.main_model_part, aux_params).Execute()
+
+        # Constitutive law import
+        from KratosMultiphysics.DamApplication import dam_constitutive_law_utility
+        dam_constitutive_law_utility.SetConstitutiveLaw(self.main_model_part)
+
+        self.main_model_part.SetBufferSize( self.settings["buffer_size"].GetInt() )
+        minimum_buffer_size = self.GetMinimumBufferSize()
+        if(minimum_buffer_size > self.main_model_part.GetBufferSize()):
+            self.main_model_part.SetBufferSize( minimum_buffer_size )
+
+    def _ConstructBuilderAndSolver(self, block_builder, linear_solver):
+
+        # Creating the builder and solver
+        if(block_builder):
+            builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(linear_solver)
+        else:
+            builder_and_solver = KratosMultiphysics.ResidualBasedEliminationBuilderAndSolver(linear_solver)
+
+        return builder_and_solver
+
+    def _ConstructScheme(self, scheme_type, solution_type):
+
+        rayleigh_m = self.settings["mechanical_solver_settings"]["rayleigh_m"].GetDouble()
+        rayleigh_k = self.settings["mechanical_solver_settings"]["rayleigh_k"].GetDouble()
+
+        if(solution_type == "Quasi-Static"):
+            if(rayleigh_m<1.0e-15 and rayleigh_k<1.0e-15):
+                scheme =  KratosDam.IncrementalUpdateStaticSmoothingScheme()
+            else:
+                scheme =  KratosDam.IncrementalUpdateStaticDampedSmoothingScheme(rayleigh_m,rayleigh_k)
+        else:
+            if(scheme_type == "Newmark"):
+                damp_factor_m = 0.0
+            else:
+                damp_factor_m = -0.01
+            scheme = KratosDam.BossakDisplacementSmoothingScheme(damp_factor_m,rayleigh_m,rayleigh_k)
+
+        return scheme
+
+    def _ConstructConvergenceCriterion(self, convergence_criterion):
+
+        D_RT = self.settings["mechanical_solver_settings"]["displacement_relative_tolerance"].GetDouble()
+        D_AT = self.settings["mechanical_solver_settings"]["displacement_absolute_tolerance"].GetDouble()
+        R_RT = self.settings["mechanical_solver_settings"]["residual_relative_tolerance"].GetDouble()
+        R_AT = self.settings["mechanical_solver_settings"]["residual_absolute_tolerance"].GetDouble()
+        echo_level = self.settings["mechanical_solver_settings"]["echo_level"].GetInt()
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
+    def _ConstructSolver(self, builder_and_solver, scheme, convergence_criterion, strategy_type):
+
+        nonlocal_damage = self.settings["mechanical_solver_settings"]["nonlocal_damage"].GetBool()
+        max_iters = self.settings["mechanical_solver_settings"]["max_iteration"].GetInt()
+        compute_reactions = self.settings["mechanical_solver_settings"]["compute_reactions"].GetBool()
+        reform_step_dofs = self.settings["mechanical_solver_settings"]["reform_dofs_at_each_step"].GetBool()
+        move_mesh_flag = self.settings["mechanical_solver_settings"]["move_mesh_flag"].GetBool()
+
+        if strategy_type == "Newton-Raphson":
+            if nonlocal_damage:
+                self.strategy_params = KratosMultiphysics.Parameters("{}")
+                self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
+                self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
+                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
+                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
+                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
+                solver = KratosPoro.PoromechanicsNewtonRaphsonNonlocalStrategy(self.mechanical_computing_model_part,
+                                                                               scheme,
+                                                                               convergence_criterion,
+                                                                               builder_and_solver,
+                                                                               self.strategy_params,
+                                                                               max_iters,
+                                                                               compute_reactions,
+                                                                               reform_step_dofs,
+                                                                               move_mesh_flag)
+            else:
+                self.main_model_part.ProcessInfo.SetValue(KratosPoro.IS_CONVERGED, True)
+                solver = KratosMultiphysics.ResidualBasedNewtonRaphsonStrategy(self.mechanical_computing_model_part,
+                                                                                    scheme,
+                                                                                    convergence_criterion,
+                                                                                    builder_and_solver,
+                                                                                    max_iters,
+                                                                                    compute_reactions,
+                                                                                    reform_step_dofs,
+                                                                                    move_mesh_flag)
+        else:
+            # Arc-Length strategy
+            self.strategy_params = KratosMultiphysics.Parameters("{}")
+            self.strategy_params.AddValue("desired_iterations",self.settings["mechanical_solver_settings"]["desired_iterations"])
+            self.strategy_params.AddValue("max_radius_factor",self.settings["mechanical_solver_settings"]["max_radius_factor"])
+            self.strategy_params.AddValue("min_radius_factor",self.settings["mechanical_solver_settings"]["min_radius_factor"])
+            self.strategy_params.AddValue("loads_sub_model_part_list",self.loads_sub_sub_model_part_list)
+            self.strategy_params.AddValue("loads_variable_list",self.settings["mechanical_solver_settings"]["loads_variable_list"])
+            if nonlocal_damage:
+                self.strategy_params.AddValue("body_domain_sub_model_part_list",self.body_domain_sub_sub_model_part_list)
+                self.strategy_params.AddValue("characteristic_length",self.settings["mechanical_solver_settings"]["characteristic_length"])
+                self.strategy_params.AddValue("search_neighbours_step",self.settings["mechanical_solver_settings"]["search_neighbours_step"])
+                solver = KratosPoro.PoromechanicsRammArcLengthNonlocalStrategy(self.mechanical_computing_model_part,
+                                                                               scheme,
+                                                                               self.mechanical_linear_solver,
+                                                                               convergence_criterion,
+                                                                               builder_and_solver,
+                                                                               self.strategy_params,
+                                                                               max_iters,
+                                                                               compute_reactions,
+                                                                               reform_step_dofs,
+                                                                               move_mesh_flag)
+            else:
+                solver = KratosPoro.PoromechanicsRammArcLengthStrategy(self.mechanical_computing_model_part,
+                                                                       scheme,
+                                                                       self.mechanical_linear_solver,
+                                                                       convergence_criterion,
+                                                                       builder_and_solver,
+                                                                       self.strategy_params,
+                                                                       max_iters,
+                                                                       compute_reactions,
+                                                                       reform_step_dofs,
+                                                                       move_mesh_flag)
+
+        return solver
+
+    def _CheckConvergence(self):
+
+        IsConverged = self.Mechanical_Solver.IsConverged()
+
+        return IsConverged
+
+    def _UpdateLoads(self):
+
+        self.Mechanical_Solver.UpdateLoads()
```

## KratosMultiphysics/DamApplication/gid_dam_output_process.py

 * *Ordering differences only*

```diff
@@ -1,763 +1,763 @@
-import os
-import KratosMultiphysics
-from KratosMultiphysics.deprecation_management import DeprecationManager
-
-class GiDDamOutputProcess(KratosMultiphysics.Process):
-
-    defaults = KratosMultiphysics.Parameters('''{
-        "result_file_configuration": {
-            "gidpost_flags": {
-                "GiDPostMode": "GiD_PostBinary",
-                "WriteDeformedMeshFlag": "WriteUndeformed",
-                "WriteConditionsFlag": "WriteElementsOnly",
-                "MultiFileFlag": "SingleFile"
-            },
-            "output_control_type": "time_s",
-            "output_interval": 1.0,
-            "start_output_results": 0,
-            "body_output": true,
-            "node_output": false,
-            "skin_output": false,
-            "plane_output": [],
-            "nodal_results": [],
-            "nodal_nonhistorical_results": [],
-            "nodal_flags_results": [],
-            "gauss_point_results": [],
-            "additional_list_files": []
-        },
-        "point_data_configuration": []
-    }''')
-
-    default_plane_output_data = KratosMultiphysics.Parameters('''{
-        "normal": [0.0, 0.0, 0.0],
-        "point" : [0.0, 0.0, 0.0]
-    }''')
-
-    __post_mode = {
-                    # JSON input
-                    "GiD_PostAscii":        KratosMultiphysics.GiDPostMode.GiD_PostAscii,
-                    "GiD_PostAsciiZipped":  KratosMultiphysics.GiDPostMode.GiD_PostAsciiZipped,
-                    "GiD_PostBinary":       KratosMultiphysics.GiDPostMode.GiD_PostBinary,
-                    "GiD_PostHDF5":         KratosMultiphysics.GiDPostMode.GiD_PostHDF5,
-                    # Legacy
-                    "Binary":               KratosMultiphysics.GiDPostMode.GiD_PostBinary,
-                    "Ascii":                KratosMultiphysics.GiDPostMode.GiD_PostAscii,
-                    "AsciiZipped":          KratosMultiphysics.GiDPostMode.GiD_PostAsciiZipped,
-                    }
-
-    __write_deformed_mesh = {
-                    # JSON input
-                    "WriteDeformed":        KratosMultiphysics.WriteDeformedMeshFlag.WriteDeformed,
-                    "WriteUndeformed":      KratosMultiphysics.WriteDeformedMeshFlag.WriteUndeformed,
-                    # Legacy
-                    True:                   KratosMultiphysics.WriteDeformedMeshFlag.WriteDeformed,
-                    False:                  KratosMultiphysics.WriteDeformedMeshFlag.WriteUndeformed,
-                    }
-
-    __write_conditions = {
-                    # JSON input
-                    "WriteConditions":      KratosMultiphysics.WriteConditionsFlag.WriteConditions,
-                    "WriteElementsOnly":    KratosMultiphysics.WriteConditionsFlag.WriteElementsOnly,
-                    "WriteConditionsOnly":  KratosMultiphysics.WriteConditionsFlag.WriteConditionsOnly,
-                    # Legacy
-                    True:                   KratosMultiphysics.WriteConditionsFlag.WriteConditions,
-                    False:                  KratosMultiphysics.WriteConditionsFlag.WriteElementsOnly,
-                    }
-
-    __multi_file_flag = {
-                    # JSON input
-                    "SingleFile":           KratosMultiphysics.MultiFileFlag.SingleFile,
-                    "MultipleFiles":        KratosMultiphysics.MultiFileFlag.MultipleFiles,
-                    # Legacy
-                    "Multiples":            KratosMultiphysics.MultiFileFlag.MultipleFiles,
-                    "Single":               KratosMultiphysics.MultiFileFlag.SingleFile,
-                    }
-
-    def __init__(self,model_part,file_name,start_time,param = None):
-        KratosMultiphysics.Process.__init__(self)
-        if param is None:
-            param = self.defaults
-        else:
-            # Warning: we may be changing the parameters object here:
-            self.TranslateLegacyVariablesAccordingToCurrentStandard(param)
-            # Note: this only validates the first level of the JSON tree.
-            # I'm not going for recursive validation because some branches may
-            # not exist and I don't want the validator assinging defaults there.
-            param.ValidateAndAssignDefaults(self.defaults)
-
-        self.param = param
-        self.base_file_name = file_name
-
-        self.model_part = model_part
-        self.body_io = None
-        self.volume_list_files = []
-
-        # The following are only used if we asked to print results on surfaces
-        self.cut_model_part = None
-        self.cut_io = None
-        self.output_surface_index = 0
-        self.cut_list_files = []
-
-        point_data_configuration = self.param["point_data_configuration"]
-        if point_data_configuration.size() > 0:
-            from KratosMultiphysics import point_output_process
-            self.point_output_process = point_output_process.PointOutputProcess(self.model_part,point_data_configuration)
-        else:
-            self.point_output_process = None
-
-        self.start_time = start_time
-        self.step_count = 0
-        self.printed_step_count = 0
-        self.next_output = 0.0
-
-    @classmethod
-    def Flush(cls,a):
-        a.flush()
-
-    # This function can be extended with new deprecated variables as they are generated
-    def TranslateLegacyVariablesAccordingToCurrentStandard(self, settings):
-        # Defining a string to help the user understand where the warnings come from (in case any is thrown)
-        context_string = type(self).__name__
-
-        if settings.Has('result_file_configuration'):
-            sub_settings_where_var_is = settings['result_file_configuration']
-            old_name = 'output_frequency'
-            new_name = 'output_interval'
-
-            if DeprecationManager.HasDeprecatedVariable(context_string, sub_settings_where_var_is, old_name, new_name):
-                DeprecationManager.ReplaceDeprecatedVariableName(sub_settings_where_var_is, old_name, new_name)
-
-        if settings.Has('result_file_configuration'):
-            sub_settings_where_var_is = settings['result_file_configuration']
-            old_name = 'write_properties_id'
-            new_name = 'write_ids'
-
-            if DeprecationManager.HasDeprecatedVariable(context_string, sub_settings_where_var_is, old_name, new_name):
-                DeprecationManager.ReplaceDeprecatedVariableName(sub_settings_where_var_is, old_name, new_name)
-
-
-    def ExecuteInitialize(self):
-        result_file_configuration = self.param["result_file_configuration"]
-        result_file_configuration.ValidateAndAssignDefaults(self.defaults["result_file_configuration"])
-
-        # If either of these is True, we will have a volume output file
-        self.body_output = result_file_configuration["body_output"].GetBool()
-        self.node_output = result_file_configuration["node_output"].GetBool()
-
-        # If skin_output is True or we have output planes, we will have a cut output file
-        self.skin_output = result_file_configuration["skin_output"].GetBool()
-        plane_output_configuration = result_file_configuration["plane_output"] # should be of array type
-        self.num_planes = plane_output_configuration.size()
-
-        # Generate the cuts and store them in self.cut_model_part
-        if self.skin_output or self.num_planes > 0:
-            self.__initialize_cut_output(plane_output_configuration)
-
-        # Retrieve gidpost flags and setup GiD output tool
-        gidpost_flags = result_file_configuration["gidpost_flags"]
-        gidpost_flags.ValidateAndAssignDefaults(self.defaults["result_file_configuration"]["gidpost_flags"])
-
-        self.__initialize_gidio(gidpost_flags,gidpost_flags)
-
-        # Process nodal and gauss point output
-        self.nodal_variables = self.__generate_variable_list_from_input(result_file_configuration["nodal_results"])
-        self.gauss_point_variables = self.__generate_variable_list_from_input(result_file_configuration["gauss_point_results"])
-        self.nodal_nonhistorical_variables = self.__generate_variable_list_from_input(result_file_configuration["nodal_nonhistorical_results"])
-        self.nodal_flags = self.__generate_flags_list_from_input(result_file_configuration["nodal_flags_results"])
-        self.nodal_flags_names =[]
-        for i in range(result_file_configuration["nodal_flags_results"].size()):
-            self.nodal_flags_names.append(result_file_configuration["nodal_flags_results"][i].GetString())
-
-        self.output_frequency = result_file_configuration["output_interval"].GetDouble()
-        self.start_output_results = result_file_configuration["start_output_results"].GetDouble()
-
-        if self.start_time >= self.start_output_results:
-            self.start_output_results = self.start_time
-            self.next_output += self.start_output_results + self.output_frequency
-        else:
-            self.next_output += self.start_output_results
-
-        ## get .post.lst files
-        #additional_list_file_data = result_file_configuration["additional_list_files"]
-        #additional_list_files = [ additional_list_file_data[i].GetInt() for i in range(0,additional_list_file_data.size()) ]
-
-
-        # Set current time parameters
-        if(  self.model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED] == True ):
-            self.step_count = self.model_part.ProcessInfo[KratosMultiphysics.STEP]
-            self.printed_step_count = self.model_part.ProcessInfo[KratosMultiphysics.PRINTED_STEP]
-
-            self.next_output = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
-
-            label = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
-
-            self.__remove_post_results_files(label)
-
-            ## Restart .post.lst files
-            #self.__restart_list_files(additional_list_files)
-        #else:
-            ## Create .post.lst files
-            #self.__initialize_list_files(additional_list_files)
-
-        # Process point recording data
-        if self.point_output_process is not None:
-            self.point_output_process.ExecuteInitialize()
-
-    def ExecuteBeforeSolutionLoop(self):
-        '''Initialize output meshes.'''
-        label = max(self.start_output_results, self.start_time)
-        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.SingleFile:
-            mesh_name = 0
-            self.__write_mesh(mesh_name)
-            self.__initialize_results(mesh_name)
-            if (self.start_output_results == 0) or (not self.start_time == 0):
-                self.__write_nodal_results(label)
-                self.__write_gp_results(label)
-                self.__write_nonhistorical_nodal_results(label)
-                self.__write_nodal_flags(label)
-
-        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
-            if (self.start_output_results == 0) or (not self.start_time == 0):
-                self.__write_mesh(label)
-                self.__initialize_results(label)
-                self.__write_nodal_results(label)
-                self.__write_nonhistorical_nodal_results(label)
-                self.__write_nodal_flags(label)
-                self.__finalize_results()
-
-            result_file_configuration = self.param["result_file_configuration"]
-            output_control_type = result_file_configuration["output_control_type"].GetString()
-            if output_control_type == "time_s":
-                self.multifiles = (
-                    MultifileList(self.base_file_name, 1),
-                    MultifileList(self.base_file_name, 60),
-                    MultifileList(self.base_file_name, 3600),
-                    MultifileList(self.base_file_name, 43200),
-                    MultifileList(self.base_file_name, 86400),
-                )
-            elif output_control_type == "time_h":
-                self.multifiles = (
-                    MultifileList(self.base_file_name, 1),
-                    MultifileList(self.base_file_name, 12),
-                    MultifileList(self.base_file_name, 24),
-                    MultifileList(self.base_file_name, 168),
-                )
-            elif output_control_type == "time_d":
-                self.multifiles = (
-                    MultifileList(self.base_file_name, 1),
-                    MultifileList(self.base_file_name, 7),
-                )
-            elif output_control_type == "time_w":
-                self.multifiles = (
-                    MultifileList(self.base_file_name, 1),
-                )
-            elif output_control_type == "step":
-                self.multifiles = (
-                    MultifileList(self.base_file_name, 1),
-                )
-            else:
-                msg = "{0} Error: Unknown value \"{1}\" read for parameter \"{2}\"".format(self.__class__.__name__,output_control_type,"output_control_type")
-                raise Exception(msg)
-
-            self.multifilelists = []
-            self.__set_multifile_lists(self.multifiles)
-
-            if self.start_output_results == 0:
-                self.__write_inital_step_in_multifile_lists(label)
-
-        if self.point_output_process is not None:
-            self.point_output_process.ExecuteBeforeSolutionLoop()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        self.step_count += 1
-
-        if self.point_output_process is not None:
-            self.point_output_process.ExecuteInitializeSolutionStep()
-
-    def ExecuteFinalizeSolutionStep(self):
-
-        if self.point_output_process is not None:
-            self.point_output_process.ExecuteFinalizeSolutionStep()
-
-    def IsOutputStep(self):
-
-        result_file_configuration = self.param["result_file_configuration"]
-        time = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
-        if result_file_configuration["output_control_type"].GetString() == "time_s":
-            time = time
-        elif result_file_configuration["output_control_type"].GetString() == "time_h":
-            time = time/3600.0
-        elif result_file_configuration["output_control_type"].GetString() == "time_d":
-            time = time/86400.0
-        elif result_file_configuration["output_control_type"].GetString() == "time_w":
-            time = time/604800.0
-
-        return ( time >= self.next_output )
-
-    def PrintOutput(self):
-
-        result_file_configuration = self.param["result_file_configuration"]
-        self.output_frequency = result_file_configuration["output_interval"].GetDouble()
-
-        if self.point_output_process is not None:
-            self.point_output_process.ExecuteBeforeOutputStep()
-            if self.point_output_process.IsOutputStep():
-                self.point_output_process.PrintOutput()
-
-        # Print the output
-        time = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
-        self.printed_step_count += 1
-        self.model_part.ProcessInfo[KratosMultiphysics.PRINTED_STEP] = self.printed_step_count
-
-        if result_file_configuration["output_control_type"].GetString() == "time_s":
-            label = time
-            time = time
-        elif result_file_configuration["output_control_type"].GetString() == "time_h":
-            label = time/3600
-            time = time/3600.0
-        elif result_file_configuration["output_control_type"].GetString() == "time_d":
-            label = time/86400
-            time = time/86400.0
-        elif result_file_configuration["output_control_type"].GetString() == "time_w":
-            label = time/604800
-            time = time/604800.0
-
-        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
-            self.__write_mesh(label)
-            self.__initialize_results(label)
-
-        self.__write_nodal_results(time)
-        self.__write_gp_results(time)
-        self.__write_nonhistorical_nodal_results(time)
-        self.__write_nodal_flags(time)
-
-        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
-            self.__finalize_results()
-            self.__write_multifile_lists(label)
-
-        # Schedule next output
-        if self.output_frequency > 0.0: # Note: if == 0, we'll just always print
-            while self.next_output <= time:
-                self.next_output += self.output_frequency
-
-        if self.point_output_process is not None:
-            self.point_output_process.ExecuteAfterOutputStep()
-
-    def ExecuteFinalize(self):
-        '''Finalize files and free resources.'''
-
-        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.SingleFile:
-            self.__finalize_results()
-
-        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
-            self.__close_multifiles()
-
-        if self.point_output_process is not None:
-            self.point_output_process.ExecuteFinalize()
-
-        # NOTE (PR): The followin lines were commented due to a warnign from 'codacy' while doing a PR. In the original 'gid_outpu_process.py these lines are uncommented.'
-        #~ for freq,f in self.volume_list_files:
-            #~ f.close()
-        #~ for freq,f in self.cut_list_files:
-            #~ f.close()
-
-        # Note: it is important to call the GidIO destructor, since it closes output files
-        # Since Python's garbage colletion DOES NOT ensure that the destructor will be called,
-        # I'm deallocating the GidIO instances explicitly. This is VERY BAD PRACTICE
-        # and effectively breaks the class if called after this point, but we haven't found
-        # a better solution yet (jcotela 12/V/2016)
-        del self.body_io
-        del self.cut_io
-
-    def __initialize_gidio(self,gidpost_flags,param):
-        '''Initialize GidIO objects (for volume and cut outputs) and related data.'''
-        self.volume_file_name = self.base_file_name
-        self.cut_file_name = self.volume_file_name+"_cuts"
-        self.post_mode = self.__get_gidpost_flag(param, "GiDPostMode", self.__post_mode)
-        self.write_deformed_mesh = self.__get_gidpost_flag(param, "WriteDeformedMeshFlag", self.__write_deformed_mesh)
-        self.write_conditions = self.__get_gidpost_flag(param,"WriteConditionsFlag",self.__write_conditions)
-        self.multifile_flag = self.__get_gidpost_flag(param,"MultiFileFlag", self.__multi_file_flag)
-
-        if self.body_output or self.node_output:
-            self.body_io = KratosMultiphysics.GidIO(self.volume_file_name,
-                                                    self.post_mode,
-                                                    self.multifile_flag,
-                                                    self.write_deformed_mesh,
-                                                    self.write_conditions)
-
-        if self.skin_output or self.num_planes > 0:
-            self.cut_io = KratosMultiphysics.GidIO(self.cut_file_name,
-                                                   self.post_mode,
-                                                   self.multifile_flag,
-                                                   self.write_deformed_mesh,
-                                                   KratosMultiphysics.WriteConditionsFlag.WriteConditionsOnly) # Cuts are conditions, so we always print conditions in the cut ModelPart
-
-    def __get_gidpost_flag(self, param, label, dictionary):
-        '''Parse gidpost settings using an auxiliary dictionary of acceptable values.'''
-
-        keystring = param[label].GetString()
-        try:
-            value = dictionary[keystring]
-        except KeyError:
-            msg = "{0} Error: Unknown value \"{1}\" read for parameter \"{2}\"".format(self.__class__.__name__,value,label)
-            raise Exception(msg)
-
-        return value
-
-    def __initialize_cut_output(self,plane_output_configuration):
-        '''Set up tools used to produce output in skin and cut planes.'''
-
-        self.cut_model_part = ModelPart("CutPart")
-        self.cut_manager = CuttingUtility()
-        self.cut_manager.FindSmallestEdge(self.model_part)
-        self.cut_manager.AddVariablesToCutModelPart(self.model_part,self.cut_model_part)
-        if self.skin_output:
-            self.cut_manager.AddSkinConditions(self.model_part,self.cut_model_part,self.output_surface_index)
-            self.output_surface_index += 1
-
-        for plane_id in range(0,plane_output_configuration.size()):
-
-            cut_data = plane_output_configuration[plane_id]
-            # This part of the input data is validated term by term
-            cut_data.ValidateAndAssignDefaults(self.default_plane_output_data)
-
-            self.__define_output_plane(cut_data)
-
-    def __initialize_list_files(self,additional_frequencies):
-        '''Set up .post.lst files for global and cut results.
-        If we have only one tipe of output (volume or cut), the
-        list file is called <gid_model_name>.post.lst. When we have
-        both types, call the volume one <gid_model_name>.post.lst and
-        the cut one <gid_model_name>_cuts.post.lst.
-        additional_frequencies should contain an array of ints N representing
-        the frequencies of additional list files. If it is not empty and GidIO
-        is configured to print multiple files, extra list files are written,
-        listing one in every N output files.'''
-        # Get a name for the GiD list file
-        # if the model folder is model.gid, the list file should be called
-        # model.post.lst
-        # NOTE (PR): In the followin lines, two variables were removed (path and ext). See 'gid_output_process.py'. They were put only because the functions have two output arguments. We can call just the one we need.
-        folder_name = os.path.split(os.getcwd())[1]
-        model_name = os.path.splitext(folder_name)[0]
-        name_base = model_name
-        name_ext = ".post.lst"
-
-        # Remove 1 from extra frequencies (and remove duplicates)
-        used_frequencies = [1,]
-        extra_frequencies = []
-        for f in additional_frequencies:
-            if f not in used_frequencies:
-                used_frequencies.append(f)
-                extra_frequencies.append(f)
-
-        if self.body_io is not None:
-            list_file = open(name_base+name_ext,"w")
-
-            if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
-                list_file.write("Multiple\n")
-            elif self.multifile_flag == KratosMultiphysics.MultiFileFlag.SingleFile:
-                list_file.write("Single\n")
-
-            self.volume_list_files.append( [1,list_file] )
-
-            if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
-                for freq in extra_frequencies:
-                    list_file_name = "{0}_list_{1}{2}".format(name_base,freq,name_ext)
-                    list_file = open(list_file_name,"w")
-                    list_file.write("Multiple\n")
-
-                    self.volume_list_files.append( [freq,list_file] )
-
-            name_base = "{0}_cuts".format(model_name)
-
-        if self.cut_io is not None:
-
-            list_file = open(name_base+name_ext,"w")
-
-            if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
-                list_file.write("Multiple\n")
-            elif self.multifile_flag == KratosMultiphysics.MultiFileFlag.SingleFile:
-                list_file.write("Single\n")
-
-            self.cut_list_files.append( [1,list_file] )
-
-            if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
-                for freq in extra_frequencies:
-                    list_file_name = "{0}_list_{1}{2}".format(name_base,freq,name_ext)
-                    list_file = open(list_file_name,"w")
-                    list_file.write("Multiple\n")
-
-                    self.cut_list_files.append( [freq,list_file] )
-
-    def __define_output_plane(self,cut_data):
-        '''Add a plane to the output plane list.'''
-
-        normal_data = cut_data["normal"]
-        n = Vector(3)
-        n[0] = normal_data[0].GetDouble()
-        n[1] = normal_data[1].GetDouble()
-        n[2] = normal_data[2].GetDouble()
-        # Sanity check on normal
-        norm2 = n[0]*n[0] + n[1]*n[1] + n[2]*n[2]
-        if norm2 < 1e-12:
-            raise Exception("{0} Error: something went wrong in output plane definition: plane {1} has a normal with module 0.".format(self.__class__.__name__,self.output_surface_index))
-
-        point_data = cut_data["point"]
-        p = Vector(3)
-        p[0] = point_data[0].GetDouble()
-        p[1] = point_data[1].GetDouble()
-        p[2] = point_data[2].GetDouble()
-
-        # And finally, define the plane
-        self.output_surface_index += 1
-        self.cut_manager.GenerateCut(   self.model_part,
-                                        self.cut_model_part,
-                                        n,
-                                        p,
-                                        self.output_surface_index,
-                                        0.01)
-
-    def __generate_variable_list_from_input(self,param):
-        '''Parse a list of variables from input.'''
-        # At least verify that the input is a string
-        if not param.IsArray():
-            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
-
-        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
-        return [ KratosMultiphysics.KratosGlobals.GetVariable( param[i].GetString() ) for i in range( 0,param.size() ) ]
-
-    def __generate_flags_list_from_input(self,param):
-        '''Parse a list of variables from input.'''
-        # At least verify that the input is a string
-        if not param.IsArray():
-            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
-
-        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
-        return [ globals()[ param[i].GetString() ] for i in range( 0,param.size() ) ]
-
-    def __write_mesh(self, label):
-
-        if self.body_io is not None:
-            self.body_io.InitializeMesh(label)
-            if self.body_output:
-                self.body_io.WriteMesh(self.model_part.GetMesh())
-            if self.node_output:
-                self.body_io.WriteNodeMesh(self.model_part.GetMesh())
-            self.body_io.FinalizeMesh()
-
-        if self.cut_io is not None:
-            self.cut_io.InitializeMesh(label)
-            self.cut_io.WriteMesh(self.cut_model_part.GetMesh())
-            self.cut_io.FinalizeMesh()
-
-    def __initialize_results(self, label):
-
-        if self.body_io is not None:
-            self.body_io.InitializeResults(label, self.model_part.GetMesh())
-
-        if self.cut_io is not None:
-            self.cut_io.InitializeResults(label,self.cut_model_part.GetMesh())
-
-    def __write_nodal_results(self, label):
-
-        if self.body_io is not None:
-            for variable in self.nodal_variables:
-                self.body_io.WriteNodalResults(variable, self.model_part.GetCommunicator().LocalMesh().Nodes, label, 0)
-
-        if self.cut_io is not None:
-            self.cut_manager.UpdateCutData(self.cut_model_part, self.model_part)
-            for variable in self.nodal_variables:
-                self.cut_io.WriteNodalResults(variable, self.cut_model_part.GetCommunicator().LocalMesh().Nodes, label, 0)
-
-    def __write_gp_results(self, label):
-
-        #if self.body_io is not None:
-        if self.body_output: # Note: if we only print nodes, there are no GaussPoints
-            for variable in self.gauss_point_variables:
-                self.body_io.PrintOnGaussPoints(variable, self.model_part, label)
-
-        # Gauss point results depend on the type of element!
-        # they are not implemented for cuts (which are generic Condition3D)
-
-    def __write_nonhistorical_nodal_results(self, label):
-
-        if self.body_io is not None:
-            for variable in self.nodal_nonhistorical_variables:
-                self.body_io.WriteNodalResultsNonHistorical(variable, self.model_part.Nodes, label)
-
-        if self.cut_io is not None:
-            self.cut_manager.UpdateCutData(self.cut_model_part, self.model_part)
-            for variable in self.nodal_nonhistorical_variables:
-                self.cut_io.WriteNodalResultsNonHistorical(variable, self.cut_model_part.Nodes, label)
-
-    def __write_nodal_flags(self, label):
-        if self.body_io is not None:
-            for flag in range(len(self.nodal_flags)):
-                self.body_io.WriteNodalFlags(self.nodal_flags[flag], self.nodal_flags_names[flag], self.model_part.Nodes, label)
-
-        if self.cut_io is not None:
-            self.cut_manager.UpdateCutData(self.cut_model_part, self.model_part)
-            for flag in range(len(self.nodal_flags)):
-                self.cut_io.WriteNodalFlags(self.nodal_flags[flag], self.nodal_flags_names[flag], self.cut_model_part.Nodes, label)
-
-    def __finalize_results(self):
-
-        if self.body_io is not None:
-            self.body_io.FinalizeResults()
-
-        if self.cut_io is not None:
-            self.cut_io.FinalizeResults()
-
-    def __restart_list_files(self,additional_frequencies):
-
-        self.__remove_list_files()
-
-        self.__initialize_list_files(additional_frequencies)
-
-        if self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostBinary:
-            ext = ".post.bin"
-        elif self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostAscii:
-            ext = ".post.res"
-        elif self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostAsciiZipped:
-            ext = ".post.res"
-        else:
-            return # No support for list_files in this format
-
-
-        # Rebuild List Files from existing problem build
-        file_id   = []
-
-        path = os.getcwd()
-
-        for f in os.listdir(path):
-
-            if(f.endswith(ext)):
-
-                #if f.name = problem_tested_145.post.bin
-                file_parts = f.split('_')  # you get ["problem","tested","145.post.bin"]
-                num_parts  = len(file_parts)
-
-                end_parts  = file_parts[num_parts-1].split(".") # you get ["145","post","bin"]
-                print_id   = end_parts[0] # you get "145"
-
-                if( print_id != "0" ):
-                    file_id.append(int(print_id))
-
-            file_id.sort()
-
-    def __set_multifile_lists(self,multifile_list):
-        for mfilelist in multifile_list:
-            self.multifilelists.append(mfilelist)
-
-        for mfilelist in self.multifilelists:
-            mfilelist.file.write("Multiple\n")
-            mfilelist.index = 1
-
-    def __write_inital_step_in_multifile_lists(self, label):
-        for mfilelist in self.multifilelists:
-
-            if (self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostBinary):
-                text_to_print = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.bin\n"
-                mfilelist.file.write(text_to_print)
-            else:
-                text_to_print1 = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.msh\n"
-                text_to_print2 = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.res\n"
-                mfilelist.file.write(text_to_print1)
-                mfilelist.file.write(text_to_print2)
-            self.Flush(mfilelist.file)
-
-    def __write_multifile_lists(self, label):
-
-        for mfilelist in self.multifilelists:
-            if (label % mfilelist.step) == 0:
-
-                if (self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostBinary):
-                    text_to_print = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.bin\n"
-                    mfilelist.file.write(text_to_print)
-                else:
-                    text_to_print1 = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.msh\n"
-                    text_to_print2 = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.res\n"
-                    mfilelist.file.write(text_to_print1)
-                    mfilelist.file.write(text_to_print2)
-                self.Flush(mfilelist.file)
-
-    @classmethod
-    def __get_multifile_list_name(cls, name):
-        return name
-
-    def __close_multifiles(self):
-        for mfilelist in self.multifilelists:
-            mfilelist.file.close()
-
-    # NOTE (PR): 'Codacy' suggest to change the following method, from a standard method to a 'classmethod' or 'staticmethod' as it does not refer to any of the class attributes
-    @classmethod
-    def __remove_list_files(cls):
-
-        path = os.getcwd()
-
-        # remove previous list files:
-        if(os.path.exists(path) == False):
-            print(" Problem Path do not exists , check the Problem Path selected ")
-        else:
-            filelist = [f for f in os.listdir(os.getcwd()) if f.endswith(".lst")]
-            for f in filelist:
-                if(os.path.exists(f)):
-                    try:
-                        os.remove(f)
-                    except WindowsError:
-                        pass
-
-    def __remove_post_results_files(self, step_label):
-
-        path = os.getcwd()
-
-        if self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostBinary:
-            ext = ".post.bin"
-        elif self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostAscii:
-            ext = ".post.res"
-        elif self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostAsciiZipped:
-            ext = ".post.res"
-
-        # remove post result files:
-        if(os.path.exists(path) == False):
-            print(" Problem Path do not exists , check the Problem Path selected ")
-        else:
-            filelist = []
-            for f in os.listdir(os.getcwd()):
-                if(f.endswith(ext)):
-
-                    #if f.name = problem_tested_145.post.bin
-                    file_parts = f.split('_')
-                    # you get the parts ["problem","tested","145.post.bin"]
-                    num_parts  = len(file_parts)
-                    # take the last part
-                    end_parts  = file_parts[num_parts-1].split(".")
-                    # you get the parts ["145","post","bin"]
-                    print_id   = end_parts[0]
-                    # you get "145"
-
-                    try:
-                        float(print_id)
-                    except ValueError:
-                        break
-
-                    if( float(print_id) >  float(step_label) ):
-                        filelist.append(f)
-
-            for f in filelist:
-                if(os.path.exists(f)):
-                    try:
-                        os.remove(f)
-                    except WindowsError:
-                        pass
-
-
-class MultifileList(object):
-
-    def __init__(self, name, step):
-        self.index = 0
-        self.step = step
-        self.name = name
-        absolute_path_to_file = os.path.join("_list_" + self.name + "_" + str(step) + ".post.lst")
-        self.file = open(absolute_path_to_file,"w")
+import os
+import KratosMultiphysics
+from KratosMultiphysics.deprecation_management import DeprecationManager
+
+class GiDDamOutputProcess(KratosMultiphysics.Process):
+
+    defaults = KratosMultiphysics.Parameters('''{
+        "result_file_configuration": {
+            "gidpost_flags": {
+                "GiDPostMode": "GiD_PostBinary",
+                "WriteDeformedMeshFlag": "WriteUndeformed",
+                "WriteConditionsFlag": "WriteElementsOnly",
+                "MultiFileFlag": "SingleFile"
+            },
+            "output_control_type": "time_s",
+            "output_interval": 1.0,
+            "start_output_results": 0,
+            "body_output": true,
+            "node_output": false,
+            "skin_output": false,
+            "plane_output": [],
+            "nodal_results": [],
+            "nodal_nonhistorical_results": [],
+            "nodal_flags_results": [],
+            "gauss_point_results": [],
+            "additional_list_files": []
+        },
+        "point_data_configuration": []
+    }''')
+
+    default_plane_output_data = KratosMultiphysics.Parameters('''{
+        "normal": [0.0, 0.0, 0.0],
+        "point" : [0.0, 0.0, 0.0]
+    }''')
+
+    __post_mode = {
+                    # JSON input
+                    "GiD_PostAscii":        KratosMultiphysics.GiDPostMode.GiD_PostAscii,
+                    "GiD_PostAsciiZipped":  KratosMultiphysics.GiDPostMode.GiD_PostAsciiZipped,
+                    "GiD_PostBinary":       KratosMultiphysics.GiDPostMode.GiD_PostBinary,
+                    "GiD_PostHDF5":         KratosMultiphysics.GiDPostMode.GiD_PostHDF5,
+                    # Legacy
+                    "Binary":               KratosMultiphysics.GiDPostMode.GiD_PostBinary,
+                    "Ascii":                KratosMultiphysics.GiDPostMode.GiD_PostAscii,
+                    "AsciiZipped":          KratosMultiphysics.GiDPostMode.GiD_PostAsciiZipped,
+                    }
+
+    __write_deformed_mesh = {
+                    # JSON input
+                    "WriteDeformed":        KratosMultiphysics.WriteDeformedMeshFlag.WriteDeformed,
+                    "WriteUndeformed":      KratosMultiphysics.WriteDeformedMeshFlag.WriteUndeformed,
+                    # Legacy
+                    True:                   KratosMultiphysics.WriteDeformedMeshFlag.WriteDeformed,
+                    False:                  KratosMultiphysics.WriteDeformedMeshFlag.WriteUndeformed,
+                    }
+
+    __write_conditions = {
+                    # JSON input
+                    "WriteConditions":      KratosMultiphysics.WriteConditionsFlag.WriteConditions,
+                    "WriteElementsOnly":    KratosMultiphysics.WriteConditionsFlag.WriteElementsOnly,
+                    "WriteConditionsOnly":  KratosMultiphysics.WriteConditionsFlag.WriteConditionsOnly,
+                    # Legacy
+                    True:                   KratosMultiphysics.WriteConditionsFlag.WriteConditions,
+                    False:                  KratosMultiphysics.WriteConditionsFlag.WriteElementsOnly,
+                    }
+
+    __multi_file_flag = {
+                    # JSON input
+                    "SingleFile":           KratosMultiphysics.MultiFileFlag.SingleFile,
+                    "MultipleFiles":        KratosMultiphysics.MultiFileFlag.MultipleFiles,
+                    # Legacy
+                    "Multiples":            KratosMultiphysics.MultiFileFlag.MultipleFiles,
+                    "Single":               KratosMultiphysics.MultiFileFlag.SingleFile,
+                    }
+
+    def __init__(self,model_part,file_name,start_time,param = None):
+        KratosMultiphysics.Process.__init__(self)
+        if param is None:
+            param = self.defaults
+        else:
+            # Warning: we may be changing the parameters object here:
+            self.TranslateLegacyVariablesAccordingToCurrentStandard(param)
+            # Note: this only validates the first level of the JSON tree.
+            # I'm not going for recursive validation because some branches may
+            # not exist and I don't want the validator assinging defaults there.
+            param.ValidateAndAssignDefaults(self.defaults)
+
+        self.param = param
+        self.base_file_name = file_name
+
+        self.model_part = model_part
+        self.body_io = None
+        self.volume_list_files = []
+
+        # The following are only used if we asked to print results on surfaces
+        self.cut_model_part = None
+        self.cut_io = None
+        self.output_surface_index = 0
+        self.cut_list_files = []
+
+        point_data_configuration = self.param["point_data_configuration"]
+        if point_data_configuration.size() > 0:
+            from KratosMultiphysics import point_output_process
+            self.point_output_process = point_output_process.PointOutputProcess(self.model_part,point_data_configuration)
+        else:
+            self.point_output_process = None
+
+        self.start_time = start_time
+        self.step_count = 0
+        self.printed_step_count = 0
+        self.next_output = 0.0
+
+    @classmethod
+    def Flush(cls,a):
+        a.flush()
+
+    # This function can be extended with new deprecated variables as they are generated
+    def TranslateLegacyVariablesAccordingToCurrentStandard(self, settings):
+        # Defining a string to help the user understand where the warnings come from (in case any is thrown)
+        context_string = type(self).__name__
+
+        if settings.Has('result_file_configuration'):
+            sub_settings_where_var_is = settings['result_file_configuration']
+            old_name = 'output_frequency'
+            new_name = 'output_interval'
+
+            if DeprecationManager.HasDeprecatedVariable(context_string, sub_settings_where_var_is, old_name, new_name):
+                DeprecationManager.ReplaceDeprecatedVariableName(sub_settings_where_var_is, old_name, new_name)
+
+        if settings.Has('result_file_configuration'):
+            sub_settings_where_var_is = settings['result_file_configuration']
+            old_name = 'write_properties_id'
+            new_name = 'write_ids'
+
+            if DeprecationManager.HasDeprecatedVariable(context_string, sub_settings_where_var_is, old_name, new_name):
+                DeprecationManager.ReplaceDeprecatedVariableName(sub_settings_where_var_is, old_name, new_name)
+
+
+    def ExecuteInitialize(self):
+        result_file_configuration = self.param["result_file_configuration"]
+        result_file_configuration.ValidateAndAssignDefaults(self.defaults["result_file_configuration"])
+
+        # If either of these is True, we will have a volume output file
+        self.body_output = result_file_configuration["body_output"].GetBool()
+        self.node_output = result_file_configuration["node_output"].GetBool()
+
+        # If skin_output is True or we have output planes, we will have a cut output file
+        self.skin_output = result_file_configuration["skin_output"].GetBool()
+        plane_output_configuration = result_file_configuration["plane_output"] # should be of array type
+        self.num_planes = plane_output_configuration.size()
+
+        # Generate the cuts and store them in self.cut_model_part
+        if self.skin_output or self.num_planes > 0:
+            self.__initialize_cut_output(plane_output_configuration)
+
+        # Retrieve gidpost flags and setup GiD output tool
+        gidpost_flags = result_file_configuration["gidpost_flags"]
+        gidpost_flags.ValidateAndAssignDefaults(self.defaults["result_file_configuration"]["gidpost_flags"])
+
+        self.__initialize_gidio(gidpost_flags,gidpost_flags)
+
+        # Process nodal and gauss point output
+        self.nodal_variables = self.__generate_variable_list_from_input(result_file_configuration["nodal_results"])
+        self.gauss_point_variables = self.__generate_variable_list_from_input(result_file_configuration["gauss_point_results"])
+        self.nodal_nonhistorical_variables = self.__generate_variable_list_from_input(result_file_configuration["nodal_nonhistorical_results"])
+        self.nodal_flags = self.__generate_flags_list_from_input(result_file_configuration["nodal_flags_results"])
+        self.nodal_flags_names =[]
+        for i in range(result_file_configuration["nodal_flags_results"].size()):
+            self.nodal_flags_names.append(result_file_configuration["nodal_flags_results"][i].GetString())
+
+        self.output_frequency = result_file_configuration["output_interval"].GetDouble()
+        self.start_output_results = result_file_configuration["start_output_results"].GetDouble()
+
+        if self.start_time >= self.start_output_results:
+            self.start_output_results = self.start_time
+            self.next_output += self.start_output_results + self.output_frequency
+        else:
+            self.next_output += self.start_output_results
+
+        ## get .post.lst files
+        #additional_list_file_data = result_file_configuration["additional_list_files"]
+        #additional_list_files = [ additional_list_file_data[i].GetInt() for i in range(0,additional_list_file_data.size()) ]
+
+
+        # Set current time parameters
+        if(  self.model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED] == True ):
+            self.step_count = self.model_part.ProcessInfo[KratosMultiphysics.STEP]
+            self.printed_step_count = self.model_part.ProcessInfo[KratosMultiphysics.PRINTED_STEP]
+
+            self.next_output = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
+
+            label = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
+
+            self.__remove_post_results_files(label)
+
+            ## Restart .post.lst files
+            #self.__restart_list_files(additional_list_files)
+        #else:
+            ## Create .post.lst files
+            #self.__initialize_list_files(additional_list_files)
+
+        # Process point recording data
+        if self.point_output_process is not None:
+            self.point_output_process.ExecuteInitialize()
+
+    def ExecuteBeforeSolutionLoop(self):
+        '''Initialize output meshes.'''
+        label = max(self.start_output_results, self.start_time)
+        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.SingleFile:
+            mesh_name = 0
+            self.__write_mesh(mesh_name)
+            self.__initialize_results(mesh_name)
+            if (self.start_output_results == 0) or (not self.start_time == 0):
+                self.__write_nodal_results(label)
+                self.__write_gp_results(label)
+                self.__write_nonhistorical_nodal_results(label)
+                self.__write_nodal_flags(label)
+
+        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
+            if (self.start_output_results == 0) or (not self.start_time == 0):
+                self.__write_mesh(label)
+                self.__initialize_results(label)
+                self.__write_nodal_results(label)
+                self.__write_nonhistorical_nodal_results(label)
+                self.__write_nodal_flags(label)
+                self.__finalize_results()
+
+            result_file_configuration = self.param["result_file_configuration"]
+            output_control_type = result_file_configuration["output_control_type"].GetString()
+            if output_control_type == "time_s":
+                self.multifiles = (
+                    MultifileList(self.base_file_name, 1),
+                    MultifileList(self.base_file_name, 60),
+                    MultifileList(self.base_file_name, 3600),
+                    MultifileList(self.base_file_name, 43200),
+                    MultifileList(self.base_file_name, 86400),
+                )
+            elif output_control_type == "time_h":
+                self.multifiles = (
+                    MultifileList(self.base_file_name, 1),
+                    MultifileList(self.base_file_name, 12),
+                    MultifileList(self.base_file_name, 24),
+                    MultifileList(self.base_file_name, 168),
+                )
+            elif output_control_type == "time_d":
+                self.multifiles = (
+                    MultifileList(self.base_file_name, 1),
+                    MultifileList(self.base_file_name, 7),
+                )
+            elif output_control_type == "time_w":
+                self.multifiles = (
+                    MultifileList(self.base_file_name, 1),
+                )
+            elif output_control_type == "step":
+                self.multifiles = (
+                    MultifileList(self.base_file_name, 1),
+                )
+            else:
+                msg = "{0} Error: Unknown value \"{1}\" read for parameter \"{2}\"".format(self.__class__.__name__,output_control_type,"output_control_type")
+                raise Exception(msg)
+
+            self.multifilelists = []
+            self.__set_multifile_lists(self.multifiles)
+
+            if self.start_output_results == 0:
+                self.__write_inital_step_in_multifile_lists(label)
+
+        if self.point_output_process is not None:
+            self.point_output_process.ExecuteBeforeSolutionLoop()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        self.step_count += 1
+
+        if self.point_output_process is not None:
+            self.point_output_process.ExecuteInitializeSolutionStep()
+
+    def ExecuteFinalizeSolutionStep(self):
+
+        if self.point_output_process is not None:
+            self.point_output_process.ExecuteFinalizeSolutionStep()
+
+    def IsOutputStep(self):
+
+        result_file_configuration = self.param["result_file_configuration"]
+        time = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
+        if result_file_configuration["output_control_type"].GetString() == "time_s":
+            time = time
+        elif result_file_configuration["output_control_type"].GetString() == "time_h":
+            time = time/3600.0
+        elif result_file_configuration["output_control_type"].GetString() == "time_d":
+            time = time/86400.0
+        elif result_file_configuration["output_control_type"].GetString() == "time_w":
+            time = time/604800.0
+
+        return ( time >= self.next_output )
+
+    def PrintOutput(self):
+
+        result_file_configuration = self.param["result_file_configuration"]
+        self.output_frequency = result_file_configuration["output_interval"].GetDouble()
+
+        if self.point_output_process is not None:
+            self.point_output_process.ExecuteBeforeOutputStep()
+            if self.point_output_process.IsOutputStep():
+                self.point_output_process.PrintOutput()
+
+        # Print the output
+        time = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
+        self.printed_step_count += 1
+        self.model_part.ProcessInfo[KratosMultiphysics.PRINTED_STEP] = self.printed_step_count
+
+        if result_file_configuration["output_control_type"].GetString() == "time_s":
+            label = time
+            time = time
+        elif result_file_configuration["output_control_type"].GetString() == "time_h":
+            label = time/3600
+            time = time/3600.0
+        elif result_file_configuration["output_control_type"].GetString() == "time_d":
+            label = time/86400
+            time = time/86400.0
+        elif result_file_configuration["output_control_type"].GetString() == "time_w":
+            label = time/604800
+            time = time/604800.0
+
+        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
+            self.__write_mesh(label)
+            self.__initialize_results(label)
+
+        self.__write_nodal_results(time)
+        self.__write_gp_results(time)
+        self.__write_nonhistorical_nodal_results(time)
+        self.__write_nodal_flags(time)
+
+        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
+            self.__finalize_results()
+            self.__write_multifile_lists(label)
+
+        # Schedule next output
+        if self.output_frequency > 0.0: # Note: if == 0, we'll just always print
+            while self.next_output <= time:
+                self.next_output += self.output_frequency
+
+        if self.point_output_process is not None:
+            self.point_output_process.ExecuteAfterOutputStep()
+
+    def ExecuteFinalize(self):
+        '''Finalize files and free resources.'''
+
+        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.SingleFile:
+            self.__finalize_results()
+
+        if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
+            self.__close_multifiles()
+
+        if self.point_output_process is not None:
+            self.point_output_process.ExecuteFinalize()
+
+        # NOTE (PR): The followin lines were commented due to a warnign from 'codacy' while doing a PR. In the original 'gid_outpu_process.py these lines are uncommented.'
+        #~ for freq,f in self.volume_list_files:
+            #~ f.close()
+        #~ for freq,f in self.cut_list_files:
+            #~ f.close()
+
+        # Note: it is important to call the GidIO destructor, since it closes output files
+        # Since Python's garbage colletion DOES NOT ensure that the destructor will be called,
+        # I'm deallocating the GidIO instances explicitly. This is VERY BAD PRACTICE
+        # and effectively breaks the class if called after this point, but we haven't found
+        # a better solution yet (jcotela 12/V/2016)
+        del self.body_io
+        del self.cut_io
+
+    def __initialize_gidio(self,gidpost_flags,param):
+        '''Initialize GidIO objects (for volume and cut outputs) and related data.'''
+        self.volume_file_name = self.base_file_name
+        self.cut_file_name = self.volume_file_name+"_cuts"
+        self.post_mode = self.__get_gidpost_flag(param, "GiDPostMode", self.__post_mode)
+        self.write_deformed_mesh = self.__get_gidpost_flag(param, "WriteDeformedMeshFlag", self.__write_deformed_mesh)
+        self.write_conditions = self.__get_gidpost_flag(param,"WriteConditionsFlag",self.__write_conditions)
+        self.multifile_flag = self.__get_gidpost_flag(param,"MultiFileFlag", self.__multi_file_flag)
+
+        if self.body_output or self.node_output:
+            self.body_io = KratosMultiphysics.GidIO(self.volume_file_name,
+                                                    self.post_mode,
+                                                    self.multifile_flag,
+                                                    self.write_deformed_mesh,
+                                                    self.write_conditions)
+
+        if self.skin_output or self.num_planes > 0:
+            self.cut_io = KratosMultiphysics.GidIO(self.cut_file_name,
+                                                   self.post_mode,
+                                                   self.multifile_flag,
+                                                   self.write_deformed_mesh,
+                                                   KratosMultiphysics.WriteConditionsFlag.WriteConditionsOnly) # Cuts are conditions, so we always print conditions in the cut ModelPart
+
+    def __get_gidpost_flag(self, param, label, dictionary):
+        '''Parse gidpost settings using an auxiliary dictionary of acceptable values.'''
+
+        keystring = param[label].GetString()
+        try:
+            value = dictionary[keystring]
+        except KeyError:
+            msg = "{0} Error: Unknown value \"{1}\" read for parameter \"{2}\"".format(self.__class__.__name__,value,label)
+            raise Exception(msg)
+
+        return value
+
+    def __initialize_cut_output(self,plane_output_configuration):
+        '''Set up tools used to produce output in skin and cut planes.'''
+
+        self.cut_model_part = ModelPart("CutPart")
+        self.cut_manager = CuttingUtility()
+        self.cut_manager.FindSmallestEdge(self.model_part)
+        self.cut_manager.AddVariablesToCutModelPart(self.model_part,self.cut_model_part)
+        if self.skin_output:
+            self.cut_manager.AddSkinConditions(self.model_part,self.cut_model_part,self.output_surface_index)
+            self.output_surface_index += 1
+
+        for plane_id in range(0,plane_output_configuration.size()):
+
+            cut_data = plane_output_configuration[plane_id]
+            # This part of the input data is validated term by term
+            cut_data.ValidateAndAssignDefaults(self.default_plane_output_data)
+
+            self.__define_output_plane(cut_data)
+
+    def __initialize_list_files(self,additional_frequencies):
+        '''Set up .post.lst files for global and cut results.
+        If we have only one tipe of output (volume or cut), the
+        list file is called <gid_model_name>.post.lst. When we have
+        both types, call the volume one <gid_model_name>.post.lst and
+        the cut one <gid_model_name>_cuts.post.lst.
+        additional_frequencies should contain an array of ints N representing
+        the frequencies of additional list files. If it is not empty and GidIO
+        is configured to print multiple files, extra list files are written,
+        listing one in every N output files.'''
+        # Get a name for the GiD list file
+        # if the model folder is model.gid, the list file should be called
+        # model.post.lst
+        # NOTE (PR): In the followin lines, two variables were removed (path and ext). See 'gid_output_process.py'. They were put only because the functions have two output arguments. We can call just the one we need.
+        folder_name = os.path.split(os.getcwd())[1]
+        model_name = os.path.splitext(folder_name)[0]
+        name_base = model_name
+        name_ext = ".post.lst"
+
+        # Remove 1 from extra frequencies (and remove duplicates)
+        used_frequencies = [1,]
+        extra_frequencies = []
+        for f in additional_frequencies:
+            if f not in used_frequencies:
+                used_frequencies.append(f)
+                extra_frequencies.append(f)
+
+        if self.body_io is not None:
+            list_file = open(name_base+name_ext,"w")
+
+            if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
+                list_file.write("Multiple\n")
+            elif self.multifile_flag == KratosMultiphysics.MultiFileFlag.SingleFile:
+                list_file.write("Single\n")
+
+            self.volume_list_files.append( [1,list_file] )
+
+            if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
+                for freq in extra_frequencies:
+                    list_file_name = "{0}_list_{1}{2}".format(name_base,freq,name_ext)
+                    list_file = open(list_file_name,"w")
+                    list_file.write("Multiple\n")
+
+                    self.volume_list_files.append( [freq,list_file] )
+
+            name_base = "{0}_cuts".format(model_name)
+
+        if self.cut_io is not None:
+
+            list_file = open(name_base+name_ext,"w")
+
+            if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
+                list_file.write("Multiple\n")
+            elif self.multifile_flag == KratosMultiphysics.MultiFileFlag.SingleFile:
+                list_file.write("Single\n")
+
+            self.cut_list_files.append( [1,list_file] )
+
+            if self.multifile_flag == KratosMultiphysics.MultiFileFlag.MultipleFiles:
+                for freq in extra_frequencies:
+                    list_file_name = "{0}_list_{1}{2}".format(name_base,freq,name_ext)
+                    list_file = open(list_file_name,"w")
+                    list_file.write("Multiple\n")
+
+                    self.cut_list_files.append( [freq,list_file] )
+
+    def __define_output_plane(self,cut_data):
+        '''Add a plane to the output plane list.'''
+
+        normal_data = cut_data["normal"]
+        n = Vector(3)
+        n[0] = normal_data[0].GetDouble()
+        n[1] = normal_data[1].GetDouble()
+        n[2] = normal_data[2].GetDouble()
+        # Sanity check on normal
+        norm2 = n[0]*n[0] + n[1]*n[1] + n[2]*n[2]
+        if norm2 < 1e-12:
+            raise Exception("{0} Error: something went wrong in output plane definition: plane {1} has a normal with module 0.".format(self.__class__.__name__,self.output_surface_index))
+
+        point_data = cut_data["point"]
+        p = Vector(3)
+        p[0] = point_data[0].GetDouble()
+        p[1] = point_data[1].GetDouble()
+        p[2] = point_data[2].GetDouble()
+
+        # And finally, define the plane
+        self.output_surface_index += 1
+        self.cut_manager.GenerateCut(   self.model_part,
+                                        self.cut_model_part,
+                                        n,
+                                        p,
+                                        self.output_surface_index,
+                                        0.01)
+
+    def __generate_variable_list_from_input(self,param):
+        '''Parse a list of variables from input.'''
+        # At least verify that the input is a string
+        if not param.IsArray():
+            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
+
+        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
+        return [ KratosMultiphysics.KratosGlobals.GetVariable( param[i].GetString() ) for i in range( 0,param.size() ) ]
+
+    def __generate_flags_list_from_input(self,param):
+        '''Parse a list of variables from input.'''
+        # At least verify that the input is a string
+        if not param.IsArray():
+            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
+
+        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
+        return [ globals()[ param[i].GetString() ] for i in range( 0,param.size() ) ]
+
+    def __write_mesh(self, label):
+
+        if self.body_io is not None:
+            self.body_io.InitializeMesh(label)
+            if self.body_output:
+                self.body_io.WriteMesh(self.model_part.GetMesh())
+            if self.node_output:
+                self.body_io.WriteNodeMesh(self.model_part.GetMesh())
+            self.body_io.FinalizeMesh()
+
+        if self.cut_io is not None:
+            self.cut_io.InitializeMesh(label)
+            self.cut_io.WriteMesh(self.cut_model_part.GetMesh())
+            self.cut_io.FinalizeMesh()
+
+    def __initialize_results(self, label):
+
+        if self.body_io is not None:
+            self.body_io.InitializeResults(label, self.model_part.GetMesh())
+
+        if self.cut_io is not None:
+            self.cut_io.InitializeResults(label,self.cut_model_part.GetMesh())
+
+    def __write_nodal_results(self, label):
+
+        if self.body_io is not None:
+            for variable in self.nodal_variables:
+                self.body_io.WriteNodalResults(variable, self.model_part.GetCommunicator().LocalMesh().Nodes, label, 0)
+
+        if self.cut_io is not None:
+            self.cut_manager.UpdateCutData(self.cut_model_part, self.model_part)
+            for variable in self.nodal_variables:
+                self.cut_io.WriteNodalResults(variable, self.cut_model_part.GetCommunicator().LocalMesh().Nodes, label, 0)
+
+    def __write_gp_results(self, label):
+
+        #if self.body_io is not None:
+        if self.body_output: # Note: if we only print nodes, there are no GaussPoints
+            for variable in self.gauss_point_variables:
+                self.body_io.PrintOnGaussPoints(variable, self.model_part, label)
+
+        # Gauss point results depend on the type of element!
+        # they are not implemented for cuts (which are generic Condition3D)
+
+    def __write_nonhistorical_nodal_results(self, label):
+
+        if self.body_io is not None:
+            for variable in self.nodal_nonhistorical_variables:
+                self.body_io.WriteNodalResultsNonHistorical(variable, self.model_part.Nodes, label)
+
+        if self.cut_io is not None:
+            self.cut_manager.UpdateCutData(self.cut_model_part, self.model_part)
+            for variable in self.nodal_nonhistorical_variables:
+                self.cut_io.WriteNodalResultsNonHistorical(variable, self.cut_model_part.Nodes, label)
+
+    def __write_nodal_flags(self, label):
+        if self.body_io is not None:
+            for flag in range(len(self.nodal_flags)):
+                self.body_io.WriteNodalFlags(self.nodal_flags[flag], self.nodal_flags_names[flag], self.model_part.Nodes, label)
+
+        if self.cut_io is not None:
+            self.cut_manager.UpdateCutData(self.cut_model_part, self.model_part)
+            for flag in range(len(self.nodal_flags)):
+                self.cut_io.WriteNodalFlags(self.nodal_flags[flag], self.nodal_flags_names[flag], self.cut_model_part.Nodes, label)
+
+    def __finalize_results(self):
+
+        if self.body_io is not None:
+            self.body_io.FinalizeResults()
+
+        if self.cut_io is not None:
+            self.cut_io.FinalizeResults()
+
+    def __restart_list_files(self,additional_frequencies):
+
+        self.__remove_list_files()
+
+        self.__initialize_list_files(additional_frequencies)
+
+        if self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostBinary:
+            ext = ".post.bin"
+        elif self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostAscii:
+            ext = ".post.res"
+        elif self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostAsciiZipped:
+            ext = ".post.res"
+        else:
+            return # No support for list_files in this format
+
+
+        # Rebuild List Files from existing problem build
+        file_id   = []
+
+        path = os.getcwd()
+
+        for f in os.listdir(path):
+
+            if(f.endswith(ext)):
+
+                #if f.name = problem_tested_145.post.bin
+                file_parts = f.split('_')  # you get ["problem","tested","145.post.bin"]
+                num_parts  = len(file_parts)
+
+                end_parts  = file_parts[num_parts-1].split(".") # you get ["145","post","bin"]
+                print_id   = end_parts[0] # you get "145"
+
+                if( print_id != "0" ):
+                    file_id.append(int(print_id))
+
+            file_id.sort()
+
+    def __set_multifile_lists(self,multifile_list):
+        for mfilelist in multifile_list:
+            self.multifilelists.append(mfilelist)
+
+        for mfilelist in self.multifilelists:
+            mfilelist.file.write("Multiple\n")
+            mfilelist.index = 1
+
+    def __write_inital_step_in_multifile_lists(self, label):
+        for mfilelist in self.multifilelists:
+
+            if (self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostBinary):
+                text_to_print = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.bin\n"
+                mfilelist.file.write(text_to_print)
+            else:
+                text_to_print1 = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.msh\n"
+                text_to_print2 = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.res\n"
+                mfilelist.file.write(text_to_print1)
+                mfilelist.file.write(text_to_print2)
+            self.Flush(mfilelist.file)
+
+    def __write_multifile_lists(self, label):
+
+        for mfilelist in self.multifilelists:
+            if (label % mfilelist.step) == 0:
+
+                if (self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostBinary):
+                    text_to_print = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.bin\n"
+                    mfilelist.file.write(text_to_print)
+                else:
+                    text_to_print1 = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.msh\n"
+                    text_to_print2 = self.__get_multifile_list_name(mfilelist.name)+"_"+"%.12g"%label+".post.res\n"
+                    mfilelist.file.write(text_to_print1)
+                    mfilelist.file.write(text_to_print2)
+                self.Flush(mfilelist.file)
+
+    @classmethod
+    def __get_multifile_list_name(cls, name):
+        return name
+
+    def __close_multifiles(self):
+        for mfilelist in self.multifilelists:
+            mfilelist.file.close()
+
+    # NOTE (PR): 'Codacy' suggest to change the following method, from a standard method to a 'classmethod' or 'staticmethod' as it does not refer to any of the class attributes
+    @classmethod
+    def __remove_list_files(cls):
+
+        path = os.getcwd()
+
+        # remove previous list files:
+        if(os.path.exists(path) == False):
+            print(" Problem Path do not exists , check the Problem Path selected ")
+        else:
+            filelist = [f for f in os.listdir(os.getcwd()) if f.endswith(".lst")]
+            for f in filelist:
+                if(os.path.exists(f)):
+                    try:
+                        os.remove(f)
+                    except WindowsError:
+                        pass
+
+    def __remove_post_results_files(self, step_label):
+
+        path = os.getcwd()
+
+        if self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostBinary:
+            ext = ".post.bin"
+        elif self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostAscii:
+            ext = ".post.res"
+        elif self.post_mode == KratosMultiphysics.GiDPostMode.GiD_PostAsciiZipped:
+            ext = ".post.res"
+
+        # remove post result files:
+        if(os.path.exists(path) == False):
+            print(" Problem Path do not exists , check the Problem Path selected ")
+        else:
+            filelist = []
+            for f in os.listdir(os.getcwd()):
+                if(f.endswith(ext)):
+
+                    #if f.name = problem_tested_145.post.bin
+                    file_parts = f.split('_')
+                    # you get the parts ["problem","tested","145.post.bin"]
+                    num_parts  = len(file_parts)
+                    # take the last part
+                    end_parts  = file_parts[num_parts-1].split(".")
+                    # you get the parts ["145","post","bin"]
+                    print_id   = end_parts[0]
+                    # you get "145"
+
+                    try:
+                        float(print_id)
+                    except ValueError:
+                        break
+
+                    if( float(print_id) >  float(step_label) ):
+                        filelist.append(f)
+
+            for f in filelist:
+                if(os.path.exists(f)):
+                    try:
+                        os.remove(f)
+                    except WindowsError:
+                        pass
+
+
+class MultifileList(object):
+
+    def __init__(self, name, step):
+        self.index = 0
+        self.step = step
+        self.name = name
+        absolute_path_to_file = os.path.join("_list_" + self.name + "_" + str(step) + ".post.lst")
+        self.file = open(absolute_path_to_file,"w")
```

## KratosMultiphysics/DamApplication/global_joint_stress_utility.py

 * *Ordering differences only*

```diff
@@ -1,27 +1,27 @@
-#importing the Kratos Library
-from KratosMultiphysics import *
-from KratosMultiphysics.StructuralMechanicsApplication import *
-# from KratosMultiphysics.ExternalSolversApplication import *
-from KratosMultiphysics.DamApplication import *
-
-class GlobalJoinStressUtility:
-
-    def __init__(self,model_part):
-
-        # This is an example of input paramerter.
-        params = Parameters("{}")
-        params.AddEmptyValue("pmid0_0").SetDouble(247.67)
-        params.AddEmptyValue("pmid0_1").SetDouble(-368.92)
-        params.AddEmptyValue("pmid0_2").SetDouble(242.6)
-        params.AddEmptyValue("pmid1_0").SetDouble(247.15)
-        params.AddEmptyValue("pmid1_1").SetDouble(-385.15)
-        params.AddEmptyValue("pmid1_2").SetDouble(242.6)
-        params.AddEmptyValue("pmid2_0").SetDouble(313.88)
-        params.AddEmptyValue("pmid2_1").SetDouble(-373.26)
-        params.AddEmptyValue("pmid2_2").SetDouble(242.6)
-
-        self.JointStressUtility = GlobalJointStressUtility(model_part, params)
-
-    def ComputingGlobalStress(self):
-
-        self.JointStressUtility.ComputingGlobalStress()
+#importing the Kratos Library
+from KratosMultiphysics import *
+from KratosMultiphysics.StructuralMechanicsApplication import *
+# from KratosMultiphysics.ExternalSolversApplication import *
+from KratosMultiphysics.DamApplication import *
+
+class GlobalJoinStressUtility:
+
+    def __init__(self,model_part):
+
+        # This is an example of input paramerter.
+        params = Parameters("{}")
+        params.AddEmptyValue("pmid0_0").SetDouble(247.67)
+        params.AddEmptyValue("pmid0_1").SetDouble(-368.92)
+        params.AddEmptyValue("pmid0_2").SetDouble(242.6)
+        params.AddEmptyValue("pmid1_0").SetDouble(247.15)
+        params.AddEmptyValue("pmid1_1").SetDouble(-385.15)
+        params.AddEmptyValue("pmid1_2").SetDouble(242.6)
+        params.AddEmptyValue("pmid2_0").SetDouble(313.88)
+        params.AddEmptyValue("pmid2_1").SetDouble(-373.26)
+        params.AddEmptyValue("pmid2_2").SetDouble(242.6)
+
+        self.JointStressUtility = GlobalJointStressUtility(model_part, params)
+
+    def ComputingGlobalStress(self):
+
+        self.JointStressUtility.ComputingGlobalStress()
```

## KratosMultiphysics/DamApplication/impose_2d_random_fields_variable_process.py

 * *Ordering differences only*

```diff
@@ -1,71 +1,71 @@
-import KratosMultiphysics
-import KratosMultiphysics.DamApplication as KratosDam
-
-try:
-    from gstools import SRF, Gaussian
-except ImportError:
-    raise ImportError("The use of the random fields module requires 'gstools'!")
-
-from statistics import mean, variance
-from math import sqrt
-
-def Factory(settings, Model):
-    if(not isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return Impose2dRandomFieldsVariableProcess(Model, settings["Parameters"])
-
-class Impose2dRandomFieldsVariableProcess(KratosMultiphysics.Process):
-    def __init__(self, Model, settings ):
-
-        KratosMultiphysics.Process.__init__(self)
-        model_part = Model[settings["model_part_name"].GetString()]
-        mean_value = settings["mean_value"].GetDouble()
-        min_value = settings["min_value"].GetDouble()
-        max_value = settings["max_value"].GetDouble()
-        var = settings["variance"].GetDouble()
-        corr_length = settings["corr_length"].GetInt()
-
-        # Gaussian random field with exponential covariance
-        model = Gaussian(dim = 2, var = var, len_scale = corr_length)
-        srf = SRF(model)
-
-        x = []
-        y = []
-        ids = []
-
-        for node in model_part.Nodes:
-            x.append(node.X)
-            y.append(node.Y)
-            ids.append(node.Id)
-
-        field = srf((x, y))
-
-        field_mean = mean(field)
-        field_var = variance(field, field_mean)
-
-        variable_values = []
-
-        for field_i in field:
-            variable_values.append(mean_value + ((field_i-field_mean)*var/sqrt(field_var)))
-
-        ### Truncate values
-        for variable_value in variable_values:
-            if variable_value < min_value:
-                variable_value = min_value
-            if variable_value > max_value:
-                variable_value = max_value
-
-        self.table = KratosMultiphysics.PiecewiseLinearTable()
-
-        for i in range(len(variable_values)):
-            self.table.AddRow(int(ids[i]), float(variable_values[i]))
-
-        self.process = KratosDam.DamRandomFieldsVariableProcess(model_part, self.table, settings)
-
-    def ExecuteInitialize(self):
-
-        self.process.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        self.process.ExecuteInitializeSolutionStep()
+import KratosMultiphysics
+import KratosMultiphysics.DamApplication as KratosDam
+
+try:
+    from gstools import SRF, Gaussian
+except ImportError:
+    raise ImportError("The use of the random fields module requires 'gstools'!")
+
+from statistics import mean, variance
+from math import sqrt
+
+def Factory(settings, Model):
+    if(not isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return Impose2dRandomFieldsVariableProcess(Model, settings["Parameters"])
+
+class Impose2dRandomFieldsVariableProcess(KratosMultiphysics.Process):
+    def __init__(self, Model, settings ):
+
+        KratosMultiphysics.Process.__init__(self)
+        model_part = Model[settings["model_part_name"].GetString()]
+        mean_value = settings["mean_value"].GetDouble()
+        min_value = settings["min_value"].GetDouble()
+        max_value = settings["max_value"].GetDouble()
+        var = settings["variance"].GetDouble()
+        corr_length = settings["corr_length"].GetInt()
+
+        # Gaussian random field with exponential covariance
+        model = Gaussian(dim = 2, var = var, len_scale = corr_length)
+        srf = SRF(model)
+
+        x = []
+        y = []
+        ids = []
+
+        for node in model_part.Nodes:
+            x.append(node.X)
+            y.append(node.Y)
+            ids.append(node.Id)
+
+        field = srf((x, y))
+
+        field_mean = mean(field)
+        field_var = variance(field, field_mean)
+
+        variable_values = []
+
+        for field_i in field:
+            variable_values.append(mean_value + ((field_i-field_mean)*var/sqrt(field_var)))
+
+        ### Truncate values
+        for variable_value in variable_values:
+            if variable_value < min_value:
+                variable_value = min_value
+            if variable_value > max_value:
+                variable_value = max_value
+
+        self.table = KratosMultiphysics.PiecewiseLinearTable()
+
+        for i in range(len(variable_values)):
+            self.table.AddRow(int(ids[i]), float(variable_values[i]))
+
+        self.process = KratosDam.DamRandomFieldsVariableProcess(model_part, self.table, settings)
+
+    def ExecuteInitialize(self):
+
+        self.process.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        self.process.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_3d_random_fields_variable_process.py

 * *Ordering differences only*

```diff
@@ -1,74 +1,74 @@
-import KratosMultiphysics
-import KratosMultiphysics.DamApplication as KratosDam
-
-try:
-    from gstools import SRF, Gaussian
-except ImportError:
-    raise ImportError("The use of the random fields module requires 'gstools'!")
-
-from statistics import mean, variance
-from math import sqrt
-
-def Factory(settings, Model):
-    if(not isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return Impose3dRandomFieldsVariableProcess(Model, settings["Parameters"])
-
-class Impose3dRandomFieldsVariableProcess(KratosMultiphysics.Process):
-    def __init__(self, Model, settings ):
-
-        KratosMultiphysics.Process.__init__(self)
-        model_part = Model[settings["model_part_name"].GetString()]
-        mean_value = settings["mean_value"].GetDouble()
-        min_value = settings["min_value"].GetDouble()
-        max_value = settings["max_value"].GetDouble()
-        var = settings["variance"].GetDouble()
-        corr_length = settings["corr_length"].GetInt()
-
-        # Gaussian random field with exponential covariance
-        model = Gaussian(dim = 3, var = var, len_scale = corr_length)
-        srf = SRF(model)
-
-        x = []
-        y = []
-        z = []
-        ids = []
-
-        for node in model_part.Nodes:
-            x.append(node.X)
-            y.append(node.Y)
-            z.append(node.Z)
-            ids.append(node.Id)
-
-        field = srf((x, y, z))
-
-        field_mean = mean(field)
-        field_var = variance(field, field_mean)
-
-        variable_values = []
-
-        for field_i in field:
-            variable_values.append(mean_value + ((field_i-field_mean)*var/sqrt(field_var)))
-
-        ### Truncate values
-        for variable_value in variable_values:
-            if variable_value < min_value:
-                variable_value = min_value
-            if variable_value > max_value:
-                variable_value = max_value
-
-        self.table = KratosMultiphysics.PiecewiseLinearTable()
-
-        for i in range(len(variable_values)):
-            self.table.AddRow(int(ids[i]), float(variable_values[i]))
-
-        self.process = KratosDam.DamRandomFieldsVariableProcess(model_part, self.table, settings)
-
-
-    def ExecuteInitialize(self):
-
-        self.process.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        self.process.ExecuteInitializeSolutionStep()
+import KratosMultiphysics
+import KratosMultiphysics.DamApplication as KratosDam
+
+try:
+    from gstools import SRF, Gaussian
+except ImportError:
+    raise ImportError("The use of the random fields module requires 'gstools'!")
+
+from statistics import mean, variance
+from math import sqrt
+
+def Factory(settings, Model):
+    if(not isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return Impose3dRandomFieldsVariableProcess(Model, settings["Parameters"])
+
+class Impose3dRandomFieldsVariableProcess(KratosMultiphysics.Process):
+    def __init__(self, Model, settings ):
+
+        KratosMultiphysics.Process.__init__(self)
+        model_part = Model[settings["model_part_name"].GetString()]
+        mean_value = settings["mean_value"].GetDouble()
+        min_value = settings["min_value"].GetDouble()
+        max_value = settings["max_value"].GetDouble()
+        var = settings["variance"].GetDouble()
+        corr_length = settings["corr_length"].GetInt()
+
+        # Gaussian random field with exponential covariance
+        model = Gaussian(dim = 3, var = var, len_scale = corr_length)
+        srf = SRF(model)
+
+        x = []
+        y = []
+        z = []
+        ids = []
+
+        for node in model_part.Nodes:
+            x.append(node.X)
+            y.append(node.Y)
+            z.append(node.Z)
+            ids.append(node.Id)
+
+        field = srf((x, y, z))
+
+        field_mean = mean(field)
+        field_var = variance(field, field_mean)
+
+        variable_values = []
+
+        for field_i in field:
+            variable_values.append(mean_value + ((field_i-field_mean)*var/sqrt(field_var)))
+
+        ### Truncate values
+        for variable_value in variable_values:
+            if variable_value < min_value:
+                variable_value = min_value
+            if variable_value > max_value:
+                variable_value = max_value
+
+        self.table = KratosMultiphysics.PiecewiseLinearTable()
+
+        for i in range(len(variable_values)):
+            self.table.AddRow(int(ids[i]), float(variable_values[i]))
+
+        self.process = KratosDam.DamRandomFieldsVariableProcess(model_part, self.table, settings)
+
+
+    def ExecuteInitialize(self):
+
+        self.process.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        self.process.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_chemo_mechanical_aging_process.py

 * *Ordering differences only*

```diff
@@ -1,23 +1,23 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-## In this case, the scalar value is automatically fixed.
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeChemoMechanicalAgingProcess(Model, settings["Parameters"])
-
-class ImposeChemoMechanicalAgingProcess(Process):
-
-    def __init__(self, Model, settings ):
-
-        Process.__init__(self)
-        model_part = Model[settings["model_part_name"].GetString()]
-        self.process = DamChemoMechanicalAgingYoungProcess(model_part, settings)
-
-    def ExecuteInitialize(self):
-        self.process.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-        self.process.ExecuteInitializeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+## In this case, the scalar value is automatically fixed.
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeChemoMechanicalAgingProcess(Model, settings["Parameters"])
+
+class ImposeChemoMechanicalAgingProcess(Process):
+
+    def __init__(self, Model, settings ):
+
+        Process.__init__(self)
+        model_part = Model[settings["model_part_name"].GetString()]
+        self.process = DamChemoMechanicalAgingYoungProcess(model_part, settings)
+
+    def ExecuteInitialize(self):
+        self.process.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+        self.process.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_face_heat_flux_process.py

 * *Ordering differences only*

```diff
@@ -1,56 +1,56 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-## In this case, the scalar value is automatically fixed.
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeFaceHeatFluxProcess(Model, settings["Parameters"])
-
-class ImposeFaceHeatFluxProcess(Process):
-
-    def __init__(self, Model, settings ):
-
-        Process.__init__(self)
-        model_part = Model[settings["model_part_name"].GetString()]
-        self.components_process_list = []
-
-        ## This process assign and uniform heat flux
-        if ("UniformFlux2D" in settings["model_part_name"].GetString()) or ("UniformFlux3D" in settings["model_part_name"].GetString()):
-            if settings["table"].GetInt() == 0:
-                t_uniform = Parameters("{}")
-                t_uniform.AddValue("model_part_name",settings["model_part_name"])
-                t_uniform.AddEmptyValue("is_fixed").SetBool(False)
-                t_uniform.AddValue("variable_name",settings["variable_name"])
-                t_uniform.AddValue("value",settings["value"])
-                self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, t_uniform))
-            else:
-                self.components_process_list.append(DamFixTemperatureConditionProcess(model_part, settings))
-
-        ## This process compute the heat flux according to q = h(t_ambient - t_current).
-        ## Setting the extra values to 0.0 it is possible to use the same process.
-        if ("TAmbientFlux2D" in settings["model_part_name"].GetString()) or ("TAmbientFlux3D" in settings["model_part_name"].GetString()):
-            t_ambient = Parameters("{}")
-            t_ambient.AddValue("model_part_name",settings["model_part_name"])
-            t_ambient.AddValue("variable_name",settings["variable_name"])
-            t_ambient.AddValue("h_0",settings["h_0"])
-            t_ambient.AddValue("ambient_temperature",settings["ambient_temperature"])
-            t_ambient.AddValue("table_ambient_temperature",settings["table_ambient_temperature"])
-            t_ambient.AddEmptyValue("emisivity").SetDouble(0.0)
-            t_ambient.AddEmptyValue("delta_R").SetDouble(0.0)
-            t_ambient.AddEmptyValue("absorption_index").SetDouble(0.0)
-            t_ambient.AddEmptyValue("total_insolation").SetDouble(0.0)
-            self.components_process_list.append(DamTSolAirHeatFluxProcess(model_part, t_ambient))
-
-        ## This process compute the heat flux according to q = h(t_sol_air - t_current)
-        if ("TSolAirFluxCondition2D" in settings["model_part_name"].GetString()) or ("TSolAirFluxCondition3D" in settings["model_part_name"].GetString()):
-            self.components_process_list.append(DamTSolAirHeatFluxProcess(model_part, settings))
-
-    def ExecuteInitialize(self):
-        for component in self.components_process_list:
-            component.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-        for component in self.components_process_list:
-            component.ExecuteInitializeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+## In this case, the scalar value is automatically fixed.
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeFaceHeatFluxProcess(Model, settings["Parameters"])
+
+class ImposeFaceHeatFluxProcess(Process):
+
+    def __init__(self, Model, settings ):
+
+        Process.__init__(self)
+        model_part = Model[settings["model_part_name"].GetString()]
+        self.components_process_list = []
+
+        ## This process assign and uniform heat flux
+        if ("UniformFlux2D" in settings["model_part_name"].GetString()) or ("UniformFlux3D" in settings["model_part_name"].GetString()):
+            if settings["table"].GetInt() == 0:
+                t_uniform = Parameters("{}")
+                t_uniform.AddValue("model_part_name",settings["model_part_name"])
+                t_uniform.AddEmptyValue("is_fixed").SetBool(False)
+                t_uniform.AddValue("variable_name",settings["variable_name"])
+                t_uniform.AddValue("value",settings["value"])
+                self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, t_uniform))
+            else:
+                self.components_process_list.append(DamFixTemperatureConditionProcess(model_part, settings))
+
+        ## This process compute the heat flux according to q = h(t_ambient - t_current).
+        ## Setting the extra values to 0.0 it is possible to use the same process.
+        if ("TAmbientFlux2D" in settings["model_part_name"].GetString()) or ("TAmbientFlux3D" in settings["model_part_name"].GetString()):
+            t_ambient = Parameters("{}")
+            t_ambient.AddValue("model_part_name",settings["model_part_name"])
+            t_ambient.AddValue("variable_name",settings["variable_name"])
+            t_ambient.AddValue("h_0",settings["h_0"])
+            t_ambient.AddValue("ambient_temperature",settings["ambient_temperature"])
+            t_ambient.AddValue("table_ambient_temperature",settings["table_ambient_temperature"])
+            t_ambient.AddEmptyValue("emisivity").SetDouble(0.0)
+            t_ambient.AddEmptyValue("delta_R").SetDouble(0.0)
+            t_ambient.AddEmptyValue("absorption_index").SetDouble(0.0)
+            t_ambient.AddEmptyValue("total_insolation").SetDouble(0.0)
+            self.components_process_list.append(DamTSolAirHeatFluxProcess(model_part, t_ambient))
+
+        ## This process compute the heat flux according to q = h(t_sol_air - t_current)
+        if ("TSolAirFluxCondition2D" in settings["model_part_name"].GetString()) or ("TSolAirFluxCondition3D" in settings["model_part_name"].GetString()):
+            self.components_process_list.append(DamTSolAirHeatFluxProcess(model_part, settings))
+
+    def ExecuteInitialize(self):
+        for component in self.components_process_list:
+            component.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+        for component in self.components_process_list:
+            component.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_grouting_reference_temperature_process.py

 * *Ordering differences only*

```diff
@@ -1,25 +1,25 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-def Factory(settings, Model):
-    if(not isinstance(settings,Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeGroutingReferenceTemperatureProcess(Model, settings["Parameters"])
-
-class ImposeGroutingReferenceTemperatureProcess(Process):
-    def __init__(self, Model, settings ):
-
-        Process.__init__(self)
-        model_part = Model[settings["model_part_name"].GetString()]
-
-        self.process = DamGroutingReferenceTemperatureProcess(model_part, settings)
-
-
-    def ExecuteInitialize(self):
-        self.process.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-        pass
-
-    def ExecuteFinalizeSolutionStep(self):
-        self.process.ExecuteFinalizeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+def Factory(settings, Model):
+    if(not isinstance(settings,Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeGroutingReferenceTemperatureProcess(Model, settings["Parameters"])
+
+class ImposeGroutingReferenceTemperatureProcess(Process):
+    def __init__(self, Model, settings ):
+
+        Process.__init__(self)
+        model_part = Model[settings["model_part_name"].GetString()]
+
+        self.process = DamGroutingReferenceTemperatureProcess(model_part, settings)
+
+
+    def ExecuteInitialize(self):
+        self.process.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+        pass
+
+    def ExecuteFinalizeSolutionStep(self):
+        self.process.ExecuteFinalizeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_heat_source_process.py

 * *Ordering differences only*

```diff
@@ -1,34 +1,34 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-## This proces sets the value of water loads.
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeHeatSourceProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class ImposeHeatSourceProcess(Process):
-    def __init__(self, Model, settings ):
-        Process.__init__(self)
-
-        model_part = Model[settings["model_part_name"].GetString()]
-
-        self.components_process_list = []
-
-        if ("NoorzaiHeatFlux2D" in settings["model_part_name"].GetString()) or ("NoorzaiHeatFlux3D" in settings["model_part_name"].GetString()):
-            self.components_process_list.append(DamNoorzaiHeatFluxProcess(model_part, settings))
-
-        if ("AzenhaHeatFlux2D" in settings["model_part_name"].GetString()) or ("AzenhaHeatFlux3D" in settings["model_part_name"].GetString()):
-            self.components_process_list.append(DamAzenhaHeatFluxProcess(model_part, settings))
-
-    def ExecuteInitialize(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitializeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+## This proces sets the value of water loads.
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeHeatSourceProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class ImposeHeatSourceProcess(Process):
+    def __init__(self, Model, settings ):
+        Process.__init__(self)
+
+        model_part = Model[settings["model_part_name"].GetString()]
+
+        self.components_process_list = []
+
+        if ("NoorzaiHeatFlux2D" in settings["model_part_name"].GetString()) or ("NoorzaiHeatFlux3D" in settings["model_part_name"].GetString()):
+            self.components_process_list.append(DamNoorzaiHeatFluxProcess(model_part, settings))
+
+        if ("AzenhaHeatFlux2D" in settings["model_part_name"].GetString()) or ("AzenhaHeatFlux3D" in settings["model_part_name"].GetString()):
+            self.components_process_list.append(DamAzenhaHeatFluxProcess(model_part, settings))
+
+    def ExecuteInitialize(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_input_table_nodal_young_modulus_process.py

 * *Ordering differences only*

```diff
@@ -1,45 +1,45 @@
-import KratosMultiphysics
-import KratosMultiphysics.DamApplication as KratosDam
-
-def Factory(settings, Model):
-    if(not isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeInputTableNodalYoungModulusProcess(Model, settings["Parameters"])
-
-class ImposeInputTableNodalYoungModulusProcess(KratosMultiphysics.Process):
-    def __init__(self, Model, settings ):
-
-        KratosMultiphysics.Process.__init__(self)
-        model_part = Model[settings["model_part_name"].GetString()]
-        settings.RemoveValue("min_value")
-        settings.RemoveValue("max_value")
-
-        # Checks if the parameter "input_file_name" exixts. If not, it create it and define it as "".
-        # This may be changed in the future, when the Nodal Reference Temp (input file) process will be fixed.
-
-        if settings.Has("input_file_name"):
-            input_file_name = settings["input_file_name"].GetString()
-        else:
-            input_file_name = ""
-
-        if ((input_file_name == "") or (input_file_name == "- No file") or (input_file_name == "- Add new file")):
-            self.table = KratosMultiphysics.PiecewiseLinearTable()
-        else:
-            self.table = KratosMultiphysics.PiecewiseLinearTable()
-
-            with open(input_file_name, 'r') as file_name:
-                for line in file_name:
-                    line_list = line.split(" ")
-                    if (len(line_list)) > 1:
-                        self.table.AddRow(float(line_list[0]), float(line_list[1]))
-
-        self.process = KratosDam.DamInputTableNodalYoungModulusProcess(model_part, self.table, settings)
-
-
-    def ExecuteInitialize(self):
-
-        self.process.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        self.process.ExecuteInitializeSolutionStep()
+import KratosMultiphysics
+import KratosMultiphysics.DamApplication as KratosDam
+
+def Factory(settings, Model):
+    if(not isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeInputTableNodalYoungModulusProcess(Model, settings["Parameters"])
+
+class ImposeInputTableNodalYoungModulusProcess(KratosMultiphysics.Process):
+    def __init__(self, Model, settings ):
+
+        KratosMultiphysics.Process.__init__(self)
+        model_part = Model[settings["model_part_name"].GetString()]
+        settings.RemoveValue("min_value")
+        settings.RemoveValue("max_value")
+
+        # Checks if the parameter "input_file_name" exixts. If not, it create it and define it as "".
+        # This may be changed in the future, when the Nodal Reference Temp (input file) process will be fixed.
+
+        if settings.Has("input_file_name"):
+            input_file_name = settings["input_file_name"].GetString()
+        else:
+            input_file_name = ""
+
+        if ((input_file_name == "") or (input_file_name == "- No file") or (input_file_name == "- Add new file")):
+            self.table = KratosMultiphysics.PiecewiseLinearTable()
+        else:
+            self.table = KratosMultiphysics.PiecewiseLinearTable()
+
+            with open(input_file_name, 'r') as file_name:
+                for line in file_name:
+                    line_list = line.split(" ")
+                    if (len(line_list)) > 1:
+                        self.table.AddRow(float(line_list[0]), float(line_list[1]))
+
+        self.process = KratosDam.DamInputTableNodalYoungModulusProcess(model_part, self.table, settings)
+
+
+    def ExecuteInitialize(self):
+
+        self.process.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        self.process.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_nodal_reference_temperature_process.py

 * *Ordering differences only*

```diff
@@ -1,46 +1,46 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-
-
-def Factory(settings, Model):
-    if(not isinstance(settings,Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeNodalReferenceTemperatureProcess(Model, settings["Parameters"])
-
-class ImposeNodalReferenceTemperatureProcess(Process):
-    def __init__(self, Model, settings ):
-
-        Process.__init__(self)
-        model_part = Model[settings["model_part_name"].GetString()]
-        variable_name = settings["variable_name"].GetString()
-        initial_value = settings["initial_value"].GetDouble()
-
-        # Checks if the parameter "input_file_name" exixts. If not, it create it and define it as "".
-        # This may be changed in the future, when the Nodal Reference Temp (input file) process will be fixed.
-
-        if settings.Has("input_file_name"):
-            input_file_name = settings["input_file_name"].GetString()
-        else:
-            input_file_name = ""
-
-        if ((input_file_name == "") or ("- No file" in input_file_name) or ("- Add new file" in input_file_name)):
-            self.table = PiecewiseLinearTable()
-        else:
-            self.table = PiecewiseLinearTable()
-            with open(input_file_name,'r') as file_name:
-                for j, line in enumerate(file_name):
-                    file_1 = line.split(" ")
-                    if (len(file_1)) > 1:
-                        self.table.AddRow(float(file_1[0]), float(file_1[1]))
-
-        self.process = DamNodalReferenceTemperatureProcess(model_part, self.table, settings)
-
-
-    def ExecuteInitialize(self):
-
-        self.process.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        self.process.ExecuteInitializeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+
+
+def Factory(settings, Model):
+    if(not isinstance(settings,Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeNodalReferenceTemperatureProcess(Model, settings["Parameters"])
+
+class ImposeNodalReferenceTemperatureProcess(Process):
+    def __init__(self, Model, settings ):
+
+        Process.__init__(self)
+        model_part = Model[settings["model_part_name"].GetString()]
+        variable_name = settings["variable_name"].GetString()
+        initial_value = settings["initial_value"].GetDouble()
+
+        # Checks if the parameter "input_file_name" exixts. If not, it create it and define it as "".
+        # This may be changed in the future, when the Nodal Reference Temp (input file) process will be fixed.
+
+        if settings.Has("input_file_name"):
+            input_file_name = settings["input_file_name"].GetString()
+        else:
+            input_file_name = ""
+
+        if ((input_file_name == "") or ("- No file" in input_file_name) or ("- Add new file" in input_file_name)):
+            self.table = PiecewiseLinearTable()
+        else:
+            self.table = PiecewiseLinearTable()
+            with open(input_file_name,'r') as file_name:
+                for j, line in enumerate(file_name):
+                    file_1 = line.split(" ")
+                    if (len(file_1)) > 1:
+                        self.table.AddRow(float(file_1[0]), float(file_1[1]))
+
+        self.process = DamNodalReferenceTemperatureProcess(model_part, self.table, settings)
+
+
+    def ExecuteInitialize(self):
+
+        self.process.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        self.process.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_nodal_young_modulus_process.py

 * *Ordering differences only*

```diff
@@ -1,28 +1,28 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-## In this case, the scalar value is automatically fixed.
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeNodalYoungModulusProcess(Model, settings["Parameters"])
-
-class ImposeNodalYoungModulusProcess(Process):
-
-    def __init__(self, Model, settings ):
-
-        Process.__init__(self)
-        model_part = Model[settings["model_part_name"].GetString()]
-        settings.AddEmptyValue("is_fixed").SetBool(True)
-
-        self.process = DamNodalYoungModulusProcess(model_part, settings)
-
-
-    def ExecuteInitialize(self):
-
-        self.process.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        self.process.ExecuteInitializeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+## In this case, the scalar value is automatically fixed.
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeNodalYoungModulusProcess(Model, settings["Parameters"])
+
+class ImposeNodalYoungModulusProcess(Process):
+
+    def __init__(self, Model, settings ):
+
+        Process.__init__(self)
+        model_part = Model[settings["model_part_name"].GetString()]
+        settings.AddEmptyValue("is_fixed").SetBool(True)
+
+        self.process = DamNodalYoungModulusProcess(model_part, settings)
+
+
+    def ExecuteInitialize(self):
+
+        self.process.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        self.process.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_reservoir_temperature_condition_process.py

 * *Ordering differences only*

```diff
@@ -1,45 +1,45 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-## This proces sets the value of a scalar variable using the BofangConditionTemperatureProcess.
-## In this case, the scalar value is automatically fixed.
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeReservoirTemperatureConditionProcess(Model, settings["Parameters"])
-
-class ImposeReservoirTemperatureConditionProcess(Process):
-
-    def __init__(self, Model, settings ):
-
-        Process.__init__(self)
-        model_part = Model[settings["model_part_name"].GetString()]
-
-        settings.AddEmptyValue("is_fixed").SetBool(True)
-
-        self.components_process_list = []
-
-        if "BOFANGTEMPERATURE" in settings["model_part_name"].GetString():
-            self.components_process_list.append(DamBofangConditionTemperatureProcess(model_part, settings))
-
-        if "CONSTANTRESERVOIRTEMPERATURE" in settings["model_part_name"].GetString():
-            self.components_process_list.append(DamReservoirConstantTemperatureProcess(model_part, settings))
-
-        if "MONITORINGRESERVOIRTEMPERATURE" in settings["model_part_name"].GetString():
-            self.components_process_list.append(DamReservoirMonitoringTemperatureProcess(model_part, settings))
-
-    def ExecuteInitialize(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitializeSolutionStep()
-
-    def ExecuteFinalizeSolutionStep(self):
-
-        for component in self.components_process_list:
-            component.ExecuteFinalizeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+## This proces sets the value of a scalar variable using the BofangConditionTemperatureProcess.
+## In this case, the scalar value is automatically fixed.
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeReservoirTemperatureConditionProcess(Model, settings["Parameters"])
+
+class ImposeReservoirTemperatureConditionProcess(Process):
+
+    def __init__(self, Model, settings ):
+
+        Process.__init__(self)
+        model_part = Model[settings["model_part_name"].GetString()]
+
+        settings.AddEmptyValue("is_fixed").SetBool(True)
+
+        self.components_process_list = []
+
+        if "BOFANGTEMPERATURE" in settings["model_part_name"].GetString():
+            self.components_process_list.append(DamBofangConditionTemperatureProcess(model_part, settings))
+
+        if "CONSTANTRESERVOIRTEMPERATURE" in settings["model_part_name"].GetString():
+            self.components_process_list.append(DamReservoirConstantTemperatureProcess(model_part, settings))
+
+        if "MONITORINGRESERVOIRTEMPERATURE" in settings["model_part_name"].GetString():
+            self.components_process_list.append(DamReservoirMonitoringTemperatureProcess(model_part, settings))
+
+    def ExecuteInitialize(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitializeSolutionStep()
+
+    def ExecuteFinalizeSolutionStep(self):
+
+        for component in self.components_process_list:
+            component.ExecuteFinalizeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_temperature_by_device_process.py

 * *Ordering differences only*

```diff
@@ -1,21 +1,21 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeTemperaturebyDeviceProcess(Model, settings["Parameters"])
-
-class ImposeTemperaturebyDeviceProcess(Process):
-
-    def __init__(self, Model, settings ):
-
-        Process.__init__(self)
-        model_part = Model[settings["model_part_name"].GetString()]
-
-        self.process = DamTemperaturebyDeviceProcess(model_part, settings)
-
-    def ExecuteInitializeSolutionStep(self):
-
-        self.process.ExecuteInitializeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeTemperaturebyDeviceProcess(Model, settings["Parameters"])
+
+class ImposeTemperaturebyDeviceProcess(Process):
+
+    def __init__(self, Model, settings ):
+
+        Process.__init__(self)
+        model_part = Model[settings["model_part_name"].GetString()]
+
+        self.process = DamTemperaturebyDeviceProcess(model_part, settings)
+
+    def ExecuteInitializeSolutionStep(self):
+
+        self.process.ExecuteInitializeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_thermal_parameters_scalar_value_process.py

 * *Ordering differences only*

```diff
@@ -1,57 +1,57 @@
-from KratosMultiphysics import *
-
-## This proces sets the value several scalar variables corresponding to the thermal problem using the ApplyConstantScalarValueProcess.
-## In this case, the scalar value is automatically fixed.
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeThemalParametersScalarValueProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class ImposeThemalParametersScalarValueProcess(Process):
-    def __init__(self, Model, settings ):
-        Process.__init__(self)
-
-        model_part = Model[settings["model_part_name"].GetString()]
-
-        self.components_process_list = []
-
-        if settings["ThermalDensity"].GetDouble() != 0:
-
-            thermal_density = Parameters("{}")
-            thermal_density.AddValue("model_part_name", settings["model_part_name"])
-            thermal_density.AddValue("value", settings["ThermalDensity"])
-            thermal_density.AddEmptyValue("variable_name").SetString("DENSITY")
-
-            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, thermal_density))
-
-        if settings["Conductivity"].GetDouble() != 0:
-
-            conductivity = Parameters("{}")
-            conductivity.AddValue("model_part_name", settings["model_part_name"])
-            conductivity.AddValue("value", settings["Conductivity"])
-            conductivity.AddEmptyValue("variable_name").SetString("CONDUCTIVITY")
-
-            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, conductivity))
-
-        if settings["SpecificHeat"].GetDouble() != 0:
-
-            specific_heat = Parameters("{}")
-            specific_heat.AddValue("model_part_name", settings["model_part_name"])
-            specific_heat.AddValue("value", settings["SpecificHeat"])
-            specific_heat.AddEmptyValue("variable_name").SetString("SPECIFIC_HEAT")
-
-            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, specific_heat))
-
-
-    def ExecuteInitialize(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitializeSolutionStep()
-
+from KratosMultiphysics import *
+
+## This proces sets the value several scalar variables corresponding to the thermal problem using the ApplyConstantScalarValueProcess.
+## In this case, the scalar value is automatically fixed.
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeThemalParametersScalarValueProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class ImposeThemalParametersScalarValueProcess(Process):
+    def __init__(self, Model, settings ):
+        Process.__init__(self)
+
+        model_part = Model[settings["model_part_name"].GetString()]
+
+        self.components_process_list = []
+
+        if settings["ThermalDensity"].GetDouble() != 0:
+
+            thermal_density = Parameters("{}")
+            thermal_density.AddValue("model_part_name", settings["model_part_name"])
+            thermal_density.AddValue("value", settings["ThermalDensity"])
+            thermal_density.AddEmptyValue("variable_name").SetString("DENSITY")
+
+            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, thermal_density))
+
+        if settings["Conductivity"].GetDouble() != 0:
+
+            conductivity = Parameters("{}")
+            conductivity.AddValue("model_part_name", settings["model_part_name"])
+            conductivity.AddValue("value", settings["Conductivity"])
+            conductivity.AddEmptyValue("variable_name").SetString("CONDUCTIVITY")
+
+            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, conductivity))
+
+        if settings["SpecificHeat"].GetDouble() != 0:
+
+            specific_heat = Parameters("{}")
+            specific_heat.AddValue("model_part_name", settings["model_part_name"])
+            specific_heat.AddValue("value", settings["SpecificHeat"])
+            specific_heat.AddEmptyValue("variable_name").SetString("SPECIFIC_HEAT")
+
+            self.components_process_list.append(ApplyConstantScalarValueProcess(model_part, specific_heat))
+
+
+    def ExecuteInitialize(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitializeSolutionStep()
+
```

## KratosMultiphysics/DamApplication/impose_uniform_temperature_process.py

 * *Ordering differences only*

```diff
@@ -1,39 +1,39 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-## This proces sets the value of a scalar variable using the ApplyConstantScalarValueProcess.
-## In this case, the scalar value is not automatically fixed, so the fixicity must be introduced before.
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeUniformTemperatureProcess(Model, settings["Parameters"])
-
-class ImposeUniformTemperatureProcess(Process):
-
-    def __init__(self, Model, settings ):
-
-        Process.__init__(self)
-        model_part = Model[settings["model_part_name"].GetString()]
-
-        if settings["table"].GetInt() == 0:
-            param = Parameters("{}")
-            param.AddValue("model_part_name",settings["model_part_name"])
-            param.AddValue("is_fixed",settings["is_fixed"])
-            param.AddValue("variable_name",settings["variable_name"])
-            param.AddValue("value",settings["value"])
-            if settings["is_fixed"].GetBool():
-                self.process = DamFixTemperatureConditionProcess(model_part, settings)
-            else:
-                self.process = ApplyConstantScalarValueProcess(model_part, param)
-        else:
-            self.process = DamFixTemperatureConditionProcess(model_part, settings)
-
-    def ExecuteInitialize(self):
-        self.process.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-        self.process.ExecuteInitializeSolutionStep()
-
-    def ExecuteFinalizeSolutionStep(self):
-        self.process.ExecuteFinalizeSolutionStep()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+## This proces sets the value of a scalar variable using the ApplyConstantScalarValueProcess.
+## In this case, the scalar value is not automatically fixed, so the fixicity must be introduced before.
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeUniformTemperatureProcess(Model, settings["Parameters"])
+
+class ImposeUniformTemperatureProcess(Process):
+
+    def __init__(self, Model, settings ):
+
+        Process.__init__(self)
+        model_part = Model[settings["model_part_name"].GetString()]
+
+        if settings["table"].GetInt() == 0:
+            param = Parameters("{}")
+            param.AddValue("model_part_name",settings["model_part_name"])
+            param.AddValue("is_fixed",settings["is_fixed"])
+            param.AddValue("variable_name",settings["variable_name"])
+            param.AddValue("value",settings["value"])
+            if settings["is_fixed"].GetBool():
+                self.process = DamFixTemperatureConditionProcess(model_part, settings)
+            else:
+                self.process = ApplyConstantScalarValueProcess(model_part, param)
+        else:
+            self.process = DamFixTemperatureConditionProcess(model_part, settings)
+
+    def ExecuteInitialize(self):
+        self.process.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+        self.process.ExecuteInitializeSolutionStep()
+
+    def ExecuteFinalizeSolutionStep(self):
+        self.process.ExecuteFinalizeSolutionStep()
```

## KratosMultiphysics/DamApplication/impose_water_loads_condition_process.py

 * *Ordering differences only*

```diff
@@ -1,48 +1,48 @@
-import KratosMultiphysics
-import KratosMultiphysics.DamApplication as KratosDam
-
-## This proces sets the value of water loads.
-
-def Factory(settings, Model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ImposeWaterLoadsConditionProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class ImposeWaterLoadsConditionProcess(KratosMultiphysics.Process):
-    def __init__(self, Model, settings ):
-        KratosMultiphysics.Process.__init__(self)
-
-        model_part = Model[settings["model_part_name"].GetString()]
-
-        self.components_process_list = []
-
-        if ("HydroLinePressure2D" in settings["model_part_name"].GetString()) or ("HydroSurfacePressure3D" in settings["model_part_name"].GetString()):
-
-            self.components_process_list.append(KratosDam.DamHydroConditionLoadProcess(model_part, settings))
-
-        if ("StraightUpliftLinePressure2D" in settings["model_part_name"].GetString()) or ("StraightUpliftSurfacePressure3D" in settings["model_part_name"].GetString()):
-
-            joint_model_part = Model["MainModelPart.Parts_" + settings["joint_group_name"].GetString()]
-            self.components_process_list.append(KratosDam.DamUpliftConditionLoadProcess(model_part, joint_model_part, settings))
-
-        if "CircularUpliftSurfacePressure3D" in settings["model_part_name"].GetString():
-
-            joint_model_part = Model["MainModelPart.Parts_" + settings["joint_group_name"].GetString()]
-            self.components_process_list.append(KratosDam.DamUpliftCircularConditionLoadProcess(model_part, joint_model_part, settings))
-
-        if ("HydroDynamicLinePressure2D" in settings["model_part_name"].GetString()) or ("HydroDynamicSurfacePressure3D" in settings["model_part_name"].GetString()):
-
-            self.components_process_list.append(KratosDam.DamWestergaardConditionLoadProcess(model_part, settings))
-
-    def ExecuteInitialize(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitialize()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        for component in self.components_process_list:
-            component.ExecuteInitializeSolutionStep()
-
-
+import KratosMultiphysics
+import KratosMultiphysics.DamApplication as KratosDam
+
+## This proces sets the value of water loads.
+
+def Factory(settings, Model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ImposeWaterLoadsConditionProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class ImposeWaterLoadsConditionProcess(KratosMultiphysics.Process):
+    def __init__(self, Model, settings ):
+        KratosMultiphysics.Process.__init__(self)
+
+        model_part = Model[settings["model_part_name"].GetString()]
+
+        self.components_process_list = []
+
+        if ("HydroLinePressure2D" in settings["model_part_name"].GetString()) or ("HydroSurfacePressure3D" in settings["model_part_name"].GetString()):
+
+            self.components_process_list.append(KratosDam.DamHydroConditionLoadProcess(model_part, settings))
+
+        if ("StraightUpliftLinePressure2D" in settings["model_part_name"].GetString()) or ("StraightUpliftSurfacePressure3D" in settings["model_part_name"].GetString()):
+
+            joint_model_part = Model["MainModelPart.Parts_" + settings["joint_group_name"].GetString()]
+            self.components_process_list.append(KratosDam.DamUpliftConditionLoadProcess(model_part, joint_model_part, settings))
+
+        if "CircularUpliftSurfacePressure3D" in settings["model_part_name"].GetString():
+
+            joint_model_part = Model["MainModelPart.Parts_" + settings["joint_group_name"].GetString()]
+            self.components_process_list.append(KratosDam.DamUpliftCircularConditionLoadProcess(model_part, joint_model_part, settings))
+
+        if ("HydroDynamicLinePressure2D" in settings["model_part_name"].GetString()) or ("HydroDynamicSurfacePressure3D" in settings["model_part_name"].GetString()):
+
+            self.components_process_list.append(KratosDam.DamWestergaardConditionLoadProcess(model_part, settings))
+
+    def ExecuteInitialize(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitialize()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        for component in self.components_process_list:
+            component.ExecuteInitializeSolutionStep()
+
+
```

## KratosMultiphysics/DamApplication/save_variables_utility.py

 * *Ordering differences only*

```diff
@@ -1,132 +1,132 @@
-# Import kratos core and applications
-import KratosMultiphysics
-import KratosMultiphysics.DamApplication as KratosDam
-import KratosMultiphysics.PoromechanicsApplication as KratosPoro
-
-class SaveVariablesUtility:
-
-    def SaveMechanicalVariables(problem_name, ProjectParameters, main_model_part, time):
-
-        OriginalMdpa = open(problem_name + ".mdpa" , 'r')
-        OutputMdpa = open(problem_name + "_mechanical_" + str(time) + ".mdpa", 'w')
-
-        for Line in OriginalMdpa:
-            if Line.startswith("Begin SubModelPart"):
-                OriginalMdpa.close()
-                break
-            OutputMdpa.write(Line)
-
-        mechanical_loads_sub_model_part_list = ProjectParameters["solver_settings"]["mechanical_solver_settings"]["problem_domain_sub_model_part_list"]
-
-        mechanical_parts = []
-
-        for i in range(mechanical_loads_sub_model_part_list.size()):
-            mechanical_parts.append(main_model_part.GetSubModelPart(mechanical_loads_sub_model_part_list[i].GetString()))
-
-        OutputMdpa.write('Begin NodalData DISPLACEMENT')
-        for part in mechanical_parts:
-            for node in part.Nodes:
-                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosMultiphysics.DISPLACEMENT)))
-        OutputMdpa.write('\nEnd NodalData\n')
-
-        OutputMdpa.write('\nBegin NodalData NODAL_CAUCHY_STRESS_TENSOR')
-        for part in mechanical_parts:
-            for node in part.Nodes:
-                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)))
-        OutputMdpa.write('\nEnd NodalData\n')
-
-        OutputMdpa.close()
-
-    def SaveFinalMechanicalVariables(problem_name, ProjectParameters, main_model_part):
-
-        OriginalMdpa = open(problem_name + ".mdpa" , 'r')
-        OutputMdpa = open(problem_name + "_mechanical.mdpa", 'w')
-
-        for Line in OriginalMdpa:
-            if Line.startswith("Begin SubModelPart"):
-                OriginalMdpa.close()
-                break
-            OutputMdpa.write(Line)
-
-        mechanical_loads_sub_model_part_list = ProjectParameters["solver_settings"]["mechanical_solver_settings"]["problem_domain_sub_model_part_list"]
-
-        mechanical_parts = []
-        for i in range(mechanical_loads_sub_model_part_list.size()):
-            mechanical_parts.append(main_model_part.GetSubModelPart(mechanical_loads_sub_model_part_list[i].GetString()))
-
-        OutputMdpa.write('Begin NodalData DISPLACEMENT')
-        for part in mechanical_parts:
-            for node in part.Nodes:
-                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosMultiphysics.DISPLACEMENT)))
-        OutputMdpa.write('\nEnd NodalData\n')
-
-        OutputMdpa.write('Begin NodalData NODAL_CAUCHY_STRESS_TENSOR')
-        for part in mechanical_parts:
-            for node in part.Nodes:
-                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)))
-        OutputMdpa.write('\nEnd NodalData\n')
-
-        OutputMdpa.close()
-
-    def SaveThermalVariables(problem_name, ProjectParameters, main_model_part, time):
-
-        OriginalMdpa = open(problem_name + ".mdpa" , 'r')
-        OutputMdpa = open(problem_name + "_thermal_" + str(time) + ".mdpa", 'w')
-
-        for Line in OriginalMdpa:
-            if Line.startswith("Begin SubModelPart"):
-                OriginalMdpa.close()
-                break
-            OutputMdpa.write(Line)
-
-        thermal_loads_sub_model_part_list = ProjectParameters["solver_settings"]["thermal_solver_settings"]["problem_domain_sub_model_part_list"]
-
-        thermal_parts = []
-
-        for i in range(thermal_loads_sub_model_part_list.size()):
-            thermal_parts.append(main_model_part.GetSubModelPart(thermal_loads_sub_model_part_list[i].GetString()))
-
-        OutputMdpa.write('Begin NodalData TEMPERATURE')
-        for part in thermal_parts:
-            for node in part.Nodes:
-                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosMultiphysics.TEMPERATURE)))
-        OutputMdpa.write('\nEnd NodalData\n')
-
-        OutputMdpa.write('\nBegin NodalData NODAL_REFERENCE_TEMPERATURE')
-        for part in thermal_parts:
-            for node in part.Nodes:
-                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosDam.NODAL_REFERENCE_TEMPERATURE)))
-        OutputMdpa.write('\nEnd NodalData\n')
-
-        OutputMdpa.close()
-
-    def SaveFinalThermalVariables(problem_name, ProjectParameters, main_model_part):
-
-        OriginalMdpa = open(problem_name + ".mdpa" , 'r')
-        OutputMdpa = open(problem_name + "_thermal.mdpa", 'w')
-
-        for Line in OriginalMdpa:
-            if Line.startswith("Begin SubModelPart"):
-                OriginalMdpa.close()
-                break
-            OutputMdpa.write(Line)
-
-        thermal_loads_sub_model_part_list = ProjectParameters["solver_settings"]["thermal_solver_settings"]["problem_domain_sub_model_part_list"]
-
-        thermal_parts = []
-        for i in range(thermal_loads_sub_model_part_list.size()):
-            thermal_parts.append(main_model_part.GetSubModelPart(thermal_loads_sub_model_part_list[i].GetString()))
-
-        OutputMdpa.write('Begin NodalData TEMPERATURE')
-        for part in thermal_parts:
-            for node in part.Nodes:
-                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosMultiphysics.TEMPERATURE)))
-        OutputMdpa.write('\nEnd NodalData\n')
-
-        OutputMdpa.write('\nBegin NodalData NODAL_REFERENCE_TEMPERATURE')
-        for part in thermal_parts:
-            for node in part.Nodes:
-                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosDam.NODAL_REFERENCE_TEMPERATURE)))
-        OutputMdpa.write('\nEnd NodalData\n')
-
-        OutputMdpa.close()
+# Import kratos core and applications
+import KratosMultiphysics
+import KratosMultiphysics.DamApplication as KratosDam
+import KratosMultiphysics.PoromechanicsApplication as KratosPoro
+
+class SaveVariablesUtility:
+
+    def SaveMechanicalVariables(problem_name, ProjectParameters, main_model_part, time):
+
+        OriginalMdpa = open(problem_name + ".mdpa" , 'r')
+        OutputMdpa = open(problem_name + "_mechanical_" + str(time) + ".mdpa", 'w')
+
+        for Line in OriginalMdpa:
+            if Line.startswith("Begin SubModelPart"):
+                OriginalMdpa.close()
+                break
+            OutputMdpa.write(Line)
+
+        mechanical_loads_sub_model_part_list = ProjectParameters["solver_settings"]["mechanical_solver_settings"]["problem_domain_sub_model_part_list"]
+
+        mechanical_parts = []
+
+        for i in range(mechanical_loads_sub_model_part_list.size()):
+            mechanical_parts.append(main_model_part.GetSubModelPart(mechanical_loads_sub_model_part_list[i].GetString()))
+
+        OutputMdpa.write('Begin NodalData DISPLACEMENT')
+        for part in mechanical_parts:
+            for node in part.Nodes:
+                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosMultiphysics.DISPLACEMENT)))
+        OutputMdpa.write('\nEnd NodalData\n')
+
+        OutputMdpa.write('\nBegin NodalData NODAL_CAUCHY_STRESS_TENSOR')
+        for part in mechanical_parts:
+            for node in part.Nodes:
+                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)))
+        OutputMdpa.write('\nEnd NodalData\n')
+
+        OutputMdpa.close()
+
+    def SaveFinalMechanicalVariables(problem_name, ProjectParameters, main_model_part):
+
+        OriginalMdpa = open(problem_name + ".mdpa" , 'r')
+        OutputMdpa = open(problem_name + "_mechanical.mdpa", 'w')
+
+        for Line in OriginalMdpa:
+            if Line.startswith("Begin SubModelPart"):
+                OriginalMdpa.close()
+                break
+            OutputMdpa.write(Line)
+
+        mechanical_loads_sub_model_part_list = ProjectParameters["solver_settings"]["mechanical_solver_settings"]["problem_domain_sub_model_part_list"]
+
+        mechanical_parts = []
+        for i in range(mechanical_loads_sub_model_part_list.size()):
+            mechanical_parts.append(main_model_part.GetSubModelPart(mechanical_loads_sub_model_part_list[i].GetString()))
+
+        OutputMdpa.write('Begin NodalData DISPLACEMENT')
+        for part in mechanical_parts:
+            for node in part.Nodes:
+                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosMultiphysics.DISPLACEMENT)))
+        OutputMdpa.write('\nEnd NodalData\n')
+
+        OutputMdpa.write('Begin NodalData NODAL_CAUCHY_STRESS_TENSOR')
+        for part in mechanical_parts:
+            for node in part.Nodes:
+                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosPoro.NODAL_CAUCHY_STRESS_TENSOR)))
+        OutputMdpa.write('\nEnd NodalData\n')
+
+        OutputMdpa.close()
+
+    def SaveThermalVariables(problem_name, ProjectParameters, main_model_part, time):
+
+        OriginalMdpa = open(problem_name + ".mdpa" , 'r')
+        OutputMdpa = open(problem_name + "_thermal_" + str(time) + ".mdpa", 'w')
+
+        for Line in OriginalMdpa:
+            if Line.startswith("Begin SubModelPart"):
+                OriginalMdpa.close()
+                break
+            OutputMdpa.write(Line)
+
+        thermal_loads_sub_model_part_list = ProjectParameters["solver_settings"]["thermal_solver_settings"]["problem_domain_sub_model_part_list"]
+
+        thermal_parts = []
+
+        for i in range(thermal_loads_sub_model_part_list.size()):
+            thermal_parts.append(main_model_part.GetSubModelPart(thermal_loads_sub_model_part_list[i].GetString()))
+
+        OutputMdpa.write('Begin NodalData TEMPERATURE')
+        for part in thermal_parts:
+            for node in part.Nodes:
+                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosMultiphysics.TEMPERATURE)))
+        OutputMdpa.write('\nEnd NodalData\n')
+
+        OutputMdpa.write('\nBegin NodalData NODAL_REFERENCE_TEMPERATURE')
+        for part in thermal_parts:
+            for node in part.Nodes:
+                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosDam.NODAL_REFERENCE_TEMPERATURE)))
+        OutputMdpa.write('\nEnd NodalData\n')
+
+        OutputMdpa.close()
+
+    def SaveFinalThermalVariables(problem_name, ProjectParameters, main_model_part):
+
+        OriginalMdpa = open(problem_name + ".mdpa" , 'r')
+        OutputMdpa = open(problem_name + "_thermal.mdpa", 'w')
+
+        for Line in OriginalMdpa:
+            if Line.startswith("Begin SubModelPart"):
+                OriginalMdpa.close()
+                break
+            OutputMdpa.write(Line)
+
+        thermal_loads_sub_model_part_list = ProjectParameters["solver_settings"]["thermal_solver_settings"]["problem_domain_sub_model_part_list"]
+
+        thermal_parts = []
+        for i in range(thermal_loads_sub_model_part_list.size()):
+            thermal_parts.append(main_model_part.GetSubModelPart(thermal_loads_sub_model_part_list[i].GetString()))
+
+        OutputMdpa.write('Begin NodalData TEMPERATURE')
+        for part in thermal_parts:
+            for node in part.Nodes:
+                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosMultiphysics.TEMPERATURE)))
+        OutputMdpa.write('\nEnd NodalData\n')
+
+        OutputMdpa.write('\nBegin NodalData NODAL_REFERENCE_TEMPERATURE')
+        for part in thermal_parts:
+            for node in part.Nodes:
+                OutputMdpa.write('\n' + str(node.Id) + ' 0 ' + str(node.GetSolutionStepValue(KratosDam.NODAL_REFERENCE_TEMPERATURE)))
+        OutputMdpa.write('\nEnd NodalData\n')
+
+        OutputMdpa.close()
```

## KratosMultiphysics/DamApplication/special_condition_process.py

 * *Ordering differences only*

```diff
@@ -1,18 +1,18 @@
-from KratosMultiphysics import *
-from KratosMultiphysics.DamApplication import *
-
-## This is process is related to add_mass processes
-
-def Factory(settings, Model):
-    if not isinstance(settings, Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return SpecialConditionProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-
-class SpecialConditionProcess(Process):
-    def __init__(self, Model, settings ):
-        Process.__init__(self)
-
-        model_part = Model[settings["model_part_name"].GetString()]
-        variable_name = settings["variable_name"].GetString()
+from KratosMultiphysics import *
+from KratosMultiphysics.DamApplication import *
+
+## This is process is related to add_mass processes
+
+def Factory(settings, Model):
+    if not isinstance(settings, Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return SpecialConditionProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+
+class SpecialConditionProcess(Process):
+    def __init__(self, Model, settings ):
+        Process.__init__(self)
+
+        model_part = Model[settings["model_part_name"].GetString()]
+        variable_name = settings["variable_name"].GetString()
```

## KratosMultiphysics/DamApplication/streamlines_output_utility.py

 * *Ordering differences only*

```diff
@@ -1,22 +1,22 @@
-#importing the Kratos Library
-from KratosMultiphysics import *
-from KratosMultiphysics.StructuralMechanicsApplication import *
-# from KratosMultiphysics.ExternalSolversApplication import *
-from KratosMultiphysics.DamApplication import *
-
-class StreamlinesOutputUtility:
-
-    def __init__(self,domain_size):
-
-        # Construct the utility
-        self.domain_size = domain_size
-        if domain_size==3:
-            self.OutputUtility = StreamlinesOutput3DUtilities()
-
-        else:
-            print("**************** Must be implemented ****************")
-
-
-    def ComputeOutputStep(self, main_model_part ,domain_size):
-
-        self.OutputUtility.ComputeOutputStep( main_model_part ,domain_size)
+#importing the Kratos Library
+from KratosMultiphysics import *
+from KratosMultiphysics.StructuralMechanicsApplication import *
+# from KratosMultiphysics.ExternalSolversApplication import *
+from KratosMultiphysics.DamApplication import *
+
+class StreamlinesOutputUtility:
+
+    def __init__(self,domain_size):
+
+        # Construct the utility
+        self.domain_size = domain_size
+        if domain_size==3:
+            self.OutputUtility = StreamlinesOutput3DUtilities()
+
+        else:
+            print("**************** Must be implemented ****************")
+
+
+    def ComputeOutputStep(self, main_model_part ,domain_size):
+
+        self.OutputUtility.ComputeOutputStep( main_model_part ,domain_size)
```

## KratosMultiphysics/DamApplication/transfer_selfweight_stress_utility.py

 * *Ordering differences only*

```diff
@@ -1,20 +1,20 @@
-#importing the Kratos Library
-from KratosMultiphysics import *
-from KratosMultiphysics.StructuralMechanicsApplication import *
-# from KratosMultiphysics.ExternalSolversApplication import *
-from KratosMultiphysics.DamApplication import *
-
-class TransferSelfweightStressToMainModelPartUtility:
-
-    def __init__(self):
-
-        self.TransferUtility = TransferSelfweightStressUtility()
-
-    def Transfer(self,selfweight_model_part,model_part,domain_size):
-
-        self.TransferUtility.Transfer(selfweight_model_part, model_part, domain_size)
-
-    def TransferInitialStress(self,model_part,domain_size):
-
-        self.TransferUtility.TransferInitialStress(model_part, domain_size)
-
+#importing the Kratos Library
+from KratosMultiphysics import *
+from KratosMultiphysics.StructuralMechanicsApplication import *
+# from KratosMultiphysics.ExternalSolversApplication import *
+from KratosMultiphysics.DamApplication import *
+
+class TransferSelfweightStressToMainModelPartUtility:
+
+    def __init__(self):
+
+        self.TransferUtility = TransferSelfweightStressUtility()
+
+    def Transfer(self,selfweight_model_part,model_part,domain_size):
+
+        self.TransferUtility.Transfer(selfweight_model_part, model_part, domain_size)
+
+    def TransferInitialStress(self,model_part,domain_size):
+
+        self.TransferUtility.TransferInitialStress(model_part, domain_size)
+
```

## Comparing `KratosDamApplication-9.4.6.dist-info/METADATA` & `KratosDamApplication-9.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1
-Name: KratosDamApplication
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
-Requires-Dist: KratosPoromechanicsApplication ==9.4.6
-Requires-Dist: KratosStructuralMechanicsApplication ==9.4.6
-
-### Using MPI in DamApplication ###
-
-Note: For the moment, MPI only works in Linux and requires compiling METIS_APPLICATION and TRILINOS_APPLICATION. Non-local Damage does not work in MPI.
-
-## Instructions to compile DamApplication for MPI (tested in Ubuntu 16.04) ##
-
-1. Make sure that the following lines are properly set in the configure.sh file:
-
--DMETIS_APPLICATION=ON								                                        \
--DMETIS_INCLUDE_DIR="/usr/include/"                                                         \
--DPARMETIS_ROOT_DIR="/usr/lib/"                                                   			\
--DTRILINOS_APPLICATION=ON							                                        \
--DTRILINOS_LIBRARY_DIR="/usr/lib/x86_64-linux-gnu/"                                         \
--DTRILINOS_INCLUDE_DIR="/usr/include/trilinos/"                                             \
--DTRILINOS_LIBRARY_PREFIX="trilinos_"                                                       \
--DCONVECTION_DIFFUSION_APPLICATION=ON 						                              \
--DEXTERNAL_SOLVERS_APPLICATION=ON						                                    \
--DSTRUCTURAL_MECHANICS_APPLICATION=ON   					                                    \
--DPOROMECHANICS_APPLICATION=ON \
--DDAM_APPLICATION=ON \
--DUSE_DAM_MPI=ON \
-
-2. Uncomment (remove #~ ) the following line in GiDInterface/Kratos.gid/apps/Dam/python/dam_main.py
-
-#~ import KratosMultiphysics.TrilinosApplication as TrilinosApplication
+Metadata-Version: 2.1
+Name: KratosDamApplication
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
+Requires-Dist: KratosPoromechanicsApplication ==9.5
+Requires-Dist: KratosStructuralMechanicsApplication ==9.5
+
+### Using MPI in DamApplication ###
+
+Note: For the moment, MPI only works in Linux and requires compiling METIS_APPLICATION and TRILINOS_APPLICATION. Non-local Damage does not work in MPI.
+
+## Instructions to compile DamApplication for MPI (tested in Ubuntu 16.04) ##
+
+1. Make sure that the following lines are properly set in the configure.sh file:
+
+-DMETIS_APPLICATION=ON								                                        \
+-DMETIS_INCLUDE_DIR="/usr/include/"                                                         \
+-DPARMETIS_ROOT_DIR="/usr/lib/"                                                   			\
+-DTRILINOS_APPLICATION=ON							                                        \
+-DTRILINOS_LIBRARY_DIR="/usr/lib/x86_64-linux-gnu/"                                         \
+-DTRILINOS_INCLUDE_DIR="/usr/include/trilinos/"                                             \
+-DTRILINOS_LIBRARY_PREFIX="trilinos_"                                                       \
+-DCONVECTION_DIFFUSION_APPLICATION=ON 						                              \
+-DEXTERNAL_SOLVERS_APPLICATION=ON						                                    \
+-DSTRUCTURAL_MECHANICS_APPLICATION=ON   					                                    \
+-DPOROMECHANICS_APPLICATION=ON \
+-DDAM_APPLICATION=ON \
+-DUSE_DAM_MPI=ON \
+
+2. Uncomment (remove #~ ) the following line in GiDInterface/Kratos.gid/apps/Dam/python/dam_main.py
+
+#~ import KratosMultiphysics.TrilinosApplication as TrilinosApplication
```

## Comparing `KratosDamApplication-9.4.6.dist-info/RECORD` & `KratosDamApplication-9.5.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-KratosMultiphysics/.libs/KratosDamApplication.pyd,sha256=w4pLyQiezWmsL2xMhr6qRrOYmg3XsybkE8UKdSBe08g,1624064
-KratosMultiphysics/.libs/KratosDamCore.dll,sha256=5TGRTEvFgQsDx09rXOe8Z7MuPOuJSlRWh0WK-iOZNo4,2483200
-KratosMultiphysics/.libs/KratosDamCore.lib,sha256=PxgLaGCpI2Z3CnTNQhFOtl1EXbisHoMFWadRvs3UHGE,266260
-KratosMultiphysics/DamApplication/__init__.py,sha256=c7O2srOPUhk-7C5tSt2u5-PtX73fwUAdw3R_oUoy-yk,373
-KratosMultiphysics/DamApplication/apply_constraint_vector_dam_table_process.py,sha256=-XVlLrbvrpveBbGFEKHaOD_LQXEpwEwE_vLSq2XyOjk,2977
-KratosMultiphysics/DamApplication/apply_load_vector_dam_process.py,sha256=lv4uldgEW93LnHX5f3Fq_QbGxGCyAFDmQCk1XyE4LvM,2558
-KratosMultiphysics/DamApplication/apply_load_vector_dam_table_process.py,sha256=WFzNTCasZfGdTj8dg00hixuVuVjE0UHwD-M-FtjLq7g,3288
-KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_mechanical.py,sha256=csGGVM7szD8oVQh--dBPRRLxMFS5ng8MpleJJUmBoWQ,4848
-KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_thermal.py,sha256=4JCDQYfdOV3o0vUNNYCKrUsvG7mb2hD-l06GdlzEuPs,9244
-KratosMultiphysics/DamApplication/check_and_prepare_selfweight_model_process_dam.py,sha256=UBluLjw550CYsMR-EEPAZIFp7aHlI5SlHhxsJwXBpn0,4956
-KratosMultiphysics/DamApplication/dam_P_solver.py,sha256=d8-pUZSksO1k-44cUg7EpCDYt29DSSUOE_Nzp-aHs_U,6973
-KratosMultiphysics/DamApplication/dam_UP_mechanical_solver.py,sha256=b-BvBwL252I2aD8dNEJ8N0ZGBY2_xmCcR8MyyqFfXZo,5397
-KratosMultiphysics/DamApplication/dam_UP_thermo_mechanic_solver.py,sha256=hrslEnAIVRePFGoUcN4r1EFzxKLgqLg2unILwpcilIM,6731
-KratosMultiphysics/DamApplication/dam_analysis.py,sha256=6ToLpeZ2fvflXxi2GPtSRtsNeNt1GLSbEwfEu0H6OHs,26347
-KratosMultiphysics/DamApplication/dam_cleaning_utility.py,sha256=UkAMZRP1YDkYsp7z7vQsHpPNenz1Ck2nktvpWLyySxM,675
-KratosMultiphysics/DamApplication/dam_constitutive_law_utility.py,sha256=c7MqIKq8s3R_Yo4vqC3uFwsyUdjEq87oBgwWe0NTLP8,793
-KratosMultiphysics/DamApplication/dam_construction_utility.py,sha256=1YtCN7nd7yEZUFxJBgg3vF5Px1ZrEhUM7LxsGmJO3BA,9313
-KratosMultiphysics/DamApplication/dam_eigen_solver.py,sha256=l71oU-l8L8FBX9Jfy-qNy1nW7cSZe_7uLEF2K_JyipU,6604
-KratosMultiphysics/DamApplication/dam_mapping_variables_utility.py,sha256=WzI3daHaZkyFK86vWlSnOMwLyHXjcUDdU_3GILe6NX4,2196
-KratosMultiphysics/DamApplication/dam_mechanical_solver.py,sha256=JDj4oc_2f4dobyBMGx03bxPfHy2CDWkejCZVxVGNWbQ,22475
-KratosMultiphysics/DamApplication/dam_selfweight_solver.py,sha256=w1KBXd4qDLkaim7hv_dtdr26mBLc00q_Hj6lIG8B3_c,24523
-KratosMultiphysics/DamApplication/dam_thermo_mechanic_solver.py,sha256=dev2Q8CHpJlaYJuUnFhDtpXLiqfcu1hr95bJMS5d8Io,29961
-KratosMultiphysics/DamApplication/gid_dam_output_process.py,sha256=ZO8WWjRKjk2g1Ys6LmXHYG4Gd1bbCAlYQ7jsBR4_nkE,35439
-KratosMultiphysics/DamApplication/global_joint_stress_utility.py,sha256=OVYkqsSAkZY_wTEfesH_y7mHf2kXFF_FB3g4ZprYqIk,1114
-KratosMultiphysics/DamApplication/impose_2d_random_fields_variable_process.py,sha256=ELh8fPXqY5cCbLMTT-cIqRY9l3XEgdFx9w38hqgSMwY,2431
-KratosMultiphysics/DamApplication/impose_3d_random_fields_variable_process.py,sha256=3a2lgihWWJ57bDHt3iR0BBm0Kx9g5wvipzTpKlY91CI,2482
-KratosMultiphysics/DamApplication/impose_chemo_mechanical_aging_process.py,sha256=iVt2pE_06ItYE9hEob7owa9Avp-VjGzmLjOyoUiIVnw,864
-KratosMultiphysics/DamApplication/impose_face_heat_flux_process.py,sha256=B26I7ykbC2b9NQcRHI3UrRtmryilPlLx5FT-kkiHdnQ,3212
-KratosMultiphysics/DamApplication/impose_grouting_reference_temperature_process.py,sha256=SJAjZxkSl6bitVtFJ6uCCBkURF7B5eR6uEZrJq_9b-0,882
-KratosMultiphysics/DamApplication/impose_heat_source_process.py,sha256=Xnuyf6hToemzkPHowkrENhnzyadcbB7wpYk5XLXu8p8,1462
-KratosMultiphysics/DamApplication/impose_input_table_nodal_young_modulus_process.py,sha256=DmAylAi-ykrpEENSYHSJ4Neah9nm2oznjB1NGxi6pxQ,1924
-KratosMultiphysics/DamApplication/impose_nodal_reference_temperature_process.py,sha256=f1dkPR8tYjFTeUuzSA2ejNx7uH1mJGC7CUTzA3edTh8,1856
-KratosMultiphysics/DamApplication/impose_nodal_young_modulus_process.py,sha256=qxJOFmu3-xwC6Ui-jgP5ZR_NbSRHUFgd4s84kvH1mUA,916
-KratosMultiphysics/DamApplication/impose_reservoir_temperature_condition_process.py,sha256=40MceeitgSI0AeIjlBLTv9Sjex4jQdUc34lNLFYY-S8,1868
-KratosMultiphysics/DamApplication/impose_temperature_by_device_process.py,sha256=L5fUEKvtKV3cW7kygsd7punHpKIkb5kfLNflHAWmRRw,723
-KratosMultiphysics/DamApplication/impose_thermal_parameters_scalar_value_process.py,sha256=IsBgDVOZ0ODhoLojexTtwWBvoRkUo8lKvNic6YDv0Lc,2480
-KratosMultiphysics/DamApplication/impose_uniform_temperature_process.py,sha256=dnHWxwv0vHmFTY4MGDb5Hi4yP-1qgqUSYdA8neX9yFk,1702
-KratosMultiphysics/DamApplication/impose_water_loads_condition_process.py,sha256=UeoFI5vzbe8AkdZ-ebGyrItmNHaDOJxjMCkzvdDn6Ho,2354
-KratosMultiphysics/DamApplication/save_variables_utility.py,sha256=SF2yPD_jVHOH59oXLPmb37zDzlR0JAyU5GNXfzl5VbA,6056
-KratosMultiphysics/DamApplication/special_condition_process.py,sha256=q2hoOgCfBkS0E_AYjS6Y3M1ZxpnSsM6szig1btukpUc,701
-KratosMultiphysics/DamApplication/streamlines_output_utility.py,sha256=T0YMHRTwrVTQxUZ87oXfS5ePv31JF6YQ9BTtVQk8SaY,724
-KratosMultiphysics/DamApplication/transfer_selfweight_stress_utility.py,sha256=jcoC1zRAhraaK3bS8H81bAwLUZFRnyfzhtrXiYnW6EA,699
-KratosDamApplication-9.4.6.dist-info/METADATA,sha256=Pfso2sH6d61WtbAVZYbJnbKRloeJU-ljKWCIwxhS9dY,2961
-KratosDamApplication-9.4.6.dist-info/WHEEL,sha256=GZFS91_ufm4WrNPBaFVPB9MvOXR6bMZQhPcZRRTN5YM,100
-KratosDamApplication-9.4.6.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
-KratosDamApplication-9.4.6.dist-info/RECORD,,
+KratosDamApplication-9.5.dist-info/METADATA,sha256=LIQIRVrFzQ_y-YBzrbMd1U1ERhbr66snNaNUKA8Y5aI,2898
+KratosDamApplication-9.5.dist-info/WHEEL,sha256=rY0Y6THYM7EImsHfF-zs67o8pQciAsMw9_YuSvftjrQ,148
+KratosDamApplication-9.5.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
+KratosDamApplication-9.5.dist-info/RECORD,,
+KratosMultiphysics/DamApplication/impose_input_table_nodal_young_modulus_process.py,sha256=0enFD0wIkiM3l3UgdhTQj_0yC4ydPfyudtIMMBbR7YE,1879
+KratosMultiphysics/DamApplication/impose_grouting_reference_temperature_process.py,sha256=EUlytZbiC1mzGQd0psi_a3hYJ9VPs7SambjUfXr_bKI,857
+KratosMultiphysics/DamApplication/apply_load_vector_dam_table_process.py,sha256=Ci1FEIxS-G5DfrlF5kxdj3y5NkuA5ajcuHmBTduDcPk,3223
+KratosMultiphysics/DamApplication/impose_thermal_parameters_scalar_value_process.py,sha256=kX88-YdsqkpEBkxj3TmTYL0eR4oREn1bJL-fAmao7qY,2423
+KratosMultiphysics/DamApplication/dam_eigen_solver.py,sha256=QNeZ7SKCUE1ig3q2TF6yb6lEDEsCqtxBDuiw3E4VypE,6374
+KratosMultiphysics/DamApplication/dam_thermo_mechanic_solver.py,sha256=lVGMYsVXIpF9dLb42mtJXNy-rFeuQKA2OCplBAsoJac,29449
+KratosMultiphysics/DamApplication/streamlines_output_utility.py,sha256=pMzX6JYphMSU_ZsRAOQPgHtGh65mUUxZVAiqFWMxGps,702
+KratosMultiphysics/DamApplication/impose_2d_random_fields_variable_process.py,sha256=J-rmJ2dxq8HiwOCFbhhZYoBkerkDj7Ad07rucAMC6l8,2360
+KratosMultiphysics/DamApplication/check_and_prepare_selfweight_model_process_dam.py,sha256=E5VSFqTg-jCb7Oau9_cjpwfFA7FWFMt0l_g3v11o9-4,4871
+KratosMultiphysics/DamApplication/gid_dam_output_process.py,sha256=4sLjAb9x0Jzf5Fds5cg7zchAq0PpLB_VRDSr7W9oiI4,34676
+KratosMultiphysics/DamApplication/impose_chemo_mechanical_aging_process.py,sha256=Th_8BplYHsaOQjQfD9gOxObqoNxXQtrS2UOcUqFMAD0,841
+KratosMultiphysics/DamApplication/impose_heat_source_process.py,sha256=o5cOx4hGp7F7FRGBWzOMjZLScpEnEd6TJNXoxMhMeCQ,1428
+KratosMultiphysics/DamApplication/dam_selfweight_solver.py,sha256=HItlOeRJcBkYuzGNOkuiwI3u6brQ1Ssa6yH3El3G61Q,24082
+KratosMultiphysics/DamApplication/impose_nodal_reference_temperature_process.py,sha256=J8zh-_A5OuQDGIcfPvzasIObx12Iwp5oHNFzOYvrE9I,1810
+KratosMultiphysics/DamApplication/dam_construction_utility.py,sha256=ULzq63aC4WIor0zsBMjz5cx0LOYtp3V-aM430Kxb9O4,9151
+KratosMultiphysics/DamApplication/impose_uniform_temperature_process.py,sha256=cgaaOobM4zXmG_hFvBUy4afdTWlFpyW72yGoMpOnLsA,1663
+KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_thermal.py,sha256=nTrH56F3D_78eMzG8PYS9rYRcCftC_P0TWG2WSa5viM,9089
+KratosMultiphysics/DamApplication/dam_cleaning_utility.py,sha256=K6oiObYybjwTqgXofohgKpuQZocAs9ekiSERJ2FLojE,650
+KratosMultiphysics/DamApplication/impose_nodal_young_modulus_process.py,sha256=GCGDe0HYVUPQl74Wm2ybZsxCcT5sGmwxXAVIOx1_ks8,888
+KratosMultiphysics/DamApplication/dam_UP_mechanical_solver.py,sha256=5pqS8RqpIOU30mfGrp4ukWA_bqxymsF0HvjFF1Cwy6Q,5269
+KratosMultiphysics/DamApplication/transfer_selfweight_stress_utility.py,sha256=Ql_POkRH2Dqgz1xPNVd_Ubi-dRwTm5uaAtIFRzN1rIE,679
+KratosMultiphysics/DamApplication/impose_reservoir_temperature_condition_process.py,sha256=RfnY8NHXra8YjIIl4O1uovSotLAqYvpzB8930ZuqRDQ,1823
+KratosMultiphysics/DamApplication/check_and_prepare_model_process_dam_mechanical.py,sha256=jf3XIMPaJMEBxvvYwf8MjSb0bvPmgweve1Pj9O9Kf64,4765
+KratosMultiphysics/DamApplication/apply_load_vector_dam_process.py,sha256=D7BrDsdc41oOr4JAW8oX5PpV9ZvM6898C8EhAJ3S8bU,2505
+KratosMultiphysics/DamApplication/impose_temperature_by_device_process.py,sha256=f-c67FT1rY6uL6vP8sXSL_vpvHt_rcNAsnYx5p3jDbI,702
+KratosMultiphysics/DamApplication/global_joint_stress_utility.py,sha256=FHYD0HF4ku2cowD4LOlXBr0pogHj2eMrvKbBWwe4g7c,1087
+KratosMultiphysics/DamApplication/dam_constitutive_law_utility.py,sha256=4NPzNsiQJswiIb_xyQ8UhObqWm2PKZFWdMxCOPey6VA,775
+KratosMultiphysics/DamApplication/dam_mechanical_solver.py,sha256=Cubzivo1YumFGbDNTa7rRhizonRXcBMSRKWDpHaavMQ,22066
+KratosMultiphysics/DamApplication/dam_UP_thermo_mechanic_solver.py,sha256=xQ6wiegu0SUaGVIcI1Yf8HbGgOYfh192qMqlF3Bga58,6575
+KratosMultiphysics/DamApplication/special_condition_process.py,sha256=mRITexX_ON_m2Knpd9Y4U_ymb63EjIeDM9vYTx3neb4,683
+KratosMultiphysics/DamApplication/impose_face_heat_flux_process.py,sha256=9HuLbMJX3ztiIZMyWR_hWTHwGfB4Bknzi-Oy-0v10BQ,3156
+KratosMultiphysics/DamApplication/dam_mapping_variables_utility.py,sha256=WzI3daHaZkyFK86vWlSnOMwLyHXjcUDdU_3GILe6NX4,2196
+KratosMultiphysics/DamApplication/dam_P_solver.py,sha256=9vWSYY4tCM9FKn7YRoLRrWUBAzk1G9a8Jcee504nzPA,6809
+KratosMultiphysics/DamApplication/save_variables_utility.py,sha256=Pe5xVuO9KCUOP-ep-1bqjoPNVuSzF1M_Zv5IMcF2uSA,5924
+KratosMultiphysics/DamApplication/__init__.py,sha256=lbSDT93fwOJsaFacUU2AB1RjVigM5zCr2CKMoLmkaMs,363
+KratosMultiphysics/DamApplication/apply_constraint_vector_dam_table_process.py,sha256=Z_Yr0iC2w97nOkfXXlfve3DYDPamPfUO8UjOibRRmyw,2916
+KratosMultiphysics/DamApplication/impose_3d_random_fields_variable_process.py,sha256=NFXJorxnkO09sOtjChyUpLzu4WSQ_5V55Us2ILnyzP8,2408
+KratosMultiphysics/DamApplication/impose_water_loads_condition_process.py,sha256=VnS7BFT0Efrq_r9nPVXWcx9qIuryKqH72c7hP_Ucvk0,2306
+KratosMultiphysics/DamApplication/dam_analysis.py,sha256=fefbTLwnOyY2KqIZP_VerfHO7d-iwxSrUyjbNBIOK_A,25883
+KratosMultiphysics/.libs/KratosDamApplication.cpython-39-x86_64-linux-gnu.so,sha256=nE1KgTyXVCTax3--8ffAZb29Ns6LELU-Imjytq3RzTs,3827505
+KratosDamApplication.libs/libKratosDamCore-90b98398.so,sha256=3pYZGz_RY2VRItr-958oiAK5TmknLjtU3vs9hBSIN3Q,11791673
```

