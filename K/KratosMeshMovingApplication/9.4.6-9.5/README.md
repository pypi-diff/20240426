# Comparing `tmp/KratosMeshMovingApplication-9.4.6-cp39-cp39-win_amd64.whl.zip` & `tmp/KratosMeshMovingApplication-9.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,539 +1,825 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    935720 (00000000000E4728h)
-  Actual end-cent-dir record offset:        935698 (00000000000E4712h)
-  Expected end-cent-dir record offset:      935698 (00000000000E4712h)
+  Zip archive file size:                   2482818 (000000000025E282h)
+  Actual end-cent-dir record offset:       2482796 (000000000025E26Ch)
+  Expected end-cent-dir record offset:     2482796 (000000000025E26Ch)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 18 entries.
-  The central directory is 1945 (0000000000000799h) bytes long,
+  central directory contains 22 entries.
+  The central directory is 2806 (0000000000000AF6h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 933753 (00000000000E3F79h).
+  is 2479990 (000000000025D776h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosMeshMovingApplication.pyd
+  KratosMeshMovingApplication-9.5.dist-info/
 
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
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         a46ae357
-  compressed size:                                355793 bytes
-  uncompressed size:                              1201152 bytes
-  length of filename:                             56 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:30
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:29 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:29 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             42 characters
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
 
-  KratosMultiphysics/.libs/KratosMeshMovingCore.dll
+  KratosMeshMovingApplication-9.5.dist-info/METADATA
 
-  offset of local header from start of archive:   355879
-                                                  (0000000000056E27h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   100
+                                                  (0000000000000064h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         98e08a86
-  compressed size:                                557761 bytes
-  uncompressed size:                              1745920 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         4db81aa2
+  compressed size:                                827 bytes
+  uncompressed size:                              1933 bytes
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
 
 Central directory entry #3:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosMeshMovingCore.lib
+  KratosMeshMovingApplication-9.5.dist-info/WHEEL
 
-  offset of local header from start of archive:   913719
-                                                  (00000000000DF137h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1035
+                                                  (000000000000040Bh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         92deb148
-  compressed size:                                4170 bytes
-  uncompressed size:                              39344 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         90d34e0d
+  compressed size:                                116 bytes
+  uncompressed size:                              148 bytes
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
 
 Central directory entry #4:
 ---------------------------
 
-  KratosMultiphysics/MeshMovingApplication/__init__.py
+  KratosMeshMovingApplication-9.5.dist-info/top_level.txt
 
-  offset of local header from start of archive:   917968
-                                                  (00000000000E01D0h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1256
+                                                  (00000000000004E8h) bytes
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
-  32-bit CRC value (hex):                         dfb1e375
-  compressed size:                                106 bytes
-  uncompressed size:                              242 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         f32d789f
+  compressed size:                                19 bytes
+  uncompressed size:                              19 bytes
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
 
 Central directory entry #5:
 ---------------------------
 
-  KratosMultiphysics/MeshMovingApplication/ale_fluid_solver.py
+  KratosMeshMovingApplication-9.5.dist-info/RECORD
 
-  offset of local header from start of archive:   918156
-                                                  (00000000000E028Ch) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1388
+                                                  (000000000000056Ch) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         640627b8
-  compressed size:                                2419 bytes
-  uncompressed size:                              10764 bytes
-  length of filename:                             60 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:30
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:29 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:29 UTC
+  32-bit CRC value (hex):                         ad8bef43
+  compressed size:                                988 bytes
+  uncompressed size:                              2154 bytes
+  length of filename:                             48 characters
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
 
-  KratosMultiphysics/MeshMovingApplication/impose_mesh_motion_process.py
+  KratosMeshMovingApplication.libs/
 
-  offset of local header from start of archive:   920665
-                                                  (00000000000E0C59h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   2482
+                                                  (00000000000009B2h) bytes
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
-  32-bit CRC value (hex):                         fba1ee82
-  compressed size:                                1508 bytes
-  uncompressed size:                              6535 bytes
-  length of filename:                             70 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:30
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:29 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:29 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             33 characters
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
 
-  KratosMultiphysics/MeshMovingApplication/mesh_moving_analysis.py
+  KratosMeshMovingApplication.libs/libKratosMeshMovingCore-b2b7db2c.so
 
-  offset of local header from start of archive:   922273
-                                                  (00000000000E12A1h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   2573
+                                                  (0000000000000A0Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         18a431f3
-  compressed size:                                1330 bytes
-  uncompressed size:                              4221 bytes
-  length of filename:                             64 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         07bad2a5
+  compressed size:                                1478240 bytes
+  uncompressed size:                              5864049 bytes
+  length of filename:                             68 characters
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
 
-  KratosMultiphysics/MeshMovingApplication/mesh_solver_base.py
+  KratosMultiphysics/
 
-  offset of local header from start of archive:   923697
-                                                  (00000000000E1831h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1480939
+                                                  (00000000001698EBh) bytes
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
-  32-bit CRC value (hex):                         acd8da23
-  compressed size:                                3171 bytes
-  uncompressed size:                              12534 bytes
-  length of filename:                             60 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
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
 
+  KratosMultiphysics/MeshMovingApplication/
+
+  offset of local header from start of archive:   1481016
+                                                  (0000000000169938h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             41 characters
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
   KratosMultiphysics/MeshMovingApplication/mesh_solver_laplacian.py
 
-  offset of local header from start of archive:   926958
-                                                  (00000000000E24EEh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1481115
+                                                  (000000000016999Bh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         6005c8df
-  compressed size:                                588 bytes
-  uncompressed size:                              1915 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         d22378b1
+  compressed size:                                577 bytes
+  uncompressed size:                              1873 bytes
   length of filename:                             65 characters
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
 
-Central directory entry #10:
+Central directory entry #11:
+---------------------------
+
+  KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_base.py
+
+  offset of local header from start of archive:   1481815
+                                                  (0000000000169C57h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         51e22bf9
+  compressed size:                                1042 bytes
+  uncompressed size:                              3349 bytes
+  length of filename:                             69 characters
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
+Central directory entry #12:
 ---------------------------
 
   KratosMultiphysics/MeshMovingApplication/mesh_solver_structural_similarity.py
 
-  offset of local header from start of archive:   927641
-                                                  (00000000000E2799h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1482984
+                                                  (000000000016A0E8h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         49e5a2e9
-  compressed size:                                469 bytes
-  uncompressed size:                              1719 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         72e45ce4
+  compressed size:                                464 bytes
+  uncompressed size:                              1685 bytes
   length of filename:                             77 characters
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
 
-Central directory entry #11:
+Central directory entry #13:
 ---------------------------
 
   KratosMultiphysics/MeshMovingApplication/python_solvers_wrapper_mesh_motion.py
 
-  offset of local header from start of archive:   928217
-                                                  (00000000000E29D9h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1483583
+                                                  (000000000016A33Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         ba77ec48
-  compressed size:                                718 bytes
-  uncompressed size:                              2628 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         10dd4b3c
+  compressed size:                                710 bytes
+  uncompressed size:                              2566 bytes
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
 
-Central directory entry #12:
+Central directory entry #14:
 ---------------------------
 
-  KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_base.py
+  KratosMultiphysics/MeshMovingApplication/ale_fluid_solver.py
 
-  offset of local header from start of archive:   929043
-                                                  (00000000000E2D13h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1484429
+                                                  (000000000016A68Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         abf7a70c
-  compressed size:                                1054 bytes
-  uncompressed size:                              3426 bytes
-  length of filename:                             69 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         3f8184af
+  compressed size:                                2401 bytes
+  uncompressed size:                              10538 bytes
+  length of filename:                             60 characters
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
+Central directory entry #15:
+---------------------------
+
+  KratosMultiphysics/MeshMovingApplication/mesh_moving_analysis.py
+
+  offset of local header from start of archive:   1486948
+                                                  (000000000016B064h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         c57d3f47
+  compressed size:                                1322 bytes
+  uncompressed size:                              4135 bytes
+  length of filename:                             64 characters
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
+Central directory entry #16:
+---------------------------
+
+  KratosMultiphysics/MeshMovingApplication/mesh_solver_base.py
+
+  offset of local header from start of archive:   1488392
+                                                  (000000000016B608h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         a57877d9
+  compressed size:                                3155 bytes
+  uncompressed size:                              12270 bytes
+  length of filename:                             60 characters
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
 ---------------------------
 
   KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_laplacian.py
 
-  offset of local header from start of archive:   930196
-                                                  (00000000000E3194h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1491665
+                                                  (000000000016C2D1h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         de305b77
-  compressed size:                                616 bytes
-  uncompressed size:                              1760 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         78625be7
+  compressed size:                                605 bytes
+  uncompressed size:                              1714 bytes
   length of filename:                             74 characters
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
 
-Central directory entry #14:
+Central directory entry #18:
 ---------------------------
 
   KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_structural_similarity.py
 
-  offset of local header from start of archive:   930916
-                                                  (00000000000E3464h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1492402
+                                                  (000000000016C5B2h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         9a301650
-  compressed size:                                477 bytes
-  uncompressed size:                              1384 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         60b884c8
+  compressed size:                                468 bytes
+  uncompressed size:                              1349 bytes
   length of filename:                             86 characters
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
 
-Central directory entry #15:
+Central directory entry #19:
 ---------------------------
 
-  KratosMeshMovingApplication-9.4.6.dist-info/METADATA
+  KratosMultiphysics/MeshMovingApplication/impose_mesh_motion_process.py
 
-  offset of local header from start of archive:   931509
-                                                  (00000000000E36B5h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1493014
+                                                  (000000000016C816h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         04059de2
-  compressed size:                                842 bytes
-  uncompressed size:                              1986 bytes
-  length of filename:                             52 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         48183cde
+  compressed size:                                1499 bytes
+  uncompressed size:                              6397 bytes
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
 
-Central directory entry #16:
+Central directory entry #20:
 ---------------------------
 
-  KratosMeshMovingApplication-9.4.6.dist-info/WHEEL
+  KratosMultiphysics/MeshMovingApplication/__init__.py
 
-  offset of local header from start of archive:   932433
-                                                  (00000000000E3A51h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1494641
+                                                  (000000000016CE71h) bytes
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
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         73ff1823
+  compressed size:                                102 bytes
+  uncompressed size:                              236 bytes
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
 
-Central directory entry #17:
+Central directory entry #21:
 ---------------------------
 
-  KratosMeshMovingApplication-9.4.6.dist-info/top_level.txt
+  KratosMultiphysics/.libs/
 
-  offset of local header from start of archive:   932608
-                                                  (00000000000E3B00h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1494853
+                                                  (000000000016CF45h) bytes
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
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         f32d789f
-  compressed size:                                21 bytes
-  uncompressed size:                              19 bytes
-  length of filename:                             57 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:30
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:29 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:29 UTC
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
 
-Central directory entry #18:
+Central directory entry #22:
 ---------------------------
 
-  KratosMeshMovingApplication-9.4.6.dist-info/RECORD
+  KratosMultiphysics/.libs/KratosMeshMovingApplication.cpython-39-x86_64-linux-gnu.so
 
-  offset of local header from start of archive:   932716
-                                                  (00000000000E3B6Ch) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1494936
+                                                  (000000000016CF98h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         2d587d01
-  compressed size:                                957 bytes
-  uncompressed size:                              2094 bytes
-  length of filename:                             50 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:24
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:24 UTC
+  32-bit CRC value (hex):                         ea0d46ac
+  compressed size:                                984913 bytes
+  uncompressed size:                              2682081 bytes
+  length of filename:                             83 characters
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
@@ -1,55 +1,67 @@
-Filename: KratosMultiphysics/.libs/KratosMeshMovingApplication.pyd
+Filename: KratosMeshMovingApplication-9.5.dist-info/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosMeshMovingCore.dll
+Filename: KratosMeshMovingApplication-9.5.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosMeshMovingCore.lib
+Filename: KratosMeshMovingApplication-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics/MeshMovingApplication/__init__.py
+Filename: KratosMeshMovingApplication-9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosMultiphysics/MeshMovingApplication/ale_fluid_solver.py
+Filename: KratosMeshMovingApplication-9.5.dist-info/RECORD
 Comment: 
 
-Filename: KratosMultiphysics/MeshMovingApplication/impose_mesh_motion_process.py
+Filename: KratosMeshMovingApplication.libs/
 Comment: 
 
-Filename: KratosMultiphysics/MeshMovingApplication/mesh_moving_analysis.py
+Filename: KratosMeshMovingApplication.libs/libKratosMeshMovingCore-b2b7db2c.so
 Comment: 
 
-Filename: KratosMultiphysics/MeshMovingApplication/mesh_solver_base.py
+Filename: KratosMultiphysics/
+Comment: 
+
+Filename: KratosMultiphysics/MeshMovingApplication/
 Comment: 
 
 Filename: KratosMultiphysics/MeshMovingApplication/mesh_solver_laplacian.py
 Comment: 
 
+Filename: KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_base.py
+Comment: 
+
 Filename: KratosMultiphysics/MeshMovingApplication/mesh_solver_structural_similarity.py
 Comment: 
 
 Filename: KratosMultiphysics/MeshMovingApplication/python_solvers_wrapper_mesh_motion.py
 Comment: 
 
-Filename: KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_base.py
+Filename: KratosMultiphysics/MeshMovingApplication/ale_fluid_solver.py
+Comment: 
+
+Filename: KratosMultiphysics/MeshMovingApplication/mesh_moving_analysis.py
+Comment: 
+
+Filename: KratosMultiphysics/MeshMovingApplication/mesh_solver_base.py
 Comment: 
 
 Filename: KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_laplacian.py
 Comment: 
 
 Filename: KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_structural_similarity.py
 Comment: 
 
-Filename: KratosMeshMovingApplication-9.4.6.dist-info/METADATA
+Filename: KratosMultiphysics/MeshMovingApplication/impose_mesh_motion_process.py
 Comment: 
 
-Filename: KratosMeshMovingApplication-9.4.6.dist-info/WHEEL
+Filename: KratosMultiphysics/MeshMovingApplication/__init__.py
 Comment: 
 
-Filename: KratosMeshMovingApplication-9.4.6.dist-info/top_level.txt
+Filename: KratosMultiphysics/.libs/
 Comment: 
 
-Filename: KratosMeshMovingApplication-9.4.6.dist-info/RECORD
+Filename: KratosMultiphysics/.libs/KratosMeshMovingApplication.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## KratosMultiphysics/MeshMovingApplication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-from KratosMultiphysics import _ImportApplication
-from KratosMeshMovingApplication import *
-application = KratosMeshMovingApplication()
-application_name = "KratosMeshMovingApplication"
-
-_ImportApplication(application, application_name)
+from KratosMultiphysics import _ImportApplication
+from KratosMeshMovingApplication import *
+application = KratosMeshMovingApplication()
+application_name = "KratosMeshMovingApplication"
+
+_ImportApplication(application, application_name)
```

## KratosMultiphysics/MeshMovingApplication/ale_fluid_solver.py

 * *Ordering differences only*

```diff
@@ -1,226 +1,226 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KM
-
-# Other imports
-from KratosMultiphysics.python_solver import PythonSolver
-import KratosMultiphysics.MeshMovingApplication.python_solvers_wrapper_mesh_motion as mesh_mothion_solvers_wrapper
-
-class AleFluidSolver(PythonSolver):
-    def __init__(self, model, solver_settings, parallelism):
-
-        self._validate_settings_in_baseclass=True # To be removed eventually
-        super().__init__(model, solver_settings)
-
-        self.start_fluid_solution_time = self.settings["start_fluid_solution_time"].GetDouble()
-
-        self.parallelism = parallelism
-
-        fluid_solver_settings       = self.settings["fluid_solver_settings"]
-        mesh_motion_solver_settings = self.settings["mesh_motion_solver_settings"]
-
-        fluid_model_part_name = fluid_solver_settings["model_part_name"].GetString()
-        if not self.model.HasModelPart(fluid_model_part_name):
-            model.CreateModelPart(fluid_model_part_name)
-
-        # Derived class decides if the reactions should be computed or not
-        self._ManipulateFluidSolverSettingsForReactionsComputation(fluid_solver_settings)
-
-        # Creating the fluid solver
-        self.fluid_solver = self._CreateFluidSolver(fluid_solver_settings, parallelism)
-
-        # Creating the mesh-motion solver
-        if not mesh_motion_solver_settings.Has("echo_level"):
-            mesh_motion_solver_settings.AddValue("echo_level", self.settings["echo_level"])
-
-        # Making sure the settings are consistent btw fluid and mesh-motion
-        if mesh_motion_solver_settings.Has("model_part_name"):
-            if not fluid_model_part_name == mesh_motion_solver_settings["model_part_name"].GetString():
-                err_msg =  'Fluid- and Mesh-Solver have to use the same MainModelPart ("model_part_name")!\n'
-                err_msg += 'Use "mesh_motion_parts" for specifying mesh-motion on sub-model-parts'
-                raise Exception(err_msg)
-        else:
-            mesh_motion_solver_settings.AddValue("model_part_name", fluid_solver_settings["model_part_name"])
-
-        domain_size = fluid_solver_settings["domain_size"].GetInt()
-        if mesh_motion_solver_settings.Has("domain_size"):
-            mesh_motion_domain_size = mesh_motion_solver_settings["domain_size"].GetInt()
-            if not domain_size == mesh_motion_domain_size:
-                raise Exception('Fluid- and Mesh-Solver have to use the same "domain_size"!')
-        else:
-            mesh_motion_solver_settings.AddValue("domain_size", fluid_solver_settings["domain_size"])
-
-        # Derived class decides if the mesh velocities should be computed or not
-        self._ManipulateMeshMotionSolverSettingsForMeshVelocityComputation(fluid_solver_settings, mesh_motion_solver_settings)
-
-        # Constructing the mesh-solver with the entire mesh
-        # if no submodelparts are specified then this is used for the computation of the mesh-motion
-        # otherwise it only adds the dofs and the variables (to the entire ModelPart!)
-        self.mesh_motion_solver_full_mesh = mesh_mothion_solvers_wrapper.CreateSolverByParameters(
-            model, mesh_motion_solver_settings, parallelism)
-
-        # Getting the min_buffer_size from both solvers
-        # and assigning it to the fluid_solver, bcs this one handles the model_part
-        self.fluid_solver.min_buffer_size = max(
-            self.fluid_solver.GetMinimumBufferSize(),
-            self.mesh_motion_solver_full_mesh.GetMinimumBufferSize())
-
-        KM.Logger.PrintInfo("::[AleFluidSolver]::", "Construction finished")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        this_defaults = KM.Parameters("""{
-            "solver_type"                 : "ale_fluid",
-            "start_fluid_solution_time"   : 0.0,
-            "ale_boundary_parts"          : [ ],
-            "mesh_motion_parts"           : [ ],
-            "fluid_solver_settings"       : { },
-            "mesh_motion_solver_settings" : { }
-        }""")
-        this_defaults.AddMissingParameters(super().GetDefaultParameters())
-        return this_defaults
-
-    def AddVariables(self):
-        self.mesh_motion_solver_full_mesh.AddVariables()
-        self.fluid_solver.AddVariables()
-
-        KM.Logger.PrintInfo("::[AleFluidSolver]::", "Variables Added")
-
-    def AddDofs(self):
-        self.mesh_motion_solver_full_mesh.AddDofs()
-        self.fluid_solver.AddDofs()
-        KM.Logger.PrintInfo("::[AleFluidSolver]::", "DOFs Added")
-
-    def Initialize(self):
-        # Saving the ALE-interface-parts for later
-        # this can only be done AFTER reading the ModelPart
-        main_model_part_name = self.settings["fluid_solver_settings"]["model_part_name"].GetString()
-
-        ale_boundary_parts_params = self.settings["ale_boundary_parts"]
-        self.ale_boundary_parts = []
-        for i_name in range(ale_boundary_parts_params.size()):
-            sub_model_part_name = ale_boundary_parts_params[i_name].GetString()
-            full_model_part_name = main_model_part_name + "." + sub_model_part_name
-            self.ale_boundary_parts.append(self.model[full_model_part_name])
-
-        mesh_motion_parts_params = self.settings["mesh_motion_parts"]
-        self.mesh_motion_solvers = []
-        if mesh_motion_parts_params.size() == 0:
-            # the entire Fluid-ModelPart is used in the Mesh-Solver
-            self.mesh_motion_solvers.append(self.mesh_motion_solver_full_mesh)
-        else:
-            # SubModelParts of the Fluid-ModelPart are used in the Mesh-Solver
-            # each SubModelPart has its own mesh-solver
-            # Note that these solvers do NOT need to call AddVariables and AddDofs
-            # since this is done already for the MainModelPart
-            for i_name in range(mesh_motion_parts_params.size()):
-                sub_model_part_name = mesh_motion_parts_params[i_name].GetString()
-                if sub_model_part_name == main_model_part_name:
-                    err_msg =  'The MainModelPart cannot be used as one of the Sub-Mesh-Solvers!\n'
-                    err_msg += 'Remove "mesh_motion_parts" for specifying mesh-motion on the MainModelPart'
-                    raise Exception(err_msg)
-                full_model_part_name = main_model_part_name + "." + sub_model_part_name
-                sub_mesh_solver_settings = self.settings["mesh_motion_solver_settings"].Clone()
-                sub_mesh_solver_settings["model_part_name"].SetString(full_model_part_name)
-
-                self.mesh_motion_solvers.append(mesh_mothion_solvers_wrapper.CreateSolverByParameters(
-                    self.model, sub_mesh_solver_settings, self.parallelism))
-
-        for mesh_solver in self.mesh_motion_solvers:
-            mesh_solver.Initialize()
-        self.fluid_solver.Initialize()
-
-        KM.Logger.PrintInfo("::[AleFluidSolver]::", "Finished initialization")
-
-    def ImportModelPart(self):
-        self.fluid_solver.ImportModelPart() # only ONE mesh_solver imports the ModelPart
-
-    def PrepareModelPart(self):
-        # Doing it ONLY for the fluid solver (since this contains filling the buffer)
-        self.fluid_solver.PrepareModelPart()
-
-    def AdvanceInTime(self, current_time):
-        # Doing it ONLY for the fluid solver
-        return self.fluid_solver.AdvanceInTime(current_time)
-
-    def Finalize(self):
-        for mesh_solver in self.mesh_motion_solvers:
-            mesh_solver.Finalize()
-        self.fluid_solver.Finalize()
-
-    def InitializeSolutionStep(self):
-        for mesh_solver in self.mesh_motion_solvers:
-            mesh_solver.InitializeSolutionStep()
-        self.fluid_solver.InitializeSolutionStep()
-
-    def Predict(self):
-        for mesh_solver in self.mesh_motion_solvers:
-            mesh_solver.Predict()
-        self.fluid_solver.Predict()
-
-    def FinalizeSolutionStep(self):
-        for mesh_solver in self.mesh_motion_solvers:
-            mesh_solver.FinalizeSolutionStep()
-        self.fluid_solver.FinalizeSolutionStep()
-
-    def SolveSolutionStep(self):
-        is_converged = True
-        for mesh_solver in self.mesh_motion_solvers:
-            is_converged &= mesh_solver.SolveSolutionStep()
-
-        if self.fluid_solver.GetComputingModelPart().ProcessInfo[KM.TIME] >= self.start_fluid_solution_time:
-            self.__ApplyALEBoundaryCondition()
-            is_converged &= self.fluid_solver.SolveSolutionStep()
-
-        return is_converged
-
-    def Check(self):
-        for mesh_solver in self.mesh_motion_solvers:
-            mesh_solver.Check()
-        self.fluid_solver.Check()
-
-    def Clear(self):
-        for mesh_solver in self.mesh_motion_solvers:
-            mesh_solver.Clear()
-        self.fluid_solver.Clear()
-
-    def GetComputingModelPart(self):
-        return self.fluid_solver.GetComputingModelPart() # this is the same as the one used in the MeshSolver
-
-    def GetFluidSolver(self):
-        return self.fluid_solver
-
-    def GetMeshMotionSolver(self):
-        if len(self.mesh_motion_solvers) > 1:
-            raise Exception('More than one mesh-motion-solver exists, please use "GetMeshMotionSolvers"')
-        return self.mesh_motion_solvers[0]
-
-    def GetMeshMotionSolvers(self):
-        return self.mesh_motion_solvers
-
-    def MoveMesh(self):
-        for mesh_solver in self.mesh_motion_solvers:
-            mesh_solver.MoveMesh()
-
-    def _CreateFluidSolver(self, solver_settings, parallelism):
-        '''This function creates the fluid solver.
-        It has to be overridden in derived classes
-        '''
-        raise NotImplementedError("Fluid solver creation must be implemented in the derived class.")
-
-    def __ApplyALEBoundaryCondition(self):
-        '''Copy the MESH_VELOCITY to the VELOCITY (ALE) on the ale-boundary
-        '''
-        for mp in self.ale_boundary_parts:
-            KM.VariableUtils().CopyVectorVar(
-                KM.MESH_VELOCITY,
-                KM.VELOCITY,
-                mp.GetCommunicator().LocalMesh().Nodes)
-            mp.GetCommunicator().SynchronizeVariable(KM.VELOCITY)
-
-    @classmethod
-    def _ManipulateFluidSolverSettingsForReactionsComputation(cls, fluid_solver_settings):
-        raise NotImplementedError('"_ManipulateFluidSolverSettingsForReactionsComputation" has to be implemented in the derived class!')
-
-    @classmethod
-    def _ManipulateMeshMotionSolverSettingsForMeshVelocityComputation(cls, fluid_solver_settings, mesh_motion_solver_settings):
-        raise NotImplementedError('"_ManipulateMeshMotionSolverSettingsForMeshVelocityComputation" has to be implemented in the derived class!')
+# Importing the Kratos Library
+import KratosMultiphysics as KM
+
+# Other imports
+from KratosMultiphysics.python_solver import PythonSolver
+import KratosMultiphysics.MeshMovingApplication.python_solvers_wrapper_mesh_motion as mesh_mothion_solvers_wrapper
+
+class AleFluidSolver(PythonSolver):
+    def __init__(self, model, solver_settings, parallelism):
+
+        self._validate_settings_in_baseclass=True # To be removed eventually
+        super().__init__(model, solver_settings)
+
+        self.start_fluid_solution_time = self.settings["start_fluid_solution_time"].GetDouble()
+
+        self.parallelism = parallelism
+
+        fluid_solver_settings       = self.settings["fluid_solver_settings"]
+        mesh_motion_solver_settings = self.settings["mesh_motion_solver_settings"]
+
+        fluid_model_part_name = fluid_solver_settings["model_part_name"].GetString()
+        if not self.model.HasModelPart(fluid_model_part_name):
+            model.CreateModelPart(fluid_model_part_name)
+
+        # Derived class decides if the reactions should be computed or not
+        self._ManipulateFluidSolverSettingsForReactionsComputation(fluid_solver_settings)
+
+        # Creating the fluid solver
+        self.fluid_solver = self._CreateFluidSolver(fluid_solver_settings, parallelism)
+
+        # Creating the mesh-motion solver
+        if not mesh_motion_solver_settings.Has("echo_level"):
+            mesh_motion_solver_settings.AddValue("echo_level", self.settings["echo_level"])
+
+        # Making sure the settings are consistent btw fluid and mesh-motion
+        if mesh_motion_solver_settings.Has("model_part_name"):
+            if not fluid_model_part_name == mesh_motion_solver_settings["model_part_name"].GetString():
+                err_msg =  'Fluid- and Mesh-Solver have to use the same MainModelPart ("model_part_name")!\n'
+                err_msg += 'Use "mesh_motion_parts" for specifying mesh-motion on sub-model-parts'
+                raise Exception(err_msg)
+        else:
+            mesh_motion_solver_settings.AddValue("model_part_name", fluid_solver_settings["model_part_name"])
+
+        domain_size = fluid_solver_settings["domain_size"].GetInt()
+        if mesh_motion_solver_settings.Has("domain_size"):
+            mesh_motion_domain_size = mesh_motion_solver_settings["domain_size"].GetInt()
+            if not domain_size == mesh_motion_domain_size:
+                raise Exception('Fluid- and Mesh-Solver have to use the same "domain_size"!')
+        else:
+            mesh_motion_solver_settings.AddValue("domain_size", fluid_solver_settings["domain_size"])
+
+        # Derived class decides if the mesh velocities should be computed or not
+        self._ManipulateMeshMotionSolverSettingsForMeshVelocityComputation(fluid_solver_settings, mesh_motion_solver_settings)
+
+        # Constructing the mesh-solver with the entire mesh
+        # if no submodelparts are specified then this is used for the computation of the mesh-motion
+        # otherwise it only adds the dofs and the variables (to the entire ModelPart!)
+        self.mesh_motion_solver_full_mesh = mesh_mothion_solvers_wrapper.CreateSolverByParameters(
+            model, mesh_motion_solver_settings, parallelism)
+
+        # Getting the min_buffer_size from both solvers
+        # and assigning it to the fluid_solver, bcs this one handles the model_part
+        self.fluid_solver.min_buffer_size = max(
+            self.fluid_solver.GetMinimumBufferSize(),
+            self.mesh_motion_solver_full_mesh.GetMinimumBufferSize())
+
+        KM.Logger.PrintInfo("::[AleFluidSolver]::", "Construction finished")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        this_defaults = KM.Parameters("""{
+            "solver_type"                 : "ale_fluid",
+            "start_fluid_solution_time"   : 0.0,
+            "ale_boundary_parts"          : [ ],
+            "mesh_motion_parts"           : [ ],
+            "fluid_solver_settings"       : { },
+            "mesh_motion_solver_settings" : { }
+        }""")
+        this_defaults.AddMissingParameters(super().GetDefaultParameters())
+        return this_defaults
+
+    def AddVariables(self):
+        self.mesh_motion_solver_full_mesh.AddVariables()
+        self.fluid_solver.AddVariables()
+
+        KM.Logger.PrintInfo("::[AleFluidSolver]::", "Variables Added")
+
+    def AddDofs(self):
+        self.mesh_motion_solver_full_mesh.AddDofs()
+        self.fluid_solver.AddDofs()
+        KM.Logger.PrintInfo("::[AleFluidSolver]::", "DOFs Added")
+
+    def Initialize(self):
+        # Saving the ALE-interface-parts for later
+        # this can only be done AFTER reading the ModelPart
+        main_model_part_name = self.settings["fluid_solver_settings"]["model_part_name"].GetString()
+
+        ale_boundary_parts_params = self.settings["ale_boundary_parts"]
+        self.ale_boundary_parts = []
+        for i_name in range(ale_boundary_parts_params.size()):
+            sub_model_part_name = ale_boundary_parts_params[i_name].GetString()
+            full_model_part_name = main_model_part_name + "." + sub_model_part_name
+            self.ale_boundary_parts.append(self.model[full_model_part_name])
+
+        mesh_motion_parts_params = self.settings["mesh_motion_parts"]
+        self.mesh_motion_solvers = []
+        if mesh_motion_parts_params.size() == 0:
+            # the entire Fluid-ModelPart is used in the Mesh-Solver
+            self.mesh_motion_solvers.append(self.mesh_motion_solver_full_mesh)
+        else:
+            # SubModelParts of the Fluid-ModelPart are used in the Mesh-Solver
+            # each SubModelPart has its own mesh-solver
+            # Note that these solvers do NOT need to call AddVariables and AddDofs
+            # since this is done already for the MainModelPart
+            for i_name in range(mesh_motion_parts_params.size()):
+                sub_model_part_name = mesh_motion_parts_params[i_name].GetString()
+                if sub_model_part_name == main_model_part_name:
+                    err_msg =  'The MainModelPart cannot be used as one of the Sub-Mesh-Solvers!\n'
+                    err_msg += 'Remove "mesh_motion_parts" for specifying mesh-motion on the MainModelPart'
+                    raise Exception(err_msg)
+                full_model_part_name = main_model_part_name + "." + sub_model_part_name
+                sub_mesh_solver_settings = self.settings["mesh_motion_solver_settings"].Clone()
+                sub_mesh_solver_settings["model_part_name"].SetString(full_model_part_name)
+
+                self.mesh_motion_solvers.append(mesh_mothion_solvers_wrapper.CreateSolverByParameters(
+                    self.model, sub_mesh_solver_settings, self.parallelism))
+
+        for mesh_solver in self.mesh_motion_solvers:
+            mesh_solver.Initialize()
+        self.fluid_solver.Initialize()
+
+        KM.Logger.PrintInfo("::[AleFluidSolver]::", "Finished initialization")
+
+    def ImportModelPart(self):
+        self.fluid_solver.ImportModelPart() # only ONE mesh_solver imports the ModelPart
+
+    def PrepareModelPart(self):
+        # Doing it ONLY for the fluid solver (since this contains filling the buffer)
+        self.fluid_solver.PrepareModelPart()
+
+    def AdvanceInTime(self, current_time):
+        # Doing it ONLY for the fluid solver
+        return self.fluid_solver.AdvanceInTime(current_time)
+
+    def Finalize(self):
+        for mesh_solver in self.mesh_motion_solvers:
+            mesh_solver.Finalize()
+        self.fluid_solver.Finalize()
+
+    def InitializeSolutionStep(self):
+        for mesh_solver in self.mesh_motion_solvers:
+            mesh_solver.InitializeSolutionStep()
+        self.fluid_solver.InitializeSolutionStep()
+
+    def Predict(self):
+        for mesh_solver in self.mesh_motion_solvers:
+            mesh_solver.Predict()
+        self.fluid_solver.Predict()
+
+    def FinalizeSolutionStep(self):
+        for mesh_solver in self.mesh_motion_solvers:
+            mesh_solver.FinalizeSolutionStep()
+        self.fluid_solver.FinalizeSolutionStep()
+
+    def SolveSolutionStep(self):
+        is_converged = True
+        for mesh_solver in self.mesh_motion_solvers:
+            is_converged &= mesh_solver.SolveSolutionStep()
+
+        if self.fluid_solver.GetComputingModelPart().ProcessInfo[KM.TIME] >= self.start_fluid_solution_time:
+            self.__ApplyALEBoundaryCondition()
+            is_converged &= self.fluid_solver.SolveSolutionStep()
+
+        return is_converged
+
+    def Check(self):
+        for mesh_solver in self.mesh_motion_solvers:
+            mesh_solver.Check()
+        self.fluid_solver.Check()
+
+    def Clear(self):
+        for mesh_solver in self.mesh_motion_solvers:
+            mesh_solver.Clear()
+        self.fluid_solver.Clear()
+
+    def GetComputingModelPart(self):
+        return self.fluid_solver.GetComputingModelPart() # this is the same as the one used in the MeshSolver
+
+    def GetFluidSolver(self):
+        return self.fluid_solver
+
+    def GetMeshMotionSolver(self):
+        if len(self.mesh_motion_solvers) > 1:
+            raise Exception('More than one mesh-motion-solver exists, please use "GetMeshMotionSolvers"')
+        return self.mesh_motion_solvers[0]
+
+    def GetMeshMotionSolvers(self):
+        return self.mesh_motion_solvers
+
+    def MoveMesh(self):
+        for mesh_solver in self.mesh_motion_solvers:
+            mesh_solver.MoveMesh()
+
+    def _CreateFluidSolver(self, solver_settings, parallelism):
+        '''This function creates the fluid solver.
+        It has to be overridden in derived classes
+        '''
+        raise NotImplementedError("Fluid solver creation must be implemented in the derived class.")
+
+    def __ApplyALEBoundaryCondition(self):
+        '''Copy the MESH_VELOCITY to the VELOCITY (ALE) on the ale-boundary
+        '''
+        for mp in self.ale_boundary_parts:
+            KM.VariableUtils().CopyVectorVar(
+                KM.MESH_VELOCITY,
+                KM.VELOCITY,
+                mp.GetCommunicator().LocalMesh().Nodes)
+            mp.GetCommunicator().SynchronizeVariable(KM.VELOCITY)
+
+    @classmethod
+    def _ManipulateFluidSolverSettingsForReactionsComputation(cls, fluid_solver_settings):
+        raise NotImplementedError('"_ManipulateFluidSolverSettingsForReactionsComputation" has to be implemented in the derived class!')
+
+    @classmethod
+    def _ManipulateMeshMotionSolverSettingsForMeshVelocityComputation(cls, fluid_solver_settings, mesh_motion_solver_settings):
+        raise NotImplementedError('"_ManipulateMeshMotionSolverSettingsForMeshVelocityComputation" has to be implemented in the derived class!')
```

## KratosMultiphysics/MeshMovingApplication/impose_mesh_motion_process.py

 * *Ordering differences only*

```diff
@@ -1,139 +1,139 @@
-# --- Core Imports ---
-import KratosMultiphysics
-
-# --- MeshMoving Imports ---
-import KratosMultiphysics.MeshMovingApplication as MeshMovingApplication
-
-
-def Factory(parameters, model):
-    if not isinstance(parameters, KratosMultiphysics.Parameters):
-        raise Exception(
-            'expected input shall be a Parameters object, encapsulating a json string')
-    return ImposeMeshMotionProcess(model, parameters["Parameters"])
-
-
-class ImposeMeshMotionProcess(KratosMultiphysics.Process):
-    """ @brief Impose a rotation followed by translation on a ModelPart.
-
-        @details The transformation is equivalent to:
-                 1) Translation to the reference frame (offset the origin)
-                 2) Specified rotation
-                 3) Reverse translation from the reference frame (undo origin offset)
-                 4) Specified translation
-                 Note: angles in radians
-
-                 The rotation can be defined by either "euler_angles"
-                 or a "rotation_axis" and "rotation_angle" pair. The following parameters can be
-                 defined parametrically (see GenericFunctionUtility):
-                 "euler_angles", "rotation_axis", "reference_point", "rotation_angle", "translation_vector"
-
-                Default parameters:
-                @code
-                {
-                    "model_part_name"       : "",
-                    "interval"              : [0.0, "End"],
-                    "rotation_definition"   : "rotation_axis",
-                    "euler_angles"          : [0.0, 0.0, 0.0],
-                    "rotation_axis"         : [0.0, 0.0, 1.0],
-                    "reference_point"       : [0.0, 0.0, 0.0]
-                    "rotation_angle"        : 0,
-                    "translation_vector"    : [0.0, 0.0, 0.0],
-                }
-                @endcode
-
-        @note the euler angles follow the convention specified by @ref{Quaternion} (Z, -X', Z")
-    """
-
-    def __init__(self,
-                 model: KratosMultiphysics.Model,
-                 parameters: KratosMultiphysics.Parameters):
-        """Impose a rotation followed by translation on a ModelPart."""
-        KratosMultiphysics.Process.__init__(self)
-
-        # 'rotation_angle' can either be a float or "End", but the validator can't handle both
-        # => convert 'rotation_angle' to the input type
-        default_parameters = self.GetDefaultParameters()
-        if parameters.Has("rotation_angle") and parameters["rotation_angle"].IsString():
-            default_parameters.RemoveValue("rotation_angle")
-            default_parameters.AddValue("rotation_angle", parameters["rotation_angle"])
-
-        parameters.ValidateAndAssignDefaults(default_parameters)
-        self.model_part = model[parameters["model_part_name"].GetString()]
-
-        # Parse interval
-        self.interval_utility = KratosMultiphysics.IntervalUtility(parameters)
-
-        # Determine whether a constant transform will suffice or a parametric one is needed
-        requires_parametric_transform = False
-
-        euler_angle_parameters = parameters["euler_angles"]
-        rotation_axis_parameters = parameters["rotation_axis"]
-        rotation_angle_parameters = parameters["rotation_angle"]
-        reference_point_parameters = parameters["reference_point"]
-        translation_vector_parameters = parameters["translation_vector"]
-
-        if rotation_angle_parameters.IsString():
-            requires_parametric_transform = True
-        else:
-            for i in range(3):
-                if euler_angle_parameters[i].IsString() or rotation_axis_parameters[i].IsString() or reference_point_parameters[i].IsString() or translation_vector_parameters[i].IsString():
-                    requires_parametric_transform = True
-                    break
-
-        rotation_definition = parameters["rotation_definition"].GetString()
-
-        if requires_parametric_transform:
-            if rotation_definition == "rotation_axis":
-                self.transform = MeshMovingApplication.ParametricAffineTransform(
-                    rotation_axis_parameters,
-                    rotation_angle_parameters,
-                    reference_point_parameters,
-                    translation_vector_parameters)
-            elif rotation_definition == "euler_angles":
-                self.transform = MeshMovingApplication.ParametricAffineTransform(
-                    euler_angle_parameters,
-                    reference_point_parameters,
-                    translation_vector_parameters)
-            else:
-                raise ValueError("Invalid rotation definition '{}'".format(rotation_definition))
-
-        else:
-            reference_point = reference_point_parameters.GetVector()
-            translation_vector = translation_vector_parameters.GetVector()
-            if rotation_definition == "rotation_axis":
-                rotation_axis = rotation_axis_parameters.GetVector()
-                rotation_angle = rotation_angle_parameters.GetDouble()
-                self.transform = MeshMovingApplication.AffineTransform(
-                    rotation_axis,
-                    rotation_angle,
-                    reference_point,
-                    translation_vector)
-            elif rotation_definition == "euler_angles":
-                euler_angles = euler_angle_parameters.GetVector()
-                self.transform = MeshMovingApplication.AffineTransform(
-                    euler_angles,
-                    reference_point,
-                    translation_vector)
-            else:
-                raise ValueError("Invalid rotation definition '{}'".format(rotation_definition))
-
-
-    def ExecuteInitializeSolutionStep(self):
-        time = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
-
-        if self.interval_utility.IsInInterval(time):
-            MeshMovingApplication.MoveModelPart(self.model_part, self.transform)
-
-
-    @staticmethod
-    def GetDefaultParameters():
-        return KratosMultiphysics.Parameters("""{
-            "model_part_name"       : "",
-            "interval"              : [0.0, "End"],
-            "rotation_definition"   : "rotation_axis",
-            "euler_angles"          : [0.0, 0.0, 0.0],
-            "rotation_axis"         : [0.0, 0.0, 1.0],
-            "reference_point"       : [0.0, 0.0, 0.0],
-            "rotation_angle"        : 0,
-            "translation_vector"    : [0.0, 0.0, 0.0]
+# --- Core Imports ---
+import KratosMultiphysics
+
+# --- MeshMoving Imports ---
+import KratosMultiphysics.MeshMovingApplication as MeshMovingApplication
+
+
+def Factory(parameters, model):
+    if not isinstance(parameters, KratosMultiphysics.Parameters):
+        raise Exception(
+            'expected input shall be a Parameters object, encapsulating a json string')
+    return ImposeMeshMotionProcess(model, parameters["Parameters"])
+
+
+class ImposeMeshMotionProcess(KratosMultiphysics.Process):
+    """ @brief Impose a rotation followed by translation on a ModelPart.
+
+        @details The transformation is equivalent to:
+                 1) Translation to the reference frame (offset the origin)
+                 2) Specified rotation
+                 3) Reverse translation from the reference frame (undo origin offset)
+                 4) Specified translation
+                 Note: angles in radians
+
+                 The rotation can be defined by either "euler_angles"
+                 or a "rotation_axis" and "rotation_angle" pair. The following parameters can be
+                 defined parametrically (see GenericFunctionUtility):
+                 "euler_angles", "rotation_axis", "reference_point", "rotation_angle", "translation_vector"
+
+                Default parameters:
+                @code
+                {
+                    "model_part_name"       : "",
+                    "interval"              : [0.0, "End"],
+                    "rotation_definition"   : "rotation_axis",
+                    "euler_angles"          : [0.0, 0.0, 0.0],
+                    "rotation_axis"         : [0.0, 0.0, 1.0],
+                    "reference_point"       : [0.0, 0.0, 0.0]
+                    "rotation_angle"        : 0,
+                    "translation_vector"    : [0.0, 0.0, 0.0],
+                }
+                @endcode
+
+        @note the euler angles follow the convention specified by @ref{Quaternion} (Z, -X', Z")
+    """
+
+    def __init__(self,
+                 model: KratosMultiphysics.Model,
+                 parameters: KratosMultiphysics.Parameters):
+        """Impose a rotation followed by translation on a ModelPart."""
+        KratosMultiphysics.Process.__init__(self)
+
+        # 'rotation_angle' can either be a float or "End", but the validator can't handle both
+        # => convert 'rotation_angle' to the input type
+        default_parameters = self.GetDefaultParameters()
+        if parameters.Has("rotation_angle") and parameters["rotation_angle"].IsString():
+            default_parameters.RemoveValue("rotation_angle")
+            default_parameters.AddValue("rotation_angle", parameters["rotation_angle"])
+
+        parameters.ValidateAndAssignDefaults(default_parameters)
+        self.model_part = model[parameters["model_part_name"].GetString()]
+
+        # Parse interval
+        self.interval_utility = KratosMultiphysics.IntervalUtility(parameters)
+
+        # Determine whether a constant transform will suffice or a parametric one is needed
+        requires_parametric_transform = False
+
+        euler_angle_parameters = parameters["euler_angles"]
+        rotation_axis_parameters = parameters["rotation_axis"]
+        rotation_angle_parameters = parameters["rotation_angle"]
+        reference_point_parameters = parameters["reference_point"]
+        translation_vector_parameters = parameters["translation_vector"]
+
+        if rotation_angle_parameters.IsString():
+            requires_parametric_transform = True
+        else:
+            for i in range(3):
+                if euler_angle_parameters[i].IsString() or rotation_axis_parameters[i].IsString() or reference_point_parameters[i].IsString() or translation_vector_parameters[i].IsString():
+                    requires_parametric_transform = True
+                    break
+
+        rotation_definition = parameters["rotation_definition"].GetString()
+
+        if requires_parametric_transform:
+            if rotation_definition == "rotation_axis":
+                self.transform = MeshMovingApplication.ParametricAffineTransform(
+                    rotation_axis_parameters,
+                    rotation_angle_parameters,
+                    reference_point_parameters,
+                    translation_vector_parameters)
+            elif rotation_definition == "euler_angles":
+                self.transform = MeshMovingApplication.ParametricAffineTransform(
+                    euler_angle_parameters,
+                    reference_point_parameters,
+                    translation_vector_parameters)
+            else:
+                raise ValueError("Invalid rotation definition '{}'".format(rotation_definition))
+
+        else:
+            reference_point = reference_point_parameters.GetVector()
+            translation_vector = translation_vector_parameters.GetVector()
+            if rotation_definition == "rotation_axis":
+                rotation_axis = rotation_axis_parameters.GetVector()
+                rotation_angle = rotation_angle_parameters.GetDouble()
+                self.transform = MeshMovingApplication.AffineTransform(
+                    rotation_axis,
+                    rotation_angle,
+                    reference_point,
+                    translation_vector)
+            elif rotation_definition == "euler_angles":
+                euler_angles = euler_angle_parameters.GetVector()
+                self.transform = MeshMovingApplication.AffineTransform(
+                    euler_angles,
+                    reference_point,
+                    translation_vector)
+            else:
+                raise ValueError("Invalid rotation definition '{}'".format(rotation_definition))
+
+
+    def ExecuteInitializeSolutionStep(self):
+        time = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
+
+        if self.interval_utility.IsInInterval(time):
+            MeshMovingApplication.MoveModelPart(self.model_part, self.transform)
+
+
+    @staticmethod
+    def GetDefaultParameters():
+        return KratosMultiphysics.Parameters("""{
+            "model_part_name"       : "",
+            "interval"              : [0.0, "End"],
+            "rotation_definition"   : "rotation_axis",
+            "euler_angles"          : [0.0, 0.0, 0.0],
+            "rotation_axis"         : [0.0, 0.0, 1.0],
+            "reference_point"       : [0.0, 0.0, 0.0],
+            "rotation_angle"        : 0,
+            "translation_vector"    : [0.0, 0.0, 0.0]
         }""")
```

## KratosMultiphysics/MeshMovingApplication/mesh_moving_analysis.py

 * *Ordering differences only*

```diff
@@ -1,86 +1,86 @@
-# Importing Kratos
-import KratosMultiphysics
-import KratosMultiphysics.MeshMovingApplication.python_solvers_wrapper_mesh_motion as mesh_mothion_solvers
-
-# Importing the base class
-from KratosMultiphysics.analysis_stage import AnalysisStage
-
-class MeshMovingAnalysis(AnalysisStage):
-    """
-    This class is the main-script of the MeshMovingApplication put in a class
-    It can be imported and used as "black-box"
-    """
-    def __init__(self, model, project_parameters):
-        # Making sure that older cases fail with a meaningful error message
-        solver_settings = project_parameters["solver_settings"]
-        if not solver_settings.Has("time_stepping"):
-            raise Exception("Using the old way to pass the time_step, this was removed!")
-
-        if not solver_settings.Has("domain_size"):
-            raise Exception("Using the old way to pass the domain_size, this was removed!")
-
-        if not solver_settings.Has("model_part_name"):
-            raise Exception("Using the old way to pass the model_part_name, this was removed!")
-
-        if not solver_settings.Has("echo_level"): # this is done to remain backwards-compatible
-            raise Exception('"solver_settings" does not have "echo_level", please add it!')
-
-        super().__init__(model, project_parameters)
-
-    #### Internal functions ####
-    def _CreateSolver(self):
-        """ Create the Solver (and create and import the ModelPart if it is not alread in the model) """
-        return mesh_mothion_solvers.CreateSolver(self.model, self.project_parameters)
-
-    def _CreateProcesses(self, parameter_name, initialization_order):
-        """Create a list of Processes
-        This method is TEMPORARY to not break existing code
-        It was removed, now throwing errors to avoid silent failures
-        """
-        list_of_processes = super()._CreateProcesses(parameter_name, initialization_order)
-
-        if parameter_name == "processes":
-            processes_block_names = ["boundary_conditions_process_list", "list_other_processes", "json_output_process",
-                "json_check_process", "check_analytic_results_process"]
-            if len(list_of_processes) == 0: # Processes are given in the old format (or no processes are specified)
-                for process_name in processes_block_names:
-                    if self.project_parameters.Has(process_name):
-                        raise Exception("Using the old way to create the processes, this was removed!")
-            else: # Processes are given in the new format
-                for process_name in processes_block_names:
-                    if self.project_parameters.Has(process_name):
-                        raise Exception("Mixing of process initialization is not alowed!")
-        elif parameter_name == "output_processes":
-            if self.project_parameters.Has("output_configuration"):
-                raise Exception("Using the old way to create the gid-output, this was removed!")
-        else:
-            raise NameError("wrong parameter name")
-
-        return list_of_processes
-
-    def _GetSimulationName(self):
-        return "::[Mesh Moving Simulation]:: "
-
-if __name__ == "__main__":
-    from sys import argv
-
-    if len(argv) > 2:
-        err_msg =  'Too many input arguments!\n'
-        err_msg += 'Use this script in the following way:\n'
-        err_msg += '- With default ProjectParameters (read from "ProjectParameters.json"):\n'
-        err_msg += '    "python3 mesh_moving_analysis.py"\n'
-        err_msg += '- With custom ProjectParameters:\n'
-        err_msg += '    "python3 mesh_moving_analysis.py CustomProjectParameters.json"\n'
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
-    simulation = MeshMovingAnalysis(model, parameters)
-    simulation.Run()
+# Importing Kratos
+import KratosMultiphysics
+import KratosMultiphysics.MeshMovingApplication.python_solvers_wrapper_mesh_motion as mesh_mothion_solvers
+
+# Importing the base class
+from KratosMultiphysics.analysis_stage import AnalysisStage
+
+class MeshMovingAnalysis(AnalysisStage):
+    """
+    This class is the main-script of the MeshMovingApplication put in a class
+    It can be imported and used as "black-box"
+    """
+    def __init__(self, model, project_parameters):
+        # Making sure that older cases fail with a meaningful error message
+        solver_settings = project_parameters["solver_settings"]
+        if not solver_settings.Has("time_stepping"):
+            raise Exception("Using the old way to pass the time_step, this was removed!")
+
+        if not solver_settings.Has("domain_size"):
+            raise Exception("Using the old way to pass the domain_size, this was removed!")
+
+        if not solver_settings.Has("model_part_name"):
+            raise Exception("Using the old way to pass the model_part_name, this was removed!")
+
+        if not solver_settings.Has("echo_level"): # this is done to remain backwards-compatible
+            raise Exception('"solver_settings" does not have "echo_level", please add it!')
+
+        super().__init__(model, project_parameters)
+
+    #### Internal functions ####
+    def _CreateSolver(self):
+        """ Create the Solver (and create and import the ModelPart if it is not alread in the model) """
+        return mesh_mothion_solvers.CreateSolver(self.model, self.project_parameters)
+
+    def _CreateProcesses(self, parameter_name, initialization_order):
+        """Create a list of Processes
+        This method is TEMPORARY to not break existing code
+        It was removed, now throwing errors to avoid silent failures
+        """
+        list_of_processes = super()._CreateProcesses(parameter_name, initialization_order)
+
+        if parameter_name == "processes":
+            processes_block_names = ["boundary_conditions_process_list", "list_other_processes", "json_output_process",
+                "json_check_process", "check_analytic_results_process"]
+            if len(list_of_processes) == 0: # Processes are given in the old format (or no processes are specified)
+                for process_name in processes_block_names:
+                    if self.project_parameters.Has(process_name):
+                        raise Exception("Using the old way to create the processes, this was removed!")
+            else: # Processes are given in the new format
+                for process_name in processes_block_names:
+                    if self.project_parameters.Has(process_name):
+                        raise Exception("Mixing of process initialization is not alowed!")
+        elif parameter_name == "output_processes":
+            if self.project_parameters.Has("output_configuration"):
+                raise Exception("Using the old way to create the gid-output, this was removed!")
+        else:
+            raise NameError("wrong parameter name")
+
+        return list_of_processes
+
+    def _GetSimulationName(self):
+        return "::[Mesh Moving Simulation]:: "
+
+if __name__ == "__main__":
+    from sys import argv
+
+    if len(argv) > 2:
+        err_msg =  'Too many input arguments!\n'
+        err_msg += 'Use this script in the following way:\n'
+        err_msg += '- With default ProjectParameters (read from "ProjectParameters.json"):\n'
+        err_msg += '    "python3 mesh_moving_analysis.py"\n'
+        err_msg += '- With custom ProjectParameters:\n'
+        err_msg += '    "python3 mesh_moving_analysis.py CustomProjectParameters.json"\n'
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
+    simulation = MeshMovingAnalysis(model, parameters)
+    simulation.Run()
```

## KratosMultiphysics/MeshMovingApplication/mesh_solver_base.py

 * *Ordering differences only*

```diff
@@ -1,264 +1,264 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-import KratosMultiphysics.MeshMovingApplication as KMM
-
-# Other imports
-from KratosMultiphysics.python_solver import PythonSolver
-
-
-class MeshSolverBase(PythonSolver):
-    """The base class for mesh motion solvers.
-
-    This class defines the user interface to mesh motion solvers.
-
-    Derived classes must override the function _CreateSolutionStrategy()
-    to customize the mesh motion algorithm. The mesh motion solving strategy and linear
-    solver should always be retrieved using the getter functions. Only the
-    member variables listed below should be accessed directly.
-
-    Public member variables:
-    settings -- Kratos parameters for general mesh motion settings.
-    mesh_model_part -- the mesh motion model part.
-    """
-    def __init__(self, model, custom_settings):
-        self._validate_settings_in_baseclass=True # To be removed eventually
-        super().__init__(model, custom_settings)
-
-        # Either retrieve the model part from the model or create a new one
-        model_part_name = self.settings["model_part_name"].GetString()
-
-        if model_part_name == "":
-            raise Exception('Please provide the model part name as the "model_part_name" (string) parameter!')
-
-        if self.model.HasModelPart(model_part_name):
-            self.mesh_model_part = self.model.GetModelPart(model_part_name)
-        else:
-            self.mesh_model_part = model.CreateModelPart(model_part_name)
-
-        domain_size = self.settings["domain_size"].GetInt()
-        if domain_size == -1:
-            raise Exception('Please provide the domain size as the "domain_size" (int) parameter!')
-
-        self.mesh_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, domain_size)
-
-        # If required, create the time discretization helper
-        if self.settings["calculate_mesh_velocity"].GetBool():
-            # BDF2 was the default in the MeshSolver-Strategies
-            default_settings = KratosMultiphysics.Parameters("""{
-                "time_scheme" : "bdf2",
-                "alpha_m": 0.0,
-                "alpha_f": 0.0
-            }""")
-
-            self.settings["mesh_velocity_calculation"].ValidateAndAssignDefaults(default_settings)
-            self.__CreateTimeIntegratorHelper()
-
-        self.reinitialize_model_part_each_step = self.settings["reinitialize_model_part_each_step"].GetBool()
-
-        KratosMultiphysics.Logger.PrintInfo("::[MeshSolverBase]:: Construction finished")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        this_defaults = KratosMultiphysics.Parameters("""{
-            "solver_type"           : "mesh_solver_base",
-            "buffer_size"           : 1,
-            "domain_size"           : -1,
-            "model_part_name"       : "",
-            "time_stepping"         : { },
-            "model_import_settings" : {
-                "input_type"     : "mdpa",
-                "input_filename" : "unknown_name"
-            },
-            "linear_solver_settings" : {
-                "solver_type" : "amgcl",
-                "smoother_type":"ilu0",
-                "krylov_type": "gmres",
-                "coarsening_type": "aggregation",
-                "max_iteration": 200,
-                "provide_coordinates": false,
-                "gmres_krylov_space_dimension": 100,
-                "verbosity" : 0,
-                "tolerance": 1e-7,
-                "scaling": false,
-                "block_size": 1,
-                "use_block_matrices_if_possible" : true,
-                "coarse_enough" : 5000
-            },
-            "reform_dofs_each_step"     : false,
-            "compute_reactions"         : false,
-            "poisson_ratio"             : 0.3,
-            "calculate_mesh_velocity"   : true,
-            "mesh_velocity_calculation" : { },
-            "superimpose_mesh_disp_with": [],
-            "superimpose_mesh_velocity_with": [],
-            "reinitialize_model_part_each_step": false
-        }""")
-        this_defaults.AddMissingParameters(super().GetDefaultParameters())
-        return this_defaults
-
-    #### Public user interface functions ####
-
-    def AddVariables(self):
-        # Add variables required for the mesh moving calculation
-        self.mesh_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.MESH_DISPLACEMENT)
-        self.mesh_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.MESH_REACTION)
-
-        # Adding Variables used for computation of Mesh-Velocity
-        if self.settings["calculate_mesh_velocity"].GetBool():
-            self.mesh_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.MESH_VELOCITY)
-            time_scheme = self.settings["mesh_velocity_calculation"]["time_scheme"].GetString()
-            if not time_scheme.startswith("bdf"): # bdfx does not need MESH_ACCELERATION
-                self.mesh_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.MESH_ACCELERATION)
-
-        KratosMultiphysics.Logger.PrintInfo("::[MeshSolverBase]:: Variables ADDED.")
-
-    def AddDofs(self):
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.MESH_DISPLACEMENT_X, KratosMultiphysics.MESH_REACTION_X, self.mesh_model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.MESH_DISPLACEMENT_Y, KratosMultiphysics.MESH_REACTION_Y, self.mesh_model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.MESH_DISPLACEMENT_Z, KratosMultiphysics.MESH_REACTION_Z, self.mesh_model_part)
-        KratosMultiphysics.Logger.PrintInfo("::[MeshSolverBase]:: DOFs ADDED.")
-
-    def AdvanceInTime(self, current_time):
-        dt = self.settings["time_stepping"]["time_step"].GetDouble()
-        new_time = current_time + dt
-        self.mesh_model_part.ProcessInfo[KratosMultiphysics.STEP] += 1
-        self.mesh_model_part.CloneTimeStep(new_time)
-
-        return new_time
-
-    def Initialize(self):
-        self._GetSolutionStrategy().Initialize()
-        #self.neighbour_search.Execute()
-        KratosMultiphysics.Logger.PrintInfo("::[MeshSolverBase]:: Finished initialization.")
-
-    def InitializeSolutionStep(self):
-        self._GetSolutionStrategy().InitializeSolutionStep()
-
-    def FinalizeSolutionStep(self):
-        self._GetSolutionStrategy().FinalizeSolutionStep()
-
-    def Predict(self):
-        self._GetSolutionStrategy().Predict()
-
-    def SolveSolutionStep(self):
-        # Calling Solve bcs this is what is currently implemented in the MeshSolverStrategies
-        # explicit bool conversion is only needed bcs "Solve" returns a double
-        is_converged = bool(self._GetSolutionStrategy().Solve())
-        self.MoveMesh()
-
-        # Superimpose the user-defined mesh displacement
-        for variable in KratosMultiphysics.kratos_utilities.GenerateVariableListFromInput(self.settings["superimpose_mesh_disp_with"]):
-            KMM.SuperImposeMeshDisplacement(variable)
-
-        # Superimpose the user-defined mesh velocity
-        for variable in KratosMultiphysics.kratos_utilities.GenerateVariableListFromInput(self.settings["superimpose_mesh_velocity_with"]):
-            KMM.SuperImposeMeshVelocity(variable)
-
-        return is_converged
-
-    def SetEchoLevel(self, level):
-        self._GetSolutionStrategy().SetEchoLevel(level)
-
-    def GetEchoLevel(self):
-        self._GetSolutionStrategy().GetEchoLevel()
-
-    def Clear(self):
-        self._GetSolutionStrategy().Clear()
-
-    def GetMinimumBufferSize(self):
-        buffer_size = max(self.settings["buffer_size"].GetInt(), self.mesh_model_part.GetBufferSize())
-        if self.settings["calculate_mesh_velocity"].GetBool():
-            buffer_size = max(buffer_size, KratosMultiphysics.TimeDiscretization.GetMinimumBufferSize(self.time_int_helper))
-        return buffer_size
-
-    def MoveMesh(self):
-        # move local and ghost nodes
-        self.mesh_model_part.GetCommunicator().SynchronizeVariable(KratosMultiphysics.MESH_DISPLACEMENT)
-        KMM.MoveMesh(self.mesh_model_part.Nodes)
-
-        # If required, calculate the MESH_VELOCITY.
-        if self.settings["calculate_mesh_velocity"].GetBool():
-            KMM.CalculateMeshVelocities(self.mesh_model_part, self.time_int_helper)
-
-    def ImportModelPart(self):
-        # we can use the default implementation in the base class
-        self._ImportModelPart(self.mesh_model_part,self.settings["model_import_settings"])
-
-    def PrepareModelPart(self):
-        if not self.mesh_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
-            self._set_and_fill_buffer()
-
-    def GetComputingModelPart(self):
-        return self.mesh_model_part
-
-    #### Specific internal functions ####
-
-    def _GetLinearSolver(self):
-        if not hasattr(self, '_linear_solver'):
-            self._linear_solver = self._CreateLinearSolver()
-        return self._linear_solver
-
-    def _GetSolutionStrategy(self):
-        if not hasattr(self, '_mesh_motion_solving_strategy'):
-            self._mesh_motion_solving_strategy = self._CreateSolutionStrategy()
-        return self._mesh_motion_solving_strategy
-
-    #### Private functions ####
-
-    def _CreateLinearSolver(self):
-        from KratosMultiphysics.python_linear_solver_factory import ConstructSolver
-        return ConstructSolver(self.settings["linear_solver_settings"])
-
-    def _CreateSolutionStrategy(self):
-        """Create the mesh motion solving strategy.
-
-        The mesh motion solving strategy must provide the functions defined in SolutionStrategy.
-        """
-        raise Exception("Mesh motion solving strategy must be created by the derived class.")
-
-    def _set_and_fill_buffer(self):
-        """Prepare nodal solution step data containers and time step information. """
-        # Set the buffer size for the nodal solution steps data. Existing nodal
-        # solution step data may be lost.
-        buffer_size = self.GetMinimumBufferSize()
-        self.mesh_model_part.SetBufferSize(buffer_size)
-        # Cycle the buffer. This sets all historical nodal solution step data to
-        # the current value and initializes the time stepping in the process info.
-        delta_time = self.mesh_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
-        time = self.mesh_model_part.ProcessInfo[KratosMultiphysics.TIME]
-        step =-buffer_size
-        time = time - delta_time * buffer_size
-        self.mesh_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, time)
-        for i in range(0, buffer_size):
-            step = step + 1
-            time = time + delta_time
-            self.mesh_model_part.ProcessInfo.SetValue(KratosMultiphysics.STEP, step)
-            self.mesh_model_part.CloneTimeStep(time)
-        self.mesh_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED] = False
-
-    def __CreateTimeIntegratorHelper(self):
-        '''Initializing the helper-class for the time-integration
-        '''
-        mesh_vel_calc_setting = self.settings["mesh_velocity_calculation"]
-        time_scheme = mesh_vel_calc_setting["time_scheme"].GetString()
-
-        if time_scheme == "bdf1":
-            self.time_int_helper = KratosMultiphysics.TimeDiscretization.BDF1()
-        elif time_scheme == "bdf2":
-            self.time_int_helper = KratosMultiphysics.TimeDiscretization.BDF2()
-        elif time_scheme == "newmark":
-            self.time_int_helper = KratosMultiphysics.TimeDiscretization.Newmark()
-        elif time_scheme == "bossak":
-            if mesh_vel_calc_setting.Has("alpha_m"):
-                alpha_m = mesh_vel_calc_setting["alpha_m"].GetDouble()
-                self.time_int_helper = KratosMultiphysics.TimeDiscretization.Bossak(alpha_m)
-            else:
-                self.time_int_helper = KratosMultiphysics.TimeDiscretization.Bossak()
-        elif time_scheme == "generalized_alpha":
-            alpha_m = mesh_vel_calc_setting["alpha_m"].GetDouble()
-            alpha_f = mesh_vel_calc_setting["alpha_f"].GetDouble()
-            self.time_int_helper = KratosMultiphysics.TimeDiscretization.GeneralizedAlpha(alpha_m, alpha_f)
-        else:
-            err_msg =  'The requested time scheme "{}" is not available for the calculation of the mesh velocity!\n'.format(time_scheme)
-            err_msg += 'Available options are: "bdf1", "bdf2", "newmark", "bossak", "generalized_alpha"'
-            raise Exception(err_msg)
+# Importing the Kratos Library
+import KratosMultiphysics
+import KratosMultiphysics.MeshMovingApplication as KMM
+
+# Other imports
+from KratosMultiphysics.python_solver import PythonSolver
+
+
+class MeshSolverBase(PythonSolver):
+    """The base class for mesh motion solvers.
+
+    This class defines the user interface to mesh motion solvers.
+
+    Derived classes must override the function _CreateSolutionStrategy()
+    to customize the mesh motion algorithm. The mesh motion solving strategy and linear
+    solver should always be retrieved using the getter functions. Only the
+    member variables listed below should be accessed directly.
+
+    Public member variables:
+    settings -- Kratos parameters for general mesh motion settings.
+    mesh_model_part -- the mesh motion model part.
+    """
+    def __init__(self, model, custom_settings):
+        self._validate_settings_in_baseclass=True # To be removed eventually
+        super().__init__(model, custom_settings)
+
+        # Either retrieve the model part from the model or create a new one
+        model_part_name = self.settings["model_part_name"].GetString()
+
+        if model_part_name == "":
+            raise Exception('Please provide the model part name as the "model_part_name" (string) parameter!')
+
+        if self.model.HasModelPart(model_part_name):
+            self.mesh_model_part = self.model.GetModelPart(model_part_name)
+        else:
+            self.mesh_model_part = model.CreateModelPart(model_part_name)
+
+        domain_size = self.settings["domain_size"].GetInt()
+        if domain_size == -1:
+            raise Exception('Please provide the domain size as the "domain_size" (int) parameter!')
+
+        self.mesh_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, domain_size)
+
+        # If required, create the time discretization helper
+        if self.settings["calculate_mesh_velocity"].GetBool():
+            # BDF2 was the default in the MeshSolver-Strategies
+            default_settings = KratosMultiphysics.Parameters("""{
+                "time_scheme" : "bdf2",
+                "alpha_m": 0.0,
+                "alpha_f": 0.0
+            }""")
+
+            self.settings["mesh_velocity_calculation"].ValidateAndAssignDefaults(default_settings)
+            self.__CreateTimeIntegratorHelper()
+
+        self.reinitialize_model_part_each_step = self.settings["reinitialize_model_part_each_step"].GetBool()
+
+        KratosMultiphysics.Logger.PrintInfo("::[MeshSolverBase]:: Construction finished")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        this_defaults = KratosMultiphysics.Parameters("""{
+            "solver_type"           : "mesh_solver_base",
+            "buffer_size"           : 1,
+            "domain_size"           : -1,
+            "model_part_name"       : "",
+            "time_stepping"         : { },
+            "model_import_settings" : {
+                "input_type"     : "mdpa",
+                "input_filename" : "unknown_name"
+            },
+            "linear_solver_settings" : {
+                "solver_type" : "amgcl",
+                "smoother_type":"ilu0",
+                "krylov_type": "gmres",
+                "coarsening_type": "aggregation",
+                "max_iteration": 200,
+                "provide_coordinates": false,
+                "gmres_krylov_space_dimension": 100,
+                "verbosity" : 0,
+                "tolerance": 1e-7,
+                "scaling": false,
+                "block_size": 1,
+                "use_block_matrices_if_possible" : true,
+                "coarse_enough" : 5000
+            },
+            "reform_dofs_each_step"     : false,
+            "compute_reactions"         : false,
+            "poisson_ratio"             : 0.3,
+            "calculate_mesh_velocity"   : true,
+            "mesh_velocity_calculation" : { },
+            "superimpose_mesh_disp_with": [],
+            "superimpose_mesh_velocity_with": [],
+            "reinitialize_model_part_each_step": false
+        }""")
+        this_defaults.AddMissingParameters(super().GetDefaultParameters())
+        return this_defaults
+
+    #### Public user interface functions ####
+
+    def AddVariables(self):
+        # Add variables required for the mesh moving calculation
+        self.mesh_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.MESH_DISPLACEMENT)
+        self.mesh_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.MESH_REACTION)
+
+        # Adding Variables used for computation of Mesh-Velocity
+        if self.settings["calculate_mesh_velocity"].GetBool():
+            self.mesh_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.MESH_VELOCITY)
+            time_scheme = self.settings["mesh_velocity_calculation"]["time_scheme"].GetString()
+            if not time_scheme.startswith("bdf"): # bdfx does not need MESH_ACCELERATION
+                self.mesh_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.MESH_ACCELERATION)
+
+        KratosMultiphysics.Logger.PrintInfo("::[MeshSolverBase]:: Variables ADDED.")
+
+    def AddDofs(self):
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.MESH_DISPLACEMENT_X, KratosMultiphysics.MESH_REACTION_X, self.mesh_model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.MESH_DISPLACEMENT_Y, KratosMultiphysics.MESH_REACTION_Y, self.mesh_model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.MESH_DISPLACEMENT_Z, KratosMultiphysics.MESH_REACTION_Z, self.mesh_model_part)
+        KratosMultiphysics.Logger.PrintInfo("::[MeshSolverBase]:: DOFs ADDED.")
+
+    def AdvanceInTime(self, current_time):
+        dt = self.settings["time_stepping"]["time_step"].GetDouble()
+        new_time = current_time + dt
+        self.mesh_model_part.ProcessInfo[KratosMultiphysics.STEP] += 1
+        self.mesh_model_part.CloneTimeStep(new_time)
+
+        return new_time
+
+    def Initialize(self):
+        self._GetSolutionStrategy().Initialize()
+        #self.neighbour_search.Execute()
+        KratosMultiphysics.Logger.PrintInfo("::[MeshSolverBase]:: Finished initialization.")
+
+    def InitializeSolutionStep(self):
+        self._GetSolutionStrategy().InitializeSolutionStep()
+
+    def FinalizeSolutionStep(self):
+        self._GetSolutionStrategy().FinalizeSolutionStep()
+
+    def Predict(self):
+        self._GetSolutionStrategy().Predict()
+
+    def SolveSolutionStep(self):
+        # Calling Solve bcs this is what is currently implemented in the MeshSolverStrategies
+        # explicit bool conversion is only needed bcs "Solve" returns a double
+        is_converged = bool(self._GetSolutionStrategy().Solve())
+        self.MoveMesh()
+
+        # Superimpose the user-defined mesh displacement
+        for variable in KratosMultiphysics.kratos_utilities.GenerateVariableListFromInput(self.settings["superimpose_mesh_disp_with"]):
+            KMM.SuperImposeMeshDisplacement(variable)
+
+        # Superimpose the user-defined mesh velocity
+        for variable in KratosMultiphysics.kratos_utilities.GenerateVariableListFromInput(self.settings["superimpose_mesh_velocity_with"]):
+            KMM.SuperImposeMeshVelocity(variable)
+
+        return is_converged
+
+    def SetEchoLevel(self, level):
+        self._GetSolutionStrategy().SetEchoLevel(level)
+
+    def GetEchoLevel(self):
+        self._GetSolutionStrategy().GetEchoLevel()
+
+    def Clear(self):
+        self._GetSolutionStrategy().Clear()
+
+    def GetMinimumBufferSize(self):
+        buffer_size = max(self.settings["buffer_size"].GetInt(), self.mesh_model_part.GetBufferSize())
+        if self.settings["calculate_mesh_velocity"].GetBool():
+            buffer_size = max(buffer_size, KratosMultiphysics.TimeDiscretization.GetMinimumBufferSize(self.time_int_helper))
+        return buffer_size
+
+    def MoveMesh(self):
+        # move local and ghost nodes
+        self.mesh_model_part.GetCommunicator().SynchronizeVariable(KratosMultiphysics.MESH_DISPLACEMENT)
+        KMM.MoveMesh(self.mesh_model_part.Nodes)
+
+        # If required, calculate the MESH_VELOCITY.
+        if self.settings["calculate_mesh_velocity"].GetBool():
+            KMM.CalculateMeshVelocities(self.mesh_model_part, self.time_int_helper)
+
+    def ImportModelPart(self):
+        # we can use the default implementation in the base class
+        self._ImportModelPart(self.mesh_model_part,self.settings["model_import_settings"])
+
+    def PrepareModelPart(self):
+        if not self.mesh_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
+            self._set_and_fill_buffer()
+
+    def GetComputingModelPart(self):
+        return self.mesh_model_part
+
+    #### Specific internal functions ####
+
+    def _GetLinearSolver(self):
+        if not hasattr(self, '_linear_solver'):
+            self._linear_solver = self._CreateLinearSolver()
+        return self._linear_solver
+
+    def _GetSolutionStrategy(self):
+        if not hasattr(self, '_mesh_motion_solving_strategy'):
+            self._mesh_motion_solving_strategy = self._CreateSolutionStrategy()
+        return self._mesh_motion_solving_strategy
+
+    #### Private functions ####
+
+    def _CreateLinearSolver(self):
+        from KratosMultiphysics.python_linear_solver_factory import ConstructSolver
+        return ConstructSolver(self.settings["linear_solver_settings"])
+
+    def _CreateSolutionStrategy(self):
+        """Create the mesh motion solving strategy.
+
+        The mesh motion solving strategy must provide the functions defined in SolutionStrategy.
+        """
+        raise Exception("Mesh motion solving strategy must be created by the derived class.")
+
+    def _set_and_fill_buffer(self):
+        """Prepare nodal solution step data containers and time step information. """
+        # Set the buffer size for the nodal solution steps data. Existing nodal
+        # solution step data may be lost.
+        buffer_size = self.GetMinimumBufferSize()
+        self.mesh_model_part.SetBufferSize(buffer_size)
+        # Cycle the buffer. This sets all historical nodal solution step data to
+        # the current value and initializes the time stepping in the process info.
+        delta_time = self.mesh_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
+        time = self.mesh_model_part.ProcessInfo[KratosMultiphysics.TIME]
+        step =-buffer_size
+        time = time - delta_time * buffer_size
+        self.mesh_model_part.ProcessInfo.SetValue(KratosMultiphysics.TIME, time)
+        for i in range(0, buffer_size):
+            step = step + 1
+            time = time + delta_time
+            self.mesh_model_part.ProcessInfo.SetValue(KratosMultiphysics.STEP, step)
+            self.mesh_model_part.CloneTimeStep(time)
+        self.mesh_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED] = False
+
+    def __CreateTimeIntegratorHelper(self):
+        '''Initializing the helper-class for the time-integration
+        '''
+        mesh_vel_calc_setting = self.settings["mesh_velocity_calculation"]
+        time_scheme = mesh_vel_calc_setting["time_scheme"].GetString()
+
+        if time_scheme == "bdf1":
+            self.time_int_helper = KratosMultiphysics.TimeDiscretization.BDF1()
+        elif time_scheme == "bdf2":
+            self.time_int_helper = KratosMultiphysics.TimeDiscretization.BDF2()
+        elif time_scheme == "newmark":
+            self.time_int_helper = KratosMultiphysics.TimeDiscretization.Newmark()
+        elif time_scheme == "bossak":
+            if mesh_vel_calc_setting.Has("alpha_m"):
+                alpha_m = mesh_vel_calc_setting["alpha_m"].GetDouble()
+                self.time_int_helper = KratosMultiphysics.TimeDiscretization.Bossak(alpha_m)
+            else:
+                self.time_int_helper = KratosMultiphysics.TimeDiscretization.Bossak()
+        elif time_scheme == "generalized_alpha":
+            alpha_m = mesh_vel_calc_setting["alpha_m"].GetDouble()
+            alpha_f = mesh_vel_calc_setting["alpha_f"].GetDouble()
+            self.time_int_helper = KratosMultiphysics.TimeDiscretization.GeneralizedAlpha(alpha_m, alpha_f)
+        else:
+            err_msg =  'The requested time scheme "{}" is not available for the calculation of the mesh velocity!\n'.format(time_scheme)
+            err_msg += 'Available options are: "bdf1", "bdf2", "newmark", "bossak", "generalized_alpha"'
+            raise Exception(err_msg)
```

## KratosMultiphysics/MeshMovingApplication/mesh_solver_laplacian.py

 * *Ordering differences only*

```diff
@@ -1,42 +1,42 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KM
-
-# Import applications
-import KratosMultiphysics.MeshMovingApplication as KratosMeshMoving
-
-# Import baseclass
-from KratosMultiphysics.MeshMovingApplication.mesh_solver_base import MeshSolverBase
-
-
-def CreateSolver(model, custom_settings):
-    return MeshSolverLaplacian(model, custom_settings)
-
-
-class MeshSolverLaplacian(MeshSolverBase):
-    def __init__(self, model, custom_settings):
-        super().__init__(model, custom_settings)
-        if custom_settings["buffer_size"].GetInt() < 2:
-            raise Exception("A buffer_size of at least 2 is required!")
-        KM.Logger.PrintInfo("::[MeshSolverLaplacian]:: Construction finished")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        this_defaults = KM.Parameters("""{
-            "buffer_size"           : 2
-        }""")
-        this_defaults.AddMissingParameters(super().GetDefaultParameters())
-        return this_defaults
-
-    def _CreateSolutionStrategy(self):
-        linear_solver = self._GetLinearSolver()
-        reform_dofs_each_step = self.settings["reform_dofs_each_step"].GetBool()
-        compute_reactions = self.settings["compute_reactions"].GetBool()
-        solving_strategy = KratosMeshMoving.LaplacianMeshMovingStrategy(self.mesh_model_part,
-                                                            linear_solver,
-                                                            0,
-                                                            reform_dofs_each_step,
-                                                            compute_reactions,
-                                                            False,
-                                                            self.echo_level,
-                                                            self.reinitialize_model_part_each_step)
-        return solving_strategy
+# Importing the Kratos Library
+import KratosMultiphysics as KM
+
+# Import applications
+import KratosMultiphysics.MeshMovingApplication as KratosMeshMoving
+
+# Import baseclass
+from KratosMultiphysics.MeshMovingApplication.mesh_solver_base import MeshSolverBase
+
+
+def CreateSolver(model, custom_settings):
+    return MeshSolverLaplacian(model, custom_settings)
+
+
+class MeshSolverLaplacian(MeshSolverBase):
+    def __init__(self, model, custom_settings):
+        super().__init__(model, custom_settings)
+        if custom_settings["buffer_size"].GetInt() < 2:
+            raise Exception("A buffer_size of at least 2 is required!")
+        KM.Logger.PrintInfo("::[MeshSolverLaplacian]:: Construction finished")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        this_defaults = KM.Parameters("""{
+            "buffer_size"           : 2
+        }""")
+        this_defaults.AddMissingParameters(super().GetDefaultParameters())
+        return this_defaults
+
+    def _CreateSolutionStrategy(self):
+        linear_solver = self._GetLinearSolver()
+        reform_dofs_each_step = self.settings["reform_dofs_each_step"].GetBool()
+        compute_reactions = self.settings["compute_reactions"].GetBool()
+        solving_strategy = KratosMeshMoving.LaplacianMeshMovingStrategy(self.mesh_model_part,
+                                                            linear_solver,
+                                                            0,
+                                                            reform_dofs_each_step,
+                                                            compute_reactions,
+                                                            False,
+                                                            self.echo_level,
+                                                            self.reinitialize_model_part_each_step)
+        return solving_strategy
```

## KratosMultiphysics/MeshMovingApplication/mesh_solver_structural_similarity.py

 * *Ordering differences only*

```diff
@@ -1,34 +1,34 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications
-import KratosMultiphysics.MeshMovingApplication as KratosMeshMoving
-
-# Import baseclass
-from KratosMultiphysics.MeshMovingApplication.mesh_solver_base import MeshSolverBase
-
-
-def CreateSolver(model, custom_settings):
-    return MeshSolverStructuralSimilarity(model, custom_settings)
-
-
-class MeshSolverStructuralSimilarity(MeshSolverBase):
-    def __init__(self, model, custom_settings):
-        super().__init__(model, custom_settings)
-        KratosMultiphysics.Logger.PrintInfo("::[MeshSolverStructuralSimilarity]:: Construction finished")
-
-    def _CreateSolutionStrategy(self):
-        linear_solver = self._GetLinearSolver()
-        reform_dofs_each_step = self.settings["reform_dofs_each_step"].GetBool()
-        compute_reactions = self.settings["compute_reactions"].GetBool()
-        poisson_ratio = self.settings["poisson_ratio"].GetDouble()
-        solving_strategy = KratosMeshMoving.StructuralMeshMovingStrategy(self.mesh_model_part,
-                                                             linear_solver,
-                                                             0,
-                                                             reform_dofs_each_step,
-                                                             compute_reactions,
-                                                             False,
-                                                             self.echo_level,
-                                                             poisson_ratio,
-                                                             self.reinitialize_model_part_each_step)
-        return solving_strategy
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications
+import KratosMultiphysics.MeshMovingApplication as KratosMeshMoving
+
+# Import baseclass
+from KratosMultiphysics.MeshMovingApplication.mesh_solver_base import MeshSolverBase
+
+
+def CreateSolver(model, custom_settings):
+    return MeshSolverStructuralSimilarity(model, custom_settings)
+
+
+class MeshSolverStructuralSimilarity(MeshSolverBase):
+    def __init__(self, model, custom_settings):
+        super().__init__(model, custom_settings)
+        KratosMultiphysics.Logger.PrintInfo("::[MeshSolverStructuralSimilarity]:: Construction finished")
+
+    def _CreateSolutionStrategy(self):
+        linear_solver = self._GetLinearSolver()
+        reform_dofs_each_step = self.settings["reform_dofs_each_step"].GetBool()
+        compute_reactions = self.settings["compute_reactions"].GetBool()
+        poisson_ratio = self.settings["poisson_ratio"].GetDouble()
+        solving_strategy = KratosMeshMoving.StructuralMeshMovingStrategy(self.mesh_model_part,
+                                                             linear_solver,
+                                                             0,
+                                                             reform_dofs_each_step,
+                                                             compute_reactions,
+                                                             False,
+                                                             self.echo_level,
+                                                             poisson_ratio,
+                                                             self.reinitialize_model_part_each_step)
+        return solving_strategy
```

## KratosMultiphysics/MeshMovingApplication/python_solvers_wrapper_mesh_motion.py

 * *Ordering differences only*

```diff
@@ -1,62 +1,62 @@
-import KratosMultiphysics
-from importlib import import_module
-
-def CreateSolverByParameters(model, solver_settings, parallelism):
-
-    solver_type = solver_settings["solver_type"].GetString()
-    if solver_type.startswith("mesh_solver_"):
-        solver_type = solver_type[12:] # remove preceding "mesh_solver_"
-        depr_msg  = 'Using the old names to construct the MeshSolver\n'
-        depr_msg += 'Please remove the preceding "mesh_solver_" from "solver_type"'
-        KratosMultiphysics.Logger.PrintWarning("DEPRECATION", depr_msg)
-
-    # Solvers for OpenMP parallelism
-    if (parallelism == "OpenMP"):
-
-        if (solver_type == "laplacian"):
-            solver_module_name = "mesh_solver_laplacian"
-
-        elif (solver_type == "structural_similarity"):
-            solver_module_name = "mesh_solver_structural_similarity"
-
-        else:
-            err_msg =  'The requested solver type "' + solver_type + '" is not in the python solvers wrapper\n'
-            err_msg += 'Available options are: "laplacian", "structural_similarity"'
-            raise Exception(err_msg)
-
-    # Solvers for MPI parallelism
-    elif (parallelism == "MPI"):
-
-        if (solver_type == "laplacian"):
-            solver_module_name = "trilinos_mesh_solver_laplacian"
-
-        elif (solver_type == "structural_similarity"):
-            solver_module_name = "trilinos_mesh_solver_structural_similarity"
-
-        else:
-            err_msg =  'The requested solver type "' + solver_type + '" is not in the python solvers wrapper\n'
-            err_msg += 'Available options are: "laplacian", "structural_similarity"'
-            raise Exception(err_msg)
-
-    else:
-        err_msg =  'The requested parallel type "' + parallelism + '" is not available!\n'
-        err_msg += 'Available options are: "OpenMP", "MPI"'
-        raise Exception(err_msg)
-
-    module_full = 'KratosMultiphysics.MeshMovingApplication.' + solver_module_name
-    solver = import_module(module_full).CreateSolver(model, solver_settings)
-
-    return solver
-
-def CreateSolver(model, custom_settings):
-
-    if (type(model) != KratosMultiphysics.Model):
-        raise Exception("input is expected to be provided as a Kratos Model object")#
-
-    if (type(custom_settings) != KratosMultiphysics.Parameters):
-        raise Exception("input is expected to be provided as a Kratos Parameters object")
-
-    solver_settings = custom_settings["solver_settings"]
-    parallelism = custom_settings["problem_data"]["parallel_type"].GetString()
-
-    return CreateSolverByParameters(model, solver_settings, parallelism)
+import KratosMultiphysics
+from importlib import import_module
+
+def CreateSolverByParameters(model, solver_settings, parallelism):
+
+    solver_type = solver_settings["solver_type"].GetString()
+    if solver_type.startswith("mesh_solver_"):
+        solver_type = solver_type[12:] # remove preceding "mesh_solver_"
+        depr_msg  = 'Using the old names to construct the MeshSolver\n'
+        depr_msg += 'Please remove the preceding "mesh_solver_" from "solver_type"'
+        KratosMultiphysics.Logger.PrintWarning("DEPRECATION", depr_msg)
+
+    # Solvers for OpenMP parallelism
+    if (parallelism == "OpenMP"):
+
+        if (solver_type == "laplacian"):
+            solver_module_name = "mesh_solver_laplacian"
+
+        elif (solver_type == "structural_similarity"):
+            solver_module_name = "mesh_solver_structural_similarity"
+
+        else:
+            err_msg =  'The requested solver type "' + solver_type + '" is not in the python solvers wrapper\n'
+            err_msg += 'Available options are: "laplacian", "structural_similarity"'
+            raise Exception(err_msg)
+
+    # Solvers for MPI parallelism
+    elif (parallelism == "MPI"):
+
+        if (solver_type == "laplacian"):
+            solver_module_name = "trilinos_mesh_solver_laplacian"
+
+        elif (solver_type == "structural_similarity"):
+            solver_module_name = "trilinos_mesh_solver_structural_similarity"
+
+        else:
+            err_msg =  'The requested solver type "' + solver_type + '" is not in the python solvers wrapper\n'
+            err_msg += 'Available options are: "laplacian", "structural_similarity"'
+            raise Exception(err_msg)
+
+    else:
+        err_msg =  'The requested parallel type "' + parallelism + '" is not available!\n'
+        err_msg += 'Available options are: "OpenMP", "MPI"'
+        raise Exception(err_msg)
+
+    module_full = 'KratosMultiphysics.MeshMovingApplication.' + solver_module_name
+    solver = import_module(module_full).CreateSolver(model, solver_settings)
+
+    return solver
+
+def CreateSolver(model, custom_settings):
+
+    if (type(model) != KratosMultiphysics.Model):
+        raise Exception("input is expected to be provided as a Kratos Model object")#
+
+    if (type(custom_settings) != KratosMultiphysics.Parameters):
+        raise Exception("input is expected to be provided as a Kratos Parameters object")
+
+    solver_settings = custom_settings["solver_settings"]
+    parallelism = custom_settings["problem_data"]["parallel_type"].GetString()
+
+    return CreateSolverByParameters(model, solver_settings, parallelism)
```

## KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_base.py

 * *Ordering differences only*

```diff
@@ -1,78 +1,78 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications
-import KratosMultiphysics.MeshMovingApplication as KratosMeshMoving
-import KratosMultiphysics.TrilinosApplication as TrilinosApplication
-from KratosMultiphysics.TrilinosApplication import trilinos_linear_solver_factory
-
-# Import baseclass
-from KratosMultiphysics.MeshMovingApplication.mesh_solver_base import MeshSolverBase
-
-# Importing MPI extensions to Kratos
-from KratosMultiphysics.mpi.distributed_import_model_part_utility import DistributedImportModelPartUtility
-
-class TrilinosMeshSolverBase(MeshSolverBase):
-    def __init__(self, model, custom_settings):
-        super().__init__(model, custom_settings)
-        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverBase]:: Construction finished")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        this_defaults = KratosMultiphysics.Parameters("""{
-            "linear_solver_settings" : {
-                "solver_type" : "amgcl",
-                "smoother_type":"ilu0",
-                "krylov_type": "gmres",
-                "coarsening_type": "aggregation",
-                "max_iteration": 200,
-                "provide_coordinates": false,
-                "gmres_krylov_space_dimension": 100,
-                "verbosity" : 0,
-                "tolerance": 1e-7,
-                "scaling": false,
-                "block_size": 1,
-                "use_block_matrices_if_possible" : true,
-                "coarse_enough" : 5000
-            }
-        }""")
-        this_defaults.AddMissingParameters(super().GetDefaultParameters())
-        return this_defaults
-
-    #### Public user interface functions ####
-
-    def AddVariables(self):
-        super().AddVariables()
-        self.mesh_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PARTITION_INDEX)
-        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverBase]:: Variables ADDED.")
-
-    def ImportModelPart(self):
-        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverBase]:: ", "Importing model part.")
-        self.distributed_model_part_importer = DistributedImportModelPartUtility(self.mesh_model_part, self.settings)
-        self.distributed_model_part_importer.ImportModelPart()
-        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverBase]:: ", "Finished importing model part.")
-
-    def PrepareModelPart(self):
-        super().PrepareModelPart()
-        # Construct the mpi-communicator
-        self.distributed_model_part_importer.CreateCommunicators()
-        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverBase]::", "ModelPart prepared for Solver.")
-
-    def Finalize(self):
-        super().Finalize()
-        self._GetSolutionStrategy().Clear() # needed for proper finalization of MPI
-
-    #### Specific internal functions ####
-
-    def get_communicator(self):
-        if not hasattr(self, '_communicator'):
-            self._communicator = TrilinosApplication.CreateEpetraCommunicator(self.mesh_model_part.GetCommunicator().GetDataCommunicator())
-        return self._communicator
-
-    #### Private functions ####
-
-    def _CreateLinearSolver(self):
-        return trilinos_linear_solver_factory.ConstructSolver(self.settings["linear_solver_settings"])
-
-    def _CreateSolutionStrategy(self):
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications
+import KratosMultiphysics.MeshMovingApplication as KratosMeshMoving
+import KratosMultiphysics.TrilinosApplication as TrilinosApplication
+from KratosMultiphysics.TrilinosApplication import trilinos_linear_solver_factory
+
+# Import baseclass
+from KratosMultiphysics.MeshMovingApplication.mesh_solver_base import MeshSolverBase
+
+# Importing MPI extensions to Kratos
+from KratosMultiphysics.mpi.distributed_import_model_part_utility import DistributedImportModelPartUtility
+
+class TrilinosMeshSolverBase(MeshSolverBase):
+    def __init__(self, model, custom_settings):
+        super().__init__(model, custom_settings)
+        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverBase]:: Construction finished")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        this_defaults = KratosMultiphysics.Parameters("""{
+            "linear_solver_settings" : {
+                "solver_type" : "amgcl",
+                "smoother_type":"ilu0",
+                "krylov_type": "gmres",
+                "coarsening_type": "aggregation",
+                "max_iteration": 200,
+                "provide_coordinates": false,
+                "gmres_krylov_space_dimension": 100,
+                "verbosity" : 0,
+                "tolerance": 1e-7,
+                "scaling": false,
+                "block_size": 1,
+                "use_block_matrices_if_possible" : true,
+                "coarse_enough" : 5000
+            }
+        }""")
+        this_defaults.AddMissingParameters(super().GetDefaultParameters())
+        return this_defaults
+
+    #### Public user interface functions ####
+
+    def AddVariables(self):
+        super().AddVariables()
+        self.mesh_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PARTITION_INDEX)
+        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverBase]:: Variables ADDED.")
+
+    def ImportModelPart(self):
+        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverBase]:: ", "Importing model part.")
+        self.distributed_model_part_importer = DistributedImportModelPartUtility(self.mesh_model_part, self.settings)
+        self.distributed_model_part_importer.ImportModelPart()
+        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverBase]:: ", "Finished importing model part.")
+
+    def PrepareModelPart(self):
+        super().PrepareModelPart()
+        # Construct the mpi-communicator
+        self.distributed_model_part_importer.CreateCommunicators()
+        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverBase]::", "ModelPart prepared for Solver.")
+
+    def Finalize(self):
+        super().Finalize()
+        self._GetSolutionStrategy().Clear() # needed for proper finalization of MPI
+
+    #### Specific internal functions ####
+
+    def get_communicator(self):
+        if not hasattr(self, '_communicator'):
+            self._communicator = TrilinosApplication.CreateEpetraCommunicator(self.mesh_model_part.GetCommunicator().GetDataCommunicator())
+        return self._communicator
+
+    #### Private functions ####
+
+    def _CreateLinearSolver(self):
+        return trilinos_linear_solver_factory.ConstructSolver(self.settings["linear_solver_settings"])
+
+    def _CreateSolutionStrategy(self):
         raise Exception("Mesh motion solver must be created by the derived class.")
```

## KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_laplacian.py

 * *Ordering differences only*

```diff
@@ -1,46 +1,46 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications
-from KratosMultiphysics.MeshMovingApplication import TrilinosExtension as TrilinosMeshMoving
-
-# Import baseclass
-from KratosMultiphysics.MeshMovingApplication.trilinos_mesh_solver_base import TrilinosMeshSolverBase
-
-
-def CreateSolver(model, custom_settings):
-    return TrilinosMeshSolverLaplacian(model, custom_settings)
-
-
-class TrilinosMeshSolverLaplacian(TrilinosMeshSolverBase):
-    def __init__(self, model, custom_settings):
-        super().__init__(model, custom_settings)
-        if custom_settings["buffer_size"].GetInt() < 2:
-            raise Exception("A buffer_size of at least 2 is required!")
-        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverLaplacian]:: Construction finished")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        this_defaults = KratosMultiphysics.Parameters("""{
-            "buffer_size"           : 2
-        }""")
-        this_defaults.AddMissingParameters(super().GetDefaultParameters())
-        return this_defaults
-
-    #### Private functions ####
-
-    def _CreateSolutionStrategy(self):
-        linear_solver = self._GetLinearSolver()
-        reform_dofs_each_step = self.settings["reform_dofs_each_step"].GetBool()
-        compute_reactions = self.settings["compute_reactions"].GetBool()
-        communicator = self.get_communicator()
-        solving_strategy = TrilinosMeshMoving.TrilinosLaplacianMeshMovingStrategy(
-            communicator,
-            self.mesh_model_part,
-            linear_solver,
-            0,
-            reform_dofs_each_step,
-            compute_reactions,
-            False,
-            self.echo_level)
-        return solving_strategy
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications
+from KratosMultiphysics.MeshMovingApplication import TrilinosExtension as TrilinosMeshMoving
+
+# Import baseclass
+from KratosMultiphysics.MeshMovingApplication.trilinos_mesh_solver_base import TrilinosMeshSolverBase
+
+
+def CreateSolver(model, custom_settings):
+    return TrilinosMeshSolverLaplacian(model, custom_settings)
+
+
+class TrilinosMeshSolverLaplacian(TrilinosMeshSolverBase):
+    def __init__(self, model, custom_settings):
+        super().__init__(model, custom_settings)
+        if custom_settings["buffer_size"].GetInt() < 2:
+            raise Exception("A buffer_size of at least 2 is required!")
+        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverLaplacian]:: Construction finished")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        this_defaults = KratosMultiphysics.Parameters("""{
+            "buffer_size"           : 2
+        }""")
+        this_defaults.AddMissingParameters(super().GetDefaultParameters())
+        return this_defaults
+
+    #### Private functions ####
+
+    def _CreateSolutionStrategy(self):
+        linear_solver = self._GetLinearSolver()
+        reform_dofs_each_step = self.settings["reform_dofs_each_step"].GetBool()
+        compute_reactions = self.settings["compute_reactions"].GetBool()
+        communicator = self.get_communicator()
+        solving_strategy = TrilinosMeshMoving.TrilinosLaplacianMeshMovingStrategy(
+            communicator,
+            self.mesh_model_part,
+            linear_solver,
+            0,
+            reform_dofs_each_step,
+            compute_reactions,
+            False,
+            self.echo_level)
+        return solving_strategy
```

## KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_structural_similarity.py

 * *Ordering differences only*

```diff
@@ -1,36 +1,36 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications
-from KratosMultiphysics.MeshMovingApplication import TrilinosExtension as TrilinosMeshMoving
-
-# Import baseclass
-from KratosMultiphysics.MeshMovingApplication.trilinos_mesh_solver_base import TrilinosMeshSolverBase
-
-
-def CreateSolver(model, custom_settings):
-    return TrilinosMeshSolverStructuralSimilarity(model, custom_settings)
-
-
-class TrilinosMeshSolverStructuralSimilarity(TrilinosMeshSolverBase):
-    def __init__(self, model, custom_settings):
-        super().__init__(model, custom_settings)
-        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverStructuralSimilarity]:: Construction finished")
-
-    #### Private functions ####
-
-    def _CreateSolutionStrategy(self):
-        linear_solver = self._GetLinearSolver()
-        communicator = self.get_communicator()
-        reform_dofs_each_step = self.settings["reform_dofs_each_step"].GetBool()
-        compute_reactions = self.settings["compute_reactions"].GetBool()
-        solving_strategy = TrilinosMeshMoving.TrilinosStructuralMeshMovingStrategy(
-            communicator,
-            self.mesh_model_part,
-            linear_solver,
-            0,
-            reform_dofs_each_step,
-            compute_reactions,
-            False,
-            self.echo_level)
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications
+from KratosMultiphysics.MeshMovingApplication import TrilinosExtension as TrilinosMeshMoving
+
+# Import baseclass
+from KratosMultiphysics.MeshMovingApplication.trilinos_mesh_solver_base import TrilinosMeshSolverBase
+
+
+def CreateSolver(model, custom_settings):
+    return TrilinosMeshSolverStructuralSimilarity(model, custom_settings)
+
+
+class TrilinosMeshSolverStructuralSimilarity(TrilinosMeshSolverBase):
+    def __init__(self, model, custom_settings):
+        super().__init__(model, custom_settings)
+        KratosMultiphysics.Logger.PrintInfo("::[TrilinosMeshSolverStructuralSimilarity]:: Construction finished")
+
+    #### Private functions ####
+
+    def _CreateSolutionStrategy(self):
+        linear_solver = self._GetLinearSolver()
+        communicator = self.get_communicator()
+        reform_dofs_each_step = self.settings["reform_dofs_each_step"].GetBool()
+        compute_reactions = self.settings["compute_reactions"].GetBool()
+        solving_strategy = TrilinosMeshMoving.TrilinosStructuralMeshMovingStrategy(
+            communicator,
+            self.mesh_model_part,
+            linear_solver,
+            0,
+            reform_dofs_each_step,
+            compute_reactions,
+            False,
+            self.echo_level)
         return solving_strategy
```

## Comparing `KratosMeshMovingApplication-9.4.6.dist-info/METADATA` & `KratosMeshMovingApplication-9.5.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-Metadata-Version: 2.1
-Name: KratosMeshMovingApplication
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
-## MeshMoving Application
-
-The MeshMoving Application (formerly ALEapplication) contains different mesh-update techniques.
-
-A typical application for the use of mesh-moving is in Fluid-Structure Interaction (FSI) when the fluid mesh is moved after the displacements of the structure are mapped on the interface
-
-### Features:
-
-- laplacian mesh motion solver
-
-- structural similarity mesh motion solver
-
-- computation of mesh velocities (ALE)
-
-- ALE-fluid solver for the usage in FSI
-
-- works both in OpenMP and MPI
-
-### Usage
-
-Check the tests for examples on how to use the solvers.
+Metadata-Version: 2.1
+Name: KratosMeshMovingApplication
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
+## MeshMoving Application
+
+The MeshMoving Application (formerly ALEapplication) contains different mesh-update techniques.
+
+A typical application for the use of mesh-moving is in Fluid-Structure Interaction (FSI) when the fluid mesh is moved after the displacements of the structure are mapped on the interface
+
+### Features:
+
+- laplacian mesh motion solver
+
+- structural similarity mesh motion solver
+
+- computation of mesh velocities (ALE)
+
+- ALE-fluid solver for the usage in FSI
+
+- works both in OpenMP and MPI
+
+### Usage
+
+Check the tests for examples on how to use the solvers.
```

## Comparing `KratosMeshMovingApplication-9.4.6.dist-info/RECORD` & `KratosMeshMovingApplication-9.5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-KratosMultiphysics/.libs/KratosMeshMovingApplication.pyd,sha256=pQv1E6fxRpXHav3v8ESEEx43ZV9XJur_lvyqSXKu1qw,1201152
-KratosMultiphysics/.libs/KratosMeshMovingCore.dll,sha256=4cWQ9V2Ojc7ehZKeYzh3CPTlU40ZHxvMFm7pWs8y-c0,1745920
-KratosMultiphysics/.libs/KratosMeshMovingCore.lib,sha256=A7qtsqdxQ5kGp75VjM68dsd9rSkRTbI2I8vG45Xg_Eg,39344
-KratosMultiphysics/MeshMovingApplication/__init__.py,sha256=Xk-CWyo7y9-l4ZHKPWC7ZiKAbQ-b6DbcJESDSKzAuyY,242
-KratosMultiphysics/MeshMovingApplication/ale_fluid_solver.py,sha256=nXrGMAPig13-CRB8as0_ymx3eXn8LvznS95EIPDu_uE,10764
-KratosMultiphysics/MeshMovingApplication/impose_mesh_motion_process.py,sha256=gVTC36_Akg9tVzeiTjhHbV756ajJoOtv60Dvs5u4cnc,6535
-KratosMultiphysics/MeshMovingApplication/mesh_moving_analysis.py,sha256=Q3le-HQX0-dfsL2U1_6YDB1SORkVbKfopmQCoihpdQs,4221
-KratosMultiphysics/MeshMovingApplication/mesh_solver_base.py,sha256=Ige4YgzGqQVlCh8leskrh-E4EkS8Qw6FnFGBUA1qaW4,12534
-KratosMultiphysics/MeshMovingApplication/mesh_solver_laplacian.py,sha256=Nfsz2C90rzBJdkH1p_H8sYH9MaF38ZPZZxYT65q-fpM,1915
-KratosMultiphysics/MeshMovingApplication/mesh_solver_structural_similarity.py,sha256=gg5m9EJoak-uhF3ia_IjZmMREjw3VBesX7CJAgUDXfY,1719
-KratosMultiphysics/MeshMovingApplication/python_solvers_wrapper_mesh_motion.py,sha256=vz3mTLmJIxAiaQMBwMoekAmMUUKvcIxxWKx1I1b_Xew,2628
-KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_base.py,sha256=vydoFjyFwmQigDO7AB5GxeIcSAoxVb9El0MWM3fI0h4,3426
-KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_laplacian.py,sha256=wA86YM8SNqTX6s24yjjJHuRWmmZhJGqFwkEfKhWTNDY,1760
-KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_structural_similarity.py,sha256=ZYoKwAz93RUgMzbPvRw5OJSo7kTzS40IbowO9fwLnpI,1384
-KratosMeshMovingApplication-9.4.6.dist-info/METADATA,sha256=92KargY0ZVlNkk1bYLZX3YjXZlZsn6wEkDlA2S3TL-I,1986
-KratosMeshMovingApplication-9.4.6.dist-info/WHEEL,sha256=GZFS91_ufm4WrNPBaFVPB9MvOXR6bMZQhPcZRRTN5YM,100
-KratosMeshMovingApplication-9.4.6.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
-KratosMeshMovingApplication-9.4.6.dist-info/RECORD,,
+KratosMeshMovingApplication.libs/libKratosMeshMovingCore-b2b7db2c.so,sha256=Y53JjqvF8xGfYS00RJnkjbb2kfYudX4NTar4U9JuwUI,5864049
+KratosMultiphysics/MeshMovingApplication/mesh_solver_laplacian.py,sha256=iZJEB1bweM_mZpeXkhaivRZrd4cdxACXvTOJKa45_hA,1873
+KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_base.py,sha256=cOGcdcb58ZO-I7RngK5hQMGat00FzlZQHnOF6NGLOzY,3349
+KratosMultiphysics/MeshMovingApplication/mesh_solver_structural_similarity.py,sha256=CS9see7PzgOAlTXf5YXXxlmJ4aK5V3lvfxw7MaNtDvg,1685
+KratosMultiphysics/MeshMovingApplication/python_solvers_wrapper_mesh_motion.py,sha256=u1ELsL6EC-K36u6MnWY8fHhKT8RVRvk-BgKJwoJBook,2566
+KratosMultiphysics/MeshMovingApplication/ale_fluid_solver.py,sha256=ragG5SOS3EwCDWNfdit5dqM7CPkPsQBwa4QKxuZ9-Lk,10538
+KratosMultiphysics/MeshMovingApplication/mesh_moving_analysis.py,sha256=5WKqHFGR8QIHrbNKjOfoG29CkM4OJaV5VgPMleCT_bk,4135
+KratosMultiphysics/MeshMovingApplication/mesh_solver_base.py,sha256=Fyz2cPTyYZZf-d-9VzkwyyxndCwWlGx4i0_1LrBlkpo,12270
+KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_laplacian.py,sha256=U1yz8l3NZAZDjVq6tFZO_21i168FU3565eoD1czS-wg,1714
+KratosMultiphysics/MeshMovingApplication/trilinos_mesh_solver_structural_similarity.py,sha256=0fb2S9OU4STfL4xE4zzs_v7INmLRt9zOwA-SMJ8iPkY,1349
+KratosMultiphysics/MeshMovingApplication/impose_mesh_motion_process.py,sha256=h9mveA7LKFpvbjU4V5F8nWVyGEfd5tW5lQ-YCILzGqc,6397
+KratosMultiphysics/MeshMovingApplication/__init__.py,sha256=qH-YUTfyUgx0keq8i3UZZ4XMQLTgnYNA6Swy--zfG4w,236
+KratosMultiphysics/.libs/KratosMeshMovingApplication.cpython-39-x86_64-linux-gnu.so,sha256=uorJbEG7Q7v9PrW7FrN_Y4Rqk0JAzKjU2R-9txJxc2M,2682081
+KratosMultiphysics/.libs/libKratosMeshMovingCore.so,sha256=_MEVLhRUfjLuEUZ56wgvFA0ZKV__eEJrn6GpsOsmroY,5451001
+KratosMeshMovingApplication-9.5.dist-info/METADATA,sha256=r49TY9vyNj4neLyEWeQzw9cwztHe1ZY8HZg3_VRAMac,1933
+KratosMeshMovingApplication-9.5.dist-info/WHEEL,sha256=rY0Y6THYM7EImsHfF-zs67o8pQciAsMw9_YuSvftjrQ,148
+KratosMeshMovingApplication-9.5.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
+KratosMeshMovingApplication-9.5.dist-info/RECORD,,
```

