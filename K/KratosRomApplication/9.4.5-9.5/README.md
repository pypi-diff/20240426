# Comparing `tmp/KratosRomApplication-9.4.5-cp39-cp39-win_amd64.whl.zip` & `tmp/KratosRomApplication-9.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,887 +1,1010 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    966921 (00000000000EC109h)
-  Actual end-cent-dir record offset:        966899 (00000000000EC0F3h)
-  Expected end-cent-dir record offset:      966899 (00000000000EC0F3h)
+  Zip archive file size:                   3827421 (00000000003A66DDh)
+  Actual end-cent-dir record offset:       3827399 (00000000003A66C7h)
+  Expected end-cent-dir record offset:     3827399 (00000000003A66C7h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 30 entries.
-  The central directory is 3157 (0000000000000C55h) bytes long,
+  central directory contains 27 entries.
+  The central directory is 3262 (0000000000000CBEh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 963742 (00000000000EB49Eh).
+  is 3824137 (00000000003A5A09h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosRomApplication.pyd
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
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:30
-  32-bit CRC value (hex):                         a2ea76fd
-  compressed size:                                424169 bytes
-  uncompressed size:                              1342976 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
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
 
-  KratosMultiphysics/.libs/KratosRomCore.dll
+  KratosMultiphysics/RomApplication/
 
-  offset of local header from start of archive:   424248
-                                                  (0000000000067938h) bytes
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
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:30
-  32-bit CRC value (hex):                         a96208c4
-  compressed size:                                487976 bytes
-  uncompressed size:                              1531904 bytes
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
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
 
 Central directory entry #3:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosRomCore.lib
+  KratosMultiphysics/RomApplication/hrom_training_utility.py
 
-  offset of local header from start of archive:   912296
-                                                  (00000000000DEBA8h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   169
+                                                  (00000000000000A9h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:30
-  32-bit CRC value (hex):                         f288f532
-  compressed size:                                3238 bytes
-  uncompressed size:                              40236 bytes
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         1b54eb44
+  compressed size:                                5666 bytes
+  uncompressed size:                              28257 bytes
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
 
 Central directory entry #4:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/__init__.py
+  KratosMultiphysics/RomApplication/python_solvers_wrapper_rom.py
 
-  offset of local header from start of archive:   915606
-                                                  (00000000000DF896h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   5951
+                                                  (000000000000173Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         3fb6b322
-  compressed size:                                147 bytes
-  uncompressed size:                              316 bytes
-  length of filename:                             45 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         75274145
+  compressed size:                                1271 bytes
+  uncompressed size:                              4349 bytes
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
 
-  KratosMultiphysics/RomApplication/auxiliary_functions_workflow.py
+  KratosMultiphysics/RomApplication/rom_manager.py
 
-  offset of local header from start of archive:   915828
-                                                  (00000000000DF974h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   7343
+                                                  (0000000000001CAFh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         7cb02df6
-  compressed size:                                445 bytes
-  uncompressed size:                              1079 bytes
-  length of filename:                             65 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         6cc2884f
+  compressed size:                                5731 bytes
+  uncompressed size:                              46517 bytes
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
 
 Central directory entry #6:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/calculate_rom_basis_output_process.py
+  KratosMultiphysics/RomApplication/rom_testing_utilities.py
 
-  offset of local header from start of archive:   916368
-                                                  (00000000000DFB90h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   13180
+                                                  (000000000000337Ch) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         5fbbe928
-  compressed size:                                2973 bytes
-  uncompressed size:                              10841 bytes
-  length of filename:                             71 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         089819a8
+  compressed size:                                776 bytes
+  uncompressed size:                              2569 bytes
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
 
-  KratosMultiphysics/RomApplication/convection_diffusion_analysis_rom.py
+  KratosMultiphysics/RomApplication/tsqr.py
 
-  offset of local header from start of archive:   919442
-                                                  (00000000000E0792h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   14072
+                                                  (00000000000036F8h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         4172bc33
-  compressed size:                                873 bytes
-  uncompressed size:                              2421 bytes
-  length of filename:                             70 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         f73f7437
+  compressed size:                                2792 bytes
+  uncompressed size:                              7828 bytes
+  length of filename:                             41 characters
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
 
-  KratosMultiphysics/RomApplication/convection_diffusion_stationary_rom_solver.py
+  KratosMultiphysics/RomApplication/randomized_singular_value_decomposition.py
 
-  offset of local header from start of archive:   920415
-                                                  (00000000000E0B5Fh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   16963
+                                                  (0000000000004243h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         120e2a93
-  compressed size:                                742 bytes
-  uncompressed size:                              2015 bytes
-  length of filename:                             79 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         c91dc8d2
+  compressed size:                                2586 bytes
+  uncompressed size:                              8901 bytes
+  length of filename:                             76 characters
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
 
-  KratosMultiphysics/RomApplication/convection_diffusion_transient_rom_solver.py
+  KratosMultiphysics/RomApplication/rom_solver.py
 
-  offset of local header from start of archive:   921266
-                                                  (00000000000E0EB2h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   19683
+                                                  (0000000000004CE3h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         bea73c4d
-  compressed size:                                743 bytes
-  uncompressed size:                              2009 bytes
-  length of filename:                             78 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         1111aacf
+  compressed size:                                1563 bytes
+  uncompressed size:                              5670 bytes
+  length of filename:                             47 characters
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
 
-  KratosMultiphysics/RomApplication/empirical_cubature_method.py
+  KratosMultiphysics/RomApplication/parallel_svd.py
 
-  offset of local header from start of archive:   922117
-                                                  (00000000000E1205h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   21351
+                                                  (0000000000005367h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         b297b4d0
-  compressed size:                                3549 bytes
-  uncompressed size:                              13632 bytes
-  length of filename:                             62 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         0fb0cdfa
+  compressed size:                                1268 bytes
+  uncompressed size:                              3202 bytes
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
 
 Central directory entry #11:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/fluid_dynamics_analysis_rom.py
+  KratosMultiphysics/RomApplication/rom_analysis.py
 
-  offset of local header from start of archive:   925758
-                                                  (00000000000E203Eh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   22726
+                                                  (00000000000058C6h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         78a6d795
-  compressed size:                                1405 bytes
-  uncompressed size:                              4734 bytes
-  length of filename:                             64 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         f9c8915e
+  compressed size:                                3909 bytes
+  uncompressed size:                              19427 bytes
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
 
 Central directory entry #12:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/hrom_training_utility.py
+  KratosMultiphysics/RomApplication/calculate_rom_basis_output_process.py
 
-  offset of local header from start of archive:   927257
-                                                  (00000000000E2619h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   26742
+                                                  (0000000000006876h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         d46b6023
-  compressed size:                                5383 bytes
-  uncompressed size:                              26781 bytes
-  length of filename:                             58 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         33200ac4
+  compressed size:                                2964 bytes
+  uncompressed size:                              10650 bytes
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
 
 Central directory entry #13:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/navier_stokes_solver_vmsmonolithic_rom.py
+  KratosMultiphysics/RomApplication/auxiliary_functions_workflow.py
 
-  offset of local header from start of archive:   932728
-                                                  (00000000000E3B78h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   29835
+                                                  (000000000000748Bh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         1ea2fcbc
-  compressed size:                                640 bytes
-  uncompressed size:                              1610 bytes
-  length of filename:                             75 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         adbe3575
+  compressed size:                                437 bytes
+  uncompressed size:                              1059 bytes
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
 
 Central directory entry #14:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/new_python_solvers_wrapper_rom.py
+  KratosMultiphysics/RomApplication/empirical_cubature_method.py
 
-  offset of local header from start of archive:   933473
-                                                  (00000000000E3E61h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   30395
+                                                  (00000000000076BBh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         906057dd
-  compressed size:                                1281 bytes
-  uncompressed size:                              4427 bytes
-  length of filename:                             67 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         c19388a5
+  compressed size:                                3523 bytes
+  uncompressed size:                              13342 bytes
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
 
 Central directory entry #15:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/parallel_svd.py
+  KratosMultiphysics/RomApplication/petrov_galerkin_training_utility.py
 
-  offset of local header from start of archive:   934851
-                                                  (00000000000E43C3h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   34038
+                                                  (00000000000084F6h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         0fb0cdfa
-  compressed size:                                1268 bytes
-  uncompressed size:                              3202 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         58337863
+  compressed size:                                2787 bytes
+  uncompressed size:                              10217 bytes
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
 
 Central directory entry #16:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/petrov_galerkin_training_utility.py
+  KratosMultiphysics/RomApplication/save_rom_coefficients_process.py
 
-  offset of local header from start of archive:   936198
-                                                  (00000000000E4906h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   36952
+                                                  (0000000000009058h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         f3362907
-  compressed size:                                2887 bytes
-  uncompressed size:                              10522 bytes
-  length of filename:                             69 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         a0a7e285
+  compressed size:                                1727 bytes
+  uncompressed size:                              5767 bytes
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
 
 Central directory entry #17:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/python_solvers_wrapper_rom.py
+  KratosMultiphysics/RomApplication/__init__.py
 
-  offset of local header from start of archive:   939184
-                                                  (00000000000E54B0h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   38803
+                                                  (0000000000009793h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         2e4b113b
-  compressed size:                                920 bytes
-  uncompressed size:                              3495 bytes
-  length of filename:                             63 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         3fb6b322
+  compressed size:                                147 bytes
+  uncompressed size:                              316 bytes
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
 
 Central directory entry #18:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/randomized_singular_value_decomposition.py
+  KratosMultiphysics/.libs/
 
-  offset of local header from start of archive:   940197
-                                                  (00000000000E58A5h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   39053
+                                                  (000000000000988Dh) bytes
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
-  32-bit CRC value (hex):                         ddf218b6
-  compressed size:                                2601 bytes
-  uncompressed size:                              9122 bytes
-  length of filename:                             76 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:44
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:43 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:43 UTC
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
 
 Central directory entry #19:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/rom_analysis.py
+  KratosMultiphysics/.libs/KratosRomApplication.cpython-39-x86_64-linux-gnu.so
 
-  offset of local header from start of archive:   942904
-                                                  (00000000000E6338h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   39136
+                                                  (00000000000098E0h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         d28afa86
-  compressed size:                                3719 bytes
-  uncompressed size:                              18713 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         90d4590d
+  compressed size:                                1164412 bytes
+  uncompressed size:                              3227745 bytes
+  length of filename:                             76 characters
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
 
 Central directory entry #20:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/rom_manager.py
+  KratosRomApplication-9.5.dist-info/
 
-  offset of local header from start of archive:   946702
-                                                  (00000000000E720Eh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1203682
+                                                  (0000000000125DE2h) bytes
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
-  32-bit CRC value (hex):                         25cd67f2
-  compressed size:                                5735 bytes
-  uncompressed size:                              47318 bytes
-  length of filename:                             48 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:44
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:43 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:43 UTC
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
 
 Central directory entry #21:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/rom_solver.py
+  KratosRomApplication-9.5.dist-info/METADATA
 
-  offset of local header from start of archive:   952515
-                                                  (00000000000E88C3h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1203775
+                                                  (0000000000125E3Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         035eb3c1
-  compressed size:                                1572 bytes
-  uncompressed size:                              5768 bytes
-  length of filename:                             47 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         aa0ffd00
+  compressed size:                                542 bytes
+  uncompressed size:                              1343 bytes
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
 
 Central directory entry #22:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/rom_testing_utilities.py
+  KratosRomApplication-9.5.dist-info/WHEEL
 
-  offset of local header from start of archive:   954164
-                                                  (00000000000E8F34h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1204418
+                                                  (00000000001260C2h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         c1444302
-  compressed size:                                784 bytes
-  uncompressed size:                              2635 bytes
-  length of filename:                             58 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
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
 
 Central directory entry #23:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/structural_mechanics_analysis_rom.py
+  KratosRomApplication-9.5.dist-info/top_level.txt
 
-  offset of local header from start of archive:   955036
-                                                  (00000000000E929Ch) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1204632
+                                                  (0000000000126198h) bytes
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
-  32-bit CRC value (hex):                         9c3fffee
-  compressed size:                                1366 bytes
-  uncompressed size:                              4667 bytes
-  length of filename:                             70 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
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
 
 Central directory entry #24:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/structural_mechanics_implicit_dynamic_rom_solver.py
+  KratosRomApplication-9.5.dist-info/RECORD
 
-  offset of local header from start of archive:   956502
-                                                  (00000000000E9856h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1204757
+                                                  (0000000000126215h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         2d82f0fb
-  compressed size:                                796 bytes
-  uncompressed size:                              2193 bytes
-  length of filename:                             85 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:44
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:43 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:43 UTC
+  32-bit CRC value (hex):                         74b58e34
+  compressed size:                                1294 bytes
+  uncompressed size:                              2571 bytes
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
 
 Central directory entry #25:
 ---------------------------
 
-  KratosMultiphysics/RomApplication/structural_mechanics_static_rom_solver.py
+  KratosRomApplication.libs/
 
-  offset of local header from start of archive:   957413
-                                                  (00000000000E9BE5h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1206150
+                                                  (0000000000126786h) bytes
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
-  32-bit CRC value (hex):                         5f600720
-  compressed size:                                757 bytes
-  uncompressed size:                              2054 bytes
-  length of filename:                             75 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:44
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:43 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:43 UTC
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
-
-  There is no file comment.
-
-Central directory entry #26:
----------------------------
-
-  KratosMultiphysics/RomApplication/tsqr.py
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
 
-  offset of local header from start of archive:   958275
-                                                  (00000000000E9F43h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 09:09:32
-  32-bit CRC value (hex):                         a245a9cc
-  compressed size:                                2812 bytes
-  uncompressed size:                              8079 bytes
-  length of filename:                             41 characters
-  length of extra field:                          0 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
-  MS-DOS file attributes (00 hex):                none
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #27:
+Central directory entry #26:
 ---------------------------
 
-  KratosRomApplication-9.4.5.dist-info/METADATA
+  KratosRomApplication.libs/libKratosLinearSolversCore-946bfc3a.so
 
-  offset of local header from start of archive:   961158
-                                                  (00000000000EAA86h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1206234
+                                                  (00000000001267DAh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         5f2e2e3f
-  compressed size:                                557 bytes
-  uncompressed size:                              1377 bytes
-  length of filename:                             45 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         bce5d88c
+  compressed size:                                1056666 bytes
+  uncompressed size:                              4673617 bytes
+  length of filename:                             64 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
-  There is no file comment.
-
-Central directory entry #28:
----------------------------
-
-  KratosRomApplication-9.4.5.dist-info/WHEEL
-
-  offset of local header from start of archive:   961790
-                                                  (00000000000EACFEh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         1ad59a98
-  compressed size:                                96 bytes
-  uncompressed size:                              100 bytes
-  length of filename:                             42 characters
-  length of extra field:                          0 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
-  MS-DOS file attributes (00 hex):                none
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #29:
+Central directory entry #27:
 ---------------------------
 
-  KratosRomApplication-9.4.5.dist-info/top_level.txt
+  KratosRomApplication.libs/libKratosRomCore-f6276baa.so
 
-  offset of local header from start of archive:   961958
-                                                  (00000000000EADA6h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   2263022
+                                                  (00000000002287EEh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         f32d789f
-  compressed size:                                21 bytes
-  uncompressed size:                              19 bytes
-  length of filename:                             50 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:01:36
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:01:36 UTC
+  32-bit CRC value (hex):                         fa3bb123
+  compressed size:                                1561003 bytes
+  uncompressed size:                              6027521 bytes
+  length of filename:                             54 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B600 hex
+  Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
-  There is no file comment.
-
-Central directory entry #30:
----------------------------
-
-  KratosRomApplication-9.4.5.dist-info/RECORD
-
-  offset of local header from start of archive:   962059
-                                                  (00000000000EAE0Bh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 10 10:30:32
-  32-bit CRC value (hex):                         a8e3dbd9
-  compressed size:                                1610 bytes
-  uncompressed size:                              3442 bytes
-  length of filename:                             43 characters
-  length of extra field:                          0 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             01B400 hex
-  MS-DOS file attributes (00 hex):                none
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,91 +1,82 @@
-Filename: KratosMultiphysics/.libs/KratosRomApplication.pyd
+Filename: KratosMultiphysics/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosRomCore.dll
+Filename: KratosMultiphysics/RomApplication/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosRomCore.lib
-Comment: 
-
-Filename: KratosMultiphysics/RomApplication/__init__.py
+Filename: KratosMultiphysics/RomApplication/hrom_training_utility.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/auxiliary_functions_workflow.py
+Filename: KratosMultiphysics/RomApplication/python_solvers_wrapper_rom.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/calculate_rom_basis_output_process.py
+Filename: KratosMultiphysics/RomApplication/rom_manager.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/convection_diffusion_analysis_rom.py
+Filename: KratosMultiphysics/RomApplication/rom_testing_utilities.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/convection_diffusion_stationary_rom_solver.py
+Filename: KratosMultiphysics/RomApplication/tsqr.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/convection_diffusion_transient_rom_solver.py
+Filename: KratosMultiphysics/RomApplication/randomized_singular_value_decomposition.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/empirical_cubature_method.py
+Filename: KratosMultiphysics/RomApplication/rom_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/fluid_dynamics_analysis_rom.py
+Filename: KratosMultiphysics/RomApplication/parallel_svd.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/hrom_training_utility.py
+Filename: KratosMultiphysics/RomApplication/rom_analysis.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/navier_stokes_solver_vmsmonolithic_rom.py
+Filename: KratosMultiphysics/RomApplication/calculate_rom_basis_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/new_python_solvers_wrapper_rom.py
+Filename: KratosMultiphysics/RomApplication/auxiliary_functions_workflow.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/parallel_svd.py
+Filename: KratosMultiphysics/RomApplication/empirical_cubature_method.py
 Comment: 
 
 Filename: KratosMultiphysics/RomApplication/petrov_galerkin_training_utility.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/python_solvers_wrapper_rom.py
-Comment: 
-
-Filename: KratosMultiphysics/RomApplication/randomized_singular_value_decomposition.py
-Comment: 
-
-Filename: KratosMultiphysics/RomApplication/rom_analysis.py
+Filename: KratosMultiphysics/RomApplication/save_rom_coefficients_process.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/rom_manager.py
+Filename: KratosMultiphysics/RomApplication/__init__.py
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/rom_solver.py
+Filename: KratosMultiphysics/.libs/
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/rom_testing_utilities.py
+Filename: KratosMultiphysics/.libs/KratosRomApplication.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/structural_mechanics_analysis_rom.py
+Filename: KratosRomApplication-9.5.dist-info/
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/structural_mechanics_implicit_dynamic_rom_solver.py
+Filename: KratosRomApplication-9.5.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/structural_mechanics_static_rom_solver.py
+Filename: KratosRomApplication-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics/RomApplication/tsqr.py
+Filename: KratosRomApplication-9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosRomApplication-9.4.5.dist-info/METADATA
+Filename: KratosRomApplication-9.5.dist-info/RECORD
 Comment: 
 
-Filename: KratosRomApplication-9.4.5.dist-info/WHEEL
+Filename: KratosRomApplication.libs/
 Comment: 
 
-Filename: KratosRomApplication-9.4.5.dist-info/top_level.txt
+Filename: KratosRomApplication.libs/libKratosLinearSolversCore-946bfc3a.so
 Comment: 
 
-Filename: KratosRomApplication-9.4.5.dist-info/RECORD
+Filename: KratosRomApplication.libs/libKratosRomCore-f6276baa.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## KratosMultiphysics/RomApplication/auxiliary_functions_workflow.py

 * *Ordering differences only*

```diff
@@ -1,20 +1,20 @@
-import dislib as ds
-from dislib.data.array import Array
-
-def load_blocks_array(blocks, shape, block_size):
-    if shape[0] < block_size[0] or  shape[1] < block_size[1]:
-        raise ValueError("The block size is greater than the ds-array")
-    return Array(blocks, shape=shape, top_left_shape=block_size,
-                     reg_shape=block_size, sparse=False)
-
-def load_blocks_rechunk(blocks, shape, block_size, new_block_size):
-    if shape[0] < new_block_size[0] or  shape[1] < new_block_size[1]:
-        raise ValueError("The block size requested for rechunk"
-                         "is greater than the ds-array")
-    final_blocks = [[]]
-    # Este bucle lo puse por si los Future objects se guardan en una lista, en caso de que la forma de guardarlos cambie, también cambiará un poco este bucle.
-    # Si blocks se pasa ya como (p. ej) [[Future_object, Future_object]] no hace falta.
-    for block in blocks:
-        final_blocks[0].append(block)
-    arr = load_blocks_array(final_blocks, shape, block_size)
-    return arr.rechunk(new_block_size)
+import dislib as ds
+from dislib.data.array import Array
+
+def load_blocks_array(blocks, shape, block_size):
+    if shape[0] < block_size[0] or  shape[1] < block_size[1]:
+        raise ValueError("The block size is greater than the ds-array")
+    return Array(blocks, shape=shape, top_left_shape=block_size,
+                     reg_shape=block_size, sparse=False)
+
+def load_blocks_rechunk(blocks, shape, block_size, new_block_size):
+    if shape[0] < new_block_size[0] or  shape[1] < new_block_size[1]:
+        raise ValueError("The block size requested for rechunk"
+                         "is greater than the ds-array")
+    final_blocks = [[]]
+    # Este bucle lo puse por si los Future objects se guardan en una lista, en caso de que la forma de guardarlos cambie, también cambiará un poco este bucle.
+    # Si blocks se pasa ya como (p. ej) [[Future_object, Future_object]] no hace falta.
+    for block in blocks:
+        final_blocks[0].append(block)
+    arr = load_blocks_array(final_blocks, shape, block_size)
+    return arr.rechunk(new_block_size)
```

## KratosMultiphysics/RomApplication/calculate_rom_basis_output_process.py

```diff
@@ -1,211 +1,217 @@
-# Import Python modules
-import json
-import numpy
-from pathlib import Path
-
-# Importing the Kratos Library
-import KratosMultiphysics
-from KratosMultiphysics.RomApplication.randomized_singular_value_decomposition import RandomizedSingularValueDecomposition
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string.")
-    return CalculateRomBasisOutputProcess(model, settings["Parameters"])
-
-class CalculateRomBasisOutputProcess(KratosMultiphysics.OutputProcess):
-    """A process to set the snapshots matrix and calculate the ROM basis from it."""
-
-    def __init__(self, model, settings):
-        KratosMultiphysics.OutputProcess.__init__(self)
-
-        # Validate input settings against defaults
-        settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
-
-        # Get the model part from which the snapshots are to be retrieved
-        if not settings["model_part_name"].GetString():
-            raise Exception("\'model_part_name\' not provided. Please specify the model part to get the snapshots from.")
-        self.model_part = model[settings["model_part_name"].GetString()]
-
-        # Set the snapshots output control and interval
-        snapshots_control_type = settings["snapshots_control_type"].GetString()
-        if snapshots_control_type == "time":
-            self.snapshots_control_is_time = True
-        elif snapshots_control_type == "step":
-            self.snapshots_control_is_time = False
-        else:
-            err_msg = "Unknown value \'{}\' for \'snapshots_control_type\'. Available options are \'time\' and \'step\'.".format(snapshots_control_type)
-            raise Exception(err_msg)
-        self.snapshots_interval = settings["snapshots_interval"].GetDouble()
-
-        # Get the variables list to be used to get the snapshots matrix information
-        # Note that we sort the snapshot variables list alphabetically
-        # This is required in order to establish a consensum for the possible visualization model part projections
-        nodal_unknowns = settings["nodal_unknowns"].GetStringArray()
-        if len(nodal_unknowns) == 0:
-            err_msg = "The snapshots matrix variables need to be specified by the user in the \'nodal_unknowns\' string array."
-            raise Exception(err_msg)
-        if any(nodal_unknowns.count(var_name) > 1 for var_name in nodal_unknowns):
-            err_msg = "There are repeated variables in the \'nodal_unknowns\' string array."
-            raise Exception(err_msg)
-        nodal_unknowns.sort()
-
-        self.snapshot_variables_list = []
-        for var_name in nodal_unknowns:
-            if not KratosMultiphysics.KratosGlobals.HasVariable(var_name):
-                err_msg = "\'{}\' variable in \'nodal_unknowns\' is not in KratosGlobals. Please check provided value.".format(var_name)
-            if not KratosMultiphysics.KratosGlobals.GetVariableType(var_name):
-                err_msg = "\'{}\' variable in \'nodal_unknowns\' is not double type. Please check provide double type variables (e.g. [\"DISPLACEMENT_X\",\"DISPLACEMENT_Y\"]).".format(var_name)
-            self.snapshot_variables_list.append(KratosMultiphysics.KratosGlobals.GetVariable(var_name))
-
-        # Set the ROM basis output settings
-        self.rom_basis_output_format = settings["rom_basis_output_format"].GetString()
-        rom_basis_output_available_formats = ["json", "numpy"]
-        if self.rom_basis_output_format not in rom_basis_output_available_formats:
-            err_msg = "Provided \'rom_basis_output_format\' is {}. Available options are \'json\' and \'numpy\'.".format(self.rom_basis_output_format)
-            raise Exception(err_msg)
-
-        self.rom_basis_output_name = settings["rom_basis_output_name"].GetString()
-
-        self.rom_basis_output_folder = Path(settings["rom_basis_output_folder"].GetString())
-
-        # Get the SVD truncation tolerance
-        self.svd_truncation_tolerance = settings["svd_truncation_tolerance"].GetDouble()
-
-        # Initialize output interval data
-        self.next_output = 0.0
-
-        # Initialize the snapshots data list
-        self.snapshots_data_list = []
-
-        # Set the flag allowing to run multiple simulations using this process #TODO cope with arbitrarily large cases (parallelism)
-        self.rom_manager = settings["rom_manager"].GetBool()
-
-
-    @classmethod
-    def GetDefaultParameters(self):
-        default_settings = KratosMultiphysics.Parameters("""{
-            "help": "A process to set the snapshots matrix and calculate the ROM basis from it.",
-            "model_part_name": "",
-            "rom_manager" : false,
-            "snapshots_control_type": "step",
-            "snapshots_interval": 1.0,
-            "nodal_unknowns": [],
-            "rom_basis_output_format": "numpy",
-            "rom_basis_output_name": "RomParameters",
-            "rom_basis_output_folder" : "rom_data",
-            "svd_truncation_tolerance": 1.0e-6
-        }""")
-
-        return default_settings
-
-    def IsOutputStep(self):
-        if self.snapshots_control_is_time:
-            time = self.__GetPrettyFloat(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
-            return time >= self.__GetPrettyFloat(self.next_output)
-        else:
-            step = self.__GetPrettyFloat(self.model_part.ProcessInfo[KratosMultiphysics.STEP])
-            return step >= self.next_output
-
-    def PrintOutput(self):
-        # Save the data in the snapshots data list
-        aux_data_array = []
-        for node in self.model_part.Nodes:
-            for snapshot_var in self.snapshot_variables_list:
-                aux_data_array.append(node.GetSolutionStepValue(snapshot_var))
-        self.snapshots_data_list.append(aux_data_array)
-
-        # Schedule next snapshot output
-        if self.snapshots_interval > 0.0: # Note: if == 0, we'll just always print
-            if self.snapshots_control_is_time:
-                time = self.__GetPrettyFloat(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
-                while self.__GetPrettyFloat(self.next_output) <= time:
-                    self.next_output += self.snapshots_interval
-            else:
-                step = self.__GetPrettyFloat(self.model_part.ProcessInfo[KratosMultiphysics.STEP])
-                while self.next_output <= step:
-                    self.next_output += self.snapshots_interval
-
-
-    def _GetSnapshotsMatrix(self):
-        snapshots_matrix = numpy.empty((self.n_nodal_unknowns*self.n_nodes,self.n_data_cols))
-        for i_col in range(self.n_data_cols):
-            aux_col = numpy.array(self.snapshots_data_list[i_col])
-            snapshots_matrix[:,i_col] = aux_col.transpose()
-        return snapshots_matrix
-
-
-    def _PrintRomBasis(self, snapshots_matrix):
-        # Initialize the Python dictionary with the default settings
-        # Note that this order is kept if Python 3.6 onwards is used
-        rom_basis_dict = {
-            "rom_manager" : False,
-            "train_hrom": False,
-            "run_hrom": False,
-            "projection_strategy": "galerkin",
-            "assembling_strategy": "global",
-            "rom_format": "numpy",
-            "rom_settings": {
-                "rom_bns_settings": {}
-            },
-            "hrom_settings": {},
-            "nodal_modes": {},
-            "elements_and_weights" : {}
-        }
-        #TODO: I'd rename elements_and_weights to hrom_weights
-
-        if self.rom_manager:
-            rom_basis_dict["rom_manager"] = True
-        rom_basis_dict["hrom_settings"]["hrom_format"] = self.rom_basis_output_format
-        n_nodal_unknowns = len(self.snapshot_variables_list)
-
-        # Calculate the randomized SVD of the snapshots matrix
-        u,_,_,_= RandomizedSingularValueDecomposition().Calculate(snapshots_matrix, self.svd_truncation_tolerance)
-
-        # Save the nodal basis
-        rom_basis_dict["rom_settings"]["nodal_unknowns"] = [var.Name() for var in self.snapshot_variables_list]
-        rom_basis_dict["rom_settings"]["number_of_rom_dofs"] = numpy.shape(u)[1] #TODO: This is way misleading. I'd call it number_of_basis_modes or number_of_rom_modes
-        rom_basis_dict["projection_strategy"] = "galerkin" # Galerkin: (Phi.T@K@Phi dq= Phi.T@b), LSPG = (K@Phi dq= b), Petrov-Galerkin = (Psi.T@K@Phi dq = Psi.T@b)
-        rom_basis_dict["assembling_strategy"] = "global" # Assemble the ROM globally or element by element: "global" (Phi_g @ J_g @ Phi_g), "element by element" sum(Phi_e^T @ K_e @ Phi_e)
-        rom_basis_dict["rom_format"] = self.rom_basis_output_format
-        rom_basis_dict["rom_settings"]["petrov_galerkin_number_of_rom_dofs"] = 0
-        #NOTE "petrov_galerkin_number_of_rom_dofs" is not used unless a Petrov-Galerkin simulation is called, in which case it shall be modified either manually or from the RomManager
-
-        # Create the folder if it doesn't already exist
-        if not self.rom_basis_output_folder.exists():
-            self.rom_basis_output_folder.mkdir(parents=True)
-
-        if self.rom_basis_output_format == "json":
-            # Storing modes in JSON format
-            i = 0
-            for node in self.model_part.Nodes:
-                rom_basis_dict["nodal_modes"][node.Id] = u[i:i+n_nodal_unknowns].tolist()
-                i += n_nodal_unknowns
-
-        elif self.rom_basis_output_format == "numpy":
-            # Storing modes in Numpy format
-            numpy.save(self.rom_basis_output_folder / "RightBasisMatrix.npy", u)
-            numpy.save(self.rom_basis_output_folder / "NodeIds.npy", numpy.arange(1,((u.shape[0]+1)/n_nodal_unknowns), 1, dtype=int))
-        else:
-            err_msg = "Unsupported output format {}.".format(self.rom_basis_output_format)
-            raise Exception(err_msg)
-
-        # Creating the ROM JSON file containing or not the modes depending on "self.rom_basis_output_format"
-        output_filename = self.rom_basis_output_folder / f"{self.rom_basis_output_name}.json"
-        with output_filename.open('w') as f:
-            json.dump(rom_basis_dict, f, indent = 4)
-
-
-
-    def ExecuteFinalize(self):
-        # Prepare a NumPy array with the snapshots data
-        self.n_nodes = self.model_part.NumberOfNodes()
-        self.n_data_cols = len(self.snapshots_data_list)
-        self.n_nodal_unknowns = len(self.snapshot_variables_list)
-
-        if not self.rom_manager:
-            self._PrintRomBasis(self._GetSnapshotsMatrix())
-
-    def __GetPrettyFloat(self, number):
-        float_format = "{:.12f}"
-        pretty_number = float(float_format.format(number))
+# Import Python modules
+import json
+import numpy
+from pathlib import Path
+
+# Importing the Kratos Library
+import KratosMultiphysics
+from KratosMultiphysics.RomApplication.randomized_singular_value_decomposition import RandomizedSingularValueDecomposition
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string.")
+    return CalculateRomBasisOutputProcess(model, settings["Parameters"])
+
+class CalculateRomBasisOutputProcess(KratosMultiphysics.OutputProcess):
+    """A process to set the snapshots matrix and calculate the ROM basis from it."""
+
+    def __init__(self, model, settings):
+        KratosMultiphysics.OutputProcess.__init__(self)
+
+        # Validate input settings against defaults
+        settings.ValidateAndAssignDefaults(self.GetDefaultParameters())
+
+        # Get the model part from which the snapshots are to be retrieved
+        if not settings["model_part_name"].GetString():
+            raise Exception("\'model_part_name\' not provided. Please specify the model part to get the snapshots from.")
+        self.model_part = model[settings["model_part_name"].GetString()]
+
+        # Set the snapshots output control and interval
+        snapshots_control_type = settings["snapshots_control_type"].GetString()
+        if snapshots_control_type == "time":
+            self.snapshots_control_is_time = True
+        elif snapshots_control_type == "step":
+            self.snapshots_control_is_time = False
+        else:
+            err_msg = "Unknown value \'{}\' for \'snapshots_control_type\'. Available options are \'time\' and \'step\'.".format(snapshots_control_type)
+            raise Exception(err_msg)
+        self.snapshots_interval = settings["snapshots_interval"].GetDouble()
+
+        # Get the variables list to be used to get the snapshots matrix information
+        # Note that we sort the snapshot variables list alphabetically
+        # This is required in order to establish a consensum for the possible visualization model part projections
+        nodal_unknowns = settings["nodal_unknowns"].GetStringArray()
+        if len(nodal_unknowns) == 0:
+            err_msg = "The snapshots matrix variables need to be specified by the user in the \'nodal_unknowns\' string array."
+            raise Exception(err_msg)
+        if any(nodal_unknowns.count(var_name) > 1 for var_name in nodal_unknowns):
+            err_msg = "There are repeated variables in the \'nodal_unknowns\' string array."
+            raise Exception(err_msg)
+        nodal_unknowns.sort()
+
+        self.snapshot_variables_list = []
+        for var_name in nodal_unknowns:
+            if not KratosMultiphysics.KratosGlobals.HasVariable(var_name):
+                err_msg = "\'{}\' variable in \'nodal_unknowns\' is not in KratosGlobals. Please check provided value.".format(var_name)
+            if not KratosMultiphysics.KratosGlobals.GetVariableType(var_name):
+                err_msg = "\'{}\' variable in \'nodal_unknowns\' is not double type. Please check provide double type variables (e.g. [\"DISPLACEMENT_X\",\"DISPLACEMENT_Y\"]).".format(var_name)
+            self.snapshot_variables_list.append(KratosMultiphysics.KratosGlobals.GetVariable(var_name))
+
+        # Set the ROM basis output settings
+        self.rom_basis_output_format = settings["rom_basis_output_format"].GetString()
+        rom_basis_output_available_formats = ["json", "numpy"]
+        if self.rom_basis_output_format not in rom_basis_output_available_formats:
+            err_msg = "Provided \'rom_basis_output_format\' is {}. Available options are \'json\' and \'numpy\'.".format(self.rom_basis_output_format)
+            raise Exception(err_msg)
+
+        self.rom_basis_output_name = settings["rom_basis_output_name"].GetString()
+
+        self.rom_basis_output_folder = Path(settings["rom_basis_output_folder"].GetString())
+
+        # Get the SVD truncation tolerance
+        self.svd_truncation_tolerance = settings["svd_truncation_tolerance"].GetDouble()
+
+        # Initialize output interval data
+        self.next_output = 0.0
+
+        # Initialize the snapshots data list
+        self.snapshots_data_list = []
+
+        # Set the flag allowing to run multiple simulations using this process #TODO cope with arbitrarily large cases (parallelism)
+        self.rom_manager = settings["rom_manager"].GetBool()
+
+
+    @classmethod
+    def GetDefaultParameters(self):
+        default_settings = KratosMultiphysics.Parameters("""{
+            "help": "A process to set the snapshots matrix and calculate the ROM basis from it.",
+            "model_part_name": "",
+            "rom_manager" : false,
+            "snapshots_control_type": "step",
+            "snapshots_interval": 1.0,
+            "nodal_unknowns": [],
+            "rom_basis_output_format": "numpy",
+            "rom_basis_output_name": "RomParameters",
+            "rom_basis_output_folder" : "rom_data",
+            "svd_truncation_tolerance": 1.0e-6
+        }""")
+
+        return default_settings
+
+    def IsOutputStep(self):
+        if self.snapshots_control_is_time:
+            time = self.__GetPrettyFloat(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
+            return time >= self.__GetPrettyFloat(self.next_output)
+        else:
+            step = self.__GetPrettyFloat(self.model_part.ProcessInfo[KratosMultiphysics.STEP])
+            return step >= self.next_output
+
+    def PrintOutput(self):
+        # Save the data in the snapshots data list
+        aux_data_array = []
+        for snapshot_var in self.snapshot_variables_list:
+            aux_data_array.append( numpy.array(KratosMultiphysics.VariableUtils().GetSolutionStepValuesVector(self.model_part.Nodes, snapshot_var, 0), copy=False ))
+        self.snapshots_data_list.append(numpy.stack(aux_data_array, axis=1).reshape(-1,1))
+
+
+        # Schedule next snapshot output
+        if self.snapshots_interval > 0.0: # Note: if == 0, we'll just always print
+            if self.snapshots_control_is_time:
+                time = self.__GetPrettyFloat(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
+                while self.__GetPrettyFloat(self.next_output) <= time:
+                    self.next_output += self.snapshots_interval
+            else:
+                step = self.__GetPrettyFloat(self.model_part.ProcessInfo[KratosMultiphysics.STEP])
+                while self.next_output <= step:
+                    self.next_output += self.snapshots_interval
+
+
+    def _GetSnapshotsMatrix(self):
+        return numpy.block(self.snapshots_data_list)
+
+
+    def _ComputeSVD(self, snapshots_matrix):
+
+        # Calculate the randomized SVD of the snapshots matrix
+        u,_,_,_= RandomizedSingularValueDecomposition().Calculate(snapshots_matrix, self.svd_truncation_tolerance)
+
+        return u
+
+
+    def _PrintRomBasis(self, u):
+        # Initialize the Python dictionary with the default settings
+        # Note that this order is kept if Python 3.6 onwards is used
+        rom_basis_dict = {
+            "rom_manager" : False,
+            "train_hrom": False,
+            "run_hrom": False,
+            "projection_strategy": "galerkin",
+            "assembling_strategy": "global",
+            "rom_format": "numpy",
+            "rom_settings": {
+                "rom_bns_settings": {}
+            },
+            "hrom_settings": {},
+            "nodal_modes": {},
+            "elements_and_weights" : {}
+        }
+        #TODO: I'd rename elements_and_weights to hrom_weights
+
+        if self.rom_manager:
+            rom_basis_dict["rom_manager"] = True
+        rom_basis_dict["hrom_settings"]["hrom_format"] = self.rom_basis_output_format
+        n_nodal_unknowns = len(self.snapshot_variables_list)
+
+        # Save the nodal basis
+        rom_basis_dict["rom_settings"]["nodal_unknowns"] = [var.Name() for var in self.snapshot_variables_list]
+        rom_basis_dict["rom_settings"]["number_of_rom_dofs"] = numpy.shape(u)[1] #TODO: This is way misleading. I'd call it number_of_basis_modes or number_of_rom_modes
+        rom_basis_dict["projection_strategy"] = "galerkin" # Galerkin: (Phi.T@K@Phi dq= Phi.T@b), LSPG = (K@Phi dq= b), Petrov-Galerkin = (Psi.T@K@Phi dq = Psi.T@b)
+        rom_basis_dict["assembling_strategy"] = "global" # Assemble the ROM globally or element by element: "global" (Phi_g @ J_g @ Phi_g), "element by element" sum(Phi_e^T @ K_e @ Phi_e)
+        rom_basis_dict["rom_format"] = self.rom_basis_output_format
+        rom_basis_dict["rom_settings"]["petrov_galerkin_number_of_rom_dofs"] = 0
+        #NOTE "petrov_galerkin_number_of_rom_dofs" is not used unless a Petrov-Galerkin simulation is called, in which case it shall be modified either manually or from the RomManager
+
+        # Create the folder if it doesn't already exist
+        if not self.rom_basis_output_folder.exists():
+            self.rom_basis_output_folder.mkdir(parents=True)
+
+        if self.rom_basis_output_format == "json":
+            # Storing modes in JSON format
+            i = 0
+            for node in self.model_part.Nodes:
+                rom_basis_dict["nodal_modes"][node.Id] = u[i:i+n_nodal_unknowns].tolist()
+                i += n_nodal_unknowns
+
+        elif self.rom_basis_output_format == "numpy":
+            # Storing modes in Numpy format
+            node_ids = []
+            for node in self.model_part.Nodes:
+                node_ids.append(node.Id)
+            node_ids = numpy.array(node_ids)
+            numpy.save(self.rom_basis_output_folder / "RightBasisMatrix.npy", u)
+            numpy.save(self.rom_basis_output_folder / "NodeIds.npy", node_ids)
+        else:
+            err_msg = "Unsupported output format {}.".format(self.rom_basis_output_format)
+            raise Exception(err_msg)
+
+        # Creating the ROM JSON file containing or not the modes depending on "self.rom_basis_output_format"
+        output_filename = self.rom_basis_output_folder / f"{self.rom_basis_output_name}.json"
+        with output_filename.open('w') as f:
+            json.dump(rom_basis_dict, f, indent = 4)
+
+
+
+    def ExecuteFinalize(self):
+        # Prepare a NumPy array with the snapshots data
+        self.n_nodes = self.model_part.NumberOfNodes()
+        self.n_data_cols = len(self.snapshots_data_list)
+        self.n_nodal_unknowns = len(self.snapshot_variables_list)
+
+        if not self.rom_manager:
+            u = self._ComputeSVD(self._GetSnapshotsMatrix())
+            self._PrintRomBasis(u)
+
+    def __GetPrettyFloat(self, number):
+        float_format = "{:.12f}"
+        pretty_number = float(float_format.format(number))
         return pretty_number
```

## KratosMultiphysics/RomApplication/empirical_cubature_method.py

 * *Ordering differences only*

```diff
@@ -1,290 +1,290 @@
-import numpy as np
-from KratosMultiphysics import Logger
-
-try:
-    from matplotlib import pyplot as plt
-    missing_matplotlib = False
-except ImportError as e:
-    missing_matplotlib = True
-
-
-class EmpiricalCubatureMethod():
-    """
-    This class selects a subset of elements and corresponding positive weights necessary for the construction of a hyper-reduced order model
-    Reference: Hernandez 2020. "A multiscale method for periodic structures using domain decomposition and ECM-hyperreduction"
-    """
-
-    def __init__(
-        self,
-        ECM_tolerance = 0,
-        Filter_tolerance = 0,
-        Plotting = False,
-        MaximumNumberUnsuccesfulIterations = 100
-    ):
-        """
-        Constructor setting up the parameters for the Element Selection Strategy
-            ECM_tolerance: approximation tolerance for the element selection algorithm
-            Filter_tolerance: parameter limiting the number of candidate points (elements) to those above this tolerance
-            Plotting: whether to plot the error evolution of the element selection algorithm
-        """
-        self.ECM_tolerance = ECM_tolerance
-        self.Filter_tolerance = Filter_tolerance
-        self.Name = "EmpiricalCubature"
-        self.Plotting = Plotting
-        self.MaximumNumberUnsuccesfulIterations = MaximumNumberUnsuccesfulIterations
-
-    def SetUp(
-        self,
-        ResidualsBasis,
-        InitialCandidatesSet = None,
-        constrain_sum_of_weights=True,
-        constrain_conditions = False,
-        number_of_conditions = 0
-    ):
-        """
-        Method for setting up the element selection
-        input:  - ResidualsBasis: numpy array containing a basis to the residuals projected
-                - constrain_sum_of_weights: enable the user to constrain weights to be the sum of the number of entities.
-                - constrain_conditions: enable the user to enforce weights to consider conditions (for specific boundary conditions).
-        """
-        self.W = np.ones(np.shape(ResidualsBasis)[0])
-        self.G = ResidualsBasis.T
-        self.y = InitialCandidatesSet
-        self.add_constrain_count = None
-        total_number_of_entities = np.shape(self.G)[1]
-        elements_constraint = np.ones(total_number_of_entities)
-        conditions_begin = total_number_of_entities - number_of_conditions
-        elements_constraint[conditions_begin:] = 0
-
-        if constrain_sum_of_weights and not constrain_conditions:
-            """
-            -This is necessary in case the sum of the columns of self.G equals the 0 vector,to avoid the trivial solution
-            -It is enforcing that the sum of the weights equals the number of columns in self.G (total number of elements)
-            """
-            projection_of_constant_vector_elements = elements_constraint - self.G.T@( self.G @ elements_constraint)
-            projection_of_constant_vector_elements/= np.linalg.norm(projection_of_constant_vector_elements)
-            self.G = np.vstack([ self.G , projection_of_constant_vector_elements] )
-            self.add_constrain_count = -1
-        elif constrain_sum_of_weights and constrain_conditions:#Only for models which contains conditions
-            projection_of_constant_vector_elements = elements_constraint - self.G.T@( self.G @ elements_constraint)
-            projection_of_constant_vector_elements/= np.linalg.norm(projection_of_constant_vector_elements)
-            self.G = np.vstack([ self.G , projection_of_constant_vector_elements] )
-            # # # # # # # # #
-            conditions_constraint = np.ones(total_number_of_entities)
-            conditions_constraint[:conditions_begin] = 0
-            projection_of_constant_vector_conditions = conditions_constraint - self.G.T@( self.G @ conditions_constraint)
-            projection_of_constant_vector_conditions/= np.linalg.norm(projection_of_constant_vector_conditions)
-            self.G = np.vstack([ self.G , projection_of_constant_vector_conditions ] )
-            self.add_constrain_count = -2
-        self.b = self.G @ self.W
-        self.UnsuccesfulIterations = 0
-
-    def Initialize(self):
-        """
-        Method performing calculations required before launching the Calculate method
-        """
-        self.GnormNOONE = np.linalg.norm(self.G[:self.add_constrain_count,:], axis = 0)
-        M = np.shape(self.G)[1]
-        normB = np.linalg.norm(self.b)
-
-        if self.y is None:
-            self.y = np.arange(0,M,1) # Set of candidate points (those whose associated column has low norm are removed)
-
-            if self.Filter_tolerance > 0:
-                TOL_REMOVE = self.Filter_tolerance * normB
-                rmvpin = np.where(self.GnormNOONE[self.y] < TOL_REMOVE)
-                #self.y_complement = self.y[rmvpin]
-                self.y = np.delete(self.y,rmvpin)
-        else:
-            self.y_complement = np.arange(0, M, 1)  # Initialize complement with all points
-            self.y_complement = np.delete(self.y_complement, self.y)  # Remove candidates from complement
-
-            if self.Filter_tolerance > 0:
-                TOL_REMOVE = self.Filter_tolerance * normB  # Compute removal tolerance
-
-                # Filter out low-norm columns from complement
-                rmvpin_complement = np.where(self.GnormNOONE[self.y_complement] < TOL_REMOVE)
-                self.y_complement = np.delete(self.y_complement, rmvpin_complement)
-
-                # Filter out low-norm columns from candidates
-                rmvpin = np.where(self.GnormNOONE[self.y] < TOL_REMOVE)
-                removed_count = np.size(rmvpin)
-                self.y = np.delete(self.y, rmvpin)
-
-                # Warning if some candidates were removed
-                if removed_count > 0:
-                    Logger.PrintWarning("EmpiricalCubatureMethod", f"Some of the candidates were removed ({removed_count} removed). To include all candidates (with 0 weights in the HROM model part) for visualization and projection, consider using 'include_elements_model_parts_list' and 'include_conditions_model_parts_list' in the 'hrom_settings'.")
-
-                # Warning if all candidates were removed
-                if np.size(self.y) == 0:
-                    Logger.PrintWarning("EmpiricalCubatureMethod", "All candidates were removed because they have no contribution to the residual. To include them all (with 0 weights in the HROM model part) for visualization and projection, use 'include_elements_model_parts_list' and 'include_conditions_model_parts_list' in the 'hrom_settings'.")
-                    self.y = self.y_complement  # Set candidates to complement
-
-        self.z = {}  # Set of intergration points
-        self.mPOS = 0 # Number of nonzero weights
-        self.r = self.b.copy() # residual vector
-        self.m = len(self.b) # Default number of points
-        self.nerror = np.linalg.norm(self.r)/normB
-        self.nerrorACTUAL = self.nerror
-
-    def Run(self):
-        self.Initialize()
-        self.Calculate()
-
-    def expand_candidates_with_complement(self):
-        self.y = np.r_[self.y,self.y_complement]
-        print('expanding set to include the complement...')
-        ExpandedSetFlag = True
-        return ExpandedSetFlag
-
-    def Calculate(self):
-        """
-        Method launching the element selection algorithm to find a set of elements: self.z, and wiegths: self.w
-        """
-        MaximumLengthZ = 0
-        ExpandedSetFlag = False
-        k = 1 # number of iterations
-        self.success = True
-        while self.nerrorACTUAL > self.ECM_tolerance and self.mPOS < self.m and np.size(self.y) != 0:
-
-            if  self.UnsuccesfulIterations >  self.MaximumNumberUnsuccesfulIterations and not ExpandedSetFlag and hasattr(self, 'y_complement'):
-                ExpandedSetFlag = self.expand_candidates_with_complement()
-
-            #Step 1. Compute new point
-            if np.size(self.y)==1:
-                #candidate set consists of a single element
-                indSORT = 0
-                i = int(self.y)
-            else:
-                ObjFun = self.G[:,self.y].T @ self.r.T
-                ObjFun = ObjFun.T #/ self.GnormNOONE[self.y]
-                indSORT = np.argmax(ObjFun)
-                i = self.y[indSORT]
-            if k==1:
-                alpha = np.linalg.lstsq(self.G[:, [i]], self.b)[0]
-                H = 1/(self.G[:,i] @ self.G[:,i].T)
-            else:
-                H, alpha = self._UpdateWeightsInverse(self.G[:,self.z],H,self.G[:,i],alpha)
-
-            #Step 3. Move i from set y to set z
-            if k == 1:
-                self.z = i
-            else:
-                self.z = np.r_[self.z,i]
-
-            #self.y = np.delete(self.y,indSORT)
-            if np.size(self.y)==1:
-                if hasattr(self, 'y_complement'):
-                    self.expand_candidates_with_complement()
-                    self.y = np.delete(self.y,indSORT)
-                else:
-                    self.success = False
-                    break
-            else:
-                self.y = np.delete(self.y,indSORT)
-
-            # Step 4. Find possible negative weights
-            if any(alpha < 0):
-                print("WARNING: NEGATIVE weight found")
-                indexes_neg_weight = np.where(alpha <= 0.)[0]
-                self.y = np.append(self.y, (self.z[indexes_neg_weight]).T)
-                self.z = np.delete(self.z, indexes_neg_weight)
-                H = self._MultiUpdateInverseHermitian(H, indexes_neg_weight)
-                alpha = H @ (self.G[:, self.z].T @ self.b)
-                alpha = alpha.reshape(len(alpha),1)
-
-            if np.size(self.z) > MaximumLengthZ :
-                self.UnsuccesfulIterations = 0
-            else:
-                self.UnsuccesfulIterations += 1
-
-            #Step 6 Update the residual
-            if np.size(alpha)==1:
-                self.r = self.b.reshape(-1,1) - (self.G[:,self.z] * alpha).reshape(-1,1)
-                self.r = np.squeeze(self.r)
-            else:
-                Aux = self.G[:,self.z] @ alpha
-                self.r = np.squeeze(self.b - Aux.T)
-            self.nerror = np.linalg.norm(self.r) / np.linalg.norm(self.b)  # Relative error (using r and b)
-            self.nerrorACTUAL = self.nerror
-
-            # STEP 7
-            self.mPOS = np.size(self.z)
-            print(f'k = {k}, m = {np.size(self.z)}, error n(res)/n(b) (%) = {self.nerror*100},  Actual error % = {self.nerrorACTUAL*100} ')
-
-            if k == 1:
-                ERROR_GLO = np.array([self.nerrorACTUAL])
-                NPOINTS = np.array([np.size(self.z)])
-            else:
-                ERROR_GLO = np.c_[ ERROR_GLO , self.nerrorACTUAL]
-                NPOINTS = np.c_[ NPOINTS , np.size(self.z)]
-
-            MaximumLengthZ = max(MaximumLengthZ, np.size(self.z))
-            k = k+1
-
-            if k-MaximumLengthZ>1000 and ExpandedSetFlag:
-                """
-                this means using the initial candidate set, it was impossible to obtain a set of positive weights.
-                Try again without constraints!!!
-                TODO: incorporate this into greater workflow
-                """
-                self.success = False
-                break
-
-        self.w = alpha.T * np.sqrt(self.W[self.z]) #TODO FIXME cope with weights vectors different from 1
-
-        print(f'Total number of iterations = {k}')
-
-        if missing_matplotlib == False and self.Plotting == True:
-            plt.plot(NPOINTS[0], ERROR_GLO[0])
-            plt.title('Element Selection Error Evolution')
-            plt.xlabel('Number of elements')
-            plt.ylabel('Error %')
-            plt.show()
-
-    def _UpdateWeightsInverse(self, A,Aast,a,xold):
-        """
-        Method for the quick update of weights (self.w), whenever a negative weight is found
-        """
-        c = np.dot(A.T, a)
-        d = np.dot(Aast, c).reshape(-1, 1)
-        s = np.dot(a.T, a) - np.dot(c.T, d)
-        aux1 = np.hstack([Aast + np.outer(d, d) / s, -d / s])
-        if np.shape(-d.T / s)[1]==1:
-            s = s.reshape(1,-1)
-            aux2 = np.squeeze(np.hstack([-d.T / s, 1 / s]))
-        else:
-            aux2 = np.hstack([np.squeeze(-d.T / s), 1 / s])
-        Bast = np.vstack([aux1, aux2])
-        v = np.dot(a.T, self.r) / s
-        x = np.vstack([(xold - d * v), v])
-        return Bast, x
-
-    def _MultiUpdateInverseHermitian(self, invH, neg_indexes):
-        """
-        Method for the quick update of weights (self.w), whenever a negative weight is found
-        """
-        neg_indexes = np.sort(neg_indexes)
-        for i in range(np.size(neg_indexes)):
-            neg_index = neg_indexes[i] - i
-            invH = self._UpdateInverseHermitian(invH, neg_index)
-        return invH
-
-    def _UpdateInverseHermitian(self, invH, neg_index):
-        """
-        Method for the quick update of weights (self.w), whenever a negative weight is found
-        """
-        if neg_index == np.shape(invH)[1]:
-            aux = (invH[0:-1, -1] * invH[-1, 0:-1]) / invH(-1, -1)
-            invH_new = invH[:-1, :-1] - aux
-        else:
-            aux1 = np.hstack([invH[:, 0:neg_index], invH[:, neg_index + 1:], invH[:, neg_index].reshape(-1, 1)])
-            aux2 = np.vstack([aux1[0:neg_index, :], aux1[neg_index + 1:, :], aux1[neg_index, :]])
-            invH_new = aux2[0:-1, 0:-1] - np.outer(aux2[0:-1, -1], aux2[-1, 0:-1]) / aux2[-1, -1]
-        return invH_new
-
-
-
-
-
-
+import numpy as np
+from KratosMultiphysics import Logger
+
+try:
+    from matplotlib import pyplot as plt
+    missing_matplotlib = False
+except ImportError as e:
+    missing_matplotlib = True
+
+
+class EmpiricalCubatureMethod():
+    """
+    This class selects a subset of elements and corresponding positive weights necessary for the construction of a hyper-reduced order model
+    Reference: Hernandez 2020. "A multiscale method for periodic structures using domain decomposition and ECM-hyperreduction"
+    """
+
+    def __init__(
+        self,
+        ECM_tolerance = 0,
+        Filter_tolerance = 0,
+        Plotting = False,
+        MaximumNumberUnsuccesfulIterations = 100
+    ):
+        """
+        Constructor setting up the parameters for the Element Selection Strategy
+            ECM_tolerance: approximation tolerance for the element selection algorithm
+            Filter_tolerance: parameter limiting the number of candidate points (elements) to those above this tolerance
+            Plotting: whether to plot the error evolution of the element selection algorithm
+        """
+        self.ECM_tolerance = ECM_tolerance
+        self.Filter_tolerance = Filter_tolerance
+        self.Name = "EmpiricalCubature"
+        self.Plotting = Plotting
+        self.MaximumNumberUnsuccesfulIterations = MaximumNumberUnsuccesfulIterations
+
+    def SetUp(
+        self,
+        ResidualsBasis,
+        InitialCandidatesSet = None,
+        constrain_sum_of_weights=True,
+        constrain_conditions = False,
+        number_of_conditions = 0
+    ):
+        """
+        Method for setting up the element selection
+        input:  - ResidualsBasis: numpy array containing a basis to the residuals projected
+                - constrain_sum_of_weights: enable the user to constrain weights to be the sum of the number of entities.
+                - constrain_conditions: enable the user to enforce weights to consider conditions (for specific boundary conditions).
+        """
+        self.W = np.ones(np.shape(ResidualsBasis)[0])
+        self.G = ResidualsBasis.T
+        self.y = InitialCandidatesSet
+        self.add_constrain_count = None
+        total_number_of_entities = np.shape(self.G)[1]
+        elements_constraint = np.ones(total_number_of_entities)
+        conditions_begin = total_number_of_entities - number_of_conditions
+        elements_constraint[conditions_begin:] = 0
+
+        if constrain_sum_of_weights and not constrain_conditions:
+            """
+            -This is necessary in case the sum of the columns of self.G equals the 0 vector,to avoid the trivial solution
+            -It is enforcing that the sum of the weights equals the number of columns in self.G (total number of elements)
+            """
+            projection_of_constant_vector_elements = elements_constraint - self.G.T@( self.G @ elements_constraint)
+            projection_of_constant_vector_elements/= np.linalg.norm(projection_of_constant_vector_elements)
+            self.G = np.vstack([ self.G , projection_of_constant_vector_elements] )
+            self.add_constrain_count = -1
+        elif constrain_sum_of_weights and constrain_conditions:#Only for models which contains conditions
+            projection_of_constant_vector_elements = elements_constraint - self.G.T@( self.G @ elements_constraint)
+            projection_of_constant_vector_elements/= np.linalg.norm(projection_of_constant_vector_elements)
+            self.G = np.vstack([ self.G , projection_of_constant_vector_elements] )
+            # # # # # # # # #
+            conditions_constraint = np.ones(total_number_of_entities)
+            conditions_constraint[:conditions_begin] = 0
+            projection_of_constant_vector_conditions = conditions_constraint - self.G.T@( self.G @ conditions_constraint)
+            projection_of_constant_vector_conditions/= np.linalg.norm(projection_of_constant_vector_conditions)
+            self.G = np.vstack([ self.G , projection_of_constant_vector_conditions ] )
+            self.add_constrain_count = -2
+        self.b = self.G @ self.W
+        self.UnsuccesfulIterations = 0
+
+    def Initialize(self):
+        """
+        Method performing calculations required before launching the Calculate method
+        """
+        self.GnormNOONE = np.linalg.norm(self.G[:self.add_constrain_count,:], axis = 0)
+        M = np.shape(self.G)[1]
+        normB = np.linalg.norm(self.b)
+
+        if self.y is None:
+            self.y = np.arange(0,M,1) # Set of candidate points (those whose associated column has low norm are removed)
+
+            if self.Filter_tolerance > 0:
+                TOL_REMOVE = self.Filter_tolerance * normB
+                rmvpin = np.where(self.GnormNOONE[self.y] < TOL_REMOVE)
+                #self.y_complement = self.y[rmvpin]
+                self.y = np.delete(self.y,rmvpin)
+        else:
+            self.y_complement = np.arange(0, M, 1)  # Initialize complement with all points
+            self.y_complement = np.delete(self.y_complement, self.y)  # Remove candidates from complement
+
+            if self.Filter_tolerance > 0:
+                TOL_REMOVE = self.Filter_tolerance * normB  # Compute removal tolerance
+
+                # Filter out low-norm columns from complement
+                rmvpin_complement = np.where(self.GnormNOONE[self.y_complement] < TOL_REMOVE)
+                self.y_complement = np.delete(self.y_complement, rmvpin_complement)
+
+                # Filter out low-norm columns from candidates
+                rmvpin = np.where(self.GnormNOONE[self.y] < TOL_REMOVE)
+                removed_count = np.size(rmvpin)
+                self.y = np.delete(self.y, rmvpin)
+
+                # Warning if some candidates were removed
+                if removed_count > 0:
+                    Logger.PrintWarning("EmpiricalCubatureMethod", f"Some of the candidates were removed ({removed_count} removed). To include all candidates (with 0 weights in the HROM model part) for visualization and projection, consider using 'include_elements_model_parts_list' and 'include_conditions_model_parts_list' in the 'hrom_settings'.")
+
+                # Warning if all candidates were removed
+                if np.size(self.y) == 0:
+                    Logger.PrintWarning("EmpiricalCubatureMethod", "All candidates were removed because they have no contribution to the residual. To include them all (with 0 weights in the HROM model part) for visualization and projection, use 'include_elements_model_parts_list' and 'include_conditions_model_parts_list' in the 'hrom_settings'.")
+                    self.y = self.y_complement  # Set candidates to complement
+
+        self.z = {}  # Set of intergration points
+        self.mPOS = 0 # Number of nonzero weights
+        self.r = self.b.copy() # residual vector
+        self.m = len(self.b) # Default number of points
+        self.nerror = np.linalg.norm(self.r)/normB
+        self.nerrorACTUAL = self.nerror
+
+    def Run(self):
+        self.Initialize()
+        self.Calculate()
+
+    def expand_candidates_with_complement(self):
+        self.y = np.r_[self.y,self.y_complement]
+        print('expanding set to include the complement...')
+        ExpandedSetFlag = True
+        return ExpandedSetFlag
+
+    def Calculate(self):
+        """
+        Method launching the element selection algorithm to find a set of elements: self.z, and wiegths: self.w
+        """
+        MaximumLengthZ = 0
+        ExpandedSetFlag = False
+        k = 1 # number of iterations
+        self.success = True
+        while self.nerrorACTUAL > self.ECM_tolerance and self.mPOS < self.m and np.size(self.y) != 0:
+
+            if  self.UnsuccesfulIterations >  self.MaximumNumberUnsuccesfulIterations and not ExpandedSetFlag and hasattr(self, 'y_complement'):
+                ExpandedSetFlag = self.expand_candidates_with_complement()
+
+            #Step 1. Compute new point
+            if np.size(self.y)==1:
+                #candidate set consists of a single element
+                indSORT = 0
+                i = int(self.y)
+            else:
+                ObjFun = self.G[:,self.y].T @ self.r.T
+                ObjFun = ObjFun.T #/ self.GnormNOONE[self.y]
+                indSORT = np.argmax(ObjFun)
+                i = self.y[indSORT]
+            if k==1:
+                alpha = np.linalg.lstsq(self.G[:, [i]], self.b)[0]
+                H = 1/(self.G[:,i] @ self.G[:,i].T)
+            else:
+                H, alpha = self._UpdateWeightsInverse(self.G[:,self.z],H,self.G[:,i],alpha)
+
+            #Step 3. Move i from set y to set z
+            if k == 1:
+                self.z = i
+            else:
+                self.z = np.r_[self.z,i]
+
+            #self.y = np.delete(self.y,indSORT)
+            if np.size(self.y)==1:
+                if hasattr(self, 'y_complement'):
+                    self.expand_candidates_with_complement()
+                    self.y = np.delete(self.y,indSORT)
+                else:
+                    self.success = False
+                    break
+            else:
+                self.y = np.delete(self.y,indSORT)
+
+            # Step 4. Find possible negative weights
+            if any(alpha < 0):
+                print("WARNING: NEGATIVE weight found")
+                indexes_neg_weight = np.where(alpha <= 0.)[0]
+                self.y = np.append(self.y, (self.z[indexes_neg_weight]).T)
+                self.z = np.delete(self.z, indexes_neg_weight)
+                H = self._MultiUpdateInverseHermitian(H, indexes_neg_weight)
+                alpha = H @ (self.G[:, self.z].T @ self.b)
+                alpha = alpha.reshape(len(alpha),1)
+
+            if np.size(self.z) > MaximumLengthZ :
+                self.UnsuccesfulIterations = 0
+            else:
+                self.UnsuccesfulIterations += 1
+
+            #Step 6 Update the residual
+            if np.size(alpha)==1:
+                self.r = self.b.reshape(-1,1) - (self.G[:,self.z] * alpha).reshape(-1,1)
+                self.r = np.squeeze(self.r)
+            else:
+                Aux = self.G[:,self.z] @ alpha
+                self.r = np.squeeze(self.b - Aux.T)
+            self.nerror = np.linalg.norm(self.r) / np.linalg.norm(self.b)  # Relative error (using r and b)
+            self.nerrorACTUAL = self.nerror
+
+            # STEP 7
+            self.mPOS = np.size(self.z)
+            print(f'k = {k}, m = {np.size(self.z)}, error n(res)/n(b) (%) = {self.nerror*100},  Actual error % = {self.nerrorACTUAL*100} ')
+
+            if k == 1:
+                ERROR_GLO = np.array([self.nerrorACTUAL])
+                NPOINTS = np.array([np.size(self.z)])
+            else:
+                ERROR_GLO = np.c_[ ERROR_GLO , self.nerrorACTUAL]
+                NPOINTS = np.c_[ NPOINTS , np.size(self.z)]
+
+            MaximumLengthZ = max(MaximumLengthZ, np.size(self.z))
+            k = k+1
+
+            if k-MaximumLengthZ>1000 and ExpandedSetFlag:
+                """
+                this means using the initial candidate set, it was impossible to obtain a set of positive weights.
+                Try again without constraints!!!
+                TODO: incorporate this into greater workflow
+                """
+                self.success = False
+                break
+
+        self.w = alpha.T * np.sqrt(self.W[self.z]) #TODO FIXME cope with weights vectors different from 1
+
+        print(f'Total number of iterations = {k}')
+
+        if missing_matplotlib == False and self.Plotting == True:
+            plt.plot(NPOINTS[0], ERROR_GLO[0])
+            plt.title('Element Selection Error Evolution')
+            plt.xlabel('Number of elements')
+            plt.ylabel('Error %')
+            plt.show()
+
+    def _UpdateWeightsInverse(self, A,Aast,a,xold):
+        """
+        Method for the quick update of weights (self.w), whenever a negative weight is found
+        """
+        c = np.dot(A.T, a)
+        d = np.dot(Aast, c).reshape(-1, 1)
+        s = np.dot(a.T, a) - np.dot(c.T, d)
+        aux1 = np.hstack([Aast + np.outer(d, d) / s, -d / s])
+        if np.shape(-d.T / s)[1]==1:
+            s = s.reshape(1,-1)
+            aux2 = np.squeeze(np.hstack([-d.T / s, 1 / s]))
+        else:
+            aux2 = np.hstack([np.squeeze(-d.T / s), 1 / s])
+        Bast = np.vstack([aux1, aux2])
+        v = np.dot(a.T, self.r) / s
+        x = np.vstack([(xold - d * v), v])
+        return Bast, x
+
+    def _MultiUpdateInverseHermitian(self, invH, neg_indexes):
+        """
+        Method for the quick update of weights (self.w), whenever a negative weight is found
+        """
+        neg_indexes = np.sort(neg_indexes)
+        for i in range(np.size(neg_indexes)):
+            neg_index = neg_indexes[i] - i
+            invH = self._UpdateInverseHermitian(invH, neg_index)
+        return invH
+
+    def _UpdateInverseHermitian(self, invH, neg_index):
+        """
+        Method for the quick update of weights (self.w), whenever a negative weight is found
+        """
+        if neg_index == np.shape(invH)[1]:
+            aux = (invH[0:-1, -1] * invH[-1, 0:-1]) / invH(-1, -1)
+            invH_new = invH[:-1, :-1] - aux
+        else:
+            aux1 = np.hstack([invH[:, 0:neg_index], invH[:, neg_index + 1:], invH[:, neg_index].reshape(-1, 1)])
+            aux2 = np.vstack([aux1[0:neg_index, :], aux1[neg_index + 1:, :], aux1[neg_index, :]])
+            invH_new = aux2[0:-1, 0:-1] - np.outer(aux2[0:-1, -1], aux2[-1, 0:-1]) / aux2[-1, -1]
+        return invH_new
+
+
+
+
+
+
```

## KratosMultiphysics/RomApplication/hrom_training_utility.py

```diff
@@ -1,423 +1,462 @@
-# Import Python modules
-import json
-import numpy as np
-from pathlib import Path
-
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications
-import KratosMultiphysics.RomApplication as KratosROM
-from KratosMultiphysics.RomApplication.empirical_cubature_method import EmpiricalCubatureMethod
-from KratosMultiphysics.RomApplication.randomized_singular_value_decomposition import RandomizedSingularValueDecomposition
-
-class HRomTrainingUtility(object):
-    """Auxiliary utility for the HROM training.
-    This class encapsulates all the functions required for the HROM training.
-    These are the ROM residuals collection, the calculation and storage of
-    the HROM weights and the creation and export of the HROM model parts.
-    """
-
-    def __init__(self, solver, custom_settings):
-        # Validate and assign the HROM training settings
-        settings = custom_settings["hrom_settings"]
-        settings.ValidateAndAssignDefaults(self.__GetHRomTrainingDefaultSettings())
-
-        # Projection strategy (residual projection)
-        settings["projection_strategy"] = custom_settings["projection_strategy"] # To be consistent with the solving strategy
-
-        # Create the HROM element selector
-        element_selection_type = settings["element_selection_type"].GetString()
-        if element_selection_type == "empirical_cubature":
-            self.hyper_reduction_element_selector = EmpiricalCubatureMethod()
-            self.element_selection_svd_truncation_tolerance = settings["element_selection_svd_truncation_tolerance"].GetDouble()
-        else:
-            err_msg = "\'{}\' HROM \'element_selection_type\' is not supported.".format(element_selection_type)
-            raise Exception(err_msg)
-
-        # Auxiliary member variables
-        self.solver = solver
-        self.time_step_residual_matrix_container = []
-        self.echo_level = settings["echo_level"].GetInt()
-        self.rom_settings = custom_settings["rom_settings"].Clone()
-        self.rom_settings.RemoveValue("rom_bns_settings") #Removing because the inner rom settings are specific for each builder and solver.
-        self.hrom_visualization_model_part = settings["create_hrom_visualization_model_part"].GetBool()
-        self.projection_strategy = settings["projection_strategy"].GetString()
-        self.hrom_output_format = settings["hrom_format"].GetString()
-        self.include_minimum_condition = settings["include_minimum_condition"].GetBool()
-        self.include_condition_parents = settings["include_condition_parents"].GetBool()
-        self.num_of_right_rom_dofs = self.rom_settings["number_of_rom_dofs"].GetInt()
-        self.constraint_sum_weights =  settings["constraint_sum_weights"].GetBool()
-
-        # Retrieve list of model parts from settings
-        self.include_conditions_model_parts_list = settings["include_conditions_model_parts_list"].GetStringArray()
-        self.include_elements_model_parts_list = settings["include_elements_model_parts_list"].GetStringArray()
-        self.include_nodal_neighbouring_elements_model_parts_list = settings["include_nodal_neighbouring_elements_model_parts_list"].GetStringArray()
-
-        # Check if the model parts exist
-        for model_part_name in self.include_conditions_model_parts_list:
-            if not self.solver.model.HasModelPart(model_part_name):
-                raise Exception('The model part named "' + model_part_name + '" does not exist in the model')
-
-        for model_part_name in self.include_elements_model_parts_list:
-            if not self.solver.model.HasModelPart(model_part_name):
-                raise Exception('The model part named "' + model_part_name + '" does not exist in the model')
-
-
-        # getting initial candidate ids for empirical cubature
-        initial_candidate_elements_model_part_list = settings["initial_candidate_elements_model_part_list"].GetStringArray()
-        initial_candidate_conditions_model_part_list = settings["initial_candidate_conditions_model_part_list"].GetStringArray()
-
-        candidate_ids = np.empty(0)
-        for model_part_name in initial_candidate_elements_model_part_list:
-            if not self.solver.model.HasModelPart(model_part_name):
-                raise Exception('The model part named "' + model_part_name + '" does not exist in the model')
-            candidate_elements_model_part = self.solver.model.GetModelPart(model_part_name)
-            if candidate_elements_model_part.NumberOfElements() == 0:
-                KratosMultiphysics.Logger.PrintWarning("HRomTrainingUtility",
-                    f"The model part named '{model_part_name}' has no associated elements. Fetching the associated neighboring elements to the model part's nodes.")
-                this_modelpart_element_ids = KratosROM.RomAuxiliaryUtilities.GetNodalNeighbouringElementIds(self.solver.GetComputingModelPart(), candidate_elements_model_part)
-            else:
-                this_modelpart_element_ids = KratosROM.RomAuxiliaryUtilities.GetElementIdsInModelPart(candidate_elements_model_part)
-            if len(this_modelpart_element_ids)>0:
-                candidate_ids = np.r_[candidate_ids, np.array(this_modelpart_element_ids)]
-
-        number_of_elements = self.solver.GetComputingModelPart().GetRootModelPart().NumberOfElements()
-        for model_part_name in initial_candidate_conditions_model_part_list:
-            if not self.solver.model.HasModelPart(model_part_name):
-                raise Exception('The model part named "' + model_part_name + '" does not exist in the model')
-            this_modelpart_condition_ids = KratosROM.RomAuxiliaryUtilities.GetConditionIdsInModelPart(self.solver.model.GetModelPart(model_part_name))
-            if len(this_modelpart_condition_ids)>0:
-                candidate_ids = np.r_[candidate_ids, np.array(this_modelpart_condition_ids)+number_of_elements]
-
-        if np.size(candidate_ids)>0:
-            self.candidate_ids = np.unique(candidate_ids).astype(int)
-        else:
-            self.candidate_ids = None
-
-        # Rom settings files
-        self.rom_basis_output_name = Path(custom_settings["rom_basis_output_name"].GetString())
-        self.rom_basis_output_folder = Path(custom_settings["rom_basis_output_folder"].GetString())
-
-    def AppendCurrentStepResiduals(self):
-        # Get the computing model part from the solver implementing the problem physics
-        computing_model_part = self.solver.GetComputingModelPart()
-
-        # If not created yet, create the ROM residuals utility
-        # Note that this ensures that the residuals utility is created in the first residuals append call
-        # If not, it might happen that the solver scheme is created by the ROM residuals call rather than by the solver one
-        if not hasattr(self, '__rom_residuals_utility'):
-            self.__rom_residuals_utility = KratosROM.RomResidualsUtility(
-                computing_model_part,
-                self.rom_settings,
-                self.solver._GetScheme())
-
-            if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","RomResidualsUtility created.")
-
-        # Generate the matrix of projected residuals
-        if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","Generating matrix of projected residuals.")
-        if (self.projection_strategy=="galerkin"):
-                res_mat = self.__rom_residuals_utility.GetProjectedResidualsOntoPhi()
-        elif (self.projection_strategy=="lspg"):
-                jacobian_phi_product = self.GetJacobianPhiMultiplication(computing_model_part)
-                res_mat = self.__rom_residuals_utility.GetProjectedResidualsOntoJPhi(jacobian_phi_product)
-        elif (self.projection_strategy=="petrov_galerkin"):
-                res_mat = self.__rom_residuals_utility.GetProjectedResidualsOntoPsi()
-        else:
-            err_msg = f"Projection strategy \'{self.projection_strategy}\' for HROM is not supported."
-            raise Exception(err_msg)
-
-        np_res_mat = np.array(res_mat, copy=False)
-        self.time_step_residual_matrix_container.append(np_res_mat)
-
-    def GetJacobianPhiMultiplication(self, computing_model_part):
-        jacobian_matrix = KratosMultiphysics.CompressedMatrix()
-        residual_vector = KratosMultiphysics.Vector(self.solver._GetBuilderAndSolver().GetEquationSystemSize())
-        delta_x_vector = KratosMultiphysics.Vector(self.solver._GetBuilderAndSolver().GetEquationSystemSize())
-
-        self.solver._GetBuilderAndSolver().BuildAndApplyDirichletConditions(self.solver._GetScheme(), computing_model_part, jacobian_matrix, residual_vector, delta_x_vector)
-
-        right_rom_basis = KratosMultiphysics.Matrix(self.solver._GetBuilderAndSolver().GetEquationSystemSize(), self.num_of_right_rom_dofs)
-        self.solver._GetBuilderAndSolver().GetRightROMBasis(computing_model_part, right_rom_basis)
-
-        jacobian_scipy_format = KratosMultiphysics.scipy_conversion_tools.to_csr(jacobian_matrix)
-        jacobian_phi_product = jacobian_scipy_format @ right_rom_basis
-
-        return jacobian_phi_product
-
-    def CalculateAndSaveHRomWeights(self):
-        # Calculate the residuals basis and compute the HROM weights from it
-        residual_basis = self.__CalculateResidualBasis()
-        n_conditions = self.solver.GetComputingModelPart().NumberOfConditions() # Conditions must be included as an extra restriction to enforce ECM to capture all BC's regions.
-        self.hyper_reduction_element_selector.SetUp(residual_basis, InitialCandidatesSet = self.candidate_ids, constrain_sum_of_weights=self.constraint_sum_weights, constrain_conditions = False, number_of_conditions = n_conditions)
-        self.hyper_reduction_element_selector.Run()
-        if not self.hyper_reduction_element_selector.success:
-            KratosMultiphysics.Logger.PrintWarning("HRomTrainingUtility", "The Empirical Cubature Method did not converge using the initial set of candidates. Launching again without initial candidates.")
-            #Imposing an initial candidate set can lead to no convergence. Restart without imposing the initial candidate set
-            self.hyper_reduction_element_selector.SetUp(residual_basis, InitialCandidatesSet = None, constrain_sum_of_weights=self.constraint_sum_weights, constrain_conditions = False, number_of_conditions = n_conditions)
-            self.hyper_reduction_element_selector.Run()
-        # Save the HROM weights in the RomParameters.json
-        # Note that in here we are assuming this naming convention for the ROM json file
-        self.AppendHRomWeightsToRomParameters()
-
-    def CreateHRomModelParts(self):
-        # Get solver data
-        model_part_name = self.solver.settings["model_part_name"].GetString()
-        model_part_output_name = self.solver.settings["model_import_settings"]["input_filename"].GetString()
-        # computing_model_part = self.solver.GetComputingModelPart()
-        #computing_model_part = self.solver.GetComputingModelPart().GetRootModelPart() #TODO: DECIDE WHICH ONE WE SHOULD USE?¿?¿ MOST PROBABLY THE ROOT FOR THOSE CASES IN WHICH THE COMPUTING IS CUSTOM (e.g. CFD)
-        aux_model = KratosMultiphysics.Model()
-        computing_model_part = aux_model.CreateModelPart("main")
-        model_part_io = KratosMultiphysics.ModelPartIO(model_part_output_name)
-        model_part_io.ReadModelPart(computing_model_part)
-
-        # Create a new model with the HROM main model part
-        # This is intentionally done in order to completely emulate the origin model part
-        aux_model = KratosMultiphysics.Model()
-        hrom_main_model_part = aux_model.CreateModelPart(model_part_name)
-
-        if self.hrom_output_format == "numpy":
-            hrom_info = KratosMultiphysics.Parameters(json.JSONEncoder().encode(self.__CreateDictionaryWithRomElementsAndWeights()))
-        elif self.hrom_output_format == "json":
-            with (self.rom_basis_output_folder / self.rom_basis_output_name).with_suffix('.json').open('r') as f:
-                rom_parameters = KratosMultiphysics.Parameters(f.read())
-                hrom_info = rom_parameters["elements_and_weights"]
-
-        # Get the weights and fill the HROM computing model part
-        if (self.projection_strategy=="lspg"):
-            KratosROM.RomAuxiliaryUtilities.SetHRomComputingModelPartWithNeighbours(hrom_info,computing_model_part,hrom_main_model_part)
-        else:
-            KratosROM.RomAuxiliaryUtilities.SetHRomComputingModelPart(hrom_info,computing_model_part,hrom_main_model_part)
-        if self.echo_level > 0:
-            KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","HROM computing model part \'{}\' created.".format(hrom_main_model_part.FullName()))
-
-        # Output the HROM model part in mdpa format
-        hrom_output_name = "{}HROM".format(model_part_output_name)
-        model_part_io = KratosMultiphysics.ModelPartIO(hrom_output_name, KratosMultiphysics.IO.WRITE | KratosMultiphysics.IO.MESH_ONLY | KratosMultiphysics.IO.SCIENTIFIC_PRECISION)
-        model_part_io.WriteModelPart(hrom_main_model_part)
-        KratosMultiphysics.kratos_utilities.DeleteFileIfExisting("{}.time".format(hrom_output_name))
-        if self.echo_level > 0:
-            KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","HROM mesh written in \'{}.mdpa\'".format(hrom_output_name))
-
-        #TODO: Make this optional
-        #TODO: Move this out of here
-        # Create the HROM visualization model parts
-        if self.hrom_visualization_model_part:
-            # Create the HROM visualization mesh from the origin model part
-            hrom_visualization_model_part_name = "{}Visualization".format(hrom_main_model_part.Name)
-            hrom_visualization_model_part = aux_model.CreateModelPart(hrom_visualization_model_part_name)
-            KratosROM.RomAuxiliaryUtilities.SetHRomVolumetricVisualizationModelPart(computing_model_part, hrom_visualization_model_part)
-            if self.echo_level > 0:
-                KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","HROM visualization model part \'{}\' created.".format(hrom_visualization_model_part.FullName()))
-
-            print(hrom_visualization_model_part)
-
-            # Write the HROM visualization mesh
-            hrom_vis_output_name = "{}HROMVisualization".format(model_part_output_name)
-            model_part_io = KratosMultiphysics.ModelPartIO(hrom_vis_output_name, KratosMultiphysics.IO.WRITE | KratosMultiphysics.IO.MESH_ONLY | KratosMultiphysics.IO.SCIENTIFIC_PRECISION)
-            model_part_io.WriteModelPart(hrom_visualization_model_part)
-            KratosMultiphysics.kratos_utilities.DeleteFileIfExisting("{}.time".format(hrom_vis_output_name))
-            if self.echo_level > 0:
-                KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","HROM visualization mesh written in \'{}.mdpa\'".format(hrom_vis_output_name))
-
-    @classmethod
-    def __GetHRomTrainingDefaultSettings(cls):
-        default_settings = KratosMultiphysics.Parameters("""{
-            "hrom_format": "numpy",
-            "element_selection_type": "empirical_cubature",
-            "element_selection_svd_truncation_tolerance": 1.0e-6,
-            "echo_level" : 0,
-            "create_hrom_visualization_model_part" : true,
-            "projection_strategy": "galerkin",
-            "include_conditions_model_parts_list": [],
-            "include_elements_model_parts_list": [],
-            "initial_candidate_elements_model_part_list" : [],
-            "initial_candidate_conditions_model_part_list" : [],
-            "include_nodal_neighbouring_elements_model_parts_list":[],
-            "include_minimum_condition": false,
-            "include_condition_parents": false,
-            "constraint_sum_weights": true
-        }""")
-        return default_settings
-
-    def __CalculateResidualBasis(self):
-        # Set up the residual snapshots matrix
-        residuals_snapshot_matrix = self._GetResidualsProjectedMatrix()
-
-        # Calculate the randomized and truncated SVD of the residual snapshots
-        u,_,_,_ = RandomizedSingularValueDecomposition(COMPUTE_V=False).Calculate(
-            residuals_snapshot_matrix,
-            self.element_selection_svd_truncation_tolerance)
-
-        return u
-
-
-
-    def _GetResidualsProjectedMatrix(self):
-        # Set up the residual snapshots matrix
-        n_steps = len(self.time_step_residual_matrix_container)
-        residuals_snapshot_matrix = self.time_step_residual_matrix_container[0]
-        for i in range(1,n_steps):
-            del self.time_step_residual_matrix_container[0] # Avoid having two matrices, numpy does not concatenate references.
-            residuals_snapshot_matrix = np.c_[residuals_snapshot_matrix,self.time_step_residual_matrix_container[0]]
-        return residuals_snapshot_matrix
-
-
-
-    def AppendHRomWeightsToRomParameters(self):
-        number_of_elements = self.solver.GetComputingModelPart().GetRootModelPart().NumberOfElements()
-        weights = np.squeeze(self.hyper_reduction_element_selector.w)
-        indexes = self.hyper_reduction_element_selector.z
-
-        # Create dictionary with HROM weights (Only used for the expansion of the selected Conditions to include their parent Elements)
-        hrom_weights = self.__CreateDictionaryWithRomElementsAndWeights(weights,indexes,number_of_elements)
-
-        # Get the root model part
-        root_model_part = self.solver.GetComputingModelPart().GetRootModelPart()
-
-        # Add conditions
-        for model_part_name in self.include_conditions_model_parts_list:
-            # Check if the sub model part exists
-            if self.solver.model.HasModelPart(model_part_name):
-                conditions_to_include_model_part = self.solver.model.GetModelPart(model_part_name)
-
-                # Call the GetConditionIdsNotInHRomModelPart function
-                new_conditions = KratosROM.RomAuxiliaryUtilities.GetConditionIdsNotInHRomModelPart(
-                    root_model_part, # The complete model part
-                    conditions_to_include_model_part, # The model part containing the conditions to be included
-                    hrom_weights)
-
-                # Add the new conditions to the conditions dict with a null weight
-                for condition_id in new_conditions:
-                    hrom_weights["Conditions"][condition_id] = 0.0
-
-                # If needed, update your weights and indexes using __AddSelectedConditionsWithZeroWeights function with the new_conditions
-                weights, indexes = self.__AddSelectedConditionsWithZeroWeights(weights, indexes, new_conditions, number_of_elements)
-
-        # Add elements
-        for model_part_name in self.include_elements_model_parts_list:
-            # Check if the sub model part exists
-            if self.solver.model.HasModelPart(model_part_name):
-                elements_to_include_model_part = self.solver.model.GetModelPart(model_part_name)
-
-                # Call the GetElementIdsNotInHRomModelPart function
-                new_elements = KratosROM.RomAuxiliaryUtilities.GetElementIdsNotInHRomModelPart(
-                    elements_to_include_model_part, # The model part containing the elements to be included
-                    hrom_weights)
-
-                # Add the new elements to the elements dict with a null weight
-                for element_id in new_elements:
-                    hrom_weights["Elements"][element_id] = 0.0
-
-                # If needed, update your weights and indexes using __AddSelectedElementsWithZeroWeights function with the new_elements
-                weights, indexes = self.__AddSelectedElementsWithZeroWeights(weights, indexes, new_elements)
-
-        # Add nodal neighbouring elements
-        for model_part_name in self.include_nodal_neighbouring_elements_model_parts_list:
-            # Check if the sub model part exists
-            if self.solver.model.HasModelPart(model_part_name):
-                nodal_neighbours_model_part = self.solver.model.GetModelPart(model_part_name)
-
-                # Call the GetNodalNeighbouringElementIdsNotInHRom function
-                new_nodal_neighbours = KratosROM.RomAuxiliaryUtilities.GetNodalNeighbouringElementIdsNotInHRom(
-                    nodal_neighbours_model_part, # The model part containing the nodal neighbouring elements to be included
-                    hrom_weights)
-
-                # Add the new nodal neighbouring elements to the elements dict with a null weight
-                for element_id in new_nodal_neighbours:
-                    hrom_weights["Elements"][element_id] = 0.0
-
-                # If needed, update your weights and indexes using __AddSelectedElementsWithZeroWeights function with the new_nodal_neighbours
-                weights, indexes = self.__AddSelectedElementsWithZeroWeights(weights, indexes, new_nodal_neighbours)
-
-        # If required, keep at least one condition per submodelpart
-        # This might be required by those BCs involving the faces (e.g. slip BCs)
-        if self.include_minimum_condition:
-            # Get the HROM conditions to be added
-            minimum_conditions = KratosROM.RomAuxiliaryUtilities.GetHRomMinimumConditionsIds(
-                self.solver.GetComputingModelPart().GetRootModelPart(), #TODO: I think this one should be the root
-                hrom_weights["Conditions"])
-
-            # Add the selected conditions to the conditions dict with a null weight
-            for cond_id in minimum_conditions:
-                hrom_weights["Conditions"][cond_id] = 0.0
-            weights, indexes = self.__AddSelectedConditionsWithZeroWeights(weights, indexes, minimum_conditions, number_of_elements)
-
-        # If required, add the HROM conditions parent elements
-        # Note that we add these with zero weight so their future assembly will have no effect
-        if self.include_condition_parents:
-            KratosMultiphysics.Logger.PrintWarning("HRomTrainingUtility", 'Make sure you set "assign_neighbour_elements_to_conditions": true in the solver_settings to have a parent element for each condition.')
-
-            # Get the HROM condition parents from the current HROM weights
-            missing_condition_parents = KratosROM.RomAuxiliaryUtilities.GetHRomConditionParentsIds(
-                self.solver.GetComputingModelPart().GetRootModelPart(), #TODO: I think this one should be the root
-                hrom_weights)
-
-            # Add the missing parents to the elements dict with a null weight
-            for parent_id in missing_condition_parents:
-                hrom_weights["Elements"][parent_id] = 0.0
-            weights, indexes = self.__AddSelectedElementsWithZeroWeights(weights,indexes, missing_condition_parents)
-
-        if self.hrom_output_format=="numpy":
-            element_indexes = np.where(indexes < number_of_elements)[0]
-            condition_indexes = np.where(indexes >= number_of_elements)[0]
-            np.save(self.rom_basis_output_folder / "HROM_ElementWeights.npy", weights[element_indexes])
-            np.save(self.rom_basis_output_folder / "HROM_ConditionWeights.npy", weights[condition_indexes])
-            np.save(self.rom_basis_output_folder / "HROM_ElementIds.npy", indexes[element_indexes])  # FIXME fix the -1 in the indexes of numpy and ids of Kratos
-            np.save(self.rom_basis_output_folder / "HROM_ConditionIds.npy", indexes[condition_indexes] - number_of_elements)  # FIXME fix the -1 in the indexes of numpy and ids of Kratos
-
-        elif self.hrom_output_format=="json":
-            with (self.rom_basis_output_folder / self.rom_basis_output_name).with_suffix('.json').open('r') as f:
-                updated_rom_parameters = json.load(f)
-                updated_rom_parameters["elements_and_weights"] = hrom_weights  # TODO: Rename elements_and_weights to hrom_weights
-
-            with (self.rom_basis_output_folder / self.rom_basis_output_name).with_suffix('.json').open('w') as f:
-                json.dump(updated_rom_parameters, f, indent=4)
-
-        if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","\'RomParameters.json\' file updated with HROM weights.")
-
-    def __AddSelectedElementsWithZeroWeights(self, original_weights,original_elements, elements_to_add):
-
-        added_elements_ids = np.array(elements_to_add)
-        updated_elements = np.r_[original_elements, added_elements_ids]
-        updated_weights = np.r_[original_weights, np.zeros(added_elements_ids.shape)]
-
-        return updated_weights, updated_elements
-
-    def __AddSelectedConditionsWithZeroWeights(self, original_weights, original_conditions, conditions_to_add, number_of_elements):
-
-        added_conditions_ids = np.array(conditions_to_add)+number_of_elements
-        updated_conditions = np.r_[original_conditions, added_conditions_ids]
-        updated_weights = np.r_[original_weights, np.zeros(added_conditions_ids.shape)]
-
-        return updated_weights, updated_conditions
-
-    def __CreateDictionaryWithRomElementsAndWeights(self, weights = None, indexes=None, number_of_elements = None):
-
-        if number_of_elements is None:
-            number_of_elements = self.solver.GetComputingModelPart().NumberOfElements()
-        if weights is None:
-            weights = np.r_[np.load(self.rom_basis_output_folder / "HROM_ElementWeights.npy"), np.load(self.rom_basis_output_folder / "HROM_ConditionWeights.npy")]
-        if indexes is None:
-            indexes = np.r_[np.load(self.rom_basis_output_folder / "HROM_ElementIds.npy"), np.load(self.rom_basis_output_folder / "HROM_ConditionIds.npy") + number_of_elements]
-        hrom_weights = {}
-        hrom_weights["Elements"] = {}
-        hrom_weights["Conditions"] = {}
-
-        if type(indexes)==np.int64 or type(indexes)==np.int32:
-            # Only one element found !
-            if indexes <= number_of_elements-1:
-                hrom_weights["Elements"][int(indexes)] = float(weights)
-            else:
-                hrom_weights["Conditions"][int(indexes)-number_of_elements] = float(weights)
-        else:
-            # Many elements found
-            for j in range (len(indexes)):
-                if indexes[j] <=  number_of_elements -1:
-                    hrom_weights["Elements"][int(indexes[j])] = float(weights[j])
-                else:
-                    hrom_weights["Conditions"][int(indexes[j])-number_of_elements] = float(weights[j])
-
-        return hrom_weights
-
-
+# Import Python modules
+import json
+import numpy as np
+from pathlib import Path
+
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications
+import KratosMultiphysics.RomApplication as KratosROM
+from KratosMultiphysics.RomApplication.empirical_cubature_method import EmpiricalCubatureMethod
+from KratosMultiphysics.RomApplication.randomized_singular_value_decomposition import RandomizedSingularValueDecomposition
+
+class HRomTrainingUtility(object):
+    """Auxiliary utility for the HROM training.
+    This class encapsulates all the functions required for the HROM training.
+    These are the ROM residuals collection, the calculation and storage of
+    the HROM weights and the creation and export of the HROM model parts.
+    """
+
+    def __init__(self, solver, custom_settings):
+        # Validate and assign the HROM training settings
+        settings = custom_settings["hrom_settings"]
+        settings.ValidateAndAssignDefaults(self.__GetHRomTrainingDefaultSettings())
+
+        # Projection strategy (residual projection)
+        settings["projection_strategy"] = custom_settings["projection_strategy"] # To be consistent with the solving strategy
+
+        # Create the HROM element selector
+        element_selection_type = settings["element_selection_type"].GetString()
+        if element_selection_type == "empirical_cubature":
+            self.hyper_reduction_element_selector = EmpiricalCubatureMethod()
+            self.element_selection_svd_truncation_tolerance = settings["element_selection_svd_truncation_tolerance"].GetDouble()
+        else:
+            err_msg = "\'{}\' HROM \'element_selection_type\' is not supported.".format(element_selection_type)
+            raise Exception(err_msg)
+
+        # Auxiliary member variables
+        self.solver = solver
+        self.time_step_residual_matrix_container = []
+        self.echo_level = settings["echo_level"].GetInt()
+        self.rom_settings = custom_settings["rom_settings"].Clone()
+        self.rom_settings.RemoveValue("rom_bns_settings") #Removing because the inner rom settings are specific for each builder and solver.
+        self.hrom_visualization_model_part = settings["create_hrom_visualization_model_part"].GetBool()
+        self.projection_strategy = settings["projection_strategy"].GetString()
+        self.hrom_output_format = settings["hrom_format"].GetString()
+        self.include_minimum_condition = settings["include_minimum_condition"].GetBool()
+        self.include_condition_parents = settings["include_condition_parents"].GetBool()
+        self.num_of_right_rom_dofs = self.rom_settings["number_of_rom_dofs"].GetInt()
+        self.constraint_sum_weights =  settings["constraint_sum_weights"].GetBool()
+
+        # Retrieve list of model parts from settings
+        self.include_conditions_model_parts_list = settings["include_conditions_model_parts_list"].GetStringArray()
+        self.include_elements_model_parts_list = settings["include_elements_model_parts_list"].GetStringArray()
+        self.include_nodal_neighbouring_elements_model_parts_list = settings["include_nodal_neighbouring_elements_model_parts_list"].GetStringArray()
+
+        # Check if the model parts exist
+        for model_part_name in self.include_conditions_model_parts_list:
+            if not self.solver.model.HasModelPart(model_part_name):
+                raise Exception('The model part named "' + model_part_name + '" does not exist in the model')
+
+        for model_part_name in self.include_elements_model_parts_list:
+            if not self.solver.model.HasModelPart(model_part_name):
+                raise Exception('The model part named "' + model_part_name + '" does not exist in the model')
+
+
+        #TODO use cpp mappings
+        root_model_part = self.solver.GetComputingModelPart().GetRootModelPart()
+        number_of_elements = root_model_part.NumberOfElements()
+        self._setup_mappings(root_model_part, number_of_elements)
+
+        # getting initial candidate ids for empirical cubature
+        initial_candidate_elements_model_part_list = settings["initial_candidate_elements_model_part_list"].GetStringArray()
+        candidate_ids = np.empty(0)
+        for model_part_name in initial_candidate_elements_model_part_list:
+            if not self.solver.model.HasModelPart(model_part_name):
+                raise Exception('The model part named "' + model_part_name + '" does not exist in the model')
+            candidate_elements_model_part = self.solver.model.GetModelPart(model_part_name)
+            if candidate_elements_model_part.NumberOfElements() == 0:
+                KratosMultiphysics.Logger.PrintWarning("HRomTrainingUtility",
+                    f"The model part named '{model_part_name}' has no associated elements. Fetching the associated neighboring elements to the model part's nodes.")
+                this_modelpart_element_ids = KratosROM.RomAuxiliaryUtilities.GetNodalNeighbouringElementIds(self.solver.GetComputingModelPart(), candidate_elements_model_part)
+            else:
+                this_modelpart_element_ids = KratosROM.RomAuxiliaryUtilities.GetElementIdsInModelPart(candidate_elements_model_part)
+            if len(this_modelpart_element_ids)>0:
+                this_modelpart_element_ids = self.map_element_ids_to_numpy_indexes(this_modelpart_element_ids)
+                candidate_ids = np.r_[candidate_ids, this_modelpart_element_ids]
+
+
+        initial_candidate_conditions_model_part_list = settings["initial_candidate_conditions_model_part_list"].GetStringArray()
+
+        for model_part_name in initial_candidate_conditions_model_part_list:
+            if not self.solver.model.HasModelPart(model_part_name):
+                raise Exception('The model part named "' + model_part_name + '" does not exist in the model')
+            this_modelpart_condition_ids = KratosROM.RomAuxiliaryUtilities.GetConditionIdsInModelPart(self.solver.model.GetModelPart(model_part_name))
+            if len(this_modelpart_condition_ids)>0:
+                this_modelpart_condition_ids = self.map_condition_ids_to_numpy_indexes(this_modelpart_condition_ids)
+                candidate_ids = np.r_[candidate_ids, this_modelpart_condition_ids]
+        if np.size(candidate_ids)>0:
+            self.candidate_ids = np.unique(candidate_ids).astype(int)
+        else:
+            self.candidate_ids = None
+
+        # Rom settings files
+        self.rom_basis_output_name = Path(custom_settings["rom_basis_output_name"].GetString())
+        self.rom_basis_output_folder = Path(custom_settings["rom_basis_output_folder"].GetString())
+
+    def _setup_mappings(self, root_model_part, number_of_elements):
+        self.element_id_to_numpy_index_mapping = {}
+        self.numpy_index_to_element_id_mapping = {}
+        for index, element in enumerate(root_model_part.Elements):
+            self.numpy_index_to_element_id_mapping[index] = element.Id-1 #FIXME -1
+            self.element_id_to_numpy_index_mapping[element.Id-1] = index #FIXME -1
+
+        self.condition_id_to_numpy_index_mapping = {}
+        self.numpy_index_to_condition_id_mapping = {}
+        for index, condition in enumerate(root_model_part.Conditions):
+            self.numpy_index_to_condition_id_mapping[index+number_of_elements] = condition.Id -1 +number_of_elements  #FIXME -1 #FIXME +number_of_elements We should remove redundant fixes
+            self.condition_id_to_numpy_index_mapping[condition.Id-1] = index+number_of_elements #FIXME -1
+
+
+    def map_condition_ids_to_numpy_indexes(self, this_modelpart_condition_ids):
+        this_modelpart_indexes_numpy = []
+        for cond_id in this_modelpart_condition_ids:
+            this_modelpart_indexes_numpy.append(self.condition_id_to_numpy_index_mapping[cond_id])
+        return np.array(this_modelpart_indexes_numpy)
+
+
+    def map_element_ids_to_numpy_indexes(self, this_modelpart_element_ids):
+        this_modelpart_indexes_numpy = []
+        for elem_id in this_modelpart_element_ids:
+            this_modelpart_indexes_numpy.append(self.condition_id_to_numpy_index_mapping[elem_id])
+        return np.array(this_modelpart_indexes_numpy)
+
+
+    def map_numpy_indexes_to_element_and_conditions_ids(self,indexes,number_of_elements):
+
+        kratos_indexes = []
+        for i in range(np.size(indexes)):
+            if indexes[i]<=number_of_elements-1:
+                kratos_indexes.append(self.numpy_index_to_element_id_mapping[indexes[i]])
+            else:
+                kratos_indexes.append(self.numpy_index_to_condition_id_mapping[indexes[i]])
+
+        return np.array(kratos_indexes) #FIXME -1
+
+
+
+    def AppendCurrentStepResiduals(self):
+        # Get the computing model part from the solver implementing the problem physics
+        computing_model_part = self.solver.GetComputingModelPart()
+
+        # If not created yet, create the ROM residuals utility
+        # Note that this ensures that the residuals utility is created in the first residuals append call
+        # If not, it might happen that the solver scheme is created by the ROM residuals call rather than by the solver one
+        if not hasattr(self, '__rom_residuals_utility'):
+            self.__rom_residuals_utility = KratosROM.RomResidualsUtility(
+                computing_model_part,
+                self.rom_settings,
+                self.solver._GetScheme())
+
+            if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","RomResidualsUtility created.")
+
+        # Generate the matrix of projected residuals
+        if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","Generating matrix of projected residuals.")
+        if (self.projection_strategy=="galerkin"):
+                res_mat = self.__rom_residuals_utility.GetProjectedResidualsOntoPhi()
+        elif (self.projection_strategy=="lspg"):
+                jacobian_phi_product = self.GetJacobianPhiMultiplication(computing_model_part)
+                res_mat = self.__rom_residuals_utility.GetProjectedResidualsOntoJPhi(jacobian_phi_product)
+        elif (self.projection_strategy=="petrov_galerkin"):
+                res_mat = self.__rom_residuals_utility.GetProjectedResidualsOntoPsi()
+        else:
+            err_msg = f"Projection strategy \'{self.projection_strategy}\' for HROM is not supported."
+            raise Exception(err_msg)
+
+        np_res_mat = np.array(res_mat, copy=False)
+        self.time_step_residual_matrix_container.append(np_res_mat)
+
+    def GetJacobianPhiMultiplication(self, computing_model_part):
+        jacobian_matrix = KratosMultiphysics.CompressedMatrix()
+        residual_vector = KratosMultiphysics.Vector(self.solver._GetBuilderAndSolver().GetEquationSystemSize())
+        delta_x_vector = KratosMultiphysics.Vector(self.solver._GetBuilderAndSolver().GetEquationSystemSize())
+
+        self.solver._GetBuilderAndSolver().BuildAndApplyDirichletConditions(self.solver._GetScheme(), computing_model_part, jacobian_matrix, residual_vector, delta_x_vector)
+
+        right_rom_basis = KratosMultiphysics.Matrix(self.solver._GetBuilderAndSolver().GetEquationSystemSize(), self.num_of_right_rom_dofs)
+        self.solver._GetBuilderAndSolver().GetRightROMBasis(computing_model_part, right_rom_basis)
+
+        jacobian_scipy_format = KratosMultiphysics.scipy_conversion_tools.to_csr(jacobian_matrix)
+        jacobian_phi_product = jacobian_scipy_format @ right_rom_basis
+
+        return jacobian_phi_product
+
+    def CalculateAndSaveHRomWeights(self):
+        # Calculate the residuals basis and compute the HROM weights from it
+        residual_basis = self.__CalculateResidualBasis()
+        n_conditions = self.solver.GetComputingModelPart().NumberOfConditions() # Conditions must be included as an extra restriction to enforce ECM to capture all BC's regions.
+        self.hyper_reduction_element_selector.SetUp(residual_basis, InitialCandidatesSet = self.candidate_ids, constrain_sum_of_weights=self.constraint_sum_weights, constrain_conditions = False, number_of_conditions = n_conditions)
+        self.hyper_reduction_element_selector.Run()
+        if not self.hyper_reduction_element_selector.success:
+            KratosMultiphysics.Logger.PrintWarning("HRomTrainingUtility", "The Empirical Cubature Method did not converge using the initial set of candidates. Launching again without initial candidates.")
+            #Imposing an initial candidate set can lead to no convergence. Restart without imposing the initial candidate set
+            self.hyper_reduction_element_selector.SetUp(residual_basis, InitialCandidatesSet = None, constrain_sum_of_weights=self.constraint_sum_weights, constrain_conditions = False, number_of_conditions = n_conditions)
+            self.hyper_reduction_element_selector.Run()
+        # Save the HROM weights in the RomParameters.json
+        # Note that in here we are assuming this naming convention for the ROM json file
+        self.AppendHRomWeightsToRomParameters()
+
+    def CreateHRomModelParts(self):
+        # Get solver data
+        model_part_name = self.solver.settings["model_part_name"].GetString()
+        model_part_output_name = self.solver.settings["model_import_settings"]["input_filename"].GetString()
+        # computing_model_part = self.solver.GetComputingModelPart()
+        #computing_model_part = self.solver.GetComputingModelPart().GetRootModelPart() #TODO: DECIDE WHICH ONE WE SHOULD USE?¿?¿ MOST PROBABLY THE ROOT FOR THOSE CASES IN WHICH THE COMPUTING IS CUSTOM (e.g. CFD)
+        aux_model = KratosMultiphysics.Model()
+        computing_model_part = aux_model.CreateModelPart("main")
+        model_part_io = KratosMultiphysics.ModelPartIO(model_part_output_name)
+        model_part_io.ReadModelPart(computing_model_part)
+
+        # Create a new model with the HROM main model part
+        # This is intentionally done in order to completely emulate the origin model part
+        aux_model = KratosMultiphysics.Model()
+        hrom_main_model_part = aux_model.CreateModelPart(model_part_name)
+
+        if self.hrom_output_format == "numpy":
+            hrom_info = KratosMultiphysics.Parameters(json.JSONEncoder().encode(self.__CreateDictionaryWithRomElementsAndWeights()))
+        elif self.hrom_output_format == "json":
+            with (self.rom_basis_output_folder / self.rom_basis_output_name).with_suffix('.json').open('r') as f:
+                rom_parameters = KratosMultiphysics.Parameters(f.read())
+                hrom_info = rom_parameters["elements_and_weights"]
+
+        # Get the weights and fill the HROM computing model part
+        if (self.projection_strategy=="lspg"):
+            KratosROM.RomAuxiliaryUtilities.SetHRomComputingModelPartWithNeighbours(hrom_info,computing_model_part,hrom_main_model_part)
+        else:
+            KratosROM.RomAuxiliaryUtilities.SetHRomComputingModelPart(hrom_info,computing_model_part,hrom_main_model_part)
+        if self.echo_level > 0:
+            KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","HROM computing model part \'{}\' created.".format(hrom_main_model_part.FullName()))
+
+        # Output the HROM model part in mdpa format
+        hrom_output_name = "{}HROM".format(model_part_output_name)
+        model_part_io = KratosMultiphysics.ModelPartIO(hrom_output_name, KratosMultiphysics.IO.WRITE | KratosMultiphysics.IO.MESH_ONLY | KratosMultiphysics.IO.SCIENTIFIC_PRECISION)
+        model_part_io.WriteModelPart(hrom_main_model_part)
+        KratosMultiphysics.kratos_utilities.DeleteFileIfExisting("{}.time".format(hrom_output_name))
+        if self.echo_level > 0:
+            KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","HROM mesh written in \'{}.mdpa\'".format(hrom_output_name))
+
+        #TODO: Make this optional
+        #TODO: Move this out of here
+        # Create the HROM visualization model parts
+        if self.hrom_visualization_model_part:
+            # Create the HROM visualization mesh from the origin model part
+            hrom_visualization_model_part_name = "{}Visualization".format(hrom_main_model_part.Name)
+            hrom_visualization_model_part = aux_model.CreateModelPart(hrom_visualization_model_part_name)
+            KratosROM.RomAuxiliaryUtilities.SetHRomVolumetricVisualizationModelPart(computing_model_part, hrom_visualization_model_part)
+            if self.echo_level > 0:
+                KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","HROM visualization model part \'{}\' created.".format(hrom_visualization_model_part.FullName()))
+
+            print(hrom_visualization_model_part)
+
+            # Write the HROM visualization mesh
+            hrom_vis_output_name = "{}HROMVisualization".format(model_part_output_name)
+            model_part_io = KratosMultiphysics.ModelPartIO(hrom_vis_output_name, KratosMultiphysics.IO.WRITE | KratosMultiphysics.IO.MESH_ONLY | KratosMultiphysics.IO.SCIENTIFIC_PRECISION)
+            model_part_io.WriteModelPart(hrom_visualization_model_part)
+            KratosMultiphysics.kratos_utilities.DeleteFileIfExisting("{}.time".format(hrom_vis_output_name))
+            if self.echo_level > 0:
+                KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","HROM visualization mesh written in \'{}.mdpa\'".format(hrom_vis_output_name))
+
+    @classmethod
+    def __GetHRomTrainingDefaultSettings(cls):
+        default_settings = KratosMultiphysics.Parameters("""{
+            "hrom_format": "numpy",
+            "element_selection_type": "empirical_cubature",
+            "element_selection_svd_truncation_tolerance": 1.0e-6,
+            "echo_level" : 0,
+            "create_hrom_visualization_model_part" : true,
+            "projection_strategy": "galerkin",
+            "include_conditions_model_parts_list": [],
+            "include_elements_model_parts_list": [],
+            "initial_candidate_elements_model_part_list" : [],
+            "initial_candidate_conditions_model_part_list" : [],
+            "include_nodal_neighbouring_elements_model_parts_list":[],
+            "include_minimum_condition": false,
+            "include_condition_parents": false,
+            "constraint_sum_weights": true
+        }""")
+        return default_settings
+
+    def __CalculateResidualBasis(self):
+        # Calculate the randomized and truncated SVD of the residual snapshots #TODO add other SVD options
+        u,_,_,_ = RandomizedSingularValueDecomposition(COMPUTE_V=False).Calculate(
+            self._GetResidualsProjectedMatrix(),
+            self.element_selection_svd_truncation_tolerance)
+
+        return u
+
+
+
+    def _GetResidualsProjectedMatrix(self):
+        return np.block(self.time_step_residual_matrix_container)
+
+
+
+    def AppendHRomWeightsToRomParameters(self):
+        number_of_elements = self.solver.GetComputingModelPart().GetRootModelPart().NumberOfElements()
+        weights = np.squeeze(self.hyper_reduction_element_selector.w)
+        indexes = self.hyper_reduction_element_selector.z
+        indexes = self.map_numpy_indexes_to_element_and_conditions_ids(indexes,number_of_elements)
+
+        # Create dictionary with HROM weights (Only used for the expansion of the selected Conditions to include their parent Elements)
+        hrom_weights = self.__CreateDictionaryWithRomElementsAndWeights(weights,indexes,number_of_elements)
+
+        # Get the root model part
+        root_model_part = self.solver.GetComputingModelPart().GetRootModelPart()
+
+        # Add conditions
+        for model_part_name in self.include_conditions_model_parts_list:
+            # Check if the sub model part exists
+            if self.solver.model.HasModelPart(model_part_name):
+                conditions_to_include_model_part = self.solver.model.GetModelPart(model_part_name)
+
+                # Call the GetConditionIdsNotInHRomModelPart function
+                new_conditions = KratosROM.RomAuxiliaryUtilities.GetConditionIdsNotInHRomModelPart(
+                    root_model_part, # The complete model part
+                    conditions_to_include_model_part, # The model part containing the conditions to be included
+                    hrom_weights)
+
+                # Add the new conditions to the conditions dict with a null weight
+                for condition_id in new_conditions:
+                    hrom_weights["Conditions"][condition_id] = 0.0
+
+                # If needed, update your weights and indexes using __AddSelectedConditionsWithZeroWeights function with the new_conditions
+                weights, indexes = self.__AddSelectedConditionsWithZeroWeights(weights, indexes, new_conditions, number_of_elements)
+
+        # Add elements
+        for model_part_name in self.include_elements_model_parts_list:
+            # Check if the sub model part exists
+            if self.solver.model.HasModelPart(model_part_name):
+                elements_to_include_model_part = self.solver.model.GetModelPart(model_part_name)
+
+                # Call the GetElementIdsNotInHRomModelPart function
+                new_elements = KratosROM.RomAuxiliaryUtilities.GetElementIdsNotInHRomModelPart(
+                    elements_to_include_model_part, # The model part containing the elements to be included
+                    hrom_weights)
+
+                # Add the new elements to the elements dict with a null weight
+                for element_id in new_elements:
+                    hrom_weights["Elements"][element_id] = 0.0
+
+                # If needed, update your weights and indexes using __AddSelectedElementsWithZeroWeights function with the new_elements
+                weights, indexes = self.__AddSelectedElementsWithZeroWeights(weights, indexes, new_elements)
+
+        # Add nodal neighbouring elements
+        for model_part_name in self.include_nodal_neighbouring_elements_model_parts_list:
+            # Check if the sub model part exists
+            if self.solver.model.HasModelPart(model_part_name):
+                nodal_neighbours_model_part = self.solver.model.GetModelPart(model_part_name)
+
+                # Call the GetNodalNeighbouringElementIdsNotInHRom function
+                new_nodal_neighbours = KratosROM.RomAuxiliaryUtilities.GetNodalNeighbouringElementIdsNotInHRom(
+                    nodal_neighbours_model_part, # The model part containing the nodal neighbouring elements to be included
+                    hrom_weights)
+
+                # Add the new nodal neighbouring elements to the elements dict with a null weight
+                for element_id in new_nodal_neighbours:
+                    hrom_weights["Elements"][element_id] = 0.0
+
+                # If needed, update your weights and indexes using __AddSelectedElementsWithZeroWeights function with the new_nodal_neighbours
+                weights, indexes = self.__AddSelectedElementsWithZeroWeights(weights, indexes, new_nodal_neighbours)
+
+        # If required, keep at least one condition per submodelpart
+        # This might be required by those BCs involving the faces (e.g. slip BCs)
+        if self.include_minimum_condition:
+            # Get the HROM conditions to be added
+            minimum_conditions = KratosROM.RomAuxiliaryUtilities.GetHRomMinimumConditionsIds(
+                self.solver.GetComputingModelPart().GetRootModelPart(), #TODO: I think this one should be the root
+                hrom_weights["Conditions"])
+
+            # Add the selected conditions to the conditions dict with a null weight
+            for cond_id in minimum_conditions:
+                hrom_weights["Conditions"][cond_id] = 0.0
+            weights, indexes = self.__AddSelectedConditionsWithZeroWeights(weights, indexes, minimum_conditions, number_of_elements)
+
+        # If required, add the HROM conditions parent elements
+        # Note that we add these with zero weight so their future assembly will have no effect
+        if self.include_condition_parents:
+            KratosMultiphysics.Logger.PrintWarning("HRomTrainingUtility", 'Make sure you set "assign_neighbour_elements_to_conditions": true in the solver_settings to have a parent element for each condition.')
+
+            # Get the HROM condition parents from the current HROM weights
+            missing_condition_parents = KratosROM.RomAuxiliaryUtilities.GetHRomConditionParentsIds(
+                self.solver.GetComputingModelPart().GetRootModelPart(), #TODO: I think this one should be the root
+                hrom_weights)
+
+            # Add the missing parents to the elements dict with a null weight
+            for parent_id in missing_condition_parents:
+                hrom_weights["Elements"][parent_id] = 0.0
+            weights, indexes = self.__AddSelectedElementsWithZeroWeights(weights,indexes, missing_condition_parents)
+
+        if self.hrom_output_format=="numpy":
+            element_indexes = np.where(indexes < number_of_elements)[0]
+            condition_indexes = np.where(indexes >= number_of_elements)[0]
+            np.save(self.rom_basis_output_folder / "HROM_ElementWeights.npy", weights[element_indexes])
+            np.save(self.rom_basis_output_folder / "HROM_ConditionWeights.npy", weights[condition_indexes])
+            np.save(self.rom_basis_output_folder / "HROM_ElementIds.npy", indexes[element_indexes])  # FIXME fix the -1 in the indexes of numpy and ids of Kratos
+            np.save(self.rom_basis_output_folder / "HROM_ConditionIds.npy", indexes[condition_indexes] - number_of_elements)  # FIXME fix the -1 in the indexes of numpy and ids of Kratos
+
+        elif self.hrom_output_format=="json":
+            with (self.rom_basis_output_folder / self.rom_basis_output_name).with_suffix('.json').open('r') as f:
+                updated_rom_parameters = json.load(f)
+                updated_rom_parameters["elements_and_weights"] = hrom_weights  # TODO: Rename elements_and_weights to hrom_weights
+
+            with (self.rom_basis_output_folder / self.rom_basis_output_name).with_suffix('.json').open('w') as f:
+                json.dump(updated_rom_parameters, f, indent=4)
+
+        if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("HRomTrainingUtility","\'RomParameters.json\' file updated with HROM weights.")
+
+    def __AddSelectedElementsWithZeroWeights(self, original_weights,original_elements, elements_to_add):
+
+        added_elements_ids = np.array(elements_to_add)
+        updated_elements = np.r_[original_elements, added_elements_ids]
+        updated_weights = np.r_[original_weights, np.zeros(added_elements_ids.shape)]
+
+        return updated_weights, updated_elements
+
+    def __AddSelectedConditionsWithZeroWeights(self, original_weights, original_conditions, conditions_to_add, number_of_elements):
+
+        added_conditions_ids = np.array(conditions_to_add)+number_of_elements
+        updated_conditions = np.r_[original_conditions, added_conditions_ids]
+        updated_weights = np.r_[original_weights, np.zeros(added_conditions_ids.shape)]
+
+        return updated_weights, updated_conditions
+
+    def __CreateDictionaryWithRomElementsAndWeights(self, weights = None, indexes=None, number_of_elements = None):
+
+        if number_of_elements is None:
+            number_of_elements = self.solver.GetComputingModelPart().NumberOfElements()
+        if weights is None:
+            weights = np.r_[np.load(self.rom_basis_output_folder / "HROM_ElementWeights.npy"), np.load(self.rom_basis_output_folder / "HROM_ConditionWeights.npy")]
+        if indexes is None:
+            indexes = np.r_[np.load(self.rom_basis_output_folder / "HROM_ElementIds.npy"), np.load(self.rom_basis_output_folder / "HROM_ConditionIds.npy") + number_of_elements]
+        hrom_weights = {}
+        hrom_weights["Elements"] = {}
+        hrom_weights["Conditions"] = {}
+
+        if type(indexes)==np.int64 or type(indexes)==np.int32:
+            # Only one element found !
+            if indexes <= number_of_elements-1:
+                hrom_weights["Elements"][int(indexes)] = float(weights)
+            else:
+                hrom_weights["Conditions"][int(indexes)-number_of_elements] = float(weights)
+        else:
+            # Many elements found
+            for j in range (len(indexes)):
+                if indexes[j] <=  number_of_elements -1:
+                    hrom_weights["Elements"][int(indexes[j])] = float(weights[j])
+                else:
+                    hrom_weights["Conditions"][int(indexes[j])-number_of_elements] = float(weights[j])
+
+        return hrom_weights
+
+
```

## KratosMultiphysics/RomApplication/petrov_galerkin_training_utility.py

```diff
@@ -1,201 +1,192 @@
-# Import Python modules
-import json
-import numpy as np
-from pathlib import Path
-from glob import glob
-
-# Importing the Kratos Library
-import KratosMultiphysics
-import KratosMultiphysics.scipy_conversion_tools
-
-# Import applications
-import KratosMultiphysics.RomApplication as KratosROM
-from KratosMultiphysics.RomApplication.randomized_singular_value_decomposition import RandomizedSingularValueDecomposition
-import KratosMultiphysics.kratos_utilities as kratos_utils
-
-class PetrovGalerkinTrainingUtility(object):
-    """Auxiliary utility for the Petrov Galerkin training.
-    This class encapsulates all the functions required for the Petrov Galerkin training.
-    These are snapshots collection for the basis Psi used for solving a Petrov Galerkin ROM.
-    The snapshots depends on the basis strategy (i.e. Jacobian or Residuals).
-    """
-
-    def __init__(self, solver, custom_settings):
-        # Validate and assign the HROM training settings
-        settings = custom_settings["rom_settings"]["rom_bns_settings"]
-        settings.ValidateAndAssignDefaults(self.__GetPetrovGalerkinTrainingDefaultSettings())
-
-        # Auxiliary member variables
-        self.solver = solver
-        self.time_step_snapshots_matrix_container = [] ## J@Phi or R
-        self.echo_level = settings["echo_level"].GetInt()
-        self.rom_settings = custom_settings["rom_settings"].Clone()
-        self.rom_settings.RemoveValue("rom_bns_settings") #Removing because the inner rom settings are specific for each builder and solver.
-        self.basis_strategy = settings["basis_strategy"].GetString()
-        self.include_phi = settings["include_phi"].GetBool()
-        self.svd_truncation_tolerance = settings["svd_truncation_tolerance"].GetDouble()
-        self.rom_basis_output_name = Path(custom_settings["rom_basis_output_name"].GetString())
-        self.rom_basis_output_folder = Path(custom_settings["rom_basis_output_folder"].GetString())
-        self.num_of_right_rom_dofs = self.rom_settings["number_of_rom_dofs"].GetInt()
-
-        self.rom_format =  custom_settings["rom_format"].GetString()
-        available_rom_format = ["json", "numpy"]
-        if self.rom_format not in available_rom_format:
-            err_msg = "Provided \'rom format\' is {}. Available options are {}.".format(self.rom_format, available_rom_format)
-            raise Exception(err_msg)
-
-
-    def AppendCurrentStepProjectedSystem(self):
-        # Get the computing model part from the solver implementing the problem physics
-        computing_model_part = self.solver.GetComputingModelPart()
-
-        # If not created yet, create the ROM residuals utility
-        # Note that this ensures that the residuals utility is created in the first residuals append call
-        # If not, it might happen that the solver scheme is created by the ROM residuals call rather than by the solver one
-        if not hasattr(self, '__rom_residuals_utility'):
-            self.__rom_residuals_utility = KratosROM.RomResidualsUtility(
-                computing_model_part,
-                self.rom_settings,
-                self.solver._GetScheme())
-
-            if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("PetrovGalerkinTrainingUtility","RomResidualsUtility created.")
-
-        # Generate the matrix of residuals or projected Jacobians.
-        if self.basis_strategy=="jacobian":
-            snapshots_matrix = self.GetJacobianPhiMultiplication(computing_model_part)
-            if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("PetrovGalerkinTrainingUtility","Generated matrix of projected Jacobian.")
-        elif self.basis_strategy=="residuals" or self.basis_strategy=="reactions":
-            snapshots_matrix = []
-            files_to_read_and_delete = glob('*.res.mm')#TODO: Stop writing to disk.
-            for to_erase_file in files_to_read_and_delete:
-                non_converged_iteration_snapshot = KratosMultiphysics.Vector()
-                KratosMultiphysics.ReadMatrixMarketVector(to_erase_file, non_converged_iteration_snapshot)
-                snapshots_matrix.append(non_converged_iteration_snapshot)
-            if self.basis_strategy == "residuals":
-                snapshots_matrix = np.array(snapshots_matrix).T
-            elif self.basis_strategy == "reactions":
-                snapshots_matrix = -np.array(snapshots_matrix).T # Negate for 'reactions' as they are residuals with opposite sign.
-            if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("PetrovGalerkinTrainingUtility","Generating matrix of residuals.")
-        else:
-            err_msg = "\'self.basis_strategy\' is not available. Select either 'jacobian' or 'residuals'."
-            raise Exception(err_msg)
-
-        np_snapshots_matrix = np.array(snapshots_matrix, copy=False)
-        self.time_step_snapshots_matrix_container.append(np_snapshots_matrix)
-
-    def GetJacobianPhiMultiplication(self, computing_model_part):
-        jacobian_matrix = KratosMultiphysics.CompressedMatrix()
-        residual_vector = KratosMultiphysics.Vector(self.solver._GetBuilderAndSolver().GetEquationSystemSize())
-        delta_x_vector = KratosMultiphysics.Vector(self.solver._GetBuilderAndSolver().GetEquationSystemSize())
-
-        self.solver._GetBuilderAndSolver().BuildAndApplyDirichletConditions(self.solver._GetScheme(), computing_model_part, jacobian_matrix, residual_vector, delta_x_vector)
-
-        right_rom_basis = KratosMultiphysics.Matrix(self.solver._GetBuilderAndSolver().GetEquationSystemSize(), self.num_of_right_rom_dofs)
-        self.solver._GetBuilderAndSolver().GetRightROMBasis(computing_model_part, right_rom_basis)
-
-        jacobian_scipy_format = KratosMultiphysics.scipy_conversion_tools.to_csr(jacobian_matrix)
-        jacobian_phi_product = jacobian_scipy_format @ right_rom_basis
-
-        return jacobian_phi_product
-
-
-    def CalculateAndSaveBasis(self, snapshots_matrix = None):
-        # Calculate the new basis and save
-        snapshots_basis = self.__CalculateResidualBasis(snapshots_matrix)
-        self.__AppendNewBasisToRomParameters(snapshots_basis)
-
-
-    @classmethod
-    def __GetPetrovGalerkinTrainingDefaultSettings(cls):
-        default_settings = KratosMultiphysics.Parameters("""{
-                "train_petrov_galerkin": false,
-                "basis_strategy": "residuals",
-                "include_phi": false,
-                "svd_truncation_tolerance": 1.0e-6,
-                "solving_technique": "normal_equations",
-                "monotonicity_preserving": false,
-                "echo_level": 0
-        }""")
-        return default_settings
-
-    def __CalculateResidualBasis(self, snapshots_matrix):
-        if snapshots_matrix is None:
-            snapshots_matrix = self._GetSnapshotsMatrix()
-        u_left,s_left,_,_ = RandomizedSingularValueDecomposition(COMPUTE_V=False).Calculate(
-            snapshots_matrix,
-            self.svd_truncation_tolerance)
-        del(snapshots_matrix)
-        #Include Phi in the span of Psi
-        if self.include_phi:
-            #Read Galerkin modes from RomParameters.json
-            u_right = self.__GetGalerkinBasis()
-            u , _= np.linalg.qr(np.c_[u_right,u_left])
-        else:
-            u = u_left
-
-        return u
-
-    def __AppendNewBasisToRomParameters(self, u):
-        petrov_galerkin_number_of_rom_dofs= np.shape(u)[1]
-        n_nodal_unknowns = len(self.rom_settings["nodal_unknowns"].GetStringArray())
-        petrov_galerkin_nodal_modes = {}
-        computing_model_part = self.solver.GetComputingModelPart()
-
-        if self.rom_format == "json":
-            i = 0
-            for node in computing_model_part.Nodes:
-                petrov_galerkin_nodal_modes[node.Id] = u[i:i+n_nodal_unknowns].tolist()
-                i += n_nodal_unknowns
-
-        elif self.rom_format == "numpy":
-            # Storing Petrov-Galerkin modes in Numpy format
-            np.save(self.rom_basis_output_folder / "LeftBasisMatrix.npy", u)
-
-        with (self.rom_basis_output_folder / self.rom_basis_output_name).with_suffix('.json').open('r') as f:
-            updated_rom_parameters = json.load(f)
-            updated_rom_parameters["rom_settings"]["petrov_galerkin_number_of_rom_dofs"] = petrov_galerkin_number_of_rom_dofs
-            updated_rom_parameters["petrov_galerkin_nodal_modes"] = petrov_galerkin_nodal_modes
-
-        with (self.rom_basis_output_folder / self.rom_basis_output_name).with_suffix('.json').open('w') as f:
-            json.dump(updated_rom_parameters, f, indent=4)
-
-        if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("PetrovGalerkinTrainingUtility","\'RomParameters.json\' file updated with HROM weights.")
-
-    def __GetPrettyFloat(self, number):
-        float_format = "{:.12f}"
-        pretty_number = float(float_format.format(number))
-        return pretty_number
-
-    def __GetGalerkinBasis(self):
-        with open(self.rom_basis_output_folder / self.rom_basis_output_name.with_suffix(".json"), 'r') as f:
-            galerkin_rom_parameters = json.load(f)
-            N_Dof_per_node = len(galerkin_rom_parameters["rom_settings"]["nodal_unknowns"])
-            N_nodes = len(galerkin_rom_parameters["nodal_modes"])
-            N_Dofs = int(N_Dof_per_node*N_nodes)
-            N_Dofs_rom = galerkin_rom_parameters["rom_settings"]["number_of_rom_dofs"]
-            u = np.zeros((N_Dofs,N_Dofs_rom))
-            counter_in = 0
-            for key in galerkin_rom_parameters["nodal_modes"].keys():
-                counter_fin = counter_in + N_Dof_per_node
-                u[counter_in:counter_fin,:] = np.array(galerkin_rom_parameters["nodal_modes"][key])
-                counter_in = counter_fin
-
-        return u
-
-
-    def _GetSnapshotsMatrix(self):
-        # Set up the snapshots matrix for new basis
-        n_steps = len(self.time_step_snapshots_matrix_container)
-        snapshots_matrix = self.time_step_snapshots_matrix_container[0]
-        for i in range(1,n_steps):
-            del self.time_step_snapshots_matrix_container[0] # Avoid having two matrices, numpy does not concatenate references.
-            snapshots_matrix = np.c_[snapshots_matrix,self.time_step_snapshots_matrix_container[0]]
-        return snapshots_matrix
-
-
-    @classmethod
-    def __OrthogonalProjector(self, A, B):
-        # A - B @(B.T @ A)
-        BtA = B.T@A
-        A -= B @ BtA
-        return A
+# Import Python modules
+import json
+import numpy as np
+from pathlib import Path
+from glob import glob
+
+# Importing the Kratos Library
+import KratosMultiphysics
+import KratosMultiphysics.scipy_conversion_tools
+
+# Import applications
+import KratosMultiphysics.RomApplication as KratosROM
+from KratosMultiphysics.RomApplication.randomized_singular_value_decomposition import RandomizedSingularValueDecomposition
+import KratosMultiphysics.kratos_utilities as kratos_utils
+
+class PetrovGalerkinTrainingUtility(object):
+    """Auxiliary utility for the Petrov Galerkin training.
+    This class encapsulates all the functions required for the Petrov Galerkin training.
+    These are snapshots collection for the basis Psi used for solving a Petrov Galerkin ROM.
+    The snapshots depends on the basis strategy (i.e. Jacobian or Residuals).
+    """
+
+    def __init__(self, solver, custom_settings):
+        # Validate and assign the HROM training settings
+        settings = custom_settings["rom_settings"]["rom_bns_settings"]
+        settings.ValidateAndAssignDefaults(self.__GetPetrovGalerkinTrainingDefaultSettings())
+
+        # Auxiliary member variables
+        self.solver = solver
+        self.time_step_snapshots_matrix_container = [] ## J@Phi or R
+        self.echo_level = settings["echo_level"].GetInt()
+        self.rom_settings = custom_settings["rom_settings"].Clone()
+        self.rom_settings.RemoveValue("rom_bns_settings") #Removing because the inner rom settings are specific for each builder and solver.
+        self.basis_strategy = settings["basis_strategy"].GetString()
+        self.include_phi = settings["include_phi"].GetBool()
+        self.svd_truncation_tolerance = settings["svd_truncation_tolerance"].GetDouble()
+        self.rom_basis_output_name = Path(custom_settings["rom_basis_output_name"].GetString())
+        self.rom_basis_output_folder = Path(custom_settings["rom_basis_output_folder"].GetString())
+        self.num_of_right_rom_dofs = self.rom_settings["number_of_rom_dofs"].GetInt()
+
+        self.rom_format =  custom_settings["rom_format"].GetString()
+        available_rom_format = ["json", "numpy"]
+        if self.rom_format not in available_rom_format:
+            err_msg = "Provided \'rom format\' is {}. Available options are {}.".format(self.rom_format, available_rom_format)
+            raise Exception(err_msg)
+
+
+    def AppendCurrentStepProjectedSystem(self):
+        # Get the computing model part from the solver implementing the problem physics
+        computing_model_part = self.solver.GetComputingModelPart()
+
+        # If not created yet, create the ROM residuals utility
+        # Note that this ensures that the residuals utility is created in the first residuals append call
+        # If not, it might happen that the solver scheme is created by the ROM residuals call rather than by the solver one
+        if not hasattr(self, '__rom_residuals_utility'):
+            self.__rom_residuals_utility = KratosROM.RomResidualsUtility(
+                computing_model_part,
+                self.rom_settings,
+                self.solver._GetScheme())
+
+            if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("PetrovGalerkinTrainingUtility","RomResidualsUtility created.")
+
+        # Generate the matrix of residuals or projected Jacobians.
+        if self.basis_strategy=="jacobian":
+            snapshots_matrix = self.GetJacobianPhiMultiplication(computing_model_part)
+            if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("PetrovGalerkinTrainingUtility","Generated matrix of projected Jacobian.")
+        elif self.basis_strategy=="residuals" or self.basis_strategy=="reactions":
+            snapshots_matrix = []
+            files_to_read_and_delete = glob('*.res.mm')#TODO: Stop writing to disk.
+            for to_erase_file in files_to_read_and_delete:
+                non_converged_iteration_snapshot = KratosMultiphysics.Vector()
+                KratosMultiphysics.ReadMatrixMarketVector(to_erase_file, non_converged_iteration_snapshot)
+                snapshots_matrix.append(non_converged_iteration_snapshot)
+            if self.basis_strategy == "residuals":
+                snapshots_matrix = np.array(snapshots_matrix).T
+            elif self.basis_strategy == "reactions":
+                snapshots_matrix = -np.array(snapshots_matrix).T # Negate for 'reactions' as they are residuals with opposite sign.
+            if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("PetrovGalerkinTrainingUtility","Generating matrix of residuals.")
+        else:
+            err_msg = "\'self.basis_strategy\' is not available. Select either 'jacobian' or 'residuals'."
+            raise Exception(err_msg)
+
+        np_snapshots_matrix = np.array(snapshots_matrix, copy=False)
+        self.time_step_snapshots_matrix_container.append(np_snapshots_matrix)
+
+    def GetJacobianPhiMultiplication(self, computing_model_part):
+        jacobian_matrix = KratosMultiphysics.CompressedMatrix()
+        residual_vector = KratosMultiphysics.Vector(self.solver._GetBuilderAndSolver().GetEquationSystemSize())
+        delta_x_vector = KratosMultiphysics.Vector(self.solver._GetBuilderAndSolver().GetEquationSystemSize())
+
+        self.solver._GetBuilderAndSolver().BuildAndApplyDirichletConditions(self.solver._GetScheme(), computing_model_part, jacobian_matrix, residual_vector, delta_x_vector)
+
+        right_rom_basis = KratosMultiphysics.Matrix(self.solver._GetBuilderAndSolver().GetEquationSystemSize(), self.num_of_right_rom_dofs)
+        self.solver._GetBuilderAndSolver().GetRightROMBasis(computing_model_part, right_rom_basis)
+
+        jacobian_scipy_format = KratosMultiphysics.scipy_conversion_tools.to_csr(jacobian_matrix)
+        jacobian_phi_product = jacobian_scipy_format @ right_rom_basis
+
+        return jacobian_phi_product
+
+
+    def CalculateAndSaveBasis(self, snapshots_matrix = None):
+        # Calculate the new basis and save
+        snapshots_basis = self._CalculateResidualBasis(snapshots_matrix)
+        self._AppendNewBasisToRomParameters(snapshots_basis)
+
+
+    @classmethod
+    def __GetPetrovGalerkinTrainingDefaultSettings(cls):
+        default_settings = KratosMultiphysics.Parameters("""{
+                "train_petrov_galerkin": false,
+                "basis_strategy": "residuals",
+                "include_phi": false,
+                "svd_truncation_tolerance": 1.0e-6,
+                "solving_technique": "normal_equations",
+                "monotonicity_preserving": false,
+                "echo_level": 0
+        }""")
+        return default_settings
+
+    def _CalculateResidualBasis(self, snapshots_matrix):
+        if snapshots_matrix is None:
+            snapshots_matrix = self._GetSnapshotsMatrix()
+        u_left,s_left,_,_ = RandomizedSingularValueDecomposition(COMPUTE_V=False).Calculate(
+            snapshots_matrix,
+            self.svd_truncation_tolerance)
+        del(snapshots_matrix)
+        #Include Phi in the span of Psi
+        if self.include_phi:
+            #Read Galerkin modes from RomParameters.json
+            u_right = self.__GetGalerkinBasis()
+            u , _= np.linalg.qr(np.c_[u_right,u_left])
+        else:
+            u = u_left
+
+        return u
+
+    def _AppendNewBasisToRomParameters(self, u):
+        petrov_galerkin_number_of_rom_dofs= np.shape(u)[1]
+        n_nodal_unknowns = len(self.rom_settings["nodal_unknowns"].GetStringArray())
+        petrov_galerkin_nodal_modes = {}
+        computing_model_part = self.solver.GetComputingModelPart()
+
+        if self.rom_format == "json":
+            i = 0
+            for node in computing_model_part.Nodes:
+                petrov_galerkin_nodal_modes[node.Id] = u[i:i+n_nodal_unknowns].tolist()
+                i += n_nodal_unknowns
+
+        elif self.rom_format == "numpy":
+            # Storing Petrov-Galerkin modes in Numpy format
+            np.save(self.rom_basis_output_folder / "LeftBasisMatrix.npy", u)
+
+        with (self.rom_basis_output_folder / self.rom_basis_output_name).with_suffix('.json').open('r') as f:
+            updated_rom_parameters = json.load(f)
+            updated_rom_parameters["rom_settings"]["petrov_galerkin_number_of_rom_dofs"] = petrov_galerkin_number_of_rom_dofs
+            updated_rom_parameters["petrov_galerkin_nodal_modes"] = petrov_galerkin_nodal_modes
+
+        with (self.rom_basis_output_folder / self.rom_basis_output_name).with_suffix('.json').open('w') as f:
+            json.dump(updated_rom_parameters, f, indent=4)
+
+        if self.echo_level > 0 : KratosMultiphysics.Logger.PrintInfo("PetrovGalerkinTrainingUtility","\'RomParameters.json\' file updated with HROM weights.")
+
+    def __GetGalerkinBasis(self):
+        if self.rom_format == "json":
+            with open(self.rom_basis_output_folder / self.rom_basis_output_name.with_suffix(".json"), 'r') as f:
+                galerkin_rom_parameters = json.load(f)
+                N_Dof_per_node = len(galerkin_rom_parameters["rom_settings"]["nodal_unknowns"])
+                N_nodes = len(galerkin_rom_parameters["nodal_modes"])
+                N_Dofs = int(N_Dof_per_node*N_nodes)
+                N_Dofs_rom = galerkin_rom_parameters["rom_settings"]["number_of_rom_dofs"]
+                u = np.zeros((N_Dofs,N_Dofs_rom))
+                counter_in = 0
+                for key in galerkin_rom_parameters["nodal_modes"].keys():
+                    counter_fin = counter_in + N_Dof_per_node
+                    u[counter_in:counter_fin,:] = np.array(galerkin_rom_parameters["nodal_modes"][key])
+                    counter_in = counter_fin
+        elif self.rom_format == "numpy":
+            u = np.load(self.rom_basis_output_folder / "RightBasisMatrix.npy")
+
+        return u
+
+
+    def _GetSnapshotsMatrix(self):
+        # Set up the snapshots matrix for new basis
+        n_steps = len(self.time_step_snapshots_matrix_container)
+        snapshots_matrix = self.time_step_snapshots_matrix_container[0]
+        for i in range(1,n_steps):
+            del self.time_step_snapshots_matrix_container[0] # Avoid having two matrices, numpy does not concatenate references.
+            snapshots_matrix = np.c_[snapshots_matrix,self.time_step_snapshots_matrix_container[0]]
+        return snapshots_matrix
+
```

## KratosMultiphysics/RomApplication/python_solvers_wrapper_rom.py

```diff
@@ -1,77 +1,78 @@
-
-import KratosMultiphysics
-from importlib import import_module
-
-def CreateSolverByParameters(model, solver_settings, parallelism):
-
-    KratosMultiphysics.Logger.PrintWarning('\x1b[1;31m[DEPRECATED CLASS] \x1b[0m',"\'python_solvers_wrapper_rom\'", "module is deprecated. Use the generic\'new_python_solvers_wrapper_rom\' one instead.")
-
-    if (type(model) != KratosMultiphysics.Model):
-        raise Exception("input is expected to be provided as a Kratos Model object")
-
-    if (type(solver_settings) != KratosMultiphysics.Parameters):
-        raise Exception("input is expected to be provided as a Kratos Parameters object")
-
-    solver_type = solver_settings["solver_type"].GetString()
-
-
-    if solver_settings.Has("time_integration_method"):
-        time_integration_method = solver_settings["time_integration_method"].GetString()
-    else:
-        time_integration_method = "implicit" # defaulting to implicit time-integration
-
-    # Solvers for OpenMP parallelism
-    if (parallelism == "OpenMP"):
-        if (solver_type == "transient" or solver_type == "Transient"):
-            solver_module_name = "convection_diffusion_transient_rom_solver"
-
-        elif (solver_type == "dynamic" or solver_type == "Dynamic"):
-            if time_integration_method == "implicit":
-                solver_module_name = "structural_mechanics_implicit_dynamic_rom_solver"
-            else:
-                err_msg =  "The requested time integration method \"" + time_integration_method + "\" is not in the python solvers wrapper\n"
-                err_msg += "Available options are: \"implicit\""
-                raise Exception(err_msg)
-
-        elif solver_type == "static" or solver_type == "Static":
-            solver_module_name = "structural_mechanics_static_rom_solver"
-
-        elif (solver_type == "stationary" or solver_type == "Stationary"):
-            solver_module_name = "convection_diffusion_stationary_rom_solver"
-
-        elif (solver_type == "monolithic" or solver_type == "Monolithic"):
-            solver_module_name = "navier_stokes_solver_vmsmonolithic_rom"
-
-        else:
-            err_msg =  "The requested solver type \"" + solver_type + "\" is not in the python solvers wrapper\n"
-            err_msg += "Available options are: \"transient\", \"stationary\""
-            raise Exception(err_msg)
-
-    # Solvers for MPI parallelism
-    elif (parallelism == "MPI"):
-        err_msg =  "The requested parallel type MPI is not yet available!\n"
-        raise Exception(err_msg)
-
-    else:
-        err_msg =  "The requested parallel type \"" + parallelism + "\" is not available!\n"
-        err_msg += "Available options are: \"OpenMP\", \"MPI\""
-        raise Exception(err_msg)
-
-    module_full = 'KratosMultiphysics.RomApplication.' + solver_module_name
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
-    return CreateSolverByParameters(model, solver_settings, parallelism)
-
+import sys
+import importlib
+
+import KratosMultiphysics
+from KratosMultiphysics import kratos_utilities
+from KratosMultiphysics.RomApplication import rom_solver
+
+
+def _GetAvailableSolverWrapperModules():
+    return {
+        "KratosMultiphysics.FluidDynamicsApplication"       : "python_solvers_wrapper_fluid",
+        "KratosMultiphysics.StructuralMechanicsApplication" : "python_solvers_wrapper_structural",
+        "KratosMultiphysics.ConvectionDiffusionApplication" : "python_solvers_wrapper_convection_diffusion",
+        "KratosMultiphysics.CompressiblePotentialFlowApplication" : "python_solvers_wrapper_compressible_potential",
+        "KratosMultiphysics.GeoMechanicsApplication" : "geomechanics_solvers_wrapper"
+    }
+
+
+def CreateSolverByParameters(model, solver_settings, parallelism, analysis_stage_module_name):
+
+    if not isinstance(model, KratosMultiphysics.Model):
+        raise Exception("input is expected to be provided as a Kratos Model object")
+
+    if not isinstance(solver_settings, KratosMultiphysics.Parameters):
+        raise Exception("input is expected to be provided as a Kratos Parameters object")
+
+    # Get the corresponding application from the analysis_stage path
+    split_analysis_stage_module_name = analysis_stage_module_name.split('.')
+    application_module_name = split_analysis_stage_module_name[0] + "." + split_analysis_stage_module_name[1]
+    if not kratos_utilities.CheckIfApplicationsAvailable(split_analysis_stage_module_name[1]):
+        raise Exception("Module {} is not available.".format(application_module_name))
+
+    # Filter and retrieve the Python solvers wrapper from the corresponding application
+    #TODO: This filtering wouldn't be required if we were using a unified solvers wrapper module name
+    available_modules = _GetAvailableSolverWrapperModules()
+
+    if application_module_name in available_modules:
+        solvers_wrapper_module_module_name = available_modules[application_module_name]
+    else:
+        err_msg = "Python module \'{0}\' is not available. Make sure \'{1}\' is compiled and implemented.\n".format(
+            application_module_name, split_analysis_stage_module_name[1])
+        err_msg += "Currently implemented applications are:\n"
+        err_msg += "".join(" - {}\n".format(key) for key in available_modules)
+        err_msg += "To add a new implementation, do so in '{}' in {}".format(
+            _GetAvailableSolverWrapperModules.__name__, __file__)
+        raise Exception(err_msg)
+    solvers_wrapper_module = importlib.import_module(application_module_name + "." + solvers_wrapper_module_module_name)
+
+    # Create a prototype class instance and get the module and name of the solver to be used as base
+    # Note that an auxiliary Kratos parameter settings without the rom_settings field is created to avoid the defaults error thrown
+    # Note that an auxiliary Kratos model is also created to avoid creating the main_model_part in the prototype class instance
+    #TODO: We could do the same exercise as we do in the stage (module_name to ClassName equal to ModuleName if we standarize the solver names)
+    aux_solver_settings = solver_settings.Clone()
+    aux_solver_settings.RemoveValue("rom_settings")
+    aux_solver_settings.RemoveValue("projection_strategy")
+    aux_solver_settings.RemoveValue("assembling_strategy")
+    aux_solver_settings.RemoveValue("monotonicity_preserving")
+    aux_base_solver_instance = solvers_wrapper_module.CreateSolverByParameters(KratosMultiphysics.Model(), aux_solver_settings, parallelism)
+
+    # Create the ROM solver from the base solver
+    rom_solver_instance = rom_solver.CreateSolver(type(aux_base_solver_instance), model, solver_settings)
+
+    return rom_solver_instance
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
+    analysis_stage = custom_settings["analysis_stage"].GetString()
+    solver_settings = custom_settings["solver_settings"]
+
+    return CreateSolverByParameters(model, solver_settings, parallelism, analysis_stage)
+
```

## KratosMultiphysics/RomApplication/randomized_singular_value_decomposition.py

 * *Ordering differences only*

```diff
@@ -1,222 +1,222 @@
-import numpy as np
-
-class RandomizedSingularValueDecomposition():
-    """
-    This class calculates the singular value decomposition of a matrix A (A = U@np.diag(S)@V.T + Error(truncation_tolerance)) using a randomized algorithm
-    Reference: Halko et al 2009. "Finding structure with randomness: Probabilistic algorithms for constructing approximate matrix decompositions"
-    """
-
-
-
-    """
-    Constructor setting up the parameters for calculation of the SVD
-        COMPUTE_U: whether to return the matrix of left singular vectors U
-        COMPUTE_V: whether to return the matrix of right singular vectors V
-        RELATIVE_SVD: If true, the truncation_tolerance is multiplied by the norm of the original matrix
-                    If false, the truncation_tolerance is taken as an absolute error tolerance
-        USE_RANDOMIZATION: If false, the standard svd algorith of numpy is followed
-    """
-    def __init__(self, COMPUTE_U=True, COMPUTE_V=True, RELATIVE_SVD=True, USE_RANDOMIZATION=True):
-        self.COMPUTE_U = COMPUTE_U
-        self.COMPUTE_V = COMPUTE_V
-        self.RELATIVE_SVD = RELATIVE_SVD
-        self.USE_RANDOMIZATION = USE_RANDOMIZATION
-
-
-
-    """
-    Method for calculating the SVD
-    input:  A: numpy array containing the matrix to decompose
-            truncation_tolerance: this parameter is employed (as is or multiplied by the norm of A, depending on self.RELATIVE_SVD) to truncate the approximation
-    output: U: numpy array containing the matrix of left singular vectors
-            S: numpy array containing the matrix of singular values
-            V: numpy array containing the matrix of right singular vectors
-            eSVD : estimation of the error of the approximation
-    """
-    def Calculate(self, A, truncation_tolerance = 0):
-        if self.USE_RANDOMIZATION == False:
-            Q='full'
-        else:
-            Q, B, eORTH, a = self._RandomizedOrthogonalization(A)  #Randomized orthogonalization (machine precision parameter = mu)
-        if len(Q)==0:
-            U=S=V=np.array([])
-            eSVD=0
-        else:
-            if isinstance(Q,str):
-                #A appears to be full rank
-                U,S,V,eSVD = self._SingularValueDecompostionTruncated( A, truncation_tolerance)
-            else:
-                if self.RELATIVE_SVD==1 and truncation_tolerance>0:
-                    truncation_tolerance = truncation_tolerance*a
-                if truncation_tolerance > eORTH:
-                    e=np.sqrt(truncation_tolerance**2 - eORTH**2)
-                else:
-                    e=truncation_tolerance
-                self.RELATIVE_SVD = 0
-                self.SVD_MaxSize = max(np.shape(A))
-                U,S,V,eSVDb = self._SingularValueDecompostionTruncated(B, e )
-                U = Q @ U
-                eSVD = np.sqrt(eORTH**2 + eSVDb**2)
-
-        return U,S,V,eSVD
-
-
-
-    """
-    Method for obtaining an othonormal basis for the range of the matrix to decompose (stage A, from reference Halko et al 2009 )
-    input:  C: numpy array containing the matrix from which the orthonornal basis will be obtained
-            mu: machine precision parameter, if not specified it is estimated
-            R: estimation for the rank of C, if not specified it is estimated
-    output: Q: numpy array containing the orthonormal basis such that norm(C - Q@Q.T@C) <= mu
-            B: numpy array Q.T@C
-            nC: numpy array estimation of the orthogonalization error
-            c : norm of C
-    """
-    def _RandomizedOrthogonalization(self, C , mu=0, R=0):
-
-        M,N=np.shape(C) # C has dimensions M by N
-        c = nC = np.linalg.norm(C, 'fro')  # Norm of the initial residual
-        if mu==0:
-            mu = max(M,N)*np.finfo(float).eps*nC/2  # Machine precision parameter
-
-        dRmax = np.ceil(0.25*(min(M,N)))
-        dRmin = min(1,min(M,N))
-        dRmin = max(dRmin, np.ceil(0.05*min(M,N) )  )
-
-        self.dRmax = dRmax
-        self.dRmin = dRmin
-        self.R = np.ceil(0.005*(min(M,N))) #Initial guess for the rank of C
-        self.TypeRankEstimate = 1 #Exponential
-
-        if R==0:
-            R=self.R
-        dR = R
-        i=1 #iteration counter
-        nC_old = c
-        R_old = 0
-        Q = B = np.array([])
-
-        while nC>mu:
-            #Omega=np.random.RandomState(seed = 1234).normal(size=(N, int(dR))) # seeded random generator
-            Omega=np.random.RandomState().normal(size=(N, int(dR))) # Draw a N x dR random matrix
-            nOmega = np.sqrt(np.prod(np.shape(C)))
-            factorRED = 10
-            self.SVD_MaxSize = max(M,N)/factorRED
-            Qi, _ = np.linalg.qr((C @ Omega)/nOmega, mode='reduced') #Using QR to obtain the orthogonal basis
-            #Qi,_,_,_ = self._SingularValueDecompostionTruncated((C @ Omega)/nOmega) #Using trunctated svd to obtain the orthogonal basis
-
-            if len(Qi)==0:
-                break
-
-            if len(Q) != 0:
-                print('reorthogonalizing')
-                self.SVD_MaxSize = max(np.shape(Qi))
-                Qi, _ = np.linalg.qr(Qi - Q @(Q.T @ Qi), mode='reduced')  #QR for re-orthogonalization
-                #Qi,_,_,_= self._SingularValueDecompostionTruncated(Qi - Q @(Q.T @ Qi))       #svdt for re-orthogonalization
-
-            #Compute Residual
-            Bi = Qi.T @ C
-            C = C - Qi @ Bi
-
-            #Basis matrix is augmented with Qi
-            if i == 1:
-                Q = Qi
-                B = Bi
-            else:
-                Q = np.c_[Q,Qi]
-                B = np.r_[B,Bi]
-            nC = np.linalg.norm(C, 'fro')  #Norm of the residual
-            print('iter = ',i,' nC = ',nC,' dR = ',dR,' R = ', np.shape(Q)[1])
-
-            R_new=np.shape(Q)[1]
-
-            if self.TypeRankEstimate == 0:
-                Rest = R_old + (R_new-R_old)/(nC-nC_old)*(mu - nC_old)  #Estimated rank (linear)
-            elif self.TypeRankEstimate == 1:
-                Rest = R_old + (R_new -R_old)/(np.log(nC) - np.log(nC_old))*(np.log(mu) - np.log(nC_old))  #Logarithmic Rank Estimation
-            else:
-                Rest = R_old + self.dRmin
-
-            dR = np.ceil(Rest-R_new)
-            dR = min(dR,self.dRmax)
-            dR = max(dR,self.dRmin)
-            Rest = R_new+ dR
-
-            if Rest >= N:
-                Q='FULL'; B=np.array([]); break
-
-            i+=1
-            R_old = R; nC_old = nC; R = Rest
-
-        return Q, B, nC, c
-
-
-    """
-    Method for calculating a truncated version of numpy's svd
-    input:  B: numpy array containing a matrix to decompose
-            epsilon: truncation tolerance for the svd
-    output: U: numpy array containing the matrix of left singular vectors. If self.COMPUTE_U=False ==> U = np.nan
-            S: numpy array containing the matrix of singular values
-            V: numpy array containing the matrix of right singular vectors. If self.COMPUTE_V=False ==> V = np.nan
-            eSVD : estimation of the error of the approximation
-    """
-    def _SingularValueDecompostionTruncated(self, B, epsilon = 0):
-
-        M,N=np.shape(B)
-
-        CalcU=self.COMPUTE_U
-        CalcV=self.COMPUTE_V
-        if hasattr(self, 'SVD_MaxSize'):
-            dimMATRIX = self.SVD_MaxSize
-        else:
-            dimMATRIX = max(M,N)
-
-        if M>=N:
-            if CalcU==True and CalcV==True:
-                U, s, V = np.linalg.svd(B, full_matrices=False) #U --> M xN, V --> N x N
-                V = V.T
-            elif CalcU==True and CalcV==False:
-                U, s, _ = np.linalg.svd(B, full_matrices=False) #U --> M xN, V --> N x N
-            else:
-                _, s, _ = np.linalg.svd(B, full_matrices=False)
-
-        else:
-            # If N>M it proves more efficient to perform the SVD of B^T
-            if CalcU==True and CalcV==True:
-                V, s, U = np.linalg.svd(B.T, full_matrices=False) #U --> M x M, V --> Nx M
-                U = U.T
-            elif CalcU==True and CalcV==False:
-                _, s, U = np.linalg.svd(B.T, full_matrices=False) #U --> M x M, V --> Nx M
-                U = U.T
-            else:
-                _, s, _ = np.linalg.svd(B.T, full_matrices=False)
-
-        tol = dimMATRIX*np.finfo(float).eps*max(s)/2
-        R = np.sum(s > tol)  # Definition of numerical rank
-        eSVD = 0
-
-        if epsilon == 0:
-            K = R
-        else:
-            SingVsq = np.multiply(s,s)
-            SingVsq.sort()
-            normEf2 = np.sqrt(np.cumsum(SingVsq))
-
-            if self.RELATIVE_SVD == 1:
-                epsilon = epsilon*normEf2[-1]
-
-            T = (sum(normEf2<epsilon))
-            K = len(s)-T
-
-        K = min(R,K)
-
-        if len(s)>K:
-            eSVD = np.sqrt(sum( (s[K+1:len(s)-1])**2  ))
-
-
-        if CalcU==True and CalcV==True:
-            return U[:, :K], s[:K], V[:, :K], eSVD
-        elif CalcU==True and CalcV==False:
-            return U[:, :K], s[:K], np.nan , eSVD
-        else:
+import numpy as np
+
+class RandomizedSingularValueDecomposition():
+    """
+    This class calculates the singular value decomposition of a matrix A (A = U@np.diag(S)@V.T + Error(truncation_tolerance)) using a randomized algorithm
+    Reference: Halko et al 2009. "Finding structure with randomness: Probabilistic algorithms for constructing approximate matrix decompositions"
+    """
+
+
+
+    """
+    Constructor setting up the parameters for calculation of the SVD
+        COMPUTE_U: whether to return the matrix of left singular vectors U
+        COMPUTE_V: whether to return the matrix of right singular vectors V
+        RELATIVE_SVD: If true, the truncation_tolerance is multiplied by the norm of the original matrix
+                    If false, the truncation_tolerance is taken as an absolute error tolerance
+        USE_RANDOMIZATION: If false, the standard svd algorith of numpy is followed
+    """
+    def __init__(self, COMPUTE_U=True, COMPUTE_V=True, RELATIVE_SVD=True, USE_RANDOMIZATION=True):
+        self.COMPUTE_U = COMPUTE_U
+        self.COMPUTE_V = COMPUTE_V
+        self.RELATIVE_SVD = RELATIVE_SVD
+        self.USE_RANDOMIZATION = USE_RANDOMIZATION
+
+
+
+    """
+    Method for calculating the SVD
+    input:  A: numpy array containing the matrix to decompose
+            truncation_tolerance: this parameter is employed (as is or multiplied by the norm of A, depending on self.RELATIVE_SVD) to truncate the approximation
+    output: U: numpy array containing the matrix of left singular vectors
+            S: numpy array containing the matrix of singular values
+            V: numpy array containing the matrix of right singular vectors
+            eSVD : estimation of the error of the approximation
+    """
+    def Calculate(self, A, truncation_tolerance = 0):
+        if self.USE_RANDOMIZATION == False:
+            Q='full'
+        else:
+            Q, B, eORTH, a = self._RandomizedOrthogonalization(A)  #Randomized orthogonalization (machine precision parameter = mu)
+        if len(Q)==0:
+            U=S=V=np.array([])
+            eSVD=0
+        else:
+            if isinstance(Q,str):
+                #A appears to be full rank
+                U,S,V,eSVD = self._SingularValueDecompostionTruncated( A, truncation_tolerance)
+            else:
+                if self.RELATIVE_SVD==1 and truncation_tolerance>0:
+                    truncation_tolerance = truncation_tolerance*a
+                if truncation_tolerance > eORTH:
+                    e=np.sqrt(truncation_tolerance**2 - eORTH**2)
+                else:
+                    e=truncation_tolerance
+                self.RELATIVE_SVD = 0
+                self.SVD_MaxSize = max(np.shape(A))
+                U,S,V,eSVDb = self._SingularValueDecompostionTruncated(B, e )
+                U = Q @ U
+                eSVD = np.sqrt(eORTH**2 + eSVDb**2)
+
+        return U,S,V,eSVD
+
+
+
+    """
+    Method for obtaining an othonormal basis for the range of the matrix to decompose (stage A, from reference Halko et al 2009 )
+    input:  C: numpy array containing the matrix from which the orthonornal basis will be obtained
+            mu: machine precision parameter, if not specified it is estimated
+            R: estimation for the rank of C, if not specified it is estimated
+    output: Q: numpy array containing the orthonormal basis such that norm(C - Q@Q.T@C) <= mu
+            B: numpy array Q.T@C
+            nC: numpy array estimation of the orthogonalization error
+            c : norm of C
+    """
+    def _RandomizedOrthogonalization(self, C , mu=0, R=0):
+
+        M,N=np.shape(C) # C has dimensions M by N
+        c = nC = np.linalg.norm(C, 'fro')  # Norm of the initial residual
+        if mu==0:
+            mu = max(M,N)*np.finfo(float).eps*nC/2  # Machine precision parameter
+
+        dRmax = np.ceil(0.25*(min(M,N)))
+        dRmin = min(1,min(M,N))
+        dRmin = max(dRmin, np.ceil(0.05*min(M,N) )  )
+
+        self.dRmax = dRmax
+        self.dRmin = dRmin
+        self.R = np.ceil(0.005*(min(M,N))) #Initial guess for the rank of C
+        self.TypeRankEstimate = 1 #Exponential
+
+        if R==0:
+            R=self.R
+        dR = R
+        i=1 #iteration counter
+        nC_old = c
+        R_old = 0
+        Q = B = np.array([])
+
+        while nC>mu:
+            #Omega=np.random.RandomState(seed = 1234).normal(size=(N, int(dR))) # seeded random generator
+            Omega=np.random.RandomState().normal(size=(N, int(dR))) # Draw a N x dR random matrix
+            nOmega = np.sqrt(np.prod(np.shape(C)))
+            factorRED = 10
+            self.SVD_MaxSize = max(M,N)/factorRED
+            Qi, _ = np.linalg.qr((C @ Omega)/nOmega, mode='reduced') #Using QR to obtain the orthogonal basis
+            #Qi,_,_,_ = self._SingularValueDecompostionTruncated((C @ Omega)/nOmega) #Using trunctated svd to obtain the orthogonal basis
+
+            if len(Qi)==0:
+                break
+
+            if len(Q) != 0:
+                print('reorthogonalizing')
+                self.SVD_MaxSize = max(np.shape(Qi))
+                Qi, _ = np.linalg.qr(Qi - Q @(Q.T @ Qi), mode='reduced')  #QR for re-orthogonalization
+                #Qi,_,_,_= self._SingularValueDecompostionTruncated(Qi - Q @(Q.T @ Qi))       #svdt for re-orthogonalization
+
+            #Compute Residual
+            Bi = Qi.T @ C
+            C = C - Qi @ Bi
+
+            #Basis matrix is augmented with Qi
+            if i == 1:
+                Q = Qi
+                B = Bi
+            else:
+                Q = np.c_[Q,Qi]
+                B = np.r_[B,Bi]
+            nC = np.linalg.norm(C, 'fro')  #Norm of the residual
+            print('iter = ',i,' nC = ',nC,' dR = ',dR,' R = ', np.shape(Q)[1])
+
+            R_new=np.shape(Q)[1]
+
+            if self.TypeRankEstimate == 0:
+                Rest = R_old + (R_new-R_old)/(nC-nC_old)*(mu - nC_old)  #Estimated rank (linear)
+            elif self.TypeRankEstimate == 1:
+                Rest = R_old + (R_new -R_old)/(np.log(nC) - np.log(nC_old))*(np.log(mu) - np.log(nC_old))  #Logarithmic Rank Estimation
+            else:
+                Rest = R_old + self.dRmin
+
+            dR = np.ceil(Rest-R_new)
+            dR = min(dR,self.dRmax)
+            dR = max(dR,self.dRmin)
+            Rest = R_new+ dR
+
+            if Rest >= N:
+                Q='FULL'; B=np.array([]); break
+
+            i+=1
+            R_old = R; nC_old = nC; R = Rest
+
+        return Q, B, nC, c
+
+
+    """
+    Method for calculating a truncated version of numpy's svd
+    input:  B: numpy array containing a matrix to decompose
+            epsilon: truncation tolerance for the svd
+    output: U: numpy array containing the matrix of left singular vectors. If self.COMPUTE_U=False ==> U = np.nan
+            S: numpy array containing the matrix of singular values
+            V: numpy array containing the matrix of right singular vectors. If self.COMPUTE_V=False ==> V = np.nan
+            eSVD : estimation of the error of the approximation
+    """
+    def _SingularValueDecompostionTruncated(self, B, epsilon = 0):
+
+        M,N=np.shape(B)
+
+        CalcU=self.COMPUTE_U
+        CalcV=self.COMPUTE_V
+        if hasattr(self, 'SVD_MaxSize'):
+            dimMATRIX = self.SVD_MaxSize
+        else:
+            dimMATRIX = max(M,N)
+
+        if M>=N:
+            if CalcU==True and CalcV==True:
+                U, s, V = np.linalg.svd(B, full_matrices=False) #U --> M xN, V --> N x N
+                V = V.T
+            elif CalcU==True and CalcV==False:
+                U, s, _ = np.linalg.svd(B, full_matrices=False) #U --> M xN, V --> N x N
+            else:
+                _, s, _ = np.linalg.svd(B, full_matrices=False)
+
+        else:
+            # If N>M it proves more efficient to perform the SVD of B^T
+            if CalcU==True and CalcV==True:
+                V, s, U = np.linalg.svd(B.T, full_matrices=False) #U --> M x M, V --> Nx M
+                U = U.T
+            elif CalcU==True and CalcV==False:
+                _, s, U = np.linalg.svd(B.T, full_matrices=False) #U --> M x M, V --> Nx M
+                U = U.T
+            else:
+                _, s, _ = np.linalg.svd(B.T, full_matrices=False)
+
+        tol = dimMATRIX*np.finfo(float).eps*max(s)/2
+        R = np.sum(s > tol)  # Definition of numerical rank
+        eSVD = 0
+
+        if epsilon == 0:
+            K = R
+        else:
+            SingVsq = np.multiply(s,s)
+            SingVsq.sort()
+            normEf2 = np.sqrt(np.cumsum(SingVsq))
+
+            if self.RELATIVE_SVD == 1:
+                epsilon = epsilon*normEf2[-1]
+
+            T = (sum(normEf2<epsilon))
+            K = len(s)-T
+
+        K = min(R,K)
+
+        if len(s)>K:
+            eSVD = np.sqrt(sum( (s[K+1:len(s)-1])**2  ))
+
+
+        if CalcU==True and CalcV==True:
+            return U[:, :K], s[:K], V[:, :K], eSVD
+        elif CalcU==True and CalcV==False:
+            return U[:, :K], s[:K], np.nan , eSVD
+        else:
             return np.nan, s[:K], np.nan , eSVD
```

## KratosMultiphysics/RomApplication/rom_analysis.py

```diff
@@ -1,289 +1,313 @@
-import importlib
-
-import KratosMultiphysics
-import KratosMultiphysics.RomApplication as KratosROM
-from KratosMultiphysics.RomApplication import new_python_solvers_wrapper_rom
-from KratosMultiphysics.RomApplication.hrom_training_utility import HRomTrainingUtility
-from KratosMultiphysics.RomApplication.petrov_galerkin_training_utility import PetrovGalerkinTrainingUtility
-from KratosMultiphysics.RomApplication.calculate_rom_basis_output_process import CalculateRomBasisOutputProcess
-import numpy as np
-
-from glob import glob
-from os import remove
-from pathlib import Path
-
-def CreateRomAnalysisInstance(cls, global_model, parameters):
-    class RomAnalysis(cls):
-
-        def __init__(self,global_model, parameters):
-            super().__init__(global_model, parameters)
-
-        def _CreateSolver(self):
-            """ Create the Solver (and create and import the ModelPart if it is not alread in the model) """
-
-            # Assign rom basis output folder and file name
-            self.rom_basis_output_name = 'RomParameters' #Default
-            self.rom_basis_output_folder = 'rom_data' #Default
-            if self.project_parameters.Has("output_processes"):
-                for name in self.project_parameters["output_processes"].keys():
-                    if name=="rom_output":
-                        rom_output_paramaters = self.project_parameters["output_processes"]["rom_output"]
-                        self.rom_basis_output_name = rom_output_paramaters[0]["Parameters"]["rom_basis_output_name"].GetString()
-                        self.rom_basis_output_folder = rom_output_paramaters[0]["Parameters"]["rom_basis_output_folder"].GetString()
-            self.rom_basis_output_name = Path(self.rom_basis_output_name)
-            self.rom_basis_output_folder = Path(self.rom_basis_output_folder)
-
-            # Get the ROM settings from the RomParameters.json input file
-            with open(self.rom_basis_output_folder / self.rom_basis_output_name.with_suffix('.json')) as rom_parameters:
-                self.rom_parameters = KratosMultiphysics.Parameters(rom_parameters.read())
-
-            # Set the ROM settings in the "solver_settings" of the solver introducing the physics
-            self.project_parameters["solver_settings"].AddValue("rom_settings", self.rom_parameters["rom_settings"])
-
-            # Inner ROM settings
-            self.rom_bns_settings = self.rom_parameters["rom_settings"]["rom_bns_settings"]
-
-            # HROM operations flags
-            self.rom_basis_process_list_check = True
-            self.rom_basis_output_process_check = True
-            self.run_hrom = self.rom_parameters["run_hrom"].GetBool() if self.rom_parameters.Has("run_hrom") else False
-            self.train_hrom = self.rom_parameters["train_hrom"].GetBool() if self.rom_parameters.Has("train_hrom") else False
-            self.rom_manager = self.rom_parameters["rom_manager"].GetBool()
-            if self.run_hrom and self.train_hrom:
-                # Check that train an run HROM are not set at the same time
-                err_msg = "\'run_hrom\' and \'train_hrom\' are both \'true\'. Select either training or running (if training has been already done)."
-                raise Exception(err_msg)
-
-            # Petrov Galerking Training settings
-            self.train_petrov_galerkin = self.rom_bns_settings["train_petrov_galerkin"].GetBool() if self.rom_bns_settings.Has("train_petrov_galerkin") else False
-            if self.train_hrom and self.train_petrov_galerkin:
-                err_msg = "\'train_petrov_galerkin\' and \'train_hrom\' are both \'true\'. Select only one training strategy."
-                raise Exception(err_msg)
-            if (self.train_hrom or self.train_petrov_galerkin) and (self.run_hrom):
-                err_msg = "\'train_petrov_galerkin\' or \'train_hrom\' and \'run_hrom\' are both \'true\'. Select either training or running (if training has been already done)."
-                raise Exception(err_msg)
-
-            # ROM solving strategy
-            self.solving_strategy = self.rom_parameters["projection_strategy"].GetString() if self.rom_parameters.Has("projection_strategy") else "galerkin"
-            self.project_parameters["solver_settings"].AddString("projection_strategy",self.solving_strategy)
-
-            # Add or remove parameters depending on the solving strategy
-            ##LSPG
-            if self.solving_strategy=="lspg":
-                solving_technique = self.rom_bns_settings["solving_technique"].GetString() if self.rom_bns_settings.Has("solving_technique") else "normal_equations"
-                # Check if the solving technique is either "normal_equations" or "qr_decomposition"
-                if solving_technique not in ["normal_equations", "qr_decomposition"]:
-                    err_msg = f"'{solving_technique}' is not a valid solving technique. Choose either 'normal_equations' or 'qr_decomposition'."
-                    raise Exception(err_msg)
-
-                self.project_parameters["solver_settings"]["rom_settings"]["rom_bns_settings"].AddString("solving_technique", solving_technique)
-                self.project_parameters["solver_settings"]["rom_settings"]["rom_bns_settings"].AddBool("train_petrov_galerkin", self.train_petrov_galerkin)
-                #Adding the basis strategy for generating the left ROB for the Petrov-Galerkin ROM.
-                petrov_galerkin_basis_strategy = self.rom_bns_settings["basis_strategy"].GetString() if self.rom_bns_settings.Has("basis_strategy") else "residuals"
-                self.project_parameters["solver_settings"]["rom_settings"]["rom_bns_settings"].AddString("basis_strategy", petrov_galerkin_basis_strategy)
-
-            ##Petrov Galerkin
-            if self.solving_strategy=="petrov_galerkin":
-                self.petrov_galerkin_rom_dofs = self.project_parameters["solver_settings"]["rom_settings"]["petrov_galerkin_number_of_rom_dofs"].GetInt()
-            else:
-                self.project_parameters["solver_settings"]["rom_settings"].RemoveValue("petrov_galerkin_number_of_rom_dofs")
-
-            # ROM assembling strategy
-            self.assembling_strategy = self.rom_parameters["assembling_strategy"].GetString() if self.rom_parameters.Has("assembling_strategy") else "global"
-            self.project_parameters["solver_settings"].AddString("assembling_strategy",self.assembling_strategy)
-
-            # Create the ROM solver
-            return new_python_solvers_wrapper_rom.CreateSolver(
-                self.model,
-                self.project_parameters)
-
-        def _GetListOfProcesses(self):
-            # Get the already existent processes list
-            list_of_processes = super()._GetListOfProcesses()
-
-            # Check if there is any instance of ROM basis output
-            if self.rom_basis_process_list_check and not self.rom_manager: #eliminate the RomOutputProcess if not run inside the RomManager
-                for process in list_of_processes:
-                    if isinstance(process, KratosROM.calculate_rom_basis_output_process.CalculateRomBasisOutputProcess):
-                        warn_msg = "\'CalculateRomBasisOutputProcess\' instance found in ROM stage. Basis must be already stored in \'RomParameters.json\'. Removing instance from processes list."
-                        KratosMultiphysics.Logger.PrintWarning("RomAnalysis", warn_msg)
-                        list_of_processes.remove(process)
-                self.rom_basis_process_list_check = False
-
-            return list_of_processes
-
-        def _GetListOfOutputProcesses(self):
-            # Get the already existent output processes list
-            list_of_output_processes = super()._GetListOfOutputProcesses()
-
-            # Check if there is any instance of ROM basis output
-            if self.rom_basis_output_process_check and not self.rom_manager: #eliminate the RomOutputProcess if not run inside the RomManager
-                for process in list_of_output_processes:
-                    if isinstance(process, KratosROM.calculate_rom_basis_output_process.CalculateRomBasisOutputProcess):
-                        warn_msg = "\'CalculateRomBasisOutputProcess\' instance found in ROM stage. Basis must be already stored in \'RomParameters.json\'. Removing instance from output processes list."
-                        KratosMultiphysics.Logger.PrintWarning("RomAnalysis", warn_msg)
-                        list_of_output_processes.remove(process)
-                self.rom_basis_output_process_check = False
-
-            return list_of_output_processes
-
-        def _GetSimulationName(self):
-            return "::[ROM Simulation]:: "
-
-        def ModifyAfterSolverInitialize(self):
-            """Here is where the ROM_BASIS is imposed to each node"""
-            super().ModifyAfterSolverInitialize()
-
-            # Get the model part where the ROM is to be applied
-            computing_model_part = self._GetSolver().GetComputingModelPart().GetRootModelPart()
-            # computing_model_part = self._GetSolver().GetComputingModelPart()
-
-            # Set ROM basis
-            nodal_modes = self.rom_parameters["nodal_modes"]
-            nodal_dofs = len(self.project_parameters["solver_settings"]["rom_settings"]["nodal_unknowns"].GetStringArray())
-            rom_dofs = self.project_parameters["solver_settings"]["rom_settings"]["number_of_rom_dofs"].GetInt()
-
-            # Set the right nodal ROM basis
-            if self.rom_parameters["rom_format"].GetString() == "json":
-                aux = KratosMultiphysics.Matrix(nodal_dofs, rom_dofs)
-                for node in computing_model_part.Nodes:
-                    node_id = str(node.Id)
-                    for j in range(nodal_dofs):
-                        for i in range(rom_dofs):
-                            aux[j,i] = nodal_modes[node_id][j][i].GetDouble()
-                    node.SetValue(KratosROM.ROM_BASIS, aux)
-
-                # Set the left nodal ROM basis if it is different than the right nodal ROM basis (i.e. Petrov-Galerkin)
-                if (self.solving_strategy == "petrov_galerkin"):
-                    petrov_galerkin_nodal_modes = self.rom_parameters["petrov_galerkin_nodal_modes"]
-                    petrov_galerkin_nodal_dofs = len(self.project_parameters["solver_settings"]["rom_settings"]["nodal_unknowns"].GetStringArray())
-                    aux = KratosMultiphysics.Matrix(petrov_galerkin_nodal_dofs, self.petrov_galerkin_rom_dofs)
-                    for node in computing_model_part.Nodes:
-                        node_id = str(node.Id)
-                        for j in range(petrov_galerkin_nodal_dofs):
-                            for i in range(self.petrov_galerkin_rom_dofs):
-                                aux[j,i] = petrov_galerkin_nodal_modes[node_id][j][i].GetDouble()
-                        node.SetValue(KratosROM.ROM_LEFT_BASIS, aux)
-
-            elif self.rom_parameters["rom_format"].GetString() == "numpy":
-                # Set the nodal ROM basis
-                node_ids = np.load(self.rom_basis_output_folder / "NodeIds.npy")
-                right_modes = np.load(self.rom_basis_output_folder / "RightBasisMatrix.npy")
-                if right_modes.ndim ==1: #check if matrix contains a single mode (a 1D numpy array)
-                    right_modes.reshape(-1,1)
-                right_modes = right_modes[:,:rom_dofs]
-                if (self.solving_strategy == "petrov_galerkin"):
-                    petrov_galerkin_rom_dofs = self.project_parameters["solver_settings"]["rom_settings"]["petrov_galerkin_number_of_rom_dofs"].GetInt()
-                    left_modes = np.load(self.rom_basis_output_folder / "LeftBasisMatrix.npy")
-                    if left_modes.ndim ==1:
-                        left_modes.reshape(-1,1)
-                    left_modes = left_modes[:,:petrov_galerkin_rom_dofs]
-
-                for node in computing_model_part.Nodes:
-                    offset = np.where(node_ids == node.Id)[0][0]*nodal_dofs
-                    node.SetValue(KratosROM.ROM_BASIS, KratosMultiphysics.Matrix(right_modes[offset:offset+nodal_dofs, :])) # ROM basis
-                    if (self.solving_strategy == "petrov_galerkin"):
-                        node.SetValue(KratosROM.ROM_LEFT_BASIS, KratosMultiphysics.Matrix(left_modes[offset:offset+nodal_dofs, :])) # ROM basis
-
-            # Check for HROM stages
-            if self.train_hrom:
-                # Pass the name of the Rom Parameters file and folder
-                self.rom_parameters.AddString("rom_basis_output_name", str(self.rom_basis_output_name))
-                self.rom_parameters.AddString("rom_basis_output_folder", str(self.rom_basis_output_folder))
-                # Create the training utility to calculate the HROM weights
-                self.__hrom_training_utility = HRomTrainingUtility(
-                    self._GetSolver(),
-                    self.rom_parameters)
-            elif self.run_hrom:
-                if self.rom_parameters["hrom_settings"]["hrom_format"].GetString() == "json":
-                    # Set the HROM weights in elements and conditions
-                    hrom_weights_elements = self.rom_parameters["elements_and_weights"]["Elements"]
-                    for key,value in zip(hrom_weights_elements.keys(), hrom_weights_elements.values()):
-                        computing_model_part.GetElement(int(key)+1).SetValue(KratosROM.HROM_WEIGHT, value.GetDouble()) #FIXME: FIX THE +1
-                    hrom_weights_condtions = self.rom_parameters["elements_and_weights"]["Conditions"]
-                    for key,value in zip(hrom_weights_condtions.keys(), hrom_weights_condtions.values()):
-                        computing_model_part.GetCondition(int(key)+1).SetValue(KratosROM.HROM_WEIGHT, value.GetDouble()) #FIXME: FIX THE +1
-                elif self.rom_parameters["hrom_settings"]["hrom_format"].GetString() == "numpy":
-                    # Set the HROM weights in elements and conditions
-                    element_indexes = np.load(f"{self.rom_basis_output_folder}/HROM_ElementIds.npy")
-                    element_weights = np.load(f"{self.rom_basis_output_folder}/HROM_ElementWeights.npy")
-                    condition_indexes = np.load(f"{self.rom_basis_output_folder}/HROM_ConditionIds.npy")
-                    conditon_weights = np.load(f"{self.rom_basis_output_folder}/HROM_ConditionWeights.npy")
-                    for i in range(np.size(element_indexes)):
-                        computing_model_part.GetElement(int( element_indexes[i])+1).SetValue(KratosROM.HROM_WEIGHT, element_weights[i]  ) #FIXME: FIX THE +1
-                    for i in range(np.size(condition_indexes)):
-                        computing_model_part.GetCondition(int( condition_indexes[i])+1).SetValue(KratosROM.HROM_WEIGHT, conditon_weights[i]  ) #FIXME: FIX THE +1
-
-
-            # Check and Initialize Petrov Galerkin Training stage
-            if self.train_petrov_galerkin:
-                # Pass the name of the Rom Parameters file and folder
-                self.rom_parameters.AddString("rom_basis_output_name", str(self.rom_basis_output_name))
-                self.rom_parameters.AddString("rom_basis_output_folder", str(self.rom_basis_output_folder))
-                self.__petrov_galerkin_training_utility = PetrovGalerkinTrainingUtility(
-                    self._GetSolver(),
-                    self.rom_parameters)
-
-        def FinalizeSolutionStep(self):
-            if self.train_petrov_galerkin:
-                self.__petrov_galerkin_training_utility.AppendCurrentStepProjectedSystem()
-                ## Delete all .res.mm files when training Petrov-Galerkin with AssembledResiduals
-                files_to_delete_list = glob('*.res.mm')
-                for to_erase_file in files_to_delete_list:
-                    remove(to_erase_file)
-
-            # Call the HROM training utility to append the current step residuals
-            # Note that this needs to be done prior to the other processes to avoid unfixing the BCs
-            if self.train_hrom:
-                self.__hrom_training_utility.AppendCurrentStepResiduals()
-
-            # #FIXME: Make this optional. This must be a process
-            # # Project the ROM solution onto the visualization modelparts
-            # if self.run_hrom:
-            #     model_part_name = self._GetSolver().settings["model_part_name"].GetString()
-            #     visualization_model_part = self.model.GetModelPart("{}.{}Visualization".format(model_part_name, model_part_name))
-            #     KratosROM.RomAuxiliaryUtilities.ProjectRomSolutionIncrementToNodes(
-            #         self.rom_parameters["rom_settings"]["nodal_unknowns"].GetStringArray(),
-            #         visualization_model_part)
-
-            # This calls the physics FinalizeSolutionStep (e.g. BCs)
-            super().FinalizeSolutionStep()
-
-
-        def GetHROM_utility(self):
-            return self.__hrom_training_utility
-
-        def GetPetrovGalerkinTrainUtility(self):
-            return self.__petrov_galerkin_training_utility
-
-
-        def Finalize(self):
-            # This calls the physics Finalize
-            super().Finalize()
-
-            # Once simulation is completed, calculate and save the HROM weights
-            if self.train_hrom and not self.rom_manager:
-                self.__hrom_training_utility.CalculateAndSaveHRomWeights()
-                self.__hrom_training_utility.CreateHRomModelParts()
-
-            # Once simulation is completed, calculate and save the Petrov Galerkin ROM basis
-            if self.train_petrov_galerkin and not self.rom_manager:
-                self.__petrov_galerkin_training_utility.CalculateAndSaveBasis()
-
-    return RomAnalysis(global_model, parameters)
-
-if __name__ == "__main__":
-
-    with open("ProjectParameters.json", 'r') as parameter_file:
-        parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-    analysis_stage_module_name = parameters["analysis_stage"].GetString()
-    analysis_stage_class_name = analysis_stage_module_name.split('.')[-1]
-    analysis_stage_class_name = ''.join(x.title() for x in analysis_stage_class_name.split('_'))
-
-    analysis_stage_module = importlib.import_module(analysis_stage_module_name)
-    analysis_stage_class = getattr(analysis_stage_module, analysis_stage_class_name)
-
-    global_model = KratosMultiphysics.Model()
-    simulation = CreateRomAnalysisInstance(analysis_stage_class, global_model, parameters)
+import importlib
+
+import KratosMultiphysics
+import KratosMultiphysics.RomApplication as KratosROM
+from KratosMultiphysics.RomApplication import python_solvers_wrapper_rom
+from KratosMultiphysics.RomApplication.hrom_training_utility import HRomTrainingUtility
+from KratosMultiphysics.RomApplication.petrov_galerkin_training_utility import PetrovGalerkinTrainingUtility
+from KratosMultiphysics.RomApplication.calculate_rom_basis_output_process import CalculateRomBasisOutputProcess
+import numpy as np
+
+from glob import glob
+from os import remove
+from pathlib import Path
+
+def CreateRomAnalysisInstance(cls, global_model, parameters):
+    class RomAnalysis(cls):
+
+        def __init__(self,global_model, parameters):
+            super().__init__(global_model, parameters)
+
+        def _CreateSolver(self):
+            """ Create the Solver (and create and import the ModelPart if it is not alread in the model) """
+
+            # Assign rom basis output folder and file name
+            self.rom_basis_output_name = 'RomParameters' #Default
+            self.rom_basis_output_folder = 'rom_data' #Default
+            if self.project_parameters.Has("output_processes"):
+                for name in self.project_parameters["output_processes"].keys():
+                    if name=="rom_output":
+                        rom_output_parameters = self.project_parameters["output_processes"]["rom_output"]
+                        for parameter_set in rom_output_parameters:
+                            if parameter_set["python_module"].GetString() == "calculate_rom_basis_output_process":
+                                if parameter_set["Parameters"].Has("rom_basis_output_name"):
+                                    self.rom_basis_output_name = parameter_set["Parameters"]["rom_basis_output_name"].GetString()
+                                if parameter_set["Parameters"].Has("rom_basis_output_folder"):
+                                    self.rom_basis_output_folder = parameter_set["Parameters"]["rom_basis_output_folder"].GetString()
+            self.rom_basis_output_name = Path(self.rom_basis_output_name)
+            self.rom_basis_output_folder = Path(self.rom_basis_output_folder)
+
+            # Get the ROM settings from the RomParameters.json input file
+            with open(self.rom_basis_output_folder / self.rom_basis_output_name.with_suffix('.json')) as rom_parameters:
+                self.rom_parameters = KratosMultiphysics.Parameters(rom_parameters.read())
+
+            # Set the ROM settings in the "solver_settings" of the solver introducing the physics
+            self.project_parameters["solver_settings"].AddValue("rom_settings", self.rom_parameters["rom_settings"])
+
+            # Inner ROM settings
+            self.rom_bns_settings = self.rom_parameters["rom_settings"]["rom_bns_settings"]
+
+            # HROM operations flags
+            self.rom_basis_process_list_check = True
+            self.rom_basis_output_process_check = True
+            self.run_hrom = self.rom_parameters["run_hrom"].GetBool() if self.rom_parameters.Has("run_hrom") else False
+            self.train_hrom = self.rom_parameters["train_hrom"].GetBool() if self.rom_parameters.Has("train_hrom") else False
+            self.rom_manager = self.rom_parameters["rom_manager"].GetBool()
+            if self.run_hrom and self.train_hrom:
+                # Check that train an run HROM are not set at the same time
+                err_msg = "\'run_hrom\' and \'train_hrom\' are both \'true\'. Select either training or running (if training has been already done)."
+                raise Exception(err_msg)
+
+            # Petrov Galerking Training settings
+            self.train_petrov_galerkin = self.rom_bns_settings["train_petrov_galerkin"].GetBool() if self.rom_bns_settings.Has("train_petrov_galerkin") else False
+            if self.train_hrom and self.train_petrov_galerkin:
+                err_msg = "\'train_petrov_galerkin\' and \'train_hrom\' are both \'true\'. Select only one training strategy."
+                raise Exception(err_msg)
+            if (self.train_hrom or self.train_petrov_galerkin) and (self.run_hrom):
+                err_msg = "\'train_petrov_galerkin\' or \'train_hrom\' and \'run_hrom\' are both \'true\'. Select either training or running (if training has been already done)."
+                raise Exception(err_msg)
+
+            # ROM solving strategy
+            self.solving_strategy = self.rom_parameters["projection_strategy"].GetString() if self.rom_parameters.Has("projection_strategy") else "galerkin"
+            self.project_parameters["solver_settings"].AddString("projection_strategy",self.solving_strategy)
+
+            # Add or remove parameters depending on the solving strategy
+            ##LSPG
+            if self.solving_strategy=="lspg":
+                solving_technique = self.rom_bns_settings["solving_technique"].GetString() if self.rom_bns_settings.Has("solving_technique") else "normal_equations"
+                # Check if the solving technique is either "normal_equations" or "qr_decomposition"
+                if solving_technique not in ["normal_equations", "qr_decomposition"]:
+                    err_msg = f"'{solving_technique}' is not a valid solving technique. Choose either 'normal_equations' or 'qr_decomposition'."
+                    raise Exception(err_msg)
+
+                self.project_parameters["solver_settings"]["rom_settings"]["rom_bns_settings"].AddString("solving_technique", solving_technique)
+                self.project_parameters["solver_settings"]["rom_settings"]["rom_bns_settings"].AddBool("train_petrov_galerkin", self.train_petrov_galerkin)
+                #Adding the basis strategy for generating the left ROB for the Petrov-Galerkin ROM.
+                petrov_galerkin_basis_strategy = self.rom_bns_settings["basis_strategy"].GetString() if self.rom_bns_settings.Has("basis_strategy") else "residuals"
+                self.project_parameters["solver_settings"]["rom_settings"]["rom_bns_settings"].AddString("basis_strategy", petrov_galerkin_basis_strategy)
+
+            ##Petrov Galerkin
+            if self.solving_strategy=="petrov_galerkin":
+                self.petrov_galerkin_rom_dofs = self.project_parameters["solver_settings"]["rom_settings"]["petrov_galerkin_number_of_rom_dofs"].GetInt()
+            else:
+                self.project_parameters["solver_settings"]["rom_settings"].RemoveValue("petrov_galerkin_number_of_rom_dofs")
+
+            # ROM assembling strategy
+            self.assembling_strategy = self.rom_parameters["assembling_strategy"].GetString() if self.rom_parameters.Has("assembling_strategy") else "global"
+            self.project_parameters["solver_settings"].AddString("assembling_strategy",self.assembling_strategy)
+
+            # Create the ROM solver
+            return python_solvers_wrapper_rom.CreateSolver(
+                self.model,
+                self.project_parameters)
+
+        def _GetListOfProcesses(self):
+            # Get the already existent processes list
+            list_of_processes = super()._GetListOfProcesses()
+
+            # Check if there is any instance of ROM basis output
+            if self.rom_basis_process_list_check and not self.rom_manager: #eliminate the RomOutputProcess if not run inside the RomManager
+                for process in list_of_processes:
+                    if isinstance(process, KratosROM.calculate_rom_basis_output_process.CalculateRomBasisOutputProcess):
+                        warn_msg = "\'CalculateRomBasisOutputProcess\' instance found in ROM stage. Basis must be already stored in \'RomParameters.json\'. Removing instance from processes list."
+                        KratosMultiphysics.Logger.PrintWarning("RomAnalysis", warn_msg)
+                        list_of_processes.remove(process)
+                self.rom_basis_process_list_check = False
+
+            return list_of_processes
+
+        def _GetListOfOutputProcesses(self):
+            # Get the already existent output processes list
+            list_of_output_processes = super()._GetListOfOutputProcesses()
+
+            # Check if there is any instance of ROM basis output
+            if self.rom_basis_output_process_check and not self.rom_manager: #eliminate the RomOutputProcess if not run inside the RomManager
+                for process in list_of_output_processes:
+                    if isinstance(process, KratosROM.calculate_rom_basis_output_process.CalculateRomBasisOutputProcess):
+                        warn_msg = "\'CalculateRomBasisOutputProcess\' instance found in ROM stage. Basis must be already stored in \'RomParameters.json\'. Removing instance from output processes list."
+                        KratosMultiphysics.Logger.PrintWarning("RomAnalysis", warn_msg)
+                        list_of_output_processes.remove(process)
+                self.rom_basis_output_process_check = False
+
+            return list_of_output_processes
+
+        def _GetSimulationName(self):
+            return "::[ROM Simulation]:: "
+
+        def ModifyAfterSolverInitialize(self):
+            """Here is where the ROM_BASIS is imposed to each node"""
+            super().ModifyAfterSolverInitialize()
+
+            # Get the model part where the ROM is to be applied
+            computing_model_part = self._GetSolver().GetComputingModelPart().GetRootModelPart()
+            # computing_model_part = self._GetSolver().GetComputingModelPart()
+
+            # Set ROM basis
+            nodal_modes = self.rom_parameters["nodal_modes"]
+            nodal_dofs = len(self.project_parameters["solver_settings"]["rom_settings"]["nodal_unknowns"].GetStringArray())
+            rom_dofs = self.project_parameters["solver_settings"]["rom_settings"]["number_of_rom_dofs"].GetInt()
+
+            # Set the right nodal ROM basis
+            if self.rom_parameters["rom_format"].GetString() == "json":
+                aux = KratosMultiphysics.Matrix(nodal_dofs, rom_dofs)
+                for node in computing_model_part.Nodes:
+                    node_id = str(node.Id)
+                    for j in range(nodal_dofs):
+                        for i in range(rom_dofs):
+                            aux[j,i] = nodal_modes[node_id][j][i].GetDouble()
+                    node.SetValue(KratosROM.ROM_BASIS, aux)
+
+                # Set the left nodal ROM basis if it is different than the right nodal ROM basis (i.e. Petrov-Galerkin)
+                if (self.solving_strategy == "petrov_galerkin"):
+                    petrov_galerkin_nodal_modes = self.rom_parameters["petrov_galerkin_nodal_modes"]
+                    petrov_galerkin_nodal_dofs = len(self.project_parameters["solver_settings"]["rom_settings"]["nodal_unknowns"].GetStringArray())
+                    aux = KratosMultiphysics.Matrix(petrov_galerkin_nodal_dofs, self.petrov_galerkin_rom_dofs)
+                    for node in computing_model_part.Nodes:
+                        node_id = str(node.Id)
+                        for j in range(petrov_galerkin_nodal_dofs):
+                            for i in range(self.petrov_galerkin_rom_dofs):
+                                aux[j,i] = petrov_galerkin_nodal_modes[node_id][j][i].GetDouble()
+                        node.SetValue(KratosROM.ROM_LEFT_BASIS, aux)
+
+            elif self.rom_parameters["rom_format"].GetString() == "numpy":
+
+                # Load node IDs and right modes
+                node_ids = np.load(self.rom_basis_output_folder / "NodeIds.npy")
+                right_modes = np.load(self.rom_basis_output_folder / "RightBasisMatrix.npy")
+
+                # Ensure right_modes is a 2D array
+                if right_modes.ndim == 1:
+                    right_modes = right_modes.reshape(-1, 1)
+
+                # Trim right_modes based on ROM degrees of freedom (DOFs)
+                right_modes = right_modes[:, :rom_dofs]
+
+                # Handle left modes for Petrov-Galerkin strategy
+                if self.solving_strategy == "petrov_galerkin":
+                    petrov_galerkin_rom_dofs = self.project_parameters["solver_settings"]["rom_settings"]["petrov_galerkin_number_of_rom_dofs"].GetInt()
+                    left_modes = np.load(self.rom_basis_output_folder / "LeftBasisMatrix.npy")
+
+                    # Ensure left_modes is a 2D array
+                    if left_modes.ndim == 1:
+                        left_modes = left_modes.reshape(-1, 1)
+
+                    # Trim left_modes based on Petrov-Galerkin ROM DOFs
+                    left_modes = left_modes[:, :petrov_galerkin_rom_dofs]
+
+                # Preprocess to create a mapping from node ID to index
+                node_id_to_index = {nid: idx for idx, nid in enumerate(node_ids)}
+
+                # Loop over each node in computing_model_part
+                for node in computing_model_part.Nodes:
+                    index = node_id_to_index[node.Id]
+                    offset = index * nodal_dofs
+
+                    # Set ROM basis for the node
+                    node.SetValue(KratosROM.ROM_BASIS, KratosMultiphysics.Matrix(right_modes[offset:offset + nodal_dofs, :]))
+
+                    # Set Petrov-Galerkin ROM basis if applicable
+                    if self.solving_strategy == "petrov_galerkin":
+                        node.SetValue(KratosROM.ROM_LEFT_BASIS, KratosMultiphysics.Matrix(left_modes[offset:offset + nodal_dofs, :]))
+
+            # Check for HROM stages
+            if self.train_hrom:
+                # Pass the name of the Rom Parameters file and folder
+                self.rom_parameters.AddString("rom_basis_output_name", str(self.rom_basis_output_name))
+                self.rom_parameters.AddString("rom_basis_output_folder", str(self.rom_basis_output_folder))
+                # Create the training utility to calculate the HROM weights
+                self.__hrom_training_utility = HRomTrainingUtility(
+                    self._GetSolver(),
+                    self.rom_parameters)
+            elif self.run_hrom:
+                if self.rom_parameters["hrom_settings"]["hrom_format"].GetString() == "json":
+                    # Set the HROM weights in elements and conditions
+                    hrom_weights_elements = self.rom_parameters["elements_and_weights"]["Elements"]
+                    for key,value in zip(hrom_weights_elements.keys(), hrom_weights_elements.values()):
+                        computing_model_part.GetElement(int(key)+1).SetValue(KratosROM.HROM_WEIGHT, value.GetDouble()) #FIXME: FIX THE +1
+                    hrom_weights_condtions = self.rom_parameters["elements_and_weights"]["Conditions"]
+                    for key,value in zip(hrom_weights_condtions.keys(), hrom_weights_condtions.values()):
+                        computing_model_part.GetCondition(int(key)+1).SetValue(KratosROM.HROM_WEIGHT, value.GetDouble()) #FIXME: FIX THE +1
+                elif self.rom_parameters["hrom_settings"]["hrom_format"].GetString() == "numpy":
+                    # Set the HROM weights in elements and conditions
+                    element_indexes = np.load(f"{self.rom_basis_output_folder}/HROM_ElementIds.npy")
+                    element_weights = np.load(f"{self.rom_basis_output_folder}/HROM_ElementWeights.npy")
+                    condition_indexes = np.load(f"{self.rom_basis_output_folder}/HROM_ConditionIds.npy")
+                    conditon_weights = np.load(f"{self.rom_basis_output_folder}/HROM_ConditionWeights.npy")
+                    for i in range(np.size(element_indexes)):
+                        computing_model_part.GetElement(int( element_indexes[i])+1).SetValue(KratosROM.HROM_WEIGHT, element_weights[i]  ) #FIXME: FIX THE +1
+                    for i in range(np.size(condition_indexes)):
+                        computing_model_part.GetCondition(int( condition_indexes[i])+1).SetValue(KratosROM.HROM_WEIGHT, conditon_weights[i]  ) #FIXME: FIX THE +1
+
+
+            # Check and Initialize Petrov Galerkin Training stage
+            if self.train_petrov_galerkin:
+                # Pass the name of the Rom Parameters file and folder
+                self.rom_parameters.AddString("rom_basis_output_name", str(self.rom_basis_output_name))
+                self.rom_parameters.AddString("rom_basis_output_folder", str(self.rom_basis_output_folder))
+                self.__petrov_galerkin_training_utility = PetrovGalerkinTrainingUtility(
+                    self._GetSolver(),
+                    self.rom_parameters)
+
+        def FinalizeSolutionStep(self):
+            if self.train_petrov_galerkin:
+                self.__petrov_galerkin_training_utility.AppendCurrentStepProjectedSystem()
+                ## Delete all .res.mm files when training Petrov-Galerkin with AssembledResiduals
+                files_to_delete_list = glob('*.res.mm')
+                for to_erase_file in files_to_delete_list:
+                    remove(to_erase_file)
+
+            # Call the HROM training utility to append the current step residuals
+            # Note that this needs to be done prior to the other processes to avoid unfixing the BCs
+            if self.train_hrom:
+                self.__hrom_training_utility.AppendCurrentStepResiduals()
+
+            # #FIXME: Make this optional. This must be a process
+            # # Project the ROM solution onto the visualization modelparts
+            # if self.run_hrom:
+            #     model_part_name = self._GetSolver().settings["model_part_name"].GetString()
+            #     visualization_model_part = self.model.GetModelPart("{}.{}Visualization".format(model_part_name, model_part_name))
+            #     KratosROM.RomAuxiliaryUtilities.ProjectRomSolutionIncrementToNodes(
+            #         self.rom_parameters["rom_settings"]["nodal_unknowns"].GetStringArray(),
+            #         visualization_model_part)
+
+            # This calls the physics FinalizeSolutionStep (e.g. BCs)
+            super().FinalizeSolutionStep()
+
+
+        def GetHROM_utility(self):
+            return self.__hrom_training_utility
+
+        def GetPetrovGalerkinTrainUtility(self):
+            return self.__petrov_galerkin_training_utility
+
+
+        def Finalize(self):
+            # This calls the physics Finalize
+            super().Finalize()
+
+            # Once simulation is completed, calculate and save the HROM weights
+            if self.train_hrom and not self.rom_manager:
+                self.__hrom_training_utility.CalculateAndSaveHRomWeights()
+                self.__hrom_training_utility.CreateHRomModelParts()
+
+            # Once simulation is completed, calculate and save the Petrov Galerkin ROM basis
+            if self.train_petrov_galerkin and not self.rom_manager:
+                self.__petrov_galerkin_training_utility.CalculateAndSaveBasis()
+
+    return RomAnalysis(global_model, parameters)
+
+if __name__ == "__main__":
+
+    with open("ProjectParameters.json", 'r') as parameter_file:
+        parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+    analysis_stage_module_name = parameters["analysis_stage"].GetString()
+    analysis_stage_class_name = analysis_stage_module_name.split('.')[-1]
+    analysis_stage_class_name = ''.join(x.title() for x in analysis_stage_class_name.split('_'))
+
+    analysis_stage_module = importlib.import_module(analysis_stage_module_name)
+    analysis_stage_class = getattr(analysis_stage_module, analysis_stage_class_name)
+
+    global_model = KratosMultiphysics.Model()
+    simulation = CreateRomAnalysisInstance(analysis_stage_class, global_model, parameters)
     simulation.Run()
```

## KratosMultiphysics/RomApplication/rom_manager.py

```diff
@@ -1,848 +1,849 @@
-import KratosMultiphysics
-from KratosMultiphysics.RomApplication.rom_testing_utilities import SetUpSimulationInstance
-from KratosMultiphysics.RomApplication.calculate_rom_basis_output_process import CalculateRomBasisOutputProcess
-from KratosMultiphysics.RomApplication.randomized_singular_value_decomposition import RandomizedSingularValueDecomposition
-import numpy as np
-import importlib
-import json
-from pathlib import Path
-
-
-
-class RomManager(object):
-
-    def __init__(self,project_parameters_name, general_rom_manager_parameters, CustomizeSimulation, UpdateProjectParameters,UpdateMaterialParametersFile):
-        #FIXME:
-        # - Use a method (upcoming) for smothly retrieving solutions. In here we are using the RomBasisOutput process in order to store the solutions
-        # - There is some redundancy between the methods that launch the simulations. Can we create a single method?
-        # - We must use the Hyper-Reduced model part for the HROM simulations. (The one in which we have eliminated the non selected elements and conditions)
-        # - Not yet paralellised with COMPSs
-        self.project_parameters_name = project_parameters_name
-        self.general_rom_manager_parameters = general_rom_manager_parameters
-        self.rom_training_parameters = self._SetRomTrainingParameters()
-        self.hrom_training_parameters = self.SetHromTrainingParameters()
-        self.CustomizeSimulation = CustomizeSimulation
-        self.UpdateProjectParameters = UpdateProjectParameters
-        self.UpdateMaterialParametersFile = UpdateMaterialParametersFile
-        self.SetUpQuantityOfInterestContainers()
-
-
-    def Fit(self, mu_train=[None], store_all_snapshots=False, store_fom_snapshots=False, store_rom_snapshots=False, store_hrom_snapshots=False, store_residuals_projected = False):
-        chosen_projection_strategy = self.general_rom_manager_parameters["projection_strategy"].GetString()
-        training_stages = self.general_rom_manager_parameters["rom_stages_to_train"].GetStringArray()
-        #######################
-        ######  Galerkin ######
-        if chosen_projection_strategy == "galerkin":
-            if any(item == "ROM" for item in training_stages):
-                fom_snapshots = self.__LaunchTrainROM(mu_train)
-                if store_all_snapshots or store_fom_snapshots:
-                    self._StoreSnapshotsMatrix('fom_snapshots', fom_snapshots)
-                self._ChangeRomFlags(simulation_to_run = "GalerkinROM")
-                rom_snapshots = self.__LaunchROM(mu_train)
-                if store_all_snapshots or store_rom_snapshots:
-                    self._StoreSnapshotsMatrix('rom_snapshots', rom_snapshots)
-                self.ROMvsFOM_train = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
-
-            if any(item == "HROM" for item in training_stages):
-                #FIXME there will be an error if we only train HROM, but not ROM
-                self._ChangeRomFlags(simulation_to_run = "trainHROMGalerkin")
-                self.__LaunchTrainHROM(mu_train, store_residuals_projected)
-                self._ChangeRomFlags(simulation_to_run = "runHROMGalerkin")
-                hrom_snapshots = self.__LaunchHROM(mu_train)
-                if store_all_snapshots or store_hrom_snapshots:
-                    self._StoreSnapshotsMatrix('hrom_snapshots', hrom_snapshots)
-                self.ROMvsHROM_train = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
-        #######################
-
-        #######################################
-        ##  Least-Squares Petrov Galerkin   ###
-        elif chosen_projection_strategy == "lspg":
-            if any(item == "ROM" for item in training_stages):
-                fom_snapshots = self.__LaunchTrainROM(mu_train)
-                if store_all_snapshots or store_fom_snapshots:
-                    self._StoreSnapshotsMatrix('fom_snapshots', fom_snapshots)
-                self._ChangeRomFlags(simulation_to_run = "lspg")
-                rom_snapshots = self.__LaunchROM(mu_train)
-                if store_all_snapshots or store_rom_snapshots:
-                    self._StoreSnapshotsMatrix('rom_snapshots', rom_snapshots)
-                self.ROMvsFOM_train = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
-            if any(item == "HROM" for item in training_stages):
-                # Change the flags to train the HROM for LSPG
-                self._ChangeRomFlags(simulation_to_run = "trainHROMLSPG")
-                self.__LaunchTrainHROM(mu_train, store_residuals_projected)
-
-                # Change the flags to run the HROM for LSPG
-                self._ChangeRomFlags(simulation_to_run = "runHROMLSPG")
-                hrom_snapshots = self.__LaunchHROM(mu_train)
-
-                if store_all_snapshots or store_hrom_snapshots:
-                    self._StoreSnapshotsMatrix('hrom_snapshots', hrom_snapshots)
-
-                self.ROMvsHROM_train = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
-                #######################################
-
-        ##########################
-        ###  Petrov Galerkin   ###
-        elif chosen_projection_strategy == "petrov_galerkin":
-            if any(item == "ROM" for item in training_stages):
-                fom_snapshots = self.__LaunchTrainROM(mu_train)
-                if store_all_snapshots or store_fom_snapshots:
-                    self._StoreSnapshotsMatrix('fom_snapshots', fom_snapshots)
-                self._ChangeRomFlags(simulation_to_run = "TrainPG")
-                self.__LaunchTrainPG(mu_train)
-                self._ChangeRomFlags(simulation_to_run = "PG")
-                rom_snapshots = self.__LaunchROM(mu_train)
-                if store_all_snapshots or store_rom_snapshots:
-                    self._StoreSnapshotsMatrix('rom_snapshots', rom_snapshots)
-                self.ROMvsFOM_train = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
-            if any(item == "HROM" for item in training_stages):
-                #FIXME there will be an error if we only train HROM, but not ROM
-                self._ChangeRomFlags(simulation_to_run = "trainHROMPetrovGalerkin")
-                self.__LaunchTrainHROM(mu_train, store_residuals_projected)
-                self._ChangeRomFlags(simulation_to_run = "runHROMPetrovGalerkin")
-                hrom_snapshots = self.__LaunchHROM(mu_train)
-                if store_all_snapshots or store_hrom_snapshots:
-                    self._StoreSnapshotsMatrix('hrom_snapshots', hrom_snapshots)
-                self.ROMvsHROM_train = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
-        ##########################
-        else:
-            err_msg = f'Provided projection strategy {chosen_projection_strategy} is not supported. Available options are \'galerkin\', \'lspg\' and \'petrov_galerkin\'.'
-            raise Exception(err_msg)
-
-
-
-    def Test(self, mu_test=[None]):
-        chosen_projection_strategy = self.general_rom_manager_parameters["projection_strategy"].GetString()
-        testing_stages = self.general_rom_manager_parameters["rom_stages_to_test"].GetStringArray()
-        #######################
-        ######  Galerkin ######
-        if chosen_projection_strategy == "galerkin":
-            if any(item == "ROM" for item in testing_stages):
-                fom_snapshots = self.__LaunchTestFOM(mu_test)
-                self._ChangeRomFlags(simulation_to_run = "GalerkinROM")
-                rom_snapshots = self.__LaunchTestROM(mu_test)
-                self.ROMvsFOM_test = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
-
-            if any(item == "HROM" for item in testing_stages):
-                #FIXME there will be an error if we only test HROM, but not ROM
-                self._ChangeRomFlags(simulation_to_run = "runHROMGalerkin")
-                hrom_snapshots = self.__LaunchTestHROM(mu_test)
-                self.ROMvsHROM_test = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
-
-
-        #######################################
-        ##  Least-Squares Petrov Galerkin   ###
-        elif chosen_projection_strategy == "lspg":
-            if any(item == "ROM" for item in testing_stages):
-                fom_snapshots = self.__LaunchTestFOM(mu_test)
-                self._ChangeRomFlags(simulation_to_run = "lspg")
-                rom_snapshots = self.__LaunchTestROM(mu_test)
-                self.ROMvsFOM_test = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
-            if any(item == "HROM" for item in testing_stages):
-                self._ChangeRomFlags(simulation_to_run = "runHROMLSPG")
-                hrom_snapshots = self.__LaunchTestHROM(mu_test)
-                self.ROMvsHROM_test = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
-        #######################################
-
-
-        ##########################
-        ###  Petrov Galerkin   ###
-        elif chosen_projection_strategy == "petrov_galerkin":
-            if any(item == "ROM" for item in testing_stages):
-                fom_snapshots = self.__LaunchTestFOM(mu_test)
-                self._ChangeRomFlags(simulation_to_run = "PG")
-                rom_snapshots = self.__LaunchTestROM(mu_test)
-                self.ROMvsFOM_test = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
-            if any(item == "HROM" for item in testing_stages):
-                #FIXME there will be an error if we only train HROM, but not ROM
-                self._ChangeRomFlags(simulation_to_run = "runHROMPetrovGalerkin")
-                hrom_snapshots = self.__LaunchTestHROM(mu_test)
-                self.ROMvsHROM_test = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
-        ##########################
-        else:
-            err_msg = f'Provided projection strategy {chosen_projection_strategy} is not supported. Available options are \'galerkin\', \'lspg\' and \'petrov_galerkin\'.'
-            raise Exception(err_msg)
-
-
-
-
-    def RunFOM(self, mu_run=[None]):
-        self.__LaunchRunFOM(mu_run)
-
-    def RunROM(self, mu_run=[None]):
-        chosen_projection_strategy = self.general_rom_manager_parameters["projection_strategy"].GetString()
-        #######################
-        ######  Galerkin ######
-        if chosen_projection_strategy == "galerkin":
-            self._ChangeRomFlags(simulation_to_run = "GalerkinROM")
-        #######################################
-        ##  Least-Squares Petrov Galerkin   ###
-        elif chosen_projection_strategy == "lspg":
-            self._ChangeRomFlags(simulation_to_run = "lspg")
-        ##########################
-        ###  Petrov Galerkin   ###
-        elif chosen_projection_strategy == "petrov_galerkin":
-            self._ChangeRomFlags(simulation_to_run = "PG")
-        else:
-            err_msg = f'Provided projection strategy {chosen_projection_strategy} is not supported. Available options are \'galerkin\', \'lspg\' and \'petrov_galerkin\'.'
-            raise Exception(err_msg)
-        self.__LaunchRunROM(mu_run)
-
-    def RunHROM(self, mu_run=[None], use_full_model_part = False):
-        chosen_projection_strategy = self.general_rom_manager_parameters["projection_strategy"].GetString()
-        #######################
-        ######  Galerkin ######
-        if chosen_projection_strategy == "galerkin":
-            self._ChangeRomFlags(simulation_to_run = "runHROMGalerkin")
-        #######################################
-        ##  Least-Squares Petrov Galerkin   ###
-        elif chosen_projection_strategy == "lspg":
-            self._ChangeRomFlags(simulation_to_run = "runHROMLSPG")
-        ##########################
-        ###  Petrov Galerkin   ###
-        elif chosen_projection_strategy == "petrov_galerkin":
-            self._ChangeRomFlags(simulation_to_run = "runHROMPetrovGalerkin")
-        else:
-            err_msg = f'Provided projection strategy {chosen_projection_strategy} is not supported. Available options are \'galerkin\', \'lspg\' and \'petrov_galerkin\'.'
-            raise Exception(err_msg)
-        self.__LaunchRunHROM(mu_run, use_full_model_part)
-
-
-    def PrintErrors(self):
-        chosen_projection_strategy = self.general_rom_manager_parameters["projection_strategy"].GetString()
-        training_stages = self.general_rom_manager_parameters["rom_stages_to_train"].GetStringArray()
-        testing_stages = self.general_rom_manager_parameters["rom_stages_to_test"].GetStringArray()
-        if any(item == "ROM" for item in training_stages):
-            print("approximation error in train set FOM vs ROM: ", self.ROMvsFOM_train)
-        if any(item == "HROM" for item in training_stages):
-            print("approximation error in train set ROM vs HROM: ", self.ROMvsHROM_train)
-        if any(item == "ROM" for item in testing_stages):
-            print("approximation error in test set FOM vs ROM: ", self.ROMvsFOM_test)
-        if any(item == "HROM" for item in testing_stages):
-            print("approximation error in test set ROM vs HROM: ",  self.ROMvsHROM_test)
-
-
-    def __LaunchTrainROM(self, mu_train):
-        """
-        This method should be parallel capable
-        """
-        with open(self.project_parameters_name,'r') as parameter_file:
-            parameters = KratosMultiphysics.Parameters(parameter_file.read())
-        SnapshotsMatrix = []
-        for Id, mu in enumerate(mu_train):
-            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
-            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy) #TODO stop using the RomBasisOutputProcess to store the snapshots. Use instead the upcoming build-in function
-            parameters_copy = self._StoreResultsByName(parameters_copy,'FOM_Fit',mu,Id)
-            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
-            self.UpdateMaterialParametersFile(materials_file_name, mu)
-            model = KratosMultiphysics.Model()
-            analysis_stage_class = self._GetAnalysisStageClass(parameters_copy)
-            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
-            simulation.Run()
-            self.QoI_Fit_FOM.append(simulation.GetFinalData())
-            for process in simulation._GetListOfOutputProcesses():
-                if isinstance(process, CalculateRomBasisOutputProcess):
-                    BasisOutputProcess = process
-            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
-        SnapshotsMatrix = np.block(SnapshotsMatrix)
-        BasisOutputProcess._PrintRomBasis(SnapshotsMatrix) #Calling the RomOutput Process for creating the RomParameter.json
-
-        return SnapshotsMatrix
-
-
-    def __LaunchROM(self, mu_train):
-        """
-        This method should be parallel capable
-        """
-        with open(self.project_parameters_name,'r') as parameter_file:
-            parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-        SnapshotsMatrix = []
-        for Id, mu in enumerate(mu_train):
-            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
-            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)  #TODO stop using the RomBasisOutputProcess to store the snapshots. Use instead the upcoming build-in function
-            parameters_copy = self._StoreResultsByName(parameters_copy,'ROM_Fit',mu,Id)
-            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
-            self.UpdateMaterialParametersFile(materials_file_name, mu)
-            model = KratosMultiphysics.Model()
-            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
-            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
-            simulation.Run()
-            self.QoI_Fit_ROM.append(simulation.GetFinalData())
-            for process in simulation._GetListOfOutputProcesses():
-                if isinstance(process, CalculateRomBasisOutputProcess):
-                    BasisOutputProcess = process
-            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
-        SnapshotsMatrix = np.block(SnapshotsMatrix)
-
-        return SnapshotsMatrix
-
-
-    def __LaunchTrainPG(self, mu_train):
-        """
-        This method should be parallel capable
-        """
-        with open(self.project_parameters_name,'r') as parameter_file:
-            parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-        PetrovGalerkinTrainMatrix = []
-        for Id, mu in enumerate(mu_train):
-            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
-            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)
-            parameters_copy = self._StoreNoResults(parameters_copy)
-            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
-            self.UpdateMaterialParametersFile(materials_file_name, mu)
-            model = KratosMultiphysics.Model()
-            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
-            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
-            simulation.Run()
-            PetrovGalerkinTrainMatrix.append(simulation.GetPetrovGalerkinTrainUtility()._GetSnapshotsMatrix()) #TODO is the best way of extracting the Projected Residuals calling the HROM residuals utility?
-        simulation.GetPetrovGalerkinTrainUtility().CalculateAndSaveBasis(np.block(PetrovGalerkinTrainMatrix))
-
-
-    def __LaunchTrainHROM(self, mu_train, store_residuals_projected=False):
-        """
-        This method should be parallel capable
-        """
-        with open(self.project_parameters_name,'r') as parameter_file:
-            parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-        RedidualsSnapshotsMatrix = []
-        for mu in mu_train:
-            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
-            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)
-            parameters_copy = self._StoreNoResults(parameters_copy)
-            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
-            self.UpdateMaterialParametersFile(materials_file_name, mu)
-            model = KratosMultiphysics.Model()
-            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
-            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
-            simulation.Run()
-            RedidualsSnapshotsMatrix.append(simulation.GetHROM_utility()._GetResidualsProjectedMatrix()) #TODO is the best way of extracting the Projected Residuals calling the HROM residuals utility?
-        RedidualsSnapshotsMatrix = np.block(RedidualsSnapshotsMatrix)
-        if store_residuals_projected:
-            self._StoreSnapshotsMatrix('residuals_projected',RedidualsSnapshotsMatrix)
-        u,_,_,_ = RandomizedSingularValueDecomposition(COMPUTE_V=False).Calculate(RedidualsSnapshotsMatrix,
-        self.hrom_training_parameters["element_selection_svd_truncation_tolerance"].GetDouble())
-        simulation.GetHROM_utility().hyper_reduction_element_selector.SetUp(u, InitialCandidatesSet = simulation.GetHROM_utility().candidate_ids)
-        simulation.GetHROM_utility().hyper_reduction_element_selector.Run()
-        if not simulation.GetHROM_utility().hyper_reduction_element_selector.success:
-            KratosMultiphysics.Logger.PrintWarning("HRomTrainingUtility", "The Empirical Cubature Method did not converge using the initial set of candidates. Launching again without initial candidates.")
-            #Imposing an initial candidate set can lead to no convergence. Restart without imposing the initial candidate set
-            simulation.GetHROM_utility().hyper_reduction_element_selector.SetUp(u, InitialCandidatesSet = None)
-            simulation.GetHROM_utility().hyper_reduction_element_selector.Run()
-        simulation.GetHROM_utility().AppendHRomWeightsToRomParameters()
-        simulation.GetHROM_utility().CreateHRomModelParts()
-
-
-    def __LaunchHROM(self, mu_train):
-        """
-        This method should be parallel capable
-        """
-        with open(self.project_parameters_name,'r') as parameter_file:
-            parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-        SnapshotsMatrix = []
-        for Id, mu in enumerate(mu_train):
-            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
-            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)
-            parameters_copy = self._StoreResultsByName(parameters_copy,'HROM_Fit',mu,Id)
-            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
-            self.UpdateMaterialParametersFile(materials_file_name, mu)
-            model = KratosMultiphysics.Model()
-            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
-            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
-            simulation.Run()
-            self.QoI_Fit_HROM.append(simulation.GetFinalData())
-            for process in simulation._GetListOfOutputProcesses():
-                if isinstance(process, CalculateRomBasisOutputProcess):
-                    BasisOutputProcess = process
-            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
-        SnapshotsMatrix = np.block(SnapshotsMatrix)
-
-        return SnapshotsMatrix
-
-
-    def __LaunchTestFOM(self, mu_test):
-        """
-        This method should be parallel capable
-        """
-        # FIXME We must include a method to retrive solutions in the nodes and stop using the CalculateRomBasisOutputProcess to stote snapshots
-        with open(self.project_parameters_name,'r') as parameter_file:
-            parameters = KratosMultiphysics.Parameters(parameter_file.read())
-        SnapshotsMatrix = []
-        for Id, mu in enumerate(mu_test):
-            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
-            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy) #TODO stop using the RomBasisOutputProcess to store the snapshots. Use instead the upcoming build-in function
-            parameters_copy = self._StoreResultsByName(parameters_copy,'FOM_Test',mu,Id)
-            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
-            self.UpdateMaterialParametersFile(materials_file_name, mu)
-            model = KratosMultiphysics.Model()
-            analysis_stage_class = self._GetAnalysisStageClass(parameters_copy)
-            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
-            simulation.Run()
-            self.QoI_Test_FOM.append(simulation.GetFinalData())
-            for process in simulation._GetListOfOutputProcesses():
-                if isinstance(process, CalculateRomBasisOutputProcess):
-                    BasisOutputProcess = process
-            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
-        SnapshotsMatrix = np.block(SnapshotsMatrix)
-
-
-        return SnapshotsMatrix
-
-
-    def __LaunchTestROM(self, mu_test):
-        """
-        This method should be parallel capable
-        """
-        with open(self.project_parameters_name,'r') as parameter_file:
-            parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-        SnapshotsMatrix = []
-        for Id, mu in enumerate(mu_test):
-            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
-            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)  #TODO stop using the RomBasisOutputProcess to store the snapshots. Use instead the upcoming build-in function
-            parameters_copy = self._StoreResultsByName(parameters_copy,'ROM_Test',mu,Id)
-            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
-            self.UpdateMaterialParametersFile(materials_file_name, mu)
-            model = KratosMultiphysics.Model()
-            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
-            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
-            simulation.Run()
-            self.QoI_Test_ROM.append(simulation.GetFinalData())
-            for process in simulation._GetListOfOutputProcesses():
-                if isinstance(process, CalculateRomBasisOutputProcess):
-                    BasisOutputProcess = process
-            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
-        SnapshotsMatrix = np.block(SnapshotsMatrix)
-
-        return SnapshotsMatrix
-
-
-
-    def __LaunchTestHROM(self, mu_test):
-        """
-        This method should be parallel capable
-        """
-        with open(self.project_parameters_name,'r') as parameter_file:
-            parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-        SnapshotsMatrix = []
-        for Id, mu in enumerate(mu_test):
-            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
-            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)
-            parameters_copy = self._StoreResultsByName(parameters_copy,'HROM_Test',mu,Id)
-            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
-            self.UpdateMaterialParametersFile(materials_file_name, mu)
-            model = KratosMultiphysics.Model()
-            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
-            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
-            simulation.Run()
-            self.QoI_Test_HROM.append(simulation.GetFinalData())
-            for process in simulation._GetListOfOutputProcesses():
-                if isinstance(process, CalculateRomBasisOutputProcess):
-                    BasisOutputProcess = process
-            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
-        SnapshotsMatrix = np.block(SnapshotsMatrix)
-
-        return SnapshotsMatrix
-
-
-    def __LaunchRunFOM(self, mu_run):
-        """
-        This method should be parallel capable
-        """
-        with open(self.project_parameters_name,'r') as parameter_file:
-            parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-        for Id, mu in enumerate(mu_run):
-            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
-            parameters_copy = self._StoreResultsByName(parameters_copy,'FOM_Run',mu,Id)
-            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
-            self.UpdateMaterialParametersFile(materials_file_name, mu)
-            model = KratosMultiphysics.Model()
-            analysis_stage_class = self._GetAnalysisStageClass(parameters_copy)
-            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
-            simulation.Run()
-            self.QoI_Run_FOM.append(simulation.GetFinalData())
-
-
-    def __LaunchRunROM(self, mu_run):
-        """
-        This method should be parallel capable
-        """
-        with open(self.project_parameters_name,'r') as parameter_file:
-            parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-        for Id, mu in enumerate(mu_run):
-            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
-            parameters_copy = self._StoreResultsByName(parameters_copy,'ROM_Run',mu,Id)
-            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
-            self.UpdateMaterialParametersFile(materials_file_name, mu)
-            model = KratosMultiphysics.Model()
-            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
-            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
-            simulation.Run()
-            self.QoI_Run_ROM.append(simulation.GetFinalData())
-
-
-    def __LaunchRunHROM(self, mu_run, use_full_model_part):
-        """
-        This method should be parallel capable
-        """
-        with open(self.project_parameters_name,'r') as parameter_file:
-            parameters = KratosMultiphysics.Parameters(parameter_file.read())
-        if not use_full_model_part:
-            model_part_name = parameters["solver_settings"]["model_import_settings"]["input_filename"].GetString()
-            parameters["solver_settings"]["model_import_settings"]["input_filename"].SetString(f"{model_part_name}HROM")
-
-        for Id, mu in enumerate(mu_run):
-            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
-            parameters_copy = self._StoreResultsByName(parameters_copy,'HROM_Run',mu,Id)
-            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
-            self.UpdateMaterialParametersFile(materials_file_name, mu)
-            model = KratosMultiphysics.Model()
-            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
-            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
-            simulation.Run()
-            self.QoI_Run_HROM.append(simulation.GetFinalData())
-
-
-    def _AddHromParametersToRomParameters(self,f):
-        f["hrom_settings"]["element_selection_type"] = self.hrom_training_parameters["element_selection_type"].GetString()
-        f["hrom_settings"]["element_selection_svd_truncation_tolerance"] = self.hrom_training_parameters["element_selection_svd_truncation_tolerance"].GetDouble()
-        f["hrom_settings"]["create_hrom_visualization_model_part"] = self.hrom_training_parameters["create_hrom_visualization_model_part"].GetBool()
-        f["hrom_settings"]["echo_level"] = self.hrom_training_parameters["echo_level"].GetInt()
-        f["hrom_settings"]["include_condition_parents"] = self.hrom_training_parameters["include_condition_parents"].GetBool()
-        f["hrom_settings"]["initial_candidate_elements_model_part_list"] = self.hrom_training_parameters["initial_candidate_elements_model_part_list"].GetStringArray()
-        f["hrom_settings"]["initial_candidate_conditions_model_part_list"] = self.hrom_training_parameters["initial_candidate_conditions_model_part_list"].GetStringArray()
-        f["hrom_settings"]["constraint_sum_weights"] = self.hrom_training_parameters["constraint_sum_weights"].GetBool()
-
-    def _ChangeRomFlags(self, simulation_to_run = 'ROM'):
-        """
-        This method updates the Flags present in the RomParameters.json file
-        for launching the correct part of the ROM workflow
-        """
-        #other options: "trainHROM", "runHROM"
-        parameters_file_folder = self.general_rom_manager_parameters["ROM"]["rom_basis_output_folder"].GetString() if self.general_rom_manager_parameters["ROM"].Has("rom_basis_output_folder") else "rom_data"
-        parameters_file_name = self.general_rom_manager_parameters["ROM"]["rom_basis_output_name"].GetString() if self.general_rom_manager_parameters["ROM"].Has("rom_basis_output_name") else "RomParameters"
-
-        # Convert to Path objects
-        parameters_file_folder = Path(parameters_file_folder)
-        parameters_file_name = Path(parameters_file_name)
-
-        parameters_file_path = parameters_file_folder / parameters_file_name.with_suffix('.json')
-
-        with parameters_file_path.open('r+') as parameter_file:
-            f=json.load(parameter_file)
-            f['assembling_strategy'] = self.general_rom_manager_parameters['assembling_strategy'].GetString() if self.general_rom_manager_parameters.Has('assembling_strategy') else 'global'
-            self._AddHromParametersToRomParameters(f)
-            if simulation_to_run=='GalerkinROM':
-                f['projection_strategy']="galerkin"
-                f['train_hrom']=False
-                f['run_hrom']=False
-                f["rom_settings"]['rom_bns_settings'] = self._SetGalerkinBnSParameters()
-            elif simulation_to_run=='trainHROMGalerkin':
-                f['train_hrom']=True
-                f['run_hrom']=False
-                f["rom_settings"]['rom_bns_settings'] = self._SetGalerkinBnSParameters()
-            elif simulation_to_run=='runHROMGalerkin':
-                f['projection_strategy']="galerkin"
-                f['train_hrom']=False
-                f['run_hrom']=True
-                f["rom_settings"]['rom_bns_settings'] = self._SetGalerkinBnSParameters()
-            elif simulation_to_run == 'lspg':
-                f['train_hrom'] = False
-                f['run_hrom'] = False
-                f['projection_strategy'] = "lspg"
-                f["rom_settings"]['rom_bns_settings'] = self._SetLSPGBnSParameters()
-            elif simulation_to_run == 'trainHROMLSPG':
-                f['train_hrom'] = True
-                f['run_hrom'] = False
-                f['projection_strategy'] = "lspg"
-                f["rom_settings"]['rom_bns_settings'] = self._SetLSPGBnSParameters()
-            elif simulation_to_run == 'runHROMLSPG':
-                f['train_hrom'] = False
-                f['run_hrom'] = True
-                f['projection_strategy'] = "lspg"
-                f["rom_settings"]['rom_bns_settings'] = self._SetLSPGBnSParameters()
-            elif simulation_to_run == 'TrainPG':
-                f['train_hrom'] = False
-                f['run_hrom'] = False
-                f['projection_strategy'] = "lspg"
-                f["rom_settings"]['rom_bns_settings'] = self._SetLSPGBnSParameters()
-                f["rom_settings"]['rom_bns_settings']['train_petrov_galerkin'] = True  # Override the default
-            elif simulation_to_run=='PG':
-                f['train_hrom']=False
-                f['run_hrom']=False
-                f['projection_strategy']="petrov_galerkin"
-                f["rom_settings"]['rom_bns_settings'] = self._SetPetrovGalerkinBnSParameters()
-            elif simulation_to_run=='trainHROMPetrovGalerkin':
-                f['train_hrom']=True
-                f['run_hrom']=False
-                f['projection_strategy']="petrov_galerkin"
-                f["rom_settings"]['rom_bns_settings'] = self._SetPetrovGalerkinBnSParameters()
-            elif simulation_to_run=='runHROMPetrovGalerkin':
-                f['train_hrom']=False
-                f['run_hrom']=True
-                f['projection_strategy']="petrov_galerkin"
-                f["rom_settings"]['rom_bns_settings'] = self._SetPetrovGalerkinBnSParameters()
-            else:
-                raise Exception(f'Unknown flag "{simulation_to_run}" change for RomParameters.json')
-            parameter_file.seek(0)
-            json.dump(f,parameter_file,indent=4)
-            parameter_file.truncate()
-
-    def _SetGalerkinBnSParameters(self):
-        # Retrieve the default parameters as a JSON string and parse it into a dictionary
-        defaults_json = self._GetGalerkinBnSParameters()
-        defaults = json.loads(defaults_json)
-
-        # Ensure 'galerkin_rom_bns_settings' exists in ROM parameters
-        if not self.general_rom_manager_parameters["ROM"].Has("galerkin_rom_bns_settings"):
-            self.general_rom_manager_parameters["ROM"].AddEmptyValue("galerkin_rom_bns_settings")
-
-        # Get the ROM parameters for Galerkin
-        rom_params = self.general_rom_manager_parameters["ROM"]["galerkin_rom_bns_settings"]
-
-        # Update defaults with any existing ROM parameters
-        self._UpdateDefaultsWithRomParams(defaults, rom_params)
-
-        return defaults
-
-    def _SetLSPGBnSParameters(self):
-        # Retrieve the default parameters as a JSON string and parse it into a dictionary
-        defaults_json = self._GetLSPGBnSParameters()
-        defaults = json.loads(defaults_json)
-
-        # Ensure 'lspg_rom_bns_settings' exists in ROM parameters
-        if not self.general_rom_manager_parameters["ROM"].Has("lspg_rom_bns_settings"):
-            self.general_rom_manager_parameters["ROM"].AddEmptyValue("lspg_rom_bns_settings")
-
-        # Get the ROM parameters for LSPG
-        rom_params = self.general_rom_manager_parameters["ROM"]["lspg_rom_bns_settings"]
-
-        # Update defaults with any existing ROM parameters
-        self._UpdateDefaultsWithRomParams(defaults, rom_params)
-
-        return defaults
-
-    def _SetPetrovGalerkinBnSParameters(self):
-        # Retrieve the default parameters as a JSON string and parse it into a dictionary
-        defaults_json = self._GetPetrovGalerkinBnSParameters()
-        defaults = json.loads(defaults_json)
-
-        # Ensure 'petrov_galerkin_rom_bns_settings' exists in ROM parameters
-        if not self.general_rom_manager_parameters["ROM"].Has("petrov_galerkin_rom_bns_settings"):
-            self.general_rom_manager_parameters["ROM"].AddEmptyValue("petrov_galerkin_rom_bns_settings")
-
-        # Get the ROM parameters for Petrov-Galerkin
-        rom_params = self.general_rom_manager_parameters["ROM"]["petrov_galerkin_rom_bns_settings"]
-
-        # Update defaults with any existing ROM parameters
-        self._UpdateDefaultsWithRomParams(defaults, rom_params)
-
-        return defaults
-
-    def _UpdateDefaultsWithRomParams(self, defaults, rom_params):
-        for key, default_value in defaults.items():
-            if rom_params.Has(key):
-                if isinstance(default_value, bool):
-                    defaults[key] = rom_params[key].GetBool()
-                elif isinstance(default_value, str):
-                    defaults[key] = rom_params[key].GetString()
-                elif isinstance(default_value, float):
-                    defaults[key] = rom_params[key].GetDouble()
-        return defaults
-
-    def _AddBasisCreationToProjectParameters(self, parameters):
-        #FIXME make sure no other rom_output already existed. If so, erase the prior and keep only the one in self.rom_training_parameters
-        parameters["output_processes"].AddEmptyArray("rom_output")
-        parameters["output_processes"]["rom_output"].Append(self.rom_training_parameters)
-
-        return parameters
-
-
-
-
-    def _StoreResultsByName(self,parameters,results_name,mu, Id):
-
-        if  self.general_rom_manager_parameters["output_name"].GetString() == "mu":
-            case_name = (", ".join(map(str, mu)))
-        elif self.general_rom_manager_parameters["output_name"].GetString() == "id":
-            case_name = str(Id)
-        if self.general_rom_manager_parameters["save_gid_output"].GetBool():
-            parameters["output_processes"]["gid_output"][0]["Parameters"]["output_name"].SetString('Results/'+ results_name +  case_name)
-        else:
-            parameters["output_processes"].RemoveValue("gid_output")
-        if self.general_rom_manager_parameters["save_vtk_output"].GetBool():
-            parameters["output_processes"]["vtk_output"][0]["Parameters"]["output_path"].SetString('Results/vtk_output_'+ results_name + case_name)
-        else:
-            parameters["output_processes"].RemoveValue("vtk_output")
-
-        return parameters
-
-
-    def _StoreNoResults(self, parameters):
-        parameters["output_processes"].RemoveValue("gid_output")
-        parameters["output_processes"].RemoveValue("vtk_output")
-
-        return parameters
-
-
-
-    def _SetRomTrainingParameters(self):
-        defaults = self._GetDefaulRomBasisOutputParameters()
-        defaults["Parameters"]["rom_manager"].SetBool(True)  # Set the flag to true when inside the RomManager to trigger particular behavior for multiple parameters
-
-        rom_params = self.general_rom_manager_parameters["ROM"]
-
-        keys_to_copy = [
-            "svd_truncation_tolerance",
-            "model_part_name",
-            "rom_basis_output_format",
-            "rom_basis_output_name",
-            "rom_basis_output_folder",
-            "nodal_unknowns",
-            "snapshots_interval",
-        ]
-
-        for key in keys_to_copy:
-            if key in rom_params.keys():
-                defaults["Parameters"][key] = rom_params[key]
-
-        return defaults
-
-
-
-
-    def SetHromTrainingParameters(self):
-        defaults = self._GetDefaulHromTrainingParameters()
-        hrom_params = self.general_rom_manager_parameters["HROM"]
-
-        keys_to_copy = [
-            "element_selection_type",
-            "element_selection_svd_truncation_tolerance",
-            "create_hrom_visualization_model_part",
-            "echo_level",
-            "constraint_sum_weights",
-        ]
-
-        for key in keys_to_copy:
-            if key in hrom_params.keys():
-                defaults[key] = hrom_params[key]
-
-        return defaults
-
-
-
-    def _GetAnalysisStageClass(self, parameters):
-
-        analysis_stage_module_name = parameters["analysis_stage"].GetString()
-        analysis_stage_class_name = analysis_stage_module_name.split('.')[-1]
-        analysis_stage_class_name = ''.join(x.title() for x in analysis_stage_class_name.split('_'))
-
-        analysis_stage_module = importlib.import_module(analysis_stage_module_name)
-        analysis_stage_class = getattr(analysis_stage_module, analysis_stage_class_name)
-
-        return analysis_stage_class
-
-
-    def _GetDefaulRomBasisOutputParameters(self):
-        rom_training_parameters = KratosMultiphysics.Parameters("""{
-                "python_module" : "calculate_rom_basis_output_process",
-                "kratos_module" : "KratosMultiphysics.RomApplication",
-                "process_name"  : "CalculateRomBasisOutputProcess",
-                "help"          : "This process should write the Rom basis",
-                "Parameters"    :
-                {
-                    "model_part_name": "",
-                    "rom_manager" : false,      // set to false for manual manipulation of ROM via flags in the RomParameters
-                    "snapshots_control_type": "step",
-                    "snapshots_interval": 1.0,
-                    "nodal_unknowns":  [],
-                    "rom_basis_output_format": "json",
-                    "rom_basis_output_name": "RomParameters",
-                    "rom_basis_output_folder": "rom_data",
-                    "svd_truncation_tolerance": 1e-3
-                }
-            }""")
-        return rom_training_parameters
-
-
-    def _GetDefaulHromTrainingParameters(self):
-        hrom_training_parameters = KratosMultiphysics.Parameters("""{
-                "hrom_format": "numpy",
-                "element_selection_type": "empirical_cubature",
-                "element_selection_svd_truncation_tolerance": 1.0e-6,
-                "echo_level" : 0,
-                "create_hrom_visualization_model_part" : true,
-                "projection_strategy": "galerkin",
-                "include_conditions_model_parts_list": [],
-                "include_elements_model_parts_list": [],
-                "initial_candidate_elements_model_part_list" : [],
-                "initial_candidate_conditions_model_part_list" : [],
-                "include_nodal_neighbouring_elements_model_parts_list":[],
-                "include_minimum_condition": false,
-                "include_condition_parents": false,
-                "constraint_sum_weights": true
-            }""")
-        return hrom_training_parameters
-
-
-    def _StoreSnapshotsMatrix(self, string_numpy_array_name, numpy_array):
-
-        # Define the directory and file path
-        rom_output_folder_name = self.rom_training_parameters["Parameters"]["rom_basis_output_folder"].GetString()
-        directory = Path(rom_output_folder_name) / 'SnapshotsMatrices'
-        file_path = directory / f'{string_numpy_array_name}.npy'
-
-        # Create the directory if it doesn't exist
-        directory.mkdir(parents=True, exist_ok=True)
-
-        #save the array inside the chosen directory
-        np.save(file_path, numpy_array)
-
-
-    def SetUpQuantityOfInterestContainers(self):
-        #TODO implement more options if the QoI is too large to keep in RAM
-        self.QoI_Fit_FOM = []
-        self.QoI_Fit_ROM = []
-        self.QoI_Fit_HROM = []
-        self.QoI_Test_FOM = []
-        self.QoI_Test_ROM = []
-        self.QoI_Test_HROM = []
-        self.QoI_Run_FOM = []
-        self.QoI_Run_ROM = []
-        self.QoI_Run_HROM = []
-
-
-    def _GetGalerkinBnSParameters(self):
-        # Define the default settings in JSON format for Galerkin BnS
-        rom_bns_settings = """{
-            "monotonicity_preserving": false
-        }"""
-        return rom_bns_settings
-
-    def _GetPetrovGalerkinBnSParameters(self):
-        # Define the default settings in JSON format for Petrov-Galerkin BnS
-        rom_bns_settings = """{
-            "monotonicity_preserving": false
-        }"""
-        return rom_bns_settings
-
-    def _GetLSPGBnSParameters(self):
-        # Define the default settings in JSON format
-        # Comments:
-        # - basis_strategy: Options include 'residuals', 'jacobian', 'reactions'
-        # - solving_technique: Options include 'normal_equations', 'qr_decomposition'
-        rom_bns_settings = """{
-            "train_petrov_galerkin": false,
-            "basis_strategy": "residuals",
-            "include_phi": false,
-            "svd_truncation_tolerance": 1e-8,
-            "solving_technique": "normal_equations",
-            "monotonicity_preserving": false
-        }"""
+import KratosMultiphysics
+from KratosMultiphysics.RomApplication.rom_testing_utilities import SetUpSimulationInstance
+from KratosMultiphysics.RomApplication.calculate_rom_basis_output_process import CalculateRomBasisOutputProcess
+from KratosMultiphysics.RomApplication.randomized_singular_value_decomposition import RandomizedSingularValueDecomposition
+import numpy as np
+import importlib
+import json
+from pathlib import Path
+
+
+
+class RomManager(object):
+
+    def __init__(self,project_parameters_name, general_rom_manager_parameters, CustomizeSimulation, UpdateProjectParameters,UpdateMaterialParametersFile):
+        #FIXME:
+        # - Use a method (upcoming) for smothly retrieving solutions. In here we are using the RomBasisOutput process in order to store the solutions
+        # - There is some redundancy between the methods that launch the simulations. Can we create a single method?
+        # - We must use the Hyper-Reduced model part for the HROM simulations. (The one in which we have eliminated the non selected elements and conditions)
+        # - Not yet paralellised with COMPSs
+        self.project_parameters_name = project_parameters_name
+        self.general_rom_manager_parameters = general_rom_manager_parameters
+        self.rom_training_parameters = self._SetRomTrainingParameters()
+        self.hrom_training_parameters = self.SetHromTrainingParameters()
+        self.CustomizeSimulation = CustomizeSimulation
+        self.UpdateProjectParameters = UpdateProjectParameters
+        self.UpdateMaterialParametersFile = UpdateMaterialParametersFile
+        self.SetUpQuantityOfInterestContainers()
+
+
+    def Fit(self, mu_train=[None], store_all_snapshots=False, store_fom_snapshots=False, store_rom_snapshots=False, store_hrom_snapshots=False, store_residuals_projected = False):
+        chosen_projection_strategy = self.general_rom_manager_parameters["projection_strategy"].GetString()
+        training_stages = self.general_rom_manager_parameters["rom_stages_to_train"].GetStringArray()
+        #######################
+        ######  Galerkin ######
+        if chosen_projection_strategy == "galerkin":
+            if any(item == "ROM" for item in training_stages):
+                fom_snapshots = self.__LaunchTrainROM(mu_train)
+                if store_all_snapshots or store_fom_snapshots:
+                    self._StoreSnapshotsMatrix('fom_snapshots', fom_snapshots)
+                self._ChangeRomFlags(simulation_to_run = "GalerkinROM")
+                rom_snapshots = self.__LaunchROM(mu_train)
+                if store_all_snapshots or store_rom_snapshots:
+                    self._StoreSnapshotsMatrix('rom_snapshots', rom_snapshots)
+                self.ROMvsFOM_train = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
+
+            if any(item == "HROM" for item in training_stages):
+                #FIXME there will be an error if we only train HROM, but not ROM
+                self._ChangeRomFlags(simulation_to_run = "trainHROMGalerkin")
+                self.__LaunchTrainHROM(mu_train, store_residuals_projected)
+                self._ChangeRomFlags(simulation_to_run = "runHROMGalerkin")
+                hrom_snapshots = self.__LaunchHROM(mu_train)
+                if store_all_snapshots or store_hrom_snapshots:
+                    self._StoreSnapshotsMatrix('hrom_snapshots', hrom_snapshots)
+                self.ROMvsHROM_train = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
+        #######################
+
+        #######################################
+        ##  Least-Squares Petrov Galerkin   ###
+        elif chosen_projection_strategy == "lspg":
+            if any(item == "ROM" for item in training_stages):
+                fom_snapshots = self.__LaunchTrainROM(mu_train)
+                if store_all_snapshots or store_fom_snapshots:
+                    self._StoreSnapshotsMatrix('fom_snapshots', fom_snapshots)
+                self._ChangeRomFlags(simulation_to_run = "lspg")
+                rom_snapshots = self.__LaunchROM(mu_train)
+                if store_all_snapshots or store_rom_snapshots:
+                    self._StoreSnapshotsMatrix('rom_snapshots', rom_snapshots)
+                self.ROMvsFOM_train = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
+            if any(item == "HROM" for item in training_stages):
+                # Change the flags to train the HROM for LSPG
+                self._ChangeRomFlags(simulation_to_run = "trainHROMLSPG")
+                self.__LaunchTrainHROM(mu_train, store_residuals_projected)
+
+                # Change the flags to run the HROM for LSPG
+                self._ChangeRomFlags(simulation_to_run = "runHROMLSPG")
+                hrom_snapshots = self.__LaunchHROM(mu_train)
+
+                if store_all_snapshots or store_hrom_snapshots:
+                    self._StoreSnapshotsMatrix('hrom_snapshots', hrom_snapshots)
+
+                self.ROMvsHROM_train = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
+                #######################################
+
+        ##########################
+        ###  Petrov Galerkin   ###
+        elif chosen_projection_strategy == "petrov_galerkin":
+            if any(item == "ROM" for item in training_stages):
+                fom_snapshots = self.__LaunchTrainROM(mu_train)
+                if store_all_snapshots or store_fom_snapshots:
+                    self._StoreSnapshotsMatrix('fom_snapshots', fom_snapshots)
+                self._ChangeRomFlags(simulation_to_run = "TrainPG")
+                self.__LaunchTrainPG(mu_train)
+                self._ChangeRomFlags(simulation_to_run = "PG")
+                rom_snapshots = self.__LaunchROM(mu_train)
+                if store_all_snapshots or store_rom_snapshots:
+                    self._StoreSnapshotsMatrix('rom_snapshots', rom_snapshots)
+                self.ROMvsFOM_train = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
+            if any(item == "HROM" for item in training_stages):
+                #FIXME there will be an error if we only train HROM, but not ROM
+                self._ChangeRomFlags(simulation_to_run = "trainHROMPetrovGalerkin")
+                self.__LaunchTrainHROM(mu_train, store_residuals_projected)
+                self._ChangeRomFlags(simulation_to_run = "runHROMPetrovGalerkin")
+                hrom_snapshots = self.__LaunchHROM(mu_train)
+                if store_all_snapshots or store_hrom_snapshots:
+                    self._StoreSnapshotsMatrix('hrom_snapshots', hrom_snapshots)
+                self.ROMvsHROM_train = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
+        ##########################
+        else:
+            err_msg = f'Provided projection strategy {chosen_projection_strategy} is not supported. Available options are \'galerkin\', \'lspg\' and \'petrov_galerkin\'.'
+            raise Exception(err_msg)
+
+
+
+    def Test(self, mu_test=[None]):
+        chosen_projection_strategy = self.general_rom_manager_parameters["projection_strategy"].GetString()
+        testing_stages = self.general_rom_manager_parameters["rom_stages_to_test"].GetStringArray()
+        #######################
+        ######  Galerkin ######
+        if chosen_projection_strategy == "galerkin":
+            if any(item == "ROM" for item in testing_stages):
+                fom_snapshots = self.__LaunchTestFOM(mu_test)
+                self._ChangeRomFlags(simulation_to_run = "GalerkinROM")
+                rom_snapshots = self.__LaunchTestROM(mu_test)
+                self.ROMvsFOM_test = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
+
+            if any(item == "HROM" for item in testing_stages):
+                #FIXME there will be an error if we only test HROM, but not ROM
+                self._ChangeRomFlags(simulation_to_run = "runHROMGalerkin")
+                hrom_snapshots = self.__LaunchTestHROM(mu_test)
+                self.ROMvsHROM_test = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
+
+
+        #######################################
+        ##  Least-Squares Petrov Galerkin   ###
+        elif chosen_projection_strategy == "lspg":
+            if any(item == "ROM" for item in testing_stages):
+                fom_snapshots = self.__LaunchTestFOM(mu_test)
+                self._ChangeRomFlags(simulation_to_run = "lspg")
+                rom_snapshots = self.__LaunchTestROM(mu_test)
+                self.ROMvsFOM_test = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
+            if any(item == "HROM" for item in testing_stages):
+                self._ChangeRomFlags(simulation_to_run = "runHROMLSPG")
+                hrom_snapshots = self.__LaunchTestHROM(mu_test)
+                self.ROMvsHROM_test = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
+        #######################################
+
+
+        ##########################
+        ###  Petrov Galerkin   ###
+        elif chosen_projection_strategy == "petrov_galerkin":
+            if any(item == "ROM" for item in testing_stages):
+                fom_snapshots = self.__LaunchTestFOM(mu_test)
+                self._ChangeRomFlags(simulation_to_run = "PG")
+                rom_snapshots = self.__LaunchTestROM(mu_test)
+                self.ROMvsFOM_test = np.linalg.norm(fom_snapshots - rom_snapshots)/ np.linalg.norm(fom_snapshots)
+            if any(item == "HROM" for item in testing_stages):
+                #FIXME there will be an error if we only train HROM, but not ROM
+                self._ChangeRomFlags(simulation_to_run = "runHROMPetrovGalerkin")
+                hrom_snapshots = self.__LaunchTestHROM(mu_test)
+                self.ROMvsHROM_test = np.linalg.norm(rom_snapshots - hrom_snapshots) / np.linalg.norm(rom_snapshots)
+        ##########################
+        else:
+            err_msg = f'Provided projection strategy {chosen_projection_strategy} is not supported. Available options are \'galerkin\', \'lspg\' and \'petrov_galerkin\'.'
+            raise Exception(err_msg)
+
+
+
+
+    def RunFOM(self, mu_run=[None]):
+        self.__LaunchRunFOM(mu_run)
+
+    def RunROM(self, mu_run=[None]):
+        chosen_projection_strategy = self.general_rom_manager_parameters["projection_strategy"].GetString()
+        #######################
+        ######  Galerkin ######
+        if chosen_projection_strategy == "galerkin":
+            self._ChangeRomFlags(simulation_to_run = "GalerkinROM")
+        #######################################
+        ##  Least-Squares Petrov Galerkin   ###
+        elif chosen_projection_strategy == "lspg":
+            self._ChangeRomFlags(simulation_to_run = "lspg")
+        ##########################
+        ###  Petrov Galerkin   ###
+        elif chosen_projection_strategy == "petrov_galerkin":
+            self._ChangeRomFlags(simulation_to_run = "PG")
+        else:
+            err_msg = f'Provided projection strategy {chosen_projection_strategy} is not supported. Available options are \'galerkin\', \'lspg\' and \'petrov_galerkin\'.'
+            raise Exception(err_msg)
+        self.__LaunchRunROM(mu_run)
+
+    def RunHROM(self, mu_run=[None], use_full_model_part = False):
+        chosen_projection_strategy = self.general_rom_manager_parameters["projection_strategy"].GetString()
+        #######################
+        ######  Galerkin ######
+        if chosen_projection_strategy == "galerkin":
+            self._ChangeRomFlags(simulation_to_run = "runHROMGalerkin")
+        #######################################
+        ##  Least-Squares Petrov Galerkin   ###
+        elif chosen_projection_strategy == "lspg":
+            self._ChangeRomFlags(simulation_to_run = "runHROMLSPG")
+        ##########################
+        ###  Petrov Galerkin   ###
+        elif chosen_projection_strategy == "petrov_galerkin":
+            self._ChangeRomFlags(simulation_to_run = "runHROMPetrovGalerkin")
+        else:
+            err_msg = f'Provided projection strategy {chosen_projection_strategy} is not supported. Available options are \'galerkin\', \'lspg\' and \'petrov_galerkin\'.'
+            raise Exception(err_msg)
+        self.__LaunchRunHROM(mu_run, use_full_model_part)
+
+
+    def PrintErrors(self):
+        chosen_projection_strategy = self.general_rom_manager_parameters["projection_strategy"].GetString()
+        training_stages = self.general_rom_manager_parameters["rom_stages_to_train"].GetStringArray()
+        testing_stages = self.general_rom_manager_parameters["rom_stages_to_test"].GetStringArray()
+        if any(item == "ROM" for item in training_stages):
+            print("approximation error in train set FOM vs ROM: ", self.ROMvsFOM_train)
+        if any(item == "HROM" for item in training_stages):
+            print("approximation error in train set ROM vs HROM: ", self.ROMvsHROM_train)
+        if any(item == "ROM" for item in testing_stages):
+            print("approximation error in test set FOM vs ROM: ", self.ROMvsFOM_test)
+        if any(item == "HROM" for item in testing_stages):
+            print("approximation error in test set ROM vs HROM: ",  self.ROMvsHROM_test)
+
+
+    def __LaunchTrainROM(self, mu_train):
+        """
+        This method should be parallel capable
+        """
+        with open(self.project_parameters_name,'r') as parameter_file:
+            parameters = KratosMultiphysics.Parameters(parameter_file.read())
+        SnapshotsMatrix = []
+        for Id, mu in enumerate(mu_train):
+            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
+            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy) #TODO stop using the RomBasisOutputProcess to store the snapshots. Use instead the upcoming build-in function
+            parameters_copy = self._StoreResultsByName(parameters_copy,'FOM_Fit',mu,Id)
+            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
+            self.UpdateMaterialParametersFile(materials_file_name, mu)
+            model = KratosMultiphysics.Model()
+            analysis_stage_class = self._GetAnalysisStageClass(parameters_copy)
+            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
+            simulation.Run()
+            self.QoI_Fit_FOM.append(simulation.GetFinalData())
+            for process in simulation._GetListOfOutputProcesses():
+                if isinstance(process, CalculateRomBasisOutputProcess):
+                    BasisOutputProcess = process
+            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
+        SnapshotsMatrix = np.block(SnapshotsMatrix)
+        u = BasisOutputProcess._ComputeSVD(SnapshotsMatrix)
+        BasisOutputProcess._PrintRomBasis(u) #Calling the RomOutput Process for creating the RomParameter.json
+
+        return SnapshotsMatrix
+
+
+    def __LaunchROM(self, mu_train):
+        """
+        This method should be parallel capable
+        """
+        with open(self.project_parameters_name,'r') as parameter_file:
+            parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+        SnapshotsMatrix = []
+        for Id, mu in enumerate(mu_train):
+            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
+            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)  #TODO stop using the RomBasisOutputProcess to store the snapshots. Use instead the upcoming build-in function
+            parameters_copy = self._StoreResultsByName(parameters_copy,'ROM_Fit',mu,Id)
+            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
+            self.UpdateMaterialParametersFile(materials_file_name, mu)
+            model = KratosMultiphysics.Model()
+            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
+            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
+            simulation.Run()
+            self.QoI_Fit_ROM.append(simulation.GetFinalData())
+            for process in simulation._GetListOfOutputProcesses():
+                if isinstance(process, CalculateRomBasisOutputProcess):
+                    BasisOutputProcess = process
+            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
+        SnapshotsMatrix = np.block(SnapshotsMatrix)
+
+        return SnapshotsMatrix
+
+
+    def __LaunchTrainPG(self, mu_train):
+        """
+        This method should be parallel capable
+        """
+        with open(self.project_parameters_name,'r') as parameter_file:
+            parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+        PetrovGalerkinTrainMatrix = []
+        for Id, mu in enumerate(mu_train):
+            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
+            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)
+            parameters_copy = self._StoreNoResults(parameters_copy)
+            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
+            self.UpdateMaterialParametersFile(materials_file_name, mu)
+            model = KratosMultiphysics.Model()
+            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
+            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
+            simulation.Run()
+            PetrovGalerkinTrainMatrix.append(simulation.GetPetrovGalerkinTrainUtility()._GetSnapshotsMatrix()) #TODO is the best way of extracting the Projected Residuals calling the HROM residuals utility?
+        simulation.GetPetrovGalerkinTrainUtility().CalculateAndSaveBasis(np.block(PetrovGalerkinTrainMatrix))
+
+
+    def __LaunchTrainHROM(self, mu_train, store_residuals_projected=False):
+        """
+        This method should be parallel capable
+        """
+        with open(self.project_parameters_name,'r') as parameter_file:
+            parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+        RedidualsSnapshotsMatrix = []
+        for mu in mu_train:
+            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
+            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)
+            parameters_copy = self._StoreNoResults(parameters_copy)
+            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
+            self.UpdateMaterialParametersFile(materials_file_name, mu)
+            model = KratosMultiphysics.Model()
+            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
+            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
+            simulation.Run()
+            RedidualsSnapshotsMatrix.append(simulation.GetHROM_utility()._GetResidualsProjectedMatrix()) #TODO is the best way of extracting the Projected Residuals calling the HROM residuals utility?
+        RedidualsSnapshotsMatrix = np.block(RedidualsSnapshotsMatrix)
+        if store_residuals_projected:
+            self._StoreSnapshotsMatrix('residuals_projected',RedidualsSnapshotsMatrix)
+        u,_,_,_ = RandomizedSingularValueDecomposition(COMPUTE_V=False).Calculate(RedidualsSnapshotsMatrix,
+        self.hrom_training_parameters["element_selection_svd_truncation_tolerance"].GetDouble())
+        simulation.GetHROM_utility().hyper_reduction_element_selector.SetUp(u, InitialCandidatesSet = simulation.GetHROM_utility().candidate_ids)
+        simulation.GetHROM_utility().hyper_reduction_element_selector.Run()
+        if not simulation.GetHROM_utility().hyper_reduction_element_selector.success:
+            KratosMultiphysics.Logger.PrintWarning("HRomTrainingUtility", "The Empirical Cubature Method did not converge using the initial set of candidates. Launching again without initial candidates.")
+            #Imposing an initial candidate set can lead to no convergence. Restart without imposing the initial candidate set
+            simulation.GetHROM_utility().hyper_reduction_element_selector.SetUp(u, InitialCandidatesSet = None)
+            simulation.GetHROM_utility().hyper_reduction_element_selector.Run()
+        simulation.GetHROM_utility().AppendHRomWeightsToRomParameters()
+        simulation.GetHROM_utility().CreateHRomModelParts()
+
+
+    def __LaunchHROM(self, mu_train):
+        """
+        This method should be parallel capable
+        """
+        with open(self.project_parameters_name,'r') as parameter_file:
+            parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+        SnapshotsMatrix = []
+        for Id, mu in enumerate(mu_train):
+            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
+            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)
+            parameters_copy = self._StoreResultsByName(parameters_copy,'HROM_Fit',mu,Id)
+            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
+            self.UpdateMaterialParametersFile(materials_file_name, mu)
+            model = KratosMultiphysics.Model()
+            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
+            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
+            simulation.Run()
+            self.QoI_Fit_HROM.append(simulation.GetFinalData())
+            for process in simulation._GetListOfOutputProcesses():
+                if isinstance(process, CalculateRomBasisOutputProcess):
+                    BasisOutputProcess = process
+            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
+        SnapshotsMatrix = np.block(SnapshotsMatrix)
+
+        return SnapshotsMatrix
+
+
+    def __LaunchTestFOM(self, mu_test):
+        """
+        This method should be parallel capable
+        """
+        # FIXME We must include a method to retrive solutions in the nodes and stop using the CalculateRomBasisOutputProcess to stote snapshots
+        with open(self.project_parameters_name,'r') as parameter_file:
+            parameters = KratosMultiphysics.Parameters(parameter_file.read())
+        SnapshotsMatrix = []
+        for Id, mu in enumerate(mu_test):
+            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
+            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy) #TODO stop using the RomBasisOutputProcess to store the snapshots. Use instead the upcoming build-in function
+            parameters_copy = self._StoreResultsByName(parameters_copy,'FOM_Test',mu,Id)
+            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
+            self.UpdateMaterialParametersFile(materials_file_name, mu)
+            model = KratosMultiphysics.Model()
+            analysis_stage_class = self._GetAnalysisStageClass(parameters_copy)
+            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
+            simulation.Run()
+            self.QoI_Test_FOM.append(simulation.GetFinalData())
+            for process in simulation._GetListOfOutputProcesses():
+                if isinstance(process, CalculateRomBasisOutputProcess):
+                    BasisOutputProcess = process
+            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
+        SnapshotsMatrix = np.block(SnapshotsMatrix)
+
+
+        return SnapshotsMatrix
+
+
+    def __LaunchTestROM(self, mu_test):
+        """
+        This method should be parallel capable
+        """
+        with open(self.project_parameters_name,'r') as parameter_file:
+            parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+        SnapshotsMatrix = []
+        for Id, mu in enumerate(mu_test):
+            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
+            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)  #TODO stop using the RomBasisOutputProcess to store the snapshots. Use instead the upcoming build-in function
+            parameters_copy = self._StoreResultsByName(parameters_copy,'ROM_Test',mu,Id)
+            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
+            self.UpdateMaterialParametersFile(materials_file_name, mu)
+            model = KratosMultiphysics.Model()
+            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
+            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
+            simulation.Run()
+            self.QoI_Test_ROM.append(simulation.GetFinalData())
+            for process in simulation._GetListOfOutputProcesses():
+                if isinstance(process, CalculateRomBasisOutputProcess):
+                    BasisOutputProcess = process
+            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
+        SnapshotsMatrix = np.block(SnapshotsMatrix)
+
+        return SnapshotsMatrix
+
+
+
+    def __LaunchTestHROM(self, mu_test):
+        """
+        This method should be parallel capable
+        """
+        with open(self.project_parameters_name,'r') as parameter_file:
+            parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+        SnapshotsMatrix = []
+        for Id, mu in enumerate(mu_test):
+            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
+            parameters_copy = self._AddBasisCreationToProjectParameters(parameters_copy)
+            parameters_copy = self._StoreResultsByName(parameters_copy,'HROM_Test',mu,Id)
+            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
+            self.UpdateMaterialParametersFile(materials_file_name, mu)
+            model = KratosMultiphysics.Model()
+            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
+            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
+            simulation.Run()
+            self.QoI_Test_HROM.append(simulation.GetFinalData())
+            for process in simulation._GetListOfOutputProcesses():
+                if isinstance(process, CalculateRomBasisOutputProcess):
+                    BasisOutputProcess = process
+            SnapshotsMatrix.append(BasisOutputProcess._GetSnapshotsMatrix()) #TODO add a CustomMethod() as a standard method in the Analysis Stage to retrive some solution
+        SnapshotsMatrix = np.block(SnapshotsMatrix)
+
+        return SnapshotsMatrix
+
+
+    def __LaunchRunFOM(self, mu_run):
+        """
+        This method should be parallel capable
+        """
+        with open(self.project_parameters_name,'r') as parameter_file:
+            parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+        for Id, mu in enumerate(mu_run):
+            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
+            parameters_copy = self._StoreResultsByName(parameters_copy,'FOM_Run',mu,Id)
+            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
+            self.UpdateMaterialParametersFile(materials_file_name, mu)
+            model = KratosMultiphysics.Model()
+            analysis_stage_class = self._GetAnalysisStageClass(parameters_copy)
+            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
+            simulation.Run()
+            self.QoI_Run_FOM.append(simulation.GetFinalData())
+
+
+    def __LaunchRunROM(self, mu_run):
+        """
+        This method should be parallel capable
+        """
+        with open(self.project_parameters_name,'r') as parameter_file:
+            parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+        for Id, mu in enumerate(mu_run):
+            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
+            parameters_copy = self._StoreResultsByName(parameters_copy,'ROM_Run',mu,Id)
+            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
+            self.UpdateMaterialParametersFile(materials_file_name, mu)
+            model = KratosMultiphysics.Model()
+            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
+            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
+            simulation.Run()
+            self.QoI_Run_ROM.append(simulation.GetFinalData())
+
+
+    def __LaunchRunHROM(self, mu_run, use_full_model_part):
+        """
+        This method should be parallel capable
+        """
+        with open(self.project_parameters_name,'r') as parameter_file:
+            parameters = KratosMultiphysics.Parameters(parameter_file.read())
+        if not use_full_model_part:
+            model_part_name = parameters["solver_settings"]["model_import_settings"]["input_filename"].GetString()
+            parameters["solver_settings"]["model_import_settings"]["input_filename"].SetString(f"{model_part_name}HROM")
+
+        for Id, mu in enumerate(mu_run):
+            parameters_copy = self.UpdateProjectParameters(parameters.Clone(), mu)
+            parameters_copy = self._StoreResultsByName(parameters_copy,'HROM_Run',mu,Id)
+            materials_file_name = parameters_copy["solver_settings"]["material_import_settings"]["materials_filename"].GetString()
+            self.UpdateMaterialParametersFile(materials_file_name, mu)
+            model = KratosMultiphysics.Model()
+            analysis_stage_class = type(SetUpSimulationInstance(model, parameters_copy))
+            simulation = self.CustomizeSimulation(analysis_stage_class,model,parameters_copy)
+            simulation.Run()
+            self.QoI_Run_HROM.append(simulation.GetFinalData())
+
+
+    def _AddHromParametersToRomParameters(self,f):
+        f["hrom_settings"]["element_selection_type"] = self.hrom_training_parameters["element_selection_type"].GetString()
+        f["hrom_settings"]["element_selection_svd_truncation_tolerance"] = self.hrom_training_parameters["element_selection_svd_truncation_tolerance"].GetDouble()
+        f["hrom_settings"]["create_hrom_visualization_model_part"] = self.hrom_training_parameters["create_hrom_visualization_model_part"].GetBool()
+        f["hrom_settings"]["echo_level"] = self.hrom_training_parameters["echo_level"].GetInt()
+        f["hrom_settings"]["include_condition_parents"] = self.hrom_training_parameters["include_condition_parents"].GetBool()
+        f["hrom_settings"]["initial_candidate_elements_model_part_list"] = self.hrom_training_parameters["initial_candidate_elements_model_part_list"].GetStringArray()
+        f["hrom_settings"]["initial_candidate_conditions_model_part_list"] = self.hrom_training_parameters["initial_candidate_conditions_model_part_list"].GetStringArray()
+        f["hrom_settings"]["constraint_sum_weights"] = self.hrom_training_parameters["constraint_sum_weights"].GetBool()
+
+    def _ChangeRomFlags(self, simulation_to_run = 'ROM'):
+        """
+        This method updates the Flags present in the RomParameters.json file
+        for launching the correct part of the ROM workflow
+        """
+        #other options: "trainHROM", "runHROM"
+        parameters_file_folder = self.general_rom_manager_parameters["ROM"]["rom_basis_output_folder"].GetString() if self.general_rom_manager_parameters["ROM"].Has("rom_basis_output_folder") else "rom_data"
+        parameters_file_name = self.general_rom_manager_parameters["ROM"]["rom_basis_output_name"].GetString() if self.general_rom_manager_parameters["ROM"].Has("rom_basis_output_name") else "RomParameters"
+
+        # Convert to Path objects
+        parameters_file_folder = Path(parameters_file_folder)
+        parameters_file_name = Path(parameters_file_name)
+
+        parameters_file_path = parameters_file_folder / parameters_file_name.with_suffix('.json')
+
+        with parameters_file_path.open('r+') as parameter_file:
+            f=json.load(parameter_file)
+            f['assembling_strategy'] = self.general_rom_manager_parameters['assembling_strategy'].GetString() if self.general_rom_manager_parameters.Has('assembling_strategy') else 'global'
+            self._AddHromParametersToRomParameters(f)
+            if simulation_to_run=='GalerkinROM':
+                f['projection_strategy']="galerkin"
+                f['train_hrom']=False
+                f['run_hrom']=False
+                f["rom_settings"]['rom_bns_settings'] = self._SetGalerkinBnSParameters()
+            elif simulation_to_run=='trainHROMGalerkin':
+                f['train_hrom']=True
+                f['run_hrom']=False
+                f["rom_settings"]['rom_bns_settings'] = self._SetGalerkinBnSParameters()
+            elif simulation_to_run=='runHROMGalerkin':
+                f['projection_strategy']="galerkin"
+                f['train_hrom']=False
+                f['run_hrom']=True
+                f["rom_settings"]['rom_bns_settings'] = self._SetGalerkinBnSParameters()
+            elif simulation_to_run == 'lspg':
+                f['train_hrom'] = False
+                f['run_hrom'] = False
+                f['projection_strategy'] = "lspg"
+                f["rom_settings"]['rom_bns_settings'] = self._SetLSPGBnSParameters()
+            elif simulation_to_run == 'trainHROMLSPG':
+                f['train_hrom'] = True
+                f['run_hrom'] = False
+                f['projection_strategy'] = "lspg"
+                f["rom_settings"]['rom_bns_settings'] = self._SetLSPGBnSParameters()
+            elif simulation_to_run == 'runHROMLSPG':
+                f['train_hrom'] = False
+                f['run_hrom'] = True
+                f['projection_strategy'] = "lspg"
+                f["rom_settings"]['rom_bns_settings'] = self._SetLSPGBnSParameters()
+            elif simulation_to_run == 'TrainPG':
+                f['train_hrom'] = False
+                f['run_hrom'] = False
+                f['projection_strategy'] = "lspg"
+                f["rom_settings"]['rom_bns_settings'] = self._SetLSPGBnSParameters()
+                f["rom_settings"]['rom_bns_settings']['train_petrov_galerkin'] = True  # Override the default
+            elif simulation_to_run=='PG':
+                f['train_hrom']=False
+                f['run_hrom']=False
+                f['projection_strategy']="petrov_galerkin"
+                f["rom_settings"]['rom_bns_settings'] = self._SetPetrovGalerkinBnSParameters()
+            elif simulation_to_run=='trainHROMPetrovGalerkin':
+                f['train_hrom']=True
+                f['run_hrom']=False
+                f['projection_strategy']="petrov_galerkin"
+                f["rom_settings"]['rom_bns_settings'] = self._SetPetrovGalerkinBnSParameters()
+            elif simulation_to_run=='runHROMPetrovGalerkin':
+                f['train_hrom']=False
+                f['run_hrom']=True
+                f['projection_strategy']="petrov_galerkin"
+                f["rom_settings"]['rom_bns_settings'] = self._SetPetrovGalerkinBnSParameters()
+            else:
+                raise Exception(f'Unknown flag "{simulation_to_run}" change for RomParameters.json')
+            parameter_file.seek(0)
+            json.dump(f,parameter_file,indent=4)
+            parameter_file.truncate()
+
+    def _SetGalerkinBnSParameters(self):
+        # Retrieve the default parameters as a JSON string and parse it into a dictionary
+        defaults_json = self._GetGalerkinBnSParameters()
+        defaults = json.loads(defaults_json)
+
+        # Ensure 'galerkin_rom_bns_settings' exists in ROM parameters
+        if not self.general_rom_manager_parameters["ROM"].Has("galerkin_rom_bns_settings"):
+            self.general_rom_manager_parameters["ROM"].AddEmptyValue("galerkin_rom_bns_settings")
+
+        # Get the ROM parameters for Galerkin
+        rom_params = self.general_rom_manager_parameters["ROM"]["galerkin_rom_bns_settings"]
+
+        # Update defaults with any existing ROM parameters
+        self._UpdateDefaultsWithRomParams(defaults, rom_params)
+
+        return defaults
+
+    def _SetLSPGBnSParameters(self):
+        # Retrieve the default parameters as a JSON string and parse it into a dictionary
+        defaults_json = self._GetLSPGBnSParameters()
+        defaults = json.loads(defaults_json)
+
+        # Ensure 'lspg_rom_bns_settings' exists in ROM parameters
+        if not self.general_rom_manager_parameters["ROM"].Has("lspg_rom_bns_settings"):
+            self.general_rom_manager_parameters["ROM"].AddEmptyValue("lspg_rom_bns_settings")
+
+        # Get the ROM parameters for LSPG
+        rom_params = self.general_rom_manager_parameters["ROM"]["lspg_rom_bns_settings"]
+
+        # Update defaults with any existing ROM parameters
+        self._UpdateDefaultsWithRomParams(defaults, rom_params)
+
+        return defaults
+
+    def _SetPetrovGalerkinBnSParameters(self):
+        # Retrieve the default parameters as a JSON string and parse it into a dictionary
+        defaults_json = self._GetPetrovGalerkinBnSParameters()
+        defaults = json.loads(defaults_json)
+
+        # Ensure 'petrov_galerkin_rom_bns_settings' exists in ROM parameters
+        if not self.general_rom_manager_parameters["ROM"].Has("petrov_galerkin_rom_bns_settings"):
+            self.general_rom_manager_parameters["ROM"].AddEmptyValue("petrov_galerkin_rom_bns_settings")
+
+        # Get the ROM parameters for Petrov-Galerkin
+        rom_params = self.general_rom_manager_parameters["ROM"]["petrov_galerkin_rom_bns_settings"]
+
+        # Update defaults with any existing ROM parameters
+        self._UpdateDefaultsWithRomParams(defaults, rom_params)
+
+        return defaults
+
+    def _UpdateDefaultsWithRomParams(self, defaults, rom_params):
+        for key, default_value in defaults.items():
+            if rom_params.Has(key):
+                if isinstance(default_value, bool):
+                    defaults[key] = rom_params[key].GetBool()
+                elif isinstance(default_value, str):
+                    defaults[key] = rom_params[key].GetString()
+                elif isinstance(default_value, float):
+                    defaults[key] = rom_params[key].GetDouble()
+        return defaults
+
+    def _AddBasisCreationToProjectParameters(self, parameters):
+        #FIXME make sure no other rom_output already existed. If so, erase the prior and keep only the one in self.rom_training_parameters
+        parameters["output_processes"].AddEmptyArray("rom_output")
+        parameters["output_processes"]["rom_output"].Append(self.rom_training_parameters)
+
+        return parameters
+
+
+
+
+    def _StoreResultsByName(self,parameters,results_name,mu, Id):
+
+        if  self.general_rom_manager_parameters["output_name"].GetString() == "mu":
+            case_name = (", ".join(map(str, mu)))
+        elif self.general_rom_manager_parameters["output_name"].GetString() == "id":
+            case_name = str(Id)
+        if self.general_rom_manager_parameters["save_gid_output"].GetBool():
+            parameters["output_processes"]["gid_output"][0]["Parameters"]["output_name"].SetString('Results/'+ results_name +  case_name)
+        else:
+            parameters["output_processes"].RemoveValue("gid_output")
+        if self.general_rom_manager_parameters["save_vtk_output"].GetBool():
+            parameters["output_processes"]["vtk_output"][0]["Parameters"]["output_path"].SetString('Results/vtk_output_'+ results_name + case_name)
+        else:
+            parameters["output_processes"].RemoveValue("vtk_output")
+
+        return parameters
+
+
+    def _StoreNoResults(self, parameters):
+        parameters["output_processes"].RemoveValue("gid_output")
+        parameters["output_processes"].RemoveValue("vtk_output")
+
+        return parameters
+
+
+
+    def _SetRomTrainingParameters(self):
+        defaults = self._GetDefaulRomBasisOutputParameters()
+        defaults["Parameters"]["rom_manager"].SetBool(True)  # Set the flag to true when inside the RomManager to trigger particular behavior for multiple parameters
+
+        rom_params = self.general_rom_manager_parameters["ROM"]
+
+        keys_to_copy = [
+            "svd_truncation_tolerance",
+            "model_part_name",
+            "rom_basis_output_format",
+            "rom_basis_output_name",
+            "rom_basis_output_folder",
+            "nodal_unknowns",
+            "snapshots_interval",
+        ]
+
+        for key in keys_to_copy:
+            if key in rom_params.keys():
+                defaults["Parameters"][key] = rom_params[key]
+
+        return defaults
+
+
+
+
+    def SetHromTrainingParameters(self):
+        defaults = self._GetDefaulHromTrainingParameters()
+        hrom_params = self.general_rom_manager_parameters["HROM"]
+
+        keys_to_copy = [
+            "element_selection_type",
+            "element_selection_svd_truncation_tolerance",
+            "create_hrom_visualization_model_part",
+            "echo_level",
+            "constraint_sum_weights",
+        ]
+
+        for key in keys_to_copy:
+            if key in hrom_params.keys():
+                defaults[key] = hrom_params[key]
+
+        return defaults
+
+
+
+    def _GetAnalysisStageClass(self, parameters):
+
+        analysis_stage_module_name = parameters["analysis_stage"].GetString()
+        analysis_stage_class_name = analysis_stage_module_name.split('.')[-1]
+        analysis_stage_class_name = ''.join(x.title() for x in analysis_stage_class_name.split('_'))
+
+        analysis_stage_module = importlib.import_module(analysis_stage_module_name)
+        analysis_stage_class = getattr(analysis_stage_module, analysis_stage_class_name)
+
+        return analysis_stage_class
+
+
+    def _GetDefaulRomBasisOutputParameters(self):
+        rom_training_parameters = KratosMultiphysics.Parameters("""{
+                "python_module" : "calculate_rom_basis_output_process",
+                "kratos_module" : "KratosMultiphysics.RomApplication",
+                "process_name"  : "CalculateRomBasisOutputProcess",
+                "help"          : "This process should write the Rom basis",
+                "Parameters"    :
+                {
+                    "model_part_name": "",
+                    "rom_manager" : false,      // set to false for manual manipulation of ROM via flags in the RomParameters
+                    "snapshots_control_type": "step",
+                    "snapshots_interval": 1.0,
+                    "nodal_unknowns":  [],
+                    "rom_basis_output_format": "json",
+                    "rom_basis_output_name": "RomParameters",
+                    "rom_basis_output_folder": "rom_data",
+                    "svd_truncation_tolerance": 1e-3
+                }
+            }""")
+        return rom_training_parameters
+
+
+    def _GetDefaulHromTrainingParameters(self):
+        hrom_training_parameters = KratosMultiphysics.Parameters("""{
+                "hrom_format": "numpy",
+                "element_selection_type": "empirical_cubature",
+                "element_selection_svd_truncation_tolerance": 1.0e-6,
+                "echo_level" : 0,
+                "create_hrom_visualization_model_part" : true,
+                "projection_strategy": "galerkin",
+                "include_conditions_model_parts_list": [],
+                "include_elements_model_parts_list": [],
+                "initial_candidate_elements_model_part_list" : [],
+                "initial_candidate_conditions_model_part_list" : [],
+                "include_nodal_neighbouring_elements_model_parts_list":[],
+                "include_minimum_condition": false,
+                "include_condition_parents": false,
+                "constraint_sum_weights": true
+            }""")
+        return hrom_training_parameters
+
+
+    def _StoreSnapshotsMatrix(self, string_numpy_array_name, numpy_array):
+
+        # Define the directory and file path
+        rom_output_folder_name = self.rom_training_parameters["Parameters"]["rom_basis_output_folder"].GetString()
+        directory = Path(rom_output_folder_name) / 'SnapshotsMatrices'
+        file_path = directory / f'{string_numpy_array_name}.npy'
+
+        # Create the directory if it doesn't exist
+        directory.mkdir(parents=True, exist_ok=True)
+
+        #save the array inside the chosen directory
+        np.save(file_path, numpy_array)
+
+
+    def SetUpQuantityOfInterestContainers(self):
+        #TODO implement more options if the QoI is too large to keep in RAM
+        self.QoI_Fit_FOM = []
+        self.QoI_Fit_ROM = []
+        self.QoI_Fit_HROM = []
+        self.QoI_Test_FOM = []
+        self.QoI_Test_ROM = []
+        self.QoI_Test_HROM = []
+        self.QoI_Run_FOM = []
+        self.QoI_Run_ROM = []
+        self.QoI_Run_HROM = []
+
+
+    def _GetGalerkinBnSParameters(self):
+        # Define the default settings in JSON format for Galerkin BnS
+        rom_bns_settings = """{
+            "monotonicity_preserving": false
+        }"""
+        return rom_bns_settings
+
+    def _GetPetrovGalerkinBnSParameters(self):
+        # Define the default settings in JSON format for Petrov-Galerkin BnS
+        rom_bns_settings = """{
+            "monotonicity_preserving": false
+        }"""
+        return rom_bns_settings
+
+    def _GetLSPGBnSParameters(self):
+        # Define the default settings in JSON format
+        # Comments:
+        # - basis_strategy: Options include 'residuals', 'jacobian', 'reactions'
+        # - solving_technique: Options include 'normal_equations', 'qr_decomposition'
+        rom_bns_settings = """{
+            "train_petrov_galerkin": false,
+            "basis_strategy": "residuals",
+            "include_phi": false,
+            "svd_truncation_tolerance": 1e-8,
+            "solving_technique": "normal_equations",
+            "monotonicity_preserving": false
+        }"""
         return rom_bns_settings
```

## KratosMultiphysics/RomApplication/rom_solver.py

 * *Ordering differences only*

```diff
@@ -1,99 +1,99 @@
-# Importing the Kratos Library
-from typing import List
-import KratosMultiphysics
-
-# Import applications
-import KratosMultiphysics.RomApplication as KratosROM
-
-def CreateSolver(cls, model, custom_settings):
-    class ROMSolver(cls):
-        """ROM solver generic main class.
-        This class serves as a generic class to make a standard Kratos solver ROM-compatible.
-        It extends the default parameters to include the \'rom_settings\' and overrides the
-        creation of the builder and solver to use the ROM one.
-        """
-
-        def __init__(self, model, custom_settings):
-            super().__init__(model, custom_settings)
-            KratosMultiphysics.Logger.PrintInfo("::[ROMSolver]:: ", "Construction finished")
-
-        @classmethod
-        def GetDefaultParameters(cls):
-            default_settings = KratosMultiphysics.Parameters("""{
-                "projection_strategy" : "galerkin",
-                "assembling_strategy" : "global",
-                "rom_settings": {
-                    "nodal_unknowns": [],
-                    "number_of_rom_dofs": 0,
-                    "rom_bns_settings": {}
-                }
-            }""")
-            default_settings.AddMissingParameters(super().GetDefaultParameters())
-            return default_settings
-
-        def _CreateBuilderAndSolver(self):
-            linear_solver = self._GetLinearSolver()
-            rom_parameters, solving_strategy = self._ValidateAndReturnRomParameters()
-            available_solving_strategies = {
-                "elemental_galerkin": KratosROM.ROMBuilderAndSolver,
-                "global_galerkin": KratosROM.GlobalROMBuilderAndSolver,
-                "lspg": KratosROM.LeastSquaresPetrovGalerkinROMBuilderAndSolver,
-                "elemental_petrov_galerkin": KratosROM.PetrovGalerkinROMBuilderAndSolver,
-                "global_petrov_galerkin": KratosROM.GlobalPetrovGalerkinROMBuilderAndSolver
-            }
-            if solving_strategy in available_solving_strategies:
-                return available_solving_strategies[solving_strategy](linear_solver, rom_parameters)
-            else:
-                err_msg = f"'Solving_strategy': '{solving_strategy}' is not available. Please select one of the following: {list(available_solving_strategies.keys())}."
-                raise ValueError(err_msg)
-
-        def _ValidateAndReturnRomParameters(self):
-            # Check that the number of ROM DOFs has been provided
-            n_rom_dofs = self.settings["rom_settings"]["number_of_rom_dofs"].GetInt()
-            if not n_rom_dofs > 0:
-                err_msg = "\'number_of_rom_dofs\' in \'rom_settings\' is {}. Please set a larger than zero value.".format(n_rom_dofs)
-                raise Exception(err_msg)
-
-            # Check if the nodal unknowns have been provided by the user
-            # If not, take the DOFs list from the base solver
-            nodal_unknowns = self.settings["rom_settings"]["nodal_unknowns"].GetStringArray()
-            if len(nodal_unknowns) == 0:
-                solver_dofs_list = self.GetDofsList()
-                if not len(solver_dofs_list) == 0:
-                    self.settings["rom_settings"]["nodal_unknowns"].SetStringArray(solver_dofs_list)
-                else:
-                    err_msg = "\'nodal_unknowns\' in \'rom_settings\' is not provided and there is a not-valid implementation in base solver."
-                    err_msg += " Please manually set \'nodal_unknowns\' in \'rom_settings\'."
-                    raise Exception(err_msg)
-            projection_strategy = self.settings["projection_strategy"].GetString()
-            assembling_strategy = self.settings["assembling_strategy"].GetString()
-
-            # Check for the 'elemental' assembling strategy in case of 'lspg' projection strategy
-            if projection_strategy == "lspg" and assembling_strategy == "elemental":
-                warn_msg = "Elemental LSPG is not yet available. Using default global assembling strategy instead."
-                KratosMultiphysics.Logger.PrintWarning("::[ROMSolver]:: ", warn_msg)
-
-            # For now, only Galerkin and Petrov-Galerkin projections have the elemental or global approach option
-            if projection_strategy in ("galerkin", "petrov_galerkin"): #TODO: Possibility of doing elemental lspg
-                available_assembling_strategies = {
-                    "global",
-                    "elemental"
-                }
-                if assembling_strategy in available_assembling_strategies:
-                    # Add the assembling strategy prefix to the projection strategy
-                    projection_strategy = f"{assembling_strategy}_{projection_strategy}"
-                else:
-                    err_msg = f"'Assembling_strategy': '{assembling_strategy}' is not available. Please select one of the following: {list(available_assembling_strategies)}."
-                    raise ValueError(err_msg)
-
-            self._AssignMissingInnerRomParameters(projection_strategy)
-
-            # Return the validated ROM parameters
-            return self.settings["rom_settings"], projection_strategy
-
-        def _AssignMissingInnerRomParameters(self, projection_strategy):
-            monotonicity_preserving = self.settings["rom_settings"]["rom_bns_settings"]["monotonicity_preserving"].GetBool() if self.settings["rom_settings"]["rom_bns_settings"].Has("monotonicity_preserving") else False
-            if projection_strategy in ("global_galerkin", "lspg", "global_petrov_galerkin"):
-                self.settings["rom_settings"]["rom_bns_settings"].AddBool("monotonicity_preserving", monotonicity_preserving)
-
+# Importing the Kratos Library
+from typing import List
+import KratosMultiphysics
+
+# Import applications
+import KratosMultiphysics.RomApplication as KratosROM
+
+def CreateSolver(cls, model, custom_settings):
+    class ROMSolver(cls):
+        """ROM solver generic main class.
+        This class serves as a generic class to make a standard Kratos solver ROM-compatible.
+        It extends the default parameters to include the \'rom_settings\' and overrides the
+        creation of the builder and solver to use the ROM one.
+        """
+
+        def __init__(self, model, custom_settings):
+            super().__init__(model, custom_settings)
+            KratosMultiphysics.Logger.PrintInfo("::[ROMSolver]:: ", "Construction finished")
+
+        @classmethod
+        def GetDefaultParameters(cls):
+            default_settings = KratosMultiphysics.Parameters("""{
+                "projection_strategy" : "galerkin",
+                "assembling_strategy" : "global",
+                "rom_settings": {
+                    "nodal_unknowns": [],
+                    "number_of_rom_dofs": 0,
+                    "rom_bns_settings": {}
+                }
+            }""")
+            default_settings.AddMissingParameters(super().GetDefaultParameters())
+            return default_settings
+
+        def _CreateBuilderAndSolver(self):
+            linear_solver = self._GetLinearSolver()
+            rom_parameters, solving_strategy = self._ValidateAndReturnRomParameters()
+            available_solving_strategies = {
+                "elemental_galerkin": KratosROM.ROMBuilderAndSolver,
+                "global_galerkin": KratosROM.GlobalROMBuilderAndSolver,
+                "lspg": KratosROM.LeastSquaresPetrovGalerkinROMBuilderAndSolver,
+                "elemental_petrov_galerkin": KratosROM.PetrovGalerkinROMBuilderAndSolver,
+                "global_petrov_galerkin": KratosROM.GlobalPetrovGalerkinROMBuilderAndSolver
+            }
+            if solving_strategy in available_solving_strategies:
+                return available_solving_strategies[solving_strategy](linear_solver, rom_parameters)
+            else:
+                err_msg = f"'Solving_strategy': '{solving_strategy}' is not available. Please select one of the following: {list(available_solving_strategies.keys())}."
+                raise ValueError(err_msg)
+
+        def _ValidateAndReturnRomParameters(self):
+            # Check that the number of ROM DOFs has been provided
+            n_rom_dofs = self.settings["rom_settings"]["number_of_rom_dofs"].GetInt()
+            if not n_rom_dofs > 0:
+                err_msg = "\'number_of_rom_dofs\' in \'rom_settings\' is {}. Please set a larger than zero value.".format(n_rom_dofs)
+                raise Exception(err_msg)
+
+            # Check if the nodal unknowns have been provided by the user
+            # If not, take the DOFs list from the base solver
+            nodal_unknowns = self.settings["rom_settings"]["nodal_unknowns"].GetStringArray()
+            if len(nodal_unknowns) == 0:
+                solver_dofs_list = self.GetDofsList()
+                if not len(solver_dofs_list) == 0:
+                    self.settings["rom_settings"]["nodal_unknowns"].SetStringArray(solver_dofs_list)
+                else:
+                    err_msg = "\'nodal_unknowns\' in \'rom_settings\' is not provided and there is a not-valid implementation in base solver."
+                    err_msg += " Please manually set \'nodal_unknowns\' in \'rom_settings\'."
+                    raise Exception(err_msg)
+            projection_strategy = self.settings["projection_strategy"].GetString()
+            assembling_strategy = self.settings["assembling_strategy"].GetString()
+
+            # Check for the 'elemental' assembling strategy in case of 'lspg' projection strategy
+            if projection_strategy == "lspg" and assembling_strategy == "elemental":
+                warn_msg = "Elemental LSPG is not yet available. Using default global assembling strategy instead."
+                KratosMultiphysics.Logger.PrintWarning("::[ROMSolver]:: ", warn_msg)
+
+            # For now, only Galerkin and Petrov-Galerkin projections have the elemental or global approach option
+            if projection_strategy in ("galerkin", "petrov_galerkin"): #TODO: Possibility of doing elemental lspg
+                available_assembling_strategies = {
+                    "global",
+                    "elemental"
+                }
+                if assembling_strategy in available_assembling_strategies:
+                    # Add the assembling strategy prefix to the projection strategy
+                    projection_strategy = f"{assembling_strategy}_{projection_strategy}"
+                else:
+                    err_msg = f"'Assembling_strategy': '{assembling_strategy}' is not available. Please select one of the following: {list(available_assembling_strategies)}."
+                    raise ValueError(err_msg)
+
+            self._AssignMissingInnerRomParameters(projection_strategy)
+
+            # Return the validated ROM parameters
+            return self.settings["rom_settings"], projection_strategy
+
+        def _AssignMissingInnerRomParameters(self, projection_strategy):
+            monotonicity_preserving = self.settings["rom_settings"]["rom_bns_settings"]["monotonicity_preserving"].GetBool() if self.settings["rom_settings"]["rom_bns_settings"].Has("monotonicity_preserving") else False
+            if projection_strategy in ("global_galerkin", "lspg", "global_petrov_galerkin"):
+                self.settings["rom_settings"]["rom_bns_settings"].AddBool("monotonicity_preserving", monotonicity_preserving)
+
     return ROMSolver(model, custom_settings)
```

## KratosMultiphysics/RomApplication/rom_testing_utilities.py

 * *Ordering differences only*

```diff
@@ -1,67 +1,67 @@
-import importlib
-
-import KratosMultiphysics
-import KratosMultiphysics.RomApplication.rom_analysis
-
-def SetUpSimulationInstance(model, parameters):
-    """ Creates and returns a ROM simulation instance """
-
-    # Get the parent simulation class
-    analysis_stage_module_name = parameters["analysis_stage"].GetString()
-    analysis_stage_class_name = analysis_stage_module_name.split('.')[-1]
-    analysis_stage_class_name = ''.join(x.title() for x in analysis_stage_class_name.split('_'))
-
-    analysis_stage_module = importlib.import_module(analysis_stage_module_name)
-    analysis_stage_class = getattr(analysis_stage_module, analysis_stage_class_name)
-
-    # Set up simulation
-    model = KratosMultiphysics.Model()
-    instance_factory = KratosMultiphysics.RomApplication.rom_analysis.CreateRomAnalysisInstance
-    simulation = instance_factory(
-        analysis_stage_class,
-        model,
-        parameters)
-
-    return simulation
-
-def GetNodalResults(model_part, variables_list):
-    # Set and return an array containing the values of the variables in the variable list
-    # Note that the array type variables need to be specified componentwise
-    results_array = []
-    for node in model_part.Nodes:
-        for variable in variables_list:
-            results_array.append(node.GetSolutionStepValue(variable))
-
-    return results_array
-
-def GetScalarNodalResults(model_part, variable):
-    # Set and return an array containing the scalar variable values
-    results_array = []
-    for node in model_part.Nodes:
-        results_array.append(node.GetSolutionStepValue(variable))
-
-    return results_array
-
-def GetVectorNodalResults(model_part, variable):
-    # Set and return an array containing the vector variable values
-    # Note that only the meaningful ones (2 in 2D and 3 in 3D) are returned
-    results_array = []
-    dim = model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
-    for node in model_part.Nodes:
-        vector_value = node.GetSolutionStepValue(variable)
-        for d in range(dim):
-            results_array.append(vector_value[d])
-
-    return results_array
-
-def GetNodalAreaVector(model_part):
-    # Calculate the NODAL_AREA and save it in the non-historical database
-    nodal_area_calculator = KratosMultiphysics.CalculateNonHistoricalNodalAreaProcess(model_part)
-    nodal_area_calculator.Execute()
-
-    # Set and return an array containing the NODAL_AREA values
-    nodal_area_array = []
-    for node in model_part.Nodes:
-        nodal_area_array.append(node.GetValue(KratosMultiphysics.NODAL_AREA))
-
+import importlib
+
+import KratosMultiphysics
+import KratosMultiphysics.RomApplication.rom_analysis
+
+def SetUpSimulationInstance(model, parameters):
+    """ Creates and returns a ROM simulation instance """
+
+    # Get the parent simulation class
+    analysis_stage_module_name = parameters["analysis_stage"].GetString()
+    analysis_stage_class_name = analysis_stage_module_name.split('.')[-1]
+    analysis_stage_class_name = ''.join(x.title() for x in analysis_stage_class_name.split('_'))
+
+    analysis_stage_module = importlib.import_module(analysis_stage_module_name)
+    analysis_stage_class = getattr(analysis_stage_module, analysis_stage_class_name)
+
+    # Set up simulation
+    model = KratosMultiphysics.Model()
+    instance_factory = KratosMultiphysics.RomApplication.rom_analysis.CreateRomAnalysisInstance
+    simulation = instance_factory(
+        analysis_stage_class,
+        model,
+        parameters)
+
+    return simulation
+
+def GetNodalResults(model_part, variables_list):
+    # Set and return an array containing the values of the variables in the variable list
+    # Note that the array type variables need to be specified componentwise
+    results_array = []
+    for node in model_part.Nodes:
+        for variable in variables_list:
+            results_array.append(node.GetSolutionStepValue(variable))
+
+    return results_array
+
+def GetScalarNodalResults(model_part, variable):
+    # Set and return an array containing the scalar variable values
+    results_array = []
+    for node in model_part.Nodes:
+        results_array.append(node.GetSolutionStepValue(variable))
+
+    return results_array
+
+def GetVectorNodalResults(model_part, variable):
+    # Set and return an array containing the vector variable values
+    # Note that only the meaningful ones (2 in 2D and 3 in 3D) are returned
+    results_array = []
+    dim = model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
+    for node in model_part.Nodes:
+        vector_value = node.GetSolutionStepValue(variable)
+        for d in range(dim):
+            results_array.append(vector_value[d])
+
+    return results_array
+
+def GetNodalAreaVector(model_part):
+    # Calculate the NODAL_AREA and save it in the non-historical database
+    nodal_area_calculator = KratosMultiphysics.CalculateNonHistoricalNodalAreaProcess(model_part)
+    nodal_area_calculator.Execute()
+
+    # Set and return an array containing the NODAL_AREA values
+    nodal_area_array = []
+    for node in model_part.Nodes:
+        nodal_area_array.append(node.GetValue(KratosMultiphysics.NODAL_AREA))
+
     return nodal_area_array
```

## KratosMultiphysics/RomApplication/tsqr.py

 * *Ordering differences only*

```diff
@@ -1,251 +1,251 @@
-import os
-# os.environ['MKL_NUM_THREADS'] = '1'
-# os.environ['OPENBLAS_NUM_THREADS']='1'
-from mpi4py import MPI
-import numpy as np
-import numpy.linalg
-
-
-def next_power_of_2(n):
-    '''
-    Find the next power of 2 of n
-    '''
-    p = 1
-    if (n and not(n & (n - 1))):
-        return n
-    while (p < n):
-        p <<= 1
-    return p
-
-# Ai and Bi are the local parts of A and B
-# this function implements Ai.T@Bi and gathers it to root
-
-
-def distributed_transpose_mult(Ai, Bi, comm, root):
-
-    AitBi = Ai.T @ Bi  # multiplication of local blocks
-
-    if(comm.rank == root):
-        AtB = np.zeros(AitBi.shape, dtype=np.double)
-    else:
-        AtB = 0
-
-    comm.Reduce([AitBi, MPI.DOUBLE], [AtB, MPI.DOUBLE], op=MPI.SUM, root=0)
-    return AtB
-
-# A -= Q Qt A
-
-def OrthogonalProjector(Ai, Qi, comm):
-    QtA = distributed_transpose_mult(Qi, Ai, comm, 0)
-    QtA = comm.bcast(QtA, 0)
-    Ai -= Qi @ QtA
-
-# apply randomization
-
-def Randomize(Ai, rand_size, comm):
-    omega = 0
-    np.random.seed(0)
-    if(comm.Get_rank() == 0):    
-        omega = np.random.random_sample((Ai.shape[1], rand_size))
-    omega = comm.bcast(omega, 0)
-    return Ai @ omega
-
-def TotalNorm(Ai, comm):
-    norm = np.array([0.0])
-    local_norm2 = np.array([np.linalg.norm(Ai)**2],dtype=np.double)
-    #comm.Allreduce([local_norm2, MPI.DOUBLE], [norm, MPI.DOUBLE], op=MPI.SUM)
-    comm.Allreduce(local_norm2, norm, op=MPI.SUM)
-    norm = np.sqrt(norm[0])
-    return norm
-
-def tsqr(Ai):
-    '''
-    Parallel QR factorization using Lapack
-            Q(m,n) is the Q matrix
-            R(n,n) is the R matrix
-    '''
-
-    # Recover rank and size
-    MPI_COMM = MPI.COMM_WORLD      # Communications macro
-    MPI_RANK = MPI_COMM.Get_rank()  # Who are you? who? who?
-    MPI_SIZE = MPI_COMM.Get_size()  # Total number of processors used (workers)
-    m, n = Ai.shape
-    # Algorithm 1 from Demmel et al (2012)
-    # 1: QR Factorization on Ai to obtain Q1i and Ri
-    Q1i, R = numpy.linalg.qr(Ai)
-    nextPower = next_power_of_2(MPI_SIZE)
-    nlevels = int(np.log2(nextPower))
-    QW = np.eye(n, dtype=np.double)
-    C = np.zeros((2 * n, n), np.double)
-    Q2l = np.zeros((2 * n * nlevels, n), np.double)
-    blevel = 1
-    for ilevel in range(nlevels):
-        # Store R in the upper part of the C matrix
-        C[:n, :] = R
-        # Decide who sends and who recieves, use R as buffer
-        prank = MPI_RANK ^ blevel
-        if MPI_RANK & blevel:
-            if prank < MPI_SIZE:
-                MPI_COMM.send(R, prank, tag=0)
-        else:
-            if prank < MPI_SIZE:
-                R = MPI_COMM.recv(source=prank, tag=0)
-                # Store R in the lower part of the C matrix
-                C[n:, :] = R
-                # 2: QR from the C matrix, reuse C and R
-                Q2i, R = np.linalg.qr(C)
-                # Store Q2i from this level
-                Q2l[2 * n * ilevel:2 * n * ilevel + 2 * n, :] = Q2i
-        blevel <<= 1
-    # At this point R is correct on processor 0
-    # Broadcast R and its part of the Q matrix
-    if MPI_SIZE > 1:    
-        blevel = 1 << (nlevels - 1)
-        mask = blevel - 1
-    for ilevel in reversed(range(nlevels)):
-        if MPI_RANK & mask == 0:
-            # Obtain Q2i for this level - use C as buffer
-            C = Q2l[2 * n * ilevel:2 * n * ilevel + 2 * n, :]
-            # Multiply by QW either set to identity or allocated to a value
-            # Store into Q2i
-            Q2i = C @ QW  # matmul(C, QW)
-            # Communications scheme
-            prank = MPI_RANK ^ blevel
-            if MPI_RANK & blevel:
-                if prank < MPI_SIZE:
-                    C = MPI_COMM.recv(source=prank, tag=0)
-                    # Recover R from the upper part of C and QW from the lower
-                    # part
-                    R = C[:n, :]
-                    QW = C[n:, :]
-            else:
-                if prank < MPI_SIZE:
-                    # Set up C matrix for sending
-                    # Store R in the upper part and Q2i on the lower part
-                    # Store Q2i of this rank to QW
-                    C[:n, :] = R
-                    C[n:, :] = Q2i[n:, :]
-                    QW = Q2i[:n, :]
-                    MPI_COMM.send(C, prank, tag=0)
-        blevel >>= 1
-        mask >>= 1
-    # Multiply Q1i and QW to obtain Qi
-    Qi = Q1i @ QW  # matmul(Q1i, QW)
-    return Qi
-
-
-
-def randomized_orthogonalization(Ai, comm, mu=0, R=0):
-    Mlocal, N = Ai.shape  # C has dimensions M by N
-    
-    #obtain M as the total size
-    mlocal = np.array([Mlocal])
-    mtotal = np.array([0])
-    comm.Allreduce([mlocal, MPI.INT], [mtotal, MPI.INT], op=MPI.SUM)
-    M = mtotal[0]
-    
-    c = nC = TotalNorm(Ai, comm)  # Norm of the initial residual
-
-    if mu == 0:
-        mu = max(M, N) * np.finfo(float).eps * nC / 2  # Machine precision parameter
-    else:
-        mu = nC*mu #it is relative to the initial norm
-
-    dRmax = np.ceil(0.25 * (min(M, N)))
-    dRmin = min(1, min(M, N))
-    dRmin = max(dRmin, np.ceil(0.05 * min(M, N)))
-
-    if(R==0):
-        R = np.ceil(0.005 * (min(M, N)))  # Initial guess for the rank of C
-    dR = int(R)
-    TypeRankEstimate = 1  # Exponential
-    i = 1  # iteration counter
-    nC_old = c
-    R_old = 0
-
-    Q = None
-    B = None
-
-    while nC > mu:
-        Qi = tsqr(Randomize(Ai, dR, comm))
-        if Q is not None:
-            for j in range(4):  # repeat application of projector to avoid numeric cancellation
-                OrthogonalProjector(Qi, Q, comm)  # Qi=qr(Qi - Q @(Q.T @ Qi))
-            Qi = tsqr(Qi)
-        Bi = distributed_transpose_mult(Qi, Ai, comm, 0)
-        Bi = comm.bcast(Bi, 0)  # broadcast Bi to all nodes
-        
-        Ai -= Qi @  Bi 
-        if i == 1:
-            Q = Qi
-            if comm.Get_rank()==0:            
-                B = Bi
-        else:
-            Q = np.c_[Q, Qi]  # da.concatenate([Q,Qi], axis=1)  #how to make this concatenation???
-            if comm.Get_rank()==0:
-                B = np.r_[B, Bi]  # da.concatenate([B,Bi], axis=0)
-        nC = TotalNorm(Ai, comm)
-        if(comm.Get_rank() == 0):
-            print('iter = ', i, ' nC = ', nC, ' dR = ', dR, ' R = ', Q.shape[1])
-        R_new = Q.shape[1]
-        if TypeRankEstimate == 0:
-            Rest = R_old + (R_new - R_old) / (nC - nC_old) * \
-                (mu - nC_old)  # Estimated rank (linear)
-        elif TypeRankEstimate == 1:
-            Rest = R_old + (R_new - R_old) / (np.log(nC) - np.log(nC_old)) * (
-                np.log(mu) - np.log(nC_old))  # Logarithmic Rank Estimation
-        else:
-            Rest = R_old + dRmin
-        dR = np.ceil(Rest - R_new)
-        dR = min(dR, dRmax)
-        dR = max(dR, dRmin)
-        Rest = R_new + dR
-        dR = int(dR)
-        if Rest >= N:
-            print("FULL")
-            Q = 'FULL'
-            B = np.array([])
-            # break
-        i += 1
-        R_old = R
-        nC_old = nC
-        R = Rest
-
-    return Q, B
-
-
-
-def svd_parallel(Q, B, comm, epsilon=0):
-
-    if(comm.rank == 0):
-        # u, s, _ = np.linalg.svd(B, full_matrices=False)
-        M,N=np.shape(B)
-        dimMATRIX = max(M,N)
-        u, s, v = np.linalg.svd(B, full_matrices=False) #U --> M xN, V --> N x N
-        v = v.T
-        tol = dimMATRIX*np.finfo(float).eps*max(s)/2
-        R = np.sum(s > tol)  # Definition of numerical rank
-        if epsilon == 0:
-            K = R
-        else:
-            SingVsq = np.multiply(s,s)
-            SingVsq.sort()
-            normEf2 = np.sqrt(np.cumsum(SingVsq))
-            epsilon = epsilon*normEf2[-1] #relative tolerance
-            T = (sum(normEf2<epsilon))
-            K = len(s)-T
-        K = min(R,K)
-        u = u[:, :K] 
-        s = s[:K] 
-        v = v[:, :K]
-    else:
-        u, s , v = [0,0,0]
-    ub = comm.bcast(u, 0)
-    s = comm.bcast(s, 0)
-    U_final = Q @ ub
-
-    return U_final,s,v
-
-    
-
-    
+import os
+# os.environ['MKL_NUM_THREADS'] = '1'
+# os.environ['OPENBLAS_NUM_THREADS']='1'
+from mpi4py import MPI
+import numpy as np
+import numpy.linalg
+
+
+def next_power_of_2(n):
+    '''
+    Find the next power of 2 of n
+    '''
+    p = 1
+    if (n and not(n & (n - 1))):
+        return n
+    while (p < n):
+        p <<= 1
+    return p
+
+# Ai and Bi are the local parts of A and B
+# this function implements Ai.T@Bi and gathers it to root
+
+
+def distributed_transpose_mult(Ai, Bi, comm, root):
+
+    AitBi = Ai.T @ Bi  # multiplication of local blocks
+
+    if(comm.rank == root):
+        AtB = np.zeros(AitBi.shape, dtype=np.double)
+    else:
+        AtB = 0
+
+    comm.Reduce([AitBi, MPI.DOUBLE], [AtB, MPI.DOUBLE], op=MPI.SUM, root=0)
+    return AtB
+
+# A -= Q Qt A
+
+def OrthogonalProjector(Ai, Qi, comm):
+    QtA = distributed_transpose_mult(Qi, Ai, comm, 0)
+    QtA = comm.bcast(QtA, 0)
+    Ai -= Qi @ QtA
+
+# apply randomization
+
+def Randomize(Ai, rand_size, comm):
+    omega = 0
+    np.random.seed(0)
+    if(comm.Get_rank() == 0):    
+        omega = np.random.random_sample((Ai.shape[1], rand_size))
+    omega = comm.bcast(omega, 0)
+    return Ai @ omega
+
+def TotalNorm(Ai, comm):
+    norm = np.array([0.0])
+    local_norm2 = np.array([np.linalg.norm(Ai)**2],dtype=np.double)
+    #comm.Allreduce([local_norm2, MPI.DOUBLE], [norm, MPI.DOUBLE], op=MPI.SUM)
+    comm.Allreduce(local_norm2, norm, op=MPI.SUM)
+    norm = np.sqrt(norm[0])
+    return norm
+
+def tsqr(Ai):
+    '''
+    Parallel QR factorization using Lapack
+            Q(m,n) is the Q matrix
+            R(n,n) is the R matrix
+    '''
+
+    # Recover rank and size
+    MPI_COMM = MPI.COMM_WORLD      # Communications macro
+    MPI_RANK = MPI_COMM.Get_rank()  # Who are you? who? who?
+    MPI_SIZE = MPI_COMM.Get_size()  # Total number of processors used (workers)
+    m, n = Ai.shape
+    # Algorithm 1 from Demmel et al (2012)
+    # 1: QR Factorization on Ai to obtain Q1i and Ri
+    Q1i, R = numpy.linalg.qr(Ai)
+    nextPower = next_power_of_2(MPI_SIZE)
+    nlevels = int(np.log2(nextPower))
+    QW = np.eye(n, dtype=np.double)
+    C = np.zeros((2 * n, n), np.double)
+    Q2l = np.zeros((2 * n * nlevels, n), np.double)
+    blevel = 1
+    for ilevel in range(nlevels):
+        # Store R in the upper part of the C matrix
+        C[:n, :] = R
+        # Decide who sends and who recieves, use R as buffer
+        prank = MPI_RANK ^ blevel
+        if MPI_RANK & blevel:
+            if prank < MPI_SIZE:
+                MPI_COMM.send(R, prank, tag=0)
+        else:
+            if prank < MPI_SIZE:
+                R = MPI_COMM.recv(source=prank, tag=0)
+                # Store R in the lower part of the C matrix
+                C[n:, :] = R
+                # 2: QR from the C matrix, reuse C and R
+                Q2i, R = np.linalg.qr(C)
+                # Store Q2i from this level
+                Q2l[2 * n * ilevel:2 * n * ilevel + 2 * n, :] = Q2i
+        blevel <<= 1
+    # At this point R is correct on processor 0
+    # Broadcast R and its part of the Q matrix
+    if MPI_SIZE > 1:    
+        blevel = 1 << (nlevels - 1)
+        mask = blevel - 1
+    for ilevel in reversed(range(nlevels)):
+        if MPI_RANK & mask == 0:
+            # Obtain Q2i for this level - use C as buffer
+            C = Q2l[2 * n * ilevel:2 * n * ilevel + 2 * n, :]
+            # Multiply by QW either set to identity or allocated to a value
+            # Store into Q2i
+            Q2i = C @ QW  # matmul(C, QW)
+            # Communications scheme
+            prank = MPI_RANK ^ blevel
+            if MPI_RANK & blevel:
+                if prank < MPI_SIZE:
+                    C = MPI_COMM.recv(source=prank, tag=0)
+                    # Recover R from the upper part of C and QW from the lower
+                    # part
+                    R = C[:n, :]
+                    QW = C[n:, :]
+            else:
+                if prank < MPI_SIZE:
+                    # Set up C matrix for sending
+                    # Store R in the upper part and Q2i on the lower part
+                    # Store Q2i of this rank to QW
+                    C[:n, :] = R
+                    C[n:, :] = Q2i[n:, :]
+                    QW = Q2i[:n, :]
+                    MPI_COMM.send(C, prank, tag=0)
+        blevel >>= 1
+        mask >>= 1
+    # Multiply Q1i and QW to obtain Qi
+    Qi = Q1i @ QW  # matmul(Q1i, QW)
+    return Qi
+
+
+
+def randomized_orthogonalization(Ai, comm, mu=0, R=0):
+    Mlocal, N = Ai.shape  # C has dimensions M by N
+    
+    #obtain M as the total size
+    mlocal = np.array([Mlocal])
+    mtotal = np.array([0])
+    comm.Allreduce([mlocal, MPI.INT], [mtotal, MPI.INT], op=MPI.SUM)
+    M = mtotal[0]
+    
+    c = nC = TotalNorm(Ai, comm)  # Norm of the initial residual
+
+    if mu == 0:
+        mu = max(M, N) * np.finfo(float).eps * nC / 2  # Machine precision parameter
+    else:
+        mu = nC*mu #it is relative to the initial norm
+
+    dRmax = np.ceil(0.25 * (min(M, N)))
+    dRmin = min(1, min(M, N))
+    dRmin = max(dRmin, np.ceil(0.05 * min(M, N)))
+
+    if(R==0):
+        R = np.ceil(0.005 * (min(M, N)))  # Initial guess for the rank of C
+    dR = int(R)
+    TypeRankEstimate = 1  # Exponential
+    i = 1  # iteration counter
+    nC_old = c
+    R_old = 0
+
+    Q = None
+    B = None
+
+    while nC > mu:
+        Qi = tsqr(Randomize(Ai, dR, comm))
+        if Q is not None:
+            for j in range(4):  # repeat application of projector to avoid numeric cancellation
+                OrthogonalProjector(Qi, Q, comm)  # Qi=qr(Qi - Q @(Q.T @ Qi))
+            Qi = tsqr(Qi)
+        Bi = distributed_transpose_mult(Qi, Ai, comm, 0)
+        Bi = comm.bcast(Bi, 0)  # broadcast Bi to all nodes
+        
+        Ai -= Qi @  Bi 
+        if i == 1:
+            Q = Qi
+            if comm.Get_rank()==0:            
+                B = Bi
+        else:
+            Q = np.c_[Q, Qi]  # da.concatenate([Q,Qi], axis=1)  #how to make this concatenation???
+            if comm.Get_rank()==0:
+                B = np.r_[B, Bi]  # da.concatenate([B,Bi], axis=0)
+        nC = TotalNorm(Ai, comm)
+        if(comm.Get_rank() == 0):
+            print('iter = ', i, ' nC = ', nC, ' dR = ', dR, ' R = ', Q.shape[1])
+        R_new = Q.shape[1]
+        if TypeRankEstimate == 0:
+            Rest = R_old + (R_new - R_old) / (nC - nC_old) * \
+                (mu - nC_old)  # Estimated rank (linear)
+        elif TypeRankEstimate == 1:
+            Rest = R_old + (R_new - R_old) / (np.log(nC) - np.log(nC_old)) * (
+                np.log(mu) - np.log(nC_old))  # Logarithmic Rank Estimation
+        else:
+            Rest = R_old + dRmin
+        dR = np.ceil(Rest - R_new)
+        dR = min(dR, dRmax)
+        dR = max(dR, dRmin)
+        Rest = R_new + dR
+        dR = int(dR)
+        if Rest >= N:
+            print("FULL")
+            Q = 'FULL'
+            B = np.array([])
+            # break
+        i += 1
+        R_old = R
+        nC_old = nC
+        R = Rest
+
+    return Q, B
+
+
+
+def svd_parallel(Q, B, comm, epsilon=0):
+
+    if(comm.rank == 0):
+        # u, s, _ = np.linalg.svd(B, full_matrices=False)
+        M,N=np.shape(B)
+        dimMATRIX = max(M,N)
+        u, s, v = np.linalg.svd(B, full_matrices=False) #U --> M xN, V --> N x N
+        v = v.T
+        tol = dimMATRIX*np.finfo(float).eps*max(s)/2
+        R = np.sum(s > tol)  # Definition of numerical rank
+        if epsilon == 0:
+            K = R
+        else:
+            SingVsq = np.multiply(s,s)
+            SingVsq.sort()
+            normEf2 = np.sqrt(np.cumsum(SingVsq))
+            epsilon = epsilon*normEf2[-1] #relative tolerance
+            T = (sum(normEf2<epsilon))
+            K = len(s)-T
+        K = min(R,K)
+        u = u[:, :K] 
+        s = s[:K] 
+        v = v[:, :K]
+    else:
+        u, s , v = [0,0,0]
+    ub = comm.bcast(u, 0)
+    s = comm.bcast(s, 0)
+    U_final = Q @ ub
+
+    return U_final,s,v
+
+    
+
+
```

